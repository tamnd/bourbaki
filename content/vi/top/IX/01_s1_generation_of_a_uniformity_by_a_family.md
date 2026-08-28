---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 1
section_title: Generation of a uniformity by a family of pseudometrics; uniformizable spaces
lang: vi
source: top-v-x
pdf_pages: 0143-0153, 0224-0232
extraction: ocr
subsections:
    - "no": 1
      title: PSEUDOMETRICS
      page: 0
      pdf_page: 143
    - "no": 2
      title: DEFINITION OF A UNIFORMITY BY MEANS OF A FAMILY OF PSEUDOMETRICS
      page: 0
      pdf_page: 144
    - "no": 3
      title: PROPERTIES OF UNIFORMITIES DEFINED BY FAMILIES OF PSEUDOMETRICS
      page: 0
      pdf_page: 147
    - "no": 4
      title: CONSTRUCTION OF A FAMILY OF PSEUDOMETRICS DEFINING A UNIFORMITY
      page: 0
      pdf_page: 148
    - "no": 5
      title: UNIFORMIZABLE SPACES
      page: 0
      pdf_page: 150
    - "no": 6
      title: SEMI-CONTINUOUS FUNCTIONS ON A UNIFORMIZABLE SPACE
      page: 0
      pdf_page: 152
statements: 15
exercises: 22
content_sha256: 86c70cd2d698f2e681d2001f6b117c6c5301444124bdbbc5db0482a25f3fa5bb
translated_from: content/en/top/IX/01_s1_generation_of_a_uniformity_by_a_family.md
source_content_sha256: d46241dcc6e0b3fdc75ac577e2626154c33e198b02447a07198d181994f0f47a
translation_model: gpt-5.4, gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-cb3b5371
glossary_version: 34
glossary_terms_sha256: 709bfd7a42f34ab5a5f743576bbcddb52468132228fde130ad448164a75531c0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. SINH MỘT CẤU TRÚC ĐỀU BỞI MỘT HỌ GIẢ KHOẢNG CÁCH; CÁC KHÔNG GIAN KHẢ CẤU TRÚC ĐỀU

### 1. GIẢ KHOẢNG CÁCH

Định nghĩa I. *Cho X là một tập hợp, một giả khoảng cách trên X là mọi ánh xạ f của X × X vào khoảng [0, +∞] của đường thẳng thực mở rộng $\overline{\mathbf{R}}$ thỏa mãn các điều kiện sau:

(EC_I) *Với mọi $x \in X, f(x, x) = 0$.
(EC_{II}) *Với mọi $x \in X$ và mọi $y \in X, f(x, y) = f(y, x)$ (đối xứng).
(EC_{III}) *Với mọi $x, y, z$ trong X,
$$
f(x, y) \leq f(x, z) + f(z, y)
$$
(bất đẳng thức tam giác).

#### Ví dụ 1 {#top-ix-s1-n1-exa-1 .statement}

Trên không gian số thực $\mathbf{R}^n$, khoảng cách Euclid (Chương VI, § 2, no. 1) là một giả khoảng cách.
2) Nếu X là một tập hợp bất kỳ, thì hàm f xác định trên $X \times X$ bởi các điều kiện $f(x, x) = 0$ với mọi $x \in X, f(x, y) = +\infty$ nếu $x \neq y$ là một giả khoảng cách trên X.
3) Nếu X là một tập hợp bất kỳ và nếu g là một hàm nhận giá trị thực hữu hạn bất kỳ xác định trên X, thì hàm f xác định trên $X \times X$ bởi $f(x, y) = |g(x) - g(y)|$ là một giả khoảng cách trên X.
\* 4) Cho X là tập hợp mọi ánh xạ liên tục từ khoảng [0, 1] của $\mathbf{R}$ vào $\mathbf{R}$. Nếu với mỗi cặp phần tử $x, y$ của X ta đặt
$$
f(x, y) = \int_0^1 |x(t) - y(t)| \, dt,
$$
thì f là một giả khoảng cách trên X. \*

Nhận xét:
1) Ví dụ 2 ở trên cho thấy rằng một giả khoảng cách có thể nhận giá trị $+\infty$ đối với một số cặp phần tử của $X$.
2) Nếu $f$ là một giả khoảng cách trên $X$, nói chung ta có thể có $f(x, y) = 0$ mà không có $x = y$, như Ví dụ 3 ở trên cho thấy (xem § 2).

Từ bất đẳng thức tam giác suy ra rằng nếu $f(x, z)$ và $f(y, z)$ là hữu hạn thì $f(x, y)$ cũng vậy; hơn nữa, trong trường hợp này ta có
$$
f(x, z) \leq f(y, z) + f(x, y) \quad \text{and} \quad f(y, z) \leq f(x, z) + f(x, y),
$$
do đó
(I)
$$
|f(x, z) - f(y, z)| \leq f(x, y).
$$

Nếu $f$ là một giả khoảng cách trên $X$, thì với mọi số thực hữu hạn $k > 0$, $kf$ cũng vậy. Nếu $\{f_i\}_{i \in I}$ là một họ giả khoảng cách bất kỳ trên $X$, tổng $\sum_{i \in I} f_i$ được xác định với mọi $x, y \in X \setminus X$; nếu $f$ ký hiệu giá trị của tổng này, thì $f$ là một giả khoảng cách trên $X$. Tương tự, cận trên đúng của họ $\{f_i\}$ (Chương IV, § 5, no. 5) là một giả khoảng cách trên $X$, vì các hệ thức $f_i(x, y) \leq f_i(x, z) + f_i(z, y)$ kéo theo
$$
\sup_{i \in I} f_i(x, y) \leq \sup_{i \in I} (f_i(x, z) + f_i(z, y)) \leq \sup_{i \in I} f_i(x, z) + \sup_{i \in I} f_i(z, y)
$$
[Chương IV, § 5, no. 7, công thức (17)].

### 2. ĐỊNH NGHĨA MỘT CẤU TRÚC ĐỀU BẰNG MỘT HỌ GIẢ KHOẢNG CÁCH

Ta đã thấy trong Chương VI, § 2, no. 3 rằng nếu, với mỗi số thực $s > 0$, ta ký hiệu bởi $U_s$ tập hợp mọi cặp $(x, y)$ điểm của $\mathbf{R}^n$ có khoảng cách Euclid không vượt quá $\leq s$, thì các $U_s$ tạo thành một hệ cơ bản các lân cận đều của cấu trúc đều của $\mathbf{R}^n$ khi $s$ chạy qua tập hợp các số thực $> 0$.

Nói chung, cho $f$ là một giả mêtric trên một tập hợp $X$: với mỗi $s > 0$, ký hiệu $U_s$ là $f^{-1}([0, s])$, và ta hãy chứng minh rằng, khi $s$ chạy qua tập hợp tất cả các số thực $> 0$, các $U_s$ tạo thành một hệ cơ bản của một cấu trúc đồng nhất trên $X$. Tiên đề $U_1$ được thỏa mãn do $\mathrm{(EC_1)}$: nếu $s = t$, ta có $U_s \subset U_t$ và do đó các $U_s$ thỏa mãn $B_1$: theo $\mathrm{(EC_{11})}$, ta có $U_s \cup U_s$ và do đó $U_{2s}$ được thỏa mãn; cuối cùng, theo $\mathrm{(EC_{111})}$, ta có $U_s = U_{2s}$, sao cho $U_{2s}$ được thỏa mãn. (Xem Chương II, § 1, no. 1, Định nghĩa 2). Do đó ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 2 {#top-ix-s1-def-2 .statement}

Cho một giả mêtric $f$ trên một tập hợp $X$, cấu trúc đồng nhất được định nghĩa bởi $f$ là cấu trúc đồng nhất trên $X$ có một hệ cơ bản của các lân cận là họ các tập hợp $\overline{f}^{-1}([0, a])$, trong đó $a$ chạy qua tập hợp tất cả các số thực $> 0$.

Hai giả mêtric trên $X$ được gọi là tương đương nếu chúng định nghĩa cùng một cấu trúc đồng nhất.

#### Nhận xét 1 {#top-ix-s1-n2-rem-1 .statement}

Nếu $(a_n)$ là một dãy bất kỳ các số $> 0$ và dần tới 0, các $U_{a_n}$ tạo thành một hệ cơ bản của các lân cận của cấu trúc đồng nhất được định nghĩa bởi $f$.
2) Định nghĩa một cấu trúc đồng nhất bởi một giả mêtric $f$ bao gồm việc lấy làm hệ cơ bản của các lân cận ảnh ngược qua $f$ của lọc lân cận của 0 trong không gian con $[0, +\infty]$ của $\overline{\mathbf{R}}$. Chú ý rằng thủ tục này hoàn toàn tương tự với thủ tục cho phép ta định nghĩa các cấu trúc đồng nhất trên một nhóm tôpô (Chương III, § 3, no. 1).

Cho $f$ và $g$ là hai giả mêtric trên $X$. Từ Định nghĩa 2 suy ra rằng cấu trúc đồng nhất được định nghĩa bởi $f$ thô hơn cấu trúc đồng nhất được định nghĩa bởi $g$ khi và chỉ khi, với mỗi $a > 0$ tồn tại $b > 0$ sao cho quan hệ $g(x, y) \leq b$ kéo theo $f(x, y) \leq a$. Một điều kiện cần và đủ để $f$ và $g$ là các giả mêtric tương đương là với mỗi $a > 0$ tồn tại $b > 0$ sao cho $g(x, y) \leq b$ kéo theo $f(x, y) \leq a$, và $f(x, y) \leq b$ kéo theo $g(x, y) \leq a$.

Đặc biệt, nếu tồn tại một hằng $k$ sao cho $f \leq kg$, thì cấu trúc đồng nhất được định nghĩa bởi $f$ thô hơn cấu trúc đồng nhất được định nghĩa bởi $g$.

Cho $\varphi$ là một ánh xạ của khoảng $[0, +\infty]$ vào chính nó, thỏa mãn các điều kiện sau: 1) $\varphi(0) = 0$, và $\varphi$ liên tục tại 0; 2) $\varphi$ tăng trong $[0, +\infty]$ và tăng ngặt trong một lân cận của 0; 3) với mọi $u \geq 0$ và $v \geq 0$, ta có $\varphi(u + v) \leq \varphi(u) + \varphi(v)$. Khi đó nếu $f$ là một giả mêtric bất kỳ trên một tập hợp $X$, hợp thành $g = \varphi \circ f$ là một giả mêtric tương đương với $f$.

Người đọc có thể dễ dàng kiểm tra rằng, chẳng hạn, ta có thể lấy $\varphi$ là một trong các hàm sau:

$$
\sqrt{u}, \quad \log (1 + u), \quad \frac{u}{1 + u}, \quad \inf (u, 1).
$$

Hai ví dụ cuối cùng cho thấy rằng luôn tồn tại các giả mêtric bị chặn tương đương với mọi giả mêtric đã cho (hữu hạn hoặc không).

#### Định nghĩa 3 {#top-ix-s1-def-3 .statement}

Nếu $(f_i)_{i \in I}$ là một họ các giả mêtric trên một tập hợp $X$, thì cận trên nhỏ nhất của tập hợp các cấu trúc đều được xác định trên $X$ bởi các giả mêtric $f_i$ được gọi là cấu trúc đều được xác định bởi họ $(f_i)$.

Hai họ các giả mêtric trên $X$ được gọi là tương đương nếu chúng xác định cùng một cấu trúc đều trên $X$.

Từ định nghĩa về cận trên nhỏ nhất của một tập hợp các cấu trúc đều (Chương II, § 2, no. 5), bộ lọc của các lân cận đều của cấu trúc đều $U$ được xác định trên $X$ bởi một họ các giả mêtric $(f_i)_{i \in I}$ là bộ lọc *sinh* (Chương I, § 6, no. 2) bởi họ các tập hợp $f_i^{-1}([0, a])$, trong đó $i$ chạy qua $I$ và $a$ chạy qua tập hợp các số thực $> 0$. Nói cách khác, ta thu được một hệ cơ bản các lân cận đều của $\mathcal{U}$ bằng cách tiến hành như sau: ta lấy tùy ý một số hữu hạn các chỉ số $i_1, i_2, \ldots, i_n$ và, tương ứng với mỗi $i_k$, một số $a_k > 0$; sau đó ta xét tập hợp $V$ gồm các cặp $(x, y) \in X \times X$ sao cho $f_{i_k}(x, y) \leq a_k$ với $1 \leq k \leq n$; các tập hợp $V$ này (với mọi lựa chọn có thể của $n$, các $i_k$ và các $a_k$) tạo thành một hệ cơ bản các lân cận đều của $\mathcal{U}$. Hơn nữa, ta có thể hạn chế về trường hợp trong đó tất cả các $a_k$ đều bằng *cùng một* số $a > 0$, vì lân cận đều gồm tất cả các cặp $(x, y)$ sao cho

$$
\sup_{1 \leq k \leq n} (f_{i_k}(x, y)) \leq \inf_{1 \leq k \leq n} a_k
$$

hiển nhiên được chứa trong $V$.

Đối với mỗi tập con hữu hạn $H$ của $I$, ký hiệu $g_H$ là bao trên của họ $(f_i)_{i \in H}$. Khi $H$ chạy qua tập hợp tất cả các tập con hữu hạn của $I$ và $a$ chạy qua tập hợp các số thực $> 0$, các tập $g_H^{-1}([0, a])$ tạo thành một *hệ cơ bản các lân cận* của đều đặn $\mathcal{U}$. Khi đó các $g_H$ là các *giả metric* trên $X$ (no. 1), và bao trên của một số hữu hạn các hàm thuộc họ $(g_H)$ thuộc về họ này, theo định nghĩa; ta biểu thị tính chất này bằng cách nói rằng họ các giả metric $(g_H)$ là *bão hòa*. Do đó họ các giả metric $(g_H)$ *tương đương* với họ $(f_i)$, và được gọi là họ các giả metric thu được bằng cách *bão hòa* $(f_i)$. Từ những điều vừa nói suy ra rằng ta luôn có thể hạn chế việc xét các đều đặn được xác định bởi các họ giả metric *bão hòa*.

Trong trường hợp riêng khi $I$ là một tập *hữu hạn*, lập luận này cho thấy đều đặn được xác định bởi họ các giả metric $(f_i)_{i \in I}$ cũng được xác định bởi *một* giả metric $g = \sup_{i \in I} f_i$ duy nhất.

Cho $\mathcal{U}, \mathcal{U}'$ là hai đều đặn trên $X$, lần lượt được xác định bởi hai họ *bão hòa* $(f_i)_{i \in I}, (g_x)_{x \in K}$. Khi đó $\mathcal{U}$ *thô hơn* $\mathcal{U}'$ khi và chỉ khi, với mỗi chỉ số $i \in I$ và mỗi số thực $a > 0$, tồn tại một chỉ số $x \in K$ và một số $b > 0$ sao cho quan hệ $g_x(x, y) \leq b$ kéo theo $f_i(x, y) \leq a$.

*Ví dụ về một đều đặn được xác định bởi một họ các giả metric.* Cho $(f_i)_{i \in I}$ là một họ tùy ý các *(hữu hạn) hàm nhận giá trị thực* xác định trên một tập hợp $X$. Gọi $\mathcal{U}$ là đều đặn nhỏ nhất trên $X$ sao cho các $f_i$ liên tục đều (Chương II, § 2, no. 3). Khi đó từ định nghĩa các lân cận của $\mathcal{U}$ (*loc. cit.*) suy ra rằng $\mathcal{U}$ là đều đặn được xác định trên $X$ bởi các giả metric

$$
g_i(x, y) = |f_i(x) - f_i(y)|.
$$

### 3. CÁC TÍNH CHẤT CỦA CÁC ĐỀU ĐẶN ĐƯỢC XÁC ĐỊNH BỞI CÁC HỌ GIẢ METRIC

Cho $\mathcal{U}$ là một đều đặn được xác định trên một tập hợp $X$ bởi một họ các giả metric hữu hạn $(f_i)$. Nếu ta trang bị $X \times X$ đều đặn là tích của $\mathcal{U}$ với chính nó, thì mỗi hàm nhận giá trị thực $f_i$ đều *liên tục đều* trên $X \times X$; vì theo (1) ta có

$$
|f_i(x, y) - f_i(x', y')| \leq f_i(x, x') + f_i(y, y'),
$$

và do đó các quan hệ $f_i(x, x') \leq \varepsilon/2, f_i(y, y') \leq \varepsilon/2$ kéo theo

$$
|f_i(x, y) - f_i(x', y')| \leq \varepsilon.
$$

Để $\mathcal{U}$ là *Hausdorff* thì, theo định nghĩa các lân cận của $\mathcal{U}$, điều kiện cần và đủ là với mỗi cặp điểm *phân biệt* $x, y$ của $X$ tồn tại một chỉ số $i$ sao cho $f_i(x, y) \neq 0$.

Đặc biệt, nếu $\mathcal{U}$ được định nghĩa bởi một giả khoảng cách *duy nhất* $f$, thì $\mathcal{U}$ là Hausdorff khi và chỉ khi quan hệ $f(x, y) = 0$ kéo theo $x = y$ (x. § 2). Nếu $\mathcal{U}$ không là Hausdorff, thì giao của tất cả các lân cận của đường chéo của $\mathcal{U}$ là tập con của $X \times X$ gồm các cặp $(x, y)$ sao cho $f_i(x, y) = 0$ với mọi $i$; tập con này là đồ thị của một quan hệ tương đương $R$ trên $X$, và cấu trúc đều Hausdorff liên kết với $\mathcal{U}$ được định nghĩa trên $X/R$ (x. Chương II, § 3, no. 8). Khi đó dễ dàng kiểm tra rằng các hàm $f_i$ là tương thích (theo $x$ và theo $y$) với quan hệ $R$ (*Set Theory*, R, § 5, no. 7) và các hàm $\overline{f_i}$, thu được từ $f_i$ bằng cách chuyển qua thương (đối với $x$ và $y$), là các giả khoảng cách trên $X/R$ và xác định cấu trúc đều Hausdorff liên kết với $\mathcal{U}$ (x. § 2, no. 1).

Nếu $A$ là một tập con không rỗng của $X$, thì hạn chế trên $A \times A$ của một giả khoảng cách trên $X$ rõ ràng là một giả khoảng cách trên $A$. Cấu trúc đều được *cảm sinh* bởi $\mathcal{U}$ trên $A$ rõ ràng là cấu trúc đều được định nghĩa bởi họ các hạn chế trên $A \times A$ của các giả khoảng cách $f_i$.

Bây giờ ta hãy xét *phần bù chỉnh* của không gian đều $X$ khi $\mathcal{U}$ là Hausdorff.

#### Mệnh đề 1 {#top-ix-s1-prop-1 .statement}

*Cho $X$ là một không gian đều Hausdorff mà cấu trúc đều $\mathcal{U}$ của nó được định nghĩa bởi một họ các giả khoảng cách hữu hạn* $(f_i)$, *và gọi* $\hat{X}$ *là phần bù chỉnh* của $X$. Khi đó các hàm $f_i$ có thể được mở rộng liên tục lên $\hat{X} \times \hat{X}$; các hàm mở rộng $\bar{f}_i$ là các giả khoảng cách hữu hạn trên $\hat{X} \times \hat{X}$, và họ $(f_i)$ xác định cấu trúc đều của $\hat{X}$.

Trước hết, các $f_i$ có thể được mở rộng bởi tính liên tục lên $\hat{X} \times \hat{X}$, vì chúng liên tục đều trên $X \times X$; và các hàm mở rộng $\bar{f}_i$ liên tục đều trên $\hat{X} \times \hat{X}$ (Chương II, § 3, no. 6, Định lý 2); hơn nữa, chúng là các giả metric trên $\hat{X}$ nhờ nguyên lý mở rộng của các bất đẳng thức (Chương IV, § 5, no. 2, Định lý 1). Gọi $\mathcal{U}_1$ là cấu trúc đều trên $\hat{X}$ thu được bởi phép hoàn thành, và gọi $\mathcal{U}_2$ là cấu trúc đều được xác định bởi họ các giả metric $(\bar{f}_i)$. Khi đó $\mathcal{U}_2$ thô hơn $\mathcal{U}_1$; bởi vì mỗi $\bar{f}_i$ liên tục đều trên $\hat{X} \times \hat{X}$ đối với $\mathcal{U}_1$, và do đó với mỗi $a > 0$ tồn tại một lân cận $V$ của $\mathcal{U}_1$ sao cho, khi $(x, y) \in V$, ta có $|\bar{f}_i(x, y) - \bar{f}_i(x, x)| \leq a$, tức là [vì $\bar{f}_i(x, x) = 0$], $V \subset \bar{f}_i([0, a])$; do đó mọi lân cận của $\mathcal{U}_2$ là một lân cận của $\mathcal{U}_1$. Mặt khác, $\mathcal{U}_1$ và $\mathcal{U}_2$ cảm sinh cùng một cấu trúc đều $\mathcal{U}$ trên $X$. Vì $\hat{X}$ đầy đủ đối với $\mathcal{U}_1$, suy ra rằng $\mathcal{U}_1$ và $\mathcal{U}_2$ trùng nhau (Chương II, § 3, no. 7, Mệnh đề 14).

### 4. PHÉP DỰNG MỘT HỌ CÁC GIẢ METRIC XÁC ĐỊNH MỘT CẤU TRÚC ĐỀU

Ý nghĩa của việc định nghĩa một cấu trúc đều bằng một họ các giả metric nằm ở chỗ mọi cấu trúc đều đều có thể thu được theo cách đó. Cụ thể:

#### Định lý 1 {#top-ix-s1-thm-1 .statement}

Cho một cấu trúc đều $\mathcal{U}$ trên một tập hợp $X$, tồn tại một họ các giả metric trên $X$ sao cho cấu trúc đều được xác định bởi họ này trùng với $\mathcal{U}$.

Đối với mỗi lân cận $V$ của cấu trúc đều $\mathcal{U}$, định nghĩa quy nạp một dãy các lân cận đối xứng $(U_n)$ sao cho $U_1 \subset V$ và $U_{n+1} \subset U_n$ với mọi $n \geq 1$. Dãy $(U_n)$ là một hệ cơ bản các lân cận của một cấu trúc đều $\mathcal{U}_V$ thô hơn $\mathcal{U}$; hơn nữa, rõ ràng rằng $\mathcal{U}$ là cận trên nhỏ nhất của tất cả các cấu trúc đều $U_V$ khi $V$ chạy qua bộ lọc các lân cận của $\mathcal{U}$. Do đó Định lý 1 là một hệ quả của mệnh đề sau:

#### Mệnh đề 2 {#top-ix-s1-prop-2 .statement}

Nếu một cấu trúc đều $\mathcal{U}$ trên $X$ có một hệ cơ bản đếm được các lân cận, thì tồn tại một giả metric $f$ trên $X$ sao cho $\mathcal{U}$ trùng với cấu trúc đều được xác định bởi $f$.

Cho $(V_n)$ là một hệ cơ bản đếm được các lân cận của $\mathcal{U}$. Định nghĩa bằng quy nạp một dãy $(U_n)$ các lân cận đối xứng của $\mathcal{U}$ sao cho $U_1 \subset V_1$ và
$$
\bigcup_{n+1}^3 \subset U_n \cap V_n \quad \text{cho} \quad n \geq 1.
$$
Rõ ràng $(U_n)$ là một hệ cơ bản khác các lân cận của $\mathcal{U}$, và ta có đặc biệt $\bigcup_{n+1}^3 \subset U_n$ với $n \geq 1$. Ta định nghĩa một hàm nhận giá trị thực $g$ trên $X \times X$ như sau: $g(x, y) = 0$ nếu $(x, y) \in U_n$ với mọi $n$; $g(x, y) = 2^{-k}$ nếu $(x, y) \in U_n$ với $1 \leq n \leq k$, nhưng $(x, y) \notin U_{k+1}$; $g(x, y) = 1$ nếu $(x, y) \notin U_1$. Hàm $g$ là đối xứng và dương, và ta có $g(x, x) = 0$ với mọi $x \in X$. Đặt
$$
f(x, y) = \inf \sum_{i=0}^{p-1} g(z_i, z_{i+1}),
$$
cận dưới lớn nhất được lấy trên tập hợp tất cả các dãy hữu hạn $(z_i)_{0 \leq i \leq p}$ ($p$ tùy ý) sao cho $z_0 = x$ và $z_p = y$. Ta sẽ chứng minh rằng $f$ là một *giả metric* thỏa mãn các bất đẳng thức
$$
\frac{1}{2} g(x, y) \leq f(x, y) \leq g(x, y).
$$
Theo định nghĩa, ngay lập tức suy ra rằng $f$ là đối xứng và dương và thỏa mãn bất đẳng thức tam giác. Cũng rõ ràng là $f(x, y) \leq g(x, y)$, do đó $f(x, x) = 0$ với mọi $x \in X$, và vì vậy $f$ là một giả metric. Để chứng minh nửa bên trái của các bất đẳng thức (2), ta hãy chứng minh bằng quy nạp theo $p$ rằng, với mọi dãy hữu hạn $(z_i)_{0 \leq i \leq p}$ gồm $p + 1$ điểm của $X$ sao cho $z_0 = x$ và $z_p = y$, ta có
$$
\sum_{i=0}^{p-1} g(z_i, z_{i+1}) \geq \frac{1}{2} g(x, y).
$$
Điều này rõ ràng nếu $p = 1$. Đặt $a = \sum_{i=0}^{p-1} g(z_i, z_{i+1})$; bất đẳng thức (3) đúng nếu $a \geq 1/2$, vì $g(x, y) \leq 1$. Giả sử khi đó rằng $a < 1/2$, và gọi $h$ là lớn nhất trong các chỉ số $q$ sao cho
$$
\sum_{i < q} g(z_i, z_{i+1}) \leq \frac{a}{2};
$$
khi đó ta có $\sum_{i < h} g(z_i, z_{i+1}) \leq a/2$ và $\sum_{i < h+1} g(z_i, z_{i+1}) > a/2$, do đó
$$
\sum_{i > h} g(z_i, z_{i+1}) \leq \frac{a}{2}.
$$

Theo giả thiết quy nạp ta có $g(x, z_h) \leq a$ và $g(z_{h+1}, y) \leq a$; mặt khác rõ ràng là $g(z_h, z_{h+1}) \leq a$. Gọi $k$ là số nguyên nhỏ nhất $> 0$ sao cho $2^{-k} \leq a$; khi đó $k \geq 2$, và $(x, z_h) \in U_k, (z_h, z_{h+1}) \in U_k, (z_{h+1}, y) \in U_k$ theo định nghĩa của $g$; do đó $(x, y) \in U_k \subset U_{k-1}^3$, điều này suy ra rằng $g(x, y) \leq 2^{1-k} \leq 2a$.

Vậy các bất đẳng thức (2) đã được chứng minh; chúng chỉ ra rằng, với mỗi $a > 0$, tập hợp $f^{-1}([0, a])$ chứa $U_k$ với mỗi chỉ số $k$ sao cho $2^{-k} < a$, và ngược lại mỗi $U_k$ chứa tập hợp $f^{-1}([0, 2^{-k-1}])$; do đó các tập hợp $f^{-1}([0, a])$ tạo thành một hệ cơ bản các lân cận của cấu trúc $\mathcal{U}$.

Q.E.D.

#### Nhận xét {#top-ix-s1-n4-rem-1 .statement}

Một cấu trúc đều $\mathcal{U}$ trên $X$ được xác định bởi họ $\Phi$ gồm tất cả các giả mêtric trên $X$ liên tục đều trên $X \times X$. Rõ ràng cấu trúc đều được xác định bởi họ $\Phi$ là thô hơn $\mathcal{U}$; ngược lại, Định lý 1 chỉ ra rằng có một họ con của $\Phi$ xác định cấu trúc đều $\mathcal{U}$ và do đó cấu trúc đều được xác định bởi $\Phi$ là mịn hơn $\mathcal{U}$.

### 5. CÁC KHÔNG GIAN KHẢ NĂNG ĐỒNG ĐỀU HÓA

Trong Chương II, § 4, no. 1, chúng ta đã đặt ra bài toán đặc trưng các không gian tôpô khả năng đồng đều hóa. Lời giải được cho bởi định lý sau:

#### Định lý 2 {#top-ix-s1-thm-2 .statement}

*Một không gian tôpô* $X$ *là khả năng đồng đều hóa khi và chỉ khi nó thỏa mãn tiên đề sau:*

(OIV) *Với mọi điểm* $x_0 \in X$ *và mọi lân cận* $V$ *của* $x_0$, *tồn tại một hàm thực liên tục trên* $X$ *nhận các giá trị trong* $[0, 1]$, *bằng* $0$ *tại* $x_0$, *và bằng* $1$ *trên* $C_V$.

Điều kiện là cần thiết. Thật vậy, nếu có một cấu trúc đều trên $X$ tương thích với tôpô của $X$, thì theo Định lý 1 cấu trúc đều này có thể được xác định bởi một họ $(f_i)$ các giả mêtric trên $X$, và ta có thể giả sử không mất tính tổng quát rằng họ này là *bão hòa* (no. 2). Từ định nghĩa của các lân cận của cấu trúc đều được xác định bởi một họ các giả mêtric như vậy, có một giả mêtric $f_\alpha$ của họ $(f_i)$, và một số $a > 0$, sao cho $f_\alpha(x_0, x) \geq a$ với mọi $x \in C_V$. Suy ra rằng hàm $g(x) = \inf \left( 1, \frac{1}{a} f_\alpha(x_0, x) \right)$ thỏa mãn tất cả các điều kiện đã nêu trong (OIV).

Điều kiện là đủ. Thật vậy, đặt $\Phi$ là tập hợp tất cả các *ánh xạ liên tục* từ $X$ vào $[0, 1]$. Tiên đề (OIV) chỉ ra rằng *cấu trúc đều thô nhất mà đối với nó mọi hàm thuộc* $\Phi$ *đều liên tục đều là tương thích* với tôpô của $X$ (Chương II, § 2, no. 3).

#### Định nghĩa 4 {#top-ix-s1-def-4 .statement}

*Một không gian tôpô được gọi là chính quy hoàn toàn nếu nó là khả năng đồng đều hóa và Hausdorff.*

Tương đương, theo Định lý 2, một không gian là chính quy hoàn toàn nếu nó thỏa mãn các tiên đề (H) [xem Chương I, § 8, no. 1, Mệnh đề 1] và (O_{IV}).

#### Nhận xét {#top-ix-s1-n5-rem-1 .statement}

Tiên đề (O_{IV}) kéo theo (O_{III}) (xem Chương I, § 8, no. 4), vì nếu V là một lân cận của x_0 và nếu f là một hàm thực liên tục trên X nhận các giá trị trong [0, 1], sao cho f(x_0) = 0, f(x) = 1 với mọi x \in \overline{V}, thì tập hợp \overline{f}([0, 1/2]) là một lân cận đóng của x_0 được chứa trong V. Đặc biệt, mọi không gian *chính quy hoàn toàn* đều *chính quy* (điều này biện minh cho thuật ngữ). Nhưng có những ví dụ về các không gian chính quy không chính quy hoàn toàn (*), do đó (O_{III}) không kéo theo (O_{IV}).

Mọi không gian compact đều chính quy hoàn toàn (Chương II, § 4, no. 1, Định lý 1) và vì thế mọi không gian con của một không gian compact cũng vậy. Bây giờ ta có thể hoàn thành mệnh đề này bằng cách chứng minh *đảo lại* của nó:

#### Mệnh đề 3 {#top-ix-s1-prop-3 .statement}

*Một không gian tôpô X là chính quy hoàn toàn khi và chỉ khi nó đồng phôi với một không gian con của một không gian compact.*

Xét cấu trúc đều thô nhất trên X sao cho mọi ánh xạ liên tục từ X vào [0, 1] đều liên tục đều; ta đã sử dụng cấu trúc đều này trong chứng minh Định lý 2, trong đó ta thấy rằng nó tương thích với tôpô của X nếu X là khả năng đồng đều hóa. Hơn nữa, cấu trúc đều này là một cấu trúc của một không gian *tiền compact*, do tính compact của khoảng [0, 1] và Mệnh đề 3 của Chương II, § 4, no. 2. Nếu X là Hausdorff, sự hoàn thành của X đối với cấu trúc này do đó là compact, và mệnh đề được chứng minh.

Do đó ta có thể nói rằng một không gian chính quy hoàn toàn có thể được *nhúng* vào một không gian compact. Thường tiện lợi khi trình bày kết quả này theo cách sau:

Nói chung, một *hộp* là một không gian tôpô K^I, tích của một họ các không gian tôpô mà mỗi không gian đều đồng nhất với một *khoảng compact* K của \mathbf{R}, được đánh chỉ số bởi một tập hợp tùy ý I. Nếu I là hữu hạn và có n phần tử, ta thu lại khái niệm về một *hộp đóng n-chiều*, được định nghĩa trong Chương VI, § 1, no. 1. Một hộp là một không gian *compact* (Chương I, § 9, no. 5, Định lý 3).

#### Mệnh đề 4 {#top-ix-s1-prop-4 .statement}

*Nếu một không gian tôpô X là chính quy hoàn toàn, nó đồng phôi với một không gian con của một hộp.*

Gọi $(f_i)_{i \in I}$ là họ tất cả các ánh xạ liên tục từ X vào K = [0, 1], và gọi g là ánh xạ $x \mapsto (f_i(x))$ từ X vào

(*) Xem A. Tychonoff, *Math. Ann.*, 102, (1930), p. 553.

K¹. Nếu $x, y$ là hai điểm phân biệt bất kỳ của $X$, suy ra từ các tiên đề (H) và (O_IV) rằng có một chỉ số $i$ sao cho $f_i(x) \neq f_i(y)$, và do đó $g$ là một ánh xạ *một-một* của $X$ vào $K^1$. Hơn nữa, ngay lập tức thấy rằng $g$ là một đẳng cấu của cấu trúc đều thô nhất trên $X$ mà tất cả các $f_i$ đều liên tục đều, lên cấu trúc đều cảm sinh trên $g(X)$ bởi cấu trúc đều tích của $K^1$; *a fortiori*, $g$ là một đồng phôi của $X$ lên $g(X)$.

### 6. CÁC HÀM NỬA LIÊN TỤC TRÊN MỘT KHÔNG GIAN CÓ THỂ ĐỀU HÓA

Trong Chương IV, § 6, no. 2, Hệ quả của Định lý 4, ta đã chỉ ra rằng bao trên của một họ các hàm liên tục nhận giá trị thực trên một không gian tôpô là một hàm nửa liên tục dưới. Nếu không gian là *có thể đều hóa*, thì có đảo lại của mệnh đề này:

#### Mệnh đề 5 {#top-ix-s1-prop-5 .statement}

*Để mọi hàm nhận giá trị thực nửa liên tục dưới $f$ (hữu hạn hoặc không) trên một không gian tôpô $X$ đều là bao trên của các hàm liên tục nhận giá trị thực trên $X$ (hữu hạn hoặc không) thỏa mãn $\leq f$, điều kiện cần và đủ là $X$ có thể đều hóa.*

Điều kiện là *cần*. Cho $x_0$ là một điểm bất kỳ của $X$ và cho $V$ là một lân cận mở bất kỳ của $x_0$; khi đó hàm đặc trưng $\varphi_V$ của tập hợp $V$ là nửa liên tục dưới (Chương IV, § 6, no. 2, Hệ quả của Mệnh đề 1); theo giả thiết, do đó tồn tại một hàm liên tục nhận giá trị thực $g$ trên $X$ sao cho $g \leq \varphi_V$ và $g(x_0) = a > 0$. Hàm liên tục $\inf \left( 1, \frac{1}{a} g^+ \right)$ nhận các giá trị của nó trong $[0, 1]$, bằng 0 trên $C_V$, và bằng 1 tại $x_0$. Vậy (Định lý 2) $X$ có thể đều hóa.

Điều kiện là *đủ*. Trước hết xét trường hợp $f$ nhận các giá trị của nó trong $[-1, +1]$. Ta phải chỉ ra rằng, với mỗi $x_0 \in X$ và mỗi số $a < f(x_0)$, có một hàm liên tục nhận giá trị thực $g$ trên $X$ sao cho $g \leq f$ và $g(x_0) \geq a$. Nếu $a \leq -1$, ta có thể lấy $g$ là hằng $-1$. Nếu $-1 < a < f(x_0)$, có một lân cận $V$ của $x_0$ sao cho $f(x) \geq a$ với mọi $x \in V$. Vì $X$ có thể đều hóa, có một hàm liên tục nhận giá trị thực $h$ trên $X$, với các giá trị trong $[0, 1]$, sao cho $h(x_0) = 0$ và $h(x) = 1$ với mọi $x \in C_V$. Khi đó ta có thể lấy $g(x) = a - (a + 1)h(x)$, và ta có một hàm liên tục thỏa mãn các điều kiện đã nêu. Chú ý rằng hàm này nhận các giá trị của nó trong $[-1, +1]$.

Trường hợp tổng quát suy ra bằng phép chuyển cấu trúc; vì có một đồng phôi tăng ngặt từ $[-1, +1]$ lên $\overline{\mathbf{R}}$ (Chương IV, § 4, no. 2, Mệnh đề 2), và định nghĩa của một hàm nửa liên tục chỉ dùng cấu trúc thứ tự và tôpô của $\overline{\mathbf{R}}$.

#### Nhận xét {#top-ix-s1-n6-rem-1 .statement}

Trong chứng minh trên, ta thấy rằng hàm $g$ không nhận giá trị $+1$. Bằng phép chuyển cấu trúc suy ra rằng mọi hàm thực nửa liên tục dưới $f$ trên không gian có thể nhất quán hóa $X$ đều là bao trên của các hàm thực liên tục $g \leq f$ trên $X$ *không nhận giá trị* $+\infty$.

### Bài tập {#top-ix-s1-exercises}

Xem [bài tập của § 1](exercises/s1/).
