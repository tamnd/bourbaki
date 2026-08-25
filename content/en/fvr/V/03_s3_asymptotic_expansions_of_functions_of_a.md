---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 3
section_title: ASYMPTOTIC EXPANSIONS OF FUNCTIONS OF A REAL VARIABLE
lang: en
source: fvr-i-vii
pdf_pages: 0242-0251, 0275-0276
extraction: ocr
subsections:
    - "no": 1
      title: 'INTEGRATION OF COMPARISON RELATIONS: **I. WEAK RELATIONS**'
      page: 0
      pdf_page: 243
    - "no": 2
      title: 'APPLICATION: LOGARITHMIC CRITERIA FOR CONVERGENCE OF INTEGRALS'
      page: 0
      pdf_page: 244
    - "no": 3
      title: 'INTEGRATION OF COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 0
      pdf_page: 245
    - "no": 4
      title: DIFFERENTIATION OF COMPARISON RELATIONS
      page: 0
      pdf_page: 247
    - "no": 5
      title: PRINCIPAL PART OF A PRIMITIVE
      page: 0
      pdf_page: 248
    - "no": 6
      title: ASYMPTOTIC EXPANSION OF A PRIMITIVE
      page: 0
      pdf_page: 250
statements: 23
exercises: 7
content_sha256: 94e95163a3bddf8b03b27bd79764ed5052fd05b0911efb3d64c9ba96e17155c0
---

## § 3. ASYMPTOTIC EXPANSIONS OF FUNCTIONS OF A REAL VARIABLE

In this section we shall consider only the case where the set $ E $ is an open interval in the extended real line $ \overline{\mathbf{R}} $, and $ \mathfrak{F} $ is a base for the trace on $ E $ of the filter of neighbourhoods of the left or right-hand endpoint $ \alpha $ of $ E $; further, we shall study above all the (finite) real functions defined on a set in $ \mathfrak{F} $ (depending on the function under consideration).

Using one of the changes of variable $ x' = -x,\ x' = \frac{1}{x-\alpha},\ x' = -\frac{1}{x-\alpha} $ as needed, one can always reduce to the case where E is an interval of the form ]$a, +\infty[$ so that $ \mathfrak{F} $ will be formed of intervals $[t, +\infty[$ with $ t > a $. We shall restrict ourselves principally to this latter case, and leave the task of translating most of the propositions we obtain (by the above changes of variable) to the reader, except for a few particularly important results.

It will be convenient to employ an abuse of language and refer to the sets in $ \mathfrak{F} $ as "neighbourhoods of $ +\infty $".

### 1. INTEGRATION OF COMPARISON RELATIONS: **I. WEAK RELATIONS**

#### Proposition 1 {#fvr-v-s3-prop-1 .statement}

*Let $ \mathbf{f} $ be a regulated vector function, $ g $ a regulated function $ \geqslant 0 $ on an interval $[a, +\infty[$, such that $ \int_a^{+\infty} g(t)\,dt > 0 $. The relation $ \mathbf{f} \preccurlyeq g $ as $ x $ tends to $ +\infty $ implies that $ \int_a^x \mathbf{f}(t)\,dt \preccurlyeq \int_a^x g(t)\,dt $. If the integral $ \int_a^{+\infty} g(t)\,dt $ converges then the integral $ \int_a^{+\infty} \mathbf{f}(t)\,dt $ converges absolutely.*

Indeed, by hypothesis there exist a $ b \geqslant a $ and a number $ c' > 0 $ such that
$$
\| \mathbf{f}(x) \| \leqslant c' g(x) \quad \text{for } x \geqslant b,
$$
whence
$$
\left\| \int_b^x \mathbf{f}(t)\,dt \right\| \leqslant \int_b^x \| \mathbf{f}(t) \| \,dt \leqslant c' \int_b^x g(t)\,dt;
$$
since, moreover, one may suppose $ b $ so large that $ \int_a^b g(t)\,dt > 0 $, there exists a $ c'' > 0 $ such that $ \left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leqslant c'' \int_a^b g(t)\,dt $; on putting $ c = \max(c', c'') $ one thus has
$$
\left\| \int_a^x \mathbf{f}(t)\,dt \right\| \leqslant c \int_a^x g(t)\,dt
$$
for every $ x \geqslant b $, whence the proposition.

#### Corollary 1 {#fvr-v-s3-prop-1-cor-1 .statement}

*If $ f $ and $ g $ are regulated functions and $ \geqslant 0 $ on the interval $[a, +\infty[$, and such that $ f \succcurlyeq g $, and if $ \int_a^{+\infty} g(t)\,dt = +\infty $, then $ \int_a^{+\infty} f(t)\,dt = +\infty $.*

#### Corollary 2 {#fvr-v-s3-prop-1-cor-2 .statement}

*If $ f $ and $ g $ are $ \geqslant 0 $ and not identically zero on $[a, +\infty[$, and such that $ f \succeq g $, then $ \int_a^x f(t)\,dt \succeq \int_a^x g(t)\,dt $.*

### 2. APPLICATION: LOGARITHMIC CRITERIA FOR CONVERGENCE OF INTEGRALS

By choosing the function g suitably one can deduce criteria for deciding whether the integral $ \int_a^{+\infty} f(t) \, dt $ of a function $ f \geq 0 $ converges or is infinite from prop. 1 of V, p. 228, and cor. 1 thereto: it suffices to choose for g a function whose primitive is known. In particular, since $ x^\mu $ has primitive $ \frac{x^{\mu+1}}{\mu+1} $ when $ \mu \neq -1 $, and $ \log x $ when $ \mu = -1 $, we have the following criterion:

#### Proposition 2 ("logarithmic criterion of order 0") {#fvr-v-s3-prop-2 .statement}

*Let f be a regulated function $ \geq 0 $ on an interval $[a, +\infty[$; if $ f(x) \preccurlyeq x^\mu $ for some $ \mu < -1 $ then the integral $ \int_a^{+\infty} f(t) \, dt $ converges; if $ f(x) \succcurlyeq x^\mu $ for some $ \mu \geq -1 $ then the integral $ \int_a^{+\infty} f(t) \, dt $ is infinite.*

This criterion is not decisive when $ 1/x^{1+\alpha} \ll f(x) \ll 1/x $ for *every* exponent $ \alpha > 0 $, as, for example, when $ f(x) = 1/x(\log x)^\mu $ ($ \mu > 0 $). But in this last case f has primitive $ \frac{1}{1-\mu} (\log x)^{1-\mu} $ if $ \mu \neq 1 $ and $ \log \log x $ when $ \mu = 1 $. Thus:

#### Proposition 3 ("logarithmic criterion of order 1") {#fvr-v-s3-prop-3 .statement}

*Let f be a regulated function $ \geq 0 $ on an interval $[a, +\infty[$; if $ f(x) \preccurlyeq 1/x(\log x)^\mu $ for some $ \mu > 1 $ then the integral $ \int_a^{+\infty} f(t) \, dt $ converges; if $ f(x) \succcurlyeq 1/x(\log x)^\mu $ for some $ \mu \leq 1 $ then the integral $ \int_a^{+\infty} f(t) \, dt $ is infinite.*

Generally, for every integer $ n \geq 0 $, let us denote by $ l_n(x) $ the function defined inductively (for x large enough) by the relations $ l_0(x) = x $, $ l_n(x) = \log(l_{n-1}(x)) $ for $ n \geq 1 $; one says that $ l_n(x) $ is the *n*th *iterated logarithm of x* (cf. Appendix). One verifies immediately that $ \frac{1}{1-\mu} (l_n(x))^{1-\mu} $ is a primitive of

$$
\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}
$$

for $ \mu \neq 1 $, and $ l_{n+1}(x) $ is a primitive of $ \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) l_n(x)} $. Hence:

#### Proposition 4 ("logarithmic criterion of order n") {#fvr-v-s3-prop-4 .statement}

*Let f be a regulated function $ \geq 0 $ on an interval $[a, +\infty[$; if, for some $ \mu > 1 $, $ f(x) \preccurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu} $, then the integral $ \int_a^{+\infty} f(t) \, dt $ converges; if $ f(x) \succcurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu} $ for some $ \mu \leq 1 $, then the integral $ \int_a^{+\infty} f(t) \, dt $ is infinite.*

Each logarithmic criterion is thus applicable to functions for which the criteria of lower order are not decisive (*cf.* V, p. 264, exerc. 5 b) and V, p. 265, exerc. 8).

Because of its usefulness we translate the criterion of order 0 for integrals $ \int_{\alpha}^{a} f(t) \, dt $ where $ f $ is regulated and $ \geq 0 $ on a non-compact interval $ ]\alpha, a] $:

#### Proposition 5 ("logarithmic criterion of order 0") {#fvr-v-s3-prop-5 .statement}

*If on a neighbourhood of $ \alpha $ one has $ f(x) \leq 1/(x-\alpha)^{\mu} $ for some $ \mu < 1 $ then the integral $ \int_{\alpha}^{a} f(t) \, dt $ converges; if $ f(x) \geq 1/(x-\alpha)^{\mu} $ for some $ \mu \geq 1 $ then the integral $ \int_{\alpha}^{a} f(t) \, dt $ is infinite.*

We leave it to the reader to translate the logarithmic criterion of order $ n $ similarly.

The application of the logarithmic criteria is immediate if one knows how to obtain the *principal part* of $ f $ with respect to a comparison scale containing the functions that feature in these criteria: if $ f_1 $ is the principal part, the integral $ \int_{\alpha}^{+\infty} f(t) \, dt $ converges or is infinite together with $ \int_{\alpha}^{+\infty} f_1(t) \, dt $, and the logarithmic criteria apply immediately to this last integral.

#### Example 1 {#fvr-v-s3-n2-exa-1 .statement}

The function $ t^p(1-t)^q $ is not bounded on $ ]0, 1[ $ when $ p < 0 $ or $ q < 0 $; by the logarithmic criterion of order 0 applied on a neighbourhood of the points 0 and 1 the integral $ \int_{0}^{1} t^p(1-t)^q \, dt $ converges if and only if $ p > -1 $ and $ q > -1 $. If so, this integral is called the *Eulerian integral of the first kind* and is denoted by $ \mathbf{B}(p+1, q+1) $ (*cf.* VII, p. 312).

#### Example 2 {#fvr-v-s3-n2-exa-2 .statement}

Consider the integral $ \int_{0}^{+\infty} t^{\lambda-1} e^{-t} \, dt $. Since $ e^{-t} \sim 1 $ on a neighbourhood of 0, one must have $ \lambda > 0 $ if this integral is to converge; this condition is also sufficient since on a neighbourhood of $ +\infty $ one has $ e^{-t} \ll t^{-\mu} $ for any $ \mu > 0 $. When $ x > 0 $ the integral is called the *Eulerian integral of the second kind* and is denoted by $ \Gamma(x) $ (*cf.* VII, p. 311).

### 3. INTEGRATION OF COMPARISON RELATIONS: II. STRONG RELATIONS

#### Proposition 6 {#fvr-v-s3-prop-6 .statement}

*Let $ \mathbf{f} $ be a regulated vector function, and $ g $ a regulated function $ \geq 0 $ on $ [a, +\infty[ $.*

1. *If the integral $ \int_{a}^{+\infty} g(t) \, dt $ converges then the relation $ \mathbf{f} \ll g $ (resp. $ \mathbf{f} \sim c g $, where $ c $ is constant) implies that $ \int_{x}^{+\infty} \mathbf{f}(t) \, dt \ll \int_{x}^{+\infty} g(t) \, dt $ (resp. $ \int_{x}^{+\infty} \mathbf{f}(t) \, dt \sim c \int_{x}^{+\infty} g(t) \, dt $).

2. *If the integral $ \int_{a}^{+\infty} g(t) \, dt $ is infinite then the relation $ \mathbf{f} \ll g $ (resp. $ \mathbf{f} \sim c g $) implies that*
$$
\int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \ll \int_{\beta}^{\gamma} g(t) \, dt \quad \text{(resp. } \int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \sim c \int_{\beta}^{\gamma} g(t) \, dt),
$$
*for any $ \alpha $ and $ \beta $ in $ [a, +\infty[ $*.

It is enough to prove the proposition for the relation $ \mathbf{f} \ll g $ since, if $ c \neq 0 $, the relation $ \mathbf{f} \sim c g $ is equivalent to $ \mathbf{f} - c g \ll g $.

The first part is an immediate consequence of the mean value theorem, since if $ \| \mathbf{f}(x) \| \leq \varepsilon g(x) $ for $ x \geq x_0 $ one deduces that

$$
\left\| \int_{x}^{+\infty} \mathbf{f}(t) \, dt \right\| \leq \int_{x}^{+\infty} \| \mathbf{f}(t) \| \, dt \leq \varepsilon \int_{x}^{+\infty} g(t) \, dt \quad \text{for } x \geq x_0.
$$

In the second place, suppose that $ \int_{a}^{+\infty} g(t) \, dt = +\infty $. If $ \| \mathbf{f}(x) \| \leq \varepsilon g(x) $ for $ x \geq x_0 \geq \max(\alpha, \beta) $, one has

$$
\begin{align*}
\int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt &= \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \int_{x_0}^{x} \| \mathbf{f}(t) \| \, dt \\
&\leq \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \varepsilon \int_{x_0}^{x} g(t) \, dt \\
&= \varepsilon \int_{\beta}^{x} g(t) \, dt + \left( \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right).
\end{align*}
$$

Now there exists an $ x_1 \geq x_0 $ such that for every $ x \geq x_1 $

$$
\left| \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right| \leq \varepsilon \int_{\beta}^{x} g(t) \, dt
$$

whence, for $ x \geq x_1 $

$$
\left\| \int_{\alpha}^{x} \mathbf{f}(t) \, dt \right\| \leq \int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt \leq 2\varepsilon \int_{\beta}^{x} g(t) \, dt
$$

which completes the proof, since $ \varepsilon > 0 $ is arbitrary.

In other words, one can integrate the two terms of a strong relation $ \mathbf{f} \ll g $, $ \mathbf{f} \sim \mathbf{a}g $, when $ g $ is positive on an interval $[a, +\infty[$, and the relation persists between the primitives of the two terms, provided one takes care to integrate from $ x $ to $ +\infty $ if $ \int_{a}^{+\infty} g(t) \, dt $ converges, and from $ \alpha $ to $ x $ (for any $ \alpha $ in $[a, +\infty[$) in the opposite case.

Note that props. 1 (V, p. 228) and 6 (V, p. 230) remain valid when $ \mathfrak{F} $ is a base for the trace filter of the intervals $[t, +\infty[$ (where $ t > a $) on the complement of a countable set (cf. I, p. 15, th. 2).

#### Example 1 {#fvr-v-s3-n3-exa-1 .statement}

On applying prop. 6 of V, p. 230, to the relation $ 1/x \ll x^{\alpha-1} $ where $ \alpha > 0 $, one again obtains the relation $ \log x \ll x^{\alpha} $ for every $ \alpha > 0 $, which is equivalent to the relation $ y^{1/\alpha} \ll e^y $ proved in III, p. 105.

#### Example 2 {#fvr-v-s3-n3-exa-2 .statement}

We have $ \left( \frac{e^t}{x} \right)' = \frac{e^t}{x} \left( 1 - \frac{1}{x} \right) \sim e^t / x $; since $ e^t / x $ tends to $ +\infty $ with $ x $, one deduces from prop. 6 of V, p. 230, that $ \int_{1}^{x} \frac{e^t}{t} \, dt \sim e^x / x $.

#### Remark {#fvr-v-s3-n3-rem-1 .statement}

When $ g $ is not assumed to remain $ \geq 0 $ on an interval $[a, +\infty[$ (or to remain $ \leq 0 $ on such an interval), and $ \int_{a}^{+\infty} g(t) \, dt $ is not convergent, the relation $ f \sim g $ does not necessarily imply that $ \int_{a}^{x} f(t) \, dt \sim \int_{a}^{x} g(t) \, dt $, as is shown by the example where $ g(x) = \sin x $ and $ f(x) = \left( 1 + \frac{\sin x}{x} \right) \sin x $; here

$$
\int_{n\pi}^{(n+1)\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{(n+1)\pi} \int_{0}^{\pi} \sin^2 t \, dt \geq \frac{1}{2} \int_{n+1}^{n+2} \frac{dt}{t},
$$

whence
$$
\int_{\pi}^{n\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{2} \int_2^{n+1} \frac{dt}{t}
$$
and the integral $ \int_1^{+\infty} dt/t $ is infinite, though $ \int_{\frac{\pi}{2}}^x g(t) \, dt = -\cos x $ remains bounded (see V, p. 260, exerc. 4).

### 4. DIFFERENTIATION OF COMPARISON RELATIONS

Propositions 1 (V, p. 228) and 6 (V, p. 230) do not have converses: the existence of a comparison relation $ f \preccurlyeq g,\ f \ll g,\ f \sim cg $ between two functions that are differentiable on a neighbourhood of $ +\infty $ does not imply the same comparison relation between their derivatives, even for real monotone functions $ f $ and $ g $.

For example, the function $ x^2 + x \sin x + \cos x $ is monotone and equivalent to $ x^2 $, but its derivative $ x(2 + \cos x) $ is not equivalent to $ 2x $.

On the other hand, one can derive comparison relations when one assumes a priori that the derivatives of the functions considered are comparable (V, p. 217). In general, we shall say that two real functions $ f $ and $ g $ defined on an interval $[a, +\infty[$ are comparable to order $ k $ on a neighbourhood of $ +\infty $ if, on a neighbourhood of $ +\infty $, they each have a regulated $ k^{th} $ derivative except at a countable set of points, and if, on this neighbourhood, $ f^{(k)} $ and $ g^{(k)} $ have constant sign (on the set on which they are defined) and are comparable.

We agree to say that two comparable real functions (V, p. 217) are comparable of order 0.

#### Proposition 7 {#fvr-v-s3-prop-7 .statement}

If two real functions $ f,\ g $, are comparable of order 1, then they are comparable; further, the relation $ f \ll g $ (resp. $ f \sim cg $, $ c $ constant) implies $ f' \ll g' $ (resp. $ f' \sim cg' $) unless $ g $ is equivalent to a nonzero constant.

Now, since $ f' $ and $ g' $ are of constant sign on an interval $[x_0, +\infty[$, both $ f $ and $ g $ are monotone on this interval, so tend to a finite or infinite limit as $ x $ tends to $ +\infty $. It is clear that $ f $ and $ g $ are comparable as $ x $ tends to $ +\infty $ if one of these limits is finite and $ \neq 0 $, or if one is zero and the other infinite. If both $ f $ and $ g $ tend to 0 one can write $ f(x) = -\int_x^{+\infty} f'(t) \, dt,\ g(x) = -\int_x^{+\infty} g'(t) \, dt $; since $ f' $ and $ g' $ are comparable the same is true for $ f $ and $ g $ and the comparison relation between $ f $ and $ g $ is the same as that between $ f' $ and $ g' $, by prop. 6 (V, p. 20). Similarly, if $ f $ and $ g $ both have an infinite limit one has $ f(x) = f(x_0) + \int_{x_0}^x f'(t) \, dt,\ g(x) = g(x_0) + \int_{x_0}^x g'(t) \, dt $; again prop. 6 (V, p. 230) shows that $ f $ and $ g $ are comparable and that the comparison relation between $ f $ and $ g $ is the same as that between $ f' $ and $ g' $. To complete the proof it remains to consider the case where $ g $ tends to $ \pm \infty $ and $ f $ to a constant: one cannot then have $ f' \succcurlyeq g' $, since then one could deduce from prop. 1 (V, p. 218) that the integral $ \int_{x_0}^{+\infty} g'(t) \, dt $ was convergent; since $ f' $ and $ g' $ have been assumed comparable, one must have $ f' \ll g' $.

#### Corollary {#fvr-v-s3-n4-cor-1 .statement}

*If two real functions $ f, g $, are comparable of order $ k \geqslant 1 $, then they are comparable of order $ p $ for $ 0 \leqslant p \leqslant k $; further, the relation $ f \ll g $ (resp. $ f \sim cg $) implies $ f^{(k)} \ll g^{(k)} $ (resp. $ f^{(k)} \sim cg^{(k)} $) unless one of the derivatives $ g^{(p)} $ ($ 0 \leqslant p \leqslant k - 1 $) is equivalent to a constant $ \neq 0 $.

Indeed, since $ f^{(k)} $ and $ g^{(k)} $ have constant sign on an interval $[x_0, +\infty[$, it follows that $ f^{(k-1)} $ and $ g^{(k-1)} $ are monotone on this interval, so have constant sign on a neighbourhood of $ +\infty $; further, prop. 7 of V, p. 232, shows that $ f^{(k-1)} $ and $ g^{(k-1)} $ are comparable, so the corollary follows from applying prop. 7 recursively.

#### Remark 1 {#fvr-v-s3-n4-rem-1 .statement}

The restriction on $ g $ in prop. 7 is essential. For example, one has $ \frac{1}{x} \ll 1 + \frac{1}{x} $ even though the derivatives of the two sides are equivalent; similarly $ 1 + \frac{1}{x} \sim 1 + \frac{1}{x^2} $, but $ 1/x^2 \gg 2/x^3 $.

#### Remark 2 {#fvr-v-s3-n4-rem-2 .statement}

Though $ f $ and $ g $ are comparable of order $ k $ a function $ f_1 $ equivalent to $ f $ need not be comparable of order $ k $ to $ g $; however it will be so if one assumes that $ f_1 $ is comparable of order $ k $ to $ f $ and that none of the derivatives $ f^{(p)} $ ($ 0 \leqslant p \leqslant k - 1 $) is equivalent to a nonzero constant.

#### Remark 3 {#fvr-v-s3-n4-rem-3 .statement}

If $ f $ and $ g $ are comparable of order $ k $ this need not be so for $ hf $ and $ hg $ even for a monotone function $ h $ as simple as $ h(x) = x $ (V, p. 260, exerc. 3); likewise, $ 1/f $ and $ 1/g $ are not necessarily comparable of order $ k $ (V, p. 259, exerc. 1).

### 5. PRINCIPAL PART OF A PRIMITIVE

Let $ f $ be a regulated real function $ \neq 0 $ having constant sign on an interval $[a, +\infty[$; the following proposition allows one to obtain the principal part of the primitive $ \int_a^{+\infty} f(t)\,dt $ if $ \int_a^{+\infty} f(t)\,dt $ converges in certain cases, and of the primitive $ \int_a^x f(t)\,dt $ if $ \int_a^{+\infty} f(t)\,dt $ is infinite:

#### Proposition 8 {#fvr-v-s3-prop-8 .statement}

*Put* $ F(x) = \int_x^{+\infty} f(t)\,dt $ *if* $ \int_a^{+\infty} f(t)\,dt $ *converges*, *and* $ F(x) = \int_a^x f(t)\,dt $ *if* $ \int_a^{+\infty} f(t)\,dt $ *is infinite*. *Suppose that* $ \log|f| $ *and* $ \log x $ *are comparable of order* 1.

1 *If* $ f $ *is of finite order* $ \mu \neq -1 $ *with respect to* $ x $ *one has*
$$
F(x) \sim \frac{1}{|\mu+1|} x f(x).
$$
(1)

2 *If* $ f $ *is of infinite order relative to* $ x $ *and if* $ f/f' $ *and* $ x $ *are comparable of order* 1, *then one has*
$$
F(x) \sim \frac{(f(x))^2}{|f'(x)|}.
$$
(2)

One should note that the hypothesis implies that $ f(x) $ has a determinate order relative to $ x $ (V, p. 219).

1 *If* $ f $ *is of order* $ \mu \neq 0 $ *relative to* $ x $ *one has* $ \log|f| \sim \mu \log x $, *so, since* $ \log|f| $ *and* $ \log x $ *are comparable of order* 1, *by prop. 7 of V, p. 232 one has* $ f'/f \sim $ μ/x, whence $ x f' \sim \mu f $. If $ \mu > -1 $ one has $ f(x) \gg x^{\mu-\varepsilon} $ for every $ \varepsilon > 0 $, and hence (V, p. 229, prop. 2) the integral $ \int_a^{+\infty} f(t)\,dt $ is infinite. One can write $ F(x) = \int_a^x f(t)\,dt = x f(x) - af(a) - \int_a^x t f'(t)\,dt $, whence again
$$
\int_a^x (f(t) + t f'(t))\,dt = x f(x) - af(a);
$$
since $ \mu \neq -1 $ we have $ f(x) + x f'(x) \sim (\mu + 1) f(x) $, so (V, p. 230, prop. 6)
$$
\int_a^x (f(t) + t f'(t))\,dt \sim (\mu + 1) F(x),
$$
which proves (1) in this case. If $ \mu = 0 $ one has likewise that $ x f'(x) \ll f(x) $, which again gives $ f(x) + x f'(x) \sim f(x) $. One argues similarly when $ \mu < -1 $, in the case where $ \int_a^{+\infty} f(t)\,dt $ converges.

2) If $ f $ is of order $ +\infty $ relative to $ x $ one has $ \log |f| \gg \log x $, so (V, p. 232, prop. 7) $ f'/f \gg 1/x $, or again, putting $ g(x) = f(x)/f'(x) $, $ g(x) \ll x $; further, since $ f(x) \gg x^\alpha $ for every $ \alpha > 0 $ the integral $ \int_a^{+\infty} f(t)\,dt $ is infinite. One can write
$$
F(x) = \int_a^x f(t)\,dt = \int_a^x g(t) f'(t)\,dt = g(x) f(x) - g(a) f(a) - \int_a^x f(t) g'(t)\,dt;
$$
since $ g $ and $ x $ are comparable of order 1, from the relation $ g(x) \ll x $ one can deduce (V, p. 232, prop. 7) that $ g'(x) \ll 1 $, hence that $ f g' \ll f $, and consequently (V, p. 230, prop.6)
$$
\int_a^x f(t) g'(t)\,dt \ll F(x),
$$
which establishes the relation (2). The proof is similar when $ f $ is of order $ -\infty $ relative to $ x $, in the case where $ \int_a^{+\infty} f(t)\,dt $ converges.

Let $ \mathcal{E} $ be a comparison scale (for real $ x $ tending to $ +\infty $) formed of nonzero real functions that are of constant sign on a neighbourhood of $ +\infty $, such that $ x \in \mathcal{E} $ and such that the product and quotient of two functions in $ \mathcal{E} $ again belongs to $ \mathcal{E} $ (V, p. 221 and p. 224). If a regulated function $ f $ with constant sign on a neighbourhood of $ +\infty $ has a principal part $ c g $ relative to $ \mathcal{E} $, then $ \int_x^{+\infty} f(t)\,dt $ (resp. $ \int_a^x f(t)\,dt $ according to the case) will be equivalent to $ c \int_x^{+\infty} g(t)\,dt $ (resp. $ c \int_a^x g(t)\,dt $); if the function $ g $ satisfies the hypotheses of prop. 8 of V, p. 233, and if (when the formula (2) of V, p. 233, applies) one knows a principal part of $ g' $ relative to $ \mathcal{E} $, one will thus have a principal part of $ \int_x^{+\infty} f(t)\,dt $ (resp. $ \int_a^x f(t)\,dt $) relative to $ \mathcal{E} $.

#### Example 1 {#fvr-v-s3-n5-exa-1 .statement}

The function $ 1/\log x $ is of order 0 relative to $ x $ and satisfies the conditions of prop. 8 of V, p. 233; thus
$$
\int_a^x \frac{dt}{\log t} \sim \frac{x}{\log x}.
$$
2) The function $ e^{t^2} $ is of order $ +\infty $ relative to $ x $ and satisfies the conditions of prop. 8, so
$$
\int_a^x e^{t^2}\,dt \sim \frac{1}{2x}\,e^{x^2}.
$$

In the Appendix (V, p. 252) we shall define a set of functions for which prop. 7 and prop. 8 always apply.

#### Remark {#fvr-v-s3-n5-rem-1 .statement}

Prop. 8 does not apply directly to a function $ f $ of order $-1$ relative to $ x $. But then one can write $ f(x) = f_1(x)/x $, with $ f_1 $ of order 0 relative to $ x $. Suppose, for example, that $ \int_a^{+\infty} f(t)\,dt $ is infinite; then

$$
F(x) = \int_a^x f(t)\,dt = \int_a^x \frac{1}{t} f_1(t)\,dt = \int_{\log a}^{\log x} f_1(e^u)\,du.
$$

If the function $ f_1(e^t) $ satisfies the hypotheses of prop. 8 and has an order $ \neq -1 $ relative to $ y $ (that is, if $ f_1(x) $ has an order $ \neq -1 $ relative to $ \log x $) the formulae (1) and (2) again allow us to obtain a principal part for $ F(x) $. For example, let $ f(x) = \frac{\exp(\sqrt{\log x})}{x \log x} $; since $ \exp(\sqrt{\log x}) $ is of order 0 relative to $ x $, $ f $ is of order $-1$; here one has $ f_1(e^t) = e^{\sqrt{t}}/y $, and this function is of order $ +\infty $ relative to $ y $; prop. 8 applies and gives $ \int_a^x e^{\sqrt{u}}/u\,du \sim 2e^{\sqrt{y}}/\sqrt{y} $: on reverting to the variable $ x $ we have $ \int_a^x \frac{\exp(\sqrt{\log t})}{t \log t}\,dt \sim \frac{2\exp(\sqrt{\log x})}{\sqrt{\log x}} $.

### 6. ASYMPTOTIC EXPANSION OF A PRIMITIVE

Let $ \mathcal{E} $ be a comparison scale on a neighbourhood of $ +\infty $ formed of real functions $ \neq 0 $ of constant sign on a neighbourhood of $ +\infty $; let $ \mathbf{f} $ be a regulated vector function defined on an interval $[a,\,+\infty[$, with values in a complete normed space $ E $, admitting an asymptotic expansion

$$
\mathbf{f} = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda + \mathbf{r}_\alpha
$$

to precision $ g_\alpha $ relative to $ \mathcal{E} $. Suppose further that every primitive $ \int_a^x g(t)\,dt $ of a function $ g \in \mathcal{E} $ admits an asymptotic expansion with respect to $ \mathcal{E} $. In these circumstances we shall see that one can obtain an asymptotic expansion of $ F(x) = \int_a^x \mathbf{f}(t)\,dt $ with respect to $ \mathcal{E} $. We distinguish two cases:

1. $ \int_a^{+\infty} g_\alpha(t)\,dt $ is infinite; then one has $ \int_a^x \mathbf{r}_\alpha(t)\,dt \ll \int_a^x g_\alpha(t)\,dt $ (V, p. 230, prop. 6); by hypothesis one can obtain an asymptotic expansion of $ \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt $ to a certain precision $ g_\rho $ (V, p. 222); if $ c g_\sigma $ is the principal part of $ \int_a^x g_\alpha(t)\,dt $ one will thus have an asymptotic expansion of $ \int_a^x \mathbf{f}(t)\,dt $ to precision $ g_{\min(\rho,\sigma)} $, with all the terms having indefinitely increasing norms.

2. $ \int_a^{+\infty} g_\alpha(t)\,dt $ converges; let $ \beta $ then be the smallest of the indices $ \lambda \leq \alpha $ such that $ \mathbf{a}_\lambda \neq 0 $ and such that $ \int_a^{+\infty} g_\lambda(t)\,dt $ converges; the integral

$$
C = \int_a^{+\infty} \left( \mathbf{f}(t) - \sum_{\lambda < \beta} \mathbf{a}_\lambda g_\lambda(t) \right) dt
$$

is then convergent, and one can write

$$
F(x) = \sum_{\lambda < \beta} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt + C - \sum_{\beta \leq \lambda \leq \alpha} \mathbf{a}_\lambda \int_a^{+\infty} g_\lambda(t)\,dt - \int_a^{+\infty} \mathbf{r}_\alpha(t)\,dt.
$$

Then $ \int_a^{+\infty} r_\alpha(t) \, dt \ll \int_1^{+\infty} g_\alpha(t) \, dt $; if $ c g_\sigma $ is the principal part of $ \int_1^{+\infty} g_\alpha(t) \, dt $, and if one has an asymptotic expansion of

$$
\sum_{\lambda < \beta} a_\lambda \int_a^\lambda g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda \leq \alpha} a_\lambda \int_\lambda^{+\infty} g_\lambda(t) \, dt
$$

to precision $ g_\rho $, one will as a result have an asymptotic expansion of $ F $ to precision $ g_{\min(\rho, \sigma)} $.

So it all amounts to finding asymptotic expansions with respect to $ \mathcal{E} $ of *primitives of functions in* $ \mathcal{E} $. We have seen how, subject to certain hypotheses on $ \mathcal{E} $, prop. 8 of V, p. 233 gives the principal part of such a primitive. Further, the proof of prop. 8 gives the expression for the difference of the two sides of formula (1) (resp. (2)) of V, p. 233, in the form of a primitive of the function $ \frac{1}{|\mu + 1|} (x f'(x) + f(x)) - f(x) $ (resp. $ f(x) g'(x) $ with $ g = f/f' $); on forming the principal part of this new primitive, as an asymptotic expansion of the right-hand side of (1) (resp. (2)), one obtains the right-hand side of the sought-for expansion (see V, p. 247-255).

#### Example 1 {#fvr-v-s3-n6-exa-1 .statement}

Let $ f(x) = 1/\log x $ ($ x > 1 $); we have seen that $ \int_a^\lambda dt / \log t \sim x / \log x $, and that the difference $ \int_a^\lambda \frac{dt}{\log t} - \frac{\lambda}{\log \lambda} $ is a primitive of $ 1/(\log x)^2 $; one can apply prop. 8 again to this function, so obtaining $ \int_a^\lambda dt / (\log t)^2 \sim x / (\log x)^2 $. By recursion one thus obtains the expansion

$$
\int_a^\lambda \frac{dt}{\log t} = \frac{x}{\log x} + \frac{x}{(\log x)^2}
+ \frac{2x}{(\log x)^3} + \cdots + (n-1)! \frac{x}{(\log x)^n} + o \left( \frac{x}{(\log x)^n} \right).
$$

Note that, irrespective of $ n $, all the terms of this expansion tend to $ +\infty $ with $ x $.

#### Example 2 {#fvr-v-s3-n6-exa-2 .statement}

Let $ f(x) = \frac{e^x}{x^2 + 1} $; one can write $ f(x) = \frac{e^x}{x^2} - \frac{e^x}{x^4} + o_1 \left( \frac{e^x}{x^4} \right) $. Prop. 8 gives the expansions

$$
\int_a^\lambda \frac{e^t}{t^2} \, dt = \frac{e^x}{x^2} + \frac{2e^x}{x^3} + \frac{6e^x}{x^4} + o_2 \left( \frac{e^x}{x^4} \right), \quad \int_a^\lambda \frac{e^t}{t^4} \, dt = \frac{e^x}{x^4} + o_3 \left( \frac{e^x}{x^4} \right)
$$

whence, on adding,

$$
\int_a^\lambda \frac{e^t}{t^2 + 1} \, dt = \frac{e^x}{x^2} + 2 \frac{e^x}{x^3} + 5 \frac{e^x}{x^4} + o_4 \left( \frac{e^x}{x^4} \right).
$$

### Exercises {#fvr-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
