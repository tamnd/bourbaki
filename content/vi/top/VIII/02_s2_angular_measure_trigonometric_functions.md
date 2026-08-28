---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 2
section_title: Angular measure, trigonometric functions
lang: vi
source: top-v-x
pdf_pages: 0111-0121, 0131-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE MULTIPLICATIVE GROUP U
      page: 0
      pdf_page: 111
    - "no": 2
      title: ANGLES
      page: 0
      pdf_page: 113
    - "no": 3
      title: ANGULAR MEASURE
      page: 0
      pdf_page: 114
    - "no": 4
      title: TRIGONOMETRIC FUNCTIONS
      page: 0
      pdf_page: 115
    - "no": 5
      title: ANGULAR SECTORS
      page: 0
      pdf_page: 118
    - "no": 6
      title: CROSSES
      page: 0
      pdf_page: 119
statements: 5
exercises: 4
content_sha256: fec720590bc8aa7130bf7311b65e3e743eb6eb5ac1a52eca01770f673ccf5ac3
translated_from: content/en/top/VIII/02_s2_angular_measure_trigonometric_functions.md
source_content_sha256: a5d3b8b9967c53f54bbfeea4b7d7a20401592cd9d0f1108eb802855c2c0273b1
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-9b60b56b
glossary_version: 34
glossary_terms_sha256: a2a2b5b00f383077c60406dffa1e909e418745c9f32f10c6f5b8c9cc7d7f7470
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. ĐO GÓC, CÁC HÀM LƯỢNG GIÁC

### 1. NHÓM NHÂN U

#### Định lý 1 {#top-viii-s2-thm-1 .statement}

Nhóm (nhân, tôpô $U$ của các số phức có môđun bằng 1 đẳng cấu với nhóm (cộng, tôpô $T$ của các số thực môđun 1.

$U = S_1$ compact và liên thông, và có một lân cận của phần tử đơn vị -1 đồng phôi với một khoảng mở của $\mathbf{R}$ (Chương VI, § 2, no. 4, Mệnh đề 5); do đó định lý là một hệ quả của đặc trưng hóa tôpô của $T$ được cho trong Chương V, § 2, Định lý 2.

#### Hệ quả {#top-viii-s2-n1-cor-1 .statement}

Nhóm nhân $C^*$ của các số phức khác không đẳng cấu với nhóm $\mathbf{R} \times T$ (cf. § 1, no. 3, Mệnh đề 1).

#### Nhận xét {#top-viii-s2-n1-rem-1 .statement}

Sự đẳng cấu của các nhóm $C^*$ và $\mathbf{R} \times T$ kéo theo sự tồn tại các căn của mọi "phương trình nhị thức" $z^n = a$ trong trường $C$. Dùng sự kiện này và tính tương thích địa phương của $C$, ta có thể thu được một chứng minh khác của định lý d'Alembert-Gauss (Bài tập 2).

(1) $$ |e(x)| = 1, $$
(2) $$ e(x + y) = e(x)e(y), $$

cùng với các hệ thức

(3) $$ e(0) = 1,\quad e(\frac{1}{4}) = i,\quad e(\frac{1}{2}) = -1,\quad e(\frac{3}{4}) = -i,\quad e(1) = 1. $$

Từ (1) và (2) suy ra

(4) $$ e(-x) = \frac{1}{e(x)} = \overline{e(x)}, $$

và từ (2) và (3) suy ra

$$
e(x + \frac{1}{4}) = ie(x),\quad e(x + \frac{1}{2}) = -e(x),
$$
$$
e(x + \frac{3}{4}) = -ie(x),\quad e(x + 1) = e(x).
$$

Do đó hàm $e(x)$ là *tuần hoàn* và có 1 làm chu kỳ chính.

#### Nhận xét {#top-viii-s2-n1-rem-2 .statement}

Ánh xạ $x + iy \to e^{x}e(y)$ là một cấu xạ ngặt của nhóm cộng $\mathbf{C}$ lên nhóm nhân $\mathbf{C}^*$, và hạn chế của nó lên một lân cận thích hợp của 0 là một đẳng cấu địa phương của $\mathbf{C}$ với $\mathbf{C}^*$. Do đó (Chương VII, § 2, no. 3) mọi cấu xạ ngặt của $\mathbf{C}$ lên $\mathbf{C}^*$ đều có dạng $x + iy \to e^{\alpha x + \beta y}e(\gamma x + \delta y)$, trong đó $\alpha, \beta, \gamma, \delta$ là các số thực tùy ý sao cho $\alpha \delta - \beta \gamma \neq 0$. Về sau ta sẽ thấy rằng chỉ có một trong các đồng cấu này, ký hiệu bởi $z \to e^z$, sao cho

$$
\lim_{z \to 0} \frac{e^z - 1}{z} = 1;
$$

và hạn chế của đồng cấu này lên trục thực chính là $e^x$ (do đó có ký hiệu này).

### 2. GÓC

Vì trường $\mathbf{R}$ có thứ tự, ta có thể định hướng mặt phẳng số thực $\mathbf{R}^2$ bằng cách lấy $e_1 \wedge e_2$ làm bivectơ dương ($e_1, e_2$ là các vectơ của cơ sở chính tắc). Trong mặt phẳng số thực định hướng $\mathbf{R}^2$ (được đồng nhất với $\mathbf{C}$ trong phần sau), khi đó ta có thể định nghĩa góc $(\Delta_1, \Delta_2)$ của một cặp tùy ý các tia $(\Delta_1, \Delta_2)$ có gốc o (*). Tập hợp $\mathfrak{A}$ của tất cả các góc có cấu trúc của một nhóm Abel (viết theo phép cộng) được định nghĩa bởi

$$
(\Delta_1, \Delta_3) = (\Delta_1, \Delta_2) + (\Delta_2, \Delta_3),
$$

do đó, đặc biệt, $(\Delta_1, \Delta_1) = 0$ và $(\Delta_2, \Delta_1) = - (\Delta_1, \Delta_2)$.

Góc phẳng $\varpi$ là nghiệm $\neq 0$ của phương trình $2\theta = 0$ trong $\mathfrak{A}$; đó là góc mà nửa trục thực âm tạo với nửa trục thực dương.

Nếu $z$ là một số phức khác không tùy ý, biên độ (hay argument) của $z$, ký hiệu là $\mathrm{Am}(z)$, là góc mà tia đi qua $z$ có gốc o tạo với nửa trục thực dương. Ánh xạ $z \to \mathrm{Am}(z)$ là một đồng cấu của nhóm nhân $\mathbf{C}^*$ lên nhóm cộng $\mathfrak{A}$, và do đó ta có

$$
\mathrm{Am}(zz') = \mathrm{Am}(z) + \mathrm{Am}(z') \quad \text{và} \quad \mathrm{Am}(\overline{z}) = \mathrm{Am}(z^{-1}) = - \mathrm{Am}(z).
$$

Góc $\delta = \mathrm{Am}(i)$ được gọi là góc vuông dương; nó là một trong các nghiệm trong $\mathfrak{A}$ của phương trình $2\theta = \varpi$, nghiệm kia là $- \delta = \delta + \varpi$.

Đồng cấu $z \to \mathrm{Am}(z)$, hạn chế trên nhóm con $\mathbf{U}$ của $\mathbf{C}^*$, là một đẳng cấu của cấu trúc nhóm của $\mathbf{U}$ lên cấu trúc nhóm của $\mathfrak{A} \ (***)$; nếu ta

(*) Ta biết từ đại số rằng một quan hệ tương đương được xác định trên tập hợp tất cả các cặp $(\Delta_1, \Delta_2)$ của các tia có gốc o bằng cách coi hai cặp $(\Delta_1, \Delta_2)$ và $(\Delta'_1, \Delta'_2)$ là tương đương nếu tồn tại một phép quay biến đồng thời $\Delta_1$ thành $\Delta'_1$ và $\Delta_2$ thành $\Delta'_2$; góc của cặp $(\Delta_1, \Delta_2)$, hay góc mà $\Delta_2$ tạo với $\Delta_1$, khi đó theo định nghĩa là lớp tương đương của cặp $(\Delta_1, \Delta_2)$.

(**) Điều này là vì mọi tia có gốc o đều gặp đường tròn $S_1$, vì trường $\mathbf{R}$ là Pythagore.

dùng đẳng cấu này để chuyển tôpô của $\mathbf{U}$ sang nhóm $\mathfrak{A}$, nhóm sau trở thành một nhóm tôpô compact, và ánh xạ $z \to \mathrm{Am}\,(z)$ của $\mathbf{C}^*$ lên $\mathfrak{A}$ là một cấu xạ ngặt từ nhóm tôpô $\mathbf{C}^*$ lên nhóm tôpô $\mathfrak{A}$.

Ta ký hiệu bởi $\theta \to f(\theta)$ đẳng cấu của $\mathfrak{A}$ lên $\mathbf{U}$ là nghịch đảo của đẳng cấu $z \to \mathrm{Am}\,(z)$ của $\mathbf{U}$ lên $\mathfrak{A}$. Theo định nghĩa $\Re(f(\theta))$ được ký hiệu bởi $\cos \theta$ và được gọi là côsin của góc $\theta$; $\Im(f(\theta))$ được ký hiệu bởi $\sin \theta$ và được gọi là sin của góc $\theta$. Các hàm này liên tục trên nhóm tôpô $\mathfrak{A}$, và thỏa mãn các hệ thức sau (*loc. cit.*), là những hệ quả ngay lập tức của các định nghĩa ở trên:

$$
\begin{align*}
\cos 0 &= 1, & \sin 0 &= 0, & \cos \varpi &= -1, & \sin \varpi &= 0, \\
\cos(-\theta) &= \cos \theta, & \sin(-\theta) &= -\sin \theta, \\
\cos(\theta + \theta') &= \cos \theta \cos \theta' - \sin \theta \sin \theta', \\
\sin(\theta + \theta') &= \sin \theta \cos \theta' + \sin \theta' \cos \theta, \\
\cos^2 \theta + \sin^2 \theta &= 1.
\end{align*}
$$

Theo định nghĩa, tang của một góc $\theta \in \mathfrak{A}$ được định nghĩa, khi $\cos \theta \neq 0$, là $\sin \theta / \cos \theta$ (*loc. cit.*) và được ký hiệu bởi $\tan \theta$; đó là một hàm liên tục, mở rộng bởi tính liên tục đến $\tilde{\mathbf{R}}$ (Chương VI, § 3, no. 4) bằng cách lấy giá trị $\infty$ cho các góc $\delta$ và $-\delta$. Ta có $\tan (\theta + \varpi) = \tan \theta$. Cotang của $\theta$, ký hiệu bởi $\cot \theta$, là phần tử của $\tilde{\mathbf{R}}$ bằng $1 / \tan \theta$.

Chú ý rằng, nếu $\mathrm{Am}\,(z) = \theta$, ta có $z = |z| (\cos \theta + i \sin \theta)$; biểu thức này được gọi là dạng lượng giác của số phức $z \neq 0$.

### 3. ĐO GÓC

Theo Định lý 1 của no. 1, nhóm tôpô $\mathfrak{A}$ các góc là đẳng cấu với $\mathbf{T}$. Mọi cấu xạ ngặt từ $\mathbf{R}$ lên $\mathfrak{A}$ đều có thể thu được bằng cách hợp thành đẳng cấu $z \to \mathrm{Am}\,(z)$ từ $\mathbf{U}$ lên $\mathfrak{A}$ với một cấu xạ ngặt từ $\mathbf{R}$ lên $\mathbf{U}$; nếu đặt $\hat{x}(x) = \mathrm{Am}\,(e(x))$, thì mọi cấu xạ ngặt từ $\mathbf{R}$ lên $\mathfrak{A}$ do đó đều có dạng $x \to g(x/a)$ ($a \neq 0$). Cho một số thực $a > 0$, được cố định một lần cho tất cả, mỗi góc $\theta$ tương ứng, qua đồng cấu $x \to \hat{x}(x/a)$, với một lớp các số thực mod $a$ (nghĩa là một phần tử của $\mathbf{Z}/a\mathbf{Z}$) được gọi là số đo của $\theta$ đối với cơ sở $a$; do lạm dụng ngôn ngữ, mỗi số thực trong lớp này cũng được gọi là một số đo của $\theta$; góc $\hat{x}(x/a)$ được gọi là góc có số đo $x$ (đối với cơ sở $a$. Nếu $x$ là một số đo của $\theta$ và $x'$ là một số đo của $\theta'$ (đối với cùng một cơ sở) thì $x + x'$ là một số đo của $\theta + \theta'$, và $-x$ là một số đo của $\theta$. Số đo chính của một góc (đối với cơ sở $a$) là số đo của nó nằm trong khoảng $[0, a[$.

Lựa chọn một cơ sở $a$. Ta luôn luôn hạn chế vào các cơ sở $a > 1$. Với mỗi $a > 1$ tương ứng một góc $\omega = \frac{\pi}{a}$ có số đo chính là 1, và được gọi là đơn vị đo góc đối với cơ sở $a$; ngược lại, với mỗi góc $\omega \neq 0$ tương ứng một $a > 1$ duy nhất sao cho $\frac{\pi}{a} = \omega$, do đó việc biết đơn vị đo góc xác định hoàn toàn cơ sở $a > 1$.

Trong các tính toán số, người ta thường lấy hoặc $a = 360$ hoặc $a = 400$; đơn vị đo góc tương ứng được gọi là độ ($a = 360$) hoặc grad ($a = 400$).

Trong giải tích, và thực vậy trong mọi ngành toán học không liên quan đến tính toán số, cơ sở $a$ được xác định bởi điều kiện

$$
\lim_{x \to 0} \frac{e(x/a) - 1}{x} = i
$$

được sử dụng một cách phổ biến; cơ sở này được ký hiệu bởi $2\pi$. Đơn vị đo góc tương ứng được gọi là radian, và số đo được gọi là số đo radian; với định nghĩa của $e^z$ đối với $z$ phức đã được nêu trước đó, ta có $e(x) = e^{2\pi ix}$ với mọi $x \in \mathbf{R}$.

Một khi cơ sở $a$ đã được chọn, khi nói về một góc người ta thường có ý nói đến một số đo của góc này đối với cơ sở $a$; sự lạm dụng ngôn ngữ này không gây trở ngại nào với điều kiện (như luôn luôn xảy ra khi không có tính toán số) cơ sở $a$ được giữ cố định trong suốt quá trình, và với điều kiện người ta nhớ rằng hai số thực đồng dư mod $a$ tương ứng với cùng một góc.

Chẳng hạn, điều thường được hiểu bởi biên độ của một số phức $z \neq 0$ là số đo theo radian của góc này, được xác định bởi các quy ước sẽ phụ thuộc vào vấn đề đang xét; một khi các quy ước này đã được thiết lập, số đo của biên độ được chọn như vậy được ký hiệu là Am $(z)$.

### 4. CÁC HÀM LƯỢNG GIÁC

Nếu ta hợp thành các hàm $\cos \theta, \sin \theta, \tan \theta, \cot \theta$ (được xác định trên $\mathcal{A}$) với đồng cấu $x \to \frac{\pi}{a}(x/a)$ của $\mathbf{R}$ lên $\mathcal{A}$, các hàm

$$
\cos \left( \frac{x}{a} \right), \quad \sin \left( \frac{x}{a} \right), \quad \tan \left( \frac{x}{a} \right), \quad \cot \left( \frac{x}{a} \right)
$$

thu được như vậy lần lượt được gọi là côsin, sin, tang và côtang của *số* $x$ tương ứng với cơ sở $a$, và được viết là $\cos_a x$, $\sin_a x$, $\tan_a x$, $\cot_a x$. Ánh xạ $x \to \cos_a x + i \sin_a x$ là hợp thành của $\theta \to \cos \theta + i \sin \theta$ và $x \to \tilde{\sigma}(x/a)$, do đó, từ định nghĩa của $\cos \theta$ và $\sin \theta$ trong no. 2, ta có đồng nhất thức

$$
e\left( \frac{x}{a} \right) = \cos_a x + i \sin_a x,
$$

tương đương với

$$
\cos_a x = \Re \left( e\left( \frac{x}{a} \right) \right), \qquad \sin_a x = \Im \left( e\left( \frac{x}{a} \right) \right),
$$

và cũng theo (4), tương đương với

$$
\cos_a x = \frac{1}{2} \left( e\left( \frac{x}{a} \right) + e\left( -\frac{x}{a} \right) \right), \qquad \sin_a x = \frac{1}{2i} \left( e\left( \frac{x}{a} \right) - e\left( -\frac{x}{a} \right) \right).
$$

Suy ra các đồng nhất thức

$$
\cos_b x = \cos_a \left( \frac{ax}{b} \right), \qquad \sin_b x = \sin_a \left( \frac{ax}{b} \right).
$$

Các hàm lượng giác duy nhất xuất hiện trong những ngành toán học mà không liên quan đến tính toán số học là những hàm tương ứng với cơ sở $2\pi$ đã nói ở trên; các hàm này được ký hiệu đơn giản là $\cos x$, $\sin x$, $\tan x$, $\cot x$ thay cho $\cos_{2\pi} x$, $\sin_{2\pi} x$, $\tan_{2\pi} x$, $\cot_{2\pi} x$. Đối với mục đích tính toán số học, có các bảng của các hàm lượng giác tương ứng với các cơ sở $a = 360$ và $a = 400$; và các công thức (6) cho phép ta suy ra các giá trị của các hàm lượng giác tương ứng với mọi cơ sở khác.

Các quan hệ được nhắc lại trước đây giữa các côsin và sin của *góc* hiển nhiên dẫn đến cùng các quan hệ giữa các côsin và các sin của các *số* đo các góc này; đặc biệt, ta có

$$
\begin{align*}
\cos_a (x + y) &= \cos_a x \cos_a y - \sin_a x \sin_a y, \\
\sin_a (x + y) &= \sin_a x \cos_a y + \sin_a y \cos_a x, \\
\cos_a (-x) &= \cos_a x, \qquad \sin_a (-x) = -\sin_a x, \\
&\cos_a^2 x + \sin_a^2 x = 1.
\end{align*}
$$

Các hàm $\cos_a x$ và $\sin_a x$ liên tục trên $\mathbf{R}$, và tuần hoàn với chu kỳ $a$; hơn nữa, $a$ là một *chu kỳ chính* của các hàm này, vì quan hệ $\cos_a x = \cos_a y$ kéo theo hoặc là $\sin_a x = \sin_a y$ hoặc

$$
\sin_a x = -\sin_a y,\quad \text{tức là,}
$$

$$
e\left(\frac{x}{a}\right) = e\left(\frac{y}{a}\right)\quad \text{hoặc}\quad e\left(\frac{x}{a}\right) = e\left(-\frac{y}{a}\right),
$$

do đó hoặc là

$$
x \equiv y \pmod{a}\quad \text{hoặc}\quad x \equiv -y \pmod{a};
$$

và tương tự

$$
\sin_a x = \sin_a y
$$

tương đương với hoặc là $x \equiv y \pmod{a}$ hoặc $x + y \equiv \frac{1}{2} a \pmod{a}$.

Suy ra từ điều này rằng $\cos\_a x$ không bao giờ nhận cùng một giá trị hai lần trong khoảng $[0, \frac{1}{2} a]$; do đó, khi bị hạn chế trên khoảng này, nó là một ánh xạ \*song ánh\* của khoảng này lên khoảng $[-1, +1]$. Vì $\cos\_a 0 = 1$ và $\cos\_a (\frac{1}{2} a) = -1$, $x \to \cos\_a x$ là một ánh xạ \*giảm nghiêm ngặt\* của $[0, \frac{1}{2} a]$ lên $[-1, 1]$ (Chương IV, § 2, no. 6, Định lý 5 và Nhận xét). Ta có $\cos\_a x = 0$ với $x = a/4$, $\cos\_a x > 0$ với $0 \leq x < a/4$, $\cos\_a x < 0$ với $a/4 < x \leq a/2$. Vì $\cos\_a (-x) = \cos\_a x$ ta có thể suy ra sự biến thiên của $\cos\_a x$ trong khoảng $[- \frac{1}{2} a, 0]$, và do đó trên toàn bộ $\mathbf{R}$ nhờ tính tuần hoàn (Hình 8). Vì $\sin\_a x = -\cos\_a(x + a/4)$ ta cũng có thể suy ra sự biến thiên của $\sin\_a x$ trong $\mathbf{R}$ (Hình 8).

![Đồ thị biểu diễn y = sin\_a x và y = cos\_a x](https://i.imgur.com/3Q5z5QG.png)

Hình 8.

Hàm $\tan\_a x$ là một ánh xạ liên tục của $\mathbf{R}$ lên $\tilde{\mathbf{R}}$; nó nhận giá trị $\infty$ tại các giá trị $\frac{1}{4} a + \frac{1}{2} k a \ (k \in \mathbf{Z})$. Vì $\frac{1}{2} a$ là một chu kỳ của $\tan\_2 x$, nó là một \*chu kỳ chính\*. Trong khoảng $[0, \frac{1}{4} a]$, $\sin\_a x$ tăng từ 0 đến 1, $\cos\_a x$ giảm từ 1 đến 0, và do đó $\tan\_a x$ \*tăng ngặt\* trong $[0, \frac{1}{4} a[$ và ánh xạ khoảng này lên $[0, +\infty[$; suy ra rằng $\tan\_a x$ tăng ngặt trong khoảng

![Đồ thị biểu diễn các đường cong được ghi nhãn y và x, với các trục được đánh dấu -a/4, 0, a/4, a/2, 3a/4](../images/complex\_numbers\_9.png)

Hình 9.

]— $\frac{1}{4} a, + \frac{1}{4} a$[. và là một đồng phôi của khoảng này lên $\mathbf{R}$ (Hình 9).

### 5. CÁC MẶT QUẠT GÓC

Cho hai tia đóng phân biệt $\Delta_1, \Delta_2$ có gốc o, gọi $x$ là số đo chính của góc $(\widehat{\Delta_1, \Delta_2})$ (đối với một cơ sở $a$, được chọn một lần cho tất cả). Hợp của các tia đóng (tương ứng mở) $\Delta$ có gốc o sao cho số đo chính $y$ của góc $(\widehat{\Delta_1, \Delta})$ thỏa mãn $0 \leq y \leq x$ (tương ứng $0 < y < x$) là hình quạt góc đóng (tương ứng mở) S có gốc $\Delta_1$ và đầu mút $\Delta_2$, như đã định nghĩa trong đại số. Vì bằng một phép quay ta luôn có thể rút gọn về trường hợp S không chứa tia đi qua điểm — 1. Nếu $\alpha$ và $\beta$ lần lượt là các góc mà $\Delta_1$ và $\Delta_2$ tạo với nửa trục thực dương, thì hình quạt góc đóng S là hợp của các nửa đường thẳng đóng $\Delta$ tạo với nửa trục thực dương một góc $\theta$ sao cho $\tan \frac{1}{2} \alpha \leq \tan \frac{1}{2} \theta \leq \tan \frac{1}{2} \beta$. Bây giờ nếu $u, v, t$ lần lượt là các số đo của $\alpha, \beta, \theta$ nằm trong khoảng ]— $\frac{1}{2} a, + \frac{1}{2} a$[, thì các bất đẳng thức này tương đương với $\tan_a \frac{1}{2} u \leq \tan_a \frac{1}{2} t \leq \tan_a \frac{1}{2} v$; và vì $\tan_a x$ là một hàm tăng trong khoảng ]— $\frac{1}{4} a, + \frac{1}{4} a$[, chúng cũng tương đương với $u \leq t \leq v$, hay với $0 \leq t - u \leq v - u$; vì $x = v - u, y = t - u$, kết quả được chứng minh cho các hình quạt góc đóng, và chứng minh cho các hình quạt góc mở là tương tự.

Một hình quạt góc đóng là một tập hợp đóng trong $\mathbf{R}^2$, và hình quạt góc mở có cùng gốc và cùng đầu mút là phần trong của nó trong $\mathbf{R}^2$

Hình 10.

(Chương VI, § 2, no. 3, Mệnh đề 3). Góc $(\widehat{\Delta_1, \Delta_2})$, với số đo chính $x$, được gọi là góc của hình quạt S; S được gọi là nhọn nếu $x < \frac{1}{2} a$, phẳng (hoặc nửa mặt phẳng đóng) nếu $x = \frac{1}{2} a$; lõm nếu $x > \frac{1}{2} a$. Một hình quạt góc nhọn là nhọn nếu $x < \frac{1}{4} a$, vuông nếu $x = \frac{1}{4} a$, tù nếu $x > \frac{1}{4} a$. Phân giác của hình quạt S là tia $\Delta$ tạo với $\Delta_1$ một góc $y = \frac{1}{2} x$.

Hai tia đóng phân biệt $\Delta_1, \Delta_2$ xác định hai hình quạt góc đóng; hợp của chúng là mặt phẳng thực $\mathbf{R}^2$, và giao của chúng là $\Delta_1 \cup \Delta_2$.

### 6. CÁC CHÉO

Trong đại số, ta cũng đã định nghĩa chéo của một cặp đường thẳng trong một không gian vectơ hai chiều trên một trường có thứ tự cực đại (*). Định nghĩa này đặc biệt áp dụng cho mặt phẳng thực $\mathbf{R}^2$. Tập hợp $\mathcal{A}_0$ tất cả các chéo có cấu trúc của một nhóm Abel (được viết theo phép cộng) được xác định bởi

$$
(\overline{D_1, D_3}) = (\overline{D_1, D_2}) + (\overline{D_2, D_3})
$$

sao cho, đặc biệt, $(\overline{D_1, D_1}) = 0$ và $(\overline{D_2, D_1}) = - (\overline{D_1, D_2})$.

Chéo phải $\delta_0$ là nghiệm $\neq 0$ của phương trình $2\theta = 0$ trong $\mathcal{A}_0$; đó là chéo mà trục ảo tạo với trục thực.

(*) Ta nhắc lại rằng một quan hệ tương đương được xác định trên tập hợp tất cả các cặp không đẳng hướng của các đường thẳng $(D_1, D_2)$ bằng cách coi hai cặp đường thẳng $(D_1, D_2)$ và $(D'_1, D'_2)$ là tương đương nếu tồn tại một phép đồng dạng trực tiếp biến $D_1$ thành $D'_1$ và $D_2$ thành $D'_2$ đồng thời; chéo của cặp $(D_1, D_2)$ khi đó là lớp tương đương của cặp này.

Chúng ta định nghĩa một đồng cấu chính tắc $\varphi$ của nhóm $\mathfrak{A}$ các góc lên nhóm $\mathfrak{A}_0$ các chéo bằng cách cho tương ứng với góc mà một tia $\Delta$ tạo với nửa trục thực dương, chéo mà đường thẳng D chứa $\Delta$ tạo với trục thực. Một chéo $\theta_0$ là ảnh qua $\varphi$ của hai góc $\theta$ và $\theta + \omega$; do đó $\mathfrak{A}_0$ đẳng cấu với thương của $\mathfrak{A}$ theo nhóm con $\{0, \omega\}$. Nếu ta chuyển sang $\mathfrak{A}_0$ tôpô của nhóm thương $\mathfrak{A}/\{0, \omega\}$ bằng song ánh đồng cấu liên kết với $\varphi$, thì $\mathfrak{A}_0$ trở thành một nhóm tôpô compact và $\varphi$ là một cấu xạ ngặt của $\mathfrak{A}$ lên $\mathfrak{A}_0$.

Nếu ta lấy hợp thành của đồng cấu $\varphi$ của $\mathfrak{A}$ lên $\mathfrak{A}_0$ với đồng cấu $x \to \tilde{\sigma}(x/a)$ của $\mathbf{R}$ lên $\mathfrak{A}$, ta được một đồng cấu $x \to \tilde{\sigma}_0(x/a)$ của $\mathbf{R}$ lên $\mathfrak{A}_0$; mỗi chéo $\theta_0 \in \mathfrak{A}_0$ tương ứng, qua đồng cấu này, với một lớp các số thực mod $\frac{1}{2} a$, lớp này được gọi là số đo của chéo $\theta_0$ (đối với cơ sở $a$); do lạm dụng ngôn ngữ, mỗi số trong lớp này được gọi là một số đo của $\theta_0$, và số thuộc khoảng $[0, \frac{1}{2} a[$ được gọi là số đo chính của $\theta_0$; chéo $\tilde{\sigma}_0(x/a)$ là chéo có số đo $x$. Mọi số đo của $\theta_0$ cũng là số đo của một trong hai góc $\theta, \theta + \omega$ mà ảnh qua đồng cấu $\varphi$ là $\theta_0$.

Ở đây cũng vậy, một khi cơ sở $a$ đã được chọn, khi nói đến một chéo, nói chung ta muốn nói, do lạm dụng ngôn ngữ, đến một số đo của chéo này đối với cơ sở $a$.

#### Nhận xét {#top-viii-s2-n6-rem-1 .statement}

Ta có thể định nghĩa một đồng cấu của $\mathbf{C}^*$ lên $\mathfrak{A}_0$ bằng cách ánh xạ mỗi số phức $z \neq 0$ vào chéo mà đường thẳng đi qua o và $z$ tạo với trục thực. Rõ ràng đồng cấu này là hợp thành của $\varphi$ và đồng cấu $z \to \mathrm{Am}\,(z)$ của $\mathbf{C}^*$ lên $\mathfrak{A}$; do đó nó là một cấu xạ ngặt của nhóm tôpô $\mathbf{C}^*$ lên nhóm tôpô $\mathfrak{A}_0$, và đồng cấu song ánh liên kết là một đẳng cấu của nhóm thương $\mathbf{C}^*/\mathbf{R}^*$ lên $\mathfrak{A}_0$.

Ta biết rằng nếu D biểu thị một đường thẳng tạo một góc chéo $\theta_0$ với trục thực và nếu $(a, b)$ là một cặp tỉ số phương của D, thì tang của góc chéo $\theta_0$ (được ký hiệu bởi $\tan\,\theta_0$) là phần tử $b/a$ của $\tilde{\mathbf{R}}$ ($= \infty$ nếu $a = 0$), cũng được gọi là hệ số góc của đường thẳng D. Nếu $\theta$ và $\theta + \omega$ là hai góc mà ảnh của chúng qua $\varphi$ là $\theta_0$, thì ta có $\tan\,\theta_0 = \tan\,\theta = \tan(\theta + \omega)$.

Ánh xạ $\theta_0 \to \tan\,\theta_0$ là một phép đồng phôi của $\mathfrak{A}_0$ lên $\tilde{\mathbf{R}}$, vì không gian tôpô $\mathbf{C}^*/\mathbf{R}^*$ chính là đường thẳng xạ ảnh thực $\mathbf{P}_1$, và theo Chương VI, § 3, no. 3, ánh xạ một đường thẳng (được xem như một điểm của $\mathbf{P}_1$) vào hệ số góc của nó là một phép đồng phôi của $\mathbf{P}_1$ lên $\tilde{\mathbf{R}}$. Nếu bây giờ ta chuyển cấu trúc nhóm của $\mathfrak{A}_0$ sang $\tilde{\mathbf{R}}$ bằng ánh xạ $\theta_0 \to \tan\,\theta_0$, ta đã xác định trên $\tilde{\mathbf{R}}$ cấu trúc của một nhóm tôpô Abel, trong đó tích của hai phần tử $t_1, t_2$ là $\frac{t_1 + t_2}{1 - t_1 t_2}$ khi $t_1, t_2$ thuộc $\mathbf{R}$ và $t_1 t_2 \neq 1$; đối với các cặp $(t_1, t_2)$ không thỏa mãn các điều kiện này, tích của $t_1$ và $t_2$ thu được bằng cách mở rộng hàm $\frac{x + y}{1 - xy}$ bằng tính liên tục tới $\tilde{\mathbf{R}} \times \tilde{\mathbf{R}}$, và vẫn được ký hiệu bởi $\frac{t_1 + t_2}{1 - t_1 t_2}$.

### Bài tập {#top-viii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
