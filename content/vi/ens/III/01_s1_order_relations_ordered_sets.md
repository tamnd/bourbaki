---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 1
section_title: Order relations. Ordered sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 131-148, 212-221
pdf_pages: 0137-0154, 0218-0227
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ORDER RELATION
      page: 131
      pdf_page: 137
    - "no": 2
      title: PREORDER RELATIONS
      page: 133
      pdf_page: 139
    - "no": 3
      title: NOTATION AND TERMINOLOGY
      page: 135
      pdf_page: 141
    - "no": 4
      title: ORDERED SUBSETS. PRODUCT OF ORDERED SETS
      page: 136
      pdf_page: 142
    - "no": 5
      title: INCREASING MAPPINGS
      page: 138
      pdf_page: 144
    - "no": 6
      title: MAXIMAL AND MINIMAL ELEMENTS
      page: 139
      pdf_page: 145
    - "no": 7
      title: GREATEST ELEMENT AND LEAST ELEMENT
      page: 140
      pdf_page: 146
    - "no": 8
      title: UPPER AND LOWER BOUNDS
      page: 141
      pdf_page: 147
    - "no": 9
      title: LEAST UPPER BOUND AND GREATEST LOWER BOUND
      page: 141
      pdf_page: 147
    - "no": 10
      title: DIRECTED SETS
      page: 145
      pdf_page: 151
    - "no": 11
      title: LATTICES
      page: 145
      pdf_page: 151
    - "no": 12
      title: TOTALLY ORDERED SETS
      page: 146
      pdf_page: 152
    - "no": 13
      title: INTERVALS
      page: 147
      pdf_page: 153
statements: 52
exercises: 24
content_sha256: 16432e6c99bb162cb614c122e8c3943c6caca06b476a78128bef36fefc624fb5
translated_from: content/en/ens/III/01_s1_order_relations_ordered_sets.md
source_content_sha256: 9aa0ba9c66e0e7562086ef9405dfbe251e949c96f337a2aa1a7cc6d19e72765c
translation_model: gpt-5.4-mini, gpt-5.4
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: 67f0216f2f8c9b554e20fcaa99b25ef1f42ac8b5d01a8ddb96951dec2c4b2106
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. Quan hệ thứ tự. Tập hợp có thứ tự

### 1. Định nghĩa của một quan hệ thứ tự

Cho $R\{x, y\}$ là một quan hệ, $x$ và $y$ là các chữ cái phân biệt. R được gọi là một *quan hệ thứ tự đối với các chữ cái x và y* (hoặc *giữa x và y*) nếu

$$(R\{x,\, y\} \ \text{ và } \ R\{\, y,\, z\}) \Rightarrow R\{x,\, z\},$$
$$(R\{x,\, y\} \ \text{ và } \ R\{\, y,\, x\}) \Rightarrow (x = y),$$
$$R\{x, y\} \Rightarrow (R\{x,\, x\} \ \text{ và } \ R\{\, y,\, y\}).$$

Quan hệ thứ nhất ở trên nói rằng R là *bắc cầu* đối với các chữ cái $x$ và $y$ (Chương II, § 6, no. 1).

*Ví dụ*

(1) Quan hệ đẳng thức, $x = y$, là một quan hệ thứ tự.

(2) Quan hệ $X \subset Y$ là một quan hệ thứ tự giữa X và Y (Chương II, § 1, no. 2, Mệnh đề 1 và 2 và tiên đề A1) mà thường được gọi là *quan hệ bao hàm*.

(3) Cho $R\{x, y\}$ là một quan hệ thứ tự giữa $x$ và $y$. Khi đó quan hệ $R\{\, y,\, x\}$ là một quan hệ thứ tự *giữa x và y*, gọi là *quan hệ đối* của quan hệ thứ tự $R\{x,\, y\}$.

Một *quan hệ thứ tự trên một tập hợp* E là một quan hệ thứ tự $R\{x,\, y\}$ đối với hai chữ cái phân biệt $x$, $y$ sao cho quan hệ $R\{x,\, x\}$ là *tương đương với* $x \in E$ (nói cách khác, là sao cho $R\{x,\, y\}$ là *phản xạ* trên E (Chương II, § 6, số 1)). Khi đó quan hệ $R\{x,\, y\}$ kéo theo "$x \in E$ và $y \in E$" và quan hệ $(R\{x,\, y\}$ và $R\{\, y,\, x\})$ là tương đương với "$x \in E$ và $y \in E$ và $x = y$".

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n1-exa-1 .statement tag=03SH}

Các quan hệ đẳng thức và bao hàm không phải là các quan hệ thứ tự trên một tập hợp, vì các quan hệ $x = x$ và $\mathrm{X} \subset \mathrm{X}$ không xác định tập (Chương II, § 1, no. 7).

#### Ví dụ 2 {#ens-iii-s1-n1-exa-2 .statement tag=03SI}

Cho $\mathrm{R}\}x,\ y\{$ là một quan hệ thứ tự giữa $x$ và $y$, và cho E là một tập hợp sao cho $x \in \mathrm{E}$ kéo theo $\mathrm{R}\}x,\ x\{$ (lưu ý rằng tập rỗng thỏa mãn điều kiện này). Khi đó quan hệ "$\mathrm{R}\}x,\ y\{$ and $x \in \mathrm{E}$ and $y \in \mathrm{E}$" là một quan hệ thứ tự trên E, điều này được kiểm tra ngay lập tức; nó được gọi là quan hệ thứ tự *cảm sinh* bởi $\mathrm{R}\}x,y\{$ trên E (xem số 4). Do sự lạm dụng ngôn ngữ, cụm từ "quan hệ $\mathrm{S}\}x,\ y\{$ là một quan hệ thứ tự giữa các phần tử của E" thường được dùng thay cho "quan hệ ($\mathrm{S}\}x,\ y\{$ and $x \in \mathrm{E}$ and $y \in \mathrm{E}$) là một quan hệ thứ tự trên E". Ví dụ, nếu A là một tập hợp, thì quan hệ "$\mathrm{X} \subset \mathrm{Y}$ and $\mathrm{X} \subset \mathrm{A}$ and $\mathrm{Y} \subset \mathrm{A}$" là một quan hệ thứ tự giữa các tập con của A.

#### Ví dụ 3 {#ens-iii-s1-n1-exa-3 .statement tag=03SJ}

Cho E, F là các tập hợp. Quan hệ "*g mở rộng f*" là một quan hệ thứ tự (giữa $f$ và $g$) trên tập hợp các ánh xạ từ các tập con của E vào F.

#### Ví dụ 4 {#ens-iii-s1-n1-exa-4 .statement tag=03V3}

Trong tập hợp $\mathfrak{P}(\mathfrak{P}(\mathrm{E}))$ gồm các tập hợp các tập con của một tập hợp E, gọi $\mathscr{P}$ là tập hợp các *phân hoạch* của E (Chương II, § 4, no. 7). Ta nhắc lại rằng một phân hoạch $\varpi$ được gọi là *thô hơn* một phân hoạch $\varpi'$ nếu với mọi $\mathrm{Y} \in \varpi'$ tồn tại $\mathrm{X} \in \varpi$ sao cho $\mathrm{Y} \subset \mathrm{X}$ (Chương II, § 4, no. 6). Với mỗi phân hoạch $\varpi$ của E, gọi $\tilde{\varpi}$ là đồ thị của quan hệ tương đương được định nghĩa bởi $\varpi$ trên E (Chương II, § 6, no. 2), nghĩa là hợp của các tập hợp $\mathrm{A} \times \mathrm{A}$ (đôi một rời nhau), trong đó A chạy qua $\varpi$. Ngay lập tức thấy rằng quan hệ "$\varpi$ thô hơn $\varpi'$" tương đương với $\tilde{\varpi} \supset \tilde{\varpi}'$, và do đó là một quan hệ thứ tự trên tập hợp $\mathscr{P}$ giữa $\varpi$ và $\varpi'$.

Một *thứ tự* trên một tập hợp E là một sự tương ứng $\Gamma = (\mathrm{G},\ \mathrm{E},\ \mathrm{E})$ có E làm nguồn và làm đích, và sao cho quan hệ $(x,\ y) \in \mathrm{G}$ là một quan hệ thứ tự trên E. Theo lối nói lạm dụng, đôi khi chúng tôi sẽ gọi đồ thị G của $\Gamma$ là một thứ tự trên E. Nếu $\mathrm{R}\}x,\ y\{$ là một quan hệ thứ tự trên E, thì nó có một đồ thị là một thứ tự trên E.

#### Mệnh đề 1 {#ens-iii-s1-prop-1 .statement tag=03JA}

*Một sự tương ứng* $\Gamma$ *giữa* E *và* E *là một thứ tự trên* E *khi và chỉ khi đồ thị của nó* G *thỏa mãn các điều kiện sau :*

(a) $\mathrm{G} \circ \mathrm{G} = \mathrm{G}$.

(b) *Tập hợp* $\mathrm{G} \cap \overset{-1}{\mathrm{G}}$ *là đường chéo* $\Delta$ *của* $\mathrm{E} \times \mathrm{E}$.

Thật vậy, quan hệ $((x,\ y) \in \mathrm{G}$ và $(y,\ z) \in \mathrm{G}) \Rightarrow ((x,\ z) \in \mathrm{G})$ có thể được viết thành $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$, và quan hệ

$$((x,\ y) \in \mathrm{G} \text{ và } (y,\ x) \in \mathrm{G}) \Leftrightarrow (x = y \text{ và } x \in \mathrm{E} \text{ và } y \in \mathrm{E})$$

có thể được viết thành $\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$. Từ $\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$ khi đó ta suy ra $\Delta \subset \mathrm{G}$, do đó $\mathrm{G} = \Delta \circ \mathrm{G} \subset \mathrm{G} \circ \mathrm{G}$; vì cũng có $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$, nên ta có

$$\mathrm{G} \circ \mathrm{G} = \mathrm{G}.$$

### 2. CÁC QUAN HỆ TIỀN THỨ TỰ

Cho $R\{x, y\}$ là một quan hệ, $x$ và $y$ là các chữ cái phân biệt. Nếu $R$ là bắc cầu và nếu ta có $R\{x, y\} \Rightarrow (R\{x, x\}$ and $R\{y, y\})$, thì không tất yếu suy ra rằng $R$ là một quan hệ thứ tự, bởi vì quan hệ

$$(R\{x, y\} \text{ và } R\{y, x\})$$

không tất yếu suy ra $x = y$. $R\{x, y\}$ được gọi là một *quan hệ tiền thứ tự* giữa $x$ và $y$; khi đó $R\{y, x\}$ cũng là một quan hệ tiền thứ tự giữa $x$ và $y$, gọi là *đối* của quan hệ $R\{x, y\}$.

Ví dụ, cho $\mathfrak{R}$ là tập các tập con của $\mathfrak{P}(E)$ tạo thành các phủ của E (Chương II, § 4, số 6). Quan hệ "$\mathfrak{R}$ thô hơn $\mathfrak{R}'$" giữa các phần tử $\mathfrak{R}$, $\mathfrak{R}'$ của $\mathfrak{R}$ (Chương II, § 4, số 6) là bắc cầu và phản xạ. Nhưng hai phủ phân biệt có thể sao cho mỗi phủ thô hơn phủ kia; ví dụ, đó là trường hợp khi $\mathfrak{R}'$ là hợp (trong $\mathfrak{P}(E)$) của $\mathfrak{R}$ và một tập con của E được chứa trong một tập của $\mathfrak{R}$ nhưng không thuộc $\mathfrak{R}$.

Nhưng trong mọi trường hợp, quan hệ $(R\{x, y\}$ và $R\{y, x\})$ là một *quan hệ tương đương* $S\{x, y\}$ đối với $x$ và $y$. Gọi $x'$, $y'$ là những chữ cái phân biệt với $x$, $y$ và không xuất hiện trong R. Khi đó $R\{x, y\}$ *tương thích* (đối với $x$ và $y$) với các quan hệ tương đương $S\{x, x'\}$ và $S\{y, y'\}$; nói cách khác (Chương II, § 6, no. 8), quan hệ

$$(R\{x, y\} \text{ và } S\{x, x'\} \text{ và } S\{y, y'\})$$

suy ra $R\{x', y'\}$.

¶ Một *quan hệ tiền thứ tự trên một tập hợp* E là một quan hệ tiền thứ tự $R\{x, y\}$ sao cho quan hệ $R\{x, x\}$ tương đương với $x \in E$. Khi đó quan hệ $R\{x, y\}$ suy ra "$x \in E$ và $y \in E$".

¶ Nếu $R\{x, y\}$ là một quan hệ tiền thứ tự trên một tập hợp E, thì quan hệ $S\{x, y\}$ được định nghĩa ở trên là một quan hệ tương đương trên E. Gọi $R'\{X, Y\}$ là quan hệ

$$X \in E/S \text{ và } Y \in E/S \text{ và } (\exists x)(\exists y)(x \in X \text{ và } y \in Y \text{ và } R\{x, y\}),$$

nghĩa là, quan hệ cảm sinh bởi R khi chuyển qua thương (đối với $x$ và $y$); ta đã thấy trong Chương II, § 6, số 3, rằng nó tương đương với quan hệ

$$X \in E/S \text{ và } Y \in E/S \text{ và } (\forall x)(\forall y)((x \in X \text{ và } y \in Y) \Rightarrow R\{x, y\}).$$

¶ Ta hãy chỉ ra rằng $R'\{X, Y\}$ là một *quan hệ thứ tự* giữa các phần tử của E/S. Quan hệ $(R'\{X, Y\}$ and $R'\{Y, Z\})$ tương đương với

$$X \in E/S \text{ và } Y \in E/S \text{ và } Z \in E/S \text{ và }$$
$$(\forall x)(\forall y)(\forall z)((x \in X \text{ và } y \in Y \text{ và } z \in Z) \Rightarrow (R\{x, y\} \text{ và } R\{y, z\}))$$

(Chương I, § 4, các tiêu chuẩn C40, C41). Vì $R\{x, y\}$ là bắc cầu và $Y \in E/S \Rightarrow Y \neq \emptyset$ (Chương II, § 6, no. 2), suy ra ngay lập tức rằng $R'\{X, Y\}$ là bắc cầu. Tiếp theo, $(R'\{X, Y\}$ and $R'\{Y, X\})$ tương đương với

$$X \in E/S \text{ và } Y \in E/S \text{ và }$$
$$(\forall x)(\forall y) \ ((x \in X \text{ và } y \in Y) \Rightarrow (R\{x, y\} \text{ và } R\{y, x\})),$$

và do đó tương đương với

$$X \in E/S \text{ và } Y \in E/S \text{ và } (\forall x)(\forall y)((x \in X \text{ và } y \in Y) \Rightarrow S\{x, y\}),$$

và vì thế suy ra

$$X \in E/S \quad \text{và} \quad Y \in E/S \quad \text{và} \quad X = Y.$$

Hơn nữa, $R\{x, y\}$ suy ra $R\{x, x\}$ và $R\{y, y\}$, và do đó $R'\{X, Y\}$ suy ra từng quan hệ

$$X \in E/S \text{ và } (\forall x)((x \in X) \Rightarrow R\{x, x\}),$$
$$Y \in E/S \text{ và } (\forall y)((y \in Y) \Rightarrow R\{y, y\}),$$

do đó $R'\{X, Y\}$ suy ra $(R'\{X, X\}$ và $R'\{Y, Y\})$. Cuối cùng, vì $x \in E$ suy ra $R\{x, x\}$, $X \in E/S$ suy ra $R'\{X, X\}$, và chứng minh của mệnh đề này là xong. $R'\{X, Y\}$ được gọi là quan hệ thứ tự *liên kết* với $R\{x, y\}$.

¶ Một *tiền thứ tự* trên một tập hợp E là một sự tương ứng $\Gamma = (G, E, E)$ có E làm nguồn và làm đích, và sao cho $(x, y) \in G$ là một quan hệ tiền thứ tự trên E. Do lạm dụng ngôn ngữ, đôi khi ta gọi đồ thị G của $\Gamma$ là một tiền thứ tự trên E. Điều cần và đủ để như vậy là $\Delta \subset G$ và $G \circ G \subset G$ (điều này kéo theo $G \circ G = G$). Khi đó quan hệ tương đương S tương ứng với quan hệ tiền thứ tự $(x, y) \in G$ có $G \cap \overset{-1}{G}$ làm đồ thị; quan hệ thứ tự liên kết với $(x, y) \in G$ có làm đồ thị tập con G' của $(E/S) \times (E/S)$ tương ứng (Chương II, § 6, no. 8) với ảnh của G dưới ánh xạ chính tắc từ $E \times E$ lên

$$(E \times E)/(S \times S).$$

#### Ví dụ {#ens-iii-s1-n2-exa-1 .statement tag=03JB}

\* Cho A là một vành có phần tử đơn vị. Quan hệ $(\exists z)(z \in \mathrm{A}$ và $y = zx)$ giữa hai phần tử $x$, $y$ của A là một quan hệ tiền thứ tự trên A; nó được đọc là "$x$ là một ước phải của $y$" hoặc "$y$ là một bội trái của $x$". \*

### 3. KÝ HIỆU VÀ THUẬT NGỮ

Các định nghĩa sẽ được nêu ở phần còn lại của tiết diện này áp dụng cho một quan hệ thứ tự (hoặc quan hệ tiền thứ tự) tùy ý $\mathrm{R}\{x, y\}$ giữa $x$ và $y$, nhưng sẽ chủ yếu được dùng trong trường hợp $\mathrm{R}\{x, y\}$ được viết là $x \leqslant y$ *(theo phép tương tự với quan hệ thứ tự thông thường giữa các số nguyên hoặc số thực)* (hoặc $x \subset y$, hoặc bằng một ký hiệu tương tự nào đó); vì vậy chúng tôi sẽ chỉ phát biểu chúng cho ký hiệu $x \leqslant y$, và để lại cho bạn đọc nhiệm vụ chuyển chúng sang các ký hiệu khác. Khi $\mathrm{R}\{x, y\}$ được viết là $x \leqslant y$, thì $y \geqslant x$ đồng nghĩa với $x \leqslant y$, và các quan hệ này được đọc là "$x$ *nhỏ hơn* $y$", hoặc "$x$ *ít hơn* $y$", hoặc "$y$ *lớn hơn* $x$", hoặc "$y$ *lớn hơn* $x$". Quan hệ $x \geqslant y$ khi đó là quan hệ tiền thứ tự (*giữa* $x$ *và* $y$) *đối* của $x \leqslant y$.

Do lạm dụng ngôn ngữ, ta sẽ thường nói đến "quan hệ $\leqslant$" thay cho "quan hệ $x \leqslant y$"; trong trường hợp này, "quan hệ $\geqslant$" là quan hệ đối của "quan hệ $\leqslant$". Ta cũng chú ý rằng, trong cùng một chứng minh, ta thường có thể dùng cùng một dấu $\leqslant$ để chỉ nhiều quan hệ thứ tự khác nhau khi không có nguy cơ nhầm lẫn.

Các điều kiện để một quan hệ viết dưới dạng $x \leqslant y$ là một quan hệ thứ tự trên một tập hợp E là như sau :

(RO$_{\mathrm{I}}$)    *Quan hệ "$x \leqslant y$ và $y \leqslant z$" kéo theo $x \leqslant z$.*
(RO$_{\mathrm{II}}$)   *Quan hệ "$x \leqslant y$ và $y \leqslant x$" kéo theo $x = y$.*
(RO$_{\mathrm{III}}$)  *Quan hệ $x \leqslant y$ kéo theo "$x \leqslant x$ và $y \leqslant y$".*
(RO$_{\mathrm{IV}}$)   *Quan hệ $x \leqslant x$ tương đương với $x \in \mathrm{E}$.*

Nếu bỏ điều kiện (RO$_{\mathrm{II}}$), ta có các điều kiện để $x \leqslant y$ là một quan hệ tiền thứ tự trên E.
¶ Khi một quan hệ thứ tự được viết là $x \leqslant y$ thì ta sẽ viết $x < y$ (hoặc $y > x$) cho quan hệ "$x \leqslant y$ and $x \neq y$"; các quan hệ này được đọc là "$x$ *nhỏ hơn nghiêm ngặt* $y$", hoặc "$x$ *bé hơn nghiêm ngặt* $y$", hoặc "$y$ *lớn hơn nghiêm ngặt* $x$", hoặc "$y$ *greater hơn nghiêm ngặt* $x$".

Ví dụ về quan hệ bao hàm cho thấy phủ định của $x \leqslant y$ (đôi khi được ký hiệu bởi $x \nleqslant y$) *không tất yếu tương đương với* $y < x$ (xem số 12).

C58. *Cho $\leqslant$ là một quan hệ thứ tự, và $x$, $y$ là hai chữ cái phân biệt. Quan hệ $x \leqslant y$ tương đương với "$x < y$ hoặc $x = y$". Mỗi quan hệ trong các quan hệ "$x \leqslant y$ và $y < z$", "$x < y$ và $y \leqslant z$" đều suy ra $x < z$.*

Mệnh đề thứ nhất suy ra từ tiêu chuẩn $A \Rightarrow ((A$ và (không $B$)) hoặc $B$) (Chương I, § 3, tiêu chuẩn C24). Để chứng minh mệnh đề thứ hai, ta nhận xét rằng mỗi giả thiết đều suy ra $x \leqslant z$, do tính bắc cầu; và quan hệ ($x = z$ và $x \leqslant y$ và $y \leqslant z$) sẽ suy ra $x = y = z$, trái với giả thiết.

¶ Để cho việc này dễ dàng hơn và để thay các tiêu chuẩn siêu toán học bằng các định lý toán học, ta thường xét một lý thuyết $\mathscr{T}$ chứa các tiên đề và các lược đồ tiên đề của lý thuyết tập hợp, và thêm vào đó, hai hằng E và $\Gamma$ thỏa mãn tiên đề

"$\Gamma$ là một thứ tự trên tập E" (số 1).

Ta sẽ ký hiệu bằng $x \leqslant y$ quan hệ $y \in \Gamma\langle x \rangle$, và ta sẽ nói rằng tập E *được sắp thứ tự bởi thứ tự* $\Gamma$ (hoặc bởi quan hệ thứ tự $y \in \Gamma\langle x \rangle$) (xem Chương IV, § 1).

¶ Mỗi khi, trong $\mathscr{T}$, $\Gamma$ là một tiền thứ tự trên E, ta cũng nói rằng E *được tiền sắp thứ tự bởi tiền thứ tự* $\Gamma$.

Trong một số tình huống (chẳng hạn trong định nghĩa sau đây), các lý thuyết mà chúng ta sẽ xét hơi phức tạp hơn một chút. Chúng tôi để cho người đọc làm tường minh các hằng và các tiên đề của những lý thuyết như vậy.

Cho E, E$'$ là hai tập hợp được sắp thứ tự bởi các thứ tự $\Gamma$, $\Gamma'$. Một *đẳng cấu của* E *lên* E$'$ (đối với các thứ tự $\Gamma$ và $\Gamma'$) là một song ánh $f$ từ E lên E$'$ sao cho các quan hệ $x \leqslant y$ và $f(x) \leqslant f(y)$ là tương đương (x. Chương IV, § 1).

### 4. TẬP HỢP CON CÓ THỨ TỰ. TÍCH CỦA CÁC TẬP HỢP CÓ THỨ TỰ

Cho E là một tập hợp được sắp thứ tự bởi một thứ tự $\Gamma$, có đồ thị G. Với mỗi tập con A của E, $G \cap (A \times A)$ là một thứ tự trên A; quan hệ thứ tự tương ứng tương đương với "$x \leqslant y$ và $x \in A$ và $y \in A$", và ta sẽ ký hiệu nó đơn giản là $x \leqslant y$ (do lạm dụng ngôn ngữ). Thứ tự và quan hệ thứ tự được định nghĩa như vậy trên A được gọi là *cảm sinh* bởi thứ tự và quan hệ thứ tự đã cho trên E; còn thứ tự và quan hệ thứ tự trên E được gọi là những *mở rộng* của thứ tự và quan hệ thứ tự mà chúng cảm sinh trên A. Mỗi khi ta xét A như một tập hợp có thứ tự, ta hiểu đó là thứ tự cảm sinh trên A bởi thứ tự trên E, trừ khi điều ngược lại được phát biểu rõ ràng.

*Ví dụ*. Các quan hệ cảm sinh bởi quan hệ bao hàm $X \subset Y$ trên những tập hợp khác nhau gồm các tập con có tầm quan trọng đáng kể. Sau đây là vài ví dụ :

#### Ví dụ 1 {#ens-iii-s1-n4-exa-1 .statement tag=03WB}

Cho E, F là hai tập hợp, và gọi $\Phi(E, F)$ là tập hợp всех ánh xạ từ các tập con của E vào F. Với mỗi $f \in \Phi(E, F)$, gọi $G_f$ là đồ thị của $f$, là một tập con của $E \times F$. Nếu ta trang bị cho $\Phi(E, F)$ quan hệ thứ tự "*g extends f*" giữa $f$ và $g$ (no. 1, Ví dụ 3), thì $f \to G_f$ là một đẳng cấu của tập hợp có thứ tự $\Phi(E, F)$ lên một tập con của $\mathfrak{P}(E \times F)$, được sắp thứ tự bởi quan hệ bao hàm.

#### Ví dụ 2 {#ens-iii-s1-n4-exa-2 .statement tag=03WC}

Với mỗi phân hoạch $\varpi$ của một tập hợp E, ký hiệu $\tilde{\varpi}$ là đồ thị của quan hệ tương đương được định nghĩa bởi $\varpi$ trên E. Ánh xạ $\varpi \to \tilde{\varpi}$ là một đẳng cấu từ tập hợp $\mathfrak{L}$ các phân hoạch của E, có thứ tự bởi quan hệ "$\varpi$ mịn hơn $\varpi'$" giữa $\varpi$ và $\varpi'$ (số 1, Ví dụ 4), lên một tập con của $\mathfrak{P}(E \times E)$, có thứ tự bởi bao hàm.

#### Ví dụ 3 {#ens-iii-s1-n4-exa-3 .statement tag=03WD}

Cho E là một tập hợp và cho $\Omega \subset \mathfrak{P}(E \times E)$ là tập hợp các đồ thị của các *tiền thứ tự* trên E (no. 2) (hoặc, do lạm dụng ngôn ngữ, là tập hợp mọi tiền thứ tự trên E). Quan hệ thứ tự $s \subset t$ giữa $s$ và $t$, được cảm sinh trên $\Omega$ bởi quan hệ bao hàm trên $\mathfrak{P}(E \times E)$, được diễn đạt bằng cách nói rằng "tiền thứ tự $s$ *mịn hơn* $t$" (hoặc rằng "$t$ *thô hơn* $s$"). Ký hiệu $x(s)y$ và $x(t)y$ lần lượt chỉ các quan hệ tiền thứ tự $(x, y) \in s$ và $(x, y) \in t$ trên E; khi đó, nói rằng $s$ mịn hơn $t$ là tương đương với việc nói rằng quan hệ $x(s)y$ *suy ra* $x(t)y$.

Cho $(E_\iota)_{\iota \in I}$ là một họ các tập hợp, và với mỗi chỉ số $\iota \in I$ cho $\Gamma_\iota$ là một thứ tự trên $E_\iota$; gọi $G_\iota \subset E_\iota \times E_\iota$ là đồ thị của nó, và ký hiệu bởi $x_\iota \leqslant y_\iota$ quan hệ thứ tự $(x_\iota, y_\iota) \in G_\iota$ trên $E_\iota$. Trên tập hợp tích $F = \prod_{\iota \in I} E_\iota$, quan hệ

$$(\forall \iota) \, ((\iota \in I) \Rightarrow (x_\iota \leqslant y_\iota))$$

là một quan hệ thứ tự giữa $x = (x_\iota)$ và $y = (y_\iota)$, như được kiểm tra ngay lập tức. Thứ tự và quan hệ thứ tự được định nghĩa như vậy trên F được gọi lần lượt là *tích của các thứ tự* $\Gamma_\iota$ và *tích của các quan hệ thứ tự* $x_\iota \leqslant y_\iota$; quan hệ này được viết là $x \leqslant y$, và tập hợp F, được sắp thứ tự bởi tích của các thứ tự $\Gamma_\iota$, được gọi là *tích của các tập hợp có thứ tự* $E_\iota$.

Người ta kiểm tra ngay lập tức rằng đồ thị của thứ tự tích trên F là ảnh của tập hợp tích $\prod_{\iota \in I} G_\iota$ dưới ánh xạ chính tắc từ $\prod_{\iota \in I} (E_\iota \times E_\iota)$ lên $F \times F$ (Chương II, § 5, no. 5).

Một ví dụ quan trọng của tích các tập hợp có thứ tự là tập hợp $F^E$ các đồ thị của những ánh xạ từ một tập hợp E vào một tập hợp có thứ tự F. Có một song ánh chính tắc từ $F^E$ lên tập hợp $\mathfrak{F}(E, F)$ các ánh xạ từ E vào F, và ánh xạ này là một đẳng cấu từ tập hợp có thứ tự $F^E$ lên $\mathfrak{F}(E, F)$ được trang bị

với thứ tự được định nghĩa bởi quan hệ "với mọi $x \in E$, $f(x) \leqslant g(x)$" giữa hai ánh xạ $f$, $g$ từ E vào F.  Quan hệ này được viết là $f \leqslant g$.

☡

Cần nhận thấy rằng trong tập hợp có thứ tự $\mathscr{F}(E, F)$, quan hệ $f < g$ có nghĩa là
$$\text{"với mọi } x \in E, f(x) \leqslant g(x), \text{ và tồn tại } y \in E \text{ sao cho } f(y) < g(y)\text{"}$$
*và không phải*
$$\text{"với mọi } x \in E, f(x) < g(x)\text{"}.$$

Để tránh nhầm lẫn, tốt hơn là không dùng ký hiệu $f < g$ trong tình huống này.

Các định nghĩa của tiểu mục này áp dụng không thay đổi cho các tập hợp tiền thứ tự khi thay "thứ tự" bằng "tiền thứ tự" ở mọi chỗ.

### 5. CÁC ÁNH XẠ TĂNG

#### Định nghĩa 1 {#ens-iii-s1-def-1 .statement tag=03JC}

*Cho* E *và* F *là các tập hợp tiền thứ tự* (*quan hệ tiền thứ tự trong mỗi tập hợp đều được ký hiệu bởi* $\leqslant$). *Một ánh xạ f từ* E *vào* F *được gọi là tăng* (hoặc *bảo toàn thứ tự*) *nếu quan hệ* $x \leqslant y$ *suy ra* $f(x) \leqslant f(y)$; *nó được gọi là giảm* (hoặc *đảo thứ tự*) *nếu quan hệ* $x \leqslant y$ *suy ra* $f(x) \geqslant f(y)$. *Một ánh xạ từ* E *vào* F *được gọi là đơn điệu nếu nó hoặc tăng hoặc giảm.*

Một ánh xạ tăng từ E vào F trở thành giảm (và ngược lại) khi ta thay *một* trong các tiền thứ tự trên E hoặc trên F bằng tiền thứ tự đối.  Mọi hàm *hằng số* đều vừa tăng vừa giảm; đảo lại của mệnh đề này thường không đúng.

Ví dụ, nếu một tập hợp E được sắp thứ tự bởi quan hệ đẳng thức, thì ánh xạ đồng nhất của E lên chính nó vừa tăng vừa giảm, nhưng không hằng nếu E có nhiều hơn một phần tử (xem Bài tập 7).

#### Định nghĩa 2 {#ens-iii-s1-def-2 .statement tag=03JD}

*Cho* E *và* F *là hai tập hợp có thứ tự. Một ánh xạ* f *từ* E *vào* F *được gọi là tăng ngặt* (hoặc *bảo toàn thứ tự ngặt*) *nếu quan hệ* $x < y$ *suy ra* $f(x) < f(y)$; *f được gọi là giảm ngặt* (hoặc *đảo thứ tự ngặt*) *nếu quan hệ* $x < y$ *suy ra* $f(x) > f(y)$. *Một ánh xạ từ* E *vào* F *được gọi là đơn điệu ngặt nếu nó hoặc tăng ngặt hoặc giảm ngặt.*

*Các ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n5-exa-1 .statement tag=03SK}

Cho E là một tập hợp.  Ánh xạ $X \rightarrow E - X$ của $\mathfrak{P}(E)$ (được sắp thứ tự bởi phép bao hàm) lên chính nó là giảm ngặt.

#### Ví dụ 2 {#ens-iii-s1-n5-exa-2 .statement tag=03SL}

Cho E là một tập hợp có thứ tự. Với mỗi $x \in E$ đặt $U_x$ là tập hợp tất cả $y \in E$ sao cho $y \geqslant x$. Ánh xạ $x \to U_x$ là một ánh xạ giảm ngặt của E vào $\mathfrak{P}(E)$ (được sắp thứ tự bởi phép bao hàm); thực vậy, quan hệ $x \leqslant y$ tương đương với $U_x \supset U_y$.

Một ánh xạ đơn ánh đơn điệu của một tập hợp có thứ tự E vào một tập hợp có thứ tự F là *đơn điệu nghiêm ngặt*; đảo lại nói chung là không đúng, vì có thể xảy ra $f(x) = f(y)$ trong khi cả hai quan hệ $x \leqslant y$, $x \geqslant y$ đều không đúng (xem no. 12, Mệnh đề 11).

¶ Một ánh xạ song ánh $f$ của một tập hợp có thứ tự E lên một tập hợp có thứ tự E' là một đẳng cấu của E lên E' (no. 3) nếu và chỉ nếu cả $f$ lẫn ánh xạ nghịch đảo của nó đều tăng.

¶ Nếu I là một tập chỉ số *có thứ tự*, thì một *họ các tập con* $(X_\iota)_{\iota \in I}$ của một tập hợp E được gọi là *tăng* nếu $\iota \to X_\iota$ là một ánh xạ tăng của I vào $\mathfrak{P}(E)$, được sắp thứ tự bởi bao hàm (nói cách khác, nếu $\iota \leqslant \varkappa$ kéo theo $X_\iota \subset X_\varkappa$). Tương tự, ta định nghĩa một họ các tập con $(X_\iota)_{\iota \in I}$ là *giảm, tăng ngặt,* hoặc *giảm nghiêm ngặt*.

#### Mệnh đề 2 {#ens-iii-s1-prop-2 .statement tag=03JE}

*Cho* E, E' *là hai tập hợp có thứ tự, và cho* $u : E \to E'$ *và* $v : E' \to E$ *là hai ánh xạ giảm sao cho với mọi* $x \in E$ *và mọi* $x' \in E'$ *ta có* $v(u(x)) \geqslant x$ *và* $u(v(x')) \geqslant x'$. *Khi đó*

$$u \circ v \circ u = u \quad \textit{và} \quad v \circ u \circ v = v.$$

Thật vậy, quan hệ $v(u(x)) \geqslant x$ kéo theo $(u(v(u(x))) \leqslant u(x)$ vì $u$ là giảm; mặt khác, ta có $u(v(u(x))) \geqslant u(x)$ do thay thế $x'$ bởi $u(x)$ trong bất đẳng thức $u(v(x')) \geqslant x'$. Do đó suy ra đẳng thức thứ nhất; chứng minh của đẳng thức thứ hai là đồng dạng.

### 6. CÁC PHẦN TỬ CỰC ĐẠI VÀ CỰC TIỂU

#### Định nghĩa 3 {#ens-iii-s1-def-3 .statement tag=03JF}

*Cho* E *là một tập hợp có thứ tự. Một phần tử* $a \in E$ *được gọi là phần tử cực tiểu* (resp. *cực đại*) *của* E *nếu quan hệ* $x \leqslant a$ (resp. $x \geqslant a$) *kéo theo* $x = a$.

Mọi phần tử cực tiểu của E đều là một phần tử cực đại đối với thứ tự đối, và ngược lại.

*Các ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n6-exa-1 .statement tag=03SM}

Cho A là một tập hợp. Trong tập con của $\mathfrak{P}(A)$ (được sắp thứ tự bởi bao hàm) gồm các tập con không rỗng của A, các phần tử cực tiểu là các tập con chỉ gồm một phần tử.

#### Ví dụ 2 {#ens-iii-s1-n6-exa-2 .statement tag=03SN}

Trong tập hợp $\Phi(E, F)$ các ánh xạ từ các tập con của E vào F (F không rỗng), được sắp thứ tự bởi quan hệ "$v$ mở rộng $u$" giữa $u$ và $v$, các phần tử cực đại là các ánh xạ từ toàn bộ E vào F.

#### Ví dụ 3 {#ens-iii-s1-n6-exa-3 .statement tag=03SO}

Trong tập hợp các số nguyên tự nhiên $> 1$, có thứ tự theo quan hệ "$m$ chia hết $n$" giữa $m$ và $n$, các phần tử cực tiểu là các số nguyên tố. $_*$

#### Ví dụ 4 {#ens-iii-s1-n6-exa-4 .statement tag=03SP}

Tập hợp các số thực không có phần tử cực đại và không có phần tử cực tiểu. $_*$

### 7. PHẦN TỬ LỚN NHẤT VÀ PHẦN TỬ NHỎ NHẤT

Nếu trong một tập hợp có thứ tự E tồn tại một phần tử $a$ sao cho $a \leqslant x$ với mọi $x \in E$, thì $a$ là phần tử *duy nhất* của E có tính chất này; thật vậy, nếu cũng có $b \leqslant x$ với mọi $x \in E$, thì ta sẽ có $a \leqslant b$ và $b \leqslant a$, và do đó $a = b$.

#### Định nghĩa 4 {#ens-iii-s1-def-4 .statement tag=03JG}

*Cho* E *là một tập hợp có thứ tự. Một phần tử* $a \in E$ *được gọi là phần tử* nhỏ nhất (resp. *lớn nhất*) *của* E *nếu với mọi* $x \in E$ *ta có* $a \leqslant x$ (resp. $x \leqslant a$).

Một tập hợp có thứ tự không nhất thiết có phần tử lớn nhất cũng không nhất thiết có phần tử nhỏ nhất. Nếu E có một phần tử nhỏ nhất $a$, thì $a$ là phần tử lớn nhất đối với thứ tự đối.

¶ Nếu E có một phần tử nhỏ nhất $a$, thì $a$ là *phần tử cực tiểu duy nhất* của E; vì nếu $x \in E$ phân biệt với $a$, ta có $a < x$.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n7-exa-1 .statement tag=03SQ}

Cho $\mathfrak{S}$ là một tập con khác rỗng của tập $\mathfrak{P}(E)$ gồm các tập con của một tập hợp E. Nếu $\mathfrak{S}$ có một phần tử nhỏ nhất (tương ứng, lớn nhất) A đối với quan hệ bao hàm, thì A là giao (tương ứng, hợp) của các tập hợp của $\mathfrak{S}$. Ngược lại, nếu giao (tương ứng, hợp) của các tập hợp của $\mathfrak{S}$ thuộc $\mathfrak{S}$, thì nó là phần tử nhỏ nhất (tương ứng, lớn nhất) của $\mathfrak{S}$.

#### Ví dụ 2 {#ens-iii-s1-n7-exa-2 .statement tag=03SR}

Đặc biệt, $\emptyset$ là phần tử nhỏ nhất và E là phần tử lớn nhất của $\mathfrak{P}(E)$. Trong tập $\Phi(E, F)$ các ánh xạ từ các tập con của E vào F, có thứ tự theo sự mở rộng của các ánh xạ (no. 1, Ví dụ 3), ánh xạ rỗng là phần tử nhỏ nhất, và không có phần tử lớn nhất trừ khi F gồm một phần tử duy nhất. Đường chéo $\Delta$ của $E \times E$ là phần tử nhỏ nhất của tập các đồ thị của các quan hệ tương đương trên E (hoặc của tập các tiền thứ tự trên E).

#### Mệnh đề 3 {#ens-iii-s1-prop-3 .statement tag=03JH}

*Cho* E *là một tập hợp có thứ tự và cho* E$'$ *là hợp rời nhau của* E *và một tập* $\{a\}$ *gồm một phần tử duy nhất. Khi đó tồn tại một thứ tự duy nhất trên* E$'$ *cảm sinh thứ tự đã cho trên* E *và sao cho* $a$ *là phần tử lớn nhất của* E$'$.

Vì nếu G là đồ thị của thứ tự trên E, thì đồ thị của một thứ tự trên E$'$ thỏa mãn các điều kiện của Mệnh đề phải là hợp G$'$ của G và tập hợp tất cả các cặp $(x, a)$ trong đó $x \in E'$; ngược lại, hiển nhiên G$'$ là đồ thị của một thứ tự trên E$'$ thỏa mãn các điều kiện đã cho.

¶ Tập hợp có thứ tự E$'$ được gọi là thu được bằng cách *thêm một phần tử lớn nhất* $a$ *vào* E (xem Bài tập 3).

¶ Một tập con A của một tập hợp tiền thứ tự E được gọi là *đồng cuối* (resp. *đồng đầu*) trong E nếu với mọi $x\in E$ tồn tại $y\in A$ sao cho $x\leq y$ (resp. $y\leq x$). Nói rằng một tập hợp có thứ tự E có một phần tử lớn nhất (resp. nhỏ nhất) do đó có nghĩa là E có một tập con đồng cuối (resp. đồng đầu) gồm một phần tử duy nhất.

### 8. CẬN TRÊN VÀ CẬN DƯỚI

#### Định nghĩa 5 {#ens-iii-s1-def-5 .statement tag=03JI}

*Cho E là một tập hợp tiền thứ tự và cho X là một tập con của E. Bất kỳ phần tử $x\in E$ nào sao cho $x\leq y$ (tương ứng $x\geq y$) với mọi $y\in X$ được gọi là một cận dưới (tương ứng cận trên) của X trong E.*

Mỗi cận trên của X là một cận dưới của X theo thứ tự đối, và ngược lại.

¶ Nếu $x$ là một cận dưới của X, thì mọi phần tử $z\leq x$ cũng là một cận dưới của X. Một cận dưới của X cũng là một cận dưới của mọi tập con của X. Một tập hợp có thứ tự X có phần tử nhỏ nhất khi và chỉ khi tồn tại một cận dưới của X thuộc X.

¶ Tập hợp các cận dưới của một tập con X của một tập hợp tiền thứ tự E có thể rỗng : đó là trường hợp khi $X=E$ và E là một tập hợp có thứ tự không có phần tử nhỏ nhất.

¶ Một tập con X của E mà tập hợp các cận dưới (tương ứng các cận trên) của nó không rỗng được gọi là *bị chặn dưới* (tương ứng *bị chặn trên*). Một tập con bị chặn cả dưới lẫn trên được gọi là *bị chặn*. Nếu X bị chặn dưới (tương ứng bị chặn trên, bị chặn), thì mọi tập con của X cũng vậy.

Mọi tập con gồm một phần tử đều bị chặn. Nhưng một tập con gồm hai phần tử không nhất thiết bị chặn trên cũng như bị chặn dưới (no. 10).

Cho E là một tập hợp tiền thứ tự và cho $f$ là một ánh xạ của một tập hợp tùy ý A vào E. Ánh xạ $f$ được gọi (theo cách nói rộng) là *bị chặn dưới* (tương ứng *bị chặn trên, bị chặn*) nếu tập hợp $f(A)$ bị chặn dưới (tương ứng bị chặn trên, bị chặn) trong E.

### 9. CẬN TRÊN NHỎ NHẤT VÀ CẬN DƯỚI LỚN NHẤT

#### Định nghĩa 6 {#ens-iii-s1-def-6 .statement tag=03JJ}

*Cho E là một tập hợp có thứ tự và X là một tập con của E. Một phần tử của E được gọi là cận dưới lớn nhất hay infimum (tương ứng, cận trên nhỏ nhất hay supremum) của X trong E nếu nó là phần tử lớn nhất (tương ứng, nhỏ nhất) của tập hợp các cận dưới (tương ứng, cận trên) của X trong E.*

Cho một tập con X của một tập hợp có thứ tự E, cận trên nhỏ nhất (tương ứng cận dưới lớn nhất) của X trong E, khi nó tồn tại, được ký hiệu bởi

$$
\operatorname{sup}_{E}X\quad(\text{resp. }\operatorname{inf}_{E}X)
$$

hoặc bởi sup X (tương ứng inf X) nếu không sợ nhầm lẫn. Cận trên nhỏ nhất (tương ứng cận dưới lớn nhất) của một tập $\{x, y\}$ gồm hai phần tử, khi nó tồn tại, được ký hiệu bởi sup $(x, y)$ (tương ứng inf $(x, y)$). Tương tự đối với cận trên nhỏ nhất và cận dưới lớn nhất của một tập hợp gồm ba phần tử, v.v.

¶ Nếu một tập con X của E có một phần tử lớn nhất $a$, thì $a$ là cận trên bé nhất của X trong E.

¶ Nếu X có một cận dưới lớn nhất $a$ trong E, thì $a$ là cận trên bé nhất của X đối với thứ tự đối trên E. Vì lý do này, trong phần lớn những gì sau đây, ta có thể tự giới hạn vào việc xét các tính chất của cận trên bé nhất.

*Ví dụ*

(1) Tập hợp các cận trên của tập rỗng $\emptyset$ trong một tập hợp có thứ tự E hiển nhiên là chính E; do đó $\emptyset$ có một supremum trong E khi và chỉ khi E có một phần tử *bé nhất*, và khi đó phần tử này là *cận trên bé nhất* của $\emptyset$.

(2) Trong tập hợp $\mathfrak{P}(E)$ các tập con của một tập hợp E, được sắp thứ tự bởi quan hệ bao hàm, mọi tập con $\mathfrak{S}$ của $\mathfrak{P}(E)$ đều có một cận trên bé nhất, đó là *hợp* của các tập hợp thuộc $\mathfrak{S}$, và một cận dưới lớn nhất, đó là *giao* của các tập hợp thuộc $\mathfrak{S}$.

(3) Cho E, F là hai tập hợp và $\Theta$ là một tập con của $\Phi(E, F)$, tập hợp các ánh xạ từ các tập con của E vào F, được sắp thứ tự theo sự mở rộng của các ánh xạ (no. 1, Ví dụ 3). Với mỗi $u \in \Phi(E, F)$, gọi $D(u)$ là miền xác định của $u$. Điều kiện để tồn tại một mở rộng chung của một họ các ánh xạ thuộc $\Phi(E, F)$ (Chương II, § 4, no. 6, Mệnh đề 7) cho thấy rằng $\Theta$ có một cận trên nhỏ nhất trong $\Phi(E, F)$ khi và chỉ khi với mỗi cặp $(u, v)$ các phần tử của $\Theta$ ta có $u(x) = v(x)$ mỗi khi $x \in D(u) \cap D(v)$.

Một ánh xạ $f$ từ một tập hợp A vào một tập hợp có thứ tự E được nói là có một cận trên nhỏ nhất nếu ảnh $f(A)$ có một cận trên nhỏ nhất trong E; khi đó cận này được gọi là *cận trên nhỏ nhất của f* và được viết là $\sup_{x \in A} f(x)$. Tương tự đối với cận dưới lớn nhất.

Đặc biệt, nếu một tập con A của E có một cận trên nhỏ nhất trong E, thì cận này là cận trên nhỏ nhất của đơn ánh chính tắc của A vào E, và vì thế có thể được viết là $\sup_{x \in A} x$.

#### Mệnh đề 4 {#ens-iii-s1-prop-4 .statement tag=03JK}

*Cho* E *là một tập hợp có thứ tự và* A *là một tập con của* E *có cả một cận dưới lớn nhất và một cận trên nhỏ nhất trong* E. *Khi đó* $\inf A \leqslant \sup A$ *nếu* $A \neq \emptyset$; *nếu* $A = \emptyset$, $\sup A$ *là phần tử nhỏ nhất và* $\inf A$ *là phần tử lớn nhất của* E.

Điều này suy ra ngay lập tức từ các định nghĩa.

#### Mệnh đề 5 {#ens-iii-s1-prop-5 .statement tag=03JL}

*Cho* E *là một tập hợp có thứ tự và* A, B *là hai tập con của* E, *mỗi tập đều có một cận trên nhỏ nhất* (resp. *cận dưới lớn nhất*) *trong* E. *Nếu* $A \subset B$, *thì* $\sup A \leqslant \sup B$ (resp. $\inf A \geqslant \inf B$).

#### Hệ quả {#ens-iii-s1-n9-cor-1 .statement tag=03JM}

*Cho $(x_\iota)_{\iota \in I}$ là một họ các phần tử của một tập hợp có thứ tự* $\mathrm{E}$ *mà có một cận trên đúng trong* $\mathrm{E}$. *Nếu* $\mathrm{J}$ *là một tập con của* $\mathrm{I}$ *sao cho họ* $(x_\iota)_{\iota \in J}$ *có một cận trên đúng trong* $\mathrm{E}$, *ta có* $\sup\limits_{\iota \in J} x_\iota \leqslant \sup\limits_{\iota \in I} x_\iota$.

#### Mệnh đề 6 {#ens-iii-s1-prop-6 .statement tag=03JN}

*Cho* $(x_\iota)_{\iota \in I}$, $(y_\iota)_{\iota \in I}$ *là hai họ các phần tử của một tập hợp có thứ tự* $\mathrm{E}$, *được đánh chỉ số bởi cùng một tập hợp* $\mathrm{I}$, *và sao cho* $x_\iota \leqslant y_\iota$ *với mọi* $\iota \in \mathrm{I}$. *Nếu cả hai họ đều có một cận trên bé nhất trong* $\mathrm{E}$, *thì* $\sup\limits_{\iota \in I} x_\iota \leqslant \sup\limits_{\iota \in I} y_\iota$.

Vì $a = \sup\limits_{\iota \in I} y_\iota$ là một cận trên của tập hợp các $y_\iota$, nên $x_\iota \leqslant y_\iota \leqslant a$ với mọi $\iota \in \mathrm{I}$, và do đó $\sup\limits_{\iota \in I} x_\iota \leqslant a$.

#### Mệnh đề 7 {#ens-iii-s1-prop-7 .statement tag=03JO}

*Cho* $(x_\iota)_{\iota \in I}$ *là một họ các phần tử của một tập hợp có thứ tự* $\mathrm{E}$, *và cho* $(\mathrm{J}_\lambda)_{\lambda \in L}$ *là một phủ của tập hợp chỉ số* $\mathrm{I}$. *Giả sử rằng mỗi họ con* $(x_\iota)_{\iota \in J_\lambda}$ *đều có cận trên đúng trong* $\mathrm{E}$. *Để họ* $(x_\iota)_{\iota \in I}$ *có cận trên đúng trong* $\mathrm{E}$, *cần và đủ là họ* $\left( \sup\limits_{\iota \in J_\lambda} x_\iota \right)_{\lambda \in L}$ *cũng có cận trên đúng trong* $\mathrm{E}$, *và khi đó ta có*

$$(1) \qquad \sup_{\iota \in I} x_\iota = \sup_{\lambda \in L} \left( \sup_{\iota \in J_\lambda} x_\iota \right).$$

Cho $b_\lambda = \sup\limits_{\iota \in J_\lambda} x_\iota$. Giả sử rằng $(x_\iota)_{\iota \in I}$ có một cận trên bé nhất $a$. Khi đó $a \geqslant b_\lambda$ với mỗi $\lambda \in \mathrm{L}$ (Hệ quả của Mệnh đề 5). Mặt khác, nếu $c \geqslant b_\lambda$ với mỗi $\lambda \in \mathrm{L}$, thì ta có $c \geqslant x_\iota$ với mỗi $\iota \in \mathrm{I}$, vì $(\mathrm{J}_\lambda)_{\lambda \in L}$ là một phủ của $\mathrm{I}$; do đó $c \geqslant a$, điều này chứng tỏ rằng

$$a = \sup_{\lambda \in L} b_\lambda.$$

Ngược lại, giả sử rằng họ $(b_\lambda)_{\lambda \in L}$ có một cận trên bé nhất $a'$. Khi đó $a' \geqslant x_\iota$ với mọi $\iota \in \mathrm{I}$. Mặt khác, nếu $c' \geqslant x_\iota$ với mọi $\iota \in \mathrm{I}$, thì đặc biệt ta có

$$c' \geqslant \sup_{\iota \in J_\lambda} x_\iota = b_\lambda$$

với mỗi $\lambda \in \mathrm{L}$, do đó $c' \geqslant a'$ và vì thế

$$a' = \sup_{\iota \in I} x_\iota.$$

#### Hệ quả {#ens-iii-s1-n9-cor-2 .statement tag=03JP}

*Cho* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *là một "họ kép" các phần tử của một tập hợp có thứ tự* $\mathrm{E}$ *sao cho với mỗi* $\mu \in \mathrm{M}$ *thì họ* $(x_{\lambda\mu})_{\lambda \in L}$ *có một cận trên đúng trong* $\mathrm{E}$. *Để họ* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *có một cận trên đúng trong* $\mathrm{E}$, *điều cần và đủ là họ* $\left( \sup\limits_{\lambda \in L} x_{\lambda\mu} \right)_{\mu \in M}$ *phải có một cận trên đúng trong*

*E, và khi đó ta có*

$$(2) \qquad \sup_{(\lambda,\,\mu)\in L\times M} x_{\lambda\mu} = \sup_{\mu\in M}\left(\sup_{\lambda\in L} x_{\lambda\mu}\right).$$

#### Mệnh đề 8 {#ens-iii-s1-prop-8 .statement tag=03QI}

*Cho* $(E_\iota)_{\iota\in I}$ *là một họ các tập hợp có thứ tự. Cho* A *là một tập con của tập hợp có thứ tự tích* $E = \prod_{\iota\in I} E_\iota$, *và đặt* $A_\iota = \mathrm{pr}_\iota A$ *với mỗi* $\iota \in I$. *Để* A *có một cận trên bé nhất trong* E *thì điều kiện cần và đủ là, với mỗi* $\iota \in I$, $A_\iota$ *có một cận trên bé nhất trong* $E_\iota$, *và khi đó ta có*

$$\sup A = (\sup A_\iota)_{\iota\in I} = \left(\sup_{x\in A} \mathrm{pr}_\iota x\right)_{\iota\in I}.$$

Giả sử rằng, với mỗi $\iota \in I$, $A_\iota$ có một cận trên bé nhất $b_\iota$ trong $E_\iota$. Khi đó, nói rằng $c = (c_\iota)$ là một cận trên của A có nghĩa là $c_\iota \geqslant b_\iota$ với mỗi $\iota \in I$, do đó $(b_\iota)_{\iota\in I}$ là một cận trên của A. Ngược lại, giả sử A có một cận trên bé nhất $a = (a_\iota)_{\iota\in I}$; với mỗi $\varkappa \in I$, $a_\varkappa$ là một cận trên của $A_\varkappa$, bởi vì nếu $x_\varkappa \in A_\varkappa$, thì tồn tại $x \in A$ sao cho $\mathrm{pr}_\varkappa x = x_\varkappa$, theo định nghĩa của $A_\varkappa$; mặt khác, nếu $a'_\varkappa$ là một cận trên của $A_\varkappa$ trong $E_\varkappa$, thì phần tử $c' = (c'_\iota)_{\iota\in I}$ mà

$$c'_\iota = a_\iota \quad \text{với} \quad \iota \neq \varkappa \qquad \text{và} \qquad c'_\varkappa = a'_\varkappa$$

là một cận trên của A; do đó $c' \geqslant a$ và vì thế $a'_\varkappa \geqslant a_\varkappa$; suy ra $a_\varkappa$ là cận trên bé nhất của $A_\varkappa$ trong $E_\varkappa$.

☡

¶ Cho F là một tập con của một tập hợp có thứ tự E, và cho A là một tập con của F. Có thể xảy ra việc một trong hai phần tử $\sup_E A$, $\sup_F A$ tồn tại nhưng phần tử kia thì không, hoặc cả hai cùng tồn tại nhưng không bằng nhau.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n9-exa-1 .statement tag=03SS}

Trong tập hợp có thứ tự $E = \mathbf{R}$ của các số thực, xét tập con $F = \mathbf{Q}$ của các số hữu tỉ và tập hợp $A \subset F$ gồm các số hữu tỉ $< \sqrt{2}$; $\sup_E A$ tồn tại nhưng $\sup_F A$ không tồn tại.

#### Ví dụ 2 {#ens-iii-s1-n9-exa-2 .statement tag=03ST}

Trong ký hiệu của Ví dụ 1, đặt G là hợp của A và tập hợp $\{2\}$; khi đó $G \subset F$ và $\sup_G A$ tồn tại, nhưng $\sup_F A$ không tồn tại.

#### Ví dụ 3 {#ens-iii-s1-n9-exa-3 .statement tag=03SU}

Với cùng ký hiệu, $\sup_E A = \sqrt{2}$, $\sup_G A = 2$. \*

Tuy nhiên, ta có kết quả sau :

#### Mệnh đề 9 {#ens-iii-s1-prop-9 .statement tag=03QJ}

*Cho* E *là một tập hợp có thứ tự,* F *là một tập con của* E, A *là một tập con của* F. *Nếu cả* $\sup_E A$ *và* $\sup_F A$ *đều tồn tại, ta có* $\sup_E A \leqslant \sup_F A$. *Nếu* $\sup_E A$ *tồn tại và thuộc* F, *thì* $\sup_F A$ *tồn tại và bằng* $\sup_E A$.

Mệnh đề thứ nhất suy ra từ sự kiện rằng tập hợp $\mathrm{M}$ các chặn trên của A trong F được chứa trong tập hợp N các chặn trên của A trong E, và từ Mệnh đề 5. Mặt khác, nếu phần tử nhỏ nhất của N nằm trong F, thì nó thuộc M và rõ ràng là phần tử nhỏ nhất của M; điều đó chứng minh mệnh đề thứ hai.

### 10. TẬP HỢP CÓ HƯỚNG

#### Định nghĩa 7 {#ens-iii-s1-def-7 .statement tag=03QK}

*Một tập hợp tiền thứ tự* E *được gọi là có hướng phải* (tương ứng, *có hướng trái*) *nếu mọi tập con gồm hai phần tử của* E *đều bị chặn trên* (tương ứng, *bị chặn dưới*).

Thay cho "có hướng phải", ta sẽ thường dùng cách nói "có hướng đối với quan hệ $\leqslant$", và các cách nói tương tự khi quan hệ tiền thứ tự được ký hiệu bởi một dấu khác. Chẳng hạn, nếu $\mathfrak{S}$ là một tập hợp các tập con của một tập hợp A, ta nói rằng $\mathfrak{S}$ là *có hướng đối với quan hệ* $\subset$ (tương ứng $\supset$) nếu, với mỗi tập con $\{\mathrm{X}, \mathrm{Y}\}$ gồm hai phần tử của $\mathfrak{S}$, tồn tại $\mathrm{Z} \in \mathfrak{S}$ sao cho $\mathrm{X} \subset \mathrm{Z}$ và $\mathrm{Y} \subset \mathrm{Z}$ (tương ứng $\mathrm{X} \supset \mathrm{Z}$ và $\mathrm{Y} \supset \mathrm{Z}$).

*Ví dụ*
(1) Một tập hợp có thứ tự có một phần tử lớn nhất thì có hướng phải.
\* (2) Trong một không gian tôpô, một hệ cơ bản các lân cận của một điểm là có hướng đối với quan hệ $\supset$.
(3) Tập hợp các môđun con kiểu hữu hạn của một môđun tùy ý là có hướng đối với quan hệ $\subset$. \*

#### Mệnh đề 10 {#ens-iii-s1-prop-10 .statement tag=03QL}

*Trong một tập hợp có thứ tự có hướng phải* E, *một phần tử cực đại a là phần tử lớn nhất của* E.

Với mọi $x \in \mathrm{E}$, theo giả thiết tồn tại $y \in \mathrm{E}$ sao cho $x \leqslant y$ và $a \leqslant y$; vì $a$ là cực đại nên $y = a$.

¶ Một tập hợp tiền thứ tự có hướng phải thì có hướng trái đối với thứ tự đối. Mọi tích của các tập có hướng phải đều có hướng phải. Mặt khác, một tập con của một tập có hướng phải không tất yếu có hướng phải. Tuy nhiên, một tập con *đồng cuối* F của một tập có hướng phải E luôn luôn có hướng phải; với $x$, $y \in \mathrm{F}$ cho trước, tồn tại $z \in \mathrm{E}$ sao cho $x \leqslant z$ và $y \leqslant z$, rồi tồn tại $t \in \mathrm{F}$ sao cho $z \leqslant t$.

### 11. DÀN

#### Định nghĩa 8 {#ens-iii-s1-def-8 .statement tag=03QM}

*Một tập hợp có thứ tự* E *được gọi là một dàn nếu mọi tập con gồm hai phần tử của* E *đều có một cận trên nhỏ nhất và một cận dưới lớn nhất trong* E.

Mọi tích của các dàn đều là một dàn; điều này suy ra từ điều kiện tồn tại một cận trên nhỏ nhất trong một tích các tập hợp có thứ tự (số 9, Mệnh đề 8). Tập hợp các tập con của một tập hợp A, được sắp thứ tự theo quan hệ bao hàm, là một dàn

bởi vì hợp và giao của hai tập con của A lại là những tập con của A.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n11-exa-1 .statement tag=03SV}

Tập hợp các số nguyên $\geq 1$, được sắp thứ tự bởi quan hệ “$m$ chia hết $n$” giữa $m$ và $n$, là một mạng; cận trên bé nhất của $\{m,n\}$ là bội chung nhỏ nhất của $m$ và $n$, và cận dưới lớn nhất là ước chung lớn nhất của chúng.

#### Ví dụ 2 {#ens-iii-s1-n11-exa-2 .statement tag=03TT}

Tập hợp các nhóm con của một nhóm G, được sắp thứ tự bởi bao hàm, là một mạng.

#### Ví dụ 3 {#ens-iii-s1-n11-exa-3 .statement tag=03TU}

Tập hợp các tôpô trên một tập hợp A, được sắp thứ tự bởi quan hệ “$\mathcal{T}$ thô hơn $\mathcal{T}'$” giữa $\mathcal{T}$ và $\mathcal{T}'$, là một mạng. (Tôpô đại cương, Chương I, § 2).

#### Ví dụ 4 {#ens-iii-s1-n11-exa-4 .statement tag=03TV}

Tập hợp $\mathscr{F}(I,\mathbf{R})$ của mọi hàm nhận giá trị thực được định nghĩa trên một khoảng I của $\mathbf{R}$ là một dàn đối với quan hệ thứ tự $f\leq g$ (no. 4), và do đó đẳng cấu với tích $\mathbf{R}^{I}$. *

#### Nhận xét {#ens-iii-s1-n11-rem-1 .statement tag=03JQ}

Một dàn hiển nhiên vừa có hướng trái vừa có hướng phải. Nhưng một tập hợp có thứ tự vừa có hướng trái vừa có hướng phải thì không tất yếu là một dàn. * Một ví dụ của trường hợp thứ hai là tập hợp các ánh xạ $x\mapsto p(x)$ của $\mathbf{R}$ vào chính nó, trong đó $p$ là một đa thức trong $\mathbf{R}[X]$, tập hợp này được sắp thứ tự bởi quan hệ $p\leq q$ (no. 4). *

### 12. TẬP HỢP ĐƯỢC SẮP THỨ TỰ TOÀN PHẦN

#### Định nghĩa 9 {#ens-iii-s1-def-9 .statement tag=03JR}

*Hai phần tử $x$, $y$ của một tập hợp tiền thứ tự E được gọi là so sánh được nếu quan hệ “$x\leq y$ hoặc $y\leq x$” là đúng. Một tập hợp E được gọi là được sắp thứ tự toàn phần nếu nó có thứ tự và nếu hai phần tử bất kỳ của E là so sánh được. Khi đó, thứ tự trên E được gọi là một thứ tự toàn phần, và quan hệ thứ tự tương ứng là một quan hệ thứ tự toàn phần.*

Nếu $x$ và $y$ là các phần tử của một tập sắp thứ tự toàn phần, thì $x=y$ hoặc $x<y$ hoặc $x>y$; do đó phủ định của $x\leq y$ là $x>y$.

Một thứ tự trên E là một thứ tự toàn phần khi và chỉ khi đồ thị G của nó thỏa mãn quan hệ $G\cup G^{-1}=E\times E$, cũng như các quan hệ $G\circ G=G$ và $G\cap G^{-1}=\Delta$.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s1-n12-exa-1 .statement tag=03SW}

Mọi tập con của một tập sắp thứ tự toàn phần đều được sắp thứ tự toàn phần theo thứ tự cảm sinh.

#### Ví dụ 2 {#ens-iii-s1-n12-exa-2 .statement tag=03TW}

Cho E là một tập hợp có thứ tự tùy ý. Tập con rỗng của E được sắp thứ tự toàn phần, và mọi tập con của E gồm một phần tử cũng vậy.

#### Ví dụ 3 {#ens-iii-s1-n12-exa-3 .statement tag=03TX}

Tập $\mathbf{R}$ các số thực được sắp thứ tự toàn phần. *

#### Ví dụ 4 {#ens-iii-s1-n12-exa-4 .statement tag=03TY}

Nếu A là một tập hợp có ít nhất hai phần tử phân biệt, thì tập $\mathscr{P}(A)$ (được sắp thứ tự theo quan hệ bao hàm) không được sắp thứ tự toàn phần, vì nếu $x\neq y$, thì các tập con $\{x\}$ và $\{y\}$ không so sánh được.

Một tập sắp thứ tự toàn phần cũng được sắp thứ tự toàn phần đối với thứ tự đối; nó là một mạng và *a fortiori* vừa có hướng trái vừa có hướng phải.

#### Mệnh đề 11 {#ens-iii-s1-prop-11 .statement tag=03JS}

*Mọi ánh xạ đơn điệu ngặt $f$ của một tập sắp thứ tự toàn phần* E *vào một tập hợp có thứ tự* F *đều là đơn ánh. Nếu $f$ tăng ngặt, thì $f$ là một đẳng cấu của* E *lên $f(\mathrm{E})$.*

Vì $x \neq y$ kéo theo hoặc $x < y$ hoặc $x > y$; do đó

$$f(x) < f(y) \qquad \text{hoặc} \qquad f(x) > f(y),$$

nên trong cả hai trường hợp đều có $f(x) \neq f(y)$. Còn phải chứng minh rằng nếu $f$ tăng ngặt, thì $f(x) \leqslant f(y)$ kéo theo $x \leqslant y$; nếu không, ta sẽ có $x > y$, và do đó $f(x) > f(y)$.

#### Mệnh đề 12 {#ens-iii-s1-prop-12 .statement tag=03JT}

*Cho* E *là một tập sắp thứ tự toàn phần và* X *là một tập con của* E. *Để một phần tử $b$ của* E *là cận trên bé nhất của* X *trong* E, *điều kiện cần và đủ là* (1) *$b$ là một cận trên của* X, (2) *với mọi $c \in \mathrm{E}$ sao cho $c < b$, tồn tại $x \in \mathrm{X}$ sao cho $c < x \leqslant b$.*

Điều kiện thứ hai nói rằng không có phần tử $c < b$ nào là một cận trên của X, tức là $b$ là một phần tử cực tiểu của tập M các cận trên của X; nhưng điều này cũng chính là nói rằng $b$ là phần tử bé nhất của M, vì M được sắp thứ tự toàn phần (no. 10, Mệnh đề 10).

### 13. CÁC KHOẢNG

Cho E là một tập hợp có thứ tự và $a$, $b$ là hai phần tử của E sao cho $a \leqslant b$. Tập con của E gồm các phần tử $x$ sao cho $a \leqslant x \leqslant b$ được gọi là *khoảng đóng có đầu mút trái a và đầu mút phải b*, và được ký hiệu bởi $[a, b]$. Tập hợp tất cả các $x \in \mathrm{E}$ sao cho $a \leqslant x < b$ (tương ứng $a < x \leqslant b$) được gọi là *khoảng nửa mở bên phải* (tương ứng *bên trái*) có các đầu mút $a$ và $b$, và được ký hiệu bởi $[a, b[$ (tương ứng $]a, b])$. Tập hợp tất cả các $x \in \mathrm{E}$ sao cho $a < x < b$ được gọi là *khoảng mở* có các đầu mút $a$ và $b$, và được ký hiệu bởi $]a, b[$.

Chú ý rằng một khoảng đóng không bao giờ rỗng; khoảng $[a, a]$ là tập hợp $\{a\}$. Mặt khác, các khoảng $[a, a[$, $]a, a]$, $]a, a[$ đều rỗng; và một khoảng mở $]a, b[$ có thể rỗng ngay cả khi $a < b$.

Cho $a$ là một phần tử của E. Tập hợp tất cả các $x \in \mathrm{E}$ sao cho $x \leqslant a$ (tương ứng $x < a$) được gọi là *khoảng* *đóng* (tương ứng *mở*) *không bị chặn về bên trái, có mút phải a*, và được ký hiệu bởi $]{\leftarrow}, a]$ (tương ứng $]{\leftarrow}, a[$); tương tự, tập hợp tất cả các $x \in \mathrm{E}$ sao cho $x \geqslant a$ (tương ứng $x > a$) được gọi là *khoảng* *đóng* (tương ứng *mở*) *có mút trái a, không bị chặn về bên phải*, và được ký hiệu bởi $[a, {\rightarrow}[$ (tương ứng $]a, {\rightarrow}[$). Cuối cùng, chính E có thể được

coi là *khoảng mở không bị chặn về bên trái và bên phải*, được ký hiệu bởi $]\leftarrow, \rightarrow[$.

#### Mệnh đề 13 {#ens-iii-s1-prop-13 .statement tag=03JU}

*Trong một dàn, giao của hai khoảng là một khoảng.* Chẳng hạn, xét giao của hai khoảng đóng $[a, b]$ và $[c, d]$, và đặt $\alpha = \sup (a, c)$, $\beta = \inf (b, d)$. Nếu đồng thời $a \leqslant x \leqslant b$ và $c \leqslant x \leqslant d$, thì ta có $\alpha \leqslant x \leqslant \beta$, và ngược lại; nếu $\alpha \not\leqslant \beta$, thì giao của $[a, b]$ và $[c, d]$ là rỗng; nếu $\alpha \leqslant \beta$, thì giao này là $[\alpha, \beta]$. Chúng tôi để bạn đọc tự hoàn thành chứng minh cho các trường hợp khác.

### Bài tập {#ens-iii-s1-exercises}

Xem [bài tập của § 1](exercises/s1/).
