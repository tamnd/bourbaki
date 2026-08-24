---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 8
section_title: Usual expansions of real numbers; the power of R
lang: vi
source: top-i-iv
pdf_pages: 0379-0383, 0407-0411
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATIONS TO A REAL NUMBER
      page: 0
      pdf_page: 379
    - "no": 2
      title: EXPANSIONS OF REAL NUMBERS RELATIVE TO A BASE SEQUENCE
      page: 0
      pdf_page: 379
    - "no": 3
      title: DEFINITION OF A REAL NUMBER BY MEANS OF ITS EXPANSION
      page: 0
      pdf_page: 380
    - "no": 4
      title: COMPARISON OF EXPANSIONS
      page: 0
      pdf_page: 382
    - "no": 5
      title: EXPANSIONS TO BASE A
      page: 0
      pdf_page: 382
    - "no": 6
      title: THE POWER OF R
      page: 0
      pdf_page: 383
statements: 3
exercises: 6
content_sha256: 5d277cc806aa4c0451c61201c041b38594c41b5f0a45bf73c9b8d813f98e6959
translated_from: content/en/top/IV/08_s8_usual_expansions_of_real_numbers_the.md
source_content_sha256: b2bfd4fbc49b036cf80faadde5f2068a1c056da3fbc11b10c1b5185ec846e570
translation_model: gpt-5.4
translation_run: translate-vi-6c609c53
glossary_version: 34
glossary_terms_sha256: 812998486be9ef86edef49a4c64c245529e303bae91a7ecc543bd1e4194736eb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 8. CÁC KHAI TRIỂN THÔNG THƯỜNG CỦA SỐ THỰC; LŨY THỪA CỦA R

### 1. XẤP XỈ MỘT SỐ THỰC

#### Định nghĩa 1 {#top-iv-s8-def-1 .statement}

Cho một số $ \varepsilon > 0 $, một số thực $ r $ được gọi là một xấp xỉ với sai số không quá $ \varepsilon $ của một số thực $ x $, nếu $ |x - r| \leq \varepsilon $; $ r $ được gọi là một xấp xỉ thiếu nếu $ r \leq x $, xấp xỉ thừa nếu $ r \geq x $.

Cho $ A $ là một tập con trù mật của $ \mathbf{R} $. Với mỗi $ x \in \mathbf{R} $ và mỗi $ \varepsilon > 0 $, tồn tại một xấp xỉ thiếu (tương ứng, xấp xỉ thừa) của $ x $ với sai số không quá $ \varepsilon $ thuộc $ A $, vì khoảng $ ]x - \varepsilon, x[ $ (tương ứng $ ]x, x + \varepsilon[ $) chứa ít nhất một điểm của $ A $. Bây giờ, nếu ta xét một dãy giảm nghiêm ngặt $ (\varepsilon_n) $ đã cho gồm các số $ > 0 $, tiến về 0, và nếu $ r_n $ là một xấp xỉ của $ x $ với sai số không quá $ \varepsilon_n $, thì dãy $ (r_n) $ có $ x $ làm giới hạn khi $ n $ tiến tới vô hạn.

Trong trường hợp $ A $ là một nhóm con của nhóm cộng $ \mathbf{R} $, và ta hạn chế các $ \varepsilon_n $ thuộc $ A $, ta có thể định nghĩa một cách chính tắc đối với mỗi $ x \in \mathbf{R} $ một dãy $ (r_n) $ các xấp xỉ thiếu của $ x $, thuộc $ A $.

Thật vậy, theo tiên đề Archimedes (\S 2, no. 1, Định lý 1), tập hợp các số nguyên $ p $ sao cho $ p \varepsilon_n \leq x $ có một phần tử lớn nhất $ p_n $; nói cách khác, tồn tại một số nguyên duy nhất $ p_n $ sao cho

$$
p_n \varepsilon_n \leq x < (p_n + 1) \varepsilon_n.
$$

Vì $ |x - p_n \varepsilon_n| \leq \varepsilon_n $, suy ra $ p_n \varepsilon_n $ là một xấp xỉ của $ x $ sai kém hơn $ \varepsilon_n $, và thuộc $ A $ theo giả thiết; tương tự, $ (p_n + 1) \varepsilon_n $ là một xấp xỉ của $ x $ sai vượt quá $ \varepsilon_n $, thuộc $ A $, và hai dãy $ (p_n \varepsilon_n) $ và $ ((p_n + 1) \varepsilon_n) $ có $ x $ làm giới hạn.

### 2. KHAI TRIỂN CỦA CÁC SỐ THỰC ĐỐI VỚI MỘT DÃY CƠ SỞ

Chúng tôi sẽ chỉ giới hạn ở việc nghiên cứu trường hợp $ \varepsilon_n = 1/d_n $, trong đó $ (d_n) $ là một dãy tăng ngặt các số nguyên sao cho $ d_0 = 1 $ và $ d_n $ là một bội của $ d_{n-1} $ với $ n \geq 1 $. Đặt $ a_n = d_n / d_{n-1} $ ($ n \geq 1 $): $ a_n $ là một số nguyên $ > 1 $. Trong trường hợp này, dãy các giá trị gần đúng thiếu hụt $ r_n = p_n / d_n $ là tăng, vì $ p_n $ là số nguyên lớn nhất sao cho $ p_n / d_n \leq x $; nhưng ta có

$$
\frac{p_{n-1}}{d_{n-1}} = \frac{p_{n-1} a_n}{d_n} \leq x < \frac{p_{n-1} + 1}{d_{n-1}} = \frac{p_{n-1} a_n + a_n}{d_n}
$$

sao cho $ a_n p_{n-1} \leq p_n < a_n p_{n-1} + a_n $, và do đó $ r_{n-1} \leq r_n \leq x $. Đặt
$$
p_n = a_n p_{n-1} + u_n;
$$
khi đó $ 0 \leq u_n - a_n $, điều này tương đương với $ 0 \leq u_n \leq a_n - 1 $, vì $ u_n $ là một số nguyên. Vì thế
$$
r_n = r_{n-1} + \frac{u_n}{d_n} = p_0 + \sum_{k=1}^n \frac{u_k}{d_k},
$$
và, vì $ x = \lim_{n \to \infty} r_n $,
$$
x = p_0 + \sum_{n=1}^\infty \frac{u_n}{d_n}.
$$
Chuỗi ở vế phải của (4), có tổng là $ x $, được gọi là khai triển của $ x $ đối với dãy cơ sở $ (d_n) $. Tất cả các hệ số $ u_n $ đều $ \geq 0 $; $ p_0 $ theo định nghĩa là số nguyên lớn nhất $ p $ sao cho $ p \leq x $; nó được gọi là phần nguyên của $ x $, và thường được ký hiệu là $ [x] $.

### 3. ĐỊNH NGHĨA MỘT SỐ THỰC BẰNG KHAI TRIỂN CỦA NÓ

Ngược lại, giả sử ta được cho một số nguyên $ q_0 $ và một dãy $ (v_n) $ ($ n \geq 1 $) các số nguyên sao cho $ 0 \leq v_n \leq a_n - 1 $; ta hỏi liệu có một số $ x $ mà khai triển (4) của nó thỏa mãn $ p_0 = q_0 $ và $ u_n = v_n $ với mọi $ n $ hay không. Nếu có một số như vậy thì nó là duy nhất, vì nó bằng
$$
q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}.
$$
Với mỗi số nguyên $ m > 0 $ ta có (theo nguyên lý so sánh)
$$
\sum_{n=m+1}^\infty \frac{v_n}{d_n} \leq \sum_{n=m+1}^\infty \frac{a_n - 1}{d_n} = \sum_{n=m+1}^\infty \left( \frac{1}{d_{n-1}} - \frac{1}{d_n} \right) = \frac{1}{d_m}
$$
và các số hạng ngoài cùng bên trái và bên phải bằng nhau chỉ khi $ v_n = a_n - 1 $ với mỗi $ n > m $ (\S 7, no. 1, Định lý 2). Do đó chuỗi có số hạng tổng quát là $ \frac{v_n}{d_n} $ là hội tụ; hơn nữa, nếu $ x = q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n} $, ta có
$$
s_m = q_0 + \sum_{n=1}^m \frac{v_n}{d_n} \leq x \leq s_m + \frac{1}{d_m}
$$
và $ x = s_m + \frac{1}{d_m} $ chỉ khi $ v_n = a_n - 1 $ với mỗi $ n > m $. Vì $ s_m $ là một phân số có mẫu số $ d_m $, số gần đúng $ r_m $ của $ x $ sai kém $ 1/d_m $ theo thiếu bằng $ s_m $ hoặc $ s_m + \frac{1}{d_m} $; và khả năng sau chỉ có thể xảy ra nếu $ v_n = a_n - 1 $ với mọi $ n > m $. Vậy:
(i) Có một số lượng *vô hạn* các giá trị của $ n $ sao cho $ v_n < a_n - 1 $: khi đó chuỗi $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $ trùng với khai triển của tổng $ x $ của nó.
(ii) Có một số nguyên $ m \geq 0 $ sao cho $ v_n = a_n - 1 $ mỗi khi $ n > m $, và $ v_m < a_m - 1 $ (nếu $ m > 0 $); khi đó tổng $ x $ của chuỗi $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $ bằng số hữu tỉ
$$
q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \frac{1}{d_m}
$$
có dạng $ k/d_m $ ($ k $ là một số nguyên); *khai triển* của $ x $ trùng với chuỗi (5), trong đó mọi số hạng có chỉ số $ > m $ đều bằng không; một khai triển như vậy được gọi là *hữu hạn*, hoặc *kết thúc*. Chuỗi
$$
q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} = q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \sum_{n=m+1}^{\infty} \frac{a_n - 1}{d_n}
$$
được gọi là *khai triển không chính quy* của số $ x $.

Ngược lại, cho $ x $ là một số hữu tỉ có thể viết dưới dạng một phân số với mẫu số $ d_n $ với một giá trị nào đó của $ n $. Gọi $ m $ là số nguyên nhỏ nhất sao cho $ x $ có dạng $ k/d_m $ ($ k $ là một số nguyên); ta có $ r_n < x $ với $ n < m $, và $ r_m = x $, và do đó khai triển của $ x $ có dạng (5), và $ x $ có một khai triển không chính tắc cho bởi (6); hơn nữa khai triển không chính tắc này là *duy nhất*.

Một số hữu tỉ, được viết dưới dạng bất khả quy $ p/q $, bằng một phân số có mẫu số $ d_n $ khi và chỉ khi $ q $ *chia* $ d_n $ (do đó số $ m $ sẽ là số nguyên $ n $ nhỏ nhất sao cho $ q $ chia $ d_n $). Có thể xảy ra trường hợp *mọi số hữu tỉ* đều có tính chất này (với một $ n $ được chọn thích hợp) : điều này xảy ra khi và chỉ khi mọi số nguyên $ > 0 $ đều chia một $ d_n $ nào đó, chẳng hạn, nếu $ d_n = n! $ Nếu các $ d_n $ có tính chất này, thì một số là hữu tỉ khi và chỉ khi khai triển của nó, đối với dãy $ (d_n) $, là hữu hạn.

Tóm lại: với mọi dãy $ s $ mà số hạng ban đầu $ q_0 $ là một số nguyên tùy ý, và mà số hạng $ v_n (n \geq 1) $ thỏa mãn $ 0 \leq v_n \leq a_n - 1 $, tương ứng một số thực bằng $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $; nếu $ I_n $ ký hiệu khoảng $[0, a_n - 1]$ của $ \mathbf{N} $, thì như vậy ta định nghĩa một ánh xạ $ \varphi $ từ $ X = \mathbf{Z} \times \prod_{n=1}^{\infty} I_n $ *lên trên* đường thẳng thực $ \mathbf{R} $; hơn nữa phương trình $ \varphi(s) = x $, trong đó $ x \in \mathbf{R} $ được cho trước, có *một* nghiệm nếu $ x $ không phải là một phân số có mẫu số $ d_n $ (với một $ n $ nào đó), và có *hai* nghiệm trong trường hợp ngược lại.

### 4. SO SÁNH CÁC KHAI TRIỂN

Nếu ta biết các khai triển của hai số thực phân biệt $ x $ và $ y $, ta có thể xác định xem $ x < y $ hay $ x > y $.

Cho $ x = p_0 + \sum_{n=1}^{\infty} u_n / d_n $, $ y = q_0 + \sum_{n=1}^{\infty} v_n / d_n $ là các khai triển của $ x $ và $ y $. Nếu $ p_0 < q_0 $ thì $ x < y $, vì

$$
p_0 \leq x < p_0 + 1 \leq q_0 \leq y.
$$

Nói chung hơn, giả sử rằng $ p_0 = q_0 $ và $ u_n = v_n $ với $ 1 \leq n \leq m $, nhưng $ u_m < v_m $; nếu

$$
r_n = p_0 + \sum_{k=1}^{n} u_k / d_k, \quad s_n = q_0 + \sum_{k=1}^{n} v_k / d_k,
$$

thì $ r_n = s_n $ với $ n < m $, và vì $ u_m + 1 \leq v_m $, nên $ r_m + \frac{1}{d_m} \leq s_m $; nhưng $ r_m \leq x < r_m + \frac{1}{d_m} \leq s_m \leq y $, do đó một lần nữa ta có $ x < y $. Nói cách khác, *thứ tự của $ x $ và $ y $ cũng chính là thứ tự của hai hạng đầu tiên phân biệt trong các khai triển tương ứng của chúng*.

Suy ra rằng, nếu $ p_0 = q_0 $ và $ u_n = v_n $ với $ n < m $, thì $ m $ số hạng đầu tiên của khai triển của mọi số $ z $ thuộc khoảng đóng có các đầu mút là $ x $ và $ y $ đều *giống hệt* như những số hạng của các khai triển của $ x $ và $ y $.

Ta cũng nhận xét rằng, trong trường hợp này, ta có $ |y - x| \leq \frac{1}{d_{m-1}} $. Nếu ta trang bị cho $ \mathbf{Z} $ và các khoảng $ I_n $ tôpô *rời rạc*, thì suy ra ánh xạ $ \varphi $ được định nghĩa ở trên là *liên tục* trên *không gian tích* $ X $.

### 5. KHAI TRIỂN THEO CƠ SỞ A

Các dãy cơ sở quan trọng nhất là những dãy mà $ d_n = a^n $, trong đó $ a $ là một số nguyên $ > 1 $; khi đó nói rằng $ a $ là *số cơ sở* (hoặc đơn giản là *cơ sở*) của các khai triển tương ứng. Trong tính toán số, người ta dùng các khai triển theo cơ sở 10, được gọi là *khai triển thập phân*; ngoài ra các khai triển theo cơ sở 2 (*nhị phân*) và cơ sở 3 (*tam phân*) cũng thường được dùng.

Để biểu diễn các xấp xỉ thiếu $ r_n $ của một số $ x \geq 0 $, trong khai triển của nó theo cơ sở $ a $, người ta dùng ký hiệu sau đây: mỗi số nguyên $ u $ sao cho $ 0 \leq u \leq a - 1 $ được biểu thị bằng một dấu riêng; nếu

$$
r_n = p_0 + \sum_{k=1}^{n} \frac{u_k}{d_k},
$$

trước hết ta viết, với sự trợ giúp của các ký hiệu này, biểu diễn theo cơ số $ a $ của số nguyên $ p_0 = [x] \geq 0 $ (*Lý thuyết tập hợp*, Chương III, § 5, no. 7), rồi ta đặt một điểm ("dấu thập phân") và lần lượt viết các ký hiệu biểu diễn các số $ u_1, u_2, \ldots, u_n $. Nếu S là ký hiệu thu được như vậy, theo thói quen người ta viết $ x = S... $, do một sự lạm dụng ngôn ngữ. Cần hiểu dứt khoát rằng một quan hệ như vậy chỉ là một phương pháp viết tắt để chỉ rằng vế phải là giá trị gần đúng của $ x $ sai khác thiếu không quá $ 1/a^n $.

Đối với các số âm, cách dùng đã được thiết lập là khác: ta viết một giá trị gần đúng của $ x' = -x > 0 $ theo hệ ký hiệu đã mô tả ở trên, và đặt trước nó dấu “—”; như vậy, chính một giá trị gần đúng của $ x $ sai khác thừa không quá $ 1/a^n $ được ký hiệu theo cách đó.

Cách dùng này có những bất tiện của nó đối với các phép tính số. Trong ký hiệu các logarit âm, người ta dùng cùng một hệ ký hiệu như đối với các số dương, bằng cách đặt một gạch trên phần nguyên, để chỉ rằng nó bằng số đối của số được viết.

### 6. LŨY THỪA CỦA R

Ta có $ \mathbf{R} = \bigcup_{n \in \mathbf{Z}} [n, n+1[ $, và mọi khoảng $ [n, n+1[ $ đều đẳng lực với $ [0, 1[ $. Vì $ [0, 1[ $ là một tập vô hạn nên suy ra $ \mathbf{R} $ đẳng lực với khoảng $ [0, 1[ $. Bằng cách xét khai triển nhị phân của các số thuộc khoảng $ [0, 1[ $ chúng ta sẽ chỉ ra rằng khoảng này đẳng lực với tập hợp S của mọi dãy $ (u_n) $ mà mỗi số hạng đều bằng 0 hoặc 1.

Trước hết, nó đẳng lực với tập con $ S' $ của S gồm các dãy $ (u_n) $ sao cho $ u_n = 0 $ với vô hạn giá trị của $ n $. Mặt khác, phần bù $ S'' $ của $ S' $ trong S đẳng lực với tập hợp tất cả các khai triển không chính quy của các số hữu tỉ bằng một phân số có mẫu số $ 2^n $; các số này tạo thành một tập con của $ \mathbf{Q} $, do đó tập hợp các số ấy là đếm được và vì thế $ S'' $ cũng đếm được. Vì $ S' $ là vô hạn, nó đẳng lực với S, suy ra kết quả.

Khi đó S đẳng lực lượng với $ \mathfrak{P}(\mathbf{N}) $; vì ta có thể định nghĩa một song ánh từ $ \mathfrak{P}(\mathbf{N}) $ lên S bằng cách ánh xạ mỗi tập con A của $ \mathbf{N} $ tới dãy $ (u_n) $ sao cho $ u_n = 0 $ nếu $ n \in A $ và $ u_n = 1 $ nếu $ n \notin CA $. Vậy ta đã chứng minh được:

#### Định lý 1 (Cantor) {#top-iv-s8-thm-1 .statement}

*Tập hợp các số thực đẳng lực lượng với tập hợp tất cả các tập con của một tập vô hạn đếm được.*

#### Hệ quả {#top-iv-s8-n6-cor-1 .statement}

*Tập hợp các số thực có một lực lượng lớn hơn nghiêm ngặt lực lượng của một tập đếm được.*

Một tập hợp đẳng lực lượng với $ \mathbf{R} $ được gọi là có lũy thừa của liên tục. Theo Mệnh đề 1 của § 4, no. 1, mọi khoảng chứa nhiều hơn một điểm đều có lũy thừa của liên tục. Hơn nữa, phần bù của một tập con đếm được của $ \mathbf{R} $ có lũy thừa của liên tục; đặc biệt, *tập hợp tất cả các số vô tỉ có lũy thừa của liên tục*.

### Bài tập {#top-iv-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
