---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 2
section_title: EXPANSIONS OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS AND OF THE FUNCTIONS ASSOCIATED WITH THEM
lang: en
source: fvr-i-vii
pdf_pages: 0120-0128, 0140-0143
extraction: ocr
subsections:
    - "no": 1
      title: EXPANSION OF THE REAL EXPONENTIAL
      page: 0
      pdf_page: 120
    - "no": 2
      title: EXPANSIONS OF THE COMPLEX EXPONENTIAL, OF $\cos x$ AND $\sin x$
      page: 0
      pdf_page: 121
    - "no": 3
      title: THE BINOMIAL EXPANSION
      page: 0
      pdf_page: 122
    - "no": 4
      title: EXPANSIONS OF log(1 + x), OF Arc tan x AND OF Arc sin x
      page: 0
      pdf_page: 126
statements: 1
exercises: 9
content_sha256: f6b088ac6701be2b05fce77ca968574d31c178217f434b3fda6539f2d3368691
---

## § 2. EXPANSIONS OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS, AND OF THE FUNCTIONS ASSOCIATED WITH THEM

### 1. EXPANSION OF THE REAL EXPONENTIAL

Since $\mathrm{D}^n \left( e^x \right) = e^x$ the Taylor expansion of order $n$ for $e^x$ is

$$
e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + \int_0^x \frac{(x-t)^n}{n!} e^t \, dt. \tag{1}
$$

The remainder in this formula is $> 0$ for $x > 0$ and has the sign of $(-1)^{n+1}$ when $x < 0$; moreover, the inequality of the mean shows that

$$
\frac{x^{n+1}}{(n+1)!} < \int_0^x \frac{(x-t)^n}{n!} e^t \, dt < \frac{x^{n+1} e^x}{(n+1)!} \qquad \text{for } x > 0 \tag{2}
$$

$$
\frac{\left| x^{n+1} \right| e^x}{(n+1)!} < \left| \int_0^x \frac{(x-t)^n}{n!} e^t \, dt \right| < \frac{\left| x^{n+1} \right|}{(n+1)!} \qquad \text{for } x < 0 \tag{3}
$$

Now one knows that the sequence $\left( x^n / n! \right)$ has limit 0 when $n$ increases indefinitely, for all $x \geqslant 0$ (*Gen. Top.*, IV, p. 365); thus, keeping $x$ fixed and letting $n$ grow indefinitely in (1) it follows, from (2) and (3), that

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} \tag{4}
$$

and the series on the right-hand side is *absolutely and uniformly convergent* on every compact interval in $\mathbf{R}$. In particular, one has the formula

$$
e = 1 + \frac{1}{1!} + \frac{1}{2!} + \cdots + \frac{1}{n!} + \cdots \tag{5}
$$

This formula allows us to calculate rational approximations as close as we desire to the number $e$; one obtains

$$
e = 2.718\,281\,828\ldots
$$

to within $1/10^9$. Formula (5) proves, moreover, that $e$ is an *irrational* number $^{2}$ (*Gen. Top.*, IV, p. 375).

#### Remark {#fvr-iii-s2-n1-rem-1 .statement}

Since the remainder in formula (1) is $> 0$ for $x > 0$ one has, for $x > 0$

$$
e^x > 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^{n+1}}{(n+1)!}
$$

and *a fortiori*

$$
e^x > \frac{x^{n+1}}{(n+1)!}
$$

for every integer $n$ : one deduces from this that $e^x / x^n$ *tends to* $+\infty$ with $x$, for every integer $n$ : we shall find this result again in chap. V by another method (V, p. 231).

$^{2}$ CH. HERMITE proved in 1873 that $e$ is a *transcendental* number over the field $\mathbf{Q}$ of rational numbers (in other words, it is not the root of any polynomial with rational coefficients) (*Œuvres*, t. III, p. 150, Paris (Gauthier-Villars), 1912).

### 2. EXPANSIONS OF THE COMPLEX EXPONENTIAL, OF $\cos x$ AND $\sin x$

Let $z$ be an arbitrary complex number and consider the function $\varphi(t) = e^{zt}$ of the real variable $t$; we have $D^n \varphi(t) = z^n e^{zt}$ and $e^z = \varphi(1)$; expressing $\varphi(1)$ by means of its Taylor series of order $n$ about the point $t = 0$ (II, p. 62) thus gives

$$
e^z = 1 + \frac{z}{1!} + \frac{z^2}{2!} + \cdots + \frac{z^n}{n!} + z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

a formula which is equivalent to (1) when $z$ is real. The remainder

$$
r_n(z) = z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

in this formula can be bounded above, in absolute value, by using the inequality of the mean; if $z = x + i y$ we have $|e^{zt}| = e^{xt}$, so $|e^{zt}| \leq 1$ if $x \leq 0$, $|e^{zt}| \leq e^x$ if $x > 0$; hence

$$
|r_n(z)| \leq \frac{|z|^{n+1}}{(n+1)!} \text{ if } x \leq 0
$$
$$
|r_n(z)| \leq \frac{|z|^{n+1} e^x}{(n+1)!} \text{ if } x > 0.
$$

As above we conclude that

$$
e^z = \sum_{n=0}^\infty \frac{z^n}{n!}
$$

the series being *absolutely and uniformly convergent* on every compact subset of $\mathbf{C}$.

From (6) one deduces in particular that

$$
e^{ix} = 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \cdots + \frac{i^n x^n}{n!} + i^{n+1} \int_0^x \frac{(x-t)^n}{n!} e^{it} \, dt
$$

from which we deduce the Taylor expansions of $\cos x$ and $\sin x$; on taking the real part of (10) for order $2n+1$ we have

$$
\cos x = 1 - \frac{x^2}{2!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!} + (-1)^{n+1} \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

with remainder bounded by

$$
\left| \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt \right| \leq \frac{|x|^{2n+2}}{(2n+2)!}.
$$

Similarly, taking the imaginary part of (10) for order $2n$, we obtain

$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!}
$$
$$
+ (-1)^n \int_0^1 \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt
$$

with remainder bounded by

$$
\left| \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt \right| \leq \frac{|x|^{2n+1}}{(2n+1)!}.
$$

Moreover, on comparing the remainders in (11) for orders $2n+1$ and $2n+3$, we have

$$
\int_0^1 \frac{(x-t)^{2n+3}}{(2n+3)!} \cos t \, dt = \frac{x^{2n+2}}{(2n+2)!} - \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

and taking (12) into account we see that the remainder in (11) has the *same sign* as $(-1)^{n+1}$ no matter what $x$; in the same way we can show that the remainder in (13) has the *same sign* as $(-1)^n x$. In particular, for $n=0$ and $n=1$ in (11), and for $n=1$ and $n=2$ in (13) we obtain the inequalities

$$
1 - \frac{x^2}{2} \leq \cos x \leq 1 \quad \text{for all } x
$$
(15)

$$
x - \frac{x^3}{6} \leq \sin x \leq x \quad \text{for all } x \geq 0.
$$
(16)

Finally, on putting $z = i x$ in (9) we have

$$
\cos x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
$$
(17)

$$
\sin x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$
(18)

these series being absolutely and uniformly convergent on every compact interval.

It is clear, furthermore, that the formulae (17) and (18) remain valid for every *complex* $x$, the series on the right-hand side being absolutely and uniformly convergent on every compact subset of $\mathbf{C}$. In particular, for every $x$ (real or complex)

$$
\cosh x = \sum_{n=0}^\infty \frac{x^{2n}}{(2n)!}
$$
$$
\sinh x = \sum_{n=0}^\infty \frac{x^{2n+1}}{(2n+1)!}.
$$

### 3. THE BINOMIAL EXPANSION

Let $m$ be an *arbitrary* real number. For $x > 0$ we have

$$
D^n (x^m) = m(m-1)\ldots(m-n+1) x^{m-n};
$$

the Taylor formula of order $n$ about the point $x = 0$ for the function $(1 + x)^m$ shows that for every $x > -1$

$$
(1 + x)^m = 1 + \binom{m}{1} x + \binom{m}{2} x^2 + \cdots + \binom{m}{n} x^n + r_n(x)
$$

with

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt
$$

where we put $\binom{m}{n} = \frac{m(m-1)\ldots(m-n+1)}{n!}$. The formula (19) reduces to the binomial formula (Alg., I, p. 99) when $m$ is an integer $> 0$ and $n \geq m$; by extension, we again call it the *binomial formula*, and the coefficients $\binom{m}{n}$ are called the *binomial coefficients*, when $m$ is an *arbitrary* real number and $n$ is an arbitrary integer $> 0$.

The remainder in (19) has the same sign as $\binom{m}{n+1}$ if $x > 0$, and the sign of $(-1)^{n+1} \binom{m}{n+1}$ if $-1 < x < 0$. Since $\left| \frac{x-t}{1+t} \right| \leq |x|$ for $t > -1$ in the interval with endpoints 0 and $x$, we have the following bound for the remainder, for $m$ and $n$ arbitrary and $x > -1$:

$$
\left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt \right|
$$
$$
\leq \left| \binom{m-1}{n} x^n ((1+x)^m - 1) \right|.
$$

If we suppose $x \geq 0$, and $n \geq m-1$, then $(1+t)^{n-m+1} \geq 1$ on the interval of integration, so

$$
0 \leq \int_0^x \frac{(x-t)^n}{(1+t)^{n-m+1}} \, dt \leq \int_0^x (x-t)^n \, dt = \frac{x^{n+1}}{n+1}
$$

which gives the estimate

$$
|r_n(x)| \leq \left| \binom{m}{n+1} \right| x^{n+1} \quad (x \geq 0,\ n \geq m-1)
$$

for the remainder. On the other hand, suppose that $-1 \leq m < 0$; if one makes the change of variable $u = \frac{x-t}{x(1+t)}$ in the integral (19) one obtains

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} (1+x)^m x^{n+1} \int_0^1 \frac{u^n \, du}{(1+ux)^{m+1}}.
$$

To estimate the integral for $x > -1$ we remark that, since $m + 1 < 1$, the integral $\int_0^1 \frac{u^n \, du}{(1-u)^{m+1}}$ converges and bounds the right-hand side of (22) since $1 + u x > 1 - u$. Now, for $-1 < x < 0$ the hypothesis on $m$ implies that all the terms $\binom{m}{1} x, \binom{m}{2} x^2, \ldots, \binom{m}{n} x^n$ which appear in the right-hand side of (19) are $\geq 0$, and hence $r_n(x) \leq (1 + x)^m$, from which, on dividing by $(1 + x)^m$,

$$
\frac{m(m-1) \ldots (m-n)}{n!} x^{n+1} \int_0^1 \frac{u^n \, du}{(1 + u x)^{m+1}} \leq 1.
$$

Moreover, for $-1 < x < 0$ the factor in front of the integral is $\geq 0$, so, letting $x$ approach $-1$,

$$
\left| \frac{m(m-1) \ldots (m-n)}{n!} \int_0^1 \frac{u^n \, du}{(1-u)^{m+1}} \right| \leq 1
$$

and consequently for $-1 \leq m < 0$ and $x > -1$ we have

$$
|r_n(x)| \leq (1 + x)^m |x|^{n+1}.
$$ (23)

From these inequalities we can, for a start, deduce that for $|x| < 1$ we have

$$
(1 + x)^m = \sum_{n=0}^\infty \binom{m}{n} x^n
$$ (24)

the right-hand side (called the binomial series) being absolutely and uniformly convergent on every compact subset of $]-1, +1[$. Indeed one can write

$$
\binom{m}{n} = (-1)^n \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n} \right)
$$ (25)

whence

$$
\left| \binom{m}{n} \right| \leq \left( 1 + \frac{|m+1|}{1} \right) \left( 1 + \frac{|m+1|}{2} \right) \ldots \left( 1 + \frac{|m+1|}{n} \right).
$$

If $|x| \leq r < 1$ there is an $n_0$ such that $1 + \frac{|m|}{n_0} < \frac{1}{r'}$, where $r < r' < 1$; whence, putting

$$
k = \left( 1 + \frac{|m|}{1} \right) \left( 1 + \frac{|m|}{2} \right) \ldots \left( 1 + \frac{|m|}{n_0} \right)
$$

we have

$$
\left| \binom{m-1}{n} x^n \right| \leq k |x|^{n_0} \left( \frac{r}{r'} \right)^{n - n_0},
$$

which proves the proposition. On the other hand, for $x > 1$, the absolute value of the general term of the series (24) increases indefinitely with $n$ if $m$ is not an integer $\geq 0$; indeed, from (25), we have for $n > n_1 \geq |m+1|$

$$
\left| \binom{m}{n} \right| \geq \left| \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right|
$$
$$
\left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n} \right).
$$

Let $n_0 \geq n_1$ be such that for $n \geq n_0$ we have $1 - \frac{|m+1|}{n} > \frac{1}{x'}$, where $1 < x' < x$. If we put
$$
k' = \left| \left( 1 - \frac{m+1}{1} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right| \left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n_0} \right)
$$
then, for $n > n_0$,
$$
\left| \binom{m}{n} x^n \right| \geq k' |x|^{n_0} \left( \frac{x}{x'} \right)^{n-n_0}
$$
from which the proposition follows.

We remark that for $m = -1$ the algebraic identity
$$
\frac{1}{1+x} = 1 - x + x^2 - \cdots + (-1)^{n-1} x^{n-1} + (-1)^n \frac{x^n}{1+x}
$$
gives the expression for the remainder in the general formula (19) without having to integrate; the formula (23) reduces in this case to the expression for the sum of the geometric series (or progression) (Gen. Top., IV, p. 364).

In the second place let us study the convergence of the binomial series for $x = 1$ or $x = -1$ (excluding the trivial case $m = 0$):

$a) \ m \leq -1$. The product with general term $1 - \frac{m+1}{n}$ converges to $+\infty$ if $m < -1$, to 1 if $m = -1$, so it follows from (25) that for $x = \pm 1$ the general term of the binomial series does not tend to 0.

$b) \ -1 < m < 0$. This time the product with general term $1 - \frac{m+1}{n}$ converges to 0, so the inequality (21) shows that $r_n(1)$ tends to 0. Thus the binomial series converges for $x = 1$ and has sum $2^m$; moreover, the binomial series is uniformly convergent on every interval $]x_0, 1]$ with $-1 < x_0 \leq 1$, by virtue of what we saw above and of (21). On the other hand, for $x = -1$ all the terms on the right-hand side of (24) are $\geq 0$, if this series were convergent one could deduce that the binomial series would be normally convergent on $[-1, 1]$ and so would have for its sum a continuous function on this interval, which is absurd because $(1+x)^m$ is not bounded on $[-1, 1]$ for $m < 0$. We conclude that also for $x = 1$ the binomial series is not absolutely convergent.

$c) \ m > 0$. The definition of $r_n(x)$ shows that $r_n(x)$ tends to the limit $r_n(-1)$ when $x$ tends to $-1$; on passing to the limit in (20) one concludes that $|r_n(-1)| \leq \left| \binom{m-1}{n} \right|$, and since $m-1 > -1$ we see that for $x = -1$ the binomial series is convergent. Furthermore, for $n > m+1$ all the terms of this series have the same sign; thus the binomial series is normally convergent on the interval [−1, 1] and has sum (1 + x)^m on this interval.

### 4. EXPANSIONS OF log(1 + x), OF Arc tan x AND OF Arc sin x

Let us integrate the two sides of (26) between 0 and x; we obtain the Taylor expansion of order n of log(1 + x), valid for x > −1

$$
\log(1 + x) = \frac{x}{1} - \frac{x^2}{2} + \frac{x^3}{3} + \cdots + (-1)^n \frac{x^n}{n} + (-1)^n \int_0^x \frac{t^n \, dt}{1 + t}.
$$ (27)

The remainder has the same sign as (−1)^n if x > 0, and is < 0 if −1 < x < 0; further, when x > 0, we have 1 + t ≥ 1 for 0 ≤ t ≤ x, and, when −1 < x < 0, we have 1 + t ≥ 1 − |x| for x ≤ 0; whence the estimates for the remainder

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{n+1} \quad \text{for } x \geq 0 \tag{28}
$$

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{(n+1)(1-|x|)} \quad \text{for } -1 < x \leq 0. \tag{29}
$$

From these last two formulae one deduces immediately that for −1 < x ≤ 1 one has

$$
\log(1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n}
$$ (30)

the series being uniformly convergent on every compact interval contained in ]−1, +1], and absolutely convergent for |x| < 1.

On the other hand, for |x| > 1 the general term in the series on the right-hand side of (30) increases indefinitely in size with n (III, p. 106). For x = −1 the series reduces to the harmonic series, which has sum +∞ (Gen. Top., IV, p. 365).

Similarly, let us replace x by x^2 in (26) and integrate both sides between 0 and x; we obtain the Taylor expansion of order 2n − 1 for Arc tan x, valid for all real x

$$
\operatorname{Arc tan} x = \frac{x}{1} - \frac{x^3}{3} + \frac{x^5}{5} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{2n-1} + (-1)^n \int_0^x \frac{t^{2n} \, dt}{1 + t^2}. \tag{31}
$$

The remainder has the sign of (−1)^n x, and since 1 + t^2 ≥ 1 for all t we have the estimate

$$
\left| \int_0^x \frac{t^{2n} \, dt}{1 + t^2} \right| \leq \frac{|x|^{2n+1}}{2n+1} \tag{32}
$$

from which one deduces that, for |x| ≤ 1,

$$
\operatorname{Arc tan} x = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^{2n-1}}{2n-1} \tag{33}
$$

the series being uniformly convergent on [−1, +1], and absolutely convergent for |x| < 1.

In particular, for x = 1 one obtains the formula

$$
\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} + \cdots + (-1)^n \frac{1}{2n+1} + \cdots .
$$

For |x| > 1 the general term of the right-hand side of (33) increases indefinitely in size with n.

Finally, for the Taylor expansion of Arc sin x we start from the expansion of its derivative (1 − x^2)^{-1/2}; this last expansion is obtained by replacing x by −x^2 in the expansion of (1 + x)^{-1/2} as a binomial series; for |x| < 1 this gives

$$
(1 - x^2)^{-1/2} = 1 + \frac{1}{2} x^2 + \frac{1.3}{2.4} x^4 + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} x^{2n} + r_n(x)
$$

with, by (23), the bound

$$
0 \leq r_n(x) \leq \frac{x^{2n+2}}{\sqrt{1-x^2}}
$$

for the remainder.

On taking the primitive of the preceding expansion we obtain

$$
\text{Arc sin } x = x + \frac{1}{2} \frac{x^3}{3} + \frac{1.3}{2.4} \frac{x^5}{5} + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1} + R_n(x)
$$

where R_n(x) has the sign of x and satisfies the inequality

$$
|R_n(x)| \leq \int_0^x \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

Further, the relation (35) shows that R_n(x) tends to a limit when x approaches 1 or −1, so one has

$$
|R_n(1)| \leq \int_0^1 \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

But the right-hand side of (37) tends to 0 when n tends to +∞ : for, since the integral $\int_0^1 dt / \sqrt{1-t^2}$ is convergent, for every ε > 0 there is an a such that 0 < a < 1 and $\int_a^1 dt / \sqrt{1-t^2} \leq \varepsilon$; on the other hand we have

$$
\int_0^a \frac{t^{2n+2} dt}{\sqrt{1-t^2}} \leq \frac{1}{\sqrt{1-a^2}} \int_0^a t^{2n+2} dt = \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}}
$$

and so there is an n_0 such that for n ≥ n_0 one has $\frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}} \leq \varepsilon$, whence, finally, |R_n(x)| ≤ 2ε for |x| ≤ 1 and n ≥ n_0. Thus one has

$$
\operatorname{Arc}\sin x = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1}
$$

(38)

the right-hand side being normally convergent on the compact interval [−1, 1].

In the opposite case one can show, as for the binomial series, that the general term in the series on the right-hand side of (38) increases indefinitely in absolute value for |x| > 1.
On putting $x = \frac{1}{2}$, for example, in (38) we obtain a new expression for the number $\pi$:

$$
\frac{\pi}{6} = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{1}{(2n+1)2^{2n+1}}
$$

which is much better suited than formula (34) to calculating approximations to $\pi$ (see Calcul numérique); one thus obtains

$$
\pi = 3.141\,592\,653\ldots
$$

accurate to within $1/10^9$.³

³ The number $\pi$ is not only irrational (cf. III, p. 126, exerc. 5) but even transcendental over the field $\mathbf{Q}$ of rational numbers, as was shown for the first time in 1882 by Lindemann (see for example D Hilbert, Gesammelte Abhandlungen, v. 1, p. 1, Berlin (Springer), 1932).

### Exercises {#fvr-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
