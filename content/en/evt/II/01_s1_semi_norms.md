---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 1
section_title: Semi-norms
lang: en
source: evt-i-v
pdf_pages: 0038-0044
extraction: ocr
subsections:
    - "no": 1
      title: Definition of semi-norms
      page: 0
      pdf_page: 38
    - "no": 2
      title: Topologies defined by semi-norms
      page: 2
      pdf_page: 39
    - "no": 3
      title: Semi-norms in quotient spaces and in product spaces
      page: 4
      pdf_page: 41
    - "no": 4
      title: Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms
      page: 5
      pdf_page: 42
statements: 15
exercises: 0
content_sha256: 91c4d031e3ebb3825cc2f99598c1def259a421c106f44ab8650a4d069bf4464d
---

## § 1. SEMI-NORMS

Throughout this paragraph, $ \mathbf{K} $ denotes a non-discrete valued division ring.

### 1. Definition of semi-norms

#### Definition 1 {#evt-ii-s1-def-1 .statement}

Let E be a left vector space over $ \mathbf{K} $. A mapping $ p $ of E in $ \mathbf{R}_+ = \{ 0, + \infty \} $, is called a semi-norm on E if it satisfies the following axioms :
(SN_I) If $ x \in \mathrm{E} $ and $ \lambda \in \mathbf{K} $ then $ p(\lambda x) = |\lambda| \, p(x) $.
(SN_II) If $ x \in \mathrm{E} $ and $ y \in \mathrm{E} $ then $ p(x + y) \leq p(x) + p(y) $.

Since $ p(x) \leq p(y) + p(x - y) $ and $ p(y) \leq p(x) + p(y - x) $, from $ p(y - x) = p(x - y) $, we deduce
$$
|p(x) - p(y)| \leq p(x - y) .
$$

#### Example 1 {#evt-ii-s1-n1-exa-1 .statement}

A norm on E is a semi-norm $ p $ such that the relation $ p(x) = 0 $ implies that $ x = 0 $ (I, p. 3).

#### Example 2 {#evt-ii-s1-n1-exa-2 .statement}

For every linear form $ f $ on E, the function $ x \mapsto |f(x)| $ is a semi-norm on E.

#### Example 3 {#evt-ii-s1-n1-exa-3 .statement}

If $ p_i (1 \leq i \leq n) $ is a finite set of semi-norms on E, then clearly $ p'(x) = \sup_{1 \leq i \leq n} p_i(x) $
and $ p''(x) = \sum_{i=1}^n \alpha_i p_i(x) $ (where the $ \alpha_i $ are $ \geq 0 $) are both semi-norms on E.

A mapping $ p $ of E in $ \mathbf{R}_+ $ is called an *ultra-semi-norm* if it satisfies (SN$_I$) and the following axiom :

(SN$_{II}'$) *If $ x \in E $ and $ y \in E $, then $ p(x + y) \leq \sup(p(x), p(y)) $.*

Clearly an ultra-semi-norm is a semi-norm.

To say that the absolute value on K is *ultrametric* (CA, VI, § 6.2) means that it is an ultra-semi-norm on the left vector space $ K_s $, which is not identically zero.

#### Proposition 1 {#evt-ii-s1-prop-1 .statement}

*Let E be a left topological vector space over K and let p be a semi-norm on E. The following conditions are equivalent :*
  *a)* *p is continuous in E.*
  *b)* *p is continuous at the point 0.*
  *c)* *p is uniformly continuous.*
  *d)* *For each real number $ \alpha > 0 $, the set W(p, $ \alpha $), of those $ x \in E $ for which $ p(x) < \alpha $, is open in E.*
  *e)* *There exists a real number $ \alpha > 0 $, such that W(p, $ \alpha $) is a neighbourhood of 0 in E.*
  *f)* *For every real number $ \alpha > 0 $, the set V(p, $ \alpha $), of those $ x \in E $ for which $ p(x) \leq \alpha $, is a neighbourhood of 0 in E.*

In fact, the implications c) $ \Rightarrow $ a) $ \Rightarrow $ b) $ \Rightarrow $ d) $ \Rightarrow $ e) $ \Rightarrow $ f) $ \Rightarrow $ c) follow immediately from (SN$_I$) and inequality (1).

#### Corollary {#evt-ii-s1-n1-cor-1 .statement}

*If p is a continuous semi-norm on E and q is a semi-norm such that $ q \leq p $, then q is continuous in E.*

When p is an *ultra-semi-norm* on E, then the sets W(p, $ \alpha $) and V(p, $ \alpha $) are *both open and closed*. For, we have seen that W(p, $ \alpha $) is open; on the other hand if z is a cluster point of W(p, $ \alpha $), then there exists $ y \in W(p, \alpha) $ such that $ p(y - z) < \alpha $, and from (SN$_{II}'$) we have $ p(z) < \alpha $, thus W(p, $ \alpha $) is closed. Also, V(p, $ \alpha $) is closed since p is continuous; further if $ p(x) \leq \alpha $ and $ p(y) \leq \alpha $, then $ p(x + y) \leq \alpha $ by (SN$_{II}'$), and this shows that V(p, $ \alpha $) is open.

### 2. Topologies defined by semi-norms

Let p be a semi-norm on the vector space E over K; for every $ \alpha > 0 $ let V(p, $ \alpha $) be the subset of those x of E for which $ p(x) \leq \alpha $. Clearly, if $ x \in V(p, \alpha) $ and $ \lambda \in K $ is such that $ |\lambda| \leq 1 $, then $ \lambda x \in V(p, \alpha) $, in other words V(p, $ \alpha $) is *balanced*. Further, for every $ x_0 \in E $, there exists a non-zero scalar $ \mu \in K $ such that $ |\mu| \geq p(x_0) \alpha^{-1} $, therefore $ \mu^{-1} x_0 \in V(p, \alpha) $ that is to say V(p, $ \alpha $) is *absorbent*. Finally, from (SN$_{II}$), we have $ V(p, \alpha/2) + V(p, \alpha/2) \subset V(p, \alpha) $, and from (SN$_I$) that for every non-zero scalar $ \lambda $ in K we have $ \lambda V(p, \alpha) = V(p, |\lambda| \alpha) $. We conclude from these remarks, by I, p. 7, prop. 4, that, when $ \alpha $ varies in the set of numbers $ > 0 $ (or only in a sequence of strictly positive numbers tending to 0) then the sets V(p, $ \alpha $) constitute a fundamental system of neighbourhoods of 0 for a topology compatible with the vector space structure of E; we say that this topology is *defined by the semi-norm p*. A vector space E with such a topology is called a *semi-normed space*. Note that if W(p, $ \alpha $) is the subset of x of E such that $ p(x) < \alpha $, then the W(p, $ \alpha $) constitute (where $ \alpha > 0 $, or $ \alpha $ varies in a strictly positive sequence of numbers tending to zero) a fundamental system of neighbourhoods of 0 for the topology defined by $ p $.

If $ \Gamma $ is a set of semi-norms on $ E $, then the *upper bound* of the topologies defined by the semi-norms $ p \in \Gamma $ is compatible with the vector space structure (I, p. 10, cor. 4). A fundamental system of neighbourhoods of 0, for this topology, is given by the finite intersections $ \bigcap_i V(p_i, \alpha_i) $ where $ p_i \in \Gamma $ and $ \alpha_i > 0 $. This topology is said to be *defined by the set of semi-norms* $ \Gamma $. It is the *coarsest* topology on $ E $ amongst those that are invariant under all translations and for which the semi-norms $ p \in \Gamma $ are continuous.

Let $ E $ be a topological vector space over $ K $: a system of semi-norms on $ E $, say $ \Gamma $, is called a *fundamental system of semi-norms* if the topology on $ E $ is the same as the topology defined by $ \Gamma $.

Let $ E $ be a vector space over $ K $, with the topology defined by a set of semi-norms $ \Gamma $. For every semi-norm $ p $, we have $ p(x - z) \leq p(x - y) + p(y - z) $, which shows that the function $ (x, y) \mapsto p(x - y) $ is a *pseudometric* on $ E $ (GT, IX, § 1.1): it follows from the definitions that, when $ p $ varies in $ \Gamma $, the set of these pseudometrics defines the uniform structure of the topological vector space $ E $.

#### Remark {#evt-ii-s1-n2-rem-1 .statement}

— 1) The topology defined by a *finite* set of semi-norms $ p_i $ ($ 1 \leq i \leq n $) on $ E $, can be defined by the *single* semi-norm $ p = \sup_{1 \leq i \leq n} p_i $. But a topology defined by an infinite set of semi-norms cannot, in general, be defined by a single semi-norm (III, p. 37, exerc. 2).

2) Let $ (\mathcal{T}_i)_{i \in I} $ be a family of topologies on a vector space $ E $ over $ K $, each of which is defined by a family of semi-norms $ \Gamma_i $. Then the topology defined by the set of semi-norms $ \Gamma = \bigcup_{i \in I} \Gamma_i $ is the upper bound of the topologies $ \mathcal{T}_i $.

3) If $ \Gamma_0 $ is a set of semi-norms *directed by the increasing* order relation defined between two semi-norms $ p, q $ on $ E $ by « there exists $ \lambda > 0 $ such that $ p \leq \lambda q $ », then a fundamental system of neighbourhoods of 0, for the topology defined by $ \Gamma_0 $, is obtained by taking the sets $ V(p, \alpha) $ where $ p \in \Gamma_0 $ and $ \alpha > 0 $. If $ \Gamma $ is any set of semi-norms on $ E $, then a filtered set of semi-norms, defining the same topology as $ \Gamma $, is the set $ \Gamma_0 $ of upper envelopes of all finite families of semi-norms belonging to $ \Gamma $.

4) Even if $ K = \mathbf{R} $, the topology of a topological vector space over $ K $ cannot always be defined by a set of semi-norms (*cf.* II, p. 24, corollary).

#### Example {#evt-ii-s1-n2-exa-1 .statement}

— Let $ \mathscr{C}^\infty(\mathbf{R}) $ be the vector space over $ \mathbf{R} $ of real valued functions that are infinitely differentiable in $ \mathbf{R} $. For every function and every pair of integers $ n \geq 0 $, $ m \geq 1 $, put

$$
p_{n,m}(f) = \sup_{-m \leq t \leq m} |f^{(n)}(t)|
$$

with $ f^{(0)} = f $. Obviously the $ p_{n,m} $ are semi-norms on $ \mathscr{C}^\infty(\mathbf{R}) $. In order that the functions $ f_\alpha $ tend to 0 (following a filter $ \mathfrak{F} $ on the set of indices) in $ \mathscr{C}^\infty(\mathbf{R}) $ for the topology $ \mathcal{T} $ defined by the semi-norms $ p_{n,m} $, it is necessary and sufficient that for all integers $ n \geq 0 $, the functions $ f_\alpha^{(n)} $ tend to 0 (following $ \mathfrak{F} $) *uniformly on every compact subset of* $ \mathbf{R} $. We say that $ \mathcal{T} $ is the *topology of compact convergence for the functions* $ f \in \mathscr{C}^\infty(\mathbf{R}) $ *and all their derivatives* (*cf.* III, p. 9).

#### Proposition 2 {#evt-ii-s1-prop-2 .statement}

*On a vector space* $ E $, *let* $ \mathcal{T} $ *be the topology defined by a set of semi-norms* $ \Gamma $.

(i) *The closure of {0} in E, for $ \mathcal{T} $, is the subset of $ x \in E $ for which $ p(x) = 0 $ for every semi-norm $ p \in \Gamma $.*

(ii) *If $ \mathcal{T} $ is Hausdorff and $ \Gamma $ is enumerable, then $ \mathcal{T} $ is metrisable.*

The proposition follows immediately from the definitions and from GT, IX, § 2 . 4, cor. 1.

Note that if $ \mathcal{T} $ is metrisable, it may be that $ \mathcal{T} $ cannot be defined by a single norm; this is the case in the example given above (*cf.* IV, p. 18, *Example 4*).

Let E be a vector space over K, with the topology defined by a set of semi-norms $ \Gamma $. Let $ \hat{E} $ be the Hausdorff completion of E (I, p. 6), and $ \hat{\Gamma} $ be the set of mappings $ \hat{p} $ of $ \hat{E} $ in $ \mathbf{R}_+ $ where $ p $ varies in $ \Gamma $ (GT, II, § 3 . 7, prop. 15). By the principle of extending inequalities, the functions $ \hat{p} \in \hat{\Gamma} $ are semi-norms on $ \hat{E} $, and the functions $ \hat{p}(x - y) $ form a set of pseudometrics defining the uniform structure of $ \hat{E} $ (GT, IX, § 1 . 3, prop. 1). We see, therefore, that $ \hat{\Gamma} $ is a fundamental set of semi-norms defining the topology of $ \hat{E} $.

### 3. Semi-norms in quotient spaces and in product spaces

Let E be a topological vector space over K, whose topology is defined by $ \Gamma $, a set of semi-norms. Clearly, the restrictions of the semi-norms of $ \Gamma $ to a vector sub-space M of E, define the topology induced on M by that of E.

Let $ \phi $ be the canonical mapping of E on the vector quotient space E/M. We show that, for every semi-norm $ p $ on E, the function

$$
\dot{p}(z) = \inf_{\phi(x) = z} p(x)
$$

is a semi-norm on E/M. In fact, it is clear that $ \dot{p} $ satisfies the condition (SN$_1$); on the other hand, if $ z', z'' $ are two vectors of E/M, we have:

$$
\begin{align*}
\inf_{\phi(x) = z' + z''} p(x) &\leq \inf_{\phi(x') = z', \phi(x'') = z''} p(x' + x'') \\
&\leq \inf_{\phi(x') = z', \phi(x'') = z''} (p(x') + p(x'')) \\
&= \inf_{\phi(x') = z'} p(x') + \inf_{\phi(x'') = z''} p(x'')
\end{align*}
$$

which shows that $ \dot{p} $ verifies (SN$_2$). We say that $ \dot{p} $ is the *quotient semi-norm* of $ p $ by M.

The same reasoning proves that, if $ p $ is an *ultra-semi-norm*, then so also is $ \dot{p} $.

This being so, we have (in the notation of No. 2)

$$
\phi(\mathrm{W}(p, \alpha)) = \mathrm{W}(\dot{p}, \alpha)
$$

for every $ \alpha > 0 $. In fact, to say that $ \dot{p}(z) < \alpha $, means that there exists $ x \in E $ such that $ \phi(x) = z $ and $ p(x) < \alpha $, from which the relation (4) follows.

We deduce from this, that, if the set of semi-norms $ \Gamma $ is *directed* (II, p. 3, *Remark 3*), then the quotient topology on $ E/M $ is defined by the set of semi-norms $ \dot{p} $, when $ p $ varies in $ \Gamma $.

If $ N $ is the closure of $ \{0\} $ in $ E $, the topology of $ E/N $ is defined by the quotient semi-norms $ \dot{p} $, where $ p $ varies in $ \Gamma $ (even if $ \Gamma $ is not filtered): here $ \dot{p}(\dot{x}) = p(x) $ for every $ x $ belonging to the class $ \dot{x} \mod N $. Note that $ E/N $ is none other than the Hausdorff space associated with $ E $ (I, p. 4).

Let $ E $ be a vector space over $ K $ and $ (E_i)_{i \in I} $ be a family of vector spaces over $ K $, where $ E_i $ has the topology $ \mathcal{T}_i $ defined by a set of semi-norms $ \Gamma_i $. For each $ i \in I $, let $ f_i $ be a linear mapping of $ E $ in $ E_i $; clearly when $ p_i $ varies in the set $ \Gamma_i $, then the $ p_i \circ f_i $ form a set $ \Gamma'_i $ of semi-norms on $ E $. The topology $ \mathcal{T} $ on $ E $, defined as being the coarsest of all those which make all the mappings $ f_i $ continuous (I, p. 9) is then defined by the set of semi-norms $ \Gamma' = \bigcup_{i \in I} \Gamma'_i $, this follows from the definition of neighbourhoods of 0 for $ \mathcal{T} $ (GT, I, § 2.3, prop. 4).

If the $ p_i $ are ultra-semi-norms, then so are the $ p_i \circ f_i $.

Let $ E $ be a vector space over $ K $, with the topology $ \mathcal{T} $ defined by a family of semi-norms $ (p_i)_{i \in I} $; for every $ i \in I $, let $ \mathcal{T}_i $ be the topology defined by the single semi-norm $ p_i $, and denote by $ E_i $ the space obtained from $ E $ using the topology $ \mathcal{T}_i $. Then the topology $ \mathcal{T} $ is the inverse image by the diagonal mapping $ \Delta : E \to \prod_{i \in I} E_i $ of the product topology on $ \prod_{i \in I} E_i $ (I, p. 9, prop. 7). For each $ i \in I $, write $ N_i $ for the closure of $ \{0\} $ in $ E_i $, and by $ F_i = E_i / N_i $, the *normed* space defined by the norm $ p_i $ corresponding to $ p_i $ (II, p. 4, formula (3)); if $ \phi_i : E_i \to F_i $ is the canonical mapping and $ \phi : (x_i) \mapsto (\phi_i(x_i)) $ the product mapping, we know that the product topology on $ \prod_{i \in I} E_i $ is the inverse image by $ \phi $ of the product topology on $ \prod_{i \in I} F_i $ (GT, II, § 3.9, prop. 18). The topology $ \mathcal{T} $ is, therefore, the inverse image under the composite mapping $ \phi \circ \Delta $ of the product topology on $ \prod_{i \in I} F_i $. In particular, if $ \mathcal{T} $ is *Hausdorff* then it follows from II, p. 3, prop. 2 that the mapping $ \phi \circ \Delta $ is *injective*, therefore:

#### Proposition 3 {#evt-ii-s1-prop-3 .statement}

*Every Hausdorff topological vector space* $ E $ *over* $ K $, *whose topology is defined by a set of semi-norms, is isomorphic to a sub-space of a product of Banach spaces*.

If, further, the topology of $ E $ is defined by an *enumerable* set of semi-norms, then $ E $ is *metrisable* (I, p. 16).

### 4. Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms

#### Proposition 4 {#evt-ii-s1-prop-4 .statement}

*Let* $ E_i $ ($ 1 \leq i \leq n $) *and* $ F $ *be topological vector spaces over* $ K $; *we suppose that, for every* $ i $, *the topology of* $ E_i $ *is defined by a directed set of semi-norms* $ \Gamma_i $, *and that the topology of* $ F $ *is defined by a set of semi-norms* $ \Gamma $. *Then a set* $ H $, *of* multilinear mappings of $ \prod_{i=1}^n E_i $ in F is equicontinuous if, and only if, for each semi-norm $ q \in \Gamma $, and each index i, there exists a semi-norm $ p_i \in \Gamma_i $, and a number $ a > 0 $, such that for each function $ u \in \mathbf{H} $ and point $ (x_i) \in \prod_{i=1}^n E_i $,

$$
q(u(x_1, x_2, ..., x_n)) \leq a \cdot p_1(x_1)\ p_2(x_2) ... p_n(x_n) .
$$

The condition is sufficient since it implies that H is equicontinuous at (0, 0, ..., 0) and therefore everywhere (I, p. 9, prop. 6).

We show that the condition is necessary. By hypothesis, for every semi-norm $ q \in \Gamma $ and every number $ \beta > 0 $, we have $ q(u(x_1, x_2, ..., x_n)) \leq \beta $ for every function $ u \in \mathbf{H} $ provided that $ p_i(x_i) \leq \alpha_i $ are true for each index $ i $, $ 1 \leq i \leq n $, and certain appropriately chosen numbers $ \alpha_i > 0 $ and semi-norms $ p_i \in \Gamma_i $. As K is non-discrete, we can also suppose that, for every $ i $, we have $ \alpha_i = |\lambda_i| < 1 $ where $ \lambda_i \in \mathbf{K} $. Then let $ (x_1, x_2, ..., x_n) $ be any point of $ \prod_{i=1}^n E_i $, and for each index $ i $, let $ m_i \in \mathbf{Z} $ be an integer such that $ p_i(x_i) \leq |\lambda_i|^{m_i + 1} $; this can be written as $ p_i(\lambda_i^{-m_i} x_i) \leq |\lambda_i| $ ($ 1 \leq i \leq n $), therefore, by hypothesis, we have

$$
q(u(x_1, x_2, ..., x_n)) \leq \beta |\lambda_1|^{m_1} |\lambda_2|^{m_2} ... |\lambda_n|^{m_n} .
$$

Suppose firstly that one of the $ p_i(x_i) $ is zero, then we can take $ m_i \in \mathbf{N} $ arbitrarily large, therefore $ q(u(x_1, x_2, ..., x_n)) = 0 $. If, on the contrary, all the $ p_i(x_i) $ are $ \neq 0 $, take the integer $ m_i $ such that $ |\lambda_i|^{m_i + 2} < p_i(x_i) \leq |\lambda_i|^{m_i + 1} $ for each $ i $; then we have $ |\lambda_i|^{m_i} < |\lambda_i|^{-2} p_i(x_i) $, from which, by (6), the relation (5) follows with

$$
a = \beta (|\lambda_1| \cdot |\lambda_2| ... |\lambda_n|)^{-2} .
$$

Q.E.D.

#### Corollary {#evt-ii-s1-n4-cor-1 .statement}

— *The set H is equicontinuous if, and only if, for every semi-norm $ q \in \Gamma $, there exists a neighbourhood of 0 in $ \prod_{i=1}^n E_i $, in which the functions $ q \circ u $, for $ u \in \mathbf{H} $, are uniformly bounded.*

The condition is evidently necessary, and the demonstration of prop. 4 shows that it implies an inequality of the form (5) for all $ u \in \mathbf{H} $, and therefore the equicontinuity of H.

We state explicitly the particular case of prop. 4 for linear mappings.

#### Proposition 5 {#evt-ii-s1-prop-5 .statement}

— *Let E, F be two topological vector spaces over a non-discrete valued division ring K; suppose that the topology of E (resp. F) is defined by a set of semi-norms $ \Gamma $ (resp. $ \Gamma' $). Let H be a set of linear mappings of E in F. The following conditions are equivalent :*
    a) H is equicontinuous.

b) For every semi-norm $ q \in \Gamma' $, there exists a finite family $ (p_i)_{1 \leq i \leq n} $ of semi-norms belonging to $ \Gamma $ and a number $ a > 0 $ such that, for all $ x \in E $ and all $ u \in H $,

$$
q(u(x)) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) .
$$

c) For every semi-norm $ q \in \Gamma' $, the mapping $ \sup_{u \in H} (q \circ u) $ is a continuous semi-norm on $ E $.

#### Corollary 1 {#evt-ii-s1-prop-5-cor-1 .statement}

— Suppose that $ \mathcal{T}, \mathcal{T}' $ are two topologies on a vector space $ E $ over $ K $ defined, respectively, by two sets of semi-norms $ \Gamma $ and $ \Gamma' $. $ \mathcal{T} $ is finer than $ \mathcal{T}' $ if, and only if, for every semi-norm $ q \in \Gamma' $, there exists a finite family $ (p_i)_{1 \leq i \leq n} $ of semi-norms belonging to $ \Gamma $ and a number $ a > 0 $ such that, for all $ x \in E $, we have $ q(x) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) $.

In fact this shows that the identity mapping of $ E $ with topology $ \mathcal{T} $, on $ E $ with topology $ \mathcal{T}' $, is continuous.

#### Corollary 2 {#evt-ii-s1-prop-5-cor-2 .statement}

— Suppose that the topology $ \mathcal{T} $ of a topological vector space $ E $ over $ K $ is defined by a directed set of semi-norms $ \Gamma $; for each semi-norm $ p \in \Gamma $, let $ E_p $ be the space obtained from $ E $ using the topology defined by $ p $. The set $ E' $ of linear forms on $ E $ that are continuous for $ \mathcal{T} $ is the union of the sets $ E'_p $, where $ E'_p $ is the set of continuous linear forms in $ E_p $ ($ p \in \Gamma $).
