---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 2
section_title: EXPANSIONS OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS AND OF THE FUNCTIONS ASSOCIATED WITH THEM
lang: vi
source: fvr-i-vii
pdf_pages: 0120-0128, 0140-0143
extraction: ocr
subsections:
    - "no": 1
      title: EXPANSION OF THE REAL EXPONENTIAL
      page: 0
      pdf_page: 120
    - "no": 2
      title: EXPANSIONS OF THE COMPLEX EXPONENTIAL, OF $ \cos x $ AND $ \sin x $
      page: 0
      pdf_page: 121
    - "no": 3
      title: THE BINOMIAL EXPANSION
      page: 0
      pdf_page: 122
    - "no": 4
      title: EXPANSIONS OF log(1 + x), OF Arc tan x AND OF Arc sin x
      page: 0
      pdf_page: 126
statements: 1
exercises: 9
content_sha256: 198d86904246905cd71fb970b143f291c3aaf8afda746095f90da8d973a01faa
translated_from: content/en/fvr/III/02_s2_expansions_of_the_exponential_and.md
source_content_sha256: 410a3583c6a8f77a8c05a5977eb588d4c142587944dbb2bd15b1210e8986d65a
translation_model: gpt-5.4
translation_run: translate-vi-0774c73d
glossary_version: 34
glossary_terms_sha256: 5c9377d1ec9b5be5018c7d68f2a29045a90e6cea733d8be112a2ca58f957aa15
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. KHAI TRIỂN CỦA HÀM MŨ THỰC VÀ CÁC HÀM SỐ LƯỢNG GIÁC, VÀ CỦA CÁC HÀM LIÊN KẾT VỚI CHÚNG

### 1. KHAI TRIỂN CỦA HÀM MŨ THỰC

Vì $ \mathrm{D}^n \left( e^x \right) = e^x $ nên khai triển Taylor cấp $ n $ của $ e^x $ là

$$
e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + \int_0^x \frac{(x-t)^n}{n!} e^t \, dt. \tag{1}
$$

Số dư trong công thức này là $ > 0 $ với $ x > 0 $ và có dấu của $ (-1)^{n+1} $ khi $ x < 0 $; hơn nữa, bất đẳng thức về trung bình cho thấy rằng

$$
\frac{x^{n+1}}{(n+1)!} < \int_0^x \frac{(x-t)^n}{n!} e^t \, dt < \frac{x^{n+1} e^x}{(n+1)!} \qquad \text{với } x > 0 \tag{2}
$$

$$
\frac{\left| x^{n+1} \right| e^x}{(n+1)!} < \left| \int_0^x \frac{(x-t)^n}{n!} e^t \, dt \right| < \frac{\left| x^{n+1} \right|}{(n+1)!} \qquad \text{với } x < 0 \tag{3}
$$

Bây giờ ta biết rằng dãy $ \left( x^n / n! \right) $ có giới hạn 0 khi $ n $ tăng vô hạn, với mọi $ x \geqslant 0 $ (*Gen. Top.*, IV, p. 365); do đó, giữ cố định $ x $ và cho $ n $ tăng vô hạn trong (1) thì từ (2) và (3) suy ra rằng

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} \tag{4}
$$

và chuỗi ở vế phải là *hội tụ tuyệt đối và đều* trên mọi khoảng compắc của $ \mathbf{R} $. Đặc biệt, ta có công thức

$$
e = 1 + \frac{1}{1!} + \frac{1}{2!} + \cdots + \frac{1}{n!} + \cdots \tag{5}
$$

Công thức này cho phép ta tính các xấp xỉ hữu tỉ tùy ý gần với số $ e $; ta được

$$
e = 2.718\,281\,828\ldots
$$

với sai số nhỏ hơn $ 1/10^9 $. Hơn nữa, công thức (5) chứng minh rằng $ e $ là một số *vô tỉ* $ ^{2} $ (*Gen. Top.*, IV, p. 375).

#### Nhận xét {#fvr-iii-s2-n1-rem-1 .statement}

Vì số dư trong công thức (1) là $ > 0 $ với $ x > 0 $ nên, với $ x > 0 $, ta có

$$
e^x > 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^{n+1}}{(n+1)!}
$$

và *a fortiori*

$$
e^x > \frac{x^{n+1}}{(n+1)!}
$$

với mọi số nguyên $ n $: từ đó suy ra rằng $ e^x / x^n $ *tiến tới* $ +\infty $ khi $ x $ tăng, với mọi số nguyên $ n $: ta sẽ gặp lại kết quả này trong chương V bằng một phương pháp khác (V, p. 231).

$^{2}$ CH. HERMITE đã chứng minh vào năm 1873 rằng $ e $ là một số *siêu việt* trên trường $ \mathbf{Q} $ các số hữu tỉ (nói cách khác, nó không phải là nghiệm của bất kỳ đa thức nào với các hệ số hữu tỉ) (*Œuvres*, t. III, p. 150, Paris (Gauthier-Villars), 1912).

### 2. KHAI TRIỂN CỦA HÀM MŨ PHỨC, CỦA $ \cos x $ VÀ $ \sin x $

Cho $ z $ là một số phức tùy ý và xét hàm $ \varphi(t) = e^{zt} $ của biến thực $ t $; ta có $ D^n \varphi(t) = z^n e^{zt} $ và $ e^z = \varphi(1) $; do đó, biểu diễn $ \varphi(1) $ bằng chuỗi Taylor cấp $ n $ của nó tại điểm $ t = 0 $ (II, p. 62) cho

$$
e^z = 1 + \frac{z}{1!} + \frac{z^2}{2!} + \cdots + \frac{z^n}{n!} + z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

một công thức tương đương với (1) khi $ z $ là thực. Số dư

$$
r_n(z) = z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

trong công thức này có thể được chặn trên, theo giá trị tuyệt đối, bằng cách dùng bất đẳng thức trung bình; nếu $ z = x + i y $ thì ta có $ |e^{zt}| = e^{xt} $, nên $ |e^{zt}| \leq 1 $ nếu $ x \leq 0 $, $ |e^{zt}| \leq e^x $ nếu $ x > 0 $; do đó

$$
|r_n(z)| \leq \frac{|z|^{n+1}}{(n+1)!} \text{ nếu } x \leq 0
$$
$$
|r_n(z)| \leq \frac{|z|^{n+1} e^x}{(n+1)!} \text{ nếu } x > 0.
$$

Như trên ta kết luận rằng

$$
e^z = \sum_{n=0}^\infty \frac{z^n}{n!}
$$

chuỗi này *hội tụ tuyệt đối và đều* trên mọi tập con compắc của $ \mathbf{C} $.

Từ (6) người ta suy ra đặc biệt rằng

$$
e^{ix} = 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \cdots + \frac{i^n x^n}{n!} + i^{n+1} \int_0^x \frac{(x-t)^n}{n!} e^{it} \, dt
$$

từ đó ta suy ra các khai triển Taylor của $ \cos x $ và $ \sin x $; khi lấy phần thực của (10) ở cấp $ 2n+1 $ ta được

$$
\cos x = 1 - \frac{x^2}{2!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!} + (-1)^{n+1} \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

với số dư được chặn bởi

$$
\left| \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt \right| \leq \frac{|x|^{2n+2}}{(2n+2)!}.
$$

Tương tự, lấy phần ảo của (10) ở cấp $ 2n $, ta được

$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!}
$$
$$
+ (-1)^n \int_0^1 \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt
$$

với số dư bị chặn bởi

$$
\left| \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt \right| \leq \frac{|x|^{2n+1}}{(2n+1)!}.
$$

Hơn nữa, khi so sánh các số dư trong (11) ở các cấp $2n+1$ và $2n+3$, ta có

$$
\int_0^1 \frac{(x-t)^{2n+3}}{(2n+3)!} \cos t \, dt = \frac{x^{2n+2}}{(2n+2)!} - \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

và khi xét đến (12), ta thấy rằng số dư trong (11) có *cùng dấu* với $(-1)^{n+1}$ bất kể $x$ là gì; theo cùng cách ấy ta có thể chứng minh rằng số dư trong (13) có *cùng dấu* với $(-1)^n x$. Đặc biệt, với $n=0$ và $n=1$ trong (11), và với $n=1$ và $n=2$ trong (13), ta thu được các bất đẳng thức

$$
1 - \frac{x^2}{2} \leq \cos x \leq 1 \quad \text{với mọi } x
$$
(15)

$$
x - \frac{x^3}{6} \leq \sin x \leq x \quad \text{với mọi } x \geq 0.
$$
(16)

Cuối cùng, khi đặt $z = i x$ trong (9) ta có

$$
\cos x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
$$
(17)

$$
\sin x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$
(18)

các chuỗi này hội tụ tuyệt đối và đều trên mọi khoảng compact.

Hơn nữa, rõ ràng là các công thức (17) và (18) vẫn đúng với mọi $x$ *phức*, các chuỗi ở vế phải hội tụ tuyệt đối và đều trên mọi tập con compact của $\mathbf{C}$. Đặc biệt, với mọi $x$ (thực hoặc phức)

$$
\cosh x = \sum_{n=0}^\infty \frac{x^{2n}}{(2n)!}
$$
$$
\sinh x = \sum_{n=0}^\infty \frac{x^{2n+1}}{(2n+1)!}.
$$

### 3. KHAI TRIỂN NHỊ THỨC

Cho $m$ là một số thực *tùy ý*. Với $x > 0$ ta có

$$
D^n (x^m) = m(m-1)\ldots(m-n+1) x^{m-n};
$$

công thức Taylor cấp $ n $ tại điểm $ x = 0 $ đối với hàm $ (1 + x)^m $ cho thấy rằng với mọi $ x > -1 $

$$
(1 + x)^m = 1 + \binom{m}{1} x + \binom{m}{2} x^2 + \cdots + \binom{m}{n} x^n + r_n(x)
$$

với

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt
$$

trong đó ta đặt $ \binom{m}{n} = \frac{m(m-1)\ldots(m-n+1)}{n!} $. Công thức (19) quy về công thức nhị thức (Alg., I, p. 99) khi $ m $ là một số nguyên $ > 0 $ và $ n \geq m $; bằng phép mở rộng, ta cũng lại gọi nó là *công thức nhị thức*, và các hệ số $ \binom{m}{n} $ được gọi là các *hệ số nhị thức*, khi $ m $ là một số thực *tùy ý* và $ n $ là một số nguyên tùy ý $ > 0 $.

Số dư trong (19) có cùng dấu với $ \binom{m}{n+1} $ nếu $ x > 0 $, và có dấu của $ (-1)^{n+1} \binom{m}{n+1} $ nếu $ -1 < x < 0 $. Vì $ \left| \frac{x-t}{1+t} \right| \leq |x| $ với $ t > -1 $ trên khoảng có hai đầu mút là 0 và $ x $, nên ta có đánh giá sau đây đối với số dư, với $ m $ và $ n $ tùy ý và $ x > -1 $:

$$
\left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt \right|
$$
$$
\leq \left| \binom{m-1}{n} x^n ((1+x)^m - 1) \right|.
$$

Nếu giả sử $ x \geq 0 $, và $ n \geq m-1 $, thì $ (1+t)^{n-m+1} \geq 1 $ trên khoảng lấy tích phân, nên

$$
0 \leq \int_0^x \frac{(x-t)^n}{(1+t)^{n-m+1}} \, dt \leq \int_0^x (x-t)^n \, dt = \frac{x^{n+1}}{n+1}
$$

điều này cho ước lượng

$$
|r_n(x)| \leq \left| \binom{m}{n+1} \right| x^{n+1} \quad (x \geq 0,\ n \geq m-1)
$$

đối với số dư. Mặt khác, giả sử rằng $ -1 \leq m < 0 $; nếu thực hiện phép thay đổi biến $ u = \frac{x-t}{x(1+t)} $ trong tích phân (19) thì thu được

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} (1+x)^m x^{n+1} \int_0^1 \frac{u^n \, du}{(1+ux)^{m+1}}.
$$

Để ước lượng tích phân khi $ x > -1 $ ta nhận xét rằng, vì $ m + 1 < 1 $, tích phân $ \int_0^1 \frac{u^n \, du}{(1-u)^{m+1}} $ hội tụ và chặn vế phải của (22) vì $ 1 + u x > 1 - u $. Bây giờ, với $ -1 < x < 0 $ thì giả thiết về $ m $ kéo theo rằng mọi hạng tử $ \binom{m}{1} x, \binom{m}{2} x^2, \ldots, \binom{m}{n} x^n $ xuất hiện ở vế phải của (19) đều $ \geq 0 $, và do đó $ r_n(x) \leq (1 + x)^m $, từ đó, sau khi chia cho $ (1 + x)^m $,

$$
\frac{m(m-1) \ldots (m-n)}{n!} x^{n+1} \int_0^1 \frac{u^n \, du}{(1 + u x)^{m+1}} \leq 1.
$$

Hơn nữa, với $ -1 < x < 0 $ thì nhân tử đứng trước tích phân là $ \geq 0 $, do đó, cho $ x $ tiến tới $ -1 $,

$$
\left| \frac{m(m-1) \ldots (m-n)}{n!} \int_0^1 \frac{u^n \, du}{(1-u)^{m+1}} \right| \leq 1
$$

và do đó với $ -1 \leq m < 0 $ và $ x > -1 $ ta có

$$
|r_n(x)| \leq (1 + x)^m |x|^{n+1}.
$$ (23)

Từ các bất đẳng thức này, trước hết ta có thể suy ra rằng với $ |x| < 1 $ ta có

$$
(1 + x)^m = \sum_{n=0}^\infty \binom{m}{n} x^n
$$ (24)

vế phải (được gọi là chuỗi nhị thức) hội tụ tuyệt đối và đều trên mọi tập con compắc của $ ]-1, +1[ $. Thật vậy ta có thể viết

$$
\binom{m}{n} = (-1)^n \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n} \right)
$$ (25)

do đó

$$
\left| \binom{m}{n} \right| \leq \left( 1 + \frac{|m+1|}{1} \right) \left( 1 + \frac{|m+1|}{2} \right) \ldots \left( 1 + \frac{|m+1|}{n} \right).
$$

Nếu $ |x| \leq r < 1 $ thì tồn tại một $ n_0 $ sao cho $ 1 + \frac{|m|}{n_0} < \frac{1}{r'} $, trong đó $ r < r' < 1 $; do đó, khi đặt

$$
k = \left( 1 + \frac{|m|}{1} \right) \left( 1 + \frac{|m|}{2} \right) \ldots \left( 1 + \frac{|m|}{n_0} \right)
$$

ta có

$$
\left| \binom{m-1}{n} x^n \right| \leq k |x|^{n_0} \left( \frac{r}{r'} \right)^{n - n_0},
$$

điều này chứng minh mệnh đề. Mặt khác, với $ x > 1 $, giá trị tuyệt đối của số hạng tổng quát của chuỗi (24) tăng vô hạn theo $ n $ nếu $ m $ không phải là một số nguyên $ \geq 0 $; thật vậy, từ (25), ta có với $ n > n_1 \geq |m+1| $

$$
\left| \binom{m}{n} \right| \geq \left| \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right|
$$
$$
\left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n} \right).
$$

Cho $ n_0 \geq n_1 $ sao cho với $ n \geq n_0 $ ta có $ 1 - \frac{|m+1|}{n} > \frac{1}{x'} $, trong đó $ 1 < x' < x $. Nếu ta đặt
$$
k' = \left| \left( 1 - \frac{m+1}{1} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right| \left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n_0} \right)
$$
thì, với $ n > n_0 $,
$$
\left| \binom{m}{n} x^n \right| \geq k' |x|^{n_0} \left( \frac{x}{x'} \right)^{n-n_0}
$$
từ đó suy ra mệnh đề.

Ta nhận xét rằng với $ m = -1 $ đồng nhất thức đại số
$$
\frac{1}{1+x} = 1 - x + x^2 - \cdots + (-1)^{n-1} x^{n-1} + (-1)^n \frac{x^n}{1+x}
$$
cho biểu thức của số dư trong công thức tổng quát (19) mà không cần phải lấy tích phân; trong trường hợp này công thức (23) quy về biểu thức tính tổng của chuỗi cấp số nhân (hay cấp số nhân) (Gen. Top., IV, p. 364).

Thứ hai, hãy khảo sát sự hội tụ của chuỗi nhị thức khi $ x = 1 $ hoặc $ x = -1 $ (loại trừ trường hợp tầm thường $ m = 0 $):

$ a) \ m \leq -1 $. Tích có số hạng tổng quát $ 1 - \frac{m+1}{n} $ hội tụ tới $ +\infty $ nếu $ m < -1 $, tới 1 nếu $ m = -1 $, do đó từ (25) suy ra rằng với $ x = \pm 1 $ số hạng tổng quát của chuỗi nhị thức không tiến tới 0.

$ b) \ -1 < m < 0 $. Lần này tích có số hạng tổng quát $ 1 - \frac{m+1}{n} $ hội tụ đến 0, nên bất đẳng thức (21) cho thấy rằng $ r_n(1) $ tiến tới 0. Do đó chuỗi nhị thức hội tụ tại $ x = 1 $ và có tổng là $ 2^m $; hơn nữa, chuỗi nhị thức hội tụ đều trên mọi khoảng $ ]x_0, 1] $ với $ -1 < x_0 \leq 1 $, do điều đã thấy ở trên và do (21). Mặt khác, với $ x = -1 $ mọi số hạng ở vế phải của (24) đều $ \geq 0 $, nếu chuỗi này hội tụ thì có thể suy ra rằng chuỗi nhị thức sẽ hội tụ chuẩn tắc trên $ [-1, 1] $ và vì thế sẽ có tổng là một hàm liên tục trên khoảng này, điều đó là vô lý vì $ (1+x)^m $ không bị chặn trên $ [-1, 1] $ đối với $ m < 0 $. Ta kết luận rằng cả với $ x = 1 $ chuỗi nhị thức cũng không hội tụ tuyệt đối.

$ c) \ m > 0 $. Định nghĩa của $ r_n(x) $ cho thấy rằng $ r_n(x) $ tiến tới giới hạn $ r_n(-1) $ khi $ x $ tiến tới $ -1 $; chuyển qua giới hạn trong (20) suy ra rằng $ |r_n(-1)| \leq \left| \binom{m-1}{n} \right| $, và vì $ m-1 > -1 $ nên ta thấy rằng với $ x = -1 $ chuỗi nhị thức là hội tụ. Hơn nữa, với $ n > m+1 $ mọi số hạng của chuỗi này đều có cùng dấu; do đó chuỗi nhị thức hội tụ chuẩn tắc trên khoảng [−1, 1] và có tổng là (1 + x)^m trên khoảng này.

### 4. KHAI TRIỂN CỦA log(1 + x), CỦA Arc tan x VÀ CỦA Arc sin x

Hãy lấy tích phân hai vế của (26) giữa 0 và x; ta thu được khai triển Taylor cấp n của log(1 + x), đúng với x > −1

$$
\log(1 + x) = \frac{x}{1} - \frac{x^2}{2} + \frac{x^3}{3} + \cdots + (-1)^n \frac{x^n}{n} + (-1)^n \int_0^x \frac{t^n \, dt}{1 + t}.
$$ (27)

Số dư có cùng dấu với (−1)^n nếu x > 0, và < 0 nếu −1 < x < 0; hơn nữa, khi x > 0, ta có 1 + t ≥ 1 với 0 ≤ t ≤ x, và, khi −1 < x < 0, ta có 1 + t ≥ 1 − |x| với x ≤ 0; do đó có các ước lượng đối với số dư

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{n+1} \quad \text{với } x \geq 0 \tag{28}
$$

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{(n+1)(1-|x|)} \quad \text{với } -1 < x \leq 0. \tag{29}
$$

Từ hai công thức cuối này suy ra ngay lập tức rằng với −1 < x ≤ 1 ta có

$$
\log(1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n}
$$ (30)

chuỗi này hội tụ đều trên mọi khoảng compắc được chứa trong ]−1, +1], và hội tụ tuyệt đối với |x| < 1.

Mặt khác, với |x| > 1 số hạng tổng quát của chuỗi ở vế phải của (30) tăng vô hạn về độ lớn theo n (III, p. 106). Với x = −1 chuỗi thu về chuỗi điều hòa, chuỗi này có tổng là +∞ (Gen. Top., IV, p. 365).

Tương tự, hãy thay thế x bằng x^2 trong (26) và lấy tích phân hai vế giữa 0 và x; ta thu được khai triển Taylor cấp 2n − 1 của Arc tan x, đúng với mọi x thực

$$
\operatorname{Arc tan} x = \frac{x}{1} - \frac{x^3}{3} + \frac{x^5}{5} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{2n-1} + (-1)^n \int_0^x \frac{t^{2n} \, dt}{1 + t^2}. \tag{31}
$$

Số dư có dấu của (−1)^n x, và vì 1 + t^2 ≥ 1 với mọi t nên ta có ước lượng

$$
\left| \int_0^x \frac{t^{2n} \, dt}{1 + t^2} \right| \leq \frac{|x|^{2n+1}}{2n+1} \tag{32}
$$

từ đó suy ra rằng, với |x| ≤ 1,

$$
\operatorname{Arc tan} x = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^{2n-1}}{2n-1} \tag{33}
$$

chuỗi này hội tụ đều trên [−1, +1], và hội tụ tuyệt đối với |x| < 1.

Đặc biệt, với x = 1 ta thu được công thức

$$
\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} + \cdots + (-1)^n \frac{1}{2n+1} + \cdots .
$$

Với |x| > 1, số hạng tổng quát của vế phải của (33) tăng vô hạn về độ lớn khi n tăng.

Sau cùng, để có khai triển Taylor của Arc sin x, ta xuất phát từ khai triển của đạo hàm của nó là (1 − x^2)^{-1/2}; khai triển sau này thu được bằng cách thay thế x bởi −x^2 trong khai triển của (1 + x)^{-1/2} thành chuỗi nhị thức; với |x| < 1 điều đó cho

$$
(1 - x^2)^{-1/2} = 1 + \frac{1}{2} x^2 + \frac{1.3}{2.4} x^4 + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} x^{2n} + r_n(x)
$$

với, theo (23), đánh giá

$$
0 \leq r_n(x) \leq \frac{x^{2n+2}}{\sqrt{1-x^2}}
$$

cho số dư.

Lấy nguyên hàm của khai triển trước đó ta được

$$
\text{Arc sin } x = x + \frac{1}{2} \frac{x^3}{3} + \frac{1.3}{2.4} \frac{x^5}{5} + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1} + R_n(x)
$$

trong đó R_n(x) có cùng dấu với x và thỏa mãn bất đẳng thức

$$
|R_n(x)| \leq \int_0^x \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

Hơn nữa, quan hệ (35) cho thấy rằng R_n(x) tiến tới một giới hạn khi x tiến tới 1 hoặc −1, do đó ta có

$$
|R_n(1)| \leq \int_0^1 \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

Nhưng vế phải của (37) tiến tới 0 khi n tiến tới +∞: thật vậy, vì tích phân $ \int_0^1 dt / \sqrt{1-t^2} $ hội tụ, nên với mọi ε > 0 tồn tại một a sao cho 0 < a < 1 và $ \int_a^1 dt / \sqrt{1-t^2} \leq \varepsilon $; mặt khác ta có

$$
\int_0^a \frac{t^{2n+2} dt}{\sqrt{1-t^2}} \leq \frac{1}{\sqrt{1-a^2}} \int_0^a t^{2n+2} dt = \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}}
$$

và vì thế tồn tại một n_0 sao cho với n ≥ n_0 ta có $ \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}} \leq \varepsilon $, do đó, sau cùng, |R_n(x)| ≤ 2ε với |x| ≤ 1 và n ≥ n_0. Vậy ta có

$$
\operatorname{Arc}\sin x = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1}
$$

(38)

vế phải hội tụ chuẩn tắc trên khoảng compact [−1, 1].

Trong trường hợp đối, có thể chứng minh, như đối với chuỗi nhị thức, rằng số hạng tổng quát trong chuỗi ở vế phải của (38) tăng vô hạn về trị tuyệt đối với |x| > 1.
Khi đặt $ x = \frac{1}{2} $, chẳng hạn, trong (38) ta thu được một biểu thức mới của số $ \pi $:

$$
\frac{\pi}{6} = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{1}{(2n+1)2^{2n+1}}
$$

công thức này thích hợp hơn nhiều so với công thức (34) để tính các giá trị gần đúng của $ \pi $ (xem Calcul numérique); do đó thu được

$$
\pi = 3.141\,592\,653\ldots
$$

chính xác sai khác không quá $ 1/10^9 $.³

³ Số $ \pi $ không những là vô tỉ (x. III, p. 126, exerc. 5) mà còn là siêu việt trên trường $ \mathbf{Q} $ của các số hữu tỉ, như Lindemann đã chứng minh lần đầu tiên vào năm 1882 (xem chẳng hạn D Hilbert, Gesammelte Abhandlungen, v. 1, p. 1, Berlin (Springer), 1932).

### Bài tập {#fvr-iii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
