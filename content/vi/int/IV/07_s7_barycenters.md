---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 7
section_title: Barycenters
lang: vi
source: int-i-vi
book_pages: INT IV.142-INT IV.148
pdf_pages: 0208-0225, 0249-0255
extraction: ocr
subsections:
    - "no": 1
      title: Definition of barycenters
      page: 101
      pdf_page: 208
    - "no": 2
      title: Extremal points and barycenters
      page: 102
      pdf_page: 209
    - "no": 3
      title: 'Applications: I. Vector spaces of continuous real functions'
      page: 106
      pdf_page: 213
    - "no": 4
      title: 'Applications: II. Vector spaces of continuous complex functions'
      page: 110
      pdf_page: 217
    - "no": 5
      title: 'Applications: III. Algebras of continuous functions'
      page: 111
      pdf_page: 218
    - "no": 6
      title: Uniqueness of integral representations
      page: 115
      pdf_page: 222
statements: 31
exercises: 10
content_sha256: a4f7743ed017f92f935a56ed007b20d75dabc04601ecb78ee98b27a2c858eb09
translated_from: content/en/int/IV/07_s7_barycenters.md
source_content_sha256: d918fc8bfca5bdbfb7f09764b73864ce7ca0e6b0610a120b0c82f1ca0bbd082a
translation_model: gpt-5.4
translation_run: translate-vi-69c0d390
glossary_version: 34
glossary_terms_sha256: f1400a095988633b745d602b6f0ddae50715c03dbfd249b51d56bb86ffb19c37
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. TRỌNG TÂM

### 1. Định nghĩa trọng tâm

Cho E là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$, $E'$ là đối ngẫu của nó, và ${E'}^*$ là đối ngẫu đại số của $E'$, trong đó E được đồng nhất một cách chính tắc với một không gian con tuyến tính của ${E'}^*$. Cho K là một tập con compắc của E; do đơn ánh chính tắc từ K vào E là liên tục với giá compact, nên với mọi độ đo $\mu$ trên K, tích phân $\int x\, d\mu(x)$ được xác định và là một phần tử của ${E'}^*$ (Ch. III, §3, No. 1). Hơn nữa, trên K, tôpô cảm sinh bởi tôpô yếu $\sigma({E'}^*, E')$ trùng với tôpô ban đầu. Cuối cùng, nếu C là bao lồi đóng của K trong ${E'}^*$ được trang bị $\sigma({E'}^*, E')$, thì $C \cap E$ là bao lồi đóng của K trong E đối với tôpô ban đầu (hoặc đối với tôpô yếu đi $\sigma(E, E')$).

#### Định nghĩa 1 {#int-iv-s7-def-1 .statement}

*Cho K là một tập con compắc của một không gian lồi địa phương Hausdorff E. Với mọi độ đo dương $\mu$ trên K có tổng khối lượng bằng 1, vectơ $b_\mu = \int x\, d\mu(x)$ (thuộc ${E'}^*$) được gọi là trọng tâm của $\mu$.*

#### Ví dụ {#int-iv-s7-n1-exa-1 .statement}

— Cho $\mu$ là một độ đo *rời rạc* trên K, dương và có tổng khối lượng bằng 1; khi đó nó có dạng $\mu = \sum_{i=1}^n \lambda_i \varepsilon_{x_i}$, trong đó $x_i \in K$, và các $\lambda_i$ là những số thực sao cho $\lambda_i \geq 0$ với mọi $i$ và $\sum_{i=1}^n \lambda_i = 1$. Vì $\int x\, d\varepsilon_y(x) = y$ (Ch. III, §3, No. 1, *Ví dụ 3*), nên $b_\mu = \int x\, d\mu(x) = \sum_i \lambda_i x_i$. Đặc biệt, với mọi $x \in K$, x là trọng tâm của độ đo $\varepsilon_x$.

#### Mệnh đề 1 {#int-iv-s7-prop-1 .statement}

*Cho E là một không gian lồi địa phương Hausdorff, K là một tập con compắc của E, và C là bao lồi đóng của K trong E. Khi đó tập C gồm các điểm của E là trọng tâm của ít nhất một độ đo dương khối lượng 1 trên K.*

Điều này không là gì khác hơn Mệnh đề 5 của Ch. III, §3, No. 2 áp dụng cho đơn ánh chính tắc từ K vào E.

#### Hệ quả {#int-iv-s7-n1-cor-1 .statement}

*Nếu bao lồi đóng C của K trong E là compắc, thì trọng tâm của mọi độ đo dương có tổng khối lượng 1 trên K đều thuộc E.*

Thật vậy, khi đó C cũng là bao lồi đóng của K trong ${E'}^*$ được trang bị tôpô yếu $\sigma(E', E')$, và chỉ cần áp dụng, cho đơn ánh chính tắc từ K vào E, Mệnh đề 4 của Ch. III, §3, No. 2.

#### Nhận xét {#int-iv-s7-n1-rem-1 .statement}

Hệ quả của Mệnh đề 1 áp dụng được đặc biệt khi K lồi hoặc khi E là gần đầy đủ.

#### Mệnh đề 2 {#int-iv-s7-prop-2 .statement}

— Cho K là một tập con compắc lồi của một không gian lồi địa phương Hausdorff E, $\mu$ là một độ đo dương có tổng khối lượng 1 trên K, $b_\mu$ là trọng tâm của nó. Với mọi hàm số lồi $f \geq 0$ nửa liên tục dưới trên K,
$$
f(b_\mu) \leq \int^* f d\mu.
$$
Người ta biết (TVS, II, §5, No. 4, Mệnh đề 5) rằng $f$ là bao trên của một họ các hạn chế lên K của các hàm afin tuyến tính liên tục $h_\alpha : x \mapsto c_\alpha + \langle x, z'_\alpha \rangle$. Khi đó
$$
\int h_\alpha(x) d\mu(x) \leq \int^* f(x) d\mu(x)
$$
với mọi $\alpha$; mà $\int h_\alpha(x) d\mu(x) = c_\alpha + \int \langle x, z'_\alpha \rangle d\mu(x)$ vì $\mu$ có tổng khối lượng 1; nhưng $\int \langle x, z'_\alpha \rangle d\mu(x) = \langle b_\mu, z'_\alpha \rangle$ theo định nghĩa trọng tâm. Do đó $\sup_\alpha \int h_\alpha(x) d\mu(x) = \sup_\alpha h_\alpha(b_\mu) = f(b_\mu)$, do đó suy ra kết luận.

Khi $\mu$ là một độ đo dương rời rạc trên K có tổng khối lượng 1, Mệnh đề 2 lại cho bất đẳng thức dùng để định nghĩa các hàm lồi trên K.

#### Hệ quả {#int-iv-s7-n1-cor-2 .statement}

— Với mọi hàm số lồi g trên K bị chặn và nửa liên tục dưới, $g(b_\mu) \leq \int g d\mu$.

Chỉ cần chú ý rằng $\inf_{x \in K} g(x) = a$ là hữu hạn và áp dụng Mệnh đề 2 cho $g - a$.

### 2. Các điểm cực biên và trọng tâm

#### Mệnh đề 3 {#int-iv-s7-prop-3 .statement}

— Cho K là một tập con compắc lồi của một không gian lồi địa phương Hausdorff E, x là một điểm của K. Mọi độ đo $\mu$ trên K, dương, có tổng khối lượng 1, và nhận x làm trọng tâm, đều nằm trong bao đóng mờ của tập các độ đo dương rời rạc có tổng khối lượng 1 và nhận x làm trọng tâm.

Cho U là một lân cận của $\mu$ đối với tôpô mờ; ta có thể giả sử rằng U gồm các độ đo $\nu$ trên K sao cho
$$
|\mu(f_i) - \nu(f_i)| \leq \delta
$$
với một số hữu hạn các hàm $f_i \in \mathcal{C}(K; \mathbf{C})$ ($1 \leq i \leq p$) và một số $\delta > 0$. Với mọi điểm $a \in K$, tồn tại một lân cận lồi đóng $V_a$ của 0 trong E sao cho
$$
|f_i(y) - f_i(a)| \leq \delta/2
$$

với $1 \leq i \leq p$ và với mọi $y \in W_a = K \cap (a + V_a)$. Vì $K$ compắc, tồn tại một số hữu hạn điểm $a_j$ ($1 \leq j \leq r$) của $K$ sao cho các $W_{a_j}$ tạo thành một phủ của $K$ ($1 \leq j \leq r$). Xét một phân hoạch đơn vị liên tục $(g_j)_{1 \leq j \leq r}$ trên $K$, phụ thuộc vào phủ $(W_{a_j})$, và đặt $\alpha_j = \mu(g_j)$ với mọi $j$; nếu $\alpha_j \neq 0$ thì đặt $\mu_j = \alpha_j^{-1} g_j \cdot \mu$, và nếu $\alpha_j = 0$ thì đặt $\mu_j = \varepsilon_{a_j}$. Mỗi độ đo $\mu_j$ đều dương, có khối lượng toàn phần bằng 1, và giá của nó được chứa trong tập hợp compắc lồi $W_{a_j}$; hơn nữa, theo định nghĩa,

$$
\mu = \sum_{j=1}^r \alpha_j \mu_j
$$

vì $g_j \cdot \mu = 0$ nếu $\mu(g_j) = 0$; các $\alpha_j$ đều $\geq 0$ và

$$
\sum_{j=1}^r \alpha_j = \sum_{j=1}^r \mu(g_j) = \mu \left( \sum_{j=1}^r g_j \right) = \mu(1) = 1 .
$$

Gọi $x_j$ là trọng tâm của $\mu_j$, thuộc $W_{a_j}$ (No. 1, Mệnh đề 1), và xét độ đo rời rạc $\nu = \sum_{j=1}^r \alpha_j \varepsilon_{x_j}$; nó là dương và có khối lượng toàn phần bằng 1, và trọng tâm của nó là $\sum_{j=1}^r \alpha_j x_j$, cũng là trọng tâm của $\mu$ theo (3), do đó bằng $x$. Hơn nữa, theo (2), $|f_i(y) - f_i(a_j)| \leq \delta/2$ với mọi $y \in W_{a_j}$ và với mọi $i$, do đó, vì $\operatorname{Supp}(\mu_j) \subset W_{a_j}$, ta có $|\mu_j(f_i) - f_i(a_j)| \leq \delta/2$ với $1 \leq i \leq p$. Mặt khác, vì $x_j \in W_{a_j}$, ta cũng có

$$
|\varepsilon_{x_j}(f_i) - f_i(a_j)| \leq \delta/2
$$

với $1 \leq i \leq p$, do đó $|\mu_j(f_i) - \varepsilon_{x_j}(f_i)| \leq \delta$ với mọi $i$ và $j$. Vì các $\alpha_j$ đều $\geq 0$ và có tổng bằng 1, suy ra từ (3) và từ định nghĩa của $\nu$ rằng $\nu$ thỏa mãn bất đẳng thức (1).

Điều phải chứng minh.

#### Hệ quả {#int-iv-s7-n2-cor-1 .statement}

— *Cho $K'$ là một tập con compắc của $K$ sao cho $K$ là bao lồi đóng của $K'$. Để $x \in K'$ là một điểm cực biên của $K$, điều kiện cần và đủ là $\varepsilon_x$ là độ đo dương duy nhất trên $K'$, có khối lượng toàn phần bằng 1, nhận $x$ làm trọng tâm.*

Giả sử $x$ là một điểm cực biên của $K$; để chứng minh rằng $\varepsilon_x$ là độ đo dương duy nhất trên $K'$, có tổng khối lượng bằng 1, nhận $x$ làm trọng tâm, theo Mệnh đề 3, chỉ cần thấy rằng tập hợp các độ đo *rời rạc* $\nu$ trên $K'$ vừa dương, vừa có tổng khối lượng bằng 1, vừa nhận $x$ làm trọng tâm, thu về $\varepsilon_x$. Nhưng một độ đo như thế $\nu$ có dạng $\sum_{i=1}^r \lambda_i \varepsilon_{x_i}$ với $\lambda_i > 0$ đối với $1 \leq i \leq r$ và $\sum_{i=1}^{r} \lambda_i = 1$, và giả thiết rằng $x$ là trọng tâm của $\nu$ có thể được viết thành $x = \sum_{i=1}^{r} \lambda_i x_i$. Vì $x$ là cực biên, điều này suy ra $x_i = x$ với mọi $i$, do đó $\nu = \varepsilon_x$.

Ngược lại, giả sử rằng $\varepsilon_x$ là độ đo dương duy nhất trên $K'$, có tổng khối lượng bằng 1, nhận $x$ làm trọng tâm, và hãy chứng minh rằng $x$ là cực biên. Trong trường hợp ngược lại, sẽ tồn tại hai điểm phân biệt $x', x''$ của $K$ và một số thực $\lambda$ sao cho $0 < \lambda < 1$ và $x = \lambda x' + (1 - \lambda) x''$. Theo Mệnh đề 1, $x'$ (tương ứng $x''$) là trọng tâm của một độ đo dương $\mu'$ (tương ứng $\mu''$) trên $K'$ có tổng khối lượng bằng 1. Khi đó $x$ là trọng tâm của $\lambda \mu' + (1 - \lambda) \mu''$. Vậy $\lambda \mu' + (1 - \lambda) \mu'' = \varepsilon_x$. Do đó $\mu'$ và $\mu''$ tỉ lệ với $\varepsilon_x$, suy ra $x' = x'' = x$, điều này vô lý.

#### Định lý 1 (Choquet) {#int-iv-s7-thm-1 .statement}

— *Cho E là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$, K là một tập con lồi compắc khả mêtric của E, và M là tập hợp các điểm cực biên của K. Tập hợp M là giao của một họ đếm được các tập mở trong K, và mọi điểm của K đều là trọng tâm của một độ đo $\mu$ trên K sao cho $\mu(K - M) = 0$.*

Để chứng minh mệnh đề thứ nhất, ký hiệu bởi I khoảng $[0, 1]$ của $\mathbf{R}$; vì K compac và khả mêtric hóa, nên $K \times K \times I$ cũng vậy; tập con U của $K \times K \times I$ gồm các bộ ba $(x, y, \lambda)$ sao cho $x \neq y$ và $0 < \lambda < 1$ là mở trong $K \times K \times I$, do đó tồn tại một dãy $(F_n)$ các tập đóng trong $K \times K \times I$ mà hợp là U (GT, IX, §2, No. 5, Mệnh đề 7). Ánh xạ $q : K \times K \times I \to K$ xác định bởi $q(x, y, \lambda) = \lambda x + (1 - \lambda) y$ là liên tục và, theo định nghĩa của điểm cực biên, $K - M = q(U) = \bigcup_n q(F_n)$; nhưng $F_n$ là compac vì nó đóng trong $K \times K \times I$, do đó $q(F_n)$ là compac và vì thế đóng trong K; vậy tập hợp $U_n = K - q(F_n)$ là mở trong K, và ta có $M = \bigcap_n U_n$.

Trong phần tiếp theo của chứng minh, ta sẽ ký hiệu bởi $u$ một hàm số liên tục và *lồi* trên K, bởi $G \subset E \times \mathbf{R}$ đồ thị của $u$, và bởi S *bao lồi đóng* của G trong $E \times \mathbf{R}$.

#### Bổ đề 1 {#int-iv-s7-lem-1 .statement}

— *Cho $\overline{u}$ là bao dưới của các hàm afin tuyến tính liên tục trên E mà $\geq u$ trên K. Khi đó S là tập hợp các điểm $(a, b) \in E \times \mathbf{R}$ sao cho $a \in K$ và $u(a) \leq b \leq \overline{u}(a)$.*

Theo định lý Hahn-Banach, để $(a, b)$ thuộc S, điều kiện cần và đủ là $h(a, b) \geq 0$ với mọi hàm afin tuyến tính liên tục $h$ trên $E \times \mathbf{R}$ sao cho $h(x, u(x)) \geq 0$ với $x \in K$. Đặt $h(x, t) = f(x) - \lambda t$, trong đó $f$ là một hàm afin tuyến tính liên tục trên E, ta thấy rằng quan hệ $(a, b) \in S$ là tương đương với tính chất sau: quan hệ

$$
f(x) \geq \lambda u(x) \quad \text{với mọi } x \in K
$$

kéo theo

(5)
$$
f(a) \geq \lambda b .
$$

Trước hết đặt $\lambda = 0$; việc (4) kéo theo (5) với mọi hàm afin tuyến tính liên tục $f$ trên $E$ là tương đương với quan hệ $a \in K$ theo định lý Hahn-Banach. Tiếp theo, đặt $\lambda = -1$ và thay $f$ bởi $-f$; khi đó quan hệ $f(x) \leq u(x)$ trong K phải kéo theo $f(a) \leq b$. Nhưng vì $u$ lồi và liên tục trên $K$, nên $u(a)$ bằng cận trên đúng của các $f(a)$ đối với các hàm afin tuyến tính liên tục $f$ trên $E$ sao cho $f(x) \leq u(x)$ trên $K$ (TVS, II, §5, No. 4, Mệnh đề 5); do đó ta thu được quan hệ $b \geq u(a)$. Cuối cùng, đặt $\lambda = 1$; khi đó nói rằng (4) kéo theo (5) có nghĩa, theo định nghĩa, là $b \leq \overline{u}(a)$. Điều này chứng minh bổ đề, vì quan hệ (4) (tương ứng. (5)) là tương đương với quan hệ thu được bằng cách nhân hai vế với một vô hướng $> 0$.

#### Bổ đề 2 {#int-iv-s7-lem-2 .statement}

*Nếu $u$ là chặt lồi trên $K$, thì $u(x) < \overline{u}(x)$ với mọi điểm không cực biên $x$ của $K$.*

Thật vậy, khi đó tồn tại hai điểm phân biệt $y, z$ của $K$ sao cho $x = (y + z)/2$, do đó $u(x) < (u(y) + u(z))/2$ vì $u$ là chặt lồi. Nếu $f$ là một hàm afin tuyến tính trên $E$, thì $f(x) = (f(y) + f(z))/2$; áp dụng quan hệ này cho các hàm afin tuyến tính liên tục $f$ thỏa mãn $f \geq u$ trên $K$, ta được

$$
\overline{u}(x) \geq (\overline{u}(y) + \overline{u}(z))/2 \geq (u(y) + u(z))/2 > u(x) .
$$

Các bổ đề này đã được thiết lập, vì vậy theo đó ta có (Bổ đề 1) $(a, \overline{u}(a)) \in S$ với mọi $a \in K$. Vì $G$ compac, là ảnh của $K$ dưới ánh xạ liên tục $x \mapsto (x, u(x))$, nên theo Mệnh đề 1 của No. 1, tồn tại một độ đo dương $\nu$ trên $G$, có tổng khối lượng bằng 1, nhận $(a, \overline{u}(a))$ làm trọng tâm. Vì hạn chế của phép chiếu $pr_1$ lên $G$ là một đồng phôi từ $G$ lên $K$, độ đo $\nu$ có thể được chuyển tải bằng đồng phôi này, điều đó cho một độ đo $\mu$ trên $K$ (dương và có tổng khối lượng bằng 1) sao cho

(6)
$$
a = \int x \, d\mu(x) \quad \text{và} \quad \overline{u}(a) = \int u(x) \, d\mu(x) .
$$

Quan hệ thứ nhất trong các quan hệ (6) có nghĩa là $a$ là trọng tâm của $\mu$. Hàm $\overline{u}$ là nửa liên tục trên và bị chặn trên $K$, nên khả tích đối với $\mu$ (§4, No. 4, Hệ quả 1 của Mệnh đề 5); hơn nữa, vì hàm $-\overline{u}$ theo định nghĩa là lồi, nên theo Hệ quả của Mệnh đề 2 của No. 1, ta có

(7)
$$
\overline{u}(a) \geq \int \overline{u}(x) \, d\mu(x) ,
$$

do đó, khi so sánh với công thức thứ hai trong các công thức (6),

$$
\int u(\mathbf{x})\, d\mu(\mathbf{x}) \geq \int \overline{u}(\mathbf{x})\, d\mu(\mathbf{x}) .
$$

Nhưng vì $u(\mathbf{x}) \leq \overline{u}(\mathbf{x})$ trên K, quan hệ (8) suy ra rằng $u(\mathbf{x}) = \overline{u}(\mathbf{x})$ hầu khắp nơi đối với $\mu$. Tính đến Bổ đề 2, ta thấy rằng Định lý 1 sẽ được chứng minh một khi bổ đề sau đây được thiết lập:

#### Bổ đề 3 {#int-iv-s7-lem-3 .statement}

*Cho E là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$, và K là một tập con lồi compac khả mêtric của E. Khi đó tồn tại một hàm số thực chặt lồi trên K.*

Vì không gian Banach $\mathcal{C}(K; \mathbf{R})$ là tách được (GT, X, §3, No. 3, Th. 1), nên không gian con $\mathcal{A}$ của $\mathcal{C}(K; \mathbf{R})$ gồm các hạn chế lên K của các *hàm affine tuyến tính liên tục trên* E cũng tách được. Do đó, lấy $(h_n)$ là một dãy trù mật trong $\mathcal{A}$, và lấy $\alpha_n > \sup_{\mathbf{x} \in K} |h_n(\mathbf{x})|$. Khi đó mỗi hàm $h_n^2 / n^2 \alpha_n^2$ đều lồi trên K (TVS, II, §2, No. 8, *Examples*), và chuỗi có số hạng tổng quát $h_n^2 / n^2 \alpha_n^2$ là hội tụ chuẩn, vì vậy tổng $u$ của nó liên tục và lồi trên K. Còn phải thấy rằng $u$ lồi nghiêm ngặt, và để làm điều này chỉ cần chứng minh rằng với mọi hai điểm phân biệt $\mathbf{x}, \mathbf{x}'$ của K, tồn tại một số nguyên $n$ sao cho hạn chế của $h_n^2$ lên đoạn có hai đầu mút $\mathbf{x}, \mathbf{x}'$ là lồi nghiêm ngặt; nhưng để được điều đó thì chỉ cần có $h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$ (*loc. cit.*). Mà tồn tại một hàm $h \in \mathcal{A}$ sao cho $h(\mathbf{x}) \neq h(\mathbf{x}')$ (TVS, II, §4, No. 1, Cor. 1 of Prop. 2) và vì dãy $(h_n)$ trù mật trong $\mathcal{A}$, nên tồn tại một $n$ sao cho $h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$.

Q.E.D.

#### Hệ quả {#int-iv-s7-n2-cor-2 .statement}

*Cho E là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$, C là một nón lồi thực sự trong E có đỉnh 0, đầy đủ và mêtric hóa được đối với cấu trúc đều cảm sinh bởi cấu trúc đều yếu hóa của E. Gọi M là hợp của các đường sinh cực biên của C. Với mọi $\mathbf{x} \in C$ đều tồn tại một tập con lồi compắc K của C và một độ đo $\lambda \geq 0$ trên K có tổng khối lượng bằng 1, sao cho $K - (M \cap K)$ là $\lambda$-không đáng kể và trọng tâm của $\lambda$ bằng $\mathbf{x}$.

Thật vậy, $\mathbf{x}$ thuộc về một thiết diện K của C (TVS, II, §7, No. 2, Prop. 5), và $M \cap K$ chứa tập hợp các điểm cực biên của K (*loc. cit.*, Cor. 1 of Prop. 4). Khi đó chỉ cần áp dụng Th. 1.

### 3. Ứng dụng: I. Các không gian vectơ các hàm thực liên tục

Cho X là một không gian compắc khác rỗng, $\mathcal{H}$ là một không gian con tuyến tính của không gian Banach $\mathcal{C}(X; \mathbf{R})$ chứa các hằng số và *phân biệt* các điểm của X (GT, X, §4, No. 1, Def. 1). Ta trang bị cho $\mathcal{H}$ tôpô không gian định chuẩn cảm sinh bởi tôpô của $C(X; \mathbf{R})$, và ký hiệu bởi $\mathcal{H}'$ đối ngẫu của không gian định chuẩn này. Với mọi $x \in X$, ánh xạ $f \mapsto f(x)$ là một dạng tuyến tính liên tục trên $\mathcal{H}$ (hạn chế lên $\mathcal{H}$ của độ đo Dirac $\varepsilon_x$), do đó là một phần tử của $\mathcal{H}'$ sẽ được ký hiệu là $i_{\mathcal{H}}(x)$, sao cho

$$
\langle f, i_{\mathcal{H}}(x) \rangle = f(x)
$$

với mọi hàm $f \in \mathcal{H}$ và mọi $x \in X$.

Ánh xạ $i_{\mathcal{H}}$ từ X vào $\mathcal{H}'$ là đơn ánh và liên tục khi $\mathcal{H}'$ được trang bị tôpô yếu $\sigma(\mathcal{H}', \mathcal{H})$; mệnh đề thứ hai suy ra ngay từ các định nghĩa và (9); còn về mệnh đề thứ nhất, chú ý rằng nếu $x, x'$ là hai điểm phân biệt của X, thì theo giả thiết tồn tại một hàm $h \in \mathcal{H}$ sao cho $h(x) \neq h(x')$, do đó, theo (9), $\langle h, i_{\mathcal{H}}(x) \rangle \neq \langle h, i_{\mathcal{H}}(x') \rangle$ và *a fortiori* $i_{\mathcal{H}}(x) \neq i_{\mathcal{H}}(x')$. Vì vậy ảnh $i_{\mathcal{H}}(X)$ là một tập con *compắc* của $\mathcal{H}'$ (đối với tôpô yếu), và $i_{\mathcal{H}}$ là một *đồng phôi* từ X lên $i_{\mathcal{H}}(X)$.

#### Mệnh đề 4 {#int-iv-s7-prop-4 .statement}

(i) *Bao lồi đóng* C *của* $i_{\mathcal{H}}(X)$ *trong* $\mathcal{H}'$ *(đối với tôpô yếu* $\sigma(\mathcal{H}', \mathcal{H})$) *là compắc*.

(ii) *Để một điểm* $i_{\mathcal{H}}(x)$ *là một điểm cực biên của* C, *điều kiện cần và đủ là độ đo dương duy nhất* $\lambda$ *trên* X *sao cho*

$$
h(x) = \int h \, d\lambda
$$

*đối với mọi hàm* $h \in \mathcal{H}$ (điều này đặc biệt kéo theo rằng $\lambda$ có khối lượng toàn phần bằng 1, vì $1 \in \mathcal{H}$) *là độ đo Dirac* $\varepsilon_x$.

Suy ra rằng, với mỗi $h \in \mathcal{H}$, hàm $z' \mapsto \langle h, z' \rangle$ trên C đạt tới cận trên đúng của nó tại ít nhất một điểm cực biên của C (TVS, II, §7, No. 1, Mệnh đề 1), và điểm này thuộc $i_{\mathcal{H}}(X)$ (*loc. cit.*, Hệ quả của Mệnh đề 2).

(i) Theo (9), $\| i_{\mathcal{H}}(x) \| \leq 1$ trong không gian định chuẩn $\mathcal{H}'$, nói cách khác $i_{\mathcal{H}}(X)$ bị chặn, và mệnh đề suy ra từ sự kiện rằng $\mathcal{H}'$, được trang bị tôpô yếu $\sigma(\mathcal{H}', \mathcal{H})$, là *gần đầy đủ* (TVS, III, §4, No. 2, Hệ quả 5 của Định lý 1).

(ii) Mọi độ đo dương $\mu$ có khối lượng 1 trên $i_{\mathcal{H}}(X)$ đều thu được, bởi phép chuyển cấu trúc nhờ phép đồng phôi $i_{\mathcal{H}}$, từ một độ đo dương $\lambda$ có khối lượng 1 trên X, còn độ đo Dirac $\varepsilon_{i_{\mathcal{H}}(x)}$ thì thu được từ $\varepsilon_x$. Nói rằng $\mu$ nhận $i_{\mathcal{H}}(x)$ làm trọng tâm có nghĩa, theo định nghĩa, là

$$
\int_X \langle h, i_{\mathcal{H}}(z) \rangle \, d\lambda(z) = \langle h, i_{\mathcal{H}}(x) \rangle
$$

đối với mọi hàm $h \in \mathcal{H}$. Có tính đến (9), mệnh đề (ii) chỉ là bản dịch của tiêu chuẩn trong No. 2, Hệ quả của Mệnh đề 3 để $i_{\mathcal{H}}(x)$ là một điểm cực biên của C.

Ta sẽ nói rằng một điểm $x \in X$ thỏa mãn điều kiện (ii) của Mệnh đề 4 là $\mathcal{H}$-cực biên; ta ký hiệu bởi $\mathrm{Ch}_{\mathcal{H}}(X)$ (hoặc đơn giản là $\mathrm{Ch}(X)$) tập hợp các điểm ấy, và bởi $\check{S}_{\mathcal{H}}(X)$ (hoặc đơn giản là $\check{S}(X)$) bao đóng của $\mathrm{Ch}_{\mathcal{H}}(X)$ trong $X$.

#### Mệnh đề 5 {#int-iv-s7-prop-5 .statement}

*Mọi hàm* $h \in \mathcal{H}$ *đều đạt tới cận trên đúng của nó tại ít nhất một điểm* $\mathcal{H}$*-cực biên*.

Cho $x$ là một điểm của $X$, $h$ là một hàm trong $\mathcal{H}$. Quan hệ $h(z) \leq h(x)$ với mọi $z \in X$ có thể viết thành $\langle h, i_{\mathcal{H}}(z) \rangle \leq \langle h, i_{\mathcal{H}}(x) \rangle$ với mọi $z \in X$, và do đó có nghĩa là siêu phẳng đóng yếu của $\mathcal{H}'$ có phương trình $\langle h, t' \rangle = \langle h, i_{\mathcal{H}}(x) \rangle$ là một *siêu phẳng tựa* của $i_{\mathcal{H}}(X)$. Ta biết rằng (TVS, II, §7, No. 1, Hệ quả của Mệnh đề 1) một siêu phẳng như vậy chứa ít nhất một điểm cực biên của bao lồi đóng của $i_{\mathcal{H}}(X)$, và một điểm như vậy $i_{\mathcal{H}}(y)$ là ảnh của một điểm $\mathcal{H}$-cực biên $y$ theo định nghĩa; do đó $h(y)$ bằng cận trên đúng của $h$ trong $X$.

#### Mệnh đề 6 {#int-iv-s7-prop-6 .statement}

*Với mọi điểm* $x \in X$, *các tính chất sau là tương đương*:

a) $x$ *là* $\mathcal{H}$*-cực biên*.

b) *Với mọi lân cận mở* $U$ *của* $x$ *trong* $X$ *và mọi* $\varepsilon > 0$, *tồn tại một hàm* $h \geq 0$ *trong* $\mathcal{H}$ *sao cho* $h(x) \leq \varepsilon$ *và* $h(y) \geq 1$ *với mọi* $y \in X - U$.

Cho $x$ là một điểm bất kỳ của $X$, $f$ là một hàm trong $\mathcal{C}(X; \mathbf{R})$; đã biết (TVS, II, §3, No. 1, Mệnh đề 1) rằng cận dưới của các số $\lambda(f)$, với mọi độ đo dương trên $X$ sao cho $\lambda(h) = h(x)$ với mọi hàm $h \in \mathcal{H}$, bằng cận trên của các số $h(x)$, khi $h$ chạy trên tập các hàm $h \in \mathcal{H}$ sao cho $h \leq f$. Giả sử rằng $x$ là $\mathcal{H}$-cực biên; khi đó từ Mệnh đề 4, (ii), suy ra rằng với mọi hàm $f \in \mathcal{C}(X; \mathbf{R})$,

$$
f(x) = \sup_{h \in \mathcal{H}, h \leq f} h(x).
$$

Để chứng minh rằng *a)* kéo theo *b)*, ta lấy $f$ là một ánh xạ liên tục từ $X$ vào $[0, 1]$, với giá đỡ được chứa trong $U$, sao cho $f(x) = 1$; khi đó, theo (11), tồn tại một hàm $h' \in \mathcal{H}$ sao cho $h' \leq f$ và $h'(x) \geq 1 - \varepsilon$. Vì $1 \in \mathcal{H}$, hàm $h = 1 - h'$ thỏa mãn các điều kiện của *b)*.

Ngược lại, giả sử điều kiện *b)* được kiểm tra; điều kiện này kéo theo rằng $1 - h \leq \varphi_U$; do đó với mọi độ đo dương $\lambda$ trên $X$ thỏa mãn điều kiện (10), ta có

$$
\lambda(U) = \lambda(\varphi_U) \geq \lambda(1 - h) = 1 - h(x) \geq 1 - \varepsilon.
$$

Vì, theo giả thiết, quan hệ này đúng với mọi $\varepsilon > 0$ và mọi lân cận mở $U$ của $x$, suy ra rằng

$$
\lambda(\{x\}) = \inf_U \lambda(U) \geq 1 - \varepsilon
$$

với mọi $\varepsilon > 0$, do đó $\lambda(\{x\}) = 1$. Vì $\lambda$ là dương và có tổng khối lượng bằng 1, tất yếu $\lambda = \varepsilon_x$, điều này chứng minh rằng $x$ là $\mathcal{H}$-cực biên, theo Mệnh đề 4, (ii).

#### Mệnh đề 7 {#int-iv-s7-prop-7 .statement}

*Cho F là một tập con đóng của X. Các tính chất sau là tương đương:*

a) *F chứa* $\check{S}_{\mathcal{H}}(X)$.

b) *Với mọi hàm* $h \in \mathcal{H}$, *tập* F *giao với tập các điểm của* X *mà tại đó* h *đạt tới cận trên của nó.*

c) *Với mọi điểm* $x \in X$, *tồn tại một độ đo dương* $\mu$ *có tổng khối lượng bằng* 1 *trên* X, *sao cho* $\operatorname{Supp}(\mu) \subset F$ *và* $h(x) = \int h \, d\mu$ *với mọi hàm* $h \in \mathcal{H}$.

Đặt $G = i_{\mathcal{H}}(F)$. Điều kiện *a)* có nghĩa là G chứa tập hợp các điểm cực biên của C. Điều kiện *b)* có nghĩa là G gặp giao của $i_{\mathcal{H}}(X)$ với mỗi siêu phẳng tựa đóng của $i_{\mathcal{H}}(X)$. Sau cùng, điều kiện *c)* có nghĩa là mỗi điểm của $i_{\mathcal{H}}(X)$ là trọng tâm của một độ đo có giá được chứa trong G; theo No. 1, Mệnh đề 1, điều này cũng tương đương với việc nói rằng bao lồi đóng của $i_{\mathcal{H}}(X)$ bằng bao lồi đóng của G. Do đó tính tương đương của các điều kiện *a)*, *b)* và *c)* suy ra từ EVT, II, §7, No. 1, Hệ quả của Mệnh đề 2.

#### Mệnh đề 8 {#int-iv-s7-prop-8 .statement}

*Giả sử X là khả mêtric. Khi đó tập hợp $\operatorname{Ch}_{\mathcal{H}}(X)$ các điểm $\mathcal{H}$-cực biên của X là giao của một họ đếm được các tập mở trong X, và với mọi $x \in X$, tồn tại một độ đo dương $\mu$ có tổng khối lượng 1 trên X sao cho*

$$
\mu(X - \operatorname{Ch}_{\mathcal{H}}(X)) = 0 \quad \text{và} \quad \int h \, d\mu = h(x)
$$

*đối với mọi $h \in \mathcal{H}$.*

Đây là bản dịch của Định lý 1 của No. 2, bởi phép chuyển cấu trúc nhờ phép đồng phôi $x \mapsto i_{\mathcal{H}}(x)$, như trong Mệnh đề 5.

Một số kết quả của Số này có thể được mở rộng khi $\mathcal{H}$ được thay bằng một tập hợp $\mathcal{P}$ các hàm xác định trên X, nhận giá trị trong $\mathbf{R} \cup \{+\infty\}$, nửa liên tục dưới, với giả thiết $\mathcal{P}$ chứa các hằng và thỏa mãn $\mathcal{P} + \mathcal{P} \subset \mathcal{P}$ (Bài tập 2).

#### Ví dụ {#int-iv-s7-n3-exa-1 .statement}

— Lấy X là quả cầu đơn vị $\|x\| \leq 1$ trong $\mathbf{R}^3$, và gọi $\mathcal{H}$ là một không gian vectơ các hàm liên tục trên X, chứa các hạn chế lên X của các hàm afin tuyến tính trên $\mathbf{R}^3$ và thỏa mãn *nguyên lý cực đại*, nghĩa là, với mọi hàm không hằng $h \in \mathcal{H}$, tập hợp các điểm của X tại đó h đạt tới cận trên của nó được chứa trong mặt cầu $S_2$. Khi đó dễ dàng suy ra từ các Mệnh đề 5 và 7 rằng $\operatorname{Ch}_{\mathcal{H}}(X) = \check{S}_{\mathcal{H}}(X) = S_2$. Một ví dụ quan trọng của một không gian vectơ $\mathcal{H}$ thỏa mãn các điều kiện trên là tập hợp các hàm liên tục trên X và *điều hòa* trong quả cầu mở $\|x\| < 1$. Đối với các hàm này, người ta chứng minh rằng độ đo dương $\mu$ có khối lượng 1 sao cho $\operatorname{Supp}(\mu) \subset S_2$ và $h(x) = \int h \, d\mu$ với mọi $h \in \mathcal{H}$ được cho, nếu $\|x\| < 1$, bởi công thức Poisson

$$
d\mu(z) = \frac{1 - \|z\|^2}{\|z - x\|^3} d\sigma(z),
$$

trong đó $\sigma$ là độ đo trên $S_2$ bất biến dưới nhóm trực giao và sao cho $\sigma(S_2) = 1$ (Ch. VII, §3, Bài tập 8).*

### 4. Ứng dụng: II. Các không gian vectơ của các hàm phức liên tục

Cho $X$ là một không gian compact khác rỗng, $\mathcal{H}$ là một không gian con tuyến tính của không gian Banach phức $\mathcal{C}(X; \mathbf{C})$ chứa các hằng và tách các điểm của $X$. Tập hợp các phần thực $\Re(f)$ của các hàm $f \in \mathcal{H}$ là một không gian con tuyến tính $\mathcal{H}_r$ của không gian vectơ thực $\mathcal{C}(X; \mathbf{R})$; với mọi $f \in \mathcal{H}$, tập hợp $\mathcal{H}_r$ cũng chứa $\mathcal{I}(f) = \Re(-if)$; suy ra $\mathcal{H}_r$ tách các điểm của $X$, vì quan hệ $h(x) = h(y)$ với mọi $h \in \mathcal{H}_r$ kéo theo $\Re(f(x)) = \Re(f(y))$ và $\mathcal{I}(f(x)) = \mathcal{I}(f(y))$, và do đó $f(x) = f(y)$ với mọi $f \in \mathcal{H}$. Các điểm $\mathcal{H}_r$-cực biên trong $X$ lại được gọi là $\mathcal{H}$-cực biên, tập hợp các điểm đó được ký hiệu là $\mathrm{Ch}_{\mathcal{H}}(X)$, và bao đóng của tập hợp sau được ký hiệu là $\check{S}_{\mathcal{H}}(X)$. Các tương tự của các Mệnh đề 5 và 7 là như sau:

#### Mệnh đề 9 {#int-iv-s7-prop-9 .statement}

*Với mọi hàm $f \in \mathcal{H}$, $\mathrm{Ch}_{\mathcal{H}}(X)$ giao với tập hợp các điểm mà tại đó $|f|$ đạt tới chặn trên đúng của nó.*

Ta có thể chỉ xét trường hợp $f$ không phải là hằng 0. Lấy $a$ là một điểm của $X$ tại đó $|f|$ đạt tới chặn trên đúng của nó, và đặt $g = f/f(a)$; khi đó $g(a) = 1$ và $|g(x)| \leq 1$ với mọi $x \in X$, do đó

$$
\Re(g(a)) = 1 \quad \text{và} \quad \Re(g(x)) \leq 1 \quad \text{với mọi } x \in X.
$$

Theo Mệnh đề 5 của No. 3 áp dụng cho $\mathcal{H}_r$, tồn tại $b \in \mathrm{Ch}_{\mathcal{H}}(X)$ tại đó $\Re((g(x))$ đạt tới chặn trên đúng 1 của nó, do đó $|g(b)| = 1$ vì $|g(b)| \leq 1$; suy ra $|f(b)| = |(f(a)| \geq |f(x)|$ với mọi $x \in X$.

#### Mệnh đề 10 {#int-iv-s7-prop-10 .statement}

*Cho $F$ là một tập con đóng của $X$. Các tính chất sau là tương đương:
a) $F$ chứa $\check{S}_{\mathcal{H}}(X)$.
b) Với mọi hàm $f \in \mathcal{H}$, $F$ giao với tập hợp các điểm của $X$ tại đó $|f|$ đạt tới cận trên của nó.
c) Với mọi điểm $x \in X$, tồn tại một độ đo dương $\mu$ có khối lượng toàn phần bằng 1 trên $X$ sao cho $\mathrm{Supp}(\mu) \subset F$ và $f(x) = \int f d\mu$ đối với mọi hàm $f \in \mathcal{H}$.
Hãy chứng minh tính tương đương của các điều kiện a) và c): đặt $f = f_1 + i f_2$ với $f_1, f_2$ thuộc $\mathcal{H}_r$; quan hệ $f(x) = \int f d\mu$ tương đương với hai quan hệ $f_1(x) = \int f_1 d\mu$ và $f_2(x) = \int f_2 d\mu$; do đó chỉ cần áp dụng cho $\mathcal{H}_r$ tính tương đương của các điều kiện a) và c) của Mệnh đề 7 của No. 3. Việc a) kéo theo b) suy ra từ Mệnh đề 9. Hãy chỉ ra rằng b) kéo theo a); vấn đề là thấy rằng nếu b) được thỏa mãn, thì, với mọi $h \in \mathcal{H}_r$, F giao với tập hợp các điểm tại đó $h$ đạt tới cận dưới của nó trong X. Điều kiện b) kéo theo rằng F khác rỗng; vì F compắc, tồn tại $a \in F$ sao cho $h(a) \leq h(y)$ với mọi $y \in F$. Lấy $f \in \mathcal{H}$ sao cho $h = \mathcal{R}(f)$; với mọi $\varepsilon > 0$, hàm $g = f - h(a) + \varepsilon$ thuộc $\mathcal{H}$, và
$$
\mathcal{R}(g(y)) = h(y) - h(a) + \varepsilon \geq \varepsilon
$$
với mọi $y \in F$. Gọi $c$ là cận trên của $|g|$ trong X, và đặt $b = c^2 / 2\varepsilon$; với mọi $y \in F$,
$$
|g(y) - b|^2 = |g(y)|^2 - 2b \mathcal{R}((g(y))) + b^2 \leq c^2 - 2b\varepsilon + b^2 = b^2,
$$
nói cách khác, cận trên trong F của hàm $|g - b|$ là $\leq b$. Vì $g - b \in \mathcal{H}$, giả thiết trên F kéo theo rằng $|g - b| \leq b$, do đó
$$
b^2 \geq |g - b|^2 = |g|^2 - 2b \mathcal{R}(g) + b^2
$$
và vì thế $\mathcal{R}(g) \geq |g|^2 / 2b \geq 0$; vì $\mathcal{R}(g) = h - h(a) + \varepsilon$, và $\varepsilon > 0$ là tùy ý, ta có $h \geq h(a)$, và $h(a)$ là cận dưới của $h$ trong X, điều này hoàn tất chứng minh.

#### Nhận xét {#int-iv-s7-n4-rem-1 .statement}

Nếu $f$ là một hàm thực liên tục, một điểm tại đó $|f|$ đạt tới cận trên của nó là một điểm tại đó một trong hai hàm $f, -f$ đạt tới cận trên của nó. Đối với một không gian vectơ $\mathcal{H}$ các hàm thực liên tục thỏa mãn các giả thiết của No. 3, các Mệnh đề 9 và 10 do đó là những hệ quả tầm thường của các Mệnh đề 5 và 7, tương ứng.

### 5. Các ứng dụng: III. Các đại số của các hàm liên tục

#### Bổ đề 4 {#int-iv-s7-lem-4 .statement}

Cho X là một không gian compact, $\mathcal{H}$ là một không gian con tuyến tính đóng của không gian Banach $\mathcal{C}(X; \mathbf{C})$ (tương ứng $\mathcal{C}(X; \mathbf{R})$). Cho a là một điểm của X có một hệ cơ bản đếm được các lân cận; giả sử rằng, với mọi số c và d sao cho $0 < c < d < 1$ và mọi lân cận mở U của a, tồn tại một $f \in \mathcal{H}$ sao cho
$$
|f| \leq 1,\quad |f(a)| \geq d,\quad |f(x)| \leq c \text{ với mọi } x \in X - U.
$$
Khi đó tồn tại một hàm $u \in \mathcal{H}$ sao cho $|u(x)| < |u(a)|$ với mọi $x \neq a$.

Cho $(V_n)$ ($n \geq 1$) là một hệ cơ bản các lân cận của $a$, và cho $\lambda, \mu, \varepsilon$ là các số sao cho
$$
0 < \lambda < 1,\quad 1 < \mu < \mu + \varepsilon \leq 1 + \lambda.
$$
Do đó $0 < \lambda / \mu < 1 / \mu < 1$. Ta sẽ định nghĩa, bằng quy nạp theo $n$ ($n \geq 1$), một dãy giảm $(U_n)$ các lân cận mở của $a$ sao cho $U_n \subset V_n$ với mọi $n$, và một dãy $(h_n)$ các hàm trong $\mathcal{H}$ thỏa mãn các hệ thức
$$
\begin{align*}
(13_n) &\quad |h_n(x)| \leq \mu \quad \text{với mọi } x \in X \\
(14_n) &\quad h_n(a) = 1 \\
(15_n) &\quad |h_n(x)| \leq \lambda \quad \text{với mọi } x \in X - U_n \\
(16_n) &\quad \left| \sum_{j=1}^n \lambda^j h_j(y) \right| < \sum_{j=1}^{n+1} \lambda^j \quad \text{với mọi } y \in X.
\end{align*}
$$

Giả sử $h_m$ và $U_m$ đã được định nghĩa với $1 \leq m < n$, thỏa mãn bốn điều kiện trên (với $n$ được thay bởi $m$); mặt khác, đặt $U_0 = X$.

Hàm $\sum_{j=1}^{n-1} \lambda^j h_j$ (bằng 0 nếu $n = 1$) là liên tục và nhận giá trị $\sum_{j=1}^{n-1} \lambda^j$ tại điểm $a$; do đó tồn tại một lân cận mở $U_n$ của $a$, được chứa trong $U_{n-1} \cap V_n$, sao cho
$$
\left| \sum_{j=1}^{n-1} \lambda^j h_j(y) \right| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n \quad \text{với mọi } y \in U_n.
$$

Theo giả thiết tồn tại một hàm $f \in \mathcal{H}$ sao cho
$$
\begin{align*}
|f(x)| &\leq 1 \quad \text{với mọi } x \in X , \quad |f(a)| \geq 1 / \mu , \\
|f(x)| &\leq \lambda / \mu \quad \text{với } x \in X - U_n .
\end{align*}
$$

Đặt $h_n = f / f(a)$; khi đó các hệ thức $(13_n)$, $(14_n)$ và $(15_n)$ đều đúng; đặt
$$
g = \sum_{j=1}^n \lambda^j h_j = \sum_{j=1}^{n-1} \lambda^j h_j + \lambda^n h_n .
$$

Theo (17) và $(13_n)$, với $y \in U_n$ ta có
$$
|g(y)| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n + \mu \lambda^n \leq \sum_{j=1}^{n+1} \lambda^j ,
$$

vì $\varepsilon + \mu \leq 1 + \lambda$; với $x \in X - U_n$, ta có $|h_p(x)| \leq \lambda$ với $1 \leq p \leq n$, do đó cũng có
$$
|g(x)| \leq \sum_{j=2}^{n+1} \lambda^j < \sum_{j=1}^{n+1} \lambda^j,
$$
điều này hoàn thành chứng minh của $(16_n)$.

Do đó, chuỗi $\sum_{n=1}^{\infty} \lambda^n h_n$ hội tụ chuẩn tắc trong $X$ vì $\lambda < 1$ và $|h_n(x)| \leq \mu$ với mọi $n$ và mọi $x \in X$; gọi $u$ là tổng của nó, khi đó $u$ thuộc $\mathcal{H}$ vì $\mathcal{H}$ đóng. Theo quan hệ $(14_n)$, ta có $u(a) = \sum_{n=1}^{\infty} \lambda^n$; mặt khác nếu $x \neq a$, tồn tại một số nguyên $n$ sao cho $x \notin U_{n+1}$; do đó $|h_{n+k}(x)| \leq \lambda$ với mọi $k \geq 1$ theo quan hệ $(15_n)$; suy ra, dùng $(16_n)$, rằng
$$
|u(x)| \leq \left| \sum_{j=1}^n \lambda^j h_j(x) \right| + \left| \sum_{j=n+1}^{\infty} \lambda^j h_j(x) \right| < \sum_{j=1}^{n+1} \lambda^j + \lambda \sum_{j=n+1}^{\infty} \lambda^j
$$
$$
= \sum_{j=1}^{\infty} \lambda^j = |u(a)|.
$$

#### Định lý 2 (E. Bishop) {#int-iv-s7-thm-2 .statement}

— *Cho $X$ là một không gian compact, $\mathcal{A}$ là một đại số con đóng của đại số Banach phức $\mathcal{C}(X; \mathbf{C})$. Giả sử rằng $\mathcal{A}$ chứa các hằng số và phân biệt các điểm của $X$. Cho $a$ là một điểm của $X$; các điều kiện sau là tương đương:

a) Tồn tại một hàm $f \in \mathcal{A}$ sao cho $|f(x)| < |f(a)|$ với mọi $x \neq a$.

b) Điểm $a$ là $\mathcal{A}$-cực biên và thừa nhận một hệ cơ bản đếm được các lân cận.

a) $\Rightarrow$ b): Cho $f \in \mathcal{A}$ sao cho $|f(a)| > |f(x)|$ với $x \neq a$; theo Mệnh đề 9 của No. 4, $a$ là một điểm $\mathcal{A}$-cực biên. Mặt khác, nếu $U_n$ là tập hợp các $x \in X$ sao cho $|f(x)| > |f(a)| - 1/n$, thì $U_n$ là một lân cận mở của $a$, và giao của các $U_n$ thu về $a$; vì $X$ compact, các $U_n$ tạo thành một hệ cơ bản các lân cận của $a$ (GT, I, §9, No. 1, Định lý 1).

b) $\Rightarrow$ a): Chỉ cần kiểm tra rằng b) kéo theo các giả thiết của Bổ đề 4. Với các ký hiệu của bổ đề đó, đặt $\varepsilon = \log d / \log c$; do đó $0 < \varepsilon < 1$. Vì $a$ là một điểm $\mathcal{A}_r$-cực biên, tồn tại một hàm $g \in \mathcal{A}$ sao cho
$$
\mathcal{R}(g) \geq 0,\quad \mathcal{R}(g(a)) \leq \varepsilon,\quad \mathcal{R}(g(x)) \geq 1 \text{ với } x \in X - U
$$

(No. 3, Mệnh đề 6, b)). Đặt $f = c^g$; vì $f$ là tổng của chuỗi hội tụ chuẩn tắc $\sum_{n=0}^{\infty} (\log c)^n g^n / n!$, ta có $f \in \mathcal{A}$ và

$$
|f| \leq 1,\quad |f(a)| \geq c^{\varepsilon} = d,\quad |f(x)| \leq c \text{ với } x \in X - U.
$$

Q.E.D.

#### Hệ quả {#int-iv-s7-n5-cor-1 .statement}

— *Giả sử thêm rằng $X$ mêtric hóa được. Khi đó các tính chất sau là tương đương*:

a) *$a$ là một điểm cực biên đối với $\mathcal{A}$ của $X$*.

b) *Tồn tại $u \in \mathcal{A}$ sao cho $|u(x)| < |u(a)|$ với mọi $x \neq a$*.

c) *Gọi $\mathfrak{M}$ là tập hợp các tập con $M$ của $X$ sao cho, với mọi hàm $f \in \mathcal{A}$, $|f|$ đạt cận trên đúng của nó trong $X$ tại ít nhất một điểm của $M$. Khi đó $a$ thuộc mọi tập hợp $M \in \mathfrak{M}$*.

d) *Gọi $\mathfrak{N}$ là tập hợp các tập con $N$ của $X$ sao cho, với mọi hàm $f \in \mathcal{A}$, $\mathcal{R}(f)$ đạt cận trên đúng của nó trong $X$ tại ít nhất một điểm của $N$. Khi đó $a$ thuộc mọi tập hợp $N \in \mathfrak{N}$*.

*Nói cách khác*,

$$
\mathrm{Ch}_{\mathcal{A}}(X) = \bigcap_{M \in \mathfrak{M}} M = \bigcap_{N \in \mathfrak{N}} N.
$$

Vì trong một không gian mêtric hóa được, mỗi điểm có một hệ cơ bản đếm được các lân cận, nên tính tương đương của a) và b) suy ra từ Định lý 2. Ta hãy chỉ ra rằng b) kéo theo c): thật vậy, $a$ là điểm duy nhất tại đó $|u|$ đạt cận trên đúng của nó; mặt khác, c) kéo theo a) vì, với mọi $f \in \mathcal{A}$, $\mathrm{Ch}_{\mathcal{A}}(X)$ cắt tập hợp các điểm tại đó $|f|$ đạt cận trên đúng của nó (No. 4, Mệnh đề 9). Cùng một lập luận ấy, dùng Mệnh đề 5 của No. 3, cho thấy rằng d) kéo theo a). Sau hết, để thấy rằng b) kéo theo d), ta có thể tự giới hạn vào trường hợp $X$ không rút gọn thành điểm duy nhất $a$, do đó $u(a) \neq 0$; khi đó hàm $v = u/u(a)$ thuộc $\mathcal{A}$, và ta có $v(a) = 1$ và $|v(x)| < 1$ với $x \neq a$, do đó $\mathcal{R}(v(a)) = 1$ và $\mathcal{R}(v(x)) < 1$ với $x \neq a$. Vì hàm $\mathcal{R}(v)$ chỉ đạt cận trên đúng của nó tại điểm $a$, nên quả thật ta có $a \in N$ với mọi $N \in \mathfrak{N}$.

#### Ví dụ {#int-iv-s7-n5-exa-1 .statement}

— Cho $X_1$ là tập hợp các điểm $(z_1, z_2) \in \mathbf{C}^2$ sao cho $|z_1|^2 + |z_2|^2 \leq 1$ (quả cầu đơn vị trong $\mathbf{R}^4$) và cho $\mathcal{A}_1'$ là tập hợp các hạn chế lên $X_1$ của các hàm chỉnh hình, nhận giá trị trong $\mathbf{C}$, được xác định trong một lân cận của $X_1$ trong $\mathbf{C}^2$ (lân cận tùy thuộc vào hàm đang xét); cho $\mathcal{A}_1$ là bao đóng của $\mathcal{A}_1'$ trong $\mathcal{C}(X_1; \mathbf{C})$, hiển nhiên là một đại số con phức đóng của $\mathcal{C}(X_1; \mathbf{C})$ và phân ly các điểm của $X_1$. Áp dụng 'nguyên lý cực đại' đối với các hàm chỉnh hình cho thấy rằng $\mathrm{Ch}_{\mathcal{A}_1}(X_1)$ là mặt cầu $S_3$.

Trong định nghĩa trước, ta thay thế $X_1$ bằng 'đa đĩa' $X_2$ được xác định bởi các quan hệ $|z_1| \leq 1$ và $|z_2| \leq 1$, điều này cho các đại số con $\mathcal{A}_2'$ và $\mathcal{A}_2$ (bao đóng của $\mathcal{A}_2'$ trong $\mathcal{C}(X_2; \mathbf{C})$. Ở đây, nguyên lý cực đại cho thấy rằng $\mathrm{Ch}_{\mathcal{A}_2}(X_2)$ là 'xuyến' được xác định bởi các quan hệ $|z_1| = 1$ và $|z_2| = 1$.

Từ các kết quả ấy, suy ra rằng không tồn tại một *đẳng cấu giải tích* từ một lân cận mở của $X_1$ lên một lân cận mở của $X_2$ mà *biến đổi* $X_1$ *thành* $X_2$; thật vậy, nếu $v$ là hạn chế lên $X_1$ của một ánh xạ như thế, thì ta sẽ có $\mathcal{A}_2 = v \mathcal{A}_1 v^{-1}$ và do đó $v$ sẽ biến đổi $S_3$ thành một không gian phôi đồng phôi với $T^2$, điều này là vô lý vì $S_3$ là đơn liên còn $T^2$ thì không. Tuy nhiên, ta lưu ý rằng các không gian $X_1$ và $X_2$ là *đồng phôi*, vì cả hai đều là các tập hợp lồi bị chặn trong $\mathbf{R}^4$ có phần trong khác rỗng.*

### 6. Tính duy nhất của các biểu diễn nguyên

Cho E là một không gian Hausdorff lồi địa phương yếu (TVS, II, §6, No. 2), C là một nón lồi nhọn thực sự trong E. Ta biết rằng C là tập hợp các phần tử $\geqslant 0$ của E đối với một quan hệ thứ tự tương thích với cấu trúc không gian vectơ của E. Khi nói rằng C được sắp thứ tự như một dàn, dĩ nhiên điều được hiểu là thứ tự cảm sinh trên C bởi thứ tự của E.

#### Bổ đề 5 {#int-iv-s7-lem-5 .statement}

*Giả sử rằng C là yếu đầy đủ. Cho $\mathcal{A}$ là tập hợp các hạn chế lên C của các dạng tuyến tính liên tục trên E. Cho $(f_\lambda)_{\lambda \in \Lambda}$ là một họ hữu hạn các phần tử của $\mathcal{A}$, và $f = \sup(f_\lambda)$. Với mọi $x \in C$, định nghĩa*

$$
\overline{f}(x) = \sup \left( f(x_1) + f(x_2) + \cdots + f(x_n) \right),
$$

*trong đó supremum được lấy trên tập hợp $S_x$ các dãy $(x_1, x_2, \ldots, x_n)$ gồm các phần tử của C sao cho $x_1 + x_2 + \cdots + x_n = x$. Cho $\mathrm{Card}\, \Lambda = p$. Khi đó tồn tại $(y_1, \ldots, y_p) \in S_x$ sao cho $\overline{f}(x) = f(y_1) + \cdots + f(y_p)$.

Ký hiệu bởi $f_1, f_2, \ldots, f_p$ các phần tử của họ $(f_\lambda)$. Với $k = 1, 2, \ldots, p$, cho $C_k$ là tập hợp các $y \in C$ sao cho

$$
f_1(y) < f(y),\ f_2(y) < f(y),\ \ldots,\ f_{k-1}(y) < f(y),\ f_k(y) = f(y).
$$

Các $C_k$ là các nón lồi rời nhau có hợp là C. Cho $x_1, x_2, \ldots, x_n$ trong C sao cho $x_1 + x_2 + \cdots + x_n = x$. Gọi $y_k$ là tổng của các $x_i$ thuộc $C_k$. Khi đó $y_1 + y_2 + \cdots + y_p = x$. Vì $f$ là afin trên $C_k$, nên $f(y_1) + \cdots + f(y_p) = f(x_1) + \cdots + f(x_n)$. Do đó

$$
f(x) = \sup \left( f(y_1) + \cdots + f(y_p) \right),
$$

trong đó $(y_1, y_2, \ldots, y_p)$ chạy qua tập hợp các dãy gồm $p$ điểm của C sao cho $y_1 + y_2 + \cdots + y_p = x$. Đặt $D = C \cap (x - C)$. Vì D là compắc (TVS, II, §6, No. 8, Hệ quả 2 của Mệnh đề 11), nên tập hợp các phần tử $(y_1, \ldots, y_p)$ của $D^p$ sao cho $y_1 + \cdots + y_p = x$ cũng vậy, do đó cận trên đúng (19) đạt được.

#### Bổ đề 6 {#int-iv-s7-lem-6 .statement}

Ta giữ nguyên các giả thiết và ký hiệu của Bổ đề 5, và giả sử các $f_\lambda$ là dương. Hàm $\overline{f}$ là thuần nhất dương, lõm và nửa liên tục trên trong C. Nó là afin nếu $C$ có thứ tự dàn.

Rõ ràng $\overline{f}$ là thuần nhất dương. Cho $x, y$ thuộc $C$. Nếu $x_1, \ldots, x_m, y_1, \ldots, y_n$ trong $C$ sao cho $x_1 + \cdots + x_m = x,\ y_1 + \cdots + y_n = y$, thì $x_1 + \cdots + x_m + y_1 + \cdots + y_n = x + y$, do đó

$$
f(x_1) + \cdots + f(x_m) + f(y_1) + \cdots + f(y_n) \leq \overline{f}(x + y);
$$

suy ra $\overline{f}(x) + \overline{f}(y) \leq \overline{f}(x + y)$, do đó $\overline{f}$ là lõm. Gọi $L$ (resp. $L_\lambda$) là tập hợp các $(t, x) \in \mathbf{R} \times E$ sao cho $x \in C$ và $0 \leq t \leq \overline{f}(x)$ (resp. $0 \leq t \leq f_\lambda(x)$). Mỗi $L_\lambda$ đều đóng trong nón lồi thực sự đầy đủ yếu $\mathbf{R}_+ \times C$, do đó tổng $\sum_{\lambda \in \Lambda} L_\lambda$ là đóng (TVS, II, §6, No. 8, Hệ quả 2 của Mệnh đề 11). Theo Bổ đề 5, tổng này bằng $L$. Vậy $L$ đóng, điều này chứng minh rằng $\overline{f}$ là nửa liên tục trên. Sau cùng, giả sử $C$ có thứ tự dàn, và ta sẽ chứng minh rằng $\overline{f}$ là lồi. Cho $x, y$ thuộc $C$ và cho $\varepsilon > 0$. Tồn tại $z_1, z_2, \ldots, z_n$ trong $C$ sao cho $f(z_1) + \cdots + f(z_n) \geq \overline{f}(x + y) - \varepsilon$ và $z_1 + \cdots + z_n = x + y$. Không gian vectơ $C - C$ có thứ tự dàn đối với thứ tự cảm sinh bởi thứ tự của $E$ (A, VI, §1, No. 9, Mệnh đề 8). Theo định lý phân tích (*loc. cit.*, No. 10, Định lý 1), tồn tại $x_1, \ldots, x_n, y_1, \ldots, y_n$ trong $C$ sao cho

$$
x_1 + y_1 = z_1,\ \ldots,\ x_n + y_n = z_n,\ x_1 + \cdots + x_n = x,\ y_1 + \cdots + y_n = y.
$$

Khi đó, vì $f$ là thuần nhất dương và lồi,

$$
\begin{align*}
\overline{f}(x + y) &\leq \varepsilon + f(z_1) + \cdots + f(z_n) \\
&\leq \varepsilon + f(x_1) + f(y_1) + \cdots + f(x_n) + f(y_n) \\
&\leq \varepsilon + \overline{f}(x) + \overline{f}(y).
\end{align*}
$$

Vì $\varepsilon$ là một số tùy ý $> 0$, ta đã chứng minh rằng $\overline{f}$ quả thật là lồi.

#### Định lý 3 (Choquet) {#int-iv-s7-thm-3 .statement}

*Cho $E$ là một không gian lồi địa phương yếu Hausdorff, $C$ là một nón lồi thực sự đầy đủ yếu có đỉnh 0 trong $E$, $G$ là hợp của các đường sinh cực biên của $C$, $K$ là một tập con lồi compắc của $C$, $\lambda$ và $\lambda'$ là các độ đo dương có khối lượng 1 trên $K$, có cùng trọng tâm, sao cho $\lambda^*(K - (K \cap G)) = {\lambda'}^*(K - (K \cap G)) = 0$. Giả sử rằng $C$ có thứ tự dàn. Khi đó, với mọi hàm lồi nửa liên tục dưới, thuần nhất dương $f \geq 0$ trên $C$, ta có $\lambda^*(f|K) = {\lambda'}^*(f|K)$.*

Gọi $\mathcal{A}$ (tương ứng $\mathcal{A}'$) là tập các hạn chế lên $C$ của các dạng tuyến tính liên tục (tương ứng các hàm afin) trên $E$. Ta biết (TVS, II, §5, No. 4, Nhận xét 2) rằng $f$ là bao trên của tập các phần tử của $\mathcal{A}$ mà $\leq f$. Tập các hàm có dạng $\sup(f_1, \ldots, f_p)$, trong đó $f_1, \ldots, f_p$ thuộc $\mathcal{A}$, $f_1 \geq 0, \ldots, f_p \geq 0$, là một tập có hướng tăng và có $f$ làm bao trên. Có tính đến §1, No. 1, Định lý 1, chỉ cần kiểm tra đẳng thức $\lambda(f|K) = \lambda'(f|K)$ khi $f$ có dạng nói trên.

Định nghĩa $\overline{f}$ như trong Bổ đề 5. Hiển nhiên là $\overline{f}(y) = f(y)$ nếu $y \in G$. Vì $\lambda^*(K - (K \cap G)) = 0$, ta có $\lambda(f|K) = \lambda(\overline{f}|K)$. Theo Bổ đề 6, $\overline{f}$ là afin và nửa liên tục trên. Do đó $\overline{f}|K$ là bao dưới của một tập có hướng giảm gồm các hạn chế lên K của các phần tử của $\mathcal{A}'$ (TVS, II, §5, No. 4, Mệnh đề 6). Gọi $x \in K$ là trọng tâm của $\lambda$. Nếu $g \in \mathcal{A}$ thì $\lambda(g|K) = g(x)$. Do đó $\lambda(\overline{f}|K) = \overline{f}(x)$ (§ 4, No. 4, Hệ quả 2 của Mệnh đề 5). Vậy $\lambda(f|K) = \overline{f}(x)$, và cũng thấy tương tự rằng $\lambda'(f|K) = \overline{f}(x)$.

#### Hệ quả {#int-iv-s7-n6-cor-1 .statement}

*Cho E là một không gian lồi địa phương Hausdorff, C là một nón lồi thực sự có đỉnh 0 trong E, thừa nhận một đáy compắc M, và gọi G là hợp của các đường sinh cực biên của C. Cho $x \in M$. Nếu C có thứ tự dàn, thì tồn tại nhiều nhất một độ đo dương $\lambda$ có khối lượng 1 trên M, sao cho $\lambda^*(M - (G \cap M)) = 0$, và có x làm trọng tâm.*

Thay thế tôpô của E bởi tôpô làm yếu đi (điều này không thay đổi tôpô của M), ta có thể giả sử E là một không gian yếu. Gọi $\lambda$ và $\lambda'$ là hai độ đo trên M có các tính chất đã nêu, và gọi h là một dạng tuyến tính liên tục trên E sao cho M là giao của C và siêu phẳng có phương trình $h(x) = 1$. Gọi $\mathcal{S}$ là tập con của $\mathcal{C}(M)$ gồm các hạn chế lên M của các hàm lồi thuần nhất dương và liên tục $\geq 0$ trên C. Nón C là đầy đủ yếu (TVS, II, §7, No. 3). Theo Định lý 3, $\lambda(f) = \lambda'(f)$ với mọi $f \in \mathcal{S}$.

Nếu $f_1, f_2, f_3, f_4$ thuộc $\mathcal{S}$, thì
$$
\begin{align*}
\sup(f_1 - f_2, f_3 - f_4) &= \sup(f_1 + f_4, f_3 + f_2) - (f_2 + f_4) \in \mathcal{S} - \mathcal{S} \\
\inf(f_1 - f_2, f_3 - f_4) &= -\sup(f_2 - f_1, f_4 - f_3) \in \mathcal{S} - \mathcal{S}.
\end{align*}
$$
Vì $h|M \in \mathcal{S}$, $\mathcal{S} - \mathcal{S}$ chứa các hàm hằng. Nếu x và y là hai điểm phân biệt của M, thì tồn tại một dạng tuyến tính liên tục trên E tách x và y, và dạng này là hiệu của hai dạng tuyến tính liên tục dương trên C (TVS, II, §6, No. 8, Bổ đề 1). Suy ra từ điều vừa nói rằng với $\alpha, \beta$ thực, tồn tại $f \in \mathcal{S} - \mathcal{S}$ sao cho $f(x) = \alpha, f(y) = \beta$. Khi đó $\mathcal{S} - \mathcal{S}$ trù mật trong $\mathcal{C}(M)$ đối với tôpô hội tụ đều (GT, X, §4, No. 1, Hệ quả của Mệnh đề 2). Vì $\lambda$ và $\lambda'$ trùng nhau trên $\mathcal{S} - \mathcal{S}$, ta có $\lambda = \lambda'$.

Bài tập

### Bài tập {#int-iv-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
