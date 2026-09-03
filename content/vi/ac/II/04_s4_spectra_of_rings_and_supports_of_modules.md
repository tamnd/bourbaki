---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 4
section_title: Spectra of rings and supports of modules
lang: vi
source: ac-i-vii
book_pages: 94-107, 140-146
pdf_pages: 0114-0127, 0160-0166
extraction: ocr
subsections:
    - "no": 1
      title: IRREDUCIBLE SPACES
      page: 94
      pdf_page: 114
    - "no": 2
      title: NOETHERIAN TOPOLOGICAL SPACES
      page: 97
      pdf_page: 117
    - "no": 3
      title: THE PRIME SPECTRUM OF A RING
      page: 98
      pdf_page: 118
    - "no": 4
      title: THE SUPPORT OF A MODULE
      page: 104
      pdf_page: 124
statements: 49
exercises: 28
content_sha256: 14f73fe44fb9e2681b77121c24e2b4800b39ad9be11ce57788d45bcc0a93ff10
translated_from: content/en/ac/II/04_s4_spectra_of_rings_and_supports_of_modules.md
source_content_sha256: afbce0ee70ea654b4478dd2d27c1a7060b1124651d86be84ea7b4b58f7101cd3
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-b4ef23db
glossary_version: 34
glossary_terms_sha256: 1524b5936a113652716cf376e3d938ad44de223967103b81b0dd7f998197f53a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. PHỔ CỦA CÁC VÀNH VÀ GIÁ ĐỠ CỦA CÁC MÔĐUN

### 1. CÁC KHÔNG GIAN BẤT KHẢ QUY

#### Định nghĩa 1 {#ac-ii-s4-def-1 .statement}

Một không gian tôpô $X$ được gọi là bất khả quy nếu mọi giao hữu hạn của các tập mở không rỗng của $X$ là không rỗng.

Bằng cách xét họ rỗng các tập mở của $X$, ta thấy rằng một không gian bất khả quy là không rỗng; để một không gian tôpô $X$ là bất khả quy, điều kiện cần và đủ là nó không rỗng và giao của hai tập mở không rỗng của $X$ luôn luôn không rỗng (hay, điều tương đương, hợp của hai tập đóng phân biệt với $X$ luôn luôn phân biệt với $X$).

#### Mệnh đề 1 {#ac-ii-s4-prop-1 .statement}

Cho $X$ là một không gian tôpô không rỗng. Các điều kiện sau là tương đương:
(a) $X$ là bất khả quy;
(b) mọi tập mở không rỗng của $X$ là trù mật trong $X$;
(c) mọi tập mở của $X$ là liên thông.

Theo định nghĩa, một tập trù mật trong $X$ là một tập hợp gặp mọi tập mở không rỗng, do đó (a) và (b) là tương đương. Hiển nhiên (c) kéo theo (a), vì nếu $U_1$ và $U_2$ là các tập mở rời nhau không rỗng, thì $U_1 \cup U_2$ là một tập mở không liên thông. Cuối cùng ta chứng minh rằng (a) kéo theo (c): nếu $U$ là một tập mở không liên thông, thì nó là hợp của hai tập hợp rời nhau không rỗng $U', U''$ mở trong $U$ và do đó cũng mở trong $X$, điều này kéo theo rằng $X$ không bất khả quy.

Một không gian Hausdorff là bất khả quy chỉ khi nó gồm một điểm duy nhất.

Một tập con $E$ của một không gian tôpô $X$ được gọi là một tập bất khả quy nếu không gian con $E$ của $X$ là bất khả quy. Điều này xảy ra khi và chỉ khi, với mọi cặp tập hợp $U, V$ mở trong $X$ và gặp $E$, $U \cap V$ cũng gặp $E$, hoặc (điều tương đương) rằng, với mọi cặp tập hợp $F, G$ đóng trong $X$ và thỏa mãn $E \subset F \cup G$, thì $E \subset F$ hoặc $E \subset G$. Bằng quy nạp theo $n$, ta suy ra rằng, nếu $(F_i)_{1 \leq i \leq n}$ là một họ hữu hạn các tập đóng của $X$ sao cho $E \subset \bigcup_{i=1}^n F_i$, thì tồn tại một chỉ số $i$ sao cho $E \subset F_i$.

#### Mệnh đề 2 {#ac-ii-s4-prop-2 .statement}

Trong một không gian tôpô $X$, để một tập hợp $E$ là bất khả quy, điều kiện cần và đủ là bao đóng $\overline{E}$ của nó là như vậy.

Để một tập mở của $X$ gặp $E$, điều kiện cần và đủ là nó gặp $\overline{E}$; khi đó mệnh đề suy ra từ các nhận xét trên.

#### Mệnh đề 3 {#ac-ii-s4-prop-3 .statement}

(i) *Nếu $X$ là một không gian bất khả quy, mọi tập con mở không rỗng của $X$ là bất khả quy.*

(ii) *Cho $(U_\alpha)_{\alpha \in A}$ là một phủ không rỗng của một không gian tôpô $X$ gồm các tập mở sao cho $U_\alpha \cap U_\beta = \emptyset$ với mọi cặp chỉ số $(\alpha, \beta)$. Nếu các tập $U_\alpha$ là bất khả quy, thì không gian $X$ là bất khả quy.*

(i) Nếu $X$ là bất khả quy, $U \subset X$ khác rỗng và mở trong $X$ và $V \subset U$ khác rỗng và mở trong $U$, thì $V$ cũng mở trong $X$, do đó trù mật trong $X$ và *a fortiori* trù mật trong $U$. Khi đó $U$ là bất khả quy (Mệnh đề 1).

(ii) Hãy chứng minh rằng, với mọi tập mở khác rỗng $V$ trong $X$, $V \cap U_\alpha \neq \emptyset$ với mọi $\alpha \in A$: suy ra rằng $V \cap U_\alpha$ trù mật trong $U_\alpha$, theo giả thiết, do đó $V$ trù mật trong $X$ và điều này chứng minh rằng $X$ là bất khả quy (Mệnh đề 1). Bây giờ tồn tại ít nhất một chỉ số $y$ sao cho $V \cap U_y \neq \emptyset$; vì $U_\alpha \cap U_y \neq \emptyset$ với mọi $\alpha$ và $V \cap U_y$ trù mật trong $U_y$, $U_y \cap V \neq \emptyset$ và *a fortiori* $U_y \cap V \neq \emptyset$, điều này hoàn tất chứng minh của (ii).

#### Mệnh đề 4 {#ac-ii-s4-prop-4 .statement}

*Cho $X$ và $Y$ là hai không gian tôpô và $f$ là một ánh xạ liên tục từ $X$ vào $Y$. Với mọi tập con bất khả quy $E$ của $X$, $f(E)$ là một tập con bất khả quy của $Y$.*

Nếu $U, V$ là hai tập mở của $Y$ giao với $f(E)$, thì $f^{-1}(U)$ và $f^{-1}(V)$ là các tập mở của $X$ giao với $E$. Do đó, $f^{-1}(U) \cap f^{-1}(V) = f^{-1}(U \cap V)$ giao với $E$, điều này kéo theo rằng $U \cap V$ giao với $f(E)$ và chứng minh mệnh đề.

#### Định nghĩa 2 {#ac-ii-s4-def-2 .statement}

*Mọi tập con bất khả quy cực đại của một không gian tôpô $X$ được gọi là một thành phần bất khả quy của $X$.*

Suy ra từ Mệnh đề 2 rằng mọi thành phần bất khả quy của $X$ đều *đóng* trong $X$.

#### Mệnh đề 5 {#ac-ii-s4-prop-5 .statement}

*Cho $X$ là một không gian tôpô. Mọi tập con bất khả quy của $X$ đều được chứa trong một thành phần bất khả quy của $X$ và $X$ là hợp của các thành phần bất khả quy của nó.*

Để chứng minh mệnh đề đầu tiên, chỉ cần, nhờ Bổ đề Zorn, chứng minh rằng tập hợp 3 các tập con bất khả quy của $X$ là *quy nạp*. Cho $\mathcal{G}$ là một tập con của $\mathfrak{S}$ được sắp thứ tự toàn phần bởi phép bao hàm; ta chứng minh rằng hợp $E$ của các tập hợp $F \in \mathcal{G}$ là bất khả quy. Cho $U, V$ là hai tập mở của $X$ giao với $E$; vì $\mathcal{G}$ được sắp thứ tự toàn phần, tồn tại một tập hợp $F \in \mathcal{G}$ giao với $U$ và $V$; vì $F$ là bất khả quy, $U \cap V$ giao với $F$ và do đó cũng giao với $E$, điều này chứng minh rằng $E$ là bất khả quy và do đó 3 là quy nạp. Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất, vì mọi tập con của $X$ gồm một điểm duy nhất đều là bất khả quy.

#### Hệ quả {#ac-ii-s4-n1-cor-1 .statement}

*Mọi thành phần liên thông của một không gian tôpô $X$ là một hợp của các thành phần bất khả quy của $X$.*

Mọi không gian con bất khả quy của $X$ đều là liên thông theo Mệnh đề 1 và do đó được chứa trong một thành phần liên thông của $X$.

Chú ý rằng hai thành phần bất khả quy phân biệt của $X$ có thể có các điểm chung (Bài tập 11).

#### Mệnh đề 6 {#ac-ii-s4-prop-6 .statement}

*Cho $X$ là một không gian tôpô và $(P_i)_{1 \leq i \leq n}$ là một phủ hữu hạn của $X$ gồm các tập đóng bất khả quy. Khi đó các thành phần bất khả quy của $X$ là các phần tử cực đại (đối với phép bao hàm) của tập hợp các $P_i$.*

Ta có thể tự giới hạn vào trường hợp không có hai $P_i$ nào so sánh được. Nếu $E$ là một tập con bất khả quy của $X$, thì $E \subset \bigcup_{i=1}^n P_i$, và do đó $E$ được chứa trong một trong các tập đóng $P_i$; điều này chứng minh rằng các $P_i$ là các tập con bất khả quy cực đại duy nhất của $X$.

#### Hệ quả {#ac-ii-s4-n1-cor-2 .statement}

*Cho $X$ là một không gian tôpô và $E$ là một không gian con chỉ có một số hữu hạn các thành phần bất khả quy phân biệt $Q_i$ ($1 \leq i \leq n$); khi đó các thành phần bất khả quy của bao đóng $\overline{E}$ trong $X$ là các bao đóng $\overline{Q}_i$ của các $Q_i$ ($1 \leq i \leq n$) và $\overline{Q}_i \# \overline{Q}_j$ với $i \neq j$.*

$\overline{E}$ là hợp của các $\overline{Q}_i$, là các tập bất khả quy (Mệnh đề 2); vì $Q_i$ là đóng trong $E$, $\overline{Q}_i \cap E = Q_i$; vì $Q_i \notin Q_j$ với $i \neq j$, $\overline{Q}_i \notin \overline{Q}_j$, do đó hệ quả theo Mệnh đề 6.

#### Nhận xét {#ac-ii-s4-n1-rem-1 .statement}

Giả sử rằng $X$ chỉ có một số hữu hạn các thành phần bất khả quy phân biệt $X_i$ ($1 \leq i \leq n$); khi đó $U_+ = \mathbf{C}(\bigcup_{j \neq i} X_j)$ là mở trong $X$ và trù mật trong $X_i$ vì $X_i \notin \bigcup_{j \neq i} X_j$; do đó các $U_i$ ($1 \leq i \leq n$) là các tập hợp mở không rỗng của $X$ bất khả quy (Mệnh đề 2), rời nhau từng đôi một và có hợp trù mật trong $X$.

#### Mệnh đề 7 {#ac-ii-s4-prop-7 .statement}

*Cho $U$ là một tập hợp con mở của một không gian tôpô $X$. Ánh xạ $V \mapsto \overline{V}$ (phần đóng trong $X$) là một song ánh từ tập hợp các tập hợp con bất khả quy của $U$ đóng trong $U$ lên tập hợp các tập hợp con bất khả quy của $X$ đóng trong $X$ và gặp $U$; song ánh ngược là $Z \mapsto Z \cap U$. Đặc biệt, song ánh này ánh xạ tập hợp các thành phần bất khả quy của $U$ lên tập hợp các thành phần bất khả quy của $X$ gặp $U$.*

Nếu $V$ đóng trong $U$ và bất khả quy, thì $\overline{V}$ bất khả quy (Mệnh đề 2) và $V = \overline{V} \cap U$. Ngược lại, nếu $Z$ bất khả quy và đóng trong $X$ và gặp $U$, thì $Z \cap U$ là một tập hợp con mở không rỗng của $Z$, do đó bất khả quy (Mệnh đề 3) và trù mật trong $Z$ và, vì $Z$ đóng, $Z = \overline{Z} \cap U$. Điều này chứng minh mệnh đề.

### 2. CÁC KHÔNG GIAN TÔPÔ NOETHER

#### Định nghĩa 3 {#ac-ii-s4-def-3 .statement}

Một không gian tôpô $X$ được gọi là Noether nếu mọi tập hợp không rỗng các tập hợp con đóng của $X$, có thứ tự bởi phép bao hàm, đều có một phần tử cực tiểu.

Điều này tương đương với việc nói rằng mọi tập hợp không rỗng các tập hợp con mở của $X$, có thứ tự bởi phép bao hàm, đều có một phần tử cực đại, hoặc mọi dãy giảm (tương ứng tăng) các tập hợp đóng (tương ứng mở) đều dừng (Lý thuyết tập hợp, Chương 111, § 6, no. 5, Mệnh đề 6).

#### Mệnh đề 8 {#ac-ii-s4-prop-8 .statement}

(i) Mọi không gian con của một không gian Noether đều là Noether.
(ii) Cho $(A_i)_{i \in I}$ là một phủ hữu hạn của một không gian tôpô $X$. Nếu các không gian con $A_i$ của $X$ là Noether, thì $X$ là Noether.

(i) Cho $X$ là một không gian Noether, $A$ là một không gian con của $X$ và $(F_i)$ là một dãy giảm các tập hợp con của $A$ đóng trong $A$; khi đó $F_i = \overline{F_n} \cap A$ và các phần đóng $\overline{F_n}$ của các $F_i$ trong $X$ tạo thành một dãy giảm các tập hợp con đóng của $X$. Vì dãy này dừng, nên dãy $(F_i)$ cũng dừng.

(ii) Cho $(G_n)_{n \geq 0}$ là một dãy giảm các tập con đóng của $X$; theo giả thiết, mỗi một trong các dãy $(G_n \cap A_i)_{n \geq 0}$ đều dừng. Vì $I$ là hữu hạn, tồn tại một số nguyên $n_0$ sao cho, với $n \geq n_0$, $G_n \cap A_i = G_{n_0} \cap A_i$, với mọi $i \in I$. Nhưng
$$
G_n = \bigcup_{i \in I} (G_n \cap A_i)
$$
và do đó dãy $(G_n)$ dừng và $X$ là Noether.

#### Mệnh đề 9 {#ac-ii-s4-prop-9 .statement}

Để một không gian tôpô $X$ là Noether, điều kiện cần và đủ là mọi tập mở trong $X$ đều quasi-compact.

Để chứng minh rằng điều kiện này là cần thiết, theo Mệnh đề 8, chỉ cần chứng minh rằng mọi không gian Noether $X$ là quasi-compact. Cho $(U_i)_{i \in I}$ là một phủ mở của $X$; tập hợp các hợp hữu hạn của các tập $U_i$ là khác rỗng và do đó nhận một phần tử cực đại $V = \bigcup_{i \in H} U_i$, trong đó $H$ là một tập con hữu hạn của $I$. Theo định nghĩa, $V \cup U_i = V$ với mọi $i \in I$ và do đó $V = X$.

Ngược lại, giả sử rằng mọi tập mở của $X$ đều quasi-compact và cho $(U_i)$ là một dãy tăng các tập con mở của $X$. Hợp $V$ của các $U_i$ là mở và do đó quasi-compact; vì $(U_i)$ là một phủ mở của $V$, tồn tại một họ con hữu hạn của $(U_i)$ là một phủ của $V$ và do đó $V = U_n$ với một chỉ số $n$ nào đó, điều này chứng minh rằng dãy $(U_i)$ dừng.

**Bổ đề 1 ("Nguyên lý quy nạp Noether").** *Cho E là một tập hợp có thứ tự mà mọi tập con khác rỗng của nó đều nhận một phần tử cực tiểu. Cho F là một tập con của E có tính chất sau: nếu $a \in E$ là sao cho quan hệ $x < a$ kéo theo $x \in F$, thì $a \in F$. Khi đó $F = E$.*

Giả sử $F \neq E$; khi đó $CF$ sẽ có một phần tử cực tiểu $b$. Theo định nghĩa, $x \in F$ với mọi $x < b$, điều này kéo theo rằng $b \in F$, là một mâu thuẫn.

#### Mệnh đề 10 {#ac-ii-s4-prop-10 .statement}

*Nếu X là một không gian Noether, tập hợp các thành phần bất khả quy của X (và a fortiori tập hợp các thành phần liên thông của X) là hữu hạn.*

Chỉ cần chứng minh rằng X là một hợp hữu hạn của các tập con đóng bất khả quy (no. **1**, Mệnh đề 6). Ta hãy chứng minh rằng nguyên lý quy nạp Noether có thể được áp dụng bằng cách lấy E là tập hợp các tập con đóng của X, có thứ tự bởi quan hệ bao hàm, và F là tập hợp các hợp hữu hạn của các tập con đóng bất khả quy. Cho Y là một tập con đóng của X sao cho mọi tập con đóng $\neq Y$ của Y đều thuộc F. Nếu Y là bất khả quy, thì $Y \in F$ theo định nghĩa; nếu không, Y là hợp của hai tập con đóng $Y_1,\ Y_2$ phân biệt với Y. Khi đó $Y_1 \in F$ và $Y_2 \in F$ theo giả thiết, do đó $Y \in F$ theo định nghĩa của F.

Đặc biệt, suy ra rằng một không gian Noether *Hausdorff* nhất thiết là *hữu hạn*.

### 3. PHỔ NGUYÊN TỐ CỦA MỘT VÀNH

Cho A là một vành và X là tập hợp các iđêan nguyên tố của A. Với mọi tập con M của A, ta ký hiệu $V(M)$ là tập hợp các iđêan nguyên tố của A chứa M; rõ ràng, nếu $a$ là iđêan của A sinh bởi M, thì $V(M) = V(a)$; nếu M gồm một phần tử duy nhất f, ta viết $V(f)$ thay cho $V(\{f\})$ và ta có $V(f) = V(Af)$. Ánh xạ $M \mapsto V(M)$ là *giảm* đối với quan hệ bao hàm trong A và X. Hơn nữa, các công thức sau đây đúng:

(1)
$$
V(0) = X, \quad V(1) = O;
$$

(2)
$$
V\left(\bigcup_{i \in I} M_i\right) = V\left(\sum_{i \in I} M_i\right) = \bigcap_{i \in I} V(M_i)
$$
với mọi họ $(M_i)_{i \in I}$ các tập con của A;

(3)
$$
V(a \cap a') = V(aa') = V(a) \cup V(a')
$$
với mọi cặp iđêan $a,\ a'$ trong A. Các công thức (1) và (2) là hiển nhiên; mặt khác, công thức (3) có nghĩa là, để một iđêan nguyên tố $p$ của A chứa một trong các iđêan $a$ hoặc $a'$, thì điều kiện cần và đủ là nó chứa $aa'$ hoặc nó chứa $a \cap a'$; khi đó nó là một hệ quả của § 1, no. 1, Mệnh đề 1. Công thức thứ hai (1) có đảo lại sau đây: nếu $a$ là một iđêan của $A$ sao cho $V(a) = \varnothing$, thì $a = A$, vì không có iđêan cực đại nào của $A$ chứa $a$. Cuối cùng, nếu $a$ là một iđêan của $A$ và $r(a)$ là căn của nó ($§ 2$, no. 6, Định nghĩa 4), thì

$$
V(a) = V(r(a))
$$

suy ra từ $§ 2$, no. 6, Hệ quả 1 của Mệnh đề 13.

Các công thức (1) đến (3) chỉ ra rằng các tập con $V(M)$ của $X$ thỏa mãn các tiên đề *tập đóng* của một tôpô (*Tôpô đại cương*, Chương I, $§ 1$, no. 4).

#### Định nghĩa 4 {#ac-ii-s4-def-4 .statement}

*Cho $A$ là một vành. Tập hợp $X$ các iđêan nguyên tố của $A$, với tôpô mà các tập đóng là các tập hợp $V(M)$, trong đó $M$ chạy qua $\mathfrak{P}(A)$, được gọi là phổ nguyên tố của $A$ và được ký hiệu bởi $\mathrm{Spec}(A)$. Tôpô được xác định như vậy được gọi là tôpô phổ hoặc tôpô Zariski trên $X$.*

Rõ ràng quan hệ $\mathrm{Spec}(A) = \varnothing$ là tương đương với $A = \{0\}$.

Cho $X$ là phổ nguyên tố của một vành $A$; với mọi $f \in A$, ký hiệu $X_f$ là tập hợp các iđêan nguyên tố của $A$ *không chứa* $f$; khi đó $X_f = X - V(f)$ và do đó $X_f$ là một tập hợp *mở*. Theo (2), mọi tập con đóng của $X$ là một giao của các tập đóng có dạng $V(f)$ và do đó các $X$, tạo thành một *cơ sở* của tôpô phổ trên $X$. Hơn nữa, suy ra ngay lập tức từ các định nghĩa rằng

$$
X_0 = O,\quad X_1 = X,
$$

và nói chung $X_{f^{-1}} = X$ với mọi phần tử khả nghịch $f$ của $A$;

$$
X_{g^{-1}} = X, nX, \quad \text{cho mọi } f, g \text{ trong } A.
$$

Với mỗi tập con $Y$ của $X$, ta ký hiệu bởi $\mathfrak{J}(Y)$ giao của các iđêan nguyên tố của $A$ thuộc $Y$. Rõ ràng $\mathfrak{J}(Y)$ là một iđêan của $A$ và ánh xạ $Y \mapsto \mathfrak{J}(Y)$ là *giảm* đối với quan hệ bao hàm trong $X$ và $A$. Rõ ràng các quan hệ

$$
\mathfrak{J}(\varnothing) = A
$$
$$
\mathfrak{J}\left( \bigcup_{\lambda \in L} Y_\lambda \right) = \bigcap_{\lambda \in L} \mathfrak{J}(Y_\lambda)
$$

đúng với mọi họ $(Y_\lambda)_{\lambda \in L}$ các tập con của $X$. Hơn nữa:

#### Mệnh đề 11 {#ac-ii-s4-prop-11 .statement}

*Cho $A$ là một vành, $a$ là một iđêan của $A$ và $Y$ là một tập con của $X = \mathrm{Spec}(A)$.
(i) $V(a)$ là đóng trong $X$ và $\mathfrak{J}(Y)$ là một iđêan của $A$ bằng căn của nó.
(ii) $\mathfrak{J}(V(a))$ *là căn của* $a$ *và* $V(\mathfrak{J}(Y))$ *là bao đóng của* $Y$ *trong* $X$.*

(iii) Các ánh xạ 3 và V xác định các song ánh giảm, trong đó một ánh xạ là nghịch đảo của ánh xạ kia, giữa tập hợp các tập con đóng của X và tập hợp các iđêan của A bằng căn của chúng.

Mệnh đề (i) và mệnh đề đầu tiên của (ii) suy ra từ các định nghĩa và § 2, no. 6, Hệ quả 1 của Mệnh đề 13. Nếu một tập đóng V(M) (với một M ⊂ A nào đó) chứa Y, thì M ⊂ p với mọi iđêan nguyên tố p ∈ Y, do đó M ⊂ J(Y) và vì thế V(M) ⊃ V(J(Y)); vì Y ⊂ V(J(Y)), V(J(Y)) là tập đóng nhỏ nhất của X chứa Y, điều này hoàn thành chứng minh của (ii). Cuối cùng, suy ra từ (ii) rằng, nếu a là một iđêan nguyên tố bằng căn của nó, thì J(V(a)) = a và rằng, nếu Y là đóng trong X, thì V(J(Y)) = Y; điều này chứng minh (iii).

Suy ra ngay lập tức từ Mệnh đề 11 rằng, nếu M là một tập con bất kỳ của A và Y là một tập con bất kỳ của X, thì V(M) = V(J(V(M))) và J(Y) = J(V(J(Y))).

#### Hệ quả 1 {#ac-ii-s4-prop-11-cor-1 .statement}

Với mọi họ (Y_λ)_{λ ∈ L} các tập con đóng của X, J(∩_{λ ∈ L} Y_λ) là căn của tổng các iđêan J(Y_λ).

Suy ra từ Mệnh đề 11 (iii) rằng J(∩_{λ ∈ L} Y_λ) là iđêan nhỏ nhất bằng căn của nó và chứa tất cả các J(Y_λ); iđêan này khi đó chứa ∑_{λ ∈ L} J(Y_λ) và do đó cũng chứa căn của ∑_{λ ∈ L} J(Y_λ) (§ 2, no. 6, Hệ quả 2 của Mệnh đề 13), do đó có hệ quả.

#### Hệ quả 2 {#ac-ii-s4-prop-11-cor-2 .statement}

Gọi r(a) là căn của một iđêan a của A; nếu a và b là hai iđêan của A, quan hệ V(a) ⊂ V(b) tương đương với b ⊂ r(a) và r(b) ⊂ r(a).

Rõ ràng ngay lập tức rằng các quan hệ b ⊂ r(a) và r(b) ⊂ r(a) là tương đương và, do V(a) = V(r(a)), hệ quả suy ra ngay lập tức từ Mệnh đề 11, (iii).

#### Hệ quả 3 {#ac-ii-s4-prop-11-cor-3 .statement}

Cho (f_λ)_{λ ∈ L} là một họ các phần tử của A. Để một phần tử g ∈ A thỏa mãn X_g ⊂ ∪_{λ ∈ L} X_{f_λ}, điều kiện cần và đủ là tồn tại một số nguyên n > 0 sao cho g^n thuộc iđêan sinh bởi các f_λ.

Quan hệ X_g ⊂ ∪_{λ ∈ L} X_{f_λ} tương đương với V(g) ⊃ ∩_{λ ∈ L} V(f_λ) và chỉ cần áp dụng Hệ quả 2.

Hệ quả 4, Để hai phần tử f, g của A thỏa mãn X_f = X_g, điều kiện cần và đủ là tồn tại hai số nguyên m > 0, n > 0 sao cho f^m ∈ Ag và g^n ∈ Af.

#### Hệ quả 5 {#ac-ii-s4-prop-11-cor-5 .statement}

Để $f \in A$ thỏa mãn $X_f = \varnothing$, điều kiện cần và đủ là $f$ lũy linh.

Điều này suy ra ngay lập tức từ Hệ quả 4.

#### Hệ quả 6 {#ac-ii-s4-prop-11-cor-6 .statement}

Bao đóng của một tập gồm một điểm $p \in X = \mathrm{Spec}(A)$ là tập $V(p)$ gồm các iđêan nguyên tố chứa $p$. Để tập $\{p\}$ là đóng trong $X$ (hay, như ta cũng sẽ nói bằng một sự lạm dụng ngôn ngữ, để $p$ là một điểm đóng của $X$), điều kiện cần và đủ là $p$ cực đại.

#### Hệ quả 7 {#ac-ii-s4-prop-11-cor-7 .statement}

Nếu $A$ là một vành Noether, $X = \mathrm{Spec}(A)$ là một không gian Noether.

#### Mệnh đề 12 {#ac-ii-s4-prop-12 .statement}

Với mọi $f \in A$, tập mở $X_f$ trong $X = \mathrm{Spec}(A)$ là quasi-compact; đặc biệt, không gian $X$ là quasi-compact.

Vì các $X_g$ tạo thành một cơ sở của tôpô, chỉ cần chứng minh rằng, nếu $(g_\lambda)_{\lambda \in L}$ là một họ các phần tử của $A$ sao cho $X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda}$, thì tồn tại một họ con hữu hạn $(g_{\lambda_i})_{i \in I}$ sao cho $X_f = \bigcup_{i \in I} X_{g_{\lambda_i}}$. Nhưng quan hệ $X_f = \bigcup_{\lambda \in L} X_{g_\lambda}$ có nghĩa là tồn tại một số nguyên $n > 0$ và một họ con hữu hạn $(g_{\lambda_i})_{i \in I}$ sao cho "f" thuộc iđêan sinh bởi họ con đó (Hệ quả 3 của Mệnh đề 11); do đó có mệnh đề.

#### Mệnh đề 13 {#ac-ii-s4-prop-13 .statement}

Cho $A, A'$ là hai vành, $X = \mathrm{Spec}(A), X' = \mathrm{Spec}(A')$ và $h$ là một đồng cấu từ $A$ đến $A'$; ánh xạ $^a h : p' \mapsto \overline{h}(p')$ từ $X'$ đến $X$ là liên tục.

Với $M \subset A$, tập hợp $(^a h)^{-1}(V(M))$ là tập hợp các iđêan nguyên tố $p'$ của $A'$ sao cho $M \subset \overline{h}(p')$, điều này tương đương với $h(M) \subset p'$; tập hợp này khi đó bằng $V(h(M))$ và do đó là đóng.

Ta gọi $^a h$ là ánh xạ liên kết với đồng cấu $h$.

#### Nhận xét {#ac-ii-s4-n3-rem-1 .statement}

Nếu $h$ là toàn ánh và $a$ là hạt nhân của nó, từ định nghĩa của tôpô phổ suy ra rằng $^a h$ là một đồng phôi từ $X'$ lên không gian con đóng $V(a)$ của $X$; để một iđêan nguyên tố $p'$ của $A'$ chứa một iđêan $b'$ của $A'$, điều kiện cần và đủ là $\overline{h}(p')$ chứa $\overline{h}(b')$; trước hết ta thấy rằng $^a h$ là đơn ánh bằng cách lấy $b'$ là nguyên tố; hơn nữa, với mọi iđêan $b'$ của $A'$, ảnh theo $^a h$ của $V(b')$ là $V(\overline{h}(b'))$, do đó là mệnh đề của chúng ta, các iđêan có dạng $\overline{h}(b')$ đều là các iđêan của $A$ chứa $a$.

#### Hệ quả {#ac-ii-s4-n3-cor-1 .statement}

Cho $S$ là một tập con nhân của $A$, $A' = S^{-1}A$ và $h$ là đồng cấu chính tắc $i_A^S$; khi đó $^a h$ là một đồng phôi từ $X' = \mathrm{Spec}(A')$ lên không gian con của $X = \mathrm{Spec}(A)$ gồm các iđêan nguyên tố của $A$ không giao với $S$.

#### Mệnh đề 14 {#ac-ii-s4-prop-14 .statement}

*Cho $A$ là một vành. Để một tập con $Y$ của $X = \mathrm{Spec}(A)$ là bất khả quy, điều kiện cần và đủ là iđêan $\mathfrak{J}(Y)$ là nguyên tố.*

Viết $p = \mathfrak{J}(Y)$, ta chú ý rằng, đối với một phần tử $f \in A$, quan hệ $f \in p$ tương đương với $Y \subset V(f)$. Giả sử rằng $Y$ là bất khả quy và cho $f, g$ là các phần tử của $A$ sao cho $fg \in p$. Khi đó
$$
Y \subset V(fg) = V(f) \cup V(g);
$$
vì $Y$ là bất khả quy và $V(f)$ và $V(g)$ là đóng, nên $Y \subset V(f)$ hoặc $Y \subset V(g)$, do đó $f \in p$ hoặc $g \in p$, điều này chứng minh rằng $p$ là nguyên tố.

Bây giờ giả sử rằng $p$ là nguyên tố; khi đó $\overline{Y} = V(p)$ (Mệnh đề 11 (ii)) và, vì $p$ là nguyên tố, $p = \mathfrak{J}(\{p\})$, do đó $\overline{Y} = V(\mathfrak{J}(\{p\})) = \{p\}$ (Mệnh đề 11 (ii)). Vì một tập hợp gồm một điểm duy nhất là bất khả quy, nên $Y$ là bất khả quy (no. 1, Mệnh đề 2).

#### Hệ quả 1 {#ac-ii-s4-prop-14-cor-1 .statement}

*Để một vành $A$ có tính chất $X = \mathrm{Spec}(A)$ là bất khả quy, điều kiện cần và đủ là thương của $A$ theo căn nil của nó $\mathfrak{N}$ là một miền nguyên.*

Theo Mệnh đề 11 (i), $\mathfrak{J}(X)$ là căn của iđêan $(0)$, tức là $\mathfrak{N}$.

#### Hệ quả 2 {#ac-ii-s4-prop-14-cor-2 .statement}

*Ánh xạ $p \mapsto V(p)$ là một song ánh của $X = \mathrm{Spec}(A)$ lên tập hợp các tập con đóng bất khả quy của $X$; đặc biệt các thành phần bất khả quy của một tập con đóng $Y$ của $X$ là các tập hợp $V(p)$, trong đó $p$ chạy qua tập hợp các phần tử cực tiểu của tập hợp các iđêan nguyên tố của $A$ chứa $\mathfrak{J}(Y)$.*

Vì $\mathfrak{J}(V(p)) = p$ đối với mọi iđêan nguyên tố $p$ của $A$ và $Y = V(\mathfrak{J}(Y))$ đối với mọi tập con đóng $Y$ của $X$, mệnh đề đầu tiên suy ra từ Mệnh đề 14; mặt khác, đối với $Y \supset V(p)$, điều kiện cần và đủ là
$$
p = \mathfrak{J}(V(p)) \supset \mathfrak{J}(Y)
$$
(Mệnh đề 11), do đó có mệnh đề thứ hai.

#### Hệ quả 3 {#ac-ii-s4-prop-14-cor-3 .statement}

*Tập hợp các iđêan nguyên tố cực tiểu của một vành Noether $A$ là hữu hạn.*

$X = \mathrm{Spec}(A)$ chỉ có một số hữu hạn các thành phần bất khả quy (Hệ quả 7 của Mệnh đề 11 và no. 2, Mệnh đề 10) và hệ quả suy ra từ Hệ quả 2 ở trên.

#### Mệnh đề 15 {#ac-ii-s4-prop-15 .statement}

Cho $A$ là một vành, $I$ là một tập hợp hữu hạn và $E$ là tập hợp các họ trực giao $(e_i)_{i \in I}$ của các phần tử lũy đẳng $e_i \neq 0$ của $A$ sao cho $\sum_{i \in I} e_i = 1$. Với mọi $(e_i)_{i \in I} \in E$, ta đặt $\overline{\omega}((e_i)_{i \in I}) = (\mathrm{V}(A(1 - e_i)))_{i \in I}$, $\sigma((e_i)_{i \in I}) = (Ae_i)_{i \in I}$. Khi đó $\overline{\omega}$ là một song ánh của $E$ lên tập hợp $P$ các phân hoạch $(U_i)_{i \in I}$ của $X = \mathrm{Spec}(A)$ thành các tập hợp mở và $\sigma$ là một song ánh của $E$ lên tập hợp $S$ các họ $(a_i)_{i \in I}$ các iđêan $\neq 0$ của $A$ sao cho $A$ là tổng trực tiếp của các $a_i$.

Cho $(e_i)_{i \in I}$ là một phần tử của $E$ và đặt $Y_i = \mathrm{V}(A(1 - e_i))$; nếu $i \neq j$, thì $1 = 1 - e_i + e_i(1 - e_j) \in A(1 - e_i) + A(1 - e_j)$, do đó $Y_i \cap Y_j = \varnothing$ (các công thức (1) và (2)). Mặt khác,

$$
\bigcup_{i \in I} Y_i = \mathrm{V}\left( \prod_{i \in I} A(1 - e_i) \right)
$$

(công thức (3));

theo giả thiết $\prod_{i \in I} (1 - e_i) = 1 - \sum_{i \in I} e_i = 0$, do đó $\bigcup_{i \in I} Y_i = X$ (công thức (I)). Vì các $Y_i$ là đóng, chúng cũng là mở, do đó $\overline{\omega}(E) \subset P$. Ngoài ra, hiển nhiên $A = \sum_{i \in I} Ae_i$; nếu $0 = \sum_{i \in I} a_i e_i$ trong đó $a_i \in A$, ta thu được, bằng cách nhân với $e_i$, $O = a_i e_i^2 = a_i e_i$ với mọi $i$; điều này chứng minh rằng $\sigma(E) \subset S$.

#### Bổ đề 2 {#ac-ii-s4-lem-2 .statement}

*Nếu* $e, f$ *là hai phần tử lũy đẳng của* $A$ *sao cho* $Ae$ *và* $Af$ *có cùng căn* *thì* $e = f$.

Theo giả thiết, tồn tại các số nguyên $m \geq 0, n \geq 0$ sao cho $e = e^m \in Af$ và $f = f^n \in Ae$; gọi $x, y$ là các phần tử của $A$ sao cho $e = xf, f = ye$; khi đó $ef = x^2 = x = e$ và tương tự $ef = ye^2 = ye = f$, do đó $e = f$.

Bổ đề 2 và Hệ quả 2 của Mệnh đề 11 cho thấy các ánh xạ $\overline{\omega}$ và $\sigma$ là *đơn ánh*.

Chúng ta hãy chỉ ra rằng $\sigma$ là toàn ánh. Nếu $(a_i)_{i \in I}$ là một phần tử của $S$, thì có các phần tử $e_i \in a_i$ sao cho $1 = \sum_{i \in I} e_i$; nếu $i \neq j$, thì $e_i e_j \in a_i \cap a_j = \{0\}$, do đó

$$
e_i = \sum_{j \in I} e_i e_j = e_i^2;
$$

cuối cùng, $Ae_i \subset a_i$, với mọi $i \in I$ và $\sum_{i \in I} Ae_i = A$, do đó $Ae_i = a_i$.

Còn lại là chứng minh rằng $\overline{\omega}$ là toàn ánh. Cho $(U_i)_{i \in I}$ là một phần tử của $P$ và đặt $Z_i = \bigcup_{j \neq i} U_j$; vì $U_i$ và $Z_i$ là đóng, tồn tại các iđêan $a_i, b_i$ của $A$ sao cho $U_i = \mathrm{V}(a_i), Z_i = \mathrm{V}(b_i)$. Bây giờ ta chỉ ra rằng có thể giả sử thêm rằng $a_i \cap b_i = 0$. Do $U_i \cap Z_i = \varnothing$, nên $a_i + b_i = A$; hãy lấy $a_i, b_i \in a_i, b_i$ sao cho $a_i + b_i = 1$. Khi đó $X = U_i \cup Z_i = \mathrm{V}(a_i b_i)$ (công thức (3)); do đó mọi phần tử của $a_i b_i$ là lũy linh (Hệ quả 2 của Mệnh đề 11); lấy $p$ là một số nguyên sao cho $a_i^p b_i^p = 0$. Khi đó $U_i \subset \mathrm{V}(Aa_i) = \mathrm{V}(Aa_i^p)$,

$$
Z_i \subset \mathrm{V}(Ab_i) = \mathrm{V}(Ab_i^p)
$$

và $V(Aa_i) \cap V(Ab_i) = V(Aa_i + Ab_i) = \varnothing$, do đó $U_i = V(Aa_i^p)$ và $Z_i = V(Ab_i^p)$, điều này xác lập mệnh đề của chúng ta bằng cách thay thế $a_i$ bởi $Aa_i^p$ và $b_i$ bởi $Ab_i^p$. Với các iđêan $a_i$ và $b_i$ được chọn như vậy, suy ra từ việc $\sigma$ là song ánh rằng tồn tại hai phần tử lũy đẳng $f_i \in a_i, e_i \in b_i$ sao cho $1 = e_i + f_i, e_i f_i = 0, a_i = Af_i, b_i = Ae_i$. Nếu $i \neq j$, thì $X = Z, \cup Z_j = V(Ae_i e_j)$, và vì $e_i e_j$ là lũy đẳng, Bổ đề 2 chỉ ra rằng $e_i e_j = 0$. Cuối cùng $e = \sum_{i \in I} e_i$ là lũy đẳng và $e_i \in Ae$ với mọi $i \in I$, do đó $V(Ae) \subset Z$, với mọi $i$; suy ra rằng

$$
V(Ae) = \varnothing = V(A.1)
$$

và Bổ đề 2 cũng chỉ ra rằng $e = 1$.

#### Hệ quả 1 {#ac-ii-s4-lem-2-cor-1 .statement}

Cho $A$ là một vành, $r$ là một iđêan nil của $A$ và $h : A \to A/r$ là đồng cấu chính tắc. Với mọi họ trực giao hữu hạn $(e'_i)_{i \in I}$ các phần tử lũy đẳng của $A/r$ sao cho $\sum_{i \in I} e'_i = 1$, tồn tại một họ trực giao hữu hạn $(e_i)_{i \in I}$ các phần tử lũy đẳng của $A$ sao cho $\sum_{i \in I} e_i = 1$ và $h(e_i) = e'_i$ với mọi $i \in I$.

Ta viết $A' = A/r$. Ta biết (Nhận xét sau Mệnh đề 13) rằng

$$
ah : \operatorname{Spec}(A') \to \operatorname{Spec}(A)
$$

là một phép đồng phôi, mọi iđêan nguyên tố của $A$ chứa $r$ theo giả thiết. Mệnh đề 15 chỉ ra rằng tồn tại trong $A$ một họ trực giao hữu hạn $(e_i)_{i \in I}$, gồm các phần tử lũy đẳng sao cho $\sum_{i \in I} e_i = 1$ và ảnh qua $ah$ của $V(A'(1 - e'_i))$ là $V(A(1 - e_i))$. Nhưng rõ ràng $V(A(1 - e_i))$ cũng là ảnh qua $ah$ của

$$
V(A'(1 - h(e'_i)));
$$

vì $1 - e'_i$ và $1 - h(e_i)$ là lũy đẳng, Bổ đề 2 chỉ ra rằng $e'_i = h(e_i)$, do đó hệ quả.

#### Hệ quả 2 {#ac-ii-s4-lem-2-cor-2 .statement}

Để phổ nguyên tố $X = \operatorname{Spec}(A)$ của một vành $A$ là liên thông, điều kiện cần và đủ là $A$ không chứa phần tử lũy đẳng nào khác $0$ và $1$.

Nói rằng $X$ không liên thông có nghĩa là tồn tại trong $X$ một tập hợp vừa mở vừa đóng và phân biệt với $\varnothing$ và $X$.

### 4. GIÁ ĐỠ CỦA MỘT MÔĐUN

#### Định nghĩa 5 {#ac-ii-s4-def-5 .statement}

Cho $A$ là một vành và $M$ là một $A$-môđun. Tập hợp các iđêan nguyên tố $p$ của $A$ sao cho $M_p \neq 0$ được gọi là giá đỡ của $M$ và được ký hiệu bởi $\operatorname{Supp}(M)$.

Vì mọi iđêan cực đại của $A$ đều là nguyên tố, nên suy ra ngay lập tức từ § 3, no. 3, Hệ quả 2 của Định lý 1, rằng để $A$-môđun $M$ bằng $0$, điều kiện cần và đủ là $\operatorname{Supp}(M) = \varnothing$.

#### Ví dụ {#ac-ii-s4-n4-exa-1 .statement}

Cho $a$ là một iđêan của $A$; theo ký hiệu của no. 3, ta có
$$
V(a) = \operatorname{Supp}(A/a).
$$
Nếu $p$ là một nguyên tố của $A$ sao cho $a \notin p$, thì $(A/a)_p = 0$ (§ 3, no. 1, Nhận xét 3); nếu ngược lại $a \subset p$, $aA_p$ được chứa trong iđêan cực đại $pA_p$ của $A$, và $(A/a)_p$ là đẳng cấu với $A_p/aA_p$ và do đó là khác không (§ 3, no. 1, Mệnh đề 3); do đó có mệnh đề của chúng ta.
Đặc biệt, $\operatorname{Supp}(A) = \operatorname{Spec}(A)$.

#### Mệnh đề 16 {#ac-ii-s4-prop-16 .statement}

Cho $A$ là một vành và $M$ là một $A$-môđun.
(i) *Nếu $N$ là một môđun con của $M$, thì*
$$
\operatorname{Supp}(M) = \operatorname{Supp}(N) \cup \operatorname{Supp}(M/N).
$$
(ii) *Nếu $M$ là tổng của một họ $(N_i)_{i \in I}$ các môđun con, thì*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(N_i).
$$
(i) Từ dãy khớp $0 \to N \to M \to M/N \to 0$, ta suy ra, với mọi iđêan nguyên tố $p$ của $A$, dãy khớp
$$
0 \to N_p \to M_p \to (M/N)_p \to 0
$$
(§ 2, no. 4, Định lý 1). Đối với $M$, để được thu gọn về 0, điều kiện cần và đủ là $N_p$ và $(M/N)_p$ cũng như vậy. Nói cách khác, quan hệ $p \notin \operatorname{Supp}(M)$ tương đương với "p $\notin \operatorname{Supp}(N)$ và $p \notin \operatorname{Supp}(M/N)$", điều này chứng minh (i).
(ii) Với mọi iđêan nguyên tố $p$ của $A$, $M$, là tổng của họ các môđun con $(N_i)_p$ (§ 2, no. 4). Nói rằng $M, \neq 0$ có nghĩa là tồn tại $i \in I$ sao cho $(N_i)_p \neq 0$, do đó (ii).

#### Hệ quả {#ac-ii-s4-n4-cor-1 .statement}

*Cho $A$ là một vành, $M$ là một $A$-môđun, $(m_i)_{i \in I}$ là một hệ các phần tử sinh của $M$ và $a$, là linh hóa tử của $m_i$. Khi đó*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} V(a_i).
$$
$\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(Am_i)$ theo Mệnh đề 16 (ii). Mặt khác, $Am_i$ là đẳng cấu với $A$-môđun $A/a_i$ và ta đã thấy rằng
$$
\operatorname{Supp}(A/a_i) = V(a_i)
$$
(Ví dụ ở trên).

#### Mệnh đề 17 {#ac-ii-s4-prop-17 .statement}

*Cho $A$ là một vành, $M$ là một $A$-môđun và $a$ là linh hóa tử của nó; nếu $M$ là sinh hữu hạn, thì* $\operatorname{Supp}(M) = V(a)$ *và* $\operatorname{Supp}(M)$ *do đó là đóng trong* $\operatorname{Spec}(A)$.
Cho $(m_i)_{1 \leq i \leq n}$ là một hệ các phần tử sinh của $M$ và cho $a$, là linh hóa tử của $m_i$; khi đó $a = \bigcap_{i=1}^n a_i$, suy ra $V(a) = \bigcup_{i=1}^n V(a_i)$ (no. 3, phương trình (3)) và Mệnh đề suy ra từ Hệ quả của Mệnh đề 16.

#### Hệ quả 1 {#ac-ii-s4-prop-17-cor-1 .statement}

Cho $A$ là một vành, $M$ là một $A$-môđun sinh hữu hạn và $a$ là một phần tử của $A$. Để $a$ thuộc mọi iđêan nguyên tố của giá của $M$, điều kiện cần và đủ là phép vị tự của $M$ với tỉ số $a$ là lũy linh.

Suy ra từ Mệnh đề 17 rằng giao của các iđêan nguyên tố thuộc $\operatorname{Supp}(M)$ là căn của linh hóa tử $a$ của $M$ (no. 3, Mệnh đề 11 (ii)). Nói rằng $a$ thuộc căn này tương đương với nói rằng tồn tại một lũy thừa $a^k \in a$ và do đó $a^k M = 0$.

#### Hệ quả 2 {#ac-ii-s4-prop-17-cor-2 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn và $a$ là một iđêan của $A$. Để $\operatorname{Supp}(M) \subset V(a)$, điều kiện cần và đủ là tồn tại một số nguyên $k$ sao cho $a^k M = 0$.

Nếu $b$ là linh hóa tử của $M$, quan hệ $\operatorname{Supp}(M) \subset V(a)$ tương đương với $V(b) \subset V(a)$ theo Mệnh đề 17 và do đó tương đương với $a \subset r(b)$, trong đó $r(b)$ là căn của $b$ (no. 3, Hệ quả 2 của Mệnh đề 11). Vì $A$ là Noether, điều kiện này cũng tương đương với sự tồn tại của một số nguyên $k > 0$ sao cho $a^k \subset b$ (§ 2, no. 6, Mệnh đề 15).

#### Mệnh đề 18 {#ac-ii-s4-prop-18 .statement}

Cho $M, M'$ là hai môđun sinh hữu hạn trên một vành $A$; khi đó

$$
\operatorname{Supp}(M \otimes_A M') = \operatorname{Supp}(M) \cap \operatorname{Supp}(M').
$$

Ta cần chứng minh rằng, nếu $p$ là một iđêan nguyên tố của $A$, các quan hệ $(M \otimes_A M')_p \neq 0$ và "$M_p \neq 0$ và $M'_p \neq 0$" là tương đương. Vì các $A_p$-môđun $M, \otimes_{A_p} M'_p$ và $(M \otimes_A M')_p$ là đẳng cấu (§ 2, no. 7, Mệnh đề 18), mệnh đề của chúng ta suy ra từ bổ đề sau:

#### Bổ đề 3 {#ac-ii-s4-lem-3 .statement}

Cho $B$ là một vành địa phương và $E$ và $E'$ là hai $B$-môđun sinh hữu hạn. Nếu $E \neq 0$ và $E' \neq 0$, thì $E \otimes_B E' \neq 0$.

Cho $k$ là trường thặng dư của $B$. Theo § 3, no. 2, Mệnh đề 4, $k \otimes_B E \neq 0$ và $k \otimes_B E' \neq 0$; khi đó ta suy ra rằng

$$
(k \otimes_B E) \otimes_k (k \otimes_B E') \neq 0
$$

(Đại số, Chương II, § 3, no. 7). Nhưng, vì tích tenxơ là kết hợp (loc. cit., § 3, no. 8), tích tenxơ này đẳng cấu với

$$
E \otimes_B ((k \otimes_k k) \otimes_B E') = E \otimes_B (k \otimes_B E')
$$

và do đó với $k \otimes_B (E \otimes_B E')$, do đó có bổ đề.

#### Hệ quả {#ac-ii-s4-n4-cor-2 .statement}

Cho $M$ là một $A$-môđun sinh hữu hạn và $n$ là linh hóa tử của nó. Với mọi iđêan $a$ của $A$, $\operatorname{Supp}(M/aM) = V(a) \cap V(n) = V(a + n)$.

$M/aM = M \otimes_A (A/a)$ và $A/a$ là sinh hữu hạn.

#### Mệnh đề 19 {#ac-ii-s4-prop-19 .statement}

Cho $A, B$ là hai vành, $\phi : A \to B$ là một đồng cấu và
$$
^{a}\phi : \operatorname{Spec}(B) \to \operatorname{Spec}(A)
$$
là ánh xạ liên tục liên kết với $\phi$ (Mệnh đề 13). Với mọi $A$-môđun $M$,
$$
\operatorname{Supp}(M_{(B)}) \subset ^{a}\phi(\operatorname{Supp}(M)) ; \text{nếu cũng } M \text{ là sinh hữu hạn, thì}
$$
$$
\operatorname{Supp}(M_{(B)}) = ^{a}\phi^{-1}(\operatorname{Supp}(M)).
$$
Cho $q$ là một iđêan nguyên tố của $B$ và $p = \phi^{-1}(q)$. Giả sử rằng $q$ thuộc $\operatorname{Supp}(M_{(B)})$; khi đó $M_{(B)} \otimes_B B_q = (M \otimes_A B) \otimes_B B_q = M \otimes_A B_q = (M \otimes_A A_p) \otimes_A B_q$, vì đồng cấu $A \to B \to B_q$ phân tích thành $A \to A_p \to B_q$ (§ 2, no. 1, Mệnh đề 2); giả thiết $M_{(B)} \otimes_B B_q \neq 0$ kéo theo do đó $M \otimes_A A_q \neq 0$, do đó có mệnh đề thứ nhất. Vì đồng cấu $\phi_q : A_p \to B_q$ là địa phương, mệnh đề thứ hai suy ra từ bổ đề sau:

#### Bổ đề 4 {#ac-ii-s4-lem-4 .statement}

Cho $A, B$ là hai vành địa phương, $p : A \to B$ là một đồng cấu địa phương và $E$ là một $A$-môđun sinh hữu hạn. Nếu $E \neq 0$, thì $E_{(B)} \neq 0$.

Cho $m$ là iđêan cực đại của $A$ và $k = A/m$ là trường thặng dư; giả thiết kéo theo rằng $B \otimes_A k = B/mB \neq 0$; vì tích tenxơ là kết hợp, $(E \otimes_A B) \otimes_A k$ đẳng cấu với $E \otimes_A (B \otimes_A k)$, do đó cũng với $E \otimes_A (k \otimes_k (B \otimes_A k))$ và cuối cùng với $(E \otimes_A k) \otimes_k (B \otimes_A k)$; theo § 3, no. 2, Mệnh đề 4, $E \otimes_A k \neq 0$, do đó $(E \otimes_A B) \otimes_A k \neq 0$ (Đại số, Chương II, § 3, no. 7) và a fortiori $E \otimes_A B \neq 0$.

#### Mệnh đề 20 {#ac-ii-s4-prop-20 .statement}

Cho $A$ là một vành và $M$ là một $A$-môđun sinh hữu hạn. Với mọi iđêan nguyên tố $p \in \operatorname{Supp}(M)$, tồn tại một $A$-đồng cấu khác không $w : M \to A/p$.

Cho $p \in \operatorname{Supp}(M)$. Vì $M$ là sinh hữu hạn và $M_p \neq 0$,
$$
M_p/pM_p = M_p \otimes_A (A_p/pA_p) \neq 0
$$
(§ 3, no. 2, Mệnh đề 4). Cho $K = A_p/pA_p$ là trường các phân thức của miền nguyên $A/p$; vì $M_p/pM_p$ là một không gian vectơ trên $K$, không rút gọn về 0, nên tồn tại một dạng tuyến tính khác không $u : M_p/pM_p \to K$. Nếu $(x_i)_1 <_n^*$ là một hệ các phần tử sinh của $M$, $\bar{x}_i$ là ảnh của $x_i$, trong $(A/p)$-môđun $M_p/pM_p$, thì tồn tại một phần tử $\alpha \neq 0$ của $A/p$ sao cho các $\alpha u(\bar{x}_i)$ thuộc $A/p$ với $1 \leq i \leq n$; do đó $v = \alpha u$ là một ánh xạ tuyến tính $(A/p)$ khác không từ $M_p/pM_p$ đến $A/p$. Ánh xạ hợp thành
$$
w : M \longrightarrow M, \longrightarrow M_p/pM_p \overset{v}{\longrightarrow} A/p
$$
do đó là đồng cấu cần tìm.

### Bài tập {#ac-ii-s4-exercises}

(b) Cho $n = \dim(M)$. Các nhân tử trực tiếp của M có chiều 1 (tương ứng. $n - 1$) được gọi là các *đường thẳng* (tương ứng. các siêu phẳng). Một tự đẳng cấu $u \in \mathbf{GL}(M)$ phân biệt với tự đẳng cấu đồng nhất được gọi là một *phép xuyên* nếu tồn tại một siêu phẳng H của M mà mọi phần tử của nó đều bất biến dưới $u$; khi đó $u(x) = x + a\phi(x)$, trong đó $\phi$ là một dạng tuyến tính trên M sao cho $H = \mathrm{Ker}(\phi)$ và $a \in H$; hãy thu được đảo lại. Nếu A là giao hoán, hãy chứng minh rằng mọi tự đẳng cấu $u \in \mathbf{GL}(M)$ có định thức 1 là một tích của các phép xuyên (nhận xét rằng, trong ma trận của $u$ đối với bất kỳ cơ sở nào của M, mỗi cột chứa ít nhất một phần tử khả nghịch của A và một ma trận dạng $I + E_{ij} \ (i \neq j)$ là ma trận của một phép xuyên).

(c) Hãy cho một ví dụ về một tự đẳng cấu $u \in \mathbf{GL}(M)$ sao cho hạt nhân của $1 - u$ không là một nhân tử trực tiếp của M (lấy A là vành địa phương $K[[X]]$ của các chuỗi lũy thừa hình thức theo một biến bất định trên một trường K và $M = A$).

(d) Hãy cho một ví dụ về các nhân tử trực tiếp N, P của M (nhất thiết tự do) sao cho $N + P$ và $N \cap P$ không là các nhân tử trực tiếp của M. (Lấy $A = K[X]/(X^2)$, trong đó K là một trường và $M = A^2$.)

¶ 15. Cho A là một vành (giao hoán) và M là một A-môđun.

(a) Để một môđun con M' của M là thuần (Chương I, § 2, Bài tập 24), điều kiện cần và đủ là, với mọi iđêan cực đại $m$ của A, $M'_m$ là một môđun con thuần của $M_m$ (dùng Định lý 1 của no. 3).

(b) Giả sử A là một vành địa phương với iđêan cực đại $m$ và M là một A-môđun tự do sinh hữu hạn. Để một môđun con sinh hữu hạn M' của M là thuần, điều kiện cần và đủ là nó là một nhân tử trực tiếp của M. (Dùng Hệ quả 1 của Mệnh đề 5 của no. 2, quy về việc chứng minh rằng, nếu $M' \subset mM$, thì $M'$ chỉ có thể là một môđun con thuần của M khi $M' = 0$.)

16. Cho $(A_\lambda, f_{\mu\lambda})$ là một hệ trực tiếp các vành địa phương, sao cho các $f_{\mu\lambda}$ là các đồng cấu địa phương; gọi $m_\lambda$ là iđêan cực đại của $A_\lambda$ và $K_\lambda = A_\lambda/m_\lambda$. Khi đó $A = \varprojlim A_\lambda$ là một vành địa phương có iđêan cực đại là $m = \varprojlim m_\lambda$ và trường dư là $\bar{K} = \varprojlim K_\lambda$. Hơn nữa, nếu $m_\mu = A_\mu m_\lambda$ với $\lambda < \mu$, thì $m = Am$, với mọi $\lambda$.

94

Xem [các bài tập của § 4](exercises/s4/).
