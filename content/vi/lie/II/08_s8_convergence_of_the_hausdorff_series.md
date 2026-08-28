---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 8
section_title: Convergence of the Hausdorff series (ultrametric case)
lang: vi
source: lie-i-iii
pdf_pages: 0188-0194, 0223-0225
extraction: ocr
subsections:
    - "no": 1
      title: $p$-adic upper bounds of the series exp, log and $\mathbf{H}$
      page: 0
      pdf_page: 189
    - "no": 2
      title: NORMED LIE ALGEBRAS
      page: 0
      pdf_page: 190
    - "no": 3
      title: GROUP DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 0
      pdf_page: 190
    - "no": 4
      title: EXPONENTIAL IN COMPLETE NORMED ASSOCIATIVE ALGEBRAS
      page: 0
      pdf_page: 192
statements: 9
exercises: 4
content_sha256: d77322565b81e513dbfd95ee99e4568c10a4cd6611d45e16b254765ee7137d85
translated_from: content/en/lie/II/08_s8_convergence_of_the_hausdorff_series.md
source_content_sha256: dd8b3a4a37711971ee89a625e730b67e3445af5fd7e146dbb08e9a125ac0c3d4
translation_model: gpt-5.4
translation_run: translate-vi-dc8f82dd
glossary_version: 34
glossary_terms_sha256: 05f806221fde68242cbee59b574d6cfe858a86c328907db6a33c4a49f2a659e9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. SỰ HỘI TỤ CỦA CHUỖI HAUSDORFF (TRƯỜNG HỢP ULTRAMETRIC)

Trong tiết này ta giả sử rằng K là một *trường giá trị đầy đủ không rời rạc có đặc số không*, với một giá trị tuyệt đối *ultrametric*. Ta ký hiệu bởi $p$ đặc số của trường thặng dư của K (*Đại số giao hoán*, Chương VI, § 3, no. 2).
Nếu $p \neq 0$, ta đặt $a = |p|$; ta biết (*Đại số giao hoán*, Chương VI, § 6, nos. 2 and 3) rằng $0 < a < 1$ và tồn tại một và chỉ một giá trị $v$ trên K nhận giá trị trong $\mathbf{R}$ mà hạn chế của nó trên $\mathbf{Q}$ là giá trị $p$-adic $v_p$ và sao cho $|x| = a^{v(x)}$ với mọi $x \in K$. Ta còn đặt:
(1)    $\theta = \frac{1}{p-1}.$

Nếu $p = 0$, ta ký hiệu bởi $a$ một số thực sao cho $0 < a < 1$ và bởi $v$ một định giá trên $\mathbf{K}$ nhận giá trị trong $\mathbf{R}$ sao cho $|x| = a^{v(x)}$ với mọi $x \in \mathbf{K}$ (*loc. cit.*). Khi đó $v(x) = 0$ với $x \in \mathbf{Q}^*$. Ta cũng viết:
$$
\theta = 0.
$$

### 1. Các chặn trên $p$-adic của các chuỗi exp, log và $\mathbf{H}$

*Trong số này, ta giả sử rằng $p \neq 0$.*

#### Bổ đề 1 {#lie-ii-s8-lem-1 .statement}

*Cho $n$ là một số nguyên $\geqslant 0$ và cho $n = n_0 + n_1 p + \cdots + n_k p^k$, với $0 \leqslant n_i \leqslant p - 1$, là khai triển $p$-adic của $n$. Đặt $S(n) = n_0 + n_1 + \cdots + n_k$. Khi đó*
$$
v_p(n!) = \frac{n - S(n)}{p - 1}.
$$
$v_p(n!) = \sum_{i=1}^n v_p(i)$ và số các số nguyên $i$ nằm giữa 1 và $n$ sao cho $v_p(i) \geqslant j$ bằng phần nguyên $[n/p^j]$ của $n/p^j$. Do đó
$$
v_p(n!) = \sum_{j \geqslant 0} j ([n/p^j] - [n/p^{j+1}]) = \sum_{j \geqslant 1} [n/p^j].
$$
Vì $[n/p^j] = \sum_{i \geqslant j} n_i p^{i-j}$, nên suy ra bổ đề.

#### Bổ đề 2 {#lie-ii-s8-lem-2 .statement}

$v(n) \leqslant v(n!) \leqslant (n - 1)\theta$ và $v(n) \leqslant (\log n)/(\log p)$ với mọi số nguyên $n \geqslant 1$.
$v(n!) = v_p(n!) = (n - S(n))\theta \leqslant (n - 1)\theta$ theo Bổ đề 1.
Mặt khác, $n \geqslant p^{v(n)}$, do đó $v(n) \leqslant (\log n)/(\log p)$.
Cho $I = \{ U, V \}$ là một tập hợp gồm hai phần tử và
$$
\mathbf{H} = \sum_{r,s \geqslant 0} H_{r,s}(U, V) \in \hat{\mathbf{L}}_{\mathbf{Q}}(I)
$$
là chuỗi Hausdorff (§ 6, no. 4, Định nghĩa 1). Cho $\mathbf{Z}_{(p)}$ là vành địa phương của $\mathbf{Z}$ đối với iđêan nguyên tố $(p)$ và $(e_b)_{b \in B}$ là một cơ sở của $\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$ trên $\mathbf{Z}$ (§ 2, no. 11, Định lý 1). Nó cũng là một cơ sở của $\mathbf{L}_{\mathbf{Q}}(I)$ trên $\mathbf{Q}$.

#### Mệnh đề 1 {#lie-ii-s8-prop-1 .statement}

*Nếu $r$ và $s$ là hai số nguyên $\geqslant 0$. Nếu $H_{r,s} = \sum_{b \in B} \lambda_b e_b$, trong đó $\lambda_b \in \mathbf{Q}$, là phân tích của $\mathbf{H}$ theo cơ sở $(e_b)_{b \in B}$, thì*
$$
v_p(\lambda_b) \geqslant -(r + s - 1)\theta \quad \text{với mọi } b \in B.
$$
Vành $\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$ được đồng nhất với môđun con trên $\mathbf{Z}_{(p)}$ của $\mathbf{A}_{\mathbf{Q}}(I)$ sinh bởi các từ $w \in \mathrm{Mo}(I)$. Vì $\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$ là một nhân tử trực tiếp của $\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$,
$$
\mathbf{L}_{\mathbf{Z}_{(p)}}(I) = \mathbf{A}_{\mathbf{Z}_{(p)}}(I) \cap \mathbf{L}_{\mathbf{Q}}(I).
$$

Cho $f$ là số nguyên sao cho $f \leq (r + s - 1)\theta < f + 1$. Quan hệ (4) tương đương với $v_p(\lambda_b) \geq -f$ với mọi $b \in B$, nghĩa là $H_{r,s} \in p^{-f}L_{\mathbf{Z}(p)}$. Nhưng điều này, theo (5), cũng tương đương với $H_{r,s} \in p^{-f}A_{\mathbf{Z}(p)}(I)$.

Theo công thức (11) của § 6, no. 4, chỉ cần chứng minh rằng, với mọi số nguyên $m \geq 1$ và mọi số nguyên $r_1, \ldots, r_m, s_1, \ldots, s_m$ sao cho
$$
r_1 + \cdots + r_m = r, \quad s_1 + \cdots + s_m = s,
$$
$$
r_i + s_i \geq 1 \quad \text{với } 1 \leq i \leq m,
$$
ta có
$$
v_p(m!r!\ldots r_m!s_1!\ldots s_m!) \leq f.
$$
Nhưng theo Bổ đề 2, $v_p(r_i!s_i!) \leq (r_i + s_i - 1)\theta$ và $v_p(m!) \leq v_p(m!) \leq (m - 1)\theta$; do đó vế trái của (7) bị chặn trên bởi
$$
\theta(m - 1 + \sum_{i=1}^m (r_i + s_i - 1)) = \theta(r + s - 1);
$$
vì nó là một số nguyên, nên nó $\leq f$, điều này hoàn tất chứng minh.

### 2. ĐẠI SỐ LIE CHUẨN

#### Định nghĩa 1 {#lie-ii-s8-def-1 .statement}

*Một đại số Lie có chuẩn trên K* là một đại số Lie được trang bị một chuẩn sao cho
$$
\|x + y\| \leq \sup(\|x\|, \|y\|)
$$
$$
\|[x, y]\| \leq \|x\| \cdot \|y\|
$$
với mọi $x, y$ trong $g$.

*Trong suốt phần còn lại của đoạn này, g ký hiệu một đại số Lie có chuẩn đầy đủ.*

Với mọi tập hợp hữu hạn I, như trong § 7, no. 1, ta định nghĩa một đồng cấu đại số Lie liên tục $u \mapsto \tilde{u}$ từ $\hat{L}(I)$ vào $\hat{P}(g^I; g)$. Ta thấy như trong § 7 rằng nếu $u = \sum_v u_v$, với $u_v \in L^v(I)$ đối với $v \in \mathbf{N}^I$, thì $\tilde{u} = \sum_v \tilde{u}_v$, trong đó $\tilde{u}_v$ là ánh xạ đa thức $(t_i)_{i \in I} \mapsto u_v((t_i))$ được định nghĩa trong § 2, no. 4. Công thức hợp thành (2) của § 7, no. 1, vẫn còn đúng.

### 3. NHÓM ĐƯỢC XÁC ĐỊNH BỞI MỘT ĐẠI SỐ LIE CÓ CHUẨN ĐẦY ĐỦ

Cho $H = \sum_{r, s \geq 0} H_{r,s} \in \hat{L}(\{U, V\})$ là chuỗi Hausdorff (§ 6, no. 4, Định nghĩa 1). Ta sẽ chỉ ra rằng chuỗi lũy thừa hình thức tương ứng có các thành phần liên tục
$$
\tilde{H} = \sum_{r, s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$
là hội tụ (*Differentiable and Analytic Manifolds*, R, 4.1.1).

Cho $r \geq 0, s \geq 0$ sao cho $r + s \neq 0$ và gọi $\| \tilde{H}_{r,s} \|$ là chuẩn của đa thức liên tục $\tilde{H}_{r,s}$ (Đa tạp khả vi và giải tích, R, Phụ lục, no. 2).

#### Bổ đề 3 {#lie-ii-s8-lem-3 .statement}

$$
\| \tilde{H}_{r,s} \| \leq a^{-(r+s-1)\theta}.
$$

Cho B là một tập Hall đối với I và cho $H_{r,s} = \sum_{b \in B} \lambda_b e_b$ là phân tích của $H_{r,s}$ theo cơ sở tương ứng của $L(\{U, V\})$. Khi đó
$$
|\lambda_b| \leq a^{-(r+s-1)\theta}.
$$
Điều này là tầm thường đối với $p = 0$, vì $\lambda_b \in \mathbf{Q}$; và nó suy ra từ Mệnh đề 1 của no. 1 khi $p \neq 0$.

Hơn nữa,
$$
\| \tilde{e}_b \| \leq 1 \quad \text{với } b \in B.
$$
Nói chung hơn, ta chứng minh bằng quy nạp theo $n$ rằng, với mọi alternant $b$ bậc $n$ theo hai bất định U và V (§ 2, no. 6), ta có $\| \tilde{b} \| \leq 1$. Nếu $n = 1$, $\tilde{b}$ là một trong các phép chiếu của $g \times g$ lên $g$ và do đó có chuẩn $\leq 1$; nếu $n > 1$, tồn tại hai alternant $b_1$ và $b_2$ có bậc $< n$ sao cho $b = [b_1, b_2]$. Vì ánh xạ $\gamma : (x, y) \mapsto [x, y]$ từ $g \times g$ vào $g$ là song tuyến tính và có chuẩn $\leq 1$, nên ta có (Đa tạp khả vi và giải tích, R, phụ lục, no. 4)
$$
\| \tilde{b} \| = \| \gamma \circ (\tilde{b}_1, \tilde{b}_2) \| \leq \| \tilde{b}_1 \| \cdot \| \tilde{b}_2 \| \leq 1.
$$
Các hệ thức (11) và (12) suy ra bổ đề.

#### Mệnh đề 2 {#lie-ii-s8-prop-2 .statement}

Chuỗi lũy thừa hình thức $\tilde{H}$ là một chuỗi hội tụ (Đa tạp Khả vi và Giải tích, R, 4.1.1). Nếu G là quả cầu $\{ x \in g \mid \| x \| < a^\theta \}$, thì miền hội tụ tuyệt đối của $\tilde{H}$ (Đa tạp Khả vi và Giải tích, R, 4.1.3) chứa $G \times G$.

Nếu $u$ và $v$ là hai số thực $> 0$ sao cho $u < a^\theta$ và $v < a^\theta$, thì (Bổ đề 3)
$$
\| \tilde{H}_{r,s} \| u^r v^s \leq a^\theta (u a^{-\theta})^r (v a^{-\theta})^s
$$
và $\| H_{r,s} \| u^r v^s$ tiến tới 0 khi $r + s$ tiến tới vô hạn.

Ta ký hiệu bởi $h : G \times G \to g$ hàm giải tích (Differentiable and Analytic Manifolds, R, 4.2.4) được xác định bởi $\tilde{H}$, nghĩa là bởi công thức
$$
h(x, y) = \sum_{r, s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y) \quad \text{với } (x, y) \in G \times G.
$$
Hàm này được gọi là hàm Hausdorff của $g$.

Cho $(x, y) \in G \times G$. Khi đó
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \sup(\| x \|, \| y \|) \\
\| h(x, y) \| \leq \sup(\| x \|, \| y \|).
$$

(17) suy ra ngay lập tức từ (16) và (16) là tầm thường đối với $r = s = 0$; nếu $r \geq 1$, thì
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \| \tilde{H}_{r,s} \| \| x \|^{r} \| y \|^{s}
$$
$$
\leq \| x \| \left( \frac{\| x \|}{a^{\theta}} \right)^{r-1} \left( \frac{\| y \|}{a^{\theta}} \right)^{s}
$$
$$
\leq \| x \|;
$$
ta lập luận tương tự nếu $s \geq 1$.

Đặc biệt, $\| h(x, y) \| < a^{\theta}$ với $(x, y) \in G \times G$.

#### Mệnh đề 3 {#lie-ii-s8-prop-3 .statement}

*Cho $G$ là quả cầu $\{ x \in g | \| x \| < a^{\theta} \}$. Ánh xạ giải tích*
$$
h : G \times G \to G
$$
*biến $G$ thành một nhóm, trong đó $0$ là phần tử đơn vị và $-x$ là nghịch đảo của $x$ với mọi $x \in G$. Hơn nữa, nếu $R$ là một số thực sao cho $0 < R < a^{\theta}$, thì quả cầu*
$$
\{ x \in g | \| x \| < R \}
$$
*(resp. $\{ x \in g | \| x \| \leq R \}$) là một nhóm con mở của $G$*.

Vì $H(U, -U) = 0$ và $H(0, U) = H(U, 0) = U$, nên $h(x, -x) = 0$ và
$$
h(0, x) = h(x, 0) = x
$$
với mọi $x \in G$. Do đó còn phải chứng minh công thức tính kết hợp
$$
h(h(x, y), z) = h(x, h(y, z)) \quad \text{với } x, y, z \text{ trong } G.
$$
Vì
$$
H(H(U, V), W) = H(U, H(V, W))
$$
trong $\hat{L}(\{ U, V, W \})$ (§ 6, no. 5, Mệnh đề 4), nên ta có
$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H})
$$
trong $\hat{P}(g \times g \times g; g)$ (no. 2) và (19) suy ra (18) theo (16) và *Variétés différentiables et analytiques*, R, 4.1.5.

*Nói cách khác (Chương III, § 1), $G$ cùng với hàm Hausdorff là một nhóm Lie.*

### 4. HÀM MŨ TRONG CÁC ĐẠI SỐ KẾT HỢP CÓ CHUẨN ĐẦY ĐỦ

Trong số này, A sẽ ký hiệu một đại số kết hợp có đơn vị với một chuẩn $x \mapsto \| x \|$ thỏa mãn các điều kiện:
$$
\| x + y \| \leq \sup(\| x \|, \| y \|) \\
\| xy \| \leq \| x \| \cdot \| y \| \\
\| 1 \| = 1
$$

với $x, y$ trong $A$, và *đầy đủ* đối với chuẩn này. Các kết quả của đoạn thứ hai và thứ ba của § 7, no. 3, vẫn còn đúng.

Ta đặt $I = \{ U \}$ và xét các ảnh $\tilde{e}$ và $\tilde{l}$ của các chuỗi $e(U) = \sum_{n \geq 1} \frac{U^n}{n!}$ và $l(U) = \sum_{n \geq 1} (-1)^{n-1} \frac{U^n}{n}$ trong $\hat{P}(A; A)$. Khi đó:

$$
\left\| \left( \frac{U^n}{n!} \right)^{\sim} \right\| \leq a^{-(n-1)\theta}
$$
$$
\left\| \left( \frac{U^n}{n} \right)^{\sim} \right\| \leq a^{-\frac{\log n}{\log p}}
$$

theo Bổ đề 2 của no. 1. Do đó *bán kính hội tụ tuyệt đối* của chuỗi $\tilde{e}$ (tương ứng, $\tilde{l}$) là $\geq a^\theta$ (tương ứng, $\geq 1$) (*Differentiable and Analytic Manifolds*, R, 4.1.3). Với $R > 0$, đặt $G_R = \{ x \in A \mid \|x\| < R \}$; ta viết $G = G_0$. Chuỗi $\tilde{e}$ (tương ứng, $\tilde{l}$) xác định một ánh xạ giải tích $e_A$ (tương ứng, $l_A$) từ $G$ (tương ứng, $G_1$) vào $A$. Ta viết:
$$
\exp_A(x) = 1 + e_A(x) = \sum_{n \geq 0} \frac{x^n}{n!} \quad \text{với } x \in G
$$
$$
\log_A(x) = l_A(x-1) = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad \text{với } x-1 \in G_1'
$$
(ta bỏ chỉ số $A$ khi không thể gây ra nhầm lẫn nào). Với $x \in G_R$ và $n \geq 1$,
$$
\left\| \frac{x^n}{n} \right\| \leq \left\| \frac{x^n}{n!} \right\| < R^n a^{-(n-1)\theta} = R \left( \frac{R}{a^\theta} \right)^{n-1}
$$
và do đó $e_A(G_R) \subset G_R$, $l_A(G_R) \subset G_R$ với $R \leq a^\theta$.

#### Mệnh đề 4 {#lie-ii-s8-prop-4 .statement}

*Cho $R$ là một số thực sao cho $0 < R \leq a^\theta$. Ánh xạ $\exp_A$ xác định một đẳng cấu giải tích từ $G_R$ lên $1 + G_R$ và đẳng cấu nghịch đảo là hạn chế của $\log_A$ trên $1 + G_R$.*

$e(l(X)) = l(e(X)) = X$. Theo (20), (21) và *Differentiable and Analytic Manifolds*, R, 4.1.5, ta suy ra rằng $e_A(l_A(x)) = l_A(e_A(x))$ với $x \in G_R$. Khi đó
$$
\exp_A(\log_A x) = x \quad \text{với } x \in 1 + G_R \\
\log_A(\exp_A x) = x \quad \text{với } x \in G_R
$$
điều này hoàn tất chứng minh.

Nếu $A$ được trang bị ngoặc $[x, y] = xy - yx$, thì $A$ trở thành một đại số Lie định chuẩn đầy đủ, vì $\|xy - yx\| \leq \sup(\|xy\|, \|yx\|) \leq \|x\| \cdot \|y\|$. Mệnh đề 2 của no. 3 suy ra rằng miền hội tụ tuyệt đối của $\tilde{H}$ chứa $G \times G$ và do đó $\tilde{H}$ xác định một hàm giải tích $h : G \times G \to A$; khi đó
$$
h(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y).
$$

#### Mệnh đề 5 {#lie-ii-s8-prop-5 .statement}

Với x, y trong G,
$$
\exp_A \cdot \exp_A y = \exp_A h(x, y).
$$
$e^{U e^V} = e^{H(U, V)}$ và do đó
$$
m \circ (1 + \tilde{\epsilon}, 1 + \tilde{\epsilon}) = (1 + \tilde{\epsilon}) \circ \tilde{H}
$$
trong $\tilde{H}(A \times A; A)$ (ở đây m ký hiệu phép nhân trên A). Khi đó mệnh đề suy ra từ Mệnh đề 2, Bổ đề 3 và Đa tạp khả vi và giải tích, R, 4.1.5.

### Bài tập {#lie-ii-s8-exercises}

Ta giả sử rằng đặc số thặng dư $p$ của trường $K$ là >0. Ta ký hiệu bởi $\mathfrak{o}_K$ vành của định giá $v$ của $K$.

Xem [các bài tập của § 8](exercises/s8/).
