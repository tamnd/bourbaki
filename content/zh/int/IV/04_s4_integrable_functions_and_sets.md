---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 4
section_title: Integrable functions and sets
lang: zh
source: int-i-vi
book_pages: INT IV.32-INT IV.59, INT IV.120-INT IV.127
pdf_pages: 0139-0166, 0227-0234
extraction: ocr
subsections:
    - "no": 1
      title: Extension of the integral
      page: 32
      pdf_page: 139
    - "no": 2
      title: Properties of the integral
      page: 34
      pdf_page: 141
    - "no": 3
      title: Passage to the limit in integrals
      page: 36
      pdf_page: 143
    - "no": 4
      title: Characterizations of integrable numerical functions
      page: 37
      pdf_page: 144
    - "no": 5
      title: Integrable sets
      page: 41
      pdf_page: 148
    - "no": 6
      title: Criteria for the integrability of a set
      page: 43
      pdf_page: 150
    - "no": 7
      title: Characterization of bounded measures
      page: 46
      pdf_page: 153
    - "no": 8
      title: Integration with respect to a measure with compact support
      page: 47
      pdf_page: 154
    - "no": 9
      title: Clans and additive set functions
      page: 50
      pdf_page: 157
    - "no": 10
      title: Approximation of continuous functions by step functions
      page: 52
      pdf_page: 159
    - "no": 11
      title: Extension of a measure defined on a family of sets
      page: 53
      pdf_page: 160
statements: 63
exercises: 23
content_sha256: c26abc49852c536d3927b8c7bdcc0356f1926b873b04031269239070403e9e0e
translated_from: content/en/int/IV/04_s4_integrable_functions_and_sets.md
translation_method: google
source_content_sha256: 66721e72e10dd21f47f9c185589d7f3417a3df9407a6866398253f6c67ed1e54
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 9a973d573443afda5308ff5c2082f3d843e0dfe640ba51e58129735d1192ceeb
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 4。 可积函数和集合

### 1. 积分的扩张

从空间 $\mathscr{L}_F^p$ 的定义可以得出，具有紧凑支撑的连续函数的子空间 $\mathscr{K}_F$ 在 $\mathscr{L}_F^p$ 中是“密集”（§ 3, No. 4，默认为 2）。每个连续（对于阶$p$均值收敛的拓扑）线性函数，在$\mathscr{K}_F$上定义，并在*完整的Hausdorff*拓扑向量空间$G$中取其值，因此可以通过连续性*以独特的方式*扩展为连续线性函数在$\mathscr{L}_F^p$上定义，值在$G$中定义（GT、II, § 3, No. 6、Th.2和III, § 3, No. 1、提案3）。

现在，对于每个具有紧凑支持的连续函数 $f$，以及 Banach 空间 $F$ 中的值，我们定义了（在第 III, § 3, No. 1 章中）相对于 $\mu$ 的*积分* $\mu(f) = \int f \, d\mu$，即元素 $F$，我们已经证明了（第 III, § 3, No. 2，第 6 条命题）不等式

$$
\left| \int f \, d\mu \right| \leqslant \int |f| \, d|\mu| = N_1(f).
$$

这个不等式证明了$\mathscr{K}_F$到$F$的线性映射$f \mapsto \int f \, d\mu$对于$\mathscr{K}_F$均值收敛的拓扑是连续的。因此可以通过连续性将其扩展到整个空间$\mathscr{L}_F^1$，我们可以得到以下定义：

#### 定义 1 {#int-iv-s4-def-1 .statement tag=08RY}

*函数属于到 $\mathscr{L}_F^1(X, \mu)$ 被认为对于测度 $\mu$* 可积（或者，再次，它们是 $\mu$ 可积）。 *可积函数$f$的积分（相对于$\mu$）是由定义值在扩张的$f$连续到线性映射$g \mapsto \int g\, d\mu$的$\mathscr{H}_F$的$\mathscr{L}_F^1$变成$F$；它再次表示为$\mu(f)$或$\int f\, d\mu$，或$\int f(x)\, d\mu(x)$或$\int f\mu$，或$\int f(x)\mu(x)$。

#### 例{#int-iv-s4-n1-exa-1 .statement tag=08RZ}

— 令 $X$ 为*离散* 空间，$\mu$ 为 $X$ 的度量，集合 $\alpha(x) = \mu(\varphi_{\{x\}})$ 对于每个 $x \in X$。那么$\mathscr{F}_F^1$中的函数是*可积的*，在其他字$\mathscr{L}_F^1 = \mathscr{F}_F^1$中；此外，对于每个函数 $f \in \mathscr{L}_F^1$，

$$
\int f\, d\mu = \sum_{x \in X} \alpha(x)f(x).
$$

对于，设 $f \in \mathscr{F}_F^1$；我们有 $|\mu|^*(|f|) = \sum_{x \in X} |\alpha(x)| \cdot |f(x)| < +\infty$ (§ 1, No. 3, *例*);对于每个 $\varepsilon > 0$，存在有限子集 $M$ 的 $X$ 使得

$$
\sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon.
$$

函数$g$在点$x \in M$处等于$f$，其中$|f|$是有限的，并且在其他地方等于0，属于到$\mathscr{H}(X; F)$，并且根据已制定的约定，

$$
|\mu|^*(|f - g|) \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

这就证明了$f \in \mathscr{L}_F^1$。另一方面，

$$
\left| \mu(g) - \sum_{x \in X} \alpha(x)f(x) \right| \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

从而第二个断言。

在其他字中，$\mu$可积函数$f$是族$(\alpha(x)f(x))_{x \in X}$是*绝对可和*（GT，IX, §3, No. 6）的函数，并且积分$\int f\, d\mu$是该族的和。

由于$\mu(f)$在$\mathscr{L}_F^1$上连续定义，并且由于它在Hausdorff空间中取其值，因此对于函数，属于到$\mathscr{L}_F^1$中0的闭包，我们有$\mu(f) = 0$，也就是说，是*可以忽略不计的*；如果$f$和$g$是两个*等价*可积函数，则$\mu(f) = \mu(g)$。 其他字、$\mu(f)$的值仅依赖于可积函数$f$的类$\tilde{f}$；它再次表示为$\mu(\tilde{f})$，函数$\tilde{f} \mapsto \mu(\tilde{f})$是$L^1_F$到$F$的连续线性映射。 如果函数$f$，值在$F$中，并且在$X$中几乎所有地方都有定义，等价于可积函数，我们再次说$f$是*可积的*，我们写成$\int f\, d\mu = \mu(\tilde{f})$；一个定义与可积函数和$\overline{\mathbf{R}}$中的值类似，几乎处处定义且有限，及其积分也是如此。

### 2. 积分的性质

#### 命题 1 {#int-iv-s4-prop-1 .statement tag=08S0}

*对于每个正的$\mu$可积数值函数$f$，*

$$
\int f\, d|\mu| = \int^* f\, d|\mu| = N_1(f) \geqslant 0.
$$

因为，$\int f\, d|\mu|$和$N_1(f)$在$\mathscr{L}^1$上连续，并且对于具有紧支撑的每个连续函数$f \geqslant 0$相等；另一方面，$\mathscr{L}^1$中的每个函数$f \geqslant 0$都是具有紧支撑的连续函数$\geqslant 0$的序列的极限（在均值收敛的意义上）（§ 3, No. 5，命题11）； 从而命题。

#### 推论 1 {#int-iv-s4-prop-1-cor-1 .statement tag=08S1}

*对于每个可积函数 $f \in \mathscr{L}^1_F$，$|f|$ 是可积的并且*

$$
\int |f|\, d|\mu| = \int^* |f|\, d|\mu| = N_1(f).
$$

我们将经常使用提案 1 及其 Cor。 1、处理可积函数$\geqslant 0$时，在替换$\int^* f\, d|\mu|$或$N_1(f)$到$\int f\, d|\mu|$。对于例，两个可积函数$f, g$“等价”，$\int |f - g|\, d|\mu| = 0$是充分必要的。

我们记得，对于函数$f$到属于到$\mathscr{L}^p_F$，函数$|f|^{p-1} \cdot f$属于到$\mathscr{L}^1_F$是必要且充分的（§ 3, No. 8，Th.7的Cor.1），即它是可积的；这就是术语 'p-th 幂可积函数' 的原因。而且：

#### 推论 2 {#int-iv-s4-prop-1-cor-2 .statement tag=08S2}

*对于每个函数 $f \in \mathscr{L}^p_F$，数值函数 $|f|^p$ 是可积的并且*

$$
N_p(f) = \left( \int |f|^p\, d|\mu| \right)^{1/p}.
$$

这是从$|f|$属于到$\mathscr{L}^p$（§ 3, No. 5，命题11）和公式（2）这一事实立即得出的。

#### 命题 2 {#int-iv-s4-prop-2 .statement tag=08S3}

— 对于每个可积函数 $f$，

$$
\left| \int f \, d\mu \right| \leq \int |f| \, d|\mu|.
$$

考虑到 (3) 和 $N_1(f)$ 在 $\mathscr{L}_F^1$ 上的连续性，这立即从不等式 (1) 过渡到极限。

#### 定理 1 {#int-iv-s4-thm-1 .statement tag=08S4}

— 设$F$和$G$是两个Banach空间，$u$是$F$到$G$的连续线性映射。对于每个可积函数 $f$ 以及 $F$ 中的值，$u \circ f$ 是可积的并且

$$
\int u(f(x)) \, d\mu(x) = u \left( \int f(x) \, d\mu(x) \right).
$$

我们已经知道$u \circ f$是可积的（§ 3, No. 5，Th.4）； 关系 (6)，对于扩张的原理恒等式，对于每个$f \in \mathscr{H}_F$、扩展、可积函数$f$都有效：因为，$f \mapsto u \circ f$对于均值收敛的拓扑是连续的，如下： 不等式$N_1(u \circ f) \leq \|u\| \cdot N_1(f)$。

#### 推论 1 {#int-iv-s4-thm-1-cor-1 .statement tag=08S5}

— 令 $a'$ 为 $F$ 上的连续线性形式。如果 $f$ 是可积函数，且值在 $F$ 中，则数值函数 $\langle f, a' \rangle$ 可积且

$$
\int \langle f(x), a' \rangle \, d\mu(x) = \left\langle \int f(x) \, d\mu(x), a' \right\rangle.
$$

我们将在第 1 章中看到。 VI, § 1，锻炼者。 7、11和12可以存在函数$f$，其中值位于无限维Banach空间$F$中，使得$\langle f, a' \rangle$对于$F$上的每个连续线性形式$a'$可积，没有$f$ 可积。

#### 推论 2 {#int-iv-s4-thm-1-cor-2 .statement tag=08S6}

— 如果 $a_k$ ($1 \leq k \leq n$) 是 $F$ 中的向量，并且 $f_k$ ($1 \leq k \leq n$) 是可积数值函数，则函数 $f = \sum_{k=1}^n a_k f_k$ 是可积的，并且

$$
\int \left( \sum_{k=1}^n a_k f_k \right) d\mu = \sum_{k=1}^n a_k \int f_k \, d\mu.
$$

### 3. 积分到极限

#### 命题 3 {#int-iv-s4-prop-3 .statement tag=08S7}

— 让 $\mathscr{B}$ 成为 $\mathscr{L}_F^1$ 上的过滤器基。假设存在紧集$K \subset X$，使得对于每个集合$M \in \mathscr{B}$，所有函数$f \in M$都在$K$中得到支持。在这些条件下，如果$\mathscr{B}$均匀收敛于$X$到$f_0$，则函数$f_0$可积且

$$
\int f_0 \, d\mu = \lim_{\mathscr{B}} \int f \, d\mu .
$$

因为，$\mathscr{B}$均值收敛于$f_0$（§ 3, No. 3，命题 4）。

#### 命题 4 {#int-iv-s4-prop-4 .statement tag=08S8}

— 令 $(f_n)$ 为可积数值函数的递增（分别为递减）序列。为了使序列的上（或下）包络$f$可积，$\sup_n \int f_n \, d|\mu| < +\infty$（或$\inf_n \int f_n \, d|\mu| > -\infty$）是必要且充分的，在这种情况下

$$
\int f \, d\mu = \lim_{n \to \infty} \int f_n \, d\mu .
$$

我们极限自己去考虑递增序列。 序列$g_n = f_n + f_1^-$是递增，由可积函数$\geqslant 0$组成；由于其上包络线为 $g = f + f_1^-$，因此从 Th 得出命题。 § 3, No. 6 中的 5 个。

#### 定理 2 {#int-iv-s4-thm-2 .statement tag=08S9}

— 令 $A$ 为指标的集合，通过具有可数基的过滤器 $\mathfrak{F}$ 进行过滤。令$(f_\alpha)_{\alpha \in A}$为可积函数族，对于滤波器$\mathfrak{F}$，几乎处处逐点收敛到函数$f$；如果存在一个数值函数 $g \geqslant 0$，使得 $\int^* g \, d|\mu| < +\infty$ 且对于每个 $\alpha \in A$，$|f_\alpha(x)| \leqslant g(x)$ 几乎无处不在 $X$ 中，则函数 $f$ 是可积的，并且

$$
\int f \, d\mu = \lim_{\mathfrak{F}} \int f_\alpha \, d\mu .
$$

定理源自勒贝格的定理（§ 3, No. 7，第6章的Cor.），因为在叙述的条件下，$f_\alpha$相对于$\mathfrak{F}$收敛于$f$。

#### 推论 1 {#int-iv-s4-thm-2-cor-1 .statement tag=08SA}

— 令$\Omega$为空间的拓扑空间，$\Omega$的$t_0$点承认可数基本邻域系统，将$X \times \Omega$的$f$映射引入$F$，具有以下性质：
a) 对于每个 $t \in \Omega$，函数 $x \mapsto f(x, t)$ 是可积的；
b) 对于每一个$x \in X$，函数$t \mapsto f(x, t)$在$t_0$连续；

c) 存在 t_0 的邻域 U 和在 X 上定义的数值函数 g \geqslant 0，使得对于所有$x \in X$ 和$t \in U$ 都有$\int^* g d|\mu| < +\infty$ 和$|\mathbf{f}(x,t)| \leqslant g(x)$。

在这些条件下，$\Omega$的映射$t \mapsto \int \mathbf{f}(x,t) d\mu(x)$进入F在点$t_0$连续。

#### 推论 2 {#int-iv-s4-thm-2-cor-2 .statement tag=08SB}

— 令$(\mathbf{f}_n)$为可积函数的序列，使得级数与一般的项$\mathbf{f}_n(x)$几乎处处收敛；如果存在函数$g \geqslant 0$使得$\int^* g d|\mu| < +\infty$并且对于每个整数$n$，$\left| \sum_{k=1}^n \mathbf{f}_k(x) \right| \leqslant g(x)$几乎无处不在，那么级数的和$\mathbf{f}(x)$（几乎无处不在定义）与一般项 $\mathbf{f}_n(x)$ 可积且

$$
\int \mathbf{f} d\mu = \sum_{n=1}^\infty \int \mathbf{f}_n d\mu
$$

（“级数的逐项积分”）。

### 4. 可积数值函数的刻画

#### 命题 5 {#int-iv-s4-prop-5 .statement tag=08SC}

— 对于数值函数 $f \geqslant 0$（有限或非有限），X 上的下半连续，要可积，$\int^* f d|\mu| < +\infty$ 是充分必要的。

这一切都归结为证明条件就足够了。 $|\mu|^*(f)$（§ 1, No. 1，定义1）的定义证明，对于每个$\varepsilon > 0$，存在一个连续的函数$g \geqslant 0$，具有紧支持，例如$g \leqslant f$和$|\mu|^*(f) \leqslant |\mu|(g) + \varepsilon$。但 $f - g$ 是下半连续且 $\geqslant 0$，因此 (§ 1, No. 1, Th. 2)

$$
|\mu|^*(f) = |\mu|(g) + |\mu|^*(f - g),
$$

在其他字$N_1(f - g) = |\mu|^*(f - g) = |\mu|^*(f) - |\mu|(g) \leqslant \varepsilon$中，证明$f$是可积的（§ 3, No. 4，命题7）。

#### 推论 1 {#int-iv-s4-prop-5-cor-1 .statement tag=08SD}

— 对于在 X 上上半连续的有限数值函数 $f \geqslant 0$，要可积，$\int^* f d|\mu| < +\infty$ 是充分必要的。

因为，如果$|\mu|^*(f) < +\infty$，则存在下半连续函数$h$，使得$f \leqslant h$和$|\mu|^*(h) < +\infty$； $h - f$处处有定义且下半连续，且$|\mu|^*(h - f) \leqslant |\mu|^*(h) < +\infty$；因此$h - f$是可积的，并且由于$f(x) = h(x) - (h(x) - f(x))$几乎无处不在，所以$f$是可积的。

#### 推论 2 {#int-iv-s4-prop-5-cor-2 .statement tag=08SE}

— 设$\mathbf{H}$为非空集合，针对关系$\leqslant$（分别$\geqslant$），下（或上）半连续可积数值函数；如果

$$
\sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty \quad \text{(resp. } \inf_{f \in \mathbf{H}} \int f \, d|\mu| > -\infty \text{)},
$$

那么 $\mathbf{H}$ 的上（或下）包络线 $g$ 是可积的，

$$
\int g \, d\mu = \lim_{f \in \mathbf{H}} \int f \, d\mu,
$$

和$\int g \, d|\mu| = \sup_{f \in \mathbf{H}} \int f \, d|\mu|$（分别为$\int g \, d|\mu| = \inf_{f \in \mathbf{H}} \int f \, d|\mu|$）。

我们可以将极限应用于下半连续函数的情况； 函数 $f^+$（分别$f^-$），当$f$超过$\mathbf{H}$时，形式有向集合适用于下（或上）半连续的$\leqslant$（或$\geqslant$） 函数$\geqslant 0$；对于$f \in \mathbf{H}$，$f^+$（或$f^-$）的上（或下）包络线等于$g^+$（或$g^-$）。另一方面，可以通过其截面（与其共尾）之一来替换 $\mathbf{H}$，$f \in \mathbf{H}$ 的由……组成 $\geqslant f_0$，对于某些函数 $f_0 \in \mathbf{H}$；然后$\int f^+ \, d|\mu| \leqslant \int f \, d|\mu| + \int f_0^- \, d|\mu|$；因此，我们看到，当$\mathbf{H}$由正函数组成时，我们被简化为证明推论的两个断言。如果$\mathbf{H}$指向$\leqslant$并且由下半连续函数$\geqslant 0$组成，那么我们知道（§ 1, No. 1，Th.1）

$$
|\mu|^*(g) = \sup_{f \in \mathbf{H}} |\mu|^*(f) = \sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty,
$$

因此 $g$ 是下半连续的，可以通过命题 5 进行积分；我们有$\int g \, d|\mu| = \lim_{f \in \mathbf{H}} \int f \, d|\mu|$，并且从$f \leqslant g$开始，还有$\lim_{f \in \mathbf{H}} N_1(g - f) = 0$，这表明$f$相对于$\mathbf{H}$收敛到$g$，从而证明了这种情况下的推论。如果$\mathbf{H}$定向于$\geqslant$并且由上半连续可积函数$f$组成，使得$0 \leqslant f \leqslant f_1$和$f_1 \in \mathbf{H}$，则存在下半连续可积函数$h$使得$f_1 \leqslant h$；我们可以写 $f = h - f'$，其中 $f(x) < +\infty$ 时写 $f'(x) = h(x) - f(x)$，否则写 $f'(x) = 0$。很明显，对于 $\leqslant$，下半连续可积函数 $\geqslant 0$ 的 $f'$ 形式有向集合，其中

$$
\int f' \, d|\mu| \leqslant \int h \, d|\mu| < +\infty;
$$

我们可以将上面已经证明的东西应用到他们身上；如果$g'$是$f'$的上包络，则$h$和$g'$几乎处处有限，因此$h - g'$几乎处处有定义，并且几乎处处等于$g$；由此，在本案中立即得出推论的结论。

#### 推论 3 {#int-iv-s4-prop-5-cor-3 .statement tag=08SF}

— 令 $f$ 为有界数值函数，在 $X$ 上上半连续且具有紧支撑。那么，对于模糊的拓扑，映射$\mu \mapsto \int f\, d\mu$是$\mathscr{M}_+(X)$上的上半连续。

如果$h$在$\mathscr{K}_+(X)$中是函数，使得$|f| \leq h$（章节III, §1, No. 2，引理1）则$0 \leq f + h \leq 2h$，并且由于$f + h$是上半连续的，因此它可以从Cor得出。 1 $f$ 是 $\mu$ - 对于 $X$ 上的每个测度 $\mu$ 可积。而且，$\mu(f) = \mu(h) - \mu(h - f)$和$h - f$是下半连续函数$\geq 0$。由于对于模糊的拓扑（§1, No. 1，命题 4），映射 $\mu \mapsto \mu(h - f)$ 在 $\mathscr{M}_+(X)$ 上是下半连续的，这证明了推论。

#### 定理 3 {#int-iv-s4-thm-3 .statement tag=08SG}

— 对于数值函数 $f \geq 0$ 可积，对于每个 $\varepsilon > 0$，存在一个具有有限值和紧支撑的上半连续函数 $g \geq 0$，以及一个下半连续可积函数 $h$，这样使得$g \leq f \leq h$ 和 $\int (h - g)\, d|\mu| \leq \varepsilon$。

根据可积性的一般标准（§3, No. 4，命题 8）、命题 5 及其推论 1，条件是足够的。让我们证明条件是必要的。如果$f \geq 0$是可积的，那么对于每个$\varepsilon > 0$，都存在函数$u \geq 0$，连续且具有紧支撑，使得$N_1(f - u) \leq \varepsilon/4$。通过$N_1$的定义，这意味着存在下半连续函数$v \geq 0$，使得$|\mu|^*(v) \leq \varepsilon/2$和$|f - u| \leq v$。因此，$-v(x) \leq f(x) - u(x) \leq v(x)$对于所有$x \in X$，并且由于$u(x)$处处有限，因此$(u(x) - v(x))^+ \leq f(x) \leq u(x) + v(x)$对于所有$x \in X$。 函数$g = (u - v)^+$和$h = u + v$满足要求。

#### 推论 {#int-iv-s4-n4-cor-1 .statement tag=08SH}

— 对于每个可积（或可积和 $\geq 0$）数值函数 $f$，存在可积的上半连续函数递增序列 $(g_n)$（或可积，有限值 $\geq 0$，并且有紧支撑），以及下半连续可积函数的递减序列$(h_n)$，这样：
$1^\circ$$g_n(x) \leq f(x) \leq h_n(x)$适用于所有$x \in X$和每个整数$n$；
$2^\circ$ $f(x)$ 几乎处处都等于序列 $(h_n)$ 的下包络线 $h$ 以及序列 $(g_n)$ 的上包络线 $g$；
$3^\circ$$\int f\, d\mu = \lim_{n \to \infty} \int g_n\, d\mu = \lim_{n \to \infty} \int h_n\, d\mu$。

首先假设$f \geq 0$。由 Th. 3 对于每个$n$，存在一个下半连续可积函数$v_n$，以及一个具有有限值和紧支撑的上半连续函数$u_n \geq 0$，使得

$$
u_n \leq f \leq v_n \quad \text{and} \quad \int (v_n - u_n)\, d|\mu| \leq 1/n;
$$

设定$g_n = \sup(u_1, u_2, \ldots, u_n)$和$h_n = \inf(v_1, v_2, \ldots, v_n)$、序列$(g_n)$和$(h_n)$满足要求。因为，由于 $g \leq f$，$g$ 可以通过 No. 3 的命题 4 进行积分，并且由于
$$
\int (f - g_n) d|\mu| \leq \int (v_n - u_n) d|\mu| \leq 1/n
$$
我们有
$$
\int (f - g) d|\mu| = \lim_{n \to \infty} \int (f - g_n) d|\mu| = 0
$$
（No. 3，命题4），证明$f$和$g$是等价的。有人对序列 $(h_n)$ 也有类似的争论。

若$f$不为正，则可将上述应用于$f^+$和$f^-$，则有两个上半连续可积函数递增序列$(g'_n), (g''_n)$，以及两个下半连续递减序列$(h'_n), (h''_n)$ 可积函数，这样：$1^\circ \ g'_n \leq f^+ \leq h'_n,\ g''_n \leq -f^- \leq h''_n;$
$2^\circ \ f^+$（分别$-f^-$）几乎处处等于$g'_n$的上包络线和$h'_n$的下包络线（分别等于$g''_n$的上包络线和$h''_n$的下包络线）；和$3^\circ$：
$$
\int f^+ d\mu = \lim_{n \to \infty} \int g'_n d\mu = \lim_{n \to \infty} \int h'_n d\mu,
$$
$$
-\int f^- d\mu = \lim_{n \to \infty} \int g''_n d\mu = \lim_{n \to \infty} \int h''_n d\mu.
$$
此外，我们可以假设 $g'_n$ 和 $h''_n$ 处处有限；显然序列$g_n = g'_n + g''_n$和$h_n = h'_n + h''_n$满足要求。

#### 例 {#int-iv-s4-n4-exa-1 .statement tag=08SI}

对于 $\mathbf{R}$ 上的每个正测量$\mu$，具有紧凑支撑的每个*步骤函数*都是$\mu$可积的；因为，开（或闭）区间的特征函数是下（或上）半连续的，并且每一步函数是这样的特征函数的线性组合。 It follows that if $\mathbf{f}$ is a *regulated* function on $\mathbf{R}$ with compact support (FRV, II, §1, No. 3), then $\mathbf{f}$ is integrable, because it is the uniform limit of a sequence of step functions $\mathbf{g}_n$ with support contained in a fixed compact set (No. 3, Prop. 3); moreover, $\int \mathbf{f}\, d\mu = \lim_{n \to \infty} \int \mathbf{g}_n\, d\mu$.

特别是，如果将 $\mu$ 视为勒贝格测度，则可以看出，对于每个具有紧支撑的受管制函数 $\mathbf{f}$，整的 $\int \mathbf{f}\, d\mu$ 等于 FRV 中定义的积分 $\int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$，II, §2, No. 1。

#### 注 1 {#int-iv-s4-n4-rem-1 .statement tag=08SJ}

令 $\mathbf{f}$ 为 $\mathbf{R}$ 上的调节函数，可关于勒贝格测度 $\mu$ 整的；则 $|\mathbf{f}|$ 也是可积的（No. 2，命题 1 的 Cor.1），并且设定 $I_n = [-n, n]$、$|\mathbf{f}|$ 是规定的函数 $|\mathbf{f}| \varphi_{I_n}$ 递增序列的上包络线，因此 $\int |\mathbf{f}|\, d\mu = \lim_{n \to \infty} \int_{-n}^{n} |\mathbf{f}(x)|\, dx$通过 Th。 2 个No. 3；因此，整的$\int_{-\infty}^{+\infty} f(x) dx$*绝对收敛*（FRV，II, §2, No. 3）。此外，Th 的$\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$。 No. 3 中的 2 个。反之，假设$\int_{-\infty}^{+\infty} f(x) dx$绝对收敛；再次，Th. 2 个No. 3、$\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$。 注如果积分$\int_{-\infty}^{+\infty} f(x) dx$收敛但不绝对收敛；那么 $f$ *对于勒贝格测度来说是不可积的。

#### 注 2 {#int-iv-s4-n4-rem-2 .statement tag=08SK}

应用于勒贝格测度和调节函数，No. 3 的第 3 条命题在紧凑区间上的调节函数积分到极限时重新产生定理（FRV，II, §3, No. 1，命题 1）；对于*序列*（或具有可数基的过滤器），调节函数，Th。 No. 3的2极大地改进了命题，因为对于紧凑区间上的均匀有界调节函数，它用*逐点*收敛代替*均匀*收敛（cf.§5, No. 4，Th.2）。然而，对于在非紧区间上调节函数的*绝对收敛*积分到极限的过渡，我们注即Th的条件。 No. 3 的 2 意味着所考虑的积分是*一致收敛的*（在 FRV 中定义的意义上，II, §3, No. 2），因此对于IV（*loc.cit.*）中给出的收敛性，不会改进条件，除非涉及函数$f_\alpha$ 在每个紧凑区间上的收敛。最后，对于经过到极限，对于调节的函数的“非绝对收敛”积分给出的条件仍然超出了章中开发的理论。

### 5. 可积集合

#### 定义 2 {#int-iv-s4-def-2 .statement tag=08SL}

*子集* $A$ *局部紧致空间* $X$ *据说对于一个测度是可积的* $\mu$ *在* $X$ *（或者，它是* $\mu$*可积）* *如果特征函数* $\varphi_A$ ** $A$ *可积。* *有限数* $\mu(A) = \int \varphi_A\, d\mu$ *称为* $A$ 的测度。

对于每个可积集合 $A$，$|\mu|(A) = |\mu|^*(A)$（No. 2，命题 1）；为了使集合*可以忽略不计*，它的*测量值零相对于*$|\mu|$是必要且充分的。

#### 命题 6 {#int-iv-s4-prop-6 .statement tag=08SM}

*有限族的并* $(A_i)_{1 \leq i \leq n}$ *可积的集合是可积的，*并且

$$
|\mu| \left( \bigcup_{i=1}^n A_i \right) \leq \sum_{i=1}^n |\mu|(A_i).
$$

*此外，如果* $A_i$ *是成对的不相交的，*那么

$$
\mu \left( \bigcup_{i=1}^n A_i \right) = \sum_{i=1}^n \mu(A_i).
$$

因为，如果 $A = \bigcup_{i=1}^n A_i$ 则 $\varphi_A = \sup \varphi_{A_i}$，因此（§ 3, No. 5，第 12 条命题的证明）如果 $A_i$ 可积，则 $A$ 也可积； 关系 (13) 是外部措施的类似关系的特例（§ 1, No. 4，第 18 条命题），考虑到关系 $|\mu|(A) = |\mu|^*(A)$；最后，如果$A_i$是成对的不相交的，则$\varphi_A = \sum_{i=1}^n \varphi_{A_i}$，从而 (14)。

#### 命题 7 {#int-iv-s4-prop-7 .statement tag=08SN}

1° *如果 A 和 B 是两个可积集合使得 $B \subset A$，则集合 $C = A - B$ 可积并且*

$$
\mu(C) = \mu(A) - \mu(B).
$$

2° *交可积集合的可数族是可积的。*

第一个部分源自$\varphi_C = \varphi_A - \varphi_B$。另一方面，如果$(A_n)$是可积的集合的序列，并且$A$是它的交，则$\varphi_A = \inf_n \varphi_{A_n}$，因此$A$是可积的（No. 3，命题4）。

#### 推论{#int-iv-s4-n5-cor-1 .statement tag=08SO}

*如果 $(A_n)$ 是可积集合的递减序列，则* $\mu(\bigcap_n A_n) = \lim_{n \to \infty} \mu(A_n)$。

因为，如果$A = \bigcap_n A_n$，则$\varphi_A$是递减序列$(\varphi_{A_n})$的下包络线（No. 3，命题4）。

#### 命题 8 {#int-iv-s4-prop-8 .statement tag=08SP}

*令$(A_n)$为可积集合的递增序列；为了使并 $A = \bigcup_n A_n$ 可积，* $\sup_n |\mu|(A_n) < +\infty$ 是必要且充分的，*在这种情况下，*

$$
\mu(A) = \lim_{n \to \infty} \mu(A_n).
$$

对于，可积函数的$\varphi_{A_n}$形式递增序列和$\varphi_A = \sup_n \varphi_{A_n}$；因此，命题是从No. 3的第4条命题得出的。

#### 推论 {#int-iv-s4-n5-cor-2 .statement tag=08SQ}

*令$(A_n)$为可积集合的序列，使得*$\sum_{n=1}^\infty |\mu|(A_n) < +\infty$； *并* $A = \bigcup_n A_n$ *可积，并且*

$$
|\mu| \left( \bigcup_n A_n \right) \leq \sum_{n=1}^\infty |\mu|(A_n).
$$

对于，$\varphi_A = \sup_n \varphi_{A_n}$ 和

$$
|\mu|^*(A) \leq \sum_{n=1}^\infty |\mu|^*(A_n) = \sum_{n=1}^\infty |\mu|(A_n) < +\infty
$$

（§1, No. 4，提案 18）；因此 A 是可积的（§3, No. 6，Th.5 的 Cor.2），并且从 $|\mu|(A) = |\mu|^*(A)$ 开始，我们确实有 (17)。

#### 命题 9 {#int-iv-s4-prop-9 .statement tag=08SR}

— 令 $(A_n)$ 为成对不相交的可积集合的序列，使得 $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$；那么

$$
\mu\left(\bigcup_n A_n\right) = \sum_{n=1}^\infty \mu(A_n).
$$

因为，如果$A = \bigcup_n A_n$则$\varphi_A = \sum_{n=1}^\infty \varphi_{A_n}$，并且命题由(17)和Cor得出。 2 Th。 2 个No. 3。

关系(18)也可以用说来表示，测度$\mu$与$X$的可积子集的集合完全相加。

### 6. 判据集合的可积性

#### 命题 10 {#int-iv-s4-prop-10 .statement tag=08SS}

— 对于 $X$ 中的开（或闭）集合 $A$ 可积，$|\mu|^*(A) < +\infty$ 是充分必要的。

由于 $\varphi_A$ 是下（或上）半连续的，命题由 No. 4 的命题 5 及其推论 1 得出。

#### 推论 1 {#int-iv-s4-prop-10-cor-1 .statement tag=08ST}

— 每个紧集都是可积的；每个相对紧凑的开集合都是可积的。

#### 推论 2 {#int-iv-s4-prop-10-cor-2 .statement tag=08SU}

— 对于 $X$ 上的每个积极措施 $\mu$，$A \mapsto \mu^*(A)$ 是 $X$ 上的容量（cf. GT、IX, §6, No. 9、例）。

#### 例 {#int-iv-s4-n6-exa-1 .statement tag=08SV}

对于 $\mathbf{R}$ 上的勒贝格测度 $\mu$，根据命题 10，每个有界开区间 $[a, b[$ 都是可积的，并且具有测度 $b - a$（\§1, No. 2，命题 9）。由于每个集合减少到点对于勒贝格测度来说可以忽略不计，因此所有具有端点 $a$ 和 $b$ 的区间都具有相同的测度 $b - a$。

#### 命题 11 {#int-iv-s4-prop-11 .statement tag=08SW}

— 令$\mathscr{G}$为集合，指向关系$\subset$，在$X$中可积开集合；为了使$A = \bigcup_{G \in \mathscr{G}} G$可积，$\sup_{G \in \mathscr{G}} |\mu|(G) < +\infty$是必要且充分的，在这种情况下$\mu(A) = \lim_\mathscr{G} \mu(G)$和$|\mu|(A) = \sup_{G \in \mathscr{G}} |\mu|(G)$。

因为，我们知道 $|\mu|^*(A) = \sup_{G \in \mathscr{G}} |\mu|(G)$ (\§1, No. 2，命题 7)；因此，命题由命题 10 得出。

#### 推论{#int-iv-s4-n6-cor-1 .statement tag=08SX}

— 令$\mathfrak{F}$为集合，指向关系$\supset$，在$X$中可积闭集合；则闭集合 $B = \bigcap_{H \in \mathfrak{F}} H$ 可积，且有
$$
\mu(B) = \lim_{\mathfrak{F}} \mu(H) \quad \text{and} \quad |\mu|(B) = \inf_{H \in \mathfrak{F}} |\mu|(H).
$$
例如，令$\mathfrak{F}$中的$H_0$为集合；由于$H_0$是可积的，它包含在可积开集合$U$中（§ 1, No. 4，命题19）； 集合 $U \cap \mathbf{C}H$ 形式集合指向关系 $\subset$，包含在 $U$ 中，并且有并 $U \cap \mathbf{C}B$；因此，我们被简化为提案 11。

#### 定理 4 {#int-iv-s4-thm-4 .statement tag=08SY}

— 为了使集合 $A$ 可积，对于每个 $\varepsilon > 0$，存在可积开集合 $G$ 和紧集 $K$ 是必要且充分的，使得 $K \subset A \subset G$ 和
$$
|\mu|(G - K) = |\mu|(G) - |\mu|(K) \leq \varepsilon.
$$

a) 条件 *足够*，因为它意味着 $\varphi_K \leq \varphi_A \leq \varphi_G$ 和 $\int (\varphi_G - \varphi_K) d|\mu| \leq \varepsilon$；因为 $\varphi_G$ 和 $\varphi_K$ 是可积的，所以 $\varphi_A$ 也是可积的（§ 3, No. 4，第 8 条）。

b) 条件是*必要的*。如果$A$可积，则存在一个开集合$G \supset A$，使得$|\mu|^*(G)$任意接近$|\mu|^*(A) = |\mu|(A)$（§ 1, No. 4，命题19）；因此，这一切都归结为证明，对于每个$\varepsilon > 0$，都存在紧集$K \subset A$，使得$|\mu|(A) - |\mu|(K) \leq \varepsilon$。由于$\varphi_A$是可积的，因此存在函数$f \geq 0$，上半连续且具有紧支撑$S$，使得$f \leq \varphi_A$和$\int (\varphi_A - f) d|\mu| \leq \varepsilon/2$（No. 4，Th.3）。令$\delta > 0$为任意数，并令$K$为点$x \in X$中的集合，使得$f(x) \geq \delta$； $K$ 是封闭的，并且包含在 $S$ 中，因此是*紧凑的*，并且从 $f \leq \varphi_A$ 开始，我们有 $K \subset A$。 集合 $B = A - K$ 可积，且$f \leq \varphi_K + \delta \varphi_B$、从而
$$
\int f d|\mu| \leq |\mu|(K) + \delta \cdot |\mu|(B) \leq |\mu|(K) + \delta \cdot |\mu|(A),
$$
最后
$$
|\mu|(A) \leq \int f d|\mu| + \frac{\varepsilon}{2} \leq |\mu|(K) + \delta \cdot |\mu|(A) + \frac{\varepsilon}{2},
$$
完成证明，因为 $\delta$ 是任意的。

#### 推论 1 {#int-iv-s4-thm-4-cor-1 .statement tag=08SZ}

— 为了使集合$A$可积，对于每个$\varepsilon > 0$，存在紧集$K \subset A$使得$|\mu|^*(A - K) \leq \varepsilon$是充分必要的。那么测度 $|\mu|(A)$ 就是测度 $|\mu|(K)$ 紧集 $K \subset A$ 的集合的至高。

条件是必要的，因为如果$G$和$K$满足条件共定理4，那么$|\mu|^*(A - K) \leq |\mu|^*(G - K) \leq \varepsilon$。

条件是足够的，因为它说，对于均值收敛的拓扑，$\varphi_A$位于可积函数$\varphi_K$的集合的闭包中（$K$是$A$的任意紧致子集）。

#### 推论 2 {#int-iv-s4-thm-4-cor-2 .statement tag=08T0}

— 对于每个可积集合 $A$，存在：

$1^\circ$ 集合 $A_1 \supset A$，可积开集合的可数交，使得$A_1 - A$可以忽略不计；

$2^\circ$ 集合 $A_2 \subset A$，成对不相交的紧集的可数并，使得$A - A_2$ 可以忽略不计。

$1^\circ$ 对于每个整数 $n$，存在一个可积开集合 $G_n \supset A$，使得$|\mu|(G_n) - |\mu|(A) \leq 1/n$；如果 $A_1$ 是 $G_n$ 的交，则 $|\mu|(A_1) = |\mu|(A)$（No. 5，第 7 条命题的修正），因此 $A_1 - A$ 可以忽略不计。

$2^\circ$ 让我们将定义紧集$K_n$归纳如下：$K_1 \subset A$和$|\mu|(A - K_1) \leq 1$； $K_n \subset A - \bigcup_{i=1}^{n-1} K_i$ 和 $|\mu|(A \cap \mathbf{C}(\bigcup_{i=1}^{n-1} K_i) \cap \mathbf{C}K_n) \leq 1/n$ 对应 $n > 1$（第 4 章）；如果$A_2$是$K_n$的并，则$|\mu|(A_2) = |\mu|(A)$（No. 5，命题8），因此$A - A_2$可以忽略不计。

#### 推论 3 {#int-iv-s4-thm-4-cor-3 .statement tag=08T1}

— 有限外部测度的每个集合都包含在可忽略的集合的并以及其测度有限的成对不相交的紧集和的可数族中。

It suffices to apply Corollary 2 to an integrable open set containing the given set.

#### 推论 4 {#int-iv-s4-thm-4-cor-4 .statement tag=08T2}

— 对于 $X$ 中的每个开集合 $U$，$|\mu|^*(U)$ 是紧集 $K \subset U$ 的措施$|\mu|(K)$ 的上乘。

如果$|\mu|^*(U) < +\infty$，则这是来自 Th 的直接的。 4. 下面的论证也涵盖了$|\mu|^*(U) = +\infty$的情况。由于 $X$ 是局部紧致的且 $U$ 是开集，$\varphi_U$ 是函数 $f \in \mathscr{K}_+$ 的集合 $H$ 的上包络线，使得 $f \leq \varphi_U$ 和 $\operatorname{Supp}(f) \subset U$ (cf. 证明 §1, No. 1、引理），并且由于 $H$ 是针对 $\leq$，因此我们在 §1, No. 1、Th 之前有 $|\mu|^*(U) = \sup_{f \in H} |\mu|(f)$。 1;如果 $f \in H$ 和 $K = \operatorname{Supp}(f)$，则 $f \leq \varphi_K \leq \varphi_U$，则推论为直接的。

注 $|\mu|^*(U)$ 也是相对紧开集合的测度$|\mu|(G)$ 的至高，使得$\overline{G} \subset U$。因为，如果$K$是$U$中包含的紧集，那么对于每个$x \in K$，都存在$x$的相对紧凑的开邻域$V$，使得$\overline{V} \subset U$。在用这些邻域的有限数覆盖$K$时，它们的并$G$是一个相对紧凑的开放集合，使得$\overline{G} \subset U$和$K \subset G$，从而$|\mu|(K) \leq |\mu|(G) \leq |\mu|^*(U)$。

### 7. 刻画有界措施

#### 命题 12 {#int-iv-s4-prop-12 .statement tag=08T3}

— 对于局部紧凑空间 $X$ 上的测度 $\mu$ 有界（第 III, §1, No. 8），$X$ 是关于 $\mu$ 可积的集合是必要且充分的（或者，同样的事情，每个有限常量函数可积）；在这种情况下，

$$
\| \mu \| = | \mu |(X) = \int d|\mu|.
$$

因为，我们已经看到 $|\mu|^*(X) = \| \mu \|$ (§ 1, No. 2)；因此，命题是从No. 6的第10条命题得出的。

对于每个有界度量 $\mu$，我们再次说 $\mu(X)$ 是 $\mu$ 的总质量。

这是从 Th 得出的。 No. 6的4，如果$\mu$是有界测度，那么对于每个$\varepsilon > 0$，存在紧集$K$使得$|\mu|(CK) \leq \varepsilon$。

#### 命题 13 {#int-iv-s4-prop-13 .statement tag=08T4}

— 令 $\mu$ 为 $X$ 上的有界测度。令$\mathscr{B}$为$\mathscr{L}_F^p$上的过滤器基，具有以下属性：
$1^\circ$ 存在集合 $M \in \mathscr{B}$，使得函数 $f \in M$ 一致有界于$X$；
$2^\circ$ $\mathscr{B}$ 均匀收敛于 $X$ 到函数 $f_0$ 的每个紧致子集。
在这些条件下，$f_0$属于到$\mathscr{L}_F^p$和$\mathscr{B}$以阶$p$到$f_0$的平均值收敛。

我们首先注，如果每个$x \in X$和每个函数$f \in M$都有$|f(x)| \leq a$，那么每个$x \in X$也有$|f_0(x)| \leq a$。因此，对于每个$\varepsilon > 0$，存在紧集$K$，使得$|\mu|(CK) \leq \varepsilon^p$和集合$N \in \mathscr{B}$，使得对于每个函数$f \in N$，对于所有$x \in K$，存在$|f(x) - f_0(x)| \leq \varepsilon(|\mu|(K))^{-1/p}$。现在，我们可以写

$$
f - f_0 = (f - f_0)\varphi_K + (f - f_0)\varphi_{CK};
$$

由上可知，如果$f \in M \cap N$则$N_p((f - f_0)\varphi_K) \leq \varepsilon$和$N_p((f - f_0)\varphi_{CK}) \leq 2a\varepsilon$，从而$N_p(f - f_0) \leq (2a + 1)\varepsilon$，从而证明命题。

#### 推论 {#int-iv-s4-n7-cor-1 .statement tag=08T5}

— 对于 $X$ 上的有界测度 $\mu$，$X$ 的每个有界连续映射 $f$ 到 $F$ 属于到每个 $\mathscr{L}_F^p$ ($1 \leq p < +\infty$)。

对于$X$的每个紧凑子集$K$，令$M_K$为$X$的映射的集合到形式$hf$的$F$，其中$h$是连续的$X$的映射到$[0, 1]$等于$K$上的1并且具有紧凑的支撑。很明显，集合$M_K$形式是$\mathscr{L}_F^p$上的滤波器基$\mathscr{B}$，函数属于到$M_K$均匀有界，$\mathscr{B}$均匀收敛到$f$ $X$ 的每个紧凑子集，从而的推论。

特别地，函数$f$是可积的，并且其积分$\int f\, d\mu$相对于积分$\int h f\, d\mu$的$\mathscr{B}$是极限。

我们将重新获得 Cor。将第 13 号提案作为 §5, No. 6 中可积性一般标准的推论。

在第记号章中。 III, §1, No. 2、$|f| \leq \|f\| \cdot 1$ 每函数 $f \in \mathscr{C}^b(X; F)$、从而，由 No. 2 的公式 (3) 和 (4)，

$$
N_p(f) \leq \|f\| \cdot N_p(1) = \|f\| \cdot \|\mu\|^{1/p}.
$$

特别是，对于 $p = 1$，No. 2 的公式 (5) 产量

$$
\left| \int f\, d\mu \right| \leq \|f\| \cdot \|\mu\|,
$$

因此映射 $f \mapsto \int f\, d\mu$ 在 Banach 空间 $\mathscr{C}^b(X; F)$ 上连续；因而，其限制到$\mathscr{C}^b(X; F)$中$\mathscr{K}(X; F)$的闭包$\mathscr{C}^0(X; F)$，即到空间连续函数在点处趋向于0（第III, §1, No. 2，第3条），因此扩张通过积分连续到 $\mathscr{C}^0(X; F)$。

### 8. 与紧凑型支持措施的集成

令$\mu$为$X$的测度，其支持$S = \operatorname{Supp}(\mu)$是紧致的；开集合 $X - S$ 可以忽略不计（§2, No. 2，提案 5）。对于每个函数 $f$ 以及向量空间 $F$ 或 $\overline{\mathbf{R}}$ 中的值，函数 $f$ 和 $f \varphi_S$ 因此是等价的 (§2, No. 4)；对于$f$是$\mu$可积（当$F$是Banach空间时），因而$f \varphi_S$是必要且充分的，在这种情况下（No. 1）

$$
\int f\, d\mu = \int f \varphi_S\, d\mu.
$$

此外，如果 $f$ 有界于 $S$，则根据 (20) 可得出

$$
\left| \int f\, d\mu \right| \leq \|\mu\| \cdot \sup_{x \in S} |f(x)|.
$$

特别是，如果 $f$ 在 $X$ 上连续，则 $f$ 是 $\mu$ 可积，因为 $fh \in \mathscr{K}(X; F)$ 对于$S$ 上的每个函数 $h \in \mathscr{K}(X; \mathbf{R})$ 等于 1（第 III, §1, No. 2、引理 1）。更准确地说：

#### 命题 14 {#int-iv-s4-prop-14 .statement tag=08T6}

— 令 X 为局部紧致空间，F a Banach 空间不减至 0；将X的所有连续映射的空间$\mathscr{C}(X; F)$装备到具有紧收敛的拓扑的F中。对于X上的测度$\mu$使得$\mathscr{K}(X; F)$的线性映射$f \mapsto \int f d\mu$进入F可扩展到F中$\mathscr{C}(X; F)$的连续线性映射，$\operatorname{Supp}(\mu)$是紧的是必要且充分的；这样扩张是唯一的，并且重合具有No. 1中定义的积分。

我们刚刚看到，如果$\mu$具有紧致支持，则对每个函数$f \in \mathscr{C}(X; F)$定义积分$\int f d\mu$，并且$\mathscr{C}(X; F)$到F中的映射$f \mapsto \int f d\mu$对于紧致收敛的拓扑是连续的。相反，假设对于紧凑收敛的拓扑，$f \mapsto \int f d\mu$在$\mathscr{K}(X; F)$是连续的。然后，有紧集$K \subset X$和数$a > 0$，使得每个函数$f \in \mathscr{K}(X; F)$都有$|\mu(f)| \leq a \cdot \sup_{x \in K} |f(x)|$；特别是，如果 $g \in \mathscr{K}(X; F)$ 的支撑不与 K 相交，则$\mu(g) = 0$。取$g = h a$，其中$a \neq 0$是F中的向量和$h \in \mathscr{K}(X; \mathbf{C})$，我们看到对于每个支持度不与K相交的函数$h \in \mathscr{K}(X; \mathbf{C})$，$\mu(h) = 0$，这证明了$\operatorname{Supp}(\mu) \subset K$。最后，扩张的唯一性源自以下事实：对于紧致收敛的拓扑，$\mathscr{K}(X; F)$在$\mathscr{C}(X; F)$中是稠密的（第III, §1, No. 2章，命题4）。

提案 14 允许确定 X 上的测度，其具有连续的扩张至 $\mathscr{C}(X; \mathbf{C})$ 的紧凑支持。因而，具有紧支撑的X上的测度集合可以用Hausdorff局部凸空间$\mathscr{C}(X; \mathbf{C})$的对偶$\mathscr{C}'(X; \mathbf{C})$来识别。回想一下，$\mathscr{C}(X; \mathbf{C})$ 是完整的（GT、X, §1, No. 6、Th. 2 的 Cor. 3），但它不一定是桶装的（Exer. 17）。然而，如果 X 在无穷大可数，因此紧集 $K_n$ 的递增序列并使得 $K_n \subset \overset{\circ}{K}_{n+1}$，则 $\mathscr{C}(X; \mathbf{C})$ 的拓扑可以由可数半范数族定义$p_n(f) = \sup_{x \in K_n} |f(x)|$，因此在本例中$\mathscr{C}(X; \mathbf{C})$ 是 Fréchet 空间。因而，对于由有界集合、空间 $\mathscr{C}'(X; \mathbf{C})$ 覆盖$\mathscr{C}(X; \mathbf{C})$ 的每个$\mathscr{G}$ 来说，$\mathscr{G}$ 拓扑是准完备的（TVS，III, §4, No. 2，Th.1 的 Cor. 4）。

我们首先考虑$\mathscr{C}'(X; \mathbf{C})$拓扑的紧致收敛（拓扑在$\mathscr{C}(X; \mathbf{C})$的紧致子集上的一致收敛）。回想一下，相对紧凑的 $\mathscr{C}(X; \mathbf{C})$ 子集 H 具有以下属性（GT、X, §2, No. 5、Th.2 的 Cor.3）：

$1^\circ$ H 等连续；

$2^\circ$ 对于每个 $x \in X$，$f(x)$ 的集合 $H(x)$（其中 $f$ 越过 H）以 $\mathbf{C}$ 为界。

#### 命题 15 {#int-iv-s4-prop-15 .statement tag=08T7}

— 令 X 为局部紧致空间，对于每个 $x \in X$，令 $\varepsilon_x$ 为点 x 处的狄拉克测度。 X到$\mathscr{C}'(X; \mathbf{C})$的映射$x \mapsto \varepsilon_x$对于$\mathscr{C}'(X; \mathbf{C})$上的紧凑收敛的拓扑是连续的。

对于这个拓扑，考虑$\mathscr{C}'(X; \mathbf{C})$中的$\varepsilon_{x_0}$邻域，我们可以假设通过采用数$\delta > 0$、$\mathscr{C}(X; \mathbf{C})$的紧凑子集H来定义它，并考虑X上的$\mu$测量的集合以及紧凑的支持，例如每函数 $f \in H$ 就有 $|\mu(f) - \varepsilon_{x_0}(f)| \leq \delta$。由于 H 是等连续的，X 中存在$x_0$ 的邻域 U，使得关系 $f \in H$ 对于所有 $x \in U$ 意味着 $|f(x) - f(x_0)| \leq \delta$，也可以写成 $|\varepsilon_x(f) - \varepsilon_{x_0}(f)| \leq \delta$ 并证明命题。(*)

#### 命题 16 {#int-iv-s4-prop-16 .statement tag=08T8}

— 令 K 为 X 上X、L 向量空间测度 $\mu$ 的紧致子集，并包含 K 中的支持。在 L 上，$\mathscr{C}'(X; \mathbf{C})$ 上紧致收敛的拓扑 $\mathscr{T}$ 所导出的拓扑以及$\mathscr{M}(X; \mathbf{C})$（第 III, §1, No. 10）重合上的严格紧致收敛拓扑$\mathscr{T}'$。

很明显，在L上，$\mathscr{T}$引起的拓扑比$\mathscr{T}'$引起的拓扑大更细。相反，令 H 为 $\mathscr{C}(X; \mathbf{C})$ 的紧致子集，$\mathscr{K}(X; \mathbf{C})$ 中的 h 函数等于 K 上的 1。很明显，函数 $fh$ 的集合 H'（其中 $f$ 超过 H）在 $\mathscr{K}(X; \mathbf{C})$ 中是严格紧致的，并且，对于每一个措施$\mu \in L$，$\mu(f) = \mu(fh)$每函数$f \in H$，从而得出结论。

#### 推论 1 {#int-iv-s4-prop-16-cor-1 .statement tag=08T9}

— 对于 X 的每个紧致子集 K 和 X 上的措施 $\mu$ 的每个数 $a > 0$、集合 B，使得 $\operatorname{Supp}(\mu) \subset K$ 和 $\| \mu \| \leq a$ 是 $\mathscr{C}'(X; \mathbf{C})$ 的等连续子集，紧致为拓扑 $\mathscr{T}$ 紧凑收敛。

设H为$\mathscr{C}(X; \mathbf{C})$由……组成或函数的子集，它们一致有界于K；存在数$c > 0$，使得$|\mu(f)| \leq c \cdot \| \mu \| \leq ac$对于每个函数$f \in H$和每个度量$\mu \in B$，根据(22)；因此$B \subset acH^\circ$在$\mathscr{C}(X; \mathbf{C})$的对偶$\mathscr{C}'(X; \mathbf{C})$中，证明B的等连续性； B 对于 $\mathscr{T}$ 是紧致的，这一事实源于以下事实：在 B 上，$\mathscr{T}$ 和模糊的拓扑诱导相同的拓扑（命题 16 和章 16）。 III, §1, No. 10，命题 17）以及 B 是模糊紧致的事实（第 17 章） III, §1, No. 9，科。第 15 号提案第 2 条和第 6 号提案§2, No. 2）。

#### 推论 2 {#int-iv-s4-prop-16-cor-2 .statement tag=08TA}

— Every measure with compact support (resp. every positive measure with compact support) $\mu$ is in the closure in $\mathscr{C}'(X; \mathbf{C})$, for the topology $\mathscr{T}$ of compact convergence, of the set of measures (resp.

(*) 事实上，映射 $x \mapsto \varepsilon_x$ 是 X 到 $\mathscr{C}'(X; \mathbf{C})$ 的同胚（第 VI, §1, No. 6、注 1）。

正测度），其支持是有限的并包含在 Supp(\mu) 中，且范数等于 $\| \mu \|$。

因为，在措施$\nu$的集合B上，使得$\mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu)$和$\| \nu \| \leq \| \mu \|$，由模糊拓扑引起的拓扑与$\mathscr{T}$引起的拓扑相同，因此推论来自第1章。 III, §2, No. 4，科斯。 Th的2和3。 1.

### 9. 部落和加法集合函数

#### 定义 3 {#int-iv-s4-def-3 .statement tag=08TB}

*如果存在定义了实值函数的代数$\mathscr{A}$（超过$\mathbf{R}$）由……组成，则称集合$A$子集非空集合$\Phi$为族$A$，这样关系 $M \in \Phi$ 和 $\varphi_M \in \mathscr{A}$ 是等价的。*

#### 例 {#int-iv-s4-n9-exa-1 .statement tag=08TC}

如果 $\mu$ 是局部紧凑空间 $X$ 的测度，则可积集合形式的特征函数的实数系数为线性组合和 *代数* $\mathscr{A}$，因为，对于任意两个可积集合 $M, N$、函数 $\varphi_M \varphi_N = \varphi_{M \cap N}$ 可积（No. 5，命题 7）；然后它来自 Defs。由图2和图3可知，$X$可积子集的集合是一个族。

#### 命题 17 {#int-iv-s4-prop-17 .statement tag=08TD}

*In order that a nonempty set $\Phi$ of subsets of a set $A$ be a clan, it is necessary and sufficient that it satisfy the following condition:*

(CL) *对于集合 $M, N$ 属于至 $\Phi$、集合 $M \cup N$ 和 $M \cap \mathbf{C}N$ 属于至 $\Phi$ 的每个对。*1

由于关系，条件是*必要的*

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N , \quad \varphi_{M \cap \mathbf{C}N} = \varphi_M - \varphi_M \varphi_N .
$$

为了证明它是“足够的”，我们首先观察到它意味着，对于$\Phi$中的任意两个集合$M, N$，从$M \cap N = M \cap \mathbf{C}(M \cap \mathbf{C}N)$开始，$M \cap N$属于到$\Phi$。令$\mathscr{E}(\Phi)$为线性组合的集合，具有实数系数，为$\Phi$的集合的特征函数。由于 $\varphi_M \varphi_N = \varphi_{M \cap N}$，$\mathscr{E}(\Phi)$ 为代数。一切都归结为，如果$M$是$A$的子集，使得$\varphi_M = \sum_i c_i \varphi_{M_i}$，其中$M_i$属于到$\Phi$，那么$M \in \Phi$。这将由以下引理产生：

#### 引理 {#int-iv-s4-n9-lem-1 .statement tag=08TE}

*令 $\Phi$ 为$A$ 满足子集非空集合公理（CL）。给定$\Phi$中集合的有限族$(M_i)_{1 \leq i \leq n}$，存在*

1 集合 $A$ 子集的氏族 $\Phi$ 也称为集合的 *环*（或 *布尔环*）；此外，如果$A \in \Phi$，则$\Phi$被称为集合（cf. GT，I, §6，Exer.20和II, §4，Exer.12）的*代数*（或*布尔代数*）。在可数并下闭合的布尔值代数称为 *部落*，或 *$\sigma$*-*代数*（GT，IX, §6, No. 3，Def. 3）。

$\Phi$中成对不相交的集合的有限族$(N_j)_{1 \leq j \leq m}$，使得每个$M_i$是$N_j$的某个数的并。

例如，考虑形式$\bigcap_{i=1}^n P_i$的$2^n - 1$集合，其中$P_i = M_i$对于某些指标$i$，$P_i = \mathbf{C} M_i$对于其他$P_i$至少有一个等于$M_i$。令$(N_j)_{1 \leq j \leq m}$为这些集合中排列在某些阶中的序列；它们是成对的不相交的和属于到 $\Phi$；另一方面，对于$(P_i)$家庭来说，每个集合$M_k$都是集合$N_j = \bigcap_{i=1}^n P_i$相应的的并，这样$P_k = M_k$，这就证明了引理。

引理成立，形式$\sum_{i=1}^n c_i \varphi_{M_i}$的每个函数，其中$M_i \in \Phi$，可以写成形式$\sum_{j=1}^m d_j \varphi_{N_j}$，其中$N_j$属于到$\Phi$ 和 是成对的不相交的；如果$\varphi_M = \sum_{j=1}^m d_j \varphi_{N_j}$，则对于每个指标$j$，必然有$d_j = 0$或$d_j = 1$，因此$M$是$N_j$中某个数的并，因此属于为$\Phi$。

每族$A$包含子集$\Phi$$A$空子集$\varnothing$；因为，至少存在一个子集$M \in \Phi$，因此$M - M = \varnothing$属于到$\Phi$。 注还有单子集$\varnothing$$A$由……组成子集集合为一族。

#### 定义 4 {#int-iv-s4-def-4 .statement tag=08TF}

*给定一个部落$\Phi$ of 子集 of 集合 $A$，和一个Banach 空间 $F$，一个人调用步骤函数*² *超过集合 of $\Phi$（或$\Phi$步） 函数)，其中$F$中有值，形式* $\sum_i a_i \varphi_{M_i}$的每个函数，*其中$a_i$属于到$F$，以及$M_i$到$\Phi$。*

很明显，$F$中的值的$\Phi$步函数的集合$\mathscr{E}_F(\Phi)$是向量空间超过$\mathbf{R}$或$\mathbf{C}$。我们刚刚在第 17 号提案中看到，实值 $\Phi$ 步长函数的集合 $\mathscr{E}(\Phi)$ 是$\mathbf{R}$ 上的 *代数*；它也是$\Phi$的集合的特征函数生成$\mathbf{R}^A$的线性子空间。

到引理，$\mathscr{E}_F(\Phi)$中的每个函数都可以写成$f = \sum_j c_j \varphi_{N_j}$，其中$N_j \in \Phi$是成对的不相交的；由此得出$|f| = \sum_j |c_j| \varphi_{N_j}$属于到$\mathscr{E}(\Phi)$。特别是，$\mathscr{E}(\Phi)$是*Riesz空间*，因为$\mathscr{E}(\Phi)$属于到$\mathscr{E}(\Phi)$中两个函数的上包络线。

#### 注 {#int-iv-s4-n9-rem-1 .statement tag=08TG}

— 很容易看出 Def. 4等价于：$F$中具有值的$\Phi$步函数是函数$f$，它仅采用值的有限数，并且对于每个$a \neq 0$ $F$、集合 $f(a)^{-1}$ 属于至 $\Phi$。

² 功能表，从而记号 $\mathscr{E}(\Phi)$如下。

#### 定义 5 {#int-iv-s4-def-5 .statement tag=08TH}

— *实值函数* $\lambda$ *在部落上定义* $\Phi$ *子集 of 集合* $A$ *如果对于每个对* $M, N$ *of 不相交的则被认为是可加的集合属于至* $\Phi$、$\lambda(M \cup N) = \lambda(M) + \lambda(N)$。

特别是从定义可以得出$\lambda(\varnothing) = 0$。

#### 命题 18 {#int-iv-s4-prop-18 .statement tag=08TI}

— *让* $\lambda$ *成为加法集合函数在部落* $\Phi$ 上定义。 *存在且仅有一个线性形式*（再次表示为$\lambda$）*在向量空间*$\mathscr{E}(\Phi)$*实值*$\Phi$*步长函数*，*使得*$\lambda(\varphi_M) = \lambda(M)$*对于每个集合* $M \in \Phi$； *此外，如果* $\lambda(M) \geqslant 0$ *对于每个* $M \in \Phi$，*则* $\lambda$ *是* $\mathscr{E}(\Phi)$ 上的正线性形式。

线性形式 $\lambda$ 的 *唯一性* 很清楚，因为$\Phi$ 生成向量空间 $\mathscr{E}(\Phi)$ 中集合的特征函数。为了证明$\lambda$的*存在*，只需证明关系$\sum_i c_i \varphi_{M_i} = 0$，其中$M_i$是非空集合属于到$\Phi$，蕴涵$\sum_i c_i \lambda(M_i) = 0$。

现在，到引理，$\Phi$中存在成对不相交的非空集合的有限族$(N_j)$，这样，对于每个指标$i$、$\varphi_{M_i} = \sum_j a_{ij} \varphi_{N_j}$与$a_{ij} = 0$或$a_{ij} = 1$。 关系 $\sum_i c_i \varphi_{M_i} = 0$，可以写作$\sum_j \left( \sum_i c_i a_{ij} \right) \varphi_{N_j} = 0$，因此意味着对于每个指标$j$，$\sum_i c_i a_{ij} = 0$。由Def。 5、然后我们有

$$
\sum_i c_i \lambda(M_i) = \sum_j \left( \sum_i c_i a_{ij} \right) \lambda(N_j) = 0,
$$

这就证明了$\lambda$的存在。最后，假设对于每个$M \in \Phi$都有$\lambda(M) \geqslant 0$；对于每个函数$f \in \mathscr{E}(\Phi)$，可以写成$f = \sum_i c_i \varphi_{M_i}$，其中$M_i \in \Phi$是成对的不相交的；如果$f \geqslant 0$，则对于每个指标$i$，$c_i \geqslant 0$使得$M_i$是非空，从而$\lambda(f) = \sum_i c_i \lambda(M_i) \geqslant 0$。

### 10. 通过步长函数逼近连续函数

#### 命题 19 {#int-iv-s4-prop-19 .statement tag=08TJ}

— *令*$X$*为局部紧凑空间，*$\Phi$**$X$的子集族，*$X$的紧凑子集*包含集合。 *对于每个连续的映射* $f$ *of* $X$ *进入 Banach 空间* $F$ *（分别为每个连续的实值函数* $f \geqslant 0$ *on* $X$）*具有紧凑的支持* $K$，*存在序列* $(g_n)$*的函数在*$\mathscr{E}_F(\Phi)$*包含在*$K$*中的支持（或序列*$(g_n)$*的函数在*$\mathscr{E}(\Phi)$*这样* $0 \leqslant g_n \leqslant f$ *对于每个* $n$) *一致收敛到* $f$ *（或$f$）。

由于$f$在$K$上一致连续，因此可以通过紧集$M_i$（$1 \leq i \leq m$）的有限数覆盖$K$，使得$f$在每个$M_i$上的振荡为$\leq 1/n$。由于$M_i$和$K$属于到$\Phi$，$K$存在划分进入集合$N_j \in \Phi$，使得集合$M_i \cap K$中的每一个都是某个特定的并 $N_j$（No. 9、引理）中的数。令$a_j$为$F$的元素，使得$|f(x) - a_j| \leq 1/n$在$N_j$上。 设定 $g_n = \sum_j a_j \varphi_{N_j}$，在本例中我们有 $|f - g_n| \leq 1/n$、从而命题。对于取 $a_j = \inf_{x \in N_j} f(x)$ 和 $g_n = \sum_j a_j \varphi_{N_j}$ 的连续实值函数 $f$，人们也提出了类似的观点。

#### 推论 1 {#int-iv-s4-prop-19-cor-1 .statement tag=08TK}

*令$\mu$为$X$的度量； 空间 $\mathscr{E}_F(\Phi)$ 在空间 $\mathscr{L}_F^p$ ($1 \leq p < +\infty$) 中都很密集。*

For, it follows from Prop. 19 and the criterion for convergence in mean for uniform limits of functions with compact support (§ 3, No. 3, Prop. 4) that $\mathscr{E}_F(\Phi)$ is dense, for the topology of convergence in mean of order $p$, in the closure of the space $\mathscr{K}_F$ of continuous functions with compact support, whence the corollary.

#### 推论 2 {#int-iv-s4-prop-19-cor-2 .statement tag=08TL}

*对于$X$的每个闭子集$S$，每个函数$f \in \mathscr{K}(X, S; \mathbf{C})$都是线性组合$\sum_i \lambda_i \varphi_{K_i}$的统一极限，其中$\lambda_i$属于到$\mathbf{C}$和$K_i$是紧凑子集 $S$。*

这样的线性组合的集合 $\mathscr{A}$ 是$\mathbf{C}$-代数。令 $\Phi$ 为子集 $M$ $X$ 的集合，使得$\varphi_M \in \mathscr{A}$；因此，$\Phi$是一个*氏族*，其所有元素都是$S$的子集，包含是$S$的紧凑子集，以及$\mathscr{E}_C(\Phi) \subset \mathscr{A}$。然后，将第 19 号提案应用于局部紧凑空间 $S$ 和氏族 $\Phi$ 就足够了。

#### 推论 3 {#int-iv-s4-prop-19-cor-3 .statement tag=08TM}

*如果$\mu$和$\nu$是$X$的两个度量，使得$\mu(K) = \nu(K)$对于$X$的每个紧凑子集$K$，则$\mu = \nu$。*

因为，它是从 Cor 得出的。 2和定义的措施，对于$X$、$\mu$和$\nu$的每个紧凑子集$S$，在$\mathscr{K}(X, S; \mathbf{C})$中采取相同的值。

### 11. 对集合族定义的测度的扩张

令$\Phi$为局部紧致空间$X$的子集的非空集合。给定一个实值函数 $M \mapsto \alpha(M)$，在$\Phi$上定义和$\geq 0$，我们建议寻找条件，其中$X$上存在正测度$\mu$，使得$\Phi$的集合是$\mu$可积的，并且$\mu(M) = \alpha(M)$ 对于所有 $M \in \Phi$。我们将极限自己考虑集合$\Phi$满足以下条件的情况：

(PC_I) *$\Phi$属于到$\Phi$的两个集合中的并和交。*

(PC_{II}) *对于紧集 K 的每个对由……组成以及X 中的开集合 U 使得$K \subset U$，存在集合 $M \in \Phi$使得$K \subset M \subset U$。*

注条件(PC_{II})通过取$K = U = \varnothing$意味着$\varnothing \in \Phi$。然而，集合$\Phi$不一定是一个氏族；对于例，X的所有紧致子集的集合满足条件(PC_I)和(PC_{II})，但一般不是族，因为如果M和N是紧致的，则$M \cap \mathbf{C}N$一般不成立。

我们假设在加法中，$\Phi$上定义的函数$\alpha$满足以下条件（显然问题有解是必要的）：

(PM_I) *关系 $M \subset N$ 意味着 $\alpha(M) \leq \alpha(N)$.*
(PM_{II}) *对于$\Phi$、$\alpha(M \cup N) \leq \alpha(M) + \alpha(N)$中的任意 M 和 N。*
(PM_{III}) *关系$M \cap N = \varnothing$意味着$\alpha(M \cup N) = \alpha(M) + \alpha(N)$.*

在条件 (PM_{III}) 中取$N = \varnothing$，可推断出 $\alpha(\varnothing) = 0$； 条件 (PM_I) 然后显示对于每个 $M \in \Phi$ 都有 $\alpha(M) \geq 0$。

#### 定理 5 {#int-iv-s4-thm-5 .statement tag=08TN}

*令$\Phi$为局部紧凑空间X、满足(PC_I)和(PC_{II})的子集的集合，并令$\alpha$为实值函数，定义于$\Phi$、满足条件（PM_I）、（PM_{II}）和（PM_{III}）。在阶中，X上存在正测度$\mu$，使得$\Phi$的集合是$\mu$可积的，并且$\mu(M) = \alpha(M)$对于所有$M \in \Phi$来说是充分必要的，$\alpha$满足加法以下条件:*

(PM_{IV}) *对于每个$\varepsilon > 0$和每个$M \in \Phi$，都存在紧集$K \subset M$和一个开放的集合$U \supset M$，这样，对于每个$N \in \Phi$满足关系 $K \subset N \subset U$，一个有$|\alpha(N) - \alpha(M)| \leq \varepsilon$。*

*此外，如果满足条件(PM_{IV})，则测度$\mu$是唯一的；对于每个紧集 $K$、$\mu(K) = \inf_{M \in \Phi, M \supset K} \alpha(M)$；每次打开集合 $U$、$\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$。*

注条件 (PM_{IV}) 相当于以下两个中的合取：

(PM'_{IV}) *对于每个$\varepsilon > 0$和每个$M \in \Phi$，都存在一个开放的集合$U \supset M$，这样，对于$U$中包含的每个$N \in \Phi$，$\alpha(N) \leq \alpha(M) + \varepsilon$。*
(PM''_{IV}) *对于每个$\varepsilon > 0$和每个$M \in \Phi$，都存在紧集$K \subset M$，这样，对于每个$N \in \Phi$包含于$K$，$\alpha(N) \geq \alpha(M) - \varepsilon$。*

因为，很明显，(PM'_{IV})和(PM''_{IV})暗示着(PM_{IV})。相反，让我们证明对于例，(PM_{IV}) 意味着 (PM'_{IV})：令 K 为紧集，U 为开集合，使得对于每个$P \in \Phi$，$K \subset M \subset U$ 和 $|\alpha(P) - \alpha(M)| \leq \varepsilon$ 满足$K \subset P \subset U$。然后，如果$N \in \Phi$和$N \subset U$、$M \cup N$属于到$\Phi$和$K \subset M \cup N \subset U$、从而$\alpha(M \cup N) \leq \alpha(M) + \varepsilon$和*更不必说*$\alpha(N) \leq \alpha(M) + \varepsilon$。

当集合$\Phi$、满足(PC_I)和(PC_{II})由*紧凑*集合组成时，则条件(PM''_{IV})被简单验证，并且(PM_{IV})则相当于 (PM'_{IV})。

条件 (PM_{IV}) 是*必要的*：这立即从 Th 开始。 No. 6 的第 4 部分关于可积集合与紧集和开集合的“近似”。为了证明定理的另一个断言，我们分几个步骤进行。

$\mathfrak{P}(X)$ 上拓扑 1° 定义。

对于紧集$K$中的每个对$(K, U)$由……组成和$X$中的开集合$U$，我们用子集$M \subset X$中的$I(K, U)$集合表示，这样$K \subset M \subset U$；在阶中，$I(K, U)$为非空，$K \subset U$是充分必要的。如果$(K', U')$是第二个对，由紧集$K'$和一个开集合$U'$组成，我们有
$$
I(K, U) \cap I(K', U') = I(K \cup K', U \cap U').
$$
令 $T$ 为由子集 $I(K, U)$ 的集合生成的 $\mathfrak{P}(X)$ 上的拓扑，因为 $K$ 运行于 $X$ 的紧致子集的集合，且$U$ 运行过$X$开子集集合；由上可知，$I(K, U)$形式基对应于拓扑$T$（GT，I, §1, No. 3）。

我们观察到，$T$的定义意味着，在$\mathfrak{P}(X)$中，$X$的紧致子集的集合是稠密的。 条件 (PC_{II}) 表示 $\Phi$ 在 $\mathfrak{P}(X)$ 上是稠密的，条件 (PM_{IV}) 表示函数 $\alpha$ 对于 $\Phi$ 来说是连续的，由拓扑引起$T$。最后，Th。 No. 6的4表示对于$T$诱导的拓扑，函数$M \mapsto \mu(M)$在$\mu$可积集合族上是连续的。

2° 唯一性 $\mu$。

我们用子集$M \subset X$的$\overline{\Phi}$集合表示，使得$\alpha(N)$趋向于有限的极限，而$N$趋于$M$（对于拓扑$T$），同时保持在$\Phi$；然后，我们可以仅以一种方式将扩展$\alpha$转换为$\overline{\Phi}$的连续映射$\overline{\alpha}$进入$\mathbf{R}$（GT，I, §8, No. 5，Th.1）。如果存在满足要求的测度$\mu$，则上述注证明$\mu$可积集合的族$\Psi$包含在$\overline{\Phi}$中，并且对于每个$M \in \Psi$都有$\mu(M) = \overline{\alpha}(M)$；这个关系尤其适用于$X$的每个紧凑子集$M$，这证明了$\mu$的唯一性（No. 10，第19号提案的Cor.3）。

$\alpha$ 至紧集 3° 扩张。

在不假设$\mu$存在的情况下，我们现在要研究$\alpha$到$\overline{\Phi}$的集合$\overline{\Phi}$和扩张$\overline{\alpha}$。我们首先展示每个紧集$K$属于到$\overline{\Phi}$以及$\overline{\alpha}(K) = \inf_{P \in \Phi, P \supset K} \alpha(P)$。 集合$a = \inf_{P \in \Phi, P \supset K} \alpha(P)$；对于每个$\varepsilon > 0$，都存在一个$M \in \Phi$，使得$K \subset M$和$\alpha(M) \leq a + \varepsilon$。通过(PM'_{IV})，存在一个开集合$U \supset M$，这样，对于$U$中包含的每个$N \in \Phi$，我们有$\alpha(N) \leq \alpha(M) + \varepsilon \leq a + 2\varepsilon$；对于每个$N \in \Phi$，这样$K \subset N \subset U$，我们因此有$a \leq \alpha(N) \leq a + 2\varepsilon$，到定义，它表明$K \in \overline{\Phi}$和$\overline{\alpha}(K) = a$。

这个结果立刻证明，如果$K_1$和$K_2$是两个紧集使得$K_1 \subset K_2$，则$\overline{\alpha}(K_1) \leq \overline{\alpha}(K_2)$。如果$K_1$和$K_2$是任意两个紧集，我们通过(PM_{II})得到$\overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$。此外，我们还将看到，如果$K_1$和$K_2$是不相交的，则$\overline{\alpha}(K_1 \cup K_2) = \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$。因为，存在两个不相交的开集合$U_1, U_2$使得$K_1 \subset U_1$，$K_2 \subset U_2$（GT，II, §4，命题4）。因此，通过(PC_{II})，也存在两个集合、$M_1 \in \Phi$、$M_2 \in \Phi$，使得$K_1 \subset M_1 \subset U_1$和$K_2 \subset M_2 \subset U_2$。现在让$P$为$\Phi$包含于$K_1 \cup K_2$中的任意集合；两个集合$P \cap M_1$和$P \cap M_2$属于到$\Phi$的并通过(PC_{I})，并且由于这两个集合是不相交的，应用(PM_I)和(PM_{III}) 产量

$$
\alpha(P) \geq \alpha(P \cap M_1) + \alpha(P \cap M_2) \geq \overline{\alpha}(K_1) + \overline{\alpha}(K_2),
$$

这就建立了我们的断言。

**4° 扩张 $\alpha$ 至开放集合。**

现在我们将看到，对于开集合$U$到属于到$\overline{\Phi}$，由于$K$运行于$U$的紧致子集的集合，所以数的上界是充分必要的$\overline{\alpha}(K)$ 是有限的；此外，$\overline{\alpha}(U)$等于这个上界。

对于，令$U$是集合属于到$\overline{\Phi}$的开；对于每一个$\varepsilon > 0$，都存在紧集$K \subset U$，这样，对于每一个集合$M \in \Phi$满足$K \subset M \subset U$，都有$|\overline{\alpha}(U) - \alpha(M)| \leq \varepsilon$，从而$|\overline{\alpha}(U) - \overline{\alpha}(K)| \leq \varepsilon$；另一方面，如果$K'$是$U$中包含的任何紧集，则$K \subset K \cup K' \subset U$，从而$|\overline{\alpha}(U) - \overline{\alpha}(K \cup K')| \leq \varepsilon$，等等$\overline{\alpha}(U) \geq \overline{\alpha}(K \cup K') - \varepsilon \geq \overline{\alpha}(K') - \varepsilon$；因此，$\overline{\alpha}(U)$确实等于数$\overline{\alpha}(K)$的上界，因为$K$超过了$U$的紧凑子集的集合。

相反，让$U$是一个开集合，使得$b = \sup_{K \subset U} \overline{\alpha}(K) < +\infty$（$K$运行在$U$的紧凑子集的集合上），并让我们证明$U \in \overline{\Phi}$。对于每个$\varepsilon > 0$，都存在紧集$K \subset U$使得$b - \varepsilon \leq \overline{\alpha}(K) \leq b$；通过 (PM''_{IV})，对于每个集合 $M \in \Phi$ 使得 $K \subset M \subset U$，存在紧集 $K' \subset M$ 使得

$$
\alpha(M) \leq \overline{\alpha}(K') + \varepsilon \leq b + \varepsilon;
$$

因此$b - \varepsilon \leq \alpha(M) \leq b + \varepsilon$，证明$U \in \overline{\Phi}$。

从开集合$U \in \overline{\Phi}$和$\overline{\alpha}(U)$的刻画，首先得出如果$U_1$和$U_2$是两个开集合使得$U_1 \subset U_2$和$U_2 \in \overline{\Phi}$，则$U_1 \in \overline{\Phi}$和$\overline{\alpha}(U_1) \leq \overline{\alpha}(U_2)$。另一方面，如果$U_1$和$U_2$是集合属于到$\overline{\Phi}$的两个开，那么$U_1 \cup U_2$和$\overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2)$也是如此。例如，令$K$为$U_1 \cup U_2$中包含的任何紧集；对于每个点$x \in K$，都存在一个$x$的紧邻域包含在$U_1$或$U_2$中；因此，我们可以通过这些邻域的有限数覆盖 $K$；如果$K_1$（或$K_2$）是$U_1$（或$U_2$）中包含的并，则$K \subset K_1 \cup K_2$，从而

$$
\overline{\alpha}(K) \leq \overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2),
$$

这建立了断言的性质。

**$\overline{\Phi}$ 和 $\overline{\alpha}$ 的 5° 性质。**

$\overline{\Phi}$和$\overline{\alpha}$的定义现在可以变换如下（考虑到（PC_{II}））：在阶和$M \in \overline{\Phi}$中，对于每个$\varepsilon > 0$，存在紧集$K$和一个开集合$U \in \overline{\Phi}$使得$K \subset M \subset U$和$\overline{\alpha}(U) - \overline{\alpha}(K) \leq \varepsilon$；此外，$\overline{\alpha}(M)$是开集合$U \in \overline{\Phi}$包含$M$的$\overline{\alpha}(U)$的*下确界*，以及紧集$K \subset M$的$\overline{\alpha}(K)$的*上界*。

由此，我们首先推断，如果$M_1, M_2$和$M_1 \cup M_2$属于到$\overline{\Phi}$，则$\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2)$。事实上，如果$U_1$和$U_2$分别是$\overline{\Phi}$包含$M_1$和$M_2$的两个开集合，并且使得$\overline{\alpha}(U_1) \leq \overline{\alpha}(M_1) + \varepsilon$和$\overline{\alpha}(U_2) \leq \overline{\alpha}(M_2) + \varepsilon$，那么$U_1 \cup U_2$属于到 $\overline{\Phi}$、包含 $M_1 \cup M_2$，因而

$$
\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2) + 2\varepsilon,
$$

从而我们的断言。

接下来，让我们证明，如果$K$是紧集并且$U$是$\overline{\Phi}$的开集合使得$K \subset U$，那么$\overline{\alpha}(U - K) = \overline{\alpha}(U) - \overline{\alpha}(K)$。综上所述，我们有$\overline{\alpha}(U) \leq \overline{\alpha}(K) + \overline{\alpha}(U - K)$。另一方面，对于每紧集 $K' \subset U - K$，

$$
\overline{\alpha}(K \cup K') = \overline{\alpha}(K) + \overline{\alpha}(K') \leq \overline{\alpha}(U);
$$

由于$U - K$是开集，并且属于到$\overline{\Phi}$，所以$\overline{\alpha}(U - K)$是$\overline{\alpha}(K')$的上界，这表明$\overline{\alpha}(K) + \overline{\alpha}(U - K) \leq \overline{\alpha}(U)$。

因而，$\overline{\Phi}$的定义现在可以用以下方式表达：在阶和$M \in \overline{\Phi}$中，对于每个$\varepsilon > 0$，存在紧集$K$和一个开集合$U \in \overline{\Phi}$是必要且充分的，使得$K \subset M \subset U$ 和 $\overline{\alpha}(U - K) \leq \varepsilon$。

我们现在可以证明 $\overline{\Phi}$ *是一个氏族*，并且 $\overline{\alpha}$ 是 $\overline{\Phi}$ 上的 *加法集合函数*。我们首先证明，如果$M$和$N$属于到$\overline{\Phi}$，那么$M \cap \mathbf{C}N$和$M \cup N$也是如此。到假设，对于每个$\varepsilon > 0$，存在两个紧集$K, K'$和$\overline{\Phi}$的两个开集合$U, U'$，这样

$$
K \subset M \subset U,\quad K' \subset N \subset U',\quad \overline{\alpha}(U - K) \leq \varepsilon,\quad \overline{\alpha}(U' - K') \leq \varepsilon.
$$

集合$K'' = K \cap \mathbf{C}U'$是紧凑型，集合$U'' = U \cap \mathbf{C}K'$是开放型，属于至$\overline{\Phi}$和$K'' \subset M \cap \mathbf{C}N \subset U''$；另一方面，$U'' - K''$包含在$U \cap \mathbf{C}K$和$U' \cap \mathbf{C}K'$的并、从而$\overline{\alpha}(U'' - K'') \leq 2\varepsilon$中，从而证明了$M \cap \mathbf{C}N \in \overline{\Phi}$。同样，$U_1 = U \cup U'$是开集，属于到$\overline{\Phi}$，$K_1 = K \cup K'$是紧集，$K_1 \subset M \cup N \subset U_1$；另一方面，$U_1 - K_1$包含在$U - K$和$U' - K'$的并中，从而又包含在$\overline{\alpha}(U_1 - K_1) \leq 2\varepsilon$中，$M \cup N$包含在属于到$\overline{\Phi}$中。最后，如果$M$和$N$是不相交的，那么

$$
\overline{\alpha}(K_1) = \overline{\alpha}(K) + \overline{\alpha}(K') \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon,
$$

因而 $\overline{\alpha}(M \cup N) \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon$；由于$\varepsilon$是任意的，所以我们有$\overline{\alpha}(M \cup N) = \overline{\alpha}(M) + \overline{\alpha}(N)$。

**6° 测量 $\mu$ 的存在。**

根据No. 9的第18条命题，$\overline{\Phi}$步函数的向量空间$\mathscr{E}(\overline{\Phi})$上存在且仅有一个正线性形式$\beta$，使得$\beta(\varphi_M) = \overline{\alpha}(M)$对于所有$M \in \overline{\Phi}$。对于$X$的每个紧凑子集$K$，让我们用$\mathscr{E}(\overline{\Phi})$的函数的*统一极限*的$\mathscr{G}(K)$空间表示，其支持包含在$K$中。由于$\beta$是正数，$|\beta(f)| \leq \overline{\alpha}(K) \cdot \|f\|$对于每个函数$f \in \mathscr{E}(\overline{\Phi})$，其支持度包含在$K$中；其中函数中的$\beta$到空间的限制是均匀收敛的拓扑的*连续*线性形式；因此，它可以扩展到$\mathscr{G}(K)$上的正连续线性形式$\overline{\beta}_K$。此外，如果$K \subset K_1$，则$\overline{\beta}_{K_1}$到$\mathscr{G}(K)$的限制与$\overline{\beta}_K$相同，因此在$\mathscr{G}(K)$的并$\mathscr{G}$上存在正的线性形式$\overline{\beta}$，即扩展形式 $\overline{\beta}_K$ 各。

现在，由于具有紧凑支持的连续实值函数的每个紧集属于到$\overline{\Phi}$，空间$\mathscr{H}$都是$\mathscr{G}$的*子空间*（No. 10，提案19）；因此，正线性形式 $\overline{\beta}$ 的 *限制* 到 $\mathscr{H}$ 是正 *测量* $\mu$。让我们证明对于每个紧集 $K$，$\mu(K) = \overline{\alpha}(K)$。对于每个$\varepsilon > 0$，都存在一个开集合$U \in \overline{\Phi}$，使得$K \subset U$、$\mu(U) \leq \mu(K) + \varepsilon$和$\overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon$。令$f$是$X$到$[0, 1]$的连续映射，其支持包含在$U$中，并且使得$f(x) = 1$在$K$上（第III, §1, No. 2，引理1）。然后 $\mu(K) \leq \mu(f) \leq \mu(U) \leq \mu(K) + \varepsilon$，另一方面，

$$
\overline{\alpha}(K) = \beta(\varphi_K) \leq \overline{\beta}(f) \leq \beta(\varphi_U) = \overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon;
$$

从$\mu(f) = \overline{\beta}(f)$开始，我们看到$|\mu(K) - \overline{\alpha}(K)| \leq \varepsilon$，并且由于$\varepsilon$是任意的，所以$\mu(K) = \overline{\alpha}(K)$。

开放集合属于至 $\overline{\Phi}$ 的刻画，与 Cor 结合。 4 Th。 No. 6的4，则表明开集合属于到$\overline{\Phi}$正是$\mu$可积开集合，并且对于这样的集合$U$，我们有$\mu(U) = \overline{\alpha}(U)$。 Th。 No. 6的4和$\overline{\Phi}$的集合的刻画以5°给出，则表明$\mu$可积的集合是$\overline{\Phi}$的集合，并且对于这样的集合$M$， $\mu(M) = \overline{\alpha}(M)$。最后，对于每个打开的集合 $U$，$\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$ 立即从 (PC$_{II}$) 和 Cor 得出。 4 Th。 4 个No. 6。

定理 5 至此完全证明。

#### 推论{#int-iv-s4-n11-cor-1 .statement tag=08TO}

— *令X为局部紧凑空间，其中X的Borel集合的可数基、$\Psi$集合、$\Psi$的$\beta$映射进入$[0, +\infty]$满足以下条件:*

(i) *如果* $(B_1, B_2, \ldots)$ *是不相交的 Borel 集合和X 的序列，则* $\beta(B_1 \cup B_2 \cup \ldots) = \beta(B_1) + \beta(B_2) + \ldots$。

(ii) *如果 B 是 X 的紧致子集，则* $\beta(B) < +\infty$。

*那么，在 X 上存在一项且仅有一项正向措施 $\mu$，使得* $\beta(B) = \mu^*(B)$ *对于所有* $B \in \Psi$。

令$\Phi$为$X$的紧凑子集的集合，并令$\alpha$为$\beta$至$\Phi$的限制。然后满足条件(PC$_I$)、(PC$_{II}$)、(PM$_I$)、(PM$_{II}$)、(PM$_{III}$)和(PM$_{IV}'$)。令$K$为$X$和$\varepsilon > 0$的紧致子集。那么$K$就是$X$相对紧凑的开放集合的递减序列$(U_1, U_2, \ldots)$交（GT，IX, §2, No. 5，命题7）。我们有 $\sum_{n=1}^{\infty} \beta(U_n - U_{n+1}) = \beta(U_1 - K) < +\infty$，因此

$$
\beta(U_n) - \beta(K) = \beta(U_n - K) = \sum_{p=n}^{\infty} \beta(U_p - U_{p+1})
$$

当$n$趋向于$\infty$时，趋向于0。这就证明条件$(\mathrm{PM}'_{\mathrm{IV}})$是满足的。由 Th. 5，在$X$上存在正测度$\mu$，使得$\mu(K) = \alpha(K)$对于$X$的每个紧凑子集$K$。由于$X$的每个开集合$U$是紧凑子集的递增序列并，所以我们有$\mu^*(U) = \beta(U)$。令 $L$ 为 $X$ 的紧致子集。根据No. 5的第7条，$L$形式的$\mu$可积子集是$L$的子集的一个部落。因此，如果$B$是$L$中包含的$\Psi$的元素，则$B$是$\mu$可积；对于每个$\varepsilon > 0$，紧集$K$和$X$中的开集合$U$，使得$K \subset B \subset U$和$\mu^*(U) - \mu(K) \leq \varepsilon$（No. 6，Th.4）。从$\beta(U) = \mu^*(U)$和$\beta(K) = \mu(K)$开始，我们看到$|\mu^*(B) - \beta(B)| \leq 2\varepsilon$。因此$\beta(B) = \mu^*(B)$。最后，$X$的每一个Borel集合$C$是两两不相交的序列并，相对紧凑的Borel集合，从而$\beta(C) = \mu^*(C)$。 $\mu$的唯一性立即从Th开始。 5.

### 习题 {#int-iv-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
