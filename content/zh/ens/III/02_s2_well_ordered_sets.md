---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 2
section_title: Well-ordered sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 148-157, 221-229
pdf_pages: 0154-0163, 0227-0235
extraction: ocr
subsections:
    - "no": 1
      title: SEGMENTS OF A WELL-ORDERED SET
      page: 148
      pdf_page: 154
    - "no": 2
      title: THE PRINCIPLE OF TRANSFINITE INDUCTION
      page: 151
      pdf_page: 157
    - "no": 3
      title: ZERMELO'S THEOREM
      page: 152
      pdf_page: 158
    - "no": 4
      title: INDUCTIVE SETS
      page: 154
      pdf_page: 160
    - "no": 5
      title: ISOMORPHISMS OF WELL-ORDERED SETS
      page: 155
      pdf_page: 161
    - "no": 6
      title: LEXICOGRAPHIC PRODUCTS
      page: 157
      pdf_page: 163
statements: 28
exercises: 20
content_sha256: 8bfb0ab6520a2aa4dd38ca55360283b271ebf17c47eac8f42ac759a328527fe2
translated_from: content/en/ens/III/02_s2_well_ordered_sets.md
translation_method: google
source_content_sha256: 529e0877ab160d3b3e3d67615a04958e997ebf0f3443b7d1ff61efd5c0edeeb3
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: d1dfd9bd0574105e93b0777eb20a79c3fb8e06c5b0240b25baead9fdd8c65599
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. WELL-ORDERED SETS

### 1. 段良序集

关系 $\mathrm{R}\{x, y\}$ 被认为是$x$和$y$之间的*良序关系*，如果R是$x$和$y$之间的序关系，并且如果对于每个非空集合E，其中$\mathrm{R}\{x, y\}$诱导序关系（即，$x \in \mathrm{E}$暗示$\mathrm{R}\{x, x\}$；cf.§ 1, no. 1），E，按此关系排序，具有*至少元素*。

¶ 集合 E 按顺序 $\Gamma$ 排序，如果关系 $y \in \Gamma\langle x\rangle$ 是$x$ 和 $y$ 之间的良序关系，则称其为“良序”； $\Gamma$ 被称为 E 上的*良序*。以下定义与此等效：

#### 定义 1 {#ens-iii-s2-def-1 .statement tag=03JY}

*集合* E *如果它是有序的并且如果* E *的每个非空子集都有至少元素，则称它是良序的。*

良序集 E 是全序的，因为 E 的每个子集 $\{x, y\}$ 都有至少元素。 E 的每个子集 A 在 E 中上界，在 E 中至少有上界。

*例*

#### 例 1 {#ens-iii-s2-n1-exa-1 .statement tag=03SX}

设 $\mathrm{E} = \{\alpha, \beta\}$ 为集合，其元素不同。容易验证$\mathrm{E} \times \mathrm{E}$的子集$\{(\alpha, \alpha), (\beta, \beta), (\alpha, \beta)\}$是E上的良序图。

#### 例 2 {#ens-iii-s2-n1-exa-2 .statement tag=03SY}

良序集的每个子集（特别是空的子集）都通过归纳排序进行了良序排列。

#### 例 3 {#ens-iii-s2-n1-exa-3 .statement tag=03SZ}

\* 非良序的全序集的存在性等价于无穷大公理（§ 4, no. 4，推论1到命题3，以及习题3）。

#### 例 4 {#ens-iii-s2-n1-exa-4 .statement tag=03T0}

如果$\Gamma$是E上的良序，则仅当E是有限的（§ 4，习题3）时，与$\Gamma$相反的排序才是E上的良序。 \*

#### 例 5 {#ens-iii-s2-n1-exa-5 .statement tag=03T1}

令 E 为良序集。邻接 E 最大元素 $b$ (§ 1, no. 7) 得到的集合 $\mathrm{E}_1$ 是良序的，因为如果 H 是 $\mathrm{E}_1$ 中除 $\{b\}$ 以外的任何非空子集，则 $\mathrm{H} \cap \mathrm{E}$ 中最小的元素也是最小的H.的元素

#### 注 {#ens-iii-s2-n1-rem-1 .statement tag=03JZ}

\* 作为无穷大公理（§ 6, no. 1）的推论，对于自然整数的例集合$\mathbf{N}$，存在没有最大元素的良序集。 \*

#### 定义 2 {#ens-iii-s2-def-2 .statement tag=03QN}

*在* E 的有序集合* E、*子集 *中，关系* $x \in \mathrm{S}$、$y \in \mathrm{E}$、*和* $y \leqslant x$ *意味着* $y \in \mathrm{S}$ *被称为* E 的段。

显然，E 的段的每个交和并都是 E 的线段。如果 S 是 E 的线段，则 S 的每个线段也是 E 的线段。集合 E 本身和空集是 E 的段。

#### 命题 1 {#ens-iii-s2-prop-1 .statement tag=03QO}

*在良序集* E 中，*除* E 之外的* E 的每个线段本身都是一个区间* $]\leftarrow, a[$，*其中* $a \in \mathrm{E}$。

令 S 为 E 的线段，使得 $\mathrm{S} \neq \mathrm{E}$。由于 $\mathrm{E} - \mathrm{S}$ 不为空，因此它至少有元素 $a$。由于定义2，关系$x \geqslant a$蕴含$x \notin \mathrm{S}$；否则我们就会得到$a \in \mathrm{S}$，这是荒谬的。因而$\mathrm{E} - \mathrm{S}$是区间$[a, \rightarrow[$，S是区间$]\leftarrow, a[$。

¶ 对于全序集 E 中的每个元素 $x$，线段 $]\leftarrow, x[$ 称为具有端点 x* 的*线段，并用 $\mathrm{S}_x$ 表示。

注如果 E 是良序且非空，则 $\mathrm{S}_x$ 至少有元素 $\alpha$，因此也是区间 $[\alpha, x[$。

令 E 为全序集。 $\mathrm{S}_x$的并 A，因为$x$贯穿E，如果E没有最大元素，则为E；如果 E 有最大元素 $b$，我们就有 $\mathrm{A} = \mathrm{E} - \{b\}$。

#### 命题 2 {#ens-iii-s2-prop-2 .statement tag=03QP}

*集合* E\* *of 段 of 良序集* E *通过包含良序。 映射* $x \rightarrow \mathrm{S}_x$ *是良序集* E *的同构到* E *的段集合，除了* E *本身。

显然，如果$x \in \mathrm{E}$和$y \in \mathrm{E}$，关系$x \leqslant y$蕴含$\mathrm{S}_x \subset \mathrm{S}_y$，$x < y$蕴涵$\mathrm{S}_x \neq \mathrm{S}_y$；因而，映射$x \rightarrow \mathrm{S}_x$是E的同构到E的段的集合S(E)上，与E本身不同(§ 1, no. 12，命题11)，因此S(E)是良序的。此外，E\* 与通过邻接最大元素从 S(E) 获得的良序集同构。

#### 命题 3 {#ens-iii-s2-prop-3 .statement tag=03QQ}

*让*$(\mathrm{X}_\iota)_{\iota \in \mathbf{I}}$*成为良序集的一个族，这样对于指标*$(\iota, \varkappa)$*中的每个对*集合*$\mathrm{X}_\iota$，$\mathrm{X}_\varkappa$*是另一个的一部分。那么集合* $\mathrm{E} = \bigcup_{\iota \in \mathbf{I}} \mathrm{X}_\iota$ * 上存在唯一的排序，其中诱导是每个* $\mathrm{X}_\iota$ 上的给定排序。 *赋予这个顺序，* E *是良序集。 * $\mathrm{X}_\iota$ *的每个* *段都是* E的段； *对于每个* $x \in \mathrm{X}_\iota$，*具有端点* $x$ *in* $\mathrm{X}_\iota$ *等于具有端点* $x$ *in* E 的线段； *并且* E *的每个段要么是* E *本身，要么是* $\mathrm{X}_\iota$之一的段。

第一个断言是以下一般引理的推论：

#### 引理 1 {#ens-iii-s2-lem-1 .statement tag=03QR}

*让*$(\mathrm{X}_\alpha)_{\alpha \in \mathrm{A}}$*成为有序集的一个家庭，针对关系*$\subset$（在其他字中，使得对于指标$\alpha$中的每个对，$\beta$都存在指标） $\gamma$使得$\mathrm{X}_\alpha \subset \mathrm{X}_\gamma$和$\mathrm{X}_\beta \subset \mathrm{X}_\gamma$）。 *假设，对于指标* $(\alpha, \beta)$ *中的每个对，使得* $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$，*在* $\mathrm{X}_\alpha$ *上由* $\mathrm{X}_\beta$ *引起的排序与在* $\mathrm{X}_\alpha$上的给定排序相同。 *在这些条件下，集合* $\mathrm{E} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{X}_\alpha$ *存在唯一的排序，其中诱导每个* $\mathrm{X}_\alpha$ 上的给定排序。

令 $\mathrm{G}_\alpha$ 为$\mathrm{X}_\alpha$ 上给定排序的图。如果 G 是 E 上的一个排序的图，其中每个 $\mathrm{X}_\alpha$ 都有诱导，而图为 $\mathrm{G}_\alpha$ 的排序，那么对于每个 $\alpha \in \mathrm{A}$，我们必须有 $\mathrm{G}_\alpha \subset \mathrm{G}$；因此 G 包含 $\bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$。另一方面，对于E的元素的每个对$(x, y)$，存在假设指标$\alpha \in \mathrm{A}$，使得$x \in \mathrm{X}_\alpha$和$y \in \mathrm{X}_\alpha$；如果$(x, y) \in \mathrm{G}$，我们有$(x, y) \in \mathrm{G}_\alpha$，所以$\mathrm{G} \subset \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$。因此，如果 E 上所需的排序存在，则其图必然为 $\mathrm{G} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$。仍有待证明的是，这个集合满足条件或引理。由于 $\mathrm{G}_\beta \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ 如果 $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$，我们对所有 $\alpha \in \mathrm{A}$ 都有 $\mathrm{G} \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$；另一方面，从假设可以得出，E 属于的任意三个元素 $x$、$y$、$z$ 都可以推导出同一个$\mathrm{X}_\alpha$。因此$(x, y) \in \mathrm{G}$在E上是序关系，引理得证。

¶ 我们现在选取命题 3 中的证明。首先让我们证明每个 $\mathrm{X}_\iota$ 都是 E 的一段。事实上，如果 $x \in \mathrm{X}_\iota$、$y \in \mathrm{E}$ 和 $y \leqslant x$，则存在指标 $\varkappa$，使得 $\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ 和$y \in \mathrm{X}_\varkappa$；因为假设$\mathrm{X}_\iota$是$\mathrm{X}_\varkappa$的一段，所以我们有$y \in \mathrm{X}_\iota$，这证明了断言。同样推理证明，对于每个$x \in \mathrm{X}_\iota$，$\mathrm{X}_\iota$中端点为$x$的线段与E中的区间$]\leftarrow, x[$相同。接下来让我们证明E是良序的。如果 H 是 E 的非空子集，则有指标 $\iota \in \mathrm{I}$ 使得 $\mathrm{H} \cap \mathrm{X}_\iota \neq \emptyset$；如果$a$是$\mathrm{X}_\iota$中$\mathrm{H} \cap \mathrm{X}_\iota$的最小元素，则$a$也是E中H的最小元素。也就是说，如果$x \in \mathrm{H}$，则存在指标$\varkappa \in \mathrm{I}$使得$\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$和$x \in \mathrm{X}_\varkappa$；我们不能有$x < a$，因为区间$]\leftarrow, a[$包含在$\mathrm{X}_\iota$中，因此我们有$x \geqslant a$，因为$\mathrm{X}_\varkappa$是全序的。

¶ 最后，我们必须证明 E 的一段（除了 E 本身之外）是 $\mathrm{X}_\iota$ 之一的段；这是前面参数的直接的推论，因为这样的段是形式$]\leftarrow, x[$（命题1）并且从$x$属于到一些$\mathrm{X}_\iota$。

### 2. 超限归纳原理

#### 引理 2 {#ens-iii-s2-lem-2 .statement tag=03K0}

令$E$为良序集，并令$\mathfrak{S}$为$E$的段的集合，具有以下性质： (1) 段属于到$\mathfrak{S}$的每一个并属于至$\mathfrak{S}$； (2) 如果$S_x\in\mathfrak{S}$，则$S_x\cup\{x\}\in\mathfrak{S}$。然后是$E$属于到$\mathfrak{S}$的每一段。

假设$E$中有段不属于属于到$\mathfrak{S}$，令$S$为其中的最小的（no. 1，命题2）。如果$S$没有最大元素，则$S$是与$S$本身不同的$S$的段的并，并且这些段属于凭借定义到$\mathfrak{S}$ $S$；因此$S\in\mathfrak{S}$，这是荒谬的。另一方面，如果$S$有最大元素$a$，则$S=S_a\cup\{a\}$，并且由于$S_a$是$S$的一段，与$S$不同，所以我们有$S_a\in\mathfrak{S}$；但还有$S\in\mathfrak{S}$，这又是荒谬的。

¶ 为了更方便，我们将把自己置于一个理论 $\mathscr{T}$ 中，其中 $E$ 是集合 *良好排序*，由关系写成 $x\leq y$。然后我们有以下判据 ：

C59。 （原理 / 超限归纳）。 *令$R\{x\}$为$\mathscr{T}$中的关系（$x$不是$\mathscr{T}$的常数），使得关系

$$
(x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\}))\Rightarrow R\{x\}
$$

是$\mathscr{T}$中的定理。在这些下，条件关系$(x\in E)\Rightarrow R\{x\}$是$\mathscr{T}$中的定理。*

令 $\mathfrak{S}$ 为段 $S$ $E$ 的集合，使得 $(y\in S)\Rightarrow R\{y\}$。显然，段属于到$\mathfrak{S}$的每个并也是属于到$\mathfrak{S}$。另一方面，如果$S_x\in\mathfrak{S}$，我们通过假设得到$R\{x\}$；因而，案例分离的$(y\in S_x\cup\{y\})\Rightarrow R\{y\}$乘以方法。因而 (引理 2) $E\in\mathfrak{S}$，证明了该准则。

¶ 在 C59、关系的应用中

$$
x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\})
$$

通常称为“感应假设”。

¶ 接下来，对于$E$的$S$线段的每个映射$g$到集合$F$，以及对于每个$x\in S$，我们将用$S_x=]\leftarrow,x[$线段的$g^{(x)}$映射表示$E$ 到$g(S_x)$，其中重合，$g$ 到$S_x$。有了这个记号我们就有了

C60。 （映射的定义除以超限归纳。） *令$u$为字母，理论上$\mathscr{T}$为$\mathrm{T}\{u\}$项。 $E$存在集合$U$和映射$f$到$U$，这样对于所有$x\in E$我们有$f(x)=\mathrm{T}\{f^{(x)}\}$。此外，集合$U$和映射$f$由这些条件唯一确定。*

我们先证明唯一性。假设$f'$和$\mathrm{U}'$也是标准的满足条件。设$\mathfrak{S}$为E的段S的集合，使得S上有$f$和$f'$重合。显然，段属于到$\mathfrak{S}$的每个并也属于至 $\mathfrak{S}$。另一方面，如果$\mathrm{S}_x \in \mathfrak{S}$，则$f$和$f'$在$\mathrm{S}_x$上一致，因而$f^{(x)} = {f'}^{(x)}$；因而

$$f(x) = \mathrm{T}\{f^{(x)}\} = \mathrm{T}\{{f'}^{(x)}\} = f'(x),$$

这表明$\mathrm{S}_x \cup \{x\} \in \mathfrak{S}$。由此可知 $\mathrm{E} \in \mathfrak{S}$ (引理 2)，因此有 $f' = f$ 和 $\mathrm{U}' = f'(\mathrm{E}) = f(\mathrm{E}) = \mathrm{U}$。

¶ 现在让 $\mathfrak{S}_1$ 表示 E 的段 S 的集合，其中存在 S *onto* $\mathrm{U_S}$ 的集合 $\mathrm{U_S}$ 和映射 $f_\mathrm{S}$，这样对于所有 $x \in \mathrm{S}$，我们都有 $f_\mathrm{S}(x) = \mathrm{T}\{f^{(x)}\}$。 对于每个$\mathrm{S} \in \mathrm{S}_1$，$f_\mathrm{S}$和$\mathrm{U_S}$由证明的第一个部分唯一确定；特别是，如果$\mathrm{S}'$和$\mathrm{S}''$是两个段属于到$\mathfrak{S}_1$，使得$\mathrm{S}' \subset \mathrm{S}''$，那么$f_{\mathrm{S}'}$是$\mathrm{S}'$到$f_{\mathrm{S}''}(\mathrm{S}')$的映射，这与$f_{\mathrm{S}''}$一致$\mathrm{S}'$。 由此注可以得出，段属于到$\mathfrak{S}_1$的每个并也是属于到$\mathfrak{S}_1$（章II, § 4, no. 6，命题7）。 On the other hand, if $\mathrm{S}_x \in \mathfrak{S}_1$, we define on $\mathrm{S} = \mathrm{S}_x \cup \{x\}$ a function $f_\mathrm{S}$ extending $f_{\mathrm{S}_x}$ by putting

$$f_\mathrm{S}(x) = \mathrm{T}\{f_{\mathrm{S}_x}\}$$

（章II, § 4, no. 7，命题8）；从$f_\mathrm{S}^{(x)} = f_{\mathrm{S}_x}$开始，显然$\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_1$。因此 (引理 2) $\mathrm{E} \in \mathfrak{S}_1$ 和证明是完备的。

¶ 通常，此标准适用于存在集合 F 的情况，使得*对于 * E 段的每映射 h *到 * F 的子集 *我们有* $\mathrm{T}\{h\} \in \mathrm{F}$。那么通过应用 C60 得到的集合 U 就是* F 的*子集。对于上面使用的记号，令$\mathfrak{S}_2$ 为E 的段 S 的$\mathfrak{S}_1$ 由……组成的子集，使得$\mathrm{U_S} \subset \mathrm{F}$。显然，段属于到$\mathfrak{S}_2$的每一个并也是属于到$\mathfrak{S}_2$；另一方面，F 上的假设意味着如果 $\mathrm{S}_x \in \mathfrak{S}_2$，我们有 $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_2$。 断言现在源自引理 2。

### 3. ZERMELO'S THEOREM

#### 引理 3 {#ens-iii-s2-lem-3 .statement tag=03K1}

*设* E *为集合，让*$\mathfrak{S}$ *为* $\mathfrak{P}(\mathrm{E})$的子集，*并让* $p$ *为* $\mathfrak{S}$ *的映射*进入* E *使得* $p(\mathrm{X}) \notin \mathrm{X}$ *对于所有* $\mathrm{X} \in \mathfrak{S}$。 *则存在* E *的子集* M *和* M *上的良序* $\Gamma$ *，这样，如果* $x \leqslant y$ *表示关系* $y \in \Gamma\langle x \rangle$ *并且* $\mathrm{S}_x$ *表示段* $]\leftarrow, x]$，

(1) *对于所有* $x \in \mathrm{M}$ *我们有* $\mathrm{S}_x \in \mathfrak{S}$ *和* $p(\mathrm{S}_x) = x$；

(2) $\mathrm{M} \notin \mathfrak{S}$。

设$\mathfrak{M}$为$\mathrm{E} \times \mathrm{E}$满足的子集G的集合，以下条件：

(a) G 是 $\mathrm{pr}_1 \mathrm{G} = \mathrm{U}$ 上的良序图；

(b) 如果$x \leqslant y$表示U上的关系$(x, y) \in \mathrm{G}$，则对于每个$x \in \mathrm{U}$，线段$\mathrm{S}_x$使得$\mathrm{S}_x \in \mathfrak{S}$和$p(\mathrm{S}_x) = x$。

¶ 我们将证明，如果 G 和 G' 是 M 的两个元素，并且如果 U，U' 表示它们的第一个投影，则两个集合 U，U' 之一包含在另一个中，并且如果对于例，$\mathrm{U} \subset \mathrm{U}'$，则 $\mathrm{G} = \mathrm{G}' \cap (\mathrm{U} \times \mathrm{U})$（在其他字中，序关系 U 上由 U' 上的序关系诱导）并且 U 是 U' 的*段*。

¶ 考虑元素 $x \in \mathrm{U} \cap \mathrm{U}'$ 的集合 V，使得带有端点 $x$ 的段在 U 和 U' 中是相同的，并且由 U 和 U' 上的排序在该段上引起的排序是相同的。很明显，V 是 U 和 U' 中的*段*，并且在 V 上导出的顺序是相同的；因而，如果我们证明$\mathrm{V} = \mathrm{U}$或$\mathrm{V} = \mathrm{U}'$，我们的断言就会得到证明。让我们通过矛盾来论证并假设$\mathrm{V} \neq \mathrm{U}$和$\mathrm{V} \neq \mathrm{U}'$。令$x$为U中$\mathrm{U} - \mathrm{V}$的最小元素，并令$x'$为U'中$\mathrm{U}' - \mathrm{V}$的最小元素； U 中有 $\mathrm{V} = \mathrm{S}_x$，U' 中有 $\mathrm{V} = \mathrm{S}_{x'}$。但是通过假设、$\mathrm{V} \in \mathfrak{S}$ 和

$$x = p(\mathrm{S}_x), \qquad x' = p(\mathrm{S}_{x'}),$$

这样$x = x'$。因此定义$x \in \mathrm{V}$，这是荒谬的。

¶ We may therefore apply Proposition 3 of no. 1 to the set of first projections $\mathrm{U} = \mathrm{pr}_1 \mathrm{G}$ (where $\mathrm{G} \in \mathfrak{M}$) and thus obtain a well-ordered set

$$\mathrm{M} = \bigcup_{\mathrm{G} \in \mathfrak{M}} \mathrm{pr}_1 \mathrm{G}.$$

很容易看出M属于到$\mathfrak{M}$的排序图。如果我们有$\mathrm{M} \in \mathrm{S}$，那么，放入$a = p(\mathrm{M})$，我们应该有$a \notin \mathrm{M}$。因而，我们可以将 M 元素 $a$ 邻接为最大元素，并且集合 $\mathrm{M}' = \mathrm{M} \cup \{a\}$ 将是良序的。由于M'中有$\mathrm{M} = \mathrm{S}_a$，所以我们应该有$\mathrm{S}_a \in \mathfrak{S}$和$p(\mathrm{S}_a) = a$；因而，M' 上的排序图将是属于到 $\mathfrak{M}$，这是荒谬的。

注，如果$\emptyset \notin \mathfrak{S}$（特别是如果$\mathfrak{S}$为空），则由引理 3断言存在的集合 M是空集；这是从条件 1 of 引理 3 得出的。

#### 定理 1（策梅洛）{#ens-iii-s2-thm-1 .statement tag=03QS}

*每个集合* E *都可以好好排序*

令 $\mathfrak{S} = \mathfrak{P}(\mathrm{E}) - \{\mathrm{E}\}$ 为 E 中除 E 本身以外的所有子集中的集合。对于每个$\mathrm{X} \in \mathfrak{S}$让$p(\mathrm{X}) = \tau_x \ (x \in \mathrm{E} - \mathrm{X})$；因为关系$\mathrm{X} \in \mathfrak{S}$意味着$(\exists x)(x \in \mathrm{E} - \mathrm{X})$，所以我们有$p(\mathrm{X}) \in \mathrm{E} - \mathrm{X}$（章I, § 4, no. 1），因此有$p(\mathrm{X}) \notin \mathrm{X}$。因而，我们可以应用引理 3，因此在 E 的子集 M 上存在良序，使得 $\mathrm{M} \notin \mathfrak{S}$；但E中唯一不存在属于到$\mathfrak{S}$的子集是E本身，定理得证。

### 4. INDUCTIVE SETS

#### 定义 3 {#ens-iii-s2-def-3 .statement tag=03K2}

*有序集合* E *如果* E 的每个总共有序子集在* E 中有上界，则称其为归纳式。

*例*

#### 例 1 {#ens-iii-s2-n4-exa-1 .statement tag=03T2}

令$\mathfrak{F}$为集合A的子集集合，按包含排序，并且使得对于$\mathfrak{G}$属于的集合$\mathfrak{F}$并总共有序子集$\mathfrak{G}$到$\mathfrak{F}$。则$\mathfrak{F}$相对于关系$\subset$可归纳，因为$\mathfrak{G}$的集合并是$\mathfrak{P}(\mathrm{A})$中$\mathfrak{G}$的最小上界。

#### 例 2 {#ens-iii-s2-n4-exa-2 .statement tag=03T3}

相对于关系$\subset$归纳的一个重要的子集集合例是集合A的子集映射图集合$\mathfrak{F}$到集合 B. 因为$\mathfrak{F}$是$\mathfrak{P}(\mathrm{A} \times \mathrm{B})$的子集，并且说$\mathfrak{F}$的子集$\mathfrak{G}$完全通过包含排序意味着$\mathfrak{G}$的元素是映射的图，这样，给定这些映射中的任何两个，一个是另一个的扩张。紧接着，$\mathfrak{G}$的集合的并是$\mathfrak{F}$的元素（章II, § 4, no. 6，命题7）。因此A入B的子集映射的集合$\Phi(\mathrm{A}, \mathrm{B})$相对于$u$和$v$之间的序关系“$v$扩展$u$”可归纳。

#### 例 3 {#ens-iii-s2-n4-exa-3 .statement tag=03T4}

\* 根据无穷大公理 (§ 6, no. 1)，自然整数的良序集相对于关系 $\leqslant$ 不可归纳。 \*

#### 定理 2（“佐恩的引理”）{#ens-iii-s2-thm-2 .statement tag=03QT}

— *每个订购集合的电感都有极大元素。*

这个定理是以下结果的特例：

#### 命题 4 {#ens-iii-s2-prop-4 .statement tag=03K3}

*让* E *是一个有序的集合，其中每个良序子集都在上面有界；那么* E *有极大元素.*

如果$v$是X和$v \notin \mathrm{X}$的上界，我们可以说元素$v \in \mathrm{E}$是E的子集X的*严格上界*。令$\mathfrak{S}$为E的子集的集合，在E中具有严格的上界，并且对于每个$\mathrm{S} \in \mathfrak{S}$，将$p(\mathrm{S}) = \tau_v(v$是S$)$的严格上界；那么$p(\mathrm{S})$是S的严格上界。应用引理 3 of no. 3到$\mathfrak{S}$和$p$，我们看到存在E的子集M和M上的良序$\Gamma$，满足引理 3 中的条件；特别是，M 在 E 中没有严格的上界。此外，$\Gamma$ 与由 E 上的排序在 M 上导出的结果相同。对于 M 关系中“$y\in\Gamma\langle x\rangle$ 和 $x\ne y$”等价于 $x\in S_y$；由于$p(S_y)=y$是$S_y$的上界（相对于E上的排序），因此意味着E中的$x<y$。但这意味着M到E中的单射是严格递增的映射（M被赋予了$\Gamma$排序）；由于 M 是全序的，因此关系 $y\in\Gamma\langle x\rangle$ 和 $x\leq y$ 在 M 中是等价的（§ 1, no. 12，命题 11）。既然如此，E中存在M的假设上界$m$；但由于M没有严格的上界，因此$m$是E的极大元素。

#### 推论 1 {#ens-iii-s2-prop-4-cor-1 .statement tag=03K4}

*令 E 为归纳有序集合，并令 a 为 E 的元素。则存在 E 的极大元素 m，使得 $m\geq a$。*

由定义 3 可知，E 中元素 $x\geq a$ 的集合 F 是归纳性的，且 F 的极大元素在 E 中也是最大的。

#### 推论 2 {#ens-iii-s2-prop-4-cor-2 .statement tag=03K5}

*令 $\mathfrak{F}$ 为集合 E 的子集的集合，这样，对于 $\mathfrak{F}$ 的每个子集 $\mathfrak{G}$（按包含完全排序），并（分别为交） 集合至 $\mathfrak{G}$ 属于至 $\mathfrak{F}$；那么$\mathfrak{F}$有一个最大（或最小）元素。*

### 5. 同构良序集

#### 定理 3 {#ens-iii-s2-thm-3 .statement tag=03K6}

*设E和F为两个良序集。那么以下两个叙述至少有一个为真：*

(1) *在 F 的一段上存在唯一的 E 同构；*

(2) *在 E 的一段上存在唯一的 F 同构。*

设$\mathfrak{F}$为E的子集的映射到F中的集合，使得每个映射定义在E的一段上，并且是该段的同构到F的一段上。然后集合$\mathfrak{F}$，按关系排序$u$和$v$之间的“$v$扩展$u$”是归纳性的。因为如果$\mathfrak{G}$是$\mathfrak{F}$的总有序子集，则映射$u\in\mathfrak{G}$域的并S是E的段的并，因此它本身是E的一个段。如果$v$是E的最小上界 $\Phi(E,F)$ (no. 4, 例 2) 中的$\mathfrak{G}$，则$v(S)$是映射$u\in\mathfrak{G}$范围中的并，因此是F的一个段。最后，对于元素的每个对 S 的$x$、$y$，使得$x<y$存在$u\in\mathfrak{G}$，其域包含既是$x$又是$y$（因为$\mathfrak{G}$是全序的）；因为$v(x)=u(x)<u(y)=v(y)$，$v$是S到$v(S)$的同构，我们的断言就被证明了。

¶ 现在令$u_0$ 为$\mathfrak{F}$ (no. 4, 定理 2) 的极大元素，并令$S_0$ 为E 的线段，E 是$u_0$ 的域。如果我们证明$S_0=E$或$u_0(S_0)=F$，定理将被证明。让我们通过反证法来假设$S_0\ne E$和$u_0(S_0)\ne F$。然后将有元素$a\in E$和元素$b\in F$，使得$S_0=]-\leftarrow,a[$和$u_0(S_0)]=]-\leftarrow,b[$（no. 1，命题1）。通过将$u_1(a)=b$放入F中，将$]-\leftarrow,a]$段的扩展$u_0$到映射$u_1$；由于$u_1$是$]-\leftarrow,a]$的同构到线段$]-\leftarrow,b]$上，因此与……矛盾是$\mathfrak{F}$中$u_0$的最大值。

¶ 定理 3 中断言的唯一性是以下引理中的推论 ：

#### 引理 4 {#ens-iii-s2-lem-4 .statement tag=03K7}

*设E、F为两个良序集，并令f、g为E到F中的两个单调递增映射，使得$f(E)$是F的线段，g为严格递增的；那么 $f(x)\leq g(x)$ 对于所有 $x\in E$。*

相反，假设元素$y\in E$中的集合使得$f(y)>g(y)$不为空；那么这个集合将至少有元素$a$。如果$x<a$，则我们有$f(x)\leq g(x)<g(a)<f(a)$，因为$g$是严格递增的。由于$f(E)$是F的线段，因此存在$z\in E$使得$g(a)=f(z)$； $f$ 是递增，因此$f(z)<f(a)$ 意味着$z<a$。因此

$$f(z)\leq g(z)<g(a)=f(z),$$

这是荒谬的。

#### 推论 1 {#ens-iii-s2-lem-4-cor-1 .statement tag=03K8}

*只有良序集 E 的同构在 E 的一段上才是 E 的恒等映射在其自身上。*

将 $F=E$ 放入定理 3。

#### 推论 2 {#ens-iii-s2-lem-4-cor-2 .statement tag=03K9}

*设E、F为两个良序集。如果在 F 的线段 T 上存在 E 的同构 $f$，并且在 E 的线段 S 上存在 F 的同构 $g$，则我们必须有 $S=E$、$T=F$ 和 $g,f$ 互为逆。*

因为$g\circ f$是E的同构到E的线段$g(T)\subset S$上；根据推论1，我们有$g(T)=S=E$，$g\circ f$是E的恒等映射。同样，$f\circ g$是F的恒等映射，从而结果。

#### 推论 3 {#ens-iii-s2-lem-4-cor-3 .statement tag=03KA}

*良序集 E 的每个子集 A 都同构于 E 的一段。*

凭借定理 3 就足以证明在形式 $S_a$的A段上不存在E的同构$g$。如果存在，则$g$将是E的严格递增的映射进入E，使得$g(a)\in S_a$，在其他字中使得$g(a)<a$；但这不等式与……矛盾引理4（$f$为恒等映射）。

### 6. LEXICOGRAPHIC PRODUCTS

令$(E_\iota)_{\iota\in I}$为有序集的族，由*有序*集合I索引。考虑乘积集合$E=\displaystyle\prod_{\iota\in I}E_\iota$和关系

$$
\text{``}x\in E\text{ and }y\in E,\text{ and for the least index }\iota\in I\text{ such that }\operatorname{pr}_{\iota}x\ne\operatorname{pr}_{\iota}y,\text{ we have }\operatorname{pr}_{\iota}x<\operatorname{pr}_{\iota}y\text{''},
$$

我们用$R\{x,y\}$表示。显然，$R\{x,x\}$等价于$x\in E$，$R\{x,y\}$意味着$R\{x,x\}$和$R\{y,y\}$，$(R\{x,y\}\text{ and }R\{y,x\})$意味着$x=y$。而且很容易验证$(R\{x,y\}\text{ and }R\{y,z\})$蕴含$R\{x,z\}$（考虑至少指标$\iota\in I$，其中三个元素$\operatorname{pr}_{\iota}x$、$\operatorname{pr}_{\iota}y$、$\operatorname{pr}_{\iota}z$中至少有两个不相等）；因此$R\{x,y\}$是乘积集合E*上的*序关系。这个关系和它的排序定义被称为*字典序关系*和$E$上的*字典顺序*（由$I$和$E_\iota$上的给定排序引起）；具有这种排序的集合 E 被称为有序集$(E_\iota)_{\iota\in I}$家族的*字典乘积*。如果每个 $E_\iota$ 都是“全序”的，则字典顺序的乘积也是“全序”的。

### 习题{#ens-iii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
