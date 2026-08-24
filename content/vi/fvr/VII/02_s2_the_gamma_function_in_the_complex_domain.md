---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 2
section_title: THE GAMMA FUNCTION IN THE COMPLEX DOMAIN
lang: vi
source: fvr-i-vii
pdf_pages: 0330-0338, 0342-0343
extraction: ocr
subsections:
    - "no": 1
      title: EXTENDING THE GAMMA FUNCTION TO C
      page: 0
      pdf_page: 330
    - "no": 2
      title: THE COMPLEMENTS’ RELATION AND THE LEGENDRE-GAUSS MULTIPLICATION FORMULA
      page: 0
      pdf_page: 331
    - "no": 3
      title: STIRLING'S EXPANSION
      page: 0
      pdf_page: 334
statements: 6
exercises: 6
content_sha256: b7b4010961c351b7237b1591fbe3a1889f1a11cd29f1c181a0ee6c0a325321f8
translated_from: content/en/fvr/VII/02_s2_the_gamma_function_in_the_complex_domain.md
source_content_sha256: 6be47bc6aec4e2250251661d315af13917b7991b97da582bdb05fa9da882ba8a
translation_model: gpt-5.4
translation_run: translate-vi-f1288f74
glossary_version: 34
glossary_terms_sha256: defda4cb89814f42f3c609577bc32fe12881469211b9e1e88d0845292cc80eef
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. HÀM GAMMA TRONG MIỀN PHỨC

### 1. MỞ RỘNG HÀM GAMMA ĐẾN C

Hãy trở lại công thức của Weierstrass cho biểu thức

$$
\frac{1}{\Gamma(x)} = x\, e^{\gamma x} \prod_{n=1}^{\infty} \left(1 + \frac{x}{n}\right) e^{-x/n}
$$

cho $1/\Gamma(x)$ với mọi $x$ thực, và xét tích vô hạn có số hạng tổng quát là $\left(1 + \frac{z}{n}\right) e^{-z/n}$ với $z$ phức tùy ý. Có thể viết $e^{-z/n} = 1 - \frac{z}{n} + h(z)$, với $|h(z)| \leq \frac{|z|^2}{2n^2} e^{|z/n|}$ (III, p. 106, công thức (8)), do đó

$$
\left(1 + \frac{z}{n}\right) e^{-z/n} = 1 + v_n(z)
$$

với $|v_n(z)| \leq \frac{|z|^2}{n^2} \left(1 + \frac{e^{|z|}}{2}(1 + |z|)\right)$; như vậy tích vô hạn đang xét hội tụ tuyệt đối và đều trên mọi tập con compắc của $\mathbf{C}$; hơn nữa, giá trị của nó chỉ bằng không tại các điểm $z = -n$ (\emph{Gen. Top.}, IX, p. 214, hệ quả). Theo công thức (1) của VII, p. 315, với mọi $z$ phức người ta đặt

$$
\frac{1}{\Gamma(z)} = z\, e^{\gamma z} \prod_{n=1}^{\infty} \left(1 + \frac{z}{n}\right) e^{-z/n}.
$$

Phiếm hàm $\Gamma(z)$ do đó được xác định với mọi điểm $z \in \mathbf{C}$ trừ các điểm $-n$ ($n \in \mathbf{N}$); nó liên tục trên tập hợp này, và $(z + n)\Gamma(z) \sim \frac{(-1)^n}{n!}$ trên một lân cận của $-n$. Công thức (2) cho thấy rằng ta có $\Gamma(\overline{z}) = \overline{\Gamma(z)}$ với mọi $z$ khác một số nguyên âm.

Lập luận cho phép chuyển từ công thức của Gauss (VII, p. 307, công thức (8)) sang công thức của Weierstrass, khi đảo ngược các bước, cũng áp dụng được cho $z$ phức và cho thấy rằng, với $z \neq -n$ ($n \in \mathbf{N}$), ta có

$$
\Gamma(z) = \lim_{n \to \infty} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

với quy ước đặt $n^z = e^{z \log n}$. Vì

$$
\frac{n^{z+1} n!}{(z+1)(z+2)\ldots(z+n+1)} = z \frac{n}{n+1+z} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

nên khi chuyển sang giới hạn, ta lại có phương trình phiếm hàm cơ bản

$$
\Gamma(z+1) = z\, \Gamma(z)
$$

với mọi $z \neq -n$ ($n \in \mathbf{N}$).

Cho $ p $ là một số nguyên tùy ý $ > 0 $, và $ K_p $ là đĩa mở $ |z| < p $; với mọi $ z \in K_p $, và mọi số nguyên $ n > p $, $ 1 + \frac{z}{n} $ không phải là một số thực âm, nên $ \log \left( 1 + \frac{z}{n} \right) $ được xác định, và từ điều trên suy ra rằng chuỗi có số hạng tổng quát $ \log \left( 1 + \frac{z}{n} \right) - \frac{z}{n} $ ($ n > p $) *hội tụ chuẩn tắc* trên $ K_p $; điều tương tự cũng đúng với chuỗi thu được bằng cách lấy đạo hàm của số hạng tổng quát một số hữu hạn lần, vì ta có

$$
\left| \frac{1}{n} - \frac{1}{z+n} \right| \leq \frac{p}{n(n-p)} \quad \text{và} \quad \left| \frac{1}{(z+n)^k} \right| \leq \frac{1}{(n-p)^k} \qquad (k > 1)
$$

với $ z \in K_p $ và $ n > p $. Khi đó ta thấy (*xem* II, p. 59, *Nhận xét 3*) rằng $ \Gamma(z) $ là *khả vi vô hạn* tại mọi điểm $ z \in \mathbf{C} $ trừ các điểm $ -n $, và tại các điểm này ta có

$$
\frac{\Gamma'(z)}{\Gamma(z)} = -\gamma - \frac{1}{z} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{z+n} \right)
$$
(5)

$$
D^{k-1} \left( \frac{\Gamma'(z)}{\Gamma(z)} \right) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(z+n)^k} \qquad \text{với} \quad k \geq 2,
$$
(6)

các vế phải của (5) và (6) là *hội tụ chuẩn tắc* trên mọi tập con compắc của $ \mathbf{C} $ không chứa số nguyên nào $ \leq 0 $. Hơn nữa, ta có thể viết

$$
\log \Gamma(z) \equiv -\gamma z - \log z + \sum_{n=1}^{\infty} \left( \frac{z}{n} - \log \left( 1 + \frac{z}{n} \right) \right) \qquad (\text{mod. } 2\pi i)
$$
(7)

với quy ước rằng khi một lôgarit trong công thức này là lôgarit của một số thực âm thì nó nhận một trong hai giá trị giới hạn (sai khác nhau bởi $ 2\pi i $) của $ \log z $ tại điểm ấy; khi đó chuỗi ở vế phải của (7) là hội tụ chuẩn tắc trên mọi tập con compắc của $ \mathbf{C} $ không chứa số nguyên nào $ \leq 0 $.

### 2. QUAN HỆ CÁC PHẦN BÙ VÀ CÔNG THỨC PHÉP NHÂN LEGENDRE-GAUSS

Từ công thức (2) của VII, p. 315, suy ra ngay lập tức rằng, với mọi $ z \in \mathbf{C} $,

$$
\frac{1}{\Gamma(z)\Gamma(-z)} = -z^2 \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right).
$$

Bấy giờ khai triển Euler của $ \sin z $ (VI, p. 287, th. 2) cho thấy rằng

$$
z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right) = \frac{1}{\pi} \sin \pi z;
$$

tính đến phương trình phiếm hàm (4) của VII, p. 315, khi đó ta thấy rằng:

#### Mệnh đề 1 {#fvr-vii-s2-prop-1 .statement}

Với mọi số phức $ z $ ta có

$$
\frac{1}{\Gamma(z)\Gamma(1-z)} = \frac{1}{\pi} \sin \pi z
$$

(quan hệ của các phần bù).

HỆ QUẢ — Với mọi số thực $ t $ ta có

$$
|\Gamma(it)| = \sqrt{\frac{\pi}{t \sinh \pi t}} \quad (t \neq 0)
$$

$$
|\Gamma(\frac{1}{2} + it)| = \sqrt{\frac{\pi}{\cosh \pi t}}.
$$

Thật vậy, từ (8) suy ra $ \Gamma(it)\Gamma(-it) = \frac{i\pi}{t \sin \pi it} = \frac{\pi}{t \sinh \pi t} $, và ta có $ \Gamma(-it) = \overline{\Gamma(it)} $; tương tự, (8) cho

$$
\Gamma\left(\frac{1}{2} + it\right)\Gamma\left(\frac{1}{2} - it\right) = \frac{\pi}{\sin (\frac{\pi}{2} + \pi it)} = \frac{\pi}{\cos \pi it} = \frac{\pi}{\cosh \pi t},
$$

và ta có

$$
\Gamma\left(\frac{1}{2} - it\right) = \overline{\Gamma\left(\frac{1}{2} + it\right)}.
$$

Bây giờ, cho $ p $ là một số nguyên bất kỳ $ > 0 $ và xét tích

$$
f(z) = \Gamma\left(\frac{z+1}{p}\right) \Gamma\left(\frac{z+2}{p}\right) \ldots \Gamma\left(\frac{z+p}{p}\right).
$$

Theo (3) (VII, p. 315), với mọi $ z \neq -n \ (n \in \mathbf{N}) $, $ f(z) $ là giới hạn của tích

$$
\frac{n^{(z+1)/p} n!}{\left(\frac{z+1}{p}\right) \left(\frac{z+1}{p} + 1\right) \ldots \left(\frac{z+1}{p} + n\right)}
$$

$$
\frac{n^{(z+2)/p} n!}{\left(\frac{z+2}{p}\right) \left(\frac{z+2}{p} + 1\right) \ldots \left(\frac{z+2}{p} + n\right)} \cdots
$$

$$
\ldots \frac{n^{(z+p)/p} n!}{\left(\frac{z+p}{p}\right) \left(\frac{z+p}{p} + 1\right) \ldots \left(\frac{z+p}{p} + n\right)}
$$

$$
= \frac{n^{z+(p+1)/2} p^{(n+1)p} (n!)^p}{(z+1)(z+2) \ldots (z+(n+1)p)}
$$

và đặc biệt $ f(0) $ là giới hạn của tích

$$
\frac{n^{(p+1)/2} p^{(n+1)p} (n!)^p}{((n+1)p)!}
$$

từ đó suy ra rằng $ f(z)/f(0) $ là giới hạn của
$$
\frac{n^z ((n+1)p)!}{(z+1)(z+2)\ldots(z+(n+1)p)}
= z\ p^{-z} \left( \frac{n}{n+1} \right)^z \cdot \frac{((n+1)p)^z ((n+1)p)!}{z(z+1)(z+2)\ldots(z+(n+1)p)}
$$
điều này, theo (3) (VII, p. 315), cho
$$
f(z) = f(0)\ z\ p^{-z}\ \Gamma(z).
$$
Nhưng ta có thể viết
$$
f(0) = \prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) = \prod_{k=1}^{p-1} \Gamma \left( 1 - \frac{k}{p} \right) = \sqrt{\prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) \Gamma \left( 1 - \frac{k}{p} \right)}
$$
vì $ f(0) > 0 $; khi đó quan hệ bù cho
$$
f(0) = \sqrt{\pi^{p-1} / \prod_{k=1}^{p-1} \sin \frac{k\pi}{p}}
$$
và vì tích ở vế phải bằng $ p/2^{p-1} $ (VI, p. 284, cor. 1), cuối cùng ta thấy rằng:

#### Mệnh đề 2 {#fvr-vii-s2-prop-2 .statement}

*Với mọi số phức* $ z $ *không là một số nguyên* $ \leqslant 0 $ *và với mọi số nguyên* $ p > 0 $ *ta có*
$$
\Gamma \left( \frac{z}{p} \right) \Gamma \left( \frac{z+1}{p} \right) \ldots \Gamma \left( \frac{z+p-1}{p} \right) = (2\pi)^{(p-1)/2}\ p^{\frac{1}{2}-z}\ \Gamma(z)
$$
*(công thức nhân Legendre-Gauss)*.

#### Mệnh đề 3 {#fvr-vii-s2-prop-3 .statement}

*Với mọi số thực* $ x > 0 $ *ta có*
$$
\int_1^{x+1} \log \Gamma(t)\ dt = x(\log x - 1) + \frac{1}{2} \log 2\pi
$$
*(tích phân của Raabe)*.

Trước hết ta thiết lập công thức (13) cho $ x = 0 $. Vì $ \log \Gamma(x) \sim \log \frac{1}{x} $ khi $ x $ tiến tới 0, tích phân $ \int_0^1 \log \Gamma(x)\ dx $ hội tụ. Hơn nữa, hàm $ \log \Gamma(x) $ giảm trên $ ]0, 1] $ (VII, p. 310); do đó với mọi $ \alpha > 0 $ ta có
$$
\frac{1}{n} \sum_{k=1}^q \log \Gamma \left( \frac{k}{n} \right) \leqslant \int_0^\alpha \log \Gamma(x)\ dx,
$$

$q$ là số nguyên lớn nhất sao cho $q/n \leqslant \alpha$. Vì $\int_0^\alpha \log \Gamma(x) dx$ tiến tới 0 cùng với $\alpha$ và cũng vì $\frac{1}{n} \sum_{k=q+1}^n \log \Gamma \left( \frac{k}{n} \right)$ tiến tới $\int_\alpha^1 \log \Gamma(x) dx$ khi $n$ tiến tới $+\infty$ (II, p. 57, Mệnh đề 5) nên ta có

$$
\int_0^1 \log \Gamma(x) dx = \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^n \log \Gamma \left( \frac{k}{n} \right).
$$

Nhưng, theo (12), vế phải của công thức này là giới hạn của

$$
\frac{n-1}{2n} \log 2\pi - \frac{1}{2} \frac{\log n}{n},
$$

do đó

$$
\int_0^1 \log \Gamma(x) dx = \frac{1}{2} \log 2\pi.
$$ (14)

Tiếp theo ta nhận xét rằng từ đồng nhất thức

$$
\log \Gamma(x+1) = \log \Gamma(x) + \log x
$$

suy ra, sau khi lấy tích phân, rằng với $x > 0$

$$
\int_0^x \log \Gamma(t+1) dt = \int_0^x \log \Gamma(t) dt + \int_0^x \log t dt.
$$

Nhưng tích phân ở vế trái cũng bằng $\int_1^{x+1} \log \Gamma(t) dt$. Vậy, theo (14),

$$
\int_1^{x+1} \log \Gamma(t) dt = \int_0^x \log t dt + \frac{1}{2} \log 2\pi = x (\log x - 1) + \frac{1}{2} \log 2\pi.
$$

### 3. KHAI TRIỂN STIRLING

Cho $x$ và $y$ là hai số phức không nằm trên nửa trục thực âm; theo công thức (3) của VII, p. 315, với các quy ước của VII, p. 316, liên quan đến các lôgarit, $\log \Gamma(x) - \log \Gamma(y)$ đồng dư modulo $2\pi i$ với giới hạn của biểu thức

$$
(x-y) \log n + \sum_{k=0}^n \left( \log(y+k) - \log(x+k) \right).
$$ (15)

Đặt $f(t) = \log(y+t) - \log(x+t)$; ta áp dụng công thức tổng Euler-Maclaurin (VI, p. 288) cho hàm $f$:

$$
f(0) + f(1) + \cdots + f(n) = \int_0^{n+1} f(t) dt - \frac{1}{2} (f(n+1) - f(0))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(n+1) - f^{(2k-1)}(0) \right) + T_p(n)
$$

với
$$
|T_p(n)| \leq \frac{4 e^{2\pi}}{(2\pi)^{2p+1}} \int_0^{n+1} |f^{(2p+1)}(u)|\ du.
$$
(16)

Vì
$$
f^{(m)}(t) = (-1)^{m-1} (m-1)! \left( \frac{1}{(y+t)^m} - \frac{1}{(x+t)^m} \right),
$$
nên $f^{(2k-1)}(n+1)$ tiến tới 0 khi $n$ tiến tới $+\infty$, với mọi $k \geq 1$; điều đó cũng đúng đối với
$$
f(n+1) = \log \left( 1 + \frac{y}{n+1} \right) - \log \left( 1 + \frac{x}{n+1} \right).
$$
Hơn nữa, ta có
$$
\int_0^{n+1} \log(x+t)\ dt = (x+n+1)(\log(x+n+1)-1) - x(\log x - 1);
$$
khi $n$ tiến tới $+\infty$, ta có khai triển tiệm cận
$$
(x+n)(\log(x+n)-1) = n \log n - n + x \log n + O \left( \frac{1}{n} \right).
$$
Thay vào biểu thức (15), cuối cùng ta thấy rằng, khi $n$ tiến tới $+\infty$, $T_p(n)$ có một giới hạn $R_p(x,\ y)$ và rằng có thể viết
$$
\log \Gamma(x) - g(x) \equiv \log \Gamma(y) - g(y) + R_p(x,\ y) \quad (\text{mod. } 2\pi i)
$$
khi đặt
$$
g(x) = x \log x - x - \frac{1}{2} \log x + \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{x^{2k-1}}.
$$
(17)

Bây giờ chúng ta sẽ đánh giá một chặn của $R_p(x,\ y)$ với sự trợ giúp của (16), giả sử rằng $x$ và $y$ đều thuộc tập con $\mathbf{H}_A$ của $\mathbf{C}$ được xác định bởi quan hệ "$\mathcal{R}(z) \geq A$ or $|\mathcal{I}(z)| \geq A$", trong đó $A$ là một số tùy ý $> 0$ (hình 2). Để làm điều đó, ta nhận xét rằng nếu $x = s + it$ với $s > A$ thì ta có $|x+u| \geq A+u$ với mọi $u > 0$, và do đó
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_0^\infty \frac{du}{(A+u)^{2p+1}} = \frac{1}{2pA^{2p}}.
$$
Tương tự, nếu $|t| \geq A$ thì ta có $|x+u| = |s+u+it| \geq \sqrt{A^2 + (s+u)^2}$ với mọi $u$ thực, do đó
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_{-\infty}^{+\infty} \frac{du}{(A^2 + u^2)^{p+1/2}} = \frac{2}{A^{2p}} \int_0^\infty \frac{dv}{(1+v^2)^{p+1/2}}.
$$
Như vậy ta thấy rằng, khi $x$ và $y$ thuộc $\mathbf{H}_A$, ta có
$$
|R_p(x,\ y)| \leq \frac{C_p}{A^{2p}}
$$

![Biểu đồ mặt phức cho thấy các trục được ghi nhãn t, s, và các miền H_A, A, -A, 0](Fig. 2)

trong đó C_p chỉ phụ thuộc vào p. Bây giờ cho $ \mathfrak{F} $ là bộ lọc có các tập hợp H_A làm cơ sở; tiêu chuẩn Cauchy cho thấy rằng, theo bộ lọc $ \mathfrak{F} $, hàm $ \log \Gamma(z) - g(z) $ có một giới hạn hữu hạn $ \delta $ (theo modulo $ 2\pi i $) và rằng, nếu đặt $ \omega(z) = \max(\mathcal{R}(z), |\mathcal{I}(z)|) $, thì ta có

$$
\log \Gamma(z) - g(z) - \delta \equiv O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i).
$$

Với x thực và > 0 ta có $ \Gamma(x) > 0 $, và $ g(x) $ là thực, nên có thể giả sử rằng $ \delta $ là thực và ta có

$$
\log \Gamma(x) = g(x) + \delta + O \left( \frac{1}{x^{2p}} \right).
$$

Bây giờ chúng ta sẽ suy ra giá trị của hằng $ \delta $: theo mệnh đề 2 của VII, p. 318, áp dụng cho $ p = 2 $, ta có, với $ x $ thực tiến tới $ +\infty $

$$
\begin{align*}
&\frac{x-1}{2} \log \frac{x}{2} - \frac{x}{2} + \frac{x}{2} \log \frac{x+1}{2} - \frac{x+1}{2} + 2\delta \\
&\qquad = x \log x - x - \frac{1}{2} \log x + (\frac{1}{2} - x) \log 2 + \frac{1}{2} \log 2\pi + \delta + o(1)
\end{align*}
$$

từ đó dễ dàng suy ra rằng $ \delta = \frac{1}{2} \log 2\pi $. Cuối cùng ta có kết quả sau:

#### Mệnh đề 4 {#fvr-vii-s2-prop-4 .statement}

*Dọc theo bộ lọc $ \mathfrak{F} $ ta có (với mọi số nguyên $ p \geqslant 1 $) khai triển tiệm cận*

$$
\log \Gamma(z) \equiv z \log z - z - \frac{1}{2} \log z + \frac{1}{2} \log 2\pi
+ \sum_{k=1}^{p} \frac{b_{2k}}{2k(2k-1)} \frac{1}{z^{2k-1}} + O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i)
$$

*(Khai triển Stirling)*.

#### Hệ quả {#fvr-vii-s2-n3-cor-1 .statement}

*Dọc theo bộ lọc $ \mathfrak{F} $ ta có*

$$
\Gamma(z) \sim \sqrt{2\pi} \exp(z \log z - z - \frac{1}{2} \log z).
$$

Đặc biệt, với $ x $ thực tiến đến $ +\infty $ thì công thức (20) có thể viết thành

$$
\Gamma(x) \sim \sqrt{2\pi} \, x^{x-1/2} e^{-x},
$$

do đó, khi số nguyên $ n $ tiến đến $ +\infty $,

$$
n! \sim \sqrt{2\pi} \, n^{n+1/2} \, e^{-n}
$$

(*xem* V, p. 244).

Từ đây người ta có thể suy ra nhiều công thức. Ví dụ, với mọi số phức $ \alpha $ và mọi số nguyên $ n $ ta có, khi $ n $ tiến tới $ +\infty $,

$$
\frac{\Gamma(n+\alpha)}{\Gamma(n)} \sim n^{\alpha} \quad (= e^{\alpha \log n}).
$$

Tương tự, với mọi số phức $ a $ không là một số nguyên $ \leqslant 0 $ ta có

$$
a(a+1)(a+2)\ldots(a+n) = \frac{\Gamma(n+a+1)}{\Gamma(a)} \sim \frac{\sqrt{2\pi}}{\Gamma(a)} \, n^{n+a+1/2} \, e^n
$$

và với mọi số phức $ a $ không là một số nguyên $ \geqslant 0 $

$$
\binom{a}{n} = \frac{(-1)^n}{\Gamma(-a)} \frac{\Gamma(n-a)}{\Gamma(n+1)} \sim \frac{(-1)^n}{\Gamma(-a)} \, n^{-a-1}.
$$

Cuối cùng, với mọi hằng thực $ k > 1 $ ta có

$$
\binom{kn}{n} = \frac{\Gamma(kn+1)}{\Gamma(n+1) \Gamma((k-1)n+1)} \sim \sqrt{\frac{k}{2\pi(k-1)n}} \left( \frac{k^k}{(k-1)^{k-1}} \right)^n.
$$

Lập luận tương tự dẫn đến mệnh đề tương tự sau đây:

#### Mệnh đề 5 {#fvr-vii-s2-prop-5 .statement}

Theo bộ lọc $ \mathfrak{F} $ ta có (với mọi số nguyên $ p \geqslant 1 $), khai triển tiệm cận

$$
\frac{\Gamma'(z)}{\Gamma(z)} = \log z - \frac{1}{2z} - \sum_{k=1}^{p} \frac{b_{2k}}{2k} \frac{1}{z^{2k}} + O \left( \frac{1}{(\omega(z))^{2p+1}} \right).
$$

Thay cho mệnh đề 2 của VII, p. 318, người ta dùng công thức

$$
\int_{x}^{x+1} \frac{\Gamma'(t)}{\Gamma(t)} \, dt = \log \Gamma(x+1) - \log \Gamma(x) = \log x
$$

để xác định hằng.

### Bài tập {#fvr-vii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
