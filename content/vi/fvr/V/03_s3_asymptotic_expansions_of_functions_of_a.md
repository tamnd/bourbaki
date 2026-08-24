---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 3
section_title: ASYMPTOTIC EXPANSIONS OF FUNCTIONS OF A REAL VARIABLE
lang: vi
source: fvr-i-vii
pdf_pages: 0242-0251, 0275-0276
extraction: ocr
subsections:
    - "no": 1
      title: 'INTEGRATION OF COMPARISON RELATIONS: **I. WEAK RELATIONS**'
      page: 0
      pdf_page: 243
    - "no": 2
      title: 'APPLICATION: LOGARITHMIC CRITERIA FOR CONVERGENCE OF INTEGRALS'
      page: 0
      pdf_page: 244
    - "no": 3
      title: 'INTEGRATION OF COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 0
      pdf_page: 245
    - "no": 4
      title: DIFFERENTIATION OF COMPARISON RELATIONS
      page: 0
      pdf_page: 247
    - "no": 5
      title: PRINCIPAL PART OF A PRIMITIVE
      page: 0
      pdf_page: 248
    - "no": 6
      title: ASYMPTOTIC EXPANSION OF A PRIMITIVE
      page: 0
      pdf_page: 250
statements: 23
exercises: 7
content_sha256: ec5a441017a674212a2bcb470f307f9b84e7e048e420ab4362aa533b04a092eb
translated_from: content/en/fvr/V/03_s3_asymptotic_expansions_of_functions_of_a.md
source_content_sha256: 7521ac56cbf35b7f93d6d96d93a265b261fdc758a60860585fe831eb54a11bbe
translation_model: gpt-5.4, copied
translation_run: translate-vi-79767b08
glossary_version: 34
glossary_terms_sha256: abd9791b5bd3b421683073342f39fc00a93d173f646f9d51b306fffa58523aa7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. KHAI TRIỂN TIỆM CẬN CỦA CÁC HÀM CỦA MỘT BIẾN THỰC

Trong mục này ta sẽ chỉ xét trường hợp tập hợp $ E $ là một khoảng mở trong đường thẳng thực mở rộng $ \overline{\mathbf{R}} $, và $ \mathfrak{F} $ là một cơ sở của vết trên $ E $ của bộ lọc các lân cận của đầu mút trái hoặc phải $ \alpha $ của $ E $; hơn nữa, trên hết ta sẽ nghiên cứu các hàm thực (hữu hạn) được xác định trên một tập hợp thuộc $ \mathfrak{F} $ (phụ thuộc vào hàm đang xét).

Dùng một trong các phép đổi biến $ x' = -x,\ x' = \frac{1}{x-\alpha},\ x' = -\frac{1}{x-\alpha} $ khi cần, luôn luôn có thể rút gọn về trường hợp E là một khoảng có dạng ]$a, +\infty[$ sao cho $ \mathfrak{F} $ được tạo bởi các khoảng $[t, +\infty[$ với $ t > a $. Ta sẽ chủ yếu giới hạn ở trường hợp sau này, và để cho người đọc tự chuyển dịch phần lớn các mệnh đề mà ta thu được (nhờ các phép đổi biến ở trên), trừ một vài kết quả đặc biệt quan trọng.

Sẽ là thuận tiện nếu dùng một lối nói lạm dụng và gọi các tập hợp trong $ \mathfrak{F} $ là "các lân cận của $ +\infty $".

### 1. PHÉP LẤY TÍCH PHÂN CỦA CÁC QUAN HỆ SO SÁNH: **I. CÁC QUAN HỆ YẾU**

#### Mệnh đề 1 {#fvr-v-s3-prop-1 .statement}

*Cho $ \mathbf{f} $ là một hàm vectơ bị điều tiết, $ g $ là một hàm bị điều tiết $ \geqslant 0 $ trên một khoảng $[a, +\infty[$, sao cho $ \int_a^{+\infty} g(t)\,dt > 0 $. Quan hệ $ \mathbf{f} \preccurlyeq g $ khi $ x $ tiến tới $ +\infty $ suy ra $ \int_a^x \mathbf{f}(t)\,dt \preccurlyeq \int_a^x g(t)\,dt $. Nếu tích phân $ \int_a^{+\infty} g(t)\,dt $ hội tụ thì tích phân $ \int_a^{+\infty} \mathbf{f}(t)\,dt $ hội tụ tuyệt đối.*

Thật vậy, theo giả thiết tồn tại một $ b \geqslant a $ và một số $ c' > 0 $ sao cho
$$
\| \mathbf{f}(x) \| \leqslant c' g(x) \quad \text{với } x \geqslant b,
$$
do đó
$$
\left\| \int_b^x \mathbf{f}(t)\,dt \right\| \leqslant \int_b^x \| \mathbf{f}(t) \| \,dt \leqslant c' \int_b^x g(t)\,dt;
$$
hơn nữa, vì có thể giả sử $ b $ đủ lớn để $ \int_a^b g(t)\,dt > 0 $, nên tồn tại một $ c'' > 0 $ sao cho $ \left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leqslant c'' \int_a^b g(t)\,dt $; đặt $ c = \max(c', c'') $ thì do đó ta có
$$
\left\| \int_a^x \mathbf{f}(t)\,dt \right\| \leqslant c \int_a^x g(t)\,dt
$$
với mọi $ x \geqslant b $, do đó suy ra mệnh đề.

#### Hệ quả 1 {#fvr-v-s3-prop-1-cor-1 .statement}

*Nếu $ f $ và $ g $ là các hàm điều chỉnh và $ \geqslant 0 $ trên khoảng $[a, +\infty[$, và sao cho $ f \succcurlyeq g $, và nếu $ \int_a^{+\infty} g(t)\,dt = +\infty $, thì $ \int_a^{+\infty} f(t)\,dt = +\infty $.*

#### Hệ quả 2 {#fvr-v-s3-prop-1-cor-2 .statement}

*Nếu $ f $ và $ g $ là $ \geqslant 0 $ và không đồng nhất bằng không trên $[a, +\infty[$, và sao cho $ f \succeq g $, thì $ \int_a^x f(t)\,dt \succeq \int_a^x g(t)\,dt $.*

### 2. ỨNG DỤNG: CÁC TIÊU CHUẨN LÔGARIT CHO SỰ HỘI TỤ CỦA CÁC TÍCH PHÂN

Bằng cách chọn hàm g một cách thích hợp, người ta có thể suy ra các tiêu chuẩn để quyết định xem tích phân $ \int_a^{+\infty} f(t) \, dt $ của một hàm $ f \geq 0 $ là hội tụ hay vô hạn từ mệnh đề 1 của V, p. 228, và hệ quả 1 theo sau đó: chỉ cần chọn cho g một hàm mà nguyên hàm của nó đã biết. Đặc biệt, vì $ x^\mu $ có nguyên hàm là $ \frac{x^{\mu+1}}{\mu+1} $ khi $ \mu \neq -1 $, và $ \log x $ khi $ \mu = -1 $, ta có tiêu chuẩn sau đây:

#### Mệnh đề 2 ("tiêu chuẩn lôgarit cấp 0") {#fvr-v-s3-prop-2 .statement}

*Nếu f là một hàm điều hòa $ \geq 0 $ trên một khoảng $[a, +\infty[$; nếu $ f(x) \preccurlyeq x^\mu $ với một $ \mu < -1 $ thì tích phân $ \int_a^{+\infty} f(t) \, dt $ hội tụ; nếu $ f(x) \succcurlyeq x^\mu $ với một $ \mu \geq -1 $ thì tích phân $ \int_a^{+\infty} f(t) \, dt $ là vô hạn.*

Tiêu chuẩn này không có tính quyết định khi $ 1/x^{1+\alpha} \ll f(x) \ll 1/x $ với *mọi* số mũ $ \alpha > 0 $, như, chẳng hạn, khi $ f(x) = 1/x(\log x)^\mu $ ($ \mu > 0 $). Nhưng trong trường hợp sau cùng này, f có nguyên thủy $ \frac{1}{1-\mu} (\log x)^{1-\mu} $ nếu $ \mu \neq 1 $ và $ \log \log x $ khi $ \mu = 1 $. Do đó:

#### Mệnh đề 3 ("tiêu chuẩn lôgarit cấp 1") {#fvr-v-s3-prop-3 .statement}

*Nếu f là một hàm điều hòa $ \geq 0 $ trên một khoảng $[a, +\infty[$; nếu $ f(x) \preccurlyeq 1/x(\log x)^\mu $ với một $ \mu > 1 $ nào đó thì tích phân $ \int_a^{+\infty} f(t) \, dt $ hội tụ; nếu $ f(x) \succcurlyeq 1/x(\log x)^\mu $ với một $ \mu \leq 1 $ nào đó thì tích phân $ \int_a^{+\infty} f(t) \, dt $ là vô hạn.*

Nói chung, với mọi số nguyên $ n \geq 0 $, ta ký hiệu bởi $ l_n(x) $ hàm được xác định quy nạp (với x đủ lớn) bởi các hệ thức $ l_0(x) = x $, $ l_n(x) = \log(l_{n-1}(x)) $ với $ n \geq 1 $; ta nói rằng $ l_n(x) $ là *logarit lặp thứ* *n* *của x* (xem phụ lục). Ta kiểm tra ngay lập tức rằng $ \frac{1}{1-\mu} (l_n(x))^{1-\mu} $ là một nguyên hàm của

$$
\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}
$$

với $ \mu \neq 1 $, và $ l_{n+1}(x) $ là một nguyên thủy của $ \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) l_n(x)} $. Do đó:

#### Mệnh đề 4 ("tiêu chuẩn lôgarit cấp n") {#fvr-v-s3-prop-4 .statement}

*Cho f là một hàm bị điều chỉnh $ \geq 0 $ trên một khoảng $[a, +\infty[$; nếu, với một $ \mu > 1 $ nào đó, $ f(x) \preccurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu} $, thì tích phân $ \int_a^{+\infty} f(t) \, dt $ hội tụ; nếu $ f(x) \succcurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu} $ với một $ \mu \leq 1 $ nào đó, thì tích phân $ \int_a^{+\infty} f(t) \, dt $ là vô hạn.*

Như vậy, mỗi tiêu chuẩn lôgarit đều áp dụng được cho các hàm mà các tiêu chuẩn cấp thấp hơn không cho phép quyết định (*cf.* V, p. 264, exerc. 5 b) and V, p. 265, exerc. 8).

Vì tính hữu ích của nó, ta phát biểu lại tiêu chuẩn cấp 0 cho các tích phân $ \int_{\alpha}^{a} f(t) \, dt $ trong đó $ f $ bị điều hòa và $ \geq 0 $ trên một khoảng không compắc $ ]\alpha, a] $:

#### Mệnh đề 5 ("tiêu chuẩn lôgarit cấp 0") {#fvr-v-s3-prop-5 .statement}

*Nếu trên một lân cận của $ \alpha $ ta có $ f(x) \leq 1/(x-\alpha)^{\mu} $ với một $ \mu < 1 $ thì tích phân $ \int_{\alpha}^{a} f(t) \, dt $ hội tụ; nếu $ f(x) \geq 1/(x-\alpha)^{\mu} $ với một $ \mu \geq 1 $ thì tích phân $ \int_{\alpha}^{a} f(t) \, dt $ là vô hạn.*

Ta để độc giả tự phát biểu lại tương tự tiêu chuẩn lôgarit cấp $ n $.

Việc áp dụng các tiêu chuẩn lôgarit là ngay lập tức nếu người ta biết cách thu được *phần chính* của $ f $ đối với một thang so sánh chứa các hàm xuất hiện trong các tiêu chuẩn ấy: nếu $ f_1 $ là phần chính, thì tích phân $ \int_{\alpha}^{+\infty} f(t) \, dt $ hội tụ hoặc vô hạn đồng thời với $ \int_{\alpha}^{+\infty} f_1(t) \, dt $, và các tiêu chuẩn lôgarit áp dụng ngay lập tức cho tích phân sau này.

#### Ví dụ 1 {#fvr-v-s3-n2-exa-1 .statement}

Hàm $ t^p(1-t)^q $ không bị chặn trên $ ]0, 1[ $ khi $ p < 0 $ hoặc $ q < 0 $; theo tiêu chuẩn lôgarit cấp 0 áp dụng trên một lân cận của các điểm 0 và 1, tích phân $ \int_{0}^{1} t^p(1-t)^q \, dt $ hội tụ khi và chỉ khi $ p > -1 $ và $ q > -1 $. Khi đó, tích phân này được gọi là *tích phân Euler loại một* và được ký hiệu bởi $ \mathbf{B}(p+1, q+1) $ (*xem* VII, p. 312).

#### Ví dụ 2 {#fvr-v-s3-n2-exa-2 .statement}

Xét tích phân $ \int_{0}^{+\infty} t^{\lambda-1} e^{-t} \, dt $. Vì $ e^{-t} \sim 1 $ trên một lân cận của 0, phải có $ \lambda > 0 $ nếu tích phân này hội tụ; điều kiện này cũng là đủ vì trên một lân cận của $ +\infty $ ta có $ e^{-t} \ll t^{-\mu} $ với mọi $ \mu > 0 $. Khi $ x > 0 $ tích phân này được gọi là *tích phân Euler loại hai* và được ký hiệu bởi $ \Gamma(x) $ (*xem* VII, p. 311).

### 3. TÍCH PHÂN CÁC QUAN HỆ SO SÁNH: II. CÁC QUAN HỆ MẠNH

#### Mệnh đề 6 {#fvr-v-s3-prop-6 .statement}

*Cho $ \mathbf{f} $ là một hàm vectơ réglée, và $ g $ là một hàm réglée $ \geq 0 $ trên $ [a, +\infty[ $.*

1. *If the integral $ \int_{a}^{+\infty} g(t) \, dt $ converges then the relation $ \mathbf{f} \ll g $ (resp. $ \mathbf{f} \sim c g $, where $ c $ is constant) implies that $ \int_{x}^{+\infty} \mathbf{f}(t) \, dt \ll \int_{x}^{+\infty} g(t) \, dt $ (resp. $ \int_{x}^{+\infty} \mathbf{f}(t) \, dt \sim c \int_{x}^{+\infty} g(t) \, dt $).

2. *If the integral $ \int_{a}^{+\infty} g(t) \, dt $ is infinite then the relation $ \mathbf{f} \ll g $ (resp. $ \mathbf{f} \sim c g $) implies that*
$$
\int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \ll \int_{\beta}^{\gamma} g(t) \, dt \quad \text{(resp. } \int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \sim c \int_{\beta}^{\gamma} g(t) \, dt),
$$
*for any $ \alpha $ and $ \beta $ in $ [a, +\infty[ $*.

Chỉ cần chứng minh mệnh đề đối với quan hệ $ \mathbf{f} \ll g $ vì, nếu $ c \neq 0 $, quan hệ $ \mathbf{f} \sim c g $ là tương đương với $ \mathbf{f} - c g \ll g $.

Phần thứ nhất là một hệ quả ngay lập tức của định lý giá trị trung bình, vì nếu $ \| \mathbf{f}(x) \| \leq \varepsilon g(x) $ với $ x \geq x_0 $ thì suy ra rằng

$$
\left\| \int_{x}^{+\infty} \mathbf{f}(t) \, dt \right\| \leq \int_{x}^{+\infty} \| \mathbf{f}(t) \| \, dt \leq \varepsilon \int_{x}^{+\infty} g(t) \, dt \quad \text{với } x \geq x_0.
$$

Tiếp theo, giả sử rằng $ \int_{a}^{+\infty} g(t) \, dt = +\infty $. Nếu $ \| \mathbf{f}(x) \| \leq \varepsilon g(x) $ với $ x \geq x_0 \geq \max(\alpha, \beta) $, ta có

$$
\begin{align*}
\int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt &= \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \int_{x_0}^{x} \| \mathbf{f}(t) \| \, dt \\
&\leq \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \varepsilon \int_{x_0}^{x} g(t) \, dt \\
&= \varepsilon \int_{\beta}^{x} g(t) \, dt + \left( \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right).
\end{align*}
$$

Bây giờ tồn tại một $ x_1 \geq x_0 $ sao cho với mọi $ x \geq x_1 $

$$
\left| \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right| \leq \varepsilon \int_{\beta}^{x} g(t) \, dt
$$

do đó, với $ x \geq x_1 $

$$
\left\| \int_{\alpha}^{x} \mathbf{f}(t) \, dt \right\| \leq \int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt \leq 2\varepsilon \int_{\beta}^{x} g(t) \, dt
$$

điều này hoàn tất chứng minh, vì $ \varepsilon > 0 $ là tùy ý.

Nói cách khác, ta có thể lấy tích phân hai vế của một quan hệ mạnh $ \mathbf{f} \ll g $, $ \mathbf{f} \sim \mathbf{a}g $, khi $ g $ dương trên một khoảng $[a, +\infty[$, và quan hệ ấy vẫn còn đúng giữa các nguyên hàm của hai vế, miễn là chú ý lấy tích phân từ $ x $ đến $ +\infty $ nếu $ \int_{a}^{+\infty} g(t) \, dt $ hội tụ, và từ $ \alpha $ đến $ x $ (với mọi $ \alpha $ trong $[a, +\infty[$) trong trường hợp đối.

Chú ý rằng các mệnh đề 1 (V, p. 228) và 6 (V, p. 230) vẫn còn đúng khi $ \mathfrak{F} $ là một cơ sở của bộ lọc vết của các khoảng $[t, +\infty[$ (với $ t > a $) trên phần bù của một tập hợp đếm được (xem I, p. 15, định lý 2).

#### Ví dụ 1 {#fvr-v-s3-n3-exa-1 .statement}

Khi áp dụng mệnh đề 6 của V, p. 230, cho quan hệ $ 1/x \ll x^{\alpha-1} $ trong đó $ \alpha > 0 $, ta lại thu được quan hệ $ \log x \ll x^{\alpha} $ với mọi $ \alpha > 0 $, quan hệ này tương đương với quan hệ $ y^{1/\alpha} \ll e^y $ đã được chứng minh trong III, p. 105.

#### Ví dụ 2 {#fvr-v-s3-n3-exa-2 .statement}

Ta có $ \left( \frac{e^t}{x} \right)' = \frac{e^t}{x} \left( 1 - \frac{1}{x} \right) \sim e^t / x $; vì $ e^t / x $ tiến tới $ +\infty $ cùng với $ x $, từ mệnh đề 6 của V, p. 230, suy ra rằng $ \int_{1}^{x} \frac{e^t}{t} \, dt \sim e^x / x $.

#### Nhận xét {#fvr-v-s3-n3-rem-1 .statement}

Khi không giả sử $ g $ giữ nguyên $ \geq 0 $ trên một khoảng $[a, +\infty[$ (hoặc giữ nguyên $ \leq 0 $ trên một khoảng như vậy), và $ \int_{a}^{+\infty} g(t) \, dt $ không hội tụ, thì quan hệ $ f \sim g $ không nhất thiết kéo theo $ \int_{a}^{x} f(t) \, dt \sim \int_{a}^{x} g(t) \, dt $, như được chỉ ra bởi ví dụ trong đó $ g(x) = \sin x $ và $ f(x) = \left( 1 + \frac{\sin x}{x} \right) \sin x $; ở đây

$$
\int_{n\pi}^{(n+1)\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{(n+1)\pi} \int_{0}^{\pi} \sin^2 t \, dt \geq \frac{1}{2} \int_{n+1}^{n+2} \frac{dt}{t},
$$

do đó
$$
\int_{\pi}^{n\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{2} \int_2^{n+1} \frac{dt}{t}
$$
và tích phân $ \int_1^{+\infty} dt/t $ là vô hạn, mặc dù $ \int_{\frac{\pi}{2}}^x g(t) \, dt = -\cos x $ vẫn bị chặn (xem V, p. 260, bài tập 4).

### 4. PHÉP VI PHÂN CÁC QUAN HỆ SO SÁNH

Mệnh đề 1 (V, p. 228) và 6 (V, p. 230) không có mệnh đề đảo: sự tồn tại của một quan hệ so sánh $ f \preccurlyeq g,\ f \ll g,\ f \sim cg $ giữa hai hàm khả vi trên một lân cận của $ +\infty $ không kéo theo cùng quan hệ so sánh ấy giữa các đạo hàm của chúng, ngay cả đối với các hàm thực đơn điệu $ f $ và $ g $.

Ví dụ, hàm $ x^2 + x \sin x + \cos x $ là đơn điệu và tương đương với $ x^2 $, nhưng đạo hàm của nó $ x(2 + \cos x) $ không tương đương với $ 2x $.

Mặt khác, có thể suy ra các quan hệ so sánh khi giả thiết trước rằng các đạo hàm của các hàm được xét là so sánh được (V, p. 217). Nói chung, ta sẽ nói rằng hai hàm thực $ f $ và $ g $ xác định trên một khoảng $[a, +\infty[$ là so sánh được cấp $ k $ trên một lân cận của $ +\infty $ nếu, trên một lân cận của $ +\infty $, mỗi hàm đều có đạo hàm bậc $ k^{th} $ được điều chỉnh trừ tại một tập hợp đếm được các điểm, và nếu, trên lân cận này, $ f^{(k)} $ và $ g^{(k)} $ có dấu không đổi (trên tập hợp mà chúng được xác định) và là so sánh được.

Ta quy ước nói rằng hai hàm thực so sánh được (V, p. 217) là so sánh được cấp 0.

#### Mệnh đề 7 {#fvr-v-s3-prop-7 .statement}

Nếu hai hàm thực $ f,\ g $ là so sánh được cấp 1, thì chúng là so sánh được; hơn nữa, quan hệ $ f \ll g $ (resp. $ f \sim cg $, $ c $ hằng) suy ra $ f' \ll g' $ (resp. $ f' \sim cg' $) trừ khi $ g $ tương đương với một hằng khác không.

Bây giờ, vì $ f' $ và $ g' $ có dấu hằng trên một khoảng $[x_0, +\infty[$, nên cả $ f $ và $ g $ đều đơn điệu trên khoảng này, do đó tiến tới một giới hạn hữu hạn hoặc vô hạn khi $ x $ tiến tới $ +\infty $. Rõ ràng là $ f $ và $ g $ so sánh được khi $ x $ tiến tới $ +\infty $ nếu một trong các giới hạn ấy là hữu hạn và $ \neq 0 $, hoặc nếu một giới hạn là không còn giới hạn kia là vô hạn. Nếu cả $ f $ và $ g $ đều tiến tới 0 thì có thể viết $ f(x) = -\int_x^{+\infty} f'(t) \, dt,\ g(x) = -\int_x^{+\infty} g'(t) \, dt $; vì $ f' $ và $ g' $ so sánh được nên điều đó cũng đúng với $ f $ và $ g $ và quan hệ so sánh giữa $ f $ và $ g $ cũng chính là quan hệ giữa $ f' $ và $ g' $, theo mệnh đề 6 (V, p. 20). Tương tự, nếu $ f $ và $ g $ đều có một giới hạn vô hạn thì ta có $ f(x) = f(x_0) + \int_{x_0}^x f'(t) \, dt,\ g(x) = g(x_0) + \int_{x_0}^x g'(t) \, dt $; một lần nữa mệnh đề 6 (V, p. 230) cho thấy rằng $ f $ và $ g $ so sánh được và quan hệ so sánh giữa $ f $ và $ g $ cũng chính là quan hệ giữa $ f' $ và $ g' $. Để hoàn tất chứng minh, còn lại phải xét trường hợp $ g $ tiến tới $ \pm \infty $ còn $ f $ tiến tới một hằng: khi đó không thể có $ f' \succcurlyeq g' $, vì khi ấy có thể suy ra từ mệnh đề 1 (V, p. 218) rằng tích phân $ \int_{x_0}^{+\infty} g'(t) \, dt $ là hội tụ; vì $ f' $ và $ g' $ đã được giả thiết là so sánh được, nên phải có $ f' \ll g' $.

#### Hệ quả {#fvr-v-s3-n4-cor-1 .statement}

*Nếu hai hàm thực $ f, g $, là khả so sánh cấp $ k \geqslant 1 $, thì chúng khả so sánh cấp $ p $ với $ 0 \leqslant p \leqslant k $; hơn nữa, quan hệ $ f \ll g $ (tương ứng $ f \sim cg $) kéo theo $ f^{(k)} \ll g^{(k)} $ (tương ứng $ f^{(k)} \sim cg^{(k)} $) trừ khi một trong các đạo hàm $ g^{(p)} $ ($ 0 \leqslant p \leqslant k - 1 $) tương đương với một hằng $ \neq 0 $.*

Thật vậy, vì $ f^{(k)} $ và $ g^{(k)} $ có dấu không đổi trên một khoảng $[x_0, +\infty[$, suy ra $ f^{(k-1)} $ và $ g^{(k-1)} $ đơn điệu trên khoảng này, nên có dấu không đổi trên một lân cận của $ +\infty $; hơn nữa, mệnh đề 7 của V, p. 232, cho thấy rằng $ f^{(k-1)} $ và $ g^{(k-1)} $ là so sánh được, do đó hệ quả thu được bằng cách áp dụng mệnh đề 7 một cách đệ quy.

#### Nhận xét 1 {#fvr-v-s3-n4-rem-1 .statement}

Hạn chế đặt trên $ g $ trong mệnh đề 7 là cốt yếu. Ví dụ, ta có $ \frac{1}{x} \ll 1 + \frac{1}{x} $ mặc dù các đạo hàm của hai vế là tương đương; tương tự, $ 1 + \frac{1}{x} \sim 1 + \frac{1}{x^2} $, nhưng $ 1/x^2 \gg 2/x^3 $.

#### Nhận xét 2 {#fvr-v-s3-n4-rem-2 .statement}

Mặc dù $ f $ và $ g $ là so sánh được cấp $ k $ thì một hàm $ f_1 $ tương đương với $ f $ không nhất thiết so sánh được cấp $ k $ với $ g $; tuy nhiên điều đó sẽ đúng nếu giả thiết rằng $ f_1 $ so sánh được cấp $ k $ với $ f $ và không một đạo hàm nào trong các đạo hàm $ f^{(p)} $ ($ 0 \leqslant p \leqslant k - 1 $) tương đương với một hằng khác không.

#### Nhận xét 3 {#fvr-v-s3-n4-rem-3 .statement}

Nếu $ f $ và $ g $ so sánh được cấp $ k $ thì điều này không nhất thiết còn đúng đối với $ hf $ và $ hg $, ngay cả đối với một hàm đơn điệu $ h $ đơn giản như $ h(x) = x $ (V, p. 260, bài tập 3); tương tự, $ 1/f $ và $ 1/g $ cũng không nhất thiết so sánh được cấp $ k $ (V, p. 259, bài tập 1).

### 5. PHẦN CHÍNH CỦA MỘT NGUYÊN THỦY

Cho $ f $ là một hàm thực được điều chỉnh $ \neq 0 $ có dấu không đổi trên một khoảng $[a, +\infty[$; mệnh đề sau cho phép thu được phần chính của nguyên hàm $ \int_a^{+\infty} f(t)\,dt $ nếu $ \int_a^{+\infty} f(t)\,dt $ hội tụ trong một số trường hợp, và của nguyên hàm $ \int_a^x f(t)\,dt $ nếu $ \int_a^{+\infty} f(t)\,dt $ là vô hạn:

#### Mệnh đề 8 {#fvr-v-s3-prop-8 .statement}

*Đặt* $ F(x) = \int_x^{+\infty} f(t)\,dt $ *nếu* $ \int_a^{+\infty} f(t)\,dt $ *hội tụ*, *và* $ F(x) = \int_a^x f(t)\,dt $ *nếu* $ \int_a^{+\infty} f(t)\,dt $ *là vô hạn*. *Giả sử rằng* $ \log|f| $ *và* $ \log x $ *so sánh được cấp* 1.

1 *Nếu* $ f $ *có cấp hữu hạn* $ \mu \neq -1 $ *đối với* $ x $ *thì ta có*
$$
F(x) \sim \frac{1}{|\mu+1|} x f(x).
$$
(1)

2 *Nếu* $ f $ *có cấp vô hạn đối với* $ x $ *và nếu* $ f/f' $ *và* $ x $ *so sánh được với cấp* 1, *thì ta có*
$$
F(x) \sim \frac{(f(x))^2}{|f'(x)|}.
$$
(2)

Cần chú ý rằng giả thiết kéo theo $ f(x) $ có một cấp xác định đối với $ x $ (V, p. 219).

1 *Nếu* $ f $ *có cấp* $ \mu \neq 0 $ *đối với* $ x $ *thì ta có* $ \log|f| \sim \mu \log x $, *nên, vì* $ \log|f| $ *và* $ \log x $ *so sánh được và có cấp* 1, *theo mệnh đề 7 của V, p. 232 ta có* $ f'/f \sim $ μ/x, do đó $ x f' \sim \mu f $. Nếu $ \mu > -1 $ thì ta có $ f(x) \gg x^{\mu-\varepsilon} $ với mọi $ \varepsilon > 0 $, và vì thế (V, p. 229, mệnh đề 2) tích phân $ \int_a^{+\infty} f(t)\,dt $ là vô hạn. Ta có thể viết $ F(x) = \int_a^x f(t)\,dt = x f(x) - af(a) - \int_a^x t f'(t)\,dt $, do đó lại có
$$
\int_a^x (f(t) + t f'(t))\,dt = x f(x) - af(a);
$$
vì $ \mu \neq -1 $ nên ta có $ f(x) + x f'(x) \sim (\mu + 1) f(x) $, do đó (V, p. 230, mệnh đề 6)
$$
\int_a^x (f(t) + t f'(t))\,dt \sim (\mu + 1) F(x),
$$
điều này chứng minh (1) trong trường hợp này. Nếu $ \mu = 0 $ thì tương tự ta có $ x f'(x) \ll f(x) $, điều này lại cho $ f(x) + x f'(x) \sim f(x) $. Ta cũng lập luận tương tự khi $ \mu < -1 $, trong trường hợp $ \int_a^{+\infty} f(t)\,dt $ hội tụ.

2' Nếu $ f $ có cấp $ +\infty $ đối với $ x $ thì ta có $ \log |f| \gg \log x $, nên (V, p. 232, mệnh đề 7) $ f'/f \gg 1/x $, hay còn viết, đặt $ g(x) = f(x)/f'(x) $, thì $ g(x) \ll x $; hơn nữa, vì $ f(x) \gg x^\alpha $ với mọi $ \alpha > 0 $ nên tích phân $ \int_a^{+\infty} f(t)\,dt $ là vô hạn. Ta có thể viết
$$
F(x) = \int_a^x f(t)\,dt = \int_a^x g(t) f'(t)\,dt = g(x) f(x) - g(a) f(a) - \int_a^x f(t) g'(t)\,dt;
$$
vì $ g $ và $ x $ so sánh được với nhau ở cấp 1, từ quan hệ $ g(x) \ll x $ ta suy ra được (V, p. 232, mệnh đề 7) rằng $ g'(x) \ll 1 $, do đó $ f g' \ll f $, và do đó (V, p. 230, mệnh đề 6)
$$
\int_a^x f(t) g'(t)\,dt \ll F(x),
$$
điều này thiết lập quan hệ (2). Chứng minh là tương tự khi $ f $ có cấp $ -\infty $ đối với $ x $, trong trường hợp $ \int_a^{+\infty} f(t)\,dt $ hội tụ.

Cho $ \mathcal{E} $ là một thang so sánh (đối với $ x $ tiến tới $ +\infty $) được tạo thành từ các hàm thực khác không có dấu không đổi trên một lân cận của $ +\infty $, sao cho $ x \in \mathcal{E} $ và sao cho tích và thương của hai hàm thuộc $ \mathcal{E} $ lại thuộc $ \mathcal{E} $ (V, p. 221 và p. 224). Nếu một hàm được điều chỉnh $ f $ có dấu không đổi trên một lân cận của $ +\infty $ có phần chính $ c g $ đối với $ \mathcal{E} $, thì $ \int_x^{+\infty} f(t)\,dt $ (tương ứng $ \int_a^x f(t)\,dt $ tùy theo trường hợp) sẽ tương đương với $ c \int_x^{+\infty} g(t)\,dt $ (tương ứng $ c \int_a^x g(t)\,dt $); nếu hàm $ g $ thỏa mãn các giả thiết của mệnh đề 8 của V, p. 233, và nếu (khi công thức (2) của V, p. 233, áp dụng được) ta biết một phần chính của $ g' $ đối với $ \mathcal{E} $, thì như vậy ta sẽ có một phần chính của $ \int_x^{+\infty} f(t)\,dt $ (tương ứng $ \int_a^x f(t)\,dt $) đối với $ \mathcal{E} $.

#### Ví dụ 1 {#fvr-v-s3-n5-exa-1 .statement}

Hàm $ 1/\log x $ có cấp 0 đối với $ x $ và thỏa mãn các điều kiện của mệnh đề 8 của V, p. 233; do đó
$$
\int_a^x \frac{dt}{\log t} \sim \frac{x}{\log x}.
$$
2) Hàm $ e^{t^2} $ có cấp $ +\infty $ đối với $ x $ và thỏa mãn các điều kiện của mệnh đề 8, nên
$$
\int_a^x e^{t^2}\,dt \sim \frac{1}{2x}\,e^{x^2}.
$$

Trong phụ lục (V, p. 252) chúng ta sẽ định nghĩa một tập hợp các hàm mà đối với chúng mệnh đề 7 và mệnh đề 8 luôn áp dụng được.

#### Nhận xét {#fvr-v-s3-n5-rem-1 .statement}

Mệnh đề 8 không áp dụng trực tiếp được cho một hàm $ f $ có cấp $-1$ đối với $ x $. Nhưng khi đó có thể viết $ f(x) = f_1(x)/x $, với $ f_1 $ có cấp 0 đối với $ x $. Chẳng hạn, giả sử rằng $ \int_a^{+\infty} f(t)\,dt $ là vô hạn; khi đó

$$
F(x) = \int_a^x f(t)\,dt = \int_a^x \frac{1}{t} f_1(t)\,dt = \int_{\log a}^{\log x} f_1(e^u)\,du.
$$

Nếu hàm $ f_1(e^t) $ thỏa mãn các giả thiết của mệnh đề 8 và có một cấp $ \neq -1 $ đối với $ y $ (nghĩa là, nếu $ f_1(x) $ có một cấp $ \neq -1 $ đối với $ \log x $) thì các công thức (1) và (2) lại cho phép ta thu được một phần chính của $ F(x) $. Ví dụ, đặt $ f(x) = \frac{\exp(\sqrt{\log x})}{x \log x} $; vì $ \exp(\sqrt{\log x}) $ có cấp 0 đối với $ x $, nên $ f $ có cấp $-1$; ở đây ta có $ f_1(e^t) = e^{\sqrt{t}}/y $, và hàm này có cấp $ +\infty $ đối với $ y $; mệnh đề 8 áp dụng được và cho $ \int_a^x e^{\sqrt{u}}/u\,du \sim 2e^{\sqrt{y}}/\sqrt{y} $: khi quay trở lại biến $ x $ ta có $ \int_a^x \frac{\exp(\sqrt{\log t})}{t \log t}\,dt \sim \frac{2\exp(\sqrt{\log x})}{\sqrt{\log x}} $.

### 6. KHAI TRIỂN TIỆM CẬN CỦA MỘT NGUYÊN HÀM

Cho $ \mathcal{E} $ là một thang so sánh trên một lân cận của $ +\infty $ được tạo thành từ các hàm thực $ \neq 0 $ có dấu không đổi trên một lân cận của $ +\infty $; cho $ \mathbf{f} $ là một hàm vectơ điều hòa xác định trên một khoảng $[a,\,+\infty[$, nhận giá trị trong một không gian định chuẩn đầy đủ $ E $, có một khai triển tiệm cận

$$
\mathbf{f} = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda + \mathbf{r}_\alpha
$$

đến cấp chính xác $ g_\alpha $ đối với $ \mathcal{E} $. Giả sử thêm rằng mọi nguyên hàm $ \int_a^x g(t)\,dt $ của một hàm $ g \in \mathcal{E} $ đều có một khai triển tiệm cận đối với $ \mathcal{E} $. Trong những điều kiện đó, ta sẽ thấy rằng có thể thu được một khai triển tiệm cận của $ F(x) = \int_a^x \mathbf{f}(t)\,dt $ đối với $ \mathcal{E} $. Ta phân biệt hai trường hợp:

1. $ \int_a^{+\infty} g_\alpha(t)\,dt $ is infinite; then one has $ \int_a^x \mathbf{r}_\alpha(t)\,dt \ll \int_a^x g_\alpha(t)\,dt $ (V, p. 230, prop. 6); by hypothesis one can obtain an asymptotic expansion of $ \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt $ to a certain precision $ g_\rho $ (V, p. 222); if $ c g_\sigma $ is the principal part of $ \int_a^x g_\alpha(t)\,dt $ one will thus have an asymptotic expansion of $ \int_a^x \mathbf{f}(t)\,dt $ to precision $ g_{\min(\rho,\sigma)} $, with all the terms having indefinitely increasing norms.

2. $ \int_a^{+\infty} g_\alpha(t)\,dt $ converges; let $ \beta $ then be the smallest of the indices $ \lambda \leq \alpha $ such that $ \mathbf{a}_\lambda \neq 0 $ and such that $ \int_a^{+\infty} g_\lambda(t)\,dt $ converges; the integral

$$
C = \int_a^{+\infty} \left( \mathbf{f}(t) - \sum_{\lambda < \beta} \mathbf{a}_\lambda g_\lambda(t) \right) dt
$$

khi đó là hội tụ, và ta có thể viết

$$
F(x) = \sum_{\lambda < \beta} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt + C - \sum_{\beta \leq \lambda \leq \alpha} \mathbf{a}_\lambda \int_a^{+\infty} g_\lambda(t)\,dt - \int_a^{+\infty} \mathbf{r}_\alpha(t)\,dt.
$$

Khi đó $ \int_a^{+\infty} r_\alpha(t) \, dt \ll \int_1^{+\infty} g_\alpha(t) \, dt $; nếu $ c g_\sigma $ là phần chính của $ \int_1^{+\infty} g_\alpha(t) \, dt $, và nếu ta có một khai triển tiệm cận của

$$
\sum_{\lambda < \beta} a_\lambda \int_a^\lambda g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda \leq \alpha} a_\lambda \int_\lambda^{+\infty} g_\lambda(t) \, dt
$$

đến cấp chính xác $ g_\rho $, thì do đó ta sẽ có một khai triển tiệm cận của $ F $ đến cấp chính xác $ g_{\min(\rho, \sigma)} $.

Vậy tất cả quy về việc tìm các khai triển tiệm cận đối với $ \mathcal{E} $ của *nguyên hàm của các hàm thuộc* $ \mathcal{E} $. Ta đã thấy rằng, với một số giả thiết nào đó trên $ \mathcal{E} $, mệnh đề 8 của V, p. 233 cho phần chính của một nguyên hàm như vậy. Hơn nữa, chứng minh của mệnh đề 8 cho biểu thức của hiệu giữa hai vế của công thức (1) (tương ứng (2)) của V, p. 233, dưới dạng một nguyên hàm của hàm $ \frac{1}{|\mu + 1|} (x f'(x) + f(x)) - f(x) $ (tương ứng $ f(x) g'(x) $ với $ g = f/f' $); khi lập phần chính của nguyên hàm mới này, như một khai triển tiệm cận của vế phải của (1) (tương ứng của (2)), ta thu được vế phải của khai triển cần tìm (xem V, p. 247-255).

#### Ví dụ 1 {#fvr-v-s3-n6-exa-1 .statement}

Cho $ f(x) = 1/\log x $ ($ x > 1 $); ta đã thấy rằng $ \int_a^\lambda dt / \log t \sim x / \log x $, và hiệu $ \int_a^\lambda \frac{dt}{\log t} - \frac{\lambda}{\log \lambda} $ là một nguyên thủy của $ 1/(\log x)^2 $; lại có thể áp dụng mệnh đề 8 cho hàm này, do đó thu được $ \int_a^\lambda dt / (\log t)^2 \sim x / (\log x)^2 $. Bằng phép truy hồi, như vậy ta thu được khai triển

$$
\int_a^\lambda \frac{dt}{\log t} = \frac{x}{\log x} + \frac{x}{(\log x)^2}
+ \frac{2x}{(\log x)^3} + \cdots + (n-1)! \frac{x}{(\log x)^n} + o \left( \frac{x}{(\log x)^n} \right).
$$

Chú ý rằng, bất kể $ n $, mọi hạng của khai triển này đều tiến tới $ +\infty $ cùng với $ x $.

#### Ví dụ 2 {#fvr-v-s3-n6-exa-2 .statement}

Cho $ f(x) = \frac{e^x}{x^2 + 1} $; có thể viết $ f(x) = \frac{e^x}{x^2} - \frac{e^x}{x^4} + o_1 \left( \frac{e^x}{x^4} \right) $. Mệnh đề 8 cho các khai triển

$$
\int_a^\lambda \frac{e^t}{t^2} \, dt = \frac{e^x}{x^2} + \frac{2e^x}{x^3} + \frac{6e^x}{x^4} + o_2 \left( \frac{e^x}{x^4} \right), \quad \int_a^\lambda \frac{e^t}{t^4} \, dt = \frac{e^x}{x^4} + o_3 \left( \frac{e^x}{x^4} \right)
$$

do đó, khi cộng lại,

$$
\int_a^\lambda \frac{e^t}{t^2 + 1} \, dt = \frac{e^x}{x^2} + 2 \frac{e^x}{x^3} + 5 \frac{e^x}{x^4} + o_4 \left( \frac{e^x}{x^4} \right).
$$

### Bài tập {#fvr-v-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
