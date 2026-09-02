---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 1
section_title: Modules
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 191-227, 380-386
pdf_pages: 0215-0251, 0404-0410
extraction: ocr
subsections:
    - "no": 1
      title: MODULES; VECTOR SPACES; LINEAR COMBINATIONS
      page: 191
      pdf_page: 215
    - "no": 2
      title: LINEAR MAPPINGS
      page: 194
      pdf_page: 218
    - "no": 3
      title: SUBMODULES; QUOTIENT MODULES
      page: 196
      pdf_page: 220
    - "no": 4
      title: EXACT SEQUENCES
      page: 197
      pdf_page: 221
    - "no": 5
      title: PRODUCTS OF MODULES
      page: 200
      pdf_page: 224
    - "no": 6
      title: DIRECT SUM OF MODULES
      page: 202
      pdf_page: 226
    - "no": 7
      title: INTERSECTION AND SUM OF SUBMODULES
      page: 205
      pdf_page: 229
    - "no": 8
      title: DIRECT SUMS OF SUBMODULES
      page: 208
      pdf_page: 232
    - "no": 9
      title: SUPPLEMENTARY SUBMODULES
      page: 210
      pdf_page: 234
    - "no": 10
      title: MODULES OF FINITE LENGTH
      page: 212
      pdf_page: 236
    - "no": 11
      title: FREE FAMILIES. BASES
      page: 214
      pdf_page: 238
    - "no": 12
      title: ANNIHILATORS. FAITHFUL MODULES. MONOGENOUS MODULES
      page: 219
      pdf_page: 243
    - "no": 13
      title: CHANGE OF RING OF SCALARS
      page: 221
      pdf_page: 245
    - "no": 14
      title: MULTIMODULES
      page: 224
      pdf_page: 248
statements: 88
exercises: 27
content_sha256: b2127d9d7696cc4553facf48c05c3a344641d32141b928829499a77a96b6234c
translated_from: content/en/alg/II/01_s1_modules.md
source_content_sha256: 7397d09a718f6180624ef63d3ea605fc93db2eb8eb18c2019f1e6cb60606e9b8
translation_model: gpt-5.4, gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-f605a7aa
glossary_version: 34
glossary_terms_sha256: 12a0f1b66c6a3a09a817ff91c5814b99fe351fa0c1b33dc15a04e1210744f404
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. MÔĐUN

### 1. MÔĐUN; KHÔNG GIAN VECTƠ; TỔ HỢP TUYẾN TÍNH

#### Định nghĩa 1 {#alg-ii-s1-def-1 .statement}

*Cho một vành* $\mathbf{A}$, *một môđun trái trên* $\mathbf{A}$ (*hay* $\mathbf{A}$-*môđun trái*) *là một tập hợp* $\mathbf{E}$ *được trang bị một cấu trúc đại số xác định bởi việc cho*:

(1) *một luật nhóm giao hoán trên* $\mathbf{E}$ (*trong phần sau sẽ viết theo lối cộng tính*);

(2) *một luật tác động* $(\alpha, x) \mapsto \alpha \top x$, *mà tập hợp các toán tử là vành* $\mathbf{A}$ *và thỏa mãn các tiên đề sau*:

$$
\begin{align*}
(\mathbf{M_I})\quad & \alpha \top (x + y) = (\alpha \top x) + (\alpha \top y) \text{ với mọi } \alpha \in \mathbf{A}, x \in \mathbf{E}, y \in \mathbf{E}; \\
(\mathbf{M_{II}})\quad & (\alpha + \beta) \top x = (\alpha \top x) + (\beta \top x) \text{ với mọi } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{III}})\quad & \alpha \top (\beta \top x) = (\alpha \beta) \top x \text{ với mọi } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{IV}})\quad & 1 \top x = x \text{ với mọi } x \in \mathbf{E}.
\end{align*}
$$

Tiên đề $(\mathbf{M_I})$ có nghĩa là phép toán ngoài của một $\mathbf{A}$-môđun trái $\mathbf{E}$ là *phân phối* đối với phép cộng trên $\mathbf{E}$; do đó một môđun là một nhóm giao hoán có toán tử.

Nếu trong Định nghĩa 1, tiên đề $(\mathbf{M_{III}})$ được thay bằng

$$
(\mathbf{M'_{III}})\quad \alpha \top (\beta \top x) = (\beta \alpha) \top x \text{ với mọi } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E},
$$

thì E với cấu trúc đại số được xác định như vậy là một môđun phải trên A hay một A-môđun phải.

Khi nói về các A-môđun (trái hay phải), các phần tử của vành A thường được gọi là các vô hướng.

Thông thường phép toán ngoài hợp thành của một A-môđun trái (tương ứng, A-môđun phải) được viết theo lối nhân, với toán tử được viết ở bên trái (tương ứng, bên phải); khi đó điều kiện (M_{III}) được viết $\alpha(\beta x) = (\alpha\beta)x$, điều kiện (M'_{III}) được viết $(x\beta)\alpha = x(\beta\alpha)$.

Nếu $A^0$ ký hiệu vành đối của A (I, § 8, no. 3), thì mọi môđun phải E trên vành A là một môđun trái trên vành $A^0$. Do đó có thể trình bày các tính chất của môđun bằng cách giới hạn một cách có hệ thống sự chú ý hoặc vào các môđun trái hoặc vào các môđun phải; trong §§ 1 và 2 nói chung chúng tôi sẽ trình bày như vậy đối với các môđun trái, và khi nói đến một môđun (không nói rõ kiểu nào) chúng tôi sẽ hiểu đó là một môđun trái mà phép toán ngoài sẽ được viết theo lối nhân. Khi vành A là giao hoán thì các khái niệm môđun phải và môđun trái đối với A là đồng nhất.

Với mọi $\alpha \in A$, ánh xạ $x \mapsto \alpha x$ của một A-môđun E vào chính nó được gọi là phép vị tự tỉ số $\alpha$ của E (I, § 4, no. 2); theo (M_I) một phép vị tự là một tự đồng cấu của cấu trúc nhóm giao hoán (không có toán tử) trên E, nhưng nói chung không phải của cấu trúc môđun trên E (I, § 4, no. 2; cf. II, § 1, no. 2 and no. 13). Do đó $\alpha 0 = 0$ và $\alpha(-x) = -(\alpha x)$; nếu $\alpha$ là một phần tử khả nghịch của A, thì phép vị tự $x \mapsto \alpha x$ là một tự đẳng cấu của cấu trúc nhóm giao hoán (không có toán tử) trên E, vì quan hệ $y = \alpha x$ kéo theo, theo (M_IV), $x = \alpha^{-1}(\alpha x) = \alpha^{-1}y$.

Tương tự, theo (M_{II}), với mọi $x \in E$, ánh xạ $\alpha \mapsto \alpha x$ là một đồng cấu từ nhóm cộng A vào nhóm giao hoán (không có toán tử) E; do đó $0x = 0$ và $(-\alpha)x = -(\alpha x)$; hơn nữa, theo (M_IV), với mọi số nguyên $n \in \mathbf{Z}$, $n.x = (n.1)x$.

Khi vành A chỉ gồm phần tử 0, mọi A-môđun E cũng chỉ gồm phần tử 0, vì khi đó $1 = 0$ trong A, do đó, với mọi $x \in E$,
$x = 1.x = 0.x = 0$.

#### Ví dụ {#alg-ii-s1-n1-exa-1 .statement}

(1) Cho $\phi$ là một đồng cấu của một vành A vào một vành B; ánh xạ $(a, x) \mapsto \phi(a)x$ (tương ứng, $(a, x) \mapsto x\phi(a)$) từ $A \times B$ vào B xác định trên B một cấu trúc A-môđun trái (tương ứng, phải). Đặc biệt nếu lấy $\phi$ là ánh xạ đồng nhất trên A, ta thu được trên A một cấu trúc A-môđun trái (tương ứng, phải) chính tắc; để tránh nhầm lẫn, tập hợp A với cấu trúc này được ký hiệu bởi $A_s$ (tương ứng, $A_d$).

(2) Trên một nhóm giao hoán G (viết theo lối cộng tính), cấu trúc nhóm có toán tử được xác định bởi phép toán ngoài $(n, x) \mapsto n.x$ (I, § 3, no. 1) là một cấu trúc môđun trên vành $\mathbf{Z}$ các số nguyên.

(3) Cho E là một nhóm giao hoán viết theo lối cộng tính, $\mathcal{E}$ là vành các tự đồng cấu của E (I, § 8, no. 3: nhắc lại rằng tích $fg$ của hai tự đồng cấu theo định nghĩa là tự đồng cấu hợp thành $f \circ g$). Phép toán ngoài $(f, x) \mapsto f(x)$ giữa các toán tử $f \in \mathscr{E}$ và các phần tử $x \in E$ xác định trên E một cấu trúc $\mathscr{E}$-môđun trái chính tắc.

Bây giờ xét một vành A và giả sử trên E đã cho một cấu trúc A-môđun trái (resp. phải); với mọi $\alpha \in A$, phép vị tự $h_\alpha : x \mapsto \alpha x$ (resp. $x \mapsto x\alpha$) thuộc $\mathscr{E}$; ánh xạ $\phi : \alpha \mapsto h_\alpha$ là một đồng cấu của vành A (resp. vành đối $A^0$) vào vành $\mathscr{E}$ và theo định nghĩa $\alpha x = (\phi(\alpha))(x)$ (resp. $x\alpha = (\phi(\alpha))(x)$). Ngược lại, việc cho một đồng cấu vành $\phi : A \to \mathscr{E}$ (resp. $\phi : A^0 \to \mathscr{E}$) xác định một cấu trúc A-môđun trái (resp. phải) trên E theo các công thức trên. Nói cách khác, việc cho một cấu trúc A-môđun trái (resp. phải) trên một nhóm cộng E với luật cộng là luật nhóm đã cho tương đương với việc cho một đồng cấu vành $A \to \mathscr{E}$ (resp. $A^0 \to \mathscr{E}$).

#### Định nghĩa 2 {#alg-ii-s1-def-2 .statement}

*Một không gian vectơ trái (resp. phải) trên một trường K là một K-môđun trái (resp. phải).*

Các phần tử của một không gian vectơ đôi khi được gọi là *vectơ*.

#### Ví dụ {#alg-ii-s1-n1-exa-2 .statement}

(4) Một trường vừa là một không gian vectơ trái vừa là một không gian vectơ phải đối với bất kỳ trường con nào của nó.

*(5)* Không gian số thực ba chiều $\mathbf{R}^3$ là một không gian vectơ đối với trường số thực $\mathbf{R}$, tích $tx$ của một số thực $t$ và một điểm $x$ có tọa độ $x_1, x_2, x_3$ là điểm có tọa độ $tx_1, tx_2, tx_3$. Tương tự, tập hợp các hàm nhận giá trị thực xác định trên một tập hợp tùy ý F là một không gian vectơ đối với $\mathbf{R}$, tích $tf$ của một số thực $t$ và một hàm $f$ là hàm nhận giá trị thực $x \mapsto tf(x)$.*

Đối với hai họ $(x_i)_{i \in I}, (y_i)_{i \in I}$ các phần tử của một A-môđun E có giá hữu hạn (I, § 2, no. 1), các phương trình sau đúng:

(1)
$$
\sum_{i \in I} (x_i + y_i) = \sum_{i \in I} x_i + \sum_{i \in I} y_i
$$

(2)
$$
\alpha \cdot \sum_{i \in I} x_i = \sum_{i \in I} (\alpha x_i) \quad \text{với mọi } \alpha \in A;
$$
các phương trình trên ngay lập tức được quy về các phương trình tương tự đối với các tổng hữu hạn bằng cách xét một tập con hữu hạn H của I chứa các giá của $(x_i)$ và $(y_i)$.

#### Định nghĩa 3 {#alg-ii-s1-def-3 .statement}

*Một phần tử x của một A-môđun E được gọi là một tổ hợp tuyến tính với các hệ số trong A của một họ $(a_i)_{i \in I}$ các phần tử của E nếu tồn tại một họ $(\lambda_i)_{i \in I}$ các phần tử của A, có giá hữu hạn, sao cho $x = \sum_{i \in I} \lambda_i a_i$.*

Nói chung có nhiều họ phân biệt $(\lambda_i)$ thỏa mãn điều kiện này (cf. no. 11).

Chú ý rằng 0 là tổ hợp tuyến tính duy nhất của họ rỗng các phần tử của E (theo quy ước của I, § 2, no. 1).

### 2. ÁNH XẠ TUYẾN TÍNH

#### Định nghĩa 4 {#alg-ii-s1-def-4 .statement}

Cho E và F là hai môđun trái đối với cùng một vành A. Một ánh xạ tuyến tính (hay ánh xạ A-tuyến tính, hay đồng cấu, hay A-đồng cấu) từ E vào F là một ánh xạ u : E → F sao cho:

(3) $u(x + y) = u(x) + u(y)$ với $x \in E, y \in E;$

(4G) $u(\lambda . x) = \lambda . u(x)$ với $\lambda \in A, x \in E.$

Nếu E và F là hai A-môđun phải, một ánh xạ tuyến tính $u : E \to F$ là một ánh xạ thỏa mãn (3) và

(4D) $u(x . \lambda) = u(x) . \lambda$ với $\lambda \in A, x \in E.$

#### Nhận xét {#alg-ii-s1-n2-rem-1 .statement}

Khi E và F là hai nhóm giao hoán được xem như các môđun trên vành $\mathbf{Z}$ (no. 1), mọi đồng cấu $u$ của nhóm E (không có toán tử) vào nhóm F (không có toán tử) cũng là một ánh xạ tuyến tính từ E vào F, vì với n là một số nguyên > 0, quan hệ $u(n . x) = n . u(x)$ suy ra từ $u(x + y) = u(x) + u(y)$ bằng quy nạp theo n và với $n = -m < 0$,
$$
u(n . x) = u(-(m . x)) = -u(m . x) = -(m . u(x)) = n . u(x).
$$

#### Ví dụ {#alg-ii-s1-n2-exa-1 .statement}

(1) Cho E là một A-môđun và a là một phần tử của E; ánh xạ $\lambda \mapsto \lambda a$ từ A-môđun $A_s$ vào E là một ánh xạ tuyến tính $\theta_a$ sao cho $\theta_a(1) = a.$
*(2) Cho I là một khoảng mở của đường thẳng thực $\mathbf{R}$, E là không gian vectơ các hàm nhận giá trị thực khả vi trên I và F là không gian vectơ của tất cả các hàm nhận giá trị thực xác định trên I. Ánh xạ $x \mapsto x'$ gán cho mỗi hàm khả vi x đạo hàm của nó là một ánh xạ tuyến tính từ E vào F.*

Chú ý rằng một phép vị tự $x \mapsto \alpha x$ trên một A-môđun E không nhất thiết là một ánh xạ tuyến tính: nói cách khác, quan hệ $\alpha(\lambda x) = \lambda(\alpha x)$ không nhất thiết đúng với mọi $\lambda \in A$ và $x \in E$. Tuy nhiên, quan hệ này đúng khi $\alpha$ thuộc tâm của A; khi đó $x \mapsto \alpha x$ được gọi là một phép vị tự trung tâm (cf. no. 13).

Nếu $u : E \to F$ là một ánh xạ tuyến tính, thì, với mọi họ $(x_i)_{i \in I}$ các phần tử của E và mọi họ $(\lambda_i)_{i \in I}$ các phần tử của A sao cho giá của họ $(\lambda_i x_i)_{i \in I}$ là hữu hạn,

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i)
$$

suy ra ngay lập tức từ (3) và (4G) bằng quy nạp theo lực lượng của giá của họ $(\lambda_i x_i)$.

#### Mệnh đề 1 {#alg-ii-s1-prop-1 .statement}

Cho E, F, G là ba A-môđun, u là một ánh xạ tuyến tính từ E vào F và v là một ánh xạ tuyến tính từ F vào G. Khi đó ánh xạ hợp thành $v \circ u$ là tuyến tính.

(1) *Nếu u:E → F và v:F → E là hai ánh xạ tuyến tính sao cho v ∘ u là ánh xạ đồng nhất trên E và u ∘ v là ánh xạ đồng nhất trên F, thì u là một đẳng cấu của E lên F và v là đẳng cấu nghịch đảo.*

(2) *Mọi ánh xạ tuyến tính song ánh u:E → F là một đẳng cấu của E lên F.*

Các mệnh đề này suy ra ngay lập tức từ Định nghĩa 4.

Các Mệnh đề 1 và 2 chỉ ra rằng các ánh xạ tuyến tính có thể được lấy làm các *phép biến hình* cho loài các cấu trúc A-môđun (*Lý thuyết tập hợp*, IV, § 2, no. 1); từ nay về sau ta luôn giả sử rằng lựa chọn các phép biến hình này đã được thực hiện.

Cho hai A-môđun trái (tương ứng phải) E và F, ký hiệu Hom(E, F) hoặc Hom_A(E, F) là tập hợp các ánh xạ tuyến tính từ E vào F.

Tập hợp Hom(E, F) là một *vành giao hoán*, một nhóm con của nhóm giao hoán tích F^E của tất cả các ánh xạ từ E vào F (I, § 4, no. 8); nhắc lại rằng với hai phần tử u, v của F^E và mọi x ∈ E,

$$(u + v)(x) = u(x) + v(x), \quad (-u)(x) = -u(x)$$

do đó suy ra ngay lập tức rằng, nếu u và v tuyến tính, thì u + v và −u cũng tuyến tính. Nếu G là một A-môđun trái (tương ứng phải) thứ ba, f, f_1, f_2 là các phần tử của Hom(E, F) và g, g_1, g_2 là các phần tử của Hom(F, G), thì các hệ thức sau được kiểm chứng ngay lập tức:

(6) $$g \circ (f_1 + f_2) = g \circ f_1 + g \circ f_2$$
(7) $$(g_1 + g_2) \circ f = g_1 \circ f + g_2 \circ f$$
(8) $$g \circ (-f) = (-g) \circ f = -(g \circ f).$$

Đặc biệt, luật hợp thành (f, g) ↦ f ∘ g trên Hom(E, E) xác định cùng với cấu trúc nhóm cộng tính ở trên một cấu trúc *vành* trên Hom(E, E), mà phần tử đơn vị của nó, ký hiệu là 1_E hoặc Id_E, là ánh xạ đồng nhất trên E; các ánh xạ tuyến tính từ E vào chính nó còn được gọi là các *tự đồng cấu* của A-môđun E và vành Hom(E, E) cũng được ký hiệu bởi End(E) hoặc End_A(E). Các *tự đẳng cấu* của A-môđun E chính là các phần tử *khả nghịch* của End(E) (Mệnh đề 2); chúng tạo thành một *nhóm* nhân, ký hiệu bởi Aut(E) hoặc GL(E), còn được gọi là *nhóm tuyến tính* đối với E.

Từ (6) và (7) suy ra rằng, với hai A-môđun E, F, Hom(E, F) có cấu trúc chính tắc của một *môđun trái* trên vành Hom(F, F) và của một *môđun phải* trên Hom(E, E).

Cho E, F, E', F' là bốn A-môđun (trái), u:E' → E và v:F → F' là các ánh xạ A-tuyến tính. Nếu mỗi phần tử f ∈ Hom(E, F) được liên kết với phần tử v ∘ f ∘ u ∈ Hom(E', F'), thì xác định được một ánh xạ

$$\operatorname{Hom}(E, F) \to \operatorname{Hom}(E', F')$$

là $\mathbf{Z}$-tuyến tính và được ký hiệu bởi $\mathrm{Hom}(u, v)$ hoặc $\mathrm{Hom}_A(u, v)$. Nếu $u, u_1, u_2$ thuộc $\mathrm{Hom}(E', E)$ và $v, v_1, v_2$ thuộc $\mathrm{Hom}(F, F')$, thì

$$
\begin{cases}
\mathrm{Hom}(u_1 + u_2, v) = \mathrm{Hom}(u_1, v) + \mathrm{Hom}(u_2, v) \\
\mathrm{Hom}(u, v_1 + v_2) = \mathrm{Hom}(u, v_1) + \mathrm{Hom}(u, v_2)
\end{cases}
$$

Cho $E'', F''$ là hai $A$-môđun, $u': E'' \to E'$ và $v': F' \to F''$ là các ánh xạ tuyến tính. Khi đó

$$
\mathrm{Hom}(u \circ u', v' \circ v) = \mathrm{Hom}(u', v') \circ \mathrm{Hom}(u, v).
$$

Nếu $u$ là một đẳng cấu của $E'$ lên $E$ và $v$ là một đẳng cấu của $F$ lên $F'$, $\mathrm{Hom}(u, v)$ là một đẳng cấu của $\mathrm{Hom}(E, F)$ lên $\mathrm{Hom}(E', F')$ mà đẳng cấu nghịch đảo là $\mathrm{Hom}(u^{-1}, v^{-1})$ theo (10).

Nếu $h$ (tương ứng $k$) là một tự đồng cấu của $E$ (tương ứng $F$), $\mathrm{Hom}(h, 1_F)$ (tương ứng $\mathrm{Hom}(1_E, k)$) chính là phép vị tự với tỷ số $h$ (tương ứng $k$) đối với cấu trúc môđun phải (tương ứng trái) trên vành $\mathrm{End}(E)$ (tương ứng $\mathrm{End}(F)$) được xác định ở trên.

### 3. MÔĐUN CON; CÁC MÔĐUN THƯƠNG

Cho $E$ là một $A$-môđun và $M$ là một tập con của $E$; để cấu trúc $A$-môđun trên $E$ cảm sinh một cấu trúc $A$-môđun trên $M$, điều kiện cần và đủ là $M$ là một nhóm con ổn định của $E$ (I, § 4, no. 3), vì nếu đúng như vậy thì cấu trúc nhóm có toán tử cảm sinh trên $M$ hiển nhiên thỏa mãn các tiên đề ($M_{II}$), ($M_{III}$) và ($M_{IV}$); khi đó $M$ với cấu trúc này (hoặc, do lạm dụng ngôn ngữ, chính tập hợp $M$) được gọi là một môđun con của $E$; đơn ánh chính tắc $M \to E$ là một ánh xạ tuyến tính. Khi $E$ là một không gian vectơ, các môđun con của nó được gọi là các không gian con vectơ (hoặc đơn giản là các không gian con nếu không thể có sự nhầm lẫn).

#### Ví dụ {#alg-ii-s1-n3-exa-1 .statement}

(1) Trong mọi môđun $E$, tập hợp chỉ gồm 0 là một môđun con (môđun con không, thường được ký hiệu bởi 0, do lạm dụng ký hiệu).
(2) Cho $A$ là một vành. Các môđun con của $A_s$ (tương ứng của $A_d$) chính là các iđêan trái (tương ứng iđêan phải) của vành $A$.
(3) Cho $E$ là một $A$-môđun, $x$ là một phần tử của $E$ và $a$ là một iđêan trái của $A$. Tập hợp các phần tử $\alpha x$, trong đó $\alpha$ chạy qua $a$, là một môđun con của $E$, được ký hiệu là $ax$.
(4) Trong một nhóm giao hoán $G$ được xét như một $\mathbf{Z}$-môđun (no. 1), mọi nhóm con của $G$ cũng là một môđun con.

*(5) Cho $I$ là một khoảng mở của đường thẳng thực $\mathbf{R}$; tập $C$ các hàm nhận giá trị thực được xác định và liên tục trên $I$ là một không gian con vectơ của không gian vectơ $\mathbf{R}^I$ gồm mọi hàm nhận giá trị thực được xác định trên $I$. Tương tự, tập $D$ các hàm khả vi trên $I$ là một không gian con vectơ của $C_*$*

Cho $E$ là một $A$-môđun. Mọi quan hệ tương đương tương thích (I, § 1, no. 6) với cấu trúc môđun trên $E$ đều có dạng $x - y \in M$, trong đó $M$ là một nhóm con ổn định của E (I, § 4, no. 4), tức là một môđun con của E. Ngay lập tức kiểm tra được rằng cấu trúc nhóm có toán tử trên nhóm thương E/M (I, § 4, no. 4) là một cấu trúc A-môđun, mà đối với cấu trúc ấy ánh xạ chính tắc $E \to E/M$ là tuyến tính; với cấu trúc này, E/M được gọi là *môđun thương* của E theo môđun con M. Một môđun thương của một không gian vectơ E được gọi là một *không gian vectơ thương* (hoặc đơn giản là một *không gian thương*) của E.

*Ví dụ* (6). Mọi iđêan trái $a$ trong một vành A xác định một môđun thương $A_s/a$ của A-môđun trái $A_s$; do lạm dụng ký hiệu, môđun thương này thường được ký hiệu là $A/a$.

Cho E, F là hai A-môđun. Hệ quả từ các tính chất tổng quát của các nhóm có toán tử (I, § 4, no. 5) (hoặc trực tiếp từ các định nghĩa) là nếu $u : E \to F$ là một ánh xạ tuyến tính, thì ảnh qua $u$ của mọi môđun con của E là một môđun con của F và ảnh ngược qua $u$ của mọi môđun con của F là một môđun con của E. Đặc biệt, *hạt nhân* $N = \overline{u}^{-1}(0)$ là một môđun con của E và ảnh $u(E)$ của E qua $u$ là một môđun con của F (I, § 4, no. 6, Mệnh đề 7); do một sự lạm dụng ngôn ngữ, $u(E)$ được gọi là *ảnh của u*. Môđun thương $E/N$ cũng được gọi là *đối ảnh* của $u$ và môđun thương $F/u(E)$ là *đối hạt nhân* của $u$. Trong *phân tích chính tắc* của $u$ (I, § 4, no. 5)

$$
u : E \xrightarrow{p} E/N \xrightarrow{v} u(E) \xrightarrow{i} F
$$

$v$ là một *đẳng cấu* từ đối ảnh của $u$ lên ảnh của $u$ (no. 2, Mệnh đề 2). Để $u$ là *đơn ánh*, điều kiện cần và đủ là hạt nhân của nó bằng không; để $u$ là *toàn ánh*, điều kiện cần và đủ là đối hạt nhân của nó bằng không.

Hạt nhân, ảnh, đối ảnh và đối hạt nhân của $u$ lần lượt được ký hiệu bởi Ker $u$, Im $u$, Coim $u$, Coker $u$.

#### Nhận xét {#alg-ii-s1-n3-rem-1 .statement}

Cho M là một môđun con của một A-môđun E và $\phi : E \to E/M$ là đồng cấu chính tắc. Để một ánh xạ A-tuyến tính $u : E \to F$ có dạng $v \circ \phi$, trong đó $v$ là một ánh xạ tuyến tính từ E/M vào F, điều kiện cần và đủ là $M \subset \mathrm{Ker}(u)$; thật vậy, nếu điều kiện này được thỏa mãn, quan hệ $x - y \in M$ kéo theo $u(x) = u(y)$, do đó $u$ tương thích với quan hệ tương đương này và rõ ràng ánh xạ $v : E/M \to F$ dẫn xuất từ $u$ bằng cách lấy thương là tuyến tính.

### 4. DÃY KHỚP

#### Định nghĩa 5 {#alg-ii-s1-def-5 .statement}

*Cho F, G, H là ba A-môđun; cho f là một đồng cấu từ F vào G và g là một đồng cấu từ G vào H. Cặp có thứ tự (f, g) được gọi là một dãy khớp nếu*

$$
g^{-1}(0) = f(F)
$$

*nói cách khác, nếu hạt nhân của g bằng ảnh của f.*

Biểu đồ

(12)
$$
F \xrightarrow{f} G \xrightarrow{g} H
$$
cũng được gọi là một *dãy khớp*.

Ta cũng xét tương tự một biểu đồ gồm bốn A-môđun và ba đồng cấu:

(13)
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

Biểu đồ này được gọi là *khớp tại* F nếu biểu đồ $E \xrightarrow{f} F \xrightarrow{g} G$ là khớp; nó được gọi là *khớp tại* G nếu $F \xrightarrow{g} G \xrightarrow{h} H$ là khớp. Nếu biểu đồ (13) *khớp tại* F *và tại* G, thì nó được gọi đơn giản là *khớp*, hoặc là một *dãy khớp*. Các dãy khớp có một số hạng tùy ý được định nghĩa tương tự.

#### Nhận xét {#alg-ii-s1-n4-rem-1 .statement}

(1) Nếu cặp có thứ tự $(f, g)$ là một dãy khớp, thì $g \circ f = 0$; nhưng dĩ nhiên tính chất này không đặc trưng các dãy khớp, vì nó chỉ có nghĩa là ảnh của $f$ *được chứa* trong hạt nhân của $g$.

Trong các mệnh đề dưới đây, E, F, G ký hiệu các A-môđun, 0 là A-môđun thu về phần tử đơn vị của nó; các mũi tên biểu thị các đồng cấu A-môđun. Vì chỉ có một đồng cấu duy nhất từ môđun 0 đến một môđun E (tương ứng từ E đến 0), nên không cần đặt tên cho các đồng cấu này trong các dãy khớp nơi chúng xuất hiện.

#### Mệnh đề 3 {#alg-ii-s1-prop-3 .statement}

(a) *Để*
$$
0 \longrightarrow E \xrightarrow{f} F
$$
*là một dãy khớp, điều kiện cần và đủ là* $f$ *đơn ánh*.

(b) *Để*
$$
E \xrightarrow{f} F \longrightarrow 0
$$
*là một dãy khớp, điều kiện cần và đủ là* $f$ *toàn ánh*.

(c) *Để*
$$
0 \longrightarrow E \xrightarrow{f} F \longrightarrow 0
$$
*là một dãy khớp, điều kiện cần và đủ là* $f$ *song ánh* (nói cách khác (no. 2, Mệnh đề 2) là $f$ là một *đẳng cấu* từ E lên F).

(d) *Nếu* F *là một môđun con của* E *và* $i : F \to E$ *là đơn ánh chính tắc,* $p : E \to E/F$ *là đồng cấu chính tắc, thì biểu đồ*
(14)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0
$$
*là một dãy khớp.*

(e) *Nếu $f : E \to F$ là một đồng cấu, thì biểu đồ*

$$
0 \longrightarrow f^{-1}(0) \overset{i}{\longrightarrow} E \overset{f}{\longrightarrow} F \overset{p}{\longrightarrow} F/f(E) \to 0
$$

*(trong đó $i$ là đơn ánh chính tắc và $p$ là toàn cấu chính tắc) là một dãy khớp.*

Mệnh đề được suy ra ngay lập tức từ các định nghĩa và Mệnh đề 2 của no. 2.

#### Nhận xét {#alg-ii-s1-n4-rem-2 .statement}

(2) Nói rằng có một dãy khớp

$$
0 \longrightarrow E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \longrightarrow 0
$$

có nghĩa là $f$ là đơn ánh, $g$ toàn ánh và song ánh chính tắc liên kết với $g$ là một *đẳng cấu* từ $F/f(E)$ lên $G$. Người ta cũng nói rằng bộ ba $(F, f, g)$ là một *mở rộng của môđun G bởi môđun E* (I, § 6, no. 7).

(3) Nếu có một dãy khớp gồm 4 hạng

$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \overset{h}{\longrightarrow} H
$$

thì đối hạt nhân của $f$ là $F/f(E) = F/g^{-1}(0)$ và hạt nhân của $h$ là $g(F)$; do đó song ánh chính tắc liên kết với $g$ là một *đẳng cấu*

$$
\operatorname{Coker} f \to \operatorname{Ker} h.
$$

(4) Xét một cặp có thứ tự các đồng cấu A-môđun

$$(15)$$
$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G.
$$

Để biểu đồ (15) là một dãy khớp, điều kiện cần và đủ là tồn tại hai A-môđun S, T và các đồng cấu $a : E \to S,\ b : S \to F,\ c : F \to T,\ d : T \to G$ sao cho ba dãy

$$(16)$$
$$
\begin{cases}
E \overset{a}{\longrightarrow} S \longrightarrow 0 \\
0 \longrightarrow S \overset{b}{\longrightarrow} F \overset{c}{\longrightarrow} T \longrightarrow 0 \\
0 \longrightarrow T \overset{d}{\longrightarrow} G
\end{cases}
$$

là *khớp* và $f = b \circ a$ và $g = d \circ c$.

Nếu (15) là một dãy khớp, thì lấy $S = f(E) = g^{-1}(0)$ và $T = g(F)$, trong đó $b$ và $d$ là các đơn ánh chính tắc còn $a$ (tương ứng $c$) là đồng cấu có cùng đồ thị với $f$ (tương ứng $g$). Ngược lại, nếu S, T, a, b, c, d thỏa mãn các điều kiện trên, thì $f(E) = b(a(E)) = b(S)$ và $g^{-1}(0) = c(d(0)) = c(0)$, do đó tính khớp của (16) cho thấy rằng $f(E) = g^{-1}(0)$.

Việc dùng các chữ cái tường minh để chỉ các đồng cấu trong một dãy khớp thường được bỏ qua khi điều đó không cần thiết cho các lập luận.

#### Nhận xét {#alg-ii-s1-n4-rem-3 .statement}

(5) Định nghĩa về dãy khớp mở rộng ngay lập tức cho các nhóm không nhất thiết giao hoán; trong trường hợp này dĩ nhiên dùng ký hiệu nhân với 0 được thay bởi 1 trong các công thức (nếu không gây nhầm lẫn). Các phần (a), (b), (c) của Mệnh đề 3 vẫn còn đúng, và cả (d) nữa khi F là một nhóm con chuẩn tắc của E. Nhận xét 2 và Mệnh đề 3(e) đúng với điều kiện $f(E)$ là một nhóm con chuẩn tắc của F; các Nhận xét 3 và 4 đúng không cần sửa đổi.

### 5. TÍCH CỦA CÁC MÔĐUN

Cho $(E_i)_{i \in I}$ là một họ các môđun trên cùng một vành A. Người ta kiểm tra ngay lập tức rằng tích của các cấu trúc môđun trên các $E_i$ ($I, § 4,$ no. 8) là một cấu trúc A-môđun trên tập hợp tích $E = \prod_{i \in I} E_i$. Với cấu trúc này, tập hợp E được gọi là môđun tích của các môđun $E_i$; nếu $x = (x_i), y = (y_i)$ là hai phần tử của E, thì

$$
\begin{cases}
x + y = (x_i + y_i) \\
\lambda \cdot x = (\lambda x_i)
\end{cases}
$$
với mọi $\lambda \in A$.

Các công thức (17) biểu thị sự kiện rằng các phép chiếu $pr_i : E \to E_i$ là các ánh xạ tuyến tính; các ánh xạ này hiển nhiên là toàn ánh.

Nhắc lại rằng nếu tập hợp chỉ số I là rỗng, thì tập hợp tích $\prod_{i \in I} E_i$ khi đó chỉ gồm một phần tử; cấu trúc môđun tích trên tập hợp này khi đó là cấu trúc mà trong đó phần tử duy nhất này là 0.

#### Mệnh đề 4 {#alg-ii-s1-prop-4 .statement}

*Cho* $E = \prod_{i \in I} E_i$ *là tích của một họ các A-môđun* $(E_i)_{i \in I}$. *Với mọi A-môđun* F *và mọi họ các ánh xạ tuyến tính* $f_i : F \to E_i$ *tồn tại một và chỉ một ánh xạ* f *từ* F *vào* E *sao cho* $pr_i \circ f = f_i$ *với mọi* $i \in I$ *và ánh xạ này là tuyến tính*.

Điều này suy ra trực tiếp từ các định nghĩa.

Tích của các môđun là "kết hợp": nếu $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của I, thì ánh xạ chính tắc
$$
\prod_{i \in I} E_i \to \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} E_i \right)
$$
là một đẳng cấu.

#### Mệnh đề 5 {#alg-ii-s1-prop-5 .statement}

(i) *Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ A-môđun có cùng tập hợp chỉ số* I; *với mọi họ các ánh xạ tuyến tính* $f_i : E_i \to F_i$ ($i \in I$), *ánh xạ* $f : (x_i) \to (f_i(x_i))$ *từ* $\prod_i E_i$ *vào* $\prod_i F_i$ *(đôi khi được ký hiệu là* $\prod_i f_i$) *là tuyến tính*.

(ii) *Cho* $(G_i)_{i \in I}$ *là một họ thứ ba các A-môđun với* I *làm tập chỉ số và, với mọi* $i \in I,$ cho $g_i : F_i \to G_i$ là một ánh xạ tuyến tính; đặt $g = \prod_i g_i$. Để mỗi dãy* $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ *đều khớp, điều kiện cần và đủ là dãy*

$$
\prod_i E_i \xrightarrow{f} \prod_i F_i \xrightarrow{g} \prod_i G_i
$$

*khớp.*

Mệnh đề (i) suy ra ngay lập tức từ các định nghĩa. Mặt khác, nói rằng $y = (y_i)$ thuộc $\operatorname{Ker}(g)$ có nghĩa là $g_i(y_i) = 0$ với mọi $i \in I$ và do đó $y_i \in \operatorname{Ker}(g_i)$ với mọi $i \in I$; tương tự, nói rằng $y$ thuộc $\operatorname{Im}(f)$ có nghĩa là tồn tại $x = (x_i) \in \prod_i E_i$ sao cho $y = f(x)$, điều này tương đương với việc nói rằng $y_i = f_i(x_i)$ với mọi $i \in I$ hoặc cũng tương đương với $y_i \in \operatorname{Im}(f_i)$ với mọi $i \in I$; do đó có (ii).

#### Hệ quả {#alg-ii-s1-n5-cor-1 .statement}

Trong các điều kiện của Mệnh đề 5, (i),

$$
\operatorname{Ker}(f) = \prod_{i \in I} \operatorname{Ker}(f_i), \qquad \operatorname{Im}(f) = \prod_{i \in I} \operatorname{Im}(f_i)
$$

và có các đẳng cấu chính tắc

$$
\operatorname{Coim}(f) \to \prod_{i \in I} \operatorname{Coim}(f_i), \qquad \operatorname{Coker}(f) = \prod_{i \in I} \operatorname{Coker}(f_i)
$$

thu được bằng cách tương ứng gắn với lớp của một phần tử $x = (x_i)$ của $\prod_i E_i$, theo $\operatorname{Ker}(f)$, (tương ứng với lớp của một phần tử $y = (y_i)$ của $\prod_i F_i$, theo $\operatorname{Im}(f)$) họ các lớp của các $x_i$ theo $\operatorname{Ker}(f_i)$ (tương ứng họ các lớp của các $y_i$ theo $\operatorname{Im}(f)$).

Đặc biệt, để $f$ là đơn ánh (tương ứng, toàn ánh, song ánh, không) thì điều kiện cần và đủ là, với mọi $i \in I$, $f_i$ là đơn ánh (tương ứng, toàn ánh, song ánh, không).

Nếu, với mọi $i \in I$, ta xét một môđun con $F_i$ của $E_i$, thì môđun $\prod_{i \in I} F_i$ là một môđun con của $\prod_{i \in I} E_i$ và theo Hệ quả của Mệnh đề 5, có một đẳng cấu chính tắc

$$
\prod_{i \in I} (E_i/F_i) \to \left( \prod_{i \in I} E_i \right) / \left( \prod_{i \in I} F_i \right).
$$

Một ví dụ quan trọng của tích các môđun là trường hợp mọi môđun nhân tử đều bằng cùng một môđun $F$; khi đó tích của chúng $F^I$ đơn giản chỉ là tập hợp các ánh xạ từ $I$ vào $F$. Ánh xạ đường chéo $F \to F^I$ biến $x \in F$ thành hàm hằng bằng $x$ trên $I$ là tuyến tính. Nếu $(E_i)_{i \in I}$ là một họ các $A$-môđun và, với mọi $i \in I$, $f_i : F \to E_i$ là một ánh xạ tuyến tính, thì ánh xạ tuyến tính $x \mapsto (f_i(x))$ từ $F$ vào $\prod_{i \in I} E_i$ là hợp thành của ánh xạ $(x_i) \mapsto (f_i(x_i))$ từ $F^I$ vào $\prod_{i \in I} E_i$ và ánh xạ đường chéo $F \to F^I$.

### 6. TỔNG TRỰC TIẾP CỦA CÁC MÔĐUN

Cho $(E_i)_{i \in I}$ là một họ các A-môđun và $F = \prod_{i \in I} E_i$ là tích của chúng. Tập hợp $E$ các $x \in F$ sao cho $\mathrm{pr}_i x = 0$ trừ ra với một số hữu hạn chỉ số hiển nhiên là một môđun con của $F$, gọi là tổng trực tiếp ngoài (hay đơn giản là tổng trực tiếp) của họ môđun $(E_i)$ và được ký hiệu bởi $\bigoplus_{i \in I} E_i$ (I, § 4, no. 9). Khi I là hữu hạn thì $\bigoplus_{i \in I} E_i = \prod_{i \in I} E_i$; nếu $I = \{p, q\}$ (khoảng của $\mathbf{Z}$), ta cũng viết

$$
\bigoplus_{i \in I} E_i = E_p \oplus E_{p+1} \oplus \cdots \oplus E_q.
$$

Với mọi $\kappa \in I$, cho $j_\kappa$ là ánh xạ $E_\kappa \to F$ gán cho mỗi $x_\kappa \in E_\kappa$ phần tử của $F$ sao cho $\mathrm{pr}_i(j_\kappa(x_\kappa)) = 0$ với $i \neq \kappa$ và $\mathrm{pr}_\kappa(j_\kappa(x_\kappa)) = x_\kappa$; ngay lập tức thấy rằng $j_\kappa$ là một ánh xạ tuyến tính đơn ánh của $E_\kappa$ vào tổng trực tiếp $E$ của các $E_i$, mà ta sẽ gọi là đơn ánh chính tắc; môđun con $j_\kappa(E_\kappa)$ của $E$, đẳng cấu với $E_\kappa$, được gọi là môđun con thành phần của $E$ có chỉ số $\kappa$. Nó thường được đồng nhất với $E_\kappa$ qua $j_\kappa$.

Với mọi $x \in E = \bigoplus_{i \in I} E_i$, do đó ta có

$$
x = \sum_{i \in I} j_i(\mathrm{pr}_i x).
$$

(20)

#### Mệnh đề 6 {#alg-ii-s1-prop-6 .statement}

*Cho* $(E_i)_{i \in I}$ *là một họ các A-môđun*, $M$ *là một A-môđun và, với mọi* $i \in I$, *cho* $f_i : E_i \to M$ *là một ánh xạ tuyến tính*. *Khi đó tồn tại một và chỉ một ánh xạ tuyến tính* $g : \bigoplus_{i \in I} E_i \to M$ *sao cho, với mọi* $i \in I$:

$$
g \circ j_i = f_i.
$$

(21)

Theo (20), nếu $g$ tồn tại thì tất yếu, với mọi $x \in \bigoplus_{i \in I} E_i$,

$$
g(x) = \sum_i g(j_i(\mathrm{pr}_i(x))) = \sum_i f_i(\mathrm{pr}_i(x)),
$$

do đó có tính duy nhất của $g$. Ngược lại, đặt $g(x) = \sum_i f_i(\mathrm{pr}_i(x))$ với mọi $x \in \bigoplus_{i \in I} E_i$, ta kiểm tra ngay lập tức rằng như vậy đã định nghĩa được một ánh xạ tuyến tính thỏa mãn các điều kiện của mệnh đề.

Khi không thể có sự nhầm lẫn, ta viết $g = \sum_{i \in I} f_i$ (điều này trái với các quy ước của I, § 2, no. 1, khi họ $(f_i)$ không có giá hữu hạn).

Đặc biệt, nếu J là một tập con bất kỳ của I, các đơn ánh chính tắc $j_i$ với $i \in J$ xác định một ánh xạ tuyến tính chính tắc $j_J : \bigoplus_{i \in J} E_i \to \bigoplus_{i \in I} E_i$, ánh xạ này gán cho mỗi $(x_i)_{i \in I}$ phần tử $(x'_i)_{i \in I}$ sao cho $x'_i = x_i$ với $i \in J$, $x'_i = 0$ với $i \notin J$; ánh xạ này hiển nhiên là đơn ánh. Hơn nữa, nếu $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của I, ánh xạ $i : \bigoplus_{\lambda \in L} \left( \bigoplus_{i \in J_\lambda} E_i \right) \to \bigoplus_{i \in I} E_i$ tương ứng với họ $(j_{J_\lambda})$ theo Mệnh đề 6 là một *đẳng cấu* gọi là chính tắc ("tính kết hợp" của các tổng trực tiếp).

#### Hệ quả 1 {#alg-ii-s1-prop-6-cor-1 .statement}

*Cho $(E_i)_{i \in I}, (F_\lambda)_{\lambda \in L}$ là hai họ A-môđun. Ánh xạ*
$$
\text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) \to \prod_{(i, \lambda) \in I \times L} \text{Hom}_A(E_i, F_\lambda)
$$
*ghép với mỗi $g \in \text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right)$ họ $(\operatorname{pr}_\lambda \circ g \circ j_i)$, là một đẳng cấu môđun trên $\mathbf{Z}$ (gọi là chính tắc).*

Điều này suy ra từ Mệnh đề 6 và no. 5, Mệnh đề 4.

#### Hệ quả 2 {#alg-ii-s1-prop-6-cor-2 .statement}

*Cho $(E_i)_{i \in I}$ là một họ A-môđun, F là một A-môđun và, với mỗi $i \in I$, cho $f_i : E_i \to F$ là một ánh xạ tuyến tính. Để $f = \sum_{i \in I} f_i$ là một đẳng cấu từ $E = \bigoplus_{i \in I} E_i$ lên F, điều kiện cần và đủ là với mỗi $i \in I$ tồn tại một ánh xạ tuyến tính $g_i : F \to E_i$ có các tính chất sau:*
(1) $g_i \circ f_i = 1_{E_i}$ với mọi $i \in I$.
(2) $g_i \circ f_\kappa = 0$ nếu $i \neq \kappa$.
(3) *Với mọi $y \in F$, họ $(g_i(y))$ có giá hữu hạn và*
$$
y = \sum_{i \in I} f_i(g_i(y)).
$$
Chú ý rằng nếu I hữu hạn, điều kiện cuối cùng cũng có thể được viết là
$$
\sum_{i \in I} f_i \circ g_i = 1_F.
$$
Hiển nhiên các điều kiện là cần thiết vì chúng được thỏa mãn bởi các $g_i = \operatorname{pr}_i \circ f_i^{-1}$. Ngược lại nếu chúng được thỏa mãn, thì với mọi $y \in F$, $g(y) = \sum_i j_i(g_i(y))$ được xác định và ngay lập tức thấy rằng $g$ là một ánh xạ tuyến tính từ F vào E. Với mọi $y \in F$, ta có $f(g(y)) = \sum_i f_i(g_i(y)) = y$ theo giả thiết. Mặt khác, với mọi $x \in E$, $g_\kappa(f(x)) = g_\kappa \left( \sum_i f_i(\operatorname{pr}_i(x)) \right) = g_\kappa(f_\kappa(\operatorname{pr}_\kappa(x))) = \operatorname{pr}_\kappa(x)$ theo giả thiết;

do đó $g(f(x)) = \sum_i j_i(g_i(f(x))) = \sum_i j_i(\mathrm{pr}_i(x)) = x$, điều này chứng minh hệ quả.

#### Mệnh đề 7 {#alg-ii-s1-prop-7 .statement}

(i) *Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ* $A$*-môđun có cùng tập hợp chỉ số* $I$; *với mọi họ các ánh xạ tuyến tính* $f_i : E_i \to F_i$ ($i \in I$), *hạn chế lên* $\bigoplus_{i \in I} E_i$ *của ánh xạ tuyến tính* $(x_i) \mapsto (f_i(x_i))$ *là một ánh xạ tuyến tính* $f : \bigoplus_{i \in I} E_i \to \bigoplus_{i \in I} F_i$ *được ký hiệu là* $\bigoplus_{i \in I} f_i$ *hoặc* $\bigoplus_i f_i$ *(trong đó* $f = f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ *nếu* $I = [p, q]$ *là một khoảng trong* $\mathbf{Z}$*).*

(ii) *Cho* $(G_i)_{i \in I}$ *là một họ thứ ba các* $A$*-môđun với* $I$ *làm tập hợp chỉ số và, với mọi* $i \in I$, *cho* $g_i : F_i \to G_i$ *là một ánh xạ tuyến tính; ta viết* $g = \bigoplus_i g_i$. *Để mỗi dãy* $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ *là khớp, điều kiện cần và đủ là dãy*
$$
\bigoplus_i E_i \xrightarrow{f} \bigoplus_i F_i \xrightarrow{g} \bigoplus_i G_i
$$
*là khớp*.

Hiển nhiên, với mọi $(x_i) \in \bigoplus_i E_i$, họ $(f_i(x_i))$ có giá hữu hạn, do đó (i). Mặt khác, nói rằng một phần tử $y = (y_i)$ của $\bigoplus_i F_i$ thuộc $\mathrm{Ker}(g)$ có nghĩa là $y_i \in \mathrm{Ker}(g_i)$ với mọi $i \in I$ (no. 5, Mệnh đề 5); tương tự, nếu $y_i \in \mathrm{Im}(f_i)$ với mọi $i \in I$, thì với mỗi $i \in I$ tồn tại một $x_i \in E_i$ sao cho $y_i = f_i(x_i)$ và khi $y_i = 0$, có thể giả sử rằng $x_i = 0$; do đó $y \in \mathrm{Im}(f)$ và đảo lại là hiển nhiên.

#### Hệ quả 1 {#alg-ii-s1-prop-7-cor-1 .statement}

*Trong các điều kiện của Mệnh đề 7, (i),*
$$
\mathrm{Ker}(f) = \bigoplus_{i \in I} \mathrm{Ker}(f_i), \qquad \mathrm{Im}(f) = \bigoplus_{i \in I} \mathrm{Im}(f_i)
$$
*và có các đẳng cấu chính tắc*
$$
\mathrm{Coim}(f) \to \bigoplus_{i \in I} \mathrm{Coim}(f_i), \qquad \mathrm{Coker}(f) \to \bigoplus_{i \in I} \mathrm{Coker}(f_i)
$$
*được định nghĩa như trong no. 5, Hệ quả của Mệnh đề 5. Đặc biệt, để* $f$ *đơn ánh (resp. toàn ánh, song ánh, không), điều kiện cần và đủ là mỗi* $f_i$ *đơn ánh (resp toàn ánh, song ánh, không)*.

Nếu, với mọi $i \in I$, ta xét một môđun con $F_i$ của $E_i$, môđun $\bigoplus_{i \in I} F_i$ là một môđun con của $\bigoplus_{i \in I} E_i$ và, theo Hệ quả 1 của Mệnh đề 7, có một đẳng cấu chính tắc
$$
\bigoplus_{i \in I} (E_i/F_i) \to \left( \bigoplus_{i \in I} E_i \right) / \left( \bigoplus_{i \in I} F_i \right).
$$

#### Hệ quả 2 {#alg-ii-s1-prop-7-cor-2 .statement}

Cho $(E_i)_{i \in I}, (E'_i)_{i \in I}, (F_\lambda)_{\lambda \in L}, (F'_\lambda)_{\lambda \in L}$ là bốn họ các $A$-môđun và, với mỗi $i \in I$ (resp. mỗi $\lambda \in L$), $u_i : E'_i \to E_i$ (resp. $v_\lambda : F_\lambda \to F'_\lambda$) là một ánh xạ tuyến tính. Khi đó biểu đồ

$$
\begin{array}{ccc}
\operatorname{Hom}\left( \bigoplus_{i \in I} E'_i, \prod_{\lambda \in L} F'_\lambda \right) & \xrightarrow{\phi'} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E'_i, F'_\lambda) \\
\uparrow & & \uparrow \\
\operatorname{Hom}\left( \bigoplus_i u_i, \prod_\lambda v_\lambda \right) & & \prod \operatorname{Hom}(u_i, v_\lambda) \\
\operatorname{Hom}\left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) & \xrightarrow{\phi} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E_i, F_\lambda)
\end{array}
$$

(trong đó $\phi$ và $\phi'$ là các đẳng cấu chính tắc được định nghĩa trong Hệ quả 1 của Mệnh đề 6) là giao hoán.

Việc kiểm tra suy ra ngay lập tức từ các định nghĩa.

Khi mọi $E_i$ bằng cùng một $A$-môđun $E$, tổng trực tiếp $\bigoplus_{i \in I} E_i$ cũng được ký hiệu bởi $E^{(I)}$: các phần tử của nó là các ánh xạ từ $I$ vào $E$ có giá hữu hạn. Nếu, với mọi $i$, $f_i$ được lấy là ánh xạ đồng nhất $E \to E$, theo Mệnh đề 6, ta thu được một ánh xạ tuyến tính $E^{(I)} \to E$, được gọi là *codiagonal*, ánh xạ mỗi họ $(x_i)_{i \in I}$ các phần tử của $E$, có giá hữu hạn, vào *tổng* của nó $\sum_{i \in I} x_i$.

#### Nhận xét {#alg-ii-s1-n6-rem-1 .statement}

Nhắc lại rằng định nghĩa tổng trực tiếp mở rộng ngay lập tức đến một họ $(E_i)_{i \in I}$ các *nhóm* không nhất thiết giao hoán, ký hiệu nhân đương nhiên thay thế ký hiệu cộng; khi đó ta nói "*tích hạn chế*" hoặc "*tổng hạn chế*" thay cho "*tổng trực tiếp*" (I, § 4, no. 9).

Lưu ý rằng $E$ là một nhóm con *chuẩn tắc* của tích $F = \prod_{i \in I} E_i$ và mỗi $j_k(E_k)$ là một nhóm con *chuẩn tắc* của $F$; hơn nữa, với hai chỉ số phân biệt $\lambda, \mu$, mọi phần tử của $j_\lambda(E_\lambda)$ *hoán vị được* với mọi phần tử của $j_\mu(E_\mu)$. Mệnh đề 6 mở rộng sang trường hợp tổng quát với giả thiết rằng, với hai chỉ số phân biệt $\lambda, \mu$, mọi phần tử của $f_\lambda(E_\lambda)$ đều *hoán vị được* trong $M$ với mọi phần tử của $f_\mu(E_\mu)$ (I, § 4, no. 9, Mệnh đề 12). Tính chất "*kết hợp*" của tổng hạn chế suy ra ngay lập tức từ điều này. Mệnh đề 7 và các Hệ quả 1 và 2 của nó vẫn đúng mà không cần sửa đổi.

### 7. GIAO VÀ TỔNG CÁC MÔĐUN CON

Đối với mọi họ $(M_i)_{i \in I}$ các môđun con của một $A$-môđun $E$, giao $\bigcap_{i \in I} E_i$ là một môđun con của $E$. Nếu, với mỗi $i \in I$, $\phi_i$ ký hiệu đồng cấu chính tắc $E \to E/M_i$, thì $\bigcap_{i \in I} M_i$ là *hạt nhân* của đồng cấu $\phi : x \mapsto (\phi_i(x))$ từ $E$ vào $\prod_{i \in I} (E/M_i)$, nói cách khác, có một *dãy khớp*

$$
0 \longrightarrow \bigcap_{i \in I} M_i \longrightarrow E \xrightarrow{\phi} \prod_{i \in I} (E/M_i).
$$

Ánh xạ tuyến tính $\phi$ và ánh xạ
$$
E / \left( \bigcap_{i \in I} M_i \right) \to \prod_{i \in I} (E / M_i)
$$
thu được bằng cách chuyển qua thương, được gọi là chính tắc.

Đặc biệt:

#### Mệnh đề 8 {#alg-ii-s1-prop-8 .statement}

*Nếu một họ* $(M_i)_{i \in I}$ *các môđun con của* $E$ *có giao rút về* $0$ *thì* $E$ *đẳng cấu chính tắc với một môđun con của* $\prod_{i \in I} (E / M_i)$.

Cho một tập con $X$ của một $A$-môđun $E$, giao $F$ của các môđun con của $E$ chứa $X$ được gọi là môđun con *sinh* bởi $X$ và $X$ được gọi là một *tập sinh* (hoặc *hệ sinh*) của $F$ (I, § 4, no. 3); đối với một họ $(a_i)_{i \in I}$ các phần tử của $E$, môđun con sinh bởi tập hợp các $a_i$ được gọi là môđun con sinh bởi họ $(a_i)$.

Một $A$-môđun được gọi là *sinh hữu hạn* nếu nó có một tập sinh *hữu hạn*.

#### Mệnh đề 9 {#alg-ii-s1-prop-9 .statement}

*Môđun con sinh bởi một họ* $(a_i)_{i \in I}$ *các phần tử của một* $A$*-môđun* $E$ *là tập hợp các tổ hợp tuyến tính của họ* $(a_i)$.

Mọi môđun con của $E$ chứa tất cả các $a_i$ cũng chứa các tổ hợp tuyến tính của các $a_i$. Ngược lại, các công thức (1) và (2) của no. 1 chứng minh rằng tập hợp các tổ hợp tuyến tính của các $a_i$ là một môđun con của $E$ mà hiển nhiên chứa tất cả các $a_i$ và do đó là môđun con nhỏ nhất chứa chúng.

#### Hệ quả 1 {#alg-ii-s1-prop-9-cor-1 .statement}

*Cho* $u : E \to F$ *là một ánh xạ tuyến tính, S là một tập con của* $E$ *và* $M$ *là môđun con của* $E$ *được sinh bởi* $S$. *Khi đó* $u(M)$ *là môđun con của* $F$ *được sinh bởi* $u(S)$.

Đặc biệt, ảnh qua $u$ của mọi môđun con sinh hữu hạn của $E$ là một môđun con sinh hữu hạn của $F$.

#### Nhận xét {#alg-ii-s1-n7-rem-1 .statement}

Nếu $u(x) = 0$ với mọi $x \in S$, thì cũng có $u(x) = 0$ với mọi $x \in M$. Đôi khi chúng tôi sẽ gọi kết quả này là *"nguyên lý mở rộng các đẳng thức tuyến tính"* hoặc *"nguyên lý mở rộng bởi tính tuyến tính"*.

Đặc biệt, để kiểm tra rằng một ánh xạ tuyến tính $u : E \to F$ có dạng $v \circ \phi$, trong đó $v : E / M \to F$ là tuyến tính và $\phi : E \to E / M$ là phép chiếu chính tắc, chỉ cần kiểm tra rằng $u(S) = 0$.

#### Hệ quả 2 {#alg-ii-s1-prop-9-cor-2 .statement}

*Môđun con sinh bởi hợp của một họ* $(M_i)_{i \in I}$ *các môđun con của một môđun* $E$ *trùng với tập hợp các tổng* $\sum_{i \in I} x_i$, *trong đó* $(x_i)_{i \in I}$ *chạy qua tập hợp các họ phần tử của* $E$ *có giá hữu hạn sao cho* $x_i \in M_i$ *với mọi* $i \in I$.

Rõ ràng mọi tổ hợp tuyến tính của các phần tử của $\bigcup_{i \in I} M_i$ đều có dạng trên; mệnh đề đảo lại là hiển nhiên.

Môđun con của E sinh bởi hợp của một họ $(M_i)_{i \in I}$ các môđun con của E được gọi là *tổng* của họ $(M_i)$ và được ký hiệu bởi $\sum_{i \in I} M_i$.

Nếu với mọi $i \in I$, $h_i$ là đơn ánh chính tắc $M_i \to E$ và $h : (x_i) \mapsto \sum_i h_i(x_i)$ là ánh xạ tuyến tính từ $\bigoplus_{i \in I} M_i$ vào E tương ứng với họ $(h_i)$ (no. 6, Mệnh đề 6), thì $\sum_{i \in I} M_i$ là *ảnh* của $h$; nói cách khác, có một *dãy khớp*

$$
\bigoplus_{i \in I} M_i \xrightarrow{h} E \longrightarrow E / \left( \sum_{i \in I} M_i \right) \longrightarrow 0.
$$

#### Hệ quả 3 {#alg-ii-s1-prop-9-cor-3 .statement}

*Nếu* $(M_\lambda)_{\lambda \in L}$ *là một họ phải có hướng các môđun con của một A-môđun E, thì tổng* $\sum_{\lambda \in L} M_\lambda$ *trùng với hợp* $\bigcup_{\lambda \in L} M_\lambda$.

$\bigcup_{\lambda \in L} M_\lambda \subset \sum_{\lambda \in L} M_\lambda$ *luôn luôn đúng không cần giả thiết; mặt khác, với mọi họ con hữu hạn* $(M_\lambda)_{\lambda \in J}$ *của* $(M_\lambda)_{\lambda \in L}$, *theo giả thiết tồn tại một* $\mu \in L$ *sao cho* $M_\lambda \subset M_\mu$ *với mọi* $\lambda \in J$, *do đó* $\sum_{\lambda \in L} M_\lambda \subset M_\mu$ *và vì thế từ Hệ quả 2 suy ra* $\sum_{\lambda \in L} M_\lambda \subset \bigcup_{\lambda \in L} M_\lambda$.

#### Hệ quả 4 {#alg-ii-s1-prop-9-cor-4 .statement}

*Cho* $0 \to E \xrightarrow{f} F \xrightarrow{g} G \to 0$ *là một dãy khớp các A-môđun, S là một hệ sinh của* E, *T là một hệ sinh của* G. *Nếu T' là một tập con của F sao cho* $g(T') = T$, *thì T' \cup f(S) là một hệ sinh của* F.

Môđun con F' của F sinh bởi T' \cup f(S) chứa $f(E)$ và, vì $g(F')$ chứa T, nên $g(F') = G$; do đó $F' = F$.

#### Hệ quả 5 {#alg-ii-s1-prop-9-cor-5 .statement}

*Trong một dãy khớp* $0 \to E \to F \to G \to 0$ *các A-môđun, nếu E và G sinh hữu hạn thì F cũng sinh hữu hạn.*

#### Mệnh đề 10 {#alg-ii-s1-prop-10 .statement}

*Cho* M, N *là hai môđun con của một A-môđun E. Khi đó có hai dãy khớp*

$$
\begin{align*}
&0 \longrightarrow M \cap N \xrightarrow{u} M \oplus N \xrightarrow{i-j} M + N \longrightarrow 0 \\
&0 \longrightarrow E/(M \cap N) \xrightarrow{v} (E/M) \oplus (E/N) \xrightarrow{p-q} E/(M + N) \longrightarrow 0
\end{align*}
$$

*trong đó* $i : M \to M + N$, $j : N \to M + N$ *là các đơn ánh chính tắc,*
$$
p : E/M \to E/(M + N) \quad \text{và} \quad q : E/N \to E/(M + N)
$$

*các toàn ánh chính tắc, và trong đó các đồng cấu u và v được xác định như sau:*

nếu $f : M \cap N \to M \to M \oplus N$ và $g : M \cap N \to N \to M \oplus N$ là các đơn ánh chính tắc, thì $u = f + g$, và nếu $r : E/(M \cap N) \to E/M \to (E/M) \oplus (E/N)$ và
$$
s : E/(M \cap N) \to E/N \to (E/M) \oplus (E/N)
$$
là các ánh xạ chính tắc, thì $v = r + s$.

Ta chứng minh tính chính xác của (29): hiển nhiên $i - j$ là toàn ánh và $u$ là đơn ánh. Mặt khác, nói rằng $(i - j)(x, y) = 0$, trong đó $x \in M$ và $y \in N$, có nghĩa là $i(x) - j(y) = 0$, do đó $i(x) = j(y) = z \in M \cap N$, suy ra theo định nghĩa $x = f(z), y = g(z)$, điều này chứng minh rằng $\operatorname{Ker}(i - j) = \operatorname{Im} u$.

Ta chứng minh tính chính xác của (30): rõ ràng $p - q$ là toàn ánh. Mặt khác, nói rằng $v(t) = 0$ với $t \in E/(M \cap N)$ có nghĩa là $r(t) = s(t) = 0$, do đó $t$ là lớp theo mod. $(M \cap N)$ của một phần tử $z \in E$ mà các lớp theo mod. $M$ và theo mod. $N$ đều bằng không, điều này kéo theo $z \in M \cap N$ và $t = 0$. Cuối cùng, nói rằng $(p - q)(x, y) = 0$, trong đó $x \in E/M, y \in E/N$ có nghĩa là $p(x) = q(y)$, hay cũng có nghĩa là tồn tại hai phần tử $z', z''$ của $E$ mà các lớp theo mod. $M$ và mod. $N$ của chúng lần lượt là $x$ và $y$ và sao cho $z' - z'' \in M + N$. Do đó tồn tại $t' \in M, t'' \in N$ sao cho $z' - z'' = t' - t''$, suy ra
$$
z' - t' = z'' - t'' = z.
$$
Gọi $w$ là lớp theo mod. $(M \cap N)$ của $z; r(w)$ là lớp theo mod. $M$ của $z$ và do đó cũng là lớp của $z'$, tức là $x$; tương tự $s(w) = y$, điều này hoàn tất chứng minh rằng $\operatorname{Ker}(p - q) = \operatorname{Im} v$.

### 8. TỔNG TRỰC TIẾP CỦA CÁC MÔĐUN CON

#### Định nghĩa 6 {#alg-ii-s1-def-6 .statement}

*Một A-môđun* $E$ *được gọi là tổng trực tiếp của một họ* $(M_\iota)_{\iota \in I}$ *các môđun con của* $E$ *nếu ánh xạ chính tắc* $\bigoplus_{\iota \in I} M_\iota \to E$ *(no. 6)* *là một đẳng cấu*.

Điều đó tương đương với việc nói rằng mọi $x \in E$ đều có thể được viết *theo một cách duy nhất* dưới dạng $x = \sum_{\iota \in I} x_\iota$, trong đó $x_\iota \in E_\iota$ với mọi $\iota \in I$; phần tử $x_\iota$ tương ứng như vậy với $x$ được gọi là *thành phần* của $x$ trong $E_\iota$; ánh xạ $x \mapsto x_\iota$ là *tuyến tính*.

#### Nhận xét {#alg-ii-s1-n8-rem-1 .statement}

(1) Cho $(M_\iota)_{\iota \in I}, (N_\iota)_{\iota \in I}$ là hai họ môđun con của một môđun $E$, với cùng tập hợp chỉ số; giả sử rằng $E$ *vừa* là tổng trực tiếp của họ $(M_\iota)$ vừa của họ $(N_\iota)$ và *rằng* $N_\iota \subset M_\iota$ với mọi $\iota \in I$. Khi đó $N_\iota = M_\iota$ *với mọi* $\iota \in I$, như suy ra ngay lập tức từ no. 6, Hệ quả 1 của Mệnh đề 7 áp dụng cho các đơn ánh chính tắc $f_\iota : N_\iota \to M_\iota$.

#### Mệnh đề 11 {#alg-ii-s1-prop-11 .statement}

*Cho* $(M_\iota)_{\iota \in I}$ *là một họ các môđun con của một A-môđun* $E$. *Các tính chất sau là tương đương*:

(a) *Môđun con* $\sum_{\iota \in I} M_\iota$ *là tổng trực tiếp của họ* $(M_\iota)_{\iota \in I}$.

(b) *Quan hệ* $\sum_{i \in I} x_i = 0$, *trong đó* $x_i \in M_i$ *với mọi* $i \in I$, *suy ra* $x_i = 0$ *với mọi* $i \in I$.

(c) *Với mọi* $\kappa \in I$, *giao của* $M_\kappa$ *và* $\sum_{i \neq \kappa} M_i$ *thu về* 0.

Ngay lập tức thấy rằng (a) và (b) là tương đương, vì quan hệ $\sum_i x_i = \sum_i y_i$ là tương đương với $\sum_i (x_i - y_i) = 0$. Mặt khác, theo Định nghĩa 6, (a) suy ra (c) bởi tính duy nhất của biểu thức của một phần tử của $\bigoplus_{i \in I} M_i$ dưới dạng một tổng trực tiếp của các phần tử $x_i \in M_i$. Cuối cùng, quan hệ $\sum_i x_i = 0$, trong đó $x_i \in M_i$ với mọi $i$, có thể viết, với mọi $\kappa \in I$, thành $x_\kappa = \sum_{i \neq \kappa} (-x_i)$; khi đó điều kiện (c) suy ra $x_\kappa = 0$ với mọi $\kappa \in I$, do đó (c) suy ra (b).

#### Định nghĩa 7 {#alg-ii-s1-def-7 .statement}

*Một tự đồng cấu e của một A-môđun E được gọi là một phép chiếu nếu* $e \circ e = e$ *(nói cách khác, nếu e là một phần tử lũy đẳng trong vành End(E)). Trong* $\operatorname{End}(E)$ *một họ* $(e_\lambda)_{\lambda \in L}$ *các phép chiếu được gọi là trực giao nếu* $e_\lambda \circ e_\mu = 0$ *với* $\lambda \neq \mu$.

#### Mệnh đề 12 {#alg-ii-s1-prop-12 .statement}

*Cho E là một A-môđun.*

(i) *Nếu E là tổng trực tiếp của một họ* $(M_\lambda)_{\lambda \in L}$ *các môđun con và, với mọi* $x \in E$, $e_\lambda(x)$ *là thành phần của x trong* $M_\lambda$, $(e_\lambda)$ *là một họ trực giao các phép chiếu sao cho* $x = \sum_{\lambda \in L} e_\lambda(x)$ *với mọi* $x \in E$.

(ii) *Ngược lại, nếu* $(e_\lambda)_{\lambda \in L}$ *là một họ trực giao các phép chiếu trong* $\operatorname{End}(E)$ *sao cho* $x = \sum_{\lambda \in L} e_\lambda(x)$ *với mọi* $x \in E$, *thì E là tổng trực tiếp của họ các môđun con* $M_\lambda = e_\lambda(E)$.

Tính chất (i) suy ra từ các định nghĩa và (ii) là một trường hợp riêng của no. 6, Hệ quả 2 của Mệnh đề 6, áp dụng cho các đơn ánh chính tắc $M_\lambda \to E$ và các ánh xạ $e_\lambda : E \to M_\lambda$.

Chú ý rằng khi L là hữu hạn thì điều kiện $x = \sum_{\lambda \in L} e_\lambda(x)$ với mọi $x \in E$ cũng có thể được viết trong $\operatorname{End}(E)$.

(31)
$$
1_E = \sum_{\lambda \in L} e_\lambda.
$$

#### Hệ quả {#alg-ii-s1-n8-cor-1 .statement}

*Với mọi phép chiếu e của E, E là tổng trực tiếp của ảnh* $M = e(E)$ *và hạt nhân* $N = e^{-1}(0)$ *của e; với mọi* $x = x_1 + x_2 \in E$ *với* $x_1 \in M$ *và* $x_2 \in N$, $x_1 = e(x)$; *1 − e là một phép chiếu của E có ảnh là N và hạt nhân là M*.

$(1 - e)^2 = 1 - 2e + e^2 = 1 - e$ *trong* $\operatorname{End}(E)$ *và do đó* $1 - e$ *là một phép chiếu; hơn nữa vì* $e(1 - e) = (1 - e)e = e - e^2 = 0$, *E là tổng trực tiếp của các ảnh* $M$ *và* $N$ *của e và* $1 - e$ *theo Mệnh đề 12. Sau cùng, với mọi* $x \in E$, *quan hệ* $x \in M$ *tương đương với* $x = e(x)$; *vì* $x = e(x)$ *theo định nghĩa kéo theo* $x \in M$ *và, ngược lại, nếu* $x = e(x')$ *với* $x' \in E$, *thì* $e(x) = e^2(x') = e(x') = x;$

điều này do đó cho thấy rằng M là hạt nhân của $1 - e$ và, khi đổi vai trò của $e$ và $1 - e$, ta cũng thấy tương tự rằng N là hạt nhân của $e$.

#### Nhận xét {#alg-ii-s1-n8-rem-2 .statement}

(2) Cho E, F là hai A-môđun sao cho E là tổng trực tiếp của một họ hữu hạn $(M_i)_{1 \leq i \leq m}$ các môđun con và F là tổng trực tiếp của một họ hữu hạn $(N_j)_{1 \leq j \leq n}$ các môđun con. Khi đó đã biết (no. 6, Hệ quả 1 của Mệnh đề 6) rằng $\mathrm{Hom}_A(E, F)$ được đồng nhất một cách chính tắc với tích $\prod_{i,j} \mathrm{Hom}_A(M_i, N_j)$; nói chính xác, với một họ $(u_{ji})$, trong đó $u_{ji} \in \mathrm{Hom}_A(M_i, N_j)$, tương ứng một ánh xạ tuyến tính $u : E \to F$ được định nghĩa như sau. Chỉ cần định nghĩa hạn chế của $u$ trên mỗi $M_i$ và với mỗi $x_i \in M_i$,
$$
u(x_i) = \sum_{j=1}^n u_{ji}(x_i).
$$
Bây giờ cho G là một A-môđun thứ ba, là tổng trực tiếp của một họ hữu hạn $(P_k)_{1 \leq k \leq p}$ các môđun con; cho $v$ là một ánh xạ tuyến tính từ F vào G và cho $(v_{kj}) \in \prod_{j,k} \mathrm{Hom}_A(N_j, P_k)$ là họ tương ứng với nó một cách chính tắc. Với mọi $x_i \in M_i$,
$$
v(u(x_i)) = \sum_{j=1}^n v(u_{ji}(x_i)) = \sum_{k=1}^p \sum_{j=1}^n v_{kj}(u_{ji}(x_i)).
$$
Do đó ta thấy rằng nếu viết
$$
w_{ki} = \sum_{j=1}^n v_{kj} \circ u_{ji} \in \mathrm{Hom}_A(M_i, P_k)
$$
thì họ $(w_{ki})$ tương ứng một cách chính tắc với ánh xạ tuyến tính hợp thành $w = v \circ u$ từ E tới G (x. § 10, no. 5).

### 9. MÔĐUN CON BỔ SUNG

#### Định nghĩa 8 {#alg-ii-s1-def-8 .statement}

Trong một A-môđun E, hai môđun con $M_1, M_2$ được gọi là bổ sung nhau nếu E là tổng trực tiếp của $M_1$ và $M_2$.

Mệnh đề 11 của no. 8 cho thấy rằng để $M_1$ và $M_2$ bổ sung nhau, điều kiện cần và đủ là $M_1 + M_2 = E$ và $M_1 \cap M_2 = \{0\}$ (x. I, § 4, no. 9, Mệnh đề 15).

#### Mệnh đề 13 {#alg-ii-s1-prop-13 .statement}

Cho $M_1, M_2$ là hai môđun con bổ sung nhau trong một A-môđun E. Hạn chế lên $M_1$ của ánh xạ chính tắc $E \to E/M_2$ là một đẳng cấu từ $M_1$ lên $E/M_2$.

Ánh xạ tuyến tính này là toàn ánh vì $M_1 + M_2 = E$ và nó là đơn ánh vì hạt nhân của nó là giao của $M_1$ với hạt nhân $M_2$ của $E \to E/M_2$ và do đó thu về $\{0\}$.

#### Hệ quả {#alg-ii-s1-n9-cor-1 .statement}

Nếu $M_2$ và $M_2'$ là hai phần bù của cùng một môđun con $M_1$ của E, thì tập hợp các cặp có thứ tự $(x, x') \in M_2 \times M_2'$ sao cho $x - x' \in M_1$ là đồ thị của một đẳng cấu từ $M_2$ lên $M_2'$.

Ngay lập tức thấy rằng đó là đồ thị của đẳng cấu hợp thành $M_2 \to E/M_1 \to M'_2$.

#### Định nghĩa 9 {#alg-ii-s1-def-9 .statement}

*Một môđun con $M$ của một $A$-môđun $E$ được gọi là một nhân tử trực tiếp của $E$ nếu nó có một môđun con bổ sung trong $E$.*

Khi điều này xảy ra, $E/M$ đẳng cấu với một phần bù của $M$ (Mệnh đề 13).

Một môđun con không nhất thiết thừa nhận một phần bù (Bài tập 11). Khi một môđun con là một nhân tử trực tiếp, nói chung nó có nhiều phần bù phân biệt; tuy nhiên các phần bù này đẳng cấu chính tắc với nhau (Hệ quả của Mệnh đề 13).

#### Mệnh đề 14 {#alg-ii-s1-prop-14 .statement}

*Điều kiện cần và đủ để một môđun con $M$ của một môđun $E$ là một nhân tử trực tiếp là tồn tại một phép chiếu của $E$ có ảnh là $M$ hoặc một phép chiếu của $E$ có hạt nhân là $M$.*

Điều này suy ra ngay lập tức từ no. 8, Mệnh đề 12 và Hệ quả.

#### Mệnh đề 15 {#alg-ii-s1-prop-15 .statement}

*Cho một dãy khớp các $A$-môđun*
$$
(33)\quad 0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$
*các mệnh đề sau là tương đương:*
(a) *Môđun con $f(E)$ của $F$ là một nhân tử trực tiếp.*
(b) *Tồn tại một phép rút tuyến tính $r : F \to E$ liên kết với $f$ (Lý thuyết tập hợp, II, § 3, no. 8, Định nghĩa 11).*
(c) *Tồn tại một tiết diện tuyến tính $s : G \to F$ liên kết với $g$ (Lý thuyết tập hợp, II, § 3, no. 8, Định nghĩa 11).*
*Khi đó, $f + s : E \oplus G \to F$ là một đẳng cấu.*

Nếu tồn tại một phép chiếu $e$ trong $\mathrm{End}(F)$ sao cho $e(F) = f(E)$, thì đồng cấu $f^{-1} \circ e : F \to E$ là một phép co rút tuyến tính liên kết với $f$; ngược lại, nếu tồn tại một phép co rút như vậy $r$, thì hiển nhiên $f \circ r$ là một phép chiếu trong $F$ có ảnh là $f(E)$, do đó (a) và (b) là tương đương (Mệnh đề 14). Nếu $f(E)$ có một phần bù $E'$ trong $F$ và $j : E' \to F$ là đơn ánh chính tắc, thì $g \circ j$ là một đẳng cấu từ $E'$ lên $G$ và đẳng cấu nghịch đảo, được xét như một ánh xạ từ $G$ vào $F$, là một tiết diện tuyến tính liên kết với $g$. Ngược lại, nếu tồn tại một tiết diện như vậy $s$, thì $s \circ g$ là một phép chiếu trong $F$ có hạt nhân là $f(E)$, do đó (a) và (c) là tương đương (Mệnh đề 14). Hơn nữa $s$ là một song ánh từ $G$ lên $s(G)$ và vì $s(G)$ bù cho $f(E)$, nên $f + s$ là một đẳng cấu.

Chú ý rằng việc cho $r$ (tương ứng $s$) tương đương với việc cho một phần bù của $f(E)$ trong $F$, tức là hạt nhân của $r$ (tương ứng ảnh của $s$).

Khi dãy khớp (33) thỏa mãn các điều kiện của Mệnh đề 15, người ta nói rằng nó *tách* hoặc nói rằng $(F, f, g)$ là một mở rộng *tầm thường* của $G$ bởi $E$ (I, § 6, no. 1).

#### Hệ quả 1 {#alg-ii-s1-prop-15-cor-1 .statement}

Cho $u : E \to F$ là một ánh xạ tuyến tính. Để tồn tại một ánh xạ tuyến tính $v : F \to E$ sao cho $u \circ v = 1_F$ (trường hợp trong đó người ta nói rằng $u$ khả nghịch phải và $v$ được gọi là nghịch đảo phải của $u$), điều kiện cần và đủ là $u$ toàn ánh và hạt nhân của nó là một nhân tử trực tiếp trong $E$. Khi đó môđun con $\operatorname{Im}(v)$ của $E$ là một phần bù của $\operatorname{Ker}(u)$.

Hiển nhiên điều kiện cần là $u$ toàn ánh; vì khi đó $v$ là một tiết diện liên kết với $u$, kết luận suy ra từ Mệnh đề 15.

#### Hệ quả 2 {#alg-ii-s1-prop-15-cor-2 .statement}

Cho $u : E \to F$ là một ánh xạ tuyến tính. Để tồn tại một ánh xạ tuyến tính $v : F \to E$ sao cho $v \circ u = 1_E$ (trường hợp khi đó nói rằng $u$ khả nghịch trái và $v$ được gọi là nghịch đảo trái của $u$), điều kiện cần và đủ là $u$ đơn ánh và ảnh của nó là một nhân tử trực tiếp trong $F$. Khi đó môđun con $\operatorname{Ker}(v)$ của $F$ là một phần bù của $\operatorname{Im}(u)$.

Hiển nhiên điều kiện cần là $u$ phải đơn ánh; vì khi đó $v$ là một phép co liên kết với $u$, kết luận cũng suy ra từ Mệnh đề 15.

#### Nhận xét {#alg-ii-s1-n9-rem-1 .statement}

(1) Cho $M, N$ là hai môđun con bù nhau trong một $A$-môđun $E$, $p, q$ là các phép chiếu của $E$ lên $M$ và $N$ tương ứng với phân tích của $E$ thành tổng trực tiếp của $M$ và $N$. Ta biết (no. 6, Hệ quả 1 của Mệnh đề 6) rằng, với mọi $A$-môđun $F$, ánh xạ $(u, v) \mapsto u \circ p + v \circ q$ là một đẳng cấu từ
$$
\operatorname{Hom}_A(M, F) \oplus \operatorname{Hom}_A(N, F)
$$
lên $\operatorname{Hom}_A(E, F)$. Ảnh của $\operatorname{Hom}_A(M, F)$ dưới đẳng cấu này là tập hợp các ánh xạ tuyến tính $w : E \to F$ sao cho $w(x) = 0$ với mọi $x \in N$.

(2) Nếu $M, N$ là hai môđun con của $E$ sao cho $M \cap N$ là một nhân tử trực tiếp của $M$ và của $N$, thì $M \cap N$ cũng là một nhân tử trực tiếp của $M + N$: nếu $P$ (resp. $Q$) là một phần bù của $M \cap N$ trong $M$ (resp. $N$), thì $M + N$ là tổng trực tiếp của $M \cap N, P$ và $Q$, như được kiểm tra ngay lập tức.

### 10. MÔĐUN CÓ ĐỘ DÀI HỮU HẠN

Nhắc lại rằng (I, § 4, no. 4, Định nghĩa 7) một $A$-môđun $M$ được gọi là đơn nếu nó không quy về 0 và không chứa môđun con nào phân biệt với $M$ và $\{0\}$. Một $A$-môđun $M$ được gọi là có độ dài hữu hạn nếu nó có một chuỗi Jordan-Hölder $(M_i)_{0 \leq i \leq n}$ và khi đó số $n$ các thương của chuỗi này (không phụ thuộc vào chuỗi Jordan-Hölder của $M$ được xét) được gọi là độ dài của $M$ (I, § 4, no. 7, Định nghĩa 11); ta sẽ ký hiệu nó bởi $\operatorname{long}(M)$ hoặc $\operatorname{long}_A(M)$. Một $A$-môđun quy về 0 có độ dài 0; nếu $M$ là một $A$-môđun khác không có độ dài hữu hạn thì $\operatorname{long}(M) > 0$.

#### Mệnh đề 16 {#alg-ii-s1-prop-16 .statement}

Cho $M$ là một $A$-môđun và $N$ là một môđun con của $M$; để $M$ có độ dài hữu hạn, điều kiện cần và đủ là $N$ và $M/N$ cũng vậy, và khi đó
$$
\operatorname{long}(N) + \operatorname{long}(M/N) = \operatorname{long}(M).
$$
Chứng minh đã được cho trong I, § 4, no. 7, Mệnh đề 10.

#### Hệ quả 1 {#alg-ii-s1-prop-16-cor-1 .statement}

Cho $M$ là một $A$-môđun có độ dài hữu hạn; để một môđun con $N$ của $M$ bằng $M$, điều kiện cần và đủ là $\operatorname{long}(N) = \operatorname{long}(M)$.

#### Hệ quả 2 {#alg-ii-s1-prop-16-cor-2 .statement}

Cho $u : M \to N$ là một đồng cấu $A$-môđun. Nếu $M$ hoặc $N$ có độ dài hữu hạn, thì $\operatorname{Im}(u)$ cũng vậy. Nếu $M$ có độ dài hữu hạn, thì $\operatorname{Ker}(u)$ cũng vậy và
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Ker}(u)) = \operatorname{long}(M).
$$
Nếu $N$ có độ dài hữu hạn, thì $\operatorname{Coker}(u)$ cũng vậy và
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Coker}(u)) = \operatorname{long}(N).
$$

#### Hệ quả 3 {#alg-ii-s1-prop-16-cor-3 .statement}

Cho $(M_i)_{0 \leq i \leq n}$ là một họ hữu hạn các $A$-môđun có độ dài hữu hạn. Nếu tồn tại một dãy khớp các ánh xạ tuyến tính
$$
0 \longrightarrow M_0 \xrightarrow{u_0} M_1 \xrightarrow{u_1} M_2 \longrightarrow \cdots \longrightarrow M_{n-1} \xrightarrow{u_{n-1}} M_n \longrightarrow 0
$$
thì
$$
\sum_{k=0}^n (-1)^k \operatorname{long}(M_k) = 0.
$$
Hệ quả là hiển nhiên đối với $n = 1$ và chính là Mệnh đề 16 đối với $n = 2$; ta chứng minh bằng quy nạp theo $n$. Nếu $M'_{n-1} = \operatorname{Im}(u_{n-2})$, thì, theo giả thiết quy nạp,
$$
\sum_{k=0}^{n-2} (-1)^k \operatorname{long}(M_k) + (-1)^{n-1} \operatorname{long}(M'_{n-1}) = 0.
$$
Mặt khác, dãy khớp $0 \to M'_{n-1} \to M_{n-1} \to M_n \to 0$ cho
$$
\operatorname{long}(M'_{n-1}) + \operatorname{long}(M_n) = \operatorname{long}(M_{n-1}),
$$
do đó quan hệ (38).

#### Hệ quả 4 {#alg-ii-s1-prop-16-cor-4 .statement}

Cho $M$ và $N$ là hai môđun con có độ dài hữu hạn của một $A$-môđun $E$; khi đó $M + N$ có độ dài hữu hạn và
$$
\operatorname{long}(M + N) + \operatorname{long}(M \cap N) = \operatorname{long}(M) + \operatorname{long}(N).
$$
Chỉ cần áp dụng Hệ quả 3 cho dãy khớp (29) (no. 7).
$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$
dùng thực tế rằng $\operatorname{long}(M \oplus N) = \operatorname{long}(M) + \operatorname{long}(N)$ theo (34).

#### Hệ quả 5 {#alg-ii-s1-prop-16-cor-5 .statement}

Cho $M$ là một $A$-môđun là tổng của một họ $(N_i)$ các môđun con có độ dài hữu hạn. Khi đó $M$ có độ dài hữu hạn và
$$
\operatorname{long}(M) \leq \sum_i \operatorname{long}(N_i).
$$

Hơn nữa, để hai vế của (40) bằng nhau, điều kiện cần và đủ là M là tổng trực tiếp của các $N_i$.

Ta đã thấy (no. 7, công thức (28)) rằng có một ánh xạ tuyến tính toàn ánh chính tắc $h : \bigoplus_i N_i \to M$; do đó hệ quả suy ra từ (35).

#### Hệ quả 6 {#alg-ii-s1-prop-16-cor-6 .statement}

*Cho M và N là hai môđun con của một A-môđun E sao cho E/M và E/N là các môđun có độ dài hữu hạn; khi đó E/(M \cap N) có độ dài hữu hạn và*

$$
\text{(41)} \quad \text{long}(E/(M \cap N)) + \text{long}(E/(M + N)) = \text{long}(E/M) + \text{long}(E/N).
$$

Chỉ cần áp dụng Hệ quả 3 cho dãy khớp (30)

$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$

dùng thực tế là

$$
\text{long}((E/M) \oplus (E/N)) = \text{long}(E/M) + \text{long}(E/N).
$$

#### Hệ quả 7 {#alg-ii-s1-prop-16-cor-7 .statement}

*Cho $(M_i)$ là một họ hữu hạn các môđun con của một A-môđun E sao cho các $E/M_i$ là các môđun có độ dài hữu hạn. Khi đó $E/(\bigcap_i M_i)$ có độ dài hữu hạn và*

$$
\text{(42)} \quad \text{long}\left(E/(\bigcap_i M_i)\right) \leq \sum_i \text{long}(E/M_i).
$$

Ta đã thấy (công thức (27)) rằng có một ánh xạ tuyến tính đơn ánh chính tắc $E/(\bigcap_i M_i) \to \bigoplus_i (E/M_i)$.

#### Nhận xét {#alg-ii-s1-n10-rem-1 .statement}

Trừ no. 7, Mệnh đề 9, *mọi* kết quả của các số 2 đến 10 đều đúng cho các *nhóm giao hoán với toán tử* tùy ý, trong các mệnh đề môđun con (tương ứng, môđun thương) được thay bằng các nhóm con ổn định (tương ứng, các nhóm thương theo nhóm con ổn định); ta cũng quy ước gọi các đồng cấu của nhóm với toán tử là "ánh xạ tuyến tính". Các hệ quả của no. 7, Mệnh đề 9 cũng đúng cho các nhóm giao hoán với toán tử: điều này là hiển nhiên đối với các Hệ quả 4 và 5, và cả đối với Hệ quả 2, vì $\alpha \left( \sum_{i \in I} x_i \right) = \sum_{i \in I} \alpha x_i$ với mọi toán tử $\alpha$, và Hệ quả 3 suy ra từ đó. Đối với Hệ quả 1, chỉ cần nhận thấy rằng nếu N là một nhóm con ổn định của F chứa $u(S)$, thì $u^{-1}(N)$ là một nhóm con ổn định của E chứa S, do đó $u^{-1}(N)$ chứa M và vì thế $u(M) \subset N$.

### 11. HỌ TỰ DO. CƠ SỞ

Cho A là một vành, T là một tập hợp và xét A-môđun $A_s^{(T)}$. Theo định nghĩa, đó là tổng trực tiếp ngoài của một họ $(M_t)_{t \in T}$ các A-môđun đều bằng $A_s$ và với mọi $t \in T$ có một đơn ánh chính tắc $j_t : A_s \to A_s^{(T)}$ (no. 6). Ta viết j_t(1) = e_t để cho $e_t = (\delta_{tt'})_{t' \in T}$, trong đó $\delta_{tt'}$ bằng 0 nếu $t' \neq t$, bằng 1 nếu $t' = t$ ("ký hiệu Kronecker"; $(t, t') \mapsto \delta_{tt'}$ chính là hàm đặc số của đường chéo của $T \times T$); khi đó mọi $x = (\xi_t)_{t \in T} \in A_s^{(T)}$ đều có thể viết duy nhất:
$$
x = \sum_{t \in T} \xi_t e_t.
$$
Ánh xạ $\phi : t \mapsto e_t$ từ $T$ vào $A_s^{(T)}$ được gọi là chính tắc; nó là đơn ánh nếu $A$ khác không. Ta sẽ thấy rằng cặp có thứ tự $(A_s^{(T)}, \phi)$ là một nghiệm của một bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1).

#### Mệnh đề 17 {#alg-ii-s1-prop-17 .statement}

*Với mọi A-môđun E và mọi ánh xạ $f : T \to E$, tồn tại một và chỉ một ánh xạ A-tuyến tính $g : A_s^{(T)} \to E$ sao cho $f = g \circ \phi$.*

Điều kiện $f = g \circ \phi$ có nghĩa là $g(e_t) = f(t)$ với mọi $t \in T$, điều này tương đương với $g(\xi e_t) = \xi f(t)$ với mọi $\xi \in A$ và mọi $t \in T$ và cũng có nghĩa là $g \circ j_t$ là ánh xạ tuyến tính $\xi \mapsto \xi f(t)$ từ $A_s$ vào $E$ với mọi $t \in T$; do đó mệnh đề là một trường hợp riêng của no. 6, Mệnh đề 6.

Ánh xạ tuyến tính $g$ được nói là *được xác định* bởi họ $(f(t))_{t \in T}$ các phần tử của $E$; theo định nghĩa
$$
g\left( \sum_{t \in T} \xi_t e_t \right) = \sum_{t \in T} \xi_t f(t).
$$

Hạt nhân $R$ của $g$ là tập hợp các $(\xi_t) \in A_s^{(T)}$ sao cho $\sum_t \xi_t f(t) = 0$; đôi khi cũng nói rằng môđun $R$ là *môđun các quan hệ tuyến tính giữa các phần tử của họ* $(f(t))_{t \in T}$. Dãy khớp
$$
0 \longrightarrow R \longrightarrow A_s^{(T)} \overset{g}{\longrightarrow} E
$$
được nói là *được xác định* bởi họ $(f(t))_{t \in T}$.

#### Hệ quả 1 {#alg-ii-s1-prop-17-cor-1 .statement}

*Cho* $T, T'$ *là hai tập hợp, $g : T \to T'$ là một ánh xạ. Khi đó tồn tại một và chỉ một ánh xạ A-tuyến tính* $f : A^{(T)} \to A^{(T')}$ *làm cho biểu đồ*
$$
\begin{array}{ccc}
T & \overset{g}{\longrightarrow} & T' \\
\downarrow \phi & & \downarrow \phi' \\
A^{(T)} & \overset{f}{\longrightarrow} & A^{(T')}
\end{array}
$$
*giao hoán, trong đó* $\phi$ *và* $\phi'$ *là các ánh xạ chính tắc.*

Chỉ cần áp dụng Mệnh đề 17 cho ánh xạ hợp thành $T \overset{g}{\to} T' \overset{\phi'}{\to} A^{(T')}$.

#### Hệ quả 2 {#alg-ii-s1-prop-17-cor-2 .statement}

*Để một họ* $(a_t)_{t \in T}$ *các phần tử của một A-môđun E là một hệ sinh của E, điều kiện cần và đủ là ánh xạ tuyến tính* $A_s^{(T)} \to E$ *được xác định bởi họ này là toàn ánh.*

Đây chỉ là một cách khác để phát biểu Mệnh đề 9 của no. 7.

#### Định nghĩa 10 {#alg-ii-s1-def-10 .statement}

*Một họ* $(a_t)_{t \in T}$ *các phần tử của một* $\mathbf{A}$*-môđun* $E$ *được gọi là một họ tự do* (tương ứng, *một cơ sở của* $E$) *nếu ánh xạ tuyến tính* $A_s^{(T)} \to E$ *được xác định bởi họ này là đơn ánh* (tương ứng, *song ánh*). *Một môđun được gọi là tự do nếu nó có một cơ sở*.

Đặc biệt, một nhóm giao hoán $G$ được gọi là *tự do* nếu $G$ (được viết theo lối cộng) là một *môđun* $\mathbf{Z}$* tự do* (xem I, § 7, no. 7).

Định nghĩa 10, cùng với Hệ quả 2 của Mệnh đề 17, cho thấy rằng một cơ sở của một $\mathbf{A}$-môđun $E$ là một *họ sinh tự do* của $E$. Vì vậy, mọi họ tự do các phần tử của $E$ đều là một cơ sở của môđun con mà nó sinh ra.

Theo định nghĩa, $\mathbf{A}$-môđun $A_s^{(T)}$ là tự do và họ $(e_t)_{t \in T}$ là một cơ sở (gọi là *chính tắc*) của $\mathbf{A}$-môđun này. Khi $\mathbf{A} \neq \{0\}$, $T$ thường được đồng nhất với tập hợp các $e_t$ bởi song ánh chính tắc $t \mapsto e_t$; điều này tương đương với việc viết $\sum_{t \in T} \xi_t \cdot t$ thay cho $\sum_{t \in T} \xi_t a_t$ cho các phần tử của $A_s^{(T)}$. Khi quy ước này được chấp nhận, các phần tử của $A_s^{(T)}$ được gọi là *các tổ hợp tuyến tính hình thức* (với các hệ số trong $\mathbf{A}$) *của các phần tử của* $T$.

Định nghĩa 10 và Mệnh đề 17 cho ngay lập tức kết quả sau đây:

#### Hệ quả 3 {#alg-ii-s1-def-10-cor-3 .statement}

*Cho* $E$ *là một* $\mathbf{A}$*-môđun tự do*, $(a_t)_{t \in T}$ *là một cơ sở của* $E$, $F$ *là một* $\mathbf{A}$*-môđun và* $(b_t)_{t \in T}$ *là một họ các phần tử của* $F$. *Tồn tại một và chỉ một ánh xạ tuyến tính* $f : E \to F$ *sao cho*
$$
f(a_t) = b_t \quad \text{với mọi } t \in T.
$$
*Để* $f$ *là đơn ánh* (tương ứng, *toàn ánh*), *điều kiện cần và đủ là* $(b_t)$ *là một họ tự do trong* $F$ (tương ứng, *một hệ sinh của* $F$).

Khi một họ $(a_t)_{t \in T}$ không tự do, ta gọi nó là *liên quan*. Định nghĩa 10 cũng có thể được phát biểu như sau: nói rằng họ $(a_t)_{t \in T}$ là *tự do* có nghĩa là quan hệ $\sum_{t \in T} \lambda_t a_t = 0$ (trong đó họ $(\lambda_t)$ có giá hữu hạn) kéo theo $\lambda_t = 0$ với mọi $t \in T$; nói rằng $(a_t)_{t \in T}$ là một *cơ sở* của $E$ có nghĩa là mọi $x \in E$ đều có thể được viết dưới dạng $x = \sum_{t \in T} \xi_t a_t$ theo một và chỉ một cách; khi đó, với mọi $t \in T$, $\xi_t$ được gọi là *thành phần* (hoặc *tọa độ*) *của* $x$ *có chỉ số* $t$ *đối với cơ sở* $(a_t)$; ánh xạ $x \to \xi_t$ từ $E$ vào $A_s$ là *tuyến tính*.

Giả sử $\mathbf{A} \neq \{0\}$; khi đó, trong một $\mathbf{A}$-môđun $E$, hai phần tử của một họ tự do $(a_t)_{t \in T}$ có các chỉ số phân biệt thì bản thân chúng cũng *phân biệt*: thật vậy, nếu $a_{t'} = a_{t''}$ với $t' \neq t''$, thì $\sum_{t \in T} \lambda_t a_t = 0$ với $\lambda_{t'} = 1$, $\lambda_{t''} = -1$ và $\lambda_t = 0$ đối với các phần tử của $T$ phân biệt với $t'$ và $t''$. Một tập con $S$ của $E$ sẽ được gọi là một *tập con tự do* (tương ứng, một *cơ sở* của $E$) nếu họ được xác định bởi ánh xạ đồng nhất của $S$ lên chính nó là tự do (tương ứng, là một cơ sở của $E$); khi đó mọi họ được xác định bởi một ánh xạ song ánh từ một tập chỉ số lên $S$ đều là tự do (tương ứng, là một cơ sở). Các phần tử của một tập con tự do của $E$ cũng được gọi là *độc lập tuyến tính*.

Nếu một tập con của E không tự do, thì nó được gọi là liên quan hoặc một hệ liên quan, và các phần tử của nó được gọi là phụ thuộc tuyến tính.

Mọi tập con của một tập con tự do đều là tự do; đặc biệt, tập con rỗng là tự do và là một cơ sở của môđun con {0} của E.

#### Mệnh đề 18 {#alg-ii-s1-prop-18 .statement}

*Để một họ $(a_t)_{t \in T}$ của một môđun E là tự do, điều kiện cần và đủ là mọi họ con hữu hạn của $(a_t)_{t \in T}$ đều tự do.*

Điều này suy ra ngay lập tức từ định nghĩa.

Mệnh đề 18 cho thấy rằng tập hợp các tập con tự do của E, được sắp thứ tự bởi quan hệ bao hàm, là quy nạp (*Lý thuyết tập hợp*, III, § 2, no. 4); vì nó không rỗng (do $\varnothing$ thuộc về nó), nên theo Bổ đề Zorn, nó có một phần tử cực đại $(a_l)_{l \in I}$. Suy ra (nếu $A \neq \{0\}$) rằng với mọi $x \in E$ tồn tại một phần tử $\mu \neq 0$ của A và một họ $(\xi_l)$ các phần tử của A sao cho $\mu x = \sum_l \xi_l a_l$ (xem § 7, no. 1).

#### Mệnh đề 19 {#alg-ii-s1-prop-19 .statement}

*Cho E là một A-môđun, là tổng trực tiếp của một họ $(M_\lambda)_{\lambda \in L}$ các môđun con. Nếu, với mỗi $\lambda \in L$, $S_\lambda$ là một tập con tự do (tương ứng, tập sinh, cơ sở) của $M_\lambda$, thì $S = \bigcup_{\lambda \in L} S_\lambda$ là một tập con tự do (tương ứng, tập sinh, cơ sở) của E.*

Mệnh đề suy ra từ các định nghĩa và quan hệ $A_s^{(S)} = \bigoplus_{\lambda \in L} A_s^{(S_\lambda)}$ (tính kết hợp của các tổng trực tiếp, xem no. 6).

#### Nhận xét {#alg-ii-s1-n11-rem-1 .statement}

(1) Theo Định nghĩa 10, nếu $A \neq \{0\}$ và $(a_l)_{l \in I}$ là một họ tự do, thì không phần tử nào $a_\kappa$ có thể bằng một tổ hợp tuyến tính của các $a_l$ có chỉ số $l \neq \kappa$. Nhưng ngược lại, một họ $(a_l)$ thỏa mãn điều kiện này không nhất thiết là một họ tự do. Chẳng hạn, cho A là một miền nguyên và $a, b$ là hai phần tử khác nhau khác không; trong A, được xét như một A-môđun, $a$ và $b$ tạo thành một hệ liên quan, vì $(-b)a + ab = 0$. Nhưng nói chung không tồn tại phần tử $x \in A$ sao cho $a = xb$ hoặc $b = xa$ (xem tuy nhiên § 7, no. 1, *Nhận xét*).

Một phần tử $x$ của một môđun E được gọi là *tự do* nếu $\{x\}$ là một tập con tự do, nghĩa là nếu quan hệ $\alpha x = 0$ kéo theo $\alpha = 0$. Mọi phần tử của một tập con tự do đều là tự do và đặc biệt 0 không thể thuộc bất kỳ tập con tự do nào khi $A \neq \{0\}$.

#### Nhận xét {#alg-ii-s1-n11-rem-2 .statement}

(2) Một môđun tự do có thể có những phần tử $\neq 0$ mà không tự do: chẳng hạn, A-môđun $A_s$ là tự do nhưng các ước phải của không trong A không phải là các phần tử tự do của $A_s$.

(3) Trong nhóm cộng $\mathbf{Z}/(n)$ ($n$ là một số nguyên $\geq 2$) được xét như một $\mathbf{Z}$-môđun, không có phần tử nào là tự do và *a fortiori* $\mathbf{Z}/(n)$ không phải là một môđun tự do.

(4) Có thể xảy ra trường hợp mọi phần tử $\neq 0$ của một A-môđun đều là tự do mà môđun lại không tự do. Chẳng hạn, trường $\mathbf{Q}$ các số hữu tỉ là một $\mathbf{Z}$-môđun có tính chất này, vì hai phần tử $\neq 0$ của $\mathbf{Q}$ luôn luôn tạo thành một hệ liên quan và do đó một cơ sở của $\mathbf{Q}$ chỉ có thể chứa một phần tử duy nhất $a$; nhưng không phải mọi phần tử của $\mathbf{Q}$ đều có dạng $na$ với $n \in \mathbf{Z}$ (xem VII, § 3).

#### Mệnh đề 20 {#alg-ii-s1-prop-20 .statement}

*Mọi A-môđun E đều đẳng cấu với một môđun thương của một A-môđun tự do.*

Nếu T là một tập sinh của E, tồn tại một ánh xạ tuyến tính toàn ánh $A_s^{(T)} \to E$ (Hệ quả 2 của Mệnh đề 17), và nếu R là hạt nhân của ánh xạ này, thì E đẳng cấu với $A_s^{(T)}/R$.

Đặc biệt, có thể lấy $T = E$; khi đó có một ánh xạ tuyến tính toàn ánh $A_s^{(E)} \to E$, được gọi là *chính tắc*.

Đặc biệt, nói rằng một A-môđun E là *sinh hữu hạn* (no. 7) có nghĩa là nó đẳng cấu với một thương của một A-môđun tự do có một *cơ sở hữu hạn* hoặc cũng có nghĩa là tồn tại một dãy khớp có dạng

$$
A_s^n \to E \to 0 \quad (n \text{ là một số nguyên } > 0).
$$

Chú ý rằng nếu $A \neq \{0\}$ thì mọi cơ sở của một môđun tự do *sinh hữu hạn* E tất yếu là *hữu hạn*, vì nếu S là một hệ sinh hữu hạn và B là một cơ sở của E, thì mỗi phần tử của S là một tổ hợp tuyến tính của một số hữu hạn phần tử của B và nếu B' là tập hợp tất cả các phần tử của B xuất hiện như vậy trong biểu thức của các phần tử của S, thì B' là hữu hạn và mọi $x \in E$ là một tổ hợp tuyến tính của các phần tử của B', do đó $B' = B$.

#### Mệnh đề 21 {#alg-ii-s1-prop-21 .statement}

*Mọi dãy khớp của các A-môđun*

$$
0 \longrightarrow G \xrightarrow{g} E \xrightarrow{f} F \longrightarrow 0
$$

*trong đó F là một A-môđun tự do, đều phân rã* (no. 9). *Nói chính xác hơn, nếu* $(b_\lambda)_{\lambda \in L}$ *là một cơ sở của F và, với mỗi* $\lambda \in L$, $a_\lambda$ *là một phần tử của E sao cho* $f(a_\lambda) = b_\lambda$, *thì họ* $(a_\lambda)_{\lambda \in L}$ *là tự do và sinh ra một môđun con bổ sung của g(G)*.

Tồn tại một và chỉ một ánh xạ tuyến tính $h : F \to E$ sao cho $h(b_\lambda) = a_\lambda$ với mọi $\lambda \in L$ (Hệ quả 3 của Mệnh đề 17). Vì h là một tiết diện tuyến tính liên quan với f, mệnh đề suy ra từ I, § 4, no. 9, Mệnh đề 15.

#### Nhận xét {#alg-ii-s1-n11-rem-3 .statement}

(5) Cho $(a_i)_{1 \leq i \leq n}$ là một *cơ sở* của một A-môđun E và cho $(b_i)_{1 \leq i \leq n}$ là một họ các phần tử của E được cho bởi các quan hệ

$$
b_i = \lambda_{1i} a_1 + \cdots + \lambda_{ii} a_i \quad (1 \leq i \leq n)
$$

trong đó $\lambda_{ii}$ là *khả nghịch* trong A; khi đó $(b_i)_{1 \leq i \leq n}$ là một *cơ sở* của E. Chỉ cần lập luận bằng quy nạp theo $n$, mệnh đề là hiển nhiên đối với $n = 1$. Nếu E' là môđun con của E được sinh bởi họ $(a_i)_{1 \leq i \leq n-1}$, thì theo giả thiết quy nạp suy ra rằng $(b_i)_{1 \leq i \leq n-1}$ là một cơ sở của E'; mặt khác, theo (46), nếu $\mu b_n \in E'$ với $\mu \in A$, thì cũng có $\mu \lambda_{nn} a_n \in E'$, do đó $\mu = 0$ vì $\lambda_{nn}$ khả nghịch. Vậy họ $(b_i)_{1 \leq i \leq n}$ là tự do và, vì
$$
a_n = -\lambda_{nn}^{-1}\lambda_{1n}a_1 - \cdots - \lambda_{nn}^{-1}\lambda_{n-1,n}a_{n-1} + \lambda_{nn}^{-1}b_n
$$
nên thấy rằng $(b_i)_{1 \leq i \leq n}$ là một hệ sinh của E, điều này hoàn tất chứng minh. Kết quả này dễ dàng được tổng quát hóa cho một họ $(a_i)_{i \in I}$ mà tập chỉ số I được sắp thứ tự tốt.

### 12. LINH HÓA TỬ. MÔĐUN TRUNG THÀNH. MÔĐUN ĐƠN SINH

#### Định nghĩa 11 {#alg-ii-s1-def-11 .statement}

*Linh hóa tử của một tập con S của một A-môđun E là tập hợp các phần tử $\alpha \in A$ sao cho $\alpha x = 0$ với mọi $x \in S$.*

Linh hóa tử của S thường được ký hiệu bởi Ann(S); đối với một tập con S chỉ gồm một phần tử x, ta viết Ann(x) thay cho Ann(\{x\}) và gọi Ann(x) là *linh hóa tử của x*.

Quan hệ $\alpha x = 0$ cũng có thể được biểu thị bằng cách nói rằng *x bị triệt tiêu bởi $\alpha$*.

Ngay lập tức thấy rằng linh hóa tử của một tập con tùy ý S của E là một *iđêan trái* của A; để nó bằng A thì điều kiện cần và đủ (theo (M_IV)) là $S = \{0\}$. Nếu hai tập con S, T của E sao cho $S \subset T$, thì linh hóa tử của T được chứa trong linh hóa tử của S. Nếu $(S_i)_{i \in I}$ là một họ tùy ý các tập con của E, thì linh hóa tử của hợp $\bigcup_i S_i$ là giao của các linh hóa tử của các $S_i$. Đặc biệt, linh hóa tử của một tập con S của E là giao của các linh hóa tử của các phần tử của S. Nói rằng một phần tử của E là *tự do* tương đương với việc nói rằng linh hóa tử của nó là $\{0\}$. Với mọi $x \in E$ và mọi $\alpha \in A$, linh hóa tử của $\alpha x$ là tập hợp các $\beta \in A$ sao cho $\beta \alpha \in \mathrm{Ann}(x)$.

Linh hóa tử của một *môđun con* M của E là một *iđêan hai phía* của A; thật vậy, nếu $\alpha x = 0$ với mọi $x \in M$, thì cũng có $\alpha (\beta x) = 0$ với mọi $x \in M$ và mọi $\beta \in A$, nên $\alpha \beta$ thuộc linh hóa tử của M với mọi $\beta \in A$. Đặc biệt, linh hóa tử của E là một iđêan hai phía của A.

Với mọi $\alpha \in A$, gọi $h_\alpha$ là phép vị tự $x \mapsto \alpha x$; ta biết rằng ánh xạ $\alpha \mapsto h_\alpha$ từ A vào vành tự đồng cấu $\mathcal{E} = \mathrm{Hom}_\mathbf{Z}(E, E)$ của nhóm giao hoán (không có toán tử) E là một *đồng cấu vành* (§ 2, no. 5). Ảnh ngược của 0 qua đồng cấu này là *linh hóa tử* $a$ của E; do đó ảnh của A qua đồng cấu $\alpha \mapsto h_\alpha$ đẳng cấu với vành thương $A/a$. Môđun E được gọi là *trung thành* nếu linh hóa tử $a$ của nó rút về 0.

Cho E là một A-môđun bất kỳ, $a$ là một iđêan hai phía của A được chứa trong Ann(E) và gọi $\dot{\alpha}$ là một phần tử của vành thương $A/a$; với mọi $x \in E$, phần tử $\alpha x$ là như nhau với mọi $\alpha \in A$ thuộc lớp $\dot{\alpha}$ mod. $a$; nếu phần tử này được ký hiệu bởi $\dot{\alpha} x$, thì ngay lập tức thấy rằng ánh xạ (α, x) ↦ αx xác định (cùng với phép cộng trên E) một cấu trúc môđun (A/α) trên E. Khi α = Ann(E), môđun (A/α) E được xác định như vậy là *trung thành*; ta sẽ nói rằng đó là môđun trung thành *liên kết* với A-môđun E. Hãy nhận xét rằng mọi môđun con của một A-môđun E cũng là môđun con của môđun trung thành liên kết và ngược lại.

#### Định nghĩa 12 {#alg-ii-s1-def-12 .statement}

*Một môđun được gọi là đơn sinh nếu nó được sinh bởi một phần tử duy nhất.*

Mệnh đề 9 của no. 7 cho thấy rằng, nếu E là một A-môđun đơn sinh và a là một phần tử sinh của E, thì E đồng nhất với tập A.a các ξa, trong đó ξ chạy qua A.

#### Ví dụ {#alg-ii-s1-n12-exa-1 .statement}

(1) Mọi nhóm đơn sinh, vì là giao hoán (I, § 4, no. 10, Mệnh đề 18), đều là một $\mathbf{Z}$-môđun đơn sinh.
(2) Nếu A là một vành giao hoán, thì các môđun con đơn sinh của A-môđun A chính là các *iđêan chính* (I, § 8, no. 6) của vành A.
(3) Mọi A-môđun *đơn* E đều đơn sinh, vì môđun con của E được sinh bởi một phần tử ≠ 0 của E tất yếu bằng E.

#### Mệnh đề 22 {#alg-ii-s1-prop-22 .statement}

*Cho A là một vành. Mọi môđun thương của $A_s$ đều đơn sinh. Ngược lại, cho E là một A-môđun đơn sinh, c là một phần tử sinh của E và a là linh hóa tử của nó; ánh xạ tuyến tính $\xi \mapsto \xi c$ xác định, khi chuyển qua thương, một đẳng cấu từ $A_s/a$ lên E.*

Vì $A_s$ tự nó là đơn sinh, được sinh bởi 1, mệnh đề thứ nhất suy ra từ no. 7, Hệ quả 1 của Mệnh đề 9. Mệnh đề thứ hai là hiển nhiên, vì $\xi \mapsto \xi c$ theo giả thiết là toàn ánh và có hạt nhân là a.

Chú ý rằng, nếu A không giao hoán, các linh hóa tử của hai phần tử sinh phân biệt c, c' của một A-môđun đơn sinh E nói chung là *phân biệt* và cũng phân biệt với linh hóa tử của môđun E. Mặt khác, nếu A là *giao hoán*, linh hóa tử của một phần tử sinh c của E được chứa trong linh hóa tử của mọi phần tử của E và do đó là linh hóa tử của toàn bộ E.

#### Hệ quả {#alg-ii-s1-n12-cor-1 .statement}

*Mọi môđun con của một A-môđun đơn sinh E đều đẳng cấu với một môđun thương b/a trong đó a và b là hai iđêan trái của A sao cho a ⊂ b. Mọi môđun thương của một môđun đơn sinh đều là đơn sinh.*

Mệnh đề thứ hai là ngay lập tức và mệnh đề thứ nhất suy ra từ Mệnh đề 22 và I, § 4, no. 6, Định lý 4.

Mặt khác cũng chú ý rằng một môđun con của một môđun đơn sinh không nhất thiết là đơn sinh. Chẳng hạn, nếu A là một vành giao hoán trong đó tồn tại các iđêan không chính (VII, § 1, no. 1), thì các iđêan ấy là những môđun con không đơn sinh của A-môđun đơn sinh A.

Từ các định nghĩa suy ra rằng một môđun con của một A-môđun E được sinh bởi một họ $(a_i)$ các phần tử của E là *tổng* của các môđun con đơn sinh

Aa_i của E; để (a_i) là một cơ sở của E, điều kiện cần và đủ là mỗi a_i là một phần tử tự do của E và tổng của các Aa_i là trực tiếp.

#### Mệnh đề 23 {#alg-ii-s1-prop-23 .statement}

Cho E là một A-môđun, là tổng trực tiếp của một họ vô hạn (M_i)_{i \in I} các môđun con khác không. Với mọi hệ sinh S của E, Card(S) \geq Card(I).

Với mọi x \in S, gọi C_x là tập hữu hạn các chỉ số i \in I sao cho thành phần của x trong M_i là \neq 0 và đặt C = \bigcup_{x \in S} C_x. Theo định nghĩa, mọi x \in S đều thuộc môđun con của E là tổng trực tiếp của các M_i với i \in C, và giả thiết rằng S sinh ra E do đó kéo theo C = I; vì I theo giả thiết là vô hạn, nên S cũng vô hạn (Set Theory, III, § 5, no. 1, Hệ quả 1 của Mệnh đề 1); do đó Card(I) = Card(C) \leq Card(S) (Set Theory, III, § 6, no. 3, Hệ quả 3 của Định lý 2).

#### Hệ quả 1 {#alg-ii-s1-prop-23-cor-1 .statement}

Trong các giả thiết của Mệnh đề 23, giả sử rằng mỗi M_i là đơn sinh và E là tổng trực tiếp của một họ thứ hai (N_\lambda)_{\lambda \in L} các môđun con đơn sinh khác không. Khi đó Card(L) = Card(I).

Nếu b_\lambda là một phần tử sinh của N_\lambda, tập các b_\lambda là một hệ sinh của E, nên Card(L) \geq Card(I). Đặc biệt L là vô hạn và, khi đổi vai trò của (M_i) và (N_\lambda), tương tự ta có Card(I) \geq Card(L), do đó có hệ quả.

#### Hệ quả 2 {#alg-ii-s1-prop-23-cor-2 .statement}

Nếu một môđun E thừa nhận một cơ sở vô hạn B, thì mọi hệ sinh của E đều có lực lượng \geq Card(B) và mọi cơ sở của E đều cùng lực lượng với B.

### 13. THAY ĐỔI VÀNH VÔ HƯỚNG

Cho A, B là hai vành và \rho là một đồng cấu của vành B vào vành A. Với mọi A-môđun E, phép toán ngoài (\beta, x) \mapsto \rho(\beta)x xác định (cùng với phép cộng) một cấu trúc B-môđun được gọi là liên kết với \rho và cấu trúc A-môđun trên E; B-môđun này được ký hiệu là \rho_*(E) hoặc E_{[B]} (và thậm chí đơn giản là E nếu không thể có nhầm lẫn). Đặc biệt, nếu B là một vành con của A và \rho : B \to A là đơn ánh chính tắc, E_{[B]} được gọi là B-môđun thu được bằng cách hạn chế vành vô hướng A xuống B; do một sự lạm dụng ngôn ngữ, cách nói này cũng được dùng khi đồng cấu \rho là tùy ý.

Nếu F là một môđun con của A-môđun E, thì \rho_*(F) là một môđun con của \rho_*(E) và \rho_*(E/F) bằng \rho_*(E)/\rho_*(F).

Cho E, F là hai A-môđun; mọi ánh xạ A-tuyến tính u : E \to F cũng là một ánh xạ B-tuyến tính E_{[B]} \to F_{[B]} được ký hiệu bởi \rho_*(u); nói cách khác, có một đơn ánh chính tắc các \mathbf{Z}-môđun

(47)
$$
\operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{[B]}, F_{[B]}).
$$

Ánh xạ này không nhất thiết là song ánh; nói cách khác, một ánh xạ B-tuyến tính E_{[B]} \to F_{[B]} không nhất thiết là A-tuyến tính. Chẳng hạn, một môđun con-B của E_{[B]} không nhất thiết là một môđun con-A của E: nếu A là một trường và B là một trường con của $A$, thì không gian con vectơ $B_s$ của $B$-không gian vectơ $(A_s)_{[B]}$ không phải là một không gian con vectơ-$A$ nếu $B \neq A$.

Ngay lập tức thấy rằng, với mọi họ $(E_i)_{i \in I}$ các $A$-môđun, $B$-môđun $\rho_*\left(\prod_{i \in I} E_i\right)$ (tương ứng, $\rho_*\left(\bigoplus_{i \in I} E_i\right)$) bằng $\prod_{i \in I} \rho_*(E_i)$ (tương ứng, $\bigoplus_{i \in I} \rho_*(E_i)$).

Mọi hệ sinh của $\rho_*(E)$ đều là một hệ sinh của $E$ nhưng đảo lại thì không nhất thiết đúng.

#### Mệnh đề 24 {#alg-ii-s1-prop-24 .statement}

*Cho $A, B$ là hai vành và $\rho : B \to A$ là một đồng cấu vành.*

(i) *Nếu $\rho$ là toàn ánh, ánh xạ chính tắc (47) là song ánh. Với mọi $A$-môđun $E$, mọi môđun con-$B$ của $\rho_*(E)$ đều là một môđun con-$A$ của $E$; mọi hệ sinh của $E$ đều là một hệ sinh của $\rho_*(E)$.*

(ii) *Nếu $\rho$ là đơn ánh, mọi họ tự do trong $A$-môđun $E$ đều là một họ tự do trong $B$-môđun $\rho_*(E)$.*

Mệnh đề này suy ra ngay lập tức từ các định nghĩa.

Chú ý rằng ngay cả khi $\rho$ là đơn ánh, một họ tự do trong $\rho_*(E)$ cũng không nhất thiết tự do trong $E$.

*Chẳng hạn, 1 và $\sqrt{2}$ không tạo thành một hệ tự do trong $\mathbf{R}$ khi coi là một $\mathbf{R}$-không gian vectơ, mặc dù chúng tạo thành một hệ tự do trong $\mathbf{R}$ khi coi là một $\mathbf{Q}$-không gian vectơ (x. Nhận xét 1).*

#### Mệnh đề 25 {#alg-ii-s1-prop-25 .statement}

*Cho $A, B$ là hai vành, $\rho : B \to A$ là một đồng cấu vành và $E$ là một $A$-môđun. Cho $(\alpha_\lambda)_{\lambda \in L}$ là một hệ sinh (tương ứng, họ tự do các phần tử, cơ sở) của $A$ khi xét như một $B$-môđun trái. Cho $(a_\mu)_{\mu \in M}$ là một hệ sinh (tương ứng, họ tự do các phần tử, cơ sở) của $A$-môđun $E$. Khi đó $(\alpha_\lambda a_\mu)_{(\lambda, \mu) \in L \times M}$ là một hệ sinh (tương ứng, (khi $\rho$ là đơn ánh) họ tự do các phần tử, cơ sở) của $B$-môđun $\rho_*(E)$.*

Nếu $x = \sum_{\mu \in M} \gamma_\mu a_\mu$, trong đó $\gamma_\mu \in A$ và $(\alpha_\lambda)$ là một hệ sinh của $A$, ta có thể viết $\gamma_\mu = \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda$, với $\beta_{\lambda \mu} \in B$, với mọi $\mu \in M$, do đó $x = \sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu$. Mặt khác, nếu $(\alpha_\lambda)$ và $(a_\mu)$ là các họ tự do, một quan hệ $\sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu = 0$, với $\beta_{\lambda \mu} \in B$, có thể được viết thành $\sum_{\mu \in M} \left( \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda \right) a_\mu = 0$; vì thế nó kéo theo $\sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda = 0$ với mọi $\mu \in M$ và do đó $\beta_{\lambda \mu} = 0$ với mọi $\lambda, \mu$ nếu $\rho$ là đơn ánh.

#### Hệ quả {#alg-ii-s1-n13-cor-1 .statement}

*Nếu $A$ là một $B$-môđun trái sinh hữu hạn và $E$ là một $A$-môđun trái sinh hữu hạn, thì $\rho_*(E)$ là một $A$-môđun trái sinh hữu hạn.*

Cho $C$ là một vành thứ ba, $\rho' : C \to B$ là một đồng cấu vành và $\rho'' = \rho \circ \rho'$ là đồng cấu hợp thành. Từ các định nghĩa, ngay lập tức suy ra rằng $\rho''_*(E) = \rho'_*(\rho_*(E))$ với mọi $A$-môđun $E$. Đặc biệt, nếu $\rho$ là một *đẳng cấu* từ $B$ lên $A$, thì $E = \rho'_*(\rho_*(E))$, trong đó $\rho'$ ký hiệu đẳng cấu nghịch đảo của $\rho$.

#### Nhận xét {#alg-ii-s1-n13-rem-1 .statement}

(1) Cho $K$ là một trường và $A$ là một vành con của $K$ có tính chất sau: với mọi họ hữu hạn $(\xi_i)_{1 \leq i \leq n}$ các phần tử của $K$, tồn tại một $\gamma \in A$ khác không sao cho $\gamma \xi_i \in A$ với $1 \leq i \leq n$ (một giả thiết luôn được thỏa mãn khi $A$ là *giao hoán* và $K$ là trường các phân thức của $A$). Cho $E$ là một không gian vectơ trên $K$ và $E_{[A]}$ là $A$-môđun thu được bằng cách hạn chế vành các vô hướng xuống $A$. Khi đó, nếu một họ $(x_\lambda)_{\lambda \in L}$ là *tự do trong* $E_{[A]}$ thì nó cũng *tự do trong* $E$. Có thể chỉ cần xét trường hợp $L = \{1, n\}$; nếu có một quan hệ $\sum_{i=1}^n \xi_i x_i = 0$ với $\xi_i \in K$, các $\xi_i$ không đồng thời bằng không, thì suy ra rằng với mọi $\beta \in A$, $\sum_{i=1}^n (\beta \xi_i) x_i = 0$. Theo giả thiết, ta có thể giả sử $\beta \neq 0$ trong $A$ sao cho $\beta \xi_i = \alpha_i$ thuộc $A$ với mọi $i$; nhưng quan hệ $\sum_{i=1}^n \alpha_i x_i = 0$ trái với giả thiết, vì các $\alpha_i$ không đồng thời bằng không.

(2) Nếu đồng cấu vành $\rho : B \to A$ là toàn ánh và $b$ là hạt nhân của nó (do đó $A$ được đồng nhất một cách chính tắc với $B/b$), thì, với mọi $A$-môđun $E$, $b$ được chứa trong linh hóa tử của $\rho_*(E)$ và $E$ là $A$-môđun dẫn xuất từ $\rho_*(E)$ bởi quá trình được định nghĩa ở no. 12.

Cho $A, B$ là hai vành và $\rho : B \to A$ là một đồng cấu. Cho $E$ là một $A$-môđun và $F$ là một $B$-môđun; một ánh xạ *B-tuyến tính* $u : F \to \rho_*(E)$ (cũng gọi là một *ánh xạ B-tuyến tính của* $F$ *vào* $E$ nếu không thể gây nhầm lẫn) cũng được gọi là một *ánh xạ nửa tuyến tính* (đối với $\rho$) của $B$-môđun $F$ vào $A$-môđun $E$; cũng nói rằng cặp có thứ tự $(u, \rho)$ là một *dimorphism* của $F$ vào $E$; do đó điều này có nghĩa là, với $x \in F, y \in F$ và $\beta \in B$,

$$
\begin{cases}
u(x + y) = u(x) + u(y) \\
u(\beta x) = \rho(\beta) u(x).
\end{cases}
$$

Tập hợp $\mathrm{Hom}_B(F, \rho_*(E))$ các ánh xạ $B$-tuyến tính của $F$ vào $E$ cũng được viết là $\mathrm{Hom}_B(F, E)$ nếu không thể có sự nhầm lẫn.

Khi $\rho$ là một *đẳng cấu* từ $B$ lên $A$, quan hệ $u(\beta x) = \rho(\beta) u(x)$ với mọi $\beta \in B$ cũng có thể viết là $u(\rho'(\alpha)x) = \alpha x$ với mọi $\alpha \in A$, trong đó $\rho'$ ký hiệu đẳng cấu nghịch đảo của $\rho$; khi đó nói rằng $u$ là nửa tuyến tính đối với $\rho$ tương đương với việc nói rằng $u$ là một *ánh xạ A-tuyến tính của* $\rho'_*(F)$ *vào* $E$.

#### Ví dụ {#alg-ii-s1-n13-exa-1 .statement}

Ta đã thấy (no. 1) rằng một phép vị tự $h_\alpha : x \mapsto \alpha x$ trên một $A$-môđun $E$ không nhất thiết là một ánh xạ tuyến tính. Nhưng nếu $\alpha$ là *khả nghịch* thì $h_\alpha$ là một *ánh xạ nửa tuyến tính* (hơn nữa còn song ánh) đối với tự đẳng cấu trong $\xi \mapsto \alpha \xi \alpha^{-1}$ của $A$, vì $\alpha(\lambda x) = (\alpha \lambda \alpha^{-1})(\alpha x)$.

Cho C là một vành thứ ba, $\rho': C \to B$ là một đồng cấu và G là một C-môđun. Nếu $v: G \to F$ là một ánh xạ nửa tuyến tính đối với $\rho'$, thì hợp thành $w = u \circ v$ là một ánh xạ nửa tuyến tính của G vào E đối với đồng cấu $\rho'' = \rho \circ \rho'$. Nếu $\rho$ là một *đẳng cấu* và $u: F \to E$ là một ánh xạ nửa tuyến tính *song ánh* đối với $\rho$, thì ánh xạ nghịch đảo $u': E \to F$ là một ánh xạ nửa tuyến tính *đối với đẳng cấu nghịch đảo* $\rho': A \to B$ của $\rho$.

Như vậy, ta thấy rằng, đối với loài cấu trúc được xác định bằng cách cho trên một cặp có thứ tự (A, E) các tập hợp một cấu trúc vành trên A và một cấu trúc A-môđun trái trên E, các *dimorphism* $(u, \phi)$ có thể được lấy làm các *morphism* (*Lý thuyết tập hợp*, IV, § 2, no. 1); trong phần sau, chúng tôi sẽ luôn giả thiết rằng lựa chọn morphism này đã được thực hiện.

*Nhận xét (3)*. Cho $A_1, A_2$ là hai vành, $A = A_1 \times A_2$ là tích của chúng và đặt $e_1 = (1, 0),\ e_2 = (0, 1)$ trong A, sao cho $A_1$ và $A_2$ được đồng nhất một cách chính tắc với các iđêan hai phía $Ae_1$ và $Ae_2$ của A. Với mọi A-môđun E, $e_1E$ và $e_2E$ là các môđun con $E_1,\ E_2$ của E, bị triệt tiêu tương ứng bởi $e_2$ và $e_1$, sao cho, khi đồng nhất một cách chính tắc $A/Ae_2$ với $A_1$ và $A/Ae_1$ với $A_2$, $E_1$ (tương ứng $E_2$) được trang bị một cấu trúc $A_1$-môđun (tương ứng $A_2$-môđun). Hơn nữa, E là *tổng trực tiếp* của $E_1$ và $E_2$, vì mọi $x \in E$ đều có thể viết thành $x = e_1x + e_2x$ và quan hệ $e_1x = e_2y$ kéo theo $e_1x = e_1^2x = e_1e_2y = 0$. Ngược lại, với mọi cặp có thứ tự gồm một $A_1$-môđun $F_1$ và một $A_2$-môđun $F_2$, đặt $E_1$ là A-môđun $(p_1) * (F_1)$, $E_2$ là A-môđun $(p_2) * (F_2)$, trong đó $p_1$ và $p_2$ lần lượt là các phép chiếu của A lên $A_1$ và $A_2$; khi đó trong A-môđun $E = E_1 \oplus E_2,\ E_1 = e_1E,\ E_2 = e_2E$. Do đó, việc nghiên cứu các A-môđun được quy về việc nghiên cứu các $A_1$-môđun và các $A_2$-môđun. Đặc biệt, mọi môđun con M của E đều có dạng $M_1 \oplus M_2$, trong đó $M_1 = e_1M$ và $M_2 = e_2M$.

### 14. ĐA MÔĐUN

Cho A, B là hai vành và xét trên một tập hợp E hai cấu trúc môđun trái có *cùng* luật cộng và lần lượt có vành các toán tử là A và B; gọi $\mathscr{E}$ là vành tự đồng cấu của nhóm cộng E và với mọi $\alpha \in A$ (tương ứng $\beta \in B$) gọi $h_\alpha$ (tương ứng $h'_\beta$) là phần tử $x \mapsto \alpha x$ (tương ứng $x \mapsto \beta x$) của $\mathscr{E}$. Rõ ràng ba tính chất sau là tương đương: (a) $h_\alpha \circ h'_\beta = h'_\beta \circ h_\alpha$ với mọi $\alpha$ và $\beta$; (b) ảnh của A dưới đồng cấu $a \mapsto h_\alpha$ thì *được chứa trong* $\mathrm{Hom}_B(E, E)$; (c) ảnh của B dưới đồng cấu $\beta \mapsto h'_\beta$ thì *được chứa trong* $\mathrm{Hom}_A(E, E)$. Khi cấu trúc A-môđun (tương ứng B-môđun) đang xét là một cấu trúc môđun phải, thì trong (b) (tương ứng (c)) phải thay A (tương ứng B) bằng $A^0$ (tương ứng $B^0$). Có thể phát biểu các tính chất trên bằng cách nói rằng hai cấu trúc môđun (trái hoặc phải) được định nghĩa trên E là *tương thích*.

#### Định nghĩa 13 {#alg-ii-s1-def-13 .statement}

*Cho* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$ *là hai họ vành; một* $((A_\lambda),\ (B_\mu))$*-đa môđun* (hay *đa môđun trên các họ vành* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$) *là một tập hợp* E *được trang bị, với mỗi* $\lambda \in L$, *một cấu trúc* $A_\lambda$*-môđun trái và, với mỗi* $\mu \in M$, *một cấu trúc* $B_\mu$*-môđun phải, mọi cấu trúc môđun ấy đều tương thích từng đôi một.*

Khi họ $(B_\mu)$ (tương ứng $(A_\lambda)$) rỗng, thì E được gọi là một *đa môđun* *trái* (tương ứng *phải*). Khi Card(L) + Card(M) = 2, ta nói "*song môđun*" thay cho "*đa môđun*"; khi đó thường thuận tiện khi xem (như luôn luôn có thể làm được bằng cách thay một vành toán tử bằng vành đối của nó, xem no. 1) một song môđun như có một cấu trúc *môđun trái* đối với một vành A và một cấu trúc *môđun phải* đối với một vành B, khi ấy tính giao hoán của các luật được biểu thị bởi quan hệ

$$
\alpha(x\beta) = (\alpha x)\beta \quad \text{với } x \in E, \alpha \in A, \beta \in B.
$$

Khi đó cũng nói rằng E là một *(A, B)*-*song môđun*.

Hai cấu trúc *đa môđun* trên một tập hợp E được gọi là *tương thích* nếu mọi cấu trúc môđun trên E dùng để định nghĩa cấu trúc đa môđun này hoặc cấu trúc đa môđun kia đều tương thích từng đôi một.

#### Ví dụ {#alg-ii-s1-n14-exa-1 .statement}

(1) Trên một vành A, các cấu trúc môđun của $A_s$ và $A_d$ là tương thích và do đó A có thể được xem một cách chính tắc như một (A, A)-song môđun.

(2) Một A-môđun trái E có một cấu trúc môđun trái chính tắc trên vành $\operatorname{End}_A(E)$ và các cấu trúc A-môđun và $\operatorname{End}_A(E)$-môđun trên E là *tương thích*.

Rõ ràng khi E là một đa môđun trên hai họ vành $(A_\lambda)_{\lambda \in L}, (B_\mu)_{\mu \in M}$, thì E cũng là một đa môđun trên mọi hai họ con $(A_\lambda)_{\lambda \in L'}, (B_\mu)_{\mu \in M'}$, trong đó các cấu trúc $A_\lambda$-môđun và $B_\mu$-môđun với $\lambda \in L'$ và $\mu \in M'$ là những cấu trúc đã cho ban đầu.

Vì các đa môđun là những ví dụ riêng của các nhóm giao hoán có toán tử, nên các kết quả từ số 2 đến no. 10 (xem số 10, *Nhận xét*) có thể được áp dụng cho chúng; đặc biệt, nếu E, F là hai $((A_\lambda), (B_\mu))$-đa môđun, thì một *đồng cấu* $u : E \to F$ là một ánh xạ là một $A_\lambda$-đồng cấu với mọi $\lambda \in L$ và một $B_\mu$-đồng cấu với mọi $\mu \in M$. Các nhóm con ổn định của một $((A_\lambda), (B_\mu))$-đa môđun là các $((A_\lambda), (B_\mu))$-đa môđun (gọi là *đa môđun con*), cũng như các thương theo các nhóm con như vậy (gọi là *đa môđun thương*); các tích và tổng trực tiếp cũng tương tự.

Cho E là một $((A_\lambda), (B_\mu))$-đa môđun và với mỗi $\lambda \in L$ (tương ứng $\mu \in M$) cho $\phi_\lambda : A'_\lambda \to A_\lambda$ (tương ứng $\psi_\mu : B'_\mu \to B_\mu$) là một đồng cấu vành; rõ ràng các cấu trúc $A'_\lambda$-môđun liên kết với các $\phi_\lambda$ và các cấu trúc $A_\lambda$-môđun đã cho trên E, và các cấu trúc $B'_\mu$-môđun liên kết với các $\psi_\mu$ và các cấu trúc $B_\lambda$-môđun đã cho trên E, là tương thích từng đôi một, và do đó xác định trên E một cấu trúc $((A'_\lambda), (B'_\mu))$-đa môđun, được gọi là *liên kết* với cấu trúc $((A_\lambda), (B_\mu))$-đa môđun đã cho và với các $\phi_\lambda$ và $\psi_\mu$.

Nếu E, F là hai đa môđun $((A_\lambda), (B_\mu))$, thì nhóm cộng các đồng cấu từ E vào F được ký hiệu là $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ (hoặc đơn giản là $\operatorname{Hom}(E, F)$). Các công thức (6) đến (8) của no. 2 hiển nhiên đúng đối với các đồng cấu đa môđun $((A_\lambda), (B_\mu))$ và, đặc biệt, $\operatorname{Hom}(E, E) = \operatorname{End}(E)$ có một cấu trúc *vành*;

hơn nữa Hom(E, F) có một cấu trúc môđun *trái* chính tắc trên End(F) và cấu trúc môđun *phải* trên End(E), hai cấu trúc này tương thích với nhau; nói cách khác, Hom(E, F) có một cấu trúc (End(F), End(E))-**song môđun** chính tắc.

Bây giờ giả sử rằng E có một cấu trúc đa môđun mà các vành toán tử trái (tương ứng phải) của nó một mặt là các $A_\lambda$ với $\lambda \in L$ (tương ứng các $B_\mu$ với $\mu \in M$) và mặt khác là các vành của một họ khác $(A'_{\lambda'})_{\lambda' \in L'}$ (tương ứng $(B'_{\mu'})_{\mu' \in M'}$). Tương tự, giả sử rằng F có một cấu trúc đa môđun mà các vành toán tử trái (tương ứng phải) của nó một mặt là các $A_\lambda$ với $\lambda \in L$ (tương ứng các $B_\mu$ với $\mu \in M$) và mặt khác là các vành của một họ khác $(A''_{\lambda''})_{\lambda'' \in L''}$ (tương ứng $(B''_{\mu''})_{\mu'' \in M''}$); để viết gọn, ta sẽ nói rằng E là một đa môđun (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$)) và F là một đa môđun (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$)). Xét E và F như các đa môđun (($A_\lambda$), ($B_\mu$)), do đó *hạn chế* các toán tử vào các họ con ($A_\lambda$) và ($B_\mu$). Theo điều đã nói ở đầu số này, các cấu trúc đa môđun được cho trên E và F xác định một cách chính tắc các đồng cấu vành

$$
A'_{\lambda'} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E), \qquad {B'_{\mu'}}^0 \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E),
$$
$$
A''_{\lambda''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F), \qquad B''_{\mu''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F);
$$

hơn nữa, hai phần tử của $\operatorname{End}_{(A_\lambda), (B_\mu)}(E)$ (tương ứng $\operatorname{End}_{(A_\lambda), (B_\mu)}(F)$), là các ảnh tương ứng của các phần tử thuộc hai vành phân biệt trong số các $A'_{\lambda'}$, hoặc các ${B'_{\mu'}}^0$ (tương ứng các $A''_{\lambda''}$ hoặc các $B''_{\mu''}$), thì giao hoán được; suy ra rằng các đồng cấu ở trên xác định trên $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ một cấu trúc *đa môđun* mà các vành toán tử *trái* là các $A''_{\lambda''}$ ($\lambda'' \in L''$) và các $B'_{\mu'}$ ($\mu' \in M'$), còn các vành toán tử *phải* là các $A'_{\lambda'}$ ($\lambda' \in L'$) và các $B''_{\mu''}$ ($\mu'' \in M''$).

Nếu bây giờ $E'$ là một đa môđun (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$)) và $F'$ là một đa môđun (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$)), thì $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')$ là một

$$
((A''_{\lambda''}), (B'_{\mu'}); (A'_{\lambda'}), (B''_{\mu''}))\text{-đa môđun};
$$

nếu $u : E' \to E, v : F \to F'$ là các đồng cấu đa môđun,

$$
\operatorname{Hom}(u, v) : \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F) \to \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')
$$

được định nghĩa như trong no. 2 và là một đồng cấu *đa môđun*.

#### Nhận xét {#alg-ii-s1-n14-rem-1 .statement}

(1) Cho F là một A-môđun và C là *tâm* của vành A; vì các vị tự trung tâm giao hoán với mọi vị tự, F có một cấu trúc *song môđun* mà các vành toán tử trái là A và C. Nếu E là một A-môđun khác, $\operatorname{Hom}_A(E, F)$ do đó có một cấu trúc C-*môđun* chính tắc (trong đó, với $f \in \operatorname{Hom}_A(E, F)$ và $\gamma \in C$, $\gamma f$ là đồng cấu $x \mapsto \gamma f(x)$); nếu E', F' là hai A-môđun, $u : E' \to E, v : F \to F'$ là hai đồng cấu A, thì ánh xạ $\operatorname{Hom}(u, v)$ là C-*tuyến tính*.

(2) Cho E là một A-môđun trái; vì A có một cấu trúc song môđun (A, A) chính tắc, nên tổng trực tiếp $A^{(T)}$ cũng vậy với mọi tập hợp chỉ số T; theo trên, $\mathrm{Hom}_A(A_s^{(T)}, E)$ có một cấu trúc *A-môđun trái* chính tắc phát sinh từ cấu trúc A-môđun *phải* trên $A_s^{(T)}$: với $f \in \mathrm{Hom}_A(A_s^{(T)}, E)$ và $\alpha \in A$, $\alpha f$ là ánh xạ tuyến tính $x \mapsto f(x\alpha)$. Hệ quả 2 của Mệnh đề 17 ở no. 11 xác định một ánh xạ chính tắc $j_{E, T}$ từ môđun tích $E^T$ vào $\mathrm{Hom}_A(A_s^{(T)}, E)$, ảnh qua $j_{E, T}$ của một họ $(x_t)_{t \in T}$ là ánh xạ tuyến tính $f : A_s^{(T)} \to E$ sao cho $f(e_t) = x_t$ với mọi $t \in T$ (trong đó $(e_t)$ là cơ sở chính tắc của $A_s^{(T)}$); ta biết (*loc. cit.*) rằng $j_{E, T}$ là *song ánh* và từ định nghĩa đã cho ở trên của cấu trúc A-môđun trên $\mathrm{Hom}_A(A_s^{(T)}, E)$ suy ra rằng $j_{E, T}$ là *A-tuyến tính*. Cuối cùng, nếu $u : E \to F$ là một đồng cấu A-môđun, thì biểu đồ

$$
\begin{array}{ccc}
E^T & \xrightarrow{j_{E, T}} & \mathrm{Hom}_A(A_s^{(T)}, E) \\
u^T \downarrow & & \downarrow \mathrm{Hom}(1, u) \\
F^T & \xrightarrow{j_{F, T}} & \mathrm{Hom}_A(A_s^{(T)}, F)
\end{array}
$$

là *giao hoán*.

Chú ý rằng khi T chỉ gồm một phần tử, $j_E : E \to \mathrm{Hom}_A(A_s, E)$ chính là ánh xạ $x \mapsto \theta_x$ được xác định ở no. 2, *Ví dụ* 1.

### Bài tập {#alg-ii-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
