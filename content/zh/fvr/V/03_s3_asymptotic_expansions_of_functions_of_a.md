---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 3
section_title: ASYMPTOTIC EXPANSIONS OF FUNCTIONS OF A REAL VARIABLE
lang: zh
source: fvr-i-vii
book_pages: 227-236, 260-261
pdf_pages: 0242-0251, 0275-0276
extraction: ocr
subsections:
    - "no": 1
      title: 'INTEGRATION OF COMPARISON RELATIONS: **I. WEAK RELATIONS**'
      page: 228
      pdf_page: 243
    - "no": 2
      title: 'APPLICATION: LOGARITHMIC CRITERIA FOR CONVERGENCE OF INTEGRALS'
      page: 229
      pdf_page: 244
    - "no": 3
      title: 'INTEGRATION OF COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 230
      pdf_page: 245
    - "no": 4
      title: DIFFERENTIATION OF COMPARISON RELATIONS
      page: 232
      pdf_page: 247
    - "no": 5
      title: PRINCIPAL PART OF A PRIMITIVE
      page: 233
      pdf_page: 248
    - "no": 6
      title: ASYMPTOTIC EXPANSION OF A PRIMITIVE
      page: 235
      pdf_page: 250
statements: 24
exercises: 7
content_sha256: d38f02ad478e84838065670eadf49b051038da954531473e58972d321dce83f1
translated_from: content/en/fvr/V/03_s3_asymptotic_expansions_of_functions_of_a.md
translation_method: google
source_content_sha256: 8e759b487c91cd2169288cb7a854bc7596023e144f6eac992de79d1711257975
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: c5d8003ca10642f0312a47df1f2178a597bac62c0d367503bb7fd2bcc8888bbf
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。实变量函数的渐近展开

在这个截面中，我们将仅考虑以下情况：集合$E$是扩展实直线$\overline{\mathbf{R}}$中的开区间，并且$\mathfrak{F}$是基，对于左侧或右侧端点$\alpha$的邻域滤波器的$E$上的迹$E$；此外，我们将首先研究$\mathfrak{F}$中集合定义的（有限）实数函数（取决于所考虑的函数）。

根据需要使用变量$x' = -x,\ x' = \frac{1}{x-\alpha},\ x' = -\frac{1}{x-\alpha}$的变换之一，对于E为区间形式]$a, +\infty[$的情况，总是可以约化，这样$\mathfrak{F}$将由区间$[t, +\infty[$和$t > a$组成。我们将主要局限于后一种情况，并将翻译我们获得的大部分命题（通过上述变量变换）的任务留给读者，除了一些特别重要的结果。

滥用语言将$\mathfrak{F}$中的集合称为“$+\infty$的邻域”会很方便。

### 1.比较整合关系：**I。弱关系**

#### 命题 1 {#fvr-v-s3-prop-1 .statement tag=08F4}

*令 $\mathbf{f}$ 为调节的向量函数，$g$ 为间隔 $[a, +\infty[$ 上的调节的函数 $\geqslant 0$，使得 $\int_a^{+\infty} g(t)\,dt > 0$。 关系 $\mathbf{f} \preccurlyeq g$ 因为 $x$ 倾向于 $+\infty$ 意味着$\int_a^x \mathbf{f}(t)\,dt \preccurlyeq \int_a^x g(t)\,dt$。如果积分 $\int_a^{+\infty} g(t)\,dt$ 收敛，则积分 $\int_a^{+\infty} \mathbf{f}(t)\,dt$ 绝对收敛。*

事实上，到假设时，存在 $b \geqslant a$ 和数 $c' > 0$，使得
$$
\| \mathbf{f}(x) \| \leqslant c' g(x) \quad \text{for } x \geqslant b,
$$
从而
$$
\left\| \int_b^x \mathbf{f}(t)\,dt \right\| \leqslant \int_b^x \| \mathbf{f}(t) \| \,dt \leqslant c' \int_b^x g(t)\,dt;
$$
此外，因为人们可能会假设$b$大到$\int_a^b g(t)\,dt > 0$，所以存在一个$c'' > 0$使得$\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leqslant c'' \int_a^b g(t)\,dt$；因此，在放入 $c = \max(c', c'')$ 时，有
$$
\left\| \int_a^x \mathbf{f}(t)\,dt \right\| \leqslant c \int_a^x g(t)\,dt
$$
每$x \geqslant b$、从而命题。

#### 推出 1 {#fvr-v-s3-prop-1-cor-1 .statement tag=08F5}

*如果$f$和$g$在区间$[a, +\infty[$上调节函数和$\geqslant 0$，则$f \succcurlyeq g$，如果$\int_a^{+\infty} g(t)\,dt = +\infty$，则$\int_a^{+\infty} f(t)\,dt = +\infty$。*

#### 推出 2 {#fvr-v-s3-prop-1-cor-2 .statement tag=08F6}

*如果$f$和$g$是$\geqslant 0$，并且$[a, +\infty[$上的零不相同，并且$f \succeq g$，则$\int_a^x f(t)\,dt \succeq \int_a^x g(t)\,dt$。*

### 2. 应用：积分收敛的对数判据

通过适当选择函数g，可以从prop推导出判据来决定函数$f \geq 0$的积分$\int_a^{+\infty} f(t) \, dt$是否收敛或无穷大。 V、p. 228 和相关的 1 个。 1 至此：对于原语已知的 g 函数来说，选择就足够了。特别是，由于$x^\mu$在$\mu \neq -1$时具有原语$\frac{x^{\mu+1}}{\mu+1}$，在$\mu = -1$时具有$\log x$，因此我们有以下标准：

#### 命题 2（“阶 0 的对数准则”）{#fvr-v-s3-prop-2 .statement tag=08F7}

*设 f 为区间 $[a, +\infty[$ 上的调节函数 $\geq 0$；如果$f(x) \preccurlyeq x^\mu$对于某些$\mu < -1$则积分$\int_a^{+\infty} f(t) \, dt$收敛；如果 $f(x) \succcurlyeq x^\mu$ 对于某些 $\mu \geq -1$ 那么积分 $\int_a^{+\infty} f(t) \, dt$ 是无限的。*

当$1/x^{1+\alpha} \ll f(x) \ll 1/x$对于*每个*指数$\alpha > 0$时，这个标准不是决定性的，对于例，当$f(x) = 1/x(\log x)^\mu$（$\mu > 0$）时。但在最后一种情况下，如果 $\mu \neq 1$，则 f 具有原语 $\frac{1}{1-\mu} (\log x)^{1-\mu}$；当 $\mu = 1$ 时，f 有原语 $\log \log x$。因此：

#### 命题 3（“阶 1 的对数准则”）{#fvr-v-s3-prop-3 .statement tag=08F8}

*设 f 为区间 $[a, +\infty[$ 上的调节函数 $\geq 0$；如果$f(x) \preccurlyeq 1/x(\log x)^\mu$对于某些$\mu > 1$则积分$\int_a^{+\infty} f(t) \, dt$收敛；如果 $f(x) \succcurlyeq 1/x(\log x)^\mu$ 对于某些 $\mu \leq 1$ 那么积分 $\int_a^{+\infty} f(t) \, dt$ 是无限的。*

一般地，对于每个整数$n \geq 0$，让我们用$l_n(x)$函数来表示，关系$l_0(x) = x$归纳定义（对于x足够大），$l_n(x) = \log(l_{n-1}(x))$对于$n \geq 1$;有人说 $l_n(x)$ 是 x* 的*n*次*迭代对数（cf. 附录）。人们立即验证 $\frac{1}{1-\mu} (l_n(x))^{1-\mu}$ 是一个原语

$$
\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}
$$

对于$\mu \neq 1$，$l_{n+1}(x)$是$\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) l_n(x)}$的原语。因此：

#### 命题 4（“阶 n 的对数准则”）{#fvr-v-s3-prop-4 .statement tag=08F9}

*设 f 为区间 $[a, +\infty[$ 上的调节函数 $\geq 0$；如果，对于某些$\mu > 1$，$f(x) \preccurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}$，则积分$\int_a^{+\infty} f(t) \, dt$收敛；如果 $f(x) \succcurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}$ 对于某些 $\mu \leq 1$，则积分 $\int_a^{+\infty} f(t) \, dt$ 是无限的。*

因此，每个对数标准适用于函数，其中阶中的判据不是决定性的（*cf.* V、p. 264，执行 5 b）和 V、p. 265，执行。 8).

由于它的实用性，我们将阶 0 的标准转换为积分 $\int_{\alpha}^{a} f(t) \, dt$，其中 $f$ 受到调节，而 $\geq 0$ 则转换为非紧区间 $]\alpha, a]$：

#### 命题 5（“阶 0 的对数标准”）{#fvr-v-s3-prop-5 .statement tag=08FA}

*如果在$\alpha$的邻域上，对于某些$\mu < 1$有$f(x) \leq 1/(x-\alpha)^{\mu}$，则积分$\int_{\alpha}^{a} f(t) \, dt$收敛；如果 $f(x) \geq 1/(x-\alpha)^{\mu}$ 对于某些 $\mu \geq 1$ 那么积分 $\int_{\alpha}^{a} f(t) \, dt$ 是无限的。*

我们留给读者类似地翻译阶$n$的对数准则。

如果知道如何获得 $f$ 的*本金部分* 相对于这些判据中的特征的比较标度包含函数，则对数判据的应用为直接的：如果 $f_1$ 是本金部分，整的$\int_{\alpha}^{+\infty} f(t) \, dt$与$\int_{\alpha}^{+\infty} f_1(t) \, dt$一起收敛或无穷大，对数判据立即应用于最后一个积分。

#### 例 1 {#fvr-v-s3-n2-exa-1 .statement tag=08FB}

当$p < 0$或$q < 0$时，函数$t^p(1-t)^q$不受$]0, 1[$限制；通过对点 0 和 1 的邻域应用阶 0 的对数准则，整的$\int_{0}^{1} t^p(1-t)^q \, dt$收敛当且仅当$p > -1$和$q > -1$。如果是这样，则该积分称为*第一类欧拉积分*，并用 $\mathbf{B}(p+1, q+1)$ (*cf.* VII, p. 312) 表示。

#### 例 2 {#fvr-v-s3-n2-exa-2 .statement tag=08FC}

考虑积分$\int_{0}^{+\infty} t^{\lambda-1} e^{-t} \, dt$。由于邻域上的 $e^{-t} \sim 1$ 为 0，因此如果该积分要收敛，则必须有 $\lambda > 0$；这个条件也足够了，因为在$+\infty$的邻域上，对于任何$\mu > 0$，都有$e^{-t} \ll t^{-\mu}$。当 $x > 0$ 时，积分称为*第二类欧拉积分*，记为 $\Gamma(x)$ (*cf.* VII, p. 311)。

### 3.比较整合关系：II。强关系

#### 命题 6 {#fvr-v-s3-prop-6 .statement tag=08FD}

*设 $\mathbf{f}$ 为受监管的向量函数，而 $g$ 为 $[a, +\infty[$ 上受监管的函数 $\geq 0$。*

1. *如果积分 $\int_{a}^{+\infty} g(t) \, dt$ 收敛，则关系 $\mathbf{f} \ll g$（分别为 $\mathbf{f} \sim c g$，其中 $c$ 为常数）意味着 $\int_{x}^{+\infty} \mathbf{f}(t) \, dt \ll \int_{x}^{+\infty} g(t) \, dt$（分别为 $\int_{x}^{+\infty} \mathbf{f}(t) \, dt \sim c \int_{x}^{+\infty} g(t) \, dt$）。

2. *如果积分 $\int_{a}^{+\infty} g(t) \, dt$ 是无穷大，则关系 $\mathbf{f} \ll g$（或 $\mathbf{f} \sim c g$）意味着*
$$
\int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \ll \int_{\beta}^{\gamma} g(t) \, dt \quad \text{(resp. } \int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \sim c \int_{\beta}^{\gamma} g(t) \, dt),
$$
*对于$[a, +\infty[$中的任何$\alpha$和$\beta$*。

证明命题对于关系$\mathbf{f} \ll g$就足够了，因为如果$c \neq 0$，关系$\mathbf{f} \sim c g$等价于$\mathbf{f} - c g \ll g$。

第一个部分是平均值定理的直接的推论，因为如果$\| \mathbf{f}(x) \| \leq \varepsilon g(x)$对于$x \geq x_0$可以推断出：

$$
\left\| \int_{x}^{+\infty} \mathbf{f}(t) \, dt \right\| \leq \int_{x}^{+\infty} \| \mathbf{f}(t) \| \, dt \leq \varepsilon \int_{x}^{+\infty} g(t) \, dt \quad \text{for } x \geq x_0.
$$

其次，假设$\int_{a}^{+\infty} g(t) \, dt = +\infty$。如果 $\| \mathbf{f}(x) \| \leq \varepsilon g(x)$ 对应 $x \geq x_0 \geq \max(\alpha, \beta)$，则有

$$
\begin{align*}
\int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt &= \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \int_{x_0}^{x} \| \mathbf{f}(t) \| \, dt \\
&\leq \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \varepsilon \int_{x_0}^{x} g(t) \, dt \\
&= \varepsilon \int_{\beta}^{x} g(t) \, dt + \left( \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right).
\end{align*}
$$

现在存在一个$x_1 \geq x_0$，对于每个$x \geq x_1$

$$
\left| \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right| \leq \varepsilon \int_{\beta}^{x} g(t) \, dt
$$

从而, $x \geq x_1$

$$
\left\| \int_{\alpha}^{x} \mathbf{f}(t) \, dt \right\| \leq \int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt \leq 2\varepsilon \int_{\beta}^{x} g(t) \, dt
$$

完成证明，因为$\varepsilon > 0$是任意的。

在其他字中，当$g$在间隔$[a, +\infty[$上为正时，可以整合强关系$\mathbf{f} \ll g$、$\mathbf{f} \sim \mathbf{a}g$的两个项，并且关系持续存在于两个项的原语之间，前提是要注意从如果$\int_{a}^{+\infty} g(t) \, dt$收敛，则从$x$到$+\infty$，反之则从$\alpha$到$x$（对于$[a, +\infty[$中的任何$\alpha$）。

注那个道具。当$\mathfrak{F}$为基时，对于可数集合的补集上的间隔$[t, +\infty[$（其中$t > a$）的跟踪过滤器，1（V，p. 228）和6（V，p. 230）仍然有效（cf.I，p. 15，第 2 个）。

#### 例 1 {#fvr-v-s3-n3-exa-1 .statement tag=08FE}

在应用支柱上。 V，p. 230，到关系$1/x \ll x^{\alpha-1}$，其中$\alpha > 0$，每$\alpha > 0$再次获得关系$\log x \ll x^{\alpha}$，相当于关系$y^{1/\alpha} \ll e^y$证明III，p. 105。

#### 例 2 {#fvr-v-s3-n3-exa-2 .statement tag=08FF}

我们有$\left( \frac{e^t}{x} \right)' = \frac{e^t}{x} \left( 1 - \frac{1}{x} \right) \sim e^t / x$；由于 $e^t / x$ 与 $x$ 趋向于 $+\infty$，因此可以从 prop 推导出来。 6 个V、p. 230、$\int_{1}^{x} \frac{e^t}{t} \, dt \sim e^x / x$。

#### 注 {#fvr-v-s3-n3-rem-1 .statement tag=08FG}

当$g$不被假设在区间$[a, +\infty[$上保持$\geq 0$（或在这样的区间上保持$\leq 0$），并且$\int_{a}^{+\infty} g(t) \, dt$不收敛时，关系$f \sim g$不一定意味着$\int_{a}^{x} f(t) \, dt \sim \int_{a}^{x} g(t) \, dt$，如例所示其中 $g(x) = \sin x$ 和 $f(x) = \left( 1 + \frac{\sin x}{x} \right) \sin x$；这里

$$
\int_{n\pi}^{(n+1)\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{(n+1)\pi} \int_{0}^{\pi} \sin^2 t \, dt \geq \frac{1}{2} \int_{n+1}^{n+2} \frac{dt}{t},
$$

从而
$$
\int_{\pi}^{n\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{2} \int_2^{n+1} \frac{dt}{t}
$$
并且积分 $\int_1^{+\infty} dt/t$ 是无限的，虽然 $\int_{\frac{\pi}{2}}^x g(t) \, dt = -\cos x$ 仍然有界（参见 V、p. 260、练习 4）。

### 4. 比较差异关系

命题 1 (V, p. 228) 和 6 (V, p. 230) 不具有逆命题：两个函数之间存在可微分的比较关系 $f \preccurlyeq g,\ f \ll g,\ f \sim cg$ $+\infty$的邻域并不意味着它们的导数之间有相同的关系比较，即使对于真正的单调函数$f$和$g$也是如此。

对于例，函数$x^2 + x \sin x + \cos x$是单调的，等价于$x^2$，但它的导数$x(2 + \cos x)$不等价于$2x$。

另一方面，当人们先验地假设所考虑的函数的导数是可比较的（V，p. 217）时，就可以推导出比较关系。一般来说，我们可以说，在区间 $[a, +\infty[$ 上定义的两个实数函数 $f$ 和 $g$ 相当于 $+\infty$ 的邻域上的阶 $k$，如果，在邻域上$+\infty$，除了点的可数集合之外，它们各自都有受管制的$k^{th}$导数，并且如果在此邻域、$f^{(k)}$和$g^{(k)}$具有常数符号（在定义它们的集合上）并且可比较。

我们同意说两个可比较的实函数（V，p. 217）可比较阶 0。

#### 命题 7 {#fvr-v-s3-prop-7 .statement tag=08FH}

如果两个实数函数$f,\ g$，阶1具有可比性，则它们具有可比性；此外，关系$f \ll g$（分别$f \sim cg$、$c$常数）意味着$f' \ll g'$（分别$f' \sim cg'$）除非$g$等价于非零的常数。

现在，由于$f'$和$g'$在区间$[x_0, +\infty[$上具有恒定符号，$f$和$g$在该区间上都是单调的，因此趋向于有限或无限极限，就像$x$趋向于$+\infty$一样。显然，$f$ 和 $g$ 具有可比性，因为如果极限之一是有限的而 $\neq 0$，或者如果一个是零而另一个是无限的，则 $x$ 趋于 $+\infty$。如果$f$和$g$都趋于0，可以写成$f(x) = -\int_x^{+\infty} f'(t) \, dt,\ g(x) = -\int_x^{+\infty} g'(t) \, dt$；由于$f'$和$g'$具有可比性，$f$和$g$也是如此，$f$和$g$之间的比较关系与$f'$和$g'$之间的比较相同。 6（V，p. 20）。类似地，如果$f$和$g$都有一个无限的极限，其中一个有$f(x) = f(x_0) + \int_{x_0}^x f'(t) \, dt,\ g(x) = g(x_0) + \int_{x_0}^x g'(t) \, dt$；再次支持。 6（V，p. 230）表明$f$和$g$是可比较的，$f$和$g$之间的比较关系与$f'$和$g'$之间的比较相同。为了完成证明，还需要考虑$g$趋向于$\pm \infty$和$f$为常数的情况：一个不能然后有$f' \succcurlyeq g'$，因为这样就可以从prop推出。 1 (V, p. 218) 整的$\int_{x_0}^{+\infty} g'(t) \, dt$收敛；由于假设 $f'$ 和 $g'$ 具有可比性，因此必须具有 $f' \ll g'$。

#### 推论{#fvr-v-s3-n4-cor-1 .statement tag=08FI}

*如果两个实数函数$f, g$，阶$k \geqslant 1$具有可比性，那么它们对于$0 \leqslant p \leqslant k$可具有阶$p$可比性；此外，关系$f \ll g$（分别$f \sim cg$）意味着$f^{(k)} \ll g^{(k)}$（分别$f^{(k)} \sim cg^{(k)}$）除非导数之一$g^{(p)}$（$0 \leqslant p \leqslant k - 1$）相当于常数$\neq 0$。

事实上，由于$f^{(k)}$和$g^{(k)}$在区间$[x_0, +\infty[$上具有常数符号，因此$f^{(k-1)}$和$g^{(k-1)}$在该区间上是单调的，因此在$+\infty$的邻域上具有常数符号；此外，道具。 V、p. 232 的 7 表明 $f^{(k-1)}$ 和 $g^{(k-1)}$ 具有可比性，因此推论来自应用命题。 7 递归。

#### 注 1 {#fvr-v-s3-n4-rem-1 .statement tag=08FJ}

限制在 $g$ 上。 7是必不可少的。对于例，有$\frac{1}{x} \ll 1 + \frac{1}{x}$甚至虽然，两边的导数是等价的；类似地$1 + \frac{1}{x} \sim 1 + \frac{1}{x^2}$，但是$1/x^2 \gg 2/x^3$。

#### 注 2 {#fvr-v-s3-n4-rem-2 .statement tag=08FK}

虽然 $f$ 和 $g$ 可与阶 $k$ 进行比较函数 $f_1$ 相当于 $f$ 无需将阶 $k$ 与 $g$ 进行比较；然而，如果假设 $f_1$ 与阶 $k$ 和 $f$ 具有可比性，并且没有一个导数 $f^{(p)}$ ($0 \leqslant p \leqslant k - 1$) 等同于非零的常数。

#### 注 3 {#fvr-v-s3-n4-rem-3 .statement tag=08FL}

如果 $f$ 和 $g$ 与阶 $k$ 具有可比性，那么对于 $hf$ 和 $hg$ 就不必如此，即使对于单调函数 $h$ 就像 $h(x) = x$ (V, p. 260，练习3）；同样，$1/f$和$1/g$不一定与阶$k$具有可比性（V、p. 259，练习1）。

### 5. 原语的部分

令 $f$ 为在区间 $[a, +\infty[$ 上具有常数符号的调节实数函数 $\neq 0$；如果$\int_a^{+\infty} f(t)\,dt$在某些情况下收敛，则以下命题允许获得原语$\int_a^{+\infty} f(t)\,dt$的本金部分，如果$\int_a^{+\infty} f(t)\,dt$是无限的，则可以获得原语$\int_a^x f(t)\,dt$的本金：

#### 命题 8 {#fvr-v-s3-prop-8 .statement tag=08FM}

*把* $F(x) = \int_x^{+\infty} f(t)\,dt$ *如果* $\int_a^{+\infty} f(t)\,dt$ *收敛*，*并且* $F(x) = \int_a^x f(t)\,dt$ *如果* $\int_a^{+\infty} f(t)\,dt$ *是无限的*。 *假设* $\log|f|$ *和* $\log x$ *相当于阶* 1。

1 *如果* $f$ *有限阶* $\mu \neq -1$ *相对于* $x$ *一个有*
$$
F(x) \sim \frac{1}{|\mu+1|} x f(x).
$$
(1)

2 *如果* $f$ *相对于* $x$ *具有无限阶 *并且如果* $f/f'$ *和* $x$ *可与阶* 1 进行比较，*则有*
$$
F(x) \sim \frac{(f(x))^2}{|f'(x)|}.
$$
(2)

人们应该注，假设意味着$f(x)$相对于$x$（V，p. 219）有一个确定的阶。

1 *如果* $f$ *属于阶* $\mu \neq 0$ *相对于* $x$ *一个有* $\log|f| \sim \mu \log x$，*所以，因为* $\log|f|$ *和* $\log x$ *可与阶* 1 进行比较，*通过道具。 7 个V，p. 232 其中一个有* $f'/f \sim$ μ/x，从而 $x f' \sim \mu f$。如果 $\mu > -1$ 对于每个 $\varepsilon > 0$ 都有 $f(x) \gg x^{\mu-\varepsilon}$，因而（V，p. 229，道具 2）整的 $\int_a^{+\infty} f(t)\,dt$ 是无限的。可以再写$F(x) = \int_a^x f(t)\,dt = x f(x) - af(a) - \int_a^x t f'(t)\,dt$、从而
$$
\int_a^x (f(t) + t f'(t))\,dt = x f(x) - af(a);
$$
因为$\mu \neq -1$我们有$f(x) + x f'(x) \sim (\mu + 1) f(x)$，所以（V，p. 230，道具6）
$$
\int_a^x (f(t) + t f'(t))\,dt \sim (\mu + 1) F(x),
$$
在这种情况下证明了（1）。如果$\mu = 0$同样有$x f'(x) \ll f(x)$，它又给出$f(x) + x f'(x) \sim f(x)$。当 $\mu < -1$ 时，在 $\int_a^{+\infty} f(t)\,dt$ 收敛的情况下，人们也有类似的争论。

2) 如果$f$相对于$x$来说是阶$+\infty$，那么一个人有$\log |f| \gg \log x$，那么（V，p. 232，道具7）$f'/f \gg 1/x$，或者再次，放入$g(x) = f(x)/f'(x)$，$g(x) \ll x$；此外，由于$f(x) \gg x^\alpha$对于每个$\alpha > 0$，整的$\int_a^{+\infty} f(t)\,dt$是无限的。一个人可以写
$$
F(x) = \int_a^x f(t)\,dt = \int_a^x g(t) f'(t)\,dt = g(x) f(x) - g(a) f(a) - \int_a^x f(t) g'(t)\,dt;
$$
由于 $g$ 和 $x$ 与阶 1 相当，从关系 $g(x) \ll x$ 可以推出（V，p. 232，命题 7）$g'(x) \ll 1$，因而$f g' \ll f$，因而（V，p. 230，道具 6）
$$
\int_a^x f(t) g'(t)\,dt \ll F(x),
$$
从而建立关系 (2)。当$f$相对于$x$为阶$-\infty$时，证明是相似的，在$\int_a^{+\infty} f(t)\,dt$收敛的情况下。

令 $\mathscr{E}$ 为比较尺度（对于趋向于 $+\infty$ 的实数 $x$），由非零的实数函数组成，其在 $+\infty$ 的邻域上具有恒定符号，使得 $x \in \mathscr{E}$ 且使得乘积和 2 的商函数再次从$\mathscr{E}$属于到$\mathscr{E}$（V、p. 221和p. 224）。如果函数$f$在$+\infty$的邻域上有常数符号，相对于$\mathscr{E}$有一个本金部分$c g$，则$\int_x^{+\infty} f(t)\,dt$（根据情况分别为$\int_a^x f(t)\,dt$）将等于$c \int_x^{+\infty} g(t)\,dt$ （分别$c \int_a^x g(t)\,dt$）；如果函数 $g$ 满足 prop 的假设。 V、p. 233 的 8，并且如果（当V、p. 233 的公式 (2) 适用时）人们知道相对于 $\mathscr{E}$ 的本金部分为 $g'$，因此，人们将拥有本金部分 $\int_x^{+\infty} f(t)\,dt$（分别为$\int_a^x f(t)\,dt$）相对于$\mathscr{E}$。

#### 例 1 {#fvr-v-s3-n5-exa-1 .statement tag=08FN}

函数 $1/\log x$ 相对于 $x$ 为阶 0 并且满足 prop 的条件。 8 个V、p. 233；因此
$$
\int_a^x \frac{dt}{\log t} \sim \frac{x}{\log x}.
$$

#### 例 2 {#fvr-v-s3-n5-exa-2 .statement tag=08FO}

函数 $e^{t^2}$ 相对于 $x$ 具有阶 $+\infty$ 且满足 prop 的条件。 8、所以
$$
\int_a^x e^{t^2}\,dt \sim \frac{1}{2x}\,e^{x^2}.
$$

在附录 (V, p. 252) 中，我们将函数的定义集合用作哪个道具。 7 和支柱。 8 始终适用。

#### 注 {#fvr-v-s3-n5-rem-1 .statement tag=08FP}

提案 8 并不直接适用于阶 $-1$ 相对于 $x$ 的函数 $f$。但是可以写 $f(x) = f_1(x)/x$，$f_1$ 相对于 $x$ 为阶 0。假设，对于例，$\int_a^{+\infty} f(t)\,dt$是无限的；然后

$$
F(x) = \int_a^x f(t)\,dt = \int_a^x \frac{1}{t} f_1(t)\,dt = \int_{\log a}^{\log x} f_1(e^u)\,du.
$$

如果函数 $f_1(e^t)$ 满足 prop 的假设。 8 并且相对于$y$有阶$\neq -1$（也就是说，如果$f_1(x)$相对于$\log x$有阶$\neq -1$）公式（1）和（2）再次允许我们获得本金部分 $F(x)$。对于例，设$f(x) = \frac{\exp(\sqrt{\log x})}{x \log x}$；因为$\exp(\sqrt{\log x})$相对于$x$是阶0，$f$是阶$-1$；这里有 $f_1(e^t) = e^{\sqrt{t}}/y$，而这个函数相对于 $y$ 是阶 $+\infty$；支柱。 8 应用并给出$\int_a^x e^{\sqrt{u}}/u\,du \sim 2e^{\sqrt{y}}/\sqrt{y}$：恢复到变量$x$，我们有$\int_a^x \frac{\exp(\sqrt{\log t})}{t \log t}\,dt \sim \frac{2\exp(\sqrt{\log x})}{\sqrt{\log x}}$。

### 6.原语的渐近展开

令$\mathscr{E}$为$+\infty$与邻域的比较标尺，由$+\infty$的邻域上的常号实数函数$\neq 0$组成；设 $\mathbf{f}$ 是在区间 $[a,\,+\infty[$ 上定义的受规向量函数，其中值位于完全规范的空间 $E$ 中，承认渐近展开

$$
\mathbf{f} = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda + \mathbf{r}_\alpha
$$

相对于 $\mathscr{E}$ 的精度为 $g_\alpha$。进一步假设函数$g \in \mathscr{E}$的每个本原$\int_a^x g(t)\,dt$都承认关于$\mathscr{E}$的渐近展开。在这些情况下，我们将看到相对于$\mathscr{E}$可以获得$F(x) = \int_a^x \mathbf{f}(t)\,dt$的渐近展开。我们区分两种情况：

1. $\int_a^{+\infty} g_\alpha(t)\,dt$是无穷大；那么就有 $\int_a^x \mathbf{r}_\alpha(t)\,dt \ll \int_a^x g_\alpha(t)\,dt$ (V, p. 230, 命题 6)；通过假设可以得到$\sum_{\lambda \leq \alpha} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt$的渐近展开达到一定精度$g_\rho$（V，p. 222）；如果$c g_\sigma$是$\int_a^x g_\alpha(t)\,dt$的主要部分，那么将有一个$\int_a^x \mathbf{f}(t)\,dt$的渐近展开精确到$g_{\min(\rho,\sigma)}$，所有项都无限期地具有递增范数。

2. $\int_a^{+\infty} g_\alpha(t)\,dt$收敛；设$\beta$为指标$\lambda \leq \alpha$的最小的，使得$\mathbf{a}_\lambda \neq 0$且$\int_a^{+\infty} g_\lambda(t)\,dt$收敛；整的

$$
C = \int_a^{+\infty} \left( \mathbf{f}(t) - \sum_{\lambda < \beta} \mathbf{a}_\lambda g_\lambda(t) \right) dt
$$

然后收敛，可以写出

$$
F(x) = \sum_{\lambda < \beta} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt + C - \sum_{\beta \leq \lambda \leq \alpha} \mathbf{a}_\lambda \int_a^{+\infty} g_\lambda(t)\,dt - \int_a^{+\infty} \mathbf{r}_\alpha(t)\,dt.
$$

然后$\int_a^{+\infty} r_\alpha(t) \, dt \ll \int_1^{+\infty} g_\alpha(t) \, dt$；如果 $c g_\sigma$ 是 $\int_1^{+\infty} g_\alpha(t) \, dt$ 的主部分，并且如果有一个渐近展开

$$
\sum_{\lambda < \beta} a_\lambda \int_a^\lambda g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda \leq \alpha} a_\lambda \int_\lambda^{+\infty} g_\lambda(t) \, dt
$$

对于精度 $g_\rho$，结果将是 $F$ 到精度 $g_{\min(\rho, \sigma)}$ 的渐近展开。

因此，这一切都相当于找到关于 * $\mathscr{E}$ 中函数的原语 $\mathscr{E}$ 的渐近展开。我们已经看到，根据 $\mathscr{E}$ 的某些假设，道具。 V、p. 233 的 8 给出了这样一个原语的本金部分。此外，道具的证明。 8 给出了函数 $\frac{1}{|\mu + 1|} (x f'(x) + f(x)) - f(x)$（分别为 $f(x) g'(x)$ 和 $g = f/f'$）基元的形式中 V、p. 233 的公式 (1)（分别为 (2)）两侧的差值表达式；在形成这个新原语的主部分时，作为（1）（或（2））右侧的渐近展开，我们获得了所寻求的展开的右侧（参见V，p. 247-255）。

#### 例 1 {#fvr-v-s3-n6-exa-1 .statement tag=08FQ}

令 $f(x) = 1/\log x$ ($x > 1$);我们已经看到了$\int_a^\lambda dt / \log t \sim x / \log x$，并且差值$\int_a^\lambda \frac{dt}{\log t} - \frac{\lambda}{\log \lambda}$是$1/(\log x)^2$的原语；可以应用道具。再次对这个函数进行8，因此得到$\int_a^\lambda dt / (\log t)^2 \sim x / (\log x)^2$。通过递归可以得到展开

$$
\int_a^\lambda \frac{dt}{\log t} = \frac{x}{\log x} + \frac{x}{(\log x)^2}
+ \frac{2x}{(\log x)^3} + \cdots + (n-1)! \frac{x}{(\log x)^n} + o \left( \frac{x}{(\log x)^n} \right).
$$

注，无论$n$如何，这个展开的所有项都倾向于$+\infty$和$x$。

#### 例 2 {#fvr-v-s3-n6-exa-2 .statement tag=08FR}

让$f(x) = \frac{e^x}{x^2 + 1}$；可以写$f(x) = \frac{e^x}{x^2} - \frac{e^x}{x^4} + o_1 \left( \frac{e^x}{x^4} \right)$。道具 8 给出展开

$$
\int_a^\lambda \frac{e^t}{t^2} \, dt = \frac{e^x}{x^2} + \frac{2e^x}{x^3} + \frac{6e^x}{x^4} + o_2 \left( \frac{e^x}{x^4} \right), \quad \int_a^\lambda \frac{e^t}{t^4} \, dt = \frac{e^x}{x^4} + o_3 \left( \frac{e^x}{x^4} \right)
$$

从而，添加后，

$$
\int_a^\lambda \frac{e^t}{t^2 + 1} \, dt = \frac{e^x}{x^2} + 2 \frac{e^x}{x^3} + 5 \frac{e^x}{x^4} + o_4 \left( \frac{e^x}{x^4} \right).
$$

### 习题{#fvr-v-s3-exercises}

§ 3](exercises/s3/)参见[习题。
