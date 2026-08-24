---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 7
section_title: Separable algebraic extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.36-A V.47, A V.151-A V.153
pdf_pages: 0150-0161, 0265-0267
extraction: ocr
subsections:
    - "no": 1
      title: Separable algebraic extensions
      page: 36
      pdf_page: 150
    - "no": 2
      title: Separable polynomials
      page: 37
      pdf_page: 151
    - "no": 3
      title: Separable algebraic elements
      page: 39
      pdf_page: 153
    - "no": 4
      title: The theorem of the primitive element
      page: 40
      pdf_page: 154
    - "no": 5
      title: Stability properties of separable algebraic extensions
      page: 41
      pdf_page: 155
    - "no": 6
      title: A separability criterion
      page: 42
      pdf_page: 156
    - "no": 7
      title: The relative separable algebraic closure
      page: 43
      pdf_page: 157
    - "no": 8
      title: The separable closure of a field
      page: 45
      pdf_page: 159
    - "no": 9
      title: Separable and inseparable degrees of an extension of finite degree
      page: 46
      pdf_page: 160
statements: 38
exercises: 5
content_sha256: b58c330177fd6569c4392844e95d41f6c614e8bf0d0df2106b74108f8760a8be
translated_from: content/en/alg/V/07_s7_separable_algebraic_extensions.md
source_content_sha256: 5aa05da3a383afbbc0ff09ac77e72873f9e34a13a6ee239fe6fd376ee0c0b6b8
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-93c80b86
glossary_version: 34
glossary_terms_sha256: cfd873d1a31f0683cb9f6ea7934bf0fe690991a8f19cbb546fb1683b75ecbacb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. MỞ RỘNG ĐẠI SỐ TÁCH ĐƯỢC

Trong suốt đoạn này $ K $ ký hiệu một trường.

### 1. Các mở rộng đại số tách được

#### Định nghĩa 1 {#alg-v-s7-def-1 .statement}

— *Cho E là một mở rộng đại số của K; khi đó E được gọi là tách được (trên K) nếu mọi mở rộng con F của E có bậc hữu hạn trên K là một đại số étale trên K* ($ V $, p. 28, Def. 1).

Cho E là một mở rộng bậc hữu hạn của K. Vì mọi đại số con của một đại số étale đều là étale ($ V $, p. 30, Prop. 3), điều đó tương đương với việc giả sử rằng E là một mở rộng tách được của $ K $, hay E là một đại số étale trên $ K $.

#### Mệnh đề 1 {#alg-v-s7-prop-1 .statement}

— *Cho E là một mở rộng đại số của K. Nếu E là tách được, thì mọi mở rộng con $ E' $ của E đều tách được. Ngược lại, nếu mọi mở rộng con bậc hữu hạn của E đều tách được thì E là tách được.*

Điều này suy ra ngay lập tức từ Định nghĩa 1.

#### Mệnh đề 2 {#alg-v-s7-prop-2 .statement}

— *Để một trường K là hoàn hảo, điều kiện cần và đủ là mọi mở rộng đại số của K đều tách được.*

Trước hết giả sử rằng K là hoàn hảo. Vì một trường là một vành rút gọn, theo Bổ đề 5 ($ V $, p. 35) suy ra rằng mọi mở rộng bậc hữu hạn của $ K $ là một đại số étale trên $ K $; do đó mọi mở rộng đại số của $ K $ đều tách được.

Bây giờ giả sử rằng $ K $ là một trường không hoàn hảo có đặc số $ p \neq 0 $. Gọi $ \Omega $ là một bao đóng đại số của $ K $. Vì $ K $ không hoàn hảo, tồn tại $ b \in K $ không thuộc $ K^p $; đặt $ a = b^{1/p} $. Khi đó mở rộng $ K(a) $ của $ K $ là p-căn và có bậc hữu hạn. Theo $ V $, p. 26, Prop. 3, tồn tại đúng một K-đồng cấu của $ K(a) $ vào $ \Omega $, và vì $ [K(a):K] > 1 $, đại số $ K(a) $ không étale trên $ K $ ($ V $, p. 32, Prop. 4). Nói cách khác, mở rộng $ K(a) $ của $ K $ có bậc hữu hạn không tách được.

#### Hệ quả {#alg-v-s7-n1-cor-1 .statement}

— *Mọi mở rộng đại số của một trường có đặc số 0, hoặc của một trường hữu hạn, đều tách được.*
    Điều này suy ra từ *V*, p. 7, Mệnh đề 5.

### 2. Đa thức tách được

#### Mệnh đề 3 {#alg-v-s7-prop-3 .statement}

— *Cho f là một đa thức khác không trong K[X] và cho Ω là một mở rộng đóng đại số của K. Các điều kiện sau là tương đương:*
    *a) Đa thức f nguyên tố cùng nhau với đạo hàm f' của nó trong K[X].*
    *b) Hoặc deg(f) = 0, hoặc deg(f) > 0 và dis(f) ≠ 0 (IV, p. 83).*
    *c) Tồn tại một mở rộng L của K sao cho f phân tích trong L[X] thành một tích các đa thức phân biệt có bậc ≤ 1.*
    *d) Các nghiệm của f trong Ω là đơn.*
    *e) Đại số trên K K[X]/(f) là etale (V, p. 28, Định nghĩa 1).*

*a) ⇒ d)*: Dưới giả thiết *a*) tồn tại hai đa thức g và h trong K[X] sao cho fg + f'h = 1 (IV, p. 12). Cho a là một nghiệm của f trong Ω; ta có
$$
f'(a)\ h(a) = f(a)\ g(a) + f'(a)\ h(a) = 1,
$$
do đó $ f'(a) \neq 0 $; vì thế $ a $ là một nghiệm đơn của f trong Ω (*IV*, p. 17, Mệnh đề 7).

*d) ⇒ c)*: Nếu *d*) đúng, f phân tích trong Ω[X] thành một tích các thừa số phân biệt có bậc ≤ 1.

*c) ⇒ b)*: Dưới giả thiết c) tồn tại một phần tử $ A \neq 0 $ trong L và các phần tử *phân biệt* $ a_1, ..., a_n $ của L sao cho $ f(X) = \lambda (X - a_1) ... (X - a_n) $. Nếu $ \deg(f) > 0 $, ta có (*IV*, p. 83, Mệnh đề 11),
$$
\operatorname{dis}(f) = \lambda^{2n-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 \neq 0.
$$

*b) ⇒ a)*: Cho c là hệ số đầu và D là biệt thức của f; kết thức của $ f' $ và f bằng ± cD (IV, p. 84, Công thức (54)), do đó khác không; vì thế (*IV*, p. 78, Hệ quả 2) các đa thức f và $ f' $ nguyên tố cùng nhau trong K[X].

*a) ⇒ e)*: Cho A là đại số trên K K[X]/(f) và x là ảnh của X trong A; theo III, p. 573, Mệnh đề 22, A-môđun $ \Omega_K(A) $ được sinh bởi các phần tử $ dx $, chịu quan hệ duy nhất $ f'(x)\ dx = 0 $. Theo *V*, p. 33, Định lý 3, do đó đại số trên K A là etale khi và chỉ khi $ f'(x) $ là một phần tử khả nghịch trong A, điều đó có nghĩa là f và $ f' $ nguyên tố cùng nhau trong K[X].

#### Định nghĩa 2 {#alg-v-s7-def-2 .statement}

— *Một đa thức $ f \in K[X] $ được gọi là tách được nếu nó khác không và thỏa mãn các điều kiện tương đương a), b), c), d) và e) của Mệnh đề 3.*

#### Nhận xét {#alg-v-s7-n2-rem-1 .statement}

— 1) Cho L là một mở rộng của K và f là một đa thức không hằng trong K[X]. Theo *e)* của Mệnh đề 3 và V, p. 32, Hệ quả 2, việc giả sử f là tách được là như nhau, dù xét như phần tử của K[X] hay của L[X]. Mặt khác, hoàn toàn có thể xảy ra trường hợp f là bất khả quy trong K[X] nhưng không bất khả quy trong L[X].

2) Cho $ f \in K[X] $; ta biết (IV, p. 13, Mệnh đề 13) rằng tồn tại các đa thức bất khả quy $ f_1, \ldots, f_m $ trong $ K[X] $ sao cho $ f = f_1 \ldots f_m $. Cho $ \Omega $ là một bao đóng đại số của $ K $; vì một đa thức bất khả quy $ g \in K[X] $ là đa thức tối tiểu trên $ K $ của mỗi nghiệm của nó trong $ \Omega $, nên hai đa thức bất khả quy phân biệt trong $ K[X] $ không có nghiệm chung nào trong $ \Omega $. Điều kiện $ d) $ của Mệnh đề 3 khi đó cho thấy rằng $ f $ là tách được khi và chỉ khi các đa thức $ f_1, \ldots, f_m $ là tách được và từng đôi một phân biệt.

#### Mệnh đề 4 {#alg-v-s7-prop-4 .statement}

— *Cho $ f $ là một đa thức bất khả quy trong $ K[X] $. Khi đó các điều kiện sau là tương đương*:

a) $ f $ tách được.
b) *Tồn tại một mở rộng $ L $ của $ K $ mà trong đó $ f $ có một nghiệm đơn.*
c) *Đạo hàm $ f' $ của f khác không.*
d) *Trường $ K $ có đặc số $ 0 $, hoặc có đặc số $ p \neq 0 $ và $ f \not\in K[X^p] $*.

Trước hết nhận thấy rằng một đa thức bất khả quy trong $ K[X] $ không phải là hằng. Hiển nhiên $ a) $ kéo theo $ b) $ (lấy một bao đóng đại số của $ K $ làm $ L $). Nếu $ x $ là một nghiệm đơn của nó trong một mở rộng $ L $ của $ K $, thì ta có $ f'(x) \neq 0 $ (IV, p. 17, Mệnh đề 7), do đó $ b) $ kéo theo $ c) $, và tính tương đương của $ c) $ và $ d) $ suy ra từ V, p. 9, Hệ quả.

Giả sử cuối cùng rằng $ f \neq 0 $; gọi $ x $ là một nghiệm của $ f $ trong một mở rộng đóng đại số $ \Omega $ của $ K $. Vì $ f $ là đa thức tối tiểu của $ x $ trên $ K $ và $ \deg f' < \deg f $, ta có $ f'(x) \neq 0 $, và do đó $ x $ là một nghiệm đơn của $ f $ (IV, p. 17, Prop. 7). Vậy $ f $ là tách được và ta đã chỉ ra rằng $ c) $ kéo theo $ a) $.

#### Hệ quả 1 {#alg-v-s7-prop-4-cor-1 .statement}

— *Để một trường $ K $ là hoàn hảo thì điều kiện cần và đủ là mọi đa thức bất khả quy của $ K[X] $ đều tách được*.

Nếu trường $ K $ có đặc số $ 0 $, thì $ K $ là hoàn hảo và mọi đa thức bất khả quy của $ K[X] $ đều tách được, theo $ d) $ ở trên. Vậy giả sử rằng $ K $ có đặc số $ p \neq 0 $.

Trước hết giả sử rằng $ K $ là hoàn hảo. Ta có $ K[X^p] = K[X]^p $, do đó không tồn tại đa thức bất khả quy nào của $ K[X] $ thuộc $ K[X^p] $. Theo Mệnh đề 4, khi đó mọi đa thức bất khả quy của $ K[X] $ đều tách được.

Bây giờ giả sử rằng $ K $ là không hoàn hảo, do đó $ K \neq K^p $. Cho $ a $ là một phần tử của $ K $ không thuộc $ K^p $; đa thức $ X^p - a $ là bất khả quy trong $ K[X] $ (V, p. 24, Bổ đề 1), và nó thuộc $ K[X^p] $, nên không tách được.

#### Hệ quả 2 {#alg-v-s7-prop-4-cor-2 .statement}

— *Để $ f \in K[X] $ là một đa thức khác không. Điều kiện cần và đủ để $ f $ tách được là tồn tại một mở rộng $ L $ của $ K $ là một trường hoàn hảo và sao cho $ f $ không có nhân tử lặp lại trong $ L[X] $*.

Cho $ \Omega $ là một bao đóng đại số của $ K $; khi và chỉ khi tách được, $ f $ không có nhân tử lặp trong $ \Omega[X] $ (Mệnh đề 3, $ d$) ). Ngược lại, nếu $ L $ là một mở rộng hoàn hảo của $ K $ sao cho $ f $ không có nhân tử lặp trong $ L[X] $, thì $ f $ tách được trong $ L[X] $ (Hệ quả 1 và Nhận xét 2), do đó cũng tách được trong $ K[X] $ (Nhận xét 1).

### 3. Các phần tử đại số tách được

#### Định nghĩa 3 {#alg-v-s7-def-3 .statement}

— Cho E là một mở rộng của K. Một phần tử x của E, đại số trên K, được gọi là tách được trên K nếu mở rộng đại số K(x) của K là tách được.

#### Mệnh đề 5 {#alg-v-s7-prop-5 .statement}

— Cho E là một mở rộng của K, x một phần tử của E đại số trên K và f là đa thức tối tiểu của x trên K. Khi đó các điều kiện sau là tương đương:
a) x tách được trên K;
b) đa thức f là tách được;
c) x là một nghiệm đơn của f.
Tính tương đương của a) và b) suy ra từ Mệnh đề 3, còn của b) và c) suy ra từ các Mệnh đề 3 và 4 (xem V, p. 37 và 38).

#### Hệ quả 1 {#alg-v-s7-prop-5-cor-1 .statement}

— Nếu một phần tử x của E là một nghiệm đơn của một đa thức g thuộc K[X], thì nó tách được trên K.
Vì đa thức tối tiểu f của x trên K chia hết g trong K[X] (V, p. 16, Định lý 1), nên x là một nghiệm đơn của f.

#### Hệ quả 2 {#alg-v-s7-prop-5-cor-2 .statement}

— Nếu một phần tử x của E là đại số và tách được trên K, thì nó đại số và tách được trên mọi mở rộng K' của K được chứa trong E.
Cho f là đa thức tối tiểu của x trên K. Khi đó x là một nghiệm đơn của f theo Mệnh đề 5, và vì f thuộc K'[X], phần tử x của E là tách được trên K' theo Hệ quả 1.

#### Hệ quả 3 {#alg-v-s7-prop-5-cor-3 .statement}

— Giả sử rằng K có đặc số $ p \neq 0 $. Để một phần tử x của E thuộc K, điều kiện cần và đủ là nó vừa đại số tách được vừa p-căn trên K.
Điều kiện đã nêu rõ ràng là cần thiết. Ngược lại, giả sử rằng x là đại số tách được trên K và p-căn cấp e trên K. Vì x tách được trên K, đa thức tối tiểu f của x trên K không thuộc K[X^p] (Mệnh đề 4 và 5); vì x là p-căn cấp e trên K, ta có $ f(X) = X^{p^e} - x^{p^e} $ (V, p. 24, Mệnh đề 1); do đó kết luận rằng $ e = 0 $, nên $ x \in K $.

#### Mệnh đề 6 {#alg-v-s7-prop-6 .statement}

— Cho E là một mở rộng của K.
a) Nếu E là đại số và tách được trên K, mọi phần tử của E đều đại số và tách được trên K.
b) Ngược lại, cho A là một tập hợp các phần tử của E, đại số và tách được trên K và sao cho $ E = K(A) $; khi đó E là đại số và tách được trên K.
Nếu E là đại số và tách được trên K, điều đó cũng đúng với mở rộng K(x) của K với mọi $ x \in E $, do đó suy ra a).
Dưới giả thiết b), mở rộng E là đại số trên K (V, p. 18, Hệ quả 1).

Cho F là một mở rộng con của E có bậc hữu hạn trên K. Theo V, p. 11, Hệ quả, tồn tại các phần tử $ x_1, \ldots, x_m $ của A sao cho $ F \subset K(x_1, \ldots, x_r) $ và ta có

$$
K(x_1, \ldots, x_m) = K[x_1, \ldots, x_m] \quad (\text{V, p. 18, Hệ quả 1}).
$$

Theo giả thiết trên A, các đại số $ K[x_1], \ldots, K[x_m] $ là étale trên K; do đó điều đó cũng đúng với $ K[x_1] \otimes \cdots \otimes K[x_m] $ (V, p. 32, Hệ quả 1). Bây giờ F đẳng cấu với một đại số con của một đại số thương của $ K[x_1] \otimes \cdots \otimes K[x_m] $, nên là étale (V, p. 30, Mệnh đề 3).

#### Hệ quả {#alg-v-s7-n3-cor-1 .statement}

— *Để một mở rộng đại số E tách được trên K, điều kiện cần và đủ là mọi phần tử của E đều là một nghiệm đơn của đa thức tối tiểu của nó trên K. Chỉ cần áp dụng Mệnh đề 5 và 6.*

### 4. Định lý phần tử nguyên thủy

Cho $ E $ là một mở rộng của $ K $; một phần tử $ x $ của $ E $ được gọi là *nguyên thủy* nếu $ E = K[x] $. Để mở rộng $ E $ có một phần tử nguyên thủy thì cần rằng $ [E : K] $ là hữu hạn.

#### Định lý 1 {#alg-v-s7-thm-1 .statement}

— *Cho E là một mở rộng của K. Khi đó các điều kiện sau là tương đương:
a) E có một phần tử nguyên thủy;
b) chỉ tồn tại một số hữu hạn các mở rộng con của E.
Các điều kiện này được thỏa mãn khi E là một mở rộng tách được bậc hữu hạn.* Trước hết giả sử rằng $ E $ có một phần tử nguyên thủy $ x $, và gọi $ f $ là đa thức tối tiểu của $ x $ trên K. Với mỗi đa thức đơn khởi $ g \in E[X] $ là ước của $ f $ trong $ E[X] $, ký hiệu $ E_g $ là mở rộng con của $ E $ được sinh bởi các hệ số của g. Vì số các đa thức g có thể có là hữu hạn (nếu $ f $ phân tích trong $ E[X] $ thành một tích của r đa thức đơn khởi bất khả quy, thì số đó bị chặn trên bởi $ 2^r $), nên số các mở rộng con $ E_g $ cũng là hữu hạn. Do đó, để chứng minh b), chỉ cần chỉ ra rằng mọi mở rộng con L của $ E $ đều là một trong các $ E_g $. Bây giờ, nếu $ L $ là một mở rộng con của E, thì ta có $ L[x] = E $; nếu g là đa thức tối tiểu của $ x $ trên L, thì ta có $ [E : L] = \deg(g) $. Mặt khác, g là một ước của f trong $ L[X] $, do đó cũng trong $ E[X] $; vậy nên ta có $ E_g \subset L $ và $ E = E_g[x] $. Vì $ g(x) = 0 $, ta có $ [E : E_g] \leq \deg(g) $, do đó $ [E : E_g] \leq [E : L] $ và vì thế $ L = E_g $ như cần phải chứng minh.

Tiếp theo ta nhận thấy rằng điều kiện b) suy ra rằng mở rộng E có bậc hữu hạn: theo Nhận xét 2 của V, p. 18, chỉ cần chứng minh rằng nó là đại số; mà nếu z là một phần tử của $ E $ siêu việt trên $ K $ thì các mở rộng con $ K(z^n), n \in \mathbf{N} $ là phân biệt từng đôi một.

Để chứng minh rằng b) $ \Rightarrow $ a), bây giờ ta phân biệt hai trường hợp:
A) Nếu trường $ K $ là *hữu hạn*, trường $ E $ là một không gian vectơ có số chiều hữu hạn trên K và do đó là một tập hợp hữu hạn. Vì thế $ ^1 $ (V, p. 78, Bổ đề 1) tồn tại một phần tử $ x $ của $ E $ sinh nhóm nhân của $ E $, và ta có $ E = K[x] $.

B) Bây giờ giả sử rằng trường $ K $ là vô hạn. Nếu $ b) $ đúng, thì mở rộng $ E $ có bậc hữu hạn, nên $ b) $ cũng có thể được phát biểu bằng cách nói rằng $ E $ chỉ có một số hữu hạn các đại số con. Như vậy, hệ quả $ b) \Rightarrow a) $ là một hệ quả của mệnh đề tổng quát hơn sau đây (mà giả thiết trường $ K $ là vô hạn là không thể thiếu được, xem V, p. 153, Bài tập 5 của § 7):

#### Mệnh đề 7 {#alg-v-s7-prop-7 .statement}

— *Giả sử rằng $ K $ là vô hạn; cho $ A $ là một đại số $ K $ giao hoán chỉ có một số hữu hạn các đại số con (ví dụ một đại số $ K $ étale, $ V $, p. 30, Mệnh đề 3) và cho $ V $ là một không gian con vectơ của $ A $ sinh ra $ A $. Khi đó tồn tại $ x \in V $ sao cho $ A = K[x] $.*

Cho $ A_1, \ldots, A_n $ là các đại số con của $ A $ phân biệt với $ A $. Nếu $ x \notin A_1 \cup \ldots \cup A_n $, thì đại số con $ K[x] $ không thể bằng bất kỳ $ A_i $ nào và do đó phải trùng với $ A $. Hơn nữa, vì $ V $ sinh ra $ A $, nên nó không được chứa trong bất kỳ không gian con nào trong các $ A_i $. Vậy Mệnh đề 7 là một hệ quả của bổ đề sau:

*Bổ đề 1. — Cho $ A $ là một không gian vectơ trên $ K $, và $ V, A_1, \ldots, A_n $ là các không gian con của $ A $. Nếu $ \mathrm{Card}(K) \geq n $ và nếu $ V $ không được chứa trong bất kỳ $ A_i $ nào, thì $ V $ không được chứa trong $ A_1 \cup \ldots \cup A_n $.*

Lập luận bằng quy nạp theo $ n $, ta chỉ cần chứng minh rằng nếu $ V \subset A $, và $ V \subset A_1 \cup \ldots \cup A_n $, thì $ V \subset A_1 \cup \ldots \cup A_{n-1} $. Lấy $ x \in V, x \notin A_n $, và lấy $ y $ tùy ý trong $ V $. Nếu $ y \in Kx $, ta có $ y \in A_1 \cup \ldots \cup A_{n-1} $; nếu không, thì các phần tử $ x $ và $ y + \lambda x, \lambda \in K $ có số lớn hơn hẳn $ n $ và thuộc $ A_1 \cup \ldots \cup A_n $, nên có hai phần tử trong số đó thuộc cùng một $ A_i $. Do đó tồn tại $ i, 1 \leq i \leq n $ sao cho hoặc $ x \in A_i $ và $ y + \lambda x \in A_i $ với một $ \lambda \in K $, hoặc $ y + \mu x \in A_i $ và $ y + \mu x \in A_i $ với hai vô hướng phân biệt $ \lambda, \mu \in K $. Trong cả hai trường hợp ta kết luận rằng $ x \in A_i $ và $ y \in A_i $; nhưng điều này kéo theo $ i \neq n $, do đó $ y \in A_1 \cup \ldots \cup A_{n-1} $, như điều phải chứng minh.

Điều này hoàn tất chứng minh về tính tương đương của $ a) $ và $ b) $ trong Định lý 1. Cuối cùng, nếu mở rộng $ E $ là tách được và có bậc hữu hạn, thì điều kiện $ b) $ đúng, theo V, p. 30, Mệnh đề 3.

### 5. Các tính chất ổn định của các mở rộng đại số tách được

#### Mệnh đề 8 {#alg-v-s7-prop-8 .statement}

— *Cho $ E $ là một mở rộng của $ K $ và $ (E_i)_{i \in I} $ là một họ các mở rộng con của $ E $ sao cho $ E = K \left( \bigcup_{i \in I} E_i \right) $. Nếu mỗi mở rộng $ E_i $ là đại số và tách được trên $ K $, thì $ E $ cũng có tính chất ấy.*

Điều này suy ra ngay từ Mệnh đề 6 (V, p. 39).

$ ^1 $ Người đọc có thể tự thuyết phục mình rằng Định lý 1 không được dùng ở đâu trước chứng minh của Bổ đề 1 ở V, p. 78.

#### Mệnh đề 9 {#alg-v-s7-prop-9 .statement}

— *Cho F là một mở rộng đại số của K và E là một mở rộng con của F. Để F tách được trên K thì điều cần và đủ là F tách được trên E và E tách được trên K.*

Trước hết giả sử rằng F tách được trên K; khi đó E tách được trên K theo Mệnh đề 1 (V, p. 36). Hơn nữa, mọi phần tử của F đều tách được trên K (V, p. 39, Mệnh đề 6), do đó cũng tách được trên E (V, p. 39, Hệ quả 2), và vì thế F tách được trên E (V, p. 39, Mệnh đề 6).

Ngược lại, giả sử rằng F tách được trên E và E tách được trên K. Ký hiệu x là một phần tử của F và $ f \in E[X] $ là đa thức tối tiểu của x trên E. Vì E đại số trên K, Định lý 2 (V, p. 18) cho thấy tồn tại một mở rộng con E' của E có bậc hữu hạn trên K sao cho $ f \in E'[X] $; khi đó f đồng thời là đa thức tối tiểu của x trên E và trên E', và vì x tách được trên E (V, p. 39, Mệnh đề 6) nên nó cũng tách được trên E' (V, p. 39, Mệnh đề 5). Đặt $ F' = E'(x) $; khi đó F tách được và có bậc hữu hạn trên E', và vì E tách được trên K nên E' tách được và có bậc hữu hạn trên K (V, p. 36, Mệnh đề 1). Do đó F tách được và có bậc hữu hạn trên K, theo V, p. 32, Hệ quả 2. Vì vậy (V, p. 39, Mệnh đề 6) x tách được trên K. Đến đây ta đã chỉ ra rằng mọi phần tử của F đều tách được trên K, suy ra F tách được trên K (V, p. 39, Mệnh đề 6).

#### Mệnh đề 10 {#alg-v-s7-prop-10 .statement}

— *Cho E và K' là hai mở rộng con của cùng một mở rộng của K và đặt $ E' = K'(E) $. Giả sử rằng E đại số trên K, do đó E' đại số trên K' (V, p. 18, Hệ quả 2).

a) *Nếu E tách được trên K, thì E' tách được trên K'._

b) *Ngược lại nếu E' tách được trên K' và E và K' rời nhau tuyến tính trên K, thì E tách được trên K._

Mệnh đề *a)* suy ra trực tiếp từ Mệnh đề 6 (V, p. 39).

Dưới giả thiết *b)*, cho F là một mở rộng con của E có bậc hữu hạn trên K. Khi đó F và K' rời nhau tuyến tính trên K, do đó K'-đại số $ F_{(K')} = K' \otimes_K F $ đẳng cấu với $ K'(F) $. Vì $ K'(F) $ là một mở rộng con của E' có bậc hữu hạn trên K' và E' đại số và tách được trên K', nên K'-đại số $ K'(F) $ là étale. Nói cách khác, K'-đại số $ F_{(K')} $ là étale, và bây giờ Hệ quả 2 của Mệnh đề 4 (V, p. 32) cho thấy rằng F là étale trên K. Vậy ta đã chỉ ra rằng E tách được trên K.

### 6. Một tiêu chuẩn tách được

#### Mệnh đề 11 {#alg-v-s7-prop-11 .statement}

— *Giả sử rằng K có số mũ đặc số p, và cho E là một mở rộng đại số của K, sinh bởi một tập hợp S. Nếu E tách được trên K, thì $ E = K(S^{p^n}) $ với mọi số nguyên $ n \geq 0 $; ngược lại nếu E có bậc hữu hạn trên K và $ E = K(S^p) $, thì E tách được trên K._

Trường hợp $ p = 1 $ là tầm thường theo Hệ quả của V, p. 37. Từ nay giả sử rằng $ p \neq 1 $.

Theo giả thiết E đại số trên K và ta có $ E = K(S) $, do đó

$$
K(S^p) = K(E^p) = K[E^p] \quad \text{theo V, p.18, Hệ quả 1.}
$$

Nếu E có bậc hữu hạn trên K, thì nó là một mở rộng tách được của K khi và chỉ khi nó là một đại số étale trên K; Hệ quả ở V, p. 35 cho thấy điều này xảy ra khi và chỉ khi $ E = K[E^p] $.

Giả sử bây giờ rằng $ E $ tách được và có bậc vô hạn trên $ K $. Khi đó $ K[E^p] $ là hợp của các vành con $ K[E'^p] $ khi $ E' $ chạy qua tập hợp các mở rộng con của $ E $ có bậc hữu hạn trên $ K $; nhưng một mở rộng như vậy $ E' $ là tách được trên $ K $ ($ V $, p. 36, Mệnh đề 1), do đó $ E' = K[E'^p] \subset K[E^p] $ theo điều đã nói; cuối cùng ta có $ E = K[E^p] $. Bằng quy nạp theo $ n \geq 0 $, quan hệ $ E = K[E^p] $ kéo theo rằng $ E = K[E^{p^n}] $.

#### Hệ quả 1 {#alg-v-s7-prop-11-cor-1 .statement}

— *Mọi mở rộng đại số của một trường hoàn hảo đều là một trường hoàn hảo.*

Cho $ K $ là một trường hoàn hảo có đặc số số mũ $ p $, và $ E $ là một mở rộng đại số của $ K $. Khi đó $ E $ tách được trên $ K $ ($ V $, p. 36, Prop. 2), do đó $ E = K(E^p) $ theo Mệnh đề 11; nhưng ta có $ K = K^p \subset E^p $, nên $ E = K(E^p) = E^p $, và vì thế $ E $ là hoàn hảo.

#### Hệ quả 2 (Mac Lane) {#alg-v-s7-prop-11-cor-2 .statement}

— *Cho $ K $ là một bao đóng đại số của $ K $ và $ K^{p^{-\infty}} $ là bao đóng hoàn hảo của $ K $ trong $ \overline{K} $. Để một mở rộng con $ E $ của $ \overline{K} $ tách được trên $ K $, điều kiện cần và đủ là nó rời nhau tuyến tính với $ K^{p^{-\infty}} $ trên $ K $.*

Ta có thể ngay lập tức rút gọn về trường hợp $ [E : K] $ là hữu hạn. Cho $ (x_i)_i $, là một cơ sở của $ E $ trên $ K $. Để $ E $ độc lập tuyến tính với $ K^{p^{-\infty}} $ thì điều cần và đủ là nó độc lập tuyến tính với $ K^{p^n} $ với mọi $ n \geq 0 $, và điều này đơn giản có nghĩa là quan hệ $ \sum_{i \in I} x_i a_i^{p^{-n}} = 0 $ kéo theo $ a_i = 0 $ với mọi $ i \in I $, đối với mọi họ $ (a_i)_i $, gồm các phần tử của $ K $. Điều này đến lượt nó có nghĩa là họ $ (x_i^{p^n})_{i \in I} $ là tự do trên $ K $, hay cũng có nghĩa là nó là một cơ sở của không gian vectơ $ E $ trên $ K $. Nói cách khác, $ E $ độc lập tuyến tính với $ K^{p^{-n}} $ khi và chỉ khi $ E = K(E^{p^n}) $. Bây giờ chỉ còn việc áp dụng Mệnh đề 11.

#### Nhận xét {#alg-v-s7-n6-rem-1 .statement}

— 1) Khi $ E $ là đại số và có bậc vô hạn trên $ K $, điều kiện $ E = K(E^p) $ không phải lúc nào cũng bảo đảm rằng $ E $ tách được trên $ K $. Ví dụ, nếu $ K $ không hoàn hảo và $ E $ là một bao đóng hoàn hảo của $ K $, thì ta có $ E = K(E^p) $ nhưng $ E $ không phải là một mở rộng tách được của $ K $ ($ V $, p. 39, Hệ quả 3).
2) Cho $ E $ là một mở rộng đại số tách được của một trường $ K $ có số mũ đặc số $ p $. Khi đó ta có $ E^p \cap K = K^p $ (Hệ quả 2); do đó nếu $ E $ hoàn hảo thì $ K $ cũng vậy.

### 7. Bao đóng đại số tách được tương đối

#### Mệnh đề 12 {#alg-v-s7-prop-12 .statement}

— *Cho $ E $ là một mở rộng của $ K $ và $ E_s $, tập hợp các phần tử của $ E $ là đại số và tách được trên $ K $. Khi đó $ E_s $, là mở rộng con lớn nhất của $ E $ là đại số và tách được trên $ K $.*

Theo Mệnh đề 6, *a*) ($ V $, p. 39), mọi mở rộng con của $ E $ mà đại số và tách được trên $ K $ đều được chứa trong $ E_s $. Theo Mệnh đề 6, *b*) (*loc. cit.*), mở rộng $ K(E_s) $ của $ K $ là đại số và tách được, do đó $ K(E_s) \subset E $, và vì thế $ K(E_s) = E_s $.

Với ký hiệu của mệnh đề trước, E, được gọi là bao đóng tách được (đại số) tương đối của K trong E. Khi K là hoàn hảo, E, là bao đóng đại số tương đối của K trong E (V, p. 36, Mệnh đề 2).

#### Mệnh đề 13 {#alg-v-s7-prop-13 .statement}

— Cho E là một mở rộng đại số của K và gọi E,, là bao đóng đại số tách được tương đối của K trong E.
a) E là một mở rộng p-căn của E,.
b) Nếu F là một mở rộng con của E sao cho E là p-căn trên F, thì F ⊃ E,.
c) E, là mở rộng con duy nhất của E tách được trên K và trên đó E là p-căn.
Chỉ cần chứng minh a) trong trường hợp K có đặc số $ p \neq 0 $. Cho x là một phần tử của E và f là đa thức tối tiểu của nó trên K. Tồn tại một số nguyên $ m \geq 0 $ sao cho f thuộc $ K[X^{p^m}] $ nhưng không thuộc $ K[X^{p^{m+1}}] $; nói cách khác, ta có $ f(X) = g(X^{p^m}) $ với $ g \in K[X] $, $ g \notin K[X^p] $. Vì f là bất khả quy nên g cũng vậy, do đó g là đa thức tối tiểu của $ x^{p^m} $ trên K. Theo V, p. 38, Mệnh đề 4 và p. 39, Mệnh đề 5, suy ra $ x^{p^m} \in E_s $, vì thế E là p-căn trên E,.

Bây giờ giả sử giả thiết b) đúng và lấy $ x \in E, $. Vì x tách được trên K nên nó cũng tách được trên F (V, p. 39, Hệ quả 2), nhưng vì E là p-căn trên F nên x cũng là p-căn trên F, do đó $ x \in F $ (V, p. 39, Hệ quả 3).

Cuối cùng c) suy ra từ a), b) và Mệnh đề 12.

#### Hệ quả 1 {#alg-v-s7-prop-13-cor-1 .statement}

— Cho E và K' là hai mở rộng của K được chứa trong cùng một mở rộng của K. Giả sử rằng E là đại số trên K và ký hiệu E, là bao đóng đại số tách được tương đối của K trong E. Khi đó $ K'(E_s) $ là bao đóng đại số tách được tương đối của K' trong $ K'(E) $.

Vì $ K'(E_s) $ là một mở rộng đại số tách được của K' theo Mệnh đề 10 (V, p. 42); vì E là p-căn trên E,, mở rộng $ K'(E) $ của $ K'(E_s) $ là p-căn (V, p. 25, Hệ quả). Bây giờ chỉ cần áp dụng Mệnh đề 13.

#### Hệ quả 2 {#alg-v-s7-prop-13-cor-2 .statement}

— Nếu E có bậc hữu hạn trên K, thì $ E_s = \bigcap_{n \geq 0} K(E^{p^n}) $.

Với mỗi số nguyên $ n \geq 0 $ ký hiệu F, là mở rộng con $ K(E^{p^n}) $ của E. Dãy $ (F_n)_{n \geq 0} $ các không gian con vectơ của E là giảm và E có số chiều hữu hạn trên K. Do đó tồn tại một số nguyên $ m \geq 0 $ sao cho $ F_m = F_n $ với mọi $ n \geq m $. Vì vậy ta có $ K(F_m^p) = F_{m+1} = F_m $, do đó $ F_m $ là một mở rộng tách được của K (V, p. 42, Mệnh đề 11); hiển nhiên rằng E là p-căn trên F,, và vì thế Mệnh đề 13 suy ra $ E_s = F_m = \bigcap_{n \geq 0} F_n $.

#### Nhận xét {#alg-v-s7-n7-rem-1 .statement}

Cho E là một mở rộng đại số của K và E, là bao đóng p-căn tương đối của E trong K (V, p. 25). Khi đó E, là mở rộng con lớn nhất của E mà p-căn trên K (V, p. 25, Mệnh đề 2). Tuy nhiên, nói chung E không tách được trên E, (V, p. 152, Bài tập 2); về trường hợp các mở rộng quasi-Galois xem V, p. 76.

### 8. Bao đóng tách được của một trường

#### Định nghĩa 4 {#alg-v-s7-def-4 .statement}

— *Một trường K được gọi là đóng tách được nếu mọi mở rộng đại số tách được của K là tầm thường.*

Một trường đóng đại số là đóng tách được. Ngược lại, nếu một trường hoàn hảo K là đóng tách được, thì nó là đóng đại số, bởi vì mọi mở rộng đại số của K đều là tách được (*V*, p. 3 , Mệnh đề 2).

#### Định nghĩa 5 {#alg-v-s7-def-5 .statement}

— *Cho K là một trường. Ta hiểu một bao đóng đại số tách được, hoặc (do lạm dụng ngôn ngữ) bao đóng tách được của K, là mọi mở rộng E của K là đại số và tách được trên K, và sao cho trường E là đóng tách được.*

Khi K là hoàn hảo, có sự đồng nhất hoàn toàn giữa các khái niệm bao đóng tách được và bao đóng đại số của K (*V*, p. 36, Mệnh đề 2 và p. 43, Hệ quả 1).

#### Mệnh đề 14 {#alg-v-s7-prop-14 .statement}

— *Cho Ω là một mở rộng đóng đại số của K.*

a) *Bao đóng đại số tách được tương đối Ω_s của K trong Ω là một bao đóng tách được của K.*

b) *Nếu E và E' là hai bao đóng tách được của K, tồn tại một K-đẳng cấu của E lên E'._*

Cho F là một mở rộng đại số tách được của Ω_s ; vì Ω đóng đại số, tồn tại một 0,-đồng cấu u của F vào Ω (*V*, p. 20, Th. 1). Theo Mệnh đề 9 (V, p. 42), $ u(F) $ tách được trên K, do đó $ u(F) = \Omega_s $. Vậy F là một mở rộng tầm thường của $ \Omega_s $ và do đó $ \Omega_s $ đóng tách được, suy ra *a)*.

Cho E là một bao đóng tách được của K. Vì E là một mở rộng đại số của K, tồn tại một K-đồng cấu v của E vào Ω (*V*, p. 20, Th. 1). Do đó $ v(E) $ là đại số tách được trên K, suy ra $ v(E) \subset \Omega_s $. Theo *V*, p. 42, Mệnh đề 9, $ \Omega_s $ tách được trên $ v(E) $ và vì trường $ v(E) $ đóng tách được, ta có $ v(E) = \Omega_s $. Suy ra v là một K-đẳng cấu của E lên $ \Omega_s $. Bây giờ *b)* là một hệ quả ngay lập tức.

#### Hệ quả {#alg-v-s7-n8-cor-1 .statement}

— *Cho E là một mở rộng đóng tách được của K và F là một mở rộng đại số tách được của K ; khi đó tồn tại một K-đồng cấu của F vào E.*

Cho Ω là một bao đóng đại số của E ; ta có $ \Omega_s \subset E $ và chỉ cần xét trường hợp $ E = \Omega_s $. Vì F là một mở rộng đại số của K, tồn tại một K-đồng cấu u của F vào Ω (*V*, p. 20, Th. 1). Vì trường $ u(F) $ là tách được trên K, ta có $ u(F) \subset \Omega_s $ và u xác định một K-đồng cấu của F vào $ \Omega_s = E $.

#### Nhận xét 1 {#alg-v-s7-n8-rem-1 .statement}

Cho E và E' là hai bao đóng tách được của K. Nếu K không đóng tách được, tồn tại nhiều K-đẳng cấu của E lên E'. \* Vì khi đó E là một mở rộng Galois không tầm thường của K, và do đó tồn tại các K-tự đồng cấu của E phân biệt với đồng nhất (*V*, p. 56, Th. 1).
\* 2) Cho E là một mở rộng đại số và tách được của K. Nếu mọi mở rộng đại số và tách được của K đều đẳng cấu với một mở rộng con của E, thì E là một bao đóng tách được của K. Thật vậy, nếu E' là một bao đóng tách được của K, thì mỗi một trong các mở rộng E và E' đều đẳng cấu với một mở rộng con của mở rộng kia; do đó E và E' là các mở rộng đẳng cấu của K (V, p. 52, Prop. 1, a)).

### 9. Bậc tách được và bậc không tách được của một mở rộng có bậc hữu hạn

Cho E là một mở rộng có bậc hữu hạn của K và $ \Omega $ là một bao đóng đại số của K. Nhắc lại (V, p. 31) rằng theo *bậc tách được* của E trên K, ký hiệu $[E : K]_s$, ta hiểu số các K-đồng cấu của E vào $ \Omega $.

#### Mệnh đề 15 {#alg-v-s7-prop-15 .statement}

*Cho E, là bao đóng tách được tương đối của K trong E; khi đó* $[E : K]_s = [E_s : K]$.

Trường $ \Omega $ là hoàn hảo và E là p-căn trên $ E_s $, theo V, p. 44, Prop. 13; do đó Prop. 3 (V, p. 26) chỉ ra rằng mọi K-đồng cấu của E, vào $ \Omega $ đều mở rộng một cách duy nhất thành một K-đồng cấu của E vào $ \Omega $; vì vậy ta có $[E : K]_s = [E_s : K]$. Vì E, là một mở rộng tách được có bậc hữu hạn của K, nó là một đại số etale trên K; do đó ta có $[E_s : K]_s = [E_s : K]$ theo V, p. 32, Prop. 4, và kết quả được suy ra.

Với ký hiệu trên, bậc của E trên $ E_s $ được gọi là *bậc không khả phân* của E trên K và được ký hiệu bởi $[E : K]_i$. Do đó ta có

(1)
$$
[E : K] = [E : K]_s \cdot [E : K]_i
$$
theo Mệnh đề 15.

Khi K có đặc số 0, thì $ E = E_s $, và do đó $[E : K]_s = [E : K]$ và $[E : K]_i = 1$. Nếu K có đặc số $ p \neq 0 $, số $[E : K]_i$ là một lũy thừa của p vì E là p-căn trên $ E_s $ (V, p. 44, Mệnh đề 13 và p. 26, Mệnh đề 4). Cần lưu ý rằng $[E : K]_i$ không nhất thiết bằng lũy thừa cao nhất của $ p $ chia hết $[E : K]_s$, cũng không nhất thiết bằng bậc $[E_s : K]$ của bao đóng p-căn tương đối của E trong K (V, p. 152, Bài tập 3 và 2).

#### Mệnh đề 16 {#alg-v-s7-prop-16 .statement}

*Cho $ \Omega $ là một mở rộng của K và E, F là hai mở rộng con của $ \Omega $, có bậc hữu hạn trên K.*

a) *Nếu $ E \subset F $, thì* $[F : K]_s = [F : E]_s \cdot [E : K]_s$, *và* $[F : K]_i = [F : E]_i \cdot [E : K]_i$.

b) *Cho $ K' $ là một mở rộng con của $ \Omega $; khi đó ta có*
$$
[K'(E) : K']_s \leq [E : K]_s \quad \text{và} \quad [K'(E) : K']_i \leq [E : K]_i,
$$
*và đẳng thức xảy ra nếu $ K' $ rời nhau tuyến tính với E trên K.*

c) *Ta có* $[K(E \cup F) : K]_s \leq [E : K]_s \cdot [F : K]_s$, *và* $[K(E \cup F) : K]_i \leq [E : K]_i \cdot [F : K]_i$, *và đẳng thức xảy ra nếu E và F rời nhau tuyến tính trên K*.

Mệnh đề về các bậc tách được trong a) suy ra từ (9) (V, p. 32). Vì $[F : K] = [F : E] \cdot [E : K]$, mệnh đề về các bậc không tách được suy ra từ điều này và (1).

Theo Hệ quả 1 của Mệnh đề 13 (V, p. 44) và Mệnh đề 15, ta có

(2) $$ [K'(E) : K']_s = [K'(E_s) : K'] , \quad [K'(E) : K']_i = [F'(E) : K'(E_s)] ; $$

khi K' rời nhau tuyến tính với E trên K, thì E, rời nhau tuyến tính với K' trên K và E rời nhau tuyến tính với K'(E_s) trên E_s (V, p. 15, Mệnh đề 8). Mệnh đề b) bây giờ suy ra từ Mệnh đề 5 (V, p. 14).

Theo a) ta có $$ [K(E \cup F) : K] = [F(E) : F] . [F : K]_s ; $$ theo b) ta có $$ [F(E) : F] , \leq [E : K] , \text{ với đẳng thức nếu } E \text{ và } F \text{ rời nhau tuyến tính trên } K. $$ Do đó ta được bất đẳng thức $$ [K(E \cup F) : K] , \leq [E : K] , . [F : K] , \text{ với đẳng thức nếu } E \text{ và } F \text{ rời nhau tuyến tính trên } K. $$ Mệnh đề của c) về các bậc không tách được được chứng minh theo cách tương tự.

### Bài tập {#alg-v-s7-exercises}

Xem [bài tập của § 7](exercises/s7/).
