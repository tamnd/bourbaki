---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 6
section_title: Topological groups with operators; topological rings division rings and fields
lang: zh
source: top-i-iv
book_pages: 271-283, 315-324
pdf_pages: 0277-0289, 0321-0330
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS WITH OPERATORS
      page: 271
      pdf_page: 277
    - "no": 2
      title: TOPOLOGICAL DIRECT SUM OF STABLE SUBGROUPS
      page: 272
      pdf_page: 278
    - "no": 3
      title: TOPOLOGICAL RINGS
      page: 274
      pdf_page: 280
    - "no": 4
      title: SUBRINGS; IDEALS; QUOTIENT RINGS; PRODUCTS OF RINGS
      page: 276
      pdf_page: 282
    - "no": 5
      title: COMPLETION OF A TOPOLOGICAL RING
      page: 276
      pdf_page: 282
    - "no": 6
      title: TOPOLOGICAL MODULES
      page: 278
      pdf_page: 284
    - "no": 7
      title: TOPOLOGICAL DIVISION RINGS AND FIELDS
      page: 281
      pdf_page: 287
    - "no": 8
      title: UNIFORMITIES ON A TOPOLOGICAL DIVISION RING
      page: 282
      pdf_page: 288
statements: 24
exercises: 26
content_sha256: 83929d8e64618654cc95db059dc24ad3d15976f2110d33813fa7e991a53c587b
translated_from: content/en/top/III/06_s6_topological_groups_with_operators.md
translation_method: google
source_content_sha256: bbc4c9265a358c8a03dba09dd6f583c1d3176c59f530f843e58111b9bb22ab18
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: bb37d5c7d7520c98bcc96ac53b572266e9590c01de02226fa0194c60f54a65ec
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 6. 拓扑群与运算符；拓扑环，划分环和域

### 1. 拓扑群与运算符

在集合 $G$ 上，如果 $G$ 的拓扑和群结构兼容 (§ 1, no. 1) 并且在加法自同态中，则群的结构与运算符和拓扑被认为是兼容的操作员产生的$G$是连续的。 集合 $G$，连同给定的群的拓扑和结构（带有运算符），则被称为带有运算符的拓扑群。

如果 $H$ 是具有算子的拓扑群 $G$ 的稳定子群，则 $G$ 的拓扑在 $H$ 上诱导的拓扑与群的结构兼容，且算子在$H$。此外：

#### 命题 1 {#top-iii-s6-prop-1 .statement tag=0BN2}

*如果$H$是带有运算符的拓扑群$G$的稳定子群，则$G$中$H$的闭包$\overline{H}$是$G$的稳定子群。*

我们已经知道（§ 2, no. 1，命题 1）$\overline{H}$是$G$的子群。另外，如果$\alpha$是$G$上的任意运算符，则连续映射$x \to x^\alpha$下的$H$的像包含在$H$中，因此$\overline{H}$的像包含在$\overline{H}$中（章I, § 2, no. 1，定理1）。

令 $H$ 为具有算子的拓扑群 $G$ 的稳定法线子群。那么对于$G$上的每个算子$\alpha$，由$x \to x^\alpha$诱导的$G/H$的映射是连续的（§ 2, no. 8，注3），并且群的结构与$G/H$上的算子因此与$G/H$上的商拓扑兼容。

令$(G_i)_{i \in I}$为具有运算符的拓扑群族，其中每个$G_i$被假定具有相同的运算符集合$\Omega$。对于每个$\alpha \in \Omega$，$G = \prod_{i \in I} G_i$的映射$x \to ((\mathrm{pr}_i x)^\alpha)$自身是连续的（章I, § 4, no. 1，命题1），并且群的结构与$G$上的运算符兼容乘积拓扑于$G$。

如果 $G$ 是带有运算符的 Hausdorff 拓扑群，并且 $G$ 具有完成$\hat{G}$ (§ 3, no. 4)，则由 $G$ 上的运算符定义的 $G$ 的每个自同态 $x \to x^\alpha$ 可以通过连续性扩展为自同态共 $\hat{G}$（§ 3, no. 3、命题 5）。因此，$\hat{G}$具有带有运算符的拓扑群的结构，并且运算符集合对于$\hat{G}$和$G$是相同的。

### 2. 稳定子群的拓扑直和

由于研究带有运算符的交换性群等同于研究模，因此我们应该有时允许自己使用适合于模的术语来实现任意带有运算符的交换性群；因此，我们可以使用*线性映射*来代替带有运算符的交换性群的同态，并且我们可以使用字*投影算子*来表示带有运算符的交换性群的幂等自同态。

如果带有运算符（加法编写）的交换拓扑群 $E$ 是稳定子群的*有限*族 $(M_i)_{1 \leq i \leq n}$ 的直和，则乘积的规范双射 $(x_i) \to \sum_{i=1}^n x_i$ 群$\prod_{i=1}^n M_i$到$E$是*连续的*，但*不一定是同胚*。

#### 定义 1 {#top-iii-s6-def-1 .statement tag=0BN3}

*令$E$为带有运算符的交换拓扑群，并令$(M_i)_{1 \leq i \leq n}$为$E$的稳定子群的有限族，使得$E$是$M_i$的直和。那么 $E$ 被称为 $M_i$ 的拓扑直和，如果乘积群 $\prod_{i=1}^n M_i$ 到 $E$ 的典范映射 $(x_i) \to \sum_{i=1}^n x_i$ 是同胚*（因此拓扑的同构群与运算符）。

#### 命题 2 {#top-iii-s6-prop-2 .statement tag=0BN4}

*令 $E$ 为具有算子的交换拓扑群，其为稳定子群 $M_i$ ($1 \leq i \leq n$) 的直和。令$(p_i)_{1 \leq i \leq n}$为与分解$E = \sum_{i=1}^n M_i$相关的投影算子族。那么$E$是$M_i$的拓扑直和当且仅当$p_i$是连续的。*

对于映射$x \to (p_i(x))$是映射$(x_i) \to \sum_{i=1}^n x_i$的倒数。

由于$1 = \sum_{i=1}^n P_i$（其中$1$表示$E$的恒等映射），投影算子$p_i$中的$n - 1$在阶中连续就足够了，因此$n$也应该是连续的。

如果$E$是两个稳定子群$M, N$的拓扑直和，则$N$被称为$E$中$M$的“拓扑补”；当且仅当 $E/M$ 的典范映射是具有运算符的拓扑群的 *同构* 时，才是这种情况。

#### 推论{#top-iii-s6-n2-cor-1 .statement tag=0BN5}

*令$E$为带有算子的交换拓扑群，并令$M$为$E$的稳定子群。那么下面的条件是等价的：*

a) $M$ 在 $E$ 中有一个拓扑补集。

b) *在 $E$ 中存在连续的投影算子 $p$ $E$，使得 $p(E) = M$。*

c) *$M$的恒等映射可以扩展到$E$的连续线性映射到$M$。*

由命题 2 可知，a) 蕴涵 b)，并且显然 b) 蕴含 c)。最后，如果$p$是$E$的连续线性映射到$M$，其中$M$的扩展恒等映射，则$p$是连续的投影算子，并且投影算子$p$和$1 - p$ 与直和分解 $E = M + N$ 相关联，其中$N = \overline{p}(0)$。

#### 注 1 {#top-iii-s6-n2-rem-1 .statement tag=0BN6}

为了避免混淆，我们将有时说，$E$的稳定子群是$M$的补集（在带有运算符的群的结构的意义上，没有拓扑）是$M$的*代数补集*。

#### 注 2 {#top-iii-s6-n2-rem-2 .statement tag=0BN7}

如果带有运算符的*Hausdorff*交换拓扑群是稳定子群族$(M_i)_{1 \leq i \leq n}$的拓扑直和，则每个子群$M_i$在$E$中*闭*，因为$M_i$是所有集合 $x \in E$使得$p_i(x) = x$（章I, § 8, no. 1，命题2）。

#### 命题 3 {#top-iii-s6-prop-3 .statement tag=0BN8}

*令$E, F$为两个带算子的可交换拓扑群，并令$u$为$E$到$F$的连续线性映射。在阶中，应该存在$F$到$E$的连续线性映射$v$，使得$u \circ v$是$F$的恒等映射（在这种情况下，$u$被认为是右可逆的，$v$是据说是$u$的*右逆*）$u$是$E$到$F$的严格态射（§ 2, no. 8）并且$\overline{u}(0)$在$E$中有一个拓扑补集是必要且充分的。*

条件是*必要的*。因为我们有 $u(v(F)) = F$ 和 *更不必说* $u(E) = F$；此外，如果$p = v \circ u$，则$p$是$E$自身的连续线性映射，使得$p^2 = p$；因此（命题 2 的推论）$p(E) = v(u(E)) = v(F)$ 在 $E$ 中具有拓扑补集 $\overline{p}(0)$；但从$u(p(x))) = u(x)$到假设，我们有$\overline{u}(0) = \overline{p}(0)$。最后，$E/\overline{u}(0)$到$F$的双射映射，与$u$相关，是$E/\overline{u}(0)$到$v(F)$的双射映射的合成，与$p$相关，以及限制 $u$至$v(F)$；由于$v$是连续的，所以这些映射都是同构，因此$u$是$E$到$F$的严格态射。

条件*足够*。因为如果$\varphi$是E到$E/\overline{u}^1(o)$上的典范同态，那么说$\overline{u}^1(o)$在E中具有拓扑补M就是说$\varphi$到M的限制是M到$E/\overline{u}^1(o)$上的同构。另一方面，由于$u = w \circ \varphi$，其中w是$E/\overline{u}^1(o)$到F的同构，我们看到u到M的限制是M到F的同构，因此逆同构v使得$u \circ v$是F到其自身的恒等映射。

#### 命题 4 {#top-iii-s6-prop-4 .statement tag=0BN9}

*设E，F是两个带有运算符的交换拓扑群，并设u是E到F的连续线性映射。在阶中，应该存在F到E的连续线性映射v，使得$v \circ u$是E到其自身的恒等映射*（在这种情况下，u被称为*左）可逆*且 v 被认为是 u 的*左逆*）*u 是 E 到 u(E) 上的（拓扑）同构是必要且充分的，并且 u(E) 在 F 中有一个拓扑补。*

条件是“足够的”，因为如果它们满足，我们可以通过将 u(E) 的同构的合成取到作为 u 的逆的 E 上，并将 F 的连续投影算子取到 u(E) 上，从而获得 u 的左逆 v。

条件是*必要的*。对于关系$v(u(x)) = x$显示$\overline{u}^1(o) = \{ o \}$；因此，u 是 E 到 u(E) 上的双射，并且由于 v 到 u(E) 的限制是连续的，因此 u 是 E 到 u(E) 上的同构。另一方面，如果我们将$q = u \circ v$，则q是F的连续线性映射到u(E)上，使得$q^2 = q$，这证明（命题2的推论）u(E)在F中具有拓扑补集。

### 3. 拓扑环

#### 定义 2 {#top-iii-s6-def-2 .statement tag=0BNA}

*拓扑环是集合A，它携带环结构和拓扑满足以下公理：*

*（AT$_\mathrm{I}$）*。 *映射* $(x, y) \to x + y$ *的* $A \times A$ *到* A *是连续的。*
*（AT$_\mathrm{II}$）*。 *映射* $x \to -x$ *从* A *到* A *是连续的。*
*（AT$_\mathrm{III}$）*。 *映射* $(x, y) \to xy$ *的* $A \times A$ *到* A *是连续的。*

前两个公理表示 A 的拓扑与其 *加法群* 结构 (§ 1, no. 1) 相容的。

如果在集合 A 上给出环结构和拓扑，则如果它们满足公理 (AT$_\mathrm{I}$)、(AT$_\mathrm{II}$) 和 (AT$_\mathrm{III}$)，则称它们是“相容的”的。

#### 例 1 {#top-iii-s6-n3-exa-1 .statement tag=0BNB}

在任何环 A 上，*离散* 拓扑与环结构兼容。 拓扑是离散的拓扑环称为*离散* 环。

#### 例 2 {#top-iii-s6-n3-exa-2 .statement tag=0BNC}

我们将在章IV中看到，有理线Q（或实直线R）的拓扑与Q（或R）的环结构兼容。*

在拓扑环中，每个左位似$x \to ax$（或每个右位似$x \to xa$）都是连续的（如果$a$是$A$的单位，则为同胚）。

因为我们可以写相同的
$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0)
$$
公理 (AT_{III}) [鉴于 (AT_I) 和 (AT_{II})] 等价于以下两个公理的合取：
（AT_{IIIa}）。 *给定任何* $x_0 \in A$、*映射* $x \to x_0 x$ *和* $x \to xx_0$ *在点* $x = 0$ 连续。
（AT_{IIIb}）。 *映射* $(x, y) \to xy$ *从* $A \times A$ *进入* $A$ *在点* $(0, 0)$ 处连续。

由此我们可以推导出条件的充要集合，其中环$A$中的$0$的邻域的滤波器$\mathfrak{B}$必须在阶到定义中满足 $A$上的拓扑与其环结构兼容：$\mathfrak{B}$必须满足公理(GA_I)和§ 1的(GA_{II})，以及以下两个公理：
(AV_I)。 *对于所有* $x_0 \in A$ *和所有* $V \in \mathfrak{B}$，*存在* $W \in \mathfrak{B}$ *这样* $x_0 W \subset V$ *和* $W x_0 \subset V$。
（AV_{II}）。 *对于所有*$V \in \mathfrak{B}$，*存在*$W \in \mathfrak{B}$*使得*$WW \subset V$。

#### 注 {#top-iii-s6-n3-rem-1 .statement tag=0BND}

在数学分析中，人们经常遇到环，其中满足公理 (AT_I)、(AT_{II}) 和 (AT_{III a})，但不满足 (AT_{III b})。 *例是紧凑群上的环度量，其中乘法是卷积，拓扑是模糊拓扑。*

*例 3).* 设$\mathfrak{B}$为*双边理想*的环$A$、由……组成上的过滤器基。 $\mathfrak{B}$是拓扑的$0$的邻域的基本系统与$A$的加法群结构兼容，并且立即从(AV_I)和(AV_{II})得出这个拓扑与 $A$ 的 *环* 结构兼容。

令$X$为拓扑空间，并令$f$和$g$为$X$的两个映射为拓扑环$A$。如果$f$和$g$在点$x_0 \in X$连续，那么$f + g$、$-f$和$fg$在这个点连续。由此可见，$X$的连续映射进入$A$形式，$X$的所有映射进入$A$的环$A^X$的*子环*。我们还看到，如果$A$是*可交换的*，那么每个*n个变量*中的多项式，其系数在$A$中并在$A^n$上定义，在$A^n$上是*连续的*。再次，让$f$和$g$是集合$X$的两个映射，通过过滤器$\mathfrak{F}$*过滤*，变成*Hausdorff*拓扑环$A$；如果$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$存在，那么$\lim_{\mathfrak{F}} (f + g)$，$\lim_{\mathfrak{F}} (-f)$和$\lim_{\mathfrak{F}} (fg)$也存在，并且我们有（章I, § 7, no. 4，命题9，推论1，以及§ 8, no. 1，命题 1）

(1) $$ \lim_{\mathfrak{F}} (f + g) = \lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g, $$
(2) $$ \lim_{\mathfrak{F}} (-f) = -\lim_{\mathfrak{F}} f, $$
(3) $$ \lim_{\mathfrak{F}} (fg) = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g). $$

### 4. 子环；理想； 商环； 乘积 / 环

如果$H$是拓扑环$A$的子环，则$A$在$H$上诱导的拓扑与$H$的环结构兼容。由此在 $H$ 上定义的拓扑环结构据说是由 $A$ 的拓扑“诱导”的。

#### 命题 5 {#top-iii-s6-prop-5 .statement tag=0BNE}

*设$H$为拓扑环$A$的稠密子环，并令$K$为$H$的子环（分别为左理想、右理想、两侧理想）。那么$A$中$K$的闭包$\overline{K}$就是$A$的子环（分别为左理想、右理想、两侧理想）。*

证明与 § 2 中的命题 8 相同，n。 3：如果例$K$是$H$上的左理想，则映射$(z, x) \to zx$在$A \times A$和映射$H \times K$上连续到$K$；因此它映射$A \times K = \overline{H} \times K$变成$\overline{H}$。

令 $H$ 为拓扑环 $A$ 中的*双面*理想。通过与商群相同的论证，我们看到$A$的拓扑除以关系$x - y \in H$的*商*与$A/H$的环结构兼容。特别是，如果$A$不是豪斯多夫，那么$A$中$\{0\}$的闭包$N$是一个*封闭的双边理想*，通过命题5； 商环，即 Hausdorff ($\S$ 2, no. 5, 命题 13) 称为与* $A$ 伴随的 *Hausdorff 环。

设$(A_i)_{i \in I}$是拓扑环的族。在集合$A = \prod_{i \in I} A_i$上，$A_i$拓扑的*乘积*与$A_i$的环结构的乘积兼容（证明与乘积群相同）；这样定义的拓扑环$A$称为拓扑环$A_i$的*乘积*。

### 5. 完成拓扑环

当我们谈到拓扑环的*均匀性时，我们总是指其*加法群*、除非的均匀性；相反，我们明确指出；特别是，如果 $A$ 的加法群是完整的，则 $A$ 被称为“完整”环。

令 $A$ 为 *Hausdorff* 拓扑环；因为加法群 $A$ 可以被视为*完整 Hausdorff 交换* 群 $\hat{A}$ 的稠密子群，其最大确定为同构 ($\S$ 3, no. 5, 定理 2)。在阶中，我们应该能够将$A$视为*完整的环*的*子环*，有必要能够通过连续到空间$\hat{A} \times \hat{A}$来实现扩展函数$xy$。这个扩张的可能性将由以下更一般的定理得出：

#### 定理 1 {#top-iii-s6-thm-1 .statement tag=0BNF}

设E、F、G为三个完全Hausdorff交换律群；设 A 为 E 的稠密子群，设 B 为 F 的稠密子群。如果 f 是 $A \times B$ 的 $\mathbf{Z}$ 连续 $\mathbf{Z}$ 双线性 (*) 映射到 G，则 f 可以通过连续性扩展到连续 $\mathbf{Z}$ 双线性将$E \times F$的映射转化为G。

令$(x_0, y_0)$为$E \times F$的任意点，令$\mathfrak{U}, \mathfrak{B}$分别为$x_0, y_0$的邻域滤波器在A、B上的迹（$\mathfrak{U}, \mathfrak{B}$是滤波器，通过假设）。为了证明 f 可以通过连续性扩展，只需证明 $f(\mathfrak{U} \times \mathfrak{B})$ 是基于 G 的柯西滤波器（章 II, § 3, no. 6，命题 11）。考虑身份

$$
f(x', y') - f(x, y) = f(x' - x, y_1) + f(x_1, y' - y) + f(x' - x, y' - y_1).
$$

我们将证明，通过在$\mathfrak{U} \times \mathfrak{B}$足够小的集合中取$(x, y)$和$(x', y')$，并适当选择$x_1$和$y_1$，我们可以使右侧的每个项变得非常小。设W为G中0的任意邻域；由于 f 在 $(0, 0) \in A \times B$ 处连续，因此存在集合 $U \in \mathfrak{B}$ 和集合 $V \in \mathfrak{B}$，使得只要 $x \in U, x' \in U, y \in V, y' \in V$ 就有 $f(x' - x, y' - y) \in W$。取点$x_1 \in U$和点$y_1 \in V$；那么对于 U 中的所有 $x, x'$ 和 V 中的所有 $y, y'$，我们将有

$$
f(x' - x, y' - y_1) + f(x - x_1, y' - y) \in W + W.
$$

另一方面，部分映射$x \to f(x, y_1)$在A上连续；因而，有集合$U' \subset U$，属于到$\mathfrak{U}$，这样，每当$x$和$x'$属于到$U'$，我们就有$f(x' - x, y_1) \in W$。同样，存在$V' \subset V$属于到$\mathfrak{B}$，这样，只要$y$和$y'$属于到$V'$，我们就有$f(x_1, y' - y) \in W$。因而，如果$(x, y)$和$(x', y')$是$U' \times V'$中的任意两个点，那么

$$
f(x', y') - f(x, y) \in W + W + W + W;
$$

这就证明了f的扩张$\overline{f}$的存在性。 $\overline{f}$是$\mathbf{Z}$双线性的事实是恒等式扩张原理直接的推论（章I, § 8, no. 1，推论1到命题2）。

Q.E.D.

将此定理应用于豪斯多夫拓扑环 A，我们取E、F和G为$\hat{A}$，A和B为环 A，f为

(*) $f$ 被称为 $\mathbf{Z}$ 双线性，如果对于 A 的所有元素 $x, x'$ 和所有元素 $y, y' \in B$ 我们有

$$
f(x + x', y) = f(x, y) + f(x', y)
$$
和
$$
f(x, y + y') = f(x, y) + f(x, y').
$$

$\mathbf{Z}$双线性映射$(x, y) \to xy$，到假设是连续的。我们再次用$\hat{A} \times \hat{A}$上扩展的函数的$xy$值表示；这个函数是$\hat{A}$上合成的律，说它是$\mathbf{Z}$双线性意味着它相对于加法在两边都是可分配的；而且它也是*关联的*，由原理或扩张的恒等式组成。因而：

#### 命题 6 {#top-iii-s6-prop-6 .statement tag=0BNG}

*Hausdorff 拓扑环* $A$ *同构于完整 Hausdorff 环* $\hat{A}$ 的稠密子环，*确定到同构*（称为 $A$ 的*完备的*）。

如果$A$是*可交换的*（分别*具有单位元素*），那么$\hat{A}$也是如此（扩张恒等式的原理）。

设$A$是拓扑环，不一定是Hausdorff；令$N$为$A$中$\{0\}$的闭包，令$A' = A/N$为与$A$相关的豪斯多夫环。那么$\hat{A}'$，即$A'$的完成，称为$A$的*豪斯多夫完成*，也用$\hat{A}$表示。如§ 3, no. 4，命题 8 所示，$A$ 的每个连续环同态 $u$ 具有*完整的 Hausdorff* 拓扑环 $C$ 都可以唯一因式分解为 $u = v \circ \varphi$，其中$v$是$\hat{A}$到$C$的连续同态，$\varphi$是$A$到$\hat{A}$的典范映射。如果$A, B$是两个拓扑环，并且$u : A \to B$是连续的同态，则存在唯一的连续同态$\hat{u} : \hat{A} \to \hat{B}$使得图表

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
\varphi \downarrow & & \psi \downarrow \\
\hat{A} & \xrightarrow{\hat{u}} & \hat{B}
\end{array}
$$

是可交换的（$\varphi$ 和 $\psi$ 是典范映射）；我们只需将前面的结果应用到$\psi \circ u$即可。

### 6. 拓扑模

#### 定义 3 {#top-iii-s6-def-3 .statement tag=0BNH}

*给定拓扑环* $A$ *与单位元素，拓扑左* $A$*-模为集合* $E$，*与*一起：

1) *左* $A$*-模块结构*;
2) *拓扑与*$E$的加法群结构兼容，*和满足以下公理*：
(MT) *映射* $(\lambda, x) \to \lambda x$ *从* $A \times E$ *进入* $E$ *是连续的*。

我们定义类似地是拓扑右$A$模的概念；由于每个右$A$-模块都可以被视为左$A^0$-模块，其中$A^0$是$A$的逆环，并且由于$A$的拓扑与$A^0$的环结构兼容，因此无需区分拓扑右$A$-模块和拓扑左$A^0$-模块。

#### 例 1 {#top-iii-s6-n6-exa-1 .statement tag=0BNI}

$\mathbf{R}$（或$\mathbf{C}$）上的拓扑向量空间是拓扑$\mathbf{R}$（或$\mathbf{C}$）模。

#### 例 2 {#top-iii-s6-n6-exa-2 .statement tag=0BNJ}

令$A$为环，令$\mathfrak{B}$为$A$的两侧理想的$A$由……组成上的滤波器基；设$E$为左$A$模块。如果我们给出$A$拓扑（与其环结构兼容），其中$\mathfrak{B}$是$0$（no. 3，例3）的邻域的基本系统，并且$E$拓扑 （与其加法群结构兼容）其中集合$aE$，因为$a$贯穿$\mathfrak{B}$，形式是$0$的邻域的基本系统（$§ 1$， no. 2，例），立即验证$E$是拓扑$A$模块。

#### 注 {#top-iii-s6-n6-rem-1 .statement tag=0BNK}

给定拓扑环$A$，考虑在左侧$A$-模块$E$、拓扑与$E$的加法群结构兼容。凭借身份
$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0)x_0 + \lambda_0(x - x_0) + (\lambda - \lambda_0)(x - x_0)
$$
公理 (MT) 等价于以下三个公理的合取：
（MT$_I'$）。 *对于每个* $x_0 \in E$，*映射* $\lambda \to \lambda x_0$ *在点* $\lambda = 0$ 处连续。
（MT$_{II}'$）。 *对于每个* $\lambda_0 \in A$，*映射* $x \to \lambda_0 x$ *在点* $x = 0$ 处连续。
（MT$_{III}'$）。 *映射* $(\lambda, x) \to \lambda x$ *在点* $(0, 0)$ 连续。

We deduce from this a necessary and sufficient set of conditions that the *filter* $\mathfrak{B}$ *of neighbourhoods of* $0$ *in an* $A$*-module* $E$ *must satisfy in order to define a topology on* $E$ *compatible with its module structure;* $\mathfrak{B}$ *must satisfy the axioms* (GA$_I$) *and* (GA$_{II}$) *of* $§ 1$, *no. 2*, *and in addition must satisfy the following three axioms:*
(MV$_I$). *对于每个*$x_0 \in E$*和*$V \in \mathfrak{B}$，*有邻域*$S$*的*$0$*在*$A$*这样*$S.x_0 \subset V$。
（MV$_{II}$）。 *对于每个*$\lambda_0 \in A$*和*$V \in \mathfrak{B}$，*存在*$W \in \mathfrak{B}$*使得*$\lambda_0 W \subset V$。
（MV$_{III}$）。 *对于每个* $V \in \mathfrak{B}$ *都存在* $U \in \mathfrak{B}$ *和邻域* $T$ *的* $0$ *在* $A$ *这样* $T.U \subset V$。

当环 $\mathbf{Z}$ 被赋予离散拓扑时，每个交换拓扑群都是拓扑$\mathbf{Z}$ 模。

如果$M$是拓扑$A$模块$E$的子模，很明显，$E$的拓扑在$M$上诱导的拓扑与$M$的模结构兼容。此外，在商$A$模$E/M$上，$E$与$M$的商拓扑的商拓扑与$A$模结构兼容。要看到这一点，只需证明 $A \times (E/M)$ 到 $E/M$ 的映射 $(\lambda, x) \to \lambda x$ 是连续的（其中 $x \to x'$ 表示 $E$ 到 $E/M$ 的典范映射）。现在，由于我们可以将认同加法拓扑群$A \times (E/M)$和$(A \times E)/(\{0\} \times M)$（§ 2, no. 9，命题26的推论），足以证明$A \times E$的映射$(\lambda, x) \to \lambda x'$变成$E/M$是连续的；这是直接的，因为所讨论的映射是$x \to x'$和$(\lambda, x) \to \lambda x$的合成。

令$(E_i)_{i \in I}$为拓扑$A$模块的任意族，并令$E = \prod_{i \in I} E_i$为$A$模块，即$E_i$的乘积。那么$E$上的乘积拓扑就与$E$的$A$模块结构兼容。为了证明这一点，只要证明 $A \times E$ 到 $E$ 的映射 $(\lambda, x) \to (\lambda \cdot \mathrm{pr}_i x)_{i \in I}$ 是连续的，或者（通过章 I, § 4, no. 1 的命题 1）对于每个指标 $x \in I$ 映射 $(\lambda, x) \to \lambda \cdot \mathrm{pr}_x x$是$A \times E$到$E_x$的连续映射；但是这个映射是$(\lambda, x_x) \to \lambda x_x$和$(\lambda, x) \to (\lambda, \mathrm{pr}_x x)$的合成，两者都是连续的。

令 $A$ 为 Hausdorff 拓扑环，$E$ 为 Hausdorff 拓扑 $A$ 模。令$\hat{E}$为加法群，这是交换拓扑群$E$（§ 3, no. 5，定理2）的完成。 加法群 $A, E$ 的乘积 $A \times E$ 的 $\mathbf{Z}$ 双线性映射 $(\lambda, x) \to \lambda x$ 到加法群 $E$ 可以通过连续性扩展到 $\mathbf{Z}$ 双线性映射 $\hat{A} \times \hat{E}$变成$\hat{E}$（no. 5，定理1），这个映射我们继续用$(\lambda, x) \to \lambda x$表示。凭借原理或扩张的身份，我们对$\lambda \in \hat{A}, \mu \in \hat{A}$和$x \in \hat{E}$有$\lambda (\mu x) = (\lambda \mu) x$，对所有$x \in \hat{E}$有$1 \cdot x = x$； 外法则$(\lambda, x) \to \lambda x$因此定义$\hat{E}$上的$\hat{A}$模块结构与其拓扑兼容。由此定义的拓扑$\hat{A}$-模块$\hat{E}$称为拓扑$A$-模块$E$的*完成*。

令$E$是拓扑环$A$上的拓扑模，其中$A$和$E$都不一定是Hausdorff。令$N$（或$F$）为$A$（或$E$）中$\{0\}$的闭包。 $N$是$A$（no. 4，命题5）的双面理想，$F$是$E$（no. 1，命题1）的子$A$模；此外，根据连续性，每当$\lambda \in N$或$x \in F$时，我们就有$\lambda x \in F$。因此，我们可以将定义乘以经过，将$(A/N) \times (E/F)$的商映射$(\dot{\lambda}, \dot{x}) \to \dot{\lambda} \dot{x}$化为$E/F$；很容易验证（通过使用 § 2, no. 9 的命题 26 的推论）该映射是连续的，因此定义结构是 $E/F$ 上的拓扑 $(A/N)$ 模。如果我们放置 $B = A/N$ 和 $L = E/F$，那么 $B$ 模块 $L$ 称为 Hausdorff 模 *关联* 与 $E$；它的补全$\hat{L}$是$A$（no. 5）的Hausdorff补全$\hat{A}$（等于定义到$\hat{B}$）的拓扑模，而这个模$\hat{L}$被称为*Hausdorff补全* $E$ 并用$\hat{E}$ 表示。我们在 , no. 4, 命题 8 中看到，$E$ 的每个连续同态 $u : E \to G$ 分解成一个完整的 Hausdorff $\hat{A}$-模 $G$ 唯一因式分解为 $u = v \circ \varphi$，其中 $v$ 是一个连续$\hat{E}$的同态进入$G$，$\varphi$是$E$的典范映射进入$\hat{E}$。我们结论如果$E, E'$是两个拓扑$A$模块并且$u : E \to E'$是一个连续同态，那么存在一个唯一的连续同态$\hat{u} : \hat{E} \to \hat{E}'$使得图表

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow \varphi & & \downarrow \varphi' \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{E}'
\end{array}
$$

是可交换的，$\varphi$ 和 $\varphi'$ 是典范映射。

定义和截面的结果同样适用于任意拓扑环上的*伪模块*，通过删除环的单位元素的所有提及。

### 7. 拓扑划分环和域

接下来，在章、IV和V中，如果$K$是环*的除法，我们将用$K^*$表示$K$的非零元素的*乘法群*。

#### 定义 4 {#top-iii-s6-def-4 .statement tag=0BNL}

*拓扑划分环是集合* $K$ *携带划分环结构和拓扑与* $K$的环结构兼容，*和加法中的满足以下公理：*

(KT) *映射* $x \to x^{-1}$ *从* $K^*$ *到* $K^*$ *是连续的。*

*交换拓扑除法环称为拓扑域。*

如果相应的环结构和拓扑兼容并且满足加法公理 (KT)，则集合 $K$ 上的除环结构和拓扑被称为“相容的”。

#### 例 1 {#top-iii-s6-n7-exa-1 .statement tag=0BNM}

在任何除法环 $K$ 上，*离散* 拓扑与除法环结构兼容。 拓扑是离散的拓扑除法环称为*离散*除法环。

#### 例 2 {#top-iii-s6-n7-exa-2 .statement tag=0BNN}

\* 有理线 $Q$（分别为实直线 $R$）的拓扑与 $R$（分别为 $R$）的域结构兼容（参见章 IV, § 3）。 \*

定义 4 表明，如果$K$ 是环的拓扑划分，则$K$ 在乘法群 $K^*$ 上*诱导*的拓扑与$K^*$ 的群结构兼容。

如果$a \neq 0$，同态$x \to ax$和$x \to xa$是$K$自身的同胚；对于所有 $b \in K$ 来说，映射 $x \to ax + b$ 也是如此。 注如果 $a \neq 0$，则$x \to ax$ 和 $x \to xa$ 是 $K$ 的（拓扑）*加法群* 的 *自同构*。如果$V$是$K$中$o$的任何邻域，则对于所有$a \neq 0$，$aV$和$Va$是$o$的邻域。

令$X$为拓扑空间，并令$f$为$X$的映射为拓扑划分环$K$。如果 $f$ 在点 $x_0 \in X$ 连续，并且如果 $f(x_0) \neq 0$，则 $f^{-1}$ 在 $x_0$ 连续。特别是，如果$K$是拓扑*域*，则$n$变量中系数在$K$中的每个*有理函数*在$K^n$的每个点处连续，其中其分母不消失。

同样，如果$f$是集合$X$的映射，经过滤器$\mathfrak{F}$过滤，成为豪斯多夫拓扑划分环$K$，并且如果$\lim_{\mathfrak{F}} f$存在且不是$0$，则$\lim_{\mathfrak{F}} f^{-1}$ 存在并且我们有

$$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}.
$$

如果$H$是拓扑除法环$K$的*除法子环*，则$K$的拓扑在$H$上诱导的拓扑与环结构的除法兼容$H$。在$H$上定义的拓扑划分环的结构据说是由$K$的拓扑划分“诱导”的。此外，$\overline{H}$也是$K$的*除法子环*（证明类似于命题5）。

在拓扑划分环 $K$ 中，集合 $\{0\}$ 的闭合是双边理想，由命题 5 实现，因此必须是 $\{0\}$ 或 $K$。在其他字中，如果$K$的拓扑不是最粗糙的拓扑（章I, § 2, no. 2），那么它是Hausdorff（§ 1, no. 2，命题2）。

### 8. 拓扑划分上的均匀性环

如果$K$是拓扑划分环，则需要区分：
1) $K$的*加法群*的均匀度，定义在$K$上，称为$K$的*加性均匀度*； 2) *乘法群* $K^*$ 的左右均匀性，它们在 $K^*$ 上定义，并被称为（滥用语言）$K$ 的*乘法*均匀性。

由 $K$ 的加法均匀性在 $K^*$ 上*引发*的均匀性通常与 $K$ 的乘法均匀性“截然不同”（参见习题 17）。

到命题 6，豪斯多夫拓扑划分环 $K$ 可以被视为 *稠密子环* 的 *完整豪斯多夫环* $\hat{K}$。在阶中，$\hat{K}$应该是*拓扑划分环*，映射 x \to x^{-1} 必须可以通过连续性扩展到 (\hat{K})^*；并且这个必要的条件也是足够的，对于函数 xx^{-1}，由于扩张的原理恒等式，x^{-1}x和1在(\hat{K})^*上相等，因此扩展的函数的值是每个x的倒数$x \neq 0$ 于 $\hat{K}$。其他字（cf.章II、、no. 6、命题11）

#### 命题 7 {#top-iii-s6-prop-7 .statement tag=0BNO}

*Hausdorff 拓扑划分的完成 $\hat{K}$ 环 K 是拓扑划分环当且仅当每个柯西滤波器（相对于加法结构）的映射 $x \to x^{-1}$ 下的像（在 0 处不具有簇点）是柯西滤波器（相对于添加剂结构）。*

存在拓扑划分环，其中条件不满足，并且其中环$\hat{K}$具有零因子（参见习题26）。此外，即使完成$\hat{K}$是拓扑除法环，也没有*先验*理由假设$\hat{K}$的*乘法*结构是*完备的*空间的结构。然而，对于除法环 K 来说，$\hat{K}$ 是*局部紧凑*（参见章 I, § 9, no. 7、命题 13 和章 III, § 3, no. 3、命题 4）以及拓扑 *域*；对于后者，我们有以下命题：

#### 命题 8 {#top-iii-s6-prop-8 .statement tag=0BNP}

*如果拓扑域 K 的加性均匀性结构是完整 Hausdorff 空间的结构，则 K* 上的乘法结构是完整空间的结构。*

我们将证明，如果 $\mathfrak{F}$ 是关于 K* 上的*乘法* 结构的柯西滤波器，则 $\mathfrak{F}$ 是关于 K* 上的*加法* 结构的柯西滤波器，并且不收敛于 0；这将确定结果。设 U 为 K 中任何 0 的邻域，令 V 为 0 的闭邻域，使得 $V \subset U, VV \subset U$ [公理 (AV$_\text{II}$)] 和 $-1 \notin V$；那么到假设时，就有集合 $A \in \mathfrak{F}$，这样，对于所有 $x \in A$ 和 $y \in A$，我们就有 $x^{-1}y \in 1 + V$。设$a \in A$，然后$A \subset a + aV$，$a + aV$是一个闭集合，包含不为0；因而 0 不在 A 的闭包中，因此不是 $\mathfrak{F}$ 的簇点。令 W 为 0 的邻域，使得 $aW \subset V$ [公理 (AV$_\text{I}$)]；那么到假设就有集合$B \in \mathfrak{F}$这样$B \subset A$，并且对于所有$x \in B$和$y \in B$，我们有$x^{-1}y \in 1 + W$；因而$y - x \in xW \subset AW \subset aW + aVW$；但 K 是可交换的，因而 $aVW = aWV \subset VW \subset U$；从而$y - x \in U + U$和命题得证。

同样的证明表明，命题8可以扩展到这样的情况：每个关于K的乘法结构*一个*的柯西滤波器也是关于另一个乘法结构的柯西滤波器。

### 习题{#top-iii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
