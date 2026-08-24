---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 2
section_title: INTEGRALS OVER NON-COMPACT INTERVALS
lang: vi
source: fvr-i-vii
pdf_pages: 0077-0083, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 77
    - "no": 2
      title: INTEGRALS OF POSITIVE FUNCTIONS OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 81
    - "no": 3
      title: ABSOLUTELY CONVERGENT INTEGRALS
      page: 0
      pdf_page: 82
statements: 9
exercises: 9
content_sha256: f55f6dcb90251edcec29938b030d946067914782480d891d331fefcb3b20f0e1
translated_from: content/en/fvr/II/02_s2_integrals_over_non_compact_intervals.md
source_content_sha256: 64275a842838d2080c7899bc5b116bdeafc42c93c4e521c8d9b045ecfe092f1d
translation_model: gpt-5.4, copied
translation_run: translate-vi-7cdd6941
glossary_version: 34
glossary_terms_sha256: aa74de58227d7e48d5b37b512e4de037a8e26d4eff9cc73c73db8bc0a2550018
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. TÍCH PHÂN TRÊN CÁC KHOẢNG KHÔNG COMPACT

### 1. ĐỊNH NGHĨA TÍCH PHÂN TRÊN MỘT KHOẢNG KHÔNG COMPACT

Cho I là một khoảng compact $[a,\ b]$ của *trục mở rộng* $\overline{\mathbf{R}}$ ($a$ và $b$ có thể vô hạn); cho $f$ là một hàm được xác định trên $[a,\ b[$, nhận giá trị trong một không gian định chuẩn đầy đủ E trên $\mathbf{R}$. Khái quát hóa định nghĩa 1 của II, p. 51, ta sẽ nói rằng một hàm $g$, được xác định trên $[a,\ b]$ với giá trị trong E, là một *nguyên hàm* của $f$ nếu nó liên tục trên $[a,\ b]$ (và đặc biệt tại các đầu mút $a$ và $b$) và có một đạo hàm bằng $f(x)$ tại mọi điểm của phần bù trong $[a,\ b[$ của một tập con đếm được của khoảng này.

Chúng tôi sẽ tự giới hạn vào trường hợp sau: tồn tại một dãy hữu hạn tăng ngặt $(c_i)_{0 \leq i \leq n}$ các điểm của $I = [a,\ b]$, sao cho $c_0 = a,\ c_n = b$, và sao cho $f$ là *được điều chỉnh* trên mỗi khoảng mở $[c_i,\ c_{i+1}[$. Mặc dù không nhất thiết được điều chỉnh trên mọi khoảng mở chứa ít nhất một điểm $c_i$ nằm trong nội bộ của $I$; một hàm như vậy sẽ được gọi là *được điều chỉnh từng khúc* trên $[a,\ b[$. Chúng tôi nhận xét rằng một hàm được điều chỉnh trên $[a,\ b[$ là được điều chỉnh từng khúc (lấy $n = 1$ trong định nghĩa trước đó).

Nếu $f$ có một nguyên hàm $g$ (theo nghĩa đã được nói chính xác ở trên), và nếu $c$ là một điểm của khoảng $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$, thì theo giả thiết, với mỗi $x$ trong khoảng này, ta có $g(x) - g(c) = \int_c^x f(t)\,dt$; vì $g$ liên tục trên $I$ theo giả thiết, suy ra $\int_c^x f(t)\,dt$ tiến tới một giới hạn trong $E$ khi $x$ tiến tới $c_i$ từ bên phải và khi $x$ tiến tới $c_{i+1}$ từ bên trái. Ngược lại, giả sử rằng các điều kiện này được thỏa mãn với mọi $t$, và gọi $g_i$ là một nguyên hàm của $f$ trên khoảng $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$; ta chú ý ngay lập tức rằng hàm $g$, được xác định trên phần bù trong $I$ của tập hợp các $c_i$, bởi điều kiện nó bằng $g_i(x) + \sum_{k=1}^i (g_{k-1}(c_k-) - g_k(c_k+))$ trên $[c_i,\ c_{i+1}[$ với $0 \leq i \leq n - 1$, là liên tục tại mọi điểm của $I$ phân biệt với các $c_i$ và có một giới hạn tại mỗi điểm đó; do đó nó có thể được kéo dài bằng tính liên tục tới mỗi điểm ấy, và hàm được kéo dài hiển nhiên là một nguyên hàm của $f$ trên $I$. Hơn nữa, rõ ràng rằng mọi nguyên hàm khác của $f$ đều có dạng $g + a$ ($a$ là một phần tử của $E$).

#### Định nghĩa 1 {#fvr-ii-s2-def-1 .statement}

*Người ta nói rằng một hàm vectơ* $f$, *từng khúc điều hòa trên một khoảng* $[a,\ b[$ *của* $\overline{\mathbf{R}}$, *có một nguyên trên khoảng này nếu* $f$ *có một nguyên hàm trên* $[a,\ b[$*; nếu* $g$ *là một trong các nguyên hàm của* $f$ *trên* $[a,\ b[$*, và nếu* $x_0$ *và* $x$ *là hai điểm bất kỳ của* $[a,\ b[$*, thì người ta gọi phần tử* $g(x) - g(x_0)$ *là nguyên của* $f$ *từ* $x_0$ *đến* $x$, *và ký hiệu nó bởi* $\int_{x_0}^x f(t)\,dt$.

Khái niệm này rõ ràng phù hợp với khái niệm đã được định nghĩa khi khoảng $[x_0,\ x]$ không chứa điểm nào trong các điểm $c_i$.

Các nhận xét đứng trước định nghĩa 1 cho thấy rằng để $f$ có một tích phân trên $[a,\ b[$ thì điều kiện cần và đủ là hạn chế của nó trên mỗi khoảng $[c_i,\ c_{i+1}[$ đều thừa nhận một tích phân trên khoảng này. Nói cách khác, ta quy về trường hợp $f$ là điều hòa trên một khoảng *không compắc* $I \subset \mathbf{R}$, có các đầu mút $a,\ b$ ($a < b$), và trong đó: 1 hoặc ít nhất một trong các số $a,\ b$ là vô hạn; 2 hoặc $f$ không điều hòa trên một khoảng compắc chứa ít nhất một trong các điểm $a,\ b$ (hai giả thuyết này không loại trừ lẫn nhau). Để $f$ có một tích phân trên $I$ thì điều kiện cần và đủ là tích phân $\int_a^x f(t)\,dt$ tiến tới một giới hạn khi điểm $(x,\ y)$ tiến tới $(a,\ b) \in \overline{\mathbf{R}}^2$ đồng thời vẫn thuộc $I \times I$: và giới hạn này chính là $\int_a^b f(t)\,dt$ theo định nghĩa 1. Do một sự lạm dụng ngôn ngữ, thay vì nói rằng $f$ có một tích phân trên $I$, người ta nói rằng tích phân $\int_a^b f(t)\,dt$ là *hội tụ* (hoặc *hội tụ*).

#### Ví dụ {#fvr-ii-s2-n1-exa-1 .statement}

i) Tích phân $\int_1^{+\infty} dt/t^2$ hội tụ và bằng 1, vì
$$
\int_1^x \frac{dt}{t^2} = 1 - \frac{1}{x}.
$$

2) Tích phân $ \int_0^1 dt / \sqrt{t} $ hội tụ và bằng 2, vì
$$
\int_1^x \frac{dt}{\sqrt{t}} = 2(1 - \sqrt{x}) \quad \text{với} \quad x > 0.
$$

3) Cho $ (\mathbf{u}_n)_{n \geq 1} $ là một dãy vô hạn các điểm của E, và gọi $ \mathbf{f} $ là hàm bậc thang được xác định trên khoảng $ [1, +\infty[ $ bởi các điều kiện: $ \mathbf{f}(x) = \mathbf{u}_n $ với $ n \leq x < n+1 $. Khi đó, để tích phân $ \int_1^{+\infty} \mathbf{f}(t)\,dt $ hội tụ thì điều kiện cần và đủ là chuỗi có số hạng tổng quát $ \mathbf{u}_n $ *hội tụ* trong E; thật vậy, ta có
$$
\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p,
$$
nên điều kiện là cần; ngược lại, nếu chuỗi có số hạng tổng quát $ \mathbf{u}_n $ hội tụ trong E, thì $ \lim_{n \to \infty} \mathbf{u}_n = 0 $; bây giờ, nếu $ n \leq x \leq n+1 $, ta có $ \int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p + \mathbf{u}_n(x-n) $. do đó tích phân này có giới hạn $ \sum_{n=1}^{\infty} \mathbf{u}_n $ khi $ x $ tiến tới $ +\infty $.

Điều đó là ngay lập tức rằng nếu một hàm từng khúc bị chặn $ \mathbf{f} $ thừa nhận một nguyên trên I thì các công thức (4) đến (9) của II, p. 59 vẫn còn đúng. Tương tự, công thức (10) của II, p. 59 được mở rộng theo cách sau: giả sử $ \mathbf{f} $ và $ \mathbf{g} $ là các nguyên hàm của các hàm bị chặn $ \mathbf{f}' $ và $ \mathbf{g}' $ trên $ ]a,\ b[ $, và ký hiệu $ [\mathbf{f}.\mathbf{g}]|_a^b $ là giới hạn (nếu nó tồn tại) của $ [\mathbf{f}.\mathbf{g}]|_x^y $ khi $ (x,\ y) $ tiến tới $ (a,\ b) $ (với $ a < x \leq y < b $); khi đó, nếu hai trong ba biểu thức $ [\mathbf{f}.\mathbf{g}]|_a^b $, $ \int_a^b [\mathbf{f}(t).\mathbf{g}'(t)]\,dt $, và $ \int_a^b [\mathbf{f}'(t).\mathbf{g}(t)]\,dt $ có nghĩa, thì biểu thức thứ ba cũng có nghĩa, và công thức (10) của II, p. 59 là đúng.

Sau cùng, cho $ f $ là một hàm thực được xác định và liên tục trên $ I = ]a,\ b[ $, và là một nguyên hàm của một hàm điều chỉnh $ f' $ trên $ ]a,\ b[ $; mặt khác, cho $ g $ là một hàm vectơ liên tục trên một khoảng mở J chứa $ f(I) $; nếu hàm $ g(f(x))f'(x) $ khả tích trên I, và nếu $ f $ tiến tới một giới hạn (hữu hạn hay không) tại các điểm $ a $ và $ b $, thì $ g $ khả tích từ $ f(a+) $ đến $ f(b-) $, và ta có công thức
$$
\int_a^b g(f(t))f'(t)\,dt = \int_{f(a+)}^{f(b-)} g(u)\,du.
$$
Thật vậy, nếu $ (x,\ y) $ tiến tới $ (a,\ b) $, thì $ (f(x),\ f(y)) $ tiến tới $ (f(a+),\ f(b-)) $ theo giả thiết; chỉ cần áp dụng công thức (12) của II, p. 60 giữa $ x $ và $ y $, rồi cho qua giới hạn để thu được (1).

Cho một hàm điều hòa $ \mathbf{f} $ trên một khoảng không compact $ I \subset \mathbf{R} $, với các đầu mút $ a $ và $ b $ ($ a < b $), điều kiện để $ \mathbf{f} $ có một tích phân trên I có thể được trình bày theo cách sau. Các khoảng compact $ J \subset I $ tạo thành một *tập có hướng* $ \mathcal{K}(I) $ đối với quan hệ $ \subset ^1 $, vì nếu $[ \alpha , \beta ]$ và $[ \gamma , \delta ]$ là hai khoảng compact được chứa trong $ I $, và nếu đặt $ \lambda = \min(\alpha, \gamma) $, $ \mu = \max(\beta, \delta) $, thì khoảng $[ \lambda , \mu ]$ được chứa trong $ I $ và chứa hai khoảng đang xét. Với mỗi khoảng compact $ J = [ \alpha , \beta ] $ được chứa trong $ I $, ta đặt

$$
\int_J f(t) \, dt = \int_\alpha^\beta f(t) \, dt;
$$

để $ f $ chấp nhận được một tích phân trên $ I $ thì điều kiện cần và đủ là ánh xạ $ J \mapsto \int_J f(t) \, dt $ có một giới hạn đối với tập có hướng $ \mathfrak{K}(I) $; khi đó giới hạn này là tích phân $ \int_a^b f(t) \, dt $, mà ta lại ký hiệu bởi $ \int_I f(t) \, dt $.

#### Mệnh đề 1 (Tiêu chuẩn Cauchy cho các tích phân) {#fvr-ii-s2-prop-1 .statement}

*Cho $ f $ là một hàm điều chỉnh trên một khoảng $ I \subset \mathbf{R} $ có các đầu mút $ a $ và $ b $ ($ a < b $). Để tích phân $ \int_a^b f(t) \, dt $ tồn tại, điều kiện cần và đủ là với mọi $ \varepsilon > 0 $, tồn tại một đoạn compact $ J_0 = [\alpha, \beta] $ được chứa trong $ I $, sao cho với mọi đoạn compact $ K = [x, y] $ được chứa trong $ I $ và không có điểm trong nào chung với $ J_0 $, ta có $ \| \int_K f(t) \, dt \| \leq \varepsilon $.*

Thật vậy, vì $ E $ là đầy đủ nên tiêu chuẩn Cauchy cho thấy rằng để tích phân $ \int_I f(t) \, dt $ hội tụ thì điều kiện cần và đủ là với mọi $ \varepsilon > 0 $ tồn tại một khoảng compact $ J_0 = [\alpha, \beta] $ sao cho với mọi khoảng compact $ J $ thỏa mãn $ J_0 \subset J \subset I $ ta có $ \| \int_J f(t) \, dt - \int_{J_0} f(t) \, dt \| \leq \varepsilon $. Mệnh đề sẽ suy ra từ bổ đề sau:

*Bổ đề. Cho $ J_0 = [\alpha, \beta] $ là một khoảng compact được chứa trong $ I $. Để có $ \| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \| \leq \varepsilon $ với mọi cặp khoảng compact $ J, J' $ được chứa trong $ I $ và chứa $ J' $ thì cần phải có $ \| \int_K f(t) \, dt \| \leq \varepsilon $, và đủ là có $ \| \int_K f(t) \, dt \| \leq \varepsilon / 2 $, với mọi khoảng compact $ K $ được chứa trong $ I $ và không có điểm trong nào chung với $ J_0 $.*

Thật vậy, nếu với $ J_0 \subset J \subset I $ và $ J_0 \subset J' \subset I $, ta có

$$
\left\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \right\| \leq \varepsilon
$$

đặc biệt ta thấy rằng, với $ x \leq y \leq \alpha $, hoặc với $ \beta \leq x \leq y $ ($ x $ và $ y $ trong $ I $), ta có $ \| \int_x^y f(t) \, dt \| \leq \varepsilon $. Ngược lại, nếu $ \| \int_K f(t) \, dt \| \leq \varepsilon / 2 $ với mọi đoạn compắc $ K \subset I $ sao cho $ K \cap J_0 = \emptyset $, và nếu $ J = [x, y] $, $ J' = [z, t] $ là hai đoạn compắc được chứa trong $ I $ và chứa $ J_0 $, ta có

1 Nhắc lại (*Lý thuyết Tập hợp*, III, p. 144) rằng một tập hợp $ \mathfrak{F} $ các tập con của $ I $ là *có hướng đối với quan hệ* $ \subset $ nếu, với mọi $ X \in \mathfrak{F} $, $ Y \in \mathfrak{F} $, tồn tại $ Z \in \mathfrak{F} $ sao cho $ X \subset Z $ và $ Y \subset Z $. Nếu $ S(X) $ ký hiệu tập con của $ \mathfrak{F} $ gồm các $ U \in \mathfrak{F} $ sao cho $ U \supset X $, thì các $ S(X) $ lập thành một cơ sở của một bộ lọc trên $ \mathfrak{F} $, gọi là *bộ lọc các thiết diện* của $ \mathfrak{F} $; giới hạn (nếu tồn tại) của một ánh xạ $ f $ từ $ \mathfrak{F} $ vào một không gian tôpô, đối với bộ lọc các thiết diện của $ \mathfrak{F} $, được gọi là *giới hạn của f đối với tập hợp có hướng* $ \mathfrak{F} $ (*x. Gen. Top.*, I, p. 70 và *Gen. Top.*, IV, p. 348).

$$
\left\| \int_J f(t)\,dt - \int_{J'} f(t)\,dt \right\| = \left\| \int_x^z f(t)\,dt + \int_t^y f(t)\,dt \right\| \leq \varepsilon,
$$
vì
$$
x \leq \alpha \leq \beta \leq y \quad \text{và} \quad z \leq \alpha \leq \beta \leq t.
$$

#### Ví dụ {#fvr-ii-s2-n1-exa-2 .statement}

Nếu khoảng I là *bị chặn*, và nếu $ f $ *bị chặn* trên I, thì tích phân $ \int_I f(t)\,dt $ luôn luôn tồn tại, vì, theo định lý giá trị trung bình, ta có, với $ y \leq \alpha \leq \beta \leq z $,
$$
\left\| \int_y^\alpha f(t)\,dt \right\| \leq (\alpha - a) \sup_{t \in I} \|f(v)\| , \quad \left\| \int_\beta^z f(t)\,dt \right\| \leq (b - \beta) \sup_{t \in I} \|f(x)\|
$$
và chỉ cần lấy $ \alpha - a $ và $ b - \beta $ đủ nhỏ để tiêu chuẩn Cauchy được thỏa mãn.

Có thể chú ý rằng trong trường hợp này một nguyên hàm của $ f $ trên I không nhất thiết có đạo hàm phải (tương ứng, trái) tại đầu mút trái (tương ứng, đầu mút phải) của I (khi số này là hữu hạn), trái với trường hợp I là compắc và $ f $ là hàm được điều chỉnh trên I (*cf.* II, p. 33, exerc. 1).

### 2. TÍCH PHÂN CỦA CÁC HÀM DƯƠNG TRÊN MỘT KHOẢNG KHÔNG COMPACT

#### Mệnh đề 2 {#fvr-ii-s2-prop-2 .statement}

*Cho $ f $ là một hàm điều chỉnh thực $ \geq 0 $ trên một khoảng $ I \subset \mathbf{R} $ có các đầu mút $ a $ và $ b $ ($ a < b $). Để tích phân $ \int_a^b f(t)\,dt $ tồn tại thì điều kiện cần và đủ là tập hợp các số $ \int_J f(t)\,dt $ bị chặn trên khi J chạy qua tập hợp các khoảng compact được chứa trong I; khi đó tích phân $ \int_a^b f(t)\,dt $ là cận trên bé nhất của tập hợp các $ \int_J f(t)\,dt $.*

Thật vậy, vì $ f \geq 0 $, quan hệ $ J \subset J' $ kéo theo rằng
$$
\int_J f\,dt \leq \int_{J'} f\,dt;
$$
do đó ánh xạ $ J \mapsto \int_J f\,dt $ là tăng, và mệnh đề suy ra từ định lý giới hạn đơn điệu (*Gen. Top.*, IV, p. 349, đl. 2).

Khi ánh xạ $ J \mapsto \int_J f(t)\,dt $ không bị chặn, nó có giới hạn $ +\infty $ đối với tập có hướng $ \mathcal{K}(I) $; khi đó, theo cách nói lạm dụng ngôn ngữ, người ta nói rằng tích phân $ \int_a^b f(t)\,dt $ bằng $ +\infty $. Các tính chất của tích phân đã được thiết lập trong số 1 được mở rộng (khi xét các hàm $ \geq 0 $) cho trường hợp mà một số tích phân đang xét là vô hạn, miễn là các hệ thức trong đó chúng xuất hiện có nghĩa.

**Mệnh đề 3 (nguyên lý so sánh).** *Cho $ f $ và $ g $ là hai hàm thực điều tiết trên một khoảng $ I \subset \mathbf{R} $, sao cho $ 0 \leq f(x) \leq g(x) $ tại mỗi điểm mà $ f $ và $ g $ liên tục (*xem* II, p. 61, mệnh đề 6). Nếu tích phân của $ g $ trên $ I $ hội tụ, thì tích phân của $ f $ cũng hội tụ, và ta có $ \int_I f(t)\,dt \leq \int_I g(t)\,dt $. Hơn nữa, hai tích phân không thể bằng nhau trừ khi $ f(x) = g(x) $ tại mọi điểm của $ I $ mà $ f $ và $ g $ liên tục.*

Bây giờ, với mọi khoảng compact $ J \subset I $ ta có

$$
\int_J f(t)\,dt \leq \int_J g(t)\,dt;
$$

vì $ \int_J g(t)\,dt \leq \int_I g(t)\,dt $, các tích phân $ \int_J f\,dt $ bị chặn trên, nên tích phân $ \int_I f(t)\,dt $ hội tụ; hơn nữa, khi chuyển qua giới hạn, ta có $ \int_I f(t)\,dt \leq \int_I g(t)\,dt $. Giả sử thêm rằng $ f(x) < g(x) $ tại một điểm $ x \in I $ mà tại đó $ f $ và $ g $ liên tục; tồn tại một khoảng compắc $[c,\ d]$ được chứa trong $ I $, không thu về một điểm (duy nhất), và sao cho $ x \in [c,\ d] $; ta có $ \int_c^d f(t)\,dt < \int_c^d g(t)\,dt $ (II, p. 61, hệ quả 1), và vì mặt khác $ \int_a^c f(t)\,dt \leq \int_a^c g(t)\,dt $ và $ \int_d^b f(t)\,dt \leq \int_d^b g(t)\,dt $ theo điều đã nói ở trên, nên khi cộng từng số hạng một, ta thấy rằng $ \int_a^b f(t)\,dt < \int_a^b g(t)\,dt $.

Mệnh đề này cung cấp phương tiện được dùng thường xuyên nhất để quyết định xem tích phân của một hàm $ f \geq 0 $ có hội tụ hay không: đó là so sánh $ f $ với một hàm đơn giản hơn $ g \geq 0 $ mà người ta đã biết tích phân của nó là hội tụ hay không hội tụ; ta sẽ thấy trong chương V cách tìm các hàm so sánh, trong những trường hợp thông dụng nhất; và ta sẽ suy ra các tiêu chuẩn thông dụng về sự hội tụ của các tích phân và của các chuỗi.

### 3. TÍCH PHÂN HỘI TỤ TUYỆT ĐỐI

#### Định nghĩa 2 {#fvr-ii-s2-def-2 .statement}

*Người ta nói rằng tích phân của một hàm điều chỉnh $ \mathbf{f} $ trên một khoảng $ I \subset \mathbf{R} $ là hội tụ tuyệt đối nếu tích phân của hàm dương $ \| \mathbf{f}(x) \| $ là hội tụ.*

#### Mệnh đề 4 {#fvr-ii-s2-prop-4 .statement}

*Nếu tích phân của $ \mathbf{f} $ trên $ I $ hội tụ tuyệt đối thì nó hội tụ, và ta có*

$$
\left| \int_I \mathbf{f}(t)\,dt \right| \leq \int_I \| \mathbf{f}(t) \| \,dt.\tag{2}
$$

Thật vậy, với mọi khoảng compắc $ J \subset I $ ta có (II, p. 61, công thức (16))

$$
\left| \int_J \mathbf{f}(t)\,dt \right| \leq \int_J \| \mathbf{f}(t) \| \,dt.\tag{3}
$$

Nếu tích phân của hàm dương $ \| \mathbf{f}(x) \| $ là hội tụ, thì với mọi $ \varepsilon > 0 $ tồn tại một khoảng compact $[\alpha,\ \beta]$ được chứa trong $ I $, sao cho, với mọi khoảng compact $[\lambda,\ \gamma]$ được chứa trong $ I $ và không có điểm trong nào chung với $[\alpha,\ \beta]$, ta có $ \int_{\lambda}^{\gamma} \| \mathbf{f}(t) \, dt \| \leq \varepsilon $ (II, p. 65, mệnh đề 1); suy ra rằng $ \left| \int_{\lambda}^{\gamma} \mathbf{f}(t)\,dt \right| \leq \varepsilon $, điều này chứng tỏ sự hội tụ của tích phân trên $ I $ (II, p. 16, mệnh đề 1); khi chuyển qua giới hạn trong (3) ta suy ra bất đẳng thức (2).

#### Hệ quả {#fvr-ii-s2-n3-cor-1 .statement}

*Cho $ E, F, G $ là ba không gian định chuẩn đầy đủ trên $ \mathbf{R} $, và $ (x, y) \mapsto x.y $ là một ánh xạ song tuyến tính liên tục từ $ E \times F $ vào $ G $. Cho $ \mathbf{f}, \mathbf{g} $ là hai hàm điều chỉnh trên $ I $, nhận giá trị trong $ E $ và $ F $ tương ứng. Nếu $ \mathbf{f} $ bị chặn trên $ I $ và nếu* tích phân của g hội tụ tuyệt đối trên I, thì tích phân của [f, g] hội tụ tuyệt đối.

Thật vậy, tồn tại một số h > 0 sao cho ta có $ \| [x.y] \| \leq h \| x \| . \| y \| $ đồng nhất (Gen. Top., IX, p. 173, th. 1); nếu đặt $ k = \sup_{x \in I} \| f(x) \| $, thì ta có $ \| [f(x).g(x)] \| \leq h k \| g(x) \| $ trên I; nguyên lý so sánh khi đó cho thấy tích phân của [f.g] hội tụ tuyệt đối, và, từ (2),

$$
\left\| \int_I [f(t).g(t)] \, dt \right\| \leq h k \int_I \| g(t) \| \, dt.
$$

#### Nhận xét {#fvr-ii-s2-n3-rem-1 .statement}

Một tích phân có thể hội tụ mà không hội tụ tuyệt đối; điều này được chỉ ra bởi Ví dụ 3 của II, p. 64, trong đó chuỗi có số hạng tổng quát $ u_n $ là hội tụ mà không hội tụ tuyệt đối.

### Bài tập {#fvr-ii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
