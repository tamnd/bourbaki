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
statements: 21
exercises: 30
content_sha256: 6d70e080c4dc42bf345b66d3fa96b50b880753f6a780fc705bbcee6fad6be3d0
translated_from: content/en/evt/II/05_s5_separation_of_convex_sets.md
source_content_sha256: ef3cb50958a2132d791f050aa2367a3e2957bbc2da2ad66deb90faecf196f50d
translation_model: gpt-5.4
translation_run: translate-vi-4ed2a9e8
glossary_version: 34
glossary_terms_sha256: c061be872cc771f37439d66febae732db42590f756b40941d63cc3ac40fa527e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. SỰ PHÂN CÁCH CỦA CÁC TẬP HỢP LỒI

### 1. Định lý Hahn-Banach (dạng hình học)

#### Định lý 1 (Hahn-Banach) {#evt-ii-s5-thm-1 .statement}

— *Cho A là một tập hợp lồi mở không rỗng của không gian vectơ tôpô E và cho M là một đa tạp tuyến tính không rỗng không giao với A. Khi đó tồn tại một siêu phẳng đóng H chứa M và không giao với A.*

Bằng phép tịnh tiến, bài toán có thể quy về trường hợp $ 0 \in A $, sao cho $ A $ là hấp thụ. Gọi $ p $ là *phiếm hàm Minkowski* của $ A $ (II, p. 20), sao cho $ A $ là tập hợp các điểm $ x \in E $ thỏa mãn $ p(x) < 1 $. Mặt khác, gọi $ V $ là không gian con vectơ của $ E $ sinh bởi $ M $; do đó $ M $ là một siêu phẳng trong $ V $ không chứa $ 0 $, và vì thế tồn tại một dạng tuyến tính duy nhất $ f $ trên $ V $ sao cho $ M $ là tập hợp các điểm $ y \in V $ mà với chúng $ f(y) = 1 $. Giả thiết $ M \cap A = \varnothing $ do đó kéo theo rằng với mọi $ y \in V $ mà $ f(y) = 1 $, ta có $ p(y) \geqslant 1 $; vì $ f $ và $ p $ là dương thuần nhất nên ta có $ f(y) \leqslant p(y) $ với mọi $ y \in V $ sao cho $ f(y) > 0 $; cuối cùng, vì $ p(y) \geqslant 0 $ với mọi $ y \in V $, ta thấy rằng $ f(y) \leqslant p(y) $ với *mọi* $ y \in V $. Theo dạng giải tích của định lý Hahn-Banach (II, p. 22, định lý 1), tồn tại một dạng tuyến tính $ h $ trên $ E $ kéo dài $ f $ và sao cho, với mọi $ x \in E $, $ h(x) \leqslant p(x) $. Gọi $ H $ là siêu phẳng trong $ E $ có phương trình $ h(x) = 1 $. Rõ ràng $ H \cap V = M $ và $ H \cap A = \varnothing $. Mặt khác, phần bù của $ H $ trong $ E $ chứa tập mở khác rỗng $ A $, do đó $ H $ là *đóng* trong $ E $ (I, p. 11, hệ quả).

C.Q.F.D.

#### Nhận xét {#evt-ii-s5-n1-rem-1 .statement}

— 1) Khi $ 0 \in M $, định lý 1 có thể được phát biểu như sau : tồn tại một *dạng tuyến tính liên tục trên E*, *sao cho* $ g(x) = 0 $ *trong* $ M $ *và* $ g(x) > 0 $ *trong* $ A $ (II, p. 8, mệnh đề 4).

2) Nếu áp dụng định lý 1 cho trường hợp $ E $ mang tôpô lồi địa phương mịn nhất (II, p. 25, *Ví dụ* 2), và nếu, để đơn giản, ta giả sử rằng $ 0 \in A $, thì ta thu được kết quả sau đây (bề ngoài không dính dáng đến tôpô): nếu $ A $ là một tập hợp lồi *hấp thụ* trong không gian vectơ thực $ E $ và nếu $ M $ là một đa tạp tuyến tính không rỗng không giao với $ A $, thì tồn tại một siêu phẳng $ H $ chứa $ M $ và sao cho $ A $ nằm về một phía của $ H $. Kết quả này không đúng với mọi tập hợp lồi $ A $ (II, p. 65, bài tập 5).

### 2. Sự tách các tập hợp lồi trong một không gian vectơ tôpô

#### Định nghĩa 1 {#evt-ii-s5-def-1 .statement}

— *Hai tập hợp không rỗng* $ A, B $ *của một không gian vectơ tôpô thực* $ E $ *được gọi là được phân cách bởi một siêu phẳng đóng* $ H $ *nếu* $ A $ *được chứa trong một trong các nửa không gian đóng được xác định bởi* $ H $ *và* $ B $ *được chứa trong nửa không gian đóng kia*.

#### Định nghĩa 2 {#evt-ii-s5-def-2 .statement}

— *Hai tập hợp không rỗng* $ A, B $ *của một không gian vectơ tôpô thực được gọi là được phân cách ngặt bởi siêu phẳng đóng* $ H $ *nếu* $ A $ *được chứa trong một trong các nửa không gian mở được xác định bởi* $ H $, *và* $ B $ *được chứa trong nửa không gian mở kia*.

#### Mệnh đề 1 {#evt-ii-s5-prop-1 .statement}

— *Cho* $ A $ *là một tập hợp lồi mở khác rỗng và cho* $ B $ *là một tập hợp lồi khác rỗng trong một không gian vectơ tôpô thực* $ E $; *nếu* $ A $ *không giao với* $ B $ *thì tồn tại một siêu phẳng đóng tách* $ A $ *khỏi* $ B $.

Vì tập hợp $ C = A - B $ là mở, lồi (II, p. 9, prop. 7) và không rỗng, lại có $ 0 \notin C $. Theo định lý 1 của II, p. 36, tồn tại một dạng tuyến tính liên tục $ f \neq 0 $ trên $ E $ sao cho $ f(z) > 0 $ trong $ C $. Khi đó, với mọi $ x \in A $, và $ y \in B $, ta có $ f(x) > f(y) $. Đặt $ \alpha = \inf_{x \in A} f(x) $; $ \alpha $ là hữu hạn và ta có $ f(x) \geq \alpha $ với mọi $ x \in A $ và $ f(y) \leq \alpha $ với mọi $ y \in B $; siêu phẳng đóng $ H $ có phương trình $ f(z) = \alpha $ tách $ A $ khỏi $ B $.

#### Nhận xét {#evt-ii-s5-n2-rem-1 .statement}

— 1) Siêu phẳng $ H $ không cắt $ A $ (II, p. 15, prop. 1; nếu $ A $ và $ B $ là hai tập hợp lồi không rỗng *mở* không cắt nhau thì tồn tại một siêu phẳng đóng tách $ A $ *nghiêm ngặt* khỏi $ B $.
2) Tuy nhiên, khi $ B $ không mở, không nhất thiết tồn tại một siêu phẳng đóng tách $ A $ nghiêm ngặt khỏi $ B $, ngay cả khi $ E $ có số chiều hữu hạn, và ngay cả khi $ \overline{A} $ không cắt $ \overline{B} $ (II, p. 78, exerc. 12).

#### Định nghĩa 3 {#evt-ii-s5-def-3 .statement}

— *Đối với một tập con* $ A $ *của một không gian vectơ* $ E $, *một siêu phẳng* $ H $ *được gọi là một siêu phẳng tựa của* $ A $, *nếu* $ H $ *chứa ít nhất một điểm của* $ A $ *và mọi điểm của* $ A $ *đều nằm về cùng một phía của* $ H $.

Cho $ f $ là một dạng tuyến tính trên $ E $ không đồng nhất bằng không; nói rằng siêu phẳng có phương trình $ f(x) = \alpha $ là một siêu phẳng tựa của $ A $ có nghĩa là $ \alpha $ hoặc là phần tử nhỏ nhất, hoặc là phần tử lớn nhất của tập hợp $ f(A) \subset \mathbf{R} $. Nói cách khác, tồn tại một siêu phẳng tựa của $ A $ song song với siêu phẳng có phương trình $ f(x) = 0 $ nếu, và chỉ nếu, một trong các cận của tập hợp $ f(A) $ là hữu hạn và thuộc $ f(A) $.

#### Mệnh đề 2 {#evt-ii-s5-prop-2 .statement}

— *Cho* $ A $ *là một tập con compắc không rỗng của một không gian vectơ tôpô* $ E $. *Với mọi siêu phẳng đóng* $ H $ *trong* $ E $, *tồn tại một siêu phẳng tựa của* $ A $ *song song với* $ H $.

Thật vậy, nếu $ f(x) = \gamma $ là một phương trình của $ H $, trong đó $ f $ là một dạng tuyến tính liên tục trên $ E $, thì hạn chế của $ f $ trên $ A $ là liên tục, do đó bị chặn và đạt các cận của nó trên $ A $ (GT, IV, § 6.1, đl. 1).

Điều này chứng tỏ rằng tồn tại một hoặc hai siêu phẳng tựa của $ A $ song song với $ H $; trường hợp thứ nhất chỉ có thể xảy ra khi $ A $ được chứa hoàn toàn trong một siêu phẳng song song với $ H $.

#### Mệnh đề 3 {#evt-ii-s5-prop-3 .statement}

— *Trong một không gian vectơ tôpô* $ E $, *cho* $ A $ *là một tập lồi đóng có* phần trong không rỗng. Khi đó mọi siêu phẳng tựa của $ A $ đều đóng và mọi điểm biên của $ A $ đều thuộc ít nhất một siêu phẳng tựa của $ A $.

Mọi siêu phẳng tựa của $ A $ đều đóng, vì mọi điểm của $ A $ đều ở cùng một phía của siêu phẳng (II, p. 15, mệnh đề 17). Mặt khác, nếu $ x_0 $ là một điểm biên của $ A $, thì $ x_0 $ không thuộc tập hợp lồi mở không rỗng $ \overset{\circ}{A} $; theo định lý 1 của II, p. 36, tồn tại một siêu phẳng $ H $ chứa $ x_0 $ và không giao với $ \overset{\circ}{A} $. Vì $ A $ là bao đóng của $ \overset{\circ}{A} $ (II, p. 14, hệ quả 1 của mệnh đề 16), suy ra từ mệnh đề 17 của II, p. 15 rằng $ H $ là một siêu phẳng tựa của $ A $.

### 3. Sự tách các tập hợp lồi trong một không gian lồi địa phương

#### Mệnh đề 4 {#evt-ii-s5-prop-4 .statement}

— Cho $ A $ là một tập hợp lồi đóng không rỗng trong một không gian lồi địa phương $ E $ và cho $ K $ là một tập hợp lồi compact không rỗng trong $ E $, không giao với $ A $. Khi đó tồn tại một siêu phẳng đóng $ H $ phân tách nghiêm ngặt $ A $ với $ K $.

Vì tồn tại một lân cận lồi mở $ V $ của 0 trong $ E $ sao cho $ A + V $ và $ K + V $ không giao nhau (GT, II, § 4.3, mệnh đề 4). Vì $ A + V $ và $ K + V $ là lồi và mở trong $ E $, mệnh đề 1 của II, p. 37 cho thấy rằng tồn tại một siêu phẳng đóng $ H $ phân tách nghiêm ngặt $ A + V $ với $ K + V $, và $ a $ fortiori $ A $ với $ K $.

#### Nhận xét {#evt-ii-s5-n3-rem-1 .statement}

— Trong một không gian lồi địa phương Hausdorff $ E $, cho $ A $ và $ B $ là hai tập hợp lồi đóng không rỗng và rời nhau; nếu $ E $ hữu hạn chiều thì tồn tại một siêu phẳng đóng tách $ A $ khỏi B (II, p. 78, exerc. 13); nhưng kết luận này không nhất thiết còn đúng khi $ E $ có chiều vô hạn (II, p. 78, exerc. 10 and 11).

#### Hệ quả 1 {#evt-ii-s5-prop-4-cor-1 .statement}

— Trong một không gian lồi địa phương, mọi tập hợp lồi đóng $ A $ đều là giao của các nửa không gian đóng chứa nó.

Thật vậy, với mọi điểm $ x \notin A $, tồn tại một siêu phẳng đóng tách chặt $ x $ khỏi $ A $ (dùng mệnh đề 4).

#### Hệ quả 2 {#evt-ii-s5-prop-4-cor-2 .statement}

— Trong một không gian lồi địa phương Hausdorff, mọi tập hợp lồi compac $ A $ đều là giao của các nửa không gian đóng chứa nó và được xác định bởi các siêu phẳng tựa của $ A $.

Thật vậy, giả sử $ x_0 \notin A $; $ \{ x_0 \} $ là đóng, do đó tồn tại một siêu phẳng đóng $ H $ tách $ x_0 $ một cách chặt khỏi $ A $ (mệnh đề 4); gọi $ f(x) = \alpha $ là một phương trình của $ H $ ($ f $ là một dạng tuyến tính liên tục) và giả sử rằng $ f(x) > \alpha $ với mọi $ x \in A $. Nếu đặt $ \gamma = \inf_{x \in A} f(x) $, thì nửa không gian được xác định bởi $ f(x) \geq \gamma $ chứa $ A $, được xác định bởi siêu phẳng tựa có phương trình $ f(x) = \gamma $, và không chứa $ x_0 $; do đó có hệ quả.

Có thể xảy ra rằng một tập hợp lồi đóng không compact và không có điểm trong, trong một không gian lồi địa phương, không có siêu phẳng tựa đóng nào (II, p. 86, bài tập 18 : xem thêm cả V, p. 71, bài tập 11).

#### Hệ quả 3 {#evt-ii-s5-prop-4-cor-3 .statement}

— Trong một không gian lồi địa phương, bao đóng của mỗi đa tạp tuyến tính $ M $ là giao của các siêu phẳng đóng chứa $ M $.

Với mọi $ x \notin \overline{M} $, gọi $ H $ là một siêu phẳng đóng tách biệt chặt $ x $ khỏi $ \overline{M} $;

khi đó $ \overline{M} $ song song với $ H $; siêu phẳng đóng $ H_1 $, chứa $ \overline{M} $ và song song với $ H $ không chứa $ x $. Hệ quả suy ra.

#### Hệ quả 4 {#evt-ii-s5-prop-4-cor-4 .statement}

*Cho $ C $ là một tập hợp lồi đóng trong một không gian lồi địa phương $ E $. Một tập con $ A $ của $ E $ được chứa trong $ C $ khi, và chỉ khi, với mọi hàm afin liên tục nhận giá trị thực $ u $ trên $ E $ sao cho $ u(x) \geqslant 0 $ với mọi $ x $ trong $ C $, ta có $ u(y) \geqslant 0 $ với mọi $ y $ trong $ A $.*

Điều kiện đó hiển nhiên là cần thiết. Ngược lại, ta sẽ chỉ ra rằng nó là đủ; nếu một điểm $ x \in A $ không được chứa trong $ C $, thì tồn tại một siêu phẳng đóng có phương trình $ f(z) = \alpha $ tách $ x $ một cách nghiêm ngặt khỏi $ C $; chẳng hạn nếu ta giả sử rằng $ f(x) < \alpha $, thì hàm afin liên tục $ u = f - \alpha $ mâu thuẫn với các giả thiết.

#### Hệ quả 5 {#evt-ii-s5-prop-4-cor-5 .statement}

*Trong một không gian lồi địa phương $ E $, bao đóng của mỗi nón lồi $ C $ có đỉnh $ 0 $ là giao của các nửa không gian đóng chứa $ C $ được xác định bởi các siêu phẳng đóng đi qua $ 0 $.*

Vì $ \overline{C} $ là một nón lồi có đỉnh $ 0 $ (II, p. 13, mệnh đề 14). Với $ x \notin \overline{C} $, tồn tại một siêu phẳng đóng $ H $ tách $ x $ một cách nghiêm ngặt khỏi $ \overline{C} $(mệnh đề 4). Bây giờ chỉ còn cần áp dụng bổ đề sau :

#### Bổ đề 1 {#evt-ii-s5-lem-1 .statement}

— *Nếu một nón $ A $, có đỉnh $ 0 $, được chứa trong một nửa-không gian mở được xác định bởi một siêu phẳng $ H $, thì nó được chứa trong một nửa-không gian đóng được xác định bởi một siêu phẳng $ H_0 $, song song với $ H $ và đi qua $ 0 $.*

Gọi $ f(z) = \alpha $ với $ \alpha < 0 $ là một phương trình của $ H $, sao cho $ f(z) = 0 $ là phương trình của $ H_0 $. Nếu tồn tại $ z \in A $ sao cho $ f(z) < 0 $, thì sẽ tồn tại $ \lambda > 0 $ sao cho $ f(\lambda z) = \alpha $, và vì $ \lambda z \in A $, điều này sẽ mâu thuẫn với giả thiết.

### 4. Xấp xỉ các hàm lồi

#### Mệnh đề 5 {#evt-ii-s5-prop-5 .statement}

*Cho $ X $ là một tập hợp lồi đóng trong một không gian lồi địa phương $ E $. Khi đó mọi hàm lồi nửa liên tục dưới $ f $ xác định trên $ X $ đều là bao trên của một họ các hàm là những hạn chế trên $ X $ của các hàm affine tuyến tính liên tục trên $ E $.*

Thật vậy, tập $ A \subset E \times \mathbf{R} $ gồm các điểm $ (x, t) $ sao cho $ x \in X $ và $ t \geqslant f(x) $ là lồi (II, p. 17, mệnh đề 19) và đóng, vì hàm $ (x, t) \mapsto f(x) - t $ là nửa liên tục dưới. Bây giờ lấy $ x $ là một điểm bất kỳ của $ X $ và lấy $ a \in \mathbf{R} $ sao cho $ a < f(x) $. Theo hệ quả 1 của II, p. 38, tồn tại một siêu phẳng đóng $ H $ trong $ E \times \mathbf{R} $, chứa $ (x, a) $ và không giao với $ A $. Mọi dạng tuyến tính liên tục trên $ E \times \mathbf{R} $ đều có dạng

$$
(z, t) \to u(z) + \lambda t ,
$$

trong đó $ \lambda \in \mathbf{R} $ và $ u $ là một dạng tuyến tính liên tục trên $ E $, suy ra $ H $ có một phương trình dạng $ u(z) + \lambda t = \alpha $, và vì $ H $ chứa $ (x, a) $ nên ta có $ \alpha = u(x) + \lambda a $. Bây giờ điểm $ (x, f(x)) \in A $ không thuộc $ H $ và do đó $ \lambda \neq 0 $. Nếu cần, chia cho $ -\lambda $, ta có thể viết phương trình của $ H $ dưới dạng $ t - a = u(z - x) $. Vì $ f(x) - a > 0 $, do đó ta có $ f(z) > u(z - x) + a $ với mọi $ z \in X $ và điều này chứng minh mệnh đề.

#### Nhận xét {#evt-ii-s5-n4-rem-1 .statement}

— 1) Suy ra từ mệnh đề 5 rằng $ f $ là bao trên của một họ *tăng* có hướng các hàm số là những hạn chế lên $ X $ của các hàm số liên tục và lồi trong $ E $.

2) Giả sử thêm rằng $ X $ là một nón lồi đóng có đỉnh 0 và $ f $ là *thuần nhất dương*. Khi đó $ f $ là bao trên của một họ hàm là các hạn chế trên $ X $ của các *dạng tuyến tính liên tục* trong $ E $. Thật vậy, lấy $ (u_\alpha) $ là một họ các hàm afin liên tục trong $ E $ mà các hạn chế của chúng trên $ X $ có $ f $ làm bao trên. Đặt $ u_\alpha = v_\alpha + \lambda_\alpha $, trong đó $ \lambda_\alpha \in \mathbf{R} $, và trong đó $ v_\alpha $ là một dạng tuyến tính liên tục trong $ E $. Ta có $ \lambda_\alpha = u_\alpha(0) \leq f(0) = 0 $. Mặt khác, nếu $ x \in X $, thì với mọi $ \mu > 0 $,
$$
\mu^{-1} \lambda_\alpha + v_\alpha(x) = \mu^{-1} (\lambda_\alpha + v_\alpha(\mu x)) = \mu^{-1} u_\alpha(\mu x) \leq \mu^{-1} f(\mu x) = f(x)
$$
do đó $ u_\alpha \leq v_\alpha \leq f $ trên $ X $ và vì thế $ f $ là bao trên của các $ v_\alpha $.

3) Hạn chế lên $ X $ của một hàm afin liên tục trong $ E $ là một hàm afin trong $ X $ (tức là vừa lõm vừa lồi II, p. 17); nhưng có thể xảy ra rằng tồn tại các hàm afin liên tục trong một tập lồi compắc $ X \subset E $, mà không phải là các hạn chế lên $ X $ của những hàm afin liên tục *trong* $ E $ (II, p. 78, bài tập II, c)). Tuy nhiên:

#### Mệnh đề 6 {#evt-ii-s5-prop-6 .statement}

*Cho $ f $ là một hàm afin nửa liên tục trên trên một tập hợp lồi compắc $ X $, của không gian lồi địa phương Hausdorff $ E $. Cho $ L $ là tập hợp các hạn chế trên $ X $ của các hàm afin liên tục trên $ E $; khi đó tập hợp $ L' $ của các $ h \in L $ sao cho $ h(x) > f(x) $ với mọi $ x \in X $ là giảm có hướng, và bao dưới của nó bằng $ f $.*

Ta có thể giả sử rằng $ X $ không rỗng. Cho $ u, v $ là hai phần tử của $ L $, sao cho $ u(x) > f(x) $ và $ v(x) > f(x) $ với mọi $ x \in X $, và cho $ b $ là một hằng là cận trên của $ u $ và $ v $. Gọi $ U $ (tương ứng $ V $) là tập hợp lồi compắc các điểm $ (x, t) $ của $ X \times \mathbf{R} $ sao cho $ u(x) \leq t \leq b $ (tương ứng $ v(x) \leq t \leq b $), và gọi $ F $ là tập hợp các $ (x, t) \in X \times \mathbf{R} $ sao cho $ t \leq f(x) $; $ F $ lồi và đóng trong $ X \times \mathbf{R} $. Bao lồi $ K $ của $ U \cup V $ không cắt $ F $, vì $ U \cup V $ được chứa trong tập hợp các $ (x, t) \in X \times \mathbf{R} $ sao cho $ f(x) < t $, là một tập hợp lồi và không cắt $ F $. Vì $ K $ compắc (II, p. 14, mệnh đề 15), ta có thể tách chặt $ F $ khỏi $ K $ bằng một siêu phẳng đóng $ H $ trong $ E \times \mathbf{R} $. Với mọi $ x \in X $, siêu phẳng $ H $ tách chặt $ (x, f(x)) $ khỏi $ (x, b) $, *và do đó* cắt đường thẳng $ \{ x \} \times \mathbf{R} $ tại đúng một điểm $ w(x) $; như vậy $ H $ là đồ thị của một hàm afin liên tục mà hạn chế $ w $ của nó trên $ X $ là một phần tử của $ L $, là một cận dưới của $ u $ và $ v $ và thỏa mãn bất đẳng thức $ w(x) > f(x) $ với mọi $ x \in X $. Điều này chứng minh rằng tập hợp $ L' $ là có hướng giảm. Mệnh đề 5 của II, p. 39, áp dụng cho $ -f $ cho thấy rằng $ f $ là bao dưới của $ L' $.

#### Hệ quả {#evt-ii-s5-n4-cor-1 .statement}

*Cho $ f $ là một hàm afin liên tục trên $ X $; khi đó tồn tại một dãy $ (h_n) $ các phần tử của $ L $ hội tụ đều đến $ f $ trên $ X $.*

Thật vậy, mệnh đề 6 và định lý Dini (GT, X, § 4.1, định lý 1) cho thấy rằng với mọi $ n $ tồn tại $ h_n \in L $ sao cho $ f \leq h_n \leq f + 1/n $.

### Bài tập {#evt-ii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
