---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 0
section_title: Fixed points of groups of affine transformations
appendix: true
lang: vi
source: evt-i-v
pdf_pages: 0221-0229, 0254-0258
extraction: ocr
subsections:
    - "no": 1
      title: The case of solvable groups
      page: 0
      pdf_page: 221
    - "no": 2
      title: Invariant means
      page: 40
      pdf_page: 222
    - "no": 3
      title: Ryll-Nardzewski theorem
      page: 41
      pdf_page: 223
    - "no": 4
      title: Applications.
      page: 44
      pdf_page: 226
statements: 10
exercises: 8
content_sha256: 1fd5178bfb1840afca3e3770877d5e89b8a4a9d1d2fd8073e7d65135d1cae7e5
translated_from: content/en/evt/IV/A_a_fixed_points_of_groups_of_affine.md
source_content_sha256: 7eb54e9666dc4f954bc5363b6489301c8e109bec69185ed8316bea9f05a72696
translation_model: gpt-5.4
translation_run: translate-vi-1f4f356d
glossary_version: 34
glossary_terms_sha256: 3c4075eb432e512c0b0cfbb9d810b8d6d6af15062866ff60ad10b689f025d145
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC
# Điểm bất động của các nhóm các phép biến đổi afin

### 1. Trường hợp các nhóm giải được

Cho E là một không gian vectơ thực, và K là một tập con lồi của E. Một ánh xạ $u : K \to K$ sao cho với $x, y$ thuộc K và với mọi số thực $t$ thuộc $[0, 1]$, ta có

$$
u(t x + (1 - t) y) = t u(x) + (1 - t) u(y)
$$

được gọi là một phép biến đổi afin. Từ quan hệ (1) suy ra rằng

$$
u \left( \sum_{i \in I} t_i x_i \right) = \sum_{i \in I} t_i u(x_i)
$$

đối với mọi tập hữu hạn I, các điểm $x_i$ thuộc K và các số thực dương $t_i$ sao cho $\sum_{i \in I} t_i = 1$.

Cho $u$ và $v$ là hai phép biến đổi afin trên K, khi đó ánh xạ $u \circ v$ là một phép biến đổi afin trên K. Nếu $v : E \to E$ là một ánh xạ tuyến tính sao cho $v(K) \subset K$, thì ánh xạ $u : K \to K$ trùng với $v$ trên K là một phép biến đổi afin.

#### Định lý 1 (Markoff-Kakutani) {#evt-iv-a0-thm-1 .statement}

— *Cho E là một không gian vectơ lồi địa phương Hausdorff trên trường $\mathbf{R}$, và K là một tập con lồi compáct không rỗng của E. Cho $\Gamma$ là một tập hợp các phép biến đổi afin liên tục trên K, từng đôi một giao hoán. Khi đó tồn tại một điểm a trong K sao cho $u(a) = a$ với mọi $u \in \Gamma$.*

Với mỗi $u \in \Gamma$, gọi $K_u$ là tập hợp mọi $x \in K$ sao cho $u(x) = x$. Ta sẽ chỉ ra rằng $K_u$ là không rỗng. Lấy $x$ là một điểm của K; với mỗi số nguyên $n \geq 1$, gọi $x_n$ là phần tử $\frac{1}{n} \sum_{i=0}^{n-1} u^i(x)$ của E. Vì K lồi và ổn định dưới $u$, các điểm $x_n$ thuộc K và vì K compắc, tồn tại một điểm giới hạn $a$ của dãy $(x_n)_{n \geq 1}$. Ánh xạ $y \mapsto u(y) - y$ từ K vào E là liên tục, do đó $u(a) - a$ là một điểm giới hạn của dãy $(u(x_n) - x_n)_{n \geq 1}$. Nhưng ta có $u(x_n) - x_n = \frac{1}{n} (u^n(x) - x)$.

Vì K compắc, nên cũng bị chặn (III, p. 3, mệnh đề 2), dãy $(u^n(x) - x)_{n \geq 1}$ bị chặn; do đó, dãy $\left( \frac{1}{n}(u^n(x) - x) \right)_{n \geq 1}$ tiến tới 0 (III, p. 4, mệnh đề 3), và vì E là Hausdorff, ta có $u(a) - a = 0$. Vậy $a \in K_u$.

Mỗi tập hợp $K_u$ là một tập con đóng và lồi của không gian compắc K, và ta sẽ chứng minh rằng giao $\bigcap_{u \in \Gamma} K_u$ là không rỗng. Để làm điều đó, chỉ cần chứng minh rằng, với $n \geq 1$ và $u_1, ..., u_n$ thuộc $\Gamma$, tập hợp $K_{u_1} \cap ... \cap K_{u_n}$ là không rỗng. Trường hợp $n = 1$ đã được xét, ta lập luận bằng quy nạp theo $n$. Giả sử $n \geq 2$ và đặt $L = K_{u_1} \cap ... \cap K_{u_{n-1}}$. Theo giả thiết quy nạp, L là một tập con compắc lồi không rỗng của E. Vì $u_n$ giao hoán với $u_1, ..., u_{n-1}$, ta có $u_n(L) \subset L$. Áp dụng phần thứ nhất của chứng minh cho phép biến đổi afin cảm sinh bởi $u_n$ trên L, ta kết luận rằng tồn tại một điểm $a$ trong L sao cho $u_n(a) = a$; khi đó $a$ thuộc $K_{u_1} \cap ... \cap K_{u_n}$, do đó tập hợp này là không rỗng.

#### Hệ quả {#evt-iv-a0-n1-cor-1 .statement}

— *Cho G là một nhóm giải được các phép biến đổi afin liên tục trên K. Khi đó tồn tại một điểm trong K bất biến dưới G.*

Theo định nghĩa của một nhóm giải được (A, I, § 6, No. 4), tồn tại một dãy giảm hữu hạn $(G_i)_{0 \leq i \leq n}$ các nhóm con phân biệt của G, sao cho $G_0 = G$, $G_n = \{e\}$ và sao cho nhóm $G_{i-1}/G_i$ là *giao hoán* với $1 \leq i \leq n$. Gọi $K_i$ là tập hợp các điểm bất động của $G_i$ trong K. Khi đó $K_n = K$. Hơn nữa, với $1 \leq i \leq n$, mọi phần tử của $G_i$ đều cảm sinh phép biến đổi đồng nhất trên $K_i$; do đó ta suy ra một tác động của nhóm Abel $G_{i-1}/G_i$ trên K nếu $K_i$ không rỗng; từ định lý 1 suy ra rằng tập hợp $K_{i-1}$ các điểm bất động của $G_{i-1}/G_i$ trong $K_i$ là không rỗng. Bằng quy nạp giảm theo $i$, ta kết luận rằng $K_0$ không rỗng, do đó có hệ quả.

### 2. Trung bình bất biến

Cho X là một không gian tôpô. Ký hiệu $\mathcal{B}(X; \mathbf{R})$ là không gian vectơ thực gồm các ánh xạ liên tục bị chặn từ X vào $\mathbf{R}$. Được trang bị chuẩn $\|f\| = \sup_{x \in X} |f(x)|$, đây là một không gian Banach (GT, X, § 3, No. 1); nó cũng là một không gian vectơ có thứ tự, trong đó quan hệ $f \geq g$ có nghĩa là «$f(x) \geq g(x)$ với mọi $x \in X$».

#### Định nghĩa 1 {#evt-iv-a0-def-1 .statement}

*Một dạng tuyến tính dương $\mu$ trên không gian $\mathcal{B}(X; \mathbf{R})$, trong đó X là một không gian tôpô, và thỏa mãn $\|\mu\| = 1$, được gọi là một trung bình trên X.*

\* Khi X compắc, một trung bình trên X là một độ đo dương trên X sao cho $\mu(X) = 1$. \*

#### Bổ đề 1 {#evt-iv-a0-lem-1 .statement}

*Tập hợp K các trung bình trên X là tập con của quả cầu đơn vị của đối ngẫu của không gian Banach $E = \mathcal{B}(X; \mathbf{R})$ mà các phần tử là những dạng tuyến tính $\mu$ sao cho $\mu(1) = 1$. Nó là một tập con của $E'$ vừa lồi vừa compắc đối với $\sigma(E', E)$.*

Cho $\mu$ là một dạng tuyến tính trên E, sao cho $\mu(1) = 1$. Với mọi hàm $f \in E$, ta định nghĩa hàm $f' \in E$ bởi $f'(x) = \|f\| - f(x)$ ($x \in X$). Trước hết giả sử rằng $\mu$ là một trung bình; với mọi $f \in E$, ta có $f' \geq 0$, do đó $\mu(f') \geq 0$, *tức là* $\mu(f) \leq \|f\|$; vì thế $\|\mu\| \leq 1$.

Ngược lại, giả sử $\mu$ thuộc $E'$, và $\| \mu \| \leq 1$; với mọi hàm dương $f \in E$, ta có $\mu(f') \leq \| f' \|$, do đó

$$
\| f \| - \mu(f) = \mu(f') \leq \| f' \| \leq \| f \|,
$$

và cuối cùng $\mu(f) \geq 0$; do đó, $\mu$ là một trung bình.

Hiển nhiên $K$ là lồi; việc nó compắc đối với $\sigma(E', E)$ suy ra từ hệ quả 3 của III, p. 17.

C.Q.F.D.

Cho $\Gamma$ là một tập hợp các ánh xạ liên tục từ $X$ vào $X$ từng đôi một giao hoán. Cho $\gamma \in \Gamma$. Với mọi hàm $f \in E$, ta có $f \circ \gamma \in E$; do đó ta có thể định nghĩa một phép biến đổi afin $u_{\gamma}$ trên tập hợp $K$ các trung bình trên $X$, bởi

$$
u_{\gamma} \mu(f) = \mu(f \circ \gamma) \quad (\mu \in K, f \in E).
$$

Nếu gán cho $K$ tôpô cảm sinh bởi $\sigma(E', E)$, thì ánh xạ $u_{\gamma}$ là liên tục. Nếu $\gamma$ là một đồng phôi, thì $u_{\gamma} \mu$ có thể được suy ra từ $\mu$ bằng phép chuyển cấu trúc. Cuối cùng, ta có $u_{\gamma} u_{\gamma'} = u_{\gamma' \gamma} u_{\gamma}$ với mọi $\gamma, \gamma'$ trong $\Gamma$. Theo định lý Markoff-Kakutani (IV, p. 39, đl. 1), *tồn tại một trung bình $\mu$ trên $X$, sao cho $u_{\gamma} \mu = \mu$ với mọi $\gamma \in \Gamma$; nói cách khác*, $\mu$ thỏa mãn quan hệ $\mu(f) = \mu(f \circ \gamma)$ với $f \in E$ và $\gamma \in \Gamma$.

Theo một cách tương tự, hệ quả của đl. 1 (IV, p. 40) kéo theo kết quả sau:

#### Mệnh đề 1 {#evt-iv-a0-prop-1 .statement}

*Cho $X$ là một không gian tôpô và $G$ là một nhóm giải được. Giả sử rằng $G$ tác động bên trái lên $X$, sao cho với mọi $g \in G$, ánh xạ $x \mapsto g.x$ từ $X$ vào $X$ là liên tục. Khi đó tồn tại một trung bình trên $X$ bất biến dưới $G$.*

#### Hệ quả {#evt-iv-a0-n2-cor-1 .statement}

*Cho $G$ là một nhóm tôpô giải được. Khi đó tồn tại một trung bình trên $G$ bất biến dưới các phép tịnh tiến trái và phải.*

Chỉ cần áp dụng mệnh đề 1 cho nhóm giải được $G \times G$ tác động trên $G$ bởi $(g.g').x = gxg'^{-1}$.

### 3. Định lý Ryll-Nardzewski

Trong tiết này, $E$ ký hiệu một *không gian* định chuẩn trên trường $\mathbf{R}$ và $\mathcal{T}$ một tôpô lồi địa phương Hausdorff trên $E$ mà đối với nó chuẩn của $E$ là *nửa liên tục dưới*. Các giả thiết này đặc biệt được thỏa mãn trong các trường hợp sau :

$a)$ $\mathcal{T}$ là tôpô cảm sinh bởi chuẩn của không gian chuẩn $E$.
$b)$ $\mathcal{T}$ là tôpô yếu $\sigma(E, E')$ của không gian chuẩn $E$.
$c)$ $E$ là đối ngẫu của một không gian chuẩn $F$ và $\mathcal{T} = \sigma(F', F)$.
$d)$ Tồn tại hai không gian chuẩn $F_1$ và $F_2$ sao cho $E = \mathscr{L}(F_1 ; F_2)$ và $\mathcal{T}$ là tôpô hội tụ đơn giản.

*Trừ khi có nói rõ khác đi, các khái niệm tôpô đều quy chiếu về tôpô $\mathcal{T}$.*

Cho $K$ là một tập con lồi của $E$. Giả sử rằng $K$ là compắc (đối với tôpô $\mathcal{T}$), và rằng $K$ thỏa mãn tiên đề đếm được thứ nhất đối với khoảng cách được xác định bởi chuẩn của $E$.

#### Bổ đề 2 {#evt-iv-a0-lem-2 .statement}

— Giả sử $K$ chứa ít nhất hai điểm. Với mọi $\varepsilon > 0$, tồn tại một phân hoạch của $K$ thành hai tập con không rỗng $K_1$ và $K_2$, có các tính chất sau :

a) $K_1$ lồi và compắc ;
b) ta có $\| x_1 - x_2 \| < \varepsilon$ với mọi $x_1$ và $x_2$ thuộc $K_2$.

Cho $L$ là bao đóng của tập hợp tất cả các điểm cực biên của $K$. Theo đ.l. Krein-Milman (II, p. 55, th. 1), $K$ là bao lồi đóng của $L$. Vì $K$ chứa ít nhất hai điểm, nên $L$ cũng vậy. Với mọi $x \in L$, gọi $A_x$ là tập hợp tất cả các $y \in L$ sao cho $\| x - y \| \leq \varepsilon / 4$. Theo giả thiết, trên $K$, tồn tại một tập con đếm được $D$ của $L$ sao cho $L = \bigcup_{x \in D} A_x$. Vì chuẩn là nửa liên tục dưới, mỗi tập hợp $A_x$ đều đóng. Áp dụng đ.l. Baire (GT, IX, § 5, No. 3, th. 1) cho không gian compact $L$, ta thấy tồn tại một điểm $a$ trong $D$ và một tập con mở $U$ trong $E$ sao cho $L \cap U$ khác rỗng và được chứa trong $A_a$. Vì $L$ chứa ít nhất hai điểm, và vì $E$ là Hausdorff, ta có thể chọn $U$ sao cho $L \notin U$.

Cho $M$ là bao lồi đóng của $L \cap \complement U$. Với mọi số thực $t$ sao cho $0 < t < 1$, gọi $M_t$ là tập hợp tất cả các vectơ có dạng $tx_1 + (1 - t) x_2$ với $x_1 \in M$ và $x_2 \in K$; đó là một tập con lồi compắc không rỗng của $K$. Ta sẽ chứng minh rằng $M_t \neq K$ bằng phản chứng. Giả sử rằng $M_t = K$; khi đó mọi điểm cực biên $x$ của $K$ đều thuộc $M_t$, nên có thể viết dưới dạng $x = tx_1 + (1 - t) x_2$ với $x_1 \in M$ và $x_2 \in K$. Điều này kéo theo rằng $x = x_1 = x_2$, và do đó $x \in M$. Theo đl. Krein-Milman (II, p. 55, đl. 1), ta có $K = M$, và $K$ là bao lồi đóng của $L \cap \complement U$. Theo II, p. 56, hệ quả, điều này kéo theo rằng $L \subset L \cap \complement U$, điều mâu thuẫn với quan hệ $L \cap U \neq \varnothing$.

Đặt $d = \sup_{x \in K, y \in K} \| x - y \|$ và chọn một số thực $t$ sao cho $0 < t < 1$ và $t < \varepsilon / 4d$. Đặt $K_1 = M_t$ và $K_2 = K - M_t$. Theo lập luận trước đó, các tập hợp $K_1$ và $K_2$ là không rỗng, và $K_1$ lồi và compact. Gọi $M'$ là bao lồi đóng của $L \cap U$. Vì $K$ là bao lồi đóng của tập hợp $L = (L \cap \complement U) \cup (L \cap U)$, nên nó cũng là bao lồi đóng của $M \cup M'$. Gọi $x_1$ và $x_2$ là hai điểm của $K_2$; với $i = 1, 2$, tồn tại $y_i \in M$, $z_i \in M'$ và một số thực $\alpha_i$ sao cho $0 \leq \alpha_i \leq 1$ và $x_i = \alpha_i y_i + (1 - \alpha_i) z_i$. Nếu $\alpha_i \geq t$, thì
$$
x_i = t y_i + (1 - t) \left\{ \frac{\alpha_i - t}{1 - t} y_i + \frac{1 - \alpha_i}{1 - t} z_i \right\}
$$
; điều này mâu thuẫn với giả thiết rằng $x_i \notin M_i$. Vậy $\alpha_i < t$, với $i = 1, 2$, và do đó
$$
\| x_i - z_i \| = \| \alpha_i (y_i - z_i) \| = \alpha_i \| y_i - z_i \| \leq \alpha_i d < dt < \varepsilon / 4 .
$$
Với mọi điểm $z$ trong $M'$, ta có $\| z - a \| \leq \varepsilon / 4$, vì $L \cap U \subset A_a$, và do đó, đặc biệt $\| z_i - a \| \leq \varepsilon / 4$. Vì thế
$$
\| x_1 - x_2 \| \leq \sum_{i=1}^2 (\| x_i - z_i \| + \| z_i - a \|) < \varepsilon .
$$
Điều này hoàn tất chứng minh.

#### Bổ đề 3 {#evt-iv-a0-lem-3 .statement}

— Cho G là một nhóm các phép biến đổi afin liên tục (đối với $\mathcal{T}$) trên K. Giả sử rằng K không rỗng và rằng $\|gx - gy\| = \|x - y\|$ với mọi x, y trong K và mọi g trong G. Khi đó tồn tại một điểm của K bất biến dưới G.

Gọi $\mathfrak{J}$ là họ các tập con không rỗng của K mà đóng, lồi và ổn định dưới G. Nếu $(L_\alpha)_{\alpha \in I}$ là một họ các phần tử của $\mathfrak{J}$ được sắp thứ tự toàn phần bởi quan hệ bao hàm, thì tập hợp $L = \bigcap_{\alpha \in I} L_\alpha$ thuộc $\mathfrak{J}$. Do đó (S, III, § 3, No. 4, đl. 2), tồn tại một phần tử L trong $\mathfrak{J}$ là cực tiểu đối với quan hệ bao hàm. Ta sẽ chứng minh rằng L thu về một điểm.

Ta lập luận bằng phản chứng, giả sử rằng L chứa ít nhất hai điểm phân biệt $x_1$ và $x_2$, đặt $x = (x_1 + x_2)/2$ và $\varepsilon = \|x_1 - x_2\|/2$. Tập compact và lồi L thỏa mãn tiên đề đếm được thứ nhất đối với khoảng cách xác định bởi chuẩn (GT, IX, § 2, No. 8). Do đó ta có thể áp dụng bổ đề 2 và tìm được một tập con compact và lồi $L_1$ của L, phân biệt với $\varnothing$ và với L, có tính chất sau :

(A) *Với mọi $y_1$ và $y_2$ trong $L - L_1$, ta có $\|y_1 - y_2\| < \varepsilon$.*

*Ta sẽ chứng minh bằng phản chứng rằng $gx \in L_1$ với mọi $g \in G$.* Giả sử $g \in G$ sao cho $gx \in L - L_1$; khi đó ta có

$$
\|gx_i - gx\| = \|x_i - x\| = \|x_1 - x_2\|/2 = \varepsilon ,
$$

với $i = 1, 2$. Theo tính chất (A), ta có $gx_i \in L_1$. Vì $L_1$ là lồi, ta kết luận rằng $gx = (gx_1 + gx_2)/2$ thuộc $L_1$, điều này mâu thuẫn với giả thiết.

Cho $L'$ là bao lồi đóng của quỹ đạo $Gx$ của x. Tập hợp $L'$ thuộc $\mathfrak{J}$. Theo lập luận trước, ta có $L' \subset L_1$, do đó $L' \subset L, L' \neq L$. Điều này mâu thuẫn với đặc trưng cực tiểu của L và chứng minh được hoàn tất.

#### Định lý 2 (Ryll-Nardzewski) {#evt-iv-a0-thm-2 .statement}

— *Cho E là một không gian định chuẩn và K là một tập con lồi không rỗng của E, compact đối với tôpô yếu $\sigma(E, E')$. Cho G là một nhóm các phép biến đổi afin đẳng cự của K. Khi đó tồn tại một điểm của K bất biến dưới G.*

Với mọi $g \in G$, ký hiệu $K_g$ là tập hợp tất cả các điểm x trong K sao cho $gx = x$; gán cho K tôpô yếu; mỗi tập hợp $K_g$ đều lồi và đóng trong không gian compact K. Ta sẽ chứng minh rằng giao $\bigcap_{g \in G} K_g$ là không rỗng; để làm điều này, chỉ cần chứng minh rằng tập hợp $K_{g_1} \cap ... \cap K_{g_n}$ là không rỗng với mọi $g_1, ..., g_n$ trong G. Cố định $g_1, ..., g_n$ và gọi H là nhóm con của G sinh bởi $\{ g_1, ..., g_n \}$. Chọn một điểm a trong K và ký hiệu L là bao lồi đóng của quỹ đạo Ha của a. Gọi D là tập hợp đếm được các phần tử dạng $\lambda_1 h_1 a + \cdots + \lambda_m h_m a$, trong đó $\lambda_1, ..., \lambda_m$ là các số hữu tỉ dương sao cho $\lambda_1 + \cdots + \lambda_m = 1$, và $h_1, ..., h_m$ là các phần tử của H. Bao đóng $\overline{D}$ của D đối với tôpô mạnh là lồi, do đó nó đóng đối với $\sigma(E, E')$ (IV, p. 4, mệnh đề 2); vì thế $\overline{D} = L$ và điều này chứng minh rằng L là một không gian metric thỏa mãn tiên đề đếm được thứ nhất đối với khoảng cách $(x, y) \mapsto \|x - y\|$. Bây giờ ta có thể áp dụng bổ đề 2. Tồn tại một điểm b trong L bất biến dưới H, do đó $b \in K_{g_1} \cap ... \cap K_{g_n}$.

#### Hệ quả {#evt-iv-a0-n3-cor-1 .statement}

— Cho E là một không gian Banach phản xạ, G là một nhóm các tự đẳng cấu của không gian định chuẩn E, và K là một tập con của E. Giả sử rằng K là không rỗng, lồi, đóng, bị chặn và ổn định dưới G. Khi đó tồn tại một điểm trong K bất biến dưới G.

Vì E là phản xạ, K là compact đối với $\sigma(E, E')$ (IV, p. 15, đl. 1). Hơn nữa, mọi phần tử của G đều thuộc $\mathcal{L}(E)$.

### 4. Các ứng dụng.

\* A) Các biểu diễn unita của nhóm :
Cho E là một không gian Hilbert phức, G là một nhóm và $\pi$ là một biểu diễn unita của G trên E, tức là một đồng cấu từ G vào nhóm các tự đẳng cấu của E. Gọi $E^G$ là không gian con Hilbert của E gồm tất cả các vectơ bất biến dưới $\pi(G)$. Với mọi $x \in E$, gọi $K_x$ là bao lồi đóng của quỹ đạo của x. Cố định một điểm x trong E.

Ta sẽ chỉ ra rằng tồn tại một điểm duy nhất trong $K_x$ bất biến dưới $\pi(G)$, tức là phép chiếu của x lên $E^G$. Theo IV, p. 44, hệ quả (áp dụng cho không gian vectơ thực nền của E), tồn tại một điểm trong $K_x$ bất biến dưới $\pi(G)$; gọi a là một điểm như vậy; khi đó $a \in E^G$. Gọi P là tập hợp tất cả các $y \in E$ sao cho $y - x$ trực giao với $E^G$; ta thấy ngay lập tức rằng P là đóng, lồi và bất biến dưới $\pi(G)$; do đó $x \in P$, suy ra $K_x \subset P$ và cuối cùng $a \in P$. Nói cách khác, $a - x$ trực giao với $E^G$; do đó a là phép chiếu của x lên $E^G$. \*

\* B) Vết của một toán tử trong một không gian Hilbert :
Giả sử rằng biểu diễn $\pi$ là bất khả quy, nghĩa là không tồn tại không gian con Hilbert nào của E, phân biệt với $\{0\}$ và với E, mà bất biến dưới $\pi(G)$. Gọi $F = \mathcal{L}^2(E)$ là không gian Hilbert của mọi toán tử Hilbert-Schmidt trên E, với tích vô hướng $\langle u|v \rangle = \operatorname{Tr}(u^*v)$. Ta định nghĩa một biểu diễn unita $\lambda$ từ G vào F bởi công thức

$$
\lambda(g).u = \pi(g)\ u\pi(g)^{-1} \quad (u \in F,\ g \in G)
$$

Không gian $F^G$ của mọi phần tử của E bất biến dưới $\lambda(G)$ gồm các nội cấu Hilbert-Schmidt $u$ của E giao hoán với $\pi(g)$ với mọi $g \in G$. Theo bổ đề Schur, một $u$ như vậy là một phép vị tự. Do đó ta phải xét hai trường hợp :
1) nếu E là hữu hạn chiều vô hạn, thì $F^G = \{0\}$;
2) nếu E là hữu hạn chiều, thì $F = \mathcal{L}(E)$ và $F^G = \mathbf{C}.1_E$.

Áp dụng kết quả của A) cho biểu diễn unita $\lambda$, ta thu được định lý sau :

Cho $u \in \mathcal{L}^2(E)$, và gọi $A_u$ là bao lồi đóng trong $\mathcal{L}^2(E)$ của tập các nội tự đồng cấu $\pi(g)\ u\pi(g)^{-1}$ của E, trong đó g chạy qua G. Nếu E vô hạn chiều, ta có $0 \in A_u$. Nếu E hữu hạn chiều và có chiều d, thì tồn tại đúng một phép vị tự trong $A_u$, đó là phép chiếu $\frac{1}{d}\ \operatorname{Tr}(u).\ 1_E$ của u lên không gian con $\mathbf{C}.1_E$ của $\mathcal{L}^2(E)$. \*

C) Độ đo Haar của một nhóm compact:

Cho G là một nhóm compact và đặt E = $\mathcal{C}(G, \mathbf{R})$ là không gian Banach của tất cả các hàm liên tục nhận giá trị thực trên G, được trang bị chuẩn

$$
\| f \| = \sup_{x \in G} |f(x)| .
$$

Với mọi $x \in G$, ta định nghĩa các tự đẳng cấu $\gamma_x$ và $\delta_x$ của E bởi các công thức

$$
\gamma_x f(y) = f(x^{-1}y) , \quad \delta_x f(y) = f(yx)
$$

(với $y \in G,\ f \in E$).

*Cho $f \in E$, gọi $\Gamma_f$ (lần lượt $\Delta_f$) là bao lồi đóng trong E, của tập hợp mọi hàm $\gamma_x f$ (lần lượt $\delta_x f$) khi x chạy trên G. Chúng ta sẽ chứng minh rằng tồn tại một hàm hằng duy nhất $\mu(f)$ thuộc $\Gamma_f$, một hàm hằng duy nhất $\mu'(f)$ thuộc $\Delta_f$, và các hằng này bằng nhau.*

Hiển nhiên là một hàm liên tục trên G là bất biến dưới các tự đẳng cấu $\gamma_x$ (tương ứng $\delta_x$) của E khi và chỉ khi nó là hằng. Bây giờ, tập hợp tất cả các hàm $\gamma_x f$ (tương ứng $\delta_x f$) với x thuộc G là compact trong E, vì ánh xạ $x \mapsto \gamma_x f$ (tương ứng $x \mapsto \delta_x f$) từ G vào E là liên tục (GT, X, § 3, No. 4, đl. 3). Suy ra (II, p. 25, mđ. 3) rằng $\Gamma_f$ (tương ứng $\Delta_f$) là một tập compact trong E đối với tôpô xác định bởi chuẩn, do đó cũng đối với $\sigma(E, E')$. Theo đl. Ryll-Nardzewski (IV, p. 43, đl. 2), tồn tại các hàm hằng trong $\Gamma_f$ và $\Delta_f$. Còn phải chứng minh rằng nếu $c_1 \in \Gamma_f$ và $c_2 \in \Delta_f$ là các hằng, thì $c_1 = c_2$.

Cho $\varepsilon > 0$. Theo giả thiết, tồn tại các điểm $x_1, ..., x_n,\ y_1, ..., y_n$ trong G và các số thực dương $\lambda_1, ..., \lambda_n,\ \mu_1, ..., \mu_m$ sao cho

$$
\lambda_1 + \cdots + \lambda_n = \mu_1 + \cdots + \mu_m = 1 .
$$
$$
\sup_{x \in G} \left| \sum_{i=1}^n \lambda_i f(x_i x) - c_1 \right| \leq \varepsilon ,
$$
$$
\sup_{x \in G} \left| \sum_{j=1}^m \mu_j f(xy_j) - c_2 \right| \leq \varepsilon .
$$

Đặt $r = \sum_{i,j} \lambda_i \mu_j f(x_i y_j)$. Khi đó $r - c_1 = \sum_{j=1}^m \mu_j a_j$ với $a_j = \sum_{i=1}^n \lambda_i f(x_i y_j) - c_1$; theo (7), ta có $|a_j| \leq \varepsilon$ với $1 \leq j \leq m$, do đó $|r - c_1| \leq \varepsilon$. Tương tự, ta chứng minh được bất đẳng thức $|r - c_2| \leq \varepsilon$, suy ra $|c_1 - c_2| \leq 2\varepsilon$. Vì $\varepsilon$ là tùy ý, ta được $c_1 = c_2$, như đã khẳng định.

Theo định nghĩa của $\mu(f)$, với mọi $\varepsilon > 0$ ta có thể tìm được các số dương $\lambda_1, ..., \lambda_n$ có tổng bằng 1 và các phần tử $x_1, ..., x_n$ trong G sao cho $\left| \sum_{i=1}^n \lambda_i f(x_i x) - \mu(f) \right| \leq \varepsilon$ với mọi $x \in G$.

Ngay lập tức thấy rằng với $f, g$ trong E và với mọi vô hướng $\lambda$, ta có $\Gamma_{f+g} \subset \Gamma_f + \Gamma_g$ và $\Gamma_{\gamma f} = \lambda \Gamma_f$, do đó ta có các hệ thức $\mu(f+g) = \mu(f) + \mu(g)$ và $\mu(\lambda f) = \lambda \mu(f)$. Vì thế, ánh xạ $\mu : f \mapsto \mu(f)$ từ E vào $\mathbf{R}$ là một trung bình trên không gian compact G (IV, p. 40); *nói cách khác $\mu$ là một độ đo dương trên G sao cho $\mu(G) = 1$*.

Hiển nhiên là $\mu$ bất biến dưới các phép tịnh tiến trái của $G$, và đẳng thức $\mu(f) = \mu'(f)$ kéo theo rằng $\mu$ cũng bất biến dưới các phép tịnh tiến phải. \* Nói cách khác, $\mu$ là một độ đo trái và một độ đo phải trên $G$ (INT, VII, § 1, No. 2, def. 2). \*

*D) Sự tồn tại của các độ đo bất biến :

Cho $X$ là một không gian tôpô Hausdorff, $\mu$ là một độ đo dương bị chặn trên $X$, và $G$ là một nhóm các đồng phôi của $X$. Giả sử rằng với mọi $g \in G$, độ đo $g.\mu$, là ảnh của $\mu$ dưới ánh xạ $g : X \to X$, có cơ sở $\mu$. Gọi $u_g$ là một hàm dương khả tích đối với $\mu$ trên $X$ sao cho $g.\mu = u_g.\mu$. Cũng giả sử rằng tồn tại hai hàm dương khả tích đối với $\mu$, $\phi$ và $\psi$, trên $X$, không phải là $\mu$-không và thỏa mãn $\phi \leq u_g \leq \psi$ $\mu$-hầu khắp nơi với mọi $g \in G$. Ta sẽ chứng minh rằng tồn tại một độ đo dương bị chặn $\nu \neq 0$ trên $X$, có cơ sở $\mu$, và bất biến dưới $G$.

Cho $P$ là tập con của không gian Banach $E = L^1(X, \mu)$ gồm các lớp hàm $f$ sao cho $\phi \leq f \leq \psi$ $\mu$-hầu khắp nơi. Khi đó $P$ là compact đối với tôpô yếu $\sigma(E, E')$. Ánh xạ $h \mapsto h.\mu$ từ $P$ vào không gian Banach $F = \mathcal{M}^b(X)$ của các độ đo thực bị chặn trên $X$, là một song ánh từ $P$ lên một tập con $P_1$ của $E$ mà lồi và compact đối với tôpô $\sigma(F, F')$. Theo giả thiết, $g.\mu \in P_1$ với mọi $g \in G$. Gọi $K$ là bao lồi đóng của tập hợp mọi độ đo $g.\mu$. Với mọi $g \in G$, ánh xạ $\nu \mapsto g.\nu$ là một phép biến đổi afin đẳng cự của $K$. Theo định lý Ryll-Nardzewski (IV, p. 43, th. 2), tồn tại một độ đo $\nu \in K$ bất biến dưới tác động của $G$. Ta có $\phi.\mu \leq \nu$, do đó $\nu \neq 0$. \*

Bài tập

### Bài tập {#evt-iv-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).
