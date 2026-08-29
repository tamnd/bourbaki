---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 3
section_title: Valuations
lang: vi
source: ac-i-vii
book_pages: 385-393, 446-449
pdf_pages: 0403-0411, 0464-0467
extraction: ocr
subsections:
    - "no": 1
      title: VALUATIONS ON A RING
      page: 385
      pdf_page: 403
    - "no": 2
      title: VALUATIONS ON A FIELD
      page: 387
      pdf_page: 405
    - "no": 3
      title: TRANSLATIONS
      page: 389
      pdf_page: 407
    - "no": 4
      title: EXAMPLES OF VALUATIONS
      page: 389
      pdf_page: 407
    - "no": 5
      title: IDEALS OF A VALUATION RING
      page: 391
      pdf_page: 409
    - "no": 6
      title: DISCRETE VALUATIONS
      page: 392
      pdf_page: 410
statements: 15
exercises: 8
content_sha256: 2b82aef8c8710f1de9e584042f511a43db377c9721ef482484075cd1d44e2762
translated_from: content/en/ac/VI/03_s3_valuations.md
source_content_sha256: 7c8006eb587e0c29f6ccf241727bf3ea54908994e1ee0854ab2d41fc36b2d06d
translation_model: gpt-5.4-mini
translation_run: translate-vi-e1600373
glossary_version: 34
glossary_terms_sha256: bab35c85e6b7f354a7a50f16fcf70c1c28d184697464bcf9cfe1b53884b17ecf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. ĐỊNH GIÁ

### 1. ĐỊNH GIÁ TRÊN MỘT VÀNH

Cho $\Gamma$ là một nhóm giao hoán được sắp thứ tự toàn phần viết theo phép cộng. Trong phần còn lại của chương này, ta sẽ phải xét, đối với một nhóm như vậy, tập thu được bằng cách ghép thêm vào $\Gamma$ một phần tử ký hiệu là $+\infty;$ ta sẽ ký hiệu tập này là $\Gamma_\infty$ và sẽ trang bị cho nó: (1) một thứ tự toàn phần sao cho $+\infty$ là phần tử lớn nhất, nói cách khác, sao cho $a < +\infty$ với mọi $a \in \Gamma;$ (2) một cấu trúc monoid giao hoán mà luật của nó cảm sinh trên $\Gamma$ luật nhóm đã cho và được xác định bởi các đẳng thức

$$
(+\infty) + (+\infty) = +\infty, \quad a + (+\infty) = +\infty
$$

với mọi $\alpha \in \Gamma$; ngay lập tức kiểm tra được rằng luật này kết hợp và giao hoán và rằng quan hệ $\alpha_1 \leq \beta$ trong $\Gamma_\infty$ kéo theo $\alpha_1 + \gamma \leq \beta + \gamma$ với mọi $\gamma \in \Gamma_a$.

#### Định nghĩa 1 {#ac-vi-s3-def-1 .statement}

*Cho $C$ là một vành (không nhất thiết giao hoán) và $\Gamma$ là một nhóm giao hoán được sắp thứ tự toàn phần viết theo phép cộng. Một định giá trên $C$ nhận giá trị trong $\Gamma$ là bất kỳ ánh xạ $v : C \to \Gamma_\infty$ thỏa mãn các điều kiện sau:*

(VL_I) $v(xy) = v(x) + v(y)$ với $x \in C, y \in C$.
(VL_{II}) $v(x + y) \geq \inf(v(x), v(y))$ với $x \in C, y \in C$.
(VL_{III}) $v(1) = 0$ và $v(0) = +\infty$.

Nếu $C$ không có ước của $0$ nào khác ngoài $0$, thì ánh xạ duy nhất $v_0$ từ $C$ đến $\Gamma_\infty$ sao cho $v_0(x) = 0$ với $x \neq 0$ và $v_0(0) = +\infty$ là một định giá, gọi là *định giá tầm thường* trên $C$. Nếu $z \in C$ sao cho $z^n = 1$ với một số nguyên $n \geq 1$, thì, theo (VL_I), $nv(z) = v(z^n) = 0$ và do đó $v(z) = 0$ đối với *mọi* định giá $v$ trên $C$, vì $\Gamma$ là một nhóm được sắp thứ tự toàn phần. Đặc biệt $v(-1) = 0$, do đó $v(-x) = v(x)$ với mọi $x \in C$. Hơn nữa, từ (VL_I) suy ra $v(xy) = v(yx)$ với mọi $x, y$ trong $C$. Nếu $x$ khả nghịch trong $C$, thì $v(x^{-1}) = -v(x)$.

#### Mệnh đề 1 {#ac-vi-s3-prop-1 .statement}

*Cho $v$ là một định giá trên một vành (không nhất thiết giao hoán) $C$. Với mọi phần tử $x_i \in C$ ($1 \leq i \leq n$),*

$$
v \left( \sum_{i=1}^n x_i \right) \geq \inf_{1 \leq i \leq n} v(x_i)
$$

Hơn nữa, nếu tồn tại duy nhất một chỉ số $k$ sao cho $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, thì hai vế của (1) bằng nhau. Đặc biệt, nếu $v(x) \neq v(y)$, thì $v(x + y) = \inf(v(x), v(y))$.

Quan hệ (1) suy ra từ tiên đề (VL$_{II}$) bằng quy nạp theo $n$. Nếu tồn tại một chỉ số duy nhất $k$ sao cho $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, thì, viết $y = \sum_{i \neq k} x_i$ và $z = \sum_{i=1}^n x_i$, ta có $v(y) > v(x_k)$ và $v(z) \geq v(x_k)$ theo (1); nếu $v(z) > v(x_k)$, quan hệ $x_k = z - y$ sẽ cho $v(x_k) \geq \inf(v(z), v(y)) > v(x_k)$, điều này là vô lý; do đó $v(z) = v(x_k)$, điều đó chứng minh mệnh đề thứ hai.

#### Hệ quả {#ac-vi-s3-n1-cor-1 .statement}

*Nếu một dãy hữu hạn các phần tử $(x_i)_{1 \leq i \leq n}$ của $C$ (với $n \geq 2$) thỏa mãn $\sum_{i=1}^n x_i = 0$, thì tồn tại ít nhất hai chỉ số phân biệt $j, k$ sao cho*

$$
v(x_j) = v(x_k) = \inf_{1 \leq i \leq n} v(x_i).
$$

Nếu chỉ có một chỉ số duy nhất $k$ sao cho $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, Mệnh đề 1 sẽ cho thấy rằng $v(x_k) = v(0) = +\infty$, do đó $v(x_i) = +\infty$ với mọi $i$, trái với quan hệ $n \geq 2$ và giả thiết đặt lên $k$.

Nhận xét
(1) Nếu $v : C \to \Gamma_\infty$ là một định giá trên $C$ và $u : B \to C$ là một đồng cấu của vành $B$ vào $C$, thì hiển nhiên ánh xạ hợp thành $B \xrightarrow{u} C \xrightarrow{v} \Gamma_\infty$ là một định giá trên $B$ với giá trị trong $\Gamma$.

(2) Các điều kiện (VL$_I$) và (VL$_{II}$) cho thấy ngay lập tức rằng tập hợp $\bar{v}^{-1}(+\infty)$ là một iđêan hai phía $\mathfrak{p}$ trong $C$ phân biệt với $C$ do (VL$_{III}$); hơn nữa, nếu $x, y$ là hai phần tử của $C$ sao cho $v(xy) = +\infty$, thì suy ra từ (VL,) rằng tất yếu $v(x) = +\infty$ hoặc $v(y) = +\infty$; nói cách khác, vành thương $C/\mathfrak{p}$ không có ước 0 nào khác 0; dễ dàng kiểm tra rằng ánh xạ $\bar{v} : C/\mathfrak{p} \to \Gamma_\infty$ dẫn xuất từ $v$ bằng cách chuyển qua thương là một định giá trên $C/\mathfrak{p}$, với ảnh ngược của $+\infty$ dưới định giá này thu gọn thành 0.

### 2. ĐỊNH GIÁ TRÊN MỘT TRƯỜNG

#### Mệnh đề 2 {#ac-vi-s3-prop-2 .statement}

Cho $K$ là một trường (không nhất thiết giao hoán) và $v$ là một định giá trên $K$ với giá trị trong $\Gamma$. Khi đó:
(i) Với $x \neq 0$, $v(x) \neq +\infty$.
(ii) Tập hợp $A$ gồm các $x \in K$ sao cho $v(x) \geq O$ là một vành con của $K$.
(iii) Với mọi $a \geq O$ trong $\Gamma$, tập $V$, (tương ứng $V'_a$) gồm các $x \in A$ sao cho $v(x) > a$ (tương ứng $v(x) \geq a$) là một iđêan hai phía của $A$ và mọi iđêan (trái hoặc phải) $\neq (O)$ của $A$ chứa một trong các $V'_a$.
(iv) Tập $m(A)$ gồm các $x \in A$ sao cho $v(x) > O$ là iđêan lớn nhất \#A trong $A$; $U(A) = A - m(A)$ là tập hợp các phần tử khả nghịch của $A$ và $\kappa(A) := A/m(A)$ là một trường (không nhất thiết giao hoán).
(v) Với mọi $x \in K - A$, $x^{-1} \in m(A)$.

Khẳng định (i) suy ra từ sự kiện là $\bar{v}^{-1}(+\infty)$ là một iđêan của $K$ không bằng $K$. Việc kiểm tra rằng $A$ là một vành và $V$, cùng với $V'_a$ là các iđêan hai phía là tầm thường nhờ các tiên đề (VL$_I$), (VL$_II$) và (VL$_III$). Nếu $a$ là một iđêan (trái, chẳng hạn) của $A$ và $x \neq 0$ thuộc $A$, mọi $y \in A$ sao cho $v(y) \geq v(x)$ đều có thể viết $y = zx$ với $z = yx^{-1}$, do đó $v(z) = v(y) - v(x) \geq O$ và vì thế $z \in A$; nói cách khác iđêan trái $Ax$ chứa các $V'_a$ với $a > v(x)$. Tập hợp $U(A) = A - m(A)$ là tập các $x \in K$ sao cho $v(x) = 0$; nếu $x \in U(A)$, thì
$$
v(x^{-1}) = -v(x) = 0,
$$
do đó $x^{-1} \in U(A)$; ngược lại, nếu $y \in A$ khả nghịch trong $A$, thì $v(y) \geq 0$, $v(y^{-1}) \geq 0$ và $v(y) + v(y^{-1}) = 0$, do đó $v(y) = 0$ và $y \in U(A)$; điều này chứng minh (iv) và (v) suy ra ngay lập tức từ các định nghĩa.

$A$ (tương ứng $m(A)$, $\kappa(A)$) được gọi là vành (tương ứng iđêan, trường thặng dư) của phép định giá $v$ trên $K$.

Rõ ràng $U(A)$ là hạt nhân của đồng cấu $v : K^* \to \Gamma$ và ảnh $v(K^*)$ của nhóm nhân $K^*$ qua $v$ là một nhóm con của nhóm cộng $\Gamma$, được gọi là nhóm thứ tự hay nhóm giá trị của $v$, do đó đẳng cấu với $K^*/U(A)$; với $x \in K$, phần tử $v(x)$ của $\Gamma_\infty$ đôi khi được gọi là phép định giá hay cấp của $x$ đối với $v$. Hai phép định giá $v, v'$ trên $K$ được gọi là tương đương nếu chúng có cùng vành.

#### Mệnh đề 3 {#ac-vi-s3-prop-3 .statement}

*Để hai phép định giá $v, v'$ trên một trường $K$ (không nhất thiết giao hoán) tương đương, điều kiện cần và đủ là tồn tại một đẳng cấu $\lambda$ của nhóm có thứ tự $v(K^*)$ lên nhóm có thứ tự $v'(K^*)$ sao cho $v' = A \circ v$.*

Giả sử $v$ và $v'$ là tương đương; theo giả thiết, vành $A$ của định giá $v$ trùng với vành của $v'$, $v$ và $v'$ (hạn chế trên $K^*$) phân tích thành các đồng cấu $K^* \to K^*/U(A) \xrightarrow{\mu} v(K^*)$, $K^* \to K^*/U(A) \xrightarrow{\nu} v'(K^*)$, trong đó $\mu$ và $\nu$ là các đẳng cấu; hơn nữa, tập các phần tử dương của $v(K^*)$ (tương ứng $v'(K^*)$) là ảnh qua $\mu$ (tương ứng $\nu$) của tập các lớp modulo $U(A)$ của các phần tử $\neq 0$ của $m(A)$; ta kết luận rằng $A = v \circ \mu^{-1}$ giải được bài toán, chiều đảo lại hiển nhiên.

Giả sử nay $K$ là một trường giao hoán; khi đó, với mọi định giá $v$ trên $K$, vành $A$ của định giá $v$ là một vành định giá của $K$ theo nghĩa của § 1, no. 2, Định nghĩa 2 (điều này biện minh cho *thuật ngữ*); điều này suy ra ngay lập tức từ Mệnh đề 2 (c) và § 1 no. 2, Định lý 1 (c). *Ngược lại*, nhắc lại rằng với mọi miền nguyên $B$ có trường phân thức là $K$ thì quan hệ chia hết $x|y$ (tương đương với $y \in Bx$) làm cho $K^*$ thành một nhóm tiền thứ tự, mà *nhóm có thứ tự liên kết* $\Gamma_B$ là thương $K^*/U(B)$ của $K^*$ theo nhóm $U(B)$ gồm các phần tử khả nghịch của $B$, các phần tử dương của nhóm này là các phần tử của $B^*/U(B)$ (trong đó $B^* = B - \{0\}$); ánh xạ $x \mapsto Bx$ xác định, bằng cách chuyển qua thương, một đẳng cấu của nhóm có thứ tự $K^*/U(B)$ lên nhóm (được sắp thứ tự bởi quan hệ $\supset$) các iđêan phân thức chính khác không của $K$ (*Đại số*, Chương VI, § 1, no. 5). Các vành $A$ có trường phân thức $K$ và sao cho nhóm $\Gamma_A = K^*/U(A)$ *được sắp thứ tự toàn phần* chính xác là các *vành định giá của K* (§ 1, no. 2, Định lý 1 (d)). Nếu $v_A$ ký hiệu *đồng cấu chính tắc* của $K^*$ lên $\Gamma_A$, thì hiển nhiên $v_A$ (được mở rộng bởi $v_A(0) = +\infty$) là một định giá (gọi là *chính tắc*) trên $K$ mà vành của nó là $A$; mọi định giá tương đương với $v_A$ có thể viết $v = \sigma \circ v_A$, trong đó $\sigma$ là một đẳng cấu của $\Gamma_A$ lên một nhóm con của nhóm mà $v$ nhận giá trị của nó (Mệnh đề 3); $\sigma \circ v_A$ được gọi là *phân tích chính tắc* của $v$.

#### Mệnh đề 4 {#ac-vi-s3-prop-4 .statement}

*Cho $C$ là một miền nguyên, $K$ là trường phân thức của nó, $C^* = C - \{0\}$ và $v : C \to \Gamma_\infty$ là một định giá trên $C$. Khi đó tồn tại duy nhất một định giá $w$ trên $K$ mở rộng $v$ và $w(K^*)$ là nhóm con của $\Gamma$ được sinh bởi $v(C^*)$.*

Theo Định lý 2 của *Algebra*, Chương I, § 2, no. 7, tồn tại duy nhất một đồng cấu $w$ từ $K^*$ đến $\Gamma$ mở rộng $v|C^*$ và $w(K^*)$ được sinh bởi $v(C^*)$. Còn phải chứng minh rằng $w$ thỏa mãn tiên đề (VL,,). Khi đó, lấy $x' \in K^*, y \in K^*$ sao cho $x + y \in K^*$; tồn tại $a \in \mathbf{C}^*$ sao cho $ax \in \mathbf{C}^*$ và $ay \in \mathbf{C}^*$, do đó $a(x + y) \in \mathbf{C}^*$. Vì hạn chế của $w$ lên $\mathbf{C}^*$ thỏa mãn (VL$_{\text{II}}$),

$$
w(a(x + y)) \geq \inf(w(ax), w(ay)).
$$

Khử $w(a)$ khỏi hai vế, ta được

$$
w(x + y) \geq \inf(w(x), w(y)).
$$

### 3. CÁC BẢN DỊCH

Cho $K$ là một trường (giao hoán), $f$ là một điểm đặt của $K$, $v$ là một định giá trên $K$ và $A$ là một vành định giá của $K$. Ta sẽ nói rằng $A$, $f$ và $v$ là *liên kết* nếu $A$ là vành của $f$ và vành của $v$. Nhờ no. 1 và § 2, no. 3, mỗi trong ba đối tượng $A$, $f$ và $v$ khi đó xác định hai đối tượng còn lại (xét đến tương đương đối với các điểm đặt và các định giá). Đặc biệt, ta có các tương đương sau:

$$
\begin{array}{ccccc}
x \in A & \Leftrightarrow & f(x) \neq \infty \\
x \in m(A) & \Leftrightarrow & f(x) = 0 \\
x \in A - m(A) = U(A) & \Leftrightarrow & f(x) \neq 0 \quad \text{và} \quad f(x) \neq \infty \Leftrightarrow v(x) = 0 \\
x \in K - A & \Leftrightarrow & f(x) = \infty & \Leftrightarrow & v(x) < 0
\end{array}
$$

Mọi kết quả liên quan đến các vành định giá, các điểm đặt hoặc các định giá đều có thể được dịch thành một kết quả liên quan đến hai khái niệm còn lại. Do đó, Mệnh đề 4 của § 2, no. 4 cho:

#### Mệnh đề 5 {#ac-vi-s3-prop-5 .statement}

*Cho $K$ là một trường, $v$ là một định giá trên $K$ và $K'$ là một mở rộng của $K$. Tồn tại một định giá $v'$ trên $K'$ sao cho hạn chế của nó lên $K$ tương đương với $v$.*

Cho $\Gamma_v$ và $\Gamma_{v'}$ là các nhóm giá trị của $v$ và $v'$. Vì hạn chế của $v'$ lên $K$ là tương đương với $v$, nên tồn tại một đẳng cấu $A$ từ $\Gamma_v$ lên một nhóm con của $\Gamma_{v'}$, sao cho $v' = A \circ v$ trên $K$. Nếu $\Gamma_v$ được đồng nhất với $\lambda(\Gamma_v)$ nhờ $\lambda$, thì thấy rằng $v'$ mở rộng $v$.

Lưu ý rằng $\Gamma_{v'}$ nói chung *khác với* $\lambda(\Gamma_v)$ và lớp tương đương của $v'$ không nhất thiết là duy nhất. Chúng ta sẽ trở lại *với* điều này ở § 8.

Dịch Định lý 3 của § 1, no. 3 (hoặc Mệnh đề 6 của § 2, no. 5), ta thu được:

#### Mệnh đề 6 {#ac-vi-s3-prop-6 .statement}

*Cho $K$ là một trường, $A$ là một vành con của $K$ và $x$ là một phần tử của $K$. Để $x$ nguyên trên $A$, điều kiện cần và đủ là mọi định giá trên $K$ dương trên $A$ đều dương tại $x$.*

Từ nay trở đi, nói chung ta sẽ để cho người đọc công việc thực hiện những bản dịch tương tự như trên.

### 4. CÁC VÍ DỤ VỀ ĐỊNH GIÁ

Các ví dụ về vành định giá được cho ở § 1, no. 4 cung cấp cho ta *Ví dụ 1 đến 4* dưới đây:

Ví dụ (1) Mọi định giá trên một trường hữu hạn F đều là tầm thường, vì mọi phần tử của F* đều là một căn của đơn vị.

Ví dụ (2) Nếu K là một trường con của một trường K', thì hạn chế lên K của một định giá trên K' là một định giá trên K.

Ví dụ (3) Cho k là một trường và K = k((T)). Ánh xạ v gán cho mỗi chuỗi lũy thừa hình thức khác không bậc của nó (Đại số, Chương IV, § 5, no. 7) là một định giá trên K mà nhóm giá trị là Z và vành của nó là k[[T]]. Điểm tương ứng là đồng cấu chính tắc f: k[[T]] → k được mở rộng lên k((T)) bằng cách đặt f(u) = ∞ nếu u ∉ k[[T]].

Ví dụ (4) Cho A là một miền iđêan chính, K là trường phân thức của nó và p là một phần tử bất khả quy của A. Với x ∈ K* hãy ký hiệu v_p(x) là số mũ của p trong phân tích của x thành các phần tử bất khả quy (Đại số, Chương VII, § 1, no. 3, Định lý 2); hiển nhiên thấy rằng v_p là một định giá mà nhóm giá trị là Z và vành của nó là A_{A_p}. Theo Mệnh đề 3 của § 1, no. 4 ta do đó thu được, tới tương đương, mọi định giá trên K không tầm thường và dương trên A. Lấy A = Z ta thu lại các định giá p-adic trên Q (Tôpô đại cương, Chương IX, § 3, no. 2); những định giá này, tới tương đương, là những định giá duy nhất trên Q không tầm thường (§ 1, no. 4, Hệ quả 1 của Mệnh đề 3). Lấy A = k[X], với k là một trường, các định giá không tầm thường trên k(X) mà các hạn chế lên k là tầm thường là (tới tương đương): một mặt là các định giá v_P, với P chạy qua tập các đa thức bất khả quy đơn nhất của k[X], và mặt khác là định giá v được xác định bởi

$$
v(P/Q) = \deg(Q) - \deg(P)
$$

cho P ∈ k[X] và Q ∈ k[X] (§ 1, no. 4, Hệ quả 2 của Mệnh đề 3); tất cả những định giá này hiển nhiên có Z làm nhóm giá trị và các trường thặng dư của chúng là các mở rộng đại số đơn sinh của k (Đại số, Chương V, § 3, no. 1).

Ví dụ (5) Ánh xạ P(X, Y) ↦ P(T, e^T) từ C[X, Y] vào C((T)) là đơn ánh (Hàm của một biến thực, Chương IV, §2, Mệnh đề 9) và do đó có thể được mở rộng thành một đẳng cấu từ C(X, Y) lên một trường con của C((T)). Hạn chế của định giá trên C((T)) được xác định trong Ví dụ 3 lên trường con này xác định một định giá trên C(X, Y) là tầm thường trên C, mà nhóm giá trị là Z và trường thặng dư của nó là C.

Mệnh đề 4 của no. 2 cho phép ta xây dựng một định giá mà nhóm giá trị và trường thặng dư của nó được cho trước:

Ví dụ (6) Cho $\Gamma$ là một nhóm được sắp thứ tự toàn phần và $k$ là một trường. Cho $\Gamma_+$ là monoid các phần tử dương của $\Gamma$ và $C$ là đại số của $\Gamma_+$ trên $k$. Theo định nghĩa, $C$ có một cơ sở $(x_\alpha)_{\alpha \in \Gamma_-}$ trên $k$ mà bảng phép nhân là $x_\alpha x_\beta = x_{\alpha + \beta}$. Nếu $x = \sum a_\alpha x_\alpha$ là một phần tử khác không của $C$, ta viết $v(x) = \inf_{a_\alpha \neq 0} (a)$ và $v(0) = +\infty$; dễ dàng kiểm tra rằng ánh xạ $v$ từ $C$ vào $\Gamma_\infty$ thỏa mãn các điều kiện (VL_I) và (VL_{II}) của no. 1 và rằng $C$ là một miền nguyên. Cho $K$ là trường phân thức của $C$ và $w$ là định giá trên $K$ kéo dài $v$ (Mệnh đề 4, no. 2). Vì mỗi phần tử của $\Gamma$ là hiệu của hai phần tử dương, nên $w$ nhận $\Gamma$ làm nhóm thứ tự. Cho $A$ là vành của $w$ và $m$ là iđêan cực đại của nó; ta sẽ chứng tỏ rằng $A$ là tổng trực tiếp của $m$ và $k$ (đồng nhất với $k \cdot 1$), điều này sẽ chứng minh rằng trường thặng dư của $w$ đẳng cấu với $k$. Rõ ràng $m \cap k = (0)$. Mặt khác, ký hiệu $p$ là iđêan của $C$ sinh bởi các $x_a$ với $a > 0$, thì mọi phần tử $x$ có giá trị 0 trong $K$ đều có thể viết dưới dạng $(a + y)/(b + z)$, trong đó $a \in k^*, b \in k^*, y \in p$ và $z \in p$; khi đó

$$
x = ab^{-1} + (by - az)b^{-1}(b + z)^{-1}
$$

suy ra $w(x - ab^{-1}) > 0$ và $x \equiv ab^{-1} \pmod{m}$; điều này chứng minh khẳng định của chúng ta.

Nếu $\Gamma = \mathbf{Z} \times \mathbf{Z}$, thì $K = k(X, Y)$ và phép dựng trên cung cấp các định giá trên $k(X, Y)$ không tầm thường trên $k$, có nhóm thứ tự là $\mathbf{Z} \times \mathbf{Z}$ và trường thặng dư là $k$. Các định giá này phụ thuộc vào cấu trúc thứ tự được chọn trên $\mathbf{Z} \times \mathbf{Z}$. Chẳng hạn, $\mathbf{Z} \times \mathbf{Z}$ có thể được cho thứ tự từ điển. Hoặc, với một số vô tỉ $a$, $\mathbf{Z} \times \mathbf{Z}$ có thể được đồng nhất với một nhóm con của $\mathbf{R}$ qua đồng cấu $(m, n) \mapsto m + n\alpha$ (một đồng cấu đơn ánh vì $a$ là vô tỉ) và được cho thứ tự cảm sinh bởi thứ tự đó trên $\mathbf{R}$.

Các phép dựng khác của các định giá dùng Mệnh đề 4 của no. 2 sẽ được trình bày ở § 10.

### 5. CÁC IĐÊAN CỦA MỘT VÀNH ĐỊNH GIÁ

#### Định nghĩa 2 {#ac-vi-s3-def-2 .statement}

*Cho G là một tập hợp có thứ tự. Một tập con của G được gọi là major nếu các quan hệ $x \in M$ và $y \geq x$ suy ra $y \in M$.*

Cho $K$ là một trường, $v$ là một định giá trên $K$, $A$ là vành của $v$ và $G$ là nhóm có thứ tự của $v$. Với mỗi tập con trội $M \subset G$, đặt $a(M)$ là tập các $x \in K$ sao cho $v(x) \in M \cup \{+\infty\}$. Rõ ràng $a(M)$ là một A-môđun con của $K$.

#### Mệnh đề 7 {#ac-vi-s3-prop-7 .statement}

*Ánh xạ $M \mapsto a(M)$ là một song ánh tăng từ tập các tập con trội của $G$ lên tập các A-môđun con của $K$.*

Cho $b$ là một A-môđun con của $K$. Tập các $v(x)$ với $x \in b - (0)$ là một tập con trội $M(b)$ của $G$. Mệnh đề 7 sẽ được chứng minh nếu các đẳng thức sau được chứng minh:

(2) $M(a(N)) = N$ với mọi tập con trội $N$ của $G$;
(3) $a(M(b)) = b$ với mọi A-môđun con $b$ của $K$.

Công thức (2) là dễ, vì với mọi $m \in N$, tồn tại $x \in K$ sao cho $v(x) = m$. Khi đó hiển nhiên $b \subset a(M(b))$; ngược lại, lấy $x \in a(M(b))$ và giả sử $x \neq 0$;

khi đó $v(x) \in M(b)$ và do đó tồn tại $y \in b$ sao cho $v(x) = v(y)$; suy ra $x = uy$ với $v(u) = 0$, điều này chứng minh rằng $x \in A$ $y \subset b$ và hoàn tất chứng minh.

#### Hệ quả {#ac-vi-s3-n5-cor-1 .statement}

Cho $G_+$ là tập các phần tử dương trong $G$. Ánh xạ $M \mapsto a(M)$ là một song ánh từ tập các tập con trội của $G_+$ lên tập các iđêan của $A$.

Vì $A = a(G_+)$, nên $a(M) \subset A$ tương đương với $M \subset G_+$.

Chẳng hạn iđêan cực đại $m(A)$ bằng $a(S)$, trong đó $S$ ký hiệu tập các phần tử dương ngặt của $G$.

### 6. CÁC ĐỊNH GIÁ RỜI RẠC

#### Định nghĩa 3 {#ac-vi-s3-def-3 .statement}

Cho $K$ là một trường (không nhất thiết giao hoán), $v$ là một định giá trên $K$ và $\Gamma$ là nhóm có thứ tự của $v$. $v$ được gọi là rời rạc nếu tồn tại một đẳng cấu (duy nhất tất yếu) của nhóm có thứ tự $\Gamma$ lên $\mathbf{Z}$. Cho $\gamma$ là phần tử của $\Gamma$ tương ứng với $1$ qua đẳng cấu này; mọi phần tử $u$ của $K$ sao cho $v(u) = \gamma$ được gọi là một phần tử đều hóa của $v$. Một định giá rời rạc được gọi là chuẩn nếu nhóm có thứ tự của nó là $\mathbf{Z}$.

Chẳng hạn định giá $v_p$ được xác định bởi một phần tử cực biên $p$ của một iđêan chính *hoặc miền nhân tử duy nhất, là một định giá rời rạc chuẩn và nhận $p$ làm một phần tử đều hóa. Đặc biệt, nếu $k$ là một trường, $k[[T]]$ là vành của một định giá rời rạc trên $k((T))$ và nhận $T$ làm một phần tử đều hóa. Cho $S$ là một đa tạp giải tích phức liên thông có chiều 1, $K$ là trường các hàm phân hình trên $S$ và $z_0$ là một điểm của $S$; tập hợp các $f \in K$ giải tích tại $z_0$ là vành của một định giá rời rạc $v$; để một hàm $f \in K$ là một phần tử đều hóa cho $v$, điều kiện cần và đủ là nó giải tích và bằng không tại $z_0$ và tồn tại một lân cận $V$ của $z_0$ trong $S$ sao cho hạn chế của $f$ lên $V$ là một đồng cấu của $V$ lên một lân cận của gốc trong $\mathbf{C}$. Chính ví dụ này và các ví dụ tương tự khác là nguồn gốc của từ "uniformizer".*

#### Mệnh đề 8 {#ac-vi-s3-prop-8 .statement}

Cho $K$ là một trường (không nhất thiết giao hoán), $v$ là một định giá rời rạc trên $K$, $A$ là vành của $v$ và $u$ là một phần tử đều hóa đối với $v$. Các iđêan khác không của $A$ là hai phía và có dạng $Au^n$ ($n \geq 0$).

Có thể giả sử rằng $v$ là chuẩn, sao cho $v(u) = 1$. Với mọi $x \in K^*$, tồn tại một số nguyên $n \in \mathbf{Z}$ sao cho $v(x) = n = v(u^n)$ và do đó ta có thể viết

$$
x = zu^n = u^n z',
$$

trong đó $z, z'$ là hai phần tử khả nghịch của vành $A$; từ đó suy ra mệnh đề.

#### Mệnh đề 9 {#ac-vi-s3-prop-9 .statement}

Cho $A$ là một miền nguyên địa phương khác với trường phân thức của nó. Các điều kiện sau là tương đương:
(a) $A$ là vành của một định giá rời rạc.
(b) $A$ là một miền iđêan chính.
(c) Iđêan $m(A)$ là chính và $\bigcap_{n=1}^{\infty} m(A)^n = (0)$.

(d) $A$ là một *vành Noether* và $m(A)$ là *chính*.
(e) $A$ là một *vành định giá Noether*.

Mệnh đề 8 cho thấy rằng (a) suy ra (b), (d) và (e). Nếu $A$ là một miền iđêan chính, thì $m(A) = Au$ và mọi iđêan khác không của $A$ đều có dạng $Au^n$ vì $A$ là địa phương (*Algebra*, chương VII, § 1, no. 3, Định lý 2); do đó $\bigcap_{n=1}^\infty m(A)^n = 0$; điều này cho thấy rằng (b) suy ra (c). Mặt khác (d) suy ra (c) (chương III, § 3, no. 2, Hệ quả của Mệnh đề 5); theo Mệnh đề 2 của § 1, no. 4, (c) suy ra (a). Vậy các điều kiện (a), (b), (c), (d) là tương đương và suy ra (e). Cuối cùng giả sử (e) đúng và ta hãy chứng minh rằng (b) đúng; chỉ cần chứng minh bổ đề sau:

#### Bổ đề 1 {#ac-vi-s3-lem-1 .statement}

*Cho $A$ là một vành định giá. Mọi $A$-môđun xoắn tự do sinh hữu hạn đều là tự do. Mọi iđêan sinh hữu hạn $\mathfrak{a}$ của $A$ đều là chính. Mọi $A$-môđun xoắn tự do đều phẳng.*

Cho $E$ là một $A$-môđun xoắn tự do sinh hữu hạn và cho $x_1, \ldots, x_n$ là các phần tử sinh của $E$ với số lượng tối thiểu; ta sẽ chứng minh rằng chúng độc lập tuyến tính. Nếu $\sum_{i=1}^n a_i x_i = 0$ ($a_i \in A$) là một quan hệ không tầm thường giữa các $x_i$, thì một trong các $a_i$, chẳng hạn $a_1$, chia hết tất cả các phần tử còn lại vì tập các iđêan chính của $A$ được sắp thứ tự toàn phần theo bao hàm (§ 1, no. 2, Định lý 1); khi đó $a_1 \neq 0$ vì quan hệ là không tầm thường. Vì $E$ là xoắn tự do, ta có thể chia cho $a_1$, tức là giả sử $a_1 = 1$. Nhưng khi đó $x_1$ là một tổ hợp tuyến tính của $x_2, \ldots, x_n$, trái với tính cực tiểu của $n$. Do đó $E$ là tự do.

Đặc biệt, mọi iđêan sinh hữu hạn $\mathfrak{a}$ của $A$ đều là chính, vì mọi phần tử của một hệ phần tử sinh của $\mathfrak{a}$ đều là bội của một trong các phần tử ấy. Mệnh đề 3 của chương I, § 2, no. 4 cho thấy mọi $A$-môđun xoắn tự do đều phẳng.

### Bài tập {#ac-vi-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
