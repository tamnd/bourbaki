---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 10
section_title: Matrices
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0362-0387, 0441-0448
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF MATRICES
      page: 0
      pdf_page: 362
    - "no": 2
      title: MATRICES OVER A COMMUTATIVE GROUP
      page: 0
      pdf_page: 363
    - "no": 3
      title: MATRICES OVER A RING
      page: 0
      pdf_page: 365
    - "no": 4
      title: MATRICES AND LINEAR MAPPINGS
      page: 0
      pdf_page: 366
    - "no": 5
      title: BLOCK PRODUCTS
      page: 0
      pdf_page: 370
    - "no": 6
      title: MATRIX OF A SEMI-LINEAR MAPPING
      page: 0
      pdf_page: 371
    - "no": 7
      title: SQUARE MATRICES
      page: 0
      pdf_page: 373
    - "no": 8
      title: CHANGE OF BASES
      page: 0
      pdf_page: 376
    - "no": 9
      title: EQUIVALENT MATRICES; SIMILAR MATRICES
      page: 0
      pdf_page: 378
    - "no": 10
      title: TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING
      page: 0
      pdf_page: 380
    - "no": 11
      title: TRACE OF A MATRIX
      page: 0
      pdf_page: 382
    - "no": 12
      title: MATRICES OVER A FIELD
      page: 0
      pdf_page: 383
    - "no": 13
      title: EQUIVALENCE OF MATRICES OVER A FIELD
      page: 0
      pdf_page: 384
statements: 35
exercises: 12
content_sha256: 1609eccce70d1890421576c5d71d0a940950156535a80fa835588d33d94e416e
translated_from: content/en/alg/II/10_s10_matrices.md
source_content_sha256: c6c108be989be9295bb6b1d49f88a54316690e415d33aae67035cb355ba5c300
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-5f9ccca3
glossary_version: 34
glossary_terms_sha256: ae97e21d0a8a6f190faca6ef4cc5787d3cc1c91f9f653f7181508772415344a9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. MA TRẬN

### 1. ĐỊNH NGHĨA VỀ MA TRẬN

#### Định nghĩa 1 {#alg-ii-s10-def-1 .statement}

Cho $ I, K, H $ là ba tập hợp; một ma trận kiểu $ (I, K) $ với các phần tử trong $ H $ (hoặc một ma trận kiểu $ (I, K) $ trên $ H $) là một họ $ M = (m_{i\kappa})_{(i, \kappa) \in I \times K} $ các phần tử của $ H $ có tập chỉ số là tích $ I \times K $. Với mọi $ i \in I $, họ $ (m_{i\kappa})_{\kappa \in K} $ được gọi là hàng của $ M $ có chỉ số $ i $; với mọi $ \kappa \in K $, họ $ (m_{i\kappa})_{i \in I} $ được gọi là cột của $ M $ có chỉ số $ \kappa $.

Nếu $ I $ (tương ứng $ K $) là hữu hạn, $ M $ được gọi là một ma trận có một số hữu hạn hàng (tương ứng cột). Tập hợp các ma trận kiểu $ (I, K) $ trên $ H $ được đồng nhất với tích $ HI^{I \times K} $.

Các tên gọi "hàng" và "cột" xuất phát từ sự kiện rằng, trong trường hợp $ I $ và $ K $ là các đoạn $ [1, p], [1, q] $ của $ \mathbf{N} $, các phần tử của ma trận được hình dung như được sắp xếp trong một bảng chữ nhật gồm $ p $ hàng (xếp theo chiều ngang) và $ q $ cột (xếp theo chiều dọc):

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdots & \cdots & \cdots & \cdots \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

Khi $ p $ và $ q $ là các số nguyên cụ thể đủ nhỏ để việc này có thể thực hiện được, theo quy ước, bảng trên là một ký hiệu thực sự biểu thị ma trận đang xét; ký hiệu này cho phép ta không dùng đến các chỉ số, với điều hiểu rằng các chỉ số của một phần tử được xác định bởi vị trí của nó trong bảng; chẳng hạn, khi ta nói đến ma trận

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

ta muốn nói đến ma trận $ (m_{ij})_{1 \leq i < 2, 1 \leq j < 3} $ sao cho

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

Thay cho ma trận kiểu $ ([1, p], [1, q]) $, ta cũng nói ma trận kiểu $ (p, q) $, hoặc ma trận có $ p $ hàng và $ q $ cột, nếu không gây nhầm lẫn; tập hợp các ma trận kiểu $ (p, q) $ trên $ H $ đôi khi được ký hiệu bởi $ \mathbf{M}_{p, q}(H) $.

Mọi ma trận trên $ H $ mà một trong các tập chỉ số $ I, K $ là rỗng đều đồng nhất với họ rỗng các phần tử của $ H $; nó cũng được gọi là ma trận rỗng. Khi $ I = \{i_0\} $ (tương ứng $ K = \{k_0\} $) là một tập hợp gồm một phần tử duy nhất, $ M $ được gọi là ma trận hàng (tương ứng ma trận cột) và chỉ số hàng (tương ứng cột) khi đó có thể được lược bỏ trong ký hiệu; khi $ I $ và $ K $ đều là các tập hợp có một phần tử, một ma trận kiểu $ (I, K) $ thường được đồng nhất với phần tử duy nhất trong ma trận này.

Một họ con $ M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L} $ của một ma trận $ M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K} $, mà tập chỉ số của nó là tích của một tập con $ J $ của $ I $ và một tập con $ L $ của $ K $, được gọi là một *ma trận con* của ma trận $ M $; người ta nói rằng nó thu được bằng cách *bỏ* trong $ M $ các hàng có chỉ số $ \iota \notin J $ và các cột có chỉ số $ \kappa \notin L $; ngược lại, người ta nói rằng $ M $ thu được bằng cách *viền* $ M' $ bởi các hàng có chỉ số $ \iota \notin J $ và các cột có chỉ số $ \kappa \notin L $.

#### Định nghĩa 2 {#alg-ii-s10-def-2 .statement}

*Chuyển vị của một ma trận* $ M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K} $, *được ký hiệu bởi* $ ^tM $, *là ma trận* $ (m'_{\kappa \iota})_{(\kappa, \iota) \in K \times I} $ *trên* $ H $ *được cho bởi* $ m'_{\kappa \iota} = m_{\iota \kappa} $ *với mọi* $ (\iota, \kappa) \in K \times L $.

Suy ra từ định nghĩa này rằng chuyển vị của một ma trận kiểu $ (I, K) $ là một ma trận kiểu $ (K, I) $ và rằng

(1)
$$
^t(^tM) = M.
$$

### 2. MA TRẬN TRÊN MỘT NHÓM GIAO HOÁN

Cho $ G $ là một nhóm giao hoán (viết theo phép cộng). Tập các ma trận trên $ G $, với các tập chỉ số đã cho $ I, K $, có một cấu trúc *nhóm giao hoán* vì nó là tập các ánh xạ từ $ I \times K $ vào $ G $; nhóm này được viết theo phép cộng, sao cho nếu $ M = (m_{\iota \kappa}) $ và $ M' = (m'_{\iota \kappa}) $ là hai phần tử của nó, thì
$$
M + M' = (m_{\iota \kappa} + m'_{\iota \kappa});
$$
phần tử đơn vị của nhóm này do đó là ma trận mà tất cả các phần tử của nó đều là *không* (gọi là *ma trận không*). Rõ ràng
(2)
$$
^t(M + M') = ^tM + ^tM'.
$$

Tổng của hai ma trận do đó chỉ được định nghĩa nếu các tập chỉ số của các hàng và các cột là *giống nhau* đối với hai ma trận.

Cho $ H', H'' $ là hai tập hợp, $ G $ là một nhóm giao hoán (viết theo phép cộng) và $ f : (h', h'') \mapsto h'h'' $ là một ánh xạ từ $ H' \times H'' $ vào $ G $. Cho hai ma trận
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \quad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
trên $ H' $ và $ H'' $ tương ứng sao cho tập chỉ số $ K $ của các cột của $ M' $ là *hữu hạn* và bằng tập chỉ số của các hàng của $ M'' $, *tích của* $ M' $ và $ M'' $ *qua* $ f $, ký hiệu bởi $ M'M'' $ hoặc $ f(M', M'') $, là ma trận
(3)
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
trên $ G $.

Định nghĩa trên giả sử rằng tập chỉ số của các cột của $ M' $ bằng tập chỉ số của các hàng của $ M'' $; đặc biệt tích $ M''M' $ *không có nghĩa nếu* $ I \neq L $. Trong công thức (3), các phần tử của *cùng một* hàng của $ M' $ xuất hiện được nhân ở bên phải với các phần tử của *cùng một* cột của $ M'' $; phép nhân được gọi là được thực hiện "hàng theo cột".

Cho $ f^0 $ là ánh xạ $(h'', h') \mapsto h'h''$ từ $ H'' \times H' $ vào $ G $; suy ra ngay lập tức từ các định nghĩa rằng
$$
t(M'M'') = tM''.tM'
$$
trong đó tích ở vế trái (tương ứng, vế phải) được tính qua $ f $ (tương ứng, qua $ f^0 $).

Khi $ H' $ và $ H'' $ tự thân là các nhóm giao hoán (được viết theo phép cộng) và $ f $ là $\mathbf{Z}$-*song tuyến tính* (\S 3, no. 1), các công thức phân phối
$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$
được kiểm chứng ngay lập tức, các tập chỉ số được giả thiết sao cho các tổng và tích xuất hiện đều được định nghĩa.

Bây giờ cho $ H_1, H_2, H_3, H_{12}, H_{23} $ và $ H $ là các nhóm giao hoán (được viết theo phép cộng), $ f_{12}:H_1 \times H_2 \to H_{12}, f_{23}:H_2 \times H_3 \to H_{23} $ là các ánh xạ và
$$
f_3:H_{12} \times H_3 \to H, \quad f_1:H_1 \times H_{23} \to H
$$
là các ánh xạ $\mathbf{Z}$-song tuyến tính; giả sử thêm rằng, với mọi $ x_i \in H_i \ (i = 1, 2, 3) $
$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$
(điều này cũng có thể được viết như trên $(x_1 x_2)x_3 = x_1(x_2 x_3)$); khi đó, nếu $ M' = (m'_{rs}), M'' = (m''_{st}), M''' = (m'''_{tu}) $ là các ma trận tương ứng trên $ H_1, H_2, H_3 $,
$$
(M'M'')M''' = M'(M''M'''')
$$
khi các tích ở hai vế (được tính tương ứng qua $ f_{12}, f_3, f_{23} $ và $ f_1 $) được định nghĩa; vì
$$
\sum_t \left( \sum_s m'_{rs} m''_{st} \right) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} \left( \sum_t m''_{st} m'''_{tu} \right)
$$
do các giả thiết đã nêu.

Hai vế của (6) cũng được ký hiệu bởi $ M'M''M''' $. Các quy ước tương tự được đưa ra cho các tích của nhiều hơn ba thừa số.

#### Nhận xét {#alg-ii-s10-n2-rem-1 .statement}

Các công thức trên mở rộng cho một tình huống tổng quát hơn. Cụ thể:

(a) Giả sử $ H = \bigcup_{(\iota, \kappa) \in I \times K} G_{\iota \kappa} $ trong đó mỗi $ G_{\iota \kappa} $ là một nhóm giao hoán được viết theo phép cộng; khi đó tổng $ M + M' $ có thể được định nghĩa khi, với mỗi cặp có thứ tự $(\iota, \kappa)$, $ m_{\iota \kappa} \in G_{\iota \kappa} $ và $ m'_{\iota \kappa} \in G_{\iota \kappa} $.

(b) Cho I, K, L là ba tập hợp với K hữu hạn và cho $ H' = \bigcup_{(i, k) \in I \times K} H'_{ik} $, $ H'' = \bigcup_{(k, l) \in K \times L} H''_{kl} $, $ H = \bigcup_{(i, l) \in I \times L} H_{il} $ là ba tập hợp; giả sử rằng mỗi $ H_{il} $ là một nhóm giao hoán được viết theo phép cộng và với mỗi bộ ba $ (i, k, l) $ cho
$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$
là một ánh xạ. Khi đó nếu $ M' = (m'_{ik})_{(i, k) \in I \times K} $, $ M'' = (m''_{kl})_{(k, l) \in K \times L} $ là các ma trận sao cho $ m'_{ik} \in H'_{ik} $ và $ m''_{kl} \in H''_{kl} $ với mọi $ i, k, l $ thì ta có thể định nghĩa tích $ M'M'' $ qua các $ f_{ikl} $. Ta để cho độc giả nhiệm vụ viết ra và chứng minh các công thức tương tự với (4), (5) và (6).

### 3. CÁC MA TRẬN TRÊN MỘT VÀNH

Các ma trận quan trọng nhất trong Toán học là các ma trận trên một vành A. Tập hợp $ A^{I \times K} $ các ma trận trên A tương ứng với các tập chỉ số I, K khi đó có một cách chính tắc một cấu trúc song môđun (A, A) (\S 1, no. 14).

Với mỗi cặp có thứ tự $ (i, k) \in I \times K $, cho $ E_{ik} $ là ma trận $ (a_{jl}) $ sao cho $ a_{ik} = 1 $ và $ a_{jl} = 0 $ với $ (j, l) \neq (i, k) $; các $ E_{ik} $ được gọi là các đơn vị ma trận trong tập hợp các ma trận $ A^{I \times K} $; nếu I và K là hữu hạn, chúng tạo thành cơ sở chính tắc của tập hợp này đối với cấu trúc môđun trái hoặc phải A của nó (\S 1, no. 11). Rõ ràng
$$
tE_{ik} = E_{ki}.
$$

Trừ khi có nói khác đi, tích $ M'M'' $ của hai ma trận trên A (được giả thiết là được định nghĩa) sẽ luôn được hiểu là tương ứng với phép nhân $ (x, y) \mapsto xy $ trong A (hay, cũng được nói là, sẽ được "tính trong A"). Khi đó ta có (no. 2) các công thức về tính kết hợp và tính phân phối

(7)
$$(XY)Z = X(YZ)$$
