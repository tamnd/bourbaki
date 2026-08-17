---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 3
section_title: Correspondences
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 75-90, 124-125
pdf_pages: 0082-0097, 0131-0132
extraction: ocr
subsections:
    - "no": 1
      title: GRAPHS AND CORRESPONDENCES
      page: 75
      pdf_page: 82
    - "no": 2
      title: INVERSE OF A CORRESPONDENCE
      page: 78
      pdf_page: 85
    - "no": 3
      title: COMPOSITION OF TWO CORRESPONDENCES
      page: 78
      pdf_page: 85
    - "no": 4
      title: FUNCTIONS
      page: 81
      pdf_page: 88
    - "no": 5
      title: RESTRICTIONS AND EXTENSIONS OF FUNCTIONS
      page: 82
      pdf_page: 89
    - "no": 6
      title: DEFINITION OF A FUNCTION BY MEANS OF A TERM
      page: 83
      pdf_page: 90
    - "no": 7
      title: COMPOSITION OF TWO FUNCTIONS. INVERSE FUNCTION
      page: 84
      pdf_page: 91
    - "no": 8
      title: RETRACTIONS AND SECTIONS
      page: 86
      pdf_page: 93
    - "no": 9
      title: FUNCTIONS OF TWO ARGUMENTS
      page: 89
      pdf_page: 96
statements: 37
exercises: 11
content_sha256: 64b1d189bf1841aed3688dfeca19a88aa39eeaa80b67f483532cc750d8671d8e
translated_from: content/en/ens/II/03_s3_correspondences.md
source_content_sha256: 8a4115cf22d57ea009a5fd57d02c81b51fc1ae5d0adb1e6d32b5c21f6d93004f
translation_model: nemotron-3-ultra-free, gpt-5-6, nemotron-3.5-lightning-free, hy3-free, laguna-s-2.1-free, gpt-5.4-mini, gpt-5.4
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: 541d5f2fb27eb2a1e4efa6cf31860539b8257ba59f4cf8e6ab0af9e7c321ab97
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. ĐỐI ỨNG

### 1. ĐỒ THỊ VÀ ĐỐI ỨNG

#### Định nghĩa 1 {#ens-ii-s3-def-1 .statement tag=03PG}

G *được gọi là một đồ thị nếu mọi phần tử của* G *là một cặp có thứ tự*, tức là nếu quan hệ

$$(\forall z)(z \in G \Rightarrow (z \text{ là một cặp có thứ tự }))$$

*là đúng.*

Nếu G là một đồ thị, quan hệ $(x, y) \in G$ được diễn đạt bằng cách nói rằng "$y$ đối ứng với $x$ dưới G".

Cho $\boldsymbol{R}\{x, y\}$ là một quan hệ, trong đó $x$ và $y$ là các chữ cái phân biệt. Cho $\boldsymbol{G}$ là một chữ cái, phân biệt với $x$ và $y$, mà không xuất hiện trong $\boldsymbol{R}$. Nếu quan hệ

$$(\exists \boldsymbol{G})(\boldsymbol{G} \text{ là một đồ thị và } (\forall x)(\forall y)(\boldsymbol{R} \Leftrightarrow ((x, y) \in \boldsymbol{G})))$$

Là đúng, quan hệ $\boldsymbol{R}$ được nói là *có đồ thị* (đối với các chữ $x$ và $y$). Đồ thị $\boldsymbol{G}$ khi đó là duy nhất nhờ Tiên đề ngoại diên, và được gọi là *đồ thị* của $\boldsymbol{R}$ đối với $x$ và $y$.

Cho $Z$ là một chữ, phân biệt với $x$ và $y$, mà không xuất hiện trong $R$. Nếu quan hệ

$$(\exists Z)(\forall x)(\forall y)(R \Rightarrow ((x, y) \in Z))$$

đúng, thì $R$ có một đồ thị; ta có thể lấy đồ thị này là tập hợp các cặp có thứ tự $z$ sao cho $z \in Z$ và $R \{ \mathrm{pr}_1 z,\ \mathrm{pr}_2 z \}$ ($z$ là một chữ cái phân biệt với $x$, $y$, $Z$ không xuất hiện trong $R$). Điều kiện này được thỏa mãn nếu ta biết một số hạng $T$, không chứa $x$ cũng như $y$, sao cho $R \Rightarrow ((x,\ y) \in T)$ là đúng.

#### Mệnh đề 1 {#ens-ii-s3-prop-1 .statement tag=03HI}

*Cho* G *là một đồ thị. Tồn tại duy nhất một tập hợp* A *và duy nhất một tập hợp* B *có các tính chất sau* :

(1) *quan hệ* $(\exists y)((x,\ y) \in \mathrm{G})$ *tương đương với* $x \in \mathrm{A}$;

(2) *quan hệ* $(\exists x)((x,\ y) \in \mathrm{G})$ *là tương đương với* $y \in \mathrm{B}$.

Vì ta chỉ cần lấy A (resp. B) là tập hợp của tất cả các đối tượng có dạng $\mathrm{pr}_1 z$ (resp. $\mathrm{pr}_2 z$), với $z \in \mathrm{G}$ (§ 1, no. 6). Chính xác,

$$\mathrm{A} = \mathscr{E}_x((\exists y)((x, y) \in \mathrm{G}))) \qquad \text{và} \qquad \mathrm{B} = \mathscr{E}_y((\exists x)((x,\ y) \in \mathrm{G}));$$

các tập hợp này được gọi lần lượt là *phép chiếu thứ nhất và thứ hai* của đồ thị G, hoặc *miền xác định* và *miền giá trị* của G; chúng được ký hiệu bằng $\mathrm{pr}_1 \langle \mathrm{G} \rangle$ và $\mathrm{pr}_2 \langle \mathrm{G} \rangle$ (hoặc $\mathrm{pr}_1 \mathrm{G}$ và $\mathrm{pr}_2 \mathrm{G}$ nếu không gây nhầm lẫn). Ngay lập tức ta kiểm tra được rằng $\mathrm{G} \subset (\mathrm{pr}_1 \mathrm{G}) \times (\mathrm{pr}_2 \mathrm{G})$; mọi tập hợp các cặp có thứ tự do đó là một tập con của một tích, và ngược lại. Nếu một trong hai tập hợp $\mathrm{pr}_1 \mathrm{G}$, $\mathrm{pr}_2 \mathrm{G}$ là rỗng, ta có $\mathrm{G} = \emptyset$ (§ 2, Mệnh đề 2).

#### Nhận xét {#ens-ii-s3-n1-rem-3 .statement tag=03S1}

Quan hệ $x = y$ không có đồ thị, vì phép chiếu thứ nhất của đồ thị, nếu nó tồn tại, sẽ là tập hợp của tất cả các đối tượng (cf. § 1, no. 7, Nhận xét).

#### Định nghĩa 2 {#ens-ii-s3-def-2 .statement tag=03HJ}

*Một sự tương ứng giữa một tập hợp* A *và một tập hợp* B *là một bộ ba*

$$\Gamma = (\mathrm{G},\ \mathrm{A},\ \mathrm{B}),$$

*nơi* G *là một đồ thị sao cho* $\mathrm{pr}_1 \mathrm{G} \subset \mathrm{A}$ *và* $\mathrm{pr}_2 \mathrm{G} \subset \mathrm{B}$. G *được gọi là đồ thị của* $\Gamma$, A *là nguồn, và* B *mục tiêu của* $\Gamma$.

Nếu $(x,\ y) \in \mathrm{G}$, ta nói rằng "$y$ tương ứng với $x$ trong sự tương ứng $\Gamma$". Với mỗi $x \in \mathrm{pr}_1 \mathrm{G}$, sự tương ứng $\Gamma$ được gọi là *được định nghĩa tại* $x$, và $\mathrm{pr}_1 \mathrm{G}$ được gọi là *miền xác định của* $\Gamma$; mỗi $y \in \mathrm{pr}_2 \mathrm{G}$ được gọi là một *giá trị nhận bởi* $\Gamma$, và $\mathrm{pr}_2 \mathrm{G}$ được gọi là *miền giá trị của* $\Gamma$.

Nếu $R \{ x, y \}$ là một quan hệ có đồ thị $G$ (đối với các chữ cái $x$, $y$), và nếu $A$, $B$ là hai tập hợp sao cho $\mathrm{pr}_1 G \subset A$ và $\mathrm{pr}_2 G \subset B$, thì ta

nói rằng $R$ là một *quan hệ giữa một phần tử của $A$ và một phần tử của $B$* (ứng với các chữ cái $x$, $y$). Sự tương ứng $\Gamma = (G, A, B)$ được gọi là sự tương ứng giữa $A$ và $B$ *được xác định bởi* quan hệ $R$ (ứng với $x$ và $y$).

Cho G là một đồ thị và cho X là một tập hợp. Quan hệ

$$x \in X \text{ và } (x, y) \in G$$

suy ra $(x, y) \in G$ và do đó có một đồ thị $G'$. Phép chiếu thứ hai của $G'$ gồm tất cả các đối tượng mà theo G tương ứng với các đối tượng của X.

#### Định nghĩa 3 {#ens-ii-s3-def-3 .statement tag=03PI}

*Cho* G *là một đồ thị và* X *là một tập hợp. Tập hợp tất cả các đối tượng tương ứng dưới* G *với các phần tử của* X *được gọi là ảnh của* X *dưới* G *và được ký hiệu bởi* $G\langle X \rangle$ *hoặc* $G(X)$.

¶ *Cho* $\Gamma = (G, A, B)$ *là một sự tương ứng và cho* X *là một tập con của* A. *Tập hợp* $G\langle X \rangle$ *cũng được ký hiệu bởi* $\Gamma\langle X \rangle$ *hoặc* $\Gamma(X)$ *và được gọi là ảnh của* X *dưới* $\Gamma$.

*Chú ý*

#### Nhận xét 1 {#ens-ii-s3-n1-rem-1 .statement tag=03PH}

Chính xác, $G\langle X \rangle$ ký hiệu tập hợp $\mathscr{E}_y((\exists x)(x \in X \text{ và } (x,y) \in G))$. Từ nay về sau chúng ta sẽ không thường chuyển các định nghĩa của mình sang ngôn ngữ hình thức.

#### Nhận xét 2 {#ens-ii-s3-n1-rem-2 .statement tag=03S2}

Các ký hiệu $G(X)$ và $\Gamma(X)$ đôi khi có thể dẫn đến sự nhầm lẫn với ký hiệu được đưa vào sau này (xem no. 4, Nhận xét theo sau Định nghĩa 9).

Cho G là một đồ thị. Vì quan hệ $(x, y) \in G$ ngụ ý $y \in \mathrm{pr}_2 G$, ta có $G\langle X \rangle \subset \mathrm{pr}_2 G$ với mọi tập hợp X. Vì $(x, y) \in G$ ngụ ý $x \in \mathrm{pr}_1 G$, ta có $G\langle \mathrm{pr}_1 G \rangle = \mathrm{pr}_2 G$. Ta có $G\langle \emptyset \rangle = \emptyset$, vì $x \notin \emptyset$ là một định lý. Nếu $X \subset \mathrm{pr}_1 G$ và $X \neq \emptyset$, ta có $G\langle X \rangle \neq \emptyset$.

#### Mệnh đề 2 {#ens-ii-s3-prop-2 .statement tag=03PJ}

*Cho* G *là một đồ thị và cho* X, Y *là hai tập hợp; thì quan hệ* $X \subset Y$ *ngụ ý* $G\langle X \rangle \subset G\langle Y \rangle$.

Đây là một hệ quả ngay lập tức của các định nghĩa và của C50 (§ 1, no. 4).

#### Hệ quả {#ens-ii-s3-n1-cor-1 .statement tag=03PK}

*Nếu* $A \supset \mathrm{pr}_1 G$, *ta có* $G\langle A \rangle = \mathrm{pr}_2 G$.

#### Định nghĩa 4 {#ens-ii-s3-def-4 .statement tag=03PL}

Cho G là một đồ thị và $x$ là một vật. Tập hợp $G\langle \{x\} \rangle$ (đôi khi được ký hiệu bằng $G(x)$, bằng cách lạm dụng ngôn ngữ) được gọi là tiết diện của G tại $x$.

Ta suy ra ngay lập tức từ C43 (Chương I, § 5, số 1) rằng mối quan hệ $y \in G\langle \{x\} \rangle$ tương đương với $(x, y) \in G$. Nếu G và $G'$ là hai đồ thị, mối quan hệ $G \subset G'$ vì vậy tương đương với

$$(\forall x)(G\langle \{x\} \rangle \subset G'\langle \{x\} \rangle).$$

Nếu $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ là một sự tương ứng giữa A và B, thì với mọi $x \in \mathrm{A}$, tiết diện của G tại $x$ cũng được gọi là *tiết diện của* $\Gamma$ *tại* $x$ và được ký hiệu bởi $\Gamma\langle\{x\}\rangle$ (hoặc $\Gamma(x)$).

### 2. TƯƠNG ỨNG NGHỊCH ĐẢO

Cho G là một đồ thị và $\mathrm{A} = \mathrm{pr}_1\mathrm{G}$, $\mathrm{B} = \mathrm{pr}_2\mathrm{G}$ là các hình chiếu của nó. Quan hệ $(y, x) \in \mathrm{G}$ kéo theo $(x, y) \in \mathrm{B} \times \mathrm{A}$; quan hệ này do đó có một đồ thị bao gồm tất cả các cặp có thứ tự $(x, y)$ sao cho $(y, x) \in \mathrm{G}$.

#### Định nghĩa 5 {#ens-ii-s3-def-5 .statement tag=03PM}

*Cho G là một đồ thị. Đồ thị mà các phần tử là các cặp có thứ tự $(x, y)$ sao cho $(y, x) \in \mathrm{G}$ được gọi là nghịch đảo của G và được ký hiệu bởi* $\overset{-1}{\mathrm{G}}$.

Với mọi tập hợp X, $\overset{-1}{\mathrm{G}}\langle\mathrm{X}\rangle$ được gọi là *ảnh ngược của* X *dưới* G.

¶ Rõ ràng rằng nghịch đảo của $\overset{-1}{\mathrm{G}}$ là G, và rằng

$$\mathrm{pr}_1\overset{-1}{\mathrm{G}} = \mathrm{pr}_2\mathrm{G}, \qquad \mathrm{pr}_2\overset{-1}{\mathrm{G}} = \mathrm{pr}_1\mathrm{G}.$$

Cụ thể, nếu X, Y là hai tập hợp, ta có

$$\overset{-1}{\overbrace{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

Một đồ thị G được gọi là *đối xứng* nếu $\overset{-1}{\mathrm{G}} = \mathrm{G}$.

¶ Cho $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ là một sự tươngứng giữa A và B. Vì $\mathrm{pr}_1\overset{-1}{\mathrm{G}} \subset \mathrm{B}$ và $\mathrm{pr}_2\overset{-1}{\mathrm{G}} \subset \mathrm{A}$, các $(\overset{-1}{\mathrm{G}}, \mathrm{B}, \mathrm{A})$ là *sự tươngứng giữa* A và B, gọi là *nghịch đảo* của sự tươngứng $\Gamma$, và ký hiệu bởi $\overset{-1}{\Gamma}$. Với mọi tập con Y của B, ảnh $\overset{-1}{\Gamma}\langle\mathrm{Y}\rangle$ của Y dưới $\overset{-1}{\Gamma}$ cũng được gọi là *ảnh ngược* của Y dưới $\Gamma$. rõ ràng nghịch đảo của $\overset{-1}{\Gamma}$ là $\Gamma$.

### 3. HỢP THỨC CỦA HAI TƯỢNG ĐÚNG

Cho G, G′ là hai đồ thị. Gọi A là tập hợp $\mathrm{pr}_1\mathrm{G}$ và gọi C là tập hợp $\mathrm{pr}_2\mathrm{G}'$. Quan hệ $(\exists y)((x, y) \in \mathrm{G}$ và $(y, z) \in \mathrm{G}')$ ngụ ý rằng $(x, z) \in \mathrm{A} \times \mathrm{C}$, và do đó có một đồ thị đối với $x$ và $z$.

#### Định nghĩa 6 {#ens-ii-s3-def-6 .statement tag=03PN}

*Cho G, G′ là hai đồ thị. Đồ thị (đối với $x$ và $z$) của quan hệ $(\exists y)((x, y) \in \mathrm{G}$ và $(y, z) \in \mathrm{G}')$ được gọi là hợp thành của G′ và G, và được ký hiệu bởi* $\mathrm{G}' \circ \mathrm{G}$ (hoặc đôi khi bởi $\mathrm{G}'\mathrm{G}$).

#### Mệnh đề 3 {#ens-ii-s3-prop-3 .statement tag=03HK}

*Cho* G, G′ *là hai đồ thị. Nghịch đảo của* G′ ∘ G *khi đó là* $\overset{-1}{G} \circ \overset{-1}{G'}$.

Với quan hệ "$(x, y) \in G$ và $(y, z) \in G'$" là tương đương với

$$(z, y) \in \overset{-1}{G'} \text{ và } (y, x) \in \overset{-1}{G}.$$

#### Mệnh đề 4 {#ens-ii-s3-prop-4 .statement tag=03HL}

*Cho* $G_1$, $G_2$, $G_3$ *là các đồ thị. Khi đó*

$$(G_3 \circ G_2) \circ G_1 = G_3 \circ (G_2 \circ G_1).$$

Quan hệ $(x, t) \in (G_3 \circ G_2) \circ G_1$ là tương đương với quan hệ

$$(\exists y)((x, y) \in G_1 \text{ và } \exists z((y, z) \in G_2 \text{ và } (z, t) \in G_3))$$

và do đó (theo C33 (Chương I, § 4, no. 3)) là tương đương với quan hệ

(1) $$(\exists y)(\exists z)((x, y) \in G_1 \text{ và } (y, z) \in G_2 \text{ và } (z, t) \in G_3).$$

Tương tự, quan hệ $(x, t) \in G_3 \circ (G_2 \circ G_1)$ là tương đương với

(2) $$(\exists z)(\exists y)((x, y) \in G_1 \text{ và } (y, z) \in G_2 \text{ và } (z, t) \in G_3).$$

Nhưng các quan hệ (1) và (2) là tương đương; do đó kết quả.

¶ Đồ thị $G_3 \circ (G_2 \circ G_1)$ được ký hiệu bởi $G_3 \circ G_2 \circ G_1$. Tương tự, nếu $G_1$, $G_2$, $G_3$, $G_4$ là các đồ thị, ta đặt

$$G_4 \circ (G_3 \circ G_2 \circ G_1) = G_4 \circ G_3 \circ G_2 \circ G_1;$$

và cứ tiếp tục như vậy.

#### Mệnh đề 5 {#ens-ii-s3-prop-5 .statement tag=03HM}

*Cho* G, G′ *là các đồ thị và cho* A *là một tập hợp. Khi đó*

$$(G' \circ G)\langle A \rangle = G'\langle G\langle A \rangle\rangle.$$

Bởi vì theo C33 (Chương I, § 4, no. 3) quan hệ $z \in (G' \circ G)\langle A \rangle$ tương đương với

$$(\exists y)((\exists x)(x \in A \text{ và } (x, y) \in G) \text{ và } (y, z) \in G')$$

và do đó tương đương với $(\exists y)(y \in G\langle A \rangle$ và $(y, z) \in G')$; do đó có kết quả.

¶ Nếu G và G′ là hai đồ thị, ta có $\mathrm{pr}_1(G' \circ G) = \overset{-1}{G}\langle \mathrm{pr}_1 G'\rangle$, và $\mathrm{pr}_2(G' \circ G) = G'\langle \mathrm{pr}_2 G\rangle$. Ví dụ, để chứng minh đẳng thức thứ hai trong số đó

đối với các quan hệ, chỉ cần chú ý rằng quan hệ $z \in \mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G})$ tương đương với $(\exists x)((x, z) \in \mathrm{G}' \circ \mathrm{G})$ và do đó tương đương với

$$(\exists y)((\exists x)((x, y) \in \mathrm{G}) \quad \text{và} \quad (y, z) \in \mathrm{G}');$$

nhưng điều này tương đương với $z \in \mathrm{G}'\langle \mathrm{pr}_2\mathrm{G}\rangle$.

¶ Nếu G là một đồ thị và X là một tập hợp sao cho $\mathrm{X} \subset \mathrm{pr}_1\mathrm{G}$, ta có

$$\mathrm{X} \subset \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle.$$

Vì quan hệ $x \in \mathrm{X}$ ngụ ý theo giả thiết rằng $(\exists y)((x, y) \in \mathrm{G})$; nhưng $(x, y) \in \mathrm{G}$ tương đương với $(y, x) \in \overset{-1}{\mathrm{G}}$, và mặt khác $(x, y) \in \mathrm{G}$ ngụ ý $(\exists z)(z \in \mathrm{X}$ và $(z, y) \in \mathrm{G})$; do đó $x \in \mathrm{X}$ ngụ ý

$$(\exists y)((\exists z)(z \in \mathrm{X} \quad \text{và} \quad (z, y) \in \mathrm{G}) \quad \text{và} \quad (y, x) \in \overset{-1}{\mathrm{G}}),$$

nghĩa là, $x \in \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle$.

¶ Dễ thấy rằng nếu $\mathrm{G}_1$, $\mathrm{G}_2$, $\mathrm{G}'_1$, $\mathrm{G}'_2$ là các đồ thị, thì các quan hệ $\mathrm{G}_1 \subset \mathrm{G}_2$ và $\mathrm{G}'_1 \subset \mathrm{G}'_2$ ngụ ý $\mathrm{G}'_1 \circ \mathrm{G}_1 \subset \mathrm{G}'_2 \circ \mathrm{G}_2$.

¶ Gọi $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ và $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ là hai tương ứng sao cho mục tiêu của $\Gamma$ trùng với nguồn của $\Gamma'$. Từ phần thảo luận ở trên ta có $\mathrm{pr}_1(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_1\mathrm{G} \subset \mathrm{A}$ và $\mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_2\mathrm{G}' \subset \mathrm{C}$; do đó chúng ta có thể nêu ra **định nghĩa** sau:

#### Định nghĩa 7 {#ens-ii-s3-def-7 .statement tag=03PO}

Cho $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ và $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ là hai sự tương ứng sao cho đích của $\Gamma$ là nguồn của $\Gamma'$. Khi đó sự tương ứng $(\mathrm{G}' \circ \mathrm{G}, \mathrm{A}, \mathrm{C})$ được gọi là hợp thành của $\Gamma'$ và $\Gamma$, và ký hiệu là $\Gamma' \circ \Gamma$ (hoặc đôi khi $\Gamma'\Gamma$).

Theo ngay lập tức từ Mệnh đề 5 rằng nếu X là một tập con của A thì ta có $(\Gamma' \circ \Gamma)\langle \mathrm{X}\rangle = \Gamma'\langle \Gamma\langle \mathrm{X}\rangle\rangle$. Hơn nữa, vì đích của $\overset{-1}{\Gamma'}$ giống như nguồn của $\overset{-1}{\Gamma}$, nên nghịch đảo của $\Gamma' \circ \Gamma$ là $\overset{-1}{\Gamma} \circ \overset{-1}{\Gamma'}$, theo Mệnh đề 3.

#### Định nghĩa 8 {#ens-ii-s3-def-8 .statement tag=03PP}

Nếu A là một tập hợp, tập hợp $\Delta_\mathrm{A}$ gồm toàn bộ các đối tượng có dạng $(x, x)$, trong đó $x \in \mathrm{A}$, được gọi là đường chéo của $\mathrm{A} \times \mathrm{A}$.

Rõ ràng ta có $\mathrm{pr}_1\Delta_\mathrm{A} = \mathrm{pr}_2\Delta_\mathrm{A} = \mathrm{A}$. Sự tương ứng

$$\mathrm{I}_\mathrm{A} = (\Delta_\mathrm{A}, \mathrm{A}, \mathrm{A})$$

được gọi là *tương ứng đơn vị* trên A; nó là chính nghịch đảo của nó.

Nếu $\Gamma$ là một sự tương ứng giữa A và B và nếu $\mathrm{I}_\mathrm{A}$, $\mathrm{I}_\mathrm{B}$ lần lượt là các tương ứng đơn vị trên A, B, thì $\Gamma \circ \mathrm{I}_\mathrm{A} = \mathrm{I}_\mathrm{B} \circ \Gamma = \Gamma$.

### 4. HÀM SỐ

#### Định nghĩa 9 {#ens-ii-s3-def-9 .statement tag=03HN}

*Một đồ thị* F *được gọi là đồ thị phiếm hàm nếu với mỗi x có nhiều nhất một đối tượng tương ứng với x qua* F (Chương I, § 5, no. 3). *Một sự tương ứng* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *được gọi là một hàm nếu đồ thị của nó* F *là một đồ thị phiếm hàm và nếu nguồn của nó* A *bằng miền xác định của nó* $\mathrm{pr}_1\mathrm{F}$. *Nói cách khác, một sự tương ứng* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *là một hàm nếu với mọi x thuộc nguồn* A *của f thì quan hệ* $(x, y) \in \mathrm{F}$ *là phiếm hàm theo y* (Chương I, § 5, no. 3); *đối tượng duy nhất tương ứng với x qua f được gọi là giá trị của f tại phần tử x của* A, *và được ký hiệu bởi* $f(x)$ (*hoặc* $f_x$, *hoặc* $\mathrm{F}(x)$, *hoặc* $\mathrm{F}_x$).

Nếu $f$ là một hàm, F là đồ thị của nó, và $x$ là một phần tử của miền xác định của $f$, thì quan hệ $y = f(x)$ khi đó tương đương với $(x, y) \in \mathrm{F}$ (Chương I, § 5, no. 3, tiêu chuẩn C46).

#### Nhận xét {#ens-ii-s3-n4-rem-1 .statement tag=03HO}

Độc giả cần lưu ý sự nhầm lẫn có thể phát sinh từ việc sử dụng đồng thời các ký hiệu $f(x)$ và $f(\mathrm{X})$ (đồng nghĩa với $f\langle \mathrm{X} \rangle$) được đưa vào trong Định nghĩa 3 (cf. Bài tập 11).

Cho A và B là hai tập hợp; một *ánh xạ từ* A *vào* B là một hàm $f$ mà nguồn (bằng miền xác định của nó) bằng A và đích bằng B; hàm như vậy cũng được gọi là *được định nghĩa trên* A và *nhận giá trị trong* B.

Thay vì cụm từ "cho $f$ là một ánh xạ từ A vào B", các cụm từ sau thường được dùng: "cho $f : \mathrm{A} \to \mathrm{B}$ là một ánh xạ" hoặc thậm chí "cho $f : \mathrm{A} \to \mathrm{B}$". Để đơn giản hóa việc trình bày một lập luận liên quan đến nhiều ánh xạ, ta sử dụng *sơ đồ* như

$$\begin{array}{ccccccc} & f & & & g & \mathrm{C} & & i & \\ \mathrm{A} & \to & \mathrm{B} & \nearrow & & & \searrow & & \mathrm{E} \\ & & & \searrow & & \mathrm{D} & \nearrow & & \\ & & & h & & & j & & \end{array}$$

trong đó một nhóm các ký hiệu như $\mathrm{A} \overset{f}{\to} \mathrm{B}$ được diễn giải là có nghĩa rằng $f$ là một ánh xạ từ A vào B.

Một hàm $f$ được định nghĩa trên A nói là *biến đổi x thành* $f(x)$ (với mọi $x \in \mathrm{A}$); $f(x)$ được gọi là *biến đổi của x bởi f* hoặc (bỏ qua cách nói) *ảnh* của $x$ dưới $f$.

Dưới một số trường hợp, một đồ thị hàm được gọi là một *họ*; tập xác định khi đó được gọi là *tập chỉ số*, và tập giá trị được gọi là (bỏ qua cách nói) *tập các phần tử* của họ. Chính trong quan hệ này mà ký hiệu chỉ số $f_x$ được dùng để chỉ giá trị của $f$ tại phần tử $x$. Khi tập chỉ số là tích của hai tập hợp, ta thường nói về một *họ kép*.

Tương tự, một hàm mà đích là E đôi khi được gọi là một *họ các phần tử* của E. Nếu mọi phần tử của E là một tập con của một tập hợp F, ta nói về một *họ các tập con* của F.

Trong suốt bộ sách này, ta sẽ thường dùng từ “hàm” thay cho “đồ thị hàm”.

*Ví dụ về hàm*

#### Ví dụ 1 {#ens-ii-s3-n4-exa-1 .statement tag=03V1}

Tập rỗng là một đồ thị hàm. Mọi hàm có đồ thị rỗng đều có tập xác định và tập giá trị bằng tập rỗng. Trong các hàm như vậy, hàm có đích rỗng (tức là hàm $(\varnothing,\varnothing,\varnothing)$) được gọi là *hàm rỗng*.

#### Ví dụ 2 {#ens-ii-s3-n4-exa-2 .statement tag=03V2}

Cho A là một tập hợp. Sự tương ứng đồng nhất của A (số 3) là một hàm, gọi là *ánh xạ đồng nhất* của A.

Do đó, với mọi tập hợp A có liên kết một họ, được định nghĩa bởi ánh xạ đồng nhất của A, mà tập chỉ số là A và tập các phần tử là A. Bỏ qua cách nói, một tập hợp đôi khi được gọi là một “họ”, trong trường hợp đó nó chính là họ được liên kết như vậy với tập hợp đang xét.

Một hàm $f$ được gọi là *hằng* nếu với mọi $x$ và $x'$ trong tập xác định của $f$ ta có $f(x)=f(x')$.

¶ Cho $f$ là một ánh xạ từ một tập hợp E vào E. Một phần tử $x$ của E được gọi là *cố định dưới* $f$ nếu $f(x)=x$.

### 5. CÁC HẠN CHẾ VÀ MỞ RỘNG CỦA CÁC HÀM

Hai hàm $f$ và $g$ được gọi là *đồng nhất* (hay *trùng nhau*) trên một tập hợp E nếu E được chứa trong các miền xác định của $f$ và $g$ và nếu $f(x)=g(x)$ với mọi $x\in E$. Hai hàm có cùng một đồ thị thì đồng nhất trên miền xác định của chúng. Nói rằng $f=g$ nghĩa là nói rằng $f$ và $g$ có cùng miền xác định A và cùng đích B, và rằng chúng đồng nhất trên A.

¶ Cho $f=(F,A,B)$ và $g=(G,C,D)$ là hai hàm. Nói rằng $F\subset G$ là nói rằng bộ xác định A của $f$ được chứa trong bộ xác định C của $g$ và rằng $g$ đồng nhất với $f$ trên A. Nếu nữa $B\subset D$, thì $g$ được gọi là một *mở rộng* của $f$ (chính xác hơn, là một *mở rộng* của $f$ đến C), và $g$ được gọi là *mở rộng* $f$ (vào C). Khi $g$ được gọi là *họ* các phần tử của D, $f$ được gọi là *họ con* của $g$.

¶ Cho $f$ là một hàm và cho A là một tập con của miền xác định của $f$. Đó là ngay lập tức rằng quan hệ “$x\in A$ and $y=f(x)$” có một đồ thị G đối với $x$ và $y$, rằng đồ thị này là phiếm hàm, và rằng A là miền xác định của nó; hàm mà đồ thị là G, mà có cùng tập đích với $f$,

được gọi là *hạn chế* của $f$ tới $A$, và đôi khi được ký hiệu bởi $f|A$. Một hàm là một mở rộng của bất kỳ hạn chế nào của nó. Nếu hai hàm $f$, $g$ có cùng tập đích và trùng nhau trên một tập hợp $E$, thì các hạn chế của chúng tới $E$ là bằng.

### 6. ĐỊNH NGHĨA MỘT HÀM BẰNG CÁCH DÙNG MỘT SỐ HẠNG

C54. *Cho $T$, $A$ là hai số hạng và cho $x$, $y$ là các chữ cái phân biệt. Giả sử rằng $x$ không xuất hiện trong $A$ và rằng $y$ không xuất hiện trong $T$ cũng như trong $A$. Cho $R$ là quan hệ “$x \in A$ và $y = T$”. Quan hệ $R$ có một đồ thị $F$ đối với các chữ cái $x$ và $y$. Đồ thị này là phiếm hàm; phép chiếu thứ nhất của nó là $A$, và phép chiếu thứ hai là tập hợp các đối tượng dạng $T$ với $x \in A$ (§ 1, no. 6). Với mọi $x \in A$ ta có $F(x) = T$.*

Cho $B$ là tập hợp các đối tượng có dạng $T$ với $x \in A$. Khi đó

$$
R \Longrightarrow ((x,y) \in A \times B);
$$

vì tập hợp ký hiệu bởi $A \times B$ không chứa $x$ cũng không chứa $y$, $R$ có đồ thị $F$ theo các ký tự $x$ và $y$ (số 1). Rõ ràng là quan hệ

$$
(x,y) \in F \quad\text{và}\quad (x,y') \in F
$$

nghĩa là $y = y'$, và do đó $F$ là một đồ thị phiếm hàm. Các khẳng định còn lại là hiển nhiên.

¶ Nếu $C$ là một tập hợp chứa tập hợp $B$ các đối tượng có dạng $T$ với $x \in A$ (trong đó $y$ không xuất hiện trong $C$), thì hàm $(F,A,C)$ cũng được ký hiệu bởi ký hiệu $x \to T$ ($x \in A$, $T \in C$); hợp tương ứng trong toán học hình thức không chứa cả $x$ lẫn $y$ và không phụ thuộc vào lựa chọn chữ cái $y$ thỏa mãn các điều kiện trên. Khi ngữ cảnh đủ rõ ràng, chúng ta sẽ cho phép mình các ký hiệu $x \to T(x \in A)$, $(T)_{x \in A}$, hoặc $x \to T$, và đôi khi đơn giản là $T$ hoặc $(T)$. *Như vậy chúng ta có thể nói về “hàm $x^3$”, nếu ngữ cảnh chỉ rõ ràng rằng chúng ta có nghĩa là ánh xạ $x \to x^3$ của tập hợp các số phức vào chính nó. *

*Các ví dụ*

#### Ví dụ 1 {#ens-ii-s3-n6-exa-1 .statement tag=03S3}

Nếu $f$ là một ánh xạ của $A$ vào $B$, thì hàm $f$ bằng hàm $x \to f(x)$ ($x \in A$, $f(x) \in B$), được viết đơn giản là $x \to f(x)$ hoặc cũng là $(f_x)_{x \in A}$ (ký hiệu sau đặc biệt liên kết với cụm từ “họ các phần tử” thay vì “hàm”).

#### Ví dụ 2 {#ens-ii-s3-n6-exa-2 .statement tag=03S4}

Cho G là một tập hợp các cặp có thứ tự. Các hàm

$$z \to \mathrm{pr}_1 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_1 z \in \mathrm{pr}_1 \mathrm{G})$$

và

$$z \to \mathrm{pr}_2 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_2 z \in \mathrm{pr}_2 \mathrm{G})$$

được gọi lần lượt là *hàm tọa độ thứ nhất và thứ hai trên* G; chúng được ký hiệu bằng $\mathrm{pr}_1$ và $\mathrm{pr}_2$ khi không có nguy nhầm lẫn.

### 7. HỢP THÀNH CỦA HAI HÀM. HÀM NGHỊCH ĐẢO

#### Mệnh đề 6 {#ens-ii-s3-prop-6 .statement tag=03HP}

*Nếu f là một ánh xạ của* A *vào* B, *và g là một ánh xạ của* B *vào* C, *thì* $g \circ f$ *là một ánh xạ của* A *vào* C.

Cho F, G là đồ thị của $f$, $g$, tương ứng, và hãy chứng minh rằng $\mathrm{G} \circ \mathrm{F}$ là một đồ thị phiếm hàm. Cho $x$, $z$, $z'$ là các đối tượng sao cho $(x, z) \in \mathrm{G} \circ \mathrm{F}$, $(x, z') \in \mathrm{G} \circ \mathrm{F}$. Tồn tại các đối tượng $y$, $y'$ sao cho

$$(x, y) \in \mathrm{F}, \qquad (x, y') \in \mathrm{F}, \qquad (y, z) \in \mathrm{G}, \qquad (y', z') \in \mathrm{G}.$$

Vì F là một đồ thị phiếm hàm, ta có $y = y'$ và do đó $(y, z') \in \mathrm{G}$. Vì G là một đồ thị phiếm hàm, suy ra $z = z'$, điều này chứng minh mệnh đề này. Hơn nữa, miền xác định của $g \circ f$ hiển nhiên là A, và chứng minh hoàn tất.

¶ Hàm $g \circ f$ cũng có thể được viết dưới dạng $x \to g(f(x))$, hoặc là $gf$ khi không có nguy cơ nhầm lẫn.

#### Định nghĩa 10 {#ens-ii-s3-def-10 .statement tag=03HQ}

Cho f là một ánh xạ từ A vào B. Ánh xạ f được gọi là đơn ánh, hay là một đơn ánh, nếu bất kỳ hai phần tử phân biệt nào của A đều có ảnh phân biệt dưới f. Ánh xạ f được gọi là toàn ánh, hay là một toàn ánh, nếu $f(\mathrm{A}) = \mathrm{B}$. Nếu f vừa là đơn ánh lẫn toàn ánh, thì nó được gọi là song ánh, hay là một song ánh.

Thay vì nói rằng $f$ là toàn ánh, chúng tôi đôi khi nói rằng $f$ là một ánh xạ từ A lên B, hoặc là sự biểu diễn tham số của B thông qua A (trong trường hợp này A được gọi là tập hợp các tham số của sự biểu diễn, và các phần tử của A được gọi là các tham số). Nếu $f$ là song ánh, chúng tôi đôi khi nói rằng f đưa A và B vào sự tương ứng một-một. Một sự song ánh của A lên chính A được gọi là phép hoán vị của A.

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s3-n7-exa-1 .statement tag=03S5}

Nếu $\mathrm{A} \subset \mathrm{B}$, ánh xạ từ A vào B mà có đồ thị là đường chéo của A là đơn ánh và được gọi là *ánh xạ chính tắc* hay *đơn ánh chính tắc* (hay đơn giản là *đơn ánh*) của A vào B.

#### Ví dụ 2 {#ens-ii-s3-n7-exa-2 .statement tag=03S6}

Cho A là một tập hợp. Ánh xạ $x \to (x, x)$ từ A vào đường chéo $\Delta_\mathbf{A}$ của $\mathrm{A} \times \mathrm{A}$ là một ánh xạ song ánh, được gọi là *ánh xạ đường chéo* của A.

#### Ví dụ 3 {#ens-ii-s3-n7-exa-3 .statement tag=03S7}

Cho G là một tập hợp các cặp có thứ tự. Ánh xạ $\mathrm{pr}_1$ (tương ứng $\mathrm{pr}_2$) từ G vào $\mathrm{pr}_1\mathrm{G}$ (tương ứng $\mathrm{pr}_2\mathrm{G}$) là toàn ánh; $\mathrm{pr}_1$ là đơn ánh khi và chỉ khi G là một đồ thị phiếm hàm.

#### Ví dụ 4 {#ens-ii-s3-n7-exa-4 .statement tag=03S8}

Cho G là một tập hợp các cặp có thứ tự. Ánh xạ

$$z \to (\mathrm{pr}_2 z,\ \mathrm{pr}_1 z)$$

từ G vào $\overset{-1}{\mathrm{G}}$ là một song ánh (được gọi là *chính tắc* song ánh).

#### Ví dụ 5 {#ens-ii-s3-n7-exa-5 .statement tag=03S9}

Cho A là một tập hợp và $b$ là một đối tượng. Ánh xạ $x \to (x,\ b)$ từ A vào $\mathrm{A} \times \{b\}$ là một song ánh.

#### Mệnh đề 7 {#ens-ii-s3-prop-7 .statement tag=03PQ}

*Cho $f$ là một ánh xạ từ* A *vào* B. *Khi đó* $\overset{-1}{f}$ *là một hàm khi và chỉ khi $f$ là song ánh.*

Nếu $\overset{-1}{f}$ là một hàm, thì nguồn B của nó bằng miền xác định của nó, nghĩa là $f(\mathrm{A})$; do đó $f$ là toàn ánh. Để chứng minh $f$ là đơn ánh, lấy $x$ và $y$ là hai phần tử của A sao cho $f(x) = f(y)$. Nếu F biểu diễn đồ thị của $f$, ta có

$$(f(x),\ x) \in \overset{-1}{\mathrm{F}} \qquad \text{và} \qquad (f(y),\ y) \in \overset{-1}{\mathrm{F}},$$

do đó

$$(f(x),\ y) \in \overset{-1}{\mathrm{F}},$$

suy ra $x = y$, điều này chứng minh mệnh đề.

¶ Ngược lại, nếu $f$ là song ánh, thì ngay lập tức $\overset{-1}{\mathrm{F}}$ là phiếm hàm và miền xác định của $\overset{-1}{f}$ bằng B.

Khi $f$ là song ánh, $\overset{-1}{f}$ được gọi là *ánh xạ nghịch đảo* của $f$; $\overset{-1}{f}$ là song ánh, $\overset{-1}{f} \circ f$ là ánh xạ đồng nhất của A, và $f \circ \overset{-1}{f}$ là ánh xạ đồng nhất của B.

¶ Nếu một phép hoán vị giống như nghịch đảo của nó, thì nó được gọi là *đối hợp*.

#### Chú ý {#ens-ii-s3-n7-rem-1 .statement tag=03HR}

Cho $f$ là một ánh xạ của A vào B. Với mỗi tập con X của A ta có (no. 3) $\mathrm{X} \subset \overset{-1}{f}\langle f\langle \mathrm{X}\rangle\rangle$. Hơn nữa, với mỗi tập con Y của B ta có $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle \subset \mathrm{Y}$, vì quan hệ $y \in f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle$ tương đương với

$$(\exists x)((\exists z)(z \in \mathrm{Y} \text{ và } z = f(x)) \text{ và } y = f(x))$$

và do đó kéo theo quan hệ $(\exists z)(z \in \mathrm{Y} \text{ và } y = z)$ và do đó cũng kéo theo quan hệ $y \in \mathrm{Y}$.

Nếu $f$ là *toàn ánh*, ta có $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle = \mathrm{Y}$ với mọi tập con Y của B, vì quan hệ $y \in \mathrm{Y} \subset \mathrm{B}$ suy ra theo giả thiết quan hệ $(\exists x)(y = f(x))$ và do đó cũng suy ra $(\exists x)(y \in \mathrm{Y} \text{ và } y = f(x))$; nhưng "$y \in \mathrm{Y}$ và $y = f(x)$" suy ra $(\exists z)(z \in \mathrm{Y} \text{ và } z = f(x))$, và mệnh đề của ta được chứng minh.

Nếu $f$ là *đơn ánh*, ta có $\overset{-1}{f}\langle f\langle X\rangle\rangle = X$ với mọi tập con X của A. Vì quan hệ $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ tương đương với $f(x) \in f\langle X\rangle$, do đó tương đương với

$$(\exists z)(z \in X \text{ và } f(z) = f(x));$$

nhưng giả thiết có nghĩa là $f(z) = f(x)$ ngụ ý $z = x$, do đó $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ ngụ ý $x \in X$.

### 8. PHÉP CO RÚT VÀ TIẾT DIỆN

#### Mệnh đề 8 {#ens-ii-s3-prop-8 .statement tag=03HS}

*Cho $f$ là một ánh xạ của* A *vào* B. *Nếu tồn tại một ánh xạ $r$* (tương ứng $s$) *của* B *vào* A *sao cho $r \circ f$* (tương ứng $f \circ s$) *là ánh xạ đồng nhất của* A (tương ứng B), *thì $f$ là đơn ánh* (tương ứng *toàn ánh*). *Ngược lại, nếu $f$ là toàn ánh, tồn tại một ánh xạ $s$ của* B *vào* A *sao cho $f \circ s$ là ánh xạ đồng nhất của* B. *Nếu $f$ là đơn ánh và nếu* A $\neq \emptyset$, *tồn tại một ánh xạ $r$ của* B *vào* A *sao cho $r \circ f$ là ánh xạ đồng nhất của* A.

Nếu tồn tại một ánh xạ $r$ từ B vào A sao cho $r \circ f$ là ánh xạ đồng nhất của A, thì đẳng thức $f(x) = f(y)$, với $x \in A$ và $y \in A$, kéo theo $x = r(f(x)) = r(f(y)) = y$, và do đó $f$ là đơn ánh. Nếu tồn tại một ánh xạ $s$ từ B vào A sao cho $f \circ s$ là ánh xạ đồng nhất của B, ta có $B = f(s(B)) \subset f(A) \subset B$, do đó $f$ là toàn ánh. Nếu $f$ là toàn ánh, đặt T là số hạng $\tau_y(y \in A \text{ và } f(y) = x)$. Ta có $f(T) = x$ với $x \in B$; nếu $s$ là ánh xạ $x \to T$ $(x \in B, T \in A)$, thì $f \circ s$ là ánh xạ đồng nhất của B. Cuối cùng, giả sử $f$ là đơn ánh và A $\neq \emptyset$, và cho $a$ là một phần tử của A. Quan hệ

$$\text{“}(y \in A \text{ và } x = f(y)) \text{ hoặc } (y = a \text{ và } x \in B - f(A))\text{''}$$

Ngụ ý $(x, y) \in B \times A$ và do đó có đồ thị R theo các chữ $x$, $y$. Đồ thị này là một ánh xạ do giả thiết trên $f$, và có B là miền xác định; và ta có $R(x) = a$ nếu $x \in B - f(A)$, và $f(R(x)) = x$ nếu $x \in f(A)$. Do đó hàm $r = (R, B, A)$ thỏa mãn $r \circ f$ là ánh xạ đồng nhất của A.

#### Hệ quả {#ens-ii-s3-n8-cor-1 .statement tag=03HT}

*Cho* A, B *là các tập hợp, cho $f$ là một ánh xạ từ* A *vào* B, *và cho $g$ là một ánh xạ từ* B *vào* A. *Nếu $g \circ f$ là ánh xạ đồng nhất của* A *và nếu $f \circ g$ là ánh xạ đồng nhất của* B, *thì $f$ và $g$ là song ánh, và $g = \overset{-1}{f}$.*

#### Định nghĩa 11 {#ens-ii-s3-def-11 .statement tag=03HU}

*Cho $f$ là một ánh xạ đơn ánh* (tương ứng, *toàn ánh*) *từ* A *vào* B. *Mọi ánh xạ $r$* (tương ứng, $s$) *từ* B *vào* A *sao cho $r \circ f$* (tương ứng, $f \circ s$) *là ánh xạ đồng nhất của* A (tương ứng, B) *được gọi là một phép co rút* (tương ứng, *tiết diện*) *của $f$.*

Thay cho phép co rút (tương ứng, tiết diện), đôi khi người ta dùng cụm từ *nghịch đảo trái* (tương ứng, *nghịch đảo phải*).

¶ Nếu $f$ là đơn ánh (tương ứng, toàn ánh) và nếu $r$ (tương ứng, $s$) là một sự co lại (tương ứng, tiết diện) của $f$, thì $f$ là một tiết diện (tương ứng, sự co lại) của $r$ (tương ứng, $s$). Do đó một sự co lại là toàn ánh và một tiết diện là đơn ánh.

¶ Nếu $f$ là toàn ánh và $s$, $s'$ là hai tiết diện của $f$ sao cho $s(\mathrm{B}) = s'(\mathrm{B})$, thì $s = s'$; vì nếu $x \in \mathrm{B}$, tồn tại $y \in \mathrm{B}$ sao cho $s(x) = s'(y)$, và ta có $x = f(s(x)) = f(s'(y)) = y$, do đó $s(x) = s'(x)$ và do đó $s = s'$. Vậy một tiết diện $s$ được xác định duy nhất bởi tập hợp $s(\mathrm{B})$. Theo lối nói lạm dụng, tập hợp $s(\mathrm{B})$ đôi khi được gọi là một *tiết diện của $f$*.

#### Định lý 1 {#ens-ii-s3-thm-1 .statement tag=03PR}

*Cho $f$ là một ánh xạ từ* A *vào* B, *cho $f'$ là một ánh xạ từ* B *vào* C, *và cho $f'' = f' \circ f$. Khi đó :*

(a) *Nếu $f$ và $f'$ là các đơn ánh, thì $f''$ là một đơn ánh. Nếu $r$, $r'$ là các phép rút của $f$, $f'$, tương ứng, thì $r \circ r'$ là một phép rút của $f''$.*

(b) *Nếu $f$ và $f'$ là các toàn ánh, thì $f''$ là một toàn ánh. Nếu $s$, $s'$ là các tiết diện của $f$, $f'$, tương ứng, thì $s \circ s'$ là một tiết diện của $f''$.*

(c) *Nếu $f''$ là một đơn ánh, thì $f$ là một đơn ánh. Nếu $r''$ là một ánh xạ rút lại của $f''$, thì $r'' \circ f'$ là một ánh xạ rút lại của $f$.*

(d) *Nếu $f''$ là một toàn ánh, thì $f'$ là một toàn ánh. Nếu $s''$ là một tiết diện của $f''$, thì $f \circ s''$ là một tiết diện của $f'$.*

(e) *Nếu $f''$ là một toàn ánh và $f'$ là một đơn ánh, thì $f$ là một toàn ánh. Nếu $s''$ là một tiết diện của $f''$, thì $s'' \circ f'$ là một tiết diện của $f$.*

(f) *Nếu $f''$ là một đơn ánh và $f$ là một toàn ánh, thì $f'$ là một đơn ánh. Nếu $r''$ là một ánh xạ co của $f''$, thì $f \circ r''$ là một ánh xạ co của $f'$.*

Với mọi tập hợp E, ký hiệu $\mathrm{I_E}$ là ánh xạ đồng nhất của E.

(a) Ta có $r \circ f = \mathrm{I_A}$ và $r' \circ f' = \mathrm{I_B}$, do đó

$$(r \circ r') \circ (f' \circ f) = r \circ \mathrm{I_B} \circ f = r \circ f = \mathrm{I_A}.$$

Nếu $f$ và $f'$ là đơn ánh, thì $f''$ là một đơn ánh, theo Mệnh đề 8 nếu $\mathrm{A} \neq \emptyset$, và hiển nhiên nếu $\mathrm{A} = \emptyset$.

(b) Ta có $f \circ s = \mathrm{I_B}$ và $f' \circ s' = \mathrm{I_C}$, do đó

$$(f' \circ f)(s \circ s') = f' \circ \mathrm{I_B} \circ s' = f' \circ s' = \mathrm{I_C}.$$

Nếu $f$ và $f'$ là toàn ánh, thì $f''$ là một toàn ánh theo Mệnh đề 8.

(c) Ta có $r'' \circ f'' = \mathrm{I_A}$, do đó $(r'' \circ f') \circ f = r'' \circ f'' = \mathrm{I_A}$. Nếu $f''$ là một đơn ánh, thì $f$ là một đơn ánh, theo Mệnh đề 8 nếu $\mathrm{A} \neq \emptyset$, và tầm thường nếu $\mathrm{A} = \emptyset$.

(d) Ta có $f'' \circ s'' = \mathrm{I_C}$, do đó $f' \circ (f \circ s'') = f'' \circ s'' = \mathrm{I_C}$. Nếu $f''$ là một toàn ánh, thì $f'$ là một toàn ánh theo Mệnh đề 8.

(e) Ta có $f'' \circ s'' = \mathrm{I_C}$, và $f'$ là một song ánh theo (d). Do đó

$$f \circ (s'' \circ f') \;=\; (\overset{-1}{f}{}' \circ f') \circ f \circ (s'' \circ f') \;=\; \overset{-1}{f}{}' \circ (f'' \circ s'') \circ f'$$
$$= \overset{-1}{f}{}' \circ \mathrm{I_C} \circ f' = \overset{-1}{f}{}' \circ f' = \mathrm{I_B}.$$

Nếu $f''$ là một ánh xạ lên và $f'$ là một đơn ánh, thì $f$ là một ánh xạ lên theo Mệnh đề 8.

(f) Ta có $r'' \circ f'' = \mathrm{I_A}$, và $f$ là một song ánh theo (c). Do đó

$$(f \circ r'') \circ f' = (f \circ r'') \circ f' \circ (f \circ \overset{-1}{f}) = f \circ (r'' \circ f'') \circ \overset{-1}{f} = f \circ \mathrm{I_A} \circ \overset{-1}{f}$$
$$= f \circ \overset{-1}{f} = \mathrm{I_B}.$$

Nếu $f''$ là một đơn ánh và $f$ là một ánh xạ lên, thì $f'$ là một đơn ánh, theo Mệnh đề 8 nếu $\mathrm{A} \neq \emptyset$, và hiển nhiên nếu $\mathrm{A} = \emptyset$ (vì khi đó ta có $\mathrm{B} = f\langle \mathrm{A}\rangle = \emptyset$).

#### Mệnh đề 9 {#ens-ii-s3-prop-9 .statement tag=03PS}

(a) *Cho* E, F, G *là các tập hợp, cho* $g$ *là một ánh xạ từ* E *lên* F *và* $f$ *là một ánh xạ từ* E *vào* G. *Khi đó tồn tại một ánh xạ* $h$ *từ* F *vào* G *sao cho* $f = h \circ g$ *nếu và chỉ nếu quan hệ* $g(x) = g(y)$ *(với* $x \in \mathrm{E}$, $y \in \mathrm{E}$*) kéo theo quan hệ* $f(x) = f(y)$. *Ánh xạ* $h$ *khi đó được xác định duy nhất bởi* $f$; *nếu* $s$ *là một tiết diện của* $g$, *ta có* $h = f \circ s$.

$$\begin{array}{ccc}
\mathrm{E} & \overset{f}{\searrow} & \\
{\scriptstyle g}\big\downarrow\big\uparrow{\scriptstyle s} & & \\
\mathrm{F} & \underset{h}{\longrightarrow} & \mathrm{G}
\end{array}
\qquad\qquad
\begin{array}{ccc}
 & \overset{f}{\nearrow} & \mathrm{E} \\
 & & {\scriptstyle r}\big\downarrow\big\uparrow{\scriptstyle g} \\
\mathrm{G} & \underset{h}{\longrightarrow} & \mathrm{F}
\end{array}$$
$$\text{(a)} \qquad\qquad\qquad \text{(b)}$$

(b) *Cho* E, F, G *là các tập hợp, cho* $g$ *là một đơn ánh từ* F *vào* E, *và cho* $f$ *là một ánh xạ từ* G *vào* E. *Khi đó tồn tại một ánh xạ* $h$ *từ* G *vào* F *sao cho* $f = g \circ h$ *khi và chỉ khi* $f(\mathrm{G}) \subset f(\mathrm{F})$. *Ánh xạ* $h$ *được xác định duy nhất bởi* $f$; *nếu* $r$ *là một phép co rút của* $g$, *thì ta có* $h = r \circ f$.

(a) Nếu $f = h \circ g$, quan hệ $g(x) = g(y)$ (trong đó $x \in \mathrm{E}$, $y \in \mathrm{E}$) rõ ràng dẫn đến $f(x) = f(y)$. Và với mỗi tiết diện $s$ của $g$ ta có

$$h = h \circ (g \circ s) = f \circ s,$$

điều này cho thấy $h$ được xác định duy nhất bởi $f$. Ngược lại, giả sử rằng quan hệ $g(x) = g(y)$ dẫn đến $f(x) = f(y)$; hãy để $s$ là một tiết diện

của $g$, và đặt $h = f \circ s$; khi đó với mọi $x \in E$ ta có $g(s(g(x))) = g(x)$, do đó $f(s(g(x))) = f(x)$, nghĩa là, $h(g(x)) = f(x)$ và do đó $f = h \circ g$.

(b) Nếu $f = g \circ h$, thì rõ ràng $f(G) \subset f(F)$, và với mọi retraction $r$ của $g$ ta có $h = (r \circ g) \circ h = r \circ f$, điều này cho thấy $h$ được xác định duy nhất bởi $f$. Ngược lại, giả sử $f(G) \subset f(F)$; cho $r$ là một retraction của $g$, và đặt $h = r \circ f$; với mỗi $x \in G$, tồn tại $y \in F$ sao cho $f(x) = g(y)$, khi đó

$$g(h(x)) = g(r(f(x))) = g(r(g(y))) = g(y) = f(x)$$

và do đó $f = g \circ h$.

### 9. CÁC HÀM CỦA HAI ĐỐI SỐ

Một *hàm của hai đối số* là một hàm có miền là một tập hợp các cặp có thứ tự (hoặc, tương đương, một tập con của một tích). Cho $f$ là một hàm như vậy; nếu $(x, y)$ là một phần tử của miền của $f$, thì giá trị $f((x, y))$ của $f$ tại phần tử $(x, y)$ nói chung được ký hiệu bởi $f(x, y)$.

¶ Cho $f$ là một hàm của hai đối số, D là miền của nó, và C là đích của nó. Với mỗi $y$, gọi $A_y$ là tập hợp của mọi $x$ sao cho $(x, y) \in D$ (nghĩa là, tiết diện của $\overset{-1}{D}$ tại $y$ (số 1)). Ánh xạ

$$x \to f(x, y) \quad (x \in A_y, f(x, y) \in C)$$

được gọi là *ánh xạ một phần được xác định bởi $f$, với giá trị $y$ của đối số thứ hai*, và ký hiệu bằng $f(\bullet, y)$, hay $f(\ , y)$ (hoặc đôi khi $f_y$); ta có $f(\bullet, y)(x) = f(x, y)$ với mọi $(x, y) \in D$. Tương tự với mỗi $x$, gọi $B_x$ là tập hợp tất cả các $y$ sao cho $(x, y) \in D$. Ánh xạ

$$y \to f(x, y) \quad (y \in B_x, f(x, y) \in C)$$

được gọi là *ánh xạ một phần được định nghĩa bởi $f$, theo giá trị $x$ của đối số thứ nhất*, và được ký hiệu bằng $f(x, \bullet)$, hoặc $f(x, \ )$ (hoặc đôi khi $f_x$); ta có $f(x, \bullet)(y) = f(x, y)$ với mọi $(x, y) \in D$.

¶ Nếu với mọi $y$ (resp. $x$) ánh xạ riêng phần $f(\bullet, y)$ (resp. $f(x, \bullet)$) là một ánh xạ hằng số, ta nói rằng $f$ *không phụ thuộc vào* đối số thứ nhất (resp. thứ hai) của nó; điều này có nghĩa là do đó $f(x, y) = f(x', y)$ bất cứ khi nào $(x, y)$ và $(x', y)$ thuộc D (resp. $f(x, y) = f(x, y')$ bất cứ khi nào $(x, y)$ và $(x, y')$ thuộc D). Với mỗi $y$ thuộc phép chiếu thứ hai của D, đặt $g(y)$ là giá trị chung của các $f(x, y)$ với $x \in A_y$; khi đó ánh xạ $y \to g(y)$ là một ánh xạ từ $\mathrm{pr}_2 D$ vào C sao cho

$$g(y) = f(x, y) \qquad \text{với mọi } (x, y) \in D.$$

¶ Ngược lại, cho $g$ là một ánh xạ từ một tập hợp B vào một tập hợp C, và cho A là một tập hợp bất kỳ. Khi đó ánh xạ $(x, y) \to g(y)$ từ $A \times B$ vào C không phụ thuộc vào đối số thứ nhất của nó.

Cho $u$ là một ánh xạ từ A vào C và $v$ là một ánh xạ từ B vào D. Ánh xạ $z \to (u(\mathrm{pr}_1 z), v(\mathrm{pr}_2 z))$ từ $A \times B$ vào $C \times D$ được gọi là (*chính tắc*) *mở rộng của $u$ và $v$ tới tích các tập hợp*, hay đơn giản là *tích của $u$ và $v$* (nếu không có nguy cơ nhầm lẫn); ảnh của nó là $u\langle A\rangle \times v\langle B\rangle$. Nó được ký hiệu bằng $u \times v$. Nếu $u$ và $v$ là đơn ánh (resp. toàn ánh) thì $u \times v$ cũng đơn ánh (resp. toàn ánh). Nếu $u$ và $v$ là song ánh, thì $u \times v$ cũng song ánh, và ánh xạ nghịch đảo của nó là $\overset{-1}{u} \times \overset{-1}{v}$. Nếu $u'$ là một ánh xạ từ C vào một tập hợp E và nếu $v'$ là một ánh xạ từ D vào một tập hợp F, ta có

$$(u' \times v') \circ (u \times v) = (u' \circ u) \times (v' \circ v).$$

Nếu U, V là các đồ thị của $u$, $v$ tương ứng, thì đồ thị W của $u \times v$ là tập hợp các cặp có thứ tự $((x,y), (z, t))$ của $(A \times B) \times (C \times D)$ sao cho $(x, z) \in U$ và $(y, t) \in V$; ánh xạ $((x, y), (z, t)) \to ((x, z), (y, t))$ đưa W vào sự tương ứng một-một với tích $U \times V$ (một tập con của $(A \times C) \times (B \times D)$) (cf. §5, no. 5).

### Bài tập {#ens-ii-s3-exercises}

Xem [bài tập cho § 3](exercises/s3/).
