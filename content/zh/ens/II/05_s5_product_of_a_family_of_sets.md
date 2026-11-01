---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 5
section_title: Product of a family of sets
lang: zh
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
content_sha256: b2b94a801a670ad708051cee985fd7f39f8739b7ca81e509b75fad961434ee31
translated_from: content/en/ens/II/05_s5_product_of_a_family_of_sets.md
translation_method: google
source_content_sha256: 0301ddc64f4634b2f737e77987e840c82975f71ef423fb30f170e6510997d48c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4f4280b8b135d61bc3347788835f61017342aaaf14cf7877b2e3c9a2b70e35d6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 5.集族的积

### 1. 集合子集公理

A4。 $(\forall \mathrm{X}) \ \mathrm{Coll}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X}).$

该公理意味着对于每一个集合X，都存在集合，其元素都是X的子集，即集合$\mathscr{E}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X})$（§1, no. 4）；这个集合记为$\mathfrak{P}(\mathrm{X})$，称为*X的子集的*集合。显然，如果$\mathrm{X} \subset \mathrm{X}'$，我们有$\mathfrak{P}(\mathrm{X}) \subset \mathfrak{P}(\mathrm{X}')$。

¶ 设 A、B 为两个集合，并令 $\Gamma$ 为 A 和 B 之间的对应。 *函数* $\mathrm{X} \to \Gamma \langle \mathrm{X} \rangle$ $(\mathrm{X} \subset \mathfrak{P}(\mathrm{A}), \ \Gamma \langle \mathrm{X} \rangle \in \mathfrak{P}(\mathrm{B}))$ 被称为 * $\Gamma$ * 的 * 规范扩张* （或简称为 *扩张*） * 子集*中的集合，用$\hat{\Gamma}$表示；它是 $\mathfrak{P}(\mathrm{A})$ 中的映射变成 $\mathfrak{P}(\mathrm{B})$。如果B和集合C之间$\Gamma'$是对应，则公式$(\Gamma' \circ \Gamma) \langle \mathrm{X} \rangle = \Gamma' \langle \Gamma \langle \mathrm{X} \rangle \rangle$表明$\Gamma' \circ \Gamma$的扩张到子集的集合是映射 $\hat{\Gamma}' \circ \hat{\Gamma}$。

#### 命题 1 {#ens-ii-s5-prop-1 .statement tag=03IJ}

(1) *如果* $f$ *是集合* E *到集合* F 的满射，*规范的扩张* $\hat{f}$ *of* $f$ *是* $\mathfrak{P}(\mathrm{E})$ *到* $\mathfrak{P}(\mathrm{F})$ 的满射。

(2) *如果* $f$ *是* E *的单射*进入* F，*规范的扩张* $\hat{f}$ *属于* $f$ *是* $\mathfrak{P}(\mathrm{E})$ *进入* $\mathfrak{P}(\mathrm{F})$的单射。

(1) 如果$s$是$f$的截面，则$f \circ s$是F的恒等映射，因此$\hat{f} \circ \hat{s}$是$\mathfrak{P}(\mathrm{F})$的恒等映射；因此 $\hat{f}$ 是满射，$\hat{s}$ 是 $\hat{f}$ (§3, no. 8) 的截面。

(2) 如果$E = \varnothing$，命题是明显的，因为那么$\mathfrak{P}(E) = \{\varnothing\}$。如果$E \ne \varnothing$且$r$是$f$的缩回，则$r \circ f$是$E$的恒等映射，因此$\hat{r} \circ \hat{f}$是$\mathfrak{P}(E)$的恒等映射；因此 $\hat{f}$ 是单射的，$\hat{r}$ 是 $\hat{f}$ (§3, no. 8) 的缩回。

### 2. 集合映射中的集合进入另一个

设$E$，$F$为集合。 $E$的映射到$F$的图是$E \times F$的子集。 $\mathfrak{P}(E \times F)$的元素的集合，其中性质是$E$的映射到$F$的图，因此是$\mathfrak{P}(E \times F)$的子集，用$F^E$表示。三元组$f = (G, E, F)$的集合，其中$G \in F^E$，因此是$E$的映射到$F$的集合；用$\mathfrak{F}(E, F)$表示。显然，$G \mapsto (G, E, F)$ 是$F^E$ 到$\mathfrak{F}(E, F)$ 的双射（称为规范的双射）。这个双射的存在使我们能够立即将与集合$F^E$相关的每个命题翻译为与$\mathfrak{F}(E, F)$相关的命题，反之亦然。

¶ 设 $E$、$E'$、$F$、$F'$ 为集合。令$u$为$E$中$E'$的映射，并令$v$为$F'$中$F$的映射。那么函数$f \mapsto v \circ f \circ u$就是$\mathfrak{F}(E, F)$的映射变成$\mathfrak{F}(E', F')$。

#### 命题 2 {#ens-ii-s5-prop-2 .statement tag=03Q5}

(1) *如果 $u$ 是 $E'$ 到 $E$ 的满射，并且 $F$ 的 $v$ 单射到 $F'$，则映射 $f \mapsto v \circ f \circ u$ 是单射的。*

(2) *如果$u$是$E'$到$E$的单射，并且$v$是$F$到$F'$的满射，则映射$f \mapsto v \circ f \circ u$是满射。*

我们假设集合 $E$、$E'$、$F$、$F'$ 都是非空的，因为否则命题就可以被简单地验证。

(1) 设$s$为$u$的截面，并令$r$为$v$的缩进（§3，定义11）。那么$r \circ (v \circ f \circ u) \circ s = I_F \circ f \circ I_E = f$，这样

$$
f \mapsto v \circ f \circ u
$$

是单射的。

(2) 令$r'$为$u$的缩进，令$s'$为$v$的截面。对于每个映射 $f' : E' \to F'$，我们都有 $v \circ (s' \circ f' \circ r') \circ u = f'$，这表明映射 $f \mapsto v \circ f \circ u$ 是满射的。

#### 推论{#ens-ii-s5-n2-cor-1 .statement tag=03Q6}

*如果$u$是$E'$的双射到$E$并且$v$是$F$的双射到$F'$，那么$f \mapsto v \circ f \circ u$是双射的。*

令$A$、$B$、$C$为三个集合，并令$f$为$B \times C$的映射到$A$。对于每个$y \in C$，令$f(\mathord{\cdot}, y)$为$B$的部分映射$x \mapsto f(x,y)$到$A$（§ 3, no. 9）； 函数 $y \mapsto f(\mathord{\cdot}, y)$ 是 $C$ 中的映射变成 $\mathfrak{F}(B, A)$。相反，对于$C$的每个映射$g$进入$\mathfrak{F}(B, A)$，都存在$\mathrm{B} \times \mathrm{C}$的唯一映射$f$进入A，使得每个$y \in \mathrm{C}$有$g(y) = f(\bullet, y)$，即映射 $(x, y) \to (g(y))(x)$。因此：

#### 命题 3 {#ens-ii-s5-prop-3 .statement tag=03Q7}

*如果对于* $\mathrm{B} \times \mathrm{C}$ *入* A *中的每个映射 $f$ *我们用* C *入* $\mathfrak{F}(\mathrm{B}, \mathrm{A})$的$\tilde{f}$ 映射 $y \to f(\bullet, y)$表示，*则函数 $f \to \tilde{f}$是双射*（称为*规范双射*）*$\mathfrak{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$*到*$\mathfrak{F}(\mathrm{C}, \mathfrak{F}(\mathrm{B}, \mathrm{A}))$。

类似地，我们将定义 $\mathfrak{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ 的*规范双射* 放到$\mathfrak{F}(\mathrm{B}, \mathfrak{F}(\mathrm{C}, \mathrm{A}))$ 上。由于映射和函数图之间一对一的对应，这些双射产生了$\mathrm{A}^{\mathrm{B} \times \mathrm{C}}$的*规范双射*到$(\mathrm{A}^{\mathrm{B}})^{\mathrm{C}}$（或$(\mathrm{A}^{\mathrm{C}})^{\mathrm{B}}$）。

### 3. 集族的积中的定义

令$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$为集合的族，并令F为具有域I的函数图，使得每个$\iota \in \mathrm{I}$都有$\mathrm{F}(\iota) \in \mathrm{X}_\iota$。那么对于每个$\iota \in \mathrm{I}$，我们有$\mathrm{F}(\iota) \in \mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$，因此F是$\mathfrak{P}(\mathrm{I} \times \mathrm{A})$的元素。具有上述性质的函数图因此形式子集为$\mathfrak{P}(\mathrm{I} \times \mathrm{A})$。

#### 定义 1 {#ens-ii-s5-def-1 .statement tag=03Q8}

*设$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是集合的一个家庭。函数图* F *的集合，其定义域* I *使得* $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ *对于每个* $\iota \in \mathrm{I}$ *被称为集合 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$族的乘积，并用* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$表示。 *对于每个* $\iota \in \mathrm{I}$、$\mathrm{X}_\iota$ *在乘积* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ 中称为指标 $\iota$ 的因子。 *映射* $\mathrm{F} \to \mathrm{F}(\iota)$ $\left( \mathrm{F} \in \prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota,\ \mathrm{F}(\iota) \in \mathrm{X}_\iota \right)$ *称为指标 $\iota$的坐标函数*（或*投影*）*，并用* $\mathrm{pr}_\iota$表示。

$\mathrm{F}(\iota)$称为F的指标*$\iota$的*坐标（或指标*$\iota$的*投影）； 指标$\iota$的坐标函数下$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$的子集A的像$\mathrm{pr}_\iota\langle \mathrm{A} \rangle$称为A的指标*$\iota$的*投影。容易验证$\mathrm{A} \subset \prod_{\iota \in \mathrm{I}} \mathrm{pr}_\iota \langle \mathrm{A} \rangle$。

我们经常使用记号$(x_\iota)_{\iota \in \mathrm{I}}$来表示$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$（§3, no. 6）中的元素。

若$\mathrm{I} = \emptyset$、集合$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$只有一个元素，即空集（§3, no. 4、例 1）。

¶ 如果乘积 $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ 中的所有因子 $\mathrm{X}_\iota$ 都等于相同的集合 E，则有 $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \mathrm{E}^{\mathrm{I}}$；这紧随定义而来。

¶ 如果 $(X_\iota)_{\iota \in I}$ 是集合的任意族并且如果 E 是集合使得

$$\bigcup_{\iota \in I} X_\iota \subset E,$$

那么定义 1 表明$\prod_{\iota \in I} X_\iota \subset E^I$；因此，在 $\prod_{\iota \in I} X_\iota$ 和集合之间存在一对一的对应，I 的映射进入 E（即 $\mathfrak{F}(I, E)$ 的子集）。

¶ 如果 $I = \{\alpha\}$ 是单个元素的集合由……组成，我们有

$$\prod_{\iota \in I} X_\iota = X_\alpha^{\{\alpha\}};$$

映射 $F \to F(\alpha)$ 就是$\prod_{\iota \in \{\alpha\}} X_\iota$ 的双射（称为*规范*）到$X_\alpha$。

¶ 设 A、B 为集合，并令 $\alpha$、$\beta$ 与对象不同（存在两个不同的对象，分别为例 $\emptyset$ 和 $\{\emptyset\}$）。考虑图 $\{(\alpha, A), (\beta, B)\}$，它显然是函数式的，并且正是$(X_\iota)_{\iota \in \{\alpha, \beta\}}$族，使得$X_\alpha = A$和$X_\beta = B$。对于每个对 $(x, y) \in A \times B$，令 $f_{x,y}$ 为函数图 $\{(\alpha, x), (\beta, y)\}$。显然函数$(x, y) \to f_{x,y}$是$A \times B$到$\prod_{\iota \in \{\alpha, \beta\}} X_\iota$的双射映射；这个双射的倒数是$g \to (g(\alpha), g(\beta))$。这两个双射被称为*规范*。接下来我们将使用这个一对一的对应从集族的积的属性推导出两个集合的积的属性。

¶ 设 $(X_\iota)_{\iota \in I}$ 为集合的族，每个族由一个元素组成，比如 $X_\iota = \{a_\iota\}$；那么乘积$\prod_{\iota \in I} X_\iota$就是单个元素$(a_\iota)_{\iota \in I}$的集合由……组成。

¶ 令 E 为集合。将 I 的*常数* 映射 $\iota \to x$ 转换为乘积 $E^I$ 的 E 形式子集 $\Delta$ 的图形，称为*对角的*。如果$\bar{x}$表示映射$\iota \to x$（其中$x \in E$）的图，则映射$x \to \bar{x}$是E在$\Delta$上的双射，称为*对角线映射*。

#### 命题 4 {#ens-ii-s5-prop-4 .statement tag=03IK}

*让*$(X_\iota)_{\iota \in I}$*成为集合的一个家庭，让你成为集合*K的双射*到指标集合*I。 *如果* U *是 u 的图，则映射* $F \to F \circ U$ *of* $\prod_{\iota \in I} X_\iota$ *进入* $\prod_{x \in K} X_{u(x)}$ *是双射的。*

让

$$A = \bigcup_{\iota \in I} X_\iota = \bigcup_{x \in K} X_{u(x)}$$

（§4，命题1）。 映射 $F\to F\circ U$ ($F\in A^I$) 是$A^I$ 的双射到$A^K$ (命题 2)。显然，条件“对于每个$\iota\in I$，$F(\iota)\in X_\iota$”相当于“对于每个$x\in K$，$(F\circ U)(x)\in X_{u(x)}$”，结果如下。

### 4.部分积

令$(X_\iota)_{\iota\in I}$为集合的家族，令$J$为$I$的子集。 乘积 $\displaystyle\prod_{\iota\in J}X_\iota$ 被称为 $\displaystyle\prod_{\iota\in I}X_\iota$ 的*部分乘积*。如果$f$是函数，其图$F$是$\displaystyle\prod_{\iota\in I}X_\iota$的成员，则$F\circ\Delta_J$（其中$\Delta_J$是$J\times J$的对角线）是$f$到$J$的*限制*的图。显然$F\circ\Delta_J\in\displaystyle\prod_{\iota\in J}X_\iota$； $\displaystyle\prod_{\iota\in I}X_\iota$的映射$F\to F\circ\Delta_J$到$\displaystyle\prod_{\iota\in J}X_\iota$称为指标*$J$的*投影，记为$\operatorname{pr}_J$。

#### 命题 5 {#ens-ii-s5-prop-5 .statement tag=03Q9}

*令$(X_\iota)_{\iota\in I}$为集合的家族，令$J$为$I$的子集。如果对于每个$\iota\in I$，我们有$X_\iota\ne\varnothing$，投影$\operatorname{pr}_J$是$\displaystyle\prod_{\iota\in I}X_\iota$的映射到$\displaystyle\prod_{\iota\in J}X_\iota$。*

鉴于上面的注，足以证明以下命题：

#### 命题 6 {#ens-ii-s5-prop-6 .statement tag=03QA}

*Let $(X_\iota)_{\iota\in I}$ be a family of sets such that $X_\iota\ne\varnothing$ for all $\iota\in I$. 如果$g$是$J\subset I$的映射到$A=\displaystyle\bigcup_{\iota\in I}X_\iota$，使得$g(\iota)\in X_\iota$对于所有$\iota\in J$，则存在$g$到$I$的扩张$f$，使得对于所有$f(\iota)\in X_\iota$ $\iota\in I$.*

对于每个$\iota\in I-J$，让$T_\iota$表示项$\tau_\iota(y\in X_\iota)$。从$X_\iota\ne\varnothing$到假设，我们为所有$\iota\in I-J$（章I, §4, no. 1）提供了$T_\iota\in X_\iota$。如果$G$是$g$的图，则图$G\cup\left(\displaystyle\bigcup_{\iota\in I-J}\{(\iota,T_\iota)\}\right)$是函数的图，它具有所需的属性，正如立即验证的那样。

#### 推论 1 {#ens-ii-s5-prop-6-cor-1 .statement tag=03QB}

*让$(X_\iota)_{\iota\in I}$成为集合的一个族，这样对于每个$\iota\in I$我们都有$X_\iota\ne\varnothing$。那么对于每个 $\alpha\in I$ 投影 $\operatorname{pr}_\alpha$ 都是 $\displaystyle\prod_{\iota\in I}X_\iota$ 的映射到 $X_\alpha$。*

$\operatorname{pr}_\alpha$是$X_\alpha^{\{\alpha\}}$典范映射合成到$X_\alpha$和映射$\operatorname{pr}_{\{\alpha\}}$的应用命题5到$I$和注子集$J=\{\alpha\}$。

#### 推论 2 {#ens-ii-s5-prop-6-cor-2 .statement tag=03QC}

*设$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是集合的一个家庭。那么$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \emptyset$当且仅当存在$\iota \in \mathrm{I}$使得$\mathrm{X}_\iota = \emptyset$。*

如果每个$\iota \in \mathrm{I}$都有$\mathrm{X}_\iota \neq \emptyset$，那么从推论1可以得出$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$；相反，如果 $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$、关系 $\mathrm{pr}_\alpha\Big(\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{X}_\alpha$ 则表明每个 $\alpha \in \mathrm{I}$ 都有 $\mathrm{X}_\alpha \neq \emptyset$。

因此，如果我们有一个非空集族$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$，我们可以引入（作为辅助常数）函数$f$，其域I使得$f(\iota) \in \mathrm{X}_\iota$适用于所有$\iota \in \mathrm{I}$。在实践中，有人说：“在每个$\mathrm{X}_\iota$中取元素$x_\iota$”。直观上，我们在每个集合$\mathrm{X}_\iota$中“选择”了元素$x_\iota$；控制其使用的逻辑符号$\tau$和判据的引入使我们无需制定“选择公理”来使运算合法化（cf.结果摘要，§4, no. 10）。

#### 推论 3 {#ens-ii-s5-prop-6-cor-3 .statement tag=03QD}

*令$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$和$(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$为集合的两个族，具有相同的指标集合I。如果每个$\iota \in \mathrm{I}$都有$\mathrm{X}_\iota \subset \mathrm{Y}_\iota$，那么*

$$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota.$$

*相反，如果$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod\limits_{\iota \in \mathrm{I}} \mathrm{Y}_\iota$，并且如果每个$\iota \in \mathrm{I}$有$\mathrm{X}_\iota \neq \emptyset$，则每个$\iota \in \mathrm{I}$有$\mathrm{X}_\iota \subset \mathrm{Y}_\iota$。*

第一个断言是显而易见的，第二个命题1，推论5，因为我们有，对于每个$\alpha \in \mathrm{I}$，

$$\mathrm{X}_\alpha = \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota\Big) = \mathrm{Y}_\alpha.$$

### 5. 结合性乘积集合

#### 命题 7 {#ens-ii-s5-prop-7 .statement tag=03IN}

*设$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是集合的一个家庭，其指标集合I不是空集。设$(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$为I的划分。然后映射*

$$f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$$

* $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ 到乘积集合 $\prod\limits_{\lambda \in \mathrm{L}} \Big(\prod\limits_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota\Big)$ 是双射（集合乘积的“结合性”）。*

将$\mathrm{pr}_{\mathrm{J}_\lambda} f$解释为函数的限制的图，其图为$f$(no. 4)，得出叙述映射$f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$是双射意味着，对于每个族$(v_\lambda)_{\lambda \in \mathrm{L}}$，其中$v_\lambda$是$\mathrm{J}_\lambda$的映射到$\bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$，存在I到$\bigcup_{\iota \in I} X_\iota$的唯一映射$u$，使得对于每个$\lambda \in L$，$v_\lambda$是$u$到$J_\lambda$的限制。但这是$(J_\lambda)_{\lambda \in L}$是I划分（§4，命题8）的假设推论。

¶ 双射在命题 7 中定义，并且它的逆双射被认为是*规范*。

*注*

#### 注 1 {#ens-ii-s5-n5-rem-1 .statement tag=03SA}

令$\alpha$、$\beta$为两个不同的对象，并令$(J_\lambda)_{\lambda \in \{\alpha, \beta\}}$为I的划分分成两个集合$J_\alpha$、$J_\beta$。因此，我们通过将$\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$的典范映射的合成形成到$\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$上并将$\prod_{\iota \in I} X_\iota$的典范映射形成到$\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$上，获得乘积$\prod_{\iota \in I} X_\iota$的一对一映射（再次称为*规范*） $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$。如果对于每个$\iota \in J_\beta$，$X_\iota$ 是*单个元素* 的集合由……组成，则$\mathrm{pr}_{J_\alpha}$ 是$\prod_{\iota \in I} X_\iota$ 到$\prod_{\iota \in J_\alpha} X_\iota$ 的双射映射。

#### 注 2 {#ens-ii-s5-n5-rem-2 .statement tag=03SB}

令$\alpha$、$\beta$、$\gamma$为三个对象，其中没有两个相等（存在三个这样的对象；对于例、$\emptyset$、$\{\emptyset\}$、$\{\{\emptyset\}\}$），并令A、B、C为集合。考虑函数图$\{(\alpha, A), (\beta, B), (\gamma, C)\}$，即集合$(X_\iota)_{\iota \in \{\alpha, \beta, \gamma\}}$族，使得$X_\alpha = A$、$X_\beta = B$、$X_\gamma = C$。对于由两个集合、$\{\alpha, \beta\}$和$\{\gamma\}$形成的$\{\alpha, \beta, \gamma\}$的划分，存在对应一个$\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$的规范双射到乘积

$$\left( \prod_{\iota \in \{\alpha, \beta\}} X_\iota \right) \times X_\gamma^{\{\gamma\}},$$

因而，$\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$的双射（再次称为*规范*）到$A \times B \times C$（§ 2, no. 2），其中变换每个图$f \in \prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$到$A \times B \times C$的元素$(f(\alpha), f(\beta), f(\gamma))$。因而，到命题 4，我们可以将六个集合、$A \times B \times C$、$B \times C \times A$、$C \times A \times B$、$B \times A \times C$、$A \times C \times B$、$C \times B \times A$中的任意两个一对一地放在对应中。

### 6.分配律公式

#### 命题 8 {#ens-ii-s5-prop-8 .statement tag=03IO}

*让*$((X_{\lambda,\iota})_{\iota \in J_\lambda})_{\lambda \in L}$*成为集合家庭的一个家庭（与指标集合*L*）。假设* $L \neq \emptyset$ *和* $J_\lambda \neq \emptyset$ *对于每个* $\lambda \in L$。 *让*

$$I = \prod_{\lambda \in L} J_\lambda \neq \emptyset.$$

*然后我们有*

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right),$$
$$\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcup_{f \in I} \left( \bigcap_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$$

（并超过交的“分配律”，以及交超过并的“分配律”）。

令$x$为$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right)$中的元素，并令$f$为I中的任意元素。存在指标$\lambda$使得$x \in \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$；因而 $x \in X_{\lambda, f(\lambda)}$ 因而

$$x \in \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}.$$

由于这对于每个 $f \in I$ 都是正确的，所以我们有

$$x \in \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

相反，令 $x$ 为不属于到集合的对象

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right).$$

那么对于每个$\lambda \in L$，我们有$x \notin \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$，这意味着指标$\iota \in J_\lambda$的集合$J'_\lambda$，使得$x \notin X_{\lambda, \iota}$对于每个$\lambda \in L$不为空。根据推论 2 命题 5，存在一个具有域 L 的函数图$f$，这样对于每个$\lambda \in L$，我们都有$f(\lambda) \in J'_\lambda$。因而，每个$\lambda \in L$对应$f \in I$和$x \notin X_{\lambda, f(\lambda)}$；因而

$$x \notin \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$$

因而

$$x \notin \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

这样就完成了第一个公式的证明。第二个公式后面是应用，第一个$((\complement_A X_{\lambda, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$，其中 A 表示并 $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\lambda \right)$。

#### 推论 {#ens-ii-s5-n6-cor-1 .statement tag=03IP}

*设* $(X_\iota)_{\iota \in I}$ *和* $(Y_\varkappa)_{\varkappa \in K}$ *为集合的两个族，其中非空指标集合* I，K。*然后*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \cup \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cup Y_\varkappa),$$
$$\left( \bigcup_{\iota \in I} X_\iota \right) \cap \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cap Y_\varkappa).$$

令$\alpha$、$\beta$为两个不同的对象；将命题 8 中的公式（以及 $L = \{\alpha,\ \beta\}$、$J_\alpha = I$、$J_\beta = K$）应用于家庭 $((Z_{\lambda,\, \mu})_{\mu \in J_\lambda})_{\lambda \in L}$，其中 $Z_{\alpha,\, \iota} = X_\iota$ 应用于所有 $\iota \in I$，$Z_{\beta,\, \varkappa} = Y_\varkappa$ 应用于每个 $\varkappa \in K$。通过$\coprod_{\lambda \in L} J_\lambda$的规范双射到$I \times K$（no. 3）的存在以及通过§ 4的命题1，我们得到了公式。

#### 命题 9 {#ens-ii-s5-prop-9 .statement tag=03IQ}

*让*$((X_{\lambda,\, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$*成为一个家庭（与指标集合*L）*集合的家庭。让*$I = \prod_{\lambda \in L} J_\lambda$。 *然后*

$$\prod_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

*和（如果* $L \neq \emptyset$ *和* $J_\lambda \neq \emptyset$ *对于每个* $\lambda \in L$）

$$\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcap_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

（乘积的“分配律”超过并和超过交）。
如果 $L = \emptyset$ 或对于某些 $\lambda \in L$ $J_\lambda = \emptyset$，则第一个公式平凡为真。如果不是，则令$g$为$\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right)$的元素。对于每个$\lambda \in L$，存在指标$\iota \in J_\lambda$，使得$g(\lambda) \in X_{\lambda,\, \iota}$；在指标 $\iota \in J_\lambda$ 的其他字、集合 $H_\lambda$ 中，$g(\lambda) \in X_{\lambda,\, \iota}$ 不为空。根据推论 2 到命题 5，因此存在一个具有域 L 的函数图 $f$，使得

$$f(\lambda) \in H_\lambda$$

对于每个$\lambda \in L$，即$g(\lambda) \in X_{\lambda,\, f(\lambda)}$。因此我们有$g \in \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)}$，因此有$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$。相反，如果

$$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right),$$

有一个函数图$f \in I$，对于每个$\lambda \in L$，我们有

$$g(\lambda) \in X_{\lambda,\, f(\lambda)}$$

以及，*更不必说*，$g(\lambda) \in \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$。这样就完成了第一个公式的证明。第二个公式的证明类似，但更简单，我们把它留给读者。

#### 推论 1 {#ens-ii-s5-prop-9-cor-1 .statement tag=03QE}

*假设*$L \neq \emptyset$*和*$J_\lambda \neq \emptyset$*对于每个*$\lambda \in L$。 *如果对于每个索引* $\lambda \in L$ *族* $(X_{\lambda, \iota})_{\iota \in J_\lambda}$ *是* $X_\lambda = \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$的划分，*那么家庭* $\left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)_{f \in I}$ *是* $\prod_{\lambda \in L} X_\lambda$的划分。

如果我们集合

$$\mathrm{P}_f = \prod_{\lambda \in L} X_{\lambda, f(\lambda)},$$

那么，凭借命题 9 的第一个公式，足以证明对于所有$f \in I$，$\mathrm{P}_f \neq \emptyset$ 以及当$f$ 和$g$ 与I 不同的元素时，$\mathrm{P}_f \cap \mathrm{P}_g = \emptyset$ 就足够了。第一个点由命题5推论2。至于第二个，如果$f \neq g$，则存在$\lambda \in L$使得

$$f(\lambda) \neq g(\lambda)$$

因此，凭借假设，$X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$。由此可见，不存在属于到$\mathrm{P}_f \cap \mathrm{P}_g$的图；因为如果 G 是这样一个图，我们就会有 $\mathrm{G}(\lambda) \in X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$，这是荒谬的。

#### 推论 2 {#ens-ii-s5-prop-9-cor-2 .statement tag=03QF}

*设*$(X_\iota)_{\iota \in I}$*和*$(Y_\varkappa)_{\varkappa \in K}$*为集合的两个族。然后*

$$\left( \bigcup_{\iota \in I} X_\iota \right) \times \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa)$$

*并且，如果* I *和* K *非空，*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \times \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa).$$

证明遵循命题 8 推论的证明模式。

#### 命题 10 {#ens-ii-s5-prop-10 .statement tag=03QG}

*设*$(X_{\iota, \varkappa})_{(\iota, \varkappa) \in I \times K}$*是集合的一个家庭，其指标集合是两个集合的积*I*和*K。*如果*$K \neq \emptyset$，*我们有*

$$\bigcap_{\varkappa \in K} \left( \prod_{\iota \in I} X_{\iota, \varkappa} \right) = \prod_{\iota \in I} \left( \bigcap_{K \in \varkappa} X_{\iota, \varkappa} \right).$$

待证明的等式两边都是函数图。图$f$属于位于左侧当且仅当对于每个$\varkappa \in K$，$f \in \prod_{\iota \in I} X_{\iota, \varkappa}$；也就是说，当且仅当 $f(\iota) \in X_{\iota, \varkappa}$ 对于所有$(\iota, \varkappa) \in I \times K$。对于右侧的$f$到属于，每个$\iota \in I$有$f(\iota) \in \bigcap_{\varkappa \in K} X_{\iota, \varkappa}$是必要且充分的，即每个对$(\iota, \varkappa) \in I \times K$有$f(\iota) \in X_{\iota, \varkappa}$。这样就完成了证明。

#### 推论{#ens-ii-s5-n6-cor-2 .statement tag=03IR}

*设*$(X_\iota)_{\iota \in I}$*和*$(Y_\iota)_{\iota \in I}$*为集合的两个族，具有相同的指标集合*$I \neq \emptyset$。 *然后*

$$\Big(\prod_{\iota \in I} X_\iota\Big) \cap \Big(\prod_{\iota \in I} Y_\iota\Big) = \prod_{\iota \in I} (X_\iota \cap Y_\iota),$$
$$\Big(\bigcap_{\iota \in I} X_\iota\Big) \times \Big(\bigcap_{\iota \in I} Y_\iota\Big) = \bigcap_{\iota \in I} (X_\iota \times Y_\iota).$$

应用命题 10 到 K（分别为 I）是两个不同元素的集合由……组成的情况。

### 7. 扩张的映射到乘积

#### 定义 2 {#ens-ii-s5-def-2 .statement tag=03IS}

*设* $(X_\iota)_{\iota \in I}$，$(Y_\iota)_{\iota \in I}$ *为集合的两个族，并让*$(g_\iota)_{\iota \in I}$ *为函数的族，且具有相同的指标集合*I*使得*$g_\iota$*为映射* $X_\iota$ *进入* $Y_\iota$ *每个* $\iota \in I$。 *对于每个* $f \in \prod_{\iota \in I} X_\iota$ *让* $u_f$ *成为函数* $\iota = g_\iota(f(\iota))$ $(\iota \in I)$的图，*这是* $\prod_{\iota \in I} Y_\iota$的元素。 *映射* $f \to u_f$ *of* $\prod_{\iota \in I} X_\iota$ *进入* $\prod_{\iota \in I} Y_\iota$ *被称为映射* $(g_\iota)_{\iota \in I}$家族的规范扩张*（或简称*扩张*）*至乘积； *it is also sometimes called the product of the family of mappings* $(g_\iota)_{\iota \in I}$.

当使用指标记号时，$(g_\iota)_{\iota \in I}$族的乘积为函数$(x_\iota)_{\iota \in I} \to (g_\iota(x_\iota))_{\iota \in I}$；它是有时，用$(g_\iota)_{\iota \in I}$表示。

如果$I = \{\alpha, \beta\}$，其中$\alpha$和$\beta$不同，映射$(g_\iota)_{\iota \in I}$族的扩张到乘积就是$\psi \circ (g_\alpha \times g_\beta) \circ \varphi$，其中$\varphi$表示$\prod_{\iota \in I} X_\iota$的典范映射到$X_\alpha \times X_\beta$ (no. 3) 和 $\psi$ 典范映射的 $Y_\alpha \times Y_\beta$ 到 $\prod_{\iota \in I} Y_\iota$。

#### 命题 11 {#ens-ii-s5-prop-11 .statement tag=03IT}

*设*$(X_\iota)_{\iota \in I}$、$(Y_\iota)_{\iota \in I}$、$(Z_\iota)_{\iota \in I}$*为集合的三个族，让*$(g_\iota)_{\iota \in I}$、$(g'_\iota)_{\iota \in I}$*为函数的两个族，都具有相同的指标集合，使得*$g_\iota$*为映射*$X_\iota$*进入*$Y_\iota$*和*$g'_\iota$*映射*$Y_\iota$*进入*$Z_\iota$，*对于每个*$\iota \in I$。 *让*$g$*和*$g'$*成为家庭中的扩张*$(g_\iota)_{\iota \in I}$*和*$(g'_\iota)_{\iota \in I}$*到乘积。那么家庭的扩张*$(g'_\iota \circ g_\iota)_{\iota \in I}$*到乘积就等于*$g' \circ g$。

这紧随定义 2。

#### 推论{#ens-ii-s5-n7-cor-1 .statement tag=03IU}

令$(X_i)_{i\in I}$、$(Y_i)_{i\in I}$为集合的两个族，并令$(g_i)_{i\in I}$为函数的族。如果$g_i$是$X_i$到$Y_i$的单射（或满射），对于每个$i\in I$，则$(g_i)_{i\in I}$到乘积的扩张$g$是单射（或单射）。 $\displaystyle\prod_{i\in I}X_i$到$\displaystyle\prod_{i\in I}Y_i$的满射）。

(1) 假设每个$i\in I$有$X_i\ne\varnothing$；否则结果是微不足道的。假设$g_i$对于每个$i\in I$都是单射的，并让$r_i$是$g_i$的缩进（§ 3, no. 8，定义11），因此$r_i\circ g_i$是$X_i$的恒等映射。设$r$为家庭$(r_i)_{i\in I}$的扩张到乘积；由于$r\circ g$是恒等映射$I_{X_i}$族的扩张到乘积，$r\circ g$是$\displaystyle\prod_{i\in I}X_i$的恒等映射，因此$g$是单射的（§ 3，命题） 8).

(2) 假设$g_i$是每个$i\in I$的$X_i$到$Y_i$的满射，并令$s_i$为$g_i$的截面 (§ 3, no. 8, 定义 11)，因此$g_i\circ s_i$ 是 $Y_i$ 中的恒等映射。如果$s$是$(s_i)_{i\in I}$族的扩张到乘积，则$g\circ s$是恒等映射$I_{Y_i}$族的扩张到乘积，因此是恒等映射 $\displaystyle\prod_{i\in I}Y_i$；因此 $g$ 是满射 (§ 3, 命题 8)。

令$(X_i)_{i\in I}$为集合的家族，令$E$为集合。对于$E$到$\displaystyle\prod_{i\in I}X_i$的每个映射$f$，$\operatorname{pr}_i\circ f$就是$E$到$X_i$的映射。如果$\bar f$是映射族的扩张到乘积，并且如果$d$是$E$到$E^I$的对角线映射，那么$f=\bar f\circ d$就是直接的。相反，令$(f_i)_{i\in I}$为函数的族，使得对于每个$i\in I$，$f_i$为$E$到$X_i$的映射，并令$\bar f$为该族的扩张至乘积；那么每个$i\in I$就有$\operatorname{pr}_i\circ(\bar f\circ d)=f_i$。由于语言滥用，映射$\bar f\circ d$也写成$(f_i)_{i\in I}$。这样我们就将定义一对一的映射的集合 $\displaystyle\prod_{i\in I}X_i^E$ 映射到集合 $\displaystyle\left(\prod_{i\in I}X_i\right)^E$；这个映射及其逆被认为是规范的。

### 习题 {#ens-ii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
