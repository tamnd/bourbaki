---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 1
section_title: Generation of a uniformity by a family of pseudometrics; uniformizable spaces
lang: zh
source: top-v-x
pdf_pages: 0143-0153, 0224-0232
extraction: ocr
subsections:
    - "no": 1
      title: PSEUDOMETRICS
      page: 0
      pdf_page: 143
    - "no": 2
      title: DEFINITION OF A UNIFORMITY BY MEANS OF A FAMILY OF PSEUDOMETRICS
      page: 0
      pdf_page: 144
    - "no": 3
      title: PROPERTIES OF UNIFORMITIES DEFINED BY FAMILIES OF PSEUDOMETRICS
      page: 0
      pdf_page: 147
    - "no": 4
      title: CONSTRUCTION OF A FAMILY OF PSEUDOMETRICS DEFINING A UNIFORMITY
      page: 0
      pdf_page: 148
    - "no": 5
      title: UNIFORMIZABLE SPACES
      page: 0
      pdf_page: 150
    - "no": 6
      title: SEMI-CONTINUOUS FUNCTIONS ON A UNIFORMIZABLE SPACE
      page: 0
      pdf_page: 152
statements: 19
exercises: 22
content_sha256: 5fb14ded2eea75f474c5ddf07fd12f1e5f1a1f0f0d7928bf3f580d97de53b72a
translated_from: content/en/top/IX/01_s1_generation_of_a_uniformity_by_a_family.md
translation_method: google
source_content_sha256: d0027c85d9e629ba1cedaa3e0f5665d96575e833d7b0b7fe5a972750416a6a6d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 04187ea656534bf0a8681a915a1bc4631881bec2e803140e76454f694b1eaae5
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 伪测量学家族的均匀性的产生；统一空间

### 1. 伪计量学

定义I。 *如果X是集合，则X上的伪度量是X×X的任意映射 f进入扩展实直线$\overline{\mathbf{R}}$的区间[0, +∞]，满足以下条件：

(EC_I) *对于所有$x \in X, f(x, x) = 0$。
(EC_{II}) *对于所有$x \in X$和所有$y \in X, f(x, y) = f(y, x)$（对称）。
(EC_{III}) *对于X中的所有$x, y, z$，
$$
f(x, y) \leq f(x, z) + f(z, y)
$$
（三角形不等式）。

#### 例 1 {#top-ix-s1-n1-exa-1 .statement tag=0C17}

在实数空间 $\mathbf{R}^n$，欧氏距离 (章 VI, § 2, no. 1) 是伪测量。

#### 例 2 {#top-ix-s1-n1-exa-2 .statement tag=0C18}

如果X是任何集合，则对于所有$x \in X, f(x, y) = +\infty$，$X \times X$上的条件$f(x, x) = 0$定义函数 f，如果$x \neq y$是X上的伪度量。

#### 例 3 {#top-ix-s1-n1-exa-3 .statement tag=0C19}

如果 X 是任意集合并且 g 是在 X 上定义的任意有限实值函数，则由 $f(x, y) = |g(x) - g(y)|$ 在 $X \times X$ 上定义的函数 f 是 X 上的伪度量。

#### 例 4 {#top-ix-s1-n1-exa-4 .statement tag=0C1A}

\* 令X为$\mathbf{R}$区间[0, 1]的所有连续映射到$\mathbf{R}$的集合。如果对于元素 $x, y$ X 中的每个对，我们将
$$
f(x, y) = \int_0^1 |x(t) - y(t)| \, dt,
$$
那么 f 是 X 上的伪度量。 \*

注：
1) 上面的例2表明，对于$X$的元素的某些对，伪度量可以取值$+\infty$。
2) 如果$f$是$X$的伪度量，那么我们一般可以有$f(x, y) = 0$而没有$x = y$，如上面的例3所示（cf.§ 2）。

从三角形不等式可以得出，如果$f(x, z)$和$f(y, z)$是有限的，那么$f(x, y)$也是有限的；此外，在这种情况下我们有
$$
f(x, z) \leq f(y, z) + f(x, y) \quad \text{and} \quad f(y, z) \leq f(x, z) + f(x, y),
$$
这样
(I)
$$
|f(x, z) - f(y, z)| \leq f(x, y).
$$

如果 $f$ 是 $X$ 上的伪度量，那么对于任何有限实数 $k > 0$，$kf$ 也是伪度量。如果$\{f_i\}_{i \in I}$是$X$上的任何伪度量族，则为所有$x, y \in X \setminus X$定义了和$\sum_{i \in I} f_i$；如果$f$表示这个和的值，那么$f$是$X$上的伪度量。同样，族$\{f_i\}$ (章 IV, § 5, no. 5) 是$X$ 上的伪度量，因为关系 $f_i(x, y) \leq f_i(x, z) + f_i(z, y)$ 意味着
$$
\sup_{i \in I} f_i(x, y) \leq \sup_{i \in I} (f_i(x, z) + f_i(z, y)) \leq \sup_{i \in I} f_i(x, z) + \sup_{i \in I} f_i(z, y)
$$
[章IV, § 5, no. 7，公式（17）]。

### 2. 定义通过伪测量学家族实现一致性

我们在章VI, § 2, no. 3中看到，如果对于每个实数$s > 0$，我们用$U_s$集合来表示$\mathbf{R}^n$的点的所有对$(x, y)$，其欧氏相距$\leq s$，则$\mathbf{R}^n$均匀度的$U_s$形式基本随行系统与$s$贯穿实数$> 0$的集合。

更一般地，让$f$是集合$X$的伪度量：对于每个$s > 0$，让$U_s$表示$f^{-1}([0, s])$，并让我们证明，当$s$贯穿所有实数$> 0$的集合时， $U_s$ 形式 $X$ 均匀性的基本系统。公理$U_1$由于$\mathrm{(EC_1)}$而得到满足：如果$s = t$，我们有$U_s \subset U_t$，因而$U_s$满足$B_1$：到$\mathrm{(EC_{11})}$，我们有$U_s \cup U_s$，因此满足$U_{2s}$；最后，到$\mathrm{(EC_{111})}$时，我们得到了$U_s = U_{2s}$，这样$U_{2s}$就得到了满足。 （参见章II, § 1, no. 1、定义2）。因此我们可以做出以下定义：

#### 定义 2 {#top-ix-s1-def-2 .statement tag=0C1B}

给定集合 $X$ 上的伪度量 $f$，$f$ 定义的均匀性是 $X$ 上的均匀性，它以集合 $\overline{f}^{-1}([0, a])$ 的随行族为基础系统，其中 $a$ 贯穿所有的集合实数$> 0$。

如果定义具有相同的均匀性，则 $X$ 上的两个伪度量被认为是等效的。

#### 注 1 {#top-ix-s1-n2-rem-1 .statement tag=0C1C}

如果$(a_n)$是数$> 0$中的任意序列且趋于0，则$U_{a_n}$形式是由$f$定义的均匀性的基本系统。

#### 注 2 {#top-ix-s1-n2-rem-2 .statement tag=0C1D}

The definition of a uniformity by a pseudometric $f$ consists in taking as a fundamental system of entourages the inverse image under $f$ of the neighbourhood filter of 0 in the subspace $[0, +\infty]$ of $\overline{\mathbf{R}}$. 注这个过程与我们能够定义拓扑群 (章 III, § 3, no. 1) 上的均匀性的过程非常相似。

令$f$和$g$为$X$上的两个伪度量。从定义 2 可以看出，$f$ 定义的均匀性比$g$ 定义的均匀性更粗糙，当且仅当对于每个$a > 0$ 存在$b > 0$，使得关系 $g(x, y) \leq b$ 蕴含$f(x, y) \leq a$。 $f$和$g$等价伪计量的必要且充分的条件是，对于每个$a > 0$，都存在$b > 0$，使得$g(x, y) \leq b$暗示$f(x, y) \leq a$，并且$f(x, y) \leq b$暗示$g(x, y) \leq a$。

特别地，如果存在常数$k$使得$f \leq kg$，则$f$定义的均匀性比$g$定义的均匀性更粗糙。

令$\varphi$为区间$[0, +\infty]$自身的映射，满足以下条件：1）$\varphi(0) = 0$，$\varphi$在0处连续； 2) 0的$[0, +\infty]$中$\varphi$为递增且邻域中为严格递增的； 3）对于所有$u \geq 0$和$v \geq 0$，我们有$\varphi(u + v) \leq \varphi(u) + \varphi(v)$。那么如果 $f$ 是集合 $X$ 上的任何伪度量，则合成 $g = \varphi \circ f$ 是等价于 $f$ 的伪度量。

读者可以很容易验证，对于例，我们可以将$\varphi$取为以下函数中的任意一个：

$$
\sqrt{u}, \quad \log (1 + u), \quad \frac{u}{1 + u}, \quad \inf (u, 1).
$$

最后两个例表明总是存在与任何给定伪度量（有限或非有限）等效的有界伪度量。

#### 定义 3 {#top-ix-s1-def-3 .statement tag=0C1E}

如果$(f_i)_{i \in I}$是集合$X$上的伪度量族，则伪度量$f_i$在$X$上定义的均匀性中集合中最小的上界称为由$(f_i)$族定义的均匀性。

如果定义在 $X$ 上具有相同的均匀性，则 $X$ 上的两个伪测量族被认为是等效的。

从集合的最小上界均匀度 (章 II, § 2, no. 5) 的定义中，由一系列伪测量$(f_i)_{i \in I}$ 在 $X$ 上定义的均匀度 $U$ 的随从过滤器是*生成*的过滤器（章） I, § 6, no. 2）由集合$f_i^{-1}([0, a])$的家族设计，其中$i$穿过$I$，$a$穿过实数$> 0$的集合。在其他字中，我们通过以下步骤获得$\mathscr{U}$随行人员的基本系统：我们随机取指标$i_1, i_2, \ldots, i_n$的有限数，并对每个$i_k$、数取相应的 $a_k > 0$；然后我们考虑对$(x, y) \in X \times X$中的集合$V$，使得$f_{i_k}(x, y) \leq a_k$对应于$1 \leq k \leq n$；这些集合$V$（对于$n$、$i_k$和$a_k$所有可能的选择）形式是$\mathscr{U}$随行人员的基本系统。此外，我们可以将自己限制在所有$a_k$等于*相同*数$a > 0$的情况，因为所有对$(x, y)$的随行人员由……组成使得

$$
\sup_{1 \leq k \leq n} (f_{i_k}(x, y)) \leq \inf_{1 \leq k \leq n} a_k
$$

显然包含在$V$中。

对于$I$的每个有限子集$H$，让$g_H$表示族$(f_i)_{i \in H}$的上层信封。 As $H$ runs through the set of all finite subsets of $I$ and $a$ runs through the set of real numbers $> 0$, the sets $g_H^{-1}([0, a])$ form a *fundamental system of entourages* of the uniformity $\mathscr{U}$. 现在$g_H$是$X$（no. 1）上的*伪计量*，以及$(g_H)$属于族的有限数的函数的上包络线，通过定义；我们用说来表达性质，伪计量学家族$(g_H)$是*饱和*的。 因此，伪测量族$(g_H)$“等价”于族$(f_i)$，并且据说是通过“饱和”$(f_i)$获得的伪测量族。 从刚才所说的可以看出，我们可能总是限制自己只考虑由“饱和”伪计量学族定义的均匀性。

在 $I$ 是*有限* 集合的特定情况下，该论证表明由伪度量族 $(f_i)_{i \in I}$ 定义的均匀性也由*单个* 伪度量 $g = \sup_{i \in I} f_i$ 定义。

令$\mathscr{U}, \mathscr{U}'$为$X$上的两个均匀性，分别由两个*饱和*族$(f_i)_{i \in I}, (g_x)_{x \in K}$定义。那么$\mathscr{U}$比$\mathscr{U}'$*粗糙*当且仅当，对于每个指标$i \in I$和每个实数$a > 0$，存在指标$x \in K$和数$b > 0$使得关系 $g_x(x, y) \leq b$ 意味着$f_i(x, y) \leq a$。

*例由一系列伪度量定义的均匀性。* 令 $(f_i)_{i \in I}$ 为在集合 $X$ 上定义的任意（有限）*实值函数* 族。令 $\mathscr{U}$ 为 $X$ 上的最粗糙均匀度，$f_i$ 相对于此均匀连续 (章 II, § 2, no. 3)。然后从$\mathscr{U}$ (*loc.cit.*) 的随从的定义得出$\mathscr{U}$是伪度量在$X$上定义的均匀性

$$
g_i(x, y) = |f_i(x) - f_i(y)|.
$$

### 3. 伪测量学族定义的均匀性的性质

令 $\mathscr{U}$ 为由一系列有限伪度量 $(f_i)$ 在集合 $X$ 上定义的均匀性。如果我们赋予$X \times X$本身$\mathscr{U}$的均匀性乘积，那么每个实值函数$f_i$在$X \times X$上都是“均匀连续”；对于 (1) 我们有

$$
|f_i(x, y) - f_i(x', y')| \leq f_i(x, x') + f_i(y, y'),
$$

因此关系 $f_i(x, x') \leq \varepsilon/2, f_i(y, y') \leq \varepsilon/2$ 意味着

$$
|f_i(x, y) - f_i(x', y')| \leq \varepsilon.
$$

对于$\mathscr{U}$成为*Hausdorff*，从$\mathscr{U}$的随行人员的定义开始，对于$X$的*不同*点$x, y$的每个对来说，有指标$i$使得$f_i(x, y) \neq 0$。

特别是，如果$\mathscr{U}$由*单个*伪度量$f$定义，则$\mathscr{U}$是豪斯多夫当且仅当关系$f(x, y) = 0$暗示$x = y$（cf.§ 2）。如果$\mathscr{U}$不是Hausdorff，则$\mathscr{U}$的所有随从的交是对$(x, y)$的$X \times X$由……组成的子集，使得所有$i$的$f_i(x, y) = 0$；这个子集是等价关系$R$在$X$上的图，与$\mathscr{U}$相关的豪斯多夫均匀性定义在$X/R$上（cf.章II, § 3, no. 8）。然后很容易验证函数$f_i$（在$x$和$y$中）与关系$R$（*集合理论*，R，§ 5, no. 7）相容的，并且函数$\overline{f_i}$，从$f_i$除以经过商（相对于$x$和$y$），是$X/R$上的伪度量，其中定义与$\mathscr{U}$相关的豪斯多夫均匀性（cf.§ 2, no. 1）。

如果$A$是$X$的非空子集，则$X$上的伪度量的限制到$A \times A$显然是$A$上的伪度量。 $\mathscr{U}$ 在 $A$ 上*引起的均匀性显然是由伪度量$f_i$ 的限制到 $A \times A$ 系列定义的。

现在让我们看看当$\mathscr{U}$是Hausdorff时制服空间$X$的*完成*。

#### 命题 1 {#top-ix-s1-prop-1 .statement tag=0C1F}

*设$X$为豪斯多夫均匀空间，其均匀性$\mathscr{U}$由一系列有限伪度量*$(f_i)$定义，*并让*$\hat{X}$*为$X$的完成*。那么函数$f_i$可以通过连续性扩展到$\hat{X} \times \hat{X}$；扩展的函数$\bar{f}_i$是$\hat{X} \times \hat{X}$上的有限伪度量，$(f_i)$定义族是$\hat{X}$的均匀性。

首先，$f_i$可以通过连续性扩展到$\hat{X} \times \hat{X}$，因为它们在$X \times X$上一致连续；且扩展函数$\bar{f}_i$在$\hat{X} \times \hat{X}$上均匀连续（章II, § 3, no. 6，定理2）；此外，由于不等式（章IV, § 5, no. 2，定理1）的原理或扩张，它们是$\hat{X}$上的伪度量。 令$\mathscr{U}_1$表示通过补全获得的$\hat{X}$上的均匀性，并令$\mathscr{U}_2$表示由伪度量族$(\bar{f}_i)$定义的均匀性。 那么$\mathscr{U}_2$比$\mathscr{U}_1$更粗糙；对于每个$\bar{f}_i$相对于$\mathscr{U}_1$在$\hat{X} \times \hat{X}$上一致连续，因此对于每个$a > 0$，存在$\mathscr{U}_1$的随从$V$，这样，每当$(x, y) \in V$时，我们就有$|\bar{f}_i(x, y) - \bar{f}_i(x, x)| \leq a$，即[自$\bar{f}_i(x, x) = 0$]， $V \subset \bar{f}_i([0, a])$；因此$\mathscr{U}_2$的每个随从都是$\mathscr{U}_1$的随从。 另一方面，$\mathscr{U}_1$和$\mathscr{U}_2$诱导在$X$上具有相同的均匀性$\mathscr{U}$。 由于$\hat{X}$相对于$\mathscr{U}_1$是完备的，因此$\mathscr{U}_1$和$\mathscr{U}_2$是相同的（章II, § 3, no. 7，命题14）。

### 4. 定义均匀性的伪测量学家族的构造

通过一系列伪测量来定义均匀性的意义在于，所有的均匀性都可以通过这种方式获得。即：

#### 定理 1 {#top-ix-s1-thm-1 .statement tag=0C1G}

给定集合 $X$ 上的均匀性 $\mathscr{U}$，$X$ 上存在一系列伪度量，使得该族定义的均匀性与 $\mathscr{U}$ 相同。

对于均匀性$\mathscr{U}$的每个周边$V$，定义归纳对称周边$(U_n)$的序列，使得对于所有$n \geq 1$有$U_1 \subset V$和$U_{n+1} \subset U_n$。 序列 $(U_n)$ 是均匀度 $\mathscr{U}_V$ 比 $\mathscr{U}$ 粗糙的基础系统；此外，很明显，$\mathscr{U}$是所有均匀性$U_V$中最小的上界，因为$V$穿过$\mathscr{U}$的随行人员过滤器。因此，定理 1 是以下命题中的推论：

#### 命题 2 {#top-ix-s1-prop-2 .statement tag=0C1H}

如果$X$上的均匀性$\mathscr{U}$具有可数的随行基数系统，则$X$上存在伪度量$f$，使得$\mathscr{U}$与$f$定义的均匀性相同。

设$(V_n)$是$\mathscr{U}$的随行人员的可数基本系统。 定义归纳序列 $(U_n)$ $\mathscr{U}$ 的对称周边，使得 $U_1 \subset V_1$ 和
$$
\bigcup_{n+1}^3 \subset U_n \cap V_n \quad \text{for} \quad n \geq 1.
$$
显然，$(U_n)$是$\mathscr{U}$随从的另一个基础系统，尤其是$\bigcup_{n+1}^3 \subset U_n$对于$n \geq 1$。我们在$X \times X$上定义实值函数$g$如下：$g(x, y) = 0$如果$(x, y) \in U_n$对于所有$n$； $g(x, y) = 2^{-k}$ 如果 $(x, y) \in U_n$ 代表 $1 \leq n \leq k$，但$(x, y) \notin U_{k+1}$； $g(x, y) = 1$ if $(x, y) \notin U_1$. 函数 $g$ 是对称且正的，对于所有 $x \in X$，我们都有 $g(x, x) = 0$。放
$$
f(x, y) = \inf \sum_{i=0}^{p-1} g(z_i, z_{i+1}),
$$
下确界接管所有有限序列 $(z_i)_{0 \leq i \leq p}$（$p$任意）中的集合，使得$z_0 = x$和$z_p = y$。我们将证明 $f$ 是一个满足不等式的“伪计量”
$$
\frac{1}{2} g(x, y) \leq f(x, y) \leq g(x, y).
$$
从定义可以立即得出 $f$ 是对称且正的，并且满足三角形不等式。而且很明显，$f(x, y) \leq g(x, y)$，因此$f(x, x) = 0$对于所有$x \in X$，因此$f$是伪度量。为了证明不等式 (2) 的左半部分，让我们通过 $p$ 上的归纳来证明，对于 $p + 1$ 点 $X$ 的每一个有限序列 $(z_i)_{0 \leq i \leq p}$，这样 $z_0 = x$ 和 $z_p = y$，我们有
$$
\sum_{i=0}^{p-1} g(z_i, z_{i+1}) \geq \frac{1}{2} g(x, y).
$$
如果$p = 1$，这很清楚。 Put $a = \sum_{i=0}^{p-1} g(z_i, z_{i+1})$;如果$a \geq 1/2$，则不等式 (3) 为真，因为$g(x, y) \leq 1$。假设 $a < 1/2$，并令 $h$ 为指标 $q$ 的最大的，使得
$$
\sum_{i < q} g(z_i, z_{i+1}) \leq \frac{a}{2};
$$
那么我们有$\sum_{i < h} g(z_i, z_{i+1}) \leq a/2$和$\sum_{i < h+1} g(z_i, z_{i+1}) > a/2$，从而
$$
\sum_{i > h} g(z_i, z_{i+1}) \leq \frac{a}{2}.
$$

通过归纳假设，我们有$g(x, z_h) \leq a$和$g(z_{h+1}, y) \leq a$；另一方面，很明显$g(z_h, z_{h+1}) \leq a$。令$k$为最小的整数$> 0$，使得$2^{-k} \leq a$；然后$k \geq 2$、$(x, z_h) \in U_k, (z_h, z_{h+1}) \in U_k, (z_{h+1}, y) \in U_k$乘$g$的定义；因此$(x, y) \in U_k \subset U_{k-1}^3$，这意味着$g(x, y) \leq 2^{1-k} \leq 2a$。

由此证明不等式(2)；他们表明，对于每个$a > 0$，集合$f^{-1}([0, a])$包含于$U_k$，对于每个指标$k$，使得$2^{-k} < a$，反之，每个$U_k$包含集合 $f^{-1}([0, 2^{-k-1}])$；因此，集合$f^{-1}([0, a])$形式是结构$\mathscr{U}$随行人员的基本系统。

Q.E.D.

#### 注 {#top-ix-s1-n4-rem-1 .statement tag=0C1I}

$X$上的均匀性$\mathscr{U}$由$X$上所有伪度量的族$\Phi$定义，这些伪度量在$X \times X$上一致连续。显然，$\Phi$族定义的均匀性比$\mathscr{U}$更粗糙；相反，定理 1 表明存在$\Phi$ 的子族，其定义均匀度$\mathscr{U}$，因此$\Phi$ 定义的均匀度比$\mathscr{U}$ 更细。

### 5. 可统一空间

在章II, § 4, no. 1中，我们提出了表征可均匀拓扑空间的问题。 解由以下定理给出：

#### 定理 2 {#top-ix-s1-thm-2 .statement tag=0C1J}

*拓扑空间* $X$ *可统一当且仅当它满足以下公理：*

(OIV) *给定任何点* $x_0 \in X$ *和任何邻域* $V$ ** $x_0$，*在* $X$ 上存在一个连续实值函数 *将其值放入* $[0, 1]$，*等于* $0$ *在* $x_0$，*并且等于* $1$ *在* $C_V$。

条件是必要的。因为如果$X$上存在与$X$的拓扑兼容的均匀性，那么通过定理1，这个均匀性可以由$X$上的伪测量族$(f_i)$来定义，并且我们可以不失一般性地假设该族是*饱和*（no. 2）。从由这样一个伪测量族定义的均匀性周围的定义，有一个$(f_i)$族的伪测量$f_\alpha$和数$a > 0$，这样对于所有$x \in C_V$都有$f_\alpha(x_0, x) \geq a$。由此可见函数$g(x) = \inf \left( 1, \frac{1}{a} f_\alpha(x_0, x) \right)$满足(OIV)中规定的所有条件。

条件就足够了。让$\Phi$是$X$到$[0, 1]$的所有*连续映射*的集合。公理 (OIV) 表明，*所有函数属于到* $\Phi$ *一致连续的最粗均匀性与 $X$ (章 II, § 2, no. 3) 的拓扑兼容*。

#### 定义 4 {#top-ix-s1-def-4 .statement tag=0C1K}

*如果拓扑空间是可均匀化且 Hausdorff 的，则称它是完全正则的。*

等价地，鉴于定理 2，如果空间满足公理(H) [cf. 章 I, § 8, no. 1, 命题 1] 和 (O_{IV})，则空间是完全正则的。

#### 注 {#top-ix-s1-n5-rem-1 .statement tag=0C1L}

公理 (O_{IV}) 意味着 (O_{III}) (cf. 章 I, § 8, no. 4)，因为如果 V 是 x_0 的邻域，并且如果 f 是 X 上的连续实值函数，且值在[0, 1]中，使得对于所有x \in \overline{V}，f(x_0) = 0, f(x) = 1，则集合 \overline{f}([0, 1/2]) 是V中包含的x_0的闭邻域。特别是，每个*完全规则*空间都是*规则*（这证明了术语）。但正则空间中有例不是完全正则(*)，所以(O_{III})并不隐含(O_{IV})。

每个紧凑空间都是完全正则的（章II, § 4, no. 1，定理1），因此紧凑空间的每个子空间也是如此。我们现在可以通过证明来完成这个命题 *逆命题*：

#### 命题 3 {#top-ix-s1-prop-3 .statement tag=0C1M}

*拓扑空间X是完全正则的当且仅当它与紧致空间的子空间同胚。*

考虑 X 上的最粗糙均匀性，相对于 X 到 [0, 1] 的所有连续映射都是均匀连续的；我们已经在定理 2 的证明中使用了这种均匀性，我们看到如果 X 是可均匀化的，那么它与 X 的拓扑兼容。此外，通过区间 [0, 1] 的紧致性和章 II, § 4, no. 2 的命题 3，该均匀性是 *预紧* 空间的结构。如果 X 是 Hausdorff，则X 对此的完备性因此是紧凑的，并且命题得到证明。

因此，我们可以说，完全规则的空间可以“嵌入”紧凑的空间中。通过以下方式呈现此结果通常很方便：

一般来说，*立方体*是拓扑空间 K^I、乘积的拓扑空间族，每个都与\mathbf{R}的*紧间隔* K相同，由任意集合I索引。如果I是有限的并且有n元素，我们恢复*n维封闭立方体*的概念，它在章VI, § 1, no. 1中定义。立方体是*紧凑* 空间 (章 I, § 9, no. 5, 定理 3)。

#### 命题 4 {#top-ix-s1-prop-4 .statement tag=0C1N}

*如果拓扑空间X是完全正则的，则它与立方体的子空间同胚。*

令 $(f_i)_{i \in I}$ 表示 X 的所有连续映射进入 K = [0, 1]，令 g 表示 X 的映射 $x \mapsto (f_i(x))$ 进入

(*) 参见 A. Tychonoff，*数学。安。*，102，（1930），p. 553。

K1。 如果$x, y$是$X$的任意两个不同的点，则根据公理(H)和(O_IV)，存在指标$i$使得$f_i(x) \neq f_i(y)$，因此$g$是$X$的*一对一*映射到$K^1$。 Moreover, it is immediate that $g$ is an isomorphism of the coarsest uniformity on $X$ for which all the $f_i$ are uniformly continuous, onto the uniformity induced on $g(X)$ by the product uniformity of $K^1$; *更不必说*，$g$是$X$到$g(X)$的同胚。

### 6. 均匀化空间上的半连续函数

在章IV, § 6, no. 2，定理4的推论中，我们证明了拓扑空间上连续实值族函数的上包络线是下半连续函数。如果空间是*可统一的*，则命题有逆命题：

#### 命题 5 {#top-ix-s1-prop-5 .statement tag=0C1O}

*在阶中，拓扑空间$X$上的每个下半连续实值函数$f$（有限或非有限）应该是$X$（有限或非有限）上的连续实值函数的上包络，其中$\leq f$，这是充分必要的$X$ 可统一。*

条件是*必要的*。令$x_0$为$X$的任意点，并令$V$为$x_0$的任意开邻域；则集合$V$的特征函数$\varphi_V$是下半连续的（章IV, § 6, no. 2，推论命题1）；因此，到假设，$X$上存在连续实值函数$g$，使得$g \leq \varphi_V$和$g(x_0) = a > 0$。连续的函数$\inf \left( 1, \frac{1}{a} g^+ \right)$在$[0, 1]$取其值，在$C_V$等于0，在$x_0$等于1。因此 (定理 2) $X$ 是可统一的。

条件*足够*。首先考虑$f$在$[-1, +1]$中取值的情况。我们必须证明，对于每个$x_0 \in X$和每个数$a < f(x_0)$，在$X$上都存在连续的实值函数$g$，使得$g \leq f$和$g(x_0) \geq a$。如果$a \leq -1$，我们可以取$g$作为常数$-1$。如果$-1 < a < f(x_0)$，则$x_0$有邻域$V$，使得所有$x \in V$都有$f(x) \geq a$。由于$X$是可统一的，$X$上有一个连续实值函数$h$，$[0, 1]$中有值，这样对于所有$x \in C_V$都有$h(x_0) = 0$和$h(x) = 1$。然后我们可以取$g(x) = a - (a + 1)h(x)$，并且我们有一个连续的函数满足指定的条件。 注这个函数在$[-1, +1]$ 中取其值。

一般情况下转移结构；因为$[-1, +1]$在$\overline{\mathbf{R}}$上存在严格递增的同胚（章IV, § 4, no. 2，命题2），并且半连续函数的定义仅涉及阶结构并且拓扑共 $\overline{\mathbf{R}}$。

#### 注 {#top-ix-s1-n6-rem-1 .statement tag=0C1P}

在上面的证明中，我们看到函数$g$并不需要值$+1$。通过传递结构，可得出可均匀化空间$X$上的每个下半连续实值函数$f$是$X$上连续实值函数$g \leq f$的上包络*不采用值* $+\infty$。

### 习题 {#top-ix-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
