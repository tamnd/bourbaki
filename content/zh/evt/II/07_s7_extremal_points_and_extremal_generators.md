---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 7
section_title: Extremal points and extremal generators
lang: zh
source: evt-i-v
book_pages: TVS II.54-TVS II.60, TVS II.87-TVS II.95
pdf_pages: 0091-0097, 0124-0132
extraction: ocr
subsections:
    - "no": 1
      title: Extremal points of compact convex sets
      page: 54
      pdf_page: 91
    - "no": 2
      title: Extremal generators of convex cones
      page: 57
      pdf_page: 94
    - "no": 3
      title: Convex cones with compact sole
      page: 59
      pdf_page: 96
statements: 25
exercises: 41
content_sha256: 138e95c8c081c7aa347704a0ed885a2e7169b29442024bfb9ebbf1077f6672c5
translated_from: content/en/evt/II/07_s7_extremal_points_and_extremal_generators.md
translation_method: google
source_content_sha256: 34250eb8b3431aeea58b08571a7b95394319981a39c9d593e7466689b9edb3b6
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 92f12a47d4428512addec4e7a91bea6111e4b9b5c95623ee120e9e22d095c1ce
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 7。极端点和极端生成元

### 1. 紧凸集合的极值点

#### 定义 1 {#evt-ii-s7-def-1 .statement tag=07IP}

令 $A$ 为仿射空间 $E$ 中的凸集合。如果不存在包含在$A$和包含$x$中的开段，则我们说点$x \in A$是$A$的极值点。

在其他字，关系$x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z$和$0 \leq \lambda \leq 1$意味着$\lambda = 0$或$\lambda = 1$（因此$x = y$或$x = z$）。 This implies that $x$ cannot be the barycentre of a set of $n$ points $x_i$ of $A$ carrying positive masses unless $x$ is one of the $x_i$; for this is just the definition when $n = 2$; for arbitrary $n$ argue by induction on $n$, as $x$ is the barycentre of $x_1$ and of the barycentre $y_1$ of the $x_i$ with $2 \leq i \leq n$, therefore $x$ is identical with $x_1$ or $y_1$, and in the second case it is sufficient to apply the induction hypothesis.

说$x$是$A$的极值点也意味着$A - \{x\}$是凸的。

#### 例 1 {#evt-ii-s7-n1-exa-1 .statement tag=07IQ}

在空间$\mathbf{R}^n$中，球体$S_{n-1}$的所有点都是闭球$B_n$的极值点。对于，如果$\sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1$和$0 < \lambda < 1$，关系
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
仅当
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1.
$$
但这意味着$\sum_i (y_i - z_i)^2 = 0$，因此对于所有$i$来说$y_i = z_i$，这证明了我们的断言。

#### 例 2 {#evt-ii-s7-n1-exa-2 .statement tag=07IR}

在实数（I，p. 4）有界序列的规范空间$\mathscr{B}(\mathbf{N})$中，单位球的极值点为点$x = (\xi_n)$，使得$|\xi_n| = 1$为全部$n$。例如，假设我们对所有 $n$ 有 $|\xi_n| \leq 1$，对一个指标 $p$ 有 $|\xi_p| < 1$。然后我们可以写
$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$
其中 $y$（分别为 $z$）为点，其所有坐标都等于 $x$ 的坐标且具有相同的指标，除了指标 $p$ 的情况，其坐标等于 1（分别为 $-1$）。这表明 $x$ 不是极值，因为我们有 $\|y\| \leq 1$ 和 $\|z\| \leq 1$。相反，如果 $|\xi_n| = 1$ 对于所有 $n$，则 $x$ 是极值，对于关系 $\xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n$ 以及 $|\eta_n| \leq 1,\ |\zeta_n| \leq 1$ 和 $0 < \lambda < 1$ 意味着 $\xi_n = \eta_n = \zeta_n$。

#### 例 3 {#evt-ii-s7-n1-exa-3 .statement tag=07IS}

设$u : E \to E'$是仿射空间$E'$中仿射空间$E$的仿射映射；设$C \subset E,\ C' \subset E'$是两个凸集合，使得$u(C) \subset C'$。如果$x'$是$C'$的极值点并且$x$是$u^{-1}(x') \cap C$的极值点，则$x$是$C$的极值点，正如它从def得出的那样。 1.

#### 命题 1 {#evt-ii-s7-prop-1 .statement tag=07IT}

令$B$为$A$的极值点的集合，Hausdorff局部凸空间$E$中的非空紧致凸集合，并让$f$为$A$及上定义的凸函数半连续。然后$f$在$A$中在$B$的点（至少）之一处达到上界。

使用 $\mathscr{F}$ 表示 A 的子集 X 族*非空、闭集，并且 A 中包含的且满足 X 的每个开段必然位于 X* 中。它具有以下属性；
(i) 属于至 $\mathscr{F}$。
(ii) 点 $a \in A$ 使得 $\{a\} \in \mathscr{F}$，当且仅当 $a$ 是 A 的极值点。
(iii) $\mathscr{F}$ 集合中$(X_\alpha)$ 的每个非空交 X 以及属于至$\mathscr{F}$。

属性 (i)、(ii) 和 (iii) 紧随定义。

(iv) 令$X \in \mathscr{F}$，且令$h$为函数，其在A中是凸且上半连续的；那么X的点的集合 Y，其中限制$h|X$在X达到其上界，使得Y属于到$\mathscr{F}$。

因为，$h|X$在X中是上半连续，在X的至少一个点中，在X上达到其上界$\alpha$（GT，IV, § 6.2，第3）；因此 Y 是非空的，它也是封闭的（GT，IV, § 6.2，道具 1）。另一方面，令 $x, y$ 为 A 的两个不同的点，并令 $z = \lambda x + (1 - \lambda) y$ 为 Y 的点，使得 $0 < \lambda < 1$；作为$Y \subset X$和$X \in \mathscr{F}$，我们有$x \in X$和$y \in X$；另一方面，由于 $h$ 是凸的，我们有

$$
h(z) \leq \lambda h(x) + (1 - \lambda) h(y)
$$

但作为$h(x) \leq \alpha, h(y) \leq \alpha$和$h(z) = \alpha$，必然有$h(x) = h(y) = \alpha$，也就是说$x \in Y$和$y \in Y$。因此$Y \in \mathscr{F}$。

建立这些属性后，令 M 为 $x \in A$ 的集合，其中 $f$ 在 A 中达到其上界；由(iv)，$M \in \mathscr{F}$。另一方面，根据 (iii) 以及 $\mathscr{F}$ 的集合子集或紧集 A 闭合的事实，$\mathscr{F}$ 对于序关系 $\supset$ 是*感应*的。到了。 2 个 S，III, § 2.4，M 包含子集 N，这是 $\mathscr{F}$ 的最小元素。我们将证明 N 由单个点组成，这将完成命题的证明。由于 E 是 Hausdorff 局部凸空间，因此足以证明 E 上的每个连续线性形式 $u$ 在 N 中都是常数（II，p. 38，cor. 1）。现在从(iv)可以得出，$x \in N$的集合$N'$，其中$u|N$在N中达到上界，使得$N'$属于到$\mathscr{F}$；由于 N 在 $\mathscr{F}$ 中最小，因此我们必然有 $N' = N$。

#### 推论 {#evt-ii-s7-n1-cor-1 .statement tag=07IU}

*设 A 为 Hausdorff 局部凸空间 E 中的紧凸集合。则包含的每个闭支撑超平面 H 至少有一个 A 的极值点。*

因为，如果$f(x) = \alpha$是H和A中的$f(x) \leq \alpha$的方程，则应用prop就足够了。 1 至 $f$。

#### 定理 1（克赖因-米尔曼）{#evt-ii-s7-thm-1 .statement tag=07IV}

— *在 Hausdorff 局部凸空间 E 中，每个紧凸集合 A 都是其极值点的集合的闭凸包络。*

设C为A的极值点的集合的闭凸包络；显然$C \subset A$。要看到$A \subset C$，只需证明，如果$u$是仿射线性函数，在E中连续，并且如果$u(x) \geq 0$在C中，则$u(x) \geq 0$也在A中（II，p. 39，cor.4）；但这是从道具得出的。 1 适用于 $-u$。

#### 命题 2 {#evt-ii-s7-prop-2 .statement tag=07IW}

*令 x 为 Hausdorff* 局部凸空间 E 中紧凸凸集合 A 的极值点。那么对于 E 中 x 的每个开邻域 V，在 E 中存在一个开半空间 F，使得 $x \in F \cap A \subset V \cap A$（在其他情况下） 字，开半空间包含 x，形式 A 中 x 的邻域的基本系统）的迹。

对于 E 包含于 x 的每个开半空间 D，集合 $A \cap \overline{D}$ 是 A 中 x 的紧邻域，并且所有这些邻域中的交恰好是点 x（任意两个不同的点可以被闭闭严格分开） 超平面（II，p. 38，命题 4）。根据 GT 的命题 1，I, § 9.2，足以证明集合 $A \cap \overline{D}$ 形式是一个过滤器基。现在如果我们写 $L_D = A \cap (E - D)$， 集合$L_D$是凸的，紧的并且包含在凸集合$A - \{x\}$中；如果$D_1, D_2$是E包含x的两个开半空间，$L_{D_1} \cup L_{D_2}$的凸包络B因此包含在$A - \{x\}$中，但B是； 紧集 (II, p. 14, 命题15)，因此存在一个闭超平面 H，将x与B严格分开(II, p. 38, 命题4)，如果由H和包含 x确定的开半空间是D，那么我们有$L_{D_1} \cup L_{D_2} \subset L_D$，因此$A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2})$。

#### 推论{#evt-ii-s7-n1-cor-2 .statement tag=07IX}

— 在 Hausdorff 局部凸空间中，令 K 为紧凸凸集合 A 的紧子集。则以下条件是等价的。

a) A 是 K 的封闭凸包络线。

b) K 满足 A 的每个集合即交及其支持之一超平面。

c) A 的极值点的 K 包含集合。

a) $\Rightarrow$ b).假设 A 存在一个支持超平面 H，其方程为 $f(x) = \alpha$，使得 $(H \cap A) \cap K = \varnothing$ 并假设，对于例，A 中存在 $f(x) \geq \alpha$。对于假设的所有 $x \in K$，$f(x) - \alpha > 0$ 并且 K 是紧致的，我们有

$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$

因此，K 包含在闭半空间 $f(x) \geq \beta$ 中；因此，K 的封闭凸包络 A 也是如此，这是荒谬的。

b) $\Rightarrow$ c)。假设 A 的极值点 x 不属于到 K； E 中 x 存在邻域 V，使得 $V \cap A \cap K = \varnothing$。但通过道具。 2，我们可以假设V是由超平面H用方程$f(z) = \alpha$定义的开半空间。如果对于例$f(x) > \alpha$，那么对于所有$y \in K$，我们有$f(y) \leq \alpha$，因此K不满足A的交和平行于H的支持超平面$f(z) = \gamma > \alpha$（II，p. 37，道具2）；这是荒谬的。

c) $\Rightarrow$ a)。这是 Krein-Milman 定理的明显推论。

#### 注 1 {#evt-ii-s7-n1-rem-1 .statement tag=07IY}

即使向量空间 E 是紧凸集合的极值点的有限维集合，也不一定是封闭的（II，p. 89，练习11）。

#### 注 2 {#evt-ii-s7-n1-rem-2 .statement tag=07IZ}

如果在非完全Hausdorff局部凸空间中K为紧集，并且A，K的闭凸包络不是紧的，则A的极值点不属于到K（II，p. 87，练习2）。

#### 注 3 {#evt-ii-s7-n1-rem-3 .statement tag=07J0}

在无限维数的 Banach 空间 E 中，中心 0 且半径为 1 的闭球可能不具有任何极值点（II，p. 89，练习 14）。

#### 注 4 {#evt-ii-s7-n1-rem-4 .statement tag=07J1}

如果 A 是 Hausdorff 局部凸空间中的紧凸集合，则可能会发生 A 的极值点不属于到 A 的任何支持超平面（II，p. 78，执行 11）。 定理 1 (II, p. 56) 的证明表明，在任何情况下，A 都是 A 的极值点集合的凸闭包络，其中属于到支撑超平面。

### 2. 凸锥体的极值生成元

令 C 为向量空间 E 中顶点为 0 的凸锥体；显然，除了顶点之外，C中没有其他点可以是极值点；当且仅当 C 是指向且正确的时，顶点是 C 的极值点。

#### 定义 2 {#evt-ii-s7-def-2 .statement tag=07J2}

设C是向量空间E中顶点0的凸锥。如果C中包含的每个开线段，而不是包含0并且与D相交的每个开线段都包含在D中，则称从0开始的半线D⊂C是C的极值生成元。

同样的道理，对于所有 x ∈ D，且 x ≠ 0，如果 y ≠ 0，y' ≠ 0 是 C 的两个点，使得 x = y + y'，则必然是 y ∈ D 且 y' ∈ D。

#### 注 1 {#evt-ii-s7-n2-rem-1 .statement tag=07J3}

令C为E中的尖真凸锥，并考虑E阶结构，其中C为元素≥0的集合（II，p. 12，命题13）；在阶中，E的元素，假设x > 0，属于到C的极值生成元，必要且充分的是，每个元素y≥0，以x为界，是形式λx，其中0≤λ≤ 1：事实上，说 y 上界为 x 意味着 x = y + y'，其中 y' ∈ C, 从而结论如下。

#### 命题 3 {#evt-ii-s7-prop-3 .statement tag=07J4}

在向量空间 E 中，令 C 为顶点为 0 的凸圆锥，令 x₀ ≠ 0 为 C 的点，D 为C 中包含的、源自 0 和包含 x₀ 的半直线。令 H 为超平面包含 x₀，而不是经过到 0。则 D 是 C 的极值生成元当且仅当 x₀ 是 H ∩ C 的极值点。

条件显然是必要的。反之，假设满足；假设有一条线 D' 不是包含 D，经过通过 x₀，并且 D' ∩ C 包含是一个开线段，x₀ 属于到该线段。设y≠0为D'的向量方向；这些假设意味着对于 |λ| 点 (1 + λ)x₀ + μy 属于到 C和|μ|足够小。但是，在由 D 和 D' 确定并带有规范拓扑的平面 P 中，x₀ 是 P ∩ C 的内部点，因此直线 P ∩ H 包含是包含在 H ∩ C 中的开线段，并且 x₀ 属于。这个与……矛盾假设。

#### 定义 3 {#evt-ii-s7-def-3 .statement tag=07J5}

令 C 为 Hausdorff 拓扑向量空间 E 中的凸集合。如果 C 中 A 的补集 C − A 是凸的，C 的紧凸非空集 A 称为 C 的上限。

令 C 为 E 中顶点为 0 的尖凸锥体，并令 A 为 C 的上限。写 B = C − A。对于每条从 0 开始的闭半线 L ⊂ C，集合 L ∩ A 和 L ∩ B 是凸集合，它们是 L 中的补集，其并是 L，并且使得 L ∩ A 是紧的。由于 L ∩ A 至少有半行 L 是非空的，我们看到 0 ∈ A，因此 L ∩ A 是一个闭线段，终点点为 0。如果 A 存在，则 C 是正确的。

#### 命题 4 {#evt-ii-s7-prop-4 .statement tag=07J6}

— 令 C 为 E 中顶点为 0 的尖凸锥体，Hausdorff 局部凸空间。

a) 令 A 为 C 的上限。令 p 为 A 规范的限制到 C (II, p. 20)。 x ∈ C 的集合使得 p(x) ≤ 1 是集合 A。 函数 p 是下半连续的，具有以下性质：
(i) 对于 C 中的任何 x、y，我们有 p(x + y) = p(x) + p(y)。
(ii) 对于任意 x ∈ C 且 λ ∈ R_+^*，我们有 p(λx) = λp(x)。
(iii) 如果 x ∈ C，关系 p(x) = 0 等价于 x = 0。

b) 相反，令 p 为 C 中定义的函数，且值位于 a) 的 [0, +∞]、满足条件 (i)、(ii) 中。设 A 为 x ∈ C 的集合，使得 p(x) ≤ 1。则 A 和 C − A 是凸的。 A 是上限，当且仅当 A 是紧致且非空的。

叙述 b) 是显而易见的。 a) 中所述的属性是注前面的属性的推论。 4和支柱。 22 个 II、p. 20 和道具。 II、p. 20 中的 23 个，除了

$$
p(x + y) \geq p(x) + p(y).
$$

当 x ≠ 0 且 y ≠ 0 时，足以证明最后这一点；因此，我们有 p(x) > 0, p(y) > 0。设 μ、λ 为两个数 > 0，使得 λ < p(x)、μ < p(y)，并用 B 表示 A 在 C 中的补集。我们有 x ε λB，y ε μB，因此 x + y ε λB + μB；根据 B 的凸性，我们有 λB + μB ⊂ (λ + μ)B, 从而 p(x + y) > λ + μ，这意味着上面提到的不等式。

#### 推论 1 {#evt-ii-s7-prop-4-cor-1 .statement tag=07J7}

— 令 C 为 E 中顶点 0 的尖凸锥体，Hausdorff 局部凸空间，令 p 为 A 的规范，C 的上限。 A 的极值点为点 0，并且点 x 位于 C 的极值生成元上，使得 p(x) = 1。

很明显，0 是 A 的极值点。设 x 为 L 上的点，C 的极值生成元，使得 p(x) = 1。令 y、z 为 A 的两个点，使得 x = $\frac{1}{2}(y + z)$。由于 L 是极值，因此我们有 y = λx 和 z = μx，其中 λ 和 μ 数 ≥ 0，使得 $\frac{1}{2}(\lambda + \mu) = 1$、$\lambda = \lambda p(x) = p(y) \leq 1$ 和 $\mu = \mu p(x) = p(z) \leq 1$，由此得出 $\lambda = \mu = 1$，因此 y = z = x；因此，x 是 A 的极值点。反之，设 x ≠ 0 是 A 的极值点。显然 p(x) = 1。设 y、y' 是 C 的两个点，使得 x = y + y'，我们将证明 y、y' 与 x 成正比。不失一般性，我们可以假设数 $\lambda = p(y)$ 和 $\lambda' = p(y')$ 是有限的且 > 0。然后通过 prop 计算$\lambda^{-1}y \in A, {\lambda'}^{-1}y' \in A, \lambda + \lambda' = 1$。 4、(i) 和等式 $x = \lambda(\lambda^{-1}y) + \lambda'({\lambda'}^{-1}y')$ 意味着，通过假设

$$
x = \lambda^{-1}y = {\lambda'}^{-1}y'.
$$

#### 推论 2 {#evt-ii-s7-prop-4-cor-2 .statement tag=07J8}

— C 的每个点，属于到C 的上限，也属于到C 极值生成元的凸封闭包络线并。

这立即来自 cor。 1 和 Krein-Milman 定理（II、p. 55、第 1）。

\* 例。 — 令 X 为局部紧致空间，即 σ 紧致。令 C 为 $\mathscr{M}_+(X)$ 中顶点 0 的闭凸锥，且拓扑为模糊。我们将证明 C 是其大写字母的并。令$(X_n)$为开路的递增序列，相对于X的紧集，其并为X。令 μ 为 C 的元素 $\neq 0$。存在$\alpha_n > 0$使得$\sum_n \alpha_n \mu(X_n) = 1$。

对于每个度量$v \in C$，放入$p(v) = \sum_n \alpha_n v(X_n) \in [0, +\infty]$。 函数 p on C satisfies 条件 (i) and (ii) of prop. 4. It is lower semi-continuous for the vague 拓扑 (INT, IV, 2nd ed., § 1, No. 1, prop. 4). 集合 A of the $\gamma \in C$ such that $p(\gamma) \leq 1$ is therefore closed and non-empty.另一方面，X的每个紧集都包含在$X_n$之一中，因此模糊有界的A也是模糊紧凑的（INT，III，第二版，§ 1, No. 9，道具15）。 集合 A is therefore a cap of C 包含于 μ. \*

#### 命题 5 {#evt-ii-s7-prop-5 .statement tag=07J9}

令 C 为 E 中顶点为 0 的真凸锥，Hausdorff 弱空间；假设C对于由E的一致结构而言是完备的，并且在C中存在0的邻域的可枚举基本系统。那么C就是它的上限的并，并且是它的极值生成元的并的封闭凸包络线。

第二个叙述源自第一个和 cor。 2 上面。使用道具。 II、p. 52、约化、命题中的11个对应于$E = \mathbf{R}^l$和$C \subset \mathbf{R}_+^l$的情况。对于所有$\alpha \in I$，用$f_\alpha$表示E中的投影$pr_\alpha$；那么$f_\alpha$是连续的线性形式。另一方面，令 $(V_n)_{n \in \mathbf{N}}$ 为 C 中 0 的邻域的可枚举基本系统。通过E的拓扑的定义，对于每个$n \in \mathbf{N}$，存在I和数$\varepsilon_n > 0$的有限子集$J_n$，使得$V_n$包含集合 $x \in C$的$W_n$使得$f_\alpha(x) \leq \varepsilon_n$对于所有$\alpha \in J_n$；把$J = \bigcup_{n \in \mathbf{N}} J_n$。令$y \neq 0$为C的点，p为函数$\sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C)$，其中选择$\lambda_\alpha > 0$使得$p(y) = 1$；这是可能的，因为如果$f_\alpha(y) = 0$对于所有$\alpha \in J$，那么$y \in V_n$对于所有$n$，这意味着$y = 0$，这与假设相反。现在我们注，对于所有$\alpha \in I$，函数$f_\alpha|C$在点0连续，因此存在$n \in \mathbf{N}$，使得$f_\alpha$在$W_n$内有界，因此在C上有界函数 $f_\beta|C$ 的有限数的线性组合，其中 $\beta \in J$。由此可知，如果 A 在 $x \in C$ 的集合中，使得 $p(x) \leq 1$，则对于所有 $\alpha \in I$，$f_\alpha$ 在 A 中有界。由于 p 在 C 中是下半连续的，因此 A 在 C 中是闭且非空的，因此是紧的。因为很明显 p 验证了 prop 的条件 (i) 和 (ii)。 II、p. 58 中的 4 个，我们看到 A 是 C 和包含 y 中的上限。

#### 注 2 {#evt-ii-s7-n2-rem-2 .statement tag=07JA}

存在弱完全且无极值生成元 (II, p. 92, 练习 31) 的真凸锥。

### 3. 带有紧凑底部的凸锥体

#### 命题 6 {#evt-ii-s7-prop-6 .statement tag=07JB}

设 E 为 Hausdorff 局部凸空间，K 为 E 中的凸紧集，且不为包含 0。则顶点 0 的最小的尖锥 C，其中包含 $K$ 为 $E$ 中的真凸锥，并且是局部紧且完备的子空间共 $E$；此外，$E$中存在一个闭超平面$H$，它不包含包含0，并且$H$满足$C$中包含的所有起始于0的半线，并且$H \cap C$是紧致的。此外，如果$D$是由$H$确定的半空间包含0，即具有这些属性的闭超平面，则$C \cap D$是$C$的上限，$C$是$\lambda(C \cap D)$的并 $\lambda > 0$。

通过道具。 II、p. 38中的4个，存在一个封闭的超平面$H$，它将0与$K$严格分开。现在，$\{0\}$和$K$的并的凸包络$A$是紧致的（II，p. 14，命题15），并且是$\lambda K$和$0 \leq \lambda \leq 1$的并。由于 0 和 $K$ 严格位于 $H$ 的相对侧，因此对于每个 $x \in K$ 都存在 $\lambda$，使得 $0 < \lambda < 1$ 和 $\lambda x \in H$。由于$C$是$\lambda \geq 1$的$\lambda A$的并，我们看到$H$满足$C$中包含的从0开始的每条半线，并且$H \cap A = H \cap C$是紧凑的。此外，$C$也是$\lambda \geq 0$的$\lambda(H \cap C)$的并；令$C_n$为$0 \leq \lambda \leq n$的$\lambda(H \cap C)$的并。显然$C_n$是$\{0\}$和$n(H \cap C)$的并的凸包络，因此它是紧的。另外，对于所有$x \in E$，在$E$和整数$n$中存在$x$的闭邻域$V$，使得$V \cap C \subset C_n$；事实上，如果$H$由方程$f(z) = \alpha$定义，其中$\alpha > 0$，则足以将$V$取由$nH$和包含0确定的闭半空间，其中$n$比$n\alpha > f(x)$大。这表明$C$是局部紧致的（取$x \in C$），并且它在$E$是封闭的。我们也可以将$K$视为完成$\hat{E}$的子集，因此$C$也在$\hat{E}$中闭合并因此完成。

给定 Hausdorff 拓扑向量空间 $E$ 中的圆锥体 $C$ 和封闭的超平面 $H$，使得 $H$ 不包含，$C$ 和 $C$ 的顶点 $s$ 为最小的顶点为 $s$ 包含 $H \cap C$ 的圆锥体，那么我们称交 $H \cap C$ 圆锥体 $C$ 的“唯一”。命题6表明，在Hausdorff局部凸空间$E$、最小的顶点0、包含的圆锥中，0不属于的紧凸圆锥集合$K$是紧底圆锥，并且每个凸圆锥都有紧底圆锥$S$，局部紧凑且完整。

#### 例 1 {#evt-ii-s7-n3-exa-1 .statement tag=07JC}

$E$、向量空间、有限维中的每一个真闭凸锥，都有一个紧凑的底部。事实上，通过II，p. 52，道具。 11 我们只需要考虑$E = \mathbf{R}^n$和$C = \mathbf{R}_+^n$的情况。如果$(e_i)_{1 \leq i \leq n}$是$\mathbf{R}^n$的典范基，显然，作为$e_i$（$1 \leq i \leq n$）的凸包络的紧凑凸集合是$\mathbf{R}_+^n$的紧凑底。

#### 例 2 {#evt-ii-s7-n3-exa-2 .statement tag=07JD}

\* 如果 $X$ 是紧凑的空间，则 $X$ 上正测量的圆锥体 $\mathscr{M}_+(X)$ 以及模糊的拓扑，是一个具有紧凑底部的圆锥体（INT，III，第二版，§ 1, No. 9，第 15 条第 3 条）。 \*

### 习题 {#evt-ii-s7-exercises}

参见[习题为 § 7](exercises/s7/)。
