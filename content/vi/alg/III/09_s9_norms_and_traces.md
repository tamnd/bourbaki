---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 9
section_title: Norms and traces
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0565-0574, 0668-0668
extraction: ocr
subsections:
    - "no": 1
      title: NORMS AND TRACES RELATIVE TO A MODULE
      page: 0
      pdf_page: 565
    - "no": 2
      title: PROPERTIES OF NORMS AND TRACES RELATIVE TO A MODULE
      page: 0
      pdf_page: 566
    - "no": 3
      title: NORM AND TRACE IN AN ALGEBRA
      page: 0
      pdf_page: 567
    - "no": 4
      title: PROPERTIES OF NORMS AND TRACES IN AN ALGEBRA
      page: 0
      pdf_page: 569
    - "no": 5
      title: DISCRIMINANT OF AN ALGEBRA
      page: 0
      pdf_page: 573
statements: 13
exercises: 1
content_sha256: df166f7af9a22f847f92199a3707dcf681a9521a13cd83538ce6cd84de81e5d1
translated_from: content/en/alg/III/09_s9_norms_and_traces.md
source_content_sha256: 5add91c7bd7089731ed7a5d2ad57c28c920b08eae47ea725f3047adcfea646a2
translation_model: gpt-5.4-mini
translation_run: translate-vi-f8256ec5
glossary_version: 34
glossary_terms_sha256: 9407633ad11ace19412a0443c80de8aedf665b07234990a89769ecf17cad6fb1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. CHUẨN VÀ VẾT

Xuyên suốt đoạn này, $ K $ sẽ ký hiệu một vành giao hoán và $ A $ một đại số kết hợp có đơn vị trên $ K $. Mọi $ A $-môđun sẽ được giả thiết là được cho cấu trúc $ K $-môđun thu được bằng cách hạn chế vô hướng xuống $ K $.

### 1. CHUẨN VÀ VẾT TƯƠNG ĐỐI VỚI MỘT MÔĐUN

#### Định nghĩa 1 {#alg-iii-s9-def-1 .statement}

Cho $ M $ là một $ A $-môđun thừa nhận một cơ sở hữu hạn như một $ K $-môđun. Với mọi $ a \in A $, ký hiệu $ a_M $ là tự đồng cấu $ x \mapsto ax $ của $ K $-môđun $ M $. Vết, định thức và đa thức đặc trưng của $ a_M $ lần lượt được gọi là vết, chuẩn và đa thức đặc trưng của $ z $ tương đối với $ M $.

Vết và chuẩn của $ a $ do đó là các phần tử của $ K $, lần lượt được ký hiệu bởi $ \operatorname{Tr}_{M/K}(a) $ và $ N_{M/K}(a) $; đa thức đặc trưng của $ a $ là một phần tử của $ K[X] $, được ký hiệu bởi $ \mathrm{Pc}_{M/K}(a; X) $. Ta bỏ $ K $ trong ký hiệu trên khi không có nguy cơ nhầm lẫn.

Từ các tính chất của vết và định thức của một tự đồng cấu (II, § 4, no. 3 và § 8, no. 1) ta thu được các hệ thức

$$
\operatorname{Tr}_M(a + a') = \operatorname{Tr}_M(a) + \operatorname{Tr}_M(a')
$$

(2)    $ \mathrm{Tr}_M(aa') = \mathrm{Tr}_M(a'a) $
(3)    $ N_M(aa') = N_M(a)N_M(a') $

với mọi $ a, a' $ trong $ A $.

Cho $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của $ K $-môđun $ M $ và $ (m_{ij}(a)) $ là ma trận của tự đồng cấu $ a_M $ đối với cơ sở này. Các hàm $ m_{ij} $ là các dạng tuyến tính trên $ K $-môđun $ A $ và

(4)    $ \mathrm{Tr}_M(a) = \sum_{i=1}^n m_{ii}(a) $
(5)    $ N_M(a) = \det(m_{ij}(a)) $
(6)    $ \mathrm{Pc}(a; X) = \det(\delta_{ij}X - m_{ij}(a)). $

Từ phương pháp tính định thức (\S 8, no. 11, công thức (50)) suy ra rằng

(7)    $ \mathrm{Pc}_M(a; X) = X^n + c_1 X^{n-1} + \cdots + c_n $

trong đó

(8)    $ c_1 = -\mathrm{Tr}_M(a), \quad c_n = (-1)^n N_M(a). $

Với $ \lambda \in K $,

(9)    $ \mathrm{Tr}_M(\lambda) = n.\lambda, \quad N_M(\lambda) = \lambda^n, \quad \mathrm{Pc}_M(\lambda; X) = (X - \lambda)^n. $

Cho $ K' $ là một $ K $-đại số giao hoán. Đặt $ M' = K' \otimes_K M $ và $ A' = K' \otimes_K A $, do đó $ M' $ có một cấu trúc môđun $ A' $ (\S 4, Ví dụ 2). Là một $ K' $-môđun, $ M' $ có cơ sở gồm các $ 1 \otimes e_i $ ($ 1 \leq i \leq n $) và ma trận của $ a_M $ đối với $ (e_i) $ bằng ma trận của $ (1 \otimes a)_M' $ đối với $ (e'_i) $. Khi đó

(12)    $ \mathrm{Tr}_{M'}(1 \otimes a) = \mathrm{Tr}_M(a).1, \quad N_{M'}(1 \otimes a) = N_M(a).1 $
        $ \mathrm{Pc}_{M'}(1 \otimes a; X) = \mathrm{Pc}_M(a; X).1 $

với mọi $ a \in A $, trong đó 1 ký hiệu phần tử đơn vị của $ K' $. Đặc biệt, nếu ta lấy $ K' = K[X] $, thì

(13)    $ \mathrm{Pc}_{M/K}(a; X) = N_{M[X]/K[X]}(X - a). $

### 2. CÁC TÍNH CHẤT CỦA CHUẨN VÀ VẾT ĐỐI VỚI MỘT MÔĐUN

Nếu $ M $ và $ M' $ là hai *đẳng cấu* $ A $-môđun với các cơ sở hữu hạn trên $ K $, thì, với mọi $ a \in A $,

(14)    $ \mathrm{Tr}_{M'}(a) = \mathrm{Tr}_M(a), \quad N_{M'}(a) = N_M(a), \quad \mathrm{Pc}_{M'}(a; X) = \mathrm{Pc}_M(a; X) $

vì nếu $ f $ là một đẳng cấu của $ M $ lên $ M' $, thì ma trận của $ a_M $ đối với một cơ sở $ B $ của $ M $ trên $ K $ chính là ma trận của $ a_{M'} $ đối với cơ sở $ f(B) $ của $ M' $.

#### Mệnh đề 1 {#alg-iii-s9-prop-1 .statement}

Cho $ M = M_0 \supset M_1 \supset \ldots \supset M_r = \{0\} $ là một dãy giảm của các môđun con của một $ A $-môđun $ M $ sao cho mỗi $ K $-môđun $ P_i = M_{i-1}/M_i $ ($ 1 \leq i \leq r $) đều thừa nhận một cơ sở hữu hạn. Khi đó $ K $-môđun $ M $ cũng thừa nhận một cơ sở hữu hạn và

$$
\operatorname{Tr}_M(a) = \sum_{i=1}^r \operatorname{Tr}_{P_i}(a), \qquad N_M(a) = \prod_{i=1}^r N_{P_i}(a)
$$
(15)

$$
P_{C_M}(a; X) = \prod_{i=1}^r P_{C_{P_i}}(a; X).
$$

Cho $ B'_i $ là một cơ sở của $ P_i $ trên $ K $; khi đó một hệ đại diện $ B_i $ của $ B'_i $ (mod. $ M_i $) là một cơ sở của một môđun con bổ sung của $ K $-môđun $ M_i $ trong $ K $-môđun $ M_{i-1} $ (II, § 1, no. 11, Mệnh đề 21). Hợp $ B $ của các $ B_i $ ($ 1 \leq i \leq r $) là một cơ sở của $ M $ trên $ K $. Gọi $ X_{tt} $ là ma trận của tự đồng cấu $ a_{P_i} $ đối với cơ sở $ B'_i $. Ngay lập tức ta có ma trận của $ a_M $ đối với $ B $ có dạng

$$
\begin{pmatrix}
X_{rr} & X_{r,r-1} & \cdots & X_{r,1} \\
0 & X_{r-1,r-1} & \cdots & X_{r-1,1} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & X_{11}
\end{pmatrix}
$$

và mệnh đề suy ra từ các công thức (4), (5) và (6) của no. 1 và công thức (31) của § 8, no. 6.

#### Mệnh đề 2 {#alg-iii-s9-prop-2 .statement}

Let $ A, A' $ là hai $ K $-đại số, $ M $ là một $ A $-môđun và $ M' $ là một $ A' $-môđun. Giả sử rằng $ M $ và $ M' $ là các $ K $-môđun tự do có số chiều tương ứng là $ n $ và $ n' $ và coi $ M \otimes_K M' $ như là một $ (A \otimes_K A') $-môđun ($ \S 4 $, no. 3, Ví dụ 2). Khi đó, với $ a \in A $ và $ a' \in A' $,

$$
\operatorname{Tr}_{M \otimes M'}(a \otimes a') = \operatorname{Tr}_M(a) \operatorname{Tr}_{M'}(a')
$$
(16)

$$
N_{M \otimes M'}(a \otimes a') = (N_M(a))^{n'} (N_{M'}(a'))^n.
$$
(17)

Công thức (16) suy ra từ II, § 4, no. 4, công thức (26) và công thức (17) từ § 8, no. 6, công thức (33).

### 3. CHUẨN VÀ VẾT TRONG MỘT ĐẠI SỐ

#### Định nghĩa 2 {#alg-iii-s9-def-2 .statement}

Cho $ A $ là một $ K $-đại số là một $ K $-môđun tự do hữu hạn chiều. Với mỗi phần tử $ a \in A $, vết (tương ứng chuẩn,\footnote{† Khái niệm này không nên lẫn với khái niệm chuẩn trong một đại số trên một trường có giá trị (\emph{Tôpô đại cương}), IX, § 3, no. 7.) tương ứng đa thức đặc trưng) của $ a $ đối với $ A $ và $ K $ là vết (tương ứng định thức, tương ứng đa thức đặc trưng) của tự đồng cấu $ x \mapsto ax $ của $ K $-môđun $ A $.

Vết, chuẩn và đa thức đặc trưng của $ a \in A $ đối với $ A $ và $ K $ được ký hiệu lần lượt là $ \mathrm{Tr}_{A/K}(a) $, $ N_{A/K}(a) $ và $ \mathrm{Pc}_{A/K}(a; X) $; ta lược bỏ $ K $ và ngay cả $ A $ khỏi ký hiệu này khi không sợ nhầm lẫn. Chú ý rằng vết (tương ứng chuẩn, đa thức đặc trưng) của $ a \in A $ chỉ là vết (tương ứng chuẩn, đa thức đặc trưng) của $ a $ đối với $ A $-môđun $ A_s $.

Giả sử rằng $ A $ là tích $ A_1 \times A_2 \times \cdots \times A_m $ của một số hữu hạn các đại số hữu hạn chiều trên $ K $ mà là các $ K $-môđun tự do. Dùng nhận xét trên và Mệnh đề 1 của no. 2, ta có, với mỗi phần tử

$$
a = (a_1, \ldots, a_m) \in A,
$$

$$
\mathrm{Tr}_{A/K}(a) = \sum_{i=1}^m \mathrm{Tr}_{A_i/K}(a_i), \qquad N_{A/K}(a) = \prod_{i=1}^m N_{A_i/K}(a_i)
$$
(18)

$$
\mathrm{Pc}_{A/K}(a; X) = \prod_{i=1}^m \mathrm{Pc}_{A_i/K}(a_i; X).
$$

Tương tự, Mệnh đề 2 của no. 2 cho thấy rằng nếu $ A $ và $ A' $ là hai đại số, là các $ K $-môđun tự do, có số chiều hữu hạn lần lượt là $ n, n' $ trên $ K $, thì, với $ a \in A, a' \in A' $.

$$
\mathrm{Tr}_{A \otimes A'}(a \otimes a') = \mathrm{Tr}_A(a) \, \mathrm{Tr}_{A'}(a')
$$
(19)

$$
N_{A \otimes A'}(a \otimes a') = (N_A(a))^{n'} (N_{A'}(a'))^n.
$$
(20)

Cuối cùng, cho $ A $ là một đại số hữu hạn chiều trên $ K $ là một $ K $-môđun tự do, $ h $ là một đồng cấu của $ K $ vào một vành giao hoán $ K' $ và $ A' = A_{(K')} $ là đại số trên $ K' $ dẫn xuất từ $ A $ bằng cách mở rộng vô hướng nhờ $ h $. Từ công thức (12) của mục 1 suy ra rằng, với mọi $ a \in A $,

$$
\mathrm{Tr}_{A'/K'}(1 \otimes a) = h(\mathrm{Tr}_{A/K}(a)), \qquad N_{A'/K'}(1 \otimes a) = h(N_{A/K}(a))
$$
(21)

$$
\mathrm{Pc}_{A'/K'}(1 \otimes a; X) = \bar{h}(\mathrm{Pc}_{A/K}(a; X))
$$

trong đó $ \bar{h} $ là đồng cấu $ K[X] \to K'[X] $ dẫn xuất từ $ h $. Đặc biệt, với $ K' = K[X] $, ta thu được, viết $ A[X] = A \otimes_K K[X] $,

$$
\mathrm{Pc}_{A/K}(a; X) = N_{A[X]/K[X]}(X - a).
$$
(22)

Tổng quát hơn, nếu $ K' $ là một đại số giao hoán trên $ K $ và $ A' = A \otimes_K K' $, thì, với mọi $ x \in A' $,

$$
\mathrm{Pc}_{A/K}(a; x) = N_{A'/K'}(x - a).
$$

#### Ví dụ {#alg-iii-s9-n3-exa-1 .statement}

(1) Cho $ A $ là một đại số bậc hai trên $ K $ kiểu $ (\alpha, \beta) $ và $ (e_1, e_2) $ là một cơ sở kiểu $ (\alpha, \beta) $ (\S 2, no. 3). Với $ x = \xi e_1 + \eta e_2 $, $ \mathrm{Tr}_{A/K}(x) = 2\xi + \beta \eta $ và $ N_{A/K}(x) = \xi^2 + \beta \xi \eta - \alpha \eta^2 $; do đó các hàm này trùng với vết và chuẩn Cayley của $ x $ (\S 2, no. 24).

(2) Cho $ A $ là một đại số quaternion trên $ K $. Một tính toán trực tiếp cho phép kiểm tra rằng $ \mathrm{Tr}_{A/\mathbf{K}}(x) = 2T(x) $ và $ N_{A/\mathbf{K}}(x) = (N(x))^2 $, trong đó T và N là vết và chuẩn Cayley (\S 2, no. 4).

(3) Cho $ A = \mathbf{M}_n(\mathbf{K}) $ và cho cơ sở chính tắc $ (E_{ij}) $ của A (II, \S 10, no. 3) được sắp theo thứ tự từ điển. Khi đó thấy ngay rằng, với mọi ma trận $ X = \sum_{i,j} \xi_{ij} E_{ij} $ ma trận (cấp $ n^2 $) của tự đồng cấu $ Y \mapsto XY $ có dạng

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

do đó $ \mathrm{Tr}_{A/\mathbf{K}}(X) = n \cdot \mathrm{Tr}(X) $ và $ N_{A/\mathbf{K}}(X) = (\det(X))^n $.

### 4. CÁC TÍNH CHẤT CỦA CHUẨN VÀ VẾT TRONG MỘT ĐẠI SỐ

#### Mệnh đề 3 {#alg-iii-s9-prop-3 .statement}

*Cho A là một đại số trên K thừa nhận một cơ sở hữu hạn. Để một phần tử $ a \in A $ khả nghịch, cần và đủ rằng $ N_{A/\mathbf{K}}(a) $ khả nghịch trong $ \mathbf{K} $.*

Nếu $ a $ có nghịch đảo $ a' $ trong $ A $, thì

$$
N_{A/\mathbf{K}}(a) N_{A/\mathbf{K}}(a') = N_{A/\mathbf{K}}(aa') = N_{A/\mathbf{K}}(1) = 1
$$

bằng công thức (3) của no. 1. Ngược lại, nếu $ N_{A/\mathbf{K}}(a) $ là khả nghịch, thì tự đồng cấu $ h : x \mapsto ax $ là song ánh (\S 8, no. 2, Định lý 1). Khi đó tồn tại $ a' \in A $ sao cho $ aa' = 1 $; rồi $ h(a'a - 1) = aa'a - a = (aa' - 1)a = 0 $, do đó $ aa' = 1 $ vì $ h $ là đơn ánh. Suy ra $ a' $ là nghịch đảo của $ a $.

#### Mệnh đề 4 {#alg-iii-s9-prop-4 .statement}

*Cho A là một K-đại số nhận một cơ sở hữu hạn. Với mọi $ a \in A $, $ \mathrm{Pc}_{A/\mathbf{K}}(a; a) = 0 $. \*

Điều này suy ra ngay lập tức từ định lý Cayley-Hamilton (\S 8, no. 11, Mệnh đề 20).

#### Mệnh đề 5 {#alg-iii-s9-prop-5 .statement}

*Cho A là một K-đại số và m là một iđêan hai phía của A. Giả sử rằng $ A_0 = A/m $ là một K-môđun tự do có số chiều hữu hạn n, rằng tồn tại một số nguyên $ r > 0 $ sao cho $ m^r = \{0\} $ và rằng $ m^{i-1}/m^i $ là một $ A_0 $-môđun tự do có số chiều hữu hạn $ s_i $ với $ 1 \leq i \leq r $. Đặt $ s = s_1 + \cdots + s_r $ và với mọi $ a \in A $ ký hiệu $ a_0 $ là lớp của $ a $ mod. m. Khi đó A là một K-môđun tự do có chiều $ ns $ và, với mọi $ a \in A $,*

$$
\mathrm{Tr}_A(a) = s \cdot \mathrm{Tr}_{A_0}(a_0), \qquad N_A(a) = (N_{A_0}(a_0))^s
$$
$$
\mathrm{Pc}_A(a; X) = (\mathrm{Pc}_{A_0}(a_0; X))^s.
$$

Do II, \S 1, no. 13, Mệnh đề 25, $ m^{i-1}/m^i $ là một K-môđun tự do có chiều $ ns_i $. Do đó có thể áp dụng Mệnh đề 1 của no. 2 với $ P_i = m^{i-1}/m^i $;

điều này trước hết cho thấy rằng $ A $ là một $ K $-môđun tự do có chiều $ n(s_1 + \cdots + s_r) = ns $. Hơn nữa, giả thiết suy ra rằng $ A $-môđun $ P_i $ đẳng cấu với một tổng trực tiếp của $ s_i $ môđun con đẳng cấu với $ A $-môđun $ A_0 $; do đó, theo Mệnh đề 1 của no. 2, $ N_{P_i}(a) = N_{A_0}(a)^{s_i} $; cuối cùng suy ra
$$
N_A(a) = N_{A_0}(a)^s.
$$
Trong công thức này $ N_{A_0}(a) $ được định nghĩa bằng cách xem $ A_0 $ như một $ A $-môđun trái và nó bằng định thức của ánh xạ tuyến tính trên K $ x \mapsto ax $ của $ A_0 $ vào chính nó; nhưng, vì $ ax = a_0x $ với $ x \in A_0 $, $ N_{A_0}(a) = N_{A_0}(a_0) $, điều đó hoàn tất chứng minh công thức (23) cho chuẩn. Hai công thức còn lại được chứng minh tương tự.

#### Mệnh đề 6 {#alg-iii-s9-prop-6 .statement}

*Cho $ A $ là một $ K $-đại số giao hoán có một cơ sở hữu hạn trên $ K $ và $ V $ là một $ A $-môđun có một cơ sở hữu hạn trên $ A $. Khi đó $ V $ có một cơ sở hữu hạn trên $ K $ và với mọi $ A $-tự đồng cấu $ u $ của $ V $, nếu $ u_K $ là ánh xạ $ u $ xét như một $ K $-tự đồng cấu của $ V $,*
$$
\begin{align*}
\operatorname{Tr}(u_K) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}(u)), \qquad \det(u_K) = N_{A/K}(\det(u)) \\
\operatorname{Pc}(u_K; X) &= N_{A[X]/K[X]}(\operatorname{Pc}(u; X)).
\end{align*}
$$
(24)

Cho $ (a_i)_{1 \leq i \leq m} $ là một cơ sở của $ A $ trên $ K $ và $ (e_j)_{1 \leq j \leq n} $ là một cơ sở của $ V $ trên $ A $; khi đó $ (a_i e_j) $ là một cơ sở của $ V $ trên $ K $ (II, § 1, no. 13, Proposition 25). Mặt khác công thức thứ ba trong các công thức (24) có thể suy ra từ công thức thứ hai áp dụng cho tự đồng cấu $ X - \bar{u} $ của $ A[X] $-môđun $ A[X] \otimes_A V $ (\S 8, no. 10). Vì vậy chỉ cần chứng minh hai công thức đầu trong (24). Trước hết ta thiết lập bổ đề sau:

*Bổ đề 1. Cho $ X_{ij} $ ($ 1 \leq i \leq n,\ 1 \leq j \leq n $) là $ n^2 $ ẩn thức, $ X $ là ma trận vuông $ (X_{ij}) $ cấp $ n $ và $ D(X_{11}, \ldots, X_{nn}) \in \mathbf{Z}[X_{11}, \ldots, X_{nn}] $ là định thức $ \det(X) $. Mặt khác cho $ A $ là một vành giao hoán, $ M_{ij} $ ($ 1 \leq i \leq n,\ 1 \leq j \leq n $) $ n^2 $ ma trận cấp $ m $ trên $ A $, đôi một giao hoán, và $ M $ là ma trận vuông cấp $ mn $ trên $ A $ có thể được biểu diễn như một ma trận vuông các ma trận (II, § 10, no. 7)
$$
M = \begin{pmatrix}
M_{11} & M_{12} & \cdots & M_{1n} \\
M_{21} & M_{22} & \cdots & M_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
M_{n1} & M_{n2} & \cdots & M_{nn}
\end{pmatrix}
$$
Khi đó định thức của $ M $ bằng định thức của ma trận vuông
$$
D(M_{11}, \ldots, M_{nn})
$$
cấp $ m $.

Ta chứng minh bằng quy nạp theo $ n $, các trường hợp $ n = 0 $ và $ n = 1 $ là tầm thường.

Cho $ Z $ là một ẩn thức mới và $ N_{ij} $ là ma trận $ M_{ij} + \delta_{ij} Z I_m $ ($ \delta_{ij} $ là chỉ số Kronecker). Nếu $ D^{ij}(X_{11}, \ldots, X_{nn}) $ là *phần bù đại số* của $ X_{ij} $ trong ma trận $ X $ (\S 8, no. 6), thì

$$
\text{(25)} \quad X_{ji} D^{ki}(X_{11}, \ldots, X_{nn}) = \delta_{jk} D(X_{11}, \ldots, X_{nn})
$$

(§ 8, no. 6, công thức (28)). Ta viết $ N'_{ij} = D^{ij}(N_{11}, \ldots, N_{nn}) $, đây là một ma trận vuông cấp $ m $ trên $ \mathbf{A}[Z] $ và xét tích $ N . U $, trong đó

$$
U = \begin{pmatrix}
N'_{11} & 0 & \cdots & 0 \\
N'_{12} & I_m & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
N'_{1n} & 0 & \cdots & I_m
\end{pmatrix},
$$
$$
N = \begin{pmatrix}
N_{11} & N_{12} & \cdots & N_{1n} \\
N_{21} & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
N_{n1} & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

Tính tích này theo khối (II, § 10, no. 5) và dùng các công thức (25), ta thu được

$$
N . U = \begin{pmatrix}
P & N_{12} & \cdots & N_{1n} \\
0 & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
0 & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

trong đó ta đã viết $ P = D(N_{11}, \ldots, N_{nn}) $. Đặt

$$
Q = \begin{pmatrix}
N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots \\
N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

đây là một ma trận cấp $ m(n-1) $; khi đó (§ 8, no. 6, công thức (31)) (det $ N $) (det $ U $) = (det $ P $)(det $ Q $) và det $ U = \det N'_{11} $. Nhưng theo giả thiết quy nạp, det $ Q = \det(D^{11}(N_{11}, \ldots, N_{nn})) = \det N'_{11} $ và theo định nghĩa của các $ N_{ij} $, rõ ràng det $ Q $ là một đa thức trong $ \mathbf{A}[Z] $ có bậc $ m(n-1) $, có số hạng $ Z^{m(n-1)} $ với hệ số 1 ; suy ra ngay lập tức det $ Q $ không phải là một ước của không trong đại số phân bậc $ \mathbf{A}[Z] $. Vì vậy ta kết luận rằng det $ N = \det(D(N_{11}, \ldots, N_{nn})) $ trong $ \mathbf{A}[Z] $; nếu thay 0 cho $ Z $ trong các đa thức này, thì det $ M = \det(D(M_{11}, \ldots, M_{nn})) $.

Sau khi đã chứng minh bổ đề này, K-môđun V là tổng trực tiếp của các K-môđun $ Ae_j $ ($ 1 \leq j \leq n $); ta viết $ u(e_j) = \sum_{k=1}^n c_{jk} e_k $. Với mọi phần tử $ xe_j \in Ae_j $, với $ x \in A $, thành phần của $ u(xe_j) $ trong $ Ae_k $ là $ xc_{jk} e_k $; suy ra ma trận của $ u_k $ đối với cơ sở $ (a_i e_j) $ của K-môđun V có thể viết dưới dạng một ma trận vuông các ma trận $ (M_{jk}) $, trong đó $ M_{jk} $ là ma trận của ánh xạ K-tuyến tính $ xe_j \mapsto xc_{jk} e_k $ từ $ Ae_j $ vào $ Ae_k $ đối với các cơ sở $ (a_i e_j)_{1 \leq i \leq m} $ và $ (a_i e_k)_{1 \leq i \leq m} $ của hai K-môđun này (II, § 10, no. 5). Nếu với mọi $ t \in A $, $ M(t) $ ký hiệu ma trận, đối với cơ sở $ (a_i)_{1 \leq i \leq m} $ của A trên K, của tự đồng cấu $ x \mapsto xt $ của A, thì $ M_{jk} = M(c_{jk}) $; vì $ t \mapsto M(t) $ là một đồng cấu vành nên các ma trận $ M_{jk} $ *giao hoán với nhau*. Khi đó
$$
\det u_K = \det(D(M_{11}, \ldots, M_{nn}))
$$
theo Bổ đề 1. Nhưng vì $ t \mapsto M(t) $ là một đồng cấu vành, $ D(M_{11}, \ldots, M_{nn}) $ là ma trận của tự đồng cấu K-tuyến tính $ x \mapsto x.\det(c_{jk}) $ của A đối với cơ sở $ (a_i) $; theo định nghĩa, định thức của nó do đó là $ N_{A/K}(\det(u)) $, điều đó chứng minh công thức thứ hai của (24). Mặt khác,
$$
\operatorname{Tr}(u_K) = \sum_{j=1}^n \operatorname{Tr}(M_{jj}) = \sum_{j=1}^n \operatorname{Tr}_{A/K}(c_{jj}) = \operatorname{Tr}_{A/K}\left( \sum_{j=1}^n c_{jj} \right) = \operatorname{Tr}_{A/K}(\operatorname{Tr}(u))
$$
và chứng minh của Mệnh đề 6 đã hoàn tất.

#### Hệ quả {#alg-iii-s9-n4-cor-1 .statement}

*Cho A là một đại số giao hoán trên K có một cơ sở hữu hạn trên K và B là một đại số trên A có một cơ sở hữu hạn trên A. Khi đó B có một cơ sở hữu hạn trên K, và, với mọi $ b \in B $ ("các công thức bắc cầu")*
$$
\begin{align*}
\operatorname{Tr}_{B/K}(b) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}_{B/A}(b)), \quad N_{B/K}(b) = N_{A/K}(N_{B/A}(b)) \\
P_{C_{B/K}}(b; X) &= N_{A[X]/K[X]}(P_{C_{B/A}}(b; X)).
\end{align*}
$$
(26)
Điều này suy ra ngay từ Mệnh đề 6, đặt $ V = B $ và $ u(x) = bx $.

#### Nhận xét {#alg-iii-s9-n4-rem-1 .statement}

*Giả sử đồng cấu $ \lambda \mapsto \lambda . 1 $ của K vào A là đơn ánh và đồng nhất K với ảnh của nó trong A; giả sử A có một cơ sở hữu hạn $ (e_i)_{1 \leq i \leq n} $ như một K-môđun. Cho s là một tự đẳng cấu của A sao cho $ s(K) = K $. Cho a là một phần tử của A; khi đó, bằng cách vận chuyển cấu trúc
$$
\begin{align*}
\operatorname{Tr}_{A/K}(s(a)) &= s(\operatorname{Tr}_{A/K}(a)) \\
N_{A/K}(s(a)) &= s(N_{A/K}(a)).
\end{align*}
$$
(27) (28)
*Hãy xét thêm một đạo hàm D của A ($ \S 10 $, no. 2) sao cho $ D(K) \subset K $ và viết $ D(e_i) = \sum_{j=1}^n e_j \mu_{ji} $ với $ \mu_{ji} \in K $; viết*
$$
\begin{align*}
D(a)e_i + aD(e_i) &= D(ae_i) = \sum_{j=1}^n (D(e_j)\lambda_{ji} + e_j D(\lambda_{ji})).
\end{align*}
$$
Suy ra rằng
$$
D(a)e_i = \sum_{j=1}^n e_j v_{ji}
$$
với $ v_{ji} = D(\lambda_{ji}) + \sum_{k=1}^n (\mu_{jk}\lambda_{ki} - \lambda_{jk}\mu_{ki}) $. Vì $ \sum_{i,k} (\mu_{ik}\lambda_{ki} - \lambda_{ik}\mu_{ki}) = 0 $, do đó $ \operatorname{Tr}_{A/\mathbf{K}}(D(a)) = \sum_{i=1}^n D(\lambda_{ii}) $, nói cách khác
$$
\operatorname{Tr}_{A/\mathbf{K}}(D(a)) = D(\operatorname{Tr}_{A/\mathbf{K}}(a)). *
$$

### 5. BIỆT THỨC CỦA MỘT ĐẠI SỐ

#### Định nghĩa 3 {#alg-iii-s9-def-3 .statement}

*Cho A là một đại số trên K có một cơ sở hữu hạn gồm n phần tử. Biệt thức của một dãy $(x_1, \ldots, x_n)$ gồm n phần tử của A, đối với K, ký hiệu bởi $D_{A/\mathbf{K}}(x_1, \ldots, x_n)$, là biệt thức của ma trận vuông*
$$
(\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
Trước hết xét một cơ sở $(e_i)_{1 \leq i \leq n}$ của A trên K và viết
$$
e_i e_j = \sum_{k=1}^n c_{ij k} e_k \quad \text{with} \quad c_{ij k} \in \mathbf{K}.
$$
Khi đó $ \operatorname{Tr}_{A/\mathbf{K}}(e_i) = \sum_{s=1}^n c_{iss} $, do đó $ \operatorname{Tr}_{A/\mathbf{K}}(e_i e_j) = \sum_{k,s} c_{ij k} c_{kss} $ và vì thế
$$
D_{A/\mathbf{K}}(e_1, \ldots, e_n) = \det \left( \left( \sum_{k,s} c_{ij k} c_{kss} \right)_{1 \leq i \leq n, 1 \leq j \leq n} \right).
$$
Bây giờ cho $(x_i)_{1 \leq i \leq n}, (x'_i)_{1 \leq i \leq n}$ là hai dãy gồm n phần tử của A và giả sử rằng tồn tại một ma trận vuông cấp n, $M = (m_{ij})$, có hệ số trong K, sao cho $x_i = \sum_{j=1}^n m_{ij} x'_j$ với $1 \leq i \leq n$. Ta viết
$$
T = (\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}, \qquad T' = (\operatorname{Tr}_{A/\mathbf{K}}(x'_i x'_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
Khi đó $ \operatorname{Tr}_{A/\mathbf{K}}(x_i x_j) = \sum_{p,q} m_{ip} m_{jq} \operatorname{Tr}_{A/\mathbf{K}}(x'_p x'_q) $, do đó $ T = M \cdot T' \cdot {}^t M $; quy tắc nhân các định thức do đó cho
$$
\det T = \det M \cdot \det T' \cdot \det {}^t M = (\det M)^2 \det T'
$$
do đó cuối cùng
$$
D_{A/\mathbf{K}}(x_1, \ldots, x_n) = (\det M)^2 D_{A/\mathbf{K}}(x'_1, \ldots, x'_n).
$$

Công thức trên cho thấy đặc biệt rằng các biệt thức của hai cơ sở của A trên K khác nhau bởi bình phương của một phần tử khả nghịch của K và do đó sinh ra cùng một (chính) iđêan của K. Iđêan này $ \Delta_{A/K} $ được gọi là iđêan biệt thức của A trên K; theo công thức (32) biệt thức của mọi dãy n phần tử của A chỉ khác nhau ở thứ tự các hạng có cùng biệt thức, vì định thức của một ma trận hoán vị bằng $ \pm 1 $.

#### Ví dụ {#alg-iii-s9-n5-exa-1 .statement}

(1) Nếu A là một đại số bậc hai kiểu $ (\alpha, \beta) $ trên K, thì (theo ký hiệu của § 2, no. 3) $ \operatorname{Tr}(e_1) = 2, \operatorname{Tr}(e_2) = \beta $,

$$
\operatorname{Tr}(e_2^2) = \alpha \operatorname{Tr}(e_1) + \beta \operatorname{Tr}(e_2) = 2\alpha + \beta^2,
$$

do đó $ D_{A/K}(e_1, e_2) = \beta^2 + 4\alpha $.

(2) Cho $ A = K[X]/K[X]P $, với $ P(X) = X^3 + pX + q $, nên nếu x là ảnh của X trong A thì 1, x, $ x^2 $ lập thành một cơ sở của A trên K và $ x^3 = -px - q $. Thấy ngay rằng $ \operatorname{Tr}(1) = 3, \operatorname{Tr}(x) = 0, \operatorname{Tr}(x^2) = -2p $, xét đến quan hệ $ x^3 = -px - q, \operatorname{Tr}(x^3) = -3q $ và $ \operatorname{Tr}(x^4) = 2p^2 $, do đó dễ dàng $ D_{A/K}(1, x, x^2) = -4p^3 - 27q^2 $.

(3) Cho A là một đại số quaternion kiểu $ (\alpha, \beta, \gamma) $ trên K và $ (1, i, j, k) $ một cơ sở của A kiểu $ (\alpha, \beta, \gamma) $; xét đến § 3, no. 5, công thức (30), dễ dàng tìm được rằng $ \operatorname{Tr}(1) = 4, \operatorname{Tr}(i) = 2\beta, \operatorname{Tr}(j) = \operatorname{Tr}(k) = 0 $, khi đó

$$
D_{A/K}(1, i, j, k) = -16\gamma^2(\beta^2 + 4\alpha)^2.
$$

(4) Cho $ A = M_n(K) $ và xét cơ sở chính tắc $ (E_{ij})_{1 \leq i \leq n, 1 \leq j \leq n} $ của A trên K (II, § 10, no. 3). Suy ra ngay rằng $ \operatorname{Tr}_{A/K}(E_{ij}) = 0 $ nếu $ j \neq i $ và $ \operatorname{Tr}_{A/K}(E_{ii}) = n $ với mọi i; do đó không khó suy ra rằng ma trận $ (\operatorname{Tr}(E_{ij}E_{hk})) $ cấp $ n^2 $ có dạng $ n.P $, trong đó P là một ma trận hoán vị, do đó $ D_{A/K}((E_{ij})) = \pm n^{n^2} $.

### Bài tập {#alg-iii-s9-exercises}

Xem [bài tập cho § 9](exercises/s9/).
