---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 5
section_title: Separation of convex sets
lang: vi
source: evt-i-v
book_pages: TVS II.36-TVS II.40, TVS II.76-TVS II.81
pdf_pages: 0073-0077, 0113-0118
extraction: ocr
subsections:
    - "no": 1
      title: The Hahn-Banach theorem (geometric form)
      page: 36
      pdf_page: 73
    - "no": 2
      title: Separation of convex sets in a topological vector space
      page: 37
      pdf_page: 74
    - "no": 3
      title: Separation of convex sets in a locally convex space
      page: 38
      pdf_page: 75
    - "no": 4
      title: Approximation to convex functions
      page: 39
      pdf_page: 76
statements: 24
exercises: 30
content_sha256: 31a557e0879006a5a36b9aac20d1ec49331093b93d07fa36eacccc88e5340864
translated_from: content/en/evt/II/05_s5_separation_of_convex_sets.md
source_content_sha256: 8980b7d757e96a97ee6883201d0701256ff95f0727965a176942f2daab25fe89
translation_model: gpt-5.4-mini
translation_run: translate-vi-4ed2a9e8
glossary_version: 34
glossary_terms_sha256: c061be872cc771f37439d66febae732db42590f756b40941d63cc3ac40fa527e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. PHÂN LY CÁC TẬP HỢP LỒI

### 1. Định lý Hahn-Banach (dạng hình học)

#### Định lý 1 (Hahn-Banach) {#evt-ii-s5-thm-1 .statement}

— *Cho A là một tập hợp lồi mở không rỗng của không gian vectơ tôpô E và cho M là một đa tạp tuyến tính không rỗng không gặp A. Khi đó tồn tại một siêu phẳng đóng H chứa M và không gặp A.*

Nhờ tịnh tiến, bài toán có thể quy về trường hợp $ 0 \in A $, sao cho $ A $ là hấp thụ. Đặt $ p $ là *gauge* của $ A $ (II, p. 20), sao cho $ A $ là tập các điểm $ x \in E $ thỏa $ p(x) < 1 $. Mặt khác, gọi $ V $ là không gian con vectơ của $ E $ sinh bởi $ M $; do đó $ M $ là một siêu phẳng trong $ V $ không chứa $ 0 $, và vì thế tồn tại duy nhất một dạng tuyến tính $ f $ trên $ V $ sao cho $ M $ là tập các điểm $ y \in V $ mà $ f(y) = 1 $. Giả thiết $ M \cap A = \varnothing $ suy ra rằng với mọi $ y \in V $ sao cho $ f(y) = 1 $, ta có $ p(y) \geqslant 1 $; vì $ f $ và $ p $ là thuần nhất dương nên ta có $ f(y) \leqslant p(y) $ với mọi $ y \in V $ sao cho $ f(y) > 0 $; cuối cùng vì $ p(y) \geqslant 0 $ với mọi $ y \in V $, ta thấy rằng $ f(y) \leqslant p(y) $ với *mọi* $ y \in V $. Theo dạng giải tích của định lý Hahn-Banach (II, p. 22, th. 1) tồn tại một dạng tuyến tính $ h $ trên $ E $ mở rộng $ f $ và sao cho, với mọi $ x \in E $, $ h(x) \leqslant p(x) $. Gọi $ H $ là siêu phẳng trong $ E $ có phương trình $ h(x) = 1 $. Rõ ràng $ H \cap V = M $ và $ H \cap A = \varnothing $. Mặt khác phần bù của $ H $ trong $ E $ chứa tập hợp mở không rỗng $ A $, do đó $ H $ là *đóng* trong $ E $ (I, p. 11, hệ quả).

Q.E.D.

#### Nhận xét 1 {#evt-ii-s5-n1-rem-1 .statement}

Khi $ 0 \in M $, th. 1 có thể phát biểu như sau : tồn tại một *dạng tuyến tính liên tục trong E*, *sao cho* $ g(x) = 0 $ *trong* $ M $ *và* $ g(x) > 0 $ *trong* $ A $ (II, p. 8, mđ. 4).

#### Nhận xét 2 {#evt-ii-s5-n1-rem-2 .statement}

Nếu áp dụng định lý 1 cho trường hợp $ E $ mang tôpô lồi địa phương thô nhất (II, p. 25, *Ví dụ* 2), và nếu, để cho đơn giản, ta giả sử rằng $ 0 \in A $, thì ta thu được kết quả sau (bề ngoài không liên quan đến tôpô) : nếu $ A $ là một tập hợp lồi *hấp thụ* trong không gian vectơ thực $ E $ và nếu $ M $ là một đa tạp tuyến tính không rỗng không cắt $ A $, thì tồn tại một siêu phẳng $ H $ chứa $ M $ và sao cho $ A $ nằm về một phía của $ H $. Kết quả này không đúng với mọi tập hợp lồi $ A $ (II, p. 65, exerc. 5).

### 2. Sự phân biệt các tập hợp lồi trong một không gian vectơ tôpô

#### Định nghĩa 1 {#evt-ii-s5-def-1 .statement}

— *Hai tập hợp không rỗng* $ A, B $ *của một không gian vectơ tôpô thực* $ E $ *được gọi là được phân biệt bởi một siêu phẳng đóng* $ H $ *nếu* $ A $ *được chứa trong một trong hai nửa không gian đóng được xác định bởi* $ H $ *và* $ B $ *được chứa trong nửa không gian đóng kia*.

#### Định nghĩa 2 {#evt-ii-s5-def-2 .statement}

— *Hai tập hợp không rỗng* $ A, B $ *của một không gian vectơ tôpô thực được gọi là được phân biệt một cách chặt bởi siêu phẳng đóng* $ H $ *nếu* $ A $ *được chứa trong một trong hai nửa không gian mở được xác định bởi* $ H $, *và* $ B $ *được chứa trong nửa không gian mở kia*.

#### Mệnh đề 1 {#evt-ii-s5-prop-1 .statement}

— *Cho* $ A $ *là một tập hợp lồi mở không rỗng và cho* $ B $ *là một tập hợp lồi không rỗng trong một không gian vectơ tôpô thực* $ E $; *nếu* $ A $ *không gặp* $ B $ *thì tồn tại một siêu phẳng đóng phân biệt* $ A $ *với* $ B $.

Vì tập hợp $ C = A - B $ là mở, lồi (II, p. 9, prop. 7) và không rỗng, đồng thời $ 0 \notin C $. Theo định lý 1 của II, p. 36, tồn tại một dạng tuyến tính liên tục $ f \neq 0 $ trên $ E $ sao cho $ f(z) > 0 $ trong $ C $. Khi đó, với mọi $ x \in A $, và $ y \in B $, ta có $ f(x) > f(y) $. Đặt $ \alpha = \inf_{x \in A} f(x) $; $ \alpha $ là hữu hạn và ta có $ f(x) \geq \alpha $ với mọi $ x \in A $ và $ f(y) \leq \alpha $ với mọi $ y \in B $; siêu phẳng đóng $ H $ có phương trình $ f(z) = \alpha $ phân biệt $ A $ với $ B $.

#### Nhận xét {#evt-ii-s5-n2-rem-1 .statement}

— 1) Siêu phẳng $ H $ không gặp $ A $ (II, p. 15, prop. 1; nếu $ A $ và $ B $ là hai tập hợp không rỗng *mở* lồi không gặp nhau thì tồn tại một siêu phẳng đóng phân biệt $ A $ *một cách chặt* với $ B $.
2) Tuy nhiên, khi $ B $ không mở, thì không nhất thiết phải có một siêu phẳng đóng phân biệt $ A $ một cách chặt với $ B $, ngay cả khi $ E $ có số chiều hữu hạn, và ngay cả khi $ \overline{A} $ không gặp $ \overline{B} $ (II, p. 78, exerc. 12).

#### Định nghĩa 3 {#evt-ii-s5-def-3 .statement}

— *Với một tập con* $ A $ *của một không gian vectơ* $ E $, *một siêu phẳng* $ H $ *được gọi là một siêu phẳng đỡ của* $ A $, *nếu* $ H $ *chứa ít nhất một điểm của* $ A $ *và mọi điểm của* $ A $ *đều nằm về cùng một phía của* $ H $.

Cho $ f $ là một dạng tuyến tính trên $ E $ không đồng nhất bằng không; nói rằng siêu phẳng của phương trình $ f(x) = \alpha $ là một siêu phẳng đỡ của $ A $ có nghĩa là $ \alpha $ hoặc là phần tử nhỏ nhất hoặc là phần tử lớn nhất của tập $ f(A) \subset \mathbf{R} $. Nói cách khác, tồn tại một siêu phẳng đỡ của $ A $ song song với siêu phẳng có phương trình $ f(x) = 0 $, khi và chỉ khi, một trong các cận của tập $ f(A) $ là hữu hạn và thuộc về $ f(A) $.

#### Mệnh đề 2 {#evt-ii-s5-prop-2 .statement}

— *Cho* $ A $ *là một tập con compact không rỗng của một không gian vectơ tôpô* $ E $. *Với mọi siêu phẳng đóng* $ H $ *trong* $ E $, *tồn tại một siêu phẳng đỡ của* $ A $ *song song với* $ H $.

Vì, nếu $ f(x) = \gamma $ là một phương trình của $ H $, trong đó $ f $ là một dạng tuyến tính liên tục trong $ E $, thì hạn chế của $ f $ trên $ A $ là liên tục, do đó bị chặn và đạt các cận của nó trên $ A $ (GT, IV, § 6.1, th. 1).

Điều này chứng tỏ rằng tồn tại một hoặc hai siêu phẳng đỡ của $ A $ song song với $ H $; trường hợp thứ nhất chỉ có thể xảy ra khi $ A $ được chứa hoàn toàn trong một siêu phẳng song song với $ H $.

#### Mệnh đề 3 {#evt-ii-s5-prop-3 .statement}

— *Trong một không gian vectơ tôpô* $ E $, *cho* $ A $ *là một tập lồi đóng có phần trong không rỗng*. Khi đó mọi siêu phẳng đỡ của $ A $ đều đóng và mọi điểm biên của $ A $ đều thuộc ít nhất một siêu phẳng đỡ của $ A $.

Mọi siêu phẳng đỡ của $ A $ đều đóng, vì mọi điểm của $ A $ đều ở cùng một phía của siêu phẳng đó (II, p. 15, prop. 17). Ngoài ra, nếu $ x_0 $ là một điểm biên của $ A $, thì $ x_0 $ không thuộc tập lồi mở không rỗng $ \overset{\circ}{A} $; sau th. 1 của II, p. 36 tồn tại một siêu phẳng $ H $ chứa $ x_0 $ và không cắt $ \overset{\circ}{A} $. Vì $ A $ là bao đóng của $ \overset{\circ}{A} $ (II, p. 14, cor. 1 to prop. 16), suy ra từ prop. 17 của II, p. 15 rằng $ H $ là một siêu phẳng đỡ của $ A $.

### 3. Sự tách các tập lồi trong một không gian địa phương lồi

#### Mệnh đề 4 {#evt-ii-s5-prop-4 .statement}

— Cho $ A $ là một tập hợp lồi đóng không rỗng trong một không gian lồi địa phương $ E $ và cho $ K $ là một tập hợp lồi compact không rỗng trong $ E $, không giao nhau với $ A $. Khi đó tồn tại một siêu phẳng đóng $ H $ phân cách chặt $ A $ với $ K $.

Vì tồn tại một lân cận lồi mở $ V $ của 0 trong $ E $ sao cho $ A + V $ và $ K + V $ không giao nhau (GT, II, § 4.3, mệnh đề 4). Do $ A + V $ và $ K + V $ là lồi và mở trong $ E $, mệnh đề 1 của II, p. 37 cho thấy rằng tồn tại một siêu phẳng đóng $ H $ phân cách chặt $ A + V $ với $ K + V $, và $ a $ fortiori $ A $ với $ K $.

#### Nhận xét {#evt-ii-s5-n3-rem-1 .statement}

Trong một không gian lồi địa phương Hausdorff $ E $, cho $ A $ và $ B $ là hai tập hợp lồi đóng không rỗng rời nhau, nếu $ E $ hữu hạn chiều thì tồn tại một siêu phẳng đóng phân cách $ A $ khỏi (II, p. 78, bài tập 13); nhưng kết luận này không nhất thiết đúng khi $ E $ có vô hạn chiều (II, p. 78, bài tập 10 và 11).

#### Hệ quả 1 {#evt-ii-s5-prop-4-cor-1 .statement}

— Trong một không gian lồi địa phương, mọi tập hợp lồi đóng $ A $ là giao của các nửa không gian đóng chứa nó.

Thật vậy, với mọi điểm $ x \notin A $, tồn tại một siêu phẳng đóng phân cách chặt $ x $ khỏi $ A $ (dùng mệnh đề 4).

#### Hệ quả 2 {#evt-ii-s5-prop-4-cor-2 .statement}

— Trong một không gian lồi địa phương Hausdorff, mọi tập hợp lồi compact $ A $ là giao của các nửa không gian đóng chứa nó và được xác định bởi các siêu phẳng đỡ của $ A $.

Thật vậy, cho $ x_0 \notin A $; $ \{ x_0 \} $ là đóng, do đó tồn tại một siêu phẳng đóng $ H $ phân cách chặt $ x_0 $ khỏi $ A $ (mệnh đề 4); cho $ f(x) = \alpha $ là một phương trình của $ H $ ($ f $ là một dạng tuyến tính liên tục) và giả sử rằng $ f(x) > \alpha $ với mọi $ x \in A $. Nếu ta đặt $ \gamma = \inf_{x \in A} f(x) $, thì nửa không gian được xác định bởi $ f(x) \geq \gamma $ chứa $ A $, được xác định bởi siêu phẳng đỡ có phương trình $ f(x) = \gamma $, và không chứa $ x_0 $; do đó có hệ quả.

Có thể xảy ra là một tập hợp lồi đóng không compact và không có điểm trong, trong một không gian lồi địa phương, không có siêu phẳng đỡ đóng nào (II, p. 86, bài tập 18 : cf. cũng V, p. 71, bài tập 11).

#### Hệ quả 3 {#evt-ii-s5-prop-4-cor-3 .statement}

— Trong một không gian lồi địa phương, bao đóng của mỗi đa tạp tuyến tính $ M $ là giao của các siêu phẳng đóng chứa $ M $.

Với mọi $ x \notin \overline{M} $, cho $ H $ là một siêu phẳng đóng phân cách chặt $ x $ khỏi $ \overline{M} $;

do đó $ \overline{M} $ song song với $ H $; siêu phẳng đóng $ H_1 $, chứa $ \overline{M} $ và song song với $ H $ không chứa $ x $. Hệ quả theo sau.

#### Hệ quả 4 {#evt-ii-s5-prop-4-cor-4 .statement}

*Cho $ C $ là một tập hợp lồi đóng trong một không gian lồi địa phương $ E $. Một tập con $ A $ của $ E $ được chứa trong $ C $, khi, và chỉ khi, với mọi hàm affine liên tục nhận giá trị thực $ u $ trong $ E $ sao cho $ u(x) \geqslant 0 $ với mọi $ x $ trong $ C $, ta có $ u(y) \geqslant 0 $ với mọi $ y $ trong $ A $.*

Điều kiện này hiển nhiên là cần thiết. Ngược lại ta chứng minh rằng nó đủ; nếu một điểm $ x \in A $ không được chứa trong $ C $, thì tồn tại một siêu phẳng đóng có phương trình $ f(z) = \alpha $ phân cách chặt $ x $ với $ C $; nếu chẳng hạn giả sử rằng $ f(x) < \alpha $, thì hàm affine liên tục $ u = f - \alpha $ mâu thuẫn với các giả thiết.

#### Hệ quả 5 {#evt-ii-s5-prop-4-cor-5 .statement}

*Trong một không gian lồi địa phương $ E $, bao đóng của mỗi nón lồi $ C $ có đỉnh $ 0 $ là giao của các nửa không gian đóng chứa $ C $ được xác định bởi các siêu phẳng đóng đi qua $ 0 $.*

Vì $ \overline{C} $ là một nón lồi có đỉnh $ 0 $ (II, p. 13, Mệnh đề 14). Với $ x \notin \overline{C} $, tồn tại một siêu phẳng đóng $ H $ phân cách chặt $ x $ với $ \overline{C} $(Mệnh đề 4). Bây giờ chỉ còn cần áp dụng bổ đề sau :

#### Bổ đề 1 {#evt-ii-s5-lem-1 .statement}

— *Nếu một nón $ A $, có đỉnh $ 0 $, được chứa trong một nửa không gian mở được xác định bởi một siêu phẳng $ H $, thì nó được chứa trong một nửa không gian đóng được xác định bởi một siêu phẳng $ H_0 $, song song với $ H $ và đi qua $ 0 $.*

Cho $ f(z) = \alpha $ với $ \alpha < 0 $ là một phương trình của $ H $, sao cho $ f(z) = 0 $ là phương trình của $ H_0 $. Nếu tồn tại $ z \in A $ sao cho $ f(z) < 0 $, thì sẽ tồn tại $ \lambda > 0 $, sao cho $ f(\lambda z) = \alpha $, và vì $ \lambda z \in A $, điều này sẽ mâu thuẫn với giả thiết.

### 4. Xấp xỉ các hàm lồi

#### Mệnh đề 5 {#evt-ii-s5-prop-5 .statement}

*Cho $ X $ là một tập hợp lồi đóng trong một không gian lồi địa phương $ E $. Khi đó mọi hàm lồi nửa liên tục dưới $ f $ được xác định trên $ X $ là bao trên của một họ các hàm là các phần hạn chế lên $ X $ của các hàm affine tuyến tính liên tục trong $ E $.*

Thật vậy, tập $ A \subset E \times \mathbf{R} $ gồm các điểm $ (x, t) $ sao cho $ x \in X $ và $ t \geqslant f(x) $ là lồi (II, p. 17, mệnh đề 19) và đóng, vì hàm $ (x, t) \mapsto f(x) - t $ là nửa liên tục dưới. Khi đó lấy $ x $ là một điểm bất kỳ của $ X $ và lấy $ a \in \mathbf{R} $ sao cho $ a < f(x) $. Theo hệ quả 1 của II, p. 38, tồn tại một siêu phẳng đóng $ H $ trong $ E \times \mathbf{R} $, chứa $ (x, a) $ và không giao với $ A $. Mọi dạng tuyến tính liên tục trên $ E \times \mathbf{R} $ đều có dạng

$$
(z, t) \to u(z) + \lambda t ,
$$

trong đó $ \lambda \in \mathbf{R} $ và $ u $ là một dạng tuyến tính liên tục trên $ E $, suy ra $ H $ có một phương trình dạng $ u(z) + \lambda t = \alpha $, và vì $ H $ chứa $ (x, a) $ nên ta có $ \alpha = u(x) + \lambda a $. Bây giờ điểm $ (x, f(x)) \in A $ không thuộc $ H $ và do đó $ \lambda \neq 0 $. Chia cho $ -\lambda $, nếu cần, ta có thể viết phương trình của $ H $ dưới dạng $ t - a = u(z - x) $. Vì $ f(x) - a > 0 $, do đó ta có $ f(z) > u(z - x) + a $ với mọi $ z \in X $ và điều này chứng minh mệnh đề.

#### Nhận xét 1 {#evt-ii-s5-n4-rem-1 .statement}

Suy ra từ mệnh đề 5 rằng $ f $ là bao trên của một họ *tăng* có hướng các hàm là những hạn chế lên $ X $ của các hàm liên tục và lồi trên $ E $.

#### Nhận xét 2 {#evt-ii-s5-n4-rem-2 .statement}

Giả sử thêm rằng $ X $ là một hình nón lồi đóng có đỉnh 0 và rằng $ f $ là *thuần nhất dương*. Khi đó $ f $ là bao trên của một họ các hàm là những hạn chế lên $ X $ của các *dạng tuyến tính liên tục* trong $ E $. Thật vậy, lấy $ (u_\alpha) $ là một họ các hàm afin tuyến tính liên tục trong $ E $ mà các hạn chế lên $ X $ của chúng có $ f $ làm bao trên. Đặt $ u_\alpha = v_\alpha + \lambda_\alpha $, trong đó $ \lambda_\alpha \in \mathbf{R} $, và trong đó $ v_\alpha $ là một dạng tuyến tính liên tục trong $ E $. Ta có $ \lambda_\alpha = u_\alpha(0) \leq f(0) = 0 $. Mặt khác, nếu $ x \in X $, thì với mọi $ \mu > 0 $,
$$
\mu^{-1} \lambda_\alpha + v_\alpha(x) = \mu^{-1} (\lambda_\alpha + v_\alpha(\mu x)) = \mu^{-1} u_\alpha(\mu x) \leq \mu^{-1} f(\mu x) = f(x)
$$
do đó $ u_\alpha \leq v_\alpha \leq f $ trên $ X $ suy ra $ f $ là bao trên của các $ v_\alpha $.

#### Nhận xét 3 {#evt-ii-s5-n4-rem-3 .statement}

Hạn chế lên $ X $ của một hàm afin liên tục trong $ E $ là một hàm afin trên $ X $ (tức là vừa lõm vừa lồi II, p. 17); nhưng có thể có những hàm afin liên tục trong một tập lồi compact $ X \subset E $, mà không phải là các hạn chế lên $ X $ của các hàm afin liên tục *trong* $ E $ (II, p. 78, bài tập II, c)). Tuy nhiên :

#### Mệnh đề 6 {#evt-ii-s5-prop-6 .statement}

*Cho $ f $ là một hàm afin nửa liên tục trên của một tập lồi compact $ X $, thuộc không gian lồi địa phương Hausdorff $ E $. Cho $ L $ là tập hợp các hạn chế lên $ X $ của các hàm afin liên tục trong $ E $; khi đó tập hợp $ L' $ gồm các $ h \in L $ sao cho $ h(x) > f(x) $ với mọi $ x \in X $, là một tập có hướng giảm và bao dưới của nó bằng $ f $.*

Ta có thể giả sử rằng $ X $ là không rỗng. Cho $ u, v $ là hai phần tử của $ L $, sao cho $ u(x) > f(x) $ và $ v(x) > f(x) $ với mọi $ x \in X $, và cho $ b $ là một hằng là cận trên của $ u $ và $ v $. Cho $ U $ (tương ứng $ V $) là tập hợp lồi compact các điểm $ (x, t) $ của $ X \times \mathbf{R} $ sao cho $ u(x) \leq t \leq b $ (tương ứng $ v(x) \leq t \leq b $), và cho $ F $ là tập các $ (x, t) \in X \times \mathbf{R} $ sao cho $ t \leq f(x) $; $ F $ là lồi và đóng trong $ X \times \mathbf{R} $. Bao lồi $ K $ của $ U \cup V $ không gặp $ F $, vì $ U \cup V $ được chứa trong tập các $ (x, t) \in X \times \mathbf{R} $ sao cho $ f(x) < t $, một tập lồi và không gặp $ F $. Vì $ K $ là compact (II, p. 14, mệnh đề 15), ta có thể tách $ F $ một cách chặt khỏi $ K $ bởi một siêu phẳng đóng $ H $ trong $ E \times \mathbf{R} $. Với mọi $ x \in X $, siêu phẳng $ H $ tách $ (x, f(x)) $ một cách chặt khỏi $ (x, b) $, *và do đó* gặp đường thẳng $ \{ x \} \times \mathbf{R} $ tại một điểm duy nhất $ w(x) $; vì vậy $ H $ là đồ thị của một hàm afin liên tục mà phép hạn chế $ w $ lên $ X $ là một phần tử của $ L $, tức là một cận dưới của $ u $ và $ v $ và thỏa mãn bất đẳng thức $ w(x) > f(x) $ với mọi $ x \in X $. Điều này chứng tỏ rằng tập $ L' $ là giảm có hướng. Mệnh đề 5 của II, p. 39, áp dụng cho $ -f $ cho thấy rằng $ f $ là bao dưới của $ L' $.

#### Hệ quả {#evt-ii-s5-n4-cor-1 .statement}

*Cho $ f $ là một hàm afin liên tục trong $ X $; khi đó tồn tại một dãy $ (h_n) $ gồm các phần tử của $ L $ hội tụ đều đến $ f $ trong $ X $. \*

Vì, mệnh đề 6 và định lý của Dini (GT, X, § 4.1, th. 1) cho thấy rằng với mọi $ n $ đều tồn tại $ h_n \in L $ sao cho $ f \leq h_n \leq f + 1/n $.

### Bài tập {#evt-ii-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
