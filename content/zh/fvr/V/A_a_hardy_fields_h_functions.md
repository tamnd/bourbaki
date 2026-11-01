---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 0
section_title: Hardy Fields. (H) Functions
appendix: true
lang: zh
source: fvr-i-vii
book_pages: 247-258, 263-267
pdf_pages: 0262-0273, 0278-0282
extraction: ocr
subsections:
    - "no": 1
      title: HARDY FIELDS
      page: 247
      pdf_page: 262
    - "no": 2
      title: EXTENSION OF A HARDY FIELD
      page: 248
      pdf_page: 263
    - "no": 3
      title: COMPARISON OF FUNCTIONS IN A HARDY FIELD
      page: 250
      pdf_page: 265
    - "no": 4
      title: (H) FUNCTIONS
      page: 252
      pdf_page: 267
    - "no": 5
      title: EXPONENTIALS AND ITERATED LOGARITHMS
      page: 253
      pdf_page: 268
    - "no": 6
      title: INVERSE FUNCTION OF AN (H) FUNCTION
      page: 255
      pdf_page: 270
statements: 21
exercises: 15
content_sha256: fe41032cbd3510789e37d2d71bbc4df57ecf931c35841e56ed6120f747ecabd5
translated_from: content/en/fvr/V/A_a_hardy_fields_h_functions.md
translation_method: google
source_content_sha256: 90e02e3632c6ecc96144815961457f749d0c9a6edf475780ab90b36dc9feca0f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9c6e8dc6931300b460990236a35f4e4c29677c4d502c176f29296031d7affd25
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录

# 哈迪域。 (H) 函数

### 1.哈迪域

令$\mathfrak{F}$为$\mathbf{R}$上由形式$[x_0, +\infty[$间隔形成的滤波器基。回想一下，我们已经定义了等价关系$R_\infty$：在函数的集合$\mathscr{H}(\mathfrak{F}, \mathbf{R})$上，定义在集合属于到$\mathfrak{F}$“存在集合$M \in \mathfrak{F}$使得$f(x) = g(x)$在$M$”（V，p. 211），并且商集$\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$被赋予结构或*环*与单位元。

#### 定义 1 {#fvr-v-a0-def-1 .statement tag=08GO}

*给定$\mathscr{H}(\mathfrak{F}, \mathbf{R})$的子集$\mathfrak{K}$，如果$\mathfrak{K}$满足以下条件，则可以说$\mathfrak{K}/R_\infty$（$\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$中$\mathfrak{K}$的典范像）是哈代域：

1. $\mathfrak{K}/R_\infty$是环$\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$中的子域。
2. *$\mathfrak{K}$中的每个函数在区间$[a, +\infty[$（取决于函数）上连续且可微，并且类相对于其导数属于到$\mathfrak{K}/R_\infty$的$R_\infty$。*

$\mathfrak{K}/R_\infty$是*域*的假设等价于以下条件：如果$f \in \mathfrak{K}$和$g \in \mathfrak{K}$则$f + g$和$fg$等于$\mathfrak{K}$中的函数在某些集合上$\mathfrak{F}$；此外，如果$f$与$\mathfrak{F}$中的集合上的零不相同，则$\mathfrak{F}$中存在集合$M$，其中$f$*不会消失*，并且$1/f$等于函数 $\mathfrak{K}$于$M$；通过条件 2'，我们总是可以假设采用$M$，使得$f$在$M$上“连续”，因此在此区间上“具有恒定的符号”。

通过滥用语言，如果$\mathfrak{K}$使得$\mathfrak{K}/R_\infty$是哈代域，我们将在下文中说$\mathfrak{K}$本身是*哈代域*。

#### 例 1 {#fvr-v-a0-n1-exa-1 .statement tag=08GP}

*有理常数*的每个Hardy域包含域（特征0的最小的域，*cf.Alg.*，V, §1），其中一个可以确定和域$\mathbf{Q}$；此外，由于两个常数不能模$R_\infty$除非全等，因而$\mathbf{Q}/R_\infty$与$\mathbf{Q}$相同。 *实常量*也是形式和 Hardy 域，其中可以确定和 $\mathbf{R}$。

#### 例 2 {#fvr-v-a0-n1-exa-2 .statement tag=08GQ}

哈代域的一个非常重要的例是有理数函数与实系数*的*集合，我们将通过语言滥用将其表示为$\mathbf{R}(x)$；如果 $f(x) = p(x)/q(x)$ 是具有实数系数的有理数函数，与零不同，它是连续的、可微的，且 $\neq 0$ 在区间 $[a, +\infty[$ 上，其中 $a$ 严格大于多项式 $p(x)$ 的实数根的最大的且$q(x)$；因而 $\mathbf{R}(x)/R_\infty$ 中除了 0 之外的每个元素都是可逆的。我们再次注，两个有理函数不能全等模$\mathbf{R}_\infty$除非，它们相等，因而$\mathbf{R}(x)/\mathbf{R}_\infty$可以再次与$\mathbf{R}(x)$等同。

### 2. 扩张哈迪域

给定一个 Hardy 域 $\mathfrak{K}$，我们将看到如何形式新的 Hardy 域 $\mathfrak{K}' \supset \mathfrak{K}$，使得 $\mathfrak{K}'/\mathbf{R}_\infty$ 可以通过*邻接*（在代数意义上的项，*cf. Alg.*，V）获得。 §2）新的元素，我们将把形式精确到$\mathfrak{K}/\mathbf{R}_\infty$。

#### 引理 1 {#fvr-v-a0-lem-1 .statement tag=08GR}

*设* $a(x), b(x)$ *为两个连续实数函数，且变换不在区间* $[x_0, +\infty[$上签名。 *如果，在这个区间上，函数* $y(x)$ *连续且可微，并且满足恒等式*

$$
y' = ay + b
$$

(1)

*则存在一个区间* $[x_1, +\infty[$ *在其上* $y$ *没有变换符号。*

事实上，让我们把 $z(x) = y(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$ (*cf. IV*, p. 183);那么，通过(1)，$z'(x) = b(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$。如果 $x \geqslant x_0$ 为 $b(x) \geqslant 0$，则 $z$ 在该区间上为递增，因此要么在所有该区间上为 $< 0$，要么在区间 $[x_1, +\infty[$ 上为零，要么在区间 $[x_1, +\infty[$ 上为 $> 0$；由于 $y$ 与 $z$ 具有相同的符号，因此在本例中证明了命题。如果 $b(x) \leqslant 0$ 对应 $x \geqslant x_0$，则论证类似。

#### 注 {#fvr-v-a0-n2-rem-1 .statement tag=08GS}

这个非常初等的性质不扩展阶 $> 1$ 的线性微分方程；对于例，函数$y = \sin x$满足$y'' + y = 0$，但变换在$+\infty$的每个邻域上签名。

#### 引理 2 {#fvr-v-a0-lem-2 .statement tag=08GT}

*设* $a(x)$ *和* $b(x)$ *是给定 Hardy 域* $\mathfrak{K}$ *和* $y(x)$ *函数满足的两个函数属于恒等式* (1) *在一个区间上* $[x_0, +\infty[$ *其中* $a$ *和* $b$ *已定义且连续*。 *如果* $p(u)$ *是* $u$ *其系数为* $x$ *属于到* $\mathfrak{K}$ 的函数，*在* $[x_0, +\infty[$ 上定义且可微，*则存在一个区间* $[x_1, +\infty[$ *在其上函数* $p(y)$ *没有变换符号*。

如果 $p(u)$ 在 $[x_0, +\infty[$ 上具有与零相同的系数，或者如果 $p(u)$ 在 $u$ 中为次数 0，则命题是平凡的，因为 $\mathfrak{K}$ 中的任何函数在区间上具有恒定符号$[x_1, +\infty[$。假设$p(u)$是次数$n > 0$； $p(u)$ 的首项系数 $c$ 则在区间 $[\alpha, +\infty[$ 上为 $\neq 0$；因此，我们可以写 $p(u) = c(u^n + c_1 u^{n-1} + \cdots + c_n)$，其中 $c, c_1, c_2, \ldots, c_n$ 是 *函数* 属于到 $\mathfrak{K}$，并且在 $[\alpha, +\infty[$ 上可微；所以只要证明引理为$c = 1$就足够了。我们以归纳对$n$争论；一个有

$$
\frac{d}{dx} (p(y)) = (ay + b)(ny^{n-1} + (n-1)c_1 y^{n-2} + \cdots + c_{n-1})
$$
$$
+ c'_1 y^{n-1} + \cdots + c'_n = na\ p(y) + q(y)
$$

其中 $q(u)$ 是次数 $\leq n - 1$ 的多项式，系数为 $\mathfrak{K}$。由假设函数$na(x)$和$q(y(x))$不变换在区间$[ \beta, +\infty[$上签名；因此，引理是引理 1 的推论。

#### 定理 1 {#fvr-v-a0-thm-1 .statement tag=08GU}

*对于给定的 Hardy 域 $\mathfrak{K}$ 和 $y(x)$ 函数满足 (1)，令 $a(x)$ 和 $b(x)$ 为两个函数属于 (1)，区间为 $[ x_0, +\infty[$。当$r(u) = p(u)/q(u)$通过$u$中的有理分式的集合且系数在$\mathfrak{K}$中时，使得$q(y)$与$+\infty$的邻域上的零不相同，集合$\mathfrak{K}(y)$ 函数$r(y)$形式哈代域.*

事实上，到引理 2，存在一个区间$[ x_1, +\infty[$，$r(y)$在其上定义、连续且没有变换符号，从中可以立即得出$\mathfrak{K}(y)/\mathbf{R}_\infty$是域；此外，由于

$$
\frac{d}{dx}(r(y)) = r'(y)y' = r'(y)(ay + b)
$$

（其中$r'(y) = (p'(y)q(y) - p(y)q'(y))/(q(y))^2$由$+\infty$的邻域上的假设定义），$\mathfrak{K}(y)$属于到$\mathfrak{K}(y)$中每个函数的导数，证明$\mathfrak{K}(y)$满足def的条件。 V、p. 247 中的 1 个。

显然，$\mathfrak{K}(y)/\mathbf{R}_\infty$是由$y$模$\mathbf{R}_\infty$的类的代数*伴随*到$\mathfrak{K}/\mathbf{R}_\infty$得到。 Again one says that $\mathfrak{K}(y)$ is obtained by *adjoining* $y$ to $\mathfrak{K}$.

#### 推论 1 {#fvr-v-a0-thm-1-cor-1 .statement tag=08GV}

*如果$\mathfrak{K}$中的$y$是函数，而不是$+\infty$的邻域上的零，则$\mathfrak{K}(\log|y|)$是哈代域。*

事实上，在 $\mathfrak{K}$ 的区间 $[ x_0, +\infty[$ 上，$(\log|y|)' = y'/y$ 等于函数。

推论 2 *如果 $y$ 是 $\mathfrak{K}$ 中的任意函数，则 $\mathfrak{K}(e^y)$ 是 Hardy 域。*

事实上，$(e^y)' = e^y y'$和$y'$等于$\mathfrak{K}$中的函数，且间隔为$[ x_0, +\infty[$。

COROLLARY 3 *If $\mathfrak{K}$ contains the real constants, and if $y$ is a function in $\mathfrak{K}$, not identically zero on a neighbourhood of $+\infty$, then $\mathfrak{K}(|y|^{\alpha})$ is a Hardy field for every real number $\alpha$.*

事实上，$\frac{d}{dx}(|y|^{\alpha}) = |y|^{\alpha} (\alpha y'/y)$和$\alpha y'/y$等于$\mathfrak{K}$中的函数，且间隔为$[ x_0, +\infty[$。

最后，我们注，如果$y$是$\mathfrak{K}$中任何函数的*原语*，那么$\mathfrak{K}(y)$又是Hardy域。

### 3. 函数与 Hardy 域的比较

#### 命题 1 {#fvr-v-a0-prop-1 .statement tag=08GW}

*同一个 Hardy 域中的两个函数可与任何阶*（V、p. 232）相媲美。

事实上，如果 $f$ 属于到 Hardy 域 $\mathscr{K}$，那么对于每个整数 $n > 0$ 都存在一个区间 $[x_0, +\infty[$，其中 $f$ $n$ 倍可微，其 $n^{th}$ 导数等于函数在$\mathscr{K}$ 在此间隔内。因此，足以证明 $\mathscr{K}$ 中的任何两个函数 $f, g$ 都是“可比较的”。如果函数之一与 $+\infty$ 的邻域上的零相同，则这一点很明显；因此，我们可以限制自己的情况，即它们在邻域和 $+\infty$ 上都严格为正。但是，对于每个实数$t$，$f - tg$等于$+\infty$的邻域上的$\mathscr{K}$中的函数，因此$+\infty$的邻域上有常数符号，这就证明了命题 （V，p. 217，第 9 条）。

由此命题可以立即推断出，如果 Hardy 域 $\mathscr{K}$ 包含为实常数（正如我们在下文中始终假设的那样），并且如果 $f$ 和 $g$ 是 $\mathscr{K}$ 中的任意两个函数，则以下任意两个函数 $e^f, e^g, \log |f|, \log |g|, |f|^{\alpha}, |g|^{\alpha}$（$\alpha$任意实数），$\int_a f, \int_a g$（$a$是$[x_0, +\infty[$区间内的任何实数，其中$f$和$g$受到调节）是*可比较的*（当它们被定义时）；事实上，任何两个函数属于到给定的 Hardy 域都可以通过将它们连续邻接到 $\mathscr{K}$ 来获得。

类似地，Hardy 域 $\mathscr{K}$ 中的每个函数 $f(x)$ 都可与 $x$ 进行比较，因为 $x$ 和 $f(x)$ 属于与通过将 $x$ 邻接而获得的 Hardy 域可以比较$\mathscr{K}$。因此，结论（特别是）$f$可与任何阶、每个幂、$x^{\alpha}$、以及$\log x$和$e^x$进行比较。

我们还可以看出，如果 $f$ 和 $g$ 属于为同一个 Hardy 域 $\mathscr{K}$，如果 $g(x) > 0$ 在区间 $[x_0, +\infty[$ 上，并且如果 $g(x)$ 趋于 0 或$+\infty$，如下所示： $x$趋于$+\infty$，则$f$相对于$g$（V，p. 219）的*阶*总是被定义。

因此，V、p. 233的第 8 条命题适用于 Hardy 域中的每个函数 $f$，并证明：

1) 如果 $f$ 相对于 $x$ 是阶 $+\infty$，则$\int_a^x f(t)\,dt \sim (f(x))^2/f'(x)$。

2) 如果$f$相对于$x$是阶$\mu > -1$，则$\int_a^x f(t)\,dt \sim \frac{1}{\mu+1} x f(x)$。

3) 如果$f$相对于$x$是阶$\mu < -1$，则$\int_a^{+\infty} f(t)\,dt \sim -\frac{1}{\mu+1} x f(x)$。

4) 如果$f$相对于$x$是阶$-\infty$，则$\int_a^{+\infty} f(t)\,dt \sim -(f(x))^2/f'(x)$。

此外，我们有以下命题：

#### 命题 2 {#fvr-v-a0-prop-2 .statement tag=08GX}

令 $f$ 为函数属于到 Hardy 域 $\mathscr{K}$。

1 如果 $f$ 相对于 $x$ 是无限的阶，则对于每个整数 $n > 0$，
$$
f^{(n)}(x) \sim \frac{(f'(x))^n}{(f(x))^{n-1}}.
$$
(2)

2° 如果 $f$ 相对于 $x$ 是有限的阶 $\mu$ 那么，对于每个 $n > 0$，
$$
f^{(n)}(x) \sim \mu(\mu - 1) \ldots (\mu - n + 1) \frac{f(x)}{x^n}
$$
$$
\sim \frac{(\mu - 1) \ldots (\mu - n + 1)}{\mu^{n-1}} \frac{(f'(x))^n}{(f(x))^{n-1}}
$$
(3)
除非 $\mu$ 是整数 $\geqslant 0$ 和 $n > \mu$。

1 如果$f$相对于$x$而言是无限的阶，则有$\log |f| \gg \log x$，因此，由于$\log |f|$和$\log x$可与任何阶、$f'/f \gg 1/x$进行比较。把$g = f'/f$；因为$g$等于$+\infty$的邻域上的$\mathscr{K}$中的函数，所以可以从$1/g \ll x$推出$g'/g^2 \ll 1$，等等$g'/g \ll g = f'/f$，或者再次推出$fg' \ll gf'$。从关系 $f' = fg$ 微分推出
$$
f'' = fg' + gf' \sim gf'
$$
或者再次$f''/f' \sim f'/f$。同样的论点，应用于 $f^{(n)}$ 而不是 $f$，则通过归纳在 $n$ 上显示 $f^{(n)}/f^{(n-1)} \sim f'/f$； 从而关系 (2)。

2 如果$f$相对于$x$是有限的阶$\mu$，并且如果$\mu \neq 0$，则有$\log |f| \sim \mu \log x$，从而，微分时，$f'(x) \sim \mu \frac{f(x)}{x}$；推论出$f'$相对于$x$而言是阶$\mu - 1$，这允许人们在$n$上通过归纳应用相同的参数，只要$\mu \neq n$、从而公式 (3) 当$\mu$不是时整数$\geqslant 0$和$< n$。

当$f$相对于$x$是阶$p \geqslant 0$的整数时，可以写成$f(x) = x^p f_1(x)$，其中$f_1$相对于$x$是阶0。通过道具。 2个有
$$
f^{(p)} \sim p! f_1.
$$
为了评估阶$n > p$的导数，我们可以将自己限制在$p = 0$的情况。那么一个有$\log |f| \ll \log x$，从而$f'(x)/f(x) \ll 1/x$，其他字$x f'(x) \ll f(x)$；如果$f$不等于常数$k \neq 0$，则在微分这个关系（V，p. 232，道具7）时，有$x f''(x) + f'(x) \ll f'(x)$，这意味着$x f''(x) \sim -f'(x)$。考虑到这个公式，人们可以通过$n$上的归纳看到$f^{(n)}$相对于$x$是阶$\leqslant -n$，并且
$$
f^{(n)} \sim (-1)^{n+1} (n-1)! \frac{f'(x)}{x^{n-1}}.
$$
(4)

如果$f$等价于常数$k \neq 0$，则有$f(x) = k + f_2(x)$和$f_2 \ll 1$，约化可以研究$f_2$的导数。

### 4.(H) 函数

#### 命题 3 {#fvr-v-a0-prop-3 .statement tag=08GY}

*如果 $\mathscr{K}_0$ 是 Hardy 域，则存在 Hardy 域 $\mathscr{K}$ 包含 $\mathscr{K}_0$，因此，对于每个函数 $z \in \mathscr{K}$，邻域上的零不相同$+\infty$、$e^z$ 和 $\log |z|$ 属于至 $\mathscr{K}$。*

Denote by $\mathscr{K}$ the set of functions $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ having the following properties: for each function $f \in \mathscr{K}$ there is a finite number of Hardy fields $\mathscr{K}_1, \mathscr{K}_2, \ldots, \mathscr{K}_n$ (the number $n$ and the fields $\mathscr{K}_i$ depending on $f$) such that $f \in \mathscr{K}_n$ and, for $0 \leq i \leq n-1$, one has $\mathscr{K}_{i+1} = \mathscr{K}_i(u_{i+1})$ where $u_{i+1}$ is equal either to $e^{z_i}$ or to $\log |z_i|$ with $z_i$ belonging to $\mathscr{K}_i$ and not vanishing identically on a neighbourhood of $+\infty$. 有人说域 $\mathscr{K}_n$ 和函数 $f$ 的 $u_1, u_2, \ldots, u_n$ 形式 a *定义序列*；同一个函数自然可以容纳多个定义序列。

按定义。 V、p. 247中的 1，每个函数 $f \in \mathscr{K}$，与 $+\infty$ 的邻域上的零不相同，具有常数符号并且在区间 $[x_0, +\infty[$ 上可微；如果$f \in \mathscr{K}_n$，则$1/f$和$f'$等于$\mathscr{K}_n$中的函数，因此等于$\mathscr{K}$中的函数，在$+\infty$的邻域上。要看出$\mathscr{K}$是哈代域，就足以证明如果$f$和$g$是$\mathscr{K}$中的两个函数，则$f - g$和$fg$等于$\mathscr{K}$中的函数邻域共 $+\infty$。现在让$f$的$u_1, u_2, \ldots, u_m$为定义序列，$v_1, v_2, \ldots, v_n$定义序列为$g$。通过连接序列 $(u_i)$ 和 $(v_i)$ 获得的序列 $u_1, u_2, \ldots, u_m, v_1, v_2, \ldots, v_n$ 又是 Hardy 域 $\mathscr{K}_{m+n}$ 的定义序列和这个域包含 $f$和$g$，因此$f - g$和$fg$等于$+\infty$的邻域上的$\mathscr{K}_{m+n}$中的函数。

有人说，在 prop 的证明中定义的 Hardy 域 $\mathscr{K}$ 。 3 是 Hardy 域 $\mathscr{K}_0$ 的 (H) *扩张*。

如果 $\mathscr{K}'$ 是另一个 Hardy 域拥有道具中所述的属性。 3，从$\mathscr{K}$的构造得出$\mathscr{K}/\mathbf{R}_\sim$*包含于*在$\mathscr{K}'/\mathbf{R}_\sim$中。滥用语言，有人说 Hardy 域 $\mathscr{K}_0$ 的 (H) 扩张是具有这些属性的 *最小的* Hardy 域 $\mathscr{K}$。

#### 定义 2 {#fvr-v-a0-def-2 .statement tag=08GZ}

* (H) 函数的域称为实系数有理函数的Hardy 域 $\mathbf{R}(x)$ 的(H) 扩张。任何函数属于到此扩张称为 (H) 函数。*

继定义之后，如果$f$是(H)函数，与$+\infty$的邻域上的零不相同，则$e^f$和$\log |f|$也是(H)函数。更一般地，如果$g$是第二个（H）函数，并且$u_1, u_2, \ldots, u_n$定义序列对于$g$，并且如果$f(x)$与$x$趋向于$+\infty$，则可以通过归纳看到$n$复合函数$u_1 \circ f, u_2 \circ f, \ldots, u_n \circ f$和$g \circ f$是(H)函数。

### 5.指数和迭代对数

我们已经（V，p. 229）定义了$n \geq 1$的*迭代对数*$l_n(x)$乘以条件$l_0(x) = x, l_n(x) = \log(l_{n-1}(x))$。以同样的方式，对于$n \geq 1$，定义*迭代指数*$e_n(x)$乘以条件$e_0(x) = x, e_n(x) = \exp(e_{n-1}(x))$。它是直接的，通过$n$上的归纳，$l_n(x)$是$e_n(x)$的逆函数，为$x > e_{n-1}(0)$定义，并且$e_m(e_n(x)) = e_{m+n}(x), l_m(l_n(x)) = l_{m+n}(x)$。每 $\mu > 0$ 关系 $\log x \ll x^\mu \ll e^x$，就有 $n \geq 1$，

$$
l_n(x) \ll (l_{n-1}(x))^\mu \quad \text{for every } \mu > 0 \tag{5}
$$

$$
e_{n-1}(x^{1+\beta}) \ll e_n(x^{1+\delta}) \ll e_n((1-\gamma)x) \ll (e_n(x))^\mu
$$
$$
\ll e_n((1+\alpha)x) \ll e_n(x^{1+\beta}) \tag{6}
$$

对于所有 $\mu > 0, \alpha > 0, \beta > 0, 0 < \gamma < 1, 0 < \delta < 1$，这些数是任意的（*cf.* V，p. 218，道具 11）。

我们已经看到 (V, p. 229)，对于 $n \geq 1$，有

$$
\frac{d}{dx}(l_n(x)) = \prod_{i=0}^{n-1} \frac{1}{l_i(x)}. \tag{7}
$$

同样对于 $n \geq 1$

$$
\frac{d}{dx}(e_n(x)) = \prod_{i=1}^n e_i(x). \tag{8}
$$

从而，通过道具。 8 个V、p. 233，每$\mu > 0$

$$
\int_a^x e_n(t^\mu) \, dt \sim \frac{x}{\mu} e_n(x^\mu) \prod_{i=0}^{n-1} \frac{1}{e_i(x^\mu)} \tag{9}
$$

$$
\int_x^{+\infty} \frac{dt}{e_n(t^\mu)} \sim \frac{x}{\mu} \prod_{i=0}^n \frac{1}{e_i(x^\mu)}. \tag{10}
$$

可以证明，如果 $f$ 是 *任意* (H) 函数使得 $f \gg 1$ 则存在两个整数 $m$ 和 $n$ 使得

$$
l_m(x) \ll f(x) \ll e_n(x)
$$

（V，p. 263，练习 1 和 p. 264，练习 5） 另一方面，可以定义递增函数 $g(x)$ （不再是 (H) 函数）使得 $g(x) \gg e_n(x)$ 为*每个* $n > 0$，或 $1 \ll g(x) \ll l_m(x)$ 代表*每个* $m > 0$（V、p. 265，练习 8、9 和 10）。

借助迭代对数，我们将证明，可以定义 $\mathscr{E}$（对于 $x$ 趋向 $+\infty$）（H）函数，即 $> 0$ 在 $+\infty$ 的邻域上，并且满足以下条件：

a) $\mathscr{E}$ 属于至$\mathscr{E}$中任意两个函数中的乘积；
b) 每函数 $f \in \mathscr{E}$ 和每实数 $\mu$ $f^\mu \in \mathscr{E}$；

c) 对于每个函数$f \in \mathscr{E}$，$\log f$是$\mathscr{E}$中函数的有限数的线性组合；
d) 对于每个函数$f \in \mathscr{E}$，除了常数1之外，$e^f$等价于$\mathscr{E}$中的函数。

首先我们考虑形式$\prod_{m=0}^{\infty} (l_m(x))^{\alpha_m}$的函数的集合$\mathscr{E}_0$，其中$\alpha_m$是实数、零，除了指标$m$的有限数； 直接的，由(5)(V，p. 253)得出，这些函数形式是满足条件$a), b)$和c)的*比较量表*。现在我们定义，通过对$n$的递归，由常数1和形式$\exp \left( \sum_{k=1}^p a_k f_k \right)$的函数形成集合$\mathscr{E}_n$（对于$n \geqslant 1$），其中$p$是任意整数 $> 0$、函数 $f_k$ ($1 \leqslant k \leqslant p$) 是$\mathscr{E}_{n-1}$中的函数，使得$f_1 \gg f_2 \gg \cdots \gg f_p \gg 1$，并且$a_k$是实数$\neq 0$；我们通过归纳表明$\mathscr{E}_n$是一个*比较量表*满足$a), b)$和c)和包含$\mathscr{E}_{n-1}$。首先，关系$\mathscr{E}_{n-1} \subset \mathscr{E}_n$适用于$n = 1$，因为$\mathscr{E}_0$中任何非常数函数的对数为形式$\sum_{k=1}^p a_k f_k$，其中$f_k$是迭代对数，所以$\gg 1$；另一方面，如果$\mathscr{E}_{n-2} \subset \mathscr{E}_{n-1}$从$\mathscr{E}_n$的定义推出$\mathscr{E}_{n-1} \subset \mathscr{E}_n$；该定义进一步表明$\mathscr{E}_n$满足$a), b)$和c)。还需要看到$\mathscr{E}_n$是一个比较标度：因为$\mathscr{E}_n$中的两个函数又是属于到$\mathscr{E}_n$的商，足以证明$\mathscr{E}_n$的每个函数$f$，除了常数1， 不能相当于常数$\neq 0$。现在，$\log f = \sum_{k=1}^p a_k f_k \sim a_1 f_1$乘以构造，并且由于$f_1 \gg 1$，$\log f$趋向于$\pm \infty$，因此$f$趋于0或$+\infty$，因为$x$趋向于$+\infty$。

既然如此，如果$\mathscr{E}$是$n \geqslant 0$的$\mathscr{E}_n$的*并*，那么$\mathscr{E}$是一个比较尺度，对于$\mathscr{E}$属于中的两个函数来说，$\mathscr{E}_n$是相同的尺度；同理，$\mathscr{E}$满足a)，显然也满足b)和c)。最后，如果$f \in \mathscr{E}$存在$n$使得$f \in \mathscr{E}_n$；如果$f$不是常数1，则$f(x)$趋向于0或$+\infty$，因为$x$趋向于$+\infty$；在第一种情况下$e^f \sim 1$，在第二种情况下，$e^f$属于到$\mathscr{E}_{n+1}$定义，依此类推到$\mathscr{E}$。

#### 注 {#fvr-v-a0-n5-rem-1 .statement tag=08H0}

尽管我们刚刚定义的尺度$\mathscr{E}$具有实际用途，但很容易给出（H）函数的例，它*相对于$\mathscr{E}$没有本金部分*。事实上，如果$f$是一个(H)函数使得$f \sim a g$，其中$a$是常数$> 0$和$g \in \mathscr{E}$，那么$\log f - \log g - \log a$随着$1/x$趋于0，所以$\log f$承认，相对于$\mathscr{E}$，渐近展开，其*余数趋于 0*，到性质 c)。现在，如果考虑例，则 (H) 函数 $f(x) = e_2 \left( x + \frac{1}{x} \right)$ 有 $\log f(x) = \exp \left( x + \frac{1}{x} \right)$，因此 $\log f$ 相对于 $\mathscr{E}$ 的渐近展开为形式

$$
\log f(x) = e^x + \frac{e^x}{x} + \frac{1}{2!} \frac{e^x}{x^2} + \cdots + \frac{1}{n!} \frac{e^x}{x^n} + o \left( \frac{e^x}{x^n} \right) \quad (n \text{ an integer } > 0).
$$

显然，这个展开中的余数相当于$\frac{1}{(n+1)!} \frac{e^x}{x^{n+1}}$，因此不趋于0。因此$f$相对于$\mathscr{E}$没有主部分。

### 6. AN (H) 函数的逆函数

如果$f$是一个(H)函数，则$f$在区间$[x_0, +\infty[$上单调连续，因此$f$的限制的逆函数$\varphi$在邻域上单调连续点$a = \lim_{x \to +\infty} f(x)$；但是，如果 $a$ 等于 $+\infty$（分别为 $-\infty$，有限），则可以证明 $\varphi(y)$（分别为 $\varphi(-y)$、$\varphi \left( a + \frac{1}{y} \right)$ 或 $\varphi \left( a - \frac{1}{y} \right)$）一般不等于邻域上的 (H) 函数 $+\infty$。然而，我们将看到，在某些重要情况下，我们可以获得相当于 $\varphi(y)$（分别为$\varphi(-y)$、$\varphi \left( a + \frac{1}{y} \right)$、$\varphi \left( a - \frac{1}{y} \right)$）的 (H) 函数，以及有时，甚至相对于标度的函数的渐近展开 $\mathscr{E}$ 定义于V、p. 254。

我们将使用以下命题：

#### 命题 4 {#fvr-v-a0-prop-4 .statement tag=08H1}

令 $p$ 和 $q$ 为两个 (H) 函数，它们在区间 $[x_0, +\infty[$ 上严格为正。

1° 如果 $q \ll p/p'$ 有 $p(x + q(x)) \sim p(x)$。
2° 如果$q \ll p/p'$ 和$q(x) \ll x$ 都存在，则$p(x - q(x)) \sim p(x)$。

如果$p \sim k$（常数$\neq 0$），则此命题的两个部分是明确的；因此，我们可以假设$p(x) \ll 1$（否则可以将论证应用于$1/p$）。然后推导出$p'(x) \ll 1$。

1° 可以用 $0 \leq \theta \leq 1$ 写出$p(x + q(x)) = p(x) + q(x)p'(x + \theta q(x))$（I、p. 14，推出）。由于$|p'(x)|$趋向于0，而$x$趋于$+\infty$，并且等于$+\infty$的邻域上的(H)函数，因此在区间$[x_1, +\infty[$上有递减，因此，对于$x \geq x_1$，有$|p'(x + \theta q(x))| \leq |p'(x)|$；从 $qp' \ll p$ 开始，一个人就有 $p(x + q(x)) \sim p(x)$。

2° 条件 $q(x) \ll x$ 确保 $x - q(x)$ 趋向于 $+\infty$ 和 $x$。再次有 $p(x - q(x)) = p(x) - q(x)p'(x - \theta p(x))$ 和 $0 \leq \theta \leq 1$。与证明的第一个部分相同的论证表明，对于$x$足够大，$|p'(x - \theta q(x))| \leq |p'(x - q(x))|$。它约化表明$q(x) \frac{p'(x - q(x))}{p(x - q(x))}$趋于0，而$x$趋于$+\infty$。如果 $p'/p \gg 1$ 从那时起 $|p'/p|$ 是 (H) 函数，递增对于 $x$ 足够大，则命题为真；因此 $q(x) \frac{|p'(x - q(x))|}{|p(x - q(x))|} \leq q(x) \frac{|p'(x)|}{|p(x)|}$，$qp' \ll p$ 假设。如果$p'/p \sim k$（$k$常量$\neq 0$）也成立，那么

$$
\frac{p'(x - q(x))}{p(x - q(x))} \sim \frac{p'(x)}{p(x)}
$$

因为$x - q(x)$趋向于$+\infty$。只剩下检查$p'/p \ll 1$的情况了。首先假设 $p(x)$ 相对于 $x$ 是*有限* 阶，因此 (V, p. 232, 命题 7) $p'(x)/p(x) \ll 1/x$。然后一个有
$$
\frac{p'(x-q(x))}{p(x-q(x))} = \frac{1}{x-q(x)} O_1(1),
$$
所以
$$
q(x) \frac{p'(x-q(x))}{p(x-q(x))} = \frac{q(x)}{x} \left( 1 - \frac{q(x)}{x} \right)^{-1} O_1(1) = \frac{q(x)}{x} O_2(1),
$$
在这种情况下，人们会发现命题 *仅*是假设 $q(x) \ll x$ 的真实主题。最后我们检查$1/x \ll p'(x)/p(x) \ll 1$的情况；那么函数$r = p'/p$相对于$x$是有限的阶；因为，根据前面的注，道具。 V、p. 255中的4个适用于这样的函数，其中一个有$p'(x-q(x))/p(x-q(x)) \sim p'(x)/p(x)$，假设$qp' \ll p$可以让我们完成证明。

#### 注 {#fvr-v-a0-n6-rem-3 .statement tag=08H2}

右$q(x)$施加的条件可能不会得到改善，如下例所示：

一）
$$
p(x) = e^x, \quad q(x) = 1 = \frac{p(x)}{p'(x)}, \quad p(x+q(x)) = ep(x)
$$

b)
$$
p(x) = \log x, \quad q(x) = x - \log x \ll \frac{p(x)}{p'(x)} = x \log x,
$$
$$
p(x-q(x)) = \log \log x \ll p(x).
$$

我们首先要研究特定类型的 (H) 函数的逆：

#### 命题 5 {#fvr-v-a0-prop-5 .statement tag=08H3}

*设g为* (H) *函数，不等于常量$\neq 0$，并且使得* $g(x) \ll x$，*且令* $u(x)$ *为* $x - g(x)$的逆函数，*在* $+\infty$的邻域上定义。 *设*$(u_n)$*为函数的序列，通过递归*$n$，*通过条件*$u_0(x) = x$，$u_n(x) = x + g(u_{n-1}(x))$*为*$n \geqslant 1$； *然后* $u_n \gg 1$ *和*
$$
u(x) - u_n(x) \sim g(x)(g'(x))^n.
$$ (11)

让我们放入$y = u(x)$，$y_n = u_n(x)$；然后是$x = y - g(y)$、$y_0 = x$和$y_n = x + g(y_{n+1})$。首先推导出 $x/y = 1 - \frac{g(y)}{y}$；由于$y$与$x$趋向于$+\infty$，假设$g(x) \ll x$表明$y = u(x) \sim x = y_0$；进一步，
$$
y - x = g(y) = g(x) + (y - x)g'(z)
$$
其中 $z$ 属于到端点为 $x, y$ 的区间；当$x$趋向于$+\infty$时，$z$也趋向于$g(x) \ll x$，$g' \ll 1$，因而$g'(z)$趋于0，因而
$$
y - x = g(x) + o(y - x)
$$

从而
$$
u(x) - x \sim g(x).
$$
(12)

第二，我们通过 $n$ 的递归证明，当 $x$ 趋于 $+\infty$ 时，有 $u_n \gg 1$，并且
$$
u(x) - u_n(x) \ll u(x) - u_{n-1}(x).
$$
(13)

事实上，$y - y_n = g(y) - g(y_{n-1}) = (y - y_{n-1})g'(z_{n-1})$，其中$z_{n-1}$属于到端点为$y$和$y_{n-1}$的区间；通过归纳假设 $z_{n-1}$ 趋向于 $+\infty$ 和 $x$，因而 $g'(z_{n-1})$ 趋向于 0，从而证明了（13）。由此关系以及 (12) 推出 $u(x) - u_n(x) \ll u(x) - x \sim g(x) \ll x \sim u(x)$、从而 $u_n(x) \sim u(x)$，进而推出 $u_n \gg 1$。最后，关系$u(x) - u_n(x) \ll u(x) - x$还可以写成$(u(x) - x) - (u_n(x) - x) \ll u(x) - x$、从而
$$
u_n(x) - x \sim u(x) - x \sim g(x).
$$
(14)

为了证明（11），首先注，如果$t(x)$是函数使得$t(x) - x \sim g(x)$，那么就有$g'(t(x)) \sim g'(x)$。事实上，对于任何$\varepsilon > 0$，$x$足够大$g'$都是单调的，所以$g'(t(x))$位于$g'(x + (1 + \varepsilon)g(x))$和$g'(x + (1 - \varepsilon)g(x))$之间。 V、p. 255的第4条命题表明，只要已经建立了关系$g \ll g'/g''$，就有$g'(t(x)) \sim g'(x)$。现在，如果$g$相对于$x$来说是无限的阶，则有（V，p. 251，道具2）$g''/g' \sim g'/g$，并且，从$g' \ll 1, g \ll g/g' \sim g'/g''$开始；如果 $g$ 相对于 $x$ 是有限的阶 $\mu$，则必然有 $\mu \leq 1$；如果$\mu < 1$，由于$g$不等于常数$\neq 0$，公式 (3) 和 (4) (V，p. 251) 再次证明$g''/g' \sim k/x$ ($k$常数$\neq 0$)，从而 $g \ll g'/g''$；最后，如果$\mu = 1$，则$g'$相对于$x$的阶为0，因此$g''/g' \ll 1/x$，再次$g \ll g'/g''$。

既然如此，由于$z_{n-1}$位于$y$和$y_n$之间，由(14)可知$z_{n-1} - x \sim g(x)$、从而$g'(z_{n-1}) \sim g'(x)$；因此
$$
y - y_n \sim (y - y_{n-1})g'(x),
$$
从而我们在$n$上通过归纳得到(11)。

#### 注 1 {#fvr-v-a0-n6-rem-1 .statement tag=08H4}

如果$g$相对于$x$为阶$< 1$，一旦$n$为足够大，函数$u(x) - u_n(x)$与$x$趋于0。事实上，在相反的情况下，每个 $n$ 都会有 $g{g''}^n \gg 1$，因此 $g$ 相对于 $1/g'$ 来说将是无限的阶；在其他字中，可以有$\log|g| \gg \log|g'|$、从而，微分时有$g'/g \gg g''/g'$。但是，如果$g$相对于$x$来说是阶$\mu < 1$，则当$\mu = -\infty, \frac{g'}{g} \sim \frac{\mu}{\mu - 1} \frac{g''}{g'}$时$\mu \neq 0$时有$g'/g \sim g''/g'$，最后当$\mu = 0$时有$g'/g \ll g''/g'$ (V, p. 251, n 3）。

相反，如果 $g$ 相对于 $x$ 为阶 1，则对于每个整数 $n > 0$，可以有 $g{g''}^n \gg 1$，如例 $g(x) = x/\log x$ 所示。

#### 注 2 {#fvr-v-a0-n6-rem-2 .statement tag=08H5}

当$g(x)$是等价于常数$k \neq 0$的(H)函数时，有$g(x) = k + g_1(x)$，其中$g_1 \ll 1$； 函数$u_1(x) = u(x) - k$是函数$x - g_1(x + k)$的逆，并且将一个带回到在道具中处理的情况。 5 个V、p. 256。

因此，要使函数 $u$ 具有渐近展开，就足以使函数 $u_n$ 具有这样的展开：如果 $g$ 相对于所考虑的尺度承认渐近展开，则因此导致（由(H) 函数) 到问题的定义在V、p. 223到227中进行了检查。

最一般的情况如下，约化适用于道具中处理的情况。 V、p. 256 中的 5 个：函数 $y = u(x)$ 假定为满足关系
$$
\varphi(x) = \psi(y) - g(y)
$$
其中 $\varphi$ 是 (H) 函数，$\psi$ 是 (H) 函数，使得 $\psi \gg 1$ 且$\psi$ 的倒数函数 $\theta$ 也是 (H) 函数，并且$g$ 是 (H) 函数，使得 $g \ll \psi$。现在让$v(x)$是$x - g(\theta(x))$的逆函数；一个有$u = \theta \circ v \circ \varphi$，和$g(\theta(x)) \ll x$；如果有人知道 $v$ 的渐近展开，感谢 prop. 5 of V, p. 256，然后可以推导出$u$的渐近展开，如V，p. 223到227。

#### 例 1 {#fvr-v-a0-n6-exa-1 .statement tag=08H6}

让我们寻找$x^5 + x$的逆函数$v(x)$的渐近展开（因为$x$趋于$+\infty$）；将$x^5 = t$一置导致求$t + t^{1/5}$的逆函数$u(t)$的展开（对于$t$趋于$+\infty$），即应用prop。 V、p. 256中的 5 个，到$g(t) = -t^{1/5}$的情况。让我们，为例，计算，$u_2(t)$；一个有
$$
u_2(t) = t - \left( t - t^{1/5} \right)^{1/5} = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{2}{25} t^{-7/5} + o_1\left( t^{-7/5} \right).
$$
此外，由 (11) (V, p. 256)
$$
u(t) - u_2(t) \sim -\frac{1}{25} t^{-7/5}
$$
从而
$$
u(t) = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{1}{25} t^{-7/5} + o_2\left( t^{-7/5} \right)
$$
推导出展开
$$
v(x) = u(x)^{1/5} = x^{1/5} - \frac{1}{5} x^{-3/5} - \frac{1}{25} x^{-7/5} + o_3\left( x^{-7/5} \right)
$$
寻求。

#### 例 2 {#fvr-v-a0-n6-exa-2 .statement tag=08H7}

让我们寻找函数$x / \log x$的逆函数的渐近展开；从恒等式$x = y / \log y$，其中$y = v(x)$，推导出$\log x = \log y - \log \log y$；当放置$z = \log y, t = \log x$时，一个有$t = z - \log z$，并且引导一个展开$t - \log t$的逆函数$u(t)$；对于例，有一个
$$
u_2(t) = t + \log(t + \log t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + o_1\left( \frac{\log t}{t^2} \right)
$$
此外，由 (11) (V, p. 256)
$$
u(t) - u_2(t) \sim \frac{\log t}{t^2}
$$
从而
$$
u(t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + \frac{\log t}{t^2} + o_2\left( \frac{\log t}{t^2} \right)
$$
返回原始问题后，得到渐近展开
$$
v(x) = x \log x + x \log \log x + x \frac{\log \log x}{\log x} + o\left( x \frac{\log \log x}{\log x} \right).
$$

#### 注 {#fvr-v-a0-n6-rem-4 .statement tag=08H8}

注两个等价 (H) 函数可以具有非等价的逆元，如两个函数 $\log x$ 和 $1 + \log x$ 的例所示。

### 习题{#fvr-v-a0-exercises}

请参阅[习题附录 0](exercises/a0/)。
