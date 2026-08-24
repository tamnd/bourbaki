---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 7
section_title: Extremal points and extremal generators
lang: vi
source: evt-i-v
book_pages: TVS II.54-TVS II.60, TVS II.87-TVS II.95
pdf_pages: 0091-0097, 0124-0132
extraction: ocr
subsections:
    - "no": 1
      title: Extremal points of compact convex sets
      page: 54
      pdf_page: 91
    - "no": 2
      title: Extremal generators of convex cones
      page: 57
      pdf_page: 94
    - "no": 3
      title: Convex cones with compact sole
      page: 59
      pdf_page: 96
statements: 12
exercises: 41
content_sha256: bf02ab99a8f50f17d92ecd5ee1c3645ebec2e7a6ea3983cb651bfb10f5597a0a
translated_from: content/en/evt/II/07_s7_extremal_points_and_extremal_generators.md
source_content_sha256: debba20c88331d55b5d9fde0b294021f9389cc1025db7ffbda646200c2d8c538
translation_model: gpt-5.4
translation_run: translate-vi-4bb1b7cf
glossary_version: 34
glossary_terms_sha256: 27fb439d820fcc96e1fcb953f29badd0182f4c9e2bd3fa9b9a61fcc3fa1ac8ca
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. CÁC ĐIỂM CỰC BIÊN VÀ CÁC PHẦN TỬ SINH CỰC BIÊN

### 1. Các điểm cực biên của các tập lồi compắc

Định nghĩa 1. — Cho $ A $ là một tập lồi trong một không gian afin $ E $. Khi đó ta nói rằng một điểm $ x \in A $ là một điểm cực biên của $ A $ nếu không tồn tại một đoạn thẳng mở nào được chứa trong $ A $ và chứa $ x $.

Nói cách khác, các hệ thức $ x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z $ và $ 0 \leq \lambda \leq 1 $ suy ra $ \lambda = 0 $ hoặc $ \lambda = 1 $ (do đó $ x = y $ hoặc $ x = z $). Điều này suy ra rằng $ x $ không thể là trọng tâm của một tập hợp gồm $ n $ điểm $ x_i $ của $ A $ mang các khối lượng dương trừ khi $ x $ là một trong các $ x_i $; bởi vì đó chính là định nghĩa khi $ n = 2 $; với $ n $ tùy ý, lập luận bằng quy nạp theo $ n $, vì $ x $ là trọng tâm của $ x_1 $ và của trọng tâm $ y_1 $ của các $ x_i $ với $ 2 \leq i \leq n $, do đó $ x $ trùng với $ x_1 $ hoặc $ y_1 $, và trong trường hợp thứ hai chỉ cần áp dụng giả thiết quy nạp.

Nói rằng $ x $ là một điểm cực biên của $ A $ cũng có nghĩa là $ A - \{x\} $ là lồi.

#### Ví dụ {#evt-ii-s7-n1-exa-1 .statement}

— 1) Trong không gian $ \mathbf{R}^n $, mọi điểm của mặt cầu $ S_{n-1} $ đều là những điểm cực biên của quả cầu đóng $ B_n $. Thật vậy, nếu $ \sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1 $ và $ 0 < \lambda < 1 $, thì quan hệ
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
chỉ có thể xảy ra nếu
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1.
$$
Nhưng điều này suy ra $ \sum_i (y_i - z_i)^2 = 0 $, do đó $ y_i = z_i $ với mọi $ i $, điều này chứng minh mệnh đề của chúng ta.

2) Trong không gian chuẩn $ \mathcal{B}(\mathbf{N}) $ của các dãy số thực bị chặn (I, p. 4), các điểm cực biên của quả cầu đơn vị là các điểm $ x = (\xi_n) $ sao cho $ |\xi_n| = 1 $ với mọi $ n $. Thật vậy, giả sử rằng ta có $ |\xi_n| \leq 1 $ với mọi $ n $ và $ |\xi_p| < 1 $ đối với một chỉ số $ p $. Khi đó ta có thể viết
$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$
trong đó $ y $ (tương ứng $ z $) là điểm mà mọi tọa độ đều bằng tọa độ của $ x $ có cùng chỉ số, trừ ở chỉ số $ p $ thì tọa độ bằng 1 (tương ứng $ -1 $). Điều này cho thấy rằng $ x $ không cực biên, vì ta có $ \|y\| \leq 1 $ và $ \|z\| \leq 1 $. Ngược lại, nếu $ |\xi_n| = 1 $ với mọi $ n $, thì $ x $ là cực biên, vì quan hệ $ \xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n $ với $ |\eta_n| \leq 1,\ |\zeta_n| \leq 1 $ và $ 0 < \lambda < 1 $ kéo theo $ \xi_n = \eta_n = \zeta_n $.

3) Cho $ u : E \to E' $ là một ánh xạ afin của một không gian afin $ E $ vào một không gian afin $ E' $; cho $ C \subset E,\ C' \subset E' $ là hai tập lồi sao cho $ u(C) \subset C' $. Nếu $ x' $ là một điểm cực biên của $ C' $ và $ x $ là một điểm cực biên của $ u^{-1}(x') \cap C $, thì $ x $ là một điểm cực biên của $ C $, như suy ra từ Định nghĩa 1.

Mệnh đề 1. — Cho $ B $ là tập hợp các điểm cực biên của $ A $, một tập hợp lồi compắc không rỗng trong một không gian lồi địa phương Hausdorff $ E $, và cho $ f $ là một hàm lồi xác định trên $ A $ và nửa liên tục trên. Khi đó $ f $ đạt cận trên của nó trên $ A $ tại một điểm (ít nhất) của $ B $.

Dùng $ \mathcal{F} $ để ký hiệu họ các tập con X của A *không rỗng, đóng, và sao cho mọi đoạn mở được chứa trong A và giao với X thì tất yếu nằm trong X*. Nó có các tính chất sau;
(i) A thuộc $ \mathcal{F} $.
(ii) Một điểm $ a \in A $ là sao cho $ \{a\} \in \mathcal{F} $ khi, và chỉ khi, $ a $ là một điểm cực biên của A.
(iii) Mọi giao không rỗng X của một họ $ (X_\alpha) $ các tập hợp của $ \mathcal{F} $ cũng thuộc $ \mathcal{F} $.

Các tính chất (i), (ii) và (iii) theo ngay lập tức từ các định nghĩa.

(iv) Cho $ X \in \mathcal{F} $, và cho $ h $ là một hàm lồi và nửa liên tục trên trong A; khi đó tập hợp Y các điểm của X tại đó hạn chế $ h|X $ đạt cận trên của nó trong X là sao cho Y thuộc $ \mathcal{F} $.

Vì $ h|X $ là nửa liên tục trên trên X nên đạt cận trên $ \alpha $ của nó trên X tại ít nhất một điểm của X (GT, IV, § 6.2, định lý 3); do đó Y không rỗng, và cũng đóng (GT, IV, § 6.2, mệnh đề 1). Mặt khác, cho $ x, y $ là hai điểm phân biệt của A và cho $ z = \lambda x + (1 - \lambda) y $ là một điểm của Y sao cho $ 0 < \lambda < 1 $; vì $ Y \subset X $ và $ X \in \mathcal{F} $, ta có $ x \in X $ và $ y \in X $; mặt khác, vì $ h $ là lồi, ta có

$$
h(z) \leq \lambda h(x) + (1 - \lambda) h(y)
$$

nhưng vì $ h(x) \leq \alpha, h(y) \leq \alpha $ và $ h(z) = \alpha $, tất yếu $ h(x) = h(y) = \alpha $, nghĩa là $ x \in Y $ và $ y \in Y $. Vậy $ Y \in \mathcal{F} $.

Sau khi đã thiết lập các tính chất này, đặt M là tập hợp các $ x \in A $ tại đó $ f $ đạt cận trên của nó trong A; theo (iv), $ M \in \mathcal{F} $. Mặt khác, từ (iii) và việc các tập hợp của $ \mathcal{F} $ là những tập con đóng của tập compact A, suy ra $ \mathcal{F} $ là *quy nạp* đối với quan hệ thứ tự $ \supset $. Theo định lý 2 của S, III, § 2.4, M chứa một tập con N là một phần tử cực tiểu của $ \mathcal{F} $. Ta sẽ chỉ ra rằng N chỉ gồm một điểm và điều này sẽ hoàn tất chứng minh của mệnh đề. Vì E là một không gian lồi địa phương Hausdorff, chỉ cần chỉ ra rằng mọi dạng tuyến tính liên tục $ u $ trên E đều hằng trên N (II, p. 38, hệ quả 1). Bây giờ từ (iv) suy ra rằng tập hợp $ N' $ gồm các $ x \in N $ tại đó $ u|N $ đạt cận trên của nó trong N là sao cho $ N' $ thuộc $ \mathcal{F} $; vì N là cực tiểu trong $ \mathcal{F} $ nên tất yếu ta có $ N' = N $.

#### Hệ quả {#evt-ii-s7-n1-cor-1 .statement}

*Cho A là một tập compact lồi trong một không gian lồi địa phương Hausdorff E. Khi đó mọi siêu phẳng tựa đóng H của A đều chứa ít nhất một điểm cực biên của A.*

Thật vậy, nếu $ f(x) = \alpha $ là một phương trình của H và nếu $ f(x) \leq \alpha $ trong A, thì chỉ cần áp dụng mệnh đề 1 cho $ f $.

#### Định lý 1 (Krein-Milman) {#evt-ii-s7-thm-1 .statement}

— *Trong một không gian lồi địa phương Hausdorff E, mọi tập lồi compắc A là bao lồi đóng của tập hợp các điểm cực biên của nó.*

Thật vậy, gọi C là bao lồi đóng của tập hợp các điểm cực biên của A; rõ ràng $ C \subset A $. Để thấy rằng $ A \subset C $, chỉ cần chứng minh rằng, nếu $ u $ là một hàm afin tuyến tính, liên tục trên E và nếu $ u(x) \geq 0 $ trong C thì cũng có $ u(x) \geq 0 $ trong A (II, p. 39, hệ quả 4); nhưng điều này suy ra từ mệnh đề 1 áp dụng cho $ -u $.

#### Mệnh đề 2 {#evt-ii-s7-prop-2 .statement}

*Cho x là một điểm cực biên của một tập lồi compắc A trong một không gian* lồi địa phương Hausdorff E. Khi đó với mọi lân cận mở V của x trong E, tồn tại một nửa-không gian mở F trong E sao cho $ x \in F \cap A \subset V \cap A $ (nói cách khác, các vết trên A của các nửa-không gian mở chứa x tạo thành một hệ lân cận cơ bản của x trong A).

Với mọi nửa-không-gian mở D của E chứa x, tập hợp $ A \cap \overline{D} $ là một lân cận compact của x trong A, và giao của tất cả các lân cận này chính xác là điểm x (mọi hai điểm phân biệt đều có thể được phân cách nghiêm ngặt bởi một siêu phẳng đóng (II, p. 38, mệnh đề 4). Theo mệnh đề 1 của GT, I, § 9.2, chỉ cần chứng minh rằng các tập hợp $ A \cap \overline{D} $ tạo thành một cơ sở lọc. Bây giờ nếu ta viết $ L_D = A \cap (E - D) $, tập hợp $ L_D $ là lồi, compact và được chứa trong tập hợp lồi $ A - \{x\} $; nếu $ D_1, D_2 $ là hai nửa-không-gian mở của E chứa x, thì bao lồi B của $ L_{D_1} \cup L_{D_2} $ do đó được chứa trong $ A - \{x\} $; nhưng B là một tập compact (II, p. 14, mệnh đề 15), vì thế tồn tại một siêu phẳng đóng H phân cách nghiêm ngặt x với B (II, p. 38, mệnh đề 4) và nếu nửa-không-gian mở được xác định bởi H và chứa x là D, thì ta có $ L_{D_1} \cup L_{D_2} \subset L_D $, do đó $ A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2}) $.

#### Hệ quả {#evt-ii-s7-n1-cor-2 .statement}

— Trong một không gian lồi địa phương Hausdorff, cho K là một tập con compact của một tập compact lồi A. Khi đó các điều kiện sau là tương đương.

a) A là bao lồi đóng của K.

b) K gặp mọi tập hợp là giao của A với một siêu phẳng tựa của nó.

c) K chứa tập hợp các điểm cực biên của A.

a) $ \Rightarrow $ b). Giả sử tồn tại một siêu phẳng tựa H của A có phương trình là $ f(x) = \alpha $, sao cho $ (H \cap A) \cap K = \varnothing $ và giả sử, chẳng hạn, rằng $ f(x) \geq \alpha $ trong A. Vì $ f(x) - \alpha > 0 $ với mọi $ x \in K $ theo giả thiết và vì K là compac nên ta có

$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$

và do đó K được chứa trong nửa không gian đóng $ f(x) \geq \beta $; vì thế điều tương tự cũng đúng với bao lồi đóng A của K, và điều này là vô lý.

b) $ \Rightarrow $ c). Giả sử rằng một điểm cực biên x của A không thuộc K; tồn tại một lân cận V của x trong E sao cho $ V \cap A \cap K = \varnothing $. Nhưng theo mệnh đề 2, ta có thể giả sử rằng V là một nửa không gian mở được xác định bởi một siêu phẳng H có phương trình $ f(z) = \alpha $. Chẳng hạn nếu $ f(x) > \alpha $, thì với mọi $ y \in K $, ta có $ f(y) \leq \alpha $, do đó K không gặp giao của A và siêu phẳng tựa $ f(z) = \gamma > \alpha $ song song với H (II, p. 37, mệnh đề 2); điều này là vô lý.

c) $ \Rightarrow $ a). Đây là một hệ quả hiển nhiên của định lý Krein-Milman.

#### Nhận xét {#evt-ii-s7-n1-rem-1 .statement}

— 1) Ngay cả khi không gian vectơ E là hữu hạn chiều thì tập hợp các điểm cực biên của một tập compact lồi cũng không nhất thiết đóng (II, p. 89, exerc. 11).

2) Nếu K là một tập compact trong một không gian lồi địa phương Hausdorff không đầy đủ, và A, bao lồi đóng của K, không compact, thì có thể có những điểm cực biên của A không thuộc K (II, p. 87, exerc. 2).

3) Trong một không gian Banach E vô hạn chiều, có thể xảy ra việc quả cầu đóng tâm 0 bán kính 1 không có điểm cực biên nào (II, p. 89, exerc. 14).

4) Nếu A là một tập compact lồi trong một không gian lồi địa phương Hausdorff, có thể xảy ra việc một điểm cực biên của A không thuộc bất kỳ siêu phẳng tựa nào của A (II, p. 78, exerc. 11). Chứng minh của định lý 1 (II, p. 56) cho thấy rằng trong mọi trường hợp A là bao lồi đóng của tập hợp các điểm cực biên của A thuộc một siêu phẳng tựa.

### 2. Các phần tử sinh cực biên của nón lồi

Cho C là một nón lồi có đỉnh 0 trong một không gian vectơ E; rõ ràng không một điểm nào khác của C ngoài đỉnh có thể là một điểm cực biên; đỉnh là một điểm cực biên của C khi và chỉ khi C là nhọn và thực sự.

Định nghĩa 2. — Cho C là một nón lồi có đỉnh 0 trong một không gian vectơ E. Ta nói rằng một nửa đường thẳng D ⊂ C xuất phát từ 0 là một phần tử sinh cực biên của C, nếu mọi đoạn thẳng mở chứa trong C, không chứa 0 và cắt D đều được chứa trong D.

Điều đó cũng tương đương với việc nói rằng với mọi x ∈ D sao cho x ≠ 0, nếu y ≠ 0, y' ≠ 0 là hai điểm của C sao cho x = y + y', thì nhất thiết phải có y ∈ D và y' ∈ D.

#### Nhận xét 1 {#evt-ii-s7-n2-rem-1 .statement}

— Cho C là một nón lồi nhọn thực sự trong E, và xét trên E cấu trúc thứ tự mà đối với nó C là tập hợp các phần tử ≥ 0 (II, p. 12, prop. 13); để một phần tử của E, chẳng hạn x > 0, thuộc một phần tử sinh cực biên của C, điều kiện cần và đủ là mọi phần tử y ≥ 0 bị chặn trên bởi x đều có dạng λx với 0 ≤ λ ≤ 1 : thật vậy, nói rằng y bị chặn trên bởi x có nghĩa là x = y + y' với y' ∈ C, do đó kết luận theo sau.

Mệnh đề 3. — Trong một không gian vectơ E, cho C là một nón lồi có đỉnh 0, và cho x₀ ≠ 0 là một điểm của C, và D là một nửa đường thẳng được chứa trong C, xuất phát từ 0 và chứa x₀. Cho H là một siêu phẳng chứa x₀ và không đi qua 0. Khi đó D là một phần tử sinh cực biên của C nếu và chỉ nếu x₀ là một điểm cực biên của H ∩ C.

Điều kiện này rõ ràng là cần thiết. Ngược lại, giả sử nó được thỏa mãn; giả sử rằng có một đường thẳng D' không chứa D, đi qua x₀ và sao cho D' ∩ C chứa một đoạn thẳng mở mà x₀ thuộc vào. Cho y ≠ 0 là một vectơ chỉ phương của D'; các giả thiết kéo theo rằng điểm (1 + λ)x₀ + μy thuộc C với |λ| và |μ| đủ nhỏ. Nhưng khi đó, trong mặt phẳng P được xác định bởi D và D' và mang tôpô chính tắc, x₀ là một điểm trong của P ∩ C, và do đó đường thẳng P ∩ H chứa một đoạn thẳng mở được chứa trong H ∩ C và mà x₀ thuộc vào. Điều này mâu thuẫn với giả thiết.

Định nghĩa 3. — Cho C là một tập hợp lồi trong một không gian vectơ tôpô Hausdorff E. Một tập hợp compact lồi khác rỗng A của C được gọi là một chỏm của C nếu phần bù C − A của A trong C là lồi.

Cho C là một nón lồi nhọn có đỉnh 0 trong E và cho A là một chỏm của C. Đặt B = C − A. Với mọi nửa đường thẳng đóng L ⊂ C xuất phát từ 0, các tập hợp L ∩ A và L ∩ B là những tập hợp lồi bù nhau trong L, có hợp là L, và sao cho L ∩ A là compact. Vì L ∩ A khác rỗng đối với ít nhất một nửa đường thẳng L, ta thấy rằng 0 ∈ A, do đó L ∩ A là một đoạn thẳng đóng có một đầu mút tại 0. Nếu A tồn tại thì C là thực sự.

#### Mệnh đề 4 {#evt-ii-s7-prop-4 .statement}

— Cho C là một nón lồi nhọn có đỉnh 0 trong E, một không gian lồi địa phương Hausdorff.

a) Cho A là một chỏm của C. Cho p là hạn chế lên C của phiếm hàm Minkowski của A (II, p. 20). Tập hợp các x ∈ C sao cho p(x) ≤ 1 là tập hợp A. Hàm p nửa liên tục dưới và có các tính chất sau :
(i) Với mọi x, y trong C, ta có p(x + y) = p(x) + p(y).
(ii) Với mọi x ∈ C và λ ∈ R_+^*, ta có p(λx) = λp(x).
(iii) Nếu x ∈ C, hệ thức p(x) = 0 tương đương với x = 0.

b) Ngược lại, cho p là một hàm xác định trên C nhận giá trị trong [0, +∞], thỏa mãn các điều kiện (i), (ii) của a). Cho A là tập hợp các x ∈ C sao cho p(x) ≤ 1. Khi đó A và C − A là lồi. A là một chỏm nếu và chỉ nếu A compact và khác rỗng.

Mệnh đề b) là hiển nhiên. Các tính chất được phát biểu trong a) là các hệ quả của các nhận xét đứng trước mệnh đề 4 và của mệnh đề 22 của II, p. 20 và mệnh đề 23 của II, p. 20 ngoại trừ

$$
p(x + y) \geq p(x) + p(y).
$$

Chỉ cần chứng minh điều cuối cùng này khi x ≠ 0 và y ≠ 0; do đó ta có p(x) > 0, p(y) > 0. Cho μ, λ là hai số > 0 sao cho λ < p(x), μ < p(y), và ký hiệu phần bù của A trong C bởi B. Ta có x ∈ λB, y ∈ μB, do đó x + y ∈ λB + μB; bởi tính lồi của B, ta có λB + μB ⊂ (λ + μ)B, do đó p(x + y) > λ + μ, điều này kéo theo bất đẳng thức đã nêu trên.

#### Hệ quả 1 {#evt-ii-s7-prop-4-cor-1 .statement}

— Cho C là một nón lồi nhọn có đỉnh 0 trong E, một không gian lồi địa phương Hausdorff và cho p là phiếm hàm Minkowski của A, một chỏm của C. Khi đó các điểm cực biên của A là điểm 0, và các điểm x trên các phần tử sinh cực biên của C sao cho p(x) = 1.

Hiển nhiên 0 là một điểm cực biên của A. Cho x là một điểm trên L, một phần tử sinh cực biên của C, và sao cho p(x) = 1. Cho y, z là hai điểm của A sao cho x = $ \frac{1}{2}(y + z) $. Vì L là cực biên, ta có y = λx và z = μx, trong đó λ và μ là các số ≥ 0 sao cho $ \frac{1}{2}(\lambda + \mu) = 1 $, $ \lambda = \lambda p(x) = p(y) \leq 1 $ và $ \mu = \mu p(x) = p(z) \leq 1 $, từ đó suy ra $ \lambda = \mu = 1 $ và do đó y = z = x; vậy x là một điểm cực biên của A. Ngược lại, cho x ≠ 0 là một điểm cực biên của A. Hiển nhiên p(x) = 1. Cho y, y' là hai điểm của C sao cho x = y + y', và ta sẽ chứng minh rằng y, y' tỉ lệ với x. Không làm mất tính tổng quát, ta có thể giả sử rằng các số $ \lambda = p(y) $ và $ \lambda' = p(y') $ là hữu hạn và > 0. Khi đó $ \lambda^{-1}y \in A, \lambda'^{-1}y' \in A, \lambda + \lambda' = 1 $ theo mệnh đề 4, (i) và đẳng thức $ x = \lambda(\lambda^{-1}y) + \lambda'(\lambda'^{-1}y') $ theo giả thiết suy ra rằng

$$
x = \lambda^{-1}y = \lambda'^{-1}y'.
$$

#### Hệ quả 2 {#evt-ii-s7-prop-4-cor-2 .statement}

— Mọi điểm của C thuộc về một cap của C cũng thuộc về bao lồi đóng của hợp các phần tử sinh cực biên của C.

Điều này suy ra ngay lập tức từ hệ quả 1 và định lý Krein-Milman (II, p. 55, định lý 1).

\* Ví dụ. — Cho X là một không gian địa phương compact và là σ-compact. Cho C là một nón lồi đóng có đỉnh 0 trong $ \mathcal{M}_+(X) $ với tôpô mơ hồ. Ta sẽ chứng minh rằng C là hợp các cap của nó. Cho $ (X_n) $ là một dãy tăng các tập mở, compact tương đối của X mà hợp của chúng là X. Cho μ là một phần tử $ \neq 0 $ của C. Tồn tại $ \alpha_n > 0 $ sao cho $ \sum_n \alpha_n \mu(X_n) = 1 $.

Với mọi độ đo $ v \in C $, đặt $ p(v) = \sum_n \alpha_n v(X_n) \in [0, +\infty] $. Hàm p trên C thỏa mãn các điều kiện (i) và (ii) của mệnh đề 4. Nó nửa liên tục dưới đối với tôpô mờ (INT, IV, ấn bản thứ 2, § 1, No. 1, mệnh đề 4). Do đó tập hợp A gồm các $ \gamma \in C $ sao cho $ p(\gamma) \leq 1 $ là đóng và không rỗng. Mặt khác, mọi tập compact của X đều được chứa trong một trong các $ X_n $, vì thế A, do bị chặn theo tôpô mờ, cũng compact đối với tôpô mờ (INT, III, ấn bản thứ 2, § 1, No. 9, mệnh đề 15). Vậy A là một thiết diện của C chứa μ. \*

Mệnh đề 5. — Cho C là một nón lồi thực sự có đỉnh 0 trong E, một không gian yếu Hausdorff; giả sử rằng C là đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của E, và rằng tồn tại một hệ cơ bản đếm được các lân cận của 0 trong C. Khi đó C là hợp của các thiết diện của nó và là bao lồi đóng của hợp các đường sinh cực biên của nó.

Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và từ hệ quả 2 ở trên. Áp dụng mệnh đề 11 của II, p. 52 đưa mệnh đề về trường hợp khi $ E = \mathbf{R}^l $ và $ C \subset \mathbf{R}_+^l $. Với mọi $ \alpha \in I $, ký hiệu phép chiếu $ pr_\alpha $ trong E bởi $ f_\alpha $; khi đó $ f_\alpha $ là một dạng tuyến tính liên tục. Mặt khác, cho $ (V_n)_{n \in \mathbf{N}} $ là một hệ cơ bản đếm được các lân cận của 0 trong C. Theo định nghĩa của tôpô trên E, với mỗi $ n \in \mathbf{N} $, tồn tại một tập con hữu hạn $ J_n $ của I và một số $ \varepsilon_n > 0 $ sao cho $ V_n $ chứa tập hợp $ W_n $ gồm các $ x \in C $ sao cho $ f_\alpha(x) \leq \varepsilon_n $ với mọi $ \alpha \in J_n $; đặt $ J = \bigcup_{n \in \mathbf{N}} J_n $. Cho $ y \neq 0 $ là một điểm của C, và p là hàm $ \sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C) $ trong đó các $ \lambda_\alpha > 0 $ được chọn sao cho $ p(y) = 1 $; điều này là có thể, vì nếu $ f_\alpha(y) = 0 $ với mọi $ \alpha \in J $, thì $ y \in V_n $ với mọi $ n $, điều đó kéo theo $ y = 0 $, trái với giả thiết. Bây giờ nhận xét rằng với mọi $ \alpha \in I $, hàm $ f_\alpha|C $ liên tục tại điểm 0, do đó tồn tại một $ n \in \mathbf{N} $ sao cho $ f_\alpha $ bị chặn trên một $ W_n $, vì thế bị chặn trên trong C bởi một tổ hợp tuyến tính của một số hữu hạn các hàm $ f_\beta|C $, trong đó $ \beta \in J $. Suy ra rằng nếu A là tập hợp các $ x \in C $ sao cho $ p(x) \leq 1 $, thì $ f_\alpha $ bị chặn trên A với mọi $ \alpha \in I $. Vì p nửa liên tục dưới trên C, suy ra A đóng và không rỗng trong C và do đó là compact. Vì hiển nhiên p thỏa mãn các điều kiện (i) và (ii) của mệnh đề 4 của II, p. 58, ta thấy rằng A là một nắp trong C và chứa y.

#### Nhận xét 2 {#evt-ii-s7-n2-rem-2 .statement}

— Tồn tại các nón lồi thực sự vừa yếu đầy đủ vừa không có phần tử sinh cực biên nào (II, p. 92, exerc. 31).

### 3. Các nón lồi có đáy compact

Mệnh đề 6. — Cho E là một không gian lồi địa phương Hausdorff và K là một tập compact lồi trong E không chứa 0. Khi đó nón nhọn nhỏ nhất C có đỉnh 0 chứa $ K $ là một nón lồi thực sự trong $ E $ và là một không gian con địa phương compact và đầy đủ của $ E $; hơn nữa, tồn tại một siêu phẳng đóng $ H $ trong $ E $ không chứa 0 và sao cho $ H $ cắt mọi nửa đường thẳng gốc 0 được chứa trong $ C $ và sao cho $ H \cap C $ là compact. Hơn nữa, nếu $ D $ là nửa không gian chứa 0 được xác định bởi $ H $, một siêu phẳng đóng có các tính chất ấy, thì $ C \cap D $ là một chỏm của $ C $ và $ C $ là hợp của các $ \lambda(C \cap D) $ với $ \lambda > 0 $.

Theo mệnh đề 4 của II, p. 38, tồn tại một siêu phẳng đóng $ H $ tách 0 một cách nghiêm ngặt khỏi $ K $. Bây giờ, bao lồi $ A $ của hợp của $ \{0\} $ và của $ K $ là compắc (II, p. 14, mệnh đề 15) và là hợp của các $ \lambda K $ với $ 0 \leq \lambda \leq 1 $. Vì 0 và $ K $ nằm một cách nghiêm ngặt về hai phía đối của $ H $, với mọi $ x \in K $ tồn tại $ \lambda $ sao cho $ 0 < \lambda < 1 $ và $ \lambda x \in H $. Vì $ C $ là hợp của các $ \lambda A $ với $ \lambda \geq 1 $, ta thấy rằng $ H $ cắt mọi nửa đường thẳng xuất phát từ 0 được chứa trong $ C $ và rằng $ H \cap A = H \cap C $ là compắc. Hơn nữa, $ C $ cũng là hợp của các $ \lambda(H \cap C) $ với $ \lambda \geq 0 $; gọi $ C_n $ là hợp của các $ \lambda(H \cap C) $ với $ 0 \leq \lambda \leq n $. Rõ ràng $ C_n $ là bao lồi của hợp của $ \{0\} $ và của $ n(H \cap C) $, do đó nó là compắc. Hơn nữa, với mọi $ x \in E $, tồn tại một lân cận đóng $ V $ của $ x $ trong $ E $ và một số nguyên $ n $ sao cho $ V \cap C \subset C_n $; thật vậy, nếu $ H $ được xác định bởi phương trình $ f(z) = \alpha $, với $ \alpha > 0 $, thì chỉ cần lấy cho $ V $ nửa không gian đóng được xác định bởi $ nH $ và chứa 0, trong đó $ n $ đủ lớn để $ n\alpha > f(x) $. Điều này chứng tỏ rằng $ C $ là compắc địa phương (lấy $ x \in C $), và rằng nó đóng trong $ E $. Ta cũng có thể xem $ K $ như một tập con của không gian đầy đủ hóa $ \hat{E} $, do đó $ C $ cũng đóng trong $ \hat{E} $ và vì vậy là đầy đủ.

Cho một nón $ C $ và một siêu phẳng đóng $ H $ trong một không gian vectơ tôpô Hausdorff $ E $, sao cho $ H $ không chứa đỉnh $ s $ của $ C $ và $ C $ là nón nhỏ nhất có đỉnh $ s $ chứa $ H \cap C $, thì ta gọi giao $ H \cap C $ là một « đáy » của nón $ C $. Mệnh đề 6 chỉ ra rằng trong một không gian lồi địa phương Hausdorff $ E $, nón nhỏ nhất có đỉnh 0, chứa một tập hợp lồi compắc $ K $ mà 0 không thuộc, là một nón có đáy compắc, và mọi nón lồi có một đáy compắc $ S $ đều là địa phương compắc và đầy đủ.

#### Ví dụ {#evt-ii-s7-n3-exa-1 .statement}

— 1) Mọi nón lồi đóng thực sự trong $ E $, một không gian vectơ có số chiều hữu hạn, đều có một đáy compact. Thật vậy, theo II, p. 52, mệnh đề 11, ta chỉ cần xét trường hợp $ E = \mathbf{R}^n $ và $ C = \mathbf{R}_+^n $. Nếu $ (e_i)_{1 \leq i \leq n} $ là cơ sở chính tắc của $ \mathbf{R}^n $, thì hiển nhiên tập lồi compact là bao lồi của các $ e_i $ ($ 1 \leq i \leq n $) là một đáy compact của $ \mathbf{R}_+^n $.

\* 2) Nếu $ X $ là một không gian compact, thì nón $ \mathcal{M}_+(X) $ các độ đo dương trên $ X $, với tôpô mơ hồ, là một nón có một đáy compact (INT, III, 2nd ed., § 1, No. 9, hệ quả 3 của mệnh đề 15). \*

### Bài tập {#evt-ii-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
