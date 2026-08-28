---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 1
section_title: Riesz spaces and fully lattice-ordered spaces
lang: vi
source: int-i-vi
pdf_pages: 0025-0032, 0039-0043
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Riesz spaces
      page: 0
      pdf_page: 25
    - "no": 2
      title: Generation of a Riesz space by its positive elements
      page: 3
      pdf_page: 27
    - "no": 3
      title: Fully lattice-ordered spaces
      page: 4
      pdf_page: 28
    - "no": 4
      title: Subspaces and product spaces of fully lattice-ordered spaces
      page: 5
      pdf_page: 29
    - "no": 5
      title: Bands in a fully lattice-ordered space
      page: 6
      pdf_page: 30
statements: 16
exercises: 12
content_sha256: be677066476dbf3cf8384795015568903ee9136525b4cf0d48570cf43694b42c
translated_from: content/en/int/II/01_s1_riesz_spaces_and_fully_lattice_ordered.md
source_content_sha256: 1c5b35994e63e08eefdec012225c55b7a20f08890336b7db13ea7edf2feca562
translation_model: gpt-5.4
translation_run: translate-vi-34b70061
glossary_version: 34
glossary_terms_sha256: 30eef11de033636e66ad8755a2000dcaead6f24788b962d9bb53c2c92a56fa4a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CÁC KHÔNG GIAN RIESZ VÀ CÁC KHÔNG GIAN ĐƯỢC SẮP THỨ TỰ DÀN ĐẦY ĐỦ

### 1. Định nghĩa các không gian Riesz

Nhắc lại rằng, trên một tập hợp E, một cấu trúc không gian vectơ trên trường $\mathbf{R}$ và một cấu trúc thứ tự được gọi là tương thích nếu chúng thỏa mãn hai tiên đề sau:

(OVS_I) *Quan hệ* $x \leq y$ *suy ra* $x + z \leq y + z$ *với mọi* $z \in E$.

(OVS_{II}) *Quan hệ* $x \geq 0$ *suy ra* $\lambda x \geq 0$ *với mọi vô hướng* $\lambda > 0$.

Không gian E, được trang bị hai cấu trúc này, được gọi là một *không gian vectơ có thứ tự* (TVS, II, §2, No. 5).

Tiên đề (OVS_I) có nghĩa là cấu trúc thứ tự và cấu trúc nhóm cộng trên E là tương thích, nói cách khác, E, được trang bị hai cấu trúc này, là một *nhóm có thứ tự* (A, VI, §1, No. 1).

Tiên đề (OVS_I) kéo theo rằng các quan hệ $x \leq y$ và $x + z \leq y + z$ là tương đương. Tương tự, từ (OVS_{II}) suy ra rằng, với mọi vô hướng $\lambda > 0$, các quan hệ $x \leq y$ và $\lambda x \leq \lambda y$ là tương đương, vì $\lambda^{-1} > 0$ và do đó quan hệ $\lambda x \leq \lambda y$ kéo theo $\lambda^{-1}(\lambda x) \leq \lambda^{-1}(\lambda y)$. Vì thế có thể nói rằng, trong một không gian vectơ có thứ tự, các phép tịnh tiến và các phép vị tự với tỷ số $> 0$ là các tự đẳng cấu của cấu trúc có thứ tự; sự kiện này cũng được diễn đạt bằng cách nói rằng thứ tự là *bất biến* dưới mọi phép tịnh tiến và mọi phép vị tự với tỷ số $> 0$. Hơn nữa, phép đối xứng $x \mapsto -x$ là một đẳng cấu từ cấu trúc có thứ tự của E lên cấu trúc có thứ tự *đối*.

#### Định nghĩa 1 {#int-ii-s1-def-1 .statement}

*Một không gian vectơ có thứ tự được gọi là một không gian Riesz (hay không gian vectơ có thứ tự dàn)*$^1$ *nếu cấu trúc thứ tự của nó là một thứ tự dàn* (nghĩa là, nếu mọi cặp phần tử $x, y$ của E đều có một cận trên $\sup(x, y)$ và một cận dưới $\inf(x, y)$ ).$^2$

\footnotetext{
$^1$ Cũng được gọi là một "dàn vectơ".
$^2$ Borne supérieure (supremum) cũng còn được dịch là "cận trên bé nhất" (S, R, §6, 7). Tương tự, borne inférieure (infimum) cũng còn được dịch là "cận dưới lớn nhất".
}

#### Ví dụ {#int-ii-s1-n1-exa-1 .statement}

Không gian $\mathbf{R}^A$ của mọi hàm thực xác định trên một tập hợp bất kỳ $A$ là một không gian Riesz (đối với quan hệ thứ tự $\langle x(t) \leq y(t) \text{ với mọi } t \in A \rangle$); thật vậy, hai hàm thực bất kỳ $x, y$ xác định trên $A$ đều có một cận trên (resp. một cận dưới) bằng ánh xạ $t \mapsto \sup(x(t), y(t))$ (resp. $t \mapsto \inf(x(t), y(t))$).

Cũng có thể nói rằng một không gian Riesz là một không gian vectơ $E$ được trang bị một cấu trúc thứ tự sao cho, một mặt, cấu trúc này và cấu trúc nhóm cộng của $E$ xác định trên $E$ một cấu trúc *nhóm có thứ tự dàn* (A, VI, §1, No. 9), và mặt khác tiên đề (OVS$_{\mathrm{II}}$) được thỏa mãn.

Do đó, mọi tính chất của các nhóm có thứ tự dàn đều áp dụng được cho các không gian Riesz; ở đây chúng tôi sẽ nhắc lại những tính chất chính ấy (x. A, VI, §1, Nos. 9 to 12), đồng thời chỉ ra những hệ quả suy ra từ tiên đề (OVS$_{\mathrm{II}}$).

Trước hết nhắc lại rằng ta viết $x^+ = \sup(x, 0)$ (*phần dương* của $x$), $x^- = (-x)^+ = \sup(-x, 0)$ (*phần âm* của $x$), $|x| = \sup(x, -x)$ (*giá trị tuyệt đối* của $x$); khi đó $x = x^+ - x^-$ và $|x| = x^+ + x^-$; ở đây, hai hệ thức này tương đương với

$$
x^+ = \frac{1}{2}(|x| + x), \quad x^- = \frac{1}{2}(|x| - x).
$$

Quan hệ $x \leq y$ tương đương với $\langle x^+ \leq y^+ \text{ và } x^- \geq y^- \rangle$. Với mọi $x$ và $y$, *bất đẳng thức tam giác* được thỏa mãn:

(1)
$$
|x + y| \leq |x| + |y|.
$$

Do tính bất biến của cấp dưới mọi phép vị tự có tỉ số $> 0$,

(2)
$$
\sup(\lambda x, \lambda y) = \lambda \sup(x, y) \quad \text{với mọi } \lambda \geq 0.
$$

Đặc biệt,

(3)
$$
(\lambda x)^+ = \lambda x^+, \quad (\lambda x)^- = \lambda x^- \quad \text{với mọi } \lambda \geq 0.
$$

Mặt khác, với $\lambda < 0$ ta có $(\lambda x)^+ = (-\lambda x)^- = |\lambda| x^-$ và $(\lambda x)^- = (-\lambda x)^+ = |\lambda| x^+$; suy ra rằng, với mọi $\lambda \in \mathbf{R}$ và mọi $x \in E$,

(4)
$$
|\lambda x| = |\lambda| \cdot |x|.
$$

Tính bất biến của cấp dưới phép tịnh tiến cho thấy rằng với mọi $z \in E$,

(5)
$$
\sup(x + z, y + z) = z + \sup(x, y),
$$
do đó, đặc biệt,

(6)
$$
\sup(x, y) = x + (y - x)^+ = \frac{1}{2}(x + y + |x - y|).
$$

Ta có các hệ thức

(7)    $\inf(x, y) = -\sup(-x, -y) ,$

(8)    $\sup(x, y) + \inf(x, y) = x + y .$

Nếu $x, y, z$ là $\geq 0$ thì (A, VI, §1, No. 12, Prop. 11)

(9)    $\inf(x + y, z) \leq \inf(x, z) + \inf(y, z) .$

Nếu A và B là hai tập con của E mà mỗi tập đều có một cận trên đúng, thì A + B cũng có một cận trên đúng và

(10)    $\sup(A + B) = \sup A + \sup B .$

Hai phần tử $x, y$ của E được gọi là rời nhau$^3$ (đối với nhau) nếu $\inf(|x|, |y|) = 0$; theo (8), quan hệ này tương đương với $\sup(|x|, |y|) = |x| + |y|$, và cũng, theo (6), tương đương với $||x| - |y|| = |x| + |y|$; 0 là phần tử duy nhất rời nhau với chính nó; với mọi $x \in E$, $x^+$ và $x^-$ rời nhau và có thể được đặc trưng như là các phần tử rời nhau duy nhất $y \geq 0, z \geq 0$ sao cho $x = y - z$. Nếu $y$ rời nhau với $x$, thì mọi $z \in E$ sao cho $|z| \leq |y|$ cũng rời nhau với $x$. Nếu $y$ và $z$ rời nhau với $x$, thì $|y| + |z|$ cũng vậy, theo bất đẳng thức (9); đặc biệt, $n|y|$ rời nhau với $x$ với mọi số nguyên $n > 0$, từ đó suy ra rằng $\lambda y$ rời nhau với $x$ với mọi vô hướng $\lambda$, vì tồn tại một số nguyên $n$ sao cho $|\lambda| \leq n$, do đó $|\lambda y| \leq n|y|$. Nếu một tập con A của E gồm các phần tử rời nhau với $x$ và nếu A có một cận trên đúng, thì cận trên đúng đó cũng rời nhau với $x$ (A, VI, §1, No. 12, Hệ quả của Mệnh đề 13).

Sau cùng, ta có bổ đề phân tích (A, VI, §1, No. 10, Đl. 1):

*Nếu* $(x_i)_{i \in I}, (y_j)_{j \in J}$ *là hai dãy hữu hạn các phần tử* $\geq 0$ *của E sao cho* $\sum_{i \in I} x_i = \sum_{j \in J} y_j$, *thì tồn tại một dãy hữu hạn* $(z_{ij})_{(i,j) \in I \times J}$ *các phần tử* $\geq 0$ *của E sao cho* $x_i = \sum_{j \in J} z_{ij}$ *với mọi* $i \in I$, *và* $y_j = \sum_{i \in I} z_{ij}$ *với mọi* $j \in J$.

### 2. Sinh một không gian Riesz bởi các phần tử dương của nó

Cho E là một không gian vectơ có thứ tự; tập P các phần tử $\geq 0$ của E là một nón lồi có đỉnh 0, nghĩa là (TVS, II, §2, No. 4), một tập hợp sao cho

$^3$ Nguyên bản là étrangers, cũng được dịch là "coprime" (A, VI, §1, No. 12); các thuật ngữ "orthogonal", "disjoint" và "mutually singular" cũng được dùng.

P + P ⊂ P và λP ⊂ P với mọi λ > 0. Ngược lại, nếu trong một không gian vectơ E trên $\mathbf{R}$, P là một nón lồi có đỉnh 0 sao cho $P \cap (-P) = \{0\}$ (nói cách khác, một nón lồi *nhọn* và *thực sự*), thì người ta biết (*loc. cit.*) rằng quan hệ $y - x \in P$ là một quan hệ thứ tự (ký hiệu $x \leq y$) tương thích với cấu trúc không gian vectơ của E. Để cấu trúc thứ tự này xác định trên E một cấu trúc *không gian Riesz*, điều kiện cần và đủ là:

$1^\circ$ P sinh ra E, nghĩa là, mọi $z \in E$ đều có dạng $y - x$, trong đó x và y thuộc P;

$2^\circ$ P thỏa mãn một trong hai điều kiện sau đây:
a) mọi cặp phần tử của P đều có một cận trên đúng trong P;
b) mọi cặp phần tử của P đều có một cận dưới đúng trong P (A, VI, §1, No. 9, Mệnh đề 8).

### 3. Không gian được sắp thứ tự đầy đủ theo dàn

#### Định nghĩa 2 {#int-ii-s1-def-2 .statement}

*Một không gian Riesz E được gọi là được sắp thứ tự đầy đủ theo dàn nếu mọi tập con khác rỗng của E bị chặn trên đều có một cận trên đúng trong E.*

Ngay lập tức thấy rằng trong một không gian được sắp thứ tự đầy đủ theo dàn E, mọi tập con khác rỗng bị chặn dưới đều có một cận dưới đúng trong E.

#### Ví dụ {#int-ii-s1-n3-exa-1 .statement}

— 1) Nếu A là một tập hợp bất kỳ, thì không gian $\mathbf{R}^A$ các hàm nhận giá trị thực xác định trên A là được sắp thứ tự đầy đủ theo dàn, cận trên đúng trong $\mathbf{R}^A$ của một họ bị chặn trên là *bao trên* của nó (GT, IV, §5, No. 5).

2) Cho F là một tập hợp bất kỳ; không gian $\mathcal{B}(F)$ các hàm *bị chặn* nhận giá trị thực trên F, được trang bị cấu trúc thứ tự cảm sinh bởi cấu trúc thứ tự của $\mathbf{R}^F$, là có cấu trúc dàn đầy đủ. Tuy nhiên, nếu F là một không gian tôpô, thì không gian $\mathcal{C}(F)$ các hàm *liên tục* nhận giá trị thực trên F (được trang bị cấu trúc thứ tự cảm sinh bởi cấu trúc thứ tự của $\mathbf{R}^F$) là một không gian Riesz nói chung không có cấu trúc dàn đầy đủ (x. Bài tập 13). Chẳng hạn, xét trường hợp $F = \mathbf{R}$; gọi I là khoảng ]0, 1[, $\varphi_I$ là hàm đặc số của I, và gọi H là tập hợp các hàm liên tục $x(t)$ sao cho $x \leq \varphi_I$; hiển nhiên H bị chặn trên trong $\mathcal{C}(F)$. Hàm $\varphi_I$ là *bao trên* của các $x \in H$, nhưng nó không phải là cận trên bé nhất của chúng trong $\mathcal{C}(F)$, vì $\varphi_I$ là nửa liên tục dưới nhưng không liên tục. Ta hãy chỉ ra rằng, thực ra, H không có cận trên bé nhất trong $\mathcal{C}(F)$; chỉ cần chứng minh rằng nếu $u$ là một hàm liên tục sao cho $u \geq \varphi_I$, thì tồn tại một hàm liên tục $v \neq u$ sao cho $u \geq v \geq \varphi_I$. Thật vậy, $u(0) \geq 1$, do đó tồn tại một số $\alpha > 0$ sao cho $u(t) > 0$ với $-\alpha \leq t \leq 0$; nếu w là một hàm liên tục bằng không ở ngoài khoảng ]$-\alpha, 0$ và sao cho $0 < w(t) < u(t)$ trên khoảng này, thì hàm $v = u - w$ thỏa các điều kiện ấy.

#### Mệnh đề 1 {#int-ii-s1-prop-1 .statement}

*Để một không gian vectơ có thứ tự E được sắp thứ tự dàn đầy đủ, điều kiện cần và đủ là E là một không gian Riesz và thỏa mãn một trong hai điều kiện sau đây:*

a) *mọi tập con khác rỗng A, gồm các phần tử $\geq 0$ của E, bị chặn trên và có hướng đối với quan hệ $\leq$, đều có một cận trên đúng trong E;*

b) *mọi tập con khác rỗng* $A$, *gồm các phần tử* $\geqslant 0$ *của* $E$ *và có hướng đối với quan hệ* $\geqslant$, *đều có một cận dưới đúng trong* $E$.

Các điều kiện ấy hiển nhiên là cần thiết. Ngược lại, giả sử rằng $E$ là một không gian Riesz thỏa mãn điều kiện *a)*. Cho $B$ là một tập con khác rỗng của $E$ bị chặn trên; tập hợp $C$ gồm các cận trên đúng của các tập con hữu hạn của $B$ là có hướng đối với quan hệ $\leqslant$; gọi $a$ là một phần tử của nó và $C_a$ là tập hợp các $x \in C$ mà $\geqslant a$; nếu ta chứng minh được rằng $C_a$ có một cận trên đúng thì cận trên đúng đó cũng sẽ là cận trên đúng của $B$. Bây giờ, $C_a - a$ là một tập hợp các phần tử $\geqslant 0$, bị chặn trên và có hướng đối với quan hệ $\leqslant$; do đó nó có một cận trên đúng $b$, do đó $a + b$ là cận trên đúng của $C_a$.

Mặt khác, điều kiện *b)* suy ra *a)*: thật vậy, nếu $F$ là một tập hợp khác rỗng gồm các phần tử $\geqslant 0$ của $E$, bị chặn trên và có hướng đối với $\leqslant$, và nếu $c$ là một cận trên của $F$, thì $c - F$ là một tập hợp gồm các phần tử $\geqslant 0$ có hướng đối với $\geqslant$; nếu nó có một cận dưới đúng $m$, thì $c - m$ là cận trên đúng của $F$.

#### Mệnh đề 2 {#int-ii-s1-prop-2 .statement}

— *Cho* $E$ *là một không gian Riesz được trang bị một tôpô Hausdorff tương thích với cấu trúc không gian vectơ có thứ tự của nó* (TVS, II, §2, No. 7). *Nếu, với mọi tập hợp* $H \subset E$ *bị chặn trên và có hướng đối với quan hệ* $\leqslant$, *bộ lọc tiết diện của* $H$ *hội tụ, thì* $E$ *có thứ tự dàn đầy đủ*.

Thật vậy, ta biết rằng giới hạn của bộ lọc tiết diện của $H$ là cận trên đúng của $H$ trong $E$ (TVS, II, §2, No. 7, Mệnh đề 18).

### 4. Không gian con và không gian tích của các không gian có thứ tự dàn đầy đủ

Cho $E$ là một không gian có thứ tự dàn đầy đủ, $H$ là một không gian con tuyến tính của $E$. Cấu trúc thứ tự cảm sinh trên $H$ bởi cấu trúc thứ tự của $E$ tương thích với cấu trúc không gian vectơ của $H$, nhưng không gian vectơ có thứ tự $H$ được xác định như vậy *không nhất thiết là một không gian có thứ tự dàn đầy đủ*.

Chính xác hơn, có thể xảy ra là $H$ không phải là một không gian Riesz (Bài tập 2), hoặc $H$ là một không gian Riesz nhưng không được sắp thứ tự dàn đầy đủ: trường hợp sau xảy ra đối với không gian con $\mathcal{C}(\mathbf{R})$ của không gian $\mathcal{B}(\mathbf{R})$ (No. 3, Ví dụ 2).

Hơn nữa, nếu $H$ là một không gian Riesz (có thứ tự dàn đầy đủ hay không) thì có thể xảy ra việc cận trên đúng *trong* $H$ của hai phần tử của $H$ khác với cận trên đúng của chúng *trong* $E$ (Bài tập 3 *b*). Cuối cùng, có thể xảy ra rằng $H$ có thứ tự dàn đầy đủ, rằng cận trên đúng của mỗi tập con *hữu hạn* của $H$ là như nhau trong $E$ và trong $H$, nhưng lại tồn tại những tập con *vô hạn* của $H$, bị chặn trên trong $H$, mà các cận trên đúng trong $E$ và $H$ là khác nhau (Bài tập 13 *f*)).

Cho $(E_\iota)_{\iota \in I}$ là một họ bất kỳ các không gian vectơ có thứ tự. Nhắc lại rằng, trong không gian tích $E = \prod_{\iota \in I} E_\iota$, quan hệ thứ tự *tích* của các quan hệ thứ tự của các không gian nhân tử là quan hệ $« x_\iota \leqslant y_\iota \text{ với mọi } \iota \in I »$ (S, III, §1, No. 4). Người ta kiểm tra ngay lập tức rằng quan hệ này tương thích với cấu trúc không gian vectơ của E; E, được trang bị cấu trúc này, được gọi là không gian tích của các không gian có thứ tự $E_\iota$.

#### Mệnh đề 3 {#int-ii-s1-prop-3 .statement}

*Cho $(E_\iota)_{\iota \in I}$ là một họ các không gian vectơ có thứ tự. Để không gian tích $E = \prod_{\iota \in I} E_\iota$ là một không gian Riesz (tương ứng là một không gian có cấu trúc dàn đầy đủ), điều kiện cần và đủ là mỗi không gian $E_\iota$ đều là một không gian Riesz (tương ứng là một không gian có cấu trúc dàn đầy đủ).*

Hãy giới hạn ở việc khảo sát trường hợp các không gian có thứ tự dàn đầy đủ. Giả sử rằng tất cả các $E_\iota$ đều có thứ tự dàn đầy đủ; gọi $A$ là một tập con khác rỗng của $E$ bị chặn trên và gọi $a = (a_\iota)$ là một cận trên của $A$. Với mọi $\iota \in I$, $\operatorname{pr}_\iota A$ bị chặn trên bởi $a_\iota$, nên có một cận trên đúng $b_\iota$ trong $E_\iota$; hiển nhiên $b = (b_\iota)$ là cận trên đúng của $A$ trong $E$.

Ngược lại, giả sử $E$ có thứ tự dàn đầy đủ. Gọi $A_\kappa$ là một tập con của $E_\kappa$ bị chặn trên, $A'_\kappa$ là tập con của $E$ gồm các $x = (x_\iota)$ sao cho $x_\kappa \in A_\kappa$ và $x_\iota = 0$ với $\iota \neq \kappa$. Ngay lập tức thấy rằng $A'_\kappa$ bị chặn trên trong $E$, do đó có một cận trên đúng $b = (b_\iota)$; theo định nghĩa của quan hệ thứ tự tích, tất yếu $b_\iota = 0$ với $\iota \neq \kappa$, và $b_\kappa$ là cận trên đúng của $A_\kappa$, điều này hoàn tất chứng minh.

#### Định nghĩa 3 {#int-ii-s1-def-3 .statement}

*Cho $E$ là một không gian vectơ có thứ tự, $V$ và $W$ là hai không gian con tuyến tính bù nhau của $E$. Ta nói rằng $E$ là tổng trực tiếp có thứ tự của $V$ và $W$ nếu ánh xạ chính tắc $(x, y) \mapsto x + y$ từ không gian vectơ có thứ tự $V \times W$ lên không gian vectơ có thứ tự $E$ là một đẳng cấu.*

#### Mệnh đề 4 {#int-ii-s1-prop-4 .statement}

*Để một không gian vectơ có thứ tự $E$ là tổng trực tiếp có thứ tự của hai không gian con tuyến tính bù nhau $V, W$, điều kiện cần và đủ là các hệ thức $x \in V, y \in W, x + y \geq 0$ kéo theo $x \geq 0$ và $y \geq 0$.*

Vì $x \geq 0$ và $y \geq 0$ kéo theo $x + y \geq 0$ trong $E$, điều kiện trong mệnh đề nói rằng $(x, y) \mapsto x + y$ biến tập hợp các phần tử $\geq 0$ của $V \times W$ thành tập hợp các phần tử $\geq 0$ của $E$.

### 5. Các dải trong một không gian được sắp thứ tự dàn đầy đủ

#### Định nghĩa 4 {#int-ii-s1-def-4 .statement}

*Trong một không gian được sắp thứ tự dàn đầy đủ $E$, một không gian con tuyến tính $B$ của $E$ được gọi là một dải nếu nó thỏa mãn các điều kiện sau: 1) các quan hệ $x \in B, y \in E$ và $|y| \leq |x|$ suy ra $y \in B$; 2) với mọi tập con khác rỗng $X$ của $B$ bị chặn trên trong $E$, cận trên đúng $\sup X$ của $X$ trong $E$ thuộc về $B$.*

#### Ví dụ {#int-ii-s1-n5-exa-1 .statement}

— Trong không gian $\mathbf{R}^A$ các hàm thực xác định trên một tập hợp $A$, tập hợp các hàm bằng không tại mọi điểm của một tập con $M$ của $A$ là một băng.

#### Nhận xét {#int-ii-s1-n5-rem-1 .statement}

— Trong không gian $\mathbf{R}^A$, không gian con $\mathcal{B}(A)$ của các hàm thực bị chặn trên $A$ thỏa mãn điều kiện 1) của Định nghĩa 4; hơn nữa, với mọi tập con $X$ của $\mathcal{B}(A)$ bị chặn trên *trong* $\mathcal{B}(A)$, bao trên của $X$ thuộc $\mathcal{B}(A)$. Tuy nhiên, nếu $A$ là vô hạn, một tập con của $\mathcal{B}(A)$ có thể *bị chặn trên trong* $\mathbf{R}^A$ *mà không bị chặn trên trong* $\mathcal{B}(A)$, trong trường hợp đó $\mathcal{B}(A)$ không phải là một dải trong $\mathbf{R}^A$.

Suy ra ngay từ Định nghĩa 4 rằng nếu $B$ là một dải trong $E$ thì, với mọi tập con khác rỗng $X$ của $B$ bị chặn dưới trong $E$, $\inf X$ thuộc $B$. Mọi dải $B$ trong $E$, được trang bị cấu trúc không gian vectơ có thứ tự cảm sinh bởi cấu trúc của $E$, đều là một không gian có thứ tự dàn đầy đủ và, với mọi tập con $X \subset B$ bị chặn trên trong $B$, cận trên đúng của $X$ trong $B$ trùng với cận trên đúng của nó trong $E$.

Giao của mọi họ các dải trong một không gian dàn có thứ tự đầy đủ $E$ cũng là một dải. Với mọi tập con $M \subset E$, tồn tại một *dải nhỏ nhất* chứa $M$ (vì chính $E$ là một dải); dải này sẽ được gọi là dải được *sinh* bởi $M$.

Các tính chất của các dải trong một không gian dàn có thứ tự đầy đủ dựa trên mệnh đề sau:

#### Mệnh đề 5 {#int-ii-s1-prop-5 .statement}

— *Cho $E$ là một không gian dàn có thứ tự đầy đủ, $A$ là một tập con không rỗng của $E$ gồm các phần tử $\geqslant 0$, sao cho: 1) $A + A \subset A$, và 2) các quan hệ $x \in A,\ 0 \leqslant y \leqslant x$ kéo theo $y \in A$. Gọi $M$ là tập hợp các cận trên đúng trong $E$ của những tập con của $A$ bị chặn trên trong $E$. Với các điều kiện đó, mọi phần tử $x \geqslant 0$ của $E$ đều có thể viết dưới dạng $y + z$, trong đó $y \in M$ là cận trên đúng của các phần tử $v \in A$ sao cho $v \leqslant x$, và trong đó $z$ là một phần tử $\geqslant 0$ xa lạ với mọi phần tử của $M$.*

Dù sao đi nữa, $y \leqslant x$, nên toàn bộ vấn đề quy về việc chỉ ra rằng $z = x - y$ là ngoại lai với mọi phần tử $t \in A$ (No. 1), nói cách khác rằng $u = \inf(z, t)$ là không. Theo giả thiết, $u \in A$ và $u \leqslant x - y$, do đó $u + y \leqslant x$; với mọi $v \in A$ sao cho $v \leqslant x$, theo định nghĩa ta có $v \leqslant y$, do đó $u + v \leqslant u + y \leqslant x$; vì $u + v \in A$ theo giả thiết, nên cũng có $u + v \leqslant y$ theo định nghĩa của $y$; sau cùng, vì $u + y$ là cận trên đúng trong $E$ của các phần tử $u + v$ sao cho $v \in A$ và $v \leqslant x$, ta có $u + y \leqslant y$, do đó $u \leqslant 0$, điều này hoàn tất chứng minh.

#### Định lý 1 (F. Riesz) {#int-ii-s1-thm-1 .statement}

— *Cho $A$ là một tập con của một không gian có thứ tự dàn đầy đủ $E$. Tập $A'$ gồm các phần tử xa lạ với mọi phần tử của $A$ là một dải; dải $A''$ gồm các phần tử xa lạ với mọi phần tử của $A'$ trùng với dải sinh bởi $A$, và $E$ là tổng trực tiếp có thứ tự của các dải $A'$ và $A''$.*

Các tính chất của các phần tử xa lạ, đã được xét lại ở No. 1, và định nghĩa của một dải, cho thấy ngay rằng $A'$ là một dải, do đó $A''$ cũng vậy. Theo Mệnh đề 5 và định nghĩa của một dải, mọi phần tử $x \geqslant 0$ của $E$ đều có thể viết dưới dạng $x = y + z$, với $y \in A'$ và $z \in A''$, trong đó $y$ và $z$ đều $\geqslant 0$; vì mọi phần tử của $E$ là hiệu của hai phần tử $\geqslant 0$, nên ta có $E = A' + A''$; mặt khác, vì $0$ là phần tử duy nhất xa lạ với chính nó, nên ta có $A' \cap A'' = \{0\}$, điều này chứng minh rằng $E$ là tổng trực tiếp của $A'$ và $A''$; cuối cùng, vì các thành phần trong $A'$ và $A''$ của một phần tử $\geqslant 0$ của $E$ đều $\geqslant 0$, nên $E$ là tổng trực tiếp có thứ tự của $A'$ và $A''$ (No. 4, Mệnh đề 4).

Còn phải chỉ ra rằng $A''$ đồng nhất với dải $B$ sinh bởi $A$. Thật vậy, $E$ là tổng trực tiếp của $B$ và dải $B'$ tạo bởi các phần tử xa lạ với mọi phần tử của $B$; vì $A \subset B$, ta có $B' \subset A'$; mặt khác $B \subset A''$ và $E$ cũng là tổng trực tiếp của $A'$ và $A''$; do đó tất yếu $B = A''$, $B' = A'$.

Định lý 1 và Mệnh đề 5 làm cho có thể đưa ra một định nghĩa khác của dải sinh bởi một tập hợp các phần tử của $E$:

#### Mệnh đề 6 {#int-ii-s1-prop-6 .statement}

— *Cho $E$ là một không gian có thứ tự dàn đầy đủ, $M$ là một tập con của $E$, và $B$ là dải sinh bởi $M$. Gọi $M_1$ là tập hợp các phần tử $\geqslant 0$ của $E$ mà mỗi phần tử đều $\leqslant$ một phần tử nào đó có dạng $\sum_i |x_i|$, trong đó $x_i \in M$; gọi $M_2$ là tập hợp các cận trên đúng của những tập con của $M_1$ bị chặn trên; khi đó tập hợp $M_2$ trùng với tập hợp các phần tử $\geqslant 0$ của $B$.*

Rõ ràng $M_2 \subset B$ theo định nghĩa của một band; mặt khác, nếu $B'$ là band của các phần tử xa lạ với mọi phần tử của $M_1$, Định lý 1 cho thấy rằng $E$ là tổng trực tiếp có thứ tự của $B$ và $B'$. Nhưng Mệnh đề 5 cho thấy rằng mọi phần tử $\geqslant 0$ của $E$ đều là tổng của một phần tử của $M_2$ và một phần tử của $B'$, do đó suy ra mệnh đề.

#### Hệ quả {#int-ii-s1-n5-cor-1 .statement}

— *Cho $a$ là một phần tử của một không gian dàn có thứ tự đầy đủ $E$, $B_a$ là dải sinh bởi $a$, $B'_a$ là dải các phần tử rời nhau với $a$. Với mọi phần tử $x \geqslant 0$ của $E$, thành phần của $x$ trong $B_a$ (đối với phân tích của $E$ thành tổng trực tiếp có thứ tự của $B_a$ và $B'_a$) bằng $\sup_{n \in \mathbf{N}} (\inf(n|a|, x))$.*

Điều này suy ra từ Mệnh đề 6, áp dụng cho $M = \{a\}$, và Mệnh đề 5.

Chú ý rằng các dải sinh bởi $a$ và $|a|$ là đồng nhất. Nếu $a$ và $b$ là hai phần tử của $E$ xa lạ với nhau, và nếu $A$ và $B$ lần lượt là các dải sinh bởi $a$ và $b$, thì mọi phần tử của $A$ đều xa lạ với mọi phần tử của $B$; thật vậy, $b$ thuộc về dải $A'$ gồm các phần tử xa lạ với $a$, do đó $B \subset A'$, và, theo Định lý 1, mọi phần tử của $A$ đều xa lạ với mọi phần tử của $A'$.

### Bài tập {#int-ii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
