---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 6
section_title: Continuous and semi-continuous real-valued functions
lang: vi
source: top-i-iv
pdf_pages: 0365-0369, 0399-0403
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 365
    - "no": 2
      title: SEMI-CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 366
statements: 15
exercises: 15
content_sha256: 33eccc256f9bbe71d37f72992f2f84f4f3f1c3fcc99008dd7050d84a6b6f4a9f
translated_from: content/en/top/IV/06_s6_continuous_and_semi_continuous_real.md
source_content_sha256: 2d73c4454ab304cb00c9ee269dc0713aebdab5f45aa6bec1c7a8237ee8a3376e
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-49d4045c
glossary_version: 34
glossary_terms_sha256: 9347e15a31e60b8563cf5a02b9063ffdfa7112e244ed4b30607b30f6061ad5ac
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. CÁC HÀM THỰC LIÊN TỤC VÀ NỬA LIÊN TỤC

### 1. CÁC HÀM THỰC LIÊN TỤC

Ngoài các tính chất tổng quát của các hàm liên tục nhận giá trị trong một không gian tôpô tùy ý (Chương I, § 2), các hàm thực liên tục còn có hai tính chất cơ bản sau:

#### Định lý 1 (Weierstrass) {#top-iv-s6-thm-1 .statement}

Cho $ f $ là một hàm thực liên tục xác định trên một không gian quasi-compact rỗng khác $ X $. Khi đó tồn tại ít nhất một điểm $ a \in X $ sao cho $ f(a) = \sup_{x \in X} (f(x)) $, và ít nhất một điểm $ b \in X $ sao cho $ f(b) = \inf_{x \in X} f(x) $. Thật vậy, $ f(X) $ là compact (Chương I, § 9, no. 4, Định lý 2) và do đó đóng trong $ \overline{\mathbf{R}} $; suy ra $ f(X) $ chứa các cận của nó.

Định lý này thường được phát biểu dưới dạng: một hàm thực liên tục trên một không gian quasi-compact rỗng khác đạt các cận của nó.

#### Hệ quả {#top-iv-s6-n1-cor-1 .statement}

Nếu một hàm thực xác định trên một không gian quasi-compact rỗng khác $ X $ liên tục và hữu hạn trên $ X $, thì nó bị chặn trong $ X $.

#### Định lý 2 (Bolzano) {#top-iv-s6-thm-2 .statement}

Cho $ f $ là một hàm thực liên tục xác định trên một không gian liên thông $ X $. Nếu $ a $ và $ b $ là hai điểm bất kỳ của $ X $, và nếu $ \alpha $ là một số thực thuộc khoảng đóng có hai đầu mút là $ f(a) $ và $ f(b) $, thì tồn tại ít nhất một điểm $ x \in X $ sao cho $ f(x) = \alpha $.

Vì $ f(X) $ là liên thông (Chương I, § 11, no. 2, Mệnh đề 4) và do đó là một khoảng của $ \overline{\mathbf{R}} $ (§ 4, no. 2, Mệnh đề 5); nên nó chứa khoảng đóng có hai đầu mút là $ f(a) $ và $ f(b) $.

Định lý này thường được phát biểu dưới dạng *một hàm thực liên tục trên một không gian liên thông không thể chuyển từ một giá trị này sang một giá trị khác mà không chuyển qua mọi giá trị trung gian*.

Tính chất này hoàn toàn không phải là đặc trưng của các hàm liên tục; có những ví dụ về các hàm xác định trên một không gian liên thông và *gián đoạn tại mọi điểm* có tính chất này (Bài tập 2).

### 2. HÀM NỬA LIÊN TỤC

Cho $ f $ là một hàm nhận giá trị thực được xác định trên một không gian tôpô $ X $. Để $ f $ liên tục tại một điểm $ a \in X $ thì điều kiện cần và đủ là:
(i) với mọi số thực $ h < f(a) $, tồn tại một lân cận $ V $ của $ a $ sao cho tại mỗi điểm $ x \in V $ ta có $ h < f(x) $;
(ii) với mọi số thực $ k > f(a) $, tồn tại một lân cận $ W $ của $ a $ sao cho tại mỗi điểm $ x \in W $ ta có $ k > f(x) $.

Các hàm thỏa mãn *chỉ một* trong hai điều kiện này đóng một vai trò quan trọng trong giải tích. Nói chính xác hơn, ta đưa ra định nghĩa sau:

#### Định nghĩa 1 {#top-iv-s6-def-1 .statement}

*Một hàm thực $ f $, xác định trên một không gian tôpô $ X $, được gọi là nửa liên tục dưới* (tương ứng *nửa liên tục trên*) *tại một điểm $ a \in X $, nếu với mỗi $ h < f(a) $ [tương ứng với mỗi $ k > f(a) $] tồn tại một lân cận $ V $ của $ a $ sao cho $ h < f(x) $ [tương ứng $ k > f(x) $] *với mọi* $ x \in V $.

*Một hàm thực được gọi là nửa liên tục dưới* (tương ứng *nửa liên tục trên*) *trên $ X $ nếu nó nửa liên tục dưới* (tương ứng *nửa liên tục trên*) *tại mọi điểm của $ X $*.

Do đó, một hàm thực $ f $ *liên tục* tại một điểm $ a $ khi và chỉ khi nó *vừa nửa liên tục trên vừa nửa liên tục dưới* tại $ a $.

Nếu $ f $ nửa liên tục dưới tại một điểm, thì $-f$ nửa liên tục trên tại điểm đó, và ngược lại; do đó trong phần sau, ta có thể hạn chế việc xét các tính chất của các hàm *nửa liên tục dưới*.

Rõ ràng một hàm nửa liên tục dưới trên $ X $ cũng nửa liên tục dưới trên mọi *không gian con* của $ X $.

#### Ví dụ 1 {#top-iv-s6-n2-exa-1 .statement}

Nếu $ f $ đạt *cực tiểu tương đối* tại một điểm $ a $, nghĩa là nếu tồn tại một lân cận $ V $ của $ a $ sao cho, với mỗi $ x \in V $, ta có $ f(a) \leq f(x) $, thì $ f $ nửa liên tục dưới tại $ a $. Đặc biệt, nếu $ f(a) = -\infty $, thì $ f $ nửa liên tục dưới tại $ a $.

#### Ví dụ 2 {#top-iv-s6-n2-exa-2 .statement}

Định nghĩa một hàm thực $ f $ trên $ \mathbf{R} $ bằng cách đặt $ f(x) = 0 $ nếu $ x $ là vô tỉ, và $ f(x) = 1/q $ nếu $ x $ là hữu tỉ và bằng phân số bất khả quy $ p/q $ ($ q > 0 $). Với mỗi số nguyên $ n > 0 $, tập hợp các số hữu tỉ $ p/q $ sao cho $ q < n $ là đóng, và các điểm của nó là cô lập; do đó với mọi $ x $ vô tỉ, tồn tại một lân cận $ V $ của $ x $ sao cho $ f(y) \leq 1/n $ với mọi $ y \in V $, điều này cho thấy $ f $ liên tục tại $ x $; mặt khác, $ f $ đạt một *cực đại tương đối* tại mọi điểm hữu tỉ $ x $. Do đó $ f $ là nửa liên tục trên trên $ \mathbf{R} $.

Điều kiện để $ f $ nửa liên tục dưới tại $ a $ có thể được phát biểu bằng cách nói rằng, với mỗi $ h < f(a) $, tập hợp $ \overline{f}([h, +\infty]) $ phải là một lân cận của $ a $.

Chỉ cần điều kiện này được thỏa mãn đối với một dãy $ (h_n) $ tăng gồm các số thực $ < f(a) $ tiến tới $ f(a) $.

Trang bị cho $ \overline{\mathbf{R}} $ tôpô trong đó các tập mở là $ \varnothing $ và mọi khoảng mở của $ \overline{\mathbf{R}} $ không bị chặn về phải (nghĩa là, mọi khoảng $ ]a, +\infty[ $ với $ a $ hữu hạn, và khoảng $ [--\infty, +\infty] = ]\leftarrow, \rightarrow[] $). Khi đó hàm thực $ f $ nửa liên tục dưới tại $ a $ khi và chỉ khi nó liên tục tại $ a $ khi được xem như một ánh xạ vào $ \overline{\mathbf{R}} $ được trang bị tôpô này.

#### Mệnh đề 1 {#top-iv-s6-prop-1 .statement}

*Một hàm thực $ f $ trên một không gian tôpô $ X $ là nửa liên tục dưới khi và chỉ khi, với mỗi số thực hữu hạn $ k $, $ \overline{f}([k, +\infty]) $ [tập hợp mọi $ x \in X $ sao cho $ f(x) > k $] là một tập hợp mở trong $ X $ [hay, tương đương, $ \overline{f}([-\infty, k]) $ là một tập hợp đóng trong $ X $].*

Vì điều kiện này cho thấy rằng $ \overline{f}([k, +\infty]) $ là một lân cận của mỗi điểm của nó.

Để $ f $ nửa liên tục dưới trên $ X $ thì điều kiện đủ là $ f^{-1}([k, +\infty]) $ mở trong $ X $ với mọi số thực $ k $ thuộc một tập con trù mật của $ \mathbf{R} $.

#### Hệ quả {#top-iv-s6-n2-cor-1 .statement}

*Một tập con $ A $ của một không gian tôpô $ X $ là mở (resp. đóng) trong $ X $ khi và chỉ khi hàm đặc số (*) của nó $ \varphi_A $ là nửa liên tục dưới (resp. trên) trên $ X $.*

Vì $ \overline{f}_A([k, +\infty]) $ rỗng với $ k \geq 1 $, bằng $ A $ với $ 0 \leq k < 1 $ và bằng $ X $ với $ k < 0 $.

#### Định lý 3 {#top-iv-s6-thm-3 .statement}

*Cho $ f $ là một hàm nửa liên tục dưới trên một không gian quasi-compact không rỗng $ X $. Khi đó có ít nhất một điểm $ a \in E $ sao cho $ f(a) = \inf_{x \in X} f(x) $ (nói cách khác, $ f $ đạt cận dưới lớn nhất của nó trong $ X $).*

Với mỗi $ k \in f(X) $, xét tập hợp $ A_k = \overline{f}([-\infty, k]) $. Các tập hợp này không rỗng và tạo thành một cơ sở lọc trên $ X $; vì chúng đóng theo Mệnh đề 1, chúng có ít nhất một điểm chung $ a $ [tiên đề (C'') cho các không gian quasi-compact]. Do đó với mọi $ x \in X $ ta có $ f(a) \leq f(x) $, và định lý được suy ra.

(*) Ta nhắc lại (Lý thuyết tập hợp, Chương III, § 5, no. 5) rằng hàm đặc số $ \varphi_A $ của một tập con $ A $ của một tập hợp $ X $ là hàm xác định trên $ X $ sao cho $ \varphi_A(x) = 1 $ với mọi $ x \in A $, và $ \varphi_A(x) = 0 $ với mọi $ x \in \complement_A $.

#### Hệ quả {#top-iv-s6-n2-cor-2 .statement}

Cho $ f $ là một hàm nửa liên tục dưới trên một không gian quasi-compact không rỗng $ X $. Nếu $ f(x) > -\infty $ với mọi $ x \in X $, thì $ f $ bị chặn dưới trong $ X $.

Chú ý rằng định lý này và định lý tương ứng đối với các hàm nửa liên tục trên bao hàm định lý Weierstrass như một trường hợp riêng (no. 1, Định lý 1).

#### Mệnh đề 2 {#top-iv-s6-prop-2 .statement}

Cho $ f $ và $ g $ là hai hàm số nhận giá trị thực, nửa liên tục dưới tại một điểm $ a \in X $. Khi đó các hàm số $ \inf(f, g) $ và $ \sup(f, g) $ là nửa liên tục dưới tại $ a $; $ f + g $ cũng vậy mỗi khi nó được xác định, và $ fg $ cũng vậy nếu $ f $ và $ g $ là $ \geq 0 $ và tích $ fg $ được xác định.

Ta cho chứng minh đối với $ f + g $; lập luận là tương tự trong các trường hợp khác. Kết quả là hiển nhiên nếu $ f(a) $ hoặc $ g(a) $ bằng $ -\infty $; nếu không, thì $ f(a) + g(a) > -\infty $. Mọi số hữu hạn $ h < f(a) + g(a) $ đều có thể viết dưới dạng $ h = r + s $, trong đó $ r < f(a) $ và $ s < g(a) $ là hữu hạn [chỉ cần lấy $ s $ sao cho $ h - f(a) < s < g(a) $]; theo giả thiết, tồn tại một lân cận $ V $ của $ a $ sao cho, với mỗi $ x \in V $, ta có $ r < f(x) $, và một lân cận $ W $ sao cho với mỗi $ x \in W $ ta có $ s < g(x) $; do đó $ h = r + s < f(x) + g(x) $ với mọi điểm $ x $ của lân cận $ V \cap W $.

Theo cùng cách ấy ta thấy rằng, nếu $ f $ là nửa liên tục dưới tại một điểm $ a $, và nếu $ f \geq 0 $, thì $ 1/f $ là nửa liên tục trên tại $ a $.

#### Định lý 4 {#top-iv-s6-thm-4 .statement}

Bao trên của một họ $ (f_i) $ các hàm nửa liên tục dưới tại một điểm $ a \in X $ là nửa liên tục dưới tại $ a $.

Cho $ g $ là bao trên. Với mỗi $ h < g(a) $ tồn tại một chỉ số $ i $ sao cho $ h < f_i(a) \leq g(a) $, và một lân cận $ V $ của $ a $ sao cho $ h < f_i(x) $ với mọi $ x \in V $; do đó $ a $ fortiori $ h < g(x) $ với mọi $ x \in V $.

Suy ra từ Mệnh đề 2 rằng bao dưới của một số hữu hạn các hàm nửa liên tục dưới vẫn lại là nửa liên tục dưới; nhưng điều này nói chung không đúng đối với bao dưới của một họ vô hạn các hàm nửa liên tục dưới. Chẳng hạn, nếu $ r $ là một số hữu tỉ bất kỳ, gọi $ f_r $ là hàm bằng 0 tại $ r $ và bằng 1 với mọi số thực $ x \neq r $; bao dưới của các $ f_r $ là hàm $ g $ bằng 0 với mọi số hữu tỉ và bằng 1 với mọi số vô tỉ ("hàm Dirichlet"), và hàm này không nửa liên tục dưới tại các điểm vô tỉ.

#### Hệ quả {#top-iv-s6-n2-cor-3 .statement}

Bao trên của một họ các hàm thực liên tục trên một không gian $ X $ là nửa liên tục dưới trên $ X $.

Trong Chương IX, § 1, no. 6, Mệnh đề 5, chúng ta sẽ chỉ ra rằng mệnh đề đảo lại của mệnh đề này là đúng nếu $ X $ là khả đều hóa (và chỉ trong trường hợp này): mọi hàm nửa liên tục dưới trên một không gian khả đều hóa đều là bao trên của một họ các hàm liên tục.

#### Mệnh đề 3 {#top-iv-s6-prop-3 .statement}

*Một hàm thực f, xác định trên một không gian tôpô X, là nửa liên tục dưới tại một điểm $ a \in X $ khi và chỉ khi* $ \liminf_{x \to a} f(x) = f(a) $ [hay, tương đương, khi và chỉ khi $ \liminf_{x \to a} f(x) \geq f(a) $].

Điều kiện này là *cần*. Thật vậy, với mọi $ h < f(a) $, tồn tại một lân cận V của $ a $ sao cho $ h < f(x) $ với mọi $ x \in V $; do đó
$$
h \leq \inf_{x \in V} f(x) \leq \liminf_{x \to a} f(x)
$$
(§ 5, no. 6, các công thức (12)), và vì thế $ f(a) \leq \liminf_{x \to a} f(x) $. Điều kiện này là *đủ*; vì nếu nó được thỏa mãn, thì với mỗi $ h < f(a) $ tồn tại một lân cận V của $ a $ sao cho $ h \leq \inf_{x \in V} f(x) $, và do đó $ f $ là nửa liên tục dưới tại $ a $.

#### Mệnh đề 4 {#top-iv-s6-prop-4 .statement}

*Cho f là một hàm nhận giá trị thực bất kỳ xác định trên một tập con trù mật A của một không gian tôpô X. Nếu, với mỗi $ x \in X $, ta đặt* $ g(x) = \liminf_{y \to x, y \in A} f(y) $, *thì g là nửa liên tục dưới trên X*.

Thật vậy, với mọi $ h < g(x) $, tồn tại một lân cận *mở* V của $ x $ sao cho, với mọi $ z \in V \cap A $, ta có $ h < f(z) $; mà V là một lân cận của mỗi điểm $ y $ của nó; do đó ta có $ \liminf_{z \to y, z \in A} f(z) = g(y) \geq h $ với mọi $ y \in V $, và kết quả suy ra.

Hàm $ g $ được gọi là *chính quy hóa nửa liên tục dưới* của $ f $. Ta định nghĩa *chính quy hóa nửa liên tục trên* của $ f $ một cách tương tự.

Ta cũng có thể định nghĩa $ g $ là hàm *lớn nhất* trong các hàm nửa liên tục dưới $ \varphi $ trên X sao cho $ \varphi(x) \leq f(x) $ với mọi $ x \in A $. Nếu $ f $ là *nửa liên tục dưới* trên A, thì $ g $ là một *mở rộng* của $ f $ lên X, theo Mệnh đề 3.

### Bài tập {#top-iv-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
