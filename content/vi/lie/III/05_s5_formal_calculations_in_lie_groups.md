---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 5
section_title: Formal calculations in Lie groups
lang: vi
source: lie-i-iii
pdf_pages: 0315-0322, 0400-0401
extraction: ocr
subsections:
    - "no": 1
      title: THE COEFFICIENTS $c_{\alpha \beta \gamma}$
      page: 0
      pdf_page: 315
    - "no": 2
      title: BRACKET IN THE LIE ALGEBRA
      page: 0
      pdf_page: 316
    - "no": 3
      title: POWERS
      page: 0
      pdf_page: 318
    - "no": 4
      title: EXPONENTIAL
      page: 0
      pdf_page: 321
statements: 5
exercises: 2
content_sha256: fd44041a354b12ad1414a3c2e7cc1c0cf6a3db3a0486ddf23cbd7ffec81830fb
translated_from: content/en/lie/III/05_s5_formal_calculations_in_lie_groups.md
source_content_sha256: cd937d983bc405d657b449070d2500d889e40909800ae25e3707f9d043c12bc7
translation_model: gpt-5-6-mini
translation_run: translate-vi-09d05e9d
glossary_version: 34
glossary_terms_sha256: 600febf89207a5120dca7932fbb36aa15d83f9401003c8ca08e7308dc30f45ce
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC PHÉP TÍNH HÌNH THỨC TRONG CÁC NHÓM LIE

Cho $f, g$ là hai chuỗi lũy thừa hình thức với các hệ số trong $K$ theo cùng các biến bất định, cho $f_i$ (tương ứng $g_i$) là thành phần thuần nhất của $f$ (tương ứng $g$) có bậc $i$. Ta sẽ viết
$$
f \equiv g \mod \deg p
$$
nếu $f_i = g_i$ với $i < p$.

Trong § này, G ký hiệu một mầm nhóm Lie số chiều hữu hạn $n$; trường cơ sở $K$ được giả thiết có đặc số không. Ta đồng nhất một lần cho tất cả, bằng một biểu đồ, một lân cận mở của $e$ trong G với một lân cận mở U của 0 trong $K^n$, sao cho $e$ được đồng nhất với 0. Với $x, y$ trong U và $n \in \mathbf{Z}$, $x.y$ ký hiệu tích của $x$ và $y$ và $x^{[m]}$ là lũy thừa thứ m của $x$ trong G (khi chúng được xác định). Các tọa độ của $x \in U$ được ký hiệu bởi $x_1, x_2, \ldots, x_n$.

### 1. CÁC HỆ SỐ $c_{\alpha \beta \gamma}$

Cho $\Omega$ là tập hợp các $(x, y) \in U \times U$ sao cho $x.y$ được xác định và thuộc U. Khi đó $\Omega$ là mở trong $U \times U$ và ánh xạ $(x, y) \mapsto x.y$ của $\Omega$ vào U là giải tích. Do đó các tọa độ $z_1, \ldots, z_n$ của $z = x.y$ cho phép các khai triển thành chuỗi nguyên quanh gốc theo các lũy thừa của $x_1, \ldots, x_n, y_1, \ldots, y_n$. Vì vậy, tồn tại các hằng số xác định rõ $c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} \in K$, sao cho
$$
z_1^{\gamma_1} \cdots z_n^{\gamma_n} = \sum_{\alpha_1, \ldots, \beta_n \in \mathbf{N}} c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} x_1^{\alpha_1} \cdots x_n^{\alpha_n} y_1^{\beta_1} \cdots y_n^{\beta_n}
$$
với $\gamma_1, \ldots, \gamma_n$ trong $\mathbf{N}$. Theo các quy ước của *Đa tạp khả vi và giải tích*, R, ta sẽ viết các công thức này ngắn gọn hơn:
$$
(x.y)^{\gamma} = \sum_{\alpha, \beta \in \mathbf{N}^n} c_{\alpha, \beta, \gamma} x^{\alpha} y^{\beta} \quad (\gamma \in \mathbf{N}^n).
$$
Vì $x.0 = 0.x = x$ với $x \in U$,
$$
c_{\alpha, 0, \gamma} = c_{0, \alpha, \gamma} = \delta_{\alpha \gamma}
$$
trong đó $\delta_{\alpha \gamma}$ là chỉ số Kronecker. Đặc biệt, từ nay viết $k$ thay cho $\varepsilon_k$ với $k = 1, \ldots, n$,
$$
(x.y)_k = x_k + y_k + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha, \beta, k} x^{\alpha} y^{\beta}.
$$
Viết $c_{\alpha \beta} = (c_{\alpha \beta 1}, c_{\alpha \beta 2}, \ldots, c_{\alpha \beta n}) \in K^n$, khi đó suy ra rằng
$$
x.y = x + y + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$

Ở vế phải của (5), ta xét thành phần thuần nhất có bậc 2:

$$
B(x, y) = \sum_{i,j=1}^n c_{ij} x_i y_j
$$

sao cho $(x, y) \mapsto B(x, y)$ là một ánh xạ song tuyến tính từ $K^n \times K^n$ vào $K^n$. Khi đó

(6)
$$
x.y \equiv x + y + B(x, y) \mod \deg 3.
$$

Mặt khác, công thức (4) suy ra rằng

(7)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{nếu } |\alpha| + |\beta| < |\gamma|
$$

và rằng các số hạng có bậc toàn phần $|\gamma|$ trong khai triển của $z^\gamma$ cũng chính là các số hạng của $(x_1 + y_1)^{\gamma_1}(x_2 + y_2)^{\gamma_2} \ldots (x_n + y_n)^{\gamma_n} = \sum_{\alpha + \beta = \gamma} ((\alpha, \beta)) x^\alpha y^\beta$ (xem *Đa tạp khả vi và giải tích*, R, Ký hiệu và quy ước). Do đó:

(8)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{nếu } |\alpha| + |\beta| = |\gamma| \quad \text{nhưng } \alpha + \beta \neq \gamma
$$
(9)
$$
c_{\alpha, \beta, \alpha + \beta} = ((\alpha, \beta)).
$$

Tính kết hợp của tích suy ra quan hệ
$$
\sum_{\xi} c_{\alpha \xi n} x^\alpha \left( \sum_{\beta, \gamma} c_{\beta \gamma \xi} y^\beta z^\gamma \right) = \sum_{\xi, \gamma} c_{\xi \gamma n} \left( \sum_{\alpha, \beta} c_{\alpha \beta \xi} x^\alpha y^\beta \right) z^\gamma
$$
đối với mọi $x, y, z$ đủ gần 0, do đó

(10)
$$
\sum_{\xi} c_{\alpha \xi n} c_{\beta \gamma \xi} = \sum_{\xi} c_{\xi \gamma n} c_{\alpha \beta \xi} \quad (\alpha, \beta, \gamma, \eta \text{ trong } \mathbf{N}^n).
$$

mầm nhóm G thừa nhận một mầm nhóm con mở giao hoán khi và chỉ khi $c_{\alpha \beta \gamma} = c_{\beta \alpha \gamma}$ đối với mọi $\alpha, \beta, \gamma$ trong $\mathbf{N}^n$.

### 2. DẤU NGOẶC TRONG ĐẠI SỐ LIE

Với $\alpha \in \mathbf{N}^n$, gọi $e_\alpha$ là phân bố điểm $\frac{1}{\alpha!} \frac{\partial^\alpha}{\partial x^\alpha}$ tại gốc. Đặc biệt,
$$
e_k = e_{e_k} = \frac{\partial}{\partial x_k}.
$$
Các $e_\alpha$ tạo thành một cơ sở của không gian vectơ $U(G)$. Nếu $f$ là một hàm giải tích trên một lân cận mở của 0 trong G và $f(x) = \sum \lambda_\alpha x^\alpha$ là khai triển của nó thành chuỗi nguyên quanh gốc, thì
$$
\langle e_\alpha, f \rangle = \lambda_\alpha.
$$
Đặc biệt,
$$
\langle e_\alpha, x^\gamma \rangle = \delta_{\alpha \gamma}.
$$

Do đó
$$
\langle e_\alpha * e_\beta, x^\gamma \rangle = \langle e_\alpha \otimes e_\beta, (x.y)^\gamma \rangle \\
= \langle e_\alpha \otimes e_\beta, \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} x^{\alpha'} y^{\beta'} \rangle \\
= \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} \langle e_\alpha, x^{\alpha'} \rangle \langle e_\beta, y^{\beta'} \rangle = c_{\alpha\beta\gamma}
$$
và do đó
$$
e_\alpha * e_\beta = \sum_\gamma c_{\alpha\beta\gamma} e_\gamma.
$$
(Công thức (10) khi đó biểu thị tính kết hợp trên $U(G)$.)
Đặc biệt, vì $L(G)$ ổn định đối với dấu ngoặc.
$$
[e_i, e_j] = \sum_k (c_{ijk} - c_{jik}) e_k.
$$
Các hằng số cấu trúc của $L(G)$ đối với cơ sở $(e_1, \ldots, e_n)$ do đó là các $c_{ijk} - c_{jik}$. Nói cách khác, bằng cách đồng nhất một cách chính tắc $L(G)$ với $K^n$, ta thu được:
$$
[x, y] = B(x, y) - B(y, x).
$$

#### Mệnh đề 1 {#lie-iii-s5-prop-1 .statement}

(i) $$ x^{[-1]} \equiv -x + B(x, x) \mod \deg 3 $$
(ii) $$ x.y.x^{[-1]} \equiv y + [x, y] \mod \deg 3 $$
(iii) $$ y^{[-1]}.x.y \equiv x + [x, y] \mod \deg 3 $$
(iv) $$ x^{[-1]}.y^{[-1]}.x.y \equiv [x, y] \mod \deg 3 $$
(v) $$ x.y.x^{[-1]}.y^{[-1]} \equiv [x, y] \mod \deg 3. $$
(Trong (i), $x^{[-1]}$ dĩ nhiên biểu thị khai triển của hàm $x \mapsto x^{[-1]}$ thành một chuỗi nguyên quanh gốc; các công thức khác có thể được hiểu tương tự.)
Gọi $g_1$ và $g_2$ là các thành phần thuần nhất của $x^{[-1]}$ có bậc 1 và 2. Khi đó
$$
0 = x.x^{[-1]} \\
\equiv x + g_1(x) + B(x, g_1(x)) \mod \deg 2 \quad \text{(theo (6))} \\
\equiv x + g_1(x) \mod \deg 2
$$
và do đó $g_1(x) = -x$. Khi đó
$$
0 = x.x^{[-1]} \\
\equiv x + (-x + g_2(x)) + B(x, -x + g_2(x)) \mod \deg 3 \\
\equiv g_2(x) - B(x, x) \mod \deg 3
$$

và do đó $g_2(x) = B(x, x)$. Điều này chứng minh (i). Khi đó, dùng (i),
$$
x.y.x^{[-1]} \equiv (x + y + B(x, y)).(-x + B(x, x)) \quad \text{mod bậc 3}
$$
$$
\equiv x + y + B(x, y) + (-x + B(x, x)) + B(x + y, -x) \quad \text{mod bậc 3}
$$
$$
\equiv y + B(x, y) - B(y, x) \quad \text{mod bậc 3}
$$
$$
\equiv y + [x, y] \quad \text{mod bậc 3 (theo (13))}
$$
do đó (ii). Chứng minh của (iii) là tương tự. Kết hợp (i) và (iii), ta thu được
$$
x^{[-1]},y^{[-1]}.x.y \equiv (-x + B(x, x)).(x + [x, y]) \quad \text{mod bậc 3}
$$
$$
\equiv -x + B(x, x) + x + [x, y] + B(-x, x) \quad \text{mod bậc 3}
$$
$$
\equiv [x, y] \quad \text{mod bậc 3}
$$
do đó (iv). Chứng minh của (v) là tương tự.

### 3. LŨY THỪA

Xét j điểm của G:
$$
x(1) = (x(1)_1, x(1)_2, \ldots, x(1)_n)
$$
$$
x(2) = (x(2)_1, x(2)_2, \ldots, x(2)_n)
$$
$$
\ldots \ldots \ldots \ldots \ldots \ldots \ldots
$$
$$
x(j) = (x(j)_1, x(j)_2, \ldots, x(j)_n).
$$
Ánh xạ $(x(1), x(2), \ldots, x(j)) \mapsto x(1).x(2)\ldots x(j)$ thừa nhận một khai triển thành chuỗi nguyên quanh gốc:

$$
x(1).x(2)\ldots x(j) = \sum_{\alpha(1), \alpha(2), \ldots, \alpha(j) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(j)} x(1)^{\alpha(1)} \ldots x(j)^{\alpha(j)}
$$

trong đó các $a_{\alpha(1), \ldots, \alpha(j)}$ là các phần tử của $\mathbf{K}^n$. Ta viết, với $j = 0, 1, 2, \ldots$,

$$
\psi_j(x) = \sum_{\alpha(1) \neq 0, \ldots, \alpha(j) \neq 0} a_{\alpha(1), \ldots, \alpha(j)} x^{\alpha(1) + \ldots + \alpha(j)}
$$

vế phải là một chuỗi nguyên hội tụ theo biến $x \in \mathbf{K}^n$. Chuỗi này thu được bằng cách loại bỏ trong (14) các số hạng mà trong đó một trong các biến $x(1), \ldots, x(j)$ không xuất hiện tường minh và sau đó viết $x(1) = x(2) = \cdots = x(j) = x$.

Nếu $t \in \mathbf{K}$, tất cả các ánh xạ lũy thừa bậc t của G đều có cùng một khai triển thành chuỗi nguyên quanh gốc, vì hai ánh xạ bất kỳ trong số chúng trùng nhau trên một lân cận của 0. Ta ký hiệu khai triển này dưới dạng chuỗi nguyên bởi $x^{[t]}$.

#### Mệnh đề 2 {#lie-iii-s5-prop-2 .statement}

(i) $\psi_j \equiv 0 \mod \deg j$.
(ii) *Nếu $t \in \mathbf{K}$, thì*
$$
x^{[t]} = \sum_{i=1}^8 \binom{t}{i} \psi_i(x)
$$
*trong đó chuỗi lũy thừa hình thức ở vế phải có nghĩa do (i).*

(Ta viết

$$
\binom{t}{i} = \frac{t(t-1)\ldots(t-i+1)}{i!}
$$

với mọi $t \in \mathbf{K}$.)

Mệnh đề (i) là hiển nhiên từ định nghĩa của các $\psi_j$.

Ta chứng minh (ii) với $t$ là một số nguyên $\geq 0$. Theo (14),

$$
x^{[t]} = \sum_{\alpha(1), \ldots, \alpha(t) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

Với $\alpha = (\alpha(1), \ldots, \alpha(t)) \in (\mathbf{N}^n)^t$, ký hiệu $\sigma(\alpha)$ là tập hợp các $j \in \{1, 2, \ldots, t\}$ sao cho $\alpha(j) \neq 0$. Nếu trong tổng (17), ta nhóm lại các số hạng mà $\sigma(\alpha)$ là như nhau, thì

$$
x^{[t]} = \sum_{\sigma \subset \{1, t\}} h_{t, \sigma}(x)
$$

trong đó

$$
h_{t, \sigma}(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

Cho $\sigma = \{j_1, j_2, \ldots, j_q\}$ với $j_1 < j_2 < \ldots < j_q$. Trong (14) (trong đó $j$ được thay bởi $t$), ta thay 0 vào $x(k)$ với $k \notin \sigma$; vì 0 là phần tử đơn vị của $G$, ta thu được khai triển của $x(j_1) \cdot x(j_2) \ldots x(j_q)$ thành một chuỗi nguyên quanh gốc:

$$
x(j_1) \cdot x(j_2) \ldots x(j_q) = \sum_{\sigma(\alpha) \subset \sigma} a_{\alpha(1), \ldots, \alpha(t)} x(j_1)^{\alpha(j_1)} x(j_2)^{\alpha(j_2)} \ldots x(j_q)^{\alpha(j_q)}
$$

và do đó, theo định nghĩa của $\psi_q$:

$$
\psi_q(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(j_1) + \ldots + \alpha(j_q)}.
$$

Theo (19) và (20), ta thấy rằng $h_{t, \sigma}(x) = \psi_{\mathrm{card}\,\sigma}(x)$. Khi đó (18) suy ra

$$
x^{[t]} = \sum_{i=0}^t \binom{t}{i} \psi_i(x) = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x).
$$

Sau đó ta viết $x^{[t]'} = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x)$ với mọi $t \in \mathbf{K}$. Trong các chuỗi nguyên $x^{[t]}$ và $x^{[t]'}$, mỗi hệ số là một hàm đa thức của $t$. Điều này là hiển nhiên đối với $x^{[t]'}$. Đối với $x^{[t]}$, chỉ cần chứng minh rằng, với mọi $u \in \mathrm{U}(G)$, ảnh của $u$ qua $x \mapsto x^{[t]}$ là một hàm đa thức của $t$. Bây giờ, với $u \in \mathrm{U}^m(G)$, ảnh này là $t^m u$ (\S 4, no. 3, Mệnh đề 7 (iv)).

Vì $x^{[t]} = x^{[t]'}$ với $t$ là một số nguyên $\geq 0$, suy ra $x^{[t]} = x^{[t]'}$ với mọi $t \in \mathbf{K}$.

#### Nhận xét {#lie-iii-s5-n3-rem-1 .statement}

(1) Ta viết điều kiện (ii) của Mệnh đề 2 với t là một số nguyên $\geqslant 0$:

$$
\begin{align*}
0 &= \psi_0(x) \\
x &= \psi_0(x) + \psi_1(x) \\
x^{[2]} &= \psi_0(x) + 2\psi_1(x) + \psi_2(x) \\
&\ldots \ldots \ldots \ldots \ldots \ldots \ldots
\end{align*}
$$

Các công thức này đủ để xác định các $\psi_i$.

(2) Ta thấy rằng $\psi_0(x) = 0, \psi_1(x) = x, \psi_2(x) = x^{[2]} - 2x$,

$$
x^{[-1]} = \sum_{i=1}^\infty (-1)^i \psi_i(x).
$$

(3) Biểu thức trên của $\psi_2$ và công thức (6) chứng minh rằng

$$
\psi_2(x) \equiv \mathrm{B}(x, x) \mod \deg 3.
$$
Dùng Mệnh đề 2, (i) và (ii), ta thấy rằng

$$
x^{[t]} \equiv tx + \binom{t}{2} \mathrm{B}(x, x) \mod \deg 3.
$$

(4) Gọi $\psi_{p,m}(x)$ và $h_{t,m}(x)$ lần lượt là các thành phần thuần nhất của $\psi_p(x)$ và $x^{[t]}$ có bậc m. Khi đó $\psi_{p,m} = 0$ với $m < p$. Mặt khác, Mệnh đề 2 (ii) cho

$$
h_{t,m}(x) = \sum_{p \leq m} \frac{t(t-1)\ldots(t-p+1)}{p!} \psi_{p,m}(x)
$$
tức là

$$
h_{t,m}(x) = \sum_{1 \leq r \leq m} t^r \phi_{r,m}(x)
$$
trong đó $\phi_{r,m}$ là các ánh xạ đa thức thuần nhất bậc m từ $\mathbf{K}^n$ vào $\mathbf{K}^n$. Đặc biệt, theo (23),

$$
\phi_{1,m}(x) = \sum_{p \leq m} \frac{(-1)^{p-1}}{p} \psi_{p,m}(x)
$$
$$
\phi_{m,m}(x) = \frac{1}{m!} \psi_{m,m}(x).
$$

(5) Nếu $\mathbf{K}$ có đặc số $> 0$, các kết quả của các số 1 và 2 vẫn đúng, với điều kiện $e_\alpha$, trong no. 2, được định nghĩa bởi $\langle e_\alpha, \sum_\beta \lambda_\beta x^\beta \rangle = \lambda_\alpha$. Trong no. 3, nếu các $\psi_j$ được định nghĩa như trên, lập luận lại chứng minh rằng $x^{[t]} = \sum_{i=1}^\infty \binom{t}{i} \psi_i(x)$ nếu $t \in \mathbf{N}$.

### 4. HÀM MŨ

Gọi $E(x)$ là khai triển của một ánh xạ hàm mũ của $G$ thành một chuỗi nguyên quanh 0. Gọi $L(x)$ là khai triển của ánh xạ nghịch đảo của một ánh xạ hàm mũ đơn ánh của $G$ thành một chuỗi nguyên quanh 0. Vì ánh xạ tiếp xúc tại 0 của mọi ánh xạ hàm mũ là đồng nhất của $L(G)$, ta có $E(x) \equiv x \mod \deg 2$ và $L(x) \equiv x \mod \deg 2$. Vì $E(L(x)) = L(E(x))$ với $x$ đủ gần 0, các chuỗi lũy thừa hình thức $E$ và $L$ thỏa mãn $E(L(X)) = L(E(X)) = X$. Một lập luận tương tự cho thấy rằng
$$
E(tX) = (E(X))^{[t]}, \quad L(X^{[t]}) = tL(X)
$$
với $t \in K$.

#### Mệnh đề 3 {#lie-iii-s5-prop-3 .statement}

(27)
$$
L = \sum_{p=1}^{\infty} \frac{(-1)^{p-1}}{p} \psi_p
$$
(28)
$$
E = \sum_{p=1}^{\infty} \frac{1}{p!} \psi_{p,p}
$$
(Nhắc lại rằng $\psi_{p,p}$ là thành phần thuần nhất của $\psi_p$ có bậc $p$.)

hoặc, theo (24),
$$
E(tx) = (E(x))^{[t]}
$$

Hai vế là các chuỗi lũy thừa hình thức theo $t$ và $x$. Đồng nhất các số hạng bậc nhất theo $t$, ta thu được
$$
x = \sum_{m \geq 0} \phi_{1,m}(E(x)).
$$
Bây giờ phép nghịch đảo của một hệ các chuỗi lũy thừa hình thức, khi có thể thực hiện được, chỉ có thể thực hiện được theo một cách duy nhất (Đại số, Chương IV, § 6, Hệ quả của Mệnh đề 8). Khi đó
$$
L(x) = \sum_{m \geq 0} \phi_{1,m}(x) \quad \text{theo (29)}
$$
$$
= \sum_{p,m} \frac{(-1)^p}{p} \psi_{p,m}(x) \quad \text{theo (25)}
$$
$$
= \sum_p \frac{(-1)^p}{p} \psi_p(x),
$$
do đó (i). Tương tự, với $t \neq 0$,
$$
L(tx) = tL((tx)^{[t^{-1}]})
$$
$$
= tL\left( \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^{m-r} \phi_{r,m}(x) \right) \quad \text{theo (24)}.
$$

Đồng nhất các số hạng bậc nhất theo t, ta thu được

$$
x = L \left( \sum_{m \geq 0} \phi_{m,m}(x) \right)
$$

do đó

$$
E(x) = \sum_{m \geq 0} \phi_{m,m}(x)
$$
$$
= \sum_{m \geq 0} \frac{1}{m!} \psi_{m,m}(x) \quad \text{theo (26).}
$$

#### Mệnh đề 4 {#lie-iii-s5-prop-4 .statement}

*Để biểu đồ của G được chính tắc, điều kiện cần và đủ là $\psi_j = 0$ với $j \geq 2$.*

Điều này đủ theo Mệnh đề 3. Giả sử rằng bảng là chính tắc và $\psi_i = 0$ với $2 \leq i < n$. Khi đó $nx = x^{[n]} = \sum_{i=0}^n \binom{n}{i} \psi_i(x) = nx + \psi_n(x)$, do đó $\psi_n = 0$. Suy ra $\psi_j = 0$ với $j \geq 2$ bằng quy nạp theo $j$.

### Bài tập {#lie-iii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
