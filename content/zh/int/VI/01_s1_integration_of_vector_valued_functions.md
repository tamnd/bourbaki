---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 1
section_title: Integration of vector-valued functions
lang: zh
source: int-i-vi
pdf_pages: 0392-0409, 0447-0453
extraction: ocr
subsections:
    - "no": 1
      title: Scalarly essentially integrable functions
      page: 2
      pdf_page: 393
    - "no": 2
      title: Properties of the integral of a scalarly essentially integrable function
      page: 5
      pdf_page: 396
    - "no": 3
      title: Integrals of operators
      page: 7
      pdf_page: 398
    - "no": 4
      title: The property (GDF)
      page: 9
      pdf_page: 400
    - "no": 5
      title: Measurable mappings and scalarly measurable mappings
      page: 12
      pdf_page: 403
    - "no": 6
      title: 'Applications: I. Extension of a continuous function to a space of measures'
      page: 13
      pdf_page: 404
    - "no": 7
      title: 'Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators'
      page: 15
      pdf_page: 406
statements: 34
exercises: 27
content_sha256: c3eb2455542c6e97c0fd61b6fc8594bd18de65701de3bf85ee88fdf69f288474
translated_from: content/en/int/VI/01_s1_integration_of_vector_valued_functions.md
translation_method: google
source_content_sha256: 9798f2a69885491f713db436a4833ff226e18b3becfed322106b65f6897d576a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: d29fb99c443d7697a2ab2d67d8cfac9e6fcc13ddee43cd128811a86b1611cf51
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。向量值函数的积分

在整个截面中，$\mu$ 表示 T 上的正测度，F 是 Hausdorff 在 $\mathbf{R}$ 上局部凸向量空间。对于 T 的每个映射 f 到 F 中，以及 F 的对偶 $F'$ 的每个元素 $z'$，我们用 $\langle f, z' \rangle$ 或 $\langle z', f \rangle$ 表示 T 上的数值函数 $z' \circ f$。 我们可以说 f 有性质 $P$ *标量*如果对于每个$z' \in F'$，$\langle z', f \rangle$有性质$P$。对于例，我们可以说$f$*本质上是$\mu$可积*，如果对于每个$z' \in F'$，$\langle z', f \rangle$本质上是$\mu$可积。\脚注{特殊情况$F = \mathscr{M}(X)$（$X$是局部紧凑的） 空间），配备了模糊的拓扑$\sigma(\mathscr{M}(X), \mathscr{K}(X))$，产生了“基本上可积$\mu$可积”的概念，对于映射$f : T \to \mathscr{M}_+(X)$，在第1章中定义。 V, §3, No. 1.}

注在这个定义中，$F$的拓扑仅通过$F$的对偶$F'$中介进行干预。如果函数 $f$ 具有性质 $P$ 标量，那么当 $F$ 的拓扑被替换为任意 Hausdorff 局部凸拓扑时，它再次具有性质 $P$ 标量，且与之间的对偶性兼容$F$ 和 $F'$。

### 1. 本质上是标量可积函数

如果 $f$ 是 $T$ 到 $F$ 的标量本质上 $\mu$ 可积映射，则映射 $z' \mapsto \int \langle f(t), z' \rangle d\mu(t)$ 是 $F'$ 上的线性形式，即代数对偶 ${F'}^*$ 的元素。

#### 定义 1 {#int-vi-s1-def-1 .statement tag=098E}

*一个调用* $f$相对于$\mu$的积分，*并表示为* $\int f d\mu$ *或* $\int f(t) d\mu(t)$，*元素 of* ${F'}^*$ *定义为*
$$
\left\langle z', \int f d\mu \right\rangle = \int \langle z', f \rangle d\mu
$$
*对于所有人*$z' \in F'$。

如果 $f$ 在紧支持下连续，则它是标量可积的且 Def. 1 重合与第 1 章中给出的 $f$ 积分的定义。 III, §3, No. 1。另一方面，如果 $F$ 是 Banach 空间并且 $f$ 本质上可积（Ch. V, §1, No. 3，Def. 3），则 $f$ 本质上可积且 Def.3。 1 重合与 $f$ 积分的定义在章 V 中给出（第 V, §1, No. 3 和第 IV, §4, No. 2，第 1 章的 Cor. 1）。

#### 例 {#int-vi-s1-n1-exa-1 .statement tag=098F}

— 设$X$为$T$的局部紧凑空间、$t \mapsto \lambda_t$映射到$X$上的测度空间$\mathscr{M}(X)$。说家庭$t \mapsto \lambda_t$是$\mu$充足意味着它由积极的措施组成，并且映射$t \mapsto \lambda_t$对于拓扑$\sigma(\mathscr{M}(X), \mathscr{K}(X))$来说基本上是$\mu$可积和$\mu$可测量。\脚注{这是章 5 第一版中的“μ-足够”的定义（第 V 章，第 1 版，§3, No. 1，定义 1）。在第二版中，前面的章是翻译，项“μ-足够”定义是一个较弱（更一般）的概念（第V, §3, No. 1，定义1）；更准确地说，一个标量本质上$\mu$可积的积极措施族$t \mapsto \lambda_t$在章V的第一版意义上是$\mu$充足，当且仅当它在第二版意义上是$\mu$充足并且模糊地$\mu$-可测量，即 $\mu$-可测量 $\sigma(\mathscr{M}(X), \mathscr{K}(X))$（第 V, §3, No. 1，提案 2 b））。当$X$的拓扑具有可数基时，两个定义是等价的（*同上*。Prop.2c）），章VI（§3）中的应用就是这种情况；因而，对于章的其余部分，“μ-足够”的两种解释以及对第1章第一版的引用之间没有区别。 V 已被第二版中最接近的等效项取代。}

关于 $\mu$ 的积分是第 1 章中表示为 $\int \lambda_t\, d\mu(t)$ 的度量。 V, §3, No. 1。

#### 注 1 {#int-vi-s1-n1-rem-1 .statement tag=098G}

如果 F 是有限维的，则 T 到 F 中的每个标量本质上可积的映射本质上都是可积的（Ch. V, §1, No. 3）。然而，在一般情况下，在紧凑的空间 T 上可忽略的标量函数甚至可能无法实现 $\mu$ 可测量（例 12）。

#### 注 2 {#int-vi-s1-n1-rem-2 .statement tag=098H}

很明显，f 的积分仅取决于 f 的类将 T 的映射空间模到 F 中，其标量局部 $\mu$ 可忽略不计。 注局部可忽略的标量函数 g 不一定几乎无处不在零（例 12）。然而，当 F' 序列 $(\mathbf{z}'_n)$ 中存在对于拓扑 $\sigma(F', F)$ 来说是密集的时，情况确实如此：因为，如果 $H_n$ 是点 $t \in T$ 的局部可忽略的集合，使得$\langle g(t), \mathbf{z}'_n \rangle \neq 0$，并 $H_n$ 的 H 局部可以忽略不计，并且对于每个 $t \notin H$，对于所有 n，从而 $g(t) = 0$，都有 $\langle g(t), \mathbf{z}'_n \rangle = 0$。

令 u 为 F 的连续线性映射到 Hausdorff 局部凸空间 G；它的转置$^t u$是$G'$到$F'$的线性映射，（代数）转置$^t(^t u)$是${F'}^*$到${G'}^*$的线性映射到扩展u，我们将再次表示为u。有了这个约定：

#### 命题 1 {#int-vi-s1-prop-1 .statement tag=098I}

— *如果 f 是 T 到 F 中的映射，并且本质上是 $\mu$ 可积，那么映射 $u \circ f$ 本质上是 $\mu$ 可积，并且*
$$
\int (u \circ f)\, d\mu = u \left( \int f\, d\mu \right).
$$
对于每个$\mathbf{z}' \in G'$、$\langle \mathbf{z}', u \circ f \rangle = \langle ^t u(\mathbf{z}'), f \rangle$、从而，第一个断言；第二个来自公式
$$
\left\langle \mathbf{z}', \int (u \circ f)\, d\mu \right\rangle = \int \langle \mathbf{z}', u \circ f \rangle\, d\mu = \left\langle ^t u(\mathbf{z}'), \int f\, d\mu \right\rangle = \left\langle \mathbf{z}', u \left( \int f\, d\mu \right) \right\rangle.
$$

特别是，如果 f 本质上是 $\mu$ 标量可积，那么当 F 的拓扑被更粗糙的拓扑替换时，它本质上仍然是 $\mu$ 标量可积。

#### 命题 2 {#int-vi-s1-prop-2 .statement tag=098J}

— *令 f 本质上是 T 到 F 的$\mu$可积映射。对于$\mu$可测量且有界的每个数值函数 $g \geqslant 0$，T 到 F 的映射 $t \mapsto g(t)f(t)$（表示为 gf 或 fg）本质上是标量$\mu$-可积，f 本质上是 $(g \cdot \mu)$-可积，并且*
$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

对于所有 $\mathbf{z}' \in F'$，这是公式 $\langle \mathbf{z}', gf \rangle = g \langle \mathbf{z}', f \rangle$ 的直接的推论，对于每个基本 $\mu$ 可积标量函数 $h$（第 V, §5, No. 3，第 1 章），这是公式 $\int h d(g \cdot \mu) = \int hg d\mu$。

A great many propositions about essentially integrable numerical functions may be transposed word for word into propositions about scalarly essentially integrable vector-valued functions. 其中更重要的是，我们提请注意条件，因为函数对于密度定义的度量本质上是可积的（第1章）。 V, §5, No. 3，Th。 1)，或关于某项措施的像（第 1 章） V, §6, No. 2，Th。 1），或关于诱导措施（第 1 章） V, §7, No. 1，Th。 1)，或者关于正测度的可求和族的和（第 1 章） V, §2, No. 2，道具。 1和3以及Cor。提案 1 中的 3）。 这些转换留给读者。

然而，要在“双积分”（第V, §3, No. 3，Th.1和§8, No. 4，Th.1（Lebesgue–Fubini定理））上获得叙述相应的到定理，有必要加强假设(cf.锻炼。1);在应用上，将先前引用的定理到函数$\langle \mathbf{z}', f \rangle$中的每一个，其中$\mathbf{z}' \in F'$，因此获得以下命题：

#### 命题 3 {#int-vi-s1-prop-3 .statement tag=098K}

— 令$X$为$X$积极措施的局部紧凑空间，$t \mapsto \lambda_t$一个$\mu$充分$^3$族（第V, §3, No. 1，定义1），并令$\nu = \int \lambda_t d\mu(t)$。令$f$为$X$的映射变为$F$；假设 $1^\circ$ $f$ 是 $\nu$ 标量可积的； $2^\circ$ 存在一个局部 $\mu$ 可忽略不计的集合 $N \subset T$，这样，对于每个 $t \notin N$，$f$ 是标量 $\lambda_t$ 可积且$\int f d\lambda_t \in F$。那么，为 $t \notin N$ 定义的函数 $t \mapsto \int f d\lambda_t$ 本质上是 $\mu$ 可标量可积的，并且 $^4$

$$
\int f(x) d\nu(x) = \int d\mu(t) \int f(x) d\lambda_t(x) .
$$

#### 命题 4 {#int-vi-s1-prop-4 .statement tag=098L}

— 令$T$和$T'$为两个局部紧凑的空间，$\mu$（分别为$\mu'$）对$T$（分别为$T'$）的正测度，$\nu = \mu \otimes \mu'$乘积对$X = T \times T'$的测度。令$f$为$X$到$F$的映射。假设： $1^\circ$ $f$ 是 $\nu$ 标量可积； $2^\circ$ 存在一个局部可忽略的 $\mu$ 集合 $N \subset T$，这样，对于每个 $t \notin N$，映射 $t' \mapsto f(t, t')$ 是$\mu'$ 标量可积的，并且$\int f(t, t') d\mu'(t') \in F$。那么，为 $t \notin N$ 定义的函数 $t \mapsto \int f(t, t') d\mu'(t')$ 本质上是 $\mu$ 可积且$^4$

$$
\iint f(t, t') d\mu(t) d\mu'(t') = \int d\mu(t) \int f(t, t') d\mu'(t') .
$$

$^3$假设族本质上是$\mu$可积就足够了，因此命题适用于“$\mu$-充分”的两种解释中的任何一种。
$^4$等式为 ${F'}^*$ 的元素。

### 2. 标量积分的性质本质上是可积函数

#### 命题 5 {#int-vi-s1-prop-5 .statement tag=098M}

— 令 $\mu$ 为 $T$ 上的有界正测度，$S$ $\mu$ 可测量集合携带 $\mu$（章节 V, §5, No. 7，定义 4），$f$ $\mu$ 可积标量 (*) 函数与 $F$ 中的值。令$D$为空间$F'$*中$f(S)$的封闭凸包络，配备拓扑$\sigma(F', F')$。然后$\int f\, d\mu \in \mu(T)D$。

由于$D$是闭半空间包含$f(S)$的交（TVS，II, §5, No. 3，第4条命题的Cor.1），因此足以证明关系$\langle f(t), z' \rangle \leq a$对于所有$t \in S$（其中$z' \in F', a \in \mathbf{R}$) 意味着$\langle z', \int f\, d\mu \rangle \leq a \cdot \mu(T)$；但从 $\int f\, d\mu = \int_S f\, d\mu$ 开始，这是从第 1 章开始的。 IV, §4, No. 2，科。 1 Th。 1.

#### 推论{#int-vi-s1-n2-cor-1 .statement tag=098N}

— 令 $\mu$ 为$T$、$S$ $\mu$ 可测量集合的有界正测度，将 $\mu$ 和 $T$ 的$f$ 映射逐级放入$F$ $\mu$是可测的，并且使得$f(S)$包含在$F$的弱紧凸凸子集$A$中。那么$f$是$\mu$可标量可积的，并且$\int f\, d\mu \in \mu(T)A \subset F$。

对于每个 $z' \in F'$，$\langle z', f \rangle$ 是 $\mu$ 可测的，并且有界于 $S$，因此可积，这证明了 $f$ 是标量可积的。此外，由于$A$在$F_\sigma$中是紧的，因此它在$F'$*中是闭的，并且$f(S)$在$F'$*中的闭凸包络包含在$A$、从而的推论中。

#### 命题 6 {#int-vi-s1-prop-6 .statement tag=098O}

— 设 $f$ 是一个本质上 $\mu$ 可积的标量函数，其中值位于 $F$ 中，因此 $\int f\, d\mu \in F$。对于$F$上的每个下半连续半范数$q$，

$$
q\left( \int f\, d\mu \right) \leq \int^\bullet (q \circ f)\, d\mu .
$$

令$D$为$z \in F$的集合，使得$q(z) \leq 1$； $D$ 是闭凸的，并且包含 $0$，因而 $D = D^{oo}$（TVS、II, §6, No. 3、Th.1 的 Cor. 3）。因而，只要证明每有一个$z' \in D^\circ$，就有$|\langle z', \int f\, d\mu \rangle| \leq \int^\bullet (q \circ f)\, d\mu$；但这是从以下事实立即得出的：每个$t \in T$都有$|\langle z', f(t) \rangle| \leq q(f(t))$。

注数值函数 $q \circ f$ 不必是$\mu$ 可测量的（例12）。

#### 命题 7 {#int-vi-s1-prop-7 .statement tag=098P}

— 设 $f$ 为 $T$ 的映射到 $F$，基本上可标量 $\mu$ 可积，这样对于 $T$ 的每个紧致子集 $K$，都包含 $f(K)$

(*) 回想一下，对于*有界*正测度 $\mu$，$\mu$-可积函数和本质上 $\mu$-可积函数的概念是相同的（第 9 章，第 V, §1, No. 3 章，Cor.）。

5 原上位积分记号为$\overline{\int^*}$，第二版改为$\int^\bullet$。 V。

在 F 的弱紧致、平衡、凸子集中。然后 $\int f d\mu$ 属于到 F 的双$F''$。

对于 T 的每个紧凑子集 K，

$$
\int f \varphi_K d\mu = \int (f \varphi_K) d(\varphi_K \cdot \mu);
$$

科。第 5 条命题可以应用于有界测度 $\varphi_K \cdot \mu$ 和函数 $f \varphi_K$，因而$\int f \varphi_K d\mu \in F$。对于每个 $z' \in F'$，$\langle z', f \rangle$ 本质上是 $\mu$ 可积的，因而（第 V, §1, No. 3 章，命题 10）

$$
\int \langle z', f \rangle d\mu = \lim_K \int \langle z', f \rangle \varphi_K d\mu,
$$

极限是相对于T的紧凑子集的递增有向集合而取的。 一个结论，相对于这个集合，对于拓扑$\sigma({F'}^*, F')$，$\int f \varphi_K d\mu$收敛到$\int f d\mu$。 现在，

$$
\left| \left\langle z', \int f \varphi_K d\mu \right\rangle \right| = \left| \int \langle z', f \rangle \varphi_K d\mu \right| \leq \int |\langle z', f \rangle| d\mu,
$$

这证明了元素$\int f \varphi_K d\mu$的集合是$F_\sigma$的*有界*子集，因此也是F的（TVS，IV, §1, No. 1，命题1）。因而，命题 7 是以下引理中的推论：

#### 引理 1 {#int-vi-s1-lem-1 .statement tag=098Q}

*F 的每个有界子集的${F'}^*$（对于拓扑 $\sigma({F'}^*, F')$）的闭包包含在双$F''$中。*

因为，F 的有界子集包含在 F 的强对偶 $F'$ 中 0 邻域的极坐标（在 $F''$ 中），因此对于 $\sigma(F'', F')$，在 $F''$ 中相对紧（TVS，III, §3, No. 5，第 7 条命题和 No. 4，第 4 条命题的 Cor.2）；由于$\sigma(F'', F')$是由$\sigma({F'}^*, F')$诱发的，所以引理得证。

#### 推论{#int-vi-s1-n2-cor-2 .statement tag=098R}

*假设 F 是半自反的，并令 f 是 T 的 $\mu$ 可标量可积到 F 中的映射，使得对于 T 的每个紧凑子集 K，$f(K)$ 是有界的。然后$\int f d\mu$属于到F.*

因为，F 的每个有界子集都是相对弱紧的（TVS、IV, §2, No. 2、Th.1）和 $F = F''$。

#### 命题 8 {#int-vi-s1-prop-8 .statement tag=098S}

*设$\mu$为T上的有界正测度，S a $\mu$可测集合将T的$\mu$、f a $\mu$可测映射带入F，使得$f(S)$包含在F的完整、有界、平衡凸子集 B中。那么，f是标量 $\mu$ 可积且 $\int f d\mu \in \mu(T)B \subset F$.*

由于 S 是 $\mu$ 可积的，因此存在由 $\mu$ 可忽略的集合 N 和紧凑子集的序列 $(K_n)$ 形成的 S 的划分，使得 f 的限制对于每个 $K_n$ 都是连续的（第 1 章） IV, §4, No. 6，第 4 条第 3 条和§5, No. 1，定义 1)；因而，$f(K_n)$ 是 $F$ 的紧致子集。然后，$f(K_n)$ 的闭合平衡凸包络$B_n$ 是预紧的（TVS，II, §4, No. 1，命题 3），并且包含在 $F$ 的完整子集 $B$ 中，因此它是紧的，并且 *更不必说* 是弱紧的。因而（Prop. 5 的 Cor.） $f \varphi_{K_n}$ 是 $\mu$ 标量可积的，并且

$$
z_n = \int f \varphi_{K_n} d\mu \in \mu(K_n)B_n \subset \mu(K_n)B .
$$

对于$F$上的每个连续半范数$p$，有以下结论

$$
p(z_n) \leq \mu(K_n) \cdot \sup_{x \in B} p(x) ;
$$

由于$B$是有界的，并且由于级数与广义项$\mu(K_n)$收敛并且具有和$\mu(T)$，因此可以看出序列与广义项$s_n = z_1 + z_2 + \cdots + z_n$是完整的柯西序列子集$\mu(T)B$共$F$。因而，这个序列收敛到$\mu(T)B$的元素$s$；因为可以假设$f(t) = 0$在$T - S$上，勒贝格的定理应用于函数$\langle z', f \rangle$（$z' \in F'$）中的每一个都证明了$s = \int f d\mu$。

### 3.算子的积分

设$G$和$H$是$\mathbf{R}$上的两个Hausdorff局部凸空间，现在假设$F$是$G$的连续线性映射到$H$的空间$\mathscr{L}(G; H)$，配备拓扑 *逐点*收敛。 $F$上的每个连续线性形式都可以扩展到乘积空间$H^G$上的连续线性形式（TVS，II, §4, No. 1，命题2），因此可以写成$u \mapsto \sum_{i=1}^n \langle u(a_i), b'_i \rangle$，其中$a_i$（分别为$b'_i$）是$G$的元素（分别是$H$的对偶$H'$）。 说$T$到$F$的映射$U$本质上是$\mu$可积，意味着对于每个$a \in G$和每个$b \in H'$，数值函数$t \mapsto \langle U(t) \cdot a, b' \rangle$本质上是$\mu$可积。

#### 命题 9 {#int-vi-s1-prop-9 .statement tag=098T}

*设 $U$ 是 $T$ 的 $\mu$ 可标量可积到 $F = \mathscr{L}_s(G; H)$ 中的映射。在阶、$\int U d\mu \in F$中，满足以下两个条件是必要且充分的：*

a) *对于每个$x \in G$，$\int (U(t) \cdot x) d\mu(t) \in H$。*

b) *对于$H'$的每个等连续子集$B'$，线性形式$u_{y'} : x \mapsto \int \langle U(t) \cdot x, y' \rangle d\mu(t)$的集合，其中$y'$超过$B'$，是等连续的。*

条件 a) 和 b) 是必要的。因为，由于对于每个$x \in G$，$\mathscr{L}_s(G; H)$到$H$的映射$\tilde{x} : V \mapsto V \cdot x$是线性的，所以可以看到（No. 1，

命题 1) $\widetilde{\mathbf{x}} \circ U : t \mapsto U(t) \cdot \mathbf{x}$ 基本上是 $\mu$ 标量可积的，并且

$$
(1) \quad S \cdot \mathbf{x} = \int (U(t) \cdot \mathbf{x})\, d\mu(t),
$$

其中$S = \int U\, d\mu \in \mathscr{L}_s(G; H)$。这就证明了a）。此外，(1)也可以写成

$$
(2) \quad \langle S \cdot \mathbf{x}, \mathbf{y}' \rangle = \int \langle U(t) \cdot \mathbf{x}, \mathbf{y}' \rangle\, d\mu(t) = \langle \mathbf{x}, u_{\mathbf{y}'} \rangle,
$$

其他字${}^t S \cdot \mathbf{y}' = u_{\mathbf{y}'}$。由于$S$是连续的，${}^t S$变换将$H'$的每个等连续子集转换为$G'$、从而的等连续子集b)。

相反，假设 a) 和 b) 已得到验证。凭借a)，将$G$的公式(1)定义线性映射$S$转化为$H$，并且对于每个$\mathbf{y}' \in H'$，这个映射满足(2)（No. 1，命题1）；但是，条件 (b) 表示 $S$ 是连续的（TVS，II, §6, No. 4，命题 5 和 6，以及 III, §3, No. 5，命题 7），因此 $S \in \mathscr{L}_s(G; H)$。最后，公式(2)证明了$S = \int U\, d\mu$。

#### 推论{#int-vi-s1-n3-cor-1 .statement tag=098U}

— *条件 b) 的第 9 条在以下两种情况下均得到满足*：

$1^\circ$ *测度 $\mu$ 是有界的，如果 $S$ 是其支撑，则 $U(S)$ 是 $\mathscr{L}(G; H)$* 的等连续子集。

满足第 9 条的 $2^\circ$ *条件 a)，空间 $G$ 是桶状的，并且，对于 $T$ 的每个紧致子集 $K$，$U(K)$ 是有界的子集 $\mathscr{L}_s(G; H)$*。

让我们首先将自己置于情况$1^\circ$。我们可以将自己限制在$S = T$（第V, §7, No. 1，Th.1）的情况。那么，对于$H'$的每个等连续子集$B'$，存在一个等连续、凸、平衡且弱闭的子集$A' \subset G'$，使得${}^t U(t) \cdot \mathbf{y}' \in A'$对于所有$\mathbf{y}' \in B'$和所有$t \in T$（TVS，II, §6, No. 4，提案 6）。由于$U$是$\mu$可标量可积，$T$的映射$t \mapsto {}^t U(t) \cdot \mathbf{y}'$进入$G$的对偶$G'$配备$\sigma(G', G)$，是$\mu$可标量可积，并且可以写成

$$
u_{\mathbf{y}'} = \int ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t).
$$

由于 $A'$ 对于 $\sigma(G', G)$ 是凸且紧的，因此 Cor. No. 2的第5条命题表明，对于每个$\mathbf{y}' \in B'$，都有$u_{\mathbf{y}'} \in \mu(T)A'$，这就证明了我们的断言。

现在让我们假设情况$2^\circ$。对于每个 $\mathbf{y}' \in H'$ 和$T$、集合的每个紧凑型子集 $K$

$$
u_{K, \mathbf{y}'} = \int \varphi_K(t) ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t),
$$

元素的代数对偶$G^*$ $G$。由于$G$是桶状的，$\mathscr{L}_s(G; H)$的每个有界子集都是等连续的（TVS，III, §4, No. 2，Th.1）；参数的第一个部分应用于函数 $\varphi_K U$ 和有界测度 $\varphi_K \cdot \mu$，显示 $u_{K, y'} \in G'$。此外，对于拓扑$\sigma(G^*, G)$，$u_{y'} = \lim_{K} = u_{K, y'}$、极限是相对于$T$的紧凑子集的递增有向集合而取的（第V, §1, No. 3章，第10条）。为了验证命题9的条件b)，根据命题9，证明(1)定义的$G$到$H$的线性映射$S$是连续的即可；此外，$G$是桶形的，因此当$G$和$H$配备其弱化拓扑时，足以证明$S$是连续的（TVS，IV, §1, No. 3，第7条）；最后，根据（2），可以简化为对于每个 $y' \in H'$ 都有 $u_{y'} \in G'$。由于$u_{y'}$处于闭包中，对于$u_{K, y'}$的集合$M'$的$\sigma(G^*, G)$，其中$K$运行于$T$的紧致子集的集合，因此足以证明$M'$ 等连续（TVS，III, §3, No. 4，命题 4）；由于$G$是桶装的，因此对于每个$x \in G$，$\langle x, u_{K, y'} \rangle$的集合都是有界的（TVS，III, §4, No. 2，Th.1）。但这是从关系立即得出的

$$
|\langle x, u_{K, y'} \rangle| = \left| \int \varphi_K(t) \langle U(t) \cdot x, y' \rangle d\mu(t) \right| \leq \int |\langle U(t) \cdot x, y' \rangle| d\mu(t).
$$

#### 命题 10 {#int-vi-s1-prop-10 .statement tag=098V}

— *令 $U$ 为 $T$ 的映射到 $F = \mathscr{L}_s(G; H)$。在以下三种情况中，$U$本质上是$\mu$可积且$\int U d\mu \in \mathscr{L}_s(G; H)$：*

a) $H$ 是准完备的，$\mu$ 是有界的，如果 $S$ 是它的支持，$U$ 是 $\mu$ 可测的，$U(S)$ 是等连续的。

b) $H$ 是半自反的，$\mu$ 是有界的，如果 $S$ 是其支持，$U$ 是标量 $\mu$ 可测的，$U(S)$ 是等连续的。

c) $H$ 是半自反的，$G$ 是桶状的，$U$ 本质上是 $\mu$ 可标量可积的，并且，对于 $T$ 的每个紧致子集 $K$，$U(K)$ 是有界的。

在所有三种情况下，$U$ 本质上是可积的这一事实是显而易见的；凭借第 9 号提案及其推论，在每种情况下都足以验证第 9 号提案的条件 a)。现在，这个条件是从第一种情况下No. 2的第 8 条提案以及 Cor.9 中得出的。在另外两种情况下，符合No. 2第7条的规定。

### 4.性质（GDF）

在本期中，我们将考虑具有以下性质的局部凸空间$F$（称为“可数闭图”性质）：⁶

⁶ *Graphe dénombrablement fermé*，从而缩写 (GDF)。

(GDF) *如果 u 是 F 的线性映射到 Banach 空间 B，使得在乘积空间 F × B 中，u 的图 Γ 的点的每个收敛序列的每个极限再次属于到 Γ，则 u 是连续的。*

每个 Fréchet 空间都有性质 (GDF)（TVS、I, §3, No. 3、Th.1 的 Cor. 5）。在附录中，我们将看到空间的其他例具有性质（GDF）。

#### 命题 11 {#int-vi-s1-prop-11 .statement tag=098W}

*每个具有性质 (GDF) 的 Hausdorff 局部凸空间 F 都是桶装的。*

设V为F中的桶，q为规范，是F上的半范数；令 H 为与空间 F 相关联的 Hausdorff 空间，并配备由该单一半范数定义的拓扑。 H 的完成$\widehat{H}$ 是 Banach 空间；令$\pi$为F的典范映射进入$\widehat{H}$；我们将证明 $\pi$ 是*连续的*（对于 F 上的原始拓扑）；这将建立命题，因为$\widehat{H}$的单位球的$\pi$下的V、逆像将是F中0的邻域。为了建立$\pi$的连续性，凭借（GDF），只需证明$\pi$的图为*于$F \times \widehat{H}$*关闭*；在其他字中，我们必须看到，如果$\mathscr{F}$是F上的一个滤波器，收敛到$x \in F$，并且它的像$\pi(\mathscr{F})$收敛到$y \in \widehat{H}$，那么$y = \pi(x)$。现在，$F'$中V的极$V^\circ$的每个元素$x'$只能以一种方式扩展为$\widehat{H}$上的连续线性形式（再次表示为$x'$），以及其中的集合形式是$\widehat{H}$对偶的单位球；因此，只要证明对于每个$x' \in V^\circ$就有$\langle y, x' \rangle = \langle \pi(x), x' \rangle$。但这是从关系得出的

$$
\langle y, x' \rangle = \lim_{\mathscr{F}} \langle \pi(z), x' \rangle = \lim_{\mathscr{F}} \langle z, x' \rangle = \langle x, x' \rangle = \langle \pi(x), x' \rangle .
$$

#### 定理 1 {#int-vi-s1-thm-1 .statement tag=098X}

(Gelfand-Dunford)—*设 F 为 Hausdorff 局部凸空间，具有性质 (GDF)，$F'_s$ 其弱对偶。对于 T 的每个映射 f 到 $F'_s$ 本质上是 $\mu$ 可标量可积的，$\int f d\mu$ 属于到 $F'$ 的积分。*

回想一下，$F'_s$ 的对偶是 F（TVS，II, §6, No. 2，命题 3）。因此，对于每个$z \in F$，数值函数$\langle z, f \rangle$本质上是$\mu$可积的；设$\theta(z)$为$L^1(\mu)$中的类。为了证明$\int f d\mu \in F'$，必须证明线性形式$z \mapsto \langle z, \int f d\mu \rangle$在F上连续；事实上，我们将证明以下更强的结果：

#### 引理 2 {#int-vi-s1-lem-2 .statement tag=098Y}

*令f为T到$F'_s$的映射，这样对于每个$z \in F$，数值函数$\langle z, f \rangle$属于到$\overline{\mathscr{L}}^p(\mu)$（$1 \leq p \leq +\infty$）；设$\theta(z)$为$L^p(\mu)$中的函数的类。那么$z \mapsto \theta(z)$就是F到$L^p(\mu)$的连续线性映射。*

凭借（GDF）性质，足以证明对于F的元素的每一个序列$(z_n)$收敛到$z$，使得$(\theta(z_n))$收敛到$u \in L^p(\mu)$，就有$u = \theta(z)$。现在，替换，如果需要序列$(z_n)$通过一个子序列，我们可以假设函数$\langle z_n, f \rangle$的序列几乎处处局部收敛到函数$h \in \overline{\mathscr{L}}^p(\mu)$，其中类$u$在$L^p(\mu)$（第 IV, §3, No. 4、第 3 章和第 V, §1, No. 3）。因为到假设，对于每个$t \in T$序列$(\langle z_n, f(t) \rangle)$收敛到$\langle z, f(t) \rangle$，我们几乎在所有地方都有$h(t) = \langle z, f(t) \rangle$，因而$u = \theta(z)$。

#### 推论 1 {#int-vi-s1-lem-2-cor-1 .statement tag=098Z}

*令$G_i$($1 \leq i \leq n$)为具有性质(GDF)的$n$豪斯多夫局部凸空间，并令$F$为$\prod_{i=1}^n G_i$上单独连续的多重线性形式的空间，配备逐点收敛的拓扑。对于 $T$ 到 $F$ 的每一个映射 $f$，本质上是 $\mu$ 可标量可积，则有 $\int f d\mu \in F$。*

空间$F$与张量积$\bigotimes_{i=1}^n G_i$对偶，$F$上逐点收敛的拓扑不是别人，正是拓扑$\sigma(F, \bigotimes_{i=1}^n G_i)$。 因而，代数对偶 ${F'}^*$ 是 $\prod_{i=1}^n G_i$ 上所有多重线性形式的空间。 设$z = (z_1, \ldots, z_n)$为$\prod_{i=1}^n G_i$的元素；对于每个多重线性形式$u \in {F'}^*$，映射$x \mapsto u(z_1, \ldots, z_{i-1}, x, z_{i+1}, \ldots, z_n)$在$G_i$上是线性形式，我们用$\lambda_i(z)(u)$表示；因而，我们将${F'}^*$的线性映射$\lambda_i(z)$转化为$G_i$的代数对偶$G_i^*$，对于拓扑$\sigma({F'}^*, \bigotimes_{i=1}^n G_i)$和$\sigma(G_i^*, G_i)$是连续的。 说$u \in F$意味着对于每一个指标$i$和每一个$z \in \prod_{i=1}^n G_i$，都有一个$\lambda_i(z)(u) \in G_i'$。 Now, by Prop. 1 of No. 1, the mapping $\lambda_i(z)$ of $F$ is a scalarly essentially $\mu$-integrable mapping of $T$ into $G_i'$ equipped with the topology $\sigma(G_i', G_i)$, and
$$
\int (\lambda_i(z) \circ f) d\mu = \lambda_i(z) \left( \int f d\mu \right).
$$
By Th. 1, $\int (\lambda_i(z) \circ f) d\mu \in G_i'$ for $1 \leq i \leq n$, therefore $\int f d\mu \in F$.

#### 推论 2 {#int-vi-s1-lem-2-cor-2 .statement tag=0990}

*设 $G$ 为具有性质 (GDF) 的 Hausdorff 局部凸空间，$H$ 为半自反空间，其强对偶 $H_b'$ 具有性质 (GDF)（cf. App.，No. 2，Prop. 3）。设$F$为空间$\mathscr{L}_s(G; H)$；对于$T$到$F$的每一个映射$U$，本质上是$\mu$可积，$\int U d\mu$属于到$F$的积分。

由于$G$是桶装的（提案11），$\mathscr{L}(G; H) = \mathscr{L}(G_\sigma; H_\sigma)$（TVS，IV, §1, No. 3，提案7）；此外，可以通过空间$\mathscr{L}_s(G_\sigma; H_\sigma)$来替换$F = \mathscr{L}_s(G; H)$，因为两个空间具有相同的对偶$G \otimes H'$（TVS，II, §6, No. 2，第3条，以及上面No. 3的第一段）。如果，对于每个$u \in \mathscr{L}(G; H) = \mathscr{L}(G_\sigma; H_\sigma)$，一个集合$\tilde{u}(x, y') = \langle u(x, y') \rangle$（对于$x \in G$，y'\in H'），线性映射$u \mapsto \tilde{u}$是F的双射到单独连续的双线性形式上的空间$F_1$ $G_\sigma \times H'_s$，其中$H'_s$表示双$H'$配备弱拓扑$\sigma(H', H)$（App.，No. 1）；此外，这个映射是$\mathscr{L}_s(G_\sigma; H_\sigma)$到$F_1$的同构，配备了拓扑的逐点收敛（*loc.cit.*）。但由于假设 H 是$H'_b$ 的对偶，$F_1$ 也是$G \times H'_b$ 上单独连续的双线性形式的空间。科。因而，2 是从 Cor 得出的。 1.

注那个科。当 G 是 *Banach 空间* 并且 H 是 *自反 Banach 空间* 时，2 特别适用。

### 5. 可测量映射和标量可测量映射

如果 T 的映射 f 进入 Hausdorff 局部凸空间 F 是标量 $\mu$ 可测的，则通常不能得出 f 是 $\mu$ 可测的结论（Exer. 12）。尽管如此：

#### 命题 12 {#int-vi-s1-prop-12 .statement tag=0991}

*如果 F 是可分离、可度量的局部凸空间，则 T 到 F 中的每个标量 $\mu$ 可测量映射 f 都是 $\mu$ 可测量。*

因为，F 可以被视为 Banach 空间的可数乘积 $\prod_n E_n$ 的子空间（TVS，II, §1, No. 3，命题 3），并且可以假设 $\mathrm{pr}_n(F)$ 在 $E_n$ 中是稠密的，因此是可分的。对于每个 n，映射 $\mathrm{pr}_n \circ f$ 是标量 $\mu$ 可测的，因而 $\mu$ 可测（第 10 章第 IV, §5, No. 5，Cor. 2），因而 f 是 $\mu$ 可测（第 IV, §5, No. 3，Th. 1）。

#### 命题 13 {#int-vi-s1-prop-13 .statement tag=0992}

*设 F 为可分离、可度量的局部凸空间 $F_n$ 的局部凸空间，即序列的直极限，F 为 $F_n$ 的并。令$F'$为F的对偶，配备拓扑$\sigma(F', F)$。然后，T 到 $F'$ 中的每个标量 $\mu$ 可测量映射 f 都是 $\mu$ 可测量。*

首先假设 F 是可度量且可分离的，并令 D 为 F 中的可数稠密集合。令 $(V_n)$ 为 F 中 0 的平衡、凸、开邻域的递减基本序列；极坐标集合 $V_n^\circ$ 是等连续的，并且它们的并是 $F'$ 的全部。设 $T_n = f(V_n^\circ)$； 序列$(T_n)$为递增和$T = \bigcup T_n$；让我们证明每个 $T_n$ 都是 $\mu$-*可测量*。事实上，$D \cap V_n^n$在$V_n$中是稠密的；对于每个$y \in D \cap V_n$，令$S_y$为$t \in T$的集合，使得$|\langle y, f(t) \rangle| \leq 1$； 假设意味着$S_y$ 中的每一个都是可测量的，$T_n$ 是$S_y$ ($y \in D \cap V_n$) 可数族的交。因而，对于 T 的每个紧致子集 K 和每个 $\varepsilon > 0$，存在整数 n 使得 $\mu(K - (K \cap T_n)) \leq \frac{\varepsilon}{4}$，然后存在 $K \cap T_n$ 的紧致子集 $K_1$ 使得 $\mu((K \cap T_n) - K_1) \leq \frac{\varepsilon}{4}$；最后，存在 $K_1$ 的紧凑子集 $K_2$，使得 $\mu(K_1 - K_2) \leq \frac{\varepsilon}{2}$ 且所有函数 $\langle y, f \rangle$ 的限制到 $K_2$，其中 $y \in D$ 是连续的（Ch. IV, §5, No. 1，命题 2）。由于集合$f(K_2) \subset f(T_n) \subset V_n^\circ$是等连续的，$\sigma(F', F)$在$f(K_2)$上引起的拓扑与$D$中逐点收敛的拓扑相同（GT，X, §2, No. 4，Th.1）；因而，$f$到$K_2$的限制是连续的，从而是第一种情况下的断言。

让我们讨论一般情况。如果$z'$是$F$上的连续线性形式，则其限制$z'_n$到$F_n$是连续的；从$F = \bigcup_n F_n$开始，$F$的对偶$F'$可以用乘积$\prod_n F'_n$和$\operatorname{pr}_n z' = z'_n$的线性子空间（代数上）来识别。此外，由于$F$的每个有限子集都包含在$F_n$之一中，因此拓扑$\sigma(F', F)$正是由拓扑$\sigma(F'_n, F_n)$的乘积拓扑引起的拓扑。既然如此，如果$f$是$\mu$标量可测量的，那么$\operatorname{pr}_n \circ f$是$\mu$可标量测量的，因为对于每个$t \in T$，$\operatorname{pr}_n(f(t))$是$f(t)$到$F_n$的限制。 证明的第一个部分显示，对于每个 $n$，$\operatorname{pr}_n \circ f$ 是 $\mu$ 可测量的，因而 $f$ 也是如此（第 IV, §5, No. 3，第 1 章）。

### 6. 应用程序：I。连续函数至空间措施的扩张

令$T$为局部紧致空间，$F$为准完备、Hausdorff局部凸空间，$f$为$T$到$F$的连续映射；如果$\mu$是$T$的正测度，且具有紧支撑$S$，则$f(S)$是紧的； $f(S)$ 的封闭凸包络是紧致的（TVS，III, §1, No. 6），因此 $f$ 是$\mu$ 标量可积且$\int f \, d\mu \in F$（No. 2，第 5 条命题的参考）。 如果现在$\lambda$是任何具有紧支撑的实测度，则$\lambda^+$和$\lambda^-$是具有紧支撑的正测度； 设定$\int f \, d\lambda = \int f \, d\lambda^+ - \int f \, d\lambda^-$，立即验证（使用关系$(\lambda + \mu)^+ + \lambda^- + \mu^- = \lambda^+ + \mu^+ + (\lambda + \mu)^-$）$\lambda \mapsto \int f \, d\lambda$是空间$\mathscr{C}'(T)$在紧支撑下$T$上的测度中的线性映射，进入局部凸空间$F$。

Let us now observe that the space $\mathscr{C}'(T)$ may be identified with the dual of the space $\mathscr{C}(T)$ of continuous numerical functions on $T$ (whence its notation), when $\mathscr{C}(T)$ is equipped with the topology of compact convergence (which we shall always assume in this No. and in the following one): for, it is known on the one hand (Ch. IV, §4, No. 8，命题 14) $T$ 上的测度可以扩展到 $\mathscr{C}(T)$ 上的连续线性形式是紧支撑测度，反之，$\mathscr{C}(T)$ 上的连续线性形式的限制到 $\mathscr{K}(T)$ 是一个测度（因为拓扑 $\mathscr{K}(T)$比$\mathscr{C}(T)$的拓扑诱发的更细）。

#### 命题 14 {#int-vi-s1-prop-14 .statement tag=0993}

*设 T 为局部紧致空间，F 为准完备，Hausdorff 局部凸空间，f 为 T 到 F 的连续映射。如果具有紧支撑的 T 上的测度空间 $\mathscr{C}'(T)$ 配备有在紧致子集中一致收敛的拓扑 $\mathscr{C}(T)$，则映射 $\lambda \mapsto \int f d\lambda$ 是 $\mathscr{C}'(T)$ 到 F 中的唯一连续线性映射 $\tilde{f}$，使得对于每个 $t \in T$ 都有 $\tilde{f}(\varepsilon_t) = f(t)$。*

要建立扩张的唯一性，只要看到点测量$\varepsilon_t$形式在$\mathscr{C}'(T)$中总共集合即可；由于 $\mathscr{C}'(T)$ 的对偶是 $\mathscr{C}(T)$ (TVS, IV, §1, No. 1, Th. 1)，因此足以观察到与所有度量 $\varepsilon_t$ 正交的每个函数 $g \in \mathscr{C}(T)$ 等于 0 by 定义 (TVS, IV, §1, No. 2,命题 2）。

现在让我们证明 $\lambda \mapsto \int f d\lambda$ 是连续的。令 V 为 F 中 0 的闭平衡凸邻域；只要证明$\mathscr{C}(T)$存在一个相对紧的子集L，使得关系$\lambda \in L^\circ$和$z' \in V^\circ$暗示$|\langle \int f d\lambda, z' \rangle| \leq 1$，或者再次暗示$|\int \langle f, z' \rangle d\lambda| \leq 1$。为此，我们将证明，当$z'$超过$V^\circ$时，数值函数$\langle f, z' \rangle$的集合L在$\mathscr{C}(T)$中相对紧凑。由于$V^\circ$有界于$\sigma(F', F)$，对于$t \in T$固定且$z'$超过$V^\circ$，数$|\langle f(t), z' \rangle|$的上界是有限的；凭借阿斯科利的定理（GT，X, §2, No. 5，Th.2的Cor.2），因此足以证明$\langle f, z' \rangle$（$z' \in V^\circ$）的集合是*等连续的*。但是，对于每个$t_0 \in T$和每个$\delta > 0$，在T中存在假设一个$t_0$的邻域W，使得$f(t) - f(t_0) \in \delta V$对于所有$t \in W$；由此可见，$|\langle f(t), z' \rangle - \langle f(t_0), z' \rangle| \leq \delta$适用于所有$t \in W$和所有$z' \in V^\circ$，从而完成证明。

#### 注 {#int-vi-s1-n6-rem-1 .statement tag=0994}

— 1) 映射 $t \mapsto \varepsilon_t$ 是 T 到空间 $\mathscr{C}'(T)$ 的*同胚*；因为，如果L是$\mathscr{C}(T)$和$t_0 \in T$的紧凑子集，则存在（GT，X, §2, No. 5，Th.2的Cor.3）$t_0$的邻域W，使得对于每个$t \in W$和每个$|g(t) - g(t_0)| \leq 1$ 函数$g \in L$，因此$\varepsilon_t - \varepsilon_{t_0} \in L^\circ$对应$t \in W$，这证明了$t \mapsto \varepsilon_t$的连续性（cf.第IV, §4, No. 8，第15条命题）；我们知道，在加法中，对于模糊拓扑来说，逆映射已经是连续的（第III, §1, No. 9，命题13），因此*更不必说*对于$\mathscr{C}(T)$的紧致子集中一致收敛的拓扑。如果然后通过$t \mapsto \varepsilon_t$将T识别为$\mathscr{C}'(T)$中的像，则可以说$\lambda \mapsto \int f d\lambda$是f到*线性*映射的唯一*连续扩张*。

2) 注，在$\lambda \mapsto \int f d\lambda$连续性的证明中，我们没有利用F是准完备的这一事实。因此，如果没有这个假设，第 14 号提案的结论仍然有效，只要在加法中知道$\int f d\mu \in F$ 对于每一项具有紧凑支持的积极措施$\mu$。

现在假设$f(T)$是F的*有界*子集。那么，对于T上的每个*有界*正测度$\mu$，f是标量$\mu$可积且$\int f d\mu \in F$

（No. 2，提案 8）。如果 $\lambda$ 是 $T$ 上的任何有界实测度，则 $\lambda^+$ 和 $\lambda^-$ 是有界的，并且我们立即看到，如上定义的 $\lambda \mapsto \int f\, d\lambda$ 是 *有界* 测度的空间 $\mathscr{M}^1(T)$ 的 *线性* 映射 $T$，转化为局部凸空间$F$，显然将$\mathscr{C}'(T)$的扩展映射$\lambda \mapsto \int f\, d\lambda$转化为$F$。

#### 命题 15 {#int-vi-s1-prop-15 .statement tag=0995}

*令$T$为局部紧致空间，$F$为准完备的Hausdorff局部凸空间，$f$为$T$的连续映射进入$F$，使得$f(T)$有界。如果$\mathscr{M}^1(T)$配备其Banach空间拓扑，则$\mathscr{M}^1(T)$到$F$的线性映射$\lambda \mapsto \int f\, d\lambda$是连续的。*

对于 $F$ 中每个 0 的闭合、平衡、凸邻域 $V$，存在一个 $\rho > 0$ 使得 $f(T) \subset \rho V$；因此，$f(T)$的封闭、平衡、凸包络$B$包含在$\rho V$中，并且到假设为止是完整的。如果$\| \lambda \| \leq 1/\rho$，则根据第8条命题No. 2和关系$\| \lambda \| = \lambda^+(T) + \lambda^-(T)$，得出$\int f\, d\lambda \in B/\rho \subset V$。

### 7. 应用程序：II。 扩张、空间措施、连续函数以及空间运算符中的值

令$G$为Hausdorff局部凸空间，$H$为Hausdorff及拟完全局部凸空间，并用$G$的连续线性映射的$F$空间$\mathscr{L}(G; H)$表示为$H$，配备*紧凑收敛*的拓扑。 空间$F$不一定是准完备的，如果$t \mapsto U(t)$是$T$到$F$的连续映射，并且$\mu$是具有紧支持的$T$的正测度，则不一定有$\int U\, d\mu \in F$（Exer. 27）。然而，如果对于$T$的每个紧致子集$K$，$U(K)$是*等连续的*，那么它在$F$中的平衡凸包络也是等连续的（TVS，III, §3, No. 4），并且由于$H$是准完全的，所以这个平衡凸包络的闭包将是一个完全的子集 / $F$（TVS，III, §3, No. 8，提案 11）；那么确实会有 $\int U\, d\mu \in F$（No. 2，提案 8）。

对$U$施加的补充条件可以用其他方式表示：

#### 引理 3 {#int-vi-s1-lem-3 .statement tag=0996}

*设$G, H$是局部紧致空间$T$到$\mathscr{L}(G; H)$的两个局部凸空间、$U$映射。以下条件是等效的：
a) $T \times G$到$H$的映射$(t, x) \mapsto U(t) \cdot x$是连续的。
b) 对于$T$的每个紧凑子集$K$，$U(K)$是等连续的，并且存在总共集合$D \subset G$，使得对于每个$x \in D$，映射$t \mapsto U(t) \cdot x$在$T$上连续。*

此外，当$U$满足这些条件时，$U$是$T$到$\mathscr{L}(G; H)$的连续映射，配备有紧收敛的拓扑。

为了看出a)蕴含b)，我们观察到对于$H$中的每个0的邻域$V$和每个$t \in K$，假设存在$T$中的$t$的邻域$L_t$和$G$中的0的邻域$W_t$，使得关系 $t' \in L_t$ 和$x \in W_t$ 意味着$U(t') \cdot x \in V$。只要用有限的数邻域$L_{t_i}$覆盖$K$，并且每当$t \in K$和$x \in W$时，在阶中取$W = \bigcap_i W_{t_i}$就可以得到$U(t) \cdot x \in V$，这就证明了$U(K)$的等连续性。

反之，假设b)得到验证；足以证明对于$T$的每个紧凑子集$K$，映射$(t, x) \mapsto U(t) \cdot x$在$K \times G$上连续。设 $M = U(K)$；由于$M$是等连续的，因此在$M$上，$G$中的逐点收敛的拓扑与$D$中的逐点收敛的拓扑相同（GT，X, §2, No. 4，Th.1）； 假设 b) 因此意味着，当 $\mathscr{L}(G; H)$ 配备了拓扑逐点收敛时，$t \mapsto U(t)$ 是$K$ 到 $\mathscr{L}(G; H)$ 的连续映射。另一方面，当$M$配备了逐点收敛的拓扑时，$(A, x) \mapsto A \cdot x$是$M \times G$到$H$的连续映射（GT，X, §2, No. 1，Prop.1的Cor.4）。由于映射$(t, x) \mapsto U(t) \cdot x$可以因式分解为$(t, x) \mapsto (U(t), x) \mapsto U(t) \cdot x$，所以结论它是连续的。

最后，引理的最后一个断言源自以下事实：在$M$上，紧致收敛的拓扑与逐点收敛相同（GT，X, §2, No. 4，Th.1）。

因此，假设$U$满足引理3中的条件；然后（如果$H$是准完整的）一个定义，如No. 6、线性映射$\lambda \mapsto \int U d\lambda$将$\mathscr{C}'(T)$放入$F = \mathscr{L}(G; H)$。我们集合$U(\lambda) = \int U d\lambda$。

#### 命题 16 {#int-vi-s1-prop-16 .statement tag=0997}

— 令 $G, H$ 为两个 Hausdorff 局部凸空间，其中 $H$ 假设为准完备。令$U$是$T$到$\mathscr{L}(G; H)$的映射，使得$(t, x) \mapsto U(t) \cdot x$是$T \times G$到$H$的连续映射。那么$\mathscr{C}'(T) \times G$到$H$的双线性映射$(\lambda, x) \mapsto U(\lambda) \cdot x$相对于$\mathscr{C}'(T)$的等连续子集和$G$的紧子集来说是低连续的（这意味着$\mathscr{C}'(T)$的线性映射$\lambda \mapsto U(\lambda)$）到 $F$ 是连续的）。

$\lambda \mapsto U(t)$作为$\mathscr{C}'(T)$的映射到$F$的连续性源自No. 6第14条命题之后的引理3和注2。因而，还需要证明对于 $H$ 中每个闭、平衡、凸邻域 0 的$V$ 以及对于 $\mathscr{C}'(T)$ 的每个等连续子集 $N$，在 $G$ 中存在一个 0 的邻域 $W$，使得关系 $x \in W, \lambda \in N$ 意味着$U(\lambda) \cdot x \in V$。我们可以假设$N = S^\circ$，其中$S$是$\mathscr{C}(T)$中0的邻域，因此我们可以假设$S$是函数$g \in \mathscr{C}(T)$的集合，使得$|g(t)| \leq 1$在紧凑的子集$K$上$T$。足以证明

|⟨U(λ)·x, x′⟩| ≤ 1，对于 x ∈ W、x′ ∈ V° 且 λ ∈ S°。现在，由于 U(K) 是等连续的，因此 G 中存在 0 的邻域 W，使得关系 t ∈ K，x ∈ W 意味着 U(t) · x ∈ V； 关系 x ∈ W, x′ ε V° 因此意味着函数 t ↦ ⟨U(t) · x, x′⟩ 属于到 S，因此 |⟨U(t) · x, x′⟩| = |∫⟨U(t)·x, x′⟩ dλ(t)| ≤ 1 × S° 的定义。

现在我们假设 U 是 T 到 F 的连续映射，而且 U(T) 是等连续的。然后，与上面相同的推理表明（因为 H 是准完备的），对于 T 上的每个有界正测度 μ，∫ U dμ ∈ F。因此可以定义，如上，线性映射 λ ↦ ∫ U dλ = U(λ) of M^1(T) into F that 扩展类似C'(T) 的映射进入 F。此外，对于 H 中每一个封闭、平衡、凸邻域 0 的V，在 G 中存在假设 0 的邻域 W，这样对于每一个 x ∈ W 且每一个 t ∈ T，都有 U(t) · x ∈ V，因而（因为 V 是弱闭) ∫ (U(t) · x)dλ(t) ∈ ||λ|| · V（No. 2，提案 5）。其他字：

#### 命题 17 {#int-vi-s1-prop-17 .statement tag=0998}

— 令 G、H 为两个 Hausdorff 局部凸空间，假设 H 是准完备的。令 U 为 T 的映射到 L(G; H) 中，使得 (t, x) ↦ U(t) · x 在 T × G 上连续，且 U(T) 等连续。然后，如果 M^1(T) 配备其 Banach 空间拓扑，则 M^1(T) × G 到 H 的双线性映射 (λ, x) ↦ U(λ) · x 是连续的（这特别意味着，当 M^1(T) 到 L(G; H) 的线性映射 λ ↦ U(λ) 是连续的） L(G; H) 配备有界收敛的拓扑）。

#### 命题 18 {#int-vi-s1-prop-18 .statement tag=0999}

— 令 G_1、G_2、H_1、H_2 为四个 Hausdorff 局部凸空间，假设 H_1 和 H_2 是准完备的。设A : G_1 → G_2 和B : H_1 → H_2 为两个连续的线性映射。令 U_1 : T → L(G_1; H_1), U_2 : T → L(G_2; H_2) 为第 16 条命题（或第 17 条命题）的两个映射满足条件，并假设对于每个 t ∈ T，B ◦ U_1(t) = U_2(t) ◦ A。然后，对于 T 上具有紧凑支持的每个测度（分别是每个有界测度）λ，B ◦ U_1(λ) = U_2(λ) ◦ A。

事实上，对于每一个 x ∈ G_1，都有 (No. 1，命题 1)

$$
(B \circ U_1(\lambda)) \cdot x = \int \left( (B \circ U_1(t)) \cdot x \right) d\lambda(t)
$$
$$
= \int \left( (U_2(t) \circ A) \cdot x \right) d\lambda(t) = U_2(\lambda) \cdot (A \cdot x).
$$

#### 注 1 {#int-vi-s1-n7-rem-1 .statement tag=099A}

假设 G 和 H 是 Banach 空间，并设 U 是 T 的映射到 L(G; H)，使得 (t, x) ↦ U(t) · x 在 T × G 上连续。 注这意味着有限函数 t ↦ \|U(t)\|在 T 的每个紧凑子集和 T 上的下半连续上有界，是连续函数 $t \mapsto |U(t) \cdot x|$ 的上包络线，因为 $x$ 在 G 中越过球$|x| \leq 1$。 集合 $h(t) = \| U(t) \|$。然后，对于 T 上的每个正测度$\mu$，使得 $h$ 是 $\mu$ 可积，我们再次有 $\int U d\mu \in \mathscr{L}(G; H)$。因为，测量$\nu = h \cdot \mu$以假设为界；因此，存在由 $\nu$ 可忽略的集合 N 和紧致子集的序列 $(K_n)$ 形成的 T 的划分。本号开头提出的论点适用于措施$\varphi_{K_n} \cdot \mu$，表明

$$
A_n = \int \varphi_{K_n} U \, d\mu \in F = \mathscr{L}(G; H),
$$

而且，（No. 2，提案 6），$\| A_n \| \leq \int \varphi_{K_n} \| U \| \, d\mu \leq \nu(K_n)$。因此，级数与一般项$A_n$绝对收敛于Banach空间$\mathscr{L}(G; H)$，且其和为$\int U \, d\mu$及$\| \int U \, d\mu \| \leq \int \| U \| \, d\mu$为直接的。

#### 注 2 {#int-vi-s1-n7-rem-2 .statement tag=099B}

假设$G = H$是准完备的，并且$U$满足第16条命题的假设。令M为空间$\mathscr{C}'(T)$的稠密子集，对于弱拓扑$\sigma(\mathscr{C}'(T), \mathscr{C}(T))$，并令X为闭线性H 的子空间使得对于每个测量 $\lambda \in M$ 都有 $U(\lambda)(X) \subset X$。然后还有$U(t)(X) \subset X$对于每个$t \in T$：实际上，对于每个$x \in X$和每个与X正交的$x' \in H'$，对于所有$\lambda \in M$来说假设$\langle U(\lambda) \cdot x, x' \rangle = 0$，可以写成$\int \langle U(t) \cdot x, x' \rangle \, d\mu(t) = 0$。因此，与 M 正交的连续函数 $t \mapsto \langle U(t) \cdot x, x' \rangle$ 为 0，对于每个 $x' \in X^\circ$ 产生 $\langle U(t) \cdot x, x' \rangle = 0$，对于所有 $t \in T$ 和 $x \in X$ 产生从而 $U(t) \cdot x \in X$，这证明了我们的断言。

### 习题{#int-vi-s1-exercises}

§ 1](exercises/s1/)参见[习题。
