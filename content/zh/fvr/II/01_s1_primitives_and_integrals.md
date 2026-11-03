---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 1
section_title: PRIMITIVES AND INTEGRALS
lang: zh
source: fvr-i-vii
book_pages: 51-62, 79-84
pdf_pages: 0066-0077, 0094-0099
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIMITIVES
      page: 51
      pdf_page: 66
    - "no": 2
      title: EXISTENCE OF PRIMITIVES
      page: 52
      pdf_page: 67
    - "no": 3
      title: REGULATED FUNCTIONS
      page: 53
      pdf_page: 68
    - "no": 4
      title: INTEGRALS
      page: 56
      pdf_page: 71
    - "no": 5
      title: PROPERTIES OF INTEGRALS
      page: 59
      pdf_page: 74
    - "no": 6
      title: INTEGRAL FORMULA FOR THE REMAINDER IN TAYLOR'S FORMULA; PRIMITIVES OF HIGHER ORDER
      page: 62
      pdf_page: 77
statements: 28
exercises: 23
content_sha256: 3299e242573c59c7dac3e3221195850d84beeb59b44aa364b37f3044a62a89ab
translated_from: content/en/fvr/II/01_s1_primitives_and_integrals.md
translation_method: google
source_content_sha256: 966025e49c722d33da4fca08c6c4f13c4514b7e1ed5ae715959b710f37572bbe
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: df2ac5c966b3c5d138b76ee7f20cae8d25b964fd774a5f3b0500aa86acbaa75a
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。原语和积分

与此相反，除非明确提到，在这个章中，我们将仅考虑实变量的向量函数，该实变量将其值置于$\mathbf{R}$上的完全规范的空间中。当我们特别处理实值函数时，我们总是会理解这些函数是有限的除非，相反。

### 1. 定义原语

向量函数$f$定义在区间$I \subset \mathbf{R}$不能是向量函数$g$的这个区间在每个点的导数（定义并连续于$I$)除非满足相当严格的条件：例如，如果$f$在$I$内部的点$x_0$处承认右极限和左极限，则$f$必须连续点 $x_0$，如下所示。 6 个I、p. 18；由此可见，如果对$I$取区间$[ -1 , 1 ]$，对于$f$，实数函数等于$[ -1 , 0[$上的$-1$，以及$[0 , 1]$上的$+1$，则$f$不是$I$ 上任意连续的函数；尽管如此，函数$|x|$在每个点$\neq 0$都有$f(x)$作为其导数；因此，人们会做出以下定义：

#### 定义 1 {#fvr-ii-s1-def-1 .statement tag=0870}

*给定在区间 $I \subset \mathbf{R}$ 上定义的向量函数 $f$，我们说在 $I$ 上定义的函数 $g$ 是 $f$ 的原语，如果 $g$ 是连续的$I$ 并且在$I$的可数子集的补码（相对于$I$）的每个点$x$处具有等于$f(x)$的导数。*

如果$g$在$I$的每个点$x$处也承认等于$f(x)$的导数，则可以说$g$是$f$的严格原语。

通过这个定义，我们可以看到上面考虑的真实函数$f$承认一个等于$|x|$的原语。

很明显，如果$f$承认$I$上的原语，那么$f$的每个原语也是每个等于$f$的函数的原语，除了$I$的可数子集的点。通过滥用语言，人们谈论函数$f_0$上的$I$上的原语仅定义在$I$的可数子集的补码上（相对于$I$）：这将是定义在上的每个函数$f$的原语$I$ 且等于点处的 $f_0$，其中定义了 $f_0$。

#### 命题 1 {#fvr-ii-s1-prop-1 .statement tag=0871}

*设$f$为$I$上定义的向量函数，值定义于$E$；如果$f$在$I$上承认原语$g$，则$I$上$f$原语的集合与函数$g + a$的集合相同，其中$a$是常数函数，其值 $E$。*

事实上，很明显，对于任何 $a \in E$，$g + a$ 都是 $f$ 的原语；另一方面，如果$g_1$是$f$的原语，则$g_1 - g$允许除$I$的可数子集的点之外的导数等于0，因此是常数（I，p. 17，推论）。

有人说函数 $f$（当它们存在时）的原语被定义为“直到一个附加常数”。对于定义 $f$ 的原语，明确地将其分配给点 $x_0 \in I$（任意）值就足够了；特别地，存在且仅有一个 $f$ 的原语 $g$ 使得 $g(x_0) = 0$；对于 $f$ 的每个原语 $h$ 都有 $g(x) = h(x) - h(x_0)$。

### 2. 原语的存在

设 $f$ 为函数，定义在任意区间 $I \subset \mathbf{R}$ 上；对于在$I$上定义的函数$g$作为$f$的原语，$g$的限制对于每个紧凑区间$J \subset I$是$f$的限制的原语是充分必要的$J$。

#### 定理 1 {#fvr-ii-s1-thm-1 .statement tag=0872}

*让$A$是集合通过过滤器$\mathfrak{F}$过滤，并且$(f_\alpha)_{\alpha \in A}$是向量函数的族，其中值在空间$E$超过$\mathbf{R}$，定义于区间$I \subset \mathbf{R}$：对于每个$\alpha \in A$，让$g_\alpha$作为$f_\alpha$的原语。我们假设：
1. 对于滤波器$\mathfrak{F}$函数$f_\alpha$均匀收敛于$I$到函数$f$的每个紧凑子集；
2.存在点$a \in I$，使得对于过滤器$\mathfrak{F}$，族$(g_\alpha(a))$在$E$中具有极限。
在这些假设下，函数$g_\alpha$（相对于$\mathfrak{F}$）在$I$的每个紧凑子集上一致收敛到$f$的原始$g$。*

在小节开头的注，我们可以将自己限制在$I$是*紧凑*区间的情况。

首先让我们证明$g_\alpha$在$I$上一致收敛到连续的函数$g$。到假设，对于每一个$\varepsilon > 0$，都有集合$M \in \mathfrak{F}$，这样，对于任何两个指标$\alpha, \beta$属于到$M$，每个$x \in I$都有$\|f_\alpha(x) - f_\beta(x)\| \leq \varepsilon$；在推论中，有一个 (I, p. 15, th. 2)

$$
\|g_\alpha(x) - g_\beta(x) - (g_\alpha(a) - g_\beta(a))\| \leq \varepsilon |x - a| \leq \varepsilon l
$$

其中$l$表示$I$的长度；由于假设$g_\alpha(a)$相对于$\mathfrak{F}$接近极限，根据柯西准则可以得出$g_\alpha$一致收敛于$I$。还需要证明 $g_\alpha$ 的极限 $g$ 是 $f$ 的原语。

对于每个整数$n > 0$，令$\alpha_n$为指标，使得$\|f(x) - f_{\alpha_n}(x)\| \leq 1/n$在$I$上；很明显，序列 $(f_{\alpha_n})$ 一致收敛到 $f$，序列 $(g_{\alpha_n})$ 一致收敛到 $I$ 上的 $g$。令$H_n$为$I$的可数子集，其中$f_{\alpha_n}$不是$g_{\alpha_n}$的导数，并令$H$为$H_n$的并，因此它是I的可数子集；我们将看到，在每个点$x \in I$而不是属于到H函数，g的导数等于$f(x)$。事实上，如上所示，对于每一个$m \geq n$和每一个$y \in I$，都有一个

$$
\| g_{\alpha_m}(y) - g_{\alpha_m}(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|.
$$

让$m$无限增加也有

$$
\| g(y) - g(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|
$$

每$y \in I$；现在，存在一个 $h > 0$，这样，对于 $|y - x| \leq h$ 和 $y \in I$，就有 $\| g_\alpha(y) - g_{\alpha_n}(x) - f_{\alpha_n}(x)(y - x) \| \leq |y - x| / n$；另一方面，因为我们有 $\| f(x) - f_{\alpha_n}(x) \| \leq 1 / n$，所以我们最终得到

$$
\| g(y) - g(x) - f(x)(y - x) \| \leq \frac{4}{n} |y - x|
$$

对于 $y \in I$ 和 $|y - x| \leq h$，可完成证明。

#### 推论 1 {#fvr-ii-s1-thm-1-cor-1 .statement tag=0873}

* 映射的集合$\mathscr{H}$从I进入E，其中承认区间I上的原语是完整向量空间$\mathscr{F}_c(I; E)$的封闭（因此完整）向量子空间映射从I进入E，赋予I*的每个紧凑子集均匀收敛的拓扑（*Gen.Top.*，X，p. 277）。

#### 推论 2 {#fvr-ii-s1-thm-1-cor-2 .statement tag=0874}

*令$x_0$为I的点，对于每个函数$f \in \mathscr{H}$，令$P(f)$为$f$的原语，在点$x_0$处消失； $\mathscr{H}$到$\mathscr{F}_c(I; E)$的映射$f \mapsto P(f)$是连续的线性映射。*

科。 1 至 th。 1 允许我们通过以下过程确定函数某些类别的原语的存在：如果知道 $\mathscr{F}_c(I; E)$ 的函数属于到子集 $\mathscr{A}$ 承认一个原语，那么函数属于到$\mathscr{F}_c(I; E)$ 中的*闭包* 向量子空间由 $\mathscr{A}$ 生成。我们将在接下来的小节中应用这个方法。

### 3. 受监管函数

#### 定义 2 {#fvr-ii-s1-def-2 .statement tag=0875}

*有人说，如果I的划分进入区间$J_k$的有限数，则区间$I \subset \mathbf{R}$的映射$f$进入集合E是一个步骤函数，使得$f$ 在每个 $J_k$ 上都是恒定的。*

令$(a_i)_{0 \leq i \leq n}$为由$J_k$的不同端点形成的严格递增序列；因为 $J_k$ 是成对不相交的，所以它们要么简化为单个 $a_i$，要么是以两个连续点 $a_i, a_{i+1}$ 作为端点的区间；此外，由于I是$J_k$的并集，因此点$a_0$是I的左端点，$a_n$是右端点。 Every step function on I can thus be characterised as a function which is constant on each of the open intervals ]$a_i,\ a_{i+1}[\ (0 \leq i \leq n - 1)$, where $(a_i)_{0 \leq i \leq n}$ is a strictly increasing sequence of points of $I$ with $a_0$ being the left-hand endpoint and $a_n$ the right-hand endpoint of $I$.

#### 命题 2 {#fvr-ii-s1-prop-2 .statement tag=0876}

*在$I$上定义的步骤函数的集合，其中向量空间$E$中的值超过$\mathbf{R}$，是向量空间$\mathscr{F}(I; E)$的向量子空间$\mathscr{E}$将$I$中的映射转化为$E$。*

事实上，让$f$和$g$是两步函数，并且$(A_i)$和$(B_j)$将$I$的两个划分转化为区间的有限数，使得$f$（分别为$g$）是常数在每个$A_i$（或$B_j$）上；无论实数$\lambda, \mu$，很明显$\lambda f + \mu g$对于非空区间$A_i \cap B_j$都是恒定的，并且$I$的这些区间形式划分。

#### 推论 {#fvr-ii-s1-n3-cor-1 .statement tag=0877}

*向量子空间 $\mathscr{E}$ 由特征函数或区间生成。*

现在让我们考虑$E$是$\mathbf{R}$上的赋范空间的情况；然后，端点为$a, b$（$a < b$）的区间$J$的特征函数立即承认一个原语，即对于$x \leq a$等于$a$，对于$a \leq x \leq b$等于$x$，对于$x \geq b$等于$b$的函数。 科。支撑。因此，图 2 表明*$E$ 中的函数和值的每一步都承认一个原语*。

我们现在可以在 n' 2 中应用方法集合。

#### 定义 3 {#fvr-ii-s1-def-3 .statement tag=0878}

*One says that a vector function, defined on an interval $I$, with values in a complete normed space $E$ over $\mathbf{R}$, is a regulated function, if it is the uniform limit of step functions on every compact subset of $I$.*

其它字中，规定的函数为步骤函数的子空间$\mathscr{E}$中$\mathscr{F}_c(I; E)$闭包的元素； $\overline{\mathscr{E}}$是$\mathscr{F}_c(I; E)$的向量子空间，并且由于$\mathscr{F}_c(I; E)$是完整的，所以$\overline{\mathscr{E}}$也是完整的；在其他字中，如果函数是在$I$的每个紧凑型子集上调节函数的统一极限，则在$I$上进行调节。为了对区间$I$进行监管$f$，其限制对$I$中包含的每个契约区间进行监管是必要且充分的。

科。 I至II、p. 53显示：

#### 定理 2 {#fvr-ii-s1-thm-2 .statement tag=0879}

*区间$I$上的每个受管制的函数都承认$I$上的原语。*

我们将变换def。 II、p. 4 至另一个中的 3 个等效项：

#### 定理 3 {#fvr-ii-s1-thm-3 .statement tag=087A}

*对于定义在区间$I$上的向量函数$f$，值在空间$E$超过$\mathbf{R}$的完整规范中，要被规范，它有一个右极限和一个左极限是必要和充分的当点属于到$I$时，$I$的每个内部点有极限，$I$的左端点有右极限，$I$的右端点有左极限。因此，$I$中$f$的不连续性的点的集合是可数的。*

由于每个区间都是紧致区间的可数并，因此可以将自己限制为第证明。 3 当I紧致时，称I = [a, b]。

1 条件是必要的。假设 f 受到调节，并且令 x 与 b 不同，为 I 的点。通过假设，对于每个 ε > 0，都有一个步骤函数 g，使得 \|f(z) - g(z)\| \leq \varepsilon 对于每个 z \in I；因为 g 在点 x 处有一个右极限，所以存在一个 y，使得 x < y \leq b 并且对于点 z, z' 中的每个对，区间]x, y] 都有 \|g(z) - g(z')\| \leq \varepsilon，并且在推论 \|f(z) - f(z')\| 中\leq 3\varepsilon;这证明（根据柯西准则）f 在点 x 处有右极限。以同样的方式证明f在I的每点处都有一个与a不同的左极限。

2° 条件就足够了。 假设它满足了；对于 I 中的每个 x \in ，都有一个开路区间 V_x = ]c_x, d_x[ 包含于 x ，因此在 I 的交上，每个开路区间 ]c_x, x[, ]x, d_x[ （当交不为空时）振荡f 的值为 \leq \varepsilon。 由于 I 是紧致的，因此 I 中存在点 x_i 的有限数，使得 V_{x_i} 形式覆盖 I；设 (a_k)_{0 \leq k \leq n} 为序列，是由点 a、b 和点 x_i、c_{x_i} 和点 x_i、c_{x_i} 构成的有限集合的递增阶点排列而成d_{x_i} 其中属于到 I； 区间 ]a_k, a_{k+1}[ (0 \leq k \leq n - 1) 中的每一个包含在区间 ]c_{x_i}, x_i[ 或 ]x_i, d_{x_i}[ 中，则 f 的振荡为 \leq \varepsilon；设 c_k 为 ]a_k, a_{k+1}[ 上 f 的值之一；将 g(a_k) = f(a_k) 表示为 0 \leq k \leq n，将 g(x) = c_k 表示为所有 x \in ]a_k, a_{k+1}[ (0 \leq k \leq n - 1)，一个定义步长函数 g 使得 \|f(z) - g(z)\| \leq \varepsilon 于 I；所以f受I调节。

最后，让我们证明，如果f在I上调节，那么它的不连续性点的集合是可数的。对于每个 n > 0，都存在一个步骤函数 g_n 使得 \|f(x) - g_n(x)\| \leq 1/n 于 I；由于序列 (g_n) 在 I 上均匀收敛于 f，我们看到 f 在每个点都是连续的，其中 g_n 都是连续的（Gen. Top.、X、p. 281、cor. 1）；但由于 g_n 除了在有限集合 H_n 的点处是连续的，因此 f 在集合 H = \bigcup_{n} H_n 的补集的点处是连续的，这是可数的。

#### 推论 1 {#fvr-ii-s1-thm-3-cor-1 .statement tag=087B}

令 f 为 I 上的调节函数；在I的每个点处，除了I的右侧端点（或左侧端点）之外，f的每个基元都有等于f(x+)的右导数（或等于f(x-)的左导数）；特别是，在每个点 x 处，其中 f 是连续的，f(x) 是其基元之一的导数。

这是第直接的推论。 3 个 II、p. 54 和 prop。 I、p. 18 中的 6 个。

#### 推论 2 {#fvr-ii-s1-thm-3-cor-2 .statement tag=087C}

令 f_i (1 \leq i \leq n) 在区间 I 上受到 n 调节函数，每个 f_i 的值位于 \mathbf{R} (1 \leq i \leq n) 上完整规范的空间 E_i 中。如果 g 是子空间 \prod_{i=1}^{n} \overline{f_i(I)} of \prod_{i=1}^{n} E_i 的连续映射到 \mathbf{R} 上的完整范数空间 F，则复合函数 x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x)) 在 I 上调节。

事实上，它显然满足 th 的条件。 II、p. 54 中的 3 个。

因此，我们可以看出，如果 f 是 I 上的调节向量函数，则真实的函数 x \mapsto \|f(x)\|也受到监管。 进一步，对I形式环实际调节函数；

此外，如果$f$和$g$是两个实数受调节的函数，则$\sup(f, g)$和$\inf(f, g)$受到调节。

#### 注 1 {#fvr-ii-s1-n3-rem-1 .statement tag=087D}

如果$f$是$I$上的实规函数，$g$是区间包含$f(I)$上的实规向量函数，则复合函数$g \circ f$不一定是规管的（$cf.$II，p. 79，练习 4）。

th 的两个特殊案例。 II、p. 54 中的 3 个尤其重要：

#### 命题 3 {#fvr-ii-s1-prop-3 .statement tag=087E}

*区间$I \subset \mathbf{R}$上的每个连续向量函数在$\mathbf{R}$上的完全规范空间$E$中取其值受到调节，并且在$I$上承认一个原语，它是其在每个点处的导数。*

#### 注 2 {#fvr-ii-s1-n3-rem-2 .statement tag=087F}

为了证明连续的函数承认一个原语，我们可以使用这样一个事实：实数变量的每个 *多项式函数*（$E$ 中的系数）承认一个原语；因为从 Weierstrass 的定理 (*Gen. Top.*, X, p. 313, 命题 3) 开始，每个连续函数都是每个紧凑区间上多项式的一致极限，第 3 个。 1 of II, p. 52 表明每个连续的函数都承认一个原语。

#### 注 3 {#fvr-ii-s1-n3-rem-3 .statement tag=087G}

前面的评论的原理无需重大修改即可扩展到在 $\mathbf{C}$ 的完全赋范空间中取值的*复*变量的向量函数。 如果$U$是$\mathbf{C}$中的开集合，同胚于$\mathbf{C}$，则在$U$上定义的向量函数$f$的*原语*是由定义上的连续函数定义$U$，在$U$的每点处具有等于$f$的导数。 有了这个定义，th。 II、p. 52 扩展未经修改（利用$U$的连通性证明$(g_\alpha)$相对于$\mathscr{F}$一致收敛于$U$的每个点的邻域，由此得出$(g_\alpha)$在$U$的每个紧凑子集上一致收敛于$\mathscr{F}$；证明使用I、p. 18的道具4完成。 因而，每个函数是$U$的每个紧凑子集上的*一致的多项式极限*，在$U$上承认一个原语；这些函数正是函数，称为$U$上的“全纯”，我们将在后面的书中进一步详细研究。

#### 命题 4 {#fvr-ii-s1-prop-4 .statement tag=087H}

*区间 $I \subset \mathbf{R}$ 上的每个单调实数函数 $f$ 都是受管制的，$f$ 的每个本原在 $I$ 上都是凸的。*

事实上，$f$满足th的标准。 *Gen.3顶部。*，IV，p. 350，道具。 4； 命题的第二个部分来自 cor。 1，来自 II，p. 55，以及来自 prop。 I、p. 27 中的 5 个。

#### 注 4 {#fvr-ii-s1-n3-rem-4 .statement tag=087I}

人们一定不要认为区间$I$上受管制的函数是唯一在$I$上具有原语的函数（$cf.$II、p. 80、习题7和8）。

### 4. 整的

我们已经在区间 $I$ 上获得了 (II, p. 54, th. 2) 受管制函数的原语，作为步骤函数原语的统一极限。这个过程可以用稍微不同的方式来表达：让$x_0, x$是$I$的任意两个点，使得$x_0 < x$；我们将区间 $[x_0, x]$ 区间 $[x_i, x_{i+1}]$ 的任何序列与并 $[x_0, x]$ 称为“细分”，其中 $(x_i)_{0 \leq i \leq n}$ 是点的严格递增的序列 $[x_0, x]$使得$x_n = x$。我们将相对于I上定义的向量函数$f$以及由$[x_i,\ x_{i+1}]$形成的细分（形式的任何表达式）调用*黎曼和*
$$
\sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)
$$
其中 $t_i$ 属于到 $[x_i,\ x_{i+1}]$ 代表 $0 \leq i \leq n-1$。那么就有以下命题：

#### 命题 5 {#fvr-ii-s1-prop-5 .statement tag=087J}

*令$f$为区间I上的受管制函数，令$g$为I上$f$的原语，$[x_0,\ x]$包含在I中的紧致区间。对于每个$\varepsilon > 0$，都存在数$\rho > 0$，这样，对于$[x_0,\ x]$到区间的长度$\leq \rho$的每一个细分，都有*
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon
$$
*(1)*
*对于相对于该细分的每个黎曼和。*

事实上，让 $f_1$ 成为一个步骤函数，使得对于每个 $y \in [x_0,\ x]$ 都有 $\|f(y) - f_1(y)\| \leq \varepsilon$；一个有，用 $g_1$ 表示 I 上的$f_1$原语，
$$
\|g(x) - g(x_0) - (g_1(x) - g_1(x_0))\| \leq \varepsilon(x - x_0)
$$
平均而言值定理，另一方面
$$
\left| \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) - \sum_{i=0}^{n-1} f_1(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon(x - x_0).
$$

因此，当$f$是*步骤函数*时，足以证明命题。 设$(y_k)_{1 \leq k \leq m}$为$[x_0,\ x]$中$f$的间断点点的严格递增的有限序列。 对于$[x_0,\ x]$每次细分为长度为$\leq \rho$的区间，每个点$y_k$最多属于这些区间中的两个；因此，$f$ 不恒定的间隔不能超过 $2m$ 个；但是，在这样的区间 $[x_i,\ x_{i+1}]$ 上，有
$$
\|g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i)\| \leq 2M (x_{i+1} - x_i)
$$
用$M$表示$\|f\|$在$[x_0,\ x]$上的最小上限；另一方面，当 $f$ 恒定于 $[x_i,\ x_{i+1}]$ 时，有
$$
g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i) = 0.
$$
由此可见差异
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right|
$$
不能超过$4Mm\rho$；因此只需$\rho \leq \varepsilon / 4Mm$即可获得(1)。

#### 注 1 {#fvr-ii-s1-n4-rem-1 .statement tag=087K}

当$f$是*连续*属性时。 5可以更简单地证明：由于$f$在$[x_0,\ x]$上一致连续，因此存在$\rho > 0$，使得在$[x_0,\ x]$中包含的长度$\leq \rho$的每个区间上，$f$的振荡为$\leq \frac{\varepsilon}{x - x_0}$；对于 $[x_0,\ x]$ 到长度 $\leq \rho$ 的区间 $[x_i,\ x_{i+1}]$ 的每个细分，以及 $[x_i,\ x_{i+1}]$ 中 $t_i$ 的每选择对于 $0 \leq i \leq n-1$，步长函数 $f_1$ 等于$[x_i,\ x_{i+1}]$ ($0 \leq i \leq n-1$) 上的$f(t_i)$，以及点 x 处的$f(x)$，使得$[x_0, x]$ 上的$\| f(y) - f_1(y) \| \leq \frac{\varepsilon}{x - x_0}$；如果 $g_1$ 是 $f_1$ 的原语，则有
$$
g_1(x) - g_1(x_0) = \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i),
$$
因此关系 (1) 紧随平均值值定理而来。

在本章的其余部分中，我们将仅限于研究区间I上*受管制的*函数的原语。对于这样的函数$f$，对于E中的值，$f$的原语$g$，对于I的任意两个点$x_0, x$，E的元素$g(x) - g(x_0)$（显然是相同的，无论是哪个原语） $f$ 的$g$ 被称为函数* $f$ *从* $x_0$ *到* $x$（或*在紧致区间* $[x_0, x]$）的积分，并用$\int_{x_0}^x f(t) dt$ 或$\int_{x_0}^x f$。这个名字和记号都起源于prop。 II、p. 57的5，表明积分可以用黎曼和任意逼近；更具体地说，我们可以将$[x_0, x]$细分为等于区间，

$$
\frac{1}{x - x_0} \int_{x_0}^x f(t) dt = \lim_{n \to \infty} \frac{1}{n} \sum_{k=0}^{n-1} f \left( x_0 + k \frac{x - x_0}{n} \right).
$$

在其他字中，元素$\frac{1}{x - x_0} \int_{x_0}^x f(t) dt$是$f$的值的*算术平均值*的极限，在$[x_0, x]$细分为等于区间的区间的左端点；有人也称其为区间$[x_0, x]$上函数$f$的*平均值*（或*平均值值*）。

到定义，函数$x \mapsto \int_{x_0}^x f(t) dt$正是$f$的原语，在点$x_0 \in I$消失；也可以用$\int_{x_0}^x f(t) dt$或$\int_{x_0}^x f$来表示。

#### 注 2 {#fvr-ii-s1-n4-rem-2 .statement tag=087L}

对于I上定义的任意函数$h$，值在E中，元素$h(x) - h(x_0)$也可写为$h(t)\Big|_{x_0}^x$；通过这个记号，我们可以看出，如果$g$是I上受管制的函数$f$的任何原语，则有

$$
\int_{x_0}^x f(t) dt = g(t)\Big|_{x_0}^x.
$$

#### 注 3 {#fvr-ii-s1-n4-rem-3 .statement tag=087M}

表达式$\int_{x_0}^x f(t) dt$和$g(t)\Big|_{x_0}^x$是表示组合的缩写符号，其中出现字母$x, x_0, f, g$，但*不是*字母$t$（*cf.集合理论*，I， p. 15);有人说这些符号中$t$是一个“*虚拟变量*”：因此可以通过任何其他不同于$x, x_0, f$和$g$的变量（以及可能进入这些符号出现的证明的变量）来计算替换$t$，而不改变如此获得的符号的含义（读者可以将这些符号与以下符号进行比较） $\sum_{i=1}^n x_i$，或$\bigcup X_i$，其中$i$同样是虚拟变量）。

#### 注 4 {#fvr-ii-s1-n4-rem-4 .statement tag=087N}

黎曼积分的近似和与积分概念的历史起源之一、面积“度量”的问题密切相关。我们将在《整的》一书中回到这个点，这本书专门讨论了这个问题所引向的积分概念的推广；其中推广函数“*集成*”不一定定义在$\mathbf{R}$的子集上；此外，即使当处理（不一定受监管）实数变量的实数函数$f$时，可以定义积分$\int_{x_0}^x f(t)\,dt$，函数$x \mapsto \int_{x_0}^x f(t)\,dt$并不总是$f$的原语，并且存在函数，其具有原语但不是我们提到的意义上的“可积”。

### 5. 积分的性质

受管制的函数积分的性质只是将第 1 章中演示的导数性质转换为适当的记号。 I。

首先，公式(3)表明，无论I的点$x,\ y,\ z$，都有

$$
\int_x^x f(t)\,dt = 0 \tag{4}
$$

$$
\int_x^y f(t)\,dt + \int_y^x f(t)\,dt = 0 \tag{5}
$$

$$
\int_x^y f(t)\,dt + \int_y^z f(t)\,dt + \int_z^x f(t)\,dt = 0 \tag{6}
$$

来自道具。 II 中有 1 个，p. 52 一个有

$$
\int_{x_0}^x (f + g) = \int_{x_0}^x f + \int_{x_0}^x g \tag{7}
$$

对于每个标量 $k$

$$
\int_{x_0}^x k f = k \int_{x_0}^x f. \tag{8}
$$

设E、F是$\mathbf{R}$上的两个完全赋范空间，u是从E到F的连续线性映射。如果f是I上的调节函数，且值在E中，则$u \circ f$是在函数上的调节函数 F 中的 I 和值（II、p. 6，对应 2），其中一个对应 $a, b \in I$（I、p. 13，第 2 条）

$$
\int_a^b u(f(t))\,dt = u \left( \int_a^b f(t)\,dt \right). \tag{9}
$$

现在令 E、F、G 为 $\mathbf{R}$ 上的三个完整范数空间，以及 $(x, y) \mapsto |x.y|$ $E \times F$ 的连续双线性映射到 G 中。令 f 和 g 为在 I 上定义且连续的两个向量函数，取它们值分别在E和F中；此外，假设 f 和 g 是*受管制* 函数的两个原语，我们通过滥用语言将其表示为 $f'$ 和 $g'$（除了可数集合的补集之外，这些函数实际上并不能保证分别等于 f 和 g 的导数）。通过道具。 I、p. 6、函数$h(x) = [f(x).g(x)]$中的 3 个，在I的可数子集的补集的每点处，有一个等于$[f(x).g'(x)] + [f'(x).g(x)]$的导数。现在，通过 $[x.y]$ 和 cor 的连续性。 II、p. 55 中的 2 个、函数、$[f.g']$ 和 $[f'.g]$ 中的每一个是 I 上受监管的函数；所以一个人有公式

$$
\int_a^b [f'(t).g(t)]\,dt = [f(t).g(t)]\Big|_a^b - \int_a^b |f(t).g'(t)|\,dt \tag{10}
$$

称为*公式用于部分*的积分，它允许人们评估许多原语。

例如，将公式与部分积分，得到以下公式

$$
\int_{x_0}^{x} t f'(t) \, dt = t f(t) \Big|_{x_0}^{x} - \int_{x_0}^{x} f(t) \, dt
$$

因此，减少了两个函数 $f(x)$ 和 $x f'(x)$ 之一的原语评估到另一个。

同样，如果$f$和$g$在区间$I$上可微分$n$倍，并且如果$f^{(n)}$和$g^{(n)}$在$I$上调节函数，则I的公式(5)， p. 21 等价于：

$$
\int_a^b [f^{(n)}(t) \cdot g(t)] \, dt
$$
$$
= \left( \sum_{p=0}^{n-1} (-1)^p [f^{(n-p-1)}(t) \cdot g^{(p)}(t)] \right) \Bigg|_a^b + (-1)^n \int_a^b [f(t) \cdot g^{(n)}(t)] \, dt
$$
(11)

其中*公式通过部分对阶n*进行积分。

现在让我们翻译公式以求复合函数的微分（I，p. 9，道具5）。令$f$是在$I$上定义且连续的实函数，它是$I$上的*调节*函数的原语（我们再次滥用语言将其写为$f'$）；此外，让 $g$ 成为开区间 $J$ 包含 $f(I)$ 上的*连续* 向量函数（其中值处于完全规范的空间中）；如果$h$表示$J$上$g$的任意原语，则$h$允许在$J$的每个点处等于$g$的导数（II，p. 56，道具3）；因此，复合函数$h \circ f$允许在$I$的可数子集的补集（相对于$I$）的所有点处等于$g(f(x)) f'(x)$的导数（I，p. 9，道具5）；由于函数 $g(f(x)) f'(x)$ 受到监管（II、p. 55，cor. 2），因此可以写公式

$$
\int_a^b g(f(t)) f'(t) \, dt = \int_{f(a)}^{f(b)} g(u) \, du
$$
(12)

将变量*的变换称为*公式，这也有利于原语的求值。

例如，如果取 $f(x) = x^2$，则可以看到公式 (12) 约化从一个到另一个对函数 $g(x)$ 和 $x g(x^2)$ 基元的求值。

为了将值定理 (I, p. 14, th. 1) 转换为实数调节函数的原语，我们首先指出紧致区间 $I$ 上的实数调节函数 $f$ 是以$I$为界；设$J$为$I$点集合，其中$f$*连续*，并放入$m = \inf_{x \in J} f(x)$，$M = \sup_{x \in J} f(x)$；知道 (II, p. 54, th. 3) $I \cap \mathbf{C}J$ 是可数的；此外，如果$B$相对于$I$是$I$和$m' = \inf_{x \in B} f(x)$、$M' = \sup_{x \in B} f(x)$的任何可数子集的补集，则有$m' \leq m \leq M \leq M'$：事实上，对于每个点$x \in J$，有B 的点$y$任意接近$x$、从而$m' \leq f(y) \leq M'$；因为$f$在点$x$连续，所以$y$接近$x$（$y$留在B中）$m' \leq f(x) \leq M'$，这证明了我们的断言。既然如此，翻译平均值值定理会得到以下命题：

#### 命题 6（平均定理）{#fvr-ii-s1-prop-6 .statement tag=087O}

*令$f$为紧凑型区间$l = [a, b]$上的真实调节函数；如果$J$是I的点的集合，其中$f$是连续的，并且$m = \inf_{x \in J} f(x)$，$M = \sup_{x \in J} f(x)$，那么*

$$
m < \frac{1}{b-a} \int_a^b f(t)\,dt < M
$$

*(13)*

*除非 $f$ 在 J 上是常数，在这种情况下，(13) 的三个成员相等。*

在其他字中，I中规定的函数$f$的*平均值*位于$f$与I的子集之间，其中$f$是连续的。

#### 推论 1 {#fvr-ii-s1-prop-6-cor-1 .statement tag=087P}

*如果I上的实调节函数$f$使得$f(x) \geq 0$在点处，其中$f$是连续的，则*$\frac{1}{b-a} \int_a^b f(t)\,dt > 0$*除非*$f(x) = 0$*在点处，其中*$f$*是连续的。*

#### 推论 2 {#fvr-ii-s1-prop-6-cor-2 .statement tag=087Q}

*令$f$和$g$为I上的两个实数调节函数，使得$g(x) \geq 0$*在点，其中*$g$*是连续的；如果* $m$ *和* $M$ *是下确界并且* $f$ *的至少上界超过点的集合，其中* $f$ *是连续的，那么*

$$
\frac{m}{b-a} \int_a^b g(t)\,dt \leq \frac{1}{b-a} \int_a^b f(t)g(t)\,dt \leq \frac{M}{b-a} \int_a^b g(t)\,dt.
$$

*(14)*

*前两个项（或最后两个）在每个点处不相等除非* $g(x)(f(x) - m) = 0$ *（或$g(x)(f(x) - M) = 0$），其中* $f$ *和* $g$ *是连续的。*

对于向量函数，平均值定理 (I, p. 15, th. 2) 产生以下命题：

#### 命题 7 {#fvr-ii-s1-prop-7 .statement tag=087R}

*让* $\mathbf{f}$ *成为紧凑区间* $I = [a, b]$上的受监管向量函数，*与值在完整规范的空间* $E$，*并让* $g$ *成为真正受监管的函数在*$I$，*使得*$g(x) \geq 0$*在点，其中*$g$*是连续的；在这些情况下*

$$
\left\| \int_a^b \mathbf{f}(t)g(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| g(t)\,dt.
$$

*(15)*

*尤其，*

$$
\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| \,dt.
$$

*(16)*

### 6. 右 taylor'S 公式中的余数进行积分公式；高阶阶的原语

公式通过阶 $n$ 的部分进行积分 (II, p. 60, 公式 (11)) 允许用积分的项表达泰勒展开中的余数 $r_n(x)$ 函数的阶$n$，允许区间I（I，p. 22）上受监管的$(n+1)^{th}$衍生；事实上，在替换上，在 (12) 中，$f$ $f'$，$b$ $x$，$g(t)$ 函数 $(t-x)^n/n!$，可以得出以下结论：

$$
f(x) = f(a) + f'(a) \frac{(x-a)}{1!} + f''(a) \frac{(x-a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x-a)^n}{n!} + \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt
$$

其他字

$$
r_n(x) = \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt,
$$

其中公式通常允许人们获得余数的简单界限。

给定区间I上的受管制函数$f$，$f$的任意原语$g$，在I中连续，依次接纳一个原语； $f$的任意基元的任意基元被称为$f$的*第二基元*。更一般地，$f$的阶$n-1$的基元的基元被称为阶*$n$的$f$的基元。人们立即看到，通过$n$上的归纳，$f$的阶$n$的两个基元之差是*次数的多项式，最多等于*$n-1$（E中的系数）。如果指定其值及其在点 $a \in I$ 处的第一个 $n-1$ 导数，则 $f$ 的阶 $n$ 的原语完全确定。

特别是，$\int_a^{(n)} f$表示$f$的阶$n$的原语及其第一个$n-1$导数在点$a$处消失。将阶 $n-1$ 的泰勒公式应用于此基元，表明如果 $g = \int_a^{(n)} f$，则

$$
g(x) = \int_a^x f(t) \frac{(x-t)^{n-1}}{(n-1)!} \, dt
$$

因此将阶 $n$ 的原语的确定简化为一个积分。

### 习题 {#fvr-ii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
