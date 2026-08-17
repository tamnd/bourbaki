---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 5
section_title: Product of a family of sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 101-112, 127
pdf_pages: 0108-0119, 0134-0134
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE SET OF SUBSETS
      page: 101
      pdf_page: 108
    - "no": 2
      title: SET OF MAPPINGS OF ONE SET INTO ANOTHER
      page: 102
      pdf_page: 109
    - "no": 3
      title: DEFINITIONS OF THE PRODUCT OF A FAMILY OF SETS
      page: 103
      pdf_page: 110
    - "no": 4
      title: PARTIAL PRODUCTS
      page: 105
      pdf_page: 112
    - "no": 5
      title: ASSOCIATIVITY OF PRODUCTS OF SETS
      page: 106
      pdf_page: 113
    - "no": 6
      title: DISTRIBUTIVITY FORMULAE
      page: 107
      pdf_page: 114
    - "no": 7
      title: EXTENSION OF MAPPINGS TO PRODUCTS
      page: 111
      pdf_page: 118
statements: 24
exercises: 3
errata:
    - says: Proposition 1, Corollary 5
      read: Proposition 6, Corollary 1
      why: Section 5 prints five corollaries in no. 4 and all five stand under Proposition 6, which is on page 105 and is the auxiliary the no. announces with "it is enough to prove the following proposition". Proposition 1 has no corollary at all, so there is no Corollary 5 of it. The sentence citing this, on page 106, needs the projection of a product onto a factor to be surjective, and that is Corollary 1 of Proposition 6, whose proof reads "Apply Proposition 5 to the subset J = {alpha} of I".
    - says: Proposition 5, Corollary 2
      read: Proposition 6, Corollary 2
      why: The volume hangs these five corollaries on Proposition 5 four times over and on Proposition 6 once, and the page prints them under Proposition 6. The fact wanted in both sentences here, on pages 108 and 109, is that a product is empty exactly when one of its factors is, which is Corollary 2. Proposition 5 is the statement about a partial product that the proof of Corollary 1 applies, and it carries no corollary of its own.
    - says: Corollary 2 to Proposition 5
      read: Corollary 2 to Proposition 6
      why: The same reference as the two above, written the other way round on page 109, and wrong the same way.
content_sha256: cd433ae713305ca85d656e5b4b29f97421627479e3f0a3611bc85e328708df1d
translated_from: content/en/ens/II/05_s5_product_of_a_family_of_sets.md
source_content_sha256: ab63a5e5cc2acfa6050b72f3f3101a1a02b76af5e7ed1e3ff8a72602c1299fba
translation_model: gpt-5.4
translation_run: translate-vi-95bbd69b
glossary_version: 29
glossary_terms_sha256: e66ac54e0dc75e594253e7fec09147aa08ae13f063ddb9787fc092f3b7f211b6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. TÍCH CỦA MỘT HỌ TẬP HỢP

### 1. TIÊN ĐỀ CỦA TẬP HỢP CÁC TẬP CON

A4. $(\forall \mathrm{X}) \ \mathrm{Coll}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X}).$

Tiên đề này có nghĩa là với mọi tập hợp X đều tồn tại một tập hợp mà các phần tử của nó là tất cả các tập con của X, tức là tập hợp $\mathscr{E}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X})$ (§1, số 4); tập hợp này được ký hiệu bởi $\mathfrak{P}(\mathrm{X})$ và được gọi là *tập hợp các tập con của* X. Rõ ràng, nếu $\mathrm{X} \subset \mathrm{X}'$, ta có $\mathfrak{P}(\mathrm{X}) \subset \mathfrak{P}(\mathrm{X}')$.

¶ Cho A, B là hai tập hợp và $\Gamma$ là một sự tương ứng giữa A và B. *hàm* $\mathrm{X} \to \Gamma \langle \mathrm{X} \rangle$ $(\mathrm{X} \subset \mathfrak{P}(\mathrm{A}), \ \Gamma \langle \mathrm{X} \rangle \in \mathfrak{P}(\mathrm{B}))$ được gọi là *mở rộng chính tắc* (hoặc đơn giản là *mở rộng*) *của* $\Gamma$ *đối với các tập hợp các tập con* và được ký hiệu bởi $\hat{\Gamma}$; đó là một ánh xạ từ $\mathfrak{P}(\mathrm{A})$ vào $\mathfrak{P}(\mathrm{B})$. Nếu $\Gamma'$ là một sự tương ứng giữa B và một tập hợp C, công thức $(\Gamma' \circ \Gamma) \langle \mathrm{X} \rangle = \Gamma' \langle \Gamma \langle \mathrm{X} \rangle \rangle$ cho thấy rằng mở rộng của $\Gamma' \circ \Gamma$ đối với các tập hợp các tập con là ánh xạ $\hat{\Gamma}' \circ \hat{\Gamma}$.

#### Mệnh đề 1 {#ens-ii-s5-prop-1 .statement tag=03IJ}

(1) *Nếu* $f$ *là một toàn ánh từ một tập hợp* E *lên một tập hợp* F, *mở rộng chính tắc* $\hat{f}$ *của* $f$ *là một toàn ánh từ* $\mathfrak{P}(\mathrm{E})$ *lên* $\mathfrak{P}(\mathrm{F})$.

(2) *Nếu* $f$ *là một đơn ánh từ* E *vào* F, *mở rộng chính tắc* $\hat{f}$ *của* $f$ *là một đơn ánh từ* $\mathfrak{P}(\mathrm{E})$ *vào* $\mathfrak{P}(\mathrm{F})$.

(1) Nếu $s$ là một tiết diện của $f$, thì $f \circ s$ là ánh xạ đồng nhất của F, do đó $\hat{f} \circ \hat{s}$ là ánh xạ đồng nhất của $\mathfrak{P}(\mathrm{F})$; vì thế $\hat{f}$ là toàn ánh và $\hat{s}$ là một tiết diện của $\hat{f}$ (§3, no. 8).

(2) Mệnh đề là hiển nhiên nếu $E = \varnothing$, vì khi đó $\mathscr{P}(E) = \{\varnothing\}$. Nếu $E \ne \varnothing$ và nếu $r$ là một phép co rút của $f$, thì $r \circ f$ là ánh xạ đồng nhất của $E$, nên $\hat{r} \circ \hat{f}$ là ánh xạ đồng nhất của $\mathscr{P}(E)$; do đó $\hat{f}$ là đơn ánh, và $\hat{r}$ là một phép co rút của $\hat{f}$ (§3, no. 8).

### 2. TẬP HỢP CÁC ÁNH XẠ TỪ MỘT TẬP HỢP VÀO MỘT TẬP HỢP KHÁC

Cho $E$, $F$ là các tập hợp. Đồ thị của một ánh xạ từ $E$ vào $F$ là một tập con của $E \times F$. Do đó tập hợp các phần tử của $\mathscr{P}(E \times F)$ có tính chất là các đồ thị của những ánh xạ từ $E$ vào $F$ là một tập con của $\mathscr{P}(E \times F)$, được ký hiệu bởi $F^E$. Do đó tập hợp các bộ ba $f = (G, E, F)$, trong đó $G \in F^E$, là tập hợp các ánh xạ từ $E$ vào $F$; nó được ký hiệu bởi $\mathscr{F}(E, F)$. Rõ ràng $G \mapsto (G, E, F)$ là một song ánh (được gọi là song ánh chính tắc) từ $F^E$ lên $\mathscr{F}(E, F)$. Sự tồn tại của song ánh này cho phép chúng ta chuyển dịch ngay lập tức mọi mệnh đề liên quan đến tập hợp $F^E$ thành một mệnh đề liên quan đến $\mathscr{F}(E, F)$, và ngược lại.

¶ Cho $E$, $E'$, $F$, $F'$ là các tập hợp. Cho $u$ là một ánh xạ từ $E'$ vào $E$, và $v$ là một ánh xạ từ $F$ vào $F'$. Khi đó hàm $f \mapsto v \circ f \circ u$ là một ánh xạ từ $\mathscr{F}(E, F)$ vào $\mathscr{F}(E', F')$.

#### Mệnh đề 2 {#ens-ii-s5-prop-2 .statement tag=03Q5}

(1) *Nếu $u$ là một toàn ánh từ $E'$ lên $E$ và $v$ là một đơn ánh từ $F$ vào $F'$, thì ánh xạ $f \mapsto v \circ f \circ u$ là đơn ánh.*

(2) *Nếu $u$ là một đơn ánh từ $E'$ vào $E$ và $v$ là một toàn ánh từ $F$ lên $F'$, thì ánh xạ $f \mapsto v \circ f \circ u$ là toàn ánh.*

Ta sẽ giả sử rằng các tập hợp $E$, $E'$, $F$, $F'$ đều không rỗng, vì nếu không thì mệnh đề hiển nhiên đúng.

(1) Cho $s$ là một tiết diện của $u$ và $r$ là một phép co rút của $v$ (§3, Định nghĩa 11). Khi đó $r \circ (v \circ f \circ u) \circ s = I_F \circ f \circ I_E = f$, nên

$$
f \mapsto v \circ f \circ u
$$

là đơn ánh.

(2) Cho $r'$ là một phép co rút của $u$ và $s'$ là một tiết diện của $v$. Với mọi ánh xạ $f' : E' \to F'$ ta có $v \circ (s' \circ f' \circ r') \circ u = f'$, điều này chứng tỏ rằng ánh xạ $f \mapsto v \circ f \circ u$ là toàn ánh.

#### Hệ quả {#ens-ii-s5-n2-cor-1 .statement tag=03Q6}

*Nếu $u$ là một song ánh từ $E'$ lên $E$ và $v$ là một song ánh từ $F$ lên $F'$, thì $f \mapsto v \circ f \circ u$ là song ánh.*

Cho $A$, $B$, $C$ là ba tập hợp và cho $f$ là một ánh xạ từ $B \times C$ vào $A$. Với mọi $y \in C$, gọi $f(\mathord{\cdot}, y)$ là ánh xạ bộ phận $x \mapsto f(x,y)$ từ $B$ vào $A$ (§ 3, no. 9); hàm $y \mapsto f(\mathord{\cdot}, y)$ là một ánh xạ từ $C$ vào $\mathscr{F}(B, A)$

tồn tại một ánh xạ duy nhất $f$ của $\mathrm{B} \times \mathrm{C}$ vào A sao cho $g(y) = f(\bullet, y)$ với mỗi $y \in \mathrm{C}$, cụ thể là ánh xạ $(x, y) \to (g(y))(x)$. Do đó:

#### Mệnh đề 3 {#ens-ii-s5-prop-3 .statement tag=03Q7}

*Nếu với mọi ánh xạ $f$ của* $\mathrm{B} \times \mathrm{C}$ *vào* A *ta ký hiệu bởi $\tilde{f}$ ánh xạ $y \to f(\bullet, y)$ của* C *vào* $\mathscr{F}(\mathrm{B}, \mathrm{A})$, *thì hàm $f \to \tilde{f}$ là một song ánh* (gọi là *song ánh chính tắc*) *của* $\mathscr{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ *lên* $\mathscr{F}(\mathrm{C}, \mathscr{F}(\mathrm{B}, \mathrm{A}))$.

Tương tự, ta định nghĩa một *song ánh chính tắc* từ $\mathscr{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ lên $\mathscr{F}(\mathrm{B}, \mathscr{F}(\mathrm{C}, \mathrm{A}))$. Do sự tương ứng một-một giữa các ánh xạ và các đồ thị phiếm hàm, các song ánh này cho ra các *song ánh chính tắc* từ $\mathrm{A}^{\mathrm{B} \times \mathrm{C}}$ lên $(\mathrm{A}^{\mathrm{B}})^{\mathrm{C}}$ (tương ứng là $(\mathrm{A}^{\mathrm{C}})^{\mathrm{B}}$).

### 3. ĐỊNH NGHĨA TÍCH CỦA MỘT HỌ TẬP HỢP

Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ tập hợp và cho F là một đồ thị phiếm hàm có miền I sao cho $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ với mỗi $\iota \in \mathrm{I}$. Khi đó, với mỗi $\iota \in \mathrm{I}$ ta có $\mathrm{F}(\iota) \in \mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$, và do đó F là một phần tử của $\mathfrak{P}(\mathrm{I} \times \mathrm{A})$. Vì vậy, các đồ thị phiếm hàm có tính chất trên tạo thành một tập con của $\mathfrak{P}(\mathrm{I} \times \mathrm{A})$.

#### Định nghĩa 1 {#ens-ii-s5-def-1 .statement tag=03Q8}

*Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp. Tập hợp các đồ thị phiếm hàm* F *có miền xác định* I *sao cho* $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ *với mỗi* $\iota \in \mathrm{I}$ *được gọi là tích của họ các tập hợp $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ và được ký hiệu là* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. *Với mỗi* $\iota \in \mathrm{I}$, $\mathrm{X}_\iota$ *được gọi là nhân tử chỉ số $\iota$ trong tích* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. *Ánh xạ* $\mathrm{F} \to \mathrm{F}(\iota)$ $\left( \mathrm{F} \in \prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota,\ \mathrm{F}(\iota) \in \mathrm{X}_\iota \right)$ *được gọi là hàm tọa độ* (hay *phép chiếu*) *chỉ số $\iota$, và được ký hiệu là* $\mathrm{pr}_\iota$.

$\mathrm{F}(\iota)$ được gọi là *tọa độ có chỉ số* $\iota$ (hoặc *phép chiếu có chỉ số* $\iota$) của F; ảnh $\mathrm{pr}_\iota\langle \mathrm{A} \rangle$ của một tập con A của $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ qua hàm tọa độ có chỉ số $\iota$ được gọi là *phép chiếu có chỉ số* $\iota$ của A. Dễ dàng kiểm tra rằng $\mathrm{A} \subset \prod_{\iota \in \mathrm{I}} \mathrm{pr}_\iota \langle \mathrm{A} \rangle$.

Ta sẽ thường dùng ký hiệu $(x_\iota)_{\iota \in \mathrm{I}}$ để chỉ một phần tử của $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ (§3, no. 6).

Nếu $\mathrm{I} = \emptyset$, tập hợp $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ chỉ có một phần tử, đó là tập rỗng (§3, no. 4, Ví dụ 1).

¶ Nếu mọi thừa số $\mathrm{X}_\iota$ của tích $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ đều bằng cùng một tập hợp E, thì ta có $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \mathrm{E}^{\mathrm{I}}$; điều này suy ra ngay lập tức từ các định nghĩa.

¶ Nếu $(X_\iota)_{\iota \in I}$ là một họ tập hợp tùy ý và nếu E là một tập hợp sao cho

$$\bigcup_{\iota \in I} X_\iota \subset E,$$

thì Định nghĩa 1 cho thấy rằng $\prod_{\iota \in I} X_\iota \subset E^I$; do đó có một sự tương ứng một-một giữa $\prod_{\iota \in I} X_\iota$ và một tập hợp các ánh xạ từ I vào E (tức là, một tập con của $\mathscr{F}(I, E)$).

¶ Nếu $I = \{\alpha\}$ là một tập hợp gồm một phần tử duy nhất, ta có

$$\prod_{\iota \in I} X_\iota = X_\alpha^{\{\alpha\}};$$

khi đó ánh xạ $F \to F(\alpha)$ là một song ánh (gọi là *chính tắc*) từ $\prod_{\iota \in \{\alpha\}} X_\iota$ lên $X_\alpha$.

¶ Cho A, B là các tập hợp và $\alpha$, $\beta$ là các đối tượng phân biệt (tồn tại hai đối tượng phân biệt, chẳng hạn $\emptyset$ và $\{\emptyset\}$). Xét đồ thị $\{(\alpha, A), (\beta, B)\}$, đồ thị này rõ ràng là phiếm hàm và chính xác là họ $(X_\iota)_{\iota \in \{\alpha, \beta\}}$ sao cho $X_\alpha = A$ và $X_\beta = B$. Với mỗi cặp $(x, y) \in A \times B$, gọi $f_{x,y}$ là đồ thị phiếm hàm $\{(\alpha, x), (\beta, y)\}$. Hiển nhiên hàm $(x, y) \to f_{x,y}$ là một ánh xạ song ánh từ $A \times B$ lên $\prod_{\iota \in \{\alpha, \beta\}} X_\iota$; ánh xạ nghịch đảo của song ánh này là $g \to (g(\alpha), g(\beta))$. Hai song ánh này được gọi là *chính tắc*. Trong phần sau, chúng tôi sẽ dùng sự tương ứng một-một này để suy ra các tính chất của tích của hai tập hợp từ các tính chất của tích của một họ tập hợp.

¶ Cho $(X_\iota)_{\iota \in I}$ là một họ các tập hợp mà mỗi tập hợp chỉ gồm một phần tử, giả sử $X_\iota = \{a_\iota\}$; khi đó tích $\prod_{\iota \in I} X_\iota$ là một tập hợp chỉ gồm phần tử duy nhất $(a_\iota)_{\iota \in I}$.

¶ Cho E là một tập hợp. Các đồ thị của các ánh xạ *hằng số* $\iota \to x$ từ I vào E tạo thành một tập con $\Delta$ của tích $E^I$, gọi là *đường chéo*. Nếu $\bar{x}$ ký hiệu đồ thị của ánh xạ $\iota \to x$ (với $x \in E$), thì ánh xạ $x \to \bar{x}$ là một song ánh từ E lên $\Delta$, gọi là *ánh xạ đường chéo*.

#### Mệnh đề 4 {#ens-ii-s5-prop-4 .statement tag=03IK}

*Cho* $(X_\iota)_{\iota \in I}$ *là một họ các tập hợp, và cho u là một song ánh từ một tập hợp* K *lên tập hợp chỉ số* I. *Nếu* U *là đồ thị của u, thì ánh xạ* $F \to F \circ U$ *từ* $\prod_{\iota \in I} X_\iota$ *vào* $\prod_{x \in K} X_{u(x)}$ *là song ánh.*

Đặt

$$A = \bigcup_{\iota \in I} X_\iota = \bigcup_{x \in K} X_{u(x)}$$

(§4, Mệnh đề 1). Ánh xạ $F\to F\circ U$ ($F\in A^I$) là một song ánh từ $A^I$ lên $A^K$ (Mệnh đề 2). Hiển nhiên điều kiện “với mọi $\iota\in I$, $F(\iota)\in X_\iota$” là tương đương với “với mọi $x\in K$, $(F\circ U)(x)\in X_{u(x)}$”, và kết quả suy ra.

### 4. CÁC TÍCH TỪNG PHẦN

Cho $(X_\iota)_{\iota\in I}$ là một họ các tập hợp, và cho $J$ là một tập con của $I$. Tích $\displaystyle\prod_{\iota\in J}X_\iota$ được gọi là một *tích bộ phận* của $\displaystyle\prod_{\iota\in I}X_\iota$. Nếu $f$ là một hàm có đồ thị $F$ là một phần tử của $\displaystyle\prod_{\iota\in I}X_\iota$, thì $F\circ\Delta_J$ (trong đó $\Delta_J$ là đường chéo của $J\times J$) là đồ thị của *hạn chế* của $f$ trên $J$. Rõ ràng $F\circ\Delta_J\in\displaystyle\prod_{\iota\in J}X_\iota$; ánh xạ $F\to F\circ\Delta_J$ từ $\displaystyle\prod_{\iota\in I}X_\iota$ vào $\displaystyle\prod_{\iota\in J}X_\iota$ được gọi là *phép chiếu có chỉ số* $J$ và được ký hiệu bởi $\operatorname{pr}_J$.

#### Mệnh đề 5 {#ens-ii-s5-prop-5 .statement tag=03Q9}

*Cho $(X_\iota)_{\iota\in I}$ là một họ các tập hợp và $J$ là một tập con của $I$. Nếu với mọi $\iota\in I$ ta có $X_\iota\ne\varnothing$, thì phép chiếu $\operatorname{pr}_J$ là một ánh xạ từ $\displaystyle\prod_{\iota\in I}X_\iota$ lên $\displaystyle\prod_{\iota\in J}X_\iota$.*

Theo các nhận xét đã nêu ở trên, chỉ cần chứng minh mệnh đề sau đây :

#### Mệnh đề 6 {#ens-ii-s5-prop-6 .statement tag=03QA}

*Cho $(X_\iota)_{\iota\in I}$ là một họ các tập hợp sao cho $X_\iota\ne\varnothing$ với mọi $\iota\in I$. Nếu $g$ là một ánh xạ từ $J\subset I$ vào $A=\displaystyle\bigcup_{\iota\in I}X_\iota$, sao cho $g(\iota)\in X_\iota$ với mọi $\iota\in J$, thì tồn tại một mở rộng $f$ của $g$ lên $I$ sao cho $f(\iota)\in X_\iota$ với mọi $\iota\in I$.*

Với mỗi $\iota\in I-J$ đặt $T_\iota$ ký hiệu số hạng $\tau_\iota(y\in X_\iota)$. Vì $X_\iota\ne\varnothing$ theo giả thiết, nên $T_\iota\in X_\iota$ với mọi $\iota\in I-J$ (Chương I, §4, no. 1). Nếu $G$ là đồ thị của $g$, thì đồ thị $G\cup\left(\displaystyle\bigcup_{\iota\in I-J}\{(\iota,T_\iota)\}\right)$ là đồ thị của một hàm có các tính chất cần có, như được kiểm tra ngay lập tức.

#### Hệ quả 1 {#ens-ii-s5-prop-6-cor-1 .statement tag=03QB}

*Cho $(X_\iota)_{\iota\in I}$ là một họ các tập hợp sao cho với mỗi $\iota\in I$ ta có $X_\iota\ne\varnothing$. Khi đó với mỗi $\alpha\in I$ phép chiếu $\operatorname{pr}_\alpha$ là một ánh xạ của $\displaystyle\prod_{\iota\in I}X_\iota$ lên $X_\alpha$.*

Áp dụng Mệnh đề 5 cho tập con $J=\{\alpha\}$ của $I$ và chú ý rằng $\operatorname{pr}_\alpha$ là hợp thành của ánh xạ chính tắc của $X_\alpha^{\{\alpha\}}$ lên $X_\alpha$ và ánh xạ $\operatorname{pr}_{\{\alpha\}}$.

#### Hệ quả 2 {#ens-ii-s5-prop-6-cor-2 .statement tag=03QC}

*Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp. Khi đó $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \emptyset$ khi và chỉ khi tồn tại $\iota \in \mathrm{I}$ sao cho $\mathrm{X}_\iota = \emptyset$.*

Nếu ta có $\mathrm{X}_\iota \neq \emptyset$ với mỗi $\iota \in \mathrm{I}$, thì từ Hệ quả 1 suy ra $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$; ngược lại, nếu $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$, quan hệ $\mathrm{pr}_\alpha\Big(\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{X}_\alpha$ cho thấy rằng $\mathrm{X}_\alpha \neq \emptyset$ với mỗi $\alpha \in \mathrm{I}$.

Do đó, nếu ta có một họ $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ các tập hợp không rỗng, ta có thể giới thiệu (như một hằng số phụ) một hàm $f$ có miền xác định là I sao cho $f(\iota) \in \mathrm{X}_\iota$ với mọi $\iota \in \mathrm{I}$. Trong thực hành người ta nói: "lấy một phần tử $x_\iota$ trong mỗi $\mathrm{X}_\iota$". Theo trực giác, như vậy ta đã "chọn" một phần tử $x_\iota$ trong mỗi tập hợp $\mathrm{X}_\iota$; việc giới thiệu dấu lôgic $\tau$ và các tiêu chuẩn chi phối việc sử dụng nó miễn cho ta khỏi sự cần thiết phải phát biểu một "tiên đề lựa chọn" để hợp thức hóa phép toán này (xem Tóm tắt các kết quả, §4, no. 10).

#### Hệ quả 3 {#ens-ii-s5-prop-6-cor-3 .statement tag=03QD}

*Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ và $(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ là hai họ tập hợp có cùng tập hợp chỉ số I. Nếu $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ với mỗi $\iota \in \mathrm{I}$, thì*

$$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota.$$

*Ngược lại, nếu $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod\limits_{\iota \in \mathrm{I}} \mathrm{Y}_\iota$, và nếu $\mathrm{X}_\iota \neq \emptyset$ với mỗi $\iota \in \mathrm{I}$, thì $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ với mỗi $\iota \in \mathrm{I}$.*

Mệnh đề thứ nhất là hiển nhiên, và mệnh đề thứ hai suy ra từ Mệnh đề 1, Hệ quả 5, vì khi đó ta có, với mỗi $\alpha \in \mathrm{I}$,

$$\mathrm{X}_\alpha = \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota\Big) = \mathrm{Y}_\alpha.$$

### 5. TÍNH KẾT HỢP CỦA TÍCH CÁC TẬP HỢP

#### Mệnh đề 7 {#ens-ii-s5-prop-7 .statement tag=03IN}

*Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp mà tập chỉ số I không phải là tập rỗng. Cho $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ là một phân hoạch của I. Khi đó ánh xạ*

$$f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$$

*của $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ vào tập hợp tích $\prod\limits_{\lambda \in \mathrm{L}} \Big(\prod\limits_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota\Big)$ là song ánh ("tính kết hợp" của tích các tập hợp).*

Từ cách diễn giải $\mathrm{pr}_{\mathrm{J}_\lambda} f$ như là đồ thị của hạn chế của hàm có đồ thị là $f$ (số 4), suy ra rằng mệnh đề cho rằng ánh xạ $f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$ là song ánh có nghĩa là, với mỗi họ $(v_\lambda)_{\lambda \in \mathrm{L}}$, trong đó $v_\lambda$ là một ánh xạ từ $\mathrm{J}_\lambda$ vào $\bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$, tồn tại một ánh xạ duy nhất $u$

của I vào $\bigcup_{\iota \in I} X_\iota$ sao cho $v_\lambda$ là hạn chế của $u$ trên $J_\lambda$ với mỗi $\lambda \in L$. Nhưng điều này là một hệ quả của giả thiết rằng $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của I (§4, Mệnh đề 8).

¶ Song ánh được định nghĩa trong Mệnh đề 7, và song ánh ngược của nó được gọi là *chính tắc*.

*Nhận xét*

#### Nhận xét 1 {#ens-ii-s5-n5-rem-1 .statement tag=03SA}

Cho $\alpha$, $\beta$ là hai đối tượng phân biệt và cho $(J_\lambda)_{\lambda \in \{\alpha, \beta\}}$ là một phân hoạch của I thành hai tập hợp $J_\alpha$, $J_\beta$. Như vậy ta thu được một ánh xạ một-một (vẫn được gọi là *chính tắc*) của tích $\prod_{\iota \in I} X_\iota$ lên $\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$ bằng cách lấy hợp thành của ánh xạ chính tắc từ $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$ lên $\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$ và ánh xạ chính tắc từ $\prod_{\iota \in I} X_\iota$ lên $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$. Nếu $X_\iota$ là một tập hợp gồm một *phần tử duy nhất* với mỗi $\iota \in J_\beta$, thì $\mathrm{pr}_{J_\alpha}$ là một ánh xạ song ánh từ $\prod_{\iota \in I} X_\iota$ lên $\prod_{\iota \in J_\alpha} X_\iota$.

#### Nhận xét 2 {#ens-ii-s5-n5-rem-2 .statement tag=03SB}

Cho $\alpha$, $\beta$, $\gamma$ là ba đối tượng, không có hai đối tượng nào bằng nhau (ba đối tượng như vậy tồn tại; chẳng hạn, $\emptyset$, $\{\emptyset\}$, $\{\{\emptyset\}\}$), và cho A, B, C là các tập hợp. Xét đồ thị phiếm hàm $\{(\alpha, A), (\beta, B), (\gamma, C)\}$, tức là họ các tập hợp $(X_\iota)_{\iota \in \{\alpha, \beta, \gamma\}}$ sao cho $X_\alpha = A$, $X_\beta = B$, $X_\gamma = C$. Với phân hoạch của $\{\alpha, \beta, \gamma\}$ tạo bởi hai tập hợp $\{\alpha, \beta\}$ và $\{\gamma\}$ tương ứng với một song ánh chính tắc từ $\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ lên tích

$$\left( \prod_{\iota \in \{\alpha, \beta\}} X_\iota \right) \times X_\gamma^{\{\gamma\}},$$

và do đó một song ánh (cũng gọi là *chính tắc*) từ $\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ lên $A \times B \times C$ (§ 2, no. 2), biến mỗi đồ thị $f \in \prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ thành phần tử $(f(\alpha), f(\beta), f(\gamma))$ của $A \times B \times C$. Theo Mệnh đề 4, do đó ta có thể thiết lập một sự tương ứng một-một giữa hai tập hợp bất kỳ trong sáu tập hợp $A \times B \times C$, $B \times C \times A$, $C \times A \times B$, $B \times A \times C$, $A \times C \times B$, $C \times B \times A$.

### 6. CÁC CÔNG THỨC PHÂN PHỐI

#### Mệnh đề 8 {#ens-ii-s5-prop-8 .statement tag=03IO}

*Cho* $((X_{\lambda,\iota})_{\iota \in J_\lambda})_{\lambda \in L}$ *là một họ (với tập chỉ số* L*) gồm các họ tập hợp. Giả sử rằng* $L \neq \emptyset$ *và rằng* $J_\lambda \neq \emptyset$ *với mỗi* $\lambda \in L$. *Đặt*

$$I = \prod_{\lambda \in L} J_\lambda \neq \emptyset.$$

*Khi đó ta có*

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right),$$
$$\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcup_{f \in I} \left( \bigcap_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$$

("tính phân phối" của hợp đối với giao, và của giao đối với hợp).

Cho $x$ là một phần tử của $\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right)$ và cho $f$ là một phần tử bất kỳ của I. Tồn tại một chỉ số $\lambda$ sao cho $x \in \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$; do đó $x \in X_{\lambda, f(\lambda)}$ và vì thế

$$x \in \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}.$$

Vì điều này đúng với mọi $f \in I$, nên ta có

$$x \in \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

Ngược lại, giả sử $x$ là một đối tượng không thuộc tập hợp

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right).$$

Khi đó với mỗi $\lambda \in L$ ta có $x \notin \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$, nghĩa là tập hợp $J'_\lambda$ các chỉ số $\iota \in J_\lambda$ sao cho $x \notin X_{\lambda, \iota}$ là không rỗng với mỗi $\lambda \in L$. Theo Mệnh đề 5, Hệ quả 2, tồn tại một đồ thị phiếm hàm $f$ có miền xác định là L sao cho với mỗi $\lambda \in L$ ta có $f(\lambda) \in J'_\lambda$. Do đó $f \in I$ và $x \notin X_{\lambda, f(\lambda)}$ với mỗi $\lambda \in L$; do đó

$$x \notin \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$$

và do đó

$$x \notin \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

Điều này hoàn tất chứng minh của công thức thứ nhất. Công thức thứ hai suy ra bằng cách áp dụng công thức thứ nhất cho họ $((\complement_A X_{\lambda, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$, trong đó A ký hiệu hợp $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\lambda \right)$.

#### Hệ quả {#ens-ii-s5-n6-cor-1 .statement tag=03IP}

*Cho* $(X_\iota)_{\iota \in I}$ *và* $(Y_\varkappa)_{\varkappa \in K}$ *là hai họ tập hợp có các tập hợp chỉ số không rỗng* I, K. *Khi đó*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \cup \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cup Y_\varkappa),$$
$$\left( \bigcup_{\iota \in I} X_\iota \right) \cap \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cap Y_\varkappa).$$

Cho $\alpha$, $\beta$ là hai đối tượng phân biệt; áp dụng các công thức của Mệnh đề 8 (với $L = \{\alpha,\ \beta\}$, $J_\alpha = I$, $J_\beta = K$) cho họ $((Z_{\lambda,\, \mu})_{\mu \in J_\lambda})_{\lambda \in L}$, trong đó $Z_{\alpha,\, \iota} = X_\iota$ với mọi $\iota \in I$ và $Z_{\beta,\, \varkappa} = Y_\varkappa$ với mỗi $\varkappa \in K$. Do sự tồn tại của song ánh chính tắc từ $\coprod_{\lambda \in L} J_\lambda$ lên $I \times K$ (no. 3) và theo Mệnh đề 1 của § 4, ta thu được các công thức đã phát biểu.

#### Mệnh đề 9 {#ens-ii-s5-prop-9 .statement tag=03IQ}

*Cho* $((X_{\lambda,\, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$ *là một họ (với tập hợp chỉ số* L) *gồm các họ tập hợp. Đặt* $I = \prod_{\lambda \in L} J_\lambda$. *Khi đó*

$$\prod_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

*và (nếu* $L \neq \emptyset$ *và* $J_\lambda \neq \emptyset$ *với mọi* $\lambda \in L$)

$$\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcap_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

("tính phân phối" của tích đối với hợp và đối với giao).
Công thức thứ nhất là hiển nhiên đúng nếu $L = \emptyset$ hoặc nếu $J_\lambda = \emptyset$ đối với một $\lambda \in L$. Nếu không, lấy $g$ là một phần tử của $\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right)$. Với mỗi $\lambda \in L$ tồn tại một chỉ số $\iota \in J_\lambda$ sao cho $g(\lambda) \in X_{\lambda,\, \iota}$; nói cách khác, tập hợp $H_\lambda$ các chỉ số $\iota \in J_\lambda$ sao cho $g(\lambda) \in X_{\lambda,\, \iota}$ là không rỗng. Do Hệ quả 2 của Mệnh đề 5, vì thế tồn tại một đồ thị phiếm hàm $f$ có miền xác định là L sao cho

$$f(\lambda) \in H_\lambda$$

với mỗi $\lambda \in L$, tức là, $g(\lambda) \in X_{\lambda,\, f(\lambda)}$. Vậy ta có $g \in \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)}$ và do đó $g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$. Ngược lại, nếu

$$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right),$$

thì tồn tại một đồ thị phiếm hàm $f \in I$ sao cho với mọi $\lambda \in L$ ta có

$$g(\lambda) \in X_{\lambda,\, f(\lambda)}$$

và, *a fortiori*, $g(\lambda) \in \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$. Điều này hoàn tất chứng minh của công thức thứ nhất. Chứng minh của công thức thứ hai là tương tự nhưng đơn giản hơn, và chúng tôi để lại cho người đọc.

#### Hệ quả 1 {#ens-ii-s5-prop-9-cor-1 .statement tag=03QE}

*Giả sử* $L \neq \emptyset$ *và* $J_\lambda \neq \emptyset$ *với mỗi* $\lambda \in L$. *Nếu với mỗi chỉ số* $\lambda \in L$ *thì họ* $(X_{\lambda, \iota})_{\iota \in J_\lambda}$ *là một phân hoạch của* $X_\lambda = \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$, *thì họ* $\left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)_{f \in I}$ *là một phân hoạch của* $\prod_{\lambda \in L} X_\lambda$.

Nếu đặt

$$\mathrm{P}_f = \prod_{\lambda \in L} X_{\lambda, f(\lambda)},$$

khi đó, do công thức thứ nhất của Mệnh đề 9, chỉ cần chứng minh rằng $\mathrm{P}_f \neq \emptyset$ với mọi $f \in I$ và $\mathrm{P}_f \cap \mathrm{P}_g = \emptyset$ mỗi khi $f$ và $g$ là các phần tử phân biệt của I. Điểm thứ nhất suy ra từ Mệnh đề 5, Hệ quả 2. Đối với điểm thứ hai, nếu $f \neq g$, tồn tại $\lambda \in L$ sao cho

$$f(\lambda) \neq g(\lambda)$$

và do đó, theo giả thiết, $X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$. Suy ra không có đồ thị nào thuộc $\mathrm{P}_f \cap \mathrm{P}_g$; thật vậy, nếu G là một đồ thị như thế, ta sẽ có $\mathrm{G}(\lambda) \in X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$, điều này là phi lý.

#### Hệ quả 2 {#ens-ii-s5-prop-9-cor-2 .statement tag=03QF}

*Cho* $(X_\iota)_{\iota \in I}$ *và* $(Y_\varkappa)_{\varkappa \in K}$ *là hai họ tập hợp. Khi đó*

$$\left( \bigcup_{\iota \in I} X_\iota \right) \times \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa)$$

*và, nếu* I *và* K *khác rỗng,*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \times \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa).$$

Chứng minh theo cùng khuôn mẫu như chứng minh của Hệ quả của Mệnh đề 8.

#### Mệnh đề 10 {#ens-ii-s5-prop-10 .statement tag=03QG}

*Cho* $(X_{\iota, \varkappa})_{(\iota, \varkappa) \in I \times K}$ *là một họ tập hợp mà tập hợp chỉ số là tích của hai tập hợp* I *và* K. *Nếu* $K \neq \emptyset$, *ta có*

$$\bigcap_{\varkappa \in K} \left( \prod_{\iota \in I} X_{\iota, \varkappa} \right) = \prod_{\iota \in I} \left( \bigcap_{K \in \varkappa} X_{\iota, \varkappa} \right).$$

Hai vế của đẳng thức cần chứng minh đều là các đồ thị phiếm hàm. Một đồ thị $f$ thuộc vế trái khi và chỉ khi, với mỗi $\varkappa \in K$, ta có $f \in \prod_{\iota \in I} X_{\iota, \varkappa}$; nghĩa là, khi và chỉ khi $f(\iota) \in X_{\iota, \varkappa}$ với mọi $(\iota, \varkappa) \in I \times K$. Để $f$ thuộc

vế phải, điều kiện cần thiết và đủ là $f(\iota) \in \bigcap_{\varkappa \in K} X_{\iota, \varkappa}$ với mỗi $\iota \in I$, tức là $f(\iota) \in X_{\iota, \varkappa}$ với mỗi cặp $(\iota, \varkappa) \in I \times K$. Điều này hoàn thành chứng minh.

#### Hệ quả {#ens-ii-s5-n6-cor-2 .statement tag=03IR}

*Cho* $(X_\iota)_{\iota \in I}$ *và* $(Y_\iota)_{\iota \in I}$ *là hai họ tập hợp có cùng tập hợp chỉ số* $I \neq \emptyset$. *Khi đó*

$$\Big(\prod_{\iota \in I} X_\iota\Big) \cap \Big(\prod_{\iota \in I} Y_\iota\Big) = \prod_{\iota \in I} (X_\iota \cap Y_\iota),$$
$$\Big(\bigcap_{\iota \in I} X_\iota\Big) \times \Big(\bigcap_{\iota \in I} Y_\iota\Big) = \bigcap_{\iota \in I} (X_\iota \times Y_\iota).$$

Áp dụng Mệnh đề 10 cho trường hợp K (tương ứng I) là một tập hợp gồm hai phần tử phân biệt.

### 7. MỞ RỘNG CÁC ÁNH XẠ TỚI CÁC TÍCH

#### Định nghĩa 2 {#ens-ii-s5-def-2 .statement tag=03IS}

*Cho* $(X_\iota)_{\iota \in I}$, $(Y_\iota)_{\iota \in I}$ *là hai họ tập hợp, và cho* $(g_\iota)_{\iota \in I}$ *là một họ hàm có cùng tập chỉ số* I *sao cho* $g_\iota$ *là một ánh xạ từ* $X_\iota$ *vào* $Y_\iota$ *với mỗi* $\iota \in I$. *Với mỗi* $f \in \prod_{\iota \in I} X_\iota$ *đặt* $u_f$ *là đồ thị của hàm* $\iota = g_\iota(f(\iota))$ $(\iota \in I)$, *là một phần tử của* $\prod_{\iota \in I} Y_\iota$. *Ánh xạ* $f \to u_f$ *từ* $\prod_{\iota \in I} X_\iota$ *vào* $\prod_{\iota \in I} Y_\iota$ *được gọi là phép mở rộng chính tắc* (hoặc đơn giản là *mở rộng*) *lên các tích của họ ánh xạ* $(g_\iota)_{\iota \in I}$; *nó cũng đôi khi được gọi là tích của họ ánh xạ* $(g_\iota)_{\iota \in I}$.

Khi dùng ký hiệu chỉ số, tích của họ $(g_\iota)_{\iota \in I}$ là hàm $(x_\iota)_{\iota \in I} \to (g_\iota(x_\iota))_{\iota \in I}$; đôi khi nó được ký hiệu bởi $(g_\iota)_{\iota \in I}$.

Nếu $I = \{\alpha, \beta\}$, trong đó $\alpha$ và $\beta$ là phân biệt, thì mở rộng lên các tích của họ các ánh xạ $(g_\iota)_{\iota \in I}$ chính là $\psi \circ (g_\alpha \times g_\beta) \circ \varphi$, trong đó $\varphi$ ký hiệu ánh xạ chính tắc từ $\prod_{\iota \in I} X_\iota$ lên $X_\alpha \times X_\beta$ (no. 3) và $\psi$ ký hiệu ánh xạ chính tắc từ $Y_\alpha \times Y_\beta$ lên $\prod_{\iota \in I} Y_\iota$.

#### Mệnh đề 11 {#ens-ii-s5-prop-11 .statement tag=03IT}

*Cho* $(X_\iota)_{\iota \in I}$, $(Y_\iota)_{\iota \in I}$, $(Z_\iota)_{\iota \in I}$ *là ba họ tập hợp và cho* $(g_\iota)_{\iota \in I}$, $(g'_\iota)_{\iota \in I}$ *là hai họ hàm, tất cả đều có cùng một tập chỉ số, sao cho* $g_\iota$ *là một ánh xạ từ* $X_\iota$ *vào* $Y_\iota$ *và* $g'_\iota$ *là một ánh xạ từ* $Y_\iota$ *vào* $Z_\iota$, *với mỗi* $\iota \in I$. *Cho* $g$ *và* $g'$ *là các mở rộng của các họ* $(g_\iota)_{\iota \in I}$ *và* $(g'_\iota)_{\iota \in I}$ *lên các tích. Khi đó mở rộng của họ* $(g'_\iota \circ g_\iota)_{\iota \in I}$ *lên các tích bằng* $g' \circ g$.

Điều này suy ra ngay lập tức từ Định nghĩa 2.

#### Hệ quả {#ens-ii-s5-n7-cor-1 .statement tag=03IU}

Cho $(X_i)_{i\in I}$, $(Y_i)_{i\in I}$ là hai họ tập hợp và cho $(g_i)_{i\in I}$ là một họ các hàm. Nếu $g_i$ là một đơn ánh (tương ứng, toàn ánh) từ $X_i$ vào $Y_i$, với mỗi $i\in I$, thì mở rộng $g$ của $(g_i)_{i\in I}$ lên các tích là một đơn ánh (tương ứng, toàn ánh) từ $\displaystyle\prod_{i\in I}X_i$ vào $\displaystyle\prod_{i\in I}Y_i$.

(1) Giả sử rằng $X_i\ne\varnothing$ với mọi $i\in I$; nếu không thì kết quả là tầm thường. Giả sử $g_i$ là đơn ánh với mọi $i\in I$, và gọi $r_i$ là một phép rút của $g_i$ (§ 3, no. 8, Định nghĩa 11), sao cho $r_i\circ g_i$ là ánh xạ đồng nhất của $X_i$. Gọi $r$ là mở rộng lên các tích của họ $(r_i)_{i\in I}$; vì $r\circ g$ là mở rộng lên các tích của họ các ánh xạ đồng nhất $I_{X_i}$, nên $r\circ g$ là ánh xạ đồng nhất của $\displaystyle\prod_{i\in I}X_i$, và do đó $g$ là đơn ánh (§ 3, Mệnh đề 8).

(2) Giả sử rằng $g_i$ là một ánh xạ toàn ánh của $X_i$ lên $Y_i$ với mỗi $i\in I$, và gọi $s_i$ là một tiết diện của $g_i$ (§ 3, no. 8, định nghĩa 11), sao cho $g_i\circ s_i$ là ánh xạ đồng nhất của $Y_i$. Nếu $s$ là mở rộng đến các tích của họ $(s_i)_{i\in I}$, thì $g\circ s$ là mở rộng đến các tích của họ các ánh xạ đồng nhất $I_{Y_i}$, và do đó là ánh xạ đồng nhất của $\displaystyle\prod_{i\in I}Y_i$; vì thế $g$ là toàn ánh (§ 3, Mệnh đề 8).

Cho $(X_i)_{i\in I}$ là một họ các tập hợp, và cho $E$ là một tập hợp. Với mọi ánh xạ $f$ từ $E$ vào $\displaystyle\prod_{i\in I}X_i$, $\operatorname{pr}_i\circ f$ là một ánh xạ từ $E$ vào $X_i$. Nếu $\bar f$ là mở rộng lên tích của họ các ánh xạ này, và nếu $d$ là ánh xạ đường chéo từ $E$ vào $E^I$, thì ngay lập tức có $f=\bar f\circ d$. Ngược lại, cho $(f_i)_{i\in I}$ là một họ các hàm sao cho $f_i$ là một ánh xạ từ $E$ vào $X_i$ với mỗi $i\in I$, và cho $\bar f$ là mở rộng lên tích của họ này; khi đó ta có $\operatorname{pr}_i\circ(\bar f\circ d)=f_i$ với mỗi $i\in I$. Do lạm dụng ngôn ngữ, ánh xạ $\bar f\circ d$ cũng được viết là $(f_i)_{i\in I}$. Theo cách đó ta định nghĩa một ánh xạ một-một từ tập hợp $\displaystyle\prod_{i\in I}X_i^E$ lên tập hợp $\displaystyle\left(\prod_{i\in I}X_i\right)^E$; ánh xạ này và ánh xạ nghịch đảo của nó được gọi là chính tắc.

### Bài tập {#ens-ii-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
