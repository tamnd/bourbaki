---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 2
section_title: Torsion modules over a principal ideal domain
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.6-A VII.14, A VII.54-A VII.59
pdf_pages: 0365-0373, 0413-0418
extraction: ocr
subsections:
    - "no": 1
      title: Modules over a product of rings
      page: 6
      pdf_page: 365
    - "no": 2
      title: Canonical decomposition of a torsion module over a principal ideal domain
      page: 7
      pdf_page: 366
    - "no": 3
      title: 'Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate'
      page: 10
      pdf_page: 369
    - "no": 4
      title: 'Applications : II. The multiplicative group of units of the integers modulo a'
      page: 12
      pdf_page: 371
statements: 16
exercises: 15
content_sha256: 6eccf2332f41cae79bc0b6fa0eeb1732c71cc44795e36dbda8ff75d4d0c8c147
translated_from: content/en/alg/VII/02_s2_torsion_modules_over_a_principal_ideal.md
source_content_sha256: 97d9eb4cdec80e2771b1c17555ea38f2de9fce79c4beef410353e551f5136a5e
translation_model: gpt-5.4
translation_run: translate-vi-a6edd116
glossary_version: 34
glossary_terms_sha256: a077c97848c4feabadcc231f1ee0a5dd5bd0b4232584a3a6b699126bdf0652ab
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. MÔĐUN XOẮN TRÊN MỘT MIỀN IĐÊAN CHÍNH

### 1. Môđun trên một tích của các vành

Cho $ A $ là một vành và $ (b_i)_{i \in I} $ là một phân tích trực tiếp của $ A $, nghĩa là (I, p. 110, Định nghĩa 7) một họ hữu hạn các iđêan hai phía của $ A $ sao cho đồng cấu tự nhiên từ $ A $ vào tích của các $ A/b_i $ là song ánh. Theo *loc. cit.*, Mệnh đề 10, tồn tại một họ $ (e_i)_{i \in I} $ các lũy đẳng trung tâm của $ A $ sao cho $ b_i = A(1 - e_i) $, $ \sum_{i \in I} e_i = 1 $ và $ e_i e_j = 0 $ với $ i \neq j $.

Với mọi $ A $-môđun trái $ M $, ký hiệu $ M_i $ là tập hợp các $ m \in M $ sao cho $ b_i m = 0 $; vì $ b_i $ là một iđêan hai phía, nên đó là một môđun con của $ M $; hơn nữa, nếu $ a, b \in A $ và $ a - b \in b_i $, thì các phép vị tự $ a_{M_i} $ và $ b_{M_i} $ trùng nhau; do đó tồn tại một cấu trúc $ (A/b_i) $-môđun duy nhất trên $ M_i $ sao cho cấu trúc $ A $-môđun của $ M_i $ được cảm sinh qua đồng cấu $ A \to A/b_i $.

#### Mệnh đề 1 {#alg-vii-s2-prop-1 .statement}

$ A $-môđun $ M $ là tổng trực tiếp của các môđun con $ M_i $ của nó.

Gọi $ p_i : M \to M $ là phép vị tự $ m \mapsto e_i m $; ánh xạ $ p_i $ là $ A $-tuyến tính vì $ e_i $ là trung tâm; vì $ e_i^2 = e_i $, $ \sum_{i \in I} e_i = 1 $ và $ e_i e_j = 0 $ với $ i \neq j $, ta có

$$
p_i \circ p_i = p_i , \quad \sum_{i \in I} p_i = 1_M , \quad p_i \circ p_j = 0 \quad \text{với} \quad i \neq j ,
$$

và các $ p_i $ tạo thành một họ trực giao các toán tử chiếu có tổng bằng đồng nhất thức (II, p. 209, Định nghĩa 7). Theo *loc. cit.*, Mệnh đề 12, môđun M là tổng trực tiếp của các môđun con $ p_i(M) = e_iM $. Ngoài ra $ e_iM $ bị triệt tiêu bởi $ b_i = A(1 - e_i) $; nếu $ i \neq j $ và $ m \in M $ thì $ (1 - e_i)e_jm = e_jm $, do đó không có phần tử khác không nào của $ e_jM $ bị triệt tiêu bởi $ 1 - e_i $, và vì thế a fortiori bởi $ b_i $. Suy ra $ e_iM = M_i $, và mệnh đề được chứng minh.

#### Nhận xét {#alg-vii-s2-n1-rem-1 .statement}

— 1) Ngược lại, với mỗi i, cho $ M'_i $ là một $ (A/b_i) $-môđun, và xét A-môđun M, là tổng trực tiếp của các A-môđun $ M'_i $; khi đó các môđun con $ M_i $ được xây dựng ở trên trùng nhau với các $ M'_i $ (chỉ cần chú ý rằng nếu $ i \neq j $ thì không có phần tử khác không nào của $ M'_j $ bị triệt tiêu bởi $ b_i $ vì $ b_i + b_j = A $). Vì thế, nói một cách đại khái, việc xét một A-môđun M hay một họ $ (M_i) $ các môđun trên các vành $ A/b_i = A_i $ là như nhau.

2) Theo chứng minh trên, các phép chiếu của M lên các thành phần $ M_i $ là các phép vị tự.

3) A-môđun M là đơn sinh khi và chỉ khi mỗi $ M_i $ là đơn sinh: nếu $ M = Am $, thì $ M_i = A_i e_i m $; ngược lại nếu $ M_i = A_i m_i $ và $ m = \sum_{i \in I} m_i $, thì $ M = Am $; thật vậy, nếu $ n \in M $ có ảnh là $ a_i m_i $ với mọi i, và nếu $ a \in A $ đồng dư với $ a_i $ mod $ b_i $ với mọi i, thì am và n có cùng ảnh trong mỗi $ M_i $, nên trùng nhau.

4) Cho M và N là hai A-môđun, với các thành phần $ (M_i) $ và $ (N_i) $. Cho $ u \in \mathrm{Hom}_A(M, N) $ là một ánh xạ A-tuyến tính từ M vào N; khi đó với mọi i và với mọi $ m \in M_i $ ta có $ u(m) \in N_i $, nên u cảm sinh một ánh xạ $ A_i $-tuyến tính $ u_i \in \mathrm{Hom}_{A_i}(M_i, N_i) $. Dễ kiểm tra rằng ánh xạ $ u \mapsto (u_i) $ là một đẳng cấu các Z-môđun (tương ứng, các A-môđun khi A là giao hoán)

$$
\mathrm{Hom}_A(M, N) \to \prod_{i \in I} \mathrm{Hom}_{A_i}(M_i, N_i).
$$

### 2. Phân tích chính tắc của một môđun xoắn trên một miền iđêan chính

Cho M là một môđun trên một vành giao hoán A. Với mỗi $ a \in A $ ký hiệu $ M(\alpha) $ là hạt nhân của tự đồng cấu $ x \mapsto \alpha x $ của M. Nếu $ a $ và $ \beta $ là hai phần tử của A sao cho $ \alpha $ chia hết $ \beta $, thì rõ ràng $ M(a) \subset M(\beta) $. Đặc biệt, khi n chạy qua tập hợp các số nguyên hữu tỉ $ \geq 1 $, các môđun con $ M(\alpha^n) $ tạo thành một dãy tăng; do đó hợp $ M $, của các $ M(\alpha^n) $ là một môđun con của M, gồm những phần tử của M bị triệt tiêu bởi một lũy thừa nào đó của a. Với mỗi môđun con N của M, rõ ràng là $ N_1 = N \cap M_a $.

#### Định nghĩa 1 {#alg-vii-s2-def-1 .statement}

Cho $ \pi $ là một phần tử bất khả quy của một miền iđêan chính A; một A-môđun M được gọi là rr-nguyên sơ *nếu*, với mọi $ x \in M $, tồn tại một số nguyên $ n \geq 1 $ sao cho $ \pi^n x = 0 $ (nói cách khác, nếu M bằng môđun con $ M_\pi $).

Rõ ràng mọi môđun cyclic có dạng $ A/(\pi^s) $ đều là rr-nguyên sơ. Với một A-môđun M tùy ý, môđun con $ M_\pi $ là rr-nguyên sơ.

#### Bổ đề 1 {#alg-vii-s2-lem-1 .statement}

— Cho M là một môđun trên một miền iđêan chính A; với mọi $ a \in A $ sao cho $ a \neq 0 $, gọi $ \alpha = \varepsilon \sum_{i=1}^r \pi_i^{n(i)} $ là một phân tích của $ \alpha $ thành các nhân tử bất khả quy (VII, p. 4). Môđun con $ N = M(a) $ gồm các phần tử của M bị triệt tiêu bởi a là tổng trực tiếp của các môđun con $ M(\pi_i^{n(i)}) $, và ánh xạ gửi mỗi $ x \in M(\alpha) $ tới thành phần của nó trong $ M(\pi_i^{n(i)}) $ có dạng $ x \mapsto \gamma_i x \ (\gamma_i \in A) $. Hơn nữa
$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}
$$
Trước hết, chú ý rằng N bị triệt tiêu bởi a, nên có một cấu trúc môđun $ A/(\alpha) $ tự nhiên. Theo Mệnh đề 4 của VII, p. 3, đồng cấu chính tắc từ $ A/(\alpha) $ vào tích của các vành $ A/(\pi_i^{n(i)}) $ là một đẳng cấu vành; nay áp dụng Mệnh đề 1 của VII, p. 6, ta suy ra rằng N là tổng trực tiếp của các $ M(\pi_i^{n(i)}) $; các phép chiếu của phân tích này là các vị tự, theo VII, p. 7, Nhận xét 2. Bao hàm thức $ M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i} $ là hiển nhiên; ngược lại, cho $ x \in M(\alpha) \cap M_{\pi_i} $. Khi đó tồn tại một lũy thừa $ \pi_i^s $ của $ \pi_i $ triệt tiêu x; ta có thể giả sử $ s \geq n(i) $; theo đồng nhất thức Bezout, tồn tại $ \lambda, \mu \in A $ sao cho $ \pi_i^{n(i)} = \lambda \pi_i^s + pa $, do đó $ \pi_i^{n(i)} x = 0 $ và cuối cùng $ x \in M(\pi_i^{n(i)}) $.

#### Bổ đề 2 {#alg-vii-s2-lem-2 .statement}

— Cho M là một môđun xoắn (II, p. 313) trên một miền nguyên A. Với mọi họ hữu hạn $ (x_i)_{1 \leq i \leq n} $ các phần tử của M, tồn tại một phần tử $ \gamma \neq 0 $ của A sao cho các $ x_i $ đều thuộc $ M(\gamma) $.
Thật vậy, với mỗi chỉ số i tồn tại một phần tử $ \alpha_i \neq 0 $ của A triệt tiêu $ x_i $, và phần tử $ \gamma = \prod_{i=1}^n \alpha_i $ sẽ thỏa mãn yêu cầu.

Định lý 1. — Cho M là một môđun xoắn trên một miền iđêan chính A; với mỗi phần tử bất khả quy $ \pi $ của A, gọi $ M_\pi $ là môđun con của M gồm các phần tử bị triệt tiêu bởi một lũy thừa nào đó của $ \pi $. Nếu P là một hệ đại diện của các phần tử bất khả quy của A, thì M là tổng trực tiếp của các môđun con $ M_\pi $ của nó với $ \pi \in P $.
Mọi phần tử $ x \in M $ đều thuộc môđun con $ M(\alpha) $ ứng với một $ a \neq 0 $ nào đó, nên theo Bổ đề 1 là một tổng của hữu hạn phần tử, mỗi phần tử trong số đó thuộc một môđun con $ M_\pi $ nào đó. Mặt khác, nếu $ \sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi $, trong đó $ x_\pi, y_\pi \in M_\pi $ với mọi $ \pi \in P $, và tất cả trừ hữu hạn nhiều trong các $ x_\pi $ và $ y_\pi $ đều bằng không, thì Bổ đề 2 cho thấy rằng tồn tại $ \gamma \neq 0 $ trong A sao cho mọi $ x_\pi $ và $ y_\pi $ đều thuộc cùng một môđun con $ M(\gamma) $; áp dụng Bổ đề 1 cho $ M(\gamma) $ cho thấy rằng $ x_\pi = y_\pi $ với mọi $ \pi \in P $, điều này hoàn tất chứng minh.

Rõ ràng, nếu $ \pi $ và $ \pi' $ là hai phần tử bất khả quy liên hợp, thì $ M_\pi = M_{\pi'} $; do đó, đối với một môđun M đã cho, môđun con $ M_\pi $ chỉ phụ thuộc vào iđêan $ (\pi) $ của A; nó được gọi là thành phần nguyên sơ rr của môđun M, và phân tích của M thành tổng trực tiếp của các $ M_\pi $ được gọi là phân tích chính tắc của M thành tổng trực tiếp của các thành phần nguyên sơ rr của nó.

#### Hệ quả 1 {#alg-vii-s2-lem-2-cor-1 .statement}

— *Mọi môđun con N của một môđun xoắn M đều là tổng trực tiếp của các môđun con N ∩ M của nó*.

Điều này suy ra từ việc N ∩ M, là thành phần nguyên sơ π N, của N.

#### Hệ quả 2 {#alg-vii-s2-lem-2-cor-2 .statement}

— *Môđun con N của A-môđun xoắn M là một nhân tử trực tiếp khi và chỉ khi N, là một nhân tử trực tiếp của M, với mọi phần tử bất khả quy π của A*.

Thật vậy, nếu N và N' là hai môđun con của M, thì M = N ⊕ N' khi và chỉ khi M, − N, ⊕ N'_π với mọi phần tử bất khả quy π của $ \mathcal{A} $ (Hệ quả 1).

#### Hệ quả 3 {#alg-vii-s2-lem-2-cor-3 .statement}

— *Cho N là một môđun con của A-môđun xoắn M. Nếu, với mọi phần tử bất khả quy π của A, hoặc N, = 0 hoặc $ (M/N)_\pi = 0 $, thì N là một nhân tử trực tiếp của M*.

Thật vậy, điều kiện $ (M/N)_\pi = 0 $ kéo theo N, = M,, và áp dụng được Hệ quả 2.

Một A-môđun M được gọi là *nửa đơn* nếu mọi môđun con của M là một nhân tử trực tiếp (x. A, VIII, § 3).

#### Hệ quả 4 {#alg-vii-s2-lem-2-cor-4 .statement}

— *Cho A là một miền iđêan chính không phải là một trường, và M là một A-môđun. Khi đó M là nửa đơn khi và chỉ khi M là một môđun xoắn và M, = M(π) với mọi phần tử bất khả quy π của A*.

Trước hết giả sử rằng M là nửa đơn; lấy x ∈ M và lấy π là một phần tử bất khả quy của $ \mathcal{A} $. Nếu N là một phần bù của $ Annx $ trong M, thì ta có thể viết $ x = \alpha \pi x + y $, với $ \alpha \in \mathcal{A} $ và $ y \in N $; nhưng điều đó kéo theo $ y = (1 - \alpha n)x $, nên
$$
\pi(1 - \alpha \pi)x \in A\pi x \cap N = 0 .
$$
Trước hết suy ra rằng M là một môđun xoắn; hơn nữa nếu $ x \in M_π $, thì $ \pi(1 - \alpha \pi)x = 0 $, do đó $ \pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x $ bằng không và $ M_π = M(\pi) $.

Ngược lại, theo Hệ quả 2, chỉ cần chứng minh rằng một A-môđun M bị triệt tiêu bởi một phần tử bất khả quy π thì là nửa đơn; nhưng điều đó là hiển nhiên, vì khi đó M có một cấu trúc tự nhiên của một không gian vectơ trên trường $ \mathcal{A}/(\pi) $, và các môđun con của M chính xác là các không gian con vectơ đối với cấu trúc này.

#### Nhận xét 1 {#alg-vii-s2-n2-rem-1 .statement}

— Rõ ràng linh hóa tử của mọi phần tử ≠ 0 của một môđun nguyên sơ τ có dạng $ A\pi^k $ (k > 0 là một số nguyên), vì đó là một iđêan chính chứa một lũy thừa của τ. Cho x là một phần tử của M; với mỗi $ \pi \in P $, ký hiệu $ x_\pi $ là thành phần của x trong $ M_π $; linh hóa tử của x là BCNN của các linh hóa tử của những $ x_\pi $ khác không, nhưng theo điều trên thì trong trường hợp này nó bằng *tích* của các linh hóa tử của những $ x_\pi $ khác không (VI, p. 16, Prop. 12 (DIV)).

#### Mệnh đề 2 {#alg-vii-s2-prop-2 .statement}

— *Nếu M là một môđun xoắn sinh hữu hạn trên một miền iđêan chính A, thì các thành phần nguyên sơ n của M là không trừ ra chỉ một số hữu hạn trong chúng, và các phép chiếu của M lên các thành phần này $ M_\pi $ là các phép vị tự*.

Điều này suy ra ngay lập tức từ Bổ đề 1, vì theo Bổ đề 2 tồn tại $ \alpha \neq 0 $ trong $ \mathcal{A} $ sao cho $ M = M(\alpha) $.

#### Nhận xét 2 {#alg-vii-s2-n2-rem-2 .statement}

— Theo VII, p. 7, Nhận xét 3, một A-môđun xoắn sinh hữu hạn là cyclic nếu và chỉ nếu mỗi thành phần nguyên sơ π của nó là cyclic.

Một trường hợp riêng quan trọng mà Định lý 1 và Mệnh đề 2 áp dụng là khi $ A = \mathbf{Z} $; một $ \mathbf{Z} $-môđun chính là một *nhóm Abel*. Một nhóm Abel được gọi là một *nhóm xoắn* nếu nó là một $ \mathbf{Z} $-môđun xoắn, nghĩa là nếu mọi phần tử của nó đều có *cấp hữu hạn*. Khi đó $ P $ được lấy là tập hợp các số nguyên tố $ > 0 $; với mỗi số nguyên tố $ p > 0 $, một nhóm (Abel) được gọi là $ p $-xoắn nếu mọi phần tử của nó đều có cấp là các lũy thừa của $ p $. Theo thuật ngữ này, Định lý 1 cho thấy rằng *mọi nhóm Abel xoắn đều là tổng trực tiếp của các nhóm p-xoắn*. Trong trường hợp các nhóm hữu hạn, điều này cũng suy ra từ I, p. 80, Định lý 4.

### 3. Ứng dụng : I. Các phân tích chính tắc của các số hữu tỉ và của các hàm hữu tỉ theo một ẩn

#### Định lý 2 {#alg-vii-s2-thm-2 .statement}

*Cho $ A $ là một miền iđêan chính, $ K $ là trường các phân thức của nó và $ P $ là một hệ các đại diện của các phần tử bất khả quy của $ A $. Với một phần tử $ x \in K $ đã cho, tồn tại một tập con hữu hạn $ H $ của $ P $, các phần tử $ a_0 \in A $ và $ a, \in A $ không chia hết cho $ p $ trong $ A $ ($ p \in H $), và các số nguyên $ s(p) > 0 $ ($ p \in H $) sao cho*

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

*trong đó $ H $ và các $ s(p) $ được xác định duy nhất bởi các điều kiện này.*

*Hơn nữa, nếu $ R_p $ ký hiệu một tập con của $ A $ chứa chính xác một phần tử của mỗi lớp thặng dư mod $ p $ trong $ A (p \in P) $, thì mỗi $ x \in K $ có thể được biểu diễn duy nhất dưới dạng*

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

*trong đó $ a \in A $ và $ r_{ph} \in R_p $ với mọi $ h $ và $ p $, và tất cả trừ hữu hạn nhiều $ r_{ph} $ đều bằng không.*

Xét $ K $ như một $ A $-môđun; khi đó $ A $ là môđun con sinh bởi 1. Môđun thương $ K/A $ là thương của $ K $ theo quan hệ tương đương $ x' - x \in A $, quan hệ này cũng được viết, theo ký hiệu của VI, p. 6, là $ x \equiv x' $ (mod 1); gọi $ f $ là đồng cấu tự nhiên từ $ K $ lên $ M = K/A $.

Môđun thương $ M $ là một *môđun xoắn*, vì mọi phần tử của $ M $ đều có dạng $ f(a/b) $ ($ a \in A, b \in A, b \neq 0 $), do đó $ b f(a/b) = f(a) = 0 $. Vì thế áp dụng được Định lý 1 của VII, p. 8. Gọi $ M_p $ ($ p \in P $) là môđun con gồm các phần tử của $ M $ bị triệt tiêu bởi các lũy thừa của $ p $; khi đó $ f^{-1}(M_p) $ là vành con $ A_p $ gồm các phần tử của $ K $ có dạng $ a p^{-n} $ trong đó $ a \in A $ và $ n \geq 0 $ là một số nguyên. Môđun $ M $ là tổng trực tiếp của các $ M_p $, nên mọi $ x \in K $ đều đồng dư mod 1 với một phần tử trong tổng của các $ A_p $; nói cách khác, công thức (1) đúng, với các số nguyên $ s(p) $ $ > 0 $, và các $ a $, hữu hạn phần tử của $ A $ sao cho $ a $, không là bội của $ p $.

Bây giờ chúng ta chỉ ra rằng các điều kiện này đối với $ s(p) $ và $ a $ xác định hoàn toàn $ H $ và các $ s(p) $. Thật vậy, khi đó $ H $ là tập hợp các $ p \in P $ sao cho thành phần của $ f(x) $ trong $ M_p $ là $ \neq 0 $. Mặt khác, nếu $ s $ và $ s' $ là hai số nguyên $ > 0 $ sao cho s \geq s' và nếu $ a $ và $ a' $ là các phần tử của $ A $ không chia hết cho $ p $ sao cho $ ap^{-s} \equiv a'p^{-s'} \pmod{1} $, thì ta suy ra rằng $ a \equiv a'p^{s-s'} \pmod{p^s} $; nếu $ s > s' $ thì $ a \equiv 0 \pmod{p} $, mâu thuẫn với các giả thiết. Lập luận này cũng cho thấy rằng mỗi $ a_i $ được xác định tốt theo mod $ p^{s(p)} $.

Để hoàn tất chứng minh, trước hết ta chú ý rằng trong mỗi lớp thặng dư mod $ p^i $ trong $ A $ đều tồn tại một phần tử duy nhất có dạng $ \sum_{h=0}^{s-1} r_h p^h $ với $ r_h \in R_p $ đối với $ 0 \leq h \leq s-1 $. Thật vậy, ta tiến hành bằng quy nạp theo $ s $ (tính chất này suy ra từ định nghĩa của $ R_p $ khi $ s = 1 $) : cho $ x \in A $; theo giả thiết quy nạp, có một phần tử duy nhất có dạng $ \sum_{h=0}^{s-2} r_h p^h $ ($ r_h \in R_p $) trong lớp thặng dư của $ x $ mod $ p^{s-1} $; khi đó $ x - \sum_{h=0}^{s-2} r_h p^h $ là một bội $ ap^{s-1} $ của $ p^{s-1} $; mà tồn tại một phần tử duy nhất $ r_s $, của $ R_p $ sao cho $ a \equiv r_s \pmod{p} $; do đó $ x \equiv \sum_{h=0}^{s-1} r_h p^h \pmod{p^s} $. Để thu được công thức (2), bây giờ chỉ cần áp dụng sự kiện này cho mỗi $ a_p $ trong công thức (1). Tính duy nhất là hiển nhiên theo điều trên.

Các áp dụng quan trọng nhất của Định lý 2 là:

I. *Vành A là vành Z của các số nguyên hữu tỉ, và K = Q*. Gọi P là tập hợp các số nguyên tố > 0, và với mỗi $ p \in P $ gọi $ R_p $ là khoảng $ (0, p-1) $ trong $ \mathbf{Z} $. Khi đó ta có phân tích chính tắc

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

với $ a \in \mathbf{Z} $, $ e_{ph} \in \mathbf{Z} $ và $ 0 \leq e_{ph} \leq p-1 $.

II. *Vành A là vành E[X] của các đa thức theo một ẩn trên một trường giao hoán E, và K = E(X)*. Gọi P là tập hợp các đa thức bất khả quy đơn nhất trong $ E[X] $ (VII, p. 5). Với $ p \in P $ ta có thể, nhờ phép chia Euclid của các đa thức (IV, p. 10), lấy $ R_p $ là tập hợp các đa thức có bậc nhỏ hơn hẳn bậc của $ p $. Khi đó ta có phân tích (gọi là chính tắc) của một hàm hữu tỉ $ r(X) \in E(X) $:

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

trong đó $ a(X) $ là một đa thức và $ v_{ph}(X) $ là một đa thức có bậc nhỏ hơn hẳn bậc của $ p(X) $, với mọi $ p $ và $ h $. Đặc biệt, nếu trường E là *đóng đại số*, thì các $ p(X) $ có dạng $ X - a $ với $ a \in E $, và do đó các $ v_{ph}(X) $ là các hằng số.

Vì thế ta có thể nói rằng không gian vectơ $ E(X) $ trên trường E có một cơ sở gồm các đơn thức $ X^n $ ($ n \geq 0 $ là một số nguyên) và các hàm hữu tỉ có dạng $ X^m / (p(X))^h $, trong đó $ p \in P $ và $ h $ và $ m $ là các số nguyên với $ h \geq 1 $ và $ 0 \leq rn < \deg(p) $.

### 4. Ứng dụng : II. Nhóm nhân các phần tử khả nghịch của các số nguyên modulo a

Cho a là một số nguyên hữu tỉ > 1, và gọi $(\mathbf{Z}/a\mathbf{Z})^*$ là nhóm nhân của các phần tử khả nghịch của vành $\mathbf{Z}/a\mathbf{Z}$. Nếu $a = \prod p_i^{n(i)}$ là phân tích của a thành các thừa số nguyên tố, thì vành $\mathbf{Z}/a\mathbf{Z}$ đẳng cấu với tích của các vành $\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$ (VII, p. 3, Prop. 4) và nhóm $(\mathbf{Z}/a\mathbf{Z})^*$ đẳng cấu với tích của các nhóm $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. Như vậy ta được quy về việc nghiên cứu các nhóm $(\mathbf{Z}/p^n\mathbf{Z})^*$, trong đó p là một số nguyên tố; nhắc lại rằng (V, p. 80) cấp $\varphi(p^n)$ của $(\mathbf{Z}/p^n\mathbf{Z})^*$ là $p^n - p^{n-1} = p^{n-1}(p-1)$.

Trước hết giả sử rằng $p > 2$; đồng cấu tự nhiên $\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$ hạn chế thành một đồng cấu nhóm từ $(\mathbf{Z}/p^n\mathbf{Z})^*$ lên $(\mathbf{Z}/p\mathbf{Z})^*$, có hạt nhân được ký hiệu là U$(p^n)$; theo VII, p. 3, Mệnh đề 3, lớp thặng dư mod $p^n$ của một số nguyên m là khả nghịch khi và chỉ khi m nguyên tố cùng nhau với p, nghĩa là khi và chỉ khi lớp thặng dư của $m$ mod $p$ là khả nghịch. Suy ra U$(p^n)$ gồm tất cả các lớp thặng dư mod $p^n$ của những số nguyên đồng dư với 1 mod p, nên có $p^{n-1}$ phần tử, và có một dãy khớp

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

Tương tự, với $n \geq 2$ cho U$(2^n)$ ký hiệu hạt nhân của đồng cấu tự nhiên từ $(\mathbf{Z}/2^n\mathbf{Z})^*$ đến $(\mathbf{Z}/4\mathbf{Z})^*$; đây là một nhóm có cấp $2^{n-2}$, gồm tất cả các lớp thặng dư mod $2^n$ của các số nguyên đồng dư với 1 mod 4, và có một dãy khớp

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### Bổ đề 3 {#alg-vii-s2-lem-3 .statement}

— Cho x, y, k là các số nguyên với $k \geq 0$, và cho $p > 2$ là một số nguyên tố. Nếu $x \equiv 1 + py \mod p^2$ thì $x^{p^k} \equiv 1 + p^{k+1}y \mod p^{k+2}$. *Nếu* $x \equiv 1 + 4y \mod 8$ thì $x^{2^k} \equiv 1 + 2^{k+2}y \mod 2^{k+3}$.

Để chứng minh mệnh đề thứ nhất, chỉ cần chỉ ra rằng, nếu $k \geq 1$ và $x \equiv 1 + p^ky \mod p^{k+1}$, thì $x^p \equiv 1 + p^{k+1}y \mod p^{k+2}$, rồi lập luận bằng quy nạp theo số nguyên k. Với mọi $a \in \mathbf{Z}$ và $k \geq 1$, ngay lập tức có rằng
$$
(1 + p^ka)^p \equiv 1 + p^{k+1}a \mod p^{k+2},
$$
do đó
$$
(1 + p^ky + p^{k+1}z)^p = (1 + p^k(y + pz))^p \equiv \\
= 1 + p^{k+1}(y + pz) \equiv 1 + p^{k+1}y \mod p^{k+2}.
$$
Tương tự, với $k \geq 1$ ta có
$$
(1 + 2^{k+1}a)^2 \equiv 1 + 2^{k+2}a \mod 2^{k+3},
$$
nên
$$
(1 + 2^{k+1}y + 2^{k+2}z)^2 \equiv 1 + 2^{k+2}y \mod 2^{k+3},
$$
do đó suy ra mệnh đề thứ hai bằng quy nạp theo k.

Mệnh đề 3. — Cho $ p > 2 $ là một số nguyên tố và cho $ n > 0 $ là một số nguyên; khi đó nhóm $ U(p^n) $ là cyclic cấp $ p^{n-1} $; nếu $ n \geq 2 $ thì lớp thặng dư mod $ p^n $ của một số nguyên $ x $ đồng dư với 1 mod $ p $ là một phần tử sinh của $ U(p^n) $ khi và chỉ khi $ x $ không đồng dư với 1 mod $ p^2 $. Cho $ m > 1 $ là một số nguyên; khi đó nhóm $ U(2^m) $ là cyclic cấp $ 2^{m-2} $; nếu $ m \geq 3 $ thì lớp thặng dư mod $ 2^m $ của một số nguyên $ x $ đồng dư với 1 mod 4 là một phần tử sinh của $ U(2^m) $ khi và chỉ khi $ x $ không đồng dư với 1 mod 8.

Vì $ U(p^n) $ có cấp $ p^{n-1} $, nên cấp của mọi phần tử $ u $ của $ U(p^n) $ là một lũy thừa của $ p $, và $ u $ là một phần tử sinh của $ U(p^n) $ khi và chỉ khi $ u^{p^{n-2}} \neq 1 $. Bây giờ nếu $ u $ là lớp của $ x = 1 + py $, thì $ u^{p^{n-2}} $ là lớp của $ 1 + p^{n-1}y $, theo Bổ đề 3, do đó $ u $ sinh ra $ U(p^n) $ khi và chỉ khi $ y \not\equiv 0 \mod p $, nói cách khác $ x \not\equiv 1 \mod p^2 $. Ví dụ, lớp $ 1 + p $ sinh ra $ U(p^n) $. Tương tự, lớp $ u $ của $ x $ modulo $ 2^n $ sinh ra $ U(2^n) $ khi và chỉ khi $ u^{2^{n-3}} \neq 1 $, điều này có nghĩa là $ x $ không đồng dư với 1 modulo 8, theo Bổ đề 3; điều này được thỏa mãn với $ x = 5 $.

#### Bổ đề 4 {#alg-vii-s2-lem-4 .statement}

— Cho $ A $ là một miền iđêan chính và cho $ 0 \to N \to M \to P \to 0 $ là một dãy khớp các $ A $-môđun. Giả sử tồn tại các phần tử nguyên tố cùng nhau $ a, b \in A $ sao cho $ aN = 0 $ và $ bP = 0 $. Khi đó dãy khớp tách được. Nếu thêm nữa $ N $ và $ P $ đều là cyclic, thì $ M $ là cyclic.

Môđun $ M $ là xoắn, vì $ abM = 0 $. Mệnh đề đầu tiên suy ra từ Hệ quả 3 của VII, p. 9. Nếu $ N $ và $ P $ là cyclic, thì chúng sinh hữu hạn, và do đó $ M $ cũng vậy (II, p. 17, Hệ quả 5); vì mỗi thành phần nguyên sơ theo $ p $ của $ M $ đẳng cấu với một thành phần nguyên sơ theo $ p $ hoặc của $ N $ hoặc của $ P $, nên theo Nhận xét 2 của VII, p. 10, suy ra rằng $ M $ là cyclic.

Định lý 3. — Nếu $ a = \prod p_i^{n(i)} $ là phân tích thành thừa số nguyên tố của số nguyên $ a > 1 $, thì nhóm $ (\mathbf{Z}/a\mathbf{Z})^* $ các phần tử khả nghịch của vành $ \mathbf{Z}/a\mathbf{Z} $ đẳng cấu với tích của các nhóm $ (\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^* $. Nếu $ p > 2 $ là một số nguyên tố và $ n \geq 1 $ là một số nguyên, thì nhóm $ (\mathbf{Z}/p^n\mathbf{Z})^* $ là cyclic cấp $ p^n \ ^1(p - 1) $. Nhóm $ (\mathbf{Z}/2\mathbf{Z})^* $ là tầm thường; với $ n \geq 2 $ thì nhóm $ (\mathbf{Z}/2^n\mathbf{Z})^* $ là tích trực tiếp của nhóm cyclic cấp $ 2^n \ ^2 $ sinh bởi lớp thặng dư của 5 mod $ 2^n $ và nhóm cyclic cấp 2 gồm các lớp thặng dư của 1 và $ -1 $ mod $ 2^n $.

Các cấp $ p^n \ ^1 $ của $ U(p^n) $ và $ p - 1 $ của $ (\mathbf{Z}/p\mathbf{Z})^* $ là nguyên tố cùng nhau; vì $ U(p^n) $ và $ (\mathbf{Z}/p\mathbf{Z})^* $ là cyclic (Mệnh đề 3 và V, p. 78, Bổ đề 1), nhóm $ (\mathbf{Z}/p^n\mathbf{Z})^* $ là cyclic (áp dụng Bổ đề 4 cho dãy khớp (3)). Nếu $ n \geq 2 $ thì hạn chế của đồng cấu $ v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* $ lên nhóm con $ (1, -1) $ là song ánh; do đó nhóm $ (\mathbf{Z}/2^n\mathbf{Z})^* $ là tích trực tiếp của nhóm con này và hạt nhân $ U(2^n) $ của $ v $; kết quả suy ra từ Mệnh đề 3.

#### Nhận xét {#alg-vii-s2-n4-rem-1 .statement}

— Cho $ p > 2 $ là một số nguyên tố và cho $ x $ là một số nguyên đồng dư với 1 mod $ p $ và không đồng dư với 1 mod $ p^2 $; có một dãy khớp

$$
\{0\} \to \mathbf{Z}/p^n \ ^1\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{\nu} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

của các nhóm, trong đó $ v $ là phép chiếu tự nhiên và $ u $ được cảm sinh trên các thương bởi ánh xạ $ r \mapsto x^r $. Cho $ \mathbf{Z}_p $ là vành các số nguyên $ p $-adic ($ V $, p. 96), và cho $ x $ là một phần tử của $ \mathbf{Z}_p $ sao cho $ x - 1 \in p\mathbf{Z}_p $ và $ x - 1 \notin p^2\mathbf{Z}_p $; khi chuyển qua giới hạn nghịch, các dãy khớp (5) cảm sinh một dãy khớp

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

trong đó $ v $ là ánh xạ tự nhiên, và ánh xạ liên tục $ u $ mở rộng ánh xạ $ n \mapsto x^n $ ($ n \in \mathbf{Z} $). Ta thường đặt $ x^n = u(x) $ với $ n \in \mathbf{Z}_p $.

Tương tự, nếu $ x \in \mathbf{Z}_2 $ với $ x - 1 \in 4\mathbf{Z} $, và $ x - 1 \notin 8\mathbf{Z}_2 $, thì có một dãy khớp tách

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

trong đó $ u $ là một mở rộng liên tục của ánh xạ $ n \mapsto x^n $

### Bài tập {#alg-vii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
