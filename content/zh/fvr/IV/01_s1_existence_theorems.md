---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 1
section_title: EXISTENCE THEOREMS
lang: zh
source: fvr-i-vii
book_pages: 163-177, 199-204
pdf_pages: 0178-0192, 0214-0219
extraction: ocr
subsections:
    - "no": 1
      title: THE CONCEPT OF A DIFFERENTIAL EQUATION
      page: 163
      pdf_page: 178
    - "no": 2
      title: DIFFERENTIAL EQUATIONS ADMITTING SOLUTIONS THAT ARE PRIMITIVES OF REGULATED FUNCTIONS
      page: 164
      pdf_page: 179
    - "no": 3
      title: EXISTENCE OF APPROXIMATE SOLUTIONS
      page: 166
      pdf_page: 181
    - "no": 4
      title: COMPARISON OF APPROXIMATE SOLUTIONS
      page: 168
      pdf_page: 183
    - "no": 5
      title: EXISTENCE AND UNIQUENESS OF SOLUTIONS OF LIPSCHITZ AND LOCALLY LIPSCHITZ EQUATIONS
      page: 171
      pdf_page: 186
    - "no": 6
      title: CONTINUITY OF INTEGRALS AS FUNCTIONS OF A PARAMETER
      page: 174
      pdf_page: 189
    - "no": 7
      title: DEPENDENCE ON INITIAL CONDITIONS
      page: 176
      pdf_page: 191
statements: 29
exercises: 18
content_sha256: 05290f17e26c14abfeda20cd661e7a80836138668abe2d5836d278e84198ecd9
translated_from: content/en/fvr/IV/01_s1_existence_theorems.md
translation_method: google
source_content_sha256: 0e1758ad98dd52ed21cb9dc147ffdbd0f25ec001d00ee20b8f91629799eb1263
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4ca5a7fc3cf53a7cac2775b8e19b1b6528afa68000aaabb6c1e391cc2b44d5c7
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。存在定理

### 1.微分方程的概念

令I为包含在$\mathbf{R}$中的区间，不简化为单个点，E是$\mathbf{R}$上的*拓扑向量空间*，并且A和B是E的两个开子集。令$(x, y, t) \mapsto g(x, y, t)$为$A \times B \times I$到E的连续映射；对于I的每个*可微分*映射u到A，其导数取B中的值，我们将I的映射$t \mapsto g(u(t), u'(t), t)$关联到E，并用$\tilde{g}(u)$表示；因此$\tilde{g}$定义在I的可微分函数到B的集合$\mathscr{D}(A, B)$上，其导数在B中具有值。我们可以说方程$\tilde{g}(u) = 0$是u中的*微分方程*（相对于*实数*变量t）；该方程的 *解* 也称为微分方程的 *整的*（在区间 I 上）；它是 I 到 A 的可微分映射，其导数取 B 中的值，使得$g(u(t), u'(t), t) = 0$ 对于*每个* $t \in I$。通过滥用语言，我们将在形式中写出微分方程$\tilde{g}(u) = 0$

$$
g(x, x', t) = 0,
$$

理解 x 属于到集合 $\mathscr{D}(A, B)$。

对于例，对于$I = E = \mathbf{R}$关系

$$
x' = 2t, \qquad tx' - 2x = 0, \qquad {x'}^2 - 4x = 0, \qquad x - t^2 = 0
$$

是微分方程，所有四个方程都承认函数 $x(t) = t^2$ 为解

在这个章中，我们在原理中仅考虑E是$\mathbf{R}$上的*完全范数空间*的情况，并且微分方程是特定的形式

$$
x' = f(t, x)
$$

（“$x'$ 中的显式方程”），其中 f 表示在 $I \times H$ 上定义的函数，其中值在 E 中，并且 H 是 E 的*开* 非空子集。 We shall, moreover, widen a little the concept of a *solution* (or *integral*) of such an equation (on the interval I): we shall say that a function u, defined and continuous on I, with values in H, is a solution (or integral) of the equation (I) if there exists a *countable* subset A of I such that at every point t of the complement of A in I the function u admits a derivative $u'(t)$ such that $u'(t) = f(t, u(t))$. 如果$u$是可微的并且对于每个点$t \in I$满足上面的关系，我们可以说它是等式（1）在I上的严格解。

在形式 $x' = f(t)$ 微分方程的特殊情况下，其中 $f$ 是 I 到 E 中的映射，上述意义上的解是函数 $f$ (II, p. 51) 的原语，并且严格解是严格原语。

当E是完全范数空间$E_i$（$1 \leq i \leq n$）的乘积时，可以写出$x = (x_i)_{1 \leq i \leq n}$和$f = (f_i)_{1 \leq i \leq n}$，其中$x_i$是从I到$E_i$的映射，$f_i$是映射从$I \times H$变为$E_i$；那么方程(1)就相当于微分方程的系统
$$
x'_i = f_i(t, x_1, x_2, \ldots, x_n) \qquad (1 \leq i \leq n).
$$
(2)

最重要的情况是$E_i$等于$\mathbf{R}$或$\mathbf{C}$；然后可以说 (2) 是标量微分方程的系统。

一可约化形式关系的学习
$$
x^{(n)} = f(t, x, x', \ldots, x^{(n-1)})
$$
到系统 (2)，其中 $x$ 是 I 上 $n$ 次可微的向量函数；对于放置$x_1 = x$，$x_p = x^{(p-1)}$对于$2 \leq p \leq n$，关系 (3) 相当于系统
$$
\begin{cases}
x'_i = x_{i+1} & (1 \leq i \leq n-1) \\
x'_n = f(t, x_1, x_2, \ldots, x_n).
\end{cases}
$$
(4)

形式(3)的关系称为阶$n$的微分方程（显式求解$x^{(n)}$）；相反，形式(1)的方程称为第一个阶的微分方程。

类似地，可以约化形式的任何“微分方程系统”
$$
D^{n_i} x_i = f_i(t, x_1, Dx_1, \ldots, D^{n_1} x_1, \ldots, x_p, Dx_p, \ldots, D^{n_p-1} x_p)
$$
形式 (2) 的 $(1 \leq i \leq p)$ 到系统，其中 $x_i$ 是 I 上的函数，其在 I 上可微分$n_i$ 倍（对于 $1 \leq i \leq p$）。

### 2. 微分方程承认解是规定函数的原语

回想一下（II，p. 54，def.3），如果在I的每个紧凑子集上，在间隔$I \subset \mathbf{R}$上定义的向量函数$u$被认为是受管制的，则它是步骤函数的统一极限；等效的条件是，在I函数$u$的每个内部点都有一个右极限和一个左极限，并且在I的左端点还有一个右极限和一个左极限在I的右侧端点，当这两个点属于到I（II，p. 54，第3个）时。在这个章中，我们将把自己限制在微分方程（1）中，其中每个解都是I上受管制的函数的原语。如果对于I的每个连续映射$u$进入H，函数$f(t, u(t))$在I上调节，则显然满足条件；下面的引理为此提供了足够的条件：

#### 引理 1 {#fvr-iv-s1-lem-1 .statement tag=08BD}

令$f$是从$I \times H$到$E$的映射，这样，在将$f_x$（对于每个$x \in H$）写入$I$的映射$t \mapsto f(t, x)$到$E$时，满足以下条件：1°每$x \in H$对$f_x$调节$I$； 2° $H$ 的映射 $x \mapsto f_x$ 到映射的集合 $\mathscr{F}(I, E)$ 从$I$ 到$E$ 是连续的，当赋予$\mathscr{F}(I, E)$ 拓扑紧收敛时（Gen.1） 顶部.，X，p. 278）。 在这些条件下：

1° 对于$I$到$H$函数$t \mapsto f(t, u(t))$的每个连续映射$u$，在$I$上调节；更准确地说，函数在点$t_0 \in I$的右（或左）极限等于函数$t \mapsto f(t, u(t_0))$在点$t_0$的右（或左）极限。

2° 如果$(u_n)$是$I$的映射的序列进入$H$，并且在$I$的每个紧凑子集上均匀收敛到$I$的连续函数$u$进入$H$，则函数 $t \mapsto f(t, u_n(t))$ 的序列在$I$ 的每个紧凑子集上一致收敛到$f(t, u(t))$。

1 令$c$为$f(t, u(t_0))$在点$t_0$处的右极限；对于每个$\varepsilon > 0$，$I$中都有一个$t_0$的紧凑邻域$V$，这样$\|f(t, u(t_0)) - c\| \leq \varepsilon$适用于$t \in V$和$t > t_0$。另一方面，存在$\delta > 0$使得关系

$$
x \in H, \quad \|x - u(t_0)\| \leq \delta
$$

对所有$s \in V$暗示$\|f(s, x) - f(s, u(t_0))\| \leq \varepsilon$；如果$W \subset V$是$I$中$t_0$的邻域，使得每个$t \in W$都有$\|u(t) - u(t_0)\| \leq \delta$，则$t \in W$和$t > t_0$有$\|f(t, u(t)) - c\| \leq 2\varepsilon$，这证明$c$是右极限 $f(t, u(t))$ 点 $t_0$。

2 令$K$为$I$的紧子集；由于$u$在$I$上连续，$u(K)$是$H$的紧子集；对于每一个$\varepsilon > 0$和$x \in u(K)$，都存在数$\delta_x$，这样，对于每一个$y \in H, \|y - x\| \leq \delta_x$和每一个$t \in K$，都有$\|f(t, y) - f(t, x)\| \leq \varepsilon$。存在点 $x_i \in u(K)$ 的有限数，使得具有中心 $x_i$ 和半径 $\frac{1}{2}\delta_{x_i}$ 形式的封闭球覆盖$u(K)$；让$\delta = \operatorname{Min}(\delta_{x_i})$。到假设时，存在整数$n_0$，因此对于$n \geq n_0$，每$t \in K$就有$\|u_n(t) - u(t)\| \leq \frac{1}{2}\delta$。现在，对于每个 $t \in K$ 都存在指标 $i$ 这样

$$
\|u(t) - x_i\| \leq \frac{1}{2}\delta_{x_i};
$$

因而，每 $t \in K$ 和每 $n \geq n_0$ 都有 $\|u_n(t) - x_i\| \leq \delta_x$、从而 $\|f(t, u_n(t)) - f(t, u(t))\| \leq 2\varepsilon$

对于其余部分，截面I将表示包含在$\mathbf{R}$中的区间，不会减少为单个点，$H$包含在标准化空间$E$中的开非空集合，并且$f$映射从$I \times H$变为$E$满足引理1的假设。

#### 命题 1 {#fvr-iv-s1-prop-1 .statement tag=08BE}

设$t_0$为$I$的点，以及$x_0$点为$H$；对于$I$上连续的函数$u$为式(1)的解，并在点$t_0$取值$x_0$，满足关系是充分必要的

$$
u(t) = x_0 + \int_{t_0}^t f(s, u(s))\, ds
$$

每$t \in I$。

事实上，到引理 1，如果$u$是(1)在$I$上的解，则$f(t, u(t))$受到调节，因而(6)的右侧被定义并且对于每个$t \in I$等于$u(t)$。相反，如果 $u$ 是满足 (6) 的连续函数，则 $f(t, u(t))$ 由引理 1 调节，因而 $u$ 的导数等于 $f(t, u(t))$，除了在可数子集的点处$I$。

#### 推论{#fvr-iv-s1-n2-cor-1 .statement tag=08BF}

*在I的每个点与该区间的左（或右）端点不同，I上（1）的每个解 u 允许左（或右）导数等于$f(t, u(t))$的左（右）极限在此点。*

#### 命题 2 {#fvr-iv-s1-prop-2 .statement tag=08BG}

*如果f是从$I \times H$到E的连续映射，则I上(1)的每个解都是严格的解。*

事实上，这样的解$u$是连续函数$f(t, u(t))$的原语（II，p. 66，道具3）。

此外，我们注，$I \times H$上的连续函数$f$满足引理1的条件（*Gen.Top.*，X，p. 286，cor.3）。

接下来我们将任意选择$t_0 \in I$和$x_0 \in H$，并考察$I$上（或$I$中$t_0$的邻域）是否存在（1）的解，取值$x_0$在点$t_0$（或者，结果相同，（6）的解）。

### 3. 存在近似解

给定数$\varepsilon > 0$，我们可以说，$I$到$H$的连续映射$u$是微分方程*解到*$\varepsilon$的*近似值

$$
x' = f(t, x)
$$

如果，$I$的*可数* 子集的补集的点，函数$u$承认满足条件的导数

$$
\|u'(t) - f(t, u(t))\| \leq \varepsilon.
$$

设$(t_0, x_0)$为$I \times H$中的点；由于 $f$ 满足引理 1 (IV, p. 165) 的假设，因此在 $I$ 中存在 $t_0$ 的紧邻域 $J$，使得 $f(t, x_0)$ 有界于 $J$，以及一个开球$S$，其中中心$x_0$包含在$H$中，使得$f(t, x) - f(t, x_0)$以$J \times S$为界；由此可见，$f(t, x)$ 在 $J \times S$ 上有*边界*。 *在此过程中，小节 J 将表示一个紧凑区间，即 I 中 t_0 的邻域，S 将是一个开球，其中心 x_0 和半径 r 包含在 H 中，其中 J 和 S 使得 f 有界于 J × S； M 表示 \|f(t, x)\| 的上界超过 J × S。*

#### 命题 3 {#fvr-iv-s1-prop-3 .statement tag=08BH}

*在 J 中包含左（或右）端点 t_0 的每个紧凑区间上，长度小于 r/(M + ε)，在等式 (1) 的 ε 范围内存在一个近似解，其中值在 S 中，并且在 t_0 处等于 x_0。*

我们假设 $t_0$ 不是 J 的右端点，并证明命题对于左端点为 $t_0$ 的区间。令$\mathscr{M}$为(1)的解的集合到$\varepsilon$之内，其中每个在S中取值，在$t_0$等于$x_0$，并定义在J中包含的半开区间$[t_0, b[$上（该区间取决于近似解正在考虑中）。首先我们证明 $\mathscr{M}$ 不为空。设c在$t_0$处是$f(t, x_0)$的右极限；通过引理 1 (IV, p. 165) 函数 $f(t, x_0 + c(t - t_0))$ 在 $t_0$ 处有右极限等于 c，因此函数 $x_0 + c(t - t_0)$ 的限制为足够小的半开区间$[t_0, b[$ 将从属于变为 $\mathscr{M}$。

我们通过关系“u是v的限制”阶集合$\mathscr{M}$，并证明$\mathscr{M}$是归纳性的（集合理论，III，p. 154）。令$(u_\alpha)$为$\mathscr{M}$和$[t_0, b_\alpha[$的总有序子集，$u_\alpha$定义的区间：对于$b_\alpha \leq b_\beta$函数$u_\beta$因此是$u_\alpha$的扩张。区间$[t_0, b_\alpha[$中的并是J中包含的区间$[t_0, b[$，对于每个$\alpha$，在$[t_0, b[$上定义的函数u，重合和$u_\alpha$在$[t_0, b_\alpha[$上定义； $b_\alpha$ 中，有递增序列 $(b_{\alpha_n})$ 趋于 b；因为你在$[t_0, b_{\alpha_n}[$函数上同意$u_{\alpha_n}$，所以你承认$[t_0, b[$的可数子集的补集的导数满足（7）点，因此集合$(u_\alpha)$的上等$\mathscr{M}$。

根据Zorn的引理（集合理论，III，p. 154，第2），$\mathscr{M}$承认极大元素$u_0$；我们将证明，如果$[t_0, t_1[$是定义$u_0$的区间，则$t_1$是J的右侧端点，否则$t_1 - t_0 \geq r/(M + \varepsilon)$。我们通过反证法来论证，假设这些条件都不成立；首先我们证明可以通过点 $t_1$ 的连续性来扩展 $u_0$；事实上，对于 $[t_0, t_1[$ 中的任何 s 和 t，

$$
\|u_0(s) - u_0(t)\| \leq (M + \varepsilon)|s - t|
$$

平均值定理；柯西准则表明$u_0$在点$t_1$处承认左极限$x_1 \in S$。现在令$c_1$为函数$f(t, x_1)$中$t_1$处的右极限；一个有 $\|c_1\| \leq M$；与证明开头相同的论点表明，可以通过函数$x_1 + c_1(t - t_1)$将扩展$u_0$转换为左端点为$t_1$的半开区间，从而将函数属于扩展为$\mathscr{M}$，即荒谬的。这就证明了命题。

当 f 在 $J \times S$ 一个可以证明上一致连续时。 3 不使用 Zorn 的引理（IV，p. 199，练习 1a））。

#### 命题 4 {#fvr-iv-s1-prop-4 .statement tag=08BI}

*(1) 的近似解到$\varepsilon$之内的集合，在相同的间隔$K \subset J$上定义并在 S 中取值，是一致等连续的。*

事实上，如果 u 是这个集合中的任何函数并且 s 和 t 是 K 的两个点，那么平均值定理

$$
\|u(s) - u(t)\| \leq (M + \varepsilon)|s - t|.
$$

#### 推论（皮亚诺定理）{#fvr-iv-s1-n3-cor-1 .statement tag=08BJ}

*如果 E 的有限维超过 $\mathbf{R}$，则存在 (1) 的解，其中值在 S 中，并且在 $t_0$ 处等于 $x_0$，在每个紧凑区间 K 上，左（或右）端点 $t_0$ 包含在 J 中并且具有长度 $< r/M$.*

确实，通过道具。 3、一旦$n$足够大，在$1/n$内就有(1)的近似解$u_n$，定义在$K$上，值在$S$中，并且在$t_0$处等于$x_0$。此外，从 $n$ 的某个值开始，$u_n(K)$ 包含在一个具有中心 $x_0$ 和半径 $< r$ 的“封闭”球中，与 $n$ 无关。 $u_n$的集合是等连续的（命题4），并且由于$E$是有限维的集合$S$在$E$中相对紧；所以对于$u_n(t)$的每一个$t \in K$集合来说，在$E$中相对紧凑。由阿斯科利的定理（*Gen.Top.*，X，p. 290，第2）$u_n$的集合相对紧凑，从$K$到映射的空间$\mathscr{F}(K; E)$相对紧凑$E$ 赋予制服范数。因此，从$(u_n)$的$(u_{n_k})$中提取出序列，它在$K$上均匀收敛到连续的函数$u$。一个有$u(K) \subset S$，所以$t \mapsto f(t, u(t))$定义在$K$上；通过引理 1 (IV, p. 165)，$f(t, u_{n_k}(t))$在$K$上均匀收敛到$f(t, u(t))$；由 (IV, p. 4, 公式 (7))，$u_{n_k}$ 是函数的原语，它在 $K$ 上统一趋向于 $f(t, u(t))$，所以 (II, p. 52, th. 1) $u$ 是 $K$ 上 (1) 的解，并且等于点 $t_0$ 上的 $x_0$。

#### 注 1 {#fvr-iv-s1-n3-rem-1 .statement tag=08BK}

微分方程 (1) 可以有“无穷多个”整的，在给定点处取相同的值。对于例，标量微分方程 $x' = 2\sqrt{|x|}$ 具有由下式定义的所有函数

$$
\begin{array}{ll}
u(t) = 0 & \text{for } -\beta \leq t \leq \alpha \\
u(t) = -(t + \beta)^2 & \text{for } t \leq -\beta \\
u(t) = (t - \alpha)^2 & \text{for } t \geq \alpha
\end{array}
$$

对于任何正数 $\alpha$ 和 $\beta$，在点 $t = 0$ 取值 0 的积分。

#### 注 2 {#fvr-iv-s1-n3-rem-2 .statement tag=08BL}

当$E$是*无限*维数（IV，p. 204，练习18）的任意完全范数空间时，皮亚诺的定理不再成立。

### 4. 近似解的比较

接下来，I和$H$如上所述，分别表示$\mathbf{R}$中包含的区间和赋范空间$E$中的开集合； $t_0$ 是 I 中的点。

#### 定义 1 {#fvr-iv-s1-def-1 .statement tag=08BM}

*给定一个正实数函数* $t \mapsto k(t)$ *定义在* $I$，*有人说映射* $f$ *从* $I \times H$ *进入* $E$ *是 Lipschitz 相对于函数* $k(t)$ *如果，对于每个* $x \in H$，*函数* $t \mapsto f(t, x)$ *受监管* $I$，*并且如果对于每个* $t \in I$ *和点* $x_1, x_2$ *的每个对* $H$，*一个有（“Lipschitz 条件")*

$$
\| f(t, x_1) - f(t, x_2) \| \leq k(t) \| x_1 - x_2 \|.
$$

(8)

如果对于某些*常数* $k \geq 0$，集合是 Lipschitz，那么我们可以说$f$ 是$I \times H$ 上的 *Lipschitz*（无需更具体）。 $I \times H$ 上的 Lipschitz 函数满足 IV、p. 165 的引理 1 的假设是直接的（逆命题为假）；当 $f$ 是 Lipschitz（在 $I \times H$ 上）时，可以说微分方程

$$
x' = f(t, x)
$$

(1)

是*Lipschitz*（$I \times H$）。

#### 例 {#fvr-iv-s1-n4-exa-1 .statement tag=08BN}

当$E = \mathbf{R}$和$H$是$\mathbf{R}$中的一个区间时，如果函数$f(t, x)$在每点$(t, x)$处承认一个*偏导数*$f'_x$（II，p. 74） $I \times H$，使得$|f'_x(t, x)| \leq k(t)$在$I \times H$上，则满足条件(8)，即值定理；稍后我们将看到这个例如何推广到$E$是任意范数空间的情况。

如果$f$是$I \times H$上的Lipschitz，那么对于每个紧凑子区间$J \subset I$和每个开球$S \subset H$，$f$在$J \times S$上*有界*。因此道具。可以应用式3(IV，p. 166)，证明式(1)近似解的存在性。但我们还有以下命题，它允许我们“比较”两个近似的解：

#### 命题 5 {#fvr-iv-s1-prop-5 .statement tag=08BO}

*令$k(t)$为$I$上的实规函数和$> 0$，令$f(t, x)$为已定义的函数，并令Lipschitz相对于$I \times H$上的$k(t)$。如果$u$和$v$是(1)的两个近似解，分别在$\varepsilon_1$和$\varepsilon_2$之内，在$I$上定义，值在$H$中，那么，对于所有$t \in I$使得$t \geq t_0$，

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\| \Phi(t) + (\varepsilon_1 + \varepsilon_2)\Psi(t)
$$

哪里

$$
\begin{cases}
\Phi(t) = 1 + \int_{t_0}^t k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds \\
\Psi(t) = t - t_0 + \int_{t_0}^t (s - t_0)k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds.
\end{cases}
$$

从关系 $\|u'(t) - f(t, u(t))\| \leq \varepsilon_1$，对可数集合的补集有效，可以从平均值值定理推断出，

$$
\left\| u(t) - u(t_0) - \int_{t_0}^t f(s, u(s))\, ds \right\| \leq \varepsilon_1 (t - t_0)
$$

和类似地

$$
\left\| v(t) - v(t_0) - \int_{t_0}^t f(s, v(s))\, ds \right\| \leq \varepsilon_2 (t - t_0)
$$

从而

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\|
$$
$$
+ \left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| + (\varepsilon_1 + \varepsilon_2)(t - t_0).
$$

由 Lipschitz 条件 (8) 一有

$$
\left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| \leq \int_{t_0}^t \|f(s, u(s)) - f(s, v(s))\|\, ds
$$
$$
\leq \int_{t_0}^t k(s) \|u(s) - v(s)\|\, ds
$$

从而，放入$w(t) = \|u(t) - v(t)\|$，

$$
w(t) \leq w(t_0) + (\varepsilon_1 + \varepsilon_2)(t - t_0) + \int_{t_0}^t k(s)w(s)\, ds.
$$

因此命题是以下引理的推论：

#### 引理 2 {#fvr-iv-s1-lem-2 .statement tag=08BP}

*如果w是区间[t_0, t_1]上的连续实数函数且满足不等式*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} k(s) w(s) \, ds
$$
(12)

*其中$\varphi$是$[t_0, t_1]$上受监管的函数$\geq 0$，那么，对于$t_0 \leq t \leq t_1$，*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds.
$$
(13)

把$y(t) = \int_{t_0}^t k(s) w(s) \, ds$； 关系 (12) 意味着

$$
y'(t) - k(t) y(t) \leq \varphi(t) k(t)
$$
(14)

是可数集合的补集。

把$z(t) = y(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right)$；那么 (14) 等价于

$$
z'(t) \leq \varphi(t) k(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right).
$$

在应用上，值定理（I，p. 15，第2个）到这个不等式，并注意到$z(t_0) = 0$，我们得到

$$
z(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( - \int_{t_0}^s k(\tau) \, d\tau \right) \, ds
$$

whence

$$
y(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds
$$

并且由于 $w(t) \leq \varphi(t) + y(t)$ 因此得到 (13)。

#### 推论{#fvr-iv-s1-n4-cor-1 .statement tag=08BQ}

*令 $\mathbf{f}$ 为常数 $k > 0$ 的 Lipschitz 函数，在 $\mathbf{I} \times \mathbf{H}$ 上定义。如果$\mathbf{u}$和$\mathbf{v}$分别是(1)在$\varepsilon_1$和$\varepsilon_2$范围内的两个近似解，定义在$\mathbf{I}$上并在$\mathbf{H}$中取它们的值，那么，对于所有$t \in \mathbf{I}$，*

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k |t - t_0|} + (\varepsilon_1 + \varepsilon_2) \frac{e^{k |t - t_0|} - 1}{k}.
$$
(15)

当$t \geq t_0$时，这个不等式实际上是(9)的直接的推论；要证明$t \leq t_0$，只需将其应用于方程即可

$$
\frac{d \mathbf{x}}{ds} = -\mathbf{f}(-s, \mathbf{x})
$$

由变量 $t = -s$ 的变换由 (1) 获得。

#### 注 1 {#fvr-iv-s1-n4-rem-1 .statement tag=08BR}

当$k = 0$不等式(15)被不等式代替时
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| + (\varepsilon_1 + \varepsilon_2) |t - t_0|
$$
其证明为直接的。

#### 注 2 {#fvr-iv-s1-n4-rem-2 .statement tag=08BS}

当E为有限维，且$\mathbf{f}$为$I \times H$上的Lipschitz时，可以证明(1) (IV, p. 166, 命题3)近似解的存在性，而无需使用选择公理 (IV, p. 199, 练习1) b））。

#### 命题 6 {#fvr-iv-s1-prop-6 .statement tag=08BT}

*设$\mathbf{f}$和$\mathbf{g}$是在$I \times H$、满足上定义的两个函数，IV、p. 165的引理 1的假设，并且在$I \times H$上，
$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leq \alpha.
$$
(16)

进一步假设 $\mathbf{g}$ 是 $I \times H$ 上常数 $k > 0$ 的 Lipschitz。在这些情况下，如果 $\mathbf{u}$ 是 $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ 的近似解，在 $\varepsilon_1$ 范围内，定义在 $I$ 上，值在 $H$ 中，并且 $\mathbf{v}$ 是 $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ 的近似解范围内$\varepsilon_2$，在$I$上定义，值在$H$中，那么，对于所有$t \in I$
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\alpha + \varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$
(17)

确实
$$
\left\| \mathbf{u}'(t) - \mathbf{g}(t, \mathbf{u}(t)) \right\| \leq \alpha + \varepsilon_1
$$
对于$I$的可数子集的$I$补集中的所有$t$；在其他字中，$\mathbf{u}$是$\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$的近似解，且在$\alpha + \varepsilon_1$之内，因此不等式(17)遵循应用支柱。 5 个IV、p. 169。

### 5. Lipschitz 方程和局部 Lipschitz 方程的存在性以及解的唯一性

#### 定理 1（柯西）{#fvr-iv-s1-thm-1 .statement tag=08BU}

*设$\mathbf{f}$为$I \times H$上的Lipschitz函数，设J为$I$的紧子区间，不简化为J的单个点，$t_0$点，S为一个开球，包含中心$\mathbf{x}_0$和半径r，包含在H中，M是$J \times S$上$\| \mathbf{f}(t, \mathbf{x}) \|$的最小上界。在这些情况下，对于每个不约化到单个点且包含在 J 的交中且具有 $]t_0 - r/M, t_0 + r/M[$ 和包含 $t_0$ 的紧凑区间 K，存在且仅有一个在 K 上定义的微分方程 $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ 的解，其中S 中的值，等于点 $t_0$ 处的 $\mathbf{x}_0$。

事实上，对于足够小的$\varepsilon > 0$，(1)的近似解到$\varepsilon$之内的集合$F_\varepsilon$，在K上定义，值在S中，并且等于点$t_0$处的$\mathbf{x}_0$，不为空（IV，p. 166，道具 3）；进一步，如果 $\mathbf{u}$ 和 $\mathbf{v}$ 属于到 $F_\varepsilon$ 那么，通过 (15) (IV. p. 170)
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq 2\varepsilon \frac{e^{k|t-t_0|} - 1}{k}
$$

对于所有$t \in K$，所以集合$F_\varepsilon$形式是一个过滤器基$\mathscr{G}$，它在$K$上均匀收敛到连续的函数$w$，等于$x_0$ $t_0$；同样，$w$在$S$中取值，因为，对于$\varepsilon$足够小，函数$u \in F_\varepsilon$在$S$中包含的封闭球中取其值。由于$f(t, u(t))$沿$\mathscr{G}$均匀趋于$K$至$f(t, w(t))$，因此$w$满足IV、p. 165的式（6），因此满足式（1）的解。 解的唯一性紧接在IV、p. 170的不等式（15），其中取$\varepsilon_1 = \varepsilon_2 = 0$和$u(t_0) = v(t_0)$。

我们可以说，在$I \times H$上定义的函数$f$是局部Lipschitz，如果对于$I \times H$的每个点$(t, x)$，存在$t$的邻域$V$（相对于$I$）并且$x$ 的邻域 $S$，使得 $f$ 是 $V \times S$ 上的 Lipschitz（常数 $k$ 取决于 $V$ 和 $S$）。根据 Borel-Lebesgue 定理，对于每个紧凑区间 $J \subset I$ 和每个点 $x_0 \in H$，都存在一个开球 $S$ 和中心 $x_0$，包含在 $H$ 中，使得 $f$ 是 Lipschitz $J \times S$；因此$f$满足IV、p. 3的假设引理 1。当$f$是$I \times H$上的局部Lipschitz时，我们可以说方程$x' = f(t, x)$是$I \times H$上的局部Lipschitz。

我们将概括并澄清这一点。 1 of IV, p. 10 对于局部 Lipschitz 方程；我们将自己限制在$t_0$是区间$I$的左端点的情况；人们可以很容易地过渡到$t_0$是$I$的任意点的情况（cf.IV，§IV??，p. 9，推论）。

#### 定理 2 {#fvr-iv-s1-thm-2 .statement tag=08BV}

*令$I \subset \mathbf{R}$为一个区间（不减少为单个点），左端点为$t_0 \in I$，令$H$为非空在$E$中开集合，以及$f$在$I \times H$上的本地Lipschitz 函数。*

$1^\circ$ *对于$x_0 \in H$，存在最大的区间$J \subset I$，左侧端点$t_0 \in J$，其上存在方程$x' = f(t, x)$的积分$u$，在$H$中取值，并在点处等于$x_0$ $t_0$；这个积分是唯一的。*

$2^\circ$ *如果$J \neq I$则$J$是有限长度的半开区间$[t_0, \beta[$；此外，对于每个紧凑子集 $K \subset H$ 集合 $\overline{u}(K)$ 都是$\mathbf{R}$ 的紧凑子集。*

$3^\circ$ *如果$J$有界，且$f(t, u(t))$有界于$J$，则$u(t)$在$J$的右端点有左极限$c$；此外，如果$J \neq I$，则$c$是$E$中$H$的边界点。*

$1^\circ$令$\mathfrak{M}$为间隔$L$的集合（不减少为单个点），其左端点$t_0 \in L$包含在$I$中，并且使得在$L$上有(1)的解 (IV, p. 163)，值在$H$，等于$x_0$在$t_0$；到了。 1 (IV, p. 171) 集合 $\mathfrak{M}$ 不为空。令$L$和$L'$为两个区间属于到$\mathfrak{M}$，并假设对于例，$L \subset L'$；如果$u$和$v$是分别在$L$和$L'$定义的(1)的两个积分，值在$H$，并且在$t_0$等于$x_0$，我们将看到$v$是扩张共 $u$。事实上，令 $t_1$ 为 $t \in L$ 的集合的上确界，使得 $u(s) = v(s)$ 对于 $t_0 \leq s \leq t$；我们将证明$t_1$是$L$的右侧端点。如果不是这样，我们将通过连续性得到$u(t_1) = v(t_1)$，并且$x_1 = u(t_1)$将属于到$H$；由于 $f$ 是本地 Lipschitz，th。由图1可知，在$t_1$的邻域上定义的(1)整的，在$H$中值且在$t_1$中等于$x_1$；因此，假设$t_1$不是$L$的右侧端点是矛盾的。现在我们看到，如果 $J$ 是区间 $L \in \mathfrak{M}$ 的并，则存在且仅有一个 (1) 的积分 $u$，定义在 $J$ 上，值在 $H$ 中，并且等于 $x_0$ 在 $t_0$ 中。

2）假设J≠I，设β为J的右端点；如果 β 是 I 的右侧端点，则 β ∈ I （因此 β 是有限的）且 J = [t_0, β[ by 假设。假设 β 不是 I 的右侧端点；如果 β ∈ J 则 u(β) = c 属于至 H；到了。 1 在 H 中存在 (1) 与值的积分，定义在区间上

$$ [\beta, \beta_1[ \subset I $$

且等于 β 处的 c；那么 J 就不会是 $\mathfrak{M}$ 中的区间的最大的，这是荒谬的；所以 J = [t_0, β[.

如果 K 是 H 的紧致子集，则 $\bar{u}^{-1}(K)$ 在 J 中是闭的；我们将看到，存在 γ ∈ J 使得 $\bar{u}^{-1}(K)$ 包含在 [t_0, γ ] 中，这将证明 $\bar{u}^{-1}(K)$ 是紧的。如果不是，则存在点 c ∈ K，使得 (β, c) 是点 (t, u(t)) 的集合的簇点，使得 t < β 且 u(t) ∈ K。由于 β ∈ I 且 c ∈ H，因此存在邻域 I 中 β 的V，以及 H 中包含中心 c 和半径 r 的开球 S，使得 f 为 Lipschitz，且以 V × S 为界；令 M 为 $\|f(t, x)\|$ 在集合上的上界。到假设时，存在 t_1 ∈ J 使得 $\beta - t_1 < r/2M$、$t_1 \in V$ 和 $\|u(t_1) - c\| \leq r/2$； th。图 1 显示存在且仅有一个 (1) 的积分，其中 H 中的值定义在区间 [t_1, t_2] 包含于 β 上，且在 t_1 处等于 u(t_1)；由于这个区间重合与 u 在区间 [t_1, β[ 上，因此 J = [t_0, β[ 不是 $\mathfrak{M}$ 中的最大的区间，这是荒谬的。

3 假设 J 有界且 $\|f(t, u(t))\| \leq M$ 在 J 上；然后 $\|u'(t)\| \leq M$ 对 J 的可数子集的补集；然后，对于 J 中的任何 s 和 t，通过值定理、$\|u(s) - u(t)\| \leq M |s - t|$ 的平均值；根据柯西准则，u 在 J 的右端点 β 处有一个左极限 c。如果 J ≠ I，则 c 不能属于到 H，因为通过在 β 处连续性扩展 u，u 将是 (1) 与 H 中的值的积分，在区间 [t_0, β] 上定义并等于 x_0 t_0;那么 J = [t_0, β]，与我们在 2 中看到的相矛盾。

#### 推论 1 {#fvr-iv-s1-thm-2-cor-1 .statement tag=08BW}

*如果 H = E 且 J ≠ I，则 f(t, u(t)) 不受 J 限制，进一步，如果 E 是有限维的，则 $\|u(t)\|$ 在 J 的右侧端点留下了极限 $+\infty$。*

第一个部分是第三个部分的直接的推论。 2 如果 E 是有限维的，则每个闭球 S ⊂ E 都是紧致的，因此第 2 个部分 。图 2 表明存在 γ ∈ J 使得 u(t) ∉ S（t > γ）。

如果 E 是有限维的，则可能会出现 J ≠ I，但 $\|u(t)\|$ 仍然有“有界”，因为 t 趋向于 J 的右侧端点（IV，p. 200，练习 5）。

#### 推论 2 {#fvr-iv-s1-thm-2-cor-2 .statement tag=08BX}

*如果，在 I × H 上，函数 f 是关于调节的函数 k(t) 的 Lipschitz，并且如果 J 属于到 I 的右侧端点 β，则 u 在 β 处有一个左极限；如果 H = E 并且 f 是关于 I × E 上受调节的函数 k(t) 的 Lipschitz，则 J = I。*

Indeed, if β ∈ I, there exists a compact neighbourhood V of β in I, such that f(t, x_0) and k(t) are bounded on V; then $\|f(t, x)\| \leq m \|x\| + h$ (m and h constant) on $V \times H$, whence $\|u'(t)\| \leq m \|u(t)\| + h$ on the complement of a countable subset of $V \cap J$, so that $\|u(t)\| \leq m \int_{t_0}^t \|u(s)\|\ ds + q$ ($q$ constant) on $V \cap J$; lemma 2 (IV, p. 170) shows that $\|u(t)\| \leq c\ e^{mt} + d$ ($c$ and $d$ constant) on $V \cap J$, and thus $f(t, u(t))$ remains *bounded* on $J$, and the corollary results from th. 2 of IV, p. 172.

#### 例 1 {#fvr-iv-s1-n5-exa-1 .statement tag=08BY}

对于形式$x' = g(t)$的微分方程，其中$g$受$I$调节，每个积分$u$都在所有$I$上明确定义。人们应该注 $u$ 可以在 $I$ 上有界，而 $g(t)$ 则不然。

#### 例 2 {#fvr-iv-s1-n5-exa-2 .statement tag=08BZ}

对于标量方程$x' = \sqrt{1 - x^2}$，有$I = \mathbf{R},\ H = ] - 1, +1[$。如果在最大的区间包含0上取$t_0 = x_0 = 0$相应的积分为$\sin t$*，其中$\sin t$的导数为正*，即在$] - \pi/2, +\pi/2[$上；在此区间的端点处，积分趋向于 $H$ 的端点。

#### 例 3 {#fvr-iv-s1-n5-exa-3 .statement tag=08C0}

对于标量方程$x' = 1 + x^2$，有$I = H = \mathbf{R}$：在$t = 0$处消失的积分为$\tan t$，而最大的区间包含 0（其中函数连续）为$J = ] - \pi/2, +\pi/2[$；并且 $|\tan t|$ 在 $J$ 的端点处趋于 $+\infty$（*cf.* IV、p. 173，cor. 1）。

#### 例 4 {#fvr-iv-s1-n5-exa-4 .statement tag=08C1}

对于标量方程 $x' = \sin tx$ ，有 $I = H = \mathbf{R}$ 并且右侧以 $I \times H$ 为界，因此 (IV, p. 173, cor. 1) 每个积分都在所有 $\mathbf{R}$ 上定义。

### 6. 参数函数的积分连续性

命题 6 (IV, p. 171) 表明，当微分方程

$$
x' = f(t, x)
$$

与 Lipschitz 方程 $x' = g(t, x)$ “接近”，并且当假设*两个*方程在相同区间上有一个近似值解时，那么这些近似值解是“接近”的；我们将通过证明 Lipschitz 方程 $x' = g(t, x)$ 的解在某个区间上的存在*意味着*在同一区间上存在 $x' = f(t, x)$ 的近似解来澄清这个结果，只要在后者上，$x' = g(t, x)$ 的解的值不是“太接近”的*边界* $H$。

#### 命题 7 {#fvr-iv-s1-prop-7 .statement tag=08C2}

*设$f$和$g$是定义在$I \times H$、满足上的两个函数，即IV的引理1的假设。 p. 165，因此，在 $I \times H$*

$$
\|f(t, x) - g(t, x)\| \leq \alpha .
$$
(16)

*进一步假设$g$是关于$I \times H$上的常数$k > 0$的Lipschitz，并且$f$是$I \times H$上的局部Lipschitz，或者$E$是有限维的。令$(t_0, x_0)$为$I \times H$、$\mu$数$> 0$中的点，并且*

$$
\varphi(t) = \mu\ e^{k(t-t_0)} + \alpha\ \frac{e^{k(t-t_0)} - 1}{k} .
$$

*令$u$为方程$x' = g(t, x)$的积分，定义在$I$包含的区间$K = [t_0, b[$上，等于点$t_0$处的$x_0$，并且对于所有$t \in K$具有中心的闭球$u(t)$，半径$\varphi(t)$包含在$H$中。在这些条件下，对于每个$y \in H$使得$\|y - x_0\| \leq \mu$存在$x' = f(t, x)$的积分$v$，定义在$K$上，值在$H$中，并且等于$y$在点 $t_0$；此外，$\|u(t) - v(t)\| \leq \varphi(t)$于$K$。*

令 $\mathscr{M}$ 为 $x' = f(t, x)$ 的积分族，其中每个积分族在 $H$ 中取其值，在 $t_0$ 处等于 $y$，并在 $I$ 中包含的半开区间 $[t_0, \tau[$ 上定义（取决于所考虑的区间）。到了。 IV、p. 171（当$f$是本地Lipschitz时）或IV、p. 167推论（当$E$是有限维时）中的1，$\mathscr{M}$不为空，与prop中的推理相同。 IV、p. 166 中的 3 表明$\mathscr{M}$ 对于阶是*归纳*“v 是 w 的限制”。设$v_0$为$\mathscr{M}$的极大元素与$[t_0, t_1[$$v_0$的定义的区间；通过道具。 IV、p. 171 中的 6 个，全部归结为证明和 $t_1 \geq b$。如果没有的话，人们就会

$$
\| u(t) - v_0(t) \| \leq \varphi(t)
$$

在区间 $[t_0, t_1[$ 上通过 prop. 6；现在，在紧凑区间 $[t_0, t_1]$ 上，调节的函数 $g(t, u(t))$ 是有界的，因此函数 $g(t, v_0(t))$ 在区间 $[t_0, t_1[$ 上有界，对于该区间上的 $\| g(t, v_0(t)) \| \leq \| g(t, u(t)) \| + k \varphi(t)$ 。由于$v_0$是$x' = g(t, x)$的近似解到$[t_0, t_1[$上的$\alpha$之内，因此存在数$M > 0$，使得在此区间上$\| v_0'(t) \| \leq M$，除了可数集合的点； 值定理现在显示，$[t_0, t_1[$ 的点 $s, t$ 的每个对 $\| v_0(s) - v_0(t) \| \leq M |s - t|$，因此（根据柯西标准）$v_0(t)$ 有一个左极限 $c$ 点 $t_1$，并且，根据连续性，一个人有$\| c - u(t_1) \| \leq \varphi(t_1)$，所以$c \in H$。现在一看，从IV，p. 171，th。 1 或 IV、p. 167，推论，存在定义在区间 $[t_1, t_2[$ 上的$x' = f(t, x)$ 整的，且在 $t_1$ 处等于 $c$，其中与……矛盾定义为 $v_0$。

#### 定理 3 {#fvr-iv-s1-thm-3 .statement tag=08C3}

*设 F 为拓扑空间，并令 f 为从 I × H × F 到 E 的映射，使得对于每个 $\xi \in F$，函数 $(t, x) \mapsto f(t, x, \xi)$ 是 I × H 上的 Lipschitz，并且这样，当 $\xi$ 趋于$\xi_0$、$f(t, x, \xi)$ 在 I × H 上一致趋向于 $f(t, x, \xi_0)$。令 $u_0(t)$ 为 $x' = f(t, x, \xi_0)$ 的积分，定义在I 包含的区间 $J = [t_0, b[$ 上，其中值在 H 中，等于 $x_0$ $t_0$。对于 J 中包含的每个紧凑区间 $[t_0, t_1]$，F 中都存在 $\xi_0$ 的邻域 V，这样，对于每个 $\xi \in V$，方程 $x' = f(t, x, \xi)$ 都有一个定义在 $[t_0, t_1]$ 上的积分（且只有一个）$u(t, \xi)$，其中值在 H 中并且等于$x_0$ $t_0$；此外，当$\xi$趋向于$\xi_0$时，解$u(t, \xi)$在$[t_0, t_1]$上均匀趋于$u_0(t)$。*

事实上，让$r > 0$这样，对于$t_0 \leq t \leq t_1$，具有中心$u_0(t)$和半径$r$的封闭球包含在$H$中；如果$f(t, x, \xi)$是关于$I \times H$上的常数$k > 0$的Lipschitz，我们取$\alpha$足够小，以至于$\alpha \frac{e^{k(t_1-t_0)} - 1}{k} < r$；取$V$，使得对于每一个$\xi \in V$，一个人在$I \times H$上有$\| f(t, x, \xi) - f(t, x, \xi_0) \| \leq \alpha$，一个人可以应用道具。 7 个IV、p. 174；此外，

$$
\| u(t, \xi) - u_0(t) \| \leq \alpha \frac{e^{k(t_1-t_0)} - 1}{k}
$$

在 $[t_0, t_1]$ 上，完成定理中的证明。

#### 注 {#fvr-iv-s1-n6-rem-1 .statement tag=08C4}

当IV的$H = E$和条件(16)时，p. 174满足$I \times E$，道具。 7 of IV、p. 174 适用于定义此解的*任何*间隔上 $x' = g(t, x)$ 的*每个* 解 $u$；人们甚至可以假设 $g(t, x)$ 是 Lipschitz 相对于受管制的函数 $k(t)$ 虽然不一定受此区间限制。

### 7. 对初始条件的依赖

令$x' = f(t, x)$为$I \times H$上的局部Lipschitz方程；到了。 2（IV，p. 172），对于$I \times H$的每个点$(t_0, x_0)$，都存在一个*最大的区间*$J(t_0, x_0) \subset I$，不会减少到单个点，包含于$t_0$，并且其上存在一个该方程的积分（且只有一个），等于 $x_0$ 在 $t_0$ 处；我们将阐明该积分以及定义它的区间$J(t_0, x_0)$依赖于点$(t_0, x_0)$的方式。

#### 定理 4 {#fvr-iv-s1-thm-4 .statement tag=08C5}

*设$f$是$I \times H$和$(a, b)$上的本地Lipschitz函数，$I \times H$的任意点。*

1 *$I$中存在$K \subset I$、$a$的邻域，$H$中存在$b$的邻域$V$，这样，对于每个点$(t_0, x_0)$ $K \times V$，存在一个积分（并且只有一个）$u(t, t_0, x_0)$定义在$K$上，值在$H$中并且等于$x_0$在点$t_0$（在其他字，$J(t_0, x_0) \supset K$对于所有$(t_0, x_0) \in K \times V$).*

2 *$K \times K \times V$到$H$的映射$(t, t_0, x_0) \mapsto u(t, t_0, x_0)$是均匀连续的。*

3 *$H$中存在$b$的邻域$W \subset V$，使得对于每个点*
$$
(t, t_0, x_0) \in K \times K \times W,
$$
*方程 $x_0 = u(t_0, t, x)$ 在 $V$ 上有一个唯一的解 $x$，等于 $u(t, t_0, x_0)$*（“积分相对于积分常数的分辨率”）。

1 令$S$为一个球，其中心$b$和半径$r$包含在$H$中，$J_0$包含在$I$中$I$、$a$的邻域中，使得$f$有界且Lipschitz（相对于某个常数 $k$）在 $J_0 \times S$ 上；用$M$表示$\|f(t, x)\|$在$J_0 \times S$上的上界。那么$I$中存在(IV, p. 171, th.1) $a$的区间$J \subset J_0$、邻域，以及$J$上定义的$x' = f(t, x)$的积分$v$，其中值 $S$ 且在 $a$ 处等于 $b$。我们将看到开球$V$与中心$b$和半径$r/2$，以及$J$的交$K$间隔$]a - l, a + l[$，其中$l$*足够小*，符合要求。确实，道具。 IV、p. 174 的 7（应用于集合 $J_0 \times S$ 和$\alpha = 0$ 的情况）表明存在$x' = f(t, x)$ *定义在* $K$ 上的积分，其中值在$S$ 中，并且等于$x_0$ 点 $t_0 \in K$，前提是
$$
\|v(t) - b\| + \|v(t_0) - x_0\| e^{k|t-t_0|} < r
$$
每$t \in K$。现在，平均值定理，一个人有
$$
\|v(t) - b\| \leq M |t - a| \leq Ml
$$
每$t \in K$；因为 $\|x_0 - b\| < r/2$ 人们认为取 $l$ 就足够了
$$
Ml + (Ml + r/2)e^{2kl} < r
$$
或关系 (18) 满足$(t, t_0, x_0)$/$K \times K \times V$。

2) 平均而言值定理我们有

$$
\| \mathbf{u}(t_1, t_0, \mathbf{x}_0) - \mathbf{u}(t_2, t_0, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

(20)

对于 K 中的所有 $t_0, t_1, t_2$ 和 V 中的 $\mathbf{x}_0$。现在支持。 5 (IV, p. 169) 表明

$$
\| \mathbf{u}(t, t_0, \mathbf{x}_1) - \mathbf{u}(t, t_0, \mathbf{x}_2) \| \leq e^{2kt} \ \| \mathbf{x}_2 - \mathbf{x}_1 \|
$$

(21)

对于 K 中的每个 $t$ 和 $t_0$，以及 V 中的 $\mathbf{x}_1$ 和 $\mathbf{x}_2$。最后，如果$t_1$和$t_2$是K中任意两个点，

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{u}(t_2, t_2, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

平均而言值定理，也就是说

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t_2 - t_1| ;
$$

因为$\mathbf{u}(t, t_2, \mathbf{x}_0)$与值$\mathbf{u}(t_1, t_2, \mathbf{x}_0)$在点$t_1$处的积分相同，道具。 5 (IV, p. 169) 表明

$$
\| \mathbf{u}(t, t_1, \mathbf{x}_0) - \mathbf{u}(t, t_2, \mathbf{x}_0) \| \leq Me^{2kl} |t_2 - t_1|
$$

(22)

对于 K 中的所有 $t, t_1, t_2$ 和 V 中的 $\mathbf{x}_0$。三个不等式(20)、(21)和(22)由此证明了映射$(t, t_0, \mathbf{x}_0) \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$在$K \times K \times V$上的一致连续性。

3 到 (20)，我们有 $\| \mathbf{u}(t, t_0, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t - t_0| \leq 2Ml$

$$
K \times K \times V.
$$

如果$l$取得足够小，使得$2Ml < r/4$，则可以看出，如果$\mathbf{x}_0$是具有中心$\mathbf{b}$且半径为$r/4$的开球W的任何点，则$\mathbf{u}(t, t_0, \mathbf{x}_0) \in V$对于任何$t$和K 中的$t_0$。若$\mathbf{x} = \mathbf{u}(t, t_0, \mathbf{x}_0)$，则函数$s \mapsto \mathbf{u}(s, t, \mathbf{x})$定义在K上，等于(1)的积分，在点$t$取值$\mathbf{x}$，即到$\mathbf{u}(s, t_0, \mathbf{x}_0)$；特别是

$$
\mathbf{x}_0 = \mathbf{u}(t_0, t_0, \mathbf{x}_0) = \mathbf{u}(t_0, t, \mathbf{x}).
$$

此外，如果$y \in V$使得$\mathbf{x}_0 = \mathbf{u}(t_0, t, y)$，那么积分$s \mapsto \mathbf{u}(s, t, y)$在$t_0$处取值$\mathbf{x}_0$，因此与$s \mapsto \mathbf{u}(s, t_0, \mathbf{x}_0)$相同，因此在$t$处取值$\mathbf{x}$，这表明$y = \mathbf{x}$ 和结论证明。

### 习题 {#fvr-iv-s1-exercises}

请参阅[习题了解§ 1](exercises/s1/)。
