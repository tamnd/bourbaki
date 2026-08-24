---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 13
section_title: p-radical extensions of height _ 1
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.98-A V.106, A V.170-A V.171
pdf_pages: 0212-0220, 0284-0285
extraction: ocr
subsections:
    - "no": 1
      title: $p$-free subsets and pbases
      page: 98
      pdf_page: 212
    - "no": 2
      title: Differentials and pbases
      page: 100
      pdf_page: 214
    - "no": 3
      title: The correspondence between subfields and Lie algebras of derivations
      page: 104
      pdf_page: 218
statements: 21
exercises: 6
content_sha256: 7885820d9be314e63df2bfd66fad78282fed8a7552ba254add76860c264573fe
translated_from: content/en/alg/V/13_s13_p_radical_extensions_of_height_1.md
source_content_sha256: ea1922d9b090562a960823c783889969946827bc39b5551a52700d5ebe93e171
translation_model: gpt-5.4, gpt-5-6-mini, copied
translation_run: translate-vi-d004b81c
glossary_version: 34
glossary_terms_sha256: 090fbc15138f46a7b8eb22c24f1f9bb9f05e4f8187caa8374ceed9ffbfbb2499
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 13. CÁC MỞ RỘNG $p$-CĂN CÓ CHIỀU CAO $\leq 1$

Trong suốt đoạn này, $p$ ký hiệu một số nguyên tố. Mọi trường được xét đều có đặc số $p$.

### 1. Các tập con $p$-tự do và các p-cơ sở

#### Định nghĩa 1 {#alg-v-s13-def-1 .statement}

Cho $K$ là một trường và $L$ là một mở rộng căn-bậc-$p$ có chiều cao $\leq 1$ của $K$. Một họ $(x_i)_{i \in I}$ các phần tử của $L$ được gọi là $p$-tự do trên $K$ (resp. một $p$-cơ sở của $L$ trên $K$) nếu $x_i \notin K$ với mọi $i \in I$ và đồng cấu từ $\bigotimes_{i \in I} K(x_i)$ vào $L$ suy ra từ các đơn ánh chính tắc $u_i : K(x_i) \to L$ là đơn ánh (resp. song ánh).

Nếu $a$ là một phần tử của $L - K$, thì nó là căn-$p$ cấp 1, và do đó đa thức tối tiểu của nó trên $K$ là $X^p - a^p$ ($V$, p. 24, Mệnh đề 1); vì vậy $\{1, a, \ldots, a^{p-1}\}$ là một cơ sở của $K(a)$ trên $K$. Cho $(x_i)_{i \in I}$ là một họ các phần tử của $L - K$ và $A$ là tập con của $\mathbf{N}^{(I)}$ gồm tất cả các họ có giá hữu hạn $a = (\alpha_i)_{i \in I}$, sao cho $\alpha_i < p$ với mọi $i \in I$; Mệnh đề 9 (III, p. 471) cho thấy rằng các phần tử $\bigotimes_{i \in I} x_i^{\alpha_i}$ khi $a$ chạy qua $A$ lập thành một cơ sở của không gian vectơ $\bigotimes_{i \in I} K(x_i)$ trên $K$. Hơn nữa, đồng cấu chính tắc từ $\bigotimes_{i \in I} K(x_i)$ vào $L$ có ảnh là $K(x_i)_{i \in I}$ ($V$, p. 18, Hệ quả 1), do đó ta có mệnh đề sau:

#### Mệnh đề 1 {#alg-v-s13-prop-1 .statement}

Cho $K$ là một trường, $L$ là một mở rộng căn $p$ có chiều cao $\leq 1$ của $K$ và $x = (x_i)_{i \in I}$ là một họ các phần tử của $L$. Khi đó không gian vectơ $K(x_i)_{i \in I}$ trên $K$ được sinh bởi các tích $x'' = \prod_{i \in I} x_i^{\alpha_i}$ với $a$ trong $A$. Để $(x_i)_{i \in I}$ là $p$-tự do (tương ứng, một $p$-cơ sở), điều kiện cần và đủ là họ $(x^a)_{a \in A}$ tự do trên $K$ (tương ứng, là một cơ sở của $L$ trên $K$).

#### Hệ quả {#alg-v-s13-n1-cor-1 .statement}

— Cho L' là một mở rộng của một trường K, được sinh bởi hai mở rộng con K' và L rời nhau tuyến tính. Giả sử rằng L là p-căn cấp $ \leq 1 $ trên K; *khi đó* L' là p-căn cấp $ \leq 1 $ trên K'. Hơn nữa, để một họ phần tử của L là p-tự do trên K (tương ứng, một p-cơ sở của $ L $ trên K) thì điều kiện cần và đủ là nó p-tự do trên K' (tương ứng, một p-cơ sở của L' trên K').

Ta có $ L'^p \subset K \subset K' $ và $ L' = K'(L) $, do đó $ L'^p = K'^p(L'^p) \subset K' $. Nói cách khác, L' là một mở rộng p-căn cấp $ \leq 1 $ của K'. Các khẳng định khác của hệ quả suy ra ngay từ Mệnh đề 1 và từ V, p. 14, Mệnh đề 5.

#### Nhận xét {#alg-v-s13-n1-rem-1 .statement}

Cho K là một trường, L là một mở rộng căn p có chiều cao $ \leq 1 $ của K và $ (x_i)_i $, một họ các phần tử của L. Cho A là đại số đa thức $ K[(X_i)_{i \in I}] $, a là iđêan của A sinh bởi các đa thức $ X_i^p - x_i^p $ và $ \varphi : A \to L $ là đồng cấu đại số trên K sao cho $ \varphi(X_i) = x_i $ với mỗi $ i \in I $. Họ $ (x_i)_i $, là p-tự do khi và chỉ khi hạt nhân của $ \varphi $ bằng a. Vì $ K[(X_i)]/a $ có thể được đồng nhất với đại số $ \bigotimes_{i \in I} K[X_i]/(X_i^p - x_i^p) $.

Cho L là một mở rộng căn p có chiều cao $ \leq 1 $ của trường K. Một tập con S của $ L $ được gọi là p-tự do (tương ứng, là một cơ sở p) nếu họ được xác định bởi ánh xạ đồng nhất của S lên chính nó là p-tự do (tương ứng, là một cơ sở p). Để một họ $ (x_i)_i $, gồm các phần tử của $ L $, là p-tự do (tương ứng, là một cơ sở p), điều kiện cần và đủ là ánh xạ $ i \mapsto x_i $ là một song ánh từ I lên một tập con p-tự do (tương ứng, một cơ sở p) của L. Theo Mệnh đề 1, mọi tập con của một tập hợp p-tự do đều là p-tự do; ngược lại, nếu S là một tập con của L mà mọi tập con hữu hạn của nó đều p-tự do, thì S là p-tự do. Cuối cùng, một cơ sở p của L trên K là một tập con p-tự do B sao cho $ L = K(B) $.

#### Mệnh đề 2 {#alg-v-s13-prop-2 .statement}

— Cho K là một trường, $ L $ là một mở rộng căn p có chiều cao $ \leq 1 $ của K và S là một tập con của L. Điều kiện cần và đủ để S là p-tự do là $ K(T) \neq K(S) $ với mọi tập con $ T \neq S $ của S.

Trước hết giả sử rằng S là p-tự do và gọi $ T \neq S $ là một tập con của S. Ký hiệu bởi A tập hợp các họ có giá hữu hạn $ a = (\alpha_s)_{s \in S} $ gồm các số nguyên từ 0 đến $ p-1 $; gọi $ A' $ là tập con của A gồm các họ $ a = (\alpha_s)_{s \in S} $ sao cho $ a_s = 0 $ với mọi s trong $ S - T $. Ta cũng đặt $ u_a = \prod_{s \in S} s^{\alpha_s} $ với $ a \in A $. Khi đó (V, p. 98, Mệnh đề 1) họ $ (u_a)_{a \in A'} $ là một cơ sở của $ K(S) $ trên K và họ con $ (u_a)_{a \in A'} $ là một cơ sở của $ K(T) $ trên K. Vì $ A' \neq A $, suy ra $ K(T) \neq K(S) $.

Giả sử bây giờ rằng S không p-tự do. Khi đó tồn tại một số nguyên $ n \geq 1 $ và một dãy các phần tử $ x_1, ..., x_n $ của S sao cho $ (x_1, ..., x_{n-1}) $ là p-tự do nhưng $ (x_1, ..., x_n) $ thì không. Ta có $ [K(x_1, ..., x_{n-1}):K] = p^{n-1} $ và $ [K(x_1, ..., x_n):K] < p^n $. Vì $ [K(x_1, ..., x_n):K] $ là một bội của $ [K(x_1, ..., x_{n-1}):K] $, do đó ta có

$$
[K(x_1, ..., x_n):K] = [K(x_1, ..., x_{n-1}):K].
$$

do đó $ x_n \in K(x_1, ..., x_{n-1}) $. Điều này cho thấy rằng $ K(S - \{x_n\}) = K(S) $.

#### Mệnh đề 3 {#alg-v-s13-prop-3 .statement}

— Cho K là một trường, L là một mở rộng căn p có chiều cao $ \leq 1 $ của K, và S, T là hai tập con của L. Các điều kiện sau là tương đương:
a) Tập con S là p-tự do trên K và T là p-tự do trên K(S).
b) $ S \cap T = \varnothing $ *và* S U T là p-tự do trên K.
Nếu T là p-tự do trên K(S), ta có $ T \cap K(S) = \varnothing $ và a fortiori $ S \cap T = \varnothing $. Do đó ta có thể giả sử S và T rời nhau. Gọi A là tập con của $ N^{(S \cup T)} $ gồm mọi họ $ a = (a_x)_{x \in S \cup T} $ sao cho $ a_x < p $ với mọi $ x \in S \cup T $, và định nghĩa các tập con $ A' $ của $ N^{(S)} $ và $ A'' $ của $ N^{(T)} $ theo cách tương tự. Ta có thể, một cách tự nhiên, đồng nhất $ N^{(S \cup T)} $ với $ N^{(S)} \times N^{(T)} $, và khi đó A được đồng nhất với $ A' \times A'' $. Với $ a \in A $ đặt $ u_a = \prod_{x \in S \cup T} x^{\alpha_x} $, và tương tự định nghĩa $ u'_\beta $ và $ u''_\gamma $ đối với $ \beta \in A' $ và $ \gamma \in A'' $. Ta có $ u_a = u'_\beta u''_\gamma $ với $ a = (\beta, \gamma) $ trong $ A = A' \times A'' $. Hơn nữa $ (u'_\beta)_{\beta \in A'} $ sinh ra không gian vectơ K K(S) (V, p. 94, Prop. 1). Để S U T là p-tự do trên K, điều kiện cần và đủ là họ $ (u'_\beta u''_\gamma)_{\beta \in A', \gamma \in A''} $ là tự do trên K (V, p. 98, Prop. 1); điều đó cũng tương đương (II, p. 222) với việc giả sử rằng họ $ (u'_\beta)_{\beta \in A'} $ là tự do trên K và họ $ (u''_\gamma)_{\gamma \in A''} $ là tự do trên K(S). Bây giờ tính tương đương của a) và b) suy ra từ Prop. 1 (V, p. 98).

#### Hệ quả {#alg-v-s13-n1-cor-2 .statement}

— Cho L là một mở rộng căn p có chiều cao $ \leq 1 $ của K và M là một mở rộng con của L. Khi đó L là căn p có chiều cao $ \leq 1 $ trên M và M là căn p có chiều cao $ \leq 1 $ trên K. Hơn nữa, nếu B là một cơ sở p của M trên K và C là một cơ sở p của L trên M, thì $ B \cap C = \varnothing $ và $ B \cup C $ là một cơ sở p của L trên K.

Cho K là một trường. Một họ $ (x_i)_{i \in I} $ được gọi là một cơ sở p (tuyệt đối) của K nếu nó là một cơ sở p của K trên $ K^p $. Với mọi số nguyên $ n \geq 1 $ ta ký hiệu bởi $ \Lambda(n) $ tập con của $ N^{(1)} $ gồm tất cả các $ a = (\alpha_i)_{i \in I} $ sao cho $ \alpha_i < p^n $ với mọi $ i \in I $.

#### Mệnh đề 4 {#alg-v-s13-prop-4 .statement}

— Cho $ x = (x_i)_{i \in I} $ là một p-cơ sở của K. Với mọi số nguyên $ n \geq 1 $, họ $ (x^u)_{u \in \Lambda(n)} $ là một cơ sở của K trên $ K^{p^n} $.

Với $ n = 1 $ thì mệnh đề quy về Mệnh đề 1 (V, p. 98). Tập hợp $ \Lambda(n) $ gồm các phần tử của $ N^{(1)} $ có dạng $ a = \beta + p^{n-1}\gamma $ với $ \beta \in \Lambda(n-1) $ và $ \gamma \in \Lambda(1) $. Phân tích như vậy là duy nhất và ta có $ x^\alpha = x^\beta (x^\gamma)^{p^{n-1}} $. Hơn nữa, họ $ (x_i^{p^{n-1}})_{i \in I} $ rõ ràng là một p-cơ sở của $ K^{p^{n-1}} $ trên $ K^{p^n} $, do đó họ $ (x^\gamma)^{p^{n-1}} $ là một cơ sở của $ K^{p^{n-1}} $ trên $ K^{p^n} $. Như vậy ta thu được kết luận bằng quy nạp, dùng II, p. 222, Mệnh đề 25.

### 2. Vi phân và p-cơ sở

Cho K là một trường (có đặc số p) và V là một không gian vectơ trên K. Ta nhắc lại (III, p. 552) rằng một đạo hàm của K vào V là một ánh xạ D từ K vào V thỏa mãn các hệ thức
$$
\begin{align*}
D(x + y) &= D(x) + D(y) \\
D(xy) &= xD(y) + yD(x)
\end{align*}
$$

với $ x,\ y \in K $. Suy ra $ D(1) = 0 $ và $ D(x^n) = nx^{n-1}D(x) $ với mọi $ x \neq 0 $ và mọi $ n \in \mathbf{Z} $ (III, p. 557 và 558). Vì $ K $ có đặc số $ p $, do đó với mọi $ x \in K $ ta có

$$
D(x^p) = 0 .
$$

Hơn nữa (III, p. 558), với $ x,\ y \in K,\ y \neq 0 $, ta có

$$
D(x/y) = (yD(x) - xD(y))/y^2
$$

Theo các công thức trên, hạt nhân của $ D $ là một trường con $ E $ của $ K $ chứa $ K^p $. Cho $ M $ là một trường con của $ K $; ta nói rằng $ D $ là một $ M $-đạo hàm nếu nó là $ M $-tuyến tính ; theo (2), điều đó cũng tương đương với việc giả sử rằng hạn chế của $ D $ trên $ M $ là không.

Trong (III, p. 570), chúng tôi đã định nghĩa môđun $ \Omega_M(K) $ các $ M $-vi phân của $ K $ và đạo hàm $ M $ chính tắc $ d = d_{K/M} $ từ $ K $ vào $ \Omega_M(K) $. Ảnh của $ d_{K/M} $ sinh ra không gian vectơ trên $ K $ $ \Omega_M(K) $. Để một ánh xạ $ D $ từ $ K $ vào $ V $ là một $ M $-đạo hàm, điều kiện cần và đủ là tồn tại một ánh xạ tuyến tính $ K $ $ u : \Omega_M(K) \to V $ sao cho $ D = u \circ d_{K/M} $; ánh xạ này $ u $ được xác định duy nhất.

#### Mệnh đề 5 {#alg-v-s13-prop-5 .statement}

*Cho $ K $ là một trường và $ L $ là một mở rộng của $ K $ sinh bởi một phần tử $ x $ sao cho $ x \notin K,\ x^p \in K $. Gọi $ V $ là một không gian vectơ trên $ L $ và $ A $ là một đạo hàm của $ K $ vào $ V $ sao cho $ \Delta(x^p) = 0 $. Khi đó tồn tại một đạo hàm duy nhất $ D $ của $ L $ vào $ V $ mở rộng $ A $ và sao cho $ D(x) = 0 $. \*

Theo $ V $, p. 24, Mệnh đề 1, $ \{1,\ x,\ \ldots,\ x^{p-1}\} $ là một cơ sở của $ L $ trên $ K $. Với mọi phần tử $ u = a_0 + a_1x + \ldots + a_{p-1}x^{p-1} $ của $ L $ (với $ a_0,\ \ldots,\ a_{p-1} $ thuộc $ K $) ta đặt $ D(u) = A(a_0) + x\Delta(a_1) + \ldots + x^{p-1}\Delta(a_{p-1}) $. Hiển nhiên $ D $ mở rộng $ A $ và thỏa mãn (1); do đó chỉ cần thiết lập quan hệ

$$
D(uv) = u \cdot D(v) + v \cdot D(u)
$$

khi $ u $ có dạng $ ax^i $ và $ v $ có dạng $ bx^j $ với $ a,\ b $ thuộc $ K,\ 0 \leq i < p $ và $ 0 \leq j < p $.

Khi $ i + j < p $ thì ta có $ uv = x^{i+j}ab $, do đó $ D(uv) = x^{i+j}\Delta(ab) $. Nếu không thì ta có $ 0 \leq i + j - p < p $ và vì thế $ uv = x^{i+j-p}(abx^p) $, với $ abx^p \in K $, nhưng vì $ A(x^p) = 0 $, ta có $ A(abx^p) = x^pA(ab) $, do đó lại có $ D(uv) = x^{i+j}\Delta(ab) $. Vậy trong mọi trường hợp ta có

$$
\begin{align*}
D(uv) &= x^{i+j}\Delta(ab) = x^i x^j (a \cdot A(b) + b \cdot \Delta(a)) \\
&= (ax^i)x^j \cdot \Delta(b) + (bx^j)x^i \cdot \Delta(a) = u \cdot D(v) + v \cdot D(u) .
\end{align*}
$$

#### Hệ quả 1 {#alg-v-s13-prop-5-cor-1 .statement}

*Cho $ K $ là một trường, $ L $ là một mở rộng căn bậc $ p $ có chiều cao $ \leq 1 $ của $ K $ và $ V $ là một không gian vectơ trên $ L $. Mọi đạo hàm $ A $ của $ K $ vào $ V $ triệt tiêu trên $ L^p $ đều mở rộng được thành một đạo hàm của $ L $ vào $ V $.

Theo bổ đề Zorn (E, III, p. 20) tồn tại một mở rộng cực đại của $ A $ thành một đạo hàm $ D_0 : L_0 \to V $, trong đó $ L_0 $ là một trường con của $ L $ chứa $ K $. Cho $ x \in L $; ta có $ x^p \in L_0 $ và $ A(x^p) = 0 $, do đó $ D_0(x^p) = 0 $. Theo Mệnh đề 5,

D_0 mở rộng thành một đạo hàm xác định trên L_0(x); bởi tính chất cực đại của D_0 suy ra L_0(x) = L, do đó x ∈ L_0. Vì x là tùy ý, ta kết luận rằng L_0 = L.

#### Hệ quả 2 {#alg-v-s13-prop-5-cor-2 .statement}

—Cho L là một mở rộng p-căn có chiều cao ≤ l của một trường K và E là một mở rộng con của L. Gọi U là không gian con của Ω_K(L) được sinh bởi các vi phân của các phần tử của E. Khi đó E gồm các phần tử của L mà vi phân của chúng thuộc U. Đặc biệt ta có d_{L/K}x ≠ 0 với mọi x ∈ L − K.

Cho x là một phần tử của L không thuộc E. Khi đó {1, x, ..., x^{p^{l-1}}} là một cơ sở của E(x) trên E. Gọi A là ánh xạ E-tuyến tính từ E(x) vào L sao cho Δ(x^i) = ix' với 0 ≤ i < p. Ta kiểm tra ngay được rằng A là một E-đạo hàm từ E(x) vào L, và đặc biệt là một K-đạo hàm. Theo Hệ quả 1 của Mệnh đề 5, tồn tại một K-đạo hàm D từ L vào L mở rộng A. Theo tính chất phổ quát của Ω_K(L), tồn tại một dạng tuyến tính u trên không gian vectơ L này sao cho D = u ∘ d_{L/K}. Ta có D(x) = x và D|E = 0; do đó ta có u(d_{L/K}x) ≠ 0 và u|U = 0, suy ra d_{L/K}x ∉ U.

Khẳng định cuối cùng là trường hợp riêng E = K; khi đó ta có U = 0.

#### Định lý 1 {#alg-v-s13-thm-1 .statement}

—Cho L là một mở rộng p-căn có chiều cao ≤ l của một trường K và (a_i)_{i ∈ I}, một họ các phần tử của L.

a) Để (x_i)_{i ∈ I} là p-tự do trên K, điều kiện cần và đủ là họ (dx_i)_{i ∈ I} tự do trong không gian vectơ L Ω_K(L).

b) Để (x_i)_{i ∈ I} sinh ra L trên K, điều kiện cần và đủ là họ (dx_i)_{i ∈ I} sinh không gian vectơ L Ω_K(L).

c) Để (x_i)_{i ∈ I} là một p-cơ sở của L trên K, điều kiện cần và đủ là họ (dx_i)_{i ∈ I} là một cơ sở của không gian vectơ L Ω_K(L).

Trước hết, hãy nhận xét rằng vi phân dx của một phần tử của trường K((x_i)_{i ∈ I}) là một tổ hợp tuyến tính với các hệ số trong L của các vi phân dx_i, i ∈ I. Để họ (x_i)_{i ∈ I} là p-tự do, điều kiện cần và đủ là x_i ∉ K(x_j)_{j ∈ I - {i}} với mọi i ∈ I (V, p. 99, Mệnh đề 2). Theo Hệ quả 2 của Mệnh đề 5, điều này có nghĩa là dx_i không phải là một tổ hợp tuyến tính của các dx_j với j ≠ i trong I. Mệnh đề a) suy ra từ đó. Bây giờ mệnh đề b) suy ra ngay từ Hệ quả 2 của Mệnh đề 5 và mệnh đề c) suy ra từ a) và b).

Hệ quả sau đây làm cho Hệ quả 1 của Mệnh đề 5 cụ thể hơn:

#### Hệ quả {#alg-v-s13-n2-cor-1 .statement}

—Cho (x_i)_{i ∈ I} là một p-cơ sở của L trên K. Cho V là một không gian vectơ trên L, A một đạo hàm của K vào V triệt tiêu trên L^p và (u_i)_{i ∈ I} là một họ các phần tử của V. Khi đó tồn tại duy nhất một đạo hàm D của L vào V mở rộng A và ánh xạ x_i thành u_i với mọi i ∈ I.

Theo Hệ quả 1 của Mệnh đề 5, tồn tại một đạo hàm D_0 từ L vào V mở rộng A. Các đạo hàm từ L vào V mở rộng A chính xác là các ánh xạ có dạng D = D_0 + u ∘ d_{L/K} trong đó u là một ánh xạ L-tuyến tính từ Ω_K(L) vào V. Ta có D(x_i) = u_i khi và chỉ khi ánh xạ tuyến tính u thỏa các điều kiện u(dx_i) = u_i − D_0(x_i). Vì họ dx_i là một cơ sở của Ω_K(L), điều này xác định u một cách duy nhất, và hệ quả được chứng minh.

Cho L là một mở rộng căn p có chiều cao $ \leq 1 $ của K và $ (x_i)_{i \in I} $ là một cơ sở p của L trên K. Theo Hệ quả của Định lý 1, với mỗi $ i \in I $ tồn tại một đạo hàm K $ D_i $ của L vào L được đặc trưng bởi $ D_i(x_j) = \delta_{ij} $ (ký hiệu Kronecker); $ D_i $ đôi khi được gọi là *đạo hàm riêng theo* $ x_i $. Khi $ I $ là *hữu hạn*, họ $ (D_i)_{i \in I} $ là một cơ sở của không gian vectơ trên L gồm các đạo hàm K của L vào L.

Định lý 1 cho phép quy việc nghiên cứu các cơ sở p về việc nghiên cứu các cơ sở của một không gian vectơ. Ví dụ ta có kết quả sau đây:

#### Định lý 2 {#alg-v-s13-thm-2 .statement}

— *Cho L là một mở rộng căn p có chiều cao $ \leq 1 $ của một trường K.*
  *a)* *Tồn tại các cơ sở p của L trên K. Chính xác hơn, nếu S là một tập con p-tự do của L trên K và T là một tập con của L sao cho $ S \subset T $ và $ L = K(T) $, thì tồn tại một cơ sở p B của L trên K sao cho $ S \subset B \subset T $.*
  *b)* *Hai cơ sở p của L trên K có cùng lực lượng.*
  *c)* *Để $[L:K]$ là hữu hạn, điều kiện cần và đủ là không gian vectơ $ \Omega_K(L) $ trên L có số chiều hữu hạn trên L, và khi đó ta có*

$$
[L : K] = p^{[\Omega_K(L) : L]}
$$

Các khẳng định *a)* và *b)* là ngay lập tức (II, p. 292). Nếu $[L : K]$ hữu hạn, theo *a)* tồn tại một p-cơ sở hữu hạn $ (x_1, ..., x_n) $ của $ L $ trên $ K $; khi đó các đơn thức $ x_1^{\alpha_1} ... x_n^{\alpha_n} $ với $ 0 \leq \alpha_i < p $ đối với $ 1 \leq i \leq n $ tạo thành một cơ sở của $ L $ trên $ K $ và các vi phân $ dx_1, ..., dx_n $ tạo thành một cơ sở của $ \Omega_K(L) $ trên $ L $. Do đó ta có $[L : K] = p^n$ và $[\Omega_K(L) : L] = n$. Ngược lại, nếu $ \Omega_K(L) $ có số chiều hữu hạn trên $ L $, thì tồn tại một p-cơ sở hữu hạn của L trên K (V, p. 102, Đl. 1) và $[L : K]$ là hữu hạn.

#### Hệ quả {#alg-v-s13-n2-cor-2 .statement}

— *Với mỗi $ x \in L - K $, tồn tại một cơ sở p của L trên K chứa X.*

Vì $ \{x\} $ là một tập con p-tự do của $ L $ trên $ K $ nên chỉ cần áp dụng Định lý 2, *a)*.

Cho K là một trường và $ L $ là một mở rộng của K. Nếu $ D $ là một K-đạo hàm của L nhận giá trị trong một không gian vectơ L, thì ta có $ D(x^p) = 0 $ với mọi $ x \in L $, và do đó $ D $ là một $ K(L^p) $-đạo hàm; suy ra $ \Omega_K(L) = \Omega_{K(L^p)}(L) $. Vì $ L $ là một mở rộng p-căn có chiều cao $ \leq 1 $ của $ K(L^p) $, ta có thể áp dụng các kết quả ở trên. Chẳng hạn, từ Định lý 1, *c)* ta suy ra điều sau: cho $ (x_i)_{i \in I} $ là một họ các phần tử của $ L $; để $ (dx_i)_{i \in I} $ là một cơ sở của không gian vectơ L $ \Omega_K(L) $ thì điều kiện cần và đủ là $ (x_i)_{i \in I} $ là một p-cơ sở của L trên $ K(L^p) $. Tương tự, Hệ quả 2 của Mệnh đề 5 cho ta:

#### Mệnh đề 6 {#alg-v-s13-prop-6 .statement}

— *Cho K là một trường (có đặc số p) và L là một mở rộng của K.*
  *a)* *Cho $ x \in L $; vi phân $ d_{L/K}x $ triệt tiêu khi và chỉ khi x thuộc $ K(L^p) $.*
  *b)* $ \Omega_K(L) = 0 $ khi và chỉ khi $ L = K(L^p) $.*
  *c)* *Giả sử rằng L là p-căn hữu hạn cấp trên K; khi đó $ \Omega_K(L) = 0 $ khi và chỉ khi $ L = K $.*

### 3. Sự tương ứng giữa các trường con và các đại số Lie các phép dẫn xuất

Ta ký hiệu bởi E một trường và bởi g tập hợp tất cả các phép dẫn xuất của E vào chính nó. Nhắc lại rằng g là một không gian vectơ trên E, với các phép toán được xác định bởi

$$(D + D')(x) = D(x) + D'(x), \quad (aD)(x) = a \cdot D(x)$$

với $D, D'$ trong $g$ và $a, x$ trong $E$. Hơn nữa, nếu $D$ và $D'$ là các phép dẫn xuất của E vào E, thì $[D, D'] = DD' - D'D$ cũng vậy (III, p. 554). Cuối cùng, công thức Leibniz (III, p. 556) cho

$$D^p(xy) = x \cdot D^p(y) + \sum_{j=1}^{p-1} \binom{p}{j} D^j(x) D^{p-j}(y) + D^p(x) \cdot y$$

($x, y$ trong $E$); vì các hệ số nhị thức $\binom{p}{j}$ với $1 \leq j \leq p-1$ đều chia được cho $p$ ($V$, p. 4, Bổ đề 1), ta thấy rằng $D^p$ là một đạo hàm của E vào E. Ta ngay lập tức tìm được quan hệ (với $a, a' \in E$)

$$[aD, a'D'] = aa' \cdot [D, D'] + (aD(a')) \cdot D' - (a'D'(a)) \cdot D.$$

Đặc biệt, ánh xạ $(D, D') \mapsto [D, D']$ từ $g \times g$ vào $g$ là $E^p$-tuyến tính.

Ta ký hiệu bởi $\mathcal{C}$ tập hợp các trường con $K$ của $E$ sao cho $E^p \subset K$ và $[E : K]$ là hữu hạn; với mỗi $K \in \mathcal{C}$ ta ký hiệu bởi $g(K)$ tập hợp các K-đạo hàm của E. Hơn nữa, ta ký hiệu bởi $\mathcal{L}$ tập hợp các không gian con vectơ $l$ của $g$ có số chiều hữu hạn trên E và sao cho $[D, D'] \in h$ và $D^p \in h$ với mọi $D, D'$ trong $h$; với mỗi $h \in \mathcal{L}$ ta ký hiệu bởi $I(h)$ tập hợp các $x \in E$ sao cho $D(x) = 0$ với mọi $D \in h$.

#### Định lý 3 (Jacobson) {#alg-v-s13-thm-3 .statement}

— *Các ánh xạ $K \mapsto g(K)$ và $l \mapsto I(h)$ lần lượt là các song ánh của $\mathcal{C}$ lên $\mathcal{L}$ và của $\mathcal{L}$ lên $\mathcal{C}$, nghịch đảo của nhau. Nếu $K \in \mathcal{C}$ và $h \in \mathcal{L}$ tương ứng với nhau, thì $[E : K] = p^{[h : E]}$*.

Chứng minh cần đến một số bổ đề sơ bộ.

#### Bổ đề 1 {#alg-v-s13-lem-1 .statement}

— *Cho L là một trường, V là một không gian vectơ trên L và u là một tự đồng cấu của V sao cho $u^p = u$. Với mỗi $i \in \mathbf{F}_p$, gọi $V_i$ là hạt nhân của $u - i$. Khi đó ta có*

$$\mathbf{V} = \bigoplus_{i \in \mathbf{F}_p} V_i.$$

Với mỗi $i \in \mathbf{F}_p$, ký hiệu $P_i(X)$ là đa thức $- \prod_{j \neq i} (X - j)$. Ta có

$$(X - i) P_i(X) = X - X^p$$

theo Công thức (2) ($V$, p. 94). Lấy đạo hàm công thức (2) đã trích dẫn, ta được

$$\sum_{i \in \mathbf{F}_p} P_i(X) = 1$$

Các công thức (8) và (9) cho thấy rằng tự đồng cấu $ P_i(u) $ của $ V $ ánh xạ $ V $ vào $ V_i $ và rằng $ \sum_{i \in \mathbf{F}_p} P_i(u) = 1 $, do đó $ V = \sum_{i \in \mathbf{F}_p} V_i $. Còn phải chỉ ra rằng tổng này là trực tiếp. Với mỗi $ i \in \mathbf{F}_p $ lấy $ v_i \in V_i $; hiển nhiên là $ P_i(u) $ triệt tiêu $ v_j $ với mọi $ j \neq i $ và ta có $ P(u)v_i = av_i $ với $ a = -\prod_{n \in \mathbf{F}_p^*} n \neq 0 $. Quan hệ $ \sum_{i \in \mathbf{F}_p} v_i = 0 $ vì thế suy ra $ v_i = 0 $ với mọi $ i \in \mathbf{F}_p $, và do đó tổng là trực tiếp.

#### Bổ đề 2 {#alg-v-s13-lem-2 .statement}

*Cho D là một đạo hàm của E sao cho $ D^p = D $ và gọi K là hạt nhân của D. Giả sử rằng tồn tại một phần tử x khác không trong E sao cho $ D(x) = x $. Khi đó K là một trường con của E chứa $ E^p $ và ta có $ [E : K] = p $.*

Rõ ràng K là một trường con của E chứa $ E^p $. Ký hiệu $ K_i $ là hạt nhân của $ D - i $ với $ i \in \mathbf{F}_p $. Ta có $ K_0 = K $ và Bổ đề 1 cho thấy rằng $ E = \bigoplus_{i \in \mathbf{F}_p} K_i $. Cho $ i \in \mathbf{F}_p $ và cho $ u $ thuộc $ K_i $; ta có
$$
D(xu) = D(x) \cdot u + x \cdot D(u) = xu + x(iu) = (i + 1)xu
$$
do đó $ xu \in K_{i+1} $. Vì x khác không, phép nhân với x là một tự đẳng cấu của không gian vectơ K E, ánh xạ $ K_i $ lên $ K_{i+1} $ với mọi $ i \in \mathbf{F}_p $. Vì $ [K_0 : K] = 1 $, ta có $ [K_i : K] = 1 $ với mọi $ i \in \mathbf{F}_p $ do đó $ [E : K] = p $.

#### Bổ đề 3 {#alg-v-s13-lem-3 .statement}

*Cho $ \mathfrak{h} \in \mathcal{L} $ có chiều s trên E. Khi đó $ I(\mathfrak{h}) $ thuộc $ \mathcal{C} $ và ta có $ [E : I(\mathfrak{h})] = p^s $.*

Hiển nhiên $ I(\mathfrak{h}) $ là một trường con của $ E $ chứa $ E^p $. Với mỗi $ x \in E $, gọi $ f_x $ là dạng tuyến tính E trên I) xác định bởi $ D \mapsto D(x) $. Vì giao của các hạt nhân của các dạng tuyến tính này bằng 0, chúng sinh không gian đối ngẫu với $ \mathfrak{h} $ (II, p. 301, Định lý 7); do đó tồn tại các phần tử $ x_1, \ldots, x_s $ của $ E $ sao cho các dạng tuyến tính $ f_{x_1}, \ldots, f_{x_s} $ lập thành một cơ sở của không gian đối ngẫu này. Gọi $ (A,, \ldots, A,) $ là cơ sở của $ \mathfrak{h} $ được đặc trưng bởi các hệ thức $ \Delta_i(x_j) = f_{x_j}(\Delta_i) = \delta_{ij} $. Đặt $ D_i = x_i \Delta_i $, khi đó $ (D_1, \ldots, D_s) $ là một cơ sở của I) trên E và ta có $ D_i(x_j) = x_i \delta_{ij} $. Các phép đạo hàm $ D_i^p - D_i $ và $ [D_i, D_j] $ với $ i, j = 1, \ldots, s $ thuộc I) và triệt tiêu $ x_1, \ldots, x_s $; do đó ta có
$$
D_i^p = D_i , \quad [D_i, D_j] = 0
$$
Với i từ 0 đến s, gọi $ K_i $ là giao của các hạt nhân của các phép đạo hàm $ D_j $ với $ 1 \leq j \leq i $. Khi đó $ K_i $ là một trường con của E và ta có
$$
E = K_0 \supset K_1 \supset \ldots \supset K_{s-1} \supset K_s = I(\mathfrak{h}) .
$$
Cho i nằm giữa 0 và $ s-1 $; khi đó $ K_i $ ổn định dưới tác dụng của $ D_{i+1} $ vì $ D_{i+1} $ giao hoán với $ D_1, \ldots, D_i $. Hơn nữa ta có $ D_{i+1}^p = D_{i+1} $, $ D_{i+1}(x_{i+1}) = x_{i+1} \neq 0 $ và $ x_{i+1} \in K_i $. Vì thế Bổ đề 1 suy ra rằng $ [K_i : K_{i+1}] = p $, do đó cuối cùng $ [E : K] = [K_0 : K_s] = p^s $.

Bây giờ ta đi đến chứng minh định lý. Cho I) $ \in \mathcal{L} $ có chiều s trên E và đặt $ K = I(\mathfrak{h}) $; khi đó $ [E : K] = p^s $ theo Bổ đề 3, do đó $ [\Omega_K(E) : E] = s $ theo

ĐL. 2, c) (V, p. 103). Theo tính chất phổ quát của môđun vi phân, ánh xạ $ u \mapsto u \circ d_{E/K} $ là một đẳng cấu từ đối ngẫu của $ \Omega_K(E) $ lên $ g(K) $, nên $[g(K):E] = s$. Bây giờ ta có $[\mathfrak{h}:E] = s$ và $ \mathfrak{h} \subset g(K) $, do đó $ \mathfrak{h} = g(K) $, tức là $ \mathfrak{h} = g(I(\mathfrak{h})) $.

Ngược lại, với mọi trường $ K \in \mathcal{C} $ thì hiển nhiên $ g(K) $ thuộc $ \mathcal{L} $ (V, p. 103, Th. 2, c)). *Nếu* $ x $ thuộc $ I(g(K)) $, thì ta có $ u(d_{E/K}x) = 0 $ với mọi dạng tuyến tính $ u $ trên $ \Omega_K(E) $, do đó $ d_{E/K}x = 0 $ và sau cùng $ x \in K $ theo Hệ quả 2 của Mệnh đề 5 (V, p. 102). Vậy ta có $ K = I(g(K)) $.

#### Nhận xét {#alg-v-s13-n3-rem-1 .statement}

— 1) Các song ánh nghịch đảo lẫn nhau $ K \mapsto g(K) $ và $ \mathfrak{h} \mapsto I(\mathfrak{h}) $ làm đảo quan hệ bao hàm; do đó $ \mathfrak{h} \mapsto I(\mathfrak{h}) $ là một đẳng cấu từ tập hợp có thứ tự $ \mathcal{L} $ lên tập hợp có thứ tự đối của $ \mathcal{C} $. Vì thế ta thu được quan hệ $ I(\mathfrak{h} \cap \mathfrak{h}') = E^p(I(\mathfrak{h}), I(\mathfrak{h}')) $ với $ \mathfrak{h}, \mathfrak{h}' $ trong $ \mathcal{L} $, bởi vì $ \mathfrak{h} \cap \mathfrak{h}' $ là phần tử lớn nhất của $ \mathcal{L} $ được chứa đồng thời trong $ \mathfrak{h} $ và trong $ \mathfrak{h}' $.

2) Có thể chỉ ra rằng mọi không gian con có số chiều hữu hạn của $ g $ ổn định đối với ánh xạ $ D \mapsto D^p $ cũng ổn định đối với phép toán ngoặc.

### Bài tập {#alg-v-s13-exercises}

Xem [bài tập cho § 13](exercises/s13/).
