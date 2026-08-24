---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 3
section_title: DERIVATIVES OF HIGHER ORDER
lang: vi
source: fvr-i-vii
pdf_pages: 0035-0038, 0054-0060
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF ORDER $ n $
      page: 0
      pdf_page: 35
    - "no": 2
      title: TAYLOR'S FORMULA
      page: 0
      pdf_page: 36
statements: 8
exercises: 18
content_sha256: 32da98ab86becb7f3a0ae9c7aace97fcab0357bc719dfc2d0e2b28e9c8a5a73c
translated_from: content/en/fvr/I/03_s3_derivatives_of_higher_order.md
source_content_sha256: b3502042b688c4ca4f6d490cd3c7155785b2edf28d35926fc607be7637b4dc64
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-c31cec4e
glossary_version: 34
glossary_terms_sha256: df82059238029d6c8da82f738f03ca29ee9279cadc1a644ab858242c7427ce1f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐẠO HÀM CẤP CAO

### 1. ĐẠO HÀM CẤP $ n $

Cho $ f $ là một hàm vectơ của một biến thực, được định nghĩa, liên tục và khả vi trên một khoảng $ I $. Nếu đạo hàm $ f' $ tồn tại trên một lân cận (đối với $ I $) của một điểm $ x_0 \in I $, và khả vi tại điểm $ x_0 $, thì đạo hàm của nó được gọi là *đạo hàm cấp hai* của $ f $ tại điểm $ x_0 $, và được ký hiệu bởi $ f''(x_0) $ hoặc $ D^2f(x_0) $. Nếu đạo hàm cấp hai này tồn tại tại mọi điểm của $ I $ (điều này kéo theo rằng $ f' $ tồn tại và liên tục trên $ I $), thì $ x \mapsto f''(x) $ là một hàm vectơ được ký hiệu bởi $ f'' $ hoặc $ D^2f $. Ta định nghĩa, theo cùng cách đó, một cách đệ quy, *đạo hàm cấp* $ n^{th} $ (hay *đạo hàm cấp* $ n $) của $ f $, và ký hiệu nó bởi $ f^{(n)} $ hoặc $ D^n f $; theo định nghĩa, giá trị của nó tại điểm $ x_0 \in I $ là đạo hàm của hàm $ f^{(n-1)} $ tại điểm $ x_0 $: định nghĩa này giả thiết sự tồn tại của *tất cả* các đạo hàm $ f^{(k)} $ cấp $ k \leq n - 1 $ trên một *lân cận* của $ x_0 $ đối với $ I $, và tính khả vi của $ f^{(n-1)} $ tại điểm $ x_0 $.

Chúng ta sẽ nói rằng $ f $ khả vi *n lần* tại điểm $ x_0 $ (tương ứng, trong một khoảng) nếu nó có đạo hàm $ n^{th} $ tại điểm này (tương ứng, trong khoảng này). Ta nói rằng $ f $ *khả vi vô hạn lần* trên $ I $ nếu với mỗi số nguyên $ n > 0 $, nó có một đạo hàm cấp $ n $ trên $ I $.

Theo quy nạp theo $ m $, ta thấy rằng

$$
D^m(D^n f) = D^{m+n} f.
$$

Chính xác hơn, khi một trong hai vế trong (1) được xác định thì vế kia cũng được xác định và bằng nó.

#### Mệnh đề 1 {#fvr-i-s3-prop-1 .statement}

*Tập hợp các hàm vectơ xác định trên một khoảng* $ I \subset \mathbf{R} $, *nhận giá trị trong một không gian vectơ tôpô cho trước* $ E $, *và có đạo hàm bậc* $ n^{th} $ *trên* $ I $, *là một không gian vectơ trên* $ \mathbf{R} $, *và* $ f \mapsto D^n f $ *là một ánh xạ tuyến tính từ không gian này vào không gian vectơ các ánh xạ tuyến tính từ* $ I $ *vào* $ E $.

Người ta chứng minh các công thức

$$
D^n(f + g) = D^n f + D^n g \tag{2}
$$
$$
D^n(fa) = D^n f . a \tag{3}
$$

bằng quy nạp theo $ n $ khi $ f $ và $ g $ có đạo hàm bậc $ n^{th} $ trên $ I $ ($ a $ là hằng).

#### Mệnh đề 2 ("công thức Leibniz") {#fvr-i-s3-prop-2 .statement}

*Cho* $ E, F, G $ *là ba không gian vectơ tôpô trên* $ \mathbf{R} $, *và* $ (x, y) \mapsto [x.y] $ *là một ánh xạ song tuyến tính liên tục từ* $ E \times F $ *vào* $ G $. *Nếu* $ f $ *(resp.* $ g $) *được xác định trên một khoảng* $ I \subset \mathbf{R} $, *nhận giá trị trong* $ E $ *(resp.* $ F $) *và có đạo hàm bậc* $ n^{th} $ *trên* $ I $, *thì* $ [f.g] $ *có đạo hàm bậc* $ n^{th} $ *trên* $ I $, *được cho bởi công thức*

$$
D^n[f.g] = [f^{(n)}.g] + \binom{n}{1}[f^{(n-1)}.g'] + \cdots + \binom{n}{p}[f^{(n-p)}.g^{(p)}] + \cdots + [f.g^{(n)}]. \tag{4}
$$

Công thức (4) được chứng minh bằng quy nạp theo $ n $ (dùng quan hệ $ \binom{n}{p} = \binom{n-1}{p} + \binom{n-1}{p-1} $ đối với các hệ số nhị thức).

Theo cùng cách đó, ta có thể kiểm tra công thức sau đây (trong đó các giả thiết giống như trong mệnh đề 2):

$$
[f^{(n)} . g] + (-1)^{n-1} [f . g^{(n)}] = D([f^{(n-1)} . g] - [f^{(n-2)} . g'] + \cdots + (-1)^{n-1} [f . g^{(n-1)}]).
$$

Các mệnh đề trước đã được phát biểu cho các hàm khả vi $ n $ lần trên một khoảng; chúng tôi để bạn đọc tự phát biểu các mệnh đề tương tự cho các hàm khả vi $ n $ lần tại một điểm.

### 2. CÔNG THỨC TAYLOR

Cho $ f $ là một hàm vectơ xác định trên một khoảng $ I \subset \mathbf{R} $, nhận giá trị trong một không gian *định chuẩn* $ E $ trên $ \mathbf{R} $; nói rằng $ f $ có đạo hàm tại một điểm $ a \in I $ có nghĩa là

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)(x-a)}{x-a} = 0;
$$

hoặc, nói cách khác, rằng $ f $ "xấp xỉ bằng" hàm *tuyến tính* $ f(a) + f'(a)(x-a) $ trên một lân cận của $ a $ (*xem* chap. V, nơi khái niệm này được phát triển một cách tổng quát). Ta sẽ thấy rằng sự tồn tại của đạo hàm cấp $ n^{th} $ của $ f $ tại điểm $ a $ cũng kéo theo theo cùng một cách rằng $ f $ "xấp xỉ bằng" một *đa thức bậc $ n $ theo $ x $*, với các hệ số trong $ E $ (*Gen. Top.*, X, p. 315) trên một lân cận của $ a $. Nói chính xác:

#### Định lý 1 {#fvr-i-s3-thm-1 .statement}

*Nếu hàm $ f $ có một đạo hàm cấp $ n^{th} $ tại điểm $ a $ thì*

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}}{(x-a)^n} = 0.
$$

Ta tiến hành bằng quy nạp theo $ n $. Định lý đúng với $ n = 1 $. Với $ n $ tùy ý, theo giả thiết quy nạp, có thể áp dụng nó cho đạo hàm $ f' $ của $ f $: với mọi $ \varepsilon > 0 $ tồn tại một $ h > 0 $ sao cho, nếu đặt

$$
g(x) = f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - f''(a)\frac{(x-a)^2}{2!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}
$$

thì, với $ |y-a| \leq h $ và $ y \in I $,

$$
\|g'(y)\| = \left\| f'(y) - f'(a) - f''(a)\frac{(y-a)}{1!} - \cdots - f^{(n)}(a)\frac{(y-a)^{n-1}}{(n-1)!} \right\|
$$
$$
\leq \varepsilon\ |y-a|^{n-1}.
$$

Ta áp dụng định lý giá trị trung bình (I, p. 15, đl. 2) trên khoảng có hai đầu mút $ a,\ x $ (với $ |x-a| \leq h $) cho hàm vectơ $ g $ và cho hàm thực tăng bằng $ \varepsilon |y - a|^n / n $ nếu $ x > a $, và bằng $ -\varepsilon |y - a|^n / n $ nếu $ x < a $; suy ra $ \|g(x)\| \leq \varepsilon |x - a|^n / n $, điều này chứng minh định lý.

Do đó ta có thể viết
$$
f(x) = f(a) + f'(a) \frac{(x - a)}{1!} + f''(a) \frac{(x - a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x - a)^n}{n!} + u(x) \frac{(x - a)^n}{n!}
$$
trong đó $ u(x) $ tiến tới 0 khi $ x $ tiến tới $ a $ mà vẫn thuộc I; công thức này được gọi là *công thức Taylor cấp* $ n $ tại điểm $ a $, và vế phải của (8) được gọi là *khai triển Taylor cấp* $ n $ của hàm $ f $ tại điểm $ a $. Số hạng cuối cùng $ r_n(x) = u(x)(x - a)^n / n! $ được gọi là *số dư* trong công thức Taylor cấp $ n $.

Khi $ f $ có một *đạo hàm cấp* $ n + 1 $ trên I, ta có thể ước lượng $ \|r_n(x)\| $ theo đạo hàm cấp $ n + 1^{th} $ này, trên toàn bộ I, chứ không chỉ trên một lân cận không xác định của $ a $:

#### Mệnh đề 3 {#fvr-i-s3-prop-3 .statement}

*Nếu $ \|f^{(n+1)}(x)\| \leq M $ trên I, thì ta có*
$$
\|r_n(x)\| \leq M \frac{|x - a|^{n+1}}{(n + 1)!}
$$
*trên* I.

Thật vậy, công thức đúng với $ n = 0 $, theo I, p. 15, định lý 2. Hãy chứng minh điều đó bằng quy nạp theo $ n $: theo giả thiết quy nạp áp dụng cho $ f' $, ta có
$$
\|r'_n(y)\| \leq M \frac{|y - a|^n}{n!}
$$
từ đó công thức (9) suy ra theo định lý giá trị trung bình (I, p. 23, định lý 2).

#### Hệ quả {#fvr-i-s3-n2-cor-1 .statement}

*Nếu* $ f $ *là một hàm thực hữu hạn có đạo hàm cấp* $ n + 1 $ *trên* I, *và nếu* $ m \leq f^{(n+1)}(x) \leq M $ *trên* I, *thì với mọi* $ x \geq a $ *trong* I *ta có*
$$
m \frac{(x - a)^{n+1}}{(n + 1)!} \leq r_n(x) \leq M \frac{(x - a)^{n+1}}{(n + 1)!}
$$
*và số hạng thứ hai không thể bằng số hạng thứ nhất* (resp. *hoặc số hạng thứ ba*) *trừ khi* $ f^{(n+1)} $ *là hằng và bằng* $ m $ (resp. $ M $) *trên khoảng* $[a, x]$.

Chứng minh được tiến hành theo cùng một cách, nhưng áp dụng đl. 1 của I, p. 14.

#### Nhận xét 1 {#fvr-i-s3-n2-rem-1 .statement}

Chúng ta đã nhận thấy trong chứng minh định lý 1 rằng nếu $ f $ có đạo hàm cấp $ n $ trên I, và nếu
$$
f(x) = a_0 + a_1(x - a) + a_2(x - a)^2 + \cdots + a_n(x - a)^n + r_n(x)
$$
là khai triển Taylor cấp $ n $ của nó tại điểm $ a $, thì khai triển Taylor cấp $ n - 1 $ của $ f' $ tại điểm $ a $ là
$$
f'(x) = a_1 + 2a_2(x - a) + \cdots + na_n(x - a)^{n-1} + r'_n(x).
$$

Ta nói rằng nó thu được từ khai triển (11) của $ f $ bằng cách *lấy đạo hàm từng số hạng*.

#### Nhận xét 2 {#fvr-i-s3-n2-rem-2 .statement}

Với cùng các giả thiết, các hệ số $ a_i $ trong (11) được xác định truy hồi bởi các hệ thức

$$
a_0 = f(a)
$$
$$
a_1 = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}
$$
$$
a_2 = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a)}{(x - a)^2}
$$
$$
\ldots
$$
$$
a_n = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a) - \cdots - a_{n-1}(x - a)^{n-1}}{(x - a)^n}.
$$

Trong trường hợp $ a = 0 $ đặc biệt suy ra rằng nếu $ f(x^p) $ ($ p $ là một số nguyên > 0) có đạo hàm cấp $ pn $ trên một lân cận của 0 thì khai triển Taylor cấp $ pn $ của hàm này đơn giản là

$$
f(x^p) = a_0 + a_1 x^p + a_2 x^{2p} + \cdots + a_n x^{np} + r_n(x^p)
$$

trong đó $ r_n(x^p) $ là phần dư trong khai triển (*xem* V, p. 222).

#### Nhận xét 3 {#fvr-i-s3-n2-rem-3 .statement}

Định nghĩa của đạo hàm cấp $ n $ và các kết quả trước đó tổng quát hóa ngay lập tức cho các hàm của một biến phức; ở đây chúng tôi sẽ không đi sâu hơn vào chủ đề này; nó sẽ được trình bày chi tiết trong một Cuốn sau của Bộ sách này.

### Bài tập {#fvr-i-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
