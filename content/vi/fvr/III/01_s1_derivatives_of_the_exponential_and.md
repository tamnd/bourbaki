---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 1
section_title: DERIVATIVES OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS
lang: vi
source: fvr-i-vii
pdf_pages: 0106-0119, 0130-0140
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF THE EXPONENTIAL FUNCTIONS; THE NUMBER $e$
      page: 0
      pdf_page: 106
    - "no": 2
      title: DERIVATIVE OF $\log_a x$
      page: 0
      pdf_page: 108
    - "no": 3
      title: DERIVATIVES OF THE CIRCULAR FUNCTIONS; THE NUMBER $\pi$
      page: 0
      pdf_page: 109
    - "no": 4
      title: INVERSE CIRCULAR FUNCTIONS
      page: 0
      pdf_page: 110
    - "no": 5
      title: THE COMPLEX EXPONENTIAL
      page: 0
      pdf_page: 112
    - "no": 6
      title: PROPERTIES OF THE FUNCTION $e^z$
      page: 0
      pdf_page: 113
    - "no": 7
      title: THE COMPLEX LOGARITHM
      page: 0
      pdf_page: 115
    - "no": 8
      title: PRIMITIVES OF RATIONAL FUNCTIONS
      page: 0
      pdf_page: 116
    - "no": 9
      title: COMPLEX CIRCULAR FUNCTIONS; HYPERBOLIC FUNCTIONS
      page: 0
      pdf_page: 117
statements: 9
exercises: 39
content_sha256: 2747be1a861a52b0a21d414d476a21cd0f1d3132c2202c75ac416d7ab555d463
translated_from: content/en/fvr/III/01_s1_derivatives_of_the_exponential_and.md
source_content_sha256: 2478d73e7dea6ae86c44de479cf637d4b4394218fc6dbee2396f8f6140182119
translation_model: gpt-5.4
translation_run: translate-vi-bf7718f9
glossary_version: 34
glossary_terms_sha256: 2c02ffec396f861a7ee582d7b770b5f73a48f098829f2e406393f8abbe55c2ba
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐẠO HÀM CỦA CÁC HÀM SỐ MŨ VÀ HÀM SỐ LƯỢNG GIÁC

### 1. ĐẠO HÀM CỦA CÁC HÀM SỐ MŨ; SỐ $e$

Ta biết rằng mọi đồng cấu liên tục của nhóm cộng $\mathbf{R}$ vào nhóm nhân $\mathbf{R}^*$ các số thực $\neq 0$ đều là một hàm dạng $x \mapsto a^x$ (gọi là một hàm số mũ), trong đó $a$ là một số $> 0$ (TG, V, p.11); đó là một đẳng cấu từ $\mathbf{R}$ lên nhóm nhân $\mathbf{R}_+^*$ các số $> 0$ nếu $a \neq 1$, và đẳng cấu nghịch đảo từ $\mathbf{R}_+^*$ lên $\mathbf{R}$ được ký hiệu bởi $\log_a x$ và được gọi là lôgarit cơ số $a$.

Ta sẽ thấy rằng hàm $f(x) = a^x$ có, với mọi $x \in \mathbf{R}$, một đạo hàm dạng $c.a^x$ (trong đó rõ ràng $c = f'(0)$). Điều này là hệ quả của định lý tổng quát sau:

#### Định lý 1 {#fvr-iii-s1-thm-1 .statement}

*Cho E là một đại số chuẩn đầy đủ trên trường $\mathbf{R}$, có một phần tử đơn vị $\mathbf{e}$, và cho $\mathbf{f}$ là một đồng cấu nhóm liên tục của nhóm cộng $\mathbf{R}$ vào nhóm nhân G các phần tử khả nghịch của E. Khi đó ánh xạ $\mathbf{f}$ khả vi tại mọi $x \in \mathbf{R}$, và*

$$
\mathbf{f}'(x) = \mathbf{f}(x)\mathbf{f}'(0).
$$

Trước hết chú ý rằng, vì E là một đại số đầy đủ, G là mở trong E (*Gen. Top.*, IX, p. 179, prop. 14). Xét hàm $g(x) = \int_0^a \mathbf{f}(x + t)\,dt$, trong đó $a > 0$ là một số mà ta sẽ chọn sau; vì $\mathbf{f}(x + t) = \mathbf{f}(x)\mathbf{f}(t)$ theo giả thiết, ta có $g(x) = \int_0^a \mathbf{f}(x)\mathbf{f}(t)\,dt = \mathbf{f}(x) \int_0^a \mathbf{f}(t)\,dt$ (I, p. 6, prop. 3). Cho $\alpha > 0$ sao cho quả cầu $\|x - \mathbf{e}\| \leq \alpha$ được chứa trong G; vì $\mathbf{f}(0) = \mathbf{e}$ và $\mathbf{f}$ liên tục theo giả thiết, có thể giả sử rằng $a$ đủ nhỏ để $\|\mathbf{f}(t) - \mathbf{e}\| \leq \alpha$ trên $[0, a]$; do đó (II, p. 61, formula (16)) ta có

$$
\left\| \frac{1}{a} \int_0^a \mathbf{f}(t)\,dt - \mathbf{e} \right\| \leq \alpha,
$$

và $\frac{1}{a} \int_0^a f(t) \, dt$ thuộc G; nói cách khác, khả nghịch; do đó $b = \int_0^a f(t) \, dt$ cũng khả nghịch và ta có thể viết $f(x) = g(x)b^{-1}$; vì thế chỉ cần chứng minh rằng g khả vi; mà, bằng phép thay đổi biến $x + t = u$ ta có $g(x) = \int_x^{x+a} f(u) \, du$; vì f liên tục, g khả vi với mọi $x \in \mathbf{R}$ (II, p. 56, prop. 3), và

$$
g'(x) = f(x+a) - f(x) = f(x)(f(a) - e).
$$

Suy ra $f'(x) = g'(x)b^{-1} = f(x)c$, trong đó $c = (f(a) - e)b^{-1}$, và rõ ràng $f'(0) = c$.

Ngược lại, có thể chứng minh, hoặc trực tiếp (III, p. 115, exerc. 1), hoặc bằng lý thuyết các phương trình vi phân tuyến tính (IV, p. 188), rằng mọi ánh xạ khả vi f từ $\mathbf{R}$ vào một đại số chuẩn đầy đủ E, sao cho $f'(x) = f(x)c$ và $f(0) = e$, đều là một đồng cấu của nhóm cộng $\mathbf{R}$ vào nhóm nhân G.

#### Mệnh đề 1 {#fvr-iii-s1-prop-1 .statement}

*Với mọi số $a > 0$ và $\neq 1$ hàm số mũ $a^\lambda$ có tại mọi điểm $x \in \mathbf{R}$ một đạo hàm bằng $(\log_e a)a^\lambda$ trong đó e là một số $> 1$ (độc lập với $a$).*

Áp dụng định lý 1 cho trường hợp E là chính trường $\mathbf{R}$, bây giờ cho thấy rằng $a^\lambda$ có một đạo hàm bằng $\varphi(a).a^\lambda$ tại mọi điểm, trong đó $\varphi(a)$ là một số thực $\neq 0$ chỉ phụ thuộc vào $a$. Cho $b$ là một số thứ hai $> 0$ và $\neq 1$; theo trên, hàm $b^\lambda$ có một đạo hàm bằng $\varphi(b).b^\lambda$; mặt khác, ta có $b^\lambda = a^\lambda \log_a b$ nên (I, p. 9, mệnh đề 5) đạo hàm của $b^\lambda$ bằng $\log_a b.\varphi(a)b^\lambda$; so sánh hai biểu thức này ta thu được

$$
\varphi(b) = \varphi(a).\log_a b.
$$ (2)

Suy ra có một số duy nhất $b$ sao cho $\varphi(b) = 1$; theo (2) quan hệ này tương đương với $b = a^{1/\varphi(a)}$. Theo quy ước, ký hiệu số thực thu được như vậy là e; từ (2) ta có $\varphi(a) = \log_e a$, điều này hoàn tất chứng minh mệnh đề 1.

Người ta thường viết $\exp x$ thay cho $e^x$.

Định nghĩa của số e cho thấy rằng

$$
D(e^\lambda) = e^\lambda
$$ (3)

điều này chứng minh rằng $e^\lambda$ là tăng ngặt, do đó $e > 1$.

Trong §2 (III, p. 105) ta sẽ thấy cách tính các giá trị gần đúng của e tùy ý sát.

#### Định nghĩa 1 {#fvr-iii-s1-def-1 .statement}

*Các lôgarit cơ sở e được gọi là lôgarit Naper (hoặc lôgarit tự nhiên).*

Ta thường bỏ cơ sở trong ký hiệu của lôgarit Naper. Trừ khi có nói ngược lại, ký hiệu $\log x$ ($x > 0$) sẽ chỉ *lôgarit Naper* của $x$. Với ký hiệu này, mệnh đề 1 có thể được viết thành đẳng thức

$$
D(a^\lambda) = (\log a)a^\lambda
$$ (4)

đúng với mọi $a > 0$ ($\log a = 0$ khi $a = 1$).

Hệ thức này cho thấy rằng $a^x$ có các đạo hàm thuộc *mọi cấp*, và rằng
$$
D^n(a^x) = (\log a)^n a^x.
$$
(5)

Đặc biệt, với $a > 0$ và $\neq 1$ ta có $D^2(a^x) > 0$ với mọi $x \in \mathbf{R}$, và do đó $a^x$ là *lồi ngặt* trên $\mathbf{R}$ (I, p. 31, hệ quả). Từ đó suy ra mệnh đề sau:

#### Mệnh đề 2 ("bất đẳng thức trung bình nhân") {#fvr-iii-s1-prop-2 .statement}

*Với mọi số* $z_i > 0$ ($1 \leq i \leq n$) *và các số* $p_i > 0$ *sao cho* $\sum_{i=1}^n p_i = 1$, *ta có*
$$
z_1^{p_1} z_2^{p_2} \cdots z_n^{p_n} \leq p_1 z_1 + p_2 z_2 + \cdots + p_n z_n.
$$
(6)
*Hơn nữa, hai vế của (6) chỉ bằng nhau nếu các* $z_i$ *bằng nhau.*

Đặt $z_i = e^{x_i}$; khi đó bất đẳng thức (6) có thể được viết
$$
\exp(p_1 x_1 + p_2 x_2 + \cdots + p_n x_n) \leq p_1 e^{x_1} + p_2 e^{x_2} + \cdots + p_n e^{x_n}.
$$
(7)
Vậy mệnh đề suy ra từ mệnh đề 1 ở I, p. 26 áp dụng cho hàm $e^x$, hàm này là lồi ngặt trên $\mathbf{R}$.

Người ta nói rằng vế trái (tương ứng, phải) của (6) là *trung bình nhân có trọng số* (tương ứng, *trung bình cộng có trọng số*) của $n$ số $z_i$ ứng với các *trọng số* $p_i$ ($1 \leq i \leq n$). Nếu $p_i = 1/n$ với $1 \leq i \leq n$, thì ta gọi các trung bình cộng và trung bình nhân tương ứng là các trung bình cộng và trung bình nhân *thông thường* của các $z_i$. Khi đó bất đẳng thức (6) có thể được viết
$$
(z_1 z_2 \cdots z_n)^{1/n} \leq \frac{1}{n}(z_1 + z_2 + \cdots + z_n).
$$
(8)

### 2. ĐẠO HÀM CỦA $\log_a x$

Vì $a^x$ là tăng nghiêm ngặt trên $\mathbf{R}$ với $a \neq 1$, áp dụng quy tắc đạo hàm của hàm nghịch đảo (I, p. 17, mệnh đề 6) ta được, với mọi $x > 0$
$$
D(\log_a x) = \frac{1}{x \log a}
$$
(9)
và đặc biệt
$$
D(\log x) = \frac{1}{x}.
$$
(10)

Nếu $u$ là một hàm thực có đạo hàm tại điểm $x_0$ và sao cho $u(x_0) > 0$, thì hàm $\log u$ có đạo hàm tại điểm $x_0$ bằng $u'(x_0)/u(x_0)$. Đặc biệt, ta có $D(\log |x|) = 1/|x| = 1/x$ nếu $x > 0$, và
$$
D(\log |x|) = -\frac{1}{|x|} = \frac{1}{x}
$$
nếu $x < 0$; nói cách khác, $D(\log |x|) = 1/x$ với mọi $x \neq 0$. Suy ra rằng nếu, trên một khoảng $I$, hàm thực $u$ khác không và có đạo hàm hữu hạn, thì $\log |u(x)|$ có đạo hàm bằng $u'/u$ trên $I$; đạo hàm này được gọi là *đạo hàm lôgarit* của $u$. Hiển nhiên đạo hàm lôgarit của $|u|^{\alpha}$ là $\alpha u'/u$, và đạo hàm lôgarit của một tích bằng tổng các đạo hàm lôgarit của các thừa số; các quy tắc này thường cho phương pháp nhanh nhất để tính đạo hàm của một hàm. Chúng lại cho, đặc biệt, công thức
$$
D(x^{\alpha}) = \alpha x^{\alpha-1} \qquad (\alpha \text{ là một số thực tùy ý, } x > 0)
$$
mà đã được chứng minh bằng một phương pháp khác (II, p. 69).

#### Ví dụ {#fvr-iii-s1-n2-exa-1 .statement}

Nếu $u$ là một hàm $\neq 0$ trên một khoảng $I$, và $v$ là một hàm thực tùy ý, thì $\log(|u|^v) = v \cdot \log |u|$, nên nếu $u$ và $v$ khả vi thì
$$
\frac{1}{|u|^v} D(|u|^v) = v' \log |u| + v \frac{u'}{u}.
$$

### 3. ĐẠO HÀM CỦA CÁC HÀM LƯỢNG GIÁC; SỐ $\pi$

Ta đã định nghĩa, trong Tôpô đại cương (*Gen. Top.*, VIII, p. 106), đồng cấu liên tục $x \mapsto \mathbf{e}(x)$ từ nhóm cộng $\mathbf{R}$ lên nhóm nhân $\mathbf{U}$ các số phức có giá trị tuyệt đối bằng 1; đó là một hàm tuần hoàn có chu kỳ chính bằng 1, và $\mathbf{e}\left(\frac{1}{4}\right) = i$. Ta biết (*loc. cit.*) rằng mọi đồng cấu liên tục từ $\mathbf{R}$ lên $\mathbf{U}$ đều có dạng $x \mapsto \mathbf{e}(x/a)$, và ta đặt $\cos_a x = \mathcal{R}(\mathbf{e}(x/a)), \sin_a x = \mathcal{I}(\mathbf{e}(x/a))$ (*các hàm lượng giác*, hay *các hàm tròn*, cơ sở $a$); các hàm sau cùng này là các ánh xạ liên tục từ $\mathbf{R}$ vào $[-1, +1]$ có chu kỳ chính bằng $a$. Ta có $\sin_a(x + a/4) = \cos_a x, \quad \cos_a(x + a/4) = -\sin_a x$, và hàm $\sin_a x$ tăng trên khoảng $[-a/4, a/4]$.

#### Mệnh đề 3 {#fvr-iii-s1-prop-3 .statement}

*Hàm* $\mathbf{e}(x)$ *có đạo hàm bằng* $2\pi i \mathbf{e}(x)$ *tại mọi điểm của* $\mathbf{R}$, *trong đó* $\pi$ *là một hằng số* $> 0$.

Bây giờ, đl. 1 của III, p. 51, áp dụng cho trường hợp trong đó E là trường $\mathbf{C}$ của các số phức, cho quan hệ $\mathbf{e}'(x) = \mathbf{e}'(0) \mathbf{e}(x)$; hơn nữa, vì $\mathbf{e}(x)$ có chuẩn Euclid hằng, $\mathbf{e}'(x)$ trực giao với $\mathbf{e}(x)$ (I, p. 7, *Ví dụ 3*); do đó ta có $\mathbf{e}'(0) = \alpha i$, với $\alpha$ thực. Vì $\sin_1 x$ tăng trên $[-\frac{1}{4}, \frac{1}{4}]$ nên đạo hàm của nó tại $x = 0$ là $\geqslant 0$, do đó $\alpha \geqslant 0$, và vì $e(x)$ không hằng, $\alpha > 0$; theo quy ước người ta ký hiệu số $\alpha$ nhận được như vậy bởi $2\pi$.

Trong §2 (III, p. 23) chúng tôi sẽ chỉ ra cách người ta có thể tính các xấp xỉ gần đúng tùy ý của số $\pi$.

Vì vậy ta có công thức

$$
D \left( e \left( \frac{x}{a} \right) \right) = \frac{2\pi i}{a} e \left( \frac{x}{a} \right).
$$

Ta thấy rằng công thức này được đơn giản hóa khi $a = 2\pi$; đó là lý do vì sao trong Giải tích người ta chỉ dùng các hàm tròn tương đối với cơ sở $2\pi$; ta thỏa thuận bỏ cơ sở trong ký hiệu của các hàm này; trừ khi nói rõ ngược lại, các ký hiệu $\cos x$, $\sin x$ và $\tan x$ lần lượt chỉ $\cos_{2\pi} x$, $\sin_{2\pi} x$ và $\tan_{2\pi} x$.

Với các quy ước ấy, và $a = 2\pi$, công thức (12) có thể được viết thành

$$
D(\cos x + i \sin x) = \cos \left( x + \frac{\pi}{2} \right) + i \sin \left( x + \frac{\pi}{2} \right),
$$

điều này tương đương với

$$
D(\cos x) = -\sin x, \qquad D(\sin x) = \cos x,
$$

từ đó suy ra

$$
D(\tan x) = 1 + \tan^2 x = \frac{1}{\cos^2 x}.
$$

Ngoài ba hàm tròn $\cos x$, $\sin x$ và $\tan x$ người ta còn dùng, trong tính toán số, ba hàm phụ trợ: côtang, secant và cosecant, được định nghĩa bởi các công thức

$$
\cot x = \frac{1}{\tan x}, \qquad \sec x = \frac{1}{\cos x}, \qquad \operatorname{cosec} x = \frac{1}{\sin x}.
$$

Nhắc lại (Top. Gen., VIII, p. 109) rằng góc tương ứng với cơ sở $2\pi$ được gọi là radian.

### 4. CÁC HÀM TRÒN NGHỊCH ĐẢO

Hạn chế của hàm $\sin x$ lên khoảng $[-\pi/2, +\pi/2]$ là tăng ngặt; người ta ký hiệu hàm nghịch đảo của nó là $\operatorname{Arc}\sin x$, do đó đây là một ánh xạ liên tục tăng ngặt của khoảng $[-1, +1]$ lên $[-\pi/2, +\pi/2]$ (hình 6). Công thức đạo hàm của các hàm nghịch đảo (I, p. 9, mệnh đề 6) cho đạo hàm của hàm này

$$
D(\operatorname{Arc}\sin x) = \frac{1}{\cos(\operatorname{Arc}\sin x)}.
$$

Vì $-\pi/2 \leq \operatorname{Arc}\sin x \leq \pi/2$ nên ta có $\cos(\operatorname{Arc}\sin x) \geq 0$, và vì

$$
\sin(\operatorname{Arc}\sin x) = x,
$$
ta có $\cos(\operatorname{Arc}\sin x) = \sqrt{1 - x^2}$, từ đó
$$
\mathrm{D}(\operatorname{Arc}\sin x) = \frac{1}{\sqrt{1 - x^2}}.
$$
Tương tự, hạn chế của $\cos x$ lên khoảng $[0, \pi]$ là giảm nghiêm ngặt; người ta ký hiệu hàm nghịch đảo của nó là $\operatorname{Arc}\cos x$, và đây là một ánh xạ giảm nghiêm ngặt của $[-1, +1]$ lên $[0, \pi]$ (hình 6). Hơn nữa

![Đồ thị biểu diễn y = Arc cos x và y = Arc sin x](https://i.imgur.com/3Q5z5QG.png)

Hình 6

$$
\sin \left( \frac{\pi}{2} - \operatorname{Arc}\cos x \right) = \cos(\operatorname{Arc}\cos x) = x
$$
và vì $-\pi/2 \leq \pi/2 - \operatorname{Arc}\cos x \leq \pi/2$, ta có
$$
\operatorname{Arc}\cos x = \frac{\pi}{2} - \operatorname{Arc}\sin x
$$
từ đó đặc biệt suy ra rằng
$$
\mathrm{D}(\operatorname{Arc}\cos x) = -\frac{1}{\sqrt{1 - x^2}}.
$$

Sau cùng, hạn chế của tan x lên khoảng ]−π/2, +π/2[ là tăng ngặt; người ta ký hiệu hàm nghịch đảo của nó là Arc tan x, và đây là một ánh xạ tăng ngặt từ \mathbf{R} lên ]−π/2, +π/2[ (hình 7); ta có

$$
\lim_{x \to -\infty} \operatorname{Arc tan} x = -\frac{\pi}{2}, \quad \lim_{x \to +\infty} \operatorname{Arc tan} x = \frac{\pi}{2},
$$

và, bằng cách áp dụng công thức đạo hàm của các hàm nghịch đảo và công thức (15) của III, p. 95, ta có

$$
\mathrm{D}\left( \operatorname{Arc tan} x \right) = \frac{1}{1 + x^2}.
$$

![Đồ thị biểu diễn y = Arc tan x](https://i.imgur.com/3Q5z5QG.png)

Hình 7

### 5. HÀM MŨ PHỨC

Chúng tôi đã xác định (Top. Gen., VIII, p. 106) tất cả các đồng cấu liên tục của nhóm tôpô (cộng tính) \mathbf{C} của các số phức lên nhóm tôpô (nhân tính) \mathbf{C}^* của các số phức khác 0; đó là các ánh xạ

$$
x + i y \mapsto e^{\alpha x + \beta y} \mathbf{e}(\gamma x + \delta y)
$$

trong đó $\alpha, \beta, \gamma, \delta$ là bốn số thực chịu điều kiện duy nhất $\alpha \delta - \beta \gamma \neq 0$. Bây giờ chúng ta đề nghị xác định những đồng cấu nào trong các đồng cấu $z \mapsto f(z)$ này là *khả vi* trên \mathbf{C}. Trước hết nhận xét rằng chỉ cần $f$ khả vi tại điểm $z = 0$; thật vậy, với mọi điểm $z \in \mathbf{C}$ ta có

$$
\frac{f(z + h) - f(z)}{h} = f(z) \frac{f(h) - 1}{h}
$$

nếu $f'(0)$ tồn tại thì $f'(z)$ cũng tồn tại, và $f'(z) = a f(z)$, với $a = f'(0)$. Mặt khác, nếu $g$ là một đồng cấu khả vi thứ hai, sao cho $g'(z) = b g(z)$, thì $g(a z / b) = f(z)$, vì ngay lập tức nhận thấy rằng thương $g(a z / b) / f(z)$ có đạo hàm bằng không ở mọi nơi và bằng 1 tại $z = 0$; do đó mọi đồng cấu khả vi đều có dạng $z \mapsto f(\lambda z)$, trong đó $f$ là một trong các đồng cấu ấy (giả sử chúng tồn tại) và $\lambda$ là một hằng (phức) bất kỳ.

Do đó, nếu $f$ khả vi tại điểm $z = 0$ thì mỗi ánh xạ $x \mapsto f(x),\ y \mapsto f(iy)$ từ $\mathbf{R}$ vào $\mathbf{C}$ tất yếu khả vi tại điểm $0$, ánh xạ thứ nhất có đạo hàm $f'(0)$, ánh xạ thứ hai có đạo hàm $if'(0)$. Bây giờ các đạo hàm tại điểm $0$ của các ánh xạ $x \mapsto e^{\alpha x} \mathbf{e}(\gamma x),\ y \mapsto e^{\beta y} \mathbf{e}(\delta y)$ lần lượt bằng $\alpha + 2\pi i \gamma$ và $\beta + 2\pi i \delta$, từ đó suy ra $\beta = -2\pi \gamma$ và $\alpha = 2\pi \delta$; riêng các điều kiện này được thỏa mãn bởi đồng cấu $x + iy \mapsto e^z \mathbf{e}(y/2\pi)$, mà tạm thời chúng ta sẽ ký hiệu là $f_0$. Bây giờ chúng ta sẽ chỉ ra rằng thực ra $f_0$ khả vi tại điểm $z = 0$.

Hiển nhiên là $x \mapsto f_0(x)$ và $y \mapsto f_0(iy)$ có các đạo hàm mọi cấp; đặc biệt, công thức Taylor cấp 1 áp dụng cho các hàm này cho thấy rằng với mọi $\varepsilon > 0$ tồn tại một $r > 0$ sao cho, nếu đặt

$$
f_0(x) = 1 + x + \varphi(x)x,\qquad f_0(iy) = 1 + iy + \psi(y)y,
$$

thì các điều kiện $|x| \leq r,\ |y| \leq r$ kéo theo $|\varphi(x)| \leq \varepsilon$ và $|\psi(y)| \leq \varepsilon$; như vậy, ta có $f_0(x + iy) = f_0(x)f_0(iy) = 1 + (x + iy) + \theta(x,\ y)$ với

$$
\theta(x,\ y) = (i + \varphi(x)\psi(y))xy + (1 + x)y\psi(y) + (1 + iy)x\varphi(x);
$$

với $|z| \leq r$ ta có $|x| \leq r$ và $|y| \leq r$, do đó

$$
|\theta(x,\ y)| \leq (1 + \varepsilon^2)|z|^2 + 2\varepsilon|z|(1 + |z|)
$$

điều này chứng tỏ rằng thương $\frac{f_0(z) - 1 - z}{z}$ tiến tới 0 cùng với $z$, nghĩa là hàm $f_0$ có đạo hàm bằng 1 tại điểm $z = 0$. Những điều trên do đó chứng minh rằng, với mọi $z \in \mathbf{C}$,

$$
D(f_0(z)) = f_0(z).
$$

Tính chất này thiết lập mối liên hệ giữa $f_0$ và hàm $e^z$, mà hơn nữa còn là hạn chế của $f_0$ lên trục thực; vì lý do đó chúng ta đưa ra định nghĩa sau:

**Định nghĩa 2** *Đồng cấu* $x + iy \mapsto e^z \mathbf{e}(y/2\pi)$ *từ* $\mathbf{C}$ *lên* $\mathbf{C}^*$ *được gọi là hàm mũ phức; giá trị của nó tại một số phức tùy ý* $z$ *được ký hiệu là* $e^z$ *hoặc* $\exp z$.

### 6. CÁC TÍNH CHẤT CỦA HÀM $e^z$

Việc $z \mapsto e^z$ là một đồng cấu của $\mathbf{C}$ lên $\mathbf{C}^*$ có thể được biểu thị bằng các đẳng thức

$$
e^{z+z'} = e^z e^{z'},\qquad e^0 = 1.\qquad e^{-z} = 1/e^z.
$$

Theo định nghĩa, với mọi $z = x + iy$, ta có

$$
e^{x+iy} = e^x (\cos y + i \sin y)
$$

và vì $e^{\lambda} > 0$ nên ta thấy $e^z$ có *môđun* là $e^{\lambda}$ và *biên độ* là $y$ (theo modulo $2\pi$).

Đặc biệt, định nghĩa 2 (III, p. 98) cho
$$
\mathbf{e}(x) = e^{2\pi i x}
$$
điều này cho phép ta viết các công thức định nghĩa $\cos x$ và $\sin x$ dưới dạng
$$
\cos x = \frac{1}{2} (e^{i x} + e^{-i x}), \qquad \sin x = \frac{1}{2i} (e^{i x} - e^{-i x})
$$
*(các công thức Euler)*.

Vì $2\pi$ là chu kỳ chính của $\mathbf{e}(y/2\pi)$, nên $2\pi i$ là *chu kỳ chính* của $e^z$; nói cách khác, nhóm các chu kỳ của $e^z$ là tập hợp các số $2n\pi i$, trong đó $n$ chạy qua $\mathbf{Z}$.

Cuối cùng, công thức (21) của III, p. 98 có thể được viết thành
$$
\mathrm{D}(e^z) = e^z
$$
do đó, với mọi số phức $a$
$$
\mathrm{D}(e^{a z}) = a\, e^{a z}.
$$

#### Nhận xét {#fvr-iii-s1-n6-rem-1 .statement}

Nếu, trong công thức (27), ta hạn chế hàm $e^{a z}$ ($a$ phức) vào trục thực, thì với $x$ thực ta lại thu được
$$
\mathrm{D}(e^{a x}) = a\, e^{a x}.
$$
Công thức này cho phép ta tính một nguyên hàm cho mỗi hàm số $e^{\alpha x} \cos \beta x$, $e^{\alpha x} \sin \beta x$ ($\alpha$ và $\beta$ thực); thật vậy, ta có $e^{(\alpha + i \beta)x} = e^{\alpha x} \cos \beta x + i e^{\alpha x} \sin \beta x$, nên, theo (28)
$$
\mathrm{D}\left( \mathcal{R}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \cos \beta x
$$
$$
\mathrm{D}\left( \mathcal{I}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \sin \beta x.
$$
Theo cùng cách ấy, ta quy việc tính một nguyên hàm của $x^n e^{\alpha x} \cos \beta x$, hoặc của $x^n e^{\alpha x} \sin \beta x$ (*n* *là một số nguyên* $> 0$) về việc tính một nguyên hàm của $x^n e^{(\alpha + i \beta)x}$; bây giờ, công thức lấy nguyên hàm từng phần bậc $n + 1$ (II, p. 60, công thức (11)) cho thấy một nguyên hàm của hàm sau cùng này là
$$
e^{(\alpha + i \beta)x} \left[ \frac{x^n}{\alpha + i \beta} - \frac{n x^{n-1}}{(\alpha + i \beta)^2} + \frac{n(n-1)x^{n-2}}{(\alpha + i \beta)^3} + \cdots + (-1)^n \frac{n!}{(\alpha + i \beta)^{n+1}} \right].
$$
Mặt khác, nhờ các công thức Euler, ta có thể biểu thị mọi lũy thừa nguyên dương của $\cos x$ hoặc của $\sin x$ như một tổ hợp tuyến tính của các hàm mũ $e^{ip x}$ ($p$ là một số nguyên dương hoặc âm). Bởi công thức (28), do đó ta có thể biểu thị một nguyên hàm của một hàm có dạng $x^n e^{\alpha x} (\cos \beta x)' (\sin \gamma x)^s$ như một tổ hợp tuyến tính của các hàm có dạng $x^p e^{\alpha x} \cos \lambda x$ và $x^p e^{\alpha x} \sin \mu x$ và ($n, p, r, s$ là các số nguyên, $\alpha, \beta, \gamma, \lambda, \mu$ thực).

#### Ví dụ {#fvr-iii-s1-n6-exa-1 .statement}

Ta có

$$
\sin^{2n} x = \frac{(-1)^n}{2^{2n}} \left( e^{i x} - e^{-i x} \right)^{2n} = \frac{(-1)^n}{2^{2n}} \left( e^{2n i x} - \binom{2n}{1} e^{(2n-2)i x} + \cdots + e^{-2n i x} \right)
$$

do đó

$$
\int_0^1 \sin^{2n} t \, dt = \frac{(-1)^n}{2^{2n}} \left( \frac{1}{n} \sin 2n x - \binom{2n}{1} \frac{1}{n-1} \sin(2n-2)x + \cdots \right.
$$
$$
\left. + (-1)^{n-1} \binom{2n}{n-1} \sin 2x + (-1)^n \binom{2n}{n} x \right)
$$

và đặc biệt

$$
\int_0^{\pi/2} \sin^{2n} t \, dt = \binom{2n}{n} \frac{1}{2^{2n}} \frac{\pi}{2} = \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{\pi}{2}.
$$ (29)

### 7. LOGARIT PHỨC

Gọi B là "dải" tạo bởi các điểm $z = x + i y$ sao cho $-\pi \leq y < \pi$; hàm $e^z$ nhận mỗi giá trị của nó trên B đúng một lần và chỉ một lần; nói cách khác, $z \mapsto e^z$ là một ánh xạ liên tục song ánh từ B lên $\mathbf{C}^*$; ảnh qua ánh xạ này của đoạn (nửa mở) $x = x_0,\ -\pi \leq y < \pi$ là đường tròn $|z| = e^{x_0}$; ảnh của đường thẳng $y = y_0$ là nửa đường thẳng (mở) xác định bởi $\mathrm{Am}(z) = y_0$ (mod. $2\pi$). Ảnh qua $z \mapsto e^z$ của phần trong $\dot{B}$ của B, nghĩa là của tập hợp các $z \in \mathbf{C}$ sao cho $|\mathcal{I}(z)| < \pi$, là phần bù F của nửa trục thực âm (đóng) trong $\mathbf{C}$; nếu quy ước ký hiệu $\mathrm{Am}(z)$ là số đo của biên độ của $z$ thuộc $[-\pi, \pi[$, thì tập hợp F có thể được xác định bởi các hệ thức $-\pi < \mathrm{Am}(z) < \pi$. Vì $z \mapsto e^z$ là một đồng cấu ngặt từ $\mathbf{C}$ lên $\mathbf{C}^*$ nên ảnh qua ánh xạ này của mọi tập con mở của B (do đó của $\mathbf{C}$) là một tập mở trong $\mathbf{C}^*$ (do đó trong F); nói cách khác, hạn chế của $z \mapsto e^z$ trên B là một đồng phôi từ $\dot{B}$ lên F. Ta ký hiệu bởi $z \mapsto \log z$ đồng phôi từ F lên B là nghịch đảo của ánh xạ sau; đối với một số phức $z \in F$, $\log z$ được gọi là giá trị chính của logarit của $z$. Nếu $z = x + i y$ và $\log z = u + i v$ thì $x + i y = e^{u+i v}$, do đó $e^u = |z|$, và vì $-\pi < v < \pi$, ta có $v = \mathrm{Am}(z)$. Hơn nữa, ta có $\tan(v + \pi/2) = -x/y$ nếu $y \neq 0$; vì thế ta có thể viết

$$
\begin{cases}
u = \log |z| = \frac{1}{2} \log(x^2 + y^2) \\
v = \frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{khi } y > 0 \\
v = 0 & \text{khi } y = 0 \\
v = -\frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{khi } y < 0.
\end{cases}
$$ (30)

Rõ ràng $\log z$ là mở rộng lên F của hàm $\log x$ xác định trên nửa trục thực dương mở $\mathbf{R}_+^*$. Nếu $z,\ z'$ là hai điểm của F sao cho $zz'$ không thực âm, ta có $\log(zz') = \log z + \log z' + 2\varepsilon \pi i$, trong đó $\varepsilon = +1,\ -1$ hoặc 0 tùy theo các giá trị của $\mathrm{Am}(z)$ và $\mathrm{Am}(z')$.

Ta chú ý rằng tại các điểm của nửa trục thực âm hàm $\log z$ không có giới hạn; chính xác hơn, nếu $x$ tiến tới $x_0 < 0$ và nếu $y$ tiến tới 0 mà vẫn > 0 (resp. < 0), thì $\log z$ tiến tới $\log |x_0| + \pi i$ (resp. $\log |x_0| - \pi i$); khi $z$ tiến tới 0, $|\log z|$ tăng vô hạn.

Sau này ta sẽ thấy lý thuyết các hàm giải tích cho phép ta mở rộng hàm $\log z$, và định nghĩa lôgarit phức trong đầy đủ tính tổng quát.

Vì $\log z$ là đồng phôi nghịch đảo của $e^z$, công thức tính vi phân của các hàm nghịch đảo (I, p. 9, mệnh đề 6) cho thấy rằng $\log z$ khả vi tại mọi điểm $z \in \mathbf{F}$, và rằng
$$
\mathrm{D}(\log z) = \frac{1}{e^{\log z}} = \frac{1}{z}
$$
một công thức tổng quát hóa công thức (10) của III, p. 93.

### 8. NGUYÊN THỦY CỦA CÁC HÀM HỮU TỈ

Công thức (31) cho phép ta tính nguyên thủy của một hàm hữu tỉ tùy ý $r(x)$ của biến thực $x$, với các hệ số thực hoặc phức. Ta biết (A.VII.7) rằng một hàm như vậy có thể được viết (theo một cách duy nhất) thành một tổng hữu hạn các hạng, là:

a) hoặc có dạng $ax^p$ ($p$ là một số nguyên $\geqslant 0$, $a$ là một số phức);
b) hoặc có dạng $a/(x-b)^m$ ($m$ là một số nguyên $\geqslant 0$, $a$ và $b$ là các số phức).

Bây giờ dễ dàng thu được một nguyên thủy của mỗi hạng này:
a) một nguyên thủy của $ax^p$ là $a \frac{x^{p+1}}{p+1}$;
b) nếu $m > 1$ thì một nguyên thủy của $a/(x-b)^m$ là $\frac{a}{(1-m)(x-b)^{m-1}}$;
c) sau cùng, từ các công thức (10) (III, p. 93) và (31) (III, p. 101), một nguyên thủy của $\frac{a}{x-b}$ là $a \log |x-b|$ nếu $b$ là thực, $a \log(x-b)$ nếu $b$ là phức. Trong trường hợp sau, nếu $b = p + iq$, ta còn có (III, p. 100, các công thức (30))
$$
\log(x-b) = \log \sqrt{(x-p)^2 + q^2} + i \operatorname{Arc tan} \frac{x-p}{q} \pm i \frac{\pi}{2}.
$$

Ta hoãn việc khảo sát các phương pháp thực hành hơn để xác định một cách tường minh một nguyên thủy của một hàm hữu tỉ được cho một cách tường minh sang phần của bộ sách này dành riêng cho Phép tính số.

Có thể rút gọn về việc tính một nguyên thủy của một hàm hữu tỉ:

1° việc tính một nguyên thủy của một hàm có dạng $r(e^{a x})$, trong đó $r$ là một hàm hữu tỉ và $a$ là một số thực; thật vậy, bằng phép thay đổi biến $u = e^{a x}$ ta rút gọn về việc tìm một nguyên thủy của $r(u)/u$;

2° việc tính một nguyên thủy của một hàm có dạng $f(\sin a x, \cos a x)$, trong đó $f$ là một hàm hữu tỉ của hai biến và $a$ là một số thực; phép thay đổi biến $u = \tan(a x/2)$ rút gọn việc này về tìm một nguyên thủy của

$$
\frac{2}{1 + u^2} \int \left( \frac{2u}{1 + u^2}, \frac{1 - u^2}{1 + u^2} \right).
$$

### 9. CÁC HÀM LƯỢNG GIÁC PHỨC; CÁC HÀM HYPERBOLIC

Các công thức của Euler (25) (III, p. 99) và định nghĩa của $e^z$ với mọi số phức $z$ cho phép ta mở rộng lên $\mathbf{C}$ các hàm $\cos x$ và $\sin x$ được định nghĩa trên $\mathbf{R}$, bằng cách đặt, với mọi $z \in \mathbf{C}$,

$$
\cos z = \frac{1}{2} (e^{i z} + e^{-i z}), \qquad \sin z = \frac{1}{2i} (e^{i z} - e^{-i z})
$$
(xem III, p. 119, bài tập 19).

Các hàm này là tuần hoàn với chu kỳ chính $2 \pi$; nghĩa là, ta có $\cos(z + \pi/2) = -\sin z, \sin(z + \pi/2) = \cos z$; ta cũng có thể kiểm tra các đồng nhất thức

$$
\cos^2 z + \sin^2 z = 1 \\
\cos(z + z') = \cos z \cos z' - \sin z \sin z' \\
\sin(z + z') = \sin z \cos z' + \cos z \sin z'.
$$

Tổng quát hơn, mọi đồng nhất thức đại số giữa các hàm lượng giác của các biến thực vẫn đúng khi ta gán cho các biến ấy các giá trị phức tùy ý (III, p. 119, bài tập 18).

Ta đặt $\tan z = \sin z / \cos z$ nếu $z \neq (2k + 1)\pi/2$ và $\cot z = \cos z / \sin z$ nếu $z \neq k \pi$; đó là các hàm tuần hoàn với chu kỳ chính $\pi$.

Công thức (27) (III, p. 99) cho thấy rằng $\cos z$ và $\sin z$ khả vi trên $\mathbf{C}$, và rằng

$$
\mathrm{D}(\cos z) = -\sin z, \qquad \mathrm{D}(\sin z) = \cos z.
$$

Đối với $z = i x$ ($x$ thực), các công thức (32) cho

$$
\cos i x = \frac{1}{2} (e^i + e^{-i}), \qquad \sin i x = \frac{i}{2} (e^i - e^{-i}).
$$

Thật tiện khi có một ký hiệu riêng cho các hàm thực được đưa vào như vậy; ta đặt

$$
\begin{cases}
\cosh x = \frac{1}{2} (e^x + e^{-x}) & \text{(cosin hyperbol của } x \text{)} \\
\sinh x = \frac{1}{2} (e^x - e^{-x}) & \text{(sin hyperbol của } x \text{)} \\
\tanh x = \frac{\sinh x}{\cosh x} = \frac{e^x - e^{-x}}{e^x + e^{-x}} & \text{(tang hyperbol của } x \text{)}
\end{cases}
$$

Do đó ta có, với mọi $x$ thực,

$$
\cos i x = \cosh x, \quad \sin i x = i \sinh x.
$$

Từ mọi đồng nhất thức giữa các hàm lượng giác trong một số nhất định các số phức $z_k$ ($1 \leq k \leq n$), người ta có thể suy ra một đồng nhất thức cho các hàm hyperbol, bằng cách thay thế $z_k$ bởi $i x_k$ ($x_k$ thực, $1 \leq k \leq n$) và dùng các công thức (34); chẳng hạn ta có

$$
\cosh^2 x - \sinh^2 x = 1
$$
$$
\cosh(x + x') = \cosh x \cosh x' + \sinh x \sinh x'
$$
$$
\sinh(x + x') = \sinh x \cosh x' - \cosh x \sinh x'.
$$

Các hàm hyperbol cho phép biểu thị các phần thực và ảo của $\cos z$ và $\sin z$ đối với $z = x + i y$, vì

$$
\cos(x + i y) = \cos x \cos i y - \sin x \sin i y = \cos x \cosh y - i \sin x \sinh y
$$
$$
\sin(x + i y) = \sin x \cos i y + \cos x \sin i y = \sin x \cosh y + i \cos x \sinh y.
$$

Sau cùng, ta có

$$
D(\cosh x) = \sinh x, \quad D(\sinh x) = \cosh x, \quad D(\tanh x) = 1 - \tanh^2 x = \frac{1}{\cosh^2 x}.
$$

Vì $\cosh x > 0$ với mọi $x$, ta suy ra rằng $\sinh x$ tăng ngặt trên $\mathbf{R}$; vì $\sinh 0 = 0$, suy ra $\sinh x$ có cùng dấu với $x$. Hệ quả là $\cosh x$ giảm nghiêm ngặt đối với $x \leq 0$, tăng ngặt đối với $x \geq 0$, sau cùng, $\tanh x$ tăng ngặt trên $\mathbf{R}$. Hơn nữa

$$
\lim_{x \to -\infty} \sinh x = -\infty, \qquad \lim_{x \to +\infty} \sinh x = +\infty
$$
$$
\lim_{x \to -\infty} \cosh x = \lim_{x \to +\infty} \cosh x = +\infty
$$
$$
\lim_{x \to -\infty} \tanh x = -1, \qquad \lim_{x \to +\infty} \tanh x = +1 \qquad \text{(hình 8 và 9)}.
$$

Đôi khi ta viết $\operatorname{Arg} \sinh x$ cho hàm nghịch đảo của $\sinh x$, là một ánh xạ tăng ngặt từ $\mathbf{R}$ lên $\mathbf{R}$: hàm này cũng có thể được biểu thị theo lôgarit, vì từ quan hệ $x = \sinh y = \frac{1}{2}(e^y - e^{-y})$ ta suy ra $e^{2y} - 2x e^y - 1 = 0$, và vì $e^y > 0$, ta có $e^y = x + \sqrt{x^2 + 1}$, nghĩa là

$$
\operatorname{Arg} \sinh x = \log \left( x + \sqrt{x^2 + 1} \right).
$$

Tương tự, ta ký hiệu bởi $\operatorname{Arg} \cosh x$ nghịch đảo của hạn chế của $\cosh x$ lên $[0, +\infty[$; ánh xạ này tăng ngặt từ $]1, +\infty[$ lên $]0, +\infty[$; như trên, người ta chứng minh được rằng

$$
\operatorname{Arg} \cosh x = \log \left( x + \sqrt{x^2 - 1} \right).
$$

Sau cùng, ta ký hiệu bởi Arg tanh $x$ hàm nghịch đảo của tanh $x$, là một ánh xạ tăng ngặt từ ]$-1, +1$ [ lên $\mathbf{R}$; hơn nữa ta có

$$
\operatorname{Arg} \tanh x = \frac{1}{2} \log \frac{1 + x}{1 - x}.
$$

#### Nhận xét {#fvr-iii-s1-n9-rem-1 .statement}

Đối với $z$ phức, đôi khi người ta viết

$$
\cosh z = \frac{1}{2} (e^z + e^{-z}) = \cos iz \\
\sinh z = \frac{1}{2} (e^z - e^{-z}) = -i \sin iz.
$$

Như vậy, các hàm này mở rộng lên $\mathbf{C}$ các hàm hyperbol được định nghĩa trên $\mathbf{R}$.

### Bài tập {#fvr-iii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
