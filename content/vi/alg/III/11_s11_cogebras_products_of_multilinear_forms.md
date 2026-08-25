---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 11
section_title: Cogebras, products of multilinear forms, inner products and duality
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0598-0635, 0671-0678
extraction: ocr
subsections:
    - "no": 1
      title: COGEBRAS
      page: 0
      pdf_page: 598
    - "no": 2
      title: COASSOCIATIVITY, COCOMMUTATIVITY, COUNIT
      page: 0
      pdf_page: 602
    - "no": 3
      title: PROPERTIES OF GRADED COGEBRAS OF TYPE N
      page: 0
      pdf_page: 608
    - "no": 4
      title: BIGEBRAS AND SKEW-BIGEBRAS
      page: 0
      pdf_page: 609
    - "no": 5
      title: THE GRADED DUALS $ T(M)^{*gr} $, $ S(M)^{*gr} $ AND $ \bigwedge(M)^{*gr} $
      page: 0
      pdf_page: 611
    - "no": 6
      title: 'INNER PRODUCTS: CASE OF ALGEBRAS'
      page: 0
      pdf_page: 618
    - "no": 7
      title: 'INNER PRODUCTS: CASE OF COGEbras'
      page: 0
      pdf_page: 621
    - "no": 8
      title: 'INNER PRODUCTS: CASE OF BIGEBRAS'
      page: 0
      pdf_page: 624
    - "no": 9
      title: INNER PRODUCTS BETWEEN $ T(M) $ AND $ T(M^*) $, $ S(M) $ AND $ S(M^*) $, $ \Lambda(M) $ AND $ \Lambda(M^*) $
      page: 0
      pdf_page: 627
    - "no": 10
      title: EXPLICIT FORM OF INNER PRODUCTS IN THE CASE OF A FINITELY GENERATED FREE MODULE
      page: 0
      pdf_page: 629
    - "no": 11
      title: ISOMORPHISMS BETWEEN $ \wedge^p(M) $ AND $ \wedge^{n-p}(M^*) $ FOR AN $ n $-DIMENSIONAL FREE MODULE M
      page: 0
      pdf_page: 631
    - "no": 12
      title: APPLICATION TO THE SUBSPACE ASSOCIATED WITH A p-VECTOR
      page: 0
      pdf_page: 632
    - "no": 13
      title: PURE $ p $-VECTORS. GRASSMANNIANS
      page: 0
      pdf_page: 633
statements: 40
exercises: 25
content_sha256: 6a45d9d4fe4ebaea1dcbee56ca30d972413aa7a965615cf3919ba42b205d5dc7
translated_from: content/en/alg/III/11_s11_cogebras_products_of_multilinear_forms.md
source_content_sha256: 650a0f34590a41cae39ed6dc5afd5bff2ee171748aeec25cd7446a1040de2d67
translation_model: gpt-5-6-mini
translation_run: translate-vi-3a454801
glossary_version: 34
glossary_terms_sha256: 22fad35f85e17929f1e3aa8ae64d4973daccea4d4a38805a8f01fb1a794d8c0c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. ĐỐI ĐẠI SỐ, TÍCH CỦA CÁC DẠNG ĐA TUYẾN TÍNH, TÍCH NỘI VÀ ĐỐI NGẪU

Trong đoạn này, A là một vành giao hoán với phân bậc tầm thường. Đối với một A-môđun phân bậc M kiểu N, M^{gr} sẽ kí hiệu A-môđun phân bậc kiểu N, mà các phần tử thuần nhất có bậc n là các dạng A-tuyến tính triệt tiêu trên M_k với mọi k ≠ n.

### 1. ĐỐI ĐẠI SỐ

#### Định nghĩa 1 {#alg-iii-s11-def-1 .statement}

Một đối đại số trên A (hoặc A-đối đại số, hoặc đơn giản là đối đại số nếu không thể có sự nhầm lẫn) là một tập hợp E với một cấu trúc được xác định bằng cách cho:
(1) một cấu trúc A-môđun trên E;
(2) một ánh xạ A-tuyến tính c: E → E ⊗_A E được gọi là đồng tích của E.

#### Định nghĩa 2 {#alg-iii-s11-def-2 .statement}

Cho hai đối đại số E, E', mà các đồng tích của chúng lần lượt được kí hiệu bởi c và c', một cấu xạ từ E vào E' là một ánh xạ A-tuyến tính u: E → E' sao cho
(1) $ (u \otimes u) \circ c = c' \circ u, $ nói cách khác, nó làm giao hoán biểu đồ các ánh xạ A-tuyến tính

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow c & & \downarrow c' \\
E \otimes_A E & \xrightarrow{u \otimes u} & E' \otimes_A E'
\end{array}
$$

Ta kiểm tra ngay lập tức rằng ánh xạ đồng nhất là một cấu xạ, rằng hợp thành của hai cấu xạ là một cấu xạ và rằng mọi cấu xạ song ánh là một đẳng cấu.

#### Ví dụ {#alg-iii-s11-n1-exa-1 .statement}

(1) Đẳng cấu chính tắc $ A \to A \otimes_A A $ (II, § 3, no. 5) xác định một cấu trúc A-đối đại số trên A.

(2) Cho E là một đối đại số, $ c $ là đồng tích của nó và $ \sigma $ là tự đẳng cấu chính tắc của A-môđun $ E \otimes_A E $ sao cho $ \sigma(x \otimes y) = y \otimes x $ với $ x \in E, y \in E $; ánh xạ A-tuyến tính $ \sigma \circ c $ xác định một cấu trúc đối đại số mới trên E. Với cấu trúc này E được gọi là đối đại số *đối* với đối đại số đã cho E.

(3) Cho B là một *đại số* trên A và cho $ m : B \otimes_A B \to B $ là ánh xạ A-tuyến tính xác định phép nhân trên B (\S 1, no. 3). Chuyển vị $ ^t m $ khi đó là một ánh xạ A-tuyến tính từ đối ngẫu $ B^* $ của A-môđun B vào đối ngẫu $ (B \otimes_A B)^* $ của A-môđun $ B \otimes_A B $. Nếu B cũng là một A-môđun *xạ ảnh sinh hữu hạn*, ánh xạ chính tắc $ \mu : B^* \otimes_A B^* \to (B \otimes_A B)^* $ là một đẳng cấu A-môđun (II, § 4, no. 4); ánh xạ $ c = \mu^{-1} \circ ^t m $ khi đó là một đồng tích xác định một cấu trúc *đối đại số* trên đối ngẫu $ B^* $ của A-môđun B.

(4) Cho X là một tập hợp, $ A^{(X)} $ là A-môđun của các tổ hợp tuyến tính hình thức của các phần tử của X với các hệ số trong A (II, § 1, no. 11) và $ (e_x)_{x \in X} $ là cơ sở chính tắc của $ A^{(X)} $. Một ánh xạ A-tuyến tính $ c : A^{(X)} \to A^{(X)} \otimes_A A^{(X)} $ được xác định bởi điều kiện $ c(e_x) = e_x \otimes e_x $ và do đó thu được một cấu trúc đối đại số chính tắc trên $ A^{(X)} $.

(5) Cho M là một A-môđun và $ T(M) $ là đại số tenxơ của M (\S 5, no. 1); theo II, § 3, no. 9 tồn tại duy nhất một ánh xạ A-tuyến tính $ c $ từ A-môđun $ T(M) $ vào A-môđun $ T(M) \otimes_A T(M) $ sao cho, với mọi $ n \geq 0 $,

$$
c(x_1 x_2 \ldots x_n) = \sum_{0 \leq p \leq n} (x_1 x_2 \ldots x_p) \otimes (x_{p+1} \ldots x_n)
$$

với mọi $ x_i \in M $ ($ x_1 x_2 \ldots x_n $ kí hiệu tích trong đại số $ T(M) $). Như vậy $ T(M) $ được trang bị một cấu trúc *đối đại số*.

(6) Cho M là một A-môđun và $ S(M) $ là đại số đối xứng của M (\S 6, no. 1); ánh xạ đường chéo $ \Delta : x \mapsto (x, x) $ từ M vào $ M \times M $ là một ánh xạ A-tuyến tính tương ứng với nó do đó có một đồng cấu $ S(\Delta) $ từ A-đại số $ S(M) $ vào A-đại số $ S(M \times M) $ (\S 6, no. 2, Mệnh đề 3). Mặt khác, trong § 6, no. 6 ta đã xác định một đẳng cấu đại số phân bậc chính tắc $ h : S(M \times M) \to S(M) \otimes_A S(M) $; bằng hợp thành ta do đó thu được một đồng cấu *đại số trên A*

$$
c = h \circ S(\Delta) : S(M) \to S(M) \otimes_A S(M),
$$

do đó xác định trên $ S(M) $ một cấu trúc *đối đại số*. Với mọi $ x \in M $, theo định nghĩa $ S(\Delta)(x) = (x, x) $ và định nghĩa của $ h $ cho trong § 6, no. 6 cho thấy rằng

$$
h((x, x)) = x \otimes 1 + 1 \otimes x.
$$

Suy ra rằng $ c $ là đồng cấu đại số duy nhất sao cho, với mọi $ x \in M $,

(4)
$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

Vì $ c $ là một đồng cấu đại số, suy ra rằng, với mọi dãy $ (x_i)_{1 \leq i \leq n} $ gồm $ n $ phần tử của $ M $,

(5)
$$
c(x_1 x_2 \ldots x_n) = \prod_{i=1}^n (x_i \otimes 1 + 1 \otimes x_i)
$$
$$
= \sum (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}})
$$

tổng ở vế phải của (5) được lấy trên mọi cặp có thứ tự của các dãy tăng ngặt (trong một số trường hợp là rỗng)

$$
i_1 < i_2 < \cdots < i_p, \quad j_1 < j_2 < \cdots < j_{n-p}
$$

của các phần tử của $ \{1, n\} $, có các tập hợp phần tử của chúng bù nhau. Phần tử $ c(x_1 x_2 \ldots x_n) $ là một phần tử có *bậc toàn phần* $ n $ trong $ S(M) \otimes_A S(M) $ và thành phần của nó có song bậc $ (p, n-p) $ là

(6)
$$
\sum_{\sigma} (x_{\sigma(1)} \ldots x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \ldots x_{\sigma(n)})
$$

trong đó tổng được lấy theo mọi hoán vị $ \sigma \in S_n $ tăng trong mỗi khoảng $ \{1, p\} $ và $ \{p+1, n\} $.

(7) Cho $ M $ là một $ A $-môđun và xét đại số ngoài $ \Lambda(M) $ như với $ S(M) $ trong *Ví dụ* 6; ánh xạ đường chéo $ \Delta : M \to M \times M $ lần này xác định một đồng cấu $ \Lambda(\Delta) $ của $ A $-đại số $ \Lambda(M) $ vào $ A $-đại số $ \Lambda(M \times M) $ (\S 7, no. 2, Mệnh đề 2); mặt khác có một đẳng cấu đại số phân bậc chính tắc

$$
h : \Lambda(M \times M) \to \Lambda(M)^g \otimes_A \Lambda(M)
$$

(\S 7, no. 7, Mệnh đề 10), do đó bằng hợp thành có một đồng cấu *đại số* $ c = h \circ \Lambda(\Delta) : \Lambda(M) \to \Lambda(M)^g \otimes_A \Lambda(M) $, có thể được xem như một đồng cấu $ A $-môđun $ \Lambda(M) \to \Lambda(M) \otimes_A \Lambda(M) $ và vì thế xác định trên $ \Lambda(M) $ một cấu trúc *đối đại số*. Có thể chứng minh như trong *Ví dụ* 6 rằng $ c $ là đồng cấu đại số duy nhất sao cho, với mọi $ x \in M $,

(7)
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$

do đó, với mọi dãy $(x_i)_{1 \leq i \leq n}$ các phần tử của $M$,
$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = (x_1 \otimes 1 + 1 \otimes x_1) \wedge \ldots \wedge (x_n \otimes 1 + 1 \otimes x_n)
$$
trong đó tích ở vế phải được lấy trong đại số
$$
\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M);
$$
để tính tích này, xét, với mỗi cặp có thứ tự của các dãy tăng ngặt
$i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$ của các phần tử của $[1, n]$, có các tập hợp phần tử của chúng bù nhau, tích $y_1 y_2 \ldots y_n$, trong đó $y_{i_h} = x_{i_h} \otimes 1$ ($1 \leq h \leq p$) và $y_{j_k} = 1 \otimes x_{j_k}$ ($1 \leq k \leq n - p$) và tổng được lấy theo tất cả các tích này. Vì đại số phân bậc $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ là phản giao hoán và các phần tử $x_i \otimes 1$ và $1 \otimes x_i$ có bậc toàn phần 1, theo § 4, no. 6, Bổ đề 3 và Bổ đề 1,
$$(8)\quad c(x_1 \wedge x_2 \wedge \cdots \wedge x_n)$$
$$
= \sum (-1)^v (x_{i_1} \wedge \cdots \wedge x_{i_p}) \otimes (x_{j_1} \wedge \cdots \wedge x_{j_{n-p}})
$$
$v$ là số các cặp có thứ tự $(h, k)$ sao cho $j_k < i_h$ và tổng được lấy theo cùng một tập hợp như trong (5). Phần tử $c(x_1 \wedge \cdots \wedge x_n)$ có *bậc toàn phần* $n$ trong $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ và thành phần thuần nhất có song bậc $(p, n - p)$ của nó bằng
$$(9)\quad \sum_{\sigma} \varepsilon_\sigma (x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \wedge \cdots \wedge x_{\sigma(n)})
$$
tổng được lấy theo các hoán vị $\sigma \in S_n$ tăng trong mỗi khoảng $[1, p]$ và $[p + 1, n]$.

Sau này khi ta nói về $A^{(x)}, T(M), S(M)$ hoặc $\bigwedge(M)$ như các *đối đại số*, ta sẽ hiểu, trừ khi có nói khác, là với các cấu trúc đối đại số được xác định trong các *Ví dụ* 4, 5, 6 và 7 tương ứng.

(8) Cho $E, F$ là hai đối đại số $A$ và $c, c'$ là các đồng tích tương ứng của chúng. Gọi $\tau : (E \otimes_A E) \otimes_A (F \otimes_A F) \to (E \otimes_A F) \otimes_A (E \otimes_A F)$ là đẳng cấu tính kết hợp sao cho $\tau((x \otimes x') \otimes (y \otimes y')) = (x \otimes y) \otimes (x' \otimes y')$ với $x, x'$ thuộc $E$ và $y, y'$ thuộc $F$. Khi đó ánh xạ tuyến tính hợp thành
$$
E \otimes_A F \xrightarrow{c \otimes c'} (E \otimes_A E) \otimes_A (F \otimes_A F) \xrightarrow{\tau} (E \otimes_A F) \otimes_A (E \otimes_A F)
$$
xác định một cấu trúc đối đại số trên $A$-môđun $E \otimes_A F$, gọi là *tích tenxơ* của các đối đại số $E$ và $F$.

Cho $E$ là một đối đại số và $\Delta$ là một monoid giao hoán. Một phép phân bậc $(E_\lambda)_{\lambda \in \Delta}$ trên $A$-môđun $E$ được gọi là *tương thích với đồng tích* $c$ của $E$ nếu $c$ là một đồng cấu phân bậc bậc $O$ của $A$-môđun phân bậc $E$ vào $A$-môđun phân bậc (kiểu $\Delta$) $E \otimes_A E$, nói cách khác (II, § 11, no. 5), nếu
$$(10)\quad c(E_\lambda) \subset \sum_{\mu + \nu = \lambda} E_\mu \otimes_A E_\nu.$$

Trong phần tiếp theo, ta sẽ thường chỉ xét đến các phép phân bậc kiểu $ \mathbf{N} $ tương thích với đồng tích; một đối đại số với phép phân bậc như vậy cũng sẽ được gọi là một *đối đại số phân bậc*. Nếu F là một đối đại số phân bậc khác, một *cấu xạ đối đại số phân bậc* $\phi : E \to F$ theo định nghĩa là một cấu xạ đối đại số (Định nghĩa 2), đồng thời là một *đồng cấu phân bậc bậc* 0 của các $A$-môđun phân bậc.

#### Ví dụ {#alg-iii-s11-n1-exa-2 .statement}

(9) Ngay lập tức thấy rằng các đối đại số $ T(M) $, $ S(M) $ và $ \Lambda(M) $ được định nghĩa ở trên là các đối đại số phân bậc.

### 2. TÍNH KẾT HỢP, TÍNH GIAO HOÁN VÀ ĐỒNG ĐƠN VỊ

Cho E là một đối đại số, $ c $ là đồng tích của nó, N, $ N' $, $ N'' $ là ba $A$-môđun và $ m $ là một ánh xạ song tuyến tính của $ N \times N' $ vào $ N'' $. Gọi $ \tilde{m} : N \otimes_A N' \to N'' $ là ánh xạ $A$-tuyến tính tương ứng với $ m $. Nếu $ u : E \to N $, $ v : E \to N' $ là hai ánh xạ $A$-tuyến tính, ta suy ra một ánh xạ $A$-tuyến tính $ u \otimes v : E \otimes_A E \to N \otimes_A N' $ và một ánh xạ $A$-tuyến tính hợp thành từ E vào $ N'' $:

$$
m(u, v) : E \xrightarrow{c} E \otimes_A E \xrightarrow{u \otimes v} N \otimes_A N' \xrightarrow{\tilde{m}} N''.
$$

Rõ ràng, như vậy ta đã xác định một ánh xạ $A$-song tuyến tính $ (u, v) \mapsto m(u, v) $ từ $ \mathrm{Hom}_A(E, N) \times \mathrm{Hom}_A(E, N') $ vào $ \mathrm{Hom}_A(E, N'') $.

Khi E là một đối đại số phân bậc, N, $ N' $, $ N'' $ là các A-môđun phân bậc cùng kiểu và $ \tilde{m} $ là một đồng cấu phân bậc bậc k từ $ N \otimes_A N' $ vào $ N'' $, thì, nếu $ u $ (tương ứng $ v $) là một đồng cấu phân bậc bậc $ p $ (tương ứng $ q $), $ m(u, v) $ là một đồng cấu phân bậc bậc $ p + q + k $.

#### Ví dụ {#alg-iii-s11-n2-exa-1 .statement}

(1) Lấy E là đối đại số phân bậc $ T(M) $ (no. 1) và giả sử rằng N, $ N' $, $ N'' $ có phân bậc tầm thường. Khi đó một đồng cấu phân bậc bậc $ -p $ từ $ T(M) $ vào N (tương ứng $ N' $, $ N'' $) tương ứng với một ánh xạ đa tuyến tính từ $ M^p $ vào N (tương ứng $ N' $, $ N'' $). Cho một ánh xạ đa tuyến tính $ u : M^p \to N $ và một ánh xạ đa tuyến tính $ v : M^q \to N' $, phương pháp trên cho phép ta suy ra một ánh xạ đa tuyến tính $ m(u, v) : M^{p+q} \to N'' $ được gọi là *tích* (đối với $ m $) của $ u $ và $ v $. Các công thức (3) (no. 1) và (11) cho thấy rằng, với $ x_1, \ldots, x_{p+q} $ trong M,

$$
(m(u, v))(x_1, \ldots, x_{p+q}) = m(u(x_1, \ldots, x_p), v(x_{p+1}, \ldots, x_{p+q})).
$$

(2) Lấy E là đối đại số phân bậc $ S(M) $ (no. 1), vẫn giữ các giả thiết trên đối với N, $ N' $, $ N'' $. Khi đó một đồng cấu phân bậc bậc $ -p $ từ $ S(M) $ vào N tương ứng với một *ánh xạ đa tuyến tính đối xứng* từ $ M^p $ vào N (\S 6, no. 3). Từ một ánh xạ đa tuyến tính đối xứng $ u : M^p \to N $ và một ánh xạ đa tuyến tính đối xứng $ v : M^q \to N' $, ta suy ra một ánh xạ đa tuyến tính đối xứng $ m(u, v) : M^{p+q} \to N'' $, cũng được ký hiệu (để tránh nhầm lẫn) bởi $ u._m v $ (hoặc thậm chí $ u.v $) và được gọi là *tích đối xứng* (đối với $ m $) của $ u $ và $ v $. Các công thức (6) (no. 1) và (11) cho thấy rằng, với $ x_1, \ldots, x_{p+q} $ trong M,

$$(u \cdot_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

tổng được lấy theo các hoán vị $ \sigma \in \mathfrak{S}_{p+q} $ tăng trên mỗi khoảng $[1, p]$ và $[p+1, p+q]$.

(3) Lấy E là đối đại số phân bậc $ \bigwedge(M) $ (no. 1). Khi đó tương tự, từ một ánh xạ đa tuyến tính phản xứng $ u : M^p \to N $ và một ánh xạ đa tuyến tính phản xứng $ v : M^q \to N' $, ta suy ra một ánh xạ đa tuyến tính phản xứng $ m(u, v) : M^{p+q} \to N'' $, cũng được ký hiệu bởi $ u \wedge_m v $ hoặc $ u \wedge v $ và được gọi là *tích phản xứng* (đối với $ m $) của $ u $ và $ v $. Các công thức (9) (no. 1) và (11) cho thấy trong trường hợp này rằng, với $ x_1, \ldots, x_{p+q} $ trong $ M $,

$$(u \wedge_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma \varepsilon_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

tổng lại vẫn được lấy trên các phép hoán vị $ \sigma \in \mathfrak{S}_{p+q} $ tăng trên mỗi một trong các khoảng $[1, p]$ và $[p+1, p+q]$.

Ta quay lại trường hợp trong đó E là một đối đại số phân bậc tùy ý (kiểu N) và giả sử rằng ba môđun N, N', N'' đều bằng môđun A cơ sở của một *đại số A phân bậc* B kiểu $ \mathbf{Z} $, ánh xạ $ m $ là phép nhân trong B, sao cho $ \tilde{m} : B \otimes_A B \to B $ là một ánh xạ A-tuyến tính phân bậc bậc 0. Khi đó thu được một cấu trúc *đại số A phân bậc* trên A-môđun phân bậc $ \mathrm{Homgr}_A(E, B) = C $.

Đặc biệt, giả sử rằng $ B = A $ (với phép phân bậc tầm thường), sao cho $ \mathrm{Homgr}_A(E, A) $ là *đối ngẫu phân bậc* $ E^{*gr} $, khi đó nó có một cấu trúc đại số A phân bậc.

Cho F là một đối đại số phân bậc khác, $ c' $ là đồng tích của nó và $ \phi : E \to F $ là một cấu xạ đối đại số phân bậc (no. 1); khi đó cấu xạ phân bậc chính tắc

$$\tilde{\phi} = \mathrm{Hom}(\phi, 1_B) : \mathrm{Homgr}_A(F, B) \to \mathrm{Homgr}_A(E, B)$$

là một *đồng cấu đại số phân bậc*. Với $ u, v $ trong $ \mathrm{Homgr}_A(F, B) $ và $ x \in E $,

$$(\tilde{\phi}(uv))(x) = (uv)(\phi(x)) = m((u \otimes v)(c'(\phi(x)))).$$

Nhưng theo giả thiết $ c'(\phi(x)) = (\phi \otimes \phi)(c(x)) $, do đó

$$(u \otimes v)(c'((x))) = (\tilde{\phi}(u) \otimes \tilde{\phi}(v))(c(x))$$

và vì thế $ \tilde{\phi}(uv) = \tilde{\phi}(u)\tilde{\phi}(v) $, điều này chứng minh mệnh đề của chúng ta.

Đặc biệt, chuyển vị phân bậc $ ^t\phi : F^{*gr} \to E^{*gr} $ là một đồng cấu đại số phân bậc.

#### Nhận xét {#alg-iii-s11-n2-rem-1 .statement}

Giả sử rằng các $ E_p $ là các A-môđun xạ ảnh sinh hữu hạn, sao cho các A-môđun phân bậc $ (E \otimes_A E)^{*gr} $ và $ E^{*gr} \otimes_A E^{*gr} $ có thể được đồng nhất một cách chính tắc (II, § 4, no. 4, Hệ quả 1 đối với Mệnh đề 4). Nếu thêm vào đó các A-môđun $ A \otimes_A A $ và $ A $ khi đó cũng được đồng nhất một cách chính tắc (II, § 3, no. 4), thì ánh xạ tuyến tính $ E^{*gr} \otimes_A E^{*gr} \to E^{*gr} $ xác định phép nhân trong $ E^{*gr} $ có thể được gọi là chuyển vị phân bậc của đồng tích $ c $.

#### Mệnh đề 1 {#alg-iii-s11-prop-1 .statement}

*Cho $ E $ là một đối đại số trên $ A $. Để với mọi đại số A kết hợp $ B $, đại số A $ \mathrm{Hom}_A(E, B) $ là kết hợp, điều kiện cần và đủ là đồng tích $ c : E \to E \otimes_A E $ phải sao cho biểu đồ*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
\downarrow c & & \downarrow l_E \otimes c \\
E \otimes_A E & \xrightarrow{c \otimes l_E} & E \otimes_A E \otimes_A E
\end{array}
$$

*là giao hoán.*

Cho $ B $ là một đại số A kết hợp và $ u, v, w $ là ba phần tử của $ C = \mathrm{Hom}_A(E, B) $. Ký hiệu $ m_3 $ là ánh xạ A-tuyến tính $ B \otimes_A B \otimes_A B \to B $ biến $ b \otimes b' \otimes b'' $ thành $ bb'b'' $. Theo định nghĩa của tích trên đại số $ C $, $ (uv)w $ là ánh xạ hợp thành

$$
E \xrightarrow{c} E \otimes E \xrightarrow{c \otimes 1_E} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B
$$

trong khi $ u(vw) $ là ánh xạ hợp thành

$$
E \xrightarrow{c} E \otimes E \xrightarrow{l_E \otimes c} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B.
$$

Suy ra rằng nếu biểu đồ (12) giao hoán, đại số $ \mathrm{Hom}_A(E, B) $ là kết hợp với mọi đại số kết hợp $ A $-đại số $ B $. Để chứng minh mệnh đề đảo lại, chỉ cần chỉ ra rằng tồn tại một đại số kết hợp $ A $-đại số $ B $ và ba ánh xạ $ A $-tuyến tính $ u, v, w $ từ $ E $ vào $ B $ sao cho ánh xạ $ m_3 \circ (u \otimes v \otimes w) $ từ $ E \otimes E \otimes E $ vào $ B $ là đơn ánh. Lấy $ B $ là $ A $-đại số $ \mathcal{T}(E) $ và $ u, v, w $ là ánh xạ chính tắc từ $ E $ vào $ \mathcal{T}(E) $. Khi đó ánh xạ $ m_3 \circ (u \otimes v \otimes w) $ là ánh xạ chính tắc $ E \otimes E \otimes E = \mathcal{T}^3(E) \to \mathcal{T}(E) $, là đơn ánh.

Khi đối đại số $ E $ thỏa mãn điều kiện của Mệnh đề 1, nó được gọi là đối kết hợp.

#### Ví dụ {#alg-iii-s11-n2-exa-2 .statement}

(4) Ngay lập tức kiểm tra được rằng đối đại số $ A $ (no. 1, Ví dụ (1)), đối đại số $ A^{(X)} $ (no. 1, Ví dụ 4) và đối đại số $ \mathcal{T}(M) $ (no. 1, Ví dụ 5) đều là đối kết hợp. Nếu $ B $ là một $ A $-đại số kết hợp đồng thời là một $ A $-môđun xạ ảnh sinh hữu hạn, thì đối đại số $ B^* $ (no. 1, Ví dụ 3) là đối kết hợp: khi đó tính giao hoán của biểu đồ (12) suy ra bằng phép chuyển vị từ tính kết hợp của $ B $ (\S 1, no. 3). Ngược lại, cùng một lập luận và phép đồng nhất chính tắc của A-môđun B với đối ngẫu kép của nó (II, § 2, no. 7, Hệ quả 4 của Mệnh đề 13) cho thấy rằng nếu các đối đại số B* là đối kết hợp, thì đại số B là kết hợp. Cuối cùng, các đối đại số S(M) và $ \Lambda(M) $ (no. 1, Các Ví dụ 6 và 7) là đối kết hợp; điều này suy ra từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{\Delta} & M \times M \\
\downarrow & & \downarrow 1_M \times \Delta \\
M \times M & \xrightarrow{\Delta \times 1_M} & M \times M \times M
\end{array}
$$

các tính chất hàm tử của S(M) (\S 6, no. 2) và $ \Lambda(M) $ (\S 7, no. 2), cho các biểu đồ giao hoán tương ứng

$$
\left\{
\begin{array}{ccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \times M) \\
\downarrow S(\Delta) & & \downarrow S(\Delta_M \times 1) \\
S(M \times M) & \xrightarrow{S(\Delta \times 1_M)} & S(M \times M \times M)
\end{array}
\right.
$$
$$
\left\{
\begin{array}{ccc}
\Lambda(M) & \xrightarrow{\Lambda(\Delta)} & \Lambda(M \times M) \\
\downarrow \Lambda(\Delta) & & \downarrow \Lambda(1_M \times \Delta) \\
\Lambda(M \times M) & \xrightarrow{\Lambda(\Delta \times 1_M)} & \Lambda(M \times M \times M)
\end{array}
\right.
$$

và sự tồn tại cũng như tính hàm tử của các đẳng cấu chính tắc đối với các đại số đối xứng và ngoại của một tổng trực tiếp (\S 6, no. 6 và \S 7, no. 7).

#### Mệnh đề 2 {#alg-iii-s11-prop-2 .statement}

*Cho E là một đối đại số trên A. Để, với mọi A-đại số giao hoán B, A-đại số $ \mathrm{Hom}_A(E, B) $ là giao hoán, điều kiện cần và đủ là đối tích $ c : E \to E \otimes_A E $ phải sao cho biểu đồ*

$$
\begin{array}{ccc}
E & & \\
 & \swarrow_c & \searrow_c \\
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E
\end{array}
$$

*(trong đó $ \sigma $ là đồng cấu đối xứng sao cho $ \sigma(x \otimes y) = y \otimes x $) là *giao hoán* (nói cách khác, chỉ cần các đối đại số E *đồng nhất với đối của nó* (no. 1, Ví dụ 2).*

Cho B là một A-đại số giao hoán và $ u, v $ là hai phần tử của $ C = \mathrm{Hom}_A(E, B) $.

Theo định nghĩa của tích trong C, $ uv $ và $ vu $ lần lượt bằng các ánh xạ hợp thành

$$
E \xrightarrow{c} E \otimes E \xrightarrow{u \otimes v} B \otimes B \xrightarrow{m} B
$$

và

$$
E \xrightarrow{c} E \otimes E \xrightarrow{v \otimes u} B \otimes B \xrightarrow{m} B.
$$

Suy ra rằng nếu biểu đồ (15) là giao hoán thì đại số $ \mathrm{Hom}_A(E, B) $ là giao hoán đối với mọi đại số giao hoán trên A B. Để thiết lập mệnh đề đảo lại, chỉ cần chỉ ra rằng tồn tại một đại số giao hoán trên A B và hai ánh xạ A-tuyến tính $ u, v $ của E vào B sao cho $ m \circ (u \otimes v): E \otimes E \to B $ là đơn ánh. Lấy B là đại số $ S(E \oplus E) $ và lấy $ u $ (tương ứng $ v $) là hợp thành của ánh xạ chính tắc $ E \oplus E \to S(E \oplus E) $ và ánh xạ $ x \mapsto (x, 0) $ (tương ứng $ x \mapsto (0, x) $) của E vào $ E \oplus E $. Nếu $ h: S(E) \otimes S(E) \to S(E \otimes E) $ là đẳng cấu chính tắc (\S 6, no. 6, Mệnh đề 9) và $ \lambda: E \to S(E) $ là ánh xạ chính tắc, thì $ h^{-1} \circ m \circ (u \otimes v) = \lambda \otimes \lambda $. Khi đó $ \lambda \otimes \lambda $ là đơn ánh, vì $ \lambda(E) $ là một nhân tử trực tiếp của $ S(E) $ (II, \S 3, no. 7, Hệ quả 5 đối với Mệnh đề 7).

Khi đối đại số E thỏa mãn điều kiện của Mệnh đề 2, nó được gọi là đối giao hoán.

#### Ví dụ {#alg-iii-s11-n2-exa-3 .statement}

(5) Hiển nhiên rằng đối đại số A (no. 1, Ví dụ 1) và đối đại số $ A^{(X)} $ (II, \S 11, no. 1, Ví dụ 4) là đối giao hoán. Từ công thức (5) của no. 1 suy ra rằng đối đại số $ S(M) $ là đối giao hoán. Cuối cùng, đối với một đại số trên A B sao cho A-môđun B là xạ ảnh và sinh hữu hạn, để đối đại số $ B^* $ (no. 1, Ví dụ 3) có tính chất là đối giao hoán, điều kiện cần và đủ là B giao hoán; vì (sử dụng sự đồng nhất chính tắc của A-môđun B với đối ngẫu kép của nó (II, \S 2, no. 7)), điều này suy ra từ sự kiện rằng tính giao hoán của biểu đồ (14) tương đương qua phép chuyển vị với tính giao hoán của biểu đồ biểu thị tính giao hoán của B (\S 1, no. 3).

#### Mệnh đề 3 {#alg-iii-s11-prop-3 .statement}

*Cho E là một đối đại số trên A. Để, với mọi đại số trên A có đơn vị B, đại số trên A $ \mathrm{Hom}_A(E, B) $ có đơn vị, điều kiện cần và đủ là tồn tại một dạng tuyến tính $ \gamma $ trên E làm cho các biểu đồ sau là giao hoán*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow \gamma \otimes 1_E \\
& & A \otimes_A E
\end{array}
$$
$ h' $

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow 1_E \otimes \gamma \\
& & E \otimes_A A
\end{array}
$$
$ h'' $

trong đó $ c: E \to E \otimes_A E $ là đồng tích và $ h' $ và $ h'' $ là các đẳng cấu chính tắc

(II, § 3, no. 4, Mệnh đề 4). *Đơn vị của* Hom$_A$(E, B) *khi đó là ánh xạ tuyến tính* x $\mapsto$ $\gamma(x)1$ (trong đó 1 chỉ phần tử đơn vị của B).

Cho $\gamma$ là một dạng tuyến tính trên E làm cho biểu đồ (16) giao hoán. Cho B là một đại số trên A có đơn vị với phần tử đơn vị 1, $\eta:A \to B$ là ánh xạ chính tắc và $v = \eta \circ \gamma$ là phần tử của đại số trên A C = Hom$_A$(E, B). Với mọi phần tử $u \in C$, $uv$ là ánh xạ hợp thành

$$
\text{(17)} \quad E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes \gamma} E \otimes A \xrightarrow{u \otimes \eta} B \otimes B \xrightarrow{m} B.
$$

Khi đó $uv = m \circ (u \otimes \eta) \circ h'' = u$. Tương tự ta chứng minh được rằng $vu = u$ và do đó $v$ là phần tử đơn vị của C. Ngược lại, cho A-môđun A $\oplus$ E được trang bị một cấu trúc đại số có đơn vị sao cho $(a, x)(a', x') = (aa', ax' + a'x)$ với $a, a'$ thuộc A và $x, x'$ thuộc E. Ký hiệu B là đại số trên A được xác định như vậy và ký hiệu C là đại số trên A Hom$_A$(E, B). Giả sử C có đơn vị và ký hiệu $e:x \mapsto (\gamma(x), \lambda(x))$ là phần tử đơn vị của nó (trong đó $\gamma(x) \in A$ và $\lambda(x) \in E$). Mặt khác, ký hiệu $f$ là phần tử $x \mapsto (0, x)$ của C. Một tính toán ngay lập tức cho thấy rằng $fe$ là phần tử

$$
x \mapsto (0, (h'')^{-1}((1_E \otimes \gamma)(c(x))))
$$

của C. Điều kiện $fe = f$ kéo theo tính giao hoán của biểu đồ thứ hai của (16) và tương tự ta thấy rằng điều kiện $ef = f$ kéo theo tính giao hoán của biểu đồ thứ nhất của (16).

Một dạng tuyến tính $\gamma$ trên E làm cho các biểu đồ (16) giao hoán được gọi là một *đồng đơn vị* của đối đại số E. Một đối đại số có *nhiều nhất một* đồng đơn vị: vì nó là phần tử đơn vị của đại số Hom$_A$(E, A). Một đối đại số có một đồng đơn vị được gọi là *có đồng đơn vị*.

#### Ví dụ {#alg-iii-s11-n2-exa-4 .statement}

(6) Ánh xạ đồng nhất là đồng đơn vị của đối đại số A; trên đối đại số $A^{(X)}$ (no. 1, *Ví dụ 4*) dạng tuyến tính $\gamma$ sao cho $\gamma(e_x) = 1$ với mọi $x \in X$ là đồng đơn vị. Trên đối đại số T(M) (tương ứng S(M), $\Lambda(M)$) dạng tuyến tính $\gamma$ sao cho $\gamma(1) = 1$ và $\gamma(z) = 0$ đối với $z$ thuộc $T^n(M)$ (tương ứng $S^n(M)$, $\Lambda^n(M)$) với $n \geq 1$ là đồng đơn vị. Cuối cùng, cho B là một đại số trên A là một A-môđun xạ ảnh sinh hữu hạn và có một phần tử đơn vị $e$; khi đó trên đối đại số B* (no. 1, *Ví dụ 3*) dạng tuyến tính $\gamma: x^* \mapsto \langle e, x^* \rangle$ là đồng đơn vị, vì dạng này chính là chuyển vị của ánh xạ A-tuyến tính $\eta_e: \xi \mapsto \xi e$ từ A vào B và do chuyển vị, tính giao hoán của các biểu đồ (16) suy ra từ tính giao hoán của các biểu đồ biểu thị (dùng $\eta_e$) sự kiện $e$ là phần tử đơn vị của B (§ 1, no. 3); lập luận tương tự hơn nữa cho thấy ngược lại rằng, nếu đối đại số B* thừa nhận một đồng đơn vị $\gamma$, chuyển vị của $\gamma$ xác định một phần tử đơn vị $e = t_\gamma(1)$ của B.

#### Mệnh đề 4 {#alg-iii-s11-prop-4 .statement}

*Cho E là một đối đại số thừa nhận một đồng đơn vị $\gamma$ và giả sử rằng tồn tại trong E một phần tử e sao cho $\gamma(e) = 1$; khi đó E là tổng trực tiếp của các A-môđun con Ae và $E_{\gamma} = \mathrm{Ker}(\gamma)$ và*

$$
\text{(18)} \quad \begin{cases}
c(e) \equiv e \otimes e \pmod{E_{\gamma} \otimes E_{\gamma}} \\
c(x) \equiv x \otimes e + e \otimes x \pmod{E_{\gamma} \otimes E_{\gamma}} & \text{với mọi } x \in E_{\gamma}.
\end{cases}
$$

Mệnh đề đầu tiên là ngay lập tức, vì $ \gamma(x - \gamma(x)e) = 0 $ và quan hệ $ \gamma(\alpha e) = 0 $ kéo theo $ \alpha = 0 $. Cho $ c(e) = \sum_i s_i \otimes t_i $, khi đó
$$
e = \sum_i \gamma(s_i)t_i = \sum_i \gamma(t_i)s_i
$$
theo (16) và $ 1 = \gamma(e) = \sum_i \gamma(s_i)\gamma(t_i) $. Do đó
$$
\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e) = \sum_i s_i \otimes t_i - \sum_i e \otimes \gamma(s_i)t_i \\
- \sum_i \gamma(t_i)s_i \otimes e \\
+ \sum_i \gamma(s_i)e \otimes \gamma(t_i)e
$$
mà, theo quan hệ trên, chính là $ c(e) - e \otimes e $; điều này do đó chứng minh quan hệ thứ nhất của (18). Mặt khác, phân tích của $ E \otimes E $ thành tổng trực tiếp
$$
A(e \otimes e) \oplus ((Ae) \otimes E_\gamma) \oplus (E_\gamma \otimes (Ae)) \oplus (E_\gamma \otimes E_\gamma)
$$
cho phép ta viết, với $ x \in E_\gamma $, $ c(x) = \lambda(e \otimes e) + (e \otimes y) + z \otimes e) + u $ trong đó $ u = \sum_j v_j \otimes w_j, y, z $ và các $ v_j $ và $ w_j $ thuộc về $ E_\gamma $. Định nghĩa của đồng đơn vị $ \gamma $ khi đó cho $ x = \lambda e + y = \lambda e + z $ và, vì $ \gamma(x) = 0 $, tất yếu $ \lambda = 0, x = y = z $, do đó có quan hệ thứ hai của (18).

#### Nhận xét {#alg-iii-s11-n2-rem-2 .statement}

Cho C là một A-đối đại số kết hợp có đồng đơn vị, B là một A-đại số kết hợp có đơn vị và M là một B-môđun trái. Ánh xạ A-song tuyến tính $ (b, m) \mapsto bm $ từ $ B \times M $ vào M xác định một ánh xạ A-song tuyến tính
$$
\operatorname{Hom}_A(C, B) \times \operatorname{Hom}_A(C, M) \to \operatorname{Hom}_A(C, M)
$$
theo quy trình tổng quát được mô tả ở đầu số này. Ta kiểm tra ngay lập tức rằng ánh xạ này xác định trên $ \operatorname{Hom}_A(C, M) $ một cấu trúc môđun trái trên vành $ \operatorname{Hom}_A(C, B) $.

### 3. CÁC TÍNH CHẤT CỦA CÁC ĐỐI ĐẠI SỐ PHÂN BẬC KIỂU N

#### Mệnh đề 5 {#alg-iii-s11-prop-5 .statement}

(i) *Cho E là một đối đại số phân bậc thừa nhận một đồng đơn vị $ \gamma $; khi đó $ \gamma $ là một dạng tuyến tính thuần nhất có bậc 0.*

(ii) *Giả sử thêm rằng tồn tại một phần tử $ e \in E $ sao cho $ E_0 = Ae $ và $ \gamma(e) = 1 $. Khi đó hạt nhân $ E_\gamma $ của $ \gamma $ bằng $ E_+ = \sum_{n \geq 1} E_n $, $ c(e) = e \otimes e $ và*
$$
c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_+ \otimes E_+)
$$
*đối với mọi* $ x \in E_+ $.

(i) Chỉ cần kiểm tra rằng $ \gamma(x) = 0 $ đối với $ x \in E_n $, với mọi $ n \geq 1 $. Vì $ c $ là một đồng cấu phân bậc của bậc 0,

$$
c(x) = \sum_{0 \leq j \leq n} \left( \sum_i y_{ij} \otimes z_{i, n-j} \right)
$$

với, với mọi $ j $ sao cho $ 0 \leq j \leq n $, $ y_{ij} $ và $ z_{ij} $ thuộc $ E_j $; áp dụng (16) (no. 2) ta thu được

$$
x = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(y_{ij}) z_{i, n-j} \right) = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(z_{i, n-j}) y_{ij} \right),
$$

do đó, bằng cách cho các thành phần có bậc 0 và bậc $ n $ ở hai vế bằng nhau

$$
x = \sum_i \gamma(y_{i0}) z_{in} = \sum_i \gamma(z_{i0}) y_{in}
$$
$$
0 = \sum_i \gamma(y_{in}) z_{i0} = \sum_i \gamma(z_{in}) y_{i0}
$$

và do đó $ \gamma(x) = \sum_i \gamma(y_{in}) \gamma(z_{i0}) = \gamma(0) = 0 $.

(ii) Vì $ \mathrm{Ker}(\gamma) $ và $ E_+ $ đều là các A-môđun con phụ trợ của $ Ae = E_0 $ và $ E_+ \subset \mathrm{Ker}(\gamma) $ theo (i), $ E_+ = \mathrm{Ker}(\gamma) $ (II, § 1, no. 8, Nhận xét 1); các khẳng định khác suy ra từ Mệnh đề 4 của no. 2.

#### Mệnh đề 6 {#alg-iii-s11-prop-6 .statement}

*Một đối đại số phân bậc E trên A có tính chất rằng, đối với mọi A-đại số giao hoán B, với phép phân bậc tầm thường, A-đại số phân bậc kiểu $ \mathbf{Z} \mathrm{Homgr}_A(E, B) $ (no. 2) là phản giao hoán (§ 4, no. 9, Định nghĩa 7), khi và chỉ khi, nếu $ \sigma_g $ là tự đẳng cấu của A-môđun $ E \otimes_A E $ sao cho*

$$
\sigma_g(x_p \otimes x_q) = (-1)^{pq} x_q \otimes x_p
$$

đối với $ x_p \in E_p, x_q \in E_q $, *trong đó p và q là các phần tử tùy ý của $ \mathbf{N} $, biểu đồ*

$$
\begin{array}{ccc}
E & & \\
 & \searrow^c & \swarrow^c \\
E \otimes_A E & \xrightarrow{\sigma_g} & E \otimes_A E
\end{array}
$$

*là giao hoán.*

Chứng minh tương tự như chứng minh của Mệnh đề 2 của no. 2.

Khi đối đại số phân bậc E thỏa mãn điều kiện của Mệnh đề 6, nó được gọi là *phản đối giao hoán*.

#### Ví dụ {#alg-iii-s11-n3-exa-1 .statement}

Điều này suy ra ngay lập tức từ công thức (8) của no. 1 rằng đối với mọi A-môđun M, đối đại số phân bậc $ \bigwedge(M) $ là *phản đối giao hoán*.

### 4. CÁC SONG ĐẠI SỐ VÀ SONG ĐẠI SỐ LỆCH

#### Định nghĩa 3 {#alg-iii-s11-def-3 .statement}

*Một song đại số phân bậc (tương ứng, song đại số phân bậc lệch) trên một vành A là một tập hợp E với một cấu trúc A-đại số phân bậc kiểu $ \mathbf{N} $ và một cấu trúc đối đại số A-phân bậc kiểu $ \mathbf{N} $, với cùng cấu trúc A-môđun phân bậc cơ sở và sao cho:*

(1) *A-đại số E là kết hợp và có đơn vị.*

(2) *Đối đại số A E là đồng kết hợp và có đồng đơn vị.*
(3) *Đồng tích c : E \to E \otimes_A E là một đồng cấu của đại số phân bậc E vào đại số phân bậc E \otimes_A E* (tương ứng. *đại số phân bậc E^g \otimes_A E* (xem § 4, no. 7)).
(4) *Đồng đơn vị $ \gamma $ của E là một đồng cấu của đại số phân bậc E vào đại số A (với phép phân bậc tầm thường) sao cho, nếu e biểu thị phần tử đơn vị của A-đại số E, thì $ \gamma(e) = 1 $.*

Nếu E là một song đại số phân bậc có phép phân bậc *tầm thường*, E được gọi đơn giản là một *song đại số*. Một song đại số phân bậc được gọi là giao hoán (tương ứng, đồng giao hoán) nếu đại số cơ sở là giao hoán (tương ứng, nếu đối đại số cơ sở là đồng giao hoán); một song đại số phân bậc lệch được gọi là phản giao hoán (tương ứng, phản đồng giao hoán) nếu đại số phân bậc cơ sở là phản giao hoán (tương ứng, nếu đối đại số phân bậc cơ sở là phản đồng giao hoán).

Từ Định nghĩa 3 và Mệnh đề 5 no. 2 suy ra rằng, đối với một song đại số phân bậc hoặc một song đại số phân bậc lệch E,

$$
c(e) = e \otimes e \\
c(x) \equiv x \otimes e + e \otimes x (\text{mod. } E_+ \otimes E_+) \quad \text{ cho } x \in E_+ = \bigoplus_{n \geq 1} E_n.
$$

Nếu E và F là hai song đại số phân bậc (tương ứng, hai song đại số phân bậc lệch), một ánh xạ $ \phi : E \to F $ được gọi là một *cấu xạ song đại số phân bậc* (tương ứng, *cấu xạ song đại số phân bậc lệch*) nếu: (1) $ \phi $ là một cấu xạ đại số phân bậc (và do đó ánh xạ phần tử đơn vị của E vào phần tử đơn vị của F); (2) $ \phi $ là một cấu xạ đối đại số phân bậc sao cho, nếu $ \gamma $ và $ \gamma' $ là các đồng đơn vị tương ứng của E và F, thì $ \gamma = \gamma' \circ \phi $.

#### Ví dụ {#alg-iii-s11-n4-exa-1 .statement}

(1) Cho S là một nửa nhóm với phần tử đơn vị u, sao cho đại số $ E = A^{(S)} $ của nửa nhóm S trên A có phần tử đơn vị $ e_u $ (§ 2, no. 6); mặt khác đã thấy rằng E một cách chính tắc có một cấu trúc đối đại số A đồng kết hợp đồng giao hoán với một đồng đơn vị $ \gamma $ sao cho $ \gamma(e_s) = 1 $ với mọi $ s \in S $ (no. 1, Ví dụ 4 và no. 2, các Ví dụ 4, 5 và 6). Công thức $ c(e_s) = e_s \otimes e_s $ cho đồng tích cũng chỉ ra ngay lập tức rằng c là một đồng cấu đại số. Như vậy một cấu trúc *song đại số đồng giao hoán* đã được xác định trên E và E, với cấu trúc này, được gọi là *song đại số của nửa nhóm S trên A*.

Nếu T là một nửa nhóm khác với phần tử đơn vị v, $ f : S \to T $ là một đồng cấu sao cho $ f(u) = v $ và $ f_{(A)} : A^{(S)} \to A^{(T)} $ là đồng cấu đại số A dẫn xuất từ $ f $ (§ 2, no. 6), thì kiểm tra ngay lập tức được rằng $ f_{(A)} $ là một *đồng cấu song đại số*.

(2) Cho M là một A-môđun. Các cấu trúc đại số A phân bậc (§ 6, no. 1) và đối đại số A phân bậc (no. 1, Ví dụ 6) được xác định trên S(M) xác định trên tập hợp này một cấu trúc *đối giao hoán, đồng đối giao hoán, bigebra phân bậc*; vì ta đã thấy (no. 1, Ví dụ 6) rằng đồng tích trên S(M) là một đồng cấu đại số và theo định nghĩa của đồng đơn vị $ \gamma $ (no. 2, Ví dụ 6) thì $ \gamma(1) = 1 $ và $ \gamma $ là một đồng cấu đại số từ E vào A.

(3) Cho M là một A-môđun. Như trong Ví dụ 2, ta thấy rằng các cấu trúc đại số A phân bậc (§ 7, no. 1) và đối đại số A phân bậc (no. 1, Ví dụ 7) trên $ \bigwedge(M) $ xác định trên tập hợp này một cấu trúc *bigebra xiên phản giao hoán, phản đối giao hoán, phân bậc*.

#### Nhận xét {#alg-iii-s11-n4-rem-1 .statement}

Nếu M là một A-môđun sao cho $ M \otimes_A M \neq \{0\} $, các cấu trúc đại số A phân bậc (§ 5, no. 1) và đối đại số A phân bậc (no. 1, Ví dụ 5) trên $ T(M) $ *không xác định* một cấu trúc bigebra, vì nói chung

$$
c(x_1 x_2 y_1 y_2) \neq c(x_1 x_2) c(y_1 y_2)
$$

đối với bốn phần tử $ x_1, x_2, y_1, y_2 $ của M, như công thức (3) của no. 1 cho thấy.

### 5. CÁC ĐỐI NGẪU PHÂN BẬC $ T(M)^{*gr} $, $ S(M)^{*gr} $ VÀ $ \bigwedge(M)^{*gr} $

*Từ đây trở đi, ta trở lại các quy ước tổng quát của chương về các đại số, do đó sẽ giả thiết rằng chúng kết hợp và có đơn vị (trừ khi có nói khác).*

Cho M là một A-môđun; các cấu trúc đối đại số A phân bậc được xác định trên $ T(M) $ (no. 1, Ví dụ 5), $ S(M) $ (no. 1, Ví dụ 6) và $ \bigwedge(M) $ (no. 1, Ví dụ 7) cho phép ta xác định một cách chính tắc trên các đối ngẫu phân bậc $ T(M)^{*gr} $, $ S(M)^{*gr} $ và $ \bigwedge(M)^{*gr} $ các cấu trúc *đại số phân bậc* kiểu N, theo no. 2, các Mệnh đề 1 và 3 và quy ước về phân bậc của đối ngẫu phân bậc của một môđun phân bậc (no. 1). Hơn nữa, đại số phân bậc $ S(M)^{*gr} $ là *giao hoán* (no. 2, Mệnh đề 2 và Ví dụ 5) và đại số phân bậc $ \bigwedge(M)^{*gr} $ là *phản giao hoán* (no. 3, Mệnh đề 6 và Ví dụ). Trong $ \bigwedge(M)^{*gr} $ *mọi phần tử bậc 1 đều có bình phương bằng không*; một phần tử như vậy được đồng nhất với một dạng tuyến tính $ f $ trên M và bình phương của nó là dạng song tuyến tính phản xứng $ f \wedge f $ trên $ M^2 $ sao cho

$$
(f \wedge f)(x, y) = f(x) f(y) - f(y) f(x)
$$

(no. 2, Ví dụ 3).

Cho N là một A-môđun khác và $ u $ là một ánh xạ A-tuyến tính từ M vào N. Ta biết rằng $ u $ xác định một cách chính tắc các đồng cấu đại số phân bậc

$$
\begin{cases}
T(u): T(M) \to T(N) \\
S(u): S(M) \to S(N) \\
\bigwedge(u): \bigwedge(M) \to \bigwedge(N)
\end{cases}
$$

(§ 5, no. 2, § 6, no. 2 và § 7, no. 2). Ngay lập tức kiểm tra được từ công thức (3) của no. 1 rằng $ T(u) $ cũng là một *cấu xạ đối đại số*. Mặt khác, nếu $ \Delta_M $ (tương ứng $ \Delta_N $) ký hiệu ánh xạ đường chéo $ M \to M \times M $ (tương ứng $ N \to N \times N $), thì có quan hệ $(u \times u) \circ \Delta_M = \Delta_N \circ u$; suy ra $ S(u \times u) \circ S(\Delta_M) = S(\Delta_N) \circ S(u) $

(tương ứng $ \Lambda(u \times u) \circ \Lambda(\Delta_M) = \Lambda(\Delta_N) \circ \Lambda(u) $).

Dùng định nghĩa của đồng tích trong $ S(M) $ và $ \Lambda(M) $ (no. 1, các Ví dụ 6 và 7) và tính chất hàm tử của các đẳng cấu chính tắc

$$
S(M \times M) \to S(M) \otimes_A S(M)
$$

và $ \Lambda(M \times M) \to \Lambda(M)^{\text{g}} \otimes_A \Lambda(M) $, ta thấy rằng $ S(u) $ và $ \Lambda(u) $ cũng là các *cấu xạ đối đại số*† (và do đó trong trường hợp này là các cấu xạ *bigebra*). Suy ra ngay lập tức rằng các *đối chuyển phân bậc* (II, § 11, no. 6) của các đồng cấu (23)

$$
\begin{align*}
tT(u): T(N)^{*gr} &\to T(M)^{*gr} \\
tS(u): S(N)^{*gr} &\to S(M)^{*gr} \\
t\Lambda(u): \Lambda(N)^{*gr} &\to \Lambda(M)^{*gr}
\end{align*}
$$

là các *đồng cấu đại số phân bậc*.

Bây giờ ta lưu ý rằng đối ngẫu $ M^* $ của M được đồng nhất với môđun con gồm các phần tử bậc 1 trong $ T(M)^{*gr} $ (tương ứng $ S(M)^{*gr} $, $ \Lambda(M)^{*gr} $). Do đó, theo tính chất phổ quát của đại số tenxơ (§ 5, no. 1) và tính chất phổ quát của đại số đối xứng (§ 6, no. 1), *tồn tại duy nhất một đồng cấu đại số phân bậc*

$$
\theta_T: T(M^*) \to T(M)^{*gr}
$$

*mở rộng đơn ánh chính tắc* $ M^* \to T(M)^{*gr} $, *và tồn tại duy nhất một đồng cấu đại số phân bậc*

$$
\theta_S: S(M^*) \to S(M)^{*gr}
$$

*mở rộng đơn ánh chính tắc* $ M^* \to S(M)^{*gr} $. Mặt khác, đơn ánh chính tắc của $ M^* $ vào đại số *đối* của $ \Lambda(M)^{*gr} $ sao cho bình phương của mọi phần tử của $ M^* $ bằng không; do đó (§ 7, no. 1, Mệnh đề 1) *tồn tại duy nhất một đồng cấu đại số phân bậc*

$$
\theta_\Lambda: \Lambda(M^*) \to (\Lambda(M)^{*gr})^0
$$

*mở rộng đơn ánh chính tắc* $ M^* \to \Lambda(M)^{*gr} $.‡ Các đồng cấu này

† Điều này cũng suy ra từ các công thức (5) và (9) của no. 1.
‡ Đơn ánh này được mở rộng thành một đồng cấu vào đại số đối của $ \Lambda(M)^{*gr} $ thay vì thành một đồng cấu vào $ \Lambda(M)^{*gr} $ vì thuận tiện cho các tính toán.

là hàm tử: chẳng hạn, với mọi $ A $-môđun homomorphism $ u : M \to N $, biểu đồ

$$
\begin{array}{ccc}
T(N^*) & \xrightarrow{T(tu)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(N)^{*gr} & \xrightarrow{t_{T(n)}} & T(M)^{*gr}
\end{array}
$$

là giao hoán, như suy ra ngay lập tức từ tính chất phổ quát của đại số tenxơ (\S 5, no. 1); có các biểu đồ giao hoán tương tự đối với $ \theta_S $ và $ \theta_\wedge $.

Ta sẽ tìm các đồng cấu $ \theta_T, \theta_S $ và $ \theta_\wedge $ một cách tường minh. Với mục đích này, nói chung hơn, xét một đối đại số $ A $-kết hợp $ E $ với đồng tích $ c $ và định nghĩa bằng quy nạp theo $ n $, với $ n \geq 2 $, ánh xạ tuyến tính $ c_n $ của $ E $ vào $ E^{\otimes n} $ bởi $ c_2 = c $ và
$$
c_n = (c_{n-1} \otimes 1_E) \circ c.
$$
Mặt khác, ta ký hiệu $ m_n : A^{\otimes n} \to A $ là ánh xạ tuyến tính chính tắc sao cho $ m_n(\xi_1 \otimes \xi_2 \otimes \cdots \otimes \xi_n) = \xi_1 \xi_2 \cdots \xi_n $ và chú ý rằng, với $ n \geq 2 $,
$$
m_n = m \circ (m_{n-1} \otimes 1_A)
$$
với $ m = m_2 $. Với ký hiệu này:

#### Bổ đề 1 {#alg-iii-s11-lem-1 .statement}

(i) *Trong đại số kết hợp $ E^* = \mathrm{Hom}_A(E, A) $, tích của $ n $ phần tử $ u_1, u_2, \ldots, u_n $ có bậc 1 được cho bởi*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n.
$$
(ii) *Giả sử thêm rằng đối đại số $ E $ được phân bậc. Khi đó, trong đại số kết hợp phân bậc $ E^{*gr} = \mathrm{Homgr}_A(E, A) $, tích của $ n $ phần tử $ u_1, u_2, \ldots, u_n $ có bậc 1 được cho bởi*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ \delta_n
$$
*trong đó $ \delta_n : E \to E^{\otimes n} $ là ánh xạ tuyến tính biến mỗi $ x \in E $ thành thành phần của $ c_n(x) $ có đa bậc $ (1, 1, \ldots, 1) $.*

Công thức (26) chỉ là định nghĩa của tích trong $ E^* $ với $ n = 2 $; để chứng minh nó bằng quy nạp theo $ n $, hãy chú ý rằng
$$
u_1 u_2 \ldots u_n
$$
$$
= m \circ ((u_1 u_2 \ldots u_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ ((m_{n-1} \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1}) \circ c_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ (m_{n-1} \otimes 1_A) \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1} \otimes u_n) \circ (c_{n-1} \otimes 1_E) \circ c
$$
$$
= m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n
$$
do (24), (25), II, \S 3, no. 3, công thức (5) và quan hệ
$$
u_n = 1_A \circ u_n \circ 1_{E^*}.
$$

Khi E được phân bậc và các phần tử $ u_i \in E^{*gr} $ thuần nhất có bậc 1, thì theo định nghĩa đối với các phần tử *thuần nhất* $ x_i \in E $,

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_n)(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0
$$

trừ khi tất cả các $ x_i $ đều có bậc 1, do đó có công thức (27).

Từ các công thức (3), (5) và (7) của no. 1 và công thức (24), khi E được lấy lần lượt là một trong ba đối đại số phân bậc $ \mathbf{T}(M) $, $ \mathbf{S}(M) $ và $ \mathbf{\Lambda}(M) $, ta thu được bằng quy nạp theo $ n $ (sử dụng sự kiện rằng đồng tích là một đồng cấu phân bậc có bậc 0), với $ x_1, x_2, \ldots, x_n $ thuộc M:

khi $ E = \mathbf{T}(M) $,
$$
\delta_n(x_1 x_2 \cdots x_n) = x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$

khi $ E = \mathbf{S}(M) $,
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$

khi $ E = \mathbf{\Lambda}(M) $,
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma \cdot x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}.
$$

Chỉ cần nhận xét, chẳng hạn khi $ E = \mathbf{\Lambda}(M) $, rằng trong biểu thức
$$
c_n(x_1 x_2 \cdots x_n) = (c_{n-1} \otimes 1_E) \left( \sum (-1)^v (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}}) \right)
$$
suy ra từ công thức (8) của no. 1, các số hạng duy nhất có thể cho một số hạng có đa bậc $(1, 1, \ldots, 1)$ là các số hạng mà $ n - p = 1 $ và do đó
$$
\delta_n(x_1 x_2 \cdots x_n)
$$
là số hạng có đa bậc $(1, 1, \ldots, 1)$ trong tổng
$$
\sum_{i=1}^n (-1)^{n-i} c_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i
$$
và số hạng này nhất thiết bằng
$$
\sum_{i=1}^n (-1)^{n-i} \delta_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i,
$$
do đó suy ra kết quả theo giả thiết quy nạp.

Dùng Bổ đề 1, tích trong $ \mathbf{T}(M)^{*gr} $ của $ n $ dạng tuyến tính $ x_1^*, x_2^*, \ldots, x_n^* $ của $ M^* $ được cho bởi

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
với $ x_i \in M $ ($ 1 \leq i \leq n $); tích của $ n $ dạng này trong $ \mathbf{S}(M)^{*gr} $ được cho bởi

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right);
$$

cuối cùng, tích của các dạng này trong $ \bigwedge(M)^{*gr} $ được cho bởi
$$
\langle x_1^* x_1^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \det(\langle x_i^*, x_j \rangle).
$$
Trong mỗi trường hợp trong ba trường hợp, lần lượt ta có
$$
\theta_T(x_1^* \otimes x_2^* \otimes \ldots \otimes x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_S(x_1^* x_2^* \ldots x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) = x_n^* x_{n-1}^* \ldots x_1^* = (-1)^{n(n-1)/2} x_1^* x_2^* \ldots x_n^*
$$
và do đó suy ra từ (28), (29) và (30) các hệ thức
$$(28\ \mathrm{bis})\quad \langle \theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*), x_1 \otimes x_2 \otimes \cdots \otimes x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle$$
(nói cách khác $ \theta_T $ hạn chế trên $ T^2(M^*) $ chính là đồng cấu chính tắc của II, § 4, no. 4)
$$(29\ \mathrm{bis})\quad \langle \theta_S(x_1^* x_2^* \ldots x_n^*), x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right)$$
$$(30\ \mathrm{bis})\quad \langle \theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*), x_1 \wedge x_2 \wedge \cdots \wedge x_n \rangle$$
$$
= (-1)^{n(n-1)/2} \det(\langle x_i^*, x_j \rangle).
$$

#### Mệnh đề 7 {#alg-iii-s11-prop-7 .statement}

*Cho M là một A-môđun xạ ảnh sinh hữu hạn. Khi đó các đồng cấu chính tắc $ \theta_T : T(M^*) \to T(M)^{*gr} $ và $ \theta_\Lambda : \bigwedge(M^*) \to (\bigwedge(M)^{*gr})^0 $ là song ánh. Ngoài ra đối ngẫu phân bậc $ \bigwedge(M)^{*gr} $ khi đó bằng đối ngẫu $ \bigwedge(M)^* $ của A-môđun $ \bigwedge(M) $.*

Trước hết giả sử rằng M có một *cơ sở hữu hạn* $ (e_i)_{1 \leq i \leq m} $ và cho $ (e_i^*)_{1 \leq i \leq m} $ là cơ sở đối ngẫu của $ M^* $ (II, § 10, no. 4). Công thức (28 bis) chỉ ra rằng, với mọi dãy hữu hạn $ s = (j_k)_{1 \leq k \leq n} $ gồm n phần tử của khoảng $ [1, m] $ của $ \mathbf{N} $,
$$
\theta_T(e_{j_1}^* \otimes \cdots \otimes e_{j_n}^*)
$$
là phần tử có chỉ số s trong cơ sở của $ (T^n(M))^* $, *đối ngẫu* với cơ sở của $ T^n(M) $ gồm các $ e_s = e_{j_1} \otimes \cdots \otimes e_{j_n} $ (\S 5, no. 5, Định lý 1). Do đó $ \theta_T $ là song ánh.

Tương tự, công thức (30 bis) chỉ ra rằng, với mọi tập con hữu hạn H của $ [1, m] $ có n phần tử, $ (-1)^{n(n-1)/2} \theta_\Lambda(e_H^*) $ (ký hiệu của § 7, no. 8, Định lý 1) là phần tử có chỉ số H trong cơ sở của $ (\bigwedge^n(M))^* $, *đối ngẫu* với cơ sở của $ \bigwedge^n(M) $ gồm các $ e_H $. Do đó $ \theta_\Lambda $ là song ánh.

Bây giờ giả sử chỉ rằng M là sinh hữu hạn và xạ ảnh; khi đó M là một nhân tử trực tiếp của một A-môđun tự do sinh hữu hạn L, do đó tồn tại hai ánh xạ A-tuyến tính $ M \xrightarrow{j} L \xrightarrow{p} M $ mà hợp thành của chúng là đồng nhất $ l_M $. Ta suy ra một biểu đồ giao hoán

$$
\begin{array}{ccc}
T(M^*) & \xrightarrow{T(tj)} & T(L^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(M)^{*gr} & \xrightarrow{tT(j)} & T(L)^{*gr}
\end{array}
$$
$$
\begin{array}{ccc}
T(L^*) & \xrightarrow{T(tp)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(L)^{*gr} & \xrightarrow{tT(p)} & T(M)^{*gr}
\end{array}
$$

và một biểu đồ giao hoán tương tự trong đó $ T $ được thay bởi $ \Lambda $. Mệnh đề suy ra từ bổ đề sau:

#### Bổ đề 2 {#alg-iii-s11-lem-2 .statement}

*Cho*

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y & \xrightarrow{v} & X \\
f \downarrow & & g \downarrow & & f \downarrow \\
X' & \xrightarrow{u'} & Y' & \xrightarrow{v'} & X'
\end{array}
$$

*là một biểu đồ giao hoán của các tập hợp và các ánh xạ sao cho $ v \circ u $ và $ v' \circ u' $ lần lượt là các ánh xạ đồng nhất của $ X $ và $ X' $. Khi đó, nếu $ g $ là đơn ánh (tương ứng toàn ánh, tương ứng song ánh), thì $ f $ cũng vậy.*

$ u $ là đơn ánh vì $ v \circ u $ là như vậy, do đó, nếu $ g $ là đơn ánh, $ u' \circ f = g \circ u $ là đơn ánh và vì vậy $ f $ là đơn ánh. Tương tự $ v' $ là toàn ánh vì $ v' \circ u' $ là như vậy; do đó, nếu $ g $ là toàn ánh, $ f \circ v = v' \circ g $ là toàn ánh và vì vậy $ f $ là toàn ánh.

Khẳng định cuối cùng của Mệnh đề 7 suy ra từ sự kiện rằng $ \Lambda(M) $ khi đó là một A-môđun sinh hữu hạn (\S 7, no. 3, Mệnh đề 6 và II, \S 11, no. 6, Nhận xét).

Bây giờ ta xét điều có thể nói về đồng cấu $ \theta_S $ khi $ M $ là *xạ ảnh và sinh hữu hạn*. Trước hết giả sử rằng $ M $ thừa nhận một cơ sở hữu hạn $ (e_i)_{1 \leq i \leq m} $. Theo ký hiệu ở đầu chương, A-môđun $ S^n(M) $ nhận làm cơ sở họ các phần tử $ e^\alpha $ sao cho $ |\alpha| = n $. Gọi $ u_\alpha $ (với $ |\alpha| = n $) là phần tử có chỉ số $ \alpha $ trong cơ sở của $ (S^n(M))^* $ *đối ngẫu* với $ (e^\alpha) $. Các phần tử $ u_\alpha $, với $ \alpha \in \mathbf{N}^m $, do đó tạo thành một cơ sở của đại số $ S(M)^{*gr} $ và ta sẽ thu được bảng phép nhân của cơ sở này một cách tường minh. Ta viết

$$
u_\alpha u_\beta = \sum_{\gamma \in \mathbf{N}^m} a_{\alpha \beta \gamma} u_\gamma \quad \text{với } a_{\alpha \beta \gamma} \in A.
$$

Khi đó theo định nghĩa

$$
a_{\alpha \beta \gamma} = \langle u_\alpha u_\beta, e^\gamma \rangle = m((u_\alpha \otimes u_\beta)(c(e^\gamma))),
$$

trong đó $ m : A \otimes A \to A $ xác định phép nhân trên $ A $ và $ c $ là đồng tích của $ S(M) $. Nói cách khác, $ a_{\alpha \beta \gamma} $ chỉ là hệ số của $ e^\alpha \otimes e^\beta $ khi $ c(e^\gamma) $ được viết theo cơ sở của $ S(M) \otimes S(M) $ gồm các $ e^\xi \otimes e^\eta $, trong đó $ \xi $ và $ \eta $ chạy qua $ \mathbf{N}^m $. Nhưng vì $ c $ là một đồng cấu đại số,

$$
c(e^\gamma) = \prod_{i=1}^m (c(e_i))^{r_i} = \prod_{i=1}^m (e_i \otimes 1 + 1 \otimes e_i)^{r_i}
$$

theo công thức (4) của no. 1; điều này cho

(31)
$$
c(e^\gamma) = \sum_{\xi + \eta = \gamma} (\xi, \eta) e^\xi \otimes e^\eta
$$
trong đó ta viết

(32)
$$
((\xi, \eta)) = \prod_{i=1}^n \frac{(\xi_i + \eta_i)!}{\xi_i! \eta_i!} \quad \text{(xem § 10, no. 4, công thức (18))}.
$$
Do đó ta thu được bảng phép nhân

(33)
$$
u_\alpha u_\beta = ((\alpha, \beta)) u_{\alpha + \beta}.
$$
Mặt khác, nếu $ (e_i^*)_{1 \leq i \leq m} $ là cơ sở của $ M^* $, đối ngẫu với $ (e_i) $, thì suy ra từ công thức (29 bis) rằng, với mọi $ \alpha \in \mathbf{N}^m $,

(34)
$$
\theta_S(e^{*\alpha}) = \alpha! u_\alpha
$$
theo ký hiệu của § 6, no. 6. Vì vậy đồng cấu $ \theta_S $ là song ánh khi và chỉ khi các $ \alpha! u_\alpha $ tạo thành một *cơ sở* của $ S(M)^{*gr} $, hoặc cũng tương đương với việc các phần tử $ \alpha! 1 $ là *khả nghịch*.

#### Mệnh đề 8 {#alg-iii-s11-prop-8 .statement}

*Giả sử vành $ A $ là một đại số trên trường $ \mathbf{Q} $ các số hữu tỉ; khi đó, với mọi $ A $-môđun xạ ảnh sinh hữu hạn $ M $, đồng cấu*

$$
\theta_S : S(M^*) \to S(M)^{*gr}
$$
*là song ánh.*

Điều đó quy về việc chứng minh điều này khi $ M $ sinh hữu hạn và tự do; ta chuyển từ trường hợp này sang trường hợp tổng quát bằng cách sử dụng Bổ đề 2 như trong chứng minh Mệnh đề 7.

#### Nhận xét {#alg-iii-s11-n5-rem-1 .statement}

Cho $ M $ là một $ A $-môđun và $ \rho : A \to B $ một đồng cấu vành giao hoán. Khi đó có một biểu đồ giao hoán gồm các đồng cấu đại số trên $ B $ phân bậc

$$
\begin{array}{ccc}
T((M^*)_{(B)}) & \longrightarrow & (T(M)^{*gr})_{(B)} \\
\downarrow_{T(u_M)} & & \downarrow^{u_{T(M)}} \\
T((M_{(B)})^*) & \xrightarrow{\theta_T} & T(M_{(B)})^{*gr}
\end{array}
$$

trong đó hàng thứ nhất là một đồng cấu hợp thành từ đồng cấu $ \theta_T \otimes 1_B : T(M^*) \otimes_A B \to T(M)^{*gr} $ và đẳng cấu chính tắc

$$
T((M^*)_{(B)}) \to T(M^*) \otimes_A B
$$

§ 5, no. 3, Mệnh đề 5). Ta kiểm tra ngay lập tức, bằng cách sử dụng công thức (28) và định nghĩa của đồng cấu $ v_E $ (II, § 5, no. 4), rằng biểu đồ này là *giao hoán*. Khi M là một *A-môđun xạ ảnh sinh hữu hạn*, $ M_{(B)} $ là một B-môđun xạ ảnh sinh hữu hạn (II, § 5, no. 1, Hệ quả của Mệnh đề 4) và tất cả các đồng cấu của biểu đồ trên đều *song ánh* (Mệnh đề 7 và II, § 5, no. 4, Mệnh đề 8). Có những biểu đồ giao hoán tương tự với T được thay bằng S hoặc $ \Lambda $; biểu đồ đối với $ \Lambda $ cũng gồm các đồng cấu song ánh khi M là xạ ảnh và sinh hữu hạn (Mệnh đề 7); nếu thêm nữa A là một đại số trên $ \mathbf{Q} $, thì biểu đồ đối với S cũng gồm các đồng cấu song ánh (Mệnh đề 8).

### 6. TÍCH NỘI: TRƯỜNG HỢP CÁC ĐẠI SỐ

Cho $ E = \bigoplus_{p \geq 0} E_p $ là một *đại số A phân bậc* kiểu $ \mathbf{N} $ và P là một A-môđun phân bậc kiểu $ \mathbf{Z} $; với mọi phần tử *thuần nhất* $ x \in E_p $, phép nhân *trái* bởi x là một ánh xạ A-tuyến tính $ e(x) $ của E vào chính nó, *phân bậc có bậc p*. Với mọi phần tử $ u \in \mathrm{Homgr}_A(E, P) $, *tích nội phải của u bởi x*, ký hiệu $ u \perp x $, là phần tử $ u \circ e(x) $ của $ \mathrm{Homgr}_A(E, P) $. Ta cũng viết $ (i(x))(u) = u \perp x $ và thấy rằng $ i(x) $ là một tự đồng cấu phân bậc có bậc p của A-môđun A phân bậc $ \mathrm{Homgr}_A(E, P) $. Nếu bây giờ $ x = \sum_{p \geq 0} x_p $ là một phần tử tùy ý của E (với $ x_p \in E_p $ với mọi $ p \geq 0 $, $ x_p = 0 $ ngoại trừ một số hữu hạn giá trị của $ p $), ta viết $ i(x) = \sum_{p=0}^\infty i(x_p) $, do đó đây là một tự đồng cấu của A-môđun $ \mathrm{Homgr}_A(E, P) $.

Để nhớ phần tử nào, trong biểu thức $ u \perp x $, “tác động” lên phần tử kia, hãy lưu ý rằng phần tử x “tác động” lên u được đặt ở đầu tự do của đường ngang trong $ \perp $.

*Tính kết hợp* của đại số E chuyển thành quan hệ $ e(xy) = e(x) \circ e(y) $ với $ x, y $ thuần nhất; do đó, theo định nghĩa của $ i(x) $,

$$
i(xy) = i(y) \circ i(x)
$$

trước hết với $ x, y $ thuần nhất và sau đó, nhờ tính tuyến tính, với $ x, y $ *tùy ý* trong E; điều này cũng có thể được viết

$$
(u \perp x) \perp y = u \perp (xy)
$$

với $ x, y $ trong E và $ u \in \mathrm{Homgr}_A(E, P) $; mặt khác, rõ ràng $ i(1) $ là ánh xạ đồng nhất (vì điều này suy ra từ $ e(1) = 1_E $) và $ x \mapsto i(x) $ là *A-tuyến tính*, do đó ta thấy rằng phép toán ngoài của phép hợp thành $ (x, u) \mapsto u \perp x $ ($ x \in E, u \in \mathrm{Homgr}_A(E, P) $) xác định, cùng với phép cộng, một cấu trúc *môđun E phải* trên $ \mathrm{Homgr}_A(E, P) $.

Đặc biệt, ta xét trường hợp $ P = A $, trong đó $ \mathrm{Homgr}_A(E, P) $ trong trường hợp này là **đối ngẫu phân bậc** $ E^{*gr} $ của $ E $; $ i(x) $ khi đó là **chuyển vị phân bậc** của **ánh xạ tuyến tính** $ e(x) $ (II, § 11, no. 6), nói cách khác, với mọi $ x, y $ trong $ E $, $ u \in E^{*gr} $,

$$
\langle u \sqcup x, y \rangle = \langle u, xy \rangle.
$$

Theo quy ước ở đầu đoạn, chú ý rằng, nếu $ x \in E_p $, thì $ i(x) $ là một tự đồng cấu của $ E^{*gr} $ **có bậc** $ -p $.

Với mọi phần tử thuần nhất $ x \in E_p $, phép nhân **phải** với $ x $ cũng được ký hiệu là $ e'(x) $ và phần tử $ u \circ e'(x) $ của $ \mathrm{Homgr}_A(E, P) $, được gọi là **tích nội bên trái của u bởi x**, bởi $ x \sqcup u $; ta viết $ i'(x) = x \sqcup u $ và do đó $ i'(x) $ là một tự đồng cấu phân bậc của $ \mathrm{Homgr}_A(E, P) $ có bậc $ p $; như trên, định nghĩa này có thể mở rộng đến trường hợp $ x $ là một phần tử tùy ý của $ E $. Vì trong trường hợp này $ e'(xy) = e'(y)e'(x) $,

$$
i'(xy) = i'(x) \circ i'(y)
$$

điều này cũng có thể viết là

$$
x \sqcup (y \sqcup u) = (xy) \sqcup u
$$

và cho thấy rằng phép toán ngoài của hợp thành $ (x, u) \mapsto x \sqcup u $ xác định, cùng với phép cộng, một cấu trúc **E-môđun trái** trên $ \mathrm{Homgr}_A(E, P) $. Mặt khác, tính kết hợp của $ E $ kéo theo $ e(x) \circ e'(y) = e'(y) \circ e(x) $ với $ x, y $ thuần nhất trong $ E $, do đó có quan hệ

$$
(y \sqcup u) \sqcup x = y \sqcup (u \sqcup x)
$$

vì vậy hai phép toán ngoài của hợp thành trên $ \mathrm{Homgr}_A(E, P) $ xác định trên tập hợp này một cấu trúc **song môđun (E, E)** (II, § 1, no. 14).

Khi lấy $ P = A $, $ i'(x) $ là chuyển vị phân bậc của $ e'(x) $; nói cách khác, với mọi $ x, y $ trong $ E $, $ u \in E^{*gr} $,

$$
\langle y, x \sqcup u \rangle = \langle yx, u \rangle.
$$

Khi đại số phân bậc $ E $ là **giao hoán**, hiển nhiên $ u \sqcup x = x \sqcup u $. Khi $ E $ là **phản giao hoán** và $ P = A $, thì với $ x \in E_p $, $ y \in E_r $ và $ u \in E_q^* $, $ yx = (-1)^{pr} xy $, do đó, theo (37) và (41), $ \langle u \sqcup x, y \rangle = (-1)^{pr} \langle y, x \sqcup u \rangle $. Nhưng vì hai vế của quan hệ này đều bằng không trừ khi $ r = q - p $,

$$
x \sqcup u = (-1)^{p(q-p)} u \sqcup x.
$$

Cho $ F $ là một đại số $ A $-phân bậc khác và $ \phi : E \to F $ là một $ A $-đồng cấu của các đại số phân bậc; khi đó $ \tilde{\phi} = \mathrm{Hom}(\phi, 1_P) : \mathrm{Homgr}_A(F, P) \to \mathrm{Homgr}_A(E, P) $ là một $ A $-đồng cấu của bậc 0; theo định nghĩa, với $ x, y $ trong $ E $ và $ u \in \mathrm{Homgr}_A(F, P) $

$$
\begin{align*}
(\tilde{\phi}(u \sqcup \phi(x)))(y) &= (u \sqcup \phi(x))(\phi(y)) \\
&= u(\phi(x)\phi(y)) = u(\phi(xy)) = (\tilde{\phi}(u))(xy) = (\tilde{\phi}(u) \sqcup x)(y)
\end{align*}
$$

hoặc cũng có

$$
\tilde{\phi}(u \sqcup \phi(x)) = \tilde{\phi}(u) \sqcup x
$$

và tương tự

$$
\tilde{\phi}(\phi(x) \sqcup u) = x \sqcup \tilde{\phi}(u).
$$

Nói cách khác, khi Homgr_A(F, P) được xem như một song môđun $(E, E)$ nhờ đồng cấu vành $ \phi : E \to F $, ta thấy rằng $ \tilde{\phi} $ là một đồng cấu song môđun $(E, E)$ (hay cũng là một $ E $-đồng cấu của song môđun $(F, F)$ Homgr_A(F, P) vào song môđun $(E, E)$ Homgr_A(E, P)).

#### Ví dụ {#alg-iii-s11-n6-exa-1 .statement}

Đặc biệt, điều trên có thể áp dụng khi E là một trong các đại số phân bậc T(M), S(M) hoặc $ \bigwedge(M) $ đối với một A-môđun M và P là một A-môđun (với phép phân bậc tầm thường). Để tìm tường minh các cấu trúc song môđun thu được như vậy, chú ý rằng các phần tử bậc $-n$ của Homgr_A(T(M), P) (resp. Homgr_A(S(M), P), resp. Homgr_A($ \bigwedge(M) $, P)) được đồng nhất với các *ánh xạ n-tuyến tính* (resp. *ánh xạ n-tuyến tính đối xứng*, resp. *ánh xạ n-tuyến tính phản xứng*) từ $ M^n $ vào P. Chỉ cần biểu diễn các tích

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$

(resp. $ f \sqcup (x_1 x_2 \ldots x_p) $), resp. $ f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) $) đối với mọi dãy hữu hạn $ (x_i)_{1 \leq i \leq p} $ các phần tử của M và các tích nội bên trái tương ứng. Ngay lập tức từ các định nghĩa suy ra rằng

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f = 0
$$

*nếu* $ p > n $ và, với $ p \leq n $, $ f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) $ (resp.

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)
$$

là ánh xạ *(n - p)*-tuyến tính được định nghĩa bởi

$$
\begin{cases}
(f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p))(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(x_1, \ldots, x_p, y_1, \ldots, y_{n-p}) \\
((x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(y_1, \ldots, y_{n-p}, x_1, \ldots, x_p).
\end{cases}
$$

Với $ p > n $, trong Homgr_A(S(M), P) (resp. Homgr_A($ \bigwedge(M) $, P)) cũng có các công thức (44) khi thay $ x_1 \otimes x_2 \otimes \cdots \otimes x_p $ bằng $ x_1 x_2 \ldots x_p $ (resp. $ x_1 \wedge x_2 \wedge \cdots \wedge x_p $). Với $ p \leq n $, những phép thay thế tương tự trong (45) định nghĩa các *ánh xạ* *(n - p)*-tuyến tính *đối xứng* $ f \sqcup (x_1 x_2 \ldots x_p) $ và $ (x_1 x_2 \ldots x_p) \sqcup f $ (resp. các *ánh xạ* *(n - p)*-tuyến tính *phản xứng*

$$
f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \quad \text{and} \quad (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \sqcup f).
$$

Khi $ n = p $, các tích trên bằng hàm hằng trên $ M $ bằng $ f(x_1, \ldots, x_p) $.

Nếu $ u : M \to N $ là một đồng cấu A-môđun, $ T(u) : T(M) \to T(N) $ là một đồng cấu đại số A-phân bậc, thì từ những gì đã thấy ở trên suy ra rằng $ (T(u))^\sim $ là một $ T(M) $-đồng cấu của song môđun $ (T(N), T(N)) $ $\mathrm{Homgr}_A(T(N), P) $ vào song môđun $ (T(M), T(M)) $ $\mathrm{Homgr}_A(T(M), P) $, tương ứng với đồng cấu vành $ T(u) $. Có các kết quả tương tự đối với $ (S(u))^\sim $ và $ (\wedge(u))^\sim $.

### 7. TÍCH NỘI: TRƯỜNG HỢP CÁC CÔĐẠI SỐ

Cho $ E = \bigoplus_{p \geq 0} E_p $ là một đối đại số phân bậc đối kết hợp có phần tử đối đơn vị. Khi đó ta biết (no. 2, các Mệnh đề 1 và 3) rằng đối ngẫu phân bậc $ E^{*\mathrm{gr}} $ có (với quy ước về phân bậc được nêu ở đầu đoạn) một cấu trúc đại số phân bậc kiểu $ \mathbf{N} $ trên $ A $, tích của hai phần tử $ u, v $ của đại số này được xác định bởi $ uv = m \circ (u \otimes v) \circ c $, trong đó $ c : E \to E \otimes_A E $ là đồng tích và $ m : A \otimes_A A \to A $ xác định phép nhân. Nói cách khác, nếu với $ x \in E $, $ c(x) = \sum_i y_i \otimes z_i $, ta có thể viết (đồng nhất một cách chính tắc $ A \otimes_A E $ và $ E $)

$$
\langle x, uv \rangle = (uv)(x) = \sum_i u(y_i)v(z_i) = v\left( \sum_i u(y_i)z_i \right)
= v(((u \otimes 1_E) \circ c)(x)) = \langle ((u \otimes 1_E) \circ c)(x), v \rangle.
$$

Điều này có thể được diễn giải bằng cách nói rằng, với mọi $ u $ thuần nhất bậc $ p $ trong $ E^{*\mathrm{gr}} $, phép nhân trái $ e(u) : v \mapsto uv $ trong $ E^{*\mathrm{gr}} $ là chuyển vị phân bậc của tự đồng cấu phân bậc bậc $ -p $

$$(46)$$
$$
i(u) = (u \otimes 1_E) \circ c
$$
của $ E $; do đó, theo ký hiệu trên,

$$
(i(u))(x) = \sum_i u(y_i)z_i.
$$

Công thức (46) cũng xác định một phần tử $ i(u) \in \mathrm{Endgr}_A(E) $ với mọi phần tử $ u \in E^{*\mathrm{gr}} $; với mọi $ x \in E $ và mọi $ u \in E^{*\mathrm{gr}} $, ta viết

$$(47)$$
$$
x \perp u = (i(u))(x)
$$
sao cho, với $ u $ và $ v $ trong $ E^{*\mathrm{gr}} $,

$$
\langle x, uv \rangle = \langle x \perp u, v \rangle.
$$

Phần tử $ x \perp u $ của $ E $ được gọi là tích vô hướng phải của $ x $ bởi $ u $.

Ở đây cũng vậy, phần tử $ u $ “tác động” lên $ x $ được đặt ở đầu tự do của đường ngang trong $ \underline{\phantom{x}} $.

Với hai phần tử bất kỳ $ u, v $ của $ E^{*\mathrm{gr}} $,

$$
x \underline{\phantom{(uv)}} = (x \underline{\phantom{u}}) \underline{\phantom{v}},
$$

nói cách khác

$$
i(uv) = i(v) \circ i(u).
$$

Như trên, đặt $ c(x) = \sum_i y_i \otimes z_i $, sao cho $ x \underline{\phantom{(uv)}} = \sum_i (uv)(y_i)z_i $. Nếu

$$
c(y_i) = \sum_j y_{ij}' \otimes y_{ij}'',
$$

thì

$$
x \underline{\phantom{(uv)}} = \sum_{i,j} u(y_{ij}')v(y_{ij}'')z_i.
$$

Mặt khác, nếu $ c(z_i) = \sum_k z_{ik}' \otimes z_{ik}'' $, thì

$$
(x \underline{\phantom{u}}) \underline{\phantom{v}} = \sum_{i,k} u(y_i)v(z_{ik}')z_{ik}''.
$$

Bây giờ, tính đối kết hợp của $ E $ cho thấy rằng (no. 2, Mệnh đề 1)

$$
\sum_{i,j} y_{ij}' \otimes y_{ij}'' \otimes z_i = \sum_{i,k} y_i \otimes z_{ik}' \otimes z_{ik}''
$$

và đẳng thức của các biểu thức (49) và (50) suy ra từ sự kiện rằng chúng lần lượt là ảnh của vế trái và vế phải của (51) qua ánh xạ tuyến tính $ f $ từ $ E \otimes E \otimes E $ vào $ E $ sao cho $ f(x \otimes y \otimes z) = u(x)v(y)z $.

Mặt khác, ta nhắc lại (no. 2, Mệnh đề 3) rằng phần tử đơn vị của đại số $ E^{*\mathrm{gr}} $ là dạng tuyến tính $ e : x \mapsto \gamma(x).1 $; do đó

$$
x \underline{\phantom{e}} = \sum_i \gamma(y_i)z_i = x
$$

do định nghĩa của đồng đơn vị. Vì ánh xạ $ u \mapsto i(u) $ là tuyến tính, ta thấy rằng luật ngoài của phép hợp thành $ (u, x) \mapsto x \underline{\phantom{u}} $ xác định một cấu trúc môđun $ E^{*\mathrm{gr}} $-phải trên $ E $.

Tương tự, với mọi $ u \in E^{*\mathrm{gr}} $, ta định nghĩa tự đồng cấu của $ E $

$$
i'(u) = (1_E \otimes u) \circ c
$$

và với mọi $ x \in E $, ta viết

$$
(i'(u))(x) = u \underline{\phantom{x}}
$$

và phần tử này của $ E $ được gọi là tích nội trái của x bởi u. Như trên, ta thấy rằng luật ngoài $(u, v) \mapsto u \sqcup x$ xác định một *cấu trúc môđun $E^{*\mathrm{gr}}$-trái* trên $E$. Hơn nữa, hai cấu trúc này là *tương thích*, nói cách khác,

$$(54)$$
$$(u \sqcup x) \sqcap v = u \sqcup (x \sqcap v)$$

với $u, v$ trong $E^{*\mathrm{gr}}$ (II, § 1, no. 14). Với cùng ký hiệu như trên, vế trái của (54) là $\sum_{i,j} u(z_i)v(y_{ij}')y_{ij}''$ và vế phải là $\sum_{i,k} v(y_i)u(z_{ik}'')z_{ik}'$; đẳng thức của chúng suy ra từ sự kiện rằng chúng là các ảnh tương ứng của vế trái và vế phải của (51) qua ánh xạ tuyến tính $g$ từ $E \otimes E \otimes E$ vào $E$ sao cho $g(x \otimes y \otimes z) = v(x)u(z)y$.

Do đó ta thấy rằng hai luật ngoài của phép hợp thành trên $E$ xác định trên tập hợp này một cấu trúc $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$-*song môđun*.

Khi đối đại số $E$ là *đối giao hoán*, thì $u \sqcup x = x \sqcap u$ với mọi $x \in E$ và $u \in E^{*\mathrm{gr}}$; khi nó là *phản đối giao hoán* (\S 4, no. 9) và $u \in E_p^*$ và $x \in E_q$, ta có thể viết $c(x) = \sum_{0 \leq j \leq q} \left( \sum_i y_{ij} \otimes z_{i, q-j} \right)$ với $y_{ij}$ và $z_{ij}$ trong $E_j$ với mọi $j$ và khi đó theo giả thiết

$$\sum_i z_{ij} \otimes y_{i, q-j} = (-1)^{j(q-j)} \sum_i y_{ij} \otimes z_{i, q-j}.$$

Theo định nghĩa, $x \sqcap u = \sum_{0 \leq j \leq q} \left( \sum_i u(y_{ij})z_{i, q-j} \right)$ và

$$u \sqcup x = \sum_{0 \leq j \leq q} \left( \sum_i u(z_{i, q-j})y_{ij} \right).$$

Vì $u(y_{ij}) = 0$ (tương ứng. $u(z_{i, q-j}) = 0$ trừ khi $j = p$ (tương ứng. $q - j = p$), từ điều trên ta thấy rằng $u \sqcup x = (-1)^{p(q-p)} x \sqcap u$.

Cuối cùng, cho $\phi : E \to F$ là một *cấu xạ đối đại số phân bậc*; khi đó đã thấy (no. 2) rằng chuyển vị phân bậc $t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$ là một *đồng cấu đại số phân bậc*; do đó, với $x \in E$, $u, v$ trong $F^{*\mathrm{gr}}$,

$$
\langle \phi(x \sqcap t\phi(u)), v \rangle = \langle x \sqcap t\phi(u), t\phi(v) \rangle = \langle x, t\phi(u)t\phi(v) \rangle = \langle x, t\phi(uv) \rangle
$$
$$
= \langle \phi(x), uv \rangle = \langle \phi(x) \sqcap u, v \rangle
$$

do đó

$$(55)$$
$$\phi(x) \sqcap u = \phi(x \sqcap t\phi(u));$$

và tương tự

$$(56)$$
$$u \sqcup \phi(x) = \phi(t\phi(u) \sqcup x).$$

Nói cách khác, $\phi$ là một *đồng cấu* $F^{*\mathrm{gr}}$ của *song môđun* $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$ $E$ vào *song môđun* $(F^{*\mathrm{gr}}, F^{*\mathrm{gr}})$ $F$, tương ứng với đồng cấu vành

$$
t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}.
$$

#### Ví dụ {#alg-iii-s11-n7-exa-1 .statement}

Đặc biệt, điều trên có thể áp dụng khi E là một trong các cogebra phân bậc T(M), S(M) hoặc $ \Lambda(M) $ đối với một A-môđun M (no. 1, Ví dụ 5, 6 và 7). Để tìm tường minh các cấu trúc song môđun thu được như vậy, một lần nữa ta đồng nhất một phần tử thuần nhất f bậc n trong $ T(M)^{*gr} $ (resp. $ S(M)^{*gr} $, resp. $ \Lambda(M)^{*gr} $) với một *dạng tuyến tính n biến* (resp. *dạng tuyến tính n biến đối xứng*, resp. *dạng tuyến tính n biến phản xứng*, còn gọi là một *dạng n biến*) trên $ M^n $. Chỉ cần biểu diễn các tích

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f \text{ (resp. } (x_1 x_2 \ldots x_p) \triangleleft f,
$$

resp. $ (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f $ đối với mọi dãy hữu hạn $ (x_i)_{1 \leq i \leq p} $ các phần tử của M và các tích nội tương ứng bên trái. Khi đó, các định nghĩa (46) và (52) và các công thức (3), (6) và (9) của no. 1 lần lượt cho:

$$
\begin{cases}
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = 0 \\
(x_1 x_2 \ldots x_p) \triangleleft f = f \triangleright (x_1 x_2 \ldots x_p) = 0 \quad \text{for } p < n. \\
(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = 0
\end{cases}
$$

Đối với $ p \geq n $, ta lần lượt có

(58) $ (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f(x_1, \ldots, x_n)x_{n+1} \otimes \cdots \otimes x_p $

(59) $ (x_1 x_2 \ldots x_p) \triangleleft f = \sum_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \cdots x_{\sigma(p)} $

(60) $ (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)} $

(trong đó, trong (59) và (60), các tổng được lấy trên các hoán vị $ \sigma \in \mathfrak{S}_p $ tăng trên từng khoảng $ [1, n] $ và $ [n+1, p] $ của $ \mathbf{N} $; và tương tự

(61) $ f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = f(x_{p-n+1}, \ldots, x_p)x_1 \otimes x_2 \otimes \cdots \otimes x_{p-n} $

(62) $ f \triangleright (x_1 x_2 \ldots x_p) = \sum_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \cdots x_{\sigma(p-n)} $

(63) $ f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p-n)} $

(trong đó, trong (62) và (63), các tổng được lấy trên các hoán vị $ \sigma \in \mathfrak{S}_p $ tăng trên từng khoảng $ [1, p-n] $ và $ [p-n+1, p] $ của $ \mathbf{N} $).

### 8. TÍCH NỘI: TRƯỜNG HỢP CÁC BIGEBRA

Cho E là một bigebra phân bậc (resp. bigebra phân bậc phản xứng) (no. 4, Định nghĩa 3); khi đó các kết quả của nos. 6 và 7 có thể được áp dụng để định nghĩa các tích nội phải $ x \triangleleft u \in E $ và $ u \triangleleft x \in E^{*gr} $ (resp. $ u \triangleright x \in E $ và $ x \triangleright u \in E^{*gr} $) với mọi $ x \in E $ và mọi $ u \in E^{*\mathrm{gr}} $. Như vậy thu được một cấu trúc song môđun $(E, E)$ và một cấu trúc song môđun $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$ trên $ E $. Hơn nữa:

#### Mệnh đề 9 {#alg-iii-s11-prop-9 .statement}

*Cho $ E $ là một bigebra phân bậc (resp. bigebra phân bậc phản xứng). Với mọi phần tử $ x $ bậc 1 của $ E $, các tích nội trái và phải bởi $ x $ là các đạo hàm (resp. phản đạo hàm) ($ \S 10 $, no. 2) của đại số $ E^{*\mathrm{gr}} $.*

Trong ký hiệu của no. 6, với mọi phần tử thuần nhất $ x $ có *bậc* 1 trong một đại số bigebra phân bậc (tương ứng, một đại số bigebra phân bậc xiên) $ E $,
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$
theo Mệnh đề 5 của no. 3 và theo sự kiện rằng $ c $ là một đồng cấu có bậc 0. Trước hết giả sử rằng $ E $ là một đại số bigebra phân bậc. Với mọi $ y \in E $, theo định nghĩa
$$
\langle (uv) \mathbin{\&} x, y \rangle = \langle uv, xy \rangle = m((u \otimes v)(c(xy)))
$$
và vì $ c $ là một đồng cấu đại số, $ c(xy) = c(x)c(y) $. Đặt $ c(y) = \sum_i s_i \otimes t_i $ với $ s_i $ và $ t_i $ thuộc $ E $; do đó
$$
c(xy) = \sum_i (xs_i) \otimes t_i + \sum_i s_i \otimes (xt_i).
$$
Suy ra $ \langle (uv) \mathbin{\&} x, y \rangle = \sum_i u(xs_i)v(t_i) + \sum_i u(s_i)v(xt_i) $. Nhưng ta có thể viết
$$
\sum_i u(xs_i)v(t_i) = m(((u \mathbin{\&} x) \otimes v)(c(y))) = \langle (u \mathbin{\&} x)v, y \rangle
$$
và tương tự
$$
\sum_i u(s_i)v(xt_i) = m((u \otimes (v \mathbin{\&} x))(c(y))) = \langle u(v \mathbin{\&} x), y \rangle,
$$
do đó, trở lại ký hiệu $ i(x) $ cho tích nội.
$$(64)$$
$$(i(x))(uv) = ((i(x))(u))v + u((i(x))(v))$$
điều này chứng minh rằng $ i(x) $ là một *đạo hàm* trong $ E^{*\mathrm{gr}} $.

Bây giờ giả sử rằng $ E $ là một *đại số bigebra phân bậc xiên*, rằng $ u \in E_p^* $, $ v \in E_q^* $ và $ y \in E_r $; khi đó ta có thể viết
$$
c(y) = \sum_{0 \leq j \leq r} \left( \sum_i s_{ij} \otimes t_{i,r-j} \right)
$$
trong đó các $ s_{ij} $ và $ t_{ij} $ thuộc $ E_j $; theo định nghĩa của tích trong $ E^g \otimes_A E $, khi đó
$$
c(xy) = c(x)c(y) = \sum_{0 \leq j \leq r} \left( \sum_i (xs_{ij}) \otimes t_{i,r-j} + (-1)^j \sum_i s_{ij} \otimes (xt_{i,r-j}) \right)
$$
do đó lần này
$$
\langle (uv) \mathbin{\&} x, y \rangle = \sum_{0 \leq j \leq r} \left( \sum_i u(xs_{ij})v(t_{i,r-j}) + (-1)^j \sum_i u(s_{ij})v(xt_{i,r-j}) \right).
$$

Khi đó cũng có $ \sum_{0 \leq j \leq r} \left( \sum_i u(x s_{ij}) v(t_{i,r-j}) \right) = \langle (u \sqcup x)v, y \rangle $. Mặt khác, $ u(s_{ij}) = 0 $ trừ khi $ j = -p $ và do đó ta cũng có thể viết
$$
\sum_{0 \leq j \leq r} (-1)^j \left( \sum_i u(s_{ij}) v(x t_{i,r-j}) \right) = (-1)^p \langle u(v \sqcup x), y \rangle.
$$
Do đó ta kết luận rằng
$$
(i(x))(uv) = ((i(x))(u))v + (-1)^p u((i(x))(v)),
$$
nói cách khác $ i(x) $ là một *phản đạo hàm* trong $ E^{*gr} $. Các khẳng định liên quan đến tích nội trái bởi một phần tử $ x $ có bậc 1 trong $ E $ được chứng minh tương tự.

#### Nhận xét {#alg-iii-s11-n8-rem-1 .statement}

(1) Cho $ E $ là một đại đại số phân bậc trên $ A $ và $ N, N', N'' $ là ba $ A $-môđun phân bậc. Cho $ m $ là một ánh xạ $ A $-song tuyến tính từ $ N \times N' $ vào $ N'' $; với $ u \in \mathrm{Homgr}_A(E, N) $ và $ v \in \mathrm{Homgr}_A(E, N') $, ký hiệu $ u.v $ là đồng cấu thuần nhất $ m \circ (u \otimes v) \circ c $ từ $ E $ vào $ N'' $. Mặt khác, ký hiệu $ i(x) $ là tích vô hướng nội (phải hoặc trái) bởi $ x \in E $ trong các $ A $-môđun $ \mathrm{Homgr}_A(E, N) $, $ \mathrm{Homgr}_A(E, N') $ và $ \mathrm{Homgr}_A(E, N'') $. Khi đó, nếu $ x $ *có bậc* 1,
$$
(i(x))(u.v) = ((i(x))(u)).v + u.((i(x))(v))
$$
với mọi $ u \in \mathrm{Homgr}_A(E, N) $ và $ v \in \mathrm{Homgr}_A(E, N') $.

Với cùng các điều kiện, nếu $ E $ là một đại đại số phân bậc lệch và $ u $ thuần nhất có bậc $ p $, thì
$$
(i(x))(u.v) = ((i(x))(u)).v + (-1)^p u.((i(x))(v)).
$$
Các chứng minh cũng giống như trong Mệnh đề 9.

(2) Cùng lập luận như trong chứng minh trên chứng minh, nói chung, rằng với mọi $ x \in E $, nếu $ c(x) = \sum_j x'_j \otimes x''_j $, thì với mọi $ u, v $ trong $ E^{*gr} $, “công thức Leibniz”
$$
(i(x))(uv) = \sum_j (i(x'_j))(u).(i(x''_j))(v)
$$
được thỏa mãn. Đặc biệt, với mọi phần tử *nguyên thủy* của một đại đại số phân bậc $ E $, tức là phần tử thỏa mãn $ c(x) = x \otimes 1 + 1 \otimes x $, $ i(x) $ là một *đạo hàm* của $ E^{*gr} $.

#### Mệnh đề 10 {#alg-iii-s11-prop-10 .statement}

*Một đại đại số phân bậc $ E $ (tương ứng, đại đại số phân bậc lệch). Với mọi phần tử $ f $ bậc 1 của $ E^{*gr} $, các tích vô hướng nội trái và phải là các đạo hàm (tương ứng, phản đạo hàm) của đại số $ E $.*

Cho $ x \in E_p, y \in E_q $ ($ p \geq 1, q \geq 1 $). Theo Mệnh đề 5 của No. 3, ta có thể viết
$$
c(x) = x \otimes 1 + \sum_{1 \leq j \leq p-1} \left( \sum_i x'_{ij} \otimes x''_{ij,p-j} \right) + 1 \otimes x
$$
$$
c(y) = y \otimes 1 + \sum_{1 \leq k \leq q-1} \left( \sum_i y'_{i,k} \otimes y''_{i,q-k} \right) + 1 \otimes y
$$

trong đó $ x'_{ij} $ và $ x''_{ij} $ thuộc $ E_j $, $ y'_{ik} $ và $ y''_{ik} $ thuộc $ E_k $. Nếu $ E $ là một đại số bigradu phân bậc, thành phần của $ c(xy) = c(x)c(y) $ thuộc $ E_1 \otimes E $, bằng
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
và do đó theo định nghĩa
$$
(xy) \leftarrow f = \sum_i f(x'_{i,1})x''_{i,p-1}y + \sum_i f(y'_{i,1})xy''_{i,q-1}
$$
$$
= (x \leftarrow f)y + x(y \leftarrow f)
$$
và tích trong phải bởi $ f $ là một *đạo hàm*. Mặt khác, nếu $ E $ là một đại số bigradu xiên, thành phần của $ c(xy) $ thuộc $ E_1 \otimes E $ bằng
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + (-1)^p \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
và lần này ta thu được
$$
(xy) \leftarrow f = (x \leftarrow f)y + (-1)^p x(y \leftarrow f)
$$
điều này chỉ ra rằng $ i(f) $ khi đó là một *phản đạo hàm*. Lập luận tương tự đối với tích trong trái bởi $ f $.

#### Ví dụ {#alg-iii-s11-n8-exa-1 .statement}

Các Mệnh đề 9 và 10 áp dụng đặc biệt cho đại số bigradu $ S(M) $ và đại số bigradu xiên $ \Lambda(M) $. Các tích trong bởi các phần tử bậc 1 trong $ S(M) $ (tương ứng $ S(M)^{*gr} $) là các *đạo hàm* *giao hoán với nhau*, vì $ S(M) $ (tương ứng $ S(M)^{*gr} $) là giao hoán.

Tương tự, các tích trong bởi các phần tử bậc 1 trong $ \Lambda(M) $ (tương ứng $ \Lambda(M)^{*gr} $) là các *phản đạo hàm*, có *bình phương không*, vì bình phương của một phần tử bậc 1 trong đại số $ \Lambda(M) $ (tương ứng $ \Lambda(M)^{*gr} $) bằng không.

### 9. CÁC TÍCH TRONG GIỮA $ T(M) $ VÀ $ T(M^*) $, $ S(M) $ VÀ $ S(M^*) $, $ \Lambda(M) $ VÀ $ \Lambda(M^*) $

Tích trong phải xác định trên $ T(M) $ (tương ứng $ S(M) $, tương ứng $ \Lambda(M) $) một cấu trúc môđun phải trên đại số $ T(M)^{*gr} $ (tương ứng $ S(M)^{*gr} $, tương ứng $ \Lambda(M)^{*gr} $) (no. 7, *Ví dụ*). Sử dụng các đồng cấu chính tắc $ \theta_T $ (tương ứng $ \theta_S $, tương ứng $ \theta_\Lambda $) của no. 5, ta suy ra
một cấu trúc môđun phải $ T(M^*) $ trên $ T(M) $
một cấu trúc môđun phải $ S(M^*) $ trên $ S(M) $
một cấu trúc môđun trái $ \Lambda(M^*) $ trên $ \Lambda(M) $.

Phép toán ngoài của bất kỳ cấu trúc nào trong các cấu trúc này cũng được ký hiệu bởi
$$
(z^*, t) \mapsto i(z^*) \cdot t
$$

(do cách dùng ngôn ngữ không chặt chẽ); ta cũng viết $ t \prec z^* $ thay cho $ i(z^*) . t $ trong trường hợp $ T(M) $ hoặc $ S(M) $; mặt khác, ta viết $ z^* \prec t $ trong trường hợp $ \Lambda(M) $ và nói rằng đây là một tích vô hướng *trái* của $ t $ bởi $ z^* $, vì khi đó ta có một luật môđun $ \Lambda(M^*) $ *trái*. Với $ z^* $ thuần nhất bậc $ n $ và $ t $ thuần nhất bậc $ p $, $ i(z^*) . t = 0 $ nếu $ p < n $ và, với $ x_i \in M $ ($ 1 \leq i \leq p $), $ x_j^* \in M^* $ ($ 1 \leq j \leq n $) và $ p \geq n $, theo các công thức (58), (59) và (60) của no. 7,

$$
(66)\quad i(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) . (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$
$$
= \left( \prod_{j=1}^n \langle x_j^*, x_j \rangle \right) x_{n+1} \otimes \cdots \otimes x_p
$$

$$
(67)\quad i(x_1^* x_2^* \ldots x_n^*) . (x_1 x_2 \ldots x_p) = \sum_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
$$

$$
(68)\quad i(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) . (x_1 \wedge x_2 \wedge \cdots \wedge x_p)
$$
$$
= (-1)^{n(n-1)/2} \sum_\sigma \varepsilon_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}
$$

trong các công thức (67) và (68), $ \sigma $ chạy qua tập hợp các hoán vị $ \sigma \in \mathfrak{S}_p $ tăng trên các khoảng $ \{1, n\} $ và $ \{n + 1, p\} $.

Ta cũng có thể viết, theo ký hiệu tích vô hướng,

$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_T(u^* v^*) \rangle \quad \text{với } t \in T(M), u^*, v^* \text{ trong } T(M^*)
$$
$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_S(u^* v^*) \rangle \quad \text{với } t \in S(M), u^*, v^* \text{ trong } S(M^*)
$$
$$
\langle v^*, u^* \prec t \rangle = \langle \theta_\Lambda(u^* \wedge v^*), t \rangle \text{ với } t \in \Lambda(M), u^*, v^* \text{ trong } \Lambda(M^*).
$$

Ta để người đọc tự tìm một cách tường minh các công thức tương tự cho các tích vô hướng trái, lần này sử dụng các công thức (61), (62) và (63).

Những điều trên có thể được áp dụng khi thay $ M $ bằng đối ngẫu của nó $ M^* $; khi đó $ M^* $ phải được thay bằng đối đối ngẫu $ M^{**} $ và chẳng hạn $ T(M^*) $ có một cấu trúc môđun phải trên đại số $ T(M^{**}) $. Nhưng ánh xạ chính tắc $ c_M : M \to M^{**} $ xác định một đồng cấu đại số $ T(c_M) : T(M) \to T(M^{**}) $, nhờ đó $ T(M^*) $ có một cấu trúc môđun *phải* $ T(M) $-*môđun*. Tương tự, $ S(M^*) $ (resp. $ \Lambda(M^*) $) có một cấu trúc *phải* $ S(M) $-*môđun* (resp. *trái* $ \Lambda(M) $-*môđun*). Các công thức tường minh cho các luật ngoài của các môđun này được dẫn xuất ngay lập tức từ những điều trên bằng cách hoán đổi vai trò của $ M $ và $ M^* $. Chú ý rằng, với mọi $ x \in M $, $ i(x) $ luôn là một *đạo hàm* (resp. *phản đạo hàm bình phương không*) của đại số phân bậc $ S(M^*) $ (resp. $ \Lambda(M^*) $).

#### Mệnh đề 11 {#alg-iii-s11-prop-11 .statement}

*Đồng cấu chính tắc* $ \theta_T : T(M^*) \to T(M)^{*gr} $ (resp. $ \theta_S : S(M) \to S(M)^{*gr} $, resp. $ \theta_\Lambda : \Lambda(M^*) \to \Lambda(M)^{*gr} $) *là một đồng cấu* $ T(M) $-*môđun phải* (resp. *$ S(M) $-môđun phải*, resp. *$ \Lambda(M) $-môđun trái*).

Trước hết ta chứng minh rằng, với $ z^* \in T(M^*) $ và $ t \in T(M) $,

$$
\theta_T(z^* \wedge t) = \theta_T(z^*) \wedge t.
$$

Vì $ M $ là một hệ sinh của đại số $ T(M) $, ta chỉ cần chứng minh (69) khi $ t = x \in M $; hơn nữa ta có thể hạn chế sự chú ý vào trường hợp $ z^* = x_1^* \otimes x_2^* \otimes \cdots \otimes x_p^* $, trong đó $ x_j^* \in M^* $, và khi đó, theo (66) với vai trò của $ M $ và $ M^* $ được hoán đổi cho nhau, $ z^* \wedge x = \langle x, x_1^* \rangle x_2^* \otimes \cdots \otimes x_p^* $. Do đó, với mọi $ y_2, \ldots, y_p $ trong $ M $,

$$
\begin{align*}
\langle \theta_T(z^* \wedge x), y_2 \otimes y_3 \otimes \cdots \otimes y_p \rangle &= \langle x, x_1^* \rangle \prod_{j=2}^p \langle y_j, x_j^* \rangle \\
&= \langle \theta_T(z^*), x \otimes y_2 \otimes \cdots \otimes y_p \rangle \\
&= \langle \theta_T(z^*) \wedge x, y_2 \otimes \cdots \otimes y_p \rangle
\end{align*}
$$

do đó có (69).

Ta chứng minh thứ hai rằng với $ z^* \in S(M^*) $ và $ t \in S(M) $,

$$
\theta_S(z^* \wedge t) = \theta_S(z^*) \wedge t.
$$

Như trên, ta có thể giới hạn vào trường hợp $ t = x \in M $. Nhưng hơn nữa, ở đây $ i(x) $ là một đạo hàm của $ S(M^*) $ và một đạo hàm của $ S(M)^{*gr} $. Do đó (\S 10, no. 7, Hệ quả của Mệnh đề 9) chỉ cần kiểm tra (70) đối với $ z^* = x^* \in M^* $, vì $ M^* $ là một hệ sinh của $ S(M^*) $; nhưng điều này là tầm thường, vì khi đó hai vế đều bằng $ \langle x^*, x \rangle $. Một lập luận tương tự chứng minh quan hệ

$$
\theta_\wedge(t \wedge z^*) = t \wedge \theta_\wedge(z^*)
$$

với $ z^* \in \Lambda(M^*) $ và $ t \in \Lambda(M) $: khi đó, lưu ý rằng với $ x \in M $, $ i(x) $ là một đạo hàm phản xứng trong $ \Lambda(M^*) $ cũng như trong $ \Lambda(M)^{*gr} $ và áp dụng \S 10, no. 7, Hệ quả của Mệnh đề 9. Có một kết quả tương tự đối với các tích nội trái.

### 10. DẠNG TƯỜNG MINH CỦA CÁC TÍCH NỘI TRONG TRƯỜNG HỢP MỘT MÔĐUN TỰ DO SINH HỮU HẠN

Cho $ M $ là một $ A $-môđun tự do sinh hữu hạn, $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của $ M $ và $ (e_i^*)_{1 \leq i \leq n} $ là cơ sở đối ngẫu của $ M^* $. Với mỗi dãy hữu hạn $ s = (i_1, \ldots, i_p) $ gồm các phần tử của $ \{1, n\} $, đặt $ e_s = e_{i_1} \otimes e_{i_2} \otimes \cdots \otimes e_{i_p} $ (resp. $ e_s^* = e_{i_1}^* \otimes \cdots \otimes e_{i_p}^* $). Ta biết (\S 5, no. 5, Định lý 1) rằng các $ e_s $ lập thành một cơ sở của $ A $-môđun $ T(M) $ và các $ e_s^* $ một cơ sở của $ A $-môđun $ T(M^*) $. Nếu $ s, t $ là hai dãy hữu hạn gồm các phần tử của $ \{1, n\} $, ký hiệu $ s.t $ là dãy thu được như sau: nếu $ s = (i_1, \ldots, i_p) $ và $ t = (j_1, \ldots, j_q) $, thì $ s.t $ là dãy $ (i_1, \ldots, i_p, j_1, \ldots, j_q) $ có $ p + q $ số hạng. Khi đó $ e_{s.t} = e_s \otimes e_t $. Từ (66) suy ra rằng

$$
\begin{cases}
e_s \wedge e_t^* = 0 & \text{nếu } s \text{ không có dạng } t.u \\
e_{t.u} \wedge e_t^* = e_u.
\end{cases}
$$

Tương tự, đại số đối xứng $ S(M) $ có cơ sở là tập hợp các đơn thức $ e^\alpha $ với $ \alpha \in \mathbf{N}^n $ (\S 6, no. 6, Định lý 1) và $ S(M^*) $ là tập hợp các đơn thức $ e^{*\alpha} $ với $ \alpha \in \mathbf{N}^n $; nhắc lại (no. 5) rằng $ u_\alpha $, với $ |\alpha| = k $, ký hiệu phần tử của cơ sở của $ (S^k(M))^* $, đối ngẫu với cơ sở $ (e^\alpha)_{|\alpha|=k} $ của $ S^k(M) $; do đó các $ u_\alpha $, với $ \alpha \in \mathbf{N}^n $, lập thành một cơ sở của $ S(M)^{*gr} $. Định nghĩa tích nội phải bởi $ e^\beta $ trong $ S(M)^{*gr} $ là chuyển vị của phép nhân bởi $ e^\beta $ trong $ S(M) $ khi đó cho thấy rằng

$$
\begin{cases}
u_\alpha \perp e^\beta = 0 & \text{nếu } \alpha \not\geq \beta \\
u_\alpha \perp e^\beta = u_{\alpha-\beta} & \text{nếu } \alpha \geq \beta.
\end{cases}
$$

(73)

Tương tự, vì $ S(M) $ ở đây được đồng nhất một cách chính tắc với đối ngẫu phân bậc của $ S(M)^{*gr} $, $ i(u_\beta) $ là chuyển vị phân bậc của phép nhân bởi $ u^\beta $ trong $ S(M)^{*gr} $ và do đó từ bảng phép nhân (33) (no. 5) của cơ sở $ (u_\alpha) $ ta suy ra rằng

$$
\begin{cases}
e^\alpha \perp u_\beta = 0 & \text{nếu } \alpha \not\geq \beta \\
e^\alpha \perp u_\beta = (\beta, \alpha - \beta)e^{\alpha-\beta} & \text{nếu } \alpha \geq \beta.
\end{cases}
$$

(74)

Đối với tích nội phải của một phần tử của $ S(M) $ bởi một phần tử của $ S(M^*) $, định nghĩa của tích này (no. 9) và công thức (34) của no. 5 cho phép ta suy ra từ (74) các công thức

$$
\begin{cases}
e^\alpha \perp e^{*\beta} = 0 & \text{nếu } \alpha \not\geq \beta \\
e^\alpha \perp e^{*\beta} = \frac{\alpha!}{(\alpha-\beta)!} e^{\alpha-\beta} & \text{nếu } \alpha \geq \beta.
\end{cases}
$$

(75)

Có các công thức tương tự cho tích nội của một phần tử của $ S(M^*) $ bởi một phần tử của $ S(M) $ bằng cách đổi chỗ vai trò của $ M $ và $ M^* $ (vì $ M^{**} $ ở đây được đồng nhất với $ M $).

#### Nhận xét {#alg-iii-s11-n10-rem-1 .statement}

Việc cho cơ sở $ (e_i)_{1 \leq i \leq n} $ cho phép ta đồng nhất đại số $ S(M) $ với đại số đa thức $ A[X_1, \ldots, X_n] $ (\S 6, no. 6); công thức (75) cho thấy rằng tích nội bởi $ e^{*\alpha} $ chính là toán tử vi phân $ D^\alpha = D_1^{\alpha_1}D_2^{\alpha_2}\ldots D_n^{\alpha_n} $, trong đó $ D_i = \partial/\partial X_i $ với $ 1 \leq i \leq n $ (\S 10, no. 11, Ví dụ).

Xét cuối cùng đại số ngoài $ \Lambda(M) $, có cơ sở là tập hợp các phần tử $ e_J $, trong đó $ J $ chạy qua tập hợp các tập con của khoảng $ \{1, n\} $ của $ \mathbf{N} $ (\S 7, no. 8, Định lý 1); tương tự $ \Lambda(M^*) $ có cơ sở là các phần tử $ e_J^* $. Từ công thức (68) của no. 9 suy ra rằng

$$
\begin{cases}
e_K^* \wedge e_J = 0 & \text{nếu } K \notin J \\
e_K^* \wedge e_J = (-1)^{p(p-1)/2} \rho_{K, J-K} e_{J-K} & \text{nếu } K \subset J \text{ và } p = \operatorname{Card}(K),
\end{cases}
$$

(76)

trong đó $ \rho_{K, J-K} $ là số được định nghĩa bởi công thức (19) của \S 7, no. 8. Có các công thức tương tự với vai trò của $ M $ và $ M^* $ được đổi chỗ.

### 11. CÁC ĐẲNG CẤU GIỮA $ \wedge^p(M) $ VÀ $ \wedge^{n-p}(M^*) $ CHO MỘT MÔĐUN TỰ DO CHIỀU $ n $

#### Mệnh đề 12 {#alg-iii-s11-prop-12 .statement}

*Cho M là một A-môđun tự do có chiều n; cho $ e \in \wedge^n(M) $ là một phần tử tạo thành một cơ sở của $ \wedge^n(M) $ và cho $ e^* $ là phần tử của $ \wedge^n(M^*) $ sao cho $ \{(-1)^{n(n-1)/2} \theta_{\wedge}(e^*)\} $ là cơ sở đối ngẫu của $ \{e\} $ trong $ (\wedge^n(M))^* $. Cho $ \phi : \wedge(M^*) \to \wedge(M) $ là ánh xạ $ z \mapsto z \wedge e^* $ và $ \phi' : \wedge(M^*) \to \wedge(M) $ là ánh xạ $ z^* \mapsto z^* \wedge e $. Cho $ \phi_p $ (resp. $ \phi'_p $) là hạn chế của $ \phi $ (resp. $ \phi' $) vào $ \wedge^p(M) $ (resp. $ \wedge^p(M^*) $). Khi đó:

(i) *Ánh xạ $ \phi $ là một đẳng cấu $ \wedge(M) $-môđun trái và ánh xạ $ \phi' $ là một đẳng cấu $ \wedge(M^*) $-môđun trái; hơn nữa các ánh xạ $ \phi $ và $ \phi' $ là nghịch đảo của nhau.*

(ii) *Ánh xạ $ \phi_p $ là một đẳng cấu của A-môđun $ \wedge^p(M) $ lên A-môđun $ \wedge^{n-p}(M^*) $ và ánh xạ $ \phi'_p $ là một đẳng cấu của A-môđun $ \wedge^p(M^*) $ lên A-môđun $ \wedge^{n-p}(M) $.

(iii) *Nếu ta viết $ B(u, v^*) = \langle u, \theta_{\wedge}(v^*) \rangle $ với $ u \in \wedge(M) $ và $ v^* \in \wedge(M^*) $ thì, với $ u^* \in \wedge^p(M^*) $ và $ v^* \in \wedge^{n-p}(M^*) $,

$$
B(\phi'_p(u^*), v^*) = (-1)^{p(n-p)} B(u^*, \phi'_{n-p}(v^*)).
$$

Tính $ \wedge(M) $-tuyến tính của $ \phi $ và tính $ \wedge(M^*) $-tuyến tính của $ \phi' $ suy ra từ các công thức $ (u \wedge v) \wedge e^* = u \wedge (v \wedge e^*) $ và $ (u^* \wedge v^*) \wedge e = u^* \wedge (v^* \wedge e) $ (no. 6, công thức (37)), sử dụng tính chất $ \theta_{\wedge} $ là một đẳng cấu từ $ \wedge(M^*) $ lên đại số đối của $ \wedge(M)^* $. Mặt khác tồn tại một cơ sở $ (e_i)_{1 \leq i \leq n} $ của M sao cho

$$
e = e_1 \wedge e_2 \wedge \cdots \wedge e_n \quad \text{và} \quad e^* = (-1)^{n(n-1)/2} e_1^* \wedge e_2^* \wedge \cdots \wedge e_n^*,
$$

trong đó $ (e_i^*) $ là cơ sở đối ngẫu của $ (e_i) $. Ta viết $ I = \{1, n\} $; suy ra từ (76) rằng, với mọi tập con J của I có p phần tử,

$$
\begin{cases}
\phi(e_J) = (-1)^{n(n-1)/2 + p(p-1)/2} \rho_{J, I-J} e_I^* J \\
\phi'(e_J^*) = (-1)^{p(p-1)/2} \rho_{J, I-J} e_{I-J}.
\end{cases}
$$

Điều này chứng minh rằng $ \phi $ và $ \phi' $ là song ánh; hơn nữa $ \rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)} $ (\S 7, no. 8, công thức (21)); vì số

$$
\frac{n(n-1)}{2} + \frac{p(p-1)}{2} + \frac{(n-p)(n-p-1)}{2} + p(n-p) = n(n-1)
$$

là chẵn, suy ra $ \phi $ và $ \phi' $ là các ánh xạ ngược của nhau. Cuối cùng, để chứng minh (77), chỉ cần lấy $ u^* = e_J^* $ và $ v^* = e_{I-J}^* $; việc kiểm tra cũng suy ra từ định nghĩa của $ \theta_{\wedge} $, các công thức (78) và quan hệ $ \rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)} $ (\S 7, no. 8, công thức (21)). Chú ý rằng, với $ u^* \in \wedge^p(M^*) $ và $ v^* \in \wedge^{n-p}(M^*) $,

B(\phi_p'(u^*), v^*) là, sai khác một dấu, hệ số của $ u^* \wedge v^* $ đối với cơ sở $ \{e^*\} $ của $ \Lambda^n(M^*) $.

#### Mệnh đề 13 {#alg-iii-s11-prop-13 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 11, với mọi tự đồng cấu g của A-môđun M.*

$$(79)$$
$$(\det g)\phi = \Lambda^{(tg)} \circ \phi \circ \Lambda(g).$$

Rõ ràng $ \Lambda^{(tg)} = \theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda} $; vì $ \Lambda(g) $ là một tự đồng cấu của đại số $ \Lambda(M) $ và theo định nghĩa, với mọi
$$z \in \Lambda(M), \quad \theta_{\Lambda}(\Lambda(g)(z) \perp e^*) = \theta_{\Lambda}(e^*) \perp \theta_{\Lambda}(\Lambda(g)(z)),$$
suy ra từ công thức (42) của no. 6 rằng
$$
((\theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}) \circ \phi \circ \Lambda(g))(z) = \theta_{\Lambda}^{-1}(t\Lambda(g)(\theta_{\Lambda}(e^*)) \perp z)
= z \perp (\Lambda^{(tg)}(e^*)) = (\det g)(z \perp e^*) = (\det g)\phi(z)
$$
có tính đến § 8, no. 4, Mệnh đề 8.

#### Hệ quả {#alg-iii-s11-n11-cor-1 .statement}

*Với mọi tự đẳng cấu g của E,*
$$(80)$$
$$\Lambda^{(tg^{-1})} = (\det g)^{-1}\phi \circ (\Lambda(g)) \circ \phi^{-1}.$$

### 12. ÁP DỤNG CHO KHÔNG GIAN CON LIÊN KẾT VỚI MỘT p-VECTƠ

Cho K là một trường và E là một không gian vectơ trên K. Nhắc lại rằng với mỗi $ p $-vectơ $ z \in \Lambda^p(E) $ có liên kết một không gian con hữu hạn chiều $ M_z $ của E, cụ thể là không gian con vectơ nhỏ nhất M của E sao cho $ z \in \Lambda^p(M) $ (§ 7, no. 2, Hệ quả của Mệnh đề 4).

#### Mệnh đề 14 {#alg-iii-s11-prop-14 .statement}

(i) *Không gian trực giao của $ M_z $ trong $ E^* $ là tập hợp các $ x^* \in E^* $ sao cho $ x^* \perp z = 0 $.*

(ii) *Không gian con $ M_z $ liên kết với z là ảnh của $ \Lambda^{p-1}(E^*) $ qua ánh xạ $ \lambda_z : u^* \mapsto u^* \perp z $ từ $ \Lambda^{p-1}(E^*) $ vào E.*

Ký hiệu N là ảnh của $ \lambda_z $. Với $ x^* \in E^* $ và $ u^* \in \Lambda^{p-1}(E^*) $,
$$
\langle \theta_{\Lambda}(x^*), u^* \perp z \rangle = \langle \theta_{\Lambda}(u^* \wedge x^*), z \rangle = (-1)^{p-1} \langle \theta_{\Lambda}(x^* \wedge u^*), z \rangle \\
= (-1)^{p-1} \langle \theta_{\Lambda}(u^*), x^* \perp z \rangle.
$$
Do đó, để $ x^* $ trực giao với N, điều kiện cần và đủ là $ x^* \perp z $ trực giao với $ \theta_{\Lambda}(\Lambda(E^*)) $. Bây giờ, điều kiện sau tương đương với việc nói rằng $ x^* \perp z = 0 $; thật vậy, cho $ (e_{\lambda})_{\lambda \in L} $ là một cơ sở của E; trang bị cho L một thứ tự toàn phần, đã thấy (§ 7, no. 8, Định lý 1) rằng các $ e_J $, với J chạy qua tập $ \mathcal{F}(L) $ các tập con hữu hạn của L, lập thành một cơ sở của $ \Lambda(E) $; từ đó suy ra từ công thức (30) của no. 5 rằng các phần tử $ \theta_{\wedge}(e_J^*) $ là, sai khác một dấu, các dạng tọa độ trên $ \wedge(E) $ đối với cơ sở $ (e_J) $; do đó có mệnh đề của ta.

Không gian trực giao của N do đó gồm các $ x^* \in E^* $ sao cho $ x^* \perp z = 0 $ và do đó kết luận của (i) sẽ suy ra từ (ii).

Trước hết ta chứng minh rằng $ N \subset M_z $. Cho M là một không gian con vectơ của E sao cho $ z \in \wedge(M) $ và cho $ j : M \to E $ là đơn ánh chính tắc; ký hiệu $ \mu_z $ là ánh xạ $ v^* \mapsto v^* \perp z $ từ $ \wedge^{p-1}(M^*) $ vào M; từ công thức (60) của no. 7 suy ra rằng có một phân tích chính tắc

$$
\lambda_z : \wedge^{p-1}(E^*) \xrightarrow{\wedge^{p-1}(t_j)} \wedge^{p-1}(M^*) \xrightarrow{\mu_z} M \xrightarrow{j} E
$$

điều này chứng tỏ rằng $ N \subset M $ và do đó $ N \subset M_z $ theo định nghĩa của $ M_z $. Còn phải chứng minh rằng $ N = M_z $. Giả sử điều ngược lại: khi đó tồn tại một cơ sở $ (e_i)_{1 \leq i \leq n} $ của $ M_z $ và một phần tử $ x^* \in E^* $ sao cho $ \langle x^*, e_1 \rangle = 1, \langle x^*, e_j \rangle = 0 $ với $ 2 \leq j \leq n $ và sao cho $ x^* $ trực giao với N, do đó $ x^* \perp z = 0 $. Ta viết $ z = \sum_H a_H e_H $, trong đó tổng được lấy trên các tập con của $ \{1, n\} $ có $ p $ phần tử. Theo (68) (no. 9),

$$
x^* \perp e_H = 0 \quad \text{nếu } 1 \notin H \\
x^* \perp e_{\{1\} \cup H} = e_H \quad \text{nếu } H \subset \{2, n\}
$$

điều này cho thấy rằng quan hệ $ x^* \perp z = 0 $ kéo theo $ a_H = 0 $ với $ 1 \in H $. Nhưng điều này là không thể, vì khi đó $ z $ thuộc $ \wedge^p(M') $, trong đó $ M' $ là không gian con của M sinh bởi $ e_2, \ldots, e_n $.

### 13. CÁC $ p $-VECTƠ THUẦN. GRASSMANNIAN

Cho K là một trường và E là một không gian vectơ trên K. Một $ p $-vectơ $ z \in \wedge^p(E) $ được gọi là *thuần* (hay đôi khi là *phân tích được*) nếu nó khác không và tồn tại các vectơ $ x_1, \ldots, x_p $ trong E sao cho $ z = x_1 \wedge x_2 \wedge \cdots \wedge x_p $. Để được như vậy, điều kiện cần và đủ là không gian con $ M_z $ liên kết với $ z $ (luôn có chiều $ \geq p $ khi $ z \neq 0 $) phải có chiều *đúng bằng* $ p $ (vì khi đó $ \wedge^p(M_z) $ có chiều 1). Đặc biệt, mọi vô hướng *khác không*, mọi phần tử khác không của $ E = \wedge^1(E) $, mọi phần tử khác không của $ \wedge^n(E) $, khi E có chiều $ n $, đều là *thuần*.

#### Mệnh đề 15 {#alg-iii-s11-prop-15 .statement}

*Cho E là một không gian vectơ có chiều n và e là một phần tử $ \neq 0 $ của $ \wedge^n(E) $ (do đó tạo thành một cơ sở của không gian vectơ này). Gọi $ \phi : \wedge(E) \to \wedge(E^*) $ là đẳng cấu không gian vectơ liên kết với e (no. 11, Mệnh đề 12). Nếu z là một phần tử thuần của $ \wedge^p(E) $, thì $ \phi(z) $ là một phần tử thuần của $ \wedge^{n-p}(E^*) $ và các không gian con liên kết với z và $ \phi(z) $ trực giao.*

Các trường hợp $ p = 0 $ và $ p = n $ là tầm thường. Vì vậy, giả sử $ 1 \leq p \leq n - 1 $ và đặt $ z = x_1 \wedge \cdots \wedge x_p \neq 0 $. Khi đó tồn tại một cơ sở $ (e_i)_{1 \leq i \leq n} $ của E sao cho $ e_i = x_i $ với $ 1 \leq i \leq p $ và $ e = e_1 \wedge e_2 \wedge \cdots \wedge e_n $. Do đó, từ công thức (78) của no. 11 suy ra $ \phi(z) = \pm e_{p+1}^* \wedge \cdots \wedge e_n^* $, và do đó có mệnh đề.

#### Hệ quả {#alg-iii-s11-n13-cor-1 .statement}

*Nếu E có chiều n, mọi $(n-1)$-vectơ khác không E đều thuần.*

#### Mệnh đề 16 {#alg-iii-s11-prop-16 .statement}

*Một phần tử $ z \neq 0 $ của $ \bigwedge^p(E) $ là thuần khi và chỉ khi, với mọi $ u^* \in \bigwedge^{p-1}(E^*) $,

$$
(u^* \perp z) \wedge z = 0.
$$

Trường hợp $ p = 0 $ là tầm thường và ta giả sử $ p \geq 1 $. Nếu $ z = x_1 \wedge \cdots \wedge x_p $, công thức (68) (no. 9) với $ n = p - 1 $ cho thấy rằng $ u^* \perp z $ là một tổ hợp tuyến tính của các $ x_i $ ($ 1 \leq i \leq p $), do đó (81). Ngược lại, nếu không gian con $ M_z $ liên kết với $ z $ có chiều $ > p $, xét một cơ sở $ (e_j)_{1 \leq j \leq n} $ của không gian con này với $ n > p $. Theo no. 11, Mệnh đề 13, mỗi $ e_j $ có dạng $ u^* \perp z $ với một $ u^* \in \bigwedge^{p-1}(E^*) $ nào đó và quan hệ (81) do đó kéo theo $ e_j \wedge z = 0 $ với $ 1 \leq j \leq n $. Suy ra trong biểu thức $ z = \sum_H a_H e_H $ (trong đó H chạy qua tập hợp các tập con của $ \{1, n\} $ có $ p $ phần tử) tất cả các hệ số $ a_H $ đều bằng không, do đó $ z = 0 $, trái với giả thiết.

Tiêu chuẩn của Mệnh đề 16 tương đương với việc viết các điều kiện (81) khi $ u^* $ chạy qua một *cơ sở* của $ \bigwedge^{p-1}(E^*) $. Đặc biệt, giả sử E có số chiều hữu hạn $ n $ và cho $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của E. Khi đó các điều kiện (81) tương đương với các điều kiện

$$(82-(J, H))$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge z \rangle = 0
$$
với mọi tập con J, H của $ \{1, n\} $ sao cho $ \mathrm{Card}(J) = p + 1 $ và $ \mathrm{Card}(H) = p - 1 $. Bây giờ, nếu I và I' là hai tập con của $ \{1, n\} $ có $ p $ phần tử, các công thức (76) của no. 10 và bảng phép nhân (20) của § 7, no. 8 cho thấy rằng

$$
\langle e_J^*, \langle e_H^* \perp e_I \rangle \wedge e_{I'} \rangle = 0
$$
*trừ khi* tồn tại một $ i \in \{1, n\} $ sao cho $ I - H = \{i\} $ và $ J - I' = \{i\} $, trong trường hợp đó

$$(83)$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = (-1)^{(p-1)(p-2)/2} \varepsilon_{i, J, H}
$$
trong đó $ \varepsilon_{i, J, H} = \rho_{\{i\}, H} \rho_{\{i\}, I'} $; khi đó có thể nói rằng với $ i \in J \cap C H $, $ \varepsilon_{i, J, H} $ bằng $ +1 $ nếu số phần tử của J nhỏ hơn $ < i $ và số phần tử của H nhỏ hơn $ < i $ có *cùng tính chẵn lẻ*, và bằng $ -1 $ trong trường hợp ngược lại.

Suy ra ngay lập tức rằng nếu ta viết $ z = \sum_I a_I e_I $, trong đó I chạy qua tập hợp các tập con của $ \{1, n\} $ có $ p $ phần tử, thì quan hệ (82–(J, H)) tương đương với quan hệ

$$
\sum_{i \in J \cup C_H} \varepsilon_{i, J, H} a_{J-\{i\}} a_{H \cup \{i\}} = 0.
$$

Các quan hệ (84) được gọi là *các quan hệ Grassman*; do đó, đây là các điều kiện cần và đủ (khi J mô tả tập hợp các tập con có $ p + 1 $ phần tử và H mô tả tập hợp các tập con có $ p - 1 $ phần tử của $ \{1, n\} $) để một phần tử $ z \neq 0 $ của $ \bigwedge^p(E) $ là *thuần túy*.

Lưu ý rằng các quan hệ (84) không độc lập. Chẳng hạn, với $ n = 4 $ và $ p = 2 $, các quan hệ Grassmann rút gọn thành quan hệ duy nhất

$$
a_{12} a_{34} - a_{13} a_{24} + a_{14} a_{23} = 0.
$$

Cho $ D_p(E) $ là tập con của $ \bigwedge^p(E) $ gồm các $ p $-vectơ *thuần*; rõ ràng $ D_p(E) $ bão hòa đối với quan hệ tương đương giữa $ u $ và $ v $: “tồn tại $ \lambda \in K^* $ sao cho $ v = \lambda u $” và hai phần tử $ u, v $ của $ D_p(E) $ là tương đương theo quan hệ này khi và chỉ khi các không gian con $ M_u $ và $ M_v $ của E liên kết với chúng là như nhau. Do đó, ta thu được một *song ánh chính tắc* của *tập hợp các không gian con vectơ p chiều* của E lên *ảnh* $ G_p(E) $ của $ D_p(E) $ *trong không gian xạ ảnh* $ \mathbf{P}(\bigwedge^p(E)) $ liên kết với $ \bigwedge^p(E) $. Tập con $ G_p(E) $ của $ \mathbf{P}(\bigwedge^p(E)) $ được gọi là *đa tạp Grassmann* có chỉ số $ p $ của không gian vectơ E. Khi E hữu hạn chiều và $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của E, đa tạp Grassmann có chỉ số $ p $ là tập hợp các điểm của $ \mathbf{P}(\bigwedge^p(E)) $ mà một hệ tọa độ thuần nhất $ (a_I) $ (đối với cơ sở $ (e_I) $ của $ \bigwedge^p(E) $) thỏa mãn các hệ thức Grassmann (84).

Khi $ E = K^n $, đôi khi ta viết $ G_{n,p}(K) $ thay cho $ G_p(K^n) $, sao cho $ G_{n,1}(K) = P_{n-1}(K) $. Ánh xạ $ M \mapsto M^0 $, liên kết với mỗi không gian con $ p $ chiều của $ K^n $ không gian con *trực giao* trong $ E^* $ (được đồng nhất với $ K^n $ theo lựa chọn cơ sở đối ngẫu với cơ sở chính tắc của $ K^n $), do đó xác định một *song ánh* chính tắc của $ G_{n,p}(K) $ lên $ G_{n,n-p}(K) $; Mệnh đề 15 chỉ ra rằng song ánh này là *hạn chế* của $ G_{n,p}(K) $ của một *đẳng cấu* chính tắc của không gian xạ ảnh $ \mathbf{P}(\bigwedge^p(K^n)) $ lên không gian xạ ảnh $ \mathbf{P}(\bigwedge^{n-p}(K^n)) $.

### Bài tập {#alg-iii-s11-exercises}

Xem [các bài tập của § 11](exercises/s11/).
