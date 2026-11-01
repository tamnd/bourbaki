---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 2
section_title: EXPANSIONS OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS AND OF THE FUNCTIONS ASSOCIATED WITH THEM
lang: zh
source: fvr-i-vii
book_pages: 105-113, 125-128
pdf_pages: 0120-0128, 0140-0143
extraction: ocr
subsections:
    - "no": 1
      title: EXPANSION OF THE REAL EXPONENTIAL
      page: 105
      pdf_page: 120
    - "no": 2
      title: EXPANSIONS OF THE COMPLEX EXPONENTIAL, OF $\cos x$ AND $\sin x$
      page: 106
      pdf_page: 121
    - "no": 3
      title: THE BINOMIAL EXPANSION
      page: 107
      pdf_page: 122
    - "no": 4
      title: EXPANSIONS OF log(1 + x), OF Arc tan x AND OF Arc sin x
      page: 111
      pdf_page: 126
statements: 1
exercises: 9
content_sha256: 11979e279ce82a91c751ddf469dba8d6fe4f05bb19a7a0deb5ff05d3a2c2b4b7
translated_from: content/en/fvr/III/02_s2_expansions_of_the_exponential_and.md
translation_method: google
source_content_sha256: 9b4d042c915247a66706e89ec93b075b9470428497af056aac806e76d9a56cf9
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 2f4b5019dcfac30b7708eb23cf51f03865bb420f4bc50fcaabb72c7300ded75d
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。指数和循环函数的展开以及与它们相关的函数

### 1. 实指数的展开

由于$\mathrm{D}^n \left( e^x \right) = e^x$$e^x$的阶$n$的泰勒展开为

$$
e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + \int_0^x \frac{(x-t)^n}{n!} e^t \, dt. \tag{1}
$$

这个公式中的余数对于$x > 0$来说是$> 0$，当$x < 0$时有$(-1)^{n+1}$的符号；此外，平均值的不等式表明

$$
\frac{x^{n+1}}{(n+1)!} < \int_0^x \frac{(x-t)^n}{n!} e^t \, dt < \frac{x^{n+1} e^x}{(n+1)!} \qquad \text{for } x > 0 \tag{2}
$$

$$
\frac{\left| x^{n+1} \right| e^x}{(n+1)!} < \left| \int_0^x \frac{(x-t)^n}{n!} e^t \, dt \right| < \frac{\left| x^{n+1} \right|}{(n+1)!} \qquad \text{for } x < 0 \tag{3}
$$

现在我们知道，对于所有 $x \geqslant 0$ (*Gen.Top.*, IV, p. 365)，当 $n$ 无限增加时，序列 $\left( x^n / n! \right)$ 的极限为 0；因此，在 (1) 中保持 $x$ 固定并让 $n$ 无限增长，从 (2) 和 (3) 可以得出：

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} \tag{4}
$$

右侧的级数在$\mathbf{R}$中的每个紧区间*绝对一致收敛*。特别是，一个人有公式

$$
e = 1 + \frac{1}{1!} + \frac{1}{2!} + \cdots + \frac{1}{n!} + \cdots \tag{5}
$$

这个公式使我们能够尽可能接近数 $e$ 的有理近似值计算；一个获得

$$
e = 2.718\,281\,828\ldots
$$

到$1/10^9$以内。此外，公式 (5) 证明$e$ 是*无理数* 数 $^{2}$ (*Gen. Top.*, IV, p. 375)。

#### 注 {#fvr-iii-s2-n1-rem-1 .statement tag=08B3}

由于公式 (1) 中的余数为 $> 0$，对于 $x > 0$ 来说，有 $x > 0$

$$
e^x > 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^{n+1}}{(n+1)!}
$$

和*更不必说*

$$
e^x > \frac{x^{n+1}}{(n+1)!}
$$

对于每一个整数 $n$ ：由此可以推断 $e^x / x^n$ *倾向于* $+\infty$ 和 $x$ ，对于每一个整数 $n$ ：我们将在第 1 章中再次找到这个结果。 V由另一个方法（V，p. 231）。

$^{2}$ CH。 HERMITE于1873年证明，$e$是有理数的域$\mathbf{Q}$的*超越*数（在其他字中，它不是任何具有有理系数的多项式的根）（*Œuvres*，t. III，p. 150，巴黎（Gauthier-Villars），1912）。

### 2. 复指数的展开，$\cos x$ 和 $\sin x$

令$z$为任意复数，并考虑实数变量$t$的函数$\varphi(t) = e^{zt}$；我们有 $D^n \varphi(t) = z^n e^{zt}$ 和 $e^z = \varphi(1)$；通过阶 $n$ 的泰勒级数表达$\varphi(1)$ 关于点 $t = 0$ (II, p. 62) 从而给出

$$
e^z = 1 + \frac{z}{1!} + \frac{z^2}{2!} + \cdots + \frac{z^n}{n!} + z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

当$z$为实数时，公式等价于(1)。剩下的

$$
r_n(z) = z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

在这个公式可以通过使用均值的不等式在绝对值上界定；如果$z = x + i y$我们有$|e^{zt}| = e^{xt}$，那么$|e^{zt}| \leq 1$如果$x \leq 0$，$|e^{zt}| \leq e^x$如果$x > 0$；因此

$$
|r_n(z)| \leq \frac{|z|^{n+1}}{(n+1)!} \text{ if } x \leq 0
$$
$$
|r_n(z)| \leq \frac{|z|^{n+1} e^x}{(n+1)!} \text{ if } x > 0.
$$

如上所述，我们结论

$$
e^z = \sum_{n=0}^\infty \frac{z^n}{n!}
$$

级数 *绝对一致收敛*于$\mathbf{C}$的每个紧致子集。

从 (6) 可以特别推断出

$$
e^{ix} = 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \cdots + \frac{i^n x^n}{n!} + i^{n+1} \int_0^x \frac{(x-t)^n}{n!} e^{it} \, dt
$$

由此我们推导出$\cos x$和$\sin x$的泰勒展开；将 (10) 的实数部分取为阶 $2n+1$ 我们有

$$
\cos x = 1 - \frac{x^2}{2!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!} + (-1)^{n+1} \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

余数的边界为

$$
\left| \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt \right| \leq \frac{|x|^{2n+2}}{(2n+2)!}.
$$

类似地，将 (10) 的虚数部分取为阶 $2n$，我们得到

$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!}
$$
$$
+ (-1)^n \int_0^1 \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt
$$

余数的边界为

$$
\left| \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt \right| \leq \frac{|x|^{2n+1}}{(2n+1)!}.
$$

此外，比较 (11) 中阶 $2n+1$ 和 $2n+3$ 的余数，我们有

$$
\int_0^1 \frac{(x-t)^{2n+3}}{(2n+3)!} \cos t \, dt = \frac{x^{2n+2}}{(2n+2)!} - \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

考虑到（12），我们看到（11）中的余数与 $(-1)^{n+1}$ *相同的符号*，无论 $x$ 是什么；以同样的方式，我们可以证明 (13) 中的余数与 $(-1)^n x$ 具有*相同的符号*。特别是，对于（11）中的$n=0$和$n=1$，以及（13）中的$n=1$和$n=2$，我们得到不等式

$$
1 - \frac{x^2}{2} \leq \cos x \leq 1 \quad \text{for all } x
$$
(15)

$$
x - \frac{x^3}{6} \leq \sin x \leq x \quad \text{for all } x \geq 0.
$$
(16)

最后，将 $z = i x$ 代入 (9) 我们有

$$
\cos x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
$$
(17)

$$
\sin x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$
(18)

这些级数在每个紧区间绝对一致收敛。

此外，很明显，公式 (17) 和 (18) 对于右侧的每个*复数* $x$、级数仍然有效，并且绝对一致地收敛于 $\mathbf{C}$ 的每个紧致子集。特别是，对于每个$x$（实数或复数）

$$
\cosh x = \sum_{n=0}^\infty \frac{x^{2n}}{(2n)!}
$$
$$
\sinh x = \sum_{n=0}^\infty \frac{x^{2n+1}}{(2n+1)!}.
$$

### 3.二项式展开

令$m$为*任意*实数。对于$x > 0$，我们有

$$
D^n (x^m) = m(m-1)\ldots(m-n+1) x^{m-n};
$$

阶 $n$ 的泰勒公式关于点 $x = 0$ 对于函数 $(1 + x)^m$ 表明对于每个 $x > -1$

$$
(1 + x)^m = 1 + \binom{m}{1} x + \binom{m}{2} x^2 + \cdots + \binom{m}{n} x^n + r_n(x)
$$

与

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt
$$

我们把$\binom{m}{n} = \frac{m(m-1)\ldots(m-n+1)}{n!}$放在哪里。当 $m$ 为整数 $> 0$ 和 $n \geq m$ 时，公式 (19) 约化到二项式公式（代数，I，p. 99）；到扩张，我们再次将其称为*二项式公式*，并且当$m$是*任意*实数并且$n$是任意整数$> 0$时，系数$\binom{m}{n}$称为*二项式系数*。

如果$x > 0$，则(19)中的余数与$\binom{m}{n+1}$具有相同的符号；如果$-1 < x < 0$，则与$(-1)^{n+1} \binom{m}{n+1}$的符号相同。由于 $t > -1$ 的 $\left| \frac{x-t}{1+t} \right| \leq |x|$ 在端点为 0 和 $x$ 的区间内，因此对于任意 $m$ 和 $n$ 以及 $x > -1$，我们对余数有以下界限：

$$
\left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt \right|
$$
$$
\leq \left| \binom{m-1}{n} x^n ((1+x)^m - 1) \right|.
$$

如果我们假设$x \geq 0$和$n \geq m-1$，那么$(1+t)^{n-m+1} \geq 1$在积分区间上，所以

$$
0 \leq \int_0^x \frac{(x-t)^n}{(1+t)^{n-m+1}} \, dt \leq \int_0^x (x-t)^n \, dt = \frac{x^{n+1}}{n+1}
$$

这给出了估计

$$
|r_n(x)| \leq \left| \binom{m}{n+1} \right| x^{n+1} \quad (x \geq 0,\ n \geq m-1)
$$

其余的。另一方面，假设$-1 \leq m < 0$；如果在积分 (19) 中对变量 $u = \frac{x-t}{x(1+t)}$ 进行变换则可得

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} (1+x)^m x^{n+1} \int_0^1 \frac{u^n \, du}{(1+ux)^{m+1}}.
$$

为了估计$x > -1$的积分，我们注认为，自$m + 1 < 1$以来，整的$\int_0^1 \frac{u^n \, du}{(1-u)^{m+1}}$收敛并限制了自$1 + u x > 1 - u$以来的（22）的右侧。现在，对于$m$上的$-1 < x < 0$假设意味着出现在（19）右侧的所有项$\binom{m}{1} x, \binom{m}{2} x^2, \ldots, \binom{m}{n} x^n$都是$\geq 0$，因此是$r_n(x) \leq (1 + x)^m$，从中除以$(1 + x)^m$，

$$
\frac{m(m-1) \ldots (m-n)}{n!} x^{n+1} \int_0^1 \frac{u^n \, du}{(1 + u x)^{m+1}} \leq 1.
$$

而且，对于积分前面的$-1 < x < 0$因子来说，是$\geq 0$，所以，让$x$逼近$-1$，

$$
\left| \frac{m(m-1) \ldots (m-n)}{n!} \int_0^1 \frac{u^n \, du}{(1-u)^{m+1}} \right| \leq 1
$$

因此对于 $-1 \leq m < 0$ 和 $x > -1$ 我们有

$$
|r_n(x)| \leq (1 + x)^m |x|^{n+1}.
$$ (23)

从这些不等式我们可以首先推断出对于 $|x| < 1$ 我们有

$$
(1 + x)^m = \sum_{n=0}^\infty \binom{m}{n} x^n
$$ (24)

右边（称为二项式级数）绝对一致地收敛于$]-1, +1[$的每个紧致子集。确实可以写

$$
\binom{m}{n} = (-1)^n \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n} \right)
$$ (25)

从而

$$
\left| \binom{m}{n} \right| \leq \left( 1 + \frac{|m+1|}{1} \right) \left( 1 + \frac{|m+1|}{2} \right) \ldots \left( 1 + \frac{|m+1|}{n} \right).
$$

如果$|x| \leq r < 1$存在$n_0$使得$1 + \frac{|m|}{n_0} < \frac{1}{r'}$，其中$r < r' < 1$； 从而，推杆

$$
k = \left( 1 + \frac{|m|}{1} \right) \left( 1 + \frac{|m|}{2} \right) \ldots \left( 1 + \frac{|m|}{n_0} \right)
$$

我们有

$$
\left| \binom{m-1}{n} x^n \right| \leq k |x|^{n_0} \left( \frac{r}{r'} \right)^{n - n_0},
$$

这就证明了命题。另一方面，对于$x > 1$，如果$m$不是整数$\geq 0$，则级数(24)的一般项的绝对值随$n$无限增加；事实上，从 (25) 开始，我们有 $n > n_1 \geq |m+1|$

$$
\left| \binom{m}{n} \right| \geq \left| \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right|
$$
$$
\left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n} \right).
$$

让$n_0 \geq n_1$这样，对于$n \geq n_0$我们有$1 - \frac{|m+1|}{n} > \frac{1}{x'}$，其中$1 < x' < x$。如果我们把
$$
k' = \left| \left( 1 - \frac{m+1}{1} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right| \left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n_0} \right)
$$
那么，对于$n > n_0$，
$$
\left| \binom{m}{n} x^n \right| \geq k' |x|^{n_0} \left( \frac{x}{x'} \right)^{n-n_0}
$$
由此得出命题。

我们注对于$m = -1$的代数恒等式
$$
\frac{1}{1+x} = 1 - x + x^2 - \cdots + (-1)^{n-1} x^{n-1} + (-1)^n \frac{x^n}{1+x}
$$
给出一般公式 (19) 中余数的表达式，无需积分； 公式 (23) 约化在本例中为几何级数（或级数）的和表达式（Gen. Top.、IV、p. 364）。

其次，让我们研究二项式级数对于$x = 1$或$x = -1$的收敛性（不包括平凡的情况$m = 0$）：

$a) \ m \leq -1$。 乘积与广义项 $1 - \frac{m+1}{n}$ 如果 $m < -1$ 则收敛到 $+\infty$，如果 $m = -1$ 则收敛到 1，因此从 (25) 可以得出，对于 $x = \pm 1$，二项式级数的广义项不会趋向于 0。

$b) \ -1 < m < 0$。这次乘积与一般的项$1 - \frac{m+1}{n}$收敛于0，所以不等式(21)表明$r_n(1)$趋于0。因此二项式级数收敛于$x = 1$，有和$2^m$；此外，根据我们在上面和 (21) 中看到的，二项式级数一致收敛于每个区间 $]x_0, 1]$ 和 $-1 < x_0 \leq 1$。另一方面，对于 $x = -1$，(24) 右侧的所有项都是 $\geq 0$，如果这个级数收敛，我们可以推断出二项式级数通常会收敛于 $[-1, 1]$，因此其和会是一个连续的函数在此区间上，这是荒谬的，因为对于 $m < 0$，$(1+x)^m$ 不受 $[-1, 1]$ 的限制。我们结论对于$x = 1$来说二项式级数也不是绝对收敛的。

$c) \ m > 0$。 $r_n(x)$的定义表明，当$x$趋向于$-1$时，$r_n(x)$趋向于极限$r_n(-1)$；在 (20) 中的经过到极限上，结论与 $|r_n(-1)| \leq \left| \binom{m-1}{n} \right|$ 一致，并且从 $m-1 > -1$ 开始，我们看到对于 $x = -1$，二项式级数是收敛的。此外，对于$n > m+1$，该级数的所有项具有相同的符号；因此，二项式级数通常收敛于区间 [−1, 1]，并且在此区间上具有和 (1 + x)^m。

### 4. 展开 OF log(1 + x), OF 反正切 x 和 OF 反正弦 x

让我们将 (26) 的两边在 0 和 x 之间积分；我们得到 log(1 + x) 的阶 n 的泰勒展开，对于 x > −1 有效

$$
\log(1 + x) = \frac{x}{1} - \frac{x^2}{2} + \frac{x^3}{3} + \cdots + (-1)^n \frac{x^n}{n} + (-1)^n \int_0^x \frac{t^n \, dt}{1 + t}.
$$ (27)

如果 x > 0，余数与 (−1)^n 具有相同的符号；如果 -1 < x < 0，则余数 < 0；此外，当 x > 0 时，我们有 1 + t ≥ 1（0 ≤ t ≤ x），并且当 −1 < x < 0 时，我们有 1 + t ≥ 1 − |x|对于 x ≤ 0； 从而剩余部分的估计

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{n+1} \quad \text{for } x \geq 0 \tag{28}
$$

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{(n+1)(1-|x|)} \quad \text{for } -1 < x \leq 0. \tag{29}
$$

从最后两个公式可以立即推断出，对于 −1 < x ≤ 1，有

$$
\log(1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n}
$$ (30)

级数一致收敛于 ]−1, +1] 中包含的每个紧区间，并且对于 |x| 绝对收敛< 1。

另一方面，对于 |x| > 1 (30) 右侧级数中的一般项的大小随 n (III, p. 106) 无限增加。对于 x = −1 级数约化到谐波级数，其具有和 +∞（Gen. Top.、IV、p. 365）。

类似地，让我们在(26)中将替换 x乘以x^2，并对0和x之间的两边进行积分；我们获得反正切 x 的阶 2n − 1 的泰勒展开，对所有实数 x 有效

$$
\operatorname{Arc tan} x = \frac{x}{1} - \frac{x^3}{3} + \frac{x^5}{5} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{2n-1} + (-1)^n \int_0^x \frac{t^{2n} \, dt}{1 + t^2}. \tag{31}
$$

余数的符号为 (−1)^n x，并且由于对于所有 t 1 + t^2 ≥ 1，我们得到了估计

$$
\left| \int_0^x \frac{t^{2n} \, dt}{1 + t^2} \right| \leq \frac{|x|^{2n+1}}{2n+1} \tag{32}
$$

由此推断，对于 |x| ≤ 1,

$$
\operatorname{Arc tan} x = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^{2n-1}}{2n-1} \tag{33}
$$

级数一致收敛于 [−1, +1]，且绝对收敛于 |x| < 1。

特别是，对于 x = 1，可得到公式

$$
\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} + \cdots + (-1)^n \frac{1}{2n+1} + \cdots .
$$

对于 |x| > 1 (33) 右边的一般项的大小随着 n 无限增加。

最后，对于 Arc sin x 的泰勒展开，我们从其导数 (1 − x^2)^{-1/2} 的展开开始；最后一个展开是通过替换 x乘以-x^2在(1 + x)^{-1/2}的展开中作为二项式级数获得；对于 |x| < 1 这给出

$$
(1 - x^2)^{-1/2} = 1 + \frac{1}{2} x^2 + \frac{1.3}{2.4} x^4 + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} x^{2n} + r_n(x)
$$

由 (23) 得出界限

$$
0 \leq r_n(x) \leq \frac{x^{2n+2}}{\sqrt{1-x^2}}
$$

其余的。

取前面展开的原语，我们得到

$$
\text{Arc sin } x = x + \frac{1}{2} \frac{x^3}{3} + \frac{1.3}{2.4} \frac{x^5}{5} + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1} + R_n(x)
$$

其中 R_n(x) 的符号为 x 并且满足不等式

$$
|R_n(x)| \leq \int_0^x \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

进一步，关系(35)表明，当x接近1或-1时，R_n(x)趋于极限，因此有

$$
|R_n(1)| \leq \int_0^1 \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

但是，当 n 趋向于 +∞ 时，(37) 的右侧趋向于 0：因为，由于积分 $\int_0^1 dt / \sqrt{1-t^2}$ 是收敛的，因此对于每个 ε > 0，都存在一个 a，使得 0 < a < 1 且$\int_a^1 dt / \sqrt{1-t^2} \leq \varepsilon$；另一方面我们有

$$
\int_0^a \frac{t^{2n+2} dt}{\sqrt{1-t^2}} \leq \frac{1}{\sqrt{1-a^2}} \int_0^a t^{2n+2} dt = \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}}
$$

因此存在一个 n_0，对于 n ≥ n_0，有 $\frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}} \leq \varepsilon$、从而，最后，|R_n(x)| |x| ≤ 2ε ≤ 1 且 n ≥ n_0。因此一个人有

$$
\operatorname{Arc}\sin x = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1}
$$

(38)

右侧通常收敛于紧区间 [−1, 1]。

在相反的情况下，可以证明，对于二项式级数，(38) 右侧级数中的一般项对于|x| 的绝对值值无限增加。 > 1.
将$x = \frac{1}{2}$代入例，在(38)中我们得到数$\pi$的新表达式：

$$
\frac{\pi}{6} = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{1}{(2n+1)2^{2n+1}}
$$

它比公式 (34) 更适合计算 $\pi$ 的近似值（参见 Calcul numérique）；由此获得

$$
\pi = 3.141\,592\,653\ldots
$$

精确到$1/10^9$.³以内

³ 数 $\pi$ 不仅是无理数（cf. III、p. 126，练习 5），而且甚至超越有理数数的域 $\mathbf{Q}$，正如 Lindemann 在 1882 年首次证明的那样（参见对于例 D Hilbert，Gesammelte Abhandlungen，v. 1，p. 1，柏林 (Springer)，1932)。

### 习题 {#fvr-iii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
