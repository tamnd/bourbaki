---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 5
section_title: Endomorphisms of vector spaces
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.70-A VII.72
pdf_pages: 0387-0407, 0429-0431
extraction: ocr
subsections:
    - "no": 1
      title: The module associated to an endomorphism
      page: 28
      pdf_page: 387
    - "no": 2
      title: Eigenvalues and eigenvectors
      page: 30
      pdf_page: 389
    - "no": 3
      title: Similarity invariants of an endomorphism
      page: 31
      pdf_page: 390
    - "no": 4
      title: Triangularisable endomorphisms
      page: 34
      pdf_page: 393
    - "no": 5
      title: 'Properties of the characteristic polynomial : trace and determinant'
      page: 36
      pdf_page: 395
    - "no": 6
      title: Characteristic polynomial of the tensor product of two endomorphisms
      page: 39
      pdf_page: 398
    - "no": 7
      title: Diagonalisable endomorphisms
      page: 40
      pdf_page: 399
    - "no": 8
      title: Semi-simple and absolutely semi-simple endomorphisms
      page: 41
      pdf_page: 400
    - "no": 9
      title: Jordan decomposition
      page: 43
      pdf_page: 402
statements: 63
exercises: 14
content_sha256: ab04544569550a7c0c69d30c90196882c9a1ce94bd99492770c5aadea7683534
translated_from: content/en/alg/VII/05_s5_endomorphisms_of_vector_spaces.md
source_content_sha256: 635a24ee64712856e67649e040727e1324e7905c74a103aed09b4ef59c6e8359
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-dd92adee
glossary_version: 34
glossary_terms_sha256: 2bb011ede861d22ac98802ec342507b3998f59c61f06d7d14601a0fc0a158aff
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. TỰ ĐỒNG CẤU CỦA CÁC KHÔNG GIAN VECTƠ

Ký hiệu. — Cho một môđun $ M $, một phần tử $ x $ của $ M $, và hai tự đồng cấu $ u $ và $ v $ của $ M $, ta sẽ viết $ u.x $, $ uv.x $ và $ uv $ thay cho $ u(x) $, $ (u \circ v)(x) $ và $ u \circ v $ tương ứng; ta sẽ ký hiệu ánh xạ đồng nhất từ $ M $ vào chính nó bởi 1 khi không thể gây nhầm lẫn.

### 1. Môđun liên kết với một tự đồng cấu

Cho $ A $ là một vành giao hoán, cho $ M $ là một $ A $-môđun, và cho $ u $ là một $ A $-tự đồng cấu của $ M $. Nhắc lại (III, p. 538) rằng ánh xạ $ (p(X), x) \mapsto p(u).x $ từ $ A[X] \times M $ vào $ M $ làm cho $ M $ trở thành một $ A[X] $-môđun, được viết là $ M_u $. Cũng nhắc lại (III, pp. 538 and 539) rằng nếu $ M[X] $ ký hiệu $ A[X] $-môđun thu được từ $ M $ bởi mở rộng vô hướng từ $ \mathbf{A} $ đến $ \mathbf{A}[X] $, và nếu $ \bar{u} $ ký hiệu $ \mathbf{A}[X] $-tự đồng cấu của $ M[X] $ cảm sinh bởi $ u $, thì tồn tại một dãy khớp của các $ \mathbf{A}[XI]$-môđun $ ^1 $

$$
(1) \quad 0 \to M[X] \xrightarrow{\psi} M[X] \xrightarrow{\varphi} M_u \to 0 ,
$$

trong đó $ \varphi(p(X) \otimes x) = p(u).x $ và $ \psi = X - \bar{u} $.

Một tự đồng cấu $ u $ của một $ \mathbf{A}$-môđun $ M $ và một tự đồng cấu $ u' $ của một $ \mathbf{A}$-môđun $ M' $ được gọi là tương tự nếu tồn tại một đẳng cấu $ g $ từ $ M $ lên $ M' $ sao cho $ u' \circ g = g \circ u $, nghĩa là (III, p. 540, Mệnh đề 19) một đẳng cấu $ g $ từ $ M_u $ lên $ M_{u'} $. Nếu $ M $ (tương ứng $ M' $) là tự do trên cơ sở hữu hạn $ B $ (tương ứng $ B' $), và nếu $ M(u) $ (tương ứng $ M(u') $) là ma trận của $ u $ (tương ứng $ u' $) đối với $ B $ (tương ứng $ B' $), thì $ u $ và $ u' $ tương tự khi và chỉ khi $ M(u) $ và $ M(u') $ là các ma trận tương tự (II, p. 356, Định nghĩa 6). Các đa thức đặc số (III, p. 541, Định nghĩa 3) của hai tự đồng cấu tương tự của các môđun tự do sinh hữu hạn là bằng nhau (III, p. 540, Mệnh đề 19).

Cho $ K $ là một trường giao hoán ; khi đó mọi cặp $ (E, u) $ gồm một không gian vectơ $ E $ trên $ K $ và một tự đồng cấu $ u $ của $ E $ tương ứng với một $ K[X] $-môđun $ E_{,,} $. Vì vành $ K[X] $ là một miền iđêan chính (IV, p. 11, Mệnh đề 11), các kết quả của các phần trước có thể được áp dụng cho $ E_{,,} $.

Trước hết ta chỉ ra cách chuyển một số khái niệm từ ngôn ngữ của các môđun sang ngôn ngữ của các tự đồng cấu của các không gian vectơ :

« $ V $ là một môđun con của $ E $, » có nghĩa là : « $ V $ là một không gian con vectơ của $ E $ đóng đối với $ u $ ».

« $ V $ là một môđun con xyclic của $ E $, » có nghĩa là : « tồn tại $ x \in V $ sao cho không gian con vectơ $ V $ được sinh bởi các phần tử $ u^i . x \ (i \in \mathbf{N}) $ ». Khi đó $ V $ được gọi là xyclic (đối với $ u $) và $ x $ được gọi là một phần tử sinh.

« $ V $ là một môđun con không phân tích được của $ E $, » có nghĩa là : « $ V $ khác không và không là tổng trực tiếp của hai không gian con khác không mỗi không gian đều đóng đối với $ u $ ».

« $ a $ là linh hóa tử của môđun con $ V $ » có nghĩa là : « $ a $ là iđêan gồm các đa thức $ p(X) \in K[X] $ sao cho $ p(u).x = 0 $ với mọi $ x \in V $ ».

Đa thức đơn khởi $ g $ sao cho $ a $ bằng iđêan chính $ (g) $ khi đó được gọi là đa thức tối tiểu của hạn chế của $ u $ lên $ V $.

« $ E_{,,} $ là xyclic với linh hóa tử $ a = (g) $ »

$$
\text{(với } g(X) = X^n + \alpha_{n-1} X^{n-1} + \cdots + \alpha_0 )
$$

$ ^1 $ Tính đơn ánh của $ \psi $, không được phát biểu trong Mệnh đề 18 của III, p. 539, được chứng minh như sau : theo ký hiệu của loc. cit., ta có

$$
\psi(\sum (X^k \otimes x_k)) = \sum X^k \otimes (x_{k-1} - u(x_k)) .
$$

Nếu $ \sum X^k \otimes x_k $ thuộc hạt nhân của $ \psi $, thì suy ra $ x_k , = u(x_k) $ với mọi $ k $, và các $ x_k $ đều bằng không, vì họ $ (x_k) $ có giá hữu hạn.

có nghĩa là : « tồn tại $ x \in E $ sao cho $ (u^i . x) $ ($ 0 \leq i \leq n - 1 $) là một cơ sở của không gian vectơ $ E $, và $ g(u).x = 0 $ ». Nói cách khác, ta có thể tìm một cơ sở của $ E $ sao cho ma trận $ U $ của $ u $ đối với cơ sở này là

$$
U = \begin{pmatrix}
0 & 0 & 0 \ldots 0 & -\alpha_0 \\
1 & 0 & 0 \ldots 0 & -\alpha_1 \\
0 & 1 & 0 \ldots 0 & -\alpha_2 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 \ldots 0 & -\alpha_{n-2} \\
0 & 0 & 0 \ldots 1 & -\alpha_{n-1}
\end{pmatrix}.
$$

« $ E $, là một môđun xoắn » có nghĩa là, theo đặc trưng hóa của các môđun xoắn xyclic được cho ở trên : « mọi môđun con xyclic của $ E $, đều hữu hạn chiều trên $ K $ ». Đặc biệt :

« $ E_u $ là một môđun xoắn sinh hữu hạn » có nghĩa là : « $ E $ hữu hạn chiều trên $ K $ ».

### 2. Trị riêng và vectơ riêng

#### Định nghĩa 1 {#alg-vii-s5-def-1 .statement}

*Cho $ E $ là một không gian vectơ trên một trường giao hoán $ K $, và $ u $ là một tự đồng cấu của $ E $. Một phần tử $ x $ của $ E $ được gọi là một vectơ riêng của $ u $ nếu tồn tại $ a \in K $ sao cho $ u . x = \alpha x $; nếu $ x \neq 0 $ thì vô hướng $ a $ được gọi là trị riêng của $ u $ tương ứng với vectơ riêng $ x $. Với mọi vô hướng $ a $, không gian con vectơ $ V_a $ gồm các $ x \in E $ sao cho $ u . x = \alpha x $ được gọi là không gian riêng của $ E $ tương ứng với $ a $.

Bội số hình học của trị riêng $ a $ là lực lượng $ \dim V_a $.

Giả sử $ E $ hữu hạn chiều. Các trị riêng của $ u $ là các phần tử $ a $ của $ K $ sao cho tự đồng cấu $ a . 1 - u $ của $ E $ không đơn ánh, nói cách khác (III, p. 524, Mệnh đề 3) sao cho $ \det(a . 1 - u) = 0 $. Nhưng, theo định nghĩa của đa thức đặc trưng $ \chi_u $ của $ u $ (III, p.541, Định nghĩa 3), ta có $ \det(a . 1 - u) = \chi_u(\alpha) $. Do đó :

#### Mệnh đề 1 {#alg-vii-s5-prop-1 .statement}

*Giả sử $ E $ là hữu hạn chiều. Khi đó một phần tử $ a $ của $ K $ là một trị riêng của tự đồng cấu $ u $ khi và chỉ khi nó là một nghiệm của đa thức đặc trưng của $ u $.

Nếu $ L $ là một mở rộng của trường $ K $, thì các nghiệm của $ \chi_u $ trong $ L $ là các trị riêng của tự đồng cấu $ 1, \otimes u $ của không gian vectơ $ L $-vectơ $ L \otimes_K E $. Chúng thường được gọi là *các trị riêng của $ u $ trong $ L $*. Do lạm dụng ngôn ngữ, ta nói rằng mọi trị riêng của $ u $ thuộc $ L $ nếu điều này đúng với mọi trị riêng của $ u $ trong một mở rộng đóng đại số của $ L $; điều này có nghĩa là $ \chi_u $ phân tích thành các nhân tử tuyến tính trong $ L[X] $.

Cho $ U $ là một ma trận bình phương cấp $ n $ với các hệ số trong $ K $. Khi đó theo định nghĩa đa thức đặc trưng của $ U $ là

$$
\chi_U(X) = \det(X . I, -U);
$$

các trị riêng của $ U $ (trong một mở rộng $ L $ của $ K $) là các nghiệm (trong $ L $) của đa thức $ \chi_U $; chúng cũng là các vô hướng $ a $ (trong $ L $) sao cho tồn tại một nghiệm khác không của hệ phương trình tuyến tính $ UX = \alpha X $, trong đó $ X $ là một ma trận cột cấp $ n $; một ma trận cột $ X $ thỏa mãn phương trình này được gọi là một vectơ riêng của $ U $ tương ứng với $ a $.

Nếu $ U $ là ma trận của một tự đồng cấu $ u $ của một không gian vectơ $ n $-chiều đối với một cơ sở $ B $, thì $ \chi_U = \chi_u $, các trị riêng của $ U $ là các trị riêng của $ u $, và các vectơ riêng của $ U $ là các ma trận của các vectơ riêng của $ u $ đối với cơ sở $ B $.

#### Mệnh đề 2 {#alg-vii-s5-prop-2 .statement}

*Cho $ u $ là một tự đồng cấu của một không gian vectơ $ E $ trên một trường giao hoán $ K $; với mỗi vô hướng $ a $, gọi $ V_a $ là không gian riêng tương ứng với $ a $. Khi đó các không gian con $ V_a $ đóng đối với $ u $ và tổng của các $ V_a $ là trực tiếp.*

Mệnh đề đầu tiên là hiển nhiên. Theo định nghĩa không gian con $ V_a $ bị triệt tiêu bởi phần tử $ X - a $ của $ K[X] $; các $ X - a, a \in K $ là bất khả quy và từng đôi một không liên hợp; do đó mệnh đề thứ hai suy ra từ VII, p. 8, Th. 1.

### 3. Các bất biến đồng dạng của một tự đồng cấu

Nếu ta dịch sự phân tích của một môđun xoắn sinh hữu hạn trong VII, p. 8, Th. 1 và p. 9, Mệnh đề 2, thì ta thu được:

#### Mệnh đề 3 {#alg-vii-s5-prop-3 .statement}

*Cho $ E $ là một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán $ K $, và cho $ u $ là một tự đồng cấu của $ E $; với mỗi đa thức đơn khởi bất khả quy $ p(X) $, cho $ M_p $ là không gian con vectơ gồm các phần tử $ x $ của $ E $ sao cho $ (p(u))^k \cdot x = 0 $ với một số nguyên $ k $. Khi đó $ M_p $ đóng dưới $ u $, không gian vectơ $ E $ là tổng trực tiếp của các $ M_p $, và tồn tại các đa thức $ s_p $ sao cho, với mọi $ x \in E $, thành phần của $ x $ trong $ M_p $ bằng $ s_p(u) \cdot x $.*

#### Nhận xét 1 {#alg-vii-s5-n3-rem-1 .statement}

Rõ ràng đa thức tối tiểu của hạn chế của $ u $ lên $ M_p $ là lũy thừa lớn nhất của $ p $ chia hết đa thức tối tiểu của $ u $. Hơn nữa ta có $ s_p(u) \cdot x = x $ với $ x \in M_p $, từ đó suy ra ngay lập tức rằng, nếu $ M_p \neq 0 $, thì $ s_p $ nguyên tố cùng nhau với $ p $.

Tương tự, theo Định lý 2 của VII, p. 19, môđun $ E_u $ đẳng cấu với một tổng trực tiếp của các môđun cyclic $ F_j = K[X]/a_j \ (1 \leq j \leq r) $, trong đó các iđêan $ a_j $ phân biệt với $ K[X] $ và $ a_j \subset a_{j+1} $; và các $ a_j $ được xác định bởi các điều kiện này. Hơn nữa, vì $ E $, là một môđun xoắn, ta có $ a_1 \neq (0) $; vì $ E $ có chiều $ n $, ta có $ r \leq n $. Đặt $ a_j = (h_j) \ (1 \leq j \leq r) $, với $ h_j $ là một đa thức đơn khởi, và xét dãy $ (q_i) \ (1 \leq i \leq n) $ gồm các đa thức được xác định bởi:

$$
\begin{cases}
q_i(X) = 1 & \text{nếu } i \leq n - r \\
q_i(X) = h_{n-i+1}(X) & \text{nếu } n - r < i \leq n .
\end{cases}
$$

Rõ ràng các đa thức $ q_i $ xác định các đa thức $ h_j $ và ngược lại, và $ E $, đẳng cấu với tổng trực tiếp của $ n $ môđun $ K[X]/(q_i) $, trong đó $ n - r $ môđun đầu tiên bằng $ 0 $.

Nói cách khác:

#### Mệnh đề 4 {#alg-vii-s5-prop-4 .statement}

— Cho E là một không gian vectơ hữu hạn chiều n trên một trường giao hoán K, và cho u là một tự đồng cấu của E. Khi đó tồn tại n đa thức monic $ q_i(X) \in K[X] $ ($ 1 \leq i \leq n $) sao cho $ q_i $ chia hết $ q_{i+1} $ với $ 1 \leq i \leq n-1 $, và E là tổng trực tiếp của n không gian con $ V_i $ ($ 1 \leq i \leq n $) đóng dưới tác động của u, xyclic (đối với u), và sao cho đa thức tối tiểu của hạn chế của u lên $ V_i $ bằng $ q_i $ ($ 1 \leq i \leq n $). Các đa thức $ q_i $ được xác định duy nhất bởi các điều kiện này, và $ q_n $ là đa thức tối tiểu q của u.

#### Nhận xét 2 {#alg-vii-s5-n3-rem-2 .statement}

Theo mệnh đề trên, tồn tại một cơ sở của E sao cho đối với cơ sở đó, ma trận U của u có dạng

$$
\begin{pmatrix}
A_{n-r+1} & 0 & \ldots & 0 & 0 \\
0 & A_{n-r+2} & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \ldots & A_{n-1} & 0 \\
0 & 0 & \ldots & 0 & A_n
\end{pmatrix}
$$

trong đó mỗi ma trận $ A_i $ có dạng (2) (lấy $ g(X) = q_i(X) $) (xem VII, p. 29-30).

#### Định nghĩa 2 {#alg-vii-s5-def-2 .statement}

— Với ký hiệu của Mệnh đề 4, n đa thức monic $ q_i(X) $ ($ 1 \leq i \leq n $) được gọi là các bất biến đồng dạng của tự đồng cấu u.

Do đó bất biến đồng dạng thứ n $ q_n $ là đa thức tối tiểu của u (Mệnh đề 4); nói cách khác, để một đa thức $ p(X) \in K[X] $ thỏa mãn $ p(u) = 0 $, điều kiện cần và đủ là $ p $ là một bội của $ q_n $.

#### Hệ quả 1 {#alg-vii-s5-def-2-cor-1 .statement}

— Cho K là một trường, cho E và $ E' $ là hai không gian vectơ hữu hạn chiều trên K, và cho u (tương ứng $ u' $) là một tự đồng cấu của E (tương ứng $ E' $). Khi đó u và $ u' $ đồng dạng (VII, tr. 29) khi và chỉ khi chúng có cùng các bất biến đồng dạng.

Thật vậy $ u $ và $ u' $ đồng dạng khi và chỉ khi các $ K[X] $-môđun E, và $ E'_u $ là đẳng cấu.

#### Hệ quả 2 {#alg-vii-s5-def-2-cor-2 .statement}

— Cho u là một tự đồng cấu của một không gian vectơ hữu hạn chiều E trên một trường K, cho $ (q_1, \ldots, q_n) $ là họ các bất biến đồng dạng của u, cho L là một mở rộng của K, cho $ E_{(L)} = L \otimes_K E $ là không gian vectơ L cảm sinh từ E bởi mở rộng vô hướng và cho $ u_{(L)} = 1_L \otimes u $ là tự đồng cấu của $ E_{(L)} $ cảm sinh bởi u. Khi đó các bất biến đồng dạng của $ u_{(L)} $ là các ảnh $ \bar{q}_1, \ldots, \bar{q}_n $ của $ q_1, \ldots, q_n $ trong $ L[X] $.

Điều này suy ra ngay lập tức từ Mệnh đề 4 và sự kiện rằng các $ L[X] $-môđun $ E_{(L)u_{(L)}} $ và $ (K[X]/(q_i))_{(L)} $ lần lượt đẳng cấu với $ L[X] \otimes_{K[X]} E_u $ và $ L[X]/(\bar{q}_i) $.

Cho U là một ma trận vuông cấp n với các hệ số trong một trường giao hoán K. Khi đó các bất biến đồng dạng của tự đồng cấu của $ K^n $ được xác định bởi U được gọi là các bất biến đồng dạng của $ U $. Khi đó suy ra từ Hệ quả 1 trên rằng hai ma trận vuông đồng dạng khi và chỉ khi chúng có cùng các bất biến đồng dạng, và rằng nếu $ u $ là một tự đồng cấu của một không gian vectơ hữu hạn chiều $ E $ trên $ K $, và $ U $ là ma trận của $ u $ đối với một cơ sở nào đó $ B $ của $ E $, thì các bất biến đồng dạng của $ U $ và $ u $ trùng nhau. Theo Hệ quả 1 và 2 trên, ta có:

#### Hệ quả 3 {#alg-vii-s5-def-2-cor-3 .statement}

— Cho $ U $ và $ V $ là hai ma trận vuông cấp $ n $ với các hệ số trong một trường giao hoán $ K $. Nếu tồn tại một ma trận vuông khả nghịch $ P $ trên một mở rộng $ K' $ nào đó của $ K $ sao cho $ V = P^{-1}UP $, thì tồn tại một ma trận vuông khả nghịch $ Q $ trên $ K $ sao cho $ V = Q^{-1}UQ $.

Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $, cho $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của $ E $ và cho $ u $ là một tự đồng cấu của $ E $. Khi đó theo dãy khớp (1) của VII, p. 29, $ K[X] $-môđun $ E $, liên kết với $ u $, là đẳng cấu với thương của $ K[X] $-môđun tự do $ E[X] $, với cơ sở $ (1 \otimes e_i) $, bởi ảnh của $ E[X] $ qua ánh xạ $ K[X] $-tuyến tính $ X - \bar{u} $. Các bất biến tương tự $ q_i(X) $ của $ u $ (VII, p. 32, Định nghĩa 2) do đó là các nhân tử bất biến của $ X - \bar{u} $ (VII, p. 22). Vì vậy Mệnh đề 6 của VII, p. 22, kéo theo:

#### Mệnh đề 5 {#alg-vii-s5-prop-5 .statement}

— Cho $ E $ là một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán $ K $, cho $ u $ là một tự đồng cấu của $ E $, và cho $ U $ là ma trận của nó đối với một cơ sở nào đó của $ E $. Khi đó với mỗi số nguyên $ m $ thỏa mãn $ 1 \leq m \leq n $, tích
$$
d_m(X) = q_1(X) q_2(X) \ldots q_m(X)
$$
của $ m $ bất biến tương tự đầu tiên của $ u $ bằng ước chung lớn nhất của các định thức con cấp $ m $ của ma trận $ XI, - U $.

#### Hệ quả 1 {#alg-vii-s5-prop-5-cor-1 .statement}

— Cho $ u $ là một tự đồng cấu của một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán $ K $, với đa thức đặc trưng $ \chi_u(X) $ và các bất biến tương tự $ q_i(X) $ ($ 1 \leq i \leq n $). Khi đó
$$
\chi_u(X) = q_1(X) q_2(X) \ldots q_n(X)
$$

#### Hệ quả 2 {#alg-vii-s5-prop-5-cor-2 .statement}

— Với ký hiệu của Hệ quả 1, cho $ q(X) $ là đa thức tối tiểu của $ u $; khi đó $ q(X) $ chia hết $ \chi_u(X) $ và $ \chi_u(X) $ chia hết $ q(X)^n $. Đặc biệt đa thức tối tiểu và đa thức đặc trưng của $ u $ có cùng các nghiệm, và đó là các giá trị riêng của $ u $.

Vì $ q(X) = q_n(X) $, rõ ràng là $ q(X) $ chia hết cho $ \chi_u(X) $. Mặt khác, vì mỗi $ q_i $ chia hết cho $ q $, tích của chúng $ \chi_u $ chia hết cho $ q^n $.

#### Hệ quả 3 {#alg-vii-s5-prop-5-cor-3 .statement}

— Một tự đồng cấu $ u $ là lũy linh khi và chỉ khi đa thức đặc trưng của nó có dạng $ X^n $.

Điều này suy ra ngay lập tức từ Hệ quả 2.

Bây giờ ta viết lại Mệnh đề 9 của VII, p. 24, cho phân tích của một môđun thành tổng trực tiếp của các môđun con không phân tích được.

#### Mệnh đề 6 {#alg-vii-s5-prop-6 .statement}

— Cho $ E $ là một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán $ K $, và cho $ u $ là một tự đồng cấu của $ E $. Khi đó $ E $ là tổng trực tiếp của các không gian con $ E_k $, đóng dưới $ u $ và cyclic đối với $ u $, sao cho đa thức tối tiểu của hạn chế của $ u $ lên $ E_k $ có dạng $ p_k^{n(k)} $, trong đó $ p_k $ là một đa thức bất khả quy, và $ E_k $ không thể biểu diễn thành tổng trực tiếp của hai không gian con khác không đều đóng dưới $ u $. Với mọi đa thức bất khả quy monic $ p \in K[X] $ và mọi số nguyên $ n \geq 1 $, số $ m(p^n) $ các không gian con $ E_k $ trong bất kỳ phân tích nào như vậy, sao cho $ p^n $ là đa thức tối tiểu của hạn chế của $ u $ lên $ E_k $, được xác định duy nhất.

Các $ p_k^{n(k)} $ xác định các bất biến đồng dạng của $ u $ và ngược lại; ta có thể chuyển từ cái này sang cái kia bằng thủ tục được giải thích trong VII, p. 25, Các chú ý 2 và 3. Hơn nữa, ta có thể ngay lập tức chuyển từ phân tích được xét trong Mệnh đề 6 sang các phân tích được xét trong Mệnh đề 3 và 4.

Chú ý rằng các đa thức bất khả quy monic $ p \in K[X] $ sao cho $ m(p^n) > 0 $ với một số nguyên $ n \geq 1 $ nào đó chính xác là các nhân tử bất khả quy monic của đa thức tối tiểu của $ u $. Như vậy, trái với các bất biến đồng dạng, các đa thức này nói chung phụ thuộc vào trường $ K $ mà ta đang làm việc.

### 4. Các tự đồng cấu tam giác hoá được

Trong tiết diện này ta sẽ quan tâm đến trường hợp trong đó đa thức tối tiểu $ p(X) $ của $ u $ phân tích thành tích của các nhân tử tuyến tính trong $ K[X] $, nói cách khác (VII, p. 33, Hệ quả 2) là trường hợp trong đó tất cả các trị riêng của $ u $ đều thuộc $ K $. Điều này đặc biệt đúng khi $ K $ là đóng đại số. Mệnh đề 3 của VII, p. 31 cho ngay lập tức:

#### Mệnh đề 7 {#alg-vii-s5-prop-7 .statement}

— Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $, và cho $ u $ là một tự đồng cấu của $ E $ mà tất cả các trị riêng của nó đều thuộc $ K $. Với mỗi trị riêng $ a $ của $ u $, cho $ M_a $ là không gian con vectơ của $ E $ gồm các phần tử $ x $ sao cho tồn tại một số nguyên $ k \geq 1 $ thỏa mãn $ (u - a)^k \cdot x = 0 $. Khi đó $ M_a $ đóng đối với $ u $, không gian vectơ $ E $ là tổng của các $ M_a $, và tồn tại các đa thức $ s_a \in K[X] $ sao cho, với mọi $ x \in E $, thành phần của $ x $ trong $ M_a $ bằng $ s_a(u) \cdot x $.

Môđun con $ M_a $, vì được sinh hữu hạn như một $ K[X] $-môđun, khi đó có một linh hóa tử có dạng $ (X - a)' $; nói cách khác, tồn tại một số nguyên $ r \geq 1 $ sao cho
$$
(u - a)^r \cdot x = 0
$$
với mọi $ x \in M_a $; hạn chế của $ u - a $ lên $ M_a $ là một tự đồng cấu lũy linh.

Vẫn giả sử rằng các trị riêng của $ u $ thuộc $ K $, ta áp dụng Mệnh đề 6 của VII, p. 34 cho $ u $. Các đa thức $ p_k $ không gì khác hơn là các $ X - a $ (khi $ a $ chạy qua tập hợp các trị riêng của $ u $), và ta thấy rằng $ E $ là tổng trực tiếp của các không gian con $ E_i $ đóng đối với $ u $, cyclic (đối với $ u $), và sao cho đa thức tối tiểu của hạn chế của $ u $ lên $ E_i $ có dạng $ (X - a)^m $. Gọi $ E_i' $ là $ K[X] $-môđun liên kết với $ E_i $; khi đó $ E_i' $ đẳng cấu với một trong các môđun $ K[X]/((X - a)^m) $. Bây giờ các lớp thặng dư mod $ (X - a)^m $ của các phần tử $ (X - \alpha)^k $ ($ 0 \leq k \leq m - 1 $) tạo thành một cơ sở $ K $ của $ K[X]/((X - a)^m) $ (IV, p. 11, Hệ quả), và

$$
X(X - \alpha)^k = \alpha (X - \alpha)^k + (X - \alpha)^{k+1}
$$

cho $ 0 \leq k \leq m - 1 $; suy ra rằng $ E_i $ có chiều $ m $, và nếu $ a $ là trị riêng duy nhất của hạn chế $ u_i $ của $ u $ trên $ E_i $, thì tồn tại một cơ sở của $ E_i $ sao cho ma trận của $ u_i $ đối với cơ sở đó là ma trận $ m \times m $

$$
U_{m,\alpha} = \begin{pmatrix}
\alpha & 0 & 0 & \ldots & 0 & 0 \\
1 & \alpha & 0 & \ldots & 0 & 0 \\
0 & 1 & \alpha & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 & \ldots & \alpha & 0 \\
0 & 0 & 0 & \ldots & 1 & \alpha
\end{pmatrix}
$$

#### Định nghĩa 3 {#alg-vii-s5-def-3 .statement}

*Với mọi trường $ K $, mọi số nguyên $ m \geq 1 $, và mọi $ a \in K $, ma trận $ U_{m,\alpha} $ được gọi là ma trận Jordan cấp $ m $ và trị riêng $ a $.*

#### Mệnh đề 8 {#alg-vii-s5-prop-8 .statement}

*Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $, và cho $ u $ là một tự đồng cấu của $ E $. Khi đó các điều kiện sau là tương đương*:

(i) *các trị riêng của $ u $ (trong một mở rộng đóng đại số nào đó của $ K $) thuộc về $ K $*;

(ii) *tồn tại một cơ sở của $ E $ sao cho ma trận của $ u $ đối với cơ sở đó là tam giác dưới (tương ứng tam giác trên)*;

(iii) *tồn tại một cơ sở của $ E $ sao cho ma trận của $ u $ đối với cơ sở đó là một khối đường chéo của các ma trận Jordan*.

Ta có (i) $ \Rightarrow $ (iii) theo Mệnh đề 7 và các nhận xét ở trên, và các khẳng định (iii) $ \Rightarrow $ (ii) và (ii) $ \Rightarrow $ (i) là tầm thường.

#### Định nghĩa 4 {#alg-vii-s5-def-4 .statement}

*Một tự đồng cấu thỏa mãn các điều kiện (i), (ii) và (iii) của Mệnh đề 8 được gọi là tam giác hóa được.*

Đặc biệt, nếu $ K $ là đóng đại số, thì mọi tự đồng cấu của một không gian vectơ $ K $ đều tam giác hóa được.

Đối với các ma trận, Mệnh đề 8 suy ra:

#### Hệ quả {#alg-vii-s5-n4-cor-1 .statement}

*Cho $ U $ là một ma trận bình phương trên một trường giao hoán $ K $ sao cho tất cả các trị riêng của $ U $ đều nằm trong $ K $; khi đó tồn tại một ma trận tương tự với $ U $ là một khối đường chéo của các ma trận Jordan.*

#### Nhận xét {#alg-vii-s5-n4-rem-1 .statement}

— 1) Từ Mệnh đề 6 của VII, p. 34, suy ra rằng, nếu $ U $ tương tự với một khối đường chéo của các ma trận Jordan $ (J_k) $, thì số các $ J_k $ có dạng $ U_{m,\alpha} $ (với $ m $ và $ \alpha $ đã cho) được xác định duy nhất bởi $ U $.

2) Tổng quát hơn, nếu $ U $ tương tự với một khối đường chéo của các ma trận Jordan $ U_{m_i, \alpha_i} $, thì các bất biến tương tự của $ U $ có thể được tính dễ dàng bằng một phương pháp mô phỏng theo phương pháp được trình bày trong VII, p. 25, Nhận xét 3 : viết tất cả các $ (X - \alpha_i)^{m_i} $ có cùng $ \alpha $ trên cùng một dòng, theo thứ tự giảm của các số mũ, và bổ sung bằng các 1 để có các dòng có độ dài bằng cấp của $ U $; khi đã làm điều này, các bất biến tương tự của $ U $ thu được, theo thứ tự giảm của các chỉ số, bằng cách lập các tích của các số hạng trong cùng một cột. Ví dụ, đối với ma trận

$$
\begin{pmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 1 & 3
\end{pmatrix}
$$

ta viết

$$
(X - 2), 1, 1 \\
(X - 3)^2, 1, 1
$$

và các bất biến tương tự là 1, 1 và $ (X - 2)\ (X - 3)' $

Bằng cách nhận thấy rằng đa thức tối tiểu của ma trận Jordan $ U_{m, \alpha} $ là $ (X - a)'' $, và rằng nó bằng đa thức đặc trưng của nó, ta thu được kết quả sau :

#### Mệnh đề 9 {#alg-vii-s5-prop-9 .statement}

— *Nếu ma trận vuông $ U $ tương tự với một khối chéo của các ma trận Jordan $ (U_{m_i, \alpha_i}) $, thì đa thức tối tiểu của $ U $ là bội chung nhỏ nhất của các $ (X - \alpha_i)^{m_i} $, và đa thức đặc trưng là tích của các $ (X - a_i)''' $.*

#### Hệ quả {#alg-vii-s5-n4-cor-2 .statement}

— *Trong ký hiệu của Mệnh đề 7, chiều của không gian con $ M_\alpha $ là bội số của trị riêng $ \alpha $ như một nghiệm của đa thức đặc trưng của $ u $.*

### 5. Các tính chất của đa thức đặc trưng : vết và định thức

Cho E là một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán K, và cho $ u $ là một tự đồng cấu của E. Theo III, p. 541, đa thức đặc trưng của $ u $ có dạng :

(5)
$$
\chi_u(X) = X^n - \mathrm{Tr}(u)\ X^{n-1} + \cdots + (-1)^n \det(u)\ .
$$

#### Mệnh đề 10 {#alg-vii-s5-prop-10 .statement}

— *Cho $ E $ là một không gian vectơ có số chiều hữu hạn $ n $ trên một trường giao hoán $ K $, cho $ u $ là một tự đồng cấu của $ E $, và cho $ \chi_u(X) = \prod_{i=1}^n (X - \alpha_i) $ là một phân tích thành các thừa số tuyến tính của đa thức đặc trưng của nó (trong một mở rộng thích hợp của $ K $, cf. V, p. 21). Nếu $ q $ là một đa thức với các hệ số trong $ K $, thì đa thức đặc trưng của $ q(u) $ được cho bởi*

(6)
$$
\chi_{q(u)}(X) = \prod_{i=1}^n (X - q(\alpha_i))\ ,
$$

và vết cùng định thức của nó được cho bởi

(7) $$
\operatorname{Tr}(q(u)) = \sum_{i=1}^n q(\alpha_i),
$$
(8) $$
\det(q(u)) = \prod_{i=1}^n q(\alpha_i).
$$

Hiển nhiên rằng (7) và (8) suy ra từ (6) nhờ vào (5). Để chứng minh công thức (6), ta có thể giả sử rằng K là đóng đại số. Khi đó ta lấy một cơ sở của E sao cho ma trận $ U $ của $ u $ là tam giác dưới ($ VII $, p. 35, Hệ quả của Mệnh đề 8); ta sẽ sử dụng bổ đề dễ dàng sau:

#### Bổ đề 1 {#alg-vii-s5-lem-1 .statement}

*Nếu B và C là các ma trận tam giác dưới cấp n với các đường chéo $ (\beta_i) $ và $ (\gamma_i) $, thì các ma trận $ B + C $ và $ BC $ là các ma trận tam giác dưới với các đường chéo $ (\beta_i + \gamma_i) $ và $ (\beta_i \gamma_i) $.*

Vì ma trận $ U $ của $ u $ là tam giác dưới với đường chéo $ (\alpha_i) $ nào đó, nên từ Bổ đề 1 suy ra rằng $ q(U) $ là một ma trận tam giác dưới với đường chéo $ (q(\alpha_i)) $. Khi đó $ X . I, -q(U) $ là một ma trận tam giác dưới với đường chéo $ (X - q(a;)) $, điều này chứng minh (6).

#### Hệ quả 1 {#alg-vii-s5-lem-1-cor-1 .statement}

*Để $ q(u) $ khả nghịch, điều kiện cần và đủ là $ q $ nguyên tố cùng nhau với $ \chi_u $.*

Thật vậy, nói rằng $ q $ và $ \chi_u $ nguyên tố cùng nhau tương đương với nói rằng chúng không có nghiệm chung trong một mở rộng đóng đại số của K, hay nói cách khác (8) là $ \det(q(u)) \neq 0 $.

#### Nhận xét 1 {#alg-vii-s5-n5-rem-1 .statement}

— Một đa thức nguyên tố cùng nhau với $ \chi_u $ khi và chỉ khi nó nguyên tố cùng nhau với đa thức tối tiểu của $ u $ (VII, p. 33, Hệ quả 2).

#### Hệ quả 2 {#alg-vii-s5-lem-1-cor-2 .statement}

*Cho $ r \in K(X) $ là một hàm hữu tỉ trên K. Khi đó $ u $ thế được (IV, p. 21) trong $ r $ khi và chỉ khi mỗi trị riêng của nó là thế được. Trong trường hợp này các công thức sau đúng:*

$$
\chi_{r(u)}(X) = \prod_{i=1}^n (X - r(\alpha_i)), \quad \operatorname{Tr}(r(u)) = \sum_{i=1}^n r(\alpha_i), \quad \det(r(u)) = \prod_{i=1}^n r(\alpha_i).
$$

Viết $ r = p/q $ trong đó $ p $ và $ q $ là các đa thức nguyên tố cùng nhau. Khi đó $ u $ thế được vào $ r $ khi và chỉ khi $ \det(q(u)) \neq 0 $, do đó khẳng định thứ nhất suy ra từ (8). Theo Hệ quả 1, ta có thể giả sử $ q $ nguyên tố cùng nhau với $ \chi_u $, do đó theo đồng nhất thức Bezout tồn tại các đa thức $ g $ và $ h $ sao cho $ qg + h\chi_u = 1 $. Khi đó $ q(\alpha_i)g(\alpha_i) = 1 $ và $ q(u)g(u) = 1 $ theo định lý Cayley-Hamilton (III, p. 541). Các công thức đã nêu khi đó thu được bằng cách áp dụng các công thức (6), (7) và (8) vào $ p(u)\ g(u) = r(u) $.

#### Hệ quả 3 {#alg-vii-s5-lem-1-cor-3 .statement}

*Với mỗi số nguyên $ s \geq 0 $ ta có $ \operatorname{Tr}(u^s) = \sum_{i=1}^n \alpha_i^s $. Công thức này cũng đúng với $ s < 0 $ miễn là $ u $ khả nghịch.*

Đây là trường hợp đặc biệt của hệ quả trước.

#### Hệ quả 4 {#alg-vii-s5-lem-1-cor-4 .statement}

— *Giả sử trường K có đặc số không; khi đó tự đồng cấu u là lũy linh khi và chỉ khi* $ \operatorname{Tr}(u^s) = 0 $ *với* $ 1 \leq s \leq n $.

Nếu $ u $ lũy linh thì các $ a_i $ đều bằng không, và $ \operatorname{Tr}(u^s) = 0 $ với mọi $ s > 0 $ (Hệ quả 3). Ngược lại, nếu $ \operatorname{Tr}(u^s) = 0 $ với $ 1 \leq s \leq n $, thì các $ a_i $ đều bằng không vì $ K $ có đặc số không (IV, p. 72, Hệ quả), và $ u $ là lũy linh (VII, p. 33).

#### Hệ quả 5 {#alg-vii-s5-lem-1-cor-5 .statement}

— *Cho Y là một bất định và gọi $ \tilde{u} $ là tự đồng cấu của không gian vectơ $ K(Y) $-vectơ $ K(Y) \otimes_K E $ cảm sinh từ $ u $ bởi mở rộng vô hướng từ $ K $ đến trường $ K(Y) $ của các hàm hữu tỉ theo $ Y $ với các hệ số trong $ K $. Khi đó tự đồng cấu $ Y \cdot 1 - \tilde{u} $ là khả nghịch. Hơn nữa, nếu $ \chi_u' $ ký hiệu đạo hàm của đa thức $ \chi_u $, thì*

$$
\operatorname{Tr}((Y \cdot 1 - \tilde{u})^{-1}) = \chi_u'(Y)/\chi_u(Y) .
$$

Tự đồng cấu $ Y \cdot 1 - \tilde{u} $ là khả nghịch vì định thức của nó là phần tử khác không $ \chi_u(Y) $ của $ K(Y) $. Suy ra $ \tilde{u} $ thế được vào hàm hữu tỉ $ r(X) = (Y - X)^{-1} $ trong $ K(Y)(X) $. Khẳng định thứ hai bây giờ suy ra từ Hệ quả 2, bởi quan hệ

$$
\chi_u'(Y)/\chi_u(Y) = \sum_i (Y - \alpha_i)^{-1} = \sum_i r(\alpha_i) .
$$

#### Hệ quả 6 {#alg-vii-s5-lem-1-cor-6 .statement}

— *Giả sử trường K có đặc số không. Khi đó, trong vành $ K[[T]] $ của các chuỗi lũy thừa hình thức, ta có*

$$
- T \frac{d}{dT} \log \det(1 - Tu) = \sum_{m \geq 1} \operatorname{Tr}(u^m) T^m
$$

Trước hết ta làm việc trong trường $ K(T) $ của các hàm hữu tỉ, và đặt $ P(T) = \det(I, -T \cdot U) $, trong đó $ U $ là ma trận của $ u $ đối với một cơ sở nào đó của $ E $. Khi đó

$$
P(T) = \det(T(T^{-1} \cdot I, -U)) = T^n \chi_U(T^{-1}) ,
$$

do đó $ P'(T)/P(T) = n/T - \chi_u'(T^{-1})/T^2 \chi_u(T^{-1}) $. Hơn nữa, theo Hệ quả 5 ta có

$$
\chi_u'(T^{-1})/T \chi_U(T^{-1}) = \operatorname{Tr}((T^{-1} \cdot I_n - U)^{-1})/T = \operatorname{Tr}((I_n - T \cdot U)^{-1}) .
$$

Suy ra $ -TP'(T)/P(T) = -n + \operatorname{Tr}((I_n - TU)') $. Hệ quả bây giờ thu được bằng cách khai triển mỗi vế của đẳng thức này thành một chuỗi lũy thừa hình thức.

#### Nhận xét 2 {#alg-vii-s5-n5-rem-2 .statement}

— Theo IV, p. 80, Hệ quả 1 và công thức (8), ta có, với mỗi đa thức $ q \in K[X] $, rằng

$$
\det q(u) = \operatorname{res}(\chi_u, q) ,
$$

trong đó $ \operatorname{res}(\chi_u, q) $ là kết quả của các đa thức $ \chi_u $ và $ q $. *Đặc biệt* nếu lấy $ q = \chi_u' $ ta thu được

$$
\det \chi_u'(u) = (-1)^{n(n-1)/2} \operatorname{dis}(\chi_u),
$$

trong đó $ \operatorname{dis}(\chi_u) $ là biệt thức của đa thức $ \chi_u $ (*IV*, p. 82, công thức (47)). Hơn nữa:

#### Hệ quả 7 {#alg-vii-s5-lem-1-cor-7 .statement}

Ta có $ \det(\operatorname{Tr}(u^{i+j})_{0 \leq i,j \leq n}) = \operatorname{dis}(\chi_u) $.

Cho D là ma trận Vandermonde $ (\alpha_i^j)_{1 \leq i,j \leq n} $. Khi đó (**III**, p. 532, công thức (29)):

$$
\det(D)^2 = \prod_{i < j} (a_j - \alpha_i)^2 = \operatorname{dis}(\chi_u).
$$

Hơn nữa, phần tử thứ $(i, j)$ của $ D \cdot 'D $ là $ \sum_k \alpha_k^{i+j-2} = \operatorname{Tr}(u^{i+j-2}) $, và hệ quả suy ra.

### 6. Đa thức đặc trưng của tích tenxơ của hai tự đồng cấu

#### Mệnh đề 11 {#alg-vii-s5-prop-11 .statement}

*Cho E* (tương ứng $ E' $) *là một không gian vectơ hữu hạn chiều trên một trường giao hoán K và cho u* (tương ứng $ u' $) *là một tự đồng cấu của E* (tương ứng $ E' $). Cho*

$$
\chi_u(X) = \prod_i (X - \alpha_i), \quad \chi_{u'}(X) = \prod_j (X - \beta_j)
$$

*là các phân tích thành các nhân tử tuyến tính của các đa thức đặc trưng của u và $ u' $* trong một mở rộng thích hợp nào đó của $ K $. *Khi đó đa thức đặc trưng của tự đồng cấu $ u \otimes u' $ của không gian vectơ $ E \otimes_K E' $ được cho bởi công thức*

$$
\chi_u \otimes u'(X) = \prod_{i,j} (X - \alpha_i \beta_j).
$$

Lập luận như trong chứng minh của Mệnh đề 10 của *VII*, p. 36, ta thấy rằng chỉ cần chứng minh bổ đề sau:

#### Bổ đề 2 {#alg-vii-s5-lem-2 .statement}

*Cho B và C là hai ma trận tam giác dưới có cấp lần lượt là m và n, với các đường chéo $ (\beta_i)_{1 \leq i \leq n} $ và $ (\gamma_j)_{1 \leq j \leq n} $. Đồng nhất tích từ điển của các tập hợp có thứ tự $ \{1, 2, \ldots, m\} $ và $ \{1, 2, \ldots, n\} $ với khoảng $ \{1, 2, \ldots, mn\} $. Khi đó ma trận tích tenxơ* (**II**, p. 357) *B $ \otimes $ C là tam giác dưới với đường chéo* $ (\beta_i \gamma_j) $.

Điều này suy ra ngay lập tức từ định nghĩa của tích tenxơ của hai ma trận (*loc. cit.*) và của tích từ điển (*Lý thuyết tập hợp*, III, p. 157).

### 7. Các tự đồng cấu chéo hóa được

#### Định nghĩa 5 {#alg-vii-s5-def-5 .statement}

— Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K và cho $ \mathfrak{F} $ là một tập hợp các tự đồng cấu của E. Khi đó $ \mathfrak{F} $ được gọi là chéo đối với một cơ sở $ (e_i) $ của E nếu ma trận của mỗi $ u \in \mathfrak{F} $ đối với $ (e_i) $ là đường chéo. Tập hợp $ \mathfrak{F} $ được gọi là chéo hóa được nếu tồn tại một cơ sở của E đối với đó $ \mathfrak{F} $ là chéo.

Định nghĩa này áp dụng đặc biệt cho trường hợp $ \mathfrak{F} $ chỉ chứa một phần tử $ u $; khi đó ta nói rằng $ u $ là chéo (chéo hóa được). Cũng lưu ý rằng $ \mathfrak{F} $ là chéo đối với một cơ sở $ (e_i) $ khi và chỉ khi các $ (e_i) $ là các vectơ riêng chung của tất cả các phần tử của $ \mathfrak{F} $; từ đó suy ra rằng $ \mathfrak{F} $ chéo hóa được khi và chỉ khi E được sinh bởi các vectơ riêng chung của tất cả các phần tử của $ \mathfrak{F} $.

Cho A là một đại số con của $ \mathrm{End}_K(E) $ chứa Id. Khi đó A chéo hóa được khi và chỉ khi nó đẳng cấu với một đại số $ K^r $ (nói cách khác là chéo hóa được theo nghĩa của V, p. 28, Định nghĩa 1); thật vậy, nếu A đẳng cấu với $ K^r $, thì A chéo hóa được theo V, p. 29, Mệnh đề 1; ngược lại, nếu A chéo hóa được, thì nó đẳng cấu với một đại số con của đại số các ma trận đường chéo, đại số này đẳng cấu như một đại số với $ K^n $, $ n = \dim(E) $, do đó A đẳng cấu với một đại số $ K^r $ nào đó (V, p. 30, Mệnh đề 3).

#### Mệnh đề 12 {#alg-vii-s5-prop-12 .statement}

— Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K, và cho u là một tự đồng cấu của E. Khi đó các điều kiện sau là tương đương:

(i) u chéo hóa được.
(ii) E là tổng trực tiếp của các không gian riêng của u.
(iii) Tất cả các nghiệm của đa thức tối tiểu của u đều thuộc K, và các nghiệm này đều đơn.

Hơn nữa, nếu các điều kiện này được thỏa mãn, thì mọi không gian con của E đóng đối với u là tổng trực tiếp của các giao của nó với các không gian riêng.

Sự tương đương của (i) và (ii) suy ra từ các nhận xét trước đó và VII, p. 31, Mệnh đề 2. Giả sử u chéo hóa được, và cho $ (\alpha_i) $ là họ các giá trị riêng của nó, và $ (V_i) $ là họ tương ứng các không gian riêng; vì hạn chế của u trên $ V_i $ là phép vị tự được xác định bởi $ \alpha_i $, nó triệt tiêu đa thức $ X - \alpha_i $; từ đó suy ra rằng u triệt tiêu đa thức $ \prod (X - \alpha_i) $, do đó đa thức này là một bội của đa thức tối tiểu của u, và vì thế trùng với nó, điều này chứng minh (iii). Ngược lại, nếu (iii) được thỏa mãn thì tồn tại một cơ sở của E đối với đó ma trận U của u là một khối đường chéo của các ma trận Jordan $ U_{m,\alpha} $ (VII, p. 35, Mệnh đề 8); khi đó theo Mệnh đề 9 các số nguyên m đều bằng 1 và do đó U là đường chéo. Cuối cùng, khẳng định cuối cùng suy ra từ sự kiện rằng nếu u chéo hóa được thì các không gian riêng của nó là các thành phần nguyên sơ của $ E_u $, và từ VII, p. 9, Hệ quả 1.

#### Hệ quả {#alg-vii-s5-n7-cor-1 .statement}

— Nếu tất cả các nghiệm của đa thức đặc trưng của u đều thuộc K, và chúng đều đơn, thì u chéo hóa được.

Thật vậy đa thức tối tiểu chia hết đa thức đặc trưng.

#### Mệnh đề 13 {#alg-vii-s5-prop-13 .statement}

— Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K, cho $ \mathcal{S} $ là một tập hợp các tự đồng cấu của E, và cho A là đại số con của $ \mathrm{End}_K(E) $ sinh bởi $ \mathcal{S} $ và $ \mathrm{Id}_E $. Khi đó các điều kiện sau là tương đương:
(i) $ \mathcal{S} $ là chéo hóa được.
(ii) Đại số trên K A là chéo hóa được.
(iii) Các phần tử của $ \mathcal{S} $ là chéo hóa được và giao hoán với nhau.

Nếu $ (e,) $ là một cơ sở của E sao cho $ \mathcal{S} $ là đường chéo đối với cơ sở này, thì A được chứa trong đại số các tự đồng cấu đường chéo đối với cơ sở này, do đó cũng là chéo hóa được; nếu A là chéo hóa được, thì cùng một lập luận cho thấy rằng $ \mathcal{S} $ là chéo hóa được. Điều này chứng minh sự tương đương của (i) và (ii). Vì hai ma trận đường chéo bất kỳ giao hoán với nhau, ta có (i) $ \rightarrow $ (iii), và còn lại là chứng minh chiều đảo. Giả sử khi đó rằng các phần tử của $ \mathcal{S} $ là chéo hóa được và giao hoán với nhau. Ta sẽ sử dụng bổ đề sau:

#### Bổ đề 3 {#alg-vii-s5-lem-3 .statement}

Cho g và h là hai tự đồng cấu giao hoán của một không gian vectơ E. Khi đó mỗi không gian riêng của g được đóng dưới h.

Thật vậy, nếu $ W_\lambda $ là không gian riêng của g tương ứng với trị riêng $ \lambda $, thì với mọi $ x \in W $, ta có
$$
gh \cdot x = hg \cdot x = h \cdot \lambda x = \lambda h \cdot x ,
$$
điều này nói rằng $ h \cdot x \in W_\lambda $.

Bây giờ ta trở lại chứng minh của Mệnh đề 13. Trong tất cả các phân tích của E thành tổng trực tiếp của các không gian con khác không, mỗi không gian con được đóng dưới tất cả các phần tử của $ \mathcal{S} $, hãy chọn một phân tích có số thành phần lớn nhất (chiều của E là một cận trên cho số này), ký hiệu $ E = \sum_{i \in I} E_i $. Cho $ u \in \mathcal{S} $ và cho $ E = \sum V_\alpha $ là phân tích của E thành tổng trực tiếp của các không gian riêng của $ u $. Theo Bổ đề 3, mỗi $ V_\alpha $ được đóng dưới $ \mathcal{S} $, và do đó mỗi $ V_i \cap E_i $ cũng vậy; theo Mệnh đề 12 mỗi $ E_i $ là tổng trực tiếp của các $ V_i \cap E_i $. Sự lựa chọn các $ E_i $ do đó buộc mỗi $ E_i $ được chứa trong một trong các $ V_\alpha $; do đó hạn chế của $ u $ trên mỗi $ E_i $ là một phép vị tự. Vì điều này đúng với mọi phần tử của $ \mathcal{S} $, suy ra rằng $ \mathcal{S} $ là chéo hóa được.

#### Hệ quả {#alg-vii-s5-n7-cor-2 .statement}

— Tổng và hợp thành của hai tự đồng cấu chéo hóa được giao hoán của E là chéo hóa được.

### 8. Tự đồng cấu nửa đơn và tự đồng cấu nửa đơn tuyệt đối

#### Định nghĩa 6 {#alg-vii-s5-def-6 .statement}

— Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K. Khi đó một tự đồng cấu u của E được gọi là nửa đơn nếu mọi không gian con của E được đóng dưới u đều có một phần bù được đóng dưới u.

Điều này có nghĩa là mọi môđun con của môđun $ K[X] $ E, là một nhân tử trực tiếp, nói cách khác môđun $ K[X] $ $ E_u $ là nửa đơn (VII, p. 9).

#### Mệnh đề 14 {#alg-vii-s5-prop-14 .statement}

— *Một tự đồng cấu u của một không gian vectơ hữu hạn chiều trên một trường giao hoán là nửa đơn khi và chỉ khi đa thức tối tiểu của u không có nhân tử bội.*

Điều này suy ra ngay lập tức từ VII, p. 9, Hệ quả 4 và p. 31, Nhận xét 1.

Cho E là một không gian vectơ trên một trường giao hoán K, cho L là một mở rộng của K, và $ u $ là một tự đồng cấu của E ; ký hiệu $ u_{(L)} $ là tự đồng cấu trên L $ l_L \otimes u $ của không gian vectơ trên L $ E_{(l.)} = L \otimes_K E $ cảm sinh từ E bởi mở rộng vô hướng. Tương tự, nếu $ \mathfrak{F} $ là một tập hợp các tự đồng cấu của E, ký hiệu $ \mathfrak{F}_{(L)} $ là tập hợp các $ u_{(L)} $ với $ u $ thuộc '8.

#### Hệ quả {#alg-vii-s5-n8-cor-1 .statement}

— *Cho u là một tự đồng cấu của một không gian vectơ hữu hạn chiều trên một trường giao hoán K, và cho L là một mở rộng của K. Nếu $ u_{(L)} $ là nửa đơn thì u là nửa đơn. Nếu u là nửa đơn và L là tách được trên K, thì $ u_{(L)} $ là nửa đơn.*

Điều này suy ra ngay lập tức từ Mệnh đề 14 và từ V, p. 120, Hệ quả 1 (chú ý rằng các đa thức tối tiểu của $ u $ và $ u_{(L)} $ trùng nhau).

#### Mệnh đề 15 {#alg-vii-s5-prop-15 .statement}

— *Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K, cho u là một tự đồng cấu của E và cho q(X) là đa thức tối tiểu của nó. Khi đó các điều kiện sau là tương đương :*

(i) *Với mọi mở rộng L của K, tự đồng cấu $ u_{(L)} $ là nửa đơn.*
(ii) *Tồn tại một mở rộng L của K sao cho tự đồng cấu $ u_{(L)} $ là chéo hóa được.*
(iii) *Đa thức q(X) là tách được trên K.*

Thật vậy, điều kiện (i) có nghĩa là đa thức $ 1 \otimes q(X) $ trong $ L[X] $ không có nhân tử bội, với mọi mở rộng L của K (Mệnh đề 14), điều kiện (ii) có nghĩa là tồn tại một mở rộng L của K sao cho mọi nghiệm của $ q(X) $ thuộc L và các nghiệm này đều đơn (VII, p. 40, Mệnh đề 12), và các điều kiện này mỗi điều kiện đều tương đương với (iii) theo định nghĩa (V, p. 38).

#### Định nghĩa 7 {#alg-vii-s5-def-7 .statement}

— *Một tự đồng cấu u thỏa mãn các điều kiện (i), (ii) và (iii) của Mệnh đề 15 được gọi là nửa đơn tuyệt đối.*

#### Hệ quả {#alg-vii-s5-n8-cor-2 .statement}

— *Điều kiện cần và đủ để u là nửa đơn tuyệt đối là tồn tại một mở rộng L của K sao cho L là hoàn hảo và $ u_{(L)} $ là nửa đơn.*

Điều kiện trong hệ quả có nghĩa là tồn tại một mở rộng L của K sao cho L là hoàn hảo và $ q(X) $ không có nhân tử bội trong $ L[X] $ (Mệnh đề 14) ; điều kiện này tương đương với (iii) theo V, p. 38, Hệ quả 2.

#### Mệnh đề 16 {#alg-vii-s5-prop-16 .statement}

— *Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K, cho $ \mathfrak{F} $ là một tập hợp các tự đồng cấu của E và cho A là đại số con của $ \mathrm{End}_K(E) $ sinh bởi $ \mathfrak{F} $ và Id. Khi đó các điều kiện sau là tương đương :*

(i) *Tồn tại một mở rộng L của K sao cho $ \mathfrak{F}_{(l.)} $ là chéo hóa được.*

(ii) *Đại số trên K* $ A $ *là étale* (V, p. 28, Định nghĩa 1).

(iii) *Các phần tử của* $ \mathfrak{F} $ *là nửa đơn tuyệt đối và giao hoán với nhau*.

Trước hết lưu ý rằng, với mọi mở rộng $ L $ của $ K $, đại số trên $ L $ sinh bởi $ \mathfrak{F}_{(L)} $ và $ \mathrm{Id}_{E_{(L)}} $ trùng với $ L \otimes_K A $; do đó theo Mệnh đề 13, $ \mathfrak{F}_{(L)} $ chéo hóa được khi và chỉ khi đại số trên $ L $ $ L \otimes_K A $ chéo hóa được. Vì vậy, tính tương đương của các điều kiện (i) và (ii) suy ra từ V, p. 28, Định nghĩa 1. Mặt khác, hiển nhiên rằng (i) $ \Rightarrow $ (iii). Cuối cùng, giả sử (iii) đúng, và lấy $ L $ là một bao đóng đại số của $ K $; khi đó các phần tử của $ \mathfrak{F}_{(L)} $ chéo hóa được (VII, p. 40, Mệnh đề 12) và giao hoán với nhau; do đó $ \mathfrak{F}_{(L)} $ chéo hóa được theo VII, p. 41, Mệnh đề 13.

#### Hệ quả {#alg-vii-s5-n8-cor-3 .statement}

*Tổng và tích của hai tự đồng cấu nửa đơn tuyệt đối giao hoán với nhau là nửa đơn tuyệt đối*.

#### Nhận xét {#alg-vii-s5-n8-rem-1 .statement}

— Giả sử các điều kiện của Mệnh đề 16 được thỏa mãn và lấy $ L $ là một mở rộng của $ K $. Theo Mệnh đề 13, tập hợp $ \mathfrak{F}_{(L)} $ chéo hóa được khi và chỉ khi đại số $ L \otimes_K A $ chéo hóa được. Suy ra từ V, p. 30, Mệnh đề 2 rằng tồn tại một mở rộng hữu hạn $ L $ của $ K $ sao cho $ \mathfrak{F}_{(L)} $ chéo hóa được. Thực ra $ L $ có thể được lấy là *Galois*; thật vậy, lấy một tập con hữu hạn $ \mathfrak{F}' $ của $ \mathfrak{F} $ sinh ra $ A $, ta có thể lấy $ L $ là một trường phân rã của các đa thức cực tiểu của các phần tử của $ \mathfrak{F}' $ (Mệnh đề 12 và 13).

### 9. Phân tích Jordan

#### Định nghĩa 8 {#alg-vii-s5-def-8 .statement}

*Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán và cho $ u $ là một tự đồng cấu của $ E $. Khi đó một phân tích Jordan của $ u $ là một cặp* $ (u_s, u_n) $, *trong đó $ u_s $ là một tự đồng cấu nửa đơn của $ E $ và $ u_n $ là một tự đồng cấu lũy linh của $ E $, sao cho* $ u_s u_n = u_n u_s $ *và* $ u = u_s + u_n $.

#### Định lý 1 {#alg-vii-s5-thm-1 .statement}

*Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $ và cho $ u $ là một tự đồng cấu của $ E $. Khi đó $ u $ có một phân tích Jordan* $ (u_s, u_n) $ *khi và chỉ khi các trị riêng của $ u $ tách được trên $ K $. Hơn nữa phân tích là duy nhất, các đa thức đặc trưng của $ u $ và $ u_s $ trùng nhau, và tồn tại các đa thức* $ P, Q \in K[X] $, *không có hạng tử hằng, sao cho* $ u_s = P(u) $ *và* $ u_n = Q(u) $.

A) Trước hết ta chứng minh trường hợp đặc biệt sau đây

#### Bổ đề 4 {#alg-vii-s5-lem-4 .statement}

*Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $ và cho $ u $ là một tự đồng cấu tam giác hóa được của $ E $. Khi đó tồn tại duy nhất một tự đồng cấu chéo hóa được $ v $ của $ E $ giao hoán với $ u $ và sao cho* $ u - v $ *là lũy linh. Hơn nữa, với các điều kiện này, các đa thức đặc trưng của $ u $ và $ v $ trùng nhau, và tồn tại một đa thức* $ P \in K[X] $ *sao cho* $ v = P(u) $.

Cho $ v $ là một tự đồng cấu chéo hóa được của $ E $ sao cho $ uv = vu $ và $ v - u $ là lũy linh; cho $ \alpha $ là một trị riêng của $ v $ và cho $ V_\alpha $ là không gian riêng tương ứng. Theo Bổ đề 3 (VII, p. 41), $ V_\alpha $ đóng đối với $ u $, và hạn chế của u - α trên V, cũng chính là hạn chế của u - v, nên là lũy linh; do đó V, được chứa trong không gian con M, gồm những x ∈ E bị triệt tiêu bởi một lũy thừa nào đó của u - a. Vì E là tổng trực tiếp của các V, và cũng là tổng trực tiếp của các M, (VII, p. 34, Mệnh đề 7), điều này cho thấy V, = M, với mọi a. Theo hệ quả của Mệnh đề 9 (VII, p. 36), suy ra rằng χ_u = χ_v ; đồng thời cũng suy ra rằng v được xác định duy nhất bởi u ; hạn chế của nó trên mỗi M_α là phép vị tự xác định bởi α.

Ngược lại, hãy định nghĩa v theo điều kiện trên; rõ ràng nó là chéo hóa được và u - v là lũy linh. Theo Mệnh đề 7 của VII, p. 34, tồn tại các đa thức q, sao cho, với mọi x ∈ E, thành phần của x trong M, là q_α(u).x. Khi đó v = ∑ αq_α(u); điều này suy ra rằng u và v giao hoán và hoàn tất chứng minh.

B) Bây giờ ta quay lại chứng minh Định lý 1.

Trước hết, giả sử rằng u có thể viết dưới dạng s + n, trong đó s là nửa đơn tuyệt đối và n là lũy linh, và s, n giao hoán với nhau. Cho Ω là một bao đóng đại số của K; khi đó u_{(Ω)} = s_{(Ω)} + n_{(Ω)}, trong đó s_{(Ω)} là chéo hóa được và n_{(Ω)} là lũy linh, và s_{(Ω)} và n_{(Ω)} giao hoán với nhau; theo Bổ đề 4 suy ra rằng s_{(Ω)}, và do đó cả s, là duy nhất, rằng các đa thức χ_{u_{(Ω)}} và χ_{s_{(Ω)}} trong Ω[X] trùng nhau, do đó cả các đa thức χ_u và χ_s cũng trùng nhau, và rằng s có thể biểu diễn dưới dạng một đa thức theo u với các hệ số trong Ω. Trước hết điều này cho thấy các trị riêng của u cũng chính là các trị riêng của s, nên tách được trên K (VII, p. 42, Mệnh đề 15); ngoài ra, vì s là một tổ hợp 0-tuyến tính của các lũy thừa của u, nó cũng là một tổ hợp K-tuyến tính của chính các lũy thừa đó (II, p. 311, Mệnh đề 19), và tồn tại một đa thức P ∈ K[X] sao cho s = P(u), do đó n = Q(u), trong đó Q(X) = X - P(X). Bây giờ ta hãy chứng minh rằng Q (và do đó P) có thể được chọn không có số hạng hằng. Nếu u khả nghịch thì đa thức đặc trưng của nó có số hạng hằng khác không, và định lý Cayley-Hamilton (III, p. 541, Mệnh đề 20) cho thấy 1 có thể biểu diễn thành một đa thức theo u không có số hạng hằng, nên mệnh đề được khẳng định trong trường hợp này. Nếu u không khả nghịch, thì hạt nhân W của nó khác không và đóng đối với n (VII, p. 41, Bổ đề 3); vì hạn chế của n trên W là lũy linh, tồn tại một vectơ x ≠ 0 trong W sao cho u(x) = n(x) = 0, điều này cho thấy Q không thể có số hạng hằng.

Ngược lại, giả sử các trị riêng của u tách được trên K, và cho L là một mở rộng Galois hữu hạn của K chứa các trị riêng này. Theo Bổ đề 4, ta có thể viết u_{(L)} = v + w, trong đó v chéo hóa được và w lũy linh, và vw = wv. Cho B là một cơ sở của E, cho B' là cơ sở tương ứng của L ⊗_K E, và cho U, V, W là các ma trận của u_{(L)}, v, w đối với B'; chú ý rằng U cũng là ma trận của u đối với B, nên có các phần tử trong K. Với mọi K-tự đẳng cấu σ của L, và mọi ma trận A có các phần tử trong L, ký hiệu A" là ma trận nhận được bằng cách áp dụng σ vào các phần tử của A. Cho a là một K-tự đẳng cấu của L; khi đó U = U^σ = (V + W)^σ = V^σ + W^σ, V^σW^σ = (VW)^σ = (WV)^σ = W^σV^σ; vì Vu là ma trận của một tự đồng cấu chéo hóa được và W" là lũy linh, theo Bổ đề 4, suy ra Vu = V và W^σ = W. Vì điều này đúng với mọi σ, các phần tử của V và W thuộc K; nếu $ u_s $ và $ u_n $ là các tự đồng cấu của E có các ma trận lần lượt là V và W đối với B, thì $ (u_s)_{(L)} = v $ và $ (u_n)_{(L)} = w $. Suy ra $ u_s $ là nửa đơn tuyệt đối, $ u_n $ là lũy linh, $ u_s $ và $ u_n $ giao hoán với nhau, và $ u = u_s + u_n $. Chứng minh được hoàn tất.

Bất cứ khi nào một tự đồng cấu f có một phân tích Jordan, ta ký hiệu nó là (f,, f,), và các tự đồng cấu f, và f, lần lượt được gọi là thành phần *nửa đơn* tuyệt đối và thành phần lũy linh của f. Khi K hoàn hảo, mọi tự đồng cấu đều có một phân tích Jordan; trong trường hợp này cũng không có sự phân biệt giữa các tự đồng cấu nửa đơn tuyệt đối và các tự đồng cấu nửa đơn, và đôi khi ta gọi « thành phần nửa đơn » thay cho « thành phần nửa đơn tuyệt đối ».

#### Hệ quả 1 {#alg-vii-s5-lem-4-cor-1 .statement}

Giả sử $ u $ có một phân tích Jordan, và cho L là một mở rộng của K. Khi đó $ u_{(L)} $ có một phân tích Jordan, với $ (u_{(L)})_s = (u_s)_{(L)} $ và $ (u_{(L)})_n = (u_n)_{(L)} $.

#### Hệ quả 2 {#alg-vii-s5-lem-4-cor-2 .statement}

Giả sử u có một phân tích Jordan. Khi đó mọi *tự đồng cấu* của E *giao hoán* với u cũng giao hoán với $ u_s $ và $ u_n $.

#### Hệ quả 3 {#alg-vii-s5-lem-4-cor-3 .statement}

Cho $ u $ và $ v $ là hai tự đồng cấu giao hoán với nhau của E có các phân tích Jordan.
a) Các tự đồng cấu $ u, v, u_s, v_s, u_n, v_n, v, $ đều giao hoán với nhau.
b) Các tự đồng cấu $ u + v $ và $ uv $ có các phân tích Jordan với
$$
(u + v)_s = u_s + v_s , \quad (u + v)_n = u_n + v_n , \quad (uv)_s = u_s v_s ,
$$
$$
(uv)_n = u_s v_n + u_n v_s + u_n v_n .
$$
Phần a) suy ra từ Hệ quả 2. Để chứng minh phần b), chỉ cần nhận thấy rằng $ u_s + v_s $ và $ u_s v_s $ là nửa đơn tuyệt đối (VII, p. 43, Hệ quả) và rằng $ u_n + v_n $ và $ u_s v_n + u_n v_s + u_n v_n $ là lũy linh (vì là các tổng của những tự đồng cấu lũy linh giao hoán với nhau).

#### Hệ quả 4 {#alg-vii-s5-lem-4-cor-4 .statement}

Giả sử $ u $ có một phân tích Jordan, và cho R là một đa thức trong $ \mathbf{K}[X] $. Khi đó tự đồng cấu $ R(u) $ có một phân tích Jordan với $ R(u)_s = R(u_s) $.

#### Nhận xét 1 {#alg-vii-s5-n9-rem-1 .statement}

Ta có $ \det(u_s) = \det(u) $ và $ \operatorname{Tr}(u_s) = \operatorname{Tr}(u) $.
2) Một điều kiện cần và đủ để $ u $ tam giác hóa được là $ u $ có một phân tích Jordan với $ u_s $ chéo hóa được. Khi đó tồn tại một cơ sở của E sao cho ma trận của $ u $ đối với cơ sở đó là tam giác dưới, và ma trận của $ u_s $ là đường chéo, với cùng đường chéo như ma trận của $ u $ (xem Bổ đề 4 và Mệnh đề 19 dưới đây).
Tuy nhiên, cần lưu ý rằng nếu ma trận của $ u $ đối với một cơ sở nào đó là tam giác, thì nói chung không suy ra rằng ma trận của $ u_s $ đối với cùng cơ sở đó là đường chéo.

3) Khái niệm phân tích Jordan đối với một ma trận vuông có thể được định nghĩa theo cách tương tự. Chẳng hạn, đối với ma trận Jordan $ U_{m,\alpha} $ ta có
$$
(U_{m,\alpha})_s = \alpha \cdot I_m , \quad (U_{m,\alpha})_n = U_{m,0} .
$$
4) Nếu $ u $ là nửa đơn nhưng không tuyệt đối nửa đơn, thì nó không có phân tích Jordan.

Một tự đồng cấu $ u $ của một không gian vectơ $ V $ trên một trường giao hoán được gọi là unipotent nếu tự đồng cấu $ u - \mathrm{Id} $, là lũy linh, nghĩa là nếu tồn tại một số nguyên $ r $ sao cho $ (u - \mathrm{Id},)' = 0 $; khi đó $ u $ là một tự đẳng cấu của $ V $, vì nếu $ u = \mathrm{Id}, - n $ với $ n' = 0 $, thì
$$
(\mathrm{Id}, + n + \ldots + n^{r-1})\ u = u (\mathrm{Id}_V + n + \ldots + n^{r-1}) = \mathrm{Id}_V .
$$
Nếu $ V $ có số chiều hữu hạn $ m $, thì $ u $ là unipotent khi và chỉ khi $ \chi_u(X) = (X - 1)^m $ (VII, p. 33, Hệ quả 3 của Mệnh đề 5).

#### Mệnh đề 17 {#alg-vii-s5-prop-17 .statement}

— Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán, và cho $ f $ là một tự đồng cấu của $ E $. Khi đó các điều kiện sau là tương đương:
(i) $ f $ có một phân tích Jordan và là một tự đẳng cấu ;
(ii) $ f $ có một phân tích Jordan và $ f_s $ là một tự đẳng cấu ;
(iii) tồn tại một tự đẳng cấu tuyệt đối nửa đơn $ a $ của $ E $ và một tự đồng cấu unipotent $ u $ của $ E $ sao cho $ f = ua = au $.
Hơn nữa, dưới các điều kiện này, trong ký hiệu của (iii), ta phải có $ a = f_s $ và $ u = 1 + f_s^{-1}f_n $.
(i) $\Rightarrow$ (ii): điều này suy ra từ Nhận xét 1.
(ii) $\Rightarrow$ (iii): lấy $ a = f_s $ và $ u = 1 + f_s^{-1}f_n $; khi đó $ f = ua = au $, trong khi $ a $ là một tự đẳng cấu tuyệt đối nửa đơn, và $ u $ là unipotent.
(iii) $\Rightarrow$ (i): trong ký hiệu của (iii), lấy $ n = a(u - 1) = (u - 1)a $. Khi đó $ an = na $ và $ f = a + n $, và $ n $ là lũy linh. Suy ra $ (a, n) $ là phân tích Jordan của $ f $. Điều này kéo theo (i) cũng như các hệ thức $ a = f_s $ và $ u = 1 + f_s^{-1}f_n $.

Đặt $ f_r = f_s^{-1}f = ff_s^{-1} = 1 + f_s^{-1}f_n $, và gọi đây là thành phần unipotent của $ f $. Cặp $ (f_s, f_r) $ thường được gọi là phân tích Jordan nhân của tự đẳng cấu $ f $.

#### Mệnh đề 18 {#alg-vii-s5-prop-18 .statement}

— Cho $ E $ là một không gian vectơ hữu hạn chiều trên một trường giao hoán $ K $, cho $ u $ là một tự đồng cấu của $ E $ và cho $ E' $ là một không gian con của $ E $ đóng đối với $ u $. Cho $ u' $ (tương ứng $ u'' $) là tự đồng cấu của $ E' $ (tương ứng $ E/E' $) cảm sinh bởi $ u $. Khi đó $ \chi_u = \chi_{u'} \cdot \chi_{u''} $.

Để $ u $ có một phân tích Jordan, điều kiện cần và đủ là $ u' $ và $ u'' $ có ; hơn nữa, nếu điều này đúng thì các thành phần nửa đơn tuyệt đối (tương ứng lũy linh) của $ u' $ và $ u'' $ là các tự đồng cấu của $ E' $ và $ E/E' $ cảm sinh bởi thành phần nửa đơn tuyệt đối (tương ứng lũy linh) của $ u $.

Cho $ B $ là một cơ sở của $ E $ chứa một cơ sở $ B' $ của $ E' $, và cho $ B'' $ là cơ sở của

$E'' = E/E'$ là ảnh của $B - B'$. Cho $U, U', U''$ lần lượt là các ma trận của $u, u', u''$ đối với $B, B', B''$. Khi đó $U$ có dạng

$$
\begin{pmatrix}
U' & Z \\
0 & U''
\end{pmatrix}
$$

và $\chi_u = \chi_U = \chi_{U'}\chi_{U''} = \chi_{u'}\chi_{u''}$ (xem III, p. 533, Bài tập 2). Ta suy ra rằng tập hợp các trị riêng của $u$ là hợp của các tập hợp các trị riêng của $u'$ và $u''$. Nếu $u'$ và $u''$ có các phân tích Jordan thì các trị riêng của $u'$ và $u''$ là tách được trên K, do đó các trị riêng của $u$ cũng vậy, và $u$ có một phân tích Jordan (VII, p. 43, Định lý 1). Ngược lại, nếu $u$ có một phân tích Jordan $(s, n)$ thì $s$ và $n$ giữ $E'$ bất biến vì chúng là các đa thức theo $u$; gọi $s', n', s'', n''$ là các tự đồng cấu của $E', E', E'', E''$ cảm sinh bởi $s, n, s, n$ tương ứng. Khi đó $s'$ và $s''$ là nửa đơn tuyệt đối, vì các đa thức cực tiểu của chúng chia hết đa thức cực tiểu của $s$ (VII, p. 42, Mệnh đề 15); ngoài ra $n'$ và $n''$ là lũy linh. Cuối cùng $u' = s' + n', u'' = s'' + n'', s'n' = n's', \text{ và } s''n'' = n''s''$, điều này hoàn tất chứng minh.

#### Mệnh đề 19 {#alg-vii-s5-prop-19 .statement}

— *Cho E là một không gian vectơ hữu hạn chiều trên một trường giao hoán K, và cho $ \mathcal{S} $ là một tập hợp các tự đồng cấu tam giác hoá được giao hoán của E. Khi đó tồn tại một cơ sở của E sao cho, đối với cơ sở đó, ma trận của mỗi phần tử u của $ \mathcal{S} $ là tam giác dưới và ma trận của $ u_s $ là đường chéo, với cùng các phần tử đường chéo như của u.*

Theo Hệ quả 3 của VII, p. 4.5, tập hợp $ \mathfrak{T}_s $ các thành phần nửa đơn tuyệt đối của các phần tử của $ \mathfrak{T} $ gồm các phần tử chéo hoá được giao hoán với nhau, do đó là chéo hoá được (VII, p. 41, Mệnh đề 13), tập hợp $ \mathfrak{T}_n $ các thành phần lũy linh của các phần tử của $ \mathcal{S} $ gồm các phần tử lũy linh giao hoán với nhau, và mỗi phần tử của $ \mathfrak{T}_n $ giao hoán với mỗi phần tử của $ \mathfrak{T}_s $. Lập luận như trong chứng minh của Mệnh đề 13 (VII, p. 41), ta thấy rằng tồn tại một phân tích của E thành tổng trực tiếp của các không gian con $E_i$, bất biến đối với $ \mathfrak{T}_s $ và $ \mathfrak{T}_n $, và sao cho hạn chế của mỗi phần tử của $ \mathcal{S} $, trên mỗi $E$, là một phép vị tự. Thay thế $E$ lần lượt bởi mỗi $E$, ta có thể giả sử rằng các phần tử của $ \mathcal{S} $, là các phép vị tự; chỉ cần chứng minh rằng tồn tại một cơ sở của E sao cho các phần tử của $ \mathfrak{T}_n $ được biểu diễn bởi các ma trận tam giác dưới với đường chéo không; do đó ta quy về trường hợp $ \mathcal{S} $ gồm các phần tử lũy linh.

Bây giờ giả sử $E \neq 0$, và cho F là một không gian con khác không của $E$, bất biến dưới $ \mathfrak{T} $, có chiều nhỏ nhất. Khi đó với mỗi $u \in \mathfrak{T}$, hạt nhân của hạn chế của $u$ lên F là khác không và bất biến dưới $ \mathfrak{T} $ (VII, p. 41, Bổ đề 3); theo lựa chọn F, hạn chế của $u$ lên F do đó bằng không với mọi $u \in \mathfrak{T}$. Cho $x \in F,\ x \neq 0$; khi đó $u(x) = 0$ với mọi $u \in \mathcal{S}$; bằng quy nạp theo chiều của E, ta có thể giả sử rằng tồn tại một cơ sở $(\bar{e}_1, ..., \bar{e}_{n-1})$ của không gian thương $E' = E/Kx$ sao cho, với mọi $u \in \mathfrak{T}$, tự đồng cấu $\bar{u}$ của $E'$ cảm sinh bởi $u$ có một ma trận đối với cơ sở này là tam giác dưới với đường chéo bằng không; nếu $e_i \in E$ chiếu lên a, với $i = 1, ..., n-1$, thì cơ sở $(e_1, ..., e_{n-1}, x)$ thỏa mãn các điều kiện yêu cầu.

Exercises

### Bài tập {#alg-vii-s5-exercises}

Tất cả các trường trong mục này đều là giao hoán trừ khi được phát biểu tường minh là khác đi.

Xem [các bài tập của § 5](exercises/s5/).
