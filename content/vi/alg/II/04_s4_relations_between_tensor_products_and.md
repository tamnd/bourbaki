---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 4
section_title: Relations between tensor products and homomorphism modules
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0291-0300, 0420-0422
extraction: ocr
subsections:
    - "no": 1
      title: THE ISOMORPHISMS $ \operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $ AND $ \operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G)) $
      page: 0
      pdf_page: 291
    - "no": 2
      title: THE HOMOMORPHISM** $ E^* \otimes_A F \to \mathrm{Hom}_A(E, F) $
      page: 0
      pdf_page: 292
    - "no": 3
      title: TRACE OF AN ENDOMORPHISM
      page: 0
      pdf_page: 297
    - "no": 4
      title: THE HOMOMORPHISM $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$
      page: 0
      pdf_page: 298
statements: 15
exercises: 9
content_sha256: c4ba6cad2bdfeb2814bf1954051cdf487507ed58c49fb930841895b9dd607bc3
translated_from: content/en/alg/II/04_s4_relations_between_tensor_products_and.md
source_content_sha256: b9c301046b44f9223afedd5ec05acb598f0ddabb1140f8edcfc362bcf970fd1d
translation_model: gpt-5-6-mini
translation_run: translate-vi-ee3a5201
glossary_version: 34
glossary_terms_sha256: db61d1b919841bcb8c317b54e539bfb79f679ea8e20a77dd8a8f6b91fdc462e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC QUAN HỆ GIỮA CÁC TÍCH TENXƠ VÀ CÁC MÔĐUN ĐỒNG CẤU

### 1. CÁC ĐẲNG CẤU $ \operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $ VÀ $ \operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G)) $

Cho E là một A-môđun phải, F là một A-môđun trái, G là một $ \mathbf{Z} $-môđun và H là $ \mathbf{Z} $-môđun các ánh xạ $ f : E \times F \to G $ song tuyến tính trên $ \mathbf{Z} $ và thỏa mãn

(1)
$$
f(x \lambda, y) = f(x, \lambda y) \quad \text{cho } x \in E, y \in F, \lambda \in A.
$$

Đã thấy (\S 3, no. 1, Mệnh đề 1) rằng tồn tại một đồng cấu $ \mathbf{Z} $-môđun chính tắc

(2)
$$
H \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G).
$$

Mặt khác, một cấu trúc A-môđun trái đã được đưa vào trên $ \operatorname{Hom}_{\mathbf{Z}}(E, G) $ và một cấu trúc A-môđun phải trên $ \operatorname{Hom}_{\mathbf{Z}}(F, G) $ (\S 3, no. 3); do đó ta có thể xét các $ \mathbf{Z} $-môđun $ \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G)) $ và $ \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)) $. Một ánh xạ $ f $ của $ E \times F $ vào G được đồng nhất một cách chính tắc với một ánh xạ của E vào tập hợp $ G^F $ các ánh xạ từ F vào G (*Lý thuyết tập hợp*, II, \S 5, no. 2); bằng cách biểu diễn sự kiện rằng ánh xạ sau thuộc về $ \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G)) $, ta thu được chính xác sự kiện rằng $ f $ là song cộng tính và các điều kiện (1); do đó có một đẳng cấu chính tắc

(3)
$$
H \to \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))
$$
và tương tự có một đẳng cấu chính tắc được xác định

(4)
$$
H \to \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)).
$$

Giả sử bây giờ rằng E và G cũng có các cấu trúc B-môđun trái (tương ứng phải) và rằng các cấu trúc A-môđun và B-môđun trên E là tương thích. Khi đó $ E \otimes_A F $ có một cấu trúc B-môđun trái (tương ứng phải) một cách chính tắc (\S 3, no. 4) và mặt khác $ \operatorname{Hom}_B(E, G) $ có một cấu trúc A-môđun trái một cách chính tắc (\S 1, no. 14). Do đó ta có thể xét các $ \mathbf{Z} $-môđun $ \operatorname{Hom}_B(E \otimes_A F, G) $ và $ \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $, lần lượt là các môđun con của $ \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G) $ và $ \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)) $ (\S 2, no. 1, Định lý 2). Ta xét điều kiện để một ánh xạ $ f \in H $ có ảnh qua các đẳng cấu (2) và (4) là một phần tử của $ \operatorname{Hom}_B(E \otimes_A F, G) $ và một phần tử của $ \operatorname{Hom}_A(E, \operatorname{Hom}_B(F, G)) $ tương ứng; trong mỗi trường hợp trong hai trường hợp ta tìm được *cùng một* điều kiện

$$
f(\beta x, y) = \beta f(x, y)
$$
(tương ứng $ f(x \beta, y) = f(x, y) \beta $)

cho $ x \in E, y \in F, \beta \in B $.

Tương tự, giả sử rằng F và G là các C-môđun trái (tương ứng phải) và rằng các cấu trúc A-môđun và C-môđun trên F là tương thích. Khi đó, để một ánh xạ $ f \in H $ có ảnh qua (2) hoặc (3) là một phần tử của $ \mathrm{Hom}_C(E \otimes_A F, G) $ hoặc $ \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)) $ tương ứng, điều kiện cần và đủ là nó thỏa mãn cùng một điều kiện

$$
f(x, \gamma y) = \gamma f(x, y)
$$
(tương ứng $ f(x, y \gamma) = f(x, y) \gamma $)

cho $ x \in E, y \in F, \gamma \in C $.

Do đó ta đã thiết lập được kết quả sau (với ký hiệu đã đưa vào ở trên):

#### Mệnh đề 1 {#alg-ii-s4-prop-1 .statement}

(a) *Cho E là một (B, A)-song môđun, F là một A-môđun trái và G là một B-môđun trái. Với mọi ánh xạ $ g \in \mathrm{Hom}_B(E \otimes_A F, G) $, gọi $ g' $ là ánh xạ từ F vào $ \mathrm{Hom}_B(E, G) $ được xác định bởi $ (g'(y))(x) = g(x \otimes y) $ với $ x \in E, y \in F $. Ánh xạ $ g \mapsto g' $ là một đẳng cấu*

(5)
$$
\beta : \mathrm{Hom}_B(E \otimes_A F, G) \to \mathrm{Hom}_A(F, \mathrm{Hom}_B(E, G)).
$$

(b) *Cho E là một A-môđun phải, F là một (A, C)-song môđun và G là một C-môđun phải. Với mọi ánh xạ $ h \in \mathrm{Hom}_C(E \otimes_A F, G) $, gọi $ h' $ là ánh xạ từ E vào $ \mathrm{Hom}_C(F, G) $ được xác định bởi $ (h'(x))(y) = h(x \otimes y) $ với $ x \in E, y \in F $. Ánh xạ $ h \mapsto h' $ là một đẳng cấu*

(6)
$$
\gamma : \mathrm{Hom}_C(E \otimes_A F, G) \to \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)).
$$

Đặc biệt B và C có thể được lấy là một vành con $ \Gamma $ của tâm của vành A; khi đó với mọi $ \Gamma $-môđun G, ba $ \Gamma $-môđun

$$
\mathrm{Hom}_\Gamma(E \otimes_A F, G), \quad \mathrm{Hom}_A(E, \mathrm{Hom}_\Gamma(F, G)), \quad \mathrm{Hom}_A(F, \mathrm{Hom}_\Gamma(E, G))
$$

Cho $ M, N $ là hai môđun con bù nhau trong $ F $ và $ i : M \to F, j : N \to F $ là các phép nhúng chính tắc. Biểu đồ

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(i) + T(j) & & \downarrow T'(i) + T'(j) \\
T(F) & \xrightarrow{\nu_F} & T'(F)
\end{array}
$$

là giao hoán và các mũi tên đứng là song ánh.

Tính giao hoán suy ra từ Bổ đề 1, các khẳng định còn lại suy ra từ § 1, no. 6, Hệ quả 2 của Mệnh đề 6 và § 3, no. 7, Mệnh đề 7.

#### Bổ đề 3 {#alg-ii-s4-lem-3 .statement}

Với các giả thiết của Bổ đề 2, để $ \nu_F $ là đơn ánh (resp. toàn ánh), điều kiện cần và đủ là $ \nu_M $ và $ \nu_N $ cũng có tính chất đó.

Điều này suy ra từ Bổ đề 2 và § 1, no. 6, Hệ quả 1 của Mệnh đề 6.

Khi đó Bổ đề 3, cùng với § 2, no. 2, Mệnh đề 4, cho thấy chỉ cần xét trường hợp $ F $ là một môđun tự do. Nhưng, nếu $ (b_\mu) $ là một cơ sở của $ F $, thì mọi phần tử của $ \mathrm{Hom}_A(E, G) \otimes_B F $ khi đó đều được viết duy nhất dưới dạng $ \sum_\mu u_\mu \otimes b_\mu $, trong đó $ u_\mu \in \mathrm{Hom}_A(E, G) $ (\S 3, no. 7, Hệ quả 1 của Mệnh đề 7); ảnh của phần tử này qua $ \nu $ là ánh xạ $ A $-tuyến tính $ x \mapsto \sum_\mu u_\mu(x) \otimes b_\mu $; nó không thể bằng không với mọi $ x \in E $ trừ khi $ u_\mu(x) = 0 $ với mọi $ x \in E $ và mọi $ \mu $, điều này tương đương với việc nói rằng $ u_\mu = 0 $ với mọi $ \mu $; do đó $ \nu $ là đơn ánh. Khi $ F $ cũng có một cơ sở hữu hạn, Bổ đề 3 cho thấy (bằng quy nạp theo số phần tử trong cơ sở của $ F $) rằng để chứng minh $ \nu $ là toàn ánh, chỉ cần làm điều đó khi $ F = B_s $; nhưng trong trường hợp này hai vế của (7) được đồng nhất một cách chính tắc với $ \mathrm{Hom}_A(E, G) $ (\S 3, no. 4, Mệnh đề 4) và $ \nu $ trở thành ánh xạ đồng nhất.

(ii) Để chứng minh mệnh đề khi $ E $ là xạ ảnh và sinh hữu hạn, lần này ta cố định $ F $ và $ G $ và viết, với mọi $ A $-môđun trái $ E $,

$$
T(E) = \mathrm{Hom}_A(E, G) \otimes_B F, \qquad T'(E) = \mathrm{Hom}_A(E, G \otimes_B F)
$$

và, với mọi đồng cấu môđun trái $ A $ $ v : E \to E' $,

$$
T(v) = \mathrm{Hom}(v, 1_G) \otimes 1_F, \qquad T'(v) = \mathrm{Hom}(v, 1_G \otimes 1_F);
$$

mặt khác, ta viết $ \nu_E $ thay cho $ \nu $. Khi đó ta có hai bổ đề sau:

#### Bổ đề 4 {#alg-ii-s4-lem-4 .statement}

Với mọi đồng cấu $ v : E \to E' $, biểu đồ

$$
\begin{array}{ccc}
T(E') & \xrightarrow{\nu_{E'}} & T'(E') \\
\downarrow T(v) & & \downarrow T'(v) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

là giao hoán.

#### Bổ đề 5 {#alg-ii-s4-lem-5 .statement}

Cho $ M $ và $ N $ là hai môđun con bù nhau trong $ E $ và $ p : E \to M, q : E \to N $ là các phép chiếu chính tắc. Biểu đồ

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(p) + T(q) & & \downarrow T'(p) + T'(q) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

là giao hoán và các mũi tên đứng là song ánh.

Chúng được chứng minh như các Bổ đề 1 và 2, có tính đến § 1, no. 6, Hệ quả 2 của Mệnh đề 6, § 2, no. 1, Mệnh đề 1 và § 3, no. 7, Mệnh đề 7.

Phần còn lại của chứng minh được tiến hành như trong (i) và quy về trường hợp $ E = A_s $; khi đó hai vế của (7) được đồng nhất một cách chính tắc với $ G \otimes_B F $ và $ \nu $ trở thành ánh xạ đồng nhất.

vào $ C $ là $ C $*-song tuyến tính*; do đó chỉ cần kiểm tra (20) khi $ u $ có dạng $ x \mapsto \langle x, a^* \rangle b $ và $ v $ có dạng $ y \mapsto \langle y, b^* \rangle a $, với $ a \in E, a^* \in E^*, b \in F, b^* \in F^* $. Nhưng khi đó $ v \circ u $ là ánh xạ $ x \mapsto \langle x, a^* \rangle \langle b, b^* \rangle a $ và $ u \circ v $ là ánh xạ $ y \mapsto \langle y, b^* \rangle \langle a, a^* \rangle b $. Công thức (17) chỉ ra rằng các giá trị của hai vế của (20) đều bằng $ \langle a, a^* \rangle \langle b, b^* \rangle $.

#### Hệ quả {#alg-ii-s4-n3-cor-1 .statement}

*Nếu $ u_1, \ldots, u_p $ là các tự đồng cấu của $ E $, thì*

$$
\mathrm{Tr}(u_1 \circ u_2 \circ \cdots \circ u_p) = \mathrm{Tr}(u_i \circ u_{i+1} \circ \cdots \circ u_p \circ u_1 \circ \cdots \circ u_{i-1})
$$

*với* $ 1 \leq i \leq p $ ("tính bất biến của vết đối với phép hoán vị chu kỳ").

Chỉ cần áp dụng (20) cho tích

$$(u_1 \circ u_2 \circ \cdots \circ u_{i-1}) \circ (u_i \circ u_{i+1} \circ \cdots \circ u_p).$$

Chú ý rằng mặt khác không nhất thiết đúng rằng

$$\operatorname{Tr}(u \circ v \circ w) = \operatorname{Tr}(u \circ w \circ v)$$

với ba tự đồng cấu $u, v, w$ của E.

### 4. ĐỒNG CẤU $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$

Cho C là một vành *giao hoán* và $E_1, E_2, F_1, F_2$ là bốn C-môđun; trong § 3, no. 5, công thức (13) ta đã định nghĩa một đồng cấu C-môđun chính tắc

(21) $\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)$.

#### Mệnh đề 4 {#alg-ii-s4-prop-4 .statement}

*Khi một trong các cặp có thứ tự* $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ *gồm các C-môđun xạ ảnh sinh hữu hạn, đồng cấu chính tắc* (21) *là song ánh.*

Hiển nhiên chỉ cần thực hiện chứng minh cho các cặp có thứ tự $(E_1, F_1)$ và $(E_1, E_2)$.

Trước hết ta xét trường hợp của cặp có thứ tự $(E_1, F_1)$; ta cố định $E_2, F_1, F_2$ và viết với *mọi* C-môđun $T(E) = \operatorname{Hom}(E, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$ và $T'(E) = \operatorname{Hom}(E \otimes E_2, F_1 \otimes F_2)$ và, với mọi đồng cấu C-môđun $v : E \to E'$,

$$T(v) = \operatorname{Hom}(v, 1_{F_1}) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

và

$$T'(v) = \operatorname{Hom}(v \otimes 1_{E_2}, 1_{F_1 \otimes F_2}).$$

Khi đó *Các Bổ đề 4 và 5* (no. 2) (*trong đó v* được thay bởi $\lambda$) *đều đúng* và được chứng minh bằng các phương pháp hoàn toàn tương tự.

Tiếp theo ta cố định $E_2$ và $F_2$ và lần này viết, với mọi C-môđun F,

$$T(F) = \operatorname{Hom}(C, F) \otimes_c \operatorname{Hom}(E_2, F_2)$$ và $T'(F) = \operatorname{Hom}(C \otimes E_2, F \otimes F_2)$ và, với mọi đồng cấu C-môđun $u : F \to F'$,

$$T(u) = \operatorname{Hom}(1_C, u) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

và

$$T'(u) = \operatorname{Hom}(1_C \otimes 1_{E_2}, u \otimes 1_{F_2}).$$

Lần này ta kiểm tra ngay lập tức rằng *Các Bổ đề 1 và 2* (no. 2) (*trong đó $\lambda$ luôn thay thế v*) *đều đúng*.

Do đó, ta chứng minh mệnh đề trước hết khi $E_1 = C$ và $F_1$ là xạ ảnh và sinh hữu hạn. Lập luận của no. 2 (dựa trên Các Bổ đề 1 và 2), cùng với các nhận xét trên, quy về việc chứng minh mệnh đề khi đồng thời $F_1 = C$; khi đó $\operatorname{Hom}(E_1, F_1), E_1 \otimes E_2$ và $F_1 \otimes F_2$ lần lượt được đồng nhất với C, $E_2$ và $F_2$ (\S 3, no. 4, Mệnh đề 4); hai vế của (21)

ĐỒNG CẤU $ \operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}(E_2, F_2) $

khi đó đều được đồng nhất một cách chính tắc với $ \operatorname{Hom}(E_2, F_2) $ và, sau các phép đồng nhất này, ta kiểm tra được rằng $ \lambda $ trở thành đồng nhất.

Bây giờ giả sử rằng $ F_1 $ là xạ ảnh và sinh hữu hạn; lập luận của no. 2 (lần này dựa vào Các Bổ đề 4 và 5) quy việc chứng minh đối với $ E_1 $ là một môđun xạ ảnh sinh hữu hạn tùy ý về trường hợp $ E_1 = C $, tức là trường hợp đầu tiên đã xét.

Đối với cặp có thứ tự $ (E_1, E_2) $, quy trình tương tự, lần này áp dụng Các Bổ đề 4 và 5 hai lần; ta để lại các chi tiết cho người đọc.

Chú ý rằng khi $ E_1 = C^{(I)} $, $ E_2 = C^{(J)} $ là tự do (sinh hữu hạn hoặc không), thì $ \operatorname{Hom}(E_1, F_1) = F_1^I $, $ \operatorname{Hom}(E_2, F_2 = F_2^J $ và
$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2) = (F_1 \otimes F_2)^{I \times J}
$$
sai khác một đẳng cấu chính tắc và (21) khi đó trùng với một trường hợp đặc biệt của đồng cấu chính tắc (22) của § 3, no. 7.
