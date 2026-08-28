---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 8
section_title: Rings
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0120-0138, 0195-0198
extraction: ocr
subsections:
    - "no": 1
      title: RINGS
      page: 0
      pdf_page: 120
    - "no": 2
      title: CONSEQUENCES OF DISTRIBUTIVITY
      page: 0
      pdf_page: 122
    - "no": 3
      title: EXAMPLES OF RINGS
      page: 0
      pdf_page: 125
    - "no": 4
      title: RING HOMOMORPHISMS
      page: 0
      pdf_page: 126
    - "no": 5
      title: SUBRINGS
      page: 0
      pdf_page: 127
    - "no": 6
      title: IDEALS
      page: 0
      pdf_page: 127
    - "no": 7
      title: QUOTIENT RINGS
      page: 0
      pdf_page: 129
    - "no": 8
      title: SUBRINGS AND IDEALS IN A QUOTIENT RING
      page: 0
      pdf_page: 130
    - "no": 9
      title: MULTIPLICATION OF IDEALS
      page: 0
      pdf_page: 131
    - "no": 10
      title: PRODUCT OF RINGS
      page: 0
      pdf_page: 132
    - "no": 11
      title: DIRECT DECOMPOSITION OF A RING
      page: 0
      pdf_page: 134
    - "no": 12
      title: RINGS OF FRACTIONS
      page: 0
      pdf_page: 136
statements: 31
exercises: 16
content_sha256: c0fbad15cfceb973a20327d2ed9055c028b5c9170ed25c44741a9a4f0b07088d
translated_from: content/en/alg/I/08_s8_rings.md
source_content_sha256: 82f3b9f6c044b6246eb0c2be0d3c2c67423e560bf34edc83e7cf960aed7cd234
translation_model: gpt-5-6, gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-d5395ffa
glossary_version: 34
glossary_terms_sha256: 1ba2a34303794c6002fe8a73fb57e88b88bbe1e94de18b15719d064d57161853
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. VÀNH

### 1. VÀNH

#### Định nghĩa 1 {#alg-i-s8-def-1 .statement}

*Một vành là một tập hợp* $\mathbf{A}$ *với hai luật hợp thành lần lượt được gọi là phép cộng và phép nhân, thỏa mãn các tiên đề sau*:

(AN I) *Đối với phép cộng* $\mathbf{A}$ *là một nhóm giao hoán*.
(AN II) *Phép nhân là kết hợp và có một phần tử đơn vị*.
(AN III) *Phép nhân có tính phân phối đối với phép cộng*.
*Vành* $\mathbf{A}$ *được gọi là giao hoán nếu phép nhân của nó là giao hoán*.

Trong phần sau, $(x, y) \mapsto x + y$ ký hiệu phép cộng và $(x, y) \mapsto xy$ ký hiệu phép nhân; $0$ ký hiệu phần tử đơn vị đối với phép cộng và $1$ ký hiệu phần tử đơn vị đối với phép nhân. Cuối cùng, $-x$ ký hiệu phần tử đối của $x$ đối với phép cộng. Do đó các tiên đề của một vành được biểu diễn bởi các đẳng thức sau:

$$
\begin{array}{ll}
(1) & x + (y + z) = (x + y) + z \quad \text{(tính kết hợp của phép cộng)} \\
(2) & x + y = y + x \quad \text{(tính giao hoán của phép cộng)} \\
(3) & 0 + x = x + 0 = x \quad \text{(không)} \\
(4) & x + (-x) = (-x) + x = 0 \quad \text{(đối)} \\
(5) & x(yz) = (xy)z \quad \text{(tính kết hợp của phép nhân)} \\
(6) & x.1 = 1.x = x \quad \text{(phần tử đơn vị)} \\
(7) & (x + y).z = xz + yz \\
(8) & x.(y + z) = xy + xz \quad \text{(tính phân phối)}
\end{array}
$$

Cuối cùng vành $\mathbf{A}$ là giao hoán nếu $xy = yx$ với $x, y$ trong $\mathbf{A}$.

Chỉ với phép cộng, $\mathbf{A}$ là một nhóm giao hoán được gọi là *nhóm cộng* của $\mathbf{A}$. Với mọi $x \in \mathbf{A}$, ta định nghĩa phép vị tự trái $\gamma_x$ và phép vị tự phải $\delta_x$ bởi $\gamma_x(y) = xy$, $\delta_x(y) = yx$. Theo các công thức (7) và (8), $\gamma_x$ và $\delta_x$ là các tự đồng cấu của nhóm cộng của $\mathbf{A}$ và do đó ánh xạ không vào không và phần tử đối vào phần tử đối. Vì vậy

$$
\begin{align*}
(9) & \quad x.0 = 0.x = 0 \\
(10) & \quad x.(-y) = (-x).y = -xy;
\end{align*}
$$
suy ra rằng $(-x)(-y) = -((-x).y) = -(-xy)$, do đó
$$(11) \quad (-x)(-y) = xy.$$
Các công thức (10) và (11) tạo thành *quy tắc dấu*. Suy ra rằng
$$-x = (-1)x = x(-1)$$
và $(-1)(-1) = 1$.

Từ (11) suy ra bằng quy nạp theo $n$ rằng
$$(12) \quad (-x)^n = \begin{cases} x^n & \text{nếu } n \text{ là chẵn} \\ -x^n & \text{nếu } n \text{ là lẻ.} \end{cases}$$

Khi nói về các phần tử *giản ước được*, các phần tử *khả nghịch*, các phần tử *khả hoán*, các phần tử *trung tâm*, *vành tử hóa* hoặc *tâm* của một vành $\mathbf{A}$, tất cả các khái niệm này đều quy về phép nhân trên $\mathbf{A}$. Nếu $x, y \in \mathbf{A}$ và $y$ là khả nghịch, phần tử $xy^{-1}$ của $\mathbf{A}$ cũng được ký hiệu là $x/y$ khi $\mathbf{A}$ là giao hoán. Tập hợp các phần tử khả nghịch của $\mathbf{A}$ ổn định đối với phép nhân. Với luật cảm sinh bởi phép nhân nó là một nhóm được gọi là *nhóm nhân* của $\mathbf{A}$, đôi khi được ký hiệu bởi $\mathbf{A}^*$.

Cho $x, y$ thuộc $\mathbf{A}$. $x$ được gọi là một *bội trái* (tương ứng *phải*) của $y$ nếu tồn tại $y' \in \mathbf{A}$ sao cho $x = y'y$ (tương ứng $x = yy'$); cũng nói rằng $y$ là một *ước phải* (tương ứng

trái) của x. Khi A là giao hoán, không cần phân biệt giữa "trái" và "phải".

Phù hợp với thuật ngữ trên, mọi phần tử $y \in \mathbf{A}$ đều được xem như một ước phải và trái của 0; nhưng, do một sự lạm dụng ngôn ngữ, nói chung thuật ngữ "ước phải (tương ứng trái) của 0" được dành cho các phần tử $y$ sao cho tồn tại $x \neq 0$ trong A thỏa mãn quan hệ $xy = 0$ (tương ứng $yx = 0$). Nói cách khác, các ước phải (tương ứng trái) của không là các phần tử không giản ước được phải (tương ứng trái).

Cho $x \in \mathbf{A}$. $x$ được gọi là lũy linh nếu tồn tại một số nguyên $n > 0$ sao cho $x^n = 0$. Khi đó phần tử $1 - x$ khả nghịch, với nghịch đảo bằng
$$
1 + x + x^2 + \cdots + x^{n-1}.
$$

Vì A là một nhóm giao hoán đối với phép cộng, phần tử $nx$ với $n \in \mathbf{Z}$ và $x \in \mathbf{A}$ đã được định nghĩa (§ 2, no. 8). Vì $\gamma_x$ và $\delta_x$ là các tự đồng cấu của nhóm cộng A, $\gamma_x(ny) = n\gamma_x(y)$ và $\delta_y(nx) = n\delta_y(x)$, do đó
$$
x.(ny) = (nx).y = n.(xy).
$$
Đặc biệt, $nx = (n.1)x$.

Một tập hợp A với phép cộng và phép nhân thỏa mãn các tiên đề của một vành ngoại trừ tiên đề đảm bảo sự tồn tại của phần tử đơn vị đối với phép nhân, được gọi là một giả-vành.

### 2. HỆ QUẢ CỦA TÍNH PHÂN PHỐI

Tính phân phối của phép nhân đối với phép cộng cho phép ta áp dụng Mệnh đề 1 của § 3, no. 4, cho
$$
\prod_{i=1}^n \left( \sum_{\lambda \in L_i} x_{i,\lambda} \right) = \sum_{\alpha_1, \ldots, \alpha_n} \prod_{i=1}^n x_{i, \alpha_i}
$$
trong đó tổng được lấy trên tất cả các dãy $(\alpha_1, \ldots, \alpha_n)$ thuộc $L_1 \times \cdots \times L_n$ và với $i = 1, \ldots, n$ họ $(x_{i,\lambda})_{\lambda \in L_i}$ các phần tử của vành A có giá hữu hạn.

#### Mệnh đề 1 {#alg-i-s8-prop-1 .statement}

Cho A là một vành giao hoán và $(x_\lambda)_{\lambda \in L}$ là một họ hữu hạn các phần tử của A. Với mỗi họ các số nguyên dương $\beta = (\beta_\lambda)_{\lambda \in L}$, đặt $|\beta| = \sum_{\lambda \in L} \beta_\lambda$. Khi đó
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}.
$$
Ta áp dụng công thức (13) với $L_i = L$ và $x_{i,\lambda} = x_\lambda$ với $1 \leq i \leq n$. Khi đó
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{\alpha_1, \ldots, \alpha_n} x_{\alpha_1} \cdots x_{\alpha_n},
$$
tổng được lấy trên tất cả các dãy $\alpha = (\alpha_1, \ldots, \alpha_n) \in L^n$.

Cho $\alpha$ thuộc $L^n$; với mọi $\lambda \in L$ ký hiệu $U_\lambda^\alpha$ là tập hợp các số nguyên $i$ sao cho $1 \leq i \leq n$ và $\alpha_i = \lambda$ và đặt $\Phi(\alpha) = (U_\lambda^\alpha)_{\lambda \in L}$. Ngay lập tức thấy rằng $\Phi$ là một song ánh từ $L^n$ lên tập hợp các phân hoạch của $\{1, 2, \ldots, n\}$ được đánh chỉ số bởi $L$. Với mọi $\beta \in \mathbf{N}^L$ sao cho $|\beta| = n$, ký hiệu $L_\beta^n$ là tập hợp các $\alpha \in L^n$ sao cho $\mathrm{Card}\ U_\beta^\alpha = \beta_\lambda$ với mọi $\lambda \in L$. Suy ra rằng họ $(L_\beta^n)_{|\beta|=n}$ là một phân hoạch của $L^n$ và rằng

$$
\mathrm{Card}\ L_\beta^n = \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!}
$$

(§ 5, no. 5).

Cuối cùng, với $\alpha \in L_\beta^n$,

$$
x_{\alpha_1} \cdots x_{\alpha_n} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_{\alpha_i} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_\lambda = \prod_{\lambda \in L} x_\lambda,
$$

do đó

$$
\sum_{(\alpha_1, \ldots, \alpha_n)} x_{\alpha_1} \cdots x_{\alpha_n} = \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} x_{\alpha_1} \cdots x_{\alpha_n}
= \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}
= \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} x_\lambda^{\beta_\lambda}
$$

và công thức (14) do đó suy ra từ (15).

#### Hệ quả 1 (công thức nhị thức) {#alg-i-s8-prop-1-cor-1 .statement}

*Cho x và y là hai phần tử của một vành giao hoán A. Khi đó*:

$$
(x + y)^n = \sum_{p=0}^n \binom{n}{p} x^p y^{n-p}.
$$

Công thức (14) áp dụng cho $L = \{1, 2\}$, $x_1 = x$ và $x_2 = y$ cho

$$
(x + y)^n = \sum_{p+q=n} \frac{n!}{p! q!} x^p y^q,
$$

tổng được lấy trên các cặp số nguyên dương có thứ tự $p, q$ với $p + q = n$. Công thức nhị thức suy ra ngay lập tức từ điều này (*Lý thuyết tập hợp*, III, § 5, no. 8).

#### Hệ quả 2 {#alg-i-s8-prop-1-cor-2 .statement}

*Cho A là một vành giao hoán, X là một tập hợp, $\mathbf{u} = (u_x)_{x \in X}$ và $\mathbf{v} = (v_x)_{x \in X}$ là hai họ phần tử của A. Ký hiệu $\mathbf{u} + \mathbf{v}$ là họ $(u_x + v_x)_{x \in X}$. Với mọi $\lambda \in \mathbf{N}^{(X)}$ ta viết $\lambda! = \prod_{x \in X} \lambda(x)!$. Khi đó với mọi $\alpha \in \mathbf{N}^{(X)}$, theo ký hiệu ở § 7, no. 8,*

$$
(\mathbf{u} + \mathbf{v})^\alpha = \sum_{\beta + \gamma = \alpha} \frac{\alpha!}{\beta! \gamma!} \mathbf{u}^\beta \mathbf{v}^\gamma.
$$

Với $x \in X$,

$$
(u_x + v_x)^{\alpha(x)} = \sum_{m+n=\alpha(x)} \frac{\alpha(x)!}{m! n!} u_x^m v_x^n
$$

theo Hệ quả 1. Lấy tích của các đẳng thức này theo $x \in X$ và dùng (13), ta thu được hệ quả.

#### Mệnh đề 2 {#alg-i-s8-prop-2 .statement}

*Cho $A$ là một vành, $x_1, \ldots, x_n$ là các phần tử của $A$ và $I = \{1, 2, \ldots, n\}$. Với $H \subset I$, ta viết $x_H = \sum_{i \in H} x_i$. Khi đó*

$$
(-1)^n \sum_{\sigma \in S_n} x_{\sigma(1)} \cdots x_{\sigma(n)} = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

*Đặc biệt, nếu $A$ là vành giao hoán,

$$
(-1)^n n! x_1 x_2 \cdots x_n = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

Cho $C$ là tập hợp các ánh xạ từ $I$ vào $\{0, 1\}$. Nếu mỗi $H \subset I$ được gửi tới hàm đặc trưng của nó, ta thu được một song ánh từ $\mathcal{P}(I)$ lên $C$. Do đó vế phải của (16) bằng:

$$
\sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \left( \sum_{i \in I} a(i) x_i \right)^n
$$
$$
= \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \sum_{(i_1, \ldots, i_n) \in I^n} a(i_1) \ldots a(i_n) x_{i_1} \ldots x_{i_n}
$$
$$
= \sum_{(i_1, \ldots, i_n) \in I^n} c_{i_1 \ldots i_n} x_{i_1} \ldots x_{i_n}
$$

trong đó

$$
c_{i_1 \ldots i_n} = \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n).
$$

(1) Giả sử rằng $(i_1, \ldots, i_n)$ không phải là một hoán vị của $I$. Tồn tại một $j \in I$ phân biệt với $i_1, \ldots, i_n$. Gọi $C'$ là tập hợp các $a \in C$ sao cho $a(j) = 0$. Với mọi $a \in C'$, đặt $a^*$ là tổng của $a$ và hàm đặc trưng của $\{j\}$. Khi đó $a^*(1) + \cdots + a^*(n) = a(1) + \cdots + a(n) + 1$ và do đó

$$
c_{i_1 \ldots i_n} = \sum_{a \in C'} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n) + (-1)^{a^*(1)+\cdots+a^*(n)} a^*(i_1) \ldots a^*(i_n)
$$
$$
= \sum_{a \in C'} ((-1)^{a(1)+\cdots+(n)} + (-1)^{a(1)+\cdots+a(n)+1}) a(i_1) \ldots a(i_n) = 0.
$$

(2) Giả sử tồn tại $\sigma \in S_n$ sao cho $i_1 = \sigma(1), \ldots, i_n = \sigma(n)$. Khi đó $a(i_1) \ldots a(i_n) = 0$ trừ khi $a$ chỉ nhận giá trị 1. Vì thế $c_{i_1 \ldots i_n} = (-1)^n$.

### 3. CÁC VÍ DỤ VỀ VÀNH

I. Vành không. Cho A là một vành. Điều kiện $0 = 1$ trong A là cần và đủ để A chỉ gồm một phần tử. Điều kiện ấy hiển nhiên là đủ. Mặt khác, nếu $0 = 1$, thì, với mọi $x \in A$, $x = x.1 = x.0 = 0$. Một vành như vậy được gọi là vành không.

II. Vành số nguyên. Với phép cộng được định nghĩa ở § 2, no. 5, và phép nhân được định nghĩa ở § 2, no. 6, $\mathbf{Z}$ là một vành giao hoán. Ký hiệu 0, 1, $-x$ phù hợp với ký hiệu đã được đưa vào trước đó.

*III. Vành các hàm nhận giá trị thực. Cho I là một khoảng trong tập $\mathbf{R}$ các số thực và A là tập hợp các hàm liên tục xác định trên I nhận giá trị thực. Tổng $f + g$ và tích $f.g$ của hai hàm $f$ và $g$ được xác định bởi
$$(f + g)(t) = f(t) + g(t), \quad (fg)(t) = f(t)g(t) \quad (t \in I).$$
Ta được một vành giao hoán có phần tử đơn vị là hằng 1.*

*IV. Vành giả chập. Cho E là tập hợp các hàm liên tục nhận giá trị thực trên $\mathbf{R}$, bằng không ngoài một khoảng bị chặn. Tổng của hai hàm được định nghĩa như trong III, nhưng tích nay được định nghĩa bởi
$$(fg)(t) = \int_{-\infty}^{\infty} f(s)g(t-s)\ ds$$
("tích chập"). Do đó ta được một vành giả giao hoán không phải là một vành (xem Tích phân, VIII, §4).*

V. Vành đối của một vành A. Cho A là một vành. Tập hợp A với phép cộng như trong A và phép nhân $(x, y) \mapsto yx$ thường được ký hiệu là $A^0$. Nó là một vành (gọi là vành đối của A) có cùng phần tử không và cùng phần tử đơn vị với A và trùng với A khi và chỉ khi A giao hoán.

VI. Vành tự đồng cấu của một nhóm giao hoán. Cho G là một nhóm giao hoán được viết theo phép cộng. Ký hiệu E là tập hợp các tự đồng cấu của G. Với $f$ và $g$ thuộc E, các ánh xạ $f + g$ và $fg$ từ G vào G được xác định bởi
$$(f + g)(x) = f(x) + g(x), \quad (fg)(x) = f(g(x)) \quad (x \in G).$$
Theo § 1, no. 5, Mệnh đề 5, $f + g$ là một tự đồng cấu của G và do đó hiển nhiên $fg = f \circ g$ cũng vậy. Theo § 4, no. 8, E là một nhóm (giao hoán) đối với phép cộng. Phép nhân hiển nhiên là kết hợp và có phần tử đơn vị $\mathrm{Id}_G$. Ngoài ra, với $f, g$ và $h$ thuộc E, ta viết $\phi = f.(g + h)$; với mọi $x \in G$,
$$\phi(x) = f((g + h)(x)) = f(g(x) + h(x)) = f(g(x)) + f(h(x))$$
vì $f$ là một tự đồng cấu của G; do đó $\phi = fg + fh$ và rõ ràng
$$(g + h)f = gf + hf.$$

Vậy E là một vành (nói chung không giao hoán) gọi là *vành tự đồng cấu của G*.

VII. *Vành giả bình phương không.* Một vành giả A được gọi là có bình phương không nếu $xy = 0$ với mọi $x, y \in A$. Cho G là một nhóm giao hoán. Nếu trang bị cho tập hợp G phép cộng của nhóm G và phép nhân $(x, y) \mapsto 0$, ta được một vành giả có bình phương không. Nó chỉ là một vành nếu $G = \{0\}$, trong trường hợp đó nó là vành không.

### 4. ĐỒNG CẤU VÀNH

#### Định nghĩa 2 {#alg-i-s8-def-2 .statement}

*Cho A và B là hai vành. Một cấu xạ, hay đồng cấu, từ A vào B là một ánh xạ f từ A vào B thỏa mãn các quan hệ:*

$$
f(x + y) = f(x) + f(y), \quad f(xy) = f(x) \cdot f(y), \quad f(1) = 1,
$$

*với mọi* $x, y$ *thuộc A*.

Hợp thành của hai đồng cấu vành là một đồng cấu vành. Cho A và B là hai vành và $f$ là một ánh xạ từ A vào B; để $f$ là một đẳng cấu, điều kiện cần và đủ là f là một đồng cấu song ánh; khi đó, $f^{-1}$ là một đồng cấu từ B vào A. Một đồng cấu của một vành A vào chính nó được gọi là một *tự đồng cấu* của A.

Cho $f : A \to B$ là một đồng cấu vành. Ánh xạ $f$ là một đồng cấu của nhóm cộng của A vào nhóm cộng của B; đặc biệt, $f(0) = 0$ và $f(-x) = -f(x)$ với mọi $x \in A$. Ảnh qua $f$ của một phần tử khả nghịch của A là một phần tử khả nghịch của B và $f$ cảm sinh một đồng cấu của nhóm nhân của A vào nhóm nhân của B.

#### Ví dụ {#alg-i-s8-n4-exa-1 .statement}

(1) Cho A là một vành. Ta thấy ngay lập tức rằng ánh xạ $n \mapsto n \cdot 1$ từ $\mathbf{Z}$ vào A là đồng cấu duy nhất từ $\mathbf{Z}$ vào A. Đặc biệt, ánh xạ đồng nhất của $\mathbf{Z}$ là tự đồng cấu duy nhất của vành $\mathbf{Z}$.

Đặc biệt, lấy A là vành tự đồng cấu của nhóm cộng $\mathbf{Z}$ (no. 3, Ví dụ VI). Ánh xạ $n \mapsto n \cdot 1$ từ $\mathbf{Z}$ vào A là một đẳng cấu từ $\mathbf{Z}$ lên A theo đúng phép dựng phép nhân trong $\mathbf{Z}$ (§ 2, no. 6).

(2) Cho $a$ là một phần tử khả nghịch của một vành A. Ánh xạ $x \mapsto axa^{-1}$ là một tự đồng cấu của A vì

$$
a(x + y)a^{-1} = axa^{-1} + aya^{-1},
$$
$$
a(xy)a^{-1} = (axa^{-1})(aya^{-1}).
$$

Nó là song ánh, vì quan hệ $x' = axa^{-1}$ tương đương với $x = a^{-1}x'a$. Do đó nó là một tự đẳng cấu của vành A, gọi là *tự đẳng cấu trong* liên kết với $a$.

### 5. VÀNH CON

#### Định nghĩa 3 {#alg-i-s8-def-3 .statement}

Cho $A$ là một vành. Một vành con của $A$ là một tập con $B$ của $A$ là một nhóm con của $A$ đối với phép cộng, ổn định đối với phép nhân và chứa phần tử khả nghịch của $A$.

Các điều kiện trên có thể được viết như sau

$$
0 \in B, \quad B + B \subset B, \quad -B \subset B, \quad B.B \subset B, \quad 1 \in B.
$$

Nếu $B$ là một vành con của $A$, nó được trang bị phép cộng và phép nhân cảm sinh bởi các phép đó trên $A$, những phép toán này làm cho nó trở thành một vành. Đơn ánh chính tắc của $B$ vào $A$ là một đồng cấu vành.

#### Ví dụ {#alg-i-s8-n5-exa-1 .statement}

(1) Mọi nhóm con của nhóm cộng $\mathbf{Z}$ chứa 1 đều bằng $\mathbf{Z}$. Do đó $\mathbf{Z}$ là vành con duy nhất của $\mathbf{Z}$.

(2) Cho $A$ là một vành và $(A_t)_{t \in I}$ là một họ các vành con của $A$; ngay lập tức ta có rằng $\bigcap_{t \in I} A_t$ là một vành con của $A$. Đặc biệt, giao của các vành con của $A$ chứa một tập con $X$ của $A$ là một vành con được gọi là vành con của $A$ sinh bởi $X$.

(3) Cho $X$ là một tập con của một vành $A$. Vành giao hoán tử của $X$ trong $A$ là một vành con của $A$. Đặc biệt, tâm của $A$ là một vành con của $A$.

(4) Cho $G$ là một nhóm giao hoán với các toán tử; ký hiệu $\Omega$ là tập hợp các toán tử và $\alpha \mapsto f_\alpha$ là tác động của $\Omega$ lên $G$. Cho $E$ là vành tự đồng cấu của nhóm không có toán tử $G$ và $F$ là tập hợp các tự đồng cấu của nhóm có toán tử $G$. Theo định nghĩa, $F$ gồm các tự đồng cấu $\phi$ của $G$ sao cho $\phi \cdot f_\alpha = f_\alpha \cdot \phi$ với mọi $\alpha \in \Omega$. Vì vậy $F$ là một vành con của vành $E$. $F$ được gọi là vành tự đồng cấu của nhóm có toán tử $G$ (xem II, § 1, no. 2). Cho $F_1$ là vành con của $E$ sinh bởi các $f_\alpha$. Khi đó $F$ là vành giao hoán tử của $F_1$ trong $E$.

### 6. IĐÊAN

#### Định nghĩa 4 {#alg-i-s8-def-4 .statement}

Cho $A$ là một vành. Một tập con $a$ của $A$ được gọi là một iđêan trái (tương ứng phải) nếu nó là một nhóm con của nhóm cộng của $A$ và các quan hệ $a \in A, x \in a$ kéo theo $ax \in a$ (tương ứng $xa \in a$). $a$ được gọi là một iđêan hai phía của $A$ nếu nó vừa là một iđêan trái vừa là một iđêan phải của $A$.

Định nghĩa của một iđêan trái có thể được biểu diễn bằng các quan hệ

$$
0 \in a, \quad a + a \subset a, \quad A.a \subset a
$$

quan hệ $-a \subset a$ suy ra từ công thức $(-1).x = -x$ và $A.a \subset a$. Với mọi $x \in A$, đặt $\gamma_x$ là ánh xạ $a \mapsto xa$ của $A$ vào $A$; tác động $x \mapsto \gamma_x$ cho nhóm cộng $A^+$ của $A$ cấu trúc của một nhóm có các toán tử với $A$ làm tập hợp các toán tử. Các iđêan trái của $A$ chính là các nhóm con của $A^+$ ổn định dưới tác động này.

Các iđêan trái trong vành $A$ chính là các iđêan phải của vành đối $A^0$. Trong một vành giao hoán, ba loài iđêan là như nhau; chúng đơn giản được gọi là iđêan.

#### Ví dụ {#alg-i-s8-n6-exa-1 .statement}

(1) Cho $A$ là một vành. Tập hợp $A$ là một iđêan hai phía của $A$; tập hợp gồm 0 cũng vậy, và nó được gọi là iđêan không và đôi khi được ký hiệu bởi 0 hoặc $(0)$ thay cho $\{0\}$.

(2) Với mọi phần tử $a$ của $A$, tập hợp $A.a$ gồm các bội trái của $a$ là một iđêan trái; tương tự tập hợp $a.A$ là một iđêan phải. Khi $a$ thuộc tâm của $A$, $A.a = a.A$; iđêan này được gọi là iđêan chính sinh bởi $a$ và được ký hiệu bởi $(a)$. $(a) = A$ khi và chỉ khi $a$ khả nghịch.

(3) Cho $M$ là một tập con của $A$. Tập hợp các phần tử $x \in A$ sao cho $xy = 0$ với mọi $y \in M$ là một iđêan trái của $A$ gọi là linh hóa tử trái của $M$. Linh hóa tử phải của $M$ được định nghĩa tương tự.

(4) Mọi giao của các iđêan trái (tương ứng phải, hai phía) của $A$ là một iđêan trái (tương ứng phải, hai phía). Cho một tập con $X$ của $A$, do đó tồn tại một iđêan trái (tương ứng phải, hai phía) nhỏ nhất chứa $X$; nó được gọi là iđêan trái (tương ứng phải, hai phía) sinh bởi $X$.

Cho $a$ là một iđêan trái của $A$. Các điều kiện $1 \notin a, a \neq A$ hiển nhiên tương đương.

#### Định nghĩa 5 {#alg-i-s8-def-5 .statement}

*Cho $A$ là một vành. Theo lối nói không chặt, một iđêan trái $a$ được gọi là cực đại nếu nó là một phần tử cực đại của tập hợp các iđêan trái khác với $A$. \*

Nói cách khác, $a$ là cực đại nếu $a \neq A$ và các iđêan trái của $A$ chứa $a$ chỉ là $a$ và $A$.

Định lý 1 (Krull). *Cho $A$ là một vành và $a$ là một iđêan trái của $A$ khác với $A$. Tồn tại một iđêan cực đại $m$ của $A$ chứa $a$. \*

Xem $A$ như tác động lên nhóm cộng $A^+$ của $A$ bởi phép nhân trái. Khi đó các iđêan trái của $A$ là các nhóm con ổn định của $A^+$. Định lý do đó suy ra từ § 4, no. 3, Mệnh đề 3 được áp dụng cho tập con $P = \{1\}$ của $A^+$.

#### Mệnh đề 3 {#alg-i-s8-prop-3 .statement}

*Cho $A$ là một vành, $(x_\lambda)_{\lambda \in L}$ là một họ các phần tử của $A$ và $a$ (tương ứng $b$) là tập hợp các tổng $\sum_{\lambda \in L} a_\lambda x_\lambda$ trong đó $(a_\lambda)_{\lambda \in L}$ là một họ có giá hữu hạn các phần tử của $A$ (tương ứng $\sum_{\lambda \in L} a_\lambda x_\lambda b_\lambda$ trong đó $(a_\lambda)_{\lambda \in L}, (b_\lambda)_{\lambda \in L}$ là các họ có giá hữu hạn các phần tử của $A$). Khi đó $a$ (tương ứng $b$) là iđêan trái (tương ứng hai phía) của $A$ được sinh bởi các phần tử $x_\lambda$.

Các công thức

$$
0 = \sum_{\lambda \in L} 0.x_\lambda
$$
$$
\sum_{\lambda \in L} a_\lambda x_\lambda + \sum_{\lambda \in L} a'_\lambda x_\lambda = \sum_{\lambda \in L} (a_\lambda + a'_\lambda)x_\lambda
$$
$$
a.\sum_{\lambda \in L} a_\lambda x_\lambda = \sum_{\lambda \in L} (aa_\lambda)x_\lambda
$$

chứng minh rằng $a$ là một iđêan trái. Cho $a'$ là một iđêan trái sao cho $x_\lambda \in a'$ với mọi $\lambda \in L$ và cho $(a_\lambda)_{\lambda \in L}$ là một họ có giá hữu hạn trong $A$. Khi đó $a_\lambda x_\lambda \in a'$ với mọi $\lambda \in L$, do đó $\sum_{\lambda \in L} a_\lambda x_\lambda \in a'$; suy ra $a \subset a'$. Do đó $a$ là iđêan trái của $A$ được sinh bởi các $x_\lambda$. Lập luận cho $b$ là tương tự.

#### Mệnh đề 4 {#alg-i-s8-prop-4 .statement}

*Cho $A$ là một vành và $(a_\lambda)_{\lambda \in L}$ là một họ các iđêan trái của $A$. Iđêan trái sinh bởi $\bigcup_{\lambda \in L} a_\lambda$ gồm các tổng $\sum_{\lambda \in L} y_\lambda$ trong đó $(y_\lambda)_{\lambda \in L}$ là một họ có giá hữu hạn sao cho $y_\lambda \in a_\lambda$ với mọi $\lambda \in L$.*

Cho $a$ là tập hợp các tổng $\sum_{\lambda \in L} y_\lambda$ với $y_\lambda \in a_\lambda$ với mọi $\lambda \in L$. Các công thức $\sum_{\lambda \in L} x_\lambda + \sum_{\lambda \in L} y_\lambda = \sum_{\lambda \in L} (x_\lambda + y_\lambda)$ và $a \cdot \sum_{\lambda \in L} x_\lambda = \sum_{\lambda \in L} a x_\lambda$ cho thấy rằng $a$ là một iđêan trái của $A$. Cho $\lambda \in L$ và $x \in a_\lambda$; viết $y_\lambda = x$ và $y_\mu = 0$ với $\mu \neq \lambda$; khi đó $x = \sum_{\lambda \in L} y_\lambda$, do đó $x \in a$ và cuối cùng $a_\lambda \subset a$. Nếu một iđêan trái $a'$ chứa $a_\lambda$ với mọi $\lambda \in L$, thì hiển nhiên nó chứa $a$ và do đó $a$ được sinh bởi $\bigcup_{\lambda \in L} a_\lambda$.

Iđêan $a$ được sinh bởi $\bigcup_{\lambda \in L} a_\lambda$ được gọi là *tổng của các iđêan trái* $a_\lambda$ và được ký hiệu bởi $\sum_{\lambda \in L} a_\lambda$ (xem II, § 1, no. 7). Đặc biệt, tổng $a_1 + a_2$ của hai iđêan trái gồm các tổng $a_1 + a_2$ trong đó $a_1 \in a_1$ và $a_2 \in a_2$.

### 7. VÀNH THƯƠNG

Cho $A$ là một vành. Nếu $a$ là một iđêan hai phía của $A$, hai phần tử $x$ và $y$ của $A$ được gọi là *đồng dư modulo* $a$, viết $x \equiv y$ (mod. $a$) hoặc $x \equiv y(a)$, nếu $x - y \in a$. Đây là một quan hệ tương đương trên $A$. Các quan hệ $x \equiv y(a)$ và $x' \equiv y'(a)$ suy ra $x + x' \equiv y + y'(a)$, $xx' \equiv xy'(a)$ vì $a$ là một iđêan trái và $xy' \equiv yy'(a)$ vì $a$ là một iđêan phải, do đó $xx' \equiv yy'(a)$. Ngược lại, nếu $R$ là một quan hệ tương đương trên $A$ tương thích với phép cộng và phép nhân, tập hợp $a$ gồm các $x \equiv 0$ mod. $R$ là một iđêan hai phía và $x \equiv y$ mod. $R$ tương đương với $x \equiv y$ mod. $a$.

Cho $A$ là một vành và $a$ là một iđêan hai phía của $A$. $A/a$ ký hiệu tập thương của $A$ theo quan hệ tương đương $x \equiv y(a)$, với phép cộng và phép nhân là các phép thương của những phép tương ứng trên $A$ ($§ 1$, no. 6, Định nghĩa 11). Ta chứng minh rằng $A/a$ là một vành:

(a) Dưới phép cộng, $A/a$ là nhóm giao hoán thương của nhóm cộng của $A$ theo nhóm con $a$.

(b) Dưới phép nhân, $A/a$ là một monoid ($§ 2$, no. 1).

(c) Cho $\xi, \eta, \zeta$ thuộc $A/a$ và cho $\pi : A \to A/a$ là ánh xạ chính tắc; ta chọn các phần tử $x, y, z$ trong $A$ sao cho $\pi(x) = \xi, \pi(y) = \eta$ và $\pi(z) = \zeta$. Khi đó
$$
\xi(\eta + \zeta) = \pi(x)\pi(y + z) = \pi(x(y + z)) = \pi(xy + xz)
= \pi(x)\pi(y) + \pi(x)\pi(z) = \xi\eta + \xi\zeta
$$
và hệ thức $(\xi + \eta)\zeta = \xi\zeta + \eta\zeta$ được thiết lập tương tự.

#### Định nghĩa 6 {#alg-i-s8-def-6 .statement}

Cho $A$ là một vành và $a$ là một iđêan hai phía của $A$. Vành thương của $A$ theo $a$, ký hiệu là $A/a$, là tập thương của $A$ theo quan hệ tương đương $x \equiv y(a)$, với phép cộng và phép nhân là các phép thương của những phép toán đó trên $A$.

Vành $A/\{0\}$ đẳng cấu với $A$ và $A/A$ là một vành không.

#### Định lý 2 {#alg-i-s8-thm-2 .statement}

Cho $A$ là một vành và $a$ là một iđêan hai phía của $A$.
(a) Ánh xạ chính tắc $\pi$ của $A$ lên $A/a$ là một đồng cấu vành.
(b) Cho $B$ là một vành và $f$ là một đồng cấu từ $A$ vào $B$. Nếu $f(a) = \{0\}$, tồn tại duy nhất một đồng cấu $\bar{f}$ từ $A/a$ vào $B$ sao cho $f = \bar{f} \circ \pi$.

Theo phép dựng, $\pi(x + y) = \pi(x) + \pi(y)$ và $\pi(xy) = \pi(x)\pi(y)$ với $x, y$ trong $A$; hơn nữa $\pi(1)$ là phần tử khả nghịch $\varepsilon$ của $A/a$, do đó (a).

Cho $A^+$ là nhóm cộng của $A$ và $B^+$ là nhóm cộng của $B$; vì $f$ là một đồng cấu từ $A^+$ vào $B^+$, bằng không trên nhóm con $a$ của $A^+$, nên tồn tại ( § 4, no. 4, Mệnh đề 5) duy nhất một đồng cấu $\bar{f}$ từ $A^+/a$ vào $B^+$ sao cho $f = \bar{f} \circ \pi$. Cho $\xi, \eta$ thuộc $A/a$; chọn $x, y$ thuộc $A$ sao cho $\pi(x) = \xi$ và $\pi(y) = \eta$; khi đó $\xi \eta = \pi(xy)$, do đó

$$
\bar{f}(\xi \eta) = \bar{f}(\pi(xy)) = f(xy) = f(x)f(y) = \bar{f}(\xi)\bar{f}(\eta)
$$

và $\bar{f}(\varepsilon) = f(\pi(1)) = f(1)$, do đó $\bar{f}$ là một đồng cấu vành.

#### Định lý 3 {#alg-i-s8-thm-3 .statement}

Cho $A$ và $B$ là các vành và $f$ là một đồng cấu từ $A$ vào $B$.
(a) Hạt nhân $a$ của $f$ là một iđêan hai phía của $B$.
(b) Ảnh $B' = f(B)$ của $f$ là một vành con của $B$.
(c) Cho $\pi : A \to A/a$ và $i : B' \to B$ là các cấu xạ chính tắc. Tồn tại một và chỉ một cấu xạ $\bar{f}$ từ $A/a$ vào $B'$ sao cho $f = i \circ \bar{f} \circ \pi$ và $\bar{f}$ là một đẳng cấu.

Vì $f$ là một cấu xạ của nhóm cộng của $A$ vào nhóm cộng của $B$, nên $a$ là một nhóm con của $A$. Nếu $x \in a$ và $a \in A$, thì $f(ax) = f(a)f(x) = 0$, do đó $ax \in a$ và tương tự $xa \in a$; do đó $a$ là một iđêan hai phía của $A$. Mệnh đề (b) là hiển nhiên. Vì $f$ bằng không trên $a$, tồn tại một cấu xạ $\bar{f}$ từ $A/a$ vào $B'$ sao cho $f = i \circ \bar{f} \circ \pi$ (Định lý 2). Tính duy nhất của $\bar{f}$ và sự kiện $\bar{f}$ là một đẳng cấu suy ra từ Lý thuyết tập hợp, II, § 6, no. 4.

### 8. CÁC VÀNH CON VÀ CÁC IĐÊAN TRONG MỘT VÀNH THƯƠNG

#### Mệnh đề 5 {#alg-i-s8-prop-5 .statement}

Cho $A$ và $A'$ là hai vành, $f$ là một đồng cấu từ $A$ vào $A'$ và $a$ là hạt nhân của $f$.
(a) Cho $B'$ là một vành con của $A'$. Khi đó $B = f^{-1}(B')$ là một vành con của $A$ chứa $a$. Nếu $f$ là toàn ánh, thì $f(B) = B'$ và $f|_B$ xác định khi chuyển qua thương một đẳng cấu của $B/a$ lên $B'$.
(b) Cho $b'$ là một iđêan trái (tương ứng phải, hai phía) của $A'$. Khi đó $b = f^{-1}(b')$ là một iđêan trái (tương ứng phải, hai phía) của $A$ chứa $a$.

(c) *Nếu $b'$ là một iđêan hai phía của $A'$, thì ánh xạ hợp thành của cấu xạ chính tắc $A' \to A'/b'$ và $f : A \to A'$ xác định, khi chuyển qua thương, một cấu xạ đơn ánh $\bar{f}$ của $A/b$ vào $A'/b'$. Nếu $f$ là toàn ánh, $\bar{f}$ là một đẳng cấu của $A/b$ lên $A'/b'$.

(d) *Giả sử $f$ là toàn ánh. Đặt $\Phi$ là tập hợp các vành con (tương ứng các iđêan trái, các iđêan phải, các iđêan hai phía) của $A$ chứa $a$. Đặt $\Phi'$ là tập hợp các vành con (tương ứng các iđêan trái, các iđêan phải, các iđêan hai phía) của $A'$. Các ánh xạ $B \to f(B)$ và $B' \mapsto \bar{f}(B')^{-1}$ là hai song ánh nghịch đảo từ $\Phi$ lên $\Phi'$ và từ $\Phi'$ lên $\Phi$.

(a) và (b) là hiển nhiên, trừ khẳng định cuối cùng của (a) suy ra từ no. 7, Định lý 3.

Cấu xạ hợp thành $g : A \to A' \to A'/b'$ xét trong (c) có hạt nhân $b$ và do đó $\bar{f}$ là một cấu xạ đơn ánh của $A/b$ vào $A'/b'$ (§ 8, no. 7, Định lý 3). Nếu $f$ là toàn ánh, $g$ là toàn ánh và do đó $\bar{f}$ là toàn ánh.

Giả sử $f$ là toàn ánh. Theo trên, ánh xạ $\theta : B' \mapsto \bar{f}(B')^{-1}$ là một ánh xạ từ $\Phi'$ vào $\Phi$. Rõ ràng ánh xạ $\eta : B \mapsto f(B)$ là một ánh xạ từ $\Phi$ vào $\Phi'$. Khi đó $\theta \circ \eta = \mathrm{Id}_{\Phi}, \eta \circ \theta = \mathrm{Id}_{\Phi'},$ do đó (d).

#### Nhận xét {#alg-i-s8-n8-rem-1 .statement}

Trong ký hiệu trên, $\theta$ và $\eta$ là các đẳng cấu tập hợp có thứ tự ($\Phi$ và $\Phi'$ được sắp thứ tự theo bao hàm).

#### Hệ quả {#alg-i-s8-n8-cor-1 .statement}

*Cho $A$ là một vành và $a$ là một iđêan hai phía của $A$.
(a) Mọi iđêan trái (tương ứng phải, hai phía) của $A/a$ đều viết được duy nhất dưới dạng $b/a$, trong đó $b$ là một iđêan trái (tương ứng phải, hai phía) của $A$ chứa $a$.
(b) Nếu $b$ là hai phía, thì đồng cấu hợp thành $A \to A/a \to (A/a)/(b/a)$ xác định, khi chuyển qua thương, một đẳng cấu của $A/b$ lên $(A/a)/(b/a)$.*

Đủ áp dụng Mệnh đề 5 cho cấu xạ chính tắc của $A$ lên $A/a$.

### 9. PHÉP NHÂN CÁC IĐÊAN

Let $A$ là một vành và $a$ và $b$ là các iđêan hai phía của $A$. Tập hợp các phần tử có dạng $x_1 y_1 + \cdots + x_n y_n$ với $n \geq 0, x_i \in a$ và $y_i \in b$ đối với $1 \leq i \leq n$, hiển nhiên là một iđêan hai phía của $A$, được ký hiệu bởi $ab$ và gọi là *tích* của các iđêan hai phía $a$ và $b$. Với phép nhân này, tập hợp các iđêan hai phía của $A$ là một monoid với phần tử đơn vị là iđêan hai phía $A$. Nếu $a, b, c$ là các iđêan hai phía của $A$, thì $a(b+c) = ab + ac, (b+c)a = ba + ca$. Nếu $A$ giao hoán, phép nhân các iđêan là giao hoán.

$ab \subset aA \subset a$ và $ab \subset Ab \subset b$, do đó

$$
ab \subset a \cap b.
$$

(21)

#### Mệnh đề 6 {#alg-i-s8-prop-6 .statement}

*Cho $a, b_1, \ldots, b_n$ là các iđêan hai phía của $A$. Nếu $A = a + b_i$ với mọi $i$, thì $A = a + b_1 b_2 \ldots b_n = a + (b_1 \cap b_2 \cap \cdots \cap b_n)$.*

Theo (21) chỉ cần chứng minh rằng $A = a + b_1 b_2 \ldots b_n$. Bằng quy nạp, chỉ cần xét trường hợp $n = 2$. Theo giả thiết, tồn tại $a, a' \in a, b_1 \in b_1, b_2 \in b_2$ sao cho $1 = a + b_1 = a' + b_2$. Khi đó
$$
1 = a' + (a + b_1) b_2 = (a' + a b_2) + b_1 b_2 \in a + b_1 b_2,
$$
suy ra $A = a + b_1 b_2$.

#### Mệnh đề 7 {#alg-i-s8-prop-7 .statement}

*Cho $b_1, \ldots, b_n$ là các iđêan hai phía của $A$ sao cho $b_i + b_j = A$ với $i \neq j$. Khi đó $b_1 \cap b_2 \cap \cdots \cap b_n = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$. Đặc biệt, nếu $A$ giao hoán, $b_1 \cap b_2 \cap \cdots \cap b_n = b_1 b_2 \ldots b_n$ (xem Bài tập 2).*

Trước hết xét trường hợp $n = 2$. Tồn tại $a_1 \in b_1, a_2 \in b_2$ sao cho $a_1 + a_2 = 1$. Nếu $x \in b_1 \cap b_2$, thì $x = x(a_1 + a_2) = x a_1 + x a_2 \in b_2 b_1 + b_1 b_2$. Do đó $b_1 \cap b_2 = b_1 b_2 + b_2 b_1$.

Giả sử giờ đẳng thức của mệnh đề đã được thiết lập cho mọi số nguyên $< n$. Theo Mệnh đề 6, $b_n + (b_1 b_2 \ldots b_{n-1}) = A$ và do đó
$$
b_1 \cap b_2 \cap \cdots \cap b_n = (b_1 \cap b_2 \cap \cdots \cap b_{n-1}) b_n + b_n (b_1 \cap b_2 \cap \cdots \cap b_{n-1})
$$
$$
= \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right) b_n
$$
$$
+ b_n \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right)
$$
$$
\subset \sum_{\tau \in S_n} b_{\tau(1)} b_{\tau(2)} \cdots b_{\tau(n)} \subset b_1 \cap b_2 \cap \cdots \cap b_n.
$$

### 10. TÍCH CỦA VÀNH

Cho $(A_i)_{i \in I}$ là một họ các vành. Cho $A$ là tập hợp tích $\prod_{i \in I} A_i$. Trên $A$ phép cộng và phép nhân được xác định bởi các công thức
$$
(x_i) + (y_i) = (x_i + y_i), \quad (x_i)(y_i) = (x_i y_i).
$$
Ngay lập tức kiểm tra được rằng $A$ là một vành gọi là *tích* của các vành $A_i$, với phần tử không là phần tử $0 = (0_i)_{i \in I}$, trong đó $0_i$ là phần tử không của $A_i$, và phần tử khả nghịch $1 = (1_i)_{i \in I}$, trong đó $1_i$ là phần tử khả nghịch của $A_i$. Nếu các $A_i$ là giao hoán, thì $A$ cũng vậy. Nếu $C_i$ là tâm của $A_i$, thì tâm của $A$ là $\prod_{i \in I} C_i$.

Với mọi $i \in I$, phép chiếu $\mathrm{pr}_i$ của $A$ lên $A_i$ là một đồng cấu vành. Nếu $B$ là một vành và $f_i : B \to A_i$ là một họ các đồng cấu, thì tồn tại một đồng cấu duy nhất $f : B \to A$ sao cho $f_i = \mathrm{pr}_i \circ f$ với mọi $i \in I$; nó được cho bởi $f(b) = (f_i(b))_{i \in I}$.

Với mọi $i \in I$, cho $a_i$ là một iđêan trái của $A_i$. Khi đó $a = \prod_{i \in I} a_i$ là một iđêan trái của $A$. Có một kết quả tương tự cho các iđêan phải, các iđêan hai phía và các vành con.

Giả sử rằng $a_i$ là một iđêan hai phía với mọi $i \in I$ và ký hiệu $f_i$ là ánh xạ chính tắc của $A_i$ lên $A_i / a_i$. Khi đó ánh xạ $f : (x_i)_{i \in I} \mapsto (f_i(x_i))_{i \in I}$ của $\prod_{i \in I} A_i$ lên $\prod_{i \in I} (A_i / a_i)$ là một đồng cấu vành có hạt nhân $\prod_{i \in I} a_i$ và do đó, khi chuyển qua thương, xác định một đẳng cấu của $\left( \prod_{i \in I} A_i \right) / \left( \prod_{i \in I} a_i \right)$ lên $\prod_{i \in I} (A_i / a_i)$.

Cho $(I_\lambda)_{\lambda \in L}$ là một phân hoạch của $I$. Song ánh chính tắc của $\prod_{i \in I} A_i$ lên $\prod_{\lambda \in L} \left( \prod_{i \in I_\lambda} A_i \right)$ là một đẳng cấu vành, theo đó hai vành này được đồng nhất.

Cho $J \subset I$. Ký hiệu $e_J$ là phần tử $(x_i)_{i \in I}$ của $A$ được xác định bởi $x_i = 1_i$ với $i \in J$, $x_i = 0_i$ với $i \in I - J$. Khi đó $e_J$ là một lũy đẳng trung tâm ($§ 1$, no. 4) của $A$. Các công thức sau suy ra ngay lập tức:

$$
\begin{align*}
e_I &= 1; \\
e_\varnothing &= 0; \\
e_{J \cap K} &= e_J e_K & \text{cho } J \subset I, K \subset I; \\
e_{J \cup K} &= e_J + e_K & \text{cho } J \subset I, K \subset I, J \cap K = \varnothing; \\
\sum_\lambda e_{J_\lambda} &= 1 & \text{nếu } (J_\lambda) \text{ là một phân hoạch hữu hạn của } I.
\end{align*}
$$

Đặt $A_J = \prod_{i \in J} A_i$. Cho $\eta_J$ là phép chiếu chính tắc của $A$ lên $A_J$. Với $x = (x_i)_{i \in J} \in A_J$, đặt $\varepsilon_J(x)$ là phần tử $(y_i)_{i \in I}$ của $A$ được xác định bởi $y_i = x_i$ với $i \in J$, $y_i = 0_i$ với $i \in I - J$. Khi đó $\eta_J$ là một đồng cấu vành của $A$ lên $A_J$, $\varepsilon_J$ là một đơn cấu của nhóm cộng của $A_J$ lên $A$ và trong biểu đồ

$$
A_J \xrightarrow{\varepsilon_J} A \xrightarrow{\eta_{I-J}} A_{I-J}
$$

hạt nhân $a_J$ của $\eta_{I-J}$ bằng ảnh của $\varepsilon_J$. Khi đó $\varepsilon_J(xx') = \varepsilon_J(x)\varepsilon_J(x')$ với mọi $x, x' \in A_J$; nhưng nói chung $\varepsilon_J$ không phải là một đồng cấu vành vì $\varepsilon_J(1) = e_J$. Rõ ràng $a_J = e_J A = A e_J$.

Đặt $e_{(i)} = e_i$ và $a_i = a_{(i)} = e_i A = A e_i$ với mọi $i \in I$. Khi đó $e_i^2 = e_i$,

$$
e_i e_j = e_j e_i = 0
$$

với $i \neq j$. Nếu $I$ hữu hạn, thì $\sum_{i \in I} e_i = 1$, nhóm cộng $A$ là tổng trực tiếp của các iđêan hai phía $a_i$ và nếu $x \in A$ thì thành phần của nó trong $a_i$ là $x e_i$. Mệnh đề sau được suy ra ngay lập tức.

#### Mệnh đề 8 {#alg-i-s8-prop-8 .statement}

*Giả sử $I$ hữu hạn. Nếu $b$ là một iđêan trái hoặc phải của $A$, thì $b$ là tổng trực tiếp của các $b \cap a_i$.*

### 11. PHÂN TÍCH TRỰC TIẾP CỦA MỘT VÀNH

Cho $A$ là một vành và $(b_i)_{i \in I}$ là một họ các iđêan hai phía của $A$. Ta sẽ gọi đồng cấu

$$
x \mapsto (\phi_i(x))_{i \in I},
$$

trong đó $\phi_i$ là đồng cấu chính tắc của $A$ lên $A/b_i$, là đồng cấu chính tắc của $A$ vào $\prod_{i \in I} (A/b_i)$.

#### Mệnh đề 9 {#alg-i-s8-prop-9 .statement}

*Cho $A$ là một vành và $(b_1, \ldots, b_n)$ là các i-đê-an hai phía của $A$ sao cho $b_i + b_j = A$ với $i \neq j$. Đồng cấu chính tắc của $A$ vào $\prod_{i=1}^n (A/b_i)$ là toàn ánh với hạt nhân $\bigcap_{i=1}^n b_i = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}.$*

Rõ ràng hạt nhân là $\bigcap_{i=1}^n b_i$. Để chứng minh tính toàn ánh, cần chỉ ra rằng, với mọi họ $(x_i)_{1 \leq i \leq n}$ các phần tử của $A$, tồn tại $x \in A$ sao cho $x \equiv x_i (b_i)$ với mọi $1 \leq i \leq n$. Ta chứng minh mệnh đề này bằng quy nạp theo lực lượng $n$ của $I$, trường hợp $n \leq 1$ là tầm thường. Theo giả thiết quy nạp, tồn tại $y \in A$ sao cho $y \equiv x_i (b_i)$ với $1 \leq i \leq n-1$. Ta tìm một $x$ có dạng $y + z$ với $z \in A$. Tất yếu $z \equiv 0 (b_i)$ với $i < n$, tức là $z \in b = \bigcap_{i=1}^{n-1} b_i$, và mặt khác $z \equiv x_n - y (b_n)$. Bây giờ $b_n + b = A$ theo no. 9, Mệnh đề 6, do đó tồn tại $z$. Cuối cùng, biểu thức thứ hai của hạt nhân suy ra từ no. 9, Mệnh đề 7.

#### Định nghĩa 7 {#alg-i-s8-def-7 .statement}

*Cho $A$ là một vành. Một họ hữu hạn $(b_i)_{i \in I}$ các i-đê-an hai phía của $A$ sao cho đồng cấu chính tắc của $A$ vào $\prod_{i \in I} (A/b_i)$ là một đẳng cấu được gọi là một phân tích trực tiếp của $A$. \*

#### Mệnh đề 10 {#alg-i-s8-prop-10 .statement}

*Cho $A$ là một vành, $A'$ là tâm của nó và $(b_i)_{i \in I}$ là một họ hữu hạn các i-đê-an hai phía của $A$. Các điều kiện sau là tương đương:

(a) họ $(b_i)_{i \in I}$ là một phân tích trực tiếp của $A$;
(b) tồn tại một họ $(e_i)_{i \in I}$ các phần tử lũy đẳng của $A'$ sao cho $e_i e_j = 0$ với $i \neq j$, $1 = \sum_{i \in I} e_i$ và $b_i = A(1 - e_i)$ với $i \in I$;
(c) $b_i + b_j = A$ với $i \neq j$ và $\bigcap_{i \in I} b_i = \{0\}$;
(d) $b_i + b_j = A$ với $i \neq j$ và $\prod_{i \in I} b_i = \{0\}$ với mọi thứ tự toàn phần trên $I$;
(e) tồn tại một phân tích trực tiếp $(b'_i)_{i \in I}$ của $A'$ sao cho $b_i = A b'_i$ với $i \in I$. \*

(a) $\Rightarrow$ (b). Nếu điều kiện (a) thỏa mãn, $A$ có thể được đồng nhất với vành $\prod_{i \in I} (A/b_i)$ và $b_i$ với hạt nhân của $\mathrm{pr}_i$. Sự tồn tại của các $e_i$ với các tính chất trong (b) khi đó suy ra từ no. 10.

(b) $\Rightarrow$ (d). Giả sử rằng các $e_i$ tồn tại với các tính chất trong (b). Với $i \neq j$, $1 - e_i \in b_i, \ e_i = e_i(1 - e_j) \in b_j$, do đó $1 \in b_i + b_j$ và $A = b_i + b_j$. Mặt khác, nếu I được cho một thứ tự toàn phần và $(x_i)_{i \in I}$ là một họ các phần tử của A, thì, vì các $e_i$ là trung tâm,

$$
\prod_{i \in I} x_i (1 - e_i) = \left( \prod_{i \in I} x_i \right) \left( \prod_{i \in I} (1 - e_i) \right) = \left( \prod_{i \in I} x_i \right) \left( 1 - \prod_{i \in I} e_i \right) = 0
$$

suy ra $\prod_{i \in I} b_i = \{0\}$.

(d) $\Rightarrow$ (c). Điều này suy ra từ no. 9, Mệnh đề 7.

(c) $\Rightarrow$ (a). Điều này suy ra từ Mệnh đề 9.

Vậy các điều kiện (a), (b), (c) và (d) là tương đương. Giả sử chúng thỏa mãn. Theo (b) $\Rightarrow$ (a), họ các $b'_i = A'(1 - e_i)$ là một phân tích trực tiếp của $A'$. Khi đó $b_i = A(1 - e_i) = Ab'_i$ với mọi $i \in I$. Do đó điều kiện (e) được thỏa mãn.

Cuối cùng, giả sử điều kiện (e) thỏa mãn. Theo (a) $\Rightarrow$ (b), tồn tại một họ $(e_i)_{i \in I}$ các phần tử lũy đẳng của $A'$ sao cho $e_i e_j = 0$ với $i \neq j$, $1 = \sum_{i \in I} e_i$ và $b'_i = A'(1 - e_i)$ với $i \in I$. Khi đó $b_i = Ab'_i = A(1 - e_i)$ với $i \in I$, do đó điều kiện (b) được thỏa mãn.

#### Nhận xét {#alg-i-s8-n11-rem-1 .statement}

Cho A là một vành. Cho $(a_i)_{i \in I}$ là một họ hữu hạn các nhóm con của nhóm cộng $A^+$ của A sao cho $A^+$ là tổng trực tiếp của các $a_i$. Giả sử $a_i a_i \subset ai$ với $i \in I$ và $a_i a_j = \{0\}$ với $i \neq j$. Khi đó $a_i$ là một iđêan hai phía của A với mọi $i \in I$. Với phép cộng và phép nhân cảm sinh bởi những phép toán trên A, $a_i$ là một vành có phần tử đơn vị là thành phần của $1 \in A$ trong $a_i$. Nếu $b_i = \sum_{j \neq i} a_j$, rõ ràng các $b_i$ thỏa mãn điều kiện (c) của Mệnh đề 10 và do đó $(b_i)_{i \in I}$ là một phân tích trực tiếp của A, được gọi là *xác định bởi* $(a_i)_{i \in I}$.

*Ví dụ*: *Các iđêan và các vành thương của* $\mathbf{Z}$

Một iđêan của $\mathbf{Z}$ là một nhóm con cộng tính của $\mathbf{Z}$ và do đó có dạng $n.\mathbf{Z}$ với $n \geqslant 0$; ngược lại, với mọi số nguyên $n \geqslant 0$, tập hợp $n.\mathbf{Z}$ là một iđêan, iđêan chính $(n)$. Do đó mọi iđêan của $\mathbf{Z}$ đều là chính và được biểu diễn duy nhất dưới dạng $n\mathbf{Z}$ với $n \geqslant 0$. Iđêan $(1)$ bằng $\mathbf{Z}$, iđêan $(0)$ chỉ gồm 0 và các iđêan khác với $\mathbf{Z}$ và $\{0\}$ do đó có dạng $n\mathbf{Z}$ với $n > 1$. Nếu $m \geqslant 1$ và $n \geqslant 1$, $m\mathbf{Z} \supset n\mathbf{Z}$ khi và chỉ khi $n \in m.\mathbf{Z}$, tức là $m$ chia hết $n$. Vì vậy, để iđêan $n\mathbf{Z}$ là cực đại, điều kiện cần và đủ là không tồn tại số nguyên $m > 1$ khác với $n$ và chia hết $n$; nói cách khác, *các iđêan cực đại của* $\mathbf{Z}$ *là các iđêan có dạng* $p\mathbf{Z}$ *trong đó* $p$ *là một số nguyên tố* (§ 4, no. 10, Definition 16).

Cho $m$ và $n$ là hai số nguyên $\geqslant 1$. Iđêan $m\mathbf{Z} + n\mathbf{Z}$ là chính, do đó tồn tại một số nguyên $d \geqslant 1$ được xác định bởi $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$; với mọi số nguyên r \geqslant 1, quan hệ "r chia hết d" tương đương với $r\mathbf{Z} \supset d\mathbf{Z}$ và do đó tương đương với "$r\mathbf{Z} \supset m\mathbf{Z}$ và $r\mathbf{Z} \supset n\mathbf{Z}$", tức là "r chia hết m và n". Như vậy thấy rằng các ước chung của m và n là các ước của d và d là *lớn nhất* trong các ước $\geqslant 1$ chung cho m và n; d được gọi là *ước chung lớn nhất* (viết tắt là g.c.d.) của m và n. Vì $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$, tồn tại hai số nguyên x và y sao cho $d = mx + ny$. m và n được gọi là *nguyên tố cùng nhau* nếu g.c.d. của chúng bằng 1. Điều này tương đương với việc giả sử rằng tồn tại các số nguyên x và y với $mx + ny = 1$.

Giao của các iđêan $m\mathbf{Z}$ và $n\mathbf{Z}$ khác 0 vì nó chứa $mn$ và do đó có dạng $r\mathbf{Z}$ với $r \geqslant 1$. Lập luận như trên, thấy rằng các bội của r là các bội chung của m và n và rằng r là *nhỏ nhất* trong các số nguyên $\geqslant 1$ là bội chung của m và n; nó được gọi là *bội chung nhỏ nhất* (l.c.m.) của m và n.

Tích của các iđêan $m\mathbf{Z}$ và $n\mathbf{Z}$ là tập hợp các $\sum_{i=1}^{r} mx_i ny_i = mn \left( \sum_{i=1}^{r} x_i y_i \right)$ với $x_1, \ldots, y_r \in \mathbf{Z}$ và do đó bằng $mn\mathbf{Z}$.

Với mọi số nguyên $n \geqslant 1$, vành thương $\mathbf{Z}/n\mathbf{Z}$ được gọi là *vành các số nguyên modulo n*; nó có n phần tử, là các lớp modulo n của các số nguyên 0, 1, 2, ..., $n - 1$. Với $n = 1$, ta thu được vành không.

#### Mệnh đề 11 {#alg-i-s8-prop-11 .statement}

*Cho $n_1, \ldots, n_d$ là các số nguyên $\geqslant 1$ nguyên tố cùng nhau từng đôi một và $n = n_1 \ldots n_r$. Đồng cấu chính tắc của $\mathbf{Z}$ vào vành tích $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$ là toàn ánh có hạt nhân $n\mathbf{Z}$ và xác định một đẳng cấu vành từ $\mathbf{Z}/n\mathbf{Z}$ lên $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$.*

Đặt $a_i = n_i\mathbf{Z}$ với $i = 1, \ldots, r$. Theo giả thiết, $a_i + a_j = \mathbf{Z}$ với $i \neq j$. Mệnh đề này theo đó suy ra từ Mệnh đề 9.

Những kết quả trên, cũng như các kết quả về phân tích thành các thừa số nguyên tố, sẽ được tổng quát hóa trong Chương VII, § 1, chương này dành cho việc nghiên cứu các vành miền iđêan chính, và trong *Đại số giao hoán*, Chương VII, § 3, chương này dành cho việc nghiên cứu các miền duy nhất phân tích.

### 12. VÀNH PHÂN THỨC

#### Định lý 4 {#alg-i-s8-thm-4 .statement}

*Cho A là một vành giao hoán và S là một tập con của A. Cho $A_S$ là monoid các phân thức của A (chỉ được trang bị phép nhân) với các mẫu số trong S (§ 2, no. 4). Cho $\varepsilon : A \to A_S$ là cấu xạ chính tắc. Trên $A_S$ tồn tại một và chỉ một phép cộng thỏa mãn các điều kiện sau:
(a) $A_S$, với phép cộng này và phép nhân của nó, là một vành giao hoán;
(b) $\varepsilon$ là một đồng cấu vành.*

Giả sử một phép cộng đã được tìm thấy cho $A_S$ thỏa mãn các điều kiện (a) và (b).

Cho $x, y \in A_S$. Cho $S'$ là monoid con nhân ổn định của $A$ do $S$ sinh ra. Tồn tại $a, b \in A$ và $p, q \in S'$ sao cho $x = a/p, y = b/q$. Khi đó

$$
x = \varepsilon(aq)\varepsilon(pq)^{-1}, \quad y = \varepsilon(bp)\varepsilon(pq)^{-1},
$$

do đó

(23)
$$
\begin{align*}
x + y &= (\varepsilon(aq) + \varepsilon(bp))\varepsilon(pq)^{-1} \\
&= \varepsilon(aq + bp)\varepsilon(pq)^{-1} \\
&= (aq + bp)/pq.
\end{align*}
$$

Điều này chứng minh tính duy nhất của phép cộng.

Ta nay *định nghĩa* một phép cộng trên $A_S$ bằng cách đặt $x + y = (aq + bp)/pq$. Cần phải chứng minh rằng định nghĩa này không phụ thuộc vào sự lựa chọn $a, b, p, q$. Bây giờ, nếu $a', b' \in A, p', q' \in S'$ sao cho $x = a'/p', y = b'/q'$, thì tồn tại $s$ và $t$ trong $S'$ sao cho $ap's = a'ps, bq't = b'qt$, do đó

$$
(aq + bp)(p'q')(st) = (a'q' + b'p')(pq)(st)
$$

và suy ra

$$
(aq + bp)/pq = (a'q' + b'p')/p'q'.
$$

Dễ dàng kiểm tra rằng phép cộng trong $A_S$ là kết hợp và giao hoán, rằng $0/1$ là phần tử đơn vị đối với phép cộng, rằng $(-a)/p$ là phần tử đối của $a/p$ và rằng $x(y + z) = xy + xz$ với mọi $x, y, z \in A_S$. Nếu $a, b \in A$, thì

$$
\varepsilon(a + b) = (a + b)/1 = a/1 + b/1 = \varepsilon(a) + \varepsilon(b)
$$

và do đó $\varepsilon$ là một đồng cấu vành.

#### Định nghĩa 8 {#alg-i-s8-def-8 .statement}

*Vành được định nghĩa trong Định lý 4 được gọi là vành phân thức liên kết với $S$, hoặc với các mẫu số trong $S$, và được ký hiệu bởi $A[S^{-1}]$.*

Phần tử không của $A[S^{-1}]$ là $0/1$, phần tử đơn vị của $A[S^{-1}]$ là $1/1$.

Ta sẽ trở lại các tính chất của $A[S^{-1}]$ trong *Đại số giao hoán*, Chương II, § 2.

Nếu $S$ là tập hợp các phần tử giản ước được của $A$, thì vành $A[S^{-1}]$ được gọi là vành phân thức toàn phần của $A$. Khi đó $A$ được đồng nhất với một vành con của $A[S^{-1}]$ nhờ ánh xạ $\varepsilon$, và ánh xạ này khi đó là đơn ánh (I, § 2, no. 4, Mệnh đề 6).

#### Định lý 5 {#alg-i-s8-thm-5 .statement}

*Cho $A$ là một vành giao hoán, $S$ là một tập con của $A$, $B$ là một vành và $f$ là một đồng cấu của $A$ vào $B$ sao cho mọi phần tử của $f(S)$ đều khả nghịch. Tồn tại một và chỉ một $\bar{f}$ từ $A[S^{-1}]$ vào $B$ sao cho $f = \bar{f} \circ \varepsilon$. \*

Chúng ta biết (§ 2, no. 4, Định lý 1) rằng tồn tại một và chỉ một cấu xạ $\bar{f}$ của monoid nhân $A[S^{-1}]$ vào monoid nhân $B$ sao cho $f = \bar{f} \circ \varepsilon$. Cho $a, b \in A, p, q \in S'$ (monoid con nhân ổn định của $A$ sinh bởi $S$). Vì các phần tử của $f(A)$ giao hoán từng đôi một,
$$
\bar{f}(a/p + b/q) = \bar{f}((aq + bp)/pq) = f(aq + bp)f(pq)^{-1}
= (f(a)f(q) + f(b)f(p))f(p)^{-1}f(q)^{-1}
= f(a)f(p)^{-1} + f(b)f(q)^{-1}
= \bar{f}(a/p) + \bar{f}(b/q).
$$
Do đó $\bar{f}$ là một đồng cấu vành.

### Bài tập {#alg-i-s8-exercises}

Xem các [bài tập của § 8](exercises/s8/).
