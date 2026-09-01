---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 7
section_title: Convergence of the Hausdorff series (real or complex case)
lang: vi
source: lie-i-iii
pdf_pages: 0182-0188, 0222-0222
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS-POLYNOMIALS WITH VALUES IN $g$
      page: 0
      pdf_page: 182
    - "no": 2
      title: GROUP GERM DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 0
      pdf_page: 183
    - "no": 3
      title: Exponential in Complete Normed Associative Algebras
      page: 0
      pdf_page: 187
statements: 4
exercises: 1
content_sha256: 86b5141541e5b8d10194af725cf8d91bad5b6e269f3dd677223c592bef332e4f
translated_from: content/en/lie/II/07_s7_convergence_of_the_hausdorff_series.md
source_content_sha256: 0c070915f018ae2f28d7ba10eba8e260e6b24a97ffbf46012a1958fa6e91eda0
translation_model: gpt-5.4
translation_run: translate-vi-ae28c9b7
glossary_version: 34
glossary_terms_sha256: 8ad9d6d175450ba3b2b0568a212614a3a918364731e1112cb1a0dfd279ca2feb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. SỰ HỘI TỤ CỦA CHUỖI HAUSDORFF (TRƯỜNG HỢP THỰC HOẶC PHỨC)

Trong đoạn này ta giả sử rằng $K$ là một trong các trường $\mathbf{R}$ hoặc $\mathbf{C}$ với trị tuyệt đối thông thường của nó. Nhắc lại rằng một đại số chuẩn hóa được trên $K$ là một đại số trên $K$ (không nhất thiết kết hợp) với một tôpô $\mathcal{T}$ có các tính chất sau:
(1) $\mathcal{T}$ có thể được xác định bởi một chuẩn:
(2) ánh xạ $(x, y) \mapsto xy$ từ $A \times A$ vào $A$ là liên tục.
Một đại số định chuẩn trên $K$ là một đại số $A$ trên $K$ với một chuẩn sao cho $\|xy\| \leq \|x\|\ \|y\|$ với mọi $x, y$ trong $A$.
Ta ký hiệu bởi $g$ một đại số Lie chuẩn hóa được đầy đủ trên $K$. Ta chọn một chuẩn trên $g$ và một số $M > 0$ sao cho
$$
\|[x, y]\| \leq M \|x\|\ \|y\| \quad \text{với } x, y \text{ trong } g.
$$

### 1. CÁC *ĐA THỨC-LIÊN TỤC* NHẬN GIÁ TRỊ TRONG $g$

Cho $I$ là một tập hợp hữu hạn và gọi $P(g^I; g)$ (tương ứng $\hat{P}(g^I; g)$) là không gian vectơ các *đa thức-liên tục* (tương ứng *chuỗi lũy thừa hình thức có các thành phần liên tục*) trên $g^I$ nhận giá trị trong $g$. Nhắc lại (*Đa tạp khả vi và giải tích*, R, Phụ lục) rằng $P(g^I; g)$ có một phân bậc kiểu $\mathbf{N}^I$ và $\hat{P}(g^I; g)$ được đồng nhất với đầy đủ hóa của không gian vectơ $P(g^I; g)$ đối với tôpô được xác định bởi bộ lọc liên kết với phân bậc của $P(g^I; g)$. Hơn nữa, $P(g^I; g)$ là một đại số Lie phân bậc với dấu ngoặc được xác định bởi $[f, g](x) = [f(x), g(x)]$ với f, g thuộc P(g^I; g), x \in g^I; cấu trúc đại số Lie này có thể được mở rộng bằng tính liên tục lên $\hat{P}(g^I; g)$ và biến nó thành một đại số Lie lọc Hausdorff đầy đủ.

Theo mệnh đề 2 của § 6, no. 3, tồn tại một và chỉ một đồng cấu đại số Lie liên tục $\phi_I : u \mapsto \tilde{u}$ từ $\hat{L}(I)$ vào $\hat{P}(g^I; g)$ ánh xạ bất định nguyên có chỉ số i tới $\mathrm{pr}_i$ với mọi $i \in I$, vì $\mathrm{pr}_i \in P(g^I; g)$. Suy ra $\tilde{u} \in P(g^I; g)$ đối với $u \in L(I)$; chính xác hơn, khi $u \in L(I)$, $\tilde{u}$ chính là ánh xạ đa thức $(t_i) \mapsto u((t_i))$ của § 2, no. 4. Mặt khác, rõ ràng $\phi_I$ tương thích với các đa phân bậc của $L(I)$ và $P(g^I; g)$. Nếu $u = \sum_{v \in \mathbf{N}^I} u_v$, trong đó $u_v \in L^v(I)$ với $v \in \mathbf{N}^I$, thì

$$
\tilde{u} = \sum_{v \in \mathbf{N}^I} \tilde{u}_v, \quad \text{trong đó } \tilde{u}_v \in P_v(g^I; g).
$$

Cho $u = (u_j)_{j \in J}$ là một họ hữu hạn các phần tử của $\hat{L}(I)$, cho $v \in \hat{L}(J)$ và đặt $w = v \circ u$ (§ 6, no. 3). Ta viết $\tilde{u} = (\tilde{u}_j)_{j \in J} \in \mathfrak{g}$. Khi đó

(2)
$$
\tilde{v} \circ \tilde{u} = (v \circ u)^{\sim}.
$$

Điều này suy ra bằng cách mở rộng theo tính liên tục công thức (7) của § 6, no. 3 và từ Differentiable and Analytic Manifolds, R, phụ lục, no. 6.

### 2. MẦM NHÓM ĐƯỢC XÁC ĐỊNH BỞI MỘT ĐẠI SỐ LIE ĐỊNH CHUẨN ĐẦY ĐỦ

Cho $H = \sum_{r,s \geq 0} H_{r,s} \in \hat{L}(U, V)$ là chuỗi Hausdorff (§ 6, no. 4, Định nghĩa 1). Ta sẽ chỉ ra rằng chuỗi lũy thừa hình thức tương ứng

(3)
$$
\tilde{H} = \sum_{r,s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$

là hội tụ (Differentiable and Analytic Manifolds, R, 3.1.1).

Ta đưa vào chuỗi lũy thừa hình thức sau đây $\eta \in \mathbf{Q}[[U, V]]$

(4)
$$
\eta(U, V) = -\log(2 - \exp(U + V))
$$
(5)
$$
= \sum_{m \geq 1} \frac{1}{m} (\exp(U + V) - 1)^m
$$
(6)
$$
= \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1, \ldots, r_m \\ s_1, \ldots, s_m}} \frac{U^{r_1} V^{s_1}}{r_1!} \frac{U^{r_2} V^{s_2}}{r_2!} \cdots \frac{U^{r_m} V^{s_m}}{s_m!}.
$$

Do đó

(7)
$$
\eta(U, V) = \sum_{r,s \geq 0} \eta_{r,s} U^r V^s,
$$

trong đó
$$
\eta_{r,s} = \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_i + s_i \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
Bây giờ cho $u$ và $v$ là hai số thực dương sao cho $u + v < \log 2$; khi đó $0 \leq \exp(u + v) - 1 < 1$; các chuỗi dẫn xuất từ (5) và (6) bằng cách thay $u$ cho $U$ và $v$ cho $V$ là hội tụ và các tính toán trên cho thấy rằng
$$
\sum_{r, s \geq 0} \eta_{r,s} u^r v^s = -\log(2 - \exp(u + v)) < +\infty.
$$
Cho $r, s \geq 0$ và ký hiệu $\| \tilde{H}_{r,s} \|$ là chuẩn của đa thức liên tục $\tilde{H}_{r,s}$ (Differentiable and Analytic Manifolds, R, Phụ lục, no. 2).

#### Bổ đề 1 {#lie-ii-s7-lem-1 .statement}

$$
\| \tilde{H}_{r,s} \| \leq M^{r+s-1} \eta_{r,s}.
$$
Cho $r_i, s_i$ thuộc $\mathbf{N}$ với $1 \leq i \leq m$, và $s_m = 1$; đặt $r = \sum_i r_i, s = \sum_i s_i$ và xét phần tử sau của $L(\{U, V\})$:
$$
Z = \left( \left( \sum_{i=1}^{m-1} (\mathrm{ad}\ U)^{r_i} (\mathrm{ad}\ V)^{s_i} \right) (\mathrm{ad}\ U)^{r_m} \right)(V).
$$
Khi đó $\tilde{Z} = f \circ p$, trong đó $f$ là ánh xạ $(r+s)$-tuyến tính sau đây từ $g^{r+s}$ vào $g$:
$$
(x_1, \ldots, x_r, y_1, \ldots, y_s) \mapsto (\mathrm{ad}(x_1) \circ \cdots \circ \mathrm{ad}(x_r) \circ \mathrm{ad}(y_1) \circ \cdots \circ \mathrm{ad}(y_s))(y_s)
$$
và trong đó $p$ là ánh xạ sau đây từ $g^2$ vào $g^{r+s}$:
$$
(x, y) \mapsto (\underbrace{x, \ldots, x}_{r}, \underbrace{y, \ldots, y}_{s});
$$
do đó $\| \tilde{Z} \| \leq \| f \| \leq M^{r+s-1}$ (Đa tạp khả vi và giải tích, R, Phụ lục). Áp dụng các bất đẳng thức này cho các hạng tử khác nhau ở vế phải của công thức (9) ở § 6, no. 4, ta thu được:
$$
\|(H'_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
Một lập luận tương tự cho
$$
\|(H''_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_{m-1}! s_1! \ldots s_{m-1}!}
$$

do đó, theo (8)

$$
\|\tilde{H}_{r,s}\| < \eta_{r,s} \frac{M^{r+s-1}}{r+s} \leq \eta_{r,s} M^{r+s-1},
$$

điều đó chứng minh bổ đề.

#### Mệnh đề 1 {#lie-ii-s7-prop-1 .statement}

*Chuỗi lũy thừa hình thức* $\tilde{H}$ *là một chuỗi hội tụ* (*Differentiable and Analytic Manifolds*, R, 3.1.1); *miền hội tụ tuyệt đối của nó* (*Differentiable and Analytic Manifolds*, R, 3.1.4) *chứa tập mở*

$$
\Omega = \left\{ (x, y) \in g \times g \mid \|x\| + \|y\| < \frac{1}{M} \log 2 \right\}.
$$

Cho $u, v$ là hai số thực $> 0$ sao cho $u + v < \frac{1}{M} \log 2$; khi đó (Bổ đề 1)

$$
\text{(12)} \quad M \sum_{r,s \geq 0} \|\tilde{H}_{r,s}\| u^r v^s \\
\leq \sum_{r,s \geq 0} \eta_{r,s} M^{r+s} u^r v^s = -\log(2 - \exp M(u + v)) < +\infty
$$
theo (9).

Ký hiệu $h : \Omega \to g$ là *hàm giải tích* (*Differentiable and Analytic Manifolds*, R, 3.2.9) được xác định bởi $\tilde{H}$, tức là bởi công thức

$$
\text{(13)} \quad h(x, y) = \sum_{r,s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y) \quad \text{với } (x, y) \in \Omega.
$$

Hàm này được gọi là *hàm Hausdorff* của $g$ đối với $M$ (hoặc đơn giản là hàm Hausdorff của $g$ nếu không thể gây nhầm lẫn). Chú ý rằng $H_{r,s}(U, -U) = 0$ nếu $r + s \geq 2$ và do đó

$$
\text{(14)} \quad h(x, -x) = 0 \quad \text{với } \|x\| < \frac{1}{2M} \log 2.
$$

Tương tự,

$$
\text{(15)} \quad h(0, x) = h(x, 0) = x \quad \text{với } \|x\| < \frac{1}{M} \log 2.
$$

#### Mệnh đề 2 {#lie-ii-s7-prop-2 .statement}

*Đặt*

$$
\Omega' = \left\{ (x, y, z) \in g \times g \times g \mid \|x\| + \|y\| + \|z\| < \frac{1}{M} \log \frac{3}{2} \right\}.
$$

*Nếu* $(x, y, z) \in \Omega'$, *thì*

$$
\text{(16)} \quad (x, y) \in \Omega, \quad (h(x, y), z) \in \Omega, \quad (y, z) \in \Omega, \quad (x, h(y, z)) \in \Omega
$$
*và*
$$
\text{(17)} \quad h(h(x, y), z) = h(x, h(y, z)).
$$

Lấy $(x, y, z) \in \Omega'$; rõ ràng $(x, y) \in \Omega$ và $(y, z) \in \Omega$. Hơn nữa:

$$
\|h(x, y)\| \leq \sum_{r, s} \|H_{r,s}\| \|x|r\|y|s,
$$

và do đó theo (13)

$$
\|h(x, y)\| \leq -\frac{1}{M} \log(2 - \exp M(\|x\| + \|y\|)).
$$

Bây giờ $M(\|x\| + \|y\|) < \log \frac{3}{2} - M\|z\|$; ta đặt $u = \exp(M\|z\|)$; khi đó $1 \leq u \leq \frac{3}{2}$ và

$$
\begin{align*}
M(\|h(x, y)\| + \|z\|) &< -\log(2 - \exp(\log \frac{3}{2} - M\|z\|)) + M\|z\| \\
&= -\log\left(2 - \frac{3}{2u}\right) + \log u = \log \frac{2u^2}{4u - 3} \\
&= \log\left(2 + \frac{2(u - 1)(u - 3)}{4u - 3}\right) \leq \log 2.
\end{align*}
$$

Ta thấy tương tự rằng $(x, h(y, z)) \in \Omega$.

Bây giờ ta chứng minh (17). Trong đại số Lie $\hat{L}(\{U, V, W\})$,

$$
H(H(U, V), W) = H(U, H(V, W))
$$

theo Mệnh đề 4 của § 6, no. 5. Do đó, theo no. 1, công thức (2), ta có trong $\hat{P}(g \times g \times g, g)$ quan hệ

$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H}).
$$

Theo *Differentiable and Analytic Manifolds*, R, 3.1.9, tồn tại một số $\varepsilon > 0$ sao cho công thức (17) đúng khi $\|x\|, \|y\|$ và $\|z\|$ đều $\leq \varepsilon$. Nhưng các hàm $(x, y, z) \mapsto h(h(x, y), z)$ và $(x, y, z) \mapsto h(x, h(y, z))$ là các hàm giải tích trên $\Omega'$ với giá trị trong $g$ (*Differentiable and Analytic Manifolds*, R, 3.2.7). Vì $\Omega'$ liên thông và chúng trùng nhau trong một lân cận của 0, nên chúng bằng nhau (*Differentiable and Analytic Manifolds*, R, 3.2.5).

Các kết quả trên kéo theo:

Cho $\alpha$ là một số thực sao cho $0 < \alpha \leq \frac{1}{3M} \log \frac{3}{2}$. Đặt

$$
G = \{x \in g \mid \|x\| < \alpha\},
$$

$$
\Theta = \{(x, y) \in G \times G \mid h(x, y) \in G\}
$$
và $m : \Theta \to G$ là hạn chế của $h$ lên $\Theta$. Khi đó:
(1) $\Theta$ là mở trong $G \times G$ và $m$ là giải tích.
(2) $x \in G$ kéo theo $(0, x) \in \Theta$, $(x, 0) \in \Theta$ và $m(0, x) = m(x, 0) = x$.
(3) $x \in G$ kéo theo $-x \in G$, $(x, -x) \in \Theta$, $(-x, x) \in \Theta$ và

$$
m(x, -x) = m(-x, x) = 0.
$$

(4) Cho x, y, z là các phần tử của G sao cho (x, y) ∈ Θ, (m(x, y), z) ∈ Θ, (y, z) ∈ Θ và (x, m(y, z)) ∈ Θ. Khi đó m(m(x, y), z) = m(x, m(y, z)).

*Nói cách khác (Chương III, § 1), nếu ta viết −x = σ(x), thì bộ bốn (G, 0, σ, m) là một mầm nhóm Lie trên K.*

### 3. Hàm mũ trong các đại số kết hợp có đơn vị định chuẩn đầy đủ

Trong số này, ta ký hiệu bởi A một đại số kết hợp có đơn vị định chuẩn đầy đủ (Tôpô đại cương, Chương IX, § 3, no. 7). Khi đó \|x.y\| ≤ \|x\|. \|y\| với x, y trong A.

Cho I là một tập hợp hữu hạn và gọi $\hat{P}(A^I; A)$ là không gian vectơ các chuỗi lũy thừa hình thức có các thành phần liên tục trên $A^I$ nhận giá trị trong A (Đa tạp khả vi và giải tích, R, Phụ lục, no. 5), với cấu trúc đại số thu được bằng cách viết

$$
f.g = m \circ (f, g) \quad \text{với } f, g \text{ trong } \hat{P}(A^I; A),
$$

trong đó $m : A \times A \to A$ ký hiệu phép nhân trên A. Lập luận như trong no. 1 và dùng Mệnh đề 1 của § 5, no. 1, ta định nghĩa một đồng cấu liên tục của các đại số có đơn vị $u \mapsto \tilde{u}$ từ $\hat{A}(I)$ vào $\hat{P}(A^I; A)$ biến ẩn bất định có chỉ số i thành $pr_i$; đồng cấu này mở rộng đồng cấu đại số Lie từ $\hat{L}(I)$ vào $\hat{P}(A^I; A)$ được định nghĩa trong no. 1. Nếu $u = \sum_v u_v$ với $u_v \in A^v(I)$ đối với $v \in \mathbf{N}^I$, thì $\tilde{u} = \sum_v \tilde{u}_v$, trong đó $\tilde{u}_v$ là ánh xạ đa thức $(t_i)_{i \in I} \mapsto u_v((t_i))$.

Cho $u = (u_j)_{j \in I}$ là một họ hữu hạn các phần tử của $\hat{A}(I)$, cho $v \in \hat{A}(J)$ và viết $w = v \circ u$ (§ 5, no. 1). Khi đó

$$
(v \circ u)^{\sim} = \tilde{v} \circ \tilde{u}.
$$

Điều này suy ra bằng cách kéo dài theo tính liên tục công thức (2) của § 5, no. 1 và từ Differentiable and Analytic Manifolds, R, phụ lục, no. 6.

Đặc biệt, ta lấy I = {U}, đồng nhất A với $A^{(U)}$ và xét các ảnh $\tilde{e}$ và $\tilde{l}$ của các chuỗi $e(U) = \sum_{n \geq 1} U^n/n!$ và $l(U) = \sum_{n \geq 1} (-1)^{n-1} U^n/n$ trong $\hat{P}(A; A)$. Khi đó $\|\tilde{U}^n\| \leq 1$ vì $\|x_1 \ldots x_n\| \leq \|x_1\| \ldots \|x_n\|$ với $x_1, \ldots, x_n$ trong A. Do đó bán kính hội tụ tuyệt đối của $\tilde{e}$ (tương ứng của $\tilde{l}$) là vô hạn (tương ứng $\geq 1$).

Ta sẽ ký hiệu bởi $e_A$ (tương ứng $l_A$) ánh xạ giải tích của A vào A (tương ứng của B vào A, trong đó B là quả cầu đơn vị mở của A) được xác định bởi chuỗi hội tụ $\tilde{e}$ (tương ứng $\tilde{l}$), và ta sẽ viết $\exp_A(x) = 1 + e_A(x)$ (với $x \in A$) và

$$
\log_A(x) = l_A(x - 1)
$$

(với $x \in A, \|x - 1\| < 1$). Khi đó

$$
\exp_A x = \sum_{n \geq 0} \frac{x^n}{n!} \quad (x \in A)
$$

(20)    $\log_A x = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad (x \in A, \|x-1\| < 1).$

Vì $(e \circ l)(U) = (l \circ e)(U) = U$ (x. § 6, no. 1), theo (18) ta có $\tilde{e} \circ \tilde{l} = \tilde{l} \circ \tilde{e} = \mathrm{Id}_A$.
Do đó (*Differentiable and Analytic Manifolds*, R, 3.1.9)
(21)    $\exp_A(\log_A(x)) = x \quad (x \in A, \|x-1\| \leq 1)$
(22)    $\log_A(\exp_A(x)) = x \quad (x \in A, \|x\| < \log 2)$
vì với $\|x\| < \log 2$ thì suy ra $\|\exp_A(x) - 1\| \leq \exp \|x\| - 1 < 1$.

Cuối cùng ta xét A như một đại số Lie chuẩn đầy đủ. Khi đó
$$
\|[x, y]\| = \|xy - yx\| \leq 2\|x\|\cdot\|y\|.
$$
Mệnh đề 1 của no. 2 suy ra rằng miền hội tụ tuyệt đối của chuỗi lũy thừa hình thức $\tilde{H}$ chứa tập hợp
$$
\Omega = \{x, y) \in A \times A \mid \|x\| + \|y\| < \frac{1}{2} \log 2\}.
$$
Do đó $\tilde{H}$ xác định một hàm giải tích $h : \Omega \to A$. Khi đó $h(x, y) = \sum_{r,s} H_{r,s}(x, y)$ (x. § 3, no. 1, *Nhận xét 4*).

#### Mệnh đề 3 {#lie-ii-s7-prop-3 .statement}

*Với $\|x\| + \|y\| < \frac{1}{2} \log 2$,*
(23)    $\exp_A x \cdot \exp_A y = \exp_A h(x, y).$
Từ (18) và quan hệ $e^u e^v = e^{u+v}$ suy ra rằng
$$
m \circ (1 + \tilde{e}, 1 + \tilde{e}) = (1 + \tilde{e}) \circ \tilde{H}
$$
trong $\hat{P}(A \times A; A)$. Do đó suy ra từ *Differentiable and Analytic Manifolds*, R, 3.1.9 rằng (23) đúng với $(x, y)$ đủ gần $(0, 0)$, do đó mệnh đề được suy ra bằng phép kéo dài giải tích (*Differentiable and Analytic Manifolds*, R, 3.2.5).

### Bài tập {#lie-ii-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
