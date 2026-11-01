---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 3
section_title: Correspondences
lang: zh
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
content_sha256: bb2f363e2faf637f2e687b8fa00b3bd913a31d24478a16ed01e2aa3823568d11
translated_from: content/en/ens/II/03_s3_correspondences.md
translation_method: google
source_content_sha256: 09657f186f72956f32a3834e46ca25f5e52a2f152080a83c21123877583d9007
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 6156c1be35e974695a1d8865d5c30fb32b8225b926c2d48b4f2dbf92b2d42742
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 3. CORRESPONDENCES

### 1. 图表和对应

#### 定义 1 {#ens-ii-s3-def-1 .statement tag=03PG}

如果* G * 的每个元素都是有序对，即如果关系*，则 G * 被称为图

$$(\forall z)(z \in G \Rightarrow (z \text{ is an ordered pair}))$$

*是真的。*

如果G是图，关系$(x, y) \in G$用说表示“G下$y$对应到$x$”。

令 $\boldsymbol{R}\{x, y\}$ 为关系，其中 $x$ 和 $y$ 是不同的字母。设$\boldsymbol{G}$是一个字母，与$x$和$y$不同，$\boldsymbol{R}$中没有出现。如果关系

$$(\exists \boldsymbol{G})(\boldsymbol{G} \text{ is a graph and } (\forall x)(\forall y)(\boldsymbol{R} \Leftrightarrow ((x, y) \in \boldsymbol{G})))$$

是真的，据说关系$\boldsymbol{R}$*有一个图形*（相对于字母$x$和$y$）。那么图$\boldsymbol{G}$凭借范围公理是唯一的，并且被称为$\boldsymbol{R}$相对于$x$和$y$的*图*。

¶ 令 $Z$ 为一个字母，与 $x$ 和 $y$ 不同，它不会出现在 $R$ 中。如果关系

$$(\exists Z)(\forall x)(\forall y)(R \Rightarrow ((x, y) \in Z))$$

为真，则 $R$ 有图；我们可以将此图视为有序对$z$的集合，使得$z \in Z$和$R \{ \mathrm{pr}_1 z,\ \mathrm{pr}_2 z \}$（$z$是与$x$、$y$、$Z$不同的字母，$R$中没有出现）。如果我们知道项$T$，则满足条件，而包含既不知道$x$，也不知道$y$，因此$R \Rightarrow ((x,\ y) \in T)$为真。

#### 命题 1 {#ens-ii-s3-prop-1 .statement tag=03HI}

*让*G *是一个图。恰好存在一个集合* A *和恰好一个集合* B *具有以下属性*：

(1) *关系* $(\exists y)((x,\ y) \in \mathrm{G})$ *等价于* $x \in \mathrm{A}$；

(2) *关系* $(\exists x)((x,\ y) \in \mathrm{G})$ *等价于* $y \in \mathrm{B}$。

因为只要取 A（分别为 B）为形式 $\mathrm{pr}_1 z$（分别为 $\mathrm{pr}_2 z$）的所有对象中的集合就足够了，其中 $z \in \mathrm{G}$ (§ 1, no. 6)。恰恰，

$$\mathrm{A} = \mathscr{E}_x((\exists y)((x, y) \in \mathrm{G}))) \qquad \text{and} \qquad \mathrm{B} = \mathscr{E}_y((\exists x)((x,\ y) \in \mathrm{G}));$$

这些集合分别称为图G的*第一和第二投影*，或者G的*域*和*范围*；它们用 $\mathrm{pr}_1 \langle \mathrm{G} \rangle$ 和 $\mathrm{pr}_2 \langle \mathrm{G} \rangle$ 表示（如果不存在混淆的风险，则用 $\mathrm{pr}_1 \mathrm{G}$ 和 $\mathrm{pr}_2 \mathrm{G}$ 表示）。立即验证$\mathrm{G} \subset (\mathrm{pr}_1 \mathrm{G}) \times (\mathrm{pr}_2 \mathrm{G})$；因此，有序对的每个集合都是乘积的子集，反之亦然。如果两个集合、$\mathrm{pr}_1 \mathrm{G}$、$\mathrm{pr}_2 \mathrm{G}$其中之一为空，则有$\mathrm{G} = \emptyset$（§ 2、命题 2）。

#### 注 {#ens-ii-s3-n1-rem-3 .statement tag=03S1}

关系 $x = y$ 没有图，对于图的第一个投影，如果存在，将是所有对象中的集合（cf. § 1, no. 7，注）。

#### 定义 2 {#ens-ii-s3-def-2 .statement tag=03HJ}

*对应在集合* A *和集合* B *之间是一个三元组*

$$\Gamma = (\mathrm{G},\ \mathrm{A},\ \mathrm{B}),$$

*其中* G *是一个图，使得* $\mathrm{pr}_1 \mathrm{G} \subset \mathrm{A}$ *和* $\mathrm{pr}_2 \mathrm{G} \subset \mathrm{B}$。 G*据说是*$\Gamma$的图，A*是源，*B*是*$\Gamma$的目标。

如果$(x,\ y) \in \mathrm{G}$，我们说“$y$对应到$x$在对应$\Gamma$”。对于每个 $x \in \mathrm{pr}_1 \mathrm{G}$ 对应 $\Gamma$ 被称为*定义于* $x$，而 $\mathrm{pr}_1 \mathrm{G}$ 被称为*$\Gamma$的*域；每个 $y \in \mathrm{pr}_2 \mathrm{G}$ 被称为由* $\Gamma$ 取的 *值，$\mathrm{pr}_2 \mathrm{G}$ 被称为* $\Gamma$ 的*范围。

如果$R \{ x, y \}$是关系，它有一个图$G$（相对于字母$x$，$y$），并且如果$A$，$B$是两个集合，使得$\mathrm{pr}_1 G \subset A$和$\mathrm{pr}_2 G \subset B$，我们说$R$ 是$A$ 的元素和$B$* 的元素之间的*关系（相对于字母$x$、$y$）。 对应$\Gamma = (G, A, B)$据说是$A$和$B$之间的对应*由*关系$R$定义（相对于$x$和$y$）。

设 G 为图，且 X 为集合。 关系

$$x \in X \text{ and } (x, y) \in G$$

意味着$(x, y) \in G$，因此有一个图$G'$。 $G'$的第二个投影由G下的所有对象组成，其中对应到X的对象。

#### 定义 3 {#ens-ii-s3-def-3 .statement tag=03PI}

*设*G*是一个图并且*X*集合。所有对象中的集合，其中* G *下的对应到* X *的元素被称为* G *下* X *的像，并用* $G\langle X \rangle$ *或* $G(X)$表示。

¶ *设* $\Gamma = (G, A, B)$ *为对应并让* X *为* A 的子集 *集合* $G\langle X \rangle$ *也表示为* $\Gamma\langle X \rangle$ *或* $\Gamma(X)$ *并称为像共* X *低于* $\Gamma$。

*注*

#### 注 1 {#ens-ii-s3-n1-rem-1 .statement tag=03PH}

准确地说，$G\langle X \rangle$表示集合$\mathscr{E}_y((\exists x)(x \in X \text{ and } (x,y) \in G))$。从现在开始，我们通常不会将我们的定义翻译成正式语言。

#### 注 2 {#ens-ii-s3-n1-rem-2 .statement tag=03S2}

记号 $G(X)$ 和 $\Gamma(X)$ 有时会导致与稍后介绍的记号混淆（cf. no. 4、注紧随定义 9）。

设 G 是一个图。由于关系$(x, y) \in G$意味着$y \in \mathrm{pr}_2 G$，因此对于每个集合X，我们有$G\langle X \rangle \subset \mathrm{pr}_2 G$。由于$(x, y) \in G$意味着$x \in \mathrm{pr}_1 G$，所以我们有$G\langle \mathrm{pr}_1 G \rangle = \mathrm{pr}_2 G$。我们有$G\langle \emptyset \rangle = \emptyset$，因为$x \notin \emptyset$是定理。如果$X \subset \mathrm{pr}_1 G$和$X \neq \emptyset$，我们有$G\langle X \rangle \neq \emptyset$。

#### 命题 2 {#ens-ii-s3-prop-2 .statement tag=03PJ}

*设* G *为一个图，并让* X，Y *为两个集合；那么关系* $X \subset Y$ *意味着* $G\langle X \rangle \subset G\langle Y \rangle$。

这是定义和 C50 (§ 1, no. 4) 的直接的推论。

#### 推论 {#ens-ii-s3-n1-cor-1 .statement tag=03PK}

*如果*$A \supset \mathrm{pr}_1 G$，*我们有*$G\langle A \rangle = \mathrm{pr}_2 G$。

#### 定义 4 {#ens-ii-s3-def-4 .statement tag=03PL}

*设*G*是一个图，并且*$x$*对象。 集合* $G\langle \{x\} \rangle$（通过滥用语言，$G(x)$表示为有时）*被称为* G *在* $x$的截面。

紧随 C43 (章 I, § 5, no. 1) 可知关系 $y \in G\langle \{x\} \rangle$ 相当于 $(x, y) \in G$。如果 G 和 $G'$ 是两个图，则关系 $G \subset G'$ 等价于

$$(\forall x)(G\langle \{x\} \rangle \subset G'\langle \{x\} \rangle).$$

如果 A 和 B 之间的 $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ 为对应，则对于 G 在 $x$ 处的每个 $x \in \mathrm{A}$ 截面也称为* $\Gamma$ *在* $x$ 的 *截面，并用 $\Gamma\langle\{x\}\rangle$ 表示（或$\Gamma(x)$）。

### 2. 逆对应

设 G 是一个图，$\mathrm{A} = \mathrm{pr}_1\mathrm{G}$、$\mathrm{B} = \mathrm{pr}_2\mathrm{G}$ 是投影。 关系 $(y, x) \in \mathrm{G}$ 意味着 $(x, y) \in \mathrm{B} \times \mathrm{A}$；因此，这个关系有一个由所有有序对$(x, y)$组成的图，使得$(y, x) \in \mathrm{G}$。

#### 定义 5 {#ens-ii-s3-def-5 .statement tag=03PM}

*设G是一个图。 元素为有序对$(x, y)$使得$(y, x) \in \mathrm{G}$的图称为G的逆图，记为*$\overset{-1}{\mathrm{G}}$。

对于每个集合X，$\overset{-1}{\mathrm{G}}\langle\mathrm{X}\rangle$被称为*X*下*G的*逆像。

¶ 很明显，$\overset{-1}{\mathrm{G}}$ 的倒数是 G，并且

$$\mathrm{pr}_1\overset{-1}{\mathrm{G}} = \mathrm{pr}_2\mathrm{G}, \qquad \mathrm{pr}_2\overset{-1}{\mathrm{G}} = \mathrm{pr}_1\mathrm{G}.$$

特别是，如果X，Y是两个集合，我们有

$$\overset{-1}{\overbrace{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

如果 $\overset{-1}{\mathrm{G}} = \mathrm{G}$，则称图 G 是“对称”的。

¶ 设 $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ 为 A 和 B 之间的对应。由于 $\mathrm{pr}_1\overset{-1}{\mathrm{G}} \subset \mathrm{B}$ 和 $\mathrm{pr}_2\overset{-1}{\mathrm{G}} \subset \mathrm{A}$，三元组 $(\overset{-1}{\mathrm{G}}, \mathrm{B}, \mathrm{A})$ 是 B 和 A 之间的 *对应，称为对应 $\Gamma$ 的*逆*，并用 $\overset{-1}{\Gamma}$ 表示。对于B的每个子集Y，$\overset{-1}{\Gamma}$下Y的像$\overset{-1}{\Gamma}\langle\mathrm{Y}\rangle$也称为$\Gamma$下Y的*逆像*。显然 $\overset{-1}{\Gamma}$ 的倒数是 $\Gamma$。

### 3. 两个对应的合成

令G、G′为两个图。令 A 表示集合 $\mathrm{pr}_1\mathrm{G}$，令 C 表示集合 $\mathrm{pr}_2\mathrm{G}'$。 关系$(\exists y)((x, y) \in \mathrm{G}$和$(y, z) \in \mathrm{G}')$意味着$(x, z) \in \mathrm{A} \times \mathrm{C}$，因此有一个关于$x$和$z$的图。

#### 定义 6 {#ens-ii-s3-def-6 .statement tag=03PN}

*设G、G′为两个图。 关系、$(\exists y)((x, y) \in \mathrm{G}$和$(y, z) \in \mathrm{G}')$的图（相对于$x$和$z$）称为G'和G的合成，并用*$\mathrm{G}' \circ \mathrm{G}$表示（或用$\mathrm{G}'\mathrm{G}$表示有时）。

#### 命题 3 {#ens-ii-s3-prop-3 .statement tag=03HK}

*设*G，G′*为两个图。 * G′ ∘ G * 的倒数是* $\overset{-1}{G} \circ \overset{-1}{G'}$。

对于关系“$(x, y) \in G$和$(y, z) \in G'$”相当于

$$(z, y) \in \overset{-1}{G'} \text{ and } (y, x) \in \overset{-1}{G}.$$

#### 命题 4 {#ens-ii-s3-prop-4 .statement tag=03HL}

*设* $G_1$、$G_2$、$G_3$ *为图形。然后*

$$(G_3 \circ G_2) \circ G_1 = G_3 \circ (G_2 \circ G_1).$$

关系 $(x, t) \in (G_3 \circ G_2) \circ G_1$ 相当于关系

$$(\exists y)((x, y) \in G_1 \text{ and } \exists z((y, z) \in G_2 \text{ and } (z, t) \in G_3))$$

因此（通过 C33 (章 I, § 4, no. 3)）到关系

(1) $$(\exists y)(\exists z)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

同样，关系$(x, t) \in G_3 \circ (G_2 \circ G_1)$等价于

(2) $$(\exists z)(\exists y)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

但关系 (1) 和 (2) 是等价的；因此结果。

¶ 图 $G_3 \circ (G_2 \circ G_1)$ 用 $G_3 \circ G_2 \circ G_1$ 表示。类似地，如果 $G_1$、$G_2$、$G_3$、$G_4$ 是图，我们将

$$G_4 \circ (G_3 \circ G_2 \circ G_1) = G_4 \circ G_3 \circ G_2 \circ G_1;$$

等等。

#### 命题 5 {#ens-ii-s3-prop-5 .statement tag=03HM}

*设* G, G′ *为图，设* A *为集合。然后*

$$(G' \circ G)\langle A \rangle = G'\langle G\langle A \rangle\rangle.$$

因为凭借 C33 (章 I, § 4, no. 3) 关系 $z \in (G' \circ G)\langle A \rangle$ 相当于

$$(\exists y)((\exists x)(x \in A \text{ and } (x, y) \in G) \text{ and } (y, z) \in G')$$

因此相当于 $(\exists y)(y \in G\langle A \rangle$ 和 $(y, z) \in G')$；因此结果。

¶ 如果 G 和 G′ 是两个图，则有 $\mathrm{pr}_1(G' \circ G) = \overset{-1}{G}\langle \mathrm{pr}_1 G'\rangle$ 和 $\mathrm{pr}_2(G' \circ G) = G'\langle \mathrm{pr}_2 G\rangle$。对于例，要证明其中的第二个关系，注就足以证明关系$z \in \mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G})$等价于$(\exists x)((x, z) \in \mathrm{G}' \circ \mathrm{G})$，因此

$$(\exists y)((\exists x)((x, y) \in \mathrm{G}) \quad \text{and} \quad (y, z) \in \mathrm{G}');$$

但这相当于$z \in \mathrm{G}'\langle \mathrm{pr}_2\mathrm{G}\rangle$。

¶ 如果 G 是一个图并且 X 集合使得 $\mathrm{X} \subset \mathrm{pr}_1\mathrm{G}$，我们有

$$\mathrm{X} \subset \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle.$$

对于关系$x \in \mathrm{X}$，假设意味着$(\exists y)((x, y) \in \mathrm{G})$；但$(x, y) \in \mathrm{G}$等价于$(y, x) \in \overset{-1}{\mathrm{G}}$，另一方面$(x, y) \in \mathrm{G}$意味着$(\exists z)(z \in \mathrm{X}$和$(z, y) \in \mathrm{G})$；因此 $x \in \mathrm{X}$ 意味着

$$(\exists y)((\exists z)(z \in \mathrm{X} \quad \text{and} \quad (z, y) \in \mathrm{G}) \quad \text{and} \quad (y, x) \in \overset{-1}{\mathrm{G}}),$$

也就是说，$x \in \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle$。

¶ 很明显，如果$\mathrm{G}_1$、$\mathrm{G}_2$、$\mathrm{G}'_1$、$\mathrm{G}'_2$是图，则关系、$\mathrm{G}_1 \subset \mathrm{G}_2$和$\mathrm{G}'_1 \subset \mathrm{G}'_2$隐含$\mathrm{G}'_1 \circ \mathrm{G}_1 \subset \mathrm{G}'_2 \circ \mathrm{G}_2$。

¶ 令$\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$和$\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$为两个对应，使得$\Gamma$的目标与$\Gamma'$的源相同。从上面的讨论我们有$\mathrm{pr}_1(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_1\mathrm{G} \subset \mathrm{A}$和$\mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_2\mathrm{G}' \subset \mathrm{C}$；因此我们可以声明以下定义：

#### 定义 7 {#ens-ii-s3-def-7 .statement tag=03PO}

*设*$\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$*和*$\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$*为两个对应，使得*$\Gamma$*的目标是*$\Gamma'$的源。 *则对应* $(\mathrm{G}' \circ \mathrm{G}, \mathrm{A}, \mathrm{C})$ *称为* $\Gamma'$ *和* $\Gamma$ 的合成，*并表示为* $\Gamma' \circ \Gamma$（或有时 $\Gamma'\Gamma$）。

从命题 5 可以立即得出，如果 X 是 A 的子集，我们就有 $(\Gamma' \circ \Gamma)\langle \mathrm{X}\rangle = \Gamma'\langle \Gamma\langle \mathrm{X}\rangle\rangle$。此外，由于$\overset{-1}{\Gamma'}$的目标与$\overset{-1}{\Gamma}$的源相同，因此$\Gamma' \circ \Gamma$的逆是$\overset{-1}{\Gamma} \circ \overset{-1}{\Gamma'}$，乘以命题3。

#### 定义 8 {#ens-ii-s3-def-8 .statement tag=03PP}

*如果*A*是形式*$(x, x)$的所有对象、集合、集合*$\Delta_\mathrm{A}$*，*其中*$x \in \mathrm{A}$、*称为*$\mathrm{A} \times \mathrm{A}$的对角线。

显然我们有$\mathrm{pr}_1\Delta_\mathrm{A} = \mathrm{pr}_2\Delta_\mathrm{A} = \mathrm{A}$。 对应

$$\mathrm{I}_\mathrm{A} = (\Delta_\mathrm{A}, \mathrm{A}, \mathrm{A})$$

称为 A 上的*恒等式对应*；它是它自己的逆。

¶ 如果 A 和 B 之间的$\Gamma$ 是对应，且$\mathrm{I}_\mathrm{A}$、$\mathrm{I}_\mathrm{B}$ 分别是A、B 上的恒等式对应，则$\Gamma \circ \mathrm{I}_\mathrm{A} = \mathrm{I}_\mathrm{B} \circ \Gamma = \Gamma$。

### 4. FUNCTIONS

#### 定义 9 {#ens-ii-s3-def-9 .statement tag=03HN}

如果对于每个 x 至多有一个对象在 * F (章 I, § 5, no. 3) 下对应到 x，则 *graph* F * 被称为函数图。 *对应* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *如果其图* F *是函数图并且其源* A *等于其域* $\mathrm{pr}_1\mathrm{F}$，则称为函数。 *在其他字中，对应* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *是函数，如果对于每个 x 属于到源* A *f 关系* $(x, y) \in \mathrm{F}$ *在 y* (章 I, § 5, no. 3) 中起作用； *f下的对应到x的唯一对象被称为f在*A的元素x处的值，*并用*$f(x)$（*或*$f_x$，*或*$\mathrm{F}(x)$，*或*$\mathrm{F}_x$）表示。

如果$f$是函数，F是它的图，并且$f$的域的$x$元素、关系$y = f(x)$则等价于$(x, y) \in \mathrm{F}$（章I, § 5, no. 3，准则C46）。

#### 注 {#ens-ii-s3-n4-rem-1 .statement tag=03HO}

读者应注意同时使用定义 3 (cf. 习题 11)中引入的记号$f(x)$和$f(\mathrm{X})$（与$f\langle \mathrm{X} \rangle$同义）可能会引起混乱。

设A和B为两个集合； * A *到* B 的 *映射是函数 $f$，其源（等于其域）等于 A，其目标等于 B；这样的函数也被认为是在A上*定义的，并且在*B中*采用它的值。

通常使用以下短语来代替短语“let $f$ be 映射 of A into B”：“let $f : \mathrm{A} \to \mathrm{B}$ be 映射”甚至“let $f : \mathrm{A} \to \mathrm{B}$”。为了简化涉及多个映射的论证的表示，我们使用*图表*，例如

$$\begin{array}{ccccccccc} & f & & & g & \mathrm{C} & & i & \\ \mathrm{A} & \to & \mathrm{B} & \nearrow & & & \searrow & & \mathrm{E} \\ & & & \searrow & & \mathrm{D} & \nearrow & & \\ & & & h & & & j & & \end{array}$$

其中$\mathrm{A} \overset{f}{\to} \mathrm{B}$等符号的群应解释为$f$是A到B的映射。

A 上定义的函数 $f$ 据说是 *变换 x 变成* $f(x)$（对于所有 $x \in \mathrm{A}$）； $f(x)$ 被 f* 称为 x 的 *变换或（滥用语言）$f$ 下$x$ 的 *像*。

¶ 在某些情况下，函数图被称为*家族*；然后，域被称为 *指标集合*，范围被称为（滥用语言）家族的元素* 的 *集合。主要是在这方面，标记记号$f_x$用于表示元素$x$处的$f$的值。当指标集合为两个集合的积时，我们常说的是*双家庭*。

¶ Likewise a function whose target is E is sometimes called a *family of elements* of E. 如果 E 的每个元素都是集合 F 的子集，我们称 F 的 *子集* 族。

在整个级数中，我们经常使用字“函数”来代替“函数图”。

*例共函数*

#### 例 1 {#ens-ii-s3-n4-exa-1 .statement tag=03V1}

空集是一个函数图。每个图为空的函数都有等于空集的定义域和值域。其中函数中，目标为空的（即函数$(\varnothing,\varnothing,\varnothing)$）称为*空函数*。

#### 例 2 {#ens-ii-s3-n4-exa-2 .statement tag=03V2}

设A为集合。 A (no. 3) 的恒等式对应是函数，称为A的*恒等映射*。

因此，每个集合 A 都有一个关联的家庭，由 A 的恒等映射定义，其指标集合是 A，其元素的集合是 A。滥用语言，集合是有时被称为“家庭”，在这种情况下，它是与集合有问题。

如果对于 $f$ 域中的所有 $x$ 和 $x'$，我们有 $f(x)=f(x')$，则函数 $f$ 被称为“常数”。

¶ 设 $f$ 为集合 E 的映射到 E 中。如果 $f(x)=x$，则 E 的元素 $x$ 被认为*固定在* $f$ 下。

### 5. 限制和扩张函数

如果 E 包含在 $f$ 和 $g$ 的域中，并且如果 $f(x)=g(x)$ 对于所有 $x\in E$，则两个函数 $f$ 和 $g$ 被认为在集合 E 上*一致*（或 *重合*）。两个具有相同图的函数在其定义域上一致。说$f=g$就是说$f$和$g$具有相同的域A和相同的目标B，并且它们在A上一致。

¶ 令 $f=(F,A,B)$ 和 $g=(G,C,D)$ 为两个函数。说$F\subset G$就是说$f$的定义域A包含在$g$的定义域C中，并且$g$与A上的$f$一致。如果还有$B\subset D$，则$g$可以说是扩张* $f$（更准确地说，$f$到C的扩张），而$g$据说是*扩展* $f$（到C）。当$g$被称为D的元素*的*家族时，$f$被称为$g$的*子家族*。

¶ 令$f$ 为函数，并令A 为$f$ 域的子集。 直接的，关系“$x\in A$和$y=f(x)$”有一个关于$x$和$y$的图G，这个图是函数的，A是它的域；图为G的函数，与$f$有相同的目标，称为$f$到$A$的*限制*，用$f|A$表示为有时。 函数是其任意限制中的扩张。如果两个函数$f$、$g$有相同的目标并且在集合$E$上达成一致，那么它们的限制到$E$是相等的。

### 6. 定义函数通过项

C54。 *令$T$、$A$为两个项，并令$x$、$y$为不同的字母。假设$x$没有出现在$A$中，并且$y$没有出现在$T$或$A$中。令$R$为关系“$x \in A$和$y = T$”。 关系 $R$ 有一个关于字母 $x$ 和 $y$ 的图表 $F$。该图是函数式的；其第一个投影为$A$，其第二个投影为$x \in A$(§ 1, no. 6)形式$T$对象集合。对于每个$x \in A$，我们有$F(x) = T$。*

对于$x \in A$，令$B$为形式$T$的对象集合。然后

$$
R \Longrightarrow ((x,y) \in A \times B);
$$

由于$A \times B$包含表示的组件既不是$x$也不是$y$，所以$R$有一个关于字母$x$和$y$（no. 1）的图$F$。很明显关系

$$
(x,y) \in F \quad\text{and}\quad (x,y') \in F
$$

意味着$y = y'$，因此$F$是一个函数图。剩下的叙述是显而易见的。

¶ 如果 $C$ 是集合，其中形式 $T$ 的对象包含集合 $B$ $x \in A$（其中 $y$ 不出现在$C$），则函数 $(F,A,C)$ 也表示为记号 $x \to T$ ($x \in A$, $T \in C$)； 相应的在形式数学包含中的组装既不是$x$也不是$y$，并且不依赖于字母$y$满足上述条件的选择。 当上下文足够明确时，我们将允许自己记号$x \to T(x \in A)$、$(T)_{x \in A}$或$x \to T$，以及有时简单地$T$或$(T)$。 *因此，如果上下文清楚表明我们的意思是集合复数的映射 $x \to x^3$ 本身，我们就可以说“函数 $x^3$”。 \*

*例*

#### 例 1 {#ens-ii-s3-n6-exa-1 .statement tag=03S3}

如果$f$是$A$的映射入$B$，则函数$f$等于函数$x \to f(x)$（$x \in A$，$f(x) \in B$），简单写为$x \to f(x)$或$(f_x)_{x \in A}$ （后者记号尤其与短语“元素家族”相关，而不是“函数”）。

#### 例 2 {#ens-ii-s3-n6-exa-2 .statement tag=03S4}

令 G 为有序对的集合。 函数

$$z \to \mathrm{pr}_1 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_1 z \in \mathrm{pr}_1 \mathrm{G})$$

和

$$z \to \mathrm{pr}_2 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_2 z \in \mathrm{pr}_2 \mathrm{G})$$

分别称为* G 上的*第一和第二坐标函数；当不存在混淆风险时，它们用 $\mathrm{pr}_1$ 和 $\mathrm{pr}_2$ 表示。

### 7. 合成两个函数。逆函数

#### 命题 6 {#ens-ii-s3-prop-6 .statement tag=03HP}

*如果f是*A*到*B的映射，*并且g是*B*到*C的映射，*那么*$g \circ f$*是*A*到*C的映射。

设F、G分别为$f$、$g$的图，并证明$\mathrm{G} \circ \mathrm{F}$是函数图。令$x$、$z$、$z'$为对象，使得$(x, z) \in \mathrm{G} \circ \mathrm{F}$、$(x, z') \in \mathrm{G} \circ \mathrm{F}$。存在对象 $y$, $y'$ 使得

$$(x, y) \in \mathrm{F}, \qquad (x, y') \in \mathrm{F}, \qquad (y, z) \in \mathrm{G}, \qquad (y', z') \in \mathrm{G}.$$

由于 F 是函数图，因此我们有 $y = y'$，因此有 $(y, z') \in \mathrm{G}$。由于 G 是函数图，因此有 $z = z'$，这证明了我们的断言。此外，$g \circ f$的定义域显然是A，并且证明是完备的。

¶ 函数 $g \circ f$ 也可以写成 $x \to g(f(x))$，或者在不存在混淆风险的情况下写成 $gf$。

#### 定义 10 {#ens-ii-s3-def-10 .statement tag=03HQ}

*令f 为* A *到* B 的映射。 *映射 f 被称为单射，或单射，如果* A * 的任何两个不同的元素在 f 下具有不同的像。 映射 f 被称为满射，或满射，if* $f(\mathrm{A}) = \mathrm{B}$。 *如果 f 既是单射又是满射，则称为双射，或双射。*

我们有时不是说$f$是满射的说，而是说$f$是A *到* B上的映射，或者说它是B通过A的*参数表示*（在这种情况下，A被称为参数*的*集合） A 的表示和元素称为*参数*）。如果$f$是双射，我们有时说*f将*A*和*B*一对一的对应*。 A 的双射到 A 上称为 A 的 *置换*。

*例*

#### 例 1 {#ens-ii-s3-n7-exa-1 .statement tag=03S5}

如果A到B的$\mathrm{A} \subset \mathrm{B}$、映射其图是A的对角线是单射的，则称为A到B的*典范映射*或*典范嵌入*（或简称为*单射*）。

#### 例 2 {#ens-ii-s3-n7-exa-2 .statement tag=03S6}

设 A 为集合。 A 的映射$x \to (x, x)$到$\mathrm{A} \times \mathrm{A}$的对角线$\Delta_\mathbf{A}$是一个双射映射，称为A的*对角线映射*。

#### 例 3 {#ens-ii-s3-n7-exa-3 .statement tag=03S7}

令 G 为集合 / 有序对。 G 的映射 $\mathrm{pr}_1$（分别为 $\mathrm{pr}_2$）到 $\mathrm{pr}_1\mathrm{G}$（分别为 $\mathrm{pr}_2\mathrm{G}$）是满射； $\mathrm{pr}_1$ 是单射的当且仅当 G 是函数图。

#### 例 4 {#ens-ii-s3-n7-exa-4 .statement tag=03S8}

令 G 为有序对的集合。 映射

$$z \to (\mathrm{pr}_2 z,\ \mathrm{pr}_1 z)$$

G 到$\overset{-1}{\mathrm{G}}$ 的值是双射（称为*规范*双射）。

#### 例 5 {#ens-ii-s3-n7-exa-5 .statement tag=03S9}

设 A 为集合和 $b$ 一个对象。 A 的映射 $x \to (x,\ b)$ 到 $\mathrm{A} \times \{b\}$ 是双射。

#### 命题 7 {#ens-ii-s3-prop-7 .statement tag=03PQ}

*设$f$是*A*到*B的映射。*则*$\overset{-1}{f}$*是函数当且仅当$f$是双射的。*

如果$\overset{-1}{f}$为函数，则其源B等于其定义域，即$f(\mathrm{A})$；因而 $f$ 是满射的。为了证明$f$是单射的，让$x$和$y$是A的两个元素，使得$f(x) = f(y)$。如果 F 表示 $f$ 的图，我们有

$$(f(x),\ x) \in \overset{-1}{\mathrm{F}} \qquad \text{and} \qquad (f(y),\ y) \in \overset{-1}{\mathrm{F}},$$

因而

$$(f(x),\ y) \in \overset{-1}{\mathrm{F}},$$

这样$x = y$，就证明了断言。

¶ 相反，如果 $f$ 是双射，则直接的 $\overset{-1}{\mathrm{F}}$ 是泛函，并且$\overset{-1}{f}$ 的定义域等于 B。

当$f$是双射时，$\overset{-1}{f}$称为$f$的*逆映射*； $\overset{-1}{f}$是双射，$\overset{-1}{f} \circ f$是A的恒等映射，$f \circ \overset{-1}{f}$是B的恒等映射。

¶ 如果置换与其逆元相同，则称其为*对合*。

#### 注 {#ens-ii-s3-n7-rem-1 .statement tag=03HR}

令 $f$ 为 A 到 B 的映射。对于 A 的每个子集 X，我们有 (no. 3) $\mathrm{X} \subset \overset{-1}{f}\langle f\langle \mathrm{X}\rangle\rangle$。此外，对于 B 的每个子集 Y，我们有 $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle \subset \mathrm{Y}$，对于关系 $y \in f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle$ 相当于

$$(\exists x)((\exists z)(z \in \mathrm{Y} \text{ and } z = f(x)) \text{ and } y = f(x))$$

因此意味着关系$(\exists z)(z \in \mathrm{Y} \text{ and } y = z)$，因此也意味着关系$y \in \mathrm{Y}$。

如果$f$是*满射*，对于B的每个子集Y，我们有$f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle = \mathrm{Y}$，因为关系$y \in \mathrm{Y} \subset \mathrm{B}$意味着假设关系$(\exists x)(y = f(x))$，因此也有$(\exists x)(y \in \mathrm{Y} \text{ and } y = f(x))$；但“$y \in \mathrm{Y}$和$y = f(x)$”意味着$(\exists z)(z \in \mathrm{Y} \text{ and } z = f(x))$，我们的断言紧随其后。

如果 $f$ 是 *内射*，则对于 A 的每个子集 X，我们都有 $\overset{-1}{f}\langle f\langle X\rangle\rangle = X$。对于关系 $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ 相当于 $f(x) \in f\langle X\rangle$，因而

$$(\exists z)(z \in X \text{ and } f(z) = f(x));$$

但假设意味着$f(z) = f(x)$蕴含$z = x$，因而$x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$蕴含$x \in X$。

### 8. 缩回与截面

#### 命题 8 {#ens-ii-s3-prop-8 .statement tag=03HS}

*设$f$为* A *入* B的映射。 *如果存在映射$r$*（分别为$s$）*为* B *入* A *使得$r \circ f$*（分别为$f \circ s$）*为恒等映射* A（分别为 B），*则 $f$ 是单射*（分别为*满射*）。 *相反，如果$f$是满射，则存在* B *到* A *的映射 $s$使得$f \circ s$是* B的恒等映射。 *如果$f$是单射并且如果* A $\neq \emptyset$，*存在映射 * B *的$r$进入* A *使得$r \circ f$是* A的恒等映射。

如果存在 B 的映射 $r$ 到 A 中，使得 $r \circ f$ 是 A 的恒等映射，则等式 $f(x) = f(y)$，其中 $x \in A$ 和 $y \in A$ 隐含 $x = r(f(x)) = r(f(y)) = y$，因此 $f$ 是单射的。如果 A 中存在 B 的映射 $s$，使得 $f \circ s$ 是 B 的恒等映射，则我们有 $B = f(s(B)) \subset f(A) \subset B$，因此 $f$ 是满射。如果 $f$ 是满射，则令 T 表示项 $\tau_y(y \in A \text{ and } f(y) = x)$。我们有$f(T) = x$换$x \in B$；如果$s$表示映射$x \to T$$(x \in B, T \in A)$，则$f \circ s$是B的恒等映射。最后，假设$f$是单射且A$\neq \emptyset$，令$a$是A的元素。 关系

$$\text{“}(y \in A \text{ and } x = f(y)) \text{ or } (y = a \text{ and } x \in B - f(A))\text{''}$$

蕴含$(x, y) \in B \times A$，因此有一个关于字母$x$、$y$的图R。该图由于假设在 $f$ 上是函数的，并且以 B 为其定义域；如果$x \in B - f(A)$，我们有$R(x) = a$，如果$x \in f(A)$，我们有$f(R(x)) = x$。因此函数$r = (R, B, A)$使得$r \circ f$是A的恒等映射。

#### 推论{#ens-ii-s3-n8-cor-1 .statement tag=03HT}

*设* A，B *为集合，设$f$为* A *入* B的映射，*并令$g$为* B *入* A的映射。 *如果$g \circ f$是* A *的恒等映射且如果$f \circ g$是* B 的恒等映射，*则 $f$ 和 $g$ 是双射，且 $g = \overset{-1}{f}$.*

#### 定义 11 {#ens-ii-s3-def-11 .statement tag=03HU}

*设 $f$ 为* A *到* B 的单射*（或*满射*）*映射。*任意映射 $r$*（或$s$）*B *到* A *使得 $r \circ f$*（或$f \circ s$） *是* A（分别为B）的恒等映射*称为撤回*（分别为*截面*）*$f$。*

使用有时代替撤回（或截面）短语*左逆*（或*右逆*）。

¶ 如果 $f$ 是单射（或满射）并且 $r$（或 $s$）是 $f$ 的回缩（或截面），则 $f$ 是 $r$ 的截面（或回缩） （分别$s$）。因此，回缩是满射的，而截面是单射的。

¶ 如果$f$是满射且$s$、$s'$是$f$的两个截面，使得$s(\mathrm{B}) = s'(\mathrm{B})$，则$s = s'$；因为如果$x \in \mathrm{B}$，则存在$y \in \mathrm{B}$使得$s(x) = s'(y)$，并且我们有$x = f(s(x)) = f(s'(y)) = y$，因而$s(x) = s'(x)$，因而$s = s'$。因此截面$s$由集合$s(\mathrm{B})$唯一确定。滥用语言，集合$s(\mathrm{B})$被有时称为$f$*的*截面。

#### 定理 1 {#ens-ii-s3-thm-1 .statement tag=03PR}

*设$f$是*A*到*B的映射，*让$f'$是*B*到*C的映射，*并让$f'' = f' \circ f$。然后：*

(a) *如果$f$和$f'$是单射，那么$f''$就是单射。如果$r$、$r'$分别是$f$、$f'$的退化，则$r \circ r'$是$f''$的缩回。*

(b) *如果 $f$ 和 $f'$ 是满射，则 $f''$ 是满射。如果$s$、$s'$分别是$f$、$f'$的截面，那么$s \circ s'$就是$f''$的截面。*

(c) *如果$f''$ 是单射，则$f$ 是单射。如果 $r''$ 是 $f''$ 的缩回，则 $r'' \circ f'$ 是 $f$ 的缩回。*

(d) *如果 $f''$ 是满射，则 $f'$ 是满射。如果 $s''$ 是 $f''$ 中的截面，则 $f \circ s''$ 是 $f'$ 中的截面。*

(e) *如果 $f''$ 是满射且 $f'$ 单射，则 $f$ 是满射。如果$s''$是$f''$中的截面，则$s'' \circ f'$是$f$中的截面。*

(f) *如果$f''$是单射并且$f$是满射，那么$f'$是单射。如果 $r''$ 是 $f''$ 的缩回，则 $f \circ r''$ 是 $f'$ 的缩回。*

对于每个集合 E，令 $\mathrm{I_E}$ 表示 E 的恒等映射。

(a) 我们有 $r \circ f = \mathrm{I_A}$ 和 $r' \circ f' = \mathrm{I_B}$，因此

$$(r \circ r') \circ (f' \circ f) = r \circ \mathrm{I_B} \circ f = r \circ f = \mathrm{I_A}.$$

如果 $f$ 和 $f'$ 为单射，则 $f''$ 为单射，如果 $\mathrm{A} \neq \emptyset$，则为命题 8，如果为 $\mathrm{A} = \emptyset$，则为命题 8。

(b) 我们有 $f \circ s = \mathrm{I_B}$ 和 $f' \circ s' = \mathrm{I_C}$，因此

$$(f' \circ f)(s \circ s') = f' \circ \mathrm{I_B} \circ s' = f' \circ s' = \mathrm{I_C}.$$

如果 $f$ 和 $f'$ 是满射，则 $f''$ 是命题 8 的满射。

(c) 我们有$r'' \circ f'' = \mathrm{I_A}$，因此有$(r'' \circ f') \circ f = r'' \circ f'' = \mathrm{I_A}$。如果$f''$是单射，那么$f$就是单射，如果$\mathrm{A} \neq \emptyset$则命题 8，如果$\mathrm{A} = \emptyset$则很简单。

(d) 我们有$f'' \circ s'' = \mathrm{I_C}$，因此有$f' \circ (f \circ s'') = f'' \circ s'' = \mathrm{I_C}$。如果 $f''$ 是满射，则 $f'$ 是命题 8 的满射。

(e) 我们有$f'' \circ s'' = \mathrm{I_C}$，并且通过(d) $f'$ 是双射。因此

$$f \circ (s'' \circ f') \;=\; (\overset{-1}{f}{}' \circ f') \circ f \circ (s'' \circ f') \;=\; \overset{-1}{f}{}' \circ (f'' \circ s'') \circ f'$$
$$= \overset{-1}{f}{}' \circ \mathrm{I_C} \circ f' = \overset{-1}{f}{}' \circ f' = \mathrm{I_B}.$$

如果 $f''$ 是满射且 $f'$ 单射，则 $f$ 是命题 8 的满射。

(f) 我们有 $r'' \circ f'' = \mathrm{I_A}$，并且通过 (c) $f$ 是双射。因此

$$(f \circ r'') \circ f' = (f \circ r'') \circ f' \circ (f \circ \overset{-1}{f}) = f \circ (r'' \circ f'') \circ \overset{-1}{f} = f \circ \mathrm{I_A} \circ \overset{-1}{f}$$
$$= f \circ \overset{-1}{f} = \mathrm{I_B}.$$

如果$f''$是单射并且$f$是一个满射，那么$f'$是单射，如果$\mathrm{A} \neq \emptyset$则命题 8，并且如果$\mathrm{A} = \emptyset$（因为那么我们有$\mathrm{B} = f\langle \mathrm{A}\rangle = \emptyset$）。

#### 命题 9 {#ens-ii-s3-prop-9 .statement tag=03PS}

(a) *设* E，F，G *为集合，让* $g$ *为* E *的映射*到* F *和* $f$ *映射 of * E *到* G。*则存在* F *到* G *的映射* $h$ *这样* $f = h \circ g$ *当且仅当关系* $g(x) = g(y)$ *（其中* $x \in \mathrm{E}$，$y \in \mathrm{E}$*）意味着关系* $f(x) = f(y)$。 *映射* $h$ *则由* $f$唯一确定； *如果*$s$*是*$g$的截面，*我们有*$h = f \circ s$。

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

(b) *设* E、F、G *为集合，让* $g$ *为* F *的单射 *入* E，*且令* $f$ *为* G *入* E 的映射。 *则存在映射* $h$ *of* G *进入*F*使得*$f = g \circ h$*当且仅当*$f(\mathrm{G}) \subset f(\mathrm{F})$。 *映射* $h$ *由* $f$唯一确定； *如果*$r$*是*$g$的撤回，*我们有*$h = r \circ f$。

(a) 如果$f = h \circ g$、关系 $g(x) = g(y)$（其中$x \in \mathrm{E}$、$y \in \mathrm{E}$）明确暗示$f(x) = f(y)$。对于 $g$ 中的每截面 $s$，我们有

$$h = h \circ (g \circ s) = f \circ s,$$

这表明$h$由$f$唯一确定。相反，假设关系$g(x) = g(y)$蕴涵$f(x) = f(y)$；令$s$为$g$中的截面，并令$h = f \circ s$；那么对于每个$x \in E$，我们有$g(s(g(x))) = g(x)$，因此有$f(s(g(x))) = f(x)$，即$h(g(x)) = f(x)$，因此有$f = h \circ g$。

(b) 如果$f = g \circ h$，那么显然是$f(G) \subset f(F)$，并且对于$g$的每一次收回$r$，我们都有$h = (r \circ g) \circ h = r \circ f$，这表明$h$是由$f$唯一确定的。相反，假设$f(G) \subset f(F)$；令$r$为$g$的缩回，并放入$h = r \circ f$；对于每个$x \in G$，都存在$y \in F$使得$f(x) = g(y)$，因此

$$g(h(x)) = g(r(f(x))) = g(r(g(y))) = g(y) = f(x)$$

因此$f = g \circ h$。

### 9. 函数两个参数

两个参数*的*函数是函数，其域是有序对的集合（或者等效地，乘积的子集）。令$f$为函数；如果$(x, y)$是$f$域的元素，元素$(x, y)$处$f$的值$f((x, y))$一般用$f(x, y)$表示。

¶ 令 $f$ 为两个参数的函数，D 为其定义域，C 为其目标。对于每个$y$，令$A_y$为所有$x$的集合，使得$(x, y) \in D$（即$\overset{-1}{D}$在$y$（no. 1）处的截面）。 映射

$$x \to f(x, y) \quad (x \in A_y, f(x, y) \in C)$$

被称为*由$f$定义的部分映射，相对于第二个参数*的值$y$，并由$f(\bullet, y)$或$f(\ , y)$（或有时$f_y$）表示；我们为所有 $(x, y) \in D$ 提供了 $f(\bullet, y)(x) = f(x, y)$。类似地，对于每个$x$，令$B_x$为所有$y$的集合，使得$(x, y) \in D$。 映射

$$y \to f(x, y) \quad (y \in B_x, f(x, y) \in C)$$

被称为*由$f$定义的部分映射，相对于第一个参数*的值$x$，并由$f(x, \bullet)$或$f(x, \ )$（或有时$f_x$）表示；我们为所有 $(x, y) \in D$ 提供了 $f(x, \bullet)(y) = f(x, y)$。

¶ 如果对于每个 $y$（分别为 $x$），部分映射 $f(\bullet, y)$（分别为 $f(x, \bullet)$）是常数映射，我们说 $f$ *不依赖于*它的第一个（或第二个）参数；因此，这意味着每当 $(x, y)$ 和 $(x', y)$ 属于到 D 时，$f(x, y) = f(x', y)$（或每当 $(x, y)$ 和 $(x, y')$ 属于到 D 时，$f(x, y) = f(x, y')$）。对于 D 的每个$y$属于到第二个投影，让$g(y)$表示$x \in A_y$的$f(x, y)$的公共的值； 映射 $y \to g(y)$ 则 $\mathrm{pr}_2 D$ 的映射变为C，使得

$$g(y) = f(x, y) \qquad \text{for all } (x, y) \in D.$$

¶ 相反，令 $g$ 为集合 B 的映射到集合 C，并令 A 为任意集合。那么$A \times B$到C的映射$(x, y) \to g(y)$不依赖于它的第一个参数。

¶ 令 $u$ 为 A 的映射到 C 和 B 的 $v$ 映射到 D。 $A \times B$ 到 $C \times D$ 的映射 $z \to (u(\mathrm{pr}_1 z), v(\mathrm{pr}_2 z))$ 称为 (*规范*) *扩张 $u$ and $v$ to 乘积集合*, or simply *乘积 of $u$ and $v$* (if there is no risk of confusion);它的范围是$u\langle A\rangle \times v\langle B\rangle$。用$u \times v$表示。 If $u$ and $v$ are injective (resp. surjective) then $u \times v$ is injective (resp. surjective). If $u$ and $v$ are bijective, then $u \times v$ is bijective, and its inverse 映射 is $\overset{-1}{u} \times \overset{-1}{v}$. If $u'$ is 映射 of C into 集合 E and if $v'$ is 映射 of D into 集合 F, we have

$$(u' \times v') \circ (u \times v) = (u' \circ u) \times (v' \circ v).$$

如果U、V分别是$u$、$v$的图，则$u \times v$的图W是$(A \times B) \times (C \times D)$的有序对$((x,y), (z, t))$的集合，使得$(x, z) \in U$和$(y, t) \in V$； 映射 $((x, y), (z, t)) \to ((x, z), (y, t))$ puts W in one-to-one 对应 with 乘积 $U \times V$ (子集 of $(A \times C) \times (B \times D)$) (cf. §5, no. 5).

### 习题 {#ens-ii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
