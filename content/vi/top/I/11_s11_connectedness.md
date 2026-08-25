---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 11
section_title: Connectedness
lang: vi
source: top-i-iv
pdf_pages: 0113-0122, 0161-0167
extraction: ocr
subsections:
    - "no": 1
      title: CONNECTED SPACES AND CONNECTED SETS
      page: 0
      pdf_page: 113
    - "no": 2
      title: IMAGE OF A CONNECTED SET UNDER A CONTINUOUS MAPPING
      page: 0
      pdf_page: 115
    - "no": 3
      title: QUOTIENT SPACES OF A CONNECTED SPACE
      page: 0
      pdf_page: 116
    - "no": 4
      title: PRODUCT OF CONNECTED SPACES
      page: 0
      pdf_page: 116
    - "no": 5
      title: COMPONENTS
      page: 0
      pdf_page: 116
    - "no": 6
      title: LOCALLY CONNECTED SPACES
      page: 0
      pdf_page: 118
    - "no": 7
      title: 'APPLICATION : THE POINCARÉ-VOLTERRA THEOREM'
      page: 0
      pdf_page: 120
statements: 28
exercises: 25
content_sha256: 260b9541a2c2dcad64b2be8f9b476faafc43d460ff7401b432edf12a7da664cc
translated_from: content/en/top/I/11_s11_connectedness.md
source_content_sha256: 49e623cd592377d1f90b814606ff58adaeff059b1eb51901b6753b81790419ce
translation_model: gpt-5-6
translation_run: translate-vi-a6bc2cb7
glossary_version: 34
glossary_terms_sha256: 9b534be55d8d9fab2b4309b0d7cadbee2a337f6b52510c41550a3009b5ec8071
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 11. TÍNH LIÊN THÔNG

### 1. CÁC KHÔNG GIAN LIÊN THÔNG VÀ CÁC TẬP LIÊN THÔNG

#### Định nghĩa 1 {#top-i-s11-def-1 .statement}

Một không gian tôpô X được gọi là liên thông nếu nó không là hợp của hai tập mở rời nhau khác rỗng.

Một định nghĩa tương đương thu được bằng cách thay thế các từ "tập mở" bởi "tập đóng". X liên thông khi và chỉ khi các tập con duy nhất của X vừa mở vừa đóng là tập rỗng và toàn bộ không gian X.

Nếu X liên thông và nếu A, B là hai tập con mở (tương ứng, đóng) khác rỗng sao cho A \cup B = X, thì A \cap B \neq \emptyset.

#### Ví dụ 1 {#top-i-s11-n1-exa-1 .statement}

Ta sẽ thấy trong Chương IV, § 2, no. 5 rằng đường thẳng thực là liên thông, còn đường thẳng hữu tỉ thì không. \*
2) Một không gian rời rạc có nhiều hơn một điểm thì không liên thông.

#### Định nghĩa 2 {#top-i-s11-def-2 .statement}

*Một tập con $ A $ của một không gian tôpô $ X $ được gọi là một tập liên thông nếu không gian con $ A $ của $ X $ là liên thông.*

Để $ A $ là một tập con liên thông của $ X $ thì điều kiện cần và đủ là, đối với mỗi phủ của $ A $ bởi hai tập con mở (hoặc đóng) $ B, C $ của $ X $ sao cho $ A \cap B $ và $ A \cap C $ là khác rỗng, ta có $ A \cap B \cap C \neq \emptyset $.

#### Ví dụ {#top-i-s11-n1-exa-2 .statement}

Trong mọi không gian tôpô, tập rỗng và mọi tập hợp gồm một điểm duy nhất đều liên thông. Trong một không gian Hausdorff $ X $, mọi tập hữu hạn gồm nhiều hơn một điểm đều không liên thông, và nói chung mọi tập con của $ X $ có nhiều hơn một điểm và có ít nhất một điểm cô lập đều không liên thông.

Nếu một tập con trù mật $ A $ là liên thông, thì toàn bộ không gian $ X $ là liên thông; nếu không, sẽ tồn tại hai tập con mở rời nhau khác rỗng $ M, N $ của $ X $ sao cho $ M \cup N = X $, và $ M \cap A, N \cap A $ sẽ là hai tập con mở rời nhau khác rỗng của $ A $ có hợp là $ A $. Do đó ta có

#### Mệnh đề 1 {#top-i-s11-prop-1 .statement}

*Nếu $ A $ là một tập liên thông, thì mọi tập hợp $ B $ sao cho $ A \subset B \subset \overline{A} $ là liên thông.*

#### Mệnh đề 2 {#top-i-s11-prop-2 .statement}

*Hợp của một họ các tập liên thông có giao khác rỗng là liên thông.*

Cho $ (A_i)_{i \in I} $ là một họ các tập con liên thông của $ X $, tất cả đều chứa cùng một điểm $ x $; ta phải chỉ ra rằng

$$
A = \bigcup_i A_i
$$

là liên thông. Nếu không, tồn tại hai tập mở $ B $ và $ C $ sao cho $ B \cap A $ và $ C \cap A $ là khác rỗng, và $ A \subset B \cup C $ và $ A \cap B \cap C = \emptyset $. $ x $ thuộc một trong các tập $ B, C $, giả sử $ x \in B $; mặt khác một trong các tập $ A_i $, giả sử $ A_x $, gặp $ C $; do đó ta có $ A_x \subset B \cup C $, $ A_x \cap B \cap C = \emptyset $ và $ B \cap A_x $ và $ C \cap A_x $ là khác rỗng. Vậy $ A_x $ không liên thông, điều này mâu thuẫn.

#### Hệ quả {#top-i-s11-n1-cor-1 .statement}

*Cho $ (A_n)_{n \geq 0} $ là một dãy vô hạn các tập liên thông sao cho $ A_{n+1} \cap A_n \neq \emptyset $ với mọi $ n \geq 0 $. Khi đó hợp $ \bigcup_{n=0}^\infty A_n $ là liên thông.*

Bằng quy nạp theo $ n $ ta thấy ngay lập tức rằng tập hợp $ B_n = \bigcup_{i=0}^n A_i $ là liên thông với mọi $ n $, theo Mệnh đề 2. Các tập hợp $ B_n $ có giao khác rỗng; do đó hợp của chúng, bằng $ \bigcup_{n=0}^\infty A_n $, là liên thông theo Mệnh đề 2.

#### Mệnh đề 3 {#top-i-s11-prop-3 .statement}

*Cho $ A $ là một tập con của một không gian tôpô $ X $. Nếu $ B $ là một tập con liên thông của $ X $ gặp cả $ A $ và $ \complement A $, thì $ B $ gặp biên của $ A $.*

Nếu không, các giao của $ B $ với phần trong và phần ngoài của $ A $ sẽ là hai tập con mở của $ B $ lập thành một phân hoạch của $ B $, và $ B $ sẽ không liên thông.

#### Hệ quả {#top-i-s11-n1-cor-2 .statement}

*Trong một không gian liên thông $ X $, mọi tập hợp không rỗng khác $ X $ đều có ít nhất một điểm biên.*

### 2. ẢNH CỦA MỘT TẬP HỢP LIÊN THÔNG QUA MỘT ÁNH XẠ LIÊN TỤC

#### Mệnh đề 4 {#top-i-s11-prop-4 .statement}

*Cho $ A $ là một tập con liên thông của một không gian tôpô $ X $, và cho $ f $ là một ánh xạ liên tục từ $ X $ vào một không gian tôpô $ X' $. Khi đó $ f(A) $ là liên thông.*

Giả sử $ f(A) $ không liên thông. Khi đó tồn tại hai tập hợp $ M', N' $ mở trong $ f^{-1}(A) $ và lập thành một phân hoạch của $ f(A) $; do đó $ A \cap f^{-1}(M') $ và $ A \cap f^{-1}(N') $ là mở trong $ A $ và lập thành một phân hoạch của $ A $; điều này mâu thuẫn với giả thiết rằng $ A $ liên thông.

*Ảnh ngược* của một tập hợp liên thông qua một ánh xạ liên tục không nhất thiết là liên thông; xét ví dụ một ánh xạ từ một không gian rời rạc vào một không gian gồm một điểm.

Từ Mệnh đề 4 ta suy ra một đặc trưng hóa khác của *các không gian không liên thông*:

#### Mệnh đề 5 {#top-i-s11-prop-5 .statement}

*Để một không gian tôpô $ X $ không liên thông, điều kiện cần và đủ là tồn tại một ánh xạ liên tục toàn ánh từ $ X $ lên một không gian rời rạc chứa nhiều hơn một điểm.*

Điều kiện này là đủ theo Mệnh đề 4. Ngược lại, nếu $ X $ không liên thông, tồn tại hai tập con mở rời nhau không rỗng $ A, B $ có hợp là $ X $, và ánh xạ $ f $ từ $ X $ lên một không gian rời rạc gồm hai phần tử $ \{a, b\} $, được xác định bởi $ f(A) = \{a\} $ và $ f(B) = \{b\} $, là liên tục.

### 3. CÁC KHÔNG GIAN THƯƠNG CỦA MỘT KHÔNG GIAN LIÊN THÔNG

#### Mệnh đề 6 {#top-i-s11-prop-6 .statement}

Mọi không gian thương của một không gian liên thông đều liên thông.

Đây là một hệ quả ngay lập tức của Mệnh đề 4 của no. 2.

#### Mệnh đề 7 {#top-i-s11-prop-7 .statement}

Cho $ X $ là một không gian tôpô và $ R $ là một quan hệ tương đương trên $ X $. Nếu không gian thương $ X/R $ liên thông, và nếu mỗi lớp tương đương mod $ R $ là liên thông, thì $ X $ liên thông.

Giả sử $ X $ không liên thông. Khi đó có một phân hoạch của $ X $ thành hai tập mở $ A, B $. Các tập $ A, B $ là bão hòa đối với $ R $; vì nếu $ x \in A $ thì lớp tương đương $ M $ của $ x $ không thể gặp $ B $, nếu không các tập $ A \cap M, B \cap M $ sẽ tạo thành một phân hoạch của $ M $ thành hai tập mở trong $ M $, điều này là không thể vì $ M $ liên thông. Các ảnh chính tắc của $ A $ và $ B $ do đó là các tập mở trong $ X/R $ và tạo thành một phân hoạch của $ X/R $; điều này mâu thuẫn với giả thiết rằng $ X/R $ liên thông.

### 4. TÍCH CỦA CÁC KHÔNG GIAN LIÊN THÔNG

#### Mệnh đề 8 {#top-i-s11-prop-8 .statement}

Mọi tích của các không gian liên thông đều liên thông. Ngược lại, nếu một tích của các không gian khác rỗng là liên thông, thì mỗi không gian nhân tử đều liên thông.

Cho $ X = \prod_{i \in I} X_i $ là một tích của các không gian tôpô. Nếu các $ X_i $ khác rỗng, ta có $ X_i = \operatorname{pr}_i X $ với mỗi $ i \in I $; do đó nếu $ X $ liên thông thì các $ X_i $ cũng liên thông (no. 2, Mệnh đề 4). Ngược lại, giả sử rằng mỗi $ X_i $ liên thông và $ X $ không liên thông. Theo Mệnh đề 5 của no. 2, tồn tại một ánh xạ toàn ánh liên tục $ f : X \to X' $, trong đó $ X' $ là một không gian rời rạc chứa nhiều hơn một điểm. Cho $ a = (a_i) $ là một điểm bất kỳ của $ X $, và $ x $ là một chỉ số bất kỳ; ánh xạ từng phần $ f_x : X_x \to X' $, được xác định bởi $ f_x(x) = f((y_i)) $ trong đó $ y_x = x $ và $ y_i = a_i $ nếu $ i \neq x $, là liên tục trên $ X_x $; vì $ X_x $ liên thông, $ f_x $ phải là hằng trên $ X_x $. Suy ra ngay lập tức bằng quy nạp rằng $ f(x) = f(a) $ đối với mọi điểm $ x = (x_i) $ sao cho $ x_i = a_i $ với mọi chỉ số $ i \in I $ trừ một số hữu hạn. Nhưng các điểm $ x $ này tạo thành một tập con trù mật của $ X $ (\S 4, no. 3, Mệnh đề 8). Do đó $ f $ liên tục trên $ X $ và hằng trên một tập con trù mật của $ X $, và vì vậy hằng trên $ X $ (\S 8, no. 1, Mệnh đề 2, Hệ quả 1). Nhưng điều này mâu thuẫn với định nghĩa của $ f $.

### 5. CÁC THÀNH PHẦN

Cho một điểm $ x $ của một không gian tôpô $ X $, hợp của các tập con liên thông của $ X $ chứa $ x $ là liên thông (no. 1, Mệnh đề 2); do đó nó là tập con liên thông lớn nhất của $ X $ whi chứa $ x $.

#### Định nghĩa 3 {#top-i-s11-def-3 .statement}
