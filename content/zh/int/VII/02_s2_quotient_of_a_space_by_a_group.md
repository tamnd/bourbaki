---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 2
section_title: Quotient of a space by a group; homogeneous spaces
lang: zh
source: int-vii-ix
book_pages: INT VII.27-INT VII.53, INT VII.87-INT VII.91
pdf_pages: 0033-0059, 0093-0097
extraction: ocr
subsections:
    - "no": 1
      title: General results
      page: 27
      pdf_page: 33
    - "no": 2
      title: The case $\chi = 1$
      page: 29
      pdf_page: 35
    - "no": 3
      title: Another interpretation of $\lambda^\#$
      page: 32
      pdf_page: 38
    - "no": 4
      title: The case that $X/H$ is paracompact
      page: 36
      pdf_page: 42
    - "no": 5
      title: Quasi-invariant measures on a homogeneous space
      page: 38
      pdf_page: 44
    - "no": 6
      title: Relatively invariant measures on a homogeneous space
      page: 43
      pdf_page: 49
    - "no": 7
      title: Haar measure on a quotient group
      page: 44
      pdf_page: 50
    - "no": 8
      title: A transitivity property
      page: 45
      pdf_page: 51
    - "no": 9
      title: Construction of the Haar measure of a group from the Haar measures of certain subgroups
      page: 48
      pdf_page: 54
    - "no": 10
      title: Integration on a fundamental domain
      page: 50
      pdf_page: 56
statements: 53
exercises: 13
content_sha256: 89f0f99c13f9835a53b2b645bfd883e85822c6315be578cdc90016aa0b70d162
translated_from: content/en/int/VII/02_s2_quotient_of_a_space_by_a_group.md
translation_method: google
source_content_sha256: d9ff9314ec23606af6278353311f4d40b921e4f3cdc62b45c0636a8821d2e713
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: d84d2690b9ad73b390c04574e38dbd510e25d791aaa71eb3a4870cce597b575b
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。 商 / 空间 by 群；均质空间

### 1. 一般结果

令 X 为局部紧致空间，其中局部紧致群 H 通过 $(x, \xi) \mapsto x\xi$ ($x \in X, \xi \in H$) 在右侧连续正确地运算。 H 定义的 X 中的等价关系是开集（GT，III, §2, No. 4，引理 2），X/H 是 Hausdorff（*loc.cit.*，§4, No. 2，命题 3），因此是局部紧致的（GT，I, §10, No. 4，命题 10）。我们用 X 的 $\pi$ 典范映射表示到X/H。 X的子集Y的饱和度为$YH = \pi^{-1}(\pi(Y))$。如果 K 是 X 的紧致子集，则 $\pi(K)$ 是紧致的并且 K 的饱和度 $\pi^{-1}(\pi(K))$ 在 X 中闭合。每个X/H 的紧凑子集是像在$\pi$ 的X 紧凑子集之下（GT，I, §10, No. 4，提案10）。 *我们假设一劳永逸地给出 H* 上的左 Haar 测度 $\beta$。

令$\chi$为H在$\mathbf{R}_+^*$中的连续表示。如果X上的函数g对于所有$x \in X$和$\xi \in H$满足$g(x\xi) = \chi(\xi)g(x)$，则其支持度S在H下是不变的，因此可以写成$\pi^{-1}(\pi(S))$。我们用$\mathscr{K}^\chi(X)$表示X上连续实值函数g形成的Riesz空间，即满足$g(x\xi) = \chi(\xi)g(x)$($x \in X, \xi \in H$)，其支持是X的紧致子集的饱和；我们用$\mathscr{K}^\chi(X)$的元素$\geqslant 0$中的$\mathscr{K}_+^\chi(X)$集合来表示。特别地，$\mathscr{K}^1(X)$正是X上连续函数的集合，在轨道上恒定，其支持是紧凑子集的饱和。

#### 命题 1 {#int-vii-s2-prop-1 .statement tag=09EY}

*设f是X上的连续实值函数，其支持S具有紧致交，每个紧致子集的饱和度为X。*

a) *对于 H 属于至 $\mathscr{K}(H)$ 上的每个 $x \in X$、函数 $\xi \mapsto f(x\xi)$；一个集合*

$$
f^\chi(x) = \int_H f(x\xi)\chi(\xi)^{-1}\, d\beta(\xi).
$$

b) *函数 $f^\chi$是连续的，零在SH之外，并且满足$f^\chi(x\xi) = \chi(\xi)f^\chi(x)$。*

c) *如果g是X上的连续实值函数并且满足$g(x\xi) = \chi(\xi)g(x)$，则$(fg)^\chi = f^1g$（$f^1$由公式（1）给出，其中$\chi$替换为H中的表示$\xi \mapsto 1$） $\mathbf{R}_+^*$).*

d) *如果*$\eta \in \mathbf{H}$，*则*$(\delta(\eta)f)^{\chi} = \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1}f^{\chi}$。

令$x_0 \in X$和$V$是$x_0$在$X$的紧邻域。 $\xi \in \mathbf{H}$的集合使得$V\xi$与$S$相交，也是$\xi \in \mathbf{H}$的集合使得$V\xi$与$S \cap VH$相交，因此在$\mathbf{H}$中是紧致的，因为$S \cap VH$是紧致的并且$\mathbf{H}$在$X$（GT、III, §4, No. 5、Th.1）下正常运行；那么§1, No. 1的引理1证明了a)和$f^{\chi}$的连续性。 b) 的其余部分是显而易见的。最后，c) 和 d) 由以下计算得出：

$$
(fg)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi)g(x\xi)\chi(\xi)^{-1}\,d\beta(\xi) = \int_{\mathbf{H}} f(x\xi)g(x)\chi(\xi)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= g(x) \int_{\mathbf{H}} f(x\xi)\,d\beta(\xi) = g(x)f^{1}(x)
$$

$$
(\delta(\eta)f)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi\eta)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= \Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi\eta^{-1})^{-1}\,d\beta(\xi)
$$
$$
= \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi)^{-1}\,d\beta(\xi).
$$

#### 命题 2 {#int-vii-s2-prop-2 .statement tag=09EZ}

*映射* $f \mapsto f^{\chi}$ *的* $\mathscr{K}(X)$ *进入* $\mathscr{K}^{\chi}(X)$ *是线性的，并且像的* $\mathscr{K}(X)$ *（或$\mathscr{K}_{+}(X)$）是* $\mathscr{K}^{\chi}(X)$ *（或$\mathscr{K}_{+}^{\chi}(X)$）。*

线性度为直接的。显然，$f^{\chi} \geqslant 0$ 对应$f \geqslant 0$。然后应用以下引理就足够了：

#### 引理 1 {#int-vii-s2-lem-1 .statement tag=09F0}

— *让*$K$*成为*$X$的紧凑子集，*$\mathscr{K}_{+}(X)$的*u函数*与*$u(x) > 0$*对于*$x \in K$。 *让*$g \in \mathscr{K}^{\chi}(X)$*使得*$\operatorname{Supp} g \subset KH$。
a) *一个有* $\inf_{x \in KH} u^{1}(x) > 0$。
b) *函数* $h$ *等于* $g/u^{1}$ *在* $KH$，*并且到* $0$ *在* $X - KH$，*属于到* $\mathscr{K}^{\chi}(X)$。
c) $g = (uh)^{\chi}$。
一个人有 $u^{1}(x) > 0$ 对应 $x \in K$，因此 $\inf_{x \in KH} u^{1}(x) = \inf_{x \in K} u^{1}(x) > 0$。
断言 b) 由此立即得出。最后，根据命题 1 c) 得到$(uh)^{\chi} = u^{1}h$，并且显然$u^{1}h = g$。

令 I 为 $\mathscr{K}^{\chi}(X)$ 上的相对有界线性形式 (Ch. II, §2, No. 2)。那么$f \mapsto I(f^{\chi})$是$\mathscr{K}(X)$上的相对有界线性形式，即$X$上的*测度*$\mu_{I}$。 映射 $I \mapsto \mu_{I}$ 由命题 2 内射。如此获得的 $X$ 上的测度 $\mu_{I}$ 可以表征如下：

#### 命题 3 {#int-vii-s2-prop-3 .statement tag=09F1}

*让*$\mu$*作为*$X$的度量。 *以下条件等效：*

a) 在$\mathscr{K}^\chi(X)$上存在相对有界的线性形式I，使得$I(f^\chi) = \mu(f)$对于所有$f \in \mathscr{K}(X)$。
b) $\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$ 对于所有 $\xi \in H$。
c) 对于$\mathscr{K}(X)$中的所有$f, g$，

(2)
$$
\mu(f \cdot g^1) = \mu(f^\chi \cdot g) .
$$

d) 如果$f \in \mathscr{K}(X)$使得$f^\chi = 0$，则$\mu(f) = 0$。

a) $\Rightarrow$ b): 如果 $\mu(f) = I(f^\chi)$ 那么，考虑到提案 1 d)，

$$
\langle \delta(\xi)\mu, f \rangle = \langle \mu, \delta(\xi^{-1})f \rangle = I\left( (\delta(\xi^{-1})f)^\chi \right)
= I(\chi(\xi)^{-1} \Delta_H(\xi)f^\chi)
= \chi(\xi)^{-1} \Delta_H(\xi) \langle \mu, f \rangle ,
$$

从而$\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$。

b) $\Rightarrow$ c)：假设满足假设 b)。请注意，$X \times H$上的函数$(x, \xi) \mapsto f(x)g(x\xi)$和$(x, \xi) \mapsto f(x\xi)g(x)$是连续的，具有紧凑的支持（因为$H$在$X$中可以正常运行）；这成立了，Th。第 2 章。 III, §4, No. 1 允许我们写：

$$
\int_X f(x) d\mu(x) \int_H g(x\xi) d\beta(\xi) = \int_H d\beta(\xi) \int_X f(x)g(x\xi) d\mu(x)
= \int_H d\beta(\xi) \int_X f(x\xi^{-1})g(x)\chi(\xi)\Delta_H(\xi)^{-1} d\mu(x)
= \int_X g(x) d\mu(x) \int_H f(x\xi^{-1})\chi(\xi)\Delta_H(\xi)^{-1} d\beta(\xi)
= \int_X g(x) d\mu(x) \int_H f(x\xi)\chi(\xi)^{-1} d\beta(\xi),
$$

这就证明了c）。

c) $\Rightarrow$ d)：如果 c) 被验证，并且如果 $f^\chi = 0$，则$\mu(f \cdot g^1) = 0$ 对于所有 $g \in \mathscr{K}(X)$，因此选择 $g \in \mathscr{K}(X)$ 时$\mu(f) = 0$，使得 $g^1 = 1$ $\mathrm{Supp}\, f$（这可以通过与 $\chi = 1$ 一起应用的第 2 条提案实现）。

d) $\Rightarrow$ a)：如果满足条件 d)，则在$\mathscr{K}^\chi(X)$上存在线性形式I，使得$\mu(f) = I(f^\chi)$对于$f \in \mathscr{K}(X)$，并且根据命题2，这个形式是相对有界的。

### 2. 案例$\chi = 1$

如果$f$在$X/H$上是函数，则$f \circ \pi$在$X$上是函数，在轨道上恒定，连续当且仅当$f$连续。 映射 $f \mapsto f \circ \pi$ 定义特别是 $\mathscr{K}(X/H)$ 的双射到 $\mathscr{K}^1(X)$。

然后，在$\chi = 1$的情况下，我们可以通过以下方式重新表述No. 1的某些结果：

令$f$为$X$上的连续数值函数，其支持具有紧致交，且每个紧致子集的饱和度为$X$。 公式

$$
f^b(\pi(x)) = \int_H f(x\xi)\, d\beta(\xi)
$$

定义 $X/H$ 上连续的函数 $f^b$。如果$g$是$X/H$上的连续函数，那么

$$
(f \cdot g \circ \pi)^b = f^b \cdot g .
$$

如果$\eta \in H$，那么

$$
(\delta(\eta)f)^b = \Delta_H(\eta)^{-1} f^b .
$$

不要忘记，$f^b$ 的定义取决于$\beta$ 的选择。如果 $H$ 是紧致的并且 $\beta$ 是标准化的，则函数 $f^b$ 是有时，称为 $f$ 的*轨道平均值*。

如果$f \in \mathscr{K}(X)$，则$f^b \in \mathscr{K}(X/H)$。 $\mathscr{K}(X)$到$\mathscr{K}(X/H)$的映射$f \mapsto f^b$是线性的，$\mathscr{K}(X)$（或$\mathscr{K}_+(X)$）的像是$\mathscr{K}(X/H)$（或$\mathscr{K}_+(X/H)$）。

#### 注 1 {#int-vii-s2-n2-rem-1 .statement tag=09F2}

— 我们将证明映射$f \mapsto f^b$是$\mathscr{K}(X)$到$\mathscr{K}(X/H)$的*严格态射*（GT，III, §2, No. 8）。

a) 映射是连续的：足以证明，对于$X$的每个紧凑子集$K$，$f \mapsto f^b$到$\mathscr{K}(X, K)$的限制是$\mathscr{K}(X, K)$到$\mathscr{K}(X/H, \pi(K))$的连续映射（TVS， II, §4, No. 4，提案 5)；由于$H$在$X$中正确运行，$\xi \in H$的集合$P$使得$K\xi$与$K$相交是紧凑的； (3) 中的一个结论就是$\sup_{x \in K} |f^b(\pi(x))| \leq \beta(P) \sup_{x \in K} |f(x)|$，这证明了我们的断言。

b) 令 $K'$ 为 $X/H$ 的紧致子集。让我们选择一个$X$的紧致子集$K$使得$\pi(K) = K'$，并让我们证明$f \mapsto f^b$到$\mathscr{K}(X, K)$的限制是$\mathscr{K}(X, K)$到$\mathscr{K}(X/H, K')$的严格态射。它足以满足构造这个限制的右逆（GT，III, §6, No. 2，命题3）。现在，通过 No. 1 的引理 1（我们采用其记号），可以通过组合以下映射来获得这样的逆：
将$\mathscr{K}(X/H, K')$的$\alpha)$映射$f' \mapsto f' \circ \pi$转换为$\mathscr{K}^1(X)$的函数集合$E$，其支持包含在$KH$中；
将$E$的$\beta)$映射转换为$E$，对于每个$g \in E$，使对应函数在$KH$上等于$g/u^1$，在$X - KH$上等于0；
将$E$的$\gamma)$映射转化为$\mathscr{K}(X)$，每函数$h \in E$，就得到对应$uh$。

c) 由此成立，如果$V$是$\mathscr{K}(X)$中0的凸邻域，则$V \cap \mathscr{K}(X, K)$是$\mathscr{K}(X, K)$中0的凸邻域，因此由b)可知$V^b \cap \mathscr{K}(X/H, K')$是$\mathscr{K}(X/H, K')$中0的凸邻域，因此$V^b$是$\mathscr{K}(X/H)$中0的凸邻域（TVS， II, §4, No. 4）。这样就完成了证明。

#### 命题 4 {#int-vii-s2-prop-4 .statement tag=09F3}

a) *令 $\lambda$ 为$X/H$ 的度量。 $X$ 上存在且仅有一个测度 $\lambda^\#$ 使得*
$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$
*对于所有$f \in \mathscr{K}(X)$。一个人拥有 $\delta(\xi)\lambda^\# = \Delta_H(\xi)\lambda^\#$，而所有$\xi \in H$。*

b) *相反，令 $\mu$ 为 $X$ 的度量，使得 $\delta(\xi)\mu = \Delta_H(\xi)\mu$ 对于所有 $\xi \in H$。 $X/H$ 上存在且仅有一个测度 $\lambda$ 使得$\mu = \lambda^\#$。*

这是命题 3 No. 1 的特例。

#### 定义 1 {#int-vii-s2-def-1 .statement tag=09F4}

*根据命题 4 中的假设和记号，$\lambda$ 被 $\beta$ 称为 $\mu$ 的商，并表示为 $\frac{\mu}{\beta}$ 或 $\mu/\beta$。*

$\mathscr{M}(X/H)$到$\mathscr{M}(X)$的映射$\lambda \mapsto \lambda^\#$无非是$\mathscr{K}(X)$的$f \mapsto f^b$到$\mathscr{K}(X/H)$的映射转置。 设$\mathfrak{F}$为$\mathscr{M}(X/H)$上的过滤器；说$\lim_{\lambda,\mathfrak{F}} \lambda^\#(f) = 0$对于所有$f \in \mathscr{K}(X)$相当于说，$\lim_{\lambda,\mathfrak{F}} \lambda(f') = 0$对于所有$f' \in \mathscr{K}(X/H)$；因此，对于模糊拓扑，映射$\lambda \mapsto \lambda^\#$是$\mathscr{M}(X/H)$的*同构*到$\mathscr{M}(X)$的线性子空间。 这个子空间是*模糊封闭的*，因为它是$\mu \in \mathscr{M}(X)$的集合，使得$\delta(\xi)\mu = \Delta_H(\xi)\mu$对于所有$\xi \in H$。 显然条件$\lambda \geqslant 0$和$\lambda^\# \geqslant 0$是等价的。

公式 (6) 可以与通常的双积分的记号类比，写成
$$
\int_X f(x) d\lambda^\#(x) = \int_{X/H} d\lambda(\dot{x}) \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$
这涉及到记号的滥用，$\int_H f(x\xi) d\beta(\xi)$的积分被视为$\dot{x}$的函数而不是$x$；在不引起混淆的情况下，这种书写方式将在下文中经常使用。

#### 注 2 {#int-vii-s2-n2-rem-2 .statement tag=09F5}

— 令 E 为局部凸向量空间，令 m 为 $X/H$ 上的向量测度，值在 E 中。$\mathscr{K}(X)$ 的映射 $f \mapsto m(f^b)$ 进入 E，则为 X 上的向量测度，值在 E 中，我们将再次表示为$m^\#$。 映射$m \mapsto m^\#$再次是$\mathscr{L}(\mathscr{K}(X/H); E)$的*同构*到$\mathscr{L}(\mathscr{K}(X); E)$的线性子空间A（当这些空间配备了逐点收敛的拓扑时）。此外，由于映射$f \mapsto f^b$是严格满射态射，子空间A精确地由X上的矢量测度n组成，即映射$f \mapsto f^b$的核N上的零。因此，在阶和 $n \in A$ 中，对于每个 $z' \in E'$，标量测量$z' \circ n$ 是 N 上的零是必要且充分的。然后从命题 3 推论出 $n \in A$ 当且仅当$\delta(\xi)n = \Delta_H(\xi)n$ 对于所有$\xi \in H$。

### 3. 另一个 $\lambda^\#$ 的解释

对于每个 $x \in X$，映射 $\xi \mapsto x\xi$ 将 H 放入 X 是适当的（GT，III, §4, No. 2，命题 4），因此 $\beta$ 承认在此映射下对 X 进行像测度，像是集中的关于轨道 $xH$（第 V, §6, No. 2 章，第 2 号提案第 3 条）；由于$\beta$是左不变的，因此像度量仅取决于$X/H$中$x$的类$u = \pi(x)$，并且将被表示为$\beta_u$。 定义，$f \in \mathscr{K}(X)$，

$$
\int_X f(y)\, d\beta_u(y) = \int_H f(x\xi)\, d\beta(\xi) = f^\flat(u).
$$

由此我们看出

$$
(\varepsilon_u)^\# = \beta_u.
$$

#### 引理 2 {#int-vii-s2-lem-2 .statement tag=09F6}

*设 f 为 X 上的函数，其中值位于拓扑空间中。*

a) *如果 f 是数值函数 $\geq 0$ 那么，对于 $x \in X$，*

$$
\int_X^* f(y)\, d\beta_{\dot{x}}(y) = \int_H^* f(x\xi)\, d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

b) *要使 f $\beta_{\dot{x}}$ 可测，H 上的函数 $\xi \mapsto f(x\xi)$ $\beta$ 可测是充分必要的。*

c) *假设f是X上的函数，值在Banach空间或$\overline{\mathbf{R}}$中；那么，要使 f $\beta_{\dot{x}}$ 可积（或本质上 $\beta_{\dot{x}}$ 可积），H 上的函数 $\xi \mapsto f(x\xi)$ 是 $\beta$ 可积（或本质上 $\beta$ 可积），在这种情况下 $\int_X f(y)\, d\beta_{\dot{x}}(y) = \int_H f(x\xi)\, d\beta(\xi)$.*

这是从第 1 章得出的。 V, §4、提案 2、提案 3 和 Th。 2.

由于 $f^\flat \in \mathscr{K}(X/H)$ 对于 $f \in \mathscr{K}(X)$，公式 (8) 证明了 $X/H$ 到 $\mathscr{M}(X)$ 的映射 $u \mapsto \beta_u$ 是模糊连续的，因此对于任何正测度，族 $(\beta_u)$ 是 $\lambda$-充分的$^1$ $\lambda$ 于 $X/H$，然后

$$
\lambda^\# = \int_{X/H} \beta_u\, d\lambda(u),
$$

这为$\lambda^\#$提供了新的解释。

$^1$ 在第 1 章第一版的意义上。 V，因此在第二个意义上是*更不必说*（cf.第VI, §1, No. 1章例的脚注）。

#### 命题 5 {#int-vii-s2-prop-5 .statement tag=09F7}

— 令 $\lambda$ 为$X/H$ 的正向测度。

a) 令$f$为$X$上的$\lambda^\#$可测函数，其中值位于拓扑空间中，在$\lambda^\#$可积集合的可数并之外。然后，$\dot{x} \in X/H$的集合使得函数$\xi \mapsto f(x\xi)$不是$\beta$可测量，在本地$\lambda$可以忽略不计。

b) 设$f$是$X$、零上的$\lambda^\#$可测函数$\geq 0$，位于$\lambda^\#$可积集合的可数并之外。那么，$X/H$上的函数$\dot{x} \mapsto \int^* f(x\xi) d\beta(\xi)$是$\lambda$可测的，并且

$$
\int_X^* f(x) d\lambda^\#(x) = \int_{X/H}^* d\lambda(\dot{x}) \int_H^* f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) 令$f$为$X$上的$\lambda^\#$可积函数，其中值位于Banach空间或$\overline{\mathbf{R}}$中。那么，$\dot{x} \in X/H$的集合使得$\xi \mapsto f(x\xi)$不是$\beta$可积，$\lambda$可以忽略不计； $X/H$ 上的函数 $f^b$ 几乎到处都由公式定义

$$
f^b(\dot{x}) = \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x))
$$

是$\lambda$可积，并且

$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$

和

$$
\int_{X/H} |f^b| d\lambda \leq \int_X |f| d\lambda^\#.
$$

d) 设$f$是$X$上的$\lambda^\#$可测函数，其中值位于Banach空间或$\overline{\mathbf{R}}$中，且零位于可数并之外$\lambda^\#$-可积集合。那么，对于 $f$ $\lambda^\#$ 可积，有必要且充分

$$
\int_{X/H}^* d\lambda(\dot{x}) \int_H^* |f(x\xi)| d\beta(\xi) < +\infty \quad (\dot{x} = \pi(x)).
$$

考虑到引理 2，断言 a)、b) 和 c) 可从第 1 章得出。 V, §3、提案 4、提案 5 和 Th。 1（除了（13），它是从（12）得出的，因为很明显$|f^b| \leq |f|^b$）； d) 由 b) 得出。

#### 命题 6 {#int-vii-s2-prop-6 .statement tag=09F8}

— 令 $\lambda$ 为$X/H$ 的正测度。

a) 设 $N$ 为 $X/H$ 中的子集。为了使$N$局部$\lambda$可忽略不计，$\pi^{-1}(N)$局部$\lambda^\#$可忽略不计是充分必要的。

b) 令g为X/H上的函数，其中值处于拓扑空间中。为了使 g $\lambda$ 可测，$g \circ \pi$ $\lambda^\#$ 可测是充分必要的。

c) 令h为X/H上的函数，其中值位于Banach空间或$\overline{\mathbf{R}}$中。为了使 h 局部 $\lambda$ 可积，$h \circ \pi$ 局部 $\lambda^\#$ 可积是必要且充分的，在这种情况下为 $(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#$。

假设 $h \circ \pi$ 是局部 $\lambda^\#$ 可积的。对于每个 $f \in \mathscr{K}(X)$，$f \cdot (h \circ \pi)$ 是 $\lambda^\#$ 可积，因此（命题 5）函数 $(f \cdot (h \circ \pi))^b = f^b \cdot h$ 是 $\lambda$ 可积，并且

$$
\int_{X/H} f^b \cdot h \, d\lambda = \int_X f \cdot (h \circ \pi) \, d\lambda^\#.
$$

由于$f \mapsto f^b$是$\mathscr{K}(X)$到$\mathscr{K}(X/H)$的满射映射，这表明h是局部$\lambda$可积的，并且

$$
(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#.
$$

特别是，如果$\pi^{-1}(N)$局部$\lambda^\#$可忽略，则$\varphi_N \circ \pi$局部$\lambda^\#$可忽略，因而$(\varphi_N \cdot \lambda)^\# = (\varphi_N \circ \pi) \cdot \lambda^\# = 0$，因而$\varphi_N \cdot \lambda = 0$和N局部$\lambda$可忽略。现在假设 $g \circ \pi$ 是 $\lambda^\#$ 可测的。令 K' 为 X/H 的紧凑子集。令 $f \in \mathscr{K}_+(X)$ 使得 $f^b = 1$ 在 K' 上（No. 1，命题 2），并令 $K = \operatorname{Supp} f$；一个有$\pi(K) \supset K'$。存在由 $\lambda^\#$ 可忽略不计的集合 M 和紧集的序列 $(K_n)$ 组成的 K 的划分，使得 $(g \circ \pi)|K_n$ 对于每个 n 都是连续的。那么$g|_{\pi(K_n)}$是连续的。设P为K'的点集合而不是属于到$\pi(K_1) \cup \pi(K_2) \cup \ldots$；则$\pi^{-1}(P) \cap K$包含在M中，因而$\lambda^\#$可忽略不计；因而$f \cdot \varphi_{\pi^{-1}(P)}$是$\lambda^\#$-可以忽略不计；由此可见（命题 5）：

$$
0 = \int_X f \cdot \varphi_{\pi^{-1}(P)} \, d\lambda^\# = \int_{X/H} f^b \cdot \varphi_P \, d\lambda \geq \int_{X/H}^* \varphi_P \, d\lambda,
$$

因而 P $\lambda$ 可忽略不计，g $\lambda$ 可测量。

如果 N 局部 $\lambda$ 可以忽略不计，则 $\pi^{-1}(N)$ 局部 $\lambda^\#$ 可以忽略不计（第 V, §6, No. 6 章，第 10 条命题第 1 条）。如果 g 是 $\lambda$ 可测的，则 $g \circ \pi$ 是 $\lambda^\#$ 可测的（*同上。*）。最后，假设 h 是局部 $\lambda$ 可积的。那么我们已经知道$h \circ \pi$是$\lambda^\#$可测的。对于每一个 $f \in \mathscr{K}_+(X)$，根据第 5 条命题，我们有：

$$
\int_X^* f(x)|h|(\pi(x)) \, d\lambda^\#(x) = \int_{X/H}^* |h|(u)f^b(u) \, d\lambda(u) < +\infty,
$$

因而$h \circ \pi$是局部$\lambda^\#$可积的。

#### 推论 1 {#int-vii-s2-prop-6-cor-1 .statement tag=09F9}

— 设$\lambda, \lambda'$为$X/H$的两个积极措施。为了使$\lambda'$具有基$\lambda$，${\lambda'}^\#$具有基$\lambda^\#$是充分必要的。为了使$\lambda$和$\lambda'$等价，$\lambda^\#$和${\lambda'}^\#$等价是充分必要的。

第一个断言由命题 6、a) 和 c) 得出。第二个是从第一个开始的。

#### 推论 2 {#int-vii-s2-prop-6-cor-2 .statement tag=09FA}

— 令 $\lambda$ 为 $X/H$ 的正测度，$f$ $\lambda^\#$ 可测数值函数 $X$。假设，对于每个$\xi \in H$，$\delta(\xi)f = f$局部$\lambda^\#$——几乎无处不在。那么，在$X/H$上存在$\lambda$可测量的函数$g$，使得$f = g \circ \pi$局部$\lambda^\#$-几乎无处不在。

替换$f$乘以$f/(1+|f|)$，对于$f$有界的情况，一个约化，因此局部$\lambda^\#$可积。让$\mu = f \cdot \lambda^\#$。 $f$上的假设意味着$\delta(\xi)\mu = f \cdot \delta(\xi)\lambda^\# = \Delta_H(\xi)\mu$适用于所有$\xi \in H$。那么存在（命题 4）对 $X/H$ 的测度 $\lambda'$ 使得 $\mu = {\lambda'}^\#$。由科. 1，在$X/H$上存在局部$\lambda$可积函数$g$使得$\lambda' = g \cdot \lambda$。根据第 6 号提案，$f \cdot \lambda^\# = {\lambda'}^\# = (g \circ \pi) \cdot \lambda^\#$、从而 $f = g \circ \pi$ 局部地$\lambda^\#$ - 几乎无处不在。

#### 推论 3 {#int-vii-s2-prop-6-cor-3 .statement tag=09FB}

— a) 设$(\lambda_\iota)_{\iota \in I}$为$X/H$上的实测度族。为了使族$(\lambda_\iota)$在$\mathscr{M}(X/H)$中上界，族$(\lambda_\iota^\#)$在$\mathscr{M}(X)$中上界是必要且充分的，在这种情况下

$$
\sup(\lambda_\iota^\#) = (\sup \lambda_\iota)^\#.
$$

b) 设$\lambda$为$X/H$的实测度。然后是$(\lambda^+)^\# = (\lambda^\#)^+$和$(\lambda^-)^\# = (\lambda^\#)^-$。

c) 令$\lambda$为$X/H$的复测度。然后$|\lambda|^\# = |\lambda^\#|$。

假设家庭 $(\lambda_\iota)$ 在上面有界，并设 $\mu = \sup \lambda_\iota$。由于 $\lambda \geq 0$ 蕴含 $\lambda^\# \geq 0$，因此对于所有 $\iota$，我们都有 $\mu^\# \geq \lambda_\iota^\#$，这表明族 $(\lambda_\iota^\#)$ 是有界的，并且

$$
(\sup \lambda_\iota)^\# \geq \sup(\lambda_\iota^\#).
$$

相反，假设族 $(\lambda_\iota^\#)$ 在上面有界，并设 $\nu = \sup(\lambda_\iota^\#)$。由于$\delta(\xi)\lambda_\iota^\# = \Delta_H(\xi)\lambda_\iota^\#$对于所有$\xi \in H$，显然是$\delta(\xi)\nu = \Delta_H(\xi)\nu$，因此存在一个测度$\mu' \in \mathscr{M}(X/H)$使得$\nu = {\mu'}^\#$。由于$\lambda^\# \geq 0$蕴含$\lambda \geq 0$，因此对于所有$\iota$，我们有$\mu' \geq \lambda_\iota$，这表明族$(\lambda_\iota)$在上面有界，并且$\nu = {\mu'}^\# \geq (\sup \lambda_\iota)^\#$，从而

$$
\sup(\lambda_\iota^\#) \geq (\sup \lambda_\iota)^\#,
$$

完成a)的证明。 断言 b) 然后立即跟随，因为，例如，$\lambda^+$ 正是$\sup(\lambda, 0)$。为了证明 c)，只需注意绝对值 1 的 $|\lambda| = \sup \mathscr{R}(\alpha \lambda)$ 超过复数 $\alpha$，另一方面，对于每个$\mu \in \mathscr{M}(X/H)$，$\mathscr{R}(\mu^\#) = (\mathscr{R}\mu)^\#$ 就足够了。

#### 注 1 {#int-vii-s2-n3-rem-1 .statement tag=09FC}

命题 6 a) 可以用说表示，$\lambda$ 是 $\pi$ 下 $\lambda^\#$ 的*伪图像*测度（第 VI, §3, No. 2 章，定义 1）。

#### 注 2 {#int-vii-s2-n3-rem-2 .statement tag=09FD}

假设 $H$ 是*紧凑*并且 $\beta$ 是标准化的。 $X$的每个紧凑子集的饱和度都是紧凑的。因此，如果$f \in \mathscr{K}(X/H)$则$f \circ \pi \in \mathscr{K}(X)$；并且，对于 $X/H$ 上的每个积极措施$\lambda$，提案 5 c) 给出

$$
\int_X (f \circ \pi)(x)\, d\lambda^\#(x) = \int_{X/H} f(u)\, d\lambda(u).
$$

在其他字中，$\lambda$是$\lambda^\#$在$\pi$下的*像*。

#### 注 3 {#int-vii-s2-n3-rem-3 .statement tag=09FE}

科。命题 6 的 3 c）立即表明，在复杂测量的情况下，小节的结果仍然有效（涉及上积分的除外）。

#### 注 4 {#int-vii-s2-n3-rem-4 .statement tag=09FF}

令$m$为$X/H$上的向量测度，$E$中的值，并令$q$为$E$上的下半连续半范数。为了使 $m$ 成为 $q$ 可大化（第 VI, §2, No. 3，定义 3），$m^\#$ 是这样的充分必要，在这种情况下为 $q(m^\#) = q(m)^\#$。这是从定义和 Cor 立即得出的结论。 3a）。

另一方面，令 $\mu$ 为$X/H$ 的正测度。对于 $m$ 为基 $\mu$ 的标量，$m^\#$ 为基 $\mu^\#$ 的标量是必要且充分的：这是从 Cor 得出的。 1.

最后，如果 $m$ 有基 $\mu$，其中密度 $f$ 相对于 $\mu$（第 VI, §2, No. 4，定义 4），则 $m^\#$ 有基 $\mu^\#$，其中密度 $f \circ \pi$：这是根据提案 6 c) 得出的。

### 4. $X/H$ 是仿紧的情况

如果$X/H$是仿紧的，我们首先会看到向量空间$\mathscr{K}^\chi(X)$，对于变量$\chi$来说，都是彼此同构的，特别是与$\mathscr{K}^1(X)$同构。

#### 命题 7 {#int-vii-s2-prop-7 .statement tag=09FG}

*假设 $X/H$ 准紧致。令$\chi$为$\mathbf{R}_+^*$中$H$的连续表示。*

a) *在$X$上存在连续的函数$r$，其中值$> 0$，使得$r(x\xi) = \chi(\xi)r(x)$对于所有$x \in X$和$\xi \in H$。*

b) *映射 $g \mapsto g/r$ 是向量空间 $\mathscr{K}^\chi(X)$ 中的同构到向量空间 $\mathscr{K}^1(X)$。*

让我们应用No. 1的第1条命题，将$f$取为函数$\geqslant 0$，这与任何轨道上的零不相同（这可以通过附录1中的引理1实现）；那么$r = f^\chi$满足a)的性质。 断言 b) 是显而易见的。

#### 命题 8 {#int-vii-s2-prop-8 .statement tag=09FH}

*假设 $X/H$ 准紧致。 $X$上存在连续的函数$h \geqslant 0$，其支持有紧致交，*每个紧致子集的饱和度为X，且满足$h^b = 1$。对于这样的函数，对于$X/H$上的每一个连续的函数$g$，都有$g = (h \cdot (g \circ \pi))^b$。

让我们应用No. 1和$\chi = 1$的命题1，对于$f$函数$\geqslant 0$，与任何轨道上的零不相同。我们每点 $x$ $X$ 都有$f^1(x) > 0$。 集合$h = f/f^1$。那么$h^1 = f^1/f^1 = 1$，因而$h^b = 1$。由此可见，如果$g$是$X/H$上的连续函数，则$(h \cdot (g \circ \pi))^b = h^b \cdot g = g$。

#### 注 1 {#int-vii-s2-n4-rem-1 .statement tag=09FI}

特别地，令$X$为局部紧致空间，离散的群$D$在右侧连续且正确地运行；假设 $X/D$ 是仿紧的。那么，$X$上存在连续的函数$h \geqslant 0$，其支持度为紧致交，每个紧致子集的饱和度为$X$，并且使得$\sum_{d \in D} h(xd) = 1$对于每个$x \in X$（所有项） 和是零，除了有限的数）。

#### 注 2 {#int-vii-s2-n4-rem-2 .statement tag=09FJ}

让我们保留第 8 条的假设和记号。映射 $g \mapsto h \cdot (g \circ \pi)$ 是 $\mathscr{K}(X/H)$ 到 $\mathscr{K}(X)$ 的连续映射，它是映射 $f \mapsto f^b$ 的右逆。因而，$\mathscr{K}(X/H)$的每个有界（或紧凑）子集都是$\mathscr{K}(X)$的有界（或紧凑）子集的像。由此，当这些空间配备有界（或紧凑）收敛的拓扑时，我们立即推断出映射 $\lambda \mapsto \lambda^\#$ 又是 $\mathscr{M}(X/H)$ 的同构到 $\mathscr{M}(X)$ 的闭合线性子空间。

#### 命题 9 {#int-vii-s2-prop-9 .statement tag=09FK}

— *我们保留命题 8 的假设和记号。*令 $\lambda$ 为$X/H$ 的正测度。

a) *对* $(\pi, h)$ *适合$\lambda^\#$，并且* $\int_X h(x) \varepsilon_{\pi(x)} d\lambda^\#(x) = \lambda$。

b) *映射* $\pi$ *适合测量* $h \cdot \lambda^\#$、*和* $\pi(h \cdot \lambda^\#) = \lambda$。

c) *让*$k$*成为函数在*$X/H$上，*与值在Banach空间或在*$\overline{\mathbf{R}}$中。 *对于*$k$*对于*$\lambda$来说是可测量的（分别是局部可积、本质上可积、可积），*对于*$h \cdot (k \circ \pi)$来说是必要且充分的*对于*$\lambda^\#$来说也是如此； *并且，如果* $k$ *本质上可积* $\lambda$，*则*

$$
\int_{X/H} k \, d\lambda = \int_X h \cdot (k \circ \pi) \, d\lambda^\#.
$$

让$f \in \mathscr{K}(X/H)$。然后 $h \cdot (f \circ \pi) \in \mathscr{K}(X)$ 和

$$
\int_X h(x) f(\pi(x)) d\lambda^\#(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}) \int_H h(x\xi) d\beta(\xi) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}),
$$

从而a)。 断言 b) 类似地证明。 c) 的断言涉及可测量性、基本可积性和公式 (14) 然后可以通过应用 Ch. 的结果获得。 V（§ 4、第 3 条、§ 5、第 1 条、§ 4、第 2 条）。如果 $k$ 是 $\lambda$ 可积，则 $h \cdot (k \circ \pi)$ 是 $\lambda^\#$ 可积（第 V, § 3, No. 3，第 1 章）。如果$h \cdot (k \circ \pi)$是$\lambda^\#$可积，则命题5证明$(h \cdot (k \circ \pi))^b = h^b \cdot k = k$是$\lambda$可积。如果 $k$ 是局部 $\lambda$ 可积的，那么 $h \cdot (k \circ \pi)$ 是局部 $\lambda^\#$ 可积的（命题 6）。最后，假设$h \cdot (k \circ \pi)$局部$\lambda^\#$可积；对于每个$f \in \mathscr{H}(X/H)$，$h \cdot (k \circ \pi) \cdot (f \circ \pi)$都有紧凑的支撑，并且
$$
|h \cdot (k \circ \pi) \cdot (f \circ \pi)| \leq M |h \cdot (k \circ \pi)|,
$$
其中$M = \sup |f|$；因而$h \cdot ((kf) \circ \pi)$是$\lambda^\#$可积，因而$kf$是$\lambda$可积，已被证明；这证明$k$确实是局部$\lambda$可积的。

#### 推论 {#int-vii-s2-n4-cor-1 .statement tag=09FL}

— *连续线性映射* $f \mapsto f^b$ *of* $L^1(X, \lambda^\#)$ *进入* $L^1(X/H, \lambda)$ *由第 5 条定义是满射*。

首先假设$X/H$是仿紧的，并令$h$在第8条命题的$X$满足条件上为函数。如果$k$是$X/H$上的$\lambda$可积数值函数，那么$h \cdot (k \circ \pi)$是$\lambda^\#$可积且$(h \cdot (k \circ \pi))^b = k$（命题9）。

一般情况下，设$u \in L^1(X/H, \lambda)$。 在紧集$K_n$的可数并之外，存在函数$f \in \mathscr{L}^1(X/H, \lambda)$和类$u$和零。 让我们递归地定义$X/H$的相对紧开集$U_n$的序列，使得$U_{n+1} \supset K_n \cup \overline{U}_n$，并让$V$作为$U_n$的并集。 那么$V$是$X/H$的开子集，紧致子集$\overline{U}_n$的可数并，因此是仿紧致（GT，I, § 9, No. 10，Th.5）。 集合 $Y = \overline{\pi}^{-1}(V)$ 并令$\lambda_V$（分别$\lambda_Y^\#$）为$\lambda$（分别$\lambda^\#$）在$V$（分别$Y$）上引起的测度。 很明显，$Y/H$可以与$V$识别（GT，I, § 3，命题10），并且$\lambda_Y^\#$可以与$(\lambda_V)^\#$识别。 此外，$f$是$V$之外的零以及属于至$\mathscr{L}^1(V, \lambda_V)$。 因此，存在$g \in \mathscr{L}^1(Y, \lambda_Y^\#)$使得$g^b = f$几乎在$V$中无处不在。 在$X - Y$上将$g$扩展0，得到函数$g_1 \in \mathscr{L}^1(X, \lambda^\#)$，显然$L^1(X/H, \lambda)$中$g_1^b$的类正是$u$。

#### 注 3 {#int-vii-s2-n4-rem-3 .statement tag=09FM}

— 假设$X/H$仿紧，并让我们保留命题 9的记号。$L^1(X/H, \lambda)$的映射$k \mapsto h \cdot (k \circ \pi)$进入$L^1(X, \lambda^\#)$，则与(14)*等距*，并且是映射$f \mapsto f^b$的*右逆* $L^1(X, \lambda^\#)$ 到$L^1(X/H, \lambda)$。

### 5. 齐次空间上的准不变测度

#### 引理 3 {#int-vii-s2-lem-3 .statement tag=09FN}

— *令 G 为局部紧致群，$\mu$ G 上的左 Haar 测度，$\nu$ 和 $\nu'$ G 上的两个非零的准不变测度。如果，对于每个 $s \in G$，$\gamma(s)\nu$ 相对于 $\nu$ 的密度和$\gamma(s)\nu'$*相对于$\nu'$局部相等$\mu$——几乎处处相等，则$\nu$和$\nu'$成比例。

写出$\nu = \rho \cdot \mu$、$\nu' = \rho' \cdot \mu$，其中$\rho, \rho'$是$G$上局部$\mu$可积函数，并且无处不在非零的（$§ 1$、No. 9，命题11）。对于每$s \in G$，

$$
\gamma(s)\nu = (\gamma(s)\rho) \cdot \mu, \qquad \gamma(s)\nu' = (\gamma(s)\rho') \cdot \mu,
$$

并且假设意味着$\rho^{-1} \cdot \gamma(s)\rho = {\rho'}^{-1} \cdot \gamma(s)\rho'$局部$\mu$-几乎无处不在。 集合 $\sigma = \rho'/\rho$，这是 $G$ 上的 $\mu$ 可测量的函数。对于本地的每个 $s \in G$、$\gamma(s)\sigma = \sigma$ $\mu$ - 几乎无处不在。因此，$\sigma$ 等于局部常量 $\mu$——几乎在任何地方，Cor.第 6 条提案 2 与 $X = H = G$ 一起应用。

令$G$为局部紧致群，$H$为$G$的闭子群。考虑关于 $H$ 的左陪集齐次空间 $G/H$，其中 $G$ 在左侧连续运算。我们将证明在$G/H$上存在且仅有一个非零的准不变测度类。

请注意，通过正确的翻译，$H$可以连续且正确地对$G$进行操作； 商空间，正是$G/H$，是仿紧致的（GT、III、$§ 4$、No. 6，第 13 条命题）。因此，我们可以应用第 1 至第 4 条的结果，其中$X = G$。 We thus have 映射 $f \mapsto f^b$ of $\mathscr{K}(G)$ onto $\mathscr{K}(G/H)$, and $\lambda \mapsto \lambda^\#$ of $\mathscr{M}(G/H)$ into $\mathscr{M}(G)$ (once a left Haar measure $\beta$ on $H$ has been fixed). $G$ 在 $G/H$ 中向左运算，这一事实产生了补充性质：

$$
\begin{align*}
(15) \qquad & \gamma_{G/H}(s) \cdot f^b = (\gamma_G(s) \cdot f)^b \qquad (s \in G,\ f \in \mathscr{K}(G)) \\
(16) \qquad & (\gamma_{G/H}(s) \cdot \lambda)^\# = \gamma_G(s) \cdot \lambda^\# \qquad (s \in G,\ \lambda \in \mathscr{M}(G/H)).
\end{align*}
$$

事实上，对于每 $x \in G$，

$$
(\gamma_{G/H}(s) \cdot f^b)(\pi(x)) = f^b(s^{-1}\pi(x)) = f^b(\pi(s^{-1}x))
= \int_H f(s^{-1}x\xi)\, d\beta(\xi) = \int_H (\gamma_G(s)f)(x\xi)\, d\beta(\xi) = (\gamma_G(s)f)^b(\pi(x)),
$$

从而公式 (15)，这意味着公式 (16)。

#### 引理 4 {#int-vii-s2-lem-4 .statement tag=09FO}

令$\lambda$为$G/H$上的$\neq 0$测度，$\mu$为$G$上的左哈尔测度。以下属性是等效的：
a) $\lambda$ 在 $G$ 下是准不变的；
b) for 子集 $A$ of $G/H$ to be locally $\lambda$-negligible, it is necessary and sufficient that $\overline{\pi}^{-1}(A)$ be locally $\mu$-negligible;
c) 测量$\lambda^\#$ 相当于$\mu$。

假设情况如此，令$\lambda^\# = \rho \cdot \mu$，其中$\rho$是局部$\mu$可积函数，且无处不在非零的。那么，对于每个$s \in G$，$\gamma_{G/H}(s)\lambda$相对于$\lambda$的密度$\theta_s$是这样的：

$$
\theta_s(\pi(x)) = \frac{\rho(s^{-1}x)}{\rho(x)}
$$

局部地 $\mu$ - $G$ 上几乎所有地方。

c) $\Rightarrow$ b)：这立即来自第 6 条 a) 提案。

b) $\Rightarrow$ a)：如果性质 b)成立，则$G/H$的局部$\lambda$可忽略的子集的集合在$G$下是不变的，因此$\lambda$在$G$下是准不变的。

a) $\Rightarrow$ c): 假设$\lambda$在$G$下准不变；对于每个$s \in G$，$\lambda$和$\gamma_{G/H}(s)\lambda$是等价的，因此$\lambda^\#$和$\gamma_G(s) \cdot \lambda^\# = (\gamma_{G/H}(s) \cdot \lambda)^\#$是等价的（第6号提案的Cor.1）；由于$\lambda^\# \neq 0$，$\lambda^\#$等价于$\mu$（§ 1, No. 9，提案11）。

此外，每$s \in G$，

$$
(\theta_s \circ \pi) \cdot \lambda^\# = (\theta_s \cdot \lambda)^\# = (\gamma_{G/H}(s)\lambda)^\# = \gamma_G(s)\lambda^\#
$$
$$
= (\gamma_G(s)\rho) \cdot \mu = \frac{\gamma_G(s)\rho}{\rho} \cdot \lambda^\#,
$$

从而 (17)。

a)和b)的等价意味着已经公布的第一个唯一性结果，甚至是更精确的结果：

#### 定理 1 {#int-vii-s2-thm-1 .statement tag=09FP}

*令$G$为局部紧致群，$H$为$G$的闭子群。*

a) *任意两个$G/H$上的非零的准不变测度是等价的； $G/H$中的子集对于这些措施来说局部可以忽略不计的是那些$G$中的逆像对于Haar措施而言局部可以忽略不计。*

b) *令$\lambda, \lambda'$为$G/H$上的两个非零的准不变测度。如果对于每个$s \in G$，$\gamma_{G/H}(s)\lambda$相对于$\lambda$的密度和$\gamma_{G/H}(s)\lambda'$相对于$\lambda'$的密度对于$\lambda$（或$\lambda'$）几乎处处相等，则$\lambda$和$\lambda'$成比例。*

断言 a) 立即从引理 4 得出。令 $\lambda$ 和 $\lambda'$ 为 b) 的两个非零的准不变测度满足条件。那么，对于每个$s \in G$，$\gamma_G(s)\lambda^\#$相对于$\lambda^\#$的密度和$\gamma_G(s){\lambda'}^\#$相对于${\lambda'}^\#$的密度局部相等$\mu$——几乎处处相等，因此 (引理 3) $\lambda^\#$和${\lambda'}^\#$成比例，因此$\lambda$和$\lambda'$成比例。

另一方面，引理 4 约化在 $G/H$ 上搜索非零的准不变测度相当于在 $G$ 上搜索测度

Haar 测量值为形式 $\lambda^\#$。关于这个主题，我们有以下引理：

#### 引理 5 {#int-vii-s2-lem-5 .statement tag=09FQ}

*令$\mu$为$G$的左哈尔测度，$\rho$为局部$\mu$可积函数。对于 $\rho \cdot \mu$ 为形式 $\lambda^\#$，对于每个 $\xi \in H$，* 是充分必要的

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*局部地$\mu$-几乎所有$G$。*

说$\rho \cdot \mu$等于形式$\lambda^\#$等于说，对于每一个$\xi \in H$，$\delta(\xi)(\rho \cdot \mu) = \Delta_H(\xi)\rho \cdot \mu$（命题4）。现在，

$$
\delta(\xi)(\rho \cdot \mu) = (\delta(\xi)\rho) \cdot (\delta(\xi)\mu) = \Delta_G(\xi)(\delta(\xi)\rho) \cdot \mu,
$$

从而引理。

我们现在可以确定已公布的存在结果，甚至是更精确的结果：

#### 定理 2 {#int-vii-s2-thm-2 .statement tag=09FR}

*令$G$为局部紧凑群，$H$为$G$的闭子群，$\mu$为$G$的左哈尔测度，$\beta$为$H$的左哈尔测度。

a) *在$G$上存在函数$\rho$连续且$> 0$，使得*

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*对于所有*$x \in G$*和*$\xi \in H$。

b) *给定这样的函数$\rho$，可以在*$G/H$*上形式测度*$\lambda = (\rho \cdot \mu)/\beta$*，并且*$\lambda$*是非零的在*$G$下准不变的正测度。

c) *对于* $s, x$ *在* $G$、$\rho(sx)/\rho(x)$ *仅取决于* $s$ *和* $\pi(x)$，*因此定义函数* $\chi$ *连续且* $> 0$ *on* $G \times (G/H)$ *这样*

$$
\chi(s, \pi(x)) = \frac{\rho(sx)}{\rho(x)}.
$$

*然后*

$$
\gamma_{G/H}(s)\lambda = \chi(s^{-1}, .) \cdot \lambda \quad \text{for all } s \in G.
$$

a) 由命题 7 得出。
b) 由引理 5 和 4 得出。
c) 由(17)得出。

#### 注 1 {#int-vii-s2-n5-rem-1 .statement tag=09FS}

从 No. 3 的注 1 推断，G/H 上的非零的准不变测度正是 G 上 Haar 测度$\pi$ 下的伪像。

#### 注 2 {#int-vii-s2-n5-rem-2 .statement tag=09FT}

如果G是李群，我们稍后会看到Th的函数$\rho$。 2 可以选择为无限可微。*

Th 条件以下。 2、第 3 条和第 4 条的某些结果可以具体化如下（考虑到第 V, §4、第 2 章和经过的提案 2，从相对于 $\mu$ 的属性到相对于 $\rho \cdot \mu$ 的属性）：

a) 令$f$为G上的$\mu$可测函数，其中值位于拓扑空间中，在$\mu$可积集合的可数并之外；那么，$\dot{x} \in G/H$的集合使得函数$\xi \mapsto f(x\xi)$不是$\beta$可测量，在本地$\lambda$可以忽略不计。

b) 令$f$为G上的$\mu$可测函数$\geqslant 0$，零位于$\mu$可积集合的可数并之外。然后，函数
$$
\dot{x} \mapsto \int_{H}^{*} f(x\xi) d\beta(\xi)
$$
$G/H$ 是$\lambda$-可测的，并且
$$
\int_{G}^{*} f(x)\rho(x) d\mu(x) = \int_{G/H}^{*} d\lambda(\dot{x}) \int_{H}^{*} f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) 令$f$为G上的$\rho \cdot \mu$可积函数，其中值位于Banach空间或$\overline{\mathbf{R}}$中。那么，$\dot{x} \in G/H$的集合使得$\xi \mapsto f(x\xi)$不是$\beta$可积，$\lambda$可以忽略不计； 函数 $\dot{x} \mapsto \int_{H} f(x\xi) d\beta(\xi)$ 是 $\lambda$ 可积，并且
$$
\int_{G} f(x)\rho(x) d\mu(x) = \int_{G/H} d\lambda(\dot{x}) \int_{H} f(x\xi) d\beta(\xi).
$$

d) G 上存在连续的函数 $h \geqslant 0$，其支撑有紧交，G 的每个紧子集 K 的饱和度为 KH，并且对于每个 $x \in G$ 都有 $\int_{H} h(x\xi) d\beta(\xi) = 1$。为了使 G/H 上的函数 g 对于 $\lambda$ 可测量（分别是局部可积、本质上可积、可积），$h \cdot (g \circ \pi)$ 对于 $\rho \cdot \mu = \lambda^{\sharp}$ 来说是必要且充分的；并且，当 g 对于 $\lambda$ 基本上可积时，有
$$
\int_{G/H} g(u) d\lambda(u) = \int_{G} h(x)g(\pi(x)) \rho(x) d\mu(x).
$$

### 6. 同质空间上的相对不变的度量

再次令 G 为局部紧致群，H 为闭子群，$\beta$ H 上的左 Haar 测度。

#### 引理 6 {#int-vii-s2-lem-6 .statement tag=09FU}

令$\lambda$为$G/H$的测度，$\chi$为G在$\mathbf{C}^*$中的连续表示。以下属性是等效的：
a) $\lambda$ 对 $G/H$ 与乘子 $\chi$ 相对不变；
b) $\lambda^\#$ 在 G 上相对不变，左乘子 $\chi$；
c) $\lambda^\#$ 为形式 $a \chi \cdot \mu$ ($a \in \mathbf{C}$)。

条件 a) 意味着，对于每个 $s \in G$，

$$
\gamma_{G/H}(s)\lambda = \chi(s)^{-1}\lambda;
$$

这相当于 $(\gamma_{G/H}(s)\lambda)^\# = \chi(s)^{-1}\lambda^\#$，即

$$
\gamma_G(s)\lambda^\# = \chi(s)^{-1}\lambda^\#.
$$

a) 和 b) 的从而等价。 b) 和 c) 的等价源自 §1, No. 8，Cor。提案 10 中的 1 条。

#### 定理 3 {#int-vii-s2-thm-3 .statement tag=09FV}

令 G 为局部紧致群，H 为 G 的闭子群，$\mu$（或 $\beta$）G 上的左 Haar 测度（或 H），$\chi$ G 在 $\mathbf{C}^*$ 中的连续表示。

a) 在阶中，在G下存在$G/H$非零的测度相对不变，并且对于乘子$\chi$，$\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)$对于所有$\xi \in H$是充分必要的。

b) 该度量在常数因子范围内是唯一的；更准确地说，它与$(\chi \cdot \mu)/\beta$成正比。

为了在G下存在$G/H$非零的测度与乘子$\chi$相对不变，$\chi \cdot \mu$是形式$\lambda^\#$是充分必要的（引理6），因此（No. 2，命题4） $\delta(\xi)(\chi \cdot \mu) = \Delta_H(\xi)(\chi \cdot \mu)$ 对于所有$\xi \in H$。这个条件也可以写成$\chi(\xi)\chi \cdot \Delta_G(\xi)\mu = \Delta_H(\xi)\chi \cdot \mu$，即

$$
\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)
$$

对于所有$\xi \in H$。 从而a)。 断言 b) 立即从引理 6 得出，并且映射 $\lambda \mapsto \lambda^\#$ 是单射的。

我们将在§3（No. 3，例 4）中看到一些非常简单的例，其中表示$\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$不能扩展到$\mathbf{C}^*$中G的连续表示。因而，在这种情况下，在 G 下不存在任何关于 $G/H$ 相对不变的非零的复测度。

#### 推论 1 {#int-vii-s2-thm-3-cor-1 .statement tag=09FW}

为了在G下$G/H$非零的存在相对不变的正测度，在$\mathbf{R}_+^*$中存在$G$的连续表示延伸表示$\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$是充分必要的。

请注意，当$H$是幺模时，条件成立。

#### 推论 2 {#int-vii-s2-thm-3-cor-2 .statement tag=09FX}

— 为了在 $G$ 下存在$G/H$ 非零的正测度不变量，$\Delta_G$ 重合与 $\Delta_H$ 在$H$ 上是必要且充分的。

#### 推论 3 {#int-vii-s2-thm-3-cor-3 .statement tag=09FY}

— 假设 $H$ 是幺模的，并且$G/H$ 非零的上存在有界正测度 $\nu$ 在 $G$ 下相对不变。那么$\nu$是不变的，$G$是幺模的。

设$\chi$为$\nu$的乘子。对于每个$s \in G$，$\nu$和$\gamma(s)\nu$具有相同的有限总质量（§ 1, No. 1，公式（6））；从$\gamma(s)\nu = \chi(s)^{-1}\nu$开始，我们有$\chi(s) = 1$。因而$\nu$是不变的。由科. 2、$\Delta_G(s) = 1$为所有$s \in H$。令$G'$为$t \in G$的集合，使得$\Delta_G(t) = 1$。这是 $G$ 包含 $H$ 的闭合法线子群。令$\pi$为$G/H$的典范映射到$G/G'$。那么$\pi(\nu)$就是非零的，在$G$下有界正测度不变量。因此群 $G/G'$ 的左 Haar 测度是有界的，因而 $G/G'$ 是紧致的（§ 1, No. 2，命题 2）。因而，$\Delta_G$下的$G$的像是$\mathbf{R}_+^*$的紧凑子群；这个子群减少到$\{1\}$，因而$\Delta_G = 1$在所有$G$上。

### 7. Haar 测量商群

#### 命题 10 {#int-vii-s2-prop-10 .statement tag=09FZ}

— 令 $G$ 为局部紧凑群，$G'$ 子群，$G''$ 群 $G/G'$，$\pi$ 典范映射 $G$ 到$G/G'$和$\alpha, \alpha', \alpha''$在$G, G', G''$上留下了哈尔措施。

a) 如果需要，将$\alpha$乘以常数因子，我们可以假设$\alpha'' = \alpha/\alpha'$。特别是，如果 $f \in \mathscr{K}(G)$ 那么

$$
\int_G f(x)\,d\alpha(x) = \int_{G''} d\alpha''(\dot{x}) \int_{G'} f(x\xi)\,d\alpha'(\xi) \quad (\dot{x} = \pi(x)).
$$

b) 对于所有$\xi \in G'$，一个人有$\Delta_G(\xi) = \Delta_{G'}(\xi)$；特别是，如果 $G$ 是幺模的，那么 $G'$ 也是幺模的。

c) $\mathbf{R}_+^*$ 中$G$的表示$\Delta_G$的核是$G$的最大幺模闭正规子群。

应用Th。 No. 6与$\chi = 1$的3（并且知道这里存在$G$下$G/G'$不变量的测度，即$\alpha''$），我们得到a）和b）； c)紧随b)而来。

#### 命题 11 {#int-vii-s2-prop-11 .statement tag=09G0}

— 我们维持命题 10 的记号。令 $u$ 为 $G$ 的自同构，使得 $u(G') = G'$。设$u'$为$u$到$G'$的限制，并且从$u$通过商推导出$G''$的$u''$自同构。然后

$$
\operatorname{mod}_G(u) = \operatorname{mod}_{G'}(u') \operatorname{mod}_{G''}(u'').
$$

因为，如果$\alpha'' = \alpha/\alpha'$则$u''(\alpha'') = u(\alpha)/u'(\alpha')$，即
$$
\operatorname{mod}_{G''}(u'')^{-1}\alpha'' = \operatorname{mod}_G(u)^{-1}\alpha/\operatorname{mod}_{G'}(u')^{-1}\alpha'
$$
$$
= \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} (\alpha/\alpha') = \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} \alpha'',
$$
从而命题。

#### 推论 {#int-vii-s2-n7-cor-1 .statement tag=09G1}

— *对于每个* $x \in G$，
$$
\Delta_G(x) = \Delta_{G/G'}(\dot{x}) \operatorname{mod}(i_x),
$$
*其中*$\dot{x}$*表示*$x$*中*$G/G'$的典范像，*和*$i_x$*自同构*$s \mapsto x^{-1}sx$*$G'$。

这是从第 11 条命题和 §1, No. 4 的公式 (33) 得出的。

### 8. 传递性性质

令 $X$ 为局部紧致空间，其中局部紧致群 $H$ 通过 $(x, \xi) \mapsto x\xi$ ($x \in X,\ \xi \in H$) 连续且*正确地*作用于右侧。 令$H'$为$H$的闭子群；那么$H'$在$X$的右侧连续且*正确地*运行。 我们用$\pi, \pi', p$表示$X$到$X/H$、$X$到$X/H'$以及$H$到$H/H'$的规范映射。

设$\beta, \beta'$为$H, H'$的左哈尔测度；假设 $\Delta_H$ 和 $\Delta_{H'}$ *重合在* $H'$ 上；然后可以对$H/H'$进行形式测度$\beta/\beta'$，在$H$下保持左不变（No. 6，Th.3）。另一方面，令 $\mu$ 为 $X$ 的正测度，使得
$$
\delta(\xi)\mu = \Delta_H(\xi)\mu
$$
对于$\xi \in H$；然后可以对$X/H$采取形式措施$\mu/\beta$，对$X/H'$实施$\mu/\beta'$（No. 2，提案4）。我们将把$\mu/\beta'$写为$\mu/\beta$的*整的*，由$X/H$的点索引的$X/H'$度量系列。当$H' = \{e\}$时，我们又会陷入No. 3的境地。

$X \times H$到$X/H'$的映射$(x, \xi) \mapsto \pi'(x\xi)$是连续的；由于$\pi'(x\xi) = \pi'(x\xi\xi')$对于所有$\xi' \in H'$这个映射定义，通过到商，$X \times (H/H')$的*连续*映射进入$X/H'$； 从而，对于$X$中的每个固定$x$，$H/H'$的部分映射$\omega_x$进入$X/H'$，通过从H的映射$\psi_x : \xi \mapsto x\xi$到商推导出来X。请注意，$\psi_{x\xi} = \psi_x \circ \gamma_H(\xi)$，因此对于所有$\xi \in H$，$\omega_{x\xi} = \omega_x \circ \gamma_{H/H'}(\xi)$。

#### 引理 7 {#int-vii-s2-lem-7 .statement tag=09G2}

*令K为X/H'的紧致子集，且L为X的紧致子集。那么 $\bigcup_{x \in L} \omega_x^{-1}(K)$ 在 H/H'._ 中是相对紧凑的

令 $K_1$ 为 X 的紧致子集，使得 $\pi'(K_1) = K$。令$K_2$为$\xi \in H$的集合，使得$L\xi$与$K_1$相交。那么 $K_2$ 是紧致的（GT，III, §4, No. 5，Th.1）。令$\xi \in H$ 使得$p(\xi) \in \bigcup_{x \in L} \omega_x^{-1}(K)$。因此，存在一个$x \in L$使得$\omega_x(p(\xi)) \in K$，在其他字使得$\pi'(x\xi) \in K$。由于$\pi'(K_1) = K$，存在$\xi' \in H'$使得$x\xi\xi' \in K_1$。那么$\xi\xi' \in K_2$，因此$p(\xi) = p(\xi\xi') \in p(K_2)$。因此我们证明了$\bigcup_{x \in L} \omega_x^{-1}(K) \subset p(K_2)$。

这个引理首先表明映射$\omega_x$是*正确的*。因而，可以在 $X/H'$ 上进行形式测量$\omega_x(\beta/\beta')$，该措施集中在$\omega_x(H/H') = \pi'(\psi_x(H)) = \pi'(xH)$。若$f \in \mathscr{K}(X/H')$、引理7和§1, No. 1、引理1则表明函数$x \mapsto \langle f, \omega_x(\beta/\beta') \rangle$在X上连续；此外，当Supp $f$ 不与$\pi'(xH)$ 相交时，$\langle f, \omega_x(\beta/\beta') \rangle$ 为零，在其他字中，当$\pi(x)$ 不与$X/H$ 中Supp $f$ 的属于到典范像时。

此外，如果 $x \in H$ 那么

$$
\omega_{x\xi}(\beta/\beta') = \omega_x(\gamma_{H/H'}(\xi)(\beta/\beta')) = \omega_x(\beta/\beta').
$$

X的映射$x \mapsto \omega_x(\beta/\beta')$进入$\mathscr{M}(X/H')$，因此定义通过商映射$u \mapsto (\beta/\beta')_u$从$X/H$进入$\mathscr{M}(X/H')$。上式表明，对于每个 $f \in \mathscr{K}(X/H')$，映射 $u \mapsto \langle f, (\beta/\beta')_u \rangle$ 是连续的且有紧支撑。因而，映射 $u \mapsto (\beta/\beta')_u$ *是一个模糊连续且* $(\mu/\beta)$*-关于* $X/H'$，*与* $X/H$ *作为指标集合* 的充分措施族。

设$x \in X$和$u = \pi(x) \in X/H$。令$f$为$X/H'$上的函数，其中值位于Banach空间或$\overline{\mathbf{R}}$中。由 Ch. V, §4，Th。 2、要使 $f$ $(\beta/\beta')_u$ 可积，$H/H'$ 上的函数 $p(\xi) \mapsto f(\omega_x(p(\xi))) = f(\pi'(x\xi))$ $(\beta/\beta')$ 可积是充分必要的，在这种情况下

$$
(21) \quad \int_{X/H'} f(u') d(\beta/\beta')_u(u') = \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}) \qquad (\dot{\xi} = p(\xi)).
$$

可测性、上积分和本质积分具有类似的性质。

#### 命题 12 {#int-vii-s2-prop-12 .statement tag=09G3}

— *根据上述记号*，

$$
\int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u) = \mu/\beta'.
$$

设$f \in \mathscr{K}(X)$，并设$f^b \in \mathscr{K}(X/H')$，定义为

$$
f^b(\pi'(x)) = \int_{H'} f(x\xi') d\beta'(\xi').
$$

(cf.No. 2)足以证明$f^b$对于(22)的两个成员具有相同的积分。现在，$\langle \mu/\beta', f^b \rangle = \langle \mu, f \rangle$。另一方面，

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} \langle (\beta/\beta')_u, f^b \rangle d(\mu/\beta)(u).
$$

现在，让$x \in X$和$u = \pi(x)$。我们有

$$
\langle (\beta/\beta')_u, f^b \rangle = \langle \omega_x(\beta/\beta'), f^b \rangle = \int_{H/H'} f^b(\omega_x(\dot{\xi})) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} f^b(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} d(\beta/\beta')(\dot{\xi}) \int_{H'} f(x\xi\xi') d\beta'(\xi')
$$
$$
= \int_H f(x\xi) d\beta(\xi).
$$

因而

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} d(\mu/\beta)(u) \int_H f(x\xi) d\beta(\xi) = \langle \mu, f \rangle,
$$

这就证明了命题。

#### 推论 1 {#int-vii-s2-prop-12-cor-1 .statement tag=09G4}

— a) *设 f 为 X/H' 上的函数，其中值在 Banach 空间或$\overline{\mathbf{R}}$ 中，可积为 $\mu/\beta'$。存在X/H 的可忽略的$(\mu/\beta)$子集 N，具有以下性质：如果$x \in X$使得$\pi(x) \notin N$，则函数$f \circ \omega_x$在H/H'上，即函数$\dot{\xi} \mapsto f(\pi'(x\xi))$，对于 $\beta/\beta'$ 可积。整的$\int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})$仅取决于$\dot{x} = \pi(x)$，并且是$\dot{x}$的$(\mu/\beta)$可积函数；和*

$$
\int_{X/H'} f d(\mu/\beta') = \int_{X/H} d(\mu/\beta)(\dot{x}) \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

b) 令$f$为$X/H'$上的函数$\geq 0$，可在$(\mu/\beta')$可积集合的可数并之外测量$\mu/\beta'$和零。然后

$$
\pi(x) \mapsto \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$

$(\mu/\beta)$-可测量，并且

$$
\int_{X/H'}^* f d(\mu/\beta') = \int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

c) 设$f$为$X/H'$上的函数，值位于Banach空间或$\overline{\mathbf{R}}$中，可在$(\mu/\beta')$可积的可数并之外测量$\mu/\beta'$和零集合。那么，对于 $f$ $(\mu/\beta')$ 可积，满足以下条件就足够了

$$
\int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* |f(\pi'(x\xi))| d(\beta/\beta')(\dot{\xi}) < +\infty.
$$

#### 推论 2 {#int-vii-s2-prop-12-cor-2 .statement tag=09G5}

— 令$G$为群、$A$和$B$闭子群的$G$，使得$A \supset B$。假设在关于$B$的左陪集的齐次空间$G/B$上，存在非零的正测度$\alpha$，它在$G$下不变并且有界。

a) $G/A$中$\alpha$的典范像是非零的正测度，在$G$下不变，并且有界。

b) $\Delta_G$ 重合，$\Delta_A$ 位于 $A$，$\Delta_B$ 位于 $B$。

c) 在$A$关于$B$的左陪集的齐次空间$A/B$上，存在$A$下且有界的非零的正测度不变量。

断言a) 是直接的。 断言 b) 由 a) 和 No. 6 得出，Cor. 2 Th。 3. 通过b)，$\Delta_A$重合与$\Delta_B$在$B$上，因此可以将当前小节的结果应用于取$X = G$、$H = A$、$H' = B$。 $G/B$ 上的函数 1 是$\alpha$ 可积的。通过Cor的a）。 1、$A/B$上的函数1对于$\beta/\beta'$可积，其中$\beta$和$\beta'$表示$A$和$B$上的左哈尔测度；因此 $\beta/\beta'$ 是有界的。

### 9. 构造群的 Haar 度量来自某些子群的 Haar 度量

令$G$是群、$X$和$Y$两个$G$的闭子群，使得$\Omega = XY$包含是$e$的邻域$U$。那么$\Omega$在$G$开放；对于任何$x_0 \in X$和$y_0 \in Y$，$XY = (x_0X)(Yy_0) \supset x_0Uy_0$和$x_0 U y_0$是$x_0 y_0$的邻域；因此$\Omega$是其每个点的邻域。

*当G为李群且李代数$g$时，条件强加于X，且若子代数相应的至X且Y有和$g$，则满足Y。*

群$X \times Y$在左侧G中连续运行，经过律$(x, y) \cdot s = x s y^{-1}$（$x \in X, y \in Y, s \in G$）。让$Z = X \cap Y$。 $X \times Y$中e的稳定子是对$(z, z)$形成的$X \times Y$的子群$Z_0$，其中$z \in Z$、子群与$Z$自然同构。因此集合 $\Omega$ 可以与左陪集的齐次空间 $(X \times Y)/Z_0$ 等同；更准确地说，将$X \times Y$的映射$(x, y) \mapsto xy^{-1}$转移到$\Omega$定义，通过商，将$(X \times Y)/Z_0$的连续双射转移到$\Omega$。我们假设这个映射 *是同胚*。 （如果 G 在无穷大可数，则尤其如此：cf. App.I。）

#### 命题 13 {#int-vii-s2-prop-13 .statement tag=09G6}

— *假设在加法中 Z 是紧致的。令$\mu_G, \mu_X, \mu_Y$为G、X、Y、$\Delta_G$到Y的$\Lambda$限制的左哈尔测度。则$\mu_G$到$\Omega$的限制$\mu$为，直到一个常数因子、$\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$的像在$X \times Y$的映射$(x, y) \mapsto xy^{-1}$到$\Omega$（映射是正确的）。

对于$x \in X, y \in Y$，

$$
\gamma((x, y)) \mu = \delta(y) \gamma(x) \mu = \Delta_G(y) \mu .
$$

将$\Omega$与齐次空间$(X \times Y)/Z_0$识别，并在$Z_0$上选择合适的Haar测度，可以看到$\mu^\#$是$X \times Y$的左Haar测度的乘积，即$\mu_X \otimes \mu_Y$除以函数$(x, y) \mapsto \Delta_G(y)^{-1}$ （No. 6，引理6）。另一方面，$\mu$是，直到常数因子，$\mu^\#$的像在$X \times Y$的典范映射到$\Omega$上（No. 3，注2）。

#### 推论 {#int-vii-s2-n9-cor-1 .statement tag=09G7}

— *令 f 为 $\Omega$ 上定义的函数，其中值在 Banach 空间或$\overline{\mathbf{R}}$ 中。为了使 f $\mu$ 可积，函数 $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ $(\mu_X \otimes \mu_Y)$ 可积是必要且充分的，在这种情况下*

$$
\int_\Omega f(\omega) d\mu(\omega) = a \iint_{X \times Y} f(xy) \Delta_G(y) \Delta_Y(y)^{-1} d\mu_X(x) d\mu_Y(y),
$$

其中 $a$ 是与 f 无关的常数 $> 0$。

根据第 13 号提案和第 13 章V, §4, No. 4，周四。 2、对于 f $\mu$ 可积，函数 $(x, y) \mapsto f(xy^{-1})$ 对于 $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$ 可积，或者函数 $(x, y) \mapsto f(xy^{-1}) \Delta_G(y)^{-1}$ 对于 $\mu_X \otimes \mu_Y$ 可积，或者函数 $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ 是充分必要的可积 $\mu_X \otimes \mu_Y$。 公式 (23) 由类似的论证得出。

#### 命题 14 {#int-vii-s2-prop-14 .statement tag=09G8}

— 假设命题13的条件成立，并且在加法中，Y是正规的。

a) $\mu_G$ 到 $\Omega$ 的限制，直到常数因子，在$X \times Y$ 的映射 $(x, y) \mapsto xy$ 到$\Omega$ 下，$\mu_X \otimes \mu_Y$ 的像。

b) 对于 $x \in X$ 和 $y \in Y$，

$$
\Delta_G(xy) = \Delta_X(x)\Delta_Y(y) \operatorname{mod}(i_x),
$$

其中 $i_x$ 表示 Y 的自同构 $v \mapsto x^{-1}vx$。

我们在 Y 上有 $\Delta_G = \Delta_Y$（命题 10 b）），因此从 (23) 可以得出 a)。让$x_0 \in X,\ y_0 \in Y$。用$X \times Y$的$p$映射$(x, y) \mapsto xy$到$\Omega$表示。自从

$$
xy(x_0y_0)^{-1} = xx_0^{-1}(x_0yy_0^{-1}x_0^{-1}) = xx_0^{-1}i_{x_0^{-1}}(yy_0^{-1}),
$$

我们有

$$
\begin{align*}
\Delta_G(x_0y_0)p(\mu_X \otimes \mu_Y) &= \delta(x_0y_0)p(\mu_X \otimes \mu_Y) \\
&= p(\delta(x_0)\mu_X \otimes i_{x_0^{-1}}\delta(y_0)\mu_Y) \\
&= p(\Delta_X(x_0)\mu_X \otimes \Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})\mu_Y) \\
&= \Delta_X(x_0)\Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})p(\mu_X \otimes \mu_Y),
\end{align*}
$$

从而b)。

#### 注 {#int-vii-s2-n9-rem-1 .statement tag=09G9}

当 G 是 X 与 Y 的拓扑半直接乘积（GT，III, §2, No. 10）时，命题 14 特别适用。在这种情况下，$Z = \{e\}$和$\Omega = G$。由于$yx = xi_x(y)$对于$x \in X,\ y \in Y$，测量$\mu_G$也是，直到常数因子，$(\operatorname{mod}\ i_x)\mu_X \otimes \mu_Y$的像在$X \times Y$的映射$(x, y) \mapsto yx$下进入G。

### 10. 基本领域的集成

令X为局部紧致空间，H为在X中连续且正确地在右侧运行的离散群。设$\pi$是$X/H$上X的典范映射。对于每个$x \in X$，我们用H中的$x$的$H_x$稳定子来表示；这是 H 的有限子群（GT，III, §4, No. 2，命题 4）；它的阶将表示为$n(x)$。对于每个$s \in H,\ H_{xs} = s^{-1}H_x s$，因此$n(xs) = n(x)$。存在 x 的开邻域 U，使得 $U \cap Us = \varnothing$ 对于 $s \notin H_x$（前述第 8 条命题的No. 4、证明）；对于$y \in U$，一个人有$H_y \subset H_x$；因此函数$n$在X上是上半连续的。当X在无穷大可数时，H是可数的；例如，令$(K_1, K_2, \ldots)$为紧致子集的序列覆盖X，并令$x_0 \in X$； $s \in H$的集合，使得$x_0 s \in K_i$是有限的（*loc.cit.*，No. 5，Th.1），从而我们的断言。

#### 定义 2 {#int-vii-s2-def-2 .statement tag=09GA}

*设$F \subset X$。有人说$F$是一个基本域（对于$H$），如果$\pi$到$F$的限制是$F$到$X/H$*的双射（在其他字，$F$是代表*系统*）对于 $H$ 定义的等价关系）。

#### 引理 8 {#int-vii-s2-lem-8 .statement tag=09GB}

— *令 $F$ 为基本域。对于每 $x \in X$，*
$$
\sum_{s \in H} \varphi_{Fs}(x) = n(x).
$$
(24)

由于$\varphi_{Fs}(xt) = \varphi_{Fst^{-1}}(x)$对于$H$中的所有$s$和$t$，当$x$被$xt$替换时，(24)的两个成员保持不变。因此我们可以假设$x \in F$。那么我们就有等价
$$
\varphi_{Fs}(x) = 1 \iff x \in Fs \iff xs^{-1} \in F \iff xs^{-1} = x \iff s \in H_x,
$$
从而 (24)。

#### 命题 15 {#int-vii-s2-prop-15 .statement tag=09GC}

*假设$X$在无穷大处是可数的。令 $\mu$ 为 $X$ 上的$\geq 0$ 测度。令$F$为基本域，使得对于每个$s \in H$，$Fs$是$\mu$可测的。设$f$是$X$上的$\mu$可积函数，值在Banach空间或$\overline{\mathbf{R}}$中。然后是*的家人
$$
\int_{Fs} n(x)^{-1} f(x) d\mu(x) \qquad (s \in H)
$$
*是可求和的，并且*
$$
\int_X f(x) d\mu(x) = \sum_{s \in H} \int_{Fs} n(x)^{-1} f(x) d\mu(x).
$$

如果$A$是$H$的有限子集，那么
$$
\left| \sum_{s \in A} n^{-1} f \varphi_{Fs} \right| \leq n^{-1} |f| \sum_{s \in A} \varphi_{Fs} \leq |f|
$$
由引理 8。引理 8 还证明$\sum_{s \in A} n^{-1} f \varphi_{Fs}$相对于$H$的有限子集的递增有向集合逐点收敛于$f$。提案 15 是从第 1 章得出的。 IV, §4, No. 3，Th。 2.

#### 定理 4 {#int-vii-s2-thm-4 .statement tag=09GD}

*令$X$为无穷大可数的局部紧致空间，$H$为离散群，在$X$、X的π典范映射右侧连续且适当地运行到X/H，μ为H、β下X不变性的正测度H 的归一化 Haar 度量，且 λ = μ/β。令 F 为 μ 可测基本域。

a) 对 $(\pi, n^{-1}\varphi_F)$ 是 μ 适应的，并且

$$
\int_X n(x)^{-1} \varphi_F(x) \varepsilon_{\pi(x)} \, d\mu(x) = \lambda.
$$

b) 映射 π 适用于 $n^{-1}\varphi_F \cdot \mu$ 和 $\pi(n^{-1}\varphi_F \cdot \mu) = \lambda$。

c) 令 k 为 X/H 上的函数。为了使 k 为 λ 可测（或 λ 可积），$n^{-1}\varphi_F(k \circ \pi)$ 为 μ 可测（或 μ 可积）是必要且充分的；并且，如果 k 是 λ 可积的，那么

$$
\int_{X/H} k \, d\lambda = \int_F n^{-1}(k \circ \pi) \, d\mu.
$$

我们有$\mu = \lambda^\sharp$。让$f \in \mathscr{H}_+(X/H)$。那么 $n^{-1}\varphi_F(f \circ \pi)$ 是 μ 可测的，$\geq 0$，根据 No. 3 的命题 5 b)，我们有

$$
\int_X^* n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H}^* f(\dot{x}) d\lambda(\dot{x}) \int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi)
$$

$\int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi) = n(x)^{-1} \sum_{\xi \in H} \varphi_F(x\xi) = 1$乘以引理 8。因此$n^{-1}\varphi_F \cdot (f \circ \pi)$是μ可积的并且

$$
\int_X n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}).
$$

这就证明了a）。 断言 b) 类似地证明。 断言 c) 可以从 a) 和 Ch. 推导出来。 V, §4，提案 3 和 Th。 2.

#### 推论 {#int-vii-s2-n10-cor-1 .statement tag=09GE}

— 我们维持 Th 的假设和记号。 4. 令F'为第二μ可测基本域。设 u 在 X 上为函数，值在 Banach 空间或$\overline{\mathbf{R}}$ 中，在 H 下不变。假设 u 在 F 上可 μ 可积。则 u 在 F' 上可 μ 可积，并且

$$
\int_F u(x) d\mu(x) = \int_{F'} u(x) d\mu(x).
$$

由于 u 和 n 在 H 下不变，因此在 X/H 上存在函数 v，使得 v o π 重合且 nu 在 F 和 F' 上。那么$n^{-1} \varphi_F(v \circ \pi) = \varphi_{F'} u, \quad n^{-1} \varphi_{F'}(v \circ \pi) = \varphi_{F'} u.$到假设，$n^{-1} \varphi_F(v \circ \pi)$是$\mu$可积的。由 Th. 4、 $v$ $\lambda$ 可积， $\varphi_{F'} \mu$ $\mu$ 可积，并且

$$
\int_F u d\mu = \int_{X/H} v d\lambda = \int_{F'} u d\mu.
$$

对于 $\mu$ 可测基本域的存在性，请参阅 Exer。 12.

### 习题 {#int-vii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
