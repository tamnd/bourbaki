---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 5
section_title: Measurable functions and sets
lang: zh
source: int-i-vi
book_pages: INT IV.59-INT IV.89, INT IV.127-INT IV.134
pdf_pages: 0166-0196, 0234-0241
extraction: ocr
subsections:
    - "no": 1
      title: Definition of measurable functions and sets
      page: 59
      pdf_page: 166
    - "no": 2
      title: Principle of localization. Locally negligible sets
      page: 61
      pdf_page: 168
    - "no": 3
      title: Elementary properties of measurable functions
      page: 63
      pdf_page: 170
    - "no": 4
      title: Limits of measurable functions
      page: 64
      pdf_page: 171
    - "no": 5
      title: Criteria for measurability
      page: 66
      pdf_page: 173
    - "no": 6
      title: Criteria for integrability
      page: 71
      pdf_page: 178
    - "no": 7
      title: Measure induced on a locally compact subspace
      page: 73
      pdf_page: 180
    - "no": 8
      title: $\mu$-dense families of compact sets
      page: 76
      pdf_page: 183
    - "no": 9
      title: Locally countable partitions
      page: 77
      pdf_page: 184
    - "no": 10
      title: Measurable functions defined on a measurable subset
      page: 78
      pdf_page: 185
    - "no": 11
      title: Convergence in measure
      page: 80
      pdf_page: 187
    - "no": 12
      title: A property of vague convergence
      page: 86
      pdf_page: 193
statements: 79
exercises: 30
content_sha256: 34a60e8b4d91187e0295427a4a7c9e333b513302db559e247ae24d31d2b97bc2
translated_from: content/en/int/IV/05_s5_measurable_functions_and_sets.md
translation_method: google
source_content_sha256: 3b5e810e086ae5ed0fb3b0f106b25333088c6f327ee0cfc196e61afb7abd9879
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8f3cb899b880182ac9254407ef0f4a8fa77079b567af3bbc77525176b41a74a4
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。可测量函数和集合

### 1. 可测量的函数和集合的定义

#### 定义 1 {#int-iv-s5-def-1 .statement tag=08UC}

*令$X$为局部紧凑空间，$\mu$为$X$的测度。 A mapping $f$ of $X$ into a topological space $F$ is said to be measurable for the measure $\mu$ (or to be $\mu$-measurable) if, for every compact subset $K$ of $X$, there exist a $\mu$-negligible set $N \subset K$ and a partition of $K - N$ formed by a sequence (finite or infinite) $(K_n)$ of compact sets, such that the restriction of $f$ to each $K_n$ is continuous.*

显然，$X$到$F$的每个连续映射都是可测的。

注如果 $\mu$ 和 $\nu$ 是 $X$ 上的两个测度，使得每个 $\mu$ 可忽略的集合都是 $\nu$ 可忽略的，那么 *每个 $\mu$ 可测的函数也是$\nu$-可测量*（cf. V, §5 章，第 5、6 号）。

定义1可以转化为以下准则：

#### 命题 1 {#int-iv-s5-prop-1 .statement tag=08UD}

*为了使$X$到$F$的映射$f$可测量，对于每个紧集$K \subset X$和每个数$\varepsilon > 0$，存在紧集$K_1 \subset K$是必要且充分的，使得$f$到$K_1$的$|\mu|(K - K_1) \leq \varepsilon$和限制是连续的。*

如果满足这个条件，我们可以递归地对不相交的紧集$K_n \subset K$进行定义递归序列，使得$|\mu|(K - \bigcup_{i=1}^n K_i) \leq 1/n$并且$f$的限制对于每个$K_n$是连续的（$§ 4$、No. 6、第 4 个）； $K_n$相对于并的$K$的补集可以忽略不计（$§ 4$，No. 5，Prop.7的Cor.），因此$f$是可测的。相反，假设存在由紧集组成的$K - N$的可忽略不计的集合$N \subset K$和划分$(K_n)$，使得$f$的限制对每个$K_n$是连续的；对于每一个$\varepsilon > 0$，都存在整数$n$，这样，如果$H = \bigcup_{i=1}^n K_i$，则$|\mu|(K - H) \leq \varepsilon$（§ 4, No. 5，第7号提案的Cor.）； 集合$H$是紧致的，$H$的$K_i$($1 \leq i \leq n$)形式到紧集的有限划分，$f$到每个$K_i$的限制是连续的；因此$f$到$H$的限制是连续的。

#### 命题 2 {#int-iv-s5-prop-2 .statement tag=08UE}

*让*$(F_n)$*成为拓扑空间的序列，并且对于每个*$n$，*让*$f_n$*成为*$X$*到*$F_n$的可测量映射。 *对于每个紧集*$K \subset X$*和每个*$\varepsilon > 0$，*存在紧集*$K_0 \subset K$*使得*$|\mu|(K - K_0) \leq \varepsilon$*和限制到*$K_0$*每个函数*$f_n$*是连续的*。

对于每个整数$n \geq 1$，都存在紧集$K_n \subset K$，使得$f_n$到$K_n$的$|\mu|(K - K_n) \leq \varepsilon / 2^n$和限制是连续的。 集合$K_0 = \bigcap_{n=1}^\infty K_n$是紧致的，函数$f_n$中的限制到$K_0$是连续的，并且由于$K - K_0$包含在$K - K_n$、$|\mu|(K - K_0) \leq \sum_{n=1}^\infty \varepsilon / 2^n = \varepsilon$的并中。

#### 定义 2 {#int-iv-s5-def-2 .statement tag=08UF}

*子集* $A$ *of* $X$ *如果其特征函数* $\varphi_A$ *可测量*，则称其为可测量。

鉴于Def。 1，同样可以说，可测量的集合$A$是集合，这样，对于每个紧集$K$，都存在可忽略不计的集合$N \subset K$和划分$(K_n)$ $K - N$由紧集的序列组成，其中每个都包含在$K \cap A$或$K \cap \complement A$中。

这个定义立即产生以下标准：

#### 命题 3 {#int-iv-s5-prop-3 .statement tag=08UG}

*对于集合* $A$ *可测量，对于每个紧集* $K$，$A \cap K$ *可积*是充分必要的。

条件是必要的，因为当$\sum_n |\mu|(A_n)$有限时，可积的集合$A_n$的序列的并是可积的（§ 4, No. 5，Prop.8的Cor.）。 条件是足够的，因为对于每个可积集合 $B$，存在可忽略不计的集合 $N \subset B$ 和划分 $B - N$ 到序列紧集 （§ 4, No. 6，第 4 章第 2 条）。

#### 推论 1 {#int-iv-s5-prop-3-cor-1 .statement tag=08UH}

*开放集合和封闭集合是可测量的*。

特别是，整个空间$X$是可测量的。

#### 推论 2 {#int-iv-s5-prop-3-cor-2 .statement tag=08UI}

— *如果 X 可度量，则 X* (GT, IX, §6, No. 2) 的每个 Souslin 子集 A *对于X* 上的每个测度 μ 都是 μ 可测的。

凭借命题3，足以证明每个相对紧的Souslin集合A都是μ可积的。现在，这样的集合 A 能够实现$|\mu|^*$（GT、IX, §6, No. 9、Th.5）。因此，对于每个 $\varepsilon > 0$ 都存在 A 的紧凑子集 K，使得 $|\mu|^*(A) \leq |\mu|^*(K) + \varepsilon = |\mu|(K) + \varepsilon$。令 U 为 X 包含于 A 中的相对紧开集合，使得

$$
|\mu|(U) = |\mu|^*(U) \leq |\mu|^*(A) + \varepsilon.
$$

然后$|\mu|^*(U - K) = |\mu|(U) - |\mu|(K) \leq 2\varepsilon$，因此$|\mu|^*(A - K) \leq 2\varepsilon$，证明A是μ可积的（§4, No. 6，Th.4的Cor.1）。

### 2. 原理本地化。局部可忽略不计集合

#### 命题 4（本地化的原理）{#int-iv-s5-prop-4 .statement tag=08UJ}

— *令 f 为 X 的映射成为拓扑空间 F。假设对于每个 $x \in X$，存在 x 的可积邻域 $V_x$ 和可测量的 X 的映射 $g_x$ 到 F 中，使得$f(y) = g_x(y)$几乎随处可见$V_x$。那么 f 是可测量的。*

令K为紧集；存在点 $x_i \in K$ 的有限数，使得 $V_{x_i}$ 形式覆盖 K。立即得出 (§4, No. 9，引理)，存在可忽略不计的集合 $N \subset K$ 和有限的划分 $K - N$由可积集合$M_j$组成，使得每个集合$K \cap V_{x_i}$是N的子集的并和$M_j$的某个数，并且使得在每个$M_j$上， $f$等于函数$g_{x_i}$之一。现在，对于每个$M_j$，都存在可忽略不计的集合、$N_j \subset M_j$和由紧集$K_{nj}\ (\mathbf{n} \in \mathbf{N})$的序列组成的$M_j - N_j$的划分；另一方面，对于每个$K_{nj}$，都存在由紧集$K_{mnj}\ (\mathbf{m} \in \mathbf{N})$的序列形成的可忽略不计的集合、$P_{nj} \subset K_{nj}$和$K_{nj} - P_{nj}$的划分，使得$f$的限制对于每个$K_{mnj}$ 是连续的。由于 N 的并，$N_j$ 和 $P_{nj}$ 可以忽略不计，$f$ 是可测的。

因此，可测量函数的概念是局部特征标的概念。

#### 定义 3 {#int-iv-s5-def-3 .statement tag=08UK}

— *如果对于每个$x \in X$，存在$x$的邻域$V$，使得$V \cap A$可以忽略不计，则称集合$A \subset X$是局部可忽略的（对于度量$\mu$）。*

通过本地化的原理，每个局部可忽略不计的集合都是*可测量的*。可忽略的集合 (§2) 的性质表明，局部可忽略的集合的每个子集都是局部可忽略的，并且局部可忽略的集合的每个可数并都是局部可忽略的。

#### 命题 5 {#int-iv-s5-prop-5 .statement tag=08UL}

— *为了使集合 A 局部可忽略不计，对于每个紧集 K，$A \cap K$ 可以忽略不计是必要且充分的。*

条件显然是足够的，因为X的每个点都有一个紧凑的邻域。这是必要的，因为如果对于每个$x \in K$，存在$x$的邻域$V_x$，使得$A \cap V_x$可以忽略不计，那么存在点$x_i \in K$的有限数，使得$V_{x_i}$形式a K 的覆盖，并且 $A \cap K$ 包含在可忽略的集合 $A \cap V_{x_i}$ 的并中。

#### 推论 1 {#int-iv-s5-prop-5-cor-1 .statement tag=08UM}

— *要使集合 A 可以忽略不计，其局部可忽略且外部测量有限是必要且充分的。*

条件显然是必要的。相反，如果满足，则A包含在可积开集合G中，它是可忽略的集合N的并和紧集的序列$(K_n)$（§ 4, No. 6，Th.4的Cor.2）；由于$A \cap N$和集合$A \cap K_n$可以忽略不计，因此它们的并A也是如此。

#### 推论 2 {#int-iv-s5-prop-5-cor-2 .statement tag=08UN}

— *每个局部可忽略的开集合都可以忽略不计*（因此包含在$\mu$的支持补中）。

因为，开集合G的外部测度是紧集$K \subset G$的测度$|\mu|(K)$的上等值（§ 4, No. 6，Th.4的Cor.4）；如果 G 局部可忽略不计，则对于 G 中包含的每个紧集 K，$|\mu|(K) = 0$，因此 $|\mu|^*(G) = 0$。

#### 推论 3 {#int-iv-s5-prop-5-cor-3 .statement tag=08UO}

— *在无穷大可数的局部紧凑空间 X 中，每个局部可忽略的集合都是可以忽略不计的。*

由于X是序列$(K_n)$或紧集的并，所以每个局部可忽略的集合A都是可忽略的集合$A \cap K_n$的并，因此可以忽略不计。

我们可以给出在无穷大不可数的局部紧致空间的例，以及空间X的测度，使得X中存在集合，其局部可忽略但不可忽略（§ 1，Exer.5）。

#### 推论 4 {#int-iv-s5-prop-5-cor-4 .statement tag=08UP}

— *令 f 为 X 的映射成为拓扑空间 F。如果 f 的不连续性的点的集合 N 局部可忽略，则 f 是可测的。*

对于每个紧集$K \subset X$，$K \cap N$可以忽略不计（命题5），因此，对于每个$\varepsilon > 0$，存在紧集$K_1 \subset K - (K \cap N)$使得$|\mu|(K - K_1) \leq \varepsilon$（§ 4, No. 6，Th.4），并且通过f到$K_1$的假设限制连续，从而结论。

如果 $P\{x\}$ 是性质，则性质 « *P\{x\} 局部几乎处处（相对于 $\mu$）» 通过定义等价于性质 «* x 的集合使得* (x $\in$ X 而不是$P\{x\}$) *局部可以忽略不计（对于测量* $\mu$）»。如果 F 是任意集合，则关系 «$f(x) = g(x)$ 局部几乎处处» 是 X 的映射的集合中的等价关系到 F 中。特别是，如果 F 是向量空间，则映射 $f$ X 代入 F 使得 f(x) = 0\text{ 局部几乎处处都被称为 } \textit{局部可忽略不计}。我们留给读者的任务是为这些概念建立大多数属性相应的，这些属性已经在§2、第4、5和6项中列举，函数几乎在任何地方都相等。我们将极限自己推论到注意到，如果X的两个\emph{连续}映射$f, g$进入豪斯多夫拓扑空间F，并且相等\emph{局部几乎处处}，则根据Cor，它们相等\emph{几乎处处}。提案 5 的第 2 条（因此在$\mu$ 的支持度每点处相等（§ 2, No. 4，提案 9））；然而，我们明确声明以下命题，即本地化的原理的直接的推论：

#### 命题 6 {#int-iv-s5-prop-6 .statement tag=08UQ}

*设 $f$ 为 X 的可测量映射到拓扑空间 F。X 到 F 的每一个映射，几乎在任何地方都等于 $f$，都是可测量的。*

### 3. 可测函数的基本性质

#### 定理 1 {#int-iv-s5-thm-1 .statement tag=08UR}

*令X为局部紧凑空间，$\mu$拓扑空间，$F = \prod_n F_n$其乘积的X，$(F_n)$序列的测度。对于每个指标 n，令$f_n$是X到$F_n$的可测量映射，并令$f(x) = (f_n(x)) \in F$；那么，对于 $f(X)$ 的每个连续映射 u 到拓扑空间 G，函数 $x \mapsto u(f(x))$ 是可测量的。*

对于X的每个紧凑子集 K和每个数$\varepsilon > 0$，存在紧集$K_1 \subset K$使得$|\mu|(K - K_1) \leq \varepsilon$并且使得所有函数$f_n$的限制到$K_1$是连续的（No. 1，提案 2）；显然$u \circ f$在$K_1$、从而定理上连续。

#### 注 {#int-iv-s5-n3-rem-1 .statement tag=08US}

— 1) 定理不扩展到拓扑空间的 \emph{任意} 乘积（例 1）。
2) 如果 $f$ 是 X 自身的连续映射，并且 $g$ 是 X 到 F 中的可测量的映射，则 $g \circ f$ 不一定是可测量的（Exer.2）。

#### 推论 1 {#int-iv-s5-thm-1-cor-1 .statement tag=08UT}

*可测量数值函数（有限或非有限）的有限数的上包络线和下包络线是可测量的。*
因为，$\sup(u, v)$和$\inf(u, v)$在$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$上连续。

#### 推论 2 {#int-iv-s5-thm-1-cor-2 .statement tag=08UU}

*要使数值函数 $f$（有限或非）可测量，$f^+$ 和 $f^-$ 可测量是充分必要的。*
Cor 需要条件。 1;这是足够的，因为映射$x \mapsto (f^+(x), f^-(x))$下$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$中X的像A不包含点$(+\infty, +\infty)$和$(-\infty, -\infty)$，因此映射$(u, v) \mapsto u - v$在A上连续。

#### 推论 3 {#int-iv-s5-thm-1-cor-3 .statement tag=08UV}

— *如果 f 和 g 是 X 的两个可测量映射到拓扑向量空间 F，则 f + g 和 αf 是可测量的（α 任何标量）。*

将 X 的可测量映射的集合转换为拓扑向量空间 F 因此为向量空间。

#### 推论 4 {#int-iv-s5-thm-1-cor-4 .statement tag=08UW}

— *设 F 为 R 上维数 n 的向量空间，并令 (e_k)_{1 \leq k \leq n} 为 F 的基。在阶中，函数 f = \和_{k=1}^{n} e_k f_k 可测，每个数值是充分必要的函数 f_k 是可测量的。*

#### 推论 5 {#int-iv-s5-thm-1-cor-5 .statement tag=08UX}

— *设 F, G, H 为三个拓扑向量空间，并设 (u, v) \to [u \cdot v] 为 F \times G 到 H 的连续双线性映射。如果 f 是 X 到 F 的可测映射，g 是 X 到 G 的可测映射，则[f \cdot g] 是 X 到 H 中可测量的映射。*

In particular, if f is a measurable mapping of X into a real (resp. complex) normed space F, and g is a measurable mapping of X into R (resp. C), then gf is measurable. 如果 F 是 *范数代数* 并且 f、g 是 X 的两个可测的映射到 F 中，则 fg 是可测的。

#### 推论 6 {#int-iv-s5-thm-1-cor-6 .statement tag=08UY}

— *如果 f 是 X 的可测量映射到标准化空间 F，则数值函数 |f|是可测量的。*

### 4. 可测量的极限函数

#### 定理 2（叶戈罗夫）{#int-iv-s5-thm-2 .statement tag=08UZ}

— *令X为局部紧凑空间，μ为X的测度，A为可数集合，$\mathfrak{F}$为A上具有可数基的过滤器，$(f_\alpha)_{\alpha \in A}$为X的可测映射族可度量空间 F。假设 $\lim_{\mathfrak{F}} f_\alpha(x) = f(x)$ 存在于 X 的局部可忽略的子集 N 的补集中。在这些条件下，
1° 函数 f（以任何方式扩展至 N）是可测量的；
2° 对于X和每个$\varepsilon > 0$的每个紧致子集 K，存在紧集$K_1 \subset K$，使得$|\mu|(K - K_1) \leq \varepsilon$和$f_\alpha$到$K_1$的限制是连续的并且均匀收敛到$K_1$上的f。

第一个断言显然是第二个的结果，我们将证明这一点。 存在紧集$K_0 \subset K$使得$|\mu|(K - K_0) \leq \varepsilon/2$并且所有函数$f_\alpha$中的限制到$K_0$是连续的（No. 1，命题2）。 对于过滤器$\mathfrak{F}$，令$(A_n)$为递减可数基；设 d 是 F 上与拓扑兼容的度量。 对于整数 $n > 0,\ r > 0$中的每一个对，令$B_{n,r}$为点$x \in K_0$中的集合，这样，对于指标$\alpha, \beta$属于中的至少一个对来说， $A_n$、$d(f_\alpha(x), f_\beta(x)) \geq 1/r$；对于固定的$\alpha$和$\beta$，$x \in K_0$的集合使得$d(f_\alpha(x), f_\beta(x)) \geq 1/r$在$K_0$内闭，因此是紧的；因而，$B_{n,r}$是包含在$K_0$中的紧集的可数并，因此是可积的（§ 4, No. 5，命题6和8）。 如果$r$固定，则集合$B_{n,r}$($n = 1, 2, \ldots$)的递减序列的交具有测度零，因为相对于过滤器$\mathfrak{F}$，$f_\alpha(x)$几乎在$K_0$中几乎所有地方都趋向于$f(x)$；因而$\lim_{n \to \infty} |\mu|(B_{n,r}) = 0$（§ 4, No. 5，第7条命题的Cor.），因此存在整数$n_r$使得$|\mu|(B_{n_r,r}) \leq \varepsilon/2^{r+2}$。 设$B$为集合$B_{n_r,r}$的并（对于$r = 1, 2, \ldots$）； $B$ 可积且

$$
|\mu|(B) \leq \sum_{r=1}^\infty |\mu|(B_{n_r,r}) \leq \varepsilon/4
$$

（§ 4, No. 5，Cor. of Prop. 8）。设$C$为$K_0$中$B$的补集；通过构造，$f_\alpha(x)$相对于滤波器$\mathfrak{F}$在$C$中均匀收敛到$f(x)$，并且由于$f_\alpha$到$C$的限制是连续的，$f$的限制也连续$C$。然后，从$|\mu|(K - K_1) = |\mu|(K - K_0) + |\mu|(B) + |\mu|(C - K_1) \leq \varepsilon$开始，取紧集$K_1 \subset C$就足够了，使得阶中的$|\mu|(C - K_1) \leq \varepsilon/4$到叙述的满足条件。

Th 的结论。如果 $F$ 不可度量，则 2 不一定成立（例 1）。如果 $F$ 可度量，并且集合 $A$ 不可数，但过滤器 $\mathfrak{F}$ 具有可数基，则 Th 的第一个结论。 2 再次有效；因为，如果$(A_n)$是$\mathfrak{F}$的可数基，并且$\alpha_n$是$A_n$的元素，那么$f$几乎在任何地方都是序列$(f_{\alpha_n})$的极限，因此是可测的；然而，Th的第二个结论。 2 不再必然有效（cf. Exer. 4）。

#### 推论 1 {#int-iv-s5-thm-2-cor-1 .statement tag=08V0}

— *令* $(f_n)$ *为数值函数（有限或非有限）的序列*。 *如果* $f_n$ *可测量，则函数* $\sup_n f_n$、$\inf_n f_n$、$\limsup_{n \to \infty} f_n$ *和* $\liminf_{n \to \infty} f_n$ *可测量*。

因为，扩展实直线 $\overline{\mathbf{R}}$ 同胚于紧区间 $\mathbf{R}$，是可度量的。 函数$\sup_n f_n$是函数$g_n = \sup(f_1, f_2, \ldots, f_n)$的递增序列的逐点极限，可测量（No. 3，Th.1的Cor.1）；类似地，$\limsup_{n \to \infty} f_n$是函数$h_n = \sup_{p \geq 0} f_{n+p}$的递减序列逐点极限，每个都可以通过前述方法测量。最后，由于$\inf_n f_n = -\sup(-f_n)$和$\liminf_{n \to \infty} f_n = -\limsup_{n \to \infty} (-f_n)$，这些函数是可测量的。

#### 推论 2 {#int-iv-s5-thm-2-cor-2 .statement tag=08V1}

— *可在* $X$ *形式部落* 中测量集合（GT，IX, §6, No. 3）。

因为，如果 M 和 N 可测量，则函数

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N \quad \text{and} \quad \varphi_{M \cap C_N} = \varphi_M - \varphi_M \varphi_N
$$

可以通过 No. 3 来衡量，Cors。 Th的3和5。 1. 如果 $(M_n)$ 是可测量的集合的序列，并且 M 是它们的并，则 $\varphi_M = \sup_n \varphi_{M_n}$ 可以通过 Cor 测量。 1 Th。 2、从而推论。

特别是，由于开集合是可测量的：

#### 推论 3 {#int-iv-s5-thm-2-cor-3 .statement tag=08V2}

*Borel 集合 in X* (GT, IX, §6, No. 3, Def. 4) *对于 X* 上的每个测量 $\mu$ 都可测量 $\mu$。

### 5. 判据用于可测量性

当F是拓扑向量空间时，在可测量的集合（§4, No. 9，Def.4）上的每一步函数，其中F中的值，显然是可测量的（No. 3，Th.1的Cor.3）；这样的函数$f$仅具有值的有限数，并且对于每个$y \in F$，$f^{-1}(y)$是可测量的。更一般地，令 F 为 X 的任何拓扑空间、$f$ 映射到 F 中，仅具有不同值 $a_i$ ($1 \leq i \leq m$) 的有限数；如果集合 $A_i = f^{-1}(a_i)$ 可测量，则函数 $f$ 可测量。因为，对于每个紧集 K 和每个集合 $A_i \cap K$，都存在由紧集的序列 $(K_{in})$ 组成的可忽略不计的集合 $N_i \subset A_i \cap K$ 和 $A_i \cap K \cap C N_i$ 的划分；由于K是集合$A_i \cap K$的并和$f$的限制，因此$K_{in}$都是常数，因此连续，$f$是可测的。通过滥用语言，我们可以说，X的映射$f$进入F是一个*可测量的步骤函数*，如果它只采用值的有限数，并且对于每个$y \in F$，$f^{-1}(y)$是可测量的。

#### 定理 3 {#int-iv-s5-thm-3 .statement tag=08V3}

*为了将 X 的映射 $f$ 转化为可测量的空间 F 可测量，对于每个紧集 $K \subset X$，存在可测量步骤序列 $(g_n)$ 是充分必要的函数，其中值在 F 中，这样，对于几乎每个 $x \in K$*，$g_n(x)$ 趋向于 $f(x)$。

条件对于 Egoroff 的定理和原理本地化来说就足够了。让我们证明这是必要的：到假设，存在由紧集组成的$K - N$的可忽略不计的集合$N \subset K$和划分$(K_m)$，使得$f$的限制对每个$K_m$是连续的。对于定义序列$(g_n)$，只需按以下方式进行即可：令$d$为与F的拓扑兼容的度量；对于每个 $K_i$ 和指标 $i \leq n$，存在 $K_i$ 的有限划分可积集合 $A_{ij}$ ($1 \leq j \leq q_i$) 足够小，使得$f$ 在每个 $A_{ij}$ 上的振荡为$\leq 1/n$（§ 4, No. 9，引理）；使$g_n$在每个$A_{ij}$上保持不变，等于此集合中$f$的值之一（对于$1 \leq i \leq n,\ 1 \leq j \leq q_i$），并且等于$X$中每个点的固定元素$a \in \mathbf{F}$不属于到任何 $A_{ij}$。很明显，序列$(g_n(x))$在$K$的每点收敛到$f(x)$，而不是属于到$N$。

#### 推论 1 {#int-iv-s5-thm-3-cor-1 .statement tag=08V4}

*令 $f$ 为 $X$ 可测量的映射到 Banach 空间 $F$；对于每个紧集$K \subset X$，存在可测量步骤函数的序列$(g_n)$，并且支持包含在$K$中，使得$|g_n(x)| \leq |f(x)|$对于所有$x \in X$并且使得对于几乎每个$g_n(x)$趋于$f(x)$ $x \in K$.*

与记号如Th的证明一样。 3，并且用$A_{ij}$中的$f$的值之一表示$a_{ij}$，则只要$|a_{ij}| \leq 1/n$和点就可以作为$A_{ij}$中的$g_n$的值，点0 $a_{ij}(1 - 1/(n|a_{ij}|))$ 否则；最后，集合$g_n(x) = 0$对$A_{ij}$($1 \leq i \leq n,\ 1 \leq j \leq q_i$)的并补。

#### 推论 2 {#int-iv-s5-thm-3-cor-2 .statement tag=08V5}

*令 $X$ 为局部紧致的空间，其无穷大可数。如果 $f$ 是 $X$ 的可测量映射到可测量的空间 $F$，则存在可测量步骤函数的序列 $(g_n)$，其中值在 $F$ 中，使得几乎每遇到 $x \in X$，$g_n(x)$ 都会倾向于 $f(x)$。*

若$X$为紧集递增序列$(A_n)$并，集合$A_n - A_{n-1}$即$X$非空形式划分可积集合；因而，存在由紧集的序列$(K_n)$形成的可忽略不计的集合$N \subset X$和$\mathbf{C}N$的划分，使得$f$的限制对每个$K_n$是连续的；然后可以像 Th 那样得出证明的结论。 3 无需修改。

#### 命题 7 {#int-iv-s5-prop-7 .statement tag=08V6}

*设$f$为$X$可测量的映射到拓扑空间$F$； $F$ 中每个关闭（或打开）集合的$f$ 下的逆像是可测量的。*

It suffices to carry out the proof for the inverse image $^{-1}f(A)$ of a closed set $A$ in $F$. 设$K$是$X$的紧子集；存在由紧集组成的可忽略不计的集合 $N \subset K$ 和 $K - N$ 的划分 $(K_n)$，使得 $f$ 的限制与每个 $K_n$ 是连续的。 因而，交$K_n \cap ^{-1}f(A)$是$f$至$K_n$的限制下封闭的集合$A$的逆像；因此它是$K_n$中的闭集合，因此是紧凑的。 因而，集合$K \cap ^{-1}f(A)$是可忽略的集合$N \cap ^{-1}f(A)$和紧集$K_n \cap ^{-1}f(A)$的并，这证明$^{-1}f(A)$是可测的。

#### 定理 4 {#int-iv-s5-thm-4 .statement tag=08V7}

— 令 F 为可度量的空间，令 d 为与拓扑兼容的 F 上的度量。为了使 X 的映射 f 进入 F 是可测量的，它满足以下两个条件是充分必要的：
a) F的每个闭球的f下的逆像是可测的；
b) 对于每个紧集 K ⊂ X，存在 F 的可数子集 H，使得几乎每个 $x \in K$ 都有 $f(x) \in \overline{H}$。

条件 a) 是第 7 条命题所必需的；另一方面，在Th的记号中。 3、 条件 b) 满足：取H为所有函数$g_n$的值构成的可数集合。

现在让我们证明条件 a) 和 b) 是充分的。令 K 为 X 的任何紧致子集； K 中存在一个可忽略的子集 N，使得 $f(K - N)$ 包含在 F 的点的可数集合闭包中，我们将其排列在序列 $(a_n)$ 中。令$A_{n,p}$为$x \in K - N$的集合，使得$d(f(x), a_n) \leq 1/p$。由条件 a) 可知 $A_{n,p}$ 是可测的。对于固定$p$，集合$B_{n,p} \subset K - N$递归设定的定义序列

$$
B_{1,p} = A_{1,p} \quad \text{and} \quad B_{n+1,p} = A_{n+1,p} \cap C \left( \bigcup_{k \leq n} A_{k,p} \right);
$$

集合$B_{n,p}$是可测量的，$K - N$的非空形式划分是可测量的。令$g_{m,p}$对于$1 \leq i \leq m$而言，函数等于集合$B_{i,p}$上的$a_i$，并且等于这些集合的并的补集上的常数$b \in F$； $g_{m,p}$是可测量的步长函数；由于$m$趋于无穷大，$g_{m,p}$在$B_{n,p}$（$n \geq 1$）上逐点收敛到函数$f_p$等于$a_n$，在$N \cup C K$上收敛到$b$，因此（Th.2）$f_p$是可测量的。由于$p$趋于无穷大，每$x \in K - N$，$f_p(x)$趋于$f(x)$，$x \in N \cup C K$趋于$b$；因此，$f_p$的极限是可测的，定位的原理证明了$f$本身是可测的。

#### 注 1 {#int-iv-s5-n5-rem-1 .statement tag=08V8}

条件 a) 单独不足以使 $f$ 可测量（Exer. 7）。

#### 注 2 {#int-iv-s5-n5-rem-2 .statement tag=08V9}

如果 F 的拓扑具有可数基，则 Th 的条件 b)。 4 自动满足 F 中 X 的每一个映射。此外，证明表明，假设逆像在有理半径闭球的 $f$ 之下就足够了，其中心属于为稠密可数子集 F，可测量集合。

#### 注 3 {#int-iv-s5-n5-rem-3 .statement tag=08VA}

假设a)可以用条件代替，F的每个空球的$f$下的逆像是可测的。

数值函数（有限或无限）的情况值得特别提及：

#### 命题 8 {#int-iv-s5-prop-8 .statement tag=08VB}

— 令 D 为 $\mathbf{R}$ 的可数稠密子集。在阶中，数值函数 $f$（有限或非）可测量，对于 $x \in X$ 的每个 $a \in D$、集合使得 $f(x) \geq a$ 可测量，就足够了（且必要）。

因为，如果是这样，对于$x$的每个$b \in \overline{\mathbf{R}}$集合，使得$f(x) \geqslant b$是可测量的，是$x$的集合（形式一个可数族）的交使得$f(x) \geqslant a$， $a$ 运行于 D 的点集合，即$\leqslant b$。 $x$的集合使得$f(x) < b$是可测量的，是可测量的集合的补集。接下来，如果$b$是有限的，则$x$的集合使得$f(x) \leqslant b$是可测量的，即$x$的集合的交使得$f(x) < b + 1/n$；并且$f(-\infty)^{-1}$是可测量的，是$x$的集合的交使得$f(x) < n$，因为$n$超过$\mathbf{Z}$。最后，$\overline{\mathbf{R}}$的每个闭区间的$f$下的逆像是可测的，即两个可测的集合的交，以及Th。可以应用4。

类似地，我们可以证明，对于$x$的每一个$a \in \mathrm{D}$，集合就足够了，这样$f(x) > a$是可测量的。

#### 推论{#int-iv-s5-n5-cor-1 .statement tag=08VC}

— *每个较低*（分别*较高*）*半连续函数是可测量的*。

因为，如果$f$是下半连续的，那么$x \in \mathrm{X}$的集合使得$f(x) \leqslant a$对于每个$a \in \overline{\mathbf{R}}$都是闭的。

当 F 可度量且*紧凑*时，Prop.7 使得锐化 Th 成为可能。 3如下：

#### 命题 9 {#int-iv-s5-prop-9 .statement tag=08VD}

— *如果 F 是可度量紧凑空间，则 X 到 F 中的每个可度量映射 f 都是可度量步骤函数* 的序列的一致极限（在所有 X 上）。

令$d$为与F的拓扑兼容的度量。对于每个正整数$n$，都存在点$a_k \in \mathrm{F}$的*有限*数，使得具有中心$a_k$和半径的闭球$B_k$ $1/n$ 形式 F 的覆盖；因而，集合 $A_k = f^{-1}(B_k)$ 是可测量的（第 7 条），并且形式覆盖了 X。因而，(§ 4, No. 9，引理)存在X的划分$(C_i)$到可测量集合的有限数，使得每个$A_k$是$C_i$中某些并。令$c_i$为$C_i$的点，并让$g_n$为可测量步长函数，等于$C_i$上的$f(c_i)$（对于每个指标$i$）。很明显，$d(f(x), g_n(x)) \leqslant 2/n$ 对于所有$x \in \mathrm{X}$。

#### 命题 10 {#int-iv-s5-prop-10 .statement tag=08VE}

— *设 F 为可分离的 Banach 空间，F' 为对偶，$(\mathbf{a}'_n)$ 单位 F' 球中的弱稠密序列（TVS，III, § 3, No. 4，第 6 命题的 Cor. 2）。*1 *为了使 X 的映射 f 进入 F 可测量，它对于每个 n 标量函数 $x \mapsto \langle \mathbf{f}(x), \mathbf{a}'_n \rangle$ 是可测量的*。

条件显然是必要的（No. 3，Th.1），让我们证明它是充分的；验证 Th 的条件 a) 就足够了。 4 并且，为此，

1 参见§ 2, No. 4末尾的脚注。

通过原理的定位就足以证明，对于X的每个紧凑子集 K和每个$B \subset F$，具有中心$a$和半径$r$，集合$A = K \cap f^{-1}(B)$是可测量的；现在，对于每 $z \in F$，

$$
|z| = \sup_n |\langle z, a'_n \rangle| / |a'_n|;
$$

因而 $A$ 是 $K$ 和集合的交定义为

$$
|\langle f(x), a'_n \rangle - \langle a, a'_n \rangle| \leq r |a'_n|;
$$

因为这些集合可以通过假设测量，所以 $A$ 是可以测量的。

#### 推论 1 {#int-iv-s5-prop-10-cor-1 .statement tag=08VF}

*设 F 为 Banach 空间。在阶中，X到F中的映射 f是可测的，满足以下两个条件是充分必要的：*

a) *对于每个 $a' \in F'$，标量函数 $x \mapsto \langle f(x), a' \rangle$ 是可测量的；*

b) *对于每个紧集 $K \subset X$，存在 F 的可数子集 H，使得 $f(x) \in \overline{H}$ 对于几乎每个 $x \in K$。*

条件的必要性由No. 3, Th 推出。 1、和钍。 4. 为了证明条件是充分的，再次验证Th的条件a)就足够了。 4. 对于第 10 条提案中的证明中的记号，我们可以（考虑到 b））假设，如果需要的话，之后在可忽略不计的集合上修改$f$，即 $f(K) \subset \overline{H}$，其中 $H$ 是可数的子集 $F$。如果$V$是集合$H \cup \{a\}$生成$F$的闭合线性子空间，则$V$是可分离的Banach空间，$V$上的每个连续线性形式都是形式的限制 $a' \in F'$；与命题 10 中相同的推理则表明$K \cap f^{-1}(B)$是可测量的。

#### 推论 2 {#int-iv-s5-prop-10-cor-2 .statement tag=08VG}

*设 F 为可度量且可分离的局部凸空间，并令 $F'$ 为其对偶。为了使 X 的映射 f 进入 F 可测量，对于每个 $a' \in F'$，标量函数 $x \mapsto \langle f(x), a' \rangle$ 可测量是必要且充分的。*

我们可以将F视为Banach 空间（TVS，II, §4, No. 3）的可数乘积$\prod_n E_n$的子空间，并且我们可以假设$\operatorname{pr}_n(F)$在$E_n$中稠密，因此是可分的。对于每个 $n$，映射 $\operatorname{pr}_n \circ f$ 都可以通过命题 10 来测量，因而 $f$ 可以通过 No. 3, Th 来测量。 1.

#### 命题 11 {#int-iv-s5-prop-11 .statement tag=08VH}

*设F为可分离可度量局部凸空间$F_n$的局部凸空间，即序列的直极限，F为$F_n$的并。令$F'$为F的对偶，配备弱拓扑$\sigma(F', F)$。为了使 X 到 $F'$ 的映射 f 可测量，对于每个 $a \in F$，标量函数 $x \mapsto \langle a, f(x) \rangle$ 可测量是必要且充分的。*

No. 3、Th 之前需要条件。 1;让我们证明它是足够的。首先假设 F 可度量且可分离，令 D 为 F 中的可数稠密集合。令 $(V_n)$ 为 F 中 0 的平衡凸开邻域的递减基序列；极坐标集合 $V_n^\circ$ 是等连续的，并且它们的并都是 $F'$。令 $X_n = f^{-1}(V_n^\circ)$； 序列$(X_n)$为递增和$X = \bigcup_n X_n$；让我们证明每个 $X_n$ 都是 $\mu$ 可测量的。事实上，$D \cap V_n$在$V_n$中是稠密的；对于每个$y \in D \cap V_n$，令$S_y$为$x \in X$的集合，使得$|\langle y, f(x) \rangle| \leq 1$； 假设意味着$S_y$ 中的每一个都是可测量的，$X_n$ 是$S_y$ 可数族中$y \in D \cap V_n$ 的交。因此，对于 X 的每个紧致子集 K 和每个 $\varepsilon > 0$，都存在整数 n 使得 $|\mu|(K - (K \cap X_n)) \leq \varepsilon/4$，然后存在 $K \cap X_n$ 的紧致子集 $K_1$ 使得 $|\mu|((K \cap X_n) - K_1) \leq \varepsilon/4$；最后，存在 $K_1$ 的紧致子集 $K_2$，使得 $|\mu|(K_1 - K_2) \leq \varepsilon/2$ 并且所有函数 $\langle y, f \rangle$ 的限制到 $K_2$，其中 $y \in D$ 是连续的（No. 1，命题 1）。 2）。由于集合$f(K_2) \subset f(X_n) \subset V_n^\circ$等连续，$\sigma(F', F)$在$f(K_2)$上诱导的拓扑与D中逐点收敛的拓扑相同（GT，X, §2, No. 4，Th.1）；因此，f 到 $K_2$ 的限制是连续的，在第一种情况下，从而我们的断言。

让我们讨论一般情况。如果$z'$是F上的连续线性形式，则其限制$z'_n$到$F_n$是连续的；从$F = \bigcup_n F_n$开始，F的对偶$F'$可以用乘积$\prod_n F'_n$的线性子空间（代数上）来识别，然后是$\operatorname{pr}_n(z') = z'_n$。此外，由于F的每个有限子集都包含在$F_n$之一中，因此拓扑$\sigma(F', F)$正是由拓扑$\sigma(F'_n, F_n)$的乘积拓扑引起的拓扑。既然如此，如果$\langle a, f \rangle$对于每个$a \in F$都是可测量的，那么对于每个n和每个$a_n \in F_n$来说$\langle a_n, \operatorname{pr}_n \circ f \rangle$也是可测量的，因为$\langle a_n, \operatorname{pr}_n \circ f \rangle = \langle a_n, f \rangle$； 证明的第一个部分则表明$\operatorname{pr}_n \circ f$对于每个n都是可测量的，因此f（No. 3，Th.1）也是可测量的。

### 6. 判据可积

#### 定理 5 {#int-iv-s5-thm-5 .statement tag=08VI}

— 在阶 X 的映射 f 转化为 Banach 空间 F 是第 p 个幂可积 ($1 \leq p < +\infty$) 时，f 可测且 $N_p(f)$ 有限是充分必要的。

条件是必要的：因为，如果$f \in \mathscr{L}_F^p$，则存在连续函数的序列$(g_n)$，具有紧支撑，几乎处处收敛于f（$§ 3$，No. 4，Th.3的Cor.2）；通过 Th。 No. 4中的2，f是可测的。

为了证明条件是充分的，我们首先建立引理：

#### 引理 1 {#int-iv-s5-lem-1 .statement tag=08VJ}

*设g为函数，F中为值，使得N_p(g) < +\infty*（在其他字中，在$\mathscr{F}_F^p$中为函数）。 *集合 A of 点 x \in X，使得 g(x) \neq 0 包含在可忽略的集合的并和紧集的序列中。*

令 $A_n$ 为点 $x \in X$ 中的集合，使得 $|g(x)| \geq 1/n$； A为$A_n$中的并、$\varphi_{A_n} \leq n|g|$、从而$|\mu|^*(A_n) \leq (n N_p(g))^p$；由此可见，$A_n$包含在可忽略不计的集合的并和紧集的序列中（§ 4, No. 6，Th.4的Cor.3），因此A也是如此。

引理证明，首先考虑 f 有 *compact* 支持 K 的情况。 1 Th。 No. 5中的3个，存在可测量步长函数的序列$(g_n)$，使得$|g_n(x)| \leq |f(x)|$在每个点$x \in X$并且$g_n(x)$几乎在任何地方都趋向于$f(x)$。此时，$g_n$是K中可测的集合的特征函数的线性组合；因为这些集合可以通过 No. 1、$g_n$ 属于到 $\mathscr{L}_F^p$ 的命题 3 进行积分。从$N_p(f) < +\infty$开始，勒贝格的定理（§ 3, No. 7，Th.6）表明f属于到$\mathscr{L}_F^p$。

一般情况下，从引理 1 可以得出，紧集存在递增序列 $(K_n)$，使得$f(x)$ 几乎在$K_n$ 的并的补码中都是零。令 $f_n$ 函数在 $K_n$ 上等于 $f(x)$，在其他地方等于 0； $f_n$ 可通过 No. 3 测量，Cor。 5 Th。 1;从参数的第一个部分开始，从 $|f_n| \leq |f|$、$f_n$ 属于到 $\mathscr{L}_F^p$。由于$f(x)$几乎处处都等于序列$f_n(x)$的极限，勒贝格的定理再次证明$f \in \mathscr{L}_F^p$，从而完成证明。

应该注意注函数 *局部可忽略但不可忽略* 不可积；因此，函数*局部几乎处处*等于可积函数不一定是可积的。

#### 推论 1 {#int-iv-s5-lem-1-cor-1 .statement tag=08VK}

*为了使集合可积，它是可测的并且具有有限的外部测度是必要且充分的。*

#### 推论 2 {#int-iv-s5-lem-1-cor-2 .statement tag=08VL}

*设$(F_n)$为拓扑空间的序列；对于每个指标 n，令$f_n$是X到$F_n$的可测量映射，并令$f(x) = (f_n(x)) \in F = \prod_n F_n$；最后，让 u 成为 Banach 空间 G 的连续映射 $f(X)$。要使函数 $g(x) = u(f(x))$ 可积，$N_1(g) < +\infty$ 是充分必要的。*

因为，g 是可测量的（No. 3，Th.1）。

#### 推论 3 {#int-iv-s5-lem-1-cor-3 .statement tag=08VM}

*对于每个可积函数 f 和每个可测量的集合 A，函数 $f \varphi_A$ 都是可积的。*

因为，它是从 Th 得出的。 5 和 No. 3，科罗纳。 5 Th。 1 $f \varphi_A$是可测量的，并且$N_1(f \varphi_A) \leq N_1(f)$。

我们为每个可积函数$f$和每个可测量的集合$A$写$\int_A f d\mu = \int f \varphi_A d\mu$（或$\int_A f \mu$）。我们还为每个数字函数（有限或无限）$f \geqslant 0$（如果$f(x) = +\infty$和$\varphi_A(x) = 0$，则在设定$f(x)\varphi_A(x) = 0$）写$\int^* f d|\mu|$（或$\int^*_A f |\mu|$）来代替$\int^* f \varphi_A d|\mu|$。

#### 推论 4 {#int-iv-s5-lem-1-cor-4 .statement tag=08VN}

*对于每个序列* $(f_n)$ *可测量的函数* $\geqslant 0$ *在* $X$，

$$
\int^*\left( \sum_n f_n \right) d|\mu| = \sum_n \int^* f_n d|\mu|.
$$

鉴于§1, No. 3，Th。 3，对于$X$上任意两个可测量的函数$f \geqslant 0, g \geqslant 0$，我们减少到证明，

$$
\int^*(f + g) d|\mu| = \int^* f d|\mu| + \int^* g d|\mu|.
$$

这无非是当$f$和$g$可积时积分的可加性。相反的情况，如果例$f$不可积，则$\int^* f d|\mu| = +\infty$乘Th。 5； *更不必说*，$\int^*(f + g) d|\mu| = +\infty$。

#### 推论 5 {#int-iv-s5-lem-1-cor-5 .statement tag=08VO}

*对于每对序列* $(A_n)$ *成对不相交的可测量集合*，

$$
|\mu|^*\left( \bigcup_n A_n \right) = \sum_n |\mu|^*(A_n).
$$

这是从 Cor 得出的。 4应用于$\varphi_{A_n}$。

### 7. 在局部紧凑子空间上引发的测量

令$X$为局部紧凑空间，$\mu$为$X$的测度，$Y$为$X$的*局部紧凑子空间*。由于$Y$是$X$中开集合和闭集合的交（GT，I, §9, No. 7，命题12），它是$\mu$可测的（No. 1，命题3的Cor.）。对于每个函数$g \in \mathscr{H}(Y; \mathbf{C})$，令$g'$为函数，在所有$X$上定义，在$Y$上等于$g$，在$X - Y$上等于0；让我们证明 $g'$ 是 $\mu$-*可积*。我们可以将自己限制在$g$是实数且$\geqslant 0$的情况（将$g$写为函数的线性组合）；由于$g'$是有界的并且具有紧支持，因此足以证明$g'$是$\mu$可测的（No. 6，Th.5）；但这是因为$g'$在$X$上是上半连续的（No. 5，Prop.8的Cor.）。因此，我们可以做出以下定义：

#### 定义 4 {#int-iv-s5-def-4 .statement tag=08VP}

— *给定局部紧凑空间X的局部紧凑子空间Y，我们将X上的测度$\mu$在Y上诱发测度，并用$\mu_Y$或$\mu|Y$表示，由公式定义的测度*

$$
\int g \, d\mu_Y = \int g' \, d\mu
$$

*对于每个函数$g \in \mathscr{K}(Y; \mathbf{C})$，其中$g'$表示函数在$Y$上等于$g$，在$X - Y$上等于0。*

#### 例 {#int-iv-s5-n7-exa-1 .statement tag=08VQ}

— 令 $\mu$ 为 $\mathbf{R}$、I *$\mathbf{R}$ 中的任何*区间的勒贝格测度； I是$\mathbf{R}$的局部紧子空间，$\mu$在I上诱发的测度是线性形式

$$
g \mapsto \int_a^b g(x) \, dx
$$

在$\mathscr{K}(I; \mathbf{C})$，其中$a$和$b$是I（cf.§ 4, No. 4，*例*）的端点（有限或非），在其他字，我们称之为*勒贝格测度I*。

当 Y 是 X 的*开* 子空间时，Def. 4 重合和定义由 $\mu$ 在 Y 上引起的测量（或 $\mu$ 到 Y 的限制）在第 1 章中给出。 III, §2, No. 1：确实，对于每个函数$g \in \mathscr{K}(Y; \mathbf{C})$函数$g'$，那么在X上连续。

我们将在第 1 章中详细研究关于诱导测度的积分。 V, §7，在那之前我们只需要以下结果：

#### 引理 2 {#int-iv-s5-lem-2 .statement tag=08VR}

— *令$\mu$为X的正测度，令K为X的紧子集。*

(i) *对于每个紧凑（或开放）子集 K* 的 H，$\mu_K(H) = \mu(H)$。

(ii) *为了使 K 的子集 N $\mu_K$-可忽略，其充分必要为$\mu$-可忽略*。

(iii) *如果S是$\mu_K$的支持，则*$\mathrm{Supp}(\mu_S) = S$。

(i) 我们可以将自己限制在 H 是紧的情况。 用$f$表示空间K中H的特征函数； $f$是上半连续，因此是$\mathscr{K}_+(K)$中函数的递减有向族$(g_\alpha)$的下包络线；我们有 $\mu_K(H) = \inf_\alpha \int g_\alpha \, d\mu_K$（§ 4, No. 4，第 5 条命题的 Cor.2）。 If $g'_\alpha$ is the function equal to $g_\alpha$ on K and to 0 on $X - K$, then $g'_\alpha$ is upper semi-continuous, and the lower envelope of the decreasing directed family $(g'_\alpha)$ is the characteristic function $\varphi_H$ of H in the space X; therefore

$$
\mu(H) = \inf_\alpha \int g'_\alpha \, d\mu = \inf_\alpha \int g_\alpha \, d\mu_K = \mu_K(H)
$$

由（1）。

(ii) 如果 N 是$\mu$-可忽略不计，则对于每个 $\varepsilon > 0$，X 中存在一个相对紧凑的 N 开邻域 U，使得 $\mu(U) \leq \varepsilon$；由于 $K - (U \cap K)$ 是紧致的，因此从 (i) 可以得出 $\mu_K(U \cap K) \leq \mu(U) \leq \varepsilon$，因此 N $\mu_K$ 可忽略不计。相反，如果 N 是 $\mu_K$ 可忽略不计，则在 X 中存在 N 的开邻域 V，使得 $\mu_K(V \cap K) \leq \varepsilon$；通过(i)，我们有$\mu(V \cap K) = \mu_K(V \cap K)$，因此$\mu(N) = 0$，因为$\varepsilon$是任意的。

(iii) 对于 K 中与 S 相交的每个开路集合 U，通过假设 $\mu_K(U \cap S) \neq 0$，因此通过 (i) 开$\mu(U \cap S) \neq 0$，并且由于 $U \cap S$ 在 S 中开路，因此通过 (i) 开$\mu_S(U \cap S) \neq 0$；因为 S 中的每个非空开集合都是形式 $U \cap S$，其中 U 在 K 中开路，这证明了 $\operatorname{Supp}(\mu_S) = S$。

#### 引理 3 {#int-iv-s5-lem-3 .statement tag=08VS}

*设 Y 为 X 的局部紧凑子空间；对于 X、$|\mu_Y| = |\mu|_Y$ 上的每个测量$\mu$。*

设f为$\mathscr{K}_+(Y)$和$\varepsilon$中的函数，任意数$> 0$；到定义，存在函数$g \in \mathscr{K}(Y; \mathbf{C})$使得$|g| \leq f$和$|\mu_Y|(f) \leq |\mu_Y(g)| + \varepsilon$。分别用将 f 和 g 扩展为 0 在 $X - Y$ 上得到的 $f'$ 和 $g'$ 函数表示，我们有 $\mu_Y(g) = \mu(g')$，并且从 $|g'| \leq f'$ 开始，

$$
|\mu(g')| \leq |\mu|(|g'|) \leq |\mu|(f') = |\mu|_Y(f),
$$

从而 $|\mu_Y|(f) \leq |\mu|_Y(f) + \varepsilon$ 并且，由于 $\varepsilon$ 是任意的，

$$
|\mu_Y|(f) \leq |\mu|_Y(f).
$$

另一方面，令 K 为 f 的支持，并令 U 为 K 在 X 中的紧邻域，使得 $|\mu|(U - K) \leq \varepsilon$；根据 Urysohn 的定理，存在函数 $f_1 \in \mathscr{K}_+(X)$，扩展 f，且支持包含在 U 中，并且$\|f_1\| = \|f\|$。存在函数$h_1 \in \mathscr{K}(X; \mathbf{C})$使得$|h_1| \leq f_1$和$|\mu|(f_1) \leq |\mu(h_1)| + \varepsilon$。如果 h 是 $h_1$ 到 Y 的限制，则$h \in \mathscr{K}(Y; \mathbf{C})$、$|h| \leq f$ 和 $\mu(h_1) - \mu_Y(h) = \mu(h_1 \varphi_{U-K})$，因此

$$
|\mu(h_1) - \mu_Y(h)| \leq \|f\| \cdot |\mu|(U - K) \leq \varepsilon \|f\|;
$$

此外，我们还有类似的

$$
|\mu|(f_1) - |\mu|_Y(f) = |\mu|(f_1 \varphi_{U-K}) \quad \text{and} \quad ||\mu|(f_1) - |\mu|_Y(f)|| \leq \varepsilon \|f\|.
$$

由此我们推断

$$
|\mu|_Y(f) \leq |\mu_Y(h)| + \varepsilon(1 + 2\|f\|) \leq |\mu_Y|(f) + \varepsilon(1 + 2\|f\|)
$$

由于$\varepsilon$是任意的，$|\mu|_Y(f) \leq |\mu_Y|(f)$可以完成证明。

### 8. $\mu$-紧集的密集族

#### 命题 12 {#int-iv-s5-prop-12 .statement tag=08VT}

— 令 $\mu$ 为局部紧致空间 $X$、$A$ $X$ 的 $\mu$ 可测量子集，以及 $A$ 紧致子集的 $\mathscr{K}$ 集合满足以下条件：
(PLI) $\mathscr{K}$ 属于到 $\mathscr{K}$ 的每个封闭（因此紧凑）子集集合。
(PLII) $\mathscr{K}$ 属于到$\mathscr{K}$ 的集合的每个有限并。
那么以下四个属性是等效的：
a) 为了使$A$中的子集$B$局部$\mu$可以忽略不计，$|\mu|^*(B \cap K) = 0$对于所有$K \in \mathscr{K}$来说是必要且充分的。
b) 对于$A$和每个$\varepsilon > 0$的每个紧凑子集$K_0$，都存在集合$K \in \mathscr{K}$，包含在$K_0$中，因此$|\mu|(K_0 - K) \leq \varepsilon$。
c) 对于$A$的每个紧凑子集$B$，存在$B$的划分，由$\mu$可忽略不计的集合$N$和序列$(H_n)$形成紧集属于至$\mathscr{K}$。
d) 对于$A$的每个紧凑子集$B$，存在紧集属于到$\mathscr{K}$的递增序列$(K_n)$，包含在$B$中，使得集合 $N = B - \bigcup_n K_n$ 是$\mu$——可以忽略不计。

对于$p \leq n$，取$K_n$为$H_p$的并，并引用（PLII），d）意味着$a); c)$意味着d），这是直接的（No. 2，命题5）。为了证明 b) 蕴含 c)，需要递归地计算 $\mathscr{K}$ 的集合的定义序列 $(H_p)$，使得 $H_{n+1} \subset B - \bigcup_{p \leq n} H_p$ 和 $|\mu|(B - \bigcup_{p \leq n} H_p) \leq 1/n$ (§ 4, No. 6, Th. 4)。

仍有待证明a）蕴涵b）。让我们用反证法来论证，假设$K$超过$K_0$属于到$\mathscr{K}$的子集的集合，数$|\mu|(K)$的上界$\alpha$是$< |\mu|(K_0)$。通过(PLII)，存在$K_0$、属于到$\mathscr{K}$的紧致子集的递增序列$(L_n)$以及$\sup_n |\mu|(L_n) = \alpha$。 集合$B = \bigcup_n L_n$； $B$ 可积且$|\mu|(B) = \alpha$，因此$|\mu|(K_0 - B) = |\mu|(K_0) - \alpha > 0$。另一方面，我们将看到对于每一个集合 $K \in \mathscr{K}$，$|\mu|(K \cap (K_0 - B)) = 0$，根据 a)，这将意味着矛盾。事实上，如果存在集合$K \in \mathscr{K}$使得$|\mu|(K \cap (K_0 - B)) > 0$，那么就会存在$K \cap (K_0 - B)$的紧子集$H$使得$|\mu|(H) > 0$。通过 (PLI)，我们将得到 $H \in \mathscr{K}$，并且对于 $n$ 足够大，

$$
|\mu|(L_n \cup H) = |\mu|(L_n) + |\mu|(H) > \alpha .
$$

但是通过（PLII）$L_n \cup H$属于到$\mathscr{K}$，以及$\alpha$的与……矛盾定义。

#### 定义 6 {#int-iv-s5-def-6 .statement tag=08VU}

— 令 $A$ 为 $X$ 的 $\mu$ 可测量子集。 $A$的紧致子集的集合$\mathscr{K}$如果满足第12条的条件(PLI)、(PLII)、$a), b), c), d)$，则称其在$A$中是$\mu$稠密。

*所有*紧凑的集合，$A$的子集在$A$中是$\mu$密集。

当$A = X$时，我们将简单地说“$\mu$-密集集合”来代替“集合$\mu$-密集$X$”。如果$X - A$局部$\mu$可忽略不计，则$A$的紧致子集的每个集合在$A$中是$\mu$稠密，在$X$中也是$\mu$稠密。

#### 注 {#int-iv-s5-n8-rem-1 .statement tag=08VV}

— 假设 $A$ 是序列 $(L_n)$ 的紧集的并以及$\mu$ 可忽略不计（分别是局部 $\mu$ 可忽略）集合，并令 $\mathscr{K}$ 为紧致的集合子集即 $A$ 中的 $\mu$ 密集。 应用到第12条的叙述的每个$L_n$性质*c*)，我们看到$A$是紧集*属于到*$\mathscr{K}$的并序列和a $\mu$-可忽略（分别为本地$\mu$-可忽略）集合。

如果$K$是$X$的紧致子集，那么就可以说$K$的紧致子集的集合是$K$中的$\mu$-稠密，或者说它是$\mu_K$-*稠密* $K$；这是从第 12 号提案的 No. 7 和条件 *b*) 的引理 2 和 3 得出的。

#### 命题 13 {#int-iv-s5-prop-13 .statement tag=08VW}

*令$A$为$X$的$\mu$可测子集，紧致子集的$\mathscr{K}$集合，即$A$中的$\mu$稠密。令 $\mathfrak{H}$ 为 $A$ 满足 (PL$_I$) 和 (PL$_{II}$) 的紧凑子集的集合，这样，对于 $H \in \mathfrak{H}$ 的每个$K \in \mathscr{K}$、集合，使得$H \subset K$ 是 $K$ 中的$\mu_K$-*稠密*（或者，相当于 $\mu$-*稠密*）。那么 $\mathfrak{H}$ 是 $A$ 中的 $\mu$ 密集。*

例如，令 $L$ 为 $A$ 的紧致子集。对于每个$\varepsilon > 0$，存在一个$K \in \mathscr{K}$，使得$K \subset L$和$|\mu|(L - K) \leq \varepsilon/2$，然后存在一个$H \in \mathfrak{H}$，使得$H \subset K$和$|\mu|(K - H) \leq \varepsilon/2$；由此可见$|\mu|(L - H) \leq \varepsilon$、从而命题。

### 9. 本地可数划分

#### 定义 7 {#int-iv-s5-def-7 .statement tag=08VX}

*拓扑空间$T$的子集的集合$\mathfrak{A}$被称为“局部可数”，如果对于每个$t \in T$，存在$t$的邻域$V$，使得集合与 $V$ 相交的 $A \in \mathfrak{A}$ 是可数的。*

如果$T$的子集的集合$\mathfrak{A}$是局部可数的，那么对于$T$的每个紧凑子集$K$，与$K$相交的$A \in \mathfrak{A}$的集合是可数的，因为$K$可以是被有限的数个点$K$的开放邻域覆盖，每个邻域仅与子集属于到$\mathfrak{A}$的可数个集合相交。

Def. 7 shows that the *union* of a locally countable set of $\mu$-measurable (resp. locally $\mu$-negligible) subsets of a locally compact space is $\mu$-measurable (resp. locally $\mu$-negligible) (No. 1, Prop. 3 and No. 2, Prop. 5).

#### 命题 14 {#int-iv-s5-prop-14 .statement tag=08VY}

*令$X$为局部紧致空间，$\mu$为$X$的测度，$A$为$X$的$\mu$可测子集，以及$\mathscr{K}$集合为子集的紧致$A$ 即 $A$ 中的 $\mu$ 密集。存在局部可数的集合$\mathfrak{H} \subset \mathscr{K}$，由成对不相交的集合组成，使得$A - \bigcup_{K \in \mathfrak{H}} K$在局部$\mu$可以忽略不计，并且对于每个$K \in \mathfrak{H}$，$\mu_K$的支持度都是$K$。*

考虑集合$\mathscr{L} \subset \mathfrak{K}$由成对的不相交的集合组成，这样，对于每个$L \in \mathscr{L}$，$\operatorname{Supp}(\mu_L) = L$。 $\mathscr{P}(\mathfrak{K})$的集合$\mathscr{L}$形式子集$\mathscr{H}$即非空（因为包含元素$\varnothing$），我们将阶乘关系包含在$\mathscr{P}(\mathfrak{K})$中。 $\mathscr{H}$*感性*的是直接的；设$\mathfrak{H}$为$\mathscr{H}$（S，R，§6, No. 10）中的极大元素。让我们首先证明 $\mathfrak{H}$ 是“局部可数”。事实上，对于每个$x \in X$，让$V$成为$x$的一个相对紧凑的开邻域；如果 $(K_i)_{1 \leq i \leq n}$ 是与 $V$ 相交的 $\mathfrak{H}$ 的不同集合的有限族，则

$$
\sum_{i=1}^n |\mu|(K_i \cap V) = |\mu|\left(V \cap \left( \bigcup_{i=1}^n K_i \right)\right)
$$

因为$K_i$是成对的不相交的、从而$\sum_{i=1}^n |\mu|(K_i \cap V) \leq |\mu|(V)$。由此可见，如果 $\mathfrak{H}_V$ 是与 $V$ 相交的 $K \in \mathfrak{H}$ 的集合，则

$$
\sum_{K \in \mathfrak{H}_V} |\mu|(K \cap V) < +\infty,
$$

并且由于 $|\mu|(K \cap V) > 0$ 对于每个 $K \in \mathfrak{H}_V$，$\mathfrak{H}_V$ 必然是可数的。接下来，让我们证明$N = A - \bigcup_{K \in \mathfrak{H}} K$在局部$\mu$可以忽略不计。我们在上面看到$N$是$\mu$可测的。如果$N$不是局部可忽略的，那么包含将是不可忽略的紧集$L_0$，因此（No. 8，命题12）不可忽略的紧集$L \subset L_0$属于到$\mathfrak{K}$。由于$|\mu_L|(L) = |\mu|(L) > 0$（No. 7、引理 2和3），$\mu$在$L$上引发的测度$\mu_L$为非零的；因此，它的支持$S$是非空紧集属于到$\mathfrak{K}$（PL₁），以及$\operatorname{Supp}(\mu_S) = S$（No. 7，引理2，（iii））。由此可见集合$\mathfrak{H} \cup \{S\}$属于到$\mathscr{H}$，其中与……矛盾定义$\mathfrak{H}$；因此，集合$N$在局部可以忽略不计，从而完成证明。

### 10. 可测量函数定义在可测量子集上

#### 命题 15 {#int-iv-s5-prop-15 .statement tag=08VZ}

*令$X$为局部紧凑空间，$\mu$为$X$的测度，$A$为$X$的$\mu$可测子集，以及$f$映射 $A$ 变为拓扑空间 $F$。以下条件是等效的：

a) $A$的紧致子集$K$的集合$\mathfrak{H}$使得$f$到$K$的限制是连续的，在$A$中是$\mu$稠密。

b) $A$的紧子集存在集合$\mathfrak{K}$，$A$中存在$\mu$密集，使得$f$的限制对每个$K \in \mathfrak{K}$是$\mu_K$可测。

c) 拓扑空间 $G$ 的$F$ 到子空间存在同胚 $j$，以及 $X$ $G$ 的 $\mu$ 可测映射 $g$，使得$g|A = j \circ f$.*

d) $f$ 的扩张到$X$ 的映射进入$F$，在$X - A$ 上恒定，$\mu$ 可测。

显然，a) 隐含 b)，d) 隐含 c)。 c) 隐含 a) 的事实源自No. 8 的第 12 条命题条件 c)。另一方面，b) 意味着 a)：for, Def。图1表明，对于每个$K \in \mathscr{K}$，$K$中包含的子集$H \in \mathscr{H}$的集合在$K$中是$\mu_K$密集（No. 8，命题12，c）），并且No. 8的命题13表明： $\mathscr{H}$ 是 $A$ 中的 $\mu$ 密集。仍有待观察 a) 是否隐含 d)。令$g$为$f$到$X$的扩张，恒定于$X - A$。对于$X$的每个紧致子集$L$，$L \cap A$和$L \cap (X - A)$都是$\mu$可积的；因此，对于每个 $\varepsilon > 0$，都存在一个紧致子集 $P \subset L \cap A$ 和一个紧致子集 $Q \subset L \cap (X - A)$，使得

$$
|\mu|((L \cap A) - P) \leq \varepsilon/4 \quad \text{and} \quad |\mu|\left((L \cap (X - A)) - Q\right) \leq \varepsilon/4.
$$

另一方面，$P$中存在集合$H \in \mathscr{H}$，使得$|\mu|(P - H) \leq \varepsilon/2$； $g$到紧集$K = H \cup Q$的限制是连续的（$g$在$Q$上恒定）和$|\mu|(L - K) \leq \varepsilon$，从而完成证明。

#### 定义 8 {#int-iv-s5-def-8 .statement tag=08W0}

*令$X$为局部紧凑空间，$\mu$为$X$的测度，$A$为$X$的$\mu$可测子集。将 $A$ 的映射 $f$ 转换为拓扑空间 $F$，如果满足命题 15 的等价条件，则称其为 $\mu$ 可测。

如果 $A$ 局部 $\mu$ 可以忽略不计，那么 $A$ 到 $F$ 的*每个* 映射都是 $\mu$ 可测量的。

#### 推论 1 {#int-iv-s5-def-8-cor-1 .statement tag=08W1}

*令$X$为局部紧凑空间，$\mu$为$X$的测度，$A$为$X$的$\mu$可测子集，以及$f$为$\mu$可测将$A$的映射转换为拓扑空间$F$。令$\mathscr{K}$为$X$的紧致子集的集合，$\mu$-稠密于$X$。那么，存在由局部可忽略的集合$N$和集合$K_\lambda \in \mathscr{K}$的局部可数族$(K_\lambda)_{\lambda \in L}$组成的$A$的划分，使得$f|K_\lambda$对于每个$\lambda \in L$都是连续的。

鉴于No. 9，第14条命题，足以证明子集$K \in \mathscr{K}$的集合$\mathscr{H} \subset \mathscr{K}$使得$K \subset A$和$f|K$是连续的，在$A$中是$\mu$稠密。现在，从No. 1的第1条和第15条的条件d)可以立即得出，对于$A$的每个紧凑子集$K_0$和每个$\varepsilon > 0$，存在子集$K \subset K_0$属于 $\mathscr{K}$使得$|\mu|(K_0 - K) \leq \varepsilon$和$f|K$是连续的；因此，结论来自于No. 8的第12条命题。

#### 推论 2 {#int-iv-s5-def-8-cor-2 .statement tag=08W2}

*令$K$为$X$的紧致子空间；在阶中，$K$的映射$f$变成拓扑空间$F$是$\mu$可测，它是$\mu_K$可测是充分必要的。*

鉴于No. 7的引理2，这立即来自No. 1的提案1和提案15的条件a)。

#### 命题 16 {#int-iv-s5-prop-16 .statement tag=08W3}

*令$\mathfrak{A}$为$\mu$的局部可数集合-可测量$X$的子集，并令$B = \bigcup_{A \in \mathfrak{A}} A$。为了使$B$的映射$f$成为空间$F$是$\mu$可测的，$f$的限制对每个$A \in \mathfrak{A}$是必要且充分的$\mu$-可测量。*

我们已经观察到 (No. 9) $B$ 是 $\mu$ 可测的。 条件显然是必要的，让我们证明它是充分的。因此，令 $K$ 为 $B$ 的紧致子集。到假设，存在集合属于到$\mathfrak{A}$的序列$(A_n)$，使得$K \cap A_n$形式覆盖$K$。 集合$C_0 = K \cap A_0$ 和
$$
C_n = K \cap A_n \cap \mathbf{C}\left( \bigcup_{i < n} C_i \right)
$$
对于$n > 0$，使得$K$的非空$C_n$形式划分变成$\mu$可积集合。由于$f$到$C_n$的限制是$\mu$可测量的，因此存在由$\mu$可忽略的集合$N_n$和序列形成的$C_n$的划分紧集的$(L_{mn})_{m \geq 0}$使得$f|L_{mn}$是连续的。由于 $N = \bigcup_n N_n$ $\mu$ 可以忽略不计，我们看到第 15 条命题的条件 a) 得到满足，从而命题。

提案 15 的性质 d) 使得可以立即将在第 2 至 5 条中观察到的在所有 $X$ 上定义的可测量函数的属性推广到在 $X$ 的可测量子集 $A$ 上定义的可测量函数；这些推广留给读者。我们仅明确指出，当假设函数 $g_x$ 中的每一个仅在 $V_x$ 中定义（或$V_x$ 中几乎所有位置）且可测量时，点本地化的原理（No. 2，命题 4）仍然有效。

### 11. 度量收敛

Let $X$ be a locally compact 空间, $\mu$ a measure on $X$, $A$ a $\mu$-measurable 子集 of $X$, and $F$ a *uniform 空间*; we shall denote by $\mathscr{S}(A, \mu; F)$, or $\mathscr{S}_F(A, \mu)$ (or simply $\mathscr{S}_F(\mu)$, or even $\mathscr{S}_F$, when $A = X$) 集合 of $\mu$-*measurable 映射 of $A$ into $F*$ （No. 10，默认值 8）。 For every entourage $V$ of the uniform 结构 of $F$, every $\mu$-integrable 集合 $B \subset A$ and every 数 $\delta > 0$, we shall denote by $W(V, B, \delta)$ 集合 of 对 $(f, g)$ of 函数 in $\mathscr{S}(A, \mu; F)$ having the following 性质: 集合 $M$ of all $x \in B$ for which $(f(x), g(x)) \notin V$ is such that $|\mu|^*(M) \leq \delta$. Let us show that 集合 $W(V, B, \delta)$ 形式 a *fundamental 系统 of entourages* for a uniform 结构 on $\mathscr{S}(A, \mu; F)$: it is clear that $W(V, B, \delta)$ is symmetric if $V$ is, and that if $V' \subset V,\ B' \supset B$ and $\delta' \leq \delta$，那么

$$
W(V', B', \delta') \subset W(V, B, \delta);
$$

it therefore suffices to verify the axiom $(U'_{III})$ (GT, II, §1, No. 1). Now, if $V'$ is an entourage such that ${V'}^2 \subset V$, then

$$
W(V', B, \delta/2) \circ W(V', B, \delta/2) \subset W(V, B, \delta).
$$

注 that as $K$ runs over a $\mu$-dense 集合 $\mathfrak{K}$ of *compact* 子集 of $A$, 集合 $W(V, K, \delta)$ also 形式 a fundamental 系统 of entourages for the preceding uniform 结构: for, for every integrable 集合 $B \subset A$, there exists 紧集 $K \in \mathfrak{K}$ contained in $B$ such that $|\mu|(B - K) \leq \delta$, and therefore $W(V, K, \delta) \subset W(V, B, 2\delta)$.

#### 定义 9 {#int-iv-s5-def-9 .statement tag=08W4}

*uniform 结构 on $\mathscr{S}(A, \mu; F)$ of which the $W(V, B, \delta)$ 形式 a fundamental 系统 of entourages is called the uniform 结构 of convergence in measure in $A$.*.

相应的拓扑 is called the *拓扑 of convergence in measure in $A$*, and a filter (or 序列) that converges for this 拓扑 is said to be *convergent in measure in $A$*; the mention of $A$ is often suppressed when $A = X$.

假设 $F$ 是 *Hausdorff*；那么，对于每个$\mu$可积集合$B \subset A$，$W(V, B, \delta)$的交，其中$V$运行在$F$的基本系统上，$\delta$运行在集合上数$> 0$，是对$(f, g)$的集合，使得$f(x) = g(x)$*几乎在$B$*中的任何地方（*相对于$\mu$*）。对于$x \in B$的集合$M$，使得$f(x) \neq g(x)$是$\mu$可积，因为它是逆像，在$\mu$可测映射$x \mapsto (f(x), g(x))$下，是对角线的补集$F \times F$，开放（No. 5，提案 7）；如果$|\mu|(M) = \alpha > 0$，则存在紧子集$K \subset M$，使得$|\mu|(M - K) < \alpha/2$并且$f$和$g$到$K$的限制是连续的；因而，存在 $F$ 的随行人员 $V_0$，使得 $(f(x), g(x)) \notin V_0$ 代表所有 $x \in K$，因而 $(f, g) \notin W(V_0, B, \alpha/2)$。

由此可知，如果 $F$ 是 Hausdorff，则 $\mathscr{S}(A, \mu; F)$ *所有*随从的交是对 $(f, g)$ 的集合，使得 $f(x) = g(x)$ *在 $A$* 中几乎无处不在。与 $\mathscr{S}(A, \mu; F)$ 相关的豪斯多夫制服空间，我们将其表示为 $S(A, \mu; F)$ 或 $S_F(A, \mu)$（或者当 $A = X$ 时甚至为 $S_F(\mu)$ 或 $S_F$），因此由关系的 *等价类* 组成$f(x) = g(x)$ 本地几乎所有$A$ » 集合 $\mathscr{S}(A, \mu; F)$。

#### 命题 17 {#int-iv-s5-prop-17 .statement tag=08W5}

— 令 $(A_\lambda)_{\lambda \in L}$ 为 $A$ 的 $\mu$ 可测量子集的局部可数族，两两配对不相交的，并且 $A - \bigcup_{\lambda \in L} A_\lambda$ 局部 $\mu$ 可忽略不计。如果对于每个类$f \in S(A, \mu; F)$和每个$\lambda \in L$，$f_\lambda$表示类$f$中任何函数的限制到$A_\lambda$中的类，则映射 $\psi : f \mapsto (f_\lambda)_{\lambda \in L}$ 是制服空间 $S(A, \mu; F)$ 的同构到乘积制服空间 $\prod_{\lambda \in L} S(A_\lambda, \mu; F)$。

从 No. 10，第 16 条命题可知 $\psi$ 是双射的。考虑$S(A, \mu; F)$的随行人员$T$，即$W(V, B, \delta)$的典范像，其中$B$是$A$的紧凑子集；我们知道$\lambda \in L$的集合$J$使得$B \cap A_\lambda \neq \varnothing$是可数的（No. 9），并且$|\mu|(B) = \sum_{\lambda \in J} |\mu|(B \cap A_\lambda)$；因此，存在 $J$ 的有限子集 $H$ 使得

$$
\sum_{\lambda \in J - H} |\mu|(B \cap A_\lambda) \leq \frac{\delta}{2}.
$$

$\psi \times \psi$下的$T$的像则包含在乘积$\prod_{\lambda \in H} W(V, B \cap A_\lambda, \delta)$的典范像中。另一方面，如果$m$是$H$的元素数，则随行人员$\prod_{\lambda \in H} W(V, A_\lambda, \delta/2m)$的$\psi \times \psi$包含典范像下的$T$像，这就证明了命题。

#### 命题 18 {#int-iv-s5-prop-18 .statement tag=08W6}

— *If $F$ is metrizable, and $A$ is 并 of a locally $\mu$-negligible 集合 and 序列 $(A_n)$ of $\mu$-integrable 集合, then 空间 $S(A, \mu; F)$ is可计量化。*

Since each $A_n$ is 并 of a negligible 集合 and 序列 of 紧集, we can suppose that the $A_n$ are already *compact* and pairwise 不相交的.然后，第 17 条命题允许我们假设 $A$ 是紧致的。 If $(V_n)$ is a countable fundamental 系统 of entourages of $F$, it is clear that the $W(V_n, A, 1/n)$ 形式 a fundamental 系统 of entourages of $S(A, \mu; F)$ as $n$ runs over $\mathbf{N}$, 从而命题。

#### 引理 4 {#int-iv-s5-lem-4 .statement tag=08W7}

— *令$F$为可度量均匀空间，并令$B \subset A$为$\mu$可积集合的可数并。 Then, for every Cauchy 序列 $(f_n)$ in $S(A, \mu; F)$, there exists a subsequence $(f_{n_k})$ of $(f_n)$ such that $(f_{n_k}(x))$ is a Cauchy 序列 in $F$ for almost every $x \in B$.*

首先假设$B$是可积的，并用$d$表示与$F$的统一结构兼容的度量。我们将在$S(A, \mu; F)$中递归函数的定义双序列$(f_{mn})$，使得$f_{0n} = f_n$对于每个$n$，$(f_{mn})_{n \geq 0}$对于每个$m > 0$都是$(f_{m-1,n})_{n \geq 0}$的子序列，并且，最后，对于$x \in B$中的每个$m > 0$集合$M_{mn}$，其中$d(f_{mn}(x), f_{m,n+1}(x)) > 1/2^{m+n+1}$都有$|\mu|(M_{mn}) \leq 1/2^{m+n+1}$的度量；

这种定义的可能性源于$(f_n)$是$\mathscr{S}(A, \mu; F)$中的柯西序列。 集合$M_m = \bigcup_{n \geq 0} M_{mn}$；然后

$$
|\mu|(M_m) \leq \sum_{n=0}^{\infty} |\mu|(M_{mn}) \leq 1/2^m
$$

并且，对于每个 $x \in B - M_m$，对于所有 $n \geq 0$ 和所有 $p > 0$，我们都有 $d(f_{mn}(x), f_{m,n+p}(x)) \leq 1/2^{m+n}$；因此，序列$(f_{mn}(x))_{n \geq 0}$是$F$中的柯西序列。现在让 $N = \bigcap_{m=0}^{\infty} M_m$； $N$可以忽略不计。每 $n \geq 0$ 集合 $g_n = f_{nn}$；对于每个$m$，序列$(g_n)_{n \geq m}$是序列$(f_{mn})_{n \geq 0}$的子序列；如果$x \in B - N$，则存在指标 $m$使得$x \notin M_m$，证明序列$(g_n(x))$是$F$中的柯西序列。

如果现在$B$是可积集合的序列$(B_m)$的并，则可以递归地定义双序列$(g_{mn})$使得$g_{0n} = f_n$，$(g_{mn})_{n \geq 0}$是每个$m > 0$的$(g_{m-1,n})_{n \geq 0}$子序列，并且序列$(g_{mn}(x))_{n \geq 0}$是$B_m - P_m$中的柯西序列，其中$P_m$可以忽略不计。对于每个$n \geq 0$，集合$h_n = g_{nn}$，因此，对于每个$m$，序列$(h_n)_{n \geq m}$是$(g_{mn})_{n \geq 0}$的子序列；对于每个 $x \in B - P$，序列 $(h_n(x))_{n \geq 0}$ 是$F$ 中的柯西序列，其中 $P = \bigcup_{m=0}^{\infty} P_m$ 可以忽略不计。

#### 命题 19 {#int-iv-s5-prop-19 .statement tag=08W8}

*如果制服空间$F$可度量且完整，则制服空间$S(A, \mu; F)$完整。*

存在$A$的紧凑子集的局部可数族$(K_{\lambda})_{\lambda \in L}$，使得$K_{\lambda}$成对不相交的且$A - \bigcup_{\lambda} K_{\lambda}$局部可忽略不计（No. 9，命题14）。根据第 17 条命题，$S(A, \mu; F)$ 同构于乘积 $\prod_{\lambda \in L} S(K_{\lambda}, \mu; F)$；因此，当 $A$ *可积*时，我们就减少到证明命题；然后$S(A, \mu; F)$是可度量的（命题18），并且通过引理 4，对于$\mathscr{S}(A, \mu; F)$中的每个柯西序列$(f_n)$，都存在一个收敛于$A - N$的子序列$(f_{n_k})$，其中$N$可以忽略不计； $(f_{n_k})$的极限$f$（以任何方式扩展到所有$A$）则$\mu$是可测量的，并且从No. 10中提到的叶戈罗夫的定理的扩张得出序列 $(f_{n_k})$ *在测量中收敛*到 $A$ 中的 $f$。这意味着$f$是$\mathscr{S}(A, \mu; F)$中序列$(f_n)$的集群点，并且由于序列$(f_n)$是假设柯西序列，因此它收敛到$f$。

Q.E.D.

#### 推论{#int-iv-s5-n11-cor-1 .statement tag=08W9}

— 令 F 为可度量的均匀值空间。

(i) $\mathscr{S}(A, \mu; F)$ 的元素的每个序列 $(f_n)$ 几乎处处局部收敛到 A 的映射 $f$（必然 $\mu$ 可测）到 F，在测度上收敛到 A 中的 $f$。

(ii) 设$(f_n)$为$\mathscr{S}(A, \mu; F)$的元素的序列，其收敛于A的映射$f$进入F。对于每个集合$B \subset A$，它是可数可积的并集合，存在$(f_n)$的子序列$(f_{n_k})$，使得对于几乎每个$x \in B$，序列$(f_{n_k}(x))$在F中收敛到$f(x)$。

(i) 断言紧随No. 10 中提到的叶戈罗夫定理的扩张。

(ii) 到引理 4，存在$(f_n)$的子序列$(f_{n_k})$，使得对于每个$x \in B - N$，$(f_{n_k}(x))$是F中的柯西序列，其中N可以忽略不计；令$f'(x) \in \widehat{F}$为$x \in B - N$的序列的极限。很明显，$f'$是$B - N$到$\widehat{F}$的$\mu$可测映射，并且序列$(f_n)$通过(i)在$B - N$中收敛到$f'$；因此，在 B 中几乎所有地方 $f'$ 都等于 $f$。

#### 命题 20 {#int-iv-s5-prop-20 .statement tag=08WA}

— 令 F 为 Banach 空间，配备由其范数定义的制服结构。

(i) 对于X的每个$\mu$可测子集A，测度收敛的拓扑与$\mathscr{S}(A, \mu; F)$的向量空间结构兼容。

(ii) 空间 $\mathscr{K}(X; F)$ 在 $\mathscr{S}(X, \mu; F)$ 中是稠密的。

(iii) 对于每一个实数$p \geq 1$，拓扑在空间$\mathscr{L}_F^p(X, \mu)$上通过拓扑的收敛测量比阶$p$的平均收敛拓扑粗糙。

(i) 对于 A 的每个$\mu$可积子集 B 和每个$\delta > 0$，用$f \in \mathscr{S}(A, \mu; F)$的$T(B, \delta)$集合表示，其中$x \in B$的集合C使得$|f(x)| \geq \delta$满足关系$|\mu|(C) \leq \delta$；显然，如果$V_\delta$是由对$(y, z)$形成的F的周边，使得$|y - z| \leq \delta$，则周边$W(V_\delta, B, \delta)$是A到F中可测量的映射的对$(f, g)$的集合，使得$f - g \in T(B, \delta)$。很明显，集合 $T(B, \delta)$ 是对称的，并且对于每个非零的标量 $\alpha$，$T(B, \delta) + T(B, \delta) \subset T(B, 2\delta)$ 和 $T(B, |\alpha|\delta) \subset \alpha T(B, \delta)$ 使得 $|\alpha| \leq 1$；因此，只需验证集合 $T(B, \delta)$ 具有吸收性（TVS，I, §1, No. 5，命题 4）。现在，如果$f$是A到F中的$\mu$可测映射，则数值函数$|f|$也是$\mu$可测（No. 3，Th.1的Cor.6）。令$C_n$为$x \in B$的集合，使得$|f(x)| \geq n$；可积集合的 $C_n$ 形式递减序列，其交为空；因此存在整数 $n$ 使得 $|\mu|(C_n) \leq \delta$ （§ 4, No. 5，第 7 号提案的 Cor.）；我们还可以假设$n$取足够大即$1/n \leq \delta$；然后$f/n^2 \in T(B, \delta)$，完成断言 (i) 的证明。

(iii) 关系 $\int |f|^p d|\mu| \leq \delta^{p+1}$ 意味着如果 $C$ 是 $x \in X$ 的集合，使得 $|f(x)| \geq \delta$，则

$$
\delta^p |\mu|^*(C) \leq \int |f|^p d|\mu| \leq \delta^{p+1},
$$

从而$|\mu|^*(C) \leq \delta$，证明(iii)。

(ii) 鉴于 (​​iii)，足以证明对于例，$\mathscr{L}_F^1$ 在 $\mathscr{S}_F$ 中是稠密的，因为到定义 $\mathscr{H}(X; F)$ 在 $\mathscr{L}_F^1$ 中是稠密的，对于均值收敛的拓扑而言。现在，令$f$为$\mathscr{S}_F$的任意元素，并令$T(B, \delta)$为空间中0的邻域；我们在（i）中看到，存在$B$的可积子集$C$，使得$|\mu|(C) \leq \delta$并且$f$在$B - C$上*有界*；然后用$g$函数表示等于$B - C$上的$f$并在$X - (B - C)$上等于0，它从No. 6，Th得出。 5 $g$可积，显然$f - g \in T(B, \delta)$。

#### 注 {#int-iv-s5-n11-rem-1 .statement tag=08WB}

— 1) 拓扑向量空间$\mathscr{S}(X, \mu; F)$不一定是局部凸的（Exer.24）。
2) 在$f$的集合上诱导拓扑，使得$N_p(f) \leq 1$通过拓扑的测量收敛可能严格比在集合通过拓扑的平均收敛阶$p$诱导的拓扑更粗糙（练习22）。不过，请参阅下面的第 21 条提案。

#### 定义 10 {#int-iv-s5-def-10 .statement tag=08WC}

*令$X$为局部紧致空间，$\mu$为$X$的测度，$F$为Banach空间和$p \in [1, +\infty[$。 $\mathscr{L}_F^p(X, \mu)$ 的子集 $H$ 被认为是阶 $p$（对于$\mu$）等可积，如果它满足以下条件：*

(i) *对于每个$\varepsilon > 0$，都存在一个$\delta > 0$，这样，对于每个$|\mu|(A) \leq \delta$的可积集合$A$和每个$f \in H$，*

$$
\int |f|^p \varphi_A d|\mu| \leq \varepsilon.
$$

(ii) *对于每个$\varepsilon > 0$，存在一个$X$的紧凑子集$K$，这样，对于每个$f \in H$，*$\int |f|^p \varphi_{X-K} d|\mu| \leq \varepsilon$。

当 $p = 1$ 时，我们说“可等积”而不是“阶 1 可等积”。

#### 注 {#int-iv-s5-n11-rem-2 .statement tag=08WD}

— 假设 $\mu$ 有界。对于每个$a > 0$，$X$的可测量映射到$F$的集合，使得$|f(x)| \leq a$几乎处处都是阶$p$等可积，对于任何$p \in [1, +\infty[$都是如此。

#### 命题 21 {#int-iv-s5-prop-21 .statement tag=08WE}

*设 $H$ 为 $\mathscr{L}_F^p(X, \mu)$ 的子集，它是阶 $p$ 等可积的。在$H$上，测度收敛的均匀结构等于$\mathscr{L}_F^p(X, \mu)$的均匀收敛结构。*

让$\varepsilon > 0$。存在具有 Def 的性质 (i) 和 (ii) 的$\delta$ 和 $K$。 10. 令$H$中的$f, g$为：

$$
|f(x) - g(x)| \leq \left( \frac{\varepsilon}{|\mu|(K)} \right)^{1/p}
$$

对于$x \in K$，措施$\leq \delta$的集合$M$除外。然后

$$
\left( \int_{X-K} |f-g|^p d|\mu| \right)^{1/p} \leq \left( \int_{X-K} |f|^p d|\mu| \right)^{1/p} + \left( \int_{X-K} |g|^p d|\mu| \right)^{1/p}
$$
$$
\leq 2\varepsilon^{1/p}
$$

和类似地
$$
\left( \int_M |f-g|^p d|\mu| \right)^{1/p} \leq 2\varepsilon^{1/p},
$$
因此
$$
\int |f-g|^p d|\mu| = \int_{X-K} |f-g|^p d|\mu| + \int_M |f-g|^p d|\mu| + \int_{K-M} |f-g|^p d|\mu|
$$
$$
\leq 2^p \varepsilon + 2^p \varepsilon + \frac{\varepsilon}{|\mu|(K)} |\mu|(K-M) \leq (2^{p+1} + 1)\varepsilon.
$$

因此，$H$上测量收敛的均匀结构是更细，而不是$\mathscr{L}_F^p(X, \mu)$引起的均匀结构。那么应用提案 20 就足够了。

### 12. 性质模糊收敛

#### 引理 5 {#int-iv-s5-lem-5 .statement tag=08WF}

*令$X$为局部紧致空间，$\mu$为$X$上的有界正测度，$F$为Banach空间，以及$f$为$X$上的有界函数，其中值为$F$。以下条件是等效的：*

(i) *$f$的不连续性点的集合是$\mu$-可忽略不计。*

(ii) *对于每个$\varepsilon > 0$，存在$F$、函数$g_1, \ldots, g_n$属于到$\mathscr{K}(X)$的元素$a_1, \ldots, a_n$，以及$X$上的有界连续函数$h \geq 0$，使得$|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|$ $X$ 和 $\int h d\mu \leq \varepsilon$。*

用$f$的不连续性点的$N$集合表示，并令$M = \sup |f|$。

(i) $\Rightarrow$ (ii)。假设满足条件(i)。让$\varepsilon > 0$。 函数 $f$ 是 $\mu$ 可积（No. 2，第 5 条命题第 4 条，以及 No. 6，第 5 条），因此在 $F$ 中存在$a_1, \ldots, a_n$，在$\mathscr{K}(X)$ 中存在$g_1, \ldots, g_n$，这样， 设定$k = |f - g_1 a_1 - \cdots - g_n a_n|$，我们有$\int k d\mu \leq \varepsilon/2$（§ 3, No. 5，

提案 10）。将$g_1, \ldots, g_n$乘以$\mathscr{K}(X)$的适当相同的元素，我们可以在加法中假设

$$
|g_1 a_1 + \cdots + g_n a_n| \leq M = \sup |f|
$$

X、从而$k \leq 2M$。 $k$的间断点点的集合$N'$包含在$N$中，因此可以忽略不计。对于每个 $x \in X$、集合 $l(x) = \limsup_{y \to x} k(y)$。

然后X上的$2M \geq l \geq k$，以及$X - N'$上的$l = k$，也就是说，几乎到处都是$\mu$，因此$\int l \, d\mu \leq \varepsilon / 2$。另一方面，$l$是有界且上半连续的，因此是有界连续函数$\geq l$的集合的下包络线。因此，在X上存在有界连续函数$h \geq l$，使得$h \leq 2M$和$\int h \, d\mu \leq \int l \, d\mu + \varepsilon / 2$（§ 4, No. 4，第5条命题的Cor.2）。然后是$\int h \, d\mu \leq \varepsilon$和$|f - g_1 a_1 - \cdots - g_n a_n| \leq h$。

(ii) $\Rightarrow$ (i)。假设满足条件(ii)。对于每个 $x \in X$ 令 $\omega(x)$ 为 f 在 x (GT, IX, § 2, No. 3) 处的振荡。让$\varepsilon > 0$。存在具有(ii)性质的$a_1, \ldots, a_n, g_1, \ldots, g_n, h$。对于每个$x \in X$，$\omega(x)$是$f - g_1 a_1 - \cdots - g_n a_n$在x处的振荡，因而$\omega(x) \leq 2h(x)$。因而$\int \omega \, d\mu \leq 2\varepsilon$。因而，$x \in X$的集合$A_\varepsilon$使得$\omega(x) \geq \sqrt{\varepsilon}$满足$\mu(A_\varepsilon) \leq 2\sqrt{\varepsilon}$。这就证明了$\mu(N) \leq 2\sqrt{\varepsilon}$，从而$\mu(N) = 0$。

#### 命题 22 {#int-iv-s5-prop-22 .statement tag=08WG}

— *令 F 为 Banach 空间、X $\mathscr{E}$ 的X、$\mu$ 元素上的局部紧致空间、$\mathscr{E}$ 集合和$\mathscr{B}$ 滤波器基 $\mathscr{E}$。假设$\mathscr{B}$模糊地收敛于$\mu$，并且$\| \nu \|$相对于$\mathscr{B}$趋于$\| \mu \|$。令 f 为 X 的映射代入 F 满足以下条件：

(i) f 是有界的，并且对于 $\mu$ 以及属于到 $\mathscr{B}$ 的某个元素的每个测度可积；
(ii) f 的不连续性的点的集合是$\mu$-可忽略不计。
那么$\int f \, d\nu$相对于$\mathscr{B}$趋向于$\int f \, d\mu$。

让$\varepsilon > 0$。 F 中存在元素 $a_1, \ldots, a_n$，$\mathscr{K}(X)$ 中存在函数 $g_1, \ldots, g_n$，X 上存在有界连续函数 $h \geq 0$，使得

$$
|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|
$$

X 和 $\int h \, d\mu \leq \varepsilon$ (引理 5)。让$M = \sup |f|$。存在 X 的紧致子集 K，使得 $\mu^*(X - K) \leq \varepsilon$（§ 4, No. 7，第 12 条命题和 No. 6，第 4 条），在 X 中存在 K 的紧致邻域 $K'$，以及连续的映射 $h'$ X 转换为 $[0, 2M]$，使得 $h' = h$ 在 K 上，$h' = 2M$ 在 $X - K'$ 上； 替换$h'$乘以$\sup(h, h')$，我们可以在加法中假设$h' \geq h$。然后$\int (h' - h) \, d\mu \leq 2M \mu^*(X - K) \leq 2M \varepsilon$。另一方面，$h' = h_1 + 2M$，其中$h_1 \in \mathscr{K}(X)$。考虑到§ 4, No. 7、第 12 号提案、数

$$
\int h' \, d\nu = \int h_1 \, d\nu + 2M \|\nu\| \text{ tends to } \int h_1 \, d\mu + 2M \|\mu\| = \int h' \, d\mu \text{ with respect to } \mathscr{B}. \text{ There then exists an } A \in \mathscr{B} \text{ such that, for every } \nu \in A,
$$
$$
\left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| \leq \varepsilon,
$$
$$
\int h \, d\nu \leq \int h' \, d\nu \leq \int h' \, d\mu + \varepsilon \leq \int h \, d\mu + 2M \varepsilon + \varepsilon \leq 2(M + 1)\varepsilon.
$$
这些不平等意味着
$$
\left| \int f \, d\nu - \int f \, d\mu \right| \leq
$$
$$
\int h \, d\nu + \left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| + \int h \, d\mu
$$
$$
\leq 2(M + 2)\varepsilon,
$$
这就证明了命题。

#### 注 {#int-iv-s5-n12-rem-1 .statement tag=08WH}

如果$f$连续且有界，则满足命题 22 的条件 (i) 和 (ii)。

#### 例 {#int-iv-s5-n12-exa-1 .statement tag=08WI}

让我们将$X$视为绝对值 1 的复数的紧致空间$\mathbf{U}$。在设定$\mu(f) = \int_0^1 f(e^{2i\pi t}) \, dt$上，对于每个$f \in \mathscr{H}(\mathbf{U})$，一个定义是$\mathbf{U}$上质量1的正测量值。另一方面，令$\theta$为实数；对于每个整数 $n \geq 0$，令 $\nu_n$ 为单位质量，放置在 $\mathbf{U}$ 的点 $e^{2i\pi n \theta}$ 处，并让
$$
\mu_n = \frac{1}{n+1} (\nu_0 + \cdots + \nu_n),
$$
因此 $\mu_n$ 是 $\mathbf{U}$ 上质量 1 的正量度。那么，如果$\theta$是无理数，则$\mu_n$模糊地趋向于$\mu$。因为，由于函数 $z \mapsto z^k$ ($k \in \mathbf{Z}$) 的线性组合在 $\mathscr{H}(\mathbf{U})$ 中是稠密的（GT，X, §4, No. 4，命题 8），因此只要证明$\mu_n(z^k)$ 对于 $k \in \mathbf{Z}$ 趋向于 $\mu(z^k)$ 即可。现在，对于$k = 0$，$\mu_n(z^k) = \mu(z^k) = 1$；对于$k \neq 0$，
$$
\mu_n(z^k) = \frac{1}{n+1} (1 + e^{2i\pi k \theta} + e^{4i\pi k \theta} + \cdots + e^{2i\pi k n \theta}).
$$
由于$e^{2i\pi k \theta} \neq 1$（因为$\theta$是无理数），我们推断
$$
|\mu_n(z^k)| = \left| \frac{1}{n+1} \frac{e^{2i\pi k(n+1)\theta} - 1}{e^{2i\pi k \theta} - 1} \right| \leq \frac{1}{n+1} \frac{2}{|e^{2i\pi k \theta} - 1|},
$$

因此$\mu_n(z^k)$趋向于$0 = \mu(z^k)$。在这些条件下，可以应用命题22，并且我们特别看到，如果$A$是$U$的子集，并且相对于$\mu$的边界可以忽略不计，那么$\mu_n(A)$趋向于$\mu(A)$。在其他字中，如果$p_n$表示整数$k \in [0, n]$中的数，使得$e^{2i\pi k \theta} \in A$，则$n^{-1} p_n$趋向于$\mu(A)$，就像$n$趋于$+\infty$一样。

### 习题 {#int-iv-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
