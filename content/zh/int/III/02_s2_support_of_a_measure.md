---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 2
section_title: Support of a measure
lang: zh
source: int-i-vi
book_pages: INT III.23-INT III.32, INT III.59
pdf_pages: 0068-0077, 0104-0104
extraction: ocr
subsections:
    - "no": 1
      title: Restriction of a measure to an open set. Definition of a measure by means of local data
      page: 23
      pdf_page: 68
    - "no": 2
      title: Support of a measure
      page: 25
      pdf_page: 70
    - "no": 3
      title: Characterization of the support of a measure
      page: 27
      pdf_page: 72
    - "no": 4
      title: Point measures. Measures with finite support
      page: 29
      pdf_page: 74
    - "no": 5
      title: Discrete measures
      page: 31
      pdf_page: 76
statements: 26
exercises: 5
content_sha256: 479f467e55e9b2cac3d12a9662eeb2490b8c85502092be5a023662341f1779d5
translated_from: content/en/int/III/02_s2_support_of_a_measure.md
translation_method: google
source_content_sha256: 1e58e2cf7e28f71e344d5832fbb288579da1f287b87e4bdbaf8b730a89a6bea7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8e785756ecc2c811f84bc677f5628f9cf55dd98522360c1d9ffb628e67a13838
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。支持某项措施

### 1. 限制的措施到开放的集合。 定义通过本地数据进行测量

令X为局部紧致空间，Y为X中的开集合。 X 的子空间 Y 是局部紧致的，并且在拓扑向量空间 E 中定义的、在 Y 上定义并具有紧致支持的每个连续函数和值，可以通过连续性扩展到所有 X，方法是在 $\mathbf{C}Y$ 上给它值 0；因此，可以用这种方式认同空间 $\mathscr{K}(Y;E)$ 与$\mathscr{K}(X;E)$ 的线性子空间形成，该线性函数具有紧致支撑 * 包含在 * Y 中。 如果 $\mu$ 是X 上的度量，则显然限制的$\mu$到$\mathscr{K}(Y;\mathbf{C})$是Y上的测度，称为$\mu$到开放子空间Y的*限制*，或$\mu$在Y上*诱导*的测度，并表示为$\mu|Y$。根据§1、第5和第6项，$|\mu|$、$\mathscr{R}\mu$和$\mathscr{I}\mu$的限制到Y分别为$|\mu|Y|$、$\mathscr{R}(\mu|Y)$和$\mathscr{I}(\mu|Y)$。如果$\mu$是实数，则根据§1, No. 5的公式(8)，$\mu^+$和$\mu^-$到Y的限制分别为$(\mu|Y)^+$和$(\mu|Y)^-$。

人们立即看出，如果Y和Z是X中的两个开集合，使得$Y \supset Z$，并且如果$\mu|Y$和$\mu|Z$是$\mu$到Y和Z的限制，那么$\mu|Z$也是限制 $\mu|Y$ 到局部紧致空间 Y 的开子空间 Z。

在 Ch. IV, §5, No. 7 我们将把定义推广到Y是X的局部紧凑子空间的情况。

注 Y 上的某个度量 *不一定* 限制 X 上的某个度量（cf. 第 V, §7, No. 2，第 3 条）。

对于例，令Y为$X = \mathbf{R}$的开区间]0,1[； 映射

$$
f \mapsto \int_0^1 \frac{f(x)}{x} dx
$$

是$Y$上的测度，因为$\mathscr{K}(Y; \mathbf{C})$中的每个函数在$\mathbf{R}$中的0邻域上都是零。然而，该措施不能可扩展到$\mathbf{R}$上的措施，因为在相反的情况下，其函数$f \in \mathscr{K}(Y; \mathbf{C})$的限制至集合使得$\|f\| \leq 1$将受到限制；但这是错误的。

然而，我们有以下命题：

#### 命题 1 {#int-iii-s2-prop-1 .statement tag=08MR}

*让*$(Y_\alpha)_{\alpha \in A}$*成为*$X$*的开放覆盖*并假设给定，在每个子空间*$Y_\alpha$，*测量*$\mu_\alpha$，*以这样的方式，对于每个对*$(\alpha, \beta)$，*限制* $\mu_\alpha$ *和* $\mu_\beta$ *到* $Y_\alpha \cap Y_\beta$ *相同。在这些条件下，存在一个且只有一个测度*$\mu$*在*$X$*上，其限制到*$Y_\alpha$*等于*$\mu_\alpha$*对于每个指标*$\alpha$。

首先让我们证明，每个函数$f \in \mathscr{K}(X; \mathbf{C})$都可以写成有限和$f = \sum_i f_i$的形式，其中，对于每个函数$f_i \in \mathscr{K}(X; \mathbf{C})$，都存在指标$\alpha_i$使得$\operatorname{Supp}(f_i) \subset Y_{\alpha_i}$。 如果$K = \operatorname{Supp}(f)$，则存在指标$\alpha_i$（$1 \leq i \leq n$）的有限数，使得$Y_{\alpha_i}$形式覆盖$K$；设 $h_i$ ($1 \leq i \leq n$) 是$X$的映射连续到$[0, 1]$，使得$h_i$的支撑是紧凑的并且包含在$1 \leq i \leq n$的$Y_{\alpha_i}$中，并且使得$\sum_{i=1}^n h_i(x) = 1$在$K$上（§ 1, No. 2，引理1）； 函数$f_i = f h_i$满足要求。 这首先表明，如果存在满足要求的度量$\mu$，那么它是*唯一的*，因为对于每个有限的和$f = \sum_{i=1}^n f_i$，其中$f_i \in \mathscr{K}(Y_{\alpha_i}; \mathbf{C})$，必然是$\mu(f) = \sum_{i=1}^n \mu_{\alpha_i}(f_i)$。 Moreover, we will have shown the existence of a linear form $\mu$ on $\mathscr{K}(X; \mathbf{C})$ whose restriction to each subspace $\mathscr{K}(Y_\alpha; \mathbf{C})$ is $\mu_\alpha$, provided we demonstrate the following property: if $(g_i)_{1 \leq i \leq m}$ and $(h_j)_{1 \leq j \leq n}$ are two finite sequences of functions in $\mathscr{K}(X; \mathbf{C})$ such that $g_i \in \mathscr{K}(Y_{\alpha_i}; \mathbf{C})$ for $1 \leq i \leq m$, $h_j \in \mathscr{K}(Y_{\beta_j}; \mathbf{C})$ for $1 \leq j \leq n$ and
$$
\sum_{i=1}^m g_i(x) = \sum_{j=1}^n h_j(x) = 1
$$
on $K$, then
$$
\sum_{i=1}^m \mu_{\alpha_i}(f g_i) = \sum_{j=1}^n \mu_{\beta_j}(f h_j).
$$
Now,
$$
f g_i = \sum_{j=1}^n f g_i h_j,
$$

从而
$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{i=1}^{m} \sum_{j=1}^{n} \mu_{\alpha_i}(f g_i h_j).
$$
同样，
$$
\sum_{j=1}^{n} \mu_{\beta_j}(f h_j) = \sum_{j=1}^{n} \sum_{i=1}^{m} \mu_{\beta_j}(f g_i h_j).
$$
但由于$f g_i h_j$的支持包含在$Y_{\alpha_i} \cap Y_{\beta_j}$中，所以我们有$\mu_{\alpha_i}(f g_i h_j) = \mu_{\beta_j}(f g_i h_j)$，它建立了我们的断言。

仍有待观察$\mu$是$X$的测度；现在，$X$的每个点都承认一个包含在$Y_\alpha$之一中的紧邻域；因此，结论立即从$\mu$的定义和§1, No. 3的第6条命题得出。

#### 推论（本地化原理）{#int-iii-s2-n1-cor-1 .statement tag=08MS}

— *令$\mu$和$\nu$为$X$的两个度量，并令$(Y_\alpha)$为$X$的开集合族，使得对于$\mu$和$\nu$的每个$\alpha$、限制至$Y_\alpha$是平等的；那么 $\mu$ 的限制和 $\nu$ 到 $Y = \bigcup_\alpha Y_\alpha$ 相等。*

### 2. 支持某项措施

令$\mu$为局部紧致空间$X$的测度，并令$\mathscr{G}$为开集合$U \subset X$的集合，使得$\mu$到$U$的限制为零；它立即从本地化的原理（No. 1，Prop.1）得出，如果$U_0$是集合$U \in \mathscr{G}$的并，那么$U_0$本身属于到$\mathscr{G}$，因此最大的集合 $\mathscr{G}$。

#### 定义 1 {#int-iii-s2-def-1 .statement tag=08MT}

*如果$\mu$是局部紧致空间$X$的测度，则定义是$\mu$的支持，表示为$\operatorname{Supp}(\mu)$，是闭集合与开集合的最大的互补$X$，其中$\mu$中的限制是零。*

说点$x \in X$不支持属于到$\mu$的支持意味着存在$x$的开邻域$V$，使得$\mu$到$V$的限制为零；因此，说$x$属于对$\mu$的支持意味着，对于$x$的*每个*邻域$V$，都存在函数$f \in \mathscr{K}(X; \mathbf{C})$，其支持度包含在$V$中，使得$\mu(f) \neq 0$。

#### 例 {#int-iii-s2-n2-exa-1 .statement tag=08MU}

— 1) 对于$X$的测度为*零*，其支持度为*空*是必要且充分的。
2）勒贝格测度对$\mathbf{R}$的支持是整条线$\mathbf{R}$；因为，它是非空并且在每个翻译下都是不变的。

3) 在$\mathbf{R}$的区间$X = [0,1]$上，考虑可数稠密子集，排列成序列$(a_n)$，并令$\mu$为通过将每个$n \geq 0$的质量$2^{-n}$放置在点$a_n$定义的度量（§ 1, No. 3、例I）。 $\mu$的支持是$X$的全部；例如，令$x$为$X$的任意点，$V$为$x$的邻域，$f$为$X$上的连续实值函数$\geq 0$，在点处等于1 $x$，其支持度包含在$V$（§ 1, No. 2，引理 1）； $y \in V$的集合使得$f(y) > 0$在$X$开放，因此包含点$a_n$，因而$\mu(f) \geq f(a_n)2^{-n} > 0$。

#### 命题 2 {#int-iii-s2-prop-2 .statement tag=08MV}

*对$\mu$措施的支持与对$|\mu|$措施的支持相同；如果$\mu$是真实的，那么它的支持度是措施$\mu^+$和$\mu^-$的支持度的并。*

因为，如果 $\mu$ 的限制到开集合 $U$ 的零是零，那么$|\mu|$ 的限制也是零（当 $\mu$ 为实数时，$\mu^+$ 和 $\mu^-$），反之亦然。

注$\mu^+$和$\mu^-$的支持可以是非空并且*相同*（cf.Ch.V, § 5，Exer.5）。

#### 命题 3 {#int-iii-s2-prop-3 .statement tag=08MW}

*如果 $\mu$ 和 $\nu$ 是局部紧凑空间 $X$ 上的两个测度，使得 $|\mu| \leq |\nu|$，则$\mathrm{Supp}(\mu) \subset \mathrm{Supp}(\nu)$。*

因为，如果 $\nu$ 的限制到开集合的值是零，那么$\mu$ 的值也是零。

#### 命题 4 {#int-iii-s2-prop-4 .statement tag=08MX}

*两项措施的和支持包含在其并支持中。*

因为，如果开放集合的两个小节中的限制是零，那么它们的和中的限制也是如此。

如果$\mu$和$\nu$是两个“正”测度，则$\lambda = \mu + \nu$的支持度“等于”$\mu$和$\nu$的支持度中的并；因为，如果$x_0$是并的点，并且$V$是$x_0$的任意邻域，则存在一个连续的函数$f \geq 0$，其支持包含在$V$中，并且数之一$\mu(f)$，$\nu(f)$为$> 0$； *更不必说*，$\lambda(f) = \mu(f) + \nu(f) > 0$。

#### 命题 5 {#int-iii-s2-prop-5 .statement tag=08MY}

*测量$\mu$的限制对开放集合$U$的支持是$\mu$的支持在$U$上的迹线。*

从定义可以明显看出命题。

#### 命题 6 {#int-iii-s2-prop-6 .statement tag=08MZ}

*局部紧凑空间$X$上的集合措施，其支持包含在封闭的集合$F$中，是$\mathscr{M}(X; \mathbf{C})$的模糊封闭线性子空间。*

因为，它是具有方程 $\mu(f) = 0$ 的模糊封闭超平面的交，其中 $f$ 运行于 $\mathscr{H}(X; \mathbf{C})$ 中的函数的集合，其支持度不与 $F$ 相交。

假设 $X$ *不是紧凑的*：给定 $X$ 上的测量的空间 $\mathscr{M}(X; \mathbf{C})$ 上的过滤器 $\Phi$，我们可以说测量 $\mu$ *沿着* $\Phi$ 无限期后退，如果对于每个紧凑子集 $X$中的$K$，存在集合$M \in \Phi$，使得对于每个度量$\mu \in M$都有$\mathrm{Supp}(\mu) \cap K = \varnothing$。

#### 命题 7 {#int-iii-s2-prop-7 .statement tag=08N0}

— *如果$\Phi$是$\mathscr{M}(X; \mathbf{C})$上的过滤器，使得$\mu$的支持度沿着$\Phi$无限后退，则$\mu$相对于$\Phi$模糊地收敛到0。*

令$f$为$\mathscr{K}(X; \mathbf{C})$中的任意函数，并令$K$为其支持。到假设时，存在集合 $M \in \Phi$，使得对于每个度量 $\mu \in M$，$\operatorname{Supp}(\mu) \cap K = \varnothing$；由此可见，对于所有$\mu \in M$，$\mu(f) = 0$，这证明了命题。

### 3. 措施的支援刻画

到定义时，如果函数 $f \in \mathscr{K}(X; \mathbf{C})$ *不与*测度 $\mu$ 的支持相交，则 $\mu(f) = 0$；但以下更精确的结果是正确的：

#### 命题 8 {#int-iii-s2-prop-8 .statement tag=08N1}

— *令 $\mu$ 为局部紧致空间 $X$ 的测度。对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$，即 $\operatorname{Supp}(\mu)$、$\mu(f) = 0$ 上的零。*

集合$K = \operatorname{Supp}(f)$，$S = \operatorname{Supp}(\mu)$。给定数$\varepsilon > 0$，令$V$为$x \in X$的集合，使得$|f(x)| < \varepsilon$； $V$ 是假设的开集合包含 $S$，因而$CS$ 是紧集 $CV$ 的邻域。由此可见，在 $[0, 1]$ 中存在 $X$ 的连续映射 $h$，在 $CV$ 上等于 1，并且$CS$ 中包含支持（§ 1, No. 2，引理 1）。由于$fh$的支撑不与$S$、$\mu(fh) = 0$相交。另一方面，$f = fh$在$K \cap CV$上，$|fh| \leq |f|$在$X$上，因而$|f - fh| \leq 2\varepsilon$在$X$上，通过$V$的选择。最后观察到存在数$M_K$，使得$|\mu(g)| \leq M_K \|g\|$对于每个函数$g \in \mathscr{K}(X; \mathbf{C})$，其支持度包含在$K$中；因为$f - fh$的支持度包含在$K$、$|\mu(f - fh)| \leq 2M_K \varepsilon$以及$|\mu(f)| = |\mu(f - fh)| \leq 2M_K \varepsilon$中；因为 $\varepsilon$ 是任意的，$\mu(f) = 0$。

#### 推论 1 {#int-iii-s2-prop-8-cor-1 .statement tag=08N2}

— *如果$\mathscr{K}(X; \mathbf{C})$中的两个函数$f, g$在$\operatorname{Supp}(\mu)$上相等，则$\mu(f) = \mu(g)$。*

#### 推论 2 {#int-iii-s2-prop-8-cor-2 .statement tag=08N3}

— *令$\mu$为$X$的正测度；如果$f \in \mathscr{K}(X; \mathbf{C})$使得$f(x) \geq 0$在$\operatorname{Supp}(\mu)$上，那么$\mu(f) \geq 0$。*

对于 $f = |f|$ 于 $\operatorname{Supp}(\mu)$，因此根据推论 1 为 $\mu(f) = \mu(|f|) \geq 0$。

#### 推论 3 {#int-iii-s2-prop-8-cor-3 .statement tag=08N4}

— *令$\mu$为$X$的有界测度；如果$f \in \mathscr{K}(X; \mathbf{C})$使得$|f(x)| \leq a$在$\operatorname{Supp}(\mu)$上，则$|\mu(f)| \leq a \|\mu\|$。*

对于$\operatorname{Supp}(|\mu|) = \operatorname{Supp}(\mu)$，如果$h$是$X$到$[0, 1]$的连续映射，在$\operatorname{Supp}(f)$上等于1并且有紧支撑，那么$|f(x)| \leq ah(x)$在$\operatorname{Supp}(\mu)$上，因此

$$
|\mu|(|f|) \leq a|\mu|(h) \leq a\|\mu\|
$$

由推论2；然后从§ 1, No. 6的公式(13)得出结论。

#### 命题 9 {#int-iii-s2-prop-9 .statement tag=08N5}

— 设$\mu$为$X$的正测度；如果$f$在$\mathscr{K}_+(X)$中是函数，使得$\mu(f) = 0$，则$f$在$\mathrm{Supp}(\mu)$上是零。

令$x$为$X$的点，使得$f(x) > 0$；让我们证明 $x$ 不会属于到 $\mathrm{Supp}(\mu)$。因为，存在$x$和数$a > 0$的紧凑邻域$V$，使得$f(y) \geq a$位于$V$上。如果 $g$ 是任何连续的函数 $\geq 0$，且支持包含在 $V$ 中，让我们证明 $\mu(g) = 0$；事实上，如果一个集合$b = \|g\|$，那么$g \leq bf/a$，从而$\mu(g) \leq b\mu(f)/a = 0$。

#### 命题 10 {#int-iii-s2-prop-10 .statement tag=08N6}

— 令 $\mu$ 为局部紧凑空间 $X$ 的测度；对于每个函数$g \in \mathscr{C}(X; \mathbf{C})$，测度$g \cdot \mu$的支持是点$x \in \mathrm{Supp}(\mu)$的集合的闭包$T$，使得$g(x) \neq 0$。

集合$S = \mathrm{Supp}(\mu)$；让$x_0$是点而不是属于到$T$；存在$x_0$的开邻域$V$，使得在$V \cap S$的每点，$g$是零；如果$f \in \mathscr{K}(X; \mathbf{C})$包含在$V$中的支持，那么$fg$在$S$上是零，因此（命题8）$\mu(gf) = 0$；其他字、$g \cdot \mu$至$V$中的限制为零。

相反，假设$g \cdot \mu$的限制到点$x_0 \in X$的开放邻域$W$是零，让我们证明不存在$g$是$\neq 0$的$W \cap S$的点。事实上，如果存在这样的点$y$，那么就会存在$y$的紧邻域$U$，包含在$W$中，每点$x$，其中$g(x) \neq 0$；但是每个函数$f \in \mathscr{K}(X; \mathbf{C})$包含在$U$中的支持都可以写成$f = gh$，其中$h \in \mathscr{K}(X; \mathbf{C})$包含在$U \subset W$中的支持；然后是$\mu(f) = \mu(gh) = 0$，与假设$y \in S$相反。

注即$T$包含在$\mu$的支持度$S$和$g$的支持度交中，但不一定等于这个交。对于例，如果$X = \mathbf{R}$、$\mu$是点 0和$g(x) = x$处的狄拉克测度，则$g \cdot \mu = 0$甚至是$g$和$\mu$的支持度的虽然交约化到点 0，因此是非空。

#### 推论{#int-iii-s2-n3-cor-1 .statement tag=08N7}

— 在阶中，措施$g \cdot \mu$为零，在$\mu$的支持下，$g$为零是必要且充分的。

#### 命题 11 {#int-iii-s2-prop-11 .statement tag=08N8}

— 每个具有紧凑支持的测度都是有界的。

因为，$|\mu|$也是一个紧支持的测度，因此我们可以将注意力限制在$\mu \geq 0$的情况；如果$h$是$X$到$[0, 1]$的连续映射，具有紧支撑并且在$\mathrm{Supp}(\mu)$上等于1，那么对于每个函数$f \in \mathscr{K}(X; \mathbf{C})$，在$\mathrm{Supp}(\mu)$上都有$|f(x)| \leq \|f\| h(x)$，因此（Prop.2的Cor.2） 8) $\mu(|f|) \leq \mu(h)\|f\|$，证明命题 (§ 1, No. 8)。

### 4. 点措施。 有限支撑的措施

#### 命题 12 {#int-iii-s2-prop-12 .statement tag=08N9}

— 令 $a_i$ ($1 \leq i \leq n$) 在局部紧凑的空间 $X$ 中与点不同。 $X$上的每一项措施，其支持包含在$a_i$的集合中，是措施$\varepsilon_{a_i}$（$1 \leq i \leq n$）中的线性组合。

因为，对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$ 满足 $n$ 关系 $f(a_i) = 0$，这样的测度$\mu$ 就是零（No. 3，第 8 条）；因为这些关系可以写成$\varepsilon_{a_i}(f) = 0$，所以$\mu$是$\varepsilon_{a_i}$的线性组合（A，II, §7, No. 5，Th.7的Cor.1）。

特别是，每项支持度为空或减少为单个点$x$的措施均为形式$\alpha \varepsilon_x$，其中$\alpha$为复数；这样的措施被称为*点措施*；因此，每个支持有限的测度都是点测度中的和。

#### 定理 1 {#int-iii-s2-thm-1 .statement tag=08NA}

— *每项措施* $\mu$ *在局部紧凑的空间* $X$ *都处于向量空间* $V$ *的模糊闭包中，其支持是有限的并包含在* $\mathrm{Supp}(\mu)$中。

只需证明$\mu$与$\mathscr{K}(X; \mathbf{C})$正交于$V$（TVS，II, §6, No. 3，Th.1的Cor.2）的子空间$V^\circ$正交，即关系$\langle f, \varepsilon_a \rangle = 0$，其中$a$跑过$\mu$的支撑，暗示$\langle f, \mu \rangle = 0$；但这只是No. 3的第8条命题。

#### 推论 1 {#int-iii-s2-thm-1-cor-1 .statement tag=08NB}

— *每个有界测度* $\mu$ *在* $X$ *上都处于凸集合* $A$ *测度的模糊闭包中，其支持是有限的并且包含在* $\mu$的支持中，*其范数是* $\leq \| \mu \|$。 *此外，如果*$\nu$*模糊地倾向于*$\mu$*同时保持在*$A$，*那么*$\| \nu \|$*倾向于*$\| \mu \|$。

To prove the first assertion, it suffices to establish that the measure $\mu$ belongs to the polar set of the polar set $A^\circ$ of $A$ in $\mathscr{K}(X; \mathbf{C})$ (TVS, II, §6, No. 3, Th. 1 and §8, No. 4); this means that for $f \in \mathscr{K}(X; \mathbf{C})$, the relations $|\langle f, \varepsilon_a \rangle| \leq 1/\| \mu \|$ for all $a \in \mathrm{Supp}(\mu)$ imply that $|\langle f, \mu \rangle| \leq 1$; but this is a consequence of Cor. 3 of Prop. 8 of No. 3.

为了证明第二个断言，我们注

$$
\liminf_{\nu \to \mu, \nu \in A} \| \nu \| \geq \| \mu \|
$$

因为函数$\nu \mapsto \| \nu \|$对于模糊拓扑来说是下半连续的（§1, No. 9，第15条命题的Cor.4），并且结论是根据$\| \nu \| \leq \| \mu \|$对于$\nu \in A$乘以定义的事实得出的。

#### 推论 2 {#int-iii-s2-thm-1-cor-2 .statement tag=08NC}

— *每个有界测度* $\mu$ *在* $X$ *上都处于集合测度的模糊闭包中，其支持是有限的并包含在* $\mu$ *的支持中，并且其范数等于* $\| \mu \|$。

我们可以假设$\mu \neq 0$。令$V$为模糊拓扑的0的开邻域；对于每个$\varepsilon$使得$0 < \varepsilon < 1$存在，根据Cor. 1，测度$\nu_0$，其支持是有限的并包含在$\mathrm{Supp}(\mu)$中，并且$\nu_0 - \mu \in V$和$\| \mu \| \geq \| \nu_0 \| \geq (1 - \varepsilon) \| \mu \|$。 设定$\nu = (\| \mu \| / \| \nu_0 \|) \nu_0$，我们有$\| \nu \| = \| \mu \|$和$\| \nu - \nu_0 \| \leq \| \mu \|$；对于$\varepsilon$足够小，我们因此有$\nu - \mu \in V + V$、从而的结论。

#### 推论 3 {#int-iii-s2-thm-1-cor-3 .statement tag=08ND}

*$X$上的每个有界正测度$\mu$都处于正测度凸集合的模糊闭包中，其支持是有限的并包含在$\mu$的支持中，并且其范数等于$\| \mu \|$。*

与 Cor 中的推理相同。由图2可知，我们可以将极限自身推导为证明，$\mu$处于由$\mathrm{Supp}(\mu)$中包含的有限支撑和范数$\leq \| \mu \|$的正测度形成的凸集合$B$的模糊闭包中。同样，只需确定 $\mu$ 属于到 $B^\circ$ 的极点集合、$B$ 的极点集合 *在空间* $\mathscr{K}(X; \mathbf{R})$（TVS、II, §6, No. 3、Th.1）；但这意味着对于$f \in \mathscr{K}(X; \mathbf{R})$关系$\langle f, \varepsilon_a \rangle \geq -1 / \| \mu \|$，对于所有$a \in \mathrm{Supp}(\mu)$意味着$\langle f, \mu \rangle \geq -1$，即No. 3的推论，Cor。提案 8 中的第 2 条。

#### 推论 4 {#int-iii-s2-thm-1-cor-4 .statement tag=08NE}

*在空间$\mathscr{M}(X; \mathbf{C})$中，点措施中的集合总计为拓扑严格紧致收敛*（§1, No. 10）。

在圆锥$\mathscr{M}_+(X)$上，严格紧致收敛的拓扑与模糊拓扑（§1, No. 10，命题18）相同，$X$上的每一个测度都可以写成$\mu_1 - \mu_2 + i \mu_3 - i \mu_4$，其中$\mu_j$（$1 \leq j \leq 4$）是正测度；因此，结论是从 Th 得出的。 1.

#### 命题 13 {#int-iii-s2-prop-13 .statement tag=08NF}

*令 $\mu$ 为局部紧致空间 $X$ 的测度。对于点$x_0$到属于到$\mathrm{Supp}(\mu)$，点测量$\varepsilon_{x_0}$处于测量$g \cdot \mu$的集合的模糊闭包中是必要且充分的，其中$g$运行在连续的集合之上函数具有紧凑的支撑，使得 $\| g \cdot \mu \| \leq 1$.*

根据No. 2的第6条命题，条件显然是足够的。要看出它是必要的，假设 $x_0 \in \mathrm{Supp}(\mu)$；考虑 $\mathscr{K}(X; \mathbf{C})$ 中的函数 $f_k$ ($1 \leq k \leq n$) 的有限数，以及任意数 $\delta > 0$；我们要证明存在函数 $g \in \mathscr{K}(X; \mathbf{C})$ 使得 $\| g \cdot \mu \| \leq 1$ 且使得
$$
|f_k(x_0) - \mu(g f_k)| \leq \delta
$$
$1 \leq k \leq n$。令 $U$ 为 $x_0$ 的相对紧邻开邻域，使得 $U$ 上每个 $f_k$ ($1 \leq k \leq n$) 的振荡为 $\leq \delta / 2$。到假设，从$x_0 \in \mathrm{Supp}(\mu)$开始，存在函数$g_0 \in \mathscr{K}(X; \mathbf{C})$，其支持度包含在$U$中，使得$\mu(g_0) \neq 0$；度量$\nu = g_0 \cdot \mu$不是零，因为对于$U$、$\nu(f) = \mu(g_0) \neq 0$上的每个函数$f \in \mathscr{K}(X; \mathbf{C})$等于1。此外，$\nu$是有界的（No. 3，命题11）；

将$g_0$乘以一个标量，我们可以假设$\| \nu \| = 1$。既然如此，设定$\alpha_k = f_k(x_0)$我们可以写，对于$1 \leq k \leq n$和每个函数$h \in \mathscr{K}(X; \mathbf{C})$，

$$
f_k(x_0) - \nu(f_k h) = \alpha_k (1 - \nu(h)) + \nu((\alpha_k - f_k)h) .
$$

由于$\nu$在$U$有支持，我们可以用限制到$U$来认同； 假设 $\| \nu \| = 1$ 那么意味着存在函数 $h \in \mathscr{K}(X; \mathbf{C})$，且支持包含在 $U$ 中，使得 $\| h \| \leq 1$ 且$| \alpha_k (1 - \nu(h)) | \leq \delta / 2$ 对于 $1 \leq k \leq n$。 $U$的定义还表明，对于所有$x \in U$，$| (\alpha_k - f_k(x)) h(x) | \leq \delta / 2$；由于$\| \nu \| = 1$和$\operatorname{Supp}(\nu) \subset U$，因此我们有$| \nu((\alpha_k - f_k)h) | \leq \delta / 2$，所以，设定$g = g_0 h$，

$$
| f_k(x_0) - \mu(g f_k) | \leq \delta \quad \text{for } 1 \leq k \leq n .
$$

这证明了命题，从$\| g \cdot \mu \| = \| (g_0 h) \cdot \mu \| \leq \| g_0 \cdot \mu \| = 1$开始。

#### 推论 {#int-iii-s2-n4-cor-1 .statement tag=08NG}

*令 $\mu$ 为$X$ 的度量。对于$X$上的措施$\nu$处于措施$g \cdot \mu$的集合的模糊封闭中，其中$g$超过$\mathscr{K}(X; \mathbf{C})$，$\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$是必要且充分的。*

对于，$\operatorname{Supp}(g \cdot \mu) \subset \operatorname{Supp}(\mu)$乘No. 3，提案10；因此，对形式$g \cdot \mu$每一个模糊的极限措施的支持也包含在$\operatorname{Supp}(\mu)$中（No. 2，第6号提案）。相反，如果$\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$，则$\nu$是$\operatorname{Supp}(\mu)$（Th.1）中包含的具有*有限*支持的措施的模糊极限，因此属于第13号提案对$g \cdot \mu$措施的集合的模糊封闭。

### 5. 离散措施

#### 命题 14 {#int-iii-s2-prop-14 .statement tag=08NH}

*对于局部紧凑空间$X$上的测度$\mu$作为离散测度（§ 1, No. 3、例I），$\operatorname{Supp}(\mu)$是$X$的离散闭子空间是必要且充分的。*

令 $\mu$ 为 $X$ 上的离散测度，由放置在 $X$ 的离散闭合子空间 $N$ 的点 $x$ 处的质量 $h(x) \neq 0$ 定义；让我们证明$\operatorname{Supp}(\mu) = N$。对于$a \in N$和$a$的每个邻域$V$，都存在函数$f \in \mathscr{K}(X; \mathbf{C})$，其支持包含在$V$中，在点$a$等于1，在其他点等于0 $N$、从而$\mu(f) = h(a) \neq 0$。另一方面，如果$b \notin N$，则存在$b$的邻域$W$不与$N$相交；对于每个函数$g \in \mathscr{K}(X; \mathbf{C})$，在$W$中包含的支持下，我们因此有$\mu(g) = 0$，这证明了$b \notin \operatorname{Supp}(\mu)$。

相反，令 $\mu$ 为度量，使得 $\operatorname{Supp}(\mu)$ 为 $X$ 的离散闭闭子空间 $N$。对于每个$a \in N$，存在$a$的开邻域$V_a$，包含没有$N$的点不同于$a$；因此，$\mu$到$V_a$的限制是支持$\{a\}$的点测度（No. 2，命题5），因此（No. 4，命题12）是形式$h(a)\varepsilon_a$，其中$h(a) \neq 0$。 设定$h(x) = 0$在$\mathbf{C}\mathbf{N}$的点，并用$\nu$表示群众定义的措施$h(x)$，本地化的原理表明$\nu = \mu$。

因此，我们看到在*离散* 空间 $X$ 上，每个度量都是*离散*。

### 习题 {#int-iii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
