---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 3
section_title: Convolution of measures on groups
lang: vi
source: int-vii-ix
book_pages: INT VIII.18-INT VIII.24, INT VIII.61-INT VIII.65
pdf_pages: 0118-0124, 0161-0165
extraction: ocr
subsections:
    - "no": 1
      title: Algebras of measures
      page: 18
      pdf_page: 118
    - "no": 2
      title: The case of a group operating on a space
      page: 21
      pdf_page: 121
    - "no": 3
      title: Convolution and linear representations
      page: 22
      pdf_page: 122
statements: 16
exercises: 13
content_sha256: 2dbc6ad12bcedbe7ca22e48ad986313b4ffa8773352d35a2895929606ba87b95
translated_from: content/en/int/VIII/03_s3_convolution_of_measures_on_groups.md
source_content_sha256: 770c50427b33153ec02eedab6fb35e27870c859fef0e164830e39a285e132540
translation_model: gpt-5.4
translation_run: translate-vi-cf425743
glossary_version: 34
glossary_terms_sha256: fb4c0cf786de2c9a75a39dbf8774a364ca3dc3f4457bba0fad58c30c3db6a848
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TÍCH CHẬP CỦA CÁC ĐỘ ĐO TRÊN NHÓM

### 1. Các đại số của độ đo

Cho G là một nhóm compact địa phương. Ta quy ước một lần cho tất cả rằng các độ đo $ \mu_1, \ldots, \mu_n $ trên G được gọi là chập được nếu chúng chập được đối với ánh xạ

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \cdots x_n;
$$

và chính bằng ánh xạ này mà tích chập $ *_{i} \mu_i $ sẽ luôn luôn được lấy. Nếu $ s \in G, t \in G $, thì

(1)
$$
\varepsilon_s * \varepsilon_t = \varepsilon_{st}.
$$

Nếu $ s \in G $ và $ \mu \in \mathcal{M}(G) $, thì

(2)
$$
\varepsilon_s * \mu = \gamma(s) \mu
$$
(3)
$$
\mu * \varepsilon_s = \delta(s^{-1}) \mu
$$

theo §1, No. 1, Ví dụ 3. Nếu G là Abel, việc nói rằng $ \mu_1 $ và $ \mu_2 $ khả hợp theo phép chập là tương đương với việc nói rằng $ \mu_2 $ và $ \mu_1 $ khả hợp theo phép chập, và khi đó ta có $ \mu_1 * \mu_2 = \mu_2 * \mu_1 $. Khi G không Abel, có thể xảy ra việc $ \mu_1 $ và $ \mu_2 $ khả hợp theo phép chập mà $ \mu_2 $ và $ \mu_1 $ lại không như vậy (Bài tập 12).

#### Mệnh đề 1 {#int-viii-s3-prop-1 .statement}

— Cho G là một nhóm compact địa phương, $ \lambda, \mu, \nu $ là các độ đo $ \neq 0 $ trên G.

(i) Nếu $ \lambda, \mu, \nu $ chập được với nhau, thì $ \lambda $ và $ \mu $, $ |\lambda| * |\mu| $ và $ \nu $, $ \mu $ và $ \nu $, $ \lambda $ và $ |\mu| * |\nu| $ cũng chập được với nhau, và ta có

$$
\lambda * \mu * \nu = (\lambda * \mu) * \nu = \lambda * (\mu * \nu).
$$

(ii) Nếu $ \lambda $ và $ \mu $ có thể lấy tích chập, cũng như $ |\lambda| * |\mu| $ và $ \nu $, thì $ \lambda, \mu, \nu $ có thể lấy tích chập. Tương tự nếu $ \mu $ và $ \nu $ có thể lấy tích chập, cũng như $ \lambda $ và $ |\mu| * |\nu| $.

Điều này suy ra từ Mệnh đề 1 của §1, No. 2.

Có thể tồn tại các độ đo $ \lambda, \mu, \nu $ trên G sao cho các tích chập $ \lambda * \mu $, $ (\lambda * \mu) * \nu $, $ \mu * \nu $, $ \lambda * (\mu * \nu) $ đều được xác định, nhưng $ (\lambda * \mu) * \nu \neq \lambda * (\mu * \nu) $ (xem Bài tập 4).

Cho $ \rho $ là một hàm hữu hạn nửa liên tục dưới $ > 0 $ trên $ G $ sao cho $ \rho(st) \leq \rho(s)\rho(t) $ với mọi $ s, t $ trong $ G $. Ta ký hiệu bởi $ \mathcal{M}^\rho(G) $ không gian vectơ các độ đo $ \lambda $ trên $ G $ sao cho $ \rho $ khả tích đối với $ \lambda $, và bởi $ \| \lambda \|_\rho $ (hoặc đơn giản là $ \| \lambda \| $) chuẩn $ \int_G \rho(s) d|\lambda|(s) $ trên không gian này. Khi $ \rho = 1 $, ta thu được tập hợp $ \mathcal{M}^1(G) $ các độ đo bị chặn trên $ G $.

#### Mệnh đề 2 {#int-viii-s3-prop-2 .statement}

(i) *Hai phần tử bất kỳ của $ \mathcal{M}^\rho(G) $ đều có thể chập được.*
(ii) *Đối với phép chập, và đối với chuẩn $ \| \lambda \| $, $ \mathcal{M}^\rho(G) $ là một đại số chuẩn đầy đủ, nhận $ \varepsilon_e $ làm phần tử đơn vị.*
(iii) $ \mathcal{C}'(G) $ *là một đại số con của $ \mathcal{M}^\rho(G) $*.

Cho $ \lambda, \mu $ thuộc $ \mathcal{M}^\rho(G) $, và ta sẽ chỉ ra rằng $ \lambda $ và $ \mu $ có thể chập được. Cho $ f \in \mathcal{K}_+(G) $. Vì $ \rho $ là $ > 0 $ và nửa liên tục dưới, tồn tại một hằng $ k > 0 $ sao cho $ f \leq k\rho $. Khi đó

$$
\int^* f(st) d|\lambda|(s) d|\mu|(t) \leq k \int^* \rho(st) d|\lambda|(s) d|\mu|(t)
$$
$$
\leq k \int^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= k \left( \int^* \rho(s) d|\lambda|(s) \right) \left( \int^* \rho(t) d|\mu|(t) \right)
$$

(Ch. V, §8, No. 3, Hệ quả 1 của Mệnh đề 8). Do đó $ (s,t) \mapsto f(st) $ là khả tích đối với $ (\lambda \otimes \mu) $, suy ra $ \lambda $ và $ \mu $ chập được. Mặt khác, dùng Ch. V (§1, Mệnh đề 4, §6, Mệnh đề 2, §8, Hệ quả 1 của Mệnh đề 8) và sự kiện rằng $ (s,t) \mapsto \rho(s)\rho(t) $ là nửa liên tục dưới trên $ G \times G $, ta có

$$
\int_G^* \rho(s) d|\lambda * \mu|(s) = \int_G^* \rho(s) d|\lambda * \mu|(s)
$$
$$
\leq \int_{G \times G}^* \rho(st) d|\lambda|(s) d|\mu|(t) \leq \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t) = \| \lambda \| \cdot \| \mu \|.
$$

Ta thấy rằng $ \lambda * \mu \in \mathcal{M}^\rho(G) $ và $ \| \lambda * \mu \| \leq \| \lambda \| \cdot \| \mu \| $. Theo Mệnh đề 1, $ \mathcal{M}^\rho(G) $ là một đại số. Ánh xạ $ \lambda \mapsto \rho \cdot \lambda $ là một ánh xạ tuyến tính đẳng cự $ \theta $ từ $ \mathcal{M}^\rho(G) $ vào $ \mathcal{M}^1(G) $; nếu $ \mu \in \mathcal{M}^1(G) $ thì $ 1/\rho $, vốn bị chặn địa phương và nửa liên tục trên, là khả tích địa phương đối với $ \mu $, và $ \rho $ là khả tích đối với $ (1/\rho) \cdot \mu $, do đó $ (1/\rho) \cdot \mu \in \mathcal{M}^\rho(G) $; điều này chứng tỏ rằng $ \theta $ là toàn ánh; vì thế $ \mathcal{M}^\rho(G) $ là một đại số định chuẩn đầy đủ. Sau hết, hiển nhiên là $ \varepsilon_e $ là một phần tử đơn vị của $ \mathcal{M}^\rho(G) $ và $ \mathcal{C}'(G) $ là một đại số con của $ \mathcal{M}^\rho(G) $ (§1, No. 4, Hệ quả của Mệnh đề 5).

Nếu $ \rho = 1 $, Mệnh đề 2, (i) và (ii) cũng suy ra từ §1, Mệnh đề 2.

#### Mệnh đề 3 {#int-viii-s3-prop-3 .statement}

*Cho $ \mu_1, \ldots, \mu_n $ là các độ đo trên G. Nếu mọi $ \mu_i $, trừ nhiều nhất một, đều có giá compắc, thì các $ \mu_i $ là khả chập.*

Thật vậy, gọi $ S_i $ là giá của $ \mu_i $, và giả sử rằng $ S_i $ là compắc với $ i \neq i_0 $. Cho K là một tập con compắc của G. Tập hợp các $ (x_1, \ldots, x_n) \in \prod_i S_i $ sao cho $ x_1 x_2 \cdots x_n \in K $ là compắc, vì các điều kiện $ x_i \in S_i $ với mọi $ i $, $ x_1 x_2 \cdots x_n \in K $ kéo theo

$$
x_{i_0} \in S_{i_0-1}^{-1} \cdots S_1^{-1} K S_n^{-1} \cdots S_{i_0+1}^{-1} .
$$

Vậy các $ \mu_i $ là khả chập (§1, No. 4, Mệnh đề 4).

#### Mệnh đề 4 {#int-viii-s3-prop-4 .statement}

*Ánh xạ $ (\lambda, \mu) \mapsto \lambda * \mu $ (tương ứng, $ (\lambda, \mu) \mapsto \mu * \lambda $), trong đó $ \lambda \in \mathcal{C}'(G) $, $ \mu \in \mathcal{M}(G) $, xác định trên $ \mathcal{M}(G) $ cấu trúc của một môđun trái (tương ứng, phải) trên đại số $ \mathcal{C}'(G) $.*

Điều này suy ra từ các Mệnh đề 1 và 3.

#### Mệnh đề 5 {#int-viii-s3-prop-5 .statement}

*Cho $ \lambda $ là một độ đo Haar trái (tương ứng, phải) trên G, và $ \mu \in \mathcal{M}^1(G) $. Khi đó $ \mu $ và $ \lambda $ (tương ứng, $ \lambda $ và $ \mu $) chập được, và $ \mu * \lambda = \mu(1)\lambda $ (tương ứng, $ \lambda * \mu = \mu(1)\lambda $).*

Ta có thể giả sử rằng $ \mu \geqslant 0 $. Cho $ f \in \mathcal{K}_+(G) $. Khi $ \lambda $ là một độ đo Haar trái,

$$
\int^* d\mu(x) \int^* f(xy)\, d\lambda(y) = \int^* d\mu(x) \int f(y)\, d\lambda(y) = \lambda(f)\|\mu\| ,
$$

do đó hàm $ (x, y) \mapsto f(xy) $ là khả tích đối với $ (\mu \otimes \lambda) $, và tích phân của nó đối với $ \mu \otimes \lambda $ là $ \lambda(f)\|\mu\| $. Ta lập luận tương tự khi $ \lambda $ là một độ đo Haar phải.

#### Mệnh đề 6 {#int-viii-s3-prop-6 .statement}

*Cho $ \mu $ và $ \nu $ là hai độ đo khả tích chập trên G. Cho $ \chi $ là một biểu diễn liên tục của G trong $ \mathbf{C}^* $. Khi đó $ \chi \cdot \mu $ và $ \chi \cdot \nu $ là khả tích chập và $ (\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu) $.*

Cho $ f \in \mathcal{K}(G) $. Khi đó $ f\chi \in \mathcal{K}(G) $, do đó hàm

$$
(x, y) \mapsto f(xy)\chi(xy) = f(xy)\chi(x)\chi(y)
$$

trên $ G \times G $ là khả tích đối với $ \mu \otimes \nu $; do đó hàm $ (x, y) \mapsto f(xy) $ là khả tích đối với $ (\chi \cdot \mu) \otimes (\chi \cdot \nu) $; do đó $ \chi \cdot \mu $ và $ \chi \cdot \nu $ là khả hợp chập. Hơn nữa,

$$
\langle \chi \cdot \mu * \chi \cdot \nu, f \rangle = \int f(xy)\chi(x)\chi(y)\, d\mu(x)\, d\nu(y)
= \int (f\chi)(xy)\, d\mu(x)\, d\nu(y) = \langle \mu * \nu, \chi f \rangle ,
$$

do đó $ (\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu) $.

#### Mệnh đề 7 {#int-viii-s3-prop-7 .statement}

*Cho G và G' là hai nhóm compact địa phương, u là một biểu diễn liên tục của G trong G', và $ \mu_1, \ldots, \mu_n $ là các độ đo trên G, tất cả đều $ \neq 0 $. Khi đó các khẳng định sau là tương đương:
(i) $ u $ là $ \mu_i $-thực sự với mọi i, và các độ đo $ u(|\mu_i|) $ chập được;
(ii) các $ \mu_i $ chập được và $ u $ là thực sự đối với $ *_{i}(|\mu_i|) $.
Khi các điều kiện này được thỏa mãn,

$$
*_{i} u(\mu_i) = u(*_{i} \mu_i).
$$

Điều này suy ra từ §1, No. 2, Hệ quả của Mệnh đề 1.

#### Hệ quả {#int-viii-s3-n1-cor-1 .statement}

*Cho G là một nhóm compact địa phương, $ \mu_1, \ldots, \mu_n $ là các độ đo trên G. Để dãy $ (\mu_i)_{1 \leq i \leq n} $ chập được, điều kiện cần và đủ là dãy $ (\check{\mu}_{n-i})_{0 \leq i \leq n-1} $ cũng vậy, trong trường hợp đó*

$$
(\mu_1 * \cdots * \mu_n)^{\vee} = \check{\mu}_n * \cdots * \check{\mu}_1.
$$

Điều này suy ra từ Mệnh đề 7 khi xét đẳng cấu $ x \mapsto x^{-1} $ của G lên nhóm đối.

### 2. Trường hợp một nhóm tác động trên một không gian

Cho X là một không gian compact địa phương mà trên đó một nhóm compact địa phương G tác động liên tục bên trái bởi

$$
(s, x) \mapsto s \cdot x.
$$

Nếu $ \mu_1, \ldots, \mu_n $ là các độ đo trên G và $ \nu $ là một độ đo trên X, thì ta sẽ nói rằng chúng khả tích chập nếu chúng như vậy đối với ánh xạ $ (s_1, \ldots, s_n, x) \mapsto s_1 \cdots s_n x $ từ $ G^n \times X $ vào X, và tích chập của chúng được hiểu theo nghĩa của ánh xạ này.

Nếu $ s \in G $ và $ x \in X $, thì

(4)
$$
\varepsilon_s * \varepsilon_x = \varepsilon_{sx}.
$$

Nếu $ s \in G $ và $ \mu \in \mathcal{M}(X) $, thì

(5)
$$
\varepsilon_s * \mu = \gamma(s)\mu
$$
theo §1, No. 1, Ví dụ 3.

#### Mệnh đề 8 {#int-viii-s3-prop-8 .statement}

— Cho $ \mu $ là một độ đo trên $ G $, $ \nu $ là một độ đo trên $ X $.
(i) Nếu $ \mu $ có giá compact, thì $ \mu $ và $ \nu $ chập được.
(ii) Nếu $ \nu $ có giá compact, và nếu $ G $ tác động một cách đúng lên $ X $, thì $ \mu $ và $ \nu $ chập được.
Điều này suy ra từ Mệnh đề 4 của §1, No. 4.

#### Mệnh đề 9 {#int-viii-s3-prop-9 .statement}

— Đối với phép chập, $ \mathcal{M}^1(X) $ là một môđun trái trên $ \mathcal{M}^1(G) $, còn $ \mathcal{M}(X) $ và $ \mathcal{C}'(X) $ là những môđun trái trên $ \mathcal{C}'(G) $.
Điều này suy ra từ Mệnh đề 8, và từ §1, các Mệnh đề 1, 3 và Hệ quả của Mệnh đề 5.

#### Mệnh đề 10 {#int-viii-s3-prop-10 .statement}

— Cho $ \mu $ là một độ đo trên $ G $, $ \nu $ là một độ đo trên $ X $, $ \mu $ và $ \nu $ có thể chập được. Giả sử thêm rằng tồn tại một độ đo dương $ \beta $ trên $ X $ sao cho $ \gamma(s)\nu $ có cơ sở $ \beta $ với mọi $ s \in G $. Khi đó $ \mu * \nu $ có cơ sở $ \beta $.
Cho $ K $ là một tập con compắc $ \beta $-không đáng kể của $ X $. Khi đó $ K $ là $ \gamma(s)|\nu| $-không đáng kể với mọi $ s \in G $. Bây giờ,
$$
|\mu| * |\nu| = \int_G (\varepsilon_s * |\nu|) d|\mu|(s)
$$
(§1, No. 5, Mệnh đề 7), và ánh xạ $ s \mapsto \varepsilon_s * |\nu| $ liên tục mơ hồ (§2, Mệnh đề 6). Do đó $ K $ là $ |\mu| * |\nu| $-không đáng kể theo Chương V, §3, No. 3, Định lý 1. Vậy $ |\mu| * |\nu| $ có cơ sở $ \beta $ (Chương V, §5, No. 5, Định lý 2).

### 3. Phép chập và các biểu diễn tuyến tính

#### Mệnh đề 11 {#int-viii-s3-prop-11 .statement}

— Cho $ G $ là một nhóm compact địa phương, $ E $ là một không gian lồi địa phương tựa-đầy đủ, $ U $ là một biểu diễn liên tục của $ G $ trong $ E $.
(i) Nếu $ \lambda \in \mathcal{C}'(G) $, $ \mu \in \mathcal{C}'(G) $, thì $ U(\lambda * \mu) = U(\lambda)U(\mu) $.
(ii) Giả sử rằng $ E $ là một không gian Banach, và đặt $ \rho(s) = \|U(s)\| $ với $ s \in G $. Nếu $ \lambda \in \mathcal{M}^\rho(G) $, $ \mu \in \mathcal{M}^\rho(G) $, thì $ U(\lambda * \mu) = U(\lambda)U(\mu) $.
Cho $ \lambda, \mu $ thuộc $ \mathcal{C}'(G) $. Với mọi $ x \in E $ ta có, khi áp dụng đặc biệt các Mệnh đề 1 và 4 của Ch. VI, §1, No. 1,
$$
U(\lambda * \mu)x = \int_G U(s)x\, d(\lambda * \mu)(s)
$$
$$
= \int_{G \times G} U(st)x\, d\lambda(s)\, d\mu(t) = \int_{G \times G} U(s)U(t)x\, d\lambda(s)\, d\mu(t)
$$
$$
= \int_G U(\lambda)U(t)x\, d\mu(t) = U(\lambda) \int_G U(t)x\, d\mu(t) = U(\lambda)U(\mu)x ,
$$
do đó suy ra (i). Một lập luận tương tự có thể được áp dụng trong trường hợp (ii).

Vẫn với G là một nhóm địa phương compact, giả sử rằng G tác động liên tục bên trái trên một không gian địa phương compact X. Điều này xác định (§2, No. 4) một biểu diễn tuyến tính liên tục $ \gamma $ của G trong $ \mathcal{M}(X) $ (được trang bị tôpô hội tụ compact trong $ \mathcal{H}(X) $).

#### Mệnh đề 12 {#int-viii-s3-prop-12 .statement}

*Nếu $ \lambda \in \mathcal{C}'(G) $ và $ \mu \in \mathcal{M}(X) $, thì*

$$
\gamma(\lambda)\mu = \lambda * \mu.
$$

Theo Mệnh đề 7 của §1, No. 5,

$$
\lambda * \mu = \int_G (\varepsilon_s * \mu) d\lambda(s).
$$

Bây giờ, $ \varepsilon_s * \mu = \gamma(s)\mu $ (No. 2, công thức (5)) và

$$
\int_G (\gamma(s)\mu) d\lambda(s) = \gamma(\lambda)\mu
$$

theo định nghĩa của $ \gamma(\lambda) $.

#### Hệ quả {#int-viii-s3-n3-cor-1 .statement}

*Ánh xạ $ (\lambda, \mu) \mapsto \lambda * \mu $ từ $ \mathcal{C}'(G) \times \mathcal{M}(X) $ vào $ \mathcal{M}(X) $ là hypoliên tục đối với các tập con đồng liên tục của $ \mathcal{C}'(G) $ và các tập con compact của $ \mathcal{M}(X) $ ($ \mathcal{C}'(G) $ và $ \mathcal{M}(X) $ lần lượt được trang bị tôpô hội tụ compact trong $ \mathcal{C}(G) $ và $ \mathcal{H}(X) $).*

Thật vậy, $ \mathcal{M}(X) $, được trang bị tôpô hội tụ compact trong $ \mathcal{H}(X) $, là gần đầy đủ. Do đó ánh xạ $ (\lambda, \mu) \mapsto \gamma(\lambda)\mu $ từ $ \mathcal{C}'(G) \times \mathcal{M}(X) $ vào $ \mathcal{M}(X) $ là hypocontinuous đối với các tập con đẳng liên tục của $ \mathcal{C}'(G) $ và các tập con compact của $ \mathcal{M}(X) $ (§2, No. 6). Khi đó chỉ cần áp dụng Mệnh đề 12.

#### Nhận xét {#int-viii-s3-n3-rem-1 .statement}

— 1) Cho $ \lambda_0 \in \mathcal{C}'(G) $. Ánh xạ $ \mu \mapsto \lambda_0 * \mu $ từ $ \mathcal{M}(X) $ vào $ \mathcal{M}(X) $ là liên tục theo nghĩa mơ hồ. Thật vậy, cho $ f \in \mathcal{H}(X) $. Ta có

$$
\langle \lambda_0 * \mu, f \rangle = \int f(sx) d\lambda_0(s) d\mu(x) = \langle \mu, g \rangle,
$$

trong đó $ g(x) = \int f(sx) d\lambda_0(s) $. Khi đó, $ g $ liên tục (Ch. VII, §1, No. 1, Bổ đề 1). Mặt khác, gọi S là giá của $ \lambda_0 $ và K là giá của $ f $. Các điều kiện $ sx \in K $ và $ s \in S $ kéo theo $ x \in S^{-1}K $; do đó giá của $ g $ được chứa trong $ S^{-1}K $, nên $ g \in \mathcal{H}(X) $. Khi ấy $ \langle \lambda_0 * \mu, f \rangle = \langle \mu, g \rangle $ là một hàm liên tục theo tôpô mờ của $ \mu $, điều đó chứng minh mệnh đề của chúng ta.

2) Cho $ \mu_0 \in \mathcal{M}(X) $. Ánh xạ $ \lambda \mapsto \lambda * \mu_0 $ từ $ \mathcal{C}'(G) $ vào $ \mathcal{M}(X) $ là liên tục đối với các tôpô $ \sigma(\mathcal{C}'(G), \mathcal{C}(G)) $ và $ \sigma(\mathcal{M}(X), \mathcal{H}(X)) $. Thật vậy, lấy $ f \in \mathcal{K}(X) $. Đặt $ h(s) = \int f(sx)\, d\mu_0(x) $, ta có $ \langle f, \lambda * \mu_0 \rangle = \langle h, \lambda \rangle $, và $ h \in \mathcal{C}(G) $ (Ch. VII, §1, No. 1, Bổ đề 1).

#### Mệnh đề 13 {#int-viii-s3-prop-13 .statement}

*Ánh xạ* $ (s, \mu) \mapsto \gamma(s)\mu $ *từ* $ G \times \mathcal{M}_+(X) $ *vào* $ \mathcal{M}_+(X) $ *là liên tục khi tập hợp* $ \mathcal{M}_+(X) $ *các độ đo dương trên* $ X $ *được trang bị tôpô mờ*.

Vì $ \gamma(s)\mu = \gamma(ss_0^{-1})\gamma(s_0)\mu $, suy ra từ *Nhận xét 1* rằng chỉ cần chứng minh tính liên tục của ánh xạ đang xét tại một điểm có dạng $ (e, \mu_0) $ với $ \mu_0 \in \mathcal{M}_+(X) $. Cho một hàm $ f \in \mathcal{K}(X) $ và một số $ \varepsilon > 0 $, khi đó vấn đề là chỉ ra rằng tồn tại một lân cận U của e trong G và một lân cận W của $ \mu_0 $ trong $ \mathcal{M}_+(X) $ sao cho các quan hệ $ s \in U, \mu \in W $ kéo theo

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon .
$$

Cho V là một lân cận compact của giá đỡ K của $ f $ trong X, và cho $ \varphi \in \mathcal{K}_+(X) $ sao cho $ \varphi(x) = 1 $ trên V; tồn tại một lân cận $ W_0 $ của $ \mu_0 $ trong $ \mathcal{M}_+(X) $ sao cho $ a = \sup_{\mu \in W_0} \mu(V) $ là hữu hạn: chỉ cần lấy $ W_0 $ là tập hợp các $ \mu \in \mathcal{M}_+(X) $ sao cho $ |\langle \varphi, \mu - \mu_0 \rangle| \leq 1 $. Vì ánh xạ $ (s, x) \mapsto sx $ là liên tục, mặt khác tồn tại một lân cận compact $ U_0 $ của e trong G sao cho $ sK \subset V $ với mọi $ s \in U_0 $; khi đó hàm $ (s, x) \mapsto f(sx) $ liên tục đều trên $ U_0 \times V $ và do đó tồn tại một lân cận $ U \subset U_0 $ của e sao cho $ |f(sx) - f(x)| \leq \varepsilon / 2a $ với mọi $ s \in U $ và $ x \in V $. Do đó, với $ s \in U $ và $ \mu \in W_0 $, ta có

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu(x) \right| \leq \varepsilon / 2 ;
$$

nếu $ W \subset W_0 $ là lân cận của $ \mu_0 $ trong $ \mathcal{M}_+(X) $ được tạo bởi các độ đo $ \mu \in W_0 $ sao cho $ \left| \int f(x)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon / 2 $, thì U và W thỏa mãn các yêu cầu.

### Bài tập {#int-viii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
