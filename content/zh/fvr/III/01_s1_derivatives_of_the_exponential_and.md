---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 1
section_title: DERIVATIVES OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS
lang: zh
source: fvr-i-vii
book_pages: 91-104, 115-125
pdf_pages: 0106-0119, 0130-0140
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF THE EXPONENTIAL FUNCTIONS; THE NUMBER $e$
      page: 91
      pdf_page: 106
    - "no": 2
      title: DERIVATIVE OF $\log_a x$
      page: 93
      pdf_page: 108
    - "no": 3
      title: DERIVATIVES OF THE CIRCULAR FUNCTIONS; THE NUMBER $\pi$
      page: 94
      pdf_page: 109
    - "no": 4
      title: INVERSE CIRCULAR FUNCTIONS
      page: 95
      pdf_page: 110
    - "no": 5
      title: THE COMPLEX EXPONENTIAL
      page: 97
      pdf_page: 112
    - "no": 6
      title: PROPERTIES OF THE FUNCTION $e^z$
      page: 98
      pdf_page: 113
    - "no": 7
      title: THE COMPLEX LOGARITHM
      page: 100
      pdf_page: 115
    - "no": 8
      title: PRIMITIVES OF RATIONAL FUNCTIONS
      page: 101
      pdf_page: 116
    - "no": 9
      title: COMPLEX CIRCULAR FUNCTIONS; HYPERBOLIC FUNCTIONS
      page: 102
      pdf_page: 117
statements: 9
exercises: 39
content_sha256: e2413fed206d04f068008ef1521fd745c91a43486b41a7af5cafc687220ddd16
translated_from: content/en/fvr/III/01_s1_derivatives_of_the_exponential_and.md
translation_method: google
source_content_sha256: 4ac8e46f4200ac7e7f332753e43fe2ec6dc6c4857b2b82b1a42df8d051c7b1e2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4fdafe7fd69f5667602a1318858b11d656e7de4e459a8cc7ac7abdfc3eae8f69
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。指数和循环函数的导数

### 1. 指数函数的导数； 数$e$

我们知道，加法群$\mathbf{R}$的每个连续同态到实数$\neq 0$的乘法群$\mathbf{R}^*$都是形式$x \mapsto a^x$的函数（称为指数函数），其中$a$是数$> 0$（TG，V，p.11）；如果$a \neq 1$，则为$\mathbf{R}$的同构到乘法群，数$> 0$的$\mathbf{R}_+^*$，而从$\mathbf{R}_+^*$到$\mathbf{R}$的逆同构用$\log_a x$表示，称为基 $a$ 的对数。

我们将看到，对于每个$x \in \mathbf{R}$，函数$f(x) = a^x$都有形式$c.a^x$的导数（显然是$c = f'(0)$）。这是由以下一般定理得出的结果：

#### 定理 1 {#fvr-iii-s1-thm-1 .statement tag=089Q}

*设 E 为域 $\mathbf{R}$ 上的完全范数代数，其中单位元 $\mathbf{e}$，并令 $\mathbf{f}$ 为加法群 $\mathbf{R}$ 到乘法群 G 的连续群同态 E 的可逆元。则映射 $\mathbf{f}$ 在每个 $x \in \mathbf{R}$ 处可微，并且*

$$
\mathbf{f}'(x) = \mathbf{f}(x)\mathbf{f}'(0).
$$

首先我们注，E是一个完整的代数，G在E中开（*Gen.Top.*，IX，p. 179，道具14）。考虑函数$g(x) = \int_0^a \mathbf{f}(x + t)\,dt$，其中$a > 0$是数，稍后我们将选择；从$\mathbf{f}(x + t) = \mathbf{f}(x)\mathbf{f}(t)$到假设，我们有$g(x) = \int_0^a \mathbf{f}(x)\mathbf{f}(t)\,dt = \mathbf{f}(x) \int_0^a \mathbf{f}(t)\,dt$（I，p. 6，道具3）。令$\alpha > 0$使得球$\|x - \mathbf{e}\| \leq \alpha$包含在G中；由于$\mathbf{f}(0) = \mathbf{e}$和$\mathbf{f}$通过假设连续，我们可以假设$a$足够小，使得$\|\mathbf{f}(t) - \mathbf{e}\| \leq \alpha$在$[0, a]$上；因而 (II, p. 61, 公式 (16)) 有

$$
\left\| \frac{1}{a} \int_0^a \mathbf{f}(t)\,dt - \mathbf{e} \right\| \leq \alpha,
$$

和 $\frac{1}{a} \int_0^a f(t) \, dt$ 属于至 G；在其他字中，是可逆的； $b = \int_0^a f(t) \, dt$也是如此，可以写$f(x) = g(x)b^{-1}$；因而，只要证明 g 可微即可；现在，通过变量$x + t = u$的变换，我们有$g(x) = \int_x^{x+a} f(u) \, du$；由于 f 是连续的，因而 g 对于所有 $x \in \mathbf{R}$（II，p. 56，命题 3）都是可微分的，并且

$$
g'(x) = f(x+a) - f(x) = f(x)(f(a) - e).
$$

因而，$f'(x) = g'(x)b^{-1} = f(x)c$，其中$c = (f(a) - e)b^{-1}$，显然是$f'(0) = c$。

相反，可以直接证明（III，p. 115，练习1），或者通过线性微分方程理论（IV，p. 188），$\mathbf{R}$的每个可微的映射 f 都可以变成完全赋范的代数 E，使得$f'(x) = f(x)c$和$f(0) = e$，是加法群$\mathbf{R}$的同态变成乘法群G。

#### 命题 1 {#fvr-iii-s1-prop-1 .statement tag=089R}

*对于每个数$a > 0$和$\neq 1$，指数函数$a^\lambda$在每个点$x \in \mathbf{R}$承认导数等于$(\log_e a)a^\lambda$，其中e是数$> 1$（独立于$a$).*

应用th。 1 到 E 为域 $\mathbf{R}$ 的情况本身现在表明，$a^\lambda$ 在每个点处具有等于 $\varphi(a).a^\lambda$ 的导数，其中 $\varphi(a)$ 为实数 $\neq 0$ 仅取决于 $a$。设$b$为第二个数、$> 0$和$\neq 1$； 函数 $b^\lambda$ 的导数等于 $\varphi(b).b^\lambda$；另一方面，我们有$b^\lambda = a^\lambda \log_a b$，所以（I，p. 9，命题5）$b^\lambda$的导数等于$\log_a b.\varphi(a)b^\lambda$；比较这两个表达式我们得到

$$
\varphi(b) = \varphi(a).\log_a b.
$$ (2)

推断出存在一个唯一的数$b$使得$\varphi(b) = 1$；由（2）这个关系相当于$b = a^{1/\varphi(a)}$。通常用 e 表示实数；从 (2) 中，一个人有 $\varphi(a) = \log_e a$，这完成了道具的证明。 1.

人们经常写$\exp x$而不是$e^x$。

数 e 的定义表明

$$
D(e^\lambda) = e^\lambda
$$ (3)

这证明$e^\lambda$是严格递增的，因此$e > 1$。

在 §2 (III, p. 105) 中，我们将看到如何计算任意逼近 e。

#### 定义 1 {#fvr-iii-s1-def-1 .statement tag=089S}

*基 e 的对数称为 Naperian 对数（或自然对数）。*

对于 Naperian 对数，我们通常在记号中省略基。 除非相反，记号 $\log x$ ($x > 0$) 将表示 $x$ 的*纳佩里安对数*。有了这个记号，道具。 1 可以写成恒等式

$$
D(a^\lambda) = (\log a)a^\lambda
$$ (4)

对任何$a > 0$有效（$\log a = 0$当$a = 1$）。

这个关系表明$a^x$有*每个阶*的导数，并且
$$
D^n(a^x) = (\log a)^n a^x.
$$
(5)

特别是，对于$a > 0$和$\neq 1$，对于所有$x \in \mathbf{R}$，都有$D^2(a^x) > 0$，因此$a^x$在$\mathbf{R}$上“严格凸”（I，p. 31，推出）。由此推导出以下命题：

#### 命题 2（“几何平均值不等式”）{#fvr-iii-s1-prop-2 .statement tag=089T}

*对于任何数* $z_i > 0$ ($1 \leq i \leq n$) *和数* $p_i > 0$ *这样* $\sum_{i=1}^n p_i = 1$，*一个有*
$$
z_1^{p_1} z_2^{p_2} \cdots z_n^{p_n} \leq p_1 z_1 + p_2 z_2 + \cdots + p_n z_n.
$$
(6)
*此外，只有当* $z_i$ *相等时，(6) 的两侧才相等。*

让我们输入 $z_i = e^{x_i}$；那么不等式 (6) 可以写成
$$
\exp(p_1 x_1 + p_2 x_2 + \cdots + p_n x_n) \leq p_1 e^{x_1} + p_2 e^{x_2} + \cdots + p_n e^{x_n}.
$$
(7)
因此，命题由命题得出。 I、p. 26 的 1 应用于函数 $e^x$，它在 $\mathbf{R}$ 上严格凸。

有人说，(6) 的左侧（或右侧）是 $n$ 数 $z_i$ 相对于 *权* $p_i$ ($1 \leq i \leq n$) 的*加权几何平均值*（或*加权算术平均值*）。如果$p_i = 1/n$对应$1 \leq i \leq n$，则将相应的算术和几何平均值称为$z_i$的*普通*算术和几何平均值。那么不等式(6)可以写成
$$
(z_1 z_2 \cdots z_n)^{1/n} \leq \frac{1}{n}(z_1 + z_2 + \cdots + z_n).
$$
(8)

### 2. $\log_a x$ 的导数

由于$a^x$对于$a \neq 1$在$\mathbf{R}$上严格单调，应用微分逆函数的规则（I，p. 17，道具6）给出，对于所有$x > 0$
$$
D(\log_a x) = \frac{1}{x \log a}
$$
(9)
特别是
$$
D(\log x) = \frac{1}{x}.
$$
(10)

如果 $u$ 是实数函数，在点 $x_0$ 处有导数，并且$u(x_0) > 0$，则函数 $\log u$ 在点 $x_0$ 处有等于 $u'(x_0)/u(x_0)$ 的导数。特别是，如果 $x > 0$，我们有 $D(\log |x|) = 1/|x| = 1/x$，并且
$$
D(\log |x|) = -\frac{1}{|x|} = \frac{1}{x}
$$
如果$x < 0$；其他字，任何$x \neq 0$为$D(\log |x|) = 1/x$。一个结论，如果在区间$I$上，实函数$u$不是零并且允许有限导数，则$\log |u(x)|$允许在$I$上等于$u'/u$的导数；该导数称为 $u$ 的*对数导数*。可知$|u|^{\alpha}$的对数导数为$\alpha u'/u$，乘积的对数导数等于因子的对数导数的和；这些规则通常提供计算计算函数导数的最快方法。他们再次给予，特别是，公式
$$
D(x^{\alpha}) = \alpha x^{\alpha-1} \qquad (\alpha \text{ an arbitrary real number, } x > 0)
$$
另一个方法（II，p. 69）已经展示过。

#### 例 {#fvr-iii-s1-n2-exa-1 .statement tag=089U}

如果 $u$ 在区间 $I$ 上是函数 $\neq 0$，且 $v$ 是任意实数函数，则 $\log(|u|^v) = v \cdot \log |u|$，因此如果 $u$ 和 $v$ 可微分
$$
\frac{1}{|u|^v} D(|u|^v) = v' \log |u| + v \frac{u'}{u}.
$$

### 3. 通函函数的衍生品； 数$\pi$

我们已经定义了，一般的拓扑（*Gen.Top.*，VIII，p. 106），加法群$\mathbf{R}$的连续同态$x \mapsto \mathbf{e}(x)$到绝对值复数的乘法群$\mathbf{U}$ 值1；这是一个周期函数，主周期为 1，且$\mathbf{e}\left(\frac{1}{4}\right) = i$。人们知道（*loc.cit.*），$\mathbf{R}$到$\mathbf{U}$的每个连续同态都是形式$x \mapsto \mathbf{e}(x/a)$，并且人们将$\cos_a x = \mathscr{R}(\mathbf{e}(x/a)), \sin_a x = \mathscr{I}(\mathbf{e}(x/a))$（*三角函数*，或*圆形函数*，到基 $a$);最后的函数是连续的映射，从$\mathbf{R}$到$[-1, +1]$，主要周期为$a$。我们有 $\sin_a(x + a/4) = \cos_a x, \quad \cos_a(x + a/4) = -\sin_a x$，函数 $\sin_a x$ 是递增在区间 $[-a/4, a/4]$ 上。

#### 命题 3 {#fvr-iii-s1-prop-3 .statement tag=089V}

*函数* $\mathbf{e}(x)$ *有一个导数等于* $2\pi i \mathbf{e}(x)$ *在* $\mathbf{R}$的每点，*其中* $\pi$ *是一个常数* $> 0$。

现在，th。 III、p. 51中的1，应用于E为复数的域$\mathbf{C}$的情况，产生关系$\mathbf{e}'(x) = \mathbf{e}'(0) \mathbf{e}(x)$；此外，由于$\mathbf{e}(x)$具有常数欧氏范数，$\mathbf{e}'(x)$与$\mathbf{e}(x)$正交（I，p. 7，*例3*）；因此，有$\mathbf{e}'(0) = \alpha i$，$\alpha$实数。由于$\sin_1 x$在$[-\frac{1}{4}, \frac{1}{4}]$上是递增，它对$x = 0$的导数是$\geqslant 0$，所以$\alpha \geqslant 0$，并且由于$e(x)$不是常数，所以$\alpha > 0$；通常用 $2\pi$ 来表示数 $\alpha$。

在 §2 (III, p. 23) 中，我们将展示如何计算任意接近数 $\pi$。

因此我们有公式

$$
D \left( e \left( \frac{x}{a} \right) \right) = \frac{2\pi i}{a} e \left( \frac{x}{a} \right).
$$

我们可以看到，当 $a = 2\pi$ 时，这个公式被简化了；这就是为什么人们只在数学分析中使用相对于基$2\pi$的循环函数；对于这些函数，我们同意在记号中省略基；与除非相反地明确提及，记号、$\cos x$、$\sin x$和$\tan x$分别表示$\cos_{2\pi} x$、$\sin_{2\pi} x$和$\tan_{2\pi} x$。

根据这些约定，$a = 2\pi$、公式 (12) 可以写成

$$
D(\cos x + i \sin x) = \cos \left( x + \frac{\pi}{2} \right) + i \sin \left( x + \frac{\pi}{2} \right),
$$

这相当于

$$
D(\cos x) = -\sin x, \qquad D(\sin x) = \cos x,
$$

由此推论

$$
D(\tan x) = 1 + \tan^2 x = \frac{1}{\cos^2 x}.
$$

除了三个圆函数、$\cos x$、$\sin x$和$\tan x$之外，在数值计算中还使用三个辅助函数：余切、正割和余割，由公式定义

$$
\cot x = \frac{1}{\tan x}, \qquad \sec x = \frac{1}{\cos x}, \qquad \operatorname{cosec} x = \frac{1}{\sin x}.
$$

回想一下（Gen. Top.，VIII，p. 109），相应的到基 $2\pi$ 的角度称为弧度。

### 4. 反圆函数

函数 $\sin x$到区间$[-\pi/2, +\pi/2]$的限制为严格递增的； 1 用 $\operatorname{Arc}\sin x$ 表示其倒数，因此它是区间 $[-1, +1]$ 到 $[-\pi/2, +\pi/2]$ 的严格递增的连续映射（图 6）。 公式用于微分逆函数 (I, p. 9, 命题 6) 给出此函数的导数

$$
D(\operatorname{Arc}\sin x) = \frac{1}{\cos(\operatorname{Arc}\sin x)}.
$$

从 $-\pi/2 \leq \operatorname{Arc}\sin x \leq \pi/2$ 开始，我们就有了 $\cos(\operatorname{Arc}\sin x) \geq 0$，并且从

$$
\sin(\operatorname{Arc}\sin x) = x,
$$
我们有 $\cos(\operatorname{Arc}\sin x) = \sqrt{1 - x^2}$，其中
$$
\mathrm{D}(\operatorname{Arc}\sin x) = \frac{1}{\sqrt{1 - x^2}}.
$$
同样，$\cos x$到区间$[0, \pi]$的限制是严格递减； 1 用 $\operatorname{Arc}\cos x$ 表示其逆函数，并将 $[-1, +1]$ 的严格递减映射映射到 $[0, \pi]$（图 6）。而且

![图表显示 y = Arc cos x 和 y = Arc sin x](https://i.imgur.com/3Q5z5QG.png)

图6

$$
\sin \left( \frac{\pi}{2} - \operatorname{Arc}\cos x \right) = \cos(\operatorname{Arc}\cos x) = x
$$
从$-\pi/2 \leq \pi/2 - \operatorname{Arc}\cos x \leq \pi/2$开始，我们有
$$
\operatorname{Arc}\cos x = \frac{\pi}{2} - \operatorname{Arc}\sin x
$$
由此特别得出结论
$$
\mathrm{D}(\operatorname{Arc}\cos x) = -\frac{1}{\sqrt{1 - x^2}}.
$$

最后，tan x 到区间 ]−π/2, +π/2[ 的限制为严格递增的； 1 表示它的逆反正 tan x，这是从 \mathbf{R} 到 ]−π/2, +π/2[ 的严格递增的映射（图 7）；我们有

$$
\lim_{x \to -\infty} \operatorname{Arc tan} x = -\frac{\pi}{2}, \quad \lim_{x \to +\infty} \operatorname{Arc tan} x = \frac{\pi}{2},
$$

并且，通过应用公式对 III、p. 95 的逆函数和公式 (15) 进行微分，我们有

$$
\mathrm{D}\left( \operatorname{Arc tan} x \right) = \frac{1}{1 + x^2}.
$$

![图表显示 y = Arc tan x](https://i.imgur.com/3Q5z5QG.png)

图7

### 5. 复指数

我们已将复数的（加法）拓扑群 \mathbf{C} 的所有连续同态确定（Gen. Top.，VIII，p. 106）到（乘法）拓扑群 \mathbf{C}^* 复数 ≠ 0；这些是映射

$$
x + i y \mapsto e^{\alpha x + \beta y} \mathbf{e}(\gamma x + \delta y)
$$

其中$\alpha, \beta, \gamma, \delta$是四个实数，受单个条件$\alpha \delta - \beta \gamma \neq 0$影响。我们现在向确定提出同态 $z \mapsto f(z)$ 中哪些在 \mathbf{C} 上是*可微分的。首先我们注$f$在点$z = 0$可微就足够了；事实上，每点 $z \in \mathbf{C}$ 就有一个

$$
\frac{f(z + h) - f(z)}{h} = f(z) \frac{f(h) - 1}{h}
$$

如果$f'(0)$存在，那么$f'(z)$、$f'(z) = a f(z)$、$a = f'(0)$也存在。另一方面，如果$g$是二阶可微分同态，使得$g'(z) = b g(z)$，则$g(a z / b) = f(z)$，对于注，商$g(a z / b) / f(z)$具有处处零导数，并且对于$z = 0$等于1；因此，所有可微的同态都是形式$z \mapsto f(\lambda z)$，其中$f$是其中之一（假设它们存在），$\lambda$是任何（复数）常数。

既然这样，如果$f$在点$z = 0$可微，那么$\mathbf{R}$到$\mathbf{C}$的映射$x \mapsto f(x),\ y \mapsto f(iy)$中的每一个都必然在点$0$可微，第一个具有导数$f'(0)$，第二个$if'(0)$。现在映射 $x \mapsto e^{\alpha x} \mathbf{e}(\gamma x),\ y \mapsto e^{\beta y} \mathbf{e}(\delta y)$在点 $0$的导数分别等于$\alpha + 2\pi i \gamma$和$\beta + 2\pi i \delta$，由此得到$\beta = -2\pi \gamma$和$\alpha = 2\pi \delta$；这些条件尤其可以通过同态$x + iy \mapsto e^z \mathbf{e}(y/2\pi)$来满足，我们将暂时用$f_0$来表示。现在我们将证明 $f_0$ 实际上在点 $z = 0$ 处可微。

显然，$x \mapsto f_0(x)$和$y \mapsto f_0(iy)$都有每个阶的导数；特别是，泰勒的阶 1 的公式应用于这些函数表明，对于每个 $\varepsilon > 0$ 都有一个 $r > 0$，这样，如果有人将

$$
f_0(x) = 1 + x + \varphi(x)x,\qquad f_0(iy) = 1 + iy + \psi(y)y,
$$

那么条件$|x| \leq r,\ |y| \leq r$意味着$|\varphi(x)| \leq \varepsilon$和$|\psi(y)| \leq \varepsilon$；既然如此，我们就有 $f_0(x + iy) = f_0(x)f_0(iy) = 1 + (x + iy) + \theta(x,\ y)$ 了

$$
\theta(x,\ y) = (i + \varphi(x)\psi(y))xy + (1 + x)y\psi(y) + (1 + iy)x\varphi(x);
$$

对于 $|z| \leq r$，我们有 $|x| \leq r$ 和 $|y| \leq r$、从而

$$
|\theta(x,\ y)| \leq (1 + \varepsilon^2)|z|^2 + 2\varepsilon|z|(1 + |z|)
$$

证明了商$\frac{f_0(z) - 1 - z}{z}$与$z$趋于0，即函数$f_0$在点$z = 0$处导数等于1。由此证明，对于所有$z \in \mathbf{C}$，

$$
D(f_0(z)) = f_0(z).
$$

该性质建立了$f_0$和函数$e^z$之间的连接，而且是$f_0$到实轴的限制；为此，我们做了以下定义：

#### 定义 2 {#fvr-iii-s1-def-2 .statement tag=089W}

*同态* $x + iy \mapsto e^z \mathbf{e}(y/2\pi)$ *of* $\mathbf{C}$ *到* $\mathbf{C}^*$ *称为复指数；其任意复数*$z$*处的值*表示为*$e^z$*或*$\exp z$。

### 6. 函数 $e^z$ 的特性

$z \mapsto e^z$是$\mathbf{C}$到$\mathbf{C}^*$的同态这一事实可以用恒等式来表达

$$
e^{z+z'} = e^z e^{z'},\qquad e^0 = 1.\qquad e^{-z} = 1/e^z.
$$

到定义，每有$z = x + iy$，

$$
e^{x+iy} = e^x (\cos y + i \sin y)
$$

并且由于$e^{\lambda} > 0$，我们可以看到$e^z$有*绝对值*$e^{\lambda}$和*幅度*$y$（模$2\pi$）。

特别是，def。 2 (III, p. 98) 给出
$$
\mathbf{e}(x) = e^{2\pi i x}
$$
这允许我们在形式中写公式定义 $\cos x$ 和 $\sin x$
$$
\cos x = \frac{1}{2} (e^{i x} + e^{-i x}), \qquad \sin x = \frac{1}{2i} (e^{i x} - e^{-i x})
$$
*（欧拉公式）*。

由于$2\pi$是$\mathbf{e}(y/2\pi)$的主周期，$2\pi i$是$e^z$的*主周期*；在其他字中，$e^z$周期的群是数$2n\pi i$中的集合，其中$n$贯穿$\mathbf{Z}$。

最后，III、p. 98的公式(21)可以写成
$$
\mathrm{D}(e^z) = e^z
$$
从而，每复数 $a$
$$
\mathrm{D}(e^{a z}) = a\, e^{a z}.
$$

#### 注 {#fvr-iii-s1-n6-rem-1 .statement tag=089X}

If, in formula (27), one restricts the function $e^{a z}$ ($a$ complex) to the real axis, one again obtains, for $x$ real,
$$
\mathrm{D}(e^{a x}) = a\, e^{a x}.
$$
This formula allows us to calculate a primitive for each of the functions $e^{\alpha x} \cos \beta x$, $e^{\alpha x} \sin \beta x$ ($\alpha$ and $\beta$ real); indeed we have $e^{(\alpha + i \beta)x} = e^{\alpha x} \cos \beta x + i e^{\alpha x} \sin \beta x$, so, by (28)
$$
\mathrm{D}\left( \mathscr{R}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \cos \beta x
$$
$$
\mathrm{D}\left( \mathscr{I}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \sin \beta x.
$$
In the same way one reduces the evaluation of a primitive of $x^n e^{\alpha x} \cos \beta x$, or of $x^n e^{\alpha x} \sin \beta x$ (*n* *an integer* $> 0$) to that of a primitive of $x^n e^{(\alpha + i \beta)x}$; now, the formula for integration by parts of order $n + 1$ (II, p. 60, formula (11)) shows that a primitive of this last function is
$$
e^{(\alpha + i \beta)x} \left[ \frac{x^n}{\alpha + i \beta} - \frac{n x^{n-1}}{(\alpha + i \beta)^2} + \frac{n(n-1)x^{n-2}}{(\alpha + i \beta)^3} + \cdots + (-1)^n \frac{n!}{(\alpha + i \beta)^{n+1}} \right].
$$
By Euler’s formulae one can on the other hand express every positive integral power of $\cos x$ or of $\sin x$ as a linear combination of exponentials $e^{ip x}$ ($p$ a positive or negative integer). 由此，通过公式(28)，可以将形式$x^n e^{\alpha x} (\cos \beta x)' (\sin \gamma x)^s$的函数的原语表示为形式$x^p e^{\alpha x} \cos \lambda x$的函数和$x^p e^{\alpha x} \sin \mu x$的线性组合和($n, p, r, s$整数，$\alpha, \beta, \gamma, \lambda, \mu$)真实）。

#### 例 {#fvr-iii-s1-n6-exa-1 .statement tag=089Y}

一个有

$$
\sin^{2n} x = \frac{(-1)^n}{2^{2n}} \left( e^{i x} - e^{-i x} \right)^{2n} = \frac{(-1)^n}{2^{2n}} \left( e^{2n i x} - \binom{2n}{1} e^{(2n-2)i x} + \cdots + e^{-2n i x} \right)
$$

whence

$$
\int_0^1 \sin^{2n} t \, dt = \frac{(-1)^n}{2^{2n}} \left( \frac{1}{n} \sin 2n x - \binom{2n}{1} \frac{1}{n-1} \sin(2n-2)x + \cdots \right.
$$
$$
\left. + (-1)^{n-1} \binom{2n}{n-1} \sin 2x + (-1)^n \binom{2n}{n} x \right)
$$

特别是

$$
\int_0^{\pi/2} \sin^{2n} t \, dt = \binom{2n}{n} \frac{1}{2^{2n}} \frac{\pi}{2} = \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{\pi}{2}.
$$ (29)

### 7. 复对数

令 B 为由点 $z = x + i y$ 形成的“带”，使得 $-\pi \leq y < \pi$； 函数 $e^z$ 在 B 上将每个值取一次且仅一次；在其他字中，$z \mapsto e^z$是B在$\mathbf{C}^*$上的双射连续映射； （半开）线段$x = x_0,\ -\pi \leq y < \pi$的这个映射之下的像是圆$|z| = e^{x_0}$；线 $y = y_0$ 的像是由 $\mathrm{Am}(z) = y_0$ (mod. $2\pi$) 定义的（开）半线。 B 内部 $\dot{B}$ 的 $z \mapsto e^z$ 下的像，即 $z \in \mathbf{C}$ 的集合的$|\mathscr{I}(z)| < \pi$，是 $\mathbf{C}$ 中（闭）负实半轴的补 F；如果同意用$\mathrm{Am}(z)$表示属于至$[-\pi, \pi[$的$z$的幅度度量，则集合F可以由关系$-\pi < \mathrm{Am}(z) < \pi$定义。由于$z \mapsto e^z$是$\mathbf{C}$到$\mathbf{C}^*$像的严格同态，在B的任何开子集的映射下（所以$\mathbf{C}$）是$\mathbf{C}^*$中的开集合（所以在F中）；在其他字中，$z \mapsto e^z$与B的限制是$\dot{B}$在F上的同胚。我们用$z \mapsto \log z$表示F在B上的同胚，是后者的逆；对于复数$z \in F$，$\log z$称为$z$对数的主值。如果$z = x + i y$和$\log z = u + i v$，则$x + i y = e^{u+i v}$，从而$e^u = |z|$，从$-\pi < v < \pi$开始，我们有$v = \mathrm{Am}(z)$。此外，如果$y \neq 0$，我们还有$\tan(v + \pi/2) = -x/y$；因此我们可以写

$$
\begin{cases}
u = \log |z| = \frac{1}{2} \log(x^2 + y^2) \\
v = \frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y > 0 \\
v = 0 & \text{if } y = 0 \\
v = -\frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y < 0.
\end{cases}
$$ (30)

显然，$\log z$是定义在正开实半轴$\mathbf{R}_+^*$上的函数$\log x$的扩张到F。如果$z,\ z'$是F的两个点，使得$zz'$不是真正的负数，我们有$\log(zz') = \log z + \log z' + 2\varepsilon \pi i$，其中$\varepsilon = +1,\ -1$或0取决于$\mathrm{Am}(z)$和$\mathrm{Am}(z')$的值。

我们注在负实半轴函数$\log z$的点处没有极限；准确地说，如果 $x$ 趋向于 $x_0 < 0$ 并且 $y$ 趋于 0 剩余 > 0（或 < 0），则 $\log z$ 趋向于 $\log |x_0| + \pi i$（或 $\log |x_0| - \pi i$）；当$z$趋于0时，$|\log z|$无限增加。

稍后我们将看到解析函数的理论如何使我们能够完全概括地实现扩展函数 $\log z$ 以及定义复对数。

由于$\log z$是$e^z$的逆同胚，公式用于微分逆函数（I，p. 9，道具6）表明$\log z$在每个点$z \in \mathbf{F}$处可微，并且
$$
\mathrm{D}(\log z) = \frac{1}{e^{\log z}} = \frac{1}{z}
$$
公式概括了III、p. 93 的公式 (10)。

### 8. 有理数原语函数

公式 (31) 允许我们使用实数或复数系数来计算实数变量 $x$ 的任意有理数函数 $r(x)$ 的原语。我们知道（A.VII.7）这样的函数可以（以独特的方式）写成项的有限和，即：

a) 形式 $ax^p$ ($p$ 整数 $\geqslant 0$, $a$ 复数)；
b) 或形式$a/(x-b)^m$（$m$整数$\geqslant 0$、$a$和$b$复数）。

现在很容易获得每个项的原语：
a) $ax^p$ 的原语是 $a \frac{x^{p+1}}{p+1}$；
b) 如果 $m > 1$ $a/(x-b)^m$ 的原语是 $\frac{a}{(1-m)(x-b)^{m-1}}$；
c) 最后，从公式 (10) (III, p. 93) 和 (31) (III, p. 101)，如果 $b$ 是实数，$\frac{a}{x-b}$ 的原语是 $a \log |x-b|$，如果 $b$ 是复数，$a \log(x-b)$。在最后一种情况下，如果 $b = p + iq$，还有 (III, p. 100, 公式 (30))
$$
\log(x-b) = \log \sqrt{(x-p)^2 + q^2} + i \operatorname{Arc tan} \frac{x-p}{q} \pm i \frac{\pi}{2}.
$$

我们推迟了对更实际的方法的检查，以明确确定有理数函数的原语，该有理数函数明确给出给本次致力于数值演算的工作的部分。

我们可以用约化来评估有理数函数的原语：

1° 形式 $r(e^{a x})$ 的函数原语的求值，其中$r$是有理数函数和$a$实数；事实上，通过变量$u = e^{a x}$的变换加一个约化来找到$r(u)/u$的原语；

2° 形式 $f(\sin a x, \cos a x)$ 的函数原语的求值，其中$f$是两个变量的有理函数，$a$是实数；变量 $u = \tan(a x/2)$ 约化的变换找到一个原语

$$
\frac{2}{1 + u^2} \int \left( \frac{2u}{1 + u^2}, \frac{1 - u^2}{1 + u^2} \right).
$$

### 9. 复杂循环函数；双曲线函数

对于每个复数 $z$，欧拉的公式 (25) (III, p. 99) 和 $e^z$ 的定义允许我们定义扩展到 $\mathbf{C}$ 函数 $\cos x$ 和 $\sin x$ $\mathbf{R}$，通过放置，为所有$z \in \mathbf{C}$

$$
\cos z = \frac{1}{2} (e^{i z} + e^{-i z}), \qquad \sin z = \frac{1}{2i} (e^{i z} - e^{-i z})
$$
（cf.III，p. 119，练习 19）。

这些函数是周期性的，主周期为$2 \pi$；也就是说，有 $\cos(z + \pi/2) = -\sin z, \sin(z + \pi/2) = \cos z$；还可以验证身份

$$
\cos^2 z + \sin^2 z = 1 \\
\cos(z + z') = \cos z \cos z' - \sin z \sin z' \\
\sin(z + z') = \sin z \cos z' + \cos z \sin z'.
$$

更一般地，当给这些变量任意复数值（III，p. 119，练习18）时，实变量的循环函数之间的每个代数恒等式仍然为真。

如果$z \neq (2k + 1)\pi/2$则放入$\tan z = \sin z / \cos z$，如果$z \neq k \pi$则放入$\cot z = \cos z / \sin z$；这些是周期函数，主周期 $\pi$。

公式 (27) (III, p. 99) 证明 $\cos z$ 和 $\sin z$ 在 $\mathbf{C}$ 上可微，且

$$
\mathrm{D}(\cos z) = -\sin z, \qquad \mathrm{D}(\sin z) = \cos z.
$$

对于 $z = i x$ ($x$实数)，公式 (32) 给出

$$
\cos i x = \frac{1}{2} (e^i + e^{-i}), \qquad \sin i x = \frac{i}{2} (e^i - e^{-i}).
$$

这样引入的真实函数有一个特定的记号是很方便的；我们把

$$
\begin{cases}
\cosh x = \frac{1}{2} (e^x + e^{-x}) & \text{(hyperbolic cosine of } x \text{)} \\
\sinh x = \frac{1}{2} (e^x - e^{-x}) & \text{(hyperbolic sine of } x \text{)} \\
\tanh x = \frac{\sinh x}{\cosh x} = \frac{e^x - e^{-x}}{e^x + e^{-x}} & \text{(hyperbolic tangent of } x \text{)}
\end{cases}
$$

因此，对于每一个实数 $x$

$$
\cos i x = \cosh x, \quad \sin i x = i \sinh x.
$$

从复数 $z_k$ ($1 \leq k \leq n$) 的某个数中的圆函数之间的每个恒等式，可以通过替换 $z_k$ $i x_k$ ($x_k$ 实数) 推导出双曲函数的恒等式， $1 \leq k \leq n$）并使用公式（34）；例如一个有

$$
\cosh^2 x - \sinh^2 x = 1
$$
$$
\cosh(x + x') = \cosh x \cosh x' + \sinh x \sinh x'
$$
$$
\sinh(x + x') = \sinh x \cosh x' - \cosh x \sinh x'.
$$

双曲函数允许我们表达 $\cos z$ 的实数和虚数部分和 $\sin z$ 的 $z = x + i y$，因为

$$
\cos(x + i y) = \cos x \cos i y - \sin x \sin i y = \cos x \cosh y - i \sin x \sinh y
$$
$$
\sin(x + i y) = \sin x \cos i y + \cos x \sin i y = \sin x \cosh y + i \cos x \sinh y.
$$

最后，有一个

$$
D(\cosh x) = \sinh x, \quad D(\sinh x) = \cosh x, \quad D(\tanh x) = 1 - \tanh^2 x = \frac{1}{\cosh^2 x}.
$$

由于$\cosh x > 0$对于所有$x$，可以推断出$\sinh x$在$\mathbf{R}$上是严格递增的；从$\sinh 0 = 0$开始，$\sinh x$与$x$具有相同的符号。在推论$\cosh x$中，$x \leq 0$为严格递减，严格递增的为$x \geq 0$，最后，$\tanh x$在$\mathbf{R}$为严格递增的。而且

$$
\lim_{x \to -\infty} \sinh x = -\infty, \qquad \lim_{x \to +\infty} \sinh x = +\infty
$$
$$
\lim_{x \to -\infty} \cosh x = \lim_{x \to +\infty} \cosh x = +\infty
$$
$$
\lim_{x \to -\infty} \tanh x = -1, \qquad \lim_{x \to +\infty} \tanh x = +1 \qquad \text{(fig. 8 and 9)}.
$$

有时我们将$\sinh x$的逆函数写为$\operatorname{Arg} \sinh x$，即从$\mathbf{R}$到$\mathbf{R}$的严格递增的映射：这个函数也可以用对数项来表示，因为从关系$x = \sinh y = \frac{1}{2}(e^y - e^{-y})$我们推导出$e^{2y} - 2x e^y - 1 = 0$，从$e^y > 0$开始，我们有$e^y = x + \sqrt{x^2 + 1}$，也就是说

$$
\operatorname{Arg} \sinh x = \log \left( x + \sqrt{x^2 + 1} \right).
$$

类似地，我们用$\operatorname{Arg} \cosh x$表示$\cosh x$到$[0, +\infty[$的限制的逆；这个映射是从$]1, +\infty[$到$]0, +\infty[$的严格递增的；如上所示

$$
\operatorname{Arg} \cosh x = \log \left( x + \sqrt{x^2 - 1} \right).
$$

最后，我们用 Arg tanh $x$ 表示 tanh $x$ 的逆函数，即从 ]$-1, +1$ [ 到 $\mathbf{R}$ 的严格递增的映射；此外，还有，

$$
\operatorname{Arg} \tanh x = \frac{1}{2} \log \frac{1 + x}{1 - x}.
$$

#### 注 {#fvr-iii-s1-n9-rem-1 .statement tag=089Z}

对于复杂的 $z$ 一个有时写入

$$
\cosh z = \frac{1}{2} (e^z + e^{-z}) = \cos iz \\
\sinh z = \frac{1}{2} (e^z - e^{-z}) = -i \sin iz.
$$

这些函数因此是扩展到$\mathbf{C}$在$\mathbf{R}$上定义的双曲线函数。

### 习题{#fvr-iii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
