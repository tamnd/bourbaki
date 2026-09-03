---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 3
section_title: Enveloping algebra of the free Lie algebra
lang: vi
source: lie-i-iii
book_pages: 136-142, 186-187
pdf_pages: 0154-0160, 0204-0205
extraction: ocr
subsections:
    - "no": 1
      title: ENVELOPING ALGEBRA OF $L(X)$
      page: 136
      pdf_page: 154
    - "no": 2
      title: PROJECTOR OF $A^+(X)$ ONTO $L(X)$
      page: 138
      pdf_page: 156
    - "no": 3
      title: DIMENSION OF THE HOMOGENEOUS COMPONENTS OF L(X)
      page: 140
      pdf_page: 158
statements: 11
exercises: 4
content_sha256: 7a02ca5a27c070db9f21c3ab55245511c6cbc69c5fedcbbb2e5561d20f7890a4
translated_from: content/en/lie/II/03_s3_enveloping_algebra_of_the_free_lie.md
source_content_sha256: 9132123acdc022535dc3e655ef1016236c6b0beebc316f3a60900b058de3ac4a
translation_model: gpt-5.4
translation_run: translate-vi-82c9aeec
glossary_version: 34
glossary_terms_sha256: 39d33b47eea43a06d602be3f4a37c642dafd484e27e30163409d21b3f50e1a8b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐẠI SỐ BAO CỦA ĐẠI SỐ LIE TỰ DO

Trong tiết này, $A(X) = A_K(X)$ ký hiệu đại số kết hợp tự do Libas(X) của tập hợp $X$ trên vành $K$ (Đại số, Chương III, § 2, no. 7, Định nghĩa 2). Đồng nhất $X$ với ảnh chính tắc của nó trong $A(X)$; nhắc lại rằng K-môđun $A(X)$ nhận monoit tự do $Mo(X)$ dẫn xuất từ $X$ làm cơ sở; $A^+(X)$ ký hiệu môđun con của $A(X)$ sinh bởi các từ khác rỗng.

### 1. ĐẠI SỐ BAO CỦA $L(X)$

#### Định lý 1 {#lie-ii-s3-thm-1 .statement}

*Cho* $\alpha : L(X) \to A(X)$ *là đồng cấu đại số Lie duy nhất kéo dài đơn ánh chính tắc của* $X$ *vào* $A(X)$ *(§ 2, no. 2, Mệnh đề 1)*. *Cho* $\sigma : L(X) \to U(L(X))$ là ánh xạ chính tắc của $L(X)$ vào đại số bao của nó và $\beta : U(L(X)) \to A(X)$ là đồng cấu đại số có đơn vị duy nhất sao cho $\beta \circ \sigma = \alpha$ (Chương I, § 2, no. 1, Mệnh đề 1). Khi đó:
(a) $\alpha$ là đơn ánh và $\alpha(L(X))$ là một môđun con hạng tử trực tiếp của $A(X)$.
(b) $\beta$ là song ánh.

Cho B là một K-đại số có đơn vị và $\phi$ là một ánh xạ từ X vào B; theo Mệnh đề 1 của § 2, no. 2, tồn tại một đồng cấu đại số Lie $\psi : L(X) \to B$ sao cho $\psi | X = \phi$; theo Mệnh đề 1 của Chương I, § 2, no. 1, tồn tại một đồng cấu đại số có đơn vị $\theta : U(L(X)) \to B$ sao cho $\theta \circ \sigma = \psi$ và do đó sao cho $(\theta \circ \sigma) | X = \phi$. Vì $\sigma(X)$ sinh đại số có đơn vị $U(L(X))$, đồng cấu $\theta$ là đồng cấu đại số có đơn vị duy nhất thỏa mãn điều kiện sau cùng. Điều này cho thấy cặp có thứ tự $(U(L(X)), \sigma | X)$ là một nghiệm của cùng bài toán ánh xạ phổ quát như $A(X)$; lấy $\phi$ là đơn ánh chính tắc của X vào $A(X)$, ta suy ra rằng $\beta$ là một đẳng cấu, điều này chứng minh (b).

Sau cùng, vì $L(X)$ là một K-môđun tự do (§ 2, no. 11, Hệ quả của Định lý 1), $\sigma$ là đơn ánh và $\sigma(L(X))$ là một môđun con hạng tử trực tiếp của $U(L(X))$ (Chương I, § 2, no. 7, Hệ quả 3 của Định lý 1). Theo (b), điều này chứng minh (a).

#### Hệ quả 1 {#lie-ii-s3-thm-1-cor-1 .statement}

Tồn tại trên đại số $A(X)$ một đồng tích duy nhất biến $A(X)$ thành một đại số kép sao cho các phần tử của X là nguyên thủy. Hơn nữa, $\beta$ là một đẳng cấu từ đại số kép $U(L(X))$ lên $A(X)$ được trang bị cấu trúc đại số kép này.

Điều này suy ra từ mệnh đề (b) của định lý và từ việc X sinh đại số có đơn vị $A(X)$.

Từ nay, $A(X)$ được trang bị cấu trúc đại số kép này và $L(X)$ được đồng nhất với ảnh của nó dưới $\alpha$, tức là với đại số con Lie của $A(X)$ sinh bởi X.

#### Hệ quả 2 {#lie-ii-s3-thm-1-cor-2 .statement}

Nếu $K$ là một trường có đặc số 0, thì $L(X)$ là đại số Lie của các phần tử nguyên thủy của $A(X)$.

Điều này suy ra từ Hệ quả 1 và Hệ quả của Mệnh đề 9 của § 1, no. 5.

#### Nhận xét {#lie-ii-s3-n1-rem-1 .statement}

(1) Cho $K'$ là một vành giao hoán chứa K. Nếu $A(X)$, $L(X)$ và $L_{K'}(X)$ được đồng nhất với các tập con của $A_{K'}(X)$, thì từ phần (a) của Định lý 1 ta suy ra quan hệ

$$
L(X) = L_{K'}(X) \cap A(X).
$$

(2) Hệ quả 2 của Định lý 1 vẫn đúng nếu chỉ giả thiết rằng nhóm cộng của vành K là không xoắn. Thật vậy, trước hết giả sử $K = \mathbf{Z}$; mọi phần tử nguyên thủy của $A(X)$ là một phần tử nguyên thủy của $A_q(X)$ và do đó thuộc $L_q(X) \cap A(X) = L(X)$ (Hệ quả 2 và công thức (1)). Trong trường hợp tổng quát, K là phẳng trên $\mathbf{Z}$ và ta áp dụng Nhận xét 2 của § 1, no. 2 và Mệnh đề 3 của § 2, no. 5.

(3) Cho $\Delta$ là một monoid giao hoán, $\phi_0$ một ánh xạ từ $X$ vào $\Delta$ và $\phi : Mo(X) \to \Delta$ là đồng cấu của monoid liên kết; nếu $A(X)$ được cho phân bậc $(A^\delta(X))_{\delta \in \Delta}$ được định nghĩa trong *Algebra*, Chương III, § 3, no. 1, *Ví dụ* 3 và $L(X)$ phân bậc $(L^\delta(X))_{\delta \in \Delta}$ được định nghĩa trong § 2, no. 6, thì ta có ngay lập tức, với $\delta \in \Delta$, $L^\delta(X) \subset L(X) \cap A^\delta(X)$. Vì $L$ là tổng của các $L^\delta(X)$ với $\delta \in \Delta$, và tổng của các $L(X) \cap A^\delta(X)$ với $\delta \in \Delta$ là trực tiếp, điều đó suy ra

$$
L^\delta(X) = L(X) \cap A^\delta(X).
$$

(4) Cho $A$ là một đại số kết hợp có đơn vị và $t = (t_i)_{i \in I}$ một họ các phần tử của $A$. Ta có một biểu đồ

$$
\begin{array}{ccc}
L(I) & \xrightarrow{f_t} & A \\
i \downarrow & & \downarrow g_t \\
A(I)
\end{array}
$$

trong đó $i$ là đơn ánh chính tắc, $f_t$ là đồng cấu đại số Lie được xác định bởi $t$ và $g_t$ là đồng cấu đại số có đơn vị sao cho $g_t(i) = t_i$ với $i \in I$. Biểu đồ là giao hoán vì $g_t \circ i$ và $f_t$ trùng nhau trên $I$. Suy ra rằng nếu $P \in L(I)$, phần tử $P((t_i)_{i \in I})$ được định nghĩa trong § 2, no. 4 trùng với phần tử $P((t_i)_{i \in I})$ được định nghĩa trong *Algebra*, Chương III, § 2, no. 8, *Ví dụ* 2.

### 2. PHÉP CHIẾU CỦA $A^+(X)$ LÊN $L(X)$

Cho $\pi$ là ánh xạ tuyến tính từ $A^+(X)$ vào $L(X)$ được định nghĩa bởi

$$
\pi(x_1 \ldots x_n) = (\operatorname{ad}(x_1) \circ \cdots \circ \operatorname{ad}(x_{n-1}))(x_n)
$$

với $n > 0, x_1, \ldots, x_n$ trong $X$.

#### Mệnh đề 1 {#lie-ii-s3-prop-1 .statement}

(a) *Hạn chế $\pi_0$ của $\pi$ lên $L(X)$ là một đạo hàm của $L(X)$.*
(b) *Với mọi số nguyên $n \geq 1$ và mọi $u$ trong $L^n(X)$, $\pi(u) = n.u$.*

(a) Cho $E$ là đại số tự đồng cấu của môđun $L(X)$ và $\theta$ là đồng cấu của $A(X)$ vào $E$ sao cho $\theta(x) = \operatorname{ad} x$ với mọi $x \in X$. Hạn chế của $\theta$ lên $L(X)$ là một đồng cấu đại số Lie của $L(X)$ vào $E$, trùng trên $X$ với biểu diễn phụ hợp của $L(X)$, do đó

$$
\theta(u).v = [u, v] \quad \text{với } u, v \text{ trong } L(X).
$$

Cho $a$ thuộc $A(X)$ và $b$ thuộc $A^+(X)$; khi đó

$$
\pi(a.b) = \theta(a).\pi(b).
$$

Chỉ cần xét trường hợp $a = x_1 \ldots x_p, \ b = x_{p+1} \ldots x_{p+q}$ với $p \geq 0, q \geq 1$ và $x_1, \ldots, x_{p+q}$ thuộc $X$; nhưng khi đó (5) suy ra ngay lập tức từ (3) vì $\theta(x) = \operatorname{ad} x$ với $x \in X$.

Cho $u$ và $v$ thuộc $L(X)$; theo (4) và (5),

$$
\pi_0([u, v]) = \pi(uv - vu) = \theta(u) \cdot \pi(v) - \theta(v) \cdot \pi(u)
= [u, \pi(v)] - [v, \pi(u)] = [u, \pi_0(v)] + [\pi_0(u), v],
$$

vậy $\pi_0$ là một đạo hàm của $L(X)$.

(b) Cho $\pi_1$ là tự đồng cấu của môđun $L(X)$ trùng trên $L^n(X)$ với phép nhân bởi số nguyên $n \geq 1$. Công thức $[L^n(X), L^m(X)] \subset L^{n+m}(X)$ cho thấy rằng $\pi_1$ là một đạo hàm (*Đại số*, Chương III, § 10, no. 3, *Ví dụ* 6). Đạo hàm $\pi_1 - \pi_0$ của $L(X)$ bằng không trên $X$ và, vì $X$ sinh ra $L(X)$, nên $\pi_0 = \pi_1$, do đó suy ra (b).

#### Hệ quả {#lie-ii-s3-n2-cor-1 .statement}

*Giả sử K là một Q-đại số. Cho P là ánh xạ tuyến tính của $A^+(X)$ vào chính nó sao cho*

$$
P(x_1 \ldots x_n) = \frac{1}{n} (\operatorname{ad} x_1 \circ \cdots \circ \operatorname{ad} x_{n-1})(x_n)
$$

*với $n \geq 1$ và $x_1, \ldots, x_n$ thuộc X. Khi đó P là một phép chiếu của $A^+(X)$ lên $L(X)$.*

Ảnh của P được chứa trong $L(X)$. Hơn nữa, với mọi $n \geq 1$ và mọi $u$ thuộc $L^n(X)$, $P(u) = \frac{1}{n} \pi(u)$, do đó $P(u) = u$ theo Mệnh đề 1. Vì

$$
L(X) = \sum_{n \geq 1} L^n(X),
$$

ta thấy hạn chế của P lên $L(X)$ là đồng nhất.

#### Nhận xét {#lie-ii-s3-n2-rem-1 .statement}

Giả sử rằng K là một trường có đặc số không và gọi Q là phép chiếu của $A(X) = U(L(X))$ lên $L(X)$ liên kết với phân bậc chính tắc của $U(L(X))$, xem § 1, no. 5. *Với $\alpha \in \mathbf{N}^{(X)}$, $Q(A^\alpha(X)) \subset L^\alpha(X)$.* Thật vậy, chỉ cần kiểm tra rằng ảnh và hạt nhân của Q là các môđun con phân bậc của $A(X)$ đối với phân bậc kiểu $\mathbf{N}^{(X)}$. Điều này là hiển nhiên đối với ảnh, vốn bằng $L(X)$. Mặt khác, gọi $n$ là một số nguyên $\geq 1$. Không gian con vectơ của $A(X)$ sinh bởi các $y^n$, trong đó $y \in L(X)$, bằng không gian con vectơ của $A(X)$ sinh bởi các $\sum_{\sigma \in S_n} y_{\sigma(1)} y_{\sigma(2)} \cdots y_{\sigma(n)}$, trong đó $y_1, y_2, \ldots, y_n$ là các phần tử thuần nhất của $L(X)$; do đó không gian con này là một môđun con phân bậc của $A(X)$.

(Xin chú ý rằng, nếu Card(X) $\geq 2$, thì các phép chiếu P và Q *không trùng nhau* trên $A^+(X)$. Thật vậy, lấy $x, y$ trong X với $x \neq y$ và viết

$$
z = x[x, y] + [x, y]x = x^2y - yx^2.
$$

Khi đó $Q(z) = 0$ và $P(z) = \frac{1}{3}[x, [x, y]] \neq 0$, xem § 2, no. 10, *Ví dụ* và no. 11, *Định lý* 1.)

### 3. CHIỀU CỦA CÁC THÀNH PHẦN THUẦN NHẤT CỦA L(X)

Cho X là một tập hợp, $\alpha$ là một phần tử của $\mathbf{N}^{(X)}$ và d là một số nguyên > 0. Ta viết $d|\alpha$ nếu tồn tại $\beta \in \mathbf{N}^{(X)}$ sao cho $\alpha = d\beta$. Phần tử $\beta$, là duy nhất, khi đó được ký hiệu là $\alpha/d$.

#### Bổ đề 1 {#lie-ii-s3-lem-1 .statement}

Cho n là một số nguyên > 0, $T_1, \ldots, T_n$ là các bất định và $u_1, \ldots, u_n$ là các phần tử của $\mathbf{Z}$. Cho $(c(\alpha))_{\alpha \in \mathbf{N}^n - \{0\}}$ là một họ các phần tử của $\mathbf{Z}$ sao cho

$$
1 - \sum_{i=1}^n u_i T_i = \prod_{\alpha \neq 0} (1 - T^\alpha)^{c(\alpha)}.
$$

Với mọi $\alpha \in \mathbf{N}^n - \{0\}$,

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!} u^{\alpha/d}
$$

trong đó $\mu$ là hàm Möbius (phụ lục).

Công thức (7) tương đương, sau khi lấy lôgarit hai vế (Đại số, Chương IV, § 6, no. 9), với:

$$
\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha).
$$

Bây giờ

$$
-\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{j \geq 1} \frac{1}{j} \left( \sum_{i=1}^n u_i T_i \right)^j
$$
$$
= \sum_{j \geq 1} \frac{1}{j} \sum_{|\beta|=j} \frac{|\beta|!}{\beta!} u^\beta T^\beta
$$
$$
= \sum_{|\beta|>0} \frac{1}{|\beta|} \frac{|\beta|!}{\beta!} u^\beta T^\beta.
$$

Mặt khác

$$
-\sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha) = \sum_{|\alpha|>0, k \geq 1} \frac{1}{k} c(\alpha) T^{k\alpha}
$$
$$
= \sum_{|\beta|>0, k|\beta} \frac{1}{k} c\left( \frac{\beta}{k} \right) T^\beta.
$$

Vậy (7) tương đương với

$$
\sum_{k|\beta} \left| \frac{\beta}{k} \right| c\left( \frac{\beta}{k} \right) = \frac{|\beta|!}{\beta!} u^\beta \quad \text{với mọi } \beta \in \mathbf{N}^n - \{0\}.
$$

Gọi $\Lambda$ là tập hợp các $(\lambda_1, \lambda_2, \ldots, \lambda_n) \in \mathbf{N}^n - \{0\}$ sao cho ước số chung lớn nhất của $\lambda_1, \lambda_2, \ldots, \lambda_n$ bằng 1. Mọi phần tử của $\mathbf{N}^n - \{0\}$ đều có thể được viết duy nhất dưới dạng $m\lambda$, trong đó $m$ là một số nguyên $\geqslant 1$ và $\lambda \in \Lambda$. Điều kiện (12) tương đương với

$$
\sum_{k|m} \left| \frac{m\lambda}{k} \right| c\left( \frac{m\lambda}{k} \right) = \frac{(m|\lambda|)!}{(m\lambda)!} u^{m\lambda} \quad \text{với mọi } \lambda \in \Lambda \text{ và mọi } m \geqslant 1.
$$

Theo công thức đảo Möbius (phụ lục), điều kiện (13) tương đương với

$$
|m\lambda| c(m\lambda) = \sum_{d|m} \mu(d) \frac{\left| \frac{m\lambda}{d} \right|!}{\left( \frac{m\lambda}{d} \right)!} u^{\frac{m\lambda}{d}}
$$

với mọi $\lambda \in \Lambda$ và mọi $m \geqslant 1$.

#### Định lý 2 {#lie-ii-s3-thm-2 .statement}

*Cho $X$ là một tập hợp hữu hạn và $n = \mathrm{Card}(X)$.*

(a) *Với mọi số nguyên $r \geqslant 1$, $K$-môđun $L^r(X)$ là tự do hạng*

$$
c(r) = \frac{1}{r} \sum_{d|r} \mu(d) n^{r/d},
$$

*trong đó $\mu$ là hàm Möbius.*

(b) *Với mọi $\alpha \in \mathbf{N}^X - \{0\}$, $K$-môđun $L^\alpha(X)$ (§ 2, no. 6) là tự do hạng*

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!}.
$$

Ta đã biết rằng các môđun $L^r(X)$, với $r \in \mathbf{N}$, và $L^\alpha(X)$, với $\alpha \in \mathbf{N}^X$, đều là tự do (§ 2, no. 11, Hệ quả của Định lý 1). Xét đa phân bậc $(A^\alpha(X))_{\alpha \in \mathbf{N}^X}$ của $A(X)$ được xác định bởi đồng cấu chính tắc $\phi$ từ $Mo(X)$ vào $\mathbf{N}^X$ (*Algebra*, Chương III, § 3, no. 1, *Ví dụ 3*); khi đó $A^\alpha(X) \cap L(X) = L^\alpha(X)$ theo *Nhận xét 3* của no. 1. Với $\alpha \in \mathbf{N}^X$, $K$-môđun $A^\alpha(X)$ nhận làm cơ sở tập hợp các từ trong đó mỗi chữ cái $x$ của $X$ xuất hiện $\alpha(x)$ lần. Gọi $d(\alpha)$ là số các từ đó, tức là hạng của $A^\alpha(X)$; ta sẽ tính theo hai cách khác nhau chuỗi lũy thừa hình thức

$$
P((T_x)_{x \in X}) \in \mathbf{Z}[[((T_x)_{x \in X})]]
$$

được xác định bởi

$$
P(T) = \sum_{\alpha \in \mathbf{N}^X} d(\alpha) T^\alpha.
$$

(1) Ta có

$$
P(T) = \sum_{m \in Mo(X)} T^{\phi(m)} = \sum_{r=0}^\infty \sum_{x_1, \ldots, x_r} T_{x_1} \cdots T_{x_r} = \sum_{r=0}^\infty \left( \sum_{x \in X} T_x \right)^r
$$

do đó

$$
P(T) = \left( 1 - \sum_{x \in X} T_x \right)^{-1}.
$$

(2) Với mọi $\alpha \in \mathbf{N}^X - \{0\}$, lấy $(e_{\alpha,j})_{1 \leq j \leq c(\alpha)}$ là một cơ sở của $L^\alpha(X)$ và trang bị cho tập $I$ các cặp có thứ tự $(\alpha, j)$ sao cho $\alpha \in \mathbf{N}^X - \{0\}$ và $1 \leq j \leq c(\alpha)$ một thứ tự toàn phần. Theo Định lý 1 của no. 1 và Định lý Poincaré–Birkhoff–Witt (Chương I, § 2, no. 7, Hệ quả 3 của Định lý 1), các phần tử
$$
y_m = \prod_{(\alpha, j) \in I} (e_{\alpha, j})^{m(\alpha, j)},
$$
trong đó chỉ số $m$ chạy qua $\mathbf{N}^{(I)}$, tạo thành một cơ sở của $A(X)$. Mỗi $y_m$ có đa bậc $\sum_{(\alpha, j) \in I} m(\alpha, j) \alpha$. Gọi $u(m)$ là đa bậc này. Suy ra
$$
P(T) = \sum_{m \in \mathbf{N}^{(I)}} T^{u(m)} = \sum_{m \in \mathbf{N}^{(I)}} \prod_{(\alpha, j) \in I} T^{m(\alpha, j)\alpha}
= \prod_{(\alpha, j) \in I} \sum_{r=0}^\infty T^{r\alpha} = \prod_{(\alpha, j) \in I} (1 - T^\alpha)^{-1},
$$
do đó cuối cùng
$$
P(T) = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{-c(\alpha)}.
$$
So sánh (18) và (19), ta được
$$
1 - \sum_{x \in X} T_x = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{c(\alpha)}.
$$
Bổ đề 1 khi đó cho (b).

Nếu bây giờ ta thay cùng một ẩn số $U$ vào chỗ các $T_x$ với $x \in X$ trong công thức (20), ta được
$$
1 - nU = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - U^{|\alpha|})^{c(\alpha)} = \prod_{r > 0} (1 - U^r)^{c(r)}.
$$
Áp dụng Bổ đề 1 một lần nữa, ta suy ra (a).

#### Ví dụ {#lie-ii-s3-n3-exa-1 .statement}

Ta có
$$
\begin{align*}
c(1) &= n, & c(2) &= \frac{1}{2}(n^2 - n), & c(3) &= \frac{1}{3}(n^3 - n), \\
c(4) &= \frac{1}{4}(n^4 - n^2), & c(5) &= \frac{1}{5}(n^5 - n), & c(6) &= \frac{1}{6}(n^6 - n^3 - n^2 + n).
\end{align*}
$$

#### Nhận xét {#lie-ii-s3-n3-rem-1 .statement}

Cho $X$ là một tập hợp và cho $\alpha \in \mathbf{N}^{(X)}$; hạng của $K$-môđun tự do $L^\alpha(X)$ cũng được cho bởi công thức (16). Điều này suy ra ngay lập tức từ Định lý 2 (b) và Mệnh đề 4 của § 2, no. 6.

### Bài tập {#lie-ii-s3-exercises}

Chữ cái $X$ chỉ một tập hợp.

Xem [bài tập của § 3](exercises/s3/).
