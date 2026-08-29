---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 10
section_title: Extensions of a valuation to a transcendental extension
lang: vi
source: ac-i-vii
book_pages: 434-440, 471-473
pdf_pages: 0452-0458, 0489-0491
extraction: ocr
subsections:
    - "no": 1
      title: THE CASE OF A MONOGENOUS TRANSCENDENTAL EXTENSION
      page: 434
      pdf_page: 452
    - "no": 2
      title: THE RATIONAL RANK OF A COMMUTATIVE GROUP
      page: 437
      pdf_page: 455
    - "no": 3
      title: THE CASE OF ANY TRANSCENDENTAL EXTENSION
      page: 438
      pdf_page: 456
statements: 14
exercises: 2
content_sha256: 0feda9fa8613a79d8478c32d496a3932f293f8b29c609e229eab54dc93a3d9a8
translated_from: content/en/ac/VI/10_s10_extensions_of_a_valuation_to_a.md
source_content_sha256: 34f40a243b26113b5ca170f44a53946190e03c0c9c5132625229fb3ca220d4f2
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-aaf67f5f
glossary_version: 34
glossary_terms_sha256: a20e9d1b2a614129d8dfb4401e81b9ddf27f34b931bdbde3ee072d3139690f5d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 10. CÁC MỞ RỘNG CỦA MỘT ĐỊNH GIÁ LÊN MỘT MỞ RỘNG SIÊU VIỆT

### 1. TRƯỜNG HỢP CỦA MỘT MỞ RỘNG SIÊU VIỆT ĐƠN SINH

#### Bổ đề 1 {#ac-vi-s10-lem-1 .statement}

Cho $K$ là *một trường*, $v$ là một định giá trên $K$, $\Gamma$ là nhóm cấp *của nó*, $\Gamma'$ là một nhóm được sắp thứ tự toàn phần chứa $\Gamma$ và $\xi$ là *một phần tử của* $\Gamma'$. Tồn tại *một* định giá duy nhất w *trên* $K(X)$ *sao cho*, *với* $P = \sum_j a_j X^j$ ($a_j \in K$), $w(P) = \inf_j (v(a_j) + j\xi)$.

Theo Mệnh đề 4 của § 3, no. 2, chỉ cần chứng minh rằng công thức

$$
w\left( \sum_j a_j X^j \right) = \inf_j (v(a_j) + j\xi)
$$

xác định một định giá trên vành $K[X]$. Vì

$$
v(a_j + b_j) + j\xi \geq \inf(v(a_j), v(b_j)) + j\xi = \inf(v(a_j) + j\xi, v(b_j) + j\xi),
$$

nên suy ra rằng

$$
w(P + Q) \geq \inf(w(P), w(Q))
$$

với $P, Q$ thuộc $K[X]$, và có đẳng thức nếu $w(P) \neq w(Q)$. Ta chứng minh rằng

$$
w(PQ) = w(P) + w(Q)
$$

với $P = \sum a_j X^j$ và $Q = \sum b_j X^j$. Gọi $i$ (tương ứng $k$) là số nguyên $j$ nhỏ nhất sao cho $v(a_j) + j\xi$ (tương ứng $v(b_j) + j\xi$) đạt giá trị nhỏ nhất của nó; gọi $a$ (tương ứng $\beta$) là giá trị nhỏ nhất này. Với $j, j'$ trong $\mathbf{N}$,

$$
w(a_j b_{j'} X^{j+j'}) = v(a_j) + j\xi + v(b_{j'}) + j'\xi \geq a + \beta,
$$

do đó $w(PQ) \geq a + \beta$ theo (2). Bây giờ xét số hạng $c X^{i+k}$ bậc $i + k$ trong $PQ$; khi đó $c = \sum_{n \in \mathbf{Z}} a_{i+n} b_{k-n}$; theo cách chọn $i$ và $k$, phần tử

$$
w(a_{i+n} b_{k-n} X^{i+k}) = v(a_{i+n}) + (i+n)\xi + v(b_{k-n}) + (k-n)\xi
$$

nhận giá trị nhỏ nhất $a + \beta$ một lần và chỉ một lần khi $n = 0$; vì thế $w(c X^{i+k}) = a + \beta$, do đó, theo (1),

$$
w(PQ) = \alpha + \beta = w(P) + w(Q).
$$

#### Mệnh đề 1 {#ac-vi-s10-prop-1 .statement}

Cho $K$ là *một trường*, $v$ *một định giá trên* $K$, $\Gamma$ *nhóm có thứ tự của nó*, $\Gamma'$ *một nhóm được sắp thứ tự toàn phần chứa* $\Gamma$ *và* $\xi$ *một phần tử của* $\Gamma'$ *sao cho các hệ thức* $n\xi \in \Gamma, n \in \mathbf{Z}$ *suy ra* $n = 0$. Khi đó tồn tại *một* định giá duy nhất w *trên* $K(X)$ *nhận giá trị trong* $\Gamma'$ *và mở rộng* $v$ *sao cho* $w(X) = \xi$. *Trường thặng dư của* w *bằng trường thặng dư của* $v$ *và nhóm có thứ tự của nó là nhóm con* $\Gamma + \mathbf{Z}\xi$ *của* $\Gamma'$.

Trước hết ta chứng minh tính duy nhất của w. Cho $P = \sum_j a_j X^j$ là một phần tử của $K[X]$. Khi đó $w(a_j X^j) = v(a_j) + j\xi$, điều này cho thấy các đơn thức $a_j X^j$ sao cho $a_j \neq 0$ có các giá trị đôi một phân biệt đối với w. Suy ra $w(P) = \inf_j (v(a_j) + j\xi)$, điều này chứng tỏ đồng thời tính duy nhất của w trên $K[X]$ (và do đó cả trên $K(X)$) và việc nhóm có thứ tự của w là $\Gamma + \mathbf{Z}\xi$. Hơn nữa, ta thấy rằng, nếu $P \neq 0$, ta có thể viết $P = a X^n (1 + u)$, trong đó $a \in K^*, n \in \mathbf{N}, u \in K(X)$ và $w(u) > 0$; vì thế mọi phần tử $R \neq 0$ của $K(X)$ đều có thể viết dưới dạng
$$
R = b X^n (1 + u'),
$$
trong đó $b \in K^*, n \in \mathbf{Z}, u' \in K(X)$ và $w(u') > 0$; khi đó $w(R) = v(b) + n \xi$, do đó $w(R) = 0$ khi và chỉ khi $v(b) = 0$ và $n = 0$; vì vậy, khi $w(R) = 0$, $R$ và $b$ đồng dư theo iđêan của $w$, điều này cho thấy trường thặng dư của $w$ bằng trường thặng dư của $v$.

Cuối cùng sự tồn tại của $w$ suy ra từ Bổ đề 1.

#### Mệnh đề 2 {#ac-vi-s10-prop-2 .statement}

*Cho $K$ là một trường, $v$ là một định giá trên $K$, $\Gamma$ là nhóm cấp của nó và $k$ là trường thặng dư của nó. Tồn tại một định giá duy nhất $w$ trên $K(X)$ mở rộng $v$ sao cho $w(X) = 0$ và ảnh $t$ của $X$ trong trường thặng dư $k'$ của $w$ là siêu việt trên $k$. Nhóm cấp của $w$ bằng nhóm cấp của $v$ và trường thặng dư của nó là $k(t)$.*

Để chứng minh tính duy nhất của $w$, với chúng ta chỉ cần chứng minh rằng, nếu $P = \sum_j a_j X^j$ là một phần tử khác không của $K[X]$, thì
$$
w(P) = \inf_j (v(a_j)).
$$
Ta có thể chia $P$ cho một phần tử của $K^*$ và giả sử rằng $v(a_j) \geq 0$ với mọi $j$ và một trong các $v(a_j)$ bằng không. Vì $w(X) = 0$, khi đó $P$ thuộc vành của $w$; viết $\bar{a}_j$ là ảnh chính tắc của $a_j$ trong $k$, ảnh chính tắc của $P$ trong trường thặng dư $k'$ là $\sum_j \bar{a}_j t^j$; vì $t$ là siêu việt trên $k$ và một trong các $\bar{a}_j$ khác không, ảnh này khác không, do đó
$$
w(P) = 0 = \inf_j (v(a_j)).
$$
Bây giờ ta chứng minh sự tồn tại của $w$. Công thức $w(P) = \inf_j (v(a_j))$ (với $P = \sum_j a_j X^j$) xác định một định giá $w$ trên $K(X)$, nhờ Bổ đề 1, và $w$ hiển nhiên có cùng nhóm giá trị như $v$. Khi đó $w(X) = 0$. Ta chứng minh rằng ảnh chính tắc $t$ của $X$ trong trường thặng dư $k'$ của $w$ là siêu việt trên $k$: nếu $\sum_j \bar{a}_j t^j = 0$, trong đó $\bar{a}_j \in k$ với mọi $j$, thì, ký hiệu bởi $a_j$ một đại diện của $\bar{a}_j$ trong vành của $v$, ta có $w \left( \sum_j a_j X^j \right) > 0$; do đó $v(a_j) > 0$ với mọi $j$, suy ra $\bar{a}_j = 0$ với mọi $j$. Cuối cùng ta chứng minh rằng $k' = k(t)$: mọi phần tử $R$ của $K(X)$ có thể viết dưới dạng $R = c \left( \sum_j a_j X^j \right) / \left( \sum_j b_j X^j \right)$, trong đó $c, a_j, b_j$ thuộc $K$, $v(a_j) \geq 0$ và $v(b_j) \geq 0$ với mọi $j$, một trong các $v(a_j)$ và một trong các $v(b_j)$ bằng không; khi đó $w(R) \geq 0$ khi và chỉ khi $v(c) \geq 0$; ký hiệu bởi $f$ đồng cấu chính tắc của vành của $w$ lên $k'$,
$$
f(R) = f(c) \left( \sum_j f(a_j) t^j \right) / \left( \sum_j f(b_j) t^j \right),
$$

điều đó chứng minh mệnh đề của chúng ta.

#### Nhận xét {#ac-vi-s10-n1-rem-1 .statement}

Không nên nghĩ rằng hai kiểu mở rộng của v lên K(X) mà ta vừa gặp là những kiểu duy nhất; có thể tồn tại một kiểu mở rộng thứ ba, trong đó $\Gamma'/\Gamma$ là một nhóm xoắn và $k'$ là một mở rộng đại số (không nhất thiết hữu hạn) của $k$. Kiểu thứ ba này không nhất thiết thu được bằng thủ tục mô tả trong Bổ đề 1 (x. § 3, Bài tập 1).

### 2. HẠNG HỮU TỈ CỦA MỘT NHÓM GIAO HOÁN

#### Định nghĩa 1 {#ac-vi-s10-def-1 .statement}

*Hạng hữu tỉ của một nhóm giao hoán G là chiều của không gian vectơ trên Q* $G \otimes_{\mathbf{Z}} \mathbf{Q}$.

Chiều này cũng có thể được định nghĩa là cận trên bé nhất (hữu hạn hoặc vô hạn) của các lực lượng $r$ sao cho tồn tại $r$ phần tử của G độc lập tuyến tính trên $\mathbf{Z}$ (*Đại số*, Chương II, § 7, no. 10, Mệnh đề 26). Hạng hữu tỉ của G là *không* khi và chỉ khi G là một nhóm xoắn. Đối với một nhóm con của nhóm cộng $\mathbf{R}^n$, khái niệm hạng hữu tỉ trùng với khái niệm được định nghĩa trong *Tôpô đại cương*, Chương VII, § 1.

Trong phần còn lại của đoạn này, ta sẽ ký hiệu hạng hữu tỉ của nhóm giao hoán G bởi $r(G)$. Nếu $G'$ là một nhóm con của G, thì (vì $\mathbf{Q}$ là một $\mathbf{Z}$-môđun phẳng) ta có đẳng thức cộng tính

$$
r(G) = r(G') + r(G/G').
$$

#### Mệnh đề 3 {#ac-vi-s10-prop-3 .statement}

*Cho G là một nhóm giao hoán được sắp thứ tự toàn phần và H là một nhóm con của G. Nếu $h(G)$ và $h(H)$ ký hiệu các chiều cao của G và H* ($§ 4$, no. 4), *thì bất đẳng thức*

$$
h(G) \leq h(H) + r(G/H)
$$

*đúng*.

Thật vậy, cho $G_0 \subset G_1 \subset \ldots \subset G_n$ là một dãy tăng ngặt các nhóm con cô lập của G. Cần thiết lập bất đẳng thức

$$
n \leq h(H) + r(G/H).
$$

Điều đó hiển nhiên với $n = 0$. Giả sử $n \geq 1$ và lập luận bằng quy nạp theo $n$. Áp dụng giả thiết quy nạp cho nhóm $G_{n-1}$ và nhóm con $H \cap G_{n-1}$ của nó, ta được

$$
n - 1 \leq h(H \cap G_{n-1}) + r(G_{n-1}/(H \cap G_{n-1})).
$$

Khi đó ta phân biệt hai trường hợp:

(a) $H \cap G_{n-1} = H$, nói cách khác $H \subset G_{n-1}$. Bất đẳng thức (7) có thể viết thành

$$
n \leq h(H) + r(G_{n-1}/H) + 1.
$$

Bây giờ $G/G_{n-1}$ là một nhóm có thứ tự toàn phần không quy về 0; do đó nó không phải là một nhóm xoắn và $r(G/G_{n-1}) \geq 1$. Do đó theo (4), $r(G/H) \geq r(G_{n-1}/H) + 1$. Thay vào (8), chắc chắn ta thu được bất đẳng thức cần chứng minh (6).

(b) $H \cap G_{n-1} \neq H$. Vì $H \cap G_{n-1}$ là một nhóm con cô lập của $H$, ta kết luận rằng $h(H) > h(H \cap G_{n-1}) + 1$. Mặt khác, hiển nhiên $r(G/H) \geq r(G_{n-1}/(H \cap G_{n-1}))$. Thay vào (7), ta lại thu được (6).

#### Hệ quả {#ac-vi-s10-n2-cor-1 .statement}

*Với mọi nhóm giao hoán được sắp thứ tự toàn phần G, $h(G) \leq r(G)$.* Ta đặt $H = (0)$ trong Mệnh đề 3.

#### Mệnh đề 4 {#ac-vi-s10-prop-4 .statement}

*Cho G là một nhóm giao hoán được sắp thứ tự toàn phần. Giả sử rằng G sinh hữu hạn và $h(G) = r(G)$. Khi đó G đẳng cấu với $\mathbf{Z}^{r(G)}$ được sắp theo thứ tự từ điển.*

Hãy viết $r = r(G) = h(G)$. Nếu $r = 0$, thì $G = (0)$. Nếu $r = 1$, cấu trúc của các nhóm giao hoán sinh hữu hạn cho thấy tồn tại một đẳng cấu $j$ từ G lên Z (*Đại số*, Chương VII, § 4, no. 6, Định lý 3). Bây giờ Z chỉ có hai thứ tự toàn phần tương thích với cấu trúc nhóm của nó, đó là thứ tự thông thường và thứ tự đối của nó. Vì thế $j$ hoặc $-j$ là một đẳng cấu của nhóm có thứ tự G lên Z với thứ tự thông thường.

Bây giờ giả sử rằng $r \geq 2$ và lập luận bằng quy nạp theo $r$. Cho H là một nhóm con cô lập của G có chiều cao $r - 1$. Khi đó $r(H) + r(G/H) = r$ (công thức (4)), $r(H) \geq h(H) = r - 1$ và $r(G/H) \geq h(G/H) = 1$ (Hệ quả của Mệnh đề 3), do đó $r(H) = r - 1$ và $r(G/H) = 1$. Giả thiết quy nạp cho thấy H đẳng cấu với $\mathbf{Z}^{r-1}$ được sắp theo thứ tự từ điển và trường hợp $r = 1$ cho thấy $G/H$ đẳng cấu với Z. Vì Z là một Z-môđun tự do, H là một *nhân tử trực tiếp* của G (*Đại số*, Chương 11, § 1, no. 11, Mệnh đề 21). Bổ đề sau đây khi đó cho thấy G đẳng cấu (không một cách chính tắc) với tích từ điển $H \times (G/H)$, điều này hoàn tất chứng minh.

#### Bổ đề 2 {#ac-vi-s10-lem-2 .statement}

*Cho H là một nhóm con cô lập của một nhóm giao hoán được sắp thứ tự toàn phần G. Nếu H là một nhân tử trực tiếp của G, thì nhóm có thứ tự G đẳng cấu với nhóm $(G/H) \times H$ được sắp theo thứ tự từ điển.*

Cho $j$ là một đẳng cấu của $(G/H) \times H$ lên G sao cho $j(0, x) = x$ với mọi $x \in H$ và $j(y, x)$ thuộc lớp kề của H. Vì $(G/H) \times H$ được sắp thứ tự toàn phần, điều này tương đương với việc chứng minh rằng $j$ là *tăng* (*Set Theory*, Chương III, § 1, no. 12, Mệnh đề 11). Cho $(y, x)$ là một phần tử $\geq 0$ của $(G/H) \times H$ được sắp thứ tự từ điển. Nếu $y > 0$, lớp kề của H chứa $j(y, x)$ là một phần tử $> 0$, do đó $j(y, x) > 0$, vì nếu không thì $y \leq 0$ (§ 4, no. 2, Mệnh đề 3). Nếu $y = 0$ và $x \geq 0$, thì $j(y, x) = x \geq 0$. Suy ra $j$ chắc chắn là tăng.

### 3. TRƯỜNG HỢP CỦA MỌI MỞ RỘNG SIÊU VIỆT

Trong no. này ta sẽ dùng ký hiệu sau : $K$ là một trường, $K'$ là một mở rộng của $K$, $v$ là một định giá trên $K$, $v'$ là một mở rộng của $v$ lên $K$, $\Gamma$ và $k$ (tương ứng $\Gamma'$ và $k'$) là nhóm cấp và trường thặng dư của $v$ (tương ứng $v'$). Ta sẽ viết:

$$
d(K'/K) = \dim.\mathrm{al},\ K' = \text{bậc siêu việt của } K' \text{ trên } K;
$$
$$
s(v'/v) = \dim.\mathrm{al},\ k' = \text{bậc siêu việt của } k' \text{ trên } k;
$$
$$
r(v'/v) = r(\Gamma'/\Gamma) = \text{hạng hữu tỉ của } \Gamma'/\Gamma,
$$

nếu các vế phải là hữu hạn; nếu không, ta sẽ quy ước rằng $d(K'/K) = +\infty$ (tương ứng $s(v'/v) = +\infty, r(v'/v) = +\infty$).

#### Định lý 1 {#ac-vi-s10-thm-1 .statement}

*Cho $x_1, \ldots, x,$ là các phần tử của vành của $v'$ mà các ảnh chính tắc $\overline{x}_i$ của chúng trong $k'$ là độc lập đại số trên $k$ và $y_1, \ldots, y_r$ là các phần tử của $K'$ sao cho các ảnh chính tắc của các $v'(y_j)$ trong $\Gamma'/\Gamma$ là độc lập tuyến tính trên $\mathbf{Z}$. Khi đó $r+s$ phần tử $x_1, \ldots, x, y_1, \ldots, y_r$ của $K'$ là độc lập đại số trên $K$; hạn chế của $v'$ lên $K(x_1, \ldots, x, y_1, \ldots, y_r)$ nhận $k(\overline{x}_1, \ldots, \overline{x}_s)$ làm trường thặng dư và*

$$
\Gamma + \mathbf{Z}v'(y_1) + \ldots + \mathbf{Z}v'(y_r)
$$

*làm *nhóm cấp*.*

Mệnh đề của chúng ta là hiển nhiên nếu $r+s = 0$. Ta lập luận bằng quy nạp theo $r+s$. Nếu $r' \leq r, s' \leq s$ và $r'+s' < r+s$, giả thiết quy nạp cho thấy rằng các giả thiết của Định lý 1 được thỏa mãn nếu thay $K$ bằng $K(x_1, \ldots, x_s, y_1, \ldots, y_{r'})$ và thay các họ $(x_1, \ldots, x_s), (y_1, \ldots, y_r)$ bằng $(x_{s'+1}, \ldots, x_s), (y_{r'+1}, \ldots, y_r)$. Vì thế bài toán được quy về một trong hai trường hợp sau đây:

(a) Có một phần tử $x$ trong vành $v'$ sao cho $\overline{x}$ là siêu việt trên $k$; khi đó cần chứng minh rằng $x$ là siêu việt trên $K$ và hạn chế của $v'$ lên $K(x)$ nhận $k(\overline{x})$ làm trường thặng dư và $\Gamma$ làm nhóm cấp.

(b) Có một phần tử $y$ trong $K'$ sao cho các hệ thức $nv'(y) \in \Gamma$ và $n \in \mathbf{Z}$ kéo theo $n = 0$; cần chứng minh rằng $y$ là siêu việt trên $K$ và hạn chế của $v'$ lên $K(y)$ nhận $k$ làm trường thặng dư và $\Gamma + \mathbf{Z}v'(y)$ làm nhóm cấp.

Bây giờ Mệnh đề 1 của § 8, no. 1 cho thấy rằng $x$ (resp. $y$) không thể là đại số trên $K$. Các mệnh đề khác của (a) (resp. (b)) suy ra ngay lập tức từ Mệnh đề 2 (resp. Mệnh đề 1) của no. 1.

#### Hệ quả 1 {#ac-vi-s10-thm-1-cor-1 .statement}

*Bất đẳng thức*

$$
s(v'/v) + r(v'/v) \leq d(K'/K)
$$

*được thỏa mãn.*

*Hơn nữa, nếu $K'$ là một mở rộng sinh hữu hạn của $K$ và đẳng thức được thỏa mãn trong (9), thì $\Gamma'/\Gamma$ là một $\mathbf{Z}$-môđun sinh hữu hạn và $k'$ là một mở rộng sinh hữu hạn của $k$.*

Cho $r$ và $s$ là các số tự nhiên sao cho $r \leq r(v'/v)$ và $s \leq s(v'/v)$; ta chứng minh rằng $r+s \leq d(K'/K)$ và điều này sẽ chứng minh (9). Theo giả thiết, tồn tại các phần tử $x_1, \ldots, x, y_1, \ldots, y$, của $K'$, thỏa mãn các giả thiết của Định lý 1.

Vì thế chúng độc lập đại số trên $K$, điều đó cho thấy bất đẳng thức $r + s < d(K'/K)$.

Nếu $K'$ là một mở rộng sinh hữu hạn của $K$, $d(K'/K)$ là hữu hạn, do đó $s(v'/v)$ và $r(v'/v)$ cũng hữu hạn; ta ký hiệu chúng lần lượt là $s$ và $r$. Có các phần tử $x_1, \ldots, x_s, y_1, \ldots, y_r$ của $K'$ thỏa mãn các giả thiết của Định lý 1. Nếu $r + s = d(K'/K)$, các phần tử này tạo thành một cơ sở siêu việt của $K'$ trên $K$ và do đó $K'$ là một mở rộng đại số hữu hạn của $K'' = K(x_1, \ldots, y_r)$. Gọi $\Gamma''$ và $k''$ là nhóm cấp và trường thặng dư của hạn chế của $v'$ lên $K''$. Theo Định lý 1, $\Gamma''/\Gamma$ là một $\mathbf{Z}$-môđun sinh hữu hạn và $k''$ là một mở rộng thuần sinh hữu hạn của $k$. Mặt khác, vì $K'$ là một mở rộng đại số hữu hạn của $K$, $\Gamma'/\Gamma$ là một nhóm hữu hạn và $k'$ là một mở rộng đại số hữu hạn của $k''$ (§ 8, no. 1, Bổ đề 2). Điều này chứng minh hệ quả.

#### Hệ quả 2 {#ac-vi-s10-thm-1-cor-2 .statement}

*Cho h và h' là các chiều cao của v và v'. Khi đó*
$$
s(v'/v) + h' \leq d(K'/K) + h.
$$
Theo Mệnh đề 3, $h' \leq r(v'/v) + h$.

#### Hệ quả 3 {#ac-vi-s10-thm-1-cor-3 .statement}

*Giả sử rằng $K'$ là một mở rộng sinh hữu hạn của $K$, rằng $\Gamma$ đẳng cấu với $\mathbf{Z}^{h'}$ (có thứ tự theo từ điển) và có đẳng thức trong công thức (10). Khi đó $\Gamma'$ đẳng cấu với $\mathbf{Z}^{h'}$ (có thứ tự theo từ điển) và $k'$ là một mở rộng sinh hữu hạn của $k$.*

Nếu có đẳng thức trong (10), có đẳng thức trong (9), do đó có việc $k'$ là một mở rộng sinh hữu hạn của $k$ và $\Gamma''$ là một $\mathbf{Z}$-môđun sinh hữu hạn. Hơn nữa, so sánh (9) và (10), ta thấy rằng $h' - h = r(\Gamma'/\Gamma)$, do đó $h' = r(\Gamma')$ và khi đó Mệnh đề 4 (no. 2) cho thấy rằng $\Gamma'$ đẳng cấu với $\mathbf{Z}^{h'}$ có thứ tự theo từ điển.

#### Hệ quả 4 {#ac-vi-s10-thm-1-cor-4 .statement}

*Giả sử rằng v là không đúng (trong trường hợp đó $k = K$). Khi đó*
$$
h(\Gamma') + d(k'/K) \leq r(\Gamma') + D(k'/K) \leq d(K'/K).
$$
*Nếu, đặc biệt, v' có chiều cao 1, thì*
$$
d(k'/K) \leq d(K'/K) - 1;
$$
*hơn nữa, nếu $K'$ là một mở rộng sinh hữu hạn của $K$ và có đẳng thức trong (12), thì $v'$ là một định giá rời rạc và $k'$ là một mở rộng sinh hữu hạn của $K$.*

Đây là một chuỗi các trường hợp đặc biệt của các Hệ quả 1, 2, 3.

### Bài tập {#ac-vi-s10-exercises}

Xem [các bài tập của § 10](exercises/s10/).
