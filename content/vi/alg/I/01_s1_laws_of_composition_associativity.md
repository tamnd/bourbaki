---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 1
section_title: Laws of composition; associativity; commutativity
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0025-0036, 0148-0150
extraction: ocr
subsections:
    - "no": 1
      title: LAWS OF COMPOSITION
      page: 0
      pdf_page: 25
    - "no": 2
      title: COMPOSITION OF AN ORDERED SEQUENCE OF ELEMENTS
      page: 0
      pdf_page: 27
    - "no": 3
      title: ASSOCIATIVE LAWS
      page: 0
      pdf_page: 28
    - "no": 4
      title: STABLE SUBSETS. INDUCED LAWS
      page: 0
      pdf_page: 30
    - "no": 5
      title: PERMUTABLE ELEMENTS. COMMUTATIVE LAWS
      page: 0
      pdf_page: 31
    - "no": 6
      title: QUOTIENT LAWS
      page: 0
      pdf_page: 35
statements: 31
exercises: 16
content_sha256: 843fbf05a07f129303afefbc44f480b298e18baedca0d2ce35e05b34adcc246a
translated_from: content/en/alg/I/01_s1_laws_of_composition_associativity.md
source_content_sha256: ee4e463c2bea3d268def69cc870b68653ee33956e50d1763ff66c0f237db3f9e
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-88bac9d5
glossary_version: 34
glossary_terms_sha256: bee1b4833f03dfb16fa1b70f9bba4c94cb053c567dfb9fa07d7a766afd60ed82
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CÁC LUẬT HỢP THÀNH; TÍNH KẾT HỢP; TÍNH GIAO HOÁN

### 1. CÁC LUẬT HỢP THÀNH

#### Định nghĩa 1 {#alg-i-s1-def-1 .statement}

Cho E là một tập hợp. Một ánh xạ f của E × E vào E được gọi là một luật hợp thành trên E. Giá trị f(x, y) của f đối với một cặp có thứ tự (x, y) ∈ E × E được gọi là hợp thành của x và y theo luật này. Một tập hợp với một luật hợp thành được gọi là một magma.

Hợp thành của x và y thường được ký hiệu bằng cách viết x và y theo một thứ tự xác định và phân cách chúng bởi một ký hiệu đặc trưng của luật đang xét (một ký hiệu mà có thể quy ước bỏ đi). Trong các ký hiệu thường dùng nhất có + và ., quy ước thông thường là bỏ ký hiệu sau nếu muốn; với các ký hiệu này, hợp thành của x và y lần lượt được viết là x + y và x.y hoặc xy. Một luật được ký hiệu bởi + thường được gọi là phép cộng (hợp thành x + y được gọi là tổng của x và y) và ta nói rằng nó được viết theo cộng tính; một luật được ký hiệu bởi . thường được gọi là phép nhân (hợp thành x.y = xy được gọi là tích của x và y) và ta nói rằng nó được viết theo nhân tính. Trong các lập luận tổng quát của các đoạn 1 đến 3 của chương này, nói chung ta sẽ dùng các ký hiệu ⊔ và ⊓ để biểu thị các luật hợp thành tùy ý.

Do lạm dụng ngôn ngữ, một ánh xạ của một tập con của E × E vào E đôi khi được gọi là một luật hợp thành không xác định khắp nơi trên E.

#### Ví dụ {#alg-i-s1-n1-exa-1 .statement}

(1) Các ánh xạ (X, Y) ↦ X ∪ Y và (X, Y) ↦ X ∩ Y là các luật hợp thành trên tập hợp các tập con của một tập hợp E.

(2) Trên tập hợp N các số tự nhiên, phép cộng, phép nhân và phép lũy thừa là các luật hợp thành (các hợp thành của x ∈ N và y ∈ N theo các luật này lần lượt được ký hiệu bởi x + y, xy hoặc x.y và x^y) (Lý thuyết tập hợp, III, § 3, no. 4).

(3) Cho E là một tập hợp; ánh xạ (X, Y) ↦ X ⋅ Y là một luật hợp thành trên tập hợp các tập con của E × E (Lý thuyết tập hợp, II, § 3, no. 3, Định nghĩa 6); ánh xạ (f, g) ↦ f ⋅ g là một luật hợp thành trên tập hợp các ánh xạ của E vào E (Lý thuyết tập hợp, II, § 5, no. 2).

(4) Cho E là một dàn (Lý thuyết tập hợp, III, § 1, no. 11); nếu sup(x, y) biểu thị cận trên nhỏ nhất của tập hợp {x, y}, ánh xạ (x, y) ↦ sup(x, y) là một luật hợp thành trên E. Tương tự đối với cận dưới lớn nhất inf(x, y). Ví dụ 1 ở trên là một trường hợp riêng của điều này với $\mathfrak{P}(E)$ được sắp thứ tự bởi bao hàm.

(5) Cho $(E_t)_{t \in I}$ là một họ các magma. Gọi $\tau_t$ là luật hợp thành trên $E_t$. Ánh xạ
$$
((x_i), (y_i)) \mapsto ((x_i \tau_t y_i))
$$
là một luật hợp thành trên tích $E = \prod_{t \in I} E_t$, được gọi là *tích* của các luật $\tau_t$. Tập hợp E với luật này được gọi là *magma tích* của các magma $E_t$. Đặc biệt, nếu mọi magma $E_t$ đều bằng cùng một magma M, ta thu được *magma các ánh xạ của I từ M*.

Cho $(x, y) \mapsto x \tau y$ là một luật hợp thành trên một tập hợp E. Với hai tập con bất kỳ X, Y của E, $X \tau Y$ (với điều kiện ký hiệu này không gây nhầm lẫn†) sẽ chỉ tập hợp các phần tử $x \tau y$ trong E, trong đó $x \in X, y \in Y$ (nói cách khác, là ảnh của $X \times Y$ qua ánh xạ $(x, y) \mapsto x \tau y$).

Nếu $a \in E$ ta thường viết $a \tau Y$ thay cho $\{a\} \tau Y$ và $X \tau a$ thay cho $X \tau \{a\}$. Ánh xạ $(X, Y) \mapsto X \tau Y$ là một luật hợp thành trên tập hợp các tập con của E.

#### Định nghĩa 2 {#alg-i-s1-def-2 .statement}

*Cho E là một magma và $\tau$ biểu thị luật hợp thành của nó. Luật hợp thành $(x, y) \mapsto y \tau x$ trên E được gọi là luật đối của luật trên. Tập hợp E với luật này được gọi là magma đối của E.*

Cho E và E' là hai magma; ta sẽ ký hiệu các luật của chúng bằng cùng một ký hiệu $\tau$. Phù hợp với các định nghĩa tổng quát (*Lý thuyết tập hợp*, IV, § 1, no. 5), một ánh xạ song ánh f của E lên E' sao cho
$$
f(x \tau y) = f(x) \tau f(y)
$$
đối với mọi cặp có thứ tự $(x, y) \in E \times E$ được gọi là một *đẳng cấu của E lên E'*. Ta nói E và E' là *đẳng cấu* nếu tồn tại một đẳng cấu của E lên E'.

Tổng quát hơn:

#### Định nghĩa 3 {#alg-i-s1-def-3 .statement}

*Một ánh xạ f của E vào E' sao cho hệ thức (1) đúng với mọi cặp có thứ tự $(x, y) \in E \times E$ được gọi là một đồng cấu, hoặc cấu xạ, của E vào E'; nếu $E = E'$, f được gọi là một tự đồng cấu của E.*

Ánh xạ đồng nhất của một magma E là một đồng cấu, hợp thành của hai đồng cấu là một đồng cấu.

† Sau đây là một ví dụ trong đó nguyên lý này sẽ dẫn đến nhầm lẫn và do đó không nên được sử dụng. Giả sử rằng luật hợp thành đang xét là luật $(A, B) \mapsto A \cup B$ giữa các tập con của một tập hợp E; một luật hợp thành
$$
(\mathcal{A}, \mathcal{B}) \mapsto F(\mathcal{A}, \mathcal{B})
$$
được dẫn xuất giữa các tập con của $\mathfrak{P}(E)$, trong đó $F(\mathcal{A}, \mathcal{B})$ là tập hợp các $A \cup B$ với $A \in \mathcal{A}, B \in \mathcal{B}$; nhưng $F(\mathcal{A}, \mathcal{B})$ không nên được ký hiệu bởi $\mathcal{A} \cup \mathcal{B}$, vì ký hiệu này đã có một nghĩa khác (hợp của $\mathcal{A}$ và $\mathcal{B}$ được xem như các tập con của $\mathfrak{P}(E)$).

Để một ánh xạ $f$ của E vào E' là một đẳng cấu, điều kiện cần và đủ là nó là một đồng cấu song ánh và khi đó $f^{-1}$ là một đẳng cấu của E' lên E.

### 2. HỢP THÀNH CỦA MỘT DÃY CÓ THỨ TỰ CÁC PHẦN TỬ

Nhắc lại rằng một họ các phần tử của một tập hợp E là một ánh xạ $i \mapsto x_i$ của một tập hợp I (được gọi là tập chỉ số) vào E; một họ $(x_i)_{i \in I}$ được gọi là hữu hạn nếu tập chỉ số là hữu hạn.

Một họ hữu hạn $(x_i)_{i \in I}$ các phần tử của E có tập chỉ số I được sắp thứ tự toàn phần được gọi là một dãy có thứ tự các phần tử của E.

Cụ thể, mọi dãy hữu hạn $(x_i)_{i \in H}$, trong đó H là một tập con hữu hạn của tập $\mathbf{N}$ các số tự nhiên, có thể được xem là một dãy có thứ tự nếu H được cho quan hệ thứ tự cảm sinh bởi quan hệ $m \leq n$ giữa các số tự nhiên.

Hai dãy có thứ tự $(x_i)_{i \in I}$ và $(y_k)_{k \in K}$ được gọi là tương tự nếu tồn tại một đẳng cấu tập có thứ tự $\phi$ của I lên K sao cho $y_{\phi(i)} = x_i$ với mọi $i \in I$.

Mọi dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ đều tương tự với một dãy hữu hạn thích hợp. Thật vậy, tồn tại một song ánh tăng từ A lên một khoảng $[0, n]$ của $\mathbf{N}$.

#### Định nghĩa 4 {#alg-i-s1-def-4 .statement}

*Cho* $(x_\alpha)_{\alpha \in A}$ *là một dãy có thứ tự các phần tử của một magma E mà tập chỉ số A không rỗng. Hợp thành (theo luật T) của dãy có thứ tự* $(x_\alpha)_{\alpha \in A}$, *được ký hiệu bởi* $\prod_{\alpha \in A} x_\alpha$, *là phần tử của E được xác định bằng quy nạp theo số phần tử của A như sau:*

(1) *nếu* $A = \{\beta\}$ *thì* $\prod_{\alpha \in A} x_\alpha = x_\beta$;

(2) *nếu* A *có* $p > 1$ *phần tử, $\beta$ là phần tử nhỏ nhất của* A *và* $A' = A - \{\beta\}$, *thì* $\prod_{\alpha \in A} x_\alpha = x_\beta \ T \left( \prod_{\alpha \in A'} x_\alpha \right)$.

Suy ra ngay lập tức (bằng quy nạp theo số phần tử của các tập chỉ số) rằng các hợp thành của hai dãy có thứ tự tương tự là bằng nhau; đặc biệt, hợp thành của mọi dãy có thứ tự bằng hợp thành của một dãy hữu hạn. Nếu $A = \{\lambda, \mu, \nu\}$ có ba phần tử ($\lambda < \mu < \nu$) thì hợp thành $\prod_{\alpha \in A} x_\alpha$ là $x_\lambda \ T \ (x_\mu \ T \ x_\nu)$.

#### Nhận xét {#alg-i-s1-n2-rem-1 .statement}

Chú ý rằng có một mức độ tùy ý nào đó trong định nghĩa hợp thành của một dãy có thứ tự; phép quy nạp mà ta đưa vào tiến hành "từ phải sang trái". Nếu ta tiến hành "từ trái sang phải", hợp thành của dãy có thứ tự trên $(x_\lambda, x_\mu, x_\nu)$ sẽ là $(x_\lambda \ T \ x_\mu) \ T \ x_\nu$.

Về mặt ký hiệu, hợp thành của một dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ được viết $\prod_{\alpha \in A}$ đối với một luật được ký hiệu bởi $\perp$; đối với một luật viết cộng tính, nó thường được ký hiệu bởi $\sum_{\alpha \in A} x_\alpha$ và được gọi là tổng của dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ (các $x_\alpha$ được gọi là các số hạng của tổng); đối với một luật viết nhân tính, nó thường được ký hiệu bởi $\prod_{\alpha \in A} x_\alpha$ và được gọi là *tích* của dãy có thứ tự $(x_\alpha)$ (các $x_\alpha$ được gọi là các *thừa số* của tích).†

Khi không có khả năng nhầm lẫn về tập chỉ số (cũng như về thứ tự của nó), người ta thường bỏ nó trong ký hiệu của hợp thành một dãy có thứ tự và khi đó viết, chẳng hạn đối với một luật viết cộng tính,
$\sum_\alpha x_\alpha$ thay cho $\sum_{\alpha \in A} x_\alpha$; tương tự đối với các ký hiệu khác.

Đối với một luật được ký hiệu bởi $\top$, hợp thành của một *dãy* $(x_i)$ có tập chỉ số là một khoảng không rỗng $[p, q]$ của $\mathbf{N}$ được ký hiệu bởi $\prod_{p \leq i \leq q} x_i$ hoặc $\prod_{i=p}^q x_i$; tương tự đối với các luật được ký hiệu bởi các ký hiệu khác.

Cho E và F là hai magma mà các luật hợp thành của chúng được ký hiệu bởi $\top$ và $f$ là một đồng cấu từ E vào F. Với mọi dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ các phần tử của E
$$
f\left( \prod_{\alpha \in A} \right) = \prod_{\alpha \in A} f(x_\alpha).
$$

### 3. CÁC LUẬT KẾT HỢP

#### Định nghĩa 5 {#alg-i-s1-def-5 .statement}

*Một luật hợp thành* $(x, y) \mapsto x \top y$ *trên một tập* E *được gọi là kết hợp nếu, với mọi phần tử* $x, y, z$ *trong* E,
$$
(x \top y) \top z = x \top (y \top z).
$$
*Một magma có luật kết hợp được gọi là một magma kết hợp*.

Luật đối của một luật kết hợp là kết hợp.

#### Ví dụ {#alg-i-s1-n3-exa-1 .statement}

(1) Phép cộng và phép nhân các số tự nhiên là các luật hợp thành kết hợp trên $\mathbf{N}$ (*Lý thuyết tập hợp*, III, § 3, no. 3, Hệ quả của Mệnh đề 5)
(2) Các luật được nêu trong các Ví dụ (1), (3) và (4) của no. 1 là kết hợp.

#### Định lý 1 (Định lý kết hợp) {#alg-i-s1-thm-1 .statement}

*Cho* E *là một magma kết hợp có luật được ký hiệu bởi* $\top$. *Cho* A *là một tập hữu hạn không rỗng được sắp thứ tự toàn phần, là hợp của một dãy có thứ tự các tập con không rỗng* $(B_i)_{i \in I}$ *sao cho các quan hệ* $\alpha \in B_i, \beta \in B_j, i < j$ *suy ra* $\alpha < \beta$; *cho* $(x_\alpha)_{\alpha \in A}$ *là một dãy có thứ tự các phần tử trong* E *với* A *là tập chỉ số. Khi đó*
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right)
$$

† Việc sử dụng thuật ngữ này và ký hiệu $\prod_{\alpha \in A} x_\alpha$ phải tránh nếu có bất kỳ nguy cơ nhầm lẫn nào với tích của các tập hợp $x_\alpha$ được định nghĩa trong lý thuyết tập hợp (*Lý thuyết tập hợp*, II, § 5, no. 3). Tuy nhiên, nếu các $x_\alpha$ là các lực lượng và phép cộng (tương ứng phép nhân) là tổng lực lượng (tương ứng tích lực lượng), thì lực lượng được ký hiệu bởi $\sum_{\alpha \in A} x_\alpha$ (tương ứng $\prod_{\alpha \in A} x_\alpha$) trong ký hiệu trên là tổng lực lượng (tương ứng tích lực lượng) của họ $(x_\alpha)_{\alpha \in A}$ (*Lý thuyết tập hợp*, III, § 3, no. 3).

§ 1.3

Ta chứng minh định lý bằng quy nạp theo lực lượng $n$ của $A$. Gọi $p$ là lực lượng của $I$ và $h$ là phần tử nhỏ nhất của nó; đặt $J = I - \{h\}$. Nếu $n = 1$, vì các $B_i$ không rỗng, tất yếu $p = 1$ và định lý là hiển nhiên. Ngược lại, giả sử định lý đúng cho một tập chỉ số có nhiều nhất $n - 1$ phần tử, ta xét hai trường hợp:

(a) $B_h$ có một phần tử duy nhất $\beta$. Đặt $C = \bigcup_{i \in J} B_i$. Vế trái của (3) bằng, theo định nghĩa, $x_\beta \top \left( \prod_{\alpha \in C} x_\alpha \right)$; vế phải bằng, theo định nghĩa,
$$
x_\beta \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right);
$$
kết quả suy ra từ sự kiện rằng định lý được giả sử đúng đối với $C$ và $(B_i)_{i \in J}$.

(b) Ngược lại, gọi $\beta$ là phần tử nhỏ nhất của $A$ (và do đó của $B_h$); đặt $A' = A - \{\beta\}$ và đặt $B'_i = A' \cap B_i$ với $i \in I$; khi đó $B'_i = B_i$ với $i \in J$. Tập hợp $A'$ có $n - 1$ phần tử và các điều kiện của định lý đúng đối với $A'$ và các tập con $B'_i$ của nó; do đó theo giả thiết:
$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{\alpha \in B'_h} x_\alpha \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right).
$$
Lập hợp thành của $x_\beta$ với mỗi vế, ta có ở vế trái, theo định nghĩa, $\prod_{\alpha \in A} x_\alpha$ và ở vế phải, sử dụng tính kết hợp,
$$
\left( x_\beta \top \left( \prod_{\alpha \in B'_h} x_\alpha \right) \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right)
$$
bằng, theo Định nghĩa 3, vế phải của công thức (3).

Đối với một luật kết hợp được ký hiệu bởi $\top$ thì hợp thành $\prod_{p \leq i \leq q} x_i$ của một dãy $(x_i)_{i \in [p, q]}$ cũng được ký hiệu (vì không thể có sự nhầm lẫn) bởi
$$
x_p \top \cdots \top x_q.
$$
Một trường hợp riêng của Định lý 1 là công thức
$$
x_0 \top x_1 \top \cdots \top x_n = (x_0 \top x_1 \top \cdots \top x_{n-1}) \top x_n.
$$
Xét một dãy có thứ tự gồm $n$ số hạng mà tất cả các số hạng đều bằng cùng một phần tử $x \in E$. Hợp thành của dãy này được ký hiệu bởi $\prod^n x$ đối với một luật được ký hiệu bởi $\top$, $\prod^n x$ đối với một luật được ký hiệu bởi $\perp$. Đối với một luật được viết theo phép nhân, hợp thành được ký hiệu bởi $x^n$ và được gọi là *lũy thừa* thứ $n$ của $x$. Đối với một luật được viết theo phép cộng, hợp thành thường được ký hiệu bởi $nx$. Định lý tính kết hợp áp dụng cho một dãy có thứ tự mà tất cả các số hạng đều bằng nhau cho phương trình

$$
\frac{n_1 + n_2 + \cdots + n_p}{T} x = \left( \frac{n_1}{T} x \right) T \left( \frac{n_2}{T} x \right) T \cdots T \left( \frac{n_p}{T} x \right).
$$

Đặc biệt, nếu $p = 2$,

$$
\frac{m+n}{T} x = \left( \frac{m}{T} x \right) T \left( \frac{n}{T} x \right)
$$
và nếu $n_1 = n_2 = \cdots = n_p = m$,
$$
\frac{pm}{T} x = \frac{p}{T} \left( \frac{m}{T} x \right).
$$

Nếu $X$ là một tập con của $E$, đôi khi chúng ta ký hiệu, phù hợp với ký hiệu ở trên, bởi $\frac{p}{T} X$ tập hợp $X_1 T X_2 T \cdots T X_p$, trong đó
$$
X_1 = X_2 = \cdots = X_p = X;
$$
do đó nó là tập hợp tất cả các hợp thành $x_1 T x_2 T \cdots T x_p$ với $x_1 \in X, x_2 \in X, \ldots, x_p \in X$.

Điều quan trọng là không được nhầm tập hợp này với tập hợp của $\frac{p}{T} x$, trong đó $x$ chạy qua $X$.

### 4. CÁC TẬP CON ỔN ĐỊNH. CÁC LUẬT CẢM SINH

#### Định nghĩa 6 {#alg-i-s1-def-6 .statement}

*Một tập con $A$ của một tập hợp $E$ được gọi là ổn định đối với luật hợp thành $T$ trên $E$ nếu hợp thành của hai phần tử của $A$ thuộc về $A$. Ánh xạ $(x, y) \mapsto x T y$ từ $A \times A$ vào $A$ khi đó được gọi là luật cảm sinh trên $A$ bởi luật $T$. Tập hợp $A$ với luật cảm sinh bởi $T$ được gọi là một magma con của $E$.*

Nói cách khác, để $A$ ổn định đối với một luật $T$ thì điều kiện cần và đủ là $A T A \subset A$. Một tập con ổn định của $E$ và magma con tương ứng thường được đồng nhất.

Giao của một họ các tập con ổn định của $E$ là ổn định; đặc biệt tồn tại một tập con ổn định nhỏ nhất $A$ của $E$ chứa một tập con đã cho $X$; nó được gọi là *sinh* bởi $X$ và $X$ được gọi là một *hệ sinh* của $A$ hoặc một *tập sinh* của $A$. Magma con tương ứng cũng được gọi là *sinh* bởi $X$.

#### Mệnh đề 1 {#alg-i-s1-prop-1 .statement}

*Cho $E$ và $F$ là hai magma và $f$ là một đồng cấu của $E$ vào $F$.
(i) Ảnh theo $f$ của một tập con ổn định của $E$ là một tập con ổn định của $F$.
(ii) Ảnh ngược theo $f$ của một tập con ổn định $F$ là một tập con ổn định của $E$.
(iii) Cho $X$ là một tập con của $E$. Ảnh theo $f$ của tập con ổn định của $E$ sinh bởi $X$ là tập con ổn định của $F$ sinh bởi $f(X)$.
(iv) Nếu $g$ là một đồng cấu thứ hai của $E$ từ $F$ thì tập hợp các phần tử $x$ của $E$ sao cho $f(x) = g(x)$ là một tập con ổn định của $E$.*

Các khẳng định (i), (ii) và (iv) là hiển nhiên; ta chứng minh (iii). Gọi $\overline{X}$ là tập con ổn định của E sinh bởi X và $\overline{f(X)}$ là tập con ổn định của F sinh bởi $f(X)$. Theo (i) $\overline{f(X)} \subset f(\overline{X})$ và theo (ii) $\overline{X} \subset f^{-1}(\overline{f(X)})$, do đó $f(\overline{X}) \subset \overline{f(X)}$.

#### Mệnh đề 2 {#alg-i-s1-prop-2 .statement}

*Cho E là một magma kết hợp và X là một tập con của E. Gọi X' là tập hợp các $x_1 \top x_2 \top \cdots \top x_n$, trong đó $n \geq 1$ và $x_i \in X$ với $1 \leq i \leq n$. Tập con ổn định sinh bởi X bằng X'._

Suy ra ngay lập tức bằng quy nạp theo n rằng hợp thành của một dãy có thứ tự gồm n số hạng thuộc X thuộc tập con ổn định sinh bởi X; do đó chỉ cần kiểm tra rằng X' là ổn định. Bây giờ nếu u và v là các phần tử của X' thì chúng có dạng $u = x_0 \top x_1 \top \cdots \top x_{n-1}$, $v = x_n \top x_{n+1} \top \cdots \top x_{n+p}$ với $x_i \in X$ với $0 \leq i \leq n + p$; khi đó (Định lý 1) $u \top v = x_0 \top x_1 \top \cdots \top x_{n+p}$ thuộc X'.

#### Ví dụ {#alg-i-s1-n4-exa-1 .statement}

(1) Trong tập $\mathbf{N}$ các số tự nhiên, tập con ổn định đối với phép cộng sinh bởi {1} là tập hợp các số nguyên $\geq 1$; đối với phép nhân tập hợp {1} là ổn định.

(2) Cho một luật $\top$ trên một tập hợp E, để một tập con {h} gồm một phần tử duy nhất là ổn định đối với luật $\top$ thì điều kiện cần và đủ là $h \top h = h$; khi đó h được gọi là *lũy đẳng*. Chẳng hạn, mọi phần tử của một dàn đều lũy đẳng đối với mỗi luật sup và inf.

(3) Đối với một luật kết hợp $\top$ trên một tập hợp E, tập con ổn định sinh bởi một tập hợp {a} gồm một phần tử duy nhất là tập hợp các phần tử $\overline{\top}^n a$, trong đó n chạy qua tập hợp các số nguyên $> 0$.

### 5. CÁC PHẦN TỬ HOÁN ĐỔI ĐƯỢC. CÁC LUẬT GIAO HOÁN

#### Định nghĩa 7 {#alg-i-s1-def-7 .statement}

*Cho E là một magma có luật được ký hiệu bởi $\top$. Hai phần tử x và y của E được gọi là giao hoán (hoặc hoán đổi được) nếu $y \top x = x \top y$.*

#### Định nghĩa 8 {#alg-i-s1-def-8 .statement}

*Một luật hợp thành trên một tập hợp E được gọi là giao hoán nếu hai phần tử bất kỳ của E giao hoán theo luật này. Một magma có luật hợp thành giao hoán được gọi là một magma giao hoán.*

Một luật giao hoán bằng với luật đối của nó.

#### Ví dụ {#alg-i-s1-n5-exa-1 .statement}

(1) Phép cộng và phép nhân các số tự nhiên là các luật giao hoán trên $\mathbf{N}$ (*Lý thuyết tập hợp*, III, § 3, no. 3, Hệ quả của Mệnh đề 5).

(2) Trên một dàn, các luật sup và inf là giao hoán; do đó, đặc biệt, các luật $\cup$ và $\cap$ giữa các tập con của một tập hợp E cũng giao hoán.

(3) Cho E là một tập hợp có lực lượng $> 1$. Luật $(f, g) \mapsto f \circ g$ giữa các ánh xạ của E vào E không giao hoán, như thấy được bằng cách lấy f và g là các ánh xạ hằng phân biệt, nhưng ánh xạ đồng nhất giao hoán được với mọi ánh xạ.

(4) Cho $(x, y) \mapsto x \top y$ là một luật giao hoán trên $E$; luật
$$
(X, Y) \mapsto X \top Y
$$
giữa các tập con của $E$ là giao hoán.

#### Định nghĩa 9 {#alg-i-s1-def-9 .statement}

*Cho $E$ là một magma và $X$ là một tập con của $E$. Tập hợp các phần tử của $E$ giao hoán với mỗi phần tử của $X$ được gọi là tập trung hóa của $X$.*

Cho $X$ và $Y$ là hai tập con của $E$ và $X'$ và $Y'$ là các tập trung hóa tương ứng của chúng. Nếu $X \subset Y$, thì $Y' \subset X'$.

Cho $(X_i)_{i \in I}$ là một họ các tập con của $E$ và với mọi $i \in I$ cho $X'_i$ là tập trung hóa của $X_i$. Tập trung hóa của $\bigcup_{i \in I} X_i$ là $\bigcap_{i \in I} X'_i$.

Cho $X$ là một tập con của $E$ và $X'$ là tập trung hóa của $X$. Tập trung hóa $X''$ của $X'$ được gọi là *tập trung hóa kép* của $X$. Khi đó $X \subset X''$. Tập trung hóa $X'''$ của $X''$ bằng $X'$. Vì $X'$ được chứa trong tập trung hóa kép của nó $X'''$ và quan hệ $X \subset X''$ kéo theo $X'''' \subset X'$.

#### Mệnh đề 3 {#alg-i-s1-prop-3 .statement}

*Cho $E$ là một magma kết hợp có luật được ký hiệu bởi $\top$. Nếu một phần tử $x$ của $E$ giao hoán với mỗi phần tử $y$ và $z$ của $E$, thì nó giao hoán với $y \top z$.*

Vì
$$
x \top (y \top z) = (x \top y) \top z = (y \top x) \top z \\
= y \top (x \top z) = y \top (z \top x) = (y \top z) \top x.
$$

#### Hệ quả {#alg-i-s1-n5-cor-1 .statement}

*Cho $E$ là một magma kết hợp. Tập trung hóa của bất kỳ tập con nào của $E$ là một tập con ổn định của $E$.*

#### Định nghĩa 10 {#alg-i-s1-def-10 .statement}

*Tập trung hóa của một magma $E$ được gọi là tâm của $E$. Một phần tử của tâm của $E$ được gọi là một phần tử trung tâm của $E$.*

Nếu $E$ là một magma kết hợp thì tâm của nó là một tập con ổn định theo Hệ quả của Mệnh đề 3 và luật cảm sinh trên tâm của nó là giao hoán.

#### Mệnh đề 4 {#alg-i-s1-prop-4 .statement}

*Cho $E$ là một magma kết hợp, $X$ và $Y$ là hai tập con của $E$. Nếu mọi phần tử của $X$ giao hoán với mọi phần tử của $Y$ thì mọi phần tử của tập con ổn định sinh bởi $X$ giao hoán với mọi phần tử của tập con ổn định sinh bởi $Y$.*

Cho $X'$ và $X''$ lần lượt là toán tử trung tâm và toán tử trung tâm kép của $X$. Chúng là các tập con ổn định của $E$. Bây giờ $X \subset X''$ và $Y \subset X'$ và do đó $X''$ (tương ứng $X'$) chứa tập con ổn định của $E$ sinh bởi $X$ (tương ứng $Y$). Vì mọi phần tử của $X''$ giao hoán với mọi phần tử của $X'$, mệnh đề được suy ra.

#### Hệ quả 1 {#alg-i-s1-prop-4-cor-1 .statement}

*Nếu $x$ và $y$ hoán vị được dưới luật kết hợp $\top$ thì $\top^m x$ và $\top^n y$ cũng hoán vị được với mọi số nguyên $m > 0$ và $n > 0$; đặc biệt $\top^m x$ và $\top^n x$ hoán vị được với mọi $x$ và mọi số nguyên $m > 0$ và $n > 0$.*

#### Hệ quả 2 {#alg-i-s1-prop-4-cor-2 .statement}

*Nếu mọi cặp các phần tử của một tập con X đều hoán vị được dưới một luật kết hợp T, thì luật cảm sinh bởi T trên tập con ổn định sinh bởi X là kết hợp và giao hoán.*

#### Định lý 2 (Định lý giao hoán) {#alg-i-s1-thm-2 .statement}

*Cho T là một luật hợp thành kết hợp trên E; cho $(x_\alpha)_{\alpha \in A}$ là một họ hữu hạn khác rỗng các phần tử của E từng đôi một hoán vị được; cho B và C là hai tập hợp được sắp thứ tự toàn phần với A là tập nền. Khi đó*
$$
\prod_{\alpha \in B} x_\alpha = \prod_{\alpha \in C} x_\alpha.
$$

Vì định lý đúng nếu A có một phần tử duy nhất, ta lập luận bằng quy nạp theo số $p$ các phần tử của A. Cho $p$ là một số nguyên > 1 và giả sử định lý đúng khi Card A < $p$. Ta chứng minh nó cho Card A = $p$. Có thể giả sử rằng A là khoảng $[0, p - 1]$ trong $\mathbf{N}$; hợp thành của dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ được xác định bởi quan hệ thứ tự tự nhiên trên A là $\prod_{i=0}^{p-1} x_i$.

Cho A một thứ tự toàn phần khác và cho h là phần tử nhỏ nhất của A theo thứ tự này và A' là tập các phần tử khác của A (được sắp thứ tự toàn phần bởi thứ tự cảm sinh). Trước hết giả sử $0 < h < p - 1$ và cho P = $\{0, 1, \ldots, h - 1\}$ và Q = $\{h + 1, \ldots, p - 1\}$; định lý được giả sử đúng cho A', áp dụng định lý kết hợp, ta thu được (vì $A' = P \cup Q$)

$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right)
$$

do đó, hợp thành $x_h$ với cả hai vế và áp dụng lặp lại tính giao hoán và tính kết hợp của T:

$$
\begin{align*}
\prod_{\alpha \in A} x_\alpha &= x_h \circ \left( \prod_{\alpha \in A'} x_\alpha \right) = x_h \circ \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right) \\
&= \left( \prod_{i=0}^{h-1} x_i \right) \circ x_h \circ \left( \prod_{i=h+1}^{p-1} x_i \right) = \prod_{i=0}^{p-1} x_i,
\end{align*}
$$

điều này chứng minh định lý trong trường hợp này. Nếu $h = 0$ hoặc $h = p - 1$, cùng một kết quả vẫn đúng, nhưng đơn giản hơn, các số hạng xuất phát từ P hoặc các số hạng xuất phát từ Q không xuất hiện trong các công thức.

Dưới một luật kết hợp giao hoán trên một tập hợp E, *hợp thành* của một *họ hữu hạn* $(x_\alpha)_{\alpha \in A}$ các phần tử của E, theo định nghĩa, là giá trị chung của các hợp thành của tất cả các *dãy có thứ tự* thu được bằng cách sắp thứ tự toàn phần A theo mọi cách có thể. Hợp thành này vẫn được ký hiệu là $\prod_{\alpha \in A} x_\alpha$ dưới một luật ký hiệu là T; tương tự đối với các ký hiệu khác.

#### Định lý 3 {#alg-i-s1-thm-3 .statement}

*Cho T là một luật kết hợp trên E và $(x_\alpha)_{\alpha \in A}$ là một họ hữu hạn khác rỗng các phần tử của E từng đôi một hoán vị được. Nếu A là hợp của các tập con khác rỗng $(B_i)_{i \in I}$ từng đôi một rời nhau, thì*

$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

Điều này suy ra từ Định lý 2 nếu $A$ và $I$ được sắp thứ tự toàn phần sao cho các $B_i$ thỏa mãn các điều kiện của Định lý 1.

Ta nêu riêng hai trường hợp đặc biệt quan trọng của định lý này:

1. If $(x_{\alpha \beta})_{(\alpha, \beta) \in A \times B}$ is a finite family of permutable elements of an associative magma whose indexing set is the product of two non-empty finite sets $A, B$ (a "double family"), then

$$
\prod_{(\alpha, \beta) \in A \times B} x_{\alpha \beta} = \prod_{\alpha \in A} \left( \prod_{\beta \in B} x_{\alpha \beta} \right) = \prod_{\beta \in B} \left( \prod_{\alpha \in A} x_{\alpha \beta} \right)
$$

như suy ra từ Định lý 3 bằng cách xem xét $A \times B$ như hợp của các tập $\{\alpha\} \times B$ một mặt và của các tập $A \times \{\beta\}$ mặt khác.

Ví dụ, nếu $B$ có $n$ phần tử và với mỗi $\alpha \in A$ tất cả các $x_{\alpha \beta}$ đều có cùng một giá trị $x_\alpha$, thì

$$
\prod_{\alpha \in A} \left( \prod^n_{\beta=1} x_\alpha \right) = \prod^n_{\alpha=1} \left( \prod_{\alpha \in A} x_\alpha \right).
$$

Nếu $B$ có hai phần tử, ta thu được các kết quả sau: cho $(x_\alpha)_{\alpha \in A}, (y_\alpha)_{\alpha \in A}$ là hai họ không rỗng các phần tử của $E$. Nếu các $x_\alpha$ và các $y_\beta$ từng đôi một khả hoán, thì

$$
\prod_{\alpha \in A} x_\alpha \prod_{\alpha \in A} y_\alpha = \left( \prod_{\alpha \in A} x_\alpha \right) \prod_{\alpha \in A} y_\alpha.
$$

Do công thức (7), hợp thành của một dãy kép $(x_{ij})$ mà tập chỉ số là tích của hai khoảng $\{p, q\}$ và $\{r, s\}$ trong $\mathbf{N}$ thường được ký hiệu, đối với một luật giao hoán kết hợp được viết theo phép cộng, bởi

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij} \quad \text{hoặc} \quad \sum_{j=r}^s \sum_{i=p}^q x_{ij}
$$

và tương tự đối với các luật được ký hiệu bằng những ký hiệu khác.

2. Let $n$ be an integer $> 0$ and let $A$ be the set of ordered pairs of integers $(i, j)$ such that $0 \leq i \leq n, 0 \leq j \leq n$ and $i < j$; the composition of a family $(x_{ij})_{(i, j) \in A}$ (under a commutative associative law) is also denoted by $\prod_{0 \leq i < j \leq n} x_{ij}$ (or simply $\prod_{i < j} x_{ij}$, if no confusion arises); Theorem 3 here gives the formulae

$$
\prod_{0 \leq i < j \leq n} x_{ij} = \prod_{i=0}^{n-1} \left( \prod_{j=i+1}^n x_{ij} \right) = \prod_{j=1}^n \left( \prod_{i=0}^{j-1} x_{ij} \right).
$$

Có các công thức tương tự công thức (7) đối với một họ mà tập chỉ số là tích của nhiều hơn hai tập, và các công thức tương tự công thức (10) đối với một họ mà tập chỉ số là tập $S_p$ các *dãy tăng ngặt* $(i_k)_{1 \leq k \leq p}$ gồm $p$ số nguyên sao cho $0 \leq i_k \leq n$ ($p \leq n + 1$): trong trường hợp sau, hợp thành của họ $(x_{i_1 i_2 \ldots i_p})_{(i_1, \ldots, i_p) \in S_p}$ được ký hiệu bởi

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p < n} x_{i_1 i_2 \ldots i_p} \quad \text{hoặc đơn giản} \quad \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \ldots i_p}.
$$

#### Mệnh đề 5 {#alg-i-s1-prop-5 .statement}

Cho E và F là các magma có các luật được ký hiệu bởi T và cho f và g là các đồng cấu từ E vào F. Gọi f T g là ánh xạ x ↦ f(x) T g(x) từ E vào F. Nếu F kết hợp và giao hoán, thì f T g là một đồng cấu.

Với mọi phần tử x và y của E:

$$(f T g)(x T y) = f(x T y) T g(x T y) = f(x) T f(y) T g(x) T g(y)$$
$$= f(x) T g(x) T f(y) T g(y) = ((f T g)(x)) T ((f T g)(y)).$$

### 6. CÁC LUẬT THƯƠNG

#### Định nghĩa 11 {#alg-i-s1-def-11 .statement}

Cho E là một tập hợp. Một luật hợp thành T và một quan hệ tương đương R trên E được gọi là tương thích nếu các quan hệ x ≡ x' (mod R) và y ≡ y' (mod R) (với x, x', y, y' ∈ E) kéo theo x T y ≡ x' T y' (mod R); luật hợp thành trên tập thương E/R ánh xạ các lớp tương đương của x và y vào lớp tương đương của x T y được gọi là luật thương của luật T đối với R. Tập hợp E/R cùng với luật thương được gọi là magma thương của E đối với R.

Nói rằng một quan hệ tương đương R trên E tương thích với luật hợp thành nội tại f: E × E → E trên E có nghĩa là ánh xạ f tương thích (theo nghĩa của Lý thuyết Tập hợp, II, § 6, no. 5) với quan hệ tương đương tích R × R trên E × E và quan hệ tương đương R trên E. (Lý thuyết Tập hợp, II, § 6, no. 8). Điều này cũng có nghĩa là đồ thị của R là một magma con của E × E.

Nếu luật T là kết hợp (tương ứng, giao hoán) thì luật thương cũng vậy (nói ngắn gọn hơn, ta nói rằng tính kết hợp, hoặc tính giao hoán, được bảo toàn khi chuyển qua thương).

Ánh xạ chính tắc từ magma E vào magma E/R là một đồng cấu.

Đối với một ánh xạ g từ E/R vào một magma F, điều kiện cần và đủ để g là một đồng cấu là hợp thành của g với ánh xạ chính tắc của E lên E/R là một đồng cấu.

Hai mệnh đề sau đây là ngay lập tức từ các định nghĩa:

#### Mệnh đề 6 {#alg-i-s1-prop-6 .statement}

Cho E và F là hai magma và f là một đồng cấu từ E vào F. Gọi R[x, y] là quan hệ f(x) = f(y) giữa các phần tử x, y của E. Khi đó R là một quan hệ tương đương trên E tương thích với luật trên E và ánh xạ từ E/R lên f(E) dẫn xuất từ f bằng cách chuyển qua thương là một đẳng cấu từ magma thương E/R lên magma con f(E) của F.

#### Mệnh đề 7 {#alg-i-s1-prop-7 .statement}

Cho E là một magma và R là một quan hệ tương đương trên E tương thích với luật trên E. Để một quan hệ tương đương S trên E/R tương thích với luật thương, điều kiện cần và đủ là S có dạng T/R, trong đó T là một quan hệ tương đương trên E được suy ra từ R và tương thích với luật trên E. Khi đó ánh xạ chính tắc từ E/T lên (E/R)/(T/R) (Lý thuyết Tập hợp, II, § 6, no. 7) là một đẳng cấu magma.

#### Mệnh đề 8 {#alg-i-s1-prop-8 .statement}

Cho E là một magma, A là một tập con ổn định của E và R là một quan hệ tương đương trên E tương thích với luật trên E. Bao đóng B của A đối với R (Lý thuyết Tập

Gọi $\top$ là luật trên $E$. Nếu $x$ và $y$ là hai phần tử của $B$ thì tồn tại hai phần tử $x'$ và $y'$ của $A$ sao cho $x \equiv x' \pmod{R}$ và $y \equiv y' \pmod{R}$; khi đó $x \top y \equiv x' \top y' \pmod{R}$ và $x' \top y' \in A$, do đó $x \top y \in B$. Vậy $B$ là một tập con ổn định của $E$ và các khẳng định khác là hiển nhiên.

Cho $M$ là một magma và $((u_\alpha, v_\alpha))_{\alpha \in I}$ là một họ các phần tử của $M \times M$. Xét tất cả các quan hệ tương đương $S$ trên $M$ tương thích với luật trên $M$ và sao cho $u_\alpha \equiv v_\alpha \pmod{S}$ với mọi $\alpha \in I$. Giao của các đồ thị của các quan hệ này là đồ thị của một quan hệ tương đương $R$ tương thích với luật trên $M$ và sao cho $u_\alpha \equiv v_\alpha \pmod{R}$. Do đó $R$ là quan hệ tương đương mịn nhất (Lý thuyết tập hợp, III, § 1, các số 3 và 7) có hai tính chất này. Nó được gọi là quan hệ tương đương tương thích với luật trên $M$ sinh bởi các $(u_\alpha, v_\alpha)$.

#### Mệnh đề 9 {#alg-i-s1-prop-9 .statement}

Giữ nguyên ký hiệu trên, cho $f$ là một đồng cấu từ $M$ vào một magma sao cho $f(u_\alpha) = f(v_\alpha)$ với mọi $\alpha \in I$. Khi đó $f$ tương thích với $R$.

Cho $T$ là quan hệ tương đương liên kết với $f$. Khi đó $u_\alpha \equiv v_\alpha \pmod{T}$ với mọi $\alpha \in I$ và $T$ tương thích với luật trên $M$, do đó $T$ thô hơn $R$; điều này chứng minh mệnh đề.

### Bài tập {#alg-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
