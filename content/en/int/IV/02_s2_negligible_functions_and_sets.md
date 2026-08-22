---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 2
section_title: Negligible functions and sets
lang: en
source: int-i-vi
book_pages: INT IV.11-INT IV.17
pdf_pages: 0118-0124
extraction: ocr
subsections:
    - "no": 1
      title: Negligible positive functions
      page: 11
      pdf_page: 118
    - "no": 2
      title: Negligible sets
      page: 12
      pdf_page: 119
    - "no": 3
      title: Properties true almost everywhere
      page: 12
      pdf_page: 119
    - "no": 4
      title: Classes of equivalent functions
      page: 13
      pdf_page: 120
    - "no": 5
      title: Functions defined almost everywhere
      page: 15
      pdf_page: 122
    - "no": 6
      title: Equivalence classes of functions with values in $ \overline{\mathbf{R}} $
      page: 16
      pdf_page: 123
statements: 15
exercises: 0
content_sha256: 4c7361ff9ebcb8d02ec514c9d8d173e91d54e1788dc634c0d028257f3a1b39af
---

## § 2. NEGLIGIBLE FUNCTIONS AND SETS

### 1. Negligible positive functions

#### Definition 1 {#int-iv-s2-def-1 .statement}

— *Given a measure $\mu$ on a locally compact space X*, *a numerical function* $f \geq 0$ (*finite or not*) *defined on X is said to be negligible for the measure $\mu$ if* $|\mu|^*(f) = 0$.

We then also say that $f$ is $\mu$*-negligible*, or simply *negligible* if no confusion can result.

#### Proposition 1 {#int-iv-s2-prop-1 .statement}

— *If* $f$ *is a negligible function* $\geq 0$, *then every numerical function* $g$ *such that* $0 \leq g \leq \alpha f$ ($\alpha$ *a scalar* $> 0$) *is negligible*. For, $0 \leq |\mu|^*(g) \leq \alpha |\mu|^*(f) = 0$.

#### Proposition 2 {#int-iv-s2-prop-2 .statement}

— *The sum and upper envelope of a sequence* $(f_n)$ *of negligible functions* $\geq 0$ *are negligible*.

For, $ |\mu|^*(\sum_n f_n) \leq \sum_n |\mu|^*(f_n) = 0 $ (\S1, No. 3, Prop. 13) and $ \sup_n f_n \leq \sum_n f_n $.

#### Proposition 3 {#int-iv-s2-prop-3 .statement}

*For a lower semi-continuous function $ f \geq 0 $ on $ X $ to be negligible, it is necessary and sufficient that $ f $ be zero on the support of $ \mu $.*

If $ |\mu|^*(f) = 0 $ then $ |\mu|(g) = 0 $ for every function $ g \in \mathcal{K}_+ $ such that $ g \leq f $; it follows (Ch. III, \S2, No. 3, Prop. 9) that $ g $ is zero on the support $ S $ of $ \mu $; since $ f $ is the upper envelope of the functions $ g \in \mathcal{K}_+ $ such that $ g \leq f $ (\S1, No. 1, Lemma), $ f(x) = 0 $ on $ S $. Conversely, if $ f(x) = 0 $ on $ S $ then $ g(x) = 0 $ on $ S $ for every function $ g \in \mathcal{K}_+ $ such that $ g \leq f $, therefore (Ch. III, \S2, No. 3, Prop. 8) $ |\mu|(g) = 0 $, which, by definition, implies that $ |\mu|^*(f) = 0 $.

### 2. Negligible sets

#### Definition 2 {#int-iv-s2-def-2 .statement}

*Given a measure $ \mu $ on a locally compact space $ X $, a subset $ A $ of $ X $ is said to be negligible for the measure $ \mu $ if $ |\mu|^*(A) = 0 $.*

One also says that $ A $ is $ \mu $-negligible, or simply negligible if no confusion can result. It comes to the same thing to say that the characteristic function $ \varphi_A $ is negligible.

#### Proposition 4 {#int-iv-s2-prop-4 .statement}

*Every subset of a negligible set is negligible; every countable union of negligible sets is negligible.*

This is an immediate consequence of Props. 1 and 2.

#### Example {#int-iv-s2-n2-exa-1 .statement}

— Let $ \mu $ be Lebesgue measure on $ \mathbf{R} $. Every set $ \{x_0\} $ reduced to a point is negligible (cf. \S1, No. 3, *Remark* 1). It follows that *every countable subset of $ \mathbf{R} $ is negligible for Lebesgue measure*. The converse of this proposition is incorrect (\S4, Exer. 4 b)).

#### Proposition 5 {#int-iv-s2-prop-5 .statement}

*The complement of the support $ S $ of $ \mu $ is the largest negligible open set in $ X $.*

For, by Prop. 3, in order that an open set $ G $ be negligible, it is necessary and sufficient that $ G \cap S = \varnothing $, that is, $ G \subset \mathbf{C}S $.

### 3. Properties true almost everywhere

Let $ X $ be a locally compact space, $ \mu $ a measure on $ X $. If $ P\{x\} $ is a property, the property « $ P\{x\} $ almost everywhere (with respect to $ \mu $) » is by definition equivalent to the property « *the set of x such that* $ (x \in X \text{ and not } P\{x\}) $ *is $ \mu $*-negligible ».

#### Theorem 1 {#int-iv-s2-thm-1 .statement}

— In order that a numerical function (finite or not) $ f \geqslant 0 $ defined on $ X $ be negligible, it is necessary and sufficient that $ f(x) = 0 $ almost everywhere.

The condition is necessary. For, suppose that $ f $ is negligible, and let $ N $ be the set of $ x \in X $ such that $ f(x) \neq 0 $; then $ \varphi_N \leqslant \sup_n (n f) $, therefore $ \varphi_N $ is negligible (No. 1, Props. 1 and 2).

The condition is sufficient. Suppose that the set $ N $ of points where $ f(x) \neq 0 $ is negligible; then $ f \leqslant \sup_n n \varphi_N $, therefore $ f $ is negligible (No. 1, Props. 1 and 2).

#### Proposition 6 {#int-iv-s2-prop-6 .statement}

— If $ f $ and $ g $ are two functions $ \geqslant 0 $ (finite or not) defined on $ X $ such that $ f(x) = g(x) $ almost everywhere, then $ |\mu|^*(f) = |\mu|^*(g) $.

Let $ N $ be the negligible set of points $ x \in X $ such that $ f(x) \neq g(x) $. The functions $ \inf(f, g) $ and $ \sup(f, g) $ being equal except at the points of $ N $, it suffices to prove the proposition assuming $ f \leqslant g $. Let $ h $ be the function equal to $ +\infty $ at the points of $ N $, and to 0 on $ CN $; then $ f \leqslant g \leqslant f + h $, thus

$$
|\mu|^*(f) \leqslant |\mu|^*(g) \leqslant |\mu|^*(f + h) \leqslant |\mu|^*(f) + |\mu|^*(h) = |\mu|^*(f)
$$

(since $ h $ is negligible), whence the proposition.

#### Proposition 7 {#int-iv-s2-prop-7 .statement}

— If $ f $ is a function $ \geqslant 0 $ defined on $ X $ such that $ |\mu|^*(f) < +\infty $, then $ f(x) $ is finite almost everywhere.

For, let $ N $ be the set of points $ x \in X $ such that $ f(x) = +\infty $; for every integer $ n $, $ n \varphi_N \leqslant f $, whence $ n |\mu|^*(\varphi_N) \leqslant |\mu|^*(f) $; since $ n $ is arbitrarily large, $ |\mu|^*(N) = 0 $.

However, even if $ X $ is compact, a function $ f \geqslant 0 $ defined on $ X $ and everywhere finite can have infinite upper integral, as is shown by the example $ X = [0, 1] $, $ f(x) = 1/x $ for $ x > 0 $ and $ f(0) = 0 $, $ \mu $ being Lebesgue measure on $ X $.

### 4. Classes of equivalent functions

Let $ \mu $ be a measure on a locally compact space $ X $. Given a set $ F $, two mappings $ f, g $ of $ X $ into $ F $ are said to be *equivalent with respect to* $ \mu $ (or $ \mu $-*equivalent*, or simply *equivalent* if no confusion can arise) if $ f(x) = g(x) $ *almost everywhere* in $ X $. Since the union of two negligible sets is negligible, one indeed defines in this way an equivalence relation in the set $ F^X $ of all mappings of $ X $ into $ F $; when we speak of the *equivalence class* of such a function $ f $ (without further specification) it will be understood to be the class of all the functions equal almost everywhere to $ f $; in this chapter and those that follow, we will indicate this class by the notation $ \tilde{f} $.

#### Proposition 8 {#int-iv-s2-prop-8 .statement}

*Let* $(F_n)$ *be a countable family (finite or infinite) of sets. For every index n, let* $f_n, g_n$ *be two equivalent mappings of X into* $F_n$; *then, there exists a negligible set H such that, for every* $x \notin H$, $f_n(x) = g_n(x)$ *for all n*.

For, the set $H_n$ of $x \in X$ such that $f_n(x) \neq g_n(x)$ is negligible, therefore so is their union H (No. 2, Prop. 4), and this set meets the requirements.

#### Corollary {#int-iv-s2-n4-cor-1 .statement}

*If* $\varphi$ *is a mapping of* $\prod_n F_n$ *into a set G, then the mappings* $\varphi((f_n))$ *and* $\varphi((g_n))$ *of X into G are equivalent*.

We denote by $\varphi((\tilde{f}_n))$ the equivalence class of every function $\varphi((f_n))$, where $f_n$ is an arbitrary function in the class $\tilde{f}_n$.

In particular, if F is a *vector space* over $\mathbf{R}$, one defines $\tilde{f} + \tilde{g}$ and $\alpha \tilde{f}$ to be the equivalence classes of $f + g$ and $\alpha f$, respectively ($f$ and $g$ being mappings of X into F, and $\alpha$ a scalar); we obtain in this way, on the set of equivalence classes of mappings of X into F, a *vector space* structure: moreover, this is the *quotient space* structure of that of $F^X$ by the linear subspace of mappings $f$ such that $\tilde{f} = \tilde{0}$ (the functions that are zero almost everywhere), which we also call *negligible* functions (with values in F). One defines similarly the product $\tilde{g} \tilde{f}$, where $\tilde{f}$ is an equivalence class of mappings of X into F, and $\tilde{g}$ is an equivalence class of (finite) numerical functions defined on X: the set of equivalence classes of mappings of X into F is thus equipped with the structure of a *module* over the set of equivalence classes of finite numerical functions defined on X (which is itself equipped with a *ring* structure). If F is an *algebra* over $\mathbf{R}$, one defines similarly an algebra structure on the set of equivalence classes of mappings of X into F.

Let F be a *metrizable* topological space, and consider a uniform structure on F compatible with its topology and defined by a *countable* family of pseudometrics $\rho_n$ (GT, IX, §§1 and 2); in order that two mappings $f, g$ of X into F be equivalent, it is necessary and sufficient that the numerical functions $\rho_n(f, g)$ be *negligible*; for, this is equivalent to saying that there exists a negligible set H in X such that, for every $x \notin H$, $\rho_n(f(x), g(x)) = 0$ for all $n$, that is, $f(x) = g(x)$. In particular, if F is a metrizable locally convex space, and $(q_n)$ is a countable family of seminorms defining the topology of F (TVS, II, §4, No. 1), in order that two mappings $f, g$ of X into F be equivalent it is necessary and sufficient that all of the numerical functions $q_n(f(x) - g(x))$ be negligible.

#### Proposition 9 {#int-iv-s2-prop-9 .statement}

— Let $ f $ and $ g $ be two continuous mappings of $ X $ into a Hausdorff topological space $ F $; for $ f $ and $ g $ to be equivalent, it is necessary and sufficient that $ f(x) = g(x) $ at every point of the support of $ \mu $.

For, the set of $ x \in X $ such that $ f(x) \neq g(x) $ is an open set (GT, I, §8, No. 1); for it to be negligible, it is necessary and sufficient that it not intersect the support of $ \mu $ (No. 2, Prop. 5).

#### Proposition 10 {#int-iv-s2-prop-10 .statement}

— Let $ F $ be a Hausdorff locally convex space over $ \mathbf{R} $ such that there exists in the dual $ F' $ of $ F $ a sequence $ (a'_n) $ that is dense for the weak topology $ \sigma(F', F) $ (TVS, II, §6, No. 2). In order that two mappings $ f, g $ of $ X $ into $ F $ be equivalent, it is necessary and sufficient that, for every $ n $, the numerical functions $ \langle f(x), a'_n \rangle $ and $ \langle g(x), a'_n \rangle $ be equivalent.

The condition is obviously necessary. Conversely, if it is satisfied, there exists a negligible set $ H $ such that, for each $ x \notin H $, $ \langle f(x), a'_n \rangle = \langle g(x), a'_n \rangle $ for every $ n $; this means that the weakly continuous linear forms $ z' \mapsto \langle f(x), z' \rangle $ and $ z' \mapsto \langle g(x), z' \rangle $ on $ F' $ are equal at each of the points $ a'_n $, hence are identical by virtue of the hypothesis, which proves that $ f(x) = g(x) $ for all $ x \notin H $.

Note that the hypothesis of Prop. 10 is applicable in particular when $ F $ is a locally convex space that is metrizable and separable¹ (TVS, III, §3, No. 4, Cor. 2 of Prop. 6).

### 5. Functions defined almost everywhere

In conformity with the definition in No. 3, a mapping $ f $ of a subset $ A $ of $ X $ into a set $ F $ is said to be defined almost everywhere if the complement of the set $ A $ on which it is defined is a negligible set. We again call equivalence class of $ f $, and denote by $ \tilde{f} $, the equivalence class of every function defined on all of $ X $ and equal to $ f(x) $ at the points $ x \in X $ where $ f $ is defined; it is clear that this class depends only on $ f $. Two functions $ f, g $ defined almost everywhere are again said to be equivalent if $ \tilde{f} = \tilde{g} $: this means, therefore, that the set of points where $ f(x) $ and $ g(x) $ are both defined and equal has negligible complement.

It follows at once that Prop. 8 of No. 4 and its corollary may be generalized to the case where in their statements it is assumed only that each of the functions $ f_n, g_n $ is defined almost everywhere; then the functions $ \varphi((f_n)) $

¹ The original is de type dénombrable, also translated as 'of countable type' (GT, IX, §2, No. 8, Def. 4) or 'second countable', or 'satisfying the second axiom of countability'. In the corollary cited here from TVS, the term 'satisfying the first axiom of countability' should be replaced by one of the foregoing terms.

and $ \varphi((g_n)) $ are themselves defined almost everywhere; the equivalence class of $ \varphi((f_n)) $ is again $ \varphi((\tilde{f}_n)) $.

A function defined almost everywhere, with values in a vector space F, is again said to be *negligible* if it is equivalent to 0. If f is a negligible function with values in F, and u is a linear mapping of F into a vector space G, then the composite function $ u \circ f $ (defined almost everywhere) is negligible; similarly, for every (finite) numerical function g, defined almost everywhere, the function $ gf $ (defined almost everywhere) is negligible.

One must take care to observe that, in the set of functions with values in F and defined almost everywhere, the internal law of composition $ (f, g) \mapsto f + g $ *is not a group law*, because, while the function 0 is indeed a neutral element for this law, if f is not everywhere defined then there does not exist a function g such that $ f + g = 0 $. This is what motivates the introduction of the equivalence classes $ \tilde{f} $, which do form a vector space.

Let $ (f_n) $ be a sequence of mappings into a *topological space* F, each of which is defined almost everywhere in X. We say that the sequence $ (f_n) $ *converges (pointwise) almost everywhere to f in* X if the set of points $ x \in X $ where all the $ f_n(x) $ are defined and the sequence $ (f_n(x)) $ has a limit equal to $ f(x) $, has negligible complement. It is clear that if, for each n, the function $ g_n $ (defined almost everywhere) is equivalent to $ f_n $, then the sequence $ (g_n) $ converges almost everywhere to $ f $.

If F is *topological vector space*, one defines similarly an *almost everywhere convergent series*, whose general term is a function $ f_n $ defined almost everywhere in X with values in F; the sum of this series is a function defined at the points where the partial sums $ \sum_{k=1}^n f_k(x) $ are defined and have a limit, and its class depends only on the classes $ \tilde{f}_n $.

### 6. Equivalence classes of functions with values in $ \overline{\mathbf{R}} $

In conformity with the definition in No. 3, we say that a function $ f $, defined almost everywhere in X and with values in $ \overline{\mathbf{R}} $, is *finite almost everywhere* if the set of $ x \in X $ for which $ f(x) $ is defined and finite has negligible complement. A function that is finite almost everywhere is equivalent to a function that is *everywhere finite*; one can therefore identify its class $ \tilde{f} $ with a class of *finite* numerical functions defined on X (or almost everywhere in X). In particular, the sum and product of two classes of functions finite almost everywhere are defined, and the set of these classes is an *algebra* over $ \mathbf{R} $. If $ (f_n) $ is a sequence of functions with values in $ \overline{\mathbf{R}} $, defined and finite almost everywhere, then the partial sums $ \sum_{k=1}^n f_k(x) $ are defined almost everywhere; if, for almost every $ x \in X $, they have a limit $ f(x) $ in $ \overline{\mathbf{R}} $, we again say that the series with general term $ f_n $ converges almost everywhere and that $ f $ is the sum of the series (note that $ f $ is not necessarily finite almost everywhere).

If $ f $ and $ g $ are two numerical functions defined and finite almost everywhere in $ X $, then $ \tilde{f} + \tilde{g} $ (resp. $ \tilde{f} \tilde{g} $) is the class of every function equal to $ f(x) + g(x) $ (resp. $ f(x)g(x) $) at the points $ x \in X $ where this expression has meaning. Note that $ f $ and $ g $ can both be *everywhere defined* without $ f(x) + g(x) $ (resp. $ f(x)g(x) $) being defined for all $ x $ (GT, IV, §4, No. 3); by definition $ f + g $ (resp. $ fg $) is then the function equal to $ f(x) + g(x) $ (resp. $ f(x)g(x) $) at the points where this expression is defined; it is therefore only defined almost everywhere.

Let $ f $ and $ g $ be two numerical functions (finite or not) defined almost everywhere in $ X $ and such that $ f(x) \leq g(x) $ almost everywhere; if $ f_1 $ is equivalent to $ f $, and $ g_1 $ is equivalent to $ g $, it is clear that also $ f_1(x) \leq g_1(x) $ almost everywhere. The relation in question therefore depends only on the classes of $ f $ and $ g $; one writes $ \tilde{f} \leq \tilde{g} $, and one verifies immediately that this relation is an *order relation* in the set of equivalence classes of functions with values in $ \overline{\mathbf{R}} $. If $ (\tilde{f}_n) $ is a countable family (finite or infinite) of such classes and if, for every $ n $, $ f_n $ and $ g_n $ are two functions defined almost everywhere and belonging to the class $ \tilde{f}_n $, it follows from Prop. 8 of No. 4 that the functions $ \sup_n f_n $ and $ \sup_n g_n $, defined almost everywhere, are equivalent; their class therefore depends only on the classes $ \tilde{f}_n $, and one verifies at once that it is the *supremum* $ \sup_n \tilde{f}_n $ of these classes in the set of classes of functions with values in $ \overline{\mathbf{R}} $, ordered in the way just described (a set which is therefore, in particular, *lattice-ordered*). One shows similarly the existence of the infimum $ \inf_n \tilde{f}_n $, and one has $ \inf_n \tilde{f}_n = -\sup_n (-\tilde{f}_n) $. It follows that $ \limsup_{n \to \infty} f_n $ and $ \limsup_{n \to \infty} g_n $ are also equivalent, and their class, which is denoted $ \limsup_{n \to \infty} \tilde{f}_n $, is equal to $ \inf_n (\sup_{p \geq 0} \tilde{f}_{n+p}) $; $ \liminf_{n \to \infty} \tilde{f}_n $ is defined similarly.

A numerical function $ f $ (finite or not) is said to be *negligible* if it is equivalent to 0; this definition is equivalent to Def. 1 for functions that are positive and everywhere defined, by virtue of Th. 1. For $ f $ to be negligible, it is necessary and sufficient that $ |f| $ be negligible (or that both $ f^+ $ and $ f^- $ be negligible).
