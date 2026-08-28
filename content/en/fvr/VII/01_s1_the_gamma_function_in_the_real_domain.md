---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 1
section_title: THE GAMMA FUNCTION IN THE REAL DOMAIN
lang: en
source: fvr-i-vii
pdf_pages: 0320-0329, 0340-0342
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE GAMMA FUNCTION
      page: 0
      pdf_page: 320
    - "no": 2
      title: PROPERTIES OF THE GAMMA FUNCTION
      page: 0
      pdf_page: 322
    - "no": 3
      title: THE EULER INTEGRALS
      page: 0
      pdf_page: 325
statements: 8
exercises: 6
content_sha256: f1dbe01f2e933089ae266a6020c73d595c10a78aa1cea50f223a11623430aacd
---

## § 1. THE GAMMA FUNCTION IN THE REAL DOMAIN

### 1. DEFINITION OF THE GAMMA FUNCTION

We have defined (Set Theory, III, p. 179) the function $n!$ for every integer $n \geq 0$, as equal to the product $\prod_{0 \leq k < n} (n - k)$; so $0! = 1$ and $(n + 1)! = (n + 1)\, n!$ for $n \geq 0$.

We set $\Gamma(n) = (n - 1)!$ for each integer $n \geq 1$; we propose to define, on the set of real numbers $x > 0$, a continuous function $\Gamma(x)$ extending the function $\Gamma$ defined on the set of integers $\geq 1$.

It is clear that there are infinitely many such functions; since $\Gamma(n + 1) = n\Gamma(n)$ for every integer $n \geq 1$ we shall restrict ourselves to considering, among the continuous functions that extend $\Gamma$, those which satisfy the equation

$$
f(x + 1) = x f(x)
$$

for every $x > 0$.

For a solution of this equation to be an extension of $\Gamma(n)$ it is necessary and sufficient that it also satisfies $f(1) = 1$.

If $f$ satisfies (1) then, by recursion on $n$,

$$
f(x + n) = x(x + 1)(x + 2) \ldots (x + n - 1)\, f(x)
$$

for every integer $n > 1$ and for all $x > 0$. This relation shows, in particular, that the values of $f$ on an interval $]n, n + 1]$ ($n$ an integer $\geq 1$) are determined by its values on the interval $]0, 1]$. Conversely, let $\varphi$ be a continuous function on $]0, 1]$ satisfying only the conditions $\varphi(1) = 1$, $\lim_{x \to 0} x \varphi(x) = 1$; for every integer $n \geq 1$ let us define $f$ on the interval $]n, n + 1]$ by the relation

$$
f(x) = (x - 1)(x - 2) \ldots (x - n)\, \varphi(x - n);
$$

it is clear that $f$ is continuous on $]0, +\infty[$, satisfies the equation (1), and extends $\Gamma(n)$.

If $f$ is a continuous solution of (1) and takes values $> 0$ on $]0, 1]$ it takes values $> 0$ on $]0, +\infty[$, by (2); the function $g(x) = \log f(x)$ is then defined and continuous on ]0, +∞[ and satisfies the equation

$$
g(x+1) - g(x) = \log x
$$

(3)

on this interval.

If $g_1$ is a second continuous solution of (3) on ]0, +∞[, and if $h = g_1 - g$, then one has $h(x+1) - h(x) = 0$ for every $x > 0$; in other words, $h$ is a continuous periodic function of period 1, defined on ]0, +∞[; conversely, for every $h$ of this nature, $g + h$ is a continuous solution of (3).

#### Proposition 1 {#fvr-vii-s1-prop-1 .statement}

*There exists one and only one convex function* $g$ *defined on* ]0, +∞[ *that satisfies the equation* (3) *and takes the value 0 for* $x = 1$.

First we show that if there is a function $g$ satisfying the conditions stated then it is well-determined on the interval ]0, 1], and consequently on the interval ]0, +∞[. Indeed, for every integer $n > 1$ the gradient of the line joining the point $(n, g(n))$ to the point $(x, g(x))$ is an increasing function of $x$, since $g$ is convex (I, p. 27, prop. 5); one thus must have, for $0 < x \leq 1$,

$$
\frac{g(n-1) - g(n)}{(n-1) - n} \leq \frac{g(n+x) - g(n)}{(n+x) - n} \leq \frac{g(n+1) - g(n)}{(n+1) - n}
$$

that is, by (3),

$$
x \log(n-1) \leq g(x+n) - g(n) \leq x \log n.
$$

Now, by (3),

$$
g(x+n) - g(n) = g(x) + \log x + \sum_{k=1}^{n-1} (\log(x+k) - \log k).
$$

Moreover, one can write $\log n = \sum_{k=2}^n \log \frac{k}{k-1}$ so the inequality (4) can be written

$$
x \sum_{k=2}^{n-1} \log \frac{k}{k-1} \leq g(x) + \log x + \sum_{k=2}^n (\log(x+k-1) - \log(k-1))
$$
$$
\leq x \sum_{k=2}^n \log \frac{k}{k-1}.
$$

Let us put, for every $n \geq 2$,

$$
u_n(x) = x \log \frac{n}{n-1} - \log(x+n-1) + \log(n-1)
$$

(5)

and

$$
g_n(x) = -\log x + \sum_{k=2}^n u_k(x).
$$

For $0 < x \leq 1$ one then has
$$
g_n(x) - x \log \frac{n}{n-1} \leq g(x) \leq g_n(x).
$$
(6)

Since $\log \frac{n}{n-1}$ tends to 0 as $n$ tends to $+\infty$ one deduces from (6) that if a solution $g$ exists then it is necessarily equal, on $]0, 1]$, to the *limit* of the $g_n(x)$.

Now one deduces immediately from (5) that for $x$ fixed and $> 0$ one has
$$
u_n(x) = -x \log \left( 1 - \frac{1}{n} \right) - \log \left( 1 + \frac{x-1}{n} \right) + \log \left( 1 - \frac{1}{n} \right) \sim \frac{x(x-1)}{2n^2}
$$
as $n$ tends to $+\infty$, which proves that the series with general term $u_n(x)$ converges for every $x > 0$. Each of the functions $u_n(x)$ being convex on $]0, +\infty[$, as is $-\log x$, the function $g(x) = -\log x + \sum_{n=2}^{\infty} u_n(x)$ is convex on this interval (I, p. 27, prop. 2 and prop. 4); finally, one has $u_n(1) = 0$, whence $g(1) = 0$, and
$$
u_n(x+1) = u_{n+1}(x) + x \left( \log \frac{n}{n-1} - \log \frac{n+1}{n} \right)
$$
whence
$$
g(x+1) = -\log(x+1) + x \log 2 + \sum_{n=3}^{\infty} u_n(x) = \log x + g(x);
$$
in other words, $g$ satisfies equation (3) of VII, p. 306.

#### Definition 1 {#fvr-vii-s1-def-1 .statement}

*We denote by* $\Gamma(x)$ *the function* $> 0$ *which is defined on the interval* $]0, +\infty[$, *that satisfies the equation*
$$
\Gamma(x+1) = x \Gamma(x),
$$
*(7)*
*and is such that* $\Gamma(1) = 1$ *and that* $\log \Gamma(x)$ *is convex on* $]0, +\infty[$.

### 2. PROPERTIES OF THE GAMMA FUNCTION

#### Proposition 2 {#fvr-vii-s1-prop-2 .statement}

*For every* $x > 0$ *one has*
$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x n!}{x(x+1)\ldots(x+n)}
$$
*(Gauss' formula)*, *and*
$$
\Gamma(x) = e^{-\gamma x} \frac{1}{x} \prod_{n=1}^{\infty} \frac{e^{x/n}}{1 + \frac{x}{n}}
$$
(9) where $\gamma$ denotes Euler’s constant, and the infinite product on the right hand side of (9) is absolutely and uniformly convergent on every compact interval of $\mathbf{R}$ not containing any integer $< 0$ (Weierstrass’ formula).

The function $\Gamma(x)$ is indefinitely differentiable on $]0, +\infty[$ and one has

$$
\frac{\Gamma'(x)}{\Gamma(x)} = -\gamma - \frac{1}{x} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{x+n} \right)
$$

and

$$
\mathrm{D}^k (\log \Gamma(x)) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(x+n)^k} \quad \text{for} \quad k \geq 2,
$$

the series on the right-hand sides of (10) and (11) being absolutely and uniformly convergent on every compact interval not containing any integer $\leq 0$.

Indeed, the proof of prop. 1 of VII, p. 306, shows that

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x (n-1)!}{x(x+1)\ldots(x+n-1)}
$$

whence Gauss’ formula, since $\frac{n}{x+n}$ tends to 1 as $n$ tends to $+\infty$. One can also write

$$
\log \frac{n}{n-1} = \frac{1}{n-1} + \left( \log \frac{n}{n-1} - \frac{1}{n-1} \right).
$$

so (in the notation of prop. 1)

$$
\exp(u_n(x)) = e^{(\log \frac{n}{n-1} - \frac{1}{n-1})} \frac{e^{x/(n-1)}}{1 + \frac{x}{n-1}}
$$

and the series with general term $\log \frac{n}{n-1} - \frac{1}{n-1}$ is absolutely convergent and has sum $-\gamma$, where $\gamma$ denotes Euler’s constant (V, p. 242), whence we obtain Weierstrass’ formula.

For $|x| \leq a$ one has $|1/(x+n)^k| \leq 1/(n-a)^k$ once $n > a$, so the series on the right-hand side in formula (11) is absolutely and uniformly convergent on every compact interval of $\mathbf{R}$ not containing any integer $\leq 0$, for any integer $k \geq 2$; the same argument applies to the right-hand side of (10), since $\left| \frac{1}{n} - \frac{1}{x+n} \right| \leq \frac{a}{n(n-a)}$ for $|x| \leq a$ and $n > a$. Since these series are obtained by differentiating the series

$$
\log \Gamma(x) = -\gamma x - \log x + \sum_{n=1}^{\infty} \left( \frac{x}{n} - \log \left( 1 + \frac{x}{n} \right) \right)
$$

term-by-term, and this converges for every $x > 0$, the series with general term $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ is absolutely and uniformly convergent on every compact interval contained in [0, +∞[, and one has the relations (10) and (11) of VII, p. 308, for every x > 0 (II, p. 52, th. 1). Moreover, for every x ∈ ℝ, the expression $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ is defined once n is large enough, so th. 1 of II, p. 52, again shows that the infinite product in the right-hand side of (9) (VII, p. 307) is absolutely and uniformly convergent on every compact interval containing no integer $\leq 0$.

The function $\Gamma(x)$, defined for $x > 0$, can be extended to the whole set of points x different from the integers $\leq 0$ so as to satisfy equation (7) of VII, p. 307, on this set: it suffices, for $-(n+1) < x < -n$, to put
$$
\Gamma(x) = \frac{1}{x(x+1)\ldots(x+n)} \Gamma(x+n+1).
$$
By prop. 2 of VII, p. 307, the formulae (8), (9), (10) and (11) of VII, p. 307 and 308, with $D^k(\log |\Gamma(x)|)$ replacing $D^k(\log \Gamma(x))$ in (11), remain valid on this set. Formula (9) (VII, p. 307) shows that $\Gamma(x) \sim 1/x$ as x tends to 0, whence, by (7) of VII, p. 307,
$$
\Gamma(x) \sim \frac{(-1)^n}{n! (x+n)}
$$
as x tends to $-n$ ($n$ an integer $\geq 0$). The function $1/\Gamma(x)$ can then be extended by continuity to all of ℝ, assigning it the value 0 at integers $\leq 0$; then, for all $x \in \mathbf{R}$
$$
\frac{1}{\Gamma(x)} = \lim_{n \to \infty} \frac{x(x+1)\ldots(x+n)}{n^n n!}
$$
and
$$
\frac{1}{\Gamma(x)} = e^{y_1 x} x \prod_{n=1}^{\infty} \left( 1 + \frac{x}{n} \right) e^{-y_1/n}
$$
and one shows as in prop. 2 of VII, p. 307, that the infinite product on the right of (13) is absolutely and uniformly convergent on every compact interval of ℝ.

Since $\Gamma(x) > 0$ for $x > 0$, equation (7) of VII, p. 307, shows that $\Gamma(x) < 0$ for $-(2n-1) < x < -(2n-2)$ and $\Gamma(x) > 0$ for
$$
-2n < x < -(2n-1)
$$
($n$ an integer $\geq 1$); also $\Gamma(x)$ has right limit $+\infty$ at the points $-2n$ and $-\infty$ at the points $-(2n+1)$, and has left limit $-\infty$ at the points $-2n$ and $+\infty$ at the points $-(2n+1)$ (for all $n \in \mathbf{N}$). Formula (11) of VII, p. 308, shows that, for $k = 2$, the right-hand side is always $\geq 0$ when it is defined, so
$$
\Gamma''(x) \Gamma(x) - (\Gamma'(x))^2 \geq 0,
$$

and consequently $\Gamma''(x)$ has the same sign as $\Gamma(x)$; thus $\Gamma$ is *convex* for $x > 0$ and for $-(2n+2) < x < -(2n+1)$, and *concave* for $-(2n+1) < x - 2n \ (n \in \mathbf{N})$; one deduces from this that, on the intervals where $\Gamma$ is convex, $\Gamma'(x)$ increases from $-\infty$ to $+\infty$, and on the intervals where $\Gamma$ is concave, $\Gamma'(x)$ decreases from $+\infty$ to $-\infty$. Whence the graph of $\Gamma$ (fig. 1).

**Fig. 1**

### 3. THE EULER INTEGRALS

For brevity we shall say that a function $f$ defined on an interval $I \subset \mathbf{R}$, and $> 0$ on this interval, is *logarithmically convex* on $I$ if $\log f$ is convex on $I$. The definition of $\Gamma(x)$ shows that this function is logarithmically convex on $]0, +\infty[$.

It is clear that the *product* of two logarithmically convex functions on $I$ is also logarithmically convex on $I$. Further:

#### Lemma 1 {#fvr-vii-s1-lem-1 .statement}

*Let $f$ and $g$ be two functions $> 0$ and twice differentiable on an open interval $I$. If $f$ and $g$ are logarithmically convex functions on $I$, then $f + g$ is logarithmically convex on $I$.*

The relation $D^2 (\log f(x)) \geq 0$ can be written $f(x)f''(x) - (f'(x))^2 \geq 0$. We are reduced to showing that the relations $a > 0, a' > 0, ac - b^2 \geq 0, a'c' - {b'}^2 \geq 0$ imply $(a + a')(c + c') - (b + b')^2 \geq 0$; now, when $a > 0$, the relation $ac - b^2 \geq 0$ is equivalent to the fact that the quadratic form $ax^2 + 2bxy + cy^2$ is $\geq 0$ on $\mathbf{R}^2$, and it is clear that if

$$
ax^2 + 2bxy + cy^2 \geq 0 \quad \text{and} \quad a'x^2 + 2b'xy + c'y^2 \geq 0
$$

on $\mathbf{R}^2$ then also $(a + a')x^2 + 2(b + b')xy + (c + c')y^2 \geq 0$ on $\mathbf{R}^2$.

#### Lemma 2 {#fvr-vii-s1-lem-2 .statement}

Let $f$ be a finite real function, $> 0$, defined and continuous on the product $I \times J$ of two open intervals of $\mathbf{R}$, and such that, for every $t \in J$ the function $x \mapsto f(x, t)$ is logarithmically convex and twice differentiable on $I$. Under these hypotheses, if the integral $g(x) = \int_J f(x, t) dt$ converges for every $x \in I$, then $g$ is logarithmically convex on $I$.

First we show that for every compact interval $K \subset J$ the function $g_K(x) = \int_K f(x, t) dt$ is logarithmically convex. Indeed, if $K = [a, b]$, the sequence of functions

$$
g_n(x) = \frac{b-a}{n} \sum_{k=0}^{n-1} f\left(x, a + k \frac{b-a}{n}\right)
$$

converges simply to $g_K(x)$ on $I$ (II, p. 57, prop. 5) hence $\log g_n$ converges simply to $\log g_K$; by lemma 1 of VII, p. 310, $\log g_n$ is convex on $I$, so (I, p. 27, prop. 4) it is the same for $\log g_K$.

On the other hand, $g$ is the pointwise limit of the $g_K$ along the directed set of compact subintervals of $I$ (II, p. 64), so $\log g$ is the pointwise limit of the $\log g_K$; these last functions being convex on $I$, so is $\log g$ (I, p. 27, prop. 4).

One can show easily that lemmas 1 and 2 remain valid even when one does not assume that the functions are twice differentiable (VII, p. 327, exerc. 5).

#### Lemma 3 {#fvr-vii-s1-lem-3 .statement}

Let $\varphi$ be a continuous function and $> 0$ on an open interval $J$ contained in $[0, +\infty[$. If $I$ is an open interval such that the integral $g(x) = \int_J t^{x-1} \varphi(t) dt$ converges for all $x \in I$, then $g$ is logarithmically convex on $I$.

Indeed, $\log t^{x-1} = (x-1) \log t$ is a function of $x$ which is convex and twice differentiable for all $t > 0$, so lemma 2 applies.

#### Proposition 3 {#fvr-vii-s1-prop-3 .statement}

For all $x > 0$

$$
\Gamma(x) = \int_0^\infty e^{-t} t^{x-1} dt
$$

(second Euler integral).

Now the function $g(x) = \int_0^\infty e^{-t} t^{x-1} dt$ is defined for all $x > 0$ (V, p. 229); lemma 3 of VII, p. 311, then shows that it is *logarithmically convex* on ]$0, +\infty[$. Moreover, on integrating by parts, one has

$$
g(x+1) = \int_0^\infty e^{-t} t^x \, dt = -e^{-t} t^x \Big|_0^\infty + x \int_0^\infty e^{-t} t^{x-1} dt = x \, g(x).
$$

Other words, $g$ is a solution of equation (1) of VII, p. 305; finally,

$$
g(1) = \int_0^\infty e^{-t} \, dt = 1;
$$

proposition therefore follows from prop. 1 of VII, p. 306.

By the change of variable $e^{-t} = u$ one deduces from (14) (VII, p. 311) the formula

$$
\Gamma(x) = \int_0^1 \left( \log \frac{1}{t} \right)^{x-1} dt.
$$

Similarly, from the change of variable $u = t^{1/x}$ we obtain

$$
x \, \Gamma(x) = \int_0^\infty e^{-t^{1/x}} \, dt
$$

again, taking account of (7) (VII, p. 3),

$$
\Gamma \left( 1 + \frac{1}{x} \right) = \int_0^\infty e^{-t^x} \, dt
$$

In particular, for $x = 2$

$$
\Gamma \left( \frac{3}{2} \right) = \frac{1}{2} \Gamma \left( \frac{1}{2} \right) = \int_0^\infty e^{-t^2} \, dt.
$$

#### Proposition 4 {#fvr-vii-s1-prop-4 .statement}

*For $x > 0$ and $y > 0$ the integral*

$$
\mathbf{B}(x, y) = \int_0^1 t^{x-1} (1-y)^{y-1} \, dt
$$

(*rst Euler integral*) *has the value*

$$
\mathbf{B}(x, y) = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$

Indeed this integral converges for $x > 0$ and $y > 0$ (V, p. 229). By lemma 3 of I, p. 311, the function $x \mapsto \mathbf{B}(x, y)$ is *logarithmically convex* for $x > 0$. Moreover,

$$
\mathbf{B}(x+1, y) = \int_0^1 (1-t)^{x+y-1} \left( \frac{t}{1-t} \right)^x \, dt
$$

Hence, on integrating by parts,

$$
\mathbf{B}(x+1, y) = -\frac{(1-t)^{x+y}}{x+y} \left( \frac{t}{1-t} \right)^x \Bigg|_0^1
+ \frac{x}{x+y} \int_0^1 (1-t)^{x+y} \left( \frac{t}{1-t} \right)^{x-1} \frac{dt}{(1-t)^2} = \frac{x}{x+y} \mathbf{B}(x, y).
$$

It follows that $f(x) = \mathbf{B}(x, y) \Gamma(x+y)$ satisfies the identity (1) of VII, p. 305
Moreover, this function is logarithmically convex, being the product of two logarithmically convex functions. Finally, one has $f(1) = \mathbf{B}(1, y) \Gamma(y+1)$, and $\mathbf{B}(1, y) = \int_0^1 (1-t)^{y-1} dt = 1/y$, whence $f(1) = \frac{1}{y} \Gamma(y+1) = \Gamma(y)$. The function $f(x)/\Gamma(y)$ is thus equal to $\Gamma(x)$ by prop. 1 of VII, p. 306, which proves (18).

By the change of variable $t = \frac{u}{u+1}$ the formula (18) becomes

$$
\int_0^\infty \frac{t^{x-1}}{(1+t)^{x+y}} dt = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}
$$
(19)

and by the change of variable $t = \sin^2 \varphi$

$$
\int_0^{\pi/2} \sin^{2x-1} \varphi \cos^{2y-1} \varphi d\varphi = \frac{1}{2} \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$
(20)

If one puts $x = y = \frac{1}{2}$ in this last formula it follows that

$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$
(21)

whence, by (17),

$$
\int_0^\infty e^{-t^2} dt = \frac{1}{2} \sqrt{\pi}.
$$
(22)

From the relation (7) of VII, p. 307, one has the asymptotic expansion

$$
\begin{align*}
\Gamma(x) &= \frac{1}{x} \Gamma(x+1) \\
&= \frac{1}{x} + \Gamma'(1) + \frac{1}{2!} \Gamma''(1)x + \cdots + \frac{1}{n!} \Gamma^{(n)}(1)x^{n-1} + O(x^n)
\end{align*}
$$
(23)

for $\Gamma(x)$, on a neighbourhood of 0.

Similarly, for all $y$ fixed and $> 0$ one can write

$$
\begin{align*}
\frac{1}{\Gamma(x+y)} &= \frac{1}{\Gamma(y)} + D \left( \frac{1}{\Gamma(y)} \right) x \\
&\quad + \frac{1}{2!} D^2 \left( \frac{1}{\Gamma(y)} \right) x^2 + \cdots + \frac{1}{n!} D^n \left( \frac{1}{\Gamma(y)} \right) x^n + O_1(x^{n+1})
\end{align*}
$$

and the formula (18) then gives, for $y$ fixed, the asymptotic expansion

$$
\mathbf{B}(x, y) = \frac{1}{x} + \left( \Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} \right)
+ \left( \frac{\Gamma''(1)}{2} - \Gamma'(1) \frac{\Gamma'(y)}{\Gamma(y)} + \frac{2{\Gamma'}^2(y) - \Gamma(y)\Gamma''(y)}{2\Gamma^2(y)} \right) x + O(x^2)
$$
on a neighbourhood of $x = 0$.

Moreover, for $x > 0$ and $y > 0$ one has
$$
\mathbf{B}(x, y) = \int_0^1 \left( t^{x-1} + t^x \frac{(1-t)^{y-1} - 1}{t} \right) dt
= \frac{1}{x} + \int_0^1 t^x \frac{(1-t)^{y-1} - 1}{t} dt.
$$
The function $\varphi(t) = \frac{(1-t)^{y-1} - 1}{t}$ is continuous on the compact interval $[0, 1]$; since
$$
t^x = e^{x \log t} = 1 + x \log t + \frac{x^2}{2!} (\log t)^2 + \cdots + \frac{x^n}{n!} (\log t)^n + r_n(x, t)
$$
with $|r_n(x, t)| \leq \frac{x^{n+1}}{(n+1)!} |\log t|^{n+1}$ (since $\log t \leq 0$ and $x > 0$), formula (25) gives the asymptotic expansion
$$
\mathbf{B}(x, y) = \frac{1}{x} + \int_0^1 \varphi(t) dt + x \int_0^1 \varphi(t) \log t \, dt + \cdots
+ \frac{x^n}{n!} \int_0^1 \varphi(t) (\log t)^n \, dt + O_2(x^{n+1})
$$
for $\mathbf{B}(x, y)$ on a neighbourhood of 0.

For $n = 1$ the identification of this expansion with (24) gives in particular
$$
\Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} = \int_0^1 \frac{(1-t)^{y-1} - 1}{t} dt.
$$

Furthermore, the formula (10) gives $\Gamma'(1) = \Gamma'(1)/\Gamma(1) = -\gamma$, so (*Gauss' integral*)
$$
\frac{\Gamma'(x)}{\Gamma(x)} + \gamma = \int_0^1 \frac{1 - (1-t)^{x-1}}{t} dt.
$$

### Exercises {#fvr-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
