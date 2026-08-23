---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 2
section_title: THE GAMMA FUNCTION IN THE COMPLEX DOMAIN
lang: en
source: fvr-i-vii
pdf_pages: 0330-0338, 0342-0343
extraction: ocr
subsections:
    - "no": 1
      title: EXTENDING THE GAMMA FUNCTION TO C
      page: 0
      pdf_page: 330
    - "no": 2
      title: THE COMPLEMENTS’ RELATION AND THE LEGENDRE-GAUSS MULTIPLICATION FORMULA
      page: 0
      pdf_page: 331
    - "no": 3
      title: STIRLING'S EXPANSION
      page: 0
      pdf_page: 334
statements: 6
exercises: 6
content_sha256: 6be47bc6aec4e2250251661d315af13917b7991b97da582bdb05fa9da882ba8a
---

## § 2. THE GAMMA FUNCTION IN THE COMPLEX DOMAIN

### 1. EXTENDING THE GAMMA FUNCTION TO C

Let us return to Weierstrass’ formula which gives the expression

$$
\frac{1}{\Gamma(x)} = x\, e^{\gamma x} \prod_{n=1}^{\infty} \left(1 + \frac{x}{n}\right) e^{-x/n}
$$

for $1/\Gamma(x)$ for all real $x$, and consider the infinite product with general term $\left(1 + \frac{z}{n}\right) e^{-z/n}$ for arbitrary complex $z$. One can write $e^{-z/n} = 1 - \frac{z}{n} + h(z)$, with $|h(z)| \leq \frac{|z|^2}{2n^2} e^{|z/n|}$ (III, p. 106, formula (8)), whence

$$
\left(1 + \frac{z}{n}\right) e^{-z/n} = 1 + v_n(z)
$$

with $|v_n(z)| \leq \frac{|z|^2}{n^2} \left(1 + \frac{e^{|z|}}{2}(1 + |z|)\right)$; thus the infinite product under consideration is absolutely and uniformly convergent on every compact subset of $\mathbf{C}$; further, its value is zero only at the points $z = -n$ (\emph{Gen. Top.}, IX, p. 214, corollary). In view of the formula (1) of VII, p. 315, for every complex $z$ one puts

$$
\frac{1}{\Gamma(z)} = z\, e^{\gamma z} \prod_{n=1}^{\infty} \left(1 + \frac{z}{n}\right) e^{-z/n}.
$$

The function $\Gamma(z)$ is thus defined for every point $z \in \mathbf{C}$ apart from the points $-n$ ($n \in \mathbf{N}$); it is continuous on this set, and $(z + n)\Gamma(z) \sim \frac{(-1)^n}{n!}$ on a neighbourhood of $-n$. Formula (2) shows that one has $\Gamma(\overline{z}) = \overline{\Gamma(z)}$ for every $z$ different from a negative integer.

The argument that allows one to pass from Gauss’ formula (VII, p. 307, formula (8)) to Weierstrass’ formula, on reversing the steps, applies also to complex $z$ and shows that, for $z \neq -n$ ($n \in \mathbf{N}$), one has

$$
\Gamma(z) = \lim_{n \to \infty} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

on agreeing to put $n^z = e^{z \log n}$. Since

$$
\frac{n^{z+1} n!}{(z+1)(z+2)\ldots(z+n+1)} = z \frac{n}{n+1+z} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

one again has, on passing to the limit, the fundamental functional equation

$$
\Gamma(z+1) = z\, \Gamma(z)
$$

for every $z \neq -n$ ($n \in \mathbf{N}$).

Let $ p $ be an arbitrary integer $ > 0 $, and $ K_p $ the open disc $ |z| < p $; for every $ z \in K_p $, and every integer $ n > p $, $ 1 + \frac{z}{n} $ is not a negative real number, so $ \log \left( 1 + \frac{z}{n} \right) $ is defined, and it follows from the above that the series with general term $ \log \left( 1 + \frac{z}{n} \right) - \frac{z}{n} $ ($ n > p $) is *normally convergent* on $ K_p $; the same holds for the series obtained by differentiating the general term a finite number of times, since one has

$$
\left| \frac{1}{n} - \frac{1}{z+n} \right| \leq \frac{p}{n(n-p)} \quad \text{and} \quad \left| \frac{1}{(z+n)^k} \right| \leq \frac{1}{(n-p)^k} \qquad (k > 1)
$$

for $ z \in K_p $ and $ n > p $. One then sees (*cf.* II, p. 59, *Remark 3*) that $ \Gamma(z) $ is *indefinitely differentiable* at all the points $ z \in \mathbf{C} $ apart from the points $ -n $, and at these points one has

$$
\frac{\Gamma'(z)}{\Gamma(z)} = -\gamma - \frac{1}{z} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{z+n} \right)
$$
(5)

$$
D^{k-1} \left( \frac{\Gamma'(z)}{\Gamma(z)} \right) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(z+n)^k} \qquad \text{for} \quad k \geq 2,
$$
(6)

the right-hand sides of (5) and (6) being *normally convergent* on every compact subset of $ \mathbf{C} $ that does not contain any integer $ \leq 0 $. Further, one can write

$$
\log \Gamma(z) \equiv -\gamma z - \log z + \sum_{n=1}^{\infty} \left( \frac{z}{n} - \log \left( 1 + \frac{z}{n} \right) \right) \qquad (\text{mod. } 2\pi i)
$$
(7)

agreeing that when a logarithm in this formula is that of a real negative number it has one or the other limit values (differing by $ 2\pi i $) of $ \log z $ at this point; the series on the right-hand side of (7) is then normally convergent on every compact subset of $ \mathbf{C} $ not containing any integer $ \leq 0 $.

### 2. THE COMPLEMENTS’ RELATION AND THE LEGENDRE-GAUSS MULTIPLICATION FORMULA

One derives immediately from formula (2) of VII, p. 315, that, for every $ z \in \mathbf{C} $,

$$
\frac{1}{\Gamma(z)\Gamma(-z)} = -z^2 \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right).
$$

Now the Euler expansion of $ \sin z $ (VI, p. 287, th. 2) shows that

$$
z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right) = \frac{1}{\pi} \sin \pi z;
$$

taking account of the functional equation (4) of VII, p. 315, one then sees that:

#### Proposition 1 {#fvr-vii-s2-prop-1 .statement}

For every complex $ z $ one has

$$
\frac{1}{\Gamma(z)\Gamma(1-z)} = \frac{1}{\pi} \sin \pi z
$$

(the complements' relation).

COROLLARY — For every real $ t $ one has

$$
|\Gamma(it)| = \sqrt{\frac{\pi}{t \sinh \pi t}} \quad (t \neq 0)
$$

$$
|\Gamma(\frac{1}{2} + it)| = \sqrt{\frac{\pi}{\cosh \pi t}}.
$$

Indeed, one deduces from (8) that $ \Gamma(it)\Gamma(-it) = \frac{i\pi}{t \sin \pi it} = \frac{\pi}{t \sinh \pi t} $, and one has $ \Gamma(-it) = \overline{\Gamma(it)} $; similarly, (8) gives

$$
\Gamma\left(\frac{1}{2} + it\right)\Gamma\left(\frac{1}{2} - it\right) = \frac{\pi}{\sin (\frac{\pi}{2} + \pi it)} = \frac{\pi}{\cos \pi it} = \frac{\pi}{\cosh \pi t},
$$

and one has

$$
\Gamma\left(\frac{1}{2} - it\right) = \overline{\Gamma\left(\frac{1}{2} + it\right)}.
$$

Now let $ p $ be any integer $ > 0 $ and consider the product

$$
f(z) = \Gamma\left(\frac{z+1}{p}\right) \Gamma\left(\frac{z+2}{p}\right) \ldots \Gamma\left(\frac{z+p}{p}\right).
$$

By (3) (VII, p. 315), for every $ z \neq -n \ (n \in \mathbf{N}) $, $ f(z) $ is the limit of the product

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

and in particular $ f(0) $ is the limit of the product

$$
\frac{n^{(p+1)/2} p^{(n+1)p} (n!)^p}{((n+1)p)!}
$$

from which it follows that $ f(z)/f(0) $ is the limit of
$$
\frac{n^z ((n+1)p)!}{(z+1)(z+2)\ldots(z+(n+1)p)}
= z\ p^{-z} \left( \frac{n}{n+1} \right)^z \cdot \frac{((n+1)p)^z ((n+1)p)!}{z(z+1)(z+2)\ldots(z+(n+1)p)}
$$
which, by (3) (VII, p. 315), gives
$$
f(z) = f(0)\ z\ p^{-z}\ \Gamma(z).
$$
But one can write
$$
f(0) = \prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) = \prod_{k=1}^{p-1} \Gamma \left( 1 - \frac{k}{p} \right) = \sqrt{\prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) \Gamma \left( 1 - \frac{k}{p} \right)}
$$
since $ f(0) > 0 $; the complements’ relation then gives
$$
f(0) = \sqrt{\pi^{p-1} / \prod_{k=1}^{p-1} \sin \frac{k\pi}{p}}
$$
and since the product on the right-hand side is equal to $ p/2^{p-1} $ (VI, p. 284, cor. 1) one sees finally that:

#### Proposition 2 {#fvr-vii-s2-prop-2 .statement}

*For every complex number* $ z $ *not an integer* $ \leqslant 0 $ *and for every integer* $ p > 0 $ *one has*
$$
\Gamma \left( \frac{z}{p} \right) \Gamma \left( \frac{z+1}{p} \right) \ldots \Gamma \left( \frac{z+p-1}{p} \right) = (2\pi)^{(p-1)/2}\ p^{\frac{1}{2}-z}\ \Gamma(z)
$$
*(Legendre-Gauss multiplication formula)*.

#### Proposition 3 {#fvr-vii-s2-prop-3 .statement}

*For every real* $ x > 0 $ *one has*
$$
\int_1^{x+1} \log \Gamma(t)\ dt = x(\log x - 1) + \frac{1}{2} \log 2\pi
$$
*(Raabe’s integral)*.

First we establish formula (13) for $ x = 0 $. Since $ \log \Gamma(x) \sim \log \frac{1}{x} $ as $ x $ tends to 0, the integral $ \int_0^1 \log \Gamma(x)\ dx $ converges. Further, the function $ \log \Gamma(x) $ decreases on $ ]0, 1] $ (VII, p. 310); for every $ \alpha > 0 $ one thus has
$$
\frac{1}{n} \sum_{k=1}^q \log \Gamma \left( \frac{k}{n} \right) \leqslant \int_0^\alpha \log \Gamma(x)\ dx,
$$

$q$ being the largest integer such that $q/n \leqslant \alpha$. Since $\int_0^\alpha \log \Gamma(x) dx$ tends to 0 with $\alpha$ and also $\frac{1}{n} \sum_{k=q+1}^n \log \Gamma \left( \frac{k}{n} \right)$ tends to $\int_\alpha^1 \log \Gamma(x) dx$ as $n$ tends to $+\infty$ (II, p. 57, prop. 5) one has

$$
\int_0^1 \log \Gamma(x) dx = \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^n \log \Gamma \left( \frac{k}{n} \right).
$$

But, by (12), the right-hand side of this formula is the limit of

$$
\frac{n-1}{2n} \log 2\pi - \frac{1}{2} \frac{\log n}{n},
$$

whence

$$
\int_0^1 \log \Gamma(x) dx = \frac{1}{2} \log 2\pi.
$$ (14)

Next we remark that from the identity

$$
\log \Gamma(x+1) = \log \Gamma(x) + \log x
$$

one deduces, on integrating, that for $x > 0$

$$
\int_0^x \log \Gamma(t+1) dt = \int_0^x \log \Gamma(t) dt + \int_0^x \log t dt.
$$

But the integral on the left-hand side is also equal to $\int_1^{x+1} \log \Gamma(t) dt$. Thus, by (14),

$$
\int_1^{x+1} \log \Gamma(t) dt = \int_0^x \log t dt + \frac{1}{2} \log 2\pi = x (\log x - 1) + \frac{1}{2} \log 2\pi.
$$

### 3. STIRLING'S EXPANSION

Let $x$ and $y$ be two complex numbers not lying on the real negative half-axis; by formula (3) of VII, p. 315, with the conventions of VII, p. 316, concerning the logarithms, $\log \Gamma(x) - \log \Gamma(y)$ is congruent modulo $2\pi i$ to the limit of the expression

$$
(x-y) \log n + \sum_{k=0}^n \left( \log(y+k) - \log(x+k) \right).
$$ (15)

Let us put $f(t) = \log(y+t) - \log(x+t)$; we apply the Euler-Maclaurin summation formula (VI, p. 288) to the function $f$:

$$
f(0) + f(1) + \cdots + f(n) = \int_0^{n+1} f(t) dt - \frac{1}{2} (f(n+1) - f(0))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(n+1) - f^{(2k-1)}(0) \right) + T_p(n)
$$

with
$$
|T_p(n)| \leq \frac{4 e^{2\pi}}{(2\pi)^{2p+1}} \int_0^{n+1} |f^{(2p+1)}(u)|\ du.
$$
(16)

Since
$$
f^{(m)}(t) = (-1)^{m-1} (m-1)! \left( \frac{1}{(y+t)^m} - \frac{1}{(x+t)^m} \right),
$$
$f^{(2k-1)}(n+1)$ tends to 0 as $n$ tends to $+\infty$, for all $k \geq 1$; it is the same for
$$
f(n+1) = \log \left( 1 + \frac{y}{n+1} \right) - \log \left( 1 + \frac{x}{n+1} \right).
$$
Moreover, one has
$$
\int_0^{n+1} \log(x+t)\ dt = (x+n+1)(\log(x+n+1)-1) - x(\log x - 1);
$$
as $n$ tends to $+\infty$, one has the asymptotic expansion
$$
(x+n)(\log(x+n)-1) = n \log n - n + x \log n + O \left( \frac{1}{n} \right).
$$
Substituting in the expression (15) one sees finally that, as $n$ tends to $+\infty$, $T_p(n)$ has a limit $R_p(x,\ y)$ and that one can write
$$
\log \Gamma(x) - g(x) \equiv \log \Gamma(y) - g(y) + R_p(x,\ y) \quad (\text{mod. } 2\pi i)
$$
on putting
$$
g(x) = x \log x - x - \frac{1}{2} \log x + \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{x^{2k-1}}.
$$
(17)

We shall now evaluate a bound for $R_p(x,\ y)$ with the help of (16), assuming that $x$ and $y$ are both in the subset $\mathbf{H}_A$ of $\mathbf{C}$ defined by the relation "$\mathcal{R}(z) \geq A$ or $|\mathcal{I}(z)| \geq A$", where $A$ is an arbitrary number $> 0$ (fig. 2). To this end we remark that if $x = s + it$ with $s > A$ one has $|x+u| \geq A+u$ for every $u > 0$, and consequently
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_0^\infty \frac{du}{(A+u)^{2p+1}} = \frac{1}{2pA^{2p}}.
$$
Similarly, if $|t| \geq A$ one has $|x+u| = |s+u+it| \geq \sqrt{A^2 + (s+u)^2}$ for all real $u$, whence
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_{-\infty}^{+\infty} \frac{du}{(A^2 + u^2)^{p+1/2}} = \frac{2}{A^{2p}} \int_0^\infty \frac{dv}{(1+v^2)^{p+1/2}}.
$$
Thus one sees that, when $x$ and $y$ are in $\mathbf{H}_A$, one has
$$
|R_p(x,\ y)| \leq \frac{C_p}{A^{2p}}
$$

![A complex plane diagram showing axes labeled t, s, and regions H_A, A, -A, 0](Fig. 2)

where C_p depends only on p. Now let $ \mathfrak{F} $ be the filter having the sets H_A as basis; the Cauchy criterion shows that, along the filter $ \mathfrak{F} $, the function $ \log \Gamma(z) - g(z) $ has a finite limit $ \delta $ (modulo $ 2\pi i $) and that, if one puts $ \omega(z) = \max(\mathcal{R}(z), |\mathcal{I}(z)|) $, one has

$$
\log \Gamma(z) - g(z) - \delta \equiv O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i).
$$

For x real and > 0 one has $ \Gamma(x) > 0 $, and $ g(x) $ is real, so one can assume that $ \delta $ is real and one has

$$
\log \Gamma(x) = g(x) + \delta + O \left( \frac{1}{x^{2p}} \right).
$$

Now we shall deduce the value of the constant $ \delta $: by prop. 2 of VII, p. 318, applied for $ p = 2 $, one has, for real $ x $ tending to $ +\infty $

$$
\begin{align*}
&\frac{x-1}{2} \log \frac{x}{2} - \frac{x}{2} + \frac{x}{2} \log \frac{x+1}{2} - \frac{x+1}{2} + 2\delta \\
&\qquad = x \log x - x - \frac{1}{2} \log x + (\frac{1}{2} - x) \log 2 + \frac{1}{2} \log 2\pi + \delta + o(1)
\end{align*}
$$

from which one deduces easily that $ \delta = \frac{1}{2} \log 2\pi $. Finally one has the following result:

#### Proposition 4 {#fvr-vii-s2-prop-4 .statement}

*Along the filter $ \mathfrak{F} $ one has (for every integer $ p \geqslant 1 $) the asymptotic expansion*

$$
\log \Gamma(z) \equiv z \log z - z - \frac{1}{2} \log z + \frac{1}{2} \log 2\pi
+ \sum_{k=1}^{p} \frac{b_{2k}}{2k(2k-1)} \frac{1}{z^{2k-1}} + O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i)
$$

*(Stirling’s expansion)*.

#### Corollary {#fvr-vii-s2-n3-cor-1 .statement}

*Along the filter $ \mathfrak{F} $ one has*

$$
\Gamma(z) \sim \sqrt{2\pi} \exp(z \log z - z - \frac{1}{2} \log z).
$$

In particular, for $ x $ real tending to $ +\infty $ the formula (20) can be written

$$
\Gamma(x) \sim \sqrt{2\pi} \, x^{x-1/2} e^{-x},
$$

whence, as the integer $ n $ tends to $ +\infty $,

$$
n! \sim \sqrt{2\pi} \, n^{n+1/2} \, e^{-n}
$$

(*cf.* V, p. 244).

One can deduce numerous formulae from this. For example, for every complex number $ \alpha $ and every integer $ n $ one has, as $ n $ tends to $ +\infty $,

$$
\frac{\Gamma(n+\alpha)}{\Gamma(n)} \sim n^{\alpha} \quad (= e^{\alpha \log n}).
$$

Similarly, for every complex number $ a $ not an integer $ \leqslant 0 $ one has

$$
a(a+1)(a+2)\ldots(a+n) = \frac{\Gamma(n+a+1)}{\Gamma(a)} \sim \frac{\sqrt{2\pi}}{\Gamma(a)} \, n^{n+a+1/2} \, e^n
$$

and for every complex number $ a $ not an integer $ \geqslant 0 $

$$
\binom{a}{n} = \frac{(-1)^n}{\Gamma(-a)} \frac{\Gamma(n-a)}{\Gamma(n+1)} \sim \frac{(-1)^n}{\Gamma(-a)} \, n^{-a-1}.
$$

Finally, for every real constant $ k > 1 $ one has

$$
\binom{kn}{n} = \frac{\Gamma(kn+1)}{\Gamma(n+1) \Gamma((k-1)n+1)} \sim \sqrt{\frac{k}{2\pi(k-1)n}} \left( \frac{k^k}{(k-1)^{k-1}} \right)^n.
$$

The same argument leads to the following analogous proposition:

#### Proposition 5 {#fvr-vii-s2-prop-5 .statement}

Along the filter $ \mathfrak{F} $ one has (for every integer $ p \geqslant 1 $), the asymptotic expansion

$$
\frac{\Gamma'(z)}{\Gamma(z)} = \log z - \frac{1}{2z} - \sum_{k=1}^{p} \frac{b_{2k}}{2k} \frac{1}{z^{2k}} + O \left( \frac{1}{(\omega(z))^{2p+1}} \right).
$$

Instead of prop. 2 of VII, p. 318, one uses the formula

$$
\int_{x}^{x+1} \frac{\Gamma'(t)}{\Gamma(t)} \, dt = \log \Gamma(x+1) - \log \Gamma(x) = \log x
$$

in order to determine the constant.

### Exercises {#fvr-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
