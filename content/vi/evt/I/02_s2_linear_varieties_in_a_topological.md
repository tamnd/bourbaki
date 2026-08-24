---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 2
section_title: Linear varieties in a topological vector space
lang: vi
source: evt-i-v
book_pages: TVS I.11-TVS I.16, TVS I.25-TVS I.28
pdf_pages: 0019-0024, 0033-0036
extraction: ocr
subsections:
    - "no": 1
      title: The closure of a linear variety
      page: 11
      pdf_page: 19
    - "no": 2
      title: Lines and closed hyperplanes
      page: 12
      pdf_page: 20
    - "no": 3
      title: Vector subspaces of finite dimension
      page: 13
      pdf_page: 21
    - "no": 4
      title: Locally compact topological vector spaces
      page: 15
      pdf_page: 23
statements: 24
exercises: 12
content_sha256: 4a01164f9def0ff965bb91e58ee0e8a829b8b5dae71836ed3349d4562ac15c71
translated_from: content/en/evt/I/02_s2_linear_varieties_in_a_topological.md
source_content_sha256: c12495ea5aa70c96ec454e4334e835094b5959ce7044f945255ffd99a6e833e3
translation_model: gpt-5.4
translation_run: translate-vi-41cdad82
glossary_version: 34
glossary_terms_sha256: 2ede0ceebec65bcf1af7532ef812dafce547390273ef7bbb6bfa2703b551db76
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC ĐA TẠP TUYẾN TÍNH TRONG MỘT KHÔNG GIAN VECTƠ TÔPÔ

### 1. Bao đóng của một đa tạp tuyến tính

Nhắc lại (A, II, § 9.3) rằng trong một không gian vectơ $ E $ trên một vành chia $ K $, một đa tạp tuyến tính afin không rỗng (gọi là « đa tạp tuyến tính » khi điều đó không thể gây nhầm lẫn) là ảnh qua một phép tịnh tiến của một không gian con vectơ của $ E $.

#### Mệnh đề 1 {#evt-i-s2-prop-1 .statement}

— *Trong một không gian vectơ tôpô $ E $, bao đóng của một đa tạp tuyến tính là một đa tạp tuyến tính.*

Vì mọi phép tịnh tiến đều là một đồng phôi của $ E $, chỉ cần chứng minh mệnh đề cho một không gian con vectơ $ M $ của $ E $, và trong trường hợp này, mệnh đề đã được chứng minh ở I, p. 4.

#### Hệ quả {#evt-i-s2-n1-cor-1 .statement}

— *Trong một không gian vectơ tôpô $ E $, mọi siêu phẳng hoặc là đóng hoặc là trù mật khắp nơi.*

Thật vậy, bao đóng của một siêu phẳng thuần nhất $ H $ chỉ có thể là $ H $ hoặc toàn bộ không gian $ E $, vì đó là một không gian con vectơ chứa $ H $ (mệnh đề 1).

Một siêu phẳng $ H $ là *đóng* trong $ E $ khi và chỉ khi $ \complement H $ chứa một điểm trong.

Không gian con vectơ $ M $ sinh bởi một tập hợp $ A $, trong một không gian vectơ tôpô $ E $, là tập hợp các tổ hợp tuyến tính của các điểm của $ A $ (A, II, § 1.7, mệnh đề 9); bao đóng của $ M $ trong $ E $ theo mệnh đề 1 là không gian con vectơ đóng nhỏ nhất chứa $ A $; ta nói rằng đó là *không gian con vectơ đóng sinh bởi* $ A $.

#### Định nghĩa 1 {#evt-i-s2-def-1 .statement}

— *Một tập hợp $ A $, trong một không gian vectơ tôpô $ E $, là toàn phần nếu và chỉ nếu không gian con vectơ đóng sinh bởi $ A $ trùng với $ E $* (nghĩa là tập hợp các tổ hợp tuyến tính của các phần tử của $ A $ là *trù mật khắp nơi*).

#### Ví dụ {#evt-i-s2-n1-exa-1 .statement}

— 1) Trong không gian định chuẩn $ \mathscr{C}(I; \mathbf{C}) $ (trên trường $ \mathbf{C} $) của các hàm liên tục trên $ I = \{0, 1\} $, nhận giá trị trong $ \mathbf{C} $, các hạn chế trên $ I $ của các hàm $ x^n \ (n \in \mathbf{N}) $ tạo thành một tập toàn phần, theo định lý Weierstrass-Stone (GT, X, § 4.2, đl. 3). Tương tự, các hạn chế trên $ I $ của các hàm $ e^{2n\pi ix} \ (n \in \mathbf{Z}) $ tạo thành một tập toàn phần (GT, X, § 4.4, mđ. 8), trong không gian con $ P $ của $ \mathscr{C}(I, \mathbf{C}) $ gồm các hàm sao cho $ f(0) = f(1) $.

2) Mọi tập hợp hấp thụ trong một không gian vectơ tôpô $ E $ trên một vành chia định giá không-rời-rạc (và đặc biệt mọi lân cận của 0 trong $ E $) đều là một tập hợp toàn phần vì nó sinh ra $ E $ (I, p. 7). Do đó một đa tạp tuyến tính không trù mật trong $ E $ tất yếu là một tập hợp thưa đâu cũng được trong $ E $ (GT, IX, § 5.1) vì bao đóng của nó không thể chứa một điểm trong.

#### Định nghĩa 2 {#evt-i-s2-def-2 .statement}

— *Một họ $ (a_i)_{i \in I} $ các điểm của một không gian vectơ tôpô $ E $ được gọi là độc lập tôpô nếu với mọi $ \kappa \in I $, không gian con vectơ đóng sinh bởi các $ a_i $, với $ i \neq \kappa $, không chứa $ a_\kappa $.*

#### Ví dụ {#evt-i-s2-n1-exa-2 .statement}

— 3) Trong không gian định chuẩn $ \mathcal{C}(I; \mathbf{C}) $ của các hàm liên tục xác định trên $ I = \{0, 1\} $, các hạn chế lên I của các hàm $ e^{2n\pi i x} $ ($ n \in \mathbf{Z} $) tạo thành một họ độc lập tôpô. Nếu $ f(x) $ là tổ hợp tuyến tính $ \sum_{k \neq n} c_k e^{2k\pi i x} $ (trong đó mọi $ c_k $ trừ một số hữu hạn đều bằng không) thì
$$
\int_0^1 |e^{2n\pi i x} - f(x)|^2 \, dx = 1 + \sum_{k \neq n} |c_k|^2 \geq 1
$$
và, *a fortiori*, theo định lý giá trị trung bình
$$
\sup_{x \in I} |e^{2n\pi i x} - f(x)| \geq 1
$$
điều này cho thấy rằng $ e^{2\pi i n x} $ không thuộc không gian con vectơ đóng của $ \mathcal{C}(I; \mathbf{C}) $ được sinh bởi $ e^{2k\pi i x}, \ k \neq n $.

Tập hợp các phần tử của một họ độc lập tôpô được gọi là một *tập độc lập tôpô* của E. Mọi tập con của một tập con độc lập tôpô đều độc lập tôpô; mọi tập con chỉ gồm một điểm $ x \neq 0 $ đều độc lập tôpô nếu E là một không gian Hausdorff.

Một họ độc lập tôpô thì độc lập (theo nghĩa đại số; *xem* A, II, § 7.1, *Nhận xét*), nhưng mệnh đề đảo lại là sai.

#### Ví dụ {#evt-i-s2-n1-exa-3 .statement}

— 4) Trong không gian chuẩn $ \mathcal{C}(I; \mathbf{C}) $ của các hàm liên tục trên $ I = \{0, 1\} $, các hạn chế lên I của các hàm $ x^n $ ($ n \in \mathbf{N} $) tạo thành một họ độc lập đại số. Nhưng tồn tại một dãy các đa thức $ (p_n) $ sao cho $ p_n(x^2) $ hội tụ đều đến $ x $ trên I (GT, X, § 4.2, bổ đề 2), điều này cho thấy rằng $ x $ thuộc không gian con vectơ đóng của $ \mathcal{C}(I; \mathbf{C}) $ được sinh bởi các hàm $ x^{2n} $ ($ n \in \mathbf{N} $).

#### Nhận xét {#evt-i-s2-n1-rem-1 .statement}

— 1) Họ các tập hợp độc lập tôpô của một không gian vectơ tôpô *không nhất thiết có tính quy nạp* đối với quan hệ bao hàm (I, p. 25, exerc. 2); do đó tình huống này khác với tình huống của các tập hợp độc lập đại số. Hơn nữa, không nhất thiết tồn tại trong E một tập con độc lập tôpô cực đại (I, p. 25, exerc. 4), do đó không nhất thiết tồn tại một tập con vừa *trù mật* vừa độc lập tôpô.

2) Cho M là một không gian con vectơ đóng của E và $ (\dot{a}_i)_{i \in I} $ là một họ độc lập tôpô trong không gian thương E/M. Nếu $ a_i $ là một phần tử bất kỳ của lớp $ \dot{a}_i $, thì từ định nghĩa 2, và từ sự kiện rằng ánh xạ chính tắc của E lên E/M là liên tục, suy ra rằng họ $ (a_i)_{i \in I} $ là độc lập tôpô. Nhưng chú ý rằng nếu N là không gian con vectơ *đóng* được sinh bởi các $ a_i $ thì có thể xảy ra $ M \cap N \neq \{0\} $ (I, p. 25, exerc. 2), và do đó tổng $ M + N $ không nhất thiết là trực tiếp theo nghĩa đại số (cũng không, *a fortiori*, theo nghĩa tôpô).

### 2. Đường thẳng và siêu phẳng đóng

Mệnh đề 2. — *Mọi không gian vectơ tôpô Hausdorff* E *có chiều* 1 *trên một thể phân chia định giá không rời rạc* K *đều đẳng cấu với* $ K_s $; *thực vậy, với mọi* $ a \neq 0 $ *trong* E, *ánh xạ* $ \xi \mapsto \xi a $ *của* $ K_s $ *lên* E *là một đẳng cấu* (nói cách khác mọi ánh xạ tuyến tính của* $ K_s $ *lên* E *đều là một đẳng cấu*).

Vì ánh xạ $ \xi \mapsto \xi a $ từ $ K_s $ lên E là song ánh và liên tục (I, p. 1, def. 1), chỉ cần chứng minh rằng nó là song liên tục. Cho $ \alpha $ là một số thực $ > 0 $, ta chứng minh rằng tồn tại một lân cận V của 0 trong E sao cho nếu $ \xi a \in V $ thì $ |\xi| < \alpha $. Vì K không rời rạc, tồn tại một phần tử $ \xi_0 \in K $ sao cho $ 0 < |\xi_0| < \alpha $; nhưng vì E là Hausdorff, có một lân cận V của 0 sao cho $ \xi_0 a $ không thuộc V. Ta có thể giả sử rằng V là cân bằng (I, p. 7, prop. 4). Khi đó, nếu $ \xi a \in V $ và $ |\xi| \geq |\xi_0| $ thì ta có $ |\xi_0 \xi^{-1}| \leq 1 $, và $ \xi_0 a = (\xi_0 \xi^{-1}) (\xi a) \in V $; vì mệnh đề sau cùng này là sai, ta thấy rằng $ \xi a \in V $ suy ra $ |\xi| < |\xi_0| < \alpha $. Điều này hoàn thành chứng minh.

#### Hệ quả 1 {#evt-i-s2-def-2-cor-1 .statement}

*Trong một không gian vectơ tôpô Hausdorff E, trên một vành chia có định giá không rời rạc K, mọi không gian con vectơ D có chiều 1 đều đẳng cấu với $ K_s $.*

#### Hệ quả 2 {#evt-i-s2-def-2-cor-2 .statement}

*Một không gian vectơ tôpô E trên một vành chia có định giá không rời rạc. Mọi không gian con vectơ D (có chiều 1) là phần bù đại số của một siêu phẳng thuần nhất đóng H cũng là phần bù tôpô của H.*

Trong D, tập $ \{0\} $ là đóng, vì nó là giao của D và tập đóng H; do đó D là Hausdorff. Nhưng vì E/H cũng Hausdorff, ánh xạ chính tắc của D lên E/H, vốn tuyến tính, cũng là một đẳng cấu theo mệnh đề 2, từ đó suy ra kết luận (GT, III, § 6.2).

#### Định lý 1 {#evt-i-s2-thm-1 .statement}

*Một không gian vectơ tôpô E trên một vành chia có định giá không rời rạc. Gọi H là một siêu phẳng trong E được xác định bởi phương trình $ f(x) = \alpha $ trong đó f là một dạng tuyến tính không đồng nhất bằng không. Khi đó H đóng trong E nếu và chỉ nếu f liên tục.*

Điều kiện ấy hiển nhiên là đủ (GT, I, § 2.1, định lý 1); ta chứng minh rằng nó là cần. Ta có thể giả sử rằng H là một siêu phẳng thuần nhất đóng có phương trình $ f(x) = 0 $. Khi đó không gian thương E/H là một không gian vectơ tôpô Hausdorff chiều 1 trên K. Ta có thể viết $ f = g \circ \phi $, trong đó $ \phi $ là ánh xạ chính tắc của E lên E/H và g là một ánh xạ tuyến tính từ E/H lên $ K_s $; theo mệnh đề 2, g liên tục, do đó f cũng vậy.

#### Hệ quả {#evt-i-s2-n2-cor-1 .statement}

*Mọi dạng tuyến tính liên tục trên E không đồng nhất bằng không đều là một cấu xạ ngặt từ E lên $ K_s $.*

#### Nhận xét {#evt-i-s2-n2-rem-1 .statement}

— Có những ví dụ về các không gian vectơ tôpô định chuẩn trên một vành chia có định giá không rời rạc đầy đủ, trong đó mọi dạng tuyến tính liên tục đều đồng nhất bằng không (I, p. 25, exerc. 4); do đó, trong một không gian như vậy, mọi siêu phẳng đều trù mật khắp nơi (I, p. 11, hệ quả).

### 3. Các không gian con vectơ có số chiều hữu hạn

#### Định lý 2 {#evt-i-s2-thm-2 .statement}

*Mọi không gian vectơ tôpô Hausdorff E, có số chiều hữu hạn n, trên một vành chia có định giá không rời rạc đầy đủ K, đều đẳng cấu với $ K_s^n $; thực vậy, với mọi cơ sở $ (e_i)_{1 \leq i \leq n} $ của E trên K, ánh xạ tuyến tính $ (\xi_i) \mapsto \sum_{i=1}^n \xi_i e_i $ là một đẳng cấu từ $ K_s^n $ lên E.*

Mệnh đề 2 của I, p. 12, suy ra rằng đl. 2 là đúng đối với $ n = 1 $; ta lập luận bằng quy nạp theo $ n $. Gọi $ H $ là không gian con vectơ của $ E $ sinh bởi $ e_1, e_2, ..., e_{n-1} $; giả thiết quy nạp là ánh xạ $ (\xi_i)_{1 \leq i \leq n-1} \mapsto \sum_{i=1}^{n-1} \xi_i e_i $ là một đẳng cấu của $ K_s^{n-1} $ lên $ H $. Không gian con $ H $, do đẳng cấu với một tích các không gian đầy đủ, nên là đầy đủ (GT, II, § 3.5, prop. 10); do đó nó *đóng* trong $ E $ (GT, II, § 3.4, prop. 8). Gọi $ D $ là không gian con $ Ke_n $ bù của $ H $ trong $ E $; $ E $ là tổng trực tiếp tôpô của $ H $ và $ D $ (I, p. 13, cor. 2), do đó ánh xạ

$$
(\xi_i)_{1 \leq i \leq n} \mapsto \sum_{i=1}^n \xi_i e_i
$$

của $ K_s^{n-1} \times K_s $ lên $ E $ là một đẳng cấu.

Khi $ n > 1 $ thì giả thiết $ K $ là *đầy đủ* là cốt yếu để định lý 2 đúng. Thật vậy, cho $ K $ là một vành chia được định giá không đầy đủ, và $ \hat{K} $ là hoàn thành của nó: với mỗi $ a \neq 0 $ của $ \hat{K} $ thì tập hợp $ K.a $ trù mật khắp nơi trong $ \hat{K} $, vì $ x \mapsto xa $ là một đồng phôi của $ \hat{K} $ lên chính nó. Nếu $ a \notin K $, không gian con $ K + Ka $ của không gian vectơ tôpô $ \hat{K} $ trên $ K $ có chiều 2 trên $ K $, nhưng nó không đẳng cấu với $ K_s^2 $ vì mọi không gian con chiều 1 trong $ K + Ka $ đều trù mật trong $ K + Ka $.

#### Hệ quả 1 {#evt-i-s2-thm-2-cor-1 .statement}

*Trong một không gian vectơ tôpô Hausdorff $ E $ trên một vành chia định giá đầy đủ không rời rạc $ K $, mọi không gian con vectơ $ F $ có số chiều hữu hạn đều đóng trong $ E $.* Thật vậy, nếu $ F $ có chiều $ n $ thì nó đẳng cấu với $ K_s^n $; do đó nó đầy đủ và vì thế đóng trong $ E $ (GT, II, § 3.4, prop. 8).

#### Hệ quả 2 {#evt-i-s2-thm-2-cor-2 .statement}

*Cho $ K $ là một vành chia định giá đầy đủ không rời rạc, và $ E $ là một không gian vectơ tôpô Hausdorff có số chiều hữu hạn trên $ K $. Nếu $ F $ là một không gian vectơ tôpô bất kỳ trên $ K $, thì mọi ánh xạ tuyến tính từ $ E $ vào $ F $ đều liên tục.*

#### Hệ quả 3 {#evt-i-s2-thm-2-cor-3 .statement}

*Trong một không gian vectơ tôpô Hausdorff $ E $, trên một vành chia được định giá đầy đủ không rời rạc, mọi tập hợp độc lập hữu hạn đều độc lập tôpô.*

#### Hệ quả 4 {#evt-i-s2-thm-2-cor-4 .statement}

*Cho $ E $ là một không gian vectơ tôpô trên một vành chia được định giá đầy đủ không rời rạc. Nếu $ M $ là một không gian con vectơ đóng của $ E $ và $ F $ là một không gian con vectơ của $ E $ có số chiều hữu hạn, thì không gian con $ M + F $ là đóng trong $ E $. Ký hiệu $ \phi $ là đồng cấu chính tắc từ $ E $ lên không gian thương $ E/M $ (tất nhiên là Hausdorff). Khi đó không gian con $ M + F $ trùng với $ \overline{\phi}^{-1}(\phi(F)) $. Bây giờ $ \phi(F) $ có số chiều hữu hạn trong $ E/M $, vì vậy (hệ quả 1) $ \phi(F) $ là đóng trong $ E/M $, và, hệ quả là, $ \overline{\phi}^{-1}(\phi(F)) $ là đóng trong $ E $.*

Ta chú ý rằng, nếu $ M $ và $ N $ là hai không gian con vectơ đóng bất kỳ trong một không gian vectơ tôpô Hausdorff $ E $, thì $ M + N $ không nhất thiết đóng trong $ E $, \* ngay cả khi $ E $ là một không gian Hilbert \* (xem IV, p. 64, exerc. 13, d)).

#### Mệnh đề 3 {#evt-i-s2-prop-3 .statement}

*Cho $ E $ là một không gian vectơ tôpô trên một thân chia định giá đầy đủ không rời rạc* $ K $. Cho $ M $ là một không gian con vectơ đóng có đối chiều hữu hạn $ n $ trong $ E $. Khi đó mọi không gian con $ N $ là một phần bù đại số của $ M $ trong $ E $ cũng là một phần bù tôpô.

Trong $ N $, tập hợp $ \{0\} $ là đóng, vì nó là giao của $ N $ và tập hợp $ M $ đóng trong $ E $; do đó $ N $ là Hausdorff. Vì $ E/M $ cũng là Hausdorff, ánh xạ chính tắc của $ N $ lên $ E/M $, vốn tuyến tính và song ánh, là song liên tục (I, p. 14, hệ quả 2), từ đó suy ra mệnh đề.

#### Hệ quả {#evt-i-s2-n3-cor-1 .statement}

*Cho $ E $ và $ F $ là hai không gian vectơ tôpô trên một thể có giá đầy đủ không rời rạc. Nếu $ F $ là Hausdorff và có số chiều hữu hạn, thì mọi ánh xạ tuyến tính liên tục của $ E $ lên $ F $ đều là một cấu xạ ngặt.*

#### Nhận xét {#evt-i-s2-n3-rem-1 .statement}

— Các kết quả của Số 2, 3 không còn đúng nữa khi $ K $ là *rời rạc*. Chẳng hạn, cho $ K_1 $ là một vành chia định giá không rời rạc và $ K $ là vành chia rời rạc thu được bằng cách trang bị cho $ K_1 $ giá trị tuyệt đối tầm thường trên $ K_1 $. Khi đó $ K_1 $ là một không gian vectơ tôpô chiều 1 trên $ K $, nhưng nó không đẳng cấu với $ K_s $. Tuy nhiên, ta có thể chứng minh rằng các kết quả của Số 2, 3 vẫn đúng ngay cả khi $ K $ là rời rạc, với điều kiện ta áp đặt lên các không gian vectơ tôpô đang xét tính chất có một hệ cơ bản các lân cận *cân bằng* của 0 (nghĩa là các lân cận $ V $ sao cho $ K.V = V $) (I, p. 27, bài tập 14); điều kiện này (vốn luôn được thỏa mãn khi $ K $ là một vành chia định giá không rời rạc, *x.* I, p. 7, mệnh đề 4) không đúng đối với mọi không gian vectơ tôpô trên $ K $, như ví dụ trước cho thấy.

### 4. Các không gian vectơ tôpô compact địa phương

#### Định lý 3 {#evt-i-s2-thm-3 .statement}

*Cho $ K $ là một vành chia định giá đầy đủ không rời rạc. Nếu $ E $ là một không gian vectơ tôpô Hausdorff trên $ K $, sao cho một lân cận nào đó $ V $ của 0 trong $ E $ là tiền compact, thì $ E $ có số chiều hữu hạn. Nếu $ E \neq \{0\} $, thì cả $ K $ lẫn $ E $ đều compact địa phương.*

Trong việc chứng minh mệnh đề thứ nhất, ta chỉ cần xét trường hợp $ E $ là *đầy đủ*; vì $ E $ là một không gian con trù mật của hoàn bị của nó $ \hat{E} $, và bao đóng $ \overline{V} $ của $ V $ trong $ \hat{E} $ là compact và là một lân cận của 0 trong $ \hat{E} $ (GT, III, § 3.4, prop. 7).

Vậy ta có thể giả sử rằng tồn tại một lân cận *compact* $ V $ của 0 trong $ E $. Lấy $ \alpha \in K $ sao cho $ 0 < |\alpha| < 1 $; khi đó có hữu hạn điểm $ a_i \in V $ sao cho

$$
V \subset \bigcup_i (a_i + \alpha V).
$$

Cho $ M $ là không gian con hữu hạn chiều của $ E $ sinh bởi các $ a_i $; nó đóng trong $ E $ (I, p. 14, cor. 1). Trong không gian vectơ tôpô Hausdorff $ E/M $, ảnh chính tắc của $ V $ là một lân cận compắc $ W $ của 0, sao cho $ W \subset \alpha W $; do đó $ \alpha^{-1} W \subset W $, và, bằng quy nạp theo $ n $, $ \alpha^{-n} W \subset W $ với mọi số nguyên dương $ n $. Vì $ W $ là hút, chúng ta kết luận rằng $ W = E/M $; và do đó $ E/M $ là *compắc*. Vì vậy, để hoàn thành chứng minh mệnh đề đầu tiên trong định lý, chỉ cần chứng minh bổ đề sau đây.

#### Bổ đề 1 {#evt-i-s2-lem-1 .statement}

— *Mọi không gian vectơ tôpô compắc $ E $ trên một thể chia định giá không rời rạc đều chỉ là tập hợp $ \{0\} $.*

Vì E là đầy đủ nên có thể giả sử K là đầy đủ (I, p. 6). Nếu E $ \neq \{0\} $ thì E chứa một đường thẳng đóng trong E (I, p. 14, hệ quả 1) và do đó compắc. Đường thẳng này đẳng cấu với $ K_s $ (I, p. 12, mệnh đề 2) và vì thế K phải compắc. Bây giờ ánh xạ $ \xi \mapsto |\xi| $ từ K vào $ \mathbf{R} $ là liên tục và vì vậy ảnh của K phải bị chặn; mặt khác tồn tại $ \gamma \in K $ sao cho $ |\gamma| > 1 $, và tập hợp $ |\gamma^n| = |\gamma|^n, n \in \mathbf{N} $, là không bị chặn. Mâu thuẫn này chứng tỏ rằng $ E = \{0\} $.

Để chứng minh mệnh đề thứ hai của định lý, nếu $ E \neq \{0\} $ thì theo phần thứ nhất của định lý, E đẳng cấu với $ K_s^n $ với $ n > 0 $; bây giờ K là đầy đủ, nên E cũng vậy, và do đó E là địa phương compắc. Nhưng $ K_s $ đẳng cấu với một đường thẳng trong E (I, p. 12, mệnh đề 2), đường thẳng này tất yếu đóng trong E (I, p. 14, hệ quả 1); suy ra K là địa phương compắc.

#### Nhận xét {#evt-i-s2-n4-rem-1 .statement}

— Kết quả của đl. 3 không còn đúng nữa nếu K là một vành chia rời rạc, như được chỉ ra bởi ví dụ $ \mathbf{R} $ (với tôpô thông thường) được xét như một không gian vectơ tôpô trên trường rời rạc $ \mathbf{Q} $.

### Bài tập {#evt-i-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
