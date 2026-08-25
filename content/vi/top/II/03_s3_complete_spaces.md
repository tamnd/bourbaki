---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 3
section_title: Complete spaces
lang: vi
source: top-i-iv
pdf_pages: 0187-0204, 0214-0215
extraction: ocr
subsections:
    - "no": 1
      title: CAUCHY FILTERS
      page: 0
      pdf_page: 187
    - "no": 2
      title: MINIMAL CAUCHY FILTERS
      page: 0
      pdf_page: 189
    - "no": 3
      title: COMPLETE SPACES
      page: 0
      pdf_page: 190
    - "no": 4
      title: SUBSPACES OF COMPLETE SPACES
      page: 0
      pdf_page: 192
    - "no": 5
      title: PRODUCTS AND INVERSE LIMITS OF COMPLETE SPACES
      page: 0
      pdf_page: 192
    - "no": 6
      title: EXTENSION OF UNIFORMLY CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 196
    - "no": 7
      title: THE COMPLETION OF A UNIFORM SPACE
      page: 0
      pdf_page: 197
    - "no": 8
      title: THE HAUSDORFF UNIFORM SPACE ASSOCIATED WITH A UNIFORM SPACE
      page: 0
      pdf_page: 202
    - "no": 9
      title: COMPLETION OF SUBSPACES AND PRODUCT SPACES
      page: 0
      pdf_page: 203
statements: 48
exercises: 7
content_sha256: 2c7bcf5aad84f4f5c6c07a63a16c572d7816ce5adb8498d93e09ee8089518fca
translated_from: content/en/top/II/03_s3_complete_spaces.md
source_content_sha256: daf59b5609a6489a672918c9bebb24140f45498174c58e5b51131f4c3c2181dd
translation_model: gpt-5.4-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-b50a24e1
glossary_version: 34
glossary_terms_sha256: dc450fee8788430448b98259c8c7f2f31e0fba18df07341997a4605e7bab3544
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. KHÔNG GIAN ĐẦY ĐỦ

### 1. BỘ LỌC CAUCHY

Khi một tập hợp $X$ được trang bị một cấu trúc đều, ta có thể định nghĩa ý nghĩa của một tập hợp con "nhỏ" của $X$ (tương đối với cấu trúc này): một tập hợp con "nhỏ" của $X$ là một tập hợp trong đó mọi điểm đều "rất gần" nhau. Chính xác:

#### Định nghĩa 1 {#top-ii-s3-def-1 .statement}

Nếu $X$ là một không gian đều và nếu $V$ là một lân cận của $X$, một tập hợp con $A$ của $X$ được nói là $V$-nhỏ nếu mọi cặp điểm của $A$ đều $V$-gần nhau (nói cách khác, nếu $A \times A \subset V$).

#### Mệnh đề 1 {#top-ii-s3-prop-1 .statement}

Trong một không gian đều $X$, nếu hai tập hợp $A$ và $B$ là $V$-nhỏ và giao nhau, thì hợp $A \cup B$ của chúng là $\vec{V}$-nhỏ.

Cho $ x $ và $ y $ là bất kỳ hai điểm nào của $ A \cup B $, và cho $ Z \in A \cap B $. Khi đó $ (x, z) \in V $ và $ (z, y) \in V $, do đó $ (x, y) \in \overline{V} $.

#### Định nghĩa 2 {#top-ii-s3-def-2 .statement}

*Một bộ lọc $ \mathcal{F} $ trên một không gian đều là một bộ lọc Cauchy nếu với mỗi lân cận $ V $ của $ X $ có một tập hợp con của $ X $ là $ V $-nhỏ và thuộc $ \mathcal{F} $.*

Ở đây một lần nữa ta có thể làm cho ngôn ngữ của mình giàu biểu đạt hơn bằng cách dùng các cụm từ "tập đủ nhỏ" và "một tập nhỏ tùy ý"; do đó Định nghĩa 2 có thể được phát biểu lại bằng cách nói rằng một bộ lọc Cauchy là một bộ lọc chứa *các tập tùy ý nhỏ*.

Một dãy vô hạn $ (u_n) $ các điểm của một không gian đều $ X $ được nói là một *dãy Cauchy* nếu bộ lọc sơ cấp liên kết với dãy là một bộ lọc Cauchy. Điều đó tương đương với việc nói rằng với mỗi lân cận $ V $ của $ X $ tồn tại một số nguyên $ n_0 $ sao cho với mọi số nguyên $ m \geq n_0 $ và $ n \geq n_0 $ ta có $ (u_m, u_n) \in V $.

#### Mệnh đề 2 {#top-ii-s3-prop-2 .statement}

*Trên một không gian đều $ X $, mọi bộ lọc hội tụ đều là một bộ lọc Cauchy.*

Nếu $ x $ là một điểm bất kỳ của $ X $ và $ V $ là một lân cận đối xứng bất kỳ của $ X $, thì lân cận $ V(x) $ của $ x $ là $ \overline{V} $-nhỏ. Nếu $ \mathcal{F} $ là một bộ lọc hội tụ về $ x $, thì có một tập của $ \mathcal{F} $ được chứa trong $ V(x) $, và do đó $ V $-nhỏ.

Rõ ràng mọi bộ lọc *mịn hơn* một bộ lọc Cauchy đều là một bộ lọc Cauchy.

#### Mệnh đề 3 {#top-ii-s3-prop-3 .statement}

*Cho $ f : X \to X' $ là một ánh xạ liên tục đều. Khi đó ảnh của một cơ sở bộ lọc Cauchy trên $ X $ qua $ f $ là một cơ sở bộ lọc Cauchy trên $ X' $.*

Cho $ g = f \times f $. Nếu $ V' $ là một lân cận của $ X' $, thì $ \overline{g^{-1}(V')} $ là một lân cận của $ X $, và ảnh theo $ f $ của một tập hợp $ \overline{g^{-1}(V')}$-nhỏ là $ V' $-nhỏ; do đó có kết quả.

Đặc biệt suy ra rằng nếu cấu trúc đều của một không gian đều $ X $ được thay thế bởi một cấu trúc đều *thô hơn*, thì mọi lọ Cauchy đối với cấu trúc đều ban đầu vẫn là một lọ Cauchy đối với cấu trúc đều mới.

Sự kiện này có thể dễ dàng ghi nhớ dưới dạng sau: *cấu trúc đều càng mịn thì càng có ít lọ Cauchy*.

#### Mệnh đề 4 {#top-ii-s3-prop-4 .statement}

*Cho $ X $ là một tập hợp, cho $ (Y_i)_{i \in I} $ là một họ các không gian đều, và với mỗi $ i \in I $ cho $ f_i $ là một ánh xạ từ $ X $ vào $ Y_i $. Cho $ X $ mang cấu trúc đều cực tiểu $ U $ sao cho các $ f_i $ là liên tục đều. Khi đó để một cơ sở lọ $ \mathcal{B} $ trên $ X $ là một cơ sở lọ Cauchy, điều kiện cần và đủ là $ f_i(\mathcal{B}) $ là một cơ sở lọ Cauchy trên $ Y_i $, với mỗi $ i \in I $.*

Điều kiện là cần theo Mệnh đề 3. Ngược lại, giả sử rằng nó được thỏa mãn, và cho $ U(V_{i_1}, \ldots, V_{i_n}) $ là một lân cận của cấu trúc đều $ \mathcal{U} $ [§ 2, no. 3, công thức (1)]. Theo giả thiết, với mỗi chỉ số $ k $ tồn tại một tập hợp $ M_k \in \mathcal{B} $ sao cho $ f_{i_k}(M_k) $ là $ V_{i_k} $-nhỏ ($ 1 \leq k \leq n $). Cho $ M $ là một tập hợp của $ \mathcal{B} $ được chứa trong $ M_k $ với $ 1 \leq k \leq n $; khi đó với mỗi cặp điểm $ x, x' $ của $ M $ ta có $[f_{i_k}(x), f_{i_k}(x')] \in V_{i_k}$ với $ 1 \leq k \leq n $, do đó
$$
(x, x') \in U(V_{i_1}, \ldots, V_{i_n}).
$$
Điều này hoàn tất chứng minh.

#### Hệ quả 1 {#top-ii-s3-prop-4-cor-1 .statement}

*Nếu một lọ Cauchy trên một không gian đều $ X $ cảm sinh một lọ trên một tập con $ A $ của $ X $, thì lọ này là một lọ Cauchy trên không gian con đều $ A $.*

#### Hệ quả 2 {#top-ii-s3-prop-4-cor-2 .statement}

*Một cơ sở lọ $ \mathcal{B} $ trên một tích $ \prod_{i \in I} X_i $ của các không gian đều là một cơ sở lọ Cauchy khi và chỉ khi, với mỗi $ i \in I $, $ \operatorname{pr}_i(\mathcal{B}) $ là một cơ sở lọ Cauchy trên $ X_i $.*

### 2. CÁC LỌ CAUCHY CỰC TIỂU

Các phần tử cực tiểu (đối với phép chứa) của tập hợp các lọ Cauchy trên một không gian đều $ X $ được gọi là *các lọ Cauchy cực tiểu* trên $ X $.

#### Mệnh đề 5 {#top-ii-s3-prop-5 .statement}

*Cho $ X $ là một không gian đều. Với mỗi bộ lọc Cauchy $ \mathfrak{F} $ trên $ X $, tồn tại một bộ lọc Cauchy cực tiểu duy nhất thô hơn $ \mathfrak{F} $. Nếu $ \mathcal{B} $ là một cơ sở của $ \mathfrak{F} $ và $ \mathcal{G} $ là một hệ cơ bản các lân cận đối xứng của $ X $, thì các tập hợp $ V(M) $ ($ M \in \mathcal{B}, V \in \mathcal{G} $) lập thành một cơ sở của $ \mathfrak{F}_0 $.*

Nếu $ M, M' $ thuộc $ \mathcal{B} $ và $ V, V' $ thuộc $ \mathcal{G} $, thì tồn tại một tập hợp $ M'' \in \mathcal{B} $ (resp. $ V'' \in \mathcal{G} $) sao cho $ M'' \subset M \cap M' $ (resp. $ V'' \subset V \cap V' $); do đó $ V''(M'') \subset V(M) \cap V'(M') $ và vì thế các tập hợp $ V(M) $ ($ M \in \mathcal{B}, V \in \mathcal{G} $) thật sự lập thành một cơ sở của một bộ lọc $ \mathfrak{F}_0 $ trên $ X $. Hơn nữa, nếu $ M $ là $ V $-nhỏ, thì $ V(M) $ là $ V $-nhỏ; do đó $ \mathfrak{F}_0 $ là một bộ lọc Cauchy và rõ ràng thô hơn $ \mathfrak{F} $. Để hoàn tất chứng minh, chỉ cần chỉ ra rằng nếu $ \mathfrak{G} $ là một bộ lọc Cauchy thô hơn $ \mathfrak{F} $, thì $ \mathfrak{G} $ mịn hơn $ \mathfrak{F}_0 $. Với mỗi $ M \in \mathcal{B} $ và mỗi $ V \in \mathcal{G} $ có một tập hợp $ N \in \mathcal{G} $ là $ V $-nhỏ; vì $ N \in \mathfrak{F} $, $ N $ giao với $ M $; do đó $ N \subset V(M) $ và vì vậy $ V(M) \in \mathfrak{G} $.

#### Hệ quả 1 {#top-ii-s3-prop-5-cor-1 .statement}

*Với mỗi $ x \in X $, bộ lọc lân cận $ \mathcal{B}(x) $ của $ x $ trong $ X $ là một bộ lọc Cauchy cực tiểu.*

Lấy $ \mathfrak{F} $ trong Mệnh đề 5 là bộ lọc của mọi tập con của $ X $ chứa $ x $, và lấy $ \mathcal{B} $ chỉ gồm phần tử duy nhất $ \{x\} $.

#### Hệ quả 2 {#top-ii-s3-prop-5-cor-2 .statement}

*Mọi điểm tụ* $ x $ *của một bộ lọc Cauchy* $ \mathfrak{F} $ *đều là một điểm giới hạn của* $ \mathfrak{F} $.

Có một bộ lọc $ \mathcal{G} $ mịn hơn cả $ \mathfrak{F} $ và $ \mathcal{B}(x) $ (Chương I, § 7, no. 2, Mệnh đề 4); vì $ \mathfrak{F} $ là một bộ lọc Cauchy, nên $ \mathcal{G} $ cũng vậy. Nếu $ \mathfrak{F}_0 $ là bộ lọc Cauchy cực tiểu duy nhất thô hơn $ \mathfrak{F} $, thì cả $ \mathfrak{F}_0 $ và $ \mathcal{B}(x) $ đều là các bộ lọc Cauchy cực tiểu thô hơn $ \mathcal{G} $. Do đó $ \mathfrak{F}_0 = \mathcal{B}(x) $, điều này chứng tỏ rằng $ \mathfrak{F} $ hội tụ đến $ x $.

#### Hệ quả 3 {#top-ii-s3-prop-5-cor-3 .statement}

*Mọi bộ lọc Cauchy, thô hơn một bộ lọc hội tụ đến một điểm* $ x $, *cũng hội tụ đến* $ x $.

Đây là một hệ quả của Hệ quả 2.

#### Hệ quả 4 {#top-ii-s3-prop-5-cor-4 .statement}

*Nếu* $ \mathfrak{F} $ *là một bộ lọc Cauchy cực tiểu, thì mọi tập hợp của* $ \mathfrak{F} $ *đều có một phần trong không rỗng cũng thuộc* $ \mathfrak{F} $ *(nói cách khác, $ \mathfrak{F} $ có một cơ sở gồm các tập mở)*.

Cho $ V $ là một lân cận đồng đều bất kỳ của $ X $; khi đó có một lân cận đồng đều mở $ U \subset V $ ($ \S $ 1, no. 2, Hệ quả 2 của Mệnh đề 2). Với mỗi tập con $ M $ của $ X $, $ U(M) $ là mở và được chứa trong $ V(M) $; do đó có kết quả, theo Mệnh đề 5.

### 3. KHÔNG GIAN ĐẦY ĐỦ

Trong một không gian đồng đều $ X $, *một bộ lọc Cauchy không nhất thiết phải có một điểm giới hạn*.

#### Ví dụ 1 {#top-ii-s3-n3-exa-1 .statement}

Xét dãy $ (u_n) $ trên đường thẳng hữu tỉ $ \mathbf{Q} $ được xác định bởi $ u_n = \sum_{p=0}^n 2^{-p(p+1)/2} $. Nếu $ m > n $ ta có
$$
|u_m - u_n| \leq 2^{-n(n+3)/2}
$$
và do đó $ (u_n) $ là một *dãy Cauchy*. Nhưng dãy này không có giới hạn trong $ \mathbf{Q} $; vì nếu số hữu tỉ $ a/b $ là một giới hạn của $ (u_n) $, thì theo (1) ta phải có với mọi $ n $
$$
|a/b - h_n/2^{n(n+1)/2}| \leq 1/2^{n(n+3)/2}
$$
trong đó $ h_n $ là một số nguyên (phụ thuộc vào $ n $); nghĩa là,
$$
|a \cdot 2^{n(n+1)/2} - b h_n| \leq b \cdot 2^{-n}
$$
với mọi $ n $. Bây giờ vế trái của bất đẳng thức này là một số nguyên với mọi $ n $, và do đó phải bằng không khi $ n $ lớn hơn một số nguyên $ n_0 $ sao cho $ b < 2^{n_0} $; vì vậy ta phải có $ a/b = u_n $ với mọi $ n > n_0 $, điều này là vô lý.

#### Ví dụ 2 {#top-ii-s3-n3-exa-2 .statement}

Cho $ X $ là một tập vô hạn, và xét tính đồng đều của các phân hoạch hữu hạn trên $ X $ ($ \S $ 2, no. 2, Nhận xét 1). Mọi *siêu lọc* $ \mathfrak{F} $ trên $ X $ là một

Bộ lọc Cauchy đối với tôpô đều này. Thật vậy, nếu $ (A_i) $ là một phân hoạch hữu hạn của $ X $ và
$$
V = \bigcup_i (A_i \times A_i)
$$
là lân cận đều tương ứng, thì ít nhất một trong các $ A_i $ thuộc $ \mathcal{F} $ (Chương I, § 6, no. 4, Hệ quả của Mệnh đề 5), và $ A_i $ là V-nhỏ. Mặt khác, $ X $ là một không gian rời rạc vô hạn, do đó không compact, và vì vậy tồn tại các siêu bộ lọc trên $ X $ không hội tụ.

#### Định nghĩa 3 {#top-ii-s3-def-3 .statement}

*Một không gian đầy đủ là một không gian đều trong đó mọi bộ lọc Cauchy đều hội tụ.*

Trong một không gian đầy đủ, mọi *dãy Cauchy* (no. 1) do đó đều hội tụ.

#### Ví dụ {#top-ii-s3-n3-exa-3 .statement}

Trên một không gian đều *rời rạc* $ X $, một bộ lọc Cauchy là một siêu bộ lọc tầm thường (Chương I, § 6, no. 4), do đó hội tụ; vì vậy, $ X $ là đầy đủ.

Từ các Định nghĩa 2 và 3 của no. 1 và Mệnh đề 2 của no. 1, ta suy ra mệnh đề sau, được gọi là *tiêu chuẩn Cauchy*:

#### Mệnh đề 6 {#top-ii-s3-prop-6 .statement}

*Cho $ \mathcal{F} $ là một bộ lọc trên một tập hợp $ X $, và cho $ f $ là một ánh xạ từ $ X $ vào một không gian đều đầy đủ $ X' $. Khi đó $ f $ có giới hạn đối với $ \mathcal{F} $ khi và chỉ khi ảnh của $ \mathcal{F} $ qua $ f $ là một cơ sở bộ lọc Cauchy.*

Tiêu chuẩn này cho thấy tầm quan trọng của các không gian đầy đủ trong mọi vấn đề liên quan đến khái niệm giới hạn: nếu một hàm nhận các giá trị của nó trong một không gian đầy đủ, ta có thể chứng minh *sự tồn tại* của một giới hạn *mà không biết trước giá trị của giới hạn*; điều này sẽ không thể thực hiện được nếu định nghĩa của giới hạn là tiêu chuẩn duy nhất về sự hội tụ mà ta có.

Một tôpô đều *mịn hơn* tôpô đều của một không gian đầy đủ không nhất thiết là tôpô đều của một không gian đầy đủ (Bài tập 2). Tuy nhiên, ta có mệnh đề sau:

#### Mệnh đề 7 {#top-ii-s3-prop-7 .statement}

*Cho $ \mathcal{U}_1, \mathcal{U}_2 $ là hai tôpô đều trên một tập hợp $ X $, và cho $ \mathcal{T}_1, \mathcal{T}_2 $ là các tôpô được cảm sinh bởi các tôpô đều này tương ứng. Giả sử rằng $ \mathcal{U}_1 $ mịn hơn $ \mathcal{U}_2 $, và rằng có một hệ cơ sở các lân cận đều của $ \mathcal{U}_1 $ đóng trong $ X \times X $ đối với tôpô $ \mathcal{T}_2 \times \mathcal{T}_2 $. Khi đó một bộ lọc $ \mathcal{F} $ trên $ X $ hội tụ trong tôpô $ \mathcal{T}_1 $ khi và chỉ khi nó là một bộ lọc Cauchy trong tôpô đều $ \mathcal{U}_1 $ và hội tụ trong tôpô $ \mathcal{T}_2 $.*

Các điều kiện rõ ràng là cần thiết, vì $ \mathcal{T}_2 $ thô hơn $ \mathcal{T}_1 $. Ngược lại, giả sử rằng các điều kiện được thỏa mãn, và cho $ x $ là một điểm giới hạn của $ \mathcal{F} $ đối với $ \mathcal{T}_2 $; ta sẽ chứng minh rằng $ x $ là một giới hạn của $ \mathcal{F} $ đối với $ \mathcal{T}_1 $. Cho $ V $ là một lân cận đều đối xứng của $ \mathcal{U}_1 $ đóng trong tôpô $ \mathcal{T}_2 \times \mathcal{T}_2 $. Theo giả thiết, $ \mathcal{F} $ chứa một tập hợp $ M $ là V-nhỏ; do đó nếu $ x' \in M $ thì ta có $ M \subset V(x') $. Nhưng $ V(x') $ đóng trong tôpô $ \mathcal{T}_2 $; do đó $ x $, nằm trong bao đóng của $ M $ đối với $ \mathcal{T}_2 $, phải thuộc $ V(x') $. Suy ra rằng $ M \subset \hat{V}(x) $, và mệnh đề được chứng minh.

#### Hệ quả {#top-ii-s3-n3-cor-1 .statement}

Trong các điều kiện của Mệnh đề 7, nếu $ U_2 $ là một tôpô đều của một không gian đầy đủ, thì $ U_1 $ cũng vậy.

Vì mọi bộ lọc Cauchy đối với $ U_1 $ khi đó là một bộ lọc Cauchy đối với $ U_2 $ và do đó hội tụ trong tôpô $ \mathcal{T}_2 $.

Chú ý rằng các giả thiết của Hệ quả của Mệnh đề 7 được thỏa mãn khi $ \mathcal{T}_1 = \mathcal{T}_2 $ (\S 1, no. 2, Hệ quả 2 của Mệnh đề 2).

### 4. KHÔNG GIAN CON CỦA CÁC KHÔNG GIAN ĐẦY ĐỦ

#### Mệnh đề 8 {#top-ii-s3-prop-8 .statement}

Mọi không gian con đóng của một không gian đầy đủ đều đầy đủ. Mọi không gian con đầy đủ của một không gian đều Hausdorff (đầy đủ hoặc không) đều đóng.

Cho $ X $ là một không gian đầy đủ và cho $ A $ là một không gian con đóng của $ X $. Nếu $ \mathfrak{F} $ là một lọc Cauchy trên $ A $, thì nó là một cơ sở lọc Cauchy trên $ X $ (mục 1, Mệnh đề 3) và do đó hội tụ đến một điểm $ x \in X $; nhưng vì $ A $ đóng nên ta có $ x \in A $, và do đó $ \mathfrak{F} $ hội tụ trong không gian con $ A $.

Bây giờ cho $ \overline{A} $ là một tập con không đóng của một không gian đều Hausdorff $ X $, và cho $ b \in \overline{A} - A $. Vết $ \mathfrak{B}_A $ trên $ A $ của lọc lân cận $ \mathfrak{B} $ của $ b $ trong $ X $ là một lọc Cauchy trên $ A $; nhưng nó không thể hội tụ đến một điểm $ c \in A $, vì nếu vậy $ c $ sẽ là một điểm giới hạn của $ \mathfrak{B} $ (mục 2, Mệnh đề 5, Hệ quả 3), điều này là vô lý vì $ b \neq c $ và $ X $ là Hausdorff.

#### Mệnh đề 9 {#top-ii-s3-prop-9 .statement}

Cho $ X $ là một không gian đều và cho $ A $ là một tập con trù mật của $ X $ sao cho mọi cơ sở lọc Cauchy trên $ A $ đều hội tụ trong $ X $. Khi đó $ X $ là đầy đủ.

Chỉ cần chứng minh rằng mọi lọc Cauchy cực tiểu $ \mathfrak{F} $ trên $ X $ đều hội tụ. Vì $ A $ trù mật và vì mỗi tập thuộc $ \mathfrak{F} $ đều có phần trong không rỗng (mục 2, Hệ quả 4 của Mệnh đề 5), vết $ \mathfrak{F}_A $ của $ \mathfrak{F} $ trên $ A $ là một lọc Cauchy trên $ A $, nên hội tụ đến một điểm $ x_0 \in X $. Vì $ \mathfrak{F} $ thô hơn lọc trên $ X $ sinh bởi $ \mathfrak{F}_A $, suy ra $ \mathfrak{F} $ hội tụ đến $ x_0 $ (mục 2, Hệ quả 3 của Mệnh đề 5).

### 5. TÍCH VÀ GIỚI HẠN NGƯỢC CỦA CÁC KHÔNG GIAN ĐẦY ĐỦ

#### Mệnh đề 10 {#top-ii-s3-prop-10 .statement}

Mọi tích của các không gian đều đầy đủ đều là đầy đủ. Ngược lại, nếu một tích của các không gian đều không rỗng là đầy đủ, thì mỗi thừa số là một không gian đều đầy đủ.

Khẳng định thứ nhất là một hệ quả của đặc trưng hóa các lọc Cauchy và các lọc hội tụ trên một không gian tích (mục 1, Hệ quả 2 của Mệnh đề 4 và Chương I, § 7, mục 6, Hệ quả 1 của Mệnh đề 10). Ngược lại, giả sử

$$
X = \prod_{i \in I} X_i
$$

là đầy đủ (các $ X_i $ không rỗng) và cho $ \mathfrak{F}_x $ là một lọc Cauchy trên $ X_x $. Với mỗi $ i \neq x $ cho $ \mathfrak{F}_i $ là một lọc Cauchy trên $ X_i $, và xét lọc tích (Chương I, § 6, mục 7)

$$
\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i \text{ trên } X;
$$

$ \mathfrak{F} $ là một lọc Cauchy (mục 1, Hệ quả 2 của Mệnh đề 4), nên hội tụ, và do đó mỗi $ \operatorname{pr}_x \mathfrak{F} = \mathfrak{F}_x $ cũng hội tụ (Chương I, § 7, mục 6, Hệ quả 1 của Mệnh đề 10).

#### Hệ quả {#top-ii-s3-n5-cor-1 .statement}

*Cho* $(X_\alpha, f_{\alpha\beta})$ *là một hệ ngược các không gian đều.* *Nếu các* $ X_\alpha $ *là Hausdorff và đầy đủ, thì* $ X = \varprojlim X_\alpha $ *cũng vậy.*

Vì $ X $ là Hausdorff và có thể được đồng nhất với một *không gian con đóng* của $ \prod_{i \in I} X_\alpha $ (Chương I, § 8, mục 2, Hệ quả 2 của Mệnh đề 7); do đó hệ quả suy ra từ Mệnh đề 10 và Mệnh đề 8 (mục 4).

Một giới hạn ngược của các không gian đều Hausdorff đầy đủ $ X_\alpha $ có thể *rỗng*, ngay cả khi tất cả các $ X_\alpha $ đều không rỗng và tất cả các $ f_{\alpha\beta} $ đều toàn ánh, như được chỉ ra bởi trường hợp các không gian rời rạc (*Lý thuyết tập hợp*, Chương III, § 1, Bài tập 32). Tuy nhiên, ta có định lý sau:

#### Định lý 1 (Mittag-Leffler) {#top-ii-s3-thm-1 .statement}

*Cho* $(X_\alpha, f_{\alpha\beta})$ *là một hệ ngược các không gian đều Hausdorff đầy đủ, được chỉ số hóa bởi một tập có hướng* $ I $ *có một tập con đồng cuối đếm được; đồng thời, giả sử rằng, với mỗi* $ \alpha \in I $, $ X_\alpha $ *có một hệ cơ sở đếm được các lân cận* (*). *Cuối cùng, giả sử rằng với mỗi* $ \alpha \in I $ *tồn tại một chỉ số* $ \beta \geq \alpha $ *thỏa mãn điều kiện sau*:

(ML$_{\alpha\beta}$) *Với mỗi* $ \gamma \geq \beta $, $ f_{\alpha\gamma}(X_\gamma) $ *trù mật trong* $ f_{\alpha\beta}(X_\beta) $.

*Cho* $ X = \varprojlim X_\alpha $ *và cho* $ f_\alpha $ *là ánh xạ chính tắc* $ X \to X_\alpha $. *Khi đó với mỗi* $ \alpha \in I $ *và mỗi* $ \beta \geq \alpha $ *thỏa mãn* (ML$_{\alpha\beta}$), $ f_\alpha(X) $ *trù mật trong* $ f_{\alpha\beta}(X_\beta) $ *(và do đó* $ X $ *không rỗng nếu tất cả các* $ X_\alpha $ *đều không rỗng)*.

Cho $ (\lambda_n) $ là một dãy các chỉ số đồng cuối trong $ I $. Bắt đầu với một chỉ số $ \alpha_0 \in I $ và định nghĩa đệ quy một dãy tăng $ (\alpha_n) $ sao cho $ \alpha_n \geq \lambda_n $ và sao cho (ML$_{\alpha_n, \alpha_{n+1}}$) đúng. Rõ ràng dãy

(*) *Điều kiện này có nghĩa là không gian đều Hausdorff* $ X_\alpha $ *là khả metrizable; xem Chương IX, § 2, no. 4, Định lý 1.*

$(\alpha_n)$ là đồng cuối trong I. Ta sẽ viết f_{mn} thay cho f_{α_mα_n} khi m ≤ n, và ta đặt f_{n, n+1}(X_{α_{n+1}}) = Y_n. Khi đó, nếu m ≤ n, f_{mn}(Y_n) trù mật trong Y_m; vì theo định nghĩa f_{m, n+1}(X_{α_{n+1}}) trù mật trong

f_{m, m+1}(X_{α_{m+1}}) = Y_m, và f_{m, n+1}(X_{α_{n+1}}) = f_{mn}[f_{n, n+1}(X_{α_{n+1}})] = f_{mn}(Y_n).

Bằng quy nạp theo n và k ta có thể định nghĩa một hệ cơ sở (V_{kn})_{k∈\mathbf{N}} của các lân cận đóng đối xứng của X_{α_n} cho mỗi n sao cho

(2)
$ \overset{2}{V}_{k+1, n} \subset V_{kn} $,

(3)
$ (f_{n, n+1} × f_{n, n+1})(V_{k, n+1}) \subset V_{kn} $.

Thực vậy, cho (U_{kn})_{k∈\mathbf{N}} là một hệ cơ sở các lân cận của X_{α_n}. Nếu ta giả sử rằng các V_{kn} đã được định nghĩa cho một n cho trước và với mọi k ∈ \mathbf{N}, thì vì f_{n, n+1} liên tục đều ta có thể định nghĩa lân cận V_{k, n+1} bằng quy nạp theo k sao cho (3) được thỏa mãn và

$ \overset{2}{V}_{k+1, n+1} \subset V_{k, n+1} ∩ U_{k+1, n+1} $

Mệnh đề suy ra.

Bây giờ cho x_0 ∈ Y_0. Ta sẽ chứng minh rằng với mỗi số nguyên k > 0 tồn tại một điểm z ∈ X sao cho [x_0, f_{α_0}(z)] ∈ V_{k-1, 0}; điều này sẽ chứng minh định lý. Vì f_{n, n+1} (Y_{n+1}) trù mật trong Y_n, ta có thể định nghĩa bằng quy nạp một dãy các điểm x_n ∈ Y_n sao cho

(4)
$$ [x_n, f_{n, n+1}(x_{n+1})] ∈ V_{k+n, n} $$

Do (3) suy ra rằng nếu m ≤ n thì

(5)
$$ [f_{mn}(x_n), f_{m, n+1}(x_{n+1})] ∈ V_{k+n, m} $$

Từ đó ta kết luận rằng với m cố định dãy (f_{mn}(x_n))_{n≥m} là một dãy Cauchy trong X_{α_m} và do đó hội tụ đến một điểm z_m; vì bằng quy nạp từ (5) suy ra rằng, với mỗi cặp số nguyên p ≥ m, q > 0, ta có

(6)
$$ [f_{mp}(x_p), f_{m, p+q}(x_{p+q})] ∈ V_{k+p+q-1, m} ∘ V_{k+p+q-2, m} ∘ ... ∘ V_{k+p, m} $$

và nhờ (2) hiển nhiên rằng vế phải của (6) được chứa trong V_{k+p-1, m}. Cho q tăng vô hạn; suy ra đặc biệt rằng, với m = p = 0, ta có (x_0, z_0) ∈ V_{k-1, 0}, vì V_{k-1, 0} đóng. Mặt khác, từ các quan hệ z_m = \lim_{n→∞} f_{mn}(x_n) và từ tính liên tục của f_{m, m+1}, ta suy ra rằng f_{m, m+1}(z_{m+1}) = z_m với mỗi m ≥ 0. Với mỗi γ ∈ I tồn tại ít nhất một số nguyên n sao cho α_n ≥ γ; đặt $ z_\gamma = f_{\gamma, \alpha_n}(z_n) $ ta kiểm tra ngay rằng $ z_\gamma $ không phụ thuộc vào giá trị của $ n $ sao cho $ \alpha_n \geq \gamma $, và rằng họ $ (z_\alpha)_{\alpha \in I} $ như thế được định nghĩa là một điểm $ z $ của $ X = \varprojlim X_\alpha $. Vì $ f_{\alpha_0}(z) = z_0 $, chứng minh hoàn tất.

#### Hệ quả 1 {#top-ii-s3-thm-1-cor-1 .statement}

*Cho* $ (X_\alpha, f_{\alpha \beta}) $ *là một hệ ngược của các tập hợp được chỉ số hóa bởi một tập có hướng* $ I $ *có một tập con đồng cuối đếm được, và giả sử rằng các* $ f_{\alpha \beta} $ *đều toàn ánh. Khi đó nếu* $ X = \varprojlim X_\alpha $, *thì ánh xạ chính tắc* $ f_\alpha : X \to X_\alpha $ *là toàn ánh với mỗi* $ \alpha \in I $.

Hãy cho mỗi $ X_\alpha $ mang cấu đều rời rạc, và áp dụng Định lý 1.

#### Hệ quả 2 {#top-ii-s3-thm-1-cor-2 .statement}

*Cho* $ I $ *là một tập có hướng có một tập con đồng cuối đếm được. Cho* $ (X_\alpha, f_{\alpha \beta}) $ *và* $ (X'_\alpha, f'_{\alpha \beta}) $ *là hai hệ ngược của các tập hợp được chỉ số hóa bởi* $ I $, *và với mỗi* $ \alpha \in I $ *cho* $ u_\alpha : X_\alpha \to X'_\alpha $ *là một ánh xạ, sao cho các* $ u_\alpha $ *lập thành một hệ ngược các ánh xạ. Cho* $ u = \varprojlim u_\alpha $. *Cho* $ x = (x'_\alpha) $ *là một phần tử của*

$$
X' = \varprojlim X'_\alpha
$$

*thỏa mãn điều kiện sau: với mỗi* $ \alpha \in I $ *có một chỉ số* $ \beta \geq \alpha $ *sao cho với mọi* $ \gamma \geq \beta $ *ta có* $ f_{\alpha \gamma}(\overline{u}_\gamma^{-1}(x_\gamma)) = f_{\alpha \beta}(\overline{u}_\beta^{-1}(x'_\beta)) $. *Khi đó tồn tại một phần tử* $ x \in X $ *sao cho* $ u(x) = x' $.

Áp dụng Định lý 1 cho hệ ngược các tập hợp $ \overline{u}_\alpha^{-1}(x'_\alpha) $, mỗi tập mang độ đều rời rạc.

#### Ví dụ {#top-ii-s3-n5-exa-1 .statement}

Giả sử ta được cho trong $ C $: (i) một dãy $ (a_n) $ các điểm phân biệt sao cho dãy $ (|a_n|) $ tăng và tiến tới $ +\infty $; (ii) với mỗi $ n $, một hàm hữu tỉ $ z \to R_n(z) $ được định nghĩa trên $ C - \{a_n\} $ và có một cực tại $ a_n $; (iii) một dãy tăng $ (B_n) $ các đĩa mở tâm 0, có hợp là $ C $, và sao cho không có $ a_k $ nào nằm trên biên của bất kỳ đĩa nào trong các đĩa $ B_n $. Với mỗi $ n $, ký hiệu $ B'_n $ là giao của $ \overline{B}_n $ và phần bù trong $ C $ của tập hợp các điểm $ a_n $; và ký hiệu $ X_n $ là tập hợp tất cả các ánh xạ

$$
z \to S(z) = P(z) + \sum_{a_k \in B'_n} R_k(z)
$$

từ $ B'_n $ vào $ C $, trong đó $ P $ là hạn chế trên $ B'_n $ của một hàm liên tục trên $ \overline{B}_n $ và giải tích trong $ B_n $. Ta định nghĩa một metric trên $ X_n $ bằng cách đặt

$$
d_n(S_1, S_2) = \sup_{z \in B'_n} |S_1(z) - S_2(z)|.
$$

It is easily verified that $ X_n $ is *đầy đủ* đối với metric này. Sau cùng, với $ n \leq m $, ta định nghĩa một ánh xạ $ f_{nm} : X_m \to X_n $ sao cho nếu $ S \in X_m $ thì $ f_{nm}(S) $ là *hạn chế* của $ S $ đến $ B'_n $. Rõ ràng là các $ f_{nm} $ *liên tục đều* và $ (X_n, f_{nm}) $ là một hệ ngược của các không gian đều. Do đó, một phần tử của giới hạn ngược $ X = \lim_{\leftarrow} X_n $ có thể được đồng nhất một cách chính tắc với một hàm phân hình $ F $ trong $ \mathbf{C} $, mà các cực duy nhất của nó là các điểm $ a_n $, và sao cho với mỗi $ n $, $ F(z) - R_n(z) $ là khả chỉnh tại $ a_n $. Định lý cổ điển của Mittag-Leffler khẳng định rằng $ X $ không rỗng; nhờ Định lý 1, ta chỉ cần kiểm tra điều kiện (ML$_{nn}$) với mọi $ n $. Đặt
$$
S_n = P_n + \sum_{a_k \in B_n} R_k
$$
là một phần tử của $ X_n $, trong đó $ P_n $ liên tục trên $ \overline{B}_n $ và khả chỉnh trong $ B_n $; với mọi $ m \geq n $, đặt $ Q_{mn} $ là sự *hạn chế* của
$$
\sum_{a_h \in B_m - B_n} R_h \text{ đến } B'_n;
$$
tổng sau này là một hàm khả chỉnh trong một lân cận nào đó của $ \overline{B}_n $, do đó (theo định lý Taylor) với mỗi $ \varepsilon > 0 $ tồn tại một đa thức $ P_{mn} $ sao cho $ |Q_{mn}(z) - P_{mn}(z)| \leq \varepsilon $ trong $ B_n $; nếu $ S_m $ là sự hạn chế của $ S_n + Q_{mn} - P_{mn} $ đến $ B'_m $, ta có $ S_m \in X_m $ và $ |S_m(z) - S_n(z)| \leq \varepsilon $ trong $ B'_n $. Điều này chứng minh xong. \*

### 6. MỞ RỘNG CÁC HÀM LIÊN TỤC ĐỀU

Định lý về mở rộng bằng tính liên tục (Chapter I, § 8, no. 5, Định lý 1) có những bổ sung quan trọng khi các hàm đang xét lấy giá trị trong một không gian đều Hausdorff đầy đủ.

#### Mệnh đề 11 {#top-ii-s3-prop-11 .statement}

*Cho $ A $ là một tập con trù mật của một không gian tôpô $ X $, và cho $ f $ là một ánh xạ từ $ A $ vào một không gian đều Hausdorff đầy đủ $ X' $. Khi đó $ f $ có thể được mở rộng bằng tính liên tục đến $ X $ khi và chỉ khi, với mỗi $ x \in X $, ảnh dưới $ f $ của vết trên $ A $ của lọc lân cận của $ x $ trong $ X $ là một cơ sở lọc Cauchy trong $ X' $.

Điều này suy ra từ định lý mở rộng bằng tính liên tục (loc. cit.) vì $ X' $ chính quy (\$ 1, no. 2, Mệnh đề 3) và vì trên $ X' $ các lọc hội tụ cũng chính là các lọc Cauchy.

Khi $ X $ cũng là một không gian đều, có định lý sau:

#### Định lý 2 {#top-ii-s3-thm-2 .statement}

*Cho $ f $ là một hàm được xác định trên một không gian con trù mật $ A $ của một không gian đều $ X $, nhận giá trị trong một không gian đều Hausdorff đầy đủ $ X' $, và giả sử rằng $ f $ liên tục đều trên $ A $. Khi đó $ f $ có thể được kéo dài ra toàn bộ $ X $ nhờ tính liên tục, và hàm kéo dài $ \overline{f} $ là liên tục đều.*

Sự tồn tại của $ \overline{f} $ là một hệ quả ngay lập tức của các Mệnh đề 3 và 11 của no. 1. Ta chứng minh rằng $ \overline{f} $ là liên tục đều. Cho $ V' $ là một lân cận đối xứng đóng của $ X' $, và cho $ V $ là một lân cận của $ X $ sao cho, khi $ x $ và $ y $ thuộc $ A $ và là $ V $-gần nhau, thì $ f(x) $ và $ f(y) $ là $ V' $-gần nhau. Ta có thể giả sử rằng $ V $ là bao đóng trong $ X \times X $ của một lân cận $ W $ của $ A $ ($ \S $ 2, no. 4, Proposition 6). Ta có $[ \bar{f}(x), \bar{f}(y) ] \in V' $ khi $ (x, y) \in W $; vì $ \bar{f} \times \bar{f} $ liên tục trên $ X \times X $ (Chương I, $ \S $ 4, no. 1, Proposition 1) nên ta cũng có $[ \bar{f}(x), \bar{f}(y) ] \in V' $ khi $ (x, y) \in V = \overline{W} $, vì $ V' $ là đóng (Chương I, $ \S $ 2, no. 1, Định lý 1).

Q.E.D.

#### Hệ quả {#top-ii-s3-n6-cor-1 .statement}

*Cho $ X_1, X_2 $ là hai không gian đều Hausdorff đầy đủ, và cho $ Y_1, Y_2 $ lần lượt là các không gian con trù mật của $ X_1, X_2 $. Khi đó mọi đẳng cấu $ f $ của $ Y_1 $ lên $ Y_2 $ đều kéo dài thành một đẳng cấu của $ X_1 $ lên $ X_2 $.*

$ f $ là liên tục đều trên $ Y_1 $, do đó (Định lý 2) được mở rộng thành một ánh xạ liên tục đều $ \bar{f} : X_1 \to X_2 $. Tương tự, nghịch đảo $ g $ của $ f $ được mở rộng thành một ánh xạ liên tục đều $ \bar{g} : X_2 \to X_1 $. Do đó, ánh xạ $ \bar{g} \circ \bar{f} $ là một ánh xạ liên tục từ $ X_1 $ vào chính nó mà hạn chế trên $ Y_1 $ là ánh xạ đồng nhất; theo nguyên lý mở rộng các ánh xạ đồng nhất (Chương I, $ \S $ 8, no. 1, Hệ quả 1 của Mệnh đề 2) $ \bar{g} \circ \bar{f} $ vì thế là ánh xạ đồng nhất của $ X_1 $; tương tự $ \bar{f} \circ \bar{g} $ là ánh xạ đồng nhất của $ X_2 $. Do đó (*Lý thuyết tập hợp*, R, $ \S $ 2, no. 12) $ \bar{f}^{-1} $ và $ \bar{g} $ là các song ánh và là nghịch đảo của nhau; chúng cũng liên tục đều và do đó là các đẳng cấu ($ \S $ 2, no. 1, Mệnh đề 2).

Cần lưu ý rằng nếu $ f $ là một ánh xạ liên tục đều *song ánh* từ $ Y_1 $ lên $ Y_2 $, thì phép mở rộng liên tục của nó *không nhất thiết vừa đơn ánh vừa toàn ánh* (Bài tập 3).

### 7. Sự hoàn chỉnh của một không gian đều

#### Định lý 3 {#top-ii-s3-thm-3 .statement}

*Cho $ X $ là một không gian đều. Khi đó tồn tại một không gian đều Hausdorff đầy đủ $ \hat{X} $ và một ánh xạ liên tục đều $ i : X \to \hat{X} $ có tính chất sau:*

(P) *Cho bất kỳ ánh xạ liên tục đều nào $ f $ từ $ X $ vào một không gian đều Hausdorff đầy đủ $ Y $, tồn tại duy nhất một ánh xạ liên tục đều $ g : \hat{X} \to Y $ sao cho $ f = g \circ i $.*

*Nếu $ (i_1, X_1) $ là một cặp khác gồm một không gian đều Hausdorff đầy đủ $ X_1 $ và một ánh xạ liên tục đều $ i_1 : X \to X_1 $ có tính chất (P), thì tồn tại duy nhất một đẳng cấu $ \varphi : \hat{X} \to X_1 $ sao cho $ i_1 = \varphi \circ i $.*

1) Định nghĩa của $ \hat{X} $. Cho $ \hat{X} $ là tập hợp các bộ lọc Cauchy cực tiểu (no. 2) trên $ X $. Ta sẽ định nghĩa một cấu trúc đều trên $ \hat{X} $. Với mục đích này, nếu $ V $ là bất kỳ lân cận đối xứng nào của $ X $, hãy ký hiệu $ \tilde{V} $ là tập hợp mọi cặp $ (\mathcal{K}, \mathcal{Y}) $ của các bộ lọc Cauchy cực tiểu có chung một tập $ V $-nhỏ. Ta sẽ chứng minh rằng các tập $ \tilde{V} $ tạo thành một hệ cơ bản các lân cận của một cấu trúc đều trên $ \hat{X} $:

(i) Vì mỗi $ \mathcal{K} \in \hat{X} $ là một bộ lọc Cauchy, theo định nghĩa ta có $ (\mathcal{K}, \mathcal{K}) \in \tilde{V} $ với mọi lân cận đối xứng $ V $ của $ X $; do đó tiên đề $ (U'_1) $ được thỏa mãn.

(ii) Nếu $ V $ và $ V' $ là hai lân cận đối xứng của $ X $, thì $ W = V \cap V' $ là một lân cận đối xứng, và mọi tập $ W $-nhỏ cũng là $ V $-nhỏ và $ V' $-nhỏ; do đó $ \tilde{W} \subset \tilde{V} \cap \tilde{V}' $, điều này chứng tỏ $ (B_1) $.

(iii) Các tập $ \tilde{V} $ là đối xứng theo định nghĩa, do đó $ (U''_1) $ được thỏa mãn.

(iv) Cho một entourage đối xứng $ V $ của $ X $, đặt $ W $ là một entourage đối xứng sao cho $ \tilde{V} \subset V $. Xét ba bộ lọc Cauchy cực tiểu $ \mathcal{K}, \mathcal{Y}, \mathcal{B} $ sao cho $ (\mathcal{K}, \mathcal{Y}) \in \tilde{W} $ và $ (\mathcal{Y}, \mathcal{B}) \in \tilde{W} $; khi đó có hai tập $ W $-nhỏ $ M, N $ sao cho $ M \in \mathcal{K} \cap \mathcal{Y} $ và $ N \in \mathcal{Y} \cap \mathcal{B} $. Vì $ M $ và $ N $ thuộc $ \mathcal{Y} $, $ M \cap N $ không rỗng và do đó (mục 1, Mệnh đề 1) $ M \cup N $ là $ \tilde{W} $-nhỏ và suy ra $ V $-nhỏ; vì $ M \cup N $ thuộc $ \mathcal{K} $ và thuộc $ \mathcal{B} $ ta có $ \tilde{W} \subset \tilde{V} $; do đó $ (U'''_1) $ được thỏa mãn.

Tiếp theo ta chứng minh rằng không gian đều $ \hat{X} $ là Hausdorff. Cho $ \mathcal{K}, \mathcal{Y} $ là hai bộ lọc Cauchy cực tiểu trên $ X $ sao cho $ (\mathcal{K}, \mathcal{Y}) \in \hat{X} $ với mọi entourage đối xứng $ V $ của $ X $. Suy ra ngay rằng các tập $ M \cup N $, với $ M \in \mathcal{K} $ và $ N \in \mathcal{Y} $, lập thành một cơ sở của một bộ lọc $ \mathcal{B} $ thô hơn $ \mathcal{K} $ và $ \mathcal{Y} $. Bây giờ $ \mathcal{B} $ là một bộ lọc Cauchy, vì với mọi entourage đối xứng $ V $ của $ X $ theo giả thiết có một tập $ V $-nhỏ $ P $ thuộc cả $ \mathcal{K} $ và $ \mathcal{Y} $ và do đó thuộc $ \mathcal{B} $. Theo định nghĩa của các bộ lọc Cauchy cực tiểu, ta có $ \mathcal{K} = \mathcal{B} = \mathcal{Y} $, và điều này cho thấy rằng $ \hat{X} $ là Hausdorff.

2) Định nghĩa của $ i $; cấu trúc đều của $ X $ là ảnh ngược qua $ i $ của cấu trúc của $ \hat{X} $. Ta biết rằng với mỗi $ x \in X $ thì bộ lọc lân cận $ \mathfrak{B}(x) $ của $ x $ trong $ X $ là một bộ lọc Cauchy cực tiểu (no. 2, Mệnh đề 5, Hệ quả 1). Vì vậy ta định nghĩa $ i(x) = \mathfrak{B}(x) $. Đặt $ f = i \times i $; ta sẽ chứng minh rằng với mỗi lân cận đối xứng $ V $ của $ X $ ta có $ j^{-1}(\tilde{V}) \subset V \cup j^{-1}[(\tilde{V})^3] $, và điều này sẽ chứng minh mệnh đề của ta (\S 2, no. 4). Bây giờ, nếu $[i(x), i(y)] \in \tilde{V}$, thì có một tập $ V $-nhỏ $ M $ là lân cận của cả $ x $ và $ y $, do đó $(x, y) \in V$. Ngược lại, nếu $(x, y) \in V$, thì thấy ngay rằng tập $ V(x) \cup V(y) $ là $ V $-nhỏ và là lân cận của cả $ x $ và $ y $.

3) $ \hat{X} $ là đầy đủ và $ i(X) $ trù mật trong $ \hat{X} $. Phần vết trên $ i(X) $ của một lân cận $ \tilde{V}(\mathcal{X}) $ của một điểm $ \mathcal{X} \in X $ là tập gồm mọi $ i(x) $ sao cho

$$
(\mathcal{X}, i(x)) \in \tilde{V}.
$$

Quan hệ này có nghĩa là có một lân cận $ V $-nhỏ của $ x $ trong $ X $ thuộc $ \mathcal{X} $, tức là $ x $ là một điểm trong của một tập $ V $-nhỏ của $ \mathcal{X} $. Đặt $ M $ là hợp của các phần trong của mọi tập $ V $-nhỏ của $ \mathcal{X} $; khi đó $ M $ thuộc $ \mathcal{X} $ (no. 2, Mệnh đề 5, Hệ quả 4) và từ những điều đã nói suy ra rằng $ \tilde{V}(\mathcal{X}) \cap i(X) = i(M) $. Suy ra rằng:

(i) $ \tilde{V}(\mathcal{X}) \cap i(X) $ không rỗng, do đó $ i(X) $ trù mật trong $ \hat{X} $.
(ii) Phần vết của $ \tilde{V}(\mathcal{X}) $ trên $ i(X) $ thuộc cơ sở lọc $ i(\mathcal{X}) $ trên $ X $; do đó cơ sở lọc này hội tụ trong $ \hat{X} $ tới điểm $ \mathcal{X} $.

Khi đó, cho $ \mathfrak{F} $ là một lọc Cauchy trên $ i(X) $; suy ra từ 2) trên và Mệnh đề 4 của no. 1, $ \overline{i^1}(\mathfrak{F}) $ là một cơ sở của một lọc Cauchy $ \mathfrak{G} $ trên $ X $. Cho $ \mathcal{X} $ là một lọc Cauchy tối tiểu thô hơn $ \mathfrak{G} $ (no. 2, Mệnh đề 5); khi đó $ i(\mathcal{X}) $ là một cơ sở lọc Cauchy trên $ i(X) $ (no. 1, Mệnh đề 3), và $ \mathfrak{F} = i[\overline{i^1}(\mathfrak{F})] $ mịn hơn lọc có cơ sở là $ i(\mathcal{X}) $. Vì lọc sau hội tụ trong $ \hat{X} $, nên $ \mathfrak{F} $ cũng hội tụ, và do đó Mệnh đề 9 của no. 4 cho thấy $ \hat{X} $ là đầy đủ.

4) Kiểm tra tính chất (P). Cho $ f $ là một ánh xạ liên tục đều của $ X $ vào một không gian Hausdorff đầy đủ. Trước hết ta chứng minh rằng tồn tại một ánh xạ liên tục đều duy nhất $ g_0 : i(X) \to Y $ sao cho $ f = g_0 \circ i $. Vì $ f $ liên tục, ta có

$$
f(x) = \lim f(\mathfrak{B}(x)),
$$

do đó nếu ta đặt $ g_0(i(x)) = \lim f(\mathfrak{B}(x)) $, ta có $ f = g_0 \circ i $; vì vậy chỉ còn phải chứng minh rằng $ g_0 $ là liên tục đều trên $ i(X) $. Cho $ U $ là một bao lân cận của $ Y $ và cho $ V $ là một bao lân cận đối xứng của $ X $ sao cho quan hệ $ (x, x') \in V $ suy ra $ (f(x), f(x')) \in U $; ta đã thấy trong 2) rằng quan hệ $ (i(x), i(x')) \in \tilde{V} $ suy ra $ (x, x') \in V $, do đó cũng suy ra
$$
(g_0(i(x)), g_0(i(x'))) \in U,
$$
điều đó chứng minh mệnh đề của chúng ta.

Cho $ g $ là mở rộng của $ g_0 $ bởi tính liên tục lên $ \hat{X} $ (no. 6, Định lý 2); khi đó $ f = g \circ i $, và hiển nhiên $ g $ là ánh xạ liên tục duy nhất của $ \hat{X} $ vào $ Y $ thỏa mãn quan hệ này, vì $ i(X) $ trù mật trong $ \hat{X} $ (Chương I, § 8, no. 1, Mệnh đề 2, Hệ quả 1).

Q.E.D.

#### Định nghĩa 4 {#top-ii-s3-def-4 .statement}

*Không gian Hausdorff đầy đủ* $ \hat{X} $ *được định nghĩa trong chứng minh của Định lý 3 được gọi là bù Hausdorff của* $ X $, *và ánh xạ* $ i : X \to \hat{X} $ *được gọi là ánh xạ chính tắc của* $ X $ *vào bù Hausdorff của nó.*

Ta cũng lưu ý các sự kiện sau:

#### Mệnh đề 12 {#top-ii-s3-prop-12 .statement}

(i) *Không gian con* $ i(X) $ *trù mật trong* $ \hat{X} $.
(ii) *Đồ thị của quan hệ tương đương* $ i(x) = i(x') $ *là giao của các lân cận của* $ X $.
(iii) *Cấu trúc đều của* $ X $ *là ảnh ngược qua* $ i $ *của cấu trúc đều của* $ \hat{X} $ *[hoặc của cấu trúc đều của không gian con* $ i(X) $].
(iv) *Các lân cận của* $ i(X) $ *là các ảnh qua* $ i \times i $ *của các lân cận của* $ X $, *và các bao đóng trong* $ \hat{X} \times \hat{X} $ *của các lân cận của* $ i(X) $ *tạo thành một hệ cơ bản các lân cận của* $ \hat{X} $.

(i) và (iii) đã được chứng minh trong quá trình chứng minh Định lý 3; (iv) là hệ quả của (i) và (iii) nhờ các kết quả tổng quát đã chứng minh trước đó (\S 2, no. 4, Nhận xét và Mệnh đề 6). Quan hệ
$$
i(x) = i(x')
$$
theo định nghĩa có nghĩa là $ x $ và $ x' $ có cùng bộ lọc lân cận. Nhưng điều này suy ra, theo định nghĩa, rằng $ (x, x') \in V $ với mọi lân cận $ V $ của $ X $, và chiều ngược lại hiển nhiên.

#### Hệ quả {#top-ii-s3-n7-cor-1 .statement}

*Nếu* $ X $ *là một không gian đều Hausdorff, thì ánh xạ chính tắc* $ i : X \to \hat{X} $ *là một đẳng cấu của* $ X $ *lên một không gian con trù mật của* $ \hat{X} $.

Khi $ X $ là Hausdorff, $ \hat{X} $ được gọi là *sự hoàn chỉnh* của $ X $, và nói chung ta *đồng nhất* $ X $ với một tập con trù mật của $ \hat{X} $ bằng $ i $.

#### Nhận xét {#top-ii-s3-n7-rem-1 .statement}

Nếu sự đồng nhất này được thực hiện, thì các bộ lọc Cauchy cực tiểu trên X chỉ là các vết trên X của các bộ lọc lân cận của các điểm của $ \hat{X} $; điều này suy ra từ chứng minh Định lý 3.

Hệ quả của Mệnh đề 12 đặc trưng hóa sự hoàn chỉnh của một không gian đều Hausdorff:

#### Mệnh đề 13 {#top-ii-s3-prop-13 .statement}

*Nếu Y là một không gian đều Hausdorff đầy đủ và X là một không gian con trù mật của Y, thì đơn ánh chính tắc $ X \to Y $ mở rộng thành một đẳng cấu của $ \hat{X} $ lên Y.*

Với mọi ánh xạ liên tục đều của X vào một không gian đều Hausdorff đầy đủ Z, theo Định lý 2 của no. 6, đều mở rộng duy nhất thành một ánh xạ liên tục đều của Y vào Z.

#### Mệnh đề 14 {#top-ii-s3-prop-14 .statement}

*Cho X là một không gian đều Hausdorff đầy đủ, $ \mathcal{U} $ là cấu trúc đều của nó, và cho Z là một không gian con trù mật của X. Nếu $ \mathcal{U}' $ là một cấu trúc đều trên X thô hơn $ \mathcal{U} $ và cảm sinh trên Z cùng một cấu trúc đều như $ \mathcal{U} $, thì $ \mathcal{U} = \mathcal{U}' $.*

Kí hiệu X' là tập hợp X với cấu trúc đều $ \mathcal{U}' $. Hợp thành của ánh xạ chính tắc $ X' \to \hat{X}' $ và ánh xạ đồng nhất $ X \to X' $ là một ánh xạ liên tục đều $ \varphi : X \to \hat{X}' $. Vì Z là Hausdorff đối với cấu trúc đều cảm sinh bởi $ \mathcal{U}' $, nên hạn chế của $ \varphi $ trên Z theo giả thiết là một đẳng cấu của Z lên không gian con trù mật $ \varphi(Z) $ của $ \hat{X}' $; suy ra (no. 6, Hệ quả của Định lý 2) rằng chính $ \varphi $ là một đẳng cấu của X lên $ \hat{X}' $, do đó $ X' = \hat{X}' $ và $ \mathcal{U}' = \mathcal{U} $.

#### Mệnh đề 15 {#top-ii-s3-prop-15 .statement}

*Cho X và X' là hai không gian đều. Với mỗi ánh xạ liên tục đều $ f : X \to X' $ có một ánh xạ liên tục đều duy nhất $ \hat{f} : \hat{X} \to \hat{X}' $ sao cho biểu đồ

$$
\begin{array}{ccc}
X & \xrightarrow{i'} & X' \\
i \downarrow & & \downarrow i' \\
\hat{X} & \xrightarrow{\hat{f}} & \hat{X}'
\end{array}
$$

giao hoán (*), trong đó $ i : X \to \hat{X} $ và $ i' : X' \to \hat{X}' $ là các ánh xạ chính tắc.

Áp dụng Định lý 3 cho hàm $ i' \circ f : X \to \hat{X}' $.

#### Hệ quả {#top-ii-s3-n7-cor-2 .statement}

*Nếu $ f : X \to X' $ và $ g : X' \to X'' $ là hai ánh xạ liên tục đều và $ h = g \circ f $, thì $ \hat{h} = \hat{g} \circ \hat{f} $.*

Đây là một hệ quả ngay lập tức của tính duy nhất trong Mệnh đề 15.

(*) Nói cách khác, $ i' \circ f = \hat{f} \circ i $.

### 8. KHÔNG GIAN ĐỀU HAUSDORFF LIÊN KẾT VỚI MỘT KHÔNG GIAN ĐỀU

#### Mệnh đề 16 {#top-ii-s3-prop-16 .statement}

Cho $ X $ là một không gian đều và $ i $ là ánh xạ chính tắc của $ X $ vào sự hoàn thành Hausdorff $ \hat{X} $. Với mỗi ánh xạ liên tục đều $ f $ của $ X $ vào một không gian đều Hausdorff $ Y $, tồn tại một ánh xạ liên tục đều duy nhất $ h : i(X) \to Y $ sao cho $ f = h \circ i $.

Ta có thể đồng nhất $ Y $ với một không gian con của sự hoàn thành của nó $ \hat{Y} $ (no. 7, Hệ quả của Mệnh đề 12), và khi đó $ f $ có thể được xét như một ánh xạ liên tục đều của $ X $ vào $ \hat{Y} $. Nhờ Định lý 3, khi đó $ f $ có dạng $ f = g \circ i $, trong đó $ g $ là một ánh xạ liên tục đều của $ \hat{X} $ vào $ \hat{Y} $. Nếu $ h $ là hạn chế của $ g $ lên $ i(X) $, thì rõ ràng $ f = h \circ i $, và $ h $ ánh xạ $ i(X) $ vào $ Y $. Tính duy nhất của $ h $ là tầm thường.

Vì vậy cặp $ (i, i(X)) $ là nghiệm của một bài toán ánh xạ phổ quát (Lý thuyết tập hợp, Chương IV, § 3, no. 1), ở đây lần này ta lấy các $ \Sigma $-tập hợp là các không gian đều Hausdorff, và các $ \sigma $-đồng cấu (resp. $ \alpha $-ánh xạ) là các ánh xạ liên tục đều (resp. các ánh xạ liên tục đều của $ X $ vào một không gian đều Hausdorff).

#### Định nghĩa 5 {#top-ii-s3-def-5 .statement}

Không gian đều Hausdorff $ i(X) $ được định nghĩa trong chứng minh của Định lý 3 được gọi là không gian đều Hausdorff liên kết với $ X $.

Sự hoàn thành Hausdorff của $ X $ như vậy là sự hoàn thành của không gian đều Hausdorff liên kết với $ X $.

#### Hệ quả {#top-ii-s3-n8-cor-1 .statement}

Cho $ X, Y $ là hai không gian đều và $ X', Y' $ là các không gian Hausdorff liên kết. Với mỗi ánh xạ liên tục đều $ f : X \to Y $ tồn tại một ánh xạ liên tục đều duy nhất $ f' : X' \to Y' $ sao cho biểu đồ

$$
\begin{array}{ccc}
X & \xrightarrow{f} & Y \\
i \downarrow & & \downarrow i' \\
X' & \xrightarrow{f'} & Y'
\end{array}
$$

là giao hoán, trong đó $ i $ và $ i' $ là các ánh xạ chính tắc.

Áp dụng Mệnh đề 16 cho $ i' \circ f : X \to Y' $.

Không gian Hausdorff liên kết với một không gian đều cũng có thể được đặc trưng bởi tính chất sau đây:

#### Mệnh đề 17 {#top-ii-s3-prop-17 .statement}

Cho $ X $ là một không gian đều, $ i(X) $ là không gian Hausdorff liên kết của nó, và cho $ f $ là một ánh xạ của $ X $ lên một không gian đều Hausdorff $ X' $, sao cho cấu trúc đều của $ X $ là ảnh ngược qua $ f $ của cấu trúc đều của $ X' $. Khi đó ánh xạ $ g : i(X) \to X' $ sao cho $ f = g \circ i $ là một đẳng cấu.

Theo Mệnh đề 16, $ g $ là liên tục đều; đồng thời $ g $ hiển nhiên là toàn ánh, và cũng là đơn ánh vì đẳng thức $ f(x) = f(y) $ suy ra theo định nghĩa rằng $ (x, y) $ thuộc mọi lân cận của $ X $, và do đó $ i(x) = i(y) $ (no. 7, Mệnh đề 12). Cuối cùng, các lân cận của $ X' $ là các ảnh qua $ f \times f $ của các lân cận của $ X $ ($ \S 2 $, no. 4, Nhận xét), do đó chúng cũng là các ảnh qua $ g \times g $ của các lân cận của $ i(X) $ (no. 7, Mệnh đề 12); suy ra điều phải chứng minh.

#### Nhận xét {#top-ii-s3-n8-rem-1 .statement}

Cho $ R $ là quan hệ tương đương $ i(x) = i(x') $ trên $ X $. Ta đã thấy (no. 7, Mệnh đề 12) rằng đồ thị $ C $ của $ R $ là giao của mọi lân cận của $ X $. Hiển nhiên mọi tập mở (và do đó mọi tập đóng) trong $ X $ đều *bão hòa* đối với $ R $; xét đến định nghĩa của ảnh ngược của một tôpô, ta kết luận rằng song ánh chính tắc của không gian thương $ X/R $ lên $ i(X) $ cảm sinh bởi $ i $ là một *đồng phôi*. Không gian Hausdorff liên kết với $ X $ vì thế có thể được đồng nhất, *với tư cách là* không gian tôpô, với $ X/R $. Ánh xạ chính tắc $ i : X \to i(X) $ là mở và đóng, và thậm chí là thực sự (Chương I, $ \S 10 $, no. 2, Ví dụ).

Cho $ X' $ là một không gian đều khác, $ C' $ là giao của mọi lân cận của $ X' $, và $ R' $ là quan hệ tương đương có đồ thị là $ C' $. Cho $ f : X \to X' $ là một ánh xạ *liên tục*. Vì ảnh ngược qua $ f $ của bất kỳ lân cận nào của $ f(x) $ là một lân cận của $ x $, suy ra ảnh ngược qua $ f $ của $ C'(f(x)) $ chứa $ C(x) $, và do đó $ f $ *tương thích* với $ R $ và $ R' $, và cảm sinh một ánh xạ liên tục $ X/R \to X'/R' $ (Chương I, $ \S 3 $, no. 4, Hệ quả của Mệnh đề 6). Điều này khái quát hóa hệ quả của Mệnh đề 16.

### 9. SỰ HOÀN THÀNH CỦA CÁC KHÔNG GIAN CON VÀ CÁC KHÔNG GIAN TÍCH

#### Mệnh đề 18 {#top-ii-s3-prop-18 .statement}

*Cho $ X $ là một tập hợp, cho $ (Y_\lambda)_{\lambda \in L} $ là một họ các không gian đều, và với mỗi $ \lambda \in L $ cho $ f_\lambda $ là một ánh xạ của $ X $ vào $ Y_\lambda $. Cho $ X $ mang cấu trúc đều thô nhất $ U $ sao cho mọi $ f_\lambda $ đều liên tục đều. Khi đó cấu trúc đều của sự hoàn thành Hausdorff $ \hat{X} $ của $ X $ là cấu trúc đều thô nhất sao cho mọi ánh xạ $ \hat{f}_\lambda : \hat{X} \to \hat{Y}_\lambda $ ($ \lambda \in L $) (no. 7, Proposition 15) đều liên tục đều. Hơn nữa, nếu $ j_\lambda $ là ánh xạ chính tắc của $ Y_\lambda $ vào $ \hat{Y}_\lambda $, và nếu $ g_\lambda = j_\lambda \circ f_\lambda $, thì $ \hat{X} $ có thể được đồng nhất với bao đóng trong $ \prod_{\lambda \in L} \hat{Y}_\lambda $ của ảnh của $ X $ dưới ánh xạ $ x \to (g_\lambda(x)) $.*

Cho $ X' $ (resp. $ Y'_\lambda $) là không gian đều Hausdorff liên kết với $ X $ (resp. $ Y_\lambda $), và cho $ f'_\lambda : X' \to Y'_\lambda $ là ánh xạ liên tục đều làm cho biểu đồ

$$
\begin{array}{ccc}
X & \xrightarrow{f_\lambda} & Y_\lambda \\
i \downarrow & & \downarrow j_\lambda \\
X' & \xrightarrow{f'_\lambda} & Y'_\lambda
\end{array}
$$

giao hoán (*i* là ánh xạ chính tắc).

Tính bắc cầu của các cấu trúc đều ban đầu (\S 2, no. 3, Proposition 5) cho thấy một mặt rằng $ \mathcal{U} $ là cấu trúc đều thô nhất sao cho các ánh xạ $ j_\lambda \circ f_\lambda : X \to Y'_\lambda $ đều liên tục, và mặt khác rằng $ \mathcal{U} $ cũng là ảnh ngược qua $ i $ của cấu trúc đều thô nhất $ \mathcal{U}' $ trên tập hợp $ X' $ sao cho các $ f'_\lambda $ đều liên tục. Bây giờ $ \mathcal{U}' $ là *Hausdorff*, vì nếu $ x_1, x_2 $ là hai điểm của $ X $ sao cho $ j_\lambda(f_\lambda(x_1)) = j_\lambda(f_\lambda(x_2)) $ với mỗi $ \lambda \in L $, thì $ (x_1, x_2) $ thuộc mọi lân cận của $ \mathcal{U} $ và do đó $ i(x_1) = i(x_2) $. Do đó Proposition 17 của no. 8 cho thấy $ \mathcal{U}' $ là cấu trúc đều của không gian Hausdorff $ X' $ liên kết với $ X $.

Do đó, song ánh $ x' \to (f'_\lambda(x')) $ đồng nhất $ X $ với một không gian con đều của tích $ \prod_\lambda Y'_\lambda $ (\S 2, no. 6, Mệnh đề 8). Vì các $ Y'_\lambda $ là Hausdorff, nên mỗi $ Y'_\lambda $ có thể được đồng nhất với một không gian con trù mật của phần hoàn thành $ \hat{Y}_\lambda $ của nó, và do đó $ \prod_\lambda Y'_\lambda $ có thể được đồng nhất với một không gian con trù mật của $ \prod_\lambda \hat{Y}_\lambda $ (Chương I, \S 4, no. 3, Mệnh đề 7). Nhưng $ \prod_\lambda \hat{Y}_\lambda $ là Hausdorff và đầy đủ (no. 5, Mệnh đề 10); do đó, bao đóng $ \overline{X'} $ của $ X' $ trong $ \prod_\lambda \hat{Y}_\lambda $ là một không gian con Hausdorff đầy đủ (no. 4, Mệnh đề 8) có thể được đồng nhất với phần hoàn thành Hausdorff $ \hat{X} $ của $ X $; dưới sự đồng nhất này, các ánh xạ $ \hat{f}_\lambda $ trở thành các phép chiếu lên các thừa số $ \hat{Y}_\lambda $, và mệnh đề được chứng minh.

#### Hệ quả 1 {#top-ii-s3-prop-18-cor-1 .statement}

*Cho $ X $ là một không gian đều và cho $ i $ là ánh xạ chính tắc của $ X $ vào phần hoàn thành Hausdorff $ \hat{X} $ của nó; cho $ A $ là một không gian con của $ X $ và $ j : A \to X $ là đơn ánh chính tắc. Khi đó $ \hat{j} : \hat{A} \to \hat{X} $ là một đẳng cấu từ $ \hat{A} $ lên bao đóng của $ i(A) $ trong $ \hat{X} $.*

#### Hệ quả 2 {#top-ii-s3-prop-18-cor-2 .statement}

*Cho $ (Y_\lambda)_{\lambda \in L} $ là một họ các không gian đều. Khi đó phần hoàn thành Hausdorff của không gian tích $ \prod_{\lambda \in L} Y_\lambda $ đẳng cấu chính tắc với tích $ \prod_{\lambda \in L} \hat{Y}_\lambda $.*

### Bài tập {#top-ii-s3-exercises}

Xem [các bài tập cho \S 3](exercises/s3/).
