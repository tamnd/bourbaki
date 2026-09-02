---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 2
section_title: LINEAR DIFFERENTIAL EQUATIONS
lang: vi
source: fvr-i-vii
pdf_pages: 0192-0213, 0219-0221
extraction: ocr
subsections:
    - "no": 1
      title: EXISTENCE OF INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 0
      pdf_page: 192
    - "no": 2
      title: LINEARITY OF THE INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 0
      pdf_page: 194
    - "no": 3
      title: INTEGRATING THE INHOMOGENEOUS LINEAR EQUATION
      page: 0
      pdf_page: 197
    - "no": 4
      title: FUNDAMENTAL SYSTEMS OF INTEGRALS OF A LINEAR SYSTEM OF SCALAR DIFFERENTIAL EQUATIONS
      page: 0
      pdf_page: 198
    - "no": 5
      title: ADJOINT EQUATION
      page: 0
      pdf_page: 201
    - "no": 6
      title: LINEAR DIFFERENTIAL EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 0
      pdf_page: 203
    - "no": 7
      title: LINEAR EQUATIONS OF ORDER $n$
      page: 0
      pdf_page: 207
    - "no": 8
      title: LINEAR EQUATIONS OF ORDER $n$ WITH CONSTANT COEFFICIENTS
      page: 0
      pdf_page: 209
    - "no": 9
      title: SYSTEMS OF LINEAR EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 0
      pdf_page: 211
statements: 25
exercises: 10
content_sha256: d7cfe1e2056f8240683f42bd24493996a92c4b4ae324320167bf918ed2633802
translated_from: content/en/fvr/IV/02_s2_linear_differential_equations.md
source_content_sha256: ed9860cc26b65ff84c11e78ae048f5030e2943903c24c951c87f27907207fd41
translation_model: gpt-5.4
translation_run: translate-vi-b7c400b5
glossary_version: 34
glossary_terms_sha256: dda11999479e6e65875fb1dfa8c2929d6683e0ddd9d2d90083f4a1d2624353e8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. PHƯƠNG TRÌNH VI PHÂN TUYẾN TÍNH

### 1. SỰ TỒN TẠI CÁC TÍCH PHÂN CỦA MỘT PHƯƠNG TRÌNH VI PHÂN TUYẾN TÍNH

Cho E là một không gian chuẩn đầy đủ trên trường $\mathbf{R}$, và J là một khoảng trong $\mathbf{R}$, không thu về một điểm. Ta nói rằng phương trình vi phân

$$
\frac{d\mathbf{x}}{dt} = \mathbf{f}(t, \mathbf{x})
$$

(1) trong đó $f$ được xác định trên $J \times E$, là một phương trình *tuyến tính* nếu, với mọi $t \in J$, ánh xạ $x \mapsto f(t, x)$ là một *ánh xạ afin tuyến tính liên tục* $^1$ từ $E$ vào chính nó; nếu đặt $b(t) = f(t, 0)$ thì ánh xạ $x \mapsto f(t, x) - f(t, 0) = f(t, x) - b(t)$ khi đó là một ánh xạ tuyến tính liên tục từ $E$ vào chính nó; từ nay về sau ta sẽ ký hiệu ánh xạ này bởi $A(t)$ và viết $A(t).x$, (hoặc đơn giản là $A(t)x$) cho giá trị của nó tại điểm $x \in E$; như vậy phương trình vi phân tuyến tính (1) có thể được viết

$$
\frac{dx}{dt} = A(t).x + b(t)
$$

(2)

trong đó $b$ là một ánh xạ từ $J$ vào $E$; khi $b = 0$ ta nói rằng phương trình vi phân tuyến tính (2) là *thuần nhất*.

#### Ví dụ 1 {#fvr-iv-s2-n1-exa-1 .statement}

Khi $E$ có số chiều hữu hạn $n$ trên $\mathbf{R}$ thì ta có thể đồng nhất tự đồng cấu $A(t)$ với *ma trận* $\left(a_{ij}(t)\right)$ của nó *đối với một cơ sở bất kỳ của* $E$ (*Alg.*, II, p. 343); khi ta đồng nhất một vectơ $x \in E$ với ma trận cột $(x_j)$ gồm các thành phần của nó đối với cơ sở của $E$ đang xét thì biểu thức $A(t).x$ phù hợp với các quy ước tổng quát của Đại số (*Alg.*, II, p. 343, prop 2). Trong trường hợp này, phương trình (2) tương đương với hệ phương trình vi phân vô hướng

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

(3)

#### Ví dụ 2 {#fvr-iv-s2-n1-exa-2 .statement}

Cho $G$ là một *đại số chuẩn đầy đủ* trên $\mathbf{R}$, và $a(t)$, $b(t)$ và $c(t)$ là ba ánh xạ từ $J$ vào $G$; phương trình

$$
\frac{dx}{dt} = a(t)x + x b(t) + c(t)
$$

là một phương trình vi phân tuyến tính; ở đây $A(t)$ là ánh xạ tuyến tính $x \mapsto a(t)x + x b(t)$ từ $G$ vào chính nó.

Với mọi $t \in J$, $A(t)$ là một phần tử của tập hợp $\mathcal{L}(E)$ các ánh xạ tuyến tính liên tục từ $E$ vào chính nó (các tự đồng cấu liên tục của $E$); ta biết (*Gen. Top.*, X, p. 298) rằng $\mathcal{L}(E)$, được trang bị *chuẩn* $\|U\| = \sup_{\|x\| \leq 1} \|Ux\|$, là một *đại số chuẩn đầy đủ* trên trường $\mathbf{R}$, và rằng $\|UV\| \leq \|U\|\ \|V\|$.

*Trong suốt tiết diện này, ta sẽ giả sử rằng các điều kiện sau đây được thỏa mãn:*

a) *Ánh xạ* $t \mapsto A(t)$ *từ* $J$ *vào* $\mathcal{L}(E)$ *là được điều chỉnh*.

b) *Ánh xạ* $t \mapsto b(t)$ *từ* $J$ *vào* $E$ *là được điều chỉnh*.

Khi $E$ có chiều $n$, $\mathcal{L}(E)$ đẳng cấu với $\mathbf{R}^{n^2}$ (như một không gian vectơ tôpô) và điều kiện *a*) có nghĩa là mỗi phần tử $a_{ij}(t)$ của ma trận $A(t)$ là một hàm *điều hòa* trên $J$.

(1) Nhắc lại rằng nếu $E$ có số chiều hữu hạn thì mọi ánh xạ afin tuyến tính từ $E$ vào chính nó đều liên tục (*Gen. Top.*, VI, p. 33 and 37).

Vì $\|A(t')\mathbf{x} - A(t)\mathbf{x}\| \leq \|A(t') - A(t)\|\|\mathbf{x}\|$, ánh xạ
$$
t \mapsto A(t).\mathbf{x} + \mathbf{b}(t)
$$
là điều hòa với mọi $\mathbf{x} \in E$; hơn nữa,
$$
\|A(t)\mathbf{x}_1 - A(t)\mathbf{x}_2\| = \|A(t)(\mathbf{x}_1 - \mathbf{x}_2)\| \leq \|A(t)\|\|\mathbf{x}_1 - \mathbf{x}_2\|
$$
với mọi $t \in J$ và mọi $\mathbf{x}_1, \mathbf{x}_2$ trong $E$; nói cách khác, vế phải của (2) thỏa mãn các điều kiện của bổ đề 1, IV, p. 165 và là Lipschitz đối với hàm điều hòa $\|A(t)\|$ trên $J \times E$. Hệ quả là (IV, p. 173, hệ quả 2):

#### Định lý 1 {#fvr-iv-s2-thm-1 .statement}

*Cho* $t \mapsto A(t)$ *là một ánh xạ điều hòa từ* $J$ *vào* $\mathcal{L}(E)$, *và* $t \mapsto \mathbf{b}(t)$ *là một ánh xạ điều hòa từ* $J$ *vào* $E$. *Với mọi điểm* $(t_0, \mathbf{x}_0)$ *của* $J \times E$ *phương trình tuyến tính* (2) *nhận một và chỉ một nghiệm xác định trên toàn bộ* $J$ *và bằng* $\mathbf{x}_0$ *tại điểm* $t_0$.

### 2. TÍNH TUYẾN TÍNH CỦA CÁC TÍCH PHÂN CỦA MỘT PHƯƠNG TRÌNH VI PHÂN TUYẾN TÍNH

Việc giải một phương trình vi phân tuyến tính (2) là một bài toán tuyến tính (*Alg.*, II, p. 240); phương trình tuyến tính thuần nhất
$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$
được gọi là *liên kết* với phương trình không thuần nhất (2); và người ta biết (*Alg.*, II, p. 241, mệnh đề 14) rằng nếu $\mathbf{u}_1$ là một tích phân của phương trình không thuần nhất (2) thì mọi tích phân của phương trình này đều có dạng $\mathbf{u} + \mathbf{u}_1$ trong đó $\mathbf{u}_1$ là một nghiệm của phương trình thuần nhất liên kết (4), và ngược lại. Trước hết chúng tôi sẽ nghiên cứu trong tiểu mục này các tích phân của một phương trình *thuần nhất* (4).

#### Mệnh đề 1 {#fvr-iv-s2-prop-1 .statement}

*Tập hợp* $\mathcal{I}$ *các tích phân của phương trình tuyến tính thuần nhất* (4), *xác định trên* $J$, *là một không gian con vectơ của không gian* $C(J; E)$ *các ánh xạ liên tục từ* $J$ *vào* $E$.

Chứng minh là ngay lập tức.

#### Định lý 2 {#fvr-iv-s2-thm-2 .statement}

*Với mọi điểm* $(t_0, \mathbf{x}_0)$ *của* $J \times E$ *gọi* $\mathbf{u}(t, t_0, \mathbf{x}_0)$ *là tích phân của phương trình thuần nhất* (4) *xác định trên* $J$ *và bằng* $\mathbf{x}_0$ *tại* $t_0$.
1. *Với mọi điểm* $t \in J$ *ánh xạ* $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ *là một ánh xạ tuyến tính song ánh song liên tục* $C(t, t_0)$ *từ* $E$ *vào chính nó*.
2. *Ánh xạ* $t \mapsto C(t, t_0)$ *từ* $J$ *vào* $\mathcal{L}(E)$ *đồng nhất với tích phân của phương trình vi phân tuyến tính thuần nhất*
$$
\frac{dU}{dt} = A(t)\ U
$$
*nhận giá trị* $I$ **(ánh xạ đồng nhất của* $E$ *vào chính nó)* *tại điểm* $t_0$.
3. *Với mọi điểm* $s, t, u$ *của* $J$
$$
C(s, u) = C(s, t)C(t, u), \qquad C(s, t) = (C(t, s))^{-1}.
$$

Theo mệnh đề 1, $\mathbf{u}(t, t_0, \mathbf{x}_1) + \mathbf{u}(t, t_0, \mathbf{x}_2)$ (resp. $\lambda \mathbf{u}(t, t_0, \mathbf{x}_0)$) là một nghiệm nguyên của (4) và nhận giá trị $\mathbf{x}_1 + \mathbf{x}_2$ (resp. $\lambda \mathbf{x}_0$) tại $t_0$, nên, theo định lý 1 của IV, p. 179, đồng nhất với $\mathbf{u}(t, t_0, \mathbf{x}_1 + \mathbf{x}_2)$ (resp. $\mathbf{u}(t, t_0, \lambda \mathbf{x}_0)$); do đó ánh xạ $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ là một ánh xạ tuyến tính $C(t, t_0)$ của E vào chính nó, và ta có thể viết $\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0). \mathbf{x}_0$.

Vì ánh xạ $(X, Y) \mapsto XY$ của $\mathcal{L}(E) \times \mathcal{L}(E)$ vào $\mathcal{L}(E)$ là liên tục (*Gen. Top.*, X, p. 298, prop. 8), ánh xạ $t \mapsto A(t)U$ của J vào $\mathcal{L}(E)$ là điều hòa với mọi $U \in \mathcal{L}(E)$; hơn nữa (*Gen. Top.*, X, p. 296)

$$
\| A(t)X - A(t)Y \| = \| A(t)(X - Y) \| \leq \| A(t) \| \| X - Y \|,
$$

nên có thể áp dụng định lý I của IV, p. 179 cho phương trình tuyến tính thuần nhất (5); gọi $V(t)$ là nghiệm nguyên của phương trình này được xác định trên J và bằng $I$ tại $t_0$. Ta có (I, p. 6, prop. 3)

$$
\frac{d}{dt} (V(t)\mathbf{x}_0) = \frac{dV(t)}{dt} \mathbf{x}_0 = A(t)(V(t)\mathbf{x}_0)
$$

và với $t = t_0$ ta có $V(t)\mathbf{x}_0 = I\mathbf{x}_0 = \mathbf{x}_0$; theo định lý 1 của IV, p. 179, phải có $V(t).\mathbf{x}_0 = C(t, t_0)\mathbf{x}_0$ với mọi $\mathbf{x}_0 \in E$, tức là, $V(t) = C(t, t_0)$; điều này chứng minh rằng $C(t, t_0)$ thuộc $\mathcal{L}(E)$, nói cách khác, rằng $\mathbf{x}_0 \mapsto C(t, t_0).\mathbf{x}_0$ là liên tục trên E, và ánh xạ $t \mapsto C(t, t_0)$ là nghiệm nguyên của (5) bằng $I$ tại $t_0$.

Cuối cùng, nghiệm nguyên $s \mapsto C(s, u).\mathbf{x}_0$ của (4) nhận giá trị $C(t, u).\mathbf{x}_0$ tại điểm $t$, nên, theo định nghĩa,

$$
C(s, u).\mathbf{x}_0 = C(s, t)(C(t, u).\mathbf{x}_0) = (C(s, t)C(t, u)).\mathbf{x}_0
$$

với mọi $\mathbf{x}_0 \in E$, do đó có hệ thức thứ nhất (6); vì $C(s, s) = I$ nên ta có $C(s, t)C(t, s) = I$, với mọi $s$ và $t$ trong J; điều này chứng minh (*Set Theory*, II, p. 86, corollary) rằng $C(t, t_0)$ là một ánh xạ song ánh của E lên chính nó, với ánh xạ nghịch đảo là $C(t_0, t)$. Điều này hoàn tất chứng minh định lý.

Người ta gọi $C(t, t_0)$ là *resolvent* của phương trình (2) của IV, p. 178.

#### Hệ quả 1 {#fvr-iv-s2-thm-2-cor-1 .statement}

*Ánh xạ gán cho mỗi điểm $\mathbf{x}_0 \in E$ hàm liên tục $t \mapsto C(t, t_0).\mathbf{x}_0$, được xác định trên J, là một đẳng cấu của không gian định chuẩn E lên không gian vectơ $\mathcal{I}$ các nghiệm nguyên của (4), được trang bị tôpô hội tụ compact.*

Hiển nhiên đó là một ánh xạ tuyến tính song ánh của E lên $\mathcal{I}$: bây giờ $C(t, t_0)$ bị chặn trên một tập compact $K \subset J$, nên $\| C(t, t_0).\mathbf{x}_0 \| \leq M \| \mathbf{x}_0 \|$ với mọi $t \in K$ và $\mathbf{x}_0 \in E$, điều này cho thấy ánh xạ ấy là liên tục; và vì

$$
C(t_0, t_0).\mathbf{x}_0 = \mathbf{x}_0,
$$

nên rõ ràng ánh xạ nghịch đảo cũng liên tục.

#### Hệ quả 2 {#fvr-iv-s2-thm-2-cor-2 .statement}

*Ánh xạ $(s, t) \mapsto C(s, t)$ của $J \times J$ vào $\mathcal{L}(E)$ là liên tục.*

Theo (6) ta có $C(s, t) = C(s, t_0) \left( C(t, t_0) \right)^{-1}$; bây giờ, ánh xạ $(X, Y) \mapsto XY$ từ $\mathcal{L}(E) \times \mathcal{L}(E)$ vào $\mathcal{L}(E)$ là liên tục, cũng như ánh xạ $X \mapsto X^{-1}$ từ nhóm (mở) các phần tử khả nghịch của $\mathcal{L}(E)$ lên chính nó (TG, IX, p. 40, mệnh đề 14).

Có thể chú ý rằng ánh xạ
$$
t \mapsto C(t_0, t) = (C(t, t_0))^{-1}
$$
có đạo hàm bằng $-(C(t, t_0))^{-1} (dC(t, t_0)/dt)(C(t, t_0))^{-1}$ (trên phần bù của một tập hợp đếm được) (I, p. 8, mệnh đề 4), nghĩa là (theo IV, p. 179, công thức (5)) bằng $-C(t_0, t) A(t)$.

#### Hệ quả 3 {#fvr-iv-s2-thm-2-cor-3 .statement}

*Cho K là một khoảng compact được chứa trong J, và đặt $k = \sup_{t \in K} \|A(t)\|$. Với mọi t và $t_0$ trong K*
$$
\|C(t, t_0) - I\| \leq e^{k|t-t_0|} - 1 .
$$ (7)

Thật vậy, $\|A(t)x_0\| \leq k \|x_0\|$ với mọi $t \in K$; trên K, hàm hằng bằng $x_0$ do đó là một tích phân gần đúng sai số không vượt quá $k \|x_0\|$ theo phương trình (4) của IV, p. 18; theo công thức (15) của IV, p. 170, do đó ta có
$$
\|C(t, t_0)x_0 - x_0\| \leq \|x_0\| (e^{k|t-t_0|} - 1)
$$
với mọi $t$ và $t_0$ trong K, và mọi $x_0$ trong E, điều này tương đương với bất đẳng thức (7) theo định nghĩa của chuẩn trên $\mathcal{L}(E)$.

#### Mệnh đề 2 {#fvr-iv-s2-prop-2 .statement}

*Cho B là một tự đồng cấu liên tục của E, độc lập với t, và giao hoán với A(t) với mọi $t \in J$; khi đó B giao hoán với $C(t, t_0)$ với mọi t và $t_0$ trong J.*

Thật vậy, theo (5)
$$
\frac{d}{dt}(BC) = BAC = ABC \quad \text{và} \quad \frac{d}{dt}(CB) = ACB ,
$$
nên $\frac{d}{dt}(BC - CB) = A(BC - CB)$; nhưng $BC(t_0, t_0) - C(t_0, t_0)B = 0$, nên (IV, p. 179, định lý 1) $BC(t, t_0) - C(t, t_0)B = 0$ với mọi $t \in J$.

Một trường hợp quan trọng của mệnh đề 2 là trường hợp E được trang bị cấu trúc không gian vectơ có chuẩn đối với *trường số phức* $\mathbf{C}$, và trong đó, với mọi $t \in J$, $A(t)$ là một tự đồng cấu của E đối với cấu trúc không gian vectơ này; điều đó có nghĩa là $A(t)$ giao hoán với tự đồng cấu liên tục $x \mapsto tx$ của E (đối với cấu trúc không gian vectơ *trên* $\mathbf{R}$); khi đó $C(t, t_0)$ giao hoán với tự đồng cấu này, điều đó có nghĩa là với mọi $t$ và $t_0$ trong J, ánh xạ $C(t, t_0)$ là một tự đồng cấu liên tục đối với cấu trúc không gian vectơ có chuẩn của E trên $\mathbf{C}$.

### 3. TÍCH PHÂN PHƯƠNG TRÌNH TUYẾN TÍNH KHÔNG THUẦN NHẤT

Việc tích phân phương trình tuyến tính không thuần nhất

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

quy về việc tích phân phương trình thuần nhất liên kết

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

và tính một nguyên hàm. Với ký hiệu của định lý 2, IV, p. 179, đặt $\mathbf{x} = C(t, t_0).\mathbf{z}$, do đó, theo công thức thứ hai (6) của IV, p. 179, $\mathbf{z} = C(t_0, t).\mathbf{x}$; nếu $\mathbf{x}$ là một tích phân của (2) thì $\mathbf{z}$ là một tích phân của phương trình $\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = A(t)C(t, t_0).\mathbf{z} + \mathbf{b}(t)$; vì ánh xạ song tuyến tính

$$
(U, y) \mapsto U.y
$$

từ $\mathcal{L}(\mathbf{E}) \times \mathbf{E}$ vào $\mathbf{E}$ là liên tục (\emph{Gen. Top.}, X, p. 297, mệnh đề 6), $\mathbf{z}$ có đạo hàm (trừ trên một tập con đếm được của J) và ta có, theo công thức đạo hàm của một hàm song tuyến tính (I, p. 6, mệnh đề 3)

$$
\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = \frac{dC(t, t_0)}{dt}.\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt} = A(t)C(t, t_0).\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt}
$$

(thay $dC(t, t_0)/dt$ bằng $A(t)C(t, t_0)$ theo (5) (IV, p. 179)). Khi đó phương trình đối với $\mathbf{z}$ quy về $C(t, t_0).d\mathbf{z}/dt = \mathbf{b}(t)$, hay cũng lại là

$$
\frac{d\mathbf{z}}{dt} = C(t_0, t).\mathbf{b}(t)
$$

theo công thức thứ hai (6) ở IV, p. 179. Bây giờ vế phải của phương trình (8) là một hàm điều hòa trên J, vì nó thu được bằng cách thay các hàm điều hòa $U$ và $y$ vào hàm song tuyến tính liên tục $U.y$ (\emph{cf.} II, p. 55, hệ quả 2); do đó phương trình (8) có một và chỉ một nguyên hàm nhận giá trị $\mathbf{x}_0$ tại $t_0$, được cho bởi công thức

$$
\mathbf{z}(t) = \mathbf{x}_0 + \int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds.
$$

Vì ta có $C(t, t_0).\int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds = \int_{t_0}^t C(t, t_0)C(t_0, s).\mathbf{b}(s)\,ds$ (II, p. 59, công thức (9)), suy ra (có tính đến công thức thứ nhất (6) ở IV, p. 179) kết quả sau đây:

#### Mệnh đề 3 {#fvr-iv-s2-prop-3 .statement}

*Với các ký hiệu của định lý 2* (IV, p. 179), *với mọi điểm* $(t_0, \mathbf{x}_0)$ *của* $J \times \mathbf{E}$ *nguyên hàm của phương trình tuyến tính* (2) *xác định trên* $J$ *và bằng* $\mathbf{x}_0$ *tại* $t_0$ *được cho bởi công thức*

$$
\mathbf{u}(t) = C(t, t_0).\mathbf{x}_0 + \int_{t_0}^t C(t, s).\mathbf{b}(s)\,ds.
$$

Phương pháp dẫn đến công thức (10), gồm việc lấy hàm $\mathbf{z}$ làm hàm chưa biết mới, thường được gọi là "phương pháp biến thiên hằng số".

### 4. HỆ CƠ BẢN CÁC NGUYÊN HÀM CỦA MỘT HỆ TUYẾN TÍNH CÁC PHƯƠNG TRÌNH VI PHÂN VÔ HƯỚNG

Trong tiểu mục này và tiểu mục tiếp theo, ta sẽ xét trường hợp E là một không gian vectơ có số chiều hữu hạn n trên trường $\mathbf{C}$ các số phức (vậy có chiều 2n trên $\mathbf{R}$), và trong đó, với mọi $t \in J$, $A(t)$ là một tự đồng cấu của E đối với cấu trúc không gian vectơ trên $\mathbf{C}$. Khi đó có thể đồng nhất $A(t)$ với ma trận $(a_{ij}(t))$ của nó đối với một cơ sở của E (trên trường $\mathbf{C}$), lần này các $a_{ij}$ là $n^2$ hàm phức xác định và điều hòa trên J; nếu ký hiệu bởi $x_j$ ($1 \leq j \leq n$) các thành phần (phức) của một vectơ $x \in E$ đối với cơ sở đã chọn, thì phương trình tuyến tính

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

lại tương đương với hệ

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

Định lý 1 (IV, p. 179) và 2 (IV, p. 179) và mệnh đề 2 (IV, p. 181) khi đó cho thấy rằng với mọi $\mathbf{x}_0 = (x_{k0})_{1 \leq k \leq n}$ trong E đều tồn tại một và chỉ một nguyên hàm $\mathbf{u} = (u_k)_{1 \leq k \leq n}$ của phương trình

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

xác định trên E và bằng $\mathbf{x}_0$ tại điểm $t_0$; nguyên hàm này có thể viết

$$
\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0).\mathbf{x}_0,
$$

trong đó $C(t, t_0)$ là một ma trận bình phương khả nghịch $(c_{ij}(t, t_0))$ cấp $n$ mà các phần tử của nó là các hàm phức liên tục trên $J \times J$ và sao cho $t \mapsto c_{ij}(t, t_0)$ là một nguyên hàm của một hàm điều hòa trên J.

Trong trường hợp riêng khi $n = 1$ thì hệ (3) rút về một phương trình vô hướng duy nhất

$$
\frac{dx}{dt} = a(t)x + b(t)
$$

trong đó $a(t)$ và $b(t)$ là các hàm phức điều hòa trên J); ta kiểm tra ngay lập tức rằng ma trận $C(t, t_0)$ (chỉ có một phần tử) bằng $\exp \left( \int_{t_0}^t a(s)\, ds \right)$; do đó nguyên hàm của (11) bằng $x_0$ tại điểm $t_0$ được cho tường minh bởi công thức

$$
u(t) = x_0 \exp \left( \int_{t_0}^t a(s)\, ds \right) + \int_{t_0}^t b(s) \exp \left( \int_{t_0}^\tau a(\tau)\, d\tau \right) ds.
$$

Trong không gian $\mathcal{C}(J; E)$ các ánh xạ liên tục từ J vào E, được trang bị tôpô hội tụ compắc, tập hợp $\mathcal{I}$ các nguyên hàm của phương trình (4) là một không gian con vectơ (trên $\mathbf{C}$) đẳng cấu với E, do đó với $\mathbf{C}^n$ (IV, p. 180, hệ quả 1, và IV, p. 181, mệnh đề 2).

Một cơ sở $(\mathbf{u}_j)_{1 \leq j \leq n}$ của không gian này (trên trường $\mathbf{C}$) được gọi là một *hệ cơ bản* các nguyên hàm của (4).

#### Mệnh đề 4 {#fvr-iv-s2-prop-4 .statement}

*Để $n$ tích phân $\mathbf{u}_j$ ($1 \leq j \leq n$) của phương trình (4) tạo thành một hệ cơ bản thì điều kiện cần và đủ là các giá trị $\mathbf{u}_j(t_0)$ của chúng tại một điểm $t_0 \in J$ là các vectơ độc lập tuyến tính trong $E$.*

Thật vậy, ánh xạ gán cho mỗi $\mathbf{x}_0 \in E$ tích phân $t \mapsto C(t, t_0).\mathbf{x}_0$ là một đẳng cấu từ $E$ lên $\mathcal{I}$ (IV, p. 180, hệ quả 1 và IV, p. 181, mệnh đề 2).

Nếu $(\mathbf{e}_j)_{1 \leq j \leq n}$ là một cơ sở bất kỳ của $E$ trên $\mathbf{C}$, thì $n$ tích phân
$$
\mathbf{u}_j(t) = C(t, t_0).\mathbf{e}_j \qquad (1 \leq j \leq n)
$$
do đó tạo thành một hệ cơ bản; nếu đồng nhất $C(t, t_0)$ với ma trận của nó đối với cơ sở $(\mathbf{e}_j)$ thì các tích phân $\mathbf{u}_j$ chính xác là các *cột* của ma trận $C(t, t_0)$. Tích phân của (4) nhận giá trị $\mathbf{x}_0 = \sum_{j=1}^n \lambda_j \mathbf{e}_j$ tại điểm $t_0$ khi đó là $C(t, t_0).\mathbf{x}_0 = \sum_{k=1}^n \lambda_k \mathbf{u}_k(t)$.

Cho *bất kỳ* $n$ tích phân nào $\mathbf{u}_j$ ($1 \leq j \leq n$) của (4), ta gọi *định thức* của $n$ tích phân này tại một điểm $t \in J$ đối với một cơ sở $(\mathbf{e}_j)_{1 \leq j \leq n}$ của $E$ là định thức
$$
\Delta(t) = (\mathbf{u}_1(t), \ \mathbf{u}_2(t), \ \ldots, \ \mathbf{u}_n(t))
$$
của $n$ vectơ $\mathbf{u}_j(t)$ đối với cơ sở $(\mathbf{e}_j)$ (*Alg.*, III, p. 522). Ta có (*Alg.*, III, p. 523, mệnh đề 2)
$$
\Delta(t) = \Delta(t_0) \det \left( C(t, t_0) \right).
$$

Theo mệnh đề 4 của IV, p. 184, để $(\mathbf{u}_j)_{1 \leq j \leq n}$ là một hệ cơ bản các tích phân của (4) thì điều kiện cần và đủ là định thức $\Delta(t)$ của các $\mathbf{u}_j$ là $\neq 0$ tại một điểm nào đó $t_0$ của $J$; công thức (14) khi đó cho thấy rằng $\Delta(t) \neq 0$ tại mọi điểm của $J$, nói cách khác, các vectơ $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) luôn luôn độc lập tuyến tính.

#### Mệnh đề 5 {#fvr-iv-s2-prop-5 .statement}

*Định thức của ma trận $C(t, t_0)$ được cho bởi công thức*
$$
\det \left( C(t, t_0) \right) = \exp \left( \int_{t_0}^t \operatorname{Tr}(A(s)) \, ds \right).
$$
(15)

Thật vậy, nếu đặt $\delta(t) = \det \left( C(t, t_0) \right)$ thì theo công thức đạo hàm của một định thức (I, p. 8, công thức (3)) ta có
$$
\frac{d \delta}{dt} = \operatorname{Tr} \left( \frac{dC(t, t_0)}{dt} (C(t, t_0))^{-1} \right) \delta(t)
$$

nghĩa là, theo phương trình vi phân (5) của IV, p. 179 mà $C(t, t_0)$ thỏa mãn,

$$
\frac{d \delta}{dt} = \operatorname{Tr}(A(t)) \delta(t).
$$

Vì $\delta(t_0) = 1$ nên công thức (15) suy ra từ biểu thức (12) (IV, p. 183) của tích phân của một phương trình tuyến tính vô hướng.

Như ta vừa thấy, việc chỉ rõ $n$ tích phân độc lập tuyến tính của (4) xác định tất cả các tích phân của phương trình này. Bây giờ ta sẽ chỉ ra rằng với $1 \leq p \leq n$, việc biết $p$ tích phân độc lập tuyến tính $\mathbf{u}_j$ ($1 \leq j \leq p$) của phương trình (4) quy việc tích phân phương trình này về việc tích phân một hệ tuyến tính thuần nhất gồm $n - p$ phương trình vô hướng. Giả sử rằng trên một khoảng $K \subset J$ có $n - p$ ánh xạ

$$
\mathbf{u}_{p+k} \quad (1 \leq k \leq n - p)
$$

từ $K$ vào $E$, là các nguyên hàm của các hàm điều chỉnh trên $K$, và sao cho, với mọi $t \in K$, $n$ vectơ $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) tạo thành một cơ sở của $E$.

Với mọi điểm $t_1 \in J$ luôn tồn tại một khoảng $K$, một lân cận của $t_1$ trong $J$, trên đó xác định được $n - p$ hàm $\mathbf{u}_{p+k}$ ($1 \leq k \leq n - p$) có các tính chất trên. Thật vậy, cho $(\mathbf{e}_i)_{1 \leq i \leq n}$ là một cơ sở của $E$; tồn tại $n - p$ vectơ của cơ sở này cùng với các $\mathbf{u}_j(t_1)$ ($1 \leq j \leq p$) tạo thành một cơ sở của $E$ (Alg., II, p. 292, th. 2); giả sử chẳng hạn đó là $\mathbf{e}_{p+1}, \ldots, \mathbf{e}_n$; vì định thức $\det(\mathbf{u}_1(t), \ldots, \mathbf{u}_p(t), \mathbf{e}_{p+1}, \ldots, \mathbf{e}_n)$ (đối với cơ sở $(\mathbf{e}_i)$) là một hàm liên tục của $t$ và không triệt tiêu tại $t = t_1$ nên tồn tại một lân cận $K$ của $t_1$ trên đó nó không triệt tiêu; khi đó có thể lấy $\mathbf{u}_{p+k}(t) = \mathbf{e}_{p+k}$ ($1 \leq k \leq n - p$) với $t \in K$.

Tồn tại một ma trận khả nghịch $B(t)$ cấp $n$, mà các phần tử là những nguyên hàm của các hàm điều chỉnh trên $K$, sao cho $B(t).\mathbf{e}_j = \mathbf{u}_j(t)$ với $1 \leq j \leq n$. Đặt $x = B(t).y$; khi đó $y$ thỏa mãn phương trình $\frac{dB}{dt}.y + B(t).\frac{dy}{dt} = A(t)B(t).y$, phương trình này cũng có thể viết là

$$
\frac{dy}{dt} = (B(t))^{-1} \left( A(t)B(t) - \frac{dB}{dt} \right) .y = H(t).y
$$

trong đó $H(t) = (h_{jk}(t))$ là một ma trận có các phần tử điều chỉnh trên $K$. Theo định nghĩa của $B(t)$ phương trình tuyến tính này nhận $p$ vectơ hằng $\mathbf{e}_j$ ($1 \leq j \leq p$) làm nghiệm; ngay lập tức suy ra rằng tất yếu $h_{jk}(t) = 0$ với $1 \leq k \leq p$; do đó các thành phần $y_k$ của $y$ (đối với cơ sở $(\mathbf{e}_i)$) có chỉ số $k \geq p + 1$ thỏa mãn một hệ tuyến tính thuần nhất gồm $n - p$ phương trình; một khi các nghiệm của hệ này được xác định, thì các $dy_j/dt$ với các chỉ số $j \leq p$ là các hàm tuyến tính của các $y_k$ với $k \geq p + 1$, nên được biết, và các nguyên hàm của các hàm này sẽ cho các $y_j$ với các chỉ số $j \leq p$.

Đặc biệt, khi người ta biết $n - 1$ tích phân độc lập tuyến tính của phương trình (4) của IV, p. 183, thì việc tích phân phương trình này quy về việc tích phân một phương trình vô hướng thuần nhất duy nhất, rồi tính $n$ nguyên hàm.

#### Nhận xét 1 {#fvr-iv-s2-n4-rem-1 .statement}

Tất cả những điều trên cũng áp dụng cho trường hợp E có chiều $n$ trên trường $\mathbf{R}$ và $A(t)$ là một tự đồng cấu của E với mọi $t \in J$: chỉ cần thay thế $\mathbf{C}$ bởi $\mathbf{R}$ ở khắp nơi.

#### Nhận xét 2 {#fvr-iv-s2-n4-rem-2 .statement}

Cho $A(t) = (a_{ij}(t))$ là một ma trận bình phương cấp $n$ mà các phần tử là những hàm điều hòa phải thực (tương ứng, phức) của $t$ trên $J$, và cho $C(t, t_0) = (c_{ij}(t, t_0))$ là ma trận giải thức của hệ tuyến tính tương ứng (3) (IV, p. 22). Cho F là một không gian định chuẩn đầy đủ tùy ý trên $\mathbf{R}$ (tương ứng, $\mathbf{C}$) và xét hệ phương trình vi phân tuyến tính

$$
\frac{dy_i}{dt} = \sum_{j=1}^n a_{ij}(t) y_j
$$

trong đó các hàm chưa biết $y_j$, nhận giá trị trong F. Ngay lập tức thấy rằng nghiệm $(\mathbf{u}_j)_{1 \leq j \leq n}$ của hệ này sao cho $\mathbf{u}_j(t_0) = \mathbf{d}_j$ với $1 \leq j \leq n$ ($\mathbf{d}_j$ tùy ý trong F) được cho bởi các công thức

$$
\mathbf{u}_i(t) = \sum_{j=1}^n c_{ij}(t, t_0) \mathbf{d}_j \qquad (1 \leq i \leq n).
$$

Ta đặc biệt xét trường hợp $A(t)$ là một tự đồng cấu của một không gian vectơ E có số chiều hữu hạn $n$ trên $\mathbf{C}$, sao cho tồn tại một cơ sở của E đối với đó ma trận của $A(t)$ có các phần tử thực với mọi $t \in J$. Khi đó điều trên cho thấy (theo đl. 1 của IV, p. 179) rằng ma trận giải thức $C(t, t_0)$ đối với cùng cơ sở ấy cũng có các phần tử thực: chỉ cần xét không gian vectơ $E_0$ trên $\mathbf{R}$ được sinh bởi cơ sở của E đang xét, và nhận xét rằng hạn chế của $A(t)$ lên $E_0$ là một tự đồng cấu của không gian vectơ này.

### 5. PHƯƠNG TRÌNH LIÊN HỢP

Vẫn giả thiết rằng không gian E có số chiều hữu hạn $n$ trên $\mathbf{C}$, ký hiệu $E^*$ là đối ngẫu của nó (A, II, p. 40), đó là một không gian có chiều $n$ trên $\mathbf{C}$ (Alg., II, p. 299, đl. 4); dạng song tuyến tính chính tắc $\langle \mathbf{x}, \mathbf{x}^* \rangle$ xác định trên $E \times E^*$ (Alg., II, p. 234) là liên tục trên tích này (vì nó là một đa thức theo các thành phần của $\mathbf{x} \in E$ và $\mathbf{x}^* \in E^*$).

Cho một phương trình tuyến tính thuần nhất (4) (IV, p. 183), trong đó $t \mapsto A(t)$ là một ánh xạ điều hòa phải từ J vào $\mathcal{L}(E)$, ta hãy xét xem có tồn tại một ánh xạ $t \mapsto \mathbf{v}(t)$ từ J vào $E^*$, là một nguyên hàm của một hàm điều hòa phải trên J, và sao cho hàm vô hướng $t \mapsto \langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ là hằng trên J khi $\mathbf{u}$ là một nghiệm tùy ý của (4); điều đó tương đương với việc viết rằng đạo hàm của hàm này phải bằng không tại mọi điểm mà $\mathbf{u}$ và $\mathbf{v}$ khả vi, nghĩa là, phải có

$$
\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle + \left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} \right\rangle = 0
$$

tại những điểm như vậy.

Bây giờ, theo (4), $\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle = \langle A(t).\mathbf{u}(t), \mathbf{v}(t) \rangle = -\langle \mathbf{u}(t), B(t).\mathbf{v}(t) \rangle$ trong đó $-B(t)$ là chuyển vị của $A(t)$ (Alg., II, p. 234). Do đó quan hệ mà $\mathbf{v}$ phải thỏa mãn có thể viết là

$$
\left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0
$$

tại mọi điểm mà $A(t)$ liên tục và $\mathbf{v}(t)$ khả vi. Bây giờ với một điểm như thế $t$ và một điểm *tùy ý* $\mathbf{x}_0 \in \mathrm{E}$, theo đ. lý 1 của IV, p. 179, tồn tại một nghiệm $\mathbf{u}$ của (4) sao cho $\mathbf{u}(t) = \mathbf{x}_0$; do đó tất phải có $\left\langle \mathbf{x}_0, \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0$ với *mọi* $\mathbf{x}_0 \in \mathrm{E}$, điều này kéo theo $\frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) = 0$. Do đó:

#### Mệnh đề 6 {#fvr-iv-s2-prop-6 .statement}

*Ánh xạ $t \mapsto \mathbf{v}(t)$ từ J vào $\mathrm{E}^*$, là một nguyên hàm của một hàm bị chặn trên J, có tính chất là $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ là hằng trên J đối với mọi nghiệm $\mathbf{u}$ của phương trình* (4) *của IV, p. 183 khi và chỉ khi $\mathbf{v}$ là một nghiệm của phương trình tuyến tính thuần nhất*

$$
\frac{d\mathbf{x}}{dt} = B(t).\mathbf{x} \tag{16}
$$

*trong đó $-B(t)$ là chuyển vị của $A(t)$.*

Phương trình (16) được gọi là *liên hợp* của (4); rõ ràng (4) là liên hợp của (16). Vì các phần tử của ma trận $B(t)$ là những hàm bị chặn theo $t$ trên J, các kết quả thu được ở trên về các phương trình tuyến tính áp dụng được cho (16). Đặc biệt, tích phân của (16) nhận giá trị $\mathbf{x}_0^*$ tại điểm $t_0$ có thể viết dưới dạng $H(t, t_0).\mathbf{x}_0^*$, trong đó $H(t, t_0)$ là một ánh xạ tuyến tính song ánh của $\mathrm{E}^*$ lên chính nó, đồng nhất với tích phân của phương trình

$$
\frac{dV}{dt} = B(t)V \tag{17}
$$

nhận giá trị $I$ tại điểm $t_0$. Do đó ta có (với ký hiệu của IV, p. 179)

$$
\left\langle C(t, t_0).\mathbf{x}_0, H(t, t_0).\mathbf{x}_0^* \right\rangle = \left\langle \mathbf{x}_0, \mathbf{x}_0^* \right\rangle
$$

với mọi $\mathbf{x}_0 \in \mathrm{E}$ và $\mathbf{x}_0^* \in \mathrm{E}^*$, điều này cho thấy

$$
H(t, t_0) = \check{C}(t, t_0) \tag{18}
$$

(phản biến của $C(t, t_0)$). Đặc biệt, nếu người ta biết một hệ cơ bản các tích phân của phương trình liên hợp (16) thì ma trận $H(t, t_0)$ được xác định, $C(t, t_0)$ cũng vậy, và do đó, *mọi* tích phân của phương trình (4) cũng được xác định.

#### Nhận xét {#fvr-iv-s2-n5-rem-1 .statement}

Cho E và F là hai không gian định chuẩn đầy đủ trên $\mathbf{R}$ (hoặc trên $\mathbf{C}$), và $(\mathbf{x}, \mathbf{y}) \mapsto \langle \mathbf{x}, \mathbf{y} \rangle$ là một dạng song tuyến tính *liên tục* trên $\mathrm{E} \times \mathrm{F}$, sao cho quan hệ “$\langle \mathbf{x}, \mathbf{y} \rangle = 0$ với mọi $\mathbf{y} \in \mathrm{F}$” (resp. $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ với mọi $\mathbf{x} \in \mathrm{E}$”) kéo theo $\mathbf{x} = 0$ (resp. $\mathbf{y} = 0$). Giả sử thêm rằng với mọi $t \in \mathrm{J}$ có một ánh xạ tuyến tính liên tục $B(t)$ của F vào chính nó, sao cho $\langle A(t).\mathbf{x}, \mathbf{y} \rangle + \langle \mathbf{x}, B(t).\mathbf{y} \rangle = 0$ với mọi $(\mathbf{x}, \mathbf{y}) \in \mathrm{E} \times \mathrm{F}$. Trong những điều kiện ấy, ta thấy như trước rằng để một ánh xạ $t \mapsto \mathbf{v}(t)$ từ J vào F, là một nguyên hàm của một hàm bị chặn, có tính chất là $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ là *hằng* đối với *mọi* tích phân $\mathbf{u}$ của (4), điều kiện cần và đủ là $\mathbf{v}$ phải là một tích phân của (16), phương trình mà ta lại gọi là *liên hợp* của (4).

### 6. PHƯƠNG TRÌNH VI PHÂN TUYẾN TÍNH VỚI HỆ SỐ HẰNG

Lại giả sử rằng E là một không gian định chuẩn đầy đủ tùy ý trên $\mathbf{R}$; cho A là một tự đồng cấu liên tục của A, độc lập với t, và xét phương trình tuyến tính thuần nhất

$$
\frac{d\mathbf{x}}{dt} = A.\mathbf{x}.
$$

Khi E có số chiều hữu hạn thì phương trình (19) tương đương với một hệ thuần nhất (3) (IV, p. 183) các phương trình vi phân vô hướng, trong đó các hệ số $a_{ij}$ là hằng.

Theo đ. lý 1 (IV, p. 179), mọi tích phân của (19) đều được xác định trên toàn bộ $\mathbf{R}$; theo đ. lý 2 (IV, p. 179), tích phân của (19) nhận giá trị $\mathbf{x}_0$ tại một điểm $t_0 \in \mathbf{R}$ có thể viết dưới dạng $C(t, t_0)\mathbf{x}_0$, trong đó $C(t, t_0)$ là một ánh xạ tuyến tính song ánh hai phía liên tục của E lên chính nó thỏa mãn phương trình

$$
\frac{dU}{dt} = AU
$$

và sao cho $C(t_0, t_0) = I$. Hơn nữa, ta có đồng nhất thức

$$
C(t + \tau, t_0 + \tau) = C(t, t_0)
$$

với mọi $\tau \in \mathbf{R}$: thật vậy, ta có $dC(s, t_0 + \tau)/ds = AC(s, t_0 + \tau)$ theo (20), và vì A là hằng nên ta cũng có

$$
\frac{dC(t + \tau, t_0 + \tau)}{dt} = AC(t + \tau, t_0 + \tau);
$$

hơn nữa

$$
C(t_0 + \tau, t_0 + \tau) = I = C(t_0, t_0).
$$

do đó ta được đồng nhất thức (21), vì nghiệm của (20) nhận giá trị I tại điểm $t_0$ là duy nhất.

Nếu đặt $C_0(t) = C(t, 0)$ thì $C(t, t_0) = C_0(t - t_0)$; hơn nữa, với mọi $\lambda \in \mathbf{R}$, $C_0(\lambda t)$ trùng với nghiệm của phương trình

$$
\frac{dU}{dt} = \lambda AU
$$

nhận giá trị I tại điểm 0. Ta đưa vào định nghĩa sau:

#### Định nghĩa 1 {#fvr-iv-s2-def-1 .statement}

*Cho A là một tự đồng cấu liên tục của E, ta ký hiệu bởi $e^A$ hoặc $\exp A$ tự đẳng cấu của E bằng giá trị tại điểm $t = 1$ của nghiệm của phương trình (20) nhận giá trị I tại điểm $t = 0$.*

Với ký hiệu này, các nhận xét đứng trước định nghĩa 1 cho thấy rằng

$$
C(t, t_0) = \exp \left( A(t - t_0) \right).
$$

Ký hiệu hàm mũ vừa đưa vào được biện minh bởi các tính chất sau, hoàn toàn tương tự với các tính chất của hàm exp z, với z thực hoặc phức (xem III, p. 98 và 106):

#### Mệnh đề 7 {#fvr-iv-s2-prop-7 .statement}

1' *Ánh xạ* $X \mapsto e^X$ *là một ánh xạ liên tục từ* $\mathcal{L}(E)$ *vào nhóm các tự đẳng cấu của* E *(các phần tử khả nghịch của* $\mathcal{L}(E)$).

2 *Ánh xạ* $t \mapsto e^{Xt}$ *từ* $\mathbf{R}$ *vào* $\mathcal{L}(E)$ *là khả vi, và*

$$
\frac{d}{dt} (e^{Xt}) = X e^{Xt} = e^{Xt} X.
$$ (24)

3 *Với mọi* $X \in \mathcal{L}(E)$ *ta có*

$$
e^X = \sum_{n=0}^{\infty} \frac{X^n}{n!}
$$ (25)

*vế phải hội tụ tuyệt đối và đều trên mọi tập con bị chặn của* $\mathcal{L}(E)$; *đặc biệt,* $e^{It} = e^t I$ *với* $t \in \mathbf{R}$.

4) *Nếu* X *và* Y *giao hoán thì* Y *và* $e^Y$ *giao hoán với* $e^X$, *và*

$$
e^{X+Y} = e^X e^Y.
$$ (26)

Quan hệ (24) suy ra từ biểu thức (23) của $C(t, 0)$ và từ việc hàm này là một nghiệm của (20); bằng phép truy hồi theo n, từ (24) ta suy ra rằng $t \mapsto e^{Xt}$ khả vi vô hạn trên $\mathbf{R}$ và rằng

$$
D^n (e^{Xt}) = X^n e^{Xt}.
$$

Do đó, theo công thức Taylor, ta có thể viết

$$
e^X = I + \frac{X}{1!} + \frac{X^2}{2!} + \cdots + \frac{X^n}{n!} + X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt.
$$ (27)

Mặt khác, hệ quả 3 của IV, p. 181 cho thấy rằng $\| e^{Xt} \| \leq \exp (\| X \| |t| )$. Vậy số dư $r_n(X) = X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt$ trong công thức (27) thỏa mãn bất đẳng thức

$$
\| r_n(X) \| \leq \frac{\| X \|^{n+1}}{(n+1)!} e^{\| X \| }
$$

do đó ta suy ra công thức (25), chuỗi ở vế phải hội tụ tuyệt đối và đều trên mọi tập con bị chặn của $\mathcal{L}(E)$. Với mọi cặp phần tử $X,\ T$ của $\mathcal{L}(E)$, do đó ta có

$$
e^{X+T} - e^X = \sum_{n=1}^{\infty} \frac{1}{n!} ((X+T)^n - X^n ).
$$

Bây giờ, ta có thể viết $(X + T)^n - X^n = \sum_{(V_i)} V_1 V_2 \ldots V_n$, trong đó tổng lấy trên $2^n - 1$ dãy $(V_i)$ các phần tử của $\mathcal{L}(E)$ sao cho $V_i = X$ hoặc $V_i = T$ với $1 \leq i \leq n$, và ít nhất một trong các $V_i$ bằng $T$; bất đẳng thức
$$
\|(X + T)^n - X^n\| \leq (\|X\| + \|T\|)^n - \|X\|^n
$$
suy ra ngay lập tức, do đó
$$
\|\exp(X + T) - \exp X\| \leq \exp \left( \|X\| + \|T\| \right) - \exp \|X\|
$$
điều này thiết lập tính liên tục của ánh xạ $X \mapsto \exp X$.

Cuối cùng, nếu $X$ và $Y$ giao hoán, thì $Y$ giao hoán với $e^{Xt}$ (IV, p. 181, prop. 2), do đó
$$
\frac{d}{dt} (e^{Xt} e^{Yt}) = X e^{Xt} e^{Yt} + e^{Xt} (Y e^{Yt}) = (X + Y) e^{Xt} e^{Yt}.
$$
Mặt khác, vì $e^{Xt} e^{Yt}$ bằng $I$ khi $t = 0$, nên ta có $e^{Xt} e^{Yt} = e^{(X+Y)t}$, do đó có công thức (26). Từ công thức sau này, đặc biệt suy ra rằng với mọi $s$ và $t$ thực tùy ý, ta có
$$
e^{X(s+t)} = e^{Xs} e^{Xt}
$$
và cũng có
$$
e^{-X} = (e^X)^{-1}.
$$

Ngược lại, ta nhận thấy rằng (26) không nhất thiết còn đúng nếu không còn giả thiết $X$ và $Y$ giao hoán: thật vậy, nó sẽ kéo theo rằng $\exp X$ và $\exp Y$ luôn luôn giao hoán, điều này không đúng, như được chỉ ra bởi những ví dụ đơn giản (IV, p. 204, exerc. 3).

Bây giờ giả sử rằng $E$ là một không gian vectơ *có số chiều hữu hạn trên trường* $\mathbf{C}$, và $A$ là một tự đồng cấu của $E$ (đối với cấu trúc không gian vectơ trên $\mathbf{C}$) mà ta có thể đồng nhất với ma trận của nó đối với một cơ sở của $E$; khi đó, với mọi $t \in \mathbf{R}$, $e^{At}$ là một tự đẳng cấu của $E$ đối với cùng cấu trúc ấy (IV, p. 181, prop. 2). Gọi $r_k$ ($1 \leq k \leq q$) là các nghiệm phân biệt (trong $\mathbf{C}$) của *đa thức đặc trưng* $\varphi(r) = \det(A - rI)$ của tự đồng cấu $A$ (các “nghiệm đặc trưng” của $A$); nếu $n_k$ là cấp bội số của $r_k$ thì $\sum_{k=1}^q n_k = n$. Ta biết rằng (Alg., VII, 31, n° 3) với mỗi nghiệm $r_k$ tương ứng một không gian con $E_k$ của $E$, có chiều $n_k$, sao cho $E_k$ *ổn định* dưới $A$, và $E$ là *tổng trực tiếp* của các $E_k$: $E_k$ có thể được định nghĩa là không gian con các vectơ $\mathbf{x}$ sao cho
$$
(A - r_k I)^{n_k} . \mathbf{x} = 0.
$$
Gọi $\mathbf{a}$ là một vectơ bất kỳ trong $E$; ta có thể viết $\mathbf{a} = \sum_{k=1}^q \mathbf{a}_k$, trong đó $\mathbf{a}_k \in E_k$; do đó, tích phân của phương trình (19) trong IV, p. 188, nhận giá trị $\mathbf{a}$ tại điểm $t = 0$ được cho bởi
$$
\mathbf{u}(t) = e^{At} . \mathbf{a} = \sum_{k=1}^q e^{At} . \mathbf{a}_k = \sum_{k=1}^q e^{r_k t} e^{(A - r_k I)t} . \mathbf{a}_k.
$$

Nhưng vì $\mathbf{a}_k \in E_k$ nên ta có

$$
e^{(A - r_k I)t} \cdot \mathbf{a}_k = \mathbf{a}_k + \frac{t}{1!}(A - r_k I) \cdot \mathbf{a}_k + \frac{t^2}{2!}(A - r_k I)^2 \cdot \mathbf{a}_k + \cdots
$$
$$
+ \frac{t^{n_k - 1}}{(n_k - 1)!}(A - r_k I)^{n_k - 1} \cdot \mathbf{a}_k .
$$

Vậy mọi tích phân của phương trình (19) trong IV, p. 188, đều có thể viết thành

$$
\mathbf{u}(t) = \sum_{k=1}^q e^{r_k t} \mathbf{p}_k(t)
$$

trong đó $\mathbf{p}_k(t)$ là một đa thức theo $t$, với các hệ số trong không gian vectơ $E_k$, và bậc $\leq n_k - 1$. Đặc biệt, nếu mọi nghiệm của phương trình đặc số của $A$ đều *đơn*, thì các không gian $E_k$ ($1 \leq k \leq n$) đều có chiều 1 trên trường $\mathbf{C}$, do đó tồn tại $n$ vectơ $c_k$ sao cho $n$ hàm $e^{r_k t} c_k$ ($1 \leq k \leq n$) lập thành một hệ cơ bản các nghiệm của phương trình (19) ở IV, p. 188.

Các nghiệm đặc số của tự đồng cấu $A$ cũng được gọi là *nghiệm đặc số của phương trình tuyến tính* (19) ở IV, p. 188. Có thể nhận thấy rằng ta thu được phương trình đặc số của $A$ bằng cách viết rằng hàm $c e^{r t}$ là một nghiệm của (19) đối với một vectơ $c \neq 0$.

Khi người ta đã xác định tường minh các nghiệm $r_k$ ($1 \leq k \leq q$), và do đó cả cấp bội số $n_k$ của $r_k$, thì trên thực tế người ta thu được các nghiệm của (19) bằng cách viết rằng phương trình này được thỏa mãn bởi biểu thức (32) ở IV, p. 191, trong đó $\mathbf{p}_k$ là một đa thức tùy ý bậc $\leq n_k - 1$, với các hệ số *trong* $E$; khi đồng nhất các hệ số của $e^{r_k t}$ (với $1 \leq k \leq q$) ở hai vế của phương trình thu được như vậy, ta được các phương trình tuyến tính đối với các hệ số của các đa thức $\mathbf{p}_k$: dễ dàng chứng minh rằng các phương trình ấy xác định các số hạng bậc $> 0$ của $\mathbf{p}_k$ như những hàm của số hạng hằng, và số hạng hằng này là một nghiệm của phương trình $(A - r_k I)^{n_k} \cdot \mathbf{x} = 0$, phương trình xác định không gian con $E_k$ (phương pháp "hệ số bất định").

#### Nhận xét {#fvr-iv-s2-n6-rem-1 .statement}

Khi tồn tại một cơ sở của $E$ sao cho ma trận của $A$ đối với cơ sở này có các phần tử *thực* (*xem* IV, p. 186, *Nhận xét* 2), thì phương trình đặc trưng của $A$ có các hệ số thực. Với mọi $\mathbf{x} = (\xi_k)_{1 \leq k \leq n}$ của $E$, được biểu thị trong cơ sở đang xét, đặt $\overline{\mathbf{x}} = (\overline{\xi}_k)_{1 \leq k \leq n}$; ánh xạ $\mathbf{x} \mapsto \overline{\mathbf{x}}$ là một phép tự hợp phản tuyến tính của $E$. Ta biết (*Đại số*, VII) rằng, nếu $r_k$ là một nghiệm không thực của phương trình đặc trưng, và $E_k$ là không gian con ổn định tương ứng, thì $\overline{r}_k$ là một nghiệm đặc trưng có cùng bội số $n_k$ như $r_k$, và ảnh $E'_k$ của $E_k$ dưới ánh xạ $\mathbf{x} \mapsto \overline{\mathbf{x}}$ là không gian con ổn định tương ứng với $\overline{r}_k$. Từ đó suy ra rằng nếu $\mathbf{u}_j$ ($1 \leq j \leq n_k$) là $n_k$ nghiệm độc lập tuyến tính nhận giá trị trong $E_k$, thì $2n_k$ nghiệm $\mathbf{u}_j + \overline{\mathbf{u}}_j,\ i(\mathbf{u}_j - \overline{\mathbf{u}}_j)$ là độc lập tuyến tính, và có, đối với cơ sở đã chọn của $E$, các thành phần là những hàm *thực* của E. Nếu $r_k$ là một nghiệm đặc trưng thực thì *Nhận xét* 2 của IV, p. 186, chỉ ra rằng (với cùng ký hiệu) có $n_k$ nghiệm độc lập tuyến tính $\mathbf{v}_j$ ($1 \leq j \leq n_k$) nhận giá trị trong $E_k$ mà các thành phần của chúng là thực. Bằng cách đó ta thu được một hệ nghiệm cơ bản của (19) mà mọi thành phần đều *thực*.

### 7. PHƯƠNG TRÌNH TUYẾN TÍNH CẤP $n$

Người ta gọi *phương trình vi phân tuyến tính cấp* $n$ là một phương trình có dạng

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = b(t)
$$

trong đó các $a_k$ ($1 \leq k \leq n$) và $b$ là những hàm thực (phức) của biến thực $t$, xác định trên một khoảng $J$ của $\mathbf{R}$. Quy trình tổng quát của IV, p. 164 cho thấy rằng phương trình này tương đương với hệ tuyến tính gồm $n$ phương trình cấp một

$$
\left\{
\begin{aligned}
\frac{dx_k}{dt} &= x_{k+1} & (1 \leq k \leq n-1) \\
\frac{dx_n}{dt} &= a_1(t)x_n + a_2(t)x_{n-1} + \cdots + a_n(t)x_1 + b(t)
\end{aligned}
\right.
$$

nghĩa là, với phương trình tuyến tính

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

trong đó ta đã đặt $\mathbf{x} = (x_1, x_2, \ldots, x_n) \in \mathbf{C}^n$, $\mathbf{b}(t) = (0, 0, \ldots, 0, b(t))$, và trong đó ma trận $A(t)$ được xác định bởi

$$
A(t) = \begin{pmatrix}
0 & 1 & 0 & \ldots & 0 \\
0 & 0 & 1 & \ldots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \ldots & 1 \\
a_n(t) & a_{n-1}(t) & a_{n-2}(t) & \ldots & a_1(t)
\end{pmatrix}.
$$

Do đó việc nghiên cứu phương trình tuyến tính cấp $n$ quy về việc áp dụng các kết quả tổng quát ở trên cho phương trình tuyến tính riêng biệt (35). Với mọi khoảng $J$ trên đó các hàm $a_j$ ($1 \leq j \leq n$) và $b$ là *điều chỉnh*, tồn tại một và chỉ một hàm $u$, xác định trên $J$, có đạo hàm liên tục cấp $n-1$, và đạo hàm *điều chỉnh* cấp $n$ trên khoảng này (trừ tại các điểm của một tập hợp đếm được), thỏa mãn (33) trên phần bù của một tập con đếm được của $J$, và sao cho

$$
u(t_0) = x_0, \qquad Du(t_0) = x_0', \ldots, \quad D^{n-1}u(t_0) = x_0^{(n-1)}
$$

trong đó $t_0$ là một điểm tùy ý của $J$, và $x_0, x_0', \ldots, x_0^{(n-1)}$ là $n$ số phức tùy ý.

Để $p$ tích phân $u_j$ ($1 \leq j \leq p$) của phương trình thuần nhất

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = 0
$$

liên kết với (33) độc lập tuyến tính (trong không gian $C(J; \mathbf{C})$ của các ánh xạ liên tục từ $J$ vào $\mathbf{C}$, được xét như một không gian vectơ trên $\mathbf{C}$), điều kiện cần và đủ là $p$ tích phân tương ứng $\mathbf{u}_j = (u_j, Du_j, \ldots, D^{n-1}u_j)$ của phương trình thuần nhất $d\mathbf{x}/dt = A(t).\mathbf{x}$ độc lập tuyến tính (trong không gian $C(J; \mathbf{C}^n)$ của các ánh xạ liên tục từ $J$ vào $\mathbf{C}^n$). Rõ ràng điều kiện này là cần thiết.

Ngược lại, nếu có $n$ hằng số phức $\lambda_j$, không phải tất cả đều bằng không, sao cho $\sum_{j=1}^n \lambda_j u_j(t) = 0$ đồng nhất trên $J$, thì suy ra $\sum_{j=1}^n \lambda_j D^k u_j(t) = 0$ trên $J$ với mọi số nguyên $k$ sao cho $1 \leq k \leq n - 1$, điều đó có nghĩa là $\sum_{j=1}^n \lambda_j \mathbf{u}_j(t) = 0$ trên $J$.

Do đó (IV, p. 180, hệ quả 1)

#### Mệnh đề 8 {#fvr-iv-s2-prop-8 .statement}

*Tập hợp các tích phân của phương trình tuyến tính thuần nhất (37), xác định trên $J$, là một không gian vectơ chiều $n$ trên trường $\mathbf{C}$.*

Cho trước tùy ý $n$ tích phân $u_j$ ($1 \leq j \leq n$) của phương trình (37), ta gọi *Wronski* của hệ tích phân này là định thức (đối với cơ sở chính tắc của $\mathbf{C}^n$) của $n$ tích phân tương ứng $\mathbf{u}_j$ của phương trình $d\mathbf{x}/dt = A(t).\mathbf{x}$, nghĩa là hàm

$$
W(t) = \begin{vmatrix}
u_1(t) & u_2(t) & \ldots & u_n(t) \\
Du_1(t) & Du_2(t) & \ldots & Du_n(t) \\
\vdots & \vdots & \ddots & \vdots \\
D^{n-1}u_1(t) & D^{n-1}u_2(t) & \ldots & D^{n-1}u_n(t)
\end{vmatrix}.
$$

Để $n$ tích phân $u_j$ độc lập tuyến tính, điều kiện cần và đủ là $W(t) \neq 0$ trên $J$; hơn nữa, để có điều đó thì chỉ cần $W(t_0) \neq 0$ tại *chỉ một* $t_0$ của $J$ (IV, p. 184, mệnh đề 4); ngoài ra, ta có (IV, p. 184, mệnh đề 5)

$$
W(t) = W(t_0) \exp \left( \int_{t_0}^t a_1(s)\, ds \right).
$$ (38)

Ta đồng nhất toán tử giải $C(t, t_0)$ của phương trình (35) với ma trận của nó đối với cơ sở chính tắc của $\mathbf{C}^n$; khi đó các cột $\mathbf{v}_j(t, t_0)$ ($1 \leq j \leq n$) của ma trận này là $n$ tích phân độc lập tuyến tính

$$
\mathbf{v}_j(t, t_0) = (v_j(t, t_0), Dv_j(t, t_0), \ldots, D^{n-1}v_j(t, t_0))
$$

của phương trình thuần nhất $d\mathbf{x}/dt = A(t).\mathbf{x}$, tương ứng với $n$ tích phân độc lập tuyến tính $v_j(t, t_0)$ của phương trình (37) sao cho

$$
D^{k-1}v_j(t_0, t_0) = \delta_{jk}
$$

(delta Kronecker) đối với $1 \leq j \leq n, 1 \leq k \leq n$ (quy ước đặt $D^0 v_j = v_j$). Đặc biệt suy ra rằng phương pháp biến thiên hằng số (IV, p. 182) áp dụng cho phương trình (35) ở đây cho, như một nghiệm riêng của (33), bằng 0 cùng với $n-1$ đạo hàm đầu của nó tại điểm $t_0$, hàm

$$
w(t) = \int_{t_0}^t v_n(t, s)b(s)\, ds.
$$ (39)

Trong trường hợp riêng của phương trình $D^n x = b(t)$, công thức (39) lại cho công thức biểu diễn nguyên hàm bậc $n$ của hàm điều hòa $b(t)$ triệt tiêu cùng với $n - 1$ đạo hàm đầu của nó tại điểm $t_0$, cụ thể là
$$
w(t) = \int_{t_0}^t b(s) \frac{(t-s)^{n-1}}{(n-1)!} \, ds
$$
(II, p. 62, công thức (19)): nghiệm của $D^n x = 0$ triệt tiêu cùng với $n - 2$ đạo hàm đầu của nó tại điểm $t_0$, và có đạo hàm bậc $n - 1$ bằng 1 tại đó, thực ra là đa thức $(t-t_0)^{n-1}/(n-1)!$.

### 8. PHƯƠNG TRÌNH TUYẾN TÍNH CẤP $n$ VỚI HỆ SỐ HẰNG

Nếu các hệ số $a_j$ trong phương trình (33) là hằng, thì ma trận tương ứng $A$ là hằng; phương trình đặc số thu được bằng cách viết rằng $e^{rt}$ là một nghiệm, điều này cho
$$
r^n - a_1 r^{n-1} - \ldots - a_{n-1} r - a_n = 0.
$$
Gọi $r_j$ ($1 \leq j \leq q$) là các nghiệm phân biệt của phương trình này, và $n_j$ ($1 \leq j \leq q$) là bội số của nghiệm $r_j \left( \sum_{j=1}^q n_j = n \right)$. Theo các kết quả của IV, p. 188 đến 194, với mỗi nghiệm $r_j$ tương ứng, đối với phương trình thuần nhất
$$
D^n x - a_1 D^{n-1} x - \cdots - a_{n-1} D x - a_n x = 0
$$
một hệ gồm $n_j$ nghiệm độc lập tuyến tính
$$
u_{jk}(t) = e^{r_j t} p_{jk}(t),
$$
trong đó $p_{jk}$ là một đa thức (với các hệ số phức) bậc $\leq n_j - 1$ ($1 \leq k \leq n_j$); hơn nữa, $n$ nghiệm $u_{jk}$ ($1 \leq j \leq q,\ 1 \leq k \leq n_j$) thu được như vậy là độc lập tuyến tính. Suy ra rằng $n_j$ đa thức $p_{jk}$ ($1 \leq k \leq n_j$) là độc lập tuyến tính trong không gian các đa thức theo $t$ bậc $\leq n_j - 1$, nên tạo thành một cơ sở (trên $\mathbf{C}$) của không gian này, vì không gian sau có chiều $n_j$. Nói cách khác:

#### Mệnh đề 9 {#fvr-iv-s2-prop-9 .statement}

*Cho $r_j$ ($1 \leq j \leq q$) là các nghiệm phân biệt của phương trình đặc số (40), và cho $n_j$ là bội số của nghiệm $r_j$ ($1 \leq j \leq q$). Khi đó $n$ hàm $t^k e^{r_j t}$ ($1 \leq k \leq n_j,\ 1 \leq j \leq q$) là các nghiệm độc lập tuyến tính của phương trình thuần nhất (41).*

Có thể chứng minh kết quả này trực tiếp theo cách sau. Từ phương trình (41) suy ra rằng đạo hàm bậc $n$ của mọi nghiệm của phương trình này là khả vi trên $\mathbf{R}$, từ đó suy ra ngay lập tức, bằng quy nạp theo số nguyên $m > n$, rằng mọi nghiệm của (41) có đạo hàm cấp $m$, tức là *khả vi vô hạn lần* trên $\mathbf{R}$. Gọi $\mathcal{D}$ là không gian vectơ (không tôpô) trên $\mathbf{C}$ của các hàm nhận giá trị phức, khả vi vô hạn lần trên $\mathbf{R}$; ánh xạ $x \mapsto Dx$ là một tự đồng cấu của không gian này, và phương trình (41) có thể được viết thành

$$
f(D)x = 0 \tag{42}
$$

trong đó $f(D) = D^n - a_1 D^{n-1} - \ldots - a_{n-1} D - a_n$ (Alg., IV, p. 4).

#### Mệnh đề 10 {#fvr-iv-s2-prop-10 .statement}

*Cho g và h là hai đa thức nguyên tố cùng nhau sao cho $f = gh$. Không gian con các nghiệm của (42) là tổng trực tiếp của các không gian con nghiệm của hai phương trình*

$$
g(D)x = 0, \qquad h(D)x = 0.
$$

Thật vậy, theo đồng nhất thức Bezout (Alg., VII. 2, đl. 1), tồn tại hai đa thức $p(D)$ và $q(D)$ sao cho $p(D)g(D) + q(D)h(D) = 1$. Với mọi nghiệm $x$ của (42), ta có thể viết $x = y + z$, trong đó $y = p(D)g(D)x$ và $z = q(D)h(D)x$; khi đó $h(D)y = p(D)(f(D)x) = 0$ và $g(D)z = q(D)(f(D)x) = 0$. Mặt khác, nếu đồng thời có $g(D)x = 0$ và $h(D)x = 0$, thì suy ra rằng

$$
x = p(D)(g(D)x) + q(D)(h(D)x) = 0,
$$

điều đó hoàn tất chứng minh.

Với ký hiệu trên, ta có thể viết

$$
f(D) = \prod_{j=1}^q (D - r_j)^{n_j}
$$

và mệnh đề 10, bằng quy nạp theo $q$, cho thấy rằng không gian con các nghiệm của (42) là tổng trực tiếp của các không gian con nghiệm của $q$ phương trình

$$
(D - r_j)^{n_j} x = 0 \qquad (1 \leq j \leq q). \tag{43}
$$

Bây giờ, với mọi số phức $r$ ta có

$$
D(e^{rt} x) = e^{rt}(D + r)x \tag{44}
$$

nên (43) tương đương với

$$
D^{n_j}(e^{-r_j t} x) = 0
$$

và do đó có các nghiệm là các hàm $e^{r_j t} p_j(t)$, trong đó $p_j$ chạy qua tập hợp các đa thức bậc $\leq n_j - 1$; như vậy ta tìm lại được mệnh đề 9 của IV, p. 194.

Giả sử phương trình thuần nhất (41) đã được giải (nghĩa là giả sử các nghiệm của phương trình đặc số đã được tìm ra), ta biết rằng phương pháp biến thiên hằng số cho phép tìm các nghiệm của phương trình không thuần nhất

$$
D^n x - a_1 D^{n-1} x - \ldots - a_{n-1} Dx - a_n x = b(t) \tag{45}
$$

trong đó $b(t)$ là một hàm bị chặn *tùy ý* (IV, p. 182); chú ý rằng nếu $b(t)$ *khả vi vô hạn lần* trên một khoảng J thì mọi tích phân của (45) đều khả vi vô hạn lần trên J. Trong trường hợp riêng $b(t) = e^{\alpha t} p(t)$, trong đó $p$ là một đa thức (với các hệ số phức) và $\alpha$ là một số phức tùy ý, ta thu được một tích phân của (45) đơn giản hơn bằng phương pháp sau. Đặt $x = e^{\alpha t} y$; phương trình

$$
f(D)x = e^{\alpha t} p(t)
$$

theo (44) có thể viết thành

$$
f(\alpha + D)y = p(t)
$$

hoặc, theo công thức Taylor áp dụng cho đa thức $f(D)$,

$$
\frac{f^{(n)}(\alpha)}{n!} D^n y + \frac{f^{(n-1)}(\alpha)}{(n-1)!} D^{n-1} y + \cdots + \frac{f'(\alpha)}{1!} Dy + f(\alpha) y = p(t). \tag{46}
$$

Gọi $m$ là bậc của đa thức $p(t) = \sum_{k=0}^m \lambda_k t^{m-k}$; nếu $f(\alpha) \neq 0$ (nghĩa là nếu $\alpha$ không phải là một nghiệm của phương trình đặc số), thì tồn tại một và chỉ một đa thức $u(t) = \sum_{k=0}^m c_k t^{m-k}$ *bậc* $m$ là một nghiệm của (46), vì các hệ số $c_k$ được xác định bởi hệ phương trình tuyến tính

$$
f(\alpha)c_k + \binom{m-k+1}{1} f'(\alpha)c_{k-1} + \binom{m-k+2}{2} f''(\alpha)c_{k-2} + \cdots
+ \binom{m}{k} f^{(k)}(\alpha)c_0 = \lambda_k \qquad (0 \leq k \leq m)
$$

mà rõ ràng thừa nhận một và chỉ một nghiệm. Ngược lại, nếu $\alpha$ là một nghiệm của phương trình đặc số, và $h$ là bội số của nó, thì phép tính trên cho thấy rằng tồn tại một và chỉ một đa thức bậc $m$ sao cho mọi nghiệm của $D^h y = v(t)$ đều là một tích phân; nói cách khác, khi đó mọi nghiệm đa thức của (46) đều có bậc $m + h$ ("cộng hưởng").

### 9. HỆ CÁC PHƯƠNG TRÌNH TUYẾN TÍNH VỚI HỆ SỐ HẰNG

Với ký hiệu của số 8, xét tổng quát hơn một hệ gồm $m$ phương trình vi phân dạng

$$
\sum_{k=1}^n p_{jk}(D) x_k = b_j(t) \qquad (1 \leq j \leq m) \tag{47}
$$

trong đó các ẩn $x_k$ ($1 \leq k \leq n$) và các vế phải $b_j$ ($1 \leq j \leq m$) là các hàm phức của biến thực $t$, và trong đó các $p_{jk}(D)$ là các đa thức (bậc tùy ý) với các hệ số *hằng* (phức) theo toán tử vi phân $D$ ($1 \leq j \leq m,\ 1 \leq k \leq n$).

Những hệ như vậy không cùng kiểu với những hệ đã xét trong IV, p. 1164 (công thức (5)), như ví dụ sau đây cho thấy:

$$
\begin{cases}
D x_1 = a(t) \\
D^2 x_1 + D x_2 + x_2 = b(t).
\end{cases}
$$

Ta sẽ giới hạn ở trường hợp các hàm $b_j(t)$ là *khả vi vô hạn* trên khoảng J, và ta sẽ chỉ tìm các nghiệm $(x_k)_{1 \leq k \leq n}$ khả vi vô hạn trên J. Đặt $\mathbf{b}(t) = (b_1(t), \ldots, b_m(t))$, (một ánh xạ từ J vào $\mathbf{C}^m$), và $\mathbf{x} = (x_1, x_2, \ldots, x_n)$, hệ (47) có thể viết thành

$$
P(D) \mathbf{x} = \mathbf{b}(t)
$$

trong đó $P(D)$ là ma trận $(p_{jk}(D))$ có m hàng và n cột, mà các hệ số thuộc vành $\mathbf{C}[D]$ các đa thức theo D, với hệ số trong $\mathbf{C}$. Gọi $f_j(D)$ ($1 \leq j \leq r \leq \operatorname{Min}(m, n)$) là các *bất biến tương tự* khác không của ma trận $P(D)$; như đã biết (*Alg.*, VII, p. 32), đó là các đa thức đơn nhất được xác định rõ, sao cho $f_j$ chia $f_{j+1}$ với $1 \leq j \leq r - 1$ ($r$ là *hạng* của $P(D)$); hơn nữa, tồn tại hai ma trận vuông $U(D)$ và $V(D)$ cấp tương ứng là m và n, *khả nghịch* (trong các vành ma trận vuông cấp tương ứng là m và n, *với hệ số trong vành $\mathbf{C}[D]$ các đa thức theo D với hệ số phức*), và sao cho mọi phần tử của ma trận $Q(D) = (q_{jk}(D)) = U(D) P(D) V(D)$ đều bằng không, trừ các phần tử đường chéo $q_{jj}(D) = f_j(D)$ với $1 \leq j \leq r$. Bây giờ đặt $\mathbf{y} = V^{-1}(D) \mathbf{x}$; phương trình (49) tương đương với phương trình

$$
U(D) (P(D)(V(D) \mathbf{y})) = U(D) \mathbf{b}
$$

nghĩa là,

$$
Q(D) \mathbf{y} = U(D) \mathbf{b}
$$

vì $U(D)$ khả nghịch. Bây giờ, nếu $\mathbf{y} = (y_1, y_2, \ldots, y_n)$, và nếu

$$
U(D) \mathbf{b}(t) = (c_1(t), \ldots, c_m(t)),
$$

thì phương trình (50) có thể viết thành

$$
f_j(D) y_j = c_j(t) \quad \text{với } 1 \leq j \leq r \tag{51}
$$
$$
0 = c_j(t) \quad \text{với } r + 1 \leq j \leq m. \tag{52}
$$

Do đó hệ không có nghiệm khả vi vô hạn nào trừ khi các điều kiện (52) được thỏa mãn; khi đó việc xác định các $y_j$ với chỉ số $j \leq r$ được rút gọn thành việc tích phân r phương trình vi phân tuyến tính hệ số hằng (51); các $y_j$ với chỉ số $> r$ là các hàm khả vi vô hạn tùy ý. Một khi các nghiệm $\mathbf{y}$ của (50) đã được xác định như vậy, ta suy ra các nghiệm của (47) từ công thức $\mathbf{x} = V(D) \mathbf{y}$.

#### Nhận xét 1 {#fvr-iv-s2-n9-rem-1 .statement}

Một số đa thức $f_j(D)$ có thể rút gọn thành các hằng khác không; khi đó các $y_j$ tương ứng được xác định hoàn toàn.

#### Nhận xét 2 {#fvr-iv-s2-n9-rem-2 .statement}

Khi các $b_j$ đều bằng không, nghĩa là, nếu hệ (47) là *thuần nhất*, thì các điều kiện (52) luôn luôn được thỏa mãn; hơn nữa, nếu $r = n$, ta thấy rằng tập hợp các nghiệm của (47) là một không gian vectơ trên $\mathbf{C}$, có chiều bằng *tổng các bậc* của các $f_j(D)$, nghĩa là bằng *bậc* của $\det(P(D))$.

#### Nhận xét 3 {#fvr-iv-s2-n9-rem-3 .statement}

Cho các đa thức $p_{jk}(D)$, một hệ (47) có nghiệm khi các vế phải là khả vi vô hạn (hoặc khả vi đến một cấp nào đó) có thể không có nghiệm khi các vế phải là các hàm điều hòa tùy ý: điều này được chỉ ra bởi ví dụ (48), vốn không có nghiệm khi $a(t)$ không phải là một nguyên hàm. Ở đây ta sẽ không tìm kiếm các điều kiện khả dĩ bổ sung xuất hiện khi các vế phải là các hàm điều hòa tùy ý.

### Bài tập {#fvr-iv-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
