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
      title: Finite $\Gamma$-sets and etale algebras
      page: 75
      pdf_page: 189
    - "no": 11
      title: The structure of quasi-Galois extensions
      page: 76
      pdf_page: 190
statements: 49
exercises: 23
content_sha256: d0c4fe0c62204dc7c4fe1aa11ef226cb4e3f09fb5060e8c84509337da5e516a2
translated_from: content/en/alg/V/10_s10_galois_extensions.md
source_content_sha256: 4d2ea6b2e3fe8136b4cbf004a6c050629d9e8414a0cc6650ceb165d4728343b0
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-19dbb229
glossary_version: 34
glossary_terms_sha256: d7731983bf105a6665742a828f144f0612c75b7d0959ab1ca7fe5f9be18cff84
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. CÁC MỞ RỘNG GALOIS

Trong suốt đoạn này, K ký hiệu một trường.

### 1. Định nghĩa các mở rộng Galois

#### Định lý 1 {#alg-v-s10-thm-1 .statement}

— Cho N là một mở rộng đại số của K và $\Gamma$ là nhóm các tự đẳng cấu của N giữ K bất biến. Khi đó các mệnh đề sau là tương đương:
a) Mọi phần tử của N bất biến dưới $\Gamma$ đều thuộc ảnh của K trong N.
b) N là một mở rộng tách được quasi-Galois của K.
c) Với mỗi $x \in N$, đa thức tối tiểu của x trên K phân rã trong $N[X]$ thành một tích các đa thức phân biệt bậc 1.
Sự tương đương của b) và c) suy ra từ Hệ quả của Mệnh đề 6 (V, p. 40) và định nghĩa mở rộng quasi-Galois (V, p. 53, Định nghĩa 2). Ta đồng nhất K với ảnh chính tắc của nó trong N.
$a) \Rightarrow c)$: Giả sử K là trường các bất biến của $\Gamma$. Cho $x \in N$, với đa thức tối tiểu $f$ trên K và gọi A là tập hợp tất cả các nghiệm của f trong N. Đặt
$$
g(X) = \prod_{y \in A} (X - y).
$$
Mọi tự đẳng cấu $a \in \Gamma$ cảm sinh một phép hoán vị của A, và do đó giữ bất biến các hệ số của đa thức $g \in N[X]$. Vì vậy ta có $g \in K[X]$ và vì $g(x) = 0$, đa thức g là một bội của $f$ trong $K[X]$ (V, p. 16, Định lý 1). Hơn nữa, $f$ và g đều là đơn thức đầu và g chia hết $f$ (IV, p. 16, Mệnh đề 5); do đó ta có $f = g$, nghĩa là đa thức tối tiểu $f$ của $x$ trên $K$ là một tích trong $N[X]$ của các đa thức phân biệt bậc 1.

c) ⇒ a): cho x là một phần tử của N không thuộc K. Ký hiệu Ω là một bao đóng đại số của K chứa N như một mở rộng con (V, p. 23, Định lý 2). Gọi f là đa thức tối tiểu của x trên K, có bậc ≥ 2 theo giả thiết, và gọi A là tập hợp các nghiệm của $f(X)$ trong N. Nếu điều kiện c) được thỏa mãn, ta có $f(X) = \prod_{y \in A} (X - y)$ và do đó (V, p. 53, Hệ quả 1) A là tập hợp các liên hợp của x trong Ω. Vì f có bậc ≥ 2, tồn tại trong A một phần tử $y \neq x$, do đó tồn tại một tự đẳng cấu u của Ω giữ K bất biến sao cho $u(x) = y$. Bây giờ theo giả thiết c), mở rộng N của K là quasi-Galois, do đó $u(N) = N$ (V, p. 54, Hệ quả 1); suy ra u cảm sinh một tự đẳng cấu a của N giữ K bất biến sao cho $\sigma(x) = y \neq x$, nên K là trường các bất biến của Γ.

#### Định nghĩa 1 {#alg-v-s10-def-1 .statement}

— Một mở rộng N của K được gọi là Galois nếu nó đại số và thỏa mãn các điều kiện tương đương a), b), c) của Định lý 1.

Cho N là một trường, Γ là một nhóm các tự đẳng cấu của N và $N_0$ là trường các bất biến của Γ. Khi N là đại số trên $N_0$ thì nó là một mở rộng Galois của $N_0$. Điều này không phải lúc nào cũng đúng: chẳng hạn, giả sử K là vô hạn và lấy N là trường các phân thức K(X); với mỗi $a \in K$ gọi $\sigma_a$ là tự đẳng cấu của K(X) biến $f(X)$ thành $f(X + a)$. Tập hợp tất cả các $a$ là một nhóm các tự đẳng cấu của K(X), mà trường các bất biến của nó dễ thấy là K; tuy nhiên K(X) không đại số trên K.

Cho Ω là một bao đóng đại số của K, gọi A là một tập hợp các phần tử của Ω tách được trên K và B là tập hợp các phần tử liên hợp trên K của các phần tử của A. Khi đó B gồm các phần tử đại số và tách được trên K. Do đó (V, p. 39, Mệnh đề 6 và p. 56, Mệnh đề 5) trường K(B) là một mở rộng tách được quasi-Galois của K; nói cách khác, mở rộng quasi-Galois sinh bởi A (V, p. 55) là một mở rộng Galois của K; ta cũng sẽ nói rằng nó là mở rộng Galois của K sinh bởi tập con A của O.

Đặc biệt, trường phân rã trong Ω của một họ các đa thức tách được trên K, một bao đóng tách được của K, là các mở rộng Galois của K.

#### Mệnh đề 1 {#alg-v-s10-prop-1 .statement}

— Cho N là một mở rộng của K và $(N_i)_{i \in I}$, một họ khác rỗng các mở rộng con của N. Đặt $E = \cap_{i \in I} N_i$ và $F = K \left( \bigcup_{i \in I} N_i \right)$. Nếu tất cả các mở rộng N, đều là Galois trên K thì điều tương tự cũng đúng với E và F.

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

Giả sử rằng $K = \mathbf{Q}$ và lấy $f = X^3 - 2$. Dùng phân tích các số nguyên thành tích các nhân tử nguyên tố (I, p. 51), ta dễ dàng thấy rằng 2 không phải là lập phương của một phần tử của $\mathbf{Q}$. Do đó đa thức $f$ là bất khả quy, vì nếu không, nó sẽ có một nghiệm trong $\mathbf{Q}$. Cho $A = \{ x_1, x_2, x_3 \}$ là tập hợp các nghiệm của $f$ trong $\Omega$ và $\Gamma$ là nhóm Galois của $f$. Nó tác động bắc cầu trên $A$; do đó cấp của nó chia hết cho ba. Mặt khác, thương $j = \frac{x_2}{x_1}$ khác 1 và ta có $j^3 = 1$. Do đó $j$ thỏa mãn quan hệ $j^2 + j + 1 = 0$; nhưng đa thức $T^2 + T + 1 = \left( T + \frac{1}{2} \right)^2 + \frac{3}{4}$ không có nghiệm trong $\mathbf{Q}$, điều này cho thấy (Ví dụ 1) rằng $[\mathbf{Q}(j) : \mathbf{Q}] = 2$. Vậy $[\mathbf{N} : \mathbf{Q}]$ chia hết cho 2, và suy ra cấp của $\Gamma$ chia hết cho 6. Vì $\Gamma$ được chứa trong nhóm $\mathfrak{S}_A$ có cấp 6, ta có $\Gamma = \mathfrak{S}_A$.

#### Ví dụ 4 {#alg-v-s10-n2-exa-4 .statement}

Giả sử $K$ có đặc số $p \neq 0$ và cho $K(T)$ là trường các phân thức hữu tỉ và $U = T^p - T$. Đặt $E = K[U]$ và $F = K[T]$, khi đó đa thức $f(X) = X^p - X - U$ của $E[X]$ có các nghiệm $T, T+1, ..., T+p-1$ trong $F$. Cho $\sigma$ là tự đẳng cấu $K$- của $F$ sao cho $\sigma(T) = T+1$. Ta có $\sigma^i(T) = T+i$ và $\sigma(U) = U$. Nhóm $G = \{ 1, \sigma, ..., \sigma^{p-1} \}$ là cyclic có cấp $p$, và trường các bất biến của nó chứa $E$; vì $[F : E] \leq p$, định lý Dedekind (V, p. 27, Hệ quả 2) suy ra rằng $E$ là trường các bất biến của $G$ và $[F : E] = p$. Do đó đa thức $f$ bất khả quy trong $E[X]$; mở rộng $F$ của $E$ là Galois, nhóm Galois $G$ của nó là cyclic có cấp $p$, và nhóm $\Gamma$ là nhóm các phép hoán vị cyclic của $T, T+1, ..., T+p-1$.

Để xem một phép tổng quát hóa của ví dụ này, xem V, p. 93, Ví dụ 2.

#### Ví dụ 5 {#alg-v-s10-n2-exa-5 .statement}

Cho $F = K(X_1, ..., X_n)$ là trường các phân thức hữu tỉ theo $n$ bất định $X_1, ..., X_n$ với các hệ số trong $K$. Đặt
$$
s_k = \sum_{1 \leq i_1 < ... < i_k \leq n} X_{i_1} ... X_{i_k}
$$
với $1 \leq k \leq n$ và $E = K(s_1, ..., s_n)$; ta ký hiệu đa thức $f(T)$ là
$$
T^n - s_1 T^{n-1} + \cdots + (-1)^n s_n .
$$
Ta có $f(T) = \prod_{i=1}^n (T - X_i)$, do đó $F$ là một trường phân rã của đa thức tách được $f(T) \in E[T]$. Hơn nữa, với mỗi phép hoán vị $a \in \mathfrak{S}_n$ tồn tại duy nhất một tự đẳng cấu $K$-tự đẳng cấu $h_a$ của $F$ sao cho $h_a(X_i) = X_{a(i)}$ với $1 \leq i \leq n$; ta có $h_a(s_k) = s_k$ với $1 \leq k \leq n$, do đó $h_a$ là một $E$-tự đẳng cấu của $F$. Nói cách khác, $F$ là một mở rộng Galois của $E$ và phép hạn chế lên tập hợp các nghiệm $\{ X_1, ..., X_n \}$ của $f(T)$ xác định một đẳng cấu từ $\mathrm{Gal}(F/E)$ lên nhóm $\mathfrak{S}_n$. Đặc biệt, $E$ gồm các phân thức hữu tỉ $f$ sao cho
$$
f(X_{\sigma(1)}, ..., X_{\sigma(n)}) = f(X_1, ..., X_n)
$$
với mọi $\sigma \in \mathfrak{S}_n$ (xem IV, p. 67, Hệ quả).

#### Ví dụ 6 {#alg-v-s10-n2-exa-6 .statement}

Giả sử rằng f là đơn thức với bậc > 0 và K có đặc số ≠ 2. Định nghĩa trên A một thứ tự toàn phần, ký hiệu bởi ≤, và đặt δ(f) = $\prod_{\alpha < \beta} (\beta - a)$, $(\alpha, \beta) \in A \times A$, và với mỗi $\sigma \in \mathfrak{S}_A$ đặt $\delta_\sigma(f) = \prod_{\alpha < \beta} (\sigma(\beta) - \sigma(\alpha))$. Ta có $\delta_\sigma(f) = \varepsilon(u) \delta(f)$, trong đó $\varepsilon(u)$ là dấu của $\sigma$ (I, p. 64) và $\delta(f) \neq 0$. Với mọi $\tau \in \mathrm{Gal}(N/K)$ ta có $\tau(\delta(f)) = \delta_{\tau|_A}(f)$. Do đó $\Gamma$ được chứa trong nhóm phản xứng $\mathfrak{A}_A$ khi và chỉ khi $\delta(f) \in K$. Hơn nữa $\delta(f)^2 = \prod_{\alpha < \beta} (\beta - a)' = d(f)$ là biệt thức của đa thức f (IV, p. 81). Do đó $\Gamma \subset \mathfrak{A}_A$ khi và chỉ khi $d(f)$ là bình phương của một phần tử của K. Vì vậy trong Ví dụ 2 ta có $d(f) = 49 = 7^2$ và trong Ví dụ 3, $d(f) = -108$ (IV, p. 85).

Cho N là một mở rộng Galois của K và L là một mở rộng con của N, Galois trên K. Mọi K-tự đẳng cấu $\sigma$ của N cảm sinh một K-tự đẳng cấu $\sigma_L$ của L (V, p. 55, Nhận xét 1). Do đó ánh xạ $\sigma \mapsto \sigma_L$ là một đồng cấu của $\mathrm{Gal}(N/K)$ vào $\mathrm{Gal}(L/K)$, gọi là đồng cấu hạn chế.

#### Mệnh đề 3 {#alg-v-s10-prop-3 .statement}

— *Đồng cấu hạn chế* của $\mathrm{Gal}(N/K)$ vào $\mathrm{Gal}(L/K)$ *là toàn ánh*.

Nói chung, xét hai mở rộng con L và L' của N, và một đẳng cấu K $u$ của L lên L'. Chọn một bao đóng đại số $\Omega$ của K chứa N như một mở rộng con (V, p. 23, Đ.lý 2). Có một tự đẳng cấu K $v$ của $\Omega$ trùng với $u$ trên L (V, p. 52, Mệnh đề 1), và vì N là một mở rộng quasi-Galois của K, $v$ cảm sinh một tự đẳng cấu K $\sigma$ của N (V, p. 55, Nhận xét 1). Nói cách khác, phần tử $\sigma$ của $\mathrm{Gal}(N/K)$ trùng với $u$ trên L.

### 3. Tôpô của nhóm Galois

Cho N là một mở rộng Galois của K và $\Gamma$ là nhóm Galois của N trên K. Ta trang bị cho N tôpô rời rạc, tập hợp $N^N$ của tất cả các ánh xạ từ N vào chính nó với tôpô tích của các tôpô rời rạc của các nhân tử ("tôpô của sự hội tụ đơn giản trong N") và nhóm $\Gamma$ với tôpô cảm sinh từ $N^N$.

Cho A là tập hợp tất cả các mở rộng con của N có bậc hữu hạn trên K. Với $\sigma \in \Gamma$ và $E \in A$ ta sẽ viết $U_E(\sigma)$ cho tập hợp các phần tử $\tau$ của $\Gamma$ có cùng hạn chế như $\sigma$ lên E. Nếu $E = K(x_1, ..., x_n)$, tập hợp $U_E(\sigma)$ gồm các phần tử $\tau \in \Gamma$ sao cho $\tau(x_i) = \sigma(x_i), ..., \tau(x_n) = \sigma(x_n)$. Suy ra rằng họ $(U_F(\sigma))_{F \in \mathcal{F}}$ là một cơ sở của lọc các lân cận của $\sigma$ trong $\Gamma$.

Khi N có bậc hữu hạn trên K, ta có $N \in A$ và $U_N(\sigma) = \{\sigma\}$, do đó tôpô của $\mathrm{Gal}(N/K)$ là rời rạc; ta nhắc lại (V, p. 58), rằng nhóm $\mathrm{Gal}(N/K)$ là hữu hạn trong trường hợp này.

Mô tả này về tôpô của $\mathrm{Gal}(N/K)$ chỉ ra rằng *đồng cấu hạn chế* của $\mathrm{Gal}(N/K)$ *lên* $\mathrm{Gal}(L/K)$ *là liên tục* đối với mọi mở rộng con L của N là Galois trên N.

Cho $A$ là một tập con của $\Gamma$. Nói rằng $A$ là mở có nghĩa là với mỗi $\sigma \in A$ tồn tại $E$ trong $A$ sao cho tập hợp $U_E(\sigma)$ được chứa trong $A$. Bao đóng $\overline{A}$ của $A$ gồm tất cả các $\sigma \in \Gamma$ sao cho với mọi $E \in A$ tồn tại $\tau \in A$ có cùng hạn chế lên $E$ như $\sigma$; trường bất biến của $\overline{A}$ giống với trường bất biến của $A$.

Cho $\varepsilon$ là phần tử trung hòa của $\Gamma$ và cho $A'$ là tập hợp các mở rộng con của $N$ là Galois và có bậc hữu hạn trên $K$. Theo Mệnh đề 2 (V, p. 57), tập hợp $A'$ là đồng biên trong $A$ và họ $(U_E(\varepsilon))_{E \in A'}$ do đó là một cơ sở của bộ lọc các lân cận của $\varepsilon$ trong $\Gamma$. Hơn nữa, với $E \in A'$, tập hợp $U_E(E)$ là hạt nhân của đồng cấu hạn chế của $\mathrm{Gal}(N/K) = \Gamma$ vào $\mathrm{Gal}(E/K)$. Vì $\mathrm{Gal}(E/K)$ hữu hạn, suy ra $U_{\Gamma}(\varepsilon)$ là một nhóm con vừa mở vừa đóng, chuẩn tắc và có chỉ số hữu hạn trong $\Gamma$.

Rõ ràng ta có $U_{\Gamma}(\sigma) = \sigma U_{\Gamma}(\varepsilon) = U_{\Gamma}(\varepsilon) \sigma$ với $\sigma \in \Gamma$ và $E \in A'$. Vì $U_{\Gamma}(\varepsilon)$ là một nhóm con chuẩn tắc của $\Gamma$ với mọi $E \in A'$ và họ $(U_E(\varepsilon))_{E \in A'}$ là một cơ sở các lân cận tại $\varepsilon$, tôpô của $\Gamma$ tương thích với cấu trúc nhóm (Gen. Top., III, p. 223). Nói cách khác, ánh xạ $(\sigma, \tau) \mapsto \sigma \tau^{-1}$ của $\Gamma \times \Gamma$ vào $\Gamma$ là liên tục.

#### Mệnh đề 4 {#alg-v-s10-prop-4 .statement}

— Cho $N$ là một mở rộng Galois của $K$. Khi đó nhóm Galois $\Gamma = \mathrm{Gal}(N/K)$ là compact và hoàn toàn không liên thông.

Mọi phần tử $\sigma$ của $\Gamma$ có một cơ sở lân cận gồm các tập mở và đóng $U_E(\sigma)$, do đó $\Gamma$ là hoàn toàn không liên thông (Gen. Top., I, p. 111). Ta có $\{\sigma\} = \bigcap_{E \in \Lambda} U_E(\sigma)$, do đó $\Gamma$ là tách. Với mỗi $x \in N$ tập hợp các liên hợp $\sigma(x)$ của $x$, khi $\sigma$ chạy qua $\Gamma$, là *hữu hạn* vì $x$ là đại số trên $K$ (V, p. Hệ quả 1); do đó tất cả các phép chiếu của $\Gamma$ lên các không gian nhân tử của $N^N$ đều là các tập hữu hạn, và điều này chỉ ra rằng $\Gamma$ là tương đối compact trong $N^N$ (Gen. Top., I, p. 88). Còn lại là chỉ ra rằng $\Gamma$ là đóng trong $N^N$. Bây giờ nếu $u$ thuộc bao đóng của $\Gamma$ trong $N^N$, thì với mỗi cặp điểm $(x, y)$ của $N$ tồn tại $a \in \Gamma$ sao cho $u(x) = \sigma(x), \ u(y) = \sigma(y), \ u(x+y) = \sigma(x+y), \ u(xy) = \sigma(xy)$, do đó $u(x+y) = u(x) + u(y)$ và $u(xy) = u(x)u(y)$. Theo cùng một lập luận ta có $u(x) = x$ với mọi $x \in K$, do đó $u$ là một $K$-đồng cấu của $N$ vào $N$; vì $N$ là đại số trên $K$, $u$ là một $K$-tự đẳng cấu của $N$ (V, p. 52, Mệnh đề 1), do đó $u \in T$.

Cho $N$ là một mở rộng Galois của $K$ và $(N_i)_{i \in I}$ là một họ có hướng tăng của các mở rộng con của $N$. Giả sử rằng $N_i$ là Galois trên $K$ với mọi $i \in I$ và $N = \bigcup_{i \in I} N_i$. Với mỗi $i \in I$, ký hiệu $\Gamma_i$ là nhóm Galois của $N_i$ trên $K$; với $i \leq j$ trong $I$, ta có $N_i \subset N_j$ và đồng cấu hạn chế $\varphi_{ij}$ của $\Gamma_j$ vào $\Gamma_i$ được xác định. Nó liên tục và do đó họ $(\Gamma_i, \varphi_{ij})$ là một hệ ngược của các nhóm tôpô. Hơn nữa, với mỗi $i \in I$, ký hiệu $\lambda_i$ là đồng cấu hạn chế của $\mathrm{Gal}(N/K)$ vào $\mathrm{Gal}(N_i/K) = \Gamma_i$; nó liên tục và ta có $\lambda_i = \varphi_{ij} \circ \lambda_j$ với $i \leq j$, do đó họ $(\lambda_i)_{i \in I}$ xác định một đồng cấu liên tục $\Lambda$ của $\mathrm{Gal}(N/K)$ vào $\varprojlim \Gamma_i$.

#### Mệnh đề 5 {#alg-v-s10-prop-5 .statement}

— *Đồng cấu* $\lambda$ *của* $\mathrm{Gal}(N/K)$ *vào* $\varprojlim \mathrm{Gal}(N_i/K)$ *là một đẳng cấu của các nhóm tôpô*.

Vì $\mathrm{Gal}(N/K)$ là compact, $\lambda$ liên tục và nhóm $\varprojlim \mathrm{Gal}(N_i/K)$ là tách được, chỉ cần chứng minh rằng $h$ là song ánh (*Gen. Top.*, *I*, p. 87, Hệ quả 2). Cho $u = (u_i)_{i \in I}$ là một phần tử của $\varprojlim \mathrm{Gal}(N_i/K)$; với mỗi $i \in I$, $u_i$ là một K-tự đẳng cấu của $N_i$ và $u_i$ là hạn chế của $u_j$ xuống $N_i$ với $i \leq j$. Vì $N = \bigcup_{i \in I} N_i$, tồn tại một phần tử duy nhất $\sigma$ của $\mathrm{Gal}(N/K)$ trùng với $u_i$ trên $N_i$ với mọi $i \in I$. Do đó $\sigma$ là phần tử duy nhất của $\mathrm{Gal}(N/K)$ sao cho $\lambda(u) = u$, suy ra $\lambda$ là song ánh.

Điều này áp dụng đặc biệt khi ta lấy họ $(N_i)$ là họ của tất cả các mở rộng con Galois hữu hạn của $N$; khi đó mỗi nhóm $\mathrm{Gal}(N_i/K)$ là rời rạc và hữu hạn. Nhóm tôpô $\mathrm{Gal}(N/K)$ do đó đẳng cấu với một giới hạn ngược có hướng của các nhóm hữu hạn, được trang bị tôpô rời rạc; đôi khi nhóm này được gọi là một nhóm tôpô *profinite*.

### 4. Hạ Galois

*Trong mục này* ta ký hiệu $N$ *là một trường*, $\Gamma$ *là một nhóm các tự đẳng cấu của* $N$, $e$ *là phần tử đơn vị của* $\Gamma$ *và* $K$ *là trường các bất biến của* $\Gamma$.

Cho $V$ là một không gian vectơ trên $N$. Ta nhắc lại (II, p. 317) rằng một *cấu trúc K* trên $V$ là một không gian con K-vectơ $V_0$ của $V$ sao cho ánh xạ K-tuyến tính $\varphi : N \otimes_K V_0 \to V$ biến $h \otimes x$ thành $\lambda x$ là song ánh. Cho $V_0$ là một cấu trúc K như vậy; với mỗi $\sigma \in \Gamma$ ta đặt $u_\sigma = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) \circ \varphi^{-1}$; khi đó ta có $u_\sigma \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{i \in I} \sigma(\lambda_i) e_i$ với mọi họ các phần tử $\lambda_i$ của $N$ và $e_i$ của $V_0$, do đó ta thu được các hệ thức
$$
\begin{align*}
u_\sigma(x + y) &= u_\sigma(x) + u_\sigma(y) \\
u_\sigma(\lambda x) &= \sigma(\lambda) u_\sigma(x) \\
u_\sigma \circ u_\tau &= u_{\sigma \tau} \\
u_e &= \mathrm{Id}_V
\end{align*}
$$
với $\sigma, \tau$ thuộc $\Gamma$, $x, y$ thuộc $V$ và $\lambda$ thuộc $N$.

#### Mệnh đề 6 {#alg-v-s10-prop-6 .statement}

— *a)* *Cho* $V$ *là một không gian vectơ trên* $N$ *có một* $K$-*cấu trúc*. *Đối với một vectơ* $x \in V$ *để hữu tỉ trên* $K$ *là điều kiện cần và đủ rằng* $u_\sigma(x) = x$ *với mọi* $\sigma \in \Gamma$. *Đối với một không gian con N-vectơ* $W$ *của* $V$ *để hữu tỉ trên* $K$ *là điều kiện cần và đủ rằng* $u_\sigma(W) \subset W$ *với mọi* $\sigma \in \Gamma$.

*b)* *Cho* $V_1$ *và* $V_2$ *là hai không gian vectơ trên* $N$, *mỗi không gian có một* $K$-*cấu trúc*. *Đối với một ánh xạ tuyến tính* $f$ *của* $V_1$ *vào* $V_2$ *để hữu tỉ trên* $K$ *là điều kiện cần và đủ rằng* $f(u_\sigma(x)) = u_\sigma(f(x))$ *với mọi* $\sigma \in \Gamma$ *và mọi* $x \in V_1$.

*Rõ ràng* $K$ *là tập hợp các* $x \in N$ *sao cho* $\sigma(xy) = x \sigma(y)$ *với mọi* $\sigma \in \Gamma$ *và mọi* $y \in N$. *Do đó mệnh đề suy ra từ Định lý 1* (II, p. 324).

#### Hệ quả {#alg-v-s10-n4-cor-1 .statement}

— Cho $V_0$ là một không gian vectơ trên $K$ và cho $W$ là một không gian con-N vectơ của $N \otimes_K V_0$. Giả sử rằng $W$ ổn định dưới các ánh xạ $\sigma \otimes \mathrm{Id}_{V_0}$ với mọi $\sigma \in \Gamma$. Gọi $W_0$ là tập hợp các $x \in V_0$ sao cho $1 \otimes x \in W$; khi đó $W_0$ là không gian con-K vectơ duy nhất của $V_0$ sao cho $W = N \otimes_K W_0$.

Chỉ cần nhận xét rằng tập hợp các phần tử có dạng $1 \otimes x \ (x \in V_0)$ là một cấu trúc-K trên $N \otimes_K V_0$ mà trên đó ta có $u_\sigma = \sigma \otimes \mathrm{Id}_{V_0}$ với $\sigma \in \Gamma$.

#### Mệnh đề 7 {#alg-v-s10-prop-7 .statement}

— Cho $V$ là một không gian vectơ trên $N$, $(u_\sigma)_\sigma$, r là một họ các ánh xạ của $V$ vào chính nó thỏa mãn (1) đến (4) và $V_0$ là tập hợp các $x \in V$ sao cho $u_\sigma(x) = x$ với mọi $\sigma \in \Gamma$.

a) $V_0$ là một không gian con-K vectơ của $V$ và ánh xạ K-tuyến tính $\varphi$ từ $N \otimes_K V_0$ vào $V$, biến $\lambda \otimes x$ thành $\lambda x$, là đơn ánh.

b) Nếu $\Gamma$ hữu hạn, thì $\varphi$ là song ánh và $V_0$ là một cấu trúc-K trên $V$.

Rõ ràng $V_0$ là một không gian con-K vectơ của $V$.

Công thức $u_\sigma \circ \varphi = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0})$ cho thấy hạt nhân $W$ của $\varphi$ ổn định dưới các ánh xạ $\sigma \otimes \mathrm{Id}_{V_0}$; do Hệ quả của Mệnh đề 6, do đó tồn tại một không gian con $W_0$ của $V_0$ sao cho $W = N \otimes_K W_0$. Nếu $x$ thuộc $W_0$ thì ta có $x = \varphi(1 \otimes x) = 0$, suy ra $W_0 = 0$ và do đó $W = 0$. Điều này chứng minh a).

Giả sử $\Gamma$ là hữu hạn; ta phải chứng minh rằng $\varphi$ là toàn ánh, hay tương đương rằng $V_0$ sinh ra không gian vectơ N $V$. Do đó, cho $f$ là một dạng N-tuyến tính trên $V$ mà hạn chế của nó lên $V_0$ bằng không. Cho $x \in V$; với mọi $A \in N$ phần tử $y, = \sum_{\sigma \in \Gamma} u_\sigma(\lambda x)$ của $V$ rõ ràng thuộc $V_0$, do đó $f(y,) = 0$, nghĩa là,
$$
\sum_{\sigma \in \Gamma} f(u_\sigma(x)) \sigma(A) = 0.
$$
Theo định lý Dedekind (V, p. 27, Hệ quả 2), do đó ta có $f(u_\sigma(x)) = 0$ với mỗi $\sigma \in \Gamma$; đặc biệt, lấy $\sigma = \varepsilon$ ta được $f(x) = 0$, điều này có nghĩa là $f = 0$. Điều này chứng minh b).

Cho $M$ là một không gian vectơ trên $N$; với mỗi $\sigma \in \Gamma$, cho $M^\sigma$ là không gian vectơ trên $N$ có cùng nhóm cộng cơ sở như $M$, với phép toán ngoài $(A, x) \mapsto \sigma(\lambda) x$. Viết $V = \prod_{\sigma \in \Gamma} M^\sigma$; nhóm cộng cơ sở của $V$ là nhóm của tất cả các ánh xạ từ $\Gamma$ vào $M$, với phép toán ngoài được định nghĩa bởi
$$
(\lambda . h)(\sigma) = \sigma(\lambda) h(\sigma) \quad (\lambda \in N, h \in V, \sigma \in \Gamma).
$$
(Tích $\sigma(\lambda) h(\sigma)$ được tính trong không gian vectơ $M$.) Hơn nữa, ta định nghĩa trên $N \otimes_K M$ một cấu trúc không gian vectơ trên $N$ bởi công thức
$$
\lambda \left( \sum_i \mu_i \otimes x_i \right) = \sum_i \lambda \mu_i \otimes x_i
$$
Cuối cùng, ta ký hiệu $\psi$ là ánh xạ K-tuyến tính từ $N \otimes_K M$ vào $V$ được đặc trưng bởi quan hệ
$$
\psi(\lambda \otimes x)(\sigma) = \sigma(\lambda) . x
$$
với $A \in N, x \in M$ và $\sigma \in \Gamma$. Rõ ràng $\psi$ là N-tuyến tính

#### Mệnh đề 8 {#alg-v-s10-prop-8 .statement}

— *Ánh xạ N-tuyến tính* $\psi$ *từ* $N \otimes_K M$ *vào* $V = \prod_{\sigma \in \Gamma} M^\sigma$ *là đơn ánh, và là song ánh nếu* $\Gamma$ *hữu hạn.*

Với mọi $a \in \Gamma$, ta định nghĩa một ánh xạ $u_\sigma$ từ $V$ vào $V$ bởi

$$
(u_\sigma h)(\tau) = h(\tau \sigma)
$$

cho $h \in V$ và $\tau \in \Gamma$. Việc kiểm tra *(1)-(4)* là ngay lập tức. Ký hiệu $V$, tập hợp các $h \in V$ sao cho $u_\sigma(h) = h$ với mọi $\sigma \in \Gamma$. Với mỗi $x \in M$, đặt $\theta(x)$ là ánh xạ hằng từ $\Gamma$ vào $M$ nhận giá trị $x$; khi đó $\theta$ là một K-đẳng cấu của $M$ lên $V$. Nếu ta định nghĩa đồng cấu $\varphi : N \otimes_K V, \to V$ như trên, ta có $\psi = \varphi \circ (\mathrm{Id}_N \otimes \theta)$ và khi đó Mệnh đề 8 suy ra từ Mệnh đề 7.

#### Hệ quả {#alg-v-s10-n4-cor-2 .statement}

— *Cho* $\psi$ *là ánh xạ K-tuyến tính từ* $N \otimes_K N$ *vào không gian vectơ tích* $N^\Gamma$ *sao cho* $\psi(x \otimes y)\,(a) = \sigma(x)\,y$ *với* $x,\,y$ *thuộc* $N$ *và* $\sigma \in \Gamma$. *Khi đó* $\psi$ *là đơn ánh và là song ánh khi* $\Gamma$ *hữu hạn.*

Đây là trường hợp riêng $M = N$ của Mệnh đề 8.

#### Nhận xét 1 {#alg-v-s10-n4-rem-1 .statement}

Cho F là một mở rộng của K và $N$ là một mở rộng con của F, và cho $\Gamma$ là một nhóm *hữu hạn* các tự đẳng cấu của $N$, mà K là trường bất biến. Mệnh đề 8 suy ra sự tồn tại của một đẳng cấu các K-đại số $0 : N \otimes_F F \to F^\Gamma$ được đặc trưng bởi $\theta(x \otimes y)\,(a) = \sigma(x)\,y$ với $x \in N,\,y \in F$ và $\sigma \in \Gamma$.

#### Nhận xét 2 {#alg-v-s10-n4-rem-2 .statement}

Ký hiệu K, N và $\Gamma$ có cùng ý nghĩa như trước. Với mỗi số nguyên $n \geqslant 1$, cho $A_n$ là tích tenxơ của n K-đại số đồng nhất với $N$; cho $B_n$ là tập hợp các ánh xạ từ $\Gamma^{n-1}$ vào $N$. Bằng quy nạp theo $n$, ta suy ra từ Hệ quả của Mệnh đề 8 sự tồn tại của một đẳng cấu $\varphi_n : A_n \to B_n$, ánh xạ $x_1 \otimes \ldots \otimes x_n$ thành hàm $(\sigma_1, \ldots, a, ) \quad \sigma_1(x_1) \cdot \sigma_n(x_{n-1})\,x_n$.

### 5. *Đối đồng điều Galois*

Cho $N$ là một trường, $\Gamma$ là một nhóm *hữu hạn* các tự đẳng cấu của $N$ và K là trường bất biến của $\Gamma$. Với mỗi số nguyên $n \geqslant 1$, ta ký hiệu $\mathbf{GL}(n, N)$ là nhóm các ma trận vuông cấp $n$ với các hệ số trong $N$ và định thức khác không (II; p. 349). Ta cho nhóm $\Gamma$ tác động lên nhóm $\mathbf{GL}(n, N)$ theo quy tắc $\sigma(A) = (\sigma(a_{ij}))$ với $A = (a_{ij})$.

#### Mệnh đề 9 {#alg-v-s10-prop-9 .statement}

— *Cho* $(U_\sigma)_{\sigma \in \Gamma}$ *là một họ các phần tử của* $\mathbf{GL}(n, N)$. *Để tồn tại* $A$ *trong* $GL(n, N)$ *sao cho* $U_\sigma = A^{-1}\,a(A)$ *với mọi* $\sigma \in \Gamma$ *là điều kiện cần và đủ để* $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ *với* $\sigma,\,\tau$ *trong* $\Gamma$.

Điều kiện là *cần*: nếu $U_\sigma = A^{-1}\,a(A)$, thì ta có

$$
U_\sigma \cdot \sigma(U_\tau) = A^{-1}\,\sigma(A)\,\sigma(A^{-1}\,\tau(A)) = A^{-1}\sigma\tau(A) = U_{\sigma \tau}.
$$

Điều kiện là *đủ*: ta đồng nhất các phần tử của $N^n$ với các ma trận có $n$ hàng và một cột với các hệ số trong $N$. Ta cho các nhóm $\Gamma$ tác động lên $N^n$ bởi
$$
\sigma(x) = (\sigma(x_i))_{1 \leq i \leq n} \quad \text{với} \quad x = (x_i)_{1 \leq i \leq n}.
$$
Với mỗi $a \in \Gamma$, ta ký hiệu $u_\sigma$ là ánh xạ $x \mapsto U_\sigma \cdot \sigma(x)$ của $N^n$ vào chính nó. Việc kiểm tra các Công thức (1) đến (3) của V, p. 62 là ngay lập tức. Hơn nữa ta có $u_\varepsilon \circ u_\varepsilon = u_\varepsilon$ và vì $u_\varepsilon$ là song ánh, ta có $u_\varepsilon = \mathrm{Id}_{N^n}$. Gọi $V_0$ là tập hợp các vectơ $x \in N^n$ sao cho $u_\sigma(x) = x$ với mọi $\sigma \in \Gamma$. Theo Mệnh đề 7 (V, p. 63), $V_0$ là một cấu trúc K trên $N^n$; đặc biệt tồn tại trong $V_0$ các vectơ $b_1, \ldots, b_n$ lập thành một cơ sở của $N^n$ trên $N$. Do đó ma trận $B$ có các cột $b_1, \ldots, b_n$ là khả nghịch và quan hệ $u_\sigma(b_i) = b_i$ với $1 \leq i \leq n$ tương đương với $U_\sigma \cdot \sigma(B) = B$. Đặt $A = B^{-1}$, ta thu được $U_\sigma = A^{-1} \sigma(A)$ với mọi $a \in \Gamma$.

#### Hệ quả 1 {#alg-v-s10-prop-9-cor-1 .statement}

*Cho $(c,)$, , , là một họ các phần tử khác không của $N$. Để tồn tại $a \neq 0$ trong $N$ sao cho $c, = \sigma(a) \cdot a'$ với mọi $a \in \Gamma$ là điều kiện cần và đủ để $c, = c, \cdot a(c,)$ với $\sigma, \tau$ trong $\Gamma$.*

#### Hệ quả 2 {#alg-v-s10-prop-9-cor-2 .statement}

*Cho $(c,)$, $\Gamma$ là một họ các phần tử của $N$. Để $b$ tồn tại trong $N$ sao cho $a, = \sigma(b) - b$ với mọi $a \in \Gamma$, điều kiện cần và đủ là $a, = a, + \sigma(a_\tau)$ với $a, \tau$ thuộc $\Gamma$.*

Ta có $\sigma \tau(b) - b = [\sigma(b) - b]^+ \sigma[\tau(b) - b]$ với mọi $b$ thuộc $N$ và $a, \tau$ thuộc $\Gamma$, do đó điều kiện là cần thiết.

Ngược lại, giả sử $a, = a, + \sigma(a_\tau)$ với mọi $a$ và $\tau$ thuộc $\Gamma$. Đặt $U_\sigma = \begin{pmatrix} 1 & a_\sigma \\ 0 & 1 \end{pmatrix}$ với $\sigma \in \Gamma$; khi đó ta có $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ với $\sigma, \tau$ thuộc $\Gamma$; theo Mệnh đề 9, do đó tồn tại một ma trận $A = \begin{pmatrix} x & y \\ z & t \end{pmatrix}$ có định thức khác không sao cho $\sigma(A) = A U_\sigma$ với mọi $a \in \Gamma$; viết quan hệ $\sigma(A) = A U_\sigma$ ta được
$$
\begin{pmatrix} \sigma(x) & \sigma(y) \\ \sigma(z) & \sigma(t) \end{pmatrix} = \begin{pmatrix} x & x a_\sigma + y \\ z & z a_\sigma + t \end{pmatrix} \quad (\sigma \in \Gamma).
$$
Đặc biệt, $x$ và $z$ thuộc $K$ và ta có
$$
\sigma(y) = x a_\sigma + y, \quad \sigma(t) = z a_\sigma + t \quad (\sigma \in \Gamma).
$$
Nếu $x \neq 0$ thì ta có $a, = \sigma(b) - b$ với $b = x^{-1} y$; nếu $z \neq 0$, ta có cùng quan hệ với $b = z^{-1} t$. Bây giờ $x$ và $z$ không thể đồng thời bằng không vì
$$
xt - yz = \det A \neq 0.
$$

### 6. Định lý của Artin

**Định lý 2 (Artin).** — *Cho $N$ là một trường, $\Gamma$ là một nhóm các tự đẳng cấu của $N$ và $K$ là trường các bất biến của $\Gamma$. Cho $V$ là một không gian vectơ con trên K của $N$ có số chiều hữu hạn* trên K. Khi đó mọi ánh xạ K-tuyến tính u của V vào N đều là một tổ hợp tuyến tính với các hệ số trong N của các hạn chế trên V của các phần tử của $\Gamma$.

Cho u là một ánh xạ K-tuyến tính từ V vào N và cho $V_{(N)} = N \otimes_K V$ là không gian vectơ N dẫn xuất từ V bằng mở rộng vô hướng; ký hiệu $\tilde{u}$ là dạng tuyến tính N trên $V_{(N)}$ sao cho $\tilde{u}(x \otimes y) = x \cdot u(y)$ với $x \in N$ và $y \in V$. Với mỗi $a \in \Gamma$ tồn tại một dạng tuyến tính N h trên $V_{(N)}$ sao cho $h_\sigma(x \otimes y) = x \sigma(y)$ với $x \in N$ và $y \in V$. Ánh xạ chính tắc của $V_{(N)} = N \otimes_K V$ vào $N \otimes_K N$ là đơn ánh. Khi đó Hệ quả của Mệnh đề 8 (V, p. 64) cho thấy rằng giao của các hạt nhân của các dạng tuyến tính h trên $V_{(N)}$ được rút gọn về 0. Do đó (II, p. 302, Hệ quả 1) tồn tại $a_1, \ldots, \sigma_n$ trong $\Gamma$ và $a_1, \ldots, a_n$ trong $N$ sao cho $\tilde{u} = \sum_{i=1}^n a_i h_{\sigma_i}$ do đó $u(x) = \sum_{i=1}^n a_i \sigma_i(x)$ với mọi $x \in V$.

Ta trang bị cho tập hợp $N^N$ gồm tất cả các ánh xạ từ N vào N tôpô tích của các tôpô rời rạc của các nhân. Định lý 2 có nghĩa là tập hợp các tổ hợp tuyến tính với các hệ số trong N của các phần tử của $\Gamma$ là trù mật trong tập hợp các ánh xạ K-tuyến tính từ N vào chính nó.

#### Định lý 3 {#alg-v-s10-thm-3 .statement}

— Cho N là một trường, $\Gamma$ là một nhóm hữu hạn các tự đẳng cấu của N và K là trường các bất biến của $\Gamma$. Gọi n là lực lượng của $\Gamma$.
a) Ta có $[N : K] = n$ và N là một mở rộng Galois của K với nhóm Galois $\Gamma$.
b) Cho $\sigma_1, \ldots, \sigma_n$ là các phần tử của $\Gamma$ và $(x_1, \ldots, x_n)$ là một cơ sở của N trên K, khi đó $\det (\sigma_i(x_j)) \neq 0$.
c) Cho u là một ánh xạ K-tuyến tính từ N vào N. Tồn tại duy nhất một họ $(a_\sigma)_\sigma$ các phần tử của N sao cho $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ với mọi $x \in N$.

Ta trang bị cho vành $N \otimes_K N$ cấu trúc đại số N mà phép toán ngoài được cho bởi $\lambda(x \otimes y) = x \otimes \lambda y$ với $\lambda, x, y$ trong N. Khi đó chiều của không gian vectơ N $NO, N$ là $[N : K]$. Chiều của không gian vectơ tích N $N^\Gamma$ bằng n. Ánh xạ $\psi$ được định nghĩa trong Hệ quả của Mệnh đề 8 (V, p. 64) là một đẳng cấu N của $NO, N$ lên $N^\Gamma$, do đó $[N : K] = n$. Gọi A là nhóm các tự đẳng cấu K của N. Ta có $\Gamma \subset A$, do đó K là trường các bất biến của A, và N là một mở rộng Galois của K. Hơn nữa, cấp của A nhiều nhất bằng $[N : K]$ theo định lý Dedekind (V, p. 27, Hệ quả 2) và vì cấp của $\Gamma$ bằng $[N : K]$, ta có $\Gamma = A$. Do đó $\Gamma$ là nhóm Galois của N trên K, và điều này chứng minh a).

Với ký hiệu của b), đặt $f_i = \psi(x_i \otimes 1)$; ta có $f_i(\sigma) = \sigma(x_i)$ với $1 \leq i \leq n$ và $\sigma \in \Gamma$. Vì $\psi$ là một đẳng cấu của các không gian vectơ N, dãy $(f_1, \ldots, f_n)$ là một cơ sở của N trên N, do đó $\det (f_j(\sigma_i)) \neq 0$, nghĩa là,

$$
\det (\sigma_i(x_j)) \neq 0
$$

Điều này chứng minh b).

Cuối cùng, c) suy ra từ Định lý 2 (V, p. 65), định lý chứng minh sự tồn tại của một họ (a,,), ,, sao cho $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ (với mọi $x \in N$), và từ định lý Dedekind (V, p. 27, Hệ quả 2), định lý chứng minh tính duy nhất của (a,,), ,$\Gamma$.

### 7. Định lý cơ bản của lý thuyết Galois

#### Định lý 4 {#alg-v-s10-thm-4 .statement}

— Cho N là một mở rộng Galois của K và $\Gamma$ là nhóm Galois của nó. Gọi $\mathcal{K}$ là tập hợp các mở rộng con của N và $\mathcal{G}$ là tập hợp các nhóm con đóng của $\Gamma$. Với mỗi nhóm con $A \in \mathcal{G}$, ta ký hiệu $k(\Delta)$ là trường các bất biến của A và với mỗi *trường con* $E \in \mathcal{K}$, ta ký hiệu $g(E)$ là nhóm các *tự đẳng cấu* E của N. *Khi đó* $A \mapsto k(\Delta)$ là một song ánh của $\mathcal{G}$ lên $\mathcal{K}$, và $E \mapsto g(E)$ là song ánh ngược.

A) Quan hệ $E = k(g(E))$ (với $E \in \mathcal{K}$) là một hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 1 {#alg-v-s10-lem-1 .statement}

Cho E là một mở rộng con của N. Khi đó N là một mở rộng Galois của E và $\mathrm{Gal}(N/E)$ là một nhóm con đóng của $\mathrm{Gal}(N/K)$ với tôpô cảm sinh.

Cho $x \in N$; đa thức tối tiểu f của x trên E chia trong $E[X]$ đa thức tối tiểu $g$ của x trên K (V, p. 17, Hệ quả 2). Vì N là Galois trên K, đa thức g là một tích trong $N[X]$ của các nhân tử phân biệt bậc 1; do đó f cũng như vậy và N là Galois trên E.

Gọi $\Gamma$ là nhóm Galois của N trên K và A là nhóm Galois của N trên E. Theo định nghĩa, A là nhóm con của $\Gamma$ gồm tất cả các $\sigma$ sao cho $\sigma(x) = x$ với mọi $x \in E$. Bây giờ, với mỗi $x \in E$, ánh xạ $\sigma \mapsto \sigma(x)$ từ $\Gamma$ vào không gian rời rạc N là liên tục, do đó D là đóng trong $\Gamma$. Cho $\sigma \in \Gamma$; với $x_1, \ldots, x_n$ thuộc N, gọi $U(x_1, \ldots, x_n)$ là tập hợp tất cả các $\tau \in \Gamma$ sao cho $\tau(x_i) = \sigma(x_i)$ với $1 \leq i \leq n$; đặt

$$
V(x_1, \ldots, x_n) = U(x_1, \ldots, x_n) \cap \Delta.
$$

Khi đó họ các tập hợp $U(x_1, \ldots, x_n)$ (tương ứng $V(x_1, \ldots, x_n)$) là một cơ sở các lân cận của $\sigma$ trong $\Gamma$ (tương ứng A). Do đó tôpô trên A là tôpô cảm sinh bởi $\Gamma$.

B) Quan hệ $A = g(k(\Delta))$ (với $A \in g$) là một hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 2 {#alg-v-s10-lem-2 .statement}

Cho A là một nhóm con của $\Gamma$. Gọi E là trường các bất biến của A; khi đó nhóm Galois của N trên E là bao đóng của A trong $\Gamma$.

Nhóm Galois của N trên E đóng trong $\Gamma$ (Bổ đề 1) và chứa A, do đó nó chứa bao đóng $\bar{\Delta}$ của A. Cho $\sigma$ là một E-tự đẳng cấu của N và cho $x_1, \ldots, x_n$ thuộc N. Vì N là Galois trên E (Bổ đề 1) nên tồn tại (V, p. 57, Mệnh đề 2) một phần mở rộng con $N_0$ của N, Galois, có bậc hữu hạn trên E và chứa $x_1, \ldots, x_n$. Cho $A_0$ là ảnh của nhóm con A của $\mathrm{Gal}(N/E)$ qua đồng cấu hạn chế của $\mathrm{Gal}(N/E)$ vào $\mathrm{Gal}(N_0/E)$. Vì $[N_0 : E]$ là hữu hạn, định lý của Dedekind (V, p. 27, Hệ quả 2) cho thấy $\mathrm{Gal}(N_0/E)$ là hữu hạn. Do đó $A_0$ là hữu hạn, và vì E là trường bất biến của $A_0$, ta có $\Delta_0 =$

Gal(N_0/E) (V, p. 66, Định lý 3). Đặc biệt, $\Delta_0$ chứa phần hạn chế của $\sigma$ trên $N_0$. Vậy tồn tại $\tau \in A$ sao cho $\sigma$ và $\tau$ có cùng phần hạn chế trên $N_0$, do đó $\sigma(x_1) = \tau(x_1), \ldots, \sigma(x_n) = \tau(x_n)$. Suy ra $\sigma$ là một điểm giới hạn của $A$ trong $\Gamma$, và do đó $\mathrm{Gal}(N/E) \subset \overline{\Delta}$.

#### Hệ quả 1 {#alg-v-s10-lem-2-cor-1 .statement}

*Cho E và E' là hai trường con của N chứa K; khi đó E $\subset$ E' nếu và chỉ nếu g(E) $\supset$ g(E'). Nếu A và A' là hai nhóm con đóng của $\Gamma$, thì A $\subset$ A' nếu và chỉ nếu k($\Delta$) $\supset$ k($\Delta'$).*

Vì hai song ánh nghịch đảo $E \rightleftharpoons g(E)$ và $A \rightleftharpoons k(\Delta)$ đều phản đảo ngược theo bao hàm.

#### Hệ quả 2 {#alg-v-s10-lem-2-cor-2 .statement}

*Cho $(E_i)_{i \in I}$ là một họ các trường con của N chứa K; đặt $L = \bigcap_{i \in I} E_i$ và $M = K\left( \bigcup_{i \in I} E_i \right)$. Khi đó g(L) là nhóm con đóng nhỏ nhất chứa $U_{i \in I} g(E_i)$ và ta có $g(M) = \bigcap_{i \in I} g(E_i)$.*

Mệnh đề thứ nhất suy ra từ Hệ quả 1 và mệnh đề thứ hai là ngay lập tức.

#### Hệ quả 3 {#alg-v-s10-lem-2-cor-3 .statement}

*Cho i = 1, 2, đặt $E_i$ là một trường con của N chứa K và cho $\Delta_i = g(E_i)$. Với mọi $\sigma \in \Gamma$ các quan hệ $\sigma(E_1) = E_2$ và $\sigma \Delta_1 \sigma^{-1} = \Delta_2$ là tương đương.*

Vì ta có $\tau \in g(\sigma(E_1))$ nếu và chỉ nếu $\tau \sigma(x) = \sigma(x)$, tức là $\sigma^{-1} \tau \sigma(x) = x$, với mọi $x \in E_1$; điều đó có nghĩa là $\sigma^{-1} \tau \sigma \in \Delta_1$, do đó $g(\sigma(E_1)) = \sigma \Delta_1 \sigma^{-1}$.

#### Hệ quả 4 {#alg-v-s10-lem-2-cor-4 .statement}

*Cho E là một trường con của N chứa K và cho $A = g(E)$. Để E là Galois trên K thì điều kiện cần và đủ là A phải là một nhóm con chuẩn tắc của $\Gamma$. Khi điều này xảy ra, đồng cấu hạn chế của $\Gamma$ vào $\mathrm{Gal}(E/K)$ xác định, qua phép qua thương, một đẳng cấu nhóm tôpô của $\Gamma / \Delta$ lên $\mathrm{Gal}(E/K)$.*

Vì N tách được trên K, điều tương tự cũng đúng với E (V, p. 36, Mệnh đề 1). Do đó E là Galois trên K khi và chỉ khi E là quasi-Galois trên K; điều này cũng có nghĩa là $\sigma(E) = E$ với mọi K-tự đẳng cấu $\sigma$ của N (V, p. 52, Mệnh đề 1 và p. 54, Mệnh đề 3). Theo Hệ quả 3 điều này tương đương với $\sigma \Delta \sigma^{-1} = A$ với mọi $\sigma \in \Gamma$.

Đồng cấu hạn chế $\varphi : \mathrm{Gal}(N/K) \to \mathrm{Gal}(E/K)$ là liên tục và toàn ánh (V, p. 60, Mệnh đề 3) và hạt nhân của nó rõ ràng bằng $A = \mathrm{Gal}(N/E)$. Vì $\Gamma$ là compact, đồng cấu của $\Gamma / \Delta$ lên $\mathrm{Gal}(E/K)$ cảm sinh từ $\varphi$ qua phép chuyển sang thương là một đẳng cấu của các nhóm tôpô (Gen. Top., I, p. 87, Hệ quả 2).

#### Hệ quả 5 {#alg-v-s10-lem-2-cor-5 .statement}

*Cho E là một trường con của N chứa K. Để E có bậc hữu hạn trên K thì cần và đủ là g(E) mở trong $\Gamma$. Khi đó, chỉ số $(\Gamma : g(E))$ là hữu hạn và bằng [E : K].*

Để $g(E)$ mở thì cần và đủ là tồn tại một phần mở rộng con F của N, có bậc hữu hạn trên K, sao cho theo ký hiệu của V, p. 60.

g(E) chứa $U_F(\mathrm{Id}_N) = g(F)$. Quan hệ $g(E) \supset g(F)$ tương đương với $E \subset F$ theo Hệ quả 1 (V, p. 68), do đó có khẳng định thứ nhất của Hệ quả 5.

Giả sử rằng $[E : K]$ là hữu hạn. Cho $\Omega$ là một bao đóng đại số của $K$ chứa $N$ như một phần mở rộng con (V, p. 23, Định lý 2) và cho $\mathcal{H}$ là tập các $K$-đồng cấu của $E$ vào $\Omega$. Mỗi phần tử của $\mathcal{H}$ đều được cảm sinh bởi một $K$-tự đẳng cấu của $\Omega$ (V, p. 52, Mệnh đề 1), và vì $N$ là quasi-Galois trên $K$, ánh xạ $\sigma \mapsto \sigma|_E$ từ $\Gamma$ vào $\mathcal{H}$ là toàn ánh. Để $\sigma$ và $\sigma'$ trong $\Gamma$ có cùng hạn chế trên $E$ thì cần và đủ là $\sigma^{-1}\sigma' \in g(E)$, do đó Card $A? = (\Gamma : g(E))$. Cuối cùng vì E là một đại số étale trên K, ta có Card $\mathcal{H} = [E : K]$ (V, p. 32, Mệnh đề 4), nên kết luận là $(\Gamma : g(E)) = [E : K]$.

#### Hệ quả 6 {#alg-v-s10-lem-2-cor-6 .statement}

— Với $i = 1, 2$ cho $E_i$ là một phần mở rộng con của $N$ và $\Gamma_i$ là nhóm Galois của $N$ trên $E_i$. Các điều kiện sau là tương đương:
a) Nhóm $\Gamma$ là tích trực tiếp của các nhóm con $\Gamma_1$ và $\Gamma_2$.
b) Các phần mở rộng $E_1$ và $E_2$ là Galois trên $K$, ta có $E_1 \cap E_2 = K$ và
$$
K(E_1 \cup E_2) = N .
$$

Để $\Gamma$ là tích trực tiếp của các nhóm con $\Gamma_1$ và $\Gamma_2$, điều kiện cần và đủ là các điều kiện sau được thỏa mãn (I, p. 48, Prop. 15):
(i) các nhóm con $\Gamma_1$ và $\Gamma_2$ là chuẩn tắc trong $\Gamma$;
(ii) $\Gamma_1 \cap \Gamma_2 = \{ \varepsilon \}$, trong đó $\varepsilon$ là phần tử đơn vị của $\Gamma$;
(iii) $\Gamma = \Gamma_1 . \Gamma_2$.

Bây giờ (i) có nghĩa là $E_1$ và $E_2$ là Galois trên $K$ (Hệ quả 4). Theo Hệ quả 2, điều kiện (ii) tương đương với $N = K(E_1 \cup E_2)$, và cuối cùng nếu (i) và (ii) được thỏa mãn, $\Gamma_1 \Gamma_2$ là nhóm con nhỏ nhất của $\Gamma$ chứa $\Gamma_1 \cup \Gamma_2$; nó đóng vì $\Gamma_1$ và $\Gamma_2$ compact và ánh xạ $(a, \tau) \mapsto \sigma \tau$ từ $\Gamma_1 \times \Gamma_2$ vào $\Gamma$ là liên tục (Gen. Top., I, p. 63, Cor. 1). Hệ quả 2 giờ đây cho thấy (iii) tương đương với $E_1 \cap E_2 = K$, và điều này chứng minh sự tương đương của a) và b).

#### Nhận xét {#alg-v-s10-n7-rem-1 .statement}

Với ký hiệu của Hệ quả 6, giả sử các điều kiện a) và b) được thỏa mãn. Các đồng cấu hạn chế $\varphi_i : \Gamma \to \mathrm{Gal}(E_i/K)$ với $i = 1, 2$ cảm sinh các đẳng cấu nhóm tôpô
$$
\Psi_1 : \Gamma_2 \to \mathrm{Gal}(E_1/K) , \quad \Psi_2 : \Gamma_1 \to \mathrm{Gal}(E_2/K)
$$
Theo a), ta thấy rằng ánh xạ $\sigma \mapsto (\varphi_1(\sigma), \varphi_2(\sigma))$ là một đẳng cấu nhóm tôpô từ $\mathrm{Gal}(N/K)$ lên $\mathrm{Gal}(E_1/K) \times \mathrm{Gal}(E_2/K)$.

### 8. Đổi trường cơ sở

Cho $N$ là một mở rộng Galois của $K$ và $\Gamma$ là nhóm Galois của $N$ trên $K$; hơn nữa, cho $N'$ là một mở rộng Galois của $K'$ với nhóm Galois $\Gamma'$. Ta sẽ đồng nhất $K$ (tương ứng $K'$) với ảnh của nó trong $N$ (tương ứng $N'$). Cho $u$ là một đồng cấu của $K$ vào $K'$ và $v$ là một đồng cấu của $N$ vào $N'$ mà hạn chế của nó lên $K$ bằng $u$ (cf.

Hình 1). Cho $\sigma \in \Gamma'$; vì $u(K) \subset K'$, $a$ là một $u(K)$-tự đẳng cấu của $N'$; hơn nữa $v(N)$ là một mở rộng Galois của $u(K)$, do đó $a$ cảm sinh một $u(K)$-tự đẳng cấu của $v(N)$ (V, p. 55, Nhận xét 1). Nói cách khác, với mọi $\sigma \in \Gamma'$ tồn tại một phần tử duy nhất $v^*(\sigma)$ của $\Gamma$ sao cho

(8)

$$
v \circ v^*(\sigma) = \sigma \circ v .
$$

![Biểu đồ cho thấy các ánh xạ v và u giữa N, N', K, K'](fig. 1)

Ánh xạ $v^*$ là một đồng cấu từ $\mathrm{Gal}(N'/K')$ vào $\mathrm{Gal}(N/K)$. Với mọi $x \in N$, ánh xạ $a \mapsto v^*(o)(x) = v^{-1}(\sigma(v(x)))$ từ $\Gamma'$ vào không gian rời rạc $N$ là liên tục, nên $v^*$ là liên tục.

Ba trường hợp riêng sau đây là quan trọng:

a) Nếu $F$ là một mở rộng Galois của $K$ và $E$ là một mở rộng con của $F$, ta biết (V, p. 67, Bổ đề 1) rằng $F$ là một mở rộng Galois của $E$. Hãy áp dụng điều vừa nói vào trường hợp $N = F$, $K' = E$, $N' = F$ và $v = \mathrm{Id}_F$. Khi đó $v^*$ chỉ là đơn ánh chính tắc

$$
j : \mathrm{Gal}(F/E) \to \mathrm{Gal}(F/K) .
$$

Điều này đôi khi được gọi là đồng cấu lạm phát.

b) Giả sử thêm rằng $E$ là Galois trên $K$. Hãy áp dụng điều vừa nói vào trường hợp $N = E$, $K' = K$, $N' = F$ và $v$ là đơn ánh chính tắc của $E$ vào $F$. Khi đó $v^*$ chỉ là đồng cấu hạn chế

$$
\pi : \mathrm{Gal}(F/K) \to \mathrm{Gal}(E/K)
$$

Ta biết (V, p. 60, Mệnh đề 3) rằng $\pi$ là toàn ánh, với hạt nhân $\mathrm{Gal}(F/E)$ và rằng bằng cách lấy thương, nó xác định một đẳng cấu nhóm tôpô từ $\mathrm{Gal}(F/K)/\mathrm{Gal}(F/E)$ lên $\mathrm{Gal}(E/K)$ (V, p. 68, Hệ quả 4).

c) Giả sử rằng $v^{-1}(K') = K$ và $N' = K'(v(N))$; ta hãy chứng minh rằng đồng cấu

$$
v^* : \mathrm{Gal}(N'/K') \to \mathrm{Gal}(N/K) ,
$$

is một đẳng cấu nhóm tôpô, đôi khi gọi là phép tịnh tiến. Vì nhóm $\mathrm{Gal}(N'/K')$ là compact, nhóm $\mathrm{Gal}(N/K)$ là tách biệt và $v^*$ là liên tục; do đó chỉ cần (Gen. Top., I, p. 87, Hệ quả 2) chứng minh rằng $v^*$ là song ánh. Bây giờ mọi phần tử $\sigma$ của hạt nhân của $v^*$ là một tự đẳng cấu của $N'$ cảm sinh đồng nhất trên $K'$ và trên $v(N)$, suy ra $a = \epsilon$ vì $N' = K'(v(N))$; do đó $v^*$ là đơn ánh. Hơn nữa, ảnh của $v^*$ là một nhóm con đóng $A$ của $\mathrm{Gal}(N/K)$

(Gen. Top., I, p. 81, *ibid.*) và trường bất biến của $A$ bằng $v^{-1}(K') = K$; vì vậy ta có $A = \mathrm{Gal}(N/K)$ (V, p. 67, Định lý 4) và do đó $v^*$ là toàn ánh.

Trường hợp tổng quát có thể được quy về các trường hợp trước bằng hợp thành. Trước hết ta nhận thấy rằng $K'(v(N))$ là trường bất biến trong $N'$ của hạt nhân $A$ của $v^*$; vì $A$ là một nhóm con chuẩn tắc của $\mathrm{Gal}(N'/K')$, nên phần mở rộng $K'(v(N))$ của $K'$ là Galois (V, p. 68, Hệ quả 4). Do đó $v^*$ là hợp thành của các đồng cấu

$$
\mathrm{Gal}(N'/K') \to \mathrm{Gal}(K'(u(N))/K') \xrightarrow{\psi} \mathrm{Gal}(N/v^{-1}(K')) \xrightarrow{j} \mathrm{Gal}(N/K);
$$

trong dãy này $\pi$ là đồng cấu hạn chế liên kết với bộ ba $K' \subset K'(u(N)) \subset N'$, $\psi$ là đẳng cấu dịch chuyển liên kết với bình phương trung tâm của biểu đồ (Hình 2) và $j$ là đồng cấu lạm phát liên kết với bộ ba $K \subset v^{-1}(K') \subset N$.

Định lý sau cho thông tin chi tiết hơn về cấu trúc của các đẳng cấu dịch chuyển.

![Biểu đồ cho thấy các mở rộng và các phép dịch chuyển](fig2.png)

Hình 2

#### Định lý 5 {#alg-v-s10-thm-5 .statement}

*Cho $N'$ là một mở rộng của $K$ được sinh bởi hai mở rộng con $K'$ và $N$. Giả sử rằng $N$ là Galois trên $K$, với nhóm Galois $\Gamma$ và rằng $K' \cap N = K$. Khi đó mở rộng $N'$ của $K'$ là Galois và đồng cấu chính tắc $\varphi$ của $K' \otimes_K N$ vào $N'$ là một đẳng cấu. Cho $\sigma \in \mathrm{Gal}(N/K)$ và cho $\sigma'$ là phần tử của $\mathrm{Gal}(N'/K')$ tương ứng với nó dưới đẳng cấu dịch chuyển; khi đó ta có $\sigma' \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes u)$.*

Chúng ta có $N' = K'(N)$ và $N$ là đại số và tách được trên $K$; do đó (V, p. 42, Mệnh đề 10), mở rộng $N'$ của $K'$ là đại số và tách được. Theo Hệ quả 4 của V, p. 54, mở rộng $N'$ của $K'$ là quasi-Galois. Vì vậy mở rộng $N'$ của $K'$ là Galois. Theo c) ở trên, ánh xạ $\sigma \mapsto \sigma|_N$ là một đồng cấu $\lambda$ từ $\mathrm{Gal}(N'/K')$ lên $\mathrm{Gal}(N/K)$.

Ta có $N = K'[N]$ vì $N$ là đại số trên $K$ (V, p. 18, Hệ quả 1), do đó $\varphi$ là toàn ánh. Nếu $a$ thuộc $\mathrm{Gal}(N/K)$, ta có

$$
\lambda^{-1}(\sigma) \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes \sigma).
$$

Do đó hạt nhân của $\varphi$ ổn định dưới các ánh xạ $\mathrm{Id}_{K'} \otimes \sigma$, nên có dạng $K' \otimes_K N_0$ với $N_0 \subset N$ (V, p. 63, Hệ quả). Với $x$ trong $N_0$ ta có $x = \varphi(1 \otimes x) = 0$, do đó $N_0 = 0$ và vì thế $\varphi$ là đơn ánh.

#### Hệ quả 1 {#alg-v-s10-thm-5-cor-1 .statement}

*Cho $E'$ là một trường con của $N'$ chứa $K'$. Tồn tại duy nhất một trường con $E$ của $N$ chứa $K$ và sao cho $E' = K'(E)$. Ta có $E = E' \cap N$.*

Đặt $E = E' \cap N$, khi đó $E' \supset K'(E)$. Bây giờ đặt $\Gamma = \mathrm{Gal}(N/K)$ và $A = \mathrm{Gal}(N/E)$, và định nghĩa $\Gamma'$ và $A'$ tương tự. Ánh xạ $A : a \mapsto a|_N$ là một đẳng cấu của $\Gamma'$ lên $\Gamma$ và đồng thời của $A'$ lên $A$; nói cách khác, $A'$ gồm những $\sigma \in \Gamma'$ sao cho $\lambda(\sigma)$ thuộc $A$. Nếu $\sigma \in \Gamma'$ để nguyên các phần tử của $K'(E)$, ta có $\lambda(\sigma) \in A$, do đó $a \in A'$ và $a$ để nguyên các phần tử của $E'$; theo Hệ quả 1 của V, p. 68 ta suy ra $K'(E) \supset E'$.

We have proved the equality $E' = K'(E)$, do đó $\varphi^{-1}(E') = K' \otimes_K E$. If $F$ is a subfield of $N$ containing $K$ and such that $E' = K'(F)$, we have likewise $\varphi^{-1}(E') = K' \otimes_K F$, do đó $F = E$.

#### Hệ quả 2 {#alg-v-s10-thm-5-cor-2 .statement}

*Cho $N$ là một mở rộng Galois của $K$. Giả sử nhóm Galois $\Gamma$ của $N$ trên $K$ là tích trực tiếp của hai nhóm con đóng $\Gamma_1$ và $\Gamma_2$ và ký hiệu $E_i$ là trường các bất biến của $\Gamma_i$ với $i = 1, 2$. Khi đó đồng cấu chính tắc của $E_1 \otimes_K E_2$ vào $N$ là một đẳng cấu.*

Ta có $E_1 \cap E_2 = K$ và $N = K(E_1 \cup E_2)$ theo Hệ quả 6 (V, p. 69), và do đó chỉ cần áp dụng Định lý 5.

#### Nhận xét {#alg-v-s10-n8-rem-1 .statement}

Cho $K$ và $K'$ là hai trường và $u$ là một đồng cấu của $K$ vào $K'$. Cho $K_s$ (resp. $K'_s$) là một bao đóng tách được (V, p. 45, Prop. 14) của $K$ (resp. $K'$) và $\Pi$ (resp. $\Pi'$) là nhóm Galois của $K_s$ trên $K$ (resp. $K'_s$ trên $K'$). Vì $K_s$ là một mở rộng đại số tách được của $K$ và mở rộng $(K'_s, u)$ của $K$ là đóng tách được, tồn tại (V, p. 45, Cor.) một đồng cấu $v$ của $K_s$ vào $K'_s$ kéo dài $u$. Từ $v$ ta thu được một đồng cấu liên tục $v^*$ của $\Pi'$ vào $\Pi$. Cho $v_1$ là một mở rộng khác của $u$; vì $K_s$ là một mở rộng quasi-Galois của $K$, tồn tại một phần tử $a_s$ của $\Pi$ sao cho $v_1 = v \circ a_s$. Ta kết luận rằng $v_1^*(\tau) = \sigma_0^{-1} v^*(\tau) \sigma_0$ với mọi $\tau \in \Pi$.

### 9. Định lý cơ sở chuẩn

Cho $N$ là một mở rộng Galois của $K$, với nhóm Galois $\Gamma$. Ta đồng nhất $\Gamma$ với cơ sở chính tắc của đại số nhóm $K^{(\Gamma)}$ (III, p. 446); khi đó $N$ có thể được xem như một $K^{(\Gamma)}$-môđun trái (III, p. 447, Ví dụ), do đó

$$
u \cdot x = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x) \quad \text{for} \quad x \in N \quad \text{and} \quad u = \sum_{\sigma \in \Gamma} a_\sigma \sigma \quad \text{in} \quad K^{(\Gamma)}.
$$

Nếu $N$ có bậc hữu hạn trên $K$, thì nhóm $\Gamma$ là hữu hạn theo định lý của Dedekind (V, p. 27, Hệ quả 2) và ta có thể định nghĩa phần tử $t = \sum_{\sigma \in \Gamma} a$ trong $K^{(\Gamma)}$; khi đó ta có

$$
\mathrm{Tr}_{N/K}(x) = \sum_{\sigma \in \Gamma} \sigma(x),
$$

nghĩa là, $\mathrm{Tr}_{N/K}(x) = t \cdot x$ với mọi $x \in N$.

Từ nay, hãy giả sử rằng $N$ có bậc hữu hạn trên $K$. Cho $x \in N$, để $\{x\}$ là một cơ sở của $\mathbf{K}^{(\Gamma)}$-môđun $N$ thì cần và đủ rằng họ $(\sigma(x))_{\sigma \in \Gamma}$ là một cơ sở của $N$ trên $K$. Một cơ sở như thế được gọi là *một cơ sở chuẩn của $N$ trên $K$*.

#### Định lý 6 {#alg-v-s10-thm-6 .statement}

*Cho $N$ là một mở rộng Galois có bậc hữu hạn trên $K$ và cho $\Gamma$ là nhóm Galois của $N$ trên $K$. Khi đó tồn tại một cơ sở chuẩn của $N$ trên $K$; nói cách khác, môđun $\mathbf{K}^{(\Gamma)}$ của $N$ là tự do hạng 1.*

Ta sẽ đưa ra hai chứng minh cho mệnh đề này. Chứng minh thứ nhất dùng bổ đề sau đây, bổ đề này sẽ được chứng minh ở Chương VIII (§ 2, No. 5).

\* Bổ đề 3. — Cho $A$ là một K-đại số, $M_1$ và $M_2$ là hai A-môđun có hạng hữu hạn trên $K$ và giả sử rằng tồn tại một mở rộng $L$ của $K$ sao cho các môđun $L \otimes_K M_1$ và $L \otimes_K M_2$ trên vành $L \otimes_K A$ là đẳng cấu. Khi đó các A-môđun $M_1$ và $M_2$ đẳng cấu.

Ta sẽ áp dụng Bổ đề 3 trong trường hợp $A = \mathbf{K}^{(\Gamma)}$, $M_1 = N$, $M_2 = A$, và $L = N$. Theo Hệ quả của V, p. 64 tồn tại một K-đẳng cấu $\varphi$ của $N \otimes_K N$ lên $N \otimes_K \mathbf{K}^{(\Gamma)}$ gửi $x \otimes y$ thành $\sum x u^1(y) \otimes \sigma$. Rõ ràng rằng $\varphi$ là một đẳng cấu của các $N \otimes_K \mathbf{K}^{(\Gamma)}$-môđun, nên định lý suy ra từ Bổ đề 3.

Cho chứng minh thứ hai ta sẽ dùng mệnh đề sau:

#### Mệnh đề 10 {#alg-v-s10-prop-10 .statement}

*Cho $x \in N$, khi đó để $\{x\}$ lập thành một cơ sở của $\mathbf{K}^{(\Gamma)}$-môđun $N$ thì cần và đủ là $\det(\sigma \tau(x))_{\sigma, \tau \in \Gamma} \neq 0$.

Vì $\mathbf{K}^{(\Gamma)}$ và $N$ có cùng chiều trên $K$, nói rằng $\{x\}$ là một cơ sở của $N$ trên $\mathbf{K}^{(\Gamma)}$ nghĩa là ánh xạ $a \mapsto ax$ từ $\mathbf{K}^{(\Gamma)}$ vào $N$ là đơn ánh. Điều này lại có nghĩa là ánh xạ $b \mapsto b(1 \otimes x)$ từ $N \otimes_K \mathbf{K}^{(\Gamma)}$ vào $N \otimes_K N$ là đơn ánh (II, p. 306, Mệnh đề 14). Bây giờ có một đẳng cấu của các $N \otimes_K \mathbf{K}^{(\Gamma)}$-môđun từ $N \otimes_K N$ lên $N \otimes_K \mathbf{K}^{(\Gamma)}$ gửi $1 \otimes x$ thành $\sum \sigma^{-1}(x) \otimes \sigma$. Suy ra rằng $\{x\}$ là một cơ sở của $N$ trên $\mathbf{K}^{(\Gamma)}$ khi và chỉ khi, với mọi họ phần tử khác không $(n_\tau)$ của $N$ ta có $\left( \sum n_\tau \otimes \tau \right) \left( \sum \sigma^{-1}(x) \otimes \sigma \right) \neq 0$. Nhưng hệ thức cuối cùng này có nghĩa là tồn tại $\sigma \in \Gamma$ sao cho $\sum n_\tau \sigma^{-1}(x) \neq 0$, do đó mệnh đề.

\* A) Giả sử rằng $K$ là vô hạn; ánh xạ $x \mapsto \det(\sigma \tau(x))$ của $N$ vào $N$ là một ánh xạ đa thức trên $K$ (IV, p. 54). Bằng cách mở rộng vô hướng từ $K$ sang $N$, ta thu được một ánh xạ tương ứng cho không gian vectơ trên $N$ $N \otimes_K N$ và ta vừa thấy rằng ánh xạ sau không đồng nhất bằng 0 (vì $N \otimes_K N$ là tự do hạng 1 trên $N \otimes_K \mathbf{K}^{(\Gamma)}$). Vậy tồn tại $x \in N$ sao cho $\det(\sigma \tau(x)) \neq 0$ (IV, p. 18, Định lý 2); nói chung hơn, từ cùng tài liệu tham khảo này ta có:

#### Mệnh đề 11 {#alg-v-s10-prop-11 .statement}

— Giả sử K là vô hạn và cho P : N → K là một ánh xạ đa thức không đồng nhất bằng 0 trên K. Tồn tại x ∈ N sao cho P(x) ≠ 0 và {x} là một cơ sở của N trên $\mathbf{K}^{(\Gamma)}$.

B) Giả sử K là hữu hạn. Theo Mệnh đề 4 (V, p. 95)$^1$ mọi mở rộng có bậc hữu hạn trên K đều có một nhóm Galois cyclic. Vì vậy nói chung hơn, ta xét trường hợp mà nhóm $\Gamma$ là cyclic cấp n; ta ký hiệu $\gamma$ là một phần tử sinh của $\Gamma$.

Bổ đề sau là một trường hợp riêng của các kết quả tổng quát hơn được chứng minh trong Chương VII. Vành $A$ hoặc là vành $\mathbf{Z}$ của các số nguyên hoặc là vành $K[X]$ của các đa thức trên trường $K$.

#### Bổ đề 4 {#alg-v-s10-lem-4 .statement}

Cho M là một A-môđun xoắn được sinh bởi một số hữu hạn phần tử $x_1, ..., x_h$; khi đó tồn tại một phần tử x của M mà linh hóa tử (II, p. 219) của nó bằng linh hóa tử của M.

Trong cả hai trường hợp, $A$ là một miền nguyên và mọi iđêan của $A$ đều chính. Khi $A = \mathbf{Z}$ (resp. $A = K[X]$), ta ký hiệu bởi $\mathcal{P}$ tập hợp các số nguyên tố (resp. tập hợp các đa thức monic bất khả quy trong $K[X]$). Với mỗi phần tử $a \neq 0$ của $A$ khi đó tồn tại một phần tử khả nghịch $u$ của $A$ và một họ $(v_p(a))_{p \in \mathcal{P}}$, có giá hữu hạn, của các số nguyên dương sao cho $a = u \prod_{p \in \mathcal{P}} p^{v_p(a)}$ và $u$ cùng các số nguyên $v_p(a)$ được xác định duy nhất (I, p. 51 và IV, p. 13, Mệnh đề 13).

Cho $a_i$ là linh hóa tử của $x_i$, (với $1 \leq i \leq h$) và $a$ là linh hóa tử của M; cho $a_1, ..., a_h, a$ là các phần tử khác 0 của $A$ sao cho $a_i = Aa_i$, và $a = Aa$; vì $a = a_1 \cap ... \cap a_h$, suy ra từ điều vừa nói rằng

$$
v_p(a) = \sup_{1 \leq i \leq h} v_p(a_i) \quad \text{cho mọi } p \in \mathcal{P}.
$$

Ta viết $a$ dưới dạng $up_1^{n(1)} ... p_r^{n(r)}$, với $p_1, ..., p_r$ phân biệt trong $\mathcal{P}$, $n(1) > 0, ..., n(r) > 0$ và $u$ là một phần tử khả nghịch của $A$. Cho $j = 1, ..., r$; theo (10) tồn tại một số nguyên $c(j)$ sao cho $1 \leq c(j) \leq h$ và $v_{p_j}(a_{c(j)}) = n(j)$; tồn tại $b_j$ trong $A$ sao cho $a_{c(j)} = p_j^{n(j)} b_j$ và phần tử $y_j = b_j x_{c(j)}$ có linh hóa tử là iđêan $Ap_j^{n(j)}$.

Ta sẽ chứng minh rằng linh hóa tử b của $y = y_1 + ... + y_r$ bằng linh hóa tử a của M. Dù sao ta cũng có $a \subset b$, nên b có dạng $Ap_1^{m(1)} ... p_r^{m(r)}$ với $0 \leq m(j) \leq n(j)$ cho $1 \leq j \leq r$. Nếu ta có $a \neq b$, thì sẽ tồn tại một số nguyên j sao cho $1 \leq j \leq r$ và $m(j) < n(j)$, và do đó $d_j = a/p_j$ sẽ triệt tiêu $y$. Nay ta có $d_j y_k = 0$ với $k \neq j$, do đó suy ra $d_j y_j = 0$; nhưng linh hóa tử của $y_j$ là $Ap_j^{m(j)}$ và $d_j$ không phải là một bội của $p_j^{m(j)}$. Vậy giả thiết $a \neq b$ là vô lý.

$^1$ Người đọc có thể dễ dàng tự thuyết phục rằng định lý cơ sở chuẩn không được dùng ở đâu trước chứng minh của mệnh đề đó.

Ta sẽ áp dụng Bổ đề 4 cho trường hợp $A$ là vành đa thức $K[X]$ và $M$ là nhóm Abel $N$ với phép toán ngoài được xác định bởi $a \cdot x = \sum_{k=0}^m c_k \gamma^k(x)$ với $a = \sum_{k=0}^\infty c_k X^k$ trong $K[X]$ và $x \in N$. Gọi $a$ là linh hóa tử của $M$, khi đó $\gamma^n = 1$, do đó đa thức $X^n - 1$ thuộc $a$. Lấy $F \in a$; *theo IV*, p. 11, Hệ quả, tồn tại các phần tử $c_0, c_1, \ldots, c_{n-1}$ của $K$ và $G \in K[X]$ sao cho

$$
F(X) = c_0 + c_1 X + \cdots + c_{n-1} X^{n-1} + (X^n - 1) G(X).
$$

Vậy ta có $c_0 + c_1 \gamma + \ldots + c_{n-1} \gamma^{n-1} = 0$ trong $\operatorname{Hom}_K(N, N)$ và vì các tự đẳng cấu $1, \gamma, \gamma^2, \ldots, \gamma^{n-1}$ của $N$ là phân biệt, định lý của Dedekind (*V*, p. 27, Hệ quả 2) suy ra rằng $c_0 = c_1 = \ldots = c_{n-1} = 0$. Cuối cùng, ta có

$$
F(X) = (X^n - 1) G(X), \quad \text{tức là, } a = (X^n - 1) K[X].
$$

Theo Bổ đề 4 tồn tại một phần tử $x$ của $N$ có linh hóa tử trong $K[X]$ bằng $(X^n - 1) K[X]$. Vì các đơn thức $1, X, \ldots, X^{n-1}$ lập thành một cơ sở của một không gian con vectơ của $K[X]$ bổ sung cho $(X^n - 1) K[X]$ (*IV*, p. 11, Hệ quả), nên các phần tử $x, \gamma(x), \ldots, \gamma^{n-1}(x)$ của $N$ là độc lập tuyến tính trên $K$. Vì $[N : K] = n$ (*V*, p. 66, Định lý 3), nên dãy $(x, \gamma(x), \ldots, \gamma^{n-1}(x))$ do đó là một cơ sở chuẩn của $N$ trên $K$.

### 10. Các $\Gamma$-tập hợp hữu hạn và các đại số etale

Cho $K_s$ là một bao đóng tách được của $K$ (*V*, p. 45, Mệnh đề 14) và $\Gamma$ là nhóm Galois của $K$, trên $K$. Ta hiểu một $\Gamma$-*tập hợp* là một tập hợp $X$ với một tác động $(\sigma, x) \mapsto \sigma x$ của nhóm $\Gamma$ sao cho nhóm ổn định của mỗi điểm của $X$ là một nhóm con *mở* của $\Gamma$. Điều đó cũng tương đương với việc nói rằng ánh xạ $(\sigma, x) \mapsto \sigma x$ của $\Gamma \times X$ vào $X$ là *liên tục* khi $X$ được trang bị tôpô rời rạc.

Cho $X$ là một $\Gamma$-tập hợp hữu hạn. Ta định nghĩa một tác động của $\Gamma$ lên đại số trên $K$ $K_s^X$ gồm các ánh xạ của $X$ vào $K_s$ bởi công thức

$$
u_\sigma f(x) = \sigma(f(\sigma^{-1}x))
$$

với $\pi \in \Gamma, f \in K_s^X$ và $x \in X$. Gọi $\Theta(X)$ là tập các phần tử bất biến của $\Gamma$ trong $K_s^X$; đây là đại số con trên $K$ của $K_s^X$ gồm các ánh xạ $f : X \to K_s$ sao cho $f(\sigma x) = \sigma(f(x))$ với $\sigma \in \Gamma$ và $x \in X$.

#### Bổ đề 5 {#alg-v-s10-lem-5 .statement}

*Cho $X$ là một $\Gamma$-tập hợp hữu hạn và cho $x_1, \ldots, x_n$ là các điểm của $X$ sao cho các quỹ đạo $\Gamma x_1, \ldots, \Gamma x_n$ tạo thành một phân hoạch của $X$. Với $1 \leq i \leq n$ cho $\Delta_i$ là nhóm ổn định của $x_i$ trong $\Gamma$ và cho $L_i$ là trường bất biến của $A_i$. Khi đó $L_1, \ldots, L_n$ là các mở rộng tách được bậc hữu hạn của $K$, và ánh xạ $f \mapsto (f(x_1), \ldots, f(x_n))$ là một đẳng cấu đại số trên $K$ từ $\Theta(X)$ lên $L_1 \times \ldots \times L_n$.*

Theo giả thiết, các nhóm con $A_i, \ldots, A_n$ của $\Gamma$ là mở và Hệ quả 5 của V, p. 68, cho thấy rằng các mở rộng con $L_1, \ldots, L_n$ của $K$ đều có bậc hữu hạn trên $K$. Rõ ràng chúng là tách được; bây giờ mệnh đề cuối cùng của Bổ đề 5 suy ra ngay lập tức.

Từ Bổ đề 5 và Định lý 4 (*V*, p. 34f.) ta thu được ngay lập tức kết quả sau.

#### Mệnh đề 12 {#alg-v-s10-prop-12 .statement}

— Với mọi $\Gamma$-tập hợp hữu hạn $X$ đại số $\Theta(X)$ là êtan trên $K$, có bậc bằng lực lượng của $X$. Hơn nữa, mọi đại số êtan trên $K$ đều đẳng cấu với một đại số có dạng $\Theta(X)$.

#### Nhận xét {#alg-v-s10-n10-rem-1 .statement}

a) Dễ dàng chứng minh rằng với mọi đồng cấu đại số trên $K$ $\varphi$ từ $\Theta(X)$ vào $K$, tồn tại một phần tử duy nhất $x$ của $X$ sao cho $\varphi(f) = f(x)$ với mọi $f \in \Theta(X)$.

2) Cho $X$ và $Y$ là hai $\Gamma$-tập hợp hữu hạn. Cho $\mathfrak{T}_\Gamma(X, Y)$ là tập hợp các ánh xạ $u$ từ $X$ vào $Y$ sao cho $u(\sigma x) = \sigma u(x)$ với mọi $\sigma \in \Gamma$ và mọi $x \in X$. Với $u \in \mathfrak{T}_\Gamma(X, Y)$ ta định nghĩa một đồng cấu đại số trên $K$ $u^*: \Theta(Y) \to \Theta(X)$ bởi $u^*(f) = f \circ u$. Với mọi đồng cấu $\Psi$ từ $\Theta(Y)$ vào $\Theta(X)$ tồn tại một phần tử duy nhất $u$ của $\mathfrak{T}_\Gamma(X, Y)$ sao cho $\Psi = u^*$.

### 11. Cấu trúc của các mở rộng quasi-Galois

#### Mệnh đề 13 {#alg-v-s10-prop-13 .statement}

— Cho $N$ là một mở rộng quasi-Galois của $K$. Ký hiệu $N_r$ là trường bất biến của nhóm tất cả các $K$-tự đẳng cấu của $N$ và ký hiệu $N_s$ là bao đóng đại số tách được tương đối của $K$ trong $N$ ($V$, p. 44). Khi đó:

a) $N_r$ là bao đóng $p$-căn tương đối của $K$ trong $N$ ($V$, p. 25).

b) $N$, là một mở rộng Galois của $K$ và mọi $K$-tự đẳng cấu của $N_s$ đều mở rộng một cách duy nhất thành một $N_r$-tự đẳng cấu của $N$.

c) Các trường $N_r$ và $N$, rời tuyến tính trên $K$ và ta có $N = K[N, \cup N_s]$; nói cách khác, đồng cấu chính tắc từ $N_r \otimes_K N$, vào $N$ là một đẳng cấu.

Cho $\Omega$ là một bao đóng đại số của $K$ chứa $N$ như một mở rộng con ($V$, p. 23, Định lý 2). Mọi $K$-tự đẳng cấu của $\Omega$ đều cảm sinh ra một tự đẳng cấu của $N$ vì $N$ là quasi-Galois. Do đó mọi phần tử của $N_r$ đều bất biến dưới nhóm các $K$-tự đẳng cấu của $\Omega$, suy ra $p$-căn trên $K$ ($V$, p. 53, Hệ quả 3). Ngược lại mọi phần tử của $N$ mà là $p$-căn trên $K$ đều rõ ràng bất biến dưới mọi $K$-tự đẳng cấu của $N$ và do đó thuộc $N_r$. Điều này chứng minh a).

Every $K$-tự đẳng cấu của $\Omega$ đưa $N$ vào $N$, do đó $N_r$ vào $N_r$, nên $N_r$ là một mở rộng quasi-Galois của $K$ ($V$, p. 54, Mệnh đề 3). Suy ra $N_s$ là một mở rộng Galois của $K$. Mọi phần tử của $N_r \cap N$, là đại số tách được và $p$-căn trên $K$, nên thuộc $K$ ($V$, p. Hệ quả 3); vì vậy ta có $K_r \cap K_s = K$. Bây giờ $N$ là $p$-căn trên $N_r$ ($V$, p. 44, Mệnh đề 13) và đại số tách được trên $N_r$ ($V$, p. 56, Định lý 1) nên vừa $p$-căn vừa tách được trên $K(N_r \cup N_s)$. Do đó ta có $N = K(N_r \cup N_s)$ ($V$, p. 39, Hệ quả 3) và các mệnh đề b), c) suy ra từ Định lý 5 ($V$, p. 71).

#### Hệ quả {#alg-v-s10-n11-cor-1 .statement}

— Cho $p$ là số mũ đặc số của $K$, $\overline{K}$ là một bao đóng đại số của $K$, $K_s$, là bao đóng tách được tương đối của $K$ trong $\overline{K}$ và $K^{p^{-\infty}}$ là bao đóng hoàn hảo của $K$. Khi đó đồng cấu chính tắc của $K^{p^\infty} \otimes K_s$ vào $\overline{K}$ là một đẳng cấu.

#### Nhận xét {#alg-v-s10-n11-rem-1 .statement}

Cho $R$ (tương ứng $S$) là một mở rộng $p$-căn (tương ứng đại số tách được) của $K$. Khi đó đại số $R \otimes_K S$ là một trường : vì $R$ (tương ứng $S$) đẳng cấu với một mở rộng con của $K^{p^\infty}$ (tương ứng $K_s$) và chỉ cần áp dụng hệ quả trên và Mệnh đề 1 của $V$, p. 17.

### Bài tập {#alg-v-s10-exercises}

Xem [các bài tập của § 10](exercises/s10/).
