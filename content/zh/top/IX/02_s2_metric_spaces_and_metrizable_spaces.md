---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 2
section_title: Metric spaces and metrizable spaces
lang: zh
source: top-v-x
pdf_pages: 0153-0166, 0232-0241
extraction: ocr
subsections:
    - "no": 1
      title: METRICS AND METRIC SPACES
      page: 0
      pdf_page: 153
    - "no": 2
      title: STRUCTURE OF A METRIC SPACE
      page: 0
      pdf_page: 154
    - "no": 3
      title: OSCILLATION OF A FUNCTION
      page: 0
      pdf_page: 157
    - "no": 4
      title: METRIZABLE UNIFORM SPACES
      page: 0
      pdf_page: 157
    - "no": 5
      title: METRIZABLE TOPOLOGICAL SPACES
      page: 0
      pdf_page: 158
    - "no": 6
      title: USE OF COUNTABLE SEQUENCES
      page: 0
      pdf_page: 159
    - "no": 7
      title: SEMI-CONTINUOUS FUNCTIONS ON A METRIZABLE SPACE
      page: 0
      pdf_page: 161
    - "no": 8
      title: METRIZABLE SPACES OF COUNTABLE TYPE
      page: 0
      pdf_page: 161
    - "no": 9
      title: COMPACT METRIC SPACES; COMPACT METRIZABLE SPACES
      page: 0
      pdf_page: 163
    - "no": 10
      title: QUOTIENT SPACES OF METRIZABLE SPACES
      page: 0
      pdf_page: 165
statements: 33
exercises: 25
content_sha256: 514856bbe1193f54564456d069f6e272568591b5ff649fc66552cb8596fa5e22
translated_from: content/en/top/IX/02_s2_metric_spaces_and_metrizable_spaces.md
translation_method: google
source_content_sha256: d331e64864dcc1e0126c3bba0d6705f7cf12cadc6c25e95836fc8a8baa92e612
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8eb8706659f4e41c16839fb6b319500366aeb97ca3393869ce18db509a214506
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. 公制空间和可计量空间

### 1. 指标和指标空间

#### 定义 1 {#top-ix-s2-def-1 .statement tag=0C2C}

*集合* $X$ *是一个有限伪度量* $d$ *在* $X$ *使得关系* $d(x, y) = 0$ *暗示* $x = y$。 *度量空间是集合* $X$ *赋予由给定度量定义的结构* $X$。

度量空间 $X$ 始终被视为携带均匀性，而拓扑由 $X$ 上的给定度量定义。

#### 例 1 {#top-ix-s2-n1-exa-1 .statement tag=0C2D}

欧氏距离$d(x, y)$ (章 VI, § 2, no. 1) 是实$n$维数空间 $\mathbf{R}^n$的度量； 函数也是如此

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \quad \text{and} \quad \sum_{i=1}^n |x_i - y_i|.
$$

所有这些指标都是*等效的*（$\S$1，no. 2）。

#### 例 2 {#top-ix-s2-n1-exa-2 .statement tag=0C2E}

在任何集合$X$上，伪度量$d$（由关系$d(x, x) = 0$和$d(x, y) = 1$（如果$x \neq y$）定义）是一个度量。 定义在 $X$ 上的均匀度是*离散*均匀度。

如果我们说一个度量是*有限*伪度量，使得该伪度量定义的均匀性是*Hausdorff*，那么我们就有定义等价于定义 1；因此，等效于度量的有限伪度量是度量。

当伪度量不是度量时，由*单个伪度量*（我们可以假设是*有限*）定义的统一空间可以简化为度量空间。令$f$为集合$X$的伪度量，令$\mathscr{U}$为$f$定义的均匀性； $\mathscr{U}$不是Hausdorff，$\mathscr{U}$的随从的交是由等价关系$f(x, y) = 0$定义的$X \times X$的子集。让$R$表示这个关系。如果$x \equiv x' \pmod{R}$，那么通过三角形不等式我们有

$$
f(x, y) \leq f(x, x') + f(x', y) = f(x', y)
$$

and similarly $f(x', y) \leq f(x, y)$, so that $f(x, y) = f(x', y)$; in other words, $f$ is a function *compatible* (in $x$ and $y$) with the equivalence relation $R$ (*Set Theory*, R, § 5, no. 7). 设$\overline{f}$是$f$在商集上诱导函数； $\overline{f}$定义在$(X/R) \times (X/R)$上，并且如果$x$和$y$是$X$的任意两个点，并且如果$\dot{x}$和$\dot{y}$表示$x$的等价类（模$R$）并且分别为$y$，则我们有$\overline{f}(\dot{x}, \dot{y}) = f(x, y)$。 紧接着，$\overline{f}$ 是$X/R$ 上的一个*度量*；它被称为与伪度量 $f$ *关联*的度量；此外，$X/R$上的定义均匀性正是与$\mathscr{U}$通过该均匀性的定义*关联的豪斯多夫均匀性（章II, § 3, no. 8，注）。 因此，通过经过到合适的商空间，由单个伪度量定义的统一结构可以减少到度量空间的结构。

指标空间的*完成*的命题 1 of § 1, no. 3 确定结构：

#### 命题 1 {#top-ix-s2-prop-1 .statement tag=0C2F}

*令$X$为空间的度量，并令$d$为其度量。如果$\hat{X}$是$X$的完备性（相对于$d$定义的均匀性），函数$d$可以通过连续性扩展到$\hat{X} \times \hat{X}$；扩展的函数$\overline{d}$是$\hat{X}$的度量，$\hat{X}$重合与度量$\overline{d}$定义的一致性。*

§ 1, no. 3的命题 1表明$\overline{d}$是$\hat{X}$上的有限伪度量，$\overline{d}$在$\hat{X}$上定义的均匀性是完成得到的均匀性；由于后一个均匀性是 Hausdorff，因此 $\overline{d}$ 是一个*度量*。每当我们将度量空间$X$视为度量空间时，总是可以理解，$\hat{X}$上的度量是通过连续性扩展$X$上的度量而获得的。

### 2. 结构指标空间

令$X$和$X'$为两个度量空间，$d$为$X$的度量，$d'$为$X'$的度量。根据一般的定义（*集合理论*，R，§ 8, no. 5），$X$到$X'$的一对一映射$f$是度量空间结构的*同构* $X$ 到 $X'$ 如果

$$(1)$$
$$
d(x, y) = d'(f(x), f(y))
$$

对于所有$x \in X$和所有$y \in X$。

注，如果$f$是$X$的映射到满足恒等式(1)的$X'$，则$f$必须是*双射的*，因此$X$的同构到$X'$；这样的同构也称为$X$到$X'$的*等距*（或*等距*映射）。

X到X'的等距当然是X的均匀性（分别为拓扑）到X'的均匀性（分别为拓扑）的同构；这些叙述中的逆命题是假的，正如不同等效度量 (§ 1, no. 2) 的存在所表明的那样。

令X为空间的度量，d为X的度量。对于每个 a > 0，让 V_a 表示所有对 (x, y) 的 X × X 由……组成的子集，使得 d(x, y) < a，并让 W_a 表示 X × X 的子集所有对 (x, y) 中的由……组成使得 d(x, y) ≤ a。作为贯穿所有实数 > 0 的集合（或仅仅数 > 0 趋向于 0 的序列），集合 V_a（或 W_a）形式开放（或封闭）随从的均匀性的基本系统 X，因为d(§ 1, no. 3)连续。我们有$\overline{V}_a \subset W_a$，但这两个集合不一定相同。

与 $\mathbf{R}^n$、集合 $V_a(x)$ 上欧氏距离的情况类比 [分别。 $W_a(x)$] 称为开（或闭）球，其中心 x 和半径 a；它是 X 中的开（或闭）集合。同样，所有 $y \in X$ 中的集合使得 $d(x, y) = a$ 被称为具有中心 x 和半径 a 的球体；这是一个封闭的集合。根据上述内容，具有中心 x 和半径形式的开（或闭）球，以 x 的邻域的基本系统作为 a，穿过所有实数 > 0 的集合，或数 > 0 的序列，这趋向于0。

读者应注意不要假设任意度量空间中的球和球体与章 VI, § 2 中研究的欧氏球和球体具有相同的属性。因此，开球的闭合不一定是具有相同中心和半径的闭球；闭球的边界不必是具有相同中心和半径的球体；不需要连接开（或闭）球；球体可以是空的 (cf. 习题 4)。

令 A 和 B 为度量空间 X 的任意两个非空子集。 数
$$
d(A, B) = \inf_{x \in A, y \in B} d(x, y)
$$
称为集合 A 和 B 之间的距离。特别地，我们用 $d(x, A)$ 表示集合 $\{x\}$ 和集合 A 之间的距离；这称为从点 x 到集合 A 的距离。因此
$$
d(x, A) = \inf_{y \in A} d(x, y)
$$
从而
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
（章IV, § 5, no. 4，命题9）。

#### 注 {#top-ix-s2-n2-rem-1 .statement tag=0C2G}

如果$d(x, A) = a$，则可能不存在到x的距离等于a的A的点。然而，如果 A 是紧的，这种情况就永远不会出现，因为此时 Weierstrass 的定理 (章 IV, § 6, no. 1, 定理 1) 显示存在$y \in A$使得$d(x, A) = d(x, y)$。

#### 命题 2 {#top-ix-s2-prop-2 .statement tag=0C2H}

*叙述* $d(x, A) = 0$ *和* $x \in \overline{A}$ *等价*。

因为$d(x, A) = 0$表达了球$V_a(x)$满足$A$无论$a > 0$的值的事实；这相当于$x \in \overline{A}$。

#### 命题 3 {#top-ix-s2-prop-3 .statement tag=0C2I}

*函数* $d(x, A)$ *在* $X$ 上均匀连续。

令$x$和$y$为$X$中的任意两个点；那么给定任何$\varepsilon > 0$，都存在$z \in A$使得$d(y, z) \leq d(y, A) + \varepsilon$，因此
$$
d(x, z) \leq d(x, y) + d(y, z) \leq d(x, y) + d(y, A) + \varepsilon
$$
由三角形不等式。

*更不必说* $d(x, A) \leq d(x, y) + d(y, A) + \varepsilon$，由于$\varepsilon$是任意的，因此$d(x, A) \leq d(x, y) + d(y, A)$。同样我们有
$$
d(y, A) \leq d(x, y) + d(x, A),
$$
这样
$$
|d(x, A) - d(y, A)| \leq d(x, y),
$$
从而结果如下。

#### 注 {#top-ix-s2-n2-rem-2 .statement tag=0C2J}

我们可以用 $X$ 的两个子集 $A, B$ 得到 $d(A, B) = 0$，从而得到 $\overline{A} \cap \overline{B} = \varnothing$，前提是子集都不由单个点组成。 例、实直线$\mathbf{R}$、整数$> 0$集合和序列$(n + 1/2^n)_{n \geq 1}$点集合两个不相交的关闭集合，其距离部分为零。

然而，如果 $A$ 是*紧凑*并且 $B$ 是*封闭*，关系 $d(A, B) = 0$ 意味着 $A \cap B \neq \varnothing$，因为凭借关系
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
从命题 3 和 Weierstrass 的定理可以得出，存在 $x_0 \in A$ 使得 $d(x_0, B) = d(A, B) = 0$ ，因此存在 (命题 2) $x_0 \in B$。

$X$ 的非空子集 $A$ 的*直径*是数（有限或等于 $+\infty$）
$$
\delta(A) = \sup_{x \in A, y \in A} d(x, y).
$$

“W_a-small 集合”（章 II, § 3, no. 1）的概念与直径$\leq a$的集合相同。当且仅当 $\delta(A) = 0$ 时，非空集合 $A$ 由单个点组成。

如果 $X$ 的子集 $A$ 是“有界”（相对于公制 $d$），则其直径是*有限*；同样，如果对于每个点 $x_0 \in X$，$A$ 都包含在具有中心 $x_0$ 的球中。有界集合中的每个子集都是有界的，有界集合的有限族中的并是有界集合。

注 $X$ 的子集可以相对于度量 $d$ 有界，但相对于等价于 $d$ (cf. § 1, no. 2) 的度量无界。

### 3. 函数的振荡

与直径概念相关的是函数$f$的振动，定义在任意集合$X$上，并以公制空间$X'$取其值；如果$A$是$X$的任意非空子集，则直径$\delta(f(A))$称为$f$在$A$的振荡。

此外，如果$X$是拓扑空间$Y$的子集，并且如果$x \in \overline{X}$，数
$$
\omega(x; f) = \inf \delta(f(V \cap X))
$$
（因为$V$在$Y$中经过$x$的邻域滤波器）称为$f$在$x \in \overline{X}$的振荡。

#### 命题 4 {#top-ix-s2-prop-4 .statement tag=0C2K}

*任意函数$f$的振荡$\omega(x; f)$，定义在拓扑空间$Y$的子集$X$上，并以度量空间$X'$取其值，是上半连续的$\overline{X}$.*

令$a$为$\overline{X}$中的任意点；那么对于每个$k > \omega(a; f)$，都存在$a$的开邻域$V$，使得$\delta(f(V \cap X)) \leq k$；对于每个 $x \in V \cap \overline{X}$，$V$ 是 $x$ 的邻域，因此
$$
\omega(x; f) \leq \delta(f(V \cap X)) \leq k,
$$
这表明$\omega$在点$a$处是上半连续的。

In order that $\omega(x; f) = 0$ at a point $x \in \overline{X}$ it is necessary and sufficient that for each $\varepsilon > 0$ there should exist a neighbourhood $V$ of $x$ such that $f(V \cap X)$ is contained in a ball of radius $\varepsilon$; if $x \in X$, this condition expresses the fact that $f$ is continuous at the point $x$ (with respect to $X$); if $x \in \overline{X} \cap \mathbf{C}X$, the image under $f$ of the trace on $X$ of the neighbourhood filter of $x$ in $Y$ is a Cauchy filter base on $X'$; in particular:

#### 命题 5 {#top-ix-s2-prop-5 .statement tag=0C2L}

*令$f$为函数，定义在拓扑空间$Y$的子集$X$上，将其值作为完整度量空间$X'$。那么$f$在点$x \in \overline{X}$相对于$X$有极限当且仅当$f$在$x$的振荡是零。*

### 4. 可计量制服空间

#### 定义 2 {#top-ix-s2-def-2 .statement tag=0C2M}

*如果度量重合和 $U$ 定义的均匀性，则集合 $X$ 上的度量据说与 $X$ 上的均匀性 $U$ 相容的。
如果 $X$ 上存在与该均匀性兼容的度量，则称集合 $X$ 上的均匀性是可度量的。如果均匀性空间的均匀性是可度量的，则称其是可度量的。*

不同的度量可以兼容相同的一致性；那么它们是“等价的”（§ 1, no. 2，定义2）。

#### 定理 1 {#top-ix-s2-thm-1 .statement tag=0C2N}

*均匀性是可度量的当且仅当它是豪斯多夫并且均匀性的随从过滤器具有可数的基。*

条件是*必要的*，对于一个度量空间的均匀性的随从过滤器的随从$V_{1/n} (n \geq 1)$形式基（与no. 2的记号）。

条件是*足够的*，因为，如果满足，则所考虑的均匀性由单个伪度量定义，即 § 1, no. 4 的命题 2；由于均匀性是 Hausdorff，因此该伪度量是度量。

#### 推论 1 {#top-ix-s2-thm-1-cor-1 .statement tag=0C2O}

*由可数伪测量族定义的豪斯多夫均匀性是可度量的。*

因为如果$(f_n)$是定义此类结构的伪计量学的序列，则随从过滤器由集合$\overline{f}_n^1([0, 1/m])$的可数族生成，其中$m$和$n$各自穿过整数$> 0$的集合。

#### 推论 2 {#top-ix-s2-thm-1-cor-2 .statement tag=0C2P}

*可计量制服空间的每个可数乘积都是可计量的。*

对于这样的空间是豪斯多夫（Hausdorff），其均匀性具有可数的基本随从系统（章II, § 2, no. 6）。

### 5. 可度量拓扑空间

#### 定义 3 {#top-ix-s2-def-3 .statement tag=0C2Q}

*如果拓扑由该度量重合和 $\mathscr{T}$ 定义，则集合 $X$ 上的度量据说与 $X$ 上的拓扑 $\mathscr{T}$ 相容的。如果 $X$ 上存在与 $X$ 的拓扑兼容的度量，则称拓扑空间是可度量的。*

集合 $X$ 上的两个指标都与相同的拓扑 $\mathscr{T}$ 相容的，可能是*不等价*。

$\mathbf{R}$的子空间$\mathbf{R}_+^*$提供了其中的例。 $\mathbf{R}$的加性均匀性引起的均匀性和$\mathbf{R}_+^*$的乘性均匀性引起的均匀性都是可度量的，并且与$\mathbf{R}_+^*$的拓扑兼容；但它们没有可比性。

我们注还可以存在与*可度量*拓扑空间（习题7）的拓扑兼容的*不可度量*一致性。

我们将满足于拓扑空间的可度量性的*必要*条件（对于必要且充分的条件，cf.§ 4，习题22）。首先，空间不能是可度量的除非它是完全规则的（事实上，我们将在§ 4, no. 1，命题2中看到，可度量的空间必然是“正常的”，这是一个更强的条件）。另一方面，定理1表明：

#### 命题 6 {#top-ix-s2-prop-6 .statement tag=0C2R}

可度量空间的每个点都有一个可数基数系统邻域。

更一般地说：

#### 命题 7 {#top-ix-s2-prop-7 .statement tag=0C2S}

在可度量空间中，每个闭集合都是可数开集合族的交，每个开集合都是可数闭集合族的并。

令 $d$ 为与可度量空间 $X$ 的拓扑兼容的度量。如果$A$是$X$的闭子集，则它是开集合$V_{1/n}(A)$的交[所有$x \in X$的集合使得$d(x, A) < 1/n$； cf.命题2]。 命题的第二个部分接下来是取补码。

#### 注 1 {#top-ix-s2-n5-rem-1 .statement tag=0C2T}

这些必要的条件是不够的（cf.习题13）。

#### 注 2 {#top-ix-s2-n5-rem-2 .statement tag=0C2U}

存在空间，其中每个点都有邻域的可数基本系统，但其中存在闭集合，其不可数开集合的交（习题15）；这样的空间是不可度量的。

Corollary 2 of Theorem 1, no. 4, shows that a countable product of metrizable topological spaces is metrizable. 另外，可度量化空间的任意族 $(X_i)_{i \in I}$ 的和 $X$ (章 I, § 2, no. 4) 也是可度量化的。 For if $d_i$ is a metric compatible with the topology of $X_i$ for each $i \in I$, we may assume that $d_i$ is bounded and that the diameter of $X_i$ is $\leq 1$; we can then define a distance $d$ compatible with the topology of $X$ by putting $d(x, y) = d_i(x, y)$ if $x$ and $y$ both belong to the same $X_i$, and $d(x, y) = 1$ otherwise.

### 6. 使用可数序列

命题 6 是可度量空间理论中点的可数序列扮演的部分的起源；对于许多问题，它们可以用来代替过滤器。这是因为可度量空间的点的邻域滤波器（因此也是收敛滤波器）由空间的点的收敛序列确定：因为点的邻域滤波器具有可数的基，因此基本滤波器更细的交比其自身（章I, § 6, no. 8，命题11），即与序列相关的基本滤波器的序列收敛到所讨论的点。

另一方面，收敛序列的概念不适合拓扑空间的研究，其中存在点，其邻域滤波器没有可数基。特别地，Hausdorff非离散拓扑空间可以被构造，其中，在每点$x$，$x$的邻域的任何可数族的交又是$x$(*)的邻域；在这样的空间中，唯一收敛的序列是那些从某个指标开始所有项都相等的序列。

作为使用可数序列的例，我们给出以下命题：

#### 命题 8 {#top-ix-s2-prop-8 .statement tag=0C2V}

*在可度量的空间* $X$ 中，*点* $x$ *位于非空子集* $A$ *of* $X$ *当且仅当存在序列 of 点 of* $A$ *其中收敛于*$x$。

我们已经从章 I, § 7, no. 3 知道条件 *足够*。要看出它是*必要的*，请考虑$x$的邻域的可数基本系统$(V_n)$，使得每个$n$都有$V_{n+1} \subset V_n$。如果$x$位于$A$的闭包中，则每个$V_n$满足$A$，并且如果$x_n$位于$V_n \cap A$，则序列$(x_n)$收敛到$x$(**)。

从命题 8 我们推导出：

#### 命题 9 {#top-ix-s2-prop-9 .statement tag=0C2W}

*度量空间* $X$ *当且仅当* $X$ 中的每个柯西序列 *收敛*时才是完备的。

令 $\hat{X}$ 为 $X$ 的补全。如果存在点$x \in \hat{X}$不属于到$X$，那么$X$的点有序列$(x_n)$收敛到$x$，这是一个非收敛柯西$X$ 中序列。

#### 命题 10 {#top-ix-s2-prop-10 .statement tag=0C2X}

*让* $X$ *成为可度量的空间，并让* $f$ *成为* $X$ *的映射 *成为拓扑空间* $X'$。 *那么* $f$ *在点* $x \in X$ *当且仅当* $(x_n)$ *是* $X$ *的点的序列，收敛到* $x$，*序列* $(f(x_n))$ *收敛到* $f(x)$ *在* $X'$。

条件是必要的，从章I, § 7, no. 4，命题9，推论1。为了证明它是充分的，考虑$X'$中$f(a)$的邻域的过滤器$\mathscr{B}'$； 假设意味着$\overline{f}^{-1}(\mathscr{B}')$比每个与序列相关的收敛到$a$的基本滤波器更粗糙，也就是说每个收敛到$a$的基本滤波器；但是

(*) 参见 J. Dieudonné, 注 de Tératopologie (I), Revue scientifique (Revue Rose), 1939, p. 39。
(**) 这个命题在某些空间中仍然有效，其中至少有一个点不具有邻域的任何可数基本系统；对于例，空间是通过在无穷大处邻接点来压缩不可数离散空间而获得的（章I, § 9, no. 8，定理4）。

这些过滤器中的交是$a$的邻域过滤器（章I, § 6, no. 8，命题11）。于是就有了这样的结果。

注命题 8 和 10 在任何空间 $X$ 中有效，其中每个点都有邻域的可数基数系统。

### 7. 可测量空间上的半连续函数

#### 命题 11 {#top-ix-s2-prop-11 .statement tag=0C2Y}

*令$X$为可度量的空间，并令$f$为$X$上的下半连续函数，其值位于$\overline{\mathbf{R}}$的闭区间$[a, b]$中。那么$f$是$X$上连续函数的递增序列的上包络线，在$[a, b]$中取值。*

通过转移结构，我们可以假设$a = 0$和$b = 1$。

(i) 首先假设$f = \varphi_A$，其中$A$是$X$的开子集。那么$g_n(x) = n \inf (d(x, X - A), 1/n)$定义的函数$g_n$是连续的，$\geq 0$在$X$上；还有 $g_n(x) = f(x)$ 当 $x \in X - A$ 以及当
$$
d(x, X - A) \geq 1/n.
$$
紧随其后的是$f = \sup_n (g_n)$。

(ii) 在一般情况下，考虑对于每个整数$n \geq 1$，开集合的有限递减序列
$$
A_k = f^{-1}\left( \left[ \frac{k}{n}, +\infty \right[ \right) \quad (0 \leq k \leq n - 1);
$$
函数 $g_n = \frac{1}{n} \sum_{k=1}^{n-1} \varphi_{A_k}$ 是下半连续，对于所有$n$，我们都有$0 \leq f(x) - g_n(x) \leq 1/n$；因此$f$是序列$(g_n)$的上包络线。另一方面，$g_n$是线性组合，具有开集合的特征函数的有限数的正系数，因此是连续函数$\geq 0$的可数序列$(h_{mn})_{m \geq 0}$的上包络线，通过(i)；因此$f = \sup_{m,n} h_{mn}$。如果我们把
$$
f_n = \sup_{p \leq n, q \leq n} h_{pq},
$$
我们看到序列$(f_n)$是连续函数$\geq 0$的递增序列，以$f$为上包络线，并且从$g_n \leq n - 1/n$开始不取值1。

### 8. 可计量空间可数型

#### 定义 4 {#top-ix-s2-def-4 .statement tag=0C2Z}

*如果拓扑具有可数基，则可度量的空间被称为可数型 （或可分离）。*

显然，可数型的可度量空间的每个子空间又是可数型。 乘积空间拓扑基定义(章I, § 4, no. 1)和no. 4的推论2到定理1表明可数可计量空间可数族乘积型是可数型的可度量空间。 同样，可数型的可度量空间的可数族中的和是可数型 (no. 5) 的可度量空间。

#### 命题 12 {#top-ix-s2-prop-12 .statement tag=0C30}

*如果X是可度量拓扑空间，则以下叙述等价*：

a) *X 是可数的型*。
b) *X 具有可数稠密子集*。
c) *X同胚于立方体$\mathbf{I}^{\mathbf{N}}$的子空间，其中$\mathbf{I}$是$\mathbf{R}$中的区间$[0, 1]$。

从前面的注可以清楚看出，c) 蕴含着 a)； a) 蕴含 b)，因为如果 $(U_n)$ 是 X 的拓扑的可数基，并且 $a_n$ 是 $U_n$ 的点，则 $a_n$ 形式的稠密子集 X。最后让我们证明 b) 蕴涵 c)。令$(a_n)$为X的点的稠密序列，对于每个$x \in X$，令$\varphi(x)$为$\mathbf{I}^{\mathbf{N}}$的点$(d(x, a_n))_{n \in \mathbf{N}}$（$d$是与拓扑兼容的度量） X，相对于X的直径为$\leq 1$）。我们将证明$\varphi$是X到$\mathbf{I}^{\mathbf{N}}$的子空间的同胚。事实上，$\varphi$是连续的，因为函数$x \to d(x, a_n)$都是连续的；并且$\varphi$是单射的，因为X的每个点都是$(a_n)$（命题8）的某个子序列的极限。设 B 为一个球，其尺寸为中心 $x_0$，半径为 $r$，位于 X 内，并令 $n$ 为整数，使得

$$
d(x_0, a_n) < \frac{1}{3} r.
$$

像在集合 W 的 $\varphi$ 下，点 $x \in X$ 使得

$$
|d(x_0, a_n) - d(x, a_n)| < \frac{1}{3} r
$$

是由$\varphi(X)$中$\varphi(x_0)$的定义邻域。但是对于每个$x \in W$，我们有$d(x, a_n) < d(x_0, a_n) + \frac{1}{3} r < \frac{2}{3} r$，从而

$$
d(x, x_0) \leq d(x_0, a_n) + d(x, a_n) < r,
$$

这表明W是B中包含的$x_0$的邻域，因此$\varphi$是X到$\varphi(X)$的同胚。

注对于任意拓扑空间 X，性质 b) 并不一定意味着存在可数基，即使X是紧的并且X的每个点都有一个可数系统邻域 （习题13；cf.章I, § 1，习题7）。

#### 命题 13 {#top-ix-s2-prop-13 .statement tag=0C31}

*设X为拓扑空间，其中有可数基$(U_n)$；那么对于X的每个开覆盖$(V_i)_{i \in I}$，都存在I的可数子集 J，使得$(V_i)_{i \in J}$是X的覆盖。*

设 H 为子集 N 由……组成指标 n，使得 U_n 包含在 V_i 的至少一个中； 序列 (U_n)_{n \in H} 是 X 的覆盖，因为每个点 x \in X 属于到某个 V_i，并且由于 V_i 是开放的，因此存在指标 n 使得 x \in U_n \子集 V_i。因此，在 I 中存在映射 $\psi$，使得对于 H 中的每个 n \，U_n \子集 V_{\psi(n)}；取J = $\psi(H)$，可数，命题得证。

### 9. 紧凑公制空间；紧凑型可测量空间

均匀空间 (章 II, § 4, no. 2, 定理 3) 的预紧性准则对于度量空间产生以下命题：

#### 命题 14 {#top-ix-s2-prop-14 .statement tag=0C32}

*度量空间 X 是预紧的，当且仅当对于每个 $\varepsilon > 0$，直径为 $\leq \varepsilon$ 的集合有限覆盖 X。*

如果我们邻接假设 X 是“完整的”，我们就有了度量空间的“紧凑性”标准。

从命题 14 我们得到一个紧凑性的“拓扑”标准，适用于可度量的空间：

#### 命题 15 {#top-ix-s2-prop-15 .statement tag=0C33}

*可度量拓扑空间X是紧的当且仅当X的点的每个无限序列在X中都有一个簇点。*

章 I, § 9, no. 1 的公理 (C) 表明条件是*必要的*。为了显示*充分性*，让 d 成为与拓扑或 X 兼容的度量。我们首先证明这样定义的度量空间X是*完整的*：X中的每个柯西序列都有一个集群点，因此是收敛的（章II, § 3, no. 2，命题5，推论2）；因此X在命题 9时是完整的。接下来我们将证明X是*预紧式*；如果不是这样，那么到命题 14 时，将存在实数 $\alpha > 0$，使得 X 无法被直径为 $\leq \alpha$ 的 X 的子集的任何有限数覆盖。然后，我们可以在 n 上对所有 $p < n$ 进行定义归纳点 X 条件 $d(x_p, x_n) > \frac{1}{2} \alpha$ 的无限序列 $(x_n)$；并且这样的序列不能有簇点，因为每个半径为$< \frac{1}{2} \alpha$包含的球最多只能有序列中的一个点。

#### 推论{#top-ix-s2-n9-cor-1 .statement tag=0C34}

*可度量拓扑空间X的子集A是相对紧凑的当且仅当A的点的每个无限序列在X中都有一个簇点。*

令 d 为与拓扑或 X 兼容的度量。我们将通过应用命题 15 的判据证明空间 $\overline{A}$ 是紧致的。令$(x_n)$ 为$\overline{A}$ 的点序列；那么对于每个指标 n 都存在 $y_n \in A$ 使得 $d(x_n, y_n) < 1/n$； 序列$(y_n)$，到假设有一个簇点$a \in X$，并且a也是序列$x_i$的簇点，因为如果$y_m$位于具有中心$a$的球中并且半径 $1/n$，对于某些 $m > n$，则 $x_m$ 位于具有中心 $a$ 和半径 $2/n$ 的球内。

需要注意的是，命题 15 并不是推论，邻域的可数基本系统在$X$的每个点处存在；有例不可计量、非紧的空间，其中每个点都有一个邻域的可数基本系统，点的每个无限序列都有一个簇点（习题15）。

#### 命题 16 {#top-ix-s2-prop-16 .statement tag=0C35}

*紧凑空间 $X$ 是可度量的当且仅当其拓扑具有可数基。*

条件是*必要的*。到命题 14，对于每个整数$n \geq 1$，$X$有有限子集$A_n$，使得$A_n$到$X$的每个点的距离为$\leq 1/n$；因此，可数集合 $A = \bigcup_n A_n$ 在 $X$ 中是稠密的，结果是从 no. 8 的命题 12 得出的。

条件*足够*。设$(U_n)$是$X$的拓扑的可数基。 $X \times X$的对角线$\Delta$每点邻域因此形式$U_n \times U_n$包含邻域； 应用 Borel-Lebesgue 公理到 $X \times X$ 的紧子集 $\Delta$，因此 $\Delta$ 包含的每个邻域是形式集合的有限并 $U_n \setminus U_n$，即 $\Delta$ 的邻域。因此，$\Delta$的邻域是有限的，形式$U_n \times U_n$形式集合并是$X$均匀性的基本系统（章） II, § 4, no. 1, 定理 1)，因此结果来自no. 4的定理 1。

#### 推论{#top-ix-s2-n9-cor-2 .statement tag=0C36}

*令$X$为局部紧致空间，并令$X'$为通过在无穷大$\omega$至$X$处邻接点而获得的紧致空间（章I, § 9, no. 8）。那么下面的叙述是等价的：*

a) *$X$的拓扑有一个可数的基。*
b) $X'$ *可度量。*
c) $X$ *可度量且$\sigma$-紧凑。*

$a \Longrightarrow b$：令$U_n$为$X$的拓扑的可数基。 点 $x \in X$ 包含的每个邻域都是$x$ 的紧凑邻域，而$x$ 的包含邻域又等于一些$U_n$。因此，$U_n$、形式、基、拓扑和$X$相对紧凑，因此我们可以假设所有$U_n$都是相对紧凑的。因此，$X$是紧集$\overline{U}_n$的可数并，即它是$\sigma$紧；这意味着 $X'$ 点 $\omega$ 具有开放邻域的可数基本系统 $V_n$（章 I, § 9, no. 9，命题 15，推论 2）。因此，点$y \in X'$包含中的每个邻域要么是$U_n$之一，要么是$V_n$之一，即$y$中的邻域，因此$U_n$和$V_n$ 形式拓扑 $X'$ 的可数基。因此 $X'$ 可以通过命题 16 来度量。

b) $\Longrightarrow c)$：如果 $X'$ 可度量，则 $\omega$ 的可数基数系统为邻域，因此 $X$ 是 $\sigma$-紧致章 I, § 9, no. 9、命题 15，推论 2。

c) $\Longrightarrow a)$：到假设，有递增序列$(V_n)$相对紧凑的开放集合覆盖$X$并且使得$\overline{V}_n \subset V_{n+1}$（章I, § 9, no. 9，命题） 15）。 子空间 $\overline{V}_n$ 是紧凑且可度量的，因此具有可数基 (命题 16)，因此 $V_n$ 也是可数的。令$(U_{mn})_{m \geq 1}$为$V_n$的拓扑中的基。对于$x \in X$和$x$的每个邻域$W$，存在$n$使得$x \in V_n$，因此存在$m$使得$x \in U_{mn} \subset V_n \cap W$。因此集合$U_{mn}$($m \geq 1, n \geq 1$)形式基拓扑$X$。

### 10. 可计量空间的商空间

如果 $X$ 是可度量的空间并且 $R$ 是 $X$ 上的等价关系，则商空间 $X/R$ 不一定是可度量的（即使 $X$ 是局部紧致 \* 且 $X/R$ 是正常的） *）。然而：

#### 命题 17 {#top-ix-s2-prop-17 .statement tag=0C37}

紧致可度量空间的每个豪斯多夫商空间都是紧致且可度量的。

同样，如果 $f$ 是紧凑可度量化空间 $X$ 到 Hausdorff 空间 $X'$ 的连续映射，则 $f(X)$ 是 $X'$ (章) 的可度量化子空间 (章) I, § 9, no. 4，定理 2，推论 4)。

令$X$为紧凑可度量空间，并令$R$为$X$上的等价关系，使得$X/R$为Hausdorff。那么$X/R$是紧致的（章I, § 9, no. 4，定理2），因此到命题16就足以证明$X/R$的拓扑有一个可数的基。为此，我们使用 $R$ 是闭集（章 I, § 10, no. 4、命题 8）以及类 mod $R$ 是紧致的事实。令$\varphi$为$X$的典范映射到$X/R$，并令$(U_n)$为$X$的拓扑的可数基。令$z$为$X/R$中的任意点，并令$V$为$X/R$中$z$的邻域；那么$\overline{\varphi}^{-1}(V)$就是紧集$\overline{\varphi}^{-1}(z)$中的$X$中的邻域。如果 $x$ 是 $\overline{\varphi}^{-1}(z)$ 中的任意点，则存在集合 $U_n$ 包含于 $x$ 且包含在 $\overline{\varphi}^{-1}(V)$ 中，因此根据 Borel-Lebesgue 公理，存在有限开覆盖 $(U_{n_k})_{1 \leq k \leq r}$ $\overline{\varphi}^{-1}(z)$，如果$W$表示$\bigcup_k U_{n_k}$，则$W$是$\overline{\varphi}^{-1}(V)$中包含的$\overline{\varphi}^{-1}(z)$的邻域。由于$R$是闭集，因此$\varphi(W)$是$X/R$中$z$的邻域，包含在$V$中（章I, § 5, no. 4，命题10）。令$\mathscr{B}$表示形式$\varphi(W)$集合的内部集合，其中$W$贯穿形式集合所有有限并的集合$\mathscr{F}$ $U_n$；然后我们证明了$\mathscr{B}$是$X/R$的拓扑的基，并且由于$\mathfrak{F}$是可数的，所以$\mathscr{B}$也是可数的。

#### 命题 18 {#top-ix-s2-prop-18 .statement tag=0C38}

*令$X$为完整度量空间，令$R$为$X$上的开等价关系，使得$X/R$为Hausdorff，并令$\varphi : X \to X/R$为典范映射。那么如果$K$是$X/R$的任何紧致子集，则存在$X$的紧致子集$K'$使得$\varphi(K') = K$。*

令 $\mathscr{B}_1$ 为 $X$ 中半径为 $1/2$ 的所有开球的集合。由于$B$穿过$\mathscr{B}_1$，集合$\varphi(B)$形式是$K$的开覆盖，因此存在点$x_1, \ldots, x_m$的有限数$X$使得像在半径为 $1/2$ 和中心的开球的 $\varphi$ 下 $x_i$ ($1 \leq i \leq m$) 形式 $K$ 的开敞覆盖物。让 $H_1 = \{ x_1, \ldots, x_m \}$ 并假设我们已经为 $1 < i \leq n$ 定义了一个有限的集合 $H_i$，这样：

(i) $H_i \subset H_{i+1}$ 和 $H_{i+1}$ 中的每个点与 $H_i$ 的距离为 $< 1/2^i$，对于 $1 \leq i \leq n - 1$；

(ii) 像位于半径为$1/2^i$的开球的$\varphi$下方，其中中心位于$H_i$的点处，形式为$K$的开敞覆盖物，对于$1 \leq i \leq n$。

令$\mathscr{B}_{n+1}$为半径为$1/2^{n+1}$的所有开球的集合，其中心$x$使得$d(x, H_n) < 1/2^n$（$d$是$X$的度量）。 $H_n$的性质表明集合$\varphi(B)$，对于$B \in \mathscr{B}_{n+1}$，形式是$K$的开覆盖；因而，存在有限的集合$L_{n+1} \subset X$，使得像位于半径为$1/2^{n+1}$的开球的$\varphi$之下，其中心属于到$L_{n+1}$形式是$K$的开球覆盖物。 Taking $H_{n+1} = H_n \cup L_{n+1}$, we see that we can define inductively an infinite sequence $(H_n)$ of finite subsets of $X$ with properties (i) and (ii) above. 让$H = \bigcup_n H_n$，并让我们证明$H$是*预紧*。 对于每个$p > 0$和每个点$z_{n+p} \in H_{n+p}$，存在点$z_{n+i} \in H_{n+i}$（$0 \leq i \leq p - 1$）中的序列，使得

$$
d(z_{n+i}, z_{n+i+1}) < 1/2^{n+i} \quad \text{for } 0 \leq i \leq p - 1;
$$

由此可见，$d(z_n, z_{n+p}) \leq \sum_{i=0}^{p-1} 1/2^{n+i} \leq 1/2^{n-1}$，因此对于所有$y \in H$，$d(y, H_n) \leq 1/2^{n-1}$，这证明了我们的断言。由于$X$是完备的，$\overline{H}$是紧致的，因而$\varphi(\overline{H})$是紧致的。接下来，让我们证明$K \subset \varphi(\overline{H})$。如果$z \in K$，则对于所有$n$，乘以定义$d(\overline{H}_n, \overline{\varphi}(z)) \leq 1/2^n$，因而$d(\overline{H}, \overline{\varphi}(z)) = 0$；但$\overline{\varphi}(z)$是闭集，$\overline{H}$是紧的，因此这意味着$\overline{H} \cap \overline{\varphi}(z) \neq \emptyset$（no. 2，注紧随命题3）；因此断言。因而，如果$K' = \overline{H} \cap \overline{\varphi}(K)$，则$K'$在$\overline{H}$中闭合，因此是紧凑的，并且根据已证明的，我们有$\varphi(K') = K$。

Q.E.D.

### 习题{#top-ix-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
