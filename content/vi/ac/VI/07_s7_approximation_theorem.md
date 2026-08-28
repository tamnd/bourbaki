---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 7
section_title: Approximation theorem
lang: vi
source: ac-i-vii
book_pages: 412-416, 460-461
pdf_pages: 0430-0434, 0478-0479
extraction: ocr
subsections:
    - "no": 1
      title: THE INTERSECTION OF A FINITE NUMBER OF VALUATION RINGS
      page: 412
      pdf_page: 430
    - "no": 2
      title: INDEPENDENT VALUATIONS
      page: 413
      pdf_page: 431
    - "no": 3
      title: THE CASE OF ABSOLUTE VALUES
      page: 415
      pdf_page: 433
statements: 14
exercises: 3
content_sha256: 279e102ebb4a2d104a52c1c46d18e586ec79f0699267b5a403e59b7de404a09d
translated_from: content/en/ac/VI/07_s7_approximation_theorem.md
source_content_sha256: a818113ef87fdb588b60c8045863641963170d0c573c7e9237ce829f4055a323
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-aac554e0
glossary_version: 34
glossary_terms_sha256: 65303e5c84f0ec7867229420ffa711f7a916e0b4187c5ba1cf6c5018b84e9d82
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. ĐỊNH LÝ XẤP XỈ

### 1. GIAO CỦA MỘT SỐ HỮU HẠN CÁC VÀNH ĐỊNH GIÁ

#### Mệnh đề 1 {#ac-vi-s7-prop-1 .statement}

Cho $K$ là một trường, $(\mathbf{A}_i)_{1 \leq i \leq n}$ là một họ hữu hạn các vành định giá của $K$ và $B = \bigcap_{i=1}^n \mathbf{A}_i$. Ta viết $p_i = B \cap m(\mathbf{A}_i)$. Khi đó $A_i = B_{p_i}$ với mọi $i$ và trường phân thức của $B$ là $K$.

Rõ ràng $B_{p_i} \subset A_i$. Để chứng minh bao hàm đảo lại, ta cần bổ đề sau:

#### Bổ đề 1 {#ac-vi-s7-lem-1 .statement}

Cho $v_i$ ($1 \leq i \leq n$) là các định giá trên trường $K$ và $x \in K^*$. Khi đó tồn tại một đa thứcf $(X)$ có dạng

$$
f(X) = 1 + n_1 X + \cdots + n_{k-1} X^{k-1} + X^k \quad (k \geq 2,\ n_j \in \mathbf{Z} \text{ với } 1 \leq j \leq k - 1)
$$

sao cho $f(x) \neq 0$ và phần tử $z = f(x)^{-1}$ có các tính chất sau đâyvới $1 \leq i \leq n$:

$$
v_i(z) = 0 \qquad \text{nếu} \quad v_i(x) \geq 0 \\
v_i(z) + v_i(x) > 0 \qquad \text{nếu} \quad v_i(x) < 0.
$$

Giả sử bổ đề này trong chốc lát, ta chỉ ra cách nó suy ra rằng $A_1 \subset B_{p_1}$. Cho $x$ là một phần tử khác không của $A_i$. Ta áp dụng bổ đề cho $x$ và các định giá $v_i$ liên kết với các $\mathbf{A}_i$. Khi đó $v_i(z) \geq 0$ và $v_i(zx) \geq 0$ với mọi $i$, do đó $z \in B$ và $zx \in B$. Vì $v_1(x) \geq 0$, $v_1(z) = 0$ và do đó $z \notin p_1$. Vậy $x = zx/z \in B_{p_1}$. Trường phân thức của $B$ khi đó chứa $A_1$ và do đó là $K$.

Bây giờ ta chuyển sang chứng minh bổ đề. Gọi $I$ là tập hợp các chỉ số $i$ sao cho $v_i(x) \geq 0$. Với mọi $i \in I$, gọi $\bar{x}_i$ là ảnh chính tắc của $x$ trong $\kappa(\mathbf{A}_i)$. Với mọi $i \in I$ ta xây dựng một đa thứcf như sau: nếu tồn tại một đa thức $g(X)$ có dạng (1) sao cho $g(\bar{x}_i) = 0$ trong $\kappa(\mathbf{A}_i)$, ta lấyf là một đa thức như vậy; nếu không ta lấy $f_i = 1$. Khi đó ta viết $f(X) = 1 + X^2 \prod_{i \in I} f_i(X)$. Hiển nhiên đó là một đa thức có dạng (1). Nếu $i \in I$, thì $f(x) \in A_i$ và cũng $(\bar{x}_i) \neq 0$ theo phép dựng; do đó $f(x) \notin m(\mathbf{A}_i)$, $v_i(f(x)) = 0$ và $v(z) = 0$. Nếu $i \notin I$, thì $v_i(x) < 0$, do đó $v_i(f(x)) = kv_i(x)$ (§ 3, no. 1, Mệnh đề 1) và

$$
v_i(x) + v_i(z) = (1 - k)v_i(x) > 0
$$

(vì $k \geq 2$). Do đó bổ đề.

#### Mệnh đề 2 {#ac-vi-s7-prop-2 .statement}

Với các giả thiết của Mệnh đề 1, giả sử thêm rằng $\mathbf{A}_i \not\subset \mathbf{A}_j$ với $i \neq j$. Khi đó các $p_i$ là các iđêan cực đại phân biệt của $B$ và mọi iđêan cực đại của $B$ đều bằng một trong các $p_i$.

Nếu $p_i \subset p_j$ với $i \neq j$, thì $\mathbf{A}_i = B_{p_i} \supset B_{p_j} = \mathbf{A}_j$. Khi đó chỉ cần áp dụng Chương II, § 3, no. 5, Hệ quả của Mệnh đề 17.

#### Hệ quả 1 {#ac-vi-s7-prop-2-cor-1 .statement}

Giả sử rằng $A_i \not\subset A_j$ với $i \neq j$. Với mọi họ các phần tử $a_i \in A_i$ ($1 \leq i \leq n$), tồn tại $x \in B$ sao cho $x \equiv a_i \pmod{m(A_i)}$ với $1 \leq i \leq n$.

Vì các $p_i$ là các iđêan cực đại của $B$, $A_i/m(A_i) = B_{p_i}/p_iB_{p_i} = B/p_i$ và do đó có thể giả sử rằng $a_i \in B$ với mọi $i$. Hệ quả suy ra từ sự kiện rằng ánh xạ chính tắc từ $B$ đến $\prod_{i=1}^n (B/p_i)$ là toàn ánh (Chương 11, § 1, no. 2, Mệnh đề 5).

#### Hệ quả 2 {#ac-vi-s7-prop-2-cor-2 .statement}

Giả sử rằng $A_i \not\subset A_j$ với $i \neq j$. Tồn tại các phần tử $x_i$ ($1 \leq i \leq n$) của $K$ sao cho $v_i(x_i) = 0$ và $v_j(x_i) > 0$ với $i \neq j$.

Với mỗi chỉ số $i$ áp dụng Hệ quả 1 cho họ $(a_i)$ sao cho $a_i = 1$ và $a_j = 0$ với $j \neq i$.

#### Hệ quả 3 {#ac-vi-s7-prop-2-cor-3 .statement}

Mọi vành định giá của $K$ chứa $B$ đều chứa một trong các $A_i$.

Ta có thể giới hạn sự chú ý vào trường hợp $A_i \not\subset A_j$ với $i \# j$. Gọi $V$ là một vành định giá của $K$ chứa $B$. Ta viết
$$
p = m(V) \cap B.
$$
Tồn tại một iđêan cực đại $p_i$ của $B$ chứa $p$, do đó
$$
A_i = B_{p_i} \subset B, \subset V.
$$

### 2. CÁC ĐỊNH GIÁ ĐỘC LẬP

#### Định nghĩa 1 {#ac-vi-s7-def-1 .statement}

Cho $A$ và $A'$ là hai vành định giá của cùng một trường $K$. $A$ và $A'$ được gọi là độc lập nếu $K$ là vành sinh bởi $A$ và $A'$. Hai định giá trên $K$ được gọi là độc lập nếu các vành của chúng độc lập và phụ thuộc trong trường hợp ngược lại.

Một định giá không đúng trên $K$ độc lập với mọi định giá trên $K$. Để hai định giá có cấp 1 trên $K$ độc lập, điều kiện cần và đủ là chúng không tương đương (§ 4, no. 5, Mệnh đề 6 (c)).

#### Định lý 1 (Định lý xấp xỉ cho các định giá) {#ac-vi-s7-thm-1 .statement}

Cho $v_i$ ($1 \leq i \leq n$) là các định giá trên một trường $K$ độc lập từng đôi một và $\Gamma_i$ là nhóm cấp của $v_i$. Cho $a_i \in K$ và $\alpha_i \in \Gamma_i$ ($1 \leq i \leq n$). Khi đó tồn tại $x \in K$ sao cho $v_i(x - a_i) \geq \alpha_i$ với mọi $i$

Nếu $v_i$ không đúng, thì $a_i = 0$ và quan hệ $v_i(x - a_i) \geq a_i$ đúng với mọi $x \in K$. Do đó ta có thể giả sử rằng các $v_i$ không không đúng.

Gọi $A_i$ là vành của $v_i$, $B = \bigcap_{i=1}^n A_i$ và $p_i = m(A_i) \cap B$. Theo Mệnh đề 1 của no. 1, các $a_i$ có thể được viết $a_i = b_i/s$ ($b_i \in B, s \in B - \{0\}$); nếu ta viết $x = y/s$ và $\alpha_i' = \alpha_i + v_i(s)$, thì $v_i(y - 6_i) \geq \alpha_i'$. Điều này chỉ ra rằng ta có thể giả sử $a_i \in B$ với mọi $i$; ta cũng có thể giả sử rằng $\alpha_i > 0$ với mọi $i$. Gọi $v_i$ là tập hợp các z \in \mathbf{K} \text{ sao cho } v_i(z) \geq a, \text{ ta viết } q_i = v_i \cap B. \text{ Với } x \in B, v_i(x - a_i) \geq \alpha_i \text{ tương đương với } x \equiv a_i (\mathfrak{q}_i). \text{ Do đó ta cần chứng minh rằng đồng cấu chính tắc } B \to \prod_{i=1}^n (B/q_i) \text{ là toàn ánh, nghĩa là } q_i + q_j = B \text{ với } i \neq j \text{ (Chương 11, § 1, no. 2, Mệnh đề 5). Vì các iđêan cực đại của B là các } \mathfrak{p}_i \text{ (Mệnh đề 2), điều này sẽ đủ để chỉ ra rằng } q_i \notin \mathfrak{p}_j \text{ với } i \neq j.

Giả sử tồn tại $i, j$ sao cho $q_i \subset \mathfrak{p}_j$ và $i \neq j$. Ta sẽ sớm thấy rằng căn của $q_i$ là một iđêan *nguyên tố* $p$ của B. Khi đó $p \subset \mathfrak{p}_j$ và cũng $p \subset \mathfrak{p}_i$ vì $\alpha_i > 0$ và do đó $q_i \subset \mathfrak{p}_i$. Vì vậy $A_1 = B_s \subset B_p$ (no. 1, Mệnh đề 1) và tương tự $A_1 \subset B_r$. Bây giờ, vì $v_i \neq (0)$ và $v_i = B_{\mathfrak{p}_i} q_i$ (Chương 11, § 2, no. 4, Mệnh đề 10), $q_i \neq (0)$, do đó $p \neq (0)$ và $B_r \neq K$. Điều này mâu thuẫn với giả thiết rằng $A_1$ và $A_1$ độc lập.

Còn lại là chứng minh rằng $p$ là nguyên tố. Điều này suy ra từ bổ đề sau:

#### Bổ đề 2 {#ac-vi-s7-lem-2 .statement}

*Cho A là một vành định giá và b là một iđêan của A phân biệt với A. Khi đó căn c của b là một iđêan nguyên tố.*

Giả sử rằng $xy \in c$. Khi đó tồn tại $n \geq 1$ sao cho $(xy)^n \in b$. Gọi $v$ là một định giá liên kết với A. Nếu, ví dụ, $v(x) \geq v(y)$, thì

$$
v(x^{2n}) \geq v(x^n y^n),
$$

do đó $x^{2n} \in b$ và $x \in c$.

#### Hệ quả 1 {#ac-vi-s7-lem-2-cor-1 .statement}

*Với mọi họ các phần tử $\gamma_i \in \Gamma_i$ ($1 \leq i \leq n$), tồn tại $x \in K$ sao cho $v_i(x) = \gamma_i$ ($1 \leq i \leq n$).

Ta có thể giả sử rằng $A_i \neq K$ với mọi $i$. Khi đó, với mọi $i$, tồn tại một $a_i \in K$ sao cho $v_i(a_i) = \gamma_i$ và một $a_r \in \Gamma_r$ sao cho $\gamma_i < a_r$. Ta áp dụng Định lý 1 cho các phần tử $a_i$ này: tồn tại $x \in K$ sao cho $v_i(x - a_i) > v_i(a_i)$; do đó, vì $x = a_i + (x - a_i)$, $v_i(x) = v_i(a_i) = \gamma_i$ ($§ 3$, no. 1, Mệnh đề 1).

#### Hệ quả 2 {#ac-vi-s7-lem-2-cor-2 .statement}

*Gọi $\mathcal{T}_i$ là tôpô được định nghĩa trên $K$ bởi $v_i$; trang bị cho $K^n$ tôpô tích của các $\mathcal{T}_i$. Nếu các $v_i$ không suy biến, đường chéo của $K^n$ là trù mật trong $K^n$.

#### Mệnh đề 3 {#ac-vi-s7-prop-3 .statement}

*Cho $v$ và $v'$ là hai định giá không suy biến trên cùng một trường $K$. Để $v$ và $v'$ định nghĩa cùng một tôpô trên $K$, điều kiện cần và đủ là chúng phụ thuộc.

Giả sử rằng các tôpô $\mathcal{T}_v$ và $\mathcal{T}_{v'}$, được định nghĩa bởi $v$ và $v'$, là đồng nhất. Vì $\mathcal{T}_v$ là Hausdorff, đường chéo của $K^2$ là đóng và do đó $v$ và $v'$ phụ thuộc (Hệ quả 2 của Định lý 1).

Ngược lại, giả sử rằng $v$ và $v'$ phụ thuộc. Khi đó các vành $A$ và $A'$ của chúng được chứa trong cùng một vành $A''$ phân biệt với $K$ và $A''$ là vành của một định giá $v''$ ($§ 4$, no. 1, Mệnh đề 1). Chỉ cần chứng minh rằng tôpô $\mathcal{T}_{v''}$ đồng nhất với $\mathcal{T}_v$. Gọi $\Gamma$ và $\Gamma''$ là các nhóm cấp của $v$ và $v''$. Có một đồng cấu tăng $\lambda$ từ $\Gamma$ lên $\Gamma''$ sao cho $v'' = A \circ v$ ($§ 4$, no. 3). Nếu $a'' \in I?''$, lấy $a \in \lambda^{-1}(a'')$; điều kiện $v(x) \geq \alpha$ suy ra $v''(x) \geq a''$. Lấy $\beta \in \Gamma$ và $\beta'' = \lambda(\beta)$; điều kiện $v(x) \leq \beta$ suy ra $v''(x) \leq \beta''$ và do đó điều kiện $v''(x) > \beta''$ suy ra $v(x) > \beta$. Vì $v$ và $v''$ không bất chính, các bất đẳng thức đang xét xác định các hệ cơ bản các lân cận của 0 đối với $\mathcal{T}_v$ và $\mathcal{T}_{v''}$. Do đó $\mathcal{T}_v = \mathcal{T}_{v''}$, điều này hoàn tất chứng minh.

Nhận xét
(1) Mệnh đề 3 cho thấy quan hệ '"$v$ và $v'$ phụ thuộc"' là một quan hệ tương đương.
(2) Xét đến các quan hệ giữa các định giá cấp 1 và các giá trị tuyệt đối siêu mêtric ($§ 6$, no. 2), Mệnh đề 3 cũng suy ra, trong trường hợp các định giá cấp 1, từ đặc trưng hóa các giá trị tuyệt đối tương đương (General Topology, Chương IX, $§ 3$, no. 2, Mệnh đề 5).

#### Mệnh đề 4 {#ac-vi-s7-prop-4 .statement}

*Cho $v_1, \ldots, v_n$ ($n \geq 2$) là các định giá từng đôi một phụ thuộc trên cùng một trường $K$. Khi đó các vành $A,, \ldots, A,$ của $v_1, \ldots, v,$ sinh ra một vành con $\delta \ K$ phân biệt với $K$.*

Với $n = 2$, Mệnh đề 4 suy ra từ Định nghĩa 1. Giả sử mệnh đề đúng đối với $n - 1$ định giá. Khi đó tồn tại một vành con A của K phân biệt với K và chứa $A,, \ldots, A,$; cũng tồn tại một vành con B $\neq K$ chứa A, _, và A_. Vì A và B chứa A, _, nên chúng so sánh được theo quan hệ bao hàm ($§ 4$, no. 1, Hệ quả của Mệnh đề 1). Do đó, vành lớn hơn trong hai vành này chứa tất cả các $A_i$.

### 3. TRƯỜNG HỢP CÁC GIÁ TRỊ TUYỆT ĐỐI

#### Định lý 2 (Định lý xấp xỉ đối với các giá trị tuyệt đối) {#ac-vi-s7-thm-2 .statement}

*Cho $f_i$ ($1 \leq i \leq n$) là các giá trị tuyệt đối trên cùng một trường $K$ không bất chính và không có hai giá trị nào tương đương. Cho $a, \ (1 \leq i \leq n)$ là các phần tử của $K$ và $\varepsilon$ là một số thực $> 0$. Khi đó tồn tại $x \in K$ sao cho $f_i(x - a,) \leq \varepsilon$ với mọi $i$.*

Cho $K_i$ là trường K với tôpô được xác định bởi $f_i$. Kết quả cần chứng minh tương đương với điều sau: trong tích $P = K_1 \times \cdots \times K_n$, bao đóng $\overline{D}$ của đường chéo D bằng P. Điều này là hiển nhiên đối với $n = 1$. Giả sử điểm này đã được thiết lập trong trường hợp có k giá trị tuyệt đối với $k < n$.

Trước hết ta chứng minh rằng tồn tại, với $2 \leq h \leq n$, một phần tử $x_h$ của K sao cho $f_1(x_h) < 1, f_2(x_h) > 1$ và $f_i(x_h) \neq 1$ với $3 \leq i \leq h$. Ta lập luận bằng quy nạp theo $h$. Nếu $h = 2$, điều này suy ra từ sự kiện rằng $f_1$ và $f_2$ không tương đương. Do đó ta giả sử sự tồn tại của $x_{h-1}$ đã được chứng minh và chứng minh sự tồn tại của $x_h$. Nếu $f_h(x_{h-1}) \neq 1$, ta có thể lấy $x_h = x_{h-1}$; nếu $f_h(x_{h-1}) = 1$, ta chọn $z \in K^*$ sao cho $f_h(z) \neq 1$ và $x_h = z(x_{h-1})^s$ giải quyết bài toán với s đủ lớn. Như vậy ta đã chứng minh sự tồn tại của $x_h$.

Khi số nguyên $q$ tiến tới vô hạn, $f_1(x_n^q)$ tiến tới 0, $f_2(x_n^q)$ tiến tới $+\infty$ và $f_i(x_n^q)$ tiến tới 0 hoặc $+\infty$ với $i \geq 3$. Viết $y_q = x_n^q(1 + x_n^q)^{-1}$,
$$
1 - y_q = (1 + x_n^q)^{-1};
$$
do đó dãy $(y,)$ tiến tới 0 trong $K_1$, tới 1 trong $K_2$ và tới 0 hoặc 1 trong $K_i$ với $i \geq 3$. Bằng cách thay đổi cách đánh số các $K_i$, ta có thể giả sử rằng tồn tại một số nguyên $r$ ($1 \leq r < n$) sao cho $\overline{D}$ chứa điểm $(e_1, \ldots, e_n)$ trong đó $e_i = 1$ với $1 \leq i \leq r$ và $e_i = 0$ với $r + 1 \leq i \leq n$. Bây giờ, $\overline{D}$ là một không gian con K-vectơ của P. Do đó $\overline{D}$ chứa các đường chéo D' và D'' của
$$
P' = K_1 \times \cdots \times K_r,
$$
và $P'' = K_{r+1} \times \cdots \times K_n$. Theo giả thiết quy nạp, $P' = \overline{D}'$ và $P'' = \overline{D}''$. Suy ra $\overline{D} = P$.

### Bài tập {#ac-vi-s7-exercises}

Xem các [bài tập cho § 7](exercises/s7/).
