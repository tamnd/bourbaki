---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 2
section_title: Uniformly continuous functions
lang: vi
source: top-i-iv
pdf_pages: 0180-0187, 0213-0214
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMLY CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 180
    - "no": 2
      title: COMPARISON OF UNIFORMITIES
      page: 0
      pdf_page: 181
    - "no": 3
      title: INITIAL UNIFORMITIES
      page: 0
      pdf_page: 182
    - "no": 4
      title: INVERSE IMAGE OF A UNIFORMITY; UNIFORM SUBSPACES
      page: 0
      pdf_page: 183
    - "no": 5
      title: LEAST UPPER BOUND OF A SET OF UNIFORMITIES
      page: 0
      pdf_page: 184
    - "no": 6
      title: PRODUCT OF UNIFORM SPACES
      page: 0
      pdf_page: 185
    - "no": 7
      title: INVERSE LIMITS OF UNIFORM SPACES
      page: 0
      pdf_page: 186
statements: 25
exercises: 6
content_sha256: dfbc9ab72bd32bcff9c23d502791233d3c78cb072c21bfacc8548e4cea42d531
translated_from: content/en/top/II/02_s2_uniformly_continuous_functions.md
source_content_sha256: dfab39c7f29bdf3cc9ab6822358b2235321a2a2e044ac8be660b8a71a747aac7
translation_model: gpt-5.4, copied
translation_run: translate-vi-88ee14c1
glossary_version: 34
glossary_terms_sha256: 8d0fcedb1fb8b5ea59e98a8247996d7f11effad38e113a0b7d177a88698a5d62
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC ÁNH XẠ LIÊN TỤC ĐỀU

### 1. CÁC ÁNH XẠ LIÊN TỤC ĐỀU

#### Định nghĩa 1 {#top-ii-s2-def-1 .statement}

*Một ánh xạ $ f $ từ một không gian đều $ X $ vào một không gian đều $ X' $ được gọi là liên tục đều nếu, với mỗi entourage $ V' $ của $ X' $, tồn tại một entourage $ V $ của $ X $ sao cho quan hệ $ (x, y) \in V $ kéo theo $ (f(x), f(y)) \in V' $.*

Nói một cách diễn đạt hơn, ta có thể nói rằng $ f $ là liên tục đều nếu $ f(x) $ và $ f(y) $ gần nhau tùy ý mỗi khi $ x $ và $ y $ đủ gần nhau.

Nếu ta đặt $ g = f \times f $, thì Định nghĩa 1 có nghĩa là *mỗi khi $ V' $ là một entourage của $ X' $, thì $ \overline{g^{-1}}(V') $ là một entourage của $ X $*.

#### Ví dụ 1 {#top-ii-s2-n1-exa-1 .statement}

Ánh xạ đồng nhất của một không gian đều vào chính nó là liên tục đều.
2) Một ánh xạ hằng từ một không gian đều vào một không gian đều là liên tục đều.
3) Mọi ánh xạ từ một không gian đều rời rạc vào một không gian đều đều là liên tục đều.

#### Mệnh đề 1 {#top-ii-s2-prop-1 .statement}

Mọi ánh xạ liên tục đều đều là liên tục.

Đây là một hệ quả ngay lập tức của các định nghĩa.

Mặt khác, một ánh xạ liên tục từ một không gian đều X vào một không gian đều X' không nhất thiết là liên tục đều, \* như được chỉ ra bởi ví dụ $ x \to x^3 $, một đồng phôi của $ \mathbf{R} $ lên chính nó, không liên tục đều đối với cấu trúc đều cộng tính. \* (Xem § 4, no. 1, Định lý 2.)

#### Mệnh đề 2 {#top-ii-s2-prop-2 .statement}

(a) Nếu $ f : X \to X' $ và $ g : X' \to X'' $ là hai ánh xạ liên tục đều, thì $ g \circ f : X \to X'' $ là liên tục đều.

(b) Một song ánh $ f $ từ một không gian đều X lên một không gian đều X' là một đẳng cấu khi và chỉ khi $ f $ và ánh xạ nghịch đảo của $ f $ là liên tục đều.

Điều này suy ra ngay lập tức từ cách giải thích Định nghĩa 1 theo ánh xạ tích $ f \times f $.

### 2. SO SÁNH CÁC CẤU TRÚC ĐỀU

Mệnh đề 2 của no. 1 cho thấy rằng ta có thể lấy các ánh xạ liên tục đều làm các cấu xạ của các cấu trúc đều (Lý thuyết tập hợp, Chương IV, § 2, no. 1); từ nay về sau, ta sẽ luôn giả sử rằng các cấu xạ đã được chọn như vậy. Phù hợp với các định nghĩa tổng quát (Lý thuyết tập hợp, Chương IV, § 2, no. 2), điều này cho phép ta định nghĩa một quan hệ thứ tự trên tập hợp các cấu trúc đều trên một tập hợp X đã cho:

#### Định nghĩa 2 {#top-ii-s2-def-2 .statement}

Nếu $ \mathcal{U}_1 $ và $ \mathcal{U}_2 $ là hai cấu trúc đều trên cùng một tập hợp X, thì nói rằng $ \mathcal{U}_1 $ mịn hơn $ \mathcal{U}_2 $ (và $ \mathcal{U}_2 $ thô hơn $ \mathcal{U}_1 $) nếu, ký hiệu bởi $ X_i $ tập hợp X được trang bị cấu trúc đều $ \mathcal{U}_i $ ($ i = 1,2 $), thì ánh xạ đồng nhất $ X_1 \to X_2 $ là liên tục đều.

Nếu $ \mathcal{U}_1 $ mịn hơn $ \mathcal{U}_2 $ và phân biệt với $ \mathcal{U}_2 $, ta nói rằng $ \mathcal{U}_1 $ mịn hơn hẳn $ \mathcal{U}_2 $ (và rằng $ \mathcal{U}_2 $ thô hơn hẳn $ \mathcal{U}_1 $).

Hai cấu trúc đều được gọi là so sánh được nếu một trong hai mịn hơn cấu trúc kia.

#### Ví dụ {#top-ii-s2-n2-exa-1 .statement}

Trong tập hợp có thứ tự các cấu trúc đều trên một tập hợp X, cấu trúc đều rời rạc là mịn nhất, và cấu trúc đều thô nhất là cấu trúc mà tập hợp các entourage chỉ gồm một phần tử duy nhất $ X \times X $.

Mệnh đề sau là một hệ quả ngay lập tức của Định nghĩa 1 của no. 1:

#### Mệnh đề 3 {#top-ii-s2-prop-3 .statement}

Nếu $ \mathcal{U}_1 $ và $ \mathcal{U}_2 $ là hai cấu trúc đều trên một tập hợp X, thì $ \mathcal{U}_1 $ mịn hơn $ \mathcal{U}_2 $ khi và chỉ khi mọi entourage của $ \mathcal{U}_2 $ đều là một entourage của $ \mathcal{U}_1 $.

#### Hệ quả {#top-ii-s2-n2-cor-1 .statement}

Cho $ \mathcal{U}_1 $ và $ \mathcal{U}_2 $ là hai cấu trúc đều trên một tập hợp X, và giả sử rằng $ \mathcal{U}_1 $ mịn hơn $ \mathcal{U}_2 $; khi đó tôpô cảm sinh bởi $ \mathcal{U}_1 $ mịn hơn tôpô cảm sinh bởi $ \mathcal{U}_2 $.

#### Nhận xét 1 {#top-ii-s2-n2-rem-1 .statement}

Có thể xảy ra trường hợp một cấu trúc đều $ \mathcal{U}_1 $ mịn hơn nghiêm ngặt một cấu trúc đều $ \mathcal{U}_2 $ nhưng hai tôpô cảm sinh là đồng nhất. Ví dụ sau cho thấy điều đó:

Cho $ X $ là một tập hợp không rỗng. Với mỗi phân hoạch hữu hạn $ \varpi = (A_i)_{1 \leq i \leq n} $ của $ X $, ký hiệu $ V_{\overline{\varpi}} $ là
$$
\bigcup_i A_i \times A_i.
$$
Khi đó các tập hợp $ V_{\overline{\varpi}} $ tạo thành một hệ cơ bản các lân cận của một cấu trúc đều $ \mathcal{U} $ trên $ X $. Thật vậy, nếu $ \varpi $ là một phân hoạch hữu hạn bất kỳ của $ X $ thì ta có $ \Delta \subset V_{\overline{\varpi}} $ và $ V_{\overline{\varpi}} \circ V_{\overline{\varpi}} = \overline{V_{\overline{\varpi}}} = V_{\overline{\varpi}} $ (\S 1, no. 1, Ví dụ 2); và nếu $ \varpi' = (B_j) $ và $ \varpi'' = (C_k) $ là hai phân hoạch hữu hạn của $ X $, thì những tập hợp trong số các tập $ B_j \cap C_k $ không rỗng tạo thành một phân hoạch hữu hạn $ \varpi $ của $ X $, và ta có $ V_{\overline{\varpi}} \subset V_{\overline{\varpi'}} \cap V_{\overline{\varpi''}} $. $ \mathcal{U} $ được gọi là cấu trúc đều của các phân hoạch hữu hạn trên $ X $. Tôpô cảm sinh bởi $ \mathcal{U} $ là tôpô rời rạc, vì với mỗi $ x \in X $ các tập hợp $ \{x\} $ và $ C\{x\} $ tạo thành một phân hoạch hữu hạn của $ X $. Tuy nhiên, nếu $ X $ là vô hạn, thì hiển nhiên $ \mathcal{U} $ thô hơn thực sự so với cấu trúc đều rời rạc.

#### Nhận xét 2 {#top-ii-s2-n2-rem-2 .statement}

Nếu $ f : X \to X' $ là một ánh xạ liên tục đều, thì $ f $ vẫn liên tục đều nếu ta thay thế cấu trúc đều của $ X $ bằng một cấu trúc đều mịn hơn và cấu trúc đều của $ X' $ bằng một cấu trúc đều thô hơn (no. 1, Mệnh đề 2). Nói cách khác, cấu trúc đều của $ X $ càng mịn và cấu trúc đều của $ X' $ càng thô thì càng có nhiều ánh xạ liên tục đều từ $ X $ vào $ X' $.

### 3. CẤU TRÚC ĐỀU BAN ĐẦU

#### Mệnh đề 4 {#top-ii-s2-prop-4 .statement}

Cho $ X $ là một tập hợp, cho $ (Y_i)_{i \in I} $ là một họ các không gian đều, và với mỗi $ i \in I $ cho $ f_i $ là một ánh xạ từ $ X $ vào $ Y_i $. Với mỗi $ i \in I $ gọi $ g_i $ là $ f_i \times f_i $. Cho $ \mathfrak{S} $ là tập hợp các tập con của $ X \times X $ có dạng $ \overline{g_i}(V_i) $, trong đó $ i \in I $ và $ V_i $ là một lân cận đều của $ Y_i $, và cho $ \mathcal{B} $ là tập hợp mọi giao hữu hạn

$$
\text{(1)} \quad U(V_{i_1}, \ldots, V_{i_n}) = \overline{g_{i_1}}(V_{i_1}) \cap \cdots \cap \overline{g_{i_n}}(V_{i_n})
$$

của các tập hợp của $ \mathfrak{S} $. Khi đó $ \mathcal{B} $ là một hệ cơ bản các entourage của một cấu trúc đều $ \mathcal{U} $ trên $ X $; cấu trúc này là cấu trúc đều ban đầu trên $ X $ đối với họ $ (f_i) $ (Lý thuyết tập hợp, Chương IV, § 2, no. 3), và đặc biệt $ \mathcal{U} $ là cấu trúc đều thô nhất trên $ X $ mà đối với nó mọi ánh xạ $ f_i $ đều liên tục đều. Mặt khác, nếu $ h $ là một ánh xạ từ một không gian đều $ Z $ vào $ X $ thì $ h $ liên tục đều (khi $ X $ được trang bị cấu trúc đều $ \mathcal{U} $) nếu và chỉ nếu mỗi ánh xạ $ f_i \circ h $ đều liên tục đều.

Ta thấy ngay lập tức rằng $ \mathcal{B} $ thỏa mãn các tiên đề $(B_1)$ và $(U'_1)$. Nếu $ W_i = \overline{g}_i^{-1}(V_i) $, thì $ \overline{W}_i = \overline{g}_i^{-1}(\overline{V}_i) $ và $ \dot{W}_i = \dot{g}_i^{-1}(\dot{V}_i) $; do đó $ \mathcal{B} $ cũng thỏa mãn các tiên đề $(U'_{II})$ và $(U'_{III})$ và vì thế là một hệ cơ bản các entourage của một cấu trúc đều $ \mathcal{U} $ trên $ X $. Hơn nữa, từ định nghĩa của $ \mathcal{U} $ và Định nghĩa 1 và no. 1, suy ra ngay lập tức rằng $ f_i $ là liên tục đều với mỗi chỉ số $ i \in I $; do đó (no. 1, Mệnh đề 2) $ f_i \circ h $ là liên tục đều với mỗi $ i \in I $ nếu $ h $ là như vậy. Ngược lại, giả sử rằng $ f_i \circ h $ là liên tục đều với mỗi $ i \in I $, và xét một tập hợp $ U(V_{i_1}, \ldots, V_{i_n}) $; theo giả thiết, với mỗi $ k $ sao cho $ 1 \leq k \leq n $, có một entourage $ W_k $ của $ Z $ sao cho quan hệ $ (z, z') \in W_k $ kéo theo $ [f_{i_k}(h(z)), f_{i_k}(h(z'))] \in V_k $; nếu
$$
W = \bigcap_k W_k,
$$
thì đồng thời $ n $ quan hệ này được thỏa mãn mỗi khi $ z $ và $ z' $ là $ W $-gần, nên khi đó ta có $ (h(z), h(z')) \in U(V_{i_1}, \ldots, V_{i_n}) $, và chứng minh là đầy đủ.

#### Hệ quả {#top-ii-s2-n3-cor-1 .statement}

*Tôpô trên $ X $ được cảm sinh bởi cấu trúc đều thô nhất $ \mathcal{U} $ sao cho các $ f_i $ là liên tục đều cũng là tôpô thô nhất sao cho các $ f_i $ là liên tục.*

Đây là một hệ quả ngay lập tức của định nghĩa các lân cận của một điểm trong tôpô sau này (Chương I, § 2, no. 3, Mệnh đề 4).

Các tính chất tổng quát của các cấu trúc ban đầu (*Lý thuyết tập hợp*, Chương IV, § 2, no. 3, tiêu chuẩn CST 10) đặc biệt suy ra tính chất *bắc cầu* sau đây:

#### Mệnh đề 5 {#top-ii-s2-prop-5 .statement}

*Cho $ X $ là một tập hợp, cho $ (Z_i)_{i \in I} $ là một họ các không gian đều, cho $ (J_\lambda)_{\lambda \in L} $ là một phân hoạch của $ I $ và cho $ (Y_\lambda)_{\lambda \in L} $ là một họ các tập hợp được đánh chỉ số bởi $ L $. Với mỗi $ \lambda \in L $, cho $ h_\lambda $ là một ánh xạ từ $ X $ vào $ Y_\lambda $; với mỗi $ \lambda \in L $ và mỗi $ i \in J_\lambda $, cho $ g_{i\lambda} $ là một ánh xạ từ $ Y_\lambda $ vào $ Z_i $; và đặt $ f_i = g_{i\lambda} \circ h_\lambda $. Trang bị cho mỗi $ Y_\lambda $ cấu trúc đều thô nhất sao cho các ánh xạ $ g_{i\lambda} $ ($ i \in J_\lambda $) là liên tục đều. Khi đó cấu trúc đều thô nhất trên $ X $ sao cho các $ f_i $ là liên tục đều trùng với cấu trúc đều thô nhất trên $ X $ sao cho các $ h_\lambda $ là liên tục đều.*

### 4. ẢNH NGƯỢC CỦA MỘT CẤU TRÚC ĐỒNG ĐỀU; CÁC KHÔNG GIAN CON ĐỒNG ĐỀU

Cho $ X $ là một tập hợp, $ Y $ là một không gian đều, $ f $ là một ánh xạ từ $ X $ vào $ Y $. Cấu trúc đều thô nhất $ \mathcal{U} $ trên $ X $ mà đối với nó $ f $ là liên tục đều được gọi là *ảnh ngược* theo $ f $ của cấu trúc đều của $ Y $. Suy ra từ Mệnh đề 4 của no. 3, và từ các công thức cho ảnh ngược của một giao, rằng các ảnh ngược theo $ g = f \times f $ của các lân cận của đường chéo của $ Y $ tạo thành một hệ cơ bản các lân cận của đường chéo đối với $ \mathcal{U} $. Tôpô cảm sinh bởi $ \mathcal{U} $ là *ảnh ngược* theo $ f $ của tôpô của $ Y $ (no. 3, Hệ quả của Mệnh đề 4).

#### Nhận xét {#top-ii-s2-n4-rem-1 .statement}

Nếu $ f : X \to Y $ là toàn ánh, thì các entourage của $ Y $ là các ảnh trực tiếp dưới $ g $ của các entourage của $ X $.

Một ánh xạ $ f $ từ một không gian đều $ X $ vào một không gian đều $ X' $ là liên tục đều nếu và chỉ nếu ảnh ngược dưới $ f $ của cấu trúc đều của $ X' $ thô hơn cấu trúc đều của $ X $.

Cho $ A $ là một tập con của một không gian đều $ X $. Cấu trúc đều cảm sinh trên $ A $ bởi cấu trúc đều của $ X $ là ảnh ngược của cấu trúc sau dưới đơn ánh chính tắc $ A \to X $. Theo Mệnh đề 4 của no. 3, điều này tương đương với định nghĩa sau:

#### Định nghĩa 3 {#top-ii-s2-def-3 .statement}

Cho $ A $ là một tập con của một không gian đều $ X $. Cấu trúc đều trên $ A $ mà tập các lân cận đều của nó là vết trên $ A \times A $ của tập các lân cận đều của $ X $ được gọi là cấu trúc đều cảm sinh trên $ A $ bởi cấu trúc đều của $ X $.

Tôpô cảm sinh bởi cấu trúc đều cảm sinh trên $ A $ trùng với tôpô cảm sinh trên $ A $ bởi tôpô của $ X $; tập $ A $, cùng với cấu trúc đều và tôpô cảm sinh bởi các cấu trúc tương ứng của $ X $, được gọi là một không gian con đều của $ X $.

Nếu $ A $ là một tập con của một không gian đều $ X $ và nếu $ f : X \to X' $ là một ánh xạ liên tục đều, thì hạn chế $ f|A $ là một ánh xạ liên tục đều từ $ A $ vào $ X' $. Nếu $ A' \subset X' $ sao cho $ f(X) \subset A' $, thì ánh xạ từ $ X $ vào không gian con đều $ A' $ của $ X' $, có cùng đồ thị như $ f $, lại cũng liên tục đều (no. 3, Mệnh đề 4).

Nếu $ B \subset A \subset X $, thì không gian con đều $ B $ của $ X $ đồng nhất với không gian con đều $ B $ của không gian con đều $ A $ của $ X $ (tính bắc cầu của các cấu trúc đều cảm sinh; no. 3, Mệnh đề 5).

#### Mệnh đề 6 {#top-ii-s2-prop-6 .statement}

Cho $ A $ là một tập con trù mật của một không gian đều $ X $. Khi đó các bao đóng, trong $ X \times X $, của các lân cận đều của không gian con đều $ A $ tạo thành một hệ cơ bản các lân cận đều của $ X $.

$ A \times A $ trù mật trong $ X \times X $ (Chương I, § 4, no. 3, Mệnh đề 7). Cho $ V $ là một entourage mở của $ A $; đó là giao của $ A \times A $ với một entourage mở $ U $ của $ X $. Ta có $ U \subset \overline{V} $ (Chương I, § 1, no. 6, Mệnh đề 5), và quan hệ này cùng với $ \overline{V} \subset \overline{U} $ chứng minh mệnh đề, theo Hệ quả 2 của Mệnh đề 2 ở § 1, no. 2.

### 5. CẬN TRÊN BÉ NHẤT CỦA MỘT TẬP HỢP CÁC CẤU TRÚC ĐỀU

Mọi họ $ (\mathcal{U}_i)_{i \in I} $ các cấu trúc đều trên một tập hợp $ X $ đều có một cận trên bé nhất $ \mathcal{U} $ trong tập hợp có thứ tự của tất cả các cấu trúc đều trên $ X $; ta chỉ cần áp dụng mệnh đề 4 của no. 3, lấy $ Y_i $ là tập hợp $ X $ được trang bị cấu trúc đều $ \mathcal{U}_i $, và $ f_i $ là ánh xạ đồng nhất $ X \to Y_i $. Tôpô cảm sinh bởi $ \mathcal{U} $ chính là cận trên bé nhất của các tôpô cảm sinh bởi các $ \mathcal{U}_i $.

Cũng suy ra từ Mệnh đề 4 của no. 3 rằng nếu $ X $ không rỗng và nếu $ \mathcal{U}_i $ là bộ lọc các entourage của $ \mathcal{U}_i $, thì bộ lọc các entourage của $ \mathcal{U} $ là cận trên bé nhất của các bộ lọc $ \mathcal{U}_i $ (Chương I, § 6, no. 2).

#### Ví dụ {#top-ii-s2-n5-exa-1 .statement}

Nếu $ \varpi $ là một phân hoạch hữu hạn bất kỳ $ (A_i)_{1 \leq i \leq n} $ của một tập hợp không rỗng $ X $, thì tập hợp $ V_\varpi = \bigcup_i (A_i \times A_i) $ tự nó tạo thành một hệ cơ sở các entourage của một cấu trúc đều $ \mathcal{U}_\varpi $ trên $ X $ (\S 1, no. 1, Ví dụ 2); khi đó cấu trúc đều của các phân hoạch hữu hạn trên $ X $ (no. 2, Nhận xét 1) là cận trên bé nhất của các cấu trúc đều $ \mathcal{U}_\varpi $.

#### Nhận xét {#top-ii-s2-n5-rem-1 .statement}

Một họ $ (\mathcal{U}_i) $ các cấu trúc đều trên $ X $ cũng có một cận dưới lớn nhất trong tập hợp có thứ tự của mọi cấu trúc đều trên $ X $, cụ thể là cận trên nhỏ nhất của tập hợp mọi cấu trúc đều trên $ X $ mà thô hơn từng $ \mathcal{U}_i $ (những cấu trúc đều như vậy có tồn tại, vì tập hợp mọi cấu trúc đều trên $ X $ có một phần tử nhỏ nhất). Nhưng (giả sử $ X $ không rỗng) bộ lọc các lân cận của đường chéo của cấu trúc đều này không nhất thiết là giao của các bộ lọc các lân cận của đường chéo của các $ \mathcal{U}_i $, vì bộ lọc sau này không nhất thiết thỏa mãn tiên đề $ (U_{III}) $ (Bài tập 4).

### 6. TÍCH CỦA CÁC KHÔNG GIAN ĐỀU

#### Định nghĩa 4 {#top-ii-s2-def-4 .statement}

*Nếu* $ (X_i)_{i \in I} $ *là một họ các không gian đều, thì không gian đều tích của họ này là tập hợp tích*
$$
X = \prod_{i \in I} X_i
$$
*được trang bị cấu trúc đều thô nhất sao cho các phép chiếu* $ pr_i : X \to X_i $
*là liên tục đều. Cấu trúc đều này được gọi là tích của các cấu trúc đều của các* $ X_i $, *và các không gian đều* $ X_i $ *được gọi là các thừa số của* $ X $.

Tôpô cảm sinh bởi cấu trúc đều tích trên $ X $ trùng với tích của các tôpô của các $ X_i $ (no. 3, Hệ quả của Mệnh đề 4).

#### Mệnh đề 7 {#top-ii-s2-prop-7 .statement}

*Cho* $ f = (f_i) $ *là một ánh xạ từ một không gian đều* $ Y $ *vào một không gian đều tích* $ X = \prod_{i \in I} X_i $. *Khi đó* $ f $ *liên tục đều khi và chỉ khi mỗi* $ f_i $ *đều liên tục đều*.

Vì $ f_i = pr_i \circ f $, đây là một trường hợp riêng của Mệnh đề 4 của no. 3.

#### Hệ quả {#top-ii-s2-n6-cor-1 .statement}

*Cho* $ (X_i)_{i \in I}, (Y_i)_{i \in I} $ *là hai họ không gian đều được đánh chỉ số bởi cùng một tập* $ I $. *Với mỗi* $ i \in I $, *cho* $ f_i $ *là một ánh xạ từ* $ X_i $ *vào* $ Y_i $. *Nếu mỗi* $ f_i $ *đều liên tục đều, thì ánh xạ tích*
$$
f : (x_i) \to (f_i(x_i)).
$$
*cũng liên tục đều. Ngược lại, nếu các* $ X_i $ *đều không rỗng và* $ f $ *liên tục đều, thì mỗi* $ f_i $ *đều liên tục đều.*

Tiêu chuẩn tổng quát về tính bắc cầu của các cấu trúc đều ban đầu (no. 3, Mệnh đề 5) cho thấy rằng, cũng như đối với tích của các không gian tôpô (Chương I, § 4, no. 1), tích của các không gian đều là kết hợp và mệnh đề sau đây là đúng:

#### Mệnh đề 8 {#top-ii-s2-prop-8 .statement}

*Cho $ X $ là một tập hợp, cho $ (Y_i)_{i \in I} $ là một họ các không gian đều, và với mỗi $ i \in I $ cho $ f_i $ là một ánh xạ từ $ X $ vào $ Y_i $. Gọi $ f $ là ánh xạ $ x \to (f_i(x)) $ từ $ X $ vào $ Y = \prod_{i \in I} Y_i $, và gọi $ U $ là cấu trúc đều thô nhất trên $ X $ mà đối với nó các $ f_i $ là liên tục đều. Khi đó $ U $ là ảnh ngược theo $ f $ của cấu trúc đều cảm sinh trên $ f(X) $ bởi cấu trúc đều tích trên $ Y $.*

#### Hệ quả {#top-ii-s2-n6-cor-2 .statement}

*Với mỗi $ i \in I $, cho $ A_i $ là một không gian con của $ Y_i $. Khi đó cấu trúc đều cảm sinh trên $ A = \prod_{i \in I} A_i $ bởi cấu trúc đều tích trên $ \prod_{i \in I} Y_i $ cũng chính là tích của các cấu trúc đều của các không gian con $ A_i $.*

Ngoài ra, ta thấy ngay lập tức rằng nếu $ X_1, X_2 $ là hai không gian đều và $ a_1 $ là một điểm bất kỳ của $ X_1 $, thì ánh xạ $ x_2 \to (a_1, x_2) $ là một đẳng cấu từ $ X_2 $ lên không gian con $ \{a_1\} \times X_2 $ của $ X_1 \times X_2 $; do đó:

#### Mệnh đề 9 {#top-ii-s2-prop-9 .statement}

*Cho $ f $ là một ánh xạ liên tục đều từ một không gian đều tích $ X_1 \times X_2 $ vào một không gian đều $ Y $; khi đó mọi ánh xạ riêng phần*

$$
x_2 \to f(x_1, x_2)
$$

*của $ X_2 $ vào $ Y $ đều liên tục đều.*

Nói cách khác, một hàm liên tục đều của hai biến thì liên tục đều đối với từng biến một.

\* Ví dụ đã cho trong Chương I, § 4, no. 2, Nhận xét 2, cho thấy đảo lại của mệnh đề này là sai. \*

### 7. GIỚI HẠN NGHỊCH ĐẢO CỦA CÁC KHÔNG GIAN ĐỀU

Cho $ I $ là một tập hợp có thứ tự bộ phận trong đó thứ tự bộ phận được viết là $ \alpha \leq \beta $. Với mỗi $ \alpha \in I $ cho $ X_\alpha $ là một không gian đều, và với mỗi cặp chỉ số $ \alpha, \beta $ sao cho $ \alpha \leq \beta $ cho $ f_{\alpha \beta} $ là một ánh xạ từ $ X_\beta $ vào $ X_\alpha $.

#### Mệnh đề 10 {#top-ii-s2-prop-10 .statement}

Cho $I$ là một tập có hướng, cho $(X_\alpha, f_{\alpha\beta})$ là một hệ ngược các không gian đều được đánh chỉ số bởi $I$, và cho $J$ là một tập con đồng tận của $I$. Với mỗi $\alpha \in I$, gọi $f_\alpha$ là ánh xạ chính tắc từ $X = \varprojlim X_\alpha$ vào $X_\alpha$, và ký hiệu $g_\alpha$ là $f_\alpha \times f_\alpha$. Khi đó họ các tập hợp $\overline{g}_\alpha^{-1}(V_\alpha)$, trong đó $\alpha$ chạy qua $J$ và trong đó, với mỗi $\alpha \in J$, $V_\alpha$ chạy qua một hệ cơ bản các lân cận đều của $X_\alpha$, là một hệ cơ bản các lân cận đều của $X$.

Chúng tôi để lại chứng minh cho bạn đọc; đó là một sự thích nghi trực tiếp của chứng minh của Mệnh đề 9 của Chương I, § 4, no. 4.

Cuối cùng, tôpô trên $X = \varprojlim X_\alpha$ cảm sinh bởi giới hạn ngược của các cấu trúc đều của các $X_\alpha$ là giới hạn ngược của các tôpô của các $X_\alpha$.

### Bài tập {#top-ii-s2-exercises}

Xem [bài tập cho § 2](exercises/s2/).
