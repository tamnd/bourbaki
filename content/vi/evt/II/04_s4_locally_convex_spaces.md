---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 4
section_title: Locally convex spaces
lang: vi
source: evt-i-v
book_pages: TVS II.23-TVS II.36, TVS II.74-TVS II.76
pdf_pages: 0060-0073, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a locally convex space
      page: 23
      pdf_page: 60
    - "no": 2
      title: Examples of locally convex spaces
      page: 25
      pdf_page: 62
    - "no": 3
      title: Locally convex initial topologies
      page: 26
      pdf_page: 63
    - "no": 4
      title: Locally convex final topologies
      page: 27
      pdf_page: 64
    - "no": 5
      title: The direct topological sum of a family of locally convex spaces
      page: 29
      pdf_page: 66
    - "no": 6
      title: Inductive limits of sequences of locally convex spaces
      page: 31
      pdf_page: 68
    - "no": 7
      title: Remarks on Fréchet spaces
      page: 34
      pdf_page: 71
statements: 33
exercises: 17
content_sha256: c80638666d24e0fedcf82b1c0fc89acb94d7fe65dc5c0bdbf83ba65d51a5886f
translated_from: content/en/evt/II/04_s4_locally_convex_spaces.md
source_content_sha256: e1bb43693581a8af707527021cd7c1fd51a9366f361ba89b7bca0de240534ab7
translation_model: gpt-5-6, gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-c1232c45
glossary_version: 34
glossary_terms_sha256: 6201e98fd19b523812d0cda306427af5d077ddb755464575a6d5953eadef2d8e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. KHÔNG GIAN LỒI ĐỊA PHƯƠNG

### 1. Định nghĩa không gian lồi địa phương

#### Định nghĩa 1 {#evt-ii-s4-def-1 .statement}

— *Một không gian vectơ tôpô là lồi địa phương (thực) nếu tồn tại một hệ lân cận cơ bản của 0 gồm các tập hợp lồi.*

Một không gian như vậy được gọi là một *không gian lồi địa phương*. Tôpô của nó được gọi là một *tôpô lồi địa phương*.

Các không gian vectơ tôpô trên $ \mathbf{R} $ mà chúng ta nghiên cứu trong phần còn lại của cuốn sách này hầu hết đều là lồi địa phương.

Nếu $ V $ là một lân cận lồi của 0 trong không gian lồi địa phương $ E $, thì $ V \cap (-V) $ là một lân cận lồi đối xứng của 0. Vì bao đóng của một tập hợp lồi là lồi (II, p. 13, mệnh đề 14), theo I, p. 7, mệnh đề 4, các lân cận của 0 trong $ E $ *đóng, đối xứng và lồi* tạo thành một hệ lân cận cơ bản bất biến qua các phép vị tự có tâm 0 và tỉ số $ \neq 0 $.

#### Mệnh đề 1 {#evt-ii-s4-prop-1 .statement}

— *Cho $ \mathfrak{S} $ là một cơ sở lọc trên một không gian vectơ $ E $ được tạo thành từ các tập hợp hấp thụ, đối xứng và lồi. Khi đó tập hợp $ \mathfrak{B} $ gồm các ảnh của các tập hợp thuộc $ \mathfrak{S} $ qua các phép vị tự có tỉ số $ > 0 $ là một hệ lân cận cơ bản của 0 đối với một tôpô lồi địa phương trên $ E $.*

Rõ ràng $ \mathfrak{B} $ là một cơ sở lọc thỏa mãn (EV_I) và (EV_{II}) của I, p. 7, mệnh đề 4; nó cũng thỏa mãn (EV_{III}) vì nếu $ V \in \mathfrak{S} $ thì $ \frac{1}{2}V + \frac{1}{2}V = V $.

Chú ý rằng nếu $ \mathcal{T} $ là tôpô lồi địa phương trên E có $ \mathfrak{B} $ làm hệ lân cận cơ bản của 0, thì các tập hợp $ (1/n) \ V $, trong đó $ n $ biến thiên trong các số nguyên $ > 0 $ và V biến thiên trong $ \mathfrak{S} $, tạo thành một hệ lân cận cơ bản của 0 đối với tôpô $ \mathcal{T} $. Khi đó $ \mathcal{T} $ là Hausdorff khi và chỉ khi, với mọi $ x \neq 0 $ trong E, tồn tại một số nguyên $ n $ và một tập hợp $ V \in \mathfrak{S} $, sao cho $ nx \notin V $; hơn nữa, nếu $ \mathfrak{S} $ là đếm được, thì tôpô $ \mathcal{T} $ là một tôpô lồi địa phương có thể mêtric hóa. Ngược lại, rõ ràng rằng nếu $ \mathcal{T} $ là một tôpô lồi địa phương có thể mêtric hóa, thì tồn tại một hệ lân cận cơ bản đếm được gồm các lân cận đóng, đối xứng, lồi của 0 đối với $ \mathcal{T} $.

#### Hệ quả {#evt-ii-s4-n1-cor-1 .statement}

— *Tôpô $ \mathcal{T} $ của một không gian vectơ tôpô E được xác định bởi một tập hợp các nửa chuẩn* (II, p. 3) *khi và chỉ khi $ \mathcal{T} $ là lồi địa phương*.

Điều kiện là cần thiết vì mọi nửa chuẩn trên E đều là một hàm lồi, và do đó, với $ \alpha > 0 $, tập hợp các $ x \in E $ sao cho $ p(x) \leq \alpha $, là lồi (II, p. 17, hệ quả). Ngược lại, nếu V là một lân cận đối xứng, đóng, lồi của 0 trong E, thì *hàm gauge* $ p $ của V là một nửa chuẩn trên E sao cho V là tập hợp các điểm $ x $ của E thỏa mãn $ p(x) \leq 1 $ (II, p. 20, mệnh đề 23).

Điều này còn cho thấy rằng một tôpô lồi địa phương $ \mathcal{T} $ được xác định bởi tập hợp *tất cả các nửa chuẩn liên tục đối với $ \mathcal{T} $*. Hơn nữa, nếu $ \mathcal{T} $ có thể mêtric hóa, thì nó được xác định bởi một tập hợp *đếm được* các nửa chuẩn.

Từ hệ quả của mệnh đề 1, tất cả các kết quả của § 1 về các tôpô được xác định bởi các tập hợp nửa chuẩn đều áp dụng đặc biệt cho các tôpô lồi địa phương trên các không gian vectơ thực. Một không gian Hausdorff lồi địa phương E có một phép hoàn thành $ \hat{E} $ cũng lồi địa phương. Một không gian lồi địa phương đầy đủ, có thể mêtric hóa được gọi là một *không gian Fréchet*; mọi không gian Banach đều là một không gian Fréchet.

#### Mệnh đề 2 {#evt-ii-s4-prop-2 .statement}

— *Cho f là một dạng tuyến tính liên tục xác định trên một không gian con vectơ M của một không gian lồi địa phương E; khi đó tồn tại một dạng tuyến tính liên tục h xác định trên E và là một mở rộng của f*.

Từ hệ quả trên và II, p. 7, hệ quả 2, tồn tại một nửa chuẩn liên tục $ p $ trên E, sao cho $ |f(y)| \leq p(y) $ với mọi $ y \in M $. Theo định lý Hahn-Banach (II, p. 23, hệ quả 1), tồn tại một dạng tuyến tính $ h $ trên E mở rộng $ f $ và sao cho $ |h(x)| \leq p(x) $ với mọi $ x \in E $, và điều này suy ra rằng $ h $ liên tục (II, p. 6, mệnh đề 5).

#### Nhận xét {#evt-ii-s4-n1-rem-1 .statement}

— Nếu $ g $ là một ánh xạ tuyến tính liên tục của M vào không gian tích $ \mathbf{R}^I $, thì tồn tại một ánh xạ tuyến tính liên tục $ h $ của E vào $ \mathbf{R}^I $ là một sự mở rộng của $ g $; vì khi viết $ g = (g_i) $, trong đó các $ g_i $ là các dạng tuyến tính liên tục xác định trên M, thì với mỗi $ i \in I $ có một sự mở rộng $ h_i $ của $ g_i $, sao cho $ h_i $ là một dạng tuyến tính liên tục trên E. Ánh xạ tuyến tính liên tục $ h = (h_i) $ có các tính chất cần thiết.

Chú ý rằng nếu F là một không gian Hausdorff lồi địa phương và $ g $ là một ánh xạ tuyến tính liên tục của M vào F, thì không nhất thiết tồn tại một ánh xạ tuyến tính liên tục của E vào F là một sự mở rộng của $ g $ (IV, p. 55, bài tập 16, c)). Tuy nhiên có tồn tại một sự mở rộng như vậy khi M hữu hạn chiều (*xem* hệ quả 2, dưới đây).

#### Hệ quả 1 {#evt-ii-s4-prop-2-cor-1 .statement}

— *Cho E là một không gian lồi địa phương. Nếu $ x_0 \in E $ không thuộc bao đóng của $ \{0\} $, thì tồn tại một dạng tuyến tính liên tục f xác định trên E sao cho $ f(x_0) \neq 0 $*.

Áp dụng mệnh đề 2 cho không gian vectơ một chiều M sinh bởi $ x_0 $ và cho dạng tuyến tính $ \xi x_0 \mapsto \xi $ xác định trên M, mà theo I, p. 12, mệnh đề 2, là liên tục.

#### Hệ quả 2 {#evt-ii-s4-prop-2-cor-2 .statement}

— Cho M là một không gian con vectơ hữu hạn chiều của E, một không gian Hausdorff lồi địa phương. Khi đó tồn tại một không gian con vectơ đóng N của E, là phần bù tôpô của M trong E.

Tồn tại một phần bù tôpô của M trong E nếu, và chỉ nếu, ánh xạ đồng nhất của M lên chính nó có thể được mở rộng thành một ánh xạ tuyến tính liên tục của E lên M, và ánh xạ đó khi ấy tất yếu là một phép chiếu liên tục (GT, III, § 6.2, hệ quả). Điều này suy ra từ nhận xét trên vì M đẳng cấu với một không gian $ \mathbf{R}^n $ (I, p. 13, định lý 2).

#### Mệnh đề 3 {#evt-ii-s4-prop-3 .statement}

— Trong một không gian lồi địa phương E, bao lồi cân bằng của một tập tiền compact cũng là một tập tiền compact.

Cho A là một tập tiền compact trong E. Với V, một lân cận lồi cân bằng của 0 trong E, tồn tại hữu hạn nhiều điểm $ a_i \in A $ ($ 1 \leq i \leq n $) sao cho A được chứa trong S, là hợp của các lân cận $ a_i + V $ ($ 1 \leq i \leq n $). Do đó C, bao lồi cân bằng của A, được chứa trong T, bao lồi cân bằng của S; nhưng T được chứa trong B + V, trong đó B ký hiệu bao lồi của tập hữu hạn các điểm $ a_i, -a_i $ ($ 1 \leq i \leq n $). Bây giờ B là tiền compact (II, p. 14, hệ quả 2); suy ra tồn tại hữu hạn nhiều điểm $ b_k \in B $ ($ 1 \leq k \leq m $) sao cho $ B_k $ được chứa trong hợp của các lân cận $ b_k + V $. Khi đó C được chứa trong hợp của các lân cận $ b_k + 2V $, và mệnh đề được chứng minh.

Chú ý rằng, trong một không gian Hausdorff lồi địa phương vô hạn chiều, bao lồi của một tập compact không nhất thiết đóng (II, p. 74, bài tập 3).

#### Hệ quả {#evt-ii-s4-n1-cor-2 .statement}

— Nếu, trong một không gian Hausdorff lồi địa phương E, một tập compact X được chứa trong một tập lồi đầy đủ (đầy đủ trong cấu trúc đều cảm sinh bởi cấu trúc của E) thì bao lồi đóng của X là compact.

Vì bao này là một tập con đóng của một không gian đầy đủ, nên nó đầy đủ, nhưng nó cũng tiền compact và Hausdorff.

Tuy nhiên, trong một không gian Hausdorff lồi địa phương không đầy đủ, bao lồi đóng của một tập compact không nhất thiết compact (II, p. 87, bài tập 2).

### 2. Các ví dụ về không gian lồi địa phương

1) Không gian $ \mathbf{R}^n $ là lồi địa phương vì các khối lập phương mở có tâm 0 là lồi (II, p. 9, mệnh đề 6). Điều này, do đó, cũng đúng cho mọi không gian vectơ tôpô thực hữu hạn chiều; thật vậy, điều đó suy ra từ điều trên và I, § 2.3, định lý 2 với giả thiết E là Hausdorff; nếu không, không gian Hausdorff F liên kết với E là hữu hạn chiều, nên lồi địa phương, và các ảnh ngược của các lân cận lồi của 0 trong F qua ánh xạ chính tắc $ E \to F $ là lồi và tạo thành một hệ cơ bản các lân cận của 0 trong E.

2) Cho E là một không gian vectơ trong $ \mathbf{R} $, và $ \mathfrak{B} $ là họ của mọi tập con của E thâu hút, đối xứng và lồi. Theo mệnh đề 1 của II, p. 23 ta thấy rằng $ \mathfrak{B} $ là một hệ cơ bản các lân cận của 0 cho một tôpô lồi địa phương $ \mathcal{T}_\omega $ trên E, là tôpô mạnh nhất trong số mọi tôpô lồi địa phương trên E. Tôpô này là Hausdorff; vì hãy lấy $ x \neq 0 $ là một điểm bất kỳ của E; tồn tại một cơ sở $(i_i)_{i \in I}$ của E với một $\alpha \in I$ sao cho $e_\alpha = x$; tập các điểm $y = \sum_i y_i e_i$ sao cho $|y_\alpha| < 1$ là thâu hút, đối xứng và lồi. Nó không chứa $x$. Từ II, p. 24, hệ quả, suy ra rằng $ \mathcal{T}_\omega $ cũng là tôpô được xác định bởi tập của *mọi* nửa chuẩn trên E, do đó mọi nửa chuẩn đều liên tục trong $ \mathcal{T}_\omega $.

Đặc biệt, nếu $u$ là một ánh xạ tuyến tính của E vào bất kỳ không gian lồi địa phương F nào, thì ảnh ngược, qua $u$, của mọi lân cận lồi của 0 trong F là một tập lồi *thâu hút* trong E; do đó nó là một lân cận của 0 đối với $ \mathcal{T}_\omega $ và vì thế $u$ là *liên tục* đối với $ \mathcal{T}_\omega $.

Cho một tập lồi C trong E, ta nói rằng một điểm $a \in C$ là một *điểm trong* của C nếu, với mọi đường thẳng D chứa a, giao $D \cap C$ chứa một đoạn mở chứa a; nói cách khác — $a + C$ là *thâu hút*. Điểm $a$ của tập A trong E là *điểm trong của A đối với* $ \mathcal{T}_\omega $ khi và chỉ khi tồn tại một tập lồi C sao cho $a \in C \subset A$, và sao cho $a$ là một điểm trong của C.

Tổng quát hơn, cho V là một đa tạp afin tuyến tính trong E, và cho C là một tập lồi được chứa trong V; một điểm $a \in C$ là một *điểm nội tại của C tương đối với* V nếu, trong không gian con vectơ $V_0 = -a + V$, điểm 0 là một điểm nội tại của tập $C_0 = -a + C$.

Khi E có số chiều hữu hạn, tôpô $\mathcal{T}_\omega$ chỉ là tôpô chính tắc trên E (I, p. 13, định lý 2); điều đó cho thấy rằng mọi điểm nội tại của một tập lồi C trong E đều là điểm trong của C theo tôpô chính tắc (*xem* II, p. 74, bài tập 5).

3) Cho A là một tập lồi đối xứng trong không gian vectơ E trên $\mathbf{R}$. Không gian con vectơ F *sinh bởi* A cũng là nón lồi sinh bởi A, vì $-A = A$; tập này là tập các $\lambda x$ với $x \in A$ và $\lambda \in \mathbf{R}$; tập A là *hấp thụ trong* F và các tập $\lambda A$ với $\lambda > 0$, tạo thành một hệ cơ sở các lân cận của 0 cho một tôpô lồi địa phương *trên* F (gọi là *được xác định bởi* A), được xác định bởi nửa chuẩn $p_A$, *hàm gauge* của A (II, p. 20, mệnh đề 22); ký hiệu $E_A$ là không gian lồi địa phương thu được khi trang bị cho F nửa chuẩn này. Không gian $E_A$ là *Hausdorff* khi và chỉ khi $p_A$ là một *nửa chuẩn* hoặc tương đương A không chứa *bất kỳ đường thẳng nào*. Nếu B là một tập lồi đối xứng thứ hai trong E và nếu $A \subset B$, thì rõ ràng $E_A \subset E_B$, và đơn ánh chính tắc của $E_A$ vào $E_B$ là *liên tục* đối với các tôpô được xác định tương ứng bởi A và bởi B. Hơn nữa, nếu $f$ là một ánh xạ tuyến tính của E vào một không gian vectơ thực $E'$, thì $f(A)$ là lồi và đối xứng trong $E'$ và $f$ là một ánh xạ tuyến tính *liên tục* của $E_A$ *trên* $E'_{f(A)}$.

Sau cùng, hãy chú ý rằng nếu E mang một tôpô $\mathcal{T}$ tương thích với cấu trúc không gian vectơ của nó, và nếu V là một lân cận *lồi* đối xứng của 0 đối với $\mathcal{T}$, thì không gian vectơ sinh bởi V trùng với E, vì V là hấp thụ, và ánh xạ đồng nhất của E vào $E_V$ là *liên tục*.

### 3. Các tôpô ban đầu lồi địa phương

#### Mệnh đề 4 {#evt-ii-s4-prop-4 .statement}

*Cho E là một không gian vectơ và cho $(E_i)_{i \in I}$ là một họ các không gian lồi địa phương. Với mỗi $i \in I$, cho $f_i$ là một ánh xạ tuyến tính của E vào $E_i$; khi đó tôpô* $\mathcal{T}$ *trên E, là tôpô thô nhất làm cho mỗi ánh xạ $ f_i $ liên tục, là một tôpô lồi địa phương.*

Dùng II, p. 24, hệ quả, đây là một trường hợp riêng của tính chất tương ứng đối với các tôpô được xác định bởi nửa chuẩn (II, p. 5).

Đặc biệt, mọi không gian con vectơ của một không gian lồi địa phương, và mọi không gian tích của các không gian lồi địa phương, đều lồi địa phương. Mọi giới hạn xạ ảnh của các không gian lồi địa phương đều lồi địa phương.

Mọi *tích đếm được* của các không gian Fréchet (và đặc biệt mọi tích đếm được của các không gian Banach) đều là một không gian Fréchet.

Mọi không gian Hausdorff lồi địa phương E đều đẳng cấu với một không gian con của một tích các không gian Banach và không gian con này đóng nếu E đầy đủ (II, p. 5, mệnh đề 3). Mọi không gian Fréchet đều đẳng cấu với một không gian con đóng của một tích đếm được các không gian Banach (*loc. cit.*).

### 4. Các tôpô cuối lồi địa phương

#### Mệnh đề 5 {#evt-ii-s4-prop-5 .statement}

*Cho E là một không gian vectơ, và $ (F_\alpha)_{\alpha \in A} $ là một họ các không gian vectơ tôpô và với mỗi $ \alpha \in A $, cho $ g_\alpha $ là một ánh xạ tuyến tính của $ F_\alpha $ vào E.*

(i) *Ký hiệu $ \mathfrak{B} $ là họ các tập con hấp thụ, đối xứng, lồi V của E sao cho $ g_\alpha^{-1}(V) $ là một lân cận của 0 trong $ F_\alpha $ với mọi $ \alpha $; họ $ \mathfrak{B} $ là một hệ cơ sở các lân cận của 0 trong E đối với một tôpô $ \mathcal{T} $ tương thích với cấu trúc không gian vectơ.*

(ii) *Một ánh xạ tuyến tính f của E vào một không gian lồi địa phương G (tương ứng, một nửa chuẩn p trên E) là liên tục đối với $ \mathcal{T} $ khi và chỉ khi, với mọi chỉ số $ \alpha $, $ f \circ g_\alpha $ (tương ứng, $ p \circ g_\alpha $) là liên tục trên $ F_\alpha $.*

(iii) *Tôpô $ \mathcal{T} $ là tôpô mịn nhất trong các tôpô lồi địa phương trên E sao cho các $ g_\alpha $ liên tục.*

*Hơn nữa, tôpô $ \mathcal{T} $ là tôpô lồi địa phương duy nhất trên E thỏa mãn điều kiện (ii) đối với các ánh xạ tuyến tính (tương ứng, đối với các nửa chuẩn).*

Vì $ \mathfrak{B} $ là một cơ sở lọc bất biến đối với các phép vị tự có tỉ số > 0, mệnh đề (i) suy ra ngay lập tức từ II, p. 23, mệnh đề 1. Theo định nghĩa của $ \mathfrak{B} $, tôpô $ \mathcal{T} $ là tôpô lồi địa phương mịn nhất trên E làm cho các $ g_\alpha $ liên tục; do đó (iii). Cuối cùng, rõ ràng rằng nếu $ f $ liên tục thì $ f \circ g_\alpha $ cũng liên tục; ngược lại, nếu các $ f \circ g_\alpha $ liên tục với mọi $ \alpha $, thì với mỗi lân cận lồi đối xứng W của 0 trong G, tập $ g_\alpha^{-1}(f^{-1}(W)) $ là một lân cận của 0 trong $ F_\alpha $ với mỗi $ \alpha $. Khi đó $ f^{-1}(W) $ là hấp thụ, đối xứng và lồi, do đó $ f^{-1}(W) $ là một lân cận của 0 trong $ \mathcal{T} $, và $ f $ liên tục. Tương tự, nếu $ p $ là một nửa chuẩn trên E sao cho $ p \circ g_\alpha $ liên tục với mọi $ \alpha $, và nếu U là tập hợp các điểm $ x \in E $ sao cho $ p(x) < 1 $, thì, với mọi $ \alpha $, tập $ g_\alpha^{-1}(U) $ là một lân cận lồi của 0 trong $ E_\alpha $ đối xứng và hấp thụ; do đó U là một lân cận của 0 trong E và $ p $ liên tục (II, p. 2, mệnh đề 1).

Mệnh đề cuối cùng suy ra từ S, IV, § 2.5, tiêu chuẩn CST 18.

Ta nói rằng $ \mathcal{T} $ là *tôpô cuối lồi địa phương* của họ các tôpô $ \mathcal{T}_\alpha $ của các $ F_\alpha $, đối với họ các ánh xạ tuyến tính $ g_\alpha $.

Có thể xảy ra rằng $ \mathcal{T} $ không phải là tôpô mịn nhất trong các tôpô trên E tương thích với cấu trúc không gian vectơ của nó và làm cho các $ f_\alpha $ liên tục (II, p. 75, bài tập 15; xem thêm II, p. 75, bài tập 14).

Trong trường hợp quan trọng nhất $ E = \sum_{\alpha \in A} g_\alpha(F_\alpha) $, ta có một hệ cơ sở các lân cận của 0 đối với $ \mathcal{T} $ như sau; với mỗi $ \alpha \in A $, lấy $ V_\alpha $ là một lân cận đối xứng của 0 đối với $ \mathcal{T}_\alpha $, lập hợp của các $ g_\alpha(V_\alpha) $ với $ \alpha \in A $ và ký hiệu bao lồi trong E của hợp này bởi $ \Gamma((g_\alpha(V_\alpha))) $; vì mọi phần tử của E đều có dạng $ \sum_{\alpha \in J} x_\alpha $, trong đó J là một tập con hữu hạn của I và $ x_\alpha \in g_\alpha(F_\alpha) $, nên ngay lập tức $ \Gamma((g_\alpha(V_\alpha))) $ là một tập lồi đối xứng hấp thụ trong E (mỗi $ V_\alpha $ đều hấp thụ trong $ F_\alpha $); vì $ \Gamma((g_\alpha(V_\alpha))) $ chứa tất cả các $ g_\alpha(V_\alpha) $, nên nó là một lân cận của 0 đối với $ \mathcal{T} $. Mặt khác, rõ ràng rằng với mọi lân cận lồi đối xứng V của 0 đối với $ \mathcal{T} $, ta có $ V \supset \Gamma((V \cap g_\alpha(F_\alpha))) $, từ đó suy ra mệnh đề của chúng ta.

#### Hệ quả 1 {#evt-ii-s4-prop-5-cor-1 .statement}

*Với các ký hiệu của mệnh đề 5, cho H là một tập các ánh xạ tuyến tính từ E vào không gian lồi địa phương G. Giả sử E là tổng các không gian con $ g_\alpha(F_\alpha) $ của nó; khi đó H là đẳng liên tục đối với $ \mathcal{T} $, khi và chỉ khi, với mọi $ \alpha $, tập $ f \circ g_\alpha $ trong đó $ f $ chạy trên H, là đẳng liên tục trong $ F_\alpha $.*

Nhắc lại I, p. 9, Mệnh đề 6, lập luận tương tự như lập luận của (ii) Mệnh đề 5. Cho W là một lân cận lồi đối xứng của 0 trong G và chú ý rằng nếu họ $ f \circ g_\alpha $, trong đó $ f \in H $ là liên tục đều, thì giao $ \bigcap_{f \in H} g_\alpha^{-1}(f^{-1}(W)) $ là một lân cận lồi đối xứng của 0 trong $ F_\alpha $. Vì giao này chính là $ g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W)) $ và tập hợp $ \bigcap_{f \in H} f^{-1}(W) $ là đối xứng và lồi, nên mọi việc quy về việc chứng minh rằng nó còn *hấp thụ*. Theo giả thiết, mọi $ x \in E $ đều có thể viết dưới dạng $ \sum_{i=1}^n g_{\alpha_i}(z_{\alpha_i}) $, trong đó $ z_{\alpha_i} \in F_{\alpha_i} $. Để chứng minh rằng tồn tại $ \lambda > 0 $ sao cho $ f(\lambda x) \in W $ với mọi $ f \in H $, chỉ cần xét trường hợp $ x = g_\alpha(z_\alpha) $ với $ z_\alpha \in F_\alpha $ (vì có thể chuyển sang trường hợp tổng quát bằng cách thay thế W bởi $ W/n $). Nhưng trường hợp này suy ra từ việc $ g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W)) $ là một lân cận của 0 trong $ F_\alpha $.

#### Hệ quả 2 {#evt-ii-s4-prop-5-cor-2 .statement}

*Cho $ (J_\lambda)_{\lambda \in L} $ là một phân hoạch của tập hợp chỉ số A. Cho $ (G_\alpha)_{\alpha \in A} $ là một họ các không gian lồi địa phương và $ (F_\lambda)_{\lambda \in L} $ là một họ các không gian vectơ. Với mỗi $ \lambda \in L $, cho $ h_\lambda $ là một ánh xạ tuyến tính từ $ F_\lambda $ vào một không gian vectơ E; với mỗi $ \lambda \in L $ và $ \alpha \in J_\lambda $, cho $ g_{\lambda \alpha} $ là một ánh xạ tuyến tính từ $ G_\alpha $ vào $ F_\lambda $. Đặt $ f_\alpha = h_\lambda \circ g_{\lambda \alpha} $. Giả sử rằng mỗi $ F_\lambda $ mang tôpô lồi địa phương mịn nhất làm cho các $ g_{\lambda \alpha} $ ($ \alpha \in J_\lambda $) liên tục. Khi đó, tôpô lồi địa phương mịn nhất trên E làm cho các $ f_\alpha $ liên tục trùng với tôpô lồi địa phương mịn nhất làm cho các $ h_\lambda $ liên tục.*

Đây là một trường hợp riêng của tiêu chuẩn CST 19, S, IV, § 2.5, và cũng có thể được chứng minh trực tiếp bằng Mệnh đề 5.

Các tôpô cuối lồi địa phương.

I. Không gian thương.

Cho M là một không gian con của không gian lồi địa phương F, và φ là ánh xạ chính tắc từ F lên F/M. Vì tôpô thương trên F/M là lồi địa phương và là mịn nhất trong tất cả các tôpô (lồi địa phương hay không) làm cho φ liên tục, nên nó cũng là tôpô cuối lồi địa phương đối với họ gồm ánh xạ duy nhất φ.

II. Giới hạn quy nạp của các không gian lồi địa phương.

Cho A là một tập hợp có thứ tự có hướng sang phải và $(E_\alpha, f_{\beta\alpha})$ là một hệ quy nạp các không gian vectơ tương ứng với tập A (A, II, § 6.2); cho $E = \varinjlim E_\alpha$ và với mỗi $\alpha \in A$, cho $f_\alpha : E_\alpha \to E$ là ánh xạ tuyến tính chính tắc. Giả sử mỗi $E_\alpha$ mang một tôpô lồi địa phương $\mathcal{T}_\alpha$, và hơn nữa giả sử rằng với $\alpha \leq \beta$, ánh xạ $f_{\beta\alpha} : E_\alpha \to E_\beta$ là *liên tục*. Khi đó ta nói rằng tôpô cuối lồi địa phương $\mathcal{T}$ của họ $(\mathcal{T}_\alpha)$ tương ứng với các ánh xạ tuyến tính $f_\alpha$ (tương ứng, không gian E mang tôpô $\mathcal{T}$) là *giới hạn quy nạp* của họ $(\mathcal{T}_\alpha)$ (tương ứng, không gian *giới hạn quy nạp* của hệ $(E_\alpha, f_{\beta\alpha})$, hay đơn giản là của các không gian lồi địa phương $E_\alpha$). Nhắc lại rằng E là hợp của các không gian con vectơ $f_\alpha(E_\alpha)$ và rằng khi $\alpha \leq \beta$, ta có $f_\alpha(E_\alpha) \subset f_\beta(E_\beta)$; nếu ta trang bị cho $f_\alpha(E_\alpha)$ tôpô cuối đối với ánh xạ $f_\alpha$ (điều đó tương đương với việc đồng nhất $f_\alpha(E_\alpha)$ với không gian thương $E_\alpha/f_\alpha^{-1}(0)$), thì tôpô $\mathcal{T}$ cũng là tôpô cuối của họ các tôpô của các $f_\alpha(E_\alpha)$, tương ứng với các đơn ánh chính tắc (II, hệ quả 2 ở trên). Hơn nữa, tính liên tục của $f_{\beta\alpha}$ với $\alpha \leq \beta$ suy ra rằng đơn ánh chính tắc $j_{\beta\alpha} : f_\alpha(E_\alpha) \to f_\beta(E_\beta)$ là liên tục, do đó E cũng là giới hạn quy nạp của $f_\alpha(E_\alpha)$ mang các tôpô nói trên tương ứng với đơn ánh $j_{\beta\alpha}$.

#### Ví dụ {#evt-ii-s4-n4-exa-1 .statement}

— Cho X là một không gian địa phương compact và $E = \mathscr{K}(X; \mathbf{R})$ là không gian vectơ của các hàm thực liên tục xác định trên X có giá compact. Với mỗi tập con compact K của X, cho $E_K$ là không gian con vectơ của E gồm các hàm $f \in E$ thỏa mãn $x \notin K \Rightarrow f(x) = 0$. Ký hiệu $\mathcal{T}_K$ là tôpô cảm sinh trên $E_K$ và $\mathcal{T}_u$ là tôpô của *hội tụ đều* trên X. Giới hạn quy nạp $\mathcal{T}$ của các tôpô $\mathcal{T}_K$ mịn hơn $\mathcal{T}_u$; ta có thể chứng minh rằng nếu X là paracompact và không compact, thì $\mathcal{T}$ mịn hơn một cách thực sự so với $\mathcal{T}_u$ (*xem* INT, III, 2nd ed., § 1.8). Tầm quan trọng của $\mathcal{T}$ nằm ở chỗ các dạng tuyến tính trên E liên tục theo $\mathcal{T}$ chính xác là các *độ đo* thực trên X (INT, III, 2nd., § 1.3).

#### Nhận xét {#evt-ii-s4-n4-rem-1 .statement}

— Trong ví dụ cuối, tôpô cảm sinh bởi $\mathcal{T}$ trên $E_K$ trùng với $\mathcal{T}_K$, vì theo định nghĩa nó thô hơn $\mathcal{T}_K$ và, do $\mathcal{T}$ mịn hơn $\mathcal{T}_u$, tôpô cảm sinh bởi $\mathcal{T}$ trên $E_K$ mịn hơn tôpô cảm sinh bởi $\mathcal{T}_u$, tức là $\mathcal{T}_K$.

Lập luận này tổng quát hóa ngay lập tức cho một giới hạn quy nạp của các tôpô lồi địa phương $(\mathcal{T}_\alpha)$ khi có một tôpô lồi địa phương $\mathcal{T}'$ trên E sao cho $\mathcal{T}_\alpha$ là tôpô cảm sinh trên $E_\alpha$ bởi $\mathcal{T}'$.

Nói tổng quát hơn, ta có thể hỏi rằng, khi giả sử $E_\beta \subset E_\alpha$ và $\mathcal{T}_\beta$ là tôpô cảm sinh bởi $\mathcal{T}_\alpha$, thì trong những trường hợp nào $\mathcal{T}$ cảm sinh $\mathcal{T}_\alpha$ trên mỗi $E_\alpha$. Nói chung điều này không đúng (II, p. 80, bài tập 26); nhưng trong các Số sau ta sẽ thấy hai tình huống quan trọng mà điều này xảy ra.

### 5. Tổng trực tiếp tôpô của một họ các không gian lồi địa phương

#### Định nghĩa 2 {#evt-ii-s4-def-2 .statement}

*Cho E là không gian vectơ là tổng trực tiếp* (A, II, § 1.6) *của họ các không gian lồi địa phương* $(E_i)_{i \in I}$. *Với mỗi* $i \in I$, *gọi* $f_i$ *là đơn ánh chính tắc* của $ E_i $ vào $ E $. *Ta gọi tổng trực tiếp tôpô của họ* $ (E_i) $ *là không gian* $ E $ *với tôpô lồi địa phương mịn nhất làm cho mỗi* $ f_i $ *liên tục (tôpô này được gọi là tổng trực tiếp của các tôpô của* $ E_i $).

Trong phần còn lại của Số này, ta giữ các ký hiệu như trong định nghĩa 2 (trừ khi có quy định rõ điều ngược lại) và ta đồng nhất, một cách chính tắc, mỗi $ E_i $ với một không gian con của $ E $, nhờ $ f_i $.

Theo mô tả tổng quát về các lân cận của một tôpô cuối lồi địa phương được cho trong II, p. 28, ở đây ta có thể thu được một hệ cơ bản các lân cận của 0 trong $ E $ đối với tôpô tổng trực tiếp, theo cách sau đây; với *mọi* họ $ (V_i)_{i \in I} $ trong đó $ V_i $ là một lân cận lồi đối xứng của 0 trong $ E_i $, xét bao lồi $ \Gamma((V_i)) $, của hợp của các $ V_i $; các $ \Gamma((V_i)) $ với mọi họ $ (V_i) $ (hoặc chỉ lấy $ V_i $ với mỗi $ i $ thuộc một hệ cơ bản các lân cận của 0 trong $ E_i $) tạo thành một hệ cơ bản các lân cận của 0 trong $ E $.

#### Ví dụ {#evt-ii-s4-n5-exa-1 .statement}

— Cho $ (a_i)_{i \in I} $ là một cơ sở của không gian vectơ $ E $ và xét tôpô chính tắc (I, p. 2, *Ví dụ 5*) trên mỗi đường thẳng $ Ra_i $; tổng trực tiếp của các tôpô này là tôpô lồi địa phương *mịn nhất* trên $ E $ (II, p. 26); thật vậy, nếu $ V $ là một tập hấp thụ, đối xứng, lồi trong $ E $, thì $ V_i = V \cap Ra_i $ là một lân cận của 0 trong $ Ra_i $ và $ V $ rõ ràng chứa bao lồi $ \Gamma((V_i)) $.

#### Mệnh đề 6 {#evt-ii-s4-prop-6 .statement}

*Một tôpô lồi địa phương* $ \mathcal{T} $ *trên* $ E $ *là tổng trực tiếp của các tôpô của* $ E_i $, *khi và chỉ khi tính chất sau đây được thỏa mãn: một ánh xạ tuyến tính từ* $ E $ *vào một không gian lồi địa phương* $ G $ *(tương ứng một nửa chuẩn* $ p $ *trên* $ E $) *là liên tục khi và chỉ khi, với mọi* $ i \in I $, *ánh xạ* $ g \circ f_i $ *(tương ứng $ p \circ f_i $) là liên tục trong* $ E_i $.

Đây là trường hợp riêng của mệnh đề 5, II, p. 27.

Nhắc lại định nghĩa tổng trực tiếp của một họ các không gian vectơ (A, II, p. 12, mệnh đề 6), ta có thể nói rằng tôpô $ \mathcal{T} $ là tôpô duy nhất mà đối với nó ánh xạ chính tắc $ g \mapsto (g \circ f_i) $ là một *song ánh*

$$
\mathcal{L}(E; G) \to \prod_{i \in I} \mathcal{L}(E_i; G)
$$

đối với mọi không gian lồi địa phương $ G $.

#### Hệ quả {#evt-ii-s4-n5-cor-1 .statement}

*Với ký hiệu của mệnh đề 5, II, p. 27, giả sử rằng* $ E $ *là tổng của các* $ g_\alpha(F_\alpha) $. *Gọi* $ F $ *là tổng trực tiếp tôpô của họ* $ (F_\alpha)_{\alpha \in A} $, *và gọi* $ j_\alpha : F_\alpha \to F $ *là đơn ánh chính tắc; giả sử rằng* $ g : F \to E $ *là ánh xạ tuyến tính sao cho* $ g \circ j_\alpha = g_\alpha $ *với mọi* $ \alpha \in A $. *Nếu* $ N $ *là hạt nhân của* $ g $, *thì song ánh chính tắc* $ F/N \to E $ *liên kết với* $ g $ *là một đẳng cấu tôpô từ* $ F/N $ *lên* $ E $ *được trang bị tôpô* $ \mathcal{T} $.

Đây là một trường hợp riêng của II, p. 28, hệ quả 2, nhớ đến II, p. 29, *Ví dụ I*.

#### Mệnh đề 7 {#evt-ii-s4-prop-7 .statement}

*Đơn ánh chính tắc* $ j : E \to \prod_{i \in I} E_i $ *là liên tục khi* $ E $ *mang tôpô tổng trực tiếp của các* $ E_i $ *và* $ \prod_{i \in I} E_i $ *mang tôpô tích. Khi* $ I $ *hữu hạn, ánh xạ này là một đẳng cấu của các không gian vectơ tôpô.*

Mệnh đề thứ nhất suy ra từ sự kiện rằng các đơn ánh chính tắc $ E_\kappa \to \prod_{\iota \in I} E_\iota $ là liên tục với mỗi $ \kappa \in I $. Nếu $ I $ hữu hạn thì $ j $ là ánh xạ đồng nhất, và chỉ cần chứng minh rằng tôpô tích $ \mathcal{T}' $ mịn hơn tôpô tổng trực tiếp $ \mathcal{T} $. Bây giờ, gọi $ V $ là một lân cận lồi của 0 đối với $ \mathcal{T} $; mỗi tập hợp $ V \cap E_\iota $ là một lân cận lồi của 0 trong $ E_\iota $; nếu $ n $ là số phần tử của $ I $, thì tập hợp $ V $ chứa tập hợp $ \frac{1}{n} \sum_n (V \cap E_\iota) $, là một lân cận của 0 đối với $ \mathcal{T}' $, và mệnh đề được chứng minh.

Khi $ I $ vô hạn, nếu, với mỗi tập con hữu hạn $ J $ của $ I $, ta ký hiệu bởi $ E_J $ không gian $ \prod_{\iota \in J} E_\iota $, được trang bị tôpô tích, thì $ E $ là *giới hạn quy nạp* của các $ E_J $ (được đồng nhất như các không gian con của $ E $).

#### Mệnh đề 8 {#evt-ii-s4-prop-8 .statement}

*Cho $ N_\iota $ là một không gian con của $ E_\iota $, với mọi $ \iota \in I $,*

(i) *Tôpô cảm sinh trên $ N = \sum_\iota N_\iota $ bởi tôpô tổng trực tiếp $ \mathcal{T} $ trên $ E $ là đồng nhất với tổng trực tiếp của các tôpô của các $ N_\iota $.*

(ii) *Ánh xạ chính tắc $ h $ từ không gian tổng trực tiếp tôpô của các $ E_\iota / N_\iota $ lên $ E/N $ (A, II, § 1.6, công thức (26)) là một đẳng cấu giữa các không gian vectơ tôpô.*

(i) Với các ký hiệu đã đưa vào ở trên, ta xét $ x = \sum_\iota \lambda_\iota x_\iota $ thuộc $ N \cap \Gamma((V_\iota)) $ ($ (\lambda_\iota) $ là một họ các số $ \geqslant 0 $ trong đó chỉ có hữu hạn nhiều số khác không, sao cho $ \sum_\iota \lambda_\iota = 1 $, và $ x_\iota \in V_\iota $, với mọi $ \iota \in I $). Vì tổng của các $ N_\iota $ là trực tiếp, ta có $ \lambda_\iota x_\iota \in N_\iota $ với mọi $ \iota \in I $; do đó, với mọi $ \iota $ sao cho $ \lambda_\iota > 0 $ ta cũng có $ x_\iota \in N_\iota \cap V_\iota $, và $ x $ thuộc bao lồi $ \Gamma((N_\iota \cap V_\iota)) $, vậy (i) được chứng minh.

(ii) Ký hiệu các ánh xạ chính tắc như sau: $ f_\iota : E_\iota \to E, h_\iota : E_\iota / N_\iota \to E/N, p_\iota : E_\iota \to E_\iota / N_\iota $ và $ p : E \to E/N $. Với mọi $ \iota \in I $, $ h_\iota \circ p_\iota = p \circ f_\iota $ và mệnh đề suy ra từ II, p. 28, hệ quả 2 và p. 29 *Ví dụ I*.

#### Hệ quả 1 {#evt-ii-s4-prop-8-cor-1 .statement}

*Nếu $ N_\iota $ đóng trong $ E_\iota $ với mọi $ \iota \in I $, thì $ N = \sum_\iota N_\iota $ trong $ E $ là đóng.*

Thật vậy, ánh xạ chính tắc $ p_\iota : E \to E_\iota $ là liên tục (II, § 4.5, mệnh đề 6) với mọi $ \iota \in I $, do đó $ p_\iota^{-1}(N_\iota) $ là đóng trong $ E $, và vì thế điều tương tự cũng đúng đối với giao $ N = \bigcap_{\iota \in I} p_\iota^{-1}(N_\iota) $.

#### Hệ quả 2 {#evt-ii-s4-prop-8-cor-2 .statement}

*Nếu mỗi $ E_\iota $ là Hausdorff, thì $ E $ cũng vậy và mỗi $ E_\iota $ là đóng trong $ E $.*

Để chứng minh mệnh đề thứ nhất, áp dụng hệ quả 1 bằng cách lấy $ N_\iota = \{0\} $ với mọi $ \iota \in I $; đối với mệnh đề thứ hai, áp dụng hệ quả 1 với $ N_\iota = E_\iota $ và $ N_\kappa = \{0\} $ với mọi $ \kappa \neq \iota $.

Ta sẽ chỉ ra trong III, p. 21, hệ quả 2 rằng nếu các $ E_\iota $ là Hausdorff và *đầy đủ* thì tổng trực tiếp tôpô của chúng $ E $ cũng vậy.

### 6. Giới hạn quy nạp của các dãy không gian lồi địa phương

Trong Số này, ta sẽ xét một *dãy tăng* $ (E_n) $ các không gian con vectơ của một không gian vectơ $ E $, sao cho $ E $ là *hợp* của các $ E_n $; ta giả sử rằng mỗi $ E_n $ mang một tôpô lồi địa phương $ \mathcal{T}_n $, sao cho, với mọi $ n $, tôpô cảm sinh trên $ E_n $ bởi $ \mathcal{T}_{n+1} $ là *thô hơn* $ \mathcal{T}_n $, và ta trang bị cho $ E $ tôpô lồi địa phương $ \mathcal{T} $ là *giới hạn quy nạp* của dãy $ (\mathcal{T}_n) $ (II, p. 29, *Ví dụ II*); các giả thiết và ký hiệu này sẽ được sử dụng trong toàn bộ phần còn lại của Số này mà không nhắc lại.

Có thể xảy ra rằng mỗi $ \mathcal{T}_n $ là Hausdorff nhưng $ \mathcal{T} $ thì không; cũng có thể xảy ra rằng với mỗi cặp số nguyên $ n, m $ sao cho $ n \leq m $, không gian con $ E_n $ là đóng trong $ E_m $ (sử dụng tôpô $ \mathcal{T}_m $) nhưng $ E_n $ không đóng trong $ E $ khi sử dụng $ \mathcal{T} $ (II, p. 80, Bài tập 26).

#### Bổ đề 1 {#evt-ii-s4-lem-1 .statement}

— *Cho $ \mathfrak{F} $ là một bộ lọc Cauchy trên $ E $ (đối với $ \mathcal{T} $); khi đó tồn tại một số nguyên $ k $ sao cho với mọi $ N \in \mathfrak{F} $ và mọi lân cận $ V $ của $ 0 $ trong $ E $, không gian con $ E_k $ gặp $ N + V $.*

Ta giả sử điều ngược lại và đi đến một mâu thuẫn. Giả sử rằng với mọi $ k $ tồn tại một lân cận lồi $ V_k $ của $ 0 $ và một tập hợp $ M_k \in \mathfrak{F} $ sao cho
$$
(E_k + V_k) \cap M_k = \varnothing.
$$
Rõ ràng ta có thể giả sử rằng $ V_{k+1} \subset V_k $ với mọi $ k $. Gọi $ V $ là bao lồi của $ \bigcup_k (E_k \cap V_k) $, rõ ràng đây là một lân cận của $ 0 $ đối với $ \mathcal{T} $. Với mọi $ n $ ta có $ V \subset V_n + E_n $; thật vậy, mọi $ x \in V $ có thể viết dưới dạng $ \sum_i \lambda_i x_i $ trong đó $ \lambda_i \geq 0 $, $ \sum_i \lambda_i = 1 $ và $ x_i \in V_i \cap E_i $ với mọi $ i $; với $ i < n $ ta có $ x_i \in E_n $, do đó $ \sum_{i < n} \lambda_i x_i \in E_n $; còn với $ i \geq n $ ta có $ x_i \in V_n $, do đó $ \sum_{i \geq n} \lambda_i x_i \in V_n $ vì $ V_n $ là lồi, chứa $ 0 $ và $ \sum_{i \geq n} \lambda_i \leq 1 $. Suy ra $ V + E_n \subset V_n + E_n $ với mọi $ n $. Vì vậy, lấy $ M \in \mathfrak{F} $ là một tập hợp $ V $-nhỏ. Với một số nguyên $ m $, $ E_m \cap M $ không rỗng; và ta kết luận rằng
$$
M \subset E_m + V \subset E_m + V_m;
$$
vì $ \mathfrak{F} $ là một bộ lọc, tập hợp $ M_m $ gặp $ M $ và do đó gặp $ E_m + V_m $; ta có một mâu thuẫn, chứng minh được bổ đề.

#### Mệnh đề 9 {#evt-ii-s4-prop-9 .statement}

*Giả sử tôpô cảm sinh trên $ E_n $ bởi $ \mathcal{T}_{n+1} $ là đồng nhất với $ \mathcal{T}_n $ đối với mọi số nguyên $ n $. Khi đó
(i) Tôpô cảm sinh bởi $ \mathcal{T} $ trên $ E_n $ là đồng nhất với $ \mathcal{T}_n $ đối với mỗi $ n $; nếu các $ \mathcal{T}_n $ là Hausdorff thì $ \mathcal{T} $ là Hausdorff.
(ii) Nếu, đối với mọi $ n $, $ E_n $ là đóng trong $ E_{n+1} $ (đối với $ \mathcal{T}_{n+1} $), thì $ E_n $ là đóng trong $ E $ (sử dụng $ \mathcal{T} $) đối với mọi $ n $.
(iii) Nếu mỗi $ E_n $ là đầy đủ (sử dụng $ \mathcal{T}_n $) thì $ E $ là đầy đủ sử dụng $ \mathcal{T} $.*

(i) Để chứng minh mệnh đề đầu tiên, chỉ cần chứng minh rằng tôpô $ \mathcal{T}'_n $ cảm sinh bởi $ \mathcal{T} $ trên $ E_n $ mịn hơn $ \mathcal{T}_n $. Với mục đích này, cho $ V_n $ là một lân cận lồi của $ 0 $ trong $ E_n $ đối với tôpô $ \mathcal{T}_n $; ta sẽ xây dựng một dãy tăng các lân cận lồi của $ 0 $ trong $ E_{n+p} $ đối với $ \mathcal{T}_{n+p} $, ký hiệu là $ (V_{n+p})_{p \geq 1} $, sao cho $ V_{n+p} \cap E_n = V_n $ đối với mọi chỉ số $ p \geq 1 $. Khi đó hợp $ V $ của dãy tăng $ (V_{n+p}) $ sẽ là một tập hợp lồi sao cho $ V \cap E_k $ là một lân cận của $ 0 $ trong $ E_k $ (sử dụng $ \mathcal{T}_k $), đối với mọi chỉ số $ k $; do đó $ V $ sẽ là một lân cận của $ 0 $ trong $ E $ đối với $ \mathcal{T} $ và vì $ V \cap E_n = V_n $, ta đã chứng minh rằng $ \mathcal{T}'_n $ mịn hơn $ \mathcal{T}_n $.

Để định nghĩa $ V_{n+p} $ ta tiến hành bằng quy nạp theo $ p $ sử dụng bổ đề sau:

#### Bổ đề 2 {#evt-ii-s4-lem-2 .statement}

*Cho $ V $ là một lân cận lồi của 0 trong $ M $, một không gian con vectơ của một không gian lồi địa phương $ F $. Khi đó tồn tại một lân cận lồi $ W $ của 0 trong $ F $ sao cho $ W \cap M = V $. Hơn nữa, nếu $ M $ là đóng trong $ F $, thì với mọi điểm $ x_0 \in \complement M $, tồn tại một lân cận lồi $ W_0 $ của 0 trong $ F $ sao cho $ W_0 \cap M = V $ và $ x_0 \notin W_0 $.*

Thực vậy, theo giả thiết tồn tại một lân cận lồi $ U $ của 0 trong $ F $ sao cho $ U \cap M \subset V $. Hiển nhiên, bao lồi $ W $ của $ U \cup V $ trong $ F $ là một lân cận của 0 trong $ F $; ta chứng minh rằng $ W \cap M = V $. Vì, mọi điểm $ z \in W $ đều có dạng $ \lambda x + (1-\lambda) y $ với $ x \in V, y \in U $, và $ 0 \leq \lambda \leq 1 $ (II, p. 9, Mệnh đề 8); nếu $ z \in M $, và $ \lambda \neq 1 $ thì tất nhiên $ y \in M $, do đó $ y \in U \cap M \subset V $ và suy ra $ z \in V $; điều này hiển nhiên đúng nếu $ \lambda = 1 $. Nếu $ M $ là đóng trong $ F $, thì không gian $ F/M $ là Hausdorff, do đó tồn tại một lân cận lồi $ U_0 \subset U $ của 0 trong $ F $ sao cho $ U_0 $ không giao với $ x_0 + M $; khi ấy bao lồi $ W_0 $ của $ U_0 \cup V $ thỏa các điều kiện yêu cầu.

Quay lại định lý, để chứng minh phần thứ hai của (i) chú ý rằng nếu $ x \in E $ thì $ x \in E_n $ với một $ n $ nào đó; nếu $ x \neq 0 $ và $ \mathcal{T}_n $ là Hausdorff thì có một lân cận $ V_n $ của 0 đối với $ \mathcal{T}_n $, không chứa $ x $. Ta thấy có một lân cận $ V $ của 0 đối với $ \mathcal{T} $ sao cho $ V \cap E_n = V_n $, suy ra $ x \notin V $, và do đó $ \mathcal{T} $ là Hausdorff.

(ii) Cho $ x \in E - E_n $; tồn tại $ m > n $ sao cho $ x \in E_m $, do đó, vì $ E_n $ là đóng trong $ E_m $ đối với $ \mathcal{T}_m $ (do giả thiết rằng $ \mathcal{T}_{n+1} $ cảm sinh $ \mathcal{T}_n $ trên $ E_n $ với mọi $ n $) tồn tại trong tôpô $ \mathcal{T}_m $ một lân cận lồi $ V_m $ của 0 trong $ E_m $ sao cho $ (x + V_m) \cap E_n $ là rỗng. Như đã thấy trong (i) tồn tại một lân cận lồi $ V $ của 0 đối với $ \mathcal{T} $ sao cho $ V \cap E_m = V_m $; và do đó $ (x + V) \cap E_m = x + V_m $, suy ra $ (x + V) \cap E_n = \varnothing $, điều này chứng minh (ii).

(iii) Từ bổ đề 1, nếu $ \mathfrak{F} $ là một *bộ lọc Cauchy cực tiểu* cho $ \mathcal{T} $ (GT, II, § 3.2) thì tồn tại một $ k $ sao cho vết của $ \mathfrak{F} $ trên $ E_k $ là một bộ lọc $ \mathfrak{F}_k $; từ (i) bộ lọc sau này là một bộ lọc Cauchy cho $ \mathcal{T}_k $ và do đó $ \mathfrak{F}_k $ hội tụ trong $ E_k $ theo giả thiết; nhưng vì bộ lọc trên $ E $ sinh bởi $ \mathfrak{F}_k $ mịn hơn $ \mathfrak{F} $, ta thấy rằng $ \mathfrak{F} $ có một điểm tụ đối với $ \mathcal{T} $ và do đó hội tụ đối với $ \mathcal{T} $.

Khi với mọi $ n $ tôpô cảm sinh trên $ E_n $ bởi $ \mathcal{T}_{n+1} $ chỉ là $ \mathcal{T}_n $ ta nói rằng $ \mathcal{T} $ là *giới hạn quy nạp ngặt* của dãy $ (\mathcal{T}_n) $ và rằng không gian $ E $ với tôpô $ \mathcal{T} $ là *giới hạn quy nạp ngặt* của dãy các không gian lồi địa phương $ E_n $.

#### Nhận xét {#evt-ii-s4-n6-rem-1 .statement}

— 1) Giả sử rằng $ E $ là hợp của một họ tăng có hướng, *không đếm được* các không gian con $ (E_\alpha)_{\alpha \in I} $, mỗi $ E_\alpha $ mang một tôpô lồi địa phương $ \mathcal{T}_\alpha $, sao cho, với $ E_\alpha \subset E_\beta $, tôpô cảm sinh trên $ E_\alpha $ bởi $ \mathcal{T}_\beta $ trùng với $ \mathcal{T}_\alpha $. Có thể xảy ra rằng tôpô cảm sinh trên mỗi $ E_\alpha $ bởi tôpô $ \mathcal{T} $ bằng $ \mathcal{T}_\alpha $ và rằng các $ E_\alpha $ là *Hausdorff và đầy đủ, nhưng $ E $ không đầy đủ đối với $ \mathcal{T} $* (INT, III, ấn bản 2, § 1, Bài tập 2).

2) Cho $ F $ là một không gian lồi địa phương, là hợp của một dãy tăng các không gian con vectơ $ (F_n) $, và với mỗi chỉ số $ n $, cho $ \mathcal{T}_n $ là tôpô cảm sinh trên $ F_n $ bởi tôpô $ \mathcal{T} $ của $ F $. Cần lưu ý rằng nói chung $ \mathcal{T} $ không phải là giới hạn quy nạp của các $ \mathcal{T}_n $.

3) Giả sử rằng $ E $ là giới hạn quy nạp chặt của dãy $ (E_n) $; nếu $ F $ là một không gian con vectơ đóng (trong $ \mathcal{T} $) của $ E $, thì có thể xảy ra rằng giới hạn quy nạp chặt của các tôpô cảm sinh bởi $ \mathcal{T}_n $ trên $ F \cap E_n $ *mịn hơn hẳn* tôpô cảm sinh bởi $ \mathcal{T} $ (IV, p. 63, bài tập 10).

#### Mệnh đề 10 {#evt-ii-s4-prop-10 .statement}

*Cho E, F là hai không gian lồi địa phương. Giả sử rằng :*

1) *Tồn tại một họ các không gian Fréchet* $ (E_\alpha) $, *và với mỗi* $ \alpha $ *một ánh xạ tuyến tính* $ g_\alpha : E_\alpha \to E $, *sao cho tôpô của E là tôpô lồi địa phương cuối cùng đối với họ* $ (g_\alpha) $.

2) *Tồn tại một dãy các không gian Fréchet* $ (F_n) $ *và với mỗi n một đơn ánh tuyến tính liên tục* $ j_n : F_n \to F $, *sao cho* $ F = \bigcup_n j_n(F_n) $.

*Khi đó mọi ánh xạ tuyến tính u từ E vào F, có đồ thị đóng trong* $ E \times F $, *đều tất nhiên liên tục.*

Để chứng minh rằng $ u $ liên tục, chỉ cần chứng minh rằng với mọi $ \alpha $, ánh xạ $ u \circ g_\alpha : E_\alpha \to F $ là liên tục (II, p. 27, mệnh đề 5). Bây giờ đồ thị của $ u \circ g_\alpha $ là ảnh ngược của đồ thị của $ u $ qua ánh xạ liên tục $ g_\alpha \times 1_F : E_\alpha \times F \to E \times F $, và do đó, theo giả thiết, là đóng trong $ E_\alpha \times F $. Vì vậy, ta có thể chỉ xét trường hợp E tự thân là một *không gian Fréchet*. Khi đó mệnh đề này là một trường hợp riêng của I, p. 20, mệnh đề 1.

#### Hệ quả {#evt-ii-s4-n6-cor-1 .statement}

*Với cùng các giả thiết trên E và F như trong mệnh đề 10 và giả sử E là Hausdorff, thì mọi ánh xạ toàn ánh liên tục v từ F vào E là một cấu xạ chặt.*

Cho N là hạt nhân của $ v $ và đặt $ N_n = j_n^{-1}(N) $; khi đó ánh xạ $ j'_n : F_n / N_n \to F / N $, cảm sinh từ $ j_n $ bằng cách lấy thương, là đơn ánh và liên tục; hơn nữa $ F_n / N_n $ là một không gian Fréchet (vì $ N_n $ là đóng) và $ F / N $ là hợp của các ảnh qua $ j'_n $. Theo giả thiết, trong phân tích chính tắc $ v : F \to F / N \xrightarrow{w} E $, ánh xạ tuyến tính $ w $ là song ánh và liên tục và do đó đồ thị của nó trong $ (F / N) \times E $ là *đóng* (GT, I, § 8.1, hệ quả 2 của mệnh đề 2). Theo các nhận xét ở đầu và theo mệnh đề 10, ánh xạ nghịch đảo $ u $ của $ w $ do đó liên tục và hệ quả được chứng minh.

\* Mệnh đề 10 và hệ quả của nó áp dụng đặc biệt khi E là một *không gian bornological đầy đủ* (III, p. 12) và F là giới hạn quy nạp của một dãy các không gian Fréchet. \*

### 7. Nhận xét về các không gian Fréchet

Ta sẽ xét mệnh đề 2 của GT, IX, § 3.1 trong trường hợp các không gian lồi địa phương.

#### Mệnh đề 11 {#evt-ii-s4-prop-11 .statement}

*Cho E là một không gian lồi địa phương có thể metr hóa. Tôpô của E có thể được xác định bởi một khoảng cách bất biến qua tịnh tiến, và sao cho các quả cầu mở là lồi.*

Cho $ (p_n)_{n \in \mathbf{N}} $ là một dãy các nửa chuẩn định nghĩa tôpô của E. Cho $ d_n $ là giả khoảng cách được định nghĩa bởi $ d_n(x, y) = \inf(p_n(x - y), 1/n) $ với $ x, y $ trong E; nó bất biến qua tịnh tiến. Với mọi $ n \geq 0 $, và mọi số thực $ R \geq 0 $, cho $ B_{n, R} $ là tập các $ x \in E $ sao cho $ d_n(x, 0) < R $. Nếu $ R \geq 1/n $, thì $ B_{n, R} = E $, và trong trường hợp còn lại $ B_{n, R} $ là tập các $ x \in E $ sao cho $ p_n(x) < R $; trong mọi trường hợp $ B_{n, R} $ là lồi.

Với $ x, y $ trong $ E $ ta định nghĩa $ d(x, y) = \sup_{n \in \mathbf{N}} d_n(x, y) $. Ta thấy ngay rằng $ d $ là một khoảng cách, bất biến qua các phép tịnh tiến trên $ E $ và định nghĩa tôpô của $ E $. Với $ x_0 \in E $ và $ R \geq 0 $, quả cầu mở tâm $ x_0 $ và bán kính $ R $ (đối với khoảng cách $ d $) bằng $ \bigcap_{n \in \mathbf{N}} (x_0 + B_{n, R}) $, do đó nó lồi.

#### Mệnh đề 12 {#evt-ii-s4-prop-12 .statement}

*Cho $ E $ và $ F $ là hai không gian Fréchet và $ u $ là một ánh xạ tuyến tính liên tục của $ E $ lên $ F $. Khi đó tồn tại một tiết diện của $ u $ liên tục mặc dù không nhất thiết tuyến tính.*

Theo mệnh đề 11, tồn tại một khoảng cách $ d $ trên $ E $, bất biến qua các phép tịnh tiến, định nghĩa tôpô của $ E $ và sao cho các quả cầu mở là lồi. Với $ y $ và $ y' $ trong $ F $, ký hiệu $ \delta(y, y') $ là khoảng cách giữa các tập hợp đóng $ u^{-1}(y) $ và $ u^{-1}(y') $ trong $ E $. Vì $ u $ là một cấu xạ ngặt (I, p. 17, th. 1), nhận xét của GT, IX, § 3.1 cho thấy rằng $ \delta $ là một khoảng cách trên $ F $ định nghĩa tôpô của $ F $. Ta sẽ xây dựng, bằng quy nạp, một dãy các ánh xạ liên tục $ (s_n)_{n \in \mathbf{N}} $ từ $ F $ vào $ E $ thỏa mãn các bất đẳng thức sau với mọi $ y \in F $:

$$
\delta(y, u(s_n(y))) < 2^{-n}
$$
$$
d(s_n(y), s_{n-1}(y)) < 2^{-n+1} \quad \text{(chỉ nếu } n \geq 1 \text{)}.
$$

Giả sử khi đó hoặc $ n = 0 $, hoặc $ n \geq 1 $ và rằng $ s_{n-1} $ đã được xây dựng. Lấy $ y_0 \in F $; vì $ u $ là toàn ánh, tập $ u^{-1}(y_0) $ là không rỗng, và với $ n \geq 1 $, ta có $ d(u^{-1}(y_0), s_{n-1}(y_0)) < 2^{-n+1} $ theo giả thiết quy nạp. Do đó tồn tại một điểm $ x_0 $ của $ E $ sao cho $ u(x_0) = y_0 $ và với $ n \geq 1 $, $ d(x_0, s_{n-1}(y_0)) < 2^{-n+1} $. Vì ánh xạ $ s_{n-1} $ liên tục, tập các điểm $ y $ của $ F $ thỏa mãn các bất đẳng thức $ \delta(y, y_0) < 2^{-n} $ và $ d(x_0, s_{n-1}(y)) < 2^{-n+1} $ là một lân cận mở của $ y_0 $. Suy ra tồn tại một phủ mở $ (V_i)_{i \in I} $ của $ F $ và các ánh xạ hằng $ s_{n,i} $ của $ F $ trong $ E $ thỏa mãn các bất đẳng thức (2) và (3) *trong* $ V_i $ trong đó ta thay $ s_n $ bởi $ s_{n,i} $. Vì không gian $ F $ là khả métrique, tồn tại một phân hoạch đơn vị liên tục $ (f_i)_{i \in I} $, tức là hữu hạn địa phương và phụ thuộc vào phủ $ (V_i)_{i \in I} $ (GT, IX, § 4.5, th. 4 và § 4.4, hq. 1). Với mọi $ y \in F $, đặt $ s_n(y) = \sum_{i \in I} f_i(y) \cdot s_{n,i}(y) $. Ánh xạ $ s_n $ của $ F $ trong $ E $ là liên tục; vì các quả cầu mở là lồi trong $ E $ và trong $ F $, ánh xạ $ s_n $ thỏa mãn các bất đẳng thức (2) và (3) với mọi $ y \in F $.

Từ bất đẳng thức (3) các ánh xạ $ s_n : F \to E $ tạo thành một dãy Cauchy, đối với sự hội tụ đều. Vì $ E $ đầy đủ, dãy $ (s_n)_{n \in \mathbf{N}} $ hội tụ đều về một ánh xạ liên tục $ s : F \to E $ (GT, X, § 1.6); công thức (2) cho thấy $ u \circ s $ là ánh xạ đồng nhất của $ F $, do đó $ s $ là một tiết diện liên tục của $ u $.

#### Hệ quả {#evt-ii-s4-n7-cor-1 .statement}

*Nếu $ L $ là một tập compact trong $ F $, thì tồn tại một tập compact $ K $ trong $ E $ sao cho $ u(K) = L $. \*

Đủ để đặt $ K = s(L) $, trong đó $ s $ là một tiết diện liên tục của $ u $.

#### Nhận xét {#evt-ii-s4-n7-rem-1 .statement}

— 1) Hệ quả của mđ. 12 cũng có thể suy ra từ đl. 1 của I, p. 17 và mđ. 18 của GT, IX, § 2.10.
2) Ta giữ các ký hiệu của mđ. 12. Lấy $ p $ là một nửa chuẩn liên tục trên $ E $;

Với mọi $ y \in F $, đặt $ q(y) = \inf_{u(x)=y} p(x) $, sao cho $ q $ là một nửa chuẩn liên tục trên $ F $ (II, p. 4). Cho $ \phi $ là một ánh xạ nửa liên tục dưới của $ F $ vào khoảng $ ]0, +\infty[ $ của $ \overline{\mathbf{R}} $. Ta chứng minh rằng tồn tại *một tiết diện liên tục s của u sao cho* $ p \circ s < q + \phi $.

Cho $ s_0 $ là một tiết diện liên tục của $ u $ (mệnh đề 12) và $ N $ là hạt nhân của $ u $. Lấy $ y_0 \in F $, khi đó tồn tại $ z_0 \in N $ sao cho $ p(s_0(y_0) + z_0) < q(y_0) + \phi(y_0) $. Tồn tại một lân cận mở $ W $ của $ y_0 $ trong $ F $ sao cho $ p(s_0(y) + z_0) < q(y) + \phi(y) $ với mọi $ y \in W $. Do đó tồn tại một phủ mở $ (W_i)_{i \in I} $ của $ F $ và các ánh xạ hằng $ t_i : F \to N $ sao cho $ p(s_0(y) + t_i(y)) < q(y) + \phi(y) $ với mọi $ y \in W_i $. Vì $ F $ khả metric, tồn tại một phân hoạch đơn vị liên tục hữu hạn địa phương phụ thuộc vào phủ $ (W_i)_{i \in I} $, ký hiệu là $ (g_i)_{i \in I} $ (GT, IX, § 4.5, định lý 4 và § 4.4, hệ quả 1). Ánh xạ $ s $ của $ F $ vào $ E $ được xác định bởi $ s(y) = s_0(y) + \sum_{i \in I} g_i(y) \cdot t_i(y) $ thỏa các điều kiện đã nêu.

### Bài tập {#evt-ii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
