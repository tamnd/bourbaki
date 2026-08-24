---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 4
section_title: Integrable functions and sets
lang: en
source: int-i-vi
book_pages: INT IV.32-INT IV.59, INT IV.120-INT IV.127
pdf_pages: 0139-0166, 0227-0234
extraction: ocr
subsections:
    - "no": 1
      title: Extension of the integral
      page: 32
      pdf_page: 139
    - "no": 2
      title: Properties of the integral
      page: 34
      pdf_page: 141
    - "no": 3
      title: Passage to the limit in integrals
      page: 36
      pdf_page: 143
    - "no": 4
      title: Characterizations of integrable numerical functions
      page: 37
      pdf_page: 144
    - "no": 5
      title: Integrable sets
      page: 41
      pdf_page: 148
    - "no": 6
      title: Criteria for the integrability of a set
      page: 43
      pdf_page: 150
    - "no": 7
      title: Characterization of bounded measures
      page: 46
      pdf_page: 153
    - "no": 8
      title: Integration with respect to a measure with compact support
      page: 47
      pdf_page: 154
    - "no": 9
      title: Clans and additive set functions
      page: 50
      pdf_page: 157
    - "no": 10
      title: Approximation of continuous functions by step functions
      page: 52
      pdf_page: 159
    - "no": 11
      title: Extension of a measure defined on a family of sets
      page: 53
      pdf_page: 160
statements: 63
exercises: 23
content_sha256: d9bf2bfdcda5ca6a66db17faa978e5ab9ec595ffc7644a6643a0e2ffb0353a31
---

## § 4. INTEGRABLE FUNCTIONS AND SETS

### 1. Extension of the integral

It follows from the definition of the space $ \mathcal{L}_F^p $ that the subspace $ \mathcal{K}_F $ of continuous functions with compact support is *dense* in $ \mathcal{L}_F^p $ (\S 3, No. 4, Def. 2). Every continuous (for the topology of convergence in mean of order $ p $) linear function, defined on $ \mathcal{K}_F $ and taking its values in a *complete Hausdorff* topological vector space $ G $, can therefore be *extended by continuity* in a unique manner, to a continuous linear function defined on $ \mathcal{L}_F^p $ with values in $ G $ (GT, II, \S 3, No. 6, Th. 2 and III, \S 3, No. 1, Prop. 3).

Now, for every continuous function $ f $ with compact support, with values in the Banach space $ F $, we have defined (in Ch. III, \S 3, No. 1) the *integral* $ \mu(f) = \int f \, d\mu $ with respect to $ \mu $, which is an element of $ F $, and we have proved (Ch. III, \S 3, No. 2, Prop. 6) the inequality

$$
\left| \int f \, d\mu \right| \leqslant \int |f| \, d|\mu| = N_1(f).
$$

This inequality proves that the linear mapping $ f \mapsto \int f \, d\mu $ of $ \mathcal{K}_F $ into $ F $ is continuous for the topology of convergence in mean in $ \mathcal{K}_F $. It can therefore be extended by continuity to the entire space $ \mathcal{L}_F^1 $, and we may make the following definition:

#### Definition 1 {#int-iv-s4-def-1 .statement}

*The functions belonging to $ \mathcal{L}_F^1(X, \mu) $ are said to be integrable with respect to the measure $ \mu $* (or, again, that they are $ \mu $-integrable). *The integral (with respect to $ \mu $) of the integrable function $ f $ is by definition the value at $ f $ of the extension by continuity to $ \mathcal{L}_F^1 $ of the linear mapping $ g \mapsto \int g\, d\mu $ of $ \mathcal{H}_F $ into $ F $; it is again denoted $ \mu(f) $ or $ \int f\, d\mu $, or $ \int f(x)\, d\mu(x) $ or $ \int f\mu $, or $ \int f(x)\mu(x) $.

#### Example {#int-iv-s4-n1-exa-1 .statement}

— Let $ X $ be a *discrete* space, $ \mu $ a measure on $ X $, and set $ \alpha(x) = \mu(\varphi_{\{x\}}) $ for every $ x \in X $. The functions in $ \mathcal{F}_F^1 $ are then *integrable*, in other words $ \mathcal{L}_F^1 = \mathcal{F}_F^1 $; moreover, for every function $ f \in \mathcal{L}_F^1 $,

$$
\int f\, d\mu = \sum_{x \in X} \alpha(x)f(x).
$$

For, let $ f \in \mathcal{F}_F^1 $; we have $ |\mu|^*(|f|) = \sum_{x \in X} |\alpha(x)| \cdot |f(x)| < +\infty $ (\S 1, No. 3, *Example*); for every $ \varepsilon > 0 $, there exists a finite subset $ M $ of $ X $ such that

$$
\sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon.
$$

The function $ g $ equal to $ f $ at the points $ x \in M $ where $ |f| $ is finite, and to 0 elsewhere, belongs to $ \mathcal{H}(X; F) $ and, by the conventions that have been made,

$$
|\mu|^*(|f - g|) \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

which proves that $ f \in \mathcal{L}_F^1 $. On the other hand,

$$
\left| \mu(g) - \sum_{x \in X} \alpha(x)f(x) \right| \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

whence the second assertion.

In other words, the $ \mu $-integrable functions $ f $ are those for which the family $ (\alpha(x)f(x))_{x \in X} $ is *absolutely summable* (GT, IX, §3, No. 6), and the integral $ \int f\, d\mu $ is the sum of this family.

Since $ \mu(f) $ is continuous on $ \mathcal{L}_F^1 $ by definition, and since it takes its values in a Hausdorff space, we have $ \mu(f) = 0 $ for every function that belongs to the closure of 0 in $ \mathcal{L}_F^1 $, that is, is *negligible*; if $ f $ and $ g $ are two *equivalent* integrable functions, then $ \mu(f) = \mu(g) $. In other words, the value of $ \mu(f) $ depends only on the class $ \tilde{f} $ of the integrable function $ f $; it is again denoted $ \mu(\tilde{f}) $, and the function $ \tilde{f} \mapsto \mu(\tilde{f}) $ is a continuous linear mapping of $ L^1_F $ into $ F $. If a function $ f $, with values in $ F $ and defined almost everywhere in $ X $, is equivalent to an integrable function, we again say that $ f $ is *integrable* and we write $ \int f\, d\mu = \mu(\tilde{f}) $; one defines similarly an integrable function with values in $ \overline{\mathbf{R}} $, defined and finite almost everywhere, as well as its integral.

### 2. Properties of the integral

#### Proposition 1 {#int-iv-s4-prop-1 .statement}

*For every positive $ \mu $-integrable numerical function $ f $,*

$$
\int f\, d|\mu| = \int^* f\, d|\mu| = N_1(f) \geqslant 0.
$$

For, $ \int f\, d|\mu| $ and $ N_1(f) $ are continuous on $ \mathcal{L}^1 $ and are equal for every continuous function $ f \geqslant 0 $ with compact support; on the other hand, every function $ f \geqslant 0 $ in $ \mathcal{L}^1 $ is the limit (in the sense of convergence in mean) of a sequence of continuous functions $ \geqslant 0 $ with compact support (\S 3, No. 5, Prop. 11); whence the proposition.

#### Corollary 1 {#int-iv-s4-prop-1-cor-1 .statement}

*For every integrable function $ f \in \mathcal{L}^1_F $, $ |f| $ is integrable and*

$$
\int |f|\, d|\mu| = \int^* |f|\, d|\mu| = N_1(f).
$$

We shall make frequent use of Prop. 1 and its Cor. 1, on replacing $ \int^* f\, d|\mu| $ or $ N_1(f) $ by $ \int f\, d|\mu| $ when dealing with an integrable function $ \geqslant 0 $. For example, for two integrable functions $ f, g $ to be *equivalent*, it is necessary and sufficient that $ \int |f - g|\, d|\mu| = 0 $.

We recall that, for a function $ f $ to belong to $ \mathcal{L}^p_F $, it is necessary and sufficient that the function $ |f|^{p-1} \cdot f $ belong to $ \mathcal{L}^1_F $ (\S 3, No. 8, Cor. 1 of Th. 7), that is, that it be integrable; this is the reason for the terminology 'p-th power integrable function'. Moreover:

#### Corollary 2 {#int-iv-s4-prop-1-cor-2 .statement}

*For every function $ f \in \mathcal{L}^p_F $, the numerical function $ |f|^p $ is integrable and*

$$
N_p(f) = \left( \int |f|^p\, d|\mu| \right)^{1/p}.
$$

This follows at once from the fact that $ |f| $ belongs to $ \mathcal{L}^p $ (\S 3, No. 5, Prop. 11) and formula (2).

#### Proposition 2 {#int-iv-s4-prop-2 .statement}

— For every integrable function $ f $,

$$
\left| \int f \, d\mu \right| \leq \int |f| \, d|\mu|.
$$

This follows at once from the inequality (1) by passage to the limit, on taking into account (3) and the continuity of $ N_1(f) $ on $ \mathcal{L}_F^1 $.

#### Theorem 1 {#int-iv-s4-thm-1 .statement}

— Let $ F $ and $ G $ be two Banach spaces, $ u $ a continuous linear mapping of $ F $ into $ G $. For every integrable function $ f $ with values in $ F $, $ u \circ f $ is integrable and

$$
\int u(f(x)) \, d\mu(x) = u \left( \int f(x) \, d\mu(x) \right).
$$

We already know that $ u \circ f $ is integrable (\S 3, No. 5, Th. 4); the relation (6), being valid for every $ f \in \mathcal{H}_F $, extends to every integrable function $ f $ by the principle of extension of identities: for, $ f \mapsto u \circ f $ is continuous for the topology of convergence in mean, as follows from the inequality $ N_1(u \circ f) \leq \|u\| \cdot N_1(f) $.

#### Corollary 1 {#int-iv-s4-thm-1-cor-1 .statement}

— Let $ a' $ be a continuous linear form on $ F $. If $ f $ is an integrable function with values in $ F $, then the numerical function $ \langle f, a' \rangle $ is integrable and

$$
\int \langle f(x), a' \rangle \, d\mu(x) = \left\langle \int f(x) \, d\mu(x), a' \right\rangle.
$$

We shall see in Ch. VI, \S 1, Exers. 7, 11 and 12 that there can exist functions $ f $, with values in an infinite-dimensional Banach space $ F $, such that $ \langle f, a' \rangle $ is integrable for every continuous linear form $ a' $ on $ F $, without $ f $ being integrable.

#### Corollary 2 {#int-iv-s4-thm-1-cor-2 .statement}

— If the $ a_k $ ($ 1 \leq k \leq n $) are vectors in $ F $ and the $ f_k $ ($ 1 \leq k \leq n $) are integrable numerical functions, then the function $ f = \sum_{k=1}^n a_k f_k $ is integrable and

$$
\int \left( \sum_{k=1}^n a_k f_k \right) d\mu = \sum_{k=1}^n a_k \int f_k \, d\mu.
$$

### 3. Passage to the limit in integrals

#### Proposition 3 {#int-iv-s4-prop-3 .statement}

— Let $ \mathcal{B} $ be a filter base on $ \mathcal{L}_F^1 $. Assume that there exists a compact set $ K \subset X $ such that, for every set $ M \in \mathcal{B} $, all of the functions $ f \in M $ have their support in $ K $. Under these conditions, if $ \mathcal{B} $ converges uniformly on $ X $ to $ f_0 $, then the function $ f_0 $ is integrable and

$$
\int f_0 \, d\mu = \lim_{\mathcal{B}} \int f \, d\mu .
$$

For, $ \mathcal{B} $ converges in mean to $ f_0 $ (\S 3, No. 3, Prop. 4).

#### Proposition 4 {#int-iv-s4-prop-4 .statement}

— Let $ (f_n) $ be an increasing (resp. decreasing) sequence of integrable numerical functions. For the upper (resp. lower) envelope $ f $ of the sequence to be integrable, it is necessary and sufficient that $ \sup_n \int f_n \, d|\mu| < +\infty $ (resp. $ \inf_n \int f_n \, d|\mu| > -\infty $), in which case

$$
\int f \, d\mu = \lim_{n \to \infty} \int f_n \, d\mu .
$$

We limit ourselves to considering an increasing sequence. The sequence $ g_n = f_n + f_1^- $ is increasing and consists of integrable functions $ \geqslant 0 $; since its upper envelope is $ g = f + f_1^- $, the proposition follows from Th. 5 of \S 3, No. 6.

#### Theorem 2 {#int-iv-s4-thm-2 .statement}

— Let $ A $ be a set of indices, filtered by a filter $ \mathfrak{F} $ with a countable base. Let $ (f_\alpha)_{\alpha \in A} $ be a family of integrable functions that, with respect to the filter $ \mathfrak{F} $, converge pointwise almost everywhere to a function $ f $; if there exists a numerical function $ g \geqslant 0 $ such that $ \int^* g \, d|\mu| < +\infty $ and such that $ |f_\alpha(x)| \leqslant g(x) $ almost everywhere in $ X $ for each $ \alpha \in A $, then the function $ f $ is integrable and

$$
\int f \, d\mu = \lim_{\mathfrak{F}} \int f_\alpha \, d\mu .
$$

The theorem follows from Lebesgue’s theorem (\S 3, No. 7, Cor. of Th. 6) since, under the conditions of the statement, $ f_\alpha $ converges in mean to $ f $ with respect to $ \mathfrak{F} $.

#### Corollary 1 {#int-iv-s4-thm-2-cor-1 .statement}

— Let $ \Omega $ be a topological space, $ t_0 $ a point of $ \Omega $ admitting a countable fundamental system of neighborhoods, $ f $ a mapping of $ X \times \Omega $ into $ F $ having the following properties:
a) for every $ t \in \Omega $, the function $ x \mapsto f(x, t) $ is integrable;
b) for every $ x \in X $, the function $ t \mapsto f(x, t) $ is continuous at $ t_0 $;

c) there exist a neighborhood U of t_0 and a numerical function g \geqslant 0 defined on X, such that $ \int^* g d|\mu| < +\infty $ and $ |\mathbf{f}(x,t)| \leqslant g(x) $ for all $ x \in X $ and $ t \in U $.

Under these conditions, the mapping $ t \mapsto \int \mathbf{f}(x,t) d\mu(x) $ of $ \Omega $ into F is continuous at the point $ t_0 $.

#### Corollary 2 {#int-iv-s4-thm-2-cor-2 .statement}

— Let $ (\mathbf{f}_n) $ be a sequence of integrable functions such that the series with general term $ \mathbf{f}_n(x) $ converges almost everywhere; if there exists a function $ g \geqslant 0 $ such that $ \int^* g d|\mu| < +\infty $ and such that, for every integer $ n $, $ \left| \sum_{k=1}^n \mathbf{f}_k(x) \right| \leqslant g(x) $ almost everywhere, then the sum $ \mathbf{f}(x) $ (defined almost everywhere) of the series with general term $ \mathbf{f}_n(x) $ is integrable and

$$
\int \mathbf{f} d\mu = \sum_{n=1}^\infty \int \mathbf{f}_n d\mu
$$

('term-by-term integration of a series').

### 4. Characterizations of integrable numerical functions

#### Proposition 5 {#int-iv-s4-prop-5 .statement}

— For a numerical function $ f \geqslant 0 $ (finite or not), lower semi-continuous on X, to be integrable, it is necessary and sufficient that $ \int^* f d|\mu| < +\infty $.

It all comes down to proving that the condition is sufficient. The definition of $ |\mu|^*(f) $ (\S 1, No. 1, Def. 1) proves that, for every $ \varepsilon > 0 $, there exists a continuous function $ g \geqslant 0 $, with compact support, such that $ g \leqslant f $ and $ |\mu|^*(f) \leqslant |\mu|(g) + \varepsilon $. But $ f - g $ is lower semi-continuous and $ \geqslant 0 $, therefore (\S 1, No. 1, Th. 2)

$$
|\mu|^*(f) = |\mu|(g) + |\mu|^*(f - g),
$$

in other words $ N_1(f - g) = |\mu|^*(f - g) = |\mu|^*(f) - |\mu|(g) \leqslant \varepsilon $, which proves that $ f $ is integrable (\S 3, No. 4, Prop. 7).

#### Corollary 1 {#int-iv-s4-prop-5-cor-1 .statement}

— For a finite numerical function $ f \geqslant 0 $, upper semi-continuous on X, to be integrable, it is necessary and sufficient that $ \int^* f d|\mu| < +\infty $.

For, if $ |\mu|^*(f) < +\infty $, then there exists a lower semi-continuous function $ h $ such that $ f \leqslant h $ and $ |\mu|^*(h) < +\infty $; $ h - f $ is everywhere defined and lower semi-continuous, and $ |\mu|^*(h - f) \leqslant |\mu|^*(h) < +\infty $; therefore $ h - f $ is integrable, and since $ f(x) = h(x) - (h(x) - f(x)) $ almost everywhere, $ f $ is integrable.

#### Corollary 2 {#int-iv-s4-prop-5-cor-2 .statement}

— Let $ \mathbf{H} $ be a nonempty set, directed for the relation $ \leqslant $ (resp. $ \geqslant $), of lower (resp. upper) semi-continuous and integrable numerical functions; if

$$
\sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty \quad \text{(resp. } \inf_{f \in \mathbf{H}} \int f \, d|\mu| > -\infty \text{)},
$$

then the upper (resp. lower) envelope $ g $ of $ \mathbf{H} $ is integrable,

$$
\int g \, d\mu = \lim_{f \in \mathbf{H}} \int f \, d\mu,
$$

and $ \int g \, d|\mu| = \sup_{f \in \mathbf{H}} \int f \, d|\mu| $ (resp. $ \int g \, d|\mu| = \inf_{f \in \mathbf{H}} \int f \, d|\mu| $).

We may limit ourselves to the case of lower semi-continuous functions; the functions $ f^+ $ (resp. $ f^- $), as $ f $ runs over $ \mathbf{H} $, then form a directed set for $ \leqslant $ (resp. $ \geqslant $) of lower (resp. upper) semi-continuous functions $ \geqslant 0 $; the upper (resp. lower) envelope of the $ f^+ $ (resp. $ f^- $), for $ f \in \mathbf{H} $, is equal to $ g^+ $ (resp. $ g^- $). On the other hand, one can replace $ \mathbf{H} $ by one of its sections (which is cofinal to it), consisting of the $ f \in \mathbf{H} $ that are $ \geqslant f_0 $, for some function $ f_0 \in \mathbf{H} $; then $ \int f^+ \, d|\mu| \leqslant \int f \, d|\mu| + \int f_0^- \, d|\mu| $; we thus see that we are reduced to proving the two assertions of the corollary when $ \mathbf{H} $ consists of positive functions. If $ \mathbf{H} $ is directed for $ \leqslant $ and consists of lower semi-continuous functions $ \geqslant 0 $, then we know (\S 1, No. 1, Th. 1) that

$$
|\mu|^*(g) = \sup_{f \in \mathbf{H}} |\mu|^*(f) = \sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty,
$$

therefore $ g $, which is lower semi-continuous, is integrable by Prop. 5; we have $ \int g \, d|\mu| = \lim_{f \in \mathbf{H}} \int f \, d|\mu| $ and, since $ f \leqslant g $, $ \lim_{f \in \mathbf{H}} N_1(g - f) = 0 $, which shows that $ f $ converges in mean to $ g $ with respect to $ \mathbf{H} $, and thus proves the corollary in this case. If $ \mathbf{H} $ is directed for $ \geqslant $ and consists of upper semi-continuous integrable functions $ f $ such that $ 0 \leqslant f \leqslant f_1 $ with $ f_1 \in \mathbf{H} $, then there exists a lower semi-continuous integrable function $ h $ such that $ f_1 \leqslant h $; we may write $ f = h - f' $, where $ f'(x) = h(x) - f(x) $ when $ f(x) < +\infty $, and $ f'(x) = 0 $ otherwise. It is clear that the $ f' $ form a directed set, for $ \leqslant $, of lower semi-continuous integrable functions $ \geqslant 0 $, with

$$
\int f' \, d|\mu| \leqslant \int h \, d|\mu| < +\infty;
$$

we can apply to them what has been proved above; if $ g' $ is the upper envelope of the $ f' $, then $ h $ and $ g' $ are finite almost everywhere, therefore $ h - g' $ is defined almost everywhere and is equal to $ g $ almost everywhere; from this, the conclusions of the corollary follow at once in this case.

#### Corollary 3 {#int-iv-s4-prop-5-cor-3 .statement}

— Let $ f $ be a bounded numerical function, upper semi-continuous on $ X $ and with compact support. Then, the mapping $ \mu \mapsto \int f\, d\mu $ is upper semi-continuous on $ \mathcal{M}_+(X) $ for the vague topology.

If $ h $ is a function in $ \mathcal{K}_+(X) $ such that $ |f| \leq h $ (Ch. III, §1, No. 2, Lemma 1) then $ 0 \leq f + h \leq 2h $, and since $ f + h $ is upper semi-continuous, it follows from Cor. 1 that $ f $ is $ \mu $-integrable for every measure $ \mu $ on $ X $. Moreover, $ \mu(f) = \mu(h) - \mu(h - f) $ and $ h - f $ is a lower semi-continuous function $ \geq 0 $. Since the mapping $ \mu \mapsto \mu(h - f) $ is lower semi-continuous on $ \mathcal{M}_+(X) $ for the vague topology (§1, No. 1, Prop. 4), this proves the corollary.

#### Theorem 3 {#int-iv-s4-thm-3 .statement}

— For a numerical function $ f \geq 0 $ to be integrable, it is necessary and sufficient that, for every $ \varepsilon > 0 $, there exist an upper semi-continuous function $ g \geq 0 $, with finite values and compact support, and a lower semi-continuous integrable function $ h $, such that $ g \leq f \leq h $ and $ \int (h - g)\, d|\mu| \leq \varepsilon $.

The condition is sufficient by a general criterion for integrability (§3, No. 4, Prop. 8), Prop. 5 and its Corollary 1. Let us show that the condition is necessary. If $ f \geq 0 $ is integrable then, for every $ \varepsilon > 0 $, there exists a function $ u \geq 0 $, continuous and with compact support, such that $ N_1(f - u) \leq \varepsilon/4 $. By the definition of $ N_1 $, this implies that there exists a lower semi-continuous function $ v \geq 0 $ such that $ |\mu|^*(v) \leq \varepsilon/2 $ and $ |f - u| \leq v $. Thus, $ -v(x) \leq f(x) - u(x) \leq v(x) $ for all $ x \in X $, and since $ u(x) $ is everywhere finite, it follows that $ (u(x) - v(x))^+ \leq f(x) \leq u(x) + v(x) $ for all $ x \in X $. The functions $ g = (u - v)^+ $ and $ h = u + v $ meet the requirements.

#### Corollary {#int-iv-s4-n4-cor-1 .statement}

— For every integrable (resp. integrable and $ \geq 0 $) numerical function $ f $, there exist an increasing sequence $ (g_n) $ of upper semi-continuous functions that are integrable (resp. integrable, with finite values $ \geq 0 $, and with compact support), and a decreasing sequence $ (h_n) $ of lower semi-continuous integrable functions, such that:
$ 1^\circ $ $ g_n(x) \leq f(x) \leq h_n(x) $ for all $ x \in X $ and every integer $ n $;
$ 2^\circ $ $ f(x) $ is equal almost everywhere to the lower envelope $ h $ of the sequence $ (h_n) $ and to the upper envelope $ g $ of the sequence $ (g_n) $;
$ 3^\circ $ $ \int f\, d\mu = \lim_{n \to \infty} \int g_n\, d\mu = \lim_{n \to \infty} \int h_n\, d\mu $.

Suppose first that $ f \geq 0 $. By Th. 3 there exist, for every $ n $, a lower semi-continuous integrable function $ v_n $, and an upper semi-continuous function $ u_n \geq 0 $ with finite values and compact support, such that

$$
u_n \leq f \leq v_n \quad \text{and} \quad \int (v_n - u_n)\, d|\mu| \leq 1/n;
$$

setting $ g_n = \sup(u_1, u_2, \ldots, u_n) $ and $ h_n = \inf(v_1, v_2, \ldots, v_n) $, the sequences $(g_n)$ and $(h_n)$ meet the requirements. For, since $ g \leq f $, $ g $ is integrable by Prop. 4 of No. 3, and since
$$
\int (f - g_n) d|\mu| \leq \int (v_n - u_n) d|\mu| \leq 1/n
$$
we have
$$
\int (f - g) d|\mu| = \lim_{n \to \infty} \int (f - g_n) d|\mu| = 0
$$
(No. 3, Prop. 4), which proves that $ f $ and $ g $ are equivalent. One argues similarly for the sequence $(h_n)$.

If $ f $ is not positive, we can apply the foregoing to $ f^+ $ and $ f^- $, thus there are two increasing sequences $(g'_n), (g''_n)$ of upper semi-continuous integrable functions, and two decreasing sequences $(h'_n), (h''_n)$ of lower semi-continuous integrable functions, such that: $ 1^\circ \ g'_n \leq f^+ \leq h'_n,\ g''_n \leq -f^- \leq h''_n; $
$ 2^\circ \ f^+ $ (resp. $-f^- $) is equal almost everywhere to the upper envelope of the $ g'_n $ and to the lower envelope of the $ h'_n $ (resp. to the upper envelope of the $ g''_n $ and to the lower envelope of the $ h''_n $); and $ 3^\circ $:
$$
\int f^+ d\mu = \lim_{n \to \infty} \int g'_n d\mu = \lim_{n \to \infty} \int h'_n d\mu,
$$
$$
-\int f^- d\mu = \lim_{n \to \infty} \int g''_n d\mu = \lim_{n \to \infty} \int h''_n d\mu.
$$
Moreover, we can suppose that the $ g'_n $ and the $ h''_n $ are everywhere finite; it is then clear that the sequences $ g_n = g'_n + g''_n $ and $ h_n = h'_n + h''_n $ meet the requirements.

#### Example {#int-iv-s4-n4-exa-1 .statement}

For every positive measure $ \mu $ on $ \mathbf{R} $, every *step function* with compact support is $ \mu $-integrable; for, the characteristic function of an open (resp. closed) interval is lower (resp. upper) semi-continuous, and every step function is a linear combination of such characteristic functions. It follows that if $ \mathbf{f} $ is a *regulated* function on $ \mathbf{R} $ with compact support (FRV, II, §1, No. 3), then $ \mathbf{f} $ is integrable, because it is the uniform limit of a sequence of step functions $ \mathbf{g}_n $ with support contained in a fixed compact set (No. 3, Prop. 3); moreover, $ \int \mathbf{f}\, d\mu = \lim_{n \to \infty} \int \mathbf{g}_n\, d\mu $.

If, in particular, $ \mu $ is taken to be Lebesgue measure, one sees that for every regulated function $ \mathbf{f} $ with compact support, the integral $ \int \mathbf{f}\, d\mu $ is equal to the integral $ \int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx $ defined in FRV, II, §2, No. 1.

#### Remark 1 {#int-iv-s4-n4-rem-1 .statement}

Let $ \mathbf{f} $ be a regulated function on $ \mathbf{R} $ that is integrable with respect to Lebesgue measure $ \mu $; then $ |\mathbf{f}| $ is also integrable (No. 2, Cor. 1 of Prop. 1), and, setting $ I_n = [-n, n] $, $ |\mathbf{f}| $ is the upper envelope of the increasing sequence of regulated functions $ |\mathbf{f}| \varphi_{I_n} $, therefore $ \int |\mathbf{f}|\, d\mu = \lim_{n \to \infty} \int_{-n}^{n} |\mathbf{f}(x)|\, dx $ by Th. 2 of No. 3; thus, the integral $ \int_{-\infty}^{+\infty} f(x) dx $ is *absolutely convergent* (FRV, II, §2, No. 3). Moreover, $ \int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx $ by Th. 2 of No. 3. Conversely, suppose that $ \int_{-\infty}^{+\infty} f(x) dx $ is absolutely convergent; again, by Th. 2 of No. 3, $ \int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx $. Note that if the integral $ \int_{-\infty}^{+\infty} f(x) dx $ is convergent but not absolutely convergent; then $ f $ *is not integrable* with respect to Lebesgue measure.

#### Remark 2 {#int-iv-s4-n4-rem-2 .statement}

Applied to Lebesgue measure and to regulated functions, Prop. 3 of No. 3 yields anew the theorem on passage to the limit for integrals of regulated functions on a compact interval (FRV, II, §3, No. 1, Prop. 1); for *sequences* (or for filters with a countable base) of regulated functions, Th. 2 of No. 3 greatly improves on this proposition since, for uniformly bounded regulated functions on a compact interval, it substitutes *pointwise* convergence for *uniform* convergence (cf. §5, No. 4, Th. 2). However, as regards the passage to the limit for *absolutely convergent* integrals of regulated functions on a noncompact interval, we note that the conditions of Th. 2 of No. 3 imply that the integrals under consideration are *uniformly convergent* (in the sense defined in FRV, II, §3, No. 2), and thus do not improve on the conditions for convergence given in Book IV (*loc. cit.*) except as concerns the convergence of the functions $ f_\alpha $ on every compact interval. Finally, the conditions for passing to the limit given for *non absolutely convergent* integrals of regulated functions remain outside the theory developed in this chapter.

### 5. Integrable sets

#### Definition 2 {#int-iv-s4-def-2 .statement}

*A subset* $ A $ *of a locally compact space* $ X $ *is said to be integrable with respect to a measure* $ \mu $ *on* $ X $ *(or, that it is* $ \mu $*-integrable)* *if the characteristic function* $ \varphi_A $ *of* $ A $ *is integrable.* *The finite number* $ \mu(A) = \int \varphi_A\, d\mu $ *is called the measure of* $ A $.

For every integrable set $ A $, $ |\mu|(A) = |\mu|^*(A) $ (No. 2, Prop. 1); for a set to be *negligible*, it is necessary and sufficient that it be of *measure zero with respect to* $ |\mu| $.

#### Proposition 6 {#int-iv-s4-prop-6 .statement}

*The union of a finite family* $ (A_i)_{1 \leq i \leq n} $ *of integrable sets is integrable,* and

$$
|\mu| \left( \bigcup_{i=1}^n A_i \right) \leq \sum_{i=1}^n |\mu|(A_i).
$$

*If, moreover, the* $ A_i $ *are pairwise disjoint,* then

$$
\mu \left( \bigcup_{i=1}^n A_i \right) = \sum_{i=1}^n \mu(A_i).
$$

For, if $ A = \bigcup_{i=1}^n A_i $ then $ \varphi_A = \sup \varphi_{A_i} $, therefore (\S3, No. 5, Cor. of Prop. 12) if the $ A_i $ are integrable then so is $ A $; the relation (13) is a special case of the analogous relation for outer measures (\S 1, No. 4, Prop. 18), on taking account of the relation $ |\mu|(A) = |\mu|^*(A) $; finally, if the $ A_i $ are pairwise disjoint, then $ \varphi_A = \sum_{i=1}^n \varphi_{A_i} $, whence (14).

#### Proposition 7 {#int-iv-s4-prop-7 .statement}

1° *If A and B are two integrable sets such that $ B \subset A $, then the set $ C = A - B $ is integrable and*

$$
\mu(C) = \mu(A) - \mu(B).
$$

2° *The intersection of a countable family of integrable sets is integrable.*

The first part follows from the fact that $ \varphi_C = \varphi_A - \varphi_B $. On the other hand, if $ (A_n) $ is a sequence of integrable sets and $ A $ is its intersection, then $ \varphi_A = \inf_n \varphi_{A_n} $, therefore $ A $ is integrable (No. 3, Prop. 4).

#### Corollary {#int-iv-s4-n5-cor-1 .statement}

*If $ (A_n) $ is a decreasing sequence of integrable sets, then* $ \mu(\bigcap_n A_n) = \lim_{n \to \infty} \mu(A_n) $.

For, if $ A = \bigcap_n A_n $ then $ \varphi_A $ is the lower envelope of the decreasing sequence $ (\varphi_{A_n}) $ (No. 3, Prop. 4).

#### Proposition 8 {#int-iv-s4-prop-8 .statement}

*Let $ (A_n) $ be an increasing sequence of integrable sets; for the union $ A = \bigcup_n A_n $ to be integrable, it is necessary and sufficient that* $ \sup_n |\mu|(A_n) < +\infty $, *in which case,*

$$
\mu(A) = \lim_{n \to \infty} \mu(A_n).
$$

For, the $ \varphi_{A_n} $ form an increasing sequence of integrable functions, and $ \varphi_A = \sup_n \varphi_{A_n} $; thus, the proposition follows from Prop. 4 of No. 3.

#### Corollary {#int-iv-s4-n5-cor-2 .statement}

*Let $ (A_n) $ be a sequence of integrable sets such that* $ \sum_{n=1}^\infty |\mu|(A_n) < +\infty $; *the union* $ A = \bigcup_n A_n $ *is integrable, and*

$$
|\mu| \left( \bigcup_n A_n \right) \leq \sum_{n=1}^\infty |\mu|(A_n).
$$

For, $ \varphi_A = \sup_n \varphi_{A_n} $ and

$$
|\mu|^*(A) \leq \sum_{n=1}^\infty |\mu|^*(A_n) = \sum_{n=1}^\infty |\mu|(A_n) < +\infty
$$

(§1, No. 4, Prop. 18); therefore A is integrable (§3, No. 6, Cor. 2 of Th. 5) and, since $|\mu|(A) = |\mu|^*(A)$, we indeed have (17).

#### Proposition 9 {#int-iv-s4-prop-9 .statement}

— Let $(A_n)$ be a sequence of pairwise disjoint integrable sets such that $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$; then

$$
\mu\left(\bigcup_n A_n\right) = \sum_{n=1}^\infty \mu(A_n).
$$

For, if $A = \bigcup_n A_n$ then $\varphi_A = \sum_{n=1}^\infty \varphi_{A_n}$, and the proposition follows from (17) and Cor. 2 of Th. 2 of No. 3.

The relation (18) is also expressed by saying that the measure $\mu$ is completely additive in the set of integrable subsets of $X$.

### 6. Criteria for the integrability of a set

#### Proposition 10 {#int-iv-s4-prop-10 .statement}

— For an open (resp. closed) set $A$ in $X$ to be integrable, it is necessary and sufficient that $|\mu|^*(A) < +\infty$.

Since $\varphi_A$ is then lower (resp. upper) semi-continuous, the proposition follows from Prop. 5 of No. 4 and its Corollary 1.

#### Corollary 1 {#int-iv-s4-prop-10-cor-1 .statement}

— Every compact set is integrable; every relatively compact open set is integrable.

#### Corollary 2 {#int-iv-s4-prop-10-cor-2 .statement}

— For every positive measure $\mu$ on $X$, $A \mapsto \mu^*(A)$ is a capacity on $X$ (cf. GT, IX, §6, No. 9, Example).

#### Example {#int-iv-s4-n6-exa-1 .statement}

For Lebesgue measure $\mu$ on $\mathbf{R}$, it follows from Prop. 10 that every bounded open interval $[a, b[$ is integrable and has measure $b - a$ (\§1, No. 2, Prop. 9). Since every set reducing to a point is negligible for Lebesgue measure, it follows that all of the intervals with endpoints $a$ and $b$ have the same measure $b - a$.

#### Proposition 11 {#int-iv-s4-prop-11 .statement}

— Let $\mathcal{G}$ be a set, directed for the relation $\subset$, of integrable open sets in $X$; for $A = \bigcup_{G \in \mathcal{G}} G$ to be integrable, it is necessary and sufficient that $\sup_{G \in \mathcal{G}} |\mu|(G) < +\infty$, in which case $\mu(A) = \lim_\mathcal{G} \mu(G)$ and $|\mu|(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$.

For, one knows that $|\mu|^*(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$ (\§1, No. 2, Prop. 7); the proposition therefore follows from Prop. 10.

#### Corollary {#int-iv-s4-n6-cor-1 .statement}

— Let $ \mathfrak{F} $ be a set, directed for the relation $ \supset $, of integrable closed sets in $ X $; then the closed set $ B = \bigcap_{H \in \mathfrak{F}} H $ is integrable, and one has
$$
\mu(B) = \lim_{\mathfrak{F}} \mu(H) \quad \text{and} \quad |\mu|(B) = \inf_{H \in \mathfrak{F}} |\mu|(H).
$$
For, let $ H_0 $ be a set in $ \mathfrak{F} $; since $ H_0 $ is integrable, it is contained in an integrable open set $ U $ (\S 1, No. 4, Prop. 19); the open sets $ U \cap \mathbf{C}H $ form a set directed for the relation $ \subset $, are contained in $ U $, and have union $ U \cap \mathbf{C}B $; we are thus reduced to Prop. 11.

#### Theorem 4 {#int-iv-s4-thm-4 .statement}

— For a set $ A $ to be integrable, it is necessary and sufficient that, for every $ \varepsilon > 0 $, there exist an integrable open set $ G $ and a compact set $ K $, such that $ K \subset A \subset G $ and
$$
|\mu|(G - K) = |\mu|(G) - |\mu|(K) \leq \varepsilon.
$$

a) The condition is *sufficient*, because it means that $ \varphi_K \leq \varphi_A \leq \varphi_G $ and $ \int (\varphi_G - \varphi_K) d|\mu| \leq \varepsilon $; since $ \varphi_G $ and $ \varphi_K $ are integrable, so is $ \varphi_A $ (\S 3, No. 4, Prop. 8).

b) The condition is *necessary*. If $ A $ is integrable, there exists an open set $ G \supset A $ such that $ |\mu|^*(G) $ is arbitrarily close to $ |\mu|^*(A) = |\mu|(A) $ (\S 1, No. 4, Prop. 19); thus, it all comes down to proving that for every $ \varepsilon > 0 $, there exists a compact set $ K \subset A $ such that $ |\mu|(A) - |\mu|(K) \leq \varepsilon $. Since $ \varphi_A $ is integrable, there exists a function $ f \geq 0 $, upper semi-continuous and with compact support $ S $, such that $ f \leq \varphi_A $ and $ \int (\varphi_A - f) d|\mu| \leq \varepsilon/2 $ (No. 4, Th. 3). Let $ \delta > 0 $ be an arbitrary number and let $ K $ be the set of points $ x \in X $ such that $ f(x) \geq \delta $; $ K $ is closed and is contained in $ S $, hence is *compact*, and since $ f \leq \varphi_A $ we have $ K \subset A $. The set $ B = A - K $ is integrable, and $ f \leq \varphi_K + \delta \varphi_B $, whence
$$
\int f d|\mu| \leq |\mu|(K) + \delta \cdot |\mu|(B) \leq |\mu|(K) + \delta \cdot |\mu|(A),
$$
and finally
$$
|\mu|(A) \leq \int f d|\mu| + \frac{\varepsilon}{2} \leq |\mu|(K) + \delta \cdot |\mu|(A) + \frac{\varepsilon}{2},
$$
which completes the proof, since $ \delta $ is arbitrary.

#### Corollary 1 {#int-iv-s4-thm-4-cor-1 .statement}

— For a set $ A $ to be integrable, it is necessary and sufficient that, for every $ \varepsilon > 0 $, there exist a compact set $ K \subset A $ such that $ |\mu|^*(A - K) \leq \varepsilon $. The measure $ |\mu|(A) $ is then the supremum of the set of measures $ |\mu|(K) $ of the compact sets $ K \subset A $.

The condition is necessary, because if $ G $ and $ K $ satisfy the conditions of Theorem 4, then $ |\mu|^*(A - K) \leq |\mu|^*(G - K) \leq \varepsilon $.

The condition is sufficient, because it says that, for the topology of convergence in mean, $ \varphi_A $ is in the closure of the set of integrable functions $ \varphi_K $ ($ K $ an arbitrary compact subset of $ A $).

#### Corollary 2 {#int-iv-s4-thm-4-cor-2 .statement}

— For every integrable set $ A $, there exist:

$ 1^\circ $ a set $ A_1 \supset A $, a countable intersection of integrable open sets, such that $ A_1 - A $ is negligible;

$ 2^\circ $ a set $ A_2 \subset A $, a countable union of pairwise disjoint compact sets, such that $ A - A_2 $ is negligible.

$ 1^\circ $ For every integer $ n $, there exists an integrable open set $ G_n \supset A $ such that $ |\mu|(G_n) - |\mu|(A) \leq 1/n $; if $ A_1 $ is the intersection of the $ G_n $, then $ |\mu|(A_1) = |\mu|(A) $ (No. 5, Cor. of Prop. 7), therefore $ A_1 - A $ is negligible.

$ 2^\circ $ Let us define compact sets $ K_n $ inductively as follows: $ K_1 \subset A $ and $ |\mu|(A - K_1) \leq 1 $; $ K_n \subset A - \bigcup_{i=1}^{n-1} K_i $ and $ |\mu|(A \cap \mathbf{C}(\bigcup_{i=1}^{n-1} K_i) \cap \mathbf{C}K_n) \leq 1/n $ for $ n > 1 $ (Th. 4); if $ A_2 $ is the union of the $ K_n $, then $ |\mu|(A_2) = |\mu|(A) $ (No. 5, Prop. 8), therefore $ A - A_2 $ is negligible.

#### Corollary 3 {#int-iv-s4-thm-4-cor-3 .statement}

— Every set of finite outer measure is contained in the union of a negligible set and a countable family of pairwise disjoint compact sets the sum of whose measures is finite.

It suffices to apply Corollary 2 to an integrable open set containing the given set.

#### Corollary 4 {#int-iv-s4-thm-4-cor-4 .statement}

— For every open set $ U $ in $ X $, $ |\mu|^*(U) $ is the supremum of the measures $ |\mu|(K) $ of the compact sets $ K \subset U $.

If $ |\mu|^*(U) < +\infty $, this is immediate from Th. 4. The following argument covers also the case that $ |\mu|^*(U) = +\infty $. Since $ X $ is locally compact and $ U $ is open, $ \varphi_U $ is the upper envelope of the set $ H $ of functions $ f \in \mathcal{K}_+ $ such that $ f \leq \varphi_U $ and $ \operatorname{Supp}(f) \subset U $ (cf. the proof of §1, No. 1, Lemma), and, since $ H $ is directed for $ \leq $, we have $ |\mu|^*(U) = \sup_{f \in H} |\mu|(f) $ by §1, No. 1, Th. 1; the corollary is then immediate from the fact that if $ f \in H $ and $ K = \operatorname{Supp}(f) $, then $ f \leq \varphi_K \leq \varphi_U $.

Note that $ |\mu|^*(U) $ is also the supremum of the measures $ |\mu|(G) $ of the relatively compact open sets such that $ \overline{G} \subset U $. For, if $ K $ is a compact set contained in $ U $ then, for every $ x \in K $, there exists a relatively compact open neighborhood $ V $ of $ x $ such that $ \overline{V} \subset U $. On covering $ K $ by a finite number of these neighborhoods, their union $ G $ is a relatively compact open set such that $ \overline{G} \subset U $ and $ K \subset G $, whence $ |\mu|(K) \leq |\mu|(G) \leq |\mu|^*(U) $.

### 7. Characterization of bounded measures

#### Proposition 12 {#int-iv-s4-prop-12 .statement}

— For a measure $ \mu $ on a locally compact space $ X $ to be bounded (Ch. III, §1, No. 8), it is necessary and sufficient that $ X $ be an integrable set with respect to $ \mu $ (or, what comes to the same thing, that every finite constant function be integrable); in this case,

$$
\| \mu \| = | \mu |(X) = \int d|\mu|.
$$

For, we have seen that $ |\mu|^*(X) = \| \mu \| $ (\S1, No. 2); the proposition therefore follows from Prop. 10 of No. 6.

For every bounded measure $ \mu $, we again say that $ \mu(X) $ is the total mass of $ \mu $.

It follows from Th. 4 of No. 6 that if $ \mu $ is a bounded measure then, for every $ \varepsilon > 0 $, there exists a compact set $ K $ such that $ |\mu|(CK) \leq \varepsilon $.

#### Proposition 13 {#int-iv-s4-prop-13 .statement}

— Let $ \mu $ be a bounded measure on $ X $. Let $ \mathcal{B} $ be a filter base on $ \mathcal{L}_F^p $ having the following properties:
$ 1^\circ $ there exists a set $ M \in \mathcal{B} $ such that the functions $ f \in M $ are uniformly bounded on $ X $;
$ 2^\circ $ $ \mathcal{B} $ converges uniformly on every compact subset of $ X $ to a function $ f_0 $.
Under these conditions, $ f_0 $ belongs to $ \mathcal{L}_F^p $ and $ \mathcal{B} $ converges in mean of order $ p $ to $ f_0 $.

We note first of all that if $ |f(x)| \leq a $ for every $ x \in X $ and every function $ f \in M $, then also $ |f_0(x)| \leq a $ for every $ x \in X $. This being so, for every $ \varepsilon > 0 $ there exist a compact set $ K $ such that $ |\mu|(CK) \leq \varepsilon^p $ and a set $ N \in \mathcal{B} $ such that, for every function $ f \in N $, $ |f(x) - f_0(x)| \leq \varepsilon(|\mu|(K))^{-1/p} $ for all $ x \in K $. Now, we may write

$$
f - f_0 = (f - f_0)\varphi_K + (f - f_0)\varphi_{CK};
$$

it follows from the foregoing that if $ f \in M \cap N $ then $ N_p((f - f_0)\varphi_K) \leq \varepsilon $ and $ N_p((f - f_0)\varphi_{CK}) \leq 2a\varepsilon $, whence $ N_p(f - f_0) \leq (2a + 1)\varepsilon $, which proves the proposition.

#### Corollary {#int-iv-s4-n7-cor-1 .statement}

— For a bounded measure $ \mu $ on $ X $, every bounded continuous mapping $ f $ of $ X $ into $ F $ belongs to each of the $ \mathcal{L}_F^p $ ($ 1 \leq p < +\infty $).

For every compact subset $ K $ of $ X $, let $ M_K $ be the set of mappings of $ X $ into $ F $ of the form $ hf $, where $ h $ is a continuous mapping of $ X $ into $[0, 1]$ equal to 1 on $ K $ and with compact support. It is clear that the sets $ M_K $ form a filter base $ \mathcal{B} $ on $ \mathcal{L}_F^p $, that the functions belonging to $ M_K $ are uniformly bounded, and that $ \mathcal{B} $ converges uniformly to $ f $ on every compact subset of $ X $, whence the corollary.

In particular, the function $ f $ is integrable and its integral $ \int f\, d\mu $ is the limit with respect to $ \mathcal{B} $ of the integrals $ \int h f\, d\mu $.

We will obtain anew the Cor. of Prop. 13 as a consequence of a general criterion for integrability in §5, No. 6.

In the notations of Ch. III, §1, No. 2, $ |f| \leq \|f\| \cdot 1 $ for every function $ f \in \mathcal{C}^b(X; F) $, whence, by the formulas (3) and (4) of No. 2,

$$
N_p(f) \leq \|f\| \cdot N_p(1) = \|f\| \cdot \|\mu\|^{1/p}.
$$

In particular, for $ p = 1 $, formula (5) of No. 2 yields

$$
\left| \int f\, d\mu \right| \leq \|f\| \cdot \|\mu\|,
$$

consequently the mapping $ f \mapsto \int f\, d\mu $ is continuous on the Banach space $ \mathcal{C}^b(X; F) $; its restriction to the closure $ \mathcal{C}^0(X; F) $ of $ \mathcal{K}(X; F) $ in $ \mathcal{C}^b(X; F) $, that is, to the space of continuous functions tending to 0 at the point at infinity (Ch. III, §1, No. 2, Prop. 3), is therefore the extension by continuity of the integral to $ \mathcal{C}^0(X; F) $.

### 8. Integration with respect to a measure with compact support

Let $ \mu $ be a measure on $ X $ whose support $ S = \operatorname{Supp}(\mu) $ is compact; the open set $ X - S $ is negligible (§2, No. 2, Prop. 5). For every function $ f $ with values in a vector space $ F $ or in $ \overline{\mathbf{R}} $, the functions $ f $ and $ f \varphi_S $ are therefore equivalent (§2, No. 4); for $ f $ to be $ \mu $-integrable (when $ F $ is a Banach space), it is therefore necessary and sufficient that $ f \varphi_S $ be so, in which case (No. 1)

$$
\int f\, d\mu = \int f \varphi_S\, d\mu.
$$

If, moreover, $ f $ is bounded on $ S $, it follows from (20) that

$$
\left| \int f\, d\mu \right| \leq \|\mu\| \cdot \sup_{x \in S} |f(x)|.
$$

In particular, if $ f $ is continuous on $ X $ then $ f $ is $ \mu $-integrable, since $ fh \in \mathcal{K}(X; F) $ for every function $ h \in \mathcal{K}(X; \mathbf{R}) $ equal to 1 on $ S $ (Ch. III, §1, No. 2, Lemma 1). More precisely:

#### Proposition 14 {#int-iv-s4-prop-14 .statement}

— Let X be a locally compact space, F a Banach space not reduced to 0; equip the space $ \mathcal{C}(X; F) $ of all continuous mappings of X into F with the topology of compact convergence. For a measure $ \mu $ on X to be such that the linear mapping $ f \mapsto \int f d\mu $ of $ \mathcal{K}(X; F) $ into F is extendible to a continuous linear mapping of $ \mathcal{C}(X; F) $ into F, it is necessary and sufficient that $ \operatorname{Supp}(\mu) $ be compact; such an extension is unique and coincides with the integral defined in No. 1.

We have just seen that if $ \mu $ has compact support, then the integral $ \int f d\mu $ is defined for every function $ f \in \mathcal{C}(X; F) $ and that the mapping $ f \mapsto \int f d\mu $ of $ \mathcal{C}(X; F) $ into F is continuous for the topology of compact convergence. Conversely, suppose that $ f \mapsto \int f d\mu $ is continuous in $ \mathcal{K}(X; F) $ for the topology of compact convergence. Then, there is a compact set $ K \subset X $ and a number $ a > 0 $ such that $ |\mu(f)| \leq a \cdot \sup_{x \in K} |f(x)| $ for every function $ f \in \mathcal{K}(X; F) $; in particular, if the support of $ g \in \mathcal{K}(X; F) $ does not intersect K, then $ \mu(g) = 0 $. Taking $ g = h a $, where $ a \neq 0 $ is a vector in F and $ h \in \mathcal{K}(X; \mathbf{C}) $, we see that $ \mu(h) = 0 $ for every function $ h \in \mathcal{K}(X; \mathbf{C}) $ whose support does not intersect K, which proves that $ \operatorname{Supp}(\mu) \subset K $. Finally, the uniqueness of the extension follows from the fact that $ \mathcal{K}(X; F) $ is dense in $ \mathcal{C}(X; F) $ for the topology of compact convergence (Ch. III, §1, No. 2, Prop. 4).

Prop. 14 permits identifying a measure on X with compact support with its continuous extension to $ \mathcal{C}(X; \mathbf{C}) $. The set of measures on X with compact support may therefore be identified with the dual $ \mathcal{C}'(X; \mathbf{C}) $ of the Hausdorff locally convex space $ \mathcal{C}(X; \mathbf{C}) $. Recall that $ \mathcal{C}(X; \mathbf{C}) $ is complete (GT, X, §1, No. 6, Cor. 3 of Th. 2), but it is not necessarily barreled (Exer. 17). However, if X is countable at infinity, hence is the union of an increasing sequence of compact sets $ K_n $ such that $ K_n \subset \overset{\circ}{K}_{n+1} $, then the topology of $ \mathcal{C}(X; \mathbf{C}) $ can be defined by the countable family of semi-norms $ p_n(f) = \sup_{x \in K_n} |f(x)| $, therefore $ \mathcal{C}(X; \mathbf{C}) $ is a Fréchet space in this case. Consequently, for every covering $ \mathcal{G} $ of $ \mathcal{C}(X; \mathbf{C}) $ by bounded sets, the space $ \mathcal{C}'(X; \mathbf{C}) $ is then quasi-complete for the $ \mathcal{G} $-topology (TVS, III, §4, No. 2, Cor. 4 of Th. 1).

We shall consider above all on $ \mathcal{C}'(X; \mathbf{C}) $ the topology of compact convergence (the topology of uniform convergence on the compact subsets of $ \mathcal{C}(X; \mathbf{C}) $). Recall that the relatively compact subsets H of $ \mathcal{C}(X; \mathbf{C}) $ are characterized by the following properties (GT, X, §2, No. 5, Cor. 3 of Th. 2):

$ 1^\circ $ H is equicontinuous;

$ 2^\circ $ for every $ x \in X $, the set $ H(x) $ of the $ f(x) $, where $ f $ runs over H, is bounded in $ \mathbf{C} $.

#### Proposition 15 {#int-iv-s4-prop-15 .statement}

— Let X be a locally compact space and, for every $ x \in X $, let $ \varepsilon_x $ be the Dirac measure at the point x. The mapping $ x \mapsto \varepsilon_x $ of X into $ \mathcal{C}'(X; \mathbf{C}) $ is continuous for the topology of compact convergence on $ \mathcal{C}'(X; \mathbf{C}) $.

Consider a neighborhood of $ \varepsilon_{x_0} $ in $ \mathcal{C}'(X; \mathbf{C}) $ for this topology, which we can suppose to be defined by taking a number $ \delta > 0 $, a compact subset H of $ \mathcal{C}(X; \mathbf{C}) $, and considering the set of measures $ \mu $ on X with compact support such that $ |\mu(f) - \varepsilon_{x_0}(f)| \leq \delta $ for every function $ f \in H $. Since H is equicontinuous, there exists a neighborhood U of $ x_0 $ in X such that the relation $ f \in H $ implies $ |f(x) - f(x_0)| \leq \delta $ for all $ x \in U $, which may also be written $ |\varepsilon_x(f) - \varepsilon_{x_0}(f)| \leq \delta $ and proves the proposition.(*)

#### Proposition 16 {#int-iv-s4-prop-16 .statement}

— Let K be a compact subset of X, L the vector space of measures $ \mu $ on X with support contained in K. On L, the topologies induced by the topology $ \mathcal{T} $ of compact convergence on $ \mathcal{C}'(X; \mathbf{C}) $ and the topology $ \mathcal{T}' $ of strictly compact convergence on $ \mathcal{M}(X; \mathbf{C}) $ (Ch. III, §1, No. 10) coincide.

It is clear that on L, the topology induced by $ \mathcal{T} $ is finer than the topology induced by $ \mathcal{T}' $. Conversely, let H be a compact subset of $ \mathcal{C}(X; \mathbf{C}) $, h a function in $ \mathcal{K}(X; \mathbf{C}) $ equal to 1 on K. It is clear that the set H' of functions $ fh $, where $ f $ runs over H, is strictly compact in $ \mathcal{K}(X; \mathbf{C}) $, and, for every measure $ \mu \in L $, $ \mu(f) = \mu(fh) $ for every function $ f \in H $, whence the conclusion.

#### Corollary 1 {#int-iv-s4-prop-16-cor-1 .statement}

— For every compact subset K of X and every number $ a > 0 $, the set B of measures $ \mu $ on X such that $ \operatorname{Supp}(\mu) \subset K $ and $ \| \mu \| \leq a $ is an equicontinuous subset of $ \mathcal{C}'(X; \mathbf{C}) $ that is compact for the topology $ \mathcal{T} $ of compact convergence.

For, let H be a subset of $ \mathcal{C}(X; \mathbf{C}) $ consisting of functions that are uniformly bounded on K; there exists a number $ c > 0 $ such that $ |\mu(f)| \leq c \cdot \| \mu \| \leq ac $ for every function $ f \in H $ and every measure $ \mu \in B $, by virtue of (22); therefore $ B \subset acH^\circ $ in the dual $ \mathcal{C}'(X; \mathbf{C}) $ of $ \mathcal{C}(X; \mathbf{C}) $, which proves the equicontinuity of B; the fact that B is compact for $ \mathcal{T} $ follows from the fact that, on B, $ \mathcal{T} $ and the vague topology induce the same topology (Prop. 16 and Ch. III, §1, No. 10, Prop. 17) and the fact that B is vaguely compact (Ch. III, §1, No. 9, Cor. 2 of Prop. 15 and §2, No. 2, Prop. 6).

#### Corollary 2 {#int-iv-s4-prop-16-cor-2 .statement}

— Every measure with compact support (resp. every positive measure with compact support) $ \mu $ is in the closure in $ \mathcal{C}'(X; \mathbf{C}) $, for the topology $ \mathcal{T} $ of compact convergence, of the set of measures (resp.

(*) In fact, the mapping $ x \mapsto \varepsilon_x $ is a homeomorphism of X into $ \mathcal{C}'(X; \mathbf{C}) $ (Ch. VI, §1, No. 6, Remark 1).

positive measures) whose support is finite and contained in Supp(\mu) and whose norm is equal to $ \| \mu \| $.

For, on the set B of measures $ \nu $ such that $ \mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu) $ and $ \| \nu \| \leq \| \mu \| $, the topology induced by the vague topology is identical to the topology induced by $ \mathcal{T} $, and the corollary therefore follows from Ch. III, §2, No. 4, Cors. 2 and 3 of Th. 1.

### 9. Clans and additive set functions

#### Definition 3 {#int-iv-s4-def-3 .statement}

*A nonempty set $ \Phi $ of subsets of a set $ A $ is said to be a clan if there exists an algebra $ \mathcal{A} $ (over $ \mathbf{R} $) consisting of real-valued functions defined on $ A $, such that the relations $ M \in \Phi $ and $ \varphi_M \in \mathcal{A} $ are equivalent.*

#### Example {#int-iv-s4-n9-exa-1 .statement}

If $ \mu $ is a measure on a locally compact space $ X $ then the linear combinations, with real coefficients, of the characteristic functions of integrable sets form an *algebra* $ \mathcal{A} $, because, for any two integrable sets $ M, N $, the function $ \varphi_M \varphi_N = \varphi_{M \cap N} $ is integrable (No. 5, Prop. 7); it then follows from Defs. 2 and 3 that the set of integrable subsets of $ X $ is a clan.

#### Proposition 17 {#int-iv-s4-prop-17 .statement}

*In order that a nonempty set $ \Phi $ of subsets of a set $ A $ be a clan, it is necessary and sufficient that it satisfy the following condition:*

(CL) *For every pair of sets $ M, N $ belonging to $ \Phi $, the sets $ M \cup N $ and $ M \cap \mathbf{C}N $ belong to $ \Phi $.*¹

The condition is *necessary*, by virtue of the relations

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N , \quad \varphi_{M \cap \mathbf{C}N} = \varphi_M - \varphi_M \varphi_N .
$$

To show that it is *sufficient*, we first observe that it implies that, for any two sets $ M, N $ in $ \Phi $, $ M \cap N $ belongs to $ \Phi $ since $ M \cap N = M \cap \mathbf{C}(M \cap \mathbf{C}N) $. Let $ \mathcal{E}(\Phi) $ be the set of linear combinations, with real coefficients, of the characteristic functions of the sets of $ \Phi $. Since $ \varphi_M \varphi_N = \varphi_{M \cap N} $, $ \mathcal{E}(\Phi) $ is an algebra. Everything comes down to showing that if $ M $ is a subset of $ A $ such that $ \varphi_M = \sum_i c_i \varphi_{M_i} $, where the $ M_i $ belong to $ \Phi $, then $ M \in \Phi $. This will result from the following lemma:

#### Lemma {#int-iv-s4-n9-lem-1 .statement}

*Let $ \Phi $ be a nonempty set of subsets of $ A $ satisfying the axiom (CL). Given a finite family $ (M_i)_{1 \leq i \leq n} $ of sets in $ \Phi $, there exists a*

¹ A clan $ \Phi $ of subsets of a set $ A $ is also known as a *ring* (or *Boolean ring*) of sets; if, moreover, $ A \in \Phi $, then $ \Phi $ is called an *algebra* (or *Boolean algebra*) of sets (cf. GT, I, §6, Exer. 20 and II, §4, Exer. 12). A Boolean algebra closed under countable unions is called a *tribe*, or *$ \sigma $*-*algebra* (GT, IX, §6, No. 3, Def. 3).

finite family $ (N_j)_{1 \leq j \leq m} $ of pairwise disjoint sets in $ \Phi $ such that each $ M_i $ is the union of a certain number of the $ N_j $.

For, consider the $ 2^n - 1 $ sets of the form $ \bigcap_{i=1}^n P_i $, where $ P_i = M_i $ for certain indices $ i $, $ P_i = \mathbf{C} M_i $ for the others, at least one of the $ P_i $ being equal to $ M_i $. Let $ (N_j)_{1 \leq j \leq m} $ be the sequence of these sets arranged in some order; they are pairwise disjoint and belong to $ \Phi $; on the other hand, every set $ M_k $ is the union of the sets $ N_j = \bigcap_{i=1}^n P_i $ corresponding to the families $ (P_i) $ such that $ P_k = M_k $, which proves the lemma.

The lemma established, every function of the form $ \sum_{i=1}^n c_i \varphi_{M_i} $, where $ M_i \in \Phi $, may be written in the form $ \sum_{j=1}^m d_j \varphi_{N_j} $, where the $ N_j $ belong to $ \Phi $ and are pairwise disjoint; if $ \varphi_M = \sum_{j=1}^m d_j \varphi_{N_j} $ then necessarily $ d_j = 0 $ or $ d_j = 1 $ for each index $ j $, thus $ M $ is the union of a certain number of the $ N_j $, and therefore belongs to $ \Phi $.

Every clan $ \Phi $ of subsets of $ A $ contains the empty subset $ \varnothing $ of $ A $; for, there exists at least one subset $ M \in \Phi $, therefore $ M - M = \varnothing $ belongs to $ \Phi $. Note also that the set of subsets of $ A $ consisting of the single subset $ \varnothing $ is a clan.

#### Definition 4 {#int-iv-s4-def-4 .statement}

*Given a clan $ \Phi $ of subsets of a set $ A $, and a Banach space $ F $, one calls step function*² *over the sets of $ \Phi $ (or $ \Phi $-step function), with values in $ F $, every function of the form* $ \sum_i a_i \varphi_{M_i} $, *where the $ a_i $ belong to $ F $, and the $ M_i $ to $ \Phi $.*

It is clear that the set $ \mathcal{E}_F(\Phi) $ of $ \Phi $-step functions with values in $ F $ is a vector space over $ \mathbf{R} $ or $ \mathbf{C} $. We have just seen in Prop. 17 that the set $ \mathcal{E}(\Phi) $ of real-valued $ \Phi $-step functions is an *algebra* over $ \mathbf{R} $; it is also the linear subspace of $ \mathbf{R}^A $ generated by the characteristic functions of the sets of $ \Phi $.

By the Lemma, every function in $ \mathcal{E}_F(\Phi) $ may be written $ f = \sum_j c_j \varphi_{N_j} $, where the $ N_j \in \Phi $ are pairwise disjoint; from this it follows that $ |f| = \sum_j |c_j| \varphi_{N_j} $ belongs to $ \mathcal{E}(\Phi) $. In particular, $ \mathcal{E}(\Phi) $ is a *Riesz space*, since the upper envelope of two functions in $ \mathcal{E}(\Phi) $ belongs to $ \mathcal{E}(\Phi) $.

#### Remark {#int-iv-s4-n9-rem-1 .statement}

— It is easily seen that Def. 4 is equivalent to the following: a $ \Phi $-step function with values in $ F $ is a function $ f $ that takes on only a finite number of values and which is such that, for every $ a \neq 0 $ in $ F $, the set $ f(a)^{-1} $ belongs to $ \Phi $.

² Fonction étagée, whence the notation $ \mathcal{E}(\Phi) $ in what follows.

#### Definition 5 {#int-iv-s4-def-5 .statement}

— *A real-valued function* $ \lambda $ *defined on a clan* $ \Phi $ *of subsets of a set* $ A $ *is said to be additive if, for every pair* $ M, N $ *of disjoint sets belonging to* $ \Phi $, $ \lambda(M \cup N) = \lambda(M) + \lambda(N) $.

It follows in particular from this definition that $ \lambda(\varnothing) = 0 $.

#### Proposition 18 {#int-iv-s4-prop-18 .statement}

— *Let* $ \lambda $ *be an additive set function defined on a clan* $ \Phi $. *There exists one and only one linear form* (again denoted $ \lambda $) *on the vector space* $ \mathcal{E}(\Phi) $ *of real-valued* $ \Phi $*-step functions*, *such that* $ \lambda(\varphi_M) = \lambda(M) $ *for every set* $ M \in \Phi $; *if, moreover,* $ \lambda(M) \geqslant 0 $ *for every* $ M \in \Phi $, *then* $ \lambda $ *is a positive linear form on* $ \mathcal{E}(\Phi) $.

The *uniqueness* of the linear form $ \lambda $ is clear, since the characteristic functions of the sets in $ \Phi $ generate the vector space $ \mathcal{E}(\Phi) $. To prove the *existence* of $ \lambda $, it suffices to prove that the relation $ \sum_i c_i \varphi_{M_i} = 0 $, where the $ M_i $ are nonempty sets belonging to $ \Phi $, implies $ \sum_i c_i \lambda(M_i) = 0 $.

Now, by the Lemma there exists a finite family $ (N_j) $ of pairwise disjoint nonempty sets in $ \Phi $ such that, for every index $ i $, $ \varphi_{M_i} = \sum_j a_{ij} \varphi_{N_j} $ with $ a_{ij} = 0 $ or $ a_{ij} = 1 $. The relation $ \sum_i c_i \varphi_{M_i} = 0 $, which may be written $ \sum_j \left( \sum_i c_i a_{ij} \right) \varphi_{N_j} = 0 $, therefore implies that $ \sum_i c_i a_{ij} = 0 $ for every index $ j $. By Def. 5, we then have

$$
\sum_i c_i \lambda(M_i) = \sum_j \left( \sum_i c_i a_{ij} \right) \lambda(N_j) = 0,
$$

which proves the existence of $ \lambda $. Finally, suppose that $ \lambda(M) \geqslant 0 $ for every $ M \in \Phi $; for every function $ f \in \mathcal{E}(\Phi) $, one can write $ f = \sum_i c_i \varphi_{M_i} $, where the $ M_i \in \Phi $ are pairwise disjoint; if $ f \geqslant 0 $, it follows that $ c_i \geqslant 0 $ for every index $ i $ such that $ M_i $ is nonempty, whence $ \lambda(f) = \sum_i c_i \lambda(M_i) \geqslant 0 $.

### 10. Approximation of continuous functions by step functions

#### Proposition 19 {#int-iv-s4-prop-19 .statement}

— *Let* $ X $ *be a locally compact space,* $ \Phi $ *a clan of subsets of* $ X $, *containing the set of compact subsets of* $ X $. *For every continuous mapping* $ f $ *of* $ X $ *into a Banach space* $ F $ *(resp. every continuous, real-valued function* $ f \geqslant 0 $ *on* $ X $) *with compact support* $ K $, *there exists a sequence* $ (g_n) $ *of functions in* $ \mathcal{E}_F(\Phi) $ *with support contained in* $ K $ *(resp. a sequence* $ (g_n) $ *of functions in* $ \mathcal{E}(\Phi) $ *such that* $ 0 \leqslant g_n \leqslant f $ *for every* $ n $) *that converges uniformly to* $ f $ *(resp. $ f $).

Since $ f $ is uniformly continuous on $ K $, one can cover $ K $ by a finite number of compact sets $ M_i $ ($ 1 \leq i \leq m $) such that the oscillation of $ f $ on each $ M_i $ is $ \leq 1/n $. Since the $ M_i $ and $ K $ belong to $ \Phi $, there exists a partition of $ K $ into sets $ N_j \in \Phi $ such that each of the sets $ M_i \cap K $ is the union of a certain number of the $ N_j $ (No. 9, Lemma). Let $ a_j $ be an element of $ F $ such that $ |f(x) - a_j| \leq 1/n $ on $ N_j $. Setting $ g_n = \sum_j a_j \varphi_{N_j} $, we have $ |f - g_n| \leq 1/n $, whence the proposition in this case. One argues similarly for a continuous real-valued function $ f $, on taking $ a_j = \inf_{x \in N_j} f(x) $ and $ g_n = \sum_j a_j \varphi_{N_j} $.

#### Corollary 1 {#int-iv-s4-prop-19-cor-1 .statement}

*Let $ \mu $ be a measure on $ X $; the space $ \mathcal{E}_F(\Phi) $ is dense in each of the spaces $ \mathcal{L}_F^p $ ($ 1 \leq p < +\infty $).*

For, it follows from Prop. 19 and the criterion for convergence in mean for uniform limits of functions with compact support (\S 3, No. 3, Prop. 4) that $ \mathcal{E}_F(\Phi) $ is dense, for the topology of convergence in mean of order $ p $, in the closure of the space $ \mathcal{K}_F $ of continuous functions with compact support, whence the corollary.

#### Corollary 2 {#int-iv-s4-prop-19-cor-2 .statement}

*For every closed subset $ S $ of $ X $, every function $ f \in \mathcal{K}(X, S; \mathbf{C}) $ is the uniform limit of linear combinations $ \sum_i \lambda_i \varphi_{K_i} $, where the $ \lambda_i $ belong to $ \mathbf{C} $ and the $ K_i $ are compact subsets of $ S $.*

The set $ \mathcal{A} $ of such linear combinations is a $ \mathbf{C} $-algebra. Let $ \Phi $ be the set of subsets $ M $ of $ X $ such that $ \varphi_M \in \mathcal{A} $; $ \Phi $ is thus a *clan* all of whose elements are subsets of $ S $, containing the compact subsets of $ S $, and $ \mathcal{E}_C(\Phi) \subset \mathcal{A} $. It then suffices to apply Prop. 19 to the locally compact space $ S $ and the clan $ \Phi $.

#### Corollary 3 {#int-iv-s4-prop-19-cor-3 .statement}

*If $ \mu $ and $ \nu $ are two measures on $ X $ such that $ \mu(K) = \nu(K) $ for every compact subset $ K $ of $ X $, then $ \mu = \nu $.*

For, it follows from Cor. 2 and the definition of a measure that, for every compact subset $ S $ of $ X $, $ \mu $ and $ \nu $ take on the same values in $ \mathcal{K}(X, S; \mathbf{C}) $.

### 11. Extension of a measure defined on a family of sets

Let $ \Phi $ be a nonempty set of subsets of a locally compact space $ X $. Given a real-valued function $ M \mapsto \alpha(M) $, defined and $ \geq 0 $ on $ \Phi $, we propose to seek conditions under which there exists a positive measure $ \mu $ on $ X $ such that the sets of $ \Phi $ are $ \mu $-integrable and $ \mu(M) = \alpha(M) $ for all $ M \in \Phi $. We shall limit ourselves to considering the case that the set $ \Phi $ satisfies the following conditions:

(PC_I) *The union and intersection of two sets of $ \Phi $ belong to $ \Phi $.*

(PC_{II}) *For every pair consisting of a compact set K and an open set U in X such that $ K \subset U $, there exists a set $ M \in \Phi $ such that $ K \subset M \subset U $.*

Note that the condition (PC_{II}) implies that $ \varnothing \in \Phi $, by taking $ K = U = \varnothing $. However, the set $ \Phi $ is not necessarily a clan; for example, the set of all compact subsets of X satisfies the conditions (PC_I) and (PC_{II}), but in general is not a clan, because if M and N are compact, the same is not in general true of $ M \cap \mathbf{C}N $.

We shall assume in addition that the function $ \alpha $ defined on $ \Phi $ satisfies the following conditions (obviously necessary for the problem to have a solution):

(PM_I) *The relation $ M \subset N $ implies $ \alpha(M) \leq \alpha(N) $.*
(PM_{II}) *For any M and N in $ \Phi $, $ \alpha(M \cup N) \leq \alpha(M) + \alpha(N) $.*
(PM_{III}) *The relation $ M \cap N = \varnothing $ implies $ \alpha(M \cup N) = \alpha(M) + \alpha(N) $.*

On taking $ N = \varnothing $ in the condition (PM_{III}), one deduces that $ \alpha(\varnothing) = 0 $; the condition (PM_I) then shows that $ \alpha(M) \geq 0 $ for every $ M \in \Phi $.

#### Theorem 5 {#int-iv-s4-thm-5 .statement}

*Let $ \Phi $ be a set of subsets of a locally compact space X, satisfying (PC_I) and (PC_{II}), and let $ \alpha $ be a real-valued function, defined on $ \Phi $, satisfying the conditions (PM_I), (PM_{II}) and (PM_{III}). In order that there exist a positive measure $ \mu $ on X such that the sets of $ \Phi $ are $ \mu $-integrable and $ \mu(M) = \alpha(M) $ for all $ M \in \Phi $, it is necessary and sufficient that $ \alpha $ satisfy in addition the following condition:*

(PM_{IV}) *For every $ \varepsilon > 0 $ and every $ M \in \Phi $, there exist a compact set $ K \subset M $ and an open set $ U \supset M $ such that, for every $ N \in \Phi $ satisfying the relation $ K \subset N \subset U $, one has $ |\alpha(N) - \alpha(M)| \leq \varepsilon $.*

*Moreover, if the condition (PM_{IV}) is satisfied, then the measure $ \mu $ is unique; for every compact set $ K $, $ \mu(K) = \inf_{M \in \Phi, M \supset K} \alpha(M) $; for every open set $ U $, $ \mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M) $.*

Note that the condition (PM_{IV}) is equivalent to the conjunction of the following two:

(PM'_{IV}) *For every $ \varepsilon > 0 $ and every $ M \in \Phi $, there exists an open set $ U \supset M $ such that, for every $ N \in \Phi $ contained in $ U $, $ \alpha(N) \leq \alpha(M) + \varepsilon $.*
(PM''_{IV}) *For every $ \varepsilon > 0 $ and every $ M \in \Phi $, there exists a compact set $ K \subset M $ such that, for every $ N \in \Phi $ containing $ K $, $ \alpha(N) \geq \alpha(M) - \varepsilon $.*

For, it is obvious that (PM'_{IV}) and (PM''_{IV}) imply (PM_{IV}). Conversely, let us show for example that (PM_{IV}) implies (PM'_{IV}): let K be a compact set and U an open set such that $ K \subset M \subset U $ and $ |\alpha(P) - \alpha(M)| \leq \varepsilon $ for every $ P \in \Phi $ satisfying $ K \subset P \subset U $. Then, if $ N \in \Phi $ and $ N \subset U $, $ M \cup N $ belongs to $ \Phi $ and $ K \subset M \cup N \subset U $, whence $ \alpha(M \cup N) \leq \alpha(M) + \varepsilon $ and *a fortiori* $ \alpha(N) \leq \alpha(M) + \varepsilon $.

When the set $ \Phi $, satisfying (PC_I) and (PC_{II}), consists of *compact* sets, then the condition (PM''_{IV}) is trivially verified, and (PM_{IV}) is then equivalent to (PM'_{IV}).

The condition (PM_{IV}) is *necessary*: this follows at once from Th. 4 of No. 6 on the 'approximation' of an integrable set by a compact set and an open set. To prove the other assertions of the theorem, we proceed in several steps.

1° Definition of a topology on $ \mathfrak{P}(X) $.

For every pair $(K, U)$ consisting of a compact set $K$ and an open set $U$ in $X$, we denote by $I(K, U)$ the set of subsets $M \subset X$ such that $K \subset M \subset U$; in order that $I(K, U)$ be nonempty, it is necessary and sufficient that $K \subset U$. If $(K', U')$ is a second pair, formed by a compact set $K'$ and an open set $U'$, we have
$$
I(K, U) \cap I(K', U') = I(K \cup K', U \cap U').
$$
Let $T$ be the topology on $\mathfrak{P}(X)$ generated by the set of subsets $I(K, U)$ as $K$ runs over the set of compact subsets of $X$, and $U$ over the set of open subsets of $X$; by the foregoing, the $I(K, U)$ form a base for the topology $T$ (GT, I, §1, No. 3).

We observe that the definition of $T$ implies that, in $\mathfrak{P}(X)$, the set of compact subsets of $X$ is dense. The condition (PC_{II}) expresses that $\Phi$ is dense in $\mathfrak{P}(X)$, and condition (PM_{IV}) expresses that the function $\alpha$ is continuous on $\Phi$ for the topology induced by $T$. Finally, Th. 4 of No. 6 expresses that the function $M \mapsto \mu(M)$ is continuous on the clan of $\mu$-integrable sets, for the topology induced by $T$.

2° Uniqueness of $\mu$.

We denote by $\overline{\Phi}$ the set of subsets $M \subset X$ such that $\alpha(N)$ tends to a finite limit as $N$ tends to $M$ (for the topology $T$) while remaining in $\Phi$; we may then extend $\alpha$ in only one way to a continuous mapping $\overline{\alpha}$ of $\overline{\Phi}$ into $\mathbf{R}$ (GT, I, §8, No. 5, Th. 1). If there exists a measure $\mu$ meeting the requirements, the above remarks prove that the clan $\Psi$ of $\mu$-integrable sets is contained in $\overline{\Phi}$ and that $\mu(M) = \overline{\alpha}(M)$ for every $M \in \Psi$; this relation holds in particular for every compact subset $M$ of $X$, which proves the uniqueness of $\mu$ (No. 10, Cor. 3 of Prop. 19).

3° Extension of $\alpha$ to the compact sets.

Without assuming the existence of $\mu$, we are now going to study the set $\overline{\Phi}$ and the extension $\overline{\alpha}$ of $\alpha$ to $\overline{\Phi}$. We first show that every compact set $K$ belongs to $\overline{\Phi}$ and that $\overline{\alpha}(K) = \inf_{P \in \Phi, P \supset K} \alpha(P)$. Set $a = \inf_{P \in \Phi, P \supset K} \alpha(P)$; for every $\varepsilon > 0$, there exists an $M \in \Phi$ such that $K \subset M$ and $\alpha(M) \leq a + \varepsilon$. By (PM'_{IV}), there exists an open set $U \supset M$ such that, for every $N \in \Phi$ contained in $U$, we have $\alpha(N) \leq \alpha(M) + \varepsilon \leq a + 2\varepsilon$; for every $N \in \Phi$ such that $K \subset N \subset U$, we therefore have $a \leq \alpha(N) \leq a + 2\varepsilon$, which, by the definitions, shows that $K \in \overline{\Phi}$ and $\overline{\alpha}(K) = a$.

This result proves at once that if $K_1$ and $K_2$ are two compact sets such that $K_1 \subset K_2$, then $\overline{\alpha}(K_1) \leq \overline{\alpha}(K_2)$. If $K_1$ and $K_2$ are any two compact sets, we have $\overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$ by (PM_{II}). We shall see, moreover, that if $K_1$ and $K_2$ are disjoint then $\overline{\alpha}(K_1 \cup K_2) = \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$. For, there then exist two disjoint open sets $U_1, U_2$ such that $K_1 \subset U_1$, $K_2 \subset U_2$ (GT, II, §4, Prop. 4). Therefore, by (PC_{II}), there also exist two sets $M_1 \in \Phi$, $M_2 \in \Phi$ such that $K_1 \subset M_1 \subset U_1$ and $K_2 \subset M_2 \subset U_2$. Now let $P$ be any set of $\Phi$ containing $K_1 \cup K_2$; the union of the two sets $P \cap M_1$ and $P \cap M_2$ belongs to $\Phi$ by (PC_{I}), and since these two sets are disjoint, application of (PM_I) and (PM_{III}) yields

$$
\alpha(P) \geq \alpha(P \cap M_1) + \alpha(P \cap M_2) \geq \overline{\alpha}(K_1) + \overline{\alpha}(K_2),
$$

which establishes our assertion.

**4° Extension of $ \alpha $ to the open sets.**

We shall now see that, for an open set $ U $ to belong to $ \overline{\Phi} $, it is necessary and sufficient that, as $ K $ runs over the set of compact subsets of $ U $, the supremum of the numbers $ \overline{\alpha}(K) $ is finite; moreover, $ \overline{\alpha}(U) $ is then equal to this supremum.

For, let $ U $ be an open set belonging to $ \overline{\Phi} $; for every $ \varepsilon > 0 $ there exists a compact set $ K \subset U $ such that, for every set $ M \in \Phi $ satisfying $ K \subset M \subset U $, one has $ |\overline{\alpha}(U) - \alpha(M)| \leq \varepsilon $, whence $ |\overline{\alpha}(U) - \overline{\alpha}(K)| \leq \varepsilon $; on the other hand, if $ K' $ is any compact set contained in $ U $, then $ K \subset K \cup K' \subset U $, whence $ |\overline{\alpha}(U) - \overline{\alpha}(K \cup K')| \leq \varepsilon $ and so $ \overline{\alpha}(U) \geq \overline{\alpha}(K \cup K') - \varepsilon \geq \overline{\alpha}(K') - \varepsilon $; $ \overline{\alpha}(U) $ is therefore indeed equal to the supremum of the numbers $ \overline{\alpha}(K) $ as $ K $ runs over the set of compact subsets of $ U $.

Conversely, let $ U $ be an open set such that $ b = \sup_{K \subset U} \overline{\alpha}(K) < +\infty $ ($ K $ running over the set of compact subsets of $ U $), and let us show that $ U \in \overline{\Phi} $. For every $ \varepsilon > 0 $, there exists a compact set $ K \subset U $ such that $ b - \varepsilon \leq \overline{\alpha}(K) \leq b $; by (PM''_{IV}), for every set $ M \in \Phi $ such that $ K \subset M \subset U $, there exists a compact set $ K' \subset M $ such that

$$
\alpha(M) \leq \overline{\alpha}(K') + \varepsilon \leq b + \varepsilon;
$$

therefore $ b - \varepsilon \leq \alpha(M) \leq b + \varepsilon $, which proves that $ U \in \overline{\Phi} $.

From this characterization of the open sets $ U \in \overline{\Phi} $, and of $ \overline{\alpha}(U) $, it follows first of all that if $ U_1 $ and $ U_2 $ are two open sets such that $ U_1 \subset U_2 $ and $ U_2 \in \overline{\Phi} $, then $ U_1 \in \overline{\Phi} $ and $ \overline{\alpha}(U_1) \leq \overline{\alpha}(U_2) $. On the other hand, if $ U_1 $ and $ U_2 $ are two open sets belonging to $ \overline{\Phi} $, then the same is true of $ U_1 \cup U_2 $, and $ \overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2) $. For, let $ K $ be any compact set contained in $ U_1 \cup U_2 $; for every point $ x \in K $, there exists a compact neighborhood of $ x $ contained in either $ U_1 $ or $ U_2 $; one can therefore cover $ K $ by a finite number of these neighborhoods; if $ K_1 $ (resp. $ K_2 $) is the union of those that are contained in $ U_1 $ (resp. $ U_2 $), then $ K \subset K_1 \cup K_2 $, whence

$$
\overline{\alpha}(K) \leq \overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2),
$$

which establishes the asserted property.

**5° Properties of $ \overline{\Phi} $ and $ \overline{\alpha} $.**

The definition of $ \overline{\Phi} $ and $ \overline{\alpha} $ can now be transformed as follows (taking into account (PC_{II})): in order that $ M \in \overline{\Phi} $, it is necessary and sufficient that, for every $ \varepsilon > 0 $, there exist a compact set $ K $ and an open set $ U \in \overline{\Phi} $ such that $ K \subset M \subset U $ and $ \overline{\alpha}(U) - \overline{\alpha}(K) \leq \varepsilon $; $ \overline{\alpha}(M) $ is, moreover, the *infimum* of the $ \overline{\alpha}(U) $ for the open sets $ U \in \overline{\Phi} $ containing $ M $, and the *supremum* of the $ \overline{\alpha}(K) $ for the compact sets $ K \subset M $.

From this, we shall first deduce that if $ M_1, M_2 $ and $ M_1 \cup M_2 $ belong to $ \overline{\Phi} $, then $ \overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2) $. Indeed, if $ U_1 $ and $ U_2 $ are two open sets of $ \overline{\Phi} $ containing $ M_1 $ and $ M_2 $, respectively, and such that $ \overline{\alpha}(U_1) \leq \overline{\alpha}(M_1) + \varepsilon $ and $ \overline{\alpha}(U_2) \leq \overline{\alpha}(M_2) + \varepsilon $, then $ U_1 \cup U_2 $ belongs to $ \overline{\Phi} $, contains $ M_1 \cup M_2 $, and consequently

$$
\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2) + 2\varepsilon,
$$

whence our assertion.

Next, let us show that if $ K $ is a compact set and $ U $ is an open set of $ \overline{\Phi} $ such that $ K \subset U $, then $ \overline{\alpha}(U - K) = \overline{\alpha}(U) - \overline{\alpha}(K) $. By the foregoing, we have $ \overline{\alpha}(U) \leq \overline{\alpha}(K) + \overline{\alpha}(U - K) $. On the other hand, for every compact set $ K' \subset U - K $,

$$
\overline{\alpha}(K \cup K') = \overline{\alpha}(K) + \overline{\alpha}(K') \leq \overline{\alpha}(U);
$$

since $ U - K $ is open and belongs to $ \overline{\Phi} $, $ \overline{\alpha}(U - K) $ is the supremum of the $ \overline{\alpha}(K') $, which shows that $ \overline{\alpha}(K) + \overline{\alpha}(U - K) \leq \overline{\alpha}(U) $.

The definition of $ \overline{\Phi} $ may therefore now be expressed in the following way: in order that $ M \in \overline{\Phi} $, it is necessary and sufficient that, for every $ \varepsilon > 0 $, there exist a compact set $ K $ and an open set $ U \in \overline{\Phi} $ such that $ K \subset M \subset U $ and $ \overline{\alpha}(U - K) \leq \varepsilon $.

We are now in a position to prove that $ \overline{\Phi} $ *is a clan* and $ \overline{\alpha} $ an *additive set function* on $ \overline{\Phi} $. We first show that if $ M $ and $ N $ belong to $ \overline{\Phi} $ then so do $ M \cap \mathbf{C}N $ and $ M \cup N $. By hypothesis, for every $ \varepsilon > 0 $ there exist two compact sets $ K, K' $ and two open sets $ U, U' $ of $ \overline{\Phi} $ such that

$$
K \subset M \subset U,\quad K' \subset N \subset U',\quad \overline{\alpha}(U - K) \leq \varepsilon,\quad \overline{\alpha}(U' - K') \leq \varepsilon.
$$

The set $ K'' = K \cap \mathbf{C}U' $ is compact, the set $ U'' = U \cap \mathbf{C}K' $ is open and belongs to $ \overline{\Phi} $, and $ K'' \subset M \cap \mathbf{C}N \subset U'' $; on the other hand, $ U'' - K'' $ is contained in the union of $ U \cap \mathbf{C}K $ and $ U' \cap \mathbf{C}K' $, whence $ \overline{\alpha}(U'' - K'') \leq 2\varepsilon $, which proves that $ M \cap \mathbf{C}N \in \overline{\Phi} $. Similarly, $ U_1 = U \cup U' $ is open and belongs to $ \overline{\Phi} $, $ K_1 = K \cup K' $ is compact, and $ K_1 \subset M \cup N \subset U_1 $; on the other hand, $ U_1 - K_1 $ is contained in the union of $ U - K $ and $ U' - K' $, whence again $ \overline{\alpha}(U_1 - K_1) \leq 2\varepsilon $, and $ M \cup N $ belongs to $ \overline{\Phi} $. Finally, if $ M $ and $ N $ are disjoint, then

$$
\overline{\alpha}(K_1) = \overline{\alpha}(K) + \overline{\alpha}(K') \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon,
$$

consequently $ \overline{\alpha}(M \cup N) \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon $; since $ \varepsilon $ is arbitrary, we have $ \overline{\alpha}(M \cup N) = \overline{\alpha}(M) + \overline{\alpha}(N) $.

**6° Existence of the measure $ \mu $.**

By Prop. 18 of No. 9, there exists one and only one positive linear form $ \beta $ on the vector space $ \mathcal{E}(\overline{\Phi}) $ of $ \overline{\Phi} $-step functions, such that $ \beta(\varphi_M) = \overline{\alpha}(M) $ for all $ M \in \overline{\Phi} $. For every compact subset $ K $ of $ X $, let us denote by $ \mathcal{G}(K) $ the space of *uniform limits* of functions of $ \mathcal{E}(\overline{\Phi}) $ whose support is contained in $ K $. Since $ \beta $ is positive, $ |\beta(f)| \leq \overline{\alpha}(K) \cdot \|f\| $ for every function $ f \in \mathcal{E}(\overline{\Phi}) $ whose support is contained in $ K $; the restriction of $ \beta $ to the space of these functions is a *continuous* linear form for the topology of uniform convergence; it may therefore be extended to a positive continuous linear form $ \overline{\beta}_K $ on $ \mathcal{G}(K) $. Moreover, if $ K \subset K_1 $, then the restriction of $ \overline{\beta}_{K_1} $ to $ \mathcal{G}(K) $ is identical to $ \overline{\beta}_K $, therefore there exists a positive linear form $ \overline{\beta} $ on the union $ \mathcal{G} $ of the $ \mathcal{G}(K) $, that extends each of the forms $ \overline{\beta}_K $.

Now, since every compact set belongs to $ \overline{\Phi} $, the space $ \mathcal{H} $ of continuous real-valued functions with compact support is a *subspace* of $ \mathcal{G} $ (No. 10, Prop. 19); the *restriction* to $ \mathcal{H} $ of the positive linear form $ \overline{\beta} $ is therefore a positive *measure* $ \mu $. Let us show that for every compact set $ K $, $ \mu(K) = \overline{\alpha}(K) $. For every $ \varepsilon > 0 $, there exists an open set $ U \in \overline{\Phi} $ such that $ K \subset U $, $ \mu(U) \leq \mu(K) + \varepsilon $ and $ \overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon $. Let $ f $ be a continuous mapping of $ X $ into $[0, 1]$ whose support is contained in $ U $ and such that $ f(x) = 1 $ on $ K $ (Ch. III, §1, No. 2, Lemma 1). Then $ \mu(K) \leq \mu(f) \leq \mu(U) \leq \mu(K) + \varepsilon $, and, on the other hand,

$$
\overline{\alpha}(K) = \beta(\varphi_K) \leq \overline{\beta}(f) \leq \beta(\varphi_U) = \overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon;
$$

since $ \mu(f) = \overline{\beta}(f) $, we see that $ |\mu(K) - \overline{\alpha}(K)| \leq \varepsilon $, and since $ \varepsilon $ is arbitrary, $ \mu(K) = \overline{\alpha}(K) $.

The characterization of the open sets belonging to $ \overline{\Phi} $, combined with Cor. 4 of Th. 4 of No. 6, then shows that the open sets belonging to $ \overline{\Phi} $ are none other than the $ \mu $-integrable open sets, and that, for such a set $ U $, we have $ \mu(U) = \overline{\alpha}(U) $. Th. 4 of No. 6 and the characterization of the sets of $ \overline{\Phi} $ given in 5° then show that the $ \mu $-integrable sets are the sets of $ \overline{\Phi} $ and that, for such a set $ M $, $ \mu(M) = \overline{\alpha}(M) $. Finally, the fact that $ \mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M) $ for every open set $ U $ follows at once from (PC$_{II}$) and Cor. 4 of Th. 4 of No. 6.

Theorem 5 is thus completely proved.

#### Corollary {#int-iv-s4-n11-cor-1 .statement}

— *Let X be a locally compact space with a countable base, $ \Psi $ the set of Borel sets of X, $ \beta $ a mapping of $ \Psi $ into $[0, +\infty]$ satisfying the following conditions:*

(i) *If* $ (B_1, B_2, \ldots) $ *is a sequence of pairwise disjoint Borel sets of X, then* $ \beta(B_1 \cup B_2 \cup \ldots) = \beta(B_1) + \beta(B_2) + \ldots $.

(ii) *If B is a compact subset of X, then* $ \beta(B) < +\infty $.

*Then, there exists one and only one positive measure $ \mu $ on X such that* $ \beta(B) = \mu^*(B) $ *for all* $ B \in \Psi $.

Let $ \Phi $ be the set of compact subsets of $ X $ and let $ \alpha $ be the restriction of $ \beta $ to $ \Phi $. The conditions (PC$_I$), (PC$_{II}$), (PM$_I$), (PM$_{II}$), (PM$_{III}$) and (PM$_{IV}'$) are then satisfied. Let $ K $ be a compact subset of $ X $, and $ \varepsilon > 0 $. Then $ K $ is the intersection of a decreasing sequence $ (U_1, U_2, \ldots) $ of relatively compact open sets of $ X $ (GT, IX, §2, No. 5, Prop. 7). We have $ \sum_{n=1}^{\infty} \beta(U_n - U_{n+1}) = \beta(U_1 - K) < +\infty $, therefore

$$
\beta(U_n) - \beta(K) = \beta(U_n - K) = \sum_{p=n}^{\infty} \beta(U_p - U_{p+1})
$$

tends to 0 as $ n $ tends to $ \infty $. This proves that the condition $(\mathrm{PM}'_{\mathrm{IV}})$ is satisfied. By Th. 5, there exists a positive measure $ \mu $ on $ X $ such that $ \mu(K) = \alpha(K) $ for every compact subset $ K $ of $ X $. Since every open set $ U $ of $ X $ is the union of an increasing sequence of compact subsets, we have $ \mu^*(U) = \beta(U) $. Let $ L $ be a compact subset of $ X $. By Prop. 7 of No. 5, the $ \mu $-integrable subsets of $ L $ form a tribe of subsets of $ L $. Therefore, if $ B $ is an element of $ \Psi $ contained in $ L $, then $ B $ is $ \mu $-integrable; for every $ \varepsilon > 0 $, there then exist a compact set $ K $ and an open set $ U $ in $ X $ such that $ K \subset B \subset U $ and $ \mu^*(U) - \mu(K) \leq \varepsilon $ (No. 6, Th. 4). Since $ \beta(U) = \mu^*(U) $ and $ \beta(K) = \mu(K) $, we see that $ |\mu^*(B) - \beta(B)| \leq 2\varepsilon $. Therefore $ \beta(B) = \mu^*(B) $. Finally, every Borel set $ C $ of $ X $ is the union of a sequence of pairwise disjoint, relatively compact Borel sets, whence $ \beta(C) = \mu^*(C) $. The uniqueness of $ \mu $ follows at once from Th. 5.

### Exercises {#int-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
