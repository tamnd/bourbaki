---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 1
section_title: Construction of a Haar measure
lang: zh
source: int-vii-ix
pdf_pages: 0007-0032, 0084-0093
extraction: ocr
subsections:
    - "no": 1
      title: Definitions and notations
      page: 0
      pdf_page: 7
    - "no": 2
      title: The existence and uniqueness theorem
      page: 6
      pdf_page: 12
    - "no": 3
      title: Modulus
      page: 10
      pdf_page: 16
    - "no": 4
      title: Modulus of an automorphism
      page: 13
      pdf_page: 19
    - "no": 5
      title: Haar measure of a product
      page: 14
      pdf_page: 20
    - "no": 6
      title: Haar measure of an inverse limit*
      page: 15
      pdf_page: 21
    - "no": 7
      title: Local definition of a Haar measure
      page: 18
      pdf_page: 24
    - "no": 8
      title: Relatively invariant measures
      page: 19
      pdf_page: 25
    - "no": 9
      title: Quasi-invariant measures
      page: 20
      pdf_page: 26
    - "no": 10
      title: Locally compact fields
      page: 21
      pdf_page: 27
    - "no": 11
      title: Finite-dimensional algebras over a locally compact field
      page: 25
      pdf_page: 31
statements: 42
exercises: 30
content_sha256: 826a0b059505119474ce418ddb246b0735fb3f4c1aa83635f1b80fa492f483d6
translated_from: content/en/int/VII/01_s1_construction_of_a_haar_measure.md
translation_method: google
source_content_sha256: e46166486e36efa944d66af30ebaacb93e9bc8f019659598c1d03449537e5e11
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 9e866c08996d498993831d4a81da0d64f5880604af2e8c4ed828fb66a47f1bab
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。 HAAR 措施的构造

### 1. 定义和记号

设 G 是一个在局部紧凑空间 X 中连续在左侧运行的拓扑群（GT，III, §2, No. 4）；对于$s \in G$和$x \in X$，令$sx$为$x$乘$s$的变换。我们用 $\gamma_X(s)$ 或 $\gamma(s)$ 表示 X 到 X 的同胚，定义为

(1)
$$
\gamma(s)x = sx.
$$

我们有

(2)
$$
\gamma(st) = \gamma(s)\gamma(t).
$$

如果$f$是$X$上定义的函数，则$\gamma(s)f$将由结构的迁移定义，即公式$(\gamma(s)f)(\gamma(s)x) = f(x)$；在其他字，

(3)
$$
(\gamma(s)f)(x) = f(s^{-1}x).
$$

如果$\mu$是在$X$上定义的测度，则$\gamma(s)\mu$也将由结构的迁移定义，这导致

(4)
$$
\langle f, \gamma(s)\mu \rangle = \langle \gamma(s^{-1})f, \mu \rangle \quad \text{for } f \in \mathscr{K}(X).
$$

在其他字，

(5)
$$
\int_X f(x) d(\gamma(s)\mu)(x) = \int_X f(sx) d\mu(x).
$$

如果 $A$ 是 $(\gamma(s)\mu)$ 可积集合，则 $s^{-1}A$ 是 $\mu$ 可积，并且

(6)
$$
(\gamma(s)\mu)(A) = \mu(s^{-1}A).
$$

度量$\gamma(s)\mu$也可以定义为$\gamma(s)$下$\mu$的*像*。

写 $d\mu(s^{-1}x)$ 代替写 $d(\gamma(s)\mu)(x)$ 是有用的有时； 公式 (5) 然后取以下形式：

$$
\int_X f(x) d\mu(s^{-1}x) = \int_X f(sx) d\mu(x);
$$

然后可以通过“替换$x$乘$sx$”从左侧推导出右侧的表达式。

#### 定义 1 {#int-vii-s1-def-1 .statement tag=09CY}

*让$\mu$作为$X$的度量。*
a) $\mu$ *如果 $\gamma(s)\mu = \mu$ *对于每个* $s \in G$，则在 $G$* 下被认为是不变的。
b) 如果对于每个* $s \in G$，$\gamma(s)\mu$ *与* $\mu$ *成比例，则$\mu$ *在$G$*下被认为是相对不变的。
c) $\mu$ *如果 $\gamma(s)\mu$ *等价于* $\mu$ *对于每个* $s \in G$，则称$G$*下是准不变的。

#### 注 {#int-vii-s1-n1-rem-1 .statement tag=09CZ}

— 1) 假设 $\mu$ 不变。那么$|\mu|$，$\mathscr{R}(\mu)$，$\mathscr{I}(\mu)$是不变的。如果$\mu$是实数，则$\mu^+$和$\mu^-$是不变的。
2) 假设$\mu$相对不变且非零的。对于每个$s \in G$，都存在一个唯一的复数$\chi(s)$，使得

(7)
$$
\gamma(s)\mu = \chi(s)^{-1}\mu,
$$

$G$上的函数$\chi$是$\mathbf{C}^*$中$G$的表示，称为$\mu$的*乘子*。 公式 (5) 然后给出

$$
(8) \quad \int_X f(sx)\, d\mu(x) = \chi(s)^{-1} \int_X f(x)\, d\mu(x),
$$

公式 (6) 给出

$$
(9) \quad \mu(sA) = \chi(s) \mu(A).
$$

根据上面的约定，(7) 也可以写成

$$
(10) \quad d\mu(sx) = \chi(s)\, d\mu(x).
$$

3) 由于$|\gamma(s)\mu| = \gamma(s)(|\mu|)$，说$\mu$是准不变的相当于说，$|\mu|$是准不变的。

如果$\mu$是准不变的并且$\mu'$是$X$上的另一个测度等于$\mu$，则$\gamma(s)\mu'$等于$\gamma(s)\mu$，因此等于$\mu$，因此等于$\mu'$，等等$\mu'$ 是准不变的。因此，说$\mu$在$G$下是准不变的，意味着$\mu$的*类*在$G$下是不变的。

为了使$\mu$是准不变的，$X$的局部$\mu$可忽略的子集的集合在$G$（第V, §5, No. 5，Th.2）下保持不变，或者同样，对于每个$\mu$-可忽略的紧凑$X$的子集$K$，并且对于每个$s \in G$，$sK$是$\mu$-可忽略不计（*loc.cit.*，*注*）。

如果$\mu$是准不变的，那么$\mu$的支持度在$G$下是不变的。特别是，如果$G$在$X$（A，I, §5, No. 5，Def.6）中是“传递”的，则该支持要么为空（如果$\mu = 0$），要么等于$X$（如果$\mu \neq 0$）。

#### 引理 1 {#int-vii-s1-lem-1 .statement tag=09D0}

— *令$X, Y, Z$为三个拓扑空间，且$Y$局部紧致。令$(x, y) \mapsto xy$为$X \times Y$到$Z$的连续映射，其中$X$的定义映射$x \mapsto u_x$经关系$u_x(y) = xy$到$\mathscr{F}(Y; Z)$。设$f$是$Z$上的连续函数，$\mathbf{R}$或Banach空间中的值，S是$f$的支持，$\mu$是$Y$上的测度。假设对于每个$x_0 \in X$，$X$中存在$x_0$的邻域$V$，使得$\bigcup_{x \in V} u_x^{-1}(S)$在$Y$中相对紧凑。然后：
a) 对于每个$x \in X$，$f \circ u_x$在$Y$上连续，有紧支撑；
b) 由a)定义的映射$x \mapsto \int_Y f(xy)\, d\mu(y)$在$X$上连续。

断言 a) 是显而易见的。让我们证明b)。由于连续性是局部性质，因此我们可以将约化应用于$\bigcup_{x \in X} u_x^{-1}(S)$包含在$Y$的紧凑子集$Y'$中的情况。由于函数 $(x, y) \mapsto f(xy)$ 在 $X \times Y$ 上连续，因此 $f \circ u_x$ 在 $Y'$ 上一致趋向于 $f \circ u_{x_0}$，因为 $x$ 趋向于 $x_0$

（GT，X, §3, No. 4，Th.3），因此$\mu(f \circ u_x)$趋于$\mu(f \circ u_{x_0})$。 从而引理。

现在让我们回到之前的记号。

#### 命题 1 {#int-vii-s1-prop-1 .statement tag=09D1}

— *假设 G 是局部紧致的。令$\mu$为非零的在X上的相对不变测度。那么它的乘子$\chi$就是G上的连续函数。*

设$f \in \mathscr{K}(X)$，S是G的$f$、$s_0$点的支持，V是G中$s_0$的紧邻域；那么集合

$$
\bigcup_{s \in V} \gamma(s)^{-1}(S) = V^{-1}S
$$

在 X 内是紧致的；由引理 1 和公式 (8)，$\chi(s^{-1}) \langle \mu, f \rangle$ 连续依赖于 $s$；如果选择$f$使得$\langle \mu, f \rangle \neq 0$，则可以看到$\chi$是连续的。

现在让 G 是一个在局部紧凑空间 X 中连续在右侧运行的拓扑群；对于$s \in G$和$x \in X$，令$xs$等于$x$除以$s$的变换。我们用 $\delta_X(s)$ 或 $\delta(s)$ 表示 X 的同胚，定义为

(1')
$$
\delta(s)x = xs^{-1}.
$$

我们有

(2')
$$
\delta(st) = \delta(s)\delta(t).
$$

截至结构的迁移、函数的$\delta(s)$的定义作用以及X的措施：

(3')
$$
(\delta(s)f)(x) = f(xs)
$$
(4')
$$
\langle f, \delta(s)\mu \rangle = \langle \delta(s^{-1})f, \mu \rangle
$$
(5')
$$
\int_X f(x) d(\delta(s)\mu)(x) = \int_X f(xs^{-1}) d\mu(x)
$$
(6')
$$
(\delta(s)\mu)(A) = \mu(As).
$$

我们同意写 $d\mu(xs)$ 代替 $d(\delta(s)\mu)(x)$，然后 (5') 取形式

$$
\int_X f(x) d\mu(xs) = \int_X f(xs^{-1}) d\mu(x).
$$

一个定义以类似的方式在G下对X的测量不变，相对不变和准不变。如果$\mu$相对不变，则其乘子$\chi$由公式定义

$$
(7') \quad \delta(s)\mu = \chi(s)\mu
$$
$$
(8') \quad \int_X f(xs)\,d\mu(x) = \chi(s)^{-1} \int_X f(x)\,d\mu(x)
$$
$$
(9') \quad \mu(As) = \chi(s)\mu(A)
$$
$$
(10') \quad d\mu(xs) = \chi(s)\,d\mu(x).
$$

如果将与G相反的群$G^0$视为$(x,s) \mapsto xs$在X中运算，则$\mu$在$G^0$下相对不变，乘子$\chi$相同。

最后，令 G 为局部紧致群。根据公式$\gamma(s)x = sx$、$\delta(s)x = xs^{-1}$，它通过左右翻译自行运行。然后

$$
(11) \quad \gamma(s)\delta(t) = \delta(t)\gamma(s).
$$

上述所有内容都适用于此，因此我们在 G 上的测度概念是*左不变*、*右不变*、*相对左不变*、*相对右不变*、*左准不变*、*右准不变*（但是，请参见第 8 条和第 9 条）。

映射 $x \mapsto x^{-1}$ 是 G 到 G 的同胚。对于 G 上的每个函数 $f$，我们在 G 上定义函数 $\check{f}$

$$
(12) \quad \check{f}(x) = f(x^{-1}).
$$

对于 G 上的每个测度 $\mu$，我们定义测度 $\check{\mu}$ 为

$$
(13) \quad \check{\mu}(f) = \mu(\check{f}) \quad \text{for } f \in \mathscr{K}(G).
$$

在其他字，

$$
(14) \quad \int_G f(x)\,d\check{\mu}(x) = \int_G f(x^{-1})\,d\mu(x).
$$

如果 A 是 $\check{\mu}$ 可积集合，则 $A^{-1}$ 是 $\mu$ 可积，并且

$$
(15) \quad \check{\mu}(A) = \mu(A^{-1}).
$$

我们同意写$d\mu(x^{-1})$代替$d\check{\mu}(x)$，然后(14)取形式

$$
\int_G f(x)\, d\mu(x^{-1}) = \int_G f(x^{-1})\, d\mu(x).
$$

### 2. 存在和唯一性定理

#### 定义 2 {#int-vii-s1-def-2 .statement tag=09D2}

*设 G 为局部紧致群。 非零的 G 上左（或右）不变的正测度称为 G 上的左（或右）Haar 测度。*

#### 定理 1 {#int-vii-s1-thm-1 .statement tag=09D3}

*在每个局部紧凑群上，都存在一个左（或右）哈尔测度，并且，直到常数因子，只存在一个。*

A) *存在。* — 集合 $\mathscr{K}(G) = \mathscr{K}$、$\mathscr{K}_+(G) = \mathscr{K}_+$、$\mathscr{K}_+^* = \mathscr{K}_+ - \{0\}$。如果C是G的紧子集，我们用$f \in \mathscr{K}_+^*$的$\mathscr{K}_+^*(C)$集合表示，并在C中提供支持。对于$f \in \mathscr{K}$和$g \in \mathscr{K}_+^*$，G中存在数、$c_1, \ldots, c_n \geq 0$和元素$s_1, \ldots, s_n$，使得$f \leq \sum_{i=1}^n c_i \gamma(s_i)g$：对于，G中存在非空开集合U，使得$\inf_{s \in U} g(s) > 0$，并且支持$f$ 可以被 U 的有限数左翻译覆盖。令 $(f : g)$ 为数 $\sum_{i=1}^n c_i$ 的下确界，对于数 $\geq 0$ 和元素的所有系统 $(c_1, \ldots, c_n, s_1, \ldots, s_n)$ G 使得$f \leq \sum_{i=1}^n c_i \gamma(s_i)g$。然后：

(i) $(\gamma(s)f : g) = (f : g)$ 代表 $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$s \in G$；
(ii) $(\lambda f : g) = \lambda(f : g)$代表$f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$\lambda \geq 0$；
(iii) $((f + f') : g) \leq (f : g) + (f' : g)$代表$f \in \mathscr{K}$、$f' \in \mathscr{K}$、$g \in \mathscr{K}_+^*$；
(iv) $(f : g) \geq (\sup f)/(\sup g)$ 代表$f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$；
(v) $(f : h) \leq (f : g)(g : h)$ 代表 $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$h \in \mathscr{K}_+^*$；
(vi) $\mathscr{K}_+^*$中的$f, f_0, g$为$0 < \frac{1}{(f_0 : f)} \leq \frac{(f : g)}{(f_0 : g)} \leq (f : f_0)$；
(vii) 令$f, f', h$在$\mathscr{K}_+$与$h(s) \geq 1$在$f + f'$的支持下，并令$\varepsilon > 0$； e 存在一个紧邻域 V，对于每个 $g \in \mathscr{K}_+^*(V)$，

$$
(f : g) + (f' : g) \leq ((f + f') : g) + \varepsilon(h : g).
$$

性质 (i)、(ii)、(iii) 是显而易见的。 设$f \in \mathscr{K}$，$g \in \mathscr{K}_+^*$；如果 $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ 与 $c_i \geq 0$，则 $\sup f \leq \sum_{i=1}^n c_i g(s_i^{-1}s)$ 对于 G 中的某些 s \，因而 $\sup f \leq (\sum_{i=1}^n c_i) \sup g$，从而 (iv)。 现在让我们证明(v)；让$f \in \mathscr{K}$，$g, h$进入$\mathscr{K}_+^*$；如果$f \leq \sum_{i=1}^n c_i \gamma(s_i)g$和$g \leq \sum_{j=1}^p d_j \gamma(t_j)h$（$G$中的$c_i \geq 0, d_j \geq 0, s_i, t_j$），则$f \leq \sum_{i,j} c_i d_j \gamma(s_i t_j)h$，因而$(f : h) \leq \sum_{i,j} c_i d_j = (\sum_i c_i)(\sum_j d_j)$；因而$(f : h) \leq (f : g)(g : h)$。 一方面应用(v)到$f_0, f, g$，另一方面到$f, f_0, g$，得到(vi)。 最后，让$f, f', h$在$\mathscr{K}_+$和$h(s) \geq 1$在$f + f'$的支持下，并让$\varepsilon > 0$。 集合$F = f + f' + \frac{1}{2} \varepsilon h$； 函数$\varphi, \varphi'$，即重合分别与$f/F$和$f'/F$在$f + f'$的支撑上，在其之外是零，属于至$\mathscr{K}_+$；对于每个$\eta > 0$，都存在$e$的紧凑邻域$V$，使得$|\varphi(s) - \varphi(t)| \leq \eta$和$|\varphi'(s) - \varphi'(t)| \leq \eta$对应于$s^{-1} t \in V$。 然后让$g \in \mathscr{K}_+^*(V)$；对于每个$s \in G$，

$$
\varphi \cdot \gamma(s)g \leq (\varphi(s) + \eta) \cdot \gamma(s)g;
$$

因为，这在点处很明显，其中$\gamma(s)g$是零，因此在$sV$之外；以及$sV$、$\varphi \leq \varphi(s) + \eta$；同样，$\varphi' \cdot \gamma(s)g \leq (\varphi'(s) + \eta) \cdot \gamma(s)g$。也就是说，令$c_1, \ldots, c_n$为$G$的数$\geq 0$和$s_1, \ldots, s_n$元素，使得$F \leq \sum_{i=1}^n c_i \gamma(s_i)g$；然后

$$
f = \varphi F \leq \sum_{i=1}^n c_i \varphi \cdot \gamma(s_i)g \leq \sum_{i=1}^n c_i (\varphi(s_i) + \eta) \cdot \gamma(s_i)g
$$

对于 $f'$ 也类似；最后

$$
(f : g) + (f' : g) \leq \sum_{i=1}^n c_i (\varphi(s_i) + \varphi'(s_i) + 2\eta) \leq (1 + 2\eta) \sum_{i=1}^n c_i
$$

从$\varphi + \varphi' \leq 1$开始。 应用定义 of $F$，则 (ii)、(iii) 和 (v)，可推出

$$
(f : g) + (f' : g) \leq (1 + 2\eta)(F : g) \leq
$$
$$
(1 + 2\eta)[((f + f') : g) + \frac{1}{2}\varepsilon(h : g)] \leq
$$
$$
(((f + f') : g) + \frac{1}{2}\varepsilon(h : g) + 2\eta((f + f') : h)(h : g) + \varepsilon\eta(h : g)
$$

并且，如果已选择$\eta$使得$\eta[2((f + f') : h) + \varepsilon] \leq \frac{1}{2}\varepsilon$，则获得(vii)。

由于 V 运行在 e 的紧邻域集合上，$\mathscr{K}_+^*$ 上的过滤器 $\mathscr{B}$ 的 $\mathscr{K}_+^*(V)$ 形式基。令$\mathscr{F}$为$\mathscr{K}_+^*$更细而非$\mathscr{B}$上的超滤器。另一方面，让我们固定$f_0 \in \mathscr{K}_+^*$并让我们集合，对于$f \in \mathscr{K}_+^*$和$g \in \mathscr{K}_+^*$，

$$
I_g(f) = \frac{(f : g)}{(f_0 : g)}.
$$

由(vi)，$\lim_{g,\mathscr{F}} I_g(f) = I(f)$存在于紧致空间$[1/(f_0 : f), (f : f_0)]$中。

由(iii)，$I(f + f') \leq I(f) + I(f')$。通过(vii)，对于所有$\varepsilon > 0$，$I(f) + I(f') \leq I(f + f') + \varepsilon I(h)$假设$h$在$f + f'$的支持下是$\geq 1$；由此可见$I(f + f') = I(f) + I(f')$。由 Ch. II, §2, No. 1，第 2 条，I 在 $\mathscr{K}$ 上可扩展到线性形式；这个线性形式是 G 上的非零的正测度，对 (i) 左不变；这就是人们所寻求的左哈尔措施。 经过与相反的群，由此推断存在正确的 Haar 测度。

B) *唯一性.* — 令 $\mu$ 为左 Haar 测度，$\nu$ 为右 Haar 测度。那么$\check{\nu}$就是左哈尔测度。我们将证明 $\mu$ 和 $\check{\nu}$ 成比例。这将证明任意两个左哈尔测度确实是成比例的。

令$f \in \mathscr{K}$ 使得$\mu(f) \neq 0$。由引理 1，函数 $D_f$ 在 G 上由公式定义

$$
D_f(s) = \mu(f)^{-1} \int f(t^{-1}s) d\nu(t)
$$

在 G 上连续。设 $g \in \mathscr{K}$。 函数 $(s, t) \mapsto f(s)g(ts)$ 与$G \times G$ 中的紧凑支撑连续。由 Ch. III, §4, No. 1，周四。 2、

$$
\begin{align*}
\mu(f)\nu(g) &= \left( \int f(s) d\mu(s) \right) \left( \int g(t) d\nu(t) \right) \\
&= \int d\mu(s) \int f(s)g(ts) d\nu(t) = \int d\nu(t) \int f(s)g(ts) d\mu(s) \\
&= \int d\nu(t) \int f(t^{-1}s)g(s) d\mu(s) \\
&= \int g(s) \left[ \int f(t^{-1}s) d\nu(t) \right] d\mu(s) = \mu(g \cdot \mu(f) D_f),
\end{align*}
$$

从而

$$
\nu(g) = \mu(D_f \cdot g).
$$

这首先证明$D_f$不依赖于$f$。因为，如果$f' \in \mathscr{K}$使得$\mu(f') \neq 0$，则$D_f \cdot \mu = D_{f'} \cdot \mu$，因此$D_f = D_{f'}$在局部几乎处处对于$\mu$，因此处处，因为$D_f$和$D_{f'}$是连续的并且$\mu$的支持度是$G$。因此我们可以写$D_f = D$。 公式 (16) 给出

$$
\mu(f)D(e) = \check{\nu}(f).
$$

公式 (19) 可以通过线性扩展至函数 $f \in \mathscr{K}$，使得$\mu(f) = 0$。自$\check{\nu} \neq 0$以来，我们有$D(e) \neq 0$。这确实建立了$\mu$和$\check{\nu}$的比例。

#### 推出{#int-vii-s1-n2-cor-1 .statement tag=09D4}

— *每个左不变式*（分别为*右不变式*）*测量*$G$*与左*（分别为*右*）*哈尔测量*成比例。

#### 例 {#int-vii-s1-n2-exa-1 .statement tag=09D5}

— 1) 在加法群$\mathbf{R}$，勒贝格测度$dx$是哈尔测度（第III, §1, No. 3，*例*）。

2) 对于每个函数 $f \in \mathscr{K}(\mathbf{R}_+^*)$，我们有 (FRV, II, §1, 公式 (12))

$$
\int_0^{+\infty} \frac{f(x)}{x} dx = \int_0^{+\infty} \frac{f(tx)}{tx} t dx = \int_0^{+\infty} \frac{f(tx)}{x} dx
$$

对于所有$t > 0$；因此，测度$x^{-1} dx$是乘法群$\mathbf{R}_+^*$的哈尔测度。

3) 让我们取$G$环面$T = \mathbf{R}/\mathbf{Z}$。令$\varphi$为$\mathbf{R}$到$T$的典范映射。对于 $f \in \mathscr{K}(T)$，函数 $f \circ \varphi$ 是连续且周期性的，在 $\mathbf{R}$ 上周期为 1，且积分

$$
I(f) = \int_a^{a+1} f(\varphi(x)) dx
$$

独立于选择或 $a \in \mathbf{R}$； 直接的平移不变；因此，定义是$T$的哈尔测度。通过结构的迁移，由此推出$I(f) = \int_a^{a+1} f(e^{2\pi i t}) dt$是绝对值1（GT，VIII, §2, No. 1）的复数的乘法群$U$的哈尔测度。

#### 命题 2 {#int-vii-s1-prop-2 .statement tag=09D6}

— *让* $G$ *成为局部紧凑的群*，$\mu$ *左或右哈尔测量* $G$。 *对于* $G$ *要离散，* $\mu(\{e\}) > 0$ 是必要且充分的。 *为了*$G$*要紧凑，*$\mu^*(G) < +\infty$是必要且充分的。

条件显然是必要的。让我们展示他们的充足性。设$V$是$e$的紧邻域。如果$\mu(\{e\}) > 0$，则$V$是自$\mu(V) < +\infty$以来的有限集合；由于 $G$ 是 Hausdorff，因此它是离散的。假设 $\mu^*(G) < +\infty$ 和 $\mu$ 对于例是左不变的。考虑集合$\mathscr{E}$/有限子集$\{s_1, \ldots, s_n\}$/$G$，使得$s_i V \cap s_j V = \varnothing$对应$i \neq j$；那么

$$
n \mu(V) = \mu(s_1 V \cup \ldots \cup s_n V) \leq \mu^*(G),
$$

因此$n \leq \mu^*(G)/\mu(V)$。因此，我们可以将选择放入$\mathscr{E}$极大元素$\{s_1, \ldots, s_n\}$。那么，对于每个$s \in G$，都存在一个$i$使得$s V \cap s_i V \neq \varnothing$，因此使得$s \in s_i V V^{-1}$。因此$G$是紧集$s_i V V^{-1}$的并，因此是紧致的。

### 3. 模数

令$\mu$为$G$的左哈尔测度。对于每个$s \in G$，$\delta(s)\mu$也是左不变的（No. 1，公式（11）），因此（Th.1）存在一个唯一的数$\Delta_G(s) > 0$，使得$\delta(s)\mu = \Delta_G(s)\mu$。凭借Th。 1、数$\Delta_G(s)$独立于$\mu$的选择。

#### 定义 3 {#int-vii-s1-def-3 .statement tag=09D7}

*$G$上的函数$\Delta_G$称为$G$的模（或模函数）。如果 $\Delta_G = 1$、群 $G$ 被称为幺模。*

也可以说$\mu$与乘子$\Delta_G$相对右不变。因此$\Delta_G$是$\mathbf{R}_+^*$*中$G$的*连续表示（No. 1，命题1）。

#### 注 {#int-vii-s1-n3-rem-1 .statement tag=09D8}

— 如果 $\varphi$ 是 $G$ 的同构到局部紧凑的群 $G'$，则$\Delta_{G'} \circ \varphi = \Delta_G$。特别是：
1) 由于$x \mapsto x^{-1}$是$G$的同构到相反的群$G^0$，所以有$\Delta_{G^0} = \Delta_G^{-1}$。
2) 如果$\varphi$是$G$中的自同构，则$\Delta_G \circ \varphi = \Delta_G$。

让$s \in G$。然后：

$$
\delta(s)(\Delta_G^{-1} \cdot \mu) = (\delta(s)\Delta_G^{-1}) \cdot (\delta(s)\mu) = (\Delta_G(s)^{-1}\Delta_G^{-1}) \cdot (\Delta_G(s)\mu) = \Delta_G^{-1} \cdot \mu,
$$

因此$\Delta_G^{-1} \cdot \mu = \mu'$是正确的哈尔测度。由此，可以推断出$\gamma(s)\mu' = (\gamma(s)\Delta_G^{-1}) \cdot \mu = \Delta_G(s)(\Delta_G^{-1} \cdot \mu) = \Delta_G(s)\mu'$，因此，对于每一个正确的哈尔测度$\nu$，我们有$\gamma(s)\nu = \Delta_G(s)\nu$。由于 $\dot{\mu}$ 是右 Haar 测度，因此 $\dot{\mu} = a \Delta_G^{-1} \cdot \mu$ 具有常数 $a > 0$；由此可见

$$
\mu = a(\Delta_G^{-1} \cdot \mu)^{\vee} = a \Delta_G \cdot \dot{\mu} = a^2 \mu,
$$

因此$a = 1$，最后是$\dot{\mu} = \Delta_G^{-1} \cdot \mu$。人们也可以看到类似的$\dot{\nu} = \Delta_G \cdot \nu$。

因此我们得到以下结果：

处方集。 — 令 G 为局部紧致群，$\Delta$ 其模，$\mu$ 左哈尔测度，$\nu$ 右哈尔测度。

1) 一个有

$$
\gamma(s)\mu = \mu \quad \delta(s)\mu = \Delta(s)\mu \quad \check{\mu} = \Delta^{-1} \cdot \mu .
$$

如果$f$在G上是$\mu$可积，则$f$的左右平移是$\mu$可积，并且

$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
(21)
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x) .
$$

此外，$\check{f}$可积$\Delta^{-1} \cdot \mu$并且

$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x) .
$$
(22)

如果 A 是 G 的 $\mu$ 可积子集，则 sA 和 As 是 $\mu$ 可积，并且

$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A) .
$$
(23)

2) 一个有

$$
\delta(s)\nu = \nu \quad \gamma(s)\nu = \Delta(s)\nu \quad \check{\nu} = \Delta \cdot \nu .
$$

如果$f$在G上是$\nu$可积，那么$f$的左右平移是$\nu$可积并且

$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\nu(x)
$$
(25)
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x) .
$$

此外，$\check{f}$可积$\Delta \cdot \nu$并且

$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x) .
$$
(26)

如果 A 是 G 的 $\nu$ 可积子集，则 sA 和 As 是 $\nu$ 可积，并且

$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s)^{-1} \nu(A) .
$$
(27)

3) $\nu$与$\Delta^{-1} \cdot \mu$成正比，$\mu$与$\Delta \cdot \nu$成正比。

4) 假设 G 是*单模*。令 $\mu$ 为 G 上的 Haar 测度。则：

$$
\gamma(s)\mu = \delta(s)\mu = \dot{\mu} = \mu .
$$

如果$f$在G上是$\mu$可积，那么$f$的左右平移是$\mu$可积，$\check{f}$也是如此，并且

$$
\int f(sx)\,d\mu(x) = \int f(xs)\,d\mu(x) = \int f(x^{-1})\,d\mu(x) = \int f(x)\,d\mu(x) .
$$

如果 A 是 G 的 $\mu$ 可积子集，则 sA、As 和 $A^{-1}$ 是 $\mu$ 可积，并且

$$
\mu(sA) = \mu(As) = \mu(A^{-1}) = \mu(A) .
$$

类似的性质成立本质积分。

#### 命题 3 {#int-vii-s1-prop-3 .statement tag=09D9}

*如果 G 中存在内自同构下 e 不变量的紧邻域 V，则 G 是单模的。*

对于，令 $\mu$ 为 G 上的左 Haar 测度。对于每个 $s \in G$，

$$
\mu(V) = \mu(s^{-1}Vs) = \Delta_G(s)\mu(V) ,
$$

自$0 < \mu(V) < +\infty$起从而$\Delta_G(s) = 1$。

由此，人们立即推断出：

#### 推出 {#int-vii-s1-n3-cor-1 .statement tag=09DA}

*如果 G 是离散的、紧致的或可交换的，则 G 是幺模的。*

当 G 是“可交换的”时，这也是微不足道的。 注另外，如果 G 是*离散*，则每个点的质量为 1 的 G 上的测度显然是 G 上的左右 Haar 测度，称为 G 上的*归一化* Haar 测度。如果 G 是*紧凑*，则 G 上存在且仅有一个 Haar 测度，使得 $\mu(G) = 1$；它被称为 G 的“归一化”Haar 测度。当 G 既是离散的又是紧致的（即有限的）时，前面的两个约定不一致；当我们遇到这种情况时，我们将始终明确指定标准化哈尔测度的含义。

幺模群的子群和商群并不总是幺模（§ 2，Exer.5）。不过，请参阅§ 2, No. 7 的第 10 号提案。

*稍后我们将看到半单或幂零连通的李群是幺模的。*

### 4. 模数自同构

设G是G的局部紧群，$\varphi$自同构，$\mu$G上的左Haar测度。显然，$\varphi^{-1}(\mu)$也是G上的左Haar测度。因此存在(No. 2，Th.1)一个且仅有一个数 $a > 0$使得$\varphi^{-1}(\mu) = a \mu$。截至 No. 2，周四。 1、这个数独立于$\mu$的选择。 注如果一个人从正确的 Haar 测度开始，对于例 $\Delta_G^{-1} \cdot \mu$ (No. 3)，我们会得到相同的标量 $a$：因为，因为 $\varphi^{-1}$ 使 $\Delta_G$ 不变（No. 3，注），一个有 $\varphi^{-1}(\Delta_G^{-1} \cdot \mu) = \Delta_G^{-1} \cdot \varphi^{-1}(\mu) = a \Delta_G^{-1} \cdot \mu$。

#### 定义 4 {#int-vii-s1-def-4 .statement tag=09DB}

*数 $a > 0$，因而 $\varphi^{-1}(\mu) = a \mu$ 称为自同构 $\varphi$ 的模，并表示为 $\operatorname{mod}_G \varphi$ 或简称为 $\operatorname{mod} \varphi$。*

如果 $f$ 是 G 上的 $\mu$ 可积函数，则

$$
\int f(\varphi^{-1}(x)) d\mu(x) = (\operatorname{mod} \varphi) \int f(x) d\mu(x).
$$

如果 A 是 G 的 $\mu$ 可积子集，则

$$
\mu(\varphi(A)) = (\operatorname{mod} \varphi) \mu(A).
$$

特别地，对于$s \in G$，令$i_s$为内自同构$x \mapsto s^{-1} x s$。那么$i_s^{-1} = \delta(s) \gamma(s)$，因而

$$
i_s^{-1}(\mu) = \delta(s) \mu = \Delta_G(s) \mu,
$$

因而

$$
\operatorname{mod} i_s = \Delta_G(s).
$$

如果 G 是离散的或紧致的，则其归一化 Haar 测度会通过 G 的每个自同构 $\varphi$ 转换为自身，正如我们通过结构的迁移立即看到的那样。因而，离散或紧凑群的 *自同构的模数为 1*。

#### 命题 4 {#int-vii-s1-prop-4 .statement tag=09DC}

*设 G 为局部紧致群、$\Gamma$ 拓扑群，以及 $\Gamma$ 的 $\gamma \mapsto u_\gamma$ 同态到 G 的自同构的群 $\mathscr{G}$，使得 $(\gamma, x) \mapsto u_\gamma(x)$是G中$\Gamma \times G$的连续映射。那么，映射$\gamma \mapsto \operatorname{mod}(u_\gamma)$是$\mathbf{R}_+^*$中$\Gamma$的连续表示。

这个映射显然是$\mathbf{R}_+^*$中$\Gamma$的表示（代数）；足以证明其连续性。令 $f \in \mathscr{K}(G)$ 并令 S 为其支持。*

令$\gamma_0 \in \Gamma$和$U$是$u_{\gamma_0}^{-1}(S)$的相对紧凑邻域。 映射$\gamma \mapsto u_\gamma$是$\Gamma$到$\mathscr{G}$的连续映射，配备拓扑紧致收敛（GT、X, §3, No. 4、Th.3）；因此 $u_\gamma^{-1}(S) \subset U$ 对于 $\gamma$ 足够接近 $\gamma_0$。 No. 1的引理 1则证明$\int f(u_\gamma(x)) d\mu(x)$（其中$\mu$表示$G$的左哈尔测度）连续依赖于$\gamma$； 从而命题。

### 5. 哈尔测量乘积

#### 命题 5 {#int-vii-s1-prop-5 .statement tag=09DD}

— *让* $(G_\iota)_{\iota \in I}$ *成为局部紧凑群*的族。 *对于每个* $\iota \in I$ *让* $\mu_\iota$ *成为* $G_\iota$ 上的左（或右）哈尔测度。 *假设存在* $I$ *的有限子集* $J$ *这样，对于每个* $\iota \in I - J$，$G_\iota$ *是紧凑的并且* $\mu_\iota(G_\iota) = 1$。 *然后乘积测量* $\bigotimes_{\iota \in I} \mu_\iota$ *是左（或右）Haar 测量* $G = \prod_{\iota \in I} G_\iota$。 *如果* $x = (x_\iota) \in G$ *那么*
$$
\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota).
$$
对于$I$的每个有限子集$J$，$\bigotimes_{\iota \in J} \mu_\iota$是$\prod_{\iota \in J} G_\iota$上的左（或右）哈尔测度，如下紧接定义。因此 $\bigotimes_{\iota \in I} \mu_\iota$ 是$G$ 的左（或右）Haar 测度（第 III, §4, No. 6 章，第 9 条）。另一方面，如果 $\mu_\iota$ 是左哈尔措施，那么
$$
\delta(x) \left( \bigotimes_{\iota \in I} \mu_\iota \right) = \bigotimes_{\iota \in I} \delta(x_\iota) \mu_\iota = \bigotimes_{\iota \in I} (\Delta_{G_\iota}(x_\iota) \mu_\iota) = \left( \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota) \right) \bigotimes_{\iota \in I} \mu_\iota,
$$
从而$\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota)$。

#### 例 {#int-vii-s1-n5-exa-1 .statement tag=09DE}

— 1) $\mathbf{R}^n$ 的勒贝格测度是加法群 $\mathbf{R}^n$ 的哈尔测度。

2) 映射 $(r, u) \mapsto ru$ 是$\mathbf{R}_+^* \times \mathbf{U}$ 的同构到$\mathbf{C}^*$（GT，VIII, §1, No. 3）。如果通过该同构将$\mathbf{C}^*$与$\mathbf{R}_+^* \times \mathbf{U}$识别，并且如果$du$表示$\mathbf{U}$上的哈尔测度，则$r^{-1} dr du$是No. 2的例2在$\mathbf{C}^*$上的哈尔测度。另一方面，将$[0, 1[$的双射$\theta \mapsto e^{2i\pi \theta}$到$\mathbf{U}$变换，将$[0, 1[$上的勒贝格测度$d\theta$转换为$\mathbf{U}$上No. 2的例3的哈尔测度。由此可见，如果$f \in \mathscr{H}(\mathbf{C}^*)$，则积分
$$
\int_0^{+\infty} \int_0^1 f(re^{2i\pi \theta}) r^{-1} dr\, d\theta
$$
定义 $\mathbf{C}^*$ 的哈尔测度。

### 6. 哈尔测量逆极限*

令 G 为局部紧致群 （因此是完备的）。令$(K_\alpha)_{\alpha \in A}$为G的紧致法线子群的递减有向族，其中交$\{e\}$（以便由$K_\alpha$形成的滤波器基收敛于e）。 集合$G_\alpha = G / K_\alpha$；令$\varphi_\alpha : G \to G_\alpha$和$\varphi_{\beta \alpha} : G_\alpha \to G_\beta \ (\alpha \geq \beta)$为典范同态。那么，逆系$(G_\alpha, \varphi_{\beta \alpha})$中的逆极限可以用G来识别，并且这个逆极限到$G_\alpha$中的典范映射可以用$\varphi_\alpha$来识别（GT，III, §7, No. 3，命题2）。 映射 $\varphi_\alpha$ 和 $\varphi_{\beta \alpha}$ 是正确的（*loc.cit.*，§4, No. 1，第 1 条命题第 2 条）。这些假设在整个小节期间保持固定。

\* 引理 2. — a) *设 $f \in \mathscr{K}_+(G)$，S 是 G 包含的紧子集，补充 $f$，U 是 S 在 G 中的开邻域，以及 $\varepsilon > 0$。 U 之外存在 $\alpha \in A$ 和函数 $g \in \mathscr{K}_+(G)$、零，并且在 $K_\alpha$ 的陪集上存在常数，使得 $|f - g| \leq \varepsilon$。

b) *令 $\mu$ 和 $\mu'$ 为 G 上的两个度量，使得 $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ 对于所有 $\alpha \in A$。然后$\mu = \mu'$。

存在$\alpha_1 \in A$使得$K_{\alpha_1} S \cap K_{\alpha_1}(G - U) = \emptyset$（GT，II, §4, No. 3，命题4）。增S并减U，因此我们可以假设S和U是$K_{\alpha_1}$的陪集的并。考虑 S 上的连续数值函数 $h$ 具有以下性质：存在一个 $\alpha \geq \alpha_1$，使得$h$ 在 $K_\alpha$ 的陪集上是常数。 $\mathscr{K}(S)$的这些函数形式子代数（因为$(K_\alpha)$是递减有向族）包含是S的常量和分隔点：对于，令$x, y$是S的两个不同的点；由于$K_\alpha$的交是$\{e\}$，因此存在$\alpha \geq \alpha_1$使得$\varphi_\alpha(x) \neq \varphi_\alpha(y)$，然后存在在$\varphi_\alpha(S)$上连续的数值函数$u$使得$u(\varphi_\alpha(x)) \neq u(\varphi_\alpha(y))$。根据 Stone–Weierstrass 定理，S 上存在一个 $\alpha \geq \alpha_1$ 和一个连续的函数 $h \geq 0$，在 $K_\alpha$ 的陪集上恒定，使得 S 上有 $|f - h| \leq \frac{\varepsilon}{2}$。对于每个 $t \in \mathbf{R}$、集合 $\delta(t) = \left( t - \frac{\varepsilon}{2} \right)^+$，并且集合$h' = \delta \circ h$。那么 $h'$ 是函数 $\geq 0$，在 S 上连续，在 $K_\alpha$ 陪集上恒定，并且在 S 上$|h - h'| \leq \frac{\varepsilon}{2}$，因此在 S 上$|f - h'| \leq \varepsilon$。另一方面，如果 x 属于到 G 中 S 的边界，则$h'(x) = 0$，因为那么$h(x) \leq \frac{\varepsilon}{2}$。如果$h'$在S的补数上扩展0，则得到满足要求的函数$g$，从而证明a）。

现在令 $\mu, \mu'$ 为 G 上的两个测度，使得 $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ 对于所有 $\alpha \in A$。对于某些$\alpha \in A$，令$v \in \mathscr{K}(G)$为$K_\alpha$陪集上的函数常数，这样我们就可以用$w \in \mathscr{K}(G_\alpha)$来写$v = w \circ \varphi_\alpha$；然后

\* 参见。章。 III, §4, No. 5。

$$
\mu(v) = (\varphi_\alpha(\mu))(w) = (\varphi_\alpha(\mu'))(w) = \mu'(v); \text{ it follows that } \mu = \mu' \text{ by virtue of a)}.
$$

#### 命题 6 {#int-vii-s1-prop-6 .statement tag=09DF}

*对于每个* $\alpha \in A$，*令* $\mu_\alpha$ *成为* $G_\alpha$ 的正测量。 *假设*$\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$*对于*$\alpha \geq \beta$。 *那么，存在且仅有一个积极措施* $\mu$ *在* $G$ *使得* $\varphi_\alpha(\mu) = \mu_\alpha$ *对于所有* $\alpha \in A$。

唯一性紧随引理 2 b)。让我们证明$\mu$的存在性。令$V$为函数属于到$\mathscr{K}(G)$的向量空间，并且在某些$K_\alpha$的陪集上恒定（$\alpha$可能取决于函数）。由引理 2 a) 可知 $V$ 满足第 1 章的条件 (P)。 III, §1, No. 7，第9条：对于所有$x \in K$，让$K$为$G$中的紧集，选择$f \in \mathscr{K}_+(G)$以及$f(x) > 0$；设$a > 0$为$K$上$f$的最小的值；由引理 2 a)，存在函数 $g \in V \cap \mathscr{K}_+(G)$使得$|f - g| \leq a/2$，因此$g(x) > 0$对于所有$x \in K$，且条件(P)得到验证。让$f \in V$。存在一个 $\alpha \in A$ 使得 $f$ 在 $K_\alpha$ 的陪集上是常数。通过商，$f$定义函数$f_\alpha \in \mathscr{K}(G_\alpha)$。 数$\mu(f) = \mu_\alpha(f_\alpha)$不依赖于$\alpha$的选择：例如，令$\beta$为任何指标，使得$f$在$K_\beta$的陪集上是常数；令 $\gamma \in A$ 使得 $\gamma \geq \alpha, \gamma \geq \beta$；那么$f$定义函数$f_\beta \in \mathscr{K}(G_\beta)$，$f_\gamma \in \mathscr{K}(G_\gamma)$使得$f = f_\beta \circ \varphi_\beta = f_\gamma \circ \varphi_\gamma$；然后$f_\alpha \circ \varphi_{\alpha\gamma} = f_\gamma$，因此$\mu_\gamma(f_\gamma) = (\varphi_{\alpha\gamma}(\mu_\gamma))(f_\alpha) = \mu_\alpha(f_\alpha)$，类似地$\mu_\gamma(f_\gamma) = \mu_\beta(f_\beta)$，从而我们的断言。如此成立，显然$\mu$在$V$上是线性形式，而$\mu(f) \geq 0$在$f \geq 0$上。根据第 9 章的提案。 III, §1, No. 7、$\mu$可以扩展到$G$上的积极措施，我们再次用$\mu$表示。一个人拥有所有$\alpha \in A$的$\varphi_\alpha(\mu) = \mu_\alpha$，直到$\mu$的构造。

#### 定义 5 {#int-vii-s1-def-5 .statement tag=09DG}

*测量* $\mu$ *据说是* $\mu_\alpha$ 的逆极限（或射影极限）。

#### 命题 7 {#int-vii-s1-prop-7 .statement tag=09DH}

*我们保留命题6的记号。如果每个* $\mu_\alpha$ *是* $G_\alpha$上的左（或右）Haar测度，*则* $\mu$ *是* $G$上的左（或右）Haar测度。

假设对于例，$\mu_\alpha$ 是左哈尔测度。让$s \in G$。对于每$x \in G$，

$$
(\varphi_\alpha \circ \gamma(s))(x) = \varphi_\alpha(sx) = \varphi_\alpha(s)\varphi_\alpha(x) = (\gamma(\varphi_\alpha(s)) \circ \varphi_\alpha)(x);
$$

因此$\varphi_\alpha(\gamma(s)\mu) = \gamma(\varphi_\alpha(s))\mu_\alpha = \mu_\alpha$。因此$\gamma(s)\mu = \mu$乘以引理2 b)，因此$\mu$是左哈尔测度。

我们假设从此以后$K_\alpha$不仅是紧凑的，而且在$G$中是开放的。那么 $G_\alpha$ 是离散的，对于 $\beta \geq \alpha$，$K_\alpha/K_\beta$ 是紧凑且离散的群，因此是有限的。 群 $G$ 是幺模的（命题 3）。

#### 命题 8 {#int-vii-s1-prop-8 .statement tag=09DI}

a) *让* $\mu$ *和* $\mu'$ *成为* $G$ *的两个正测度，使得对于每个* $\alpha$ *和每个* $C$ *的* $K_\alpha$、$\mu(C) = \mu'(C)$。 *然后*$\mu = \mu'$。

b) *修复* $\alpha_0 \in A$。 *对于每个*$\alpha \geq \alpha_0$*令*$n_\alpha$*为有限群*$K_{\alpha_0}/K_\alpha$元素数。 *存在且仅有一个正测度*$\mu$*在*$G$*上，对于每个*$\alpha \geq \alpha_0$，*每个陪集*$K_\alpha$*都有测度*$n_\alpha^{-1}$。 *此外，$\mu$是*$G$的哈尔测度，*使得*$\mu(K_{\alpha_0}) = 1$。

令 $\mu$ 和 $\mu'$ 为$G$ 满足条件 a) 的两个正测度。离散群 $G_\alpha$ 的点对于$\varphi_\alpha(\mu)$ 和 $\varphi_\alpha(\mu')$、从而 $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ 具有相同的度量，对于所有 $\alpha$ 也是如此。因此 $\mu = \mu'$ (引理 2 b))。

让我们证明b)。对于每个 $\alpha \geq \alpha_0$，令 $\mu_\alpha$ 为离散群 $G_\alpha$ 的 Haar 测度，这样每个点都有测度 $n_\alpha^{-1}$。令$\alpha, \beta$ 使得$\alpha \geq \beta \geq \alpha_0$。那么$K_\beta/K_\alpha$有$n_\alpha/n_\beta$元素。因此$\varphi_{\beta\alpha}(\mu_\alpha)$是$G_\beta$的测度，使得每个点都有测度$n_\alpha^{-1} \cdot \frac{n_\alpha}{n_\beta} = n_\beta^{-1}$；其他字，$\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$。然后应用 Props 就足够了。 6和7。

#### 例 {#int-vii-s1-n6-exa-1 .statement tag=09DJ}

— 令$\mathbf{Q}_p$为$p$-adic 域，$\mathbf{Q}$对于$p$-adic绝对值$|x|_p = p^{-v_p(x)}$的完成（GT，IX, §3, No. 2，*例3*）。 $\mathbf{Q}_p$中的元素称为*$p$*-*adic 数*。我们再次用$|x|_p$表示$p$进绝对值值到$\mathbf{Q}_p$的连续扩张。一个有

$$
|x + y|_p \leq \sup(|x|_p, |y|_p)
$$

对于$\mathbf{Q}$中的$x, y$（*loc.cit.*），因此对于$\mathbf{Q}_p$中的$x, y$；此外，如果$|y|_p < |x|_p$则$|x + y|_p = |x|_p$，因为$|x|_p = |(x + y) - y|_p \leq \sup(|x + y|_p, |y|_p)$。如果$(x_n)$是$\mathbf{Q}_p$的点的序列趋向于$x \in \mathbf{Q}_p^*$，则$|x - x_n|_p < |x|_p$和$|x - x_n|_p < |x_n|_p$为$n$足够大，因此$|x|_p = |x_n|_p$。这证明，对于每个 $x \in \mathbf{Q}_p^*$，$|x|_p$ 是 $p$ 的幂。

设$\mathbf{Z}_p$为$\mathbf{Z}$在$\mathbf{Q}_p$的闭包；这是 $\mathbf{Q}_p$ 中的子环；它的元素称为*$p$*-*adic 整数*。每 $x \in \mathbf{Z}_p$ 就有 $|x|_p \leq 1$。相反，令$x$为$\mathbf{Q}_p$的元素，使得$|x|_p \leq 1$，并让我们证明$x \in \mathbf{Z}_p$；由我们上面看到，存在$\mathbf{Q}$的元素趋于$x$的序列$(x_n)$，以及$|x_n|_p \leq 1$趋向于$n$足够大；足以证明 $x_n$ 属于到 $\mathbf{Z}_p$ 对于 $n$ 足够大；在其他字，我们被简化为$x \in \mathbf{Q}$的情况；那么 $x = a/b$ 与 $b$ 互质于 $p$；对于每个整数$n > 0$，都存在$b'_n \in \mathbf{Z}$和$h_n \in \mathbf{Z}$，使得$bb'_n + h_n p^n = 1$，从而$x = \frac{abb'_n + ah_n p^n}{b} = ab'_n + \frac{ah_n p^n}{b}$和$|x - ab'_n|_p \leq p^{-n}$，因此$ab'_n$趋向于$x$。

由此可见，中心 0、半径 $p^{-n}$ 的闭球，与中心 0、半径 $p^{-n+1}$ 的开球相同，为 $p^n \mathbf{Z}_p$。因此，拓扑空间$\mathbf{Q}_p$是零维的，因此完全断开（GT，IX, §6, No. 4）。

让我们证明整数$0, 1, \ldots, p^n - 1$构成系统，其中$\mathbf{Z}_p$模$p^n \mathbf{Z}_p$。首先，$|k - k'|_p > p^{-n}$对于两个这样的整数、$k$和$k'$，因此类模$p^n \mathbf{Z}_p$这些整数是不同的。另一方面，令 $x \in \mathbf{Z}_p$；存在$k \in \mathbf{Z}$使得$|x - k|_p \leq p^{-n}$；将$p^n$的合适倍数添加到$k$，可以假设$k \in [0, p^n - 1]$和$x$与$k$模$p^n \mathbf{Z}_p$全等。 从而我们的断言。这表明 $\mathbf{Z}_p / p^n \mathbf{Z}_p$ 与 $\mathbf{Z}/p^n \mathbf{Z}$ 是规范同构的。此外，我们还可以看出 $\mathbf{Z}_p$ 是预紧的，因此是“紧”的，因为它是完备的。由于$\mathbf{Z}_p$是$\mathbf{Q}_p$的开子群，$\mathbf{Q}_p$是*局部紧的*。 $\mathbf{Q}_p$ 中的拓扑具有可数基（GT，IX, §2, No. 9，Cor. of Prop. 16）。 加法群$\mathbf{Q}_p$可以与离散的群$\mathbf{Q}_p / p^n \mathbf{Z}_p$中的逆极限识别。

在加法群$\mathbf{Q}_p$上存在且仅有一个哈尔测度$\alpha$使得$\alpha(\mathbf{Z}_p) = 1$；它被称为 $\mathbf{Q}_p$ 上的*标准化 Haar 度量*。由于$\mathbf{Z}_p$是$p^n$不相交的陪集$p^n \mathbf{Z}_p$（$n$整数$\geq 0$）的并，所以有$\alpha(p^n \mathbf{Z}_p) = p^{-n}$；类似地$\alpha(p^{-n} \mathbf{Z}_p) = p^n$，所以最后，对于每个$n \in \mathbf{Z}$，$\alpha(p^n \mathbf{Z}_p) = p^{-n}$。根据命题 8 b)，$\alpha$ *是 * $\mathbf{Q}_p$ *上的唯一正测度，使得 * $p^n \mathbf{Z}_p$ (*n* *整数* $\geq 0$) *的每个陪集都有测度* $p^{-n}$。

$\alpha$到$\mathbf{Z}_p$的限制显然是$\mathbf{Z}_p$的哈尔测度。

### 7. Haar 测度的局部定义

#### 命题 9 {#int-vii-s1-prop-9 .statement tag=09DK}

*设 G 为局部紧致群，V G 的开子集，以及 $\mu$ 非零的 V 上的正测度，具有以下性质：如果 U 是 V 的开子集并且如果 $s \in G$使得$sU \subset V$，那么在U到sU的同胚$x \mapsto sx$下，由$\mu$在U上引起的测度$\mu_U$的像是$\mu_{sU}$。那么，G 上存在且仅剩一个 Haar 测度 $\alpha$，诱导 $\mu$ V。*

对于每个$s \in G$，令$\mu_s$是$\mu$的像，在V的同胚$x \mapsto sx$到sV上。 $\mu_s$至$V \cap sV$的限制是$x \mapsto sx$至$s^{-1}V \cap V$的限制下的$\mu_{s^{-1}V \cap V}$像；到假设，这个像就是$\mu_{V \cap sV}$。 通过翻译，一个结论由此可知，对于任何$s, t$，$\mu_s$和$\mu_t$具有相同的限制到$sV \cap tV$。 因此，根据第 1 章的提案 1。 III, §2, No. 1，G 上存在一个测度 $\alpha$，对于每个 $s$，sV 上有诱导 $\mu_s$。 很明显，$\alpha$ 是 G 上唯一的左 Haar 测度，在 V 上归纳出 $\mu$。

#### 推论{#int-vii-s1-n7-cor-1 .statement tag=09DL}

*设 G，G' 是两个局部紧致群，V（分别为 V'），G 的中性元素（分别为 G'）的开邻域，以及 $\varphi$ G' 的局部同构，其中 G（GT，III, §1, No. 3，Def.2）定义在V'，这样$\varphi(V') = V$。令$\alpha'$为G'上的左哈尔测度，$\alpha'_V$，其限制至$V'$。那么$\varphi(\alpha'_{V'})$是$G$上唯一的左哈尔测度$\alpha$的限制到$V$。

令$V_1$是$e$在$G$中的开邻域，使得$V_1 V_1^{-1} \subset V$。令$\mu$为$\varphi(\alpha'_{V'})$到$V_1$中的限制。令$U$为$V_1$的开子集，并令$s \in G$为$sU \subset V_1$。然后$s \in V_1 V_1^{-1} \subset V$，因此$s = \varphi(s')$对于一些$s' \in V'$。让$x \in U$。然后 $x = \varphi(x')$ 对应一些 $x' \in V'$，因此从 $sx \in sU \subset V$ 开始为 $sx = \varphi(s')\varphi(x') = \varphi(s'x')$。由于$G'$中的左翻译保留了$\alpha'$，我们可以看到第9条命题的$V_1$和$\mu$满足条件。设$\alpha$为$G$的左哈尔测度，归纳出$\mu$ $V_1$。对于每个$t \in V$，在$V_1$中存在$e$的开邻域$W$，使得$tW \subset V$。那么$\varphi(\alpha'_{V'})$到$tW$的限制可以通过从$\mu$到$W$的限制翻译推出，因此是$\alpha$到$tW$的限制。因此，$\varphi(\alpha'_{V'})$是$\alpha$到$V$中的限制。

有人说$\alpha$ *是通过本地同构* $\varphi$从* $\alpha'$ *推导出来的。

#### 例 {#int-vii-s1-n7-exa-1 .statement tag=09DM}

— 在 No. 2、*例 3* 中获得的$T$ 的 Haar 测度可以通过 $R$ 与 $T$ 的局部同构从 $R$ 上的勒贝格测度推导出来。

### 8. 相对不变的措施

#### 命题 10 {#int-vii-s1-prop-10 .statement tag=09DN}

*令$G$为局部紧凑群，$\mu$为$G$与乘子$\chi$的相对左不变测度。如果$\chi_1$是$\mathbf{C}^*$中$G$的连续表示，则测度$\chi_1 \cdot \mu$与乘子$\chi_1 \chi$相对左不变。*

对于，

$$
\gamma(s)(\chi_1 \cdot \mu) = (\gamma(s)\chi_1) \cdot (\gamma(s)\mu) = (\chi_1(s^{-1})\chi_1) \cdot (\chi(s)^{-1}\mu)
= (\chi_1 \chi)(s)^{-1}(\chi_1 \cdot \mu).
$$

#### 推论 1 {#int-vii-s1-prop-10-cor-1 .statement tag=09DO}

*令$\mu$为$G$的左哈尔测度。为了使$G$上的非零的测度$\nu$相对左不变，它是形式$a \chi \cdot \mu$是充分必要的，其中$a \in \mathbf{C}^*$和$\chi$是$\mathbf{C}^*$中$G$的连续表示；那么它的乘子就是$\chi$。*

条件就足够了（提案 10）。另一方面，如果 $\nu$ 是非零的与乘子 $\chi$ 相对左不变测度，则 $\chi^{-1} \cdot \nu$ 是左不变的（命题 10），因此是形式 $a \mu$ 与 $a \in \mathbf{C}^*$ (No. 2，科 1)。

#### 推论 2 {#int-vii-s1-prop-10-cor-2 .statement tag=09DP}

*每个相对左不变的测度都是相对右不变的。*

对于，Cor 的记号。 1、

$$
\delta(s)(\chi \cdot \mu) = (\delta(s)\chi) \cdot (\delta(s)\mu) = (\chi(s)\chi) \cdot (\Delta_G(s)\mu)
= (\chi \Delta_G)(s)(\chi \cdot \mu).
$$

由于科。 2，我们今后将讨论“G 上的*相对不变的测量”，而无需进一步说明。相对不变的测度承认左哈尔测度和右哈尔测度作为特殊情况。给定 G 上相对不变的测度 $\nu$，可以方便地区分其 *左乘子* $\chi$ 和 *右乘子* $\chi'$，由 $\gamma(s)\nu = \chi(s)^{-1}\nu$、$\delta(s)\nu = \chi'(s)\nu$ 定义。通过 (34)，这些乘子满足关系

$$
\chi' = \chi \Delta_G.
$$

仍然用 $\mu$ 表示左哈尔测度，我们有

$$
\nu' = (\chi \cdot \mu)' = \dot{\chi} \cdot \dot{\mu} = (\chi^{-1} \Delta_G^{-1}) \cdot \mu,
$$

因此$\nu'$与左乘子$\chi^{-1} \Delta_G^{-1}$和右乘子$\chi^{-1}$相对不变。

对于每个相对不变的度量，可忽略、局部可忽略、可测量和局部可积函数的概念都是相同的。

### 9. 准不变测度

#### 命题 11 {#int-vii-s1-prop-11 .statement tag=09DQ}

*设 G 为局部紧致群，$\mu$ G 上的左 Haar 测度。要使 G 上的测度 $\nu \neq 0$ 保持拟不变，$\nu$ 等于 $\mu$ 是充分必要的。*

充足性是显而易见的。令$\nu \neq 0$为左准不变测度，并证明$\nu$等价于$\mu$。我们可以将自己限制在$\nu > 0$的情况。设 A 是 G 的紧子集。我们将证明，就像建立命题一样，条件 $\mu(A) = 0$、$\nu(A) = 0$ 是等价的（Ch. V, §5, No. 5、Th. 2）。

a) 对于每个$f \in \mathscr{K}_+(G)$，$G \times G$上的函数$(x, y) \mapsto f(x)\varphi_A(xy)$是$(\nu \otimes \mu)$可积，因为它是上半连续、有界的，并且如果集合$K = \operatorname{Supp} f$为一个，它的支持包含在紧集$K \times K^{-1}A$中。因此，根据 Lebesgue-Fubini 定理，

$$
\int d\nu(y) \int \varphi_A(xy)f(x)\,d\mu(x) = \int f(x)\,d\mu(x) \int \varphi_A(xy)\,d\nu(y).
$$

b) 假设$\nu(A) = 0$。通过假设，$\nu(xA) = 0$ 对于所有 $x \in G$，因此 (36) 的右侧是零。因此，存在一个可忽略的 $\nu$ 集合 $N_f$，对于 $y \notin N_f$，

$$
(37) \quad 0 = \int \varphi_A(xy)f(x)\,d\mu(x) = \Delta_G(y)^{-1} \int \varphi_A(x)f(xy^{-1})\,d\mu(x).
$$

设B是G的紧子集，使得$\nu(B) \neq 0$，并且$\mathscr{K}_+(G)$中的$f$函数等于$AB^{-1}$上的1。则存在 $y \in B$ 使得 (37) 得到验证。但由于$\varphi_A(x)f(xy^{-1}) = \varphi_A(x)$对应$y \in B$，这就证明了$\mu(A) = 0$。

c) 假设$\mu(A) = 0$。那么，对于每个 $f \in \mathscr{K}_+(G)$，(36) 的左侧是零，因此右侧也是。因而，存在局部 $\mu$ 可忽略不计的集合 M，使得 $\int \varphi_A(xy)\,d\nu(y) = 0$ 对于 $x \notin M$。从$\mu \neq 0$开始，对于某些$x \in G$、从而$\nu(A) = 0$，可以得出$\nu(xA) = 0$。

应用命题 11 到 $G^0$，可以看到右侧的准不变测度与左侧的准不变测度相同。它们被简单地称为 G 上的准不变测度。

### 10. 局部紧凑域

#### 定义 6 {#int-vii-s1-def-6 .statement tag=09DR}

— *令 K 为局部紧致域*$^{(1)}$。 *对于 $a \in K^*$，称为 a* 的模，并用 $\mathrm{mod}_K(a)$ 或简称为 $\mathrm{mod}(a)$ 表示，*自同构* $x \mapsto ax$ *加法群* $K^+$ *基础 K 的模；一个集合* $\mathrm{mod}(0) = 0$。

#### 例 {#int-vii-s1-n10-exa-1 .statement tag=09DS}

— 1) 设 $K = \mathbf{R}$。如果$s > 0$则$s \cdot [0,1] = [0,s]$；如果$s < 0$，$s \cdot [0,1] = [s,0]$。因而 $\mathrm{mod}_\mathbf{R} t = |t|$ 对于所有 $t \in \mathbf{R}$。

2）令$K = \mathbf{Q}_p$。如果$s \in \mathbf{Q}_p^*$使得$|s|_p = p^{-n}$，则$s \mathbf{Z}_p$是$x \in \mathbf{Q}_p$的集合使得$|x|_p \leq p^{-n}$；因而，如果 $\mu$ 表示$\mathbf{Q}_p$ 上的归一化 Haar 测度，则$\mu(s \mathbf{Z}_p) = p^{-n}$。因而 $\mathrm{mod}_{\mathbf{Q}_p} t = |t|_p$ 对于所有$t \in \mathbf{Q}_p$。

#### 命题 12 {#int-vii-s1-prop-12 .statement tag=09DT}

— *函数 mod 在 K 上连续，并且* $\mathrm{mod}(ab) = \mathrm{mod}(a)\mathrm{mod}(b)$ *对于所有* $a, b$ *在 K* 中。

最后一个断言是显而易见的。 No. 4的命题4表明函数模在$K^*$的每点连续。它仍然只是显示其在 0 处的连续性。这对于离散 K 来说是显而易见的；因此我们假设 K 非离散。令$\alpha$为$K^+$的哈尔测度，令C为K的紧致子集，使得$\alpha(C) > 0$；对于$a \in K^*$，我们有$\alpha(aC) = \mathrm{mod}(a)\alpha(C)$。

（1）军团（A，I, §9, No. 1），又译为“师环”（GT，III, §6, No. 7）。

由于 K 不是离散的，$\alpha(\{0\}) = 0$（No. 2，命题 2）；因而，对于每个$\varepsilon > 0$，都存在一个为0的开邻域U，使得$\alpha(U) \leq \varepsilon$。由于 K 中的乘积是连续的，因而 $a$ 的 $aC \subset U$ 足够接近 0，然后是 $\mathrm{mod}(a) \leq \varepsilon / \alpha(C)$。

#### 命题 13 {#int-vii-s1-prop-13 .statement tag=09DU}

— *对于每个* $M > 0$，*让* $V_M$ *成为* $x \in K$ *的集合 *这样* $\mathrm{mod}(x) \leq M$。 *如果* K *是非离散的，则* $V_M$ *形式是* K 中* 0 *的紧邻域的基本系统。

根据第 12 条命题，$V_M$ 是 0 的闭邻域。让我们证明它们是紧邻域。设 U 为 0 的紧邻域。K 中存在 $r \neq 0$，使得所有 $n > 0$ 都有 $\mathrm{mod}(r) < 1$ 和 $r^n \in U$：对于，令 W 为 0 的邻域，使得 $WU \subset U$；根据命题 12，K 中存在 $r \neq 0$，使得 $\mathrm{mod}(r) < 1$ 和 $r \in U \cap W$；然后$r^2 \in WU \subset U$，以及$r^n \in U$，对于$n > 0$，在$n$ 上归纳。我们将证明$V_M$包含在集合$r^{-q}U$（$q$整数$\geq 0$）的有限并中，这将证明$V_M$确实是紧致的。如果$x$是序列$(r^n)$的簇点，则$\mathrm{mod}(x)$是序列$(\mathrm{mod}(r)^n)$的簇点，因此$\mathrm{mod}(x) = 0$，$x = 0$；由于 U 是紧致的，因此 (GT, I, §9, No. 1, Cor. of Th. 1) $\lim_{n \to \infty} r^n = 0$。现在让$a \in V_M$。由于序列$(r^n a)_{n \geq 0}$趋于0，因此存在最小的整数$n \geq 0$使得$r^n a \in U$。如果$n > 0$则$r^{n-1} a \notin U$，因此$r^n a \in U \cap C(rU)$； $U \cap C(rU)$ 的闭包 X 是紧致的，因为 U 是紧致的，并且它不是包含 0，因为 $rU$ 是 0 的邻域；因此，在 X 中，$\mathrm{mod}(x)$ 的边界为数 $m > 0$。因此，如果$n > 0$，我们有$m \leq \mathrm{mod}(r^n a)$，从而$\mathrm{mod}(r^{-1})^n \leq M/m$。由于$\mathrm{mod}(r^{-1}) > 1$，整数$n$只能承担值的有限数，数不依赖于$a$，这完成了我们的断言的证明。

正是如此，因为$V_M$约化的交到$\{0\}$$V_M$形式是0邻域的基本系统（GT，I, §9, No. 2，提案1）。

#### 推论{#int-vii-s1-n10-cor-1 .statement tag=09DV}

— *非离散局部紧致域的拓扑承认可数基。*

对于，K 是紧集 $V_1, V_2, \ldots$ 中的并。另一方面，K 可通过 GT 命题 1 IX, §3, No. 1 进行度量。因此，K 的拓扑承认可数基（*loc.cit.*，§2, No. 9，Prop.16 的 Cor.）。

#### 命题 14 {#int-vii-s1-prop-14 .statement tag=09DW}

— *让* $\alpha$ *成为* $K^+$ 上的哈尔测度。 *那么测量* $\beta = (\mathrm{mod}_K)^{-1} \cdot \alpha$ *在* $K^*$ *上是乘法群* $K^*$ 上的左哈尔测量。

例如，如果将 K 的 $b \in K^*$、映射 $a \mapsto b^{-1} a$ 转化为 K 变换 $\alpha$ 转化为 $(\mathrm{mod}_K b) \alpha$，因此 $(\mathrm{mod}_K)^{-1} \cdot \alpha$ 转化为自身，从而命题。

#### 推论{#int-vii-s1-n10-cor-2 .statement tag=09DX}

— *Let* f *be a function defined on* $K^*$, *with values in* $\overline{\mathbf{R}}$ *or in a Banach space. 对于* f *为* $\beta$-*可积，$(\mathrm{mod}_K)^{-1} f$为$\alpha$可积是必要且充分的，在这种情况下

$$
\int_{K^*} f(x) d\beta(x) = \int_{K^+} (\mathrm{mod}_K(x))^{-1} f(x) d\alpha(x).
$$

这是根据 Cor 的第 14 号提案得出的。提案 13 和章节。 V, §5, No. 3，Th。 1.

#### 命题 15 {#int-vii-s1-prop-15 .statement tag=09DY}

— *假设 K 是可交换的。令 u 为向量空间 E = K^n 中的自同构。然后*

$$
\mathrm{mod}_E u = \mathrm{mod}_K(\det u).
$$

当$u$运行超过$\mathbf{GL}(E)$的生成元的系统时，验证公式就足够了。现在，$\mathbf{GL}(E)$由以下元素生成（A，II, §10, No. 13，第14号提案的Cor.2）：
(a) 元素 $u_1$ / 形式

$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$

其中$\sigma \in \mathfrak{S}_n$；
(b) 元素 $u_2$ 形式

$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n)
$$

与 $a \in K^*$；
(c) 元素 $u_3$ / 形式

$$
(x_1, \ldots, x_n) \mapsto (x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n).
$$

如果 $f \in \mathscr{H}(E)$ 那么，用 $\alpha$ 表示$K^+$ 上的 Haar 测度，

$$
\int \cdots \int_{K^n} f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1) d\alpha(x_2) \ldots d\alpha(x_n)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^n} f(x_1, \ldots, x_n) d\alpha(x_1) \ldots d\alpha(x_n),
$$

另一方面，$\mathrm{mod}_K(\det u_3) = \mathrm{mod}_K(1) = 1$、从而是$u_3$的结果。 $u_1$和$u_2$以类似的方式建立。

令 K 为 K 上有限维 n 的可交换局部紧凑域，E 向量空间。如果 $\varphi$ 是向量空间 $K^n$ 的同构到向量空间 E，$\varphi$ 变换拓扑将 $K^n$ 转换为 E 上的拓扑，使 E 成为局部紧凑的向量空间。这个拓扑（称为规范）独立于$\varphi$，因为向量空间$K^n$的每个自同构都是双连续的。如果没有明确指出相反的情况，当我们将 E 称为拓扑向量空间时，拓扑将始终被理解为刚刚定义的那个。 向量空间 E 的每个自同构 u 都是双连续的，因此定义了$\mathrm{mod}_E u$。另一方面，如果 u 是 E 的不可逆自同态，则有一个集合 $\mathrm{mod}_E u = 0$。然后：

#### 推论 1 {#int-vii-s1-prop-15-cor-1 .statement tag=09DZ}

— *令 K 为可交换局部紧域，K 上的 E 有限维向量空间，以及向量空间 E 的 u 自同态。然后* $\mathrm{mod}_E(u) = \mathrm{mod}_K(\det u)$。

如果 u 可逆，则由命题 15 得出。如果 u 不可逆，则 $\det u = 0$，因此 $\mathrm{mod}_K(\det u) = 0 = \mathrm{mod}_E u$。

#### 推论 2 {#int-vii-s1-prop-15-cor-2 .statement tag=09E0}

— *令 E 为有限维 n 的实数向量空间，E 的 $(e_1, e_2, \ldots, e_n)$ 基，* $x = \sum_{i=1}^n \xi_i e_i \in E$ *的 P 集合 *使得* $0 \leq \xi_i \leq 1$ *对于所有 i*，以及 $\mu$ *对加法群 E 的独特哈尔测度使得* $\mu(P) = 1$。 *设*$x_1, \ldots, x_n$*为E的点，S为集合*$\{0, x_1, \ldots, x_n\}$的E中的闭凸包络。 *写作*$x_i = \sum_{j=1}^n \alpha_{ij} e_j$，*一个有*

$$
\mu(S) = \mu(\dot{S}) = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

我们将认同E与$\mathbf{R}^n$通过同构将变换$(e_i)$转化为$\mathbf{R}^n$的典范基。然后$\mu$ 与$\mathbf{R}^n$ 上的勒贝格测度$\mu_n$ 进行识别。

首先假设 $x_i = e_i$ 对于所有 i。那么 S 是 $\mathbf{R}^n$ 中 $x = (\xi_i)$ 的集合 $S_n$ 使得

$$
\xi_i \geq 0 \text{ for all } i \quad \text{and} \quad \xi_1 + \cdots + \xi_n \leq 1.
$$

集合$\mu_n(S_n) = a_n$。让$\lambda \in \mathbf{R}$。将$\mathbf{R}^n$与$\mathbf{R}^{n-1} \times \mathbf{R}$识别，我们可以在$\lambda$处考虑$S_n$的截面$C_\lambda$。如果$\lambda < 0$或$\lambda > 1$，则这个截面为空；如果 $0 \leq \lambda \leq 1$，$C_\lambda$ 是 $(\xi_1, \ldots, \xi_{n-1}) \in \mathbf{R}^{n-1}$ 的集合，使得

$$
\xi_1 \geq 0, \ldots, \xi_{n-1} \geq 0, \quad \xi_1 + \cdots + \xi_{n-1} \leq 1 - \lambda,
$$

因此可以从$S_{n-1}$乘以位似的比率$1 - \lambda$推出，从而得到$\mu_{n-1}(C_\lambda) = (1 - \lambda)^{n-1} a_{n-1}$。由勒贝格-富比尼定理，

$$
a_n = \int_0^1 (1 - \lambda)^{n-1} a_{n-1} d\lambda = \frac{1}{n} a_{n-1}.
$$

从$a_1 = 1$开始，我们就看到了$a_n = \frac{1}{n!}$。

让我们回到推论的一般情况。令 $u$ 为 $\mathbf{R}^n$ 的自同态，使得 $u(e_i) = x_i$ 对于所有 $i$。一个有$u(S_n) = S$。如果 $u$ 可逆，则第 15 条命题证明

$$
\mu_n(S) = \frac{1}{n!} |\det u| = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

由于$S - \overset{\circ}{S}$包含在超平面的有限数中，因此$\mu(\overset{\circ}{S}) = \mu(S)$。最后，如果$u$不可逆，则$S$包含在超平面中，因此$\mu(S) = 0 = \det(\alpha_{ij})$。

### 11. 局部紧致域上的有限维代数

令$K$为交换域，$A$是有限秩与单位元元素的$K$代数。对于每个$a \in A$，令$L_a, R_a$为向量空间$A$的自同态、$x \mapsto ax$、$x \mapsto xa$，并让$N_{A/K}(a) \in K$、$N_{A^0/K}(a) \in K$为$a$的范数 $A$ 和反代数 $A^0$ 中的正则表示；回想一下$N_{A/K}(a) = \det(L_a)$，$N_{A^0/K}(a) = \det(R_a)$（A，III, §9, No. 3）。以下条件是等效的：$a$可逆，$L_a$在$\mathrm{Hom}_K(A, A)$中可逆，$R_a$在$\mathrm{Hom}_K(A, A)$中可逆，$N_{A/K}(a) \neq 0$，$N_{A^0/K}(a) \neq 0$。我们用$A$的可逆元的$A^*$集合来表示。

现在假设域 $K$ 是局部紧凑的，因此代数 $A$ 是局部紧凑的。那么$N_{A/K}$和$N_{A^0/K}$是$A$的映射连续到$K$，因此$A^*$在$A$开。由科. No. 10第15号提案1，

$$
\mathrm{mod}_A L_a = \mathrm{mod}_K N_{A/K}(a), \quad \mathrm{mod}_A R_a = \mathrm{mod}_K N_{A^0/K}(a).
$$

#### 命题 16 {#int-vii-s1-prop-16 .statement tag=09E1}

— *令$\alpha$为加法群对$A$的哈尔测度。措施*

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha(a), \quad (\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha(a)
$$

*在 $A^*$ 上分别是乘法群 $A^*$ 的左、右哈尔测度。*

令$\alpha'$为$\alpha$到开集合$A^*$的限制。对于$a \in A^*$，有$L_a(\alpha') = (\mathrm{mod}_K N_{A/K}(a))^{-1} \alpha'$，因此$(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha'(a)$是$A^*$的左哈尔测度（No. 8，第10号提案的Cor.1）。 经过到反代数，可以看出$(\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha'(a)$是$A^*$的正确哈尔测度。

#### 命题 17 {#int-vii-s1-prop-17 .statement tag=09E2}

— *假设 A 是域（局部紧凑）。对于每个 $a \in A$、$\mathrm{mod}_A(a) = \mathrm{mod}_K N_{A/K}(a)$。*

这是(38)第一个公式的翻译。

#### 例 {#int-vii-s1-n11-exa-1 .statement tag=09E3}

— 1) 取$K = \mathbf{R}$，$A = \mathbf{C}$。考虑到 *Alg.*，第 1 章。 VIII, §12，n° 2，道具。 4、对于所有$z \in \mathbf{C}$，我们得到$\mathrm{mod}_\mathbf{C}(z) = |z|^2$。 (2)

2) 取$K = \mathbf{R}$，对于A来说，*四元数域* $\mathbf{H}$（GT，VIII, §1, No. 4）。考虑以下 $\mathbf{M}_2(\mathbf{C})$ 的元素：

$$
X_1 = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix} \quad X_2 = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \quad X_3 = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}
$$

其中，与$I_2$、$\mathbf{M}_2(\mathbf{C})$中的形式基一起超过$\mathbf{C}$。很容易验证

$$
X_1^2 = X_2^2 = X_3^2 = -I_2, \qquad X_1 X_2 = -X_2 X_1 = X_3,
$$
$$
X_2 X_3 = -X_3 X_2 = X_1, \qquad X_3 X_1 = -X_1 X_3 = X_2.
$$

因此，映射$a + b i + c j + d k \mapsto a I_2 + b X_1 + c X_2 + d X_3$可以扩展到代数$\mathbf{C} \otimes_\mathbf{R} \mathbf{H}$到代数$\mathbf{M}_2(\mathbf{C})$的$\mathbf{C}$同构。由于$[\mathbf{H} : \mathbf{R}] = 4$，$\mathbf{C}$是$\mathbf{H}$的中和域（*Alg.*，第VIII, §10，n° 5），并且$q = a + b i + c j + d k \in \mathbf{H}$的约化范数是

$$
\mathrm{Nrd}(q) = \det(a I_2 + b X_1 + c X_2 + d X_3)
$$
$$
= \det \begin{pmatrix} a + i d & -c + i b \\ c + i b & a - i d \end{pmatrix} = a^2 + b^2 + c^2 + d^2 = \|q\|^2.
$$

作者：*Alg.*，章节。 VIII, §12，n° 3，道具。 8、1个有

$$
\mathrm{N}_{\mathbf{H}/\mathbf{R}}(q) = (\mathrm{Nrd}_{\mathbf{H}/\mathbf{R}}(q))^2 = \|q\|^4.
$$

这表明，第 17 号提案表明

$$
\mathrm{mod}_\mathbf{H}(q) = \|q\|^4.
$$

对局部紧致域的结构将在CA，VI, §9进行更深入的研究。

(2) 这也可从 Cor 中得出。命题 15 的 1 以及左乘 $z = a + i b$ 相对于 $\mathbf{C}$ 的典范基 $1, i$ 与$\mathbf{R}$ 的矩阵 $\begin{pmatrix} a & -b \\ b & a \end{pmatrix}$ 的事实。

### 习题{#int-vii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
