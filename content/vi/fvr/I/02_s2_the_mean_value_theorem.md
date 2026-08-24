---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 2
section_title: THE MEAN VALUE THEOREM
lang: vi
source: fvr-i-vii
pdf_pages: 0027-0034, 0052-0054
extraction: ocr
subsections:
    - "no": 1
      title: ROLLE'S THEOREM
      page: 0
      pdf_page: 27
    - "no": 2
      title: THE MEAN VALUE THEOREM FOR REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 28
    - "no": 3
      title: THE MEAN VALUE THEOREM FOR VECTOR FUNCTIONS
      page: 0
      pdf_page: 30
    - "no": 4
      title: CONTINUITY OF DERIVATIVES
      page: 0
      pdf_page: 33
statements: 21
exercises: 14
content_sha256: 5d9d22d4022374c1f2b1f43dbe7f16eae2e7bcf4371789a3c1a7610d27967d23
translated_from: content/en/fvr/I/02_s2_the_mean_value_theorem.md
source_content_sha256: a38b0b71726db7638222498a9f8d96ec6066d0c8b8907804d8a53707f2d8e51c
translation_model: gpt-5.4, copied
translation_run: translate-vi-2283b08e
glossary_version: 34
glossary_terms_sha256: 174370f24293ce7e6f988933a4191dc2e8d99fef3b424dc6365ed4ee46a58b89
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỊNH LÝ GIÁ TRỊ TRUNG BÌNH

Các giả thiết và kết luận được chứng minh trong § 1 có tính chất địa phương: chúng chỉ liên quan đến các tính chất của các hàm đang xét trên một lân cận nhỏ tùy ý của một điểm cố định. Trái lại, các vấn đề mà chúng ta khảo sát trong tiết này liên quan đến các tính chất của một hàm trên toàn bộ một khoảng.

### 1. ĐỊNH LÝ ROLLE

#### Mệnh đề 1 ("định lý Rolle") {#fvr-i-s2-prop-1 .statement}

Cho $ f $ là một hàm thực, hữu hạn và liên tục trên một khoảng đóng $ I = [a, b] $ (trong đó $ a < b $), có đạo hàm (hữu hạn hay không) tại mọi điểm của ]$ a, b $[, và sao cho $ f(a) = f(b) $. Khi đó tồn tại một điểm $ c $ của ]$ a, b $[ sao cho $ f'(c) = 0 $.

Mệnh đề là hiển nhiên nếu $ f $ là hằng: nếu không, chẳng hạn $ f $ nhận những giá trị $ > f(a) $, và do đó đạt cận trên nhỏ nhất của nó tại một điểm $ c $ nằm bên trong I (Gen. Top., IV, p. 359, th. 1). Vì $ f $ đạt cực đại địa phương tại điểm này nên ta có $ f'(c) = 0 $ (I, p. 20, prop. 7).

#### Hệ quả {#fvr-i-s2-n1-cor-1 .statement}

Cho $ f $ là một hàm thực, hữu hạn và liên tục trên $ [a, b] $ (với $ a < b $), và có đạo hàm (hữu hạn hay không) tại mọi điểm. Khi đó tồn tại một điểm $ c $ của ]$ a, b $[ sao cho $ f(b) - f(a) = f'(c)(b - a) $.

Chỉ cần áp dụng mệnh đề 1 cho hàm $ f(x) - \frac{f(b) - f(a)}{b - a}(x - a) $.

Hệ quả này có nghĩa là có một điểm $ M_c = (c, f(c)) $ trên đồ thị $ C $ của $ f $ sao cho $ a < c < b $ và sao cho tiếp tuyến với $ C $ tại điểm này song song với đường thẳng nối các điểm $ M_a = (a, f(a)) $ và $ M_b = (b, f(b)) $.

### 2. ĐỊNH LÝ GIÁ TRỊ TRUNG BÌNH CHO CÁC HÀM NHẬN GIÁ TRỊ THỰC

Kết quả quan trọng sau đây là một hệ quả của hệ quả của mệnh đề 1: nếu ta có $ m \leq f'(x) \leq M $ trên ]$ a, b $[, thì cũng có $ m \leq \frac{f(b) - f(a)}{b - a} \leq M $. Nói cách khác, một *chặn đối với đạo hàm của* $ f' $ trên toàn bộ khoảng có các đầu mút $ a, b $ kéo theo *cùng chặn đó* đối với $ \frac{f(b) - f(a)}{b - a} $ (tỉ số của "số gia" của hàm số với "số gia" của biến trên khoảng). Chúng tôi sẽ phát biểu chính xác hơn kết quả cơ bản này, và tổng quát hóa nó, trong phần tiếp theo.

#### Mệnh đề 2 {#fvr-i-s2-prop-2 .statement}

*Cho* $ f $ *là một hàm thực hữu hạn và liên tục trên khoảng đóng bị chặn* $ I = [a, b] $ *(trong đó* $ a < b $*) và có đạo hàm phải* (hữu hạn hay không) *tại mọi điểm của phần bù tương đối trong* $ [a, b) $ *của một tập con đếm được* $ A $ *của khoảng này. Nếu* $ f'_d(x) \geq 0 $ *tại mọi điểm của* $ [a, b[ $ *không thuộc* $ A $, *thì ta có* $ f(b) \geq f(a) $; *nếu hơn nữa,* $ f'_d(x) > 0 $ *tại ít nhất một điểm của* $ [a, b[ $, *thì* $ f(b) > f(a) $.

Cho $ \varepsilon > 0 $ tùy ý, và ký hiệu bởi $ (a_n)_{n \geq 1} $ một dãy thu được bằng cách liệt kê tập hợp đếm được $ A $. Gọi $ J $ là tập hợp các điểm $ y \in I $ sao cho ta có

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

(1)

với mọi $ x $ sao cho $ a \leq x \leq y $, trong đó tổng ở số hạng thứ hai của vế phải được lấy trên mọi chỉ số $ n $ mà $ a_n < x $. Ta sẽ chỉ ra rằng nếu $ f'_d(x) \geq 0 $ tại mọi điểm của $ [a, b[ $ phân biệt với các $ a_n $, thì $ J = I $.

Rõ ràng là $ J $ không rỗng, vì $ a \in J $; hơn nữa định nghĩa của tập hợp này cho thấy rằng nếu $ y \in J $ thì ta có $ x \in J $ với $ a \leq x \leq y $, do đó $ J $ là một *khoảng* có đầu mút trái là $ a $ (*Gen. Top.*, IV, p. 336, mệnh đề 1); gọi $ c $ là đầu mút phải của nó. Ta có $ c \in J $; điều này rõ ràng nếu $ c = a $; nếu không, với mọi $ x < c $ ta có bất đẳng thức (1), và *a fortiori*

$$
f(x) - f(a) \geq -\varepsilon(c - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

từ đó suy ra, khi cho $ x $ tiến tới $ c $ trong bất đẳng thức này (vì $ f $ liên tục), rằng $ c $ thỏa mãn (1).

Vì thế, ta sẽ thấy rằng tất yếu phải có $ c = b $. Thật vậy, nếu có $ c < b $, thì hiển nhiên ta có $ c \notin A $; nay $ f'_d(c) $ tồn tại, và vì theo giả thiết $ f'_d(c) \geq 0 $, nên tồn tại một $ y $ sao cho $ c < y \leq b $ và sao cho với $ c \leq x \leq y $ ta có

$$
f(x) - f(c) \geq -\varepsilon(x - c)
$$

từ đó, có tính đến (1), trong đó $ x $ được thay bởi $ c $,

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n} \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

điều đó có nghĩa là $ y \in J $, mâu thuẫn với định nghĩa của $ c $. Vậy ta có $ c = a_k $ với một chỉ số $ k $ nào đó; vì $ f $ liên tục tại điểm $ a_k $ nên tồn tại một $ y $ sao cho $ c < y \leq b $ và sao cho với $ c < x \leq y $ ta có
$$
f(x) - f(c) \geq -\frac{\varepsilon}{2^k}
$$
từ đó, có tính đến (1), trong đó $ x $ được thay bởi $ c $,
$$
f(x) - f(a) \geq -\varepsilon(c-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n} \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
điều này lại dẫn đến một mâu thuẫn; do đó ta có $ c = b $, và hệ quả là
$$
f(b) - f(a) \geq -\varepsilon(b-a) - \varepsilon \sum_{a_n < b} \frac{1}{2^n} \geq -\varepsilon(b-a) - \varepsilon. \tag{2}
$$
Vì $ \varepsilon > 0 $ là tùy ý nên từ (2) ta suy ra rằng $ f(b) \geq f(a) $, điều đó chứng minh phần thứ nhất của mệnh đề.

Bây giờ ta nhận xét rằng kết quả này áp dụng cho một khoảng $[x, y]$ với $ a \leq x < y \leq b $ chứng minh rằng $ f $ là *tăng* trên I; nếu có $ f(b) = f(a) $ thì có thể suy ra rằng $ f $ là *hằng* trên I, và khi đó $ f'_d(x) = 0 $ tại mọi điểm của $[a, b[$; phần thứ hai suy ra từ điều này.

#### Hệ quả {#fvr-i-s2-n2-cor-1 .statement}

*Cho $ f $ là một hàm thực liên tục hữu hạn trên $[a, b]$ (trong đó $ a < b $) và có đạo hàm phải tại mọi điểm của phần bù trong $[a, b[$ của một tập con đếm được $ A $ của khoảng này. Để $ f $ tăng trên I thì điều kiện cần và đủ là $ f'_d(x) \geq 0 $ tại mọi điểm của $[a, b[$ không thuộc $ A $; để $ f $ tăng ngặt thì điều kiện cần và đủ là điều kiện trước đó được thỏa mãn, và thêm nữa tập hợp các điểm $ x $ mà tại đó $ f'_d(x) > 0 $ là trù mật trong $[a, b]$.*

#### Nhận xét 1 {#fvr-i-s2-n2-rem-1 .statement}

Mệnh đề 2 vẫn đúng khi thay khoảng $[a, b[$ bằng ]$a, b$ và các từ "đạo hàm phải" bằng "đạo hàm trái".

#### Nhận xét 2 {#fvr-i-s2-n2-rem-2 .statement}

Giả thiết về *tính liên tục* của $ f $ trên khoảng đóng I (chứ không chỉ *liên tục phải* $ ^4 $ tại mọi điểm của $[a, b[$) là cốt yếu để mệnh đề 2 đúng (*xem* I, p. 36, bài tập 8 ).

#### Nhận xét 3 {#fvr-i-s2-n2-rem-3 .statement}

Không thể bảo đảm kết luận của mệnh đề 2 nếu ta chỉ giả sử rằng tập hợp $ A $ các điểm "ngoại lệ" là không đâu trù mật trong I, nhưng không đếm được (*xem* I, p. 37, bài tập 3).

Mệnh đề 2 kéo theo định lý cơ bản sau đây (dường như tổng quát hơn):

**ĐỊNH LÝ 1** (định lý giá trị trung bình). *Cho $ f $ và $ g $ là hai hàm thực hữu hạn liên tục xác định trên một khoảng đóng bị chặn $ I = [a, b] $ và có một

$ ^4 $ Một hàm xác định trên một khoảng $ I \subset \mathbf{R} $ được gọi là *liên tục phải* tại một điểm $ x_0 \in I $ nếu hạn chế của nó trên khoảng $ I \cap [x_0, +\infty[ $ liên tục tại điểm $ x_0 $ đối với khoảng này; điều đó cũng tương đương với việc nói rằng giới hạn phải của hàm này tồn tại tại điểm ấy và bằng giá trị của hàm tại điểm ấy.

đạo hàm phải (hữu hạn hay không) tại mọi điểm của phần bù tương đối trong $[a,\ b[$ của một tập con đếm được của khoảng này. Giả sử thêm rằng $f'_d(x)$ và $g'_r(x)$ không đồng thời vô hạn, trừ tại các điểm của một tập con đếm được của I, và rằng tồn tại các số hữu hạn $m$, $M$ sao cho

$$
mg'_r(x) \leq f'_d(x) \leq Mg'_r(x)
$$

trừ tại các điểm của một tập con đếm được của I (thay thế $Mg'_r(x)$ (resp. $mg'_r(x)$) bởi 0 nếu $M = 0$ (resp. $m = 0$) và $g'_r(x) = \pm \infty$. Trong các điều kiện ấy, ta có

$$
m(g(b) - g(a)) < f(b) - f(a) < M(g(b) - f(a))
$$

trừ khi ta có $f(x) = Mg(x) + k$, hoặc $f(x) = mg(x) + k$ ($k$ hằng) với mọi $x \in I$.

Chỉ cần áp dụng mệnh đề 2 cho các hàm $Mg - f$ và $f - mg$, mà dưới các giả thiết của chúng ta, có đạo hàm phải dương trừ tại các điểm của một tập con đếm được của I.

#### Nhận xét {#fvr-i-s2-n2-rem-4 .statement}

Định lý 1 không còn đúng nếu cho phép $f'_d$ và $g'$ đồng thời vô hạn trên một tập con không đếm được của I (xem I, p. 37, bài tập 3).

#### Hệ quả {#fvr-i-s2-n2-cor-2 .statement}

Cho $f$ là một hàm hữu hạn liên tục trên $[a,\ b]$ (trong đó $a < b$) và có đạo hàm phải (hữu hạn hay không) tại mọi điểm của phần bù tương đối B trong $[a,\ b[$ của một tập con đếm được của khoảng này. Nếu $m$ và $M$ là các cận dưới lớn nhất và cận trên nhỏ nhất của $f'_d$ trên B thì ta có

$$
m(b - a) < f(b) - f(a) < M(b - a)
$$

nếu $f$ không phải là một hàm tuyến tính afin; nếu $f$ là tuyến tính afin thì ta có

$$
m = M = \frac{f(b) - f(a)}{b - a}.
$$

Các bất đẳng thức (5) là hệ quả của (4) khi $m$ và $M$ hữu hạn; trường hợp một trong hai số đó là vô hạn thì tầm thường.

#### Nhận xét {#fvr-i-s2-n2-rem-5 .statement}

Các bất đẳng thức (5) chứng minh rằng một hàm liên tục không thể có đạo hàm phải bằng $+\infty$ tại mọi điểm của một khoảng (x. I, p. 38, bài tập 6).

### 3. ĐỊNH LÝ GIÁ TRỊ TRUNG BÌNH CHO CÁC HÀM VECTƠ

#### Định lý 2 {#fvr-i-s2-thm-2 .statement}

Cho $f$ là một hàm vectơ được xác định và liên tục trên một khoảng đóng bị chặn $I = [a,\ b]$ của $\mathbf{R}$ (với $a < b$) và nhận giá trị trong một không gian định chuẩn E trên $\mathbf{R}$; cho $g$ là một hàm thực tăng liên tục trên I. Giả sử rằng $f$ và $g$ có đạo hàm phải tại mọi điểm của phần bù tương đối trong $[a,\ b[$ của một tập con đếm được A của khoảng này (cho phép $ g'_r(x) $ là vô hạn tại một số điểm $ x \notin A $), và giả sử rằng tại mỗi điểm ấy ta có

$$
\| f'_d(x) \| \leq g'_r(x).
$$

Dưới các giả thiết đó ta có

$$
\| f(b) - f(a) \| \leq g(b) - g(a).
$$

Chứng minh tiến hành tương tự như chứng minh của mệnh đề 2. Cho $ \varepsilon > 0 $ là tùy ý, và $ (a_n) $ là dãy thu được bằng cách liệt kê A theo một thứ tự nào đó. Gọi J là tập hợp các điểm $ y \in I $ sao cho, với mọi $ x $ thỏa mãn $ a \leq x \leq y $ ta có

$$
\| f(x) - f(a) \| \leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n};
$$

ta sẽ chỉ ra rằng $ J = I $. Ta thấy ngay lập tức, như trong mệnh đề 2, rằng J là một khoảng có đầu mút trái là $ a $; nếu c là đầu mút phải của nó thì $ c \in J $; thật vậy, với mọi $ x < c $ ta có (8), và *a fortiori*

$$
\| f(x) - f(a) \| \leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

từ đó, cho $ x $ tiến tới $ c $ trong bất đẳng thức này, theo tính liên tục của $ f $ suy ra rằng $ c $ thỏa mãn (8).

Ta hãy chỉ ra rằng tất phải có $ c = b $. Vậy giả sử rằng $ c < b $ và hơn nữa $ c \notin A $: khi đó $ f'_d(c) $ và $ g'_r(c) $ tồn tại và thỏa mãn (6); trước hết giả sử rằng $ g'_r(c) $ (tất yếu là $ \geq 0 $) hữu hạn; khi đó luôn có thể viết $ f'_d(c) = u g'_r(c) $, với $ \| u \| \leq 1 $; vì hàm $ f(x) - u g(x) $ có đạo hàm phải bằng không tại điểm $ c $ nên phải tồn tại một $ y $ sao cho $ c < y \leq b $ và sao cho với $ c \leq x \leq y $ ta có

$$
\| f(x) - f(c) - u(g(x) - g(c)) \| \leq \varepsilon (x - c)
$$

từ đó

$$
\| f(x) - f(c) \| \leq g(x) - g(c) + \varepsilon (x - c)
$$

và, có tính đến (8), trong đó $ x $ được thay bởi $ c $,

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}.
\end{align*}
$$

Vậy ta có $ y \in J $, điều này là mâu thuẫn. Bây giờ giả sử rằng $ c \notin A $ và $ g'_r(c) = +\infty $; khi đó tồn tại một $ y $ sao cho $ c < y \leq b $ và sao cho với $ c \leq x \leq y $ thì một mặt ta có

$$
\| f(x) - f(c) \| \leq (\| f'_d(c) \| + 1) (x - c)
$$

còn mặt khác ta có

$$
g(x) - g(c) \geq (\| f'_d(c) \| + 1) (x - c)
$$

suy ra

$$
\| f(x) - f(c) \| \leq g(x) - g(c)
$$

và suy ra như trên. Sau cùng, nếu có $ c = a_k $, thì tồn tại một $ y $ sao cho $ c < y \leq b $, và sao cho với $ c < x \leq y $ ta có

$$
\| f(x) - f(c) \| \leq \frac{\varepsilon}{2^k}
$$

từ đó, có tính đến (8), với $ x $ được thay bởi $ c $,

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
\end{align*}
$$

điều này lại dẫn đến một mâu thuẫn. Chứng minh kết thúc như chứng minh của mệnh đề 2.

Q.E.D.

#### Nhận xét 1 {#fvr-i-s2-n3-rem-1 .statement}

Ở đây cũng vậy, trong mệnh đề của định lý 2 người ta có thể thay khoảng $[a, b[$ bằng ]$a, b]$ và "đạo hàm phải" bằng "đạo hàm trái".

#### Nhận xét 2 {#fvr-i-s2-n3-rem-2 .statement}

Ta sẽ chỉ ra về sau cách đồng nhất trường hợp đẳng thức trong (7), và cũng cách tổng quát hóa định lý 2 cho trường hợp E là một không gian lồi địa phương tùy ý, với sự trợ giúp của một phương pháp chứng minh khác cho phép suy ra định lý 2 từ định lý 1.

#### Hệ quả {#fvr-i-s2-n3-cor-1 .statement}

Để một hàm vectơ liên tục trên một khoảng $ I \subset \mathbf{R} $, nhận giá trị trong một không gian định chuẩn E trên $ \mathbf{R} $, là hằng trên I, thì đủ là nó có đạo hàm phải không tại mọi điểm của phần bù (tương đối đối với I) của một tập con đếm được của I.

#### Nhận xét {#fvr-i-s2-n3-rem-3 .statement}

Các chứng minh của định lý 1 và 2 dựa một cách cốt yếu trên các tính chất tôpô đặc biệt của trường $ \mathbf{R} $; người ta có thể cho các ví dụ về các trường định giá K mà đối với chúng tồn tại những ánh xạ tuyến tính không hằng từ K vào chính nó có đạo hàm không tại mọi điểm (x. I, p. 37, bài tập 2).

#### Mệnh đề 3 {#fvr-i-s2-prop-3 .statement}

Cho $ f $ là một hàm vectơ nhận giá trị trong một không gian chuẩn E trên $ \mathbf{R} $, được xác định và liên tục trên một khoảng $ I \subset \mathbf{R} $, và khả vi phải trên phần bù B (đối với I) của một tập con đếm được của I; khi đó với mọi điểm $ x_0 \in B, x \in I, y \in I $, ta có (chẳng hạn giả sử rằng $ x < y $)

$$
\| f(y) - f(x) - f'_d(x_0)(y - x) \| \leq (y - x) \sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \|.
$$ (9)

Thật vậy chỉ cần áp dụng đl. 2, thay thế $ f $ bằng hàm

$$
f(z) - f'_d(x_0)z,
$$

và $ g $ bằng hàm tuyến tính có đạo hàm là $ \sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \| $.

Định lý 2 mở rộng cho các hàm vectơ của một biến phức:

#### Mệnh đề 4 {#fvr-i-s2-prop-4 .statement}

*Cho $ f $ là một hàm khả vi liên tục của một biến phức xác định trên một tập con mở lồi $ A $ của trường $ \mathbf{C} $, với giá trị trong một không gian định chuẩn $ E $ trên trường $ \mathbf{C} $. Nếu ta có $ \|f'(z)\| \leq m $ với mọi $ z \in A $, thì ta có $ \|f(b) - f(a)\| \leq m |b - a| $ đối với mọi cặp điểm $ a, b $ của $ A $.*

Ta đặt $ g(t) = \frac{1}{b - a} f(a + t(b - a)) $ với $ 0 \leq t \leq 1 $; do $ g'(t) = f'(a + t(b - a)) $, áp dụng đl. 2 cho hàm $ g $ suy ra mệnh đề ngay lập tức.

#### Hệ quả {#fvr-i-s2-n3-cor-2 .statement}

*Một hàm vectơ $ f $ của một biến phức, được xác định và liên tục trên một tập mở $ A \subset \mathbf{C} $, và nhận giá trị trong một không gian định chuẩn trên $ \mathbf{C} $, là hằng nếu nó có đạo hàm bằng không tại mọi điểm của $ A $.*

Thật vậy, gọi $ a $ là một điểm tùy ý của $ A $; tập $ B $ gồm các điểm $ z $ của $ A $ mà tại đó $ f(z) = f(a) $ là *đóng* vì $ f $ liên tục; nó cũng *mở*, như được chứng minh bằng cách áp dụng mệnh đề 4 (với $ m = 0 $) cho một lân cận mở lồi, được chứa trong $ A $, của một điểm tùy ý của $ B $; do đó nó đồng nhất với $ A $.

#### Mệnh đề 5 {#fvr-i-s2-prop-5 .statement}

*Cho $ f $ là một hàm vectơ của một biến phức, được xác định, liên tục và khả vi trên một tập hợp mở lồi $ A \subset \mathbf{C} $, nhận giá trị trong một không gian định chuẩn trên trường $ \mathbf{C} $; khi đó, với mọi điểm $ x_0, x $ và $ y $ trong $ A $, ta có*
$$
\|f(y) - f(x) - f'_d(x_0)(y - x)\| \leq |y - x| \sup_{z \in A} \|f'(z) - f'(x_0)\|.
$$
(10)

Chỉ cần áp dụng đl. 2 cho hàm
$$
g(t) = f(x + t(y - x)) - f'(x_0)(y - x)t
$$
trên khoảng $[0, 1]$.

### 4. TÍNH LIÊN TỤC CỦA CÁC ĐẠO HÀM

#### Mệnh đề 6 {#fvr-i-s2-prop-6 .statement}

*Cho $ I $ là một khoảng mở trong $ \mathbf{R} $, cho $ x_0 $ là một trong các đầu mút của $ I $, và $ f $ là một hàm vectơ xác định và liên tục trên $ I $, nhận giá trị trong một không gian định chuẩn đầy đủ $ E $ trên $ \mathbf{R} $; giả sử rằng $ f $ có đạo hàm phải tại các điểm của phần bù $ B $ trong $ I $ của một tập con đếm được của $ I $. Khi đó điều kiện cần và đủ để $ f'_d(x) $ có giới hạn khi $ x $ tiến tới $ x_0 $ mà vẫn thuộc $ B $ và $ \neq x_0 $ là $ \frac{f(y) - f(x)}{y - x} $ có giới hạn $ c $ khi $ (x, y) $ tiến tới $ (x_0, x_0) $ với điều kiện $ x \in I, y \in I, x \neq x_0, y \neq x_0 $ và $ x \neq y $. Trong các điều kiện đó, $ f $ được kéo dài bằng liên tục tới điểm $ x_0 $, đạo hàm phải $ f'_d(x) $ tiến tới $ c $ khi $ x $ tiến tới $ x_0 $ (mà vẫn thuộc B), và hàm $ f $ đã được kéo dài (xác định trên $ I \cup \{x_0\} $) có đạo hàm tại $ x_0 $ bằng $ c $.*

Giả sử chẳng hạn rằng $ x_0 $ là đầu mút bên phải của I. Trước hết ta hãy chỉ ra rằng nếu $ f'_d(x) $ tiến tới $ c $ khi $ x $ tiến tới $ x_0 $ mà vẫn nằm trong B và $ \neq x_0 $, thì $ \frac{f(y) - f(x)}{y - x} $ tiến tới $ c $; điều này suy ra ngay lập tức từ định lý 2 áp dụng cho hàm $ f(z) - cz $, cho

$$
\| f(y) - f(x) - c(y - x) \| \leq (y - x) \sup_{z \in B,\ x < z < y} \| f'_d(z) - c \|
$$

với $ x < y < x_0 $. Ngược lại, nếu $ \frac{f(y) - f(x)}{y - x} $ tiến tới $ c $, thì với mọi $ \varepsilon > 0 $ tồn tại một $ h > 0 $ sao cho các điều kiện $ |x - x_0| < h,\ |y - x_0| < h\ (x \neq x_0,\ y \neq x_0) $ suy ra

$$
\| f(y) - f(x) - c(y - x) \| \leq \varepsilon |y - x|.
$$

Nhưng với mọi $ x \in B $ và $ \neq x_0 $ sao cho $ |x - x_0| < h $ tồn tại một $ k > 0 $ (phụ thuộc vào $ x $) sao cho quan hệ $ x < y < x + k $ kéo theo

$$
\| f(y) - f(x) - f'_d(x)(y - x) \| \leq \varepsilon |y - x|
$$

từ đó, xét (11):

$$
\| f'_d(x) - c \| \leq 2\varepsilon
$$

với $ |x - x_0| < h,\ x \in B $ và $ x \neq x_0 $. điều đó chứng tỏ rằng $ f'_d(x) $ tiến tới $ c $. Hơn nữa, từ quan hệ (11) ta có ngay lập tức rằng

$$
\| f(y) - f(x) \| \leq (\|c\| + \varepsilon) |y - x|,
$$

điều này chứng tỏ (theo tiêu chuẩn Cauchy) rằng $ f $ có một giới hạn $ d $ tại điểm $ x_0 $ khi $ x $ tiến tới điểm này mà vẫn thuộc I và $ \neq x_0 $; bây giờ, cho $ x $ tiến tới $ x_0 $ trong (11), với $ y \in I,\ y \neq x_0 $ và $ |y - x_0| \leq h $, ta có

$$
\left\| \frac{f(y) - d}{y - x_0} - c \right\| \leq \varepsilon
$$

điều đó chứng tỏ rằng $ c $ là đạo hàm tại điểm $ x_0 $ của hàm $ f $ được mở rộng bằng liên tục lên $ I \cup \{x_0\} $.

#### Nhận xét {#fvr-i-s2-n4-rem-1 .statement}

Một lập luận tương tự, dựa trên đl. 1, cho thấy rằng nếu $ f $ là một hàm thực sao cho $ f'_d(x) $ tiến tới $ +\infty $ tại điểm $ x_0 $ thì tỷ số

$$
(f(y) - f(x))/(y - x)
$$

cũng tiến tới $ +\infty $, và ngược lại; hơn nữa, nếu $ f $ có một giới hạn hữu hạn tại điểm $ x_0 $ (điều này không phải là một hệ quả của giả thiết hiện tại), thì hàm $ f $ được mở rộng bằng liên tục đến $ x_0 $ có một đạo hàm bằng $ +\infty $ tại điểm này.

### Bài tập {#fvr-i-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
