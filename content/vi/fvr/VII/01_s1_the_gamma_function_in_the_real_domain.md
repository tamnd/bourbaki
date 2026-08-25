---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 1
section_title: THE GAMMA FUNCTION IN THE REAL DOMAIN
lang: vi
source: fvr-i-vii
pdf_pages: 0320-0329, 0340-0342
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE GAMMA FUNCTION
      page: 0
      pdf_page: 320
    - "no": 2
      title: PROPERTIES OF THE GAMMA FUNCTION
      page: 0
      pdf_page: 322
    - "no": 3
      title: THE EULER INTEGRALS
      page: 0
      pdf_page: 325
statements: 8
exercises: 6
content_sha256: 269b1726990989ee10e2c92cf6f19f0a4cb068f37f951d5e899dc8b7c0a38f4a
translated_from: content/en/fvr/VII/01_s1_the_gamma_function_in_the_real_domain.md
source_content_sha256: 752ce38907fef650e8ea8bf4b5fa4f04eca836602530c6e62155c59c5cb349bb
translation_model: gpt-5.4
translation_run: translate-vi-f4ac4aa2
glossary_version: 34
glossary_terms_sha256: 06416adb088ec5c56b6dd43613d8f2e4ccad8f1eb6b86f9210f272576ddb1a06
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. HÀM GAMMA TRONG MIỀN THỰC

### 1. ĐỊNH NGHĨA CỦA HÀM GAMMA

Ta đã định nghĩa (Lý thuyết tập hợp, III, p. 179) hàm $n!$ với mọi số nguyên $n \geq 0$, bằng tích $\prod_{0 \leq k < n} (n - k)$; do đó $0! = 1$ và $(n + 1)! = (n + 1)\, n!$ với $n \geq 0$.

Ta đặt $\Gamma(n) = (n - 1)!$ với mỗi số nguyên $n \geq 1$; ta dự định định nghĩa, trên tập hợp các số thực $x > 0$, một hàm liên tục $\Gamma(x)$ mở rộng hàm $\Gamma$ đã được định nghĩa trên tập hợp các số nguyên $\geq 1$.

Rõ ràng là có vô hạn nhiều hàm như vậy; vì $\Gamma(n + 1) = n\Gamma(n)$ với mọi số nguyên $n \geq 1$ nên ta sẽ chỉ xét, trong số các hàm liên tục mở rộng $\Gamma$, những hàm thỏa mãn phương trình

$$
f(x + 1) = x f(x)
$$

cho mọi $x > 0$.

Để một nghiệm của phương trình này là một mở rộng của $\Gamma(n)$ thì điều kiện cần và đủ là nó cũng thỏa mãn $f(1) = 1$.

Nếu $f$ thỏa mãn (1) thì, bằng phép truy hồi theo $n$,

$$
f(x + n) = x(x + 1)(x + 2) \ldots (x + n - 1)\, f(x)
$$

với mọi số nguyên $n > 1$ và với mọi $x > 0$. Quan hệ này cho thấy, đặc biệt, rằng các giá trị của $f$ trên một khoảng $]n, n + 1]$ ($n$ là một số nguyên $\geq 1$) được xác định bởi các giá trị của nó trên khoảng $]0, 1]$. Ngược lại, cho $\varphi$ là một hàm liên tục trên $]0, 1]$ chỉ thỏa mãn các điều kiện $\varphi(1) = 1$, $\lim_{x \to 0} x \varphi(x) = 1$; với mọi số nguyên $n \geq 1$ ta định nghĩa $f$ trên khoảng $]n, n + 1]$ bởi quan hệ

$$
f(x) = (x - 1)(x - 2) \ldots (x - n)\, \varphi(x - n);
$$

rõ ràng là $f$ liên tục trên $]0, +\infty[$, thỏa mãn phương trình (1), và mở rộng $\Gamma(n)$.

Nếu $f$ là một nghiệm liên tục của (1) và nhận các giá trị $> 0$ trên $]0, 1]$ thì, theo (2), nó nhận các giá trị $> 0$ trên $]0, +\infty[$; khi đó hàm $g(x) = \log f(x)$ được xác định và liên tục trên ]0, +∞[ và thỏa mãn phương trình

$$
g(x+1) - g(x) = \log x
$$

(3)

trên khoảng này.

Nếu $g_1$ là một nghiệm liên tục thứ hai của (3) trên ]0, +∞[, và nếu $h = g_1 - g$, thì ta có $h(x+1) - h(x) = 0$ với mọi $x > 0$; nói cách khác, $h$ là một hàm tuần hoàn liên tục có chu kỳ 1, được xác định trên ]0, +∞[; ngược lại, với mọi $h$ có tính chất này, $g + h$ là một nghiệm liên tục của (3).

#### Mệnh đề 1 {#fvr-vii-s1-prop-1 .statement}

*Tồn tại một và chỉ một hàm lồi* $g$ *được xác định trên* ]0, +∞[ *thỏa mãn phương trình* (3) *và nhận giá trị 0 tại* $x = 1$.

Trước hết ta chỉ ra rằng nếu có một hàm $g$ thỏa mãn các điều kiện đã nêu thì nó được xác định rõ trên khoảng ]0, 1], và do đó trên khoảng ]0, +∞[. Thật vậy, với mọi số nguyên $n > 1$ hệ số góc của đường thẳng nối điểm $(n, g(n))$ với điểm $(x, g(x))$ là một hàm tăng theo $x$, vì $g$ là lồi (I, p. 27, mệnh đề 5); do đó ta phải có, với $0 < x \leq 1$,

$$
\frac{g(n-1) - g(n)}{(n-1) - n} \leq \frac{g(n+x) - g(n)}{(n+x) - n} \leq \frac{g(n+1) - g(n)}{(n+1) - n}
$$

nghĩa là, theo (3),

$$
x \log(n-1) \leq g(x+n) - g(n) \leq x \log n.
$$

Bây giờ, theo (3),

$$
g(x+n) - g(n) = g(x) + \log x + \sum_{k=1}^{n-1} (\log(x+k) - \log k).
$$

Hơn nữa, ta có thể viết $\log n = \sum_{k=2}^n \log \frac{k}{k-1}$ nên bất đẳng thức (4) có thể viết thành

$$
x \sum_{k=2}^{n-1} \log \frac{k}{k-1} \leq g(x) + \log x + \sum_{k=2}^n (\log(x+k-1) - \log(k-1))
$$
$$
\leq x \sum_{k=2}^n \log \frac{k}{k-1}.
$$

Đặt, với mọi $n \geq 2$,

$$
u_n(x) = x \log \frac{n}{n-1} - \log(x+n-1) + \log(n-1)
$$

(5)

và

$$
g_n(x) = -\log x + \sum_{k=2}^n u_k(x).
$$

Khi đó đối với $0 < x \leq 1$ ta có
$$
g_n(x) - x \log \frac{n}{n-1} \leq g(x) \leq g_n(x).
$$
(6)

Vì $\log \frac{n}{n-1}$ tiến tới 0 khi $n$ tiến tới $+\infty$ nên từ (6) suy ra rằng nếu một nghiệm $g$ tồn tại thì tất yếu nó bằng, trên $]0, 1]$, với *giới hạn* của các $g_n(x)$.

Bây giờ người ta suy ra ngay lập tức từ (5) rằng với $x$ cố định và $> 0$ ta có
$$
u_n(x) = -x \log \left( 1 - \frac{1}{n} \right) - \log \left( 1 + \frac{x-1}{n} \right) + \log \left( 1 - \frac{1}{n} \right) \sim \frac{x(x-1)}{2n^2}
$$
khi $n$ tiến tới $+\infty$, điều này chứng minh rằng chuỗi có số hạng tổng quát $u_n(x)$ hội tụ với mọi $x > 0$. Mỗi hàm $u_n(x)$ đều lồi trên $]0, +\infty[$, cũng như $-\log x$, nên hàm $g(x) = -\log x + \sum_{n=2}^{\infty} u_n(x)$ lồi trên khoảng này (I, p. 27, mệnh đề 2 và mệnh đề 4); cuối cùng, ta có $u_n(1) = 0$, do đó $g(1) = 0$, và
$$
u_n(x+1) = u_{n+1}(x) + x \left( \log \frac{n}{n-1} - \log \frac{n+1}{n} \right)
$$
do đó
$$
g(x+1) = -\log(x+1) + x \log 2 + \sum_{n=3}^{\infty} u_n(x) = \log x + g(x);
$$
nói cách khác, $g$ thỏa mãn phương trình (3) của VII, p. 306.

#### Định nghĩa 1 {#fvr-vii-s1-def-1 .statement}

*Ta ký hiệu bởi* $\Gamma(x)$ *hàm* $> 0$ *được xác định trên khoảng* $]0, +\infty[$, *thỏa mãn phương trình*
$$
\Gamma(x+1) = x \Gamma(x),
$$
*(7)*
*và sao cho* $\Gamma(1) = 1$ *và* $\log \Gamma(x)$ *là lồi trên* $]0, +\infty[$.

### 2. CÁC TÍNH CHẤT CỦA HÀM GAMMA

#### Mệnh đề 2 {#fvr-vii-s1-prop-2 .statement}

*Với mọi* $x > 0$ *ta có*
$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x n!}{x(x+1)\ldots(x+n)}
$$
*(công thức của Gauss)*, *và*
$$
\Gamma(x) = e^{-\gamma x} \frac{1}{x} \prod_{n=1}^{\infty} \frac{e^{x/n}}{1 + \frac{x}{n}}
$$
(9) trong đó $\gamma$ ký hiệu hằng số của Euler, và tích vô hạn ở vế phải của (9) hội tụ tuyệt đối và đều trên mọi khoảng compact của $\mathbf{R}$ không chứa số nguyên nào $< 0$ (công thức của Weierstrass).

Hàm $\Gamma(x)$ khả vi vô hạn lần trên $]0, +\infty[$ và ta có

$$
\frac{\Gamma'(x)}{\Gamma(x)} = -\gamma - \frac{1}{x} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{x+n} \right)
$$

và

$$
\mathrm{D}^k (\log \Gamma(x)) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(x+n)^k} \quad \text{với} \quad k \geq 2,
$$

các chuỗi ở vế phải của (10) và (11) tuyệt đối hội tụ và hội tụ đều trên mọi khoảng compắc không chứa số nguyên nào $\leq 0$.

Thật vậy, chứng minh của prop. 1 của VII, p. 306, chỉ ra rằng

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x (n-1)!}{x(x+1)\ldots(x+n-1)}
$$

do đó có công thức của Gauss, vì $\frac{n}{x+n}$ tiến tới 1 khi $n$ tiến tới $+\infty$. Ta cũng có thể viết

$$
\log \frac{n}{n-1} = \frac{1}{n-1} + \left( \log \frac{n}{n-1} - \frac{1}{n-1} \right).
$$

nên (theo ký hiệu của prop. 1)

$$
\exp(u_n(x)) = e^{(\log \frac{n}{n-1} - \frac{1}{n-1})} \frac{e^{x/(n-1)}}{1 + \frac{x}{n-1}}
$$

và chuỗi có số hạng tổng quát $\log \frac{n}{n-1} - \frac{1}{n-1}$ là tuyệt đối hội tụ và có tổng bằng $-\gamma$, trong đó $\gamma$ ký hiệu hằng số Euler (V, p. 242), do đó ta thu được công thức của Weierstrass.

Với $|x| \leq a$ ta có $|1/(x+n)^k| \leq 1/(n-a)^k$ khi $n > a$, do đó chuỗi ở vế phải của công thức (11) hội tụ tuyệt đối và đều trên mọi khoảng compact của $\mathbf{R}$ không chứa số nguyên nào $\leq 0$, với mọi số nguyên $k \geq 2$; cùng lập luận ấy áp dụng được cho vế phải của (10), vì $\left| \frac{1}{n} - \frac{1}{x+n} \right| \leq \frac{a}{n(n-a)}$ với $|x| \leq a$ và $n > a$. Vì các chuỗi này thu được bằng cách vi phân từng số hạng chuỗi

$$
\log \Gamma(x) = -\gamma x - \log x + \sum_{n=1}^{\infty} \left( \frac{x}{n} - \log \left( 1 + \frac{x}{n} \right) \right)
$$

và chuỗi này hội tụ với mọi $x > 0$, nên chuỗi có số hạng tổng quát $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ hội tụ tuyệt đối và đều trên mọi khoảng compact được chứa trong [0, +∞[, và ta có các hệ thức (10) và (11) của VII, p. 308, với mọi x > 0 (II, p. 52, định lý 1). Hơn nữa, với mọi x ∈ ℝ, biểu thức $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ được xác định khi n đủ lớn, nên định lý 1 của II, p. 52, lại cho thấy rằng tích vô hạn ở vế phải của (9) (VII, p. 307) hội tụ tuyệt đối và đều trên mọi khoảng compact không chứa số nguyên nào $\leq 0$.

Hàm $\Gamma(x)$, được xác định với $x > 0$, có thể được mở rộng ra toàn bộ tập hợp các điểm x khác các số nguyên $\leq 0$ sao cho thỏa mãn phương trình (7) của VII, p. 307, trên tập hợp này: chỉ cần, với $-(n+1) < x < -n$, đặt
$$
\Gamma(x) = \frac{1}{x(x+1)\ldots(x+n)} \Gamma(x+n+1).
$$
Theo mệnh đề 2 của VII, p. 307, các công thức (8), (9), (10) và (11) của VII, p. 307 và 308, với $D^k(\log |\Gamma(x)|)$ thay thế $D^k(\log \Gamma(x))$ trong (11), vẫn đúng trên tập hợp này. Công thức (9) (VII, p. 307) cho thấy rằng $\Gamma(x) \sim 1/x$ khi x tiến tới 0, do đó, theo (7) của VII, p. 307,
$$
\Gamma(x) \sim \frac{(-1)^n}{n! (x+n)}
$$
khi x tiến tới $-n$ ($n$ là một số nguyên $\geq 0$). Khi đó hàm $1/\Gamma(x)$ có thể được mở rộng bằng liên tục ra toàn bộ ℝ, bằng cách gán cho nó giá trị 0 tại các số nguyên $\leq 0$; khi đó, với mọi $x \in \mathbf{R}$
$$
\frac{1}{\Gamma(x)} = \lim_{n \to \infty} \frac{x(x+1)\ldots(x+n)}{n^n n!}
$$
và
$$
\frac{1}{\Gamma(x)} = e^{y_1 x} x \prod_{n=1}^{\infty} \left( 1 + \frac{x}{n} \right) e^{-y_1/n}
$$
và người ta chứng minh như trong mệnh đề 2 của VII, p. 307, rằng tích vô hạn ở vế phải của (13) hội tụ tuyệt đối và đều trên mọi khoảng compắc của ℝ.

Vì $\Gamma(x) > 0$ với $x > 0$, công thức (7) của VII, p. 307, cho thấy rằng $\Gamma(x) < 0$ với $-(2n-1) < x < -(2n-2)$ và $\Gamma(x) > 0$ với
$$
-2n < x < -(2n-1)
$$
($n$ là một số nguyên $\geq 1$); ngoài ra $\Gamma(x)$ có giới hạn phải bằng $+\infty$ tại các điểm $-2n$ và bằng $-\infty$ tại các điểm $-(2n+1)$, và có giới hạn trái bằng $-\infty$ tại các điểm $-2n$ và bằng $+\infty$ tại các điểm $-(2n+1)$ (với mọi $n \in \mathbf{N}$). Công thức (11) của VII, p. 308, cho thấy rằng, với $k = 2$, vế phải luôn luôn $\geq 0$ khi nó được xác định, nên
$$
\Gamma''(x) \Gamma(x) - (\Gamma'(x))^2 \geq 0,
$$

và do đó $\Gamma''(x)$ có cùng dấu với $\Gamma(x)$; vì thế $\Gamma$ là *lồi* đối với $x > 0$ và đối với $-(2n+2) < x < -(2n+1)$, và *lõm* đối với $-(2n+1) < x - 2n \ (n \in \mathbf{N})$; từ đó suy ra rằng, trên các khoảng mà $\Gamma$ lồi, $\Gamma'(x)$ tăng từ $-\infty$ đến $+\infty$, và trên các khoảng mà $\Gamma$ lõm, $\Gamma'(x)$ giảm từ $+\infty$ đến $-\infty$. Do đó có đồ thị của $\Gamma$ (hình 1).

**Hình 1**

### 3. CÁC TÍCH PHÂN EULER

Để cho gọn, ta sẽ nói rằng một hàm $f$ được xác định trên một khoảng $I \subset \mathbf{R}$, và $> 0$ trên khoảng này, là *lồi theo lôgarit* trên $I$ nếu $\log f$ lồi trên $I$. Định nghĩa của $\Gamma(x)$ cho thấy rằng hàm này là *lồi theo lôgarit* trên $]0, +\infty[$.

Hiển nhiên là *tích* của hai hàm lồi theo lôgarit trên $I$ cũng lồi theo lôgarit trên $I$. Hơn nữa:

#### Bổ đề 1 {#fvr-vii-s1-lem-1 .statement}

*Cho $f$ và $g$ là hai hàm số $> 0$ và khả vi hai lần trên một khoảng mở $I$. Nếu $f$ và $g$ là các hàm lồi theo lôgarit trên $I$, thì $f + g$ lồi theo lôgarit trên $I$.*

Quan hệ $D^2 (\log f(x)) \geq 0$ có thể được viết thành $f(x)f''(x) - (f'(x))^2 \geq 0$. Ta quy về việc chỉ ra rằng các quan hệ $a > 0, a' > 0, ac - b^2 \geq 0, a'c' - b'^2 \geq 0$ kéo theo $(a + a')(c + c') - (b + b')^2 \geq 0$; mà, khi $a > 0$, quan hệ $ac - b^2 \geq 0$ tương đương với việc dạng toàn phương $ax^2 + 2bxy + cy^2$ là $\geq 0$ trên $\mathbf{R}^2$, và hiển nhiên là nếu

$$
ax^2 + 2bxy + cy^2 \geq 0 \quad \text{và} \quad a'x^2 + 2b'xy + c'y^2 \geq 0
$$

trên $\mathbf{R}^2$ thì cả $(a + a')x^2 + 2(b + b')xy + (c + c')y^2 \geq 0$ cũng vậy trên $\mathbf{R}^2$.

#### Bổ đề 2 {#fvr-vii-s1-lem-2 .statement}

Cho $f$ là một hàm thực hữu hạn, $> 0$, được xác định và liên tục trên tích $I \times J$ của hai khoảng mở của $\mathbf{R}$, và sao cho, với mọi $t \in J$ hàm $x \mapsto f(x, t)$ là lồi lôgarit và khả vi hai lần trên $I$. Dưới các giả thiết đó, nếu nguyên $g(x) = \int_J f(x, t) dt$ hội tụ với mọi $x \in I$, thì $g$ là lồi lôgarit trên $I$.

Trước hết ta chứng minh rằng với mọi khoảng compact $K \subset J$ hàm $g_K(x) = \int_K f(x, t) dt$ là lồi lôgarit. Thật vậy, nếu $K = [a, b]$, dãy các hàm

$$
g_n(x) = \frac{b-a}{n} \sum_{k=0}^{n-1} f\left(x, a + k \frac{b-a}{n}\right)
$$

hội tụ đơn giản tới $g_K(x)$ trên $I$ (II, p. 57, mệnh đề 5), do đó $\log g_n$ hội tụ đơn giản tới $\log g_K$; theo bổ đề 1 của VII, p. 310, $\log g_n$ là lồi trên $I$, nên (I, p. 27, mệnh đề 4) $\log g_K$ cũng vậy.

Mặt khác, $g$ là giới hạn điểm của các $g_K$ theo tập có hướng các khoảng con compact của $I$ (II, p. 64), nên $\log g$ là giới hạn điểm của các $\log g_K$; các hàm sau cùng này lồi trên $I$, nên $\log g$ cũng lồi (I, p. 27, mệnh đề 4).

Có thể dễ dàng chỉ ra rằng các bổ đề 1 và 2 vẫn đúng ngay cả khi không giả thiết rằng các hàm khả vi hai lần (VII, p. 327, bài tập 5).

#### Bổ đề 3 {#fvr-vii-s1-lem-3 .statement}

Cho $\varphi$ là một hàm liên tục và $> 0$ trên một khoảng mở $J$ được chứa trong $[0, +\infty[$. Nếu $I$ là một khoảng mở sao cho nguyên $g(x) = \int_J t^{x-1} \varphi(t) dt$ hội tụ với mọi $x \in I$, thì $g$ lồi lôgarit trên $I$.

Thật vậy, $\log t^{x-1} = (x-1) \log t$ là một hàm của $x$ lồi và khả vi hai lần với mọi $t > 0$, nên bổ đề 2 áp dụng được.

#### Mệnh đề 3 {#fvr-vii-s1-prop-3 .statement}

Với mọi $x > 0$

$$
\Gamma(x) = \int_0^\infty e^{-t} t^{x-1} dt
$$

(nguyên Euler thứ hai).

Bây giờ hàm $g(x) = \int_0^\infty e^{-t} t^{x-1} dt$ được xác định với mọi $x > 0$ (V, p. 229); bổ đề 3 của VII, p. 311, khi đó cho thấy rằng nó *lồi theo logarit* trên ]$0, +\infty[$. Hơn nữa, bằng cách tích phân từng phần, ta có

$$
g(x+1) = \int_0^\infty e^{-t} t^x \, dt = -e^{-t} t^x \Big|_0^\infty + x \int_0^\infty e^{-t} t^{x-1} dt = x \, g(x).
$$

Nói cách khác, $g$ là một nghiệm của phương trình (1) của VII, p. 305; cuối cùng,

$$
g(1) = \int_0^\infty e^{-t} \, dt = 1;
$$

do đó mệnh đề suy ra từ mệnh đề 1 của VII, p. 306.

Bằng phép thay đổi biến $e^{-t} = u$ người ta suy ra từ (14) (VII, p. 311) công thức

$$
\Gamma(x) = \int_0^1 \left( \log \frac{1}{t} \right)^{x-1} dt.
$$

Tương tự, từ phép thay đổi biến $u = t^{1/x}$ ta thu được

$$
x \, \Gamma(x) = \int_0^\infty e^{-t^{1/x}} \, dt
$$

lại nữa, có xét đến (7) (VII, p. 3),

$$
\Gamma \left( 1 + \frac{1}{x} \right) = \int_0^\infty e^{-t^x} \, dt
$$

Đặc biệt, với $x = 2$

$$
\Gamma \left( \frac{3}{2} \right) = \frac{1}{2} \Gamma \left( \frac{1}{2} \right) = \int_0^\infty e^{-t^2} \, dt.
$$

#### Mệnh đề 4 {#fvr-vii-s1-prop-4 .statement}

*Với $x > 0$ và $y > 0$ tích phân*

$$
\mathbf{B}(x, y) = \int_0^1 t^{x-1} (1-y)^{y-1} \, dt
$$

(*tích phân Euler thứ nhất*) *có giá trị*

$$
\mathbf{B}(x, y) = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$

Thật vậy, tích phân này hội tụ khi $x > 0$ và $y > 0$ (V, p. 229). Theo bổ đề 3 của I, p. 311, hàm $x \mapsto \mathbf{B}(x, y)$ là *lồi lôgarit* khi $x > 0$. Hơn nữa,

$$
\mathbf{B}(x+1, y) = \int_0^1 (1-t)^{x+y-1} \left( \frac{t}{1-t} \right)^x \, dt
$$

Do đó, bằng phép lấy tích phân từng phần,

$$
\mathbf{B}(x+1, y) = -\frac{(1-t)^{x+y}}{x+y} \left( \frac{t}{1-t} \right)^x \Bigg|_0^1
+ \frac{x}{x+y} \int_0^1 (1-t)^{x+y} \left( \frac{t}{1-t} \right)^{x-1} \frac{dt}{(1-t)^2} = \frac{x}{x+y} \mathbf{B}(x, y).
$$

Suy ra $f(x) = \mathbf{B}(x, y) \Gamma(x+y)$ thỏa mãn đẳng thức (1) của VII, p. 305
Hơn nữa, hàm này là lồi lôgarit, vì là tích của hai hàm lồi lôgarit. Cuối cùng, ta có $f(1) = \mathbf{B}(1, y) \Gamma(y+1)$, và $\mathbf{B}(1, y) = \int_0^1 (1-t)^{y-1} dt = 1/y$, do đó $f(1) = \frac{1}{y} \Gamma(y+1) = \Gamma(y)$. Vì thế hàm $f(x)/\Gamma(y)$ bằng $\Gamma(x)$ theo mệnh đề 1 của VII, p. 306, điều này chứng minh (18).

Bằng phép thay đổi biến $t = \frac{u}{u+1}$ công thức (18) trở thành

$$
\int_0^\infty \frac{t^{x-1}}{(1+t)^{x+y}} dt = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}
$$
(19)

và bằng phép thay đổi biến $t = \sin^2 \varphi$

$$
\int_0^{\pi/2} \sin^{2x-1} \varphi \cos^{2y-1} \varphi d\varphi = \frac{1}{2} \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$
(20)

Nếu đặt $x = y = \frac{1}{2}$ trong công thức cuối cùng này thì suy ra

$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$
(21)

do đó, theo (17),

$$
\int_0^\infty e^{-t^2} dt = \frac{1}{2} \sqrt{\pi}.
$$
(22)

Từ quan hệ (7) của VII, p. 307, ta có khai triển tiệm cận

$$
\begin{align*}
\Gamma(x) &= \frac{1}{x} \Gamma(x+1) \\
&= \frac{1}{x} + \Gamma'(1) + \frac{1}{2!} \Gamma''(1)x + \cdots + \frac{1}{n!} \Gamma^{(n)}(1)x^{n-1} + O(x^n)
\end{align*}
$$
(23)

cho $\Gamma(x)$, trên một lân cận của 0.

Tương tự, với mọi $y$ cố định và $> 0$ ta có thể viết

$$
\begin{align*}
\frac{1}{\Gamma(x+y)} &= \frac{1}{\Gamma(y)} + D \left( \frac{1}{\Gamma(y)} \right) x \\
&\quad + \frac{1}{2!} D^2 \left( \frac{1}{\Gamma(y)} \right) x^2 + \cdots + \frac{1}{n!} D^n \left( \frac{1}{\Gamma(y)} \right) x^n + O_1(x^{n+1})
\end{align*}
$$

và khi đó công thức (18) cho, với $y$ cố định, khai triển tiệm cận

$$
\mathbf{B}(x, y) = \frac{1}{x} + \left( \Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} \right)
+ \left( \frac{\Gamma''(1)}{2} - \Gamma'(1) \frac{\Gamma'(y)}{\Gamma(y)} + \frac{2\Gamma'^2(y) - \Gamma(y)\Gamma''(y)}{2\Gamma^2(y)} \right) x + O(x^2)
$$
trên một lân cận của $x = 0$.

Hơn nữa, với $x > 0$ và $y > 0$ ta có
$$
\mathbf{B}(x, y) = \int_0^1 \left( t^{x-1} + t^x \frac{(1-t)^{y-1} - 1}{t} \right) dt
= \frac{1}{x} + \int_0^1 t^x \frac{(1-t)^{y-1} - 1}{t} dt.
$$
Hàm $\varphi(t) = \frac{(1-t)^{y-1} - 1}{t}$ liên tục trên khoảng compắc $[0, 1]$; vì
$$
t^x = e^{x \log t} = 1 + x \log t + \frac{x^2}{2!} (\log t)^2 + \cdots + \frac{x^n}{n!} (\log t)^n + r_n(x, t)
$$
với $|r_n(x, t)| \leq \frac{x^{n+1}}{(n+1)!} |\log t|^{n+1}$ (vì $\log t \leq 0$ và $x > 0$), công thức (25) cho khai triển tiệm cận
$$
\mathbf{B}(x, y) = \frac{1}{x} + \int_0^1 \varphi(t) dt + x \int_0^1 \varphi(t) \log t \, dt + \cdots
+ \frac{x^n}{n!} \int_0^1 \varphi(t) (\log t)^n \, dt + O_2(x^{n+1})
$$
của $\mathbf{B}(x, y)$ trên một lân cận của 0.

Với $n = 1$ việc đồng nhất khai triển này với (24) đặc biệt cho
$$
\Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} = \int_0^1 \frac{(1-t)^{y-1} - 1}{t} dt.
$$

Hơn nữa, công thức (10) cho $\Gamma'(1) = \Gamma'(1)/\Gamma(1) = -\gamma$, do đó (*tích phân của Gauss*)
$$
\frac{\Gamma'(x)}{\Gamma(x)} + \gamma = \int_0^1 \frac{1 - (1-t)^{x-1}}{t} dt.
$$

### Bài tập {#fvr-vii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
