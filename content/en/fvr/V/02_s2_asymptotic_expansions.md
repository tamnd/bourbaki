---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 2
section_title: ASYMPTOTIC EXPANSIONS
lang: en
source: fvr-i-vii
pdf_pages: 0235-0242
extraction: ocr
subsections:
    - "no": 1
      title: SCALES OF COMPARISON
      page: 0
      pdf_page: 235
    - "no": 2
      title: PRINCIPAL PARTS AND ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 236
    - "no": 3
      title: SUMS AND PRODUCTS OF ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 238
    - "no": 4
      title: COMPOSITION OF ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 239
    - "no": 5
      title: ASYMPTOTIC EXPANSIONS WITH VARIABLE COEFFICIENTS
      page: 0
      pdf_page: 241
statements: 12
exercises: 0
content_sha256: 6dbb80b4d9ced8125da9a25c398bf8dcaeecf4ed6cdb3e6fcc1e622bcbf5063e
---

## § 2. ASYMPTOTIC EXPANSIONS

### 1. SCALES OF COMPARISON

Let E be a set filtered by a filter with base $ \mathfrak{F} $, and K a non-discrete valued field (most often $ K = \mathbf{R} $ or $ K = \mathbf{C} $). In the set of functions in $ \mathcal{H}(\mathfrak{F}, K) $ not equivalent to 0 modulo $ R_\infty $ (that is, those for which in every set in $ \mathfrak{F} $ there is at least one point where the function does not vanish), the relation " $ f \ll g $ or $ f = g $" is an order relation.

#### Definition 1 {#fvr-v-s2-def-1 .statement}

*One says that a subset $ \mathcal{E} $ of $ \mathcal{H}(\mathfrak{F}, K) $ formed of functions not equivalent to 0 modulo $ R_\infty $ is a comparison scale when $ \mathcal{E} $ is totally ordered by the relation " $ f \ll g $ or $ f = g $".*

In other words, if $ f $ and $ g $ are functions in $ \mathcal{E} $ then one (and only one) of the relations $ f \ll g $, $ g \ll f $, $ f = g $ always holds. It follows that on $ \mathcal{E} $ *the relation* $ f \asymp g $ (and *a fortiori* $ |f| \sim a\,|g| $, where $ a $ is a number $ > 0 $) *implies* $ f = g $.

Every subset of a comparison scale is clearly also a comparison scale.

#### Example 1 {#fvr-v-s2-n1-exa-1 .statement}

For $ x $ real and tending to $ +\infty $ the set of functions $ x^\alpha $ ($ \alpha $ an arbitrary real number) is a comparison scale. The same is true for the functions $ (x-a)^\alpha $ when $ \mathfrak{F} $ is the set of open intervals with left-hand endpoint $ a $.

#### Example 2 {#fvr-v-s2-n1-exa-2 .statement}

For $ z $ complex tending to $ \infty $ the set of functions $ z^n $ ($ n $ a rational integer) is a comparison scale; so are the functions $ (z-a)^n $ when $ \mathfrak{F} $ is the trace on the complement of the point $ a \in \mathbf{C} $ of the filter of neighbourhoods of this point.

#### Example 3 {#fvr-v-s2-n1-exa-3 .statement}

Let F be normed space; the family of functions $ \|x-\mathbf{a}\|^\alpha $ ($ \alpha $ an arbitrary real number) is a comparison scale when $ \mathfrak{F} $ is the trace on the complement of $ \mathbf{a} $ of the filter of neighbourhoods of this point. Note that if $ p $ and $ q $ are two distinct norms on F, the union of the two comparison scales $ (p(x-\mathbf{a}))^\alpha $ and $ (q(x-\mathbf{a}))^\alpha $ is not in general a comparison scale.

#### Example 4 {#fvr-v-s2-n1-exa-4 .statement}

For $ x $ real tending to $ +\infty $ the family $ \mathcal{E} $ of functions of the form $ \exp(p(x)) $, where $ p $ runs through the set of *polynomials without constant term* (with real coefficients), is a comparison scale: it suffices to remark that the quotient of two functions in $ \mathcal{E} $ is again in $ \mathcal{E} $, and that a function $ \exp(p(x)) $ must tend either to 0 or $ +\infty $ if $ p \neq 0 $; indeed, $ p(x) \sim \alpha x^n $ where $ n > 0 $ and $ \alpha \neq 0 $; if $ \alpha > 0 $ then $ p(x) > \frac{1}{2} \alpha x^n $ for $ x $ sufficiently large; if $ \alpha < 0 $ then $ p(x) < \frac{1}{2} \alpha x^n $ for $ x $ sufficiently large; in the first case $ \exp(p(x)) $ tends to $ +\infty $, in the second to 0.

#### Example 5 {#fvr-v-s2-n1-exa-5 .statement}

For $ x $ real tending to $ +\infty $ the set $ \mathcal{E} $ of functions of the form $ x^\alpha (\log x)^\beta $ (defined for $ x > 1 $), where $ \alpha $ and $ \beta $ are arbitrary real numbers, is a comparison scale. Indeed, here again the quotient of two functions in $ \mathcal{E} $ is a function in $ \mathcal{E} $; it is enough to show that if $ \alpha $ and $ \beta $ are not both zero then $ x^\alpha (\log x)^\beta $ tends to 0 or $ +\infty $; this is clear if $ \alpha = 0, \beta \neq 0 $; if $ \alpha > 0 $ one has $ (\log x)^{-\beta} \ll x^\alpha $, and if $ \alpha < 0 $ one has $ (\log x)^\beta \ll x^{-\alpha} $ for any $ \beta $, whence the proposition.

Note that this last comparison scale is a totally ordered set (for the relation "f $ \ll $ g" or $ f = g $") whose order structure is isomorphic to the *lexicographic* order on $ \mathbf{R}^2 $ (*Set Theory*, III, p. 157); recall that in this structure the relation $ (\alpha, \beta) < (\gamma, \delta) $ means "$ \alpha < \gamma $, or $ \alpha = \gamma $ and $ \beta < \delta $").

Similarly, the scale formed by the functions $ \exp(p(x)) $, where $ p $ runs through the set $ P_0 $ of polynomials with no constant term, has order structure isomorphic to the order structure of $ P_0 $, in which the relation $ p < q $ implies that the dominant term of the polynomial $ q - p $ has a coefficient $ > 0 $ (*cf. Alg.*, VI. 19, *Example 2*).

Let $ \varphi $ be a map from a set F into E, such that $ \varphi^{-1}(\mathfrak{F}) $ is a filter base on F. If $ \mathcal{E} $ is a comparison scale on E (for the filter base $ \mathfrak{F} $) then the functions $ f \circ \varphi $, as $ f $ runs through $ \mathcal{E} $, form a comparison scale on F (for the filter base $ \varphi^{-1}(\mathfrak{F}) $).

### 2. PRINCIPAL PARTS AND ASYMPTOTIC EXPANSIONS

Let $ \mathcal{E} $ be a comparison scale formed by functions with values in a non-discrete valued field K. Let V be a normed space over K, and let $ \mathbf{f} $ be a function in $ \mathcal{H}(\mathfrak{F}, V) $; if there are a function $ g \in \mathcal{E} $ and an element $ \mathbf{a} \neq 0 $ in V such that $ \mathbf{f} \sim \mathbf{a}g $, one says that $ \mathbf{a}g $ is a *principal part* of $ \mathbf{f} $ relative to the scale $ \mathcal{E} $. From def. 1 of V, p. 10, $ \mathbf{f} $ can have *only one* principal part relative to $ \mathcal{E} $, for if $ g_1,\ g_2 $ are two functions in $ \mathcal{E} $ and $ \mathbf{a}_1,\ \mathbf{a}_2 $ are two $ \neq 0 $ elements of V, then the relation $ \mathbf{a}_1 g_1 \sim \mathbf{a}_2 g_2 $ implies $ |g_1| \asymp |g_2| $ and consequently $ g_1 = g_2 $, whence $ (\mathbf{a}_2 - \mathbf{a}_1)g_1 \ll g_1 $, and since $ g_1 $ is not identically zero on any set in $ \mathcal{E} $ this implies $ \mathbf{a}_2 = \mathbf{a}_1 $.

If $ \mathbf{f} $ has a principal part relative to a comparison scale $ \mathcal{E} $ it has *the same* principal part relative to every comparison scale $ \mathcal{E}' \supset \mathcal{E} $.

#### Example 1 {#fvr-v-s2-n2-exa-1 .statement}

For $ x $ real (resp. complex) tending to $ +\infty $ (resp. $ \infty $), every polynomial $ a_0 x^n + a_1 x^{n-1} + \ldots + a_n $ with coefficients in V, such that $ a_0 \neq 0 $, has principal part $ a_0 x^n $ with respect to the scale $ x^n $ (or any scale containing the $ x^n $). It follows that every rational fraction $ \frac{a_0 x^n + \cdots + a_m}{b_0 x^n + \cdots + b_n} $ with real or complex coefficients such that $ a_0 b_0 \neq 0 $ has principal part $ \frac{a_0}{b_0} x^n $ with respect to the same scale.

#### Example 2 {#fvr-v-s2-n2-exa-2 .statement}

A function may be comparable to all the functions of a scale and yet not admit a principal part with respect to this scale. For example, for $ x $ real tending to $ +\infty $, $ \sqrt{x} $ has no principal part with respect to the scale $ x^n $ where $ n $ is a rational integer; $ \log x $ has no principal part with respect to the scale of $ x^\alpha $ ($ \alpha $ arbitrary real); $ \exp(\sqrt{\log x}) $ and $ x' = e^{x \log x} $ have no principal part with respect to the scale of the $ x^\alpha (\log x)^\beta $, nor with respect to the scale of the $ \exp(p(x)) $ ($ p $ a polynomial with no constant term).

The concept of principal part admits extensive generalization. Suppose that a function $ f \in \mathcal{H}(\mathfrak{F}, V) $ has a principal part $ a_1 g_1 $ with respect to a scale $ \mathcal{E} $; the relation $ f \sim a_1 g_1 $ is equivalent to $ f - a_1 g_1 \ll g_1 $ (V, p. 216, def. 4); to study the function $ f $ more closely one is thus led to consider the function $ f - a_1 g_1 $. If this function has a principal part $ a_2 g_2 $ with respect to $ \mathcal{E} $ one must have $ g_2 \ll g_1 $ and $ f - a_1 g_1 - a_2 g_2 \ll g_2 $.

More generally, suppose that the scale $ \mathcal{E} $ is written parametrically in the form $ (g_\alpha) $ where $ \alpha $ runs through a set of indices $ A $ endowed with a totally ordered structure isomorphic to the *opposite* of the order structure of $ \mathcal{E} $: the relation $ \alpha < \beta $ is thus equivalent to $ g_\beta \ll g_\alpha $. In these circumstances:

#### Definition 2 {#fvr-v-s2-def-2 .statement}

*One says that a function* $ f \in \mathcal{H}(\mathfrak{F}, V) $ *admits an asymptotic expansion to precision* $ g_\alpha $ *(relative to the scale* $ \mathcal{E} $*) *if there exists a family* $ (a_\lambda)_{\lambda \leq \alpha} $ *of elements of* $ V $, *all but a finite number of them being* $ 0 $, *such that* $ f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha $. *One says that* $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ *is an asymptotic expansion of* $ f $ *to precision* $ g_\alpha $, *that the* $ a_\lambda g_\lambda $ ($ \lambda \leq \alpha $) *are its terms, the* $ a_\lambda $ *its coefficients, and the function* $ r_\alpha = f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ *the remainder of this expansion*.

To express the fact that $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ is an asymptotic expansion of $ f $ to precision $ g_\alpha $ one most often restricts oneself to writing

$$
f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o(g_\alpha) \quad \text{(or } f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o_k(g_\alpha)
$$

if there are several functions in the proof) following the notation of V, p. 219 and 220.

Of two asymptotic expansions (of two functions, distinct or not) relative to the same scale $ \mathcal{E} $, one says that the one with precision of greater index is the *more precise*.

If $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ is an asymptotic expansion of $ f $ to precision $ g_\alpha $, then, for every $ \beta < \alpha $, $ \sum_{\lambda \leq \beta} a_\lambda g_\lambda $ is an asymptotic expansion of $ f $ to precision $ g_\beta $ (V, p. 215, prop. 5): one says that it is obtained by *reducing the precision* of the given expansion $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ of $ f $ to $ g_\beta $.

If $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ and $ \sum_{\lambda \leq \alpha} b_\lambda g_\lambda $ are asymptotic expansions to the *same* precision $ g_\alpha $ of two functions $ f_1, f_2 $, then $ \sum_{\lambda \leq \alpha} (a_\lambda + b_\lambda) g_\lambda $ is an asymptotic expansion of $ f_1 + f_2 $ to precision $ g_\alpha $ (V, p. 215, prop. 5); and for every scalar $ c $, $ \sum_{\lambda \leq \alpha} a_\lambda c g_\lambda $ is an asymptotic expansion of $ f_1 c $ to precision $ g_\alpha $. It follows that if a function admits an asymptotic expansion to precision $ g_\alpha $ then this expansion is *unique*: it is sufficient to see that the function 0 does not admit an asymptotic expansion with precision $ g_\alpha $ having coefficients $ \neq 0 $. For, if $ 0 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha $, and if $ \gamma $ were the least of the indices $ \lambda \leq \alpha $ such that $ a_\lambda \neq 0 $, one would have $ a_\gamma g_\gamma = - \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda - r_\alpha \ll g_\gamma $, which is absurd.

To say that a function $ f $ admits an asymptotic expansion to precision $ g_\alpha $, all of whose coefficients are *zero*, is equivalent to saying that $ f \ll g_\alpha $. If $ f $ admits an asymptotic expansion $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $ to precision $ g_\alpha $ whose coefficients are not all zero, and if $ \gamma $ is the smallest of the indices $ \lambda $ such that $ a_\lambda \neq 0 $, then $ a_\gamma g_\gamma $ is the *principal part* of $ f $ relative to the scale $ \mathcal{E} $, for one has $ f - a_\gamma g_\gamma = \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha \ll g_\gamma $; similarly, if $ \mu \leq \alpha $ is an index such that $ a_\mu \neq 0 $, then $ a_\mu g_\mu $ is the principal part of $ f - \sum_{\lambda < \mu} a_\lambda g_\lambda $.

The most important asymptotic expansions in applications are those relative to the scale of the $ x^{-n} $ (resp. of the $ z^{-n} $), where $ n $ is a positive or negative integer, as $ x $ tends to $ +\infty $ or to $ -\infty $ (resp. when the complex number $ z $ tends to $ \infty $), or relative to the scale of the $ (x - c)^n $ (resp. $ (z - c)^n $) when the real number $ x $ tends to $ c $ from the right or left (resp. when the complex number $ z $ tends to $ c $). We saw in I, p. 21 that every vector function of a real variable $ x $ which is $ k $ times differentiable at a point $ c \in \mathbf{R} $ admits a Taylor expansion of order $ k $ at this point, that is, an asymptotic expansion to precision $ (x - c)^k $ with respect to the scale of the $ (x - c)^n $.

### 3. SUMS AND PRODUCTS OF ASYMPTOTIC EXPANSIONS

If $ f_1, f_2 $ admit asymptotic expansions to precision $ g_\alpha $ and $ g_\beta $ respectively, relative to a comparison scale $ \mathcal{E} $, one deduces expansions to precision $ g_{\min(\alpha, \beta)} $ by *limiting* the two expansions to this precision; we have seen in V, p. 222 how one obtains an asymptotic expansion for $ f_1 + f_2 $ to precision $ g_{\min(\alpha, \beta)} $.

Let $ V_1, V_2 $ and $ V $ be three normed spaces over the field $ K $, and let $ (\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}. \mathbf{y}] $ be a *continuous bilinear map* from $ V_1 \times V_2 $ into $ V $; we suppose further, for the rest of this section, that the scale $ \mathcal{E} $ is such that the *product* of any two functions in $ \mathcal{E} $ is again in $ \mathcal{E} $ (which is true for all the comparison scales given as examples (in V, p. 220)).

Now let $ f_1, f_2 $ be two functions in $ \mathcal{H}(\mathfrak{F}, V_1) $ and $ \mathcal{H}(\mathfrak{F}, V_2) $ respectively, having asymptotic expansions $ f_1 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha $ and $ f_2 = \sum_{\mu \leq \beta} b_\mu g_\mu + r_\beta $ to precision $ g_\alpha $ and $ g_\beta $ respectively, with respect to the scale $ \mathcal{E} $. Suppose further that neither the $ a_\lambda $ nor the $ b_\mu $ are all zero, and let $ a_\gamma g_\gamma $ and $ b_\delta g_\delta $ be the principal parts of $ f_1 $ and $ f_2 $. By hypothesis, one can write $ g_\gamma g_\beta = g_\rho $ and $ g_\delta g_\alpha = g_\sigma $; let us show that the sum $ \sum [\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu $ taken over all pairs $ (\lambda, \mu) $ such that $ g_{\min(\rho, \sigma)} \ll g_\lambda g_\mu $, is an *asymptotic expansion of* $[f_1.f_2]$ *to precision* $g_{\min(\rho, \sigma)}$. Now the difference between $[f_1.f_2]$ and this sum is the sum of a finite number of terms, each of which is either of the form $[\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$ with $g_\lambda g_\mu \ll g_{\min(\rho, \sigma)}$, or of the form $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda$ where $\lambda \geq \gamma$, or of the form $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu$ where $\mu \geq \delta$; but since $[\mathbf{x}. \mathbf{y}]$ is continuous, one has from (V, p. 213, prop. 3 and V, p. 215, prop. 6) that $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda \preccurlyeq \mathbf{r}_\beta g_\lambda \ll g_\beta g_\gamma = g_\rho$ for $\lambda \geq \gamma$, and similarly $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu \preccurlyeq \mathbf{r}_\alpha g_\mu \ll g_\alpha g_\delta = g_\sigma$ for $\mu \geq \delta$, whence the proposition (V, p. 215, prop. 5).

If all the $\mathbf{a}_\lambda$ are zero one has $[f_1.f_2] \ll g_\alpha g_\delta$: in other words, one has an asymptotic expansion of $[f_1.f_2]$ with zero terms, to precision $g_\alpha g_\delta$; similarly if all the $\mathbf{a}_\lambda$ and $\mathbf{b}_\mu$ are zero one has an asymptotic expansion of $[f_1.f_2]$ with zero terms to precision $g_\alpha g_\beta$.

We shall apply the preceding result principally to the case where V is a *normed algebra* over K and the bilinear function $[\mathbf{x}. \mathbf{y}]$ is the product xy in this algebra; the most important cases are those where V is equal to $\mathbf{R}$ or to $\mathbf{C}$.

In particular, if $f_i$ ($1 \leq i \leq n$) are n functions in $\mathcal{H}(\mathfrak{F}, K)$ each of which admits an asymptotic expansion with respect to $\mathcal{E}$ one can obtain an asymptotic expansion with respect to $\mathcal{E}$ for every *polynomial* $\sum_{(v_i)} \mathbf{a}_{v_1 v_2} v_n f_1^{v_1} \ldots f_n^{v_n}$ in the $f_i$ with coefficients in a normed space V; furthermore, the preceding rules allow one to determine the precision of the expansion obtained, if one knows those of the expansions of the functions $f_i$.

### 4. COMPOSITION OF ASYMPTOTIC EXPANSIONS

Let $f$ be a function in $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ (resp. $\mathcal{H}(\mathfrak{F}, \mathbf{C})$), admitting an asymptotic expansion to precision $g_\alpha$ with respect to a scale $\mathcal{E}$, and *having limit* 0 along the filter with base $\widetilde{\mathfrak{F}}$. On the other hand let $\mathbf{h}$ be a function with values in a normed space V over $\mathbf{R}$ (resp. $\mathbf{C}$), defined on a neighbourhood of the point 0 in $\mathbf{R}$ (resp. $\mathbf{C}$), and *n times differentiable* on this neighbourhood; then

$$
\mathbf{h}(t) = c_0 + c_1 t + \cdots + c_n t^n + o(t^n)
$$

on this neighbourhood (I, p. 21), whence, on a suitable set in $\widetilde{\mathfrak{F}}$

$$
\mathbf{h} \circ f = c_0 + c_1 f + \cdots + c_n f^n + o(f^n).
$$

We have seen, in n 3, how to form an asymptotic expansion for $c_0 + c_1 f + \cdots + c_n f^n$ to a precision $g_\rho$ determined by the precision of the expansion of $f$; moreover, suppose that the coefficients of the asymptotic expansion of $f$ are not all zero, and that $a_\gamma g_\gamma$ is the principal part of $f$, and let $g_\sigma = g_\gamma^n$; if $\sigma < \rho$ one will have an expansion of $\mathbf{h} \circ f$ to precision $g_\sigma$ on limiting the expansion of $\sum_{k=0}^n c_k f^k$ to this precision; if, on the contrary, $\rho \leq \sigma$, then the expansion of $\sum_{k=0}^n c_k f^k$ is also an expansion of $\mathbf{h} \circ f$ to precision $g_\rho$.

If all the terms of the asymptotic expansion of $ f $ are zero, and if $ g_\alpha \ll 1 $, then $ f \ll g_\alpha $ and so $ f^k \ll g_\alpha^k \ll g_\alpha $ for every integer $ k > 0 $; if $ c_m $ is the first coefficient of index $ > 0 $ which is not zero (assuming that the $ c_k $ for indices $ k > 0 $ are not all 0), then $ c_0 $ is an asymptotic expansion of $ h \circ f $ to precision $ g_\alpha^m $.

In the remainder of this section we shall restrict ourselves to the case where the functions in $ \mathcal{E} $ have real values and are strictly positive on a set in $ \mathfrak{F} $, and we shall consider asymptotic expansions only of functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $. Suppose first that for every function $ g \in \mathcal{E} $ and every real number $ \nu $, $ g^\nu $ again belongs to $ \mathcal{E} $: this condition is fulfilled, for example, by the scale of the $ x^\alpha $ or by that of the $ x^\alpha |\log x|^\beta $ ($ \alpha $ and $ \beta $ being arbitrary real numbers) on a neighbourhood of $ +\infty $ or a neighbourhood of 0 in $ \mathbf{R} $. This property implies that the quotient of two functions in $ \mathcal{E} $ again belongs to $ \mathcal{E} $. This being so, from an asymptotic expansion relative to $ \mathcal{E} $ of a function $ f \in \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, to precision $ g_\alpha $, one can derive an expansion for $ |f|^\nu $ for every real number $ \nu $. Let us restrict ourselves to the case where the coefficients of the expansion of $ f $ are not all zero, and let $ a_\gamma g_\gamma $ be the principal part of $ f $; one can write $ |f|^\nu = |a_\gamma|^\nu g_\gamma^\nu (1 + h)^\nu $, with
$$
h = \sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} + o \left( \frac{g_\alpha}{g_\gamma} \right).
$$
Under our hypotheses $ \sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} $ is an asymptotic expansion of $ h $, to precision $ g_\alpha / g_\gamma $; since $ h $ tends to 0 along $ \mathfrak{F} $ the method described above gives an asymptotic expansion of $ (1 + h)^\nu $, then an expansion of $ |f|^\nu $ on multiplying by $ |a_\gamma|^\nu g_\gamma^\nu $.

With the same hypotheses on $ f $ one can write
$$
\log |f| = \log |a_\gamma g_\gamma| + \log (1 + h)
$$
and $ \log (1 + h) $ can be expanded, as has been said above, the function $ \log (1 + t) $ being indefinitely differentiable on a neighbourhood of 0; if, further, $ \log g_\gamma $ admits an asymptotic expansion with respect to $ \mathcal{E} $, or with respect to a scale $ \mathcal{E}_1 \supset \mathcal{E} $, one obtains an asymptotic expansion for $ \log |f| $ on adding the two asymptotic expansions.

#### Example {#fvr-v-s2-n4-exa-1 .statement}

We have $ (1 + x)^{1/x} = \exp \left( \frac{1}{x} \log (1 + x) \right) $: when $ x $ tends to $ +\infty $ we have $ \log (1 + x) = \log x + \log \left( 1 + \frac{1}{x} \right) $, whence the asymptotic expansion of $ \frac{1}{x} \log (1 + x) $ with respect to the scale of the $ x^\alpha (\log x)^\beta $:
$$
\frac{1}{x} \log (1 + x) = \frac{\log x}{x} + \frac{1}{x^2} - \frac{1}{2x^3} + o_1 \left( \frac{1}{x^3} \right).
$$
From this expansion, and from the Taylor expansion
$$
e^u = 1 + u + \frac{u^2}{2} + \frac{u^3}{6} + o(u^3)
$$

on a neighbourhood of $ u = 0 $, one deduces the asymptotic expansion

$$
(1 + x)^{1/x} = 1 + \frac{\log x}{x} + \frac{1}{2} \frac{(\log x)^2}{x^2} + \frac{1}{x^2}
+ \frac{1}{6} \frac{(\log x)^3}{x^3} + \frac{\log x}{x^3} - \frac{1}{2x^3} + o_2 \left( \frac{1}{x^3} \right)
$$

with respect to the scale $ x^\alpha (\log x)^\beta $ by the methods explained above.

Keeping the same hypotheses and notation, the asymptotic expansion of $ e^f $ does not pose new problems except when $ f \gg 1 $; one must then distinguish two cases, as $ g_\alpha \gg 1 $ or $ g_\alpha \ll 1 $. In the first case, giving an expansion for $ f $ does not allow one to obtain a principal part for $ e^f $ relative to $ \mathcal{E} $, because one does not know in general whether the remainder $ r_\alpha $ tends to 0, that is, whether $ e^{r_\alpha} $ tends to 1. On the contrary, if $ g_\alpha \ll 1 $ then $ r_\sigma \ll 1 $ and so $ e^f \sim \exp \left( \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \right) $. One can make this result more precise: let $ a_\gamma g_\gamma $ be the principal part of $ f $ and let $ \delta $ be the index (such that $ \gamma < \delta \leq \alpha $) for which $ g_\delta = 1 $; we put $ f_1 = \sum_{\lambda \leq \delta} a_\lambda g_\lambda $, $ f_2 = \sum_{\delta < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha $; we have $ f = f_1 + f_2 $, so $ e^f = e^{f_1} e^{f_2} $, and the general method explained at the start of this subsection allows one to form an asymptotic expansion of $ e^{f_2} $ (starting from the Taylor expansion of $ e^t $ at the point $ t = 0 $). One will then have an asymptotic expansion for $ e^f $ if $ e^{f_1} = \prod_{\lambda \leq \delta} \exp(a_\lambda g_\lambda) $ belongs to $ \mathcal{E} $, or to a scale $ \mathcal{E}_1 $ containing $ \mathcal{E} $.

#### Example {#fvr-v-s2-n4-exa-2 .statement}

We have $ x^{1/1} = \exp \left( \log x \cdot \exp \left( \frac{1}{x} \log x \right) \right) $; when $ x $ tends to $ +\infty $ one has $ \log x \ll x $, whence the asymptotic expansion of $ \log x \cdot \exp \left( \frac{1}{x} \log x \right) $ with respect to the scale $ x^\alpha (\log x)^\beta $:

$$
\log x \cdot \exp \left( \frac{1}{x} \log x \right) = \log x + \frac{(\log x)^2}{x} + \frac{1}{2} \frac{(\log x)^3}{x^2} + o \left( \frac{(\log x)^3}{x^2} \right).
$$

All the terms of this expansion, starting from the second, tend to 0; from this expansion and from the Taylor expansion $ e^u = 1 + u + u^2/2 + o(u^2) $ on a neighbourhood of $ u = 0 $ one deduces

$$
x^{1/1} = 1 + (\log x)^2 + \frac{1}{2} \frac{(\log x)^4}{x} + \frac{1}{2} \frac{(\log x)^3}{x} + o \left( \frac{(\log x)^3}{x} \right).
$$

### 5. ASYMPTOTIC EXPANSIONS WITH VARIABLE COEFFICIENTS

One can generalize the concept of principal part, and that of an asymptotic expansion, in the following way. Let $ \mathcal{E} $ be a comparison scale formed of real (resp. complex) functions such that, for each of them, there is a set in $ \mathfrak{F} $ on which the function *does not vanish at any point*. Further, let $ C $ be a set of functions in $ \mathcal{H}(\mathfrak{F}, V) $ satisfying the following three conditions:

(CO₁) For every function $ a \in C $ one has $ a \preccurlyeq 1 $.
(CO₂) The relation $ a \ll 1 $ for a function $ a \in C $ implies $ a = 0 $.
(CO₃) $ C $ is a vector space over $ \mathbf{R} $ (resp. $ \mathbf{C} $).

Now let $ f $ be any function in $ \mathcal{H}(\mathfrak{F}, V) $; if there exist a function $ g \in \mathcal{E} $ and a nonzero function $ a \in C $ such that $ f - ag \ll g $ one will say that $ ag $ is a principal part of $ f $, relative to the comparison scale $ \mathcal{E} $ and to the domain of coefficients $ C $. If such a principal part exists, it is unique: for suppose that there are two principal parts $ a_1 g_1 $ and $ a_2 g_2 $; one cannot have $ g_1 \ll g_2 $ since from (CO₁) one could deduce that $ a_1 g_1 \ll g_2 $ and $ f - a_1 g_1 \ll g_1 \ll g_2 $, so $ f \ll g_2 $; but one would also have $ a_2 g_2 \ll g_2 $ and consequently $ a_2 \ll 1 $ contradicting the hypothesis $ a_2 \neq 0 $ and (CO₂). So one must have $ g_1 = g_2 $; from the relations $ f - a_1 g_1 \ll g_1, f - a_2 g_1 \ll g_1 $ one deduces that $ (a_2 - a_1)g_1 \ll g_1 $ whence $ a_2 - a_1 \ll 1 $, and consequently $ a_2 = a_1 $, by (CO₂) and (CO₃).

#### Example {#fvr-v-s2-n5-exa-1 .statement}

For $ x $ real tending to $ +\infty $ the periodic bounded functions on $ \mathbf{R} $, having the same period $ \tau $, satisfy conditions (CO₁), (CO₂) and (CO₃): if $ \lim_{x \to +\infty} a(x) = 0 $ then for every $ \varepsilon > 0 $ there is an $ x_0 $ such that $ |a(x)| \leq \varepsilon $ for every $ x \geq x_0 $; one deduces that $ |a(x)| \leq \varepsilon $ for $ 0 \leq x \leq \tau $ too, since there exists an integer $ n $ such that $ x + n\tau \geq x_0 $, and such that $ a(x) = a(x + n\tau) $; since $ \varepsilon $ is arbitrary one has $ a(x) = 0 $ on $ [0, \tau] $, hence everywhere.

With the notation of V, p. 222, we will say that $ \sum_{\lambda \leq \alpha} a_\lambda g_\lambda $, where the $ a_\lambda $ belong to $ C $ and all but a finite number of them are zero, is an asymptotic expansion of $ f $ with coefficients in $ C $, to precision $ g_\alpha $, if $ f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha $; for every index $ \mu $ such that $ a_\mu \neq 0 $ then $ a_\mu g_\mu $ is the principal part of $ f - \sum_{\lambda < \mu} a_\lambda g_\lambda $, relative to $ \mathcal{E} $ and to $ C' $, which proves the uniqueness of the asymptotic expansion of $ f $ (to precision $ g_\alpha $) when it exists.

The methods given in n 3 (V, p. 223) for forming an asymptotic expansion for $ f_1 + f_2 $ or for $ [f_1 . f_2] $, starting from given asymptotic expansions for $ f_1 $ and $ f_2 $, can again be applied to expansions with variable coefficients, so long as the $ [a_\lambda . b_\mu] $ belong to the domain of coefficients $ C $ corresponding to the normed space $ V $ or admit an asymptotic expansion with coefficients in $ C $.
