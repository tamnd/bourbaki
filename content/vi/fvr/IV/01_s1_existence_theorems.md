---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 1
section_title: EXISTENCE THEOREMS
lang: vi
source: fvr-i-vii
pdf_pages: 0178-0192, 0214-0219
extraction: ocr
subsections:
    - "no": 1
      title: THE CONCEPT OF A DIFFERENTIAL EQUATION
      page: 0
      pdf_page: 178
    - "no": 2
      title: DIFFERENTIAL EQUATIONS ADMITTING SOLUTIONS THAT ARE PRIMITIVES OF REGULATED FUNCTIONS
      page: 0
      pdf_page: 179
    - "no": 3
      title: EXISTENCE OF APPROXIMATE SOLUTIONS
      page: 0
      pdf_page: 181
    - "no": 4
      title: COMPARISON OF APPROXIMATE SOLUTIONS
      page: 0
      pdf_page: 183
    - "no": 5
      title: EXISTENCE AND UNIQUENESS OF SOLUTIONS OF LIPSCHITZ AND LOCALLY LIPSCHITZ EQUATIONS
      page: 0
      pdf_page: 186
    - "no": 6
      title: CONTINUITY OF INTEGRALS AS FUNCTIONS OF A PARAMETER
      page: 0
      pdf_page: 189
    - "no": 7
      title: DEPENDENCE ON INITIAL CONDITIONS
      page: 0
      pdf_page: 191
statements: 29
exercises: 18
content_sha256: 50b479e1745705545f5e0aebcc292714bf1fc189c954aa24ebb9d1f2d28987a1
translated_from: content/en/fvr/IV/01_s1_existence_theorems.md
source_content_sha256: 2a0ebfd7467ee48420642d2462fb0e4209b34c54a99b6fdf811e56e594cacd20
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-9ae23bd9
glossary_version: 34
glossary_terms_sha256: fbe878df09c69445411adbbf2e8ba8f08ab13c32e45fa870e8746ac45d275224
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CÁC ĐỊNH LÝ TỒN TẠI

### 1. KHÁI NIỆM PHƯƠNG TRÌNH VI PHÂN

Cho I là một khoảng được chứa trong $\mathbf{R}$, không thu về một điểm duy nhất, E là một *không gian vectơ tôpô* trên $\mathbf{R}$, và A và B là hai tập con mở của E. Cho $(x, y, t) \mapsto g(x, y, t)$ là một ánh xạ liên tục từ $A \times B \times I$ vào E; với mỗi ánh xạ *khả vi* u từ I vào A có đạo hàm nhận giá trị trong B, ta gắn với u ánh xạ $t \mapsto g(u(t), u'(t), t)$ từ I vào E, và ký hiệu nó là $\tilde{g}(u)$; do đó $\tilde{g}$ được xác định trên tập hợp $\mathcal{D}(A, B)$ gồm các hàm khả vi từ I vào B mà các đạo hàm của chúng có giá trị trong B. Ta nói phương trình $\tilde{g}(u) = 0$ là một *phương trình vi phân* theo u (đối với biến *thực* t); một *nghiệm* của phương trình này cũng được gọi là một *nguyên* của phương trình vi phân (trên khoảng I); đó là một ánh xạ khả vi từ I vào A, có đạo hàm nhận giá trị trong B, sao cho $g(u(t), u'(t), t) = 0$ với *mọi* $t \in I$. Theo lối nói tắt, ta sẽ viết phương trình vi phân $\tilde{g}(u) = 0$ dưới dạng

$$
g(x, x', t) = 0,
$$

với quy ước rằng x thuộc tập hợp $\mathcal{D}(A, B)$.

Ví dụ, với $I = E = \mathbf{R}$, các quan hệ

$$
x' = 2t, \qquad tx' - 2x = 0, \qquad {x'}^2 - 4x = 0, \qquad x - t^2 = 0
$$

là các phương trình vi phân, cả bốn phương trình đều nhận hàm $x(t) = t^2$ làm nghiệm

Trong chương này, về nguyên tắc, ta chỉ xét trường hợp E là một *không gian định chuẩn đầy đủ* trên $\mathbf{R}$, và các phương trình vi phân có dạng đặc biệt

$$
x' = f(t, x)
$$

(“các phương trình tường minh theo $x'$”), trong đó f là một hàm xác định trên $I \times H$ nhận giá trị trong E, và H là một tập con *mở* khác rỗng của E. Hơn nữa, ta sẽ mở rộng một chút khái niệm *nghiệm* (hay *nguyên*) của một phương trình như vậy (trên khoảng I): ta nói rằng một hàm u, xác định và liên tục trên I, nhận giá trị trong H, là một nghiệm (hay nguyên) của phương trình (I) nếu tồn tại một tập con *đếm được* A của I sao cho tại mọi điểm t thuộc phần bù của A trong I, hàm u có đạo hàm $u'(t)$ thỏa mãn $u'(t) = f(t, u(t))$. Nếu $u$ khả vi và thỏa mãn quan hệ trên tại mọi điểm $t \in I$ thì ta nói rằng nó là một nghiệm ngặt của phương trình (1) trên I.

Trong trường hợp riêng của một phương trình vi phân có dạng $x' = f(t)$, trong đó $f$ là một ánh xạ từ I vào E, các nghiệm theo nghĩa trên là các nguyên của hàm $f$ (II, p. 51), và các nghiệm ngặt là các nguyên ngặt.

Khi E là một tích của các không gian định chuẩn đầy đủ $E_i$ ($1 \leq i \leq n$), ta có thể viết $x = (x_i)_{1 \leq i \leq n}$ và $f = (f_i)_{1 \leq i \leq n}$, trong đó $x_i$ là một ánh xạ từ I vào $E_i$ và $f_i$ là một ánh xạ từ $I \times H$ vào $E_i$; khi đó phương trình (1) tương đương với hệ các phương trình vi phân
$$
x'_i = f_i(t, x_1, x_2, \ldots, x_n) \qquad (1 \leq i \leq n).
$$
(2)

Trường hợp quan trọng nhất là khi các $E_i$ bằng $\mathbf{R}$ hoặc $\mathbf{C}$; khi đó ta nói rằng (2) là một hệ các phương trình vi phân vô hướng.

Có thể rút gọn việc nghiên cứu các quan hệ dạng
$$
x^{(n)} = f(t, x, x', \ldots, x^{(n-1)})
$$
về việc nghiên cứu hệ (2), trong đó $x$ là một hàm vectơ khả vi $n$ lần trên I; vì nếu đặt $x_1 = x$, và $x_p = x^{(p-1)}$ với $2 \leq p \leq n$, thì quan hệ (3) tương đương với hệ
$$
\begin{cases}
x'_i = x_{i+1} & (1 \leq i \leq n-1) \\
x'_n = f(t, x_1, x_2, \ldots, x_n).
\end{cases}
$$
(4)

Một quan hệ dạng (3) được gọi là một phương trình vi phân cấp $n$ (được giải tường minh theo $x^{(n)}$); trái lại, các phương trình dạng (1) được gọi là các phương trình vi phân cấp một.

Tương tự, có thể rút gọn mọi “hệ phương trình vi phân” dạng
$$
D^{n_i} x_i = f_i(t, x_1, Dx_1, \ldots, D^{n_1} x_1, \ldots, x_p, Dx_p, \ldots, D^{n_p-1} x_p)
$$
$(1 \leq i \leq p)$ về một hệ dạng (2), trong đó $x_i$ là hàm trên I khả vi $n_i$ lần trên I (với $1 \leq i \leq p$).

### 2. CÁC PHƯƠNG TRÌNH VI PHÂN NHẬN CÁC NGHIỆM LÀ NGUYÊN CỦA CÁC HÀM ĐƯỢC ĐIỀU CHỈNH

Nhắc lại (II, p. 54, def. 3) rằng một hàm vectơ $u$ xác định trên một khoảng $I \subset \mathbf{R}$ được gọi là được điều chỉnh nếu nó là giới hạn đều của các hàm bậc thang trên mọi tập con compact của I; một điều kiện tương đương là tại mọi điểm trong của I hàm $u$ có một giới hạn phải và một giới hạn trái, và đồng thời có một giới hạn phải tại đầu mút bên trái của I và một giới hạn trái tại đầu mút bên phải của I, khi hai điểm này thuộc I (II, p. 54, th. 3). Trong chương này ta sẽ giới hạn vào các phương trình vi phân (1) mà mọi nghiệm đều là một nguyên của một hàm được điều chỉnh trên I. Điều kiện này hiển nhiên được thỏa mãn nếu, với mọi ánh xạ liên tục $u$ từ I vào H, hàm $f(t, u(t))$ được điều chỉnh trên I; bổ đề sau đây cho một điều kiện đủ cho điều này:

#### Bổ đề 1 {#fvr-iv-s1-lem-1 .statement}

Cho $f$ là một ánh xạ từ $I \times H$ vào $E$ sao cho, khi viết $f_x$ (với mọi $x \in H$) là ánh xạ $t \mapsto f(t, x)$ của $I$ vào $E$, các điều kiện sau được thỏa mãn: 1° $f_x$ là điều hòa trên $I$ với mọi $x \in H$; 2° ánh xạ $x \mapsto f_x$ của $H$ vào tập hợp $\mathcal{F}(I, E)$ các ánh xạ từ $I$ vào $E$ là liên tục khi trang bị cho $\mathcal{F}(I, E)$ tôpô hội tụ đều trên các tập con compact (Gen. Top., X, p. 278). Dưới các điều kiện này:

1° Với mọi ánh xạ liên tục $u$ của $I$ vào $H$, hàm $t \mapsto f(t, u(t))$ là điều hòa trên $I$; chính xác hơn, giới hạn phải (tương ứng giới hạn trái) của hàm này tại một điểm $t_0 \in I$ bằng giới hạn phải (tương ứng giới hạn trái) của hàm $t \mapsto f(t, u(t_0))$ tại điểm $t_0$.

2° Nếu $(u_n)$ là một dãy các ánh xạ của $I$ vào $H$ hội tụ đều đến một hàm liên tục $u$ của $I$ vào $H$ trên mọi tập con compact của $I$, thì dãy các hàm $t \mapsto f(t, u_n(t))$ hội tụ đều đến $f(t, u(t))$ trên mọi tập con compact của $I$.

1 Gọi $c$ là giới hạn phải của $f(t, u(t_0))$ tại điểm $t_0$; với mọi $\varepsilon > 0$ tồn tại một lân cận compact $V$ của $t_0$ trong $I$ sao cho $\|f(t, u(t_0)) - c\| \leq \varepsilon$ với $t \in V$ và $t > t_0$. Mặt khác, tồn tại $\delta > 0$ sao cho các hệ thức

$$
x \in H, \quad \|x - u(t_0)\| \leq \delta
$$

suy ra $\|f(s, x) - f(s, u(t_0))\| \leq \varepsilon$ với mọi $s \in V$; nếu $W \subset V$ là một lân cận của $t_0$ trong $I$ sao cho $\|u(t) - u(t_0)\| \leq \delta$ với mọi $t \in W$, thì $\|f(t, u(t)) - c\| \leq 2\varepsilon$ với $t \in W$ và $t > t_0$, điều này chứng minh rằng $c$ là giới hạn phải của $f(t, u(t))$ tại điểm $t_0$.

2 Cho $K$ là một tập con compact của $I$; vì $u$ liên tục trên $I$, $u(K)$ là một tập con compact của $H$; với mọi $\varepsilon > 0$ và $x \in u(K)$ tồn tại một số $\delta_x$ sao cho, với mọi $y \in H, \|y - x\| \leq \delta_x$ và mọi $t \in K$, ta có $\|f(t, y) - f(t, x)\| \leq \varepsilon$. Có một số hữu hạn các điểm $x_i \in u(K)$ sao cho các quả cầu đóng có tâm $x_i$ và bán kính $\frac{1}{2}\delta_{x_i}$ tạo thành một phủ của $u(K)$; đặt $\delta = \operatorname{Min}(\delta_{x_i})$. Theo giả thiết tồn tại một số nguyên $n_0$ sao cho với $n \geq n_0$ ta có $\|u_n(t) - u(t)\| \leq \frac{1}{2}\delta$ với mọi $t \in K$. Bây giờ, với mọi $t \in K$ tồn tại một chỉ số $i$ sao cho

$$
\|u(t) - x_i\| \leq \frac{1}{2}\delta_{x_i};
$$

do đó ta có $\|u_n(t) - x_i\| \leq \delta_x$, suy ra $\|f(t, u_n(t)) - f(t, u(t))\| \leq 2\varepsilon$ với mọi $t \in K$ và mọi $n \geq n_0$

Trong phần này, tôi sẽ ký hiệu một khoảng chứa trong $\mathbf{R}$, không suy biến thành một điểm duy nhất, $H$ là một tập mở khác rỗng chứa trong không gian định chuẩn $E$, và $f$ là một ánh xạ từ $I \times H$ vào $E$ thỏa mãn các giả thiết của bổ đề 1.

#### Mệnh đề 1 {#fvr-iv-s1-prop-1 .statement}

Cho $t_0$ là một điểm của $I$ và $x_0$ là một điểm của $H$; để một hàm liên tục $u$ là một nghiệm của phương trình (1) trên $I$ và nhận giá trị $x_0$ tại điểm $t_0$, điều kiện cần và đủ là nó thỏa mãn quan hệ

$$
u(t) = x_0 + \int_{t_0}^t f(s, u(s))\, ds
$$

với mọi $t \in I$.

Thật vậy, theo bổ đề 1, nếu $u$ là một nghiệm của (1) trên $I$, thì $f(t, u(t))$ là điều hòa, do đó vế phải của (6) được xác định và bằng $u(t)$ với mọi $t \in I$. Ngược lại, nếu $u$ là một hàm liên tục thỏa mãn (6) thì $f(t, u(t))$ là điều hòa, theo bổ đề 1, do đó $u$ có đạo hàm bằng $f(t, u(t))$ ngoại trừ tại các điểm của một tập con đếm được của $I$.

#### Hệ quả {#fvr-iv-s1-n2-cor-1 .statement}

*Tại mọi điểm của I phân biệt với mút trái (tương ứng. mút phải) của khoảng này, mọi nghiệm u của (1) trên I đều có một đạo hàm trái (tương ứng. phải) bằng giới hạn trái (phải) của $f(t, u(t))$ tại điểm này.*

#### Mệnh đề 2 {#fvr-iv-s1-prop-2 .statement}

*Nếu f là một ánh xạ liên tục từ $I \times H$ vào E, thì mọi nghiệm của (1) trên I là một nghiệm ngặt.*

Thật vậy, một nghiệm như vậy $u$ là một nguyên thủy của hàm liên tục $f(t, u(t))$ (II, p. 66, mệnh đề 3).

Hơn nữa, ta chú ý rằng một hàm liên tục $f$ trên $I \times H$ thỏa mãn các điều kiện của bổ đề 1 (*Gen. Top.*, X, p. 286, hệ quả 3).

Trong phần tiếp theo, ta sẽ chọn tùy ý $t_0 \in I$ và $x_0 \in H$ và xét xem có tồn tại các nghiệm của (1) trên $I$ (hoặc trên một lân cận của $t_0$ trong $I$) nhận giá trị $x_0$ tại điểm $t_0$ hay không (hay, tương đương, các nghiệm của (6)).

### 3. TỒN TẠI CÁC NGHIỆM XẤP XỈ

Cho một số $\varepsilon > 0$, ta nói rằng một ánh xạ liên tục $u$ từ $I$ vào $H$ là một *nghiệm xấp xỉ với sai số không quá* $\varepsilon$ của phương trình vi phân

$$
x' = f(t, x)
$$

nếu, tại mọi điểm thuộc phần bù của một tập con *đếm được* của $I$, hàm $u$ có đạo hàm thỏa mãn điều kiện

$$
\|u'(t) - f(t, u(t))\| \leq \varepsilon.
$$

Cho $(t_0, x_0)$ là một điểm của $I \times H$; vì $f$ thỏa mãn các giả thiết của bổ đề 1 (IV, p. 165), tồn tại một lân cận compact $J$ của $t_0$ trong $I$ sao cho $f(t, x_0)$ bị chặn trên $J$, và một hình cầu mở $S$ có tâm $x_0$ được chứa trong $H$, sao cho $f(t, x) - f(t, x_0)$ bị chặn trên $J \times S$; suy ra $f(t, x)$ *bị chặn* trên $J \times S$. *Trong suốt tiểu mục này, J sẽ ký hiệu một khoảng compact là lân cận của t_0 trong I, S sẽ là một hình cầu mở có tâm x_0 và bán kính r được chứa trong H, với J và S sao cho f bị chặn trên J × S; và M sẽ ký hiệu cận trên của \|f(t, x)\| trên J × S.*

#### Mệnh đề 3 {#fvr-iv-s1-prop-3 .statement}

*Trên mọi khoảng compact có đầu mút trái (hoặc phải) là t_0 được chứa trong J, có độ dài nhỏ hơn r/(M + ε), tồn tại một nghiệm xấp xỉ với sai số không quá ε của phương trình (1), nhận các giá trị trong S và bằng x_0 tại t_0.*

Ta giả sử rằng $t_0$ không phải là đầu mút phải của J, và chứng minh mệnh đề đối với các khoảng có đầu mút trái $t_0$. Gọi $\mathcal{M}$ là tập hợp các nghiệm của (1) với sai số không quá $\varepsilon$, mỗi nghiệm nhận các giá trị trong S, bằng $x_0$ tại $t_0$ và được xác định trên một khoảng nửa mở $[t_0, b[$ được chứa trong J (khoảng này phụ thuộc vào nghiệm xấp xỉ đang xét). Trước hết ta chứng minh rằng $\mathcal{M}$ không rỗng. Gọi c là giới hạn phải của $f(t, x_0)$ tại $t_0$; theo bổ đề 1 (IV, p. 165), hàm $f(t, x_0 + c(t - t_0))$ có giới hạn phải bằng c tại $t_0$, do đó hạn chế của hàm $x_0 + c(t - t_0)$ trên một khoảng nửa mở đủ nhỏ $[t_0, b[$ sẽ thuộc $\mathcal{M}$.

Ta sắp thứ tự tập hợp $\mathcal{M}$ theo quan hệ “u là một hạn chế của v”, và chứng minh rằng $\mathcal{M}$ là quy nạp (Lý thuyết tập hợp, III, p. 154). Cho $(u_\alpha)$ là một tập con được sắp thứ tự toàn phần của $\mathcal{M}$ và $[t_0, b_\alpha[$ là khoảng mà $u_\alpha$ được xác định: nếu $b_\alpha \leq b_\beta$ thì hàm $u_\beta$ do đó là một mở rộng của $u_\alpha$. Hợp của các khoảng $[t_0, b_\alpha[$ là một khoảng $[t_0, b[$ được chứa trong J, và tồn tại duy nhất một hàm u xác định trên $[t_0, b[$ trùng với $u_\alpha$ trên $[t_0, b_\alpha[$ với mỗi $\alpha$; trong các $b_\alpha$ có một dãy tăng $(b_{\alpha_n})$ tiến tới b; vì u trùng với $u_{\alpha_n}$ trên $[t_0, b_{\alpha_n}[$ nên hàm u có một đạo hàm thỏa mãn (7) tại mọi điểm của phần bù của một tập con đếm được của $[t_0, b[$, và do đó là cận trên của tập $(u_\alpha)$ trong $\mathcal{M}$.

Theo bổ đề Zorn (Lý thuyết tập hợp, III, p. 154, th. 2), $\mathcal{M}$ có một phần tử cực đại $u_0$; ta sẽ chứng minh rằng nếu $[t_0, t_1[$ là khoảng mà $u_0$ được xác định, thì hoặc $t_1$ là đầu mút phải của J, hoặc $t_1 - t_0 \geq r/(M + \varepsilon)$. Ta lập luận phản chứng, giả sử không điều kiện nào trong hai điều kiện này đúng; trước hết ta chứng minh rằng có thể mở rộng $u_0$ bằng tính liên tục tại điểm $t_1$; thật vậy, với mọi s và t trong $[t_0, t_1[$,

$$
\|u_0(s) - u_0(t)\| \leq (M + \varepsilon)|s - t|
$$

theo định lý giá trị trung bình; tiêu chuẩn Cauchy cho thấy $u_0$ có giới hạn trái $x_1 \in S$ tại điểm $t_1$. Bây giờ cho $c_1$ là giới hạn phải tại $t_1$ của hàm $f(t, x_1)$; ta có $\|c_1\| \leq M$; lập luận giống như ở đầu chứng minh cho thấy có thể mở rộng $u_0$ đến một khoảng nửa mở có đầu mút trái là $t_1$ bằng hàm $x_1 + c_1(t - t_1)$, sao cho hàm mở rộng thuộc $\mathcal{M}$, điều này là vô lý. Điều này chứng minh mệnh đề.

Khi f liên tục đều trên $J \times S$, có thể chứng minh mệnh đề 3 mà không dùng bổ đề Zorn (IV, p. 199, bài tập 1a)).

#### Mệnh đề 4 {#fvr-iv-s1-prop-4 .statement}

*Tập hợp các nghiệm xấp xỉ của (1) trong phạm vi $\varepsilon$, được xác định trên cùng một khoảng $K \subset J$ và nhận giá trị trong S, là liên tục đều đồng bậc.*

Thật vậy, nếu u là một hàm bất kỳ trong tập hợp này và s và t là hai điểm của K, thì theo định lý giá trị trung bình

$$
\|u(s) - u(t)\| \leq (M + \varepsilon)|s - t|.
$$

#### Hệ quả (định lý Peano) {#fvr-iv-s1-n3-cor-1 .statement}

*Nếu E có số chiều hữu hạn trên $\mathbf{R}$ thì tồn tại một nghiệm của (1) nhận giá trị trong S và bằng $x_0$ tại $t_0$, trên mọi khoảng compact K có đầu mút trái (hoặc phải) $t_0$ được chứa trong J và có độ dài $< r/M$.*

Quả vậy, theo mệnh đề 3, một khi $n$ đủ lớn thì có một nghiệm xấp xỉ $u_n$ của (1) sai khác trong phạm vi $1/n$, được xác định trên $K$, có các giá trị trong $S$, và bằng $x_0$ tại $t_0$. Hơn nữa, từ một giá trị nào đó của $n$ trở đi, $u_n(K)$ được chứa trong một quả cầu *đóng* tâm $x_0$ và bán kính $< r$, độc lập với $n$. Tập hợp các $u_n$ là đồng liên tục (mệnh đề 4), và vì $E$ là hữu hạn chiều nên tập hợp $S$ là tương đối compact trong $E$; do đó với mọi $t \in K$ tập hợp các $u_n(t)$ là tương đối compact trong $E$. Theo định lý Ascoli (*Gen. Top.*, X, p. 290, th. 2), tập hợp các $u_n$ là tương đối compact trong không gian $\mathcal{F}(K; E)$ của các ánh xạ từ $K$ vào $E$ được trang bị chuẩn đều. Do đó có một dãy trích ra từ $(u_{n_k})$ của $(u_n)$ hội tụ đều trên $K$ tới một hàm liên tục $u$. Ta có $u(K) \subset S$, do đó $t \mapsto f(t, u(t))$ được xác định trên $K$; theo bổ đề 1 (IV, p. 165), $f(t, u_{n_k}(t))$ hội tụ đều tới $f(t, u(t))$ trên $K$; theo (IV, p. 4, công thức (7)), $u_{n_k}$ là một nguyên hàm của một hàm hội tụ đều tới $f(t, u(t))$ trên $K$, do đó (II, p. 52, th. 1) $u$ là một nghiệm của (1) trên $K$, và bằng $x_0$ tại điểm $t_0$.

#### Nhận xét 1 {#fvr-iv-s1-n3-rem-1 .statement}

Có thể có *vô hạn nhiều* tích phân của một phương trình vi phân (1) nhận cùng một giá trị tại một điểm đã cho. Ví dụ, phương trình vi phân vô hướng $x' = 2\sqrt{|x|}$ có tất cả các hàm được xác định bởi

$$
\begin{array}{ll}
u(t) = 0 & \text{cho } -\beta \leq t \leq \alpha \\
u(t) = -(t + \beta)^2 & \text{cho } t \leq -\beta \\
u(t) = (t - \alpha)^2 & \text{cho } t \geq \alpha
\end{array}
$$

là các tích phân nhận giá trị 0 tại điểm $t = 0$, với mọi số dương $\alpha$ và $\beta$.

#### Nhận xét 2 {#fvr-iv-s1-n3-rem-2 .statement}

Định lý Peano không còn đúng khi $E$ là một không gian chuẩn đầy đủ tùy ý có chiều *vô hạn* (IV, p. 204, exerc. 18).

### 4. SO SÁNH CÁC NGHIỆM XẤP XỈ

Trong phần sau, I và $H$ lần lượt ký hiệu, như trên, một khoảng được chứa trong $\mathbf{R}$ và một tập mở trong không gian chuẩn $E$; $t_0$ là một điểm của I.

#### Định nghĩa 1 {#fvr-iv-s1-def-1 .statement}

*Cho $t \mapsto k(t)$ là một hàm thực dương xác định trên $I$, người ta nói rằng một ánh xạ $f$ từ $I \times H$ vào $E$ là Lipschitz đối với hàm $k(t)$ nếu, với mọi $x \in H$, hàm $t \mapsto f(t, x)$ là hàm chỉnh trên $I$, và nếu, với mọi $t \in I$ và mọi cặp điểm $x_1, x_2$ của $H$, ta có (điều kiện "Lipschitz")*

$$
\| f(t, x_1) - f(t, x_2) \| \leq k(t) \| x_1 - x_2 \|.
$$

(8)

Ta sẽ nói rằng $f$ là *Lipschitz* (không nói cụ thể hơn) trên $I \times H$ nếu nó là Lipschitz trên tập hợp này đối với một *hằng* $k \geq 0$. Điều đó hiển nhiên là một hàm Lipschitz trên $I \times H$ thỏa mãn các giả thiết của bổ đề 1 của IV, p. 165 (đảo lại là sai); khi $f$ là Lipschitz (trên $I \times H$), ta nói rằng phương trình vi phân

$$
x' = f(t, x)
$$

(1)

là *Lipschitz* (trên $I \times H$).

#### Ví dụ {#fvr-iv-s1-n4-exa-1 .statement}

Khi $E = \mathbf{R}$ và $H$ là một khoảng trong $\mathbf{R}$, nếu hàm $f(t, x)$ thừa nhận một *đạo hàm riêng* $f'_x$ (II, p. 74) tại mọi điểm $(t, x)$ của $I \times H$, sao cho $|f'_x(t, x)| \leq k(t)$ trên $I \times H$, thì điều kiện (8) được thỏa mãn, theo định lý giá trị trung bình; về sau ta sẽ thấy ví dụ này khái quát hóa như thế nào sang trường hợp $E$ là một không gian chuẩn tùy ý.

Nếu $f$ là Lipschitz trên $I \times H$ thì $f$ là *bị chặn* trên $J \times S$ với mọi khoảng con compact $J \subset I$ và mọi quả cầu mở $S \subset H$. Do đó có thể áp dụng mệnh đề 3 (IV, p. 166), và nó chứng minh sự tồn tại của các nghiệm xấp xỉ của phương trình (1). Nhưng ta còn có mệnh đề sau, cho phép ta *so sánh* hai nghiệm xấp xỉ:

#### Mệnh đề 5 {#fvr-iv-s1-prop-5 .statement}

*Cho $k(t)$ là một hàm thực chỉnh và $> 0$ trên $I$, và cho $f(t, x)$ là một hàm được xác định và Lipschitz đối với $k(t)$ trên $I \times H$. Nếu $u$ và $v$ là hai nghiệm xấp xỉ của (1), với độ chính xác lần lượt là $\varepsilon_1$ và $\varepsilon_2$, được xác định trên $I$ với giá trị trong $H$, thì, với mọi $t \in I$ sao cho $t \geq t_0$,*

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\| \Phi(t) + (\varepsilon_1 + \varepsilon_2)\Psi(t)
$$

where

$$
\begin{cases}
\Phi(t) = 1 + \int_{t_0}^t k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds \\
\Psi(t) = t - t_0 + \int_{t_0}^t (s - t_0)k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds.
\end{cases}
$$

Từ quan hệ $\|u'(t) - f(t, u(t))\| \leq \varepsilon_1$, đúng trên phần bù của một tập đếm được, suy ra, từ định lý giá trị trung bình, rằng

$$
\left\| u(t) - u(t_0) - \int_{t_0}^t f(s, u(s))\, ds \right\| \leq \varepsilon_1 (t - t_0)
$$

và tương tự

$$
\left\| v(t) - v(t_0) - \int_{t_0}^t f(s, v(s))\, ds \right\| \leq \varepsilon_2 (t - t_0)
$$

do đó

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\|
$$
$$
+ \left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| + (\varepsilon_1 + \varepsilon_2)(t - t_0).
$$

Theo điều kiện Lipschitz (8) ta có

$$
\left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| \leq \int_{t_0}^t \|f(s, u(s)) - f(s, v(s))\|\, ds
$$
$$
\leq \int_{t_0}^t k(s) \|u(s) - v(s)\|\, ds
$$

do đó, đặt $w(t) = \|u(t) - v(t)\|$,

$$
w(t) \leq w(t_0) + (\varepsilon_1 + \varepsilon_2)(t - t_0) + \int_{t_0}^t k(s)w(s)\, ds.
$$

Mệnh đề này do đó là hệ quả của bổ đề sau:

#### Bổ đề 2 {#fvr-iv-s1-lem-2 .statement}

*Nếu w là một hàm thực liên tục trên khoảng [t_0, t_1] và thỏa mãn bất đẳng thức*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} k(s) w(s) \, ds
$$
(12)

*trong đó $\varphi$ là một hàm điều tiết $\geq 0$ trên $[t_0, t_1]$, thì, với $t_0 \leq t \leq t_1$,*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds.
$$
(13)

Đặt $y(t) = \int_{t_0}^t k(s) w(s) \, ds$; quan hệ (12) suy ra rằng

$$
y'(t) - k(t) y(t) \leq \varphi(t) k(t)
$$
(14)

trên phần bù của một tập đếm được.

Đặt $z(t) = y(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right)$; khi đó (14) tương đương với

$$
z'(t) \leq \varphi(t) k(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right).
$$

Áp dụng định lý giá trị trung bình (I, p. 15, đl. 2) cho bất đẳng thức này, và lưu ý rằng $z(t_0) = 0$, ta thu được

$$
z(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( - \int_{t_0}^s k(\tau) \, d\tau \right) \, ds
$$

do đó

$$
y(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds
$$

và vì $w(t) \leq \varphi(t) + y(t)$ nên suy ra (13).

#### Hệ quả {#fvr-iv-s1-n4-cor-1 .statement}

*Cho $\mathbf{f}$ là một hàm Lipschitz với hằng số $k > 0$, xác định trên $\mathbf{I} \times \mathbf{H}$. Nếu $\mathbf{u}$ và $\mathbf{v}$ là hai nghiệm gần đúng của (1) với sai số lần lượt là $\varepsilon_1$ và $\varepsilon_2$, xác định trên $\mathbf{I}$ và nhận giá trị trong $\mathbf{H}$, thì, với mọi $t \in \mathbf{I}$,*

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k |t - t_0|} + (\varepsilon_1 + \varepsilon_2) \frac{e^{k |t - t_0|} - 1}{k}.
$$
(15)

Bất đẳng thức này thực ra là một hệ quả trực tiếp của (9) khi $t \geq t_0$; để chứng minh nó cho $t \leq t_0$ chỉ cần áp dụng nó cho phương trình

$$
\frac{d \mathbf{x}}{ds} = -\mathbf{f}(-s, \mathbf{x})
$$

thu được từ (1) bằng phép đổi biến $t = -s$.

#### Nhận xét 1 {#fvr-iv-s1-n4-rem-1 .statement}

Khi $k = 0$ thì bất đẳng thức (15) được thay bằng bất đẳng thức
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| + (\varepsilon_1 + \varepsilon_2) |t - t_0|
$$
mà chứng minh của nó là hiển nhiên.

#### Nhận xét 2 {#fvr-iv-s1-n4-rem-2 .statement}

Khi E có số chiều hữu hạn, và $\mathbf{f}$ là Lipschitz trên $I \times H$, ta có thể chứng minh sự tồn tại của các nghiệm gần đúng của (1) (IV, p. 166, mệnh đề 3) mà không dùng tiên đề lựa chọn (IV, p. 199, bài tập 1 b)).

#### Mệnh đề 6 {#fvr-iv-s1-prop-6 .statement}

*Cho $\mathbf{f}$ và $\mathbf{g}$ là hai hàm xác định trên $I \times H$, thỏa mãn các giả thiết của bổ đề 1 của IV, p. 165, và sao cho, trên $I \times H$,
$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leq \alpha.
$$
(16)

Giả sử thêm rằng $\mathbf{g}$ là Lipschitz với hằng số $k > 0$ trên $I \times H$. Trong những điều kiện này, nếu $\mathbf{u}$ là một nghiệm gần đúng của $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ với sai số $\varepsilon_1$, xác định trên $I$, nhận giá trị trong $H$, và $\mathbf{v}$ là một nghiệm gần đúng của $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ với sai số $\varepsilon_2$, xác định trên $I$, nhận giá trị trong $H$, thì, với mọi $t \in I$
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\alpha + \varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$
(17)

Quả vậy
$$
\left\| \mathbf{u}'(t) - \mathbf{g}(t, \mathbf{u}(t)) \right\| \leq \alpha + \varepsilon_1
$$
với mọi $t$ thuộc phần bù trong $I$ của một tập con đếm được của $I$; nói cách khác, $\mathbf{u}$ là một nghiệm xấp xỉ của $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ trong phạm vi $\alpha + \varepsilon_1$, do đó bất đẳng thức (17) suy ra bằng cách áp dụng mệnh đề 5 của IV, p. 169.

### 5. SỰ TỒN TẠI VÀ TÍNH DUY NHẤT CỦA CÁC NGHIỆM CỦA CÁC PHƯƠNG TRÌNH LIPSCHITZ VÀ LIPSCHITZ ĐỊA PHƯƠNG

#### Định lý 1 (Cauchy) {#fvr-iv-s1-thm-1 .statement}

*Cho $\mathbf{f}$ là một hàm Lipschitz trên $I \times H$, cho J là một khoảng con compact của $I$, không rút gọn thành một điểm duy nhất, $t_0$ là một điểm của J, S là một quả cầu mở có tâm $\mathbf{x}_0$ và bán kính r, được chứa trong H, và M là cận trên nhỏ nhất của $\| \mathbf{f}(t, \mathbf{x}) \|$ trên $J \times S$. Trong các điều kiện này, với mọi khoảng compact K không rút gọn thành một điểm duy nhất và được chứa trong giao của J với $]t_0 - r/M, t_0 + r/M[$, và chứa $t_0$, tồn tại một và chỉ một nghiệm của phương trình vi phân $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ xác định trên K, có các giá trị trong S, và bằng $\mathbf{x}_0$ tại điểm $t_0$.

Quả vậy, với $\varepsilon > 0$ đủ nhỏ, tập hợp $F_\varepsilon$ các nghiệm xấp xỉ của (1) trong phạm vi $\varepsilon$, xác định trên K, có các giá trị trong S, và bằng $\mathbf{x}_0$ tại điểm $t_0$, không rỗng (IV, p. 166, mệnh đề 3); hơn nữa, nếu $\mathbf{u}$ và $\mathbf{v}$ thuộc $F_\varepsilon$ thì, theo (15) (IV. p. 170)
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq 2\varepsilon \frac{e^{k|t-t_0|} - 1}{k}
$$

với mọi $t \in K$, do đó các tập hợp $F_\varepsilon$ tạo thành một cơ sở lọc $\mathcal{G}$ hội tụ đều trên $K$ đến một hàm liên tục $w$, bằng $x_0$ tại $t_0$; đồng thời $w$ nhận các giá trị trong $S$, vì, với $\varepsilon$ đủ nhỏ, các hàm $u \in F_\varepsilon$ nhận các giá trị của chúng trong một quả cầu đóng được chứa trong $S$. Vì $f(t, u(t))$ hội tụ đều trên $K$ đến $f(t, w(t))$ dọc theo $\mathcal{G}$, $w$ thỏa mãn phương trình (6) của IV, p. 165, nên là một nghiệm của (1). Tính duy nhất của nghiệm suy ra ngay lập tức từ bất đẳng thức (15) của IV, p. 170, trong đó lấy $\varepsilon_1 = \varepsilon_2 = 0$ và $u(t_0) = v(t_0)$.

Ta sẽ nói rằng một hàm $f$ xác định trên $I \times H$ là Lipschitz địa phương nếu, với mọi điểm $(t, x)$ của $I \times H$, tồn tại một lân cận $V$ của $t$ (đối với $I$) và một lân cận $S$ của $x$ sao cho $f$ là Lipschitz trên $V \times S$ (với một hằng $k$ phụ thuộc vào $V$ và $S$). Theo định lý Borel-Lebesgue, với mọi khoảng compact $J \subset I$ và mọi điểm $x_0 \in H$ tồn tại một quả cầu mở $S$ có tâm $x_0$, được chứa trong $H$, sao cho $f$ là Lipschitz trên $J \times S$; do đó $f$ thỏa mãn các giả thiết của bổ đề 1 của IV, p. 3. Khi $f$ là Lipschitz địa phương trên $I \times H$ ta sẽ nói rằng phương trình $x' = f(t, x)$ là Lipschitz địa phương trên $I \times H$.

Ta sẽ tổng quát hóa và làm rõ định lý 1 của IV, p. 10 cho các phương trình Lipschitz địa phương; ta tự giới hạn vào trường hợp $t_0$ là đầu mút trái của khoảng $I$; ta có thể dễ dàng chuyển sang trường hợp $t_0$ là một điểm tùy ý của $I$ (cf. IV, §IV ??, p. 9, hệ quả).

#### Định lý 2 {#fvr-iv-s1-thm-2 .statement}

*Cho $I \subset \mathbf{R}$ là một khoảng (không suy giảm thành một điểm duy nhất) có đầu mút trái $t_0 \in I$, cho $H$ là một tập hợp mở khác rỗng trong $E$, và $f$ là một hàm Lipschitz địa phương trên $I \times H$.*

$1^\circ$ *Với $x_0 \in H$ tồn tại một khoảng lớn nhất $J \subset I$, có đầu mút trái $t_0 \in J$, trên đó tồn tại một nguyên hàm $u$ của phương trình $x' = f(t, x)$ nhận các giá trị trong $H$ và bằng $x_0$ tại điểm $t_0$; nguyên hàm này là duy nhất.*

$2^\circ$ *Nếu $J \neq I$ thì $J$ là một khoảng nửa mở $[t_0, \beta[$ có độ dài hữu hạn; hơn nữa, với mọi tập con compact $K \subset H$ tập $\overline{u}(K)$ là một tập con compact của $\mathbf{R}$.*

$3^\circ$ *Nếu $J$ bị chặn, và nếu $f(t, u(t))$ bị chặn trên $J$, thì $u(t)$ có giới hạn trái $c$ tại đầu mút phải của $J$; hơn nữa, nếu $J \neq I$ thì $c$ là một điểm biên của $H$ trong $E$.*

$1^\circ$ Cho $\mathfrak{M}$ là tập hợp các khoảng $L$ (không thu gọn thành một điểm duy nhất) có đầu mút trái $t_0 \in L$, được chứa trong $I$ và sao cho trên $L$ có một nghiệm của (1) (IV, p. 163) nhận các giá trị trong $H$ và bằng $x_0$ tại $t_0$; theo định lý 1 (IV, p. 171), tập hợp $\mathfrak{M}$ không rỗng. Cho $L$ và $L'$ là hai khoảng thuộc $\mathfrak{M}$, và giả sử, chẳng hạn, rằng $L \subset L'$; nếu $u$ và $v$ là hai nghiệm của (1) lần lượt xác định trên $L$ và $L'$, nhận các giá trị trong $H$ và bằng $x_0$ tại $t_0$, ta sẽ thấy rằng $v$ là một mở rộng của $u$. Thật vậy, gọi $t_1$ là supremum của tập hợp các $t \in L$ sao cho $u(s) = v(s)$ với $t_0 \leq s \leq t$; ta sẽ chứng minh rằng $t_1$ là đầu mút phải của $L$. Nếu không phải như vậy, do tính liên tục ta có $u(t_1) = v(t_1)$, và $x_1 = u(t_1)$ thuộc $H$; vì $f$ là Lipschitz địa phương, định lý 1 cho thấy chỉ có thể tồn tại duy nhất một nghiệm của (1) được xác định trên một lân cận của $t_1$, nhận các giá trị trong $H$ và bằng $x_1$ tại $t_1$; do đó giả sử rằng $t_1$ không phải là đầu mút phải của $L$ dẫn đến một mâu thuẫn. Ta thấy rằng nếu $J$ là hợp của các khoảng $L \in \mathfrak{M}$ thì tồn tại duy nhất một nghiệm $u$ của (1), xác định trên $J$, nhận các giá trị trong $H$ và bằng $x_0$ tại $t_0$.

2' Giả sử rằng J ≠ I và gọi β là đầu mút phải của J; nếu β là đầu mút phải của I thì β ∈ I (do đó β là hữu hạn) và J = [t_0, β[ theo giả thiết. Khi đó giả sử β không phải là đầu mút phải của I; nếu β ∈ J thì u(β) = c thuộc H; theo định lý 1, tồn tại một nghiệm của (1) nhận các giá trị trong H, được xác định trên một khoảng

$$ [\beta, \beta_1[ \subset I $$

và bằng c tại β; khi đó J không phải là khoảng lớn nhất trong các khoảng thuộc $\mathfrak{M}$, điều này là vô lý; do đó J = [t_0, β[.

Nếu K là một tập con compact của H thì $\bar{u}^{-1}(K)$ đóng trong J; ta sẽ thấy rằng tồn tại một γ ∈ J sao cho $\bar{u}^{-1}(K)$ được chứa trong [t_0, γ ], điều này sẽ chứng minh rằng $\bar{u}^{-1}(K)$ compact. Nếu không, sẽ tồn tại một điểm c ∈ K sao cho (β, c) là một điểm tụ của tập hợp các điểm (t, u(t)) sao cho t < β và u(t) ∈ K. Vì β ∈ I và c ∈ H nên tồn tại một lân cận V của β trong I, và một quả cầu mở S tâm c và bán kính r được chứa trong H, sao cho f Lipschitz và bị chặn trên V × S; gọi M là supremum của $\|f(t, x)\|$ trên tập hợp này. Theo giả thiết tồn tại một t_1 ∈ J sao cho $\beta - t_1 < r/2M$, $t_1 \in V$ và $\|u(t_1) - c\| \leq r/2$; định lý 1 chỉ ra rằng tồn tại duy nhất một nguyên của (1), nhận giá trị trong H, được xác định trên một khoảng [t_1, t_2] chứa β, và bằng u(t_1) tại t_1; vì khoảng này trùng với u trên khoảng [t_1, β[ nên suy ra rằng J = [t_0, β[ không phải là khoảng lớn nhất trong $\mathfrak{M}$, điều này là vô lý.

3 Giả sử rằng J bị chặn và $\|f(t, u(t))\| \leq M$ trên J; khi đó $\|u'(t)\| \leq M$ trên phần bù của một tập con đếm được của J; do đó, theo định lý giá trị trung bình, $\|u(s) - u(t)\| \leq M |s - t|$ với mọi s và t trong J; theo tiêu chuẩn Cauchy, u có một giới hạn trái c tại đầu mút phải β của J. Nếu J ≠ I thì c không thể thuộc H, vì bằng cách mở rộng u liên tục tại β, u sẽ là một nguyên của (1) nhận giá trị trong H, được xác định trên một khoảng [t_0, β] và bằng x_0 tại t_0; khi đó ta có J = [t_0, β], trái với điều đã thấy trong 2 .

#### Hệ quả 1 {#fvr-iv-s1-thm-2-cor-1 .statement}

*Nếu H = E và J ≠ I thì f(t, u(t)) không bị chặn trên J, và nếu thêm rằng E hữu hạn chiều, thì $\|u(t)\|$ có giới hạn trái $+\infty$ tại đầu mút phải của J.*

Phần thứ nhất là một hệ quả ngay lập tức của phần thứ ba của định lý 2. Nếu E hữu hạn chiều thì mọi quả cầu đóng S ⊂ E đều compact, do đó phần thứ hai của định lý 2 chỉ ra rằng tồn tại một γ ∈ J sao cho u(t) ∉ S với t > γ.

Nếu E hữu hạn chiều thì có thể xảy ra J ≠ I nhưng $\|u(t)\|$ vẫn *bị chặn* khi t tiến tới đầu mút phải của J (IV, p. 200, bài tập 5).

#### Hệ quả 2 {#fvr-iv-s1-thm-2-cor-2 .statement}

*Nếu, trên I × H, hàm f là Lipschitz đối với một hàm điều chỉnh k(t), và nếu đầu mút phải β của J thuộc I, thì u có một giới hạn trái tại β; nếu H = E và nếu f là Lipschitz đối với một hàm điều chỉnh k(t) trên I × E, thì J = I.*

Thật vậy, nếu β ∈ I, tồn tại một lân cận compact V của β trong I, sao cho f(t, x_0) và k(t) bị chặn trên V; khi đó $\|f(t, x)\| \leq m \|x\| + h$ (m và h hằng) trên $V \times H$, do đó $\|u'(t)\| \leq m \|u(t)\| + h$ trên phần bù của một tập con đếm được của $V \cap J$, nên $\|u(t)\| \leq m \int_{t_0}^t \|u(s)\|\ ds + q$ ($q$ hằng) trên $V \cap J$; bổ đề 2 (IV, p. 170) chỉ ra rằng $\|u(t)\| \leq c\ e^{mt} + d$ ($c$ và $d$ hằng) trên $V \cap J$, và do đó $f(t, u(t))$ vẫn *bị chặn* trên $J$, và hệ quả suy ra từ định lý 2 của IV, p. 172.

#### Ví dụ 1 {#fvr-iv-s1-n5-exa-1 .statement}

Đối với một phương trình vi phân có dạng $x' = g(t)$, trong đó $g$ là hàm điều chỉnh trên $I$, mọi nguyên $u$ đều được xác định rõ ràng trên toàn bộ $I$. Cần chú ý rằng $u$ có thể bị chặn trên $I$ mà $g(t)$ không bị chặn.

#### Ví dụ 2 {#fvr-iv-s1-n5-exa-2 .statement}

Đối với phương trình vô hướng $x' = \sqrt{1 - x^2}$ ta có $I = \mathbf{R},\ H = ] - 1, +1[$. Nếu lấy $t_0 = x_0 = 0$ thì nguyên tương ứng là $\sin t$ *trên khoảng lớn nhất chứa 0 mà đạo hàm của $\sin t$ là dương*, tức là trên $] - \pi/2, +\pi/2[$; tại các đầu mút của khoảng này, nguyên tiến tới một đầu mút của $H$.

#### Ví dụ 3 {#fvr-iv-s1-n5-exa-3 .statement}

Đối với phương trình vô hướng $x' = 1 + x^2$ ta có $I = H = \mathbf{R}$: nguyên triệt tiêu tại $t = 0$ là $\tan t$, và khoảng lớn nhất chứa 0 mà hàm này liên tục là $J = ] - \pi/2, +\pi/2[$; và $|\tan t|$ tiến tới $+\infty$ tại các đầu mút của $J$ (*xem* IV, p. 173, hệ quả 1).

#### Ví dụ 4 {#fvr-iv-s1-n5-exa-4 .statement}

Đối với phương trình vô hướng $x' = \sin tx$ ta có $I = H = \mathbf{R}$ và vế phải bị chặn trên $I \times H$, do đó (IV, p. 173, hệ quả 1) mọi nguyên đều được xác định trên toàn bộ $\mathbf{R}$.

### 6. TÍNH LIÊN TỤC CỦA CÁC NGUYÊN NHƯ CÁC HÀM CỦA MỘT THAM SỐ

Mệnh đề 6 (IV, p. 171) chỉ ra rằng khi một phương trình vi phân

$$
x' = f(t, x)
$$

"gần" một phương trình Lipschitz $x' = g(t, x)$ và khi giả sử rằng *cả hai* phương trình đều có một nghiệm gần đúng trên cùng một khoảng, thì các nghiệm gần đúng này "gần" nhau; ta sẽ làm rõ kết quả này bằng cách chứng minh rằng sự tồn tại các nghiệm của phương trình Lipschitz $x' = g(t, x)$ trên một khoảng *suy ra* sự tồn tại các nghiệm gần đúng của $x' = f(t, x)$ trên cùng khoảng đó, miễn là, trên khoảng sau, các giá trị của nghiệm của $x' = g(t, x)$ không "quá gần" với *biên* của $H$.

#### Mệnh đề 7 {#fvr-iv-s1-prop-7 .statement}

*Cho $f$ và $g$ là hai hàm xác định trên $I \times H$, thỏa mãn các giả thiết của bổ đề 1 của IV. p. 165, và sao cho, trên $I \times H$*

$$
\|f(t, x) - g(t, x)\| \leq \alpha .
$$
(16)

*Giả sử thêm rằng $g$ là Lipschitz theo hằng số $k > 0$ trên $I \times H$ và rằng $f$ là Lipschitz địa phương trên $I \times H$, hoặc rằng $E$ là hữu hạn chiều. Cho $(t_0, x_0)$ là một điểm của $I \times H$, $\mu$ là một số $> 0$, và*

$$
\varphi(t) = \mu\ e^{k(t-t_0)} + \alpha\ \frac{e^{k(t-t_0)} - 1}{k} .
$$

*Cho $u$ là một nghiệm của phương trình $x' = g(t, x)$ xác định trên một khoảng $K = [t_0, b[$ được chứa trong $I$, bằng $x_0$ tại điểm $t_0$, và sao cho với mọi $t \in K$ quả cầu đóng tâm $u(t)$ và bán kính $\varphi(t)$ được chứa trong $H$. Trong các điều kiện đó, với mọi $y \in H$ sao cho $\|y - x_0\| \leq \mu$ tồn tại một nghiệm $v$ của $x' = f(t, x)$, xác định trên $K$, nhận giá trị trong $H$, và bằng $y$ tại điểm $t_0$; hơn nữa, $\|u(t) - v(t)\| \leq \varphi(t)$ trên $K$. \*

Cho $\mathcal{M}$ là họ các nghiệm của $x' = f(t, x)$ mà mỗi nghiệm đều nhận giá trị trong $H$, bằng $y$ tại $t_0$, và được xác định trên một khoảng nửa mở $[t_0, \tau[$ được chứa trong $I$ (tùy theo khoảng đang xét). Theo Định lý 1 của IV, p. 171 (khi $f$ là Lipschitz địa phương) hoặc hệ quả của IV, p. 167 (khi $E$ là hữu hạn chiều), $\mathcal{M}$ không rỗng, và lập luận tương tự như ở Mệnh đề 3 của IV, p. 166 cho thấy rằng $\mathcal{M}$ là *quy nạp* đối với thứ tự "v là một hạn chế của w". Cho $v_0$ là một phần tử cực đại của $\mathcal{M}$ và $[t_0, t_1[$ là khoảng xác định của $v_0$; theo Mệnh đề 6 của IV, p. 171, toàn bộ quy về việc chứng minh rằng $t_1 \geq b$. Nếu không, ta sẽ có

$$
\| u(t) - v_0(t) \| \leq \varphi(t)
$$

trên khoảng $[t_0, t_1[$ theo mệnh đề 6; bây giờ trên khoảng compact $[t_0, t_1]$ hàm điều hòa $g(t, u(t))$ bị chặn, do đó hàm $g(t, v_0(t))$ bị chặn trên khoảng $[t_0, t_1[$, vì $\| g(t, v_0(t)) \| \leq \| g(t, u(t)) \| + k \varphi(t)$ trên khoảng này. Vì $v_0$ là một nghiệm xấp xỉ của $x' = g(t, x)$ trong phạm vi $\alpha$ trên $[t_0, t_1[$ nên tồn tại một số $M > 0$ sao cho $\| v_0'(t) \| \leq M$ trên khoảng này, trừ tại các điểm của một tập hợp đếm được; định lý giá trị trung bình cho thấy rằng $\| v_0(s) - v_0(t) \| \leq M |s - t|$ với mọi cặp điểm $s, t$ của $[t_0, t_1[$, do đó (theo tiêu chuẩn Cauchy) $v_0(t)$ có một giới hạn trái $c$ tại điểm $t_1$, và, theo tính liên tục, ta có $\| c - u(t_1) \| \leq \varphi(t_1)$, và vì vậy $c \in H$. Bây giờ ta thấy, từ IV, p. 171, đl. 1 hoặc IV, p. 167, hệ quả, rằng tồn tại một nguyên của $x' = f(t, x)$ được xác định trên một khoảng $[t_1, t_2[$ và bằng $c$ tại $t_1$, điều này mâu thuẫn với định nghĩa của $v_0$.

#### Định lý 3 {#fvr-iv-s1-thm-3 .statement}

*Cho F là một không gian tôpô và cho f là một ánh xạ từ I × H × F vào E sao cho, với mọi $\xi \in F$, hàm $(t, x) \mapsto f(t, x, \xi)$ là Lipschitz trên I × H, và sao cho, khi $\xi$ tiến tới $\xi_0$, $f(t, x, \xi)$ tiến đều tới $f(t, x, \xi_0)$ trên I × H. Cho $u_0(t)$ là một nguyên của $x' = f(t, x, \xi_0)$ được xác định trên một khoảng $J = [t_0, b[$ được chứa trong I, với các giá trị trong H, và bằng $x_0$ tại $t_0$. Với mọi khoảng compact $[t_0, t_1]$ được chứa trong J tồn tại một lân cận V của $\xi_0$ trong F sao cho, với mọi $\xi \in V$, phương trình $x' = f(t, x, \xi)$ có một nguyên (và chỉ một) $u(t, \xi)$ được xác định trên $[t_0, t_1]$, với các giá trị trong H và bằng $x_0$ tại $t_0$; hơn nữa, khi $\xi$ tiến tới $\xi_0$ nghiệm $u(t, \xi)$ tiến đều tới $u_0(t)$ trên $[t_0, t_1]$.*

Thật vậy, cho $r > 0$ sao cho với $t_0 \leq t \leq t_1$ thì quả cầu đóng tâm $u_0(t)$ và bán kính $r$ được chứa trong $H$; nếu $f(t, x, \xi)$ là Lipschitz theo hằng số $k > 0$ trên $I \times H$ ta lấy $\alpha$ đủ nhỏ để $\alpha \frac{e^{k(t_1-t_0)} - 1}{k} < r$; chọn $V$ sao cho, với mọi $\xi \in V$, ta có $\| f(t, x, \xi) - f(t, x, \xi_0) \| \leq \alpha$ trên $I \times H$, ta có thể áp dụng mệnh đề 7 của IV, p. 174; hơn nữa,

$$
\| u(t, \xi) - u_0(t) \| \leq \alpha \frac{e^{k(t_1-t_0)} - 1}{k}
$$

trên $[t_0, t_1]$, điều đó hoàn tất chứng minh định lý.

#### Nhận xét {#fvr-iv-s1-n6-rem-1 .statement}

Khi $H = E$ và điều kiện (16) của IV, p. 174 được thỏa trên $I \times E$, mệnh đề 7 của IV, p. 174 áp dụng cho *mọi* nghiệm $u$ của $x' = g(t, x)$ trên *bất kỳ* khoảng nào nơi nghiệm này được xác định; thậm chí có thể giả sử rằng $g(t, x)$ là Lipschitz theo một hàm điều hòa $k(t)$ mặc dù không nhất thiết bị chặn trên khoảng này.

### 7. PHỤ THUỘC VÀO CÁC ĐIỀU KIỆN BAN ĐẦU

Cho $x' = f(t, x)$ là một phương trình Lipschitz địa phương trên $I \times H$; theo đl. 2 (IV, p. 172), với mọi điểm $(t_0, x_0)$ của $I \times H$ tồn tại một *khoảng lớn nhất* $J(t_0, x_0) \subset I$, không thu về một điểm duy nhất, chứa $t_0$, và trên đó tồn tại một nguyên hàm (và chỉ một) của phương trình này, bằng $x_0$ tại $t_0$; ta sẽ làm rõ cách thức mà nguyên hàm này, và khoảng $J(t_0, x_0)$ nơi nó được xác định, phụ thuộc vào điểm $(t_0, x_0)$.

#### Định lý 4 {#fvr-iv-s1-thm-4 .statement}

*Cho $f$ là một hàm Lipschitz địa phương trên $I \times H$ và $(a, b)$ là một điểm tùy ý của $I \times H$.*

1 *Tồn tại một khoảng $K \subset I$, một lân cận của $a$ trong $I$, và một lân cận $V$ của $b$ trong $H$ sao cho, với mọi điểm $(t_0, x_0)$ của $K \times V$, tồn tại một nguyên hàm (và chỉ một) $u(t, t_0, x_0)$ được xác định trên $K$, nhận giá trị trong $H$ và bằng $x_0$ tại điểm $t_0$ (nói cách khác, $J(t_0, x_0) \supset K$ đối với mọi $(t_0, x_0) \in K \times V$).*

2 *Ánh xạ $(t, t_0, x_0) \mapsto u(t, t_0, x_0)$ từ $K \times K \times V$ vào $H$ là liên tục đều.*

3 *Có một lân cận $W \subset V$ của $b$ trong $H$ sao cho, với mọi điểm*
$$
(t, t_0, x_0) \in K \times K \times W,
$$
*phương trình $x_0 = u(t_0, t, x)$ có một nghiệm duy nhất $x$ trên $V$ bằng với $u(t, t_0, x_0)$* ("giải nghiệm theo hằng số tích phân").

1 Cho $S$ là một quả cầu tâm $b$ và bán kính $r$ được chứa trong $H$, và $J_0$ là một khoảng được chứa trong $I$, một lân cận của $a$ trong $I$, sao cho $f$ bị chặn và Lipschitz (với một hằng số $k$ nào đó) trên $J_0 \times S$; ký hiệu $M$ là cận trên đúng của $\|f(t, x)\|$ trên $J_0 \times S$. Khi đó tồn tại (IV, p. 171, định lý 1) một khoảng $J \subset J_0$, một lân cận của $a$ trong $I$, và một nghiệm $v$ của $x' = f(t, x)$ được xác định trên $J$, nhận giá trị trong $S$ và bằng $b$ tại $a$. Ta sẽ thấy rằng quả cầu mở $V$ tâm $b$ và bán kính $r/2$, cùng với giao $K$ của $J$ với một khoảng $]a - l, a + l[$, trong đó $l$ là *đủ nhỏ*, là như yêu cầu. Thật vậy, mệnh đề 7 của IV, p. 174 (áp dụng cho tập hợp $J_0 \times S$ và trường hợp $\alpha = 0$) cho thấy tồn tại một nghiệm của $x' = f(t, x)$ *được xác định trên* $K$, nhận giá trị trong $S$, và bằng $x_0$ tại một điểm $t_0 \in K$, miễn là
$$
\|v(t) - b\| + \|v(t_0) - x_0\| e^{k|t-t_0|} < r
$$
với mọi $t \in K$. Bây giờ, theo định lý giá trị trung bình, ta có
$$
\|v(t) - b\| \leq M |t - a| \leq Ml
$$
với mọi $t \in K$; vì $\|x_0 - b\| < r/2$ nên thấy rằng chỉ cần chọn $l$ sao cho
$$
Ml + (Ml + r/2)e^{2kl} < r
$$
hoặc quan hệ (18) được thỏa mãn với mọi $(t, t_0, x_0)$ thuộc $K \times K \times V$.

2' Theo định lý giá trị trung bình ta có

$$
\| \mathbf{u}(t_1, t_0, \mathbf{x}_0) - \mathbf{u}(t_2, t_0, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

(20)

với mọi $t_0, t_1, t_2$ trong K và $\mathbf{x}_0$ trong V. Bây giờ mệnh đề 5 (IV, p. 169) cho thấy rằng

$$
\| \mathbf{u}(t, t_0, \mathbf{x}_1) - \mathbf{u}(t, t_0, \mathbf{x}_2) \| \leq e^{2kt} \ \| \mathbf{x}_2 - \mathbf{x}_1 \|
$$

(21)

cho mọi $t$ và $t_0$ trong K, và $\mathbf{x}_1$ và $\mathbf{x}_2$ trong V. Cuối cùng, nếu $t_1$ và $t_2$ là bất kỳ hai điểm nào trong K,

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{u}(t_2, t_2, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

theo định lý giá trị trung bình, tức là

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t_2 - t_1| ;
$$

vì $\mathbf{u}(t, t_2, \mathbf{x}_0)$ đồng nhất với tích phân nhận giá trị $\mathbf{u}(t_1, t_2, \mathbf{x}_0)$ tại điểm $t_1$, Mệnh đề 5 (IV, p. 169) cho thấy rằng

$$
\| \mathbf{u}(t, t_1, \mathbf{x}_0) - \mathbf{u}(t, t_2, \mathbf{x}_0) \| \leq Me^{2kl} |t_2 - t_1|
$$

(22)

với mọi $t, t_1, t_2$ trong K và $\mathbf{x}_0$ trong V. Do đó ba bất đẳng thức (20), (21) và (22) chứng minh tính liên tục đều của ánh xạ $(t, t_0, \mathbf{x}_0) \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ trên $K \times K \times V$.

3 Theo (20), ta có $\| \mathbf{u}(t, t_0, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t - t_0| \leq 2Ml$ trên

$$
K \times K \times V.
$$

Nếu $l$ được lấy đủ nhỏ, sao cho $2Ml < r/4$, thì khi đó thấy rằng nếu $\mathbf{x}_0$ là bất kỳ điểm nào của quả cầu mở W tâm $\mathbf{b}$ và bán kính $r/4$, thì $\mathbf{u}(t, t_0, \mathbf{x}_0) \in V$ với mọi $t$ và $t_0$ trong K. Nếu $\mathbf{x} = \mathbf{u}(t, t_0, \mathbf{x}_0)$, thì hàm $s \mapsto \mathbf{u}(s, t, \mathbf{x})$ khi đó được xác định trên K và bằng tích phân của (1) nhận giá trị $\mathbf{x}$ tại điểm $t$, tức là bằng $\mathbf{u}(s, t_0, \mathbf{x}_0)$; đặc biệt

$$
\mathbf{x}_0 = \mathbf{u}(t_0, t_0, \mathbf{x}_0) = \mathbf{u}(t_0, t, \mathbf{x}).
$$

Hơn nữa, nếu $y \in V$ sao cho $\mathbf{x}_0 = \mathbf{u}(t_0, t, y)$, thì tích phân $s \mapsto \mathbf{u}(s, t, y)$ nhận giá trị $\mathbf{x}_0$ tại $t_0$ nên đồng nhất với $s \mapsto \mathbf{u}(s, t_0, \mathbf{x}_0)$, mà do đó nhận giá trị $\mathbf{x}$ tại $t$, điều này suy ra $y = \mathbf{x}$ và kết thúc chứng minh.

### Bài tập {#fvr-iv-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
