---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 2
section_title: Convex sets
lang: vi
source: evt-i-v
book_pages: TVS II.7-TVS II.21
pdf_pages: 0044-0058, 0102-0109
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a convex set
      page: 7
      pdf_page: 44
    - "no": 2
      title: Intersections of convex sets. Products of convex sets
      page: 9
      pdf_page: 46
    - "no": 3
      title: Convex envelope of a set
      page: 9
      pdf_page: 46
    - "no": 4
      title: Convex cones
      page: 10
      pdf_page: 47
    - "no": 5
      title: Ordered vector spaces
      page: 12
      pdf_page: 49
    - "no": 6
      title: Convex cones in topological vector spaces
      page: 13
      pdf_page: 50
    - "no": 7
      title: Topologies on ordered vector spaces
      page: 15
      pdf_page: 52
    - "no": 8
      title: Convex functions
      page: 16
      pdf_page: 53
    - "no": 9
      title: Operations on convex functions
      page: 18
      pdf_page: 55
    - "no": 10
      title: Convex functions over an open convex set
      page: 18
      pdf_page: 55
    - "no": 11
      title: Semi-norms and convex sets
      page: 19
      pdf_page: 56
statements: 49
exercises: 43
content_sha256: 4c1f60d8ab6be2aa596b031746ddcdadb1b96c462aeabf21f9df572f698bb5d7
translated_from: content/en/evt/II/02_s2_convex_sets.md
source_content_sha256: 742c952fc6a2e57dc8eb5e75ac174e898ff3d3d87043cbf6c8ab24a81db58512
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-aad0b89a
glossary_version: 34
glossary_terms_sha256: 8ed9a942de6ebeb556aadcb6bd427d52e672eb4d0d5b98090346e86d5424703f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. TẬP HỢP LỒI

### 1. Định nghĩa tập hợp lồi

Với hai điểm bất kỳ $x, y$ của một không gian affine $E$, tập hợp các điểm $\lambda x + \mu y$ trong đó $\lambda \geq 0, \mu \geq 0, \lambda + \mu = 1$ được gọi là đoạn đóng có các đầu mút $x$ và $y$; nó suy biến thành một điểm khi $x = y$. Phần bù của $x$ trong đoạn này được gọi là đoạn có các đầu mút $x, y$, mở tại $x$ và đóng tại $y$; nó rỗng nếu $x = y$. Cuối cùng, phần bù của $\{ x, y \}$ trong đoạn đóng có các đầu mút $x, y$ được gọi là đoạn mở có các đầu mút $x, y$; nó rỗng khi $x = y$.

#### Định nghĩa 1 {#evt-ii-s2-def-1 .statement}

— Một tập con $A$ của một không gian affine $E$ là lồi nếu, với mọi hai điểm $x, y$ của $A$, đoạn đóng có các đầu mút $x, y$ được chứa trong $A$.

Vì $(1 - \lambda) a + \lambda x = a + \lambda (x - a)$, định nghĩa này tương đương với điều sau: tập hợp $A$ là lồi nếu, với mọi điểm $a \in A$, biến đổi của $A$ bởi một phép vị tự có tâm $a$ và tỉ số $\lambda$ trong đó $0 < \lambda < 1$, được chứa trong $A$ (nói cách khác, $A$ ổn định đối với các phép vị tự này).

#### Ví dụ 1 {#evt-ii-s2-n1-exa-1 .statement}

Mọi đa tạp affine tuyến tính của $E$ (và đặc biệt là tập rỗng) đều lồi.
2) Các tập hợp lồi không rỗng duy nhất trong $\mathbf{R}$ là các khoảng (GT, IV, § 2.4, mệnh đề. 1).
3) Cho $E$ là một không gian vectơ và $\|x\|$ là một chuẩn trên $E$; quả cầu đơn vị $B$, được tạo bởi các điểm $x$

sao cho $\|x\| \leq 1$, là lồi vì các quan hệ $\|x\| \leq 1, \|y\| \leq 1$, kéo theo, với $0 \leq \lambda \leq 1$, rằng
$$
\|\lambda x + (1 - \lambda) y\| \leq \lambda \|x\| + (1 - \lambda) \|y\| \leq \lambda + (1 - \lambda) = 1 .
$$

#### Nhận xét {#evt-ii-s2-n1-rem-1 .statement}

— Cho $A$ là một tập con lồi của một không gian vectơ $E$; với mọi vô hướng $\alpha > 0$ và $\beta > 0$ ta có $\alpha A + \beta A = (\alpha + \beta) A$. Nói cách khác, với mọi $x \in A, y \in A$, tồn tại $z \in A$ sao cho $(\alpha + \beta) z = \alpha x + \beta y$; thực ra quan hệ này có thể viết dưới dạng $z = \frac{\alpha}{\alpha + \beta} x + \frac{\beta}{\alpha + \beta} y$ và ta có $\frac{\alpha}{\alpha + \beta} > 0, \frac{\beta}{\alpha + \beta} > 0$ và $\frac{\alpha}{\alpha + \beta} + \frac{\beta}{\alpha + \beta} = 1$, từ đó suy ra mệnh đề, khi sử dụng định nghĩa. 1.

#### Mệnh đề 1 {#evt-ii-s2-prop-1 .statement}

*Cho $(x_i)$ là một họ các điểm của một tập con lồi $A$; mọi trọng tâm $\sum_i \lambda_i x_i$ của các $x_i$ được lập bởi các trọng số dương $\lambda_i$ (sao cho $\sum_i \lambda_i = 1$ và $\lambda_i = 0$ trừ hữu hạn chỉ số, xem A, II, § 9.3) đều thuộc $A$.*

Rõ ràng ta chỉ cần xét trường hợp các chỉ số là $1, 2, ..., p$ và $\lambda_i > 0$ với mỗi $i$; mệnh đề là tầm thường nếu $p = 1$; ta chứng minh kết quả bằng quy nạp theo $p$. Đặt $\mu = \sum_{i=1}^{p-1} \lambda_i > 0$, và $y = \sum_{i=1}^{p-1} \frac{\lambda_i}{\mu} x_i$; giả thiết quy nạp suy ra $y \in A$. Vì $\lambda_p = 1 - \mu$ và $\sum_{i=1}^p \lambda_i x_i = \mu y + (1 - \mu) x_p$, nên theo định nghĩa 1, $\sum_{i=1}^p \lambda_i x_i$ thuộc $A$.

#### Mệnh đề 2 {#evt-ii-s2-prop-2 .statement}

*Cho $E$ và $F$ là hai không gian afin và $f$ là một ánh xạ afin tuyến tính từ $E$ vào $F$; khi đó ảnh của một tập con lồi của $E$ qua $f$, và ảnh ngược của một tập con lồi của $F$ qua $f$ đều lồi.*

Ảnh qua $f$ của đoạn đóng có các đầu mút $x, y$ là đoạn đóng có các đầu mút $f(x), f(y)$, do đó có mệnh đề thứ nhất. Ta suy ra rằng ảnh ngược của một đoạn đóng của $F$ qua $f$ chứa mọi đoạn đóng có các đầu mút thuộc nó; mệnh đề thứ hai của mệnh đề 2 được suy ra.

Đặc biệt, ảnh của một tập lồi qua một phép vị tự hoặc một phép tịnh tiến là một tập lồi.

#### Mệnh đề 3 {#evt-ii-s2-prop-3 .statement}

*Trong không gian afin $E$, cho $H$ là một siêu phẳng được xác định bởi quan hệ $g(x) = 0$, trong đó $g$ là một hàm afin không hằng trên $E$. Khi đó các nửa không gian được xác định bởi các quan hệ $g(x) \geq 0, g(x) \leq 0, g(x) > 0, g(x) < 0$ là lồi.*

Vì các tập này là ảnh ngược qua $g$ của các khoảng của $\mathbf{R}$ và do đó là lồi.

Với các ký hiệu của mệnh đề 3, các điểm của một tập con $M$ của một không gian afin *nằm về cùng một phía* (tương ứng *nằm nghiêm ngặt về cùng một phía*) của siêu phẳng $H$ nếu $M$ được chứa trong một trong các nửa không gian được xác định bởi $g(x) \geq 0, g(x) \leq 0$ (tương ứng $g(x) > 0$ hoặc $g(x) < 0$).

#### Mệnh đề 4 {#evt-ii-s2-prop-4 .statement}

*Các điểm của $A$, một tập con lồi của một không gian afin $E$, nằm nghiêm ngặt về cùng một phía của một siêu phẳng $H$ khi và chỉ khi $A$ không gặp $H$.*

Rõ ràng điều kiện là cần thiết. Ngược lại, giả sử điều kiện ấy được thỏa mãn và cho $g(x) = 0$, là một phương trình xác định H ($g$ là một ánh xạ afin tuyến tính của E vào $\mathbf{R}$). Tập $g(A)$ là lồi trong $\mathbf{R}$, do đó nó là một khoảng, và $0 \notin g(A)$. Suy ra $g(x)$ có cùng dấu với mọi $x \in A$.

### 2. Giao của các tập lồi. Tích của các tập lồi

#### Mệnh đề 5 {#evt-ii-s2-prop-5 .statement}

— *Giao của mọi họ các tập con lồi của một không gian afin* E *là lồi*.

Mệnh đề suy ra ngay lập tức từ định nghĩa 1 của II, p. 7.

#### Mệnh đề 6 {#evt-ii-s2-prop-6 .statement}

— *Cho* $(E_i)_{i \in I}$ *là một họ các không gian vectơ, và với mỗi* $i \in I$, *cho* $A_i$ *là một tập con không rỗng của* $E_i$. *Khi đó tập* $A = \prod_{i \in I} A_i$ *là lồi trong* $E = \prod_{i \in I} E_i$, *khi và chỉ khi, với mọi* $i \in I$, *tập* $A_i$ *là lồi trong* $E_i$.

Thật vậy, mỗi phép chiếu $\mathrm{pr}_i$ là một ánh xạ tuyến tính và ta có $A_i = \mathrm{pr}_i A$ và $A = \bigcap_{i \in I} \mathrm{pr}_i^{-1}(A_i)$; mệnh đề suy ra từ các mệnh đề 2 và 5 ở trên.

#### Hệ quả {#evt-ii-s2-n2-cor-1 .statement}

— *Trong không gian* $\mathbf{R}^n$ *mọi hình hộp song song* (GT, VI, § 1.3) *đều là một tập con lồi*.

Vì nó là ảnh qua một ánh xạ afin tuyến tính của một hình hộp chữ nhật, và hình hộp chữ nhật này là lồi theo mệnh đề 6.

#### Mệnh đề 7 {#evt-ii-s2-prop-7 .statement}

— *Cho* A *và* B *là hai tập con lồi của không gian vectơ* E. *Với mọi số thực* $\alpha, \beta$ *tập* $\alpha A + \beta B$ *(tập các điểm có dạng* $\alpha x + \beta y$, *trong đó* $x$ *biến thiên trong* A, *và* $y$ *trong* B*) *là lồi*.

Vì $\alpha A + \beta B$ là ảnh của tập con lồi $A \times B$ của $E \times E$ qua ánh xạ tuyến tính $(x, y) \mapsto \alpha x + \beta y$ của $E \times E$ vào $E$.

### 3. Bao lồi của một tập

#### Định nghĩa 2 {#evt-ii-s2-def-2 .statement}

— *Cho một tập con* A *của một không gian afin* E, *ta gọi giao của mọi tập lồi chứa* A, *là bao lồi của* A, *tức là* (II, p. 9, mệnh đề 5) *nó là tập lồi nhỏ nhất chứa* A.

#### Mệnh đề 8 {#evt-ii-s2-prop-8 .statement}

— *Với mọi họ* $(A_i)_{i \in I}$ *các tập con lồi của một không gian afin* E, *bao lồi của* $\bigcup_{i \in I} A_i$ *chính là tập các tổ hợp tuyến tính* $\sum_{i \in I} \lambda_i x_i$, *trong đó* $x_i \in A_i, \lambda_i \geq 0$ *với mọi* $i \in I$ ($\lambda_i = 0$ *trừ hữu hạn nhiều chỉ số*) *và* $\sum_{i \in I} \lambda_i = 1$.

Ký hiệu tập các tổ hợp tuyến tính ấy là C, hiển nhiên C được chứa trong mọi tập lồi chứa tất cả các $A_i$ (II, p. 8, mệnh đề 1); mặt khác $A_i \subset C$ với mọi $i$. Điều còn lại phải chứng minh là C lồi. Cho $x = \sum \lambda_i x_i$, $y = \sum \mu_i y_i$ là hai điểm của C và $\alpha$ là một số sao cho $0 < \alpha < 1$, viết γ_i = αλ_i + (1 - α) μ_i cho mọi i ∈ I, và cho J là tập (hữu hạn) các chỉ số của I sao cho γ_i ≠ 0. Ta có thể viết αx + (1 - α)y = ∑_{i∈J} γ_i z_i, trong đó

$$ z_i = γ_i^{-1}(αλ_i x_i + (1 - α) μ_i y_i) $$

thuộc A_i với mọi i ∈ J; nhưng $\sum_{i∈J} γ_i = α \sum_{i∈I} \lambda_i + (1 - α) \sum_{i∈I} \mu_i = 1$, và ta thấy rằng $ax + (1 - \alpha) y ∈ C$. Mệnh đề được chứng minh.

#### Hệ quả 1 {#evt-ii-s2-prop-8-cor-1 .statement}

*Bao lồi của một tập con A của E trùng với tập các tổ hợp tuyến tính $\sum_i λ_i x_i$, trong đó $(x_i)$ là bất kỳ một họ hữu hạn các điểm của A, các số $λ_i > 0, \text{ với mọi } i$ và $\sum_i λ_i = 1$.*

Chiều của đa tạp tuyến tính afin (A, II, § 9.3) được sinh bởi tập lồi A được gọi là *chiều* của A.

Cho E là một không gian vectơ. Bao lồi C của bao cân bằng của một tập hợp A trong E được gọi là *bao lồi cân bằng* (hay *bao lồi đối xứng*) của A; hiển nhiên nó là tập lồi đối xứng nhỏ nhất chứa A; nó cũng là bao lồi của $A \cup (-A)$, vì mọi điểm của bao cân bằng của A đều thuộc về một đoạn thẳng có hai đầu mút a và −a với $a ∈ A$. Tập C trùng với tập các tổ hợp tuyến tính $\sum_i λ_i x_i$ với $x_i ∈ A$ và $\sum_i |λ_i| ≤ 1$; vì rõ ràng tập các điểm này là lồi và chứa A và −A; đủ để chứng minh rằng nó được chứa trong C, và để làm điều đó ta chỉ cần xét những tổ hợp tuyến tính sao cho $μ = \sum_i |λ_i| > 0$; khi đó ta có thể viết $\sum_i λ_i x_i = μ \cdot \sum_i α_i y_i$ với $α_i = λ_i/μ$ và $y_i = x_i$, nếu $λ_i ≥ 0$; và $α_i = -λ_i/μ$; $y_i = -x_i$ nếu $λ_i < 0$; hiển nhiên $\sum_i α_i = 1$, và khẳng định của chúng ta được chứng minh.

#### Hệ quả 2 {#evt-ii-s2-prop-8-cor-2 .statement}

*Cho f là một ánh xạ tuyến tính affine từ không gian affine E vào không gian affine F; với mỗi tập con A của E, bao lồi của f(A) là ảnh qua f của bao lồi của A.*

Có một mệnh đề tương tự cho các ánh xạ tuyến tính và các bao lồi cân bằng.

### 4. Nón lồi

#### Định nghĩa 3 {#evt-ii-s2-def-3 .statement}

*Một tập con C của một không gian affine E là một nón có đỉnh x_0 nếu C bất biến đối với mọi phép vị tự tâm x_0 và tỉ số > 0.*

Trong mục này và mục kế tiếp, ta giả sử rằng ta đã chọn đỉnh của nón đang xét làm gốc trong E; *tức là* ta giả sử rằng E là một không gian vectơ, và khi ta nói về một nón, thì hiểu là nón đó có đỉnh 0. Tập các điểm có dạng $λa$ với $λ > 0$ (tương ứng $λ ≥ 0$), trong đó $a$ là một vectơ khác không, được gọi là một *nửa đường thẳng mở* (tương ứng *nửa đường thẳng đóng*) xuất phát từ 0.

Một nón C có đỉnh 0 được gọi là *nhọn* nếu $0 ∈ C$, và *không nhọn* nếu ngược lại. Một nón nhọn hoặc là chính điểm đơn $\{0\}$ hoặc là hợp của một tập các nửa đường thẳng đóng xuất phát từ 0. Một nón không nhọn là hợp (có thể rỗng) của các nửa đường thẳng mở xuất phát từ 0. Nếu C là một nón không nhọn, thì $C \cup \{0\}$ là một nón nhọn. Nếu C là một nón nhọn, thì $C - \{0\}$ là một nón không nhọn.

Nếu C là một nón *lồi* không nhọn, thì $C \cup \{0\}$ là một nón lồi nhọn. Tuy nhiên, nếu C là một nón lồi nhọn, $C - \{0\}$ không nhất thiết lồi. Ta nói rằng một nón lồi nhọn là *thực sự* nếu nó không chứa bất kỳ đường thẳng nào đi qua 0. Khi đó

#### Mệnh đề 9 {#evt-ii-s2-prop-9 .statement}

*Một nón lồi nhọn C là thực sự khi và chỉ khi nón không nhọn $C'$, là phần bù của 0 trong C, là lồi.*

Nếu C chứa một đường thẳng đi qua 0 thì hiển nhiên $C'$ không lồi. Giả sử bây giờ C là thực sự và cho x, y là hai điểm của $C'$. Đoạn thẳng đóng có hai đầu mút x, y được chứa trong C; nếu nó chứa 0 thì $\lambda x + (1 - \lambda) y = 0$ với một $\lambda$ nào đó thỏa $0 < \lambda < 1$, do đó $x = \mu y$ với $\mu < 0$. Vậy C chứa đường thẳng đi qua 0 và x, trái với giả thiết.

#### Mệnh đề 10 {#evt-ii-s2-prop-10 .statement}

*Một tập con C của E là một nón lồi khi và chỉ khi $C + C \subset C$ và $\lambda C \subset C$ với mọi $\lambda > 0$.*

Vì điều kiện $\lambda C \subset C$ với mọi $\lambda > 0$ đặc trưng cho các nón. Nếu C là lồi thì ta có $C + C = \frac{1}{2}C + \frac{1}{2}C = C$ (II, p. 8, *Nhận xét*). Ngược lại, nếu nón C thỏa $C + C \subset C$, thì với $0 < \lambda < 1$, ta có $\lambda C + (1 - \lambda) C = C + C \subset C$, điều này cho thấy C là lồi.

#### Hệ quả 1 {#evt-ii-s2-prop-10-cor-1 .statement}

*Nếu C là một nón lồi không rỗng, không gian vectơ sinh bởi C là tập $C - C$ (tập các điểm $x - y$ khi x, y thay đổi trong C).*

Thật vậy, nếu $V = C - C$, thì V không rỗng, ta có $\lambda V = V$ với mọi $\lambda \neq 0$, và $V + V = C + C - (C + C) \subset C - C = V$, điều này cho thấy V là một không gian con vectơ. Cuối cùng mọi không gian con vectơ chứa C cũng chứa V.

#### Hệ quả 2 {#evt-ii-s2-prop-10-cor-2 .statement}

*Nếu C là một nón lồi nhọn, không gian con vectơ lớn nhất được chứa trong C là tập $C \cap (-C)$.*

Thật vậy, nếu $W = C \cap (-C)$, thì W không rỗng và $\lambda W = W$ với mọi $\lambda \neq 0$, đồng thời
$$
W + W \subset (C + C) \cap (-(C + C)) \subset C \cap (-C) = W,
$$
điều đó cho thấy W là một không gian con vectơ. Hiển nhiên mọi không gian con vectơ được chứa trong C cũng được chứa trong W.

Hiển nhiên, nếu $f$ là một ánh xạ tuyến tính từ E vào một không gian vectơ F, thì $f(C)$, ảnh của một nón lồi C trong E, là một nón lồi trong F. Mọi giao của các nón lồi (có đỉnh 0) trong E đều là một nón lồi. Với mọi tập con A của E, giao của các nón lồi chứa A (chúng tồn tại, chính E cũng là một nón như vậy) là nón lồi nhỏ nhất chứa A; nó được gọi là nón lồi *sinh* bởi A.

#### Mệnh đề 11 {#evt-ii-s2-prop-11 .statement}

*Cho $(C_i)_{i \in I}$ là một họ các nón lồi trong E; nón lồi sinh bởi hợp của các $C_i$ trùng với tập các điểm $\sum_{i \in J} x_i$, trong đó J là một tập con hữu hạn bất kỳ của I và $x_i \in C_i$ với mọi $i \in J$. \*

Thật vậy, hiển nhiên C, tập các điểm như vậy, là một nón lồi chứa hợp của các $C_i$, và nó được chứa trong mọi nón lồi nào chứa hợp này.

#### Hệ quả {#evt-ii-s2-n4-cor-1 .statement}

— *Với mọi tập con A của E, nón lồi sinh bởi A, trùng với tập các tổ hợp tuyến tính* $\sum_{i \in J} \lambda_i x_i$, *trong đó* $(x_i)_{i \in J}$ *là bất kỳ một họ hữu hạn không rỗng các điểm của A, và trong đó* $\lambda_i > 0$ *với mọi* $i \in J$.

Chỉ cần thấy rằng, nếu một nón lồi chứa một điểm $x \neq 0$ của A thì nó cũng chứa nửa đường thẳng $C_x$ gồm các điểm $\lambda x$ trong đó $\lambda$ biến thiên trong tập các số dương, và rằng $C_x$ là một nón lồi.

#### Mệnh đề 12 {#evt-ii-s2-prop-12 .statement}

— *Nếu A là một tập lồi trong E, thì nón lồi sinh bởi A trùng với* $C = \bigcup_{\lambda > 0} \lambda A$.

Tập C rõ ràng là một nón; chỉ cần chứng minh rằng C là lồi. Cho $\lambda x, \mu y$ là hai điểm của C ($\lambda > 0, \mu > 0, x \in A, y \in A$). Cho $\alpha, \beta$ là hai số $> 0$ sao cho $\alpha + \beta = 1$. Khi đó $\alpha \lambda x + \beta \mu y = (\alpha \lambda + \beta \mu) z$, với $z \in A$, và $\alpha \lambda + \beta \mu > 0$; do đó $\alpha \lambda x + \beta \mu y \in C$.

#### Nhận xét {#evt-ii-s2-n4-rem-1 .statement}

— 1) Với các giả thiết của Mệnh đề 12, nếu $0 \notin A$, thì nón C không nhọn, do đó $C \cup \{0\}$ là *thực sự*.

2) Cho A là một tập lồi bất kỳ trong E; xét tập lồi $A_1 = A \times \{1\}$ trong không gian $F = E \times \mathbf{R}$ và nón lồi C có đỉnh 0 được sinh bởi $A_1$. Mệnh đề 12 cho thấy rằng $A_1$ là giao của C với siêu phẳng $E \times \{1\}$ trong F. Do đó, mọi tập lồi trong E có thể được xem là phép chiếu lên E của giao của một nón lồi có đỉnh 0 trong F với siêu phẳng $E \times \{1\}$.

### 5. Không gian vectơ có thứ tự

Một cấu trúc *tiền thứ tự* trên một không gian vectơ E, ký hiệu bởi $x \leqslant y$ hoặc $y \geqslant x$, là *tương thích* với cấu trúc không gian vectơ của E nếu nó thỏa mãn hai tiên đề sau;

*(EO$_I$)* *Nếu* $x \leqslant y$ *thì* $x + z \leqslant y + z$ *với mọi* $z \in E$.

*(EO$_{II}$)* *Nếu* $x \geqslant 0$ *thì* $\lambda x \geqslant 0$ *với mọi vô hướng* $\lambda \geqslant 0$.

Không gian vectơ E, mang hai cấu trúc này, được gọi là một *không gian vectơ tiền thứ tự* (tương ứng là *không gian vectơ có thứ tự* khi quan hệ tiền thứ tự trên E là một quan hệ thứ tự).

Chú ý rằng tiên đề (EO$_I$) có nghĩa là cấu trúc tiền thứ tự và cấu trúc nhóm cộng của E là tương thích, nghĩa là E khi mang hai cấu trúc này là một *nhóm tiền thứ tự* (A, VI, p. 3).

#### Ví dụ {#evt-ii-s2-n5-exa-1 .statement}

— Trên không gian $E = \mathbf{R}^A$ của tất cả các hàm giá trị thực hữu hạn xác định trên A, quan hệ thứ tự được cho bởi « với mọi $t \in A$, $x(t) \leqslant y(t)$ » là tương thích với cấu trúc không gian vectơ của E.

#### Mệnh đề 13 {#evt-ii-s2-prop-13 .statement}

— (i) *Tập P, gồm các phần tử* $\geqslant 0$, *của một không gian vectơ tiền thứ tự E, là một nón lồi nhọn*.

(ii) *Ngược lại, nếu P là một nón lồi nhọn trong E, thì quan hệ* $y - x \in P$ *là một quan hệ tiền thứ tự trên E, và cấu trúc tiền thứ tự mà nó xác định là cấu trúc duy nhất* tương thích với cấu trúc không gian vectơ của E và sao cho P là tập các phần tử $\geqslant 0$.

(iii) Quan hệ $y - x \in P$, với P là một nón lồi nhọn, là một quan hệ thứ tự trên E nếu và chỉ nếu P là một nón thực sự.

(i) Các tiên đề (EO_I) và (EO_{II}) suy ra $P + P \subset P$ và $\lambda P \subset P$ với mọi $\lambda > 0$. Vì $0 \in P$, suy ra P là một nón lồi nhọn (II, p. 11, Mệnh đề 10).

(ii) Ngược lại, nếu P là một nón lồi nhọn, thì quan hệ $P + P \subset P$ suy ra rằng quan hệ $y - x \in P$ là một quan hệ tiền thứ tự tương thích với cấu trúc nhóm cộng của E (A, VI, p. 3, Mệnh đề 3); viết nó dưới dạng $x \leqslant y$, ta được tập P trùng với tập các $x \geqslant 0$; hơn nữa quan hệ $\lambda P \subset P$ với mọi $\lambda \geqslant 0$ cho thấy tiên đề (EO_{II}) được thỏa mãn.

(iii) Nói P là thực sự có nghĩa là $P \cap (-P) = \{0\}$ (II, p. 11, Hệ quả 2), do đó $y - x \in P$ là một quan hệ thứ tự.

#### Ví dụ {#evt-ii-s2-n5-exa-2 .statement}

\* Cho H là một không gian Hilbert thực; trong không gian vectơ $\mathcal{L}(H)$ của các tự đồng cấu liên tục của H, các tự đồng cấu Hermit dương tạo thành một nón lồi nhọn thực sự; do đó, nón này xác định một cấu trúc cấp tương thích với cấu trúc không gian vectơ của $\mathcal{L}(H)$ và trong đó quan hệ $A \leqslant B$ có nghĩa là $B - A$ là một tự đồng cấu Hermit dương. \*

Với mọi nón lồi nhọn P trong không gian vectơ E, tập $P \cap (-P)$ là một không gian con vectơ, H, của E (II, p. 11, hệ quả 2). Ảnh chính tắc $P'$ của P trong $E/H$ là một nón lồi và ảnh ngược của $P'$ trong E là P. Do đó $P' \cap (-P') = \{0\}$, và $P'$ xác định một cấu trúc cấp trên $E/H$ tương thích với cấu trúc không gian vectơ của nó.

Một dạng tuyến tính $f$ trên một không gian vectơ có cấp trước E được gọi là dương nếu $x \geqslant 0$ trong E kéo theo $f(x) \geqslant 0$. Hay, tương đương, nếu nón lồi P gồm các phần tử $\geqslant 0$ trong E được chứa trong nửa không gian gồm những $x$ sao cho $f(x) \geqslant 0$. Rõ ràng, trong đối ngẫu $E^*$ của E, tập các dạng tuyến tính dương là một nón lồi nhọn.

### 6. Các nón lồi trong các không gian vectơ tôpô

#### Mệnh đề 14 {#evt-ii-s2-prop-14 .statement}

Trong một không gian vectơ tôpô E, bao đóng của một tập lồi (tương ứng, của một nón lồi) là một tập lồi (tương ứng, một nón lồi có cùng đỉnh).

Thật vậy, cho A là một tập lồi; ánh xạ $(x, y) \mapsto \lambda x + (1 - \lambda) y$, trong đó $0 < \lambda < 1$, là liên tục trong $E \times E$ và ánh xạ $A \times A$ vào A; do đó (GT, I, § 2.1, định lý 1) nó ánh xạ $\overline{A} \times \overline{A}$ vào $\overline{A}$, điều này cho thấy $\overline{A}$ là lồi. Tương tự, nếu C là một nón lồi có đỉnh 0 thì $\overline{C} + \overline{C} \subset \overline{C}$ và $\lambda \overline{C} \subset \overline{C}$ với mọi $\lambda > 0$.

#### Định nghĩa 4 {#evt-ii-s2-def-4 .statement}

Với mọi tập A của một không gian vectơ tôpô E, giao của tất cả các tập lồi đóng chứa A được gọi là bao lồi đóng của A; đó là tập lồi đóng nhỏ nhất chứa A.

Theo mệnh đề 14, bao lồi đóng của A là bao đóng của bao lồi của A; rõ ràng nó cũng chính là bao lồi đóng của $\overline{A}$.

Tương tự, ta gọi tập đối xứng, lồi, đóng nhỏ nhất chứa A là bao lồi đóng đối xứng (hoặc bao lồi đóng cân bằng) của A; đó là bao đóng của bao lồi đối xứng của A (II, p. 10); nó cũng là bao lồi đóng đối xứng của $\overline{A}$.

#### Mệnh đề 15 {#evt-ii-s2-prop-15 .statement}

— Cho $A_i$ ($1 \leq i \leq n$) là một số hữu hạn các tập lồi compact trong một không gian vectơ tôpô Hausdorff E. Khi đó bao lồi của hợp các $A_i$ là compact (và do đó cũng chính là bao lồi đóng của hợp này).

Cho B là tập compact trong $\mathbf{R}^n$ được xác định bởi các điểm $(\lambda_1, \lambda_2, ..., \lambda_n)$ trong đó $\lambda_i \geq 0$ ($1 \leq i \leq n$), và $\sum_{i=1}^n \lambda_i = 1$. Định nghĩa một ánh xạ liên tục từ $B \times \prod_{i=1}^n A_i \subset \mathbf{R}^n \times E^n$ vào E bởi công thức $(\lambda_1, \lambda_2, ..., \lambda_n, x_1, x_2, ..., x_n) \mapsto \sum_{i=1}^n \lambda_i x_i$. Bao lồi C của $\bigcup_{i=1}^n A_i$ là ảnh của $B \times \prod_{i=1}^n A_i$ qua ánh xạ này; vì $B \times \prod_{i=1}^n A_i$ là compact và E là Hausdorff, suy ra C là compact.

#### Hệ quả 1 {#evt-ii-s2-prop-15-cor-1 .statement}

— Trong một không gian vectơ tôpô Hausdorff, bao lồi của một tập hữu hạn là compact.

#### Hệ quả 2 {#evt-ii-s2-prop-15-cor-2 .statement}

— Trong một không gian vectơ tôpô E, bao lồi của một tập hữu hạn là tiền compact.

Thật vậy, gọi j là ánh xạ chính tắc từ E vào hoàn thành Hausdorff của nó $\hat{E}$; nếu C là bao lồi của A, thì $j(C)$ là bao lồi của tập hữu hạn $j(A)$ trong $\hat{E}$, do đó $j(C)$ là compact (hệ quả 1) và vì vậy C là tiền compact (GT, II, § 4.2).

#### Mệnh đề 16 {#evt-ii-s2-prop-16 .statement}

— Cho A là một tập con lồi, có ít nhất một điểm trong $x_0$, của một không gian vectơ tôpô E. Với mọi điểm $x \in \overline{A}$, mọi điểm của đoạn mở có hai đầu mút $x_0, x$ đều nằm trong phần trong của A.

Với mọi điểm y của đoạn này, gọi f là phép vị tự có tâm y và tỉ số $\lambda < 0$, biến $x_0$ thành x. Nếu V là một lân cận mở của $x_0$ được chứa trong A, thì $f(V)$ là một lân cận của x và do đó chứa một điểm $f(z) \in A$; khi đó

$$
f(z) - y = \lambda (z - y) = \lambda (z - f(z)) + \lambda (f(z) - y),
$$

hence $y - f(z) = \frac{\lambda}{\lambda - 1} (z - f(z))$, do đó y được biến đổi thành z bởi phép vị tự g, có tâm $f(z)$ và tỉ số $\mu = \lambda / (\lambda - 1)$; vì $0 < \mu < 1$, g biến đổi V thành một lân cận của 0 được chứa trong A. Mệnh đề được chứng minh.

#### Hệ quả 1 {#evt-ii-s2-prop-16-cor-1 .statement}

— Phần trong $\overset{\circ}{A}$ của một tập hợp lồi $\overline{A}$, tự nó là một tập hợp lồi; nếu $\overset{\circ}{A}$ không rỗng, thì nó trùng với phần trong của $\overline{A}$, và $\overline{A}$ là một tập hợp lồi trùng với bao đóng của $\overset{\circ}{A}$.

Theo mệnh đề 16, nếu $\overset{\circ}{A}$ không rỗng, thì nó là một tập hợp lồi và mọi điểm của $\overline{A}$ đều là điểm tụ của $\overset{\circ}{A}$. Tiếp theo ta chứng minh rằng mọi điểm trong của $\overline{A}$ đều thuộc $\overset{\circ}{A}$. Cho x là một điểm trong của $\overline{A}$ và giả sử, để xác định, rằng $x = 0$. Cho V là một lân cận đối xứng của 0 được chứa trong $\overline{A}$ và cho $y \in \overset{\circ}{A} \cap V$; khi đó $-y \in \overline{A}$, và do đó, theo mệnh đề 16, ta thấy rằng $0 \in \overset{\circ}{A}$, nếu $y \neq 0$; điều này hiển nhiên đúng nếu $y = 0$.

#### Hệ quả 2 {#evt-ii-s2-prop-16-cor-2 .statement}

— *Phần trong* $\dot{C}$ *của một nón lồi* C, *tự nó là một nón lồi; nếu* $\dot{C}$ *không rỗng thì nó trùng với phần trong của* $\overline{C}$, *và* $\overline{C}$ *là một nón lồi nhọn trùng với bao đóng của* $\dot{C}$.

Vì các phép vị tự có tỉ số $> 0$ và tâm 0 biến C thành chính nó, nên chúng cũng biến $\dot{C}$ thành chính nó, do đó $\dot{C}$ là một nón; phần còn lại của hệ quả suy ra từ hệ quả 1 và nhận xét hiển nhiên rằng nếu C không rỗng thì $\overline{C}$ chứa đỉnh của C.

Cho H là một siêu phẳng đóng trong không gian vectơ tôpô E trên $\mathbf{R}$; nó có phương trình dạng $f(x) = \alpha$, trong đó $f$ là một dạng tuyến tính liên tục không đồng nhất bằng không trên E (I, p. 13, định lý 1). Các nửa không gian đóng được xác định tương ứng bởi $f(x) \leqslant \alpha$ và $f(x) \geqslant \alpha$ do đó là các tập hợp lồi *đóng*; các phần bù của chúng được xác định tương ứng bởi $f(x) > \alpha$ và $f(x) < \alpha$, là các tập hợp lồi *mở*. Ta nói rằng các nửa không gian này là các nửa không gian đóng (t.ư. mở) *được xác định* bởi H.

#### Mệnh đề 17 {#evt-ii-s2-prop-17 .statement}

— *Trong một không gian vectơ tôpô* E, *cho* A *là một tập hợp có ít nhất một điểm trong, và sao cho tất cả các điểm của nó nằm cùng một phía của một siêu phẳng* H. *Khi đó* H *là đóng, các điểm trong của* A *nằm ngặt cùng một phía của* H, *và các điểm tụ của* A *nằm cùng phía của* H. *Đặc biệt các nửa không gian mở (t.ư. đóng) được xác định bởi các siêu phẳng đóng*.

Thật vậy, giả sử H chứa gốc và $f(x) = 0$ là một phương trình của H; giả sử, để xác định, rằng $f(x) \geqslant 0$ với mọi $x \in A$. Nửa không gian tạo bởi các điểm y sao cho $f(y) > -1$ chứa ít nhất một điểm trong, và, bằng phép tịnh tiến, điều tương tự cũng đúng đối với nửa không gian các điểm y sao cho $f(y) > 0$; điều này chứng tỏ H là đóng (I, p. 11, hệ quả). Khi đó ta biết rằng $f$ là một cấu xạ ngặt của E vào $\mathbf{R}$ (I, p. 13, hệ quả), do đó $f(\dot{A})$ là một tập hợp mở trong $\mathbf{R}$. Tập hợp này không thể chứa 0, vì khi đó nó sẽ chứa các số $< 0$ trái với giả thiết; do đó nó được chứa trong khoảng mở $]0, +\infty[$. Mặt khác, nửa không gian gồm những y sao cho $f(y) \geqslant 0$ là đóng và chứa A, do đó nó chứa $\overline{A}$.

#### Hệ quả {#evt-ii-s2-n6-cor-1 .statement}

— *Cho* P *là một nón lồi nhọn, có ít nhất một điểm trong, của không gian vectơ tôpô* E. *Khi đó mỗi dạng tuyến tính* f *không đồng nhất bằng không trên* E, *và dương đối với cấu trúc tiền thứ tự được xác định bởi* P (II, p. 13), *nhất thiết liên tục*. *Hơn nữa, nếu* x *là điểm trong của* P *thì* $f(x) > 0$ *và nếu* x *là điểm tụ của* P *thì* $f(x) \geqslant 0$.

Áp dụng mệnh đề 17 vào trường hợp $A = P$ trong đó H là siêu phẳng có phương trình $f(x) = 0$.

#### Nhận xét {#evt-ii-s2-n6-rem-1 .statement}

Trong một không gian vectơ tôpô E, mọi tập hợp lồi C đều liên thông. Thật vậy, nếu $a \in C$, thì C là hợp của các đoạn có đầu mút a và đóng tại a; các đoạn này liên thông và kết quả suy ra từ GT, I, § 11.1, mệnh đề 2.

### 7. Tôpô trên các không gian vectơ có thứ tự

Cho E là một không gian vectơ có thứ tự. Một tôpô trên E là *tương thích* với cấu trúc không gian vectơ có thứ tự của E nếu nó vừa tương thích với cấu trúc không gian vectơ của E vừa thỏa mãn tiên đề sau :

(TO) *Nón lồi của các* x *với* $x \geqslant 0$, *là đóng trong* E.

Một không gian vectơ có thứ tự E với một tôpô tương thích được gọi là một không gian vectơ tôpô có thứ tự.

#### Ví dụ {#evt-ii-s2-n7-exa-1 .statement}

Không gian $\mathbf{R}^n$ với tôpô thông thường của nó và cấu trúc thứ tự là tích của cấu trúc thứ tự của các thừa số của nó là một không gian vectơ tôpô có thứ tự. Mặt khác, với $n \geq 2$, khi $\mathbf{R}^n$ mang thứ tự từ điển (S, III, § 2.6), tôpô thông thường không tương thích với cấu trúc không gian vectơ có thứ tự của $\mathbf{R}^n$.

Cho A là một tập hợp; không gian vectơ $\mathcal{B}(A ; \mathbf{R})$ của các hàm bị chặn nhận giá trị thực được định nghĩa trên A, với tôpô được xác định bởi chuẩn $\|x\| = \sup_{t \in A} |x(t)|$ và cấu trúc thứ tự cảm sinh bởi cấu trúc thứ tự tích của $\mathbf{R}^A$, là một không gian vectơ tôpô có thứ tự.

Trong một không gian vectơ tôpô có thứ tự E, tập các phần tử $x \leq 0$ là đóng; vì các phép tịnh tiến là các đồng phôi, ta suy ra rằng, với mọi $a \in E$, tập các phần tử $x \geq a$ (resp. $x \leq a$) là đóng. Vì $\{0\}$ là giao của các tập $x \geq 0$ và $x \leq 0$, suy ra $\{0\}$ là đóng và E là Hausdorff.

#### Mệnh đề 18 {#evt-ii-s2-prop-18 .statement}

Trong một không gian vectơ tôpô có thứ tự E, cho H là một tập hợp có hướng bởi quan hệ $\leq$. Nếu bộ lọc tiết diện của H có một giới hạn trong E, thì giới hạn này là cận trên của H.

Thật vậy, cho $b = \lim_{x \in H} x$; với mọi $y \in H$, tập các $x \in H$ sao cho $x \geq y$ là một tập của bộ lọc tiết diện của H, do đó b là một điểm tụ của tập này; nhưng vì tập $x \geq y$ là đóng trong E, ta có $b \geq y$, vậy b là một cận trên của H. Mặt khác, nếu a là một cận trên của H, thì H được chứa trong tập đóng $x \leq a$; vì b là một điểm tụ của H, ta có $b \leq a$, điều này hoàn thành chứng minh (II, p. 72, exerc. 42).

### 8. Hàm lồi

#### Định nghĩa 5 {#evt-ii-s2-def-5 .statement}

Cho X là một tập con lồi của không gian afin E. Một hàm hữu hạn nhận giá trị thực, được định nghĩa trên X, là lồi (resp. lồi chặt) nếu với bất kỳ hai điểm phân biệt x, y của X và bất kỳ số thực $\lambda, 0 < \lambda < 1$, ta có:

(1)
$$
f(\lambda x + (1 - \lambda) y) \leq \lambda f(x) + (1 - \lambda) f(y)
$$
(resp.

(2)
$$
f(\lambda x + (1 - \lambda) y) < \lambda f(x) + (1 - \lambda) f(y)).
$$

Khi $E = \mathbf{R}$, định nghĩa này của hàm lồi trùng với định nghĩa trong FVR, I, p. 32. Hơn nữa, f là lồi (resp. lồi chặt) trong X nếu, và chỉ nếu, với mọi đường thẳng afin $D \subset E$, hạn chế của f lên $X \cap D$ là lồi (resp. lồi chặt) trong $X \cap D$.

#### Ví dụ {#evt-ii-s2-n8-exa-1 .statement}

Nếu f là một hàm afin tuyến tính trên E, thì f và $f^2$ là các hàm lồi trên E; điều này hiển nhiên đối với f vì
$$
f(\lambda x + (1 - \lambda) y) = \lambda f(x) + (1 - \lambda) f(y);
$$
mặt khác, nếu $\alpha = f(x), \beta = f(y)$, thì;
$$
\lambda \alpha^2 + (1 - \lambda) \beta^2 - (\lambda \alpha + (1 - \lambda) \beta)^2 = \lambda(1 - \lambda) (\alpha - \beta)^2 \geq 0
$$

với $0 < \lambda < 1$; hơn nữa, hạn chế của $f^2$ lên một đường thẳng afin $D \subset E$ là *lồi chặt nếu $f|D$ không phải là một hằng số*.

Một hàm nhận giá trị thực $f$, được định nghĩa trên $X$, là *lõm* (resp. *lõm chặt*) nếu — $f$ là lồi (resp. lồi chặt). Nghĩa là, với mọi hai điểm phân biệt $x, y$ của $X$ và mọi số $\lambda$, sao cho $0 < \lambda < 1$, ta có

$$
f(\lambda x + (1 - \lambda) y) \geqslant \lambda f(x) + (1 - \lambda) f(y)
$$

(resp.

$$
f(\lambda x + (1 - \lambda) y) > \lambda f(x) + (1 - \lambda) f(y)).
$$

Một ánh xạ từ $X$ vào $\mathbf{R}$ là *afin* nếu nó vừa lồi vừa lõm (*cf.* II, p. 78, exerc. 11).

#### Mệnh đề 19 {#evt-ii-s2-prop-19 .statement}

*Cho $X$ là một tập hợp lồi của không gian afin $E$; và cho $f$ là một hàm thực xác định trên $X$. Ký hiệu tập hợp các điểm $(x, a) \in E \times \mathbf{R}$ sao cho $x \in X$ và $f(x) \leqslant a$ (tương ứng $x \in X$ và $f(x) < a$) bởi $F$ (tương ứng $F'$). Khi đó các điều kiện sau là tương đương*:

a) *Hàm $f$ là lồi*.
b) *Tập hợp $F$ trong không gian afin $E \times \mathbf{R}$ là lồi*.
c) *Tập hợp $F'$ trong không gian afin $E \times \mathbf{R}$ là lồi*.

Ta chứng minh rằng $a) \Rightarrow c)$. Cho $(x, a)$ và $(y, b)$ là hai điểm của $F'$ và $0 < \lambda < 1$, khi đó $f(x) < a,\ f(y) < b$ và nếu $f$ là lồi

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) < \lambda a + (1 - \lambda) b
$$

điều này cho thấy điểm $\lambda(x, a) + (1 - \lambda)(y, b)$ của $E \times \mathbf{R}$ thuộc $F'$. Do đó $F'$ là lồi.

Tiếp theo ta chứng minh rằng $c) \Rightarrow b)$. Nếu $(x, a), (y, b)$ là hai điểm của $F$ thì với mọi $\varepsilon > 0$, $(x, a + \varepsilon)$ và $(y, b + \varepsilon)$ thuộc $F'$ và, nếu $0 < \lambda < 1$, điều tương tự cũng đúng với $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b + \varepsilon)$; theo định nghĩa của $F$, điều này suy ra rằng $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ thuộc $F$.

Cuối cùng $b) \Rightarrow a)$, vì (với ký hiệu trên), nếu $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ thuộc $F$ thì

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda a + (1 - \lambda) b
$$

với điều kiện $a \geqslant f(x)$ và $b \geqslant f(y)$; do đó (1) suy ra và $f$ là lồi.

#### Hệ quả {#evt-ii-s2-n8-cor-1 .statement}

*Nếu $f$ là lồi trên $X$, thì với mọi $\alpha \in \mathbf{R}$, tập hợp các $x \in X$ sao cho $f(x) \leqslant \alpha$ (tương ứng $f(x) < \alpha$) là lồi*.

Thật vậy, đó là phép chiếu lên $E$ của giao của $F$ (tương ứng $F'$) và siêu phẳng $E \times \{\alpha\}$ trong $E \times \mathbf{R}$.

#### Mệnh đề 20 {#evt-ii-s2-prop-20 .statement}

*Cho $f$ là một hàm lồi, xác định trên một tập hợp lồi $X$ của không gian affine* E. Khi đó với mọi họ $(x_i)_{1 \leq i \leq p}$ gồm $p$ điểm của X và mọi họ $(\lambda_i)_{1 \leq i \leq p}$ gồm $p$ số thực, tất cả $\geq 0$, sao cho $\sum_{i=1}^p \lambda_i = 1$, ta có:

(3)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

Nếu $f$ là hàm lồi nghiêm ngặt và $\lambda_i > 0$ với mọi $i$, thì

(4)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i),
$$
trừ khi tất cả các $x_i$ bằng nhau.

Bất đẳng thức (3) suy ra từ II, mệnh đề 19 ở trên và II, p. 8, mệnh đề 1. Giả sử rằng các $x_i$ không tất cả bằng nhau (điều này kéo theo $p \geq 2$) và các $\lambda_i$ đều $> 0$; khi đó điểm $z = \sum_{i=1}^p \lambda_i x_i$ khác ít nhất một $x_i$. Không mất tính tổng quát, giả sử $z \neq x_1$, viết $z = \lambda_1 x_1 + (1 - \lambda_1) y_1$ trong đó $y_1 = \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} x_i$. Khi đó $y_1 \neq x_1$ và, vì $0 < \lambda_1 < 1$, theo giả thiết, ta có
$$
f(z) < \lambda_1 f(x_1) + (1 - \lambda_1) f(y_1).
$$
Nhưng theo (3) $f(y_1) \leq \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} f(x_i)$, và bất đẳng thức (4) suy ra.

### 9. Các phép toán trên các hàm lồi

Cho X là một tập hợp lồi của một không gian affine E. Nếu $f_i (1 \leq i \leq p)$ là hữu hạn hàm lồi xác định trên X và $c_i (1 \leq i \leq p)$ là các số $\geq 0$ thì hàm $f = \sum_{i=1}^p c_i f_i$ là lồi trên X.

Nếu $(f_i)$ là một họ bất kỳ các hàm lồi xác định trên X và nếu $g$, bao trên của họ trong X, là hữu hạn thì $g$ là lồi.

Cuối cùng, nếu H là một tập hợp các hàm lồi xác định trên X, và $\mathfrak{F}$ là một bộ lọc trên H hội tụ đơn giản trong X tới hàm thực hữu hạn $f_0$, thì $f_0$ là lồi trên X.

### 10. Các hàm lồi trên một tập hợp lồi mở

#### Mệnh đề 21 {#evt-ii-s2-prop-21 .statement}

Cho $f$ là một hàm lồi, xác định trên tập hợp lồi mở khác rỗng X trong không gian vectơ tôpô E. Khi đó $f$ liên tục khi và chỉ khi nó bị chặn trên khi hạn chế trên một tập con mở khác rỗng U của X.

Điều kiện này hiển nhiên là cần thiết, ta chứng minh rằng nó là đủ. Cho $x_0 \in X$ là một điểm sao cho $f$ bị chặn trên trong một lân cận V của $x_0$; trước hết ta chỉ ra rằng $f$ liên tục tại $x_0$. Bằng phép tịnh tiến, ta có thể tự giới hạn vào trường hợp $x_0 = 0$ và $f(x_0) = 0$; hơn nữa ta có thể giả sử rằng lân cận V là cân bằng (I, p. 7, mệnh đề 4). Giả sử rằng $f(x) \leq a$ trong V; với mọi $\varepsilon, 0 < \varepsilon < 1$, ta nhận thấy rằng nếu $x \in \varepsilon V$, thì $x/\varepsilon \in V$ và $-x/\varepsilon \in V$. Áp dụng bất đẳng thức (1) của II, p. 16 cho các điểm $x/\varepsilon$ và 0 và cho số $\lambda = \varepsilon$, ta thấy rằng $f(x) \leq \varepsilon f(x/\varepsilon) \leq \varepsilon a$; áp dụng nó cho các điểm $x$ và $-x/\varepsilon$ và số $\lambda = 1/(1 + \varepsilon)$, ta được $f(x) \geq -\varepsilon f(-x/\varepsilon) \geq -\varepsilon a$. Do đó $f(x)$ nhỏ tùy ý trong $\varepsilon V$, nếu $\varepsilon$ đủ nhỏ, và $f$ liên tục tại $x = 0$.

Bây giờ cho $y$ là một điểm bất kỳ của X; vì X là mở, tồn tại một số $\rho > 1$ sao cho $z = \rho y$ thuộc X. Gọi $g$ là phép vị tự $x \mapsto \lambda x + (1 - \lambda)z$ có tâm $z$ và tỉ số $\lambda = 1 - \frac{1}{\rho}$, biến 0 thành $y$; với mọi điểm $g(x) \in g(V)$, từ (1) ta có

$$
f(g(x)) \leq \lambda f(x) + (1 - \lambda) f(z) \leq \lambda a + (1 - \lambda) f(z) .
$$

Do đó $f$ bị chặn trên trong một lân cận của $y$ và vì thế, theo phần đầu, liên tục tại $y$. Mệnh đề được chứng minh.

#### Hệ quả {#evt-ii-s2-n10-cor-1 .statement}

*Mọi hàm lồi f xác định trên một tập hợp lồi mở X trong $\mathbf{R}^n$ đều liên tục trong X.*

Ta có thể giả sử rằng X không rỗng. Khi đó tồn tại trong X, $n + 1$ điểm độc lập afin $a_i$ ($0 \leq i \leq n$) và bao lồi của các điểm này, S, chứa tập hợp mở không rỗng gồm các điểm $\sum_{i=0}^n \lambda_i a_i$ với $0 < \lambda_i < 1$ đối với mọi $i$ và $\sum_{i=0}^n \lambda_i = 1$. Theo II, p. 17, mệnh đề 20, $f$ bị chặn trên trong S và do đó liên tục.

Trong một không gian vectơ tôpô vô hạn chiều, nói chung tồn tại các dạng tuyến tính không liên tục (II, p. 80, bài tập 25) và do đó các hàm lồi không liên tục tại bất kỳ điểm nào.

### 11. Nửa chuẩn và các tập hợp lồi

Cho E là một không gian vectơ trên $\mathbf{R}$; một ánh xạ $p$ từ E vào $\mathbf{R}$ được gọi là *thuần nhất dương* nếu, với mọi $\lambda \geq 0$ và mọi $x \in E$ ta có

$$
p(\lambda x) = \lambda p(x) .
$$

Một hàm thuần nhất dương $p$ trên E là lồi nếu và chỉ nếu nó thỏa mãn tiên đề (SN$_{\text{II}}$) của II, p. 1 đối với mọi $x, y$ của E;

$$
p(x + y) \leq p(x) + p(y) .
$$

Thật vậy, nếu $p$ là lồi, thì với $x, y$ trong E,

$$
p(\frac{1}{2}(x + y)) \leq \frac{1}{2}p(x) + \frac{1}{2}p(y)
$$

và theo (5), quan hệ này tương đương với (6). Ngược lại, nếu (6) đúng thì ta cũng có với mọi $\lambda$ sao cho $0 < \lambda < 1$,

$$
p(\lambda x + (1 - \lambda) y) \leq p(\lambda x) + p((1 - \lambda) y) = \lambda p(x) + (1 - \lambda) p(y)
$$

theo (5).

Một hàm thuần nhất dương lồi trên E được gọi là *nửa tuyến tính*.

Nếu $p$ là một hàm nửa tuyến tính xác định trên E; thì theo II, § 2.8, hệ quả, với mọi $a > 0$, tập hợp $V(p, a)$ (tương ứng $W(p, a)$) gồm các điểm $x \in E$ sao cho $p(x) \leq a$ (tương ứng $p(x) < a$) là lồi; hơn nữa tập hợp này là *hấp thụ được*, vì với mọi $x \in E$, tồn tại $\lambda > 0$ sao cho $p(\lambda x) = \lambda p(x) < a$.

Có một đảo lại một phần của kết quả này:

#### Mệnh đề 22 {#evt-ii-s2-prop-22 .statement}

*Cho A là một tập hợp lồi, chứa 0, trong không gian vectơ E. Với mọi $x \in E$, đặt*

$$
p_A(x) = \inf_{\rho > 0, x \in \rho A} \rho
$$
(0 $\leq p_A(x) \leq \infty$). *Hàm $p_A$ thỏa mãn*
$$
p_A(x + y) \leq p_A(x) + p_A(y), \qquad p_A(\lambda x) = \lambda p_A(x)
$$
\* với mọi $x, y$ trong E và $\lambda > 0$. Nếu $V(p_A, \alpha)$ (tương ứng $W(p_A, \alpha)$) ký hiệu tập hợp các $x \in E$ sao cho $p_A(x) \leq \alpha$ (tương ứng $p_A(x) < \alpha$), thì*
$$
W(p_A, 1) \subset A \subset V(p_A, 1).
$$
*Nếu A hấp thụ được thì $p_A$ hữu hạn* (do đó *nửa tuyến tính*).

Vì các quan hệ $x \in \rho A$ và $\lambda x \in \lambda \rho A$ là tương đương khi $\lambda > 0$, ta có $p_A(\lambda x) = \lambda p_A(x)$ với $\lambda > 0$. Cho $x, y$ là hai điểm của E. Nếu $x$ (tương ứng $y$) không bị A hấp thụ thì $p_A(x) = +\infty$ (tương ứng $p_A(y) = +\infty$) và bất đẳng thức $p_A(x + y) \leq p_A(x) + p_A(y)$ là hiển nhiên đúng. Giả sử tồn tại $\alpha > 0, \beta > 0$ sao cho $x \in \alpha A$, và $y \in \beta A$; khi đó $x + y \in \alpha A + \beta A = (\alpha + \beta) A$ (II, p. 8, *Nhận xét*); và do đó $p_A(x + y) \leq p_A(x) + p_A(y)$. Bao hàm $A \subset V(p_A, 1)$ là rõ ràng. Bao hàm $W(p_A, 1) \subset A$ suy ra vì A là lồi và chứa 0. Cuối cùng nếu A hấp thụ được thì $p_A$ hiển nhiên hữu hạn.

Hàm $p_A$ được xác định bởi (7) được gọi là *hàm gauge* của tập hợp lồi A. Nếu A hấp thụ được và đối xứng, thì $p_A$ là một nửa chuẩn.

#### Mệnh đề 23 {#evt-ii-s2-prop-23 .statement}

*Cho E là một không gian vectơ tôpô. Nếu A là một tập hợp lồi mở chứa 0, thì $p_A$ hữu hạn và liên tục, và $A = W(p_A, 1)$. Nếu A là một tập hợp lồi đóng chứa 0, thì $p_A$ nửa liên tục dưới và $A = V(p_A, 1)$.*

Nếu A mở và chứa 0 thì nó hấp thụ được. Với $x \in A$, tồn tại $\rho < 1$ sao cho $x / \rho \in A$, và do đó $p_A(x) < 1$; điều này, kết hợp với (9), cho $A = W(p_A, 1)$. Vì hàm lồi $p_A$ bị chặn trên trong tập hợp mở A, nên nó liên tục trong E (II, p. 18, mệnh đề 21).

Giả sử A là đóng và chứa 0. Với mọi $x \in E$ sao cho $p_A(x) \leq 1$, ta có $x \in \rho A$ với mọi $\rho > 1$, do đó $x \in A$ vì A là đóng; nhớ lại (9), điều này cho thấy rằng $A = V(p_A, 1)$. Với mọi $\mu > 0$, $\mu A$ do đó là tập hợp các $x$ sao cho $p_A(x) \leq \mu$; vì $p_A(x) \geq 0$ trong E, điều này cho thấy rằng $p_A$ là nửa liên tục dưới trong E (GT, IV, § 6.2).

Một hàm dưới tuyến tính dương $p$ trên E là hàm gauge của mỗi tập lồi A sao cho $W(p, 1) \subset A \subset V(p, 1)$.

### Bài tập {#evt-ii-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
