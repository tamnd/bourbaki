---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 1
section_title: Prehilbertian spaces and hilbertian spaces
lang: vi
source: evt-i-v
pdf_pages: 0259-0275, 0318-0328
extraction: ocr
subsections:
    - "no": 1
      title: Hermitian forms
      page: 0
      pdf_page: 259
    - "no": 2
      title: Positive hermitian forms
      page: 2
      pdf_page: 260
    - "no": 3
      title: Prehilbertian spaces
      page: 4
      pdf_page: 262
    - "no": 4
      title: Hilbertian spaces
      page: 6
      pdf_page: 264
    - "no": 5
      title: Convex subsets of a prehilbertian space
      page: 9
      pdf_page: 267
    - "no": 6
      title: Vector subspaces and orthoprojectors
      page: 12
      pdf_page: 270
    - "no": 7
      title: Dual of a hilbertian space
      page: 15
      pdf_page: 273
statements: 41
exercises: 6
content_sha256: 5225c61ea5dc1a952d38fe07735c8588075848460b3c57f5fb8d179cac224f66
translated_from: content/en/evt/V/01_s1_prehilbertian_spaces_and_hilbertian.md
source_content_sha256: 4bfeeee4e5c1a6ce99f5c929d436d1d7c6606ff2f9558da7d47b0ffdba15c626
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-f0b45ea2
glossary_version: 34
glossary_terms_sha256: 3c6226fc075229ab034ae45c5df9a3887f08fbb64f972d7fc50a2b31e4861576
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. KHÔNG GIAN TIỀN HILBERT VÀ KHÔNG GIAN HILBERT

### 1. Các dạng Hermit

Ta nhắc lại định nghĩa sau đã cho trong Đại số (A, IX, § 3, No. 1):

#### Định nghĩa 1 {#evt-v-s1-def-1 .statement}

Cho E là một không gian vectơ trên trường K. Một dạng Hermit (trái) trên E là một ánh xạ f từ E × E vào K thỏa mãn các điều kiện sau (với $x_1, x_2, x, y_1, y_2, y$ trong E và $\lambda, \mu$ trong K):

(1)
$$
\begin{cases}
f(x_1 + x_2, y) = f(x_1, y) + f(x_2, y) \\
f(x, y_1 + y_2) = f(x, y_1) + f(x, y_2)
\end{cases}
$$

(2)
$$
\begin{cases}
f(\lambda x, y) = \overline{\lambda} f(x, y) \\
f(x, \mu y) = \mu f(x, y)
\end{cases}
$$

(3)
$$
f(x, y) = \overline{f(y, x)} .
$$

Khi trường K là R, khái niệm dạng Hermit trên E quy về khái niệm dạng song tuyến tính đối xứng trên E × E (A, III, § 6, No. 3).

Ta ghi nhận rằng điều kiện thứ hai của (1) và điều kiện thứ hai của (2) suy ra từ ba điều kiện còn lại.

¹ Đối với bạn đọc đặc biệt quan tâm đến các không gian Hilbert, chúng tôi xin chỉ ra rằng chỉ No. 7 của § 1 và No. 8 của § 4 phụ thuộc vào các kết quả của các chương III và IV. Về điều này bạn đọc có thể tham khảo « Tóm tắt một số tính chất quan trọng của không gian Banach » xuất hiện ở cuối tập này. Những chỗ dẫn chiếu duy nhất đến các chương I và II liên quan đến định nghĩa của một tập lồi và của một nửa chuẩn (II, p. 1 và p. 7), của một tổng trực tiếp tôpô (I, p. 4), của một họ đầy đủ và một họ độc lập tôpô (I, p. 12).

Từ (1) và (2) ta suy ra ngay rằng

$$
f(\sum_j \lambda_j x_j, \sum_k \mu_k y_k) = \sum_{j,k} \overline{\lambda}_j \mu_k f(x_j, y_k).
$$

Đặc biệt, nếu E hữu hạn chiều, và nếu $(e_j)_{1 \leq j \leq n}$ là một cơ sở của E, thì với $x = \sum_{j=1}^n \xi_j e_j$ và $y = \sum_{j=1}^n \eta_j e_j$, ta có,

$$
f(x, y) = \sum_{j,k} \alpha_{jk} \overline{\xi}_j \eta_k
$$

với ký hiệu $\alpha_{jk} = f(e_j, e_k)$; hơn nữa, quan hệ (3) tương đương với $\alpha_{jk} = \overline{\alpha}_{kj}$ với mọi cặp chỉ số $j, k$; điều này suy ra đặc biệt rằng các số $\alpha_{jj}$ là thực.

Từ (3), số $Q(x) = f(x, x)$ là thực với mọi $x \in E$. Hơn nữa, ta ngay lập tức thiết lập các công thức sau, gọi là *công thức phân cực*

(5)
$$
4f(x, y) = \sum_{\varepsilon^2 = 1} \varepsilon Q(x + \varepsilon y) \quad \text{nếu } K \text{ là } \mathbf{R},
$$
(6)
$$
4f(x, y) = \sum_{\varepsilon^4 = 1, \varepsilon \in \mathbf{C}} \varepsilon Q(x + \overline{\varepsilon} y) \quad \text{nếu } K \text{ là } \mathbf{C}.
$$

#### Nhận xét {#evt-v-s1-n1-rem-1 .statement}

— Ta nhận thấy rằng công thức (6) đúng cho mọi dạng *nửa song tuyến tính* trên $E \times E$ (tức là, cho mọi hàm $f$ thỏa mãn (1) và (2), nhưng không nhất thiết (3)). Nhận xét này cho thấy rằng, khi $K = \mathbf{C}$, một dạng *nửa song tuyến tính* $f$ sao cho $f(x, x)$ là thực với mọi $x \in E$ thì tất yếu *Hermit*: quan hệ (6) khi đó cho $\overline{f(y, x)} = f(x, y)$ vì ta có $y + \varepsilon x = \varepsilon(x + \overline{\varepsilon} y)$ và $Q(\varepsilon z) = Q(z)$ mỗi khi $\varepsilon^4 = 1$.

Từ các công thức phân cực, đặc biệt ta có,

#### Mệnh đề 1 {#evt-v-s1-prop-1 .statement}

*Nếu $f$ là một dạng Hermit trên $E$, và $M$ là một không gian con vectơ của $E$ sao cho $f(x, x) = 0$ với mọi $x \in M$, thì ta cũng có $f(x, y) = 0$ với mọi cặp điểm $x, y$ trong $M$.*

Cho $f$ là một dạng Hermit trên $E$; tập hợp $N$ gồm mọi $x \in E$ sao cho $f(x, y) = 0$ với mọi $y \in E$ là một không gian con vectơ của $E$. Từ (3) suy ra rằng, nếu $x_1 \equiv x_2$ (mod. $N$) và $y_1 \equiv y_2$ (mod. $N$), ta có $f(x_1, y_1) = f(x_2, y_2)$; do đó, trên không gian thương $E/N$ ta định nghĩa một dạng sesquilinear $f$ bằng cách đặt $f(\dot{x}, \dot{y}) = f(x, y)$ với mọi $x \in \dot{x}$ và mọi $y \in \dot{y}$; rõ ràng rằng $f$ là Hermit và quan hệ «$f(\dot{x}, \dot{y}) = 0$ với mọi $\dot{y} \in E/N$» kéo theo $\dot{x} = 0$ trong $E/N$, nói cách khác (A, IX) $f$ là tách được. Ta nói rằng $f$ là dạng Hermit *tách được* *liên kết* với $f$.

### 2. Các dạng Hermit dương

#### Định nghĩa 2 {#evt-v-s1-def-2 .statement}

*Cho $E$ là một không gian vectơ trên trường $K$. Một dạng Hermit $f$ trên $E$ được gọi là dương nếu $f(x, x) \geq 0$ với mọi $x \in E$.*

Rõ ràng rằng các dạng Hermit trên một không gian vectơ $E$ tạo thành một không gian vectơ *trên trường* $\mathbf{R}$ (nhưng không trên trường $\mathbf{C}$, khi $K$ là $\mathbf{C}$) : trong không gian này các dạng Hermit dương tạo thành *một nón lồi thực sự nhọn* (II, p. 10) như là kết quả của định nghĩa 2 và mệnh đề 1.

#### Mệnh đề 2 {#evt-v-s1-prop-2 .statement}

— *Nếu f là một dạng Hermit dương, ta có*

$$
|f(x, y)|^2 \leq f(x, x) \ f(y, y)
$$

*đối với mọi x và y trong E* (bất đẳng thức Cauchy-Schwarz).

Trước hết giả sử rằng ta có $f(y, y) \neq 0$. Với mọi $\xi \in \mathbf{K}$, ta có

$$
f(y, y) \ f(x + \xi y, x + \xi y) \geq 0
$$

có thể được viết dưới dạng

$$
f(x, x) \ f(y, y) - |f(x, y)|^2 + (\xi f(y, y) + \overline{f(x, y)}) (\overline{\xi} f(y, y) + f(x, y)) \geq 0 .
$$

Thay thế $\xi$ bởi $-\overline{f(x, y)}/f(y, y)$ trong bất đẳng thức này, ta thu được (7). Nếu $f(x, x) \neq 0$, ta lập luận tương tự.

Cuối cùng, nếu $f(x, x) = f(y, y) = 0$, ta có $f(x + \xi y, x + \xi y) \geq 0$ với mọi $\xi \in \mathbf{K}$, điều này có thể được viết dưới dạng

$$
\xi f(x, y) + \overline{\xi} f(x, y) \geq 0 .
$$

Thay thế $\xi$ bởi $-\overline{f(x, y)}$ trong bất đẳng thức này, ta thu được $-2 \ |f(x, y)|^2 \geq 0$, và do đó $f(x, y) = 0$; trong trường hợp này ta lại thu được (7).

#### Hệ quả 1 {#evt-v-s1-prop-2-cor-1 .statement}

— *Nếu f là một dạng Hermit dương, tập hợp N gồm mọi x \in E sao cho f(x, x) = 0 trùng với không gian con vectơ gồm mọi x \in E sao cho f(x, y) = 0 với mọi y \in E.*

#### Hệ quả 2 {#evt-v-s1-prop-2-cor-2 .statement}

— *Để một dạng Hermit dương là tách được, điều kiện cần và đủ là quan hệ x \neq 0 kéo theo f(x, x) > 0.*

Điều này suy ra ngay lập tức từ hệ quả 1.

Đối với mọi dạng Hermit dương f trên E, dạng Hermit tách được liên kết với f (V, p. 2) hiển nhiên là một dạng Hermit dương trên E/N.

#### Mệnh đề 3 {#evt-v-s1-prop-3 .statement}

— *Cho f là một dạng Hermit dương trên E. Đặt*

$$
p(x) = f(x, x)^{1/2}
$$

*với mọi x \in E. Khi đó p là một chuẩn bán phần trên E, và là một chuẩn khi và chỉ khi f là tách được.*

Chỉ cần chứng minh bất đẳng thức $p(x + y) \leq p(x) + p(y)$. Nhưng ta có

$$
f(x + y, x + y) = f(x, x) + f(y, y) + f(x, y) + \overline{f(x, y)}
$$

và, theo bất đẳng thức Cauchy-Schwarz

$$
f(x + y, x + y) \leq f(x, x) + f(y, y) + 2(f(x, x) f(y, y))^{1/2}
$$
$$
= (f(x, x)^{1/2} + f(y, y)^{1/2})^2 .
$$

#### Nhận xét {#evt-v-s1-n2-rem-1 .statement}

— 1) Giả sử f là dương và tách, và cho x, y là hai vectơ $\neq 0$. Chứng minh của bất đẳng thức Cauchy-Schwarz chỉ ra rằng, nếu hai vế của (7) bằng nhau, thì tồn tại một vô hướng $\xi$ sao cho $f(x + \xi y, x + \xi y) = 0$, do đó $x + \xi y = 0$, nói cách khác, $x$ và $y$ phụ thuộc tuyến tính; đảo lại là ngay lập tức. Chứng minh của bất đẳng thức (8) chỉ ra rằng đẳng thức $p(x + y) = p(x) + p(y)$ chỉ có thể xảy ra nếu $x$ và $y$ phụ thuộc tuyến tính; nếu $y = \lambda x$, đẳng thức trước có thể được viết thành $|1 + \lambda| = 1 + |\lambda|$, và suy ra rằng $\lambda$ là *thực và dương*.

2) Cho $f$ là một dạng Hermit dương trên $E$, và gán cho $E$ nửa chuẩn $x \mapsto f(x, x)^{1/2}$; nếu $f$ là dạng Hermit dương, tách được xác định trên $E/N$ liên kết với $f$, thì không gian chuẩn thu được bằng cách gán chuẩn $x \mapsto f(\dot{x}, \dot{x})^{1/2}$ cho $E/N$ là không gian chuẩn liên kết với $E$ (II, p. 5).

#### Định nghĩa 3 {#evt-v-s1-def-3 .statement}

*Cho $E$ là một không gian vectơ trên trường $K$. Một nửa chuẩn $p$ trên $E$ được gọi là tiền-Hilbert nếu tồn tại một dạng Hermit dương $f$ trên $E$ sao cho $p(x) = f(x, x)^{1/2}$ với mọi $x \in E$*.

Nhận xét rằng đối với một nửa chuẩn $p$ trên $E$, tồn tại nhiều nhất một dạng Hermit dương $f$ sao cho $p(x) = f(x, x)^{1/2}$ với mọi $x \in E$; điều này suy ra từ các công thức phân cực (V, p. 2).

### 3. Các không gian tiền-Hilbert

#### Định nghĩa 4 {#evt-v-s1-def-4 .statement}

*Một không gian tiền-Hilbert là một tập hợp $E$ với cấu trúc của một không gian vectơ trên $K$ và với một dạng Hermit dương. Ta nói rằng $E$ là một không gian tiền-Hilbert thực (tương ứng phức) khi $K$ là $\mathbf{R}$ (tương ứng $K$ là $\mathbf{C}$).*

#### Ví dụ 1 {#evt-v-s1-n3-exa-1 .statement}

Dạng $(\lambda, \mu) \mapsto \overline{\lambda} \mu$ xác định một cấu trúc tiền-Hilbert trên $K$, được gọi là *chính tắc*. Khi $K$ được xem như một không gian tiền-Hilbert, ta luôn hiểu rằng, trừ khi có nói khác đi, nó có cấu trúc này.

#### Ví dụ 2 {#evt-v-s1-n3-exa-2 .statement}

Cho $I$ là một khoảng (bị chặn hoặc không) trong $\mathbf{R}$, và cho $E$ là tập hợp các hàm điều hòa (FVR, II, p. 4) được xác định trên $I$ với các giá trị trong $\mathbf{C}$, có giá đỡ compact. Rõ ràng rằng $E$ là một không gian vectơ trên $\mathbf{C}$; cho $f$ là dạng nửa song tuyến tính $(x, y) \mapsto \int_1^1 \overline{x(t)}\ y(t)\ dt$; điều này là ngay lập tức rằng $f$ là một dạng Hermit dương trên $E$, và do đó xác định một cấu trúc tiền-Hilbert trên không gian này.

#### Ví dụ 3 {#evt-v-s1-n3-exa-3 .statement}

Cho $n \geqslant 0$ là một số nguyên. Ta định nghĩa một cấu trúc không gian tiền-Hilbert trên không gian $K^n$, bằng dạng Hermit

$$
(x, y) \mapsto \sum_{j=1}^n \overline{x_j} y_j
$$

(với $x = (x_1, ..., x_n)$ và $y = (y_1, ..., y_n)$). Khi $K$ là $\mathbf{R}$, ta thấy rằng đây chỉ là tích vô hướng của hai vectơ của $\mathbf{R}^n$ (GT, VI, § 2, No. 2).

#### Ví dụ 4 {#evt-v-s1-n3-exa-4 .statement}

Cho $\ell^2$ (hay $\ell^2(\mathbf{N})$) là tập hợp các dãy $x = (x_n)_{n \in \mathbf{N}}$ gồm các phần tử của $K$ sao cho $\sum_{n=0}^\infty |x_n|^2$ là hữu hạn. Có thể chứng minh rằng $\ell^2$ là một không gian con vectơ của $K^\mathbf{N}$ và định nghĩa một cấu trúc không gian tiền Hilbert trên $\ell^2$ bằng dạng Hermit $(x, y) \mapsto \sum_{n=0}^\infty \overline{x_n} y_n$ (xem V, p. 18).

#### Ví dụ 5 {#evt-v-s1-n3-exa-5 .statement}

Cho $E$ là một không gian tiền Hilbert thực, $f$ là dạng song tuyến tính đối xứng tương ứng trên $E$. Cho $E_{(c)}$ là phức hóa không gian vectơ của $E$; ta đồng nhất $E$ với một tập con của $E_{(c)}$ qua ánh xạ $x \mapsto 1 \otimes x$, sao cho mọi phần tử của $E_{(c)}$ đều có thể viết duy nhất dưới dạng $x_1 + ix_2$ với $x_1, x_2$ trong $E$. Ánh xạ $f$ mở rộng duy nhất thành một dạng Hermit $f_{(c)}$ trên $E_{(c)}$; ta có,

$$
f_{(c)}(x_1 + ix_2, y_1 + iy_2) = f(x_1, y_1) + f(x_2, y_2) + i(f(x_1, y_2) - f(x_2, y_1)) .
$$

Đặc biệt, ta có
$$
f_{(\mathbf{C})}(x_1 + ix_2, x_1 + ix_2) = f(x_1, x_1) + f(x_2, x_2) \geqslant 0,
$$
do đó $f_{(\mathbf{C})}$ là dương. Ta nói rằng $E_{(\mathbf{C})}$, cùng với $f_{(\mathbf{C})}$, là *phức hóa không gian tiền Hilbert* của $E$.

Khi chỉ xét một cấu trúc không gian tiền Hilbert trên một không gian vectơ $E$, giá trị, đối với một cặp $(x, y)$ các phần tử của $E$, của dạng Hermit định nghĩa cấu trúc nói trên được ký hiệu bởi $\langle x|y \rangle_E$ hoặc đơn giản là $\langle x|y \rangle$, nếu không dễ gây nhầm lẫn. Số này được gọi là *tích vô hướng* $^1$ của $x$ và $y$ (*bình phương vô hướng* của $x$ nếu $y = x$). Hai vectơ $x, y$ được gọi là *vuông góc* nếu $\langle x|y \rangle = 0$. Hàm $x \mapsto \|x\| = \langle x|x \rangle^{1/2}$ là một *bán chuẩn* trên không gian vectơ $E$ (V, p. 3); một không gian tiền Hilbert luôn được xét cùng với bán chuẩn này được gán cho nó (và do đó cũng cùng với tôpô và cấu trúc đều tương ứng).

Với các ký hiệu này, trong một không gian tiền Hilbert $E$, bất đẳng thức Cauchy-Schwarz có thể được viết là
$$
|\langle x|y \rangle| \leqslant \|x\| \cdot \|y\|.
$$

Do đó, tích vô hướng là một *dạng sesquilinear liên tục* trên $E \times E$ (II, p. 5, Mệnh đề 4).

Để $E$ là Hausdorff, điều kiện cần và đủ là $x \mapsto \|x\|$ là một *chuẩn* trên $E$; nói cách khác, dạng Hermit $(x, y) \mapsto \langle x|y \rangle$ *dương và phân biệt*; điều này tương đương với việc nói rằng *$0$ là vectơ duy nhất của $E$, vuông góc với chính nó*.

Theo các định nghĩa tổng quát (S, IV, § 1, No. 5), một đẳng cấu từ một không gian tiền Hilbert $E$ lên một không gian tiền Hilbert $F$ là một ánh xạ tuyến tính song ánh $u$ từ $E$ lên $F$ sao cho
$$
\langle u(x)|u(y) \rangle = \langle x|y \rangle
$$
với mọi $x$ và $y$ trong $E$. Ta suy ra từ đó rằng $\|u(x)\| = \|x\|$ với mọi $x \in E$, và hiển nhiên $u$ là một đẳng cấu đối với các cấu trúc không gian vectơ tôpô của $E$ và của $F$; nếu $E$ và $F$ là Hausdorff, $u$ là một *đẳng cự* từ $E$ lên $F$. Ngược lại, nếu $u$ là một ánh xạ tuyến tính song ánh từ $E$ lên $F$, sao cho $\|u(x)\| = \|x\|$ với mọi $x \in E$, các công thức phân cực (V, p. 2) chỉ ra rằng $u$ là một đẳng cấu không gian tiền Hilbert từ $E$ lên $F$.

Cho $E$ là một không gian tiền Hilbert *phức*, và $\langle x|y \rangle$ là tích vô hướng trong $E$. Trên tập hợp $E$, ta có thể định nghĩa một cấu trúc không gian vectơ thứ hai đối với $\mathbf{C}$, lấy cùng luật của nhóm cộng và lấy luật hợp thành ngoài $(\lambda, x) \mapsto \overline{\lambda} x$ (A, II, § 1, No. 13) cho cấu trúc không gian vectơ này, $(x, y) \mapsto \langle y|x \rangle$ là một *dạng Hermit dương*

1 Đôi khi có thể xảy ra rằng ta viết $(x|y)$ cho $\langle y|x \rangle$. Lưu ý rằng công thức (4) của V, p. 2, có các dạng tương đương sau:
$$
\begin{align*}
\langle \sum_i \lambda_i x_i | \sum_j \mu_j y_j \rangle &= \sum_{i,j} \overline{\lambda}_i \mu_j \langle x_i|y_j \rangle. \\
(\sum_i \lambda_i x_i | \sum_j \mu_j y_j) &= \sum_{i,j} \lambda_i \overline{\mu}_j (x_i|y_j).
\end{align*}
$$

. Không gian tiền Hilbert $\overline{E}$ thu được bằng cách gán cấu trúc không gian vectơ mới này và dạng Hermit mới cho E, được gọi là liên hợp với E. Một đẳng cấu $u$ từ E lên $\overline{E}$ là một ánh xạ nửa tuyến tính từ E lên chính nó (đối với tự đẳng cấu $\xi \mapsto \overline{\xi}$ của $\mathbf{C}$) sao cho $\langle u(y)|u(x) \rangle = \langle x|y \rangle$ hoặc $\langle u(x)|u(y) \rangle = \overline{\langle x|y \rangle}$ (với $x, y$ trong E); ánh xạ như vậy được gọi là một nửa tự đẳng cấu của không gian tiền Hilbert E.

Nếu E là một không gian tiền Hilbert, M là một không gian vectơ con của E, hạn chế của tích vô hướng $\langle x|y \rangle$ trên $M \times M$ là một dạng Hermit dương trên M, từ đó định nghĩa một cấu trúc không gian tiền Hilbert trên M; ta nói rằng cấu trúc này được cảm sinh bởi cấu trúc của E, hoặc M là một không gian con tiền Hilbert của E.

### 4. Các không gian Hilbert

#### Định nghĩa 5 {#evt-v-s1-def-5 .statement}

*Một không gian Hilbert* (hay *không gian Hilbert*) *là một không gian tiền Hilbert Hausdorff và đầy đủ*. *Ta nói rằng một chuẩn trên một không gian vectơ E (trên K) là Hilbert nếu nó là tiền Hilbert, và nếu không gian chuẩn E là đầy đủ*.

Nếu E là một không gian Hilbert và M là một không gian vectơ con đóng của E, cấu trúc không gian tiền Hilbert cảm sinh trên M thực sự là một cấu trúc không gian Hilbert. Trong trường hợp này ta nói rằng M, với cấu trúc cảm sinh, là một *không gian con Hilbert* của E.

#### Ví dụ 1 {#evt-v-s1-n4-exa-1 .statement}

Các không gian tiền Hilbert được định nghĩa trong các ví dụ 1, 3, 4 của V, p. 4, là các không gian Hilbert. Mặt khác, không gian tiền Hilbert được định nghĩa trong ví dụ 2 không Hausdorff cũng không đầy đủ. Phức hóa của một không gian Hilbert là một không gian Hilbert.

#### Ví dụ 2 {#evt-v-s1-n4-exa-2 .statement}

Cho X là một không gian tôpô Hausdorff và cho $\mu$ là một độ đo dương trên X. Cho $L^2(X, \mu)$ là không gian gồm các lớp tương đương, đối với $\mu$, của tất cả các hàm bình phương $\mu$-khả tích trên X với giá trị trong $\mathbf{C}$. Đây là một không gian Hilbert phức, có tích vô hướng được cho bởi

$$
\langle f|g \rangle = \int_X \overline{f(x)}\ g(x)\ d\mu(x) .
$$

#### Ví dụ 3 {#evt-v-s1-n4-exa-3 .statement}

Let $n \geqslant 1$ be an integer and let U be an open set in $\mathbf{R}^n$. Let $\mu$ be the measure on U induced by the Lebesgue measure on $\mathbf{R}^n$, and put $\mathcal{H}^0 = L^2(U, \mu)$. Let $\mathcal{H}^1$ denote the space of all functions $f \in \mathcal{H}^0$ with the following property; for $1 \leqslant i \leqslant n$, there exists a function $g_i \in \mathcal{H}^\circ$ such that

$$
\int_U g_i(x)\ h(x)\ d\mu(x) = - \int_U f(x)\ D_i h(x)\ d\mu(x)
$$

for every function $h$ of class $C^1$ with compact support in U. The function $g_i$ is defined uniquely up to equivalence with respect to $\mu$, and is denoted by $D_i f$ or $\partial f / \partial x_i$ (ith partial derivative). By induction on the integer $s \geqslant 1$, we define $\mathcal{H}^s$ as the set of all functions $f \in \mathcal{H}^1$ such that $D_i f \in \mathcal{H}^{s-1}$ for $1 \leqslant i \leqslant n$. We define a scalar product on $\mathcal{H}^s$ by the formula

$$
\langle f|g \rangle = \sum_{k=0}^s \sum_{1 \leqslant i_1 \leqslant \ldots \leqslant i_k \leqslant n} \int \overline{D_{i_1} \ldots D_{i_k} f} \cdot D_{i_1} \ldots D_{i_k} g\ d\mu .
$$

Khi đó $\mathcal{H}^s$ là một không gian Hilbert phức, được gọi là *không gian Sobolev* cấp s.

#### Ví dụ 4 {#evt-v-s1-n4-exa-4 .statement}

Cho X là một đa tạp vi phân lớp $C^r$ (với $r \geqslant 1$) thuần túy có số chiều hữu hạn $n$.

Trong không gian bó sợi vectơ $\Lambda^n T(X)$, gọi L là phần bù của tiết diện không. Với mọi số thực $\lambda \neq 0$, ánh xạ $u \mapsto \lambda u$ từ $\Lambda^n T(X)$ vào chính nó giữ L ổn định.

Cho $\alpha$ là một số phức. Một hàm nhận giá trị phức $\omega$ trên L sao cho $\omega(\lambda u) = |\lambda|^{\alpha} \omega(u)$ với $u \in L$ và mọi số thực khác không $\lambda$ được gọi là một mật độ cấp $\alpha$ trên X. Ta nói rằng một mật độ $\omega$ cấp 1 là tích phân được địa phương nếu tồn tại một phủ mở $(U_i)_{i \in I}$ của X, và với mọi $i \in I$ một hệ tọa độ $\xi_i = (\xi_i^1, ..., \xi_i^n)$ trên $U_i$ và một hàm nhận giá trị phức $f_i$ trên $\xi_i(U_i)$ thỏa mãn các điều kiện sau:

a) Hàm $f_i$ tích phân được địa phương trên tập mở $\xi_i(U_i)$ của $\mathbf{R}^n$ đối với độ đo Lebesgue $\mu$;

b) Cho $x \in U_i$; nếu $(\partial_{1,i,x}, ..., \partial_{n,i,x})$ là cơ sở của $T_x X$ liên kết với hệ tọa độ $(\xi_i', ..., \xi_i^n)$ trong $U_i$ thì ta có
$$
\omega(\partial_{1,i,x} \wedge ... \wedge \partial_{n,i,x}) = f_i(\xi_i^1(x), ..., \xi_i^n(x)) .
$$

Khi đó, tồn tại duy nhất một độ đo $\tilde{\omega}$ trên X sao cho với mọi $i \in I$, ảnh của hạn chế của $\tilde{\omega}$ lên $U_i$ qua $\xi_i$ bằng độ đo $f_i \cdot \mu$ (xem VAR, R, 10.4.3).

Cho $\mathcal{V}$ (tương ứng $\mathcal{N}$) là không gian vectơ của các mật độ khả đo $\omega$ cấp $1/2$ sao cho độ đo liên kết với mật độ $|\omega|^2$ cấp 1 là bị chặn (tương ứng bằng không). Cho $\omega_1$ và $\omega_2$ thuộc $\mathcal{V}$; khi đó $\omega = \overline{\omega_1} \omega_2$ là một mật độ cấp 1, và độ đo $\tilde{\omega}$ liên kết với $\omega$ là bị chặn; số $\int_X \tilde{\omega}$ chỉ phụ thuộc vào các lớp $\dot{\omega}_1$ và $\dot{\omega}_2$ của $\omega_1$ và $\omega_2$ modulo $\mathcal{N}$ và được ký hiệu bởi $\langle \omega_1 | \omega_2 \rangle$ hoặc $\langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$. Khi đó ánh xạ $(\dot{\omega}_1, \dot{\omega}_2) \mapsto \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$ gán cho không gian vectơ $\Omega_{1/2}(X) = \mathcal{V}/\mathcal{N}$ một cấu trúc không gian Hilbert phức.

#### Ví dụ 5 {#evt-v-s1-n4-exa-5 .statement}

Cho D là đĩa mở có tâm 0 và bán kính 1 trong $\mathbf{C}$. *Không gian Hardy* $H^2(D)$ gồm tất cả các hàm chỉnh hình $f : D \to \mathbf{C}$ sao cho
$$
\sup_{0 < R < 1} \int_0^1 |f(R \cdot e(\theta))|^2 d\theta < + \infty .
$$
Nếu $f_1$ và $f_2$ thuộc $H^2(D)$, giới hạn
$$
\langle f_1 | f_2 \rangle = \lim_{R \to 1} \int_0^1 \overline{f_1(R \cdot e(\theta))} \cdot f_2(R \cdot e(\theta)) \, d\theta
$$
tồn tại; ánh xạ $(f_1, f_2) \mapsto \langle f_1 | f_2 \rangle$ gán cho không gian vectơ $H^2(D)$ một cấu trúc không gian Hilbert phức.

Để một hàm $f : D \to \mathbf{C}$ thuộc $H^2(D)$ thì cần và đủ rằng tồn tại một dãy $(a_n)_{n \in \mathbf{N}}$ các số phức sao cho $\sum_{n=0}^\infty |a_n|^2 < + \infty$ và
$$
f(z) = \sum_{n=0}^\infty a_n z^n
$$
với mọi $z \in D$. Khi đó ta có $\|f\|^2 = \sum_{n=0}^\infty |a_n|^2$, điều này cho một đẳng cấu từ $H^2(D)$ lên không gian Hilbert $\ell^2$ (V, p. 4).

Mọi không gian tiền Hilbert Hausdorff đều đẳng cấu với một không gian con trù mật khắp nơi của một không gian Hilbert được xác định tới một đẳng cấu. Chính xác:

#### Mệnh đề 4 {#evt-v-s1-prop-4 .statement}

— *Cho E là một không gian tiền Hilbert Hausdorff, $\hat{E}$ là không gian hoàn thiện theo chuẩn của E* (GT, IX, § 3, No. 3). *Tích vô hướng* $(x, y) \mapsto \langle x|y \rangle$ *mở rộng liên tục thành một dạng Hermit dương và tách trên* $\hat{E}$, *và xác định một cấu trúc không gian Hilbert trên* $\hat{E}$.

Sự tồn tại của phép mở rộng của $(x, y) \mapsto \langle x|y \rangle$ sang $\hat{E} \times \hat{E}$ suy ra từ tính liên tục của dạng sesqui tuyến tính này trên $E \times E$ (GT, III, § 6, No. 5, th. 1). Hơn nữa, phép mở rộng này, cũng sẽ được ký hiệu bởi $(x, y) \mapsto \langle x|y \rangle$, là một dạng Hermit và thỏa mãn quan hệ $\langle x|x \rangle = \|x\|^2$, nhờ nguyên lý mở rộng các đẳng thức ($\|x\|$ là chuẩn trên $\hat{E}$ thu được bằng cách mở rộng chuẩn trên E bằng liên tục); điều này chứng tỏ rằng quan hệ $\langle x|x \rangle = 0$ kéo theo $x = 0$ trong $\hat{E}$, do đó dạng $(x, y) \mapsto \langle x|y \rangle$ là dương và tách, và do đó xác định một cấu trúc không gian Hilbert trên $\hat{E}$. Q.E.D.

Không gian Hilbert này được gọi là *sự hoàn thiện* của không gian tiền Hilbert Hausdorff E.

\* *Ví dụ 6*. — Cho U là một tập con mở của $\mathbf{R}^n$ ($n \geqslant 1$). Cho $\mathscr{C}_0^1(\mathrm{U})$ là không gian vectơ của tất cả các hàm lớp $\mathrm{C}^1$ có giá compact trong U. Ta định nghĩa một cấu trúc không gian tiền Hilbert Hausdorff trên $\mathscr{C}_0^1(\mathrm{U})$ mà tích vô hướng được cho bởi

$$
\langle f|g \rangle = \sum_{i=1}^{n} \int_{\mathrm{U}} \overline{\mathrm{D}_i f(x)} . \mathrm{D}_i g(x) \, dx .
$$

Không gian tiền Hilbert này không đầy đủ. Phần hoàn thành của nó được gọi là *không gian Dirichlet* liên kết với U. \*

#### Hệ quả {#evt-v-s1-n4-cor-1 .statement}

— *Cho V là một không gian vectơ trên K và f là một dạng Hermit dương trên V.*
a) *Tồn tại một không gian Hilbert E và một ánh xạ tuyến tính* $u : V \to E$ *sao cho* $f(x, y) = \langle u(x)|u(y) \rangle$ *với x, y trong V, và sao cho u(V) trù mật trong E.*
b) *Nếu hai cặp* $(E_i, u_i)$ *thỏa mãn các điều kiện tương tự như a), thì tồn tại một đẳng cấu duy nhất* \phi *từ không gian Hilbert* $E_1$ *lên không gian Hilbert* $E_2$ *sao cho* $u_2 = \phi \circ u_1$.

Gọi N là tập hợp tất cả các $x \in V$ sao cho $f(x, x) = 0$. Ta định nghĩa một dạng Hermit dương và tách trên không gian V/N bởi $\langle \dot{x}|\dot{y} \rangle = f(x, y)$ với $x \in \dot{x}$ và $y \in \dot{y}$. Gọi E là sự hoàn thành của V/N thành một không gian Hilbert và u là ánh xạ $x \mapsto x + N$ từ V vào E. Khi đó các điều kiện của *a*) được thỏa mãn.

Trong các giả thiết của *b*), N bằng hạt nhân của u_1 và của u_2. Do đó tồn tại một ánh xạ tuyến tính song ánh \phi_0 từ u_1(V) lên u_2(V) sao cho u_2(x) = \phi_0(u_1(x)) với mọi x \in V. Ta kiểm tra ngay lập tức rằng \phi_0 là một đẳng cấu của các không gian tiền Hilbert, suy ra là một đẳng cự. Vì u_i(V) trù mật trong E_i với i = 1, 2, \phi_0 mở rộng duy nhất thành một đẳng cự \phi từ E_1 lên E_2, và *b*) theo sau.

Ta nói rằng không gian Hilbert E là *phần hoàn thành tách* của V (đối với dạng *f*).

*Ví dụ 7*. — Cho G là một nhóm (với phần tử đơn vị 1) và \pi là một đồng cấu từ G vào nhóm các tự đẳng cấu của một không gian Hilbert phức E ; ta nói rằng \pi là một *biểu diễn đơn vị* của G trong E. Cho $a \in E$ ; ta đặt

$$
\phi(x) = \langle a|\pi(x).a \rangle
$$

với mọi $x \in G$. Khi đó $\phi : G \to \mathbf{C}$ là *xác định dương*, nói cách khác thỏa mãn quan hệ :

(PD) Đối với mọi $\lambda_1, ..., \lambda_n$ trong $\mathbf{C}$ và $x_1, ..., x_n$ trong G, ta có

$$
\sum_{i,j=1}^n \overline{\lambda_i} \lambda_j \phi(x_i^{-1} x_j) \geqslant 0 .
$$

Thật vậy, hạng tử đầu tiên của (11) chính là $\| \sum_{i=1}^n \lambda_i \pi(x_i) . a \| ^2$.

Ngược lại, cho $\phi$ là một hàm xác định dương trên G. Cho $C^{(G)}$ là không gian vectơ của mọi hàm có giá hữu hạn trên G. Ta định nghĩa một dạng Hermit \Phi trên G bởi

$$
\Phi(u, v) = \sum_{x,y \in G} \overline{u(x)} \ v(y) \ \phi(x^{-1} y)
$$

và quan hệ (PD) biểu thị rằng \Phi là dương. Theo hệ quả của Mệnh đề 4, tồn tại một không gian Hilbert E và một ánh xạ tuyến tính \rho : C^{(G)} \to E, có ảnh trù mật, sao cho

$$
\Phi(u, v) = \langle \rho(u)|\rho(v) \rangle \quad \text{cho} \quad u, v \quad \text{thuộc} \quad C^{(G)} .
$$

### 5. Các tập con lồi của một không gian tiền Hilbert

Nếu ta tính $\| x - y \| ^2 = \langle x - y|x - y \rangle$ và $\| x + y \| ^2 = \langle x + y|x + y \rangle$ cho bất kỳ hai điểm nào $x, y$ của một không gian tiền Hilbert $E$, ta ngay lập tức được « đẳng thức trung vị »

$$
\| \frac{1}{2}(x + y) \| ^2 + \| \frac{1}{2}(x - y) \| ^2 = \frac{1}{2} (\| x \| ^2 + \| y \| ^2 ) .
$$

Từ đẳng thức này ta suy ra mệnh đề sau:

![Biểu đồ cho thấy các tập B', B và A, với x và y được đánh dấu trong A](https://i.imgur.com/3Q5z5QG.png)

Fig. 1.

#### Mệnh đề 5 {#evt-v-s1-prop-5 .statement}

— Cho $E$ là một không gian tiền Hilbert. Cho $d$ là một số thực $> 0$, $\delta$ là một số thực thỏa mãn $0 \leqslant \delta \leqslant d$. Cho $B$ và $B'$ là các tập con của $E$ được xác định bởi $\| x \| < d$,

$$
\|x\| \leq d + \delta \text{ tương ứng, và cho } A \text{ là một tập lồi được chứa trong } B' - B. \text{ Khi đó với mọi cặp điểm } x, y \text{ của } A, \text{ ta có } \|x - y\| \leq \sqrt{12d\delta} \text{ (hình 1).}
$$
Thật vậy, ta có $\frac{1}{2}(x + y) \in A$, do đó $\left\| \frac{1}{2}(x + y) \right\| \geq d$; do đó từ (14) ta được bất đẳng thức
$$
\left\| \frac{1}{2}(x - y) \right\|^2 = \frac{1}{2}(\|x\|^2 + \|y\|^2) - \left\| \frac{1}{2}(x + y) \right\|^2 \leq (d + \delta)^2 - d^2 \leq 3d\delta
$$
từ đó mệnh đề suy ra.

#### Định lý 1 {#evt-v-s1-thm-1 .statement}

*Cho E là một không gian tiền Hilbert, và H là một tập con lồi không rỗng của E sao cho H là một không gian con đều Hausdorff và đầy đủ của E. Với mọi $x \in E$, tồn tại một điểm duy nhất $p_H(x)$ trong H sao cho $\|x - p_H(x)\| = \inf_{y \in H} \|x - y\|$. Phần tử $p_H(x)$ của H cũng là phần tử duy nhất $a$ của H thỏa mãn quan hệ*
$$
\Re \langle x - a | y - a \rangle \leq 0
$$
*với mọi* $y \in H$.

![Biểu đồ cho thấy một điểm x, một điểm y, và một đoạn thẳng được gắn nhãn a + λ(y − a)](https://i.imgur.com/3Q5z5QG.png)

Fig. 2.

Đặt $d = \inf_{y \in H} \|x - y\|$, và với mọi số nguyên $n > 0$, gọi $H_n$ là tập hợp các điểm $y$ của H sao cho $\|x - y\| \leq d + n^{-1}$. Tập hợp $H_n$ là đóng trong H, là lồi và khác rỗng, và đường kính của nó bị chặn bởi $\sqrt{12 \frac{d}{n}}$ với mọi $n$ đủ lớn, theo mệnh đề 5. Dãy $(H_n)_{n \geq 1}$ là giảm, và tập hợp H là Hausdorff và đầy đủ nên suy ra rằng cơ sở của lọ Cauchy $(H_n)_{n \geq 1}$ hội tụ đến một điểm $p_H(x)$ của H; ta có $\{ p_H(x) \} = \bigcap_{n \geq 1} H_n$, do đó $p_H(x)$ là điểm duy nhất $a$ của H sao cho $\|x - a\| = d$.

1 Ta nhắc lại (GT, VIII, § 1, No. 1) rằng $\Re(z)$ ký hiệu phần thực của số phức z; ta có $\Re(z) = z$ nếu z là thực.

Cho $y \in \mathbf{H}$; vì $\mathbf{H}$ là lồi, điểm $z(\lambda) = p_{\mathbf{H}}(x) + \lambda(y - p_{\mathbf{H}}(x))$ của E thuộc về $\mathbf{H}$ với mọi số thực $\lambda$ sao cho $0 < \lambda < 1$. Do đó ta có
$$
\| x - z(\lambda) \|^{2} \geq \| x - p_{\mathbf{H}}(x) \|^{2} \quad \text{với} \quad 0 < \lambda < 1 ,
$$
suy ra
$$
\mathcal{R} \langle x - p_{\mathbf{H}}(x)|y - p_{\mathbf{H}}(x) \rangle = \lim_{\lambda \to 0} \frac{1}{2\lambda} \left\{ \| x - p_{\mathbf{H}}(x) \|^{2} - \| x - z(\lambda) \|^{2} \right\} \leq 0 .
$$
Ngược lại, cho $a$ là một điểm của $\mathbf{H}$ sao cho $\mathcal{R} \langle x - a|y - a \rangle \leq 0$ với mọi $y \in \mathbf{H}$. Với mọi $y \in \mathbf{H}$, ta có
$$
\| x - y \|^{2} = \| x - a \|^{2} + \| y - a \|^{2} - 2 \mathcal{R} \langle x - a|y - a \rangle \geq \| x - a \|^{2} ,
$$
và do đó $\| x - a \| = d$ và cuối cùng suy ra $a = p_{\mathbf{H}}(x)$ từ phần đầu của chứng minh. Q.E.D.

Trong phần tiếp theo, ánh xạ $p_{\mathbf{H}}$ của E vào $\mathbf{H}$ sẽ được gọi là *phép chiếu* từ E lên $\mathbf{H}$. Ta nhận xét rằng $p_{\mathbf{H}}(x) = x$ với mọi $x \in \mathbf{H}$.

Phần đầu của định lý 1 đúng với các giả thiết tổng quát hơn về không gian E (V, p. 67, bài tập 31).

Chứng minh của định lý 1 thiết lập, trong số các kết quả khác, tính chất sau đây :

#### Hệ quả 1 {#evt-v-s1-thm-1-cor-1 .statement}

*Cho I là một tập hợp có hướng bởi một lọ $\mathfrak{F}$ và cho $(y_{i})_{i \in I}$ là một họ các điểm của $\mathbf{H}$. Cho $x \in \mathbf{E}$. Giả sử rằng ta có*
$$
\lim_{i, \mathfrak{F}} \| x - y_{i} \| = \inf_{z \in \mathbf{H}} \| x - z \| .
$$
*Khi đó $y_{i}$ tiến tới $p_{\mathbf{H}}(x)$ đối với lọ $\mathfrak{F}$.*

#### Hệ quả 2 {#evt-v-s1-thm-1-cor-2 .statement}

*Với mọi $x, y$ trong $\mathbf{E}$, ta có*
$$
\| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \| \leq \| x - y \| .
$$
*Đặc biệt, ánh xạ $p_{\mathbf{H}}$ từ $\mathbf{E}$ vào $\mathbf{H}$ là liên tục.*

Cho $x, y$ là hai điểm của $\mathbf{E}$. Đặt $a = p_{\mathbf{H}}(x) - x, b = p_{\mathbf{H}}(y) - p_{\mathbf{H}}(x), c = y - p_{\mathbf{H}}(y)$. Theo công thức (15) (V, p. 10) ta có $\mathcal{R} \langle a|b \rangle \geq 0$ và $\mathcal{R} \langle c|b \rangle \geq 0$. Ta cũng có $a + b + c = y - x$, điều này cho,
$$
\| x - y \|^{2} = \| a + b + c \|^{2} = \| b \|^{2} + \| a + c \|^{2} + 2 \mathcal{R} \langle a|b \rangle + 2 \mathcal{R} \langle c|b \rangle
$$
$$
\geq \| b \|^{2} = \| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \|^{2} .
$$
Điều này chứng minh hệ quả 2.

#### Mệnh đề 6 {#evt-v-s1-prop-6 .statement}

*Cho $\mathbf{E}$ là một không gian tiền Hilbert và cho $\Phi$ là một tập giảm có hướng không rỗng của các tập con lồi Hausdorff và đầy đủ không rỗng của $\mathbf{E}$. Với mọi $x \in \mathbf{E}$ và mọi tập con $\mathbf{H}$ của $\mathbf{E}$, đặt $d(x, \mathbf{H}) = \inf_{z \in \mathbf{H}} \| x - z \|$. Để giao M của các tập H thuộc $\Phi$ là không rỗng, điều kiện cần và đủ là tồn tại $x_0$ trong E sao cho $\sup_{H \in \Phi} d(x_0, H)$ là hữu hạn. Với mọi $x \in E$ ta có khi đó
$$
p_M(x) = \lim_{H \in \Phi} p_H(x)
$$
(giới hạn đối với tập có hướng $\Phi$).

Nếu M là không rỗng, $d(x, H) \leq d(x, M)$ với mọi $H \in \Phi$ và mọi $x \in E$.

Ngược lại, giả sử rằng tồn tại một điểm $x_0$ trong E và một số thực $C \geq 0$ sao cho $d(x_0, H) \leq C$ với mọi $H \in \Phi$. Cho $x \in E$; khi đó
$$
d(x, H) \leq \|x - x_0\| + C \quad \text{với mọi } H \in \Phi,
$$
do đó số $d = \sup_{H \in \Phi} d(x, H)$ là hữu hạn. Gọi B là tập hợp tất cả các $z \in E$ sao cho $\|x - z\| \leq d$. Vì B là lồi và đóng trong E, các tập $H \cap B$, với H chạy qua $\Phi$, là lồi, Hausdorff và đầy đủ. Cho $\varepsilon > 0$; tồn tại một tập $H \in \Phi$ sao cho $d(x, H) \geq d - \varepsilon$, và nếu $\varepsilon < d/2$, đường kính của $H \cap B$ bị chặn bởi $\sqrt{12 \varepsilon (d - \varepsilon)}$ theo mệnh đề 5 (V, p. 9). Nói cách khác, với mọi $H_0 \in \Phi$, các tập đóng $H \cap B$, với $H \in \Phi$ và $H \subset H_0$, tạo thành một cơ sở của lọc Cauchy trên không gian Hausdorff và đầy đủ $H_0$. Do đó giao của các tập $H \cap B$ (với $H \in \Phi$) thu gọn thành một điểm y. Ta được $y \in M$ và $\|x - y\| = d = d(x, M)$. Vì M đóng trong $H_0$, nó là một tập Hausdorff, lồi và đầy đủ trong E, và do đó $y = p_M(x)$. Với mọi $H \in \Phi$, ta có $p_H(x) \in H \cap B$, từ đó suy ra rằng $p_M(x) = \lim_{H \in \Phi} p_H(x)$.

#### Mệnh đề 7 {#evt-v-s1-prop-7 .statement}

*Cho E là một không gian tiền Hilbert Hausdorff và cho $\Psi$ là một tập tăng có hướng không rỗng của các tập con lồi, đầy đủ không rỗng của E. Đặt $A = \bigcup_{H \in \Psi} H$ và giả sử rằng bao đóng N của A là đầy đủ. Khi đó N là lồi và ta có*
$$
p_N(x) = \lim_{H \in \Psi} p_H(x) \text{ với mọi } x \in E.
$$

Hiển nhiên rằng A là lồi, do đó bao đóng của nó N là lồi (II, p. 13). Với các ký hiệu của mệnh đề 6, $d(x, N) = \inf_{H \in \Psi} d(x, H)$, và do đó $d(x, N)$ là giới hạn của $d(x, H)$ đối với lọc tiết diện của $\Psi$. Vì $p_H(x) \in H$ và
$$
\lim_{H \in \Psi} \|x - p_H(x)\| = \lim_{H \in \Psi} d(x, H) = d(x, N),
$$
suy ra từ hệ quả 1 của V, p. 11 rằng $p_H(x)$ tiến đến phép chiếu $p_N(x)$ của $x$ lên N đối với lọc tiết diện của $\Psi$.

### 6. Không gian con vectơ và các phép chiếu trực giao

Cho E là một không gian tiền Hilbert. Nhắc lại rằng hai vectơ $x$ và $y$ của E được gọi là *trực giao* nếu $\langle x | y \rangle = 0$; khi đó
$$
\|x + y\|^2 = \|x\|^2 + \|y\|^2
$$
(« định lý Pythagoras »).

Cho A là một tập con của E. Ta nói rằng một vectơ x trong E là trực giao với A nếu nó trực giao với mọi vectơ của A. Tập hợp tất cả các vectơ trực giao với A là một không gian con vectơ đóng của A, ký hiệu bởi $A^\circ$ và được gọi (do lạm dụng ngôn ngữ) là phần trực giao của A.

Cho A và B là hai tập con của E. Ta nói rằng A và B là trực giao nếu mọi vectơ của A đều trực giao với mọi vectơ của B. Điều này tương đương với việc nói rằng $A \subset B^\circ$, hoặc rằng $B \subset A^\circ$. Nếu E là Hausdorff và nếu A và B trực giao thì $A \cap B$ là rỗng hoặc thu gọn về 0 vì 0 là vectơ duy nhất của E trực giao với chính nó.

#### Định lý 2 {#evt-v-s1-thm-2 .statement}

*Cho E là một không gian tiền Hilbert và M là một không gian con vectơ của E, Hausdorff và đầy đủ. Khi đó E là tổng trực tiếp tôpô của M và $M^\circ$ là không gian con trực giao với M. Phép chiếu từ E lên M liên kết với phân tích $E = M \oplus M^\circ$ là phép chiếu $p_M$ từ E lên M được định nghĩa trong định lý 1 (V, p. 10).

Trước hết ta chứng minh rằng $x - p_M(x)$ thuộc $M^\circ$ với mọi $x \in E$. Cho $y \in M$. Với mọi vô hướng $\lambda \in K$, vectơ $p_M(x) + \lambda y$ thuộc M; do đó theo công thức 15 (V, p. 10) ta có,

$$
\mathcal{R}(\lambda \langle x - p_M(x)|y \rangle) \leq 0
$$

với mọi $\lambda \in K$. Nếu, đặc biệt, ta lấy $\lambda = \overline{\langle x - p_M(x)|y \rangle}$ ta kết luận rằng $\langle x - p_M(x)|y \rangle = 0$, do đó có mệnh đề của ta.

Vì M là Hausdorff, 0 là vectơ duy nhất của M, trực giao với chính nó, do đó $M \cap M^\circ = \{0\}$. Với mọi $x \in E$, ta có $p_M(x) \in M$ và $x - p_M(x) \in M^\circ$. Do đó, E là tổng trực tiếp của M và $M^\circ$, và $p_M$ là phép chiếu từ E lên M với hạt nhân $M^\circ$. Vì $p_M$ là một ánh xạ liên tục từ E vào M (V, p. 11, hệ quả 2), nên suy ra từ GT, III, § 6, No. 2 rằng E là tổng trực tiếp tôpô của M và $M^\circ$.

#### Hệ quả {#evt-v-s1-n6-cor-1 .statement}

*Cho E là một không gian tiền Hilbert Hausdorff và M là một không gian con vectơ hữu hạn chiều của E. Khi đó E là tổng trực tiếp của M và $M^\circ$.

Vì E là Hausdorff, nên M cũng vậy; vì M hữu hạn chiều, nó đầy đủ (I, p. 13). Do đó chỉ cần áp dụng định lý 2.

Với các ký hiệu của định lý 2, ta nói rằng $M^\circ$ là phần bù trực giao của M và rằng $p_M$ là phép chiếu trực giao (hoặc phép chiếu vuông góc, hoặc do lạm dụng ngôn ngữ, phép chiếu) từ E lên M; nếu x là một vectơ của E, vectơ $p_M(x)$ của M cũng được gọi là phép chiếu trực giao của x lên M. Chú ý rằng $p_M$ là một ánh xạ tuyến tính liên tục từ E lên M và ta có $\|p_M\| = 1$ theo hệ quả 2 của V, p. 11, ngoại trừ trường hợp $M = \{0\}$ khi đó $p_M = 0$.

Suy ra ngay lập tức từ định lý Pythagoras rằng ánh xạ chính tắc $\psi$ từ $E/M$ lên $M^\circ$ suy ra từ phân tích tổng trực tiếp $E = M \oplus M^\circ$ là đẳng cự nếu $E/M$ được gán chuẩn nửa thương từ chuẩn nửa của E (II, p. 4). Ta sẽ luôn gán cho $E/M$ cấu trúc tiền Hilbert đó sao cho $\psi$ là một đẳng cấu của các không gian tiền Hilbert; khi đó chuẩn nửa thương trên $E/M$ được suy ra từ cấu trúc tiền Hilbert này.

Ta sẽ thường xuyên sử dụng các kết quả trước đó khi E là một không gian Hilbert và M là một không gian con vectơ đóng của E. Trong trường hợp này, $M^\circ$ là một không gian con vectơ đóng của E, và $p_{M^\circ} = 1 - p_M$, và $(M^\circ)^\circ = M$.

#### Mệnh đề 8 {#evt-v-s1-prop-8 .statement}

— Cho E là một không gian Hilbert, M là một không gian con vectơ đóng của E, I là một tập hợp có thứ tự có hướng không rỗng và $(M_i)_{i \in I}$ là một họ các không gian con vectơ đóng của E. Ta giả sử rằng hoặc ánh xạ $i \mapsto M_i$ là tăng và M là bao đóng của $\bigcup_{i \in I} M_i$, hoặc ánh xạ $i \mapsto M_i$ là giảm và $M = \bigcap_{i \in I} M_i$. Khi đó $p_M(x) = \lim_{i \in I} p_{M_i}(x)$ với mọi $x \in E$.

Mệnh đề 8 suy ra ngay lập tức từ các mệnh đề 6 (V, p. 11) và 7 (V, p. 12).

#### Mệnh đề 9 {#evt-v-s1-prop-9 .statement}

— Cho E là một không gian Hilbert và M, N là hai không gian con vectơ đóng của E.

(a) Các điều kiện sau là tương đương :
(i) $p_M p_N = p_N p_M$;
(ii) nếu $x \in M$ trực giao với $M \cap N$ và nếu $y \in N$ trực giao với $M \cap N$, thì x và y trực giao;
(iii) mọi vectơ của M trực giao với $M \cap N$ đều trực giao với N;
(iv) $M = (M \cap N) + (M \cap N^\circ)$.

b) Nếu các điều kiện tương đương của a) được thỏa mãn, ta có $p_{M \cap N} = p_M p_N$, không gian con vectơ $M + N$ của E là đóng và ta có $p_{M+N} = p_M + p_N - p_M p_N$.

c) Ta có $p_M p_N = 0$ khi và chỉ khi M trực giao với N. Nếu vậy, thì không gian con vectơ $M + N$ của E là đóng, và $p_{M+N} = p_M + p_N$.

Đặt $L = M \cap N$, $M_1 = M \cap L^\circ$ và $N_1 = N \cap L^\circ$. Điều kiện (ii) suy ra rằng $M_1$ và $N_1$ trực giao, và (iii) suy ra rằng $M_1$ và N trực giao. Vì ta có $N = N_1 + L$ và $M_1$ trực giao với L, ta đã chứng minh sự tương đương của (ii) và (iii). Nếu điều kiện (iii) được thỏa mãn, ta có $M_1 = M \cap N^\circ$ và vì $M = L + M_1$, điều kiện (iv) được thỏa mãn. Ngược lại, từ (iv) ta kết luận rằng $M_1 = M \cap N^\circ$ vì các không gian con $M \cap N$ và $M \cap N^\circ$ của M trực giao, và do đó $M_1 \subset N^\circ$, nghĩa là quan hệ (iii).

Giả sử điều kiện (iv) được thỏa mãn. Hiển nhiên rằng $p_N(y) = p_L(y)$ với mọi $y \in M$ và do đó $p_N p_M(x) = p_L p_M(x)$ với mọi $x \in E$. Nhưng, với mọi $x \in E$, vectơ $p_L p_M(x)$ thuộc L, và vectơ
$$
x - p_L p_M(x) = (x - p_M(x)) + (p_M(x) - p_L(p_M(x)))
$$
thuộc $M^\circ + L^\circ = L^\circ$; do đó ta có $p_L p_M(x) = p_L(x)$. Cuối cùng, $p_N p_M = p_L p_M = p_L$. Vì điều kiện (ii) tương đương với (iv) và đối xứng theo M và N, ta cũng có $p_M p_N = p_L$. Cuối cùng ta được $p_M p_N = p_N p_M = p_{M \cap N}$, điều này cho (i).

Ngược lại, giả sử điều kiện (i) được thỏa mãn. Lấy $x \in M$; ta có
$$
p_M(p_N(x)) = p_N(p_M(x)) = p_N(x)
$$
và do đó $p_N(x) \in M$. Ta kết luận rằng $x - p_N(x) \in M$, do đó $x$ là tổng của một phần tử $p_N(x)$ của $M \cap N$ và một phần tử $x - p_N(x)$ của $M \cap N^\circ$, điều này cho (iv).

Ta đã chứng minh a) và phần đầu của b). Bây giờ giả sử rằng $p_M$ và $p_N$ giao hoán và đặt $q = p_M + p_N - p_M p_N$; vì $p_M$ và $p_N$ là các lũy đẳng trong đại số $\mathcal{L}(E)$, q cũng vậy; do đó (GT, III, § 6, No. 2) ảnh của q là một không gian con vectơ đóng của E.

Hiển nhiên ảnh của $q$ được chứa trong $M + N$; tuy nhiên, ta có $p_N(x) = x$, do đó $q(x) = x$ với mọi $x \in N$; vì ta cũng có $q = p_M + p_N - p_N p_M$, suy ra $q(x) = x$ với mọi $x \in M$. Ta kết luận rằng ảnh của $q$ bằng $M + N$. Phần trực giao của $M + N$ bằng $M^\circ \cap N^\circ$, và hạt nhân của $q$ hiển nhiên chứa $M^\circ \cap N^\circ$, do đó $q = p_{M+N}$. Điều này chứng minh $b)$.

Ta có $p_M p_N = 0$ khi và chỉ khi ảnh $N$ của $p_N$ được chứa trong hạt nhân $M^\circ$ của $p_M$, tức là, khi và chỉ khi $M$ vuông góc với $N$. Phần còn lại của mệnh đề $c)$ khi đó là một trường hợp riêng của $b)$.

#### Nhận xét {#evt-v-s1-n6-rem-1 .statement}

— Cho $E$ là một không gian Hilbert và $M, N$ là hai không gian con vectơ đóng của $E$. Quan hệ $M \subset N$ tương đương với tính trực giao của $M$ và $N^\circ$, tức là, với quan hệ $p_M p_{N^\circ} = 0$ theo mệnh đề 9, $c)$. Vì ta có $p_{N^\circ} = 1 - p_N$, ta kết luận rằng *các quan hệ* $M \subset N$ *và* $p_M = p_M p_N$ *là tương đương* (« định lý ba đường vuông góc », *xem* hình 3).

![Biểu đồ cho thấy các không gian con M, N, và các phép chiếu p_M(x), p_N(x)](https://i.imgur.com/3Q5z5QG.png)

Hình 3.

### 7. Đối ngẫu của một không gian Hilbert

#### Định lý 3 {#evt-v-s1-thm-3 .statement}

*Cho $E$ là một không gian Hilbert. Với mỗi $x \in E$, đặt $x^*$ là dạng tuyến tính liên tục $y \mapsto \langle x | y \rangle$ trên $E$; ánh xạ $x \mapsto x^*$ là một ánh xạ song ánh, nửa tuyến tính (đối với tự đẳng cấu $\xi \mapsto \bar{\xi}$) từ $E$ lên đối ngẫu của nó $E'$, và là một đẳng cự từ không gian định chuẩn $E$ lên không gian định chuẩn $E'$.*

Ánh xạ $x \mapsto x^*$ là nửa tuyến tính theo (2) (V, p. 1) và nhờ bất đẳng thức Cauchy-Schwarz, ta có $\|x^*\| = \sup_{\|y\| \leq 1} |\langle x | y \rangle| = \|x\|$, do đó $x \mapsto x^*$ là một đẳng cự từ $E$ vào $E'$, và đặc biệt là đơn ánh. Để hoàn tất chứng minh, ta cần chứng minh rằng với mọi $x' \neq 0$ trong $E'$, tồn tại $x \in E$ sao cho $x' = x^*$. Nhưng siêu phẳng $H = \mathrm{Ker}\, x'$ là đóng trong $E$; phần trực giao của nó là một đường thẳng $D$. Gọi $b$ là một phần tử khác không của $D$; hạt nhân của dạng tuyến tính $b^*$ bằng $H$ và vì thế tồn tại một vô hướng $\lambda \neq 0$ sao cho $x' = \lambda \cdot b^* = (\overline{\lambda} \cdot b)^*$. ĐPCM.

Ánh xạ $x \mapsto x^*$ từ $E$ lên đối ngẫu của nó $E'$ được gọi là *chính tắc*. Ánh xạ nghịch đảo từ $E'$ lên $E$ cũng được gọi là chính tắc và được ký hiệu bởi $x' \mapsto x'^*$. Ta có

$$
\langle x | y \rangle = \langle y, x^* \rangle, \quad \langle x, x' \rangle = \langle x'^* | x \rangle
$$

với $x, y$ trong $E$ và $x'$ trong $E'$. Cũng vậy $(x^*)^* = x$ với $x \in E$.

Khi K là $\mathbf{R}$, ánh xạ $x \mapsto x^*$ là tuyến tính. Ta sẽ chuyển tích vô hướng của E sang E' qua ánh xạ này. Khi $K = \mathbf{C}$, ta có thể xem ánh xạ $x \mapsto x^*$ như một đẳng cấu từ không gian vectơ $\overline{E}$, không gian liên hợp của E, lên E' (V, p. 6). Ta sẽ chuyển tích vô hướng của $\overline{E}$ sang E' qua ánh xạ này.

Trong hai trường hợp xét, E' là một không gian Hilbert và ta có các công thức

$$
\langle x^*|y^* \rangle = \overline{\langle x|y \rangle}, \quad \langle x'|x' \rangle = \|x'\|^2
$$

với $x, y$ trong E và $x'$ trong E'.

Nói rằng vectơ $x \in E$ trực giao với vectơ $y \in E$ là tương đương với nói rằng dạng tuyến tính $x^* \in E'$ trực giao với $y$ theo nghĩa được định nghĩa ở II, p. 41 (điều này biện minh cho việc dùng từ « trực giao » trong hai trường hợp). Nếu M là một không gian con vectơ đóng của E, thì không gian con $M^\circ$ trực giao với M trong E' (II, p. 44) là ảnh qua $x \mapsto x^*$ của phần trực giao của M trong E, được định nghĩa ở V, p. 13 (điều này biện minh cho việc dùng ký hiệu $M^\circ$ trong hai trường hợp).

#### Hệ quả 1 {#evt-v-s1-thm-3-cor-1 .statement}

*Để họ $(x_i)_{i \in I}$ các điểm của một không gian Hilbert E là đầy đủ, thì cần và đủ rằng các hệ thức $\langle x_i|y \rangle = 0$ với $y \in E$ và với mọi chỉ số $i \in I$ kéo theo rằng $y = 0$.*

Thật vậy, điều này nói rằng 0 là vectơ duy nhất của E' trực giao với tất cả các $x_i$ (II, p. 43 và IV, p. 1).

#### Hệ quả 2 {#evt-v-s1-thm-3-cor-2 .statement}

*Cho E và F là hai không gian Hilbert. Với $u \in \mathcal{L}(E; F)$, $x \in E$ và $y \in F$, đặt*

$$
\Phi_u(y, x) = \langle y|u(x) \rangle .
$$

*Ánh xạ $u \mapsto \Phi_u$ là một đẳng cấu từ không gian Banach $\mathcal{L}(E; F)$ lên không gian của tất cả các dạng $^1$ nửa song tuyến tính liên tục trên $F \times E$, được trang bị chuẩn*

$$
\|f\| = \sup_{\substack{x \in E, y \in F \\ \|x\| \leq 1, \|y\| \leq 1}} |f(y, x)| .
$$

Hiển nhiên $\Phi_u$ là nửa song tuyến tính và liên tục với mọi $u \in \mathcal{L}(E; F)$. Ngược lại, cho $f$ là một dạng nửa song tuyến tính liên tục trên $F \times E$. Với mọi $x \in E$, ánh xạ $y \mapsto f(y, x)$ là một dạng tuyến tính liên tục trên không gian Hilbert F. Theo định lý 3, với mọi $x \in E$, tồn tại một phần tử duy nhất $u(x)$ trong F sao cho $f(y, x) = \langle u(x)|y \rangle$ với mọi $y \in F$. Ánh xạ $u : x \mapsto u(x)$ từ E vào F là tuyến tính và ta có

$$
\begin{align*}
\|f\| &= \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |f(y, x)| = \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |\langle y|u(x) \rangle| \\
&= \sup_{\|x\| \leq 1} \|u(x)\| ;
\end{align*}
$$

suy ra $u$ thuộc $\mathcal{L}(E; F)$, $f = \Phi_u$ và $\|u\| = \|f\|$. Điều này chứng minh hệ quả 2.

$^1$ Nhắc lại (A, IX, § 1, No. 5) rằng một dạng nửa song tuyến tính (ở bên trái) $f$ trên $F \times E$ là một ánh xạ từ $F \times E$ vào K thỏa mãn các quan hệ (1) và (2) của V, p. 1.

Ánh xạ chính tắc từ E vào không gian đối ngẫu kép E'' của nó (IV, p. 14) ánh xạ E lên E'', nói cách khác (IV, p. 16), E là một không gian Banach phản xạ. Thật vậy, nếu E là một không gian Hilbert thực (resp. phức), thì ánh xạ chính tắc $\phi$ từ E' lên E là một đẳng cấu từ không gian định chuẩn E' lên E (resp. lên không gian liên hợp $\overline{E}$ của E); áp dụng định lý 3 cho E (resp. E), ta thấy rằng mọi dạng tuyến tính liên tục trên không gian định chuẩn E' đều có dạng $x' \mapsto \langle \phi(x')|x \rangle = \langle x, x' \rangle$ với $x \in E$, do đó mệnh đề của chúng ta suy ra.

Như một hệ quả (IV, p. 17, mệnh đề 6):

#### Định lý 4 {#evt-v-s1-thm-4 .statement}

*Trong một không gian Hilbert E, quả cầu đơn vị là compact yếu.*

#### Mệnh đề 10 {#evt-v-s1-prop-10 .statement}

*Nếu, trong một không gian Hilbert E, một bộ lọc $\mathfrak{F}$ hội tụ yếu tới $x_0$, và nếu hơn nữa $\lim_{\mathfrak{F}} \|x\| = \|x_0\|$, thì $\mathfrak{F}$ hội tụ tới $x_0$ đối với tôpô ban đầu của E.*

Thật vậy, $\|x - x_0\|^2 = \|x\|^2 - 2\Re \langle x|x_0 \rangle + \|x_0\|^2$. Vì $\langle x|x_0 \rangle$ tiến tới $\|x_0\|^2$ theo $\mathfrak{F}$ theo giả thiết, và $\|x\|$ tiến tới $\|x_0\|$ theo $\mathfrak{F}$, nên $\|x - x_0\|$ tiến tới 0 theo $\mathfrak{F}$, do đó mệnh đề.

#### Nhận xét {#evt-v-s1-n7-rem-1 .statement}

— Nếu E là một không gian tiền Hilbert Hausdorff và $\hat{E}$ là bao đóng Hilbert của E, ta biết (III, p. 16) rằng đối ngẫu E' của E có thể được đồng nhất với đối ngẫu của $\hat{E}$; khi đó từ định lý 3 (V, p. 15) suy ra rằng mọi dạng tuyến tính liên tục trên E có thể được viết một cách duy nhất dưới dạng $x \mapsto \langle a|x \rangle$, với $a \in \hat{E}$.

### Bài tập {#evt-v-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
