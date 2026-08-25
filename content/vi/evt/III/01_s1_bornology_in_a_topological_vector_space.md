---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 1
section_title: Bornology in a topological vector space
lang: vi
source: evt-i-v
pdf_pages: 0133-0143, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Bornologies
      page: 0
      pdf_page: 133
    - "no": 2
      title: Bounded subsets of a topological vector space
      page: 2
      pdf_page: 134
    - "no": 3
      title: Image under a continuous mapping
      page: 4
      pdf_page: 136
    - "no": 4
      title: Bounded subsets in certain inductive limits
      page: 5
      pdf_page: 137
    - "no": 5
      title: The spaces $E_A$ (A bounded)
      page: 7
      pdf_page: 139
    - "no": 6
      title: Complete bounded sets and quasi-complete spaces
      page: 8
      pdf_page: 140
    - "no": 7
      title: Examples
      page: 9
      pdf_page: 141
statements: 30
exercises: 16
content_sha256: 670f0ecc210b3f4e72bf27defc032db9ab96fdac6d93832273e87ff746c6f976
translated_from: content/en/evt/III/01_s1_bornology_in_a_topological_vector_space.md
source_content_sha256: d71d0969533dd7f5fff98cca3d3702c7e8c3ccc31a6fa2115384c36fec2e38a7
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ef9d8679
glossary_version: 34
glossary_terms_sha256: e5d4bd9a01bcdaf1c102507e0247cf70b936bc295a3dca49e4b914cfdce864fa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. BORNÔ HỌC TRONG KHÔNG GIAN VECTƠ TÔPÔ

### 1. Các bornôlôgi

#### Định nghĩa 1 {#evt-iii-s1-def-1 .statement}

— *Một bornôlôgi trên một tập hợp* $E$ *là một tập con* $\mathcal{B}$ *của tập hợp tất cả các tập con của* $E$ *thỏa mãn các điều kiện sau* (cf. GT, X, § 1.2, Nhận xét 2).
(B1) *Mọi tập con của một tập hợp thuộc* $\mathcal{B}$ *đều thuộc* $\mathcal{B}$.
(B2) *Mọi hợp hữu hạn của các tập hợp thuộc* $\mathcal{B}$ *đều thuộc* $\mathcal{B}$.

*Ta nói rằng* $\mathcal{B}$ *là phủ nếu mọi phần tử của* $E$ *được chứa trong một tập hợp thuộc* $\mathcal{B}$, *hay, tương đương, nếu* $\mathcal{B}$ *là một phủ của* $E$.

#### Ví dụ {#evt-iii-s1-n1-exa-1 .statement}

— Cho E là một không gian metric; tập hợp tất cả các tập con bị chặn của E (GT, IX, § 2, No. 2) là một bornôlôgi phủ trên E. Cho G là nhóm các đẳng cự của E; tập hợp tất cả các tập con M của G sao cho với mọi $x \in E$, tập hợp $M.x$ là một tập con bị chặn của E, là một bornôlôgi phủ trên G.

Nếu $\mathcal{B}$ là một bornôlôgi trên một tập hợp E, một tập con $\mathcal{B}_1$ của $\mathcal{B}$ được gọi là một *cơ sở* của $\mathcal{B}$ nếu mọi tập hợp thuộc $\mathcal{B}$ đều được chứa trong một tập hợp thuộc $\mathcal{B}_1$.

Giao của một họ các bornôlôgi trên E là một bornôlôgi; do đó với mọi tập con $\mathfrak{S}$ của $\mathfrak{P}(E)$, tồn tại một bornôlôgi nhỏ nhất chứa $\mathfrak{S}$; bornôlôgi này được gọi là *sinh bởi* $\mathfrak{S}$ và nhận làm cơ sở tập hợp các hợp hữu hạn của các tập hợp thuộc $\mathfrak{S}$. Nếu E và E' là hai tập hợp, và $\mathcal{B}$ (resp. $\mathcal{B}'$) là một bornôlôgi trên E (resp. E'), bornôlôgi tích là bornôlôgi trên $E \times E'$ nhận các tập hợp $M \times M'$ làm cơ sở, trong đó $M \in \mathcal{B}$ và $M' \in \mathcal{B}'$.

#### Định nghĩa 2 {#evt-iii-s1-def-2 .statement}

*Cho $E$ là một không gian vectơ. Một bornôlôgi $\mathcal{B}$ trên $E$ được gọi là lồi nếu với mọi $X \in \mathcal{B}$ và $t \in K$, tập hợp đồng dạng $tX$ và bao lồi cân bằng $\Gamma(X)$ (II, p. 10) của $X$ đều thuộc $\mathcal{B}$.*

Nếu $X$ và $Y$ là hai tập con của $E$, ta có
$$
X + Y \subset 2\Gamma(X \cup Y)
$$
$$
\lambda X \subset t\Gamma(X) \quad \text{pour} \quad |\lambda| \leq t .
$$

Do đó, nếu $\mathcal{B}$ là một bornôlôgi lồi trên $E$, nếu $A$ là một tập con bị chặn của $K$ và nếu $X, Y$ thuộc $\mathcal{B}$, thì $X + Y \in \mathcal{B}$ và $A.X \in \mathcal{B}$.

### 2. Các tập con bị chặn của một không gian vectơ tôpô

#### Định nghĩa 3 {#evt-iii-s1-def-3 .statement}

*Cho $E$ là một không gian vectơ tôpô. Một tập con $A$ của $E$ được gọi là bị chặn nếu nó bị hấp thụ bởi mọi lân cận của $0$ trong $E$ (I, p. 7, def. 4).*

Để $A$ bị chặn, điều kiện đủ là $A$ được hấp thụ bởi mọi lân cận của một hệ lân cận cơ bản của $0$. Vì tồn tại một hệ lân cận cơ bản cân bằng của $0$ (I, p. 7, prop. 4), điều này tương đương với việc nói rằng, với mọi lân cận $V$ của $0$ trong $E$, tồn tại $\lambda \in K$ sao cho $A \subset \lambda V$.

Giả sử tôpô của $E$ được xác định bởi một hệ $\Gamma$ các nửa chuẩn (II, p. 3); khi đó một tập con $A$ của $E$ bị chặn khi và chỉ khi mọi nửa chuẩn $p \in \Gamma$ đều bị chặn trên $A$.

Đặc biệt, nếu $E$ là một không gian nửa chuẩn, một tập con $A$ của $E$ bị chặn khi và chỉ khi nó được chứa trong một quả cầu. Nói cách khác, nếu $E$ là không gian chuẩn thì điều này có nghĩa là $A$ bị chặn đối với cấu trúc không gian mêtric của $E$ (GT, IX, § 2, No. 2).

#### Nhận xét {#evt-iii-s1-n2-rem-1 .statement}

— 1) Nếu $E$ là một không gian nửa chuẩn, các quả cầu tạo thành một hệ lân cận cơ bản bị chặn của $0$ trong $E$. Đảo lại, nếu $E$ là một không gian vectơ tôpô lồi địa phương, và nếu tồn tại một lân cận bị chặn của $0$ trong $E$, thì lân cận này chứa một lân cận lồi cân bằng $W$, và hàm gauge của $W$ khi đó là một nửa chuẩn xác định tôpô của $E$.

Do đó, nếu $E$ là lồi địa phương và mêtric hóa được, và nếu tôpô của nó không thể được xác định bởi một chuẩn duy nhất, thì không tồn tại khoảng cách nào trên $E$ xác định tôpô của nó và sao cho các tập con bị chặn đối với $d$ (GT, IX, § 2, No. 2) chính là các tập con bị chặn của $E$. Chính xác hơn, với mọi khoảng cách $d$ trên $E$, bất biến qua phép tịnh tiến và xác định tôpô của $E$, các tập con bị chặn của $E$ đều bị chặn đối với $d$ (III, p. 38, exerc. 3), nhưng đảo lại là sai.

2) Cho $M$ là một không gian con vectơ của $E$ được trang bị tôpô cảm sinh. Để một tập con của $M$ bị chặn trong $M$, điều kiện cần và đủ là nó bị chặn trong $E$.

3) Cho $N$ là giao của tất cả các lân cận của $0$ trong $E$, sao cho $\tilde{E} = E/N$ là không gian vectơ Hausdorff liên kết với $E$. Khi đó $N$ bị chặn; nếu $\pi : E \to \tilde{E}$ là đồng cấu chính tắc thì một tập con $B$ của $E$ bị chặn khi và chỉ khi $\pi(B)$ bị chặn.

4) Cho $E$ là một không gian lồi địa phương Hausdorff; khi đó với mọi $x \neq 0$ trong $E$, tồn tại một nửa chuẩn liên tục $p$ sao cho $p(x) \neq 0$; nửa chuẩn này không bị chặn trên nửa đường thẳng thực $\mathbf{R}_+ . x$ sinh bởi $x$. Do đó không có không gian con khác không nào của $E$ là bị chặn. Đặc biệt, một tập con bị chặn không chứa đường thẳng nào.

#### Định nghĩa 4 {#evt-iii-s1-def-4 .statement}

*Cho $E$ là một không gian lồi địa phương. Một bornology $\mathcal{B}$ trên $E$ được gọi là thích nghi với $E$, nếu nó lồi, gồm các tập con bị chặn của $E$ và nếu bao đóng của mọi tập hợp thuộc $\mathcal{B}$ cũng thuộc $\mathcal{B}$.*

#### Mệnh đề 1 {#evt-iii-s1-prop-1 .statement}

*Cho $E$ là một không gian lồi địa phương. Tập hợp các tập con bị chặn của $E$ là một bornology thích nghi.*

Ta cần thiết lập các tính chất sau:
$a)$ Nếu $B$ là một tập con bị chặn của $E$, mọi tập con của $B$ đều bị chặn.
$b)$ Hợp của hai tập con bị chặn là bị chặn.
$c)$ Mọi tập hợp đồng dạng với một tập bị chặn đều bị chặn.
$d)$ Bao lồi cân bằng đóng (II, p. 13) của một tập con bị chặn là bị chặn.
Nếu $p$ là một nửa chuẩn liên tục trên $E$, các quả cầu của $p$ là lồi, cân bằng, đóng và tập hợp đồng dạng với một quả cầu là một quả cầu. Do đó, nếu $p$ bị chặn trên hai tập con $X$ và $Y$ của $E$, thì nó cũng bị chặn trên bao lồi cân bằng đóng của $X \cup Y$, và trên các tập hợp đồng dạng với chúng. Điều này thiết lập các tính chất $b), c)$ và $d)$, còn $a)$ là hiển nhiên.

#### Định nghĩa 5 {#evt-iii-s1-def-5 .statement}

*Cho $E$ là một không gian lồi địa phương. Tập hợp tất cả các tập con bị chặn của $E$ được gọi là bornology chính tắc của $E$.*

Nếu $\mathcal{B}$ là một tập hợp các tập con bị chặn của $E$, thì tồn tại một bornology nhỏ nhất $\tilde{\mathcal{B}}$ thích nghi với $E$ và chứa $\mathcal{B}$. Các tập hợp của $\tilde{\mathcal{B}}$ là những tập được chứa trong một tập hợp đồng dạng với bao lồi cân bằng đóng của một hợp hữu hạn các tập hợp thuộc $\mathcal{B}$.

Mọi bornology thích nghi đều được chứa trong bornology chính tắc.

#### Mệnh đề 2 {#evt-iii-s1-prop-2 .statement}

*Trong một không gian lồi địa phương $E$, mọi tập tiền compact đều bị chặn.*
Cho $A$ là một tập con tiền compact của $E$, và $V$ là một lân cận lồi cân bằng của $0$. Tồn tại một dãy hữu hạn $(a_i)_{1 \leq i \leq n}$ các điểm của $A$ sao cho
$$
A \subset \bigcup_{1 \leq i \leq n} (a_i + V).
$$
Vì $B = \{a_1, ..., a_n\}$ bị chặn, tồn tại một vô hướng $\lambda$ sao cho $0 < \lambda < 1$ và $\lambda B \subset V$; ta có $\lambda A \subset \lambda B + \lambda V \subset V + V$, từ đó suy ra mệnh đề.

#### Hệ quả {#evt-iii-s1-n2-cor-1 .statement}

*Trong một không gian lồi địa phương, tập hợp các điểm của một dãy Cauchy là bị chặn.*
Thực vậy, tập hợp này là tiền compact (GT, II, § 4, No. 2).

#### Nhận xét 5 {#evt-iii-s1-n2-rem-5 .statement}

— Nói chung các tập con bị chặn của một không gian lồi địa phương $E$ không phải tất cả đều là tiền compact (ví dụ, nếu $E$ là một không gian định chuẩn vô hạn chiều, quả cầu đơn vị của nó không compact (I, p. 15, th. 3)). Tuy nhiên, điều này đúng nếu $E$ là một không gian yếu (II, p. 42) : vì không gian vectơ tôpô Hausdorff liên kết với E khi đó đẳng cấu với một không gian con của một tích K^l mà các tập con bị chặn của nó là tiền compact (*cf.* III, p. 4, cor. 2).
Về các ví dụ khác, xem IV, p. 18.

#### Mệnh đề 3 {#evt-iii-s1-prop-3 .statement}

— *Cho A là một tập con của một không gian lồi địa phương E. Giả sử rằng A bị chặn; khi đó với mọi dãy (x_n) các điểm của A và với mọi dãy (\lambda_n) các vô hướng tiến tới 0, dãy (\lambda_n x_n) tiến tới 0. Ngược lại, nếu tồn tại một dãy (\lambda_n) các vô hướng khác không sao cho với mọi dãy (x_n) các điểm của A, dãy (\lambda_n x_n) bị chặn, thì A bị chặn.*

Giả sử rằng A bị chặn. Nếu (\lambda_n) là một dãy các vô hướng tiến tới 0, và V là một lân cận của 0, ta có \lambda_n A \subset V khi n đủ lớn, và mệnh đề đầu tiên suy ra.

Ngược lại, nếu A không bị chặn và nếu (\lambda_n) là một dãy các vô hướng \neq 0, thì tồn tại một nửa chuẩn liên tục p và một dãy (x_n) các điểm của A, sao cho $p(x_n) \geq \frac{n}{|\lambda_n|}$. Khi đó ta có $p(\lambda_n x_n) \geq n$, và dãy (\lambda_n x_n) không bị chặn.

#### Hệ quả {#evt-iii-s1-n2-cor-2 .statement}

— *Một tập con A của E bị chặn khi và chỉ khi mọi tập con đếm được của A đều bị chặn.*

### 3. Ảnh qua một ánh xạ liên tục

#### Mệnh đề 4 {#evt-iii-s1-prop-4 .statement}

— *Cho E và F là hai không gian lồi địa phương và f : E \to F là một ánh xạ liên tục. Giả sử rằng f(0) = 0 và tồn tại một số thực m \geq 0 sao cho f(\lambda x) = \lambda^m f(x) với mọi \lambda > 0. Khi đó, nếu A là một tập con bị chặn của E, f(A) bị chặn trong F.*

Thật vậy, nếu V là một lân cận của 0 trong F, thì $f^{-1}(V)$ là một lân cận của 0 trong E. Nếu A bị chặn trong E, tồn tại \lambda > 0 sao cho A \subset \lambda f^{-1}(V) và điều này suy ra rằng $f(A) \subset \lambda^m V$.

#### Hệ quả 1 {#evt-iii-s1-prop-4-cor-1 .statement}

— *Cho E và F là hai không gian lồi địa phương, và u : E \to F là một ánh xạ tuyến tính liên tục. Nếu A là một tập con bị chặn của E, thì u(A) bị chặn trong F.*

#### Hệ quả 2 {#evt-iii-s1-prop-4-cor-2 .statement}

— *Cho E = \prod_{i \in I} E_i là tích của một họ các không gian lồi địa phương. Khi đó một tập con của E bị chặn khi và chỉ khi tất cả các phép chiếu của nó đều bị chặn.*

Nói chung hơn :

#### Hệ quả 3 {#evt-iii-s1-prop-4-cor-3 .statement}

— *Cho E là một không gian vectơ, (F_i)_{i \in I} là một họ các không gian lồi địa phương và f_i là một ánh xạ tuyến tính từ E vào F_i (với i \in I). Giả sử E được trang bị tôpô thô nhất (lồi địa phương) sao cho mọi f_i đều liên tục (II, p. 26). Khi đó, để một tập con A của E bị chặn, điều kiện cần và đủ là f_i(A) bị chặn trong F_i với mọi i \in I.*

Thật vậy, nếu A bị chặn, các f_i(A) cũng vậy (hệ quả 1). Ngược lại, nếu các f_i(A) bị chặn và nếu p là một nửa chuẩn liên tục trên E, thì tồn tại một tập con hữu hạn J của I và một họ $(q_j)_{j \in J}$, trong đó $q_j$ là một nửa chuẩn liên tục trên $F_j$, sao cho $p \leq \sup_{j \in J} (q_j \circ f_j)$ do đó p bị chặn trên A.

#### Hệ quả 4 {#evt-iii-s1-prop-4-cor-4 .statement}

*Cho $E_i$ ($1 \leq i \leq n$) và $F$ là các không gian lồi địa phương, và $f$ là một ánh xạ đa tuyến tính liên tục từ $\prod_{i=1}^n E_i$ vào $F$. Nếu $B_i$ là một tập con bị chặn của $E_i$, với $1 \leq i \leq n$, thì $f(\prod_{i=1}^n B_i)$ bị chặn trong $F$.*

#### Hệ quả 5 {#evt-iii-s1-prop-4-cor-5 .statement}

*Cho $E$ và $F$ là hai không gian lồi địa phương và $u : E \to F$ là một ánh xạ đa thức liên tục. Nếu $A$ là một tập con bị chặn của $E$, thì $u(A)$ bị chặn.*

### 4. Các tập con bị chặn trong một số giới hạn quy nạp

#### Mệnh đề 5 {#evt-iii-s1-prop-5 .statement}

*Cho $(E_i)_{i \in I}$ là một họ các không gian lồi địa phương Hausdorff, và cho E là tổng trực tiếp tôpô của họ này (II, p. 29). Để một tập con $B$ của $E$ bị chặn, điều kiện cần và đủ là tồn tại một tập con hữu hạn $J$ của $I$ sao cho $\operatorname{pr}_i(B)$ bị chặn trong $E_i$ với $i \in J$ và $\operatorname{pr}_i(B) \subset \{0\}$ với mọi $i \notin J$.*

Cho $J$ là một tập con hữu hạn của $I$. Vì tôpô của $E$ cảm sinh tôpô tích trên $\prod_{j \in J} E_j$ (II, p. 30, prop. 7 và p. 31, prop. 8), nên từ III, p. 4, cor. 2 suy ra rằng điều kiện là đủ.

Ngược lại, cho $B$ là một tập con bị chặn của $E$. Khi đó $\operatorname{pr}_i(B)$ bị chặn với mọi $i$ (III, p. 4, hệ quả 1). Do đó chỉ cần chứng minh rằng tồn tại một tập con hữu hạn $J$ của $I$ sao cho $\operatorname{pr}_i(B) \subset \{0\}$ với mọi $i \notin J$. Nếu không, thì tồn tại một dãy vô hạn $(i_n)$ gồm các phần tử phân biệt của $I$ và một dãy vô hạn $(x_n)$ gồm các phần tử của $B$ sao cho $\operatorname{pr}_{i_n}(x_n) \neq 0$. Vì $E_{i_n}$ là Hausdorff, tồn tại một nửa chuẩn liên tục $p_n$ trên $E_{i_n}$ sao cho $p_n(\operatorname{pr}_{i_n}(x_n)) \geq n$. Do đó $p = \sum_{n \geq 1} p_n \circ \operatorname{pr}_{i_n}$ là một nửa chuẩn liên tục trên $E$ và $p$ không bị chặn trên $B$, đây là một mâu thuẫn.*

#### Mệnh đề 6 {#evt-iii-s1-prop-6 .statement}

*Một $E$ là một không gian lồi địa phương là giới hạn quy nạp ngặt của một dãy tăng $(E_n)$ các không gian con vectơ đóng của $E$ (II, p. 33). Một tập con $B$ của $E$ bị chặn khi và chỉ khi nó được chứa trong một trong các không gian con $E_n$, và bị chặn trong không gian con này.

Điều kiện là đủ, vì tôpô cảm sinh trên $E_n$ bởi tôpô của $E$ chính xác là tôpô đã cho của $E_n$ (II, p. 32, mệnh đề 9). Để thấy rằng điều kiện là cần thiết, chỉ cần (III, p. 4, mệnh đề 3) chứng minh rằng nếu một dãy $(x_m)$ các điểm của $E$ không được chứa trong bất kỳ không gian con nào $E_n$, thì nó không thể tiến tới 0. Bằng cách trích ra một dãy con của dãy $(x_m)$, ta có thể giả sử rằng tồn tại một dãy tăng ngặt $(n_k)$ các số nguyên sao cho, với mỗi chỉ số $k$, ta có $x_k \notin E_{n_k}$ và $x_k \in E_{n_{k+1}}$. Khi đó tồn tại (II, p. 33, bổ đề 2) một dãy tăng $(V_k)$ các tập lồi sao cho $V_k$ là một lân cận của 0 trong $E_{n_k}$, $V_{k+1} \cap E_{n_k} = V_k$ và sao cho $x_k \notin V_{k+1}$ với mọi chỉ số $k$. Hợp $V$ của các $V_k$ khi đó là một lân cận của 0 trong $E$, và ta có $x_k \notin V$ với mọi $k$. Điều này chứng minh rằng dãy $(x_k)$ không tiến tới 0.*

Kết luận của mệnh đề 6 không nhất thiết đúng đối với một không gian $E$ là giới hạn quy nạp của một tập có hướng không đếm được gồm các không gian con đóng của $E$ (xem III, p. 38, bài tập 7).

#### Mệnh đề 7 {#evt-iii-s1-prop-7 .statement}

— Cho $(E_n)_{n \geq 0}$ là một dãy các không gian lồi địa phương Hausdorff, và với mọi $n$, cho $u_n : E_n \to E_{n+1}$ là một ánh xạ tuyến tính đơn ánh và compact (nghĩa là tồn tại một lân cận của 0 trong $E_n$ mà ảnh của nó qua $u_n$ là tương đối compact; điều này suy ra rằng $u_n$ liên tục). Cho $E$ là giới hạn quy nạp của hệ $(E_n, u_n)$ (II, p. 29), và cho $v_n$ là ánh xạ chính tắc từ $E_n$ vào $E$. Khi đó không gian lồi địa phương $E$ là Hausdorff. Hơn nữa, với mọi tập con $A$ của $E$, các điều kiện sau là tương đương :
(i) $A$ bị chặn;
(ii) tồn tại một số nguyên $n$ sao cho $A$ là ảnh qua $v_n$ của một tập con bị chặn của $E_n$;
(iii) $A$ là tương đối compact.
Ta đồng nhất $E_n$ với một không gian con vectơ của $E$ (được trang bị một tôpô mịn hơn tôpô cảm sinh).

#### Bổ đề 1 {#evt-iii-s1-lem-1 .statement}

Dưới giả thiết của mệnh đề 7, tôpô của $E$ là tôpô mịn nhất mà đối với nó mọi ánh xạ $v_n : E_n \to E$ đều liên tục.

Ta phải chứng minh rằng, nếu $U$ là một tập con của $E$ sao cho $U \cap E_n$ là mở trong $E_n$ với mọi $n$, thì $U$ là mở trong $E$; nói cách khác, ta phải chứng minh rằng, với mọi $x \in U$, tồn tại một tập hợp *lồi cân bằng* $V$ sao cho $x + V \subset U$ và $V \cap E_n$ là một lân cận của 0 trong $E_n$ với mọi $n$ đủ lớn (II, p. 27, prop. 5). Với mỗi $n$, gọi $W_n$ là một lân cận lồi cân bằng của 0 trong $E_n$ sao cho bao đóng $H_n$ của $W_n$ trong $E_{n+1}$ là compact. Lấy $x \in U$ và gọi $n_0$ là một số nguyên sao cho $x \in E_{n_0}$. Ta sẽ xây dựng, bằng quy nạp, một dãy $(\varepsilon_n)_{n \geq 0}$ các vô hướng $> 0$ sao cho $x + \sum_{n_0 \leq i \leq n} \varepsilon_i H_i$ được chứa trong $U$ với $n \geq n_0$. Giả sử rằng các $\varepsilon_i$ với $i < n$ đã được xây dựng. Nếu $n = n_0$, đặt $V_{n-1} = \{0\}$; nếu không, đặt
$$
V_{n-1} = \sum_{n_0 \leq i \leq n-1} \varepsilon_i H_i.
$$
Khi đó $V_{n-1}$ là compact trong $E_n$, và *a fortiori* trong $E_{n+1}$. Vì $U \cap E_{n+1}$ là mở trong $E_{n+1}$, tồn tại một vô hướng $\varepsilon_n > 0$ sao cho $x + V_n = x + V_{n-1} + \varepsilon_n H_n$ được chứa trong $U$ (GT, II, § 4, No. 3, hệ quả). Đặt $V = \bigcup_{n \geq n_0} V_n$. Khi đó $V$ lồi và cân bằng; với $n \geq n_0$, ta có $V \cap E_n \supset \varepsilon_n H_n \cap E_n \supset \varepsilon_n W_n$, do đó $V \cap E_n$ là một lân cận của 0 trong $E_n$. Điều này hoàn thành chứng minh của bổ đề.

Tập hợp $U = E - \{0\}$ là sao cho tập hợp $U \cap E_n = E_n - \{0\}$ là mở trong $E_n$ với mọi $n$, do đó $U$ là mở trong $E$, điều này chứng minh rằng $E$ là Hausdorff (GT, III, § 1, No. 3, prop. 2). Rõ ràng tính chất (ii) kéo theo (iii) và (iii) kéo theo (i). Cuối cùng ta chứng minh rằng (i) kéo theo (ii). Để làm điều này, chỉ cần chứng minh rằng nếu một tập con $A$ của $E$ không bị hấp thụ bởi bất kỳ tập hợp nào trong các tập $\sum_{0 \leq i \leq n} H_i$, thì $A$ không bị chặn. Nhưng khi đó tồn tại một dãy $(x_n)_{n \geq 1}$ các điểm của $A$ sao cho, với mọi $n$, ta có $x_n \notin n^2 \sum_{0 \leq i \leq n} H_i$.

Khi đó tập hợp của các $x_n / n$ là đóng theo bổ đề 1, vì giao của nó với $E_m$ là rời rạc với mọi số nguyên $m$. Phần bù của tập hợp các $x_n / n$ khi đó là một lân cận mở của 0 không hấp thụ dãy $(x_n)$, do đó $A$ không bị chặn.

#### Nhận xét 1 {#evt-iii-s1-n4-rem-1 .statement}

Với các ký hiệu trên, cho $F_n$ là không gian vectơ sinh bởi $H_n$, với một chuẩn bằng gauge của $H_n$. Ta sẽ thấy (III, p. 8, cor.) rằng $F_n$ là một không gian Banach. Đơn ánh từ $F_n$ vào $E_{n+1}$ là compact, do đó *a fortiori* đơn ánh $w_n$ từ $F_n$ vào $F_{n+1}$ cũng vậy. Hơn nữa, $E$ là *giới hạn quy nạp của hệ quy nạp* $(F_n, w_n)$ *của các không gian Banach*. Thật vậy, một lân cận lồi cân bằng $V$ của 0 trong $E$ là sao cho $V \cap E_n$ hấp thụ $H_{n-1}$ với mọi $n \geq 1$, và ngược lại, nếu một tập lồi cân bằng $W$ trong $E$ là sao cho $W \cap E_n$ hấp thụ $H_{n-1}$, thì $W \cap E_{n-1}$ chứa một tập đồng dạng với $W_{n-1}$ với mọi $n \geq 1$, và do đó $W$ là một lân cận của 0 trong $E$.

#### Nhận xét 2 {#evt-iii-s1-n4-rem-2 .statement}

Cho $F$ là một không gian lồi địa phương, $k$ một số nguyên $\geq 0$ và $f : E^k \to F$ một ánh xạ đa tuyến tính. Để $f$ liên tục, điều kiện cần và đủ là hạn chế của $f$ trên $E_n^k$ liên tục với mọi $n$. Ta kiểm tra ngay lập tức rằng $E^k$ có tôpô lồi địa phương cuối đối với họ các ánh xạ tuyến tính $v_n \times \cdots \times v_n : E_n \times \cdots \times E_n \to E \times \cdots \times E$ (II, p. 28, cor. 2 and p. 30, prop. 7) và rằng $u_n \times \cdots \times u_n$ là một ánh xạ tuyến tính đơn ánh compact từ $(E_n)^k$ vào $(E_{n+1})^k$. Bây giờ chỉ cần áp dụng bổ đề 1.

### 5. Các không gian $E_A$ (A bị chặn)

Cho $E$ là một không gian lồi địa phương và $A$ là một tập con lồi cân bằng của $E$. Ta nhắc lại rằng $E_A$ ký hiệu không gian vectơ sinh bởi $A$, với $p_A$ là hàm gauge của $A$, như là nửa chuẩn (II, p. 26, *Ví dụ 3*). Ta kiểm tra ngay lập tức rằng đơn ánh chính tắc của $E_A$ vào $E$ là liên tục khi và chỉ khi $A$ bị chặn. Nếu thêm vào đó $E$ là Hausdorff, một tập hợp bị chặn $A$ không chứa một đường thẳng (III, p. 2, *Nhận xét 4*) và do đó $p_A$ là một chuẩn (II, *loc. cit.*).

Ta sẽ nói rằng một không gian đều $X$ là *nửa đầy đủ* nếu mọi dãy Cauchy trong $X$ đều hội tụ. Một không gian đều đầy đủ là nửa đầy đủ; nhưng điều đảo lại không phải lúc nào cũng đúng (GT, II, § 4, exerc. 4); tuy nhiên, một không gian nửa đầy đủ khả mêtric là đầy đủ (GT, IX, § 2, No. 6, prop. 9).

#### Mệnh đề 8 {#evt-iii-s1-prop-8 .statement}

*Cho $E$ là một không gian lồi địa phương Hausdorff và cho $A$ là một tập con đóng, cân bằng, bị chặn và lồi của $E$. Cho $(x_n)$ là một dãy Cauchy trong $E_A$. Khi đó dãy này hội tụ trong $E_A$ khi và chỉ khi nó hội tụ trong $E$.*

Đơn ánh chính tắc từ $E_A$ vào $E$ là liên tục. Do đó, nếu $(x_n)$ hội tụ trong $E_A$, thì nó hội tụ trong $E$. Ngược lại, giả sử $(x_n)$ hội tụ về $y$ trong $E$. Tồn tại một dãy tăng các số nguyên $(n_k)$ sao cho $p_A(x_m - x_n) \leq 2^{-k-1}$ nếu $m \geq n_k$ và $n \geq n_k$. Do đó dãy $(x_{n_k} + 2^{-k}A)$ là giảm. Vì $A$ đóng trong $E$, ta có $y \in \bigcap_k (x_{n_k} + 2^{-k}A)$, điều này chứng minh rằng $(x_{n_k})$, do đó $(x_n)$, hội tụ về $y$ trong $E_A$.

#### Hệ quả {#evt-iii-s1-n5-cor-1 .statement}

— *Nếu A là nửa đầy đủ (đặc biệt là đầy đủ) thì E_A là một không gian Banach.*
    Thật vậy, một dãy Cauchy trong E_A cũng là một dãy Cauchy đối với tôpô của E và được chứa trong một tập đồng dạng với A, do đó hội tụ trong E.

### 6. Các tập hợp bị chặn đầy đủ và các không gian gần đầy đủ

#### Định nghĩa 6 {#evt-iii-s1-def-6 .statement}

— *Một không gian lồi địa phương E được gọi là gần đầy đủ nếu mọi tập con đóng và bị chặn của E đều đầy đủ (đối với cấu trúc đều cảm sinh bởi cấu trúc đều của E).*
    Một không gian lồi địa phương đầy đủ là gần đầy đủ, nhưng điều đảo lại không phải lúc nào cũng đúng. *Ví dụ, nếu E là một không gian Hilbert vô hạn chiều, hoặc tổng quát hơn, một không gian Banach phản xạ vô hạn chiều, thì E với tôpô yếu hơn của nó là gần đầy đủ nhưng không đầy đủ (II, p. 51, prop. 9).*
    Một không gian gần đầy đủ là nửa đầy đủ, vì mọi dãy Cauchy đều được chứa trong một tập đóng và bị chặn (III, p. 3, hệ quả và prop. 1). Đặc biệt, một không gian lồi địa phương khả mêtric và gần đầy đủ là đầy đủ.
    Trong một không gian gần đầy đủ Hausdorff, bao đóng và bao lồi cân bằng đóng của một tập con tiền compact là compact; thực ra, chúng là tiền compact (II, p. 25, prop. 3), và đầy đủ vì đóng và bị chặn (III, p. 3, prop. 2).

#### Mệnh đề 9 {#evt-iii-s1-prop-9 .statement}

— (i) *Một không gian con vectơ đóng của một không gian lồi địa phương gần đầy đủ là gần đầy đủ.*
    (ii) *Tích của các không gian lồi địa phương gần đầy đủ là gần đầy đủ.*
    (iii) *Tổng trực tiếp tôpô của các không gian lồi địa phương gần đầy đủ là gần đầy đủ.*
    (iv) *Một không gian lồi địa phương là giới hạn quy nạp ngặt của một dãy các không gian con gần đầy đủ đóng thì là gần đầy đủ.*
    Mệnh đề (i) suy ra từ *Nhận xét 2* (III, p. 2), (ii) từ III, p. 4, cor. 2, (iii) từ prop. 5 (III, p. 5) và (iv) từ prop. 6 (III, p. 5).

    Ta sẽ thấy sau này rằng không gian thương của một không gian lồi địa phương gần đầy đủ theo một không gian vectơ đóng không nhất thiết là gần đầy đủ (IV, p. 63, exerc. 10).

#### Mệnh đề 10 {#evt-iii-s1-prop-10 .statement}

— *Cho E là một không gian lồi địa phương, M là một không gian con vectơ của E sao cho mọi điểm của E đều thuộc bao đóng của một tập con bị chặn của M. Khi đó mọi ánh xạ tuyến tính liên tục f từ M vào một không gian lồi địa phương Hausdorff gần đầy đủ F đều duy nhất mở rộng thành một ánh xạ tuyến tính liên tục từ E vào F.*
    Giả thiết suy ra rằng M trù mật trong E, do đó f duy nhất mở rộng thành một ánh xạ tuyến tính liên tục $\hat{f}$ từ E vào phần bù $\hat{F}$ của F (GT, III, § 3, No. 4, corollary). Nhưng mọi $x \in F$ đều thuộc bao đóng của một tập con bị chặn B của M; do đó $\hat{f}(x)$ thuộc bao đóng của $f(B)$ trong $\hat{F}$. Nhưng $f(B)$ bị chặn trong F, do đó bao đóng của nó trong F là đầy đủ, và trùng với bao đóng của nó trong $\hat{F}$. Điều này chứng minh rằng $\hat{f}(x) \in F$.

### 7. Các ví dụ

a) Cho X là một không gian tôpô. Cho $\mathcal{R}(X)$, không gian vectơ của các hàm số (hữu hạn) trên X, được trang bị tôpô hội tụ compact (GT, X, § 1, No. 3): đây là tôpô thô nhất mà các ánh xạ hạn chế $\mathcal{R}(X) \to \mathcal{R}(H)$ là liên tục (trong đó H chạy qua họ các tập con compact của X và $\mathcal{R}(H)$ được trang bị tôpô hội tụ đều). Hệ quả 3 của III, p. 4 cho thấy rằng một tập con A của $\mathcal{R}(X)$ bị chặn khi và chỉ khi, với mọi tập con compact H của X, tập hợp các hạn chế lên H của các hàm thuộc A bị chặn đều.

*b) (Các không gian của các hàm khả vi vô hạn.) Cho $n \geqslant 1$ là một số nguyên. Với mọi tập mở U trong $\mathbf{R}^n$, ký hiệu $\mathcal{C}^\infty(U)$ là không gian vectơ của các hàm khả vi vô hạn trên U (VAR, R, 2.3). Cho f thuộc $\mathcal{C}^\infty(U)$. Với mọi đa chỉ số $\alpha = (\alpha_1, ..., \alpha_n)$ thuộc $\mathbf{N}^n$, $\partial^\alpha f$ ký hiệu đạo hàm riêng $\partial^{|\alpha|} f / \partial x_1^{\alpha_1} ... \partial x_n^{\alpha_n}$; đây là một hàm liên tục trên U (VAR, R, 2.3 và 2.4). Với mọi số nguyên $m \geqslant 0$, và mọi tập con compact H của U, đặt

$$
p_{m,H}(f) = \sup_{\substack{|\alpha| \leqslant m \\ x \in H}} |\partial^\alpha f(x)| .
$$

Khi đó $p_{m,H}$ là một nửa chuẩn trên $\mathcal{C}^\infty(U)$.

Trang bị cho $\mathcal{C}^\infty(U)$ tôpô được xác định bởi các nửa chuẩn $p_{m,H}$. Đây là tôpô thô nhất sao cho các ánh xạ $f \to \partial^\alpha f$ từ $\mathcal{C}^\infty(U)$ vào $\mathcal{R}(U)$ là liên tục, trong đó $\mathcal{R}(U)$ được trang bị tôpô hội tụ compact. Tồn tại một dãy tăng các tập con compact $(H_n)_{n \geqslant 0}$ của U mà các phần trong của chúng phủ U; họ các nửa chuẩn $p_{m,H_n}$ xác định tôpô của $\mathcal{C}^\infty(U)$, khi đó nó trở thành một không gian lồi địa phương mêtric hóa được. Không gian $\mathcal{C}^\infty(U)$ là đầy đủ; nói cách khác, nó là một không gian Fréchet (II, p. 24): thực vậy, cho $(f_k)$ là một dãy Cauchy trong $\mathcal{C}^\infty(U)$; với mọi $\alpha \in \mathbf{N}^n$, dãy $(\partial^\alpha f_k)$ hội tụ trong không gian đầy đủ $\mathcal{R}(U)$ (TG, X, § 1, No. 5, th. 1) tới một hàm liên tục $g_\alpha$. Bằng quy nạp theo $|\alpha|$, ta suy ra từ th. 1 của FVR, II, p. 2 rằng $g_\alpha = \partial^\alpha g_0$ với mọi $\alpha \in \mathbf{N}^n$. Nói cách khác, dãy $(f_k)$ hội tụ tới $g_0$ trong $\mathcal{C}^\infty(U)$.

Cho A là một tập con của $\mathcal{C}^\infty(U)$. Để A bị chặn, điều kiện cần và đủ là số $\sup_{f \in A} p_{m,H}(f)$ hữu hạn với mọi số nguyên $m \geqslant 0$ và mọi tập con compact H của U; điều kiện này có nghĩa là với mọi $\alpha \in \mathbf{N}^n$, tập hợp các hàm $\partial^\alpha f|H$ với $f \in A$ bị chặn đều với mọi compact $H \subset U$.

Cho $H \subset U$ là compact. Ta ký hiệu $\mathcal{C}_H^\infty(U)$ là không gian con của $\mathcal{C}^\infty(U)$ gồm những hàm có giá nằm trong H. Không gian $\mathcal{C}_c^\infty(U)$ của các hàm khả vi vô hạn có giá compact trong U là hợp tăng có hướng của các không gian con $\mathcal{C}_H^\infty(U)$ khi H chạy qua họ các tập con compact của U. Mỗi không gian $\mathcal{C}_H^\infty(U)$ được trang bị tôpô cảm sinh bởi tôpô của $\mathcal{C}^\infty(U)$, và $\mathcal{C}_c^\infty(U)$ với tôpô giới hạn quy nạp tương ứng. Nếu các tập $H_n$ sao cho các phần trong của chúng lập thành một phủ của U, thì không gian $\mathcal{C}_c^\infty(U)$ là giới hạn quy nạp ngặt của các không gian Fréchet $\mathcal{C}_{H_n}^\infty(U)$; do đó nó đầy đủ (II, p. 32, prop. 9) và mọi tập con bị chặn của $\mathcal{C}_c^\infty(U)$ được chứa trong một trong các không gian con $\mathcal{C}_{H_n}^\infty(U)$ (III, p. 5, prop. 6). \*

c) (Các không gian Gevrey.) Cho I là một khoảng compact trong $\mathbf{R}$. Với mọi số nguyên $n \geqslant 0$, $D^n f$ ký hiệu đạo hàm cấp $n$ của một hàm số $f$ xác định trên I (khi đạo hàm này tồn tại). Cho $s \geqslant 1$ và $M \geqslant 0$ là hai số thực. Ký hiệu $\mathcal{G}_{s,M}(I)$ là không gian vectơ gồm các hàm khả vi vô hạn $f$ trên I (FVR, I, p. 28) sao cho dãy $(|D^n f|/M^n(n!)^s)_{n \geqslant 0}$ bị chặn trong không gian $\mathcal{C}(I)$ của tất cả các hàm liên tục trên I (với tôpô hội tụ đều). Không gian $\mathcal{G}_{s,M}(I)$ là một không gian Banach với chuẩn

$$
\|f\|_{s,M} = \sup_{n \geqslant 0, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

Với $M \leqslant M'$, ta có $\mathcal{G}_{s,M}(I) \subset \mathcal{G}_{s,M'}(I)$, và

$$
\|f\|_{s,M'} \leqslant \|f\|_{s,M}
$$

với mọi $f \in \mathcal{G}_{s,M}(I)$. Ký hiệu $\mathcal{G}_s(I)$ là hợp của các không gian $\mathcal{G}_{s,M}(I)$ và trang bị cho nó tôpô giới hạn quy nạp của các tôpô của $\mathcal{G}_{s,M}(I)$.

Cho $M < M'$ và gọi B là quả cầu đơn vị (đóng) trong $\mathcal{G}_{s,M}(I)$. Ta sẽ chứng minh rằng B là một tập con compact của không gian Banach $\mathcal{G}_{s,M'}(I)$. Rõ ràng B đóng trong $\mathcal{G}_{s,M'}(I)$ và do đó chỉ cần chứng minh rằng B là tiền compact trong $\mathcal{G}_{s,M'}(I)$. Cho $\varepsilon > 0$ và cho N là một số nguyên dương sao cho $(M/M')^N \leqslant \varepsilon/2$. Cho $k$ là một số nguyên dương; tập hợp tất cả các hàm $D^{k+1} f$, khi $f$ chạy trên B, bị chặn trong $\mathcal{C}(I)$, do đó tập hợp tất cả các hàm $D^k f$, khi $f$ chạy trên B, là tương đối compact trong $\mathcal{C}(I)$: điều này suy ra từ định lý số gia hữu hạn (FVR, I, p. 23, cor. 1) và định lý Ascoli (GT, X, § 2, No. 5). Ta định nghĩa một chuẩn trên $\mathcal{G}_{s,M}(I)$ bởi

$$
q(f) = \sup_{0 \leqslant n \leqslant N, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

Lập luận trên cho thấy B là tiền compact đối với tôpô liên kết với chuẩn $q$; nói cách khác, tồn tại một tập con hữu hạn C của B sao cho với mọi $f \in B$, tồn tại $g \in C$ sao cho $q(f - g) \leqslant \varepsilon$. Cuối cùng, với mọi $n > N$, ta có

$$
|D^n f(x) - D^n g(x)|/M^n(n!)^s \leqslant 2(M/M')^n \leqslant \varepsilon ,
$$

từ đó suy ra $\|f - g\| \leqslant \varepsilon$. Điều này chứng minh rằng B là tiền compact trong $\mathcal{G}_{s,M'}(I)$.

Không gian $\mathcal{G}_s(I)$ là giới hạn quy nạp của các không gian $\mathcal{G}_{s,k}(I)$ khi $k$ chạy trên $\mathbf{N}$; theo mệnh đề 7 (III, p. 6), mọi tập con bị chặn của $\mathcal{G}_s(I)$ đều được chứa trong một trong các không gian $\mathcal{G}_{s,k}(I)$ và là tương đối compact trong không gian này.

\* d) (Các không gian hàm chỉnh hình.) Cho $n \geqslant 1$ là một số nguyên. Với mọi tập con mở U của $\mathbf{C}^n$, $\mathcal{H}(U)$ ký hiệu không gian các hàm chỉnh hình trong U, và được trang bị tôpô hội tụ compact trong U. Với mọi tập con compact L của $\mathbf{C}^n$, $\mathcal{H}(L)$ ký hiệu không gian các mầm của các hàm chỉnh hình trong một lân cận của L; ta trang bị cho không gian này tôpô lồi địa phương mịn nhất sao cho các ánh xạ chính tắc $\pi_U : \mathcal{H}(U) \to \mathcal{H}(L)$ là liên tục, trong đó U chạy trên tập hợp các lân cận mở của L.

Với mọi số nguyên $m \geq 1$, đặt $U_m$ là tập hợp các điểm của $\mathbf{C}^n$ cách L một khoảng $< 1/m$. Có thể chứng minh rằng ánh xạ chính tắc $\pi_{U_m}$ từ $\mathcal{H}(U_m)$ vào $\mathcal{H}(L)$ là *đơn ánh*, và ánh xạ hạn chế từ $\mathcal{H}(U_m)$ vào $\mathcal{H}(U_p)$ là *compact* với $p \geq m$. Khi đó ta có thể áp dụng mệnh đề 7 (III, p. 6). Cho A là một tập con bị chặn của $\mathcal{H}(L)$; khi đó tồn tại một số nguyên $m \geq 1$ sao cho A gồm các mầm của các hàm trong một lân cận của L, thuộc một tập hợp B bị chặn trong $\mathcal{H}(U_m)$. Hơn nữa, một ánh xạ $\phi$ từ $\mathcal{H}(L)$ vào một không gian tôpô T là liên tục khi và chỉ khi ánh xạ $\phi \circ \pi_U$ từ $\mathcal{H}(U)$ vào T liên tục với mọi lân cận mở U của L. \*

### Bài tập {#evt-iii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
