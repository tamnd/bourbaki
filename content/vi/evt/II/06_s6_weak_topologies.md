---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 6
section_title: Weak topologies
lang: vi
source: evt-i-v
book_pages: TVS II.40-TVS II.53, TVS II.81-TVS II.86
pdf_pages: 0077-0090, 0118-0123
extraction: ocr
subsections:
    - "no": 1
      title: Dual vector spaces
      page: 40
      pdf_page: 77
    - "no": 2
      title: Weak topologies
      page: 42
      pdf_page: 79
    - "no": 3
      title: Polar sets and orthogonal subspaces
      page: 44
      pdf_page: 81
    - "no": 4
      title: Transposition of a continuous linear mapping
      page: 46
      pdf_page: 83
    - "no": 5
      title: Quotient spaces and subspaces of a weak space
      page: 48
      pdf_page: 85
    - "no": 6
      title: Products of weak topologies
      page: 50
      pdf_page: 87
    - "no": 7
      title: Weakly complete spaces
      page: 51
      pdf_page: 88
    - "no": 8
      title: Complete convex cones in weak spaces
      page: 52
      pdf_page: 89
statements: 41
exercises: 20
content_sha256: 61c16998c83e69790232fad377576526efb752c889b05ee1f4851616f07da0b0
translated_from: content/en/evt/II/06_s6_weak_topologies.md
source_content_sha256: 109eceeeb99cc76649276c19786c2e09a70e1491d491d1e3c49c950e18545c64
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-bef4b978
glossary_version: 34
glossary_terms_sha256: dcf6c6c18f4883e6428f98bc383169a5b307703af616402f6a780a0808a7a4eb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. TÔPÔ YẾU

### 1. Không gian vectơ đối ngẫu

Cho $ F $ và $ G $ là hai không gian vectơ thực và cho $ (x, y) \mapsto B(x, y) $ là một dạng *song tuyến tính* trên $ F \times G $. Ta nói rằng dạng song tuyến tính $ B $ *đặt các không gian vectơ* $ F $ *và* $ G $ *vào đối ngẫu*, hay rằng F và G đối ngẫu với nhau (đối với B). Nhắc lại rằng ta nói $ x \in F $ và $ y \in G $ trực giao với nhau (đối với đối ngẫu xác định bởi B) nếu $ B(x, y) = 0 $; ta nói rằng một tập con M của F và một tập con N của G trực giao với nhau nếu mọi $ x \in M $ đều trực giao với mọi $ y \in N $ (A, IX, § 1.2).

Ta nói rằng đối ngẫu xác định bởi B là tách được trong F (resp. trong G) nếu nó thỏa mãn điều kiện sau đây:

(D_I) *Với mọi $ x \neq 0 $ trong F, tồn tại $ y \in G $ sao cho $ B(x, y) \neq 0 $.* (resp.

(D_{II}) *Với mọi $ y \neq 0 $ trong G, tồn tại $ x \in F $ sao cho $ B(x, y) \neq 0 $.)

Đối ngẫu xác định bởi B được gọi là tách được nếu nó vừa tách được trong F vừa tách được trong G. Để điều này xảy ra, điều kiện cần và đủ là dạng song tuyến tính B phải tách được theo nghĩa của A, IX, § 1.1. Chính xác hơn, ta có kết quả sau đây:

#### Mệnh đề 1 {#evt-ii-s6-prop-1 .statement}

*Cho F, G là hai không gian vectơ thực và B là một dạng song tuyến tính trên $ F \times G $. Đặt*

$$
d_B : y \mapsto B(., y),
$$
$$
s_B : x \mapsto B(x, .)
$$

*là các ánh xạ tuyến tính của G vào đối ngẫu $ F^* $ của F và của F vào đối ngẫu $ G^* $ của G, tương ứng liên kết với phía phải và phía trái của B* (A, IX, § 1.1). Khi đó B đặt F và G vào một đối ngẫu tách được trong G (resp. trong F), khi và chỉ khi $ d_B $ (resp. $ s_B $) là đơn ánh.*

Khi F và G được đặt vào đối ngẫu tách được bởi B, ta thường đồng nhất F (resp. G) với một không gian con của $ G^* $ (resp. $ F^* $) nhờ $ s_B $ (resp. $ d_B $). Khi ta xét F (resp. G) như một không gian con của $ G^* $ (resp. $ F^* $) mà không chỉ rõ cách thực hiện sự đồng nhất này, ta luôn sử dụng các sự đồng nhất nêu trên; khi đó dạng song tuyến tính B được đồng nhất với hạn chế trên $ F \times G $ của dạng song tuyến tính chính tắc:

$$
(x^*, x) \mapsto \langle x, x^* \rangle \quad (\text{resp. } (x, x^*) \mapsto \langle x, x^* \rangle).
$$

#### Ví dụ {#evt-ii-s6-n1-exa-1 .statement}

— 1) Cho E là một không gian vectơ và E* là đối ngẫu của nó. Dạng song tuyến tính chính tắc $ (x, x^*) \mapsto \langle x, x^* \rangle $ trên $ E \times E^* $ (A, II, § 2.3) đặt E và E* vào đối ngẫu tách được: vì (D_{II}) đúng theo định nghĩa của quan hệ $ x^* \neq 0 $, và mặt khác, ta biết rằng với mọi $ x \neq 0 $ trong E, tồn tại một dạng tuyến tính $ x^* \in E^* $ sao cho $ \langle x, x^* \rangle \neq 0 $ (A, II, § 7.5, th. 6), điều này chứng minh (D_I); sự đồng nhất E với một không gian con của $ E^{**} $ ở đây được thực hiện bởi ánh xạ chính tắc $ c_E $ (*loc. cit.*).

Khi E có *chiều hữu hạn*, *không gian con duy nhất* G của E* được đặt vào đối ngẫu tách được bởi hạn chế trên $ E \times G $ của dạng song tuyến tính chính tắc là chính không gian E*; vì khi đó E được đồng nhất một cách chính tắc với $ E^{**} $ (*loc. cit.*), nếu ta có $ G \neq E^* $, sẽ tồn tại $ a \neq 0 $ trong E sao cho $ \langle a, x^* \rangle = 0 $ với mọi $ x^* \in G $ (A, II, § 7.5, th. 7), điều này mâu thuẫn với giả thiết.

2) Khi E là một không gian vectơ có *chiều vô hạn*, và E' là một không gian vectơ con của E*, đối ngẫu giữa E và E' xác định bởi hạn chế trên $ E \times E' $ của dạng song tuyến tính chính tắc luôn tách được trong E'; nó có thể tách được trong E ngay cả khi $ E' \neq E^* $. Trường hợp quan trọng nhất xảy ra khi E là một không gian vectơ tôpô.

#### Định nghĩa 1 {#evt-ii-s6-def-1 .statement}

— *Đối ngẫu của một không gian vectơ tôpô E là không gian con E' của E*, đối ngẫu của không gian vectơ E, gồm các dạng tuyến tính liên tục trên E.*

Khi E là một không gian *Hausdorff lồi địa phương*, đối ngẫu giữa E và đối ngẫu E' của nó là tách được: điều này suy ra từ định lý Hahn-Banach (II, p. 24, cor. 1) rằng với mọi $ x \neq 0 $ trong E, tồn tại $ x' \in E' $ sao cho $ \langle x, x' \rangle \neq 0 $.

#### Nhận xét {#evt-ii-s6-n1-rem-1 .statement}

— 1) Khi E là một không gian vectơ *tôpô*, đối ngẫu $ E^* $ của *không gian vectơ* E sẽ được gọi là *đối ngẫu đại số* của E để tránh nhầm lẫn. Ta cũng chú ý rằng $ E^* $ là đối ngẫu của không gian vectơ tôpô thu được bằng cách trang bị cho E tôpô lồi địa phương *mịn nhất* (II, p. 25, *Ví dụ* 2).
2) Đối ngẫu E' của một không gian vectơ tôpô tự nó không mang một tôpô, trừ khi điều này được nói rõ.
3) Nếu F và $ G \subset F^* $ đối ngẫu tách được với nhau bởi dạng song tuyến tính chính tắc, thì điều này cũng đúng đối với F và $ G_1 $, với mọi không gian con $ G_1 $ của $ F^* $ sao cho $ G \subset G_1 $.

### 2. Tôpô yếu

#### Định nghĩa 2 {#evt-ii-s6-def-2 .statement}

— *Cho F và G là hai không gian vectơ được đặt trong đối ngẫu bởi dạng song tuyến tính B. Tôpô thô nhất trên F làm cho mọi dạng tuyến tính $ B(., y): x \mapsto B(x, y) $ liên tục, với y thay đổi trong G, được gọi là tôpô yếu trên F xác định bởi đối ngẫu giữa F và G, và được ký hiệu là $ \sigma(F, G) $.*

Tương tự, ta định nghĩa tôpô yếu $ \sigma(G, F) $ trên G, đổi chỗ F và G trong định nghĩa 1 ; khả năng đổi chỗ F và G này áp dụng cho tất cả các kết quả và định nghĩa tiếp theo trong đoạn này.

Ta dùng tính từ « yếu » và trạng từ « yếu » để chỉ các tính chất tương đối với một tôpô yếu $ \sigma(F, G) $ khi không có khả năng nhầm lẫn. Chẳng hạn, ta sẽ nói « hội tụ yếu » và « các hàm liên tục yếu » v.v.

Khi $ G \subset F^* $, ký hiệu $ \sigma(F, G) $ luôn chỉ tôpô yếu được xác định bởi đối ngẫu tương ứng với hạn chế lên $ F \times G $ của dạng song tuyến tính chính tắc $ (x, x^*) \mapsto \langle x, x^* \rangle $.

Không có các giả thiết bổ sung trên F và G, ta thường viết $ \langle x, y \rangle $ cho giá trị $ B(x, y) $ của dạng song tuyến tính B tại $ (x, y) $, khi không có sự mơ hồ ; ta sẽ dùng quy ước này trong phần còn lại của đoạn này.

Một không gian vectơ F mang một tôpô yếu $ \sigma(F, G) $ được gọi là một *không gian yếu*.

Một tôpô yếu $ \sigma(F, G) $ là *lồi địa phương* (II, p. 26, mệnh đề 4) ; chính xác hơn, nó là ảnh ngược của tôpô *tích* của $ \mathbf{R}^G $ qua ánh xạ tuyến tính $ \phi : x \mapsto (\langle x, y \rangle)_{y \in G} $ từ F vào $ \mathbf{R}^G $. Nó được xác định bởi tập các *bán chuẩn* $ x \mapsto |\langle x, y \rangle| $ khi y thay đổi trong G (II, p. 5). Với mọi $ \alpha > 0 $, và mọi họ hữu hạn $ (y_i)_{1 \leq i \leq n} $ các phần tử của G, gọi $ W(y_1, ..., y_n; \alpha) $ là tập các $ x \in F $ sao cho $ |\langle x, y_i \rangle| \leq \alpha $ với $ 1 \leq i \leq n $; các tập hợp này (với $ \alpha, n $ và $ y_i $ tùy ý) tạo thành một *hệ cơ bản các lân cận của* 0 đối với $ \sigma(F, G) $. Chú ý rằng $ W(y_1, ..., y_n; \alpha) $ chứa *không gian con vectơ* của F, có đối chiều *hữu hạn*, được xác định bởi các phương trình $ \langle x, y_i \rangle = 0 $ với $ 1 \leq i \leq n $.

#### Mệnh đề 2 {#evt-ii-s6-prop-2 .statement}

— *Tôpô yếu* $ \sigma(F, G) $ *là Hausdorff khi và chỉ khi đối ngẫu giữa* $ F $ *và* $ G $ *là phân biệt trong* $ F $.

Đây là một trường hợp riêng của II, p. 3, mệnh đề 2.

#### Mệnh đề 3 {#evt-ii-s6-prop-3 .statement}

— *Cho* $ F $ *và* $ G $ *là hai không gian vectơ thực đối ngẫu. Mọi dạng tuyến tính trên* $ F $, *liên tục đối với* $ \sigma(F, G) $, *có thể viết dưới dạng* $ x \mapsto \langle x, y \rangle $ *với một* $ y \in G $. *Phần tử* $ y \in G $ *là duy nhất khi đối ngẫu là phân biệt trong* $ G $.

Bởi vì, nói rằng dạng tuyến tính $ f $ trên $ F $ liên tục đối với $ \sigma(F, G) $ có nghĩa là tồn tại một tập hữu hạn các phần tử $ y_i \in G $ ($ 1 \leq i \leq n $) sao cho, với mọi $ x $ trong $ F $, $ |f(x)| \leq \sup_{1 \leq i \leq n} |\langle x, y_i \rangle| $ (II, p. 6, mệnh đề 5). Do đó, $ n $ hệ thức $ \langle x, y_i \rangle = 0 $ ($ 1 \leq i \leq n $) kéo theo $ f(x) = 0 $, và vì vậy (A, II, § 7.5, hệ quả 1), tồn tại một tổ hợp tuyến tính $ y = \sum_{i=1}^n \lambda_i y_i $ sao cho $ f(x) = \langle x, y \rangle $ với mọi $ x \in F $. Tính duy nhất suy ra từ (D$_\text{II}$).

Nói cách khác, khi đối ngẫu là phân cách trong $ G $, và $ F $ có tôpô $ \sigma(F, G) $, thì ta có thể đồng nhất $ G $ một cách chính tắc với đối ngẫu của $ F $ đối với tôpô này (II, p. 42, def. 1).

#### Hệ quả 1 {#evt-ii-s6-prop-3-cor-1 .statement}

— *Một họ* $ (a_i) $ *các điểm của* $ F $ *là toàn phần đối với tôpô* $ \sigma(F, G) $ *khi và chỉ khi, với mọi* $ y \neq 0 $ *trong* $ G $, *tồn tại một chỉ số* $ i $ *sao cho* $ \langle a_i, y \rangle \neq 0 $.

Khi sử dụng mệnh đề 3 và I, p. 13, th. 1, tính chất này biểu thị rằng đối với $ \sigma(F, G) $ không có siêu phẳng đóng nào chứa tất cả các $ a_i $; do đó hệ quả suy ra từ hệ quả 3 của II, p. 38.

#### Hệ quả 2 {#evt-ii-s6-prop-3-cor-2 .statement}

— *Một họ* $ (a_i) $ *các điểm của* $ F $ *độc lập tôpô đối với tôpô* $ \sigma(F, G) $, *khi và chỉ khi, với mọi chỉ số* $ i $, *tồn tại một phần tử* $ b_i \in G $ *sao cho* : $ \langle a_i, b_i \rangle \neq 0 $ *và* $ \langle a_\kappa, b_i \rangle = 0 $ *với mọi* $ \kappa \neq i $.

Điều này có nghĩa là, với mọi $ i $, tồn tại một siêu phẳng đóng trong $ \sigma(F, G) $, chứa tất cả các $ a_\kappa $ với chỉ số $ \kappa \neq i $ nhưng không chứa $ a_i $.

#### Hệ quả 3 {#evt-ii-s6-prop-3-cor-3 .statement}

— *Cho* $ G_1 $ *và* $ G_2 $ *là hai không gian con vectơ của* $ F^* $, *đối ngẫu với* $ F $ *(đối với hạn chế của dạng song tuyến tính chính tắc)*. *Khi đó* $ \sigma(F, G_2) $ *mịn hơn* $ \sigma(F, G_1) $ *khi và chỉ khi* $ G_1 \subset G_2 $.

Điều kiện hiển nhiên là đủ; ngược lại, nếu $ \sigma(F, G_2) $ mịn hơn $ \sigma(F, G_1) $, thì mọi dạng tuyến tính liên tục đối với $ \sigma(F, G_1) $ cũng liên tục đối với $ \sigma(F, G_2) $, do đó $ G_1 \subset G_2 $ theo mệnh đề 3.

#### Hệ quả 4 {#evt-ii-s6-prop-3-cor-4 .statement}

— *Cho* $ G $ *là một không gian con vectơ của đối ngẫu* $ F^* $, *của không gian vectơ* $ F $. *Khi đó* $ F $ *và* $ G $ *ở trong đối ngẫu phân cách* (đối với dạng song tuyến tính chính tắc) *khi và chỉ khi* $ G $ *trù mật trong* $ F^* $ *đối với tôpô* $ \sigma(F^*, F) $.

Điều này suy ra từ hệ quả 1.

### 3. Tập cực và các không gian con trực giao

#### Định nghĩa 2 {#evt-ii-s6-def-2-bis .statement}

Cho F và G là hai không gian vectơ (thực) ở trong đối ngẫu. Với mỗi tập hợp M của F, ta gọi cực của M là tập hợp các y ∈ G sao cho $ \langle x, y \rangle \geq -1 $ với mọi $ x \in M $. (Đối với các không gian vectơ phức, xem II, p. 64.)

Nếu $ G_1, G_2 $ là hai không gian con của $ F^* $ sao cho $ G_1 \subset G_2 $, thì cực của M trong $ G_1 $ là giao của $ G_1 $ với cực của M trong $ G_2 $.

Khi không có nguy cơ nhầm lẫn, ta dùng $ M^\circ $ để ký hiệu cực, trong G, của tập con M của F. Tương tự, ta định nghĩa cực trong F của một tập hợp trong G.

Hiển nhiên, với mọi vô hướng $ \lambda \neq 0 $ và mọi $ M \subset F $, ta có $ (\lambda M)^\circ = \lambda^{-1} M^\circ $. Quan hệ $ M \subset N \subset F $ suy ra $ N^\circ \subset M^\circ $; nếu N hấp thụ M thì $ M^\circ $ hấp thụ $ N^\circ $; với mọi họ $ (M_\alpha) $ các tập hợp của F, tập cực của $ \bigcup \alpha M_\alpha $ là giao của các tập cực $ M_\alpha^\circ $. Vì, với $ y \in M^\circ $, các nửa không gian đóng được xác định bởi các quan hệ $ \langle x, y \rangle \geq -1 $ chứa 0 và M, nên ta thấy rằng nếu $ M_1 $ là bao lồi của $ M \cup \{0\} $, thì $ M_1^\circ = M^\circ $.

Rõ ràng $ M \subset M^{\circ \circ} $. Do đó
$$
(M^{\circ \circ})^\circ \subset M^\circ \subset (M^\circ)^{\circ \circ} = (M^{\circ \circ})^\circ
$$
tức là $ M^{\circ \circ \circ} = M^\circ $ (xem S, III, § 1.5, mệnh đề 2).

Nếu M là một tập con đối xứng của F, $ M^\circ $ là một tập con đối xứng của G; trong trường hợp này $ M^\circ $ cũng là tập hợp các $ y \in G $ sao cho $ |\langle x, y \rangle| \leq 1 $ với mọi $ x \in M $.

#### Mệnh đề 4 {#evt-ii-s6-prop-4 .statement}

(i) Với mọi tập hợp M của F, tập cực $ M^\circ $ là một tập lồi chứa 0 và đóng trong G đối với tôpô $ \sigma(G, F) $.

(ii) Nếu M là một nón có đỉnh 0, thì $ M^\circ $ là một nón có đỉnh 0 và nó cũng là tập hợp các $ y \in G $ sao cho $ \langle x, y \rangle \geq 0 $ với mọi $ x \in M $.

(iii) Nếu M là một không gian con vectơ của F, thì $ M^\circ $ là một không gian con vectơ của G, và nó cũng là tập hợp các $ y \in G $ sao cho $ \langle x, y \rangle = 0 $ với mọi $ x \in M $.

(i) Vì các dạng tuyến tính $ y \mapsto \langle x, y \rangle $ liên tục đối với $ \sigma(G, F) $, mệnh đề suy ra ngay lập tức từ các định nghĩa và từ thực tế rằng một nửa không gian được xác định bởi một siêu phẳng là lồi.

(ii) Nếu M là một nón có đỉnh 0 và nếu $ x \in M, y \in M^\circ $, thì vì $ \lambda x \in M $, với mọi $ \lambda > 0 $, ta có $ \langle \lambda x, y \rangle \geq -1 $, tức là $ \lambda \langle x, y \rangle \geq -1 $. Vì điều này đúng với mọi $ \lambda > 0 $, suy ra $ \langle x, y \rangle \geq 0 $, và (ii) được chứng minh.

(iii) Tương tự, nếu M là một không gian con vectơ của F, các quan hệ $ x \in M, y \in M^\circ $ lần này suy ra rằng $ \lambda \langle x, y \rangle \geq -1 $ với mọi vô hướng thực $ \lambda $, điều này chỉ có thể xảy ra khi $ \langle x, y \rangle = 0 $.

Nếu M là một không gian con vectơ của F, ta nói rằng $ M^\circ $ là trực giao của M trong G; nếu $ G \subset F^* $, thì $ M^\circ $ là giao của G với không gian con trực giao với M trong đối ngẫu đại số $ F^* $ của F (A, II, § 2.4, def. 4).

Với một không gian con vectơ M của F và một không gian con vectơ N của G, ta nói rằng M và N trực giao nếu $ M \subset N^o $ (hay, tương đương, nếu $ N \subset M^\circ $).

#### Định lý 1 (Định lý hai cực) {#evt-ii-s6-thm-1 .statement}

Cho F, G là hai không gian vectơ thực đối ngẫu. Với mọi tập con M của F, tập cực $ M^{\circ \circ} $ trong F của tập cực $ M^\circ $ của M trong G là bao lồi đóng (đối với $ \sigma(F, G) $) của $ M \cup \{0\} $.

Chúng ta đã thấy rằng chỉ cần xét trường hợp $ M $ là lồi và $ 0 \in M $. Gọi bao đóng của $ M $ trong tôpô $ \sigma(F, G) $ là $ \overline{M} $, khi đó $ \overline{M} $ là một tập hợp lồi trong $ F $; mệnh đề 4 của II, p. 44 cho thấy $ M^{\circ\circ} \supseteq \overline{M} $. Mặt khác, nếu $ a \in F $ không thuộc $ \overline{M} $ thì tồn tại một siêu phẳng đóng $ H $ trong $ F $ tách $ a $ một cách nghiêm ngặt khỏi $ \overline{M} $ (II, p. 38, mệnh đề 4); vì $ H $ không chứa 0, tồn tại $ y \in G $ sao cho $ H $ có phương trình $ \langle x, y \rangle = -1 $ (II, p. 43, mệnh đề 3); do đó $ \langle x, y \rangle > -1 $ với mọi $ x \in \overline{M} $ và $ \langle a, y \rangle < -1 $. Điều này suy ra rằng $ y \in M^\circ $ và $ a \notin M^{\circ\circ} $, và quan hệ $ M^{\circ\circ} = \overline{M} $ được suy ra.

#### Hệ quả 1 {#evt-ii-s6-thm-1-cor-1 .statement}

*Với mọi họ* $ (M_\alpha) $ *các tập hợp lồi đóng của* $ F $ *(trong tôpô* $ \sigma(F, G) $*), mỗi tập hợp chứa* 0, *tập hợp đối cực của giao* $ M = \bigcap \limits_{\alpha} M_\alpha $ *là bao lồi đóng* (*theo* $ \sigma(G, F) $) *của hợp các* $ M_\alpha^\circ $.

Thật vậy, nếu $ N $ là bao lồi đóng này, thì

$$
N^\circ = \bigcap \limits_{\alpha} M_\alpha^{\circ\circ} = \bigcap \limits_{\alpha} M_\alpha = M
$$

do đó $ N = N^{\circ\circ} = M^\circ $.

Kết luận của hệ quả 1 không nhất thiết đúng nếu các $ M_\alpha $ không lồi.

#### Hệ quả 2 {#evt-ii-s6-thm-1-cor-2 .statement}

*Với mọi không gian con vectơ* $ M $ *của* $ F $, *không gian con* $ M^{\circ\circ} $ *là bao đóng của* $ M $ *trong tôpô* $ \sigma(F, G) $.

#### Nhận xét {#evt-ii-s6-n3-rem-1 .statement}

— Mọi lân cận của 0 trong $ G $ đối với tôpô $ \sigma(G, F) $ đều chứa một lân cận $ V $ được xác định bởi một số hữu hạn bất đẳng thức có dạng $ |\langle x_i, y \rangle| \leq 1 $ ($ 1 \leq i \leq n $), trong đó các $ x_i $ là các điểm tùy ý của $ F $. Nếu $ A $ là *bao lồi đối xứng* của tập hợp các $ x_i $, thì $ V $ là *tập hợp cực* $ A^\circ $ của $ A $ trong $ G $. Ta có thể nói rằng *các tập cực trong* $ G $ *của các tập đối xứng hữu hạn trong* $ F $ (hoặc của các bao lồi của chúng) lập thành một hệ cơ bản các lân cận của 0 trong $ G $ đối với $ \sigma(G, F) $. Nếu đối ngẫu là tách được trong $ F $, các bao lồi này *compact* đối với $ \sigma(F, G) $ (II, p. 14, hệ quả 1 của mệnh đề 15), và có số chiều hữu hạn. Ngược lại, mọi *tập compact, lồi có số chiều hữu hạn* $ C $ trong $ F $ (với tôpô $ \sigma(F, G) $) đều được chứa trong bao lồi của một *tập con hữu hạn* của $ F $. Thật vậy, cho $ M $ là một không gian con vectơ có số chiều hữu hạn chứa $ C $. Nếu $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của $ M $, ta có thể giả sử rằng $ C $ được chứa trong hình bình hành đóng tâm 0 và được dựng trên các vectơ của cơ sở $ e_i $ (GT, VI, § 1.3); giờ đây ngay lập tức thấy rằng hình bình hành này là bao lồi của các điểm $ \sum \limits_{i=1}^n \varepsilon_i e_i $ với $ \varepsilon_i = \pm 1 $.

Do đó ta có thể nói rằng (nếu $ \sigma(F, G) $ là Hausdorff) *các tập cực của các tập hữu hạn chiều, lồi, compact trong* $ F $ (đối với $ \sigma(F, G) $ hoặc đối với bất kỳ tôpô lồi địa phương Hausdorff nào mịn hơn $ \sigma(F, G) $ trên $ F $) lập thành một hệ cơ bản các lân cận của 0 đối với $ \sigma(G, F) $.

#### Hệ quả 3 {#evt-ii-s6-thm-1-cor-3 .statement}

*Cho* $ \mathcal{T} $ *là tôpô của một không gian lồi địa phương* $ E $ *và cho* $ E' $ *là đối ngẫu của nó* (II, p. 42, định nghĩa 1).

(i) *Các tập lồi đóng trong E là như nhau đối với tôpô $ \mathcal{T} $ và đối với tôpô yếu $ \sigma(E, E') $.*

(ii) *Với mọi tập con M của E, tập cực $ M^{\circ\circ} $ trong E của tập cực $ M^\circ $ của M trong $ E' $, là bao lồi đóng của $ M \cup \{0\} $ đối với tôpô $ \mathcal{T} $.*

Rõ ràng, (ii) suy ra từ (i) và định lý 1. Từ định nghĩa của đối ngẫu $ E' $, suy ra từ II, p. 43, mệnh đề 3 rằng các dạng tuyến tính liên tục trên E đối với tôpô $ \mathcal{T} $ cũng chính là các dạng tuyến tính liên tục đối với $ \sigma(E, E') $. Do đó các nửa không gian đóng trong E cũng chính là các nửa không gian đóng đối với $ \mathcal{T} $ và đối với $ \sigma(E, E') $ (II, p. 15, mệnh đề 17), và mệnh đề (i) do đó suy ra từ II, p. 38, hệ quả 1.

### 4. Chuyển vị của một ánh xạ tuyến tính liên tục

Trong No. này, ta giả sử rằng (F, G) và $ (F_1, G_1) $ là hai không gian vectơ đối ngẫu.

#### Mệnh đề 5 {#evt-ii-s6-prop-5 .statement}

*Cho u là một ánh xạ tuyến tính từ F vào* $ F_1 $. *Các tính chất sau là tương đương:*

a) *u liên tục đối với các tôpô yếu* $ \sigma(F, G) $ *và* $ \sigma(F_1, G_1) $;

b) *tồn tại một ánh xạ* $ v : G_1 \to G $ *sao cho*

$$
\langle u(y), z_1 \rangle = \langle y, v(z_1) \rangle
$$

*với mọi* $ y \in F $ *và* $ z \in G_1 $.

*Nếu các tính chất này đúng và nếu đối ngẫu giữa F và G là tách được trong G, thì ánh xạ v thỏa mãn (1) là duy nhất, và v là tuyến tính.*

Nếu u liên tục đối với các tôpô yếu, thì với mọi $ z_1 \in G_1 $, dạng tuyến tính $ y \mapsto \langle u(y), z_1 \rangle $ trên F liên tục đối với $ \sigma(F, G) $, do đó (II, p. 43, mệnh đề 3) có thể viết dưới dạng $ y \mapsto \langle y, v(z_1) \rangle $ với $ v(z_1) \in G $, điều này cho thấy a) suy ra b). Ngược lại, nếu b) đúng, với mọi $ z_1 \in G_1 $, dạng tuyến tính

$$
y \mapsto \langle y, v(z_1) \rangle = \langle u(y), z_1 \rangle
$$

liên tục đối với $ \sigma(F, G) $ : từ định nghĩa của các tôpô yếu suy ra u liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $ (I, p. 10, hệ quả 1). Tính duy nhất của v suy ra từ (D_{II}) và tính duy nhất này kéo theo v tuyến tính.

#### Nhận xét {#evt-ii-s6-n4-rem-1 .statement}

— Giả sử rằng đối ngẫu giữa F và G là phân tách được trong G và đối ngẫu giữa $ F_1 $ và $ G_1 $ là phân tách được trong $ G_1 $. Nếu ta đồng nhất G và $ G_1 $ với các không gian con của $ F^* $ và $ F_1^* $ tương ứng, thì các điều kiện a) và b) tương đương với $ ^t u(G_1) \subset G $; v là hạn chế của chuyển vị $ ^t u $ của u (A, II, § 2.5) lên $ G_1 $.

Ta nói đơn giản (khi không có nguy cơ nhầm lẫn) rằng v là *chuyển vị* của u (đối với đối ngẫu một bên giữa F và G và bên kia giữa $ F_1 $ và $ G_1 $), và ta lại dùng $ ^t u $ để ký hiệu nó.

#### Hệ quả {#evt-ii-s6-n4-cor-1 .statement}

*Giả sử rằng đối ngẫu giữa F và G là phân tách được trong G. Nếu u là một ánh xạ tuyến tính từ F vào $ F_1 $, liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $, thì chuyển vị của nó là một ánh xạ tuyến tính từ $ G_1 $ vào $ G $, liên tục đối với $ \sigma(G_1, F_1) $ và $ \sigma(G, F) $. Hơn nữa, nếu đối ngẫu giữa $ F_1 $ và $ G_1 $ là phân tách được trong $ F_1 $ thì $ {}^t({}^t u) = u $.*

Chỉ cần đổi $ F $ và $ F_1 $ với $ G $ và $ G_1 $ trong mệnh đề 5.

#### Mệnh đề 6 {#evt-ii-s6-prop-6 .statement}

*Giả sử rằng đối ngẫu giữa $ F $ và $ G $ (tương ứng, $ F_1 $ và $ G_1 $) là phân tách được trong $ G $ (tương ứng, $ F_1 $). Cho $ u $ là một ánh xạ tuyến tính từ $ F $ vào $ F_1 $ liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $. Cho $ A $ là một tập hợp trong $ F $ và $ A_1 $ là một tập hợp trong $ F_1 $; khi đó*:

(i) *Ta có $ (u(A))^{\circ} = {}^t u^{-1}(A^{\circ}) $.*

(ii) *Ta có $ {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} $; hơn nữa, nếu $ A $ đóng, lồi (đối với $ \sigma(F_1, G_1) $), và chứa gốc, thì ta có $ {}^t u(A_1^{\circ}) = (u^{-1}(A_1))^{\circ} $.*

Cho $ z_1 \in G_1 $, quan hệ $ z_1 \in (u(A))^{\circ} $ tương đương với $ \langle u(y), z_1 \rangle \geq -1 $ với mọi $ y \in A $, và quan hệ $ {}^t u(z_1) \in A^{\circ} $ tương đương với $ \langle y, {}^t u(z_1) \rangle \geq -1 $ với mọi $ y \in A $ và mệnh đề (i) suy ra từ (1). Tiếp theo, đổi chỗ $ u $ và $ {}^t u $ và áp dụng (i) cho tập hợp $ A_1^{\circ} $ của $ G_1 $, ta được

$$
({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ}) \supset u^{-1}(A_1)
$$

từ đó, khi lấy đối cực,

$$
({}^t u(A_1^{\circ}))^{\circ \circ} \subset (u^{-1}(A_1))^{\circ} .
$$

Theo định lý song đối cực (II, p. 44, th. 1), ta có $ {}^t u(A_1^{\circ}) \subset ({}^t u(A_1^{\circ}))^{\circ \circ} $; khẳng định cuối cùng suy ra từ (2) và định lý song đối cực, vì khi đó $ A_1^{\circ \circ} = A_1 $ và $ {}^t u(A_1^{\circ}) $ là lồi và chứa gốc.

#### Hệ quả 1 {#evt-ii-s6-prop-6-cor-1 .statement}

*Với các ký hiệu của mệnh đề 6, quan hệ $ u(A) \subset A_1 $ kéo theo $ {}^t u(A_1^{\circ}) \subset A^{\circ} $; nếu thêm $ A_1 $ lồi, đóng (đối với $ \sigma(F_1, G_1) $) và chứa gốc, thì hai quan hệ này tương đương.*

Thật vậy, quan hệ $ u(A) \subset A_1 $ tương đương với $ A \subset u^{-1}(A_1) $, do đó kéo theo

$$
{}^t u(A_1^{\circ}) \subset {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} \subset A^{\circ}
$$

và ngược lại, quan hệ $ {}^t u(A_1^{\circ}) \subset A^{\circ} $ kéo theo

$$
A^{\circ \circ} \subset ({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ})
$$

theo (2). Khi $ A_1 = A_1^{\circ \circ} $, ta suy ra $ A \subset u^{-1}(A_1) $.

#### Hệ quả 2 {#evt-ii-s6-prop-6-cor-2 .statement}

*Cho $ u $ là một ánh xạ tuyến tính từ $ F $ vào $ F_1 $ liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $. Khi đó*

(3)

$$
\operatorname{Ker}({}^t u) = (\operatorname{Im}(u))^{\circ} ,
$$

(4)

$$
\overline{\operatorname{Im}({}^t u)} = (\operatorname{Ker}(u))^{\circ} .
$$

*Giả sử rằng các đối ngẫu giữa $ F $ và $ G $ và giữa $ F_1 $ và $ G_1 $ là phân biệt; khi đó $ u(F) $ trù mật trong $ F_1 $ (đối với $ \sigma(F_1, G_1) $) khi và chỉ khi $ {}^t u $ đơn ánh.*

Áp dụng mệnh đề 6 với $ A = F $ và $ A_1 = \{0\} $, sử dụng thực tế rằng các tôpô yếu $ \sigma(G, F) $ và $ \sigma(F_1, G_1) $ là Hausdorff. Khẳng định cuối cùng suy ra từ (4), đổi chỗ $ u $ và $ ^t u $.

### 5. Không gian thương và các không gian con của một không gian yếu

Cho $ F, G $ là hai không gian vectơ thực đối ngẫu. Cho $ M $ là một không gian con của $ F $, và xét không gian con $ N $ của phần tử trực giao $ M^\circ $ trong $ G $; nếu $ y_1, y_2 $ là hai điểm của $ G $ đồng dư mod. $ N $ thì $ \langle x, y_1 \rangle = \langle x, y_2 \rangle $ với mọi $ x \in M $. Với mỗi lớp $ \dot{y} $ mod. $ N $, ký hiệu giá trị chung của $ \langle x, y \rangle $ khi $ y $ biến thiên trong $ \dot{y} $ bởi $ \langle x, \dot{y} \rangle $; rõ ràng $ (x, \dot{y}) \mapsto \langle x, \dot{y} \rangle $ là một dạng song tuyến tính trên $ M \times (G/N) $.

#### Mệnh đề 7 {#evt-ii-s6-prop-7 .statement}

— *Cho $ M $ là một không gian con của $ F $ và $ N $ là một không gian con của $ G $ trong đó $ F $ và $ G $ là hai không gian vectơ đối ngẫu. Giả sử rằng $ M $ và $ N $ trực giao (điều này tương đương với việc nói rằng $ N \subset M^\circ $, hoặc $ M \subset N^\circ $). Khi đó các không gian vectơ $ M $ và $ G/N $ là đối ngẫu với nhau bởi dạng song tuyến tính* $ (x, \dot{y}) \mapsto \langle x, \dot{y} \rangle $.

(i) *Tôpô $ \sigma(M, G/N) $ đối với đối ngẫu này được cảm sinh bởi $ \sigma(F, G) $ (và đặc biệt ta có $ \sigma(F, G) = \sigma(F, G/F^\circ) $).

(ii) *Tôpô $ \sigma(G/N, M) $ đối với đối ngẫu này thô hơn tôpô thương của $ \sigma(G, F) $ bởi $ N $; các tôpô này trùng nhau khi và chỉ khi $ M + G^\circ = N^\circ $.

(i) Mọi phần tử của $ G/N $ là một lớp mod. $ N $ của một phần tử của $ G $; nếu $ z_i (1 \leq i \leq n) $ là các phần tử của $ G $ và $ \dot{z}_i (1 \leq i \leq n) $ là lớp của $ z_i $ trong $ G/N $ thì tập hợp các $ y \in M $ sao cho $ |\langle y, \dot{z}_i \rangle| \leq \alpha $ với $ 1 \leq i \leq n $ là vết trên $ M $ của tập hợp các $ x \in F $ sao cho $ |\langle x, z_i \rangle| \leq \alpha $ với $ 1 \leq i \leq n $; kết luận suy ra từ định nghĩa các lân cận của 0 đối với tôpô yếu.

(ii) Cho $ p : G \to G/N $ là toàn cấu chính tắc. Ta chứng minh rằng *tôpô thương* $ \mathcal{T} $ *của* $ \sigma(G, F) $ *theo* $ N $ *trùng với* $ \sigma(G/N, N^\circ) $. Vì, với $ z \in G, y \in N^\circ $, ta có $ \langle y, p(z) \rangle = \langle y, z \rangle $, nên mọi lân cận của 0 đối với $ \sigma(G/N, N^\circ) $ đều có dạng $ p(V) $, trong đó $ V $ là một lân cận của 0 đối với $ \sigma(G, F) $ bão hòa đối với quan hệ $ z - z' \in N $, do đó $ \mathcal{T} $ mịn hơn $ \sigma(G/N, N^\circ) $. Ngược lại, cho $ U = W(y_1, ..., y_n; \alpha) $ là một lân cận của 0 trong $ G $ đối với $ \sigma(G, F) $, trong đó $ y_i \in F $ với $ 1 \leq i \leq n $ và $ \alpha > 0 $; ta sẽ thấy rằng với $ 1 \leq i \leq n $, tồn tại các phần tử $ t_i \in N^\circ $ sao cho nếu đặt $ U' = W(t_1, ..., t_n; \alpha) $, thì $ p(U') \subset p(U) $; điều này sẽ chứng tỏ rằng $ \sigma(G/N, N^\circ) $ mịn hơn $ \mathcal{T} $ và do đó thực ra trùng với $ \mathcal{T} $. Bây giờ, cho $ L $ là không gian con vectơ của $ F $ sinh bởi $ N^\circ $ và các $ y_i $, và ký hiệu $ P $ là không gian con bù của $ N^\circ $ trong $ L $; nó có chiều hữu hạn, giả sử là $ m $. Cho $ (x_j)_{1 \leq j \leq m} $ là một cơ sở của $ P $; các hạn chế trên $ N $ của các dạng tuyến tính $ x \mapsto \langle x_j, z \rangle $ là độc lập tuyến tính, vì nếu không thì tồn tại $ x \neq 0 $ trong $ P $ sao cho $ \langle x, z \rangle = 0 $ với mọi $ z \in N $, tức là $ x \in N^\circ $, điều này mâu thuẫn với định nghĩa của $ P $. Do đó ta kết luận rằng với mọi $ z' \in G $, tồn tại $ s \in N $ sao cho $ \langle x_j, z' \rangle = \langle x_j, s \rangle $ với mọi $ j $; nếu $ z' = z + s $, thì ta có $ \langle x, z \rangle = 0 $ với mọi $ x \in P $. Với điều này, đặt $ y_i = t_i + w_i $, trong đó $ t_i \in N^\circ $ và $ w_i \in P $; ta có $ \langle y_i, z \rangle = \langle t_i, z \rangle = \langle t_i, z' \rangle $ với $ 1 \leq i \leq n $; do đó, với mọi $ z' \in U' $, tồn tại $ z \in U $ sao cho $ z' - z \in N $, tức là ta có $ p(U') \subset p(U) $.

Quay trở lại trường hợp M là một không gian con bất kỳ của N°, ta lưu ý rằng hiển nhiên $ \sigma(G/N, M) = \sigma(G/N, M + G^\circ) $; hơn nữa, từ mệnh đề 3 của II, p. 43, ta thấy rằng, nếu $ y \in N^\circ $ sao cho dạng tuyến tính $ \dot{z} \mapsto \langle y, \dot{z} \rangle $ là liên tục đối với $ \sigma(G/N, M) $, thì tất yếu $ y \in M + G^\circ $. Ta kết luận rằng điều kiện $ M + G^\circ = N^\circ $ là cần và đủ để tôpô thương $ \mathcal{T} $ bằng $ \sigma(G/N, M) $.

#### Nhận xét {#evt-ii-s6-n5-rem-1 .statement}

— Đối ngẫu giữa M và G/N (trong đó M và N là hai không gian con trực giao) là tách được trong M khi và chỉ khi $ M \cap G^\circ = \{0\} $; nó tách được trong G/N khi và chỉ khi $ N = M^\circ $.

#### Hệ quả 1 {#evt-ii-s6-prop-7-cor-1 .statement}

— Giả sử đối ngẫu giữa F và G là tách được trong F. Với một không gian con vectơ M của F, tôpô $ \sigma(G/M^\circ, M) $ đồng nhất với tôpô thương của $ \sigma(G, F) $ theo $ M^\circ $, khi và chỉ khi M đóng đối với tôpô $ \sigma(F, G) $.

Điều này suy ra từ mệnh đề 7 khi đặt $ N = M^\circ $, và nhớ rằng $ M^{\circ \circ} $ là bao đóng của M đối với $ \sigma(F, G) $ (II, p. 45, hệ quả 2).

#### Hệ quả 2 {#evt-ii-s6-prop-7-cor-2 .statement}

— Nếu M có số chiều hữu hạn n và đối ngẫu là tách được trong F, thì $ M^\circ $ có đối chiều n trong G. Nếu M đóng đối với $ \sigma(F, G) $ và có đối chiều hữu hạn n, và nếu đối ngẫu là tách được trong G, thì $ M^\circ $ có chiều n.

Thật vậy, $ G/M^0 $ ở trong đối ngẫu tách được với M; nếu M có chiều n, thì điều tương tự cũng đúng đối với $ G/M^\circ $ (II, p. 41, ví dụ 1). Nếu M đóng, $ F/M = F/M^{\circ \circ} $ ở trong đối ngẫu tách được với $ M^\circ $; nếu F/M có chiều n, thì điều tương tự cũng đúng đối với $ M^\circ $ (II, p. 41, ví dụ 1).

#### Hệ quả 3 {#evt-ii-s6-prop-7-cor-3 .statement}

— Cho (F, G), (F_1, G_1) là hai cặp không gian trong đối ngẫu tách được và cho u là một ánh xạ tuyến tính từ F vào F_1, liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $. Khi đó u là một cấu xạ ngặt từ F vào F_1 khi và chỉ khi Im($ ^t u $) là một không gian con đóng trong G đối với $ \sigma(G, F) $.

Đặt $ N = \operatorname{Im}(^t u) \subset G $; ta biết rằng $ N^0 = \operatorname{Ker}(u) $ trong F (II, p. 47, công thức (3)). Đặt $ p : F \to F/N^\circ $ là ánh xạ chính tắc sao cho u phân tích thành

$$
u : F \xrightarrow{p} F/N^\circ \xrightarrow{w} F_1,
$$

trong đó w đơn ánh. Các không gian $ F/N^\circ $ và N ở trong đối ngẫu tách được và theo công thức (1) của II, p. 48, ta có $ \langle w(\dot{y}), z_1 \rangle = \langle \dot{y}, ^t u(z_1) \rangle $ với mọi $ \dot{y} \in F/N^\circ $ và $ z_1 \in G_1 $. Quan hệ này cho thấy w là một đẳng cấu của $ F/N^\circ $, chuyển tôpô $ \sigma(F/N^\circ, N) $ lên u(F), với tôpô cảm sinh bởi $ \sigma(F_1, G_1) $. Do đó kết luận suy ra từ hệ quả 1 và định nghĩa cấu xạ ngặt.

#### Hệ quả 4 {#evt-ii-s6-prop-7-cor-4 .statement}

— Cho (F, G), (F_1, G_1) là hai cặp trong đối ngẫu tách được, và cho u là một ánh xạ tuyến tính từ F vào F_1 liên tục đối với $ \sigma(F, G) $ và $ \sigma(F_1, G_1) $. Khi đó u toàn ánh khi và chỉ khi $ ^t u $ là một đẳng cấu từ $ G_1 $ (với tôpô $ \sigma(G_1, F_1) $) lên $ ^t u(G_1) $ với tôpô cảm sinh bởi $ \sigma(G, F) $.

Thật vậy, nói rằng $ u(F) = F_1 $ tương đương với nói rằng $ u(F) $ đóng và trù mật khắp nơi trong $ F_1 $ đối với $ \sigma(F_1, G_1) $; hệ quả 4 sau đó suy ra từ hệ quả 3 áp dụng cho $ ^t u $ và II, p. 47, hệ quả 2.

#### Nhận xét {#evt-ii-s6-n5-rem-2 .statement}

— 1) Cho $ (F_1, G_1), (F_2, G_2), (F_3, G_3) $ là ba cặp không gian trong đối ngẫu tách được và xét một dãy gồm hai ánh xạ tuyến tính

$$
F_1 \xrightarrow{u} F_2 \xrightarrow{v} F_3
$$

liên tục đối với các tôpô yếu tương ứng với G_1, G_2, G_3; ta xét dãy các ánh xạ chuyển vị

$$
G_3 \xrightarrow{^tv} G_2 \xrightarrow{^tu} G_1 .
$$

Hiển nhiên $ ^t(v \circ u) = ^t u \circ ^t v $, do đó quan hệ $ v \circ u = 0 $ tương đương với $ ^t u \circ ^t v = 0 $. Dãy (5) là khớp khi và chỉ khi ba điều kiện sau đây được thỏa mãn

a) $ ^t u \circ ^t v = 0 $;
b) $ \operatorname{Im}(^t v) $ trù mật trong $ \operatorname{Ker}(^t u) $;
c) $ ^t u $ là một cấu xạ ngặt của $ G_2 $ vào $ G_1 $.

Điều này thực chất suy ra từ hệ quả 3 của II, p. 49 và các công thức (3) và (4) của II, p. 47.

2) Không nên nghĩ rằng khi $ u $ là một cấu xạ ngặt của $ F $ vào $ F_1 $, thì $ ^t u $ nhất thiết là một cấu xạ ngặt của $ G_1 $ vào $ G $; nói cách khác, $ u $ có thể là một cấu xạ ngặt mà $ u(F) $ không đóng trong $ F_1 $ đối với $ \sigma(F_1, G_1) $. Điều này được chỉ ra bởi ví dụ trong đó $ F $ là một không gian con không đóng của $ F_1 $ và $ G = G_1 / F^\circ $, $ u $ là đơn ánh chính tắc. Tương tự, việc dãy (5) khớp không nhất thiết kéo theo dãy (6) khớp, tuy nhiên, nếu dãy (5) khớp và $ v $ là một cấu xạ ngặt, thì dãy (6) khớp, theo nhận xét 1 và theo II, p. 49, hệ quả 3.

### 6. Tích của các tôpô yếu

#### Mệnh đề 8 {#evt-ii-s6-prop-8 .statement}

— Cho $ (F_i, G_i)_{i \in I} $ là một họ các cặp không gian đối ngẫu. Cho $ F = \prod_{i \in I} F_i $ là không gian tích của các $ F_i $ và $ G = \bigoplus_{i \in I} G_i $ là tổng trực tiếp của các $ G_i $. Nếu, với mọi $ x = (x_i) \in F $ và mọi $ y = (y_i) \in G $, ta viết $ \langle x, y \rangle = \sum_{i \in I} \langle x_i, y_i \rangle $ (một tổng chỉ có hữu hạn số hạng khác không) thì tôpô $ \sigma(F, G) $ (đối với dạng song tuyến tính $ (x, y) \mapsto \langle x, y \rangle $) là tích của các tôpô $ \sigma(F_i, G_i) $.

Thật vậy, cho một tôpô $ \mathcal{T} $ trên $ F $; để, với mọi $ y \in G $, dạng tuyến tính $ x \mapsto \langle x, y \rangle $ liên tục đối với $ \mathcal{T} $, thì theo định nghĩa của $ \langle x, y \rangle $, điều kiện cần và đủ là mỗi ánh xạ $ x \mapsto \langle \operatorname{pr}_i x, y_i \rangle $ phải liên tục đối với $ \mathcal{T} $, trong đó $ i $ tùy ý trong $ I $ và $ y_i $ trong $ G_i $; nhưng điều này có nghĩa là mỗi ánh xạ $ \operatorname{pr}_i $ của $ F $ vào $ F_i $ liên tục đối với $ \mathcal{T} $ và đối với $ \sigma(F_i, G_i) $ (I, p. 10, hệ quả 1); điều này hoàn tất chứng minh.

#### Nhận xét {#evt-ii-s6-n6-rem-1 .statement}

— Phép đối ngẫu giữa $ F $ và $ G $ là phân cách được trong $ F $ (tương ứng, trong $ G $) khi và chỉ khi với mọi $ i \in I $, phép đối ngẫu giữa $ F_i $ và $ G_i $ là phân cách được trong $ F_i $ (tương ứng, trong $ G_i $). Nếu phép đối ngẫu giữa $ F $ và $ G $ là phân cách được trong $ F $ (tương ứng, $ G $), thì, trong $ F $ (tương ứng, $ G $), không gian con trực giao với một $ G_i $ (tương ứng, $ F_i $), được đồng nhất một cách chính tắc với một không gian con của $ G $ (tương ứng, $ F $), là không gian con của tích của các $ F_\kappa $ với $ \kappa \neq i $ (tương ứng, tổng trực tiếp của các $ G_\kappa $ sao cho $ \kappa \neq i $).

#### Hệ quả 1 {#evt-ii-s6-prop-8-cor-1 .statement}

— Cho F và G là hai không gian vectơ đối ngẫu phân cách được. Nếu không gian F (với $ \sigma(F, G) $) là tổng tôpô trực tiếp của hai không gian con M, N thì không gian G (với $ \sigma(G, F) $) là tổng tôpô trực tiếp của các không gian con $ M^\circ, N^\circ $ lần lượt trực giao với M và N.

Thật vậy, cho $ p : F \to M, q : F \to N $ là các phép chiếu tương ứng với phân tích F thành tổng trực tiếp của M và N; khi đó ánh xạ $ (p, q) : F \to M \times N $ là một đẳng cấu tôpô. Nếu $ M_1 = G/M^\circ, N_1 = G/N^\circ $, thì các tôpô trên M và N (cảm sinh bởi tôpô của F) lần lượt đồng nhất với $ \sigma(M, M_1) $, $ \sigma(N, N_1) $ (II, p. 48, mệnh đề 7). Ánh xạ $ ^t(p, q) : M_1 \times N_1 \to G $ là một đẳng cấu tôpô khi ta trang bị cho $ M_1, N_1 $ và G các tôpô $ \sigma(M_1, M) $, $ \sigma(N_1, N) $ và $ \sigma(G, F) $, theo mệnh đề 8. Qua ánh xạ này, $ M_1 $ (tương ứng, $ N_1 $) có ảnh trong G là không gian con $ N^\circ $ (tương ứng, $ M^\circ $), và tôpô $ \sigma(M_1, M) $ (tương ứng, $ \sigma(N_1, N) $) có ảnh là tôpô cảm sinh trên $ N^\circ $ (tương ứng, $ M^\circ $) bởi $ \sigma(G, F) $, từ đó suy ra hệ quả.

#### Hệ quả 2 {#evt-ii-s6-prop-8-cor-2 .statement}

— Cho $ (e_i)_{i \in J} $ là một cơ sở của không gian vectơ F với đối ngẫu $ F^* $, và cho $ u : \mathbf{R}^{(I)} \to F $ là một đẳng cấu (đại số) được xác định bởi cơ sở này. Khi đó ánh xạ chuyển vị $ ^t u : F^* \to \mathbf{R}^I $ là một đẳng cấu tôpô khi $ F^* $ được trang bị tôpô $ \sigma(F^*, F) $ và $ \mathbf{R}^I $ tôpô tích.

Chúng ta biết (A, II, § 2.6, prop. 10) rằng $ ^t u $ là một song ánh, và nếu với một $ x^* \in F^* $, ta đặt $ \langle e_i, x^* \rangle = \xi_i^* $ với mọi $ i \in I $, thì ảnh $ ^t u(x^*) $ là vectơ $ (\xi_i^*) $ của $ \mathbf{R}^I $, do đó, với mọi $ x = \sum_i \xi_i e_i $ trong F, ta có $ \langle x, x^* \rangle = \sum_i \xi_i \xi_i^* $. Hệ quả sau đó suy ra từ công thức này và mệnh đề 8.

### 7. Các không gian đầy đủ yếu

#### Mệnh đề 9 {#evt-ii-s6-prop-9 .statement}

— Cho F, G là hai không gian vectơ đối ngẫu phân ly. Nếu $ \hat{F} $ là sự đầy đủ hóa của không gian F đối với tôpô $ \sigma(F, G) $ và nếu ta xét đơn ánh chính tắc $ j : F \to G^* $, trong đó $ G^* $ được trang bị tôpô $ \sigma(G^*, G) $, thì mở rộng liên tục $ \hat{j} : \hat{F} \to G^* $ của j là một đẳng cấu của các không gian vectơ tôpô.

Thật vậy, ta thấy rằng $ G^* $, được trang bị $ \sigma(G^*, G) $, là Hausdorff và đầy đủ (II, p. 51, cor. 2); nếu ta đồng nhất F qua j với một không gian con vectơ của $ G^* $ thì tôpô cảm sinh trên F bởi $ \sigma(G^*, G) $ là $ \sigma(F, G) $, và F trù mật trong $ G^* $ đối với tôpô $ \sigma(G^*, G) $ (II, p. 43, cor. 4); từ đó mệnh đề được suy ra.

Do đó, các không gian vectơ đầy đủ đối với một tôpô yếu chính là các đối ngẫu $ G^* $ của các không gian vectơ tùy ý G được trang bị $ \sigma(G^*, G) $; theo II, p. 51, cor. 2, chúng (về mặt tôpô) đẳng cấu với các tích $ \mathbf{R}^I $ của các đường thẳng thực. Để đơn giản hóa cách diễn đạt, ta sẽ gọi chúng là các tích của các đường thẳng (để có một đặc trưng nội tại của các không gian này, xem II, p. 85, exerc. 13 và II, p. 81, exerc. 1).

Ta chú ý rằng trên $ G^* $, tôpô $ \sigma(G^*, G) $ là cực tiểu trong các tôpô yếu Hausdorff; thật vậy, một tôpô yếu thô hơn $ \sigma(G^*, G) $ nhất thiết có dạng $ \sigma(G^*, H) $ trong đó $ H \subset G $ (II, p. 43, cor. 3); nhưng nếu $ H \neq G $, thì tồn tại một dạng tuyến tính $ x^* \in G^* $ khác không và trực giao với $ H $ (A, II, § 7.3, prop. 8), do đó $ \sigma(G^*, H) $ không Hausdorff.

Ta suy ra từ nhận xét này rằng, nếu $ F, G $ là hai không gian vectơ, thì một *song ánh tuyến tính* $ u : G^* \to F^* $, liên tục đối với các tôpô $ \sigma(G^*, G) $ và $ \sigma(F^*, F) $, nhất thiết là *bicontinuous*.

#### Mệnh đề 10 {#evt-ii-s6-prop-10 .statement}

*Cho $ G $ là một không gian vectơ thực và $ F = G^* $ là đối ngẫu của nó với tôpô $ \sigma(G^*, G) $.*

(i) *Ánh xạ $ V \mapsto V^\circ $ là một song ánh từ tập hợp các không gian con vectơ của $ G $ lên tập hợp các không gian con vectơ đóng của $ F $.*

(ii) *Mọi không gian con vectơ đóng của $ F $ đều là một tích của các đường thẳng và có một phần bù tôpô.*

Theo định lý lưỡng cực (II, p. 45, cor. 2) $ V \mapsto V^\circ $ là một song ánh từ tập hợp các không gian con vectơ $ V $ của $ G $, *đóng* đối với $ \sigma(G, G^*) $ lên tập hợp các không gian con vectơ đóng của $ F $. Nhưng, theo định nghĩa, *mọi* dạng tuyến tính trên $ G $ đều liên tục đối với $ \sigma(G, G^*) $, do đó mọi không gian con vectơ trong $ G $ đều đóng, vì được xác định bởi một hệ phương trình $ \langle y, y_\lambda^* \rangle = 0 $ (trong đó $ y_\lambda^* \in G^* $); điều này chứng minh (i).

Bây giờ cho $ W $ là một không gian con đóng của $ F $; khi đó ta có $ W = V^\circ $ với $ V = W^\circ $ trong $ G $. Cho $ V' $ là một không gian bù của $ V $ trong $ G $. Ta biết rằng $ F = G^* $ có thể được đồng nhất một cách chính tắc với $ V^* \oplus {V'}^* $, và $ {V'}^* $ được đồng nhất với $ V^\circ = W $ (A, II, § 2.6, hệ quả của mệnh đề 10); hơn nữa (II, p. 50, mệnh đề 8), tôpô $ \sigma(G^*, G) $ có thể được đồng nhất với tích của các tôpô $ \sigma(V^*, V) $ và $ \sigma({V'}^*, V') $; điều này chứng minh mệnh đề (ii).

Mặc dù, đối với tôpô $ \sigma(G, G^*) $, mọi không gian con vectơ của $ G $ đều đóng, ta chú ý rằng nếu $ G $ có chiều vô hạn thì tôpô $ \sigma(G, G^*) $ không phải là tôpô lồi địa phương mạnh nhất trên $ G $, mọi lân cận của 0 đối với $ \sigma(G, G^*) $ đều chứa một không gian con vectơ có chiều vô hạn: tuy nhiên, nó là mạnh nhất trong các tôpô *yếu* trên $ G $ (II, p. 43, hệ quả 3).

### 8. Nón lồi đầy đủ trong các không gian yếu

#### Bổ đề 1 {#evt-ii-s6-lem-1 .statement}

*Một không gian yếu Hausdorff $ E $ và một nón thực sự $ C $ có đỉnh 0 trong $ E $, tức là đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của $ E $. Khi đó mọi dạng tuyến tính liên tục trên $ E $ là hiệu của hai dạng tuyến tính liên tục trên $ E $ dương trên $ C $.*

Cho $ E' $ là đối ngẫu của $ E $ và $ F $ là đối ngẫu đại số của $ E' $, với tôpô $ \sigma(F, E') $. Cho $ H = C^\circ - C^\circ $ là không gian con vectơ của $ E' $ được tạo bởi các hiệu của các dạng tuyến tính liên tục trên $ E $ và dương trên $ C $ (II, p. 44, mệnh đề 4). Chỉ cần chứng minh rằng trực giao của $ H $ trong $ F $ là $ \{0\} $ (II, p. 41, *Ví dụ* 1). Khi đó cho $ a \in F $ trực giao với $ H $; vì $ a $ trực giao với $ C^\circ $, nên nó phải thuộc song cực của $ C $ trong $ F $. Nhưng $ E $ có thể được đồng nhất với một không gian con của $ F $, và vì $ C $ đầy đủ, do đó đóng trong $ F $, ta có $ a \in C $ (II, p. 44, định lý 1). Tương tự $ a $ trực giao với $ -C^\circ $ và do đó $ a \in -C $. Vì $ C $ là thực sự, ta có $ a = 0 $.

#### Mệnh đề 11 {#evt-ii-s6-prop-11 .statement}

*Cho $ E $ là một không gian yếu Hausdorff, và $ C $ là một nón lồi thực sự có đỉnh 0 trong $ E $ và đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của $ E $.*

Khi đó tồn tại một tập hợp I và một ánh xạ tuyến tính liên tục u từ E vào không gian tích $ \mathbf{R}^I $ có các tính chất sau:

a) u là một đẳng cấu của C lên $ u(C) $ đối với các cấu trúc đều lần lượt cảm sinh bởi các cấu trúc đều của E và $ \mathbf{R}^I $.

b) Ta có $ u(C) \subset \mathbf{R}_+^I $.

Hơn nữa, nếu cấu trúc đều cảm sinh trên C bởi cấu trúc đều của E là khả mêtric, thì có thể lấy $ I = \mathbf{N} $.

Cho $ (f_i)_{i \in I} $ là một họ các dạng tuyến tính liên tục trên E sao cho các tổng hữu hạn của các giả mêtric dạng $ (x, y) \mapsto |f_i(x - y)| $ trên $ C \times C $ định nghĩa cấu trúc đều của C. (Nếu cấu trúc đều là khả mêtric thì có thể lấy $ I = \mathbf{N} $.) Theo Bổ đề 1, ta có thể giả sử thêm rằng mỗi $ f_i $ đều dương trên C. Gọi u là ánh xạ tuyến tính $ x \mapsto (f_i(x))_{i \in I} $ từ E vào $ \mathbf{R}^I $. Hiển nhiên u liên tục và $ u(C) \subset \mathbf{R}_+^I $. Hạn chế $ u|C $ là một ánh xạ đều liên tục toàn ánh từ C lên $ u(C) $. Hơn nữa, nếu $ x, y $ thuộc C sao cho $ f_i(x) = f_i(y) $ với mọi $ i \in I $, thì $ x = y $ vì cấu trúc đều của C là Hausdorff; do đó $ u|C $ là song ánh. Cuối cùng, nếu W là một lân cận đều của cấu trúc đều của C, thì tồn tại một tập hữu hạn J của I và một số $ \varepsilon > 0 $ sao cho các quan hệ $ |f_i(x) - f_i(y)| \leq \varepsilon $ với $ i \in J $ kéo theo $ (x, y) \in W $; do đó $ u|C $ là một đẳng cấu của C lên $ u(C) $ đối với các cấu trúc đều đang xét.

#### Hệ quả 1 {#evt-ii-s6-prop-11-cor-1 .statement}

— Cho E là một không gian yếu Hausdorff và C là một nón lồi thực sự có đỉnh 0 trong E, đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của E. Khi đó ánh xạ $ (x, y) \mapsto x + y $ từ $ C \times C $ vào C là thực sự.

Theo Mệnh đề 11, ta có thể giả sử rằng $ E = \mathbf{R}^I $ và $ C = \mathbf{R}_+^I $ (GT, I, § 10.1, hệ quả 1 và 4). Nhưng khi đó ánh xạ $ (x, y) \mapsto x + y $ từ $ C \times C $ vào C được viết dưới dạng $ ((\xi_i), (\eta_i)) \mapsto (\xi_i + \eta_i) $, và ta có thể hạn chế vào việc chứng minh rằng ánh xạ liên tục $ f : (\xi, \eta) \mapsto \xi + \eta $ từ $ \mathbf{R}_+ \times \mathbf{R}_+ $ vào $ \mathbf{R}_+ $, là thực sự (GT, I, § 10.1, hệ quả 3), Bây giờ, với mọi $ \zeta \in \mathbf{R}_+ $, ta thấy rằng $ f(\zeta) $ là tập hợp các cặp $ (\xi, \zeta - \xi) $ sao cho $ 0 \leq \xi \leq \zeta $, do đó ảnh ngược bởi f của khoảng $ [0, \zeta] $ là tập hợp các $ (\xi, \eta) \in \mathbf{R}_+ \times \mathbf{R}_+ $ sao cho $ \xi + \eta \leq \zeta $, là compact. Kết luận suy ra bằng cách áp dụng (GT, I, § 10.3, Mệnh đề 7).

#### Hệ quả 2 {#evt-ii-s6-prop-11-cor-2 .statement}

— Cho E là một không gian yếu Hausdorff, và C là một nón lồi thực sự có đỉnh 0 trong E, đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của E.

(i) Với mọi điểm a của E, giao $ C \cap (a - C) $ là compact.

(ii) Cho A, B là hai tập đóng trong C. Khi đó $ A + B $ là một tập đóng trong C.

(i) Tập hợp các $ (x, y) \in C \times C $ sao cho $ x + y = a $ là compact theo Hệ quả 1 và GT, I, § 10.2, định lý 1, b). Bây giờ tập hợp này cũng chính là tập hợp các $ (x, a - x) $ với $ x \in C \cap (a - C) $, điều này chứng minh (i).

(ii) Nếu A và B đóng trong C, thì $ A \times B $ đóng trong $ C \times C $, do đó $ A + B $ đóng trong C theo Hệ quả 1 và GT, I, § 10.1, Mệnh đề 1.

### Bài tập {#evt-ii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
