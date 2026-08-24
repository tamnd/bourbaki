---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 8
section_title: Complex locally convex spaces
lang: vi
source: evt-i-v
book_pages: TVS II.95
pdf_pages: 0097-0102, 0132-0132
extraction: ocr
subsections:
    - "no": 1
      title: Topological vector spaces over $ \mathbf{C} $
      page: 60
      pdf_page: 97
    - "no": 2
      title: Complex locally convex spaces
      page: 62
      pdf_page: 99
    - "no": 3
      title: The Hahn-Banach theorem and its applications
      page: 63
      pdf_page: 100
    - "no": 4
      title: Weak topologies on complex vector spaces
      page: 64
      pdf_page: 101
statements: 10
exercises: 3
content_sha256: a8d9510bb9d88bb64c7cf9d0cba266fc82c554084b29ee94daae20ab994b1ada
translated_from: content/en/evt/II/08_s8_complex_locally_convex_spaces.md
source_content_sha256: f1b6f9a0f20e8a5d426e0afb015b4b18f923029970ed2f6ea81b92b6461e39ff
translation_model: gpt-5.4
translation_run: translate-vi-5e3c7937
glossary_version: 34
glossary_terms_sha256: 60d9a344896129b744fb54988d5c556221956de081e0aee34044fe8a890b2973
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. CÁC KHÔNG GIAN PHỨC LỒI ĐỊA PHƯƠNG

### 1. Các không gian vectơ tôpô trên $ \mathbf{C} $

Cho $ E $ là một không gian vectơ tôpô trên $ \mathbf{C} $, trường số phức; tôpô của $ E $ cũng tương thích với cấu trúc không gian vectơ trên $ \mathbf{R} $, thu được bằng cách hạn chế trường các vô hướng xuống $ \mathbf{R} $. Ta ký hiệu bởi $ E_0 $ không gian vectơ tôpô trên $ \mathbf{R} $ *nền tảng của* E (I, p. 2). Chú ý rằng, trong $ E_0 $, ánh xạ $ x \mapsto ix $ (không phải là một phép vị tự) là một *tự đẳng cấu* $ u $ của cấu trúc không gian vectơ tôpô của $ E_0 $ sao cho $ u^2(x) = -x $.

Ngược lại, cho F là một không gian vectơ tôpô trên $ \mathbf{R} $, và giả sử rằng tồn tại một tự đẳng cấu $ u $ của F sao cho $ u^2 = -1_F $ ($ 1_F $ là tự đẳng cấu đồng nhất của F). Ta biết (A, IX, § 3, No. 2) rằng khi đó có thể định nghĩa trên F một cấu trúc không gian vectơ đối với $ \mathbf{C} $ bằng cách viết $ \lambda x = \alpha x + \beta u(x) $ với mọi $ \lambda = \alpha + i\beta \in \mathbf{C} $ và mọi $ x \in F $. Hơn nữa, vì ánh xạ $ (\alpha, \beta, x) \mapsto \alpha x + \beta u(x) $ từ $ \mathbf{R}^2 \times F $ vào F là liên tục nên tôpô của F tương thích với cấu trúc không gian vectơ đối với $ \mathbf{C} $ được định nghĩa ở trên; nếu E ký hiệu không gian vectơ tôpô trên $ \mathbf{C} $ được định nghĩa theo cách đó, thì F là không gian vectơ tôpô trên $ \mathbf{R} $ làm nền cho E.

#### Nhận xét {#evt-ii-s8-n1-rem-1 .statement}

— Với một không gian vectơ tôpô F trên $ \mathbf{R} $, không phải luôn luôn tồn tại một tự đẳng cấu $ u $ của F mà bình phương của nó là $ -1_F $; chẳng hạn, không thể định nghĩa cấu trúc không gian vectơ đối với $ \mathbf{C} $ trên một không gian vectơ trên $ \mathbf{R} $ có chiều *lẻ* hữu hạn.

Cho E là một không gian vectơ tôpô trên $ \mathbf{C} $, và $ E_0 $ là không gian vectơ tôpô trên $ \mathbf{R} $ làm nền cho E. Mọi đa tạp tuyến tính M trong E cũng là một đa tạp tuyến tính trong $ E_0 $, nhưng đảo lại thì sai. Để tránh nhầm lẫn, ta nói rằng một đa tạp tuyến tính đối với một cấu trúc không gian vectơ trên $ \mathbf{C} $ (tương ứng trên $ \mathbf{R} $) là một đa tạp tuyến tính *phức* (tương ứng *thực*). Một đa tạp tuyến tính phức có chiều hữu hạn $ n $ (tương ứng có đối chiều hữu hạn $ n $) là một đa tạp tuyến tính thực có chiều $ 2n $ (tương ứng có đối chiều $ 2n $). Để một không gian con vectơ thực M của E cũng là một không gian con vectơ phức, điều kiện cần và đủ là $ iM \subset M $.

Nhớ rằng, nếu E và F là hai không gian vectơ tôpô trên $ \mathbf{C} $, thì một ánh xạ từ E vào F được gọi là $ \mathbf{C} $-tuyến tính (tương ứng $ \mathbf{R} $-tuyến tính) nếu nó là một ánh xạ tuyến tính đối với các cấu trúc không gian vectơ của E và của F trên $ \mathbf{C} $ (tương ứng $ \mathbf{R} $); mọi ánh xạ $ \mathbf{C} $-tuyến tính hiển nhiên đều $ \mathbf{R} $-tuyến tính nhưng đảo lại thì sai. Ta nói rằng một dạng tuyến tính $ \mathbf{C} $ trên E là một dạng tuyến tính *phức* và rằng một dạng tuyến tính $ \mathbf{R} $ trên E (*tức là* một dạng tuyến tính trên $ E_0 $) là một dạng tuyến tính *thực*. Nếu $ f $ là một dạng tuyến tính phức trên E, thì hiển nhiên phần thực $ g = \Re f $ và phần ảo $ h = \Im f $ của $ f $ là các dạng tuyến tính thực; hơn nữa, quan hệ $ f(ix) = if(x) $ kéo theo đẳng thức $ h(x) = -g(ix) $; nói cách khác, ta có

$$
f(x) = (\Re f)(x) - i(\Re f)(ix).
$$

Ngược lại, nếu $ g $ là một dạng tuyến tính thực trên E, thì $ f(x) = g(x) - ig(ix) $ là dạng tuyến tính phức duy nhất trên E sao cho $ \Re f = g $; và $ f $ liên tục khi, và chỉ khi, $ g $ liên tục.

Bây giờ cho H là một *siêu phẳng phức* trong E, có phương trình $ f(x) = \alpha + i\beta $, trong đó $ f $ là một dạng tuyến tính phức trên E; đặt $ g = \Re f $, ta thấy rằng H là giao của hai *siêu phẳng thực* $ H_1, H_2 $ có các phương trình lần lượt là $ g(x) = \alpha $ và $ g(ix) = -\beta $; nếu H là *đóng* thì $ H_1 $ và $ H_2 $ cũng vậy (I, p. 13, th. 1). Ngược lại, cho $ H_0 $ là một siêu phẳng *thực* thuần nhất, có phương trình $ g(x) = 0 $ (trong đó $ g $ là một dạng tuyến tính thực trên E); khi đó H, giao của $ H_0 $ và $ iH_0 $, là một siêu phẳng *phức* thuần nhất, và nếu $ f $ là dạng tuyến tính phức sao cho $ \Re f = g $, thì $ f(x) = 0 $ là phương trình của H; nếu $ H_0 $ đóng thì H cũng đóng.

Cho G là một không gian vectơ tôpô trên $ \mathbf{R} $ và gọi $ G_{(c)} $ là không gian vectơ trên $ \mathbf{C} $ thu được từ G bằng cách mở rộng trường vô hướng lên $ \mathbf{C} $ (A, II, § 5.1). Đồng nhất G với một tập con của $ G_{(c)} $ bởi ánh xạ $ x \mapsto 1 \otimes x $. Khi đó ánh xạ $ \mathbf{R} $-tuyến tính $ (x, y) \mapsto x + i.y $ là một song ánh từ $ G \times G $ lên $ G_{(c)} $, nhờ đó ta chuyển tôpô tích của $ G \times G $ sang $ G_{(c)} $. Khi đó $ G_{(c)} $ với tôpô này là một không gian vectơ tôpô trên $ \mathbf{C} $. Ta nói rằng $ G_{(c)} $ là *không gian vectơ tôpô phức hóa của* G.

### 2. Không gian lồi địa phương phức

Nói rằng một tập con A của một không gian vectơ phức E là *cân bằng* có nghĩa là, với mọi $ x \in A $, ta có $ \rho x \in A $ khi $ 0 \leq \rho \leq 1 $ và $ e^{i\vartheta}x \in A $ với mọi $ \vartheta $ thực.

Ta nói rằng một tập hợp A của E là *lồi* nếu nó lồi trong không gian thực $ E_0 $ làm nền cho E. Để một tập lồi $ A \neq \varnothing $ của E là cân bằng, điều kiện đủ là $ e^{i\vartheta}A \subset A $ với mọi $ \vartheta $ thực; thật vậy, điều đó trước hết kéo theo rằng $ -A = A $; vì A lồi, suy ra 0 thuộc A và do đó $ \rho A \subset A $ khi $ 0 \leq \rho \leq 1 $.

Cho E là một không gian vectơ tôpô phức. Tập hợp cân bằng lồi nhỏ nhất (tương ứng, tập hợp đóng cân bằng lồi nhỏ nhất) chứa một tập hợp A của E được gọi là *bao lồi cân bằng* (tương ứng, *bao đóng lồi cân bằng*) của A; bao đóng lồi cân bằng của A là bao đóng của bao lồi cân bằng của A. Tập hợp sau cùng này là bao lồi của hợp các tập hợp $ e^{i\vartheta}A $; do đó ta có thể định nghĩa nó là tập hợp các tổng tuyến tính $ \sum_i \lambda_i x_i $, khi $ (x_i) $ là một họ hữu hạn bất kỳ các điểm của A, và $ (\lambda_i) $ là một họ các số phức sao cho $ \sum_i |\lambda_i| \leq 1 $. Nếu A là tiền compắc thì bao cân bằng của nó cũng vậy (I, p. 6, prop. 3).

Ta nói rằng một không gian vectơ tôpô phức E là *lồi địa phương* nếu không gian vectơ tôpô thực nền $ E_0 $ là lồi địa phương, nghĩa là nếu mọi lân cận của 0 trong E đều chứa một lân cận lồi của 0; một tôpô $ \mathcal{T} $ trên E là *lồi địa phương* nếu nó tương thích với cấu trúc không gian vectơ của E (đối với $ \mathbf{C} $) và nếu E, với tôpô $ \mathcal{T} $, là lồi địa phương. Vì trong trường hợp này mọi lân cận đóng lồi V của 0 đều chứa một lân cận cân bằng W của 0 (I, p. 7, prop. 4), ta thấy rằng V cũng chứa U, là bao đóng lồi cân bằng của W; nói cách khác, các lân cận *cân bằng, đóng, lồi* của 0 lập thành một hệ cơ bản các lân cận của 0 trong E, bất biến dưới mọi phép vị tự có tỷ số $ \neq 0 $.

Ngược lại, cho E là một không gian vectơ phức và $ \mathfrak{S} $ là một cơ sở lọc trên E gồm các tập hợp *hấp thụ*, *lồi cân bằng*. Khi đó ta biết (II, p. 23, prop. 1) rằng tập hợp $ \mathfrak{B} $, gồm các ảnh của các tập hợp thuộc $ \mathfrak{S} $ qua các phép vị tự có tỉ số $ > 0 $, là một hệ cơ bản các lân cận của 0 đối với một tôpô lồi địa phương $ \mathcal{T} $ trên không gian vectơ thực $ E_0 $ làm nền cho E. Hơn nữa, vì các tập hợp của $ \mathfrak{B} $ là cân bằng, chúng bất biến dưới mọi phép vị tự $ x \mapsto e^{i\vartheta}x $, điều đó cho thấy $ \mathcal{T} $ là tương thích với cấu trúc không gian vectơ của E (trên $ \mathbf{C} $) (I, p. 7, prop. 4).

Mọi tôpô lồi địa phương trên một không gian vectơ phức E đều có thể được xác định bởi một tập hợp các nửa chuẩn, vì phiếm hàm Minkowski của một lân cận mở lồi cân bằng của 0 là một nửa chuẩn trên E.

Các ý tưởng và kết quả đối với các không gian lồi địa phương thực được trình bày chi tiết trong II, p. 25 đến 36, mở rộng sang các không gian lồi địa phương phức mà không cần sửa đổi gì ngoài việc thay các tập hợp lồi đối xứng bằng các tập hợp lồi cân bằng.

Một không gian lồi địa phương phức là một không gian Fréchet nếu nó mêtric hóa được và đầy đủ.

### 3. Định lý Hahn-Banach và các ứng dụng của nó

#### Định lý 1 (Hahn-Banach) {#evt-ii-s8-thm-1 .statement}

— Cho V là một không gian con vectơ của E, trong đó E là một không gian vectơ phức, và cho f là một dạng tuyến tính (phức) trên V và p là một nửa chuẩn trên E sao cho $ |f(y)| \leq p(y) $ với mọi $ y \in V $. Khi đó tồn tại một dạng tuyến tính $ f_1 $ trên E mở rộng f và sao cho $ |f_1(x)| \leq p(x) $ với mọi $ x \in E $.

Vì $ g = \Re f $ là một dạng tuyến tính thực được xác định trên V và thỏa mãn $ |\cdot(y)| \leq p(y) $ tại mọi điểm của V; do đó tồn tại một dạng tuyến tính thực $ g_1 $ trên E kéo dài g và sao cho $ |g_1(x)| \leq p(x) $ với mọi $ x \in E $ (II, p. 23, hệ quả 1). Đặt $ f_1(x) = g_1(x) - ig_1(ix) $ là dạng tuyến tính phức trên E mà $ g_1 $ là phần thực của nó (II, p. 61). Với mọi số thực $ \vartheta $

$$
|\Re(e^{i\vartheta}f_1(x))| = |\Re(f_1(e^{i\vartheta}x))| = |g_1(e^{i\vartheta}x)| \leq p(e^{i\vartheta}x) = p(x)
$$

vì $ p $ là một nửa chuẩn trên không gian phức E; điều này suy ra quan hệ $ |f_1(x)| \leq p(x) $, và định lý được chứng minh.

#### Hệ quả 1 {#evt-ii-s8-thm-1-cor-1 .statement}

— Cho $ x_0 $ là một điểm của một không gian vectơ tôpô phức E và p là một nửa chuẩn liên tục trên E; khi đó tồn tại một dạng tuyến tính liên tục (phức) f được xác định trên E, sao cho $ f(x_0) = p(x_0) $ và $ |f(x)| \leq p(x) $ với mọi $ x \in E $.

#### Hệ quả 2 {#evt-ii-s8-thm-1-cor-2 .statement}

— Cho V là một không gian con vectơ của một không gian lồi địa phương phức E và f là một dạng tuyến tính phức xác định và liên tục trên V; khi đó tồn tại một dạng tuyến tính liên tục $ f_1 $ xác định trên E và kéo dài f. Nếu E là không gian định chuẩn thì tồn tại một dạng $ f_1 $ như vậy còn thỏa mãn $ \|f_1\| = \|f\| $.

#### Hệ quả 3 {#evt-ii-s8-thm-1-cor-3 .statement}

— Cho M là một không gian con vectơ hữu hạn chiều của một không gian lồi địa phương phức Hausdorff E. Khi đó tồn tại một không gian con vectơ đóng N của E là một phần bù tôpô của M trong E.

Các chứng minh dùng định lý 1, p. 24 giống hệt các chứng minh của II, p. 23, hệ quả 2 và hệ quả 3, p. 24, mệnh đề 2 và p. 25, hệ quả 2.

#### Mệnh đề 1 {#evt-ii-s8-prop-1 .statement}

— Cho A là một tập hợp lồi mở không rỗng trong một không gian vectơ tôpô phức E và M là một đa tạp tuyến tính phức không rỗng không giao với A. Khi đó tồn tại một siêu phẳng phức đóng H chứa M và không giao với A.

Ta có thể giả sử rằng $ 0 \in M $. Khi đó tồn tại một siêu phẳng thực đóng $ H_0 $ chứa M và không giao với A (II, p. 36; định lý 1). Vì $ M = iM $, siêu phẳng phức đóng $ H = H_0 \cap (iH_0) $ có các tính chất được yêu cầu.

#### Hệ quả {#evt-ii-s8-n3-cor-1 .statement}

— Trong một không gian lồi địa phương phức E, mọi đa tạp tuyến tính phức đóng M là giao của các siêu phẳng phức đóng chứa nó.

Thật vậy, với mọi $ x \notin M $, tồn tại một lân cận mở lồi $ V $ của $ x $ không giao với $ M $, và do đó tồn tại một siêu phẳng phức đóng $ H $ chứa $ M $ và không giao với $ V $; *a fortiori* $ H $ không chứa $ x $.

#### Mệnh đề 2 {#evt-ii-s8-prop-2 .statement}

*Cho $ A $ là một tập hợp cân bằng lồi mở không rỗng của một không gian vectơ tôpô phức $ E $, và $ B $ là một tập hợp lồi không rỗng không giao với $ A $. Khi đó tồn tại một dạng tuyến tính phức liên tục $ f $ trên $ E $ và một số $ \alpha > 0 $ sao cho $ |f(x)| < \alpha $ trong $ A $ và $ |f(y)| \geq \alpha $ trong $ B $.*

Thật vậy, tồn tại một dạng tuyến tính *thực* liên tục $ g $ trên $ E $ và một số thực $ \alpha $ sao cho $ g(x) < \alpha $ trong $ A $ và $ g(y) \geq \alpha $ trong $ B $ (II, p. 37, mệnh đề 1). Vì $ 0 \in A $, ta có $ \alpha > 0 $. Ta chỉ ra rằng dạng tuyến tính phức liên tục $ f(x) = g(x) - ig(ix) $ và số $ \alpha $ có các tính chất cần có. Thật vậy, vì $ \Re f = g $, ta có $ |f(y)| \geq \alpha $ trong $ B $. Mặt khác, với mọi $ x \in A $ và mọi $ \vartheta $ thực, điểm $ e^{i\vartheta}x $ thuộc $ A $, vì $ A $ là cân bằng, và ta có $ f(x) = e^{-i\vartheta}f(e^{i\vartheta}x) $; khi đó tồn tại một số $ \vartheta $ sao cho $ |f(x)| = \Re(e^{i\vartheta}f(x)) = g(e^{i\vartheta}x) < \alpha $, và mệnh đề được suy ra.

#### Mệnh đề 3 {#evt-ii-s8-prop-3 .statement}

*Cho $ A $ là một tập hợp cân bằng, đóng, lồi trong một không gian lồi địa phương phức $ E $ và cho $ K $ là một tập hợp lồi compắc không rỗng trong $ E $ không giao với $ A $. Khi đó tồn tại một dạng tuyến tính phức liên tục $ f $ trên $ E $ và một số $ \alpha > 0 $ sao cho $ |f(x)| < \alpha $ trên $ A $ và $ |f(y)| > \alpha $ trên $ K $.*

Mệnh đề này suy ra từ II, p. 38, mệnh đề 4 như mệnh đề 2 suy ra từ II, p. 37, mệnh đề 1.

### 4. Các tôpô yếu trên các không gian vectơ phức

Định nghĩa và các kết quả của II, § 6, Nos. 1 và 2 áp dụng không thay đổi cho các không gian vectơ *phức*. Nếu $ F $ và $ G $ là hai không gian vectơ phức đối ngẫu với nhau bởi một dạng song tuyến tính $ B $, thì các không gian nền $ F_0 $ và $ G_0 $ đối ngẫu với nhau bởi $ \Re B $, và suy ra từ II, p. 61, công thức (1) rằng các tôpô yếu $ \sigma(F, G) $ và $ \sigma(F_0, G_0) $ là đồng nhất.

#### Định nghĩa 1 {#evt-ii-s8-def-1 .statement}

*Cho $ F $ và $ G $ là hai không gian vectơ phức đối ngẫu với nhau. Với mọi tập con $ M $ của $ F $, cực của $ M $ trong $ G $, ký hiệu là $ M^\circ $, là tập hợp các $ y \in G $ sao cho $ \Re(\langle x, y \rangle) \geq -1 $ với mọi $ x \in M $.*

Nếu $ M^\circ $ là cực của $ M \subset F $ trong $ G $ thì $ (\lambda M)^\circ = \lambda^{-1}M^\circ $ với mọi $ \lambda \in \mathbf{C}^* $.

Nếu $ M $ là một không gian con vectơ (phức) của $ E $, thì $ M^\circ $ là một không gian con vectơ đóng (đối với $ \sigma(G, F) $), vì quan hệ $ \Re(\lambda \langle x, y \rangle) \geq -1 $ với *mọi* vô hướng $ \lambda \in \mathbf{C} $ suy ra $ \langle x, y \rangle = 0 $; ở đây nữa ta nói rằng $ M^\circ $ là không gian con của $ G $ *trực giao* với $ M $.

Nếu $ M $ là một tập hợp cân bằng trong $ F $, thì $ M^\circ $ là một tập hợp cân bằng trong $ G $; trong trường hợp này $ M^\circ $ là tập hợp các $ y \in G $ sao cho $ |\langle x, y \rangle| \leq 1 $ với mọi $ x \in M $; vì quan hệ này tương đương với $ \Re(\langle \zeta x, y \rangle) \leq 1 $ với mọi $ x \in M $ và mọi $ \zeta \in \mathbf{C} $ sao cho $ |\zeta| = 1 $.

Các kết quả của II, p. 41 đến 51 cũng đúng không có hạn chế nào đối với các không gian vectơ phức.

Bài tập

### Bài tập {#evt-ii-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
