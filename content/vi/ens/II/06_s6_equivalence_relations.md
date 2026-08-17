---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 6
section_title: Equivalence relations
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 112-122, 127-129
pdf_pages: 0119-0129, 0134-0136
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN EQUIVALENCE RELATION
      page: 113
      pdf_page: 120
    - "no": 2
      title: EQUIVALENCE CLASSES ; QUOTIENT SET
      page: 114
      pdf_page: 121
    - "no": 3
      title: RELATIONS COMPATIBLE WITH AN EQUIVALENCE RELATION
      page: 116
      pdf_page: 123
    - "no": 4
      title: SATURATED SUBSETS
      page: 117
      pdf_page: 124
    - "no": 5
      title: MAPPINGS COMPATIBLE WITH EQUIVALENCE RELATIONS
      page: 118
      pdf_page: 125
    - "no": 6
      title: INVERSE IMAGE OF AN EQUIVALENCE RELATION; INDUCED EQUIVALENCE RELATION
      page: 119
      pdf_page: 126
    - "no": 7
      title: QUOTIENTS OF EQUIVALENCE RELATIONS
      page: 119
      pdf_page: 126
    - "no": 8
      title: PRODUCT OF TWO EQUIVALENCE RELATIONS
      page: 120
      pdf_page: 127
    - "no": 9
      title: CLASSES OF EQUIVALENT OBJECTS
      page: 121
      pdf_page: 128
statements: 12
exercises: 11
content_sha256: b974e1b991017b4b7f3d0ceeb1aa9f83860cbebeb103be703961f68820063b3d
translated_from: content/en/ens/II/06_s6_equivalence_relations.md
source_content_sha256: c6c3e77659f381e6b77f183ba2f44f12d66221c3beccde4dd5c2acdfdb891b2e
translation_model: gpt-5.4
translation_run: translate-vi-95bbd69b
glossary_version: 29
glossary_terms_sha256: 26e806c6479ae1050a151f9741551faef4ab049eff3fdf5435567f91f2fa1712
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. QUAN HỆ TƯƠNG ĐƯƠNG

Về nguyên lý, từ nay chúng tôi sẽ thôi dùng các chữ nghiêng đậm để biểu thị các dãy ký hiệu không xác định; độc giả sẽ có thể dễ dàng nhận ra từ ngữ cảnh những mệnh đề áp dụng cho các chữ cái hoặc các quan hệ không xác định.

### 1. ĐỊNH NGHĨA CỦA MỘT QUAN HỆ TƯƠNG ĐƯƠNG

Cho $R\{x, y\}$ là một quan hệ, trong đó $x$ và $y$ là các chữ cái phân biệt. Quan hệ $R$ được gọi là *đối xứng* (đối với các chữ cái $x$ và $y$) nếu

$$R\{x, y\} \Rightarrow R\{y, x\}.$$

Khi đó, bằng cách thay $x$ và $y$ bởi hai chữ $x'$ và $y'$, phân biệt với nhau và với mọi chữ xuất hiện trong $R$, rồi sau đó lần lượt thay $y$ và $x$ cho $x'$ và $y'$, ta thấy rằng

$$R\{y, x\} \Rightarrow R\{x, y\}.$$

Do đó $R\{x, y\}$ và $R\{y, x\}$ là tương đương.

¶ Cho $z$ là một chữ cái không xuất hiện trong $R$. Quan hệ $R$ được gọi là *bắc cầu* (đối với các chữ cái $x, y$) nếu ta có

$$(R\{x, y\} \text{ và } R\{y, z\}) \Rightarrow R\{x, z\}.$$

#### Ví dụ {#ens-ii-s6-n1-exa-6 .statement tag=03TP}

Quan hệ $x = y$ là đối xứng và bắc cầu. Quan hệ $X \subset Y$ là bắc cầu nhưng không đối xứng. Quan hệ $X \cap Y = \emptyset$ là đối xứng nhưng không bắc cầu.

Nếu $R\{x, y\}$ vừa đối xứng vừa bắc cầu thì nó được gọi là một *quan hệ tương đương* (đối với các chữ $x$ và $y$). Trong trường hợp này, ký hiệu $x \equiv y \pmod{R}$ đôi khi được dùng như một từ đồng nghĩa của $R\{x, y\}$; đọc là "*x tương đương với y theo môđun* $R$". Nếu $R$ là một quan hệ tương đương, ta có $R\{x, y\} \Rightarrow (R\{x, x\}$ và $R\{y, y\})$, vì $R\{x, y\}$ suy ra $R\{y, x\}$, và $(R\{x, y\}$ và $R\{y, x\})$ suy ra $(R\{x, x\}$ và $R\{y, y\})$ theo các định nghĩa.

¶ Cho $R\{x, y\}$ là một quan hệ; ta nói nó là *phản xạ trên* $E$ (đối với các chữ $x, y$) nếu quan hệ $R\{x, x\}$ tương đương với $x \in E$. Nếu không thể có sự mơ hồ nào về $E$, người ta đơn giản nói, do lạm dụng ngôn ngữ, rằng $R$ là phản xạ.

¶ Một *quan hệ tương đương trên* $E$ được định nghĩa là một quan hệ tương đương phản xạ trên $E$. Nếu $R\{x, y\}$ là một quan hệ tương đương trên $E$, ta có $R\{x, y\} \Rightarrow ((x, y) \in E \times E)$, do đó $R$ có một đồ thị (đối với các chữ cái $x, y$). Ngược lại, giả sử rằng quan hệ tương đương $R\{x, y\}$ có đồ thị $G$. Nhận thấy rằng quan hệ $R\{x, x\}$ tương đương với quan hệ $(\exists y)R\{x, y\}$; thật vậy, quan hệ thứ nhất suy ra quan hệ thứ hai (Chương I, § 4, no. 2, lược đồ S5), và ngược lại, vì $R\{x, y\}$ suy ra $R\{x, x\}$, nên $(\exists y) R\{x, y\}$ suy ra $(\exists y) R\{x, x\}$ và do đó cũng suy ra $R\{x, x\}$. Vậy $R\{x, x\}$ tương đương với $x \in \mathrm{pr}_1 G$, và do đó $R$ là một quan hệ tương đương trên $\mathrm{pr}_1 G$.

¶ Một *tương đương* trên một tập hợp E là một sự tương ứng mà tập nguồn và tập đích đều bằng E, và có đồ thị F sao cho quan hệ $(x, y) \in F$ là một quan hệ tương đương trên E.

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s6-n1-exa-1 .statement tag=03IX}

Quan hệ $x = y$ là một quan hệ tương đương không có đồ thị, vì nếu có thì phép chiếu thứ nhất của đồ thị này sẽ là tập hợp mọi đối tượng.

#### Ví dụ 2 {#ens-ii-s6-n1-exa-2 .statement tag=03SC}

Quan hệ "$x = y$ và $x \in E$" là một quan hệ tương đương trên E mà đồ thị là đường chéo của $E \times E$.

#### Ví dụ 3 {#ens-ii-s6-n1-exa-3 .statement tag=03TQ}

Quan hệ "tồn tại một song ánh từ X lên Y" là một quan hệ tương đương không có đồ thị (xem Chương III, § 3).

#### Ví dụ 4 {#ens-ii-s6-n1-exa-4 .statement tag=03TR}

Quan hệ "$x \in E$ và $y \in E$" là một quan hệ tương đương trên E, mà đồ thị là $E \times E$.

#### Ví dụ 5 {#ens-ii-s6-n1-exa-5 .statement tag=03TS}

Giả sử $A \subset E$; khi đó quan hệ

$$(x \in E - A \text{ và } y = x) \text{ hoặc } (x \in A \text{ và } y \in A)$$

là một quan hệ tương đương trên E.
(6) \* Quan hệ "$x \in \mathbf{Z}$ và $y \in \mathbf{Z}$ và $x - y$ chia được cho 4" là một quan hệ tương đương trên $\mathbf{Z}$.\*

#### Mệnh đề 1 {#ens-ii-s6-prop-1 .statement tag=03QH}

*Một sự tương ứng* $\Gamma$ *giữa* X *và* X *là một quan hệ tương đương trên* X *khi và chỉ khi nó thỏa mãn các điều kiện sau :* (a) X *là miền xác định của* $\Gamma$; (b) $\Gamma = \overset{-1}{\Gamma}$; (c) $\Gamma \circ \Gamma = \Gamma$.
Cho $\Gamma$ là một sự tương ứng giữa X và X, và G là đồ thị của nó. Nếu $\Gamma$ là một quan hệ tương đương trên X, thì $(x, x) \in G$ với mọi $x \in X$; do đó X là miền xác định của $\Gamma$. Quan hệ $(x, y) \in G$ tương đương với $(y, x) \in G$, do đó tương đương với $(x, y) \in \overset{-1}{G}$, nên $G = \overset{-1}{G}$ và vì thế $\Gamma = \overset{-1}{\Gamma}$. Các quan hệ $(x, y) \in G$ và $(y, z) \in G$ kéo theo $(x, z) \in G$, nên $G \circ G \subset G$; ngược lại, $(x, y) \in G$ kéo theo $(x, x) \in G$ và do đó $(x, y) \in G \circ G$, nên $G \subset G \circ G$; vậy $G = G \circ G$ và do đó $\Gamma = \Gamma \circ \Gamma$.
¶ Ngược lại, giả sử rằng các điều kiện (a), (b), và (c) được thỏa mãn. Quan hệ $(x, y) \in G$ là đối xứng (theo (b)) và bắc cầu (theo (c)); do đó nó là một quan hệ tương đương, và theo (a) nó là một quan hệ tương đương trên X.

### 2. CÁC LỚP TƯƠNG ĐƯƠNG ; TẬP THƯƠNG

Cho $f$ là một hàm, E là tập xác định của nó, F là đồ thị của nó. Quan hệ "$x \in E$ và $y \in E$ và $f(x) = f(y)$" là một quan hệ tương đương trên E, được gọi là quan hệ tương đương *liên kết với f*. Nó tương đương với quan hệ $(\exists z)((x, z) \in F$ và $(y, z) \in F)$, tức là với $(\exists z)((x, z) \in F$ và $(z, y) \in \overset{-1}{F})$, và do đó đồ thị của nó là $\overset{-1}{F} \circ F$.

¶ Bây giờ ta sẽ chỉ ra rằng mọi quan hệ tương đương $\mathrm{R}$ trên một tập hợp $\mathrm{E}$ đều thuộc kiểu này. Gọi $\mathrm{G}$ là đồ thị của $\mathrm{R}$. Với mỗi $x \in \mathrm{E}$, tập hợp (không rỗng) $\mathrm{G}(x) \subset \mathrm{E}$ được gọi là *lớp tương đương của $x$ đối với* $\mathrm{R}$; do đó nó là tập hợp tất cả các $y \in \mathrm{E}$ sao cho $\mathrm{R}\{x, y\}$. Mọi tập hợp có thể viết dưới dạng $\mathrm{G}(x)$ với một $x \in \mathrm{E}$ nào đó đều được gọi là một lớp tương đương (đối với $\mathrm{R}$). Một phần tử của một lớp tương đương được gọi là một *đại diện* của lớp đó. Tập hợp các lớp tương đương đối với $\mathrm{R}$ (nghĩa là, tập hợp tất cả các đối tượng có dạng $\mathrm{G}(x)$ với một $x \in \mathrm{E}$ nào đó) được gọi là *tập thương* của $\mathrm{E}$ theo $\mathrm{R}$ và được ký hiệu bởi $\mathrm{E}/\mathrm{R}$. Ánh xạ $x \to \mathrm{G}(x)$ $(x \in \mathrm{E})$ có nguồn là $\mathrm{E}$ và đích là $\mathrm{E}/\mathrm{R}$ được gọi là *ánh xạ chính tắc* của $\mathrm{E}$ lên $\mathrm{E}/\mathrm{R}$.

C55. *Cho* $\mathrm{R}$ *là một quan hệ tương đương trên một tập hợp* $\mathrm{E}$, *và cho $p$ là ánh xạ chính tắc từ* $\mathrm{E}$ *lên* $\mathrm{E}/\mathrm{R}$. *Khi đó*

$$\mathrm{R}\{x, y\} \Leftrightarrow (p(x) = p(y)).$$

Với ký hiệu trên, cho $x$ và $y$ là các phần tử của $\mathrm{E}$ sao cho

$$(x, y) \in \mathrm{G}.$$

Khi đó $x \in \mathrm{E}$ và $y \in \mathrm{E}$; ta chứng minh rằng $\mathrm{G}(x) = \mathrm{G}(y)$. Vì $y \in \mathrm{G}(x)$, nên ta có (Mệnh đề 1) $\mathrm{G}(y) \subset (\mathrm{G} \circ \mathrm{G})(x) = \mathrm{G}(x)$. Mặt khác, ta cũng có $(y, x) \in \mathrm{G}$, do đó $\mathrm{G}(x) \subset \mathrm{G}(y)$ và vì thế

$$\mathrm{G}(x) = \mathrm{G}(y),$$

nghĩa là, $p(x) = p(y)$. Ngược lại, nếu $\mathrm{G}(x) = \mathrm{G}(y)$, thì ta có $y \in \mathrm{G}(y) = \mathrm{G}(x)$, nên $(x, y) \in \mathrm{G}$. Điều này kết thúc chứng minh.

¶ Một tiết diện của ánh xạ chính tắc $p$ từ $\mathrm{E}$ lên $\mathrm{E}/\mathrm{R}$ (§ 3, no. 8, Định nghĩa 11) được gọi vắn tắt là một *tiết diện* của $\mathrm{E}$ (đối với quan hệ $\mathrm{R}$).

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s6-n2-exa-1 .statement tag=03SD}

Cho $\mathrm{R}$ là quan hệ tương đương "$x \in \mathrm{E}$ và $y \in \mathrm{E}$ và $x = y$" trên một tập hợp $\mathrm{E}$. Khi đó lớp tương đương của $x \in \mathrm{E}$ là tập hợp $\{x\}$, và ánh xạ chính tắc $x \to \{x\}$ từ $\mathrm{E}$ lên $\mathrm{E}/\mathrm{R}$ là song ánh.

#### Ví dụ 2 {#ens-ii-s6-n2-exa-2 .statement tag=03SE}

Cho $\mathrm{E}$, $\mathrm{F}$ là hai tập hợp và gọi $\mathrm{R}$ là quan hệ tương đương trên $\mathrm{E} \times \mathrm{F}$ liên kết với ánh xạ $\mathrm{pr}_1$ từ $\mathrm{E} \times \mathrm{F}$ lên $\mathrm{E}$. Các lớp tương đương đối với $\mathrm{R}$ là các tập hợp có dạng $\{x\} \times \mathrm{F}$, trong đó $x \in \mathrm{E}$; ánh xạ $x \to \{x\} \times \mathrm{F}$ là một song ánh từ $\mathrm{E}$ lên $(\mathrm{E} \times \mathrm{F})/\mathrm{R}$.

Cho $\mathrm{R}$ là một quan hệ tương đương trên một tập hợp $\mathrm{E}$. Tập thương $\mathrm{E}/\mathrm{R}$ là một tập con của $\mathfrak{P}(\mathrm{E})$, và ánh xạ đồng nhất của $\mathrm{E}/\mathrm{R}$ là một *phân hoạch* của $\mathrm{E}$ (§ 4, no. 7); thật vậy, nếu $\mathrm{G}$ là đồ thị của $\mathrm{R}$, thì ta có $x \in \mathrm{G}(x)$ với mọi $x \in \mathrm{E}$,

và nếu hai lớp tương đương $\mathrm{G}(x)$ và $\mathrm{G}(y)$ có một phần tử chung $z$, thì $\mathrm{R}\{x,\ z\}$ và $\mathrm{R}\{y,\ z\}$, suy ra $\mathrm{G}(x) = \mathrm{G}(y)$. Hơn nữa, quan hệ

$$(\exists \mathrm{X})(\mathrm{X} \in \mathrm{E}/\mathrm{R} \text{ và } x \in \mathrm{X} \text{ và } y \in \mathrm{X})$$

là tương đương với $\mathrm{R}\{x,\ y\}$.

¶ Ngược lại, cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một phân hoạch của một tập hợp E. Ngay lập tức kiểm tra được rằng quan hệ $(\exists \iota)(\iota \in \mathrm{I}$ and $x \in \mathrm{X}_\iota$ and $y \in \mathrm{Y}_\iota)$ là một quan hệ tương đương R trên E; các lớp tương đương đối với R chính là các tập hợp $\mathrm{X}_\iota$ của phân hoạch, và ánh xạ $\iota \to \mathrm{X}_\iota$ là một song ánh từ I lên E/R. Mọi tập con S của E sao cho, với mỗi $\iota \in \mathrm{I}$, tập hợp $\mathrm{S} \cap \mathrm{X}_\iota$ chỉ gồm một phần tử được gọi là một *hệ đại diện* (hay một *transversal*) của các lớp tương đương đối với R. Tên gọi này cũng được dùng để chỉ mọi đơn ánh từ một tập hợp K vào E sao cho ảnh của K dưới đơn ánh này là một hệ đại diện của các lớp tương đương đối với R; ví dụ, mọi *tiết diện* của E đối với R.

### 3. CÁC QUAN HỆ TƯƠNG THÍCH VỚI MỘT QUAN HỆ TƯƠNG ĐƯƠNG

Cho $\mathrm{R}\{x,\ x'\}$ là một quan hệ tương đương và cho $\mathrm{P}\{x\}$ là một quan hệ. Quan hệ $\mathrm{P}\{x\}$ được gọi là *tương thích với quan hệ tương đương* $\mathrm{R}\{x,\ x'\}$ (đối với $x$) nếu ta có

$$(\mathrm{P}\{x\} \text{ và } \mathrm{R}\{x,\ y\}) \Rightarrow \mathrm{P}\{y\},$$

trong đó $y$ chỉ một chữ cái không xuất hiện trong P cũng không xuất hiện trong R.

Ví dụ, từ C43 (Chương I, §5), no. 1) suy ra rằng mọi quan hệ $\mathrm{P}\{x\}$ đều tương thích với quan hệ tương đương $x = x'$.

C56. *Cho* $\mathrm{R}\{x,\ x'\}$ *là một quan hệ tương đương trên một tập hợp* E, *và cho* $\mathrm{P}\{x\}$ *là một quan hệ không chứa chữ cái* $x'$ *và tương thích (đối với* $x$*) với quan hệ tương đương* $\mathrm{R}\{x,\ x'\}$. *Khi đó, nếu* $t$ *không xuất hiện trong* $\mathrm{P}\{x\}$, *thì quan hệ "*$t \in \mathrm{E}/\mathrm{R}$ *và* $(\exists x)(x \in t$ *và* $\mathrm{P}\{x\})$*" tương đương với quan hệ "*$t \in \mathrm{E}/\mathrm{R}$ *và* $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$*".*

Cho $t \in \mathrm{E}/\mathrm{R}$. Nếu tồn tại $a \in t$ sao cho $\mathrm{P}\{a\}$, thì với mỗi $x \in t$ ta có $\mathrm{R}\{a,\ x\}$ và do đó $\mathrm{P}\{x\}$. Suy ra $(\exists x)(x \in t$ và $\mathrm{P}\{x\})$ kéo theo $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$. Điều đảo lại là hiển nhiên vì $t \in \mathrm{E}/\mathrm{R}$ kéo theo $t \neq \emptyset$.

¶ Quan hệ

$$t \in \mathrm{E}/\mathrm{R} \text{ và } (\exists x)(x \in t \text{ và } \mathrm{P}\{x\})$$

được gọi là *cảm sinh bởi* $P\{x\}$ *khi chuyển qua thương* (đối với $x$) đối với R. Nếu quan hệ này được ký hiệu bởi $P'\{t\}$, và nếu $f$ là ánh xạ chính tắc từ E lên E/R, thì quan hệ

$$y \in E \text{ và } P'\{f(y)\}$$

(trong đó $y$ không xuất hiện trong $P\{x\}$) *tương đương* với ( $y \in E$ và $P\{y\}$), như được kiểm chứng ngay lập tức.

### 4. CÁC TẬP CON BÃO HÒA

Cho $R\{x, y\}$ là một quan hệ tương đương trên một tập hợp E, và A là một tập con của E. A được gọi là *bão hòa đối với* R nếu quan hệ $x \in A$ tương thích (đối với $x$) với $R\{x, y\}$; hay, tương đương, nếu *với mỗi $x \in A$ lớp tương đương của $x$ được chứa trong* A. Nói cách khác, một tập hợp là bão hòa đối với R khi và chỉ khi nó là *hợp của một tập hợp các lớp tương đương đối với* R.

¶ Cho $f$ là ánh xạ chính tắc của E lên E/R. Nếu A bão hòa đối với R, thì lớp tương đương của mỗi $x \in A$, bằng $\overset{-1}{f}\langle\{f(x)\}\rangle$, được chứa trong A, và do đó $\overset{-1}{f}\langle f\langle A\rangle\rangle \subset A$; vì trong mọi trường hợp ta đều có $A \subset \overset{-1}{f}\langle f\langle A\rangle\rangle$, suy ra $\overset{-1}{f}\langle f\langle A\rangle\rangle = A$. Ngược lại, nếu $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$, thì với mọi $x \in A$ lớp tương đương $K = f(x)$ của $x$ đối với R là một phần tử của $f\langle A\rangle$; và vì $K = \overset{-1}{f}\langle\{K\}\rangle$, ta có $K \subset \overset{-1}{f}\langle f\langle A\rangle\rangle = A$. Như vậy các tập con của E bão hòa đối với R chính xác là các tập con A của E sao cho $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$. Tương đương, chúng là các tập con của E có dạng $\overset{-1}{f}\langle B\rangle$, với $B \subset E/R$; vì quan hệ $A = \overset{-1}{f}\langle B\rangle$ kéo theo $B = f\langle A\rangle$, nên $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$.

¶ Nếu $(X_\iota)_{\iota \in I}$ là một họ các tập con bão hòa của E, thì các tập hợp $\bigcup_{\iota \in I} X_\iota$ và $\bigcap_{\iota \in I} X_\iota$ là bão hòa (§4, Mệnh đề 3 và 4). Nếu A là một tập con bão hòa của E, thì $\complement_E A$ cũng vậy (§4, Mệnh đề 6).

¶ Bây giờ cho A là một tập con tùy ý của E. Khi đó tập hợp $\overset{-1}{f}\langle f\langle A\rangle\rangle$ chứa A và là bão hòa. Ngược lại, nếu A′ là một tập con bão hòa của E chứa A, thì ta có $f\langle A'\rangle \supset f\langle A\rangle$, nên

$$A' = \overset{-1}{f}\langle f\langle A'\rangle\rangle \supset \overset{-1}{f}\langle f\langle A\rangle\rangle.$$

Vì thế ta có thể nói rằng $\overset{-1}{f}\langle f\langle A\rangle\rangle$ là tập con bão hòa "nhỏ nhất" của E chứa A (xem Chương III); tập hợp này được gọi là *bão hòa*

của A đối với quan hệ R. Ngay lập tức thấy rằng bão hòa của A là hợp của các lớp tương đương của các phần tử của A. Nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập con của E và nếu $\mathrm{A}_\iota$ là bão hòa của $\mathrm{X}_\iota$ đối với R, thì bão hòa của $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ là $\bigcup_{\iota \in \mathrm{I}} \mathrm{A}_\iota$ (§4, Mệnh đề 3).

### 5. CÁC ÁNH XẠ TƯƠNG THÍCH VỚI CÁC QUAN HỆ TƯƠNG ĐƯƠNG

Cho R là một quan hệ tương đương trên một tập hợp E, và cho $f$ là một hàm có miền xác định E. Khi đó, người ta nói rằng $f$ *tương thích với quan hệ* R nếu quan hệ $y = f(x)$ tương thích (đối với $x$) với quan hệ $\mathrm{R}\{x,\ x'\}$.

¶ Nói như thế cũng tương đương với việc nói rằng hạn chế của $f$ trên mỗi lớp tương đương là một ánh xạ hằng, trong trường hợp đó ta nói rằng *$f$ là hằng trên mỗi lớp tương đương đối với* R. Nếu $g$ là ánh xạ chính tắc của E lên E/R, thì một mệnh đề tương đương là quan hệ $g(x) = g(x')$ kéo theo $f(x) = f(x')$; do đó (§3, Mệnh đề 9) ta có tiêu chuẩn sau :

C57. *Cho* R *là một quan hệ tương đương trên một tập hợp* E, *và cho g là ánh xạ chính tắc của* E *lên* E/R. *Khi đó một ánh xạ f từ* E *vào* F *tương thích với* R *khi và chỉ khi f có thể được viết dưới dạng h $\circ$ g, trong đó h là một ánh xạ từ* E/R *vào* F. *Ánh xạ h được xác định duy nhất bởi f; nếu s là một tiết diện bất kỳ của g, ta có h $= f \circ s$.*

Ánh xạ $h$ được gọi là *cảm sinh bởi f khi chuyển qua thương* đối với R.

¶ Cho $f$ là một ánh xạ từ một tập hợp E vào một tập hợp F, và đặt $\mathrm{A} = f\langle \mathrm{E}\rangle \subset \mathrm{F}$. Gọi R là quan hệ tương đương liên kết với $f$ (số 2); hiển nhiên $f$ tương thích với R. Hơn nữa, ánh xạ $h$ cảm sinh bởi $f$ khi chuyển qua thương là một *đơn ánh* từ E/R vào F : thật vậy, nếu $t$, $t'$ là các lớp tương đương đối với R sao cho $h(t) = h(t')$, thì ta có $f(x) = f(x')$ với mọi $x \in t$ và $x' \in t'$, điều này kéo theo $t = t'$ theo định nghĩa của R. Gọi $k$ là ánh xạ từ E/R lên A có cùng đồ thị với $h$; khi đó $k$ là *song ánh*. Nếu $j$ là đơn ánh chính tắc của A vào F và nếu $g$ là ánh xạ chính tắc từ E lên E/R, thì ta có thể viết

$$f = j \circ k \circ g.$$

Quan hệ này được gọi là *phân tích chính tắc của f*.

¶ Cho $f$ là một ánh xạ của một tập hợp E vào một tập hợp F, R là một quan hệ tương đương trên E, và S là một quan hệ tương đương trên F. Gọi $u$ là ánh xạ chính tắc của E lên E/R, và $v$ là ánh xạ chính tắc

ánh xạ từ $F$ lên $F/S$. Ánh xạ $f$ được gọi là *tương thích với các quan hệ tương đương* $R$ và $S$ nếu $v\mathbin{\circ}f$ tương thích với $R$; điều đó có nghĩa là quan hệ $x\equiv x'$ (mod $R$) *kéo theo* $f(x)\equiv f(x')$ (mod $S$). Khi đó, ánh xạ $h$ từ $E/R$ vào $F/S$ được cảm sinh bởi $v\mathbin{\circ}f$ khi chuyển qua thương theo $R$ được gọi là *ánh xạ cảm sinh bởi $f$ khi chuyển qua các thương theo $R$ và $S$*; nó được đặc trưng bởi quan hệ $v\mathbin{\circ}f=h\mathbin{\circ}u$.

### 6. ẢNH NGƯỢC CỦA MỘT QUAN HỆ TƯƠNG ĐƯƠNG; QUAN HỆ TƯƠNG ĐƯƠNG CẢM SINH

Cho $\varphi$ là một ánh xạ từ một tập hợp $E$ vào một tập hợp $F$, và $S$ là một quan hệ tương đương trên $F$. Nếu $u$ là ánh xạ chính tắc của $F$ lên $F/S$, thì quan hệ tương đương liên kết với ánh xạ $u\mathbin{\circ}\varphi$ từ $E$ vào $F/S$ được gọi là *ảnh ngược* của $S$ theo $\varphi$; nếu $R$ là quan hệ này, thì $R\{x,y\}$ tương đương với $S\{\varphi(x),\varphi(y)\}$, và các lớp tương đương đối với $R$ là các ảnh ngược theo $\varphi$ của các lớp tương đương đối với $S$ cắt $\varphi\langle E\rangle$.

¶ Đặc biệt, xét một quan hệ tương đương $R$ trên một tập hợp $E$, và cho $A$ là một tập con của $E$; khi đó ảnh ngược của $R$ qua đơn ánh $j$ của $A$ vào $E$ được gọi là quan hệ tương đương *cảm sinh* bởi $R$ trên $A$, và được ký hiệu bởi $R_A$.

¶ Các lớp tương đương đối với $R_A$ là các *vết* trên $A$ của các lớp tương đương đối với $R$ cắt $A$. Phép đơn ánh $j$ hiển nhiên tương thích với các quan hệ $R_A$ và $R$; ánh xạ $h$ từ $A/R_A$ vào $E/R$ được cảm sinh bởi $j$ khi chuyển qua thương theo $R_A$ và $R$ là một ánh xạ *đơn ánh* từ $A/R_A$ vào $E/R$: thật vậy, nếu $f$ (resp. $g$) là ánh xạ chính tắc từ $E$ lên $E/R$ (resp. từ $A$ lên $A/R_A$), thì quan hệ $h(g(x))=h(g(x'))$, trong đó $x\in A$ và $x'\in A$, tương đương với $f(x)=f(x')$ và do đó với $g(x)=g(x')$. Ảnh $h\langle A/R_A\rangle$ bằng $f\langle A\rangle$. Nếu $k$ là ánh xạ song ánh từ $A/R_A$ lên $f\langle A\rangle$ có cùng đồ thị với $h$, thì $k$ và ánh xạ nghịch đảo của nó được gọi là *chính tắc*.

### 7. THƯƠNG CỦA CÁC QUAN HỆ TƯƠNG ĐƯƠNG

Cho $R$, $S$ là hai quan hệ tương đương theo hai chữ $x$, $y$. Ta sẽ nói rằng $S$ *mịn hơn* $R$ (hoặc rằng $R$ *thô hơn* $S$) nếu quan hệ $S\Rightarrow R$ là đúng. Nếu $R$ và $S$ là các quan hệ tương đương trên cùng một tập hợp $E$, thì mệnh đề nói rằng $S$ mịn hơn $R$ có nghĩa là đồ thị của $S$ được chứa trong đồ thị của $R$, hay cũng có nghĩa là mọi lớp tương đương đối với $S$ đều được chứa trong một lớp tương đương đối với $R$; hoặc, tương đương, mọi lớp tương đương đối với $R$ đều bão hòa đối với $S$.

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s6-n7-exa-1 .statement tag=03SF}

Quan hệ "$x \in E$ và $y \in E$ và $x = y$" mịn hơn mọi quan hệ tương đương trên E. Quan hệ "$x \in E$ và $y \in E$" thô hơn mọi quan hệ tương đương trên E.

#### Ví dụ 2 {#ens-ii-s6-n7-exa-2 .statement tag=03SG}

Quan hệ tương đương "$x \in \mathbf{Z}$ và $y \in \mathbf{Z}$ và $x - y$ chia được cho 4" mịn hơn quan hệ tương đương "$x \in \mathbf{Z}$ và $y \in \mathbf{Z}$ và $x - y$ chia được cho 2". \*

Cho R và S là hai quan hệ tương đương trên cùng một tập hợp E, sao cho S mịn hơn R. Gọi $f$ và $g$ lần lượt là các ánh xạ chính tắc của E lên E/R và của E lên E/S; khi đó hàm $f$ tương thích với S. Gọi $h$ là hàm cảm sinh bởi $f$ khi chuyển qua thương theo S; khi đó $h$ là một ánh xạ từ E/S lên E/R. Quan hệ tương đương liên kết với $h$ trên E/S được gọi là *thương của* R *theo* S và được ký hiệu là R/S. Quan hệ $x \equiv y \pmod{R}$ tương đương với $g(x) \equiv g(y) \pmod{R/S}$, và các lớp tương đương đối với R/S là các ảnh qua $g$ của các lớp tương đương đối với R. Gọi $h = j \circ h_2 \circ h_1$ là phân tích chính tắc (no. 5) của ánh xạ $h$. Khi đó $h_1$ là ánh xạ chính tắc từ E/S lên (E/S)/(R/S), $j$ là ánh xạ đồng nhất của E/R, và $h_2$ là một ánh xạ một-một từ (E/S)/(R/S) lên E/R. Ánh xạ $h_2$ và ánh xạ nghịch đảo của nó được gọi là *chính tắc*.

¶ Ngược lại, xét một quan hệ tương đương tùy ý T trên tập hợp E/S, và gọi R là quan hệ tương đương trên E là ảnh ngược qua $g$ của quan hệ T (số 6). Vì quan hệ $x \equiv y \pmod{R}$ tương đương với $g(x) \equiv g(y) \pmod{T}$, suy ra T tương đương với R/S.

### 8. TÍCH CỦA HAI QUAN HỆ TƯƠNG ĐƯƠNG

Cho $R\{x, y\}$ và $R'\{x', y'\}$ là hai quan hệ tương đương. Gọi $S\{u, v\}$ là quan hệ

$$(\exists x)(\exists y)(\exists x')(\exists y')(u = (x, x') \text{ và } v = (y, y') \text{ và } R\{x, y\} \text{ và } R'\{x', y'\});$$

người ta kiểm tra ngay lập tức rằng $S\{u, v\}$ là một quan hệ tương đương, được gọi là *tích* của R và R', và được ký hiệu bởi $R \times R'$. Giả sử rằng R là một quan hệ tương đương trên một tập hợp E và R' là một quan hệ tương đương trên một tập hợp E'. Khi đó quan hệ $S\{u, u\}$ tương đương với

$$(\exists x)(\exists x')(u = (x, x') \text{ và } R\{x, x\} \text{ và } R'\{x', x'\})$$

tức là, với $(\exists x)(\exists x')(u = (x, x')$ và $x \in E$ và $x' \in E')$, do đó với $u \in E \times E'$. Suy ra $R \times R'$ là một quan hệ tương đương trên $E \times E'$. Nếu

$$u = (x, x')$$

là một phần tử của $E \times E'$, thì quan hệ $S\{u, v\}$ tương đương với

$$(\exists y)(\exists y')(v = (y, y') \text{ và } R\{x, y\} \text{ và } R'\{x', y'\});$$

nếu $G$ và $G'$ lần lượt là các đồ thị của $R$ và $R'$, thì quan hệ này đến lượt nó tương đương với $v \in G(x) \times G(x')$. Do đó *mọi lớp tương đương đối với* $R \times R'$ *đều là tích của một lớp tương đương đối với* $R$ *và một lớp tương đương đối với* $R'$, *và ngược lại.*

¶ Cho $f$ và $f'$ lần lượt là các ánh xạ chính tắc từ $E$ lên $E/R$ và từ $E'$ lên $E'/R'$, và $f \times f'$ là mở rộng chính tắc của $f$ và $f'$ tới các tập hợp tích (§ 3, no. 9). Khi đó $(f \times f')(x, x') = (f(x), f'(x'))$ với mọi $(x, x') \in E \times E'$. Ảnh ngược qua $f \times f'$ của một phần tử $(u, u')$ của $(E/R) \times (E'/R')$ chính là tích $u \times u'$ của lớp tương đương $u$ đối với $R$ và lớp tương đương $u'$ đối với $R'$. Suy ra quan hệ tương đương liên kết với $f \times f'$ là tương đương với $R \times R'$. Do đó ánh xạ $f \times f'$ có thể được viết thành $h \circ g$, trong đó $g$ là ánh xạ chính tắc từ $E \times E'$ lên

$$(E \times E')/(R \times R')$$

và $h$ là một song ánh từ $(E \times E')/(R \times R')$ lên

$$(E/R) \times (E'/R');$$

ánh xạ $h$ này và ánh xạ nghịch đảo của nó được gọi là *chính tắc*.

#### Nhận xét {#ens-ii-s6-n8-rem-1 .statement tag=03IY}

Cho $P\{x, x'\}$ là một quan hệ trong đó các chữ $y$, $y'$ không xuất hiện. Người ta nói P là *tương thích* với các quan hệ tương đương $R\{x, y\}$ và $R'\{x', y'\}$ (đối với $x$ và $x'$) nếu quan hệ $(P\{x, x'\}$ và $R\{x, y\}$ và $R'\{x', y'\})$ suy ra $P\{y, y'\}$. Cho $Q\{u\}$ là quan hệ $(\exists x)(\exists x')(u = (x, x')$ và $P\{x, x'\})$; khi đó nói rằng $Q\{u\}$ tương thích (đối với $u$) với quan hệ tương đương $S\{u, v\}$, tích của $R$ và $R'$, cũng là cùng một điều.

### 9. CÁC LỚP ĐỐI TƯỢNG TƯƠNG ĐƯƠNG

Cho $R\{x, y\}$ là một quan hệ tương đương, quan hệ này có thể không có đồ thị. Hiển nhiên là nếu $x$, $x'$, $y$ là ba chữ phân biệt, thì quan hệ $R\{x, x'\}$ kéo theo "$R\{x, y\} \Longleftrightarrow R\{x', y\}$" và do đó cũng kéo theo quan hệ $(\forall y)(R\{x, y\} \Longleftrightarrow R\{x', y\})$. Theo lược đồ S7 (Chương I, § 5, no. 1), nếu đặt $\theta\{x\} = \tau_y(R\{x, y\})$, thì quan hệ $R\{x, x'\}$ kéo theo

$$\theta\{x\} = \theta\{x'\}.$$

Mặt khác, chú ý rằng theo định nghĩa $R\{x, \theta\{x\}\}$ là quan hệ $(\exists y)(R\{x, y\})$ và do đó (no. 1) là tương đương với $R\{x, x\}$. Suy ra quan hệ $(R\{x, x\}$ and $R\{x', x'\}$ and $\theta\{x\} = \theta\{x'\})$ là *tương đương* với $R\{x, x'\}$, vì nó kéo theo, theo S6 (Chương I, §5, no. 1), quan hệ

$$(R\{x, x\} \text{ và } R\{x', x'\} \text{ và } (R\{x', \theta\{x\}\} \Leftrightarrow R\{x', \theta\{x'\}\})),$$

do đó cũng kéo theo $(R\{x, \theta\{x\}\}$ and $R\{x', \theta\{x\}\})$, và cuối cùng là $R\{x, x'\}$ theo tính bắc cầu và tính đối xứng. Và vì ngược lại, $R\{x, x'\}$ kéo theo $R\{x, x\}$ và $R\{x', x'\}$, nên mệnh đề đã được chứng minh. Số hạng $\theta\{x\}$ được gọi là *lớp các đối tượng tương đương với x* (đối với quan hệ R).

¶ Bây giờ giả sử rằng T là một số hạng sao cho quan hệ

(1) $$(\forall y)(R\{y, y\} \Rightarrow (\exists x)(x \in T \text{ và } R\{x, y\}))$$

là đúng. Khi đó quan hệ $(\exists x)(R\{x, x\}$ và $z = \theta\{x\})$ là *xác định tập theo z*. Thật vậy, ta có thể giả sử rằng $x \in T$ kéo theo $R\{x, x\}$; chỉ cần thay thế T bằng tập hợp tất cả các $x \in T$ sao cho $R\{x, x\}$ (nhận thấy rằng $R\{x, y\}$ kéo theo $R\{x, x\}$). Gọi $\Theta$ là tập hợp của tất cả các đối tượng có dạng $\theta\{x\}$ với $x \in T$ (§1, no. 6). Giả sử rằng $R\{y, y\}$ là đúng; khi đó tồn tại $x \in T$ sao cho $R\{x, y\}$ và do đó $\theta\{y\} = \theta\{x\} \in \Theta$. Tập hợp $\Theta$ được gọi là *tập hợp các lớp của các đối tượng tương đương* đối với R; và với mỗi $x$ sao cho $R\{x, x\}$, $\theta\{x\}$ là phần tử *duy nhất* $z \in \Theta$ sao cho $R\{x, z\}$.

Với cùng giả thiết đó, cho $A\{x\}$ là một số hạng sao cho $R\{x, y\}$ kéo theo $A\{x\} = A\{y\}$. Khi đó quan hệ $(\exists x)(R\{x, x\}$ và $z = \{x\})$ xác định tập theo $z$, vì $R\{x, x\}$, tương đương với $R\{x, \theta\{x\}\}$, kéo theo $A\{x\} = A\{\theta\{x\}\}$, và do đó nếu E là tập hợp các đối tượng dạng $A\{t\}$ với $t \in \Theta$, thì $R\{x, x\}$ kéo theo $A\{x\} \in E$. Nếu $f$ là hàm $t \to A\{t\}$ $(t \in \Theta, A\{t\} \in E)$, thì quan hệ $R\{x, x\}$ kéo theo $A\{x\} = f(\theta\{x\})$.

Đặc biệt, nếu R là một quan hệ tương đương *trên một tập hợp* F, ta có thể lấy $A\{x\}$ là *lớp tương đương của x đối với* R (no. 2), và khi đó hàm $f$ là một *song ánh* từ $\Theta$ lên tập thương F/R; điều này biện minh cho thuật ngữ đã được đưa vào.

\* *Ví dụ*. Gọi $R\{x, y\}$ là quan hệ tương đương "$x$ và $y$ là hai không gian vectơ có cùng số chiều hữu hạn trên $\mathbf{C}$"; quan hệ này không có đồ thị. Nó thỏa mãn điều kiện (1) khi T là tập hợp mọi không gian con vectơ của $\mathbf{C}^{(\mathbf{N})}$, hoặc khi tập con T' của T gồm các không gian $\mathbf{C}^n$ $(n \in \mathbf{N})$ với các quy ước rằng $\mathbf{C}^0$ chỉ gồm điểm 0 của $\mathbf{C}^{(\mathbf{N})}$ và rằng $\mathbf{C}^n$ $(n > 0)$ là tổng của $n$ thành phần đầu tiên của tổng trực tiếp $\mathbf{C}^{(\mathbf{N})}$. Với lựa chọn thứ hai này ta có $\Theta = T'$.\*

### Bài tập {#ens-ii-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
