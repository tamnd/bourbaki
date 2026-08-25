---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 8
section_title: Norms and traces
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.47-A V.51, A V.153
pdf_pages: 0161-0165, 0267-0267
extraction: ocr
subsections:
    - "no": 1
      title: Recall
      page: 47
      pdf_page: 161
    - "no": 2
      title: Norms and traces in etale algebras
      page: 47
      pdf_page: 161
    - "no": 3
      title: Norms and traces in extensions of finite degree
      page: 50
      pdf_page: 164
statements: 9
exercises: 2
content_sha256: a2f90ac6e9d6874ca37d78203eee3c5acb637228b1b11b66365bb854a84c33d8
translated_from: content/en/alg/V/08_s8_norms_and_traces.md
source_content_sha256: ecf695e74a6f72139dba063988cb43aedaa2286d094bf1ceb5de0b1f88085933
translation_model: gpt-5.4-mini
translation_run: translate-vi-a02df5e1
glossary_version: 34
glossary_terms_sha256: 3d3dff0ef52b100386cbcbd96727b803fb4ee76c65158c149cdcb0b05e2c3b0a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. CÁC CHUẨN VÀ VẾT

Trong toàn bộ đoạn này K ký hiệu một trường.

### 1. Nhắc lại

Cho A là một đại số có bậc hữu hạn $ n $ trên K. Với mỗi $ x \in A $ ta ký hiệu bởi $ L_x $ ánh xạ tuyến tính $ a \mapsto xa $ từ A vào chính nó. Ta nhắc lại (III, p. 543) rằng vết của $ L_x $ được gọi là vết của x đối với A và được viết là $ \mathrm{Tr}_{A/K}(x) $; tương tự, định thức của $ L_x $ được gọi là chuẩn của x đối với A và được ký hiệu bởi $ N_{A/K}(x) $. Biệt thức của một dãy $ (x_1, ..., x_n) $ gồm n phần tử của A được định nghĩa là định thức $ D_{A/K}(x_1, ..., x_n) $ của ma trận $ (\mathrm{Tr}_{A/K}(x_i x_j))_{1 \leq i,j \leq n} $ (III, p. 549).

Cho K' là một mở rộng của K và cho $ A' = A_{(K')} $ là đại số K'-dẫn xuất từ A bằng phép chuyển qua vô hướng. Ta có các công thức

(1) $$
\mathrm{Tr}_{A'/K'}(1 \otimes x) = \mathrm{Tr}_{A/K}(x) . 1 , \quad N_{A'/K'}(1 \otimes x) = N_{A/K}(x) . 1
$$
với mọi $ x \in A $ (III, p. 544). Với mọi dãy $ (x_1, ..., x_n) $ các phần tử của A, ta có

(2) $$
D_{A'/K'}(1 \otimes x_1, ..., 1 \otimes x_n) = D_{A/K}(x_1, ..., x_n) . 1 ,
$$
suy ra từ công thức đầu tiên (1).

### 2. Chuẩn và vết trong các đại số étale

Cho A là một đại số étale có (bậc) $ n $ trên K. Theo định nghĩa, khi đó tồn tại một mở rộng L của K và các đồng cấu phân biệt $ u_1, ..., u_n $ của A vào L với các tính chất sau.

a) mọi đồng cấu của $ A $ vào $ L $ đều bằng một trong các $ u_i $ (V, p. 29, Hệ quả);
b) tồn tại một đẳng cấu đại số $ u : A_{(L)} \to L^n $ sao cho

$$
u(1 \otimes x) = (u_1(x), \ldots, u_n(x)) \quad \text{với mọi } x \in A .
$$

Hơn nữa, mọi mở rộng đóng đại số $ L $ của $ K $ đều có các tính chất trên (V, p. 30, Mệnh đề 2).

Trong phần sau, ta cố định $ L, u_1, \ldots, u_n $. Cho $ x \in A $; ta sẽ chứng minh các công thức

$$
\text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) , \quad \text{N}_{A/K}(x) \cdot 1 = \prod_{i=1}^n u_i(x) .
$$

Cho $ v $ là phép nhân bởi $ l \otimes x $ trong $ A_{(L)} $; xét theo cơ sở của $ A_{(L)} $ là ảnh qua $ u^{-1} $ của cơ sở chính tắc của $ L^n $, ma trận của ánh xạ tuyến tính $ v $ là đường chéo, với các phần tử đường chéo $ u_1(x), \ldots, u_n(x) $. Suy ra rằng

$$
Tr_{A_{(L)}/L}(1 \circ x) \cdot 1 = \sum_{r=1}^n u_i(x) , \quad \text{do đó} \quad \text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) \text{ theo (1)} ;
$$

trường hợp của chuẩn được xét tương tự.

Hơn nữa, cho $ (x,, \ldots, x,) $ là một dãy các phần tử của $ A $, cho U là ma trận

$$
(u_i(x_j))_{1 \leq i,j \leq n}
$$

và cho $ (t_{ij}) = 'U . U $. Theo công thức đầu tiên (3), ta có

$$
\text{Tr}_{A/K}(x_i x_j) \cdot 1 = \sum_{k=1}^n u_k(x_i x_j) = \sum_{k=1}^n u_k(x_i) u_k(x_j) = t_{ij} ;
$$

chuyển sang định thức, ta được

$$
D_{A/K}(x_1, \ldots, x_r) \cdot 1 = [\det u_i(x_j)]^2 .
$$

#### Mệnh đề 1 {#alg-v-s8-prop-1 .statement}

— *Cho $ A $ là một đại số giao hoán có bậc hữu hạn trên $ K $. Khi đó các điều kiện sau là tương đương*:
a) *Đại số $ A $ là étale.*
b) *Tồn tại một cơ sở của $ A $ có biệt thức khác không.*
c) *Với mỗi $ x \neq 0 $ trong $ A $, tồn tại $ y $ trong $ A $ sao cho $ \text{Tr}_{A/K}(xy) \neq 0 $.*
*Hơn nữa, khi các điều kiện này được thỏa mãn, biệt thức của bất kỳ cơ sở nào của $ A $ đều khác không.*

Ta sẽ chỉ ra rằng khi giả sử $ A $ là étale, thì biệt thức của $ A $ đối với bất kỳ cơ sở $ (x,, \ldots, x,) $ nào của $ A $ trên $ K $ đều khác không; điều này sẽ đặc biệt thiết lập suy ra $ a) \Rightarrow b) $. Theo (4), với ký hiệu ở trên, chỉ cần chỉ ra rằng ma trận U khả nghịch, hay tương đương, rằng hệ các phương trình tuyến tính

$$
\sum_{i=1}^n \lambda_i u_i(x_j) = 0 \quad (\text{cho } 1 \leq j \leq n)
$$

chỉ có nghiệm $ \lambda_1 = \cdots = A, = 0 $ trong L. Bây giờ từ quan hệ (5) suy ra $ \sum_{i=1}^n \lambda_i u_i(x) = 0 $ với mọi $ x \in A $, do đó $ \lambda_i = 0 $ với $ 1 \leq i \leq n $, theo định lý về tính độc lập tuyến tính của các đồng cấu (V, p. 27, Định lý 1).

Sự tương đương của b) và c) là hệ quả của bổ đề tổng quát sau:

#### Bổ đề 1 {#alg-v-s8-lem-1 .statement}

Cho V là một không gian vectơ có số chiều hữu hạn trên K và B là một *dạng song tuyến tính trên* V x V. Cho $(v_1, \ldots, v_n)$ *là một cơ sở của* V *trên* K *và* $ \Delta = \det B(v_i, v_j) $. Khi đó $ A \neq 0 $ khi và chỉ *khi*, với mỗi $ x \neq 0 $ trong V, tồn tại y trong V sao cho $ B(x, y) \neq 0 $.

Ta có $ A \neq 0 $ khi và chỉ khi hệ phương trình tuyến tính

$$
\sum_{i=1}^n \lambda_i B(v_i, v_j) = 0 \quad (1 \leq j \leq n)
$$

chỉ có nghiệm $ A, = \cdots = A, = 0 $ trong K. Nếu đặt $ x = \sum_{i=1}^n \lambda_i v_i $, thì hệ trên tương đương với $ B(x, v_j) = 0 $ cho $ 1 \leq j \leq n $, hay cũng vậy, vì $(v_1, \ldots, v_n)$ là một cơ sở của V trên K, với $ B(x, y) = 0 $ với mọi $ y \in V $, do đó suy ra bổ đề.

Ta sẽ chứng minh rằng điều kiện c) suy ra rằng A là một vành không có phần tử lũy linh khác 0. Cho x là một phần tử lũy linh của A : với mọi $ y \in A $ thì phần tử xy là lũy linh, và do đó tự đồng cấu $ L_{xy} $ của không gian vectơ A là lũy linh. Bổ đề sau suy ra rằng $ \mathrm{Tr}(xy) = 0 $ với mọi $ y \in A $, do đó $ x = 0 $ dưới giả thiết c).

#### Bổ đề 2 {#alg-v-s8-lem-2 .statement}

Cho V là một không gian vectơ có số chiều hữu hạn trên K và $ u $ là một tự đồng cấu lũy linh của V, khi đó $ \mathrm{Tr}(u) = 0 $.

Với mỗi số nguyên $ n \geq 0 $ đặt $ V_n $ là ảnh của $ u^n $. Vì $ u $ lũy linh, tồn tại một số nguyên $ r \geq 0 $ sao cho $ V_0 = V, V_r = 0 $ và $ V_i \neq V_{i+1} $ với $ 0 \leq i < r - 1 $. Gọi d, là số chiều của $ V_{i-1} $ (với $ 1 \leq i \leq r $). Tồn tại một cơ sở $(x,, \ldots, x_d)$ của V sao cho các vectơ $ x_j $ với $ d - d_i < j \leq d $ lập thành một cơ sở của $ V_{i-1} $ (với $ 1 \leq i \leq r $). Ta có $ u(V_{i-1}) \subset V_i $ và do đó các phần tử trên đường chéo của ma trận của $ u $ đối với cơ sở $(x,, \ldots, x,) $ đều bằng không. Vậy ta có $ \mathrm{Tr}(u) = 0 $ và bổ đề được chứng minh.

Sau cùng ta chứng minh rằng b) suy ra a). Cho $(x,, \ldots, x_n)$ là một cơ sở của A trên K sao cho $ D_{A/K}(x_1, \ldots, x_n) \neq 0 $. Cho K' là một mở rộng của K, A' là K'-đại số thu được từ A bằng mở rộng vô hướng và $ x'_i = 1 \otimes x_i $ với $ 1 \leq i \leq n $. Theo Công thức (2) (V, p. 47) ta có $ D_{A'/K'}(x'_1, \ldots, x'_n) \neq 0 $. Áp dụng kết quả trước cho A' ta thấy A' là reduced, do đó đại số A là étale (V, p. 34, Định lý 4).

#### Hệ quả {#alg-v-s8-n2-cor-1 .statement}

— Cho E là một mở rộng *có bậc hữu hạn* của K. Để E tách được thì điều kiện cần và đủ là tồn tại a trong E sao cho $ \mathrm{Tr}_{E/K}(a) \neq 0 $.

Điều kiện ấy là cần thiết theo Mệnh đề 1. Ngược lại, giả sử rằng tồn tại $ a \in E $ sao cho $ \mathrm{Tr}_{E/K}(a) \neq 0 $. Cho $ x \neq 0 $ trong E, nếu đặt $ y = a x' $, thì $ \mathrm{Tr}_{E/K}(xy) \neq 0 $. Nay Mệnh đề 1 cho thấy E là một đại số étale trên K, do đó là một mở rộng tách được của K.

### 3. Chuẩn và vết trong các mở rộng bậc hữu hạn

Các công thức về tính bắc cầu trong các đại số (III, p. 548) suy ra mệnh đề sau trong trường hợp các mở rộng bậc hữu hạn.

#### Mệnh đề 2 {#alg-v-s8-prop-2 .statement}

— Cho F là một mở rộng bậc hữu hạn của K và E là một mở rộng trung gian của F. Khi đó với mọi $ x \in F $ ta có
$$
\text{Tr}_{F/K}(x) = \text{Tr}_{E/K}(\text{Tr}_{F/E}(x)) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(\text{N}_{F/E}(x)) .
$$

#### Hệ quả {#alg-v-s8-n3-cor-1 .statement}

==========

— Đặt $ m = [F : E] $; khi đó với mọi $ x \in E $ ta có
$$
\text{Tr}_{F/K}(x) = m \cdot \text{Tr}_{E/K}(x) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(x)^m .
$$

#### Mệnh đề 3 {#alg-v-s8-prop-3 .statement}

— Cho E là một mở rộng bậc hữu hạn n của K và x là một phần tử của E, có bậc d trên K. Viết $ f(X) = X^d + \sum_{i=1}^d a_i X^{d-i} $ cho đa thức tối tiểu của X trên K. Khi đó ta có
$$
\text{Tr}_{E/K}(x) = - \frac{n}{d} a_1 \\
\text{N}_{E/K}(x) = (((-1)^d a_d)^{n/d} = (-1)^n a_d^{n/d} .
$$

Mệnh đề 3 suy ra trực tiếp từ Hệ quả của Mệnh đề 2 và bổ đề:

#### Bổ đề 3 {#alg-v-s8-lem-3 .statement}

Cho R là một vành giao hoán, $ f(X) = X^d + \sum_{i=1}^d a_i X^{d-i} $ là một đa thức đơn khởi của $ \mathbf{R}[X] $, A là đại số trên R $ \mathbf{R}[X]/(f) $ và x là lớp thặng dư của X trong A. Khi đó $ \text{Tr}_{A/R}(x) = -a_1 $ và $ \text{N}_{A/R}(x) = (-1)^d a_d $.

Theo Hệ quả (IV, p. 11) dãy $ (1, x, ..., x^{d-1}) $ là một cơ sở của A; hơn nữa ta có
$$
x \cdot 1 = x , \quad x \cdot x = x^2 , \ldots , x \cdot x^{d-2} = x^{d-1} ,
$$
$$
x \cdot x^{d-1} = -a_d \cdot 1 - a_{d-1} \cdot x - \ldots - a_1 \cdot x^{d-1}
$$

Ma trận biểu diễn phép nhân với x theo cơ sở $ (1, x, ..., x^{d-1}) $ của $ A $ có dạng sau (ta lấy $ d = 5 $ để cố định ý tưởng):

$$
\begin{pmatrix}
0 & 0 & 0 & 0 & -a \\
1 & 0 & 0 & 0 & -a \\
0 & 1 & 0 & 0 & -a_3 \\
0 & 0 & 1 & 0 & -a_2 \\
0 & 0 & 0 & 1 & -a_1
\end{pmatrix}
$$

Vết của ma trận này rõ ràng là $ -a $; định thức có thể được tính bằng cách khai triển theo hàng thứ nhất, và khi đó ta tìm được

$$
(-1)^{d-1} (-a_d) = (-1)^d a_d .
$$

Trong phần còn lại của số này, ta ký hiệu E là một mở rộng bậc hữu hạn của K và $ x $ là một phần tử của E. Chúng tôi sẽ chỉ ra cách tính chuẩn và vết của $ x $ trong các trường hợp khác nhau.

$ a) $ *Trường hợp của một mở rộng tách được*: giả sử E là tách được bậc $ n $ trên K, ký hiệu $ \Omega $ là một bao đóng đại số của K và $ \sigma_1, \ldots, \sigma_n $ là $ n $ đồng cấu K phân biệt của E vào R. Theo Công thức (3) ($ V $, p. 48) ta có trong R

$$
\text{Tr}_{E/K}(x) = \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \prod_{i=1}^n \sigma_i(x) .
$$

$ b) $ *Trường hợp của một mở rộng p-căn*: giả sử K có đặc số $ p > 0 $ và mở rộng E là p-căn; tồn tại một số nguyên $ e \geq 0 $ sao cho $[E:K] = p^e$ ($ V $, p. 26, Mệnh đề 4). Nếu $ f $ là bậc của x trên K, đa thức tối tiểu của x trên K là $ X^{p^f} - x^{p^f} $ ($ V $, p. 24, Mệnh đề 1). Theo Mệnh đề 3 ta có $ N_{E/K}(x) = (x^{p^f})^{p^e/p^f} $, do đó

$$
N_{E/K}(x) = x^{p^e} = x^{[E:K]}
$$

Với vết ta được $ \text{Tr}_{E/K}(x) = -p^{e-f} a $, trong đó $ a $ là hệ số của $ X^{p^f-1} $ trong đa thức $ X^{p^f} - x^{p^f} $; nói cách khác, ta có

$$
\text{Tr}_{E/K}(x) = p^e \cdot x = [E:K] x = \begin{cases} x & \text{nếu } [E:K] = 1 \\ 0 & \text{nếu } [E:K] > 1 . \end{cases}
$$

$ c) $ *Trường hợp tổng quát*: ta có thể tóm tắt việc tính chuẩn và vết trong mệnh đề sau:

#### Mệnh đề 4 {#alg-v-s8-prop-4 .statement}

*Cho p là số mũ đặc trưng của K và E là một mở rộng bậc hữu hạn của K. Cho $ \sigma_1, \ldots, \sigma_n $ là các đồng cấu K phân biệt của E vào một bao đóng đại số $ \Omega $ của K, và cho $ p^e = [E:K]_i $. Với mỗi $ x \in E $ ta có trong $ \Omega $*

$$
\text{Tr}_{E/K}(x) = p^e \cdot \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \left( \prod_{i=1}^n \sigma_i(x) \right)^{p^e} .
$$

Cho E, là bao đóng tách được tương đối của K trong E; khi đó $ E_s $ là một mở rộng tách được bậc $ n $ của K và $ \sigma_1, \ldots, \sigma_n $ cảm sinh các đồng cấu K phân biệt của E, vào R; hơn nữa, E là một mở rộng p-căn của E, bậc p$^e$ ($ V $, p. 44, Mệnh đề 13 và p. 46). Do đó Mệnh đề 4 suy ra từ các Công thức (6), (7), (13), (14) và (12).

### Bài tập {#alg-v-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
