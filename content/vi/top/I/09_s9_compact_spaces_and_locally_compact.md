---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 9
section_title: Compact spaces and locally compact spaces
lang: vi
source: top-i-iv
pdf_pages: 0089-0103, 0147-0156
extraction: ocr
subsections:
    - "no": 1
      title: QUASI-COMPACT SPACES AND COMPACT SPACES
      page: 0
      pdf_page: 89
    - "no": 2
      title: REGULARITY OF A COMPACT SPACE
      page: 0
      pdf_page: 91
    - "no": 3
      title: QUASI-COMPACTS SETS; COMPACT SETS; RELATIVELY COMPACT SETS
      page: 0
      pdf_page: 91
    - "no": 4
      title: IMAGE OF A COMPACT SPACE UNDER A CONTINUOUS MAPPING
      page: 0
      pdf_page: 93
    - "no": 5
      title: PRODUCT OF COMPACT SPACES
      page: 0
      pdf_page: 94
    - "no": 6
      title: INVERSE LIMITS OF COMPACT SPACES
      page: 0
      pdf_page: 95
    - "no": 7
      title: LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 96
    - "no": 8
      title: EMBEDDING OF A LOCALLY COMPACT SPACE IN A COMPACT SPACE
      page: 0
      pdf_page: 98
    - "no": 9
      title: LOCALLY COMPACT $ \sigma $-COMPACT SPACES
      page: 0
      pdf_page: 99
    - "no": 10
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 100
statements: 50
exercises: 4
content_sha256: 389d8c1060f073a78c4ce19ca4a47a065ba9ffc31ec3d4a43c015123d669b103
translated_from: content/en/top/I/09_s9_compact_spaces_and_locally_compact.md
source_content_sha256: ea4e6b44516b83eeb3c2d7eac50490f302ca8fe98e1658cd11ee7efac69f4df3
translation_model: gpt-5.4-mini
translation_run: translate-vi-96a7bc15
glossary_version: 34
glossary_terms_sha256: 11590fc32d9c9bdcc7f939c17129c95f39d269867c4b46cba92a3d890752d32f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 9. CÁC KHÔNG GIAN COMPACT VÀ CÁC KHÔNG GIAN COMPACT ĐỊA PHƯƠNG

### 1. CÁC KHÔNG GIAN QUASI-COMPACT VÀ CÁC KHÔNG GIAN COMPACT

#### Định nghĩa 1 {#top-i-s9-def-1 .statement}

*Một không gian tôpô* $ X $ *được gọi là quasi-compact nếu nó thỏa mãn tiên đề sau*:

(C) *Mọi lọc trên* $ X $ *đều có ít nhất một điểm tụ*.

*Một không gian tôpô được gọi là compact nếu nó quasi-compact và Hausdorff*.

Từ tiên đề này suy ra ngay rằng nếu $ f $ là một ánh xạ của một tập hợp $ Z $ vào một không gian quasi-compact $ X $, và $ \mathfrak{F} $ là bất kỳ một lọc nào trên $ Z $, thì $ f $ có ít nhất một điểm tụ đối với $ \mathfrak{F} $. Đặc biệt, mọi dãy điểm của một không gian quasi-compact đều có ít nhất một điểm tụ; nhưng điều kiện này không tương đương với (C) (Bài tập 11).

Ta nêu ba tiên đề, mỗi tiên đề đều *tương đương với tiên đề* (C):

(C') *Mọi siêu lọc trên* $ X $ *đều hội tụ*.

(C') $ \Longrightarrow $ (C): Nếu $ \mathfrak{F} $ là một lọc trên $ X $ thì có một siêu lọc mịn hơn $ \mathfrak{F} $ (\S 6, no. 4, Định lý 1). Vì siêu lọc này hội tụ đến một điểm $ x $, nên $ x $ là một điểm tụ của $ \mathfrak{F} $.

(C) $ \Longrightarrow $ (C'): Vì nếu một siêu lọc có một điểm tụ thì nó hội tụ đến điểm này (\S 7, no. 2, Hệ quả của Mệnh đề 4).

Nếu $ f $ là một ánh xạ của một tập hợp $ Z $ vào một không gian quasi-compact $ X $, và $ \mathfrak{U} $ là một siêu lọc trên $ Z $, thì $ f $ có ít nhất một điểm giới hạn đối với $ \mathfrak{U} $ (\S 6, no. 6, Mệnh đề 10).

(C'') *Mọi họ các tập hợp con đóng của* $ X $ *có giao rỗng đều chứa một họ con hữu hạn có giao rỗng*.

(C) $ \Longrightarrow $ (C''): Giả sử $ \mathcal{G} $ là một họ các tập hợp con đóng của $ X $ có giao rỗng. Nếu mọi họ con hữu hạn của $ \mathcal{G} $ đều có giao khác rỗng, thì $ \mathcal{G} $ sinh ra một lọc (\S 6, no. 2, Mệnh đề 1) và lọc này có một điểm tụ theo giả thiết. Điểm này thuộc mọi tập hợp của $ \mathcal{G} $ (vì chúng đóng); do đó ta có một mâu thuẫn.

$(C'') \implies (C)$: Vì nếu $(C)$ sai thì tồn tại một lọc $ \mathfrak{F} $ trên $ X $ không có điểm tụ; do đó các bao đóng của các tập hợp của $ \mathfrak{F} $ tạo thành một họ các tập hợp con đóng của $ X $ mâu thuẫn với tiên đề $(C'')$.

$(C''')$ (Tiên đề Borel-Lebesgue) *Mọi phủ mở của* $ X $ *đều chứa một phủ mở hữu hạn của* $ X $.

$(C''') \iff (C'')$ bằng cách lấy phần bù.

Nếu $ X $ là quasi-compact, thì mọi *phủ hữu hạn địa phương* $ \mathfrak{R} $ của $ X $ đều *hữu hạn*. Vì mỗi điểm của $ X $ đều có một lân cận mở chỉ giao với một số hữu hạn các tập hợp của $ \mathfrak{R} $, và bởi $(C''')$ thì một số hữu hạn các lân cận này phủ $ X $.

#### Ví dụ 1 {#top-i-s9-n1-exa-1 .statement}

Mọi không gian *hữu hạn* đều *quasi-compact*, và nói chung mọi không gian chỉ có một số hữu hạn các tập hợp mở đều quasi-compact. Một không gian hữu hạn là compact khi và chỉ khi nó rời rạc, vì một không gian Hausdorff hữu hạn là rời rạc ($ \S 8 $, no. 1, Hệ quả của Mệnh đề 3). Ngược lại, *mọi không gian compact rời rạc đều hữu hạn*, vì trong một không gian như vậy các tập hợp gồm một điểm là mở; do đó không gian là hữu hạn bởi $(C''')$.

#### Ví dụ 2 {#top-i-s9-n1-exa-2 .statement}

#### Định lý 1 {#top-i-s9-thm-1 .statement}

*Cho* $ \mathfrak{F} $ *là một bộ lọc trên một không gian quasi-compact* $ X $ *và cho* $ A $ *là tập hợp các điểm tụ của* $ \mathfrak{F} $. *Khi đó mọi lân cận của* $ A $ *đều thuộc* $ \mathfrak{F} $.

Cho $ V $ là một lân cận của $ A $ và giả sử rằng mọi tập hợp của $ \mathfrak{F} $ đều giao với $ \complement V $. Khi đó các giao của những tập hợp của $ \mathfrak{F} $ với $ \complement V $ tạo thành một cơ sở của một bộ lọc $ \mathcal{G} $ trên $ X $; $ X $ là quasi-compact, nên $ \mathcal{G} $ có ít nhất một điểm tụ $ y $, điểm này không thuộc $ A $, vì lân cận $ V $ của $ A $ không giao với một số tập của $ \mathcal{G} $. Nhưng vì $ \mathcal{G} $ mịn hơn $ \mathfrak{F} $, nên $ y $ cũng là một điểm tụ của $ \mathfrak{F} $, trái với giả thiết.

#### Hệ quả {#top-i-s9-n1-cor-1 .statement}

Để một bộ lọc trên một không gian compact hội tụ thì cần và đủ là nó có một điểm tụ duy nhất.

Tính cần thiết theo § 8, no. 1, Mệnh đề 1; tính đủ theo Định lý 1 trên đây.

### 2. TÍNH CHÍNH QUY CỦA MỘT KHÔNG GIAN COMPACT

#### Mệnh đề 1 {#top-i-s9-prop-1 .statement}

Cho $ X $ là một không gian compact, $ x $ là một điểm của $ X $. Để một cơ sở của bộ lọc $ B $ gồm các lân cận đóng của $ x $ là một hệ cơ bản các lân cận của $ x $ thì cần và đủ là giao của các tập của $ B $ chỉ gồm $ x $.

Điều kiện là cần thiết vì $ X $ là Hausdorff (§ 8, no. 1, Mệnh đề 1). Điều đó là đủ, vì nó có nghĩa là $ x $ là điểm tụ duy nhất của $ B $; do đó $ B $ hội tụ về $ x $ theo Hệ quả của Định lý 1 ở no. 1.

#### Hệ quả {#top-i-s9-n2-cor-1 .statement}

Mọi không gian compact đều chính quy.

Vì từ tiên đề (Hi) (§ 8, no. 1, Mệnh đề 1) suy ra rằng cơ sở của bộ lọc được tạo bởi tất cả các lân cận đóng của một điểm tùy ý của không gian thỏa mãn điều kiện của Mệnh đề 1.

Mệnh đề sau làm rõ Hệ quả của Mệnh đề 1:

#### Mệnh đề 2 {#top-i-s9-prop-2 .statement}

Cho $ X $ là một không gian compact và cho $ A $, $ B $ là hai tập con đóng rời nhau của $ X $. Khi đó tồn tại hai tập mở $ U $, $ V $, sao cho $ U \cap V = \varnothing $ và $ A \subset U $ và $ B \subset V $.

Giả sử kết luận là sai. Nếu mọi lân cận $ U $ của $ A $ đều giao với mọi lân cận $ V $ của $ B $, thì các tập $ U \cap V $ tạo thành một cơ sở của bộ lọc $ B $ trên $ X $, do đó có một điểm tụ $ x \in X $. Bây giờ $ x $ phải thuộc $ A $, vì nếu $ y $ là một điểm bất kỳ của $ X $ không thuộc $ A $ thì có một lân cận của $ y $ và một lân cận của $ A $ không giao nhau, vì $ X $ chính quy, và do đó $ y $ không thể là một điểm tụ của $ B $. Tương tự $ x $ phải thuộc $ B $ và ta có một mâu thuẫn.

Mệnh đề này có những hệ quả quan trọng sẽ được xét trong Chương IX, § 4.

Không gian quasi-compact không Hausdorff $ X $ của Ví dụ 2 ở no. 1 không thỏa mãn tiên đề $(O_{III})$, và do đó a fortiori cũng không thỏa mãn tính chất nêu trong Mệnh đề 2, vì bất kỳ hai tập mở không rỗng nào của không gian này luôn giao nhau.

### 3. CÁC TẬP QUASI-COMPACT; CÁC TẬP COMPACT; CÁC TẬP TƯƠNG ĐỐI COMPACT

#### Định nghĩa 2 {#top-i-s9-def-2 .statement}

Một tập con $ A $ của một không gian tôpô $ X $ được gọi là một tập quasi-compact (resp. compact) nếu không gian con $ A $ là quasi-compact (resp. compact).

Một tập con $ A $ của một không gian tôpô $ X $ là một tập quasi-compact khi và chỉ khi mọi phủ của $ A $ bởi *các tập mở của* $ X $ chứa một phủ hữu hạn của $ A $; điều này suy ra từ tiên đề $(C''')$. Trong một không gian Hausdorff, các khái niệm tập quasi-compact và tập compact là như nhau, vì mọi không gian con đều Hausdorff.

#### Ví dụ 1 {#top-i-s9-n3-exa-1 .statement}

Trong một không gian tôpô $ X $, mọi tập con hữu hạn đều quasi-compact; tập rỗng và mọi tập hợp gồm một điểm đều compact.

2) Trong một không gian tôpô $ X $, cho $ (x_n)_{n \in \mathbf{N}} $ là một dãy vô hạn các điểm hội tụ đến một điểm $ a $; khi đó tập $ A $ gồm các điểm $ x_n $ ($ n \in \mathbf{N} $) và $ a $ là quasi-compact. Thật vậy, nếu $ (U_i) $ là một phủ của $ A $ bởi các tập mở của $ X $, thì $ a \in U_x $ với một chỉ số $ x $ nào đó. $ U_x $ là một lân cận của $ a $ và do đó chỉ có một số hữu hạn chỉ số $ n_k $ sao cho $ x_{n_k} \notin U_x $. Với mỗi chỉ số $ k $ cho $ i_k $ là một chỉ số sao cho $ x_{n_k} \in U_{i_k} $; khi đó $ U_x $ và các $ U_{i_k} $ tạo thành một phủ mở hữu hạn của $ A $.

#### Mệnh đề 3 {#top-i-s9-prop-3 .statement}

*Mọi tập con đóng của một không gian quasi-compact* (resp. *compact*) *đều quasi-compact* (resp. *compact*).

Đây là một hệ quả ngay lập tức của tiên đề $(C'')$ nếu ta nhận xét rằng nếu $ A $ đóng trong $ X $ thì mọi tập hợp nào đóng trong $ A $ cũng đóng trong $ X $.

#### Mệnh đề 4 {#top-i-s9-prop-4 .statement}

*Mọi tập con compact của một không gian Hausdorff đều đóng.*

Cho $ A $ là một tập con compact của một không gian Hausdorff $ X $, và cho $ x $ là một điểm bất kỳ của $ \overline{A} $; ta phải chứng minh rằng $ x \in A $. Theo giả thiết, mọi lân cận của $ x $ đều gặp $ A $, và do đó bộ lọc lân cận $ \mathcal{B} $ của $ x $ trong $ X $ gây ra một bộ lọc $ \mathcal{B}_A $ trên $ A $; $ A $ là compact do đó $ \mathcal{B}_A $ có một điểm tụ $ y \in A $. Vì bộ lọc $ \mathcal{B} $ thô hơn bộ lọc trên $ X $ sinh bởi $ \mathcal{B}_A $ (coi như một cơ sở bộ lọc trên $ X $), nên $ y $ cũng là một điểm tụ của $ \mathcal{B} $; do đó $ y = x $, vì $ \mathcal{B} $ hội tụ tới $ x $ trong $ X $ và $ X $ là Hausdorff (\S 8, no. 1, Mệnh đề 1).

#### Hệ quả {#top-i-s9-n3-cor-1 .statement}

*Trong một không gian compact* $ X $ *một tập con* $ A $ *là compact nếu và chỉ nếu nó đóng trong* $ X $.

#### Mệnh đề 5 {#top-i-s9-prop-5 .statement}

*Hợp của một họ hữu hạn các tập con quasi-compact của một không gian tôpô là quasi-compact.*

It is sufficient to show that if $ A $ and $ B $ are two quasi-compact subsets of a topological space $ X $, then $ A \cup B $ is quasi-compact. Let $ \mathcal{R} $ be covering of $ A \cup B $; then $ \mathcal{R} $ is a covering of $ A $ and a covering of $ B $; hence $ \mathcal{R} $ contains a finite covering $ \mathcal{R}_1 $ of $ A $ and a finite covering $ \mathcal{R}_2 $ of $ B $; $ \mathcal{R}_1 \cup \mathcal{R}_2 $ is thus a finite covering of $ A \cup B $ contained in $ \mathcal{R} $.

#### Định nghĩa 3 {#top-i-s9-def-3 .statement}

*Một tập con* $ A $ *của một không gian tôpô* $ X $ *được gọi là tương đối quasi-compact* (resp. *tương đối compact*) *trong* $ X $ *nếu* $ A $ *được chứa trong một tập con quasi-compact* (resp. *compact*) *của* $ X $.

Nói gọn, ta cũng nói rằng $ A $ là một "tập quasi-compact tương đối" (resp. "tập compact tương đối") khi không có sự nhập nhằng nào về $ X $. Trong một không gian *Hausdorff*, các khái niệm tập quasi-compact tương đối và tập compact tương đối là như nhau.

#### Mệnh đề 6 {#top-i-s9-prop-6 .statement}

*Nếu $ X $ là một không gian Hausdorff, thì một tập con $ A $ của $ X $ là tương đối compact khi và chỉ khi $ \overline{A} $ là compact.*

Nếu $ A $ là tương đối compact, thì $ \overline{A} $ compact theo Mệnh đề 4 và hệ quả của nó; chiều ngược lại là hiển nhiên.

#### Mệnh đề 7 {#top-i-s9-prop-7 .statement}

*Nếu $ A $ là một tập con quasi-compact tương đối của một không gian tôpô $ X $, thì mọi cơ sở lọc trên $ A $ đều có một điểm tụ trong $ X $. \*

Thật vậy, nếu $ A \subset K $, trong đó $ K $ là một tập con quasi-compact của $ X $, thì mọi cơ sở lọc trên $ A $ đều có một điểm tụ trong $ K $.

Đảo lại của mệnh đề này không đúng nếu không có hạn chế nào trên $ X $ (Bài tập 22).

#### Nhận xét {#top-i-s9-n3-rem-1 .statement}

Trong một không gian không Hausdorff, một tập compact không nhất thiết đóng, và bao đóng của nó không nhất thiết quasi-compact (Bài tập 5); giao của hai tập compact không nhất thiết quasi-compact (Bài tập 5); hợp của hai tập compact không nhất thiết compact (Bài tập 5).

### 4. ẢNH CỦA MỘT KHÔNG GIAN COMPACT QUA MỘT ÁNH XẠ LIÊN TỤC

#### Định lý 2 {#top-i-s9-thm-2 .statement}

*Nếu $ f $ là một ánh xạ liên tục từ một không gian quasi-compact $ X $ vào một không gian tôpô $ X' $, thì tập $ f(X) $ là quasi-compact.*

Cho $ \mathcal{R} $ là một phủ của $ f(X) $ bởi các tập mở trong $ X' $; khi đó $ \overline{f}^{-1}(\mathcal{R}) $ là một phủ mở của $ X $ (\S 2, no. 1, Định lý 1); do đó tồn tại một tập con hữu hạn $ \mathcal{S} $ của $ \mathcal{R} $ sao cho $ (\mathcal{S} \overline{f}) $ là một phủ của $ X $; nhưng khi đó $ \mathcal{S} $ là một phủ của $ f(X) $ và định lý được chứng minh.

#### Hệ quả 1 {#top-i-s9-thm-2-cor-1 .statement}

*Cho $ f $ là một ánh xạ liên tục của một không gian tôpô $ X $ vào một không gian Hausdorff $ X' $. Khi đó ảnh qua $ f $ của bất kỳ tập gần compact nào (tương ứng gần compact tương đối) trong $ X $ là một tập compact (tương ứng compact tương đối) trong $ X' $.*

#### Hệ quả 2 {#top-i-s9-thm-2-cor-2 .statement}

*Mọi ánh xạ liên tục $ f $ của một không gian gần compact $ X $ vào một không gian Hausdorff $ X' $ đều là ánh xạ đóng. Nếu thêm $ f $ là song ánh, thì $ f $ là một đồng phôi.*

Điều này suy ra ngay lập tức từ Hệ quả 1 và Mệnh đề 4 của no. 3.

Đặc biệt:

#### Hệ quả 3 {#top-i-s9-thm-2-cor-3 .statement}

*Một tôpô Hausdorff thô hơn tôpô của một không gian gần compact phải trùng với tôpô nói trên.*

#### Hệ quả 4 {#top-i-s9-thm-2-cor-4 .statement}

*Cho $ X $ là một không gian tôpô và $ R $ là một quan hệ tương đương Hausdorff trên $ X $.*

a) *Nếu có một tập gần compact $ K $ trong $ X $ mà giao với mọi lớp tương đương mod $ R $, thì $ X/R $ là compact và ánh xạ chính tắc của $ K/R_K $ lên $ X/R $ là một đồng phôi.*

b) *Nếu $ K $ cũng gặp mỗi lớp tương đương tại đúng một điểm, thì $ K $ là một tiết diện liên tục của $ X $ đối với quan hệ $ R $* (\$ 3, no. 5).

Cho $ f $ là hạn chế trên $ K $ của ánh xạ chính tắc $ X \to X/R $. Vì $ X/R $ là Hausdorff nên suy ra từ Hệ quả 1 rằng $ X/R $ là compact và từ Hệ quả 2 rằng $ f $ là đóng; do đó song ánh $ K/R_K \to X/R $ tương ứng với $ f $ là một đồng phôi (\$ 5, no. 2, Mệnh đề 3). Điều này giải quyết a); b) suy ra ngay lập tức, vì lúc này ta có $ K/R_K = K $.

### 5. TÍCH CỦA CÁC KHÔNG GIAN COMPACT

#### Định lý 3 (Tychonoff) {#top-i-s9-thm-3 .statement}

*Mọi tích của các không gian gần compact (tương ứng compact) đều là gần compact (tương ứng compact). Ngược lại, nếu một tích của các không gian không rỗng là gần compact (tương ứng compact) thì mỗi nhân tử đều là gần compact (tương ứng compact).*

Xét theo đặc trưng hóa các không gian tích Hausdorff được cho trong \$ 8, no. 2, Mệnh đề 7, chỉ cần chứng minh các khẳng định đối với các không gian gần compact. Nếu $ X = \prod_{i \in I} X_i $ là gần compact và không rỗng, thì $ X_i = \operatorname{pr}_i(X) $ là gần compact do Định lý 2 của no. 4. Ngược lại, giả sử các $ X_i $ đều gần compact và cho $ \mathcal{U} $ là một siêu lọc trên $ X $; khi đó với mỗi $ i \in I $, $ \operatorname{pr}_i(\mathcal{U}) $ là một cơ sở siêu lọc trên $ X_i $ (\$ 6, no. 6, Mệnh đề 10) nên do tiên đề (C') nó hội tụ; vì vậy $ \mathcal{U} $ hội tụ (\$ 7, no. 6, Hệ quả 1 của Mệnh đề 10) và do đó $ X $ là gần compact.

#### Hệ quả {#top-i-s9-n5-cor-1 .statement}

*Để một tập con của một tích các không gian tôpô là gần compact tương đối thì điều kiện cần và đủ là mỗi ảnh chiếu của nó phải gần compact tương đối trong nhân tử tương ứng.*

Điều kiện cần suy ra từ Định lý 2 của \$ 4. Để chứng minh điều kiện đủ, cho $ A $ là một tập con của $ \prod_i X_i $ sao cho, với mỗi chỉ số $ i $, $ \operatorname{pr}_i(A) $ được chứa trong một tập gần compact $ K_i $ của $ X_i $; khi đó $ A $ được chứa trong tập gần compact $ \prod_i K_i $ của $ \prod_i X_i $.

### 6. GIỚI HẠN NGHỊCH ĐẢO CỦA CÁC KHÔNG GIAN COMPACT

#### Mệnh đề 8 {#top-i-s9-prop-8 .statement}

Cho $(X_\alpha, f_{\alpha\beta})$ là một hệ ngược các không gian compact được chỉ số bởi một tập có hướng $I$ sao cho $f_{\alpha\alpha}$ là ánh xạ đồng nhất với mỗi $\alpha \in I$. Đặt $X = \varprojlim X_\alpha$ là giới hạn ngược và $f_\alpha : X \to X_\alpha$ là ánh xạ chính tắc (\S 4, no. 4). Khi đó
a) $X$ là compact và với mỗi $\alpha \in I$ ta có
$$
f_\alpha(X) = \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta).
$$
b) *Nếu các* $X_\alpha$ *đều không rỗng thì* $X$ *không rỗng*.

$X$ là một không gian con đóng của $\prod_\alpha X_\alpha$ (\S 8, no. 2, Mệnh đề 7, Hệ quả 2) và do Định lý 3 của no. 5 cùng Mệnh đề 3 của no. 3 thì nó compact. Các khẳng định còn lại là hệ quả của *Lý thuyết tập hợp*, chương III, \S 7, no. 4, Định lý 1. Ta áp dụng định lý này bằng cách lấy $\mathcal{S}_\alpha$ là tập hợp các tập con đóng của $X_\alpha$. Các điều kiện (i) và (ii) chỉ là các tiên đề $(O'_1)$ và $(C'')$ tương ứng; điều kiện (iii) được thỏa vì $\{x_\alpha\}$ là đóng và $f_{\alpha\beta}$ liên tục (\S 2, no. 1, Định lý 1), và cuối cùng điều kiện (iv) được thỏa nhờ Hệ quả 2 của Định lý 2 của no. 4.

#### Hệ quả 1 {#top-i-s9-prop-8-cor-1 .statement}

*Cho* $(X_\alpha, f_{\alpha\beta})$ *là một hệ ngược các không gian tôpô được chỉ số bởi một tập có hướng, sao cho với mỗi cặp chỉ số* $\alpha, \beta$ *mà* $\alpha \leq \beta$ *và với mỗi* $x_\alpha \in X_\alpha$, $\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$ *là compact*. *Khi đó đẳng thức (1) đúng và* $\overline{f}_{\alpha}^{-1}(x_\alpha)$ *là compact với mỗi chỉ số* $\alpha$ *và mỗi* $x_\alpha \in X_\alpha$.

Với mỗi $x_\alpha \in \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta)$ và mỗi $\beta \geq \alpha$, đặt $L_\beta$ là $\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$. Nếu $\alpha \leq \beta \leq \gamma$, thì ta có $f_{\beta\gamma}(L_\gamma) \subset L_\beta$ và tập hợp mọi chỉ số $\beta \geq \alpha$ là đồng cuối trong tập chỉ số. Suy ra ngay rằng các $L_\beta$ ($\beta \geq \alpha$) tạo thành một hệ ngược các không gian tôpô (với các hạn chế của các $f_{\beta\gamma}$ làm ánh xạ), mà giới hạn ngược $L$ của chúng đồng phôi với $\overline{f}_{\alpha}^{-1}(x_\alpha)$. Vì theo giả thiết các $L_\beta$ là compact và không rỗng, hệ quả suy ra từ Mệnh đề 8.

#### Hệ quả 2 {#top-i-s9-prop-8-cor-2 .statement}

*Cho* $(X_\alpha, f_{\alpha\beta})$ *và* $(X'_\alpha, f'_{\alpha\beta})$ *là hai hệ ngược các không gian tôpô được chỉ số bởi cùng một tập có hướng* $I$, *và cho* $(u_\alpha)$ *là một hệ ngược các ánh xạ* $u_\alpha : X_\alpha \to X'_\alpha$. *Đặt* $X = \varprojlim X_\alpha$, $X' = \varprojlim X'_\alpha$, $u = \varprojlim u_\alpha$. *Khi đó*:
a) *Nếu* $x' = (x'_\alpha) \in X'$ *sao cho* $\overline{u'}_{\alpha}^{-1}(x'_\alpha)$ *compact và không rỗng với mỗi* $\alpha \in I$, *thì* $\overline{u}^{-1}(x')$ *compact và không rỗng*.

b) *Nếu các* $ X_\alpha $ *là compact, các* $ X'_\alpha $ *Hausdorff và các* $ u_\alpha $ *toàn ánh và liên tục, thì* $ u $ *toàn ánh.*

Let $ L_\alpha $ denote $ \overline{u}_\alpha^{-1}(x'_\alpha) $; then rõ ràng các $ L_\alpha $ lập thành một hệ ngược của các không gian tôpô (với các hạn chế của các $ f_{\alpha\beta} $ làm ánh xạ) và $ \overline{u}^{-1}(x' = L) $ là giới hạn ngược của các $ L_\alpha $; do đó mệnh đề a) suy ra từ Mệnh đề 8. Mệnh đề b) là một hệ quả tức thì, xét đến Mệnh đề 3 của no. 3.

### 7. CÁC KHÔNG GIAN ĐỊA PHƯƠNG COMPACT

#### Định nghĩa 4 {#top-i-s9-def-4 .statement}

*Một không gian tôpô $ X $ được gọi là địa phương compact nếu nó là Hausdorff và nếu mỗi điểm của $ X $ đều có một lân cận compact.*

Rõ ràng một không gian compact là địa phương compact, nhưng điều ngược lại là sai; chẳng hạn, mọi không gian *rời rạc* đều là địa phương compact, nhưng không compact nếu *vô hạn*.

\* Như ta sẽ thấy ở Chương IV, § 2, đường thẳng thực $ \mathbf{R} $ là địa phương compact, nhưng không compact. \*

#### Mệnh đề 9 {#top-i-s9-prop-9 .statement}

*Mọi không gian địa phương compact đều chính quy.*

Cho $ X $ là một không gian địa phương compact, thì mỗi điểm $ x \in X $ đều có một lân cận compact $ V $; vì $ X $ là Hausdorff, nên $ V $ đóng (no. 3, Mệnh đề 4). Mặt khác, $ V $ là một không gian con chính quy của $ X $ (no. 2, Hệ quả của Mệnh đề 1) và do đó $ X $ chính quy (\S 8, no. 4, Mệnh đề 13).

#### Hệ quả {#top-i-s9-n7-cor-1 .statement}

*Trong một không gian địa phương compact, mỗi điểm đều có một hệ cơ bản các lân cận compact.*

Vì giao của một lân cận đóng của $ x $ và một lân cận compact của $ x $ là một lân cận compact của $ x $ (no. 3, Mệnh đề 3).

Tồn tại những không gian tôpô *không Hausdorff* mà trong đó mỗi điểm đều có một hệ cơ bản các lân cận compact (Bài tập 5).

Hệ quả của Mệnh đề 9 có thể được tổng quát hóa như sau:

#### Mệnh đề 10 {#top-i-s9-prop-10 .statement}

*Trong một không gian địa phương compact $ X $, mọi tập compact $ K $ đều có một hệ cơ bản các lân cận compact.*

Cho $ U $ là một lân cận tùy ý của $ K $. Với mỗi $ x \in K $ có một lân cận compact $ W(x) $ của $ x $ được chứa trong $ U $. Các phần trong của các tập

W(x) lập thành một phủ mở của K khi x chạy qua K; do đó tồn tại một số hữu hạn các điểm $ x_i \in K $ ($ 1 \leq i \leq n $) sao cho các phần trong của các W(x_i) phủ K. Hợp V của các W(x_i) vì thế là một lân cận compact của K được chứa trong U (no. 3, Mệnh đề 5).

#### Mệnh đề 11 {#top-i-s9-prop-11 .statement}

*Cho X là một không gian địa phương compact và F là một tập con của X sao cho F \cap K là compact hễ khi nào K là một tập con compact của X. Khi đó F đóng trong X.*

Xét Mệnh đề 4 của no. 3, điều này suy ra từ Mệnh đề 3 a) của § 3, no. 1.

#### Mệnh đề 12 {#top-i-s9-prop-12 .statement}

*Trong một không gian Hausdorff X, mọi không gian con địa phương compact A đều đóng địa phương.*

Theo giả thiết, với mọi $ x \in A $ đều có một lân cận V của x trong X sao cho $ V \cap A $ là compact và do đó đóng trong V (no. 3, Mệnh đề 4).

#### Mệnh đề 13 {#top-i-s9-prop-13 .statement}

*Mọi không gian con đóng địa phương của một không gian địa phương compact X đều địa phương compact.*

Cho A là một không gian con đóng địa phương của X; khi đó với mỗi $ x \in A $ có một lân cận U của x trong X sao cho $ U \cap A $ đóng trong U. Cho $ V \subset U $ là một lân cận compact của x trong X; $ V \cap A = V \cap (U \cap A) $ đóng trong V và do đó compact (no. 3, Mệnh đề 3). Vì $ V \cap A $ là một lân cận của x trong A, nên điều phải chứng minh đã xong (rõ ràng A là Hausdorff).

Định lý 1 (no. 1) và Hệ quả 2 của Định lý 2 (no. 4) *không mở rộng* sang các không gian địa phương compact không compact.

Chẳng hạn, trong một không gian rời rạc vô hạn X, bộ lọc gồm những tập chứa một điểm $ x \in X $ đã cho và có phần bù hữu hạn có x là điểm tụ duy nhất của nó nhưng không hội tụ đến x. Vì mọi ánh xạ f của X vào một không gian Hausdorff X' đều liên tục, ảnh của một tập con tùy ý của X qua f (tập này đóng trong X, vì X là rời rạc) nói chung sẽ không là một tập con đóng của X'.

Mệnh đề tương ứng với Định lý 3 của no. 5 là mệnh đề sau đây:

#### Mệnh đề 14 {#top-i-s9-prop-14 .statement}

a) *Cho $ (X_i)_{i \in I} $ là một họ các không gian địa phương compact sao cho $ X_i $ compact đối với mọi chỉ số trừ một số hữu hạn. Khi đó không gian tích $ X = \prod_{i \in I} X_i $ là địa phương compact.*

b) *Ngược lại, nếu tích của một họ $ (X_i)_{i \in I} $ các không gian tôpô không rỗng là địa phương compact, thì các thừa số $ X_i $ là compact đối với mọi chỉ số trừ một số hữu hạn, và các thừa số không compact là địa phương compact.*

b) Nếu $ X = \prod_{i \in I} X_i $ là địa phương compact và các $ X_i $ không rỗng, thì mỗi $ X_i $ đồng phôi với một không gian con đóng của $ X $ ($ \S 4 $, no. 2, Mệnh đề 4 và $ \S 4 $, no. 3, Hệ quả của Mệnh đề 7), nên địa phương compact theo Mệnh đề 13. Cho $ a = (a_i) $ là một điểm của $ X $ và cho $ V $ là một lân cận compact của $ a $; vì ta có $ \operatorname{pr}_i V = X_i $ đối với mọi chỉ số trừ một số hữu hạn ($ \S 4 $, no. 1), suy ra từ no. 4, Hệ quả 1 của Định lý 2 rằng các $ X_i $ compact ngoại trừ một số hữu hạn chỉ số.

### 8. NHÚNG CỦA MỘT KHÔNG GIAN ĐỊA PHƯƠNG COMPACT VÀO MỘT KHÔNG GIAN COMPACT

#### Định lý 4 (Alexandroff) {#top-i-s9-thm-4 .statement}
==========

*Nếu $ X $ là một không gian compact địa phương bất kỳ, thì tồn tại một không gian compact $ X' $ và một đồng phôi $ f $ của $ X $ lên phần bù của một điểm trong $ X' $. Hơn nữa, nếu $ X'_1 $ là một không gian compact khác sao cho có một đồng phôi $ f_1 $ của $ X $ lên phần bù của một điểm trong $ X'_1 $, thì tồn tại một đồng phôi duy nhất $ g $ của $ X' $ lên $ X'_1 $ sao cho $ f_1 = g \circ f $.*

Trước hết ta chứng minh mệnh đề thứ hai của định lý. Ta có
$$
f(X) = X' - \{ \omega \} \quad \text{và} \quad f_1(X) = X'_1 - \{ \omega_1 \}.
$$
Nếu đồng phôi $ g $ tồn tại thì nó phải duy nhất, vì theo định nghĩa ta có $ g(x') = f_1(\overline{f}(x')) $ nếu $ x' \neq \omega $ và do đó $ g(\omega) = \omega_1 $. Còn lại chỉ cần chứng minh rằng song ánh $ g : X' \to X'_1 $ được định nghĩa như vậy là liên tục hai chiều; vì $ X' $ và $ X'_1 $ có thể thay thế cho nhau, ta chỉ cần chứng minh rằng ảnh qua $ g $ của một lân cận của một điểm $ x' \in X' $ là một lân cận của $ g(x') $ trong $ X'_1 $. Điều này hiển nhiên từ định nghĩa của $ g $ nếu $ x' \neq \omega $. Nếu $ x' = \omega $, cho $ V' $ là một lân cận mở của $ \omega $ trong $ X' $; khi đó $ X' - V' = K $ là đóng trong $ X' $ và do đó compact (no. 3, Mệnh đề 3) và được chứa trong $ f(X) $; suy ra $ g(K) = f_1(\overline{f}(K)) $ là compact (no. 4, Định lý 2, Hệ quả 1). Suy ra $ g(V') = X'_1 - g(K) $ là một lân cận mở của $ \omega_1 $ (no. 3, Mệnh đề 4). Vậy $ g $ là một đồng phôi.

Để chứng minh phần thứ nhất của định lý, hãy cho $ X' $ là một tập hợp là tổng của $ X $ và một tập hợp gồm một điểm duy nhất $ \omega $. Ta định nghĩa một tôpô trên $ X' $ bằng cách lấy tập $ \mathcal{O} $ các tập con mở của $ X' $ gồm tất cả các tập con mở của $ X $ và mọi tập con có dạng $ (X - K) \cup \{ \omega \} $, trong đó $ K $ là một tập con compact của $ X $. Vì mọi giao của các tập con compact của $ X $ đều là compact (no. 3, Mệnh đề 3 và 4) và vì mọi tập con đóng của một tập compact đều là compact (no. 3, Mệnh đề 3), suy ra $ \mathfrak{D} $ thỏa mãn tiên đề $(O_I)$; và vì mọi hợp hữu hạn của các tập con compact của $ X $ đều là compact (no. 3, Mệnh đề 5), $ \mathfrak{D} $ cũng thỏa mãn $(O_{II})$. Mọi tập con compact của $ X $ đều đóng trong $ X $ (no. 3, Mệnh đề 4) và do đó tôpô cảm sinh trên $ X $ bởi tôpô của $ X' $ là tôpô ban đầu trên $ X $. Vậy chỉ còn phải chứng minh rằng $ X' $ là compact. Trước hết, $ X' $ là *Hausdorff*. Thật vậy, nếu $ x, y $ là hai điểm phân biệt bất kỳ của $ X $, thì chúng có các lân cận mở rời nhau $ V, W $ tương ứng trong $ X $, và $ V, W $ là mở trong $ X' $; mặt khác mỗi $ x \in X $ có một lân cận compact $ K $ trong $ X $, cũng là một lân cận của $ x $ trong $ X' $, còn

$$
(X - K) \cup \{ \omega \}
$$

là một lân cận của $ \omega $ trong $ X' $ và hiển nhiên không giao với $ K $. Cuối cùng, $ X' $ là *gần compact*. Cho $ (U_\lambda)_{\lambda \in L} $ là một phủ mở của $ X' $; khi đó với ít nhất một chỉ số $ \mu \in L $ ta có $ U_\mu = (X - K_\mu) \cup \{ \omega \} $ trong đó $ K_\mu $ là một tập con compact của $ X $. Suy ra tồn tại một tập con hữu hạn $ H $ của $ L $ sao cho các tập $ U_\lambda $ (với $ \lambda \in H $) phủ $ K_\mu $; nếu $ J = H \cup \{ \mu \} $, thì $ (U_\lambda)_{\lambda \in J} $ là một phủ mở hữu hạn của $ X' $, và chứng minh hoàn tất.

Lưu ý rằng nếu $ X $ đã *compact* rồi, thì $ \omega $ là một điểm *cô lập* của không gian compact $ X' $; do đó $ X' $ là *tổng* ($ \S $ 2, no. 4, Ví dụ 3) của không gian $ X $ và không gian $ \{ \omega \} $.

When a compact space $ X' $ has been constructed as above from a locally compact space $ X $ by adjoining an element $ \omega $, it is often said that $ \omega $ is the "điểm ở vô cùng" of $ X' $, and that $ X' $ is obtained from $ X $ by adjoining a point at infinity. $ X' $ is also called the *compact hóa Alexandroff* or the *compact hóa một điểm* of the locally compact space $ X $.

\* Ví dụ. If we apply Alexandroff's theorem to the real plane $ \mathbf{R}^2 $, we get a compact space homeomorphic to the sphere $ S_2 $ whose equation is $ x_1^2 + x_2^2 + x_3^2 = 1 $ in $ \mathbf{R}^3 $. A homeomorphism of these two spaces may be described as follows: the point $ \omega $ (the point at infinity) adjoined to $ \mathbf{R}^2 $ is mapped to $ (0, 0, 1) \in S_2 $, and every point $ (x_1, x_2) $ of $ \mathbf{R}^2 $ is mapped to the point where the line joining the points $ (0, 1, 1) $ and $ (x_1, x_2, 0) $ in $ \mathbf{R}^3 $ meets $ S_2 $ again. This homeomorphism is known as *phép chiếu lập thể*.

### 9. CÁC KHÔNG GIAN ĐỊA PHƯƠNG COMPACT $ \sigma $-COMPACT

#### Định nghĩa 5 {#top-i-s9-def-5 .statement}

*Một không gian địa phương compact $ X $ được gọi là $ \sigma $-compact hay đếm được tại vô cùng nếu nó là một hợp đếm được của các tập con compact.*

#### Ví dụ 1 {#top-i-s9-n9-exa-1 .statement}

Một không gian rời rạc là $ \sigma $-compact khi và chỉ khi nó đếm được.
\* 2) Đường thẳng thực $ \mathbf{R} $ là địa phương compact và $ \sigma $-compact, vì nó là hợp của các đoạn compact $[ -n, +n ]$ với $ n \in \mathbf{N} $. \*

#### Nhận xét {#top-i-s9-n9-rem-1 .statement}

Một không gian Hausdorff có thể là hợp đếm được của các không gian con compact mà không phải là địa phương compact. \* Một ví dụ là không gian Hilbert với tôpô yếu, như chúng ta sẽ chứng minh trong một tập sau.

#### Mệnh đề 15 {#top-i-s9-prop-15 .statement}

*Nếu $ X $ là một không gian địa phương compact $ \sigma $-compact, thì tồn tại một dãy $ (U_n) $ gồm các tập con mở tương đối compact của $ X $ phủ $ X $, sao cho $ \overline{U}_n \subset U_{n+1} $ với mỗi $ n $.

Cho $ X $ là hợp của một dãy $ (K_n) $ các tập compact. Cho $ U_1 $ là một lân cận mở tương đối compact của $ K_1 $ (no. 7, Proposition 10) và định nghĩa $ U_n $ theo quy nạp với $ n > 1 $ là một lân cận mở tương đối compact của $ \overline{U}_{n-1} \in K_n $ (no. 3, Proposition 5; no. 7, Proposition 10). Dãy $ (U_n) $ rõ ràng có các tính chất cần thiết.

#### Hệ quả 1 {#top-i-s9-prop-15-cor-1 .statement}

*Với ký hiệu của Mệnh đề 15, mọi tập con compact $ K $ của $ X $ đều được chứa trong một $ U_n $ nào đó.

Vì $ K $ có thể được phủ bởi một số hữu hạn các $ U_k $, theo tiên đề (C''').

#### Hệ quả 2 {#top-i-s9-prop-15-cor-2 .statement}

*Cho $ X $ là một không gian địa phương compact và cho $ X' $ là không gian compact thu được bằng cách thêm vào $ X $ một điểm ở vô cùng $ \omega $ (no. 8). Khi đó $ X $ là $ \sigma $-compact khi và chỉ khi điểm $ \omega $ có một hệ lân cận cơ bản đếm được trong $ X' $.*

If $ X $ là $ \sigma $-compact ta có thể xây dựng một dãy các tập hợp con $ U_n $ của $ X $ như trong Mệnh đề 15, và các lân cận $ X' - \overline{U}_n $ của $ \omega $ trong $ X' $ tạo thành một hệ cơ bản các lân cận của $ \omega $ nhờ Hệ quả 1. Chiều đảo lại suy ra từ thực tế là các phần bù của các lân cận mở của $ \omega $ là các tập hợp con compact của $ X $.

Rõ ràng mọi không gian con đóng của một không gian compact địa phương và $ \sigma $-compact là compact địa phương và $ \sigma $-compact. Tương tự, bất kỳ tích hữu hạn nào của các không gian compact địa phương và $ \sigma $-compact đều là compact địa phương và $ \sigma $-compact.

Tuy nhiên, lưu ý rằng một không gian con mở của một không gian compact chưa chắc đã là $ \sigma $-compact, như định lý của Alexandroff (no. 8, Định lý 4) cho thấy.

### 10. KHÔNG GIAN PARACOMPACT

#### Định nghĩa 6 {#top-i-s9-def-6 .statement}

*Một không gian tôpô được gọi là paracompact nếu nó là Hausdorff và thỏa mãn tiên đề sau:*

(PC) *Mọi phủ mở $ \mathcal{R} $ của $ X $ đều có một tinh luyện mở hữu hạn địa phương $ \mathcal{R}' $.*
(Lý thuyết tập hợp, Chương II, § 4, no. 6, Định nghĩa 5).

Mọi *không gian compact* đều rõ ràng là paracompact. Mọi không gian *rời rạc* $ X $ đều là paracompact, vì phủ mở gồm tất cả các tập hợp gồm một điểm của $ X $ là hữu hạn địa phương và mịn hơn mọi phủ mở của $ X $.

#### Mệnh đề 16 {#top-i-s9-prop-16 .statement}

*Mọi không gian con đóng* $ F $ *của một không gian paracompact* $ X $ *đều là paracompact*.

Chắc chắn $ F $ là Hausdorff. Mặt khác, nếu $ (V_i) $ là một phủ mở trong không gian con $ F $, thì mỗi $ V_i $ có dạng $ V_i = U_i \cap F $, trong đó $ U_i $ mở trong $ X $. Hãy xét phủ mở $ \mathcal{R} $ của $ X $ gồm CF và các $ U_i $; vì $ X $ là paracompact, nên $ \mathcal{R} $ có một tinh luyện hữu hạn địa phương $ \mathcal{R}' $, và các giao với $ F $ của các tập hợp thuộc $ \mathcal{R}' $ tạo thành một phủ mở hữu hạn địa phương của $ F $ mịn hơn phủ đã cho $ (V_i) $.

Mặt khác, một không gian con mở của một không gian compact chưa chắc là paracompact (Bài tập 11).

#### Mệnh đề 17 {#top-i-s9-prop-17 .statement}

*Tích của một không gian paracompact và một không gian compact là paracompact*.

Cho $ X $ là một không gian paracompact, $ Y $ là một không gian compact, $ \mathcal{R} $ là một phủ mở của $ X \times Y $. Với mỗi $ (x, y) \in X \times Y $ có một lân cận mở $ V(x, y) $ của $ x $ trong $ X $ và một lân cận mở $ W(x, y) $ của $ y $ trong $ Y $ sao cho $ V(x, y) \times W(x, y) $ được chứa trong một tập thuộc $ \mathcal{R} $. Với mỗi $ x \in X $, các tập $ W(x, y) $ khi $ y $ chạy qua $ Y $ tạo thành một phủ mở của $ Y $; do đó tồn tại một số hữu hạn các điểm
$$
y_i \in Y \quad (1 \leq i \leq n(x))
$$
sao cho các $ W(x, y_i) $ phủ $ Y $. Kí hiệu $ U(x) $ là
$$
\bigcap_{i=1}^{n(x)} V(x, y_i);
$$
khi đó mỗi tập mở $ U(x) \times W(x, y_i) $ đều được chứa trong một tập của $ \mathcal{R} $. Bây giờ cho $ (T_i)_{i \in I} $ là một phủ mở hữu hạn địa phương của $ X $ mịn hơn phủ $ (U(x))_{x \in X} $. Với mỗi $ i \in I $, lấy $ x_i $ là một điểm của $ X $ sao cho $ T_i \subset U(x_i) $, và kí hiệu $ S_{i, k} $ là các tập $ W(x_i, y_k) $ tương ứng với điểm $ x_i $ này ($ 1 \leq k \leq n(x_i) $). Rõ ràng các tập
$$
T_i \times S_{i, k} \quad (i \in I, \ 1 \leq k \leq n(x_i) \text{ for each } i \in I)
$$
tạo thành một phủ mở của $ X \times Y $ mịn hơn $ \mathcal{R} $, và chứng minh sẽ đầy đủ nếu ta chỉ ra rằng phủ này hữu hạn địa phương. Cho $ (x, y) $ là một điểm bất kỳ của $ X \times Y $; có một lân cận $ Q $ của $ x $ chỉ gặp một số hữu hạn các tập $ T_i $, và do đó lân cận $ Q \times Y $ của $ (x, y) $ chỉ gặp một số hữu hạn các tập $ T_i \times S_{i, k} $.

#### Mệnh đề 18 {#top-i-s9-prop-18 .statement}

*Tổng* (\S 2, no. 4, Ví dụ 3) *của một họ* $(X_i)_{i \in I}$ *các không gian paracompact là paracompact*.

Cho $X$ là tổng của các $X_i$, và cho $(V_\lambda)_{\lambda \in L}$ là một phủ mở của $X$. Phủ được tạo bởi các tập mở $X_i \cap Y_\lambda$ mịn hơn $(V_\lambda)$. Với mỗi $i \in I$, cho $(U_{i,\mu})_{\mu \in M_i}$ là một tinh chỉnh mở hữu hạn địa phương của phủ $(V_\lambda \cap X_i)_{\lambda \in L}$; khi đó phủ mở của $X$ được tạo bởi các

$$
U_{i,\mu} \quad (i \in I, \ \mu \in M_i \text{ for each } i \in I)
$$

là hữu hạn địa phương và tinh chỉnh phủ ban đầu $(V_\lambda)$.

#### Định lý 5 {#top-i-s9-thm-5 .statement}

*À không gian compact địa phương* $X$ *là paracompact khi và chỉ khi* $X$ *là tổng của một họ các không gian compact $\sigma$-compact địa phương*.

Giả sử $X$ là paracompact, và với mỗi $x \in X$ hãy cho $V_x$ là một lân cận mở tương đối compact của $x$ trong $X$. Khi đó theo giả thiết tồn tại một phủ mở hữu hạn địa phương $(U(\alpha))_{\alpha \in A}$ của $X$ tinh chỉnh phủ $(V_x)_{x \in X}$. Vì thế các $U(\alpha)$ đều tương đối compact. Mỗi tập con compact $K$ của $X$ chỉ gặp hữu hạn nhiều tập $U(\alpha)$, vì các tập không rỗng $U(\alpha) \cap K$ tạo thành một phủ mở hữu hạn địa phương của không gian compact $X$; do đó chúng phải có hữu hạn phần tử (mục 1). Bây giờ hãy đặt $R$ là quan hệ sau giữa hai điểm $x, y$ của $X$: "tồn tại một dãy hữu hạn $(\alpha_i)_{1 \leq i \leq n}$ các chỉ số trong $A$ sao cho $x \in U(\alpha_1), \ y \in U(\alpha_n)$ và $U(\alpha_i)$ giao với $U(\alpha_{i+1})$ với $1 \leq i \leq n - 1$".

Dễ thấy ngay rằng $R$ là một quan hệ tương đương, và mỗi lớp tương đương theo $R$ là một tập con *mở* của $X$ [vì các $U(\alpha)$ là các tập mở]. Do đó $X$ là *tổng* của các không gian con compact địa phương (mục 7, Mệnh đề 13) được tạo bởi các lớp tương đương theo $R$, và còn lại phải chứng minh rằng mỗi không gian con đó là hợp của một họ con đếm được của họ $(U(\alpha))$.

Cho $x$ là một điểm bất kỳ của $X$, và định nghĩa một dãy $(C_n)$ gồm các tập con mở tương đối compact của $X$ bằng quy nạp theo $n$ như sau; $C_1$ là hợp của các tập $U(\alpha)$ chứa $x$, và với mỗi $n > 1$, $C_n$ là hợp của các tập $U(\alpha)$ giao với $C_{n-1}$. Dễ dàng kiểm tra bằng quy nạp theo $n$ rằng mỗi $C_n$ đều tương đối compact và là hợp của một số hữu hạn các tập $U(\alpha)$. Hơn nữa, lớp tương đương của $x$ đối với $R$ là hợp của các $C_n$: vì nếu $(\alpha_i)_{1 \leq i \leq n}$ là một dãy các chỉ số sao cho $x \in U(\alpha_1)$ và $U(\alpha_i)$ giao với $U(\alpha_{i+1})$ với $1 \leq i \leq n - 1$, thì ta thấy bằng quy nạp theo $i$ rằng $U(\alpha_i) \subset C_i$ với $1 \leq i \leq n$. Suy ra các lớp tương đương mod $R$ là $\sigma$-compact, và điều đó hoàn tất chứng minh phần thứ nhất của định lý.

Để chứng minh mệnh đề đảo lại, ta có thể giả sử (theo Mệnh đề 18) rằng $ X $ là $ \sigma $-compact. Cho $ \mathcal{H} = (G_\lambda)_{\lambda \in L} $ là một phủ mở bất kỳ của $ X $, và cho $ (U_n) $ là một dãy các tập mở tương đối compact trong $ X $ có các tính chất đã nêu trong Mệnh đề 15 của no. 9. Ký hiệu $ K_n $ là tập compact $ \overline{U}_n - U_{n-1} $ ($ U_n = \emptyset $ nếu $ n \leq 0 $). Tập mở $ U_{n+1} - \overline{U}_{n-2} $ là một lân cận của $ K_n $ theo phép dựng; do đó với mỗi $ x \in K_n $ tồn tại một lân cận $ W_x $ của $ x $ được chứa trong một trong các tập $ G_\lambda $ và đồng thời cũng được chứa trong $ U_{n+1} - \overline{U}_{n-2} $. Vì $ K_n $ là compact, một số hữu hạn các tập $ W_x $ phủ $ K_n $; gọi $ H_{ni} (1 \leq i \leq p_n) $ là các tập ấy. Khi đó họ $ \mathcal{H}' $ gồm các tập $ H_{ni} (n \geq 1, 1 \leq i \leq p_n \text{ cho mỗi } n) $ là một phủ mở của $ X $ tinh lọc $ \mathcal{H} $, và vì thế để hoàn tất chứng minh ta phải chỉ ra rằng $ \mathcal{H}' $ là *hữu hạn địa phương*. Cho $ z $ là một điểm bất kỳ của $ X $, $ n $ là số nguyên nhỏ nhất sao cho $ z \in U_n $; khi đó vì $ z \notin U_{n-1} $, tồn tại một lân cận $ T $ của $ z $ được chứa trong $ U_n $ và không cắt $ U_{n-2} $. Suy ra rằng $ T $ chỉ cắt những tập $ H_{mi} $ sao cho $ n - 2 \leq m \leq n + 1 $, tức là $ T $ chỉ cắt một số hữu hạn các tập của $ \mathcal{H}' $.

Trong quá trình chứng minh, ta cũng đã thiết lập kết quả sau:

#### Hệ quả {#top-i-s9-n10-cor-1 .statement}

*Cho $ X $ là một không gian compact địa phương paracompact. Khi đó mọi phủ mở $ \mathcal{H} $ của $ X $ đều có một tinh lọc mở *hữu hạn địa phương* $ \mathcal{H}' $ gồm các tập tương đối compact. Nếu $ X $ là $ \sigma $-compact thì $ \mathcal{H}' $ có thể chọn là đếm được.*

### Bài tập {#top-i-s9-exercises}

Xem [các bài tập cho § 9](exercises/s9/).
