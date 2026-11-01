---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 1
section_title: Upper integral of a positive function
lang: zh
source: int-i-vi
pdf_pages: 0108-0118, 0225-0227
extraction: ocr
subsections:
    - "no": 1
      title: Upper integral of a lower semi-continuous positive function
      page: 0
      pdf_page: 108
    - "no": 2
      title: Outer measure of an open set
      page: 4
      pdf_page: 111
    - "no": 3
      title: Upper integral of a positive function
      page: 6
      pdf_page: 113
    - "no": 4
      title: Outer measure of an arbitrary set
      page: 10
      pdf_page: 117
statements: 34
exercises: 8
content_sha256: 763156bef545dd2997bc6f1b7024ae7c2680d333083f2a634358915526dc4281
translated_from: content/en/int/IV/01_s1_upper_integral_of_a_positive_function.md
translation_method: google
source_content_sha256: faecbc2539033964cc900d67680366e3bd2e09f8e66d8294cd0ca0a84e783552
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 84184fadaf26d38aaf68ee82ab2a2aa0c402c66d57c9baa49354ff12e13736f1
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。正函数的上积分

### 1. 下半连续正函数的上积分

令X为局部紧致空间，$\mu$为X的正测度；我们知道$\mu$在格子$\mathscr{K}_+(X)$上是递增函数（也将表示为$\mathscr{K}_+$）。

我们用X上的数值函数的$\mathscr{I}_+(X)$（或简称为$\mathscr{I}_+$）集合表示，无论是否有限，它们在X上都是正的且下半连续。\脚注{1}回想一下，函数的任何族的和 $\mathscr{I}_+$属于至$\mathscr{I}_+$； $\mathscr{I}_+$中的函数的乘积由有限的数$\alpha > 0$属于到$\mathscr{I}_+$； $\mathscr{I}_+$中函数的*任何*系列的上封套和$\mathscr{I}_+$中函数的*有限*系列的下封套以及属于至$\mathscr{I}_+$（GT、IV, §6, No. 2、第2条和第4条）。我们还将利用以下引理：

#### 引理 {#int-iv-s1-n1-lem-1 .statement tag=08P2}

— *每个函数* $f \in \mathscr{I}_+$ *是集合* 的上封套（针对关系 $\leq$）*所有函数* $g \in \mathscr{K}_+$ *使得* $g \leq f$。

对于每个$x \in X$使得$f(x) > 0$，以及对于每个实数$a$使得$0 < a < f(x)$，在假设存在一个$x$的紧邻域V使得$f(y) \geq a$在V上；另一方面，存在函数$g \in \mathscr{K}_+$，V包含支持，等于$a$在点$x$和$\leq a$

(1) “I”，如“下等”；字母$\mathscr{L}$（如“下”）被其他函数空间抢占，将在§3中讨论。

V（GT、IX, §1, No. 5、周四 2）；因此$0 \leq g \leq f$和$g(x) \geq a$，这就证明了引理。

#### 定义 1 {#int-iv-s1-def-1 .statement tag=08P3}

*给定 $X$ 上的正测度$\mu$，可将函数$f \in \mathscr{J}_+$（相对于$\mu$）的上积分称为正数（有限或等于$+\infty$）*

$$
\mu^*(f) = \sup_{g \in \mathscr{H}_+, g \leq f} \mu(g).
$$

对于每个函数$f \in \mathscr{H}_+$，很明显$\mu^*(f) = \mu(f)$，在其他字$\mu^*$中是$\mu$到$\mathscr{J}_+$的*扩张*。

#### 例 {#int-iv-s1-n1-exa-1 .statement tag=08P4}

— 令$X$为*离散*空间，$\mu$为$X$的正测度，集合$\alpha(x) = \mu(\varphi_{\{x\}})$为所有$x \in X$。那么在 $X$ 上定义的每个数值函数 $f$ 都是连续的；对于这样的函数$f \geq 0$、$\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$，每当$\alpha(x) = 0$和$f(x) = +\infty$时，我们同意集合$\alpha(x)f(x) = 0$。对于，
$$
\sum_{x \in X} \alpha(x)f(x) = \sup_M \left( \sum_{x \in M} \alpha(x)f(x) \right),
$$
其中 $M$ 超过 $X$ 的所有有限子集中的集合。如果存在$x_0 \in X$使得$f(x_0) = +\infty$和$\alpha(x_0) > 0$，则每当$x_0 \in M$时就有$\sum_{x \in M} \alpha(x)f(x) = +\infty$，而另一方面，对于每个整数$n > 0$，$f \geq n \cdot \varphi_{\{x_0\}}$，因此$\mu^*(f) \geq n \alpha(x_0)$等等$\mu^*(f) = +\infty$。相反，如果 $\alpha(x) = 0$ 位于点，其中 $f(x) = +\infty$，则函数 $g$ 等于 $f$，位于点 $x \in M$，其中 $\alpha(x) > 0$ 且在其他地方属于等于 0 $\mathscr{H}_+$，因此，根据约定，$\mu(g) = \sum_{x \in M} \alpha(x)f(x)$，这再次证明了关系$\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$。

#### 命题 1 {#int-iv-s1-prop-1 .statement tag=08P5}

*对于每个有限的实数$\alpha > 0$和每个函数$f \in \mathscr{J}_+$，*
$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### 命题 2 {#int-iv-s1-prop-2 .statement tag=08P6}

*集合$\mathscr{J}_+$，函数$\mu^*$为递增。*
证明是来自 Def 的直接的。 1.

#### 定理 1 {#int-iv-s1-thm-1 .statement tag=08P7}

*令$H$为$\mathscr{J}_+$中函数的非空集合，指向关系$\leq$。对于$X$上的每一项积极措施$\mu$，*
$$
\mu^*\left( \sup_{g \in H} g \right) = \sup_{g \in H} \mu^*(g) = \lim_{g \in H} \mu^*(g).
$$

让$f = \sup_{g \in H} g$。我们首先要证明定理的特殊情况，即函数$g \in H$及其上包络线$f$*属于到*$\mathscr{H}_+$。然后，根据 Dini 的定理（GT、X, §4, No. 1、Th.1），$H$ 的截面滤波器在 $X$ 的每个紧凑子集上，特别是在 $f$ 的支持 K 上*均匀地*收敛到 $f$。由于$0 \leq g \leq f$对于每个函数$g \in \mathbf{H}$，$\mathbf{H}$中每个函数的支持度都包含在$K$中；但定义$\mu$在连续函数的向量空间$\mathscr{K}(X, K; \mathbf{C})$上连续，并包含在$K$中的支持，对于一致收敛的拓扑；在这种情况下，从而关系 (2)。

让我们讨论一般情况。很明显，对于每个函数$g \in \mathbf{H}$，$\mu^*(g) \leq \mu^*(f)$。由Def。 1，这一切都归结为，对于每个函数$\psi \in \mathscr{K}_+$使得$\psi \leq f$，

$$
\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g).
$$

对于每个函数$g \in \mathbf{H}$，令$\Phi_g$为函数$\varphi \in \mathscr{K}_+$的集合，使得$\varphi \leq g$，并令$\Phi$为集合$\Phi_g$的并，如$g$运行超过$\mathbf{H}$；由于$\mathbf{H}$是有向的，所以$\Phi$和$f = \sup_{\varphi \in \Phi} \varphi$也是有向的。由于$\psi \leq f$，$\psi$是函数$\inf(\psi, \varphi)$的集合的上包络线，因为$\varphi$超过$\Phi$；但从$\psi$和函数$\inf(\psi, \varphi)$属于到$\mathscr{K}_+$，证明的第一个部分显示$\mu(\psi) = \sup_{\varphi \in \Phi} \mu(\inf(\psi, \varphi))$。现在，每个 $\varphi \in \Phi$ 属于到集合 $\Phi_g$，因此

$$
\mu(\inf(\psi, \varphi)) \leq \mu(\varphi) \leq \mu^*(g) \leq \sup_{g \in \mathbf{H}} \mu^*(g),
$$

由此立即得出$\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g)$。由此我们证明了$\mu^*(f) = \sup_{g \in \mathbf{H}} \mu^*(g)$；那么关系$\mu^*(f) = \lim_{g \in \mathbf{H}} \mu^*(g)$就是单调极限定理的推论（GT，IV, §5, No. 2，Th.2）。

#### 定理 2 {#int-iv-s1-thm-2 .statement tag=08P8}

*如果$f_1$和$f_2$是$\mathscr{I}_+$中的两个函数那么*

$$
\mu^*(f_1 + f_2) = \mu^*(f_1) + \mu^*(f_2).
$$

由于$\varphi_1$（或$\varphi_2$）在$\mathscr{K}_+$中超过函数的集合，因此$\varphi_1 \leq f_1$（或$\varphi_2 \leq f_2$），函数$\varphi_1 + \varphi_2$形式有向集合 （对于$\leq$）其上封套是$f_1 + f_2$。因此，通过 Th. 1、

$$
\mu^*(f_1 + f_2) = \sup \mu(\varphi_1 + \varphi_2) = \sup (\mu(\varphi_1) + \mu(\varphi_2)),
$$

其中$(\varphi_1, \varphi_2)$超过$\mathscr{K}_+$中函数的对的集合，使得$\varphi_1 \leq f_1$和$\varphi_2 \leq f_2$；自从

$$
\sup (\mu(\varphi_1) + \mu(\varphi_2)) = \sup \mu(\varphi_1) + \sup \mu(\varphi_2)
$$

（GT，IV, §5, No. 7，第 12 号提案的 Cor.2），定理已被证明。

#### 命题 3 {#int-iv-s1-prop-3 .statement tag=08P9}

— *对于每个家庭* $(f_\iota)_{\iota \in I}$ *函数中* $J_+$，

$$
\mu^*\left( \sum_{\iota \in I} f_\iota \right) = \sum_{\iota \in I} \mu^*(f_\iota).
$$

对于 $I$ 的每个有限子集 $J$，可以从 Th 得出。 2 (由$J$元素数归纳)$\mu^*\left( \sum_{\iota \in J} f_\iota \right) = \sum_{\iota \in J} \mu^*(f_\iota)$； as $J$ runs over 集合 of 有限子集 of $I$, 函数 $g_J = \sum_{\iota \in J} f_\iota$ 属于 to $J_+$ and 形式有向集合 for 关系 $\leq$, whose upper envelope is 函数$\sum_{\iota \in I} f_\iota$；因此命题由 Th 得出。 1.

#### 命题 4 {#int-iv-s1-prop-4 .statement tag=08PA}

— *让*$f$*成为函数在*$J_+$中。 *映射* $\mu \mapsto \mu^*(f)$ *of 集合* $\mathscr{M}_+(X)$ *of positive measures on* $X$, *into the extended 实直线* $\overline{\mathbf{R}}$, *is lower semi-continuous for the vague 拓扑 on* $\mathscr{M}_+(X)$ *(Ch. III, §1, No. 9)*。

For, this 映射 is by 定义 the upper envelope of 映射 $\mu \mapsto \mu(g)$, where $g$ runs over 集合 of 函数 in $\mathscr{K}_+$ such that $g \leq f$;并且通过模糊拓扑的定义，映射$\mu \mapsto \mu(g)$在$\mathscr{M}(X)$上连续。

### 2. 开放的外部尺寸集合

给定一个 *开* 集合 $G \subset X$，其特征函数 $\varphi_G$ 在 $X$ 上是“下半连续”（GT，IV, §6, No. 2，Prop. 1 的 Cor.）。因此，我们可以做出以下定义：

#### 定义 2 {#int-iv-s1-def-2 .statement tag=08PB}

— *Given a positive measure* $\mu$ *on* $X$, *for every open 集合* $G \subset X$ *upper integral* $\mu^*(\varphi_G)$ *is called the outer measure of* $G$ *and is denoted* $\mu^*(G)$.

因此，开集合$G$的外部度量为数$\geq 0$，有限或等于$+\infty$。显然$\mu^*(\varnothing) = 0$。此外，$\mu^*(X) = \| \mu \|,$如第1章公式(22)所示。 III, §1, No. 8。

#### 命题 5 {#int-iv-s1-prop-5 .statement tag=08PC}

— *相对紧凑的开放集合* $G$ *的外部测量是有限的*。

因为，在这种情况下存在函数 $f \in \mathscr{K}_+$ 使得 $\varphi_G \leq f$ (Ch. III, §1, No. 2, 引理 1), 从而

$$
\mu^*(G) = \mu^*(\varphi_G) \leq \mu^*(f) = \mu(f) < +\infty.
$$

有限外部测度的开集合并不总是相对紧凑（例 3）。

#### 命题 6 {#int-iv-s1-prop-6 .statement tag=08PD}

—*如果*G₁和G2*是两个开集合，使得*G₁⊂G2，*则*μ*(G₁)≤μ*(G2)。
对于，关系 G₁ ⊂ G2 等价于 φG₁ ≤ φG2。

#### 命题 7 {#int-iv-s1-prop-7 .statement tag=08PE}

— *设*$\mathfrak{B}$*为针对关系*⊂的*X*开子集集合； *然后*

$$
\mu^*\left(\bigcup_{G \in \mathfrak{B}} G\right) = \sup_{G \in \mathfrak{B}} \mu^*(G).
$$

函数 φ_G 形式有向集合 (for ≤) in $\mathscr{I}_+$ and their upper envelope is the characteristic 函数 of 并 of 集合 G ∈ $\mathfrak{B}$;因此命题是 Th 的推论。 1.

#### 命题 8 {#int-iv-s1-prop-8 .statement tag=08PF}

— *设* (G_ι)_{ι \in I} *为任意开集合族；那么*

$$
\mu^*\left(\bigcup_{\iota \in I} G_\iota\right) \leq \sum_{\iota \in I} \mu^*(G_\iota).
$$

*此外，如果* G_ι *是成对的不相交的那么*

$$
\mu^*\left(\bigcup_{\iota \in I} G_\iota\right) = \sum_{\iota \in I} \mu^*(G_\iota).
$$

对于，如果 G = $\bigcup_{\iota \in I} G_\iota$ 则 φ_G = su_{ι \in I} φ_{G_ι} ≤ $\sum_{\iota \in I} \varphi_{G_\iota}$；当G_ι成对不相交的时，φ_G = $\sum_{\iota \in I} \varphi_{G_\iota}$；因此，命题是 Props 的推论。 2和3。

#### 例 {#int-iv-s1-n2-exa-1 .statement tag=08PG}

— 令 X = \mathbf{R} 并令 μ 为 \mathbf{R} 上的勒贝格测度（第 III, §1, No. 3 章）；我们将得到确定 *开区间* G = ]a, b[ (−∞ ≤ a < b ≤ +∞) 的外部测度。首先假设 a 和 b 是有限的。对于 $\mathscr{K}_+$ 中的每个函数 f，且 f ≤ φ_G，我们可以通过平均值的定理（FRV，II, §1, No. 5，命题 6），

$$
\int_{-\infty}^{+\infty} f(x)\, dx = \int_a^b f(x)\, dx \leq b - a,
$$

从而$\mu^*(G) \leq b - a$。另一方面，对于每个$\varepsilon > 0$，都存在函数$f \in \mathscr{K}_+$，使得$f \leq \varphi_G$和$f(x) = 1$对于$a + \varepsilon \leq x \leq b - \varepsilon$，从而$\mu^*(G) \geq b - a - 2\varepsilon$；由于 $\varepsilon$ 是任意的，$\mu^*(G) = b - a$；在其他字中，$G$的外部度量等于其*长度*。对于 $G$ 是无界开区间的情况，此结果为扩展，因为它随后包含有界开区间为任意大长度；因此在这种情况下是$\mu^*(G) = +\infty$。

现在令$G$为$\mathbf{R}$中任意开集合； $G$ 是成对不相交的开区间 $]a_k, b_k[$ 的可数集合（有限或无限）的并（GT，IV, §2, No. 5，命题 2），因而

$$
\mu^*(G) = \sum_k (b_k - a_k)
$$

（提案 8）；其他字：

#### 命题 9 {#int-iv-s1-prop-9 .statement tag=08PH}

*对于$\mathbf{R}$上的勒贝格测度，$\mathbf{R}$中开集合的外部测度等于其连通分量的长度的和。*

注特别是，如果$G$ 是$\mathbf{R}$ 中的开集合，使得$\mu^*(G) = 0$，则$G$ 是*空*。

### 3. 正函数的上积分

对于$X$上定义的每个数值函数$f \geq 0$（有限或非有限），都存在函数$h \in \mathscr{I}_+$，这样$f \leq h$，如果没有其他则为常数$+\infty$。

#### 定义 3 {#int-iv-s1-def-3 .statement tag=08PI}

*令$\mu$为$X$的正测度；对于 $X$ 上定义的每个数字函数 $f \geq 0$（有限或非有限），正数*

$$
\mu^*(f) = \inf_{h \geq f, h \in \mathscr{I}_+} \mu^*(h)
$$

(*有限或等于$+\infty$) *称为$f$的上积分（相对于$\mu$）。*

当$f \in \mathscr{I}_+$时，数$\mu^*(f)$等于Def中定义的上积分。 1、因为 $\mu^*$ 是 $\mathscr{I}_+$ 中的递增。

我们还将使用记号$\int^* f d\mu$、$\int^* f(x) d\mu(x)$、$\int^* f \mu$和$\int^* f(x) \mu(x)$来代替记号$\mu^*(f)$。

#### 例 {#int-iv-s1-n3-exa-1 .statement tag=08PJ}

— 如果 $X$ 是*离散* 空间，$\mu$ $X$ 上的正测度，并且如果集合 $\alpha(x) = \mu(\varphi_{\{x\}})$，则$\mu^*(f) = \sum_{x \in X} \alpha(x) f(x)$ 对于$X$ 上定义的每个数值函数 $f \geq 0$，因为这样的函数是连续的（No. 1，*例*）。

#### 命题 10 {#int-iv-s1-prop-10 .statement tag=08PK}

— *如果 f 和 g 是在 X 上定义的两个数值函数 $\geqslant 0$，使得 $f \leqslant g$，则$\mu^*(f) \leqslant \mu^*(g)$。*

#### 命题 11 {#int-iv-s1-prop-11 .statement tag=08PL}

— *对于每个有限实数 $\alpha > 0$ 以及X 上定义的每个数值函数 $f \geqslant 0$，

$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### 命题 12 {#int-iv-s1-prop-12 .statement tag=08PM}

— *如果$f_1$和$f_2$是定义在X上的两个数值函数$\geqslant 0$，则

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(f_1) + \mu^*(f_2).
$$

对于每个函数$h_1 \in \mathscr{I}_+$这样$f_1 \leqslant h_1$和每个函数$h_2 \in \mathscr{I}_+$这样$f_2 \leqslant h_2$，我们有，通过Th。 2、

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(h_1 + h_2) = \mu^*(h_1) + \mu^*(h_2),
$$
从而（GT、IV, §5, No. 7、第 12 号提案第 2 条）

$$
\mu^*(f_1 + f_2) \leqslant \inf_{h_1 \geqslant f_1, h_1 \in \mathscr{I}_+} \mu^*(h_1) + \inf_{h_2 \geqslant f_2, h_2 \in \mathscr{I}_+} \mu^*(h_2),
$$
这正是不等式 (9)。

道具。 10、11和12表示$\mu^*$是在X（第I，No. 1）上定义的数值函数$\geqslant 0$的集合上的*递增正齐次*和*凸*函数。 注，如果$f_1$和$f_2$是任意两个正数函数，则(9)的两个成员不一定相等（§ 4，Exer.8d)）；在§5, No. 6中，我们将给出条件，其中等式成立。

#### 定理 3 {#int-iv-s1-thm-3 .statement tag=08PN}

— *对于X上定义的数值函数$\geqslant 0$的每个递增序列$(f_n)$，

$$
\mu^*\left( \sup_n f_n \right) = \sup_n \mu^*(f_n).
$$

由于函数 $f_n$ 都小于或等于 $\sup_n f_n$，所以一切都归结为证明 $\mu^*(\sup_n f_n) \leqslant \sup_n \mu^*(f_n)$；如果不等式的第二个成员是$+\infty$，这一点是显而易见的。相反的情况下，$\mu^*(f_n) < +\infty$对于所有$n$；我们将证明，对于每个$\varepsilon > 0$，$\mathscr{I}_+$中存在函数的*递增*序列$(g_n)$，使得$f_n \leqslant g_n$和$\mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon$。如果$g$是序列$(g_n)$的上包络线，那么我们将有$\mu^*(g) = \sup_n \mu^*(g_n)$（No. 1，Th.1），从而$\mu^*(g) \leqslant \sup \mu^*(f_n) + \varepsilon$；由于$\sup f_n \leqslant g$和$\varepsilon$是任意的，因此定理将被证明。

到假设，存在函数$h_n \in \mathscr{J}_+$使得$f_n \leq h_n$和$\mu^*(f_n) \leq \mu^*(h_n) \leq \mu^*(f_n) + \varepsilon/2^n$；让我们证明函数 $g_n = \sup(h_1, h_2, \ldots, h_n)$ 满足要求。它们为属于至$\mathscr{J}_+$、形式递增序列以及满足$f_n \leq g_n$所有$n$；我们将证明

$$
\mu^*(g_n) \leq \mu^*(f_n) + \varepsilon \left( 1 - \frac{1}{2^n} \right).
$$

让我们以归纳对$n$进行争论；案例$n = 1$是微不足道的。另一方面$g_{n+1} = \sup(g_n, h_{n+1})$、$g_n \geq f_n$和$h_{n+1} \geq f_{n+1} \geq f_n$、从而$\inf(g_n, h_{n+1}) \geq f_n$；自从

$$
\inf(g_n, h_{n+1}) + \sup(g_n, h_{n+1}) = g_n + h_{n+1},
$$

这是从 Th 得出的。 No. 1 中的 2 个

$$
\begin{align*}
\mu^*(g_{n+1}) &= \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(\inf(g_n, h_{n+1})) \\
&\leq \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(f_n) \\
&\leq \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^n} \right) + \frac{\varepsilon}{2^{n+1}} \\
&= \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^{n+1}} \right).
\end{align*}
$$

Q.E.D.

#### 推论{#int-iv-s1-n3-cor-1 .statement tag=08PO}

— *令$\mathfrak{F}$为数值函数$\geq 0$的集合，指向关系$\leq$，这样存在$\mathfrak{F}$的可数共尾子集$\mathfrak{G}$* (S, III, §1, No. 7);然后

$$
\mu^*\left( \sup_{f \in \mathfrak{F}} f \right) = \sup_{f \in \mathfrak{F}} \mu^*(f).
$$

例如，$\mathfrak{G}$中存在函数的递增、序列与$\mathfrak{F}$具有相同的上包络线：如果$(f_n)$是$\mathfrak{G}$的函数的序列，排列在任意阶中，令$(f_{n_k})$是由条件 $n_1 = 1$, $f_{n_{k+1}} \geq \sup(f_{n_k}, f_k)$ 递归定义的子序列；很明显，该子序列具有指定的属性。

#### 注 {#int-iv-s1-n3-rem-1 .statement tag=08PP}

— 1) 当$\mathfrak{F}$是函数$\geq 0$的*不可数*有向集合并且不是下半连续时，关系(11)不一定成立。取例$X = \mathbf{R}$，$\mu$是$\mathbf{R}$上的勒贝格测度，并考虑特征函数$\varphi_M$的有向（对于$\leq$）集合$\mathfrak{F}$的所有*有限*子集M $\mathbf{R}$。那么对于每一个有限子集 M，$\mu^*(\varphi_M) = 0$，因为点包含在任意小长度的开区间中，并且集合的特征函数减少到点，因此根据Def具有上积分零。 3 和No. 2 的第 9 号提案。但$\mathscr{F}$的上包络线是等于1的常数函数和$\mu^*(1) = +\infty$。

2) 注对于函数 $\geqslant 0$ 的 *递减* 序列 $(f_n)$，不一定有 $\mu^*(\inf_n f_n) = \inf_n \mu^*(f_n)$，即使对于所有 $n$ 都有 $\mu^*(f_n) < +\infty$ (cf.) §4，Exer 8 c))。

#### 命题 13 {#int-iv-s1-prop-13 .statement tag=08PQ}

*对于每个序列* $(f_n)$ *数值函数* $\geqslant 0$ *定义于* $X$，

$$
\mu^*\left( \sum_{n=1}^\infty f_n \right) \leqslant \sum_{n=1}^\infty \mu^*(f_n).
$$

只需应用函数$g_n = \sum_{k=1}^n f_k$的关系(10)到递增序列即可，同时考虑到，通过(9)，

$$
\mu^*(g_n) \leqslant \sum_{k=1}^n \mu^*(f_k).
$$

在 §5, No. 6 中，我们将给出条件，其中 (12) 的两个成员相等。

#### 命题 14（法图的引理）{#int-iv-s1-prop-14 .statement tag=08PR}

— *对于每个序列* $(f_n)$ *数值函数* $\geqslant 0$，

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \liminf_{n \to \infty} \mu^*(f_n).
$$

对于每个整数 $n$、集合 $g_n = \inf_{p \geqslant 0} f_{n+p}$； 序列 $(g_n)$ 是递增和 $\liminf_{n \to \infty} f_n = \sup_n g_n$、从而，通过 (10)，

$$
\mu^*(\liminf_{n \to \infty} f_n) = \sup_n \mu^*(g_n);
$$

但从$g_n \leqslant f_{n+p}$到$p \geqslant 0$，我们有$\mu^*(g_n) \leqslant \mu^*(f_{n+p})$，从而$\mu^*(g_n) \leqslant \inf_{p \geqslant 0} \mu^*(f_{n+p})$，最后

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \sup_n \left( \inf_{p \geqslant 0} \mu^*(f_{n+p}) \right) = \liminf_{n \to \infty} \mu^*(f_n).
$$

#### 推论{#int-iv-s1-n3-cor-2 .statement tag=08PS}

*让*$(f_n)$*成为数值函数*$\geqslant 0$*的序列*这样，对于每个*$x \in X$，$\lim_{n \to \infty} f_n(x) = +\infty$。 *如果* $\mu$ *不是零度量，则* $\lim_{n \to \infty} \mu^*(f_n) = +\infty$。

如果$f_0$是等于$+\infty$的常数函数，则$f_0$是$\mathscr{K}_+$的所有函数的上包络线，并且从$\mu \neq 0$开始，我们有$\mu^*(f_0) > 0$；但由于$f_0 = \alpha f_0$对应于每个$\alpha > 0$，必然有$\mu^*(f_0) = +\infty$（命题11）。 不等式 (13) 则表明 $\mu^*(f_n)$ 与 $n$ 趋向于 $+\infty$。

#### 命题 15 {#int-iv-s1-prop-15 .statement tag=08PT}

*对于$X$上的每个标量$\alpha > 0$和每个对积极措施$\mu, \nu$，*

$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + \nu)^* = \mu^* + \nu^*.
$$

*此外，关系$\mu \leq \nu$意味着$\mu^* \leq \nu^*$。*

让我们证明关系 (15)。 集合$\lambda = \mu + \nu$；因此 $\lambda(f) = \mu(f) + \nu(f)$ 为 $f \in \mathscr{K}_+$；对于 $f \in \mathscr{J}_+$、$\lambda^*(f)$（分别为 $\mu^*(f)$、$\nu^*(f)$）的值为 $\lambda(g)$（分别为 $\mu(g)$、$\nu(g)$）的极限，因为 $g$ 超出所有$g \in \mathscr{K}_+$中的有向集合（对于$\leq$）使得$g \leq f$；因此$\lambda^*(f) = \mu^*(f) + \nu^*(f)$。最后，如果$f$是在$X$上定义的任何函数$\geq 0$，则$\lambda^*(f)$（分别是$\mu^*(f)$、$\nu^*(f)$）是$\lambda^*(h)$（分别是$\mu^*(h)$）的极限， $\nu^*(h)$），因为$h$超过所有函数$h \in \mathscr{J}_+$中的有向集合（对于$\geq$），使得$h \geq f$；再次，通过极限，我们有$\lambda^*(f) = \mu^*(f) + \nu^*(f)$，这证明了（15）。 关系(14)同理成立。最后，如果$\mu \leq \nu$可以写成$\nu = \mu + (\nu - \mu)$，其中$\nu - \mu \geq 0$，因此$\nu^* = \mu^* + (\nu - \mu)^*$，这表明$\mu^* \leq \nu^*$。

### 4. 任意集合的外部度量

#### 定义 4 {#int-iv-s1-def-4 .statement tag=08PU}

*令$\mu$为$X$的正测度；对于$X$的每个子集$A$，上积分$\mu^*(\varphi_A)$称为$A$的外部测度（相对于测度$\mu$）并表示为$\mu^*(A)$。*

因此，集合的外部度量为数$\geq 0$，有限或等于$+\infty$，即，对于开放的集合，重合，其外部度量在Def中定义。 No. 2 中的 2 个。

#### 命题 16 {#int-iv-s1-prop-16 .statement tag=08PV}

*如果$A$和$B$是$X$中的两个子集，使得$A \subset B$，则$\mu^*(A) \leq \mu^*(B)$。*

#### 推论{#int-iv-s1-n4-cor-1 .statement tag=08PW}

*$X$中的每个相对紧集都有有限的外部测度。*

因为，这样的集合包含在一个相对紧凑的开集合（GT，I, §9, No. 7，命题10）中，其外部测度是有限的（No. 2，命题5）。

#### 命题 17 {#int-iv-s1-prop-17 .statement tag=08PX}

— *如果* $(A_n)$ *是X* 的子集中的递增序列，则$\mu^*(\bigcup_n A_n) = \sup_n \mu^*(A_n)$。

#### 命题 18 {#int-iv-s1-prop-18 .statement tag=08PY}

— *对于序列* $(A_n)$ *子集 X*，

$$
\mu^*\left(\bigcup_n A_n\right) \leq \sum_n \mu^*(A_n).
$$

这些命题是Props的翻译。 10和13以及Th。 No. 3中的3个用于特征函数中的集合。

#### 命题 19 {#int-iv-s1-prop-19 .statement tag=08PZ}

— *对于 X* 的每个子集 A，$\mu^*(A)$ *是开集合包含 A* 的外部度量的下确界。

如果$\mu^*(A) = +\infty$，则命题是明显的。相反的情况，对于每个$\varepsilon$使得$0 < \varepsilon < 1$，存在函数$f \in \mathscr{J}_+$使得$\varphi_A \leq f$和$\mu^*(A) \leq \mu^*(f) \leq \mu^*(A) + \varepsilon$。令 G 为 $x \in X$ 的集合，使得 $f(x) > 1 - \varepsilon$。由于$f$是下半连续的，G是*开*（GT，IV, §6, No. 2，命题1）和包含A；另一方面$f \geq (1 - \varepsilon)\varphi_G$，从而

$$
\mu^*(G) \leq \frac{1}{1 - \varepsilon} \mu^*(f) \leq \frac{1}{1 - \varepsilon} (\mu^*(A) + \varepsilon);
$$

由于 $\varepsilon$ 是任意的，我们可以看到 $\mu^*(G)$ 与 $\mu^*(A)$、从而命题的差异尽可能小。

### 习题 {#int-iv-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
