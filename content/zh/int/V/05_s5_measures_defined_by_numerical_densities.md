---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 5
section_title: Measures defined by numerical densities
lang: zh
source: int-i-vi
book_pages: INT V.38-INT V.62, INT V.99-INT V.107
pdf_pages: 0293-0317, 0354-0362
extraction: ocr
subsections:
    - "no": 1
      title: Locally integrable functions
      page: 38
      pdf_page: 293
    - "no": 2
      title: Measures defined by numerical densities
      page: 40
      pdf_page: 295
    - "no": 3
      title: Integration with respect to a measure defined by a density
      page: 42
      pdf_page: 297
    - "no": 4
      title: Behavior of the product with respect to the usual operations
      page: 45
      pdf_page: 300
    - "no": 5
      title: Characterization of measures with base $\mu$
      page: 48
      pdf_page: 303
    - "no": 6
      title: Equivalent measures
      page: 52
      pdf_page: 307
    - "no": 7
      title: Alien measures
      page: 54
      pdf_page: 309
    - "no": 8
      title: 'Applications: I. Duality of the spaces $L^p$'
      page: 56
      pdf_page: 311
    - "no": 9
      title: 'Applications: II. Functions of measures'
      page: 60
      pdf_page: 315
    - "no": 10
      title: Diffuse measures; atomic measures
      page: 61
      pdf_page: 316
statements: 52
exercises: 31
content_sha256: fc7405a59f10bf7d8ef75e8872b045a9db8402fc42f05c0813f0c05fe8365d6c
translated_from: content/en/int/V/05_s5_measures_defined_by_numerical_densities.md
translation_method: google
source_content_sha256: d1c0e47776f33ebac3f5f4eb44ad8e2e1b76c65670899f2de059c9d70818f487
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 42570adcf8eed1333d6ac01bccf85458378e3caa4904846e8281f32f956a439f
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 5。由数值密度定义的度量

### 1. 本地可积函数

#### 命题 1 {#int-v-s5-prop-1 .statement tag=092D}

*让 g 被定义为函数，几乎在 T 中的任何地方（对于正测度 $\mu$），值在 Banach 空间 F 中（分别在 $\overline{\mathbf{R}}$ 中）。以下属性是等效的：*

a) *对于每个点 $t \in T$，存在 t 的邻域 V，使得函数 $g \varphi_V$ 是 $\mu$ 可积。*

b) *函数 g 是 $\mu$ 可测量的，对于每个紧集 $K \subset T$，$\int^* |g|\varphi_K\,d\mu < +\infty$。*

c) *对于每个数值函数 $h \in \mathscr{K}(T)$，$gh$ 是 $\mu$ 可积。*

让我们证明 a) 蕴涵 b)；因为，函数 g 可以通过定位的原理来测量（第 IV, §5, No. 2 章，第 4 条）。另一方面，对于每个$t \in K$，到假设，存在$T$中$t$的邻域$V_t$，使得$g \varphi_{V_t}$可积；因此，我们可以用有限的数邻域$V_i$（$1 \leq i \leq n$）覆盖$K$，使得函数$g \varphi_{V_i}$可积。从$|g| \varphi_K \leq \sum_{i=1}^n |g| \varphi_{V_i}$开始，一个人就有了$\int^* |g| \varphi_K \, d\mu < +\infty$。

其次，b) 蕴含 c)，因为 $gh$ 是可测的，如果 $L$ 是 $h$ 的紧支撑，那么 $|gh| \leq \|h\| \cdot |g| \varphi_L$，因此 $\int^* |gh| \, d\mu < +\infty$乘以假设；因此，$gh$ 可根据可积性准则进行积分（Ch. IV, §5, No. 6，Th. 5）。

最后，c) 暗示了 a)。事实上，对于每个$t \in T$，让$V$成为$t$的紧邻域。存在$T$到$[0,1]$的连续映射$h$，等于$V$上的1并且有紧支撑（第III, §1, No. 2，引理1）；由假设 $gh$ 是可积的，因此 $g \varphi_V = (gh) \varphi_V$ 也是可积的（第 IV, §5, No. 6 章，第 5 章第 3 章）。

#### 定义 1 {#int-v-s5-def-1 .statement tag=092E}

*函数* $g$，*几乎在* $T$（*对于正测量* $\mu$）中局部定义，*在 Banach 空间* $F$（*分别在* $\overline{\mathbf{R}}$）中使用值，*据说可以局部可积* $\mu$（*或局部* $\mu$*-可积*）*如果它满足条件* a), b), c) *命题1.* *如果* $\theta$ *是一个复杂的测度，函数* $g$ *局部定义* $\theta$*-几乎无处不在如果对于正测度* $|\theta|$ 是局部可积的，则称其为局部* $\theta$*-可积。

如果 $g$ 是局部 $\theta$ 可积的，那么每个函数等于 $g$ 的地方几乎处处都是局部可积的。显然，两个局部可积函数的和是局部可积的。 函数与 $F$ 中的值，*随处定义*且对于 $\theta$ 可局部积分，形式向量空间表示为 $\mathscr{L}_{loc}^1(T, \theta; F)$；当$F = \mathbf{R}$或$\mathbf{C}$时，如果没有歧义，通常会省略$F$的提及。这个空间将始终配备（没有明确提及相反）由半范数$g \mapsto \int |g \varphi_K| \, d|\theta|$定义的拓扑，其中$K$运行超过$T$的紧凑子集的集合。相关的 Hausdorff 空间、$\mathscr{L}_{loc}^1(T, \theta; F)$ 的商和映射的子空间 $\mathscr{N}_F^\infty$，几乎在所有地方都是零，被表示为 $L_{loc}^1(T, \theta; F)$。 空间 $L_{loc}^1(T, \theta; F)$ 和 $L_{loc}^1(T, |\theta|; F)$ 相同。

可以证明刚刚定义的拓扑向量空间是*完整的*（例31）。

每个可测量的函数 $g$，本质上以每个紧集为界，都是局部可积的。对于每个数$p$使得$1 \leq p \leq +\infty$，每个函数$g \in \mathscr{L}_F^p$都是局部可积的；事实上，对于每个函数$h \in \mathscr{H}(T)$，$h$属于到$\mathscr{L}^q$（其中$q$是指数共轭到$p$），因此$gh$是可积的（第1章）。 IV, §6, No. 4，第 2 章第 4 章。

令$F, G, H$为三个Banach空间，并且$(u, v) \mapsto \Phi(u, v)$为$F \times G$到$H$的连续双线性映射。如果 $f$ 是局部可积的，并且在 F 中取其值，并且如果 $g \in \mathscr{L}_G^\infty$，则 $\Phi(f, g)$ 是局部可积的（第 IV, §6, No. 4 章，第 2 章的 Cor. 1）。

### 2. 由数值密度定义的度量

令 $g$ 为正数函数局部定义 $\mu$ - 几乎在 T 中任何地方且局部 $\mu$ - 可积； $t$的集合，使得$g(t) = +\infty$在局部$\mu$可以忽略不计，因为对于每个紧集K，$g \varphi_K$是$\mu$可积（第IV, §2, No. 3，第7条）。现在让 $g'$ 为局部可积函数，它是正且有限的，等于 $g$ 局部 $\mu$——几乎处处； 集合$\lambda'_t = g'(t) \varepsilon_t$。 T 的映射 $t \mapsto \lambda'_t$ 到 $\mathscr{M}_+(T)$ 是模糊的 $\mu$ 可测量的，并且本质上是可标量可积的（或者再次，对 $(I, g')$，其中 I 是 T 的恒等映射，是$\mu$-改编）；积分$\nu = \int \lambda'_t d\mu(t)$不依赖于特定的函数$g'$，局部几乎处处都等于$g$，用于措施$\lambda'_t$的定义。该措施$\nu$由条件决定

$$
\int f(t)\,d\nu(t) = \int f(t)g(t)\,d\mu(t) \quad \text{for } f \in \mathscr{K}(T).
$$

如果现在$\theta$是一个复数测度，并且如果$u$是一个复数函数（或函数与$\overline{\mathbf{R}}$中的值）在本地定义$\theta$——几乎在任何地方都可以对$\theta$进行本地可积，则可以写

$$
\begin{align*}
u &= g_1 - g_2 + i(g_3 - g_4) \\
\theta &= \mu_1 - \mu_2 + i(\mu_3 - \mu_4)
\end{align*}
$$

其中 $\mu_1 = (\Re \theta)^+$、$\mu_2 = (\Re \theta)^-$、$\mu_3 = (\Im \theta)^+$、$\mu_4 = (\Im \theta)^-$（III, §1, No. 5 章），以及其中 $g_1, g_2, g_3, g_4$ 具有类似含义；由于 $|u|$ 是局部 $|\theta|$ 可积的，因此每个正值函数 $g_i$ ($i = 1, 2, 3, 4$) 对于每个正测度 $\mu_j$ ($j = 1, 2, 3, 4$) 都是局部可积的，因此映射

$$
f \mapsto \int f(t)u(t)\,d\theta(t)
$$

$\mathscr{K}(T)$ 是一个复杂的度量。

#### 定义 2 {#int-v-s5-def-2 .statement tag=092F}

*令$\theta$为复数测度，并令$u$为复数函数（或函数与$\overline{\mathbf{R}}$中的值）本地定义$\theta$-几乎处处且本地$\theta$可积。 T 上的复测度 $f \mapsto \int fu\,d\theta$ 被认为是测度 $\theta$ 与函数 $u$ 的乘积，或密度 $u$ 相对于 $\theta$ 的测度，并表示为 $u \cdot \theta$。

每个由局部 $\mu$ 可积函数对正测度 $\mu$ 进行乘积的复杂测度称为具有基 $\mu$ 的测度。

按照惯例，关系 $\eta = u \cdot \theta$ 又写成

$$
d\eta(t) = u(t)\, d\theta(t).
$$

当 $u$ 处处定义且连续时，可以恢复第 1 章中给出的定义。 III, §1, No. 4。很明显，如果$u_1$和$u_2$是局部$\theta$可积的，那么$(u_1 + u_2) \cdot \theta = u_1 \cdot \theta + u_2 \cdot \theta$。类似地，如果$\theta_1$和$\theta_2$是$T$的两个测度，并且如果$u$对于$\theta_1$和$\theta_2$来说是函数局部可积，那么$u$对于$\theta_1 + \theta_2$来说是局部可积的并且有一个$u \cdot (\theta_1 + \theta_2) = u \cdot \theta_1 + u \cdot \theta_2$。

从今以后，我们将把自己限制在到处都定义的函数的情况； 扩张到函数几乎到处都在本地定义，这总是显而易见的，留给读者。

对于大多数部分，以下命题允许将复杂措施的情况减少为积极措施的情况：

#### 命题 2 {#int-v-s5-prop-2 .statement tag=092G}

*令$\theta$为复数测度，$u$为局部$\theta$可积复数函数；那么*

$$
|u \cdot \theta| = |u| \cdot |\theta|.
$$

我们从一个辅助结果开始：

#### 引理 1 {#int-v-s5-lem-1 .statement tag=092H}

— *令 $\theta$ 为复数测度，并令 $f$ 为 $\overline{\mathscr{L}}^1_C(T, \theta)$ 的元素。然后*

$$
\langle|\theta|, |f|\rangle = \sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle| = \sup_{c \in \mathscr{B}_1} |\langle\theta, cf\rangle|,
$$

*其中$\mathscr{K}_1$（或$\mathscr{B}_1$）表示复数函数$c$的集合，与紧凑支撑（或Borel）连续，使得$|c| \leq 1$。

我们先来处理$f \in \mathscr{K}(T; \mathbf{C})$的情况。显然

$$
\sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle| \leq \sup_{c \in \mathscr{B}_1} |\langle\theta, cf\rangle| \leq \langle|\theta|, |f|\rangle
$$

（第 IV, §4, No. 2 章，提案 2）。另一方面，令$g$为$\mathscr{K}(T; \mathbf{C})$的元素，使得$|g| \leq |f|$； $g$是序列的统一极限，$\mathscr{K}(T; \mathbf{C})$的元素的$(g_n)$，其支撑包含在由$t$形成的开放集合$U$中，使得$f(t) \neq 0$，并且人们可以清楚地假设：每 $n$ $|g_n| \leq |f|$。 集合$c_n(t) = g_n(t)/f(t)$为$t \in U$，$c_n(t) = 0$为$t \notin U$；然后$c_n \in \mathscr{K}_1$，$g = \lim_{n \to \infty} c_n f$，因此$|\langle\theta, g\rangle| = \lim_{n \to \infty} |\langle\theta, c_n f\rangle|$，最后

$$
\sup_{|g| \leq |f|, g \in \mathscr{K}(T; \mathbf{C})} |\langle\theta, g\rangle| \leq \sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle|.
$$

结论乘注意到，该不等式的第一个成员等于$\langle |\theta|, |f| \rangle$（第III, §1, No. 6，公式（12））。

接下来，用 $\overline{\mathscr{L}}_C^1(\theta)$ 的 $f$ 元素表示，并让我们证明 (4) 再次成立：足以验证此关系的三个成员对于 $\overline{\mathscr{L}}_C^1(\theta)$ 的拓扑持续依赖于 $f$，因为它们重合依赖于稠密子空间$\mathscr{K}(T; \mathbf{C})$。这是由以下不等式立即产生的，其中 $f$ 和 $f'$ 表示元素或 $\overline{\mathscr{L}}_C^1(\theta)$：

$$
|\langle |\theta|, |f| \rangle - \langle |\theta|, |f'| \rangle| \leq \langle |\theta|, |f - f'| \rangle = \overline{N}_1(f - f')
$$
$$
|\langle \theta, cf \rangle - \langle \theta, cf' \rangle| \leq \langle |\theta|, |c||f - f'| \rangle \leq \overline{N}_1(f - f')
$$

对于所有$c \in \mathscr{B}_1$。 引理由此成立。

命题 2 中的经过到证明，让我们将引理应用于函数 $uh$，其中$h$ 属于到$\mathscr{K}_+(T)$。这产生：

$$
\langle |\theta|, |uh| \rangle = \sup_{c \in \mathscr{K}_1} |\langle \theta, cuh \rangle| = \sup_{c \in \mathscr{K}_1} |\langle u \cdot \theta, ch \rangle| = \langle |u \cdot \theta|, h \rangle .
$$

然而，第一个成员也等于

$$
\langle |\theta|, |u|h \rangle = \langle |u| \cdot |\theta|, h \rangle .
$$

因此，两个度量 $|u| \cdot |\theta|$ 和 $|u \cdot \theta|$ 相等。

#### 推论 {#int-v-s5-n2-cor-1 .statement tag=092I}

*设$g_1$和$g_2$为两个局部$\mu$可积数值函数；那么*

$$
\inf(g_1 \cdot \mu, g_2 \cdot \mu) = \inf(g_1, g_2) \cdot \mu ; \quad \sup(g_1 \cdot \mu, g_2 \cdot \mu) = \sup(g_1, g_2) \cdot \mu .
$$

*特别地，如果$g$是局部$\mu$可积数值函数，那么*

$$
(g \cdot \mu)^+ = g^+ \cdot \mu ; \quad (g \cdot \mu)^- = g^- \cdot \mu .
$$

这是从第 2 章的第 2 条命题和公式 (6) 立即得出的。 II, §1, No. 1。

### 3. 相对于密度定义的度量进行积分

*在这个小节的叙述中，$g$表示正数值函数，在各处定义且局部$\mu$可积，$\theta$表示复数测度，$u$表示局部$\theta$可积复数函数.*

No. 2中的注表明§4的结果适用于措施$\nu = g \cdot \mu = \int g(t) \varepsilon_t \, d\mu(t)$（甚至虽然措施$g(t) \varepsilon_t$未定义除非$g(t) \neq +\infty$）。因此我们得到以下叙述：

#### 命题 3 {#int-v-s5-prop-3 .statement tag=092J}

*对于 $T$ 上定义的每个数字函数 $f \geqslant 0$，*

$$
\int^\bullet f \, d\nu = \int^\bullet (f g) \, d\mu .
$$

这是从 Th 得出的。 1 个§4, No. 2。

#### 推论 1 {#int-v-s5-prop-3-cor-1 .statement tag=092K}

*在阶、函数$\mathbf{f}$、值在Banach空间或$\overline{\mathbf{R}}$中，对于$u \cdot \theta$的测度局部可忽略不计，$u \mathbf{f}$对于$\theta$局部可忽略是必要且充分的。*

说$\mathbf{f}$（或$u \mathbf{f}$）对于$u \cdot \theta$（或$\theta$）局部可以忽略不计，相当于说，$|\mathbf{f}|$（或$|u| \cdot |\mathbf{f}|$）对于$|u \cdot \theta|$（或$|\theta|$）局部可以忽略不计。因此，根据No. 2的命题2，我们被简化为$\mathbf{f}, u, \theta$为正的情况； 叙述则立即由命题 3 得出。

#### 推论 2 {#int-v-s5-prop-3-cor-2 .statement tag=092L}

*设$u_1$和$u_2$是两个局部$\theta$可积复数函数。在阶和 $u_1 \cdot \theta = u_2 \cdot \theta$ 中，$u_1$ 和 $u_2$ 几乎处处局部相等是必要且充分的。*

立即简化为表明$u \cdot \theta = 0$意味着$u(t) = 0$局部几乎无处不在；但$u \cdot \theta = 0$意味着函数1对于测度$u \cdot \theta$来说局部可以忽略不计。然后应用推论 1。

#### 推论 3 {#int-v-s5-prop-3-cor-3 .statement tag=092M}

*令$u$为复数函数，对于正测度$\mu$可局部积分。为了使 $u \cdot \mu$ 成为一个积极的措施，$u(t) \geqslant 0$ 几乎在任何地方都是必要且充分的。*

因为，当且仅当 $u \cdot \mu = |u \cdot \mu| = |u| \cdot \mu$（命题 2）时，$u \cdot \mu$ 才为正，这几乎在任何地方都等价于局部$u = |u|$（Cor. 2）。

#### 命题 4 {#int-v-s5-prop-4 .statement tag=092N}

*为了将 $T$ 的映射 $f$ 转换成拓扑空间 $G$ 对于测度 $u \cdot \theta$ 可测，$f$ 的限制到$\theta$ 可测集合是必要且充分的$t$的$S$使得$u(t) \neq 0$是$\theta$可测量的。*

当$u$和$\theta$为正时，这立即从§4, No. 3的命题3得出。由于命题 2，结果是扩展到 $u$ 和 $\theta$ 很复杂的情况。

#### 推论 {#int-v-s5-n3-cor-1 .statement tag=092O}

*令 $\mathbf{f}$ 为 $T$ 上定义的函数，其中值在 Banach 空间 $F$ 或$\overline{\mathbf{R}}$ 中。为了使 $\mathbf{f}$ $(u \cdot \theta)$ 可测量，$u \mathbf{f}$ $\theta$ 可测量是充分必要的。*

因为，$u \mathbf{f}$是扩张除以$(u \mathbf{f})|S$到$T$中的0。

#### 定理 1 {#int-v-s5-thm-1 .statement tag=092P}

*令 $\mathbf{f}$ 为 $T$ 上定义的函数，其中值在 Banach 空间 $F$ 或$\overline{\mathbf{R}}$ 中。在阶中，$\mathbf{f}$对于*测度$\eta = u \cdot \theta$本质上可积，$uf$本质上$\theta$可积是必要且充分的，在这种情况下

$$
\int f \, d\eta = \int (uf) \, d\theta .
$$

此外，假设$u$是连续的，并且$u(t) \neq 0$对于所有$t \in T$；那么$f$对于测度$\eta$可积当且仅当$uf$对于$\theta$可积。

从 Th 立即得出 $u$ 和 $\theta$ 为正的情况。 2 个§4, No. 4。 叙述的第一个和最后一个断言紧随其后，因为$f$相对于$\eta = u \cdot \theta$本质上可积（可积）当且仅当它对于$|\eta| = |u| \cdot |\theta|$本质上可积（可积）。最后，假设 $f$ 本质上可积为 $\eta$（因此也可积为 $|\eta|$）；我们利用分解 (2)：$f$ 对于每个测度 $\eta_{ij} = g_i \cdot \mu_j$ ($i = 1, 2, 3, 4,\ j = 1, 2, 3, 4$) 本质上是可积的，因为这些测度是 $\leq |\eta|$。我们有

$$
\int f \, d\eta_{ij} = \int g_i f \, d\mu_j .
$$

公式 (6) 紧随其后。

#### 推论 {#int-v-s5-n3-cor-2 .statement tag=092Q}

为了使测度$u \cdot \theta$有界，$u$本质上$\theta$可积是必要且充分的。

#### 例 {#int-v-s5-n3-exa-1 .statement tag=092R}

令$A$为$T$中的子集；为了使$\varphi_A$局部$\mu$可积，$A$是$\mu$可测是充分必要的。假设满足条件，则集合$\nu = \varphi_A \cdot \mu$；对于 $T$ 上定义的每个数字函数 $f \geq 0$，我们有

$$
\int^\bullet f \, d\nu = \int^\bullet f \varphi_A \, d\mu ,
$$

也用 $\int_A^\bullet f \, d\mu$ (cf. Ch. IV, §5, No. 6) 表示的数量。为了使$T$的映射$g$成为空间$G$是$\nu$可测的，$g$到$A$的限制是必要且充分的$\mu$-可测量。为了将$T$的映射$f$转化为Banach空间$F$或转化为$\overline{\mathbf{R}}$本质上$\nu$可积，$f \varphi_A$本质上$\mu$可积是必要且充分的，在这种情况下

$$
\int f \, d\nu = \int f \varphi_A \, d\mu ,
$$

也表示为 $\int_A f \, d\mu$ 的表达式。 请注意，如果 $T$ 的两个映射进入 $G$（或 $F, \overline{\mathbf{R}}$）重合在 $A$ 上，则其中一个为 $\nu$ 可测（或实质上 $\nu$ 可积），则另一个也是必要且充分的。 如果现在$g$是映射进入$T$的任意子集$B \supset A$的$G$，则可以说$g$是$\mu$可测量*在*$A$，如果任意扩张到$T$ $g$到$A$的限制是$\nu$可测，相当于说，$g$到$A$的限制是$\mu$可测。 将 $B$ 的映射 $f$ 转化为 Banach 空间 $F$，或转化为 $\overline{\mathbf{R}}$，据说是 *本质上* $\mu$ 可在 * $A$ 上积分，如果某些扩张 $\overline{f}$ 到$f$到$A$的限制的$T$本质上是$\nu$可积；一然后集合
$$
\int_A f \, d\mu = \int_A \overline{f} \, d\mu = \int \overline{f} \varphi_A \, d\mu,
$$
有人说$\int_A f \, d\mu$是*$f$*在*$A$上的*整的（或*扩展到*$A$）。 如果$f$是在$B \supset A$上定义的数值函数$\geqslant 0$，则定义与$\int_A^* f \, d\mu$和$\int_A^\bullet f \, d\mu$类似。 最后，如果 $g$ 到 $A$ 的限制的扩张 $\overline{g}$ 到 $T$，则在 $B \supset A$ 上定义的数值函数 $g$ 被认为是 * 局部 * $\mu$ 可在 * $A$ 上可积的。是局部$\nu$可积的：这相当于说，对于$T$的每个紧凑子集$K$，$\overline{g} \varphi_{K \cap A}$是$\mu$可积。

### 4. 乘积相对于通常运算的行为

#### 命题 5 {#int-v-s5-prop-5 .statement tag=092S}

*让*$(\lambda_\alpha)_{\alpha \in A}$*成为*$T$的一系列积极措施，*针对关系*$\leqslant$，*承认*$\mathscr{M}(T)$*最高*$\lambda$。 *对于正数函数* $g$ *要局部* $\lambda$-*可积，必要且充分的是* $g$ *局部* $\lambda_\alpha$-*对于每个* $\alpha \in A$ *可积，并且族* $(g \cdot \lambda_\alpha)$ *在* $\mathscr{M}(T)$上有界； *在这种情况下，
$$
g \cdot \lambda = \sup_{\alpha \in A} g \cdot \lambda_\alpha.
$$
显然条件是必要的。相反，假设$g$对于每个测度$\lambda_\alpha$都是局部可积的，并且族$(g \cdot \lambda_\alpha)_{\alpha \in A}$在上面有界；用 $\lambda'$ 表示其上界。 函数 $g$ 则 $\lambda$ 可测（§ 1, No. 4，第 11 条命题第 2 条）；此外，对于每个函数 $h \in \mathscr{K}_+(T)$，
$$
\int^\bullet (hg) \, d\lambda = \sup_{\alpha \in A} \int^\bullet (hg) \, d\lambda_\alpha = \sup_{\alpha \in A} \int^\bullet h \, d(g \cdot \lambda_\alpha) = \int^\bullet h \, d\lambda'
$$
（§ 1, No. 4，提案 11）。首先，这意味着第一个成员对于任何$h$都是有限的，因此$g$是局部$\lambda$可积的；因此，符号$\int^\bullet$可以替换为$\int$，并且公式可以写成$\int h \, d(g \cdot \lambda) = \int h \, d\lambda'$。接下来是$g \cdot \lambda = \lambda'$，这样就完成了证明。

#### 推论 {#int-v-s5-n4-cor-1 .statement tag=092T}

— 假设 $\mu$ 是 T 上度量族 $(\mu_\alpha)_{\alpha \in A}$ 的和。对于定义在 T 上的正数值函数 g 局部 $\mu$ 可积，g 对每个 $\alpha \in A$ 局部 $\mu_\alpha$ 可积是必要且充分的，且族 $(g \cdot \mu_\alpha)_{\alpha \in A}$是可总结的。在这种情况下，

$$
g \cdot \mu = \sum_{\alpha \in A} g \cdot \mu_\alpha.
$$

令$(g_\alpha)_{\alpha \in A}$是在T上定义的$\mu$-可测量正函数的族。令$S_\alpha$是$t \in T$的集合，使得$g_\alpha(t) \neq 0$。如果族 $(S_\alpha)$ 是局部可数的（第 IV, §5, No. 9 章），我们可以说族 $(g_\alpha)$ 是*局部可数的*；这相当于说，对于 T 中的每个紧集 K，$\alpha \in A$ 中的集合使得 $g_\alpha|K$ 不是零是可数的。

#### 命题 6 {#int-v-s5-prop-6 .statement tag=092U}

— 令 $(g_\alpha)_{\alpha \in A}$ 为 T 上定义的局部 $\mu$ 可积正数值函数的局部可数族。在阶中，函数 $g = \sum_{\alpha \in A} g_\alpha$ 为局部 $\mu$ 可积，测度族 $(g_\alpha \cdot \mu)_{\alpha \in A}$ 可求和是必要且充分的，在这种情况下

$$
g \cdot \mu = \sum_{\alpha \in A} g_\alpha \cdot \mu.
$$

很明显，$g$ 是 $\mu$ 可测的（第 IV, §5, No. 2 章，第 4 条命题和 No. 4，第 2 条的 Cor.1）。因此，对于$g$局部$\mu$可积，$\mu^\bullet(gf)$对于每个$f \in \mathscr{H}_+(T)$是有限的是必要且充分的。现在，由于$\alpha \in A$的集合使得$g_\alpha f \neq 0$是可数的，我们有$\mu^\bullet(gf) = \sum_{\alpha \in A} \mu^\bullet(g_\alpha f)$（§1, No. 1，Prop.2的Cor.）。 集合$\nu_\alpha = g_\alpha \cdot \mu$； 条件 $\mu^\bullet(gf) < +\infty$ 等价于条件 $\sum_{\alpha \in A} \nu_\alpha(f) < +\infty$：在其他字中，$g$ 是局部 $\mu$ 可积的，当且仅当族 $(\nu_\alpha)$ 可求和。将该族的和记为$\nu$，则上述计算得到等式$\nu(f) = \mu^\bullet(gf)$，相当于(8)。

#### 推论 {#int-v-s5-n4-cor-2 .statement tag=092V}

— 令 $(g_\alpha)$ 为局部 $\mu$ 可积数值函数的序列，使得测度 $g_n \cdot \mu$ 的序列为递增。在阶中，这个序列在T上的实测度有序向量空间$\mathscr{M}(T)$中有上界，函数$g = \sup g_n$是局部$\mu$可积的充分必要； 序列 $(g_n \cdot \mu)$ 中的$\mathscr{M}(T)$ 的上界就是测度$g \cdot \mu$。

将第 6 条命题应用到函数（几乎所有地方都是局部正数）$g'_n = g_{n+1} - g_n$ 就足够了。

#### 命题 7 {#int-v-s5-prop-7 .statement tag=092W}

— 令X为无穷大可数的局部紧凑空间，并令$t \mapsto \lambda_t$为T到$\mathscr{M}_+(X)$的$\mu$充分映射。

令 $g$ 为在 $X$ 上定义的正数值函数，可对测度 $\nu = \int \lambda_t d\mu(t)$ 进行局部可积。 $t \in T$的集合使得$g$不是局部$\lambda_t$可积，那么对于$\mu$，映射$t \mapsto g \cdot \lambda_t$（局部定义$\mu$-几乎无处不在）是$\mu$-足够的，并且

$$
g \cdot \nu = \int (g \cdot \lambda_t) d\mu(t).
$$

设$(K_n)_{n \in \mathbf{N}}$为$X$的紧凑子集的递增序列，其内部覆盖$X$；如果 $\eta$ 是 $X$ 上的任何正测度，​​则说 $g$ 是局部 $\eta$ 可积的，相当于说 $g \varphi_{K_n}$ 对于每个 $n$ 是 $\eta$ 可积的。现在令$H_n$为$t \in T$的集合，使得$g \varphi_{K_n}$不可积$\lambda_t$，并令$H = \bigcup_n H_n$；由于$H_n$对于所有$n$（§ 3, No. 3，Th.1）来说在本地$\mu$可以忽略不计，因此$H$也是如此，它建立了叙述的第一个断言。对于$H$中的$t$，替换$\lambda_t$除以0（这不是变换度量$\nu$），我们可以假设$g$对于每个$t \in T$是局部$\lambda_t$可积的。对于$X$上定义的每一个$\nu$可测量正函数$h$，根据§ 3, No. 2的第3条和第5条，我们有，

$$
\int^\bullet h d(g \cdot \nu) = \int^\bullet (gh) d\nu = \int^\bullet d\mu(t) \int^\bullet (gh) d\lambda_t = \int^\bullet d\mu(t) \int^\bullet h d(g \cdot \lambda_t).
$$

这个公式和§ 3, No. 2的命题5首先表明（在取$h \in \mathscr{K}_+(X)$时）映射$t \mapsto g \cdot \lambda_t$本质上是$\mu$可标量可积的，并且它的积分是$g \cdot \nu$；在其他字中，关系 (9) 成立。接下来，让我们通过正测量$\mu' \leq \mu$来计算替换$\mu$，并让我们对$h$取一个正下半连续函数：从这些关系立即可以得出$t \mapsto g \cdot \lambda_t$是$\mu$-充分的（§ 3, No. 1，定义1）。

#### 命题 8 {#int-v-s5-prop-8 .statement tag=092X}

*令$\theta$为$T$的复测度，$g_1$为本地$\theta$可积复数函数，$\theta_1$测度$g_1 \cdot \theta$。对于在 $T$ 上定义的复数函数 $g_2$ 局部 $\theta_1$ 可积，$g_2 g_1$ 局部 $\theta$ 可积是必要且充分的，在这种情况下*

$$
g_2 \cdot \theta_1 = g_2 \cdot (g_1 \cdot \theta) = (g_2 g_1) \cdot \theta
$$
（“结合性公式”）。

根据命题4的推论，说$g_2$是$\theta_1$可测就相当于说说$g_2 g_1$是$\theta$可测。让我们假设这个条件得到满足。对于每个函数 $f \in \mathscr{K}_+(T)$，我们有命题 2 和 3，

$$
\int^\bullet |g_2| f d|\theta_1| = \int^\bullet |g_2| f |g_1| d|\theta| = \int^\bullet |g_2 g_1| f d|\theta|.
$$

因此，说 $g_2$ 是局部 $\theta_1$ 可积的，就等价于说 $g_2 g_1$ 是局部 $\theta$ 可积的。假设 Th 满足条件。 1 我们有

$$
\int f \, d(g_2 \cdot \theta_1) = \int f g_2 \, d\theta_1 = \int f g_2 g_1 \, d\theta = \int f \, d(g_2 g_1 \cdot \theta),
$$

公式相当于(10)。

### 5. 刻画措施，基 $\mu$

#### 定理 2（勒贝格-尼科迪姆）{#int-v-s5-thm-2 .statement tag=092Y}

— *令$\mu$和$\nu$为$T$的两个积极措施。以下属性是等效的：*

1) $\nu$ *是基 $\mu$* 的度量。
2) *每个局部$\mu$-可忽略的集合都是局部$\nu$-可忽略*。
3) *每个$\mu$-可忽略的紧集都是$\nu$-可忽略*。

很明显，1) 意味着 2)（命题 3 的 Cor.1），而 2) 意味着 3)。我们将证明 3) 蕴涵 1)。我们首先注意到，如果满足条件 3)，那么每个集合$A$是“普遍可测”且局部$\mu$-可忽略的，局部$\nu$-可忽略的；对于，$\nu^\bullet(A) = \sup \nu(K)$，其中$K$超过$A$中包含的紧集的集合（§ 1, No. 3，第10条，a）和第1章。 IV, § 4, No. 6，科。 2 Th。 4).接下来，我们将建立两个引理。

#### 引理 2 {#int-v-s5-lem-2 .statement tag=092Z}

— *令 $\alpha$ 为 $T$ 上的有界正测度，$\beta$ 为 $T$ 上的实测度，使得 $|\beta| \leq M \alpha$，其中 $M$ 为正常数。那么，存在实数函数$u$、$\alpha$可积，使得$\beta = u \cdot \alpha$*。

令$g$为空间$\mathscr{L}_\mathbf{R}^2(T, \alpha)$中的元素； $g$ 是 $\beta$ 可测量的且 $\int^\bullet |g|^2 \, d|\beta| \leq M \int^\bullet |g|^2 \, d\alpha < +\infty$。 函数$g$，因此属于到$\mathscr{L}^2(T, |\beta|)$，并且也到$\mathscr{L}^1(T, |\beta|)$，因为$\beta$是有界的。根据柯西-施瓦茨不等式，

$$
|\beta(g)|^2 \leq \left( \int |g| \, d|\beta| \right)^2 \leq \left( \int d|\beta| \right) \left( \int |g|^2 \, d|\beta| \right) \leq M^2 \alpha(1) \, \alpha(|g|^2).
$$

因此映射$g \mapsto \beta(g)$是$\mathscr{L}^2(T, \alpha)$上的连续线性形式。与 $\mathscr{L}^2(T, \alpha)$ 相关联的 Hausdorff 空间是希尔伯特空间，则存在（TVS，Ch. V, § 1, No. 7，Th. 3）实函数 $u \in \mathscr{L}^2(T, \alpha)$，因此也有属于到 $\mathscr{L}^1(T, \alpha)$，这样每 $g \in \mathscr{L}^2(T, \alpha)$ $\beta(g) = \alpha(ug)$。 应用这个关系换$g \in \mathscr{K}(T)$，一看就是$\beta = u \cdot \alpha$。

#### 引理 3 {#int-v-s5-lem-3 .statement tag=0930}

— *假设正测度$\nu$使得每个$\mu$-可忽略的紧集都是$\nu$-可忽略。令 $\mathfrak{K}$ 为 $T$ 的紧凑子集 $K$ 的集合，具有以下性质：*

(11) 存在常数$M \geq 0$使得$\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$。
那么集合$\mathscr{K}$在$T$中是$\mu$密集。

如果$K$满足(11)，并且如果$A$是包含在$K$中的Borel集合，则立即从命题8得出$\varphi_A \cdot \nu \leq M \varphi_A \cdot \mu$；由此，可以推导出$\mathscr{K}$属于的两个元素$K, K'$到$\mathscr{K}$的并因为$\varphi_{K \cup K'} = \varphi_K + \varphi_A$，其中$A = K' \cap \complement K$。为了建立引理，还需要证明每个紧集$L$使得$\mu(L) > 0$包含紧集$K \in \mathscr{K}$使得$\mu(K) > 0$（第IV, §5, No. 8，第12条）。 选择数 $M > \nu(L)/\mu(L)$ 并将引理 1 应用于有界正测度 $\alpha = \varphi_L \cdot (\nu + M \mu)$ 和测度 $\beta = \varphi_L \cdot (\nu - M \mu)$。 替换如果需要函数 $u$ 使得$\beta = u \cdot \alpha$乘以函数等于它$\alpha$——几乎在任何地方，我们都可以假设$u$是普遍可测的（§3, No. 4，第7条）并且零在$L$。 集合 $H$ 的 $t \in T$ 使得 $L$ 中包含的 $u(t) < 0$ 不能被 $\mu$ 忽略不计，因为它将是 $\nu$ 忽略不计（由注在证明开始时制作） Th. 2)，因此 $\alpha$ 可以忽略不计，并且可以有 $\beta(L) > 0$，其中与……矛盾选择为 $M$。令$K$为紧集包含在$H$中，使得$\mu(K) > 0$；让我们证明$K \in \mathscr{K}$，这将建立引理。根据第 8 号提案，

$$
\varphi_K \cdot (\nu - M \mu) = \varphi_K \cdot \beta = \varphi_K \cdot (u \cdot \alpha) = (\varphi_K u) \cdot \alpha .
$$

函数 $\varphi_K u$ 是负数，因此我们确实有 $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$。

现在让我们完成定理 2 的证明。假设条件 3) 已被验证，且定义 $\mathscr{K}$ 如引理 3 所示。令 $(K_\alpha)_{\alpha \in A}$ 为成对的不相交的元素的局部可数族$\mathscr{K}$，使得集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$ 局部 $\mu$ 可以忽略不计（第 IV, §5, No. 9，第 14 条命题）；家庭$(K_\alpha)$是局部可数的，$N$是普遍可测的，因此局部$\nu$可以忽略不计。 集合$\mu_\alpha = \varphi_{K_\alpha} \cdot \mu$、$\nu_\alpha = \varphi_{K_\alpha} \cdot \nu$；由于函数 $\varphi_{K_\alpha}$ 形式是一个局部可数家庭，对于 $\mu$ 和 $\nu$，其和在局部几乎处处都等于 1，命题 6 意味着 $\mu = \sum_{\alpha \in A} \mu_\alpha$、$\nu = \sum_{\alpha \in A} \nu_\alpha$。另一方面，通过$\mathscr{K}$的定义，对于每个$\alpha$，都存在一个常数$M_\alpha$，使得$\nu_\alpha \leq M_\alpha \mu_\alpha$；因此，引理 2 意味着函数 $g_\alpha$ 的存在，可以假设它是 $K_\alpha$ 之外的零并且为正（第 3 条命题的 Cor. 3），这样 $\nu_\alpha = g_\alpha \cdot \mu_\alpha$。因此（No. 4，提案 8）

$$
\nu_\alpha = g_\alpha \cdot \mu_\alpha = g_\alpha \cdot (\varphi_{K_\alpha} \cdot \mu) = (g_\alpha \varphi_{K_\alpha}) \cdot \mu = g_\alpha \cdot \mu .
$$

集合$g = \sum_{\alpha \in A} g_\alpha$；由于族 $(g_\alpha)$ 是局部可数的，族 $(\nu_\alpha)$ 是可求和的，命题 6 意味着 $g$ 是局部 $\mu$ 可积的，并且 $\nu = g \cdot \mu$ 建立了定理。

#### 推论 1 {#int-v-s5-thm-2-cor-1 .statement tag=0931}

— 设 $\mathscr{N}$ 为集合，其中基 $\mu$，承认$\mathscr{M}(T)$ 中的上等$\nu$；那么 $\nu$ 是基 $\mu$ 的度量。

科。提案2允许减少到$\mathscr{N}$为递增有向集合的情况。对于每一个局部 $\mu$ 可忽略不计的集合 $A$，根据 §1, No. 4 的第 11 条提案，

$$
\nu^\bullet(A) = \sup_{\lambda \in \mathscr{N}} \lambda^\bullet(A) = 0.
$$

因此，定理 2 意味着$\nu$ 是基 $\mu$ 的测度。

#### 推论 2 {#int-v-s5-thm-2-cor-2 .statement tag=0932}

— 设$\nu$为$T$的实测度。在阶中，$\nu$属于到完全格序空间$\mathscr{M}(T)$（第II, §1, No. 5）中由$\mu$生成的能带，$\nu$是基的测度是必要且充分的$\mu$。

在考虑$\nu^+$和$\nu^-$时，立即将其简化为积极措施$\nu$的情况（No. 2，Prop.2的Cor.）。那么让我们集合$\nu_n = \inf(n\mu, \nu)$； $\nu$ 属于到由 $\mu$ 生成的带当且仅当 $\nu = \sup_n \nu_n$（第 II, §1, No. 5 章，第 6 条命题）。现在，$\nu_n$以$n\mu$为界，是一个以Th为基$\mu$的测度。 2；因此，关系$\nu = \sup_n \nu_n$意味着$\nu$是基$\mu$的测度（Cor.1）。相反，假设 $\nu$ 是基 $\mu$: $\nu = g \cdot \mu$ 的测度，其中 $g$ 是局部 $\mu$ 可积且为正值。然后$\nu_n = \inf(g, n) \cdot \mu$（第2条命题的Cor.），并且立即从勒贝格的定理（第IV, §4, No. 3章，第4条命题）得出$\nu = \sup_n \nu_n$。

#### 推论 3 {#int-v-s5-thm-2-cor-3 .statement tag=0933}

— 令 $\theta$ 为复杂测度；存在普遍可测的函数$v$，以及$|v| = 1$，使得$\theta = v \cdot |\theta|$，$|\theta| = \overline{v} \cdot \theta$。

写$\theta = \theta_1 - \theta_2 + i(\theta_3 - \theta_4)$，其中$\theta_1 = (\Re \theta)^+$，$\theta_2 = (\Re \theta)^-$，$\theta_3 = (\Im \theta)^+$，$\theta_4 = (\Im \theta)^-$；正测度 $\theta_i$ ($i = 1, 2, 3, 4$)，以 $|\theta|$ (第 III, §1, No. 6, 公式 (17)) 为界，是基 $|\theta|$ 定理 2 的测度。因此，存在局部 $|\theta|$ 可积函数$v$使得$\theta = v \cdot |\theta|$。 命题 2 然后产生关系 $|\theta| = |v| \cdot |\theta|$，这意味着 $|v| = 1$ 局部$|\theta|$——几乎无处不在（第 3 条的 Cor. 2）。最后，根据第 8 号提案，$\overline{v} \cdot \theta = (v \overline{v}) \cdot |\theta| = |\theta|$。由于函数$v$仅定义为局部$|\theta|$可忽略不计的函数，因此可以假设$v$是普遍可测的（§3, No. 4，第7条）并且$|v| = 1$无处不在。

#### 注 1 {#int-v-s5-n5-rem-1 .statement tag=0934}

假设$\lambda$是正测度，$v$是$\lambda$可测的函数，使得$|v| = 1$局部$\lambda$几乎处处可积（这意味着$v$局部$\lambda$可积），并且$\theta = v \cdot \lambda$。命题 2 立即表明 $\lambda = |\theta|$；在其他字中，前述叙述的性质表征了积极措施$|\theta|$。

#### 注 2 {#int-v-s5-n5-rem-2 .statement tag=0935}

如果 $|\theta| \leq a \mu$，其中 $\mu$ 是正测度，$a$ 是数 $\geq 0$，则 $\theta$ 是具有基 $\mu$ 的测度。

#### 推论 4 {#int-v-s5-thm-2-cor-4 .statement tag=0936}

— 令 $\rho$ 和 $\theta$ 为两个复数度量。在阶中，存在局部$\theta$可积函数$u$使得$\rho = u \cdot \theta$，每个$\theta$可忽略的紧集是$\rho$可忽略的是充分必要的。

条件显然是必要的。相反，假设每个$\theta$-可忽略的紧集都是$\rho$-可忽略； 定理 2 意味着存在局部$|\theta|$可积函数$g$，使得$|\rho| = g \cdot |\theta|$。另一方面，科。 3 意味着存在函数 $v_1$（分别为 $v_2$）、绝对值值 1 以及可测量的度量 $|\rho|$（分别为 $\theta$），使得 $\rho = v_1 \cdot |\rho|$（分别为 $|\theta| = \overline{v_2} \cdot \theta$）。然后，根据第 8 条命题，$\rho = u \cdot \theta$ 与 $u = v_1 g \overline{v_2}$。

#### 推论 5 {#int-v-s5-thm-2-cor-5 .statement tag=0937}

— 令 $\mu$ 和 $\nu$ 为 Th 的 T. 条件 1), 2), 3) 的两个正测度。 2 也相当于以下：

4) 对于每个$\nu$可积数值函数$f \geq 0$和每个数$\varepsilon > 0$，都存在一个$\delta > 0$，使得关系$0 \leq h \leq f$和$\int^* h \, d\mu \leq \delta$隐含$\int^* h \, d\nu < \varepsilon$。

5) 对于每个函数$g \in \mathscr{K}_+(\mathrm{T})$和每个数$\varepsilon > 0$，都存在一个$\delta > 0$，这样，对于上面由$g$和满足$\int h \, d\mu \leq \delta$界定的每个$h \in \mathscr{K}_+(\mathrm{T})$，都有$\int h \, d\nu \leq \varepsilon$。

6) 对于每个紧集$K \subset \mathrm{T}$和每个数$\varepsilon > 0$，都存在一个$\delta > 0$，使得关系$A \subset K$和$\mu^*(A) \leq \delta$隐含$\nu^*(A) \leq \varepsilon$。

4) $\Rightarrow$ 6) $\Rightarrow$ 3) 的含义是显而易见的。

假设存在有限的函数$k \geq 0$，普遍可测且局部$\mu$可积，使得$\nu = k \cdot \mu$，让我们证明满足条件4)。令$f$为$\nu$可积函数$\geq 0$，并令$\varepsilon > 0$。对于每个整数$n \geq 0$，令$A_n$为$t \in \mathrm{T}$的集合，使得$k(t) \geq n$。 函数 $f \varphi_{A_n}$ 形式递减序列，以$f$为界并逐点趋于0，因此存在$N$使得$\int f \varphi_{A_N} \, d\nu \leq \varepsilon/2$（第IV, §4, No. 3，第4条）。如果$h$在$\mathrm{T}$满足$0 \leq h \leq f$和$\int^* h \, d\mu \leq \varepsilon/2N$上是函数，则

$$
\nu^*(h) \leq \nu^*(h \varphi_{A_N}) + \nu^*(h(1 - \varphi_{A_N}))
$$
$$
\leq \nu^*(f \varphi_{A_N}) + \mu^*(h(1 - \varphi_{A_N})k)
$$
$$
\leq \frac{\varepsilon}{2} + N \mu^*(h) \leq \varepsilon.
$$

由此我们证明了条件4)和6)等价于Th的条件。 2.

显然，4）暗示着5）。最后，如果满足条件 5)，则 $\nu$ 属于到由 $\mu$ 生成的频带（第 II, §2, No. 2，提案 5），因此有基 $\mu$（Cor. 2）。

#### 学院{#int-v-s5-n5-sch-1 .statement tag=0938}

对于每个$\dot{f} \in L^1_{\mathrm{loc}}(\mathrm{T}, \mu; \mathbf{R})$，集合$\varphi(\dot{f}) = f \cdot \mu$，其中$f \in \dot{f}$； 映射$\varphi$是线性的，递增是单射的（第3命题的Cor.2），$\mathscr{M}(T)$中的像是由$\mu$（第2命题的Cor.2）生成的能带B。因此，映射$\varphi$允许将$L^1_{\text{loc}}(T, \mu; \mathbf{R})$与空间识别为T上的实际度量；由于空间$L^p_R(T, \mu)$都是$L^1_{\text{loc}}(T, \mu; \mathbf{R})$的子空间，因此它们也可以被识别为$\mathscr{M}(T)$的子空间。类似的考虑也适用于复值函数和度量。请注意，上面考虑的映射$\varphi$是$L^1_{\text{loc}}$和B的有序向量空间结构的同构，但对于这些的*拓扑向量空间*结构显然不是同构空间。

由于完全晶格有序空间中的每个能带本身就是完全晶格有序空间（第 II, §1, No. 5），因此可以看到空间 $L^1_{\text{loc}}$ 是*完全晶格有序*；但值得记住的是，等价类的不可数族$(\dot{f}_\alpha)$的$L^1_{\text{loc}}$中的上界不一定与函数$f_\alpha$的上包络线的类相同。然而，我们看到，对于局部 $\mu$ 可积函数的 *递增序列* $(f_n)$，其上包络$f$ 局部$\mu$ 可积，$f \cdot \mu$ 是$\mathscr{M}(T)$ 中$(f_n \cdot \mu)$ 测度序列的上乘（Cor. of Prop. 6）。

这是 Th 的推论 3 的一个有趣的推论。 2：

#### 命题 9 {#int-v-s5-prop-9 .statement tag=0939}

*令 $\theta$ 为有界复数测度；要使$\theta$成为积极措施，$\| \theta \| = \theta(1)$.*是必要且充分的。

条件显然是必要的。相反，假设$\| \theta \| = \int d\theta$，并用$v$表示绝对值1的$|\theta|$可测量函数，使得$\theta = v \cdot |\theta|$。由于$\| \theta \| = \int d|\theta|$（第IV, §4, No. 7，第12条命题）和$\int d\theta = \int v \cdot d|\theta|$（第1条），假设意味着$\int (1 - v) \, d|\theta| = 0$，因此意味着$\int \mathscr{R}(1 - v) \, d|\theta| = 0$。 函数$\mathscr{R}(1 - v)$为正，因此零几乎无处不在，这意味着$v = 1$几乎无处不在并完成证明。

### 6. 等效措施

#### 命题 10 {#int-v-s5-prop-10 .statement tag=093A}

*令$\mu$和$\nu$为T上的两个正测度。以下条件是等价的：
a) 局部可忽略的集合对于$\mu$和$\nu$是相同的。
b) $\mathscr{M}(T)$ 中$\mu$ 和$\nu$ 生成的能带是相同的。
c) 一个有$\nu = g \cdot \mu$，其中$g$在本地$\mu$可积，而$g(t) > 0$在$\mu$几乎任何地方都可积。*

条件 a) 和 b) 由 Cor 等价。 2 Th。 2 个No. 5。如果满足，则$\nu = g \cdot \mu$和$\mu = h \cdot \nu$，其中$g$（分别$h$）为正，且对于$\mu$（分别$\nu$）可局部积分。因此（No. 4，命题 8）$hg$ 是局部$\mu$可积且$\mu = (hg) \cdot \mu$。由此可见（No. 3，第 3 条命题的 Cor.2），对于 $\mu$，$hg$ 几乎在任何地方都等于 1，因此对于 $\mu$，$g(t) > 0$ 和 $h(t) = 1/g(t)$ 几乎在任何地方都等于 1。相反，假设 $\nu = g \cdot \mu$ 和 $g(t) > 0$ 局部几乎处处都是 $\mu$；

因为 $(1/g)g$ 几乎在任何地方都被局部定义并且是局部 $\mu$ 可积的，$1/g$ 是局部 $\nu$ 可积的并且$(1/g) \cdot \nu = \mu$（No. 4，第 8 条）。

#### 定义 3 {#int-v-s5-def-3 .statement tag=093B}

*如果提案 10 的措施 $|\theta|$ 和 $|\theta'|$ 满足条件 a)、b)、c)，则称局部紧凑空间 $T$ 上的两个复杂措施 $\theta, \theta'$ 是等效的。*

因而，为了使$\theta$和$\theta'$等价，$|\theta|$和$|\theta'|$等价是充分必要的。

#### 注 {#int-v-s5-n6-rem-1 .statement tag=093C}

— 如果 $\mu$ 和 $\nu$ 是两个等效的正测量，则在 $T$ 上定义的可测量函数，以及任何拓扑空间 $G$ 中的值，对于 $\mu$ 和 $\nu$ *相同*，如下： No. 3 的第 4 号提案。

#### 命题 11 {#int-v-s5-prop-11 .statement tag=093D}

*令 $\mu$ 为 $T$ 的正测度。如果 $T$ 在无穷大处可数，则存在连续函数 $h$，使得 $h(t) > 0$ 对于所有 $t \in T$ 且测度 $\nu = h \cdot \mu$（相当于 $\mu$）有界。*

令$(K_n)$为紧集的序列，形成$T$的覆盖，并且对于每个$n$，令$f_n$为$\mathscr{H}(T)$中的函数，使得$0 \leq f_n \leq 1$和$f_n(t) = 1$在$K_n$（第III, §1, No. 2、引理1）。令$(a_n)$为数$> 0$中的序列，使得$\sum_n a_n < +\infty$； 级数$h = \sum_n a_n f_n$通常会收敛于$T$，因而$h$是$T$上的连续函数，使得$h(t) > 0$对于所有$t \in T$，通过构造。 设定 $\nu = h \cdot \mu$，则我们有（第 3 条命题和第 IV, §1, No. 3 章，第 13 条命题）

$$
\nu^*(1) = \int^* h \, d\mu \leq \sum_n a_n \int f_n \, d\mu .
$$

例如，当$\int f_n \, d\mu > 1$时为$a_n = 2^{-n} (\int f_n \, d\mu)^{-1}$，否则为$a_n = 2^{-n}$，我们有$\sum_n a_n < +\infty$和$\nu^*(1) < +\infty$，这证明了命题。

#### 命题 12 {#int-v-s5-prop-12 .statement tag=093E}

*令$(\mu_n)$为$T$上有界正测度的序列； $T$ 上存在有界正测度 $\mu$，使得关系 $\mu^*(N) = 0$ 等价于每个 $n$» 的“$\mu_n^*(N) = 0$”；每个措施$\mu_n$都有基$\mu$。此外，如果$\mu'$是具有性质的$T$的第二个正测度，则$\mu$和$\mu'$是等价的。*

叙述的最后一个部分立即从 Def 开始。 3. 为了证明$\mu$的存在，我们可以限制为对于每个$n$都有$\mu_n \neq 0$；然后，度量族$\mu_n / 2^n \| \mu_n \|$可在$\mathscr{M}(T)$中求和，并且其和$\mu$使得$\| \mu \| \leq 1$。此外，由于$\mu_n \leq 2^n \| \mu_n \| \cdot \mu$，关系$\mu(N) = 0$意味着$\mu_n(N) = 0$对于所有$n$；相反，如果$N$是集合，对于所有$\mu_n$来说可以忽略不计，那么对于$\mu$来说，它在局部可以忽略不计

（§2, No. 2，第 1 条命题的 Cor.2），因此 $\mu$ 可忽略不计，因为 $\mu$ 有界（§1, No. 2，第 7 条命题的 Cor.2）。

### 7. 外国人措施

给定 $T$ 上的两个实测度 $\rho, \sigma$，回想一下，如果 $\mathscr{M}(T)$ 中的 $\inf(|\rho|, |\sigma|) = 0$（第 II, §1, No. 1），则$\rho$ 和 $\sigma$ 被认为是（彼此）陌生的。与给定度量不同的实际度量已知为形式频带（Ch. II, §1, No. 5，Th. 1）。此定义可以立即扩展到复杂措施的情况。

#### 定义 4 {#int-v-s5-def-4 .statement tag=093F}

*有人说，$T$上的复杂测度$\theta$集中在$T$的子集$M$上，或者$M$携带$\theta$，如果$\mathbf{C}M$对于$\theta$局部可忽略不计。*

当且仅当集合$M$携带$\theta$时，它携带$|\theta|$。相当于说$M$携带$\theta$，或者$M$是$\theta$可测且$\theta = \varphi_M \cdot \theta$。如果$\theta$集中在$M$，则基$|\theta|$的每个小节都集中在$M$。

#### 命题 13 {#int-v-s5-prop-13 .statement tag=093G}

*在阶中，$T$上的两个复杂测度$\rho$和$\sigma$彼此陌生，$T$中存在两个不相交的集合$R$和$S$使得$\rho$是充分必要的集中在$R$，$\sigma$集中在$S$； $R$ 和 $S$ 可以被认为是普遍可测的。*

集合$\mu = |\rho|$、$\nu = |\sigma|$、$\lambda = \mu + \nu$；由于$\mu$和$\nu$以上由$\lambda$为界，因此存在两个局部$\lambda$可积函数$u$和$v$（可以假设其可以通过§3, No. 4，第7条命题普遍测量），使得$\mu = u \cdot \lambda$，$\nu = v \cdot \lambda$。然后

$$
\inf(|\rho|, |\sigma|) = \inf(\mu, \nu) = \inf(u, v) \cdot \lambda
$$

（No. 2，Cor. of Prop. 2）。令$A$（分别为$B$）为$t \in T$的集合，使得$u(t) > 0$和$v(t) = 0$（分别为$u(t) = 0$和$v(t) > 0$）。如果$\rho$和$\sigma$是外来的，那么$\inf(u, v) = 0$在本地$\lambda$-几乎无处不在（No. 3，第3号命题的Cor.2），因此不相交的普遍可测集合$A$和$B$携带分别为$\mu$和$\nu$。相反，假设$\mu$和$\nu$分别由不相交的、集合、$R$和$S$携带； $\varphi_R$ 可测量$\mu = u \cdot \lambda$ 和 $\mu = \varphi_R \cdot \mu$。根据No. 4第8条，函数$u' = u \varphi_R$是$\lambda$可测量的，并且$\mu = u' \cdot \lambda$。类似地，如果$v' = v \varphi_S$则$\nu = v' \cdot \lambda$；一个结论，通过评论$\inf(u', v') = 0$（No. 2，Prop.2的Cor.）。

#### 推论 1 {#int-v-s5-prop-13-cor-1 .statement tag=093H}

*对于$T$上的每个实际测量$\nu$，存在两个不相交的集合$M, N$，分别携带$\nu^+$和$\nu^-$。*

必须注意不要混淆支持$\nu$措施的概念和集中$\nu$的集合。 $\nu$ 的支撑 S 是最小的闭合集合承载 $\nu$（第 III, § 2, No. 2 第 2 章和第 IV, §2, No. 2 第 5 章）。然而，可能存在 S 的子集与 S 不同并携带 $\nu$。更一般地，对于具有相同支持的两项积极措施$\mu$和$\nu$，可以拥有$\inf(\mu, \nu) = 0$（示例5）。

注还有，集合携带$\nu$的交是点$t \in T$的集合，使得$|\nu|(\{t\}) > 0$，并且它可以是空的（例如，在勒贝格测度的情况下）；因此，一般不存在最小的集合携带$\nu$。

#### 推论 2 {#int-v-s5-prop-13-cor-2 .statement tag=093I}

— 令$\rho$和$\sigma$为两个外来复测度，并令$\rho'$和$\sigma'$分别为允许相对于$\rho$和$\sigma$的密度的两个复测度；那么$\rho'$和$\sigma'$是外星人。

#### 推论 3 {#int-v-s5-prop-13-cor-3 .statement tag=093J}

— 设$\rho$和$\sigma$为两个外来复测度；然后$|\rho + \sigma| = |\rho| + |\sigma|$。

用$v$（或$w$）表示绝对值值 1 的普遍可测函数，使得$\rho = v \cdot |\rho|$（或$\sigma = w \cdot |\sigma|$）（第2条的Cor.3），并用A表示普遍可测的集合 $\rho$，使得$B = \mathbf{C}A$携带$\sigma$（提案13）；然后还有$\rho + \sigma = (v \varphi_A + w \varphi_B) \cdot (|\rho| + |\sigma|)$。由于函数 $v \varphi_A + w \varphi_B$ 的绝对值等于 1，推论由命题 2 得出。

#### 定理 3（勒贝格）{#int-v-s5-thm-3 .statement tag=093K}

— T 上的每个复杂测度 $\theta$ 都可以用一种且仅一种方式写成形式 $\theta = g \cdot \mu + \theta'$，其中 $g$ 是本地 $\mu$ 可积的，$\theta'$ 是与 $\mu$ 不同的测度。然后$|\theta| = |g| \cdot \mu + |\theta'|$。

当 $\theta$ 为正时，这立即从 F. Riesz (Ch. II, §1, No. 5, Th. 1) 的定理得出，应用于 T 上实际测量的完全晶格有序空间 $\mathscr{M}(T)$，以及在考虑到 Cor 的情况下，应用于此空间中 $\mu$ 生成的带。 No. 5 中的 2 个，Th。 2；此外，$\theta'$和$g \cdot \mu$则为正，这意味着$g$局部为正$\mu$——几乎无处不在（第3条的Cor.3）。为了处理$\theta$不是正数的情况，集合$\nu = |\theta|$、$\nu = f \cdot \mu + \nu'$（其中$f$是正数，并且$\nu'$和$\mu$互不相容），以及$\theta = v \cdot \nu$，其中$v$是普遍可测的绝对值 1 的函数（第 2 条的 Cor. 3）。然后我们有（命题8）$\theta = g \cdot \mu + \theta'$，以及$g = v f$（因此$|g| = f$）和$\theta' = v \cdot \nu'$（因此命题2的$|\theta'| = \nu'$）； Cor. 措施$\theta'$ 和$\mu$ 是互不相容的。提案 13 的 2。只需建立唯一性或分解。因此，假设$\theta = g \cdot \mu + \theta' = g_1 \cdot \mu + \theta'_1$，其中$\theta'$和$\theta'_1$与$\mu$不相容； $|\theta' - \theta'_1|$ 的边界为 $|\theta'| + |\theta'_1|$，因此 $\theta' - \theta'_1$ 与 $\mu$ 不相容，因此也与 $(g_1 - g) \cdot \mu$ 不相容。 关系$\theta' - \theta'_1 = (g_1 - g) \cdot \mu$则意味着两个成员是零，从而证明了唯一性。

回想一下（No. 5、Th.2 和 Scholium），空间 $L^1_{loc}(T, \mu; \mathbf{C})$ 可以（通过映射 $g \mapsto g \cdot \mu$）与子空间或 $\mathscr{M}_\mathbf{C}(T)$ 一起识别。根据此约定，定理 3 采用以下形式：

#### 推论 {#int-v-s5-n7-cor-1 .statement tag=093L}

— *在空间 $L^1_{\text{loc}}(T, \mu; \mathbf{C})$ 上存在空间 $\mathscr{M}_\mathbf{C}(T)$ 的投影算子 p，其核 $\overline{p}^{-1}(0)$ 是集合与 $\mu$ 不同的复杂测度，使得*

$$
|\theta| = |p(\theta)| + |\theta - p(\theta)|,\quad p(|\theta|) = |p(\theta)|
$$

*对于每一个复杂的测量$\theta$。*

如果 $p$ 被限制为集合有界度量，则可在空间 $L^1_\mathbf{C}(T, \mu)$ 上获得空间 $\mathscr{M}_\mathbf{C}^1(T)$ 的投影算子 $p^1$； 关系 $\| \theta \| = |\theta|(1)$ 意味着$\| \theta \| = \| p^1(\theta) \| + \| \theta - p^1(\theta) \|$ 对于每个有界复数测度 $\theta$。

### 8. 应用：I。 空间 $L^p$ 的对偶性

我们在这里只处理真实的空间$L^p$的情况。

回想一下，两个数 $p, q$ 使得 $1 \leq p \leq +\infty$、$1 \leq q \leq +\infty$、$1/p + 1/q = 1$ 被称为 *共轭指数*（第 IV, §6, No. 4 章）。每函数 $g \in \mathscr{L}^q$ 定义 $L^p$ 上有一个连续的线性形式 $\theta_g$，由经过到商从 $\mathscr{L}^p$ 上的线性形式 $f \mapsto \int fg\,d\mu$ 开始获得，并且有一个$N_q(g) = \| \theta_g \|$（第 IV, §6, No. 4 章，第 3 号提案的Cor.）。 经过到商，因此从映射$g \mapsto \theta_g$推出$L^q$的等距线性映射$\varphi$到$L^p$的对偶$(L^p)'$。我们将证明，对于 $1 \leq p < +\infty$，$\varphi$ 映射 $L^q$ *到* $(L^p)'$，这样我们今后就可以将认同 Banach 空间 $L^q$ 与 Banach 空间 $(L^p)'$ 通过同构 $\varphi$。其他项中所述：

#### 定理 4 {#int-v-s5-thm-4 .statement tag=093M}

— *令 p 和 q 为两个共轭指数，使得 $1 \leq p < +\infty$。 $\mathscr{L}^p(T, \mu)$上的每个连续线性形式都是型$f \mapsto \int fg\,d\mu$，其中g是$\mathscr{L}^q(T, \mu)$中的函数，而$L^q$中的类是明确定义的。*

令$\theta$为$\mathscr{L}^p$上连续的线性形式；因而，对于每个函数$f \in \mathscr{L}^p$，存在数$a \geq 0$这样的$|\theta(f)| \leq a \cdot N_p(f)$。 考虑$\theta$对紧支持连续函数空间$\mathscr{K}(T)$的限制：对于T的每个紧子集K和每个函数$f \in \mathscr{K}(T, K)$（K中包含的紧支持连续函数空间），有$N_p(f) \leq (\mu(K))^{1/p} \| f \|$；因而，由$\mathscr{L}^p$的拓扑在$\mathscr{K}(T, K)$上导出的拓扑比一致收敛的拓扑更粗糙，并且$\theta$对每个$\mathscr{K}(T, K)$的限制对于后者拓扑来说是连续的。 这意味着 $\theta$ 到 $\mathscr{K}(T)$ 的限制是*实际度量* $\nu$（第 1 章） III, §1, No. 3，默认。 2）。

让我们证明对于 $\mathscr{K}(T)$ 中的每个函数 $f$，$|\nu|(|f|) \leq a \cdot N_p(f)$。只要证明公式对于$f \geq 0$就足够了。现在，对于$\mathscr{K}(T)$中的每个函数$\psi$使得$|\psi| \leq f$，我们有
$$
|\nu(\psi)| \leq a \cdot N_p(\psi) \leq a \cdot N_p(f);
$$
我们的断言源自第1章中给出的度量的绝对值的表达式。 III, §1, No. 6、公式 (12)。 关系$|\nu|(|f|) \leq a (\mu(|f|^p))^{1/p}$扩展立即针对$f$是紧集的特征函数的情况，通过通向下包络线的方式，然后暗示每个$\mu$-可忽略的紧集是$\nu$-可忽略的，因而 $\nu$ 是一个度量*与基* $\mu$ (No. 5, Th. 2)。

因而，存在一个局部 $\mu$ 可积正函数 $h_1$，使得对于每个函数 $f \in \mathscr{K}(T)$ 都有 $|\nu|(f) = \int f h_1 d\mu$。让我们证明$h_1$在局部几乎处处都等于$\mathscr{L}^q$中的函数。如果$\mathscr{K}(T)$中的函数$f \geq 0$使得$N_p(f) \leq 1$，则$\int f h_1 d\mu = |\nu|(f) \leq a$。对于具有紧凑支持的 T 的每个连续映射 $f_0$ 到$[0,1]$，因此我们有 $\sup \int (f_0 h_1) f d\mu \leq a$，因为 $f$ 在 $\mathscr{K}(T)$ 中运行超过函数 $\geq 0$ 的集合，从而得到 $N_p(f) \leq 1$。由此推断，通过第 1 章的公式 (11)。 IV, §6, No. 4，那个$N_q(f_0 h_1) \leq a$。由此可见，当 K 时，$\sup_{K} N_q(\varphi_K h_1) \leq a$ 会超过 T 的紧凑子集的集合，这证明了我们的断言（§1，命题 9）。

令 $v$ 为绝对值 1 的普遍可测（实数）函数，使得 $\nu = v \cdot |\nu|$（Th. 2 的 Cor. 3）并令 $g = v h_1$；然后$\nu = g \cdot \mu$，$g$属于到$\mathscr{L}^q$。对于每个函数$f \in \mathscr{K}(T)$，我们有$\theta(f) = \nu(f) = \int f g d\mu$。其他字中，$\mathscr{K}(T)$上连续的线性形式$\theta$和$\theta_g$重合；因而，它们在 $\mathscr{L}^p$ 上相等，因为 $\mathscr{K}(T)$ 在 $\mathscr{L}^p$ 中是稠密的，这完成了证明。

#### 推论 {#int-v-s5-n8-cor-1 .statement tag=093N}

— *对于每个数 p 使得 $1 < p < +\infty$，Banach 空间 $L^p(T, \mu)$ 是自反的。*

一般来说，$L^\infty$的对偶与$L^1$不同构，因而$L^1$和$L^\infty$不是自反的（Exer.10）。我们将描述$L^\infty$上的连续线性形式，从$\mathscr{L}^\infty$上的线性形式$g \mapsto \int f g d\mu$到商，其中$g \in \mathscr{L}^1$。

有序的向量空间 $L^\infty(T, \mu)$，即 $L^1_{loc}(T, \mu)$ 的子空间，是*完全格序的*；因为，如果$(f_\alpha)$是$\mathscr{L}^\infty$中的正函数族，其类$(\dot{f}_\alpha)$的集合在$L^\infty$中上界，则存在一个$a \geq 0$，使得$N_\infty(f_\alpha) \leq a$对于所有$\alpha$。由于 $L^1_{loc}(T, \mu)$ 是完全格序的，$(\dot{f}_\alpha)$族在$L^1_{loc}(T, \mu)$中承认一个上等$\dot{h}$；但由于每一个$\alpha$都有$\dot{a} \geq \dot{f}_\alpha$，我们有$\dot{h} \leq \dot{a}$，因而$N_\infty(h) \leq a$，从而我们的断言。

#### 命题 14 {#int-v-s5-prop-14 .statement tag=093O}

— *在阶中，$\mathscr{L}^\infty$上的正线性形式$\theta$为型$f \mapsto \int f g d\mu$，其中$g \in \mathscr{L}^1$，有充分必要*，*对于每个递增定向家庭$(f_\alpha)_{\alpha \in A}$的正函数 $\mathscr{L}^\infty$，其类$(\dot{f}_\alpha)_{\alpha \in A}$的集合在$L^\infty$上有界，并承认$\dot{h}$为其空间中的上等，有

$$
\theta(h) = \sup_{\alpha \in A} \theta(f_\alpha).
$$

让我们首先证明条件是必要的。测度$h \cdot \mu$是测度$f_\alpha \cdot \mu$（No. 5，Scholium）的集合在$\mathscr{M}(T)$中的至高；因此（第II, §2, No. 2），对于$\mathscr{K}(T)$中的每个函数$\varphi \geq 0$，我们有$\int h \varphi \, d\mu = \sup_{\alpha \in A} \int f_\alpha \varphi \, d\mu$。如果现在$a$是数$\geq 0$，使得$N_\infty(f_\alpha) \leq a$对于所有$\alpha \in A$（这意味着$N_\infty(h) \leq a$），那么对于每个$\varepsilon > 0$，都存在一个$\varphi \in \mathscr{K}(T)$，使得$\varphi \geq 0$和$N_1(g - \varphi) \leq \varepsilon$，从中我们推断$\int f_\alpha |g - \varphi| \, d\mu \leq a \varepsilon$ 适用于所有 $\alpha \in A$ 和 $\int h |g - \varphi| \, d\mu \leq a \varepsilon$。从$\sup_{\alpha \in A} \int f_\alpha g \, d\mu \leq \int h g \, d\mu$开始，这就证明了这个不等式的两个成员是相等的。

为了确定条件就足够了，我们将使用以下引理：

#### 引理 4 {#int-v-s5-lem-4 .statement tag=093P}

1° *令 $f$ 为$T$ 上的下半连续且有界正函数。那么$L^\infty$中的类$\dot{f}$是类$\dot{\varphi}$的集合的上确界，其中$\varphi$超过$\mathscr{K}(T)$中的函数的集合，使得$0 \leq \varphi \leq f$.*

2° *令 $f$ 为 $T$ 上可测量且有界的正函数。那么$L^\infty$中的类$\dot{f}$是类$\dot{\psi}$的集合的下确界，其中$\psi$越过下半连续的集合并且在$T$上有界函数为$\geq f$.*

1° 设 $\mathscr{L}^\infty$ 中的 $f'$ 为函数，使得 $\dot{f}'$ 为函数 $\varphi$ 的类 $\dot{\varphi}$ 集合 $L^\infty$ 中的上界$\mathscr{K}(T)$使得$0 \leq \varphi \leq f$；显然$\dot{f}' \leq \dot{f}$。令$U$为$T$的相对紧凑的开子集；对于 $\mathscr{K}(T)$ 中的每一个函数 $h$，使得 $0 \leq h \leq f \varphi_U$ 到定义，本地几乎所有地方都有 $h(t) \leq f'(t)$，因此几乎所有地方都有 $h(t) \leq f'(t) \varphi_U(t)$；由此可见$\int h \, d\mu \leq \int f' \varphi_U \, d\mu$。然而，由于$f \varphi_U$是下半连续的，$\int f \varphi_U \, d\mu = \sup \int h \, d\mu$，其中$h$在$\mathscr{K}(T)$中超过函数的集合，使得$0 \leq h \leq f \varphi_U$（第IV, §1, No. 1，定义1）；因此

$$
\int f \varphi_U \, d\mu \leq \int f' \varphi_U \, d\mu,
$$

并且由于 $f' \varphi_U \leq f \varphi_U$ 几乎无处不在，必然 $f \varphi_U = f' \varphi_U$ 几乎无处不在，从而 $f = f'$ 局部几乎无处不在。

2° 设$f'$为$\mathscr{L}^\infty$中的函数，使得$\dot{f}'$为有界下半连续函数$\psi$的类$\dot{\psi}$的集合$L^\infty$中的下确界，并且$\geq f$；然后$\dot{f}' \geq \dot{f}$。设$K$是$T$的紧子集；对于每个有界的下半连续函数$h$和$\geq f \varphi_K$，令$\overline{h}$为函数等于$K$上的$h$以及$T - K$上的$\|f\| + \|h\|$。那么 $\overline{h}$ 是下半连续的，$\geq f$，因此几乎处处局部都有定义 $\overline{h}(t) \geq f'(t)$；由此可见，$h(t) \geq f'(t)\varphi_K(t)$几乎无处不在，从而$\int h d\mu \geq \int f'\varphi_K d\mu$。但是 $\int f\varphi_K d\mu = \inf \int h d\mu$，其中 $h$ 超过有界的下半连续函数的集合和 $\geq f\varphi_K$（第 IV, §1, No. 3，定义 3）；因此

$$
\int f\varphi_K d\mu \geq \int f'\varphi_K d\mu,
$$

由于 $f\varphi_K \leq f'\varphi_K$ 几乎无处不在，必然 $f\varphi_K = f'\varphi_K$ 几乎无处不在，从而 $f = f'$ 局部几乎无处不在。

引理已被证明，令$\theta$为第14条命题叙述中$\mathscr{L}^\infty$满足条件的正线性形式。$\theta$到空间$\mathscr{K}(T)$的限制是对$T$采取积极措施$\nu$。我们将证明，对于每一个正函数 $f \in \mathscr{L}^\infty(T, \mu)$，都有 $\theta(f) = \nu^*(f)$。首先假设 $f$ 是下半连续（且有界）；通过引理 4，$f$是类$\dot{\varphi}$的递增有向集合的上等，其中$\varphi$在$\mathscr{K}(T)$中超过函数的有向集合$\Phi$，这样那个$0 \leq \varphi \leq f$。由于假设$\theta(f) = \sup_{\varphi \in \Phi} \theta(\varphi)$和$\nu^*(f) = \sup_{\varphi \in \Phi} \nu(\varphi)$定义，我们的断言在这种情况下得到了证明。其次，假设$f$是$\mu$可测且有界；然后，通过定义，$\nu^*(f) = \inf_{\psi \in \Psi} \nu^*(\psi)$，其中$\psi$运行在有界的下半连续函数和$\geq f$的递减有向集合$\Psi$上。如果$a \geq \|f\|$则，叙述应用假设到函数$a - \psi$类递增有向集合，其中$\psi \in \Psi$和$\psi \leq a$，可见，凭借引理，即$\theta(f) = \inf_{\psi \in \Psi} \theta(\psi)$，因此确实是$\theta(f) = \nu^*(f)$。特别是，对于每个$\mu$-可忽略的函数$f \geq 0$，一个人有$\theta(f) = 0$，因而$\nu^*(f) = 0$，因而（No. 5，Th.2）$\nu$是一个度量*与基*$\mu$；此外，$\nu^*(1) = \theta(1) < +\infty$，因而（Th.1的Cor.）$\nu = g \cdot \mu$与$g \in \mathscr{L}^1(T, \mu)$。最后，由于每个$\mu$可测函数都是$\nu$可测，因此每个正函数$f \in \mathscr{L}^\infty(T, \mu)$都是$\nu$可积和$\int fg d\mu = \nu^*(f) = \theta(f)$，从而完成证明。

第 14 号提案中的一个结论型 $f \mapsto \int fg d\mu$ 的 $\mathscr{L}^\infty$ 上的线性形式，其中 $g \in \mathscr{L}^1$，是差 $\theta_1 - \theta_2$，其中 $\theta_1$ 和 $\theta_2$ 为正线性形式提案 14 的满足条件。

### 9. 应用：II。 函数措施

令 $\mu_1, \mu_2, \ldots, \mu_n$ 为 T 上的实测度，并令 $u(x_1, \ldots, x_n)$ 为有限数值函数，在 $\mathbf{R}^n$ 上定义，且为正齐次，即 (Ch. I, §1, No. 1)，使得

$$
u(\alpha x_1, \ldots, \alpha x_n) = \alpha u(x_1, \ldots, x_n)
$$

对于每个标量$\alpha \geqslant 0$。 T 上存在正测度 $\lambda$，使得 $|\mu_i| \leqslant \lambda$ 适合 $1 \leqslant i \leqslant n$（例如，和 $\sum_{i=1}^n |\mu_i|$）。令 $\lambda$ 和 $\lambda'$ 为 T 上的两个此类测度。可以写为 $\mu_i = f_i \cdot \lambda = f'_i \cdot \lambda'$，其中 $f_i$（分别为 $f'_i$）是可测的，并且本质上有界于测度 $\lambda$（分别为 $\lambda'$）（No. 5，Th.2）。我们将建立以下结果：*在阶中，数值函数$u(f_1, \ldots, f_n)$对于$\lambda$可局部可积，函数$u(f'_1, \ldots, f'_n)$对于$\lambda'$可局部可积是必要且充分的，在这种情况下*

$$
u(f_1, \ldots, f_n) \cdot \lambda = u(f'_1, \ldots, f'_n) \cdot \lambda'.
$$

从$|\mu_i| \leqslant \inf(\lambda, \lambda')$开始，我们可以将自己限制在$\lambda \leqslant \lambda'$的情况。然后$\lambda = g \cdot \lambda'$，其中$g$是$\lambda'$可测量的函数，使得$0 \leqslant g \leqslant 1$（No. 5，Th.2）； 从而（No. 4，提案 8）

$$
\mu_i = f_i \cdot (g \cdot \lambda') = (f_i g) \cdot \lambda';
$$

由此可见（No. 3，第 3 条命题第 2 条），对于 $\lambda'$，$f_i g$ 几乎在任何地方都等于 $f'_i$。因而，通过 (12)，

$$
u(f'_1, \ldots, f'_n) = u(f_1 g, \ldots, f_n g) = u(f_1, \ldots, f_n) g
$$

当地几乎所有地方都只需$\lambda'$。在阶中，$u(f'_1, \ldots, f'_n)$ 是局部 $\lambda'$ 可积的，因而，$u(f_1, \ldots, f_n) g$ 对于 $\lambda'$ 是局部可积的，因而（No. 4，命题 8）$u(f_1, \ldots, f_n)$ 对于 $\lambda$ 是局部可积的；然后（No. 4，提案 8）

$$
u(f'_1, \ldots, f'_n) \cdot \lambda' = (u(f_1, \ldots, f_n) g) \cdot \lambda' = u(f_1, \ldots, f_n) \cdot \lambda.
$$

因而，测度$u(f_1, \ldots, f_n) \cdot \lambda$仅取决于测度$\mu_1, \ldots, \mu_n$和函数$u$；它也表示为$u(\mu_1, \ldots, \mu_n)$。因而，每当 $u$ 是正齐次函数时，就定义该测度，使得对于所有 $|\mu_i|$ 的正测度 $\lambda$ 即上界，$u(f_1, \ldots, f_n)$ 是局部 $\lambda$ 可积的，其中 $f_i$ 表示密度 $\mu_i$相对于$\lambda$。请注意，当 $u$ 是正齐次且*连续*时，条件得到满足：对于，则有
$$
|u(x_1, \ldots, x_n)| \leq a(|x_1| + |x_2| + \cdots + |x_n|)
$$
（*u* 的边界在 $(0, \ldots, 0)$ 的足够小的邻域内），并且由于 $u(f_1, \ldots, f_n)$ 是 $\lambda$ 可测的（章节 IV, §5, No. 3，Th. 1），因此根据可积性准则，它是局部 $\lambda$ 可积的（章节 IV, §5, No. 6，Th. 5）。

令$u_1, \ldots, u_p$是在$\mathbf{R}^n$上定义的正齐次数值函数，使得$p$函数$g_k = u_k(f_1, \ldots, f_n)$$(1 \leq k \leq p)$是局部$\lambda$可积的。令 $v$ 为在 $\mathbf{R}^p$ 上定义的正齐次数值函数，使得 $v(g_1, \ldots, g_p)$ 是局部 $\lambda$ 可积的。 集合
$$
w(x_1, \ldots, x_n) = v(u_1(x_1, \ldots, x_n), \ldots, u_p(x_1, \ldots, x_n)).
$$
那么，函数$w$是正齐次的，$w(f_1, \ldots, f_n)$是局部$\lambda$可积的，并且通过定义，
$$
w(\mu_1, \ldots, \mu_n) = v(u_1(\mu_1, \ldots, \mu_n), \ldots, u_p(\mu_1, \ldots, \mu_n)).
$$

在函数$x^+, x^-, |x|, x+y, \inf(x, y), \sup(x, y)$的特殊情况下，刚才描述的过程定义的措施分别为重合，以及那些已标记为$\mu^+, \mu^-, |\mu|, \mu+\nu, \inf(\mu, \nu), \sup(\mu, \nu)$的措施；这是从 Cor 立即得出的。 No. 2 的第 2 号提案。如果$\mu$和$\nu$是两个实度量，并且$\theta = \mu + i\nu$，则$|\theta| = \sqrt{\mu^2 + \nu^2}$；例如，令 $\lambda$ 为$\geq 0$ 的测度，即 $|\mu|$ 和 $|\nu|$ 的上界，并令 $f, g$ 为$\lambda$ 局部可积函数，使得 $\mu = f \cdot \lambda,\ \nu = g \cdot \lambda$；那么
$$
\sqrt{\mu^2 + \nu^2} = \sqrt{f^2 + g^2} \cdot \lambda,
$$
$$
\theta = (f + ig) \cdot \lambda,\ \text{therefore (No. 2, Prop. 2)}\ |\theta| = \sqrt{f^2 + g^2} \cdot \lambda.
$$
该方法可以应用于$\mathbf{R}^n$中曲线的正齐次函数$(x_1^2 + \ldots + x_n^2)^{1/2}$到定义长度。

### 10. 分散措施；原子措施

#### 定义 5 {#int-v-s5-def-5 .statement tag=093Q}

*如果* $|\theta|(\{t\}) = 0$ *对于每个* $t \in T$，则 T 上的测量 $\theta$ 被认为是扩散的。

#### 例 {#int-v-s5-n10-exa-1 .statement tag=093R}

— $\mathbf{R}$ 上的勒贝格测度是分散的（第 IV, §1, No. 3，*注* 1）。

说$\theta$是$T$上的分散测度相当于说，每个具有有限补集的集合都携带$|\theta|$，或者再次说$|\theta|$与每个点测度都是陌生的。因此，漫反射测量形式 $\mathscr{M}(T)$ 中的一个频带（Ch. II, §1, No. 5，Th. 1）。

回想一下（第 III, §1, No. 3 章），$T$ 上的复数测度 $\rho$ 被称为“原子”，如果它是形式 $\sum_{t \in T} \alpha(t) \varepsilon_t$，其中 $\alpha$ 是 $T$ 上的复数函数，使得对于每个紧凑，$\sum_{t \in K} |\alpha(t)| < +\infty$ $T$的子集$K$，表示族$(\alpha(t) \varepsilon_t)_{t \in T}$是可和的（§2, No. 1，注2）。然后它是从Cor之后的注开始的。 3 Th。 No. 5 中的 2 个$|\rho| = \sum_{t \in T} |\alpha(t)| \varepsilon_t$。这些公式中出现的函数$\alpha$是唯一确定的，因为$\alpha(t) = \rho(\{t\})$。原子测量和扩散测量是互不相容的。

#### 命题 15 {#int-v-s5-prop-15 .statement tag=093S}

*$T$上的每个复杂测度$\sigma$都可以用一种且仅一种方式写成形式$\rho + \theta$，其中$\rho$是原子测度，$\theta$是扩散测度；那么就有 $|\sigma| = |\rho| + |\theta|$.*。

分解的唯一性是显而易见的，因为$\rho$是原子的，$\theta$是扩散的，必然是$\rho = \sum_{t \in T} \rho(\{t\}) \varepsilon_t = \sum_{t \in T} \sigma(\{t\}) \varepsilon_t$和$\theta = \sigma - \rho$。为了建立存在性，只要观察到每一个紧集$K$都有$\sum_{t \in K} |\sigma(\{t\})| \leq |\sigma|(K) < +\infty$，这样就可以集合$\sum_{t \in T} \sigma(\{t\}) \varepsilon_t = \rho$。措施 $\sigma - \rho$ 显然是分散的，关系 $|\sigma| = |\rho| + |\sigma - \rho|$ 立即从 Cor 开始。 No. 7第13号提案第3条。

人们观察到，这个证明表明，如果$\sigma$由集合$M$携带，并且如果每个$t \in M$都有$|\sigma|(\{t\}) > 0$，那么$\sigma$是*原子的*。

### 习题 {#int-v-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
