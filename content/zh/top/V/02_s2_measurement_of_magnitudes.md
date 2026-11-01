---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 2
section_title: Measurement of magnitudes
lang: zh
source: top-v-x
pdf_pages: 0018-0023, 0031-0031
extraction: ocr
statements: 5
exercises: 2
content_sha256: 4e46e512bca08ca50bc373bfbe6a88fea8163713933188b80d1cad77d66a99f9
translated_from: content/en/top/V/02_s2_measurement_of_magnitudes.md
translation_method: google
source_content_sha256: 4c0d4a053c85b93dc23047deb4096b5b7869ee2eb4c5bc580d37bfd28b4c40a9
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 14b416132342cb1d6875031f1ba365994cd7a00a15ad325d81fe0118fac3a71d
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. 幅度测量

我们已经看到（cf.历史注记到章IV）问题的震级测量是实数概念的起源；更准确地说，出于实际或理论的目的，逐渐开始研究的各种型的大小首先被彼此分开考虑，并且用相同的数系统测量所有型的可能性已经作为实验事实出现，而之前希腊人则构想了给出严格证明的大胆想法。在他们建立的公理论中，大小的概念与合成的律（相同型的大小的“加法”）和顺序关系（关系“A小于B”，称为大小比较的关系）有关。接下来我们将检查相同的问题，也就是说，我们将研究条件，它必须强加于合成的内部律，以及阶中集合E的顺序关系，它应该与R的子集E'同构的，赋予结构由 R 中的加法和关系 $\leq$ 引出。由于我们不会先验地假设 E 上的合成的给定律是可交换的，因此我们将使用乘法记号；但除此之外，我们几乎不会脱离经典论证。

令E按序关系写成$x \leq y$线性排序集合，并假设E有最小的元素$\omega$。令I为E的子集，使得$\omega \in I$，并且使得关系$x \in I$和$y \leq x$隐含$y \in I$；还假设我们在E上给出了合成$(x, y) \to xy$的律，乘积$xy$被定义为I的元素的所有对（$xy$属于到E，但不一定是I）。此外，我们制作以下假设：

(GR_I) $\omega$ 是单位元素 [$\omega x = x \omega = x$ 对于所有 $x \in I$] 且合成的律是关联的 [在以下意义上：只要 $x \in I, y \in I, z \in I, xy \in I$ 和 $yz \in I$，则$x(yz) = (xy)z$]。

(GR_{II}) 关系$x < y$在元素与I之间意味着，对于所有$z \in I$、关系$xz < yz$和$zx < zy$。

(GR_{III})I中元素$> \omega$的集合不为空且没有最小的元素；并且给定 I 的任何元素 $x, y$ 使得 $x < y$，存在 $z > \omega$ 使得 $xz \leq y$。

条件 (GR_{II}) 意味着元素和 I 之间的不等式可以用项乘以项：$x < y$ 和 $x' < y'$ 意味着 $xx' < yy'$（对于 $xx' < yx'$ 和$yx' < yy'$）。特别是，我们对所有 $x > \omega$ ($x \in I, y \in I$) 都有 $y < yx$。

给定I的元素的有限序列$(x_i)_{1 \leq i \leq p}$，我们可以在这个序列$\prod_{i=1}^p x_i$的$p$乘积上定义乘归纳等于$\left( \prod_{i=1}^{p-1} x_i \right) x_p$，前提是：定义了乘积 $\prod_{i=1}^{p-1} x_i$，并且定义了属于到 I：因此，如果定义了 $\prod_{i=1}^p x_i$，则定义了乘积 $\prod_{i=1}^q x_i$ 以及属于到 I，对于 $2 \leq q \leq p - 1$。通过使所有$x_i$等于相同的元素$x \in I$，我们特别看到，如果定义了$x^p$，则定义了$x^q$，并且对于$2 \leq q \leq p - 1$，属于到I。按照惯例，对于所有 $x \in I$，我们定义 $x^0$ 等于 $\omega$。通过(GR$_\text{II}$)，如果$x > \omega$，如果定义了$x^p$，则对于$1 \leq q \leq p - 1$我们有$\omega < x^q < x^p$；如果定义了$x < y$并且定义了$y^p$，那么我们会看到（通过$p$上的归纳）定义了$x^p$和$x^p < y^p$。另一方面，结合性条件（GR$_\text{I}$）通过$n$上的归纳意味着，如果定义了$x^{m+n}$，那么$x^m x^n$也定义了，$x^{m+n} = x^m x^n$也定义了。相反，根据(GR$_\text{I}$)和(GR$_\text{II}$)，如果$x^m x^n$被定义并且属于到I，那么$x^{m+n}$被定义并且我们有$x^{m+n} = x^m x^n$；这再次由$n$上的归纳证明，因为我们有$x^{n-1} \leq x^n$，因此定义了$x^m x^{n-1}$，并且属于到I；由假设、$x^m x^{n-1} = x^{m+n-1} \in I$，因此 $(x^{m+n-1})x = x^{m+n}$ 被定义为由先前的结果等于 $x^m x^n$。同样，通过归纳对$n$的证明，如果定义了$x^{mn}$，则定义了$(x^m)^n$，并且$x^{mn} = (x^m)^n$；相反，如果定义了 $(x^m)^n$ 且属于到 I，则定义了 $x^{mn}$ 且等于 $(x^m)^n$。

最后，公理 (GR$_\text{III}$) 意味着，对于所有$x \in I$使得$x > \omega$，存在$y > \omega$使得$y^2 \leq x$。因为如果$x > \omega$存在$z > \omega$使得$z < x$，然后存在$t > \omega$使得$zt \leq x$；取 $y$ 为两个元素 $z, t$ 中较小的一个。通过$n$上的归纳，我们推断存在$u > \omega$使得$u^{2^n} \leq x$。

现在就让我们介绍一下以下假设：

(GR$_\text{IV}$)（“阿基米德公理”）。 *对于所有*$x \in I$*和*$y \in I$*使得*$x > \omega$，*存在整数*$n > 0$*使得*$x^n$*被定义并且*$x^n > y$。

如果我们取 E 为实数 $\geq 0$ 的集合，其中包含 0 和任意小数 $> 0$，I 为 E 的交，区间为 R，其左端点为 0，并且包含数、合成的律至少是I 的元素加法，并且如果我们假设只要$x \in I$ 和$y \in I$ 就有$x + y \in E$ 那么很明显满足公理（GR$_\text{I}$）、（GR$_\text{II}$）、（GR$_\text{III}$）和（GR$_\text{IV}$）（*）。

(*) 在实验科学中出现的集合“量级”中，公理（GR$_\text{I}$）和（GR$_\text{II}$）至少大约能够被实验验证。另一方面，公理（GR$_\text{III}$）假设存在“尽可能小的大小”，显然不能以同样的方式成立；它纯粹是*先验*假设。至于公理（GR$_\text{IV}$），它可以被认为是对一个事实的“外推”，该事实可以通过实验验证，其幅度不“太小”。

反之：

#### 命题 1 {#top-v-s2-prop-1 .statement tag=0BVG}

令 E 为线性有序集合且最小的元素 ω；令 I 为 E 的子集，使得 ω ε I 且关系 x ε I，y ≤ x 意味着 y ε I；设 (x, y) → xy 为 E 上合成的律，定义为 x ∈ I 和 y I。那么，如果满足公理(GR_I)、(GR_{II})、(GR_{III})和(GR_{IV})，则存在I的严格递增的映射f到集合R_+ 实数 ≥ 0，使得

$$
f(xy) = f(x) + f(y)
$$

每当 x ε I，y ε I 且 xy ε I；此外，f(I)的交与R的每个区间[0, f(b)]在该区间内都是稠密的，其中b表示I的任意元素。

给定 I 的任意两个元素 x, y 使得 y ≠ ω，让我们用 (x : y) 最大的整数 n ≥ 0 表示，使得 y^n 被定义且 ≤ x (*)；这个整数存在于(GR_{IV})；如果 (x : y) = p，则定义 y^{p+1} 并且 > x。如果 x ε I，y ε I 且 xy ε I，我们有

(I)
$$
(x : z) + (y : z) \leq (xy : z) \leq (x : z) + (y : z) + 1.
$$

对于令 (x:z) = p, (y:z) = q；那么我们有 z^p ≤ x, z^q ≤ y；由于 xy ∈ I，定义了 z^p z^q 且属于至 I，因此定义了 z^{p+q} 且 z^{p+q} = z^p z^q ≤ xy；此外，如果定义了 z^{p+q+2}，则 z^{p+q+2} > xy，因为 z^{p+1} > x 且 z^{q+1} > y。

接下来我们建立不等式

(2)
$$
\begin{cases}
(x : y) (y : z) \leq (x : z), \\
((x : y) + 1) ((y : z) + 1) \geq (x : z) + 1.
\end{cases}
$$

令 (x : y) = p 且 (y : z) = q；则 y^p ≤ x 且 z^q ≤ y，因此定义 (z^q)^p 且 ≤ x；因此属于变为I；因而 z^{pq} 被定义，并且我们有 z^{pq} = (z^q)^p ≤ x，由此得出第一个不等式。另一方面，如果定义了 z^{(p+1)(q+1)}，则有 z^{(p+1)(q+1)} > x，因为 y^{p+1} > x 且 z^{q+1} > y；因此第二个不等式。

设$\tilde{\mathscr{X}}$表示I中元素 > ω的有序集合的截面滤波器，相对于关系≥；区间 ]ω, z[，其中 z 穿过所有元素 > ω 中的集合，形式基中的 $\tilde{\mathscr{X}}$。给定 I 的两个元素 a 和 x，使得 a > ω，我们将证明比率 $\frac{(x : z)}{(a : z)}$，它是为 z ≤ a 定义的，并且是有理数数 > 0，

(*) 当 E = I 为自然整数的集合，合成的律为加法时，(x : y) 为 x/y 的积分部分。

是$z$的函数，相对于$\mathfrak{F}$有*极限*。这是显而易见的，如果$x = \omega$，则$(x : z) = 0$，对于所有$z$。如果$x > \omega$，我们将证明映射$z \to \frac{(x : z)}{(a : z)}$下$\mathfrak{F}$的像$\mathscr{G}$（仅限于$z > \omega$中的集合，即$\leq x$和$\leq a$）是柯西滤波器基为*乘法* 群 $\mathbf{R}_+^*$ 的一致结构，因此收敛到实数 $> 0$。 注首先，给定$u > \omega$，$(u : z)$相对于$\mathfrak{F}$有极限$+\infty$：因为存在$z > \omega$使得$z^{2^n} \leq u$，从而$(u : z) \geq 2^n > n$。现在任意取数$\varepsilon > 0$；存在$t > \omega$使得$(x : t) \geq 1 / \varepsilon$和$(a : t) \geq 1 / \varepsilon$。考虑双不等式

$$
\frac{(x : t)}{(a : t) + 1} \cdot \frac{(t : z)}{(t : z) + 1} \leq \frac{(x : z)}{(a : z)} \leq \frac{(x : t) + 1}{(a : t)} \cdot \frac{(t : z) + 1}{(t : z)},
$$

这直接由不等式 (2) 得出。存在$z_0 > \omega$使得$z \leq z_0$蕴含$(t : z) \geq 1 / \varepsilon$，因此

$$
\frac{1}{(1 + \varepsilon)^2} \frac{(x : t)}{(a : t)} \leq \frac{(x : z)}{(a : z)} \leq (1 + \varepsilon)^2 \frac{(x : t)}{(a : t)},
$$

这表明$\mathscr{G}$是乘法均匀性的柯西滤波器基。

一劳永逸地修复元素$a > \omega$（“测量的单位”）和每个$x \in I$投入

$$
f(x) = \lim_{z \in \mathfrak{F}} \frac{(x : z)}{(a : z)}.
$$

根据已经证明的，对于$x > \omega$我们有$f(\omega) = 0$，$f(x) > 0$，以及$f(a) = 1$。如果我们通过 $(a : z)$ 进行除不等式 (1) 并针对$\mathfrak{F}$传递到极限，我们会看到

$$
f(xy) = f(x) + f(y)
$$

每当$x \in I, y \in I$和$xy \in I$时。同样，关系$x \leq y$意味着$(x : z) \leq (y : z)$，从而除以$(a : z)$和经过到极限，我们得到$f(x) \leq f(y)$，所以$f$是$I$上的*递增*。我们推断$f$在$I$上是*严格递增的*；对于如果$x < y$，则存在$z > \omega$使得$xz \leq y$，从而$f(xz) \leq f(y)$；从$xz \in I$开始，

$$
f(x) + f(z) = f(xz) \leq f(y);
$$

但是$f(z) > 0$，所以确实是$f(x) < f(y)$。

最后，如果$f(I)$的$b \in I$、交以及$\mathbf{R}$的区间$[0, f(b)]$在这个区间是稠密的。因为如果$n$是任何整数$> 0$，则存在$x > \omega$使得$f(x) \leq 2^{-n}$（取$x$使得$x^{2^n} \leq a$）；如果$p$是最小的整数使得$x^{p+1} > b$，我们有$(p+1)f(x) > f(b)$和$qf(x) \leq f(b)$对应$1 \leq q \leq p$；因此$[0, f(b)]$和长度$> 2^{-n}$包含中包含的每个区间至少有形式$qf(x) = f(x^q) \in f(I)$中的一个点。因此，命题 1 中的证明是完整的。

#### 注 1 {#top-v-s2-rem-1 .statement tag=0BVH}

关系 $x \in I, y \in I, xy \in I, yx \in I$ 表示
$$
f(xy) = f(x) + f(y) = f(yx),
$$
因此 $yx = xy$ 因为 $f$ 是严格递增的；在其他字中，律由$E$的合成的律在适当选择的间隔$[0, b]$上（例如，使得$b^2 \leq a$）是*可交换的*。

#### 注 2 {#top-v-s2-rem-2 .statement tag=0BVI}

$I$的每个映射$g$进入$\mathbf{R}_+$，满足与$f$相同的条件，是形式$x \to \lambda f(x)$，其中$\lambda > 0$。因为如果 $\lambda = g(a) > 0$, 关系 $z^p \leq x \leq z^{p+1}, z^q \leq a \leq z^{q+1}$ 意味着假设,
$$
pg(z) \leq g(x) \leq (p+1)g(z), \qquad qg(z) \leq g(a) \leq (q+1)g(z),
$$
从而
$$
\lambda \frac{(x : z)}{(q : z) + 1} \leq g(x) \leq \lambda \frac{(x : z) + 1}{(q : z)},
$$
因此，相对于$\tilde{x}$，经过到极限，我们有$g(x) = \lambda f(x)$。

让我们求条件，其中 $f(I)$ 是 $\mathbf{R}_+$ 的*区间*。显然以下两个条件是必要的：

(GR_{IIIa}) *$I$中元素$> \omega$的集合不为空且没有最小的元素，并且给定$I$中的任意两个元素$x, y$使得$x < y$，有存在$z \in I$使得$xz = y$*（幅度的“减法”）。

(GR_{IVa}) *以$I$的元素为界的$I$的元素的每个递增序列，在$I$*中至少有上界。

我们将证明这些条件也是充分的，而且它们允许我们免除公理（GR_{IV}）（阿基米德公理）。准确地说，我们要证明以下命题：

#### 命题 2 {#top-v-s2-prop-2 .statement tag=0BVJ}

*如果$E$ 满足公理 (GR_I), (GR_{II}), (GR_{IIIa}) 和 (GR_{IVa}) 的线性有序集合 $E$ 和子集 $I$，则存在将$I$的严格递增的映射$f$转移到$\mathbf{R}$区间，以$0$作为其左端点，使得每当$x, y$和$xy$属于时$f(\omega) = 0$和$f(xy) = f(x) + f(y)$到$I$.*

让我们首先证明公理 (GR_{IV}) 是满足的。我们通过矛盾来论证：假设存在$x, y \in I$，使得$x > \omega$、$x^n$被定义，并且$x^n \leq y$对于所有整数$n > 0$。 递增序列 $(x^n)$ 至少有上界 $b \in I$ (GR$_{\text{IV}_a}$)。从$x < b$开始，存在$c \in I$使得$xc = b$乘以(GR$_{\text{III}_a}$)，并且从$x > \omega$开始我们有$c < b$。现在，对于每个$n$，我们有$x^{n+1} \leq b = xc$，从而$x^n \leq c$（GR$_{\text{II}}$）：$x^n$的上界$b$因此是$\leq c$，这是一个矛盾。

因此，我们可以得到应用命题 1。 仍然需要证明，如果 $\gamma = f(c)$ ($c > \omega$) 是 $f(I)$ 中的任意元素，并且如果 $\beta$ 是使得 $0 < \beta < \gamma$ 的任意实数，则存在 $b \in I$ 使得 $f(b) = \beta$ （章IV, § 2, no. 4，命题1）。由于$f(I)$和$[0, \gamma]$的交在$[0, \gamma]$是稠密的，因此存在$I$的元素的递增序列$(x_n)$，使得$f(x_n)$有$\beta$为极限。令$b$为$I$中序列$(x_n)$中最小的上界；我们对所有$n$有$f(b) \geq f(x_n)$，因此$f(b) \geq \beta$；但$f(b) > \beta$是不可能的，否则会存在$y \in I$使得$\beta < f(y) < f(b)$，并且由于$\beta$是序列$(f(x_n))$中最小的上界，所以我们应该对所有$n$，从而有$f(x_n) < f(y) < f(b)$ $x_n < y < b$ 对于所有$n$，这是荒谬的。因此$f(b) = \beta$，命题2因此得证。

#### 注 {#top-v-s2-n0-rem-3 .statement tag=0BVK}

当$I = E$、像$f(I) = f(E)$是$\mathbf{R}_+$的整体时，如果$b > \omega$，那么$b^n$是对所有$n$定义的，因此$n \cdot f(b)$属于到$f(E)$对于所有$n$；这意味着$f(E)$不受上面的限制，因为$f(b) > 0$。

### 习题{#top-v-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
