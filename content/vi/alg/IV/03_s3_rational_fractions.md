---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 3
section_title: Rational fractions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.19-A IV.24, A IV.89-A IV.90
pdf_pages: 0028-0033, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Definition of rational fractions
      page: 19
      pdf_page: 28
    - "no": 2
      title: Degrees
      page: 20
      pdf_page: 29
    - "no": 3
      title: Substitutions
      page: 21
      pdf_page: 30
    - "no": 4
      title: Differentials and derivations
      page: 23
      pdf_page: 32
statements: 6
exercises: 7
content_sha256: 7eb8296c3bdd43339dab986ddb6ed7030982369e56afd097238045f4f5c84d4c
translated_from: content/en/alg/IV/03_s3_rational_fractions.md
source_content_sha256: 1454c218e59fd22dd66a7d3b73222098aac8674c609849f8e3e5a2017a4c893e
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-f4318889
glossary_version: 34
glossary_terms_sha256: f73a5ae1d01c1698995b7f8178887ba5a6c8e55c8538f7abb4f950f62292be9e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. PHÂN THỨC HỮU TỈ

### 1. Định nghĩa về phân thức hữu tỉ

#### Định nghĩa 1 {#alg-iv-s3-def-1 .statement}

*Cho K là một trường giao hoán và I là một tập hợp. Trường phân thức (I, p. 116) của miền nguyên $ K[(X_i)_{i \in I}] $ được ký hiệu bởi $ K((X_i)_{i \in I}) $ hay $ K(X_i)_{i \in I} $. Các phần tử của nó được gọi là các phân thức hữu tỉ theo các ẩn $ X_i $ với hệ số trong K.*

Với $ I = \{1, 2, \ldots, n\} $ ta viết $ K(X_1, X_2, \ldots, X_n) $ thay cho $ K((X_i)_{i \in I}) $.

Cho A là một miền nguyên và K là trường phân thức của nó. Vành $ A[(X_i)_{i \in I}] $ có thể được đồng nhất với một vành con của $ K[(X_i)_{i \in I}] $, do đó cũng của $ K((X_i)_{i \in I}) $. Với mỗi $ f \in K[(X_i)_{i \in I}] $ tồn tại một phần tử khác không $ \alpha $ của A sao cho $ \alpha f \in A[(X_i)_{i \in I}] $. Do đó mọi phần tử của $ K((X_i)_{i \in I}) $ đều có thể viết dưới dạng $ u/v $ với $ u, v \in A[(X_i)_{i \in I}], v \neq 0 $. Vì thế $ K((X_i)_{i \in I}) $ có thể được đồng nhất với trường phân thức của $ A[(X_i)_{i \in I}] $.

Bây giờ cho K là một trường giao hoán, I là một tập hợp và J ⊂ I. Đặt B = K[(X_i)_{i ∈ J}], khi đó K[(X_i)_{i ∈ I}] = B[(X_i)_{i ∈ I - J}], và theo điều vừa nói, K((X_i)_{i ∈ I}) có thể được đồng nhất với K'((X_i)_{i ∈ I - J}), trong đó K' = K((X_i)_{i ∈ J}).

### 2. Bậc

Cho K là một trường giao hoán. Với mỗi phần tử r của K((X_i)_{i ∈ I}) tồn tại u, v ∈ K[(X_i)_{i ∈ I}] sao cho v ≠ 0 và r = $ \frac{u}{v} $. Quan hệ $ \frac{u}{v} = \frac{u_1}{v_1} $, trong đó v ≠ 0, v_1 ≠ 0, là tương đương với uv_1 = vu_1; nếu r ≠ 0, ta có u ≠ 0 và u_1 ≠ 0, nên deg u + deg v_1 = deg v + deg u_1 (IV, p. 9), hay cũng deg u − deg v = deg u_1 − deg v_1. Số nguyên deg u − deg v do đó chỉ phụ thuộc vào r; ta gọi nó là bậc, hay bậc toàn phần, của r, và ký hiệu nó bằng deg r. Ta quy ước viết deg 0 = −∞. Nếu J ⊂ I, ta cũng có thể định nghĩa bậc đối với các X_j với chỉ số j ∈ J. Khi r là một đa thức, các khái niệm này trùng với những khái niệm đã định nghĩa trong IV, p. 2.

#### Mệnh đề 1 {#alg-iv-s3-prop-1 .statement}

— Cho r, s là hai phân thức hữu tỉ.

(i) Nếu deg r ≠ deg s, ta có

$$
r + s \neq 0 \quad \text{and} \quad \deg(r + s) = \sup(\deg r, \deg s)
$$

Nếu deg r = deg s, ta có deg(r + s) ≤ deg r.

(ii) Ta có deg(rs) = deg r + deg s.

Ta có thể chỉ cần xét trường hợp r và s đều khác 0.

Viết r = $ \frac{u}{v} $, s = $ \frac{w}{z} $, trong đó u, v, w, z là các đa thức khác không. Ta có rs = $ \frac{uw}{vz} $, và do đó

$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z =
= \deg r + \deg s.
$$

Mặt khác, ta có r + s = $ \frac{uz + vw}{vz} $. Giả sử deg r ≠ deg s, nói cách khác deg u + deg z ≠ deg w + deg v. Khi đó uz + vw ≠ 0, và

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&= \sup(\deg(uz), \deg(vw)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s).
\end{align*}
$$

Giả sử deg r = deg s, tức là deg u + deg z = deg w + deg v. Nếu r + s ≠ 0, thì ta có

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r
\end{align*}
$$

\* Ánh xạ r ↦ −deg r do đó là một định giá rời rạc trên trường K((X_i)_{i ∈ I}). \*

### 3. Phép thế

Cho K là một trường giao hoán, E là một K-đại số kết hợp có đơn vị, $ x = (x_i)_{i \in I} $ là một họ các phần tử của E từng đôi một giao hoán. Đặt $ B = K[(X_i)_{i \in I}] $ và $ S_x $ là tập hợp tất cả các $ v \in B $ khác không sao cho $ v(x) $ khả nghịch trong E. Cho $ u \in B,\ v \in S_x $ và $ f = \frac{u}{v} \in K((X_i)_{i \in I}) $. Phần tử $ u(x)\ v(x)^{-1} = v(x)^{-1}u(x) $ được xác định trong E; hơn nữa, nếu $ u_1,\ v_1 $ là hai đa thức sao cho $ f = \frac{u_1}{v_1} $ và $ v_1 \in S_x $, thì $ uv_1 = vu_1 $, suy ra $ u(x)v_1(x) = v(x)u_1(x) $ và do đó
$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

Cho $ f \in K((X_i)_{i \in I}) $. Nếu tồn tại *ít nhất một cặp* $(u, v)$ sao cho $ f = \frac{u}{v} $ và $ v \in S_x $, ta sẽ nói rằng x *có thể thế* trong $ f $; khi đó phần tử $ u(x)\ v(x)^{-1} $ chỉ phụ thuộc vào $ f $ và $ x $ được ký hiệu bởi $ f(x) $ hay $ f((x_i)) $ hay $ f((x_i)_{i \in I}) $.

#### Mệnh đề 2 {#alg-iv-s3-prop-2 .statement}

*Cho K là một trường giao hoán, E là một đại số trên K kết hợp có đơn vị và $ x = (x_i)_{i \in I} $ là một họ các phần tử đôi một giao hoán của E. Tập hợp $ S_x^{-1}B $ gồm các $ f \in K((X_i)_{i \in I}) $ sao cho x thế được vào $ f $ là một đại số con trên K của $ K((X_i)_{i \in I}) $. Ánh xạ $ f \mapsto f(x) $ là một đồng cấu có đơn vị $ \varphi $ từ $ S_x^{-1}B $ vào E. Ảnh $ \varphi(S_x^{-1}B) $ là tập hợp tất cả các $ yz^{-1} $, trong đó y chạy qua đại số con có đơn vị $ K[x]_E $ của E được sinh bởi họ x và z chạy qua tập hợp tất cả các phần tử khả nghịch của $ K[x]_E $.

Cho $ f_1 = \frac{u_1}{v_1},\ f_2 = \frac{u_2}{v_2} $ là hai phần tử của $ K((X_i)_{i \in I}) $ sao cho $ v_1,\ v_2 \in S_x $. Ta có $ f_1 + f_2 = \frac{u_1v_2 + u_2v_1}{v_1v_2},\ f_1f_2 = \frac{u_1u_2}{v_1v_2} $ và $ v_1,\ v_2 \in S_x $. Do đó $ S_x^{-1}B $ là một đại số con trên K của $ K((X_i)_{i \in I}) $. Phần còn lại của mệnh đề là hiển nhiên.

#### Hệ quả {#alg-iv-s3-n3-cor-1 .statement}

*Cho L là một trường giao hoán, K là một trường con của L, $ x = (x_i)_{i \in I} $ là một họ các phần tử của L, M là tập gồm các $ x_i $, U là tập tất cả các $ f \in K((X_i)_{i \in I}) $ sao cho x thế được vào $ f $ và $ \varphi $ là đồng cấu $ f \mapsto f(x) $ của U vào L. Khi đó $ \varphi(U) $ là trường con của L sinh bởi $ KUM $.*

Cho L' là trường con của L được sinh bởi $ KUM $. Ta có
$$
K \cup M \subset \varphi(U) \subset L'
$$
và $ \varphi(U) $ là một vành con của L. Bây giờ Mệnh đề 2 suy ra rằng $ \varphi(U) $ là một trường con của L, do đó $ \varphi(U) = L' $.

Cho $ f \in K((X_i)_{i \in I}) $ và cho $ (g_i)_{i \in I} $ là một họ các phần tử của $ K((Y_l)_{l \in L}) $. Nếu $(g_i)_{i \in I}$ thế được vào $f$, thì $f((g_i))$ là một phần tử của $K((Y_l)_{l \in L})$. Đặc biệt, $(X_i)_{i \in I}$ thế được vào $f$ và $f = f((X_i)_{i \in I})$.

#### Mệnh đề 3 {#alg-iv-s3-prop-3 .statement}

— Cho E là một đại số trên K mà kết hợp, giao hoán, có đơn vị và khác không. Cho $ f \in K((X_i)_{i \in I}) $ và với mỗi $ i \in I $, cho $ g_i \in K((Y_l)_{l \in L}) $. Cho một họ y = $(y_l)_{l \in L}$ các phần tử của E, giả sử rằng y thế được vào từng $g_i$ và $(g_i(y))_{i \in I}$ thế được vào $f$. Khi đó:
(i) $(g_i)_{i \in I}$ thế được vào $f$;
(ii) nếu ký hiệu h là phần tử $f((g_i))$ của $K((Y_l)_{l \in L})$, thì y thế được vào h và $h(y) = f((g_i(y)))$.

Ta có thể giả sử I hữu hạn. Theo giả thiết, với mỗi $ i \in I $, $ g_i $ có thể viết dưới dạng $ p_i/q_i $ trong đó $ p_i, q_i \in K[(Y_l)_{l \in L}] $ và $ q_i(y) $ khả nghịch trong E. Tương tự, $ f $ có thể viết thành $ u/v $, trong đó $ u, v \in K[(X_i)_{i \in I}] $ và $ v((g_i(y))) $ khả nghịch. Đặt $ m = \sup(\deg u, \deg v) $, và đặt $ w = \prod_{i \in I} q_i \in K[(Y_l)_{l \in L}] $, $ u_1 = u((g_i)) w^m, v_1 = v((g_i)) w^m $. Đa thức u là một tổ hợp tuyến tính trên K của các đơn thức $\prod_{i \in I} X_i^{v_i}$ sao cho $\sum_{i \in I} v_i \leq m$. Ta có $ w^m \prod_{i \in I} g_i^{v_i} = w^m \left( \prod_{i \in I} p_i^{v_i} \right) \left( \prod_{i \in I} q_i^{v_i} \right)^{-1} \in K[(Y_l)_{l \in L}] $ theo cách chọn m. Do đó $ u_1 \in K[(Y_l)_{l \in L}] $ và tương tự $ v_1 \in K[(Y_l)_{l \in L}] $. Hơn nữa, $ v_1(y) = (w(y))^m v((g_i(y))) $ là khả nghịch. Vì thế $ v_1 \neq 0 $, vì $ E \neq 0 $, và do đó $ v((g_i)) \neq 0 $. Vậy họ $(g_i)$ thế được vào $f$. Ngoài ra ta có $ f((g_i)) = u_1/v_1 $, do đó y thế được vào $h = f((g_i))$, và $ h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y))) $.

Cho K là một trường giao hoán, E là một đại số trên K giao hoán, kết hợp và có đơn vị, và cho $ f \in K((X_i)_{i \in I}) $. Đặt $ T_f $ là tập tất cả các $ x = (x_i)_{i \in I} \in E^I $ thế được vào $ f $. Ánh xạ $ x \mapsto f(x) $ từ $ T_f $ vào E được gọi là hàm hữu tỉ gắn với f (và E); đôi khi ta ký hiệu nó bởi $ \tilde{f} $. Nếu $ g \in K((X_i)_{i \in I}) $ thì ta có $ T_f \cap T_g \subset T_{f+g}, T_f \cap T_g \subset T_{fg} $, do đó hàm hữu tỉ gắn với $ f + g $ (tương ứng $ fg $) được xác định trên $ T_f \cap T_g $ và trên tập này nhận cùng giá trị với $ \tilde{f} + \tilde{g} $ (tương ứng $ \tilde{f}\tilde{g} $). Đặt $ T'_f $ là tập các $ x \in T_f $ sao cho $ f(x) $ khả nghịch; nếu $ x \in T'_f $, thì x thế được vào $ 1/f $ và hàm hữu tỉ gắn với $ 1/f $ nhận tại x giá trị $ f(x)^{-1} $.

Nếu K là một trường giao hoán vô hạn, $ f \in K((X_i)_{i \in I}) $, $ g \in K((X_i)_{i \in I}) $ và $ \tilde{f}, \tilde{g} $ là các hàm hữu tỉ gắn với $ f, g $ (và K), và nếu $ \tilde{f}(x) = \tilde{g}(x) $ với mọi $ x \in T_f \cap T_g $ thì $ f = g $. Thật vậy, nếu $ f = u/v $ và $ g = u_1/v_1 $, trong đó u, v, $ u_1, v_1 $ là các đa thức, ta có $ u(x)v_1(x) = u_1(x)v(x) $ với mọi x sao cho $ v(x)v_1(x) \neq 0 $, suy ra $ uv_1 = u_1v $ (IV, p. 18, Định lý 2). Do đó ánh xạ $ f \mapsto \tilde{f} $ là đơn ánh và ta sẽ thường đồng nhất f và $ \tilde{f} $.

\* Dựa vào tính nhân tử hóa duy nhất của $ K[(X_i)_{i \in I}] $ (Comm. Alg., VII, § 3, No. 2 p. 502 and Hệ quả của Định lý 2 p. 506), ta dễ dàng chứng minh điều sau đây: với mọi $ f \in K((X_i)_{i \in I}) $ tồn tại $ u, v \in K[(X_i)_{i \in I}] $ sao cho:
    1) $ f = u/v $;
    2) để $ x \in K^I $ thế được vào $ f $ thì điều kiện cần và đủ là $ v(x) \neq 0. $

### 4. Vi phân và phép vi phân

Cho $ K $ là một trường giao hoán. Theo III, p. 558, Mđ. 5, mọi đạo hàm $ D $ của $ K[(X_i)_{i \in I}] $ đều mở rộng một cách duy nhất thành một đạo hàm $ \bar{D} $ của $ K((X_i)_{i \in I}) $. Nếu $ D, D' $ là các đạo hàm hoán vị được của $ K[(X_i)_{i \in I}] $, thì giao hoán tử $ [D, D'] = DD' - D'D $ bằng không, do đó $ [\bar{D}, \bar{D}'] $, là một đạo hàm của $ K((X_i)_{i \in I}) $ mở rộng $ [D, D'] $, cũng bằng không; nói cách khác, $ D $ và $ D' $ là hoán vị được. Đặc biệt, các đạo hàm $ D_i $ (IV, p. 6) mở rộng thành các đạo hàm của $ K((X_i)_{i \in I}) $, vẫn ký hiệu là $ D_i $ và từng đôi một hoán vị được. Nếu $ f \in K((X_i)_{i \in I}), D_i f $ còn được viết là $ D_{x_i} f $ hoặc $ \frac{\partial f}{\partial x_i} $ hoặc $ f'_{x_i} $. Khi chỉ có một bất định $ X $ thì dùng ký hiệu $ Df, \frac{df}{dX}, f' $.

Cho $ B = K[(X_i)_{i \in I}], C = K((X_i)_{i \in I}) $. Theo III, p. 574, Mđ. 23, ánh xạ chính tắc

$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$

là một đẳng cấu của các không gian vectơ $ C $. Theo III, p. 570, ta thấy rằng không gian vectơ $ C $ $ \Omega_K(C) $ có cơ sở là họ $ (dX_i)_{i \in I} $ các vi phân của các $ X_i $. Gọi $ \partial_i $ là dạng tọa độ có chỉ số $ i $ trên $ \Omega_K(C) $ đối với cơ sở đó. Khi đó ánh xạ $ u \mapsto (\partial_i, du) $ từ $ C $ vào chính nó là một đạo hàm của $ C $, biến $ X_i $ thành 1 và $ X_j $ thành 0 với $ j \neq i $, và do đó bằng $ D_i $; nói cách khác, ta có

$$
du = \sum_{i \in I} (D_i u) dX_i
$$

với mọi $ u \in C $. Nếu $ I $ hữu hạn, $ (D_i)_{i \in I} $ là một cơ sở của không gian vectơ $ C $ các đạo hàm của $ C $.

#### Mệnh đề 4 {#alg-iv-s3-prop-4 .statement}

— *Cho $ E $ là một $ K $-đại số kết hợp, giao hoán và có đơn vị, $ x = (x_i)_{i, I} $ là một họ các phần tử của $ E $ và $ f \in K((X_i)_{i, I}) $. Giả sử rằng $ x $ có thể thế vào $ f $ và $ y = f(x) $.
(i) Với mọi đạo hàm $ A $ của $ K((X_i)_{i, I}) $ ánh xạ $ K[(X_i)_{i, I}] $ vào chính nó, $ x $ có thể thế vào $ Af $.
(ii) Với mọi đạo hàm $ D $ của $ E $ vào một $ E $-môđun ta có

$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

Cho $ f = \frac{u}{v} $ với $ u, v \in K[(X_i)_{i \in I}] $ và $ v(x) $ khả nghịch trong E. Cho A là một đạo hàm của $ K((X_i)_{i \in I}) $ ánh xạ $ K[(X_i)_{i \in I}] $ vào chính nó. Ta có
$$
\Delta f = \frac{(\Delta u)\ v - u(\Delta v)}{v^2}
$$
và $ v^2(x) $ khả nghịch, do đó x có thể thế vào $ Af $. Thứ hai, đặt $ r = u(x) $, $ s = v(x) $; ta có $ y = s^{-1}r $, do đó với mọi đạo hàm D của E vào một E-môđun ta có
$$
\begin{align*}
Dy &= s^{-2}(s(Dr) - r(Ds)) \\
&= s^{-2}\left( s \sum_{i \in I} (D_iu)(x) \cdot Dx_i - r \sum_{i \in I} (D_iv)(x) \cdot Dx_i \right)
\end{align*}
$$
theo Mệnh đề 4 của IV, p. 6. Do đó $ Dy = \sum_{i \in I} w_i \cdot Dx_i $ với
$$
w_i = v(x)^{-2}(v(x)(D_iu)(x) - u(x)(D_iv)(x)) = (D_if)(x).
$$

### Bài tập {#alg-iv-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
