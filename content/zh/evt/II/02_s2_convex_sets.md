---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 2
section_title: Convex sets
lang: zh
source: evt-i-v
book_pages: TVS II.7-TVS II.21
pdf_pages: 0044-0058, 0102-0109
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a convex set
      page: 7
      pdf_page: 44
    - "no": 2
      title: Intersections of convex sets. Products of convex sets
      page: 9
      pdf_page: 46
    - "no": 3
      title: Convex envelope of a set
      page: 9
      pdf_page: 46
    - "no": 4
      title: Convex cones
      page: 10
      pdf_page: 47
    - "no": 5
      title: Ordered vector spaces
      page: 12
      pdf_page: 49
    - "no": 6
      title: Convex cones in topological vector spaces
      page: 13
      pdf_page: 50
    - "no": 7
      title: Topologies on ordered vector spaces
      page: 15
      pdf_page: 52
    - "no": 8
      title: Convex functions
      page: 16
      pdf_page: 53
    - "no": 9
      title: Operations on convex functions
      page: 18
      pdf_page: 55
    - "no": 10
      title: Convex functions over an open convex set
      page: 18
      pdf_page: 55
    - "no": 11
      title: Semi-norms and convex sets
      page: 19
      pdf_page: 56
statements: 51
exercises: 43
content_sha256: 9f78c4ba070c242476fcc41e6887b724520c6f96addaaa110c8c3add9ea73a0d
translated_from: content/en/evt/II/02_s2_convex_sets.md
translation_method: google
source_content_sha256: a0e92c270cc61535db50016db128351dc2a69eca0c0c5a5f6017a665abb322f1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 2b438a0c45e4206b05fd7699c4a2591ab7964bb93481426b8daf3c83b451ce24
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。凸集合

### 1. 凸集合的定义

对于仿射空间$E$、点$\lambda x + \mu y$的任意两个点$x, y$、集合，其中$\lambda \geq 0, \mu \geq 0, \lambda + \mu = 1$称为以点$x$和$y$结尾的闭线段；当$x = y$时，它从约化到点。该线段中$x$的补集称为结尾为点$x, y$的线段，在$x$开，在$y$闭；如果 $x = y$ 则为空。最后以点$x, y$为结尾的闭段中$\{ x, y \}$的补集称为以点$x, y$为结尾的开段；当$x = y$时它是空的。

#### 定义 1 {#evt-ii-s2-def-1 .statement tag=07B4}

— 仿射空间 $E$ 的子集 $A$ 是凸的，如果对于 $A$ 的每两个点 $x, y$，以点 $x, y$ 结尾的闭线段包含在 $A$ 中。

作为$(1 - \lambda) a + \lambda x = a + \lambda (x - a)$，这个定义等价于：集合$A$是凸的，如果对于每个点$a \in A$，$A$的变换乘以中心的位似 $a$和比率$\lambda$，其中$0 < \lambda < 1$包含在$A$中（在其他字中，$A$对于这些同位语是稳定的）。

#### 例 1 {#evt-ii-s2-n1-exa-1 .statement tag=07B5}

$E$（特别是空集）的每个线性仿射簇都是凸的。

#### 例 2 {#evt-ii-s2-n1-exa-2 .statement tag=07B6}

$\mathbf{R}$ 中唯一的非空凸集合是区间（GT，IV, § 2.4，道具 1）。

#### 例 3 {#evt-ii-s2-n1-exa-3 .statement tag=07B7}

令 $E$ 为向量空间，并且在 $E$ 上为 $\|x\|$ 范数； 单位球$B$，由点$x$组成

这样 $\|x\| \leq 1$ 是凸的，因为关系 $\|x\| \leq 1, \|y\| \leq 1$，对于 $0 \leq \lambda \leq 1$ 意味着
$$
\|\lambda x + (1 - \lambda) y\| \leq \lambda \|x\| + (1 - \lambda) \|y\| \leq \lambda + (1 - \lambda) = 1 .
$$

#### 注{#evt-ii-s2-n1-rem-1 .statement tag=07B8}

— 令 $A$ 为向量空间 $E$ 的凸子集；对于任何标量 $\alpha > 0$ 和 $\beta > 0$，我们有 $\alpha A + \beta A = (\alpha + \beta) A$。在其他字中，对于任何$x \in A, y \in A$，存在$z \in A$使得$(\alpha + \beta) z = \alpha x + \beta y$；事实上，这个关系可以写成$z = \frac{\alpha}{\alpha + \beta} x + \frac{\beta}{\alpha + \beta} y$，并且我们有$\frac{\alpha}{\alpha + \beta} > 0, \frac{\beta}{\alpha + \beta} > 0$和$\frac{\alpha}{\alpha + \beta} + \frac{\beta}{\alpha + \beta} = 1$，使用def可以从中得出断言。 1.

#### 命题 1 {#evt-ii-s2-prop-1 .statement tag=07B9}

*设$(x_i)$为凸子集$A$的点族； $x_i$的每个重心$\sum_i \lambda_i x_i$由正质量$\lambda_i$形成（例如$\sum_i \lambda_i = 1$和$\lambda_i = 0$，除了有限多个指标、cf. A、II, § 9.3）属于到$A$。*

显然，我们只需要考虑对于每个$i$，指标是$1, 2, ..., p$和$\lambda_i > 0$的情况；如果 $p = 1$，命题是微不足道的；我们通过$p$上的归纳证明结果。把$\mu = \sum_{i=1}^{p-1} \lambda_i > 0$，和$y = \sum_{i=1}^{p-1} \frac{\lambda_i}{\mu} x_i$； 归纳假设意味着$y \in A$。现在为 $\lambda_p = 1 - \mu$ 和 $\sum_{i=1}^p \lambda_i x_i = \mu y + (1 - \mu) x_p$，它来自 def。 1 $\sum_{i=1}^p \lambda_i x_i$ 属于至 $A$。

#### 命题 2 {#evt-ii-s2-prop-2 .statement tag=07BA}

*设$E$和$F$为两个仿射空间，$f$为$E$在$F$的仿射线性映射；那么$f$下$E$的凸子集的像，以及$f$下$F$的凸子集的逆像都是凸的。*

结尾为点 $x, y$ 的闭合线段的 $f$ 下的像是结尾为点 $f(x), f(y)$ 的闭合线段，因此第一个叙述。我们推导出$F$的闭路段在$f$包含下的逆像，每个闭路段的端点为点属于；道具的第二个叙述。 2如下。

特别是位似下凸集合的像或平移是凸集合。

#### 命题 3 {#evt-ii-s2-prop-3 .statement tag=07BB}

*在仿射空间$E$中，令$H$为由关系$g(x) = 0$定义的超平面，其中$g$是$E$上的非常数仿射函数。那么由关系 $g(x) \geq 0, g(x) \leq 0, g(x) > 0, g(x) < 0$ 定义的半空间是凸的。*

因为这些是逆像低于$g$或区间或$\mathbf{R}$，因此是凸的。

具有记号的支撑。 3 仿射空间的子集 $M$ 的点位于超平面 $H$ 的*同一侧*（或*严格位于同一侧*），如果 $M$ 包含在由 $g(x) \geq 0, g(x) \leq 0$ 定义的半空间之一中（分别为 $g(x) > 0$ 或 $g(x) < 0$）。

#### 命题 4 {#evt-ii-s2-prop-4 .statement tag=07BC}

*当且仅当$A$不满足$H$时，$A$的点、仿射空间$E$的凸子集严格位于超平面$H$的同一侧。*

显然条件是必要的。相反，假设满足，并令 $g(x) = 0$ 为定义 H 的方程（$g$ 是 E 在 $\mathbf{R}$ 中的仿射线性映射）。 集合 $g(A)$ 在 $\mathbf{R}$ 中是凸的，因此它是区间，以及 $0 \notin g(A)$。因此$g(x)$对于所有$x \in A$来说都是固定符号。

### 2. 凸集合的交。凸集合的乘积

#### 命题 5 {#evt-ii-s2-prop-5 .statement tag=07BD}

— *交任何凸族子集仿射空间* E *是凸*。

命题紧随 def 之后。 1 个II、p. 7。

#### 命题 6 {#evt-ii-s2-prop-6 .statement tag=07BE}

— *让* $(E_i)_{i \in I}$ *成为向量空间的一个家族，并且对于每个* $i \in I$，*让* $A_i$ *成为* $E_i$的非空子集。 *则集合* $A = \prod_{i \in I} A_i$ *在* $E = \prod_{i \in I} E_i$ 中凸，*当且仅当，对于所有* $i \in I$，*集合* $A_i$ *在* $E_i$ 中凸。

事实上，每个投影$\mathrm{pr}_i$都是线性映射，我们有$A_i = \mathrm{pr}_i A$和$A = \bigcap_{i \in I} \mathrm{pr}_i^{-1}(A_i)$； 命题来自 props。上面2和5。

#### 推论 {#evt-ii-s2-n2-cor-1 .statement tag=07BF}

— *在空间* $\mathbf{R}^n$ *每个平行同位素* (GT, VI, § 1.3) *是凸子集*。

因为它是在长方体的仿射线性映射下的像，并且最后一个是由支柱凸出的。 6.

#### 命题 7 {#evt-ii-s2-prop-7 .statement tag=07BG}

— *设* A *和* B *为向量空间* E的两个凸子集。 *对于任何实数* $\alpha, \beta$ *集合* $\alpha A + \beta B$ *(形式* $\alpha x + \beta y$ 点集合，*其中* $x$ *在* A 中变化，*且* $y$ *在* B*) 中是凸*。

对于$\alpha A + \beta B$是$E$中$E \times E$的线性映射$(x, y) \mapsto \alpha x + \beta y$下$E \times E$的凸子集$A \times B$的像。

### 3. 集合的凸包络线

#### 定义 2 {#evt-ii-s2-def-2 .statement tag=07BH}

— *给定仿射空间* E 的子集* A *，*我们称所有凸集合包含* A 的交，*A 的凸包络，*也就是说*（II，p. 9，道具 5）*它是最小的凸集合包含* A.

#### 命题 8 {#evt-ii-s2-prop-8 .statement tag=07BI}

— *对于任何族* $(A_i)_{i \in I}$ *仿射空间* E 的凸子集，*$\bigcup_{i \in I} A_i$ *的凸包络 *恰好是线性组合* $\sum_{i \in I} \lambda_i x_i$ 的集合，*其中* $x_i \in A_i, \lambda_i \geq 0$ *对于所有* $i \in I$ ($\lambda_i = 0$) *除了有限多个指标*) *和* $\sum_{i \in I} \lambda_i = 1$。

用C表示这些线性组合中的集合，显然C包含在每个凸集合中，其中包含所有$A_i$（II，p. 8，道具1）；另一方面，对于每个$i$，$A_i \subset C$。 剩下要证明的是 C 是凸的。 令$x = \sum \lambda_i x_i$、$y = \sum \mu_i y_i$为C的两个点，$\alpha$为数，使得$0 < \alpha < 1$，对于每个i ∈ I，写出γ_i = αλ_i + (1 - α) μ_i，并令J为集合（有限） 指标 I 其中 γ_i ≠ 0。 我们可以写 αx + (1 - α)y = Σ_{i∈J} γ_i z_i，其中

$$ z_i = \gamma_i^{-1}(\alpha\lambda_i x_i + (1 - \alpha) \mu_i y_i) $$

对于所有 i ∈ J，属于到 A_i；但是$\sum_{i\in J} \gamma_i = \alpha \sum_{i\in I} \lambda_i + (1 - \alpha) \sum_{i\in I} \mu_i = 1$，我们看到$ax + (1 - \alpha) y \in C$。 命题得证。

#### 推论 1 {#evt-ii-s2-prop-8-cor-1 .statement tag=07BJ}

*E 的子集 A 的凸包络与线性组合 $\sum_i \lambda_i x_i$ 的集合相同，其中 $(x_i)$ 是 A 的点、数 $\lambda_i > 0, \text{ for all } i$ 和 $\sum_i \lambda_i = 1$ 的任何有限族。*

由凸集合 A 生成的仿射线性簇 (A, II, § 9.3) 的维数称为 A 的 *维数*。

令 E 为向量空间。 E 中集合 A 的平衡包络线的凸包络线 C 称为 A 的*平衡凸包络线*（或*对称凸包络线*）；显然，包含于 A 是最小的对称凸集合；它也是 $A \cup (-A)$ 的凸包络线，因为属于的平衡包络线的每个点到具有端点 a 和 −a 的线段，其中 $a \in A$。 集合 C 重合，其中集合为线性组合 $\sum_i \lambda_i x_i$，其中 $x_i \in A$ 和 $\sum_i |\lambda_i| \leq 1$；因为很明显，点的集合是凸的，包含A和-A；证明它包含在C中就足够了，为此我们只需要考虑那些$\mu = \sum_i |\lambda_i| > 0$的线性组合；然后我们可以用$\alpha_i = \lambda_i/\mu$和$y_i = x_i$来写$\sum_i \lambda_i x_i = \mu \cdot \sum_i \alpha_i y_i$，如果$\lambda_i \geq 0$；和$\alpha_i = -\lambda_i/\mu$； $y_i = -x_i$如果$\lambda_i < 0$；显然$\sum_i \alpha_i = 1$，我们的断言就被证明了。

#### 推论 2 {#evt-ii-s2-prop-8-cor-2 .statement tag=07BK}

*设 f 为仿射空间 F 中仿射空间 E 的仿射线性映射；对于 E 的每个子集 A，f(A) 的凸包络线是 A 的凸包络线 f 下的像。*

线性映射也有类似的叙述和平衡凸包络线。

### 4. 凸锥体

#### 定义 3 {#evt-ii-s2-def-3 .statement tag=07BL}

*仿射空间的子集 C 如果 C 对于中心 x_0 的所有同位性且比率 > 0 都是不变的，则 E 是顶点为 x_0 的圆锥体。*

我们将假设在这一项和接下来的一项中，我们选择了所考虑的圆锥体的顶点作为 E 中的原点； *即*我们假设 E 是向量空间，当我们谈到圆锥体时，可以理解为该圆锥体的顶点为 0。对于 $\lambda > 0$（分别为 $\lambda \geq 0$），形式 $\lambda a$ 的点集合，其中 $a$ 是非空向量，被称为始于 0 的*开半线*（或*闭半线*）。

如果 $0 \in C$，则顶点 0 的圆锥体 C 被称为“有尖的”，否则被称为“无尖的”。尖锥体要么是单个点 $\{0\}$，要么是从 0 开始的闭合半线的集合的并。非尖锥体是从 0 开始的开放半线的并（可能是空的）。如果 C 是非尖锥体，则 $C \cup \{0\}$ 是尖锥体。如果 C 是尖锥体，则 $C - \{0\}$ 是非尖锥体。

如果 C 是非尖*凸*锥体，则 $C \cup \{0\}$ 是尖头凸锥体。然而，如果C是尖凸锥体，则$C - \{0\}$不一定是凸锥体。如果一个尖的凸锥体不包含穿过0的任何线经过，我们就说它是“正确的”。然后

#### 命题 9 {#evt-ii-s2-prop-9 .statement tag=07BM}

*当且仅当非尖锥$C'$（C中0的补集）是凸的时，尖凸锥C才是正确的。*

如果 C 包含是一条穿过 0 的线，那么显然 $C'$ 不是凸的。现在假设C是正确的，并且令x，y是$C'$的两个点。以点 x, y 为终点的闭线段包含在C中；如果它包含 0 那么 $\lambda x + (1 - \lambda) y = 0$ 对于某些 $\lambda$ 和 $0 < \lambda < 1$，因此 $x = \mu y$ 和 $\mu < 0$。因此，C包含穿过0和x的线，与假设相反。

#### 命题 10 {#evt-ii-s2-prop-10 .statement tag=07BN}

*E 的子集 C 是凸锥当且仅当 $C + C \subset C$ 和 $\lambda C \subset C$ 对于所有 $\lambda > 0$。*

对于条件 $\lambda C \subset C$ 对于所有 $\lambda > 0$ 表征锥体。如果 C 是凸的，我们有 $C + C = \frac{1}{2}C + \frac{1}{2}C = C$ (II, p. 8, *注*)。相反，如果圆锥体C满足$C + C \subset C$，那么对于$0 < \lambda < 1$，我们有$\lambda C + (1 - \lambda) C = C + C \subset C$，这表明C是凸的。

#### 推论 1 {#evt-ii-s2-prop-10-cor-1 .statement tag=07BO}

*如果C是非空凸锥体，C生成的向量空间是集合$C - C$（点$x - y$的集合，其中x，y在C中变化）。*

因为，如果$V = C - C$，则V非空，对于所有$\lambda \neq 0$，我们有$\lambda V = V$，以及$V + V = C + C - (C + C) \subset C - C = V$，这表明V是向量子空间。最后每向量子空间包含C还有包含V。

#### 推论 2 {#evt-ii-s2-prop-10-cor-2 .statement tag=07BP}

*若C为尖凸锥体，则C包含的最大的向量子空间为集合$C \cap (-C)$。*

对于，如果 $W = C \cap (-C)$，那么 W 是非空的，并且 $\lambda W = W$ 对于所有 $\lambda \neq 0$，也
$$
W + W \subset (C + C) \cap (-(C + C)) \subset C \cap (-C) = W,
$$
这表明W是向量子空间。显然C中包含的每个向量子空间也包含在W中。

显然，如果$f$是向量空间F中E的线性映射，则E中凸锥C的$f(C)$、像是F中的凸锥。E中每一个交凸锥（顶点为0）都是凸锥。对于凸锥体包含 A 的 E 交的每个子集 A（这些存在，E 本身就是这样一个锥体）是最小的凸锥体，即包含 A；它被称为由 A *生成*的凸锥体。

#### 命题 11 {#evt-ii-s2-prop-11 .statement tag=07BQ}

*令$(C_i)_{i \in I}$为E中的凸锥族； $C_i$的并生成的凸锥与点$\sum_{i \in J} x_i$的集合相同，其中J是所有$i \in J$的I和$x_i \in C_i$中的任何有限子集。*

事实上，显然这样的点的C、集合，是$C_i$的凸锥包含并，并且它包含在包含这个并的任意凸锥中。

#### 推论 {#evt-ii-s2-n4-cor-1 .statement tag=07BR}

— *对于 E 的任何子集 A，由 A 生成的凸锥体与线性组合* $\sum_{i \in J} \lambda_i x_i$ 的集合相同，*其中* $(x_i)_{i \in J}$ *是 A 的点的任何有限非空族，并且其中* $\lambda_i > 0$ *对于所有* $i \in J$。

足以看出，如果 A 的凸锥包含点 $x \neq 0$，那么它也是包含点 $\lambda x$ 的半线$C_x$，其中$\lambda$在正数的集合变化，并且$C_x$是凸锥体。

#### 命题 12 {#evt-ii-s2-prop-12 .statement tag=07BS}

— *如果A是E中的凸集合，则A生成的凸锥体与*$C = \bigcup_{\lambda > 0} \lambda A$相同。

集合 C 显然是一个圆锥体；只要证明 C 是凸的就足够了。令$\lambda x, \mu y$为C($\lambda > 0, \mu > 0, x \in A, y \in A$)中的两个点。令$\alpha, \beta$为两个数$> 0$，使得$\alpha + \beta = 1$。然后是$\alpha \lambda x + \beta \mu y = (\alpha \lambda + \beta \mu) z$，还有$z \in A$，还有$\alpha \lambda + \beta \mu > 0$；因此$\alpha \lambda x + \beta \mu y \in C$。

#### 注 {#evt-ii-s2-n4-rem-1 .statement tag=07BT}

— 1）根据道具的假设。 12、如果$0 \notin A$，则圆锥体C是非尖的，因此$C \cup \{0\}$是*正确的*。

2) 设A为E中任意凸集合；考虑空间$F = E \times \mathbf{R}$中的凸集合$A_1 = A \times \{1\}$以及由$A_1$生成的顶点为0的凸锥C。命题 12 表明，F 中 $A_1$ 是 C 和超平面 $E \times \{1\}$ 的交。因此，E 中的每个凸集合都可以被视为 F 中顶点为 0 的凸锥的交的 E 上的投影，并且超平面$E \times \{1\}$。

### 5. 已订购向量空间

向量空间 E 上的 *预序* 结构，用 $x \leqslant y$ 或 $y \geqslant x$ 表示，如果满足以下两个公理，则与 E 的向量空间结构 *相容的*；

*(EO$_I$)* *如果* $x \leqslant y$ *则* $x + z \leqslant y + z$ *对于所有* $z \in E$。

*(EO$_II$)* *如果* $x \geqslant 0$ *则* $\lambda x \geqslant 0$ *对于每个标量* $\lambda \geqslant 0$。

携带这两个结构的向量空间 E 被称为*预排序的向量空间* （分别是当 E 上预序的关系是阶时*排序的向量空间*）。

注意公理（EO$_I$）意味着E的预序结构和加法群结构是兼容的，也就是说，E携带这两个结构，是一个*预序的群*（A，VI， p. 3）。

#### 例 {#evt-ii-s2-n5-exa-1 .statement tag=07BU}

— 在 A 上定义的所有有限实值函数的空间$E = \mathbf{R}^A$上，阶的关系由«对于所有$t \in A$，$x(t) \leqslant y(t)$»给出，与E的向量空间结构兼容。

#### 命题 13 {#evt-ii-s2-prop-13 .statement tag=07BV}

— (i) *集合 P，元素* $\geqslant 0$，*预定的向量空间 E，是尖凸锥*。

(ii) *相反，如果 P 是 E 中的尖凸锥体，则关系* $y - x \in P$ *是 E 上的预序关系，且预序结构定义是唯一*与 的向量空间结构兼容的E 且 P 为集合或元素 $\geqslant 0$。

(iii) 关系 $y - x \in P$，其中 P 为尖凸圆锥，当且仅当 P 为真圆锥时，在 E 上为序关系。

(i) 公理 (EO_I) 和 (EO_{II}) 意味着对于所有 $\lambda > 0$ 都有 $P + P \subset P$ 和 $\lambda P \subset P$。由于 $0 \in P$，因此 P 是尖凸锥体（II，p. 11，命题 10）。

(ii) 相反，如果 P 是尖凸锥体，关系 $P + P \subset P$ 意味着关系 $y - x \in P$ 是预序与 E 的加法群结构兼容 (A, VI, p. 3, prop. 3）；明确写出$x \leqslant y$、集合 P与$x \geqslant 0$的集合相同；进一步，对于所有 $\lambda \geqslant 0$ 关系 $\lambda P \subset P$ 表明满足公理 (EO_{II})。

(iii) 说 P 是正确的意味着 $P \cap (-P) = \{0\}$ (II, p. 11, cor. 2)，因此 $y - x \in P$ 是序关系。

#### 例 {#evt-ii-s2-n5-exa-2 .statement tag=07BW}

\* 设 H 为真正的希尔伯特空间； H的连续自同态的向量空间$\mathscr{L}(H)$中，正厄米特自同态形式为正尖凸锥；因此，这个圆锥体定义阶结构与$\mathscr{L}(H)$的向量空间结构兼容，其中关系$A \leqslant B$意味着$B - A$是正厄米特自同态。 \*

对于向量空间 E 中的任意尖凸圆锥 P，集合 $P \cap (-P)$ 是 E 的向量子空间，H（II，p. 11，cor. 2）。 $E/H$ 中 P 的典范像 $P'$ 是凸锥，E 中 $P'$ 的逆像是 P。因此 $P' \cap (-P') = \{0\}$，$E/H$ 上的 $P'$ 定义阶结构与其兼容向量空间结构。

如果 E 中的 $x \geqslant 0$ 蕴涵 $f(x) \geqslant 0$，则预购的向量空间 E 上的线性形式 $f$ 被认为是正数。或者，如果E中元素$\geqslant 0$的凸锥体P包含在那些$x$的一半空间中，其中$f(x) \geqslant 0$。显然，在对偶$E^*$到E中，正线性形式的集合是尖凸锥体。

### 6. 拓扑中的凸锥向量空间

#### 命题 14 {#evt-ii-s2-prop-14 .statement tag=07BX}

在拓扑向量空间 E 中，凸集合（分别是凸锥体）的闭包是凸集合（分别是具有相同顶点的凸锥体）。

对于，令 A 为凸集合； 映射$(x, y) \mapsto \lambda x + (1 - \lambda) y$，其中$0 < \lambda < 1$在$E \times E$中连续，映射$A \times A$在A中连续；因此 (GT, I, § 2.1, th. 1) 它在 $\overline{A}$ 中有映射 $\overline{A} \times \overline{A}$，这表明 $\overline{A}$ 是凸的。类似地，如果 C 是顶点为 0 的凸圆锥体，则对于所有 $\lambda > 0$ 来说，$\overline{C} + \overline{C} \subset \overline{C}$ 和 $\lambda \overline{C} \subset \overline{C}$。

#### 定义 4 {#evt-ii-s2-def-4 .statement tag=07BY}

对于拓扑向量空间 E 的任意集合 A，所有闭凸集合包含 A 的交称为 A 的凸闭包络；是最小的凸闭集合包含A。

来自道具。 14、A的凸闭包络线是A的凸包络线的闭包；它显然与 $\overline{A}$ 的凸封闭包络线相同。

类似地，我们称最小的对称、凸、闭集合即包含A，A的对称凸闭包络（或平衡凸闭包络）；是 A 的对称凸包络 (II, p. 10) 的闭包；它也是$\overline{A}$的对称凸闭包络线。

#### 命题 15 {#evt-ii-s2-prop-15 .statement tag=07BZ}

— 令 $A_i$ ($1 \leq i \leq n$) 为 Hausdorff 拓扑向量空间 E 中紧致凸集合的有限数。则 $A_i$ 的并的凸包络是紧致的（因此，与此的凸闭包络相同） 并）。

令 B 为由点 $(\lambda_1, \lambda_2, ..., \lambda_n)$ 定义的 $\mathbf{R}^n$ 中的紧集，其中 $\lambda_i \geq 0$ ($1 \leq i \leq n$) 和 $\sum_{i=1}^n \lambda_i = 1$。 E 中定义 $B \times \prod_{i=1}^n A_i \subset \mathbf{R}^n \times E^n$ 的连续映射由公式 $(\lambda_1, \lambda_2, ..., \lambda_n, x_1, x_2, ..., x_n) \mapsto \sum_{i=1}^n \lambda_i x_i$ 组成。 $\bigcup_{i=1}^n A_i$的凸包络C在这个映射下是$B \times \prod_{i=1}^n A_i$的像；由于 $B \times \prod_{i=1}^n A_i$ 是紧的，E 是 Hausdorff，因此 C 是紧的。

#### 推论 1 {#evt-ii-s2-prop-15-cor-1 .statement tag=07C0}

— 在 Hausdorff 拓扑向量空间中，有限集合的凸包络是紧致的。

#### 推论 2 {#evt-ii-s2-prop-15-cor-2 .statement tag=07C1}

— 在拓扑向量空间 E 中，有限集合的凸包络是预紧的。

事实上，令 j 为 E 的 Hausdorff 完成$\hat{E}$ 中的典范映射；如果C是A的凸包络，则$j(C)$是$\hat{E}$中有限集合$j(A)$的凸包络，因此$j(C)$是紧的（cor.1），因此C是预紧的（GT，II, § 4.2）。

#### 命题 16 {#evt-ii-s2-prop-16 .statement tag=07C2}

— 令 A 为拓扑向量空间 E 的凸子集，至少有一个内部点 $x_0$。对于任意点 $x \in \overline{A}$，末端为点 $x_0, x$ 的开段的每个点位于在 A 的内部。

对于该段的任何点 y，令 f 为中心 y 的位似和比率 $\lambda < 0$，其中变换 $x_0$ 变为 x。如果V是A中包含的$x_0$的开邻域，则$f(V)$是x的邻域，因此包含点$f(z) \in A$；现在

$$
f(z) - y = \lambda (z - y) = \lambda (z - f(z)) + \lambda (f(z) - y),
$$

因此 $y - f(z) = \frac{\lambda}{\lambda - 1} (z - f(z))$，因此 y 通过位似 g、中心 $f(z)$ 和比率 $\mu = \lambda / (\lambda - 1)$ 变换为 z；由于$0 < \mu < 1$，g变换V进入A中包含的0的邻域，命题被证明。

#### 推论 1 {#evt-ii-s2-prop-16-cor-1 .statement tag=07C3}

— 凸集合 $\overline{A}$ 的内部 $\overset{\circ}{A}$ 本身就是凸集合；如果$\overset{\circ}{A}$不为空，则重合具有$\overline{A}$的内部，并且$\overline{A}$是集合，重合具有$\overset{\circ}{A}$的闭包。

它来自道具。 16，如果$\overset{\circ}{A}$不为空，则它是凸集合，并且$\overline{A}$的每个点是$\overset{\circ}{A}$的簇点。接下来我们展示$\overline{A}$属于到$\overset{\circ}{A}$的每个内部点。令 x 为 $\overline{A}$ 的内部点，并假设 $x = 0$ 是确定的。令V为0的对称邻域，包含在$\overline{A}$中，并令$y \in \overset{\circ}{A} \cap V$；现在$-y \in \overline{A}$，因此，通过道具。 16、我们看到$0 \in \overset{\circ}{A}$，如果$y \neq 0$；如果$y = 0$，这显然是正确的。

#### 推论 2 {#evt-ii-s2-prop-16-cor-2 .statement tag=07C4}

— *内部* $\dot{C}$ *凸锥体* C，*本身是凸锥体；如果* $\dot{C}$ *不为空，那么它的重合与* $\overline{C}$、*和* $\overline{C}$ *的内部是一个尖凸圆锥体，重合与* $\dot{C}$闭合。

由于比率 $> 0$ 和中心 0 变换 C 与自身相似，因此它们对 $\dot{C}$ 也同样相似，因此 $\dot{C}$ 是圆锥体； 推论的其余部分来自 cor。 1 以及明显的注释，如果 C 不为空，则 $\overline{C}$ 包含于 C 的顶点。

设 H 为 $\mathbf{R}$ 拓扑向量空间 E 中的闭超平面；它有一个方程形式 $f(x) = \alpha$，其中 $f$ 是连续的线性形式，与 E 中的零不同（I，p. 13，第 1）。因此，分别由$f(x) \leqslant \alpha$和$f(x) \geqslant \alpha$定义的闭合半部空间是*闭合*凸集合；它们的补集分别由$f(x) > \alpha$和$f(x) < \alpha$定义，是*开*凸集合。我们说这些半空间是由 H *确定*的闭（或开）半空间。

#### 命题 17 {#evt-ii-s2-prop-17 .statement tag=07C5}

— *在拓扑向量空间* E 中，*令* A *为集合，且至少有一个内部点，并且其所有点位于超平面* H 的同一侧。 *然后* H * 闭合，* A *的内部点严格位于* H 的同一侧，*和簇* A 的点 *位于* H 的同一侧。 *特别是开（或闭）一半空间由闭超平面* 确定。

事实上，假设 H 包含原点，$f(x) = 0$ 是 H 的方程；为了明确起见，假设 $f(x) \geqslant 0$ 对于所有 $x \in A$。由点 y 形成的半部空间，使得$f(y) > -1$ 包含至少有一个内部点，并且，通过翻译，同样适用于点 y 的半部空间，使得$f(y) > 0$；这表明 H 是闭集 (I, p. 11, 推论)。那么我们知道$f$是E在$\mathbf{R}$上的严格态射（I，p. 13，推论），因此$f(\dot{A})$是$\mathbf{R}$上的开集合。这集合不能包含 0 或者它会包含数 $< 0$ 与假设相反；因此它包含在开放的区间$]0, +\infty[$中。另一方面，那些 y 的一半空间 $f(y) \geqslant 0$ 是闭集且包含 A，因此它是包含 $\overline{A}$。

#### 推论 {#evt-ii-s2-n6-cor-1 .statement tag=07C6}

— *设* P *为拓扑向量空间* E 的尖凸锥体，至少有一个内部点。 *然后每个线性形式* f *与* E上的零不相同，*并且对于由* P (II, p. 13)定义的预序结构为正，*必然是连续的*。 *此外，如果* x *位于* P *then* $f(x) > 0$ *的内部，并且如果* x *是* P *then* $f(x) \geqslant 0$的簇点。

应用道具。 17 到情况$A = P$，其中H是超平面，方程为$f(x) = 0$。

#### 注 {#evt-ii-s2-n6-rem-1 .statement tag=07C7}

在拓扑向量空间 E 中，每个凸集合 C 都是相连的。事实上，如果$a \in C$，则C是段的并，结尾为点a，并在a处闭合；这些是相连的，结果来自 GT, I, § 11.1, prop。 2.

### 7. 有序向量空间上的拓扑

令 E 为有序向量空间。 E 上的拓扑与 E 的有序向量空间结构 *相容的*，如果它既与 E 的向量空间结构兼容并且满足以下公理：

(TO) ** x *与* $x \geqslant 0$ 的凸锥体，*在* E 中闭合。

具有兼容拓扑的有序向量空间 E 称为有序拓扑向量空间。

#### 例 {#evt-ii-s2-n7-exa-1 .statement tag=07C8}

空间$\mathbf{R}^n$及其通常的拓扑和阶结构即阶乘积其因子结构是有序拓扑向量空间。另一方面，对于$n \geq 2$，当$\mathbf{R}^n$携带字典顺序的阶（S，III, § 2.6）时，通常的拓扑与$\mathbf{R}^n$的有序向量空间结构不兼容。

设A为集合； A 上定义的实值有界函数的向量空间 $\mathscr{B}(A ; \mathbf{R})$，其中拓扑由范数 $\|x\| = \sup_{t \in A} |x(t)|$ 定义，阶结构由乘积阶结构引发$\mathbf{R}^A$，是有序拓扑向量空间。

在有序拓扑向量空间 E 中，元素 $x \leq 0$ 的集合是闭集；由于翻译是同态，我们推断，对于所有 $a \in E$，元素 $x \geq a$（或$x \leq a$）的集合都是封闭的。由于$\{0\}$是集合、$x \geq 0$和$x \leq 0$的交，因此$\{0\}$是闭集且E是Hausdorff。

#### 命题 18 {#evt-ii-s2-prop-18 .statement tag=07C9}

在有序拓扑向量空间 E 中，令 H 为关系 $\leq$ 所指向的集合。如果H的截面滤波器在E中有极限，那么这个极限就是H的上界。

对于，设 $b = \lim_{x \in H} x$；对于$y \in H$、$x \in H$的集合，使得$x \geq y$是H的截面滤波器的集合，因此b是该集合的集群点；但由于集合 $x \geq y$ 在 E 中是闭的，所以我们有 $b \geq y$，因此 b 是 H 的上界。 另一方面，如果 a 是 H 的上界，则 H 包含在闭闭的集合 $x \leq a$ 中；由于 b 是 H 的簇点，因此我们有 $b \leq a$，它完成证明（II，p. 72，执行 42）。

### 8. 凸函数

#### 定义 5 {#evt-ii-s2-def-5 .statement tag=07CA}

设 X 为仿射空间 E 的凸子集。如果对于 X 的任何两个不同的点 x, y 和任意一个，在 X 上定义的实值有限函数是凸的（或严格凸的） 实数$\lambda, 0 < \lambda < 1$，我们有：

(1)
$$
f(\lambda x + (1 - \lambda) y) \leq \lambda f(x) + (1 - \lambda) f(y)
$$
（分别。

(2)
$$
f(\lambda x + (1 - \lambda) y) < \lambda f(x) + (1 - \lambda) f(y)).
$$

当$E = \mathbf{R}$时，凸函数的这个定义与FVR中的I、p. 32是一样的。此外，f 在 X 中是凸（或严格凸）的，当且仅当对于每条仿射线 $D \subset E$，f 到 $X \cap D$ 的限制在 $X \cap D$ 中是凸（或严格凸）。

#### 例 {#evt-ii-s2-n8-exa-1 .statement tag=07CB}

如果 f 是 E 上的仿射线性函数，则 f 和 $f^2$ 在 E 上是凸函数；这对于 f 来说是显而易见的，因为
$$
f(\lambda x + (1 - \lambda) y) = \lambda f(x) + (1 - \lambda) f(y);
$$
另一方面，如果$\alpha = f(x), \beta = f(y)$，那么；
$$
\lambda \alpha^2 + (1 - \lambda) \beta^2 - (\lambda \alpha + (1 - \lambda) \beta)^2 = \lambda(1 - \lambda) (\alpha - \beta)^2 \geq 0
$$

$0 < \lambda < 1$；此外，如果$f|D$不是常数，则$f^2$到仿射线$D \subset E$的限制是*严格凸的*。

如果 - $f$ 是凸的（或严格凸的），则在 $X$ 上定义的实值函数 $f$ 是*凹*（或*严格凹*）。也就是说，对于$X$的每两个不同的点$x, y$和每个数$\lambda$，使得$0 < \lambda < 1$，我们有

$$
f(\lambda x + (1 - \lambda) y) \geqslant \lambda f(x) + (1 - \lambda) f(y)
$$

（分别。

$$
f(\lambda x + (1 - \lambda) y) > \lambda f(x) + (1 - \lambda) f(y)).
$$

如果$\mathbf{R}$中的$X$的映射既是凸的又是凹的，则它是*仿射*（*cf.* II、p. 78，练习11）。

#### 命题 19 {#evt-ii-s2-prop-19 .statement tag=07CC}

*令$X$为仿射空间$E$的凸集合；并令 $f$ 为在 $X$ 上定义的实值函数。将点 $(x, a) \in E \times \mathbf{R}$ 中的集合表示为 $F$（分别为 $F'$），其中 $x \in X$ 和 $f(x) \leqslant a$（分别为 $x \in X$ 和 $f(x) < a$）。那么下面的条件是等价的*：

a) *函数 $f$ 是凸的*。
b) *仿射空间 $E \times \mathbf{R}$ 中的集合 $F$ 是凸的*。
c) *仿射空间$E \times \mathbf{R}$中的集合$F'$是凸的*。

我们证明$a) \Rightarrow c)$。设$(x, a)$和$(y, b)$是$F'$和$0 < \lambda < 1$的两个点，则$f(x) < a,\ f(y) < b$并且如果$f$是凸的

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) < \lambda a + (1 - \lambda) b
$$

这表明$E \times \mathbf{R}$属于到$F'$的点$\lambda(x, a) + (1 - \lambda)(y, b)$。因此 $F'$ 是凸的。

接下来我们展示$c) \Rightarrow b)$。如果$(x, a), (y, b)$是$F$的两个点，那么对于每个$\varepsilon > 0$，$(x, a + \varepsilon)$和$(y, b + \varepsilon)$属于到$F'$，如果$0 < \lambda < 1$，$(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b + \varepsilon)$也是如此；通过$F$的定义，这意味着$(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$属于到$F$。

最后$b) \Rightarrow a)$，对于（与上面的记号），如果$(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$属于到$F$则

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda a + (1 - \lambda) b
$$

提供$a \geqslant f(x)$和$b \geqslant f(y)$；因此 (1) 成立，$f$ 是凸的。

#### 推论 {#evt-ii-s2-n8-cor-1 .statement tag=07CD}

*如果 $f$ 在 $X$ 中是凸的，则对于所有 $\alpha \in \mathbf{R}$、$x \in X$ 的集合，使得 $f(x) \leqslant \alpha$（或 $f(x) < \alpha$）是凸的*。

事实上，它是$F$（或$F'$）的交的$E$上的投影和$E \times \mathbf{R}$中的超平面$E \times \{\alpha\}$。

#### 命题 20 {#evt-ii-s2-prop-20 .statement tag=07CE}

*令 $f$ 为凸函数，在仿射* 空间 E 的凸集合 $X$ 上定义。 然后对于$p$点的X的每个家庭$(x_i)_{1 \leq i \leq p}$和$p$实数的每个家庭$(\lambda_i)_{1 \leq i \leq p}$，所有$\geq 0$，这样$\sum_{i=1}^p \lambda_i = 1$，我们有：

(3)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

如果 $f$ 是严格凸的，并且如果 $\lambda_i > 0$ 对于所有 $i$，则

(4)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i),
$$
除非所有$x_i$ 都相等。

不等式 (3) 源自II，道具。上面的 19 和II，p. 8，道具。 1. 假设$x_i$不全部相等（这意味着$p \geq 2$）并且$\lambda_i$都$> 0$；那么点 $z = \sum_{i=1}^p \lambda_i x_i$ 与至少一个 $x_i$ 不同。为了确定性，假设$z \neq x_1$，在$y_1 = \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} x_i$处写下$z = \lambda_1 x_1 + (1 - \lambda_1) y_1$。然后$y_1 \neq x_1$，以及$0 < \lambda_1 < 1$，到假设，我们有，
$$
f(z) < \lambda_1 f(x_1) + (1 - \lambda_1) f(y_1).
$$
但由 (3) $f(y_1) \leq \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} f(x_i)$ 和不等式 (4) 得出。

### 9. 运算在凸函数上

设 X 为仿射空间 E 的凸集合。如果 $f_i (1 \leq i \leq p)$ 是在 X 上定义的有限多个凸函数，并且 $c_i (1 \leq i \leq p)$ 是数 $\geq 0$，则函数 $f = \sum_{i=1}^p c_i f_i$ 是凸的X。

如果 $(f_i)$ 是在 X 上定义的任意凸函数族，并且$g$（X中该族的上包络线）是有限的，则 $g$ 是凸的。

最后，如果 H 是在 X 上定义的凸函数的集合，并且 $\mathfrak{F}$ 是 H 上的一个滤波器，它在 X 中简单地收敛到有限实值函数 $f_0$，则 $f_0$ 在 X 上是凸的。

### 10. 开放凸面集合上的凸面函数

#### 命题 21 {#evt-ii-s2-prop-21 .statement tag=07CF}

令 $f$ 为凸函数，定义在拓扑向量空间 E 中的非空开凸集合 X 上。 那么$f$是连续的当且仅当当限制于X的某个非空开子集U时，它在上面有界。

条件显然是必要的，我们证明它是充分的。令$x_0 \in X$为点，使得$f$在$x_0$的邻域V上界；我们首先证明$f$在$x_0$连续。通过翻译，我们可以将自己限制在$x_0 = 0$和$f(x_0) = 0$的情况；此外，我们可以假设邻域 V 是平衡的（I，p. 7，命题 4）。假设V中有$f(x) \leq a$；对于每个$\varepsilon, 0 < \varepsilon < 1$，我们观察到如果$x \in \varepsilon V$，则$x/\varepsilon \in V$和$-x/\varepsilon \in V$。 II、p. 16到点$x/\varepsilon$和0到数$\lambda = \varepsilon$的应用不等式（1），我们看到$f(x) \leq \varepsilon f(x/\varepsilon) \leq \varepsilon a$； 应用到点 $x$ 和 $-x/\varepsilon$ 和数 $\lambda = 1/(1 + \varepsilon)$，得到 $f(x) \geq -\varepsilon f(-x/\varepsilon) \geq -\varepsilon a$。因此，如果$\varepsilon$足够小，$f(x)$在$\varepsilon V$中任意小，并且$f$在$x = 0$处连续。

现在让$y$是X的一些点；由于 X 是开放的，因此存在数 $\rho > 1$，使得 $z = \rho y$ 属于到 X。令$g$为中心$z$与$\lambda = 1 - \frac{1}{\rho}$之比位似$x \mapsto \lambda x + (1 - \lambda)z$，其中变换0变为$y$；对于每个点 $g(x) \in g(V)$，我们有 (1)

$$
f(g(x)) \leq \lambda f(x) + (1 - \lambda) f(z) \leq \lambda a + (1 - \lambda) f(z) .
$$

因此，$f$以$y$的邻域为界，因此，通过第一个部分，在$y$处连续。 命题得证。

#### 推论 {#evt-ii-s2-n10-cor-1 .statement tag=07CG}

*在$\mathbf{R}^n$中的开凸集合X上定义的每个凸函数f在X中都是连续的。*

我们可以假设 X 不为空。那么，在X、$n + 1$仿射独立点$a_i$($0 \leq i \leq n$)和这些点、S、包含的凸包络中，存在由点$\sum_{i=0}^n \lambda_i a_i$构成的开非空集，其中$0 < \lambda_i < 1$ 适用于所有 $i$ 和 $\sum_{i=0}^n \lambda_i = 1$。由II，p. 17，道具。 20, $f$ 在 S 中有界，因此是连续的。

在无限维数的拓扑向量空间中，通常存在线性不连续形式（II，p. 80，练习25），因此存在凸函数，它们在任何点都不连续。

### 11. 半范数和凸集合

令 E 为向量空间大于 $\mathbf{R}$； $\mathbf{R}$ 中 E 的映射 $p$ 是*正齐次*，如果对于每个 $\lambda \geq 0$ 和所有 $x \in E$ 我们有

$$
p(\lambda x) = \lambda p(x) .
$$

E 上的正齐次函数 $p$ 是凸的，当且仅当它对于 E 的所有 $x, y$ 满足 II、p. 1 的公理 (SN$_{\text{II}}$)；

$$
p(x + y) \leq p(x) + p(y) .
$$

事实上，如果 $p$ 是凸的，那么对于 E 中的 $x, y$，

$$
p(\frac{1}{2}(x + y)) \leq \frac{1}{2}p(x) + \frac{1}{2}p(y)
$$

并且，根据(5)，该关系等价于(6)。相反，如果 (6) 成立，那么对于所有 $\lambda$ 也有 $0 < \lambda < 1$，

$$
p(\lambda x + (1 - \lambda) y) \leq p(\lambda x) + p((1 - \lambda) y) = \lambda p(x) + (1 - \lambda) p(y)
$$

使用(5)。

E 上的凸正齐次函数称为*次线性*。

如果$p$是定义在E上的次线性函数；然后，通过II, § 2.8，推论，对于点$x \in E$的所有$a > 0$，集合$V(p, a)$（分别$W(p, a)$），其中$p(x) \leq a$（分别$p(x) < a$）是凸的；此外，这个集合是*吸收性的*，因为对于所有$x \in E$，存在$\lambda > 0$使得$p(\lambda x) = \lambda p(x) < a$。

此结果的部分逆命题：

#### 命题 22 {#evt-ii-s2-prop-22 .statement tag=07CH}

*设 A 为凸集合、包含 0，位于向量空间 E 中。对于所有 $x \in E$，输入*

$$
p_A(x) = \inf_{\rho > 0, x \in \rho A} \rho
$$
（0$\leq p_A(x) \leq \infty$）。 *函数$p_A$满足*
$$
p_A(x + y) \leq p_A(x) + p_A(y), \qquad p_A(\lambda x) = \lambda p_A(x)
$$
*适用于 E 中的所有 $x, y$ 和 $\lambda > 0$。如果$V(p_A, \alpha)$（或$W(p_A, \alpha)$）表示集合 / $x \in E$，其中$p_A(x) \leq \alpha$（或$p_A(x) < \alpha$），则*
$$
W(p_A, 1) \subset A \subset V(p_A, 1).
$$
*如果 A 是吸收性的，则 $p_A$ 是有限的*（因此 *次线性*）。

由于当 $\lambda > 0$ 时，关系 $x \in \rho A$ 和 $\lambda x \in \lambda \rho A$ 是等价的，因此对于 $\lambda > 0$，我们有 $p_A(\lambda x) = \lambda p_A(x)$。令$x, y$为E的两个点。如果$x$（或$y$）不被A吸收，则$p_A(x) = +\infty$（或$p_A(y) = +\infty$）和不等式$p_A(x + y) \leq p_A(x) + p_A(y)$显然为真。假设存在$\alpha > 0, \beta > 0$使得$x \in \alpha A$和$y \in \beta A$；然后 $x + y \in \alpha A + \beta A = (\alpha + \beta) A$ (II, p. 8, *注*);因此$p_A(x + y) \leq p_A(x) + p_A(y)$。包含$A \subset V(p_A, 1)$显然是正确的。由于 A 是凸的且包含 0，所以包含$W(p_A, 1) \subset A$。最后，如果 A 是吸收性的，则 $p_A$ 显然是有限的。

由（7）定义的函数$p_A$称为凸集合A的*规范*。如果A是吸收性且对称的，则$p_A$是半范数。

#### 命题 23 {#evt-ii-s2-prop-23 .statement tag=07CI}

*设 E 为拓扑向量空间。如果 A 是开凸集合，其中包含 0，则 $p_A$ 是有限且连续的，并且 $A = W(p_A, 1)$。如果 A 是闭凸集合包含 0，则 $p_A$ 是下半连续且 $A = V(p_A, 1)$。*

如果 A 开且包含 0，则它是吸水性的。对于$x \in A$，存在$\rho < 1$使得$x / \rho \in A$，因此存在$p_A(x) < 1$；与 (9) 结合得到 $A = W(p_A, 1)$。由于凸函数 $p_A$ 的边界在开集合 A 中，因此它在 E 中是连续的（II，p. 18，命题 21）。

假设 A 是闭合的并且包含 0。对于每个 $x \in E$ 和 $p_A(x) \leq 1$，对于所有 $\rho > 1$，我们有 $x \in \rho A$，因此由于 A 是闭合的，因此有 $x \in A$；记住(9)，这表明$A = V(p_A, 1)$。对于所有$\mu > 0$，$\mu A$因此是$x$的集合，使得$p_A(x) \leq \mu$；如E中的$p_A(x) \geq 0$，这表明$p_A$在E中是下半连续的（GT，IV, § 6.2）。

E 上的正次线性函数 $p$ 是每个凸面集合 A 的规格，其中 $W(p, 1) \subset A \subset V(p, 1)$。

### 习题 {#evt-ii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
