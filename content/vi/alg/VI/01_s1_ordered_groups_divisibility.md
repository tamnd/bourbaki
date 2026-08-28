---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 1
section_title: Ordered groups. Divisibility
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0312-0330, 0341-0348
extraction: ocr
subsections:
    - "no": 1
      title: Definition of ordered monoids and groups
      page: 0
      pdf_page: 312
    - "no": 2
      title: Pre-ordered monoids and groups
      page: 3
      pdf_page: 314
    - "no": 3
      title: Positive elements
      page: 3
      pdf_page: 314
    - "no": 4
      title: Filtered groups
      page: 4
      pdf_page: 315
    - "no": 5
      title: Divisibility relations in a field
      page: 5
      pdf_page: 316
    - "no": 6
      title: Elementary operations on ordered groups
      page: 7
      pdf_page: 318
    - "no": 7
      title: Increasing homomorphisms of ordered groups
      page: 7
      pdf_page: 318
    - "no": 8
      title: Suprema and infima in an ordered group
      page: 8
      pdf_page: 319
    - "no": 9
      title: Lattice ordered groups
      page: 10
      pdf_page: 321
    - "no": 10
      title: The decomposition theorem
      page: 11
      pdf_page: 322
    - "no": 11
      title: Positive and negative parts
      page: 12
      pdf_page: 323
    - "no": 12
      title: Coprime elements
      page: 13
      pdf_page: 324
    - "no": 13
      title: Irreducible elements
      page: 17
      pdf_page: 328
statements: 52
exercises: 34
content_sha256: e3e585a2a4aeab33f921b3d9db8806be1e051cd589eb4b681c324c1c14dc83ac
translated_from: content/en/alg/VI/01_s1_ordered_groups_divisibility.md
source_content_sha256: 5dfbd1ec95d8ba9a7a5492cea424d8856e8b03e0d486d93477fdfa800389bdd9
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-a2a28731
glossary_version: 34
glossary_terms_sha256: 2018b3110938eb96099782e0d5944f31d223e11c6135798e6844d84465ceca1b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. NHÓM CÓ THỨ TỰ. TÍNH CHIA HẾT

Các khái niệm và kết quả được trình bày trong mục này liên quan đến việc nghiên cứu các quan hệ thứ tự trong các nửa nhóm giao hoán (I, p. 12, Định nghĩa 2), trường hợp quan trọng nhất là các nhóm Abel. Trừ khi có nói rõ khác đi, chúng ta sẽ dùng ký hiệu cộng tính cho luật hợp thành trong tất cả các nhóm và nửa nhóm được xét. Mặt khác, khi tiếp tục, chúng ta sẽ trình bày một số ứng dụng đại số quan trọng của lý thuyết các nhóm và nửa nhóm có thứ tự, và theo đó sẽ chuyển một số kết quả của chúng ta sang ký hiệu nhân tính thích hợp cho các ứng dụng này.

### 1. Định nghĩa các nửa nhóm và nhóm có thứ tự

#### Định nghĩa 1 {#alg-vi-s1-def-1 .statement}

— Một cấu trúc nửa nhóm giao hoán (được viết theo cộng tính) và một thứ tự (được viết $\leq$) trên một tập hợp $M$ được gọi là tương thích nếu chúng thỏa mãn tiên đề sau:

(OM) Với mỗi $z \in M$, quan hệ $x \leq y$ kéo theo $x + z \leq y + z$.

Một tập hợp $M$ được trang bị một cấu trúc nửa nhóm giao hoán và một thứ tự tương thích với nhau được gọi là một nửa nhóm có thứ tự; nếu cấu trúc nửa nhóm giao hoán của nó là một cấu trúc nhóm, thì nó được gọi là một nhóm có thứ tự.

Theo cách tương tự, ta có thể định nghĩa khái niệm một nửa nhóm có thứ tự không giao hoán (VI, p. 30, Bài tập 1).

Nếu một thứ tự tương thích với một cấu trúc nửa nhóm đã cho, thì thứ tự đối cũng vậy.

#### Ví dụ 1 {#alg-vi-s1-n1-exa-1 .statement}

Nhóm cộng của các số nguyên hữu tỉ, và nhóm cộng của các số hữu tỉ, là các nhóm có thứ tự đối với thứ tự được định nghĩa trong I, pp. 21 và 117. *Điều tương tự cũng đúng đối với nhóm cộng của các số thực (Gen. Top., IV, p 3). \*

#### Ví dụ 2 {#alg-vi-s1-n1-exa-2 .statement}

*Nhóm cộng của các hàm số hữu hạn có giá trị số được định nghĩa trên một tập hợp $E$ là một nhóm có thứ tự đối với thứ tự « $f(x) \leq g(x)$ với mọi $x \in E$ », được viết $f \leq g$. Quan hệ này nói rằng đồ thị của hàm $f$ nằm bên dưới đồ thị của hàm $g$. Đôi khi người đọc có thể thấy thuận tiện khi suy nghĩ theo cách biểu diễn bằng đồ thị này. \*

Theo các định nghĩa tổng quát (Lý thuyết tập hợp, IV, p. 264), một ánh xạ song ánh $f$ từ một nửa nhóm có thứ tự M lên một nửa nhóm có thứ tự M' được gọi là một *đẳng cấu* của M lên M' nếu cấu trúc của M' thu được từ cấu trúc của M bằng cách vận chuyển nó theo $f$. Điều này tương đương với việc nói rằng $f$ là một ánh xạ *lên* M' sao cho

$$
f(x + y) = f(x) + f(y)
$$

(tức là một đồng cấu của nửa nhóm M lên nửa nhóm M'), và các quan hệ $x \leq y$ và $f(x) \leq f(y)$ là tương đương (do đó đặc biệt $f(x) = f(y)$ kéo theo $x = y$, nghĩa là $f$ là đơn ánh).

#### Mệnh đề 1 (« phép cộng các bất đẳng thức ») {#alg-vi-s1-prop-1 .statement}

— *Trong một nửa nhóm có thứ tự M*, cho $(x_i)$ và $(y_i)$ ($1 \leq i \leq n$) là hai dãy gồm n phần tử sao cho $x_i \leq y_i$ với mọi $i$; khi đó ta có

$$
x_1 + \cdots + x_n \leq y_1 + \cdots + y_n
$$

*Nếu hơn nữa tất cả các phần tử $x_i, y_i$ đều giản ước được (I, p. 15, Định nghĩa 5) (đặc biệt nếu M là một nhóm), và nếu $x_i < y_i$ đối với một $i$ nào đó, thì*

$$
x_1 + \cdots + x_n < y_1 + \cdots + y_n .
$$

Trường hợp tổng quát quy về trường hợp $n = 2$ bằng quy nạp, sử dụng sự kiện rằng tổng của các phần tử giản ước được là giản ước được cho khẳng định thứ hai (I, p. 15, Mệnh đề 2). Khẳng định thứ nhất suy ra từ các quan hệ

$$
x_1 + x_2 \leq x_1 + y_2 \quad \text{và} \quad x_1 + y_2 \leq y_1 + y_2 ,
$$

là các hệ quả của các giả thiết và của (OM). Khi đó, quan hệ

$$
x_1 + x_2 = y_1 + y_2
$$

sẽ kéo theo

$$
x_1 + x_2 = x_1 + y_2 = y_1 + y_2 ,
$$

do đó $x_2 = y_2$ và $x_1 = y_1$ nếu $x$, và $y_2$ là giản ước được, điều này chứng minh khẳng định thứ hai.

#### Mệnh đề 2 {#alg-vi-s1-prop-2 .statement}

*Trong một nhóm có thứ tự G*, các quan hệ $x \leq y$ *và* $x + z \leq y + z$ *là tương đương*.

Thật vậy, ta có thể thu được mỗi quan hệ từ quan hệ kia bằng cách cộng $z$ hoặc $(-z)$ vào hai vế.

Sự kiện này có thể được diễn đạt bằng cách nói rằng, trong một nhóm có thứ tự G, thứ tự là *bất biến qua phép tịnh tiến*. Nói cách khác, một phép tịnh tiến là một *tự đẳng cấu* của *thứ tự* của một nhóm có thứ tự.

#### Hệ quả {#alg-vi-s1-n1-cor-1 .statement}

— Trong một nhóm có thứ tự $G$, các quan hệ $x \leq y$, $0 \leq y - x$, $x - y \leq 0$ và $-y \leq -x$ là tương đương.

Thật vậy, ta áp dụng Mệnh đề 2, lần lượt lấy $z = -x$, $z = -y$ và $z = -(x + y)$.

Đặc biệt ta suy ra từ hệ quả này rằng nếu $G$ là một nhóm có thứ tự, ánh xạ $x \mapsto -x$ từ $G$ vào chính nó biến thứ tự của $G$ thành thứ tự đối.

### 2. Các nửa nhóm và nhóm tiền thứ tự

Nhắc lại rằng nếu một quan hệ $x \leq y$ giữa các phần tử của một tập hợp $E$ là phản xạ và bắc cầu, thì nó được gọi là một quan hệ tiền thứ tự (Lý thuyết tập hợp, III, p. 133). Quan hệ « $x \leq y$ và $y \leq x$ » là một quan hệ tương đương $S$ trên $E$, tương thích với quan hệ $x \leq y$; khi chuyển qua thương, quan hệ $\leq$ sinh ra một quan hệ thứ tự trên $E/S$, gọi là quan hệ thứ tự liên kết với $\leq$.

#### Định nghĩa 2 {#alg-vi-s1-def-2 .statement}

— Một quan hệ tiền thứ tự (viết $\leq$) và một cấu trúc monoid giao hoán (viết theo phép cộng) trên một tập hợp $M$ được gọi là tương thích nếu chúng thỏa mãn tiên đề sau:

(POM) Với mỗi $z \in M$, quan hệ $x \leq y$ kéo theo $x + z \leq y + z$.

Một tập hợp $M$ được trang bị một cấu trúc monoid giao hoán và một quan hệ tiền thứ tự tương thích với nhau được gọi là một monoid tiền thứ tự.

Cho $M$ là một monoid tiền thứ tự, và $S$ là quan hệ tương đương « $x \leq y$ và $y \leq x$ ». Theo (POM), quan hệ $x \equiv x' \pmod{S}$ kéo theo $x + y \leq x' + y$ và $x' + y \leq x + y$ với mọi $y \in M$, nghĩa là $x + y \equiv x' + y \pmod{S}$. Nói cách khác, quan hệ tương đương $S$ tương thích với phép cộng trong $M$ (I, p. 11). Do đó thương theo $S$ của luật cộng trên $M$, cùng với thứ tự liên kết với $\leq$, cho $M/S$ cấu trúc của một monoid có thứ tự. Trong trường hợp $M$ là một nhóm tiền thứ tự, nhóm $M/S$ là thương của $M$ theo nhóm con gồm tất cả các phần tử $x$ sao cho $x \leq 0$ và $0 \leq x$.

### 3. Các phần tử dương

Cho $G$ là một nhóm tiền thứ tự với quan hệ tiền thứ tự $\leq$; nếu $0 \leq x$ và $0 \leq y$ thì ta suy ra rằng $y \leq x + y$ theo (POM), và do đó $0 \leq x + y$ theo tính bắc cầu; điều này nói rằng tập hợp $G_+$ gồm các phần tử $x \in G$ sao cho $0 \leq x$ là đóng đối với phép cộng; hơn nữa, quan hệ $x \leq y$ tương đương với $0 \leq y - x$, nghĩa là $y - x \in G_+$. Ngược lại:

#### Mệnh đề 3 {#alg-vi-s1-prop-3 .statement}

— Nếu $P$ là một tập con của một nhóm Abel $G$, chứa $0$ và sao cho $P + P \subset P$, thì quan hệ $y - x \in P$ là một quan hệ tiền thứ tự tương thích với cấu trúc nhóm của $G$. Để quan hệ này làm cho $G$ thành một nhóm có thứ tự, điều kiện cần và đủ là có $P \cap (-P) = \{0\}$; để $G$ là một nhóm được sắp thứ tự toàn phần theo thứ tự này, điều kiện cần và đủ là ngoài ra còn có $P \cup (-P) = G$.

Hiển nhiên là quan hệ $y - x \in P$ có tính phản xạ và bắc cầu, và (nếu được viết là $x \leq y$) thỏa mãn tiên đề *POM*. Để chứng minh mệnh đề thứ hai, chỉ cần nhận xét rằng $P \cap (-P)$ là nhóm con $G'$ gồm các phần tử $x$ sao cho $0 \leq x$ và $x \leq 0$. Cuối cùng, nói rằng $G$ được sắp thứ tự toàn phần có nghĩa là, với mỗi cặp phần tử $x, y$ của $G$, ít nhất một trong các phần tử $x - y, y - x$ thuộc $P$, điều này hoàn thành chứng minh.

#### Định nghĩa 3 {#alg-vi-s1-def-3 .statement}

*Trong một nhóm có thứ tự $G$, mọi phần tử $x$ sao cho $0 \leq x$ (resp. $x \leq 0$) được gọi là một phần tử dương (resp. âm).*

Chú ý rằng $0$ là phần tử duy nhất *vừa dương vừa âm* ; mọi phần tử $x$ sao cho $0 < x$ (resp. $x < 0$) được gọi là *dương ngặt* (resp. *âm ngặt*).

#### Ví dụ {#alg-vi-s1-n3-exa-1 .statement}

— Trong nhóm cộng $\mathbf{Z} \times \mathbf{Z}$, cho $P$ là tập hợp các phần tử $(x, y)$ thỏa mãn hai bất đẳng thức $ax + by \geq 0$ và $cx + dy \geq 0$, trong đó $a, b, c, d$ là các số nguyên (* hoặc các số thực *) sao cho $ad - bc \neq 0$; « nón » $P$ thỏa mãn hai điều kiện đầu của Mệnh đề 3. Bằng cách này có thể xác định các thứ tự khác nhau tương thích với cấu trúc nhóm của $\mathbf{Z} \times \mathbf{Z}$; nhóm này không được sắp thứ tự toàn phần theo bất kỳ thứ tự nào trong các thứ tự này.

#### Nhận xét {#alg-vi-s1-n3-rem-1 .statement}

— Theo điều kiện $P + P \subset P$, quan hệ $x \geq 0$ trong một nhóm có thứ tự kéo theo rằng $nx \geq 0$ với mọi số tự nhiên $n$. Nếu ngoài ra phần tử dương $x$ của $G$ có cấp hữu hạn $n$, thì $-x = (n-1)x$ là dương ; vì

$$
P \cap (-P) = \{0\},
$$

điều này kéo theo $x = 0$. Đặc biệt, nếu mọi phần tử của $G$ đều có cấp hữu hạn, thì $P = \{0\}$; quan hệ $x \leq y$ khi đó tương đương với $x = y$ (thứ tự *rời rạc*).

### 4. Các nhóm lọc

Nhắc lại (*Lý thuyết tập hợp*, III, p. 145) rằng một tập hợp có thứ tự $G$ là *lọc phải* (resp. *lọc trái*)\footnote{1} nếu với mỗi cặp $(x, y)$ các phần tử của $G$ tồn tại $z \in G$ sao cho $x \leq z$ và $y \leq z$ (resp. $z \leq x$ và $z \leq y$). Mọi nhóm có thứ tự lọc phải $G$ cũng là lọc trái và ngược lại : thật vậy, vì tồn tại $z \in G$ sao cho $-x \leq z$ và $-y \leq z$, ta có $-z \leq x$ và $-z \leq y$ (VI, p. 3, Hệ quả). Do đó ta sẽ chỉ nói về các nhóm lọc.

#### Mệnh đề 4 {#alg-vi-s1-prop-4 .statement}

*Để một nhóm có thứ tự $G$ là lọc thì điều kiện cần và đủ là nó được sinh bởi các phần tử dương của nó, nghĩa là mọi phần tử là hiệu của hai phần tử dương.*

Thật vậy, nếu $G$ là có hướng, thì với mỗi $x \in G$ tồn tại một phần tử dương $z$ sao cho $x \leq z$, và $x$ là hiệu của hai phần tử dương $z$ và $z - x$. Ngược lại, nếu $x = u - v$ và $y = w - t$ với $u, v, w, t$ dương, thì phần tử $u + w$ lớn hơn $x$ và lớn hơn $y$.

1 Thuật ngữ được sử dụng trong *loc. cit.* là *có hướng*.

#### Mệnh đề 5 {#alg-vi-s1-prop-5 .statement}

— *Nếu* $(x_i)$ *là một họ hữu hạn các phần tử của một nhóm có hướng G, thì tồn tại* $z \in G$ *sao cho* $x_i + z$ *là dương với mỗi i.*

*Nếu* $x_i = u_i - v_i$, *với* $u_i$ *và* $v_i$ *dương, thì chỉ cần lấy* $z$ *là tổng của họ* $(v_i)$.

### 5. Các quan hệ chia hết trong một trường

Ở đây ta sẽ định nghĩa một số nhóm có thứ tự đóng vai trò quan trọng trong đại số. Ký hiệu thường dùng cho các nhóm này là ký hiệu nhân; do đó, việc áp dụng các kết quả đã thu được trong ký hiệu cộng tính cho các nhóm này giả định trước việc chuyển sang ký hiệu nhân — điều này hẳn không gây khó khăn cho người đọc. *Trong suốt tiết diện này, chữ A sẽ ký hiệu một miền nguyên và K là trường phân thức của nó* (*l*, p. 116).

Trong nhóm nhân $\mathbf{K}^*$ gồm các phần tử khác không của $\mathbf{K}$, tập hợp P gồm các phần tử khác không của A đóng đối với phép nhân, vì A là một vành. Do đó nó định nghĩa một quan hệ thứ tự trước trên $\mathbf{K}^*$ bởi $x^{-1}y \in P$, nghĩa là « tồn tại $z \in P$ sao cho $y = zx$ », khiến $\mathbf{K}^*$ trở thành một *nhóm có thứ tự trước* (viết theo ký hiệu nhân) (*VI*, p. 3, Prop. 3). Mở rộng thuật ngữ liên quan đến các phần tử của A (I, p. 97) sang $\mathbf{K}^*$, quan hệ $x^{-1}y \in P$ cũng có thể được phát biểu là: *x chia hết y*, hoặc x là một *ước của y*, hoặc y là một *bội của x* (đối với vành A); và ta sẽ gọi quan hệ $x^{-1}y \in P$ là *quan hệ chia hết* trong $\mathbf{K}^*$ đối với vành A. Quan hệ « x 'chia hết y » được ký hiệu $x \mid y$, và phủ định của nó là $x \nmid y$. Các phần tử của P không gì khác hơn là các *bội của 1*.

#### Nhận xét 1 {#alg-vi-s1-n5-rem-1 .statement}

Quan hệ chia hết trong $\mathbf{K}^*$ phụ thuộc một cách cốt yếu vào vành A cụ thể. Nếu $A = K$ ta thu được quan hệ « tầm thường », theo đó $x \mid y$ với mọi cặp $(x, y)$ các phần tử của $\mathbf{K}^*$. Cho p và q là các số nguyên tố; các số hữu tỉ r/s mà mẫu số không là bội của $p$ (tương ứng q) lập thành một vành con $\mathbf{Z}_{(p)}$ (tương ứng $\mathbf{Z}_{(q)}$) của $\mathbf{Q}$; các quan hệ chia hết trong $\mathbf{Q}^*$ tương ứng với hai vành này là phân biệt nếu $p \neq q$, số $p/q$ là một bội của 1 theo một quan hệ nhưng không phải theo quan hệ kia.

#### Nhận xét 2 {#alg-vi-s1-n5-rem-2 .statement}

Đôi khi ta sẽ mở rộng định nghĩa của quan hệ $x \mid y$ cho các cặp phần tử của $\mathbf{K}$ (thay vì chỉ $\mathbf{K}^*$), trong đó quan hệ này được hiểu là « tồn tại $z \in A$ sao cho $y = zx$ »; do đó ta sẽ có $x \mid 0$ với mọi $x \in K$. Điều này cho phép ta phát biểu các kết quả sau mà không có hạn chế: nếu $x \mid y$ và $x \mid z$ thì $x \mid (y - z)$; nếu $x \mid y$ và $x \nmid z$ thì $x \nmid (y - z)$. Theo cùng cách đó ta có thể mở rộng toàn bộ thuật ngữ tương ứng.

Để thu được một *quan hệ thứ tự* (No. 2) từ quan hệ chia hết, ta phải chuyển qua nhóm thương của $\mathbf{K}^*$ theo nhóm con $\mathbf{A}^*$ gồm các phần tử $x \in \mathbf{K}^*$ sao cho $x \mid 1$ và $1 \mid x$; đó là các phần tử của P là *ước của 1*, tức là các phần tử *khả nghịch* của $A$; do lạm dụng ngôn ngữ, chúng thường được gọi là các đơn vị của vành A. Khi đó nhóm thương $\mathbf{K}^*/\mathbf{A}^*$ là một nhóm có thứ tự. Hai phần tử $x$ và $y$ của $\mathbf{K}^*$ thuộc cùng một lớp kề của $\mathbf{A}^*$ được gọi là *liên hợp*; điều này có nghĩa là $x \mid y$ và $y \mid x$. Ngược lại, nếu x chia hết y mà y không chia hết x, ta nói rằng x chia ngặt y, hoặc x là một ước ngặt của y, hoặc y là một bội ngặt của x.

Chú ý rằng $K^*/A^*$ là một nhóm *lọc*, vì K là trường các phân thức của A (VI, p. 4, Prop. 4).

Nói rằng hai phần tử x và y của $K^*$ là liên hợp cũng chính là nói rằng chúng có *cùng* các bội trong K, theo tính bắc cầu của quan hệ chia hết. Với mọi $x \in K$, ta sẽ ký hiệu $Ax$ là tập hợp tất cả các phần tử zx với $z \in A$; tập hợp $Ax$ là một môđun con của K, xem như một A-môđun. Mở rộng thuật ngữ liên quan đến trường hợp $x \in A$, ta sẽ gọi nó là một iđêan phân thức chính của trường K đối với vành A. Trái lại, các iđêan của vành A được gọi là nguyên.

Chú ý rằng nếu $A \neq K$ thì một iđêan phân thức chính $\neq \{0\}$ không phải là một iđêan của K được xem như một vành.

Iđêan phân thức chính $Ax$ còn được ký hiệu là (x). Ta sẽ viết $x \equiv 0$ (mody) với $x \in Ay$ và $x \equiv x'$ (mody) với $x - x' \in Ay$; nếu $x \equiv x'$ (mody) thì $zx \equiv zx'$ (mod $zy$) với mọi $z \in K$.

Chú ý rằng $x \equiv x'$ (mod y) không kéo theo $zx \equiv zx'$ (mod y) trừ khi $z \in A$. Do đó trong $\mathbf{Q}$, đối với $\mathbf{Z}$, ta có $4 \equiv 2$ (mod 2) nhưng không có $2 \equiv 1$ (mod 2).

Quan hệ $x | y$ hiển nhiên tương đương với $(x) \supset (y)$. Ánh xạ $x \mapsto (x)$ từ $K^*$ lên tập hợp $\mathcal{P}^*$ các iđêan phân thức chính $\neq (0)$ của K, do đó xác định, khi chuyển qua thương, một ánh xạ song ánh từ $K^*/A^*$ lên $\mathcal{P}^*$; chuyển cấu trúc nhóm của $K^*/A^*$ sang $\mathcal{P}^*$ bằng ánh xạ này, ta được định nghĩa tích của hai iđêan phân thức chính (x) và (y) là iđêan (xy ), chỉ phụ thuộc vào (x) và (y). Được trang bị luật này và quan hệ thứ tự $(x) \supset (y)$, tập hợp $\mathcal{P}^*$ là một nhóm có thứ tự, đẳng cấu với $K^*/A^*$. Theo quy ước, ta sẽ đồng nhất $\mathcal{P}^*$ với $K^*/A^*$ qua ánh xạ trên.

Chú ý rằng quan hệ « x chia hết y », trong trường hợp các số nguyên dương, kéo theo x nhỏ hơn y, tương ứng với bao hàm $(x) \supset (y)$, trong đó iđêan (x) « lớn hơn » iđêan (y). Ta có thể ghi nhớ sự « đảo thứ tự » này bằng cách nhận xét rằng chẳng hạn 7 có « nhiều bội hơn » 91.

Nếu mở rộng quan hệ $x | y$ đến mọi phần tử của K, quan hệ này vẫn tương đương với $(x) \supset (y)$ trong tập hợp $\mathcal{P}$ gồm tất cả các iđêan phân thức chính của K (trong đó $(0)$ là phần tử nhỏ nhất theo quan hệ bao hàm).

Như trong các tiết trước, nói chung trong phần tiếp theo ta sẽ dùng ký hiệu cộng tính. Tuy nhiên, thuật ngữ liên quan đến tính chia hết sẽ được đưa vào theo thuật ngữ cộng tính tương ứng, trong các đoạn được mở đầu bằng dấu (DIV) (trong đó hiểu rằng ký hiệu được sử dụng là ký hiệu của tiết hiện tại). Để giúp người đọc dễ dàng hơn, một số kết quả sẽ được chuyển sang ngôn ngữ của tính chia hết, chẳng hạn bản dịch của Prop. 7 được ký hiệu là « PROPOSITION 7 (DIV) ».

### 6. Các phép toán sơ cấp trên các nhóm có thứ tự

Cho H là một nhóm con của một nhóm có thứ tự G; rõ ràng hạn chế của quan hệ thứ tự của G lên H tương thích với cấu trúc nhóm của H; ta luôn lấy H được sắp thứ tự theo cách này, trừ khi có nói khác. Nếu P là tập hợp các phần tử dương của G thì tập hợp các phần tử dương của H là H ∩ P.

Cho (G,) là một họ các nhóm có thứ tự; theo định nghĩa tích của các tập hợp có thứ tự (Set Theory, III, p. 137), nhóm tích G = $\prod G_i$ được trang bị một quan hệ thứ tự, quan hệ « (x,) ≤ (y,) » giữa hai phần tử của G theo định nghĩa chính là « x, ≤ y, với mọi α ». Ngay lập tức thấy rằng quan hệ thứ tự này tương thích với cấu trúc nhóm của G; quan hệ thứ tự này làm cho G thành một nhóm có thứ tự mà ta gọi là tích của các nhóm có thứ tự G,. Các phần tử dương của G là những phần tử mà mọi thành phần đều dương. Trong trường hợp tất cả các thừa số G, đều đồng nhất với cùng một nhóm có thứ tự H, thì G là nhóm H' các ánh xạ từ tập hợp chỉ số I vào H, quan hệ « f ≤ g » giữa hai ánh xạ từ I vào H chính là « f(α) ≤ g(α) với mọi α ∈ I »; các ánh xạ dương là những ánh xạ chỉ nhận các giá trị dương. Tổng trực tiếp của một họ (G,) các nhóm có thứ tự được định nghĩa là một nhóm con có thứ tự của tích của chúng (II, p. 202).

Cho (G_i)_i, là một họ các nhóm có thứ tự mà tập hợp chỉ số I được sắp thứ tự tốt: nhắc lại (Set Theory, III, p. 157) rằng một quan hệ thứ tự, gọi là quan hệ thứ tự từ điển, được xác định trên tập tích G = $\prod G_i$, quan hệ « (x,) < (y,) » giữa hai phần tử của G theo định nghĩa chính là « nếu β là chỉ số nhỏ nhất trong các chỉ số i sao cho x_i ≠ y_i, thì x_β < y_β ». Nhắc lại rằng tích của một họ được sắp thứ tự tốt các tập hợp được sắp thứ tự toàn phần là được sắp thứ tự toàn phần theo quan hệ thứ tự từ điển. Trong trường hợp tổng quát, quan hệ thứ tự từ điển trên G tương thích với cấu trúc nhóm của nó, như được kiểm tra ngay lập tức; được trang bị quan hệ thứ tự này, nhóm G do đó là một nhóm có thứ tự, gọi là tích từ điển của họ được sắp thứ tự tốt các nhóm có thứ tự (G,).

#### Nhận xét 1 {#alg-vi-s1-n6-rem-1 .statement}

Trong những trường hợp thường gặp nhất, tập chỉ số có thứ tự tốt I sẽ là một khoảng hữu hạn (1, n) trong N.
    2) Tập hợp các phần tử dương của tích từ điển G gồm 0 và những phần tử khác không mà thành phần khác không có chỉ số nhỏ nhất là dương.

### 7. Đồng cấu tăng của các nhóm có thứ tự

Cho G và G' là hai nhóm có thứ tự; trong số các đồng cấu f từ nhóm cộng cơ sở của G vào nhóm cộng cơ sở của G', ta có thể xét các ánh xạ tăng, tức là những ánh xạ sao cho x ≤ y kéo theo f(x) ≤ f(y). Do quan hệ $f(y - x) = f(y) - f(x)$, suy ra rằng các đồng cấu tăng từ G vào G' được đặc trưng bởi tính chất ảnh của một phần tử dương của G qua một đồng cấu như vậy là một phần tử dương của G'; nếu P (resp. P') ký hiệu tập hợp các phần tử dương của G (resp. G'), điều này có thể viết là $f(P) \subset P'$. Rõ ràng đơn ánh chính tắc của một nhóm con G vào một nhóm có thứ tự G', và phép chiếu của một tích các nhóm có thứ tự lên một trong các thừa số của nó, là các đồng cấu tăng.

Một đẳng cấu (VI, p. 2) $f$ từ một nhóm có thứ tự G lên một nhóm có thứ tự G' là một đồng cấu song ánh từ G lên G' sao cho cả $f$ lẫn đồng cấu nghịch đảo đều tăng, nói cách khác $f(P) = P'$.

Có thể xảy ra trường hợp một đẳng cấu từ nhóm cơ sở của G lên nhóm cơ sở của G' là tăng mà đẳng cấu nghịch đảo không tăng. Chẳng hạn, điều này xảy ra nếu $G = G'$, nếu $f$ là ánh xạ đồng nhất trên G, và nếu $P \subset P'$ nhưng $P \neq P'$. Do đó trong $\mathbf{Z}$ ta có thể lấy $P'$ là tập hợp các số nguyên dương (thông thường) và P là tập hợp các số nguyên dương chẵn.

(DIV) Cho K là trường các hàm hữu tỉ $F_2(X)$ trên trường $F_2$ có cấp 2. Các quan hệ chia hết tương ứng với các vành $F_2[X] = A'$ và $F_2[X^2, X^3] = A$ xác định hai cấu trúc nhóm có thứ tự phân biệt trên $K^*$, sao cho $A \subset A'$ (chúng là các cấu trúc nhóm có thứ tự vì 1 là phần tử khả nghịch duy nhất trong A và phần tử khả nghịch duy nhất trong A').

### 8. Cực đại và cực tiểu trong một nhóm có thứ tự

Nhắc lại (Lý thuyết tập hợp, III, p. 141) rằng nếu tập hợp các cận trên của một tập con F của một tập hợp có thứ tự E (tức là tập hợp các $z \in E$ sao cho $x \leq z$ với mọi $x \in F$) có một phần tử nhỏ nhất a, thì phần tử này, khi đó là duy nhất, được gọi là cực đại của F. Nếu F là tập hợp các phần tử trong một họ $(x_i)_i$, gồm các phần tử của E, thì cực đại của nó, nếu tồn tại, được ký hiệu là $\sup x_i$ (hoặc $\sup x_i$ hoặc đơn giản là $\sup(x_i)$); nếu đó là một họ hữu hạn $(x_i)$ ($1 \leq i \leq n$), cực đại này còn được ký hiệu là $\sup_{\text{LEI}} (x_1, \ldots, x_n)$. Cực tiểu được định nghĩa tương tự và được ký hiệu là inf. Các phép toán sup và inf là kết hợp và giao hoán.

Nhắc lại (Lý thuyết tập hợp, loc. cit.) rằng nếu F là một tập con của một tập hợp có thứ tự E, và $(x_i)$ là một họ các phần tử của F, thì sự tồn tại của $\sup(x_i)$ trong E (có thể ký hiệu là $\sup_E(x_i)$) không kéo theo sự tồn tại của một cực đại của các $x_i$ trong F (có thể ký hiệu là $\sup_F(x_i)$ khi nó tồn tại); nếu cả hai đều tồn tại thì ta chỉ biết rằng $\sup_E(x_i) \leq \sup_F(x_i)$; tuy nhiên nếu $\sup_E(x_i)$ tồn tại và thuộc F, thì $\sup_F(x_i)$ tồn tại và bằng $\sup_E(x_i)$. Chẳng hạn, trong vành đa thức $A = K[X, Y]$ (K là một trường), các iđêan chính AX và AY có iđêan $AX + AY$ làm cực đại (theo quan hệ $\subset$) trong tập hợp có thứ tự gồm các iđêan của A, nhưng có iđêan A làm cực đại trong tập hợp tất cả các iđêan chính của A.

(DIV) Một phần tử d của $K^*$ được gọi là một ước chung lớn nhất, viết tắt là gcd, của một họ $(x_i)$ các phần tử của $K^*$, nếu iđêan phân thức chính (d) là supremum trong $\mathcal{P}^*$ (theo quan hệ $\subset$) của họ các iđêan $((x_i))$, hay nói cách khác nếu quan hệ $z \mid d$ với $z \in K^*$ tương đương với « $z \mid x_i$ với mọi $i$ ». Tương tự, ta nói rằng $m \in K^*$ là một bội chung nhỏ nhất, hay một lcm, của họ $(x_i)$ nếu $(m)$ là infimum trong $\mathcal{P}^*$ của họ các iđêan $((x_i))$, tức là nếu m | z tương đương với « x_i | z với mọi i ». Nói $(m) = \cap_{i} (x_i)$ cũng là điều tương đương; thật vậy, điều kiện $x_i | z$ với mọi $i$ tương đương với $z \in A x$, với mọi $i$, tức là $z \in \cap_{i} (x_i)$, và điều kiện $m | z$ tương đương với $z \in (m)^1$.

Chú ý rằng nếu một iđêan phân thức chính (d) thỏa mãn $(d) = \sum (x_i)$ thì d là một gcd của họ $(x_i)$; nhưng ngược lại, một gcd của $(x_i)$ không nhất thiết thỏa mãn điều kiện trên (xem VI, p. 33, Ex. 24).

Gcd và lcm, nếu tồn tại, được xác định duy nhất modulo nhóm con U các đơn vị của $K^*$, tức là hai gcd (hoặc hai lcm) của một họ đã cho là liên kết; do lạm dụng ngôn ngữ, ta thường viết gcd$(x_i)$ và lcm$(x_i)$ cho bất kỳ gcd hoặc lcm nào của họ $(x_i)$, khi những phần tử như vậy tồn tại.

(DIV) Do lạm dụng ngôn ngữ, đôi khi ta mở rộng khái niệm gcd cho một họ $(x_i)$ các phần tử của K, trong đó một số phần tử có thể bằng không; gcd này lại được định nghĩa là một phần tử d sao cho quan hệ $z | d$ tương đương với « $z | x_i$ với mọi $i$ »; rõ ràng d bằng 0 nếu tất cả các $x_i$ đều bằng không; nếu không thì d là một gcd của các $x_i$ khác không. Tương tự, lcm của một họ mà một số phần tử có thể bằng không là 0.

Trong một nhóm có thứ tự G, một hệ quả ngay lập tức của tính bất biến qua phép tịnh tiến của thứ tự (VI, p. 2, Prop. 2) là

(1)
$$
\sup(z + x_i) = z + \sup(x_i)
$$
theo nghĩa là, bất cứ khi nào một vế được xác định thì vế kia cũng được xác định và hai vế bằng nhau. Tương tự, từ sự kiện ánh xạ $x \mapsto -x$ biến thứ tự của G thành thứ tự đối (VI, p. 3, Cor.) suy ra rằng

(2)
$$
\inf(-x_i) = -(\sup(x_i)),
$$
quan hệ này được hiểu theo cùng nghĩa như quan hệ trước.

#### Mệnh đề 6 {#alg-vi-s1-prop-6 .statement}

— Cho $(x_i)_{i \in A}, (y_\beta)_{\beta \in B}$ là hai họ các phần tử của một nhóm có thứ tự G, mỗi họ đều có một supremum. Khi đó họ $(x_\alpha + y_\beta)_{(\alpha, \beta) \in A \times B}$ có một supremum, và
$$
\sup_{(\alpha, \beta) \in A \times B} (x_\alpha + y_\beta) = \sup_{\alpha \in A} x_\alpha + \sup_{\beta \in B} y_\beta.
$$
Thật vậy, từ $x_\alpha + y_\beta \leq z$ với mọi $\alpha$ và $\beta$, ta suy ra $\sup(x_i) + \sup(y_\beta) \leq z$ với mọi $\beta$, và do đó $\sup(x_i) + \sup(y_\beta) \leq z$.

1 Khi A là vành các số nguyên (tương ứng, vành đa thức một biến với các hệ số trong một trường), các định nghĩa này trùng với các định nghĩa trong I, p. 112 (tương ứng, IV, p. 12, Def. 1).

### 9. Các nhóm có thứ tự dàn

Nhắc lại rằng một tập hợp có thứ tự trong đó mọi tập con hữu hạn khác rỗng đều có một supremum và một infimum được gọi là một dàn (E, III, p. 13). Rõ ràng tích của các nhóm có thứ tự dàn, và đặc biệt là tích của các nhóm có thứ tự toàn phần, là một nhóm có thứ tự dàn. Trái lại, một nhóm con của một nhóm có thứ tự dàn không nhất thiết có thứ tự dàn.

Như vậy, trong nhóm có thứ tự tích $Z \times Z$, « antidiagonal » (tập hợp các cặp $(n, n')$ sao cho $n + n' = 0$) có thứ tự rời rạc, và do đó không phải là một nhóm có thứ tự dàn. *Nhóm cộng của các đa thức một biến thực (VI, p. 1, ví dụ 2) là một nhóm lọc (vì cả $p(x)$ và $q(x)$ đều nhỏ hơn $(p(x))^2 + (q(x))^2 + 1$) mà ta có thể chứng minh là không có thứ tự dàn. \*

#### Mệnh đề 7 {#alg-vi-s1-prop-7 .statement}

— *Nếu x và y là hai phần tử của một nhóm có thứ tự G, và nếu một trong các phần tử $\inf(x, y)$, $\sup(x, y)$ tồn tại, thì phần tử kia cũng tồn tại, và $x + y = \inf(x, y) - \sup(x, y)$.

Thật vậy, theo các quan hệ (1) và (2) (VI, p. 9), ta có

$$
\sup(a - x, a - y) = a + \sup(-x, -y) = a - \inf(x, y),
$$

và chỉ cần lấy $a = x + y$.

#### Mệnh đề 7 {#alg-vi-s1-div-prop-7 .statement}

— *Nếu $a, b \in K^*$, và nếu d là một gcd của a và b, và m là một lcm của a và b, thì tích dm là một phần tử liên kết với ab.

#### Mệnh đề 8 {#alg-vi-s1-prop-8 .statement}

— *Cho P là tập hợp các phần tử dương của một nhóm có thứ tự $G$. Để G là một nhóm có thứ tự dàn, điều kiện cần và đủ là* $G = P - P$, *và thêm nữa P, được trang bị thứ tự cảm sinh, thỏa mãn một trong hai điều kiện sau:*

a) *Mỗi cặp phần tử của P có một cận trên đúng trong P.*
b) *Mỗi cặp phần tử của P có một cận dưới đúng trong P.*

*Tính cần thiết của các điều kiện này là hiển nhiên: thật vậy quan hệ* $G = P - P$ *nói rằng G là lọc (VI, p. 4, Prop. 4); mặt khác cận trên đúng và cận dưới đúng *trong* G của hai phần tử của P là dương, nên cũng là cận trên đúng và cận dưới đúng của chúng trong P.*

*Ngược lại, trước hết hãy chú ý rằng dưới giả thiết a) (tương ứng b)), mỗi cặp phần tử x, y của P có một cận trên đúng (tương ứng cận dưới đúng) *trong* G bằng với cận trên đúng a (tương ứng cận dưới đúng b) của nó *trong* P. Điều này là hiển nhiên đối với a, vì mọi cận trên của x và y đều dương; đối với b, lấy* $z \in G$ *là một cận dưới của x và y; khi đó tồn tại* $u \in P$ *sao cho* $z + u \in P$, *vì* $G = P - P$; *bây giờ* $\inf_P(x + u, y + u)$ *lớn hơn* $b + u$, *nên có dạng* $b + c + u$ *($c \geq 0$); vì* $b + c$ *nhỏ hơn x và nhỏ hơn y, ta có* $c = 0$; *do đó* $\inf_P(x + u, y + u) = b + u$, *điều này kéo theo* $z + u \leq b + u$, *vì vậy* $z \leq b$ *và dĩ nhiên b là cận dưới đúng của x và y trong G. Bây giờ nếu x và y là các phần tử tùy ý của G thì ta chuyển chúng về P: lấy* $v \in P$ *sao cho* $x + v$ *và* $y + v$ *là dương (VI, p. 5, Prop. 5); dưới giả thiết a) (tương ứng b)) tồn tại một cận trên đúng (tương ứng cận dưới đúng) của* $x + v$ *và* $y + v$ *trong* $P$, *và do đó cũng trong* $G$ *theo điều vừa thấy; bằng phép tịnh tiến, x và y có một cận trên đúng (tương ứng cận dưới đúng) trong* $G$; *sự tồn tại của một trong hai cái đó kéo theo cái kia, theo Prop. 7, và điều này cho thấy các điều kiện là đủ.*

### 10. Định lý phân tích

#### Định lý 1 (định lý phân tích) {#alg-vi-s1-thm-1 .statement}

— *Cho* $(x_i)_{1 \leq i \leq p}$ *và* $(y_j)_{1 \leq j \leq q}$ *là hai dãy hữu hạn các phần tử dương của một nhóm có thứ tự dàn* $G$ *sao cho* $$
\sum_{i=1}^p x_i = \sum_{j=1}^q y_j ;
$$ *khi đó tồn tại một dãy kép* $(z_{ij})_{1 \leq i \leq p, 1 \leq j \leq q}$ *gồm các phần tử dương của* $G$ *sao cho* $x_i = \sum_{j=1}^q z_{ij}$ *với mọi* $i$, *và* $y_j = \sum_{i=1}^p z_{ij}$ *với mọi* $j$.

1) Trước hết ta chứng minh định lý trong trường hợp $p = q = 2$. Cho $x, x', y, y'$ là các phần tử dương của $G$ sao cho $x + x' = y + y'$, và đặt $a = \sup(0, x - y')$. Vì
$$
x - y' = y - x'
$$
nhỏ hơn $x$ và nhỏ hơn $y$, suy ra $b = x - a$ và $c = y - a$ là dương, cũng như $d = a - (x - y')$. Ta cũng có
$$
x = a + b, \quad x' = c + d, \quad y = a + c \quad \text{and} \quad y' = b + d .
$$

2) Bây giờ ta chứng minh rằng nếu định lý đúng với $p < m$ và $q = n$ ($m > 2,\ n \geq 2$) thì nó đúng với $p = m$ và $q = n$. Theo giả thiết, ta có $x, + \sum_{i=1}^{m-1} x_i = \sum_{j=1}^n y_j$. Vì định lý đúng với $p = 2$ và $q = n$, tồn tại hai dãy hữu hạn $(z_j'), (z_j'')$ gồm $n$ phần tử dương sao cho $\sum_{i=1}^{m-1} x_i = \sum_{j=1}^n z_j'$, $x_m = \sum_{j=1}^n z_j''$, và $y_j = z_j' + z_j''$ với $1 \leq j \leq n$. Mặt khác, vì định lý đúng với $p = m - 1$ và $q = n$, tồn tại một dãy kép $(u_{ij})_{1 \leq i \leq m-1, 1 \leq j \leq n}$ sao cho $x_i = \sum_{j=1}^n u_{ij}$ với $1 \leq i \leq m - 1$, và $z_j' = \sum_{i=1}^{m-1} u_{ij}$ với $1 \leq j \leq n$. Đặt
$$
z_{ij} = u_{ij} \quad \text{với} \quad 1 \leq i \leq m - 1 , \quad \text{và} \quad z_{mj} = z_j'' \quad (1 \leq j \leq n) ,
$$
ta hiển nhiên thu được một dãy kép thỏa mãn các điều kiện của định lý.

3) Bằng cách đổi chỗ các $x_i$ và các $y_j$, ta thấy tương tự rằng, nếu định lý đúng với $p = m$ và $q < n$ ($m \geq 2,\ n > 2$), thì nó đúng với $p = m$ và $q = n$. Do đó, định lý được chứng minh bằng quy nạp kép, bắt đầu từ trường hợp $p = q = 2$, vì nó hiển nhiên đúng khi $p \leq 1$ hoặc $q \leq 1$.

#### Hệ quả {#alg-vi-s1-n10-cor-1 .statement}

— Cho $y, x_1, x_2, \ldots, x_n$ là $n + 1$ phần tử dương của $G$ sao cho $y \leq \sum_{i=1}^n x_i$; khi đó tồn tại $n$ phần tử dương $y_i$ ($1 \leq i \leq n$) sao cho $y_i \leq x_i$ và $y = \sum_{i=1}^n y_i$.

Chỉ cần áp dụng định lý 1 cho dãy $(x_i)$ và dãy gồm hai phần tử $y$ và $z = \left( \sum_{i=1}^n x_i \right) - y$.

### 11. Phần dương và phần âm

#### Định nghĩa 4 {#alg-vi-s1-def-4 .statement}

— Trong một nhóm $G$ có thứ tự dàn, phần dương (tương ứng phần âm, giá trị tuyệt đối) của một phần tử $x \in G$ là phần tử $\sup(x, 0)$ (tương ứng $\sup(-x, 0)$, $\sup(x, -x)$), được ký hiệu lần lượt là $x^+$ (tương ứng $x^-$, $|x|$).

Mặc dù mang tên như vậy, phần âm $x^-$ là một phần tử dương.

Rõ ràng $x^- = (-x)^+$ và $|-x| = |x|$. Ta cũng chú ý đến các công thức sau đây, công thức thứ nhất là một hệ quả ngay lập tức của các định nghĩa và tính bất biến của thứ tự đối với phép tịnh tiến, còn công thức thứ hai suy ra từ công thức thứ nhất theo Mệnh đề 7 của VI, p. 10:

$$
\begin{cases}
\sup(x, y) = x + (y - x)^+ \\
\inf(x, y) = y - (y - x)^+
\end{cases}
$$

#### Mệnh đề 9 {#alg-vi-s1-prop-9 .statement}

— a) Với mỗi phần tử $x$ của một nhóm $G$ có thứ tự dàn, ta có $x = x^+ - x^-$ và $\inf(x^+, x^-) = 0$.

b) Với mọi cách biểu diễn $x$ thành hiệu của hai phần tử dương, chẳng hạn $x = u - v$, ta có $u = x^+ + w$ và $v = x^- + w$ với $w = \inf(u, v)$. Đặc biệt nếu $\inf(u, v) = 0$ thì $u = x^+$ và $v = x^-$.

c) Quan hệ « $x \leq y$ » là tương đương với « $x^+ \leq y^+$ and $x^- \geq y^-$ ».

d) Ta có $|x| = x^+ + x^- \geq 0$.

e) Với mọi $x$ và $y$ trong $G$, ta có bất đẳng thức $|x + y| \leq |x| + |y|$, và nói chung hơn $\left| \sum_{i=1}^n x_i \right| \leq \sum_{i=1}^n |x_i|$ đối với mọi họ hữu hạn $(x_i)$ các phần tử của $G$.

f) Với mọi $x$ và $y$ trong $G$ ta có $||x| - |y|| \leq |x - y|$.

Chúng ta sẽ chứng minh đồng thời a) và b). Nếu $x = u - v$ với $u$ và $v$ dương, thì $u$ lớn hơn hoặc bằng $x$, nên $u \geq \sup(x, 0) = x^+$, và $w = u - x^+$ là dương. Mặt khác ta có

$$
x^+ - x = \sup(x, 0) - x = \sup(x - x, -x) = x
$$

do đó suy ra $x = x^+ - x^-$, và $v - x^- = w$. Nếu $z \leq x^-$ thì $z \leq x^+ - x$, và vì thế $x \leq x^+ - z$; nếu thêm nữa $z \leq x^+$, thì $x^z - z$ là dương, và vì thế x^i \leq x^+ - z \text{ theo định nghĩa của } x^i. \text{ Vậy ta có } z \leq 0, \text{ điều này kéo theo } \inf(x^+, x^-) = 0, \text{ do đó bằng phép tịnh tiến } \inf(u, v) = w.

c) Quan hệ $x \leq y$ kéo theo $\sup(y, 0) \geq x$ và $\sup(y, 0) \geq 0$, do đó $x^i \leq y^i$; tương tự, nếu $-y \leq -x$ thì suy ra $x^- \geq y^-$. Chiều đảo lại suy ra ngay lập tức từ $x = x^+ - x$ và $y = y^+ - y$.

d) Vì $x \leq x^+$ và $-x \leq x^-$, hiển nhiên
$$
|x| = \sup(x, -x) \leq x^+ + x
$$
Ngược lại, nếu $a \geq x$ và $a \geq -x$ thì từ c) suy ra $a^+ \geq x^+$, $a^+ \geq x^-$, $a^- \leq x^-$ và $a^- \leq x^+$; vì $a^-$ là dương và $\inf(x^i, x^-) = 0$, hai bất đẳng thức cuối suy ra $a^- = 0$ và $a = a^+$; khi đó hai bất đẳng thức đầu cho $a \geq \sup(x^+, x^-)$, và $\sup(x^+, x^-)$ bằng $x^+ + x^-$ theo a) và theo Mệnh đề 7 của VI, p. 10.

e) Vì $x$ và $y$ s $|x|$ và $y$, ta có $x + y \leq |x| + |y|$; vì $-x \leq |x|$ và $-y \leq |y|$, ta có $-x - y \leq |x| + |y|$; do đó bất đẳng thức thứ nhất. Bất đẳng thức thứ hai suy ra bằng quy nạp theo n.

f) Thay x và y lần lượt bằng y và x - y trong e), ta được
$$
|x| - |y| \leq |x - y|
$$
tương tự ta có $|y| - |x| \leq |y - x| = |x - y|$; do đó kết quả đã nêu.

#### Nhận xét {#alg-vi-s1-n11-rem-1 .statement}

Từ d) suy ra rằng $|x| = 0$ kéo theo $x = 0$ (vì $x^+$ và $x^-$ là dương); do đó $x \neq 0$ kéo theo $|x| > 0$.

#### Mệnh đề 9 {#alg-vi-s1-div-prop-9 .statement}

— Nếu nhóm $\mathcal{P}^*$ các iđêan phân thức chính của K có thứ tự dàn, thì mọi phần tử x của $K^*$ đều có thể viết dưới dạng $x = uv^{-1}$, trong đó u và v là các phần tử của A sao cho $1 = \gcd(u, v)$; với mọi biểu thức khác $x = u'{v'}^{-1}$ của x dưới dạng thương của hai phần tử của A, ta có $u' = uw$ và $v' = vw$, trong đó w là một ước chung lớn nhất của $u', v'$; đặc biệt nếu $1 = \gcd(u', v')$ thì u' và v' lần lượt là các phần tử liên kết của u và v.

Một biểu thức $uv^{-1}$ như vậy của một phần tử x của $K^*$ thường được gọi là một phân số tối giản.

### 12. Các phần tử nguyên tố cùng nhau

#### Định nghĩa 5 {#alg-vi-s1-def-5 .statement}

— Trong một nhóm có thứ tự, hai phần tử x và y được gọi là nguyên tố cùng nhau nếu $\inf(x, y) = 0$.

Trong một số trường hợp, tự nhiên là định nghĩa hai phần tử là nguyên tố cùng nhau nếu $\inf(|x|, |y|) = 0$ (cf. INT, II, § 1) hoặc đưa vào thuật ngữ tương ứng trong lý thuyết chia hết. Ở đây chúng ta sẽ không làm như vậy.

Hai phần tử nguyên tố cùng nhau nhất thiết là dương. Các phần dương và âm $x^+$ và $x^-$ của x là nguyên tố cùng nhau (VI, p. 12, Mệnh đề 9, a)). Các phần tử $x_i$ của một họ (x,)_, , được gọi là *nguyên tố cùng nhau theo tập* nếu $\inf_{i \in I} x_i = 0$; nếu các $x_i$ đều $\geq 0$ thì chỉ cần tồn tại một tập con hữu hạn J của I sao cho các phần tử tương ứng là nguyên tố cùng nhau theo tập. Các phần tử của một họ (x,) được gọi là *từng đôi một nguyên tố cùng nhau* nếu $\inf(x_i, x_j) = 0$ với mọi cặp $(\ell, \kappa)$ chỉ số phân biệt.

Các $x_i$ có thể nguyên tố cùng nhau theo tập mà không từng đôi một nguyên tố cùng nhau.

Nếu x và y nguyên tố cùng nhau, ta cũng nói rằng x nguyên tố cùng nhau với y, hoặc y nguyên tố cùng nhau với X

(DIV) Hai phần tử x và y của K được gọi là *nguyên tố cùng nhau* nếu các iđêan chính (x) và (y) khác không và nguyên tố cùng nhau trong $\mathcal{P}^*$; điều này tương đương với việc 1 là một ước chung lớn nhất của x và y, và kéo theo x và y *thuộc* A. Chẳng hạn tử số và mẫu số của một phân số tối giản là nguyên tố cùng nhau. Các khái niệm về các phần tử từng đôi một và theo tập nguyên tố cùng nhau được định nghĩa tương tự.

(DIV) Khi x và y nguyên tố cùng nhau, người ta thường nói chúng « nguyên tố cùng nhau »; thuận tiện là tránh thuật ngữ này, vì nó có thể gây nhầm lẫn với khái niệm số nguyên tố (I, p. 50, Định nghĩa 16).

#### Mệnh đề 10 {#alg-vi-s1-prop-10 .statement}

*Cho x, y và z là ba phần tử của một nhóm có thứ tự; để x – z và y – z nguyên tố cùng nhau, điều kiện cần và đủ là z = inf (x, y).*

Thật vậy, các hệ thức $z = \inf(x, y)$ và $0 = \inf(x - z, y - z)$ là tương đương.

**Mệnh đề 10 (DIV).** — *Cho a, b và c là ba phần tử của K với c $\neq 0$; để các thương $ac^{-1}$ và $bc^{-1}$ nguyên tố cùng nhau, điều kiện cần và đủ là c là một ước chung lớn nhất của a và b.*

#### Mệnh đề 11 {#alg-vi-s1-prop-11 .statement}

*Nếu $(x_i), (y_j)$ là hai họ hữu hạn các phần tử dương của một nhóm có thứ tự dàn, thì*

$$
\inf \left( \sum_i x_i, \sum_j y_j \right) \leq \sum_{i,j} \inf(x_i, y_j)
$$

Lập luận bằng quy nạp theo số phần tử trong các họ $(x_i)$ và $(y_j)$, chỉ cần chứng minh rằng, nếu x, y và z là các phần tử dương, thì

$$
\inf(x, y + z) \leq \inf(x, y) + \inf(x, z).
$$

Thật vậy, đặt $t = \inf(x, y + z)$; theo VI, p. 12, Cor., ta có thể viết $t = t_1 + t_2$ với $0 \leq t_1 \leq y$ và $0 \leq t_2 \leq z$; vì $t_1$ và $t_2$ là dương, ta cũng có $t_1 \leq x$ và $t_2 \leq x$, do đó $t_1 \leq \inf(x, y)$ và $t_2 \leq \inf(x, z)$.

#### Hệ quả 1 {#alg-vi-s1-prop-11-cor-1 .statement}

*Nếu x và y là hai phần tử nguyên tố cùng nhau, và z là một phần tử dương, của một nhóm có thứ tự dàn, thì $\inf(x, z) = \inf(x, y + z)$.*

Thật vậy $\inf(x, y + z) \leq \inf(x, z)$ theo Prop. 11, và $\inf(x, z) \leq \inf(x, y + z)$ vì $y \geq 0$, do đó suy ra hệ quả.

#### Hệ quả 2 {#alg-vi-s1-prop-11-cor-2 .statement}

— Trong một nhóm có thứ tự dàn, nếu x và y nguyên tố cùng nhau và nếu z $\geq 0$ và $x \leq y + z$, thì $x \leq z$.

#### Hệ quả 3 {#alg-vi-s1-prop-11-cor-3 .statement}

— Trong một nhóm có thứ tự dàn, nếu x nguyên tố cùng nhau với y và với z, thì nó cũng nguyên tố cùng nhau với $y + z$.

#### Hệ quả 4 {#alg-vi-s1-prop-11-cor-4 .statement}

— Nếu $(x_i)_{1 \leq i \leq n}$ và $(y_j)_{1 \leq j \leq m}$ là hai họ hữu hạn các phần tử của một nhóm có thứ tự dàn G, sao cho mỗi $x_i$ nguyên tố cùng nhau với mỗi $y_j$, thì $x_1 + \ldots + x_n$ nguyên tố cùng nhau với $y_1 + \ldots + y_m$.
Điều này suy ra từ Cor. 3 bằng quy nạp theo m và n.

#### Hệ quả 5 {#alg-vi-s1-prop-11-cor-5 .statement}

— Với mọi số nguyên $n \geq 0$ ta có $(nx)^+ = nx^+$ và $(nx)^- = nx^-$; với mọi $n \in \mathbf{Z}$ ta có $|nx| = |n| \cdot |x|$.
Thật vậy $nx = nx^+ - nx^-$; vì $x^+$ và x nguyên tố cùng nhau, nên $nx^+$ và $nx^-$ cũng nguyên tố cùng nhau nếu $n \geq 0$ (Cor. 4); mệnh đề thứ nhất suy ra theo Prop. 9 b) của VI, p. 12. Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất theo Prop. 9 d) trong trường hợp $n \geq 0$; trường hợp $n < 0$ suy ra từ đó như là hệ quả của quan hệ $|-x| = |x|$.

#### Mệnh đề 11 {#alg-vi-s1-div-prop-11 .statement}

— Giả sử tập hợp $\mathcal{P}^*$ là một dàn, và cho $(a_i)$, $(b_j)$ là hai họ hữu hạn các phần tử của A. Khi đó mọi ước chung lớn nhất của $\prod_i a_i$ và $\prod_j b_j$ đều chia tích $\prod_{i,j} \gcd(a_i, b_j)$.

#### Hệ quả 1 {#alg-vi-s1-div-prop-11-cor-1 .statement}

— Nếu a, b, c là ba phần tử của A sao cho a nguyên tố cùng nhau với b, thì mọi ước chung lớn nhất của a và c cũng là một ước chung lớn nhất của a và bc.

#### Hệ quả 2 (Bổ đề Euclid) {#alg-vi-s1-div-prop-11-cor-2 .statement}

— Cho a, b, c là ba phần tử của A. Nếu a nguyên tố cùng nhau với b và chia bc, thì nó chia c.

#### Hệ quả 3 {#alg-vi-s1-div-prop-11-cor-3 .statement}

— Nếu x nguyên tố cùng nhau với y và với z, thì nó nguyên tố cùng nhau với yz.

#### Hệ quả 4 {#alg-vi-s1-div-prop-11-cor-4 .statement}

— Nếu $(x_i)$ và $(y_j)$ là hai họ hữu hạn các phần tử của A sao cho mỗi $x_i$ nguyên tố cùng nhau với mỗi $y_j$, thì tích của các $x_i$ nguyên tố cùng nhau với tích của các $y_j$.

#### Hệ quả 5 {#alg-vi-s1-div-prop-11-cor-5 .statement}

— Nếu d là một gcd của x và y, thì $d^n$ là một gcd của $x^n$ và $y^n$ với mỗi số nguyên dương n.
Thật vậy $xd^1$ và $yd^1$ nguyên tố cùng nhau (Mệnh đề 10 (DIV)), và do đó $x^n d^{-n}$ và $y^n d^{-n}$ cũng vậy (Hệ quả 4).

#### Mệnh đề 12 {#alg-vi-s1-prop-12 .statement}

— Cho $x_i$ ($1 \leq i \leq n$) là n phần tử từng đôi một nguyên tố cùng nhau trong một nhóm có thứ tự dàn. Khi đó
$$
\sup(x_1, \ldots, x_n) = x_1 + \cdots + x_n .
$$

Điều này suy ra từ công thức $u + v = \sup(u, v) + \inf(u, v)$ (VI, p. 10, Mệnh đề 7) bằng quy nạp theo $n$, dùng sự kiện rằng $x_i$ nguyên tố cùng nhau với $x_1 + \ldots + x_{i-1}$ với $2 \leq i \leq n$ (Hệ quả 4 của Mệnh đề 11).

#### Nhận xét {#alg-vi-s1-n12-rem-1 .statement}

Mệnh đề 7 của VI, p. 10 cũng cho thấy rằng điều kiện cần và đủ để $x$ và $y$ nguyên tố cùng nhau là $x + y = \sup(x, y)$.

#### Mệnh đề 12 {#alg-vi-s1-div-prop-12 .statement}

— *Cho $a_i$ là một số hữu hạn $n$ các phần tử từng đôi một nguyên tố cùng nhau của $\mathbf{A}$; khi đó tích $a_1 \ldots a_n$ là một lcm của $a_1, \ldots, a_n$.*

#### Mệnh đề 13 {#alg-vi-s1-prop-13 .statement}

— *Trong một nhóm có thứ tự dàn $G$, cho $(x_\alpha)$ là một họ có cận dưới đúng (tương ứng cận trên đúng), và cho $z$ là một phần tử tùy ý của $G$; khi đó họ $(\sup(z, x_\alpha))$ (tương ứng $(\inf(z, x_\alpha))$) có một cận dưới đúng (tương ứng cận trên đúng) và*

$$
\begin{align*}
\inf_{\alpha} (\sup(z, x_\alpha)) &= \sup \left( z, \inf_{\alpha} x_\alpha \right) \\
\sup_{\alpha} (\inf(z, x_\alpha)) &= \inf \left( z, \sup_{\alpha} x_\alpha \right)
\end{align*}
$$

*tương ứng.*

Giả sử rằng họ $(x_\alpha)$ có một cận dưới đúng $y$. Ta sẽ chứng minh rằng $\sup(z, y)$ là một cận dưới đúng của họ $(\sup(z, x_\alpha))$.

Thật vậy $\sup(z, x_\alpha) = z + (x_\alpha - z)^+$ và bằng cách tịnh tiến ta có thể rút gọn về trường hợp $z = 0$, nghĩa là ta phải chứng minh rằng $(x_\alpha^+)$ có một cận dưới đúng bằng $y^+$. Vì $y \leq x_\alpha$ nên ta có $y^+ \leq x_\alpha^+$ với mọi $\alpha$ (VI, p. 12, Mệnh đề 9, c)). Ngược lại, nếu $a \leq x_\alpha^+$ với mọi $a$, thì suy ra $a \leq x_\alpha + x_\alpha^-$ (Mệnh đề 9, a)); bây giờ $y^- \geq x_\alpha^-$ vì $y \leq x_\alpha$; do đó $a \leq x_\alpha + y^-$ với mọi $a$, nghĩa là $a \leq y + y^- = y^+$.

Công thức kia suy ra bằng cách chuyển sang quan hệ thứ tự đối.

#### Hệ quả {#alg-vi-s1-n12-cor-1 .statement}

— *Nếu một phần tử $z$ của một nhóm có thứ tự dàn $G$ nguyên tố cùng nhau với mỗi phần tử $x_\alpha$ của một họ có cận dưới đúng $y$, thì $z$ nguyên tố cùng nhau với $y$.*

Đây là một hệ quả ngay lập tức của công thức thứ hai (4).

#### Nhận xét {#alg-vi-s1-n12-rem-2 .statement}

Áp dụng các công thức của Mệnh đề 13 cho một họ gồm hai phần tử $(x, y)$, ta thu được các công thức sau, diễn tả sự kiện rằng mỗi một trong các luật hợp thành sup, inf trong một nhóm có thứ tự dàn đều *phân phối* đối với luật kia:

$$
\begin{align*}
\sup(z, \inf(x, y)) &= \inf(\sup(z, x), \sup(z, y)) \\
\inf(z, \sup(x, y)) &= \sup(\inf(z, x), \inf(z, y)) .
\end{align*}
$$

Tính chất phân phối này là đặc thù của *nhóm* có thứ tự dàn, và không mở rộng đến các dàn tùy ý, hay ngay cả đến các monoid có thứ tự dàn (xem VI, p. 33, Bài tập 24).

### 13. Phần tử bất khả quy

#### Định nghĩa 6 {#alg-vi-s1-def-6 .statement}

— *Một phần tử x của một nhóm có thứ tự G được gọi là bất khả quy nếu nó là một phần tử cực tiểu trong tập hợp các phần tử dương ngặt của G.*

Cho x là một phần tử bất khả quy của nhóm có thứ tự G; nếu y là một phần tử dương của G thì phần tử inf(x, y), nếu nó tồn tại, chỉ có thể bằng x hoặc bằng 0. Do đó trong một nhóm có thứ tự dàn G, mọi y dương hoặc lớn hơn hoặc nguyên tố cùng nhau với phần tử bất khả quy x; đặc biệt, hai phần tử bất khả quy phân biệt nguyên tố cùng nhau.

(DIV) Một phần tử p của A được gọi là *bất khả quy* nếu iđêan (p) là một phần tử bất khả quy của nhóm có thứ tự $\mathcal{P}^*$; điều này có nghĩa là p không phải là không cũng không phải là khả nghịch, và mọi phần tử của $A$ chia hết p đều liên kết либо với p hoặc với 1. Nếu $\mathcal{P}^*$ là một dàn có thứ tự, thì mọi $a \in A$ hoặc nguyên tố cùng nhau với p hoặc là một bội của p.

*Ví dụ (DIV). —* 1) Một số nguyên $p > 0$ là bất khả quy trong $\mathbf{Z}$ khi và chỉ khi nó là *nguyên tố* (I, p. 50).

2) Một đa thức theo một ẩn trên một trường K là bất khả quy khi và chỉ khi nó là bất khả quy theo nghĩa thông thường (IV, p. 13).

#### Mệnh đề 14 {#alg-vi-s1-prop-14 .statement}

— *Để một phần tử $x > 0$ của một nhóm có thứ tự G là bất khả quy, điều kiện đủ là nó thỏa mãn tính chất sau đây:*

(P) *Các quan hệ $x \leq y + z,\ y \geq 0,\ z \geq 0$ suy ra $x \leq y$ hoặc $x \leq z$.*
*Điều kiện này là cần thiết khi G là một dàn có thứ tự.*

Nếu G là một dàn có thứ tự và x là bất khả quy, ta vừa thấy rằng y hoặc lớn hơn x hoặc nguyên tố cùng nhau với x; trong trường hợp sau, Hệ quả 2 của VI, p. 15 cho thấy rằng z lớn hơn x. Ngược lại, giả sử điều kiện được thỏa mãn: nếu $0 \leq y \leq x$ thì suy ra, bằng cách đặt $x = y + z\ (z \geq 0)$, rằng hoặc $x \leq y$ hoặc $x \leq z$; trong trường hợp thứ nhất ta có $x = y$; trong trường hợp thứ hai ta có $x \leq x - y$, nên $y \leq 0$ và do đó $y = 0$; điều này cho thấy x quả thật là bất khả quy.

#### Mệnh đề 14 {#alg-vi-s1-div-prop-14 .statement}

— *Để một phần tử khác không p của A là bất khả quy, điều kiện đủ là nó không là một phần tử khả nghịch, và nó không thể chia hết một tích của hai phần tử của A mà không chia hết một trong hai phần tử ấy. Điều kiện này là cần thiết nếu $\mathcal{P}^*$ là một dàn có thứ tự.*

#### Nhận xét {#alg-vi-s1-n13-rem-1 .statement}

Mệnh đề 14 (DIV) cũng có thể được phát biểu như sau: nếu p là một phần tử khác không của A sao cho iđêan (p) là *nguyên tố* (I, p. 117, Định nghĩa 3) thì p là bất khả quy; ngược lại, nếu $\mathcal{P}^*$ là một dàn có thứ tự và p là bất khả quy thì iđêan (p) là nguyên tố.

#### Mệnh đề 15 {#alg-vi-s1-prop-15 .statement}

— *Trong một nhóm có thứ tự G, cho $(p_i)_{i \in I}$ là một họ các phần tử dương phân biệt từng đôi một của G thỏa mãn điều kiện (P) (và do đó là bất khả quy). Khi đó ánh xạ*

$$
(n_i)_{i \in I} \mapsto \sum_{i \in I} n_i p_i
$$

*là một đẳng cấu của nhóm có thứ tự $\mathbf{Z}^{(1)}$, tổng trực tiếp của các nhóm có thứ tự $Z$ (VI, p. 7), lên nhóm con có thứ tự của $G$ được sinh bởi các $p_\iota$.*

Chỉ cần chứng minh rằng quan hệ $\sum_{\iota \in I} n_\iota p_\iota \geq 0$ tương đương với $n_\iota \geq 0$ với mọi $\iota$, vì đặc biệt quan hệ $\sum_{\iota \in I} n_\iota p_\iota = 0$ sẽ suy ra $n_\iota = 0$ với mọi $\iota$, do đó điều này sẽ cho thấy họ $(p_\iota)$ độc lập tuyến tính. Bây giờ gọi $I'$ (tương ứng, $I''$) là tập con hữu hạn của $I$ gồm những $\iota$ sao cho $n_\iota > 0$ (tương ứng, $n_\iota < 0$) ; ta có

$$
\sum_{\iota \in I'} n_\iota p_\iota \geq \sum_{\iota \in I''} (-n_\iota)p_\iota .
$$

Đặc biệt, với $\lambda \in I''$, điều này suy ra rằng $p_\lambda \leq \sum_{\iota \in I'} n_\iota p_\iota$, và từ tính chất (P) suy ra bằng quy nạp rằng phải có $p_\lambda \leq p_\iota$ với một $\iota \in I'$ nào đó; vì $p_\iota$ là bất khả quy, điều này sẽ kéo theo $p_\lambda = p_\iota$, điều vô lý. Vậy $I'$ là rỗng, điều này chứng minh mệnh đề.

#### Định lý 2 {#alg-vi-s1-thm-2 .statement}

— Cho $G$ là một nhóm lọc. Khi đó các tính chất sau là tương đương:
a) $G$ đẳng cấu với một nhóm có thứ tự dạng $\mathbf{Z}^{(1)}$.
b) $G$ là một dàn có thứ tự và thỏa mãn điều kiện sau:
(MIN) Mọi tập hợp khác rỗng các phần tử dương của $G$ đều có một phần tử cực tiểu.
c) $G$ thỏa mãn điều kiện (MIN) và mọi phần tử bất khả quy của $G$ đều có tính chất (P).
d) $G$ được sinh bởi các phần tử bất khả quy của nó, và mọi phần tử bất khả quy của $G$ đều có tính chất (P).

Trước hết ta hãy chỉ ra rằng a) suy ra b). Nhóm $\mathbf{Z}^{(1)}$ được sắp thứ tự theo dàn, vì là tổng trực tiếp của các nhóm được sắp thứ tự toàn phần. Mặt khác, cho $E$ là một tập hợp khác rỗng các phần tử dương của $\mathbf{Z}^{(1)}$ và cho $x = \sum n_\iota e_\iota$ là một phần tử của $E$ (trong đó $(e_\iota)$ ký hiệu cơ sở tự nhiên của $\mathbf{Z}^{(1)}$) ; có một số hữu hạn $\prod (n_\iota + 1)$ các phần tử $y$ của $\mathbf{Z}^{(1)}$ sao cho $0 \leq y \leq x$, do đó tập hợp $F$ các phần tử của $E$ nhỏ hơn hoặc bằng $x$ a fortiori là hữu hạn ; vì nó khác rỗng, nó chứa một phần tử cực tiểu (Lý thuyết tập hợp, III, p. 170, Hệ quả 2), rõ ràng là một phần tử cực tiểu của $E$.

Rõ ràng b) suy ra c), theo Mệnh đề 14. Ta hãy chỉ ra rằng c) suy ra d). Vì $G$ được lọc, chỉ cần kiểm tra (VI, p. 4, Mệnh đề 4) rằng tập hợp $F$ các phần tử dương của $G$ là các tổng của những phần tử bất khả quy thì bằng $G_+ - \{0\}$. Nếu điều này không đúng, thì từ (MIN) suy ra rằng phần bù của $F$ trong $G_+ - \{0\}$ sẽ có một phần tử cực tiểu $a$; theo định nghĩa, $a$ không bất khả quy, nên là tổng của hai phần tử dương ngặt $x$ và $y$; vì $x < a$ và $y < a$, các phần tử này thuộc $F$, và do đó là các tổng của những phần tử bất khả quy, suy ra $a$ cũng vậy, mâu thuẫn. Cuối cùng, d) suy ra a) theo Mệnh đề 15.

Ta sẽ áp dụng Định lý 2 cho lý thuyết tính chia hết trong các miền iđêan chính (VII, p. 4) và trong các miền phân tích duy nhất (AC, VII, § 3), cũng như cho việc nghiên cứu các iđêan trong một vành Dedekind (AC, VII, § 2).

### Bài tập {#alg-vi-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
