---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 3
section_title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
lang: en
source: fvr-i-vii
pdf_pages: 0303-0305, 0311-0312
extraction: ocr
subsections:
    - "no": 1
      title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
      page: 0
      pdf_page: 303
    - "no": 2
      title: APPLICATION TO ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 304
statements: 0
exercises: 3
content_sha256: b90058728ed6629413e6ddb0b487cfedb0fe875b20fb58e137a5696743e86033
---

## § 3. BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA

### 1. BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA

The estimate obtained in (16) for the Bernoulli polynomials on the interval $[0, 1]$ allows one to estimate the remainder $ T_p(x, n) $ in the Euler-Maclaurin summation formula (VI, p. 282, formula (39)) easily:

$$
\left\{
\begin{array}{l}
f(x) + f(x+1) + \cdots + f(x+n) \\
\phantom{=} = \int_x^{x+n+1} f(t)\,dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
\phantom{=} \phantom{=} + \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n).
\end{array}
\right.
$$

Indeed, one has (VI, p. 283, formula (41))

$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s)\,ds
$$

where $ \overline{B}_{2p+1}(t) $ is the periodic function of period 1 equal to $ B_{2p+1}(t) $ on the interval $[0, 1[$. The formula (16) of VI, p. 288, shows that

$$
|\overline{B}_{2p+1}(t)| \leq 4e^{2\pi} \frac{(2p+1)!}{(2\pi)^{2p+1}}
$$
(3)

for all $ t \in \mathbf{R} $, and applying the mean value formula gives the estimate

$$
|T_p(x, n)| \leq \frac{4e^{2\pi}}{(2\pi)^{2p+1}} \int_x^{x+n+1} |f^{(2p+1)}(t)| \, dt
$$
(4)

for $ T_p(x, n) $.

### 2. APPLICATION TO ASYMPTOTIC EXPANSIONS

The Euler-Maclaurin formula allows one to give a more complete solution (in the most important cases) to the problem treated in V, p. 238 to 242, that of obtaining an asymptotic expansion of the partial sum $ s_n = \sum_{m=0}^n g(m) $ (resp. of the remainder $ r_n = \sum_{m=n+1}^\infty g(m) $), where $ g $ is a scalar function, $ > 0 $, monotone, defined on $ [0, +\infty[ $.

We shall restrict ourselves to the case where $ g $ is an (H) function (V, p. 252), of order 0 relative to $ e^x $; in other words, one has the relation $ g' \ll g $; from this relation one deduces $ g^{(k+1)} \ll g^{(k)} $ for every integer $ k > 0 $ such that none of the derivatives $ g^{(h)} $ of order $ h \leq k $ is equivalent to a constant (V, p. 232, prop. 7). Let $ p $ be an integer such that none of the derivatives $ g^{(h)} $ of order $ h \leq 2p $ is equivalent to a constant. First we assume that the series with general term $ g(n) $ has infinite sum, and distinguish several cases:

1. $ |g^{(2p-1)}(n)| $ tends to $ +\infty $ with $ n $; we have the same, by the hypothesis, for $ |g^{(2k-1)}(n)| $ for $ 1 \leq k \leq p $; further, since $ g^{(2p+1)} $ is monotone on a neighbourhood of $ +\infty $, the formula (4) of VI, p. 289, gives $ T_p(0, n) = O(g^{(2p)}(n+1)) = o(g^{(2p-1)}(n+1)) $; the Euler-Maclaurin formula, applied for $ x = 0 $, shows that

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t) \, dt - \frac{1}{2} g(n+1)
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

each of the terms of this sum being negligible relative to the preceding one; on expanding each of them relative to a comparison scale $ \mathcal{E} $ one will then have an asymptotic expansion for $ s_n $.

2) Now suppose that for an index $ q $ such that $ 1 \leq q \leq p $ we have $ |g^{(2q-1)}(n)| $ tending to $ +\infty $ with $ n $, but that $ g^{(2k-1)}(n) $ tends to 0 for $ k > q $. Since $ g^{(2p+1)} $ is monotone on a neighbourhood of $ +\infty $ the integral $ \int_0^\infty |g^{(2p+1)}(u)| \, du $ converges, and one can then write

= $ \sum_{m=0}^{n} g(m) = \int_0^{n+1} g(t)\,dt - \frac{1}{2}g(n+1) + \sum_{k=1}^{q} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + C $
$$
+ \sum_{k=q+1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right)
$$
C is a constant: indeed
$$
\int_{n+1}^{\infty} |g^{(2p+1)}(u)|\,du = O\left(g^{(2p)}(n+1)\right) = o\left(g^{(2p-1)}(n+1)\right).
$$
The same formula is valid when $ g(n) $ itself tends to 0. Finally, when the series general term $ g(n) $ converges one has, for the remainder $ r_n = \sum_{m=n+1}^{\infty} g(m) $, the expansion
$$
= \sum_{m=n+1}^{\infty} g(m) = \int_{n+1}^{\infty} g(t)\,dt + \frac{1}{2}\,g(n+1)
$$
$$
- \sum_{k=1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right).
$$

### Exercises {#fvr-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
