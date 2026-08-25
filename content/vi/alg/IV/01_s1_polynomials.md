---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 1
section_title: Polynomials
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0010-0023, 0095-0096
extraction: ocr
subsections:
    - "no": 1
      title: Definition of polynomials
      page: 0
      pdf_page: 10
    - "no": 2
      title: Degrees
      page: 2
      pdf_page: 11
    - "no": 3
      title: Substitutions
      page: 4
      pdf_page: 13
    - "no": 4
      title: Differentials and derivations
      page: 6
      pdf_page: 15
    - "no": 5
      title: Divisors of zero in a polynomial ring
      page: 9
      pdf_page: 18
    - "no": 6
      title: Euclidean division of polynomials in one indeterminate
      page: 10
      pdf_page: 19
    - "no": 7
      title: Divisibility of polynomials in one indeterminate [^1]
      page: 11
      pdf_page: 20
    - "no": 8
      title: Irreducible polynomials
      page: 13
      pdf_page: 22
statements: 30
exercises: 5
content_sha256: 14afa86d0da6a7349449843772660bf456c15e929b49453f0952672423538d99
translated_from: content/en/alg/IV/01_s1_polynomials.md
source_content_sha256: 680d2b1dc0057e134cacc841defea4521163184e80d9745b8d469153561a213f
translation_model: gpt-5-6-mini
translation_run: translate-vi-df5a3f08
glossary_version: 34
glossary_terms_sha256: 58b667d804ab953d266e51e939824215cfb47d912a977972d07a0394d9abad46
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐA THỨC

### 1. Định nghĩa đa thức

Cho $ I $ là một tập hợp. Ta nhắc lại (III, p. 452) rằng đại số giao hoán tự do trên $ I $ trên $ \mathbf{A} $ được ký hiệu bởi $ \mathbf{A}[(X_i)_{i \in I}] $ hoặc $ \mathbf{A}[X_i]_{i \in I} $. Các phần tử của đại số này được gọi là *đa thức* theo các bất định $ X_i $ (hoặc theo các bất định $ X_i $) với các hệ số trong $ \mathbf{A} $. Ta nhắc lại rằng bất định $ X_i $ là ảnh chính tắc của $ i $ trong đại số giao hoán tự do trên $ I $ trên $ \mathbf{A} $; đôi khi thuận tiện khi ký hiệu ảnh này bằng một ký hiệu khác như $ X'_i, Y_i, T_i $, v.v. Quy ước này thường được đưa vào bằng một câu như: « Cho $ Y = (Y_i)_{i \in I} $ là một họ các bất định »; trong trường hợp này đại số các đa thức được xét được ký hiệu bởi $ \mathbf{A}[Y] $. Khi $ I = \{1, 2, \ldots, n\} $, người ta viết $ \mathbf{A}[X_1, X_2, \ldots, X_n] $ thay cho $ \mathbf{A}[(X_i)_{i \in I}] $.

Với $ \nu \in \mathbf{N}^{(I)} $ ta đặt

$$
X^\nu = \prod_{i \in I} X_i^{\nu_i}.
$$

Khi đó $ (X^\nu)_{\nu \in \mathbf{N}^{(I)}} $ là một cơ sở của $ \mathbf{A} $-môđun $ \mathbf{A}[(X_i)_{i \in I}] $. Các $ X^\nu $ được gọi là *đơn thức* theo các bất định $ X_i $. Với $ \nu = 0 $ ta thu được phần tử đơn vị của $ \mathbf{A}[(X_i)_{i \in I}] $. Mọi đa thức $ u \in \mathbf{A}[(X_i)_{i \in I}] $ đều có thể được viết theo đúng một cách dưới dạng

$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$

trong đó $ a_\nu \in \mathbf{A} $ và các $ \alpha_\nu $ đều bằng không trừ một số hữu hạn; các $ a_\nu $ được gọi là *các hệ số* của $ u $; các $ \alpha_\nu X^\nu $ được gọi là *các số hạng* của $ u $ (thường phần tử $ \alpha_\nu X^\nu $ được gọi là số hạng theo $ X^\nu $), đặc biệt số hạng $ \alpha_0 X^0 $, đồng nhất với $ a_0 $, được gọi là *số hạng hằng* của $ u $. Khi $ \alpha_\nu = 0 $, theo lối nói lạm dụng, ta nói rằng $ u $ *không chứa phần tử* theo $ X^\nu $; đặc biệt khi $ \alpha_0 = 0 $, ta nói rằng $ u $ là một đa thức *không có số hạng hằng* (III, p. 453). Mọi bội vô hướng của 1 đều được gọi là một *đa thức hằng*.

Cho B là một vành giao hoán và $ \rho : A \to B $ là một đồng cấu vành. Ta xem $ B[(X_i)_{i \in I}] $ như một đại số trên A nhờ $ \rho $. Như vậy ánh xạ $ \sigma $ từ $ A[(X_i)_{i \in I}] $ vào $ B[(X_i)_{i \in I}] $ biến đổi $ \sum \alpha_v X^\nu $ thành $ \sum \rho(\alpha_v) X^\nu $ là một đồng cấu các đại số trên A; nếu $ u \in A[(X_i)_{i \in I}] $, đôi khi ta ký hiệu ảnh của $ u $ qua đồng cấu này là $ ^\rho u $. Đồng cấu từ $ B \otimes_A A[(X_i)_{i \in I}] $ vào $ B[(X_i)_{i \in I}] $ được xác định một cách chính tắc bởi $ \sigma $ biến, với mọi $ i \in I $, $ 1 \otimes X_i $ thành $ X_i $; đây là một đẳng cấu các đại số trên B (III, p. 449).

Cho M là một A-môđun tự do với cơ sở $ (e_i)_{i \in I} $. Tồn tại chính xác một đồng cấu có đơn vị $ \varphi $ từ đại số đối xứng $ S(M) $ vào đại số $ A[(X_i)_{i \in I}] $ sao cho $ \varphi(e_i) = X_i $ với mỗi $ i \in I $, và đồng cấu này là một đẳng cấu (III, p. 506). Đẳng cấu này được gọi là chính tắc. Nó cho phép ta áp dụng cho các đại số đa thức một số tính chất của các đại số đối xứng. Ví dụ, cho $ (I_1), \ldots, L $ là một phân hoạch của I. Gọi $ \varphi_\lambda $ là đồng cấu từ $ P_\lambda = A[(X_i)_{i \in I_\lambda}] $ vào $ P = A[(X_i)_{i \in I}] $ biến đổi $ X_i $ (với tư cách là phần tử của $ P_\lambda $) thành $ X_i $ (với tư cách là phần tử của P). Khi đó các $ \varphi_\lambda $ xác định một đồng cấu của đại số $ \bigotimes_{h \in L} P_\lambda $ vào đại số P, và đồng cấu này là một đẳng cấu (III, p. 503, Mệnh đề 9).

Cho E là một A-môđun, và đặt $ E \otimes_A A[(X_i)_{i \in I}] = E[(X_i)_{i \in I}] $. Các phần tử của A-môđun $ E[(X_i)_{i \in I}] $ được gọi là các đa thức theo các bất định $ X_i $ với hệ số trong E. Một đa thức như vậy có thể được viết theo đúng một cách dưới dạng $ \sum_{v \in \mathbf{N}^{(I)}} e_v \otimes X^\nu $, trong đó $ e_v \in E $ và các $ e_v $ bằng không với tất cả trừ một số hữu hạn các chỉ số; ta thường viết $ e_v X^\nu $ thay cho $ e_v \otimes X^\nu $.

### 2. Bậc

Cho $ P = A[(X_i)_{i \in I}] $ là một đại số đa thức. Với mỗi số nguyên $ n \in \mathbf{N} $, gọi $ P_n $ là môđun con của P sinh bởi các đơn thức $ X^\nu $ sao cho $ |\nu| = \sum_{i \in I} \nu_i $ bằng n. Khi đó $ (P_n), \ldots $ là một phép phân bậc biến $ A[(X_i)_{i \in I}] $ thành một đại số phân bậc kiểu $ \mathbf{N} $ (III, p. 459). Các phần tử thuần nhất bậc $ n $ trong $ A[(X_i)_{i \in I}] $ đôi khi được gọi là các dạng bậc $ n $ đối với các bất định $ X_i $.

Khi xét bậc của các đa thức không thuần nhất, ta quy ước thêm vào tập hợp $ \mathbf{N} $ các số tự nhiên một phần tử được viết là $ -\infty $ và mở rộng quan hệ thứ tự và phép cộng của $ \mathbf{N} $ lên $ \mathbf{N} \cup \{-\infty\} $ theo các quy ước sau, trong đó $ n \in \mathbf{N} $,

$$
-\infty < n , \quad (-\infty) + n = n + (-\infty) = -\infty , \quad (-\infty) + (-\infty) = -\infty .
$$

Cho $ u = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^\nu $ là một đa thức. Thành phần thuần nhất $ u_n $ bậc n của $ u $ (đối với phân hoạch kiểu N được định nghĩa ở trên) bằng $ \sum_{|\nu|=n} \alpha_\nu X^\nu $, và ta rõ ràng có $ u = \sum_{n \in \mathbf{N}} u_n $. Nếu $ u \neq 0 $, các $ u_n $ không phải tất cả đều bằng không, và ta định nghĩa *bậc* (hay *bậc toàn phần*) của $ u $, ký hiệu là $ \deg u $, là lớn nhất trong các số $ n $ sao cho $ u_n \neq 0 $; nói cách khác (III, p. 453), bậc của $ u $ là lớn nhất trong các số nguyên $ |\nu| $ đối với các đa chỉ số $ \nu $ sao cho $ a_\nu \neq 0 $. Khi $ u = 0 $, theo quy ước bậc của $ u $ là $ -\infty $. Với mọi số nguyên $ p \in \mathbf{N} $, quan hệ $ \deg u \leq p $ do đó tương đương với « $ a_\nu = 0 $ với mọi đa chỉ số $ \nu $ có $ |\nu| > p $ »; tập hợp các đa thức $ u $ sao cho $ \deg u \leq p $ do đó là một A-môđun con của $ A[(X_i)_{i \in I}] $, bằng $ P_0 + P_1 + \ldots + P_p $ với các ký hiệu ở trên.

Cho E là một A-môđun. Họ $ (E \otimes P_n)_{n \in \mathbf{N}} $ là một phân hoạch kiểu N của môđun $ E[(X_i)_{i \in I}] = E \otimes_A A[(X_i)_{i \in I}] $ các đa thức có hệ số trong E. Ta mở rộng cho trường hợp này các quy ước đã được chấp nhận ở trên về bậc của các đa thức không thuần nhất.

#### Mệnh đề 1 {#alg-iv-s1-prop-1 .statement}

*Cho $ u $ và $ v $ là hai đa thức.*

(i) Nếu $ \deg u \neq \deg v $, *ta có*
$$
u + v \neq 0 \quad \text{và} \quad \deg(u + v) = \sup(\deg u, \deg v).
$$
Nếu $ \deg u = \deg v $ *ta có* $ \deg(u + v) \leq \deg u $.

(ii) *Ta có* $ \deg(uv) \leq \deg u + \deg v $.
Chứng minh là ngay lập tức.

Cho $ J \subset I $ và $ B = A[(X_i)_{i \in I - J}] $; ta sẽ đồng nhất $ A[(X_i)_{i \in I}] $ với $ B[(X_i)_{i \in J}] $ (III, p. 453 f.). Bậc của $ u \in A[(X_i)_{i \in I}] $, với tư cách là phần tử của $ B[(X_i)_{i \in J}] $, được gọi là bậc của $ u $ đối với các $ X_i $ có chỉ số $ i \in J $ (III, p. 454).

Cho $ u = \sum_{k=0}^n a_k X^k \in A[X] $ là một đa thức khác không bậc $ n $ với một ẩn duy nhất. Hệ số $ a_n $, khác không theo giả thiết, được gọi là *hệ số dẫn* của $ u $. *Một* đa thức $ u \neq 0 $ có hệ số dẫn bằng 1 được gọi là một *đa thức đơn khởi*.

Trong $ A[X_1, X_2, \ldots, X_q] $ số các đơn thức có bậc toàn phần $ p $ bằng số các phần tử $ (n_k)_{1 \leq k \leq q} $ của $ \mathbf{N}^q $ sao cho $ \sum_{k=1}^q n_k = p $, tức là $ \binom{q+p-1}{p} $
(Sets III, Prop. 15, p. 182)

Nói chung hơn, cho $A$ là một vị nhóm giao hoán và $ (\delta_i)_{i \in I} $, một họ các phần tử của A. Có một phép phân bậc duy nhất kiểu A của đại số $ A[(X_i)_{i \in I}] $ sao cho mỗi đơn thức $ X^\nu $ có bậc $ \sum_{i \in I} \nu_i \delta_i $ (III, p. 458, ví dụ 3). Trường hợp được xét ở trên là trường hợp $ A = \mathbf{N} $ và $ \delta_i = 1 $. Trong trường hợp tổng quát, để tránh nhầm lẫn, ta sẽ dùng từ « trọng số » thay cho « bậc » và « đẳng trọng » thay cho « thuần nhất ». Chẳng hạn, có một phép phân bậc duy nhất kiểu N của đại số $ A[(X_i)_{i \geq 1}] $ sao cho $ X_i $ có trọng số $ i $ với mỗi số nguyên $ i \geq 1 $. Các phần tử đẳng trọng trọng số $ n $ là các đa thức có dạng $ \sum a_{\nu} X^{\nu} $, trong đó $ a_{\nu} = 0 $ với $ \sum_{i \geq 1} i \cdot \nu_i \neq n $.

### 3. Phép thế

Cho E là một đại số kết hợp có đơn vị trên $ \mathcal{A} $ và $ x = (x_i)_{i \in I} $ là một họ các phần tử từng đôi một hoán vị được của E. Cho $ X = (X_i)_{i \in I} $ là một họ các bất định. Theo III, Mệnh đề 7, p. 449, tồn tại một đồng cấu có đơn vị duy nhất $ f $ của $ \mathcal{A}[X] $ vào $ E $ sao cho $ f(X_i) = x_i $ với mọi $ i \in I $. Ảnh của một phần tử $ u $ của $ \mathcal{A}[X] $ qua $ f $ được viết là $ u(x) $ và được gọi là *phần tử của E thu được bằng cách thế $ x_i $ cho $ X_i $ trong $ u $*, hoặc cũng là *giá trị của $ u $ đối với $ X_i = x_i $*. Đặc biệt, $ u = u((X_i)_{i \in I}) $. Nếu $ I = \{1, \ldots, n\} $ ta viết $ u(x_1, \ldots, x_n) $ thay cho $ u((x_i)_{i \in I}) $. Tổng quát hơn, nếu M là một A-môđun và nếu o là một phần tử của

$$
M[(X_i)_{i \in I}] = M \otimes_A \mathcal{A}[(X_i)_{i \in I}],
$$

ta ký hiệu ảnh của $ v $ trong $ M \otimes_A E = M_{(E)} $ qua ánh xạ $ 1_M \otimes f $ bởi $ v(x) $.

Nếu đồng cấu $ u \mapsto u(x) $ của $ \mathcal{A}[X] $ vào E là đơn ánh, ta nói rằng họ $ x $ là *tự do đại số* trên $ \mathcal{A} $, hoặc rằng các $ x_i $ là *độc lập đại số* trên $ \mathcal{A} $. Điều này cũng có nghĩa là các đơn thức $ x^{\nu} $ ($ \nu \in \mathbf{N}^{(I)} $) độc lập tuyến tính trên $ \mathcal{A} $.

Nếu $ \lambda $ là một đồng cấu có đơn vị của E vào một đại số A-kết hợp có đơn vị E', ta có

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i)_{i \in I})) ,
$$

vì $ \lambda \circ f $ là một đồng cấu của $ \mathcal{A}[X] $ vào E' gửi $ X_i $ đến $ \lambda(x_i) $.

Cho $ u \in \mathcal{A}[X] $. Nếu $ E $ là giao hoán, ánh xạ $ x \mapsto u(x) $ từ $ E^1 $ vào E được gọi là *hàm đa thức* xác định bởi $ u $ (và đại số $ E $) ; đôi khi ta sẽ ký hiệu nó bởi $ \tilde{u} $ (hoặc thậm chí chỉ bởi $ u $).

Cho $ Y = (Y_j)_{j \in J} $ là một họ khác của các bất định, và ta lấy E là đại số đa thức $ \mathcal{A}[Y] $. Với $ u \in \mathcal{A}[X] $, lấy $ g_i \in \mathcal{A}[Y] $ với $ i \in I $ và đặt $ g = (g_i)_{i \in I} $; gọi $ u(g) \in \mathcal{A}/[Y] $ là đa thức thu được bằng cách thay các đa thức $ g_i $ vào $ X_i $ trong $ u $. Cho $ y = (y_j)_{j \in J} $ là một họ các phần tử từng đôi một hoán vị được của một đại số A-kết hợp có đơn vị $ E' $ ; áp dụng (1) và lấy đồng cấu $ g \mapsto g(y) $ của $ E $ vào $ E' $ làm $ \mathcal{A} $, ta thu được

$$
(u(g))(y) = u((g_i(y))) .
$$

Nếu $ f = (f_i)_{i \in I} \in (\mathcal{A}[(X_j)_{j \in J}])^I $ và $ g = (g_j)_{j \in J} \in (\mathcal{A}[(Y_k)_{k \in K}])^J $, ta ký hiệu bởi $ f \circ g $ hoặc $ f(g) $, họ các đa thức $ (f_i(g))_{i \in I} \in (\mathcal{A}[(Y_k)_{k \in K}])^I $. Nếu ta ký hiệu bởi $ \tilde{f} $ ánh xạ $ x \mapsto (f_i(x))_{i \in I} $ từ $ {E'}^J $ vào $ {E'}^I $ (trong đó $ E' $ là một đại số $ A $-kết hợp, giao hoán và có đơn vị), thì quan hệ (2) suy ra

$$(3)$$
$$(\mathrm{fog})'' = \tilde{f} \circ \tilde{g}.$$

Nếu $ h = (h_k)_{k \in K} \in (A[(Z_l)_l \bullet_L])^K $, từ (2) suy ra rằng :

$$(4)$$
$$f \circ (g \circ h) = (f \circ g) \circ h.$$

#### Mệnh đề 2 {#alg-iv-s1-prop-2 .statement}

*Cho $ a = (a_i)_{i \in I} $, là một họ các phần tử của $ A $ và cho $ u \in A[X] $. Nếu $ v $ là đa thức thu được bằng cách thay $ X_i + a_i $ cho $ X_i $ với mỗi $ i \in I $, thì số hạng hằng của $ v $ bằng $ u(a) $.*

Số hạng hằng của $ v $ thu được bằng cách thay 0 cho $ X_i $ trong $ v $ với mỗi $ i \in I $. Do đó kết quả suy ra từ (2).

#### Hệ quả 1 {#alg-iv-s1-prop-2-cor-1 .statement}

*Cho $ m $ là iđêan của các đa thức $ u \in A[X] $ sao cho $ u(a) = 0 $. Khi đó $ m $ được sinh bởi các đa thức $ X_i - a_i $ (với $ i \in I $).*

Hiển nhiên là $ X_i - a_i \in m $ với mỗi $ i \in I $. Cho $ u \in m $ và cho $ v $ như trong Mệnh đề 2. Vì $ v $ không có số hạng hằng, tồn tại một họ $ (P_i)_{i \in I} $, gồm các đa thức trong $ A[X] $ có giá hữu hạn sao cho

$$
v(X) = \sum_{i \in I} X_i \cdot P_i(X).
$$

Nếu ta thay $ X_i $ bởi $ X_i - a_i $ với mỗi $ i \in I $ trong phương trình trên, ta thu được một quan hệ dạng $ u(X) = \sum_{i \in I} (X_i - a_i) \cdot P'_i(X) $, do đó có hệ quả.

#### Hệ quả 2 {#alg-iv-s1-prop-2-cor-2 .statement}

*Cho $ X = (X_i)_{i \in I} $ và $ Y = (Y_i)_{i \in I} $ là hai họ các phần tử bất định. Tập hợp các đa thức $ u \in A[X,Y] $ sao cho $ u(X,X) = 0 $ là iđêan của $ A[X,Y] $ sinh bởi các đa thức $ X_i - Y_i $ (với $ i \in I $).*

Hệ quả này suy ra trực tiếp từ Hệ quả 1 bằng cách thay $ A $ bởi $ A[Y] $ và $ a_i $ bởi $ Y_i $, hiểu $ A[X,Y] $ như vành đa thức theo các $ X_i $ với các hệ số trong $ A[Y] $.

#### Mệnh đề 3 {#alg-iv-s1-prop-3 .statement}

*Cho $ u \in A[X] $ và cho $ X.Z $ là họ $ (X_iZ)_{i \in I} $, gồm các phần tử của vành đa thức $ A[X][Z] $. Hệ số của $ Z^k $ trong $ u(X.Z) $ là thành phần thuần nhất bậc $ k $ của $ u $, với mọi số nguyên dương $ k $.*

Chỉ cần chứng minh Mệnh đề này trong trường hợp $ u $ là một đơn thức, và trong trường hợp này kết quả là hiển nhiên.

#### Hệ quả {#alg-iv-s1-n3-cor-1 .statement}

*Để một đa thức $ u \in A[X] $ là thuần nhất bậc $ k $ thì điều kiện cần và đủ là :*

$$
u(X.Z) = u(X) \cdot Z^k.
$$

#### Nhận xét {#alg-iv-s1-n3-rem-1 .statement}

— Cho $ x \in A^I $ và cho $ f $ là ánh xạ $ u \mapsto u(x) $ từ $ A[X] $ vào $ A $. Cho một $ A $-môđun $ M $, ta xét đồng cấu $ 1 \otimes f $ của $ M[X] = M \otimes_A A[X] $ vào $ M \otimes_A A = M $. Với mỗi $ v \in M[X] $ ta có $ (1 \otimes f)(v) = v(x) $. Nếu $ v = \sum_{\nu \in \mathbf{N}^{(l)}} e_\nu X^\nu $, thì $ v(x) = \sum_{\nu \in \mathbf{N}^{(l)}} x^\nu e_\nu $.

### 4. Vi phân và đạo hàm

Cho $ B = A[(X_i)_{i \in I}] $, theo III, p. 569 với mỗi $ i \in I $ tồn tại duy nhất một A-đạo hàm $ D_i $ của B sao cho
$$
D_i X_i = 1 , \quad D_i X_j = 0 \quad \text{đối với} \quad j \neq i
$$
Đa thức $ D_i P $ được gọi là *đạo hàm riêng* của $ P $ *theo* $ X_i $; ta cũng ký hiệu nó bởi $ D_{X_i} P $ hoặc $ \frac{\partial P}{\partial X_i} $ hoặc $ P'_{X_i} $. Theo III, p. 558, công thức (21), ta có, với $ \nu = (\nu,) \in \mathbf{N}^{(l)} $,
$$
D_i (X^\nu) = \begin{cases}
\nu_i X_i^{\nu_i - 1} \prod_{j \in I - \{i\}} X_j^{\nu_j} & \text{nếu } \nu_i > 0 \\
0 & \text{nếu } \nu_i = 0
\end{cases}
$$
Từ (6) suy ra $ D_i D_j = D_j D_i $ với mọi $ i, j \in I $. Với $ \nu = (\nu_i)_{i \in I} \in \mathbf{N}^{(l)} $ ta đặt $ D^\nu = \prod_{i \in I} D_i^{\nu_i} $ và $ \nu! = \prod_{i \in I} (\nu_i!) $. Với thứ tự tích trên $ \mathbf{N}^{(l)} $ ta có
$$
D^\nu(X^\mu) = \begin{cases}
\frac{\mu!}{(\mu - \nu)!} X^{\mu - \nu} & \text{nếu } \nu \leq \mu , \\
0 & \text{nếu không .}
\end{cases}
$$
Khi $ P $ là một đa thức theo một bất định duy nhất $ X $, đạo hàm riêng duy nhất của $ P $ được viết là $ DP $ hoặc $ \frac{dP}{dX} $ hoặc $ P' $ và được gọi đơn giản là *đạo hàm* của $ P $.

Lại cho $ B = A[(X_i)_{i \in I}] $; theo III, p. 569, B-môđun các vi phân A của $ B $, $ \Omega_A(B) $, có họ $ (dX_i)_{i,} $, các vi phân của các $ X_i $ làm cơ sở. Gọi $ \partial_i $ là dạng tọa độ của chỉ số $ i $ đối với cơ sở này trên $ \Omega_A(B) $. Khi đó ánh xạ $ u \mapsto (\partial_i, du) $ từ B vào chính nó là một đạo hàm của B, biến $ X_i $ thành 1 và $ X_j $ thành 0 với $ j \neq i $, và do đó là $ D_i $; nói cách khác, ta có
$$
du = \sum_{i \in I} (D_i u) dX_i
$$
với mỗi $ u \in B $. Nếu I hữu hạn, $ (D_i)_{i \in I} $ là một cơ sở của B-môđun các đạo hàm của B.

#### Mệnh đề 4 {#alg-iv-s1-prop-4 .statement}

*Cho E là một A-đại số kết hợp, giao hoán và có đơn vị, $ x = (x_i)_{i \in I} $ là một họ các phần tử của E, u là một phần tử của $ A[(X_i)_{i,}] $ và $ y = u(x) $. Khi đó với mọi đạo hàm D của E vào một E-môđun ta có*
$$
Dy = \sum_{i \in I} (D_i u)(x) \cdot Dx_i .
$$

Chỉ cần chứng minh mệnh đề khi $ u $ là một đơn thức, và trong trường hợp đó điều này suy ra từ III, p. 558, Mệnh đề 6.

#### Hệ quả {#alg-iv-s1-n4-cor-1 .statement}

— *Cho $ f \in A[X_1, ..., X_p] $ và $ g_i \in A[Y_1, ..., Y_q] $ với $ 1 \leq i \leq p $, và đặt $ h = f(g_1, ..., g_p) $, khi đó với $ 1 \leq j \leq q $ ta có*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j}.
$$

Đây là trường hợp đặc biệt $ E = A[Y_1, ..., Y_r] $, $ x_i = g_i $ và $ D = \partial / \partial Y_j $ của Mệnh đề 4.

Cho $ X = (X_i)_{i \in I} $, $ Y = (Y_i)_{i \in I} $ là hai họ biến bất định rời nhau, và viết $ X + Y $ cho họ $ (X_i + Y_i)_{i \in I} $. Cho $ u \in A[X] $, xét phần tử $ u(X + Y) $ của $ A[X, Y] $. Với $ \nu \in \mathbf{N}^{(I)} $ ta ký hiệu $ A^\nu u $ là hệ số của $ Y_\nu $ trong $ u(X + Y) $, được xem như đa thức theo các $ Y_i $ với các hệ số thuộc $ A[X] $. Theo định nghĩa ta có $ A^\nu u \in A[X] $ và

$$
u(X + Y) = \sum_\nu (\Delta^\nu u)(X) Y^\nu.
$$

(Ở đây và trong phần còn lại của No. này, các tổng được lấy trên tập hợp chỉ số $ \mathbf{N}^{(I)} $ trừ khi có nói khác.)

Cho $ a \in A' $, khi thay $ a $ cho $ X $ và $ X - a $ cho $ Y $ trong (9), ta được

$$
u(X) = \sum_\nu (\Delta^\nu u)(a)(X - a)^\nu.
$$

Đặc biệt ta có

$$
u(X) = \sum_\nu (\Delta^\nu u)(0) X^\nu.
$$

Nếu $ u, v \in A[X] $, ta có

$$
(uv)(X + Y) = \left( \sum_\nu (\Delta^\nu u)(X) Y^\nu \right) \left( \sum_\rho (\Delta^\rho v)(X) Y^\rho \right)
= \sum_\sigma \left[ \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(X)(\Delta^\rho v)(X) \right] Y^\sigma
$$

suy ra

$$
\Delta^\sigma(uv) = \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(\Delta^\rho v).
$$

Cho $ Z = (Z_i)_{i \in I} $ là một họ biến bất định khác.

Ta có:

$$
\sum_{\nu} (\Delta^\nu u)(\mathbf{X})(\mathbf{Y} + \mathbf{Z})^\nu = u(\mathbf{X} + \mathbf{Y} + \mathbf{Z})
$$
$$
= \sum_{\sigma} (Au u)(\mathbf{X} + \mathbf{Y})Zu
$$
$$
= \sum_{\rho, \sigma} (\Delta^\rho \Delta^\sigma u)(\mathbf{X}) Y^\rho Z^\sigma u,
$$

suy ra theo I, p. 99, Hệ quả 2:

(13)
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u.
$$

#### Mệnh đề 5 {#alg-iv-s1-prop-5 .statement}

— *Với mọi* $ u \in \mathbf{A}[\mathbf{X}] $ *và* $ \nu \in \mathbf{N}^{(I)} $ *ta có*

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

Trước hết, giả sử $ \nu $ có độ dài 1 ; khi đó tồn tại một phần tử $ i $ của I sao cho $ \nu = \varepsilon_i $, tức là $ \nu_i = 1 $ và $ \nu_j = 0 $ với mọi $ j \neq i $ trong I. Công thức (12) cho thấy $ A'' $ là một đạo hàm của đại số trên A $ \mathbf{A}[\mathbf{X}] $, rõ ràng nhận giá trị không trên $ X_j $ với $ j \neq i $ và giá trị 1 trên $ X_i $. Do đó ta có $ \Delta^{\varepsilon_i} = D_i $ với mỗi $ i \in I $.

Theo (13) ta có

(14)
$$
(\rho! \; \Delta^\rho) \cdot (\sigma! \; \Delta^\sigma) = (\rho + \sigma)! \; \Delta^{\rho + \sigma}
$$

trong đại số tự đồng cấu của A-môđun $ \mathbf{A}[\mathbf{X}] $. Bây giờ suy ra bằng quy nạp theo độ dài của $ \nu $ rằng $ \nu! \; A'' = D^\nu $.

Nếu $ \mathbf{A} $ là một Q-đại số, các công thức (9), (10), (11) do đó có thể được viết

(15)
$$
u(\mathbf{X} + \mathbf{Y}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(\mathbf{X}) \mathbf{Y}^\nu
$$
(16)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(a)(\mathbf{X} - a)^\nu
$$
(17)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(0) \; X^\nu
$$

Cả ba công thức (15), (16), (17) đều được gọi là « công thức Taylor ».

#### Mệnh đề 6 (*« đồng nhất thức Euler »*) {#alg-iv-s1-prop-6 .statement}

— *Cho* $ u \in \mathbf{A}[\mathbf{X}] $ *là một đa thức thuần nhất bậc r ; ta có*

$$
\sum_{i \in I} X_i \cdot D_i u = ru.
$$

Gọi D là ánh xạ A-tuyến tính từ $ A[X] $ vào chính nó sao cho $ D(v) = sv $ khi v thuần nhất bậc s. Ta biết (III, p. 554, Ví dụ 6) rằng D là một đạo hàm của $ A[X] $. Do đó Mệnh đề 6 là một Hệ quả của Mệnh đề 4 (IV, p. 6).

### 5. Các ước của không trong một vành đa thức

#### Mệnh đề 7 {#alg-iv-s1-prop-7 .statement}

— *Cho $ f \in A[X] $ là một đa thức khác không theo một bất định và $ a $ là hệ số dẫn đầu của nó. Nếu $ a $ giản ước được trong A (đặc biệt là khi và chỉ khi nó đơn nhất) thì với mọi phần tử khác không'g của $ A[X] $, ta có*

$$
fg \neq 0 \quad \text{and} \quad \deg(fg) = \deg f + \deg g
$$

Cho $ g \in A[X] $ là một đa thức khác không, $ \beta $ là hệ số dẫn đầu của nó, $ n = \deg f $ và $ p = \deg g $. Hệ số của $ X^{n+p} $ trong $ fg $ là $ \alpha \beta $, khác không, do đó có mệnh đề.

#### Mệnh đề 8 {#alg-iv-s1-prop-8 .statement}

— *Nếu A là một miền nguyên, thì $ A[(X_i)_{i \in I}] $ cũng là một miền nguyên.*

Cho $ u, v $ là hai phần tử khác không của $ A[(X_i)_{i \in I}] $; ta phải chứng minh rằng $ uv \neq 0 $. Khi đó $ u $ và $ v $ thuộc một vành $ A[(X_j)_{j \in J}] $, trong đó J là một tập con hữu hạn của I. Do đó ta có thể giới hạn về trường hợp I là hữu hạn và bằng $ \{1, 2, ..., p\} $. Mặt khác, vành $ A[X_1, ..., X_p] $ đẳng cấu với vành đa thức theo $ X_p $ với các hệ số trong $ A[X_1, ..., X_{p-1}] $. Bằng quy nạp theo $ p $, do đó ta quy về việc chứng minh mệnh đề đối với $ A[X] $, và lúc này chỉ cần áp dụng Mệnh đề 7.

#### Hệ quả 1 {#alg-iv-s1-prop-8-cor-1 .statement}

— *Nếu A là một miền nguyên, và $ u, v $ là các phần tử của $ A[(X_i)_{i \in I}] $, thì $ \deg(uv) = \deg u + \deg v $.*

Ta có thể giới hạn về trường hợp $ u $ và $ v $ khác không. Đặt $ m = \deg u, n = \deg v $; ta có

$$
u = u_0 + u_1 + \cdots + u_m, \quad v = v_0 + v_1 + \cdots + v_n
$$

trong đó $ u_h $ (tương ứng $ v_h $) là thành phần thuần nhất bậc $ h $ của $ u $ (tương ứng của v). Vì $ u_m \neq 0 $ và $ v_n \neq 0 $, ta có $ u_m v_n \neq 0 $ (Mệnh đề 8). Khi đó $ uv = u_m v_n + w $ với $ \deg w < m + n $, do đó có kết quả.

#### Hệ quả 2 {#alg-iv-s1-prop-8-cor-2 .statement}

— *Nếu A là một miền nguyên, các phần tử khả nghịch của $ A[(X_i)_{i \in I}] $ là các phần tử khả nghịch của A.*

Điều này có ngay lập tức từ Hệ quả 1.

#### Mệnh đề 9 {#alg-iv-s1-prop-9 .statement}

— *Cho $ u \in A[(X_i)_{i \in I}] $; để u lũy linh trong vành $ A[(X_i)_{i \in I}] $, điều kiện cần và đủ là mọi hệ số của nó đều lũy linh trong vành A.*

Như trong chứng minh của Mệnh đề 8, ta có thể quy về trường hợp các đa thức theo một biến X. Nếu mọi hệ số của $ u $ đều lũy linh, thì $ u $ lũy linh (I, p. 99, Hệ quả 1). Giả sử $ u $ lũy linh nhưng khác không và gọi $ n $ là bậc của nó; ta sẽ lập luận bằng quy nạp theo $ n $. Gọi $ a $ là hệ số dẫn đầu của $ u $. Tồn tại một số nguyên $ m > 0 $ sao cho $ u^m = 0 $. Hệ số dẫn đầu của $ u^m $ là $ a^m $, do đó $ a^m = 0 $. Khi đó $ u - \alpha X^n $ là lũy linh (I, loc. cit.) và giả thiết quy nạp cho thấy mọi hệ số của $ u - \alpha X^n $ đều lũy linh. Do đó mọi hệ số của $ u $ đều lũy linh.

#### Nhận xét {#alg-iv-s1-n5-rem-1 .statement}

Cho $ u $ và $ v $ là các phần tử của $ A[(X_i)_i \in ,] $, và giả sử rằng $ A $ là một miền nguyên, $ v $ là một bội khác không của $ u $ và $ v $ thuần nhất; khi đó $ u $ cũng thuần nhất. Thật vậy, lấy $ u' \in A[(X_i)_i ,_1] $ sao cho $ v = uu' $; ta có $ u \neq 0 $, $ u' \neq 0 $, và nếu
$$
u = u_h + u_{h+1} + \cdots + u_k \\
u' = u_{h'} + u_{h'+1} + \cdots + u_{k'}
$$
là các phân tích của $ u $ và $ u' $ thành các thành phần thuần nhất, với $ u_h \neq 0 $, $ u_k \neq 0 $, $ u_{h'} \neq 0 $, $ u_{k'} \neq 0 $, thì $ v = u_h u_{h'} + u_h u_{h'+1} + \ldots + u_k u_{k'} $ và $ u_h u_{h'} $ là phần tử thuần nhất khác không có bậc $ h + h' $ trong khi $ u_k u_{k'} $ là phần tử thuần nhất khác không có bậc $ k + k' $ (Mệnh đề 8). Vì $ v $ thuần nhất, ta có $ h + h' = k + k' $ do đó $ h = k $, $ h' = k' $.

### 6. Phép chia Euclid các đa thức theo một bất định

#### Mệnh đề 10 {#alg-iv-s1-prop-10 .statement}

*Cho $ f $ và $ g $ là các phần tử khác không của $ A[X] $ có bậc lần lượt là $ m $ và $ n $. Gọi $ \alpha_0 $ là hệ số dẫn đầu của $ f $ và $ \mu = \sup(n - m + 1, 0) $. Tồn tại $ u, v \in A[X] $ sao cho*
$$
\alpha_0^\mu g = uf + v, \quad \deg v < m.
$$
*Nếu $ \alpha_0 $ giản ước được trong $ A $, thì $ u $ và $ v $ được xác định duy nhất bởi các tính chất này.*

Sự tồn tại của $ u $ và $ v $ là rõ ràng khi $ n < m $, vì khi đó ta có thể lấy $ u = 0 $ và $ v = g $. Với $ n \geq m $ ta sẽ dùng quy nạp theo $ n $. Gọi $ \beta $ là hệ số dẫn đầu của $ g $; nếu $ f = \sum_{k=0}^m \alpha_k X^{m-k} $, ta có thể viết $ \alpha_0^\mu g = \alpha_0^\mu \beta X^n \cdot f + \alpha_0^{\mu-1} g_1 $, trong đó $ g_1 \in A[X] $ và $ \deg g_1 < n $. Theo giả thiết quy nạp tồn tại $ u_1, v \in A[X] $ sao cho $ \alpha_0^{\mu-1} g_1 = u_1 f + v $ và $ \deg v < m $. Do đó
$$
\alpha_0^\mu g = (\alpha_0^{\mu-1} \beta X^{n-m} + u_1) f + v
$$
và chỉ cần đặt $ u = \alpha_0^{\mu-1} \beta X^{n-m} + u_1 $.

Giả sử $ \alpha_0 $ là giản ước được trong $ A $, bây giờ chứng minh tính duy nhất của $ u $ và $ v $. Cho $ u, v, u_1, v_1 \in A[X] $ là sao cho
$$
\alpha_0^\mu g = uf + v = u_1 f + v_1, \quad \deg v < m, \quad \deg v_1 < m
$$

Ta có $(u - u_1) f = v_1 - v$ và $\deg(v_1 - v) < m$, do đó $u - u_1 = 0$ (IV, p. 9, Mệnh đề 7) và vì vậy $v_1 - v = 0$.

#### Hệ quả (« Phép chia Euclid của các đa thức ») {#alg-iv-s1-n6-cor-1 .statement}

— Cho $f$ là một phần tử khác không của $A[X]$ có *hệ số* đầu là khả nghịch và $m = \deg f$.
(i) Với mọi $g \in A[X]$ tồn tại $u,\ v \in A[X]$ sao *cho*
$$
g = uf + v , \quad \deg v < m .
$$
Hơn nữa, các điều kiện này xác định $u$ và $v$ duy nhất.
(ii) Các môđun con của $A[X]$, $A + AX + \ldots + AX^{m-1}$ và $fA[X]$, là bù nhau trong $A[X]$.
(iii) Giả sử $f$ không hằng và xét $A[X]$ như một $A[T]$-*môđun* nhờ đồng cấu $u(T) \mapsto u(f(X))$ của $A[T]$ vào $A[X]$. Khi đó $A[X]$ là một $A[T]$-*môđun* tự do với cơ sở $(1, X, \ldots, X^{m-1})$.
Các mệnh đề (i) và (ii) là những hệ quả ngay lập tức của Mệnh đề 10.
Ta chứng minh (iii). Gọi $\psi$ là đồng cấu $v \mapsto v(f(X), X)$ của $A[T, X]$ vào $A[X]$. Trước hết xét $A[T, X]$ như một vành đa thức theo $T$ với các hệ số trong $A[X]$; Hệ quả 1 của IV, p. 5 chỉ ra rằng hạt nhân $a$ của $\psi$ là iđêan $(T - f(X))$ của $A[T, X]$. Bây giờ xét $A[T, X]$ như một vành đa thức theo $X$ với các hệ số trong $A[T]$; khi đó $\psi$ là một ánh xạ tuyến tính $A[T]$ của $A[T][X]$ vào $A[X]$. Mệnh đề (ii) ở trên (được áp dụng cho đa thức $f(X) - T$ theo $X$ với các hệ số trong $A[T]$) chỉ ra rằng $(1, X, \ldots, X^{m-1})$ là một cơ sở của một môđun con $A[T]$ của $A[T, X]$ bù với $a$. Vì $\psi(X^i) = X^i$ với mọi số nguyên $i \geq 0$, (iii) suy ra ngay lập tức.

Với các ký hiệu của (i), ta sẽ nói rằng $u$ là thương và $v$ là phần dư trong phép chia Euclid của $g$ cho $f$; để phần dư triệt tiêu thì điều kiện cần và đủ là $f$ chia hết $g$.

### 7. Tính chia hết của các đa thức theo một bất định [^1]

#### Mệnh đề 11 {#alg-iv-s1-prop-11 .statement}

— Cho $K$ là một *trường* giao hoán.
(i) Với mọi iđêan khác không $a$ của $K[X]$ tồn tại chính xác một đa thức *đơn khởi* $f$ trong $K[X]$ sao cho $a = (f )$.
(ii) Cho $f_1$ và $f_2$ thuộc $K[X]$; để $(f,) = (f_2)$ đúng thì điều kiện cần và đủ là tồn tại một phần tử khác không $\lambda$ của $K$ sao cho $f_2 = \lambda f_1$.
Ta hãy chứng minh (ii), tính đủ của điều kiện đã nêu là rõ ràng. Trường hợp $f_1$ và $f_2$ sinh ra iđêan không là tầm thường. Do đó giả sử rằng các đa thức khác không $f_1$ và $f_2$ sinh ra cùng một iđêan của $K[X]$. Khi đó tồn tại các đa thức $u_1$ và $u_2$ sao cho $f_1 = u_1 f_2$ và $f_2 = u_2 f_1$; do đó $u_1 u_2 = 1$, từ đó $ \deg u_1 + \deg u_2 = 0 $ và vì vậy $ \deg u_2 = 0 $. Như vậy ta đã chứng minh rằng $ u_2 $ là một phần tử khác không của $ K $.

Để chứng minh (i), cho $ f $ là một đa thức đơn khởi trong $ a $ có bậc nhỏ nhất có thể. Với $ g $ thuộc $ a $, gọi $ u $ và $ v $ là thương và phần dư của phép chia Euclid của $ g $ cho $ f $; khi đó $ v = g - u f $ thuộc $ a $ và ta có $ \deg v < \deg f $; nếu $ v $ khác không, sẽ tồn tại một phần tử khác không $ A $ của $ K $ sao cho $ \lambda v $ là đơn khởi, và vì $ \lambda v \in a $, điều này sẽ mâu thuẫn với định nghĩa của f. Do đó ta có $ a = (f) $; tính duy nhất của đa thức đơn khởi $ f $ sao cho $ a = (f) $ bây giờ suy ra từ (ii).

#### Mệnh đề 12 {#alg-iv-s1-prop-12 .statement}

*Cho $ K $ là một trường giao hoán và $ f, g $ là hai phần tử của $ K[X] $. Với mọi đa thức $ d $ trong $ K[X] $, các tính chất sau là tương đương*:

(i) *Đa thức $ d $ chia hết cho $ f $ và $ g $ và mọi đa thức chia hết cho cả $ f $ và $ g $ đều chia hết cho $ d $*.

(ii) *Đa thức $ d $ chia hết cho $ f $ và $ g $ và tồn tại hai đa thức $ u $ và $ v $ sao cho $ d = u f + v g $*.

(iii) *Quan hệ $ (d) = (f) + (g) $ đúng giữa các iđêan trong $ K[X] $*.

*Đa thức $ d $ được xác định sai khác một phép nhân với một phần tử khác không của $ K $ bởi các tính chất này. Nếu $ f $ và $ g $ không đồng thời bằng không, thì $ d \neq 0 $ và bậc của $ d $ lớn hơn hoặc bằng bậc của mọi đa thức chia hết cho cả $ f $ và $ g $*.

Khi $ f $ và $ g $ bằng không, mỗi tính chất (i) đến (iii) chỉ được thỏa mãn đối với $ d = 0 $, do đó khi ấy chúng tương đương. Từ đây về sau ta giả sử rằng $ f, g $ không đồng thời bằng 0 và ký hiệu $ a $ là iđêan $ (f) + (g) $ của $ K[X] $.

Ta nhận xét rằng đối với mọi đa thức $ u $ và $ v $ trong $ K[X] $, các tính chất $ (u) \supset (v) $ và « $ u $ chia hết cho $ v $ » là tương đương. Mệnh đề (ii) do đó tương đương với « $ (d) \supset (f) $ và $ (d) \supset (g) $ và $ d \in (f) + (g) $ », tức là (iii). Rõ ràng rằng (ii) suy ra (i). Cuối cùng giả sử rằng (i) đúng; ta có $ (d) \supset (f) $ và $ (d) \supset (g) $, do đó $ (d) \supset a $; mặt khác, theo Mđ. 11 (IV, p. 12) tồn tại một đa thức $ d_1 $ sao cho $ a = (d,) $; vì $ d_1 $ chia hết cho cả $ f $ và $ g $, nó chia hết cho $ d $ theo giả thiết, do đó $ (d) \subset a $, và cuối cùng ta có $ (d) = a $, tức là, (iii).

Các khẳng định khác của Mđ. 12 là những hệ quả ngay lập tức của Mđ. 11 áp dụng cho iđêan $ a = (f) + (g) $.

#### Định nghĩa 1 {#alg-iv-s1-def-1 .statement}

*Với ký hiệu của Mđ. 12 ta nói rằng $ d $ là một ước chung lớn nhất (viết tắt là gcd) của $ f $ và $ g $. Ta nói rằng $ f $ và $ g $ nguyên tố cùng nhau hoặc rằng $ f $ nguyên tố với $ g $ nếu $ 1 $ là một gcd của $ f $ và $ g $*.

Nói rằng $ f $ và $ g $ nguyên tố cùng nhau do đó có nghĩa là tồn tại các đa thức $ u $ và $ v $ trong $ K[X] $ sao cho $ u f + v g = 1 $.

#### Hệ quả 1 {#alg-iv-s1-def-1-cor-1 .statement}

*Cho $ d $ là một ước chung lớn nhất của $ f $ và $ g $ và $ K' $ là một trường giao hoán chứa $ K $ như trường con. Khi đó $ d $ là một ước chung lớn nhất của $ f $ và $ g $ được xem như các phần tử của $ K'[X] $*.

Điều này suy ra từ Mệnh đề 12, (iii).

#### Hệ quả 2 {#alg-iv-s1-def-1-cor-2 .statement}

— Cho d là một ước chung lớn nhất của f và g.
    (i) Nếu $ u \in K[X] $, du là một ước chung lớn nhất của fu và gu.
    (ii) Nếu $ v \in K[X] $ là một ước của f và g ($ \neq 0 $), thì $ d/v $ là một ước chung lớn nhất của $ f/v $ và $ g/v $.
    Điều này suy ra từ Mệnh đề 12, (ii).

#### Hệ quả 3 {#alg-iv-s1-def-1-cor-3 .statement}

— Cho w là một nhân tử chung của f và g. Để w là một ước chung lớn nhất của f và g thì điều kiện cần và đủ là $ f/w $ và $ g/w $ nguyên tố cùng nhau.
    Điều này suy ra từ Hệ quả 2.

#### Hệ quả 4 {#alg-iv-s1-def-1-cor-4 .statement}

— Cho $ f, g, h \in K[X] $. Nếu f chia hết cho gh và nguyên tố cùng nhau với g, thì f chia hết cho h.
    Vì f chia hết cho gh và fh, nên f chia hết cho mọi ước chung lớn nhất của gh và fh, đặc biệt là h (Hệ quả 2, (i)).

#### Hệ quả 5 {#alg-iv-s1-def-1-cor-5 .statement}

— Cho $ f, g \in K[X] $. Để f và g nguyên tố cùng nhau thì điều kiện cần và đủ là ảnh chính tắc của g trong $ K[X]/(f) $ phải khả nghịch.
    Vì điều kiện này có nghĩa là tồn tại $ u, v \in K[X] $ sao cho $ uf + vg = 1 $.

#### Hệ quả 6 {#alg-iv-s1-def-1-cor-6 .statement}

— Cho $ f, g_1, g_2, ..., g_n \in K[X] $. Nếu f nguyên tố cùng nhau với $ g_1, g_2, ..., g_n $, thì f nguyên tố cùng nhau với $ g_1g_2...g_n $.

\* HỆ QUẢ 7. — Để f và g nguyên tố cùng nhau thì điều kiện cần và đủ là chúng không có nghiệm chung trong bất kỳ mở rộng nào của K.
    Vì nếu d là một ước chung lớn nhất của f, g thì các nghiệm chung của f và g trong một mở rộng K' của K là các nghiệm của d trong K'. Khi đó hệ quả suy ra từ V, p. 21, Mệnh đề 4.

### 8. Các đa thức bất khả quy

#### Định nghĩa 2 {#alg-iv-s1-def-2 .statement}

— Cho K là một trường giao hoán. Ta nói rằng $ f \in K[X] $ là bất khả quy nếu $ \deg f \geq 1 $ và f không chia hết cho bất kỳ đa thức g nào sao cho $ 0 < \deg g < \deg f $.
    Điều này cũng tương đương với việc nói rằng $ \deg f \geq 1 $ và các ước duy nhất của f trong $ K[X] $ là các vô hướng $ \neq 0 $ và các tích của f với các vô hướng $ \neq 0 $. Vì quan hệ $ (f) \subset (g) $ có nghĩa là g chia hết cho f, ta thấy rằng các đa thức bất khả quy của $ K[X] $ cũng có thể được định nghĩa là các đa thức f sao cho iđêan $ (f) $ là cực đại (I, p. 104).

    Cho $ f, g \in K[X] $. Nếu f bất khả quy, hiển nhiên rằng hoặc f và g nguyên tố cùng nhau hoặc f chia hết cho g. Nếu f và g đều bất khả quy, thì hoặc f và g nguyên tố cùng nhau hoặc mỗi đa thức là tích của đa thức kia với một vô hướng $ \neq 0 $. Đặc biệt, hai đa thức đơn thức bất khả quy phân biệt là nguyên tố cùng nhau.

#### Mệnh đề 13 {#alg-iv-s1-prop-13 .statement}

— Cho $ \mathcal{I} $ là tập hợp các đa thức đơn thức bất khả quy trong $ K[X] $. Cho f là một phần tử khác không của $ K[X] $ và a là hệ số dẫn đầu của nó; khi đó tồn tại chính xác một họ các số nguyên dương $(v_p)_{p \in \mathcal{S}}$ có giá hữu hạn, sao cho ta có một phân tích

$$
f = \alpha \prod_{p \in \mathcal{S}} p^{v_p}.
$$

Chỉ cần chứng minh mệnh đề trong trường hợp $f$ là đơn thức, tức là khi $\alpha = 1$. Ta sẽ lập luận bằng quy nạp theo bậc n của f, trường hợp $n = 0$ là tầm thường. Giả sử khi đó rằng $n \geq 1$ và mệnh đề đã được thiết lập cho mọi đa thức có bậc $< n$.

Cho $E$ là tập hợp các đa thức đơn khởi $\neq 1$ chia hết cho $f$; ta có $f \in E$ nên $E$ không rỗng và tồn tại trong $E$ một đa thức $g$ có bậc nhỏ nhất. Rõ ràng $g$ là bất khả quy và tồn tại một đa thức đơn khởi $h$ có bậc $< n$ sao cho $f = gh$; theo giả thiết quy nạp, $h$ là tích của một họ hữu hạn các đa thức đơn khởi bất khả quy, do đó $f$ có cùng tính chất. Điều này chứng minh sự tồn tại của phân tích (18).

Bây giờ chứng minh tính duy nhất của phân tích (18). Cho $(w_p)_{p \in \mathcal{S}}$ là một họ các số nguyên dương có giá hữu hạn, sao cho $f = \prod_{p \in \mathcal{S}} p^{w_p}$. Vì $f$ có bậc $n \geq 1$, tồn tại $p \in \mathcal{S}$ sao cho $w_p > 0$; nếu $v_p = 0$, thì $f$ là tích của một họ các phần tử của $\mathcal{S}$ phân biệt với $p$, do đó nó nguyên tố cùng nhau với $p$ (IV, p. 13, Hệ quả 6), trái với việc $p$ chia hết $f$. Theo giả thiết quy nạp, đa thức $f/p$ có một phân tích duy nhất kiểu (18); do đó ta kết luận đẳng thức $w_q = v_q$ với mọi $q \in \mathbf{4}$.

Cho $f$ là một đa thức khác không trong $\mathbf{K}[X]$. Ta nói rằng $f$ không có các nhân tử bội nếu các số mũ $v_p$ trong phân tích (18) đều $\leq 1$; cũng có thể nói rằng $f$ là tích của một dãy hữu hạn các đa thức bất khả quy từng đôi một phân biệt, hoặc cũng có thể nói rằng $f$ không chia hết cho bình phương của bất kỳ đa thức không hằng nào của $\mathbf{K}[X]$.

### Bài tập {#alg-iv-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).

[^1]: Người đọc sẽ nhận thấy sự tương tự giữa các kết quả của Số này và Số tiếp theo với các tính chất chia hết của vành $Z$ các số nguyên (I, p. 112). Chúng phụ thuộc cốt yếu vào tính chất là trong các vành $Z$ và $K[X]$, mọi iđêan đều là chính, như ta sẽ thấy trong Chương VII, § 1.
