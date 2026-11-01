---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 2
section_title: THE GAMMA FUNCTION IN THE COMPLEX DOMAIN
lang: zh
source: fvr-i-vii
book_pages: 315-323, 327-328
pdf_pages: 0330-0338, 0342-0343
extraction: ocr
subsections:
    - "no": 1
      title: EXTENDING THE GAMMA FUNCTION TO C
      page: 315
      pdf_page: 330
    - "no": 2
      title: THE COMPLEMENTS’ RELATION AND THE LEGENDRE-GAUSS MULTIPLICATION FORMULA
      page: 316
      pdf_page: 331
    - "no": 3
      title: STIRLING'S EXPANSION
      page: 319
      pdf_page: 334
statements: 6
exercises: 6
content_sha256: 7c3a77b3bd4a239555c1f11585f4b20103f8b1e793b6cb7f4e68e3c86c3def91
translated_from: content/en/fvr/VII/02_s2_the_gamma_function_in_the_complex_domain.md
translation_method: google
source_content_sha256: 1c81174cbd47bb500a623e0c569e0a38286f1c72eeae4b3d0069a0e65ec296a4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 51e773a2ab55a2544d9c991463669d91046868da392fc88f45c0d689b251ad91
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。复杂域中的 GAMMA 函数

### 1. 将 GAMMA 函数扩展到 C

让我们回到 Weierstrass 的公式，它给出了表达式

$$
\frac{1}{\Gamma(x)} = x\, e^{\gamma x} \prod_{n=1}^{\infty} \left(1 + \frac{x}{n}\right) e^{-x/n}
$$

对于$1/\Gamma(x)$对于所有实数$x$，并考虑无限乘积与一般项$\left(1 + \frac{z}{n}\right) e^{-z/n}$对于任意复数$z$。可以写 $e^{-z/n} = 1 - \frac{z}{n} + h(z)$，与 $|h(z)| \leq \frac{|z|^2}{2n^2} e^{|z/n|}$ (III, p. 106, 公式 (8)), 从而

$$
\left(1 + \frac{z}{n}\right) e^{-z/n} = 1 + v_n(z)
$$

与 $|v_n(z)| \leq \frac{|z|^2}{n^2} \left(1 + \frac{e^{|z|}}{2}(1 + |z|)\right)$；因此，所考虑的无限乘积绝对一致地收敛于$\mathbf{C}$的每个紧致子集；此外，它的值仅在点$z = -n$处是零（\emph{Gen.Top.}，IX，p. 214，推论）。鉴于 VII、p. 315 的公式 (1)，对于每一个复数 $z$ 都有一个放

$$
\frac{1}{\Gamma(z)} = z\, e^{\gamma z} \prod_{n=1}^{\infty} \left(1 + \frac{z}{n}\right) e^{-z/n}.
$$

因此，除了点 $-n$ ($n \in \mathbf{N}$) 之外，函数 $\Gamma(z)$ 也被定义为每个点 $z \in \mathbf{C}$；在这个集合上是连续的，$(z + n)\Gamma(z) \sim \frac{(-1)^n}{n!}$在$-n$的邻域上是连续的。 公式 (2) 表明对于每个 $z$ 都有 $\Gamma(\overline{z}) = \overline{\Gamma(z)}$ 与负的整数不同。

允许从高斯的公式（VII，p. 307，公式（8））传递到魏尔斯特拉斯的公式的论证，在反转步骤时，也适用于复数$z$，并且表明，对于$z \neq -n$（$n \in \mathbf{N}$），我们有

$$
\Gamma(z) = \lim_{n \to \infty} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

同意放置$n^z = e^{z \log n}$。自从

$$
\frac{n^{z+1} n!}{(z+1)(z+2)\ldots(z+n+1)} = z \frac{n}{n+1+z} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

又在经过到极限上有基本函数方程

$$
\Gamma(z+1) = z\, \Gamma(z)
$$

对于每个 $z \neq -n$ ($n \in \mathbf{N}$)。

设$p$为任意整数$> 0$，$K_p$为开盘$|z| < p$；对于每个 $z \in K_p$ 和每个整数 $n > p$，$1 + \frac{z}{n}$ 都不是负的实数，因此定义了 $\log \left( 1 + \frac{z}{n} \right)$，并且从上面得出，级数与一般项 $\log \left( 1 + \frac{z}{n} \right) - \frac{z}{n}$ ($n > p$) *通常收敛*于$K_p$；这同样适用于通过将一般的项微分到有限的数次而获得的级数，因为有

$$
\left| \frac{1}{n} - \frac{1}{z+n} \right| \leq \frac{p}{n(n-p)} \quad \text{and} \quad \left| \frac{1}{(z+n)^k} \right| \leq \frac{1}{(n-p)^k} \qquad (k > 1)
$$

对于 $z \in K_p$ 和 $n > p$。然后我们会看到 (*cf.* II, p. 59, *注 3*) $\Gamma(z)$ 除了点 $-n$ 之外，点 $z \in \mathbf{C}$ 都是“无限可微”，并且在这些点处，我们有

$$
\frac{\Gamma'(z)}{\Gamma(z)} = -\gamma - \frac{1}{z} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{z+n} \right)
$$
(5)

$$
D^{k-1} \left( \frac{\Gamma'(z)}{\Gamma(z)} \right) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(z+n)^k} \qquad \text{for} \quad k \geq 2,
$$
(6)

(5) 和 (6) 的右侧在 $\mathbf{C}$ 的每个紧致子集上“通常收敛”，但包含不存在任何整数 $\leq 0$。此外，还可以写出

$$
\log \Gamma(z) \equiv -\gamma z - \log z + \sum_{n=1}^{\infty} \left( \frac{z}{n} - \log \left( 1 + \frac{z}{n} \right) \right) \qquad (\text{mod. } 2\pi i)
$$
(7)

同意当公式中的对数是实负数的对数时，它在点处具有$\log z$的一个或另一个极限值（相差$2\pi i$）； (7) 右边的级数通常收敛于$\mathbf{C}$的每个紧致子集，而不是包含任何整数$\leq 0$。

### 2. 补数关系和勒让德高斯乘法公式

直接从VII、p. 315的公式 (2) 推导出来，对于每个$z \in \mathbf{C}$，

$$
\frac{1}{\Gamma(z)\Gamma(-z)} = -z^2 \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right).
$$

现在$\sin z$ (VI, p. 287, th. 2) 的欧拉展开表明

$$
z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right) = \frac{1}{\pi} \sin \pi z;
$$

考虑VII、p. 315的函数方程(4)，可以看出：

#### 命题 1 {#fvr-vii-s2-prop-1 .statement tag=08JB}

对于每一个复数 $z$ 都有

$$
\frac{1}{\Gamma(z)\Gamma(1-z)} = \frac{1}{\pi} \sin \pi z
$$

（补数'关系）。

#### 推出{#fvr-vii-s2-n2-cor-1 .statement tag=08JC}

对于每一个真实的 $t$ 都有

$$
|\Gamma(it)| = \sqrt{\frac{\pi}{t \sinh \pi t}} \quad (t \neq 0)
$$

$$
|\Gamma(\frac{1}{2} + it)| = \sqrt{\frac{\pi}{\cosh \pi t}}.
$$

事实上，从 (8) 可以推导出 $\Gamma(it)\Gamma(-it) = \frac{i\pi}{t \sin \pi it} = \frac{\pi}{t \sinh \pi t}$，并且有$\Gamma(-it) = \overline{\Gamma(it)}$；类似地，(8) 给出

$$
\Gamma\left(\frac{1}{2} + it\right)\Gamma\left(\frac{1}{2} - it\right) = \frac{\pi}{\sin (\frac{\pi}{2} + \pi it)} = \frac{\pi}{\cos \pi it} = \frac{\pi}{\cosh \pi t},
$$

一个有

$$
\Gamma\left(\frac{1}{2} - it\right) = \overline{\Gamma\left(\frac{1}{2} + it\right)}.
$$

现在让 $p$ 为任意整数 $> 0$ 并考虑乘积

$$
f(z) = \Gamma\left(\frac{z+1}{p}\right) \Gamma\left(\frac{z+2}{p}\right) \ldots \Gamma\left(\frac{z+p}{p}\right).
$$

根据 (3) (VII, p. 315)，对于每个 $z \neq -n \ (n \in \mathbf{N})$，$f(z)$ 是乘积中的极限

$$
\frac{n^{(z+1)/p} n!}{\left(\frac{z+1}{p}\right) \left(\frac{z+1}{p} + 1\right) \ldots \left(\frac{z+1}{p} + n\right)}
$$

$$
\frac{n^{(z+2)/p} n!}{\left(\frac{z+2}{p}\right) \left(\frac{z+2}{p} + 1\right) \ldots \left(\frac{z+2}{p} + n\right)} \cdots
$$

$$
\ldots \frac{n^{(z+p)/p} n!}{\left(\frac{z+p}{p}\right) \left(\frac{z+p}{p} + 1\right) \ldots \left(\frac{z+p}{p} + n\right)}
$$

$$
= \frac{n^{z+(p+1)/2} p^{(n+1)p} (n!)^p}{(z+1)(z+2) \ldots (z+(n+1)p)}
$$

特别是 $f(0)$ 是极限 / 乘积

$$
\frac{n^{(p+1)/2} p^{(n+1)p} (n!)^p}{((n+1)p)!}
$$

由此可知 $f(z)/f(0)$ 是极限
$$
\frac{n^z ((n+1)p)!}{(z+1)(z+2)\ldots(z+(n+1)p)}
= z\ p^{-z} \left( \frac{n}{n+1} \right)^z \cdot \frac{((n+1)p)^z ((n+1)p)!}{z(z+1)(z+2)\ldots(z+(n+1)p)}
$$
由 (3) (VII, p. 315) 得出
$$
f(z) = f(0)\ z\ p^{-z}\ \Gamma(z).
$$
但可以写
$$
f(0) = \prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) = \prod_{k=1}^{p-1} \Gamma \left( 1 - \frac{k}{p} \right) = \sqrt{\prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) \Gamma \left( 1 - \frac{k}{p} \right)}
$$
自 $f(0) > 0$ 起；补数’ 关系则给出
$$
f(0) = \sqrt{\pi^{p-1} / \prod_{k=1}^{p-1} \sin \frac{k\pi}{p}}
$$
由于右侧的乘积等于$p/2^{p-1}$（VI，p. 284，cor.1），我们最终看到：

#### 命题 2 {#fvr-vii-s2-prop-2 .statement tag=08JD}

*对于每个复数* $z$ *不是整数* $\leqslant 0$ *并且对于每个整数* $p > 0$ *一个有*
$$
\Gamma \left( \frac{z}{p} \right) \Gamma \left( \frac{z+1}{p} \right) \ldots \Gamma \left( \frac{z+p-1}{p} \right) = (2\pi)^{(p-1)/2}\ p^{\frac{1}{2}-z}\ \Gamma(z)
$$
*（勒让德-高斯乘法公式）*。

#### 命题 3 {#fvr-vii-s2-prop-3 .statement tag=08JE}

*对于每个真实* $x > 0$ *一个有*
$$
\int_1^{x+1} \log \Gamma(t)\ dt = x(\log x - 1) + \frac{1}{2} \log 2\pi
$$
*（拉贝积分）*。

首先我们为$x = 0$建立公式(13)。由于$\log \Gamma(x) \sim \log \frac{1}{x}$随着$x$趋于0，整的$\int_0^1 \log \Gamma(x)\ dx$收敛。此外，函数$\log \Gamma(x)$在$]0, 1]$上减少（VII，p. 310）；对于每 $\alpha > 0$ 一个人因此有
$$
\frac{1}{n} \sum_{k=1}^q \log \Gamma \left( \frac{k}{n} \right) \leqslant \int_0^\alpha \log \Gamma(x)\ dx,
$$

$q$ 最大的整数使得$q/n \leqslant \alpha$。由于 $\int_0^\alpha \log \Gamma(x) dx$ 与 $\alpha$ 趋于 0，并且 $\frac{1}{n} \sum_{k=q+1}^n \log \Gamma \left( \frac{k}{n} \right)$ 趋于 $\int_\alpha^1 \log \Gamma(x) dx$，因为 $n$ 趋于 $+\infty$（II，p. 57，道具 5），因此有

$$
\int_0^1 \log \Gamma(x) dx = \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^n \log \Gamma \left( \frac{k}{n} \right).
$$

但是，根据 (12)，这个公式的右侧是极限

$$
\frac{n-1}{2n} \log 2\pi - \frac{1}{2} \frac{\log n}{n},
$$

从而

$$
\int_0^1 \log \Gamma(x) dx = \frac{1}{2} \log 2\pi.
$$ (14)

接下来我们注从恒等式来看

$$
\log \Gamma(x+1) = \log \Gamma(x) + \log x
$$

在积分时，我们可以推断出 $x > 0$

$$
\int_0^x \log \Gamma(t+1) dt = \int_0^x \log \Gamma(t) dt + \int_0^x \log t dt.
$$

但左边的积分也等于$\int_1^{x+1} \log \Gamma(t) dt$。因此，通过 (14)，

$$
\int_1^{x+1} \log \Gamma(t) dt = \int_0^x \log t dt + \frac{1}{2} \log 2\pi = x (\log x - 1) + \frac{1}{2} \log 2\pi.
$$

### 3.斯特林展开

令$x$和$y$为不位于实负半轴上的两个复数；由VII、p. 315的公式(3)，按照VII、p. 316的对数约定，$\log \Gamma(x) - \log \Gamma(y)$与表达式的$2\pi i$模极限全等

$$
(x-y) \log n + \sum_{k=0}^n \left( \log(y+k) - \log(x+k) \right).
$$ (15)

让我们把$f(t) = \log(y+t) - \log(x+t)$；我们将欧拉-麦克劳林求和公式 (VI, p. 288) 应用于函数 $f$：

$$
f(0) + f(1) + \cdots + f(n) = \int_0^{n+1} f(t) dt - \frac{1}{2} (f(n+1) - f(0))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(n+1) - f^{(2k-1)}(0) \right) + T_p(n)
$$

与
$$
|T_p(n)| \leq \frac{4 e^{2\pi}}{(2\pi)^{2p+1}} \int_0^{n+1} |f^{(2p+1)}(u)|\ du.
$$
(16)

自从
$$
f^{(m)}(t) = (-1)^{m-1} (m-1)! \left( \frac{1}{(y+t)^m} - \frac{1}{(x+t)^m} \right),
$$
对于所有 $k \geq 1$，$f^{(2k-1)}(n+1)$ 趋于 0，因为 $n$ 趋于 $+\infty$；对于
$$
f(n+1) = \log \left( 1 + \frac{y}{n+1} \right) - \log \left( 1 + \frac{x}{n+1} \right).
$$
此外，还有一个
$$
\int_0^{n+1} \log(x+t)\ dt = (x+n+1)(\log(x+n+1)-1) - x(\log x - 1);
$$
由于 $n$ 趋于 $+\infty$，因此渐近展开
$$
(x+n)(\log(x+n)-1) = n \log n - n + x \log n + O \left( \frac{1}{n} \right).
$$
代入式(15)，最终可知，由于$n$趋于$+\infty$，$T_p(n)$有极限$R_p(x,\ y)$，并且可以写成
$$
\log \Gamma(x) - g(x) \equiv \log \Gamma(y) - g(y) + R_p(x,\ y) \quad (\text{mod. } 2\pi i)
$$
推杆上
$$
g(x) = x \log x - x - \frac{1}{2} \log x + \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{x^{2k-1}}.
$$
(17)

我们现在将在（16）的帮助下评估$R_p(x,\ y)$的界限，假设$x$和$y$都在由关系“$\mathscr{R}(z) \geq A$或$|\mathscr{I}(z)| \geq A$”定义的$\mathbf{C}$的子集$\mathbf{H}_A$中，其中$A$ 是任意数 $> 0$（图 2）。为此，我们注，如果$x = s + it$和$s > A$，每个$u > 0$都有$|x+u| \geq A+u$，因而
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_0^\infty \frac{du}{(A+u)^{2p+1}} = \frac{1}{2pA^{2p}}.
$$
类似地，如果 $|t| \geq A$ 对于所有实数 $u$ 都有 $|x+u| = |s+u+it| \geq \sqrt{A^2 + (s+u)^2}$，则从而
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_{-\infty}^{+\infty} \frac{du}{(A^2 + u^2)^{p+1/2}} = \frac{2}{A^{2p}} \int_0^\infty \frac{dv}{(1+v^2)^{p+1/2}}.
$$
由此可见，当$x$和$y$在$\mathbf{H}_A$时，有
$$
|R_p(x,\ y)| \leq \frac{C_p}{A^{2p}}
$$

![复平面图表显示标记为 t、s 的轴和区域 H_A、A、-A、0]（图 2）

其中 C_p 仅取决于 p。现在令$\mathfrak{F}$为集合H_A为基的滤波器；柯西准则表明，沿着过滤器 $\mathfrak{F}$，函数 $\log \Gamma(z) - g(z)$ 具有有限的极限 $\delta$（模 $2\pi i$），并且如果有人放入 $\omega(z) = \max(\mathscr{R}(z), |\mathscr{I}(z)|)$，则有

$$
\log \Gamma(z) - g(z) - \delta \equiv O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i).
$$

对于 x 实数且 > 0，有 $\Gamma(x) > 0$，并且 $g(x)$ 是实数，因此可以假设 $\delta$ 是实数，并且有

$$
\log \Gamma(x) = g(x) + \delta + O \left( \frac{1}{x^{2p}} \right).
$$

现在我们将通过 prop 推导常数 $\delta$ 的值。 2 个VII，p. 318，申请了$p = 2$，一个已经有了，真正的$x$ 倾向于$+\infty$

$$
\begin{align*}
&\frac{x-1}{2} \log \frac{x}{2} - \frac{x}{2} + \frac{x}{2} \log \frac{x+1}{2} - \frac{x+1}{2} + 2\delta \\
&\qquad = x \log x - x - \frac{1}{2} \log x + (\frac{1}{2} - x) \log 2 + \frac{1}{2} \log 2\pi + \delta + o(1)
\end{align*}
$$

由此可以很容易地推导出$\delta = \frac{1}{2} \log 2\pi$。最终得到如下结果：

#### 命题 4 {#fvr-vii-s2-prop-4 .statement tag=08JF}

*沿着过滤器$\mathfrak{F}$，有一个（对于每个整数$p \geqslant 1$）渐近展开*

$$
\log \Gamma(z) \equiv z \log z - z - \frac{1}{2} \log z + \frac{1}{2} \log 2\pi
+ \sum_{k=1}^{p} \frac{b_{2k}}{2k(2k-1)} \frac{1}{z^{2k-1}} + O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i)
$$

*（斯特林的展开）*。

#### 推出{#fvr-vii-s2-n3-cor-1 .statement tag=08JG}

*沿着过滤器$\mathfrak{F}$有一个*

$$
\Gamma(z) \sim \sqrt{2\pi} \exp(z \log z - z - \frac{1}{2} \log z).
$$

特别是，对于 $x$ 实数趋于 $+\infty$ 公式 (20) 可以写成

$$
\Gamma(x) \sim \sqrt{2\pi} \, x^{x-1/2} e^{-x},
$$

从而，因为整数 $n$ 趋于 $+\infty$，

$$
n! \sim \sqrt{2\pi} \, n^{n+1/2} \, e^{-n}
$$

（*cf.* V、p. 244）。

由此可以推导出无数公式。对于例，对于每一个复数$\alpha$和每一个整数$n$，因为$n$趋向于$+\infty$，

$$
\frac{\Gamma(n+\alpha)}{\Gamma(n)} \sim n^{\alpha} \quad (= e^{\alpha \log n}).
$$

类似地，对于每一个复数 $a$ 而不是整数 $\leqslant 0$ ，都有一个

$$
a(a+1)(a+2)\ldots(a+n) = \frac{\Gamma(n+a+1)}{\Gamma(a)} \sim \frac{\sqrt{2\pi}}{\Gamma(a)} \, n^{n+a+1/2} \, e^n
$$

对于每个复数 $a$ 不是整数 $\geqslant 0$

$$
\binom{a}{n} = \frac{(-1)^n}{\Gamma(-a)} \frac{\Gamma(n-a)}{\Gamma(n+1)} \sim \frac{(-1)^n}{\Gamma(-a)} \, n^{-a-1}.
$$

最后，对于每个实数常数$k > 1$，有

$$
\binom{kn}{n} = \frac{\Gamma(kn+1)}{\Gamma(n+1) \Gamma((k-1)n+1)} \sim \sqrt{\frac{k}{2\pi(k-1)n}} \left( \frac{k^k}{(k-1)^{k-1}} \right)^n.
$$

同样的论点导致以下类似的命题：

#### 命题 5 {#fvr-vii-s2-prop-5 .statement tag=08JH}

沿着过滤器$\mathfrak{F}$（对于每个整数$p \geqslant 1$），渐近展开

$$
\frac{\Gamma'(z)}{\Gamma(z)} = \log z - \frac{1}{2z} - \sum_{k=1}^{p} \frac{b_{2k}}{2k} \frac{1}{z^{2k}} + O \left( \frac{1}{(\omega(z))^{2p+1}} \right).
$$

而不是道具。 VII、p. 318 2 个，其中 1 个使用公式

$$
\int_{x}^{x+1} \frac{\Gamma'(t)}{\Gamma(t)} \, dt = \log \Gamma(x+1) - \log \Gamma(x) = \log x
$$

在阶到确定中为常数。

### 习题 {#fvr-vii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
