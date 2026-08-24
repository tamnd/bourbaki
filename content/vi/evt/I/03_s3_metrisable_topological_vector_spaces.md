---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 3
section_title: Metrisable topological vector spaces
lang: vi
source: evt-i-v
book_pages: TVS I.28-TVS I.29
pdf_pages: 0024-0030, 0036-0037
extraction: ocr
subsections:
    - "no": 1
      title: Neighbourhoods of 0 in a metrisable topological vector space
      page: 16
      pdf_page: 24
    - "no": 2
      title: Properties of metrisable vector spaces
      page: 17
      pdf_page: 25
    - "no": 3
      title: Continuous linear functions in a metrisable vector space
      page: 17
      pdf_page: 25
statements: 11
exercises: 9
content_sha256: 9c88732d9a39f151af3933a8377bb36ccfb45bcbfb04d6d143c296448e07cf0f
translated_from: content/en/evt/I/03_s3_metrisable_topological_vector_spaces.md
source_content_sha256: 184c133d6175f986f7939f6da88ce54db00e8a895f550755698af591ddbd4947
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-7fcbc987
glossary_version: 34
glossary_terms_sha256: b9d89d12dc667051b8a3549959d021e4af53db9e49e21adb0aa9848cc4d8a17b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC KHÔNG GIAN VECTƠ TÔPÔ KHẢ METRIC HÓA

### 1. Các lân cận của 0 trong một không gian vectơ tôpô khả metric hóa

Ta nói rằng một không gian vectơ tôpô E là *khả metric hóa* nếu tôpô của nó là khả metric hóa. Xét theo cấu trúc nhóm cộng và tôpô của nó, do đó E là một nhóm khả metric hóa (GT, IX, § 3.1).

Ta biết rằng, để một nhóm tôpô là khả metric hóa, điều kiện cần và đủ là tồn tại một hệ cơ bản đếm được các lân cận của phần tử đơn vị $ e $, mà giao của chúng là phần tử duy nhất $ e $ (GT, IX, § 3.1, mệnh đề 1).

Ta cũng biết rằng cấu trúc đều của một không gian vectơ tôpô khả metric hóa E có thể được xác định bởi một *khoảng cách bất biến* $ d(x, y) = |x - y| $, trong đó $ x \mapsto |x| $ là một ánh xạ liên tục từ E vào $ \mathbf{R}_+ $ thỏa mãn các điều kiện: 1) $ |-x| = |x| $; 2) $ |x + y| \leq |x| + |y| $; 3) quan hệ $ |x| = 0 $ tương đương với $ x = 0 $ (GT, IX, § 3.1, mệnh đề 3).

Ta đã thấy (GT, IX.§ 3.1, prop. 2) cách một khoảng cách như vậy d có thể được định nghĩa bằng cách dùng một dãy giảm $ (W_n) $ các lân cận của 0 trong E, tạo thành một hệ cơ bản các lân cận và sao cho $ W_{n+1} + W_{n+1} + W_{n+1} \subset W_n $. Khi E là một không gian vectơ khả mêtric trên một vành chia định giá không rời rạc K, ta cũng có thể giả sử rằng các $ W_n $ là cân bằng (I, p. 7, prop. 4); nếu ta quay lại quá trình định nghĩa của $ d $ (*loc. cit.*) thì có thể thấy *quan hệ* $ |\lambda| \leq 1 \implies |\lambda x| \leq |x| $. Hơn nữa các điều kiện (EVT$_I$) và (EVT$_{II}$) của I, p. 2 kéo theo cả việc $ |\lambda x_0| $ *tiến tới 0 khi $ \lambda $ tiến tới 0 trong K* với mọi $ x_0 \in E $, lẫn việc $ |\lambda_0 x| $ *tiến tới 0 khi $ |x| $ tiến tới 0* với mọi $ \lambda_0 \in K $. Ngược lại, nếu hàm $ |x| $ có tất cả các tính chất trước đó và nếu $ W_n $ là tập hợp các $ x \in E $ sao cho $ |x| \leq 2^{-n} $, thì các $ W_n $ tạo thành một hệ cơ bản các lân cận cân bằng của 0 đối với một tôpô khả mêtric trên E tương thích với cấu trúc không gian vectơ của E.

#### Nhận xét {#evt-i-s3-n1-rem-1 .statement}

Một trong những lớp quan trọng nhất của các không gian vectơ mêtric hoá được là các không gian định chuẩn (I, p. 3). Nhưng cần lưu ý rằng tồn tại các không gian vectơ mêtric hoá được mà tôpô của chúng không thể được xác định bởi một chuẩn (I, § 3, exerc. 1); về sau chúng ta sẽ nghiên cứu các ví dụ quan trọng.

### 2. Các tính chất của các không gian vectơ mêtric hoá được

Mọi không gian con vectơ của một không gian vectơ tôpô mêtric hoá được E đều mêtric hoá được; điều tương tự đúng cho mọi không gian thương E/M của E bởi một không gian con vectơ đóng M (GT, IX, § 3.1, prop. 4). Mọi tích của một họ đếm được các không gian vectơ tôpô mêtric hoá được đều mêtric hoá được (GT, IX, § 2.4, cor. 2). Nếu K_0 là một vành chia định giá đầy đủ, và K là một vành con chia trù mật khắp nơi trong K_0, phép đầy đủ $ \hat{E} $ của một không gian vectơ mêtric hoá được E trên K là một không gian vectơ mêtric hoá được trên K_0 (I, p. 6 và GT, IX, § 2, No. 1, prop. 1). Cuối cùng, nếu E là một không gian vectơ mêtric hoá được đầy đủ, thì với mọi không gian con vectơ đóng M của E, không gian thương E/M là đầy đủ (GT, IX, § 3.1, prop. 4).

### 3. Các hàm tuyến tính liên tục trong một không gian vectơ mêtric hoá được

#### Định lý 1 (Banach) {#evt-i-s3-thm-1 .statement}

Cho E và F là hai không gian vectơ mêtric hoá được trên một vành chia định giá không rời rạc K, và cho u là một ánh xạ tuyến tính liên tục của E vào F. Giả sử rằng E là đầy đủ. Khi đó các điều kiện sau là tương đương:
(i) u là một cấu xạ toàn ánh ngặt.
(ii) F là đầy đủ và u là toàn ánh.
(iii) Ảnh của u không là tập hợp hạng bé trong F (GT, IX, § 5.2).
(iv) Với mọi lân cận V của 0 trong E, tập hợp $ \overline{u(V)} $ là một lân cận của 0 trong F.

Trước hết (i) kéo theo (ii), vì cho u là một cấu xạ toàn ánh ngặt và N là hạt nhân của u. Khi đó u cảm sinh một đẳng cấu từ E/N lên F. Nhưng E mêtric hoá được và đầy đủ, do đó E/N là đầy đủ (GT, IX, § 3.1, prop. 4), vậy F là đầy đủ.

Tiếp theo (ii) kéo theo (iii). Cho F là đầy đủ và u là toàn ánh. Ảnh của u chính xác là F và do đó không là tập hợp hạng bé trong F theo định lý Baire (GT, IX, § 5.3).

Bổ đề sau đây chỉ ra rằng (iii) kéo theo (iv).

#### Bổ đề 1 {#evt-i-s3-lem-1 .statement}

Cho E và F là hai không gian vectơ tôpô trên một vành chia định giá không rời rạc K, và cho u là một ánh xạ tuyến tính liên tục của E vào F sao cho ảnh của E không là tập hợp hạng bé. Khi đó, với mọi lân cận V của 0 trong E, tập hợp $ \overline{u(V)} $ là một lân cận của 0 trong F.

Cho W là một lân cận cân bằng của 0 trong E sao cho W + W ⊂ V (I, § 1.5, prop. 4). Cho α là một phần tử của K sao cho |α| > 1; khi đó E là hợp của các tập hợp $ \alpha^n W $ trong đó n biến thiên trong $ \mathbf{N} $; thực vậy, với mọi x ∈ E, tồn tại β ∈ K sao cho x ∈ βW (I, p. 7, prop. 4) và tồn tại một số nguyên n ≥ 0 sao cho |β| < |α|^n, khi đó x ∈ $ \alpha^n W $ vì W là cân bằng. Do đó, u(E) là hợp của dãy các tập hợp $ u(\alpha^n W) = \alpha^n u(W) $, và vì u(E) không là tập hợp hạng bé trong F, ít nhất một trong các tập hợp $ \alpha^n \overline{u(W)} $ có một điểm trong (GT, IX, § 5.3, def. 2) và do đó $ \overline{u(W)} $ có một điểm trong.

Cho $ y_0 $ là một điểm trong của $ \overline{u(W)} $; vì $ -u(W) = u(W) $, và do đó $ -\overline{u(W)} = \overline{u(W)} $ nên suy ra $ 0 = y_0 + (-y_0) $ là một điểm trong của $ \overline{u(W)} + \overline{u(W)} $. Vì phép cộng vectơ là một ánh xạ liên tục từ $ F \times F $ vào $ F $, tập hợp $ \overline{u(W)} + \overline{u(W)} $ được chứa trong bao đóng của tập hợp

$$
u(W) + u(W) = u(W + W) \subset u(V);
$$

do đó $ \overline{u(V)} $ là một lân cận của 0 trong $ F $.

Trước khi chứng minh rằng (iv) kéo theo (i), ta chứng minh bổ đề sau đây, trong đó ta quy ước rằng, trong mọi không gian mêtric, $ B_r(x) $ ký hiệu quả cầu *đóng* tâm $ x $ bán kính $ r $.

#### Bổ đề 2 {#evt-i-s3-lem-2 .statement}

*Cho E và F là hai không gian mêtric, và giả sử thêm rằng E cũng đầy đủ. Cho u là một ánh xạ tuyến tính từ E vào F có tính chất sau: với mọi số $ r > 0 $, tồn tại một số $ \rho(r) > 0 $ sao cho, với mọi $ x \in E $, ta có*

$$
B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))}.
$$

*Trong các điều kiện ấy, với mọi $ a > r $, ảnh $ u(B_a(x)) $ chứa quả cầu $ B_{\rho(r)}(u(x)) $.*

Cho $ (r_n) $ là một dãy vô hạn các số $ > 0 $ sao cho $ r_1 = r $ và $ a = \sum_{n=1}^{\infty} r_n $. Với mỗi chỉ số $ n $ tồn tại một số $ \rho_n > 0 $ (với $ \rho_1 = \rho(r) $) sao cho

$$
B_{\rho_n}(u(x)) \subset \overline{u(B_{r_n}(x))}
$$

với mọi $ x \in E $; ta có thể, và sẽ, giả sử rằng $ \lim_{n \to \infty} \rho_n = 0 $.

Cho $ x_0 $ là một điểm của E, và $ y $ là một điểm của $ B_{\rho(r)}(u(x_0)) $. Ta sẽ chứng minh rằng $ y $ thuộc $ u(B_a(x_0)) $.

Vì mục đích đó, một dãy $ (x_n)_{n>0} $ các điểm của E được định nghĩa bằng quy nạp sao cho, với mọi $ n \geq 1 $, ta có $ x_n \in B_{r_n}(x_{n-1}) $ và $ u(x_n) \in B_{\rho_{n+1}}(y) $. Nếu các $ x_i $ đã được định nghĩa với $ 0 \leq i \leq n-1 $ và thỏa mãn các hệ thức ấy, thì ta có $ y \in B_{\rho_n}(u(x_{n-1})) $; vì

$$
B_{\rho_n}(u(x_{n-1})) \subset \overline{u(B_{r_n}(x_{n-1}))},
$$

tồn tại một điểm $ x_n \in B_{r_n}(x_{n-1}) $ mà ảnh $ u(x_n) $ của nó thuộc lân cận $ B_{\rho_{n+1}}(y) $ của $ y $, điều đó thiết lập sự tồn tại của dãy $ (x_n) $.

Vì khoảng cách từ $ x_n $ đến $ x_{n+p} $ nhỏ hơn $ r_{n+1} + r_{n+2} + \cdots + r_{n+p} $, mà đại lượng này nhỏ tùy ý khi $ n $ đủ lớn, nên dãy $ (x_n) $ là một dãy Cauchy trong E. Vì E đầy đủ, dãy $ (x_n) $ hội tụ đến một điểm $ x $ của E. Khoảng cách từ $ x_0 $ đến $ x $ nhỏ hơn $ \sum_{n=1}^{\infty} r_n = a $, do đó $ x \in B_a(x_0) $. Nhưng $ u $ liên tục, nên dãy $ u(x_n) $ hội tụ đến $ u(x) $; mặt khác $ u(x_n) \in B_{\rho_{n+1}}(y) $, suy ra $ y = u(x) $, và bổ đề được chứng minh.

Ta quay lại định lý và chứng minh rằng (iv) kéo theo (i). Giả sử rằng $ u $ thỏa mãn điều kiện (iv). Đối với mỗi không gian E và F, xét một khoảng cách bất biến theo phép tịnh tiến và xác định tôpô của nó (I, p. 16). Theo giả thiết, tập $ \overline{u(B_r(0))} $ là một lân cận của 0 trong F với mọi $ r > 0 $, và do đó tồn tại một số $ \rho(r) > 0 $ sao cho $ B_{\rho(r)}(0) \subset u(B_r(0)) $. Bằng phép tịnh tiến ta kết luận rằng $ B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))} $ với mọi $ r > 0 $ và mọi $ x \in E $. Theo bổ đề 2, với mọi cặp số thực dương $ (a, r), a > r > 0 $, ta có $ B_{\rho(r)}(0) \subset u(B_a(0)) $; do đó $ u $ là một cấu xạ ngặt của E lên F. Ta đã chứng minh rằng (iv) kéo theo (i) và chứng minh của định lý được hoàn tất.

#### Hệ quả 1 {#evt-i-s3-lem-2-cor-1 .statement}

*Nếu E và F là hai không gian vectơ mêtric hóa được đầy đủ trên một thể có giá trị không rời rạc, thì mọi ánh xạ tuyến tính liên tục song ánh của E lên F đều là một đẳng cấu.*

Đặc biệt, nếu E và F là hai không gian *định chuẩn* đầy đủ, thì tồn tại một số $ a > 0 $ sao cho $ \|u(x)\| \geq a.\|x\| $ với mọi $ x \in E $.

#### Hệ quả 2 {#evt-i-s3-lem-2-cor-2 .statement}

*Cho E là một không gian vectơ trên một vành chia được định giá không rời rạc, và $ \mathcal{T}_1 $ và $ \mathcal{T}_2 $ là hai tôpô trên E tương thích với cấu trúc không gian vectơ của nó và đối với mỗi tôpô ấy E đều mêtric hóa được và đầy đủ. Khi đó, nếu $ \mathcal{T}_1 $ và $ \mathcal{T}_2 $ so sánh được, thì chúng trùng nhau.*

#### Hệ quả 3 {#evt-i-s3-lem-2-cor-3 .statement}

*Cho E và F là hai không gian vectơ đầy đủ mêtric hóa được trên một vành chia được định giá không rời rạc. Để một ánh xạ tuyến tính liên tục u từ E vào F là một cấu xạ ngặt, điều kiện cần và đủ là $ u(E) $ đóng trong F.*

Điều kiện là cần, vì nếu $ u $ là một cấu xạ ngặt, thì ảnh $ u(E) $, do đẳng cấu với thương $ E/u^{-1}(0) $, là đầy đủ (I, p. 17) và do đó đóng trong F. Điều kiện là đủ, vì nếu $ u(E) $ đóng trong F, thì $ u(E) $ phải là một không gian vectơ đầy đủ mêtric hóa được và do đó theo định lý 1, $ u $ là một cấu xạ ngặt từ E lên $ u(E) $.

#### Hệ quả 4 {#evt-i-s3-lem-2-cor-4 .statement}

*Cho E là một không gian vectơ đầy đủ mêtric hóa được trên một vành chia được định giá không rời rạc. Nếu M và N là hai không gian con vectơ đóng, là các phần bù (đại số) của nhau trong E, thì E là tổng trực tiếp tôpô của M và N.*

Thật vậy, $ M \times N $ là một không gian vectơ đầy đủ mêtric hóa được và ánh xạ $ (y, z) \mapsto y + z $ từ $ M \times N $ lên E là liên tục và song ánh, do đó là một đẳng cấu (hệ quả 1).

#### Hệ quả 5 (Định lý đồ thị đóng) {#evt-i-s3-lem-2-cor-5 .statement}

— *Cho E và F là hai không gian vectơ mêtric hoá được đầy đủ trên một thể chia có giá trị không rời rạc. Để một ánh xạ tuyến tính u từ E vào F liên tục, điều kiện cần và đủ là đồ thị của nó, trong không gian tích $ E \times F $, là đóng.*

Điều kiện đó là cần thiết vì đồ thị của một ánh xạ liên tục vào một không gian Hausdorff là đóng (GT, I, § 8.1, hệ quả 2). Để thấy rằng nó là đủ, hãy chú ý rằng nó kéo theo đồ thị G của $ u $, là một không gian con vectơ đóng của không gian mêtric hoá được đầy đủ $ E \times F $, tự nó cũng mêtric hoá được và đầy đủ. Phép chiếu $ z \mapsto \mathrm{pr}_1(z) $ của G lên E là một ánh xạ tuyến tính liên tục, song ánh, do đó là một đẳng cấu (hệ quả 1); vì ánh xạ nghịch đảo của nó là $ x \mapsto (x, u(x)) $, suy ra $ u $ là liên tục trong E.

Ta có thể phát biểu hệ quả này dưới dạng sau: $ u $ là liên tục nếu tình huống sau xảy ra: nếu dãy $ (x_n) $ các điểm của E vừa hội tụ về 0 vừa *có tính chất là dãy* $ (u(x_n)) $ *hội tụ về* $ y $, thì tất yếu phải có $ y = 0 $.

#### Ví dụ {#evt-i-s3-n3-exa-1 .statement}

— Cho E là một không gian con vectơ của không gian các hàm thực xác định trên $ I = [0, 1] $; gọi $ \| f \| $ là một chuẩn trên E, theo đó E là *đầy đủ*, và sao cho tôpô của nó mịn hơn tôpô hội tụ đơn. Giả sử thêm rằng E chứa tập hợp $ \mathcal{C}^\infty(I) $ các hàm khả vi vô hạn trên I; ta sẽ chỉ ra rằng tồn tại một số nguyên $ k \geq 0 $, sao cho E chứa tập hợp $ \mathcal{C}^k(I) $ gồm tất cả các hàm có đạo hàm bậc $ k $ liên tục trên I.

Với mọi cặp số nguyên $ m > 0,\ n \geq 0 $, gọi $ V_{mn} $ là tập hợp các hàm $ f \in \mathcal{C}^\infty(I) $ sao cho $ |f^{(h)}(x)| \leq 1/m $ với $ 0 \leq h \leq n $ và với mọi $ x \in I $. Các $ V_{m,n} $ tạo thành một hệ cơ bản các lân cận của 0 đối với một tôpô khả mêtric tương thích với cấu trúc không gian vectơ của $ \mathcal{C}^\infty(I) $, hơn nữa $ \mathcal{C}^\infty(I) $ là *đầy đủ* trong tôpô này (FVR, II, p. 2, định lý 1). Gọi $ u $ là ánh xạ chính tắc từ $ \mathcal{C}^\infty(I) $ vào E; ta sẽ chỉ ra rằng $ u $ là *liên tục*. Theo hệ quả 5 ở trên, chỉ cần chứng minh rằng nếu một dãy $ (f_n) $ hội tụ về 0 trong $ \mathcal{C}^\infty(I) $ và hội tụ đến một giới hạn $ f $ trong E thì tất yếu $ f = 0 $. Nhưng điều này là ngay lập tức vì, theo giả thiết, $ f $ là giới hạn theo hội tụ đơn của $ (f_n) $. Do đó tồn tại một số nguyên $ k \geq 0 $ và một số $ a > 0 $ sao cho quan hệ

$$
p_k(f) = \sup_{\substack{x \in I \\ 0 \leq h \leq k}} |f^{(h)}(x)| \leq a
$$

hàm ý $ \| f \| \leq 1 $ với mọi $ f \in \mathcal{C}^\infty(I) $.

Nhưng $ p_k $ là một chuẩn trên không gian $ \mathcal{C}^k(I) $ và $ \mathcal{C}^\infty(I) $ là một không gian con trù mật khắp nơi trong $ \mathcal{C}^k(I) $ đối với chuẩn này (tập hợp các đa thức đã là trù mật khắp nơi trong $ \mathcal{C}^k(I) $, một hệ quả ngay lập tức của định lý Weierstrass-Stone). Theo điều đã nói trước, ánh xạ đồng nhất của $ \mathcal{C}^\infty(I) $ (mang chuẩn $ p_k $) vào E là liên tục, và vì vậy nó có thể được mở rộng một cách liên tục ra toàn bộ không gian $ \mathcal{C}^k(I) $ (vì E là đầy đủ). Điều này chứng minh mệnh đề của chúng ta.

#### Mệnh đề 1 {#evt-i-s3-prop-1 .statement}

*Cho E, F là hai không gian vectơ tôpô trên một thể chia định chuẩn không rời rạc K. Giả sử rằng :*

1) E *là mêtric hóa được và đầy đủ*.
2) *Tồn tại một dãy* $ (F_n) $ *các không gian vectơ mêtric hóa được đầy đủ trên K và, với mỗi n, một ánh xạ tuyến tính đơn ánh liên tục* $ v_n $ *từ* $ F_n $ *vào F sao cho F là hợp của các không gian con* $ v_n(F_n) $.

*Bây giờ cho u là một ánh xạ tuyến tính của E vào F. Nếu đồ thị của u đóng trong* $ E \times F $, *thì tồn tại một số nguyên n và một ánh xạ tuyến tính liên tục* $ u_n $ *của E vào* $ F_n $ *sao cho* $ u = v_n \circ u_n $ *(điều này kéo theo rằng u liên tục và* $ u(E) \subset v_n(F_n) $).*

Cho G là đồ thị của $ u $ trong $ E \times F $. Với mọi $ n $, ta xét ánh xạ tuyến tính liên tục $ w_n : (x, y) \mapsto (x, v_n(y)) $ từ $ E \times F_n $ vào $ E \times F $; vì G đóng, tập $ w_n^{-1}(G) = G_n $ là một không gian con vectơ đóng của $ E \times F_n $; nếu $ p_n $ là hạn chế lên $ G_n $ của phép chiếu thứ nhất $ \mathrm{pr}_1 $, ta có $ p_n(G_n) = u^{-1}(v_n(F_n)) $. Vì $ p_n $ liên tục và $ G_n $ đầy đủ (do $ G_n $ đóng trong không gian đầy đủ $ E \times F_n $), theo định lý 1, $ p_n(G_n) $ hoặc là gầy trong E hoặc là toàn bộ E. Nhưng, theo giả thiết, E là hợp của các $ p_n(G_n) $, và vì E đầy đủ, các $ p_n(G_n) $ không thể đều gầy trong E theo định lý Baire (GT, IX, § 5.3, đl. 1). Do đó tồn tại một số nguyên n sao cho $ p_n(G_n) = E $, hay nói cách khác $ u(E) \subset v_n(F_n) $. Hơn nữa, vì $ v_n $ đơn ánh, $ G_n $ là đồ thị của một ánh xạ tuyến tính $ u_n $ từ E vào $ F_n $, và theo định lý đồ thị đóng (I, p. 19, hq. 5) $ u_n $ là *liên tục*; khi đó từ các định nghĩa suy ra rằng $ u = v_n \circ u_n $.

Bài tập

### Bài tập {#evt-i-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
