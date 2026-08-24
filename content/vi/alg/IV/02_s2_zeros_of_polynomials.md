---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 2
section_title: Zeros of polynomials
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.14-A IV.19, A IV.87-A IV.88
pdf_pages: 0023-0028, 0096-0097
extraction: ocr
subsections:
    - "no": 1
      title: Roots of a polynomial in one indeterminate. Multiplicity
      page: 14
      pdf_page: 23
    - "no": 2
      title: Differential criterion for the multiplicity of a root
      page: 17
      pdf_page: 26
    - "no": 3
      title: Polynomial functions on an infinite integral domain
      page: 17
      pdf_page: 26
statements: 19
exercises: 5
content_sha256: b0d5f66a1220ec67ec82120406d3b7558532475e835544f6757469622c91349a
translated_from: content/en/alg/IV/02_s2_zeros_of_polynomials.md
source_content_sha256: 8d0335eecb42b2e149eb6aac4d5d9373decfe3986e5c6770a233303e929f0f7f
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-d00ab518
glossary_version: 34
glossary_terms_sha256: 37f4db831b1d3735eebc06a4e8d6115867d591372884726c453b2737ca1ef1cc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC NGHIỆM KHÔNG CỦA ĐA THỨC

### 1. Nghiệm của một đa thức theo một ẩn. Bội số

Cho $g \in A[(X_i)_{i \in I}]$ và cho $E$ là một $A$-đại số kết hợp có đơn vị. Cho $x = (x_i)_{i \in I}$ là một họ các phần tử từng đôi một giao hoán của $E$. Ta sẽ nói rằng $x$ là một nghiệm không của $g$ trong $E^l$ nếu $g(x) = 0$. Nếu $f$ là một đa thức theo một ẩn duy nhất, thì một nghiệm không của $f$ trong $E$ cũng được gọi là một nghiệm của $f$ trong $E$.

#### Mệnh đề 1 {#alg-iv-s2-prop-1 .statement}

— Cho $f \in A[X]$ và $\alpha \in A$. Số dư của phép chia $f$ cho $X - \alpha$ là $f(\alpha)$. Để $\alpha$ là một nghiệm của $f$ thì điều kiện cần và đủ là $X - \alpha$ là một ước của $f$ trong $A[X]$.

Thật vậy, nếu $ u,\ v \in \mathbf{A}[X] $ sao cho $ f = (X - \alpha)\ u + v,\ \deg v < 1 $, thì $ v $ là một vô hướng và $ f(a) = (a - a)\ u(\alpha) + v = v $. Điều này chứng minh mệnh đề thứ nhất, và mệnh đề thứ hai suy ra từ đó.

#### Mệnh đề 2 {#alg-iv-s2-prop-2 .statement}

— *Cho $ f \in \mathbf{A}[X] $, $ a \in \mathbf{A} $, và cho $ h $ là một số nguyên $ \geq 0 $. Các điều kiện sau là tương đương*:
(i) $ f $ chia hết cho $ (X - \alpha)^h $ nhưng không chia hết cho $ (X - \alpha)^{h-1} $;
(ii) *tồn tại $ g \in \mathbf{A}[X] $ sao cho $ f = (X - \alpha)^h g $ và $ g(a) \neq 0 $.
(i) $ \Rightarrow $ (ii) suy ra ngay từ Mệnh đề 1.
(ii) $ \Rightarrow $ (i) : Giả sử rằng $ f = (X - \alpha)^h g $, trong đó $ g $ không nhận $ a $ làm nghiệm. Khi đó $ f $ chia hết cho $ (X - \alpha)^h $; nếu tồn tại $ g_1 \in \mathbf{A}[X] $ sao cho $ f = (X - \alpha)^{h+1} g_1 $, thì vì $ (X - \alpha)^n $ không phải là ước của không trong $ \mathbf{A}[X] $ (IV, p. 9, Mệnh đề 7), ta có $ g = (X - a)\ g_1 $ và do đó $ g(\alpha) = 0 $, điều này là vô lý.

#### Mệnh đề 3 {#alg-iv-s2-prop-3 .statement}

— *Cho $ f $ là một phần tử khác không của $ \mathbf{A}[X] $ và $ a \in \mathbf{A} $. Tồn tại duy nhất một số nguyên $ h \geq 0 $ thỏa mãn các điều kiện (i) và (ii) của Mệnh đề 2.*
Điều này hiển nhiên đối với điều kiện (i), lưu ý rằng nếu f chia được cho $ (X - \alpha)^h $, thì $ \deg f \geq h $ (IV, p. 9, Mệnh đề 7).

#### Định nghĩa 1 {#alg-iv-s2-def-1 .statement}

— *Với ký hiệu trên, ta nói rằng $ a $ có cấp $ h $, hay bội số $ h $ đối với $ f $.*
Nếu $ h > 0 $ ta cũng nói rằng $ a $ là một nghiệm cấp $ h $ hay bội số $ h $ của f. Một nghiệm cấp 1 được gọi là một nghiệm đơn, một nghiệm cấp 2 là một nghiệm kép,... Một nghiệm có cấp $ > 1 $ được gọi là bội.

#### Nhận xét 1 {#alg-iv-s2-n1-rem-1 .statement}

Nếu $ f = 0 $ ta quy ước nói rằng $ a $ có cấp $ \geq h $ đối với $ f $, với mọi $ a \in \mathbf{A} $ và số nguyên $ h \geq 0 $. Với mọi $ f \in \mathbf{A}[X] $ và $ a \in \mathbf{A} $, nói rằng $ a $ có cấp $ \geq h $ đối với $ f $ có nghĩa là $ (X - \alpha)^h $ chia hết $ f $.
2) Cho $ B $ là một vành giao hoán chứa $ \mathbf{A} $ như vành con. Cho $ f \in \mathbf{A}[X] $ là khác không và $ a \in \mathbf{A} $. Cấp của $ a $ đối với $ f $ là như nhau, dù ta xét $ f $ như một phần tử của $ B[X] $ hay như một phần tử của $ \mathbf{A}[X] $. Điều này hiển nhiên từ điều kiện (ii) của Mệnh đề 2.

#### Mệnh đề 4 {#alg-iv-s2-prop-4 .statement}

— *Cho $ f $ và $ g $ là các phần tử khác không của $ \mathbf{A}[X] $. Cho $ a \in \mathbf{A} $, và gọi các bậc của $ a $ đối với $ f $ và $ g $ lần lượt là $ p $ và $ q $.*
(i) *Bậc của $ a $ đối với $ f + g $ là $ \geq \inf(p, q) $. Nó bằng $ \inf(p, q) $ nếu $ p \neq q $*.
(ii) *Bậc của $ a $ đối với $ fg $ là $ \geq p + q $. Nó bằng $ p + q $ nếu $ \mathbf{A} $ là một miền nguyên*.

Vì ta có $ f(X) = (X - \alpha)^p f_1(X) $, $ g(X) = (X - \alpha)^q g_1(X) $ với $ f_1(\alpha) \neq 0 $, $ g_1(a) \neq 0 $. Chẳng hạn giả sử rằng $ p \leq q $; khi đó ta có
$$
f(X) + g(X) = (X - \alpha)^p (f_1(X) + (X - \alpha)^{q-p} g_1(X)) .
$$

và nếu $ p < q $, $ a $ không là nghiệm của $ f_1(X) + (X - \alpha)^{q-p} g_1(X) $; điều này chứng minh (i). Mặt khác, ta có $ f(X)g(X) = (X - \alpha)^{p+q} f_1(X)g_1(X) $ và $ f_1(\alpha)g_1(\alpha) \neq 0 $ nếu $ A $ là một miền nguyên; điều này chứng minh (ii).

#### Mệnh đề 5 {#alg-iv-s2-prop-5 .statement}

*Giả sử rằng $ A $ là một miền nguyên. Cho $ f $ là một phần tử khác không của $ A[X] $, và $ a,, \ldots, \alpha_p $ là các nghiệm phân biệt từng đôi một của $ f $ trong $ A $, có các cấp $ k_1, \ldots, k_r $. Ta có*

$$
f(X) = (X - \alpha_1)^{k_1}(X - \alpha_2)^{k_2} \ldots (X - \alpha_p)^{k_p} g(X)
$$

*trong đó $ g \in A[X] $ và $ a,, \ldots, a, $ không phải là các nghiệm của $ g $.*

Ta tiến hành bằng quy nạp theo $ p $, mệnh đề là hiển nhiên đối với $ p = 1 $, theo Định nghĩa 1. Khi đó giả sử rằng $ f(X) = g_1(X)g_2(X) $, trong đó

$$
g_1(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_{p-1})^{k_{p-1}}, \quad g_2(X) \in A[X].
$$

Vì $ A $ là một miền nguyên và $ \alpha_p $ phân biệt với $ a,, \ldots, \alpha_{p-1} $ nên $ \alpha_p $ không phải là một nghiệm của $ g_1(X) $, do đó $ \alpha_p $ là một nghiệm cấp $ k_p $ của $ g_2(X) $ (Mệnh đề 4, (ii)). Suy ra $ g_2(X) $ chia được cho $ (X - \alpha_p)^{k_p} $, và vì thế

$$
f(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_p)^{k_p} g(X)
$$

trong đó $ g(X) \in A[X] $. Rõ ràng $ a,, \ldots, \alpha_p $ không phải là các nghiệm của $ g $.

#### Định lý 1 {#alg-iv-s2-thm-1 .statement}

*Cho $ A $ là một miền nguyên. Với một phần tử khác không $ f $ của $ A[X] $, bậc $ n $, thì tổng các cấp của mọi nghiệm của nó trong $ A $ là $ \leq n $.*

Điều này suy ra ngay lập tức từ Mệnh đề 5.

#### Hệ quả {#alg-iv-s2-n1-cor-1 .statement}

*Giả sử $ A $ là một miền nguyên và cho $ f, g \in A[X] $, bậc $ \leq n $. Nếu tồn tại $ n + 1 $ phần tử $ x_1, \ldots, x_{n+1} $ của $ A $ từng đôi một phân biệt sao cho $ f(x_i) = g(x_i) $ với $ 1 \leq i \leq n + 1 $, thì $ f = g $.*

Chỉ cần áp dụng Đl. 1 cho $ f - g $.

#### Mệnh đề 6 (công thức nội suy Lagrange) {#alg-iv-s2-prop-6 .statement}

— *Cho $ K $ là một trường giao hoán, $ \alpha_1, \alpha_2, \ldots, a, $ là các phần tử phân biệt của $ K $ và $ \beta_1, \beta_2, \ldots, \beta_n $ là các phần tử bất kỳ của $ K $. Với $ i = 1, 2, \ldots, n $ ta đặt*

$$
f_i(X) = \prod_{j \in U(i)} (X - \alpha_j)/(\alpha_i - \alpha_j),
$$

*trong đó $ U(i) $ là tập hợp các số nguyên $ j $ sao cho $ j \neq i $ và $ 1 \leq j \leq n $. Khi đó $ \beta_1 f_1 + \ldots + \beta_n f_n $ là phần tử duy nhất $ f $ của $ K[X] $ sao cho $ \deg f < n $ và $ f(\alpha_i) = \beta_i $ với $ 1 \leq i \leq n $.*

Tính duy nhất của f suy ra từ Hệ quả của Định lý 1. Cho $ f = \beta_1 f_1 + \ldots + \beta_n f_n $, khi đó vì $ f_i $ có bậc $ n - 1 $, ta có $ \deg f < n $. Mặt khác, $ f_i(\alpha_j) = 0 $ với $ j \neq i $ và $ f_i(\alpha_i) = 1 $, do đó $ f(\alpha_i) = \beta_i $ với $ 1 \leq i \leq n $.

#### Hệ quả {#alg-iv-s2-n1-cor-2 .statement}

— Giả sử rằng $ \mathbf{A} $ là một miền nguyên. Cho $ f \in \mathbf{A}[X] $, có bậc $ < n $, và cho $ K $ là một vành con của $ \mathbf{A} $ đồng thời là một trường. Nếu tồn tại $ n $ phần tử phân biệt $ \alpha_1, \ldots, a_n $ của $ \mathbf{A} $ sao cho $ \alpha_i \in K $ và $ f(\alpha_i) \in K $ với $ i = 1, \ldots, n $, thì $ f \in K[X] $.

### 2. Tiêu chuẩn vi phân cho bội số của một nghiệm

#### Mệnh đề 7 {#alg-iv-s2-prop-7 .statement}

— Cho $ f \in \mathbf{A}[X] $ và cho $ a \in \mathbf{A} $ là một nghiệm của f: Để $ a $ là một nghiệm đơn của f thì điều kiện cần và đủ là $ a $ không là một nghiệm của đạo hàm $ Df $ của $ f $.

Theo giả thiết ta có $ f = (X - a)\ g $, với $ g \in \mathbf{A}[X] $. Để $ a $ là một nghiệm đơn của $ f $ thì điều kiện cần và đủ là $ g(\alpha) \neq 0 $. Bây giờ ta có $ Df = g + (X - \alpha)\ Dg $, do đó $ (Df)(\alpha) = g(\alpha) $.

Nói chung hơn:

#### Mệnh đề 8 {#alg-iv-s2-prop-8 .statement}

— Cho $ f \in \mathbf{A}[X] $ và $ a \in \mathbf{A} $, và giả sử rằng $ a $ có cấp $ k \geq 1 $ đối với $ f $: Khi đó $ a $ có cấp $ \geq k - 1 $ đối với $ Df $. Nếu $ k . 1 $ giản ước được trong $ \mathbf{A} $, thì $ a $ có cấp $ k - 1 $ đối với $ Df $.

Theo giả thiết, tồn tại $ g \in \mathbf{A}[X] $ sao cho $ f = (X - a)^k g $ và $ g(a) \neq 0 $. Do đó $ Df = k(X - \alpha)^{k-1}g + (X - \alpha)^k Dg = (X - \alpha)^{k-1}(kg + (X - \alpha)\ Dg) $, điều này thiết lập phần thứ nhất của mệnh đề. Giá trị của $ kg + (X - \alpha)\ Dg $ tại $ X = \alpha $ là $ kg(a) $, và giá trị này khác không nếu $ k . 1 $ là giản ước được trong $ \mathbf{A} $; điều này chứng minh phần thứ hai của mệnh đề.

Cho $ k $ là một số nguyên $ > 0 $ sao cho $ k . 1 = 0 $ trong $ \mathbf{A} $. Nếu $ f(X) = X^k $, thì $ 0 $ là một nghiệm cấp $ k $ của $ f $, và là một nghiệm có cấp lớn tùy ý của $ Df $.

#### Hệ quả {#alg-iv-s2-n2-cor-1 .statement}

— Cho $ f \in \mathbf{A}[X] $, $ a \in \mathbf{A} $ và $ p $ là một số nguyên $ \geq 0 $; hơn nữa, giả sử rằng $ p! . 1 $ là giản ước được trong $ \mathbf{A} $. Khi đó, để $ a $ là một nghiệm cấp $ p $ của $ f $, điều kiện cần và đủ là $ a $ là một nghiệm của $ f, Df, ..., D^{p-1}f $ và không là một nghiệm của $ D^pf $.

Điều này suy ra từ Mệnh đề 8 bằng quy nạp theo $ p $.

### 3. Hàm đa thức trên một miền nguyên vô hạn

#### Mệnh đề 9 {#alg-iv-s2-prop-9 .statement}

— Giả sử rằng $ A $ là một miền nguyên. Cho $ I $ là một tập hợp, $ (\mathbf{H}_i)_{i \in I} $ là một họ các tập con vô hạn của $ \mathbf{A} $ và $ H = \prod_{i \in I} \mathbf{H}_i \subset A' $. Nếu f là một phần tử khác không của $ \mathbf{A}[(X_i)_{i \in I}] $, và $ H_f $ là tập hợp mọi $ x \in H $ sao cho $ f(x) \neq 0 $, thì $ H $ và $ H_f $ có cùng lực lượng.

a) Trước hết giả sử rằng $ I $ là hữu hạn và đặt $ n = \mathrm{Card}\ I $. Mệnh đề là hiển nhiên với $ n = 0 $; ta sẽ chứng minh nó bằng quy nạp theo $ n $. Chọn một phần tử $ i_0 $ của $ I $ và đặt $ J = I - \{i_0\} $, $ B = \mathbf{A}[(X_i)_{i \in J}] $. Vì $ f \neq 0 $, ta có thể viết $ f = \sum_{k=0}^m g_k X_{i_0}^k $, where g_0, \ldots, g_m \in B \text{ và } g_m \neq 0. \text{ Theo giả thiết quy nạp tập hợp K của mọi } x \in \prod_{i \in s} H_i \text{ sao cho } g_m(x) \neq 0 \text{ là đẳng lực với } \prod_{i \in J} H_i. \text{ Với } x \in K \text{ đa thức}
$$
h(X_{i_0}) = \sum_{k=0}^m g_k(x) X_{i_0}^k \in A[X_{i_0}]
$$
là khác không. Theo Định lý 1 (IV, p. 16), tập hợp các $ a \in H_{i_0} $ sao cho $ h(\alpha) \neq 0 $ là đẳng lực với $ H_{i_0} $, do đó
$$
\operatorname{Card} H \geq \operatorname{Card} H_f \geq (\operatorname{Card} K) \cdot (\operatorname{Card} H_{i_0}) = \operatorname{Card} H,
$$
và vì thế $ \operatorname{Card} H = \operatorname{Card} H_f $.

b) Trong trường hợp tổng quát, tồn tại một tập con hữu hạn $ I' $ của I sao cho $ f \in A[(X_i)_{i \in I'}] $. Gọi $ H'_f $ là tập hợp mọi $ x \in \prod_{i \in I'} H_i $ sao cho $ f(x) \neq 0 $. Khi đó
$$
H_f = H'_f \times \left( \prod_{i \in I - I'} H_i \right),
$$
và chỉ cần áp dụng phần đầu của chứng minh cho $ H'_f $.

#### Hệ quả 1 {#alg-iv-s2-prop-9-cor-1 .statement}

— *Ta giữ giả thiết và ký hiệu của Mệnh đề 9. Nếu l không rỗng, thì $ H_f $ là vô hạn.*

#### Hệ quả 2 {#alg-iv-s2-prop-9-cor-2 .statement}

— *Giả sử rằng A là một miền nguyên vô hạn hoặc rằng A là một đại số trên một trường vô hạn. Với mọi $ f \in A[(X_i)_{i \in I}] $, gọi $ \tilde{f}: A^I \to A $ là hàm đa thức được xác định bởi f (IV, p. 4). Khi đó ánh xạ $ f \mapsto \tilde{f} $ là đơn ánh.*

Khi A là một miền nguyên vô hạn, hệ quả suy ra ngay từ Mệnh đề 9. Giả sử A là một đại số trên một trường vô hạn k. Gọi $ f = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v $ là một phần tử khác không của $ A[(X_i)_{i \in I}] $; khi đó tồn tại $ v_0 \in \mathbf{N}^{(I)} $ sao cho $ \alpha_{v_0} \neq 0 $, và một dạng K-tuyến tính $ \varphi $ trên A sao cho $ \varphi(\alpha_{v_0}) \neq 0 $. Gọi $ g = \sum_{v \in \mathbf{N}^{(I)}} \varphi(a_v) X^v \in k[(X_i)_{i \in I}] $; ta có $ g \neq 0 $, do đó tồn tại $ x \in k^I $ sao cho $ g(x) \neq 0 $. Khi đó $ \varphi(f(x)) = g(x) \neq 0 $, và vì thế $ f(x) \neq 0 $.

Khi A là một miền nguyên vô hạn hoặc khi A là một đại số trên một trường vô hạn, thông thường ta sẽ đồng nhất f với $ \tilde{f} $.

Giả sử A là hữu hạn và đặt $ f(X) = \prod_{a \in A} (X - a) $, khi đó $ f \neq 0 $, nhưng $ \tilde{f} = 0 $. Với các ví dụ khác, xem IV, p. 88, bài tập 7 và 8.

#### Định lý 2 (Nguyên lý mở rộng các đồng nhất thức đại số) {#alg-iv-s2-thm-2 .statement}

— *Giả sử A là một miền nguyên vô hạn. Cho $ g_1, \ldots, g_m, f $ là các phần tử của $ A[(X_i)_{i \in I}] $ và giả sử các giả thiết sau đây được thỏa mãn:*

a) $ g_1 \neq 0, \ldots, g_m \neq 0 $;
b) *với mọi* $ x \in \mathbf{A}^1 $ *sao cho* $ g_1(x) \neq 0, \ldots, g_m(x) \neq 0 $, *ta có* $ f(x) = 0 $. *Khi đó* $ f = 0 $.

Thật vậy, nếu $ f \neq 0 $, thì ta có $ fg_1 \ldots g_m \neq 0 $ (IV, p. 9, Prop. 8), do đó tồn tại $ x \in \mathbf{A}^1 $ sao cho $ f(x)g_1(x) \ldots g_m(x) \neq 0 $ (IV, p. 18, Hệ quả 2), điều này mâu thuẫn với giả thiết.

#### Chú giải {#alg-iv-s2-n3-sch-1 .statement}

— Cho A là một miền nguyên và $ f \in A[(X_i)_{i \in I}] $. Định lý 2 cung cấp một phương tiện thuận tiện để chứng minh rằng $ f = 0 $. Chỉ cần xét một miền nguyên vô hạn E chứa A như vành con; nếu ta có thể chỉ ra rằng $ f((x_i)) = 0 $ với mọi $ (x_i) \in E^I $ (hoặc thậm chí chỉ với những $ (x_i) \in E^I $ tại đó một số hữu hạn đa thức khác không đã cho không triệt tiêu) thì suy ra $ f = 0 $. Nếu chính A không vô hạn, chẳng hạn ta có thể lấy E là vành $ A[X] $ hoặc trường phân thức của nó.

Một khi đã chứng minh quan hệ $ f = 0 $, ta rõ ràng có thể suy ra rằng $ f((y_i)) = 0 $ với mọi $ (y_i) \in F^I $, trong đó F là một đại số trên A có đơn vị, kết hợp và giao hoán bất kỳ; đặc biệt F có thể hữu hạn hoặc không nguyên.

Nói cách khác, chứng minh của đồng nhất thức $ f((x_i)) = 0 $ khi các $ x_i $ chạy trong một miền nguyên vô hạn chứa A như vành con (với hạn chế có thể có là $ g_k((x_i)) \neq 0 $ đối với $ 1 \leq k \leq m $, trong đó các $ g_k $ là những đa thức khác không) kéo theo cùng đồng nhất thức đó khi các $ x_i $ chạy trong bất kỳ đại số trên A nào có đơn vị, kết hợp và giao hoán.

Đặc biệt, cho $ f \in Z[(X_i)_{i \in I}] $. Nếu $ f((x_i)) = 0 $ khi các $ x_i $ chạy trong $ \mathbf{Z} $ (với hạn chế có thể có là $ g_k((x_i)) \neq 0 $ đối với $ 1 \leq k \leq m $, trong đó các $ g_k $ là những phần tử khác không của $ \mathbf{Z}[(X_i)] $), thì ta có cùng đồng nhất thức đó khi các $ x_i $ chạy trong một vành giao hoán tùy ý.

### Bài tập {#alg-iv-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
