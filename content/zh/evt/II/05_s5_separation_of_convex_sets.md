---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 5
section_title: Separation of convex sets
lang: zh
source: evt-i-v
book_pages: TVS II.36-TVS II.40, TVS II.76-TVS II.81
pdf_pages: 0073-0077, 0113-0118
extraction: ocr
subsections:
    - "no": 1
      title: The Hahn-Banach theorem (geometric form)
      page: 36
      pdf_page: 73
    - "no": 2
      title: Separation of convex sets in a topological vector space
      page: 37
      pdf_page: 74
    - "no": 3
      title: Separation of convex sets in a locally convex space
      page: 38
      pdf_page: 75
    - "no": 4
      title: Approximation to convex functions
      page: 39
      pdf_page: 76
statements: 24
exercises: 30
content_sha256: c10f080849a1b5775a80c43cae1fe0dbdb75bcc259eec1fbf1c699f77d98bb8f
translated_from: content/en/evt/II/05_s5_separation_of_convex_sets.md
translation_method: google
source_content_sha256: 497d18fc81f060c697d16f5bff7ad7d5e4bacb2a2d64dfc57ebdfcc324868bea
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: eaf263803596546550637881ca3cb9ef4f1390ed9878dde23789c8e9d489fdfd
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 5。凸面分离集合

### 1. Hahn-Banach 定理（几何形式）

#### 定理 1（哈恩-巴纳赫）{#evt-ii-s5-thm-1 .statement tag=07FI}

— *设 A 为拓扑向量空间 E 的开凸非空集，并令 M 为不满足 A 的非空线性簇。则存在闭超平面 H，其中包含 M 且不满足 A。*

通过翻译，问题可以简化为$0 \in A$，因此$A$是吸收性的。 令 $p$ 为$A$ (II, p. 20) 的*规格*，使得$A$ 为点 $x \in E$ 的集合，从而$p(x) < 1$。 另一方面，令$V$为$M$生成的$E$的向量子空间；因此$M$是$V$中的超平面，而不是包含$0$，因此$V$上有一个唯一的线性形式$f$，使得$M$是点的集合 $y \in V$ $f(y) = 1$。 因此，假设$M \cap A = \varnothing$意味着对于所有$y \in V$（其中$f(y) = 1$），我们有$p(y) \geqslant 1$；由于 $f$ 和 $p$ 是正齐次的，因此对于所有 $y \in V$，我们有 $f(y) \leqslant p(y)$，使得 $f(y) > 0$；最后，对于所有$y \in V$，我们看到$f(y) \leqslant p(y)$对于所有$p(y) \geqslant 0$，对于*所有*$y \in V$。 通过 Hahn-Banach 定理 (II, p. 22, 第 1) 的分析形式，$E$ 上存在线性形式 $h$，其中扩展 $f$ 并且对于所有 $x \in E$， $h(x) \leqslant p(x)$。 令 $H$ 为 $E$ 中的超平面，并使用等式 $h(x) = 1$。 显然$H \cap V = M$和$H \cap A = \varnothing$。 另一方面，$E$包含中$H$的补集是开非空集$A$，因此$H$在$E$（I，p. 11，推论）中是“闭”的。

Q.E.D.

#### 注 1 {#evt-ii-s5-n1-rem-1 .statement tag=07FJ}

当$0 \in M$时，th。 1 可以表述如下：E* 中存在*连续的线性形式，*使得* $g(x) = 0$ *in* $M$ *和* $g(x) > 0$ *in* $A$（II，p. 8，命题 4）。

#### 注 2 {#evt-ii-s5-n1-rem-2 .statement tag=07FK}

如果我们应用定理 1 到 $E$ 带有最好的局部凸拓扑 (II, p. 25, *例* 2)，并且如果为了简单起见，我们假设 $0 \in A$，那么我们得到以下结果（表面上不涉及拓扑) : 如果$A$是实向量空间$E$中的*吸收性*凸集合，并且如果$M$是不满足$A$的非空线性簇，则存在超平面$H$包含于 $M$ 且$A$ 位于$H$ 的一侧。此结果不适用于每个凸集合 $A$（II、p. 65、练习 5）。

### 2. 拓扑向量空间中凸集合的分离

#### 定义 1 {#evt-ii-s5-def-1 .statement tag=07FL}

— *真实拓扑向量空间* $E$ *的两个非空集合* $A, B$ *被认为由闭超平面* $H$ *if* $A$ *包含在由* $H$ *和*确定的闭半空间之一中$B$ *包含在另一个封闭的半空间中*。

#### 定义 2 {#evt-ii-s5-def-2 .statement tag=07FM}

— *实拓扑向量空间的两个非空集合* $A, B$ *被认为是被闭超平面* $H$ *如果* $A$ *包含在由* $H$确定的开半空间之一中，*并且* $B$ *包含在另一个中打开半空间*。

#### 命题 1 {#evt-ii-s5-prop-1 .statement tag=07FN}

— *设* $A$ *为实拓扑向量空间* $E$中的开非空凸集合，并让* $B$ *为非空凸集合； *如果*$A$*不满足*$B$*则存在一个封闭的超平面将*$A$*与*$B$分开。

对于集合 $C = A - B$ 是开、凸（II、p. 9，道具 7）且非空，也是 $0 \notin C$。通过II、p. 36的定理 1，$E$上存在连续的线性形式$f \neq 0$，使得$C$中存在$f(z) > 0$。然后，对于所有 $x \in A$ 和 $y \in B$，我们有 $f(x) > f(y)$。写$\alpha = \inf_{x \in A} f(x)$； $\alpha$是有限的，我们对所有$x \in A$有$f(x) \geq \alpha$，对所有$y \in B$有$f(y) \leq \alpha$；封闭的超平面 $H$ 与方程 $f(z) = \alpha$ 将 $A$ 与 $B$ 分开。

#### 注 {#evt-ii-s5-n2-rem-1 .statement tag=07FO}

— 1) 超平面 $H$ 不满足 $A$ (II, p. 15, 命题 1; 如果 $A$ 和 $B$ 是两个凸非空*开* 集合不满足则存在闭超平面将 $A$ *严格*与 $B$ 分开。
2) 然而，当$B$不开时，即使$E$是有限维，即使$\overline{A}$不满足$\overline{B}$，也不一定存在将$A$与$B$严格分开的闭超平面。 （II，p. 78，练习 12）。

#### 定义 3 {#evt-ii-s5-def-3 .statement tag=07FP}

— *对于向量空间* $E$的子集* $A$ *，*超平面* $H$ *被称为* $A$的支撑超平面，*如果* $H$ *包含至少有一个点* $A$ *和* $A$ 的所有点 *位于* $H$ 的同一侧。

令$f$为$E$上的线性形式，且与零不相同；如果说方程 $f(x) = \alpha$ 的超平面是$A$ 的支持超平面，则意味着$\alpha$ 是集合 $f(A) \subset \mathbf{R}$ 的最小的或最大的成员。在其他字中，存在与方程$f(x) = 0$的超平面平行的$A$的支持超平面，当且仅当集合$f(A)$的界限之一是有限的并且属于到$f(A)$。

#### 命题 2 {#evt-ii-s5-prop-2 .statement tag=07FQ}

— *让* $A$ *成为拓扑向量空间* $E$的非空紧致子集。 *对于每个闭合的超平面* $H$ *在* $E$，*存在* $A$ *平行于* $H$的支持超平面。

因为，如果$f(x) = \gamma$是$H$的方程，其中$f$是$E$中的连续线性形式，则$f$到$A$的限制是连续的，因此有界并在$A$中达到其界限（GT， IV, § 6.1，第 1)。

这说明$A$存在一两个平行于$H$的支撑超平面；第一种情况只有当$A$完全包含在与$H$平行的超平面中时才会出现。

#### 命题 3 {#evt-ii-s5-prop-3 .statement tag=07FR}

— *在拓扑向量空间* $E$ 中，*令* $A$ *为闭凸集合，且*具有非空内部。然后$A$的每个支撑超平面都被关闭，并且$A$属于的每个边界点到$A$的至少一个支撑超平面。

$A$ 的每个支撑超平面都是封闭的，因为 $A$ 的所有点都在超平面的同一侧（II，p. 15，道具 17）。另外，如果$x_0$是$A$的边界点，则$x_0$不会属于到开非空凸集合$\overset{\circ}{A}$； 之后th。 II、p. 36中的1个存在超平面$H$，且包含$x_0$不满足$\overset{\circ}{A}$。由于 $A$ 是 $\overset{\circ}{A}$ 的闭包（II、p. 14，根据第 1 条到第 16 条），它由第 16 条命题得出。 $H$是$A$的支持超平面的II、p. 15的17。

### 3. 局部凸空间中凸集合的分离

#### 命题 4 {#evt-ii-s5-prop-4 .statement tag=07FS}

— 令$A$为局部凸空间$E$中的闭非空凸集合，并令$K$为$E$中的紧致非空凸集合，且不满足$A$。那么存在一个封闭的超平面$H$，它将$A$与$K$严格分开。

因为$E$中存在0的开凸邻域$V$，使得$A + V$和$K + V$不满足（GT，II, § 4.3，道具4）。由于$A + V$和$K + V$在$E$中是凸且开的，道具。 II、p. 37的1表明，存在一个封闭的超平面$H$，将$A + V$与$K + V$严格分开，$a$更不必说$A$与$K$严格分开。

#### 注 {#evt-ii-s5-n3-rem-1 .statement tag=07FT}

在Hausdorff局部凸空间$E$中，令$A$和$B$为两个不相交的闭非空凸集，如果$E$是有限维的，则存在一个闭超平面将$A$与(II，p. 78，练习13)分开；但当$E$具有无限维数时（II、p. 78、练习10和11），这个结论不一定成立。

#### 推论 1 {#evt-ii-s5-prop-4-cor-1 .statement tag=07FU}

— 在局部凸空间中，每个闭凸集合$A$是其包含的闭半空间的交。

事实上，对于每个点$x \notin A$，都存在一个封闭的超平面，它将$x$与$A$严格分开（使用命题4）。

#### 推论 2 {#evt-ii-s5-prop-4-cor-2 .statement tag=07FV}

— 在 Hausdorff 局部凸空间中，每个紧凸集合 $A$ 都是闭半空间的交，其中包含是由 $A$ 的支持超平面确定的。

对于，设 $x_0 \notin A$； $\{ x_0 \}$ 是闭的，因此存在一个闭的超平面 $H$，它将 $x_0$ 与 $A$ 严格分开（命题 4）；令 $f(x) = \alpha$ 为 $H$ 的方程（$f$ 连续线性形式），并假设 $f(x) > \alpha$ 对于所有 $x \in A$。如果我们放入$\gamma = \inf_{x \in A} f(x)$，$f(x) \geq \gamma$包含$A$定义的半空间，是由方程$f(x) = \gamma$的支持度超平面决定的，而不是包含$x_0$； 从而推论。

有可能，一个不紧且没有内部点的闭凸集合，在局部凸空间中，没有任何闭支撑超平面 (II, p. 86, exerc.18 : cf. 还有 V, p. 71, exerc. 11）。

#### 推论 3 {#evt-ii-s5-prop-4-cor-3 .statement tag=07FW}

— 在局部凸空间中，每个线性簇 $M$ 的闭包是包含 $M$ 的闭包超平面的交。

对于所有$x \notin \overline{M}$，令$H$是一个封闭的超平面，将$x$与$\overline{M}$严格分开；

因此$\overline{M}$平行于$H$；闭合的超平面 $H_1$、包含 $\overline{M}$ 且与 $H$ 平行，则不存在包含 $x$。接下来是推论。

#### 推论 4 {#evt-ii-s5-prop-4-cor-4 .statement tag=07FX}

*设$C$为局部凸空间$E$中的闭凸集合。 $E$的子集$A$包含在$C$中，当且仅当，对于$E$中的每个实值连续仿射函数$u$，使得$u(x) \geqslant 0$对于$C$中的所有$x$，我们有$u(y) \geqslant 0$ 适用于 $A$ 中的所有 $y$。*

条件显然是必要的。反之，我们证明它是充分的；如果点$x \in A$不包含在$C$中，则存在等式$f(z) = \alpha$的闭超平面，严格地将$x$与$C$分开；例如，如果我们假设 $f(x) < \alpha$，则连续仿射函数 $u = f - \alpha$ 与……矛盾假设。

#### 推论 5 {#evt-ii-s5-prop-4-cor-5 .statement tag=07FY}

*在局部凸空间$E$中，顶点$0$的每个凸锥$C$的闭包是由经过$0$的闭超平面确定的闭半空间包含$C$的交。*

对于 $\overline{C}$ 来说，是一个顶点为 $0$ 的凸锥（II，p. 13，道具 14）。对于$x \notin \overline{C}$，存在一个封闭的超平面$H$，它将$x$与$\overline{C}$严格分开（命题4）。现在只需应用以下引理：

#### 引理 1 {#evt-ii-s5-lem-1 .statement tag=07FZ}

— *如果顶点为 $0$ 的圆锥体 $A$ 包含在由超平面 $H$ 确定的开半空间中，则它包含在由超平面 $H_0$ 确定的闭半空间中，该闭半空间与 $H$ 平行并穿过 $0$。*

设$f(z) = \alpha$与$\alpha < 0$为$H$的方程，则$f(z) = 0$为$H_0$的方程。如果存在$z \in A$使得$f(z) < 0$，那么就会存在$\lambda > 0$，使得$f(\lambda z) = \alpha$，并且作为$\lambda z \in A$，这将与假设矛盾。

### 4. 近似凸函数

#### 命题 5 {#evt-ii-s5-prop-5 .statement tag=07G0}

*设$X$为局部凸空间$E$中的闭凸集合。那么$X$中定义的每个下半连续凸函数$f$都是$E$中连续仿射线性函数的限制到$X$的函数族的上包络线。*

对于点$(x, t)$的集合$A \subset E \times \mathbf{R}$，使得$x \in X$和$t \geqslant f(x)$是凸的（II，p. 17，命题19）并且是闭的，因为函数$(x, t) \mapsto f(x) - t$是下半连续的。然后令$x$为$X$中的任意点，并令$a \in \mathbf{R}$满足$a < f(x)$。由科。 II、p. 38中的1，$E \times \mathbf{R}$中存在闭超平面$H$，即包含$(x, a)$且不满足$A$。 $E \times \mathbf{R}$ 上的每个线性连续形式为形式

$$
(z, t) \to u(z) + \lambda t ,
$$

其中$\lambda \in \mathbf{R}$和$u$是$E$上的连续线性形式，因此$H$有一个方程形式$u(z) + \lambda t = \alpha$，而$H$包含$(x, a)$我们有$\alpha = u(x) + \lambda a$。现在点 $(x, f(x)) \in A$ 不会属于到 $H$，因此$\lambda \neq 0$。除以$-\lambda$，如有必要，我们可以将$H$的方程写为$t - a = u(z - x)$。作为$f(x) - a > 0$，因此，对于所有$z \in X$，我们有$f(z) > u(z - x) + a$，这证明了命题。

#### 注 1 {#evt-ii-s5-n4-rem-1 .statement tag=07G1}

它来自道具。 5. $f$是函数的有向*递增*族的上包络线，它是函数的限制到$X$，在$E$中是连续且凸的。

#### 注 2 {#evt-ii-s5-n4-rem-2 .statement tag=07G2}

进一步假设 $X$ 是一个顶点为 0 的封闭凸锥体，并且 $f$ 是*正齐次*。那么$f$是函数族的上层信封，它是$E$中*连续线性形式*的限制到$X$。例如，令$(u_\alpha)$为$E$中的连续仿射线性函数族，其中限制至$X$以$f$作为其上包络线。放入$u_\alpha = v_\alpha + \lambda_\alpha$，其中$\lambda_\alpha \in \mathbf{R}$，并且$v_\alpha$是$E$中的连续线性形式。我们有$\lambda_\alpha = u_\alpha(0) \leq f(0) = 0$。另一方面，如果$x \in X$，对于每个$\mu > 0$，我们有，
$$
\mu^{-1} \lambda_\alpha + v_\alpha(x) = \mu^{-1} (\lambda_\alpha + v_\alpha(\mu x)) = \mu^{-1} u_\alpha(\mu x) \leq \mu^{-1} f(\mu x) = f(x)
$$
因此$u_\alpha \leq v_\alpha \leq f$位于$X$中，因此$f$是$v_\alpha$的上包络线。

#### 注 3 {#evt-ii-s5-n4-rem-3 .statement tag=07G3}

$E$中连续仿射函数的限制到$X$是函数，即$X$中的仿射（即凹凸II、p. 17）；但也有可能在紧凸集合$X \subset E$中存在连续仿射函数，而不是连续仿射函数*in*$E$（II，p. 78，exerc）的限制到$X$。 II，c))。然而：

#### 命题 6 {#evt-ii-s5-prop-6 .statement tag=07G4}

*令 $f$ 为 Hausdorff 局部凸空间 $E$ 的紧凸集合 $X$ 中的上半连续仿射函数。令$L$为$E$中连续仿射函数的限制至$X$的集合； $h \in L$的集合$L'$，使得所有$x \in X$的$h(x) > f(x)$，然后是递减定向，并且其下包络线等于$f$。*

我们可以假设$X$非空。令$u, v$为$L$的两个元素，使得$u(x) > f(x)$和$v(x) > f(x)$适用于所有$x \in X$，并令$b$为常数，即$u$和$v$的上界。令$U$（或$V$）为$X \times \mathbf{R}$的点$(x, t)$的紧凸集合，使得$u(x) \leq t \leq b$（或$v(x) \leq t \leq b$），并令$F$为集合 $(x, t) \in X \times \mathbf{R}$使得$t \leq f(x)$； $F$ 是凸的并且在 $X \times \mathbf{R}$ 内闭合。 $U \cup V$的凸包络$K$不满足$F$，因为$U \cup V$包含在$(x, t) \in X \times \mathbf{R}$的集合中，使得$f(x) < t$、集合是凸的并且不满足$F$。由于$K$是紧致的（II，p. 14，道具15），我们可以通过$E \times \mathbf{R}$中的闭超平面$H$严格地将$F$与$K$分开。对于每个$x \in X$，超平面$H$严格地将$(x, f(x))$与$(x, b)$分开，*因此*在单个点$w(x)$中满足线$\{ x \} \times \mathbf{R}$；因此$H$是连续仿射函数的图，其限制$w$到$X$是$L$的成员，即$u$和$v$的下界并且满足不等式 $w(x) > f(x)$ 对于所有 $x \in X$。这证明集合$L'$是递减有向。 II、p. 39的第5条命题应用于$-f$表明$f$是$L'$的下包络线。

#### 推论 {#evt-ii-s5-n4-cor-1 .statement tag=07G5}

*令$f$为$X$中的连续仿射函数；则存在$L$的元素的序列$(h_n)$在$X$中均匀收敛到$f$。*

对于，道具。 6 和 Dini 的定理（GT，X, § 4.1，第 1）表明，对于所有$n$，都存在$h_n \in L$，使得 $f \leq h_n \leq f + 1/n$。

### 习题{#evt-ii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
