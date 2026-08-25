---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 10
section_title: Galois extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.56-A V.76, A V.154-A V.160
pdf_pages: 0170-0190, 0268-0274
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Galois extensions
      page: 56
      pdf_page: 170
    - "no": 2
      title: The Galois group
      page: 58
      pdf_page: 172
    - "no": 3
      title: Topology of the Galois group
      page: 60
      pdf_page: 174
    - "no": 4
      title: Galois descent
      page: 62
      pdf_page: 176
    - "no": 5
      title: '*Galois cohomology*'
      page: 64
      pdf_page: 178
    - "no": 6
      title: Artin’s theorem
      page: 65
      pdf_page: 179
    - "no": 7
      title: The fundamental theorem of Galois theory
      page: 67
      pdf_page: 181
    - "no": 8
      title: Change of base field
      page: 69
      pdf_page: 183
    - "no": 9
      title: The normal basis theorem
      page: 72
      pdf_page: 186
    - "no": 10
      title: Finite $ \Gamma $-sets and etale algebras
      page: 75
      pdf_page: 189
    - "no": 11
      title: The structure of quasi-Galois extensions
      page: 76
      pdf_page: 190
statements: 49
exercises: 23
content_sha256: 4d695e51cd3f2e6a1186a9bdffd7504e1182109602ee665d16ee71b13ac34f8c
translated_from: content/en/alg/V/10_s10_galois_extensions.md
source_content_sha256: ca3fc22a3927420d19131276d84c6a18bdb2e1153a1a717cbafc7ecf2e2c2650
translation_model: gpt-5-6-mini
translation_run: translate-vi-19dbb229
glossary_version: 34
glossary_terms_sha256: d7731983bf105a6665742a828f144f0612c75b7d0959ab1ca7fe5f9be18cff84
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. CÁC MỞ RỘNG GALOIS

Trong suốt đoạn này, K ký hiệu một trường.

### 1. Định nghĩa các mở rộng Galois

#### Định lý 1 {#alg-v-s10-thm-1 .statement}

— Cho N là một mở rộng đại số của K và $ \Gamma $ là nhóm các tự đẳng cấu của N giữ K bất biến. Khi đó các mệnh đề sau là tương đương:
a) Mọi phần tử của N bất biến dưới $ \Gamma $ đều thuộc ảnh của K trong N.
b) N là một mở rộng tách được quasi-Galois của K.
c) Với mỗi $ x \in N $, đa thức tối tiểu của x trên K phân rã trong $ N[X] $ thành một tích các đa thức phân biệt bậc 1.
Sự tương đương của b) và c) suy ra từ Hệ quả của Mệnh đề 6 (V, p. 40) và định nghĩa mở rộng quasi-Galois (V, p. 53, Định nghĩa 2). Ta đồng nhất K với ảnh chính tắc của nó trong N.
$ a) \Rightarrow c) $: Giả sử K là trường các bất biến của $ \Gamma $. Cho $ x \in N $, với đa thức tối tiểu $ f $ trên K và gọi A là tập hợp tất cả các nghiệm của f trong N. Đặt
$$
g(X) = \prod_{y \in A} (X - y).
$$
Mọi tự đẳng cấu $ a \in \Gamma $ cảm sinh một phép hoán vị của A, và do đó giữ bất biến các hệ số của đa thức $ g \in N[X] $. Vì vậy ta có $ g \in K[X] $ và vì $ g(x) = 0 $, đa thức g là một bội của $ f $ trong $ K[X] $ (V, p. 16, Định lý 1). Hơn nữa, $ f $ và g đều là đơn thức đầu và g chia hết $ f $ (IV, p. 16, Mệnh đề 5); do đó ta có $ f = g $, nghĩa là đa thức tối tiểu $ f $ của $ x $ trên $ K $ là một tích trong $ N[X] $ của các đa thức phân biệt bậc 1.

c) ⇒ a): cho x là một phần tử của N không thuộc K. Ký hiệu Ω là một bao đóng đại số của K chứa N như một mở rộng con (V, p. 23, Định lý 2). Gọi f là đa thức tối tiểu của x trên K, có bậc ≥ 2 theo giả thiết, và gọi A là tập hợp các nghiệm của $ f(X) $ trong N. Nếu điều kiện c) được thỏa mãn, ta có $ f(X) = \prod_{y \in A} (X - y) $ và do đó (V, p. 53, Hệ quả 1) A là tập hợp các liên hợp của x trong Ω. Vì f có bậc ≥ 2, tồn tại trong A một phần tử $ y \neq x $, do đó tồn tại một tự đẳng cấu u của Ω giữ K bất biến sao cho $ u(x) = y $. Bây giờ theo giả thiết c), mở rộng N của K là quasi-Galois, do đó $ u(N) = N $ (V, p. 54, Hệ quả 1); suy ra u cảm sinh một tự đẳng cấu a của N giữ K bất biến sao cho $ \sigma(x) = y \neq x $, nên K là trường các bất biến của Γ.

#### Định nghĩa 1 {#alg-v-s10-def-1 .statement}

— Một mở rộng N của K được gọi là Galois nếu nó đại số và thỏa mãn các điều kiện tương đương a), b), c) của Định lý 1.

Cho N là một trường, Γ là một nhóm các tự đẳng cấu của N và $ N_0 $ là trường các bất biến của Γ. Khi N là đại số trên $ N_0 $ thì nó là một mở rộng Galois của $ N_0 $. Điều này không phải lúc nào cũng đúng: chẳng hạn, giả sử K là vô hạn và lấy N là trường các phân thức K(X); với mỗi $ a \in K $ gọi $ \sigma_a $ là tự đẳng cấu của K(X) biến $ f(X) $ thành $ f(X + a) $. Tập hợp tất cả các $ a $ là một nhóm các tự đẳng cấu của K(X), mà trường các bất biến của nó dễ thấy là K; tuy nhiên K(X) không đại số trên K.

Cho Ω là một bao đóng đại số của K, gọi A là một tập hợp các phần tử của Ω tách được trên K và B là tập hợp các phần tử liên hợp trên K của các phần tử của A. Khi đó B gồm các phần tử đại số và tách được trên K. Do đó (V, p. 39, Mệnh đề 6 và p. 56, Mệnh đề 5) trường K(B) là một mở rộng tách được quasi-Galois của K; nói cách khác, mở rộng quasi-Galois sinh bởi A (V, p. 55) là một mở rộng Galois của K; ta cũng sẽ nói rằng nó là mở rộng Galois của K sinh bởi tập con A của O.

Đặc biệt, trường phân rã trong Ω của một họ các đa thức tách được trên K, một bao đóng tách được của K, là các mở rộng Galois của K.

#### Mệnh đề 1 {#alg-v-s10-prop-1 .statement}

— Cho N là một mở rộng của K và $ (N_i)_{i \in I} $, một họ khác rỗng các mở rộng con của N. Đặt $ E = \cap_{i \in I} N_i $ và $ F = K \left( \bigcup_{i \in I} N_i \right) $. Nếu tất cả các mở rộng N, đều là Galois trên K thì điều tương tự cũng đúng với E và F.

Trước hết E là đại số và tách được trên K (V, p. 36, Mệnh đề 1) và điều tương tự cũng đúng với F (V, p. 41, Mệnh đề 8). Hơn nữa, E và F là quasi-Galois trên K theo Mệnh đề 4 (V, p. 55).

#### Mệnh đề 2 {#alg-v-s10-prop-2 .statement}

— Cho N là một mở rộng Galois của K và E là một mở rộng con của N, có bậc hữu hạn trên K. Tồn tại một mở rộng con F của N chứa E, Galois và có bậc hữu hạn trên K.

Vì N là quasi-Galois trên K, Hệ quả 1 của V, p. 56 chứng minh sự tồn tại của một mở rộng con quasi-Galois F của N chứa E và có bậc hữu hạn trên K. Vì N tách được trên K, điều tương tự cũng đúng với F (V, p. 36, Mệnh đề 1), do đó F là Galois trên K.

Mệnh đề 2 kéo theo kết quả sau: cho R là một bao đóng đại số của K và E₁, ..., Eₙ là các mở rộng đại số tách được có bậc hữu hạn trên K, được chứa trong R. Khi đó tồn tại một mở rộng Galois N của K, có bậc hữu hạn, được chứa trong R và chứa E₁, ..., Eₙ.

### 2. Nhóm Galois

#### Định nghĩa 2 {#alg-v-s10-def-2 .statement}

Cho N là một mở rộng Galois của trường K. Nhóm gồm tất cả các tự đẳng cấu của N giữ K bất biến sẽ được gọi là nhóm Galois của N trên K và ký hiệu là Gal(N/K).

Cho N là một mở rộng Galois hữu hạn của K. Khi đó N là một mở rộng tách được và quasi-Galois hữu hạn của K. Do đó (V, p. 32, Mệnh đề 4 và V, p. 54, Mệnh đề 3), cấp của Gal(N/K) bằng [N : K]. Sau này ta sẽ chứng minh rằng nếu N là một mở rộng Galois của K sao cho Gal(N/K) hữu hạn, thì N có bậc hữu hạn trên K (V, p. 66, Định lý 3).

Cho Ω là một mở rộng đóng đại số của K và A là tập hợp các nghiệm trong Ω của một đa thức tách được f ∈ K[X]. Khi đó trường N = K(A) là một mở rộng Galois của K. Rõ ràng mọi tự đẳng cấu của N giữ K bất biến đều giữ A ổn định, và vì A sinh N trên K, ánh xạ a ↦ σ|A là một đẳng cấu của Gal(N/K) lên một nhóm con Γ của nhóm đối xứng S_A của tập hợp A, nhóm này sẽ được gọi là nhóm Galois của đa thức f. Từ Nhận xét 3 (V, p. 55) suy ra rằng nếu x và y thuộc A, các tính chất sau là tương đương:

a) x và y liên hợp trên K,
b) x và y thuộc cùng một quỹ đạo dưới tác động của Γ,
c) x và y là các nghiệm của cùng một nhân tử bất khả quy của f.

Đặc biệt, f bất khả quy khi và chỉ khi A khác rỗng và Γ tác động bắc cầu trên A.

#### Ví dụ 1 {#alg-v-s10-n2-exa-1 .statement}

Giả sử đặc số của K khác 2 và cho N là một mở rộng bậc hai của K. Nếu x ∈ N − K, thì ta có N = K(x) và đa thức tối tiểu của x trên K có dạng f(X) = X² − aX + b, với a, b ∈ K. Do đó ta có f(X) = (X − x)(X − y), trong đó y = a − x, nên y liên hợp với x; vì f(X) tách được, mở rộng N là Galois. Nhóm Gal(N/K) có hai phần tử cảm sinh hai phép hoán vị của tập hợp {x, y}.

#### Ví dụ 2 {#alg-v-s10-n2-exa-2 .statement}

Cho f = X³ + X² − 2X − 1 ∈ Q[X]. Đa thức f bất khả quy, vì nếu không, nó có một nghiệm x ∈ Q; viết x = a/b với a, b ∈ Z, a và b nguyên tố cùng nhau, ta phải có a(a² + ab − 2b²) = b³ và a³ = b(b² + 2ab − a²); nhưng điều này suy ra a chia hết cho b và b chia hết cho a, do đó x = ±1, điều này là không thể. Đặt ξ = e^{2\pi i / 7} ∈ C; khi đó đa thức f có các nghiệm α = ξ + ξ⁻¹, β = ξ² + ξ⁻², γ = ξ³ + ξ⁻³. Ta có β = a² − 2 và γ = a³ − 3α, do đó mở rộng Q(α) là Galois trên Q. Nhóm Galois của Q(α) trên Q là cyclic có cấp 3 và được sinh bởi một phần tử σ sao cho σ(α) = β, σ(β) = γ, σ(γ) = α. \*

#### Ví dụ 3 {#alg-v-s10-n2-exa-3 .statement}

Giả sử rằng $ K = \mathbf{Q} $ và lấy $ f = X^3 - 2 $. Dùng phân tích các số nguyên thành tích các nhân tử nguyên tố (I, p. 51), ta dễ dàng thấy rằng 2 không phải là lập phương của một phần tử của $ \mathbf{Q} $. Do đó đa thức $ f $ là bất khả quy, vì nếu không, nó sẽ có một nghiệm trong $ \mathbf{Q} $. Cho $ A = \{ x_1, x_2, x_3 \} $ là tập hợp các nghiệm của $ f $ trong $ \Omega $ và $ \Gamma $ là nhóm Galois của $ f $. Nó tác động bắc cầu trên $ A $; do đó cấp của nó chia hết cho ba. Mặt khác, thương $ j = \frac{x_2}{x_1} $ khác 1 và ta có $ j^3 = 1 $. Do đó $ j $ thỏa mãn quan hệ $ j^2 + j + 1 = 0 $; nhưng đa thức $ T^2 + T + 1 = \left( T + \frac{1}{2} \right)^2 + \frac{3}{4} $ không có nghiệm trong $ \mathbf{Q} $, điều này cho thấy (Ví dụ 1) rằng $ [\mathbf{Q}(j) : \mathbf{Q}] = 2 $. Vậy $ [\mathbf{N} : \mathbf{Q}] $ chia hết cho 2, và suy ra cấp của $ \Gamma $ chia hết cho 6. Vì $ \Gamma $ được chứa trong nhóm $ \mathfrak{S}_A $ có cấp 6, ta có $ \Gamma = \mathfrak{S}_A $.

#### Ví dụ 4 {#alg-v-s10-n2-exa-4 .statement}

Giả sử $ K $ có đặc số $ p \neq 0 $ và cho $ K(T) $ là trường các phân thức hữu tỉ và $ U = T^p - T $. Đặt $ E = K[U] $ và $ F = K[T] $, khi đó đa thức $ f(X) = X^p - X - U $ của $ E[X] $ có các nghiệm $ T, T+1, ..., T+p-1 $ trong $ F $. Cho $ \sigma $ là tự đẳng cấu $ K $- của $ F $ sao cho $ \sigma(T) = T+1 $. Ta có $ \sigma^i(T) = T+i $ và $ \sigma(U) = U $. Nhóm $ G = \{ 1, \sigma, ..., \sigma^{p-1} \} $ là cyclic có cấp $ p $, và trường các bất biến của nó chứa $ E $; vì $ [F : E] \leq p $, định lý Dedekind (V, p. 27, Hệ quả 2) suy ra rằng $ E $ là trường các bất biến của $ G $ và $ [F : E] = p $. Do đó đa thức $ f $ bất khả quy trong $ E[X] $; mở rộng $ F $ của $ E $ là Galois, nhóm Galois $ G $ của nó là cyclic có cấp $ p $, và nhóm $ \Gamma $ là nhóm các phép hoán vị cyclic của $ T, T+1, ..., T+p-1 $.

Để xem một phép tổng quát hóa của ví dụ này, xem V, p. 93, Ví dụ 2.

#### Ví dụ 5 {#alg-v-s10-n2-exa-5 .statement}

Cho $ F = K(X_1, ..., X_n) $ là trường các phân thức hữu tỉ theo $ n $ bất định $ X_1, ..., X_n $ với các hệ số trong $ K $. Đặt
$$
s_k = \sum_{1 \leq i_1 < ... < i_k \leq n} X_{i_1} ... X_{i_k}
$$
với $ 1 \leq k \leq n $ và $ E = K(s_1, ..., s_n) $; ta ký hiệu đa thức $ f(T) $ là
$$
T^n - s_1 T^{n-1} + \cdots + (-1)^n s_n .
$$
Ta có $ f(T) = \prod_{i=1}^n (T - X_i) $, do đó $ F $ là một trường phân rã của đa thức tách được $ f(T) \in E[T] $. Hơn nữa, với mỗi phép hoán vị $ a \in \mathfrak{S}_n $ tồn tại duy nhất một tự đẳng cấu $ K $-tự đẳng cấu $ h_a $ của $ F $ sao cho $ h_a(X_i) = X_{a(i)} $ với $ 1 \leq i \leq n $; ta có $ h_a(s_k) = s_k $ với $ 1 \leq k \leq n $, do đó $ h_a $ là một $ E $-tự đẳng cấu của $ F $. Nói cách khác, $ F $ là một mở rộng Galois của $ E $ và phép hạn chế lên tập hợp các nghiệm $ \{ X_1, ..., X_n \} $ của $ f(T) $ xác định một đẳng cấu từ $ \mathrm{Gal}(F/E) $ lên nhóm $ \mathfrak{S}_n $. Đặc biệt, $ E $ gồm các phân thức hữu tỉ $ f $ sao cho
$$
f(X_{\sigma(1)}, ..., X_{\sigma(n)}) = f(X_1, ..., X_n)
$$
với mọi $ \sigma \in \mathfrak{S}_n $ (xem IV, p. 67, Hệ quả).

#### Ví dụ 6 {#alg-v-s10-n2-exa-6 .statement}

Giả sử rằng f là đơn thức với bậc > 0 và K có đặc số ≠ 2. Định nghĩa trên A một thứ tự toàn phần, ký hiệu bởi ≤, và đặt δ(f) = $ \prod_{\alpha < \beta} (\beta - a) $, $ (\alpha, \beta) \in A \times A $, và với mỗi $ \sigma \in \mathfrak{S}_A $ đặt $ \delta_\sigma(f) = \prod_{\alpha < \beta} (\sigma(\beta) - \sigma(\alpha)) $. Ta có $ \delta_\sigma(f) = \varepsilon(u) \delta(f) $, trong đó $ \varepsilon(u) $ là dấu của $ \sigma $ (I, p. 64) và $ \delta(f) \neq 0 $. Với mọi $ \tau \in \mathrm{Gal}(N/K) $ ta có $ \tau(\delta(f)) = \delta_{\tau|_A}(f) $. Do đó $ \Gamma $ được chứa trong nhóm phản xứng $ \mathfrak{A}_A $ khi và chỉ khi $ \delta(f) \in K $. Hơn nữa $ \delta(f)^2 = \prod_{\alpha < \beta} (\beta - a)' = d(f) $ là biệt thức của đa thức f (IV, p. 81). Do đó $ \Gamma \subset \mathfrak{A}_A $ khi và chỉ khi $ d(f) $ là bình phương của một phần tử của K. Vì vậy trong Ví dụ 2 ta có $ d(f) = 49 = 7^2 $ và trong Ví dụ 3, $ d(f) = -108 $ (IV, p. 85).

Cho N là một mở rộng Galois của K và L là một mở rộng con của N, Galois trên K. Mọi K-tự đẳng cấu $ \sigma $ của N cảm sinh một K-tự đẳng cấu $ \sigma_L $ của L (V, p. 55, Nhận xét 1). Do đó ánh xạ $ \sigma \mapsto \sigma_L $ là một đồng cấu của $ \mathrm{Gal}(N/K) $ vào $ \mathrm{Gal}(L/K) $, gọi là đồng cấu hạn chế.

#### Mệnh đề 3 {#alg-v-s10-prop-3 .statement}

— *Đồng cấu hạn chế* của $ \mathrm{Gal}(N/K) $ vào $ \mathrm{Gal}(L/K) $ *là toàn ánh*.

Nói chung, xét hai mở rộng con L và L' của N, và một đẳng cấu K $ u $ của L lên L'. Chọn một bao đóng đại số $ \Omega $ của K chứa N như một mở rộng con (V, p. 23, Đ.lý 2). Có một tự đẳng cấu K $ v $ của $ \Omega $ trùng với $ u $ trên L (V, p. 52, Mệnh đề 1), và vì N là một mở rộng quasi-Galois của K, $ v $ cảm sinh một tự đẳng cấu K $ \sigma $ của N (V, p. 55, Nhận xét 1). Nói cách khác, phần tử $ \sigma $ của $ \mathrm{Gal}(N/K) $ trùng với $ u $ trên L.

### 3. Tôpô của nhóm Galois

Cho N là một mở rộng Galois của K và $ \Gamma $ là nhóm Galois của N trên K. Ta trang bị cho N tôpô rời rạc, tập hợp $ N^N $ của tất cả các ánh xạ từ N vào chính nó với tôpô tích của các tôpô rời rạc của các nhân tử ("tôpô của sự hội tụ đơn giản trong N") và nhóm $ \Gamma $ với tôpô cảm sinh từ $ N^N $.

Cho A là tập hợp tất cả các mở rộng con của N có bậc hữu hạn trên K. Với $ \sigma \in \Gamma $ và $ E \in A $ ta sẽ viết $ U_E(\sigma) $ cho tập hợp các phần tử $ \tau $ của $ \Gamma $ có cùng hạn chế như $ \sigma $ lên E. Nếu $ E = K(x_1, ..., x_n) $, tập hợp $ U_E(\sigma) $ gồm các phần tử $ \tau \in \Gamma $ sao cho $ \tau(x_i) = \sigma(x_i), ..., \tau(x_n) = \sigma(x_n) $. Suy ra rằng họ $ (U_F(\sigma))_{F \in \mathcal{F}} $ là một cơ sở của lọc các lân cận của $ \sigma $ trong $ \Gamma $.

Khi N có bậc hữu hạn trên K, ta có $ N \in A $ và $ U_N(\sigma) = \{\sigma\} $, do đó tôpô của $ \mathrm{Gal}(N/K) $ là rời rạc; ta nhắc lại (V, p. 58), rằng nhóm $ \mathrm{Gal}(N/K) $ là hữu hạn trong trường hợp này.

Mô tả này về tôpô của $ \mathrm{Gal}(N/K) $ chỉ ra rằng *đồng cấu hạn chế* của $ \mathrm{Gal}(N/K) $ *lên* $ \mathrm{Gal}(L/K) $ *là liên tục* đối với mọi mở rộng con L của N là Galois trên N.

Cho $ A $ là một tập con của $ \Gamma $. Nói rằng $ A $ là mở có nghĩa là với mỗi $ \sigma \in A $ tồn tại $ E $ trong $ A $ sao cho tập hợp $ U_E(\sigma) $ được chứa trong $ A $. Bao đóng $ \overline{A} $ của $ A $ gồm tất cả các $ \sigma \in \Gamma $ sao cho với mọi $ E \in A $ tồn tại $ \tau \in A $ có cùng hạn chế lên $ E $ như $ \sigma $; trường bất biến của $ \overline{A} $ giống với trường bất biến của $ A $.

Cho $ \varepsilon $ là phần tử trung hòa của $ \Gamma $ và cho $ A' $ là tập hợp các mở rộng con của $ N $ là Galois và có bậc hữu hạn trên $ K $. Theo Mệnh đề 2 (V, p. 57), tập hợp $ A' $ là đồng biên trong $ A $ và họ $ (U_E(\varepsilon))_{E \in A'} $ do đó là một cơ sở của bộ lọc các lân cận của $ \varepsilon $ trong $ \Gamma $. Hơn nữa, với $ E \in A' $, tập hợp $ U_E(E) $ là hạt nhân của đồng cấu hạn chế của $ \mathrm{Gal}(N/K) = \Gamma $ vào $ \mathrm{Gal}(E/K) $. Vì $ \mathrm{Gal}(E/K) $ hữu hạn, suy ra $ U_{\Gamma}(\varepsilon) $ là một nhóm con vừa mở vừa đóng, chuẩn tắc và có chỉ số hữu hạn trong $ \Gamma $.

Rõ ràng ta có $ U_{\Gamma}(\sigma) = \sigma U_{\Gamma}(\varepsilon) = U_{\Gamma}(\varepsilon) \sigma $ với $ \sigma \in \Gamma $ và $ E \in A' $. Vì $ U_{\Gamma}(\varepsilon) $ là một nhóm con chuẩn tắc của $ \Gamma $ với mọi $ E \in A' $ và họ $ (U_E(\varepsilon))_{E \in A'} $ là một cơ sở các lân cận tại $ \varepsilon $, tôpô của $ \Gamma $ tương thích với cấu trúc nhóm (Gen. Top., III, p. 223). Nói cách khác, ánh xạ $ (\sigma, \tau) \mapsto \sigma \tau^{-1} $ của $ \Gamma \times \Gamma $ vào $ \Gamma $ là liên tục.

#### Mệnh đề 4 {#alg-v-s10-prop-4 .statement}

— Cho $ N $ là một mở rộng Galois của $ K $. Khi đó nhóm Galois $ \Gamma = \mathrm{Gal}(N/K) $ là compact và hoàn toàn không liên thông.

Mọi phần tử $ \sigma $ của $ \Gamma $ có một cơ sở lân cận gồm các tập mở và đóng $ U_E(\sigma) $, do đó $ \Gamma $ là hoàn toàn không liên thông (Gen. Top., I, p. 111). Ta có $ \{\sigma\} = \bigcap_{E \in \Lambda} U_E(\sigma) $, do đó $ \Gamma $ là tách. Với mỗi $ x \in N $ tập hợp các liên hợp $ \sigma(x) $ của $ x $, khi $ \sigma $ chạy qua $ \Gamma $, là *hữu hạn* vì $ x $ là đại số trên $ K $ (V, p. Hệ quả 1); do đó tất cả các phép chiếu của $ \Gamma $ lên các không gian nhân tử của $ N^N $ đều là các tập hữu hạn, và điều này chỉ ra rằng $ \Gamma $ là tương đối compact trong $ N^N $ (Gen. Top., I, p. 88). Còn lại là chỉ ra rằng $ \Gamma $ là đóng trong $ N^N $. Bây giờ nếu $ u $ thuộc bao đóng của $ \Gamma $ trong $ N^N $, thì với mỗi cặp điểm $ (x, y) $ của $ N $ tồn tại $ a \in \Gamma $ sao cho $ u(x) = \sigma(x), \ u(y) = \sigma(y), \ u(x+y) = \sigma(x+y), \ u(xy) = \sigma(xy) $, do đó $ u(x+y) = u(x) + u(y) $ và $ u(xy) = u(x)u(y) $. Theo cùng một lập luận ta có $ u(x) = x $ với mọi $ x \in K $, do đó $ u $ là một $ K $-đồng cấu của $ N $ vào $ N $; vì $ N $ là đại số trên $ K $, $ u $ là một $ K $-tự đẳng cấu của $ N $ (V, p. 52, Mệnh đề 1), do đó $ u \in T $.

Cho $ N $ là một mở rộng Galois của $ K $ và $ (N_i)_{i \in I} $ là một họ có hướng tăng của các mở rộng con của $ N $. Giả sử rằng $ N_i $ là Galois trên $ K $ với mọi $ i \in I $ và $ N = \bigcup_{i \in I} N_i $. Với mỗi $ i \in I $, ký hiệu $ \Gamma_i $ là nhóm Galois của $ N_i $ trên $ K $; với $ i \leq j $ trong $ I $, ta có $ N_i \subset N_j $ và đồng cấu hạn chế $ \varphi_{ij} $ của $ \Gamma_j $ vào $ \Gamma_i $ được xác định. Nó liên tục và do đó họ $ (\Gamma_i, \varphi_{ij}) $ là một hệ ngược của các nhóm tôpô. Hơn nữa, với mỗi $ i \in I $, ký hiệu $ \lambda_i $ là đồng cấu hạn chế của $ \mathrm{Gal}(N/K) $ vào $ \mathrm{Gal}(N_i/K) = \Gamma_i $; nó liên tục và ta có $ \lambda_i = \varphi_{ij} \circ \lambda_j $ với $ i \leq j $, do đó họ $ (\lambda_i)_{i \in I} $ xác định một đồng cấu liên tục $ \Lambda $ của $ \mathrm{Gal}(N/K) $ vào $ \varprojlim \Gamma_i $.

#### Mệnh đề 5 {#alg-v-s10-prop-5 .statement}

— *Đồng cấu* $ \lambda $ *của* $ \mathrm{Gal}(N/K) $ *vào* $ \varprojlim \mathrm{Gal}(N_i/K) $ *là một đẳng cấu của các nhóm tôpô*.

Vì $ \mathrm{Gal}(N/K) $ là compact, $ \lambda $ liên tục và nhóm $ \varprojlim \mathrm{Gal}(N_i/K) $ là tách được, chỉ cần chứng minh rằng $ h $ là song ánh (*Gen. Top.*, *I*, p. 87, Hệ quả 2). Cho $ u = (u_i)_{i \in I} $ là một phần tử của $ \varprojlim \mathrm{Gal}(N_i/K) $; với mỗi $ i \in I $, $ u_i $ là một K-tự đẳng cấu của $ N_i $ và $ u_i $ là hạn chế của $ u_j $ xuống $ N_i $ với $ i \leq j $. Vì $ N = \bigcup_{i \in I} N_i $, tồn tại một phần tử duy nhất $ \sigma $ của $ \mathrm{Gal}(N/K) $ trùng với $ u_i $ trên $ N_i $ với mọi $ i \in I $. Do đó $ \sigma $ là phần tử duy nhất của $ \mathrm{Gal}(N/K) $ sao cho $ \lambda(u) = u $, suy ra $ \lambda $ là song ánh.

Điều này áp dụng đặc biệt khi ta lấy họ $ (N_i) $ là họ của tất cả các mở rộng con Galois hữu hạn của $ N $; khi đó mỗi nhóm $ \mathrm{Gal}(N_i/K) $ là rời rạc và hữu hạn. Nhóm tôpô $ \mathrm{Gal}(N/K) $ do đó đẳng cấu với một giới hạn ngược có hướng của các nhóm hữu hạn, được trang bị tôpô rời rạc; đôi khi nhóm này được gọi là một nhóm tôpô *profinite*.

### 4. Hạ Galois

*Trong mục này* ta ký hiệu $ N $ *là một trường*, $ \Gamma $ *là một nhóm các tự đẳng cấu của* $ N $, $ e $ *là phần tử đơn vị của* $ \Gamma $ *và* $ K $ *là trường các bất biến của* $ \Gamma $.

Cho $ V $ là một không gian vectơ trên $ N $. Ta nhắc lại (II, p. 317) rằng một *cấu trúc K* trên $ V $ là một không gian con K-vectơ $ V_0 $ của $ V $ sao cho ánh xạ K-tuyến tính $ \varphi : N \otimes_K V_0 \to V $ biến $ h \otimes x $ thành $ \lambda x $ là song ánh. Cho $ V_0 $ là một cấu trúc K như vậy; với mỗi $ \sigma \in \Gamma $ ta đặt $ u_\sigma = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) \circ \varphi^{-1} $; khi đó ta có $ u_\sigma \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{i \in I} \sigma(\lambda_i) e_i $ với mọi họ các phần tử $ \lambda_i $ của $ N $ và $ e_i $ của $ V_0 $, do đó ta thu được các hệ thức
$$
\begin{align*}
u_\sigma(x + y) &= u_\sigma(x) + u_\sigma(y) \\
u_\sigma(\lambda x) &= \sigma(\lambda) u_\sigma(x) \\
u_\sigma \circ u_\tau &= u_{\sigma \tau} \\
u_e &= \mathrm{Id}_V
\end{align*}
$$
với $ \sigma, \tau $ thuộc $ \Gamma $, $ x, y $ thuộc $ V $ và $ \lambda $ thuộc $ N $.

#### Mệnh đề 6 {#alg-v-s10-prop-6 .statement}

— *a)* *Cho* $ V $ *là một không gian vectơ trên* $ N $ *có một* $ K $-*cấu trúc*. *Đối với một vectơ* $ x \in V $ *để hữu tỉ trên* $ K $ *là điều kiện cần và đủ rằng* $ u_\sigma(x) = x $ *với mọi* $ \sigma \in \Gamma $. *Đối với một không gian con N-vectơ* $ W $ *của* $ V $ *để hữu tỉ trên* $ K $ *là điều kiện cần và đủ rằng* $ u_\sigma(W) \subset W $ *với mọi* $ \sigma \in \Gamma $.

*b)* *Cho* $ V_1 $ *và* $ V_2 $ *là hai không gian vectơ trên* $ N $, *mỗi không gian có một* $ K $-*cấu trúc*. *Đối với một ánh xạ tuyến tính* $ f $ *của* $ V_1 $ *vào* $ V_2 $ *để hữu tỉ trên* $ K $ *là điều kiện cần và đủ rằng* $ f(u_\sigma(x)) = u_\sigma(f(x)) $ *với mọi* $ \sigma \in \Gamma $ *và mọi* $ x \in V_1 $.

*Rõ ràng* $ K $ *là tập hợp các* $ x \in N $ *sao cho* $ \sigma(xy) = x \sigma(y) $ *với mọi* $ \sigma \in \Gamma $ *và mọi* $ y \in N $. *Do đó mệnh đề suy ra từ Định lý 1* (II, p. 324).

#### Hệ quả {#alg-v-s10-n4-cor-1 .statement}

— Cho $ V_0 $ là một không gian vectơ trên $ K $ và cho $ W $ là một không gian con-N vectơ của $ N \otimes_K V_0 $. Giả sử rằng $ W $ ổn định dưới các ánh xạ $ \sigma \otimes \mathrm{Id}_{V_0} $ với mọi $ \sigma \in \Gamma $. Gọi $ W_0 $ là tập hợp các $ x \in V_0 $ sao cho $ 1 \otimes x \in W $; khi đó $ W_0 $ là không gian con-K vectơ duy nhất của $ V_0 $ sao cho $ W = N \otimes_K W_0 $.

Chỉ cần nhận xét rằng tập hợp các phần tử có dạng $ 1 \otimes x \ (x \in V_0) $ là một cấu trúc-K trên $ N \otimes_K V_0 $ mà trên đó ta có $ u_\sigma = \sigma \otimes \mathrm{Id}_{V_0} $ với $ \sigma \in \Gamma $.

#### Mệnh đề 7 {#alg-v-s10-prop-7 .statement}

— Cho $ V $ là một không gian vectơ trên $ N $, $ (u_\sigma)_\sigma $, r là một họ các ánh xạ của $ V $ vào chính nó thỏa mãn (1) đến (4) và $ V_0 $ là tập hợp các $ x \in V $ sao cho $ u_\sigma(x) = x $ với mọi $ \sigma \in \Gamma $.

a) $ V_0 $ là một không gian con-K vectơ của $ V $ và ánh xạ K-tuyến tính $ \varphi $ từ $ N \otimes_K V_0 $ vào $ V $, biến $ \lambda \otimes x $ thành $ \lambda x $, là đơn ánh.

b) Nếu $ \Gamma $ hữu hạn, thì $ \varphi $ là song ánh và $ V_0 $ là một cấu trúc-K trên $ V $.

Rõ ràng $ V_0 $ là một không gian con-K vectơ của $ V $.

Công thức $ u_\sigma \circ \varphi = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) $ cho thấy hạt nhân $ W $ của $ \varphi $ ổn định dưới các ánh xạ $ \sigma \otimes \mathrm{Id}_{V_0} $; do Hệ quả của Mệnh đề 6, do đó tồn tại một không gian con $ W_0 $ của $ V_0 $ sao cho $ W = N \otimes_K W_0 $. Nếu $ x $ thuộc $ W_0 $ thì ta có $ x = \varphi(1 \otimes x) = 0 $, suy ra $ W_0 = 0 $ và do đó $ W = 0 $. Điều này chứng minh $ a) $.

Giả sử $ \Gamma $ là hữu hạn; ta phải chứng minh rằng $ \varphi $ là toàn ánh, hay tương đương rằng $ V_0 $ sinh ra không gian vectơ N $ V $. Do đó, cho $ f $ là một dạng N-tuyến tính trên $ V $ mà hạn chế của nó lên $ V_0 $ bằng không. Cho $ x \in V $; với mọi $ A \in N $ phần tử $ y, = \sum_{\sigma \in \Gamma} u_\sigma(\lambda x) $ của $ V $ rõ ràng thuộc $ V_0 $, do đó $ f(y,) = 0 $, nghĩa là,
$$
\sum_{\sigma \in \Gamma} f(u_\sigma(x)) \sigma(A) = 0.
$$
Theo định lý Dedekind (V, p. 27, Hệ quả 2), do đó ta có $ f(u_\sigma(x)) = 0 $ với mỗi $ \sigma \in \Gamma $; đặc biệt, lấy $ \sigma = \varepsilon $ ta được $ f(x) = 0 $, điều này có nghĩa là $ f = 0 $. Điều này chứng minh $ b) $.

Cho $ M $ là một không gian vectơ trên $ N $; với mỗi $ \sigma \in \Gamma $, cho $ M^\sigma $ là không gian vectơ trên $ N $ có cùng nhóm cộng cơ sở như $ M $, với phép toán ngoài $ (A, x) \mapsto \sigma(\lambda) x $. Viết $ V = \prod_{\sigma \in \Gamma} M^\sigma $; nhóm cộng cơ sở của $ V $ là nhóm của tất cả các ánh xạ từ $ \Gamma $ vào $ M $, với phép toán ngoài được định nghĩa bởi
$$
(\lambda . h)(\sigma) = \sigma(\lambda) h(\sigma) \quad (\lambda \in N, h \in V, \sigma \in \Gamma).
$$
(Tích $ \sigma(\lambda) h(\sigma) $ được tính trong không gian vectơ $ M $.) Hơn nữa, ta định nghĩa trên $ N \otimes_K M $ một cấu trúc không gian vectơ trên $ N $ bởi công thức
$$
\lambda \left( \sum_i \mu_i \otimes x_i \right) = \sum_i \lambda \mu_i \otimes x_i
$$
Cuối cùng, ta ký hiệu $ \psi $ là ánh xạ K-tuyến tính từ $ N \otimes_K M $ vào $ V $ được đặc trưng bởi quan hệ
$$
\psi(\lambda \otimes x)(\sigma) = \sigma(\lambda) . x
$$
với $ A \in N, x \in M $ và $ \sigma \in \Gamma $. Rõ ràng $ \psi $ là N-tuyến tính

#### Mệnh đề 8 {#alg-v-s10-prop-8 .statement}

— *Ánh xạ N-tuyến tính* $ \psi $ *từ* $ N \otimes_K M $ *vào* $ V = \prod_{\sigma \in \Gamma} M^\sigma $ *là đơn ánh, và là song ánh nếu* $ \Gamma $ *hữu hạn.*

Với mọi $ a \in \Gamma $, ta định nghĩa một ánh xạ $ u_\sigma $ từ $ V $ vào $ V $ bởi

$$
(u_\sigma h)(\tau) = h(\tau \sigma)
$$

cho $ h \in V $ và $ \tau \in \Gamma $. Việc kiểm tra *(1)-(4)* là ngay lập tức. Ký hiệu $ V $, tập hợp các $ h \in V $ sao cho $ u_\sigma(h) = h $ với mọi $ \sigma \in \Gamma $. Với mỗi $ x \in M $, đặt $ \theta(x) $ là ánh xạ hằng từ $ \Gamma $ vào $ M $ nhận giá trị $ x $; khi đó $ \theta $ là một K-đẳng cấu của $ M $ lên $ V $. Nếu ta định nghĩa đồng cấu $ \varphi : N \otimes_K V, \to V $ như trên, ta có $ \psi = \varphi \circ (\mathrm{Id}_N \otimes \theta) $ và khi đó Mệnh đề 8 suy ra từ Mệnh đề 7.

#### Hệ quả {#alg-v-s10-n4-cor-2 .statement}

— *Cho* $ \psi $ *là ánh xạ K-tuyến tính từ* $ N \otimes_K N $ *vào không gian vectơ tích* $ N^\Gamma $ *sao cho* $ \psi(x \otimes y)\,(a) = \sigma(x)\,y $ *với* $ x,\,y $ *thuộc* $ N $ *và* $ \sigma \in \Gamma $. *Khi đó* $ \psi $ *là đơn ánh và là song ánh khi* $ \Gamma $ *hữu hạn.*

Đây là trường hợp riêng $ M = N $ của Mệnh đề 8.

#### Nhận xét 1 {#alg-v-s10-n4-rem-1 .statement}

Cho F là một mở rộng của K và $ N $ là một mở rộng con của F, và cho $ \Gamma $ là một nhóm *hữu hạn* các tự đẳng cấu của $ N $, mà K là trường bất biến. Mệnh đề 8 suy ra sự tồn tại của một đẳng cấu các K-đại số $ 0 : N \otimes_F F \to F^\Gamma $ được đặc trưng bởi $ \theta(x \otimes y)\,(a) = \sigma(x)\,y $ với $ x \in N,\,y \in F $ và $ \sigma \in \Gamma $.

#### Nhận xét 2 {#alg-v-s10-n4-rem-2 .statement}

Ký hiệu K, N và $ \Gamma $ có cùng ý nghĩa như trước. Với mỗi số nguyên $ n \geqslant 1 $, cho $ A_n $ là tích tenxơ của n K-đại số đồng nhất với $ N $; cho $ B_n $ là tập hợp các ánh xạ từ $ \Gamma^{n-1} $ vào $ N $. Bằng quy nạp theo $ n $, ta suy ra từ Hệ quả của Mệnh đề 8 sự tồn tại của một đẳng cấu $ \varphi_n : A_n \to B_n $, ánh xạ $ x_1 \otimes \ldots \otimes x_n $ thành hàm $ (\sigma_1, \ldots, a, ) \quad \sigma_1(x_1) \cdot \sigma_n(x_{n-1})\,x_n $.

### 5. *Đối đồng điều Galois*

Cho $ N $ là một trường, $ \Gamma $ là một nhóm *hữu hạn* các tự đẳng cấu của $ N $ và K là trường bất biến của $ \Gamma $. Với mỗi số nguyên $ n \geqslant 1 $, ta ký hiệu $ \mathbf{GL}(n, N) $ là nhóm các ma trận vuông cấp $ n $ với các hệ số trong $ N $ và định thức khác không (II; p. 349). Ta cho nhóm $ \Gamma $ tác động lên nhóm $ \mathbf{GL}(n, N) $ theo quy tắc $ \sigma(A) = (\sigma(a_{ij})) $ với $ A = (a_{ij}) $.

#### Mệnh đề 9 {#alg-v-s10-prop-9 .statement}

— *Cho* $ (U_\sigma)_{\sigma \in \Gamma} $ *là một họ các phần tử của* $ \mathbf{GL}(n, N) $. *Để tồn tại* $ A $ *trong* $ GL(n, N) $ *sao cho* $ U_\sigma = A^{-1}\,a(A) $ *với mọi* $ \sigma \in \Gamma $ *là điều kiện cần và đủ để* $ U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau) $ *với* $ \sigma,\,\tau $ *trong* $ \Gamma $.

Điều kiện là *cần*: nếu $ U_\sigma = A^{-1}\,a(A) $, thì ta có

$$
U_\sigma \cdot \sigma(U_\tau) = A^{-1}\,\sigma(A)\,\sigma(A^{-1}\,\tau(A)) = A^{-1}\sigma\tau(A) = U_{\sigma \tau}.
$$

Điều kiện là *đủ*: ta đồng nhất các phần tử của $ N^n $ với các ma trận có $ n $ hàng và một cột với các hệ số trong $ N $. Ta cho các nhóm $ \Gamma $ tác động lên $ N^n $ bởi
$$
\sigma(x) = (\sigma(x_i))_{1 \leq i \leq n} \quad \text{với} \quad x = (x_i)_{1 \leq i \leq n}.
$$
Với mỗi $ a \in \Gamma $, ta ký hiệu $ u_\sigma $ là ánh xạ $ x \mapsto U_\sigma \cdot \sigma(x) $ của $ N^n $ vào chính nó. Việc kiểm tra các Công thức (1) đến (3) của V, p. 62 là ngay lập tức. Hơn nữa ta có $ u_\varepsilon \circ u_\varepsilon = u_\varepsilon $ và vì $ u_\varepsilon $ là song ánh, ta có $ u_\varepsilon = \mathrm{Id}_{N^n} $. Gọi $ V_0 $ là tập hợp các vectơ $ x \in N^n $ sao cho $ u_\sigma(x) = x $ với mọi $ \sigma \in \Gamma $. Theo Mệnh đề 7 (V, p. 63), $ V_0 $ là một cấu trúc K trên $ N^n $; đặc biệt tồn tại trong $ V_0 $ các vectơ $ b_1, \ldots, b_n $ lập thành một cơ sở của $ N^n $ trên $ N $. Do đó ma trận $ B $ có các cột $ b_1, \ldots, b_n $ là khả nghịch và quan hệ $ u_\sigma(b_i) = b_i $ với $ 1 \leq i \leq n $ tương đương với $ U_\sigma \cdot \sigma(B) = B $. Đặt $ A = B^{-1} $, ta thu được $ U_\sigma = A^{-1} \sigma(A) $ với mọi $ a \in \Gamma $.

#### Hệ quả 1 {#alg-v-s10-prop-9-cor-1 .statement}

*Cho $ (c,) $, , , là một họ các phần tử khác không của $ N $. Để tồn tại $ a \neq 0 $ trong $ N $ sao cho $ c, = \sigma(a) \cdot a' $ với mọi $ a \in \Gamma $ là điều kiện cần và đủ để $ c, = c, \cdot a(c,) $ với $ \sigma, \tau $ trong $ \Gamma $.*

#### Hệ quả 2 {#alg-v-s10-prop-9-cor-2 .statement}

*Cho $ (c,) $, $ \Gamma $ là một họ các phần tử của $ N $. Để $ b $ tồn tại trong $ N $ sao cho $ a, = \sigma(b) - b $ với mọi $ a \in \Gamma $, điều kiện cần và đủ là $ a, = a, + \sigma(a_\tau) $ với $ a, \tau $ thuộc $ \Gamma $.*

Ta có $ \sigma \tau(b) - b = [\sigma(b) - b]^+ \sigma[\tau(b) - b] $ với mọi $ b $ thuộc $ N $ và $ a, \tau $ thuộc $ \Gamma $, do đó điều kiện là cần thiết.

Ngược lại, giả sử $ a, = a, + \sigma(a_\tau) $ với mọi $ a $ và $ \tau $ thuộc $ \Gamma $. Đặt $ U_\sigma = \begin{pmatrix} 1 & a_\sigma \\ 0 & 1 \end{pmatrix} $ với $ \sigma \in \Gamma $; khi đó ta có $ U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau) $ với $ \sigma, \tau $ thuộc $ \Gamma $; theo Mệnh đề 9, do đó tồn tại một ma trận $ A = \begin{pmatrix} x & y \\ z & t \end{pmatrix} $ có định thức khác không sao cho $ \sigma(A) = A U_\sigma $ với mọi $ a \in \Gamma $; viết quan hệ $ \sigma(A) = A U_\sigma $ ta được
$$
\begin{pmatrix} \sigma(x) & \sigma(y) \\ \sigma(z) & \sigma(t) \end{pmatrix} = \begin{pmatrix} x & x a_\sigma + y \\ z & z a_\sigma + t \end{pmatrix} \quad (\sigma \in \Gamma).
$$
Đặc biệt, $ x $ và $ z $ thuộc $ K $ và ta có
$$
\sigma(y) = x a_\sigma + y, \quad \sigma(t) = z a_\sigma + t \quad (\sigma \in \Gamma).
$$
Nếu $ x \neq 0 $ thì ta có $ a, = \sigma(b) - b $ với $ b = x^{-1} y $; nếu $ z \neq 0 $, ta có cùng quan hệ với $ b = z^{-1} t $. Bây giờ $ x $ và $ z $ không thể đồng thời bằng không vì
$$
xt - yz = \det A \neq 0.
$$

### 6. Định lý của Artin

**Định lý 2 (Artin).** — *Cho $ N $ là một trường, $ \Gamma $ là một nhóm các tự đẳng cấu của $ N $ và $ K $ là trường các bất biến của $ \Gamma $. Cho $ V $ là một không gian vectơ con trên K của $ N $ có số chiều hữu hạn* trên K. Khi đó mọi ánh xạ K-tuyến tính u của V vào N đều là một tổ hợp tuyến tính với các hệ số trong N của các hạn chế trên V của các phần tử của $ \Gamma $.

Cuối cùng, c) suy ra từ Định lý 2 (V, p. 65), định lý chứng minh sự tồn tại của một họ (a,,), ,, sao cho $ u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x) $ (với mọi $ x \in N $), và từ định lý Dedekind (V, p. 27, Hệ quả 2), định lý chứng minh tính duy nhất của (a,,), ,$ \Gamma $.

### 7. Định lý cơ bản của lý thuyết Galois

#### Định lý 4 {#alg-v-s10-thm-4 .statement}

— Cho N là một mở rộng Galois của K và $ \Gamma $ là nhóm Galois của nó. Gọi $ \mathcal{K} $ là tập hợp các mở rộng con của N và $ \mathcal{G} $ là tập hợp các nhóm con đóng của $ \Gamma $. Với mỗi nhóm con $ A \in \mathcal{G} $, ta ký hiệu $ k(\Delta) $ là trường các bất biến của A và với mỗi *trường con* $ E \in \mathcal{K} $, ta ký hiệu $ g(E) $ là nhóm các *tự đẳng cấu* E của N. *Khi đó* $ A \mapsto k(\Delta) $ là một song ánh của $ \mathcal{G} $ lên $ \mathcal{K} $, và $ E \mapsto g(E) $ là song ánh ngược.

A) Quan hệ $ E = k(g(E)) $ (với $ E \in \mathcal{K} $) là một hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 1 {#alg-v-s10-lem-1 .statement}

Cho E là một mở rộng con của N. Khi đó N là một mở rộng Galois của E và $ \mathrm{Gal}(N/E) $ là một nhóm con đóng của $ \mathrm{Gal}(N/K) $ với tôpô cảm sinh.

Cho $ x \in N $; đa thức tối tiểu f của x trên E chia trong $ E[X] $ đa thức tối tiểu $ g $ của x trên K (V, p. 17, Hệ quả 2). Vì N là Galois trên K, đa thức g là một tích trong $ N[X] $ của các nhân tử phân biệt bậc 1; do đó f cũng như vậy và N là Galois trên E.

Gọi $ \Gamma $ là nhóm Galois của N trên K và A là nhóm Galois của N trên E. Theo định nghĩa, A là nhóm con của $ \Gamma $ gồm tất cả các $ \sigma $ sao cho $ \sigma(x) = x $ với mọi $ x \in E $. Bây giờ, với mỗi $ x \in E $, ánh xạ $ \sigma \mapsto \sigma(x) $ từ $ \Gamma $ vào không gian rời rạc N là liên tục, do đó D là đóng trong $ \Gamma $. Cho $ \sigma \in \Gamma $; với $ x_1, \ldots, x_n $ thuộc N, gọi $ U(x_1, \ldots, x_n) $ là tập hợp tất cả các $ \tau \in \Gamma $ sao cho $ \tau(x_i) = \sigma(x_i) $ với $ 1 \leq i \leq n $; đặt

$$
V(x_1, \ldots, x_n) = U(x_1, \ldots, x_n) \cap \Delta.
$$

Khi đó họ các tập hợp $ U(x_1, \ldots, x_n) $ (tương ứng $ V(x_1, \ldots, x_n) $) là một cơ sở các lân cận của $ \sigma $ trong $ \Gamma $ (tương ứng A). Do đó tôpô trên A là tôpô cảm sinh bởi $ \Gamma $.

B) Quan hệ $ A = g(k(\Delta)) $ (với $ A \in g $) là một hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 2 {#alg-v-s10-lem-2 .statement}

Cho A là một nhóm con của $ \Gamma $. Gọi E là trường các bất biến của A; khi đó nhóm Galois của N trên E là bao đóng của A trong $ \Gamma $.
