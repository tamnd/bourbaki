---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 11
section_title: Graded modules and rings
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0387-0401, 0448-0449
extraction: ocr
subsections:
    - "no": 1
      title: GRADED COMMUTATIVE GROUPS
      page: 0
      pdf_page: 387
    - "no": 2
      title: GRADED RINGS AND MODULES
      page: 0
      pdf_page: 388
    - "no": 3
      title: GRADED SUBMODULES
      page: 0
      pdf_page: 391
    - "no": 4
      title: CASE OF AN ORDERED GROUP OF DEGREES
      page: 0
      pdf_page: 395
    - "no": 5
      title: GRADED TENSOR PRODUCT OF GRADED MODULES
      page: 0
      pdf_page: 398
    - "no": 6
      title: GRADED MODULES OF GRADED HOMOMORPHISMS
      page: 0
      pdf_page: 399
statements: 28
exercises: 1
content_sha256: 14f2a544058b4ff9e74982ebe9de411e2a925b2d86486efec010490100f2d581
translated_from: content/en/alg/II/11_s11_graded_modules_and_rings.md
source_content_sha256: d4e3ce7cd2b861bb7c9f076b7cfbacdd960d48f097f2e3c7ac86a9264dde8772
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-cafeca20
glossary_version: 34
glossary_terms_sha256: 09e8e4d89891aaccd6f14f4f7506cbdf7e592acc01502cfb33092d12f204e00f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. MÔĐUN VÀ VÀNH PHÂN BẬC

*Từ no. 2 của đoạn này trở đi, $ \Delta $ sẽ ký hiệu một nửa nhóm giao hoán (I, § 2, no. 1), được viết theo phép cộng, với phần tử đơn vị được ký hiệu bởi 0.*

### 1. CÁC NHÓM GIAO HOÁN PHÂN BẬC

Ta sẽ chuyển sang một ngôn ngữ khác các định nghĩa liên quan đến các tổng trực tiếp (§ 1, no. 8).

#### Định nghĩa 1 {#alg-ii-s11-def-1 .statement}

*Cho một nhóm giao hoán $ G $ được viết theo phép cộng và một tập hợp $ \Delta $, một phân bậc kiểu $ \Delta $ trên $ G $ là một họ $ (G_\lambda)_{\lambda \in \Delta} $ các nhóm con của $ G $, mà $ G $ là tổng trực tiếp của chúng. Tập hợp $ G $, với cấu trúc được xác định bởi luật nhóm và phân bậc của nó, được gọi là một nhóm (giao hoán) phân bậc kiểu $ \Delta $.*

$ \Delta $ được gọi là *tập hợp các bậc* của $ G $. Một phần tử $ x \in G $ được gọi là *thuần nhất* nếu nó thuộc một trong các $ G_\lambda $, *thuần nhất bậc* $ \lambda $ nếu $ x \in G_\lambda $. Phần tử 0 do đó thuần nhất với mọi bậc; nhưng nếu $ x \neq 0 $ là thuần nhất, nó chỉ thuộc một trong các $ G_\lambda $; chỉ số $ \lambda $ sao cho $ x \in G_\lambda $ khi đó được gọi là *bậc của* $ x $ (hoặc đôi khi là *trọng số* của $ x $) và đôi khi được ký hiệu bởi $ \deg(x) $. Mọi $ y \in G $ có thể được viết duy nhất dưới dạng một tổng $ \sum_\lambda y_\lambda $ các phần tử thuần nhất với $ y_\lambda \in G_\lambda $; $ y_\lambda $ được gọi là *thành phần thuần nhất bậc* $ \lambda $ (hoặc đơn giản là *thành phần bậc* $ \lambda $) của $ y $. Khi từ "trọng số" được dùng thay cho "bậc", tính từ "thuần nhất" được thay bằng "đẳng trọng".

#### Ví dụ {#alg-ii-s11-n1-exa-1 .statement}

(1) Cho một nửa nhóm giao hoán bất kỳ $ \Delta $ (với phần tử đơn vị 0) và một nhóm giao hoán $ G $, một phân bậc $ (G_\lambda)_{\lambda \in \Delta} $ được xác định trên $ G $ bằng cách lấy $ G_0 = G $ và $ G_\lambda = \{0\} $ với $ \lambda \neq 0 $; phân bậc này được gọi là *tầm thường*.

(2) Cho $ \Delta, \Delta' $ là hai tập hợp và $ \rho $ là một ánh xạ từ $ \Delta $ vào $ \Delta' $. Cho $ (G_\lambda)_{\lambda \in \Delta} $ là một phân bậc kiểu $ \Delta $ trên một nhóm giao hoán $ G $; với $ \mu \in \Delta' $, cho $ G'_\mu $ là tổng của các $ G_\lambda $ sao cho $ \rho(\lambda) = \mu $; rõ ràng $ (G'_\mu)_{\mu \in \Delta'} $ là một phân bậc kiểu $ \Delta' $ trên $ G $, được gọi là *dẫn xuất* từ $ (G_\lambda) $ bằng ánh xạ $ \rho $.

Khi $ \Delta $ là một nhóm giao hoán được viết theo phép cộng và $ \rho $ là ánh xạ $ \lambda \mapsto -\lambda $ của $ \Delta $ lên chính nó, $ (G'_\mu) $ được gọi là phân bậc *đối* của $ (G_\lambda) $.

(3) Nếu $ \Delta = \Delta_1 \times \Delta_2 $ là một tích của hai tập hợp, một phân bậc kiểu $ \Delta $ được gọi là một *phân bậc đôi* của các kiểu $ \Delta_1, \Delta_2 $. Với mọi $ \lambda \in \Delta_1 $, đặt $ G'_\lambda = \bigoplus_{\mu \in \Delta_2} G_{\lambda \mu} $ và, với mọi $ \mu \in \Delta_2 $, đặt $ G''_\mu = \bigoplus_{\lambda \in \Delta_1} G_{\lambda \mu} $; rõ ràng $ (G'_\lambda)_{\lambda \in \Delta_1} $ là một phân bậc kiểu $ \Delta_1 $ và $ (G''_\mu)_{\mu \in \Delta_2} $ là một phân bậc kiểu $ \Delta_2 $ trên $ G $; các phân bậc này được gọi là các *phân bậc từng phần* dẫn xuất từ phân bậc đôi $ (G_{\lambda \mu}) $. Chú ý rằng $ G_{\lambda \mu} = G'_\lambda \cap G''_\mu $; ngược lại, nếu $ (G'_\lambda)_{\lambda \in \Delta_1} $ và $ (G''_\mu)_{\mu \in \Delta_2} $ là hai phân bậc trên $ G $ sao cho $ G $ là tổng trực tiếp của các $ G_{\lambda \mu} = G'_\lambda \cap G''_\mu $, thì các nhóm con này tạo thành một phân bậc đôi của các kiểu $ \Delta_1, \Delta_2 $ trên $ G $, mà trong đó $ (G'_\lambda) $ và $ (G''_\mu) $ là các phân bậc từng phần. Chúng tôi để cho người đọc nhiệm vụ mở rộng điều này đến trường hợp $ \Delta $ là một tích hữu hạn của các tập hợp.

(4) Cho $ \Delta_0 $ là một monoid giao hoán được viết cộng tính, với phần tử đơn vị ký hiệu bởi 0; cho $ I $ là một tập hợp bất kỳ và $ \Delta_0^{(I)} = \Delta $ ký hiệu monoid con của tích $ \Delta_0^I $ gồm các họ $ (\lambda_i)_{i \in I} $ có giá hữu hạn. Cho $ \rho : \Delta \to \Delta_0 $ là đồng cấu toàn ánh (đường chéo) của $ \Delta $ vào $ \Delta_0 $ được xác định bởi $ \rho((\lambda_i)) = \sum_{i \in I} \lambda_i $. Từ mỗi phân bậc kiểu $ \Delta $ ta dẫn xuất được một phân bậc kiểu $ \Delta_0 $ bằng phương tiện của $ \rho $ (*Ví dụ 2*); nó được gọi là *phân bậc toàn phần* liên kết với "phân bậc nhiều" đã cho kiểu $ \Delta $.

Các định nghĩa và ví dụ của số này mở rộng ngay lập tức đến trường hợp $ G $ là một nhóm *không nhất thiết giao hoán*; chỉ cần thay thế khắp nơi khái niệm tổng trực tiếp bằng khái niệm "tổng hạn chế" (\S 1, no. 6, *Nhận xét*). Chú ý rằng trong trường hợp này các $ G_\lambda $ là các nhóm con chuẩn tắc của $ G $ và rằng với $ \lambda \neq \mu $ mọi phần tử của $ G_\lambda $ là hoán vị được với mọi phần tử của $ G_\mu $.

### 2. CÁC VÀNH VÀ MÔĐUN PHÂN BẬC

#### Định nghĩa 2 {#alg-ii-s11-def-2 .statement}

*Một vành $ A $ và một phân bậc $ (A_\lambda) $ kiểu $ \Delta $ trên nhóm cộng $ A $, phân bậc này được nói là tương thích với cấu trúc vành trên $ A $ nếu*

$$
A_\lambda A_\mu \subset A_{\lambda + \mu} \quad \text{với mọi } \lambda, \mu \text{ trong } \Delta.
$$

*Vành $ A $ với phân bậc này khi đó được gọi là một vành phân bậc kiểu $ \Delta $.*

#### Mệnh đề 1 {#alg-ii-s11-prop-1 .statement}

*Nếu mọi phần tử của $ \Delta $ là giản ước được và $ (A_\lambda) $ là một phân bậc kiểu $ \Delta $ tương thích với cấu trúc của một vành $ A $, $ A_0 $ là một vành con của $ A $ (và đặc biệt $ 1 \in A_0 $).*

Vì $ A_0 A_0 \subset A_0 $ theo định nghĩa, chỉ cần chứng minh rằng $ 1 \in A_0 $. Gọi $ 1 = \sum_{\lambda \in \Delta} e_\lambda $ là phân tích của 1 thành các thành phần thuần nhất của nó. Nếu $ x \in A_\mu $, thì $ x = x . 1 = \sum_{\lambda \in \Delta} x e_\lambda $; so sánh các thành phần bậc $ \mu $, (vì $ \mu + \lambda = \mu $ suy ra $ \lambda = 0 $) $ x = x e_0 $. Vì quan hệ này đúng với mọi phần tử thuần nhất của $ A $, nó đúng với mọi $ x \in A $; đặc biệt $ 1 = 1 . e_0 = e_0 \in A_0 $.

#### Định nghĩa 3 {#alg-ii-s11-def-3 .statement}

*Cho $ A $ là một vành phân bậc kiểu $ \Delta $, $ (A_\lambda) $ là phân bậc của nó và $ M $ là một $ A $-môđun trái (resp. phải); một phân bậc $ (M_\lambda) $ kiểu $ \lambda $ trên nhóm cộng $ M $ là tương thích với cấu trúc $ A $-môđun trên $ M $ nếu*

(2)
$$
A_\lambda M_\mu \subset M_{\lambda + \mu} \quad (\text{resp. } M_\mu A_\lambda \subset M_{\lambda + \mu})
$$
*với mọi $ \lambda, \mu $ trong $ \Delta $. Khi đó môđun $ M $ với phân bậc này được gọi là một môđun phân bậc trái (resp. phải) kiểu $ \Delta $ trên vành phân bậc $ A $.*

Khi các phần tử của $ \Delta $ là giản ước được, từ (2) và Mệnh đề 1 suy ra rằng các $ M_\lambda $ là các $ A_0 $-môđun.

Rõ ràng nếu $ A $ là một vành phân bậc kiểu $ \Delta $, thì $ A $-môđun trái $ A_s $ (resp. $ A $-môđun phải $ A_d $) là phân bậc kiểu $ \Delta $.

#### Ví dụ {#alg-ii-s11-n2-exa-1 .statement}

(1) Trên mọi vành $ A $, phân bậc tầm thường kiểu $ \Delta $ là tương thích với cấu trúc vành. Nếu $ A $ được phân bậc bởi phân bậc tầm thường, để một phân bậc $ (M_\lambda) $ kiểu $ \Delta $ trên một $ A $-môđun $ M $ là tương thích với cấu trúc $ A $-môđun, điều kiện cần và đủ là các $ M_\lambda $ là các *môđun con* của $ M $.

(2) Cho $ A $ là một vành phân bậc kiểu $ \Delta $, $ M $ là một $ A $-môđun phân bậc kiểu $ \Delta $ và $ \rho $ là một đồng cấu của $ \Delta $ vào một nửa nhóm giao hoán $ \Delta' $ có phần tử đơn vị được ký hiệu bởi 0. Khi đó $ A $ là một vành phân bậc kiểu $ \Delta' $ và $ M $ là một môđun phân bậc kiểu $ \Delta' $ đối với các phép phân bậc kiểu $ \Delta' $ dẫn xuất từ $ \rho $ và các phép phân bậc kiểu $ \Delta $ trên $ A $ và $ M $ bằng thủ tục của no. 1, *Ví dụ* 1: điều này suy ra ngay lập tức từ quan hệ $ \rho(\lambda + \mu) = \rho(\lambda) + \rho(\mu) $.

Đặc biệt, nếu $ \Delta = \Delta_1 \times \Delta_2 $ là một tích của hai nửa nhóm giao hoán, các phép chiếu $ \mathrm{pr}_1 $ và $ \mathrm{pr}_2 $ là các đồng cấu và các phép phân bậc tương ứng chính là các *phép phân bậc từng phần* dẫn xuất từ các phép phân bậc kiểu $ \Delta $ (no. 1, *Ví dụ* 3); do đó các phép phân bậc từng phần này tương thích với cấu trúc vành của $ A $ và cấu trúc môđun của $ M $.

Tương tự, nếu $ \Delta = \Delta_0^{(r)} $ (trong đó $ \Delta_0 $ là một nửa nhóm giao hoán có phần tử đơn vị được ký hiệu bởi 0), *phép phân bậc toàn phần* (no. 1, Ví dụ 4) kiểu $ \Delta_0 $ dẫn xuất từ phép phân bậc kiểu $ \Delta $ trên $ A $ (resp. $ M $) bằng đồng cấu đường chéo là tương thích với cấu trúc vành trên $ A $ (resp. với cấu trúc môđun trên $ M $).

(3) Cho $ A $ là một vành phân bậc kiểu $ \Delta $, $ M $ là một $ A $-môđun phân bậc kiểu $ \Delta $ và $ \lambda_0 $ là một phần tử của $ \Delta $; với mọi $ \lambda \in \Delta $, đặt $ M'_\lambda = M_{\lambda + \lambda_0} $ và gọi $ M' $ là $ \mathbf{Z} $-môđun $ \bigoplus_{\lambda \in \Delta} M'_\lambda $. Vì $ A_\lambda M'_\mu \subset M_{\lambda + \mu + \lambda_0} = M'_{\lambda + \mu} $, nên $ M' $ là một $ A $-môđun và các $ M'_\lambda $ tạo thành trên $ M' $ một phép phân bậc kiểu $ \Delta $ tương thích với cấu trúc $ A $-môđun của $ M' $; $ A $-môđun phân bậc $ M' $ kiểu $ \Delta $ được xác định như vậy được gọi là thu được bằng cách dịch chuyển bởi $ \lambda_0 $ phép phân bậc của $ M $ và được ký hiệu là $ M(\lambda_0) $. Khi $ \Delta $ là một nhóm, $ A $-môđun nền của $ A $-môđun phân bậc $ M' $ được đồng nhất với $ M $.

*(4) Cho $ B $ là một vành giao hoán. Vành đa thức $ B[X] $ theo một bất định là phân bậc kiểu $ \mathbf{N} $ bởi các môđun con $ BX^n $ ($ n \geqslant 0 $) (xem III, § 2, no. 9 và IV).*

*(5) Cho $ B $ là một vành giao hoán, $ E $ là một $ B $-môđun, $ Q $ là một dạng toàn phương trên $ E $ và $ C(Q) $ là đại số Clifford của $ Q $ (xem IX, § 9). Các $ B $-môđun con $ C^+(Q) $ và $ C^-(Q) $ tạo thành trên $ C(Q) $ một phép phân bậc kiểu $ \mathbf{Z}/2\mathbf{Z} $ tương thích với cấu trúc vành trên $ C(Q) $.*

#### Nhận xét {#alg-ii-s11-n2-rem-1 .statement}

(1) Các phép phân bậc thường được sử dụng nhất là kiểu $ \mathbf{Z} $ hoặc kiểu $ \mathbf{Z}^n $; khi ta nói về các môđun và vành phân bậc (tương ứng phân bậc kép, phân bậc ba, v.v.) mà không nói đến kiểu, ta hiểu rằng ta nói đến các phép phân bậc kiểu $ \mathbf{Z} $ (tương ứng $ \mathbf{Z}^2, \mathbf{Z}^3 $, v.v.); một vành phân bậc (tương ứng môđun) kiểu $ \mathbf{N} $ cũng được gọi là một vành phân bậc (tương ứng môđun) với các bậc dương.

(2) Các $ \mathbf{Z} $-môđun phân bậc kiểu $ \Delta $, khi $ \mathbf{Z} $ có phép phân bậc tầm thường, chính là các nhóm giao hoán phân bậc (mà tập hợp các bậc là một nửa nhóm giao hoán) của Định nghĩa 1 (no. 1).

#### Định nghĩa 4 {#alg-ii-s11-def-4 .statement}

*Cho $ A, A' $ là hai vành phân bậc cùng kiểu $ \Delta $ và $ (A_\lambda), (A'_\lambda) $ là các phép phân bậc tương ứng của chúng. Một đồng cấu vành $ h : A \to A' $ được gọi là phân bậc nếu $ h(A_\lambda) \subset A'_\lambda $ với mọi $ \lambda \in \Delta $.

Cho $ M, M' $ là hai môđun phân bậc kiểu $ \Delta $ trên một vành phân bậc kiểu $ \Delta $. Cho $ u : M \to M' $ là một $ A $-đồng cấu và $ \delta $ là một phần tử của $ \Delta $; $ u $ được gọi là phân bậc bậc $ \delta $ nếu $ u(M_\lambda) \subset M_{\lambda + \delta} $ với mọi $ \lambda \in \Delta $.

Cho $ A $ là một vành phân bậc kiểu $ \Delta $, $ A' $ là một vành phân bậc kiểu $ \Delta' $ và $ \rho : \Delta \to \Delta' $ là một đồng cấu. Một đồng cấu vành $ h : A \to A' $ được gọi là phân bậc nếu $ h $ là một đồng cấu phân bậc của các vành phân bậc kiểu $ \Delta' $ khi $ A $ được trang bị phép phân bậc kiểu $ \Delta' $ dẫn xuất từ phép phân bậc kiểu $ \Delta $ của nó bằng cách dùng $ \rho $ (no. 1, Ví dụ 2); điều này có nghĩa là $ h(A_\lambda) \subset A'_{\rho(\lambda)} $ với mọi $ \lambda \in \Delta $.

Một $ A $-đồng cấu $ u : M \to M' $ được gọi là phân bậc nếu tồn tại $ \delta \in \Delta $ sao cho $ u $ là phân bậc bậc $ \delta $. Nếu $ u \neq 0 $ và mọi phần tử của $ \Delta $ đều giản ước được, thì bậc $ \delta $ của $ u $ khi đó được xác định duy nhất.

Nếu $ h : A \to A', h' : A' \to A'' $ là hai đồng cấu phân bậc của các vành phân bậc kiểu $ \Delta $, thì $ h' \circ h : A \to A'' $ cũng vậy; đối với một ánh xạ $ h : A \to A' $ là một đẳng cấu vành phân bậc, điều kiện cần và đủ là $ h $ song ánh và $ h $ cùng với ánh xạ nghịch đảo $ h' $ là các đồng cấu phân bậc; điều kiện này cũng đủ nếu $ h $ là một đồng cấu phân bậc song ánh. Như vậy thấy rằng các đồng cấu phân bậc có thể được lấy làm các cấu xạ của loài cấu trúc vành phân bậc kiểu $ \Delta $ (*Lý thuyết tập hợp*, IV, § 2, no. 1).

Tương tự, nếu $ u : M \to M' $ và $ u' : M' \to M'' $ là hai đồng cấu phân bậc của các A-môđun phân bậc kiểu $ \Delta $, có các bậc tương ứng $ \delta $ và $ \delta' $, thì $ u' \circ u : M \to M'' $ là một đồng cấu phân bậc có bậc $ \delta + \delta' $. Nếu $ \delta $ có nghịch đảo $ -\delta $ trong $ \Delta $ và $ u : M \to M' $ là một đồng cấu phân bậc song ánh có bậc $ \delta $, ánh xạ nghịch đảo $ u' : M' \to M $ là một đồng cấu phân bậc song ánh có bậc $ -\delta $. Suy ra như trên rằng các *đồng cấu phân bậc có bậc* 0 có thể được lấy làm các cấu xạ của loài các A-môđun phân bậc kiểu $ \Delta $. Nhưng một đồng cấu phân bậc song ánh $ u : M \to N $ có bậc $ \neq 0 $ không phải là một đẳng cấu A-môđun phân bậc nếu $ M $ và $ N $ khác không và các phần tử của $ \Delta $ là giản ước được.

#### Ví dụ {#alg-ii-s11-n2-exa-2 .statement}

(6) Nếu $ M $ là một A-môđun phân bậc và $ M(\lambda_0) $ là một A-môđun phân bậc thu được bằng cách dịch chuyển (no. 2, *Ví dụ 3*), ánh xạ tuyến tính theo $ \mathbf{Z} $ từ $ M(\lambda_0) $ vào $ M $ trùng với đơn ánh chính tắc trên mỗi $ M_{\lambda + \lambda_0} $ là một đồng cấu phân bậc có bậc $ \lambda_0 $ (song ánh khi $ \Delta $ là một *nhóm*).

(7) Nếu $ a $ là một phần tử thuần nhất có bậc $ \delta $ thuộc tâm của $ A $, phép vị tự $ x \mapsto ax $ của mọi A-môđun phân bậc $ M $ là một đồng cấu phân bậc có bậc $ \delta $.

*Nhận xét* (3) Một A-môđun phân bậc $ M $ được gọi là một *A-môđun phân bậc tự do* nếu tồn tại một cơ sở $ (m_i)_{i \in I} $ của $ M $ gồm các phần tử *thuần nhất*. Giả sử điều đó đúng và $ \Delta $ là một *nhóm* giao hoán; gọi $ \lambda_i $ là bậc của $ m_i $ và xét với mỗi $ i $ A-môđun dịch chuyển $ A(-\lambda_i) $ (no. 2, *Ví dụ 3*); nếu $ e_i $ biểu thị phần tử 1 của $ A $ được xét như một phần tử *có bậc* $ \lambda_i $ trong $ A(-\lambda_i) $, ánh xạ A-tuyến tính $ u : \bigoplus_{i \in I} A(-\lambda_i) \to M $ sao cho $ u(e_i) = m_i $ với mọi $ i $, là một *đẳng cấu A-môđun phân bậc*.

Giả sử luôn rằng $ \Delta $ là một nhóm giao hoán, bây giờ cho $ N $ là một A-môđun phân bậc, $ (n_i)_{i \in I} $ là một hệ các phần tử sinh *thuần nhất* của $ N $ và giả sử rằng $ n_i $ có bậc $ \mu_i $. Khi đó ánh xạ A-tuyến tính $ v : \bigoplus_{i \in I} A(-\mu_i) \to N $ sao cho $ u(e_i) = n_i $ với mọi $ i $ là một *đồng cấu môđun A phân bậc toàn ánh có bậc* 0. Nếu $ N $ là một A-môđun phân bậc *sinh hữu hạn*, thì luôn tồn tại một hệ hữu hạn các phần tử sinh thuần nhất của $ N $ và do đó tồn tại một đồng cấu toàn ánh kiểu trên với $ I $ *hữu hạn*.

### 3. CÁC MÔĐUN CON PHÂN BẬC

#### Mệnh đề 2 {#alg-ii-s11-prop-2 .statement}

*Cho A là một vành phân bậc kiểu $ \Delta $, M là một A-môđun phân bậc kiểu $ \Delta $, $ (M_\lambda) $ là phân bậc của nó và N là một môđun con A của M. Các tính chất sau là tương đương:*

(a) $ N $ *là tổng của họ* $ (N \cap M_\lambda)_{\lambda \in \Delta} $.
(b) *Các thành phần thuần nhất của mọi phần tử của N thuộc N*.
(c) $ N $ *được sinh bởi các phần tử thuần nhất*.

Mọi phần tử của N có thể được viết một cách duy nhất thành tổng của các phần tử của các $ M_\lambda $ và do đó ngay lập tức suy ra rằng (a) và (b) là tương đương và rằng (a) kéo theo (c). Ta chứng minh rằng (c) kéo theo (b). Khi đó cho $ (x_i)_{i \in I} $ là một họ các phần tử sinh thuần nhất $ \neq 0 $ của N và cho $ \delta(i) $ là bậc của $ x_i $. Mọi phần tử của N có thể được viết $ \sum_i a_i x_i $ với $ a_i \in A $; nếu $ a_{i,\lambda} $ là thành phần của $ a_i $ có bậc $ \lambda $, kết luận suy ra từ quan hệ

$$
\sum_{i \in I} \left( \sum_{\mu \in \Delta} a_{i,\mu} x_i \right) = \sum_{\lambda \in \Delta} \left( \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i \right).
$$

**Nhận xét (1)** Trong ký hiệu trên, quan hệ $ \sum_{i \in I} a_i x_i = 0 $ do đó tương đương với hệ các quan hệ $ \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i = 0 $. Khi $ \Delta $ là một nhóm, các quan hệ này có thể được viết $ \sum_{i \in I} a_{i,\lambda - \delta(i)} x_i = 0 $.

Khi một môđun con N của M có các tính chất tương đương được nêu trong Mệnh đề 2, rõ ràng các $ N \cap M_\lambda $ tạo thành một phân bậc tương thích với cấu trúc A-môđun của N, gọi là *phân bậc cảm sinh* bởi phân bậc trên M; N với phân bậc này được gọi là một *môđun con phân bậc* của M.

#### Hệ quả 1 {#alg-ii-s11-prop-2-cor-1 .statement}

*Nếu N là một môđun con phân bậc của M và $ (x_i) $ là một hệ sinh của N, các thành phần thuần nhất của các $ x_i $ tạo thành một hệ sinh của N.*

#### Hệ quả 2 {#alg-ii-s11-prop-2-cor-2 .statement}

*Nếu N là một môđun con sinh hữu hạn của M, N thừa nhận một hệ sinh hữu hạn gồm các phần tử thuần nhất.*

Chỉ cần áp dụng Hệ quả 1, lưu ý rằng một phần tử của M chỉ có một số hữu hạn các thành phần thuần nhất $ \neq 0 $.

Một môđun con phân bậc của $ A_s $ (tương ứng $ A_d $) được gọi là một *iđêan trái phân bậc* (tương ứng *phải*) của vành phân bậc A. Với mọi vành con B của $ A(B \cap A_\lambda)(B \cap A_\mu) \subset B \cap A_{\lambda+\mu} $; nếu B là một *môđun con-$\mathbf{Z}$ phân bậc* của A, phân bậc cảm sinh trên B bởi phân bậc trên A do đó tương thích với cấu trúc vành trên B; khi đó B được gọi là một *vành con phân bậc* của A.

Rõ ràng nếu N (tương ứng B) là một môđun con A phân bậc của M (tương ứng một vành con phân bậc của A), đơn ánh chính tắc $ N \to M $ (tương ứng $ B \to A $) là một đồng cấu môđun phân bậc có bậc 0 (tương ứng một đồng cấu vành phân bậc).

Nếu N là một môđun con phân bậc của một A-môđun phân bậc M và $ (M_\lambda)_{\lambda \in \Delta} $ là phân bậc của M, các môđun con $ (M_\lambda + N)/N $ của $ M/N $ tạo thành một *phân bậc* tương thích với cấu trúc của môđun thương này. Thật vậy, nếu $ N_\lambda = M_\lambda \cap N $, $ (M_\lambda + N)/N $ được đồng nhất với $ M_\lambda/N_\lambda $ và suy ra từ Mệnh đề 2 và § 1, no. 6, công thức (26) rằng $ M/N $ là tổng trực tiếp của chúng. Hơn nữa,

$$
A_\lambda(M_\mu + N) \subset A_\lambda M_\mu + N \subset M_{\lambda+\mu} + N
$$

và do đó $ A_\lambda((M_\mu + N)/N) \subset (M_{\lambda+\mu} + N)/N $, điều này xác lập mệnh đề của chúng ta.

Phân bậc $ ((M_\lambda + N)/N)_{\lambda \in \Delta} $ được gọi là phân bậc thương của phân bậc trên M bởi N và môđun thương M/N với phân bậc này được gọi là môđun thương phân bậc của M bởi môđun con phân bậc N; đồng cấu chính tắc M $\to$ M/N là một đồng cấu phân bậc có bậc 0 đối với phân bậc này.

Nếu b là một iđêan hai phía phân bậc của A, phân bậc thương trên A/b tương thích với cấu trúc vành trên A/b; vành A/b với phân bậc này được gọi là vành phân bậc thương của A bởi b; đồng cấu chính tắc A $\to$ A/b là một đồng cấu vành phân bậc đối với phân bậc này.

#### Mệnh đề 3 {#alg-ii-s11-prop-3 .statement}

*Cho A là một vành phân bậc kiểu $\Delta$, M, N là hai A-môđun phân bậc kiểu $\Delta$ và u: M \to N là một đồng cấu A phân bậc có bậc $\delta$. Khi đó:*
(i) Im(u) là một môđun con phân bậc của N.
(ii) *Nếu $\delta$ là một phần tử chính quy của $\Delta$, Ker(u) là một môđun con phân bậc của M.*
(iii) *Nếu $\delta = 0$, song ánh M/Ker(u) \to Im(u) liên kết một cách chính tắc với u là một đẳng cấu của các môđun phân bậc.*

Mệnh đề (i) suy ra ngay lập tức từ các định nghĩa và Mệnh đề 2(c). Nếu x là một phần tử của M sao cho u(x) = 0 và x = \sum_\lambda x_\lambda là phân tích của nó thành các thành phần thuần nhất (trong đó x_\lambda có bậc \lambda), thì

$$
\sum_\lambda u(x_\lambda) = u(x) = 0
$$

và u(x_\lambda) có bậc \lambda + \delta; nếu \delta là chính quy thì quan hệ \lambda + \delta = \mu + \delta kéo theo \lambda = \mu, do đó các u(x_\lambda) là các thành phần thuần nhất của u(x) và tất yếu u(x_\lambda) = 0 với mọi \lambda \in \Delta, điều này chứng minh (ii). Song ánh v: M/Ker(u) \to Im(u) liên kết một cách chính tắc với u khi đó là một đồng cấu phân bậc có bậc \delta, như suy ra từ định nghĩa của phân bậc thương; do đó (iii) khi \delta = 0.

#### Hệ quả {#alg-ii-s11-n3-cor-1 .statement}

*Cho A, B là hai vành phân bậc kiểu $\Delta$ và u: A \to B là một đồng cấu phân bậc của các vành phân bậc. Khi đó Im(u) là một môđun con phân bậc của B, Ker(u) là một iđêan hai phía phân bậc của A và song ánh A/Ker(u) \to Im(u) liên kết một cách chính tắc với u là một đẳng cấu của các vành phân bậc.*

Chỉ cần áp dụng Mệnh đề 3 cho u được xem như một đồng cấu bậc 0 của các môđun phân bậc $\mathbf{Z}$.

#### Mệnh đề 4 {#alg-ii-s11-prop-4 .statement}

*Cho A là một vành phân bậc kiểu $\Delta$ và M là một A-môđun phân bậc kiểu $\Delta$.*
(i) *Mọi tổng và mọi giao của các môđun con phân bậc của M là một môđun con phân bậc.*
(ii) *Nếu x là một phần tử thuần nhất của M có bậc $\mu$ giản ước được trong $\Delta$, linh hóa tử của x là một iđêan trái phân bậc của A.*
(iii) *Nếu mọi phần tử của $\Delta$ đều giản ước được, linh hóa tử của một môđun con phân bậc của M là một iđêan hai phía phân bậc của A.*

Nếu $(\mathbf{N}_i)$ là một họ các môđun con phân bậc của $M$, tính chất (c) của Mệnh đề 2 chỉ ra rằng tổng của các $\mathbf{N}_i$ được sinh bởi các phần tử thuần nhất và tính chất (b) của Mệnh đề 2 chứng minh rằng các thành phần thuần nhất của mọi phần tử của $\bigcap_i \mathbf{N}_i$ thuộc $\bigcap_i \mathbf{N}_i$; do đó có (i).

Để chứng minh (ii), chỉ cần chú ý rằng $\operatorname{Ann}(x)$ là hạt nhân của đồng cấu $a \mapsto ax$ của A-môđun $A_s$ vào $M$ và rằng đồng cấu này là phân bậc có bậc $\mu$; kết luận suy ra từ Mệnh đề 3(ii). Cuối cùng (iii) là một hệ quả của (i) và (ii) vì linh hóa tử của một môđun con phân bậc $N$ của $M$ là giao của các linh hóa tử của các phần tử thuần nhất của $N$, theo Mệnh đề 2.

#### Nhận xét 2 {#alg-ii-s11-n3-rem-2 .statement}

Cho $M$ là một A-môđun phân bậc và $E$ là một môđun con của $M$; suy ra từ Mệnh đề 4(i) rằng tồn tại một môđun con phân bậc *lớn nhất* $N'$ của $M$ được chứa trong $E$ và một môđun con phân bậc *nhỏ nhất* $N''$ của $M$ chứa $E$; $N'$ là tập hợp các $x \in E$ mà mọi thành phần thuần nhất của nó thuộc $E$ và $N''$ là môđun con của $M$ được sinh bởi các thành phần thuần nhất của một hệ sinh của $E$.

#### Mệnh đề 5 {#alg-ii-s11-prop-5 .statement}

*Cho $A$ là một vành phân bậc kiểu $\Delta$. Nếu mọi phần tử của $\Delta$ đều giản ước được, thì, với mọi phần tử thuần nhất $a \in A$, bộ giao hoán của $a$ trong $A$ (I, § 1, no. 5) là một vành con phân bậc của $A$.*

Giả sử rằng $a$ có bậc $\delta$; đặt $b = \sum_\lambda b_\lambda$ là một phần tử giao hoán được với $a$, $b_\lambda$ là thành phần thuần nhất của $b$ có bậc $\lambda$ với mọi $\lambda \in \Delta$. Khi đó theo giả thiết $\sum_\lambda (ab_\lambda - b_\lambda a) = 0$ và $ab_\lambda - b_\lambda a$ là thuần nhất có bậc $\lambda + \delta$; vì $\delta$ giản ước được, suy ra rằng $ab_\lambda = b_\lambda a$ với mọi $\lambda$, điều này chứng minh mệnh đề của ta.

#### Hệ quả {#alg-ii-s11-n3-cor-2 .statement}

*Nếu mọi phần tử của $\Delta$ đều giản ước được, bộ giao hoán của vành con phân bậc $B$ của $A$ (và đặc biệt là tâm của $A$) là một vành con phân bậc của $A$.*

Nó là giao của các bộ giao hoán của các phần tử thuần nhất của $B$.

Nhận xét (3) *Một hệ trực tiếp $(A_\alpha, \phi_{\beta\alpha})$ của các vành phân bậc kiểu $\Delta$ (tương ứng, một hệ trực tiếp $(M_\alpha, f_{\beta\alpha})$ của các môđun $A_\alpha$ phân bậc kiểu $\Delta$) là một hệ trực tiếp của các vành (tương ứng, các môđun $A_\alpha$) sao cho mỗi $A_\alpha$ (tương ứng, $M_\alpha$) là phân bậc kiểu $\Delta$ và mỗi $\phi_{\beta\alpha}$ (tương ứng, $f_{\beta\alpha}$) là một *đồng cấu của các vành phân bậc* (tương ứng, một *đồng cấu $A_\alpha$* bậc 0 của *các môđun phân bậc*). Nếu $(A^\lambda_\alpha)_{\lambda \in \Delta}$ (tương ứng, $(M^\lambda_\alpha)_{\lambda \in \Delta}$) là phân bậc của $A_\alpha$ (tương ứng, $M_\alpha$) và ta viết

$$
A = \lim_{\longrightarrow} A_\alpha,\quad A^\lambda = \lim_{\longrightarrow} A^\lambda_\alpha \quad (\text{resp. } M = \lim_{\longrightarrow} M_\alpha,\ M^\lambda = \lim_{\longrightarrow} M^\lambda_\alpha),
$$

thì theo § 6, no. 2, Mệnh đề 5, $(A^\lambda)$ (tương ứng, $(M^\lambda)$) là một phân bậc của A (tương ứng, M) và theo I, § 10, nos. 3 và 4, phân bậc này tương thích với cấu trúc vành trên A (tương ứng, cấu trúc A-môđun trên M). Vành phân bậc A (tương ứng, môđun A phân bậc M) được gọi là giới hạn trực tiếp của hệ trực tiếp của các vành phân bậc $(A_\alpha, \phi_{\beta\alpha})$ (tương ứng, các môđun phân bậc $(M_\alpha, f_{\beta\alpha})$). Nếu $\phi_\alpha : A_\alpha \to A$ (tương ứng, $f_\alpha : M_\alpha \to M$) là ánh xạ chính tắc, thì $\phi_\alpha$ (tương ứng, $f_\alpha$) là một đồng cấu của các vành phân bậc (tương ứng, một đồng cấu bậc 0 của các môđun $A_\alpha$ phân bậc).

### 4. TRƯỜNG HỢP NHÓM CÁC BẬC CÓ THỨ TỰ

Một cấu trúc có thứ tự (ký hiệu bởi $\leq$) trên một nhóm giao hoán $\Delta$ được viết theo phép cộng được gọi là *tương thích* với cấu trúc nhóm nếu, với mọi $\rho \in \Delta$, quan hệ $\lambda \leq \mu$ kéo theo $\lambda + \rho \leq \mu + \rho$. Khi đó, nhóm $\Delta$ với cấu trúc có thứ tự này được gọi là một *nhóm có thứ tự*. Ta sẽ nghiên cứu chi tiết các nhóm này trong VI, § 1; ở đây ta chỉ giới hạn ở nhận xét rằng trong một nhóm như vậy, quan hệ $\lambda > 0$ kéo theo $\lambda + \mu > \mu$ với mọi $\mu$, vì theo định nghĩa nó kéo theo $\lambda + \mu \geq \mu$ và quan hệ $\xi + \mu = \mu$ tương đương với $\xi = 0$.

Cho $\Delta$ là một nhóm giao hoán có thứ tự, A là một vành phân bậc kiểu $\Delta$ và $(A_\lambda)$ là phân bậc của nó, và giả sử rằng quan hệ $A_\lambda \neq \{0\}$ kéo theo $\lambda \geq 0$; khi đó từ các định nghĩa suy ra rằng $\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$ là một *iđêan hai phía phân bậc* của A, theo nhận xét vừa nêu.

#### Mệnh đề 6 {#alg-ii-s11-prop-6 .statement}

*Cho $\Delta$ là một nhóm giao hoán có thứ tự, A là một vành phân bậc kiểu $\Delta$, $(A_\lambda)$ là phân bậc của nó, M là một môđun A phân bậc kiểu $\Delta$ và $(M_\lambda)$ là phân bậc của nó. Giả sử rằng quan hệ $A_\lambda \neq \{0\}$ kéo theo $\lambda \geq 0$ và tồn tại $\lambda_0$ sao cho $M_{\lambda_0} \neq \{0\}$ và $M_\lambda = \{0\}$ với $\lambda < \lambda_0$. Khi đó, nếu $\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$, thì $\mathfrak{I}_0 M \neq M$.*

Cho $x$ là một phần tử khác không của $M_{\lambda_0}$; giả sử rằng $x \in \mathfrak{I}_0 M$. Khi đó $x = \sum_i a_i x_i$, trong đó các $a_i$ là các phần tử thuần nhất $\neq 0$ của $\mathfrak{I}_0$ và các $x_i$ là các phần tử thuần nhất $\neq 0$ của M với $\deg(x) = \deg(a_i) + \deg(x_i)$ với mọi $i$ (no. 2). Nhưng, vì $\deg(a_i) > 0$, $\lambda_0 = \deg(a_i) + \deg(x_i) > \deg(x_i)$, điều này mâu thuẫn với giả thiết.

#### Hệ quả 1 {#alg-ii-s11-prop-6-cor-1 .statement}

*Với các giả thiết trên $\Delta$ và A của Mệnh đề 6, nếu M là một A-môđun phân bậc sinh hữu hạn sao cho $\mathfrak{I}_0 M = M$, thì $M = \{0\}$.*

Giả sử $M \neq \{0\}$. Gọi $\lambda_0$ là một phần tử cực tiểu của tập hợp các bậc của một hệ sinh hữu hạn của M gồm các phần tử thuần nhất $\neq 0$; khi đó các giả thiết của Mệnh đề 6 được thỏa mãn, điều này dẫn đến một mâu thuẫn.

#### Hệ quả 2 {#alg-ii-s11-prop-6-cor-2 .statement}

*Với các giả thiết trên $\Delta$ và A của Mệnh đề 6, cho M là một* A-môđun phân bậc sinh hữu hạn và $ \mathbf{N} $ là một môđun con phân bậc của $ \mathbf{M} $ sao cho $ \mathbf{N} + \mathfrak{J}_0 \mathbf{M} = \mathbf{M} $; khi đó $ \mathbf{N} = \mathbf{M} $.

$ \mathbf{M}/\mathbf{N} $ là một A-môđun phân bậc sinh hữu hạn và giả thiết suy ra rằng $ \mathfrak{J}_0 . (\mathbf{M}/\mathbf{N}) = \mathbf{M}/\mathbf{N} $; do đó $ \mathbf{M}/\mathbf{N} = 0 $.

#### Hệ quả 3 {#alg-ii-s11-prop-6-cor-3 .statement}

*Với các giả thiết trên $ \Delta $ và $ \mathbf{A} $ của Mệnh đề 6, cho $ u : \mathbf{M} \to \mathbf{N} $ là một đồng cấu phân bậc của các A-môđun phải phân bậc $ \mathbf{A} $, trong đó $ \mathbf{N} $ được giả thiết là sinh hữu hạn. Nếu đồng cấu*

$$
u \otimes 1 : \mathbf{M} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) \to \mathbf{N} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

*là toàn ánh, thì $ u $ là toàn ánh.*

$ u(\mathbf{M}) $ là một môđun con phân bậc của $ \mathbf{N} $ và $ (\mathbf{A}/\mathfrak{J}_0) $-môđun

$$
(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

là đẳng cấu với $ (N \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0))/\mathrm{Im}(u \otimes 1) $ (\S 3, no. 6, Mệnh đề 6). Giả thiết do đó suy ra $ (N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) = 0 $ và do đó $ \mathbf{N} = u(\mathbf{M}) $ theo Hệ quả 1.

#### Nhận xét {#alg-ii-s11-n4-rem-1 .statement}

Từ chứng minh của Hệ quả 1 suy ra rằng Hệ quả 1 và 2 (tương ứng Hệ quả 3) vẫn đúng khi, thay vì giả sử rằng $ \mathbf{M} $ (tương ứng $ \mathbf{N} $) là sinh hữu hạn, đưa ra giả thiết sau: tồn tại một tập con $ \Delta^+ $ của $ \Delta $ thỏa mãn các điều kiện sau:

(1) với $ \lambda \notin \Delta^+ $, $ M_\lambda = \{0\} $ (tương ứng $ N_\lambda = \{0\} $);
(2) mọi tập con khác rỗng của $ \Delta^+ $ đều có một phần tử nhỏ nhất.

Điều này xảy ra nếu $ \Delta = \mathbf{Z} $ và $ \mathbf{M} $ (tương ứng $ \mathbf{N} $) là một môđun phân bậc với các bậc *dương*.

#### Mệnh đề 7 {#alg-ii-s11-prop-7 .statement}

*Giả sử rằng $ \Delta = \mathbf{Z} $. Với các giả thiết về $ \mathbf{A} $ và $ \mathbf{M} $ của Mệnh đề 6, xét môđun $ \mathbf{A}_0 $-phân bậc $ \mathbf{N} = \mathbf{M}/\mathfrak{J}_0 \mathbf{M} $ và giả sử các điều kiện sau được thỏa mãn:
(i) mỗi $ N_\lambda $ được xét như một $ \mathbf{A}_0 $-môđun đều có một cơ sở $ (y_{i\lambda})_{i \in I_\lambda} $;
(ii) đồng cấu chính tắc $ \mathfrak{J}_0 \otimes_{\mathbf{A}} \mathbf{M} \to \mathbf{M} $ là đơn ánh.

Khi đó $ \mathbf{M} $ là một $ \mathbf{A} $-môđun tự do phân bậc (no. 2, Nhận xét 3) và, chính xác hơn, nếu $ x_{i\lambda} $ là một phần tử của $ M_\lambda $ có ảnh trong $ N_\lambda $ là $ y_{i\lambda} $, thì họ $ (x_{i\lambda})_{(i, \lambda) \in I} $ (trong đó $ I $ là tập hợp các $ I_\lambda $) là một cơ sở của $ \mathbf{M} $.*

Ta biết (no. 2, *Nhận xét 3*) rằng có một $ \mathbf{A} $-môđun tự do phân bậc $ \mathbf{L} $ (có phân bậc $ (L_\lambda) $) và một đồng cấu toàn ánh $ p : \mathbf{L} \to \mathbf{M} $ bậc 0 sao cho $ p(e_{i\lambda}) = x_{i\lambda} $ với mọi $ (i, \lambda) \in I $ ($ (e_{i\lambda})_{(i, \lambda) \in I} $ là một cơ sở của $ \mathbf{L} $ gồm các phần tử thuần nhất $ e_{i\lambda} \in L_\lambda $). Theo *Nhận xét* trên, suy ra rằng $ p $ là *toàn ánh*. Xét môđun $ \mathbf{A} $-phân bậc $ \mathbf{R} = \mathrm{Ker}(p) $ và lưu ý rằng $ R_\lambda = \{0\} $ với $ \lambda < \lambda_0 $ theo định nghĩa; ta cần chứng minh rằng $ \mathbf{R} = \{0\} $ và theo Mệnh đề 6, chỉ cần chứng minh rằng $ \mathfrak{J}_0 R = R $. Xét biểu đồ giao hoán (\S 3, no. 6, Mệnh đề 5)

$$
\begin{array}{ccccccccc}
\mathfrak{J}_0 \otimes R & \xrightarrow{1 \otimes j} & \mathfrak{J}_0 \otimes L & \xrightarrow{1 \otimes p} & \mathfrak{J}_0 \otimes M & \longrightarrow & 0 \\
\downarrow a & & \downarrow b & & \downarrow c & & \\
0 & \longrightarrow & R & \xrightarrow{f} & L & \xrightarrow{p} & M & \longrightarrow & 0
\end{array}
$$

trong đó $ j $ là đơn ánh chính tắc, $ a, b, c $ suy ra từ đơn ánh chính tắc $ \mathfrak{J}_0 \to A $ (\S 3, no. 4, Mệnh đề 4); cần chứng minh rằng $ a $ là toàn ánh. Lưu ý rằng, vì $ L $ là tự do, $ b $ là đơn ánh (\S 3, no. 7, Hệ quả 6 của Mệnh đề 7) và $ c $ là đơn ánh theo giả thiết. Khi đó, cho $ t $ là một phần tử của $ R $ và $ t $ là lớp của nó trong $ R / \mathfrak{J}_0 R $; khi đó có một dãy khớp (\S 3, no. 6, Mệnh đề 5 và Hệ quả 2 của Mệnh đề 6)

$$
R / \mathfrak{J}_0 R \xrightarrow{j} L / \mathfrak{J}_0 L \xrightarrow{\bar{p}} M / \mathfrak{J}_0 M \longrightarrow 0
$$

trong đó $ j $ và $ \bar{p} $ được suy ra từ $ j $ và $ p $ khi chuyển qua các thương và $ \bar{p} $ theo giả thiết là một song ánh; khi đó $ j(\bar{t}) = 0 $, nói cách khác $ j(t) \in \mathfrak{J}_0 L $. Khi đó tồn tại một phần tử $ z \in \mathfrak{J}_0 \otimes L $ sao cho $ j(t) = b(z) $; vì $ p(b(z)) = 0 $, $ c((1 \otimes p)(z)) = 0 $ và, vì $ c $ là đơn ánh, $ (1 \otimes p)(z) = 0 $. Nói cách khác, $ z $ là ảnh của một phần tử $ t' \in \mathfrak{J}_0 \otimes R $ qua $ 1 \otimes j $ và khi đó $ j(a(t')) = b(z) = j(t) $; vì $ j $ là đơn ánh, điều này kéo theo $ t = a(t') $.

Sau này chúng ta sẽ chỉ ra (Đại số giao hoán, II, \S 3, no. 2, Mệnh đề 5) cách mở rộng mệnh đề này cho các môđun không phân bậc.

#### Bổ đề 1 {#alg-ii-s11-lem-1 .statement}

*Đối với một nhóm giao hoán $ \Delta $, để tồn tại trên $ \Delta $ một thứ tự toàn phần tương thích với cấu trúc nhóm của $ \Delta $, điều kiện cần và đủ là $ \Delta $ không xoắn.*

Nếu tồn tại một cấu trúc thứ tự như vậy trên $ \Delta $ và nếu $ \lambda > 0 $, thì $ \lambda + \mu > 0 $ với mọi $ \mu \geq 0 $ và đặc biệt, bằng quy nạp theo số nguyên $ n > 0 $, $ n.\lambda > 0 $, điều này chứng minh rằng $ \Delta $ không xoắn (vì mọi phần tử $ \neq 0 $ của $ \Delta $ hoặc là $ > 0 $ hoặc là $ < 0 $). Ngược lại, nếu $ \Delta $ không xoắn, $ \Delta $ là một môđun con-$ \mathbf{Z} $ của một không gian vectơ $ \mathbf{Q} $ (\S 7, no. 10, Hệ quả 1 của Mệnh đề 26) mà có thể giả sử có dạng $ \mathbf{Q}^{(I)} $; nếu $ I $ được cho một thứ tự tốt (*Lý thuyết tập hợp*, III, \S 2, no. 3, Định lý 1) và $ \mathbf{Q} $ thứ tự thông thường của nó, tập hợp $ \mathbf{Q}^{(I)} $ với *thứ tự từ điển* là được sắp thứ tự toàn phần (*Lý thuyết tập hợp*, III, \S 2, no. 6); hiển nhiên thứ tự này tương thích với cấu trúc nhóm cộng của $ \mathbf{Q}^{(I)} $.

#### Mệnh đề 8 {#alg-ii-s11-prop-8 .statement}

*Cho $ \Delta $ là một nhóm giao hoán không xoắn và $ A $ là một vành phân bậc kiểu $ \Delta $. Nếu tích trong $ A $ của hai phần tử thuần nhất $ \neq 0 $ là $ \neq 0 $, thì vành $ A $ không có ước của 0.*

Cho $ \Delta $ được trang bị một thứ tự toàn phần tương thích với cấu trúc nhóm của nó (Bổ đề

1) và cho $ x = \sum_{\lambda \in \Delta} x_\lambda, y = \sum_{\lambda \in \Delta} y_\lambda $ là hai phần tử khác không của $ A $ ($ x_\lambda $ và $ y_\lambda $ là thuần nhất có bậc $ \lambda $ với mọi $ \lambda \in \Delta $); gọi $ \alpha $ (tương ứng $ \beta $) là phần tử lớn nhất trong các phần tử $ \lambda \in \Delta $ sao cho $ x_\lambda \neq 0 $ (tương ứng $ y_\lambda \neq 0 $); rõ ràng rằng nếu $ \lambda \neq \alpha $ hoặc $ \mu \neq \beta $, thì hoặc $ x_\lambda y_\mu = 0 $ hoặc $ \deg(x_\lambda y_\mu) < \alpha + \beta $; thành phần thuần nhất của $ xy $ có bậc $ \alpha + \beta $ do đó là $ x_\alpha y_\beta $, phần tử này khác không theo giả thiết; do đó $ xy \neq 0 $.

### 5. TÍCH TENXƠ PHÂN BẬC CỦA CÁC MÔĐUN PHÂN BẬC

Cho $ \Delta $ là một nửa nhóm giao hoán với phần tử đơn vị của nó được ký hiệu là 0, $ A $ là một vành phân bậc kiểu $ \Delta $ và $ M $ (tương ứng $ N $) là một A-môđun phải (tương ứng trái) phân bậc kiểu $ \Delta $. Gọi $ (A_\lambda) $ (tương ứng $ (M_\lambda), (N_\lambda) $) là sự phân bậc của $ A $ (tương ứng $ M, N $); tích tenxơ $ M \otimes_{\mathbf{Z}} N $ của các $\mathbf{Z}$-môđun $ M $ và $ N $ là tổng trực tiếp của các $ M_\lambda \otimes_{\mathbf{Z}} N_\mu $ (\S 3, no. 7, Mệnh đề 7) và do đó các môđun sau tạo thành một *sự phân bậc kép* kiểu $ \Delta, \Delta $ trên $\mathbf{Z}$-môđun này. Xét trên $ M \otimes_{\mathbf{Z}} N $ *sự phân bậc toàn phần* kiểu $ \Delta $ liên kết với sự phân bậc kép này (no. 1, *Ví dụ 4*); nó gồm các môđun con-$\mathbf{Z}$ $ P_\lambda = \sum_{\mu + \nu = \lambda} (M_\mu \otimes_{\mathbf{Z}} N_\nu) $. Ta biết rằng $\mathbf{Z}$-môđun $ M \otimes_A N $ là môđun thương của $ M \otimes_{\mathbf{Z}} N $ theo môđun con-$\mathbf{Z}$ $ Q $ sinh bởi các phần tử $ (xa) \otimes y - x \otimes (ay) $, trong đó $ x \in M, y \in N $ và $ a \in A $ (\S 3, no. 1); nếu, với mọi $ \lambda \in \Delta $, $ x_\lambda, y_\lambda, a_\lambda $ là các thành phần thuần nhất có bậc $ \lambda $ của $ x, y, a $ tương ứng, thì rõ ràng $ (xa) \otimes y - x \otimes (zy) $ là tổng của các phần tử thuần nhất $ (x_\lambda a_\nu) \otimes y_\mu - x_\lambda \otimes (a_\nu y_\mu) $, nói cách khác $ Q $ là một môđun con-$\mathbf{Z}$ *phân bậc* của $ M \otimes_{\mathbf{Z}} N $ (no. 3, Mệnh đề 2) và thương

$$
M \otimes_A N = (M \otimes_{\mathbf{Z}} N)/Q
$$

do đó có một cách chính tắc một cấu trúc môđun $\mathbf{Z}$ phân bậc kiểu $\Delta$ (no. 3). Hơn nữa (no. 3, Mệnh đề 5), *tâm* $C$ của $A$ là một vành con phân bậc của $A$; phép phân bậc mà ta vừa định nghĩa trên $M \otimes_A N$ là *tương thích với cấu trúc môđun của nó trên vành phân bậc* $C$. Vì $M \otimes_{\mathbf{Z}} N$ có một cách chính tắc *hai* cấu trúc $C$-môđun, mà theo đó lần lượt $c(x \otimes y) = (xc) \otimes y$ và $(x \otimes y)c = x \otimes (cy)$ với $x \in M, y \in N, c \in C$ (\S 3, no. 3); nếu $x \in M_\lambda, y \in N_\mu, c \in C \cap A_v$, thì hai phần tử $c(x \otimes y)$ và $(x \otimes y)c$ thuộc $(M \otimes_{\mathbf{Z}} N)_{\lambda + \mu + v}$ và hiệu của chúng thuộc $Q$, do đó ảnh chung của chúng trong $M \otimes_A N$ thuộc $(M \otimes_A N)_{\lambda + \mu + v}$, điều này chứng minh mệnh đề của ta. Khi nói đến $M \otimes_A N$ như một *môđun* $C$-*phân bậc*, ta luôn muốn nói đến cấu trúc được định nghĩa như trên, trừ khi có nói khác. Chú ý rằng $(M \otimes_A N)_\lambda$ có thể được định nghĩa là nhóm cộng của $M \otimes_A N$ sinh bởi các $x_\mu \otimes y_\nu$, trong đó $x_\mu \in M_\mu, y_\nu \in N_\nu$ và $\mu + \nu = \lambda$.

Cho $M'$ (tương ứng $N'$) là một môđun $A$-phải (tương ứng trái) phân bậc khác và $u : M \to M', v : N \to N'$ là các đồng cấu phân bậc có các bậc tương ứng là $\alpha$ và $\beta$. Khi đó ngay lập tức suy ra từ nhận xét trên rằng $u \otimes v$ là một đồng cấu *phân bậc* $(C$-môđun) có bậc $\alpha + \beta$.

Khi $A$ giao hoán, một phép phân bậc (tương thích với cấu trúc $A$-môđun) cũng được định nghĩa trên tích tenxơ của một số hữu hạn bất kỳ các $A$-môđun phân bậc; hơn nữa, ngay lập tức thấy rằng các đẳng cấu kết hợp như $(M \otimes N) \otimes P \to M \otimes (N \otimes P)$ ($ \S 3 $, no. 8, Mệnh đề 8) là các đẳng cấu của các môđun *phân bậc*.

#### Nhận xét {#alg-ii-s11-n5-rem-1 .statement}

Khi $A$ có phép phân bậc *tầm thường* (no. 1, *Ví dụ* 1), khi đó $(M \otimes_A N)_\lambda$ đơn giản là tổng trực tiếp của các $Y$-môđun con $M_\mu \otimes_A N_\nu$ của $M \otimes_A N$ sao cho $\mu + \nu = \lambda$.

Cho $ M $ (tương ứng $ N $) là một môđun phải phân bậc (tương ứng trái) $ A $ kiểu $ \Delta $, $ P $ là một môđun $ \mathbf{Z} $ phân bậc kiểu $ \Delta $ và $ f $ là một ánh xạ $ \mathbf{Z} $-song tuyến tính từ $ M \times N $ vào $ P $ thỏa mãn điều kiện (1) của $ \S 3 $, no. 1, và hơn nữa sao cho
$$
f(x_\lambda, y_\mu) \in P_{\lambda+\mu} \quad \text{cho } x_\lambda \in M_\lambda, y_\mu \in N_\mu, \lambda, \mu \text{ thuộc } \Delta.
$$
Khi đó $ f(x, y) = g(x \otimes y) $, trong đó $ g : M \otimes_A N \to P $ là một ánh xạ $ \mathbf{Z} $-tuyến tính ($ \S 3 $, no. 1, Mệnh đề 1) và suy ra từ điều kiện trên rằng $ g $ là một đồng cấu môđun $ \mathbf{Z} $ phân bậc *phân bậc* bậc 0.

Cho $ B $ là một vành phân bậc khác kiểu $ \Delta $ và $ \rho : A \to B $ là một đồng cấu của các vành phân bậc (no. 2); khi đó $ \rho^*(B_d) $ là một môđun phải $ A $ phân bậc kiểu $ \Delta $. Nếu $ E $ là một môđun trái $ A $ phân bậc kiểu $ \Delta $ và $ \rho^*(B_d) \otimes_A E $ được cho cấu trúc môđun $ \mathbf{Z} $ phân bậc kiểu $ \Delta $ được định nghĩa ở trên, thì cấu trúc môđun trái $ B $ chính tắc ($ \S 5 $, no. 1) tương thích với phân bậc của
$$
E_{(B)} = \rho^*(E) = \rho^*(B_d) \otimes_A E.
$$
Môđun $ B $ phân bậc thu được như vậy được gọi là thu được bằng cách mở rộng vành vô hướng tới $ B $ nhờ $ \rho $ và khi ta nói về $ E_{(B)} $ hoặc $ \rho^*(E) $ như một môđun $ B $ phân bậc, ta luôn luôn hiểu là cấu trúc này, trừ khi có nói khác đi.

### 6. CÁC MÔĐUN PHÂN BẬC CỦA CÁC ĐỒNG CẤU PHÂN BẬC

Ta giả sử trong số này rằng nửa nhóm $ \Delta $ là một *nhóm*. Cho $ A $ là một vành phân bậc kiểu $ \Delta $ và $ M, N $ là hai $ A $-môđun trái phân bậc (chẳng hạn) kiểu $ \Delta $. Ký hiệu $ H_\lambda $ là nhóm cộng của các *đồng cấu thuần nhất bậc* $ \lambda $ của $ M $ vào $ N $ (no. 2); trong nhóm cộng $ \mathrm{Hom}_A(M, N) $ của *tất cả* các đồng cấu của $ M $ vào $ N $ (với các cấu trúc $ A $-môđun *không phân bậc*) tổng (với $ \lambda \in \Delta $) của các $ H_\lambda $ là *trực tiếp*. Thật vậy, nếu có một quan hệ $ \sum_\lambda u_\lambda = 0 $ với $ u_\lambda \in H_\lambda $ với mọi $ \lambda $, thì suy ra $ \sum_\lambda u_\lambda(x_\mu) = 0 $ với mọi $ \mu $ và mọi $ x_\mu \in M_\mu $. Vì các phần tử của $ \Delta $ là giản ước được, $ u_\lambda(x_\mu) $ là thành phần thuần nhất của $ \sum_\lambda u_\lambda(x_\mu) $ có bậc $ \lambda + \mu $; do đó $ u_\lambda(x_\mu) = 0 $ với mọi cặp có thứ tự $ (\mu, \lambda) $ và mọi $ x_\mu \in M_\mu $, điều này kéo theo $ u_\lambda = 0 $ với mọi $ \lambda \in \Delta $. Ta sẽ ký hiệu (trong đoạn này) bởi $ \mathrm{Homgr}_A(M, N) $ nhóm con cộng tính của $ \mathrm{Hom}_A(M, N) $ là tổng của các $ H_\lambda $ và ta sẽ gọi nó là nhóm cộng của các $ A $-*đồng cấu môđun* phân bậc của $ M $ vào $ N $. Cho $ C $ là tâm của $ A $, là một vành con phân bậc (no. 3, Hệ quả của Mệnh đề 5); đối với cấu trúc $ C $-môđun chính tắc trên $ \mathrm{Hom}_A(M, N) $ ($ \S 1 $, no. 14, *Nhận xét* 1), $ \mathrm{Homgr}_A(M, N) $ là một *môđun con* và phép phân bậc $ (H_\lambda) $ là *tương thích* với cấu trúc $ C $-môđun: thật vậy, nếu $ c_v \in C \cap A_v $, $ x_\mu \in N_\mu $ và $ u_\lambda \in H_\lambda $, thì theo định nghĩa $ (c_vu_\lambda)(x_\mu) = c_v.u_\lambda(x_\mu) \subset N_{\lambda+\mu+v} $ và do đó $ c_vu_\lambda \in H_{\lambda+v} $.

Cho $ M' $ và $ N' $ là hai $ A $-môđun trái phân bậc kiểu $ \Delta $ và $ u': M' \to M $, $ v': N \to N' $ là các đồng cấu phân bậc có các bậc tương ứng $ \alpha $ và $ \beta $. Khi đó ngay lập tức có rằng $ \mathrm{Hom}(u', v'): w \mapsto v' \circ w \circ u' $ ánh xạ $ \mathrm{Homgr}_A(M, N) $ vào $ \mathrm{Homgr}_A(M', N') $ và rằng hạn chế của nó trên $ \mathrm{Homgr}_A(M, N) $ là một đồng cấu *phân bậc* vào $ \mathrm{Homgr}_A(M', N') $ *có bậc* $ \alpha + \beta $.

Đặc biệt $ \mathrm{Homgr}_A(M, M) $ là một *vành con phân bậc* của $ \mathrm{End}_A(M) $, được ký hiệu là $ \mathrm{Endgr}_A(M) $.

#### Nhận xét {#alg-ii-s11-n6-rem-1 .statement}

Nếu $ M $ và $ N $ là các $ A $-môđun trái phân bậc, $ \mathrm{Homgr}_A(M, N) $ nói chung phân biệt với $ \mathrm{Hom}_A(M, N) $. Tuy nhiên hai tập hợp này bằng nhau khi $ M $ là một $ A $-môđun *sinh hữu hạn*. Vì khi đó $ M $ được sinh bởi một số hữu hạn các phần tử thuần nhất $ x_i $ ($ 1 \leq i \leq n $); gọi $ d(i) $ là bậc của $ x_i $; cho $ u \in \mathrm{Hom}_A(M, N) $ và với mọi $ \lambda \in \Delta $ gọi $ z_{i,\lambda} $ là thành phần thuần nhất của $ u(x_i) $ có bậc $ \lambda + d(i) $. Ta chứng minh rằng tồn tại một đồng cấu $ u_\lambda : M \to N $ sao cho $ u_\lambda(x_i) = z_{i,\lambda} $ với mọi $ i $. Chỉ cần chứng minh rằng nếu $ \sum_i a_ix_i = 0 $ với $ a_i \in A $ đối với $ 1 \leq i \leq n $, thì $ \sum_i a_iz_{i,\lambda} = 0 $ với mọi $ \lambda \in \Delta $ ($ \S 1 $, no. 7, *Nhận xét*). Có thể giả sử rằng mỗi $ a_i $ là thuần nhất có bậc $ d'(i) $ sao cho $ d(i) + d'(i) = \mu $ với mọi $ i $ (no. 3, *Nhận xét* 1); khi đó $ \sum_i a_iu(x_i) = 0 $; lấy thành phần thuần nhất có bậc $ \lambda + \mu $ ở vế trái, ta thu được $ \sum_i a_iz_{i,\lambda} = 0 $, do đó sự tồn tại của đồng cấu $ u_\lambda $; rõ ràng hơn nữa $ u_\lambda $ là *phân bậc* có bậc $ \lambda $. Cuối cùng, $ u_\lambda = 0 $ ngoại trừ một số hữu hạn các giá trị của $ \lambda $, và $ u = \sum_\lambda u_\lambda $ theo định nghĩa, điều này chứng minh mệnh đề của chúng ta.

Đặc biệt, $ \mathrm{Homgr}_A(A_s, M) = \mathrm{Hom}_A(A_s, M) $ với mọi $ A $-môđun trái $ M $ phân bậc; hơn nữa $ \mathrm{Hom}_A(A_s, M) $ có cấu trúc *A-môđun trái phân bậc* (chứ không chỉ là cấu trúc $ C $-môđun phân bậc), và ngay lập tức thấy rằng với cấu trúc này, ánh xạ chính tắc từ $ M $ vào $ \mathrm{Hom}_A(A_s, M) $ ($ \S 1 $, no. 14, *Nhận xét* 2) là một *đẳng cấu A-môđun phân bậc*.

Tương tự, $ \mathrm{Homgr}_A(M, A_s) $ có cấu trúc *A-môđun phải phân bậc* (chứ không chỉ là cấu trúc $ C $-môđun phân bậc); nó được gọi là *đối ngẫu phân bậc* của $ A $-môđun $ M $ phân bậc và được ký hiệu là $ M^{*\mathrm{gr}} $, hoặc đơn giản là $ M^* $ khi không gây nhầm lẫn. Nếu $ u : M \to N $ là một đồng cấu phân bậc có bậc $ \delta $, thì theo điều trên, hạn chế của $ {}^t u = \mathrm{Hom}(u, 1_{A_s}) $ lên $ N^{*\mathrm{gr}} $ là một đồng cấu phân bậc từ đối ngẫu phân bậc $ N^{*\mathrm{gr}} $ vào đối ngẫu phân bậc $ M^{*\mathrm{gr}} $, có bậc $ \delta $, được gọi là *chuyển vị phân bậc* của $ u $.

Đôi khi ta xét trên đối ngẫu phân bậc $ M^{*\mathrm{gr}} $ phép phân bậc dẫn xuất từ phép trên bằng cách dùng đẳng cấu $ \lambda \mapsto -\lambda $ của $ \Delta $ (no. 1, *Ví dụ* 2), sao cho các phần tử thuần nhất có bậc $ \lambda $ trong $ M^{*\mathrm{gr}} $ là các dạng tuyến tính phân bậc *có bậc* $ -\lambda $ trên $ M $ (khi $ A $ có phép phân bậc tầm thường, đó là các dạng tuyến tính không trên các $ M_\mu $ có chỉ số $ \mu \neq \lambda $). Khi đó, nếu $ u : M \to N $ là một đồng cấu phân bậc có bậc $ \delta $, $ u' $ trở thành một đồng cấu phân bậc có bậc $ -\delta $.

Giả sử $ A $ là *giao hoán* và phân bậc kiểu $ \Delta $ và $ M, N, P, Q $ là bốn $ A $-môđun *phân bậc* kiểu $ \Delta $. Khi đó có các *đồng cấu phân bậc chính tắc có bậc* 0

(3) $$
\operatorname{Homgr}_A(M, \operatorname{Homgr}_A(N, P)) \to \operatorname{Homgr}_A(M \otimes_A N, P)
$$
(4) $$
\operatorname{Homgr}_A(M, N) \otimes_A P \to \operatorname{Homgr}_A(M, N \otimes_A P)
$$
(5) $$
\operatorname{Homgr}_A(M, P) \otimes_A \operatorname{Homgr}_A(N, Q) \to \operatorname{Homgr}_A(M \otimes_A N, P \otimes_A Q)
$$
(các tích tenxơ được trang bị các phép phân bậc được định nghĩa trong no. 5) nhận được bằng cách hạn chế các đồng cấu chính tắc được định nghĩa trong § 4, các no. 1, 2 và 4; thật vậy, nếu $ u : M \to \operatorname{Homgr}_A(N, P) $ là một đồng cấu phân bậc có bậc $ \delta $, thì với mọi $ x \in M_\lambda $, $ u(x) $ là một đồng cấu phân bậc $ N \to P $ có bậc $ \delta + \lambda $ và do đó, với $ y \in N_\mu $, $ u(x)(y) \in P_{\delta + \lambda + \mu} $; nếu $ v : M \otimes_A N \to P $ tương ứng một cách chính tắc với $ u $, thì thấy rằng $ v $ là một đồng cấu phân bậc có bậc $ \delta $, do đó có mệnh đề của chúng ta về (3); hơn nữa thấy rằng đồng cấu này là *song ánh*. Lập luận tương tự áp dụng cho (4) và (5).

Nếu đặc biệt $ P = Q = A $ trong (5), thì có một đồng cấu *phân bậc* chính tắc có bậc 0

(6) $$
M^{*\mathrm{gr}} \otimes_A N^{*\mathrm{gr}} \to (M \otimes_A N)^{*\mathrm{gr}}.
$$

### Bài tập {#alg-ii-s11-exercises}

Xem [các bài tập cho § 11](exercises/s11/).
