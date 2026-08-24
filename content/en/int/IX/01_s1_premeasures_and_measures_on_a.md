---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 1
section_title: Premeasures and measures on a topological space
lang: en
source: int-vii-ix
pdf_pages: 0183-0204, 0288-0289
extraction: ocr
subsections:
    - "no": 1
      title: Encumbrances
      page: 0
      pdf_page: 183
    - "no": 2
      title: Premeasures and measures
      page: 3
      pdf_page: 185
    - "no": 3
      title: Examples of measures
      page: 6
      pdf_page: 188
    - "no": 4
      title: Locally negligible sets and functions
      page: 8
      pdf_page: 190
    - "no": 5
      title: Measurable sets and functions
      page: 9
      pdf_page: 191
    - "no": 6
      title: Directed families; support of a measure
      page: 11
      pdf_page: 193
    - "no": 7
      title: Upper envelopes and sums of measures
      page: 12
      pdf_page: 194
    - "no": 8
      title: Crushings
      page: 13
      pdf_page: 195
    - "no": 9
      title: Upper integral
      page: 17
      pdf_page: 199
    - "no": 10
      title: Integration theory
      page: 20
      pdf_page: 202
statements: 52
exercises: 10
content_sha256: 09dfd62372172bb0f417cdcb29ddcb19df14c593ed44b869e32a2b25b4cf5f72
---

## § 1. PREMEASURES AND MEASURES ON A TOPOLOGICAL SPACE

### 1. Encumbrances

#### Definition 1 {#int-ix-s1-def-1 .statement}

— Let T be a set. One calls encumbrance on T any mapping p of $ \mathcal{F}_+(T) $ into $ \overline{\mathbf{R}}_+ $ that has the following properties:
a) If f and g are two elements of $ \mathcal{F}_+ $ such that $ f \leq g $, then $ p(f) \leq p(g) $.
b) If f is an element of $ \mathcal{F}_+ $, and t is a number $ \geq 0 $, then $ p(tf) = tp(f) $.

c) *If f and g are two elements of $ \mathcal{F}_+ $, then $ p(f + g) \leq p(f) + p(g) $.*
d) *If $ (f_n) $ is an increasing sequence of elements of $ \mathcal{F}_+ $, and if $ f = \lim_{n \to \infty} f_n $, then $ p(f) = \lim_{n \to \infty} p(f_n) $.*
*If A is a subset of T, we write $ p(A) $ instead of $ p(\varphi_A) $.*

The condition b) implies that $ p(0) = 0 $. On the other hand, let $ (f_n) $ be a sequence of elements of $ \mathcal{F}_+ $; the conditions c) and d) imply the inequality

$$
p\left( \sum_n f_n \right) \leq \sum_n p(f_n)
$$

(the *inequality of countable convexity*).

For example, let T be a locally compact space, $ \mu $ a positive measure on T; then $ \mu^* $ and $ \mu^\bullet $ are encumbrances on T. This follows from Props. 10, 11, 12 and Th. 3 of Ch. IV, §1, No. 3 for $ \mu^* $, and from Prop. 1 of Ch. V, §1, No. 1 for $ \mu^\bullet $.

#### Proposition 1 {#int-ix-s1-prop-1 .statement}

*Let $ (p_\alpha)_{\alpha \in A} $ be a family of encumbrances on T. The sum and upper envelope of the family $ (p_\alpha) $ (in $ \mathcal{F}_+(\mathcal{F}_+(T)) $) are then encumbrances.*

The sum of a finite family of encumbrances obviously being an encumbrance, it suffices to treat the case of the upper envelope. The properties a), b), c) of Definition 1 being obviously satisfied, it remains to establish d). Set $ p = \sup_\alpha p_\alpha $; then, with the notations of Definition 1 d),

$$
p(f) = \sup_\alpha p_\alpha(f) = \sup_\alpha \sup_n p_\alpha(f_n) = \sup_n \sup_\alpha p_\alpha(f_n) = \sup_n p(f_n).
$$

#### Definition 2 {#int-ix-s1-def-2 .statement}

*Let p be an encumbrance on a set T. One says that p is bounded if $ p(T) < +\infty $. If T is a topological space, p is said to be locally bounded provided that every $ x \in T $ admits a neighborhood V such that $ p(V) < +\infty $.*

It then follows from the properties a) and c) of Def. 1 that $ p(K) < +\infty $ for every compact subset K of T. In particular, if T is compact, then every locally bounded encumbrance on T is bounded.

Let p be an encumbrance on a set T, and A a subset of T. For every function $ f \in \mathcal{F}_+(A) $, let $ f^0 $ be the extension by 0 of f to T; the mapping $ f \mapsto p(f^0) $ on $ \mathcal{F}_+(A) $ is then an encumbrance, called *the encumbrance induced by p* on A, and is denoted $ p|A $ or $ p_A $.

Let T and U be two sets, $ \pi $ a mapping of T into U, and p an encumbrance on T. The encumbrance $ \pi(p) $ on U, whose value for $ f \in \mathcal{F}_+(U) $ is given by

$$
(\pi(p))(f) = p(f \circ \pi),
$$

is called the *image encumbrance* of $ p $ under $ \pi $.

Let $ p $ be an encumbrance on a set $ T $; $ p $ is said to be *concentrated* on a subset $ A $ of $ T $ if $ p(T - A) = 0 $.

#### Lemma 1 {#int-ix-s1-lem-1 .statement}

— *If the encumbrance $ p $ is concentrated on $ A \subset T $, then $ p(f) = p(f \varphi_A) $ for every $ f \in \mathcal{F}_+(T) $.*

For, set $ T - A = B $, so that $ p(\varphi_B) = 0 $; then

$$
f \varphi_B \leq (+\infty) \cdot \varphi_B = \sup_{n \in \mathbf{N}} n \varphi_B,
$$

therefore $ p(f \varphi_B) = 0 $ by properties $ a), b), d) $ of Def. 1. It follows from $ c) $ that $ p(f) \leq p(f \varphi_A) + p(f \varphi_B) = p(f \varphi_A) $, and finally $ p(f) = p(f \varphi_A) $ by $ a) $.

### 2. Premeasures and measures

Let $ T $ be a topological space, and let $ \mathfrak{K} $ be the set of compact subsets of $ T $, ordered by inclusion. For every $ K \in \mathfrak{K} $, let $ \mathcal{M}(K; \mathbf{C}) $ be the set of complex measures on $ K $. For every pair $ (K, L) $ of elements of $ \mathfrak{K} $ such that $ K \subset L $, let $ \iota_{KL} $ be the mapping of $ \mathcal{M}(L; \mathbf{C}) $ into $ \mathcal{M}(K; \mathbf{C}) $ that associates to each measure $ \mu $ on $ L $ the measure $ \mu_K $ induced by $ \mu $ on $ K $ (Ch. IV, §5, No. 7, Def. 4). Then $ \iota_{KM} = \iota_{KL} \circ \iota_{LM} $ when $ K, L $ and $ M $ are compact subsets of $ T $ such that $ K \subset L \subset M $; this follows from the transitivity of induced measures (Ch. V, §7, No. 2, Prop. 4). The elements of the *inverse limit* of the family $ (\mathcal{M}(K; \mathbf{C}))_{K \in \mathfrak{K}} $ for the mappings $ \iota_{KL} $ will be called *premeasures* on $ T $. In other words:

#### Definition 3 {#int-ix-s1-def-3 .statement}

*One calls premeasure on a topological space $ T $ every mapping $ w $ that associates, to every compact subset $ K $ of $ T $, a measure $ w_K $ on $ K $, and that has the following property:

*If $ K $ and $ L $ are compact subsets of $ T $ such that $ K \subset L $, the measure $ (w_L)_K $ induced by $ w_L $ on $ K $ is equal to $ w_K $.

The premeasure $ w $ is said to be real (resp. positive) if all of the measures $ w_K $ are real (resp. positive).*

Let $ w $ and $ w' $ be two premeasures on $ T $, $ t $ a complex number; the premeasures $ w + w' $ and $ tw $ are defined by the formulas $ (w + w')_K = w_K + w'_K $, $ (tw)_K = tw_K $ for every compact subset $ K $ of $ T $. The premeasures on $ T $ obviously form a vector space, which is denoted $ \mathcal{P}(T; \mathbf{C}) $; the space of real premeasures will be denoted $ \mathcal{P}(T; \mathbf{R}) $, or more often $ \mathcal{P}(T) $, and the convex cone of positive premeasures will be denoted $ \mathcal{P}_+(T) $. Let $ w $ be a premeasure; the mapping $ K \mapsto |w_K| $ is then a premeasure on $ T $ (Ch. IV, §5, No. 7, Lemma 3), which will be denoted $ |w| $. If $ w $ is real, one sets w^+ = \frac{1}{2}(|w| + w),\ w^- = \frac{1}{2}(|w| - w); these two premeasures being positive, one sees that every real premeasure is the difference of two positive premeasures. Clearly $(w^+)_K = (w_K)^+$, $(w^-)_K = (w_K)^-$ for every compact subset K of T.

The vector space $P(T)$ is ordered by the cone $P_+(T)$. It is clear that $w^+ = \sup(w, 0),\ w^- = \sup(-w, 0)$; consequently, $P(T)$ is lattice-ordered and $\sup(w, w') = w + (w' - w)^+,\ \inf(w, w') = w - (w' - w)^-$. Moreover, clearly

$$
(\sup(w, w'))_K = \sup(w_K, w'_K),\quad (\inf(w, w'))_K = \inf(w_K, w'_K)
$$

for every compact subset K of T.

#### Definition 4 {#int-ix-s1-def-4 .statement}

*Let w be a positive premeasure on T. We shall set, for every function $f \in \mathcal{F}_+(T)$,*

$$(1)$$
$$
w^\bullet(f) = \sup_K (w_K)^\bullet(f_K),
$$

*where K runs over the set of compact subsets of T.*

For each compact set K, let $p^K$ be the image encumbrance of the encumbrance $(w_K)^\bullet$ under the canonical injection of K into T; $w^\bullet$ is the upper envelope of the encumbrances $p^K$, hence is an encumbrance (No. 1, Prop. 1). One says that $w^\bullet$ is the *essential upper integral* associated with the positive premeasure w. One often writes $\int^\bullet f\, dw$ or $\int^\bullet f(t)\, dw(t)$ instead of $w^\bullet(f)$.

*Remark 1).* — If v and w are two positive premeasures, then $(v + w)^\bullet = v^\bullet + w^\bullet$ (Ch. V, §1, No. 1, Prop. 3). If v and w are two complex premeasures, then $|v + w|^\bullet \leq |v|^\bullet + |w|^\bullet$.

#### Proposition 2 {#int-ix-s1-prop-2 .statement}

*a) Let w be a positive premeasure. For every compact subset K of T, the encumbrance $(w^\bullet)_K$ induced by $w^\bullet$ on K is equal to $(w_K)^\bullet$. For every function $f \in \mathcal{F}_+(T)$, one has the relations $(w_K)^\bullet(f_K) = w^\bullet(f_{\varphi_K})$ and*

$$(2)$$
$$
w^\bullet(f) = \sup_K w^\bullet(f_{\varphi_K}).
$$

*b) Conversely, let p be an encumbrance on T satisfying the following conditions:
1) For every compact subset K of T, there exists a positive measure $w_K$ on K such that $p_K = (w_K)^\bullet$.
2) For every function $f \in \mathcal{F}_+(T)$, $p(f) = \sup_K p(f_{\varphi_K})$.
The mapping $w : K \mapsto w_K$ is then a positive premeasure on T, and $p = w^\bullet$.

Let us prove $a$: let $g \in \mathcal{F}_+(K)$ and let $g^0$ be the extension by zero of $g$ to $T$; then, by the definition of induced encumbrances,

$$
(w^\bullet)_K(g) = w^\bullet(g^0) = \sup_L (w_L)^\bullet(g^0|L),
$$

where $L$ runs over the set of compact subsets of $T$, or merely the set of those that contain $K$. But if $L$ contains $K$, then $(w_L)^\bullet(g^0|L) = (w_K)^\bullet(g)$ from the fact that $g^0|L$ is zero outside $K$ (Ch. V, §7, No. 1, Prop. 1), which proves the first assertion. Therefore

$$
(w_K)^\bullet(f_K) = (w^\bullet)_K(f_K) = w^\bullet((f_K)^0) = w^\bullet(f_{\varphi_K})
$$

for all $f \in \mathcal{F}_+(T)$, and (2) merely translates the formula (1).

Let us pass to $b$: the measure $w_K$ considered in 1) is unique (Ch. V, §1, No. 1). Let us show that the mapping $K \mapsto w_K$ is a premeasure: let $K$ and $L$ be two compact subsets such that $K \subset L$, and let $\lambda$ be the measure induced by $w_L$ on $K$; everything comes down to showing that $\lambda^\bullet = (w_K)^\bullet$. Now, $\lambda^\bullet = ((w_L)^\bullet)_K$ (Ch. V, §7, No. 1, Prop. 1); since $(w_L)^\bullet = p_L$, we have $\lambda^\bullet = (p_L)_K = p_K = (w_K)^\bullet$.

Let us denote by $w$ the premeasure $K \mapsto w_K$; since $p_K = (w_K)^\bullet = (w^\bullet)_K$, we have $p(f_{\varphi_K}) = p_K(f_K) = (w^\bullet)_K(f_K) = w^\bullet(f_{\varphi_K})$. The two encumbrances $p$ and $w^\bullet$ are therefore equal by virtue of the formula (2) and the hypothesis 2) on $p$.

Q.E.D.

Since the induced encumbrance $(w^\bullet)_K$ is equal to $(w_K)^\bullet$, there is no ambiguity in simply writing $w_K^\bullet$. We shall employ this notation from now on.

#### Corollary {#int-ix-s1-n2-cor-1 .statement}

— *Let $v$ and $w$ be two positive premeasures on $T$, such that $v^\bullet(L) = w^\bullet(L)$ for every compact subset $L$ of $T$; then $v = w$. In particular, the relation $v^\bullet = w^\bullet$ implies $v = w$*.

For, let $K$ be a compact set in $T$; for every compact set $L \subset K$, one has the relation

$$
w_K(L) = w_K^\bullet(L) = w^\bullet(L) = v^\bullet(L) = v_K^\bullet(L) = v_K(L)
$$

by Prop. 2; therefore $w_K = v_K$ (Ch. IV, §4, No. 10, Cor. 3 of Prop. 19), and finally $w = v$ by the definition of premeasures.

#### Definition 5 {#int-ix-s1-def-5 .statement}

— *Let $w$ be a premeasure on a topological space $T$. One says that $w$ is a measure (resp. a bounded measure) if the encumbrance $|w|^\bullet$ is locally bounded (resp. bounded) (cf. No. 1, Def. 2)*.

The set of complex measures on $T$ is obviously a vector space (*Remark* 1), which will be denoted $\mathcal{M}(T; \mathbf{C})$. The space of real measures will be denoted $ \mathcal{M}(T; \mathbf{R}) $ or more often $ \mathcal{M}(T) $, and the cone of positive measures will be denoted $ \mathcal{M}_+(T) $.

If $ w $ is a complex measure, its real part and its imaginary part are real measures. If $ w $ is a real measure, $ w^+ $ and $ w^- $ are positive measures. Every complex (resp. real) measure is thus a linear combination (resp. difference) of positive measures.

#### Remark 2 {#int-ix-s1-n2-rem-2 .statement}

If $ T $ is *locally compact*, then every premeasure $ w $ on $ T $ is a measure. For, every $ x \in T $ admits a compact neighborhood $ K $, and $ |w|^*(K) = \|w_K\| < +\infty $, so that the encumbrance $ |w|^* $ is locally bounded.

#### Remark 3 {#int-ix-s1-n2-rem-3 .statement}

For every Borel subset $ A $ of $ T $ (in particular for $ A = T $) and every positive measure $ \mu $ on $ T $, the number $ \mu^*(A) $ is the supremum of the measures $ \mu^*(K) $ of the compact subsets of $ A $. Indeed, for every compact subset $ K $ of $ A $, one has $ \mu^*(K) \leq \mu^*(A) $; on the other hand, if $ \mathfrak{K} $ is the set of compact subsets of $ T $, then

$$
\mu^*(A) = \sup_{K \in \mathfrak{K}} \mu_K^*(A \cap K) = \sup_{K \in \mathfrak{K}} \sup_{L \in \mathfrak{K}, L \subset A \cap K} \mu_K^*(L) \leq \sup_{L \in \mathfrak{K}, L \subset A} \mu^*(L)
$$

by Cor. 1 of Th. 4 of Ch. IV, §4, No. 6.

### 3. Examples of measures

#### Example 1 {#int-ix-s1-n3-exa-1 .statement}

— *Measures on a locally compact space.*

The following proposition shows that the theory of this chapter contains that of Ch. IV. In the statement, the word 'measure' and the notation $ \mathcal{M}(T; \mathbf{C}) $ are taken in the sense of the earlier chapters.

#### Proposition 3 {#int-ix-s1-prop-3 .statement}

*Let $ T $ be a locally compact space, and let $ \mu $ be a measure on $ T $. Denote by $ W(\mu) $ the mapping that associates to each compact subset $ K $ of $ T $ the induced measure $ \mu_K $. Then $ W(\mu) $ is a premeasure on $ T $, one has $ W(|\mu|) = |W(\mu)| $, and the linear mapping $ W : \mu \mapsto W(\mu) $ is a bijection of the space $ \mathcal{M}(T; \mathbf{C}) $ onto the space $ \mathcal{P}(T; \mathbf{C}) $ of premeasures on $ T $. Moreover, if $ \mu $ is positive then $ \mu^* = (W(\mu))^* $.

It is clear that $ W(\mu) $ is a premeasure (Ch. V, §7, No. 2, Prop. 4) and that the mapping $ W $ is linear. The relation $ W(\mu) = 0 $ means that $ \mu $ induces the measure 0 on every compact set in $ T $; then $ \mu(f) = 0 $ for $ f \in \mathcal{H}(T; \mathbf{C}) $, thus $ \mu = 0 $, which proves that $ W $ is injective. It remains to prove that $ W $ is surjective. Since every premeasure is a linear combination of positive premeasures, it will suffice to construct, for every *positive* premeasure $ w $, a positive measure $ \mu $ such that $ w = W(\mu) $. Let $ f \in \mathcal{H}(T) $ be a given function, and let $ L $ be a compact set containing the support of $ f $; the number $ w_L(f_L) $ is independent of the choice of $ L $, by the definition of induced measures, so that one can set $ \mu(f) = w_L(f_L) $; then $ \mu $ is a positive linear form on $ \mathcal{H}(T) $, that is, a positive measure. Let us verify that $ w = W(\mu) $; first, the relation $ \mu^\bullet(f) = w_L^\bullet(f_L) $ extends to the case that $ f $ is a finite upper semi-continuous function that is positive and is zero outside $ L $. For, let $ M $ be a compact neighborhood of $ L $, and $ \mathcal{H} $ the (decreasing directed) set of continuous functions on $ T $, with support contained in $ M $, that are $ \geq f $. Then (Ch. IV, §4, No. 4, Cor. 2 of Prop. 5)

$$
\mu^\bullet(f) = \inf_{h \in \mathcal{H}} \mu(h) = \inf_{h \in \mathcal{H}} w_M(h_M) = w_M^\bullet(f_M),
$$

and on the other hand $ w_M^\bullet(f_M) = w_L^\bullet(f_L) $ since $ f_M $ is zero on $ M - L $ (Ch. V, §7, No. 1, Prop. 1). In particular, if $ f $ is taken to be the extension by 0 of an element of $ \mathcal{H}_+(L) $, this formula shows that $ \mu_L = w_L $ by the definition of induced measures, thus indeed $ W(\mu) = w $.

If $ \mu $ is positive, then

$$
\mu^\bullet(f) = \sup_K \mu^\bullet(f \varphi_K) = \sup_K \mu_K^\bullet(f_K) = (W(\mu))^\bullet(f)
$$

for every $ f \in \mathcal{F}_+(T) $ (Ch. V, §1, Def. 1 and §7, Prop. 1). The relation $ |W(\mu)| = W(|\mu|) $ is obvious (Ch. IV, §5, No. 7, Lemma 3).

Q.E.D.

When $ T $ is *locally compact*, we shall from now on *identify* the spaces $ \mathcal{M}(T; \mathbf{C}) $ and $ \mathcal{P}(T; \mathbf{C}) $ by means of the bijection $ W $.

#### Example 2 {#int-ix-s1-n3-exa-2 .statement}

— *Measures with compact support on a topological space.*

#### Lemma 2 {#int-ix-s1-lem-2 .statement}

— *Let $ T $ be a topological space, $ L $ a compact subset of $ T $, and $ \lambda $ a positive measure on $ L $. There exists a unique positive measure $ \mu $ on $ T $ such that, for every function $ f \in \mathcal{F}_+(T) $,*

(2)
$$
\mu^\bullet(f) = \lambda^\bullet(f_L).
$$

Let us set $ p(f) = \lambda^\bullet(f_L) $ for every $ f \in \mathcal{F}_+(T) $, and let us show that the conditions 1) and 2) of Prop. 2 *b*) are satisfied. The second is obviously satisfied: indeed, $ p(f) = p(f \varphi_K) $ if $ K $ contains $ L $. If $ K \subset T $ is compact, and if $ h \in \mathcal{F}_+(K) $, then

$$
p_K(h) = p(h^0) = \lambda^\bullet(h^0|L).
$$

But $ h^0|L $ is the extension by 0 of $ h_{K \cap L} $ to $ L $: the last expression is therefore equal to $ (\mu_K)^\bullet(h) $, where $ \mu_K $ is the image of $ \lambda|K \cap L $ under the injection of $ K \cap L $ into $ K $ (Ch. V, §6, No. 2, Prop. 2 and §7, No. 1, Prop. 1), and $ p_K = (\mu_K)^\bullet $. Condition 1) of Prop. 2 *b*) is therefore also satisfied, and the existence of $ \mu $ follows at once.

Q.E.D.

We shall say that $ \mu $ is the measure on T *defined* by $ \lambda $. In particular, for every point $ x $ of T one can define the measure $ \varepsilon_x $; it is characterized by $ (\varepsilon_x)^*(f) = f(x) $ for $ f \in \mathcal{F}_+(T) $.

#### Remark {#int-ix-s1-n3-rem-1 .statement}

— 1) When T is locally compact, $ \mu $ is the image of $ \lambda $ under the injection of L into T. We shall see in §2, No. 3, *Example*, when image measures will have been treated, that this interpretation remains valid for arbitrary spaces.
2) We shall also see that the measures defined in *Example* 2 are positive measures on T with compact support (No. 6, *Remark* 2)).

*We shall henceforth consider only positive measures, absent express mention to the contrary. For the rest of this section, T will denote a topological space and $ \mu $ a positive measure on T.*

Numerous results in the following subsections may be extended to positive premeasures. This extension is left to the reader.

### 4. Locally negligible sets and functions

#### Definition 6 {#int-ix-s1-def-6 .statement}

*A function* $ f \in \mathcal{F}_+ $ (resp. *a subset* A *of* T) *is said to be locally negligible for the measure* $ \mu $ *if* $ \mu^*(f) = 0 $ (resp. $ \mu^*(A) = 0 $). *One says that* $ \mu $ *is concentrated on a subset* A *of* T *if* T − A *is locally* $ \mu $*-negligible*.

#### Remark {#int-ix-s1-n4-rem-1 .statement}

— 1) The concepts so defined coincide, when T is locally compact, with the usual concepts.
2) After we have defined *negligible* sets, we will see that the locally negligible sets are indeed those whose germ, at every point of T, is the germ of a negligible set (No. 9, Cor. 2 of Prop. 14).
3) As in Chs. IV and V, the expression 'locally almost everywhere' will be synonymous with 'except on a locally negligible set'.
4) If $ \theta $ is a complex measure, we shall say that a function (resp. a subset of T) is locally negligible for $ \theta $ if it is so for the positive measure $ |\theta| $.

#### Example {#int-ix-s1-n4-exa-1 .statement}

— Let L be a compact subset of T, $ \lambda $ a measure on L, and $ \mu $ the measure on T defined by $ \lambda $ (No. 3, *Example* 2). The formula (3) implies at once that a function $ f \in \mathcal{F}_+(T) $ is locally $ \mu $-negligible if and only if $ f_L $ is $ \lambda $-negligible.

It follows immediately from formula (1) that a function $ f \in \mathcal{F}_+(T) $ is locally $ \mu $-negligible if and only if $ f_K $ is $ \mu_K $-negligible for every compact subset K of T. Thus the properties of locally negligible sets reduce at once to those of negligible sets in compact spaces, treated in Ch. IV. Here are some results that will be used henceforth without further reference.

— For a function $ f \geqslant 0 $ to be locally negligible, it is necessary and sufficient that $ f(t) = 0 $ locally almost everywhere (Ch. IV, §2, No. 3, Th. 1). If $ f $ is a function with values in a Banach space, it is therefore equivalent to say that $ f = 0 $ locally almost everywhere or that $ \mu^*(|f|) = 0 $; in this case we shall again say that $ f $ is locally negligible.

— The sum and upper envelope of a sequence of locally negligible functions $ \geqslant 0 $ are locally negligible (*loc. cit.*, No. 1, Prop. 2).

— If $ f $ and $ g $ are two functions $ \geqslant 0 $ that are equal locally almost everywhere, then $ \mu^\bullet(f) = \mu^\bullet(g) $ (*loc. cit.*, No. 3, Prop. 6).

### 5. Measurable sets and functions

#### Definition 7 {#int-ix-s1-def-7 .statement}

*A function* $ f $ *defined on* $ T $, *with values in a topological space* $ F $ (*Hausdorff or not*) *is said to be measurable for the measure* $ \mu $ *(or to be* $ \mu $*-measurable)* if, *for every compact subset* $ K $ *of* $ T $, *the function* $ f_K $ *is* $ \mu_K $*-measurable*.

This amounts to saying that there exists, for every compact set $ K $, a partition of $ K $ into a $ \mu_K $-negligible set $ N $ and a sequence $ (K_n) $ of compact sets, such that the restriction of $ f $ to each $ K_n $ is continuous. Since it is equivalent to say that $ N $ is $ \mu_K $-negligible or that it is locally $ \mu $-negligible (No. 4), one sees that $ f $ is $ \mu $-measurable if and only if, for every compact set $ K $, there exists a partition of $ K $ into a locally $ \mu $-negligible set $ N $ and a sequence $ (K_n) $ of compact sets such that $ f_{K_n} $ is continuous for all $ n $. This definition is identical to that of Def. 1 of Ch. IV, §5, No. 1, and one thus recovers the usual concept of measurable function when $ T $ is locally compact.

A subset $ A $ of $ T $ is said to be measurable if its characteristic function is measurable. When $ A $ is $ \mu $-measurable and $ \mu^\bullet(A) < +\infty $, this number is denoted simply $ \mu(A) $ and is called the *measure* of $ A $. One similarly writes $ \mu(f) $ for $ \mu^\bullet(f) $ when $ f $ is $ \geqslant 0 $, $ \mu $-measurable, and $ \mu^\bullet(f) < +\infty $.

If $ \theta $ is a complex measure on $ T $, a function $ f $ (resp. a subset of $ T $) is said to be $ \theta $-measurable if it is measurable for the positive measure $ |\theta| $. The results below may be extended to complex measures.

#### Example {#int-ix-s1-n5-exa-1 .statement}

— Let $ L $ be a compact subset of $ T $, $ \lambda $ a measure on $ L $, and $ \mu $ the measure on $ T $ defined by $ \lambda $ (No. 3, *Example 2*). A function $ f $ defined on $ T $ is $ \mu $-measurable if and only if $ f_L $ is $ \lambda $-measurable. For, this condition is obviously necessary. Conversely, if it is satisfied, there exists a partition of $ L $ into a $ \lambda $-negligible set $ N $ and a sequence $ (L_n) $ of compact sets, such that $ f_{L_n} $ is continuous for all $ n $. If $ K $ is a compact subset of $ T $, the set $ K - \bigcup^n (K \cap L_n) $ has an intersection with $ L $ that is $ \lambda $-negligible, hence this set is $ \mu $-negligible by formula (3) of No. 3, and the restriction of $ f $ to $ K \cap L_n $ is continuous for all $ n $.

Def. 7 permits extending, without a new proof, a number of results on measurable functions to the case of spaces not locally compact. Here are some of them, which we shall use henceforth without further reference: the open sets and the closed sets of $ T $ are $ \mu $-measurable; the $ \mu $-measurable sets form a tribe (Ch. IV, §5, No. 4, Cor. 2 of Th. 2), that contains the Borel sets of T (loc. cit., Cor. 3), and the Souslin sets (Ch. IV, §5, No. 1, Cor. 2 of Prop. 3)(1). The usual algebraic operations on numerical functions preserve measurability (Ch. IV, §5, No. 3), as do the operations of countable passage to the limit (loc. cit., No. 4, Th. 2 and Cor. 1). The following property merits more explicit mention:

#### Proposition 4 {#int-ix-s1-prop-4 .statement}

— Let $ f $ be a positive function and $ (g_n)_{n \geq 1} $ a sequence of $ \mu $-measurable positive functions on T. Setting $ g = \sum_{n \geq 1} g_n $, one has

$$
\mu^\bullet(fg) = \sum_{n \geq 1} \mu^\bullet(fg_n).
$$

Set $ h_n = \sum_{i=1}^n g_i $ for all $ n \geq 1 $. For every compact subset K of T,

$$
\mu_K^\bullet((fh_n)_K) = \sum_{i=1}^n \mu_K^\bullet((f g_i)_K)
$$

by Prop. 2 of Ch. V, §1, No. 1 applied to the compact space K. Passing to the limit with respect to the increasing directed set of compact subsets of T, one obtains

$$
\mu^\bullet(fh_n) = \sum_{i=1}^n \mu^\bullet(f g_i).
$$

Now, $ fg $ is the limit of the increasing sequence $ (fh_n)_{n \geq 1} $, whence $ \mu^\bullet(fg) = \lim_{n \to \infty} \mu^\bullet(fh_n) $; the preceding formula then immediately implies (4).

#### Corollary {#int-ix-s1-n5-cor-1 .statement}

— Let $ (A_n) $ be a sequence of pairwise disjoint measurable subsets, with union A. For every subset B of T,

$$
\mu^\bullet(A \cap B) = \sum_n \mu^\bullet(A_n \cap B)
$$

and in particular

$$
\mu^\bullet(A) = \sum_n \mu^\bullet(A_n).
$$

Among the properties of measurable functions or sets that extend as above to Hausdorff spaces, we cite also Prop. 12 of Ch. IV, §5, No. 8 ($ \mu $-dense families of compact sets). Thus, a function $ f $ with values in a topological

(1) The proof of this corollary is valid without modification for Souslin sets in a nonmetrizable locally compact space (GT, IX, §6, No. 9, Th. 5).

space (Hausdorff or not) is $ \mu $-measurable if and only if the set of compact subsets K of T, such that $ f_K $ is continuous, is $ \mu $-dense (*loc. cit.*, No. 10, Prop. 15).

### 6. Directed families; support of a measure

**Proposition 5. — a)** *Let H be an increasing directed set of functions $ \geqslant 0 $ that are lower semi-continuous on every compact subset of T. Then*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

*b)* *Let H be a decreasing directed set of functions $ \geqslant 0 $ that are upper semi-continuous on every compact subset of T. If there exists in H a function $ h_0 $ such that $ \mu^\bullet(h_0) < +\infty $, then*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

For every compact set $ K \subset T $, we have in case *a)*

$$
\mu^\bullet \left( \sup_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \sup_{h \in H} h_K \right) = \sup_{h \in H} \mu_K^\bullet(h_K) = \sup_{h \in H} \mu^\bullet(h \varphi_K),
$$

and in case *b)*

$$
\mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \inf_{h \in H} h_K \right) = \inf_{h \in H} \mu_K^\bullet(h_K) = \inf_{h \in H} \mu^\bullet(h \varphi_K),
$$

by Prop. 2 of No. 2, and Prop. 8 of Ch. V, §1, No. 2. Case *a*) follows at once, by passage to the supremum with respect to K (No. 2, Prop. 2). To treat case *b*), denote by $ \varepsilon $ a number $ > 0 $, and choose a compact set K such that $ \mu^\bullet(h_0 \varphi_K) \geqslant \mu^\bullet(h_0) - \varepsilon $. We then have (No. 5, Prop. 4) $ \mu^\bullet(h_0 \varphi_{C_K}) \leqslant \varepsilon $; for every function $ h \in H $ that is $ \leqslant h_0 $, we therefore have $ \mu^\bullet(h \varphi_{C_K}) \leqslant \varepsilon $, and finally $ \mu^\bullet(h \varphi_K) \geqslant \mu^\bullet(h) - \varepsilon $ by Prop. 4 of No. 5. Therefore

$$
\mu^\bullet \left( \inf_{h \in H} h \right) \geqslant \mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h \varphi_K) \geqslant \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h) - \varepsilon.
$$

Consequently the left side of (6) is $ \geqslant $ the right side; the reverse inequality being obvious, the proposition is established.

#### Corollary {#int-ix-s1-n6-cor-1 .statement}

— a) Let $(U_\alpha)_{\alpha \in I}$ be an increasing directed family of open subsets of $T$, with union $U$. Then $\mu^\bullet(U) = \sup_{\alpha \in I} \mu^\bullet(U_\alpha)$.

b) Let $(F_\alpha)_{\alpha \in I}$ be a decreasing directed family of closed subsets of $T$, with intersection $F$. If there exists an $\alpha \in I$ such that $\mu^\bullet(F_\alpha)$ is finite, then $\mu^\bullet(F) = \inf_{\alpha \in I} \mu^\bullet(F_\alpha)$.

By the preceding corollary, there exists a largest locally negligible open set; this justifies the following definition:

#### Definition 8 {#int-ix-s1-def-8 .statement}

— *The support of a measure $\mu$ on $T$ is defined to be the complement of the largest locally $\mu$-negligible open set in $T$*.

The support of $\mu$ is denoted $\operatorname{Supp}(\mu)$.

#### Remark 1 {#int-ix-s1-n6-rem-1 .statement}

If $\mu$ is a complex measure, the support of $\mu$ is defined to be the support of the positive measure $|\mu|$; it is again the complement of the largest locally $\mu$-negligible open set.

#### Remark 2 {#int-ix-s1-n6-rem-2 .statement}

Let us show that the measures introduced in *Example 2* of No. 3 are measures with compact support in $T$. Let $\mu$ be a positive measure on $T$ whose support is a compact set $K$, and let $\nu$ be the measure defined by $\mu_K$ (in the sense of No. 3). Let $f \in \mathcal{F}_+(T)$; then

$$
\nu^\bullet(f) = \mu_K^\bullet(f_K) \quad \text{(No. 3, formula (3))}.
$$

The encumbrance $\mu^\bullet$ being concentrated on $K$, we also have

$$
\mu^\bullet(f) = \mu^\bullet(f \varphi_K) = \mu^\bullet((f_K)^0) = \mu_K^\bullet(f_K),
$$

whence $\mu^\bullet = \nu^\bullet$, and finally $\mu = \nu$. Conversely, if $K$ is a compact set in $T$ and $\lambda$ a measure on $K$, and if $\mu$ is the measure on $T$ defined by $\lambda$, then $\mu^\bullet(\mathbf{C}K) = 0$ (No. 3, formula (3)); consequently, the support of $\mu$ is contained in $K$, hence is compact.

### 7. Upper envelopes and sums of measures

#### Proposition 6 {#int-ix-s1-prop-6 .statement}

— *Let $(\lambda_\alpha)_{\alpha \in A}$ be an increasing directed family of measures on $T$, and let $p = \sup_\alpha \lambda_\alpha^\bullet$. For the family $(\lambda_\alpha)$ to be bounded above in $\mathcal{M}(T)$, it is necessary and sufficient that the encumbrance $p$ be locally bounded. The family $(\lambda_\alpha)$ then admits a supremum $\lambda$ in $\mathcal{M}(T)$, and $\lambda^\bullet = p$. For every compact set $K$, the measure $\lambda_K$ is the supremum of the measures $(\lambda_\alpha)_K$ in $\mathcal{M}(K)$*.

If the family $(\lambda_\alpha)$ is bounded above in $\mathcal{M}(T)$, then $p$ is obviously locally bounded. Conversely, let us assume $p$ to be locally bounded, and let us show that it satisfies the conditions 1) and 2) of Prop. 2 b) of No. 2. For 2), this results from the following equalities:

$$
p(f) = \sup_\alpha \lambda_\alpha^\bullet(f) = \sup_\alpha \sup_K \lambda_\alpha^\bullet(f \varphi_K) = \sup_K \sup_\alpha \lambda_\alpha^\bullet(f \varphi_K) = \sup_K p(f \varphi_K).
$$

On the other hand, let K be a compact set; the encumbrance $ p_K $ is equal to the upper envelope of the encumbrances $ (\lambda_\alpha^\bullet)_K $ and it is bounded since $ p $ is locally bounded. The measures $ (\lambda_\alpha)_K $ therefore admit a supremum $ \lambda_K $ in $ \mathcal{M}(K) $, and $ \lambda_K^\bullet = p_K $ (Ch. V, §1, No. 4, Prop. 11). The condition 1) of Prop. 2 b) of No. 2 is thus satisfied, therefore there exists a measure $ \lambda $ on T such that $ \lambda^\bullet = p $; it is clear that $ \lambda $ is the supremum of the measures $ \lambda_\alpha $.

#### Definition 9 {#int-ix-s1-def-9 .statement}

*Let $ (\mu_i)_{i \in I} $ be a family of measures on T. Let A be the set of finite subsets of I; for every $ \alpha \in A $ let $ \lambda_\alpha = \sum_{i \in \alpha} \mu_i $. If the family $ (\lambda_\alpha) $ admits a supremum $ \mu $ in $ \mathcal{M}(T) $, the family $ (\mu_i) $ is said to be summable, $ \mu $ is called the sum of the family $ (\mu_i) $, and one writes $ \mu = \sum_{i \in I} \mu_i $.*

This definition extends the definition of Ch. V, §2, No. 1.

#### Proposition 7 {#int-ix-s1-prop-7 .statement}

*For the family $ (\mu_i)_{i \in I} $ to be summable, with sum $ \mu $, it is necessary and sufficient that the encumbrance $ p = \sum_{i \in I} \mu_i^\bullet $ be locally bounded, in which case $ p = \mu^\bullet $. For every compact subset K of T, the family $ ((\mu_i)_K)_{i \in I} $ is then summable in $ \mathcal{M}(K) $, and $ \mu_K = \sum_{i \in I} (\mu_i)_K $.*

With notations as in Def. 9, $ \lambda_\alpha^\bullet = \sum_{i \in \alpha} \mu_i^\bullet $ for every finite subset $ \alpha $ of I (No. 2, *Remark* 1). The statement is then an immediate consequence of Prop. 6.

The relation $ \mu_K = \sum_{i \in I} (\mu_i)_K $ and Prop. 2 of Ch. V, §2, No. 2 yields the following result:

#### Proposition 8 {#int-ix-s1-prop-8 .statement}

*Let $ \mu $ be the sum of a summable family $ (\mu_i)_{i \in I} $ of measures on T. In order that a mapping f of T into a topological space F (Hausdorff or not) be $ \mu $-measurable, it is necessary and sufficient that f be $ \mu_i $-measurable for every $ i \in I $.*

### 8. Crushings

#### Definition 10 {#int-ix-s1-def-10 .statement}

*One calls crushing of T for $ \mu $, or $ \mu $-crushing, any locally countable family $ (K_\alpha)_{\alpha \in A} $ of pairwise disjoint compact subsets of T such that the set $ N = T - \bigcup_{\alpha \in A} K_\alpha $ is locally $ \mu $-negligible.*

#### Proposition 9 {#int-ix-s1-prop-9 .statement}

*a) There exists a crushing $ (K_\alpha)_{\alpha \in A} $ of T for $ \mu $.
b) Let $ (K_\alpha)_{\alpha \in A} $ be a crushing of T for $ \mu $. If $ \mu_\alpha $ is the measure on T defined by $ \mu_{K_\alpha} $ (No. 3, Example 2), then the family $ (\mu_\alpha)_{\alpha \in A} $ is summable,* its sum is equal to $ \mu $, and, for every function $ f \in \mathcal{F}_+(T) $,

$$
\mu^\bullet(f) = \sum_{\alpha \in A} \mu_\alpha^\bullet(f) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_{K_\alpha}) . \tag{1}
$$

For a mapping $ g $ of $ T $ into a topological space $ G $ (Hausdorff or not) to be $ \mu $-measurable, it is necessary and sufficient that $ g_{K_\alpha} $ be $ \mu_{K_\alpha} $-measurable for every $ \alpha \in A $.

A) *Existence of a crushing*:

The proof is a repetition of that of Prop. 14 of Ch. IV, §5, No. 9, with slight modifications. Let $ \mathcal{K} $ be the set of compact subsets $ K $ of $ T $ such that $ \mathrm{Supp}(\mu_K) = K $, and let $ \mathcal{H} $ be the set (ordered by inclusion) of subsets $ \mathcal{L} $ of $ \mathcal{K} $ consisting of pairwise disjoint sets. Let us first show that every element $ \mathcal{L} $ of $ \mathcal{H} $ is *locally countable*. Let $ x $ be a point of $ T $, and $ V $ an open neighborhood of $ x $ such that $ \mu^\bullet(V) < +\infty $; let $ \mathcal{L}_V $ be the set of $ K \in \mathcal{L} $ that intersect $ V $. If $ (K_i)_{1 \leq i \leq n} $ is a finite sequence of distinct elements of $ \mathcal{L}_V $, we have, by the Cor. of Prop. 4,

$$
\sum_{i=1}^n \mu^\bullet(K_i \cap V) = \mu^\bullet\left(V \cap \left( \bigcup_{i=1}^n K_i \right) \right) \leq \mu^\bullet(V),
$$

because the $ K_i $ are pairwise disjoint. Thus,

$$
\sum_{K \in \mathcal{L}_V} \mu^\bullet(K \cap V) < +\infty.
$$

Now, $ \mu^\bullet(K \cap V) = \mu_K^\bullet(K \cap V) > 0 $ for every $ K \in \mathcal{L}_V $, because $ K \cap V $ is nonempty, open in $ K $, and the support of $ \mu_K $ is all of $ K $; $ \mathcal{L}_V $ is therefore countable, and $ \mathcal{L} $ is indeed locally countable. It is immediate that $ \mathcal{H} $ is inductive, and nonempty (one has $ \varnothing \in \mathcal{H} $). Thus, let $ \mathfrak{H} $ be a maximal element of $ \mathcal{H} $. We are going to show that the set $ N = T - \bigcup_{K \in \mathfrak{H}} K $ is locally negligible. By Prop. 2, it suffices to verify that $ \mu^\bullet(N \cap L) = 0 $ for every compact set $ L $, or again that $ \mu_L^\bullet(N \cap L) = 0 $. We shall argue by contradiction. Thus, suppose that $ \mu_L^\bullet(N \cap L) > 0 $. Since the set of $ K \in \mathfrak{H} $ that intersect $ L $ is countable, $ N \cap L $ is $ \mu_L $-measurable; therefore there exists a compact set $ J $ contained in $ N \cap L $ such that $ \mu_L^\bullet(J) > 0 $. Let $ S $ be the support of the nonzero measure $ (\mu_L)_J = \mu_J $; it is contained in $ N $, the measure $ \mu_S $ is nonzero, and $ \mathrm{Supp}(\mu_S) = S $ (Ch. IV, §5, No. 7, Lemma 2). The set $ \mathfrak{H} \cup \{S\} $ therefore belongs to $ \mathcal{H} $, in contradiction with the maximal character of $ \mathfrak{H} $. This proves the existence of a crushing.

(1) We shall see later on (§2, No. 2) that $ \mu_\alpha $ is the measure $ \varphi_{K_\alpha} \cdot \mu $.

B) Proof of (7):
For every $ \alpha \in A $, $ \mu_\alpha^\bullet(f) = \mu_{K_\alpha}^\bullet(f_{K_\alpha}) = \mu^\bullet(f \varphi_{K_\alpha}) $ by formula (3) of No. 3 and Prop. 2 a) of No. 2; these formulas show that the encumbrance $ \sum_{\alpha \in A} \mu_\alpha^\bullet $ is $ \leq \mu^\bullet $, hence that the family $ (\mu_\alpha)_{\alpha \in A} $ is summable (No. 7, Prop. 7). It thus suffices to show that $ \mu = \sum_{\alpha \in A} \mu_\alpha $, that is, to establish the formula
$$
\mu_K^\bullet = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet
$$
for every compact subset K of T. Now, K being fixed, the set $ A' $ of $ \alpha \in A $ such that $ K_\alpha $ intersects K is countable. Let $ g \in \mathcal{F}_+(K) $; then $ g^0 = g^0 \varphi_N + \sum_{\alpha \in A} g^0 \varphi_{K_\alpha} $, and $ g^0 \varphi_{K_\alpha} = 0 $ for $ \alpha \in A - A' $; by Prop. 4 of No. 5, it follows that $ \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) $, whence
$$
\mu_K^\bullet(g) = \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g^0) = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet(g);
$$
thus (8) is established.

C) Measurability:
For a function $ g $ defined on T to be $ \mu $-measurable, it is necessary and sufficient that it be $ \mu_\alpha $-measurable for every $ \alpha \in A $ (No. 7, Prop. 8); but this amounts to saying that $ g_{K_\alpha} $ is $ \mu_{K_\alpha} $-measurable for all $ \alpha \in A $ (No. 5, Example). Q.E.D.

As in Prop. 14 of Ch. IV, §5, No. 9, one can require the compact sets $ K_\alpha $ to belong to a $ \mu $-dense set of compact subsets of T, given in advance. We will only need the following result, which we shall establish directly:

#### Proposition 10 {#int-ix-s1-prop-10 .statement}

— *If g is a $ \mu $-measurable mapping with values in a topological space G (Hausdorff or not), there exists a $ \mu $-crushing $ (L_\beta)_{\beta \in B} $ of T such that the restrictions $ g_{L_\beta} $ are continuous for all $ \beta \in B $.*

Consider a crushing $ (K_\alpha)_{\alpha \in A} $ of T for $ \mu $. Since the mapping $ g $ is measurable, there exists for each $ \alpha \in A $ a partition of $ K_\alpha $ into a sequence $ (K_{\alpha n}) $ of compact sets and a locally negligible set $ N_\alpha $, such that the restriction of $ g $ to each of the sets $ K_{\alpha n} $ is continuous. The family $ (K_{\alpha n})_{(\alpha, n) \in A \times \mathbf{N}} $ is then the sought-for crushing. For, it is locally countable, and the set $ N' = N \cup (\bigcup_\alpha N_\alpha) $ is locally negligible, because a compact set intersects at most a countable infinity of sets $ N_\alpha $.

#### Scholium {#int-ix-s1-n8-sch-1 .statement}

— Let $ (K_\alpha)_{\alpha \in A} $ be a crushing of T, and let $ N = T - \bigcup_\alpha K_\alpha $. We denote by $ T' $ the locally compact space obtained by equipping $ T' $ with the sum topology of the topologies of the subspaces $ K_\alpha $ and any locally compact topology on $ N $ (unless expressly mentioned to the contrary, $ N $ will always be equipped with the discrete topology). For each $ \alpha \in A $, let $ i_\alpha $ be the canonical injection of $ K_\alpha $ into $ T' $, and let $ \mu'_\alpha $ be the measure on $ T' $ that is the image of $ \mu_{K_\alpha} $ under $ i_\alpha $. The family $ (\mu'_\alpha) $ is summable: for, if $ f $ is a continuous function on $ T' $ with compact support, then $ \operatorname{Supp}(f) $ intersects $ K_\alpha $ for only a finite number of indices $ \alpha $. We set $ \mu' = \sum_{\alpha \in A} \mu'_\alpha $. The set $ N $ being locally negligible for $ \mu' $, since it is so for each $ \mu'_\alpha $ (Prop. 9), the family $ (K_\alpha)_{\alpha \in A} $ is a $ \mu' $-crushing of $ T' $; now, the measure induced by $ \mu' $ on $ K_\alpha $ is obviously $ \mu_{K_\alpha} $ and the formula (7), applied to $ \mu $ and to $ \mu' $, shows that $ \mu^\bullet = \mu'^\bullet $. Similarly, the last assertion of the statement of Prop. 9, applied to $ \mu $ and to $ \mu' $, shows that *the measurable mappings are the same for the two measures $ \mu $ and $ \mu' $*.

These two properties permit reducing nearly all of the theory of integration with respect to $ \mu $ to the theory elaborated for locally compact spaces. These considerations will be developed in No. 10.

Here is another application of the concept of crushing:

#### Proposition 11 {#int-ix-s1-prop-11 .statement}

*Let $ X $ be a $ \mu $-measurable subset of $ T $. There exists a locally countable family $ (L_\alpha)_{\alpha \in A} $ of compact subsets of $ X $, pairwise disjoint, such that $ X - \bigcup_{\alpha \in A} L_\alpha $ is locally $ \mu $-negligible. If, in addition, $ X $ is the union of a sequence $ (X_n) $ of measurable sets such that $ \mu^\bullet(X_n) < +\infty $, then the set $ B $ of $ \alpha \in A $ such that $ \mu^\bullet(L_\alpha) \neq 0 $ is countable, and $ X - \bigcup_{\beta \in B} L_\beta $ is locally $ \mu $-negligible.*

Let $ f $ be the characteristic function of $ X $, and let $ (K_\alpha)_{\alpha \in A} $ be a crushing of $ T $ such that the restriction of $ f $ to each of the $ K_\alpha $ is continuous (Prop. 10). The set $ L_\alpha = K_\alpha \cap X $ is then compact for every $ \alpha \in A $, and $ (L_\alpha)_{\alpha \in A} $ is the desired family. Let us pass to the second assertion; the measurable sets $ X_n $ may clearly be assumed to be disjoint, and it suffices to establish the assertion for each of them. In other words, changing notation if necessary, we can suppose that $ \mu^\bullet(X) < +\infty $. The set $ B $ of $ \alpha \in A $ such that $ \mu^\bullet(L_\alpha) > 0 $ is then countable, and it only remains to prove that the set $ N = \bigcup_{\alpha \in A - B} L_\alpha $ is locally negligible. But $ K $ is a compact set; the family $ (L_\alpha)_{\alpha \in A} $ being locally countable, the set $ K \cap N $ is the union of a *countable* subfamily of the family $ (K \cap L_\alpha)_{\alpha \in A - B} $, and this set is therefore locally negligible. The same is then true of $ N $ (No. 2, Prop. 2) and the proposition is established.

### 9. Upper integral

#### Definition 11 {#int-ix-s1-def-11 .statement}

*For every function $ f \in \mathcal{F}_+(T) $, one defines the upper integral of $ f $ (with respect to the measure $ \mu $) to be the finite or infinite positive number*

$$
\mu^*(f) = \inf_g \mu^\bullet(g),
$$

*where $ g $ runs over the set of lower semi-continuous functions that are $ \geqslant f $.*

The notations $ \int^* f(t) d\mu(t) $ and $ \int^* f d\mu $ are also used. When $ T $ is locally compact, this definition coincides with the usual definition (Ch. V, §1, No. 1, Prop. 4). Clearly $ \mu^\bullet(f) \leqslant \mu^*(f) $, with equality when $ f $ is lower semi-continuous. If $ A $ is a subset of $ T $, one writes $ \mu^*(A) $ instead of $ \mu^*(\varphi_A) $, and this number is called the *outer measure* of $ A $. The measurable sets with finite outer measure are called *integrable sets*, as in the case of locally compact spaces.

A function $ f $ with values in a Banach space or in $ \overline{\mathbf{R}} $ such that $ \mu^*(|f|) = 0 $ is said to be *negligible*; a set $ A \subset T $ is said to be negligible if $ \varphi_A $ is negligible, that is, if $ \mu^*(A) = 0 $. The expression *almost everywhere* is introduced as in Ch. IV, §2, No. 3.

#### Proposition 12 {#int-ix-s1-prop-12 .statement}

*The function $ \mu^* $ is an encumbrance on $ T $.*

The properties $ a), b), c) $ of Def. 1 of No. 1 are obvious. The proof of the property $ d) $ is identical to that of Th. 3 of Ch. IV, §1, No. 3, on taking into account Props. 4 and 5 *a)*.

#### Corollary {#int-ix-s1-n9-cor-1 .statement}

*A function $ f $, with values in a Banach space or in $ \overline{\mathbf{R}} $, is negligible if and only if $ f(t) = 0 $ almost everywhere.*

One reduces immediately to the case of a positive function. The proof is then identical to that of Th. 1 of Ch. IV, §2, No. 3.

#### Proposition 13 {#int-ix-s1-prop-13 .statement}

*For every subset $ A $ of $ T $, $ \mu^*(A) $ is the infimum of the outer measures of the open sets containing $ A $.*

The proof is identical to that of Prop. 19 of Ch. IV, §1, No. 4.

#### Definition 12 {#int-ix-s1-def-12 .statement}

*Let $ f $ be a function defined on $ T $, with values in a Banach space or in $ \overline{\mathbf{R}} $. One says that $ f $ is moderated for the measure $ \mu $, or $ \mu $-moderated, if $ f $ is zero on the complement of a countable union of integrable open sets. A subset $ A $ of $ T $ is said to be moderated if the function $ \varphi_A $ is moderated. The measure $ \mu $ is said to be moderated if the function $ 1 $ is $ \mu $-moderated.*

For example, since the encumbrance $ \mu^\bullet $ is locally bounded, every compact subset $ K $ of $ T $ is contained in an open set $ V $ such that $ \mu^\bullet(V) < +\infty $; a function that is zero outside a compact set is therefore moderated. A negligible function is moderated. The remarks following Def. 2 of Ch. V, §1, No. 2 can immediately be extended to the present context. In particular, the sum of a sequence of moderated positive functions is moderated.

#### Remark 1 {#int-ix-s1-n9-rem-1 .statement}

On a Lindelöf space T (TG, IX, Appendix I, Def. 1),¹ and in particular on a Souslin space (ibid., Cor. of Prop. 1), every measure is moderated. For, the open sets of finite measure form a covering of T, from which one can extract a countable covering of T.

#### Remark 2 {#int-ix-s1-n9-rem-2 .statement}

Beware, however, that the existence of a sequence of Borel sets of finite measure for $ \mu $, with union T, does not necessarily imply the existence of a sequence of open sets of finite measure with union T (in other words, does not imply that $ \mu $ is moderated). See Exer. 8.

#### Proposition 14 {#int-ix-s1-prop-14 .statement}

Let $ f \in \mathcal{F}_+(T) $. If $ f $ is $ \mu $-moderated, then $ \mu^*(f) = \mu^\bullet(f) $; if $ f $ is not $ \mu $-moderated, then $ \mu^*(f) = +\infty $.

If $ \mu^*(f) < +\infty $, there exists a lower semi-continuous function $ g \geq f $ such that $ \mu^\bullet(g) < +\infty $. For every $ n \in \mathbf{N} $, let $ G_n $ be the set of $ t \in T $ such that $ g(t) > 1/n $; the set $ G_n $ is open, one has $ \mu^\bullet(G_n) \leq n \mu^\bullet(g) < +\infty $, and $ f $ is zero outside the union of the $ G_n $: the function $ f $ is therefore moderated.

Next, let us show that $ \mu^* $ and $ \mu^\bullet $ have the same value for moderated functions. Since $ \mu^* $ and $ \mu^\bullet $ are encumbrances, it suffices to establish the relation $ \mu^*(f) = \mu^\bullet(f) $ when $ f $ is a positive function, bounded above by a constant M, and zero outside an open set G of finite measure, which we shall now do.

The measure $ \mu $ is the supremum, in $ \mathcal{M}(T) $, of an increasing directed family $ (\mu_i)_{i \in I} $ of measures with compact support: this follows at once from Prop. 9 of No. 8. Let $ g $ be a lower semi-continuous function on T, between $ f $ and the lower semi-continuous function $ M \varphi_G $. Set $ \nu_i = \mu - \mu_i $; then $ \mu^\bullet = \mu_i^\bullet + \nu_i^\bullet $ (No. 2, Remark 1), consequently
$$
\mu^\bullet(g) - \mu^\bullet(f) = (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + (\nu_i^\bullet(g) - \nu_i^\bullet(f))
$$
$$
\leq (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + \nu_i^\bullet(M \varphi_G).
$$
One has $ \nu_i^\bullet(M \varphi_G) = \mu^\bullet(M \varphi_G) - \mu_i^\bullet(M \varphi_G) $ and $ \mu^\bullet(M \varphi_G) = \sup \mu_i^\bullet(M \varphi_G) $ (No. 7, Prop. 6); the number $ \nu_i^\bullet(M \varphi_G) $ may therefore be made arbitrarily small by a suitable choice of $ i $. Thus everything comes down to showing that one can find, for any number $ c > 0 $ and any index $ i \in I $, a lower semi-continuous function $ g $ between $ f $ and $ M \varphi_G $, such that $ \mu_i^\bullet(g) - \mu_i^\bullet(f) \leq c $. Now, let L be the compact support of the measure $ \mu_i $, and let $ \lambda $ be the measure $ (\mu_i)_L $; since $ \mu_i $ is concentrated on L, one has $ \mu_i^\bullet(h) = \mu_i^\bullet(h \varphi_L) = \lambda^\bullet(h_L) $ for every function $ h \in \mathcal{F}_+(T) $ (No. 1, Lemma 1 and No. 2, Prop. 2); therefore
$$
\mu_i^\bullet(g) - \mu_i^\bullet(f) = \lambda^\bullet(g_L) - \lambda^\bullet(f_L).
$$

¹ The cited appendix in TG does not appear in GT (which translated an earlier edition of Ch. IX). Lindelöf spaces are defined in GT, I, §9, Exer. 14; this exercise and the definition of Souslin space (GT, IX, §6, No. 2, Def. 2) cover the material needed here.

But L is compact; therefore $ \lambda^* = \lambda^* $, consequently there exists a lower semi-continuous function $ h $ defined on L, that is $ \geq f_L $ and is such that $ \lambda^*(h) \leq \lambda^*(f_L) + c $. Since the set L is closed in T, the function k equal to h on L, and to $ +\infty $ on $ T - L $, is lower semi-continuous on T and is $ \geq f $, and $ \lambda^*(k_L) = \lambda^*(h) \leq \lambda^*(f_L) + c $. It remains only to set $ g = \inf(k, M \varphi_G) $: $ g $ is lower semi-continuous, $ g \geq f $ and

$$
\mu_i^*(g) \leq \mu_i^*(k) = \lambda^*(k_L) \leq \lambda^*(f_L) + c = \mu_i^*(f) + c.
$$

#### Corollary 1 {#int-ix-s1-prop-14-cor-1 .statement}

*For a function to be negligible, it is necessary and sufficient that it be locally negligible and moderated.*

#### Corollary 2 {#int-ix-s1-prop-14-cor-2 .statement}

*For a function $ f $ to be locally negligible, it is necessary and sufficient that every $ x \in T $ possess a neighborhood V such that $ f \varphi_V $ is negligible.*

For, if this property is satisfied, $ f \varphi_K $ is negligible for every compact set K, and $ f $ is therefore locally negligible (No. 2, Prop. 2). Conversely, suppose that $ f $ is locally negligible, and let $ x $ be a point of T; $ x $ admits an open neighborhood V of finite measure. The function $ f \varphi_V $ is then locally negligible and moderated, hence is negligible.

#### Corollary 3 {#int-ix-s1-prop-14-cor-3 .statement}

*Let $ f $ be a moderated function defined on T. There exists a sequence $ (K_n) $ of pairwise disjoint compact sets, and a negligible set H, such that $ f = f \varphi_H + \sum_n f \varphi_{K_n} $.*

For, let G be a set that is a countable union of integrable open sets, such that $ f $ is zero outside G; then G is the union of a sequence $ (K_n) $ of pairwise disjoint compact sets and a locally negligible set H (No. 8, Prop. 11); but H is moderated, therefore negligible.

#### Corollary 4 {#int-ix-s1-prop-14-cor-4 .statement}

*If $ \mu $ and $ \nu $ are two measures on T such that $ \mu^* = \nu^* $, then $ \mu = \nu $.*

For, the equality $ \mu^* = \nu^* $ implies that $ \mu^*(f) = \nu^*(f) $ for every positive function $ f $ that is moderated for $ \mu $ and $ \nu $, hence for every positive function with compact support; it follows that $ \mu^* = \nu^* $ (No. 2, Prop. 2), then $ \mu = \nu $ (No. 2, Cor. of Prop. 2).

#### Corollary 5 {#int-ix-s1-prop-14-cor-5 .statement}

*If $ \mu $ is a moderated measure on T, there exists a sequence $ (\mu_n)_{n \in \mathbf{N}} $ of measures with compact support such that $ \mu = \sum_{n \in \mathbf{N}} \mu_n $.*

By hypothesis, the constant function 1 is $ \mu $-moderated. Let us apply Cor. 3 to the case $ f = 1 $; thus, there exists a sequence $ (K_n)_{n \in \mathbf{N}} $ of pairwise disjoint compact subsets of T such that $ 1 = \sum_{n \in \mathbf{N}} \varphi_{K_n} $ $ \mu $-almost everywhere. Let $ \mu_n $ be the measure on T defined by the measure $ \mu_{K_n} $ on $ K_n $ (No. 3, Example 2). One knows (No. 6, Remark 2) that $ \mu_n $ has compact support, and that $ \mu_n^\bullet(f) = \mu^\bullet(f \varphi_{K_n}) $ for $ f \in \mathcal{F}_+(T) $. Now, $ f $ is equal to $ \sum_{n \in \mathbf{N}} f \varphi_{K_n} $ $ \mu $-almost everywhere, whence

$$
\mu^\bullet(f) = \sum_{n \in \mathbf{N}} \mu^\bullet(f \varphi_{K_n}) = \sum_{n \in \mathbf{N}} \mu_n^\bullet(f).
$$

It follows that $ \mu = \sum_{n \in \mathbf{N}} \mu_n $ (No. 7, Prop. 7).

### 10. Integration theory

#### Definition 13 {#int-ix-s1-def-13 .statement}

— *Let* $ p \in [1, +\infty[ $; *one denotes by* $ \overline{\mathcal{L}}^p(T, \mu) $ *(resp.* $ \overline{\mathcal{L}}_F^p(T, \mu) $ *if F is a Banach space) the set of mappings* $ \mathbf{f} $ *of T into* $ \overline{\mathbf{R}} $ *(resp. into F) that are $ \mu $-measurable and satisfy* $ \mu^\bullet(|\mathbf{f}|^p) < +\infty $. *One denotes by* $ \mathcal{L}^p(T, \mu) $ *(resp.* $ \mathcal{L}_F^p(T, \mu) $*) the set of $ \mu $-moderated elements of* $ \overline{\mathcal{L}}^p(T, \mu) $ *(resp.* $ \overline{\mathcal{L}}_F^p(T, \mu) $*).*

We will write $ \overline{N}_p(\mathbf{f}) = \left( \mu^\bullet(|\mathbf{f}|^p) \right)^{1/p} $, $ N_p(\mathbf{f}) = \left( \mu^*(|\mathbf{f}|^p) \right)^{1/p} $. We denote by $ \overline{N}_\infty(\mathbf{f}) $ the infimum of the numbers $ k \geq 0 $ such that $ |\mathbf{f}| \leq k $ locally $ \mu $-almost everywhere; if $ \overline{N}_\infty(\mathbf{f}) < +\infty $, $ \mathbf{f} $ is said to be essentially bounded. The set of measurable and essentially bounded mappings of T into $ \overline{\mathbf{R}} $ (resp. into F) is denoted $ \overline{\mathcal{L}}^\infty(T, \mu) $ (resp. $ \overline{\mathcal{L}}_F^\infty(T, \mu) $). The elements of $ \overline{\mathcal{L}}_F^1(T, \mu) $ (resp. $ \mathcal{L}_F^1(T, \mu) $) are called essentially integrable functions (resp. integrable functions) with values in F.

If $ \mu $ is a complex measure, one sets

$$
\overline{\mathcal{L}}_F^p(T, \mu) = \overline{\mathcal{L}}_F^p(T, |\mu|) \quad \text{and} \quad \mathcal{L}_F^p(T, \mu) = \mathcal{L}_F^p(T, |\mu|).
$$

The above notations are often abbreviated to $ \overline{\mathcal{L}}_F^p(\mu) $, $ \overline{\mathcal{L}}_F^p $ or $ \mathcal{L}^p(\mu) $, $ \mathcal{L}^p $, if this does not lead to any confusion.

We saw in No. 8 (*Scholium*) that one can construct a locally compact space T', having the same underlying set as T and a topology finer than that of T, and equip T' with a measure $ \mu' $ such that the $ \mu $-measurable functions and the $ \mu' $-measurable functions are the same, and such that the essential upper integrals of positive functions for $ \mu $ and $ \mu' $ are equal. It follows that the sets $ \overline{\mathcal{L}}_F^p(\mu) $ and $ \overline{\mathcal{L}}_F^p(\mu') $ are identical for $ 1 \leq p \leq +\infty $ $ ^{(1)} $. This also implies without new proof that $ \overline{\mathcal{L}}_F^p $ is a vector space, and that the function $ \overline{N}_p $ is a semi-norm on $ \overline{\mathcal{L}}_F^p(\mu) $, for which this space is complete.

Let $ \mathbf{f} $ be an element of $ \overline{\mathcal{L}}_F^p $ ($ 1 \leq p < +\infty $); since one has $ \mu^\bullet(|\mathbf{f}|^p) = \mu'^\bullet(|\mathbf{f}|^p) < +\infty $, Prop. 7 of Ch. V, §1, No. 2 implies that $ \mathbf{f} $ is zero outside

(1) Note that the space $ \mathcal{L}_F^p(\mu) $ is contained in $ \mathcal{L}_F^p(\mu') $, but is in general distinct from it.

the union of a sequence of compact subsets of T' and a locally $ \mu' $-negligible set; the latter set being locally $ \mu $-negligible, and every compact subset of T' being compact in T, it follows that f is equal locally $ \mu $-almost everywhere to a $ \mu $-moderated function. Let us denote by $ \overline{\mathcal{N}}_F $ (resp. $ \mathcal{N}_F $) the space of locally $ \mu $-negligible (resp. $ \mu $-negligible) functions; we thus have $ \overline{\mathcal{L}}_F^p = \mathcal{L}_F^p + \overline{\mathcal{N}}_F $, and $ \mathcal{N}_F = \mathcal{L}_F^p \cap \overline{\mathcal{N}}_F $ (No. 9, Cor. 1 of Prop. 14). The space $ \overline{\mathcal{L}}_F^p / \overline{\mathcal{N}}_F $ may therefore be canonically identified with $ \mathcal{L}_F^p / \mathcal{N}_F $, and one verifies immediately that this identification preserves norm; this quotient space is denoted $ L_F^p(\mu) $. It can be interpreted as the normed space associated with each of the semi-normed spaces $ \overline{\mathcal{L}}_F^p(\mu) $ and $ \mathcal{L}_F^p(\mu) $; since $ \overline{\mathcal{L}}_F^p $ is complete, the same is true of $ L_F^p $ and $ \mathcal{L}_F^p $.

The set of functions f with values in F, continuous on T' with compact support, is dense in $ \overline{\mathcal{L}}_F^p(\mu') = \overline{\mathcal{L}}_F^p(\mu) $ (Ch. IV, §3, No. 4, Def. 2). Let us take up again the notations of the Scholium of No. 8. Since a compact subset of T' intersects only a finite number of the compact sets $ K_\alpha $, every continuous function f on T' with compact support may be written as a sum
$$
f = \sum_{\alpha \in A} f_\alpha + g,
$$
where $ f_\alpha $ is, for every $ \alpha $, the extension by 0 of a continuous function on $ K_\alpha $, where $ f_\alpha = 0 $ except for a finite number of indices, and where g is locally $ \mu $-negligible. We thus have the following result:

#### Proposition 15 {#int-ix-s1-prop-15 .statement}

*The set of functions f with values in F, such that Supp(f) is compact and such that the restriction of f to Supp(f) is continuous, is dense in $ \overline{\mathcal{L}}_F^p(\mu) $ and in $ \mathcal{L}_F^p(\mu) $, for $ 1 \leq p < +\infty $.*

Note that these functions *are not* continuous functions *on* T with compact support.

Let us pass to the definition of the integral.

#### Proposition 16 {#int-ix-s1-prop-16 .statement}

*There exists one and only one continuous linear mapping $ f \mapsto \int f d\mu $, of the space $ \overline{\mathcal{L}}_F^1(\mu) $ into F, having the following property:
If f is of the form $ t \mapsto g(t)a $, where $ a \in F $, and where g is a positive function, finite, $ \mu $-measurable and such that $ \mu^*(g) < +\infty $, then $ \int f d\mu = \mu^*(g) \cdot a $.*

For, the semi-normed spaces $ \overline{\mathcal{L}}_F^1(\mu) $ and $ \overline{\mathcal{L}}_F^1(\mu') $ are identical. Since $ \mu^* = \mu'^* $, the mapping $ f \mapsto \int f d\mu' $ satisfies the conditions of the statement. On the other hand, the set of functions of the form $ f = g \cdot a $ considered in the statement is *total* in $ \overline{\mathcal{L}}_F^1(\mu') $ (Ch. IV, §3, No. 5, Prop. 10), whence uniqueness.

One says that $ \int f\, d\mu $ is the integral of $ f $ with respect to $ \mu $, and this vector is also denoted $ \mu(f) $ or $ \int f(t)\, d\mu(t) $.

Since $ \int f\, d\mu = \int f\, d\mu' $ for every essentially integrable function $ f $ with values in $ F $, all of the theory of the essential integral extends to measures on Hausdorff spaces, without new proofs; from it, one deduces results relative to the ordinary integral by restricting oneself to moderated functions. We cite in particular the following results:

— Th. 3 of Ch. IV, §3, No. 4, its extension to $ \overline{\mathcal{L}}_F^p $, and its two corollaries.
— Th. 4 of Ch. IV, §3, No. 5 (composition with a continuous linear mapping) and its corollaries; Props. 9, 11 and 12 of the same No.
— All of the results of Ch. IV, §3, No. 6, relative to the ordered vector space structure of $ L^p $.
— All of the results of Ch. IV, §3, No. 7, and in particular Lebesgue’s theorem.
— All of the results of Ch. IV, §3, No. 8, on the relations between the spaces $ L_F^p $.
— Theorem 2 of Ch. IV, §4, No. 3 (the statement of Lebesgue’s theorem specific to $ L_F^1 $).
— Hölder’s inequality (Ch. IV, §6, No. 4, Th. 2) and its corollaries.
— The relations between the spaces $ L_F^p $ established in Ch. IV, §6, No. 5.
— The results on the duality of the spaces $ L^p $ established in Ch. V, §5, No. 8.
— The Dunford–Pettis theorem (Ch. VI, §2, No. 5, Th. 1), its Corollaries 1 and 2, and Prop. 10 of Ch. VI, §2, No. 6 (dual of $ L_F^1 $).

### Exercises {#int-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
