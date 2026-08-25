---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 4
section_title: The extended real line
lang: vi
source: top-i-iv
pdf_pages: 0348-0353, 0394-0395
extraction: ocr
subsections:
    - "no": 1
      title: HOMEOMORPHISMS OF OPEN INTERVALS OF $ \mathbf{R} $
      page: 0
      pdf_page: 348
    - "no": 2
      title: THE EXTENDED LINE
      page: 0
      pdf_page: 349
    - "no": 3
      title: ADDITION AND MULTIPLICATION IN $ \overline{\mathbf{R}} $
      page: 0
      pdf_page: 351
statements: 11
exercises: 7
content_sha256: 9e3a6dd77130a121725c8dbbcf170d61ed10213dee64058cb6e373ac74631ccd
translated_from: content/en/top/IV/04_s4_the_extended_real_line.md
source_content_sha256: 8896fe25e69f07b614cde7d2b86558a1c5fa38420ee161ac676b8d3b817492cc
translation_model: gpt-5.4
translation_run: translate-vi-45e1198d
glossary_version: 34
glossary_terms_sha256: abbe8d97db43c6322153973490569f4658d27622594da81702b62b326d2633c1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. ĐƯỜNG THẲNG THỰC MỞ RỘNG

### 1. CÁC ĐỒNG PHÔI CỦA CÁC KHOẢNG MỞ CỦA $ \mathbf{R} $

#### Mệnh đề 1 {#top-iv-s4-prop-1 .statement}

Mọi khoảng mở không rỗng của $ \mathbf{R} $ đều đồng phôi với $ \mathbf{R} $.

Trước hết hãy xét một khoảng mở bị chặn $ I = ]a, b[ $ ($ a < b $). Với mỗi $ x \in I $ đặt $ f(x) = -\left( \frac{1}{x-a} + \frac{1}{x-b} \right) $. Hàm này liên tục và tăng ngặt trên $ I $, vì ta đã thấy rằng $ \frac{1}{x-b} $ giảm nghiêm ngặt trên $ ]-, b[ $ và $ \frac{1}{x-a} $ giảm nghiêm ngặt trên $ ]a, \to[ $. Suy ra $ f $ là một phép đồng phôi từ $ I $ lên một khoảng $ f(I) $ của $ \mathbf{R} $ (\S 2, no. 6, Định lý 5). $ f(I) $ không bị chặn trên cũng không bị chặn dưới; chẳng hạn, nếu ta có $ f(x) \leq c $ với mọi $ x \in I $, thì sẽ suy ra $ 1 - \frac{b-x}{x-a} \leq c(b-x) $, vì $ b-x > 0 $; và điều này dẫn đến mâu thuẫn khi $ x $ đủ gần $ b $ (do tính liên tục tại điểm $ b $ của hai vế của bất đẳng thức, vốn là các hàm hữu tỉ). Do đó $ f(I) = \mathbf{R} $, và vì thế mọi khoảng mở bị chặn đều đồng phôi với $ \mathbf{R} $. Gọi $ g $ là hàm nghịch đảo của $ f $: nó ánh xạ mọi khoảng mở không bị chặn của $ \mathbf{R} $ lên một khoảng $ J $ được chứa trong $ I $ và mở trong $ I $. Vì $ I $ mở trong $ \mathbf{R} $, nên $ J $ cũng mở trong $ \mathbf{R} $; vì nó bị chặn, nên nó đồng phôi với $ \mathbf{R} $; và như vậy ta đã chứng minh rằng mọi khoảng mở không bị chặn đều đồng phôi với $ \mathbf{R} $.

#### Nhận xét {#top-iv-s4-n1-rem-1 .statement}

Để chỉ ra rằng mọi khoảng mở *bị chặn* đều đồng phôi với nhau, chỉ cần nhận xét rằng, nếu $ a \neq b $ và $ a' \neq b' $, thì có một đồng phôi của $ \mathbf{R} $ lên chính nó, có dạng $ x \to ax + \beta $ (và chỉ có một) biến $ a $ thành $ a' $ và $ b $ thành $ b' $, và do đó biến khoảng mở (tương ứng, nửa mở, đóng) với các đầu mút $ a, b $ thành khoảng mở (tương ứng, nửa mở, đóng) với các đầu mút $ a', b' $; bạn đọc có thể dễ dàng kiểm tra điều này bằng cách tính $ \alpha $ và $ \beta $.

### 2. ĐƯỜNG THẲNG MỞ RỘNG

Bây giờ ta sẽ định nghĩa, bằng cách *thêm vào* $ \mathbf{R} $ hai phần tử mới, một không gian tôpô $ \overline{\mathbf{R}} $ sao cho mọi đồng phôi của $ \mathbf{R} $ lên một khoảng mở bị chặn $ I $ của $ \mathbf{R} $ đều có thể được mở rộng thành một đồng phôi của $ \overline{\mathbf{R}} $ lên khoảng đóng có cùng các đầu mút như $ I $.

Gọi $ \overline{\mathbf{R}} $ là tập hợp thu được bằng cách kề thêm (*Lý thuyết tập hợp*, R, § 4, no. 5) vào $ \mathbf{R} $ hai phần tử mới, ký hiệu là $ -\infty $ và $ +\infty $. Ta mở rộng thứ tự trên $ \mathbf{R} $ thành thứ tự trên $ \overline{\mathbf{R}} $ bằng cách đặt $ -\infty < a $ và $ a < +\infty $ với mọi $ a \in \mathbf{R} $, và $ -\infty < +\infty $; hiển nhiên như vậy ta thu được một tập hợp có thứ tự toàn phần, mà thứ tự của nó cảm sinh thứ tự của đường thẳng thực trên $ \mathbf{R} $. Tiếp theo, xét tôpô trên $ \overline{\mathbf{R}} $ được sinh bởi tập hợp các khoảng mở của $ \overline{\mathbf{R}} $. Vì vết trên $ \mathbf{R} $ của một khoảng mở của $ \overline{\mathbf{R}} $ là một khoảng mở của $ \mathbf{R} $, nên tôpô này cảm sinh trên $ \mathbf{R} $ tôpô của đường thẳng thực.

#### Định nghĩa 1 {#top-iv-s4-def-1 .statement}

*Tập hợp* $ \overline{\mathbf{R}} $ *được trang bị cấu trúc thứ tự và tôpô được định nghĩa ở trên được gọi là đường thẳng thực mở rộng.*

Khi dùng đường thẳng mở rộng $ \overline{\mathbf{R}} $ thì thường thuận tiện khi gọi các điểm của nó là *các số thực*, theo một sự lạm dụng ngôn ngữ; khi đó các điểm của $ \mathbf{R} $ được gọi là *các số thực hữu hạn*. Chúng tôi sẽ chấp nhận quy ước này *trong tiết diện này và ba tiết diện tiếp sau của chương này*; mỗi khi về sau chúng tôi chấp nhận quy ước này, chúng tôi sẽ nói rõ tường minh nó mở rộng đến phần nào của văn bản.

Nếu $ a $ là một số thực hữu hạn, các khoảng $[a, +\infty[$ và ]—$ \infty, a]$ (tương ứng ]$ a, +\infty[$ và ]—$ \infty, a[$) của $ \overline{\mathbf{R}} $ được chứa trong $ \mathbf{R} $ và trùng nhau với các khoảng của $ \mathbf{R} $ từ trước đến nay được ký hiệu bởi $[a, \rightarrow[$ và ]$ \leftarrow, a]$ (tương ứng ]$ a, \rightarrow[$ và ]$ \leftarrow, a[$); ký hiệu mới này được dùng thường xuyên hơn nhiều. Hơn nữa, $ \mathbf{R} $ trùng nhau với khoảng ]—$ \infty, +\infty[$ của $ \overline{\mathbf{R}} $, và đôi khi cũng được ký hiệu như vậy.

#### Mệnh đề 2 {#top-iv-s4-prop-2 .statement}

*Mọi phép đồng phôi* $ f $ *của* $ \mathbf{R} $ *lên một khoảng* ]$ a, b[$ *đều có thể được mở rộng thành một phép đồng phôi* $ \overline{f} $ *của* $ \overline{\mathbf{R}} $ *lên* $[a, b]$. *Nếu* $ f $ *là một hàm tăng, thì* $ \overline{f} $ *là một đẳng cấu thứ tự của* $ \overline{\mathbf{R}} $ *lên* $[a, b]$.

Cho $ f $ là một đồng phôi tăng. Nếu ta mở rộng $ f $ lên $ \mathbf{R} $ bằng cách đặt $ \overline{f}(-\infty) = a $ và $ \overline{f}(+\infty) = b $, thì hiển nhiên $ \overline{f} $ là một ánh xạ tăng ngặt (và do đó là một song ánh) từ $ \overline{\mathbf{R}} $ lên $[a, b]$. Do đó $ \overline{f} $ biến mọi khoảng mở của $ \overline{\mathbf{R}} $ thành một khoảng mở đối với $[a, b]$, và vì thế là một đồng phôi từ $ \mathbf{R} $ lên $[a, b]$ theo Định nghĩa 1 và Mệnh đề 5 của § 1, no. 4.

Nếu $ f $ giảm, ta áp dụng điều đã được chứng minh cho đồng phôi tăng $ x \to -f(x) $ từ $ \mathbf{R} $ lên ]$ -b, -a[$.

Mọi tính chất của khoảng $[a, b]$ thu được trong § 2, chỉ liên quan đến cấu trúc cấp và tôpô của khoảng, do đó có thể được chuyển sang $ \overline{\mathbf{R}} $; vì thế có các mệnh đề sau:

#### Mệnh đề 3 {#top-iv-s4-prop-3 .statement}

*Đường thẳng thực mở rộng là compact.*

Do đó (Chương II, § 4, no. 1, Định lý 1) có một cấu trúc đều duy nhất trên $ \overline{\mathbf{R}} $ tương thích với tôpô của nó; cấu trúc đều này đẳng cấu với cấu trúc đều cảm sinh trên $[a, b]$ bởi cấu trúc đều cộng tính của $ \mathbf{R} $. Nhưng cần nhận xét rằng cấu trúc đều *cảm sinh* trên $ \mathbf{R} $ bởi cấu trúc đều của $ \overline{\mathbf{R}} $ *không phải là cấu trúc đều cộng tính của* $ \mathbf{R} $ (mặc dù nó tương thích với tôpô của đường thẳng thực); vì $ \mathbf{R} $ là một không gian *đầy đủ* đối với cấu trúc đều cộng tính của nó, nhưng không phải là một không gian con đầy đủ của $ \overline{\mathbf{R}} $, vì nó không đóng trong $ \overline{\mathbf{R}} $.

#### Mệnh đề 4 {#top-iv-s4-prop-4 .statement}

*Mọi tập con không rỗng của* $ \overline{\mathbf{R}} $ *đều có một cận trên bé nhất và một cận dưới lớn nhất.*

Cận trên bé nhất (tương ứng, cận dưới lớn nhất) của một tập con không rỗng $ A $ của $ \mathbf{R} $ được ký hiệu bởi $ \sup A $ (tương ứng, $ \inf A $). Rõ ràng

(1)
$$
\inf A \leq \sup A.
$$

Nếu $ A \subset B $, thì $ \sup A \leq \sup B $ và $ \inf A \geq \inf B $ (*Lý thuyết tập hợp*, Chương III, § 1, no. 9, Mệnh đề 4).

#### Mệnh đề 5 {#top-iv-s4-prop-5 .statement}

*Một tập con $ A $ của $ \overline{\mathbf{R}} $ là liên thông khi và chỉ khi $ A $ là một khoảng.*

#### Hệ quả {#top-iv-s4-n2-cor-1 .statement}

*Đường thẳng thực mở rộng là một không gian liên thông, liên thông địa phương.*

#### Mệnh đề 6 {#top-iv-s4-prop-6 .statement}

*Một ánh xạ $ f $ từ một khoảng $ I $ của $ \overline{\mathbf{R}} $ vào $ \overline{\mathbf{R}} $ là một đồng phôi của $ I $ lên $ f(I) $ khi và chỉ khi $ f $ đơn điệu nghiêm ngặt và liên tục trên $ I $; khi đó $ f(I) $ là một khoảng của $ \overline{\mathbf{R}} $.

Sau cùng, các hàm $ \sup(x, y) $ và $ \inf(x, y) $ là *liên tục* trên $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $.

### 3. PHÉP CỘNG VÀ PHÉP NHÂN TRONG $ \overline{\mathbf{R}} $

Trước hết chú ý rằng hàm $ -x $ có thể được mở rộng bằng tính liên tục lên $ \overline{\mathbf{R}} $, theo các công thức $ -(-\infty) = +\infty $ và $ -(+\infty) = -\infty $; hàm được mở rộng như vậy là một đồng phôi của $ \overline{\mathbf{R}} $ lên chính nó.

Tiếp theo, xét các hàm $ x + y $ và $ xy $, được xác định trên $ \mathbf{R} \times \mathbf{R} $, nhận giá trị trong $ \mathbf{R} $; khi coi chúng nhận giá trị *trong không gian tôpô* $ \overline{\mathbf{R}} $, ta sẽ thấy rằng chúng cũng có thể được mở rộng bằng tính liên tục tại một số điểm của $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $.

Đối với $ x + y $, đặt $ A' = ]-\infty, +\infty] $ và $ A'' = [-\infty, +\infty[ $. Khi đó ta có mệnh đề sau:

#### Mệnh đề 7 {#top-iv-s4-prop-7 .statement}

*Hàm $ x + y $ có thể được mở rộng bằng tính liên tục trên mỗi tập hợp $ A' \times A' $ và $ A'' \times A'' $, theo các công thức*

$$
(2)
\begin{cases}
x + (+\infty) = (+\infty) + x = +\infty & (x \neq -\infty), \\
x + (-\infty) = (-\infty) + x = -\infty & (x \neq +\infty).
\end{cases}
$$

Chẳng hạn, ta hãy chỉ ra rằng khi $ (x, y) $ tiến tới điểm $ (a, +\infty) $ ($ a \neq -\infty $) mà vẫn nằm trong $ \mathbf{R} \times \mathbf{R} $, thì $ x + y $ tiến tới $ +\infty $. Tồn tại một số hữu hạn $ b < a $, và khoảng $ ]b, +\infty[ $ là một lân cận của $ a $ trong $ \mathbf{R} $; với mọi $ c $ hữu hạn cho trước, các hệ thức $ x > b $ và $ y > c - b $ kéo theo $ x + y > c $, và điều này cho thấy rằng $ x + y $ gần $ +\infty $ tùy ý miễn là $ (x, y) $ đủ gần $ (a, +\infty) $. Lập luận cũng tương tự trong các trường hợp khác.

Trái lại, $ x + y $ *không có giới hạn* tại các điểm $ (-\infty, +\infty) $ và $ (+\infty, -\infty) $ của $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $. Thật vậy, nếu $ x + y $ có giới hạn $ k $ (hữu hạn hoặc vô hạn) khi $ (x, y) $ tiến tới $ (+\infty, -\infty) $ trong khi vẫn thuộc $ \mathbf{R} \times \mathbf{R} $, thì suy ra rằng, với mỗi $ a $ hữu hạn, hàm $ (x + a) - x $ sẽ tiến tới $ k $ khi $ x $ tiến tới $ +\infty $ trong khi vẫn thuộc $ \mathbf{R} $; và điều này là vô lý, vì $ (x + a) - x = a $ và $ a $ là tùy ý.

Nếu $ x, y, z, t $ là các điểm của $ \overline{\mathbf{R}} $ sao cho $ x \leq y $ và $ z \leq t $, thì $ x + z \leq y + t $ bất cứ khi nào cả hai vế của bất đẳng thức này đều xác định.

Chú ý rằng trong $ \overline{\mathbf{R}} $ quan hệ $ x < y $ kéo theo $ x + z < y + z $ chỉ khi $ z $ là hữu hạn, theo các công thức (2); dễ dàng kiểm tra rằng các quan hệ $ x < y $ và $ z < t $ kéo theo $ x + z < y + t $ bất cứ khi nào cả hai vế của bất đẳng thức này đều xác định.

Trong $ \overline{\mathbf{R}} $ ta đặt $ x^+ = \sup (x, 0), x^- = \sup (-x, 0), |x| = \sup (x, -x) $; do đó $ (+\infty)^+ = (-\infty)^- = +\infty $ và $ (+\infty)^- = (-\infty)^+ = 0 $, và $ |+\infty| = |- \infty| = +\infty $. Các tổng $ x^+ - x^- $ và $ x^+ + x^- $ được xác định với mọi $ x \in \overline{\mathbf{R}} $ và vì thế lần lượt bằng $ x $ và $ |x| $ theo nguyên lý mở rộng các đồng nhất thức. Hơn nữa, bất cứ khi nào tổng $ x + y $ được xác định, ta có $ |x + y| \leq |x| + |y| $.

Ngược lại, hãy lưu ý rằng các công thức (6) và (7) của § 1, no. 1 có thể không còn có nghĩa đối với một số giá trị của $ x $ và $ y $ trong $ \overline{\mathbf{R}} $; chẳng hạn, nếu $ x = -\infty $ và $ y = 0 $ thì ta có $ \sup (x, y) = 0 $, nhưng tổng $ x + (y - x)^+ $ không được xác định, vì $ (y - x)^+ = +\infty $.

Ký hiệu $ \overline{\mathbf{R}}^* $ là phần bù của o trong $ \overline{\mathbf{R}} $. Khi đó, tương tự của Mệnh đề 7 đối với phép nhân được phát biểu như sau:

#### Mệnh đề 8 {#top-iv-s4-prop-8 .statement}

*Hàm xy có thể được mở rộng liên tục lên tập $ \overline{\mathbf{R}}^* \times \overline{\mathbf{R}}^* $ theo các công thức*

$$
\begin{cases}
x.(+\infty) = (+\infty).x = \begin{cases} +\infty & \text{nếu } x > 0 \\ -\infty & \text{nếu } x < 0 \end{cases} \\
x.(-\infty) = (-\infty).x = \begin{cases} -\infty & \text{nếu } x > 0 \\ +\infty & \text{nếu } x < 0. \end{cases}
\end{cases}
$$

(3)

Chúng tôi để lại chứng minh cho người đọc; nó tương tự với chứng minh của Mệnh đề 7.

Tương tự, ta thấy rằng $ xy $ không có giới hạn tại các điểm $ (0, +\infty), (+\infty, 0), (0, -\infty), (-\infty, 0) $ của $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $.

Hàm $ xy $ là một luật hợp thành trên $ \overline{\mathbf{R}}^* $ mở rộng luật phép nhân trên $ \mathbf{R} $; luật này kết hợp và giao hoán (nguyên lý mở rộng các đồng nhất thức); nó có 1 là phần tử đơn vị; và các phần tử không chính quy trong $ \overline{\mathbf{R}}^* $ là $ +\infty $ và $ -\infty $.

Nếu $ x \leq y $ và $ z > 0 $ thì ta có $ xz \leq yz $ mỗi khi hai vế của bất đẳng thức này đều được xác định. Nếu tích $ xy $ được xác định, thì $ |x| \cdot |y| $ cũng được xác định, và ta có $ |xy| = |x| \cdot |y| $.

Cuối cùng, công thức phân phối

$$
x(y + z) = xy + xz
$$

vẫn còn đúng, theo nguyên lý mở rộng các đồng nhất thức, mỗi khi mọi phép toán xuất hiện ở một trong hai vế đều được xác định.

Chú ý rằng có thể xảy ra trường hợp vế trái của (4) được xác định trong khi vế phải thì không: chẳng hạn, xét trường hợp $ x = +\infty $, $ y = 2 $ và $ z = -1 $. Vì vậy, cần sử dụng công thức tính phân phối một cách thận trọng trong $ \overline{\mathbf{R}} $.

### Bài tập {#top-iv-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
