---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 3
section_title: Algebraic extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.15-A V.19, A V.147-A V.150
pdf_pages: 0129-0133, 0261-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraic elements of an algebra
      page: 15
      pdf_page: 129
    - "no": 2
      title: Algebraic extensions
      page: 17
      pdf_page: 131
    - "no": 3
      title: Transitivity of algebraic extensions. Fields that are relatively algebraically closed in an extension field
      page: 19
      pdf_page: 133
statements: 15
exercises: 13
content_sha256: 5a812c483a2ae692fe9172df9ea287985004cafdd850c31afe1e8dfd323be550
translated_from: content/en/alg/V/03_s3_algebraic_extensions.md
source_content_sha256: 17c946f4566c0b7e2c26fd35edc67eac1891ca428d8e227bcf617d53f96ac501
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-8d26213a
glossary_version: 34
glossary_terms_sha256: b96166760c5884143b9ab3cecdd370fa535764ee4a88c99cdc03fb254bc7665d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. MỞ RỘNG ĐẠI SỐ

### 1. Các phần tử đại số của một đại số

Cho A là một đại số trên một trường K và x là một phần tử của A. Có thể xảy ra hai trường hợp:

a) Họ các đơn thức $(x^n)_{n \in \mathbf{N}}$ là tự do trên $K$. Khi đó ta nói rằng $x$ là siêu việt trên $K$. Có một đẳng cấu từ đại số đa thức $K[X]$ lên đại số con $K[x]$ của $A$ được sinh bởi $x$, và đại số con này có bậc vô hạn trên $K$.

b) Có một số nguyên $n \geq 1$ sao cho các đơn thức $1,\ x,\ \ldots,\ x^{n-1},\ x^n$ độc lập tuyến tính; điều này tương đương với việc tồn tại một đa thức $f \neq 0$ trong $K[X]$ sao cho $f(x) = 0$. Khi đó ta nói rằng $x$ là đại số trên $K$. Số nguyên nhỏ nhất $n \geq 1$ thỏa mãn tính chất trên được gọi là bậc của $x$ trên $K$. Nếu bậc của $x$ trên $K$ là $n$, thì các đơn thức $1,\ x,\ \ldots,\ x^{n-1}$ độc lập tuyến tính trên $K$ và tồn tại các phần tử $a_0,\ a,,\ \ldots,\ a_{-1}$ của $K$ sao cho
$$
x^n = a_0 + a_1 x + \cdots + a_{n-1} x^{n-1}
$$
Đa thức $f(X) = X^n - \sum_{k=0}^{n-1} a_k X^k$ là đa thức đơn khởi duy nhất có bậc $n$ trong $K[X]$ sao cho $f(x) = 0$; nó được gọi là đa thức tối tiểu của $x$ trên $K$.

#### Định lý 1 {#alg-v-s3-thm-1 .statement}

— Cho $A$ là một đại số trên một trường $K$, $x$ là một phần tử của $A$ đại số trên $K$, $n$ là bậc và $f$ là đa thức tối tiểu của $x$ trên $K$.

a) Để một đa thức $g \in K[X]$ thỏa mãn $g(x) = 0$ thì điều kiện cần và đủ là $g$ là một bội của $f$.

b) Ánh xạ $g \mapsto g(x)$ xác định qua phép chuyển qua các thương một đẳng cấu của đại số thương $K[X]/(f)$ lên đại số $K[x]$, và các phần tử $1,\ x,\ \ldots,\ x^{n-1}$ tạo thành một cơ sở của $K[x]$ trên $K$. Đặc biệt, $[K[x]:K] = n$.

c) Giả sử rằng $A$ là một miền nguyên. Khi đó $K[x]$ là một trường và $f$ là đa thức bất khả quy monic duy nhất trong $K[X]$ sao cho $f(x) = 0$.

d) Để $x$ khả nghịch trong $A$, điều kiện cần và đủ là $f(0) \neq 0$; khi đó ta có $x^{-1} \in K[x]$.

Tồn tại một đồng cấu đại số duy nhất $\varphi : K[X] \to A$ sao cho $\varphi(X) = x$; ta có $\varphi(P) = P(x)$ với mọi $P \in K[X]$ và ảnh của $\varphi$ bằng $K[x]$. Gọi $a$ là hạt nhân của $\varphi$: theo phép dựng, đa thức tối tiểu $f$ của $x$ trên $K$ thuộc $a$ và nó là đa thức đơn khởi có bậc nhỏ nhất trong $a$. Do đó ($IV$, p. 11, Prop. 11) ta có $a = (f)$, do đó $a$. Mệnh đề $b$) suy ra ngay từ a) và Hệ quả của Mệnh đề 10 của $IV$, p. 11.

Giả sử rằng $A$ là một miền nguyên. Đại số $K[x]$ khi đó là một miền nguyên và có bậc hữu hạn trên $K$, do đó nó là một trường ($V$, p. 10, Hệ quả). Vì thế iđêan $(f)$ của $K[x]$ là cực đại, điều đó có nghĩa là $f$ là bất khả quy trong $K[X]$ ($IV$, p. 13). Sau hết, cho $g$ là một đa thức bất khả quy đơn nhất trong $K[X]$ sao cho $g(x) = 0$; theo $a$) nó là một bội của $f$, do đó $g = f$, và điều này chứng minh $c$).

Còn phải chứng minh $d$). Tồn tại một đa thức $g \in K[X]$ bậc $n-1$ và một phần tử $a$ của $K$ sao cho $f(X) = Xg(X) + a$, do đó $f(0) = a$. Nếu $a = 0$, ta có $xg(x) = f(x) = 0$, và $g(x) \neq 0$, vậy khi đó $x$ không khả nghịch trong $A$. Nếu ngược lại $a \neq 0$, thì ta có $x \cdot [-a^{-1}g(x)] = 1$, nên khi đó $x$ khả nghịch trong $A$ và $x^{-1} = -a^{-1}g(x)$.

#### Hệ quả 1 {#alg-v-s3-thm-1-cor-1 .statement}

— Cho $ A $ là một đại số trên một trường $ K $. Để một phần tử $ x $ của $ A $ là đại số trên $ K $, điều kiện cần và đủ là đại số con $ K[x] $ của $ A $ sinh bởi $ x $ phải có bậc hữu hạn trên $ K $. Đặc biệt, nếu $ A $ có bậc hữu hạn trên $ K $, thì mọi phần tử của $ A $ đều đại số trên $ K $.

#### Hệ quả 2 {#alg-v-s3-thm-1-cor-2 .statement}

— Cho $ E $ là một mở rộng của $ K $, $ A $ là một đại số trên $ E $ và $ x $ là một phần tử của $ A $ đại số trên $ K $. Khi đó $ x $ đại số trên $ E $, đa thức tối tiểu của $ x $ trên $ E $ chia đa thức tối tiểu của $ x $ trên $ K $ và bậc của $ x $ trên $ E $ nhiều nhất bằng bậc của $ x $ trên $ K $.

Vì lấy $ f $ là đa thức tối tiểu của $ x $ trên $ K $; ta có $ f(x) = 0 $ và $ f \in E[X] $, do đó $ x $ đại số trên $ E $ và $ f $ là một bội của đa thức tối tiểu của $ x $ trên $ E $ (Đl. 1, *a*).

#### Nhận xét {#alg-v-s3-n1-rem-1 .statement}

— Cho $ E $ là một mở rộng của một trường $ K $ và $ x $ là một phần tử của $ E $ là nghiệm của một đa thức bất khả quy đơn nhất $ f \in K[X] $. Khi đó Th. 1, *c*) cho thấy rằng $ f $ là đa thức tối tiểu của $ x $ trên $ K $.

#### Ví dụ {#alg-v-s3-n1-exa-1 .statement}

— \* 1) Trong trường số phức $ \mathbf{C} $, số $ i $ là đại số bậc 2 trên trường nguyên tố $ \mathbf{Q} $; vì nếu $ f(X) = X^2 + 1 $, thì $ f(i) = 0 $, và $ x^2 + 1 \neq 0 $ với mọi $ x \in \mathbf{Q} $, do đó $ i \notin \mathbf{Q} $. Vậy trường $ \mathbf{Q}(i) $ là một mở rộng bậc 2 của $ \mathbf{Q} $; nó gồm tất cả các số $ a + bi $, trong đó $ a, b $ là hữu tỉ. Tương tự, $ i $ là đại số bậc 2 trên trường $ \mathbf{R} $ của các số thực, và $ \mathbf{C} $ là một mở rộng bậc 2 của $ \mathbf{R} $. \*

2) Cho $ K $ là một trường và $ F $ là trường $ K(X) $ các phân thức hữu tỉ theo một ẩn trên $ K $. Gọi $ E $ là trường con $ K(X^3) $ của $ F $; ta có $ F = E(X) $ và $ X $ là đại số trên $ E $, vì nó là một nghiệm của đa thức $ Y^3 - X^3 $ của vành $ E[Y] $; đa thức này là bất khả quy trong $ E[Y] $, vì nếu ngược lại thì nó sẽ có ít nhất một nhân tử bậc nhất, và khi đó sẽ tồn tại hai đa thức khác không $ u(X) $, $ v(X) $ của $ K[X] $ sao cho $ (u(X^3))^3 = X^3(v(X^3))^3 $, điều này vô lý, vì nếu $ m $ và $ n $ là các bậc của $ u $ và $ v $, thì điều đó sẽ kéo theo $ 9m = 9n + 3 $, hay $ 3m = 3n + 1 $. Do đó trường $ F $ có bậc 3 trên $ E $, và mọi phần tử của $ F $ có thể được viết theo đúng một cách như một tổ hợp tuyến tính $ f(X^3) + Xg(X^3) + X^2 h(X^3) $, trong đó $ f, g, h $ là ba phân thức hữu tỉ của $ K(X) $.

\* 3) Trong trường $ \mathbf{R} $ các số thực, có thể chứng minh được $ ^1 $ rằng số $ \pi $ là siêu việt trên trường nguyên tố $ \mathbf{Q} $. \*

### 2. Mở rộng đại số

#### Định nghĩa 1 {#alg-v-s3-def-1 .statement}

— Một mở rộng $ E $ của một trường $ K $ được gọi là đại số (trên $ K $) nếu mọi phần tử của $ E $ đều đại số trên $ K $. Một mở rộng $ E $ của $ K $ mà không đại số được gọi là siêu việt (trên $ K $).

#### Mệnh đề 1 {#alg-v-s3-prop-1 .statement}

— Để một mở rộng $ E $ của $ K $ là đại số thì điều kiện cần và đủ là mọi đại số con trên K $ A $ của $ E $ đều là một trường.

$ ^1 $ Xem chẳng hạn D. Hilbert, Gesammelte Abhandlungen, vol. 1, p. 1 (Berlin (Springer), 1932).

Điều kiện là cần thiết : nếu $ E $ là đại số trên $ K $ và $ x \neq 0 $ là một phần tử của một đại số con trên K $ A $ của $ E $, thì $ x^{-1} \in K[x] \subset A $ theo $ V $, p. 16, Định lý 1, d). Do đó $ A $ là một trường.

Điều kiện là đủ: nếu nó được thỏa mãn và $ x $ là một phần tử $ \neq 0 $ của $ E $, thì vành $ K[x] $ là một trường, do đó $ x^{-1} \in K[x] $; nói cách khác, tồn tại một đa thức $ g \in K[X] $ sao cho $ x^{-1} = g(x) $, hay cũng vậy $ xg(x) - 1 = 0 $; điều này cho thấy $ x $ là đại số trên $ K $, do đó $ E $ là một mở rộng đại số của $ K $.

#### Mệnh đề 2 {#alg-v-s3-prop-2 .statement}

— *Nếu một mở rộng E của K có bậc hữu hạn n, thì nó là đại số và bậc trên K của mỗi phần tử của E chia hết cho n.*

Thật vậy, với $ x \in E $, $ [K(x):K] $ là hữu hạn và là ước của n ($ V $, p. 10, Hệ quả 1) và do đó $ x $ là đại số trên $ K $ ($ V $, p. 17, Hệ quả 1).

*Tồn tại những mở rộng đại số bậc vô hạn, chẳng hạn bao đóng đại số của một trường hữu hạn (V, p. 24, Nhận xét 4).*

#### Định lý 2 {#alg-v-s3-thm-2 .statement}

— *Cho E là một mở rộng sinh hữu hạn của K, được sinh bởi các phần tử $ a_1, ..., a_m $, là những phần tử đại số trên K; khi đó E là một mở rộng bậc hữu hạn của K. Nếu bậc của $ a_i $ trên $ K(a_1, a_2, ..., a_{i-1}) $ là $ n_i $ (với $ 1 \leq i \leq m $), thì bậc của E trên K là $ n_1 n_2 ... n_m $ và các phần tử $ a_1^{v_1} a_2^{v_2} ... a_m^{v_m} $ ($ 0 \leq v_i \leq n_i - 1 $) lập thành một cơ sở của E trên K.*

Các phần tử $ a_i^{v_i} $ ($ 0 \leq v_i \leq n_i - 1 $) tạo thành một cơ sở của $ K(a_1, a_2, ..., a_i) $ trên $ K(a_1, a_2, ..., a_{i-1}) $ theo Th. 1, b) của $ V $, p. 16; do đó định lý được suy ra bằng quy nạp theo $ m $ từ Prop. 25 của II, p. 222.

#### Hệ quả 1 {#alg-v-s3-thm-2-cor-1 .statement}

— *Cho E là một mở rộng của K và A là một tập con của E gồm các phần tử đại số trên K. Khi đó $ K(A) $ là đại số trên K và ta có $ K[A] = K(A) $.*

Mỗi $ x \in K(A) $ đều thuộc một trường $ K(F) $, trong đó F là một tập con hữu hạn của $ A $ ($ V $, p. 11, Hệ quả); bây giờ $ K(F) $ là đại số trên $ K $ và bằng $ K[F] $ theo Định lý 2, do đó $ x $ là đại số trên $ K $ và $ K(A) = K[A] $.

#### Hệ quả 2 {#alg-v-s3-thm-2-cor-2 .statement}

— *Cho L là một mở rộng của K và E, F là các mở rộng con của L. Nếu F là đại số trên K, vành con $ K[E, F] $ của L sinh bởi $ E \cup F $ là một trường trùng với $ E(F) $ và đại số trên E.*

Mỗi phần tử của $ F $, là đại số trên $ K $, cũng là đại số trên $ E $ ($ V $, p. 17, Hệ quả 2), do đó $ E(F) $ là một mở rộng đại số của $ E $, và ta có $ E(F) = E[F] $ theo Hệ quả 1.

#### Nhận xét {#alg-v-s3-n2-rem-1 .statement}

— 1) Với ký hiệu của Đl. 2, $ E = K[a_1, a_2, ..., a_n] $ và do đó $ E $ đẳng cấu với một thương $ K[X_1, X_2, ..., X_m]/\mathfrak{a} $; vì $ E $ là một trường, $ a $ là một iđêan cực đại trong $ K[X_1, ..., X_m] $.

2) Cho $ E $ là một mở rộng đại số của $ K $, có bậc vô hạn. Theo Định lý 2, tồn tại một dãy vô hạn $ (a_i) $, gồm các phần tử của $ E $ sao cho $ a_i \notin K(a_1, a_2, ..., a_{i-1}) $; Định lý 2 còn cho thấy rằng bậc của $ K(a_1, a_2, ..., a_n) $ trên $ K $ nhận những giá trị lớn tùy ý. Nói cách khác, nếu E là một mở rộng đại số của K sao cho các bậc [F : K] của các mở rộng con F của E có bậc hữu hạn trên K đều bị chặn, thì E là một mở rộng hữu hạn bậc của K.

### 3. Tính bắc cầu của các mở rộng đại số. Các trường tương đối đóng đại số trong một trường mở rộng

#### Mệnh đề 3 {#alg-v-s3-prop-3 .statement}

— Cho E và F là hai trường mở rộng của một trường K sao cho K ⊂ E ⊂ F. Điều kiện cần và đủ để F là đại số trên K là E đại số trên K và F đại số trên E.

Điều kiện đó là cần, theo V, p. 17, Hệ quả 2. Hãy chứng minh rằng nó là đủ. Cho x là một phần tử tùy ý của F; nó là đại số trên E; gọi g ∈ E[X] là đa thức tối tiểu của nó trên E. Nếu A là tập hợp (hữu hạn) các hệ số của g, thì g ∈ K(A)[X], do đó x là đại số trên K(A) và K(A U {x}) = K(A)(x) có bậc hữu hạn trên K(A). Bây giờ A ⊂ E và E là đại số trên K, nên K(A) có bậc hữu hạn trên K, theo Định lý 2. Vậy nên (V, p. 10, Định lý 1), K(A U {x}) có bậc hữu hạn trên K, điều này chứng tỏ x là đại số trên K (V, p. 18, Mệnh đề 2).

#### Định nghĩa 2 {#alg-v-s3-def-2 .statement}

— Một trường con K của một trường E được gọi là tương đối đóng đại số trong E nếu mọi phần tử của E là đại số trên K đều thuộc về K.

Điều đó tương đương với việc nói rằng K là mở rộng đại số duy nhất của K được chứa trong E. Mọi trường K đều tương đối đóng đại số trong chính nó. Trong § 4 chúng ta sẽ nghiên cứu các trường tương đối đóng đại số trong mỗi trường mở rộng chứa nó.

#### Mệnh đề 4 {#alg-v-s3-prop-4 .statement}

— Cho E là một mở rộng của một trường K; tập hợp L các phần tử của E là đại số trên K tạo thành một mở rộng con của E, tương đối đóng đại số trong E.

Thật vậy, trường K(L) là đại số trên K (Hệ quả 1 của Định lý 2), nên K(L) ⊂ L; suy ra K(L) = L và L là một trường. Mặt khác, nếu x ∈ E là đại số trên L, thì nó cũng là đại số trên K (Mệnh đề 3) và do đó thuộc về L.

Mở rộng L của K gồm tất cả các phần tử của E là đại số trên K được gọi là bao đóng đại số tương đối của K trong E; đó là mở rộng đại số lớn nhất của K được chứa trong E.

### Bài tập {#alg-v-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
