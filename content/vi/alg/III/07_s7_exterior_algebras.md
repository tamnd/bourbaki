---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 7
section_title: Exterior algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0531-0546, 0657-0661
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE EXTERIOR ALGEBRA OF A MODULE
      page: 0
      pdf_page: 531
    - "no": 2
      title: Functorial properties of the exterior algebra
      page: 0
      pdf_page: 532
    - "no": 3
      title: ANTICOMMUTATIVITY OF THE EXTERIOR ALGEBRA
      page: 0
      pdf_page: 534
    - "no": 4
      title: '*n*-th EXTERIOR POWER OF A MODULE AND ALTERNATING MULTILINEAR MAPPINGS'
      page: 0
      pdf_page: 535
    - "no": 5
      title: EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 537
    - "no": 6
      title: DIRECT LIMITS OF EXTERIOR ALGEBRAS
      page: 0
      pdf_page: 538
    - "no": 7
      title: EXTERIOR ALGEBRA OF A DIRECT SUM. EXTERIOR ALGEBRA OF A GRADED MODULE
      page: 0
      pdf_page: 539
    - "no": 8
      title: EXTERIOR ALGEBRA OF A FREE MODULE
      page: 0
      pdf_page: 541
    - "no": 9
      title: CRITERIA FOR LINEAR INDEPENDENCE
      page: 0
      pdf_page: 543
statements: 31
exercises: 15
content_sha256: 337759b3d5363282eaa7cb42891fab1bf80413cd754594cc0d72d0291f135d74
translated_from: content/en/alg/III/07_s7_exterior_algebras.md
source_content_sha256: cbe5ec3c1d32b8ff814eadc31480406f3c983dc3cf510530feed48e0dcec19d0
translation_model: gpt-5-6-mini
translation_run: translate-vi-ad8b440c
glossary_version: 34
glossary_terms_sha256: 9f1e10c30a591b7118cb2afe31617ed956382a0f8f1494a43de7f075949362e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐẠI SỐ NGOÀI

### 1. ĐỊNH NGHĨA CỦA ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN

#### Định nghĩa 1 {#alg-iii-s7-def-1 .statement}

Cho $ A $ là một vành giao hoán và $ M $ là một $ A $-môđun. Đại số ngoài của $ M $, được ký hiệu bởi $ \bigwedge(M) $ hoặc $ \mathrm{Alt}(M) $ hoặc $ \bigwedge_A(M) $, là đại số trên $ A $ là thương của đại số tenxơ $ T(M) $ theo iđêan hai phía $ \mathfrak{J}'' $ (cũng được ký hiệu bởi $ \mathfrak{J}_{M}'' $) sinh bởi các phần tử $ x \otimes x $, trong đó $ x $ chạy qua $ M $.

Vì iđêan $ \mathfrak{J}'' $ được sinh bởi các phần tử thuần nhất bậc 2, nên nó là một iđêan phân bậc (II, § 11, no. 3, Mệnh đề 2); ta viết $ \mathfrak{J}_n'' = \mathfrak{J}'' \cap T^n(M) $; đại số $ \bigwedge(M) $ do đó được phân bậc bởi phép phân bậc (được gọi là chính tắc) gồm các $ \bigwedge^n(M) = T^n(M)/\mathfrak{J}_n'' $. Khi đó $ \mathfrak{J}_0'' = \mathfrak{J}_1'' = \{0\} $ và do đó $ \bigwedge^0(M) $ được đồng nhất với $ A $ và $ \bigwedge^1(M) $ với $ T^1(M) = M $; trong phần tiếp theo ta sẽ luôn thực hiện các sự đồng nhất này và đơn ánh chính tắc $ M \to \bigwedge(M) $ sẽ được ký hiệu bởi $ \phi'' $ hoặc $ \phi_M'' $.

#### Mệnh đề 1 {#alg-iii-s7-prop-1 .statement}

Cho $ E $ là một $ A $-đại số và $ f : M \to E $ là một ánh xạ $ A $-tuyến tính sao cho
$$
(f(x))^2 = 0 \quad \text{với mọi } x \in M.
$$
Tồn tại một và chỉ một đồng cấu đại số $ g : \bigwedge(M) \to E $ sao cho $ f = g \circ \phi'' $.

Nói cách khác, $ (\bigwedge(M), \phi'') $ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1), trong đó $ \Sigma $ là loài của cấu trúc $ A $-đại số, các ánh xạ $ \alpha $ là các ánh xạ tuyến tính từ $ A $-môđun $ M $ đến một $ A $-đại số thỏa mãn (1).

Tính duy nhất của $ g $ suy ra từ sự kiện rằng $ \phi''(M) = M $ sinh $ \bigwedge(M) $. Để chứng minh sự tồn tại của $ g $, ta nhận xét rằng theo § 5, no. 1, Mệnh đề 1 tồn tại một đồng cấu đại số $ A $ $ g_1 : T(M) \to E $ sao cho $ f = g_1 \circ \phi $; ta cần chứng minh rằng $ g_1 $ bằng không trên iđêan $ \mathfrak{J}'' $, vì khi đó nếu
$$
p : T(M) \to \bigwedge(M) = T(M)/\mathfrak{J}''
$$
là đồng cấu chính tắc, ta có thể viết $ g_1 = g \circ p $, trong đó $ g : \bigwedge(M) \to E $ là một đồng cấu đại số và kết luận sẽ suy ra từ sự kiện rằng $ p \circ \phi = \phi'' $. Bây giờ, hạt nhân của $ g_1 $ là một iđêan hai phía mà, nhờ (1) và quan hệ $ g_1 \circ \phi = f $, chứa các phần tử $ x \otimes x $ với $ x \in M $. Điều này hoàn thành chứng minh.

#### Nhận xét {#alg-iii-s7-n1-rem-1 .statement}

(1) Giả sử rằng E là một đại số trên A phân bậc kiểu $ \mathbf{Z} $, với phép phân bậc $(E_n)$, và cũng giả sử rằng ánh xạ tuyến tính $ f $ (được giả thiết thỏa mãn (1)) sao cho
$$
f(M) \subset E_1.
$$
Khi đó quan hệ $ g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p) $ với các $ x_i \in M $ cho thấy rằng $ g(\bigwedge^p(M)) \subset E_p $ với mọi $ p \geq 0 $ và do đó $ g $ là một đồng cấu đại số phân bậc.

(2) Để tránh nhầm lẫn, tích của hai phần tử $ u, v $ của đại số ngoài $ \bigwedge(M) $ thường được ký hiệu bởi $ u \wedge v $ và được gọi là *tích ngoài* của $ u $ bởi $ v $. Do đó các phần tử của $ \bigwedge^n(M) $ là các tổng của các phần tử có dạng $ x_1 \wedge x_2 \wedge \cdots \wedge x_n $ với $ x_i \in M $ với $ 1 \leq i \leq n $ và thường được gọi là *n-vectơ*.

### 2. Các tính chất hàm tử của đại số ngoài

#### Mệnh đề 2 {#alg-iii-s7-prop-2 .statement}

*Cho $ A $ là một vành giao hoán, $ M $ và $ N $ là hai $ A $-môđun và $ u : M \to N $ là một ánh xạ $ A $-tuyến tính. Tồn tại một và chỉ một đồng cấu đại số trên $ A $*
$$
u'' : \bigwedge(M) \to \bigwedge(N)
$$
*thỏa mãn rằng biểu đồ*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M'' & & \downarrow \phi_N'' \\
\bigwedge(M) & \xrightarrow{u''} & \bigwedge(N)
\end{array}
$$

*là giao hoán. Hơn nữa, $ u'' $ là một đồng cấu đại số phân bậc.*

Sự tồn tại và tính duy nhất của $ u' $ suy ra từ no. 1, Mệnh đề 1 áp dụng cho đại số $ \bigwedge(N) $ và $ f = \phi_N'' \circ u : M \to \bigwedge(N) $; vì $ f(M) \subset N $ và do đó $ f $ thỏa mãn điều kiện (1) theo định nghĩa của $ \mathfrak{g}_N'' $: vì $ f(M) \subset \bigwedge^1(N) = N $, sự kiện rằng $ u'' $ là một đồng cấu đại số phân bậc suy ra từ *Nhận xét* 1 của no. 1.

Đồng cấu $ u'' $ của Mệnh đề 2 từ nay về sau sẽ được ký hiệu bởi $ \bigwedge(u) $. Nếu $ P $ là một $ A $-môđun và $ v : N \to P $ là một ánh xạ $ A $-tuyến tính, thì
$$
\bigwedge(v \circ u) = \bigwedge(v) \circ \bigwedge(u)
$$
vì $ \bigwedge(v) \circ \bigwedge(u) $ là một đồng cấu đại số làm cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{v \quad u} & P \\
\downarrow \phi_M' & & \downarrow \phi_P' \\
\bigwedge(M) & \xrightarrow{\bigwedge(v) \circ \bigwedge(u)} & \bigwedge(P)
\end{array}
$$

giao hoán.

Vì $ \Lambda(M) $ chứa $ M = \Lambda^1(M) $, $ \Lambda(u) $ đôi khi được gọi là mở rộng chính tắc của $ u $ lên $ \Lambda(M) $. Hạn chế $ \Lambda^n(u): \Lambda^n(M) \to \Lambda^n(N) $ là sao cho
$$
\Lambda^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
với các $ x_i \in M $, vì $ \Lambda(u) $ là một đồng cấu đại số và $ \Lambda^1(u) = u $; hạn chế $ \Lambda^0(u) $ lên $ A $ là ánh xạ đồng nhất. Chú ý rằng $ \Lambda^n(u) $ thu được từ $ T^n(u): T^n(M) \to T^n(N) $ bằng cách chuyển qua các thương.

#### Mệnh đề 3 {#alg-iii-s7-prop-3 .statement}

*Nếu $ u: M \to N $ là một ánh xạ tuyến tính $ A $-toàn ánh, đồng cấu $ \Lambda(u): \Lambda(M) \to \Lambda(N) $ là toàn ánh và hạt nhân của nó là iđêan hai phía của $ \Lambda(M) $ sinh bởi hạt nhân $ P \subset M \subset \Lambda(M) $ của $ u $.

Chứng minh được suy ra từ chứng minh của § 6, no. 2, Mệnh đề 4, thay $ S $ bởi $ \Lambda $ và $ \mathfrak{g}' $ bởi $ \mathfrak{g}'' $.

Nếu $ u: M \to N $ là một ánh xạ tuyến tính đơn ánh, không phải lúc nào cũng đúng rằng $ \Lambda(u) $ là một ánh xạ đơn ánh (\S 6, Bài tập 3) (tuy nhiên xem dưới đây no. 9, Hệ quả của Mệnh đề 12). Tuy nhiên điều này đúng khi $ u $ là một đơn ánh sao cho $ u(M) $ là một nhân tử trực tiếp của $ N $ và khi đó ảnh của $ \Lambda(u) $ (đẳng cấu với $ \Lambda(M) $) là một nhân tử trực tiếp của $ \Lambda(N) $; chứng minh cũng giống như chứng minh của các khẳng định tương tự đối với $ T(u) $ (\S 5, no. 2) thay $ T $ bởi $ \Lambda $.

#### Mệnh đề 4 {#alg-iii-s7-prop-4 .statement}

*Cho $ N $ và $ P $ là hai môđun con của một A-môđun $ M $ sao cho tổng của chúng $ N + P $ là một nhân tử trực tiếp trong $ M $ và giao của chúng $ N \cap P $ là một nhân tử trực tiếp trong $ N $ và trong $ P $. Khi đó các đồng cấu $ \Lambda(N) \to \Lambda(M) $, $ \Lambda(P) \to \Lambda(M) $ và $ \Lambda(N \cap P) \to \Lambda(M) $, các mở rộng chính tắc của các đơn ánh chính tắc, là đơn ánh; nếu $ \Lambda(N) $, $ \Lambda(P) $ và $ \Lambda(N \cap P) $ được đồng nhất với các đại số con của $ \Lambda(M) $ bằng các đồng cấu này, thì*
$$
\Lambda(N \cap P) = \Lambda(N) \cap \Lambda(P).
$$
Chứng minh được suy ra từ chứng minh của § 5, no. 2, Mệnh đề 4 thay $ T $ bởi $ \Lambda $ trong toàn bộ. Các giả thiết của Mệnh đề 4 luôn được thỏa mãn bởi các môđun con tùy ý $ N, P $ của $ M $ khi $ A $ là một trường.

#### Hệ quả {#alg-iii-s7-n2-cor-1 .statement}

*Cho $ K $ là một trường giao hoán và $ M $ là một không gian vectơ trên $ K $. Với mọi phần tử $ z \in \Lambda(M) $, tồn tại một không gian con vectơ nhỏ nhất $ N $ của $ M $ sao cho $ z \in \Lambda(N) $ và $ N $ là hữu hạn chiều.*

Chứng minh được suy ra từ chứng minh của § 5, no. 2, Hệ quả của Mệnh đề 4 thay $ T $ bởi $ \Lambda $ trong toàn bộ.

$ N $ được gọi là không gian con vectơ của $ M $ liên kết với phần tử $ z $ của $ \Lambda(M) $.

### 3. PHẢN GIAO HOÁ CỦA ĐẠI SỐ NGOÀI

#### Mệnh đề 5 {#alg-iii-s7-prop-5 .statement}

(i) Cho $ (x_i)_{1 \leq i \leq n} $ là một dãy hữu hạn các phần tử của môđun $ M $; với mọi phép hoán vị $ \sigma $ trong nhóm đối xứng $ S_n $,

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $ \varepsilon_\sigma $ ký hiệu dấu của phép hoán vị $ \sigma $.

(ii) Nếu tồn tại hai chỉ số phân biệt $ i, j $ sao cho $ x_i = x_j $, tích

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

bằng không.

(i) Trước hết, vì $ x \wedge x = 0 $ với mọi $ x \in M $ theo định nghĩa của iđêan $ \mathfrak{g}' $, nên, với $ x, y $ trong $ M $,

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

Điều này thiết lập (6) trong trường hợp $ n = 2 $. Trường hợp tổng quát suy ra từ § 4, no. 6, Bổ đề 3.

(ii) Theo giả thiết của (ii), tồn tại một phép hoán vị $ \sigma \in S_n $ sao cho $ \sigma(1) = i $ và $ \sigma(2) = j $; khi đó vế trái của (6) bằng không đối với phép hoán vị này và do đó vế phải cũng vậy.

#### Hệ quả 1 {#alg-iii-s7-prop-5-cor-1 .statement}

Cho $ H, K $ là hai tập hợp con bù nhau của khoảng $ [1, n] $ của $ \mathbf{N} $ và cho $ (i_h)_{1 \leq h \leq p}, (j_k)_{1 \leq k \leq n-p} $ là các dãy các phần tử của $ H $ và $ K $ tương ứng, được sắp xếp theo thứ tự tăng; ta viết

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

khi đó

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $ \nu $ là số các cặp có thứ tự $ (i, j) \in H \times K $ sao cho $ i > j $.

Theo Mệnh đề 5, điều này quy về việc chứng minh

#### Bổ đề 1 {#alg-iii-s7-lem-1 .statement}

Nếu $ \sigma \in S_n $ là phép hoán vị sao cho $ \sigma(h) = i_h $ với $ 1 \leq h \leq p $, $ \sigma(h) = j_{n-p} $ với $ p + 1 \leq h \leq n $, thì $ \varepsilon_\sigma = (-1)^\nu $.

Với $ 1 \leq h < h' \leq p $ hoặc $ p + 1 \leq h < h' \leq n $, $ \sigma(h') > \sigma(h) $ và số các cặp có thứ tự $ (h, h') $ sao cho $ 1 \leq h \leq p < h' \leq n $ và $ \sigma(h) > \sigma(h') $ bằng $ \nu $.

#### Hệ quả 2 {#alg-iii-s7-lem-1-cor-2 .statement}

Đại số phân bậc $ \bigwedge(M) $ là phản xứng ($ \S 4 $, no. 9).

Chỉ cần áp dụng Mệnh đề 13 của $ \S 4 $, no. 9 cho $ \bigwedge(M) $, lấy tập hợp $ M $ làm hệ sinh và sử dụng Mệnh đề 5.

#### Mệnh đề 6 {#alg-iii-s7-prop-6 .statement}

*Nếu M là một A-môđun sinh hữu hạn, $ \bigwedge(M) $ là một A-môđun sinh hữu hạn; ngoài ra, nếu M thừa nhận một hệ sinh gồm n phần tử, thì $ \bigwedge^p(M) = \{0\} $ với $ p > n $.*

Cho $ (x_i)_{1 \leq i \leq n} $ là một hệ sinh của M. Mọi phần tử của $ \bigwedge^p(M) $ là một tổ hợp tuyến tính của các phần tử có dạng
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
trong đó các chỉ số $ i_k $ thuộc $ \{1, n\} $; theo Mệnh đề 5, có thể giả sử các chỉ số này phân biệt (nếu không phần tử tương ứng bằng không). Nếu $ p > n $, không có dãy chỉ số nào như vậy và do đó $ \bigwedge^p(M) = \{0\} $. Nếu $ p \leq n $, các dãy này có số lượng hữu hạn, điều này hoàn tất chứng minh.

### 4. LŨY THỪA NGOÀI THỨ *n* CỦA MỘT MÔĐUN VÀ CÁC ÁNH XẠ ĐA TUYẾN TÍNH PHẢN XỨNG
