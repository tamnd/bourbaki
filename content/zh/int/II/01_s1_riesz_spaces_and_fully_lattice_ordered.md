---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 1
section_title: Riesz spaces and fully lattice-ordered spaces
lang: zh
source: int-i-vi
pdf_pages: 0025-0032, 0039-0043
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Riesz spaces
      page: 0
      pdf_page: 25
    - "no": 2
      title: Generation of a Riesz space by its positive elements
      page: 3
      pdf_page: 27
    - "no": 3
      title: Fully lattice-ordered spaces
      page: 4
      pdf_page: 28
    - "no": 4
      title: Subspaces and product spaces of fully lattice-ordered spaces
      page: 5
      pdf_page: 29
    - "no": 5
      title: Bands in a fully lattice-ordered space
      page: 6
      pdf_page: 30
statements: 16
exercises: 14
content_sha256: 1f4672f6efffcedc65e4da74ff34866a41855fe267f670a3c6c0729d394b18dc
translated_from: content/en/int/II/01_s1_riesz_spaces_and_fully_lattice_ordered.md
translation_method: google
source_content_sha256: f6de0bc69857035c277cfc2ec3ab4f18a8859401aa3da4819959e20e4920524e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 64ba8c3b90dbb92683bfbf78918b391d3b90770a4f2718c7785a694b1402c060
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。 RIESZ 空间和全格序空间

### 1. 里斯的定义空间

回想一下，在集合 E 上，向量空间结构超过域 $\mathbf{R}$ 和阶结构被认为是兼容的，如果它们满足以下两个公理：

(OVS_I) *关系* $x \leq y$ *意味着* $x + z \leq y + z$ *对于所有* $z \in E$。

(OVS_{II}) *关系* $x \geq 0$ *意味着* $\lambda x \geq 0$ *对于每个标量* $\lambda > 0$。

空间 E，配备这两个结构，称为*有序向量空间*（TVS，II, §2, No. 5）。

Axiom（OVS_I）表示E上的阶结构和加法群结构是兼容的，在其他字中，E配备了这两个结构，是一个*有序的群*（A，VI, §1, No. 1）。

公理 (OVS_I) 意味着关系 $x \leq y$ 和 $x + z \leq y + z$ 是等价的。类似地，从(OVS_{II})可以得出，对于每个标量$\lambda > 0$，关系$x \leq y$和$\lambda x \leq \lambda y$是等价的，因为$\lambda^{-1} > 0$和关系$\lambda x \leq \lambda y$意味着$\lambda^{-1}(\lambda x) \leq \lambda^{-1}(\lambda y)$。因此，我们可以说，在有序的向量空间中，比率$> 0$的平移和同位是阶结构的自同构；这一事实也由说表达，阶在每个翻译和比率 $> 0$ 的每个位似下都是“不变”。此外，E 的阶结构与阶结构的对称性$x \mapsto -x$ 是同构。

#### 定义 1 {#int-ii-s1-def-1 .statement tag=08JO}

*有序向量空间被认为是 Riesz 空间（或晶格有序向量空间）*$^1$ *如果其阶结构是晶格排序*（也就是说，如果元素的每个对 E 的 $x, y$ 具有上界 $\sup(x, y)$ 和下确界 $\inf(x, y)$ )。$^2$

(1) 也称为“向量格子”。

（2）Borne superérieure（supremum）又译为“最少上界”（S、R、§6、7）。同样，borne inférieure（infimum）也被翻译为“下确界”。

#### 例 {#int-ii-s1-n1-exa-1 .statement tag=08JP}

在任意集合 $A$ 上定义的所有实值函数的空间 $\mathbf{R}^A$ 是 Riesz 空间（对于序关系 $\langle x(t) \leq y(t) \text{ for all } t \in A \rangle$）；例如，在 $A$ 上定义的任意两个实数值函数 $x, y$ 的上界（或下确界）等于映射 $t \mapsto \sup(x(t), y(t))$（或 $t \mapsto \inf(x(t), y(t))$）。

也可以说，Riesz 空间是向量空间 $E$ 配备阶结构，这样，一方面，$E$ 的结构和加法群结构定义 $E$ (A, VI, §1, No. 9) 上的*格序群* 结构，另一方面满足公理 (OVS$_{\mathrm{II}}$)。

因此，格序群的所有性质都适用于Riesz空间；我们将在这里回顾主要的（cf. A，VI, §1，第 9 到 12 个），并指出从公理（OVS$_{\mathrm{II}}$）流出的推论。

我们首先记得写$x^+ = \sup(x, 0)$（$x$的*正部分*）、$x^- = (-x)^+ = \sup(-x, 0)$（$x$的*负部分*）、$|x| = \sup(x, -x)$（$x$的*绝对值*）；然后$x = x^+ - x^-$和$|x| = x^+ + x^-$；这里，这两个关系相当于

$$
x^+ = \frac{1}{2}(|x| + x), \quad x^- = \frac{1}{2}(|x| - x).
$$

关系 $x \leq y$ 相当于 $\langle x^+ \leq y^+ \text{ and } x^- \geq y^- \rangle$。对于任何 $x$ 和 $y$，*三角形不等式* 成立：

(1)
$$
|x + y| \leq |x| + |y|.
$$

根据$> 0$的每位似下阶的不变性，

(2)
$$
\sup(\lambda x, \lambda y) = \lambda \sup(x, y) \quad \text{for all } \lambda \geq 0.
$$

特别是，

(3)
$$
(\lambda x)^+ = \lambda x^+, \quad (\lambda x)^- = \lambda x^- \quad \text{for all } \lambda \geq 0.
$$

另一方面，对于$\lambda < 0$，我们有$(\lambda x)^+ = (-\lambda x)^- = |\lambda| x^-$和$(\lambda x)^- = (-\lambda x)^+ = |\lambda| x^+$；由此可见，对于每个$\lambda \in \mathbf{R}$和每个$x \in E$，

(4)
$$
|\lambda x| = |\lambda| \cdot |x|.
$$

阶在平移下的不变性表明，对于所有$z \in E$，

(5)
$$
\sup(x + z, y + z) = z + \sup(x, y),
$$
从而，特别是，

(6)
$$
\sup(x, y) = x + (y - x)^+ = \frac{1}{2}(x + y + |x - y|).
$$

我们有关系

(7) $\inf(x, y) = -\sup(-x, -y) ,$

(8) $\sup(x, y) + \inf(x, y) = x + y .$

如果 $x, y, z$ 是 $\geq 0$ 则（A，VI, §1, No. 12，命题 11）

(9) $\inf(x + y, z) \leq \inf(x, z) + \inf(y, z) .$

如果 A 和 B 是 E 的两个子集，每个都有一个上界，那么 A + B 也有一个上界，并且

(10) $\sup(A + B) = \sup A + \sup B .$

如果 $\inf(|x|, |y|) = 0$，E 中的两个元素 $x, y$ 被认为是异类$^3$（彼此）；根据(8)，该关系等价于$\sup(|x|, |y|) = |x| + |y|$，并且根据(6)，等价于$||x| - |y|| = |x| + |y|$； 0 是唯一一个与自身无关的元素；对于每个$x \in E$、$x^+$和$x^-$都是外星人，并且可以被表征为唯一的外星人元素$y \geq 0, z \geq 0$使得$x = y - z$。如果$y$与$x$不相容，那么每个$z \in E$使得$|z| \leq |y|$也与$x$不相容。如果$y$和$z$与$x$不相容，那么$|y| + |z|$也不相容，不等式 (9)；特别是，对于每个整数 $n > 0$，$n|y|$ 与 $x$ 是陌生的，由此得出，对于每个标量 $\lambda$，$\lambda y$ 与 $x$ 是陌生的，因为存在整数 $n$ 使得$|\lambda| \leq n$、从而$|\lambda y| \leq n|y|$。如果 E 的子集 A 由与 $x$ 不同的元素组成，并且如果 A 有一个上界，那么该上界也与 $x$ 不同（A，VI, §1, No. 12，第 13 条命题的 Cor.）。

最后，我们有分解引理（A，VI, §1, No. 10，Th.1）：

*如果* $(x_i)_{i \in I}, (y_j)_{j \in J}$ *是 E 的元素* $\geq 0$ *中的两个有限序列，使得* $\sum_{i \in I} x_i = \sum_{j \in J} y_j$，*则存在元素* $\geq 0$ *的有限序列* $(z_{ij})_{(i,j) \in I \times J}$ *，使得* $x_i = \sum_{j \in J} z_{ij}$ *对于所有* $i \in I$，*和* $y_j = \sum_{i \in I} z_{ij}$ *对于所有* $j \in J$。

### 2. 由正元素生成 Riesz 空间

令 E 为有序向量空间； E 的元素 $\geq 0$ 的集合 P 是顶点为 0 的凸锥体，即 (TVS, II, §2, No. 4), 集合使得

$^3$原文为étrangers，又译为“coprime”（A、VI, §1, No. 12）；还使用项“正交”、“不相交的”和“互奇异”。

P + P ⊂ P 和 λP ⊂ P 对于所有 λ > 0。相反，如果在 $\mathbf{R}$ 上的向量空间 E 中，P 是一个顶点为 0 的凸锥体，使得 $P \cap (-P) = \{0\}$（在其他字中，一个*尖的*和*真*凸锥体），人们知道（*loc.cit.*） 关系$y - x \in P$是序关系（表示为$x \leq y$）与E的向量空间结构兼容。为此阶结构到定义a *Riesz空间* 结构对于E，有必要且充分：

$1^\circ$ P 生成 E，即每个 $z \in E$ 都是形式 $y - x$，其中 x 和 y 属于到 P；

$2^\circ$ P满足以下两个条件之一：
a) P 的元素中的每一个对在P中都有上界；
b) P 的元素中的每个对在 P 中都有一个下确界（A，VI, §1, No. 9，命题 8）。

### 3. 完全格序空间

#### 定义 2 {#int-ii-s1-def-2 .statement tag=08JQ}

*如果上面有界的 E 的每个非空子集在 E 中都有上界，则称 Riesz 空间 E 是完全格序的。*

直接的，在完全格序的空间 E 中，下界的每个非空子集在 E 中都有下确界。

#### 例 {#int-ii-s1-n3-exa-1 .statement tag=08JR}

— 1) 如果 A 是在 A 上定义的实值函数的任何集合、空间 $\mathbf{R}^A$ 是完全格序的，则其上界的族的 $\mathbf{R}^A$ 中的上界是其*上包络*（GT，IV, §5, No. 5）。

2) 令F为任意集合； F 上*有界*实值函数的空间$\mathscr{B}(F)$，配备由$\mathbf{R}^F$诱导的阶结构，是完全格序的。然而，如果 F 是拓扑空间，则 F 上*连续*实值函数的空间 $\mathscr{C}(F)$（配有由 $\mathbf{R}^F$ 诱导的阶结构）是一个 Riesz 空间，通常不是完全晶格有序的（cf. 锻炼。13）。考虑例$F = \mathbf{R}$的情况；令I为区间]0, 1[，$\varphi_I$I的特征函数，并令H为连续函数$x(t)$的集合，使得$x \leq \varphi_I$；很明显，H 在 $\mathscr{C}(F)$ 中有界。 函数$\varphi_I$是$x \in H$的*上包络*，但它不是它们在$\mathscr{C}(F)$中的上界，因为$\varphi_I$是下半连续但不连续。让我们证明，事实上，H 在 $\mathscr{C}(F)$ 中没有上界；只要证明，如果$u$是一个连续的函数使得$u \geq \varphi_I$，那么存在一个连续的函数$v \neq u$使得$u \geq v \geq \varphi_I$。现在，$u(0) \geq 1$，因此存在数$\alpha > 0$，使得$u(t) > 0$对应于$-\alpha \leq t \leq 0$；如果 w 是连续函数，零在区间]$-\alpha, 0$ 之外，且在该区间上有 $0 < w(t) < u(t)$，则函数 $v = u - w$ 满足要求。

#### 命题 1 {#int-ii-s1-prop-1 .statement tag=08JS}

*对于有序向量空间 E 来说，它是完全格序的，E 是 Riesz 空间并且它是满足以下两个条件之一是必要且充分的：*

a) *E 的非空子集 A、元素 $\geq 0$ 的由……组成，其上界有界并指向关系 $\leq$，在 E 中有上界；*

b) *每非空子集* $A$、*由……组成 of 元素* $\geqslant 0$ *of* $E$ *并针对关系* $\geqslant$，*有下确界* $E$。

条件显然是必要的。相反，假设 $E$ 是 Riesz 空间满足条件 *a)*。令 $B$ 为上面有界的 $E$ 的非空子集； $B$的有限子集上位的集合$C$由……组成针对关系$\leqslant$；设$a$为$x \in C$的元素和$C_a$集合之一，即$\geqslant a$；如果我们证明$C_a$有上界，那么它也将是$B$的上界。现在，$C_a - a$是元素$\geqslant 0$的集合，以上面为界并指向关系$\leqslant$；因此它有一个上界$b$，因而$a + b$是$C_a$的上界。

另一方面，条件 *b)* 蕴含 *a)*：对于，如果 $F$ 是 $E$ 的元素 $\geqslant 0$ 的非空集合，在上面有界并指向 $\leqslant$，并且如果 $c$ 是上界对于$F$，则$c - F$是元素$\geqslant 0$中的集合，指向$\geqslant$；如果它有下确界$m$，则$c - m$是$F$的上确界。

#### 命题 2 {#int-ii-s1-prop-2 .statement tag=08JT}

— *让* $E$ *成为配备有与其订购的向量空间结构*（TVS，II, §2, No. 7）兼容的 Hausdorff 拓扑的 Riesz 空间。 *如果，对于每个集合* $H \subset E$ *，其上界为关系* $\leqslant$，* $H$ *的 *截面滤波器是收敛的，则* $E$ *是完全格序的*。

事实上，我们知道$H$的截面滤波器的极限是$E$中$H$的上界（TVS，II, §2, No. 7，第18条命题）。

### 4. 全格序空间的子空间和乘积空间

令$E$为完全格序空间，$H$为$E$的线性子空间。由$E$在$H$上诱导的阶结构与$H$的向量空间结构兼容，但如此定义的有序向量空间$H$*不一定是完全晶格有序的空间*。

更准确地说，可能会发生 $H$ 不是 Riesz 空间（示例 2），或者 $H$ 是 Riesz 空间但不是完全格序的：后者是空间 $\mathscr{B}(\mathbf{R})$ 的子空间 $\mathscr{C}(\mathbf{R})$ 的情况（No. 3，例2）。

此外，如果 $H$ 是 Riesz 空间（完全格序或非完全格序），则 $H$ 的两个元素的上界 *in* $H$ 可能与它们的上界 *in* $E$ 不同（Exer. 3 *b*）。最后，$H$可能是完全格序的，$H$的每个*有限*子集的上界在$E$和$H$中是相同的，但是存在$H$的*无限*子集，其上界为$H$，$E$和$H$中的上界是不同的（Exer.13 *f*））。

令$(E_\iota)_{\iota \in I}$为有序向量空间的任意族。回想一下，在乘积空间$E = \prod_{\iota \in I} E_\iota$中，因子空间的序关系的*乘积*序关系是关系$« x_\iota \leqslant y_\iota \text{ for all } \iota \in I »$（S， III, §1, No. 4）。立即验证这个关系与E的向量空间结构兼容； E，配备此结构，称为订购的空间$E_\iota$的乘积空间。

#### 命题 3 {#int-ii-s1-prop-3 .statement tag=08JU}

*令$(E_\iota)_{\iota \in I}$为有序向量空间的族。对于乘积空间 $E = \prod_{\iota \in I} E_\iota$ 是 Riesz 空间 （分别是完全格序的空间），空间 $E_\iota$ 中的每一个都是 Riesz 空间 （分别是完全格序的空间）是充分必要的晶格有序空间).*

让我们只检查完全格序空间的情况。假设所有$E_\iota$都是完全晶格有序的；令$A$为上面有界的$E$的非空子集，并让$a = (a_\iota)$为$A$的上界。对于每个 $\iota \in I$，$\operatorname{pr}_\iota A$ 的上界为 $a_\iota$，因此在 $E_\iota$ 中有一个上界 $b_\iota$；显然$b = (b_\iota)$是$A$在$E$中的上界。

相反，假设 $E$ 是完全晶格有序的。令$A_\kappa$为上面有界的$E_\kappa$的子集，由$x = (x_\iota)$形成的$E$的$A'_\kappa$子集，使得$x_\kappa \in A_\kappa$和$x_\iota = 0$为$\iota \neq \kappa$。 $A'_\kappa$在$E$的上界是直接的，因此有上界$b = (b_\iota)$；通过乘积序关系的定义，对于$\iota \neq \kappa$必然是$b_\iota = 0$，$b_\kappa$是$A_\kappa$的上等，​​从而完成证明。

#### 定义 3 {#int-ii-s1-def-3 .statement tag=08JV}

*令$E$为$E$的有序向量空间、$V$和$W$两个补充线性子空间。有人说$E$是$V$和$W$的有序直和，如果有序向量空间$V \times W$的典范映射$(x, y) \mapsto x + y$到有序向量空间$E$是同构。*

#### 命题 4 {#int-ii-s1-prop-4 .statement tag=08JW}

*对于有序向量空间 $E$ 是两个补充线性子空间 $V, W$ 的有序直和，关系 $x \in V, y \in W, x + y \geq 0$ 隐含$x \geq 0$ 和$y \geq 0$ 是充分必要的。*

由于$x \geq 0$和$y \geq 0$在$E$中暗示$x + y \geq 0$，叙述中的条件表示元素$\geq 0$的$(x, y) \mapsto x + y$变换集合 $V \times W$ 变为集合元素 $\geq 0$ $E$。

### 5. 完全晶格有序的能带空间

#### 定义 4 {#int-ii-s1-def-4 .statement tag=08JX}

*在完全格序空间 $E$ 中，$E$ 的线性子空间 $B$ 如果满足以下条件，则被称为带： 1) 关系 $x \in B, y \in E$ 和 $|y| \leq |x|$ 意味着$y \in B$； 2) 对于 $B$ 的每个非空子集 $X$，其边界在 $E$ 中，$E$ 属于到 $B$ 中$X$ 的上等$\sup X$。*

#### 例 {#int-ii-s1-n5-exa-1 .statement tag=08JY}

在集合$A$上定义的实值函数空间$\mathbf{R}^A$中，函数集合共零子集$M$点 $A$是一支乐队。

#### 注 {#int-ii-s1-n5-rem-1 .statement tag=08JZ}

在空间$\mathbf{R}^A$中，$A$上的有界实值函数的子空间$\mathscr{B}(A)$满足Def的条件1)。 4；此外，对于 $\mathscr{B}(A)$ 的每个子集 $X$，其边界在 *in* $\mathscr{B}(A)$ 之上，$X$ 属于到 $\mathscr{B}(A)$ 的上包络线。然而，如果 $A$ 是无限的，$\mathscr{B}(A)$ 的子集可能会在* $\mathbf{R}^A$ 中*上界，而不会在* $\mathscr{B}(A)$ 中上界，在这种情况下，$\mathscr{B}(A)$ 不是 $\mathbf{R}^A$ 中的带。

它立即来自 Def。 4 如果$B$是$E$中的一个带，那么对于$B$的每个非空子集$X$，其边界在$E$、$\inf X$、属于到$B$。 $E$中的每个带$B$，配备由$E$的带引起的有序向量空间结构，是完全格序的空间，并且对于在$B$中上界的每个子集$X \subset B$，其上界$B$中的$X$与$E$中的上界相同。

完全格序的空间 $E$ 中任何能带族的交也是一个能带。对于每个子集 $M \subset E$，都存在一个 *最小的带* 包含 $M$ （因为 $E$ 本身就是一个带）；该乐队将被称为由 $M$ *生成*的乐队。

完全晶格有序空间中的能带属性取决于以下命题：

#### 命题 5 {#int-ii-s1-prop-5 .statement tag=08K0}

— *令 $E$ 为完全格序空间，$A$ $E$ 由……组成元素 $\geqslant 0$ 的非空子集，使得：1) $A + A \subset A$ 和 2) 关系 $x \in A,\ 0 \leqslant y \leqslant x$ 暗示$y \in A$。令$M$为$E$中的上界集合，其中$A$的子集在$E$的上方有界。在这些条件下，$E$的每个元素$x \geqslant 0$都可以写成形式$y + z$，其中$y \in M$是元素$v \in A$的上等$v \leqslant x$，并且其中$z$ 是元素 $\geqslant 0$，对于 $M$ 的每一个元素都是陌生的。*

无论如何$y \leqslant x$，所以这一切都归结为表明$z = x - y$对于每个元素$t \in A$（No. 1）来说都是陌生的，在其他字中$u = \inf(z, t)$是零。通过假设、$u \in A$和$u \leqslant x - y$，因此$u + y \leqslant x$；对于每个$v \in A$，使得$v \leqslant x$，乘以定义$v \leqslant y$，因此$u + v \leqslant u + y \leqslant x$；从 $u + v \in A$ 到假设，也从 $y$ 到 $u + v \leqslant y$ 到定义；最后，由于$u + y$是元素$u + v$在$E$中的上等，使得$v \in A$和$v \leqslant x$，我们有$u + y \leqslant y$、从而$u \leqslant 0$，从而完成证明。

#### 定理 1（F.里斯）{#int-ii-s1-thm-1 .statement tag=08K1}

— *令$A$为完全格序空间$E$的子集。与$A$的每个元素都是陌生的元素集合$A'$是一个乐队； 元素的带$A''$与$A'$的每个元素都是陌生的，与$A$生成的带相同，$E$是带$A'$和$A''$的有序直和。*

在No. 1中回顾过的外星人元素的属性，以及乐队的定义，立即表明$A'$是一个乐队，因此$A''$也是一个乐队。通过命题 5和定义，$E$的每个元素$x \geqslant 0$可以写成$x = y + z$，$y \in A'$和$z \in A''$，$y$和$z$为$\geqslant 0$；因为$E$的每一个元素都是两个元素$\geqslant 0$之差，所以我们有$E = A' + A''$；另一方面，由于$0$是唯一一个与自身不相容的元素，所以我们有$A' \cap A'' = \{0\}$，这证明$E$是$A'$和$A''$的直和；最后，由于元素、$\geqslant 0$的$E$的$A'$和$A''$的分量是$\geqslant 0$，$E$是$A'$和$A''$的有序直和（No. 4，命题 4）。

仍有待证明 $A''$ 与 $A$ 生成的带 $B$ 相同。现在，$E$是$B$的直和，并且由元素形成的乐队$B'$对于$B$的所有元素来说是陌生的；从$A \subset B$开始，我们有$B' \subset A'$；另一方面，$B \subset A''$和$E$也是$A'$和$A''$的直和；因此必然是$B = A''$，$B' = A'$。

定理1和命题5使得可以给出由$E$的元素的集合生成的带的另一个定义：

#### 命题 6 {#int-ii-s1-prop-6 .statement tag=08K2}

— *令$E$为空间、$E$的完全格序空间、$M$子集，以及$B$由$M$生成的能带。令$M_1$为$E$的元素$\geqslant 0$中的集合，其中每个$\leqslant$是形式$\sum_i |x_i|$中的一些元素，其中$x_i \in M$；设$M_2$为上面有界的$M_1$的子集的上界集合；那么集合 $M_2$ 与 $B$ 元素 $\geqslant 0$ 集合相同。*

显然 $M_2 \subset B$ 乘定义的频带；另一方面，如果$B'$是元素的带，与$M_1$的每个元素都不相交，则定理1表明$E$是$B$和$B'$的有序直和。但命题 5表明，$E$的每个元素$\geqslant 0$是$M_2$的元素和和$B'$的元素、从而命题。

#### 推论{#int-ii-s1-n5-cor-1 .statement tag=08K3}

— *令$a$为完全格序空间$E$的元素，$B_a$由$a$生成的能带，$B'_a$与$a$不同的元素能带。对于$E$的每个元素$x \geqslant 0$，$B_a$中$x$的分量（对于$E$的分解，作为$B_a$和$B'_a$的有序直和）等于$\sup_{n \in \mathbf{N}} (\inf(n|a|, x))$.*

这是从命题 6 开始，应用于 $M = \{a\}$ 和命题 5。

注 $a$ 和 $|a|$ 生成的能带是相同的。如果$a$和$b$是$E$中互不相干的两个元素，并且如果$A$和$B$分别是由$a$和$b$生成的能带，则$A$中的每个元素对于 $B$ 中的每一个元素都是陌生的；因为，$b$属于对于元素的$A'$来说是陌生的$a$，从而$B \subset A'$，并且，到定理1，$A$的每一个元素对于每一个来说都是陌生的元素共 $A'$。

### 习题 {#int-ii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
