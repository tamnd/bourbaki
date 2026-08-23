---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 2
section_title: INTEGRALS OVER NON-COMPACT INTERVALS
lang: en
source: fvr-i-vii
pdf_pages: 0077-0083, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 77
    - "no": 2
      title: INTEGRALS OF POSITIVE FUNCTIONS OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 81
    - "no": 3
      title: ABSOLUTELY CONVERGENT INTEGRALS
      page: 0
      pdf_page: 82
statements: 9
exercises: 9
content_sha256: 64275a842838d2080c7899bc5b116bdeafc42c93c4e521c8d9b045ecfe092f1d
---

## § 2. INTEGRALS OVER NON-COMPACT INTERVALS

### 1. DEFINITION OF AN INTEGRAL OVER A NON-COMPACT INTERVAL

Let I be a compact interval $[a,\ b]$ in the *extended line* $\overline{\mathbf{R}}$ ($a$ and $b$ may be infinite); let $f$ be a function defined on $[a,\ b[$, taking its values in a complete normed space E over $\mathbf{R}$. Generalizing def. 1 of II, p. 51, we shall say that a function $g$, defined on $[a,\ b]$ with values in E, is a *primitive* of $f$ if it is continuous on $[a,\ b]$ (and in particular at the endpoints $a$ and $b$) and admits a derivative equal to $f(x)$ at all the points of the complement with respect to $[a,\ b[$ of a countable subset of this interval.

We shall restrict ourselves to the following case: there exists a finite strictly increasing sequence $(c_i)_{0 \leq i \leq n}$ of points of $I = [a,\ b]$, such that $c_0 = a,\ c_n = b$, and such that $f$ is *regulated* on each of the open intervals $[c_i,\ c_{i+1}[$. Though not necessarily regulated on every open interval containing at least one point $c_i$ interior to $I$; such a function will be called *piecewise regulated* on $[a,\ b[$. We remark that a regulated function on $[a,\ b[$ is piecewise regulated (taking $n = 1$ in the preceding definition).

If $f$ admits a primitive $g$ (in the sense made precise above), and if $c$ is a point of the interval $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$, one has, by hypothesis, for each $x$ in this interval, that $g(x) - g(c) = \int_c^x f(t)\,dt$; since $g$ is continuous on $I$ by hypothesis, one sees that $\int_c^x f(t)\,dt$ tends to a limit in $E$ when $x$ tends to $c_i$ from the right and when $x$ tends to $c_{i+1}$ from the left. Conversely, suppose that these conditions are satisfied for all $t$, and let $g_i$ be a primitive of $f$ on the interval $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$; we note immediately that the function $g$, defined on the complement with respect to $I$ of the set of $c_i$, by the condition that it be equal to $g_i(x) + \sum_{k=1}^i (g_{k-1}(c_k-) - g_k(c_k+))$ on $[c_i,\ c_{i+1}[$ for $0 \leq i \leq n - 1$, is continuous at every point of $I$ distinct from the $c_i$ and admits a limit at each of these points; it can therefore be extended by continuity to each of these points, and the extended function is evidently a primitive of $f$ on $I$. It is clear, moreover, that every other primitive of $f$ is of the form $g + a$ ($a$ an element of $E$).

#### Definition 1 {#fvr-ii-s2-def-1 .statement}

*One says that a vector function* $f$, *piecewise regulated on an interval* $[a,\ b[$ *of* $\overline{\mathbf{R}}$, *admits an integral on this interval if* $f$ *admits a primitive on* $[a,\ b[$*; if* $g$ *is any one of the primitives of* $f$ *on* $[a,\ b[$*, and* $x_0$ *and* $x$ *are any two points of* $[a,\ b[$*, *one calls the element* $g(x) - g(x_0)$ *the integral of* $f$ *from* $x_0$ *to* $x$, *and one denotes it by* $\int_{x_0}^x f(t)\,dt$.

This concept clearly agrees with that defined when the interval $[x_0,\ x]$ contains none of the points $c_i$.

The remarks which precede def. 1 show that for $f$ to have an integral on $[a,\ b[$ it is necessary and sufficient that its restriction to each of the intervals $[c_i,\ c_{i+1}[$ should admit an integral over this interval. In other words, one reduces to the case where $f$ is regulated on a *non-compact* interval $I \subset \mathbf{R}$, with endpoints $a,\ b$ ($a < b$), and where: 1 either one of the numbers $a,\ b$ (at least) is infinite; 2 or $f$ is not regulated on a compact interval containing at least one of the points $a,\ b$ (these two hypotheses not being mutually exclusive). For $f$ to have an integral over $I$ it is necessary and sufficient that the integral $\int_a^x f(t)\,dt$ approaches a limit when the point $(x,\ y)$ approaches $(a,\ b) \in \overline{\mathbf{R}}^2$ while remaining in $I \times I$: and this limit is no other than $\int_a^b f(t)\,dt$ according to def. 1. By an abuse of language, instead of saying that $f$ has an integral over $I$, one says that the integral $\int_a^b f(t)\,dt$ is *convergent* (or *converges*).

#### Example {#fvr-ii-s2-n1-exa-1 .statement}

i) The integral $\int_1^{+\infty} dt/t^2$ is convergent and equal to 1, for
$$
\int_1^x \frac{dt}{t^2} = 1 - \frac{1}{x}.
$$

2) The integral $ \int_0^1 dt / \sqrt{t} $ is convergent and equal to 2, for
$$
\int_1^x \frac{dt}{\sqrt{t}} = 2(1 - \sqrt{x}) \quad \text{for} \quad x > 0.
$$

3) Let $ (\mathbf{u}_n)_{n \geq 1} $ be an infinite sequence of points of E, and let $ \mathbf{f} $ be the step function defined on the interval $ [1, +\infty[ $ by the conditions: $ \mathbf{f}(x) = \mathbf{u}_n $ for $ n \leq x < n+1 $. Then for the integral $ \int_1^{+\infty} \mathbf{f}(t)\,dt $ to be convergent it is necessary and sufficient that the series with general term $ \mathbf{u}_n $ be *convergent* in E; indeed, one has
$$
\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p,
$$
so the condition is necessary; conversely, if the series with general term $ \mathbf{u}_n $ converges in E, then $ \lim_{n \to \infty} \mathbf{u}_n = 0 $; now, if $ n \leq x \leq n+1 $, one has $ \int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p + \mathbf{u}_n(x-n) $. so this integral has the limit $ \sum_{n=1}^{\infty} \mathbf{u}_n $ when $ x $ tends to $ +\infty $.

It is immediate that if a piecewise regulated function $ \mathbf{f} $ admits an integral over I then the formulae (4) to (9) of II, p. 59 remain valid. Similarly, formula (10) of II, p. 59 extends in the following manner: $ \mathbf{f} $ and $ \mathbf{g} $ are assumed to be primitives of the regulated functions $ \mathbf{f}' $ and $ \mathbf{g}' $ on $ ]a,\ b[ $, and one denotes by $ [\mathbf{f}.\mathbf{g}]|_a^b $ the limit (if it exists) of $ [\mathbf{f}.\mathbf{g}]|_x^y $ as $ (x,\ y) $ tends to $ (a,\ b) $ (with $ a < x \leq y < b $); then, if two of the (three) expressions $ [\mathbf{f}.\mathbf{g}]|_a^b $, $ \int_a^b [\mathbf{f}(t).\mathbf{g}'(t)]\,dt $, and $ \int_a^b [\mathbf{f}'(t).\mathbf{g}(t)]\,dt $ have a meaning, then so has the third, and the formula (10) of II, p. 59 is valid.

Finally, let $ f $ be a real function which is defined and continuous on $ I = ]a,\ b[ $, and is the primitive of a regulated function $ f' $ on $ ]a,\ b[ $; let on the other hand $ g $ be a continuous vector function on an open interval J containing $ f(I) $; if the function $ g(f(x))f'(x) $ admits an integral over I, and if $ f $ tends to a limit (finite or not) at the points $ a $ and $ b $, then $ g $ admits an integral from $ f(a+) $ to $ f(b-) $, and one has the formula
$$
\int_a^b g(f(t))f'(t)\,dt = \int_{f(a+)}^{f(b-)} g(u)\,du.
$$
Indeed, if $ (x,\ y) $ tends to $ (a,\ b) $, then $ (f(x),\ f(y)) $ tends to $ (f(a+),\ f(b-)) $ by hypothesis; it suffices to apply formula (12) of II, p. 60 between $ x $ and $ y $, and to pass to the limit to obtain (1).

Given a regulated function $ \mathbf{f} $ on a non-compact interval $ I \subset \mathbf{R} $, with endpoints $ a $ and $ b $ ($ a < b $), the condition for $ \mathbf{f} $ to have an integral over I can be presented in the following manner. The compact intervals $ J \subset I $ form a *directed set* $ \mathcal{K}(I) $ with respect to the relation $ \subset ^1 $, for if $[ \alpha , \beta ]$ and $[ \gamma , \delta ]$ are two compact intervals contained in $ I $, and if one puts $ \lambda = \min(\alpha, \gamma) $, $ \mu = \max(\beta, \delta) $, then the interval $[ \lambda , \mu ]$ is contained in $ I $ and contains the two intervals considered. For each compact interval $ J = [ \alpha , \beta ] $ contained in $ I $, let us put

$$
\int_J f(t) \, dt = \int_\alpha^\beta f(t) \, dt;
$$

for $ f $ to admit an integral over $ I $ it is necessary and sufficient that the map $ J \mapsto \int_J f(t) \, dt $ have a limit with respect to the directed set $ \mathfrak{K}(I) $; this limit is then the integral $ \int_a^b f(t) \, dt $, which we again denote by $ \int_I f(t) \, dt $.

#### Proposition 1 (Cauchy’s criterion for integrals) {#fvr-ii-s2-prop-1 .statement}

*Let $ f $ be a regulated function on an interval $ I \subset \mathbf{R} $ having endpoints $ a $ and $ b $ ($ a < b $). For the integral $ \int_a^b f(t) \, dt $ to exist it is necessary and sufficient that for every $ \varepsilon > 0 $ there exist a compact interval $ J_0 = [\alpha, \beta] $ contained in $ I $, such that for any compact interval $ K = [x, y] $ contained in $ I $ and having no interior points in common with $ J_0 $, one has $ \| \int_K f(t) \, dt \| \leq \varepsilon $.*

Indeed, since $ E $ is complete the Cauchy criterion shows that for the integral $ \int_I f(t) \, dt $ to be convergent it is necessary and sufficient that for any $ \varepsilon > 0 $ there exists a compact interval $ J_0 = [\alpha, \beta] $ with for every compact interval $ J $ such that $ J_0 \subset J \subset I $ one has $ \| \int_J f(t) \, dt - \int_{J_0} f(t) \, dt \| \leq \varepsilon $. The proposition will follow from the following lemma:

*Lemma. Let $ J_0 = [\alpha, \beta] $ be a compact interval contained in $ I $. In order that $ \| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \| \leq \varepsilon $ for every pair of compact intervals $ J, J' $ contained in $ I $ and containing $ J' $ it is necessary that $ \| \int_K f(t) \, dt \| \leq \varepsilon $, and it suffices that $ \| \int_K f(t) \, dt \| \leq \varepsilon / 2 $, for every compact interval $ K $ contained in $ I $ and having no interior point in common with $ J_0 $.*

Indeed, if for $ J_0 \subset J \subset I $ and $ J_0 \subset J' \subset I $, one has

$$
\left\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \right\| \leq \varepsilon
$$

one sees in particular that, for $ x \leq y \leq \alpha $, or for $ \beta \leq x \leq y $ ($ x $ and $ y $ in $ I $), one has $ \| \int_x^y f(t) \, dt \| \leq \varepsilon $. Conversely, if $ \| \int_K f(t) \, dt \| \leq \varepsilon / 2 $ for every compact interval $ K \subset I $ such that $ K \cap J_0 = \emptyset $, and if $ J = [x, y] $, $ J' = [z, t] $ are two compact intervals contained in $ I $ and containing $ J_0 $, one has

1 Recall (*Set Theory*, III, p. 144) that a set $ \mathfrak{F} $ of subsets of $ I $ is *directed with respect to the relation* $ \subset $ if, for any $ X \in \mathfrak{F} $, $ Y \in \mathfrak{F} $, there exists $ Z \in \mathfrak{F} $ such that $ X \subset Z $ and $ Y \subset Z $. If $ S(X) $ denotes the subset of $ \mathfrak{F} $ formed by the $ U \in \mathfrak{F} $ such that $ U \supset X $, then the $ S(X) $ form a base for a filter on $ \mathfrak{F} $, called the *filter of sections* of $ \mathfrak{F} $; the limit (if it exists) of a map $ f $ of $ \mathfrak{F} $ into a topological space, with respect to the filter of sections of $ \mathfrak{F} $, is called the *limit of f with respect to the directed set* $ \mathfrak{F} $ (*cf. Gen. Top.*, I, p. 70 and *Gen. Top.*, IV, p. 348).

$$
\left\| \int_J f(t)\,dt - \int_{J'} f(t)\,dt \right\| = \left\| \int_x^z f(t)\,dt + \int_t^y f(t)\,dt \right\| \leq \varepsilon,
$$
since
$$
x \leq \alpha \leq \beta \leq y \quad \text{and} \quad z \leq \alpha \leq \beta \leq t.
$$

#### Example {#fvr-ii-s2-n1-exa-2 .statement}

If the interval I is *bounded*, and if $ f $ is *bounded* on I, then the integral $ \int_I f(t)\,dt $ always exists, for, by the mean value theorem, one has, for $ y \leq \alpha \leq \beta \leq z $,
$$
\left\| \int_y^\alpha f(t)\,dt \right\| \leq (\alpha - a) \sup_{t \in I} \|f(v)\| , \quad \left\| \int_\beta^z f(t)\,dt \right\| \leq (b - \beta) \sup_{t \in I} \|f(x)\|
$$
and it suffices to take $ \alpha - a $ and $ b - \beta $ small enough for the Cauchy criterion be satisfied.

One may note that in this case a primitive of $ f $ on I does not necessarily have a right (resp. left) derivative at the left-hand endpoint (resp. right-hand endpoint) of I (when this number is finite) contrary to the situation when I is compact and $ f $ is regulated on I (*cf.* II, p. 33, exerc. 1).

### 2. INTEGRALS OF POSITIVE FUNCTIONS OVER A NON-COMPACT INTERVAL

#### Proposition 2 {#fvr-ii-s2-prop-2 .statement}

*Let $ f $ be a real regulated function $ \geq 0 $ on an interval $ I \subset \mathbf{R} $ with endpoints $ a $ and $ b $ ($ a < b $). For the integral $ \int_a^b f(t)\,dt $ to exist it is necessary and sufficient that the set of numbers $ \int_J f(t)\,dt $ be bounded above when J runs through the set of compact intervals contained in I; the integral $ \int_a^b f(t)\,dt $ is then the least upper bound of the set of $ \int_J f(t)\,dt $.*

Indeed, since $ f \geq 0 $, the relation $ J \subset J' $ implies that
$$
\int_J f\,dt \leq \int_{J'} f\,dt;
$$
the map $ J \mapsto \int_J f\,dt $ is thus increasing, and the proposition follows from the monotone limit theorem (*Gen. Top.*, IV, p. 349, th. 2).

When the map $ J \mapsto \int_J f(t)\,dt $ is not bounded it has limit $ +\infty $ with respect to the directed set $ \mathcal{K}(I) $; then one says, by abuse of language, that the integral $ \int_a^b f(t)\,dt $ is equal to $ +\infty $. The properties of integrals established in n 1 extend (when dealing with functions $ \geq 0 $) to the case where certain of the integrals concerned are infinite, provided that the relations in which they feature make sense.

**PROPOSITION 3 (comparison principle).** *Let $ f $ and $ g $ be two real regulated functions on an interval $ I \subset \mathbf{R} $, such that $ 0 \leq f(x) \leq g(x) $ at each point where $ f $ and $ g $ are continuous (*cf.* II, p. 61, prop. 6). If the integral of $ g $ over $ I $ is convergent, so also is the integral of $ f $, and one has $ \int_I f(t)\,dt \leq \int_I g(t)\,dt $. Further, the two integrals cannot be equal unless $ f(x) = g(x) $ at every point of $ I $ where $ f $ and $ g $ are continuous.*

Now for every compact interval $ J \subset I $ one has

$$
\int_J f(t)\,dt \leq \int_J g(t)\,dt;
$$

since $ \int_J g(t)\,dt \leq \int_I g(t)\,dt $, the integrals $ \int_J f\,dt $ are bounded above, so the integral $ \int_I f(t)\,dt $ is convergent; further, on passing to the limit, one has $ \int_I f(t)\,dt \leq \int_I g(t)\,dt $. Suppose further that $ f(x) < g(x) $ at a point $ x \in I $ at which $ f $ and $ g $ are continuous; there exists a compact interval $[c,\ d]$ contained in $ I $, not reducing to a (single) point, and such that $ x \in [c,\ d] $; one has $ \int_c^d f(t)\,dt < \int_c^d g(t)\,dt $ (II, p. 61, cor. 1), and since on the other hand $ \int_a^c f(t)\,dt \leq \int_a^c g(t)\,dt $ and $ \int_d^b f(t)\,dt \leq \int_d^b g(t)\,dt $ from the above, one sees, on adding term-by-term, that $ \int_a^b f(t)\,dt < \int_a^b g(t)\,dt $.

This proposition provides the most frequently used means for deciding if the integral of a function $ f \geq 0 $ is or is not convergent: namely, comparing $ f $ to a simpler function $ g \geq 0 $ whose integral one already knows to be, or not to be, convergent; we shall see in chap. V how to search for comparator functions, in the most usual cases; and we shall deduce everyday criteria for the convergence of integrals and of series.

### 3. ABSOLUTELY CONVERGENT INTEGRALS

#### Definition 2 {#fvr-ii-s2-def-2 .statement}

*One says that the integral of a regulated function $ \mathbf{f} $ over an interval $ I \subset \mathbf{R} $ is absolutely convergent if the integral of the positive function $ \| \mathbf{f}(x) \| $ is convergent.*

#### Proposition 4 {#fvr-ii-s2-prop-4 .statement}

*If the integral of $ \mathbf{f} $ over $ I $ is absolutely convergent then it is convergent, and one has*

$$
\left| \int_I \mathbf{f}(t)\,dt \right| \leq \int_I \| \mathbf{f}(t) \| \,dt.\tag{2}
$$

Indeed, for every compact interval $ J \subset I $ one has (II, p. 61, formula (16))

$$
\left| \int_J \mathbf{f}(t)\,dt \right| \leq \int_J \| \mathbf{f}(t) \| \,dt.\tag{3}
$$

If the integral of the positive function $ \| \mathbf{f}(x) \| $ is convergent, then for every $ \varepsilon > 0 $ there exists a compact interval $[\alpha,\ \beta]$ contained in $ I $, such that, for every compact interval $[\lambda,\ \gamma]$ contained in $ I $ and having no interior point in common with $[\alpha,\ \beta]$, one has $ \int_{\lambda}^{\gamma} \| \mathbf{f}(t) \, dt \| \leq \varepsilon $ (II, p. 65, prop. 1); one deduces that $ \left| \int_{\lambda}^{\gamma} \mathbf{f}(t)\,dt \right| \leq \varepsilon $, which shows convergence of the integral over $ I $ (II, p. 16, prop. 1); on passing to the limit in (3) one deduces the inequality (2).

#### Corollary {#fvr-ii-s2-n3-cor-1 .statement}

*Let $ E, F, G $ be three complete normed spaces over $ \mathbf{R} $, and $ (x, y) \mapsto x.y $ a continuous bilinear map from $ E \times F $ into $ G $. Let $ \mathbf{f}, \mathbf{g} $ be two regulated functions on $ I $, with values in $ E $ and $ F $ respectively. If $ \mathbf{f} $ is bounded on $ I $ and if the* integral of g is absolutely convergent over I, then the integral of [f, g] is absolutely convergent.

Indeed, there exists a number h > 0 such that one has $ \| [x.y] \| \leq h \| x \| . \| y \| $ identically (Gen. Top., IX, p. 173, th. 1); if one puts $ k = \sup_{x \in I} \| f(x) \| $, then one has $ \| [f(x).g(x)] \| \leq h k \| g(x) \| $ on I; the comparison principle now shows that the integral of [f.g] is absolutely convergent, and, from (2),

$$
\left\| \int_I [f(t).g(t)] \, dt \right\| \leq h k \int_I \| g(t) \| \, dt.
$$

#### Remark {#fvr-ii-s2-n3-rem-1 .statement}

An integral can be convergent without being absolutely convergent; this is what is shown by Example 3 of II, p. 64, where the series with general term $ u_n $ is convergent without being absolutely convergent.

### Exercises {#fvr-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
