---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 1
section_title: Algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0452-0462, 0642-0642
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ALGEBRA
      page: 0
      pdf_page: 452
    - "no": 2
      title: SUBALGEBRAS. IDEALS. QUOTIENT ALGEBRAS
      page: 0
      pdf_page: 453
    - "no": 3
      title: DIAGRAMS EXPRESSING ASSOCIATIVITY AND COMMUTATIVITY
      page: 0
      pdf_page: 455
    - "no": 4
      title: PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 456
    - "no": 5
      title: RESTRICTION AND EXTENSION OF SCALARS
      page: 0
      pdf_page: 457
    - "no": 6
      title: INVERSE AND DIRECT LIMITS OF ALGEBRAS
      page: 0
      pdf_page: 458
    - "no": 7
      title: BASES OF AN ALGEBRA. MULTIPLICATION TABLE
      page: 0
      pdf_page: 460
statements: 5
exercises: 1
content_sha256: 72426c09e6abcc97a1768328d91d6cf476003479c528e977b35086f32eca7a0e
translated_from: content/en/alg/III/01_s1_algebras.md
source_content_sha256: 853e46b000e1371a2a7000c89d62a9451dbe1eeb1284e7720ff37b270335c947
translation_model: gpt-5-6-mini
translation_run: translate-vi-118c701b
glossary_version: 34
glossary_terms_sha256: b7cda63a24ecb0d9192a28e7fb04bd4e0bcd6bdacd7e723546d55576fcd6f5bd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐẠI SỐ

### 1. ĐỊNH NGHĨA ĐẠI SỐ

#### Định nghĩa 1 {#alg-iii-s1-def-1 .statement}

Cho $A$ là một vành giao hoán. Một đại số trên $A$ (hay một $A$-đại số, hoặc đơn giản là một đại số, khi không sợ nhầm lẫn) là một tập hợp $E$ với một cấu trúc được xác định bằng cách cho:
(1) một cấu trúc $A$-môđun trên $E$;
(2) một ánh xạ song tuyến tính trên $A$ (II, § 3, no. 5) từ $E \times E$ vào $E$.

Ánh xạ song tuyến tính trên $A$ từ $E \times E$ vào $E$ xuất hiện trong định nghĩa này được gọi là phép nhân của đại số $E$; nó thường được ký hiệu bởi $(x, y) \mapsto x.y$, hoặc đơn giản bởi $(x, y) \mapsto xy$.

Cho $(\alpha_i)_{i \in I}$ và $(\beta_j)_{j \in J}$ là hai họ các phần tử của $A$, có giá hữu hạn (I, § 2, no. 1). Khi đó, với mọi họ $(x_i)_{i \in I}$ và $(y_j)_{j \in J}$ các phần tử của $E$, công thức phân phối tổng quát (I, § 3, no. 4)

$$
\left( \sum_{i \in I} \alpha_i x_i \right) \left( \sum_{j \in J} \beta_j y_j \right) = \sum_{(i, j) \in I \times J} (\alpha_i \beta_j)(x_i y_j)
$$

đúng; đặc biệt

$$
(\alpha x)y = x(\alpha y) = \alpha(xy) \quad \text{với } \alpha \in A, x \in E \text{ và } y \in E.
$$

Ánh xạ song tuyến tính $(x, y) \mapsto yx$ từ $E \times E$ vào $E$ và cấu trúc $A$-môđun trên $E$ xác định trên $E$ một cấu trúc $A$-đại số, gọi là đối với cấu trúc đại số đã cho. Tập hợp $E$ với cấu trúc mới này được gọi là đại số đối của đại số $E$; nó thường được ký hiệu là $E^0$. Đại số $A$-đại số $E$ được gọi là giao hoán nếu nó đồng nhất với đại số đối của nó, nói cách khác nếu phép nhân trong $E$ là giao hoán. Một đẳng cấu từ $E$ lên $E^0$ cũng được gọi là một tự đẳng cấu đối của đại số $E$.

Khi phép nhân trong đại số $E$ là kết hợp, $E$ được gọi là một $A$-đại số kết hợp. Khi phép nhân trong $E$ có một phần tử đơn vị (duy nhất tất yếu (I, § 2, no. 1)), phần tử này được gọi là phần tử đơn vị của $E$ và $E$ được gọi là một đại số có đơn vị.

#### Ví dụ {#alg-iii-s1-n1-exa-1 .statement}

(1) Mọi vành giao hoán $A$ đều có thể được xem như một $A$-đại số (kết hợp và giao hoán).
(2) Cho $E$ là một vành giả (I, § 8, no. 1). Phép nhân trên $E$ và cấu trúc $\mathbf{Z}$-môđun duy nhất trên $E$ xác định trên $E$ một cấu trúc $\mathbf{Z}$-đại số kết hợp.
(3) Cho $F$ là một tập hợp và $A$ là một vành giao hoán. Tập hợp $A^F$ gồm mọi ánh xạ từ $F$ vào $A$, với cấu trúc vành tích (I, § 8, no. 10) và cấu trúc

$A$-môđun tích (II, § 1, no. 5) là một $A$-đại số kết hợp và giao hoán.

(4) Cho E là một $A$-đại số; các luật nội tại $(x, y) \mapsto xy + yx$ và $(x, y) \mapsto xy - yx$ xác định (cùng với cấu trúc $A$-môđun trên E) hai cấu trúc $A$-đại số trên E, nói chung không kết hợp; luật thứ nhất

$$(x, y) \mapsto xy + yx$$

luôn giao hoán.

#### Định nghĩa 2 {#alg-iii-s1-def-2 .statement}

*Cho hai đại số* E, E' *trên một vành giao hoán* A, *một đồng cấu của* E *vào* E' *là một ánh xạ* $f : E \to E'$ *sao cho*
(1) *f là một đồng cấu* A*-môđun*;
(2) $f(xy) = f(x)f(y)$ *với mọi* $x \in E$ *và* $y \in E$.

Rõ ràng hợp thành của hai đồng cấu đại số trên A là một đồng cấu đại số trên A. Mọi đồng cấu đại số song ánh đều là một đẳng cấu. Do đó, có thể lấy các đồng cấu đại số trên A làm các *cấu xạ* của loài cấu trúc đại số trên A (*Lý thuyết tập hợp*, IV, 2, no. 1). Trong những điều sau đây, ta luôn giả sử rằng lựa chọn các cấu xạ này đã được thực hiện. Nếu E, E' là hai đại số trên A, ký hiệu $\operatorname{Hom}_{A\text{-alg}}(E, E')$ là tập hợp các đồng cấu đại số trên A của E vào E'.

Cho E, E' là hai đại số, mỗi đại số đều có một phần tử đơn vị. Một đồng cấu của E vào E' biến phần tử đơn vị của E thành phần tử đơn vị của E' được gọi là một *đồng cấu có đơn vị* (hay *cấu xạ đại số có đơn vị*).

### 2. ĐẠI SỐ CON. IĐÊAN. ĐẠI SỐ THƯƠNG

Cho A là một vành giao hoán và E là một đại số trên A. Nếu F là một môđun con trên A của W ổn định đối với phép nhân trên E, thì hạn chế trên F × F của phép nhân của E xác định (cùng với cấu trúc môđun trên A của F) một cấu trúc đại số trên A trên F. F, với cấu trúc này, được gọi là một *đại số con* của đại số trên A E. Mọi giao của các đại số con của E đều là một đại số con của E. Với mọi họ $(x_i)_{i \in I}$ các phần tử của E, giao của các đại số con của E chứa tất cả các $x_i$ được gọi là đại số con của E *sinh* bởi họ $(x_i)_{i \in I}$ và $(x_i)_{i \in I}$ được gọi là một *hệ sinh* (hay *họ sinh*) của đại số con này. Nếu $u : E \to E'$ là một đồng cấu đại số trên A, ảnh $u(F)$ của mọi đại số con F của E là một đại số con của E'.

Cho E là một đại số *kết hợp*. Với mọi tập con M của E, tập $M'$ gồm các phần tử của E hoán đổi được với mọi phần tử của M là một đại số con của E, được gọi là đại số con *trung tâm hóa* của M trong E (I, § 1, no. 5). Trung tâm hóa $M''$ của $M'$ trong E cũng được gọi là *trung tâm hóa kép* của M; rõ ràng $M \subset M''$. Suy ra rằng $M'$ được chứa trong trung tâm hóa kép $M''$ của nó, mà chính là trung tâm hóa của $M''$; nhưng quan hệ $M \subset M''$ kéo theo $M'' \subset M'$, do đó $M' = M''$ (xem *Lý thuyết tập hợp*, III, § 1, no. 7, Mệnh đề 2). Nếu F là một đại số con của E, *tâm* của F là giao $F \cap F'$ của F và trung tâm hóa $F'$ của nó trong E. Chú ý rằng nếu

F là *giao hoán*, thì $F \subset F'$ và do đó $F' \supset F''$; trung tâm hóa kép $F''$ của F trong trường hợp này là *tâm* của F.

Đối với một số đại số không kết hợp (chẳng hạn các đại số Lie), các khái niệm trung tâm hóa của một đại số con và tâm được định nghĩa khác đi (*Nhóm Lie và đại số Lie*, I, § 1, no. 6).

Một tập con $a$ của một đại số trên A E được gọi là một *iđêan trái* (resp. *iđêan phải*) của E khi $a$ là một môđun con trên A của E và các quan hệ $x \in a,\ y \in E$ kéo theo $yx \in a$ (resp. $xy \in a$). Nói cách khác, $a$ là một iđêan trái của E khi và chỉ khi nó là một iđêan phải của đại số đối $E^0$. Một *iđêan hai phía* của E là một tập con $a$ của E vừa là một iđêan trái vừa là một iđêan phải. Khi E là kết hợp và có một phần tử đơn vị $e$, thì, với $\alpha \in A$ và $x \in E$, $\alpha x = (\alpha e)x = x(\alpha e)$ theo (2) (no. 1), và do đó các iđêan (phải, trái, hai phía) của *vành* E (I, § 8, no. 6) trùng với các iđêan (phải, trái, hai phía) của *đại số* E. Mọi tổng và mọi giao của các iđêan trái (resp. phải, hai phía) của đại số E đều là một iđêan trái (resp. phải, hai phía). Giao của các iđêan trái (resp. phải, resp. hai phía) chứa một tập con X của E được gọi là iđêan trái (resp. phải, resp. hai phía) của E *sinh* bởi X.

Cho $b$ là một iđêan *hai phía* của một đại số trên A E. Nếu $x \equiv x' \pmod{b}$ và $y \equiv y' \pmod{b}$, thì
$$
x(y - y') \in b \quad \text{và} \quad (x - x')y' \in b
$$
và do đó $xy \equiv x'y' \pmod{b}$. Vì vậy, có thể xác định một luật nội trên môđun thương trên A $E/b$, là thương của luật nhân $(x, y) \mapsto xy$ của E theo quan hệ tương đương $x \equiv x' \pmod{b}$ (I, § 1, no. 6). Ngay lập tức kiểm tra được rằng luật thương này là một ánh xạ song tuyến tính trên A từ $(E/b) \times (E/b)$ vào $E/b$; do đó nó xác định, cùng với cấu trúc môđun trên A của $E/b$, một cấu trúc đại số trên A trên $E/b$. $E/b$, với cấu trúc đại số này, được gọi là *đại số thương* của đại số E theo iđêan hai phía $b$. Ánh xạ chính tắc $p : E \to E/b$ là một đồng cấu đại số.

Cho E, $E'$ là hai đại số trên A và $u : E \to E'$ là một đồng cấu đại số. Ảnh $u(E)$ là một đại số con của $E'$ và hạt nhân $b = u^{-1}(0)$ là một iđêan hai phía của E; hơn nữa, trong phân tích chính tắc của $u$:
$$
E \xrightarrow{p} E/b \xrightarrow{v} u(E) \xrightarrow{j} E'
$$
$v$ là một *đẳng cấu đại số*. Nói chung, mọi kết quả của Chương I, § 8, no. 9 vẫn còn đúng (và cả các chứng minh của chúng) khi từ "vành" được thay bằng "đại số".

Cho A là một vành giao hoán và E là một đại số trên A. Trên tập hợp $\tilde{E} = A \times E$, ta định nghĩa các luật hợp thành sau:
$$
\begin{align*}
(\lambda, x) + (\mu, y) &= (\lambda + \mu, x + y) \\
(\lambda, x)(\mu, y) &= (\lambda \mu, xy + \mu x + \lambda y) \\
\lambda(\mu, x) &= (\lambda \mu, \lambda x).
\end{align*}
$$

Ngay lập tức kiểm tra được rằng $\tilde{E}$, với các luật hợp thành này, là một đại số trên $A$ và $(1,0)$ là một phần tử đơn vị của đại số này. Tập $\{0\} \times E$ là một iđêan hai phía của $\tilde{E}$ và $x \mapsto (0,x)$ là một đẳng cấu của đại số E lên đại số con $\{0\} \times E$, nhờ đó E và $\{0\} \times E$ được đồng nhất. $\tilde{E}$ được gọi là đại số dẫn xuất từ E bằng cách ghép thêm một phần tử đơn vị; nó kết hợp (tương ứng, giao hoán) khi và chỉ khi E kết hợp.

### 3. CÁC BIỂU ĐỒ BIỂU DIỄN TÍNH KẾT HỢP VÀ TÍNH GIAO HOÁN

Cho $A$ là một vành giao hoán và $E$ một A-môđun; cho một ánh xạ song tuyến tính từ $E \times E$ vào E tương đương với cho một ánh xạ A-tuyến tính:

$$
m : E \otimes_A E \to E
$$

(II, § 3, no. 5). Do đó, một cấu trúc đại số trên $E$ được xác định bằng cách cho một cấu trúc môđun A trên $E$ và một ánh xạ A-tuyến tính từ $E \otimes_A E$ vào E.

Cho $E'$ là một đại số trên A khác và $m' : E' \otimes_A E' \to E'$ là ánh xạ A-tuyến tính xác định phép nhân của $E'$. Một ánh xạ $f : E \to E'$ là một đồng cấu đại số trên A khi và chỉ khi $f$ là một ánh xạ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{f \otimes f} & E' \otimes_A E' \\
\downarrow m & & \downarrow m' \\
E & \xrightarrow{f} & E'
\end{array}
$$

Để một đại số trên $A$ là kết hợp, điều kiện cần và đủ (tính đến tính kết hợp của các tích tenxơ, cf. II, § 3, no. 8) là biểu đồ của các ánh xạ A-tuyến tính

$$
\begin{array}{ccc}
E \otimes_A E \otimes_A E & \xrightarrow{m \otimes 1_E} & E \otimes_A E \\
\downarrow 1_E \otimes m & & \downarrow m \\
E \otimes_A E & \xrightarrow{m} & E
\end{array}
$$

là giao hoán. Tương tự, để đại số trên $A$ là giao hoán, điều kiện cần và đủ là biểu đồ của các ánh xạ A-tuyến tính

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E \\
\downarrow m & & \downarrow m \\
E & & E
\end{array}
$$

là giao hoán, trong đó $\sigma$ ký hiệu ánh xạ A-tuyến tính chính tắc được xác định bởi σ(x \otimes y) = y \otimes x \text{ với } x \in E, y \in E \text{ (II, § 3, no. 1, Hệ quả 2 của Mệnh đề 1).}

Với mọi $c \in E$, ký hiệu $\eta_c$ là ánh xạ A-tuyến tính từ A vào E được xác định bởi điều kiện $\eta_c(1) = c$. Để $c$ là một phần tử đơn vị của E, điều kiện cần và đủ là hai biểu đồ

$$
\begin{array}{ccc}
A \otimes_A E & \xrightarrow{\eta_c \otimes 1_E} & E \otimes_A E \\
\downarrow i & & \downarrow m \\
E & & E \\
& \uparrow & \\
E \otimes_A A & \xrightarrow{1_E \otimes \eta_c} & E \otimes_A E \\
& \downarrow i' & \downarrow m \\
E & & E
\end{array}
$$

là giao hoán ($i$ và $i'$ ký hiệu các đẳng cấu chính tắc (II, § 3, no. 4, Mệnh đề 4)).

Cho E là một đại số trên A có phần tử đơn vị e và đặt $\eta = \eta_e$ (cũng ký hiệu là $\eta_E$); khi đó $\eta(\alpha \beta) = \eta(\alpha) \eta(\beta) = \alpha \eta(\beta)$, vì theo (2) (no. 1),

$$(\alpha e)(\beta e) = (\alpha \beta)e = \alpha(\beta e);$$

do đó $\eta$ là một đồng cấu đại số trên A. Chú ý rằng cấu trúc môđun trên A của E có thể được định nghĩa bằng cách dùng $\eta$, vì

$$(3)$$
$$\alpha x = \eta(\alpha) \cdot x \quad \text{với } \alpha \in A, x \in E$$

(trong đó, ở vế phải, phép nhân được thực hiện trong E). Ảnh của đồng cấu $\eta$ là một đại số con của E mà các phần tử của nó giao hoán với mọi phần tử của E. Hạt nhân của đồng cấu $\eta$ là linh hóa tử của phần tử e của A-môđun E; theo (3), nó cũng là linh hóa tử của A-môđun E (II, § 1, no. 12).

Khi đại số E có đơn vị và kết hợp, $\eta$ là một đồng cấu vành. Ngược lại, cho $\rho : A \to B$ là một đồng cấu vành sao cho ảnh $\rho(A)$ được chứa trong tâm của B, đồng thời giả sử vành A giao hoán; khi đó trên B có một cấu trúc đại số trên A, kết hợp và có đơn vị, bằng cách viết (xem (3))

$$\lambda x = \rho(\lambda) \cdot x \quad \text{với } \lambda \in A, x \in E.$$

### 4. TÍCH CỦA CÁC ĐẠI SỐ

Cho $(E_i)_{i \in I}$ là một họ các đại số trên cùng một vành giao hoán A. Người ta kiểm tra ngay lập tức rằng trên tập hợp tích $E = \prod_{i \in I} E_i$, cấu trúc A-môđun tích (II, § 1, no. 5) và phép nhân

$$(4)$$
$$((x_i), (y_i)) \mapsto (x_i y_i)$$

xác định một cấu trúc đại số trên A; với cấu trúc này, tập hợp E được gọi là đại số tích của họ các đại số $(E_i)_{i \in I}$.

Khi tất cả các đại số $E_i$ đều kết hợp (tương ứng, giao hoán, tương ứng, có đơn vị), thì tích của chúng cũng vậy. Hơn nữa, mọi tính chất nêu trong I, § 8, no. 10 đều mở rộng không thay đổi cho các tích tùy ý của các đại số.

### 5. HẠN CHẾ VÀ MỞ RỘNG CÁC VÔ HƯỚNG

Cho $A_0$ và A là hai vành giao hoán và $\rho : A_0 \to A$ là một đồng cấu vành. Nếu E là một đại số trên A, ta ký hiệu (phù hợp với II, § 1, no. 13) $\rho_* (E)$ là A-môđun được xác định bởi phép cộng trên E và phép toán ngoài

$$
\lambda . x = \rho(\lambda)x \quad \text{với mọi } \lambda \in A_0 \text{ và mọi } x \in E.
$$

Phép nhân trong E và cấu trúc A-môđun trên $\rho_* (E)$ xác định một cấu trúc đại số trên A trên $\rho_* (E)$. Khi $A_0$ là một vành con của A và $\rho$ là đơn ánh chính tắc, đại số $\rho_* (E)$ được nói là thu được từ E bằng cách hạn chế vành vô hướng A xuống $A_0$. Do lạm dụng ngôn ngữ, người ta cũng đôi khi nói như vậy khi $\rho$ tùy ý.

Cho F là một đại số trên $A_0$. Một đồng cấu đại số trên $A_0$ $F \to \rho_* (E)$ được gọi là một bán-đồng cấu (đối với $\rho$) hoặc một $\rho$-đồng cấu của F vào đại số trên A E; nó cũng được gọi là một đồng cấu trên $A_0$ nếu không gây nhầm lẫn. Nếu E, $E'$ là hai đại số trên A, mọi đồng cấu đại số trên A $E \to E'$ cũng là một đồng cấu đại số trên $A_0$ $\rho_* (E) \to \rho_* (E')$.

Xét hai vành giao hoán A và B và một đồng cấu vành $\rho : A \to B$. Với mọi A-môđun E, B-môđun $\rho^*(E) = E \otimes_A B$, thu được từ E bằng cách mở rộng vành vô hướng A lên B, đã được định nghĩa (II, § 5, no. 1). Nếu E cũng là một đại số trên A, ta sẽ định nghĩa trên $\rho^*(E)$ một cấu trúc đại số trên B. Vì mục đích này, nhận thấy rằng $(E \otimes_A B) \otimes_B (E \otimes_A B)$ đẳng cấu một cách chính tắc với $(E \otimes_A E) \otimes_A B$ (II, § 5, no. 1, Mệnh đề 3). Nếu $m : E \otimes_A E \to E$ xác định phép nhân trên E, ánh xạ $m \otimes 1_B : (E \otimes_A E) \otimes_A B \to E \otimes_A B$ do đó được đồng nhất một cách chính tắc với một ánh xạ B-tuyến tính

$$
m' : \rho^*(E) \otimes_B \rho^*(E) \to \rho^*(E)
$$

xác định cấu trúc đại số trên B mong muốn trên $\rho^*(E)$. Do đó

(5)

$$
(x \otimes \beta)(x' \otimes \beta') = (xx') \otimes (\beta \beta')
$$

đối với $x, x'$ trong E, $\beta$ và $\beta'$ trong B. Đại số trên B $\rho^*(E)$ được gọi là dẫn xuất từ đại số trên A E bằng cách mở rộng vành A các vô hướng đến B (thông qua $\rho$). Nó cũng được ký hiệu là $E_{(B)}$ hoặc $E \otimes_A B$. Khi E kết hợp (tương ứng giao hoán, tương ứng có đơn vị), thì $\rho^*(E)$ cũng vậy.

#### Mệnh đề 1 {#alg-iii-s1-prop-1 .statement}

Với mọi đại số trên A E, ánh xạ chính tắc $\phi_E : x \mapsto x \otimes 1$ từ E vào $E_{(B)}$ là một đồng cấu đại số trên A. Hơn nữa, với mọi đại số trên B F và mọi đồng cấu $A$-đại số $f : E \to F$, tồn tại duy nhất một đồng cấu $B$-đại số $\bar{f} : E_{(B)} \to F$ sao cho $\bar{f}(x \otimes 1) = f(x)$ với mọi $x \in E$.

Mệnh đề đầu tiên suy ra ngay lập tức từ định nghĩa phép nhân trong $E_{(B)}$, cho $(x \otimes 1)(x' \otimes 1) = (xx') \otimes 1$ với $x \in E$ và $x' \in E$. Sự tồn tại và tính duy nhất của ánh xạ $B$-tuyến tính $\bar{f}$ từ $E_{(B)}$ vào F thỏa mãn quan hệ $\bar{f}(x \otimes 1) = f(x)$ với mọi $x \in E$ suy ra từ II, § 5, no. 1, Mệnh đề 1; ở đây, tất cả quy về việc kiểm tra rằng $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ với $y$ và $y'$ trong $E_{(B)}$; vì các phần tử có dạng $x \otimes 1$ (với $x \in E$) sinh môđun $B$ $E_{(B)}$, ta có thể chỉ xét trường hợp $y = x \otimes 1, y' = x' \otimes 1$ với $x \in E, x' \in E$; vì $yy' = (xx') \otimes 1$, quan hệ $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ khi đó suy ra từ $f(xx') = f(x)f(x')$.

Cũng có thể nói rằng $f \mapsto \bar{f}$ là một song ánh chính tắc

$$
\text{Hom}_{A\text{-đại số.}}(E, \rho_*(F)) \to \text{Hom}_{B\text{-đại số.}}(\rho^*(E), F).
$$

Do đó, cặp có thứ tự gồm $E_{(B)}$ và $\phi_E$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết Tập hợp, IV, § 3, no. 1), trong đó $\Sigma$ là loài cấu trúc đại số trên $B$ và các ánh xạ $\alpha$ là các đồng cấu từ $E$ vào một đại số trên $B$.

#### Hệ quả {#alg-iii-s1-n5-cor-1 .statement}

*Cho $E, E'$ là hai đại số trên $A$; với mọi đồng cấu đại số trên $A$ $u : E \to E'$, $u \otimes 1_B$ là đồng cấu đại số trên $B$ duy nhất $v : E \otimes_A B \to E' \otimes_A B$ làm cho biểu đồ giao hoán*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E \otimes_A B \\
u \downarrow & & \downarrow v \\
E' & \xrightarrow{\phi_{E'}} & E' \otimes_A B
\end{array}
$$

Cho $C$ là một vành giao hoán thứ ba và $\sigma : B \to C$ là một đồng cấu vành; ngay lập tức thấy rằng đồng cấu $C$ chính tắc

$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$

ánh xạ $(x \otimes 1) \otimes 1$ thành $x \otimes 1$ với mọi $x \in E$ (II, § 5, no. 1, Mệnh đề 2) là một đẳng cấu đại số.

### 6. GIỚI HẠN NGƯỢC VÀ GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ

Cho $I$ là một tập tiền thứ tự và $(A_i, \phi_{ij})$ là một hệ ngược của các *vành giao hoán* với $I$ làm tập chỉ số. Cho $(E_i, f_{ij})$ là một hệ ngược của các môđun $A_i$ với $I$ làm tập chỉ số (II, § 6, no. 1) và giả sử thêm rằng mỗi $E_i$ có một cấu trúc đại số trên $A_i$ và với $i \leq j$, $f_{ij}$ là một đồng cấu đại số $A_j$ (đối với $\phi_{ij}$) (no. 5). Đặt $A = \lim \leftarrow A_i$ và $E = \lim \leftarrow E_i$, nó có một cấu trúc $A$-môđun, là giới hạn ngược của cấu trúc các $A_i$-môđun $E_i$ (II, § 6, no. 1); ta kiểm tra ngay lập tức rằng luật hợp thành trên $E$, được xét như giới hạn ngược của các $E_i$ được xét như các magma đối với phép nhân (I, § 10, no. 1), cùng với cấu trúc $A$-môđun trên $E$, xác định trên $E$ một cấu trúc đại số $A$; $(E_i, f_{ij})$ được gọi là một *hệ ngược* của các đại số $A_i$ và đại số $A$-đại số $E$ được gọi là *giới hạn ngược* của nó. Nếu $f_i : E \to E_i$, $\phi_i : A \to A_i$ là các ánh xạ chính tắc, $f_i$ là một đồng cấu đại số *$A$* (đối với $\phi_i$). Nếu các $E_i$ là kết hợp (tương ứng, giao hoán), thì $E$ cũng vậy; nếu mỗi $E_i$ có một phần tử đơn vị $e_i$ và $f_{ij}(e_j) = e_i$ với $i \leq j$, thì $e = (e_i)$ là một phần tử đơn vị của đại số $E$.

Cho $(E'_i, f'_{ij})$ là một hệ ngược khác của các đại số $A_i$ và với mọi $i$, $u_i : E_i \to E'_i$ là một đồng cấu đại số $A_i$, các ánh xạ này lập thành một *hệ ngược*; khi đó $u = \lim u_i$ là một *đồng cấu đại số $A$*.

Giả sử bây giờ rằng tất cả các $A_i$ đều bằng cùng một *vành* giao hoán $A$ và các $\phi_{ij}$ bằng $\mathrm{Id}_A$, sao cho $E = \lim \leftarrow E_i$ là một $A$-đại số. Cho $F$ là một $A$-đại số và, với mọi $i \in I$, cho $u_i : F \to E_i$ là một đồng cấu đại số trên $A$ sao cho $(u_i)$ là một hệ ngược các ánh xạ; khi đó $u = \lim \leftarrow u_i$ là một đồng cấu của đại số $F$ vào đại số $E$. *Ngược lại*, với mọi đồng cấu đại số trên $A$ $v : F \to E$, họ các $v_i = f_i \circ v$ là một hệ ngược các đồng cấu đại số trên $A$ sao cho $v = \lim \leftarrow v_i$. Hơn nữa, viết $\bar{f}_{ij} = \mathrm{Hom}(1_F, f_{ij})$, $(\mathrm{Hom}_{A\text{-đại số.}}(F, E_i), \bar{f}_{ij})$ rõ ràng là một hệ ngược các tập hợp, nên thấy rằng các nhận xét trên cũng có thể được diễn đạt bằng cách nói rằng ánh xạ chính tắc $v \mapsto (f_i \circ v)$ là một *song ánh*

$$
l_F : \mathrm{Hom}_{A\text{-đại số.}}(F, \lim \leftarrow E_i) \to \lim \leftarrow \mathrm{Hom}_{A\text{-đại số.}}(F, E_i).
$$

Hơn nữa, với mọi đồng cấu đại số trên $A$ $w : F \to F'$, các

$$
\bar{w}_i = \mathrm{Hom}(w, 1_{E_i}) : \mathrm{Hom}_{A\text{-đại số.}}(F', E_i) \to \mathrm{Hom}_{A\text{-đại số.}}(F, E_i)
$$

tạo thành một hệ ngược các ánh xạ và biểu đồ

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-đại số.}}(F', \lim \leftarrow E_i) & \xrightarrow{l_{F'}} & \lim \leftarrow \mathrm{Hom}_{A\text{-đại số.}}(F', E_i) \\
\downarrow \mathrm{Hom}(w, 1_E) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-đại số.}}(F, \lim \leftarrow E_i) & \xrightarrow{l_F} & \lim \leftarrow \mathrm{Hom}_{A\text{-đại số.}}(F, E_i)
\end{array}
$$

là giao hoán.

Giả sử bây giờ rằng $I$ có *hướng phải*. Xét một hệ trực tiếp các vành giao hoán $(A_i, \phi_{ji})$ và một hệ trực tiếp $(E_i, f_{ji})$ của các $A_i$-môđun, với $I$ làm tập hợp chỉ số; giả sử rằng mỗi $E_i$ có một cấu trúc $A_i$-đại số và, với $i \leq j$, $f_{ji}$ là một đồng cấu đại số trên $A_i$ (đối với $\phi_{ji}$) (no. 5). Đặt $A = \lim \to A_i$, $E = \lim \to E_i$; $E$ có một cấu trúc $A$-môđun, là giới hạn trực tiếp của các cấu trúc $A_i$-môđun của $E_i$ (II, § 6, no. 2); hơn nữa, luật hợp thành trên E được xét như giới hạn trực tiếp của các E_i, được xét như các magma đối với phép nhân (I, § 10, no. 3), cùng với cấu trúc $A$-môđun trên E, xác định một cấu trúc $A$-đại số trên E; $(E_i, f_{ji})$ được gọi là một hệ trực tiếp các $A_i$-đại số và $A$-đại số E được gọi là giới hạn trực tiếp của nó. Nếu f_i : E_i \to E, \phi_i : A_i \to A là các ánh xạ chính tắc, f_i là một đồng cấu đại số trên $A_i$ (đối với $\phi_i$). Nếu các E_i kết hợp (tương ứng, giao hoán), thì E cũng vậy; nếu mỗi E_i có một phần tử đơn vị e_i và f_{ji}(e_i) = e_j với i \leq j, E có một phần tử đơn vị e sao cho f_i(e_i) = e với mọi i \in I.

Cho $(E'_i, f'_{ji})$ là một hệ trực tiếp khác của các $A_i$-đại số và với mọi i cho $u_i : E_i \to E'_i$ là một đồng cấu đại số trên $A_i$, các ánh xạ này tạo thành một hệ trực tiếp; khi đó u = \lim \to u_i là một đồng cấu đại số trên A.

Giả sử bây giờ rằng tất cả các vành A_i đều bằng cùng một vành A và các $\phi_{ji}$ bằng Id_A, sao cho E = \lim \to E_i là một A-đại số. Cho F là một A-đại số và với mọi i cho u_i : E_i \to F là một đồng cấu đại số trên A sao cho (u_i) là một hệ trực tiếp các ánh xạ; khi đó u = \lim \to u_i là một đồng cấu của đại số E vào đại số F. Ngược lại, với mọi đồng cấu đại số trên A v : E \to F, họ các v_i = v \circ f_i là một hệ trực tiếp các đồng cấu đại số trên A sao cho v = \lim \to v_i. Hơn nữa, viết $\vec{f}_{ij} = \mathrm{Hom}(f_{ij}, 1_F)$, $(\mathrm{Hom}_{A\text{-đại số.}}(E_i, F), \vec{f}_{ij})$ rõ ràng là một hệ ngược các tập hợp, nên thấy rằng các nhận xét trên cũng có thể được diễn đạt bằng cách nói rằng ánh xạ chính tắc v \mapsto (v \circ f_i) là một song ánh

d_F : \mathrm{Hom}_{A\text{-đại số.}}(\lim \to E_i, F) \to \lim \leftarrow \mathrm{Hom}_{A\text{-đại số.}}(E_i, F).

Hơn nữa, với mọi đồng cấu đại số trên A w : F \to F', các

\bar{w}_i = \mathrm{Hom}(1_{E_i}, w) : \mathrm{Hom}_{A\text{-đại số.}}(E_i, F) \to \mathrm{Hom}_{A\text{-đại số.}}(E_i, F')

tạo thành một hệ ngược các ánh xạ và biểu đồ

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-đại số.}}(\lim \to E_i, F) & \xrightarrow{d_F} & \lim \mathrm{Hom}_{A\text{-đại số.}}(E_i, F) \\
\downarrow \mathrm{Hom}(1_E, w) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-đại số.}}(\lim \to E_i, F') & \xrightarrow{d_{F'}} & \lim \mathrm{Hom}_{A\text{-đại số.}}(E_i, F')
\end{array}
$$

là giao hoán.

### 7. CƠ SỞ CỦA MỘT ĐẠI SỐ. BẢNG PHÉP NHÂN

Theo định nghĩa, một cơ sở của một A-đại số E là một cơ sở của E đối với cấu trúc A-môđun của nó. Cho (a_i)_{i \in I} là một cơ sở của E; tồn tại duy nhất một họ (\gamma^k_{ij})_{(i, j, k) \in I \times I \times I} các phần tử của vành A sao cho với mọi cặp có thứ tự (i, j) \in I \times I, tập hợp các k \in I sao cho \gamma^j_{ij} \neq 0 là hữu hạn và

$$
a_i a_j = \sum_{k \in I} \gamma^k_{ij} a_k.
$$

Các $\gamma_{ij}^k$ được gọi là *các hằng số cấu trúc* của đại số E đối với cơ sở $(a_i)$ và các hệ thức (7) tạo thành *bảng phép nhân* của đại số E (đối với cơ sở $(a_i)$).

Các hệ thức (7) có thể hình dung được viết ra bằng cách xếp các vế phải của các hệ thức này trong một bảng vuông

$$
\begin{array}{c|c|c}
 & \cdots & a_j & \cdots \\
\hline
 & & & \\
\vdots & & & \\
\hline
a_j & & \sum_k \gamma_{ij}^k a_k & \\
\vdots & & & \\
\end{array}
$$

với quy ước rằng phần tử xuất hiện ở hàng có chỉ số i và cột có chỉ số j bằng tích $a_i a_j$.

Ngược lại, cho một *A-môđun* E, một cơ sở $(a_i)_{i \in I}$ của E và một họ $(\gamma_{ij}^k)$ các phần tử của A sao cho với mọi cặp có thứ tự $(i, j) \in I \times I$, tập hợp $k \in I$ sao cho $\gamma_{ij}^k \neq 0$ là hữu hạn, thì trên E tồn tại duy nhất một cấu trúc đại số trên A sao cho các hệ thức (7) được thỏa mãn, vì A-môđun $E \otimes_A E$ là tự do và nhận $(a_i \otimes a_j)_{(i, j) \in I \times I}$ làm cơ sở (xem II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7).

Cho E là một đại số trên A và $(a_i)_{i \in I}$ là một hệ sinh của A-môđun E (chẳng hạn một cơ sở). Để E là *kết hợp*, điều kiện cần và đủ là các $a_i$ thỏa mãn *các hệ thức kết hợp*

$$(8)$$
$$(a_i a_j) a_k = a_i (a_j a_k) \quad \text{với mọi } i, j, k$$

Ánh xạ $(x, y, z) \mapsto (xy)z - x(yz)$ là một ánh xạ A-trilinear
$$
E \times E \times E \to E
$$
và do đó xác định một ánh xạ A-tuyến tính $E \otimes_A E \otimes_A E \to E$; nếu ánh xạ sau bằng không đối với mọi phần tử $a_i \otimes a_j \otimes a_k$, vốn tạo thành một hệ sinh của A-môđun $E \otimes_A E \otimes_A E$, thì nó đồng nhất bằng không.

Tương tự, để E là *giao hoán*, điều kiện cần và đủ là các $a_i$ thỏa mãn *các hệ thức giao hoán*

$$(9)$$
$$a_i a_j = a_j a_i \quad \text{với mọi } i, j.$$

Chứng minh là tương tự, lần này xét ánh xạ A-song tuyến tính $(x, y) \mapsto xy - yx$. Cuối cùng, để một phần tử $e \in E$ là một phần tử đơn vị, điều kiện cần và đủ là các $a_i$ thỏa mãn các hệ thức

$$(10)$$
$$a_i = e a_i = a_i e \quad \text{với mọi } i,$$

như thấy được lần này bằng cách xét các ánh xạ A-tuyến tính $x \mapsto x - xe$ và $x \mapsto x - ex$.

Khi $(a_i)_{i \in I}$ là một cơ sở của E và $(\gamma_{ij}^k)$ là họ các hằng số cấu trúc tương ứng, các hệ thức (8) tương đương với các hệ thức

$$
\sum_r \gamma_{ij}^r \gamma_{rk}^s = \sum_r \gamma_{ir}^s \gamma_{jk}^r
$$

với mọi $i, j, k, s$. Tương tự, các hệ thức (9) tương đương với $\gamma_{ij}^k = \gamma_{ji}^k$ với mọi $i, j, k$.

Cho $(a_i)_{i \in I}$ là một cơ sở của đại số trên A E; nếu $\rho : A \to B$ là một đồng cấu vành, $(a_i \otimes 1)$ là một cơ sở của đại số trên B $\rho^*(E) = E \otimes_A B$ (II, § 5, no. 1, Mệnh đề 4). Nếu $(\gamma_{ij}^k)$ là họ các hằng số cấu trúc tương ứng với cơ sở $(a_i)$, thì họ $(\rho(\gamma_{ij}^k))$ là họ các hằng số cấu trúc của $\rho^*(E)$ tương ứng với cơ sở $(a_i \otimes 1)$.

### Bài tập {#alg-iii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
