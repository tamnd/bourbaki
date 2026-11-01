---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 2
section_title: INTEGRALS OVER NON-COMPACT INTERVALS
lang: zh
source: fvr-i-vii
book_pages: 62-68, 84-86
pdf_pages: 0077-0083, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 62
      pdf_page: 77
    - "no": 2
      title: INTEGRALS OF POSITIVE FUNCTIONS OVER A NON-COMPACT INTERVAL
      page: 66
      pdf_page: 81
    - "no": 3
      title: ABSOLUTELY CONVERGENT INTEGRALS
      page: 67
      pdf_page: 82
statements: 9
exercises: 9
content_sha256: eabe6ceeb570d5320d48fdd4356f1127963f480b5fc796133c0373d07bddbc50
translated_from: content/en/fvr/II/02_s2_integrals_over_non_compact_intervals.md
translation_method: google
source_content_sha256: c9b52ed8d14396c752cf882b9999823a887d9dfcc853a8cd546dc7a96f2d2721
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: e5edc26423e87296409ad951c1c6ff73531f365991fad0b1f4869816a6b24ac2
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。非紧区间上的积分

### 1. 非紧区间上的积分的定义

令I为*延长线*$\overline{\mathbf{R}}$中的紧致区间$[a,\ b]$（$a$和$b$可能是无限的）；设$f$是在$[a,\ b[$上定义的函数，将其值取入$\mathbf{R}$的完整规范的空间E中。概括 def。 1 of II, p. 51，我们可以说函数 $g$，定义在$[a,\ b]$上，E中的值，是$f$的*原语*，如果它在$[a,\ b]$上连续（特别是在端点$a$和$b$）并允许在该区间的可数子集的补集的$[a,\ b[$的所有点处导数等于$f(x)$。

我们将自己限制在以下情况：存在$I = [a,\ b]$的点的有限严格递增的序列$(c_i)_{0 \leq i \leq n}$，使得$c_0 = a,\ c_n = b$，并且使得$f$在每个开区间$[c_i,\ c_{i+1}[$上受到“调节”。 虽然不一定在每个开区间包含点 $c_i$ $I$ 内部进行调节；这样的函数将被称为$[a,\ b[$上的“分段调节”。我们注认为$[a,\ b[$上的调节函数是分段调节的（取前面定义中的$n = 1$）。

如果$f$承认一个原语$g$（在上面精确的意义上），并且如果$c$是区间$[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$的点，则通过假设，对于这个区间中的每个$x$，有$g(x) - g(c) = \int_c^x f(t)\,dt$；由于$g$在$I$上连续假设，因此可以看出，当$x$从右侧趋向于$c_i$以及当$x$从左侧趋向于$c_{i+1}$时，$E$中$\int_c^x f(t)\,dt$趋向于极限。相反，假设所有$t$都满足这些条件，并令$g_i$为$f$在区间$[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$上的原语；我们注立即知道函数$g$，定义在$c_i$的集合相对于$I$的补集上，通过条件它等于$0 \leq i \leq n - 1$在$[c_i,\ c_{i+1}[$上的$g_i(x) + \sum_{k=1}^i (g_{k-1}(c_k-) - g_k(c_k+))$，在每个连续$I$中的点与$c_i$不同，并在每个点处承认极限；因此，它可以通过连续性扩展到这些点中的每一个，并且扩展的函数显然是$I$上的$f$的原语。此外，很明显，$f$的所有其他原语都是形式$g + a$（$E$的$a$元素）。

#### 定义 1 {#fvr-ii-s2-def-1 .statement tag=088F}

*有人说向量函数*$f$，*分段调节在一个区间*$[a,\ b[$*of*$\overline{\mathbf{R}}$，*在这个区间上承认一个积分如果*$f$*在*$[a,\ b[$*上承认一个原语；如果* $g$ *是* $f$ *在* $[a,\ b[$* 上的任意一个原语，并且* $x_0$ *和* $x$ *是* $[a,\ b[$* 的任意两个点，*一个调用元素* $g(x) - g(x_0)$ *的积分* $f$ *从* $x_0$ *到* $x$，*1 用* $\int_{x_0}^x f(t)\,dt$ 表示。

这个概念显然与当区间$[x_0,\ x]$包含没有点$c_i$时定义的概念一致。

注位于 def 之前。图 1 表明，对于 $f$ 在 $[a,\ b[$ 上有积分，其限制对于每个区间 $[c_i,\ c_{i+1}[$ 应该允许在该区间上积分是充分必要的。在其他字中，约化对应于$f$ 在*非紧凑*区间 $I \subset \mathbf{R}$ 上进行调节，端点为 $a,\ b$ ($a < b$)，并且其中： 1 数 $a,\ b$ 中的任一者（至少）是无限的； 2 或 $f$ 不受紧凑区间包含至少点 $a,\ b$ 之一的调节（这两个假设并不相互排斥）。为了使$f$在$I$上有积分，当点$(x,\ y)$接近$(a,\ b) \in \overline{\mathbf{R}}^2$同时保持在$I \times I$内时，整的$\int_a^x f(t)\,dt$接近极限是必要且充分的：而这个极限正是$\int_a^b f(t)\,dt$根据定义。 1. 通过滥用语言，人们说积分 $\int_a^b f(t)\,dt$ *收敛*（或 *收敛*），而不是说 $f$ 具有超过 $I$ 的积分，而不是说。

#### 例 {#fvr-ii-s2-n1-exa-1 .statement tag=088G}

i) 整的 $\int_1^{+\infty} dt/t^2$ 收敛并等于 1，对于
$$
\int_1^x \frac{dt}{t^2} = 1 - \frac{1}{x}.
$$

2) 整的$\int_0^1 dt / \sqrt{t}$收敛并且等于2，对于
$$
\int_1^x \frac{dt}{\sqrt{t}} = 2(1 - \sqrt{x}) \quad \text{for} \quad x > 0.
$$

3) 令$(\mathbf{u}_n)_{n \geq 1}$为E的点的无限序列，并令$\mathbf{f}$为由条件在区间$[1, +\infty[$上定义的步长函数：$n \leq x < n+1$的$\mathbf{f}(x) = \mathbf{u}_n$。那么，要使积分 $\int_1^{+\infty} \mathbf{f}(t)\,dt$ 收敛，级数与一般项 $\mathbf{u}_n$ 在 E 中“收敛”是必要且充分的；确实，一个人有
$$
\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p,
$$
所以条件是必要的；反之，若级数与一般项$\mathbf{u}_n$收敛于E，则$\lim_{n \to \infty} \mathbf{u}_n = 0$；现在，如果$n \leq x \leq n+1$，则有$\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p + \mathbf{u}_n(x-n)$。所以当$x$趋于$+\infty$时，这个积分有极限$\sum_{n=1}^{\infty} \mathbf{u}_n$。

直接的，如果分段调节函数$\mathbf{f}$承认超过I的积分，则II的公式（4）到（9），p. 59仍然有效。类似地，II、p. 59扩展的公式(10)按如下方式：假设$\mathbf{f}$和$\mathbf{g}$是$]a,\ b[$上受管制的函数、$\mathbf{f}'$和$\mathbf{g}'$的原语，1表示通过$[\mathbf{f}.\mathbf{g}]|_x^y$的$[\mathbf{f}.\mathbf{g}]|_a^b$极限（如果存在），因为$(x,\ y)$趋于$(a,\ b)$（与$a < x \leq y < b$）；那么，如果（三个）表达式$[\mathbf{f}.\mathbf{g}]|_a^b$、$\int_a^b [\mathbf{f}(t).\mathbf{g}'(t)]\,dt$和$\int_a^b [\mathbf{f}'(t).\mathbf{g}(t)]\,dt$中的两个有意义，那么第三个也有意义，并且II、p. 59的公式(10)有效。

最后，令$f$为实数函数，它在$I = ]a,\ b[$上定义且连续，并且是$]a,\ b[$上受管制的函数$f'$的原语；另一方面，令 $g$ 为开区间 J 包含于 $f(I)$ 上的连续向量函数；如果函数 $g(f(x))f'(x)$ 允许在 I 上积分，并且如果 $f$ 在点 $a$ 和 $b$ 处趋于极限（有限或非有限），则 $g$ 允许从 $f(a+)$ 到$f(b-)$，一个有公式
$$
\int_a^b g(f(t))f'(t)\,dt = \int_{f(a+)}^{f(b-)} g(u)\,du.
$$
事实上，如果$(x,\ y)$趋向于$(a,\ b)$，那么$(f(x),\ f(y))$趋向于$(f(a+),\ f(b-))$假设；只需在$x$和$y$之间应用II、p. 60的公式(12)，并传递到极限即可获得(1)。

给定非紧区间 $I \subset \mathbf{R}$ 上的调节函数 $\mathbf{f}$，端点为 $a$ 和 $b$ ($a < b$)，$\mathbf{f}$ 具有超过I 的积分的条件可以通过以下方式呈现。紧致区间 $J \subset I$ 形式 a *有向集合* $\mathscr{K}(I)$ 相对于关系 $\subset ^1$，如果 $[ \alpha , \beta ]$ 和 $[ \gamma , \delta ]$ 是 $I$ 中包含的两个紧致区间，并且如果有人放入 $\lambda = \min(\alpha, \gamma)$， $\mu = \max(\beta, \delta)$，则区间$[ \lambda , \mu ]$包含在所考虑的两个区间$I$和包含中。对于 $I$ 中包含的每个紧凑区间 $J = [ \alpha , \beta ]$，让我们将

$$
\int_J f(t) \, dt = \int_\alpha^\beta f(t) \, dt;
$$

为了使$f$承认超过$I$的积分，映射$J \mapsto \int_J f(t) \, dt$相对于有向集合$\mathfrak{K}(I)$有极限是必要且充分的；这个极限就是积分$\int_a^b f(t) \, dt$，我们再次用$\int_I f(t) \, dt$表示。

#### 命题 1（柯西积分准则）{#fvr-ii-s2-prop-1 .statement tag=088H}

*令 $f$ 为区间 $I \subset \mathbf{R}$ 上的调节函数，具有端点 $a$ 和 $b$ ($a < b$)。为了使积分$\int_a^b f(t) \, dt$存在，对于每个$\varepsilon > 0$存在一个包含在$I$中的紧致区间$J_0 = [\alpha, \beta]$是必要且充分的，这样对于包含在$I$中并且在公共的中没有内部点和$J_0$的任何紧致区间$K = [x, y]$，有一个$\| \int_K f(t) \, dt \| \leq \varepsilon$.*

事实上，由于$E$是完备的，柯西准则表明，对于积分$\int_I f(t) \, dt$收敛，对于任何$\varepsilon > 0$，存在一个紧致区间$J_0 = [\alpha, \beta]$，并且对于每个紧致区间$J$，使得$J_0 \subset J \subset I$有$\| \int_J f(t) \, dt - \int_{J_0} f(t) \, dt \| \leq \varepsilon$是必要且充分的。 命题源自以下引理：

#### 引理 {#fvr-ii-s2-n1-lem-1 .statement tag=088I}

*设$J_0 = [\alpha, \beta]$为$I$包含的紧区间。在阶中，$\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \| \leq \varepsilon$对于$I$和包含$J'$中包含的每个对紧致区间$J, J'$来说，对于每个紧致区间，$\| \int_K f(t) \, dt \| \leq \varepsilon$是必要的，并且$\| \int_K f(t) \, dt \| \leq \varepsilon / 2$就足够了$K$ 包含在 $I$ 中，且公共的中没有内部点，且$J_0$。*

事实上，如果对于 $J_0 \subset J \subset I$ 和 $J_0 \subset J' \subset I$，有

$$
\left\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \right\| \leq \varepsilon
$$

特别是，对于$x \leq y \leq \alpha$或$\beta \leq x \leq y$（$I$中的$x$和$y$），一个人有$\| \int_x^y f(t) \, dt \| \leq \varepsilon$。相反，如果 $\| \int_K f(t) \, dt \| \leq \varepsilon / 2$ 对于每个紧凑区间 $K \subset I$ 使得 $K \cap J_0 = \emptyset$，并且如果 $J = [x, y]$、$J' = [z, t]$ 是包含在 $I$ 和包含 $J_0$ 中的两个紧凑区间，则有

1 回想一下（*集合理论*，III，p. 144），$I$的子集的集合$\mathfrak{F}$*相对于关系*$\subset$，如果对于任何$X \in \mathfrak{F}$， $Y \in \mathfrak{F}$，存在$Z \in \mathfrak{F}$使得$X \subset Z$和$Y \subset Z$。如果$S(X)$表示由$U \in \mathfrak{F}$形成的$\mathfrak{F}$的子集，使得$U \supset X$，则$\mathfrak{F}$上的过滤器的$S(X)$形式基，称为截面*的*过滤器$\mathfrak{F}$；将$\mathfrak{F}$的映射$f$的极限（如果存在）转换成拓扑空间，相对于$\mathfrak{F}$的截面的滤波器，称为f相对于有向集合的*极限* $\mathfrak{F}$（*cf. Gen.Top.*、I、p. 70 和 *Gen.Top.*、IV、p. 348）。

$$
\left\| \int_J f(t)\,dt - \int_{J'} f(t)\,dt \right\| = \left\| \int_x^z f(t)\,dt + \int_t^y f(t)\,dt \right\| \leq \varepsilon,
$$
自从
$$
x \leq \alpha \leq \beta \leq y \quad \text{and} \quad z \leq \alpha \leq \beta \leq t.
$$

#### 例 {#fvr-ii-s2-n1-exa-2 .statement tag=088J}

如果区间I是*有界*，并且如果$f$在I上有*有界*，那么积分$\int_I f(t)\,dt$总是存在，对于值定理来说，对于$y \leq \alpha \leq \beta \leq z$，
$$
\left\| \int_y^\alpha f(t)\,dt \right\| \leq (\alpha - a) \sup_{t \in I} \|f(v)\| , \quad \left\| \int_\beta^z f(t)\,dt \right\| \leq (b - \beta) \sup_{t \in I} \|f(x)\|
$$
只要$\alpha - a$和$b - \beta$足够小就可以满足柯西准则。

人们可能注，在这种情况下，I上的$f$原语不一定在I的左端点（或右端点）处具有右（或左）导数（当此数有限时），这与I是紧致的且$f$的情况相反受I监管（*cf.* II、p. 33，执行 1）。

### 2. 非紧区间上的正函数积分

#### 命题 2 {#fvr-ii-s2-prop-2 .statement tag=088K}

*令 $f$ 为区间 $I \subset \mathbf{R}$ 上的实数调节函数 $\geq 0$，端点为 $a$ 和 $b$ ($a < b$)。为了使积分 $\int_a^b f(t)\,dt$ 存在，当 J 穿过 I 中包含的紧区间集合时，数 $\int_J f(t)\,dt$ 的集合在上面有界是必要且充分的；那么积分 $\int_a^b f(t)\,dt$ 就是 $\int_J f(t)\,dt$ 的集合中最小的上界。*

事实上，由于$f \geq 0$，关系$J \subset J'$意味着
$$
\int_J f\,dt \leq \int_{J'} f\,dt;
$$
因此，映射$J \mapsto \int_J f\,dt$是递增，命题源自单调极限定理（*Gen.Top.*，IV，p. 349，第2个）。

当映射$J \mapsto \int_J f(t)\,dt$无界时，相对于有向集合$\mathscr{K}(I)$有极限$+\infty$；然后有人滥用语言说积分$\int_a^b f(t)\,dt$等于$+\infty$。在n 1 扩展（当处理函数$\geq 0$时）中建立的积分的性质，适用于某些相关积分是无限的情况，前提是它们所在的关系有意义。

**命题 3（比较原理）。** *让$f$和$g$是间隔$I \subset \mathbf{R}$上的两个实调节函数，使得$0 \leq f(x) \leq g(x)$在每个点，其中$f$和$g$是连续的（*cf.* II、p. 61，第 6 条）。如果$g$右$I$的积分收敛，$f$的积分也收敛，并且有$\int_I f(t)\,dt \leq \int_I g(t)\,dt$。此外，在$I$的每点处，两个积分不能等于除非$f(x) = g(x)$，其中$f$和$g$是连续的。*

现在对于每个紧凑区间 $J \subset I$ 都有

$$
\int_J f(t)\,dt \leq \int_J g(t)\,dt;
$$

由于$\int_J g(t)\,dt \leq \int_I g(t)\,dt$，整的$\int_J f\,dt$有界于上，因此积分$\int_I f(t)\,dt$收敛；此外，在经过到极限，一个人有$\int_I f(t)\,dt \leq \int_I g(t)\,dt$。进一步假设$f(x) < g(x)$在点$x \in I$处$f$和$g$连续；存在 $I$ 中包含的紧凑区间 $[c,\ d]$，不会减少到（单个）点，并且使得 $x \in [c,\ d]$；一个有$\int_c^d f(t)\,dt < \int_c^d g(t)\,dt$（II，p. 61，cor.1），而另一方面，由于从上面的$\int_a^c f(t)\,dt \leq \int_a^c g(t)\,dt$和$\int_d^b f(t)\,dt \leq \int_d^b g(t)\,dt$，我们可以看到，在逐项添加时，$\int_a^b f(t)\,dt < \int_a^b g(t)\,dt$。

这个命题提供了最常用的方法来判断函数$f \geq 0$的积分是否收敛：即，将$f$与一个更简单的函数$g \geq 0$进行比较，其积分已经知道是否收敛；我们将在第二章中看到。在最常见的情况下，V如何搜索比较器函数；我们将每天推导判据积分和级数的收敛性。

### 3. 绝对收敛积分

#### 定义 2 {#fvr-ii-s2-def-2 .statement tag=088L}

*有人说，如果正数函数 $\| \mathbf{f}(x) \|$ 的积分收敛，则规定的函数 $\mathbf{f}$ 在区间 $I \subset \mathbf{R}$ 上的积分绝对收敛。*

#### 命题 4 {#fvr-ii-s2-prop-4 .statement tag=088M}

*如果$\mathbf{f}$在$I$上的积分绝对收敛，则它是收敛的，并且有*

$$
\left| \int_I \mathbf{f}(t)\,dt \right| \leq \int_I \| \mathbf{f}(t) \| \,dt.\tag{2}
$$

事实上，对于每个紧凑区间 $J \subset I$ 都有 (II, p. 61, 公式 (16))

$$
\left| \int_J \mathbf{f}(t)\,dt \right| \leq \int_J \| \mathbf{f}(t) \| \,dt.\tag{3}
$$

如果正函数 $\| \mathbf{f}(x) \|$ 的积分是收敛的，则对于每个 $\varepsilon > 0$，都存在一个包含在 $I$ 中的紧致区间 $[\alpha,\ \beta]$，这样，对于包含在 $I$ 中且在公共的中没有内部点的每个紧致区间 $[\lambda,\ \gamma]$， $[\alpha,\ \beta]$，一个有$\int_{\lambda}^{\gamma} \| \mathbf{f}(t) \, dt \| \leq \varepsilon$（II，p. 65，道具1）；推论出$\left| \int_{\lambda}^{\gamma} \mathbf{f}(t)\,dt \right| \leq \varepsilon$，这表明$I$上的积分收敛（II，p. 16，命题1）； (3) 中的经过到极限推出不等式 (2)。

#### 推论{#fvr-ii-s2-n3-cor-1 .statement tag=088N}

*令$E, F, G$是$\mathbf{R}$上的三个完整范数空间，$(x, y) \mapsto x.y$是从$E \times F$到$G$的连续双线性映射。令$\mathbf{f}, \mathbf{g}$为$I$上的两个调节函数，值分别位于$E$和$F$。如果 $\mathbf{f}$ 有界于 $I$ 并且 g* 的积分在 I 上绝对收敛，则 [f, g] 的积分绝对收敛。

事实上，存在数 h > 0，使得 $\| [x.y] \| \leq h \| x \| . \| y \|$ 相同（Gen. Top., IX, p. 173, th. 1）；如果有人放入$k = \sup_{x \in I} \| f(x) \|$，那么有人在I上有$\| [f(x).g(x)] \| \leq h k \| g(x) \|$；比较原理现在表明 [f.g] 的积分绝对收敛，并且根据 (2)，

$$
\left\| \int_I [f(t).g(t)] \, dt \right\| \leq h k \int_I \| g(t) \| \, dt.
$$

#### 注 {#fvr-ii-s2-n3-rem-1 .statement tag=088O}

积分可以收敛，但不绝对收敛；这就是II、p. 64的例 3 所示，其中级数与一般项$u_n$收敛，但不是绝对收敛。

### 习题 {#fvr-ii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
