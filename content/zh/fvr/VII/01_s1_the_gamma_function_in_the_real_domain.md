---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 1
section_title: THE GAMMA FUNCTION IN THE REAL DOMAIN
lang: zh
source: fvr-i-vii
book_pages: 305-314, 325-327
pdf_pages: 0320-0329, 0340-0342
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE GAMMA FUNCTION
      page: 305
      pdf_page: 320
    - "no": 2
      title: PROPERTIES OF THE GAMMA FUNCTION
      page: 307
      pdf_page: 322
    - "no": 3
      title: THE EULER INTEGRALS
      page: 310
      pdf_page: 325
statements: 8
exercises: 6
content_sha256: 66e2271b371cc25160f236ffb566da9e2b269c490dacf66d8ecb969cb012e7aa
translated_from: content/en/fvr/VII/01_s1_the_gamma_function_in_the_real_domain.md
translation_method: google
source_content_sha256: c14b2d3b10b39cdfef4ea9acb546a2878e81232b29d6cdb8928fc7269171f7f2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 3cc128c37a3cb40fbe42ee75f0078ca65ac0412ff7c38b69825b9ad1c2ee265d
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。实数域中的伽玛函数

### 1. 伽玛定义函数

我们为每个整数$n \geq 0$定义了(集合理论,III,p. 179)函数$n!$，等于乘积$\prod_{0 \leq k < n} (n - k)$；所以$0! = 1$和$(n + 1)! = (n + 1)\, n!$代表$n \geq 0$。

我们每整数$n \geq 1$集合$\Gamma(n) = (n - 1)!$；我们建议在实数$x > 0$的集合上向定义，延伸在整数$\geq 1$的集合上定义的连续函数$\Gamma(x)$延伸函数$\Gamma$。

显然这样的函数有无穷多个；由于$\Gamma(n + 1) = n\Gamma(n)$对于每个整数$n \geq 1$，我们将限制自己在连续函数中考虑扩展$\Gamma$，那些满足方程

$$
f(x + 1) = x f(x)
$$

每$x > 0$。

为了使该等式的解成为$\Gamma(n)$的扩张，它还满足$f(1) = 1$是充分必要的。

如果$f$满足(1)，那么通过对$n$的递归，

$$
f(x + n) = x(x + 1)(x + 2) \ldots (x + n - 1)\, f(x)
$$

对于每个整数 $n > 1$ 以及所有 $x > 0$。这个关系特别表明，区间$]n, n + 1]$上$f$的值（$n$整数$\geq 1$）由区间$]0, 1]$上的值确定。反之，令$\varphi$为$]0, 1]$满足上的连续函数，仅条件$\varphi(1) = 1$、$\lim_{x \to 0} x \varphi(x) = 1$；对于每个整数$n \geq 1$，让我们在区间$]n, n + 1]$ by 关系定义$f$

$$
f(x) = (x - 1)(x - 2) \ldots (x - n)\, \varphi(x - n);
$$

显然$f$在$]0, +\infty[$上连续，满足式(1)，且扩展$\Gamma(n)$。

如果$f$是(1)的连续解并且在$]0, 1]$上取值$> 0$，则在$]0, +\infty[$上取值$> 0$，通过(2)；然后定义函数 $g(x) = \log f(x)$ 并在 ]0, +∞[ 上连续并满足方程

$$
g(x+1) - g(x) = \log x
$$

(3)

关于这个区间。

如果 $g_1$ 是 (3) 在 ]0, +∞[ 上的第二个连续解，并且如果 $h = g_1 - g$，则每 $x > 0$ 就有 $h(x+1) - h(x) = 0$；在其他字中，$h$ 是周期 1 的连续周期函数，定义在 ]0, +∞[ 上；相反，对于这种性质的每个 $h$，$g + h$ 是 (3) 的连续解。

#### 命题 1 {#fvr-vii-s1-prop-1 .statement tag=08IX}

*存在且仅有一个凸函数* $g$ *定义在* ]0, +∞[ *满足方程* (3) *并且对于* $x = 1$取值 0。

首先我们证明，如果存在函数 $g$ 满足条件，那么它在区间 ]0, 1] 上是明确确定的，因此在区间 ]0, +∞[ 上是明确确定的。事实上，对于每个整数$n > 1$，连接点$(n, g(n))$到点$(x, g(x))$的直线的梯度是$x$的递增函数，因为$g$是凸的（I， p. 27，道具 5)；因而，对于 $0 < x \leq 1$，必须有，

$$
\frac{g(n-1) - g(n)}{(n-1) - n} \leq \frac{g(n+x) - g(n)}{(n+x) - n} \leq \frac{g(n+1) - g(n)}{(n+1) - n}
$$

也就是说，通过(3)，

$$
x \log(n-1) \leq g(x+n) - g(n) \leq x \log n.
$$

现在，通过 (3)，

$$
g(x+n) - g(n) = g(x) + \log x + \sum_{k=1}^{n-1} (\log(x+k) - \log k).
$$

此外，可以写 $\log n = \sum_{k=2}^n \log \frac{k}{k-1}$，所以不等式 (4) 可以写成

$$
x \sum_{k=2}^{n-1} \log \frac{k}{k-1} \leq g(x) + \log x + \sum_{k=2}^n (\log(x+k-1) - \log(k-1))
$$
$$
\leq x \sum_{k=2}^n \log \frac{k}{k-1}.
$$

让我们对每个 $n \geq 2$，

$$
u_n(x) = x \log \frac{n}{n-1} - \log(x+n-1) + \log(n-1)
$$

(5)

和

$$
g_n(x) = -\log x + \sum_{k=2}^n u_k(x).
$$

对于 $0 < x \leq 1$ 则有
$$
g_n(x) - x \log \frac{n}{n-1} \leq g(x) \leq g_n(x).
$$
(6)

由于 $\log \frac{n}{n-1}$ 趋于 0，而 $n$ 趋于 $+\infty$，因此从 (6) 可以推断，如果解 $g$ 存在，那么它在 $]0, 1]$ 上必然等于 $g_n(x)$ 的 *极限*。

现在，我们可以立即从 (5) 推断出，对于 $x$ 是固定的，而$> 0$ 则有
$$
u_n(x) = -x \log \left( 1 - \frac{1}{n} \right) - \log \left( 1 + \frac{x-1}{n} \right) + \log \left( 1 - \frac{1}{n} \right) \sim \frac{x(x-1)}{2n^2}
$$
因为$n$趋于$+\infty$，这证明级数与一般项$u_n(x)$对于每个$x > 0$收敛。每个函数$u_n(x)$在$]0, +\infty[$上凸，$-\log x$、函数$g(x) = -\log x + \sum_{n=2}^{\infty} u_n(x)$在区间上凸（I、p. 27、第2条和第4条）；最后，有 $u_n(1) = 0$、从而 $g(1) = 0$，以及
$$
u_n(x+1) = u_{n+1}(x) + x \left( \log \frac{n}{n-1} - \log \frac{n+1}{n} \right)
$$
从而
$$
g(x+1) = -\log(x+1) + x \log 2 + \sum_{n=3}^{\infty} u_n(x) = \log x + g(x);
$$
其它字、$g$满足VII、p. 306的式(3)。

#### 定义 1 {#fvr-vii-s1-def-1 .statement tag=08IY}

*我们表示为* $\Gamma(x)$ *函数* $> 0$ *定义在区间* $]0, +\infty[$，*满足方程*
$$
\Gamma(x+1) = x \Gamma(x),
$$
*(7)*
*并且是这样的*$\Gamma(1) = 1$*并且*$\log \Gamma(x)$*在*$]0, +\infty[$上是凸的。

### 2. 伽玛函数的性质

#### 命题 2 {#fvr-vii-s1-prop-2 .statement tag=08IZ}

*对于每个* $x > 0$ *一个有*
$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x n!}{x(x+1)\ldots(x+n)}
$$
*（高斯公式）*，*和*
$$
\Gamma(x) = e^{-\gamma x} \frac{1}{x} \prod_{n=1}^{\infty} \frac{e^{x/n}}{1 + \frac{x}{n}}
$$
(9) 其中 $\gamma$ 表示欧拉常数，(9) 右侧的无穷乘积绝对一致地收敛于$\mathbf{R}$的每个紧致区间，而不是包含任何整数$< 0$（Weierstrass’ 公式）。

函数 $\Gamma(x)$ 在 $]0, +\infty[$ 上无限可微，并且有

$$
\frac{\Gamma'(x)}{\Gamma(x)} = -\gamma - \frac{1}{x} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{x+n} \right)
$$

和

$$
\mathrm{D}^k (\log \Gamma(x)) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(x+n)^k} \quad \text{for} \quad k \geq 2,
$$

(10) 和 (11) 右侧的级数绝对一致地收敛于每个紧致区间，而不是包含任何整数$\leq 0$。

事实上，道具的证明。 VII、p. 306 中的 1 表明

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x (n-1)!}{x(x+1)\ldots(x+n-1)}
$$

从而高斯’公式，因为$\frac{n}{x+n}$趋于1，而$n$趋于$+\infty$。也可以写一写

$$
\log \frac{n}{n-1} = \frac{1}{n-1} + \left( \log \frac{n}{n-1} - \frac{1}{n-1} \right).
$$

所以（在第 1 条的记号中）

$$
\exp(u_n(x)) = e^{(\log \frac{n}{n-1} - \frac{1}{n-1})} \frac{e^{x/(n-1)}}{1 + \frac{x}{n-1}}
$$

级数与一般项$\log \frac{n}{n-1} - \frac{1}{n-1}$绝对收敛，并有和$-\gamma$，其中$\gamma$表示欧拉常数（V，p. 242），从而我们得到Weierstrass’ 公式。

对于$|x| \leq a$，有一个$|1/(x+n)^k| \leq 1/(n-a)^k$一次$n > a$，所以公式(11)右边的级数绝对一致地收敛于$\mathbf{R}$的每个紧致区间，而不是包含任何整数 $\leq 0$，对于任何整数 $k \geq 2$；同样的论证也适用于 (10) 的右侧，因为 $\left| \frac{1}{n} - \frac{1}{x+n} \right| \leq \frac{a}{n(n-a)}$ 适合 $|x| \leq a$ 和 $n > a$。因为这些级数是通过微分级数得到的

$$
\log \Gamma(x) = -\gamma x - \log x + \sum_{n=1}^{\infty} \left( \frac{x}{n} - \log \left( 1 + \frac{x}{n} \right) \right)
$$

逐项收敛，并且对于每个 $x > 0$、级数以及一般项 $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ 绝对一致地收敛于 [0, +∞[ 中包含的每个紧致区间，并且有 VII 的关系 (10) 和 (11)， p. 308，对于每个 x > 0（II，p. 52，第 1）。此外，对于每个 x ∈ $\mathbf{R}$，一旦 n 足够大，表达式 $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ 就被定义，所以 th。 II，p. 52的1，再次证明了（9）右边的无限乘积（VII，p. 307）绝对一致地收敛于每个紧致区间包含，没有整数$\leq 0$。

对于$x > 0$定义的函数$\Gamma(x)$，可以推广到与整数$\leq 0$不同的点x的整个集合，从而得到VII、p. 307的满足方程（7），对此集合：对于 $-(n+1) < x < -n$ 来说就足够了
$$
\Gamma(x) = \frac{1}{x(x+1)\ldots(x+n)} \Gamma(x+n+1).
$$
通过道具。 VII、p. 307、公式 (8)、(9)、(10) 和 (11) VII、p. 307 和 308 中的 2 个，以及 (11) 中的$D^k(\log |\Gamma(x)|)$ 替换 $D^k(\log \Gamma(x))$，在此仍然有效集合。 公式 (9) (VII, p. 307) 通过VII, p. 307的(7)可知当x趋于0时$\Gamma(x) \sim 1/x$, 从而,
$$
\Gamma(x) \sim \frac{(-1)^n}{n! (x+n)}
$$
因为 x 趋于 $-n$ ($n$ 整数 $\geq 0$)。然后，函数$1/\Gamma(x)$可以通过连续性扩展到所有$\mathbf{R}$，在整数$\leq 0$处将其分配为值0；那么，对于所有$x \in \mathbf{R}$
$$
\frac{1}{\Gamma(x)} = \lim_{n \to \infty} \frac{x(x+1)\ldots(x+n)}{n^n n!}
$$
和
$$
\frac{1}{\Gamma(x)} = e^{y_1 x} x \prod_{n=1}^{\infty} \left( 1 + \frac{x}{n} \right) e^{-y_1/n}
$$
其中一个显示如道具中所示。 VII、p. 307的2，证明(13)右边的无限乘积绝对一致收敛于$\mathbf{R}$的每个紧致区间。

由于$\Gamma(x) > 0$对于$x > 0$，VII、p. 307的等式(7)表明$\Gamma(x) < 0$对于$-(2n-1) < x < -(2n-2)$和$\Gamma(x) > 0$对于
$$
-2n < x < -(2n-1)
$$
（$n$整数$\geq 1$）；另外$\Gamma(x)$在点$-2n$有右极限$+\infty$，在点$-(2n+1)$有$-\infty$，在点$-2n$有左极限$-\infty$以及 $+\infty$ 点 $-(2n+1)$（对于所有 $n \in \mathbf{N}$）。 VII、p. 308的公式(11)表明，对于$k = 2$，定义时其右侧始终为$\geq 0$，因而
$$
\Gamma''(x) \Gamma(x) - (\Gamma'(x))^2 \geq 0,
$$

因而 $\Gamma''(x)$ 与 $\Gamma(x)$ 具有相同的符号；因而$\Gamma$对于$x > 0$和$-(2n+2) < x < -(2n+1)$来说是*凸*，对于$-(2n+1) < x - 2n \ (n \in \mathbf{N})$来说是*凹*；由此推断，在$\Gamma$为凸的区间上，$\Gamma'(x)$从$-\infty$增加到$+\infty$，而在$\Gamma$为凹的区间上，$\Gamma'(x)$从$+\infty$减少到$-\infty$。 从而$\Gamma$的图表（图1）。

**如图。 1**

### 3. 欧拉积分

为了简洁起见，我们可以说，如果 $\log f$ 在 $I$ 上凸，则在区间 $I \subset \mathbf{R}$ 上定义的函数 $f$ 以及在此区间上定义的 $> 0$ 在 $I$ 上*对数凸*。 $\Gamma(x)$的定义表明，这个函数在$]0, +\infty[$上是对数凸的。

显然，$I$上的两个对数凸函数的*乘积*在$I$上也是对数凸的。进一步：

#### 引理 1 {#fvr-vii-s1-lem-1 .statement tag=08J0}

*设$f$和$g$是两个函数$> 0$，并且在开区间$I$上两次可微。如果 $f$ 和 $g$ 在 $I$ 上呈对数凸函数，则 $f + g$ 在 $I$ 上呈对数凸。*

关系$D^2 (\log f(x)) \geq 0$可以写成$f(x)f''(x) - (f'(x))^2 \geq 0$。我们简化为表明关系 $a > 0, a' > 0, ac - b^2 \geq 0, a'c' - {b'}^2 \geq 0$ 暗示 $(a + a')(c + c') - (b + b')^2 \geq 0$；现在，当$a > 0$、关系$ac - b^2 \geq 0$等价于$\mathbf{R}^2$上的二次形式$ax^2 + 2bxy + cy^2$为$\geq 0$，显然，如果

$$
ax^2 + 2bxy + cy^2 \geq 0 \quad \text{and} \quad a'x^2 + 2b'xy + c'y^2 \geq 0
$$

在 $\mathbf{R}^2$ 上，然后也在 $\mathbf{R}^2$ 上 $(a + a')x^2 + 2(b + b')xy + (c + c')y^2 \geq 0$。

#### 引理 2 {#fvr-vii-s1-lem-2 .statement tag=08J1}

令$f$为有限实数函数、$> 0$，在$\mathbf{R}$的两个开区间的乘积$I \times J$上定义且连续，并且对于每个$t \in J$函数$x \mapsto f(x, t)$是对数凸且两次在 $I$ 上可微。在这些假设下，如果积分 $g(x) = \int_J f(x, t) dt$ 对于每个 $x \in I$ 都收敛，则 $g$ 在 $I$ 上呈对数凸。

首先，我们证明对于每个紧凑区间 $K \subset J$ 函数 $g_K(x) = \int_K f(x, t) dt$ 都是对数凸的。事实上，如果 $K = [a, b]$、序列或函数

$$
g_n(x) = \frac{b-a}{n} \sum_{k=0}^{n-1} f\left(x, a + k \frac{b-a}{n}\right)
$$

在$I$（II，p. 57，命题5）上简单地收敛到$g_K(x)$，因此$\log g_n$简单地收敛于$\log g_K$；由 VII、p. 310、$\log g_n$ 的引理 1 在 $I$ 上凸，因此（I、p. 27、命题 4）对于 $\log g_K$ 也是如此。

另一方面，$g$是$g_K$沿$I$（II，p. 64）的紧致子区间有向集合的逐点极限，因此$\log g$是$\log g_K$的逐点极限；最后的函数在$I$上凸，$\log g$也是凸的（I，p. 27，道具4）。

即使不假设函数两次可微（VII、p. 327、练习 5），也可以轻松证明引理 1 和 2 仍然有效。

#### 引理 3 {#fvr-vii-s1-lem-3 .statement tag=08J2}

设$\varphi$是$[0, +\infty[$中包含的开区间$J$上的连续函数和$> 0$。如果$I$是开区间，使得积分$g(x) = \int_J t^{x-1} \varphi(t) dt$对于所有$x \in I$收敛，则$g$在$I$上呈对数凸。

事实上，$\log t^{x-1} = (x-1) \log t$是$x$的函数，它是凸的并且对于所有$t > 0$可两次微分，因此引理2适用。

#### 命题 3 {#fvr-vii-s1-prop-3 .statement tag=08J3}

对于所有人$x > 0$

$$
\Gamma(x) = \int_0^\infty e^{-t} t^{x-1} dt
$$

（第二欧拉积分）。

现在函数$g(x) = \int_0^\infty e^{-t} t^{x-1} dt$被定义为所有$x > 0$（V，p. 229）； 引理 3 of VII, p. 311，则表明它在 ]$0, +\infty[$ 上*对数凸*。此外，通过部分进行积分，有

$$
g(x+1) = \int_0^\infty e^{-t} t^x \, dt = -e^{-t} t^x \Big|_0^\infty + x \int_0^\infty e^{-t} t^{x-1} dt = x \, g(x).
$$

其它字、$g$为VII、p. 305等式(1)的解；最后，

$$
g(1) = \int_0^\infty e^{-t} \, dt = 1;
$$

因此，命题由道具得出。 1 个VII、p. 306。

通过变量$e^{-t} = u$的变换可以从 (14) (VII, p. 311) 公式推出

$$
\Gamma(x) = \int_0^1 \left( \log \frac{1}{t} \right)^{x-1} dt.
$$

类似地，从变量$u = t^{1/x}$的变换我们得到

$$
x \, \Gamma(x) = \int_0^\infty e^{-t^{1/x}} \, dt
$$

再次考虑 (7) (VII, p. 3)，

$$
\Gamma \left( 1 + \frac{1}{x} \right) = \int_0^\infty e^{-t^x} \, dt
$$

特别是对于$x = 2$

$$
\Gamma \left( \frac{3}{2} \right) = \frac{1}{2} \Gamma \left( \frac{1}{2} \right) = \int_0^\infty e^{-t^2} \, dt.
$$

#### 命题 4 {#fvr-vii-s1-prop-4 .statement tag=08J4}

*对于 $x > 0$ 和 $y > 0$ 整的*

$$
\mathbf{B}(x, y) = \int_0^1 t^{x-1} (1-y)^{y-1} \, dt
$$

(*第一个欧拉积分*) *有值*

$$
\mathbf{B}(x, y) = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$

事实上，这个积分对于$x > 0$和$y > 0$（V，p. 229）是收敛的。通过 I、p. 311、函数 $x \mapsto \mathbf{B}(x, y)$ 的引理 3 是 $x > 0$ 的*对数凸*。而且，

$$
\mathbf{B}(x+1, y) = \int_0^1 (1-t)^{x+y-1} \left( \frac{t}{1-t} \right)^x \, dt
$$

因此，通过部分积分，

$$
\mathbf{B}(x+1, y) = -\frac{(1-t)^{x+y}}{x+y} \left( \frac{t}{1-t} \right)^x \Bigg|_0^1
+ \frac{x}{x+y} \int_0^1 (1-t)^{x+y} \left( \frac{t}{1-t} \right)^{x-1} \frac{dt}{(1-t)^2} = \frac{x}{x+y} \mathbf{B}(x, y).
$$

由此可知$f(x) = \mathbf{B}(x, y) \Gamma(x+y)$满足VII、p. 305的恒等式(1)
而且，这个函数是对数凸的，是两个对数凸函数的乘积。最后，有$f(1) = \mathbf{B}(1, y) \Gamma(y+1)$、$\mathbf{B}(1, y) = \int_0^1 (1-t)^{y-1} dt = 1/y$、从而$f(1) = \frac{1}{y} \Gamma(y+1) = \Gamma(y)$。因此，根据属性，函数$f(x)/\Gamma(y)$等于$\Gamma(x)$。 VII、p. 306 中的 1，证明 (18)。

由变量 $t = \frac{u}{u+1}$ 公式的变换 (18) 变为

$$
\int_0^\infty \frac{t^{x-1}}{(1+t)^{x+y}} dt = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}
$$
(19)

以及变量 $t = \sin^2 \varphi$ 的变换

$$
\int_0^{\pi/2} \sin^{2x-1} \varphi \cos^{2y-1} \varphi d\varphi = \frac{1}{2} \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$
(20)

如果将 $x = y = \frac{1}{2}$ 放入最后一个公式中，则可以得出：

$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$
(21)

从而，由 (17)，

$$
\int_0^\infty e^{-t^2} dt = \frac{1}{2} \sqrt{\pi}.
$$
(22)

从VII、p. 307的关系(7)，有渐近展开

$$
\begin{align*}
\Gamma(x) &= \frac{1}{x} \Gamma(x+1) \\
&= \frac{1}{x} + \Gamma'(1) + \frac{1}{2!} \Gamma''(1)x + \cdots + \frac{1}{n!} \Gamma^{(n)}(1)x^{n-1} + O(x^n)
\end{align*}
$$
(23)

对于 $\Gamma(x)$，在邻域 0 上。

类似地，对于所有$y$固定和$> 0$都可以写

$$
\begin{align*}
\frac{1}{\Gamma(x+y)} &= \frac{1}{\Gamma(y)} + D \left( \frac{1}{\Gamma(y)} \right) x \\
&\quad + \frac{1}{2!} D^2 \left( \frac{1}{\Gamma(y)} \right) x^2 + \cdots + \frac{1}{n!} D^n \left( \frac{1}{\Gamma(y)} \right) x^n + O_1(x^{n+1})
\end{align*}
$$

公式 (18) 然后给出，对于固定的 $y$，渐近展开

$$
\mathbf{B}(x, y) = \frac{1}{x} + \left( \Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} \right)
+ \left( \frac{\Gamma''(1)}{2} - \Gamma'(1) \frac{\Gamma'(y)}{\Gamma(y)} + \frac{2{\Gamma'}^2(y) - \Gamma(y)\Gamma''(y)}{2\Gamma^2(y)} \right) x + O(x^2)
$$
于$x = 0$的邻域。

此外，对于$x > 0$和$y > 0$，有
$$
\mathbf{B}(x, y) = \int_0^1 \left( t^{x-1} + t^x \frac{(1-t)^{y-1} - 1}{t} \right) dt
= \frac{1}{x} + \int_0^1 t^x \frac{(1-t)^{y-1} - 1}{t} dt.
$$
函数 $\varphi(t) = \frac{(1-t)^{y-1} - 1}{t}$ 在紧致体区间 $[0, 1]$上连续；自从
$$
t^x = e^{x \log t} = 1 + x \log t + \frac{x^2}{2!} (\log t)^2 + \cdots + \frac{x^n}{n!} (\log t)^n + r_n(x, t)
$$
与 $|r_n(x, t)| \leq \frac{x^{n+1}}{(n+1)!} |\log t|^{n+1}$ （因为 $\log t \leq 0$ 和 $x > 0$），公式 (25) 给出渐近展开
$$
\mathbf{B}(x, y) = \frac{1}{x} + \int_0^1 \varphi(t) dt + x \int_0^1 \varphi(t) \log t \, dt + \cdots
+ \frac{x^n}{n!} \int_0^1 \varphi(t) (\log t)^n \, dt + O_2(x^{n+1})
$$
对于 0 的邻域上的 $\mathbf{B}(x, y)$。

对于 $n = 1$ 展开与 (24) 的辨识特别给出
$$
\Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} = \int_0^1 \frac{(1-t)^{y-1} - 1}{t} dt.
$$

此外，公式 (10) 给出$\Gamma'(1) = \Gamma'(1)/\Gamma(1) = -\gamma$，因此（*高斯积分*）
$$
\frac{\Gamma'(x)}{\Gamma(x)} + \gamma = \int_0^1 \frac{1 - (1-t)^{x-1}}{t} dt.
$$

### 习题{#fvr-vii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
