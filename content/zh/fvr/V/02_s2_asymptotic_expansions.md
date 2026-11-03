---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 2
section_title: ASYMPTOTIC EXPANSIONS
lang: zh
source: fvr-i-vii
book_pages: 220-227
pdf_pages: 0235-0242
extraction: ocr
subsections:
    - "no": 1
      title: SCALES OF COMPARISON
      page: 220
      pdf_page: 235
    - "no": 2
      title: PRINCIPAL PARTS AND ASYMPTOTIC EXPANSIONS
      page: 221
      pdf_page: 236
    - "no": 3
      title: SUMS AND PRODUCTS OF ASYMPTOTIC EXPANSIONS
      page: 223
      pdf_page: 238
    - "no": 4
      title: COMPOSITION OF ASYMPTOTIC EXPANSIONS
      page: 224
      pdf_page: 239
    - "no": 5
      title: ASYMPTOTIC EXPANSIONS WITH VARIABLE COEFFICIENTS
      page: 226
      pdf_page: 241
statements: 12
exercises: 0
content_sha256: 1083cac88b4c22ed94b51c2779ef0379f5cd2b78c8ee2fc0080d62a343e4b1d3
translated_from: content/en/fvr/V/02_s2_asymptotic_expansions.md
translation_method: google
source_content_sha256: 3913fa9ae08c74aef17f721c054e1ae91ca2d4d4ef6bc764fb678147ac681601
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 812815bfe82fc3431d899d96e3c384cf6afa415c731b3dd4844d0714bb357308
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。渐近展开

### 1. 比较尺度

令 E 为集合，由具有基 $\mathfrak{F}$ 的过滤器过滤，K 为非离散值域（最常见的是 $K = \mathbf{R}$ 或 $K = \mathbf{C}$）。 $\mathscr{H}(\mathfrak{F}, K)$中函数的集合不等于0模$R_\infty$（即，$\mathfrak{F}$中的每个集合中至少有一个点，其中函数不消失），关系“ $f \ll g$或$f = g$”是序关系。

#### 定义 1 {#fvr-v-s2-def-1 .statement tag=08ES}

*有人说，函数不等于0模$R_\infty$形成的$\mathscr{H}(\mathfrak{F}, K)$的子集$\mathscr{E}$是当$\mathscr{E}$由关系“$f \ll g$或$f = g$”全序时的比较尺度。*

在其他字中，如果$\mathscr{E}$中$f$和$g$是函数，则关系、$f \ll g$、$g \ll f$、$f = g$中的一个（且只有一个）始终成立。因此，在 $\mathscr{E}$ *关系* $f \asymp g$（和 *更不必说* $|f| \sim a\,|g|$，其中 $a$ 是数 $> 0$）*意味着* $f = g$。

比较量表的每个子集显然也是比较量表。

#### 例 1 {#fvr-v-s2-n1-exa-1 .statement tag=08ET}

对于$x$真实且趋于函数$x^\alpha$（$\alpha$任意实数）的$+\infty$集合是一个比较尺度。当$\mathfrak{F}$是左端点为$a$的开区间的集合时，函数$(x-a)^\alpha$也是如此。

#### 例 2 {#fvr-v-s2-n1-exa-2 .statement tag=08EU}

对于$z$复数趋于函数$z^n$的$\infty$集合（$n$一个有理整数）是一个比较尺度；当$\mathfrak{F}$是该点的邻域的过滤器的点$a \in \mathbf{C}$的补集时，函数$(z-a)^n$也是如此。

#### 例 3 {#fvr-v-s2-n1-exa-3 .statement tag=08EV}

设 F 为空间； 函数$\|x-\mathbf{a}\|^\alpha$（$\alpha$任意实数）族是当$\mathfrak{F}$是该点的邻域滤波器的$\mathbf{a}$补线上的迹时的比较尺度。请注意，如果$p$和$q$是F上的两个不同的范数，则两个比较尺度$(p(x-\mathbf{a}))^\alpha$和$(q(x-\mathbf{a}))^\alpha$的并通常不是比较尺度。

#### 例 4 {#fvr-v-s2-n1-exa-4 .statement tag=08EW}

对于趋向于 $+\infty$ 形式 $\exp(p(x))$ 函数的$\mathscr{E}$族$x$实数，其中$p$贯穿没有常数项*的*多项式的集合（具有实数系数），是一个比较尺度：只要注意到$\mathscr{E}$中的两个函数中的商再次在$\mathscr{E}$中，并且如果$p \neq 0$，函数$\exp(p(x))$必须趋向于0或$+\infty$；事实上，$p(x) \sim \alpha x^n$，其中$n > 0$和$\alpha \neq 0$；如果$\alpha > 0$则$p(x) > \frac{1}{2} \alpha x^n$对于$x$足够大；如果$\alpha < 0$则$p(x) < \frac{1}{2} \alpha x^n$对于$x$足够大；在第一种情况下，$\exp(p(x))$趋于$+\infty$，在第二种情况下趋于0。

#### 例 5 {#fvr-v-s2-n1-exa-5 .statement tag=08EX}

对于形式$x^\alpha (\log x)^\beta$的函数的$x$实数趋于$+\infty$集合$\mathscr{E}$（为$x > 1$定义），其中$\alpha$和$\beta$是任意实数，是比较量表。事实上，在这里，$\mathscr{E}$中的两个函数中的商又是$\mathscr{E}$中的函数；足以证明，如果$\alpha$和$\beta$不都是零，则$x^\alpha (\log x)^\beta$趋于0或$+\infty$；如果$\alpha = 0, \beta \neq 0$，这很清楚；如果 $\alpha > 0$ 一个有 $(\log x)^{-\beta} \ll x^\alpha$，并且如果 $\alpha < 0$ 一个有 $(\log x)^\beta \ll x^{-\alpha}$，对于任何 $\beta$、从而命题。

请注意，最后一个比较比例为全序集（对于关系“f $\ll$ g”或$f = g$”），其阶结构同构于 $\mathbf{R}^2$ (*集合) 上的 *字典* 阶理论*、III、p. 157）；回想一下，在此结构关系$(\alpha, \beta) < (\gamma, \delta)$表示“$\alpha < \gamma$，或$\alpha = \gamma$和$\beta < \delta$”）。

类似地，由函数 $\exp(p(x))$ 形成的标度，其中 $p$ 穿过没有常数项的多项式的集合 $P_0$，阶结构同构于阶结构 $P_0$，其中关系 $p < q$ 意味着多项式 $q - p$ 的主导项有系数 $> 0$ (*cf. Alg.*, VI.19, *例 2*）。

令$\varphi$为从集合F到E的映射，使得$\varphi^{-1}(\mathfrak{F})$是F上的过滤器基。如果$\mathscr{E}$是E上的比较尺度（对于过滤器基$\mathfrak{F}$）则函数$f \circ \varphi$，如$f$ 贯穿$\mathscr{E}$、形式 F 上的比较尺度（对于过滤器基 $\varphi^{-1}(\mathfrak{F})$）。

### 2. 本金部分和渐近展开

令$\mathscr{E}$为非离散值域 K中由函数与值形成的比较尺度。令V为K上的标准化空间，令$\mathbf{f}$为$\mathscr{H}(\mathfrak{F}, V)$中的函数；如果V中有函数$g \in \mathscr{E}$和元素$\mathbf{a} \neq 0$使得$\mathbf{f} \sim \mathbf{a}g$，则可以说$\mathbf{a}g$是$\mathbf{f}$相对于规模$\mathscr{E}$的*主部分*。从定义。 V、p. 10、$\mathbf{f}$ 中的 1 个相对于 $\mathscr{E}$ 只能有一个主体部分，因为如果$g_1,\ g_2$ 是$\mathscr{E}$ 中的两个函数，并且$\mathbf{a}_1,\ \mathbf{a}_2$ 是两个$\neq 0$ V的元素，则关系$\mathbf{a}_1 g_1 \sim \mathbf{a}_2 g_2$蕴含$|g_1| \asymp |g_2|$，因而$g_1 = g_2$，从而$(\mathbf{a}_2 - \mathbf{a}_1)g_1 \ll g_1$，并且由于$g_1$与零在任何集合上不相同$\mathscr{E}$ 这意味着$\mathbf{a}_2 = \mathbf{a}_1$。

如果$\mathbf{f}$相对于比较尺度$\mathscr{E}$具有主体部分，则相对于每个比较尺度$\mathscr{E}' \supset \mathscr{E}$，它具有*相同的主体部分。

#### 例 1 {#fvr-v-s2-n2-exa-1 .statement tag=08EY}

对于$x$实数（或复数）趋向于$+\infty$（或$\infty$），每个多项式$a_0 x^n + a_1 x^{n-1} + \ldots + a_n$，其中系数位于V，使得$a_0 \neq 0$，相对于标度具有主部分$a_0 x^n$ $x^n$（或任何包含 $x^n$）。由此可见，每个有理分数 $\frac{a_0 x^n + \cdots + a_m}{b_0 x^n + \cdots + b_n}$ 与实数或复数系数使得 $a_0 b_0 \neq 0$ 对于相同的标度具有主部分 $\frac{a_0}{b_0} x^n$。

#### 例 2 {#fvr-v-s2-n2-exa-2 .statement tag=08EZ}

函数可以与某个量表的所有函数进行比较，但不承认该量表的主要部分。例如，对于趋向于$+\infty$的$x$实数，$\sqrt{x}$相对于标度$x^n$没有本金部分，其中$n$是有理数整数； $\log x$相对于$x^\alpha$的规模没有本金部分（$\alpha$任意实数）； $\exp(\sqrt{\log x})$ 和 $x' = e^{x \log x}$ 相对于 $x^\alpha (\log x)^\beta$ 的标度没有主部分，也相对于 $\exp(p(x))$ 的标度（$p$ 没有常数项的多项式）。

本金部分的概念承认广泛的推广。假设函数$f \in \mathscr{H}(\mathfrak{F}, V)$相对于规模$\mathscr{E}$有一个本金部分$a_1 g_1$； 关系 $f \sim a_1 g_1$ 相当于$f - a_1 g_1 \ll g_1$（V，p. 216，def. 4）；为了更仔细地研究函数$f$，我们会考虑函数$f - a_1 g_1$。如果这个函数相对于$\mathscr{E}$有一个本金部分$a_2 g_2$，则必须有$g_2 \ll g_1$和$f - a_1 g_1 - a_2 g_2 \ll g_2$。

更一般地，假设标度$\mathscr{E}$以参数方式写成形式$(g_\alpha)$，其中$\alpha$贯穿指标$A$的集合，赋予全序结构同构于阶的*相反* $\mathscr{E}$的结构：关系$\alpha < \beta$因此相当于$g_\beta \ll g_\alpha$。在这些情况下：

#### 定义 2 {#fvr-v-s2-def-2 .statement tag=08F0}

*有人说函数* $f \in \mathscr{H}(\mathfrak{F}, V)$ *承认渐近展开精确* $g_\alpha$ *（相对于尺度* $\mathscr{E}$*） *如果存在一个族* $(a_\lambda)_{\lambda \leq \alpha}$ *元素的* $V$，*除有限之外其中数是*$0$，*使得*$f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$。 *有人说*$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$*是*$f$*精确到*$g_\alpha$的渐近展开，**$a_\lambda g_\lambda$（$\lambda \leq \alpha$）*是它的项，*$a_\lambda$*它的系数，并且函数* $r_\alpha = f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ *剩余的展开*。

为了表达这样一个事实：$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$是$f$的渐近展开，精确到$g_\alpha$，这是自己最常写的限制

$$
f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o(g_\alpha) \quad \text{(or } f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o_k(g_\alpha)
$$

如果证明中有几个函数），其后面是V、p. 219和220的记号。

在相对于相同尺度 $\mathscr{E}$ 的两个渐近展开（两个函数，无论是否不同）中，有人说精度大于指标的那个是“更精确”。

如果 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ 是 $f$ 到精度 $g_\alpha$ 的渐近展开，则对于每个 $\beta < \alpha$，$\sum_{\lambda \leq \beta} a_\lambda g_\lambda$ 是 $f$ 到精度 $g_\beta$ 的渐近展开 (V， p. 215，道具 5)：有人说它是通过将给定的 $f$ 展开 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ 的精度降低到 $g_\beta$ 来获得的。

如果 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ 和 $\sum_{\lambda \leq \alpha} b_\lambda g_\lambda$ 渐近展开到两个函数 $f_1, f_2$ 的*相同*精度 $g_\alpha$，则 $\sum_{\lambda \leq \alpha} (a_\lambda + b_\lambda) g_\lambda$ 是 $f_1 + f_2$ 到精度 $g_\alpha$ 的渐近展开 （V，p. 215，第 5 条）；对于每个标量 $c$，$\sum_{\lambda \leq \alpha} a_\lambda c g_\lambda$ 是 $f_1 c$ 到精度 $g_\alpha$ 的渐近展开。由此可见，如果函数承认渐近展开达到精度 $g_\alpha$，那么这个展开是*唯一的*：足以看出函数 0 不承认渐近展开具有系数的精度 $g_\alpha$ $\neq 0$。因为，如果 $0 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$ 和 $\gamma$ 是指标 $\lambda \leq \alpha$ 中最小的一个，使得$a_\lambda \neq 0$，那么就会有$a_\gamma g_\gamma = - \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda - r_\alpha \ll g_\gamma$，这是荒谬的。

说函数 $f$ 承认渐近展开到精度 $g_\alpha$，其所有系数都是 *零*，相当于说和 $f \ll g_\alpha$。如果 $f$ 承认渐进展开 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ 达到精度 $g_\alpha$，且系数不全为零，并且如果 $\gamma$ 是指标 $\lambda$ 的最小的，使得$a_\lambda \neq 0$，则$a_\gamma g_\gamma$是$f$相对于尺度$\mathscr{E}$的*本数部分*，因为一个人有$f - a_\gamma g_\gamma = \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha \ll g_\gamma$；类似地，如果 $\mu \leq \alpha$ 是指标，使得 $a_\mu \neq 0$，则 $a_\mu g_\mu$ 是 $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$ 的主部分。

应用中最重要的渐近展开是那些相对于$x^{-n}$（分别是$z^{-n}$）的标度，其中$n$是正或负整数，因为$x$趋于$+\infty$或$-\infty$（分别当复数 $z$ 趋向于 $\infty$），或者当实数 $x$ 从右或向左趋于 $c$ 时（分别当复数时），或相对于 $(x - c)^n$（或$(z - c)^n$）的比例$z$趋于$c$）。我们在I、p. 21中看到，实变量$x$的每个向量函数在点$c \in \mathbf{R}$可微分$k$倍，承认阶的泰勒展开 $k$ 在此点，即相对于 $(x - c)^n$ 的标度，渐近展开到精度 $(x - c)^k$。

### 3. 渐近展开的和和乘积

如果$f_1, f_2$允许渐近展开分别达到精度$g_\alpha$和$g_\beta$，相对于比较尺度$\mathscr{E}$，通过将两个展开*限制*到该精度，可以将展开推导到精度$g_{\min(\alpha, \beta)}$；我们已经在 V、p. 222 中看到了如何获得 $f_1 + f_2$ 到精度 $g_{\min(\alpha, \beta)}$ 的渐近展开。

令$V_1, V_2$和$V$为域$K$上的三范数空间，并令$(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}. \mathbf{y}]$为从$V_1 \times V_2$到$V$的*连续双线性映射*；我们进一步假设，对于这个截面的其余部分，$\mathscr{E}$的比例是这样的，$\mathscr{E}$中任何两个函数的*乘积*再次在$\mathscr{E}$中（对于所有给出的例比较比例（在V中， p. 220））。

现在让$f_1, f_2$分别是$\mathscr{H}(\mathfrak{F}, V_1)$和$\mathscr{H}(\mathfrak{F}, V_2)$中的两个函数，相对于标度$\mathscr{E}$，分别具有渐近展开、$f_1 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$和$f_2 = \sum_{\mu \leq \beta} b_\mu g_\mu + r_\beta$的精度$g_\alpha$和$g_\beta$。进一步假设$a_\lambda$和$b_\mu$都不全是零，并令$a_\gamma g_\gamma$和$b_\delta g_\delta$作为$f_1$和$f_2$的主部分。到假设，可以写出$g_\gamma g_\beta = g_\rho$和$g_\delta g_\alpha = g_\sigma$；让我们证明，和$\sum [\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$接管了所有对$(\lambda, \mu)$，使得$g_{\min(\rho, \sigma)} \ll g_\lambda g_\mu$是*$[f_1.f_2]$*精确*$g_{\min(\rho, \sigma)}$的*渐近展开。现在$[f_1.f_2]$和这个和之间的差异是项的有限数的和，每个形式$[\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$和$g_\lambda g_\mu \ll g_{\min(\rho, \sigma)}$，或者形式$[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda$其中$\lambda \geq \gamma$，或形式$[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu$，其中$\mu \geq \delta$；但由于 $[\mathbf{x}. \mathbf{y}]$ 是连续的，因此可以从 (V, p. 213, 命题 3 和 V, p. 215, 命题 6) 得到$[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda \preccurlyeq \mathbf{r}_\beta g_\lambda \ll g_\beta g_\gamma = g_\rho$ $\lambda \geq \gamma$，类似地$[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu \preccurlyeq \mathbf{r}_\alpha g_\mu \ll g_\alpha g_\delta = g_\sigma$ $\mu \geq \delta$， 从而命题（V，p. 215，道具 5）。

如果所有$\mathbf{a}_\lambda$都是零，其中一个有$[f_1.f_2] \ll g_\alpha g_\delta$：在其他字中，一个有$[f_1.f_2]$的渐近展开，其中零项，精确到$g_\alpha g_\delta$；类似地，如果所有 $\mathbf{a}_\lambda$ 和 $\mathbf{b}_\mu$ 都是零，则其中一个具有 $[f_1.f_2]$ 的渐近展开，其中零项的精度为 $g_\alpha g_\beta$。

我们主要将前面的结果应用到V是K上的*范数代数*并且双线性函数$[\mathbf{x}. \mathbf{y}]$是这个代数中的乘积xy；最重要的情况是V等于$\mathbf{R}$或$\mathbf{C}$。

特别是，如果 $f_i$ ($1 \leq i \leq n$) 是 $\mathscr{H}(\mathfrak{F}, K)$ 中的 n 个函数，其中每个函数都允许关于 $\mathscr{E}$ 的渐近展开式，则对于 $f_i$ 中的每个*多项式* $\sum_{(v_i)} \mathbf{a}_{v_1 v_2} v_n f_1^{v_1} \ldots f_n^{v_n}$，系数在赋范空间 V 中，可以获得关于 $\mathscr{E}$ 的渐近展开式；此外，如果知道函数$f_i$的展开式，则前面的规则允许我们确定所获得的展开式的精度。

### 4. 渐近展开的合成

令$f$在$\mathscr{H}(\mathfrak{F}, \mathbf{R})$（或$\mathscr{H}(\mathfrak{F}, \mathbf{C})$）中为函数，相对于尺度$\mathscr{E}$，承认渐进展开达到精度$g_\alpha$，并且*沿着具有基$\widetilde{\mathfrak{F}}$的滤波器具有极限* 0。 另一方面，令$\mathbf{h}$为一个函数，其值位于$\mathbf{R}$（或$\mathbf{C}$）上的赋范空间V中，定义在$\mathbf{R}$（或$\mathbf{C}$）中点0的邻域上，并且在该邻域上*n次可微*；然后

$$
\mathbf{h}(t) = c_0 + c_1 t + \cdots + c_n t^n + o(t^n)
$$

在这个邻域（I，p. 21），从而，在$\widetilde{\mathfrak{F}}$合适的集合上

$$
\mathbf{h} \circ f = c_0 + c_1 f + \cdots + c_n f^n + o(f^n).
$$

我们已经看到，在 n 3 中，如何将 $c_0 + c_1 f + \cdots + c_n f^n$ 的形式渐近展开达到由展开的 $f$ 精度确定的精度 $g_\rho$；另外，假设$f$的渐近展开的系数不全是零，并且$a_\gamma g_\gamma$是$f$的主部分，令$g_\sigma = g_\gamma^n$；如果 $\sigma < \rho$ 将 $\mathbf{h} \circ f$ 的展开限制为$g_\sigma$ 精度，并将 $\sum_{k=0}^n c_k f^k$ 的展开限制为该精度；相反，如果$\rho \leq \sigma$，则$\sum_{k=0}^n c_k f^k$的展开也是$\mathbf{h} \circ f$的展开，精确到$g_\rho$。

如果$f$的渐近展开的所有项都是零，并且如果$g_\alpha \ll 1$，那么对于每个整数$k > 0$，$f \ll g_\alpha$等等$f^k \ll g_\alpha^k \ll g_\alpha$；如果$c_m$是指标$> 0$的第一个系数，且不是零（假设指标$k > 0$的$c_k$不全为0），那么$c_0$是展开的渐近$h \circ f$ 精确到$g_\alpha^m$。

在这个截面的其余部分中，我们将限制自己的情况，即$\mathscr{E}$中的函数具有实数值，并且在$\mathfrak{F}$中的集合上严格为正，并且我们将仅考虑$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的函数的渐近展开。首先假设对于每个函数$g \in \mathscr{E}$和每个实数$\nu$、$g^\nu$再次属于到$\mathscr{E}$：这个条件是满足的，例如，通过$x^\alpha$的规模或通过$x^\alpha |\log x|^\beta$的规模（$\alpha$和$\beta$是任意实数）在$+\infty$的邻域或$\mathbf{R}$中的0的邻域。这个性质意味着$\mathscr{E}$中的两个函数又是属于到$\mathscr{E}$中的商。正因如此，从函数$f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$相对于$\mathscr{E}$的渐近展开，到精度$g_\alpha$，对于每个实数$\nu$，可以推导出$|f|^\nu$的展开。让我们限制一下$f$的展开的系数不都是零的情况，并让$a_\gamma g_\gamma$作为$f$的主要部分；可以写 $|f|^\nu = |a_\gamma|^\nu g_\gamma^\nu (1 + h)^\nu$，其中
$$
h = \sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} + o \left( \frac{g_\alpha}{g_\gamma} \right).
$$
根据我们的假设，$\sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma}$是$h$的渐近展开，精确到$g_\alpha / g_\gamma$；由于上述$h$沿着$\mathfrak{F}$方法趋向于0，给出$(1 + h)^\nu$的渐近展开，然后乘以$|a_\gamma|^\nu g_\gamma^\nu$，$|f|^\nu$的展开。

右 $f$ 进行同样的假设，可以写出
$$
\log |f| = \log |a_\gamma g_\gamma| + \log (1 + h)
$$
并且 $\log (1 + h)$ 可以展开，如上所述，函数 $\log (1 + t)$ 在 0 的邻域上无限可微；此外，如果$\log g_\gamma$承认关于$\mathscr{E}$或关于$\mathscr{E}_1 \supset \mathscr{E}$的渐近展开，则通过将两个渐近展开相加，可以得到$\log |f|$的渐近展开。

#### 例{#fvr-v-s2-n4-exa-1 .statement tag=08F1}

我们有$(1 + x)^{1/x} = \exp \left( \frac{1}{x} \log (1 + x) \right)$：当$x$趋向于$+\infty$时，我们有$\log (1 + x) = \log x + \log \left( 1 + \frac{1}{x} \right)$，从而相对于$x^\alpha (\log x)^\beta$标度的$\frac{1}{x} \log (1 + x)$的渐近展开：
$$
\frac{1}{x} \log (1 + x) = \frac{\log x}{x} + \frac{1}{x^2} - \frac{1}{2x^3} + o_1 \left( \frac{1}{x^3} \right).
$$
来自这个展开，以及来自泰勒展开
$$
e^u = 1 + u + \frac{u^2}{2} + \frac{u^3}{6} + o(u^3)
$$

在$u = 0$的邻域上，推导出渐近展开

$$
(1 + x)^{1/x} = 1 + \frac{\log x}{x} + \frac{1}{2} \frac{(\log x)^2}{x^2} + \frac{1}{x^2}
+ \frac{1}{6} \frac{(\log x)^3}{x^3} + \frac{\log x}{x^3} - \frac{1}{2x^3} + o_2 \left( \frac{1}{x^3} \right)
$$

相对于上面解释的$x^\alpha (\log x)^\beta$乘方法的比例。

保持相同的假设和记号，$e^f$的渐近展开不会构成新的问题，除非$f \gg 1$；然后必须区分两种情况，如$g_\alpha \gg 1$或$g_\alpha \ll 1$。第一种情况，给$f$给出展开，并不能获得$e^f$相对于$\mathscr{E}$的本金部分，因为一般不知道余数$r_\alpha$是否趋于0，即$e^{r_\alpha}$是否趋于1。相反，如果$g_\alpha \ll 1$则$r_\sigma \ll 1$ $e^f \sim \exp \left( \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \right)$。可以使这个结果更加精确：令$a_\gamma g_\gamma$为$f$的主部分，令$\delta$为指标（这样$\gamma < \delta \leq \alpha$），其中$g_\delta = 1$；我们把$f_1 = \sum_{\lambda \leq \delta} a_\lambda g_\lambda$，$f_2 = \sum_{\delta < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$；我们有$f = f_1 + f_2$，所以$e^f = e^{f_1} e^{f_2}$，并且在小节开始时解释的一般方法允许人们形式一个$e^{f_2}$的渐近展开（从$e^t$的泰勒展开开始） 点$t = 0$）。如果 $e^{f_1} = \prod_{\lambda \leq \delta} \exp(a_\lambda g_\lambda)$ 属于到 $\mathscr{E}$，或者到$\mathscr{E}_1$ 包含 $\mathscr{E}$，那么对于 $e^f$ 将会有一个渐近展开。

#### 例 {#fvr-v-s2-n4-exa-2 .statement tag=08F2}

我们有$x^{1/1} = \exp \left( \log x \cdot \exp \left( \frac{1}{x} \log x \right) \right)$；当 $x$ 趋于 $+\infty$ 时，$\log x \ll x$，从而 $\log x \cdot \exp \left( \frac{1}{x} \log x \right)$ 相对于标度 $x^\alpha (\log x)^\beta$ 的渐近展开：

$$
\log x \cdot \exp \left( \frac{1}{x} \log x \right) = \log x + \frac{(\log x)^2}{x} + \frac{1}{2} \frac{(\log x)^3}{x^2} + o \left( \frac{(\log x)^3}{x^2} \right).
$$

这个展开的所有项，从第二个开始，趋于0；由此展开和从$u = 0$的邻域上的泰勒展开$e^u = 1 + u + u^2/2 + o(u^2)$一推论

$$
x^{1/1} = 1 + (\log x)^2 + \frac{1}{2} \frac{(\log x)^4}{x} + \frac{1}{2} \frac{(\log x)^3}{x} + o \left( \frac{(\log x)^3}{x} \right).
$$

### 5. 渐近展开且变量系数

我们可以通过以下方式概括本金部分和渐近展开的概念。令 $\mathscr{E}$ 为由实数（或复数）函数形成的比较尺度，使得对于它们中的每一个，$\mathfrak{F}$ 中存在集合，其中函数 *不会在任何点* 处消失。进一步，设$C$为$\mathscr{H}(\mathfrak{F}, V)$满足中函数的集合，以下三个条件：

(CO₁) 每函数 $a \in C$ 就有 $a \preccurlyeq 1$。
(CO2) 关系 $a \ll 1$ 对于函数 $a \in C$ 意味着 $a = 0$。
(CO₃) $C$ 是向量空间超过 $\mathbf{R}$（分别为 $\mathbf{C}$）。

现在让$f$为$\mathscr{H}(\mathfrak{F}, V)$中的任意函数；如果存在函数$g \in \mathscr{E}$和非零的函数$a \in C$，使得$f - ag \ll g$可以说$ag$是$f$的主部分，相对于比较尺度$\mathscr{E}$和域系数$C$。如果存在这样一个主体部分，那么它是唯一的：假设有两个主体部分、$a_1 g_1$和$a_2 g_2$；一个不能有$g_1 \ll g_2$，因为从(CO₁)可以推断出$a_1 g_1 \ll g_2$和$f - a_1 g_1 \ll g_1 \ll g_2$，所以$f \ll g_2$；但也有 $a_2 g_2 \ll g_2$，因而 $a_2 \ll 1$ 与假设 $a_2 \neq 0$ 和 (CO2) 相矛盾。所以必须有$g_1 = g_2$；从关系 $f - a_1 g_1 \ll g_1, f - a_2 g_1 \ll g_1$ 可以通过 (CO2) 和 (CO₃) 推导出 $(a_2 - a_1)g_1 \ll g_1$ 从而 $a_2 - a_1 \ll 1$，从而推导出 $a_2 = a_1$。

#### 例 {#fvr-v-s2-n5-exa-1 .statement tag=08F3}

对于趋于 $+\infty$ 的 $x$ 实数，$\mathbf{R}$ 上的周期性有界函数，具有相同的周期 $\tau$、满足条件 (CO₁)、(CO2) 和 (CO₃)：如果 $\lim_{x \to +\infty} a(x) = 0$，则对于每个$\varepsilon > 0$ 存在一个$x_0$，使得每个$x \geq x_0$有$|a(x)| \leq \varepsilon$；对于$0 \leq x \leq \tau$也可以推出$|a(x)| \leq \varepsilon$，因为存在整数$n$使得$x + n\tau \geq x_0$，并且使得$a(x) = a(x + n\tau)$；因为$\varepsilon$是任意的，所以在$[0, \tau]$上有$a(x) = 0$，因此无处不在。

对于V、p. 222的记号，我们会说$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$，其中$a_\lambda$、属于到$C$以及除了有限的数之外的所有其他都是零，是一个渐近展开 $f$ 与 $C$ 中的系数，精确到 $g_\alpha$，如果 $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$；对于每个指标$\mu$，使得$a_\mu \neq 0$，则$a_\mu g_\mu$是$f - \sum_{\lambda < \mu} a_\lambda g_\lambda$的主部分，相对于$\mathscr{E}$和$C'$，这证明了唯一性的渐近展开 $f$（精确到$g_\alpha$）（当它存在时）。

n 3 (V, p. 223) 中给出的方法，用于形成$f_1 + f_2$或$[f_1 . f_2]$的渐近展开，从$f_1$和$f_2$的给定渐近展开开始，可以再次应用于展开对于变量系数，只要将$[a_\lambda . b_\mu]$属于到系数$C$相应的的域到范数空间$V$或承认渐近展开与系数 $C$。
