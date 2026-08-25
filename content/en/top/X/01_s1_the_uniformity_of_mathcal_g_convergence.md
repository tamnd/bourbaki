---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 1
section_title: The uniformity of $ \mathcal{G} $-convergence
lang: en
source: top-v-x
pdf_pages: 0280-0289, 0324-0327
extraction: ocr
subsections:
    - "no": 1
      title: THE UNIFORMITY OF UNIFORM CONVERGENCE
      page: 0
      pdf_page: 280
    - "no": 2
      title: $ \mathfrak{S} $-convergence
      page: 0
      pdf_page: 281
    - "no": 3
      title: EXAMPLES OF $ \mathcal{E} $-CONVERGENCE
      page: 0
      pdf_page: 283
    - "no": 4
      title: PROPERTIES OF THE SPACES $ \mathcal{F}_\mathcal{S}(X; Y) $
      page: 0
      pdf_page: 284
    - "no": 5
      title: COMPLETE SUBSETS OF $ \mathcal{F}_\mathcal{S}(X; Y) $
      page: 0
      pdf_page: 285
    - "no": 6
      title: $ \mathcal{E} $-CONVERGENCE IN SPACES OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 286
statements: 33
exercises: 12
content_sha256: 4118cf9d425a5c3a0cd266fbb19181dfd798c8a4a1de28103c5b93a49cf6e260
---

## 1. THE UNIFORMITY OF $ \mathcal{G} $-CONVERGENCE

Notation. If $ X $ and $ Y $ are any two sets, we recall that the set of all mappings of $ X $ into $ Y $ is denoted by $ \mathcal{F}(X; Y) $, and may be identified with the product set $ Y^X $ (Set Theory, Chapter II, § 5, no. 2). For each subset $ H $ of $ \mathcal{F}(X; Y) $ and each $ x \in X $, we shall denote by $ H(x) $ the set of elements $ u(x) \in Y $ as $ u $ runs through $ H $. If $ \Phi $ is a filter base on $ \mathcal{F}(X; Y) $, we denote by $ \Phi(x) $ the filter base on $ Y $ formed by the sets $ H(x) $ as $ H $ runs through $ \Phi $. Finally, we recall that, for each $ u \in \mathcal{F}(X; Y) $ and each subset $ A $ of $ X $, $ u|A $ denotes the restriction of $ u $ to $ A $, which is a mapping of $ A $ into $ Y $; if $ H $ is a subset of $ \mathcal{F}(X; Y) $, $ H|A $ will denote the set of restrictions $ u|A $ of functions $ u \in H $.

### 1. THE UNIFORMITY OF UNIFORM CONVERGENCE

Let $ X $ be a set and let $ Y $ be a uniform space. For each entourage $ V $ of $ Y $, let $ W(V) $ denote the set of all pairs $ (u, v) $ of mappings of $ X $ into $ Y $ such that $ (u(x), v(x)) \in V $ for all $ x \in X $. As $ V $ runs through the set of entourages of $ Y $, the sets $ W(V) $ form a fundamental system of entourages of a uniformity on $ \mathcal{F}(X; Y) $. For they clearly satisfy Axiom $ (U'_1) $ (Chapter II, § 1, no. 1); if $ V, V' $ are two entourages of $ Y $ such that $ V \subset V' $, we have $ W(V) \subset W(V') $, and therefore the sets $ W(V) $ satisfy

$ (B_1) $ (Chapter I, § 6, no. 3); we have $ \widehat{W(V)} = W(\overline{V}) $ so that $ (U''_{II}) $ is satisfied; finally, the relations "$ (u(x), v(x)) \in V $ for all $ x \in X $" and "$ (v(x), w(x)) \in V $ for all $ x \in X $" imply the relation "$ (u(x), w(x)) \in \overline{V}^2 $ for all $ x \in X $"; in other words, we have $ \widehat{W(V)} \subset W(\overline{V}^2) $, which proves $ (U'''_{III}) $.

#### Definition 1 {#top-x-s1-def-1 .statement}

*The uniformity on the set $ \mathcal{F}(X; Y) $ which has as a fundamental system of entourages the set of subsets $ W(V) $, where $ V $ runs through the set of entourages of $ Y $, is called the uniformity of uniform convergence. The topology it induces is called the topology of uniform convergence. If a filter $ \Phi $ on $ \mathcal{F}(X; Y) $ converges to an element $ u_0 $ with respect to this topology, $ \Phi $ is said to converge uniformly to $ u_0 $.*

Note that the *topology* of uniform convergence on $ \mathcal{F}(X; Y) $ depends on the uniform structure of $ Y $ and not merely on the topology of $ Y $ (Exercise 4).

The uniform space obtained by endowing $ \mathcal{F}(X; Y) $ with the uniformity of uniform convergence is denoted by $ \mathcal{F}_u(X; Y) $.

### 2. $ \mathfrak{S} $-convergence

#### Definition 2 {#top-x-s1-def-2 .statement}

*Let $ X $ be a set, $ Y $ a uniform space, $ \mathfrak{S} $ a set of subsets of $ X $. The uniformity of uniform convergence in the sets of $ \mathfrak{S} $, or simply the uniformity of $ \mathfrak{S} $-convergence, is the coarsest uniformity on $ \mathcal{F}(X; Y) $ which makes uniformly continuous the restriction mappings $ u \to u|A $ of $ \mathcal{F}(X, Y) $ into the uniform spaces $ \mathcal{F}_u(A; Y) $, where $ A $ runs through $ \mathfrak{S} $. The uniform space obtained by endowing $ \mathcal{F}(X; Y) $ with the uniformity of $ \mathfrak{S} $-convergence is denoted by $ \mathcal{F}_{\mathfrak{S}}(X; Y) $.*

The topology induced by the uniformity of $ \mathfrak{S} $-convergence is called the *topology of $ \mathfrak{S} $-convergence*; it is the coarsest for which all the mappings $ u \to u|A $ of $ \mathcal{F}(X; Y) $ into $ \mathcal{F}_u(A; Y) $ ($ A \in \mathfrak{S} $) are continuous (Chapter II, § 2, no. 3, Proposition 4, Corollary).

A filter $ \Phi $ on $ \mathcal{F}(X; Y) $ converges to $ u_0 $ with respect to the topology of $ \mathfrak{S} $-convergence if and only if $ u|A $ converges uniformly to $ u_0|A $ with respect to $ \Phi $ for all $ A \in \mathfrak{S} $ (Chapter I, § 7, no. 6, Proposition 10), and $ \Phi $ is therefore said to *converge uniformly to $ u_0 $ on the sets of $ \mathfrak{S} $*.

A filter base $ \Phi $ on $ \mathcal{F}_{\mathfrak{S}}(X; Y) $ is a Cauchy filter base if and only if, for each $ A \in \mathfrak{S} $, the image of $ \Phi $ under the mapping $ u \to u|A $ is a Cauchy filter base on $ \mathcal{F}_u(A; Y) $ (Chapter II, § 3, no. 1, Proposition 4).

Let $ f $ be a mapping of a topological (resp. uniform) space $ Z $ into $ \mathcal{F}_{\mathfrak{S}}(X; Y) $. Then $ f $ is continuous (resp. uniformly continuous) if and only if, for each $ A \in \mathfrak{S} $, the mapping $ z \to f(z)|A $ of $ Z $ into $ \mathcal{F}_u(A; Y) $ is continuous (resp. uniformly continuous) (Chapter I, § 2, no. 3, Proposition 4; Chapter II, § 2, no. 3, Proposition 4).

Finally, let $ M $ be a subset of $ \mathcal{F}_{\mathfrak{S}}(X; Y) $; then $ M $ is precompact if and only if, for each $ A \in \mathfrak{S} $, the set of restrictions $ u|A $ for $ u \in M $ is a precompact subset of $ \mathcal{F}_u(A; Y) $ (Chapter II, § 4, no. 2, Proposition 3).

#### Remark 1 {#top-x-s1-n2-rem-1 .statement}

The general definition of the entourages of an initial uniformity (Chapter II, § 2, no. 3, Proposition 4) shows that a fundamental system of entourages of $ \mathcal{F}_\mathcal{S}(X; Y) $ may be obtained as follows: for each $ A \in \mathcal{S} $ and each entourage $ V $ of a fundamental system of entourages $ \mathcal{B} $ of $ Y $, let $ W(A, V) $ be the set of all pairs of mappings $ (u, v) $ of $ X $ into $ Y $ such that $ (u(x), v(x)) \in V $ for each $ x \in A $; as $ A $ runs through $ \mathcal{S} $ and $ V $ runs through $ \mathcal{B} $, the *finite intersections of the sets* $ W(A, V) $ form a fundamental system of entourages of $ \mathcal{F}_\mathcal{S}(X; Y) $.

This description shows immediately that if $ \mathcal{S}, \mathcal{S}' $ are two sets of subsets of $ X $ such that $ \mathcal{S} \subset \mathcal{S}' $, then the uniformity of $ \mathcal{S}' $-convergence is *finer* than that of $ \mathcal{S} $-convergence.

#### Remark 2 {#top-x-s1-n2-rem-2 .statement}

However, the uniformity of $ \mathcal{S} $-convergence is unaltered by replacing $ \mathcal{S} $ by the set $ \mathcal{S}' $ of all subsets of $ X $ *which are contained in finite unions of sets of* $ \mathcal{S} $. In the study of $ \mathcal{S} $-convergence we may therefore always restrict ourselves to the case where the set $ \mathcal{S} $ satisfies the following two conditions:

(F'$_1$) *Every subset of a set of* $ \mathcal{S} $ *belongs to* $ \mathcal{S} $.

(F'$_2$) *Every finite union of sets of* $ \mathcal{S} $ *belongs to* $ \mathcal{S} $.

If (F'$_2$) is satisfied, we obtain a fundamental system of entourages of $ \mathcal{F}_\mathcal{S}(X; Y) $ by taking all the sets $ W(A, V) $, where $ A $ runs through $ \mathcal{S} $ and $ V $ runs through a fundamental system of entourages of $ Y $.

#### Remark 3 {#top-x-s1-n2-rem-3 .statement}

The uniformity of $ \mathcal{S} $-convergence is the inverse image, under the mapping $ u \to (u|A)_{A \in \mathcal{S}} $ of $ \mathcal{F}(X; Y) $ into $ \prod_{A \in \mathcal{S}} \mathcal{F}_u(A; Y) $, of the uniformity of this product space (Chapter II, § 2, no. 6, Proposition 8). If $ \mathcal{S} $ is a *covering* of $ X $, this mapping is *injective* and $ \mathcal{F}_\mathcal{S}(X; Y) $ is therefore isomorphic to the uniform subspace of $ \prod_{A \in \mathcal{S}} \mathcal{F}_u(A; Y) $ which is the image of this mapping.

#### Proposition 1 {#top-x-s1-prop-1 .statement}

*If* $ Y $ *is Hausdorff and* $ \mathcal{S} $ *is a covering of* $ X $, *then the space* $ \mathcal{F}_\mathcal{S}(X; Y) $ *is Hausdorff*.

Let $ u, v $ be two elements of $ \mathcal{F}_\mathcal{S}(X; Y) $ such that $ (u, v) \in W(A, V) $ for every entourage $ V $ of $ Y $ and every $ A \in \mathcal{S} $. Since $ Y $ is Hausdorff it follows that $ u $ and $ v $ coincide on every set $ A \in \mathcal{S} $, and since $ \mathcal{S} $ covers $ X $ we must have $ u = v $.

#### Remark 4 {#top-x-s1-n2-rem-4 .statement}

Let $ H $ be a subset of $ \mathcal{F}(X; Y) $. By abuse of language, the uniformity (resp. topology) induced on $ H $ by the uniformity (resp. topology) of $ \mathcal{S} $-convergence on $ \mathcal{F}(X; Y) $ is called the uniformity (resp. topology) of $ \mathcal{S} $-convergence on the set $ H $.

#### Remark 5 {#top-x-s1-n2-rem-5 .statement}

Let $ L $ be a set filtered by a filter $ \mathfrak{S} $, and let $ \lambda \to u_\lambda $ be a mapping of $ L $ into $ \mathcal{F}_\mathcal{S}(X; Y) $ which has a limit $ v $ with respect to $ \mathfrak{S} $; we say then that, *with respect to the filter* $ \mathfrak{S} $, *the mappings* $ u_\lambda $ *of* $ X $ *into* $ Y $ *converge uniformly to* $ v $ *[or that the family* $ (u_\lambda) $ *is uniformly convergent to* $ v $] *in every set of* $ \mathcal{S} $. *If* $ L = \mathbf{N} $ *and* $ \mathfrak{S} $ *is the Fréchet filter*, we omit mention of $ \mathfrak{S} $ *in this statement*.

More particularly, suppose that there is a commutative and associative law of composition (written additively) defined on $ Y $. If $ (u_n) $ is any sequence of mappings of $ X $ into $ Y $, let $ v_n $ be the mapping defined by

$$
v_n(x) = \sum_{k=0}^n u_k(x) \quad (n \in \mathbf{N});
$$

we say that *the series whose general term is* $ u_n $ *is uniformly convergent in every set of* $ \mathcal{G} $ *if the sequence* $ (v_n) $ *is uniformly convergent in every set of* $ \mathcal{G} $. Likewise we define a *uniformly summable family* $ (u_\lambda)_{\lambda \in L} $ of mappings of $ X $ into $ Y $ by considering the mappings $ x \to \sum_{\lambda \in J} n_\lambda(x) $ for all finite subsets $ J $ of $ L $ and the limit of these mappings in $ \mathcal{F}_\mathcal{G}(X; Y) $ with respect to the directed set of finite subsets of $ L $ (Chapter III, § 5, no. 1).

#### Remark 6 {#top-x-s1-n2-rem-6 .statement}

It follows immediately from Definitions 1 and 2 that, for every $ x \in \bigcup_{A \in \mathcal{G}} A $, the mapping $ u \to u(x) $ of $ \mathcal{F}_\mathcal{G}(X; Y) $ into $ Y $ is *uniformly continuous*. Hence, in particular, if $ \overline{H} $ denotes the closure of a subset $ H $ of $ \mathcal{F}_\mathcal{G}(X; Y) $, we have $ \overline{H}(x) \subset \overline{H(x)} $ for all $ x \in \bigcup_{A \in \mathcal{G}} A $ (Chapter I, § 2, no. 1, Theorem 1).

### 3. EXAMPLES OF $ \mathcal{E} $-CONVERGENCE

I. *Uniform convergence in a subset of* $ X $. Let $ A $ be a subset of $ X $ and take $ \mathcal{G} = \{ A \} $. The uniformity (resp. topology) of $ \mathcal{G} $-convergence is then called the *uniformity* (resp. *topology*) *of uniform convergence in* $ A $; if a filter $ \Phi $ on $ \mathcal{F}_\mathcal{G}(X; Y) $ converges to $ u_0 $, it is said to converge to $ u_0 $ *uniformly in* $ A $. When $ A = X $ we recover the structure of uniform convergence defined in no. 1.

II. *Pointwise convergence in a subset of* $ X $. Let $ A $ be a subset of $ X $, and take $ \mathcal{G} $ to be the set of all subsets of $ X $ which consist of a single point belonging to $ A $ (by Remark 2 of no. 2 it comes to the same thing if we take $ \mathcal{G} $ to be the set of all finite subsets of $ A $). The uniformity (resp. topology) of $ \mathcal{G} $-convergence is then called the *uniformity* (resp. *topology*) *of pointwise convergence in* $ A $; if a filter $ \Phi $ on $ \mathcal{F}_\mathcal{G}(X; Y) $ converges to $ u_0 $, it is said to converge to $ u_0 $ *pointwise in* $ A $. This will be the case if and only if, for each $ x \in A $, $ u_0(x) $ is a limit of $ u(x) $ with respect to the filter $ \Phi $.

In particular, when $ A = X $, the uniformity (resp. topology) of pointwise convergence in $ X $ is called simply the *uniformity* (resp. *topology*) *of pointwise convergence*; the uniform space obtained by endowing $ \mathcal{F}(X; Y) $ with this structure is denoted by $ \mathcal{F}_s(X; Y) $. Note that the topology of pointwise convergence is just the *product* topology on $ Y^X $ and therefore depends only on the topology of $ Y $, and not on its uniform structure.

III. Compact convergence. Suppose that $ X $ is a topological space, and take $ \mathcal{S} $ to be the set of all compact subsets of $ X $. The uniformity (resp. the topology) of $ \mathcal{S} $-convergence is then called the uniformity (resp. the topology) of compact convergence, and the uniform space obtained by endowing $ \mathcal{F}(X; Y) $ with this uniformity is denoted by $ \mathcal{F}_c(X; Y) $. The structure of compact convergence is coarser than that of uniform convergence, and the two coincide if $ X $ is compact; also it is finer than the structure of pointwise convergence, and these two coincide if $ X $ is discrete.

If $ X $ is a uniform space we can define on $ \mathcal{F}(X; Y) $ the uniformity of precompact convergence by taking $ \mathcal{S} $ to be the set of all precompact subsets of $ X $. Again, if $ X $ is a metric space we may take $ \mathcal{S} $ to be the set of all bounded subsets of $ X $; the uniformity of $ \mathcal{S} $-convergence is then called the uniformity of bounded convergence.

### 4. PROPERTIES OF THE SPACES $ \mathcal{F}_\mathcal{S}(X; Y) $

#### Proposition 2 {#top-x-s1-prop-2 .statement}

Let $ X_1, X_2 $ be two sets, let $ Y $ be a uniform space and let $ \mathcal{S}_i $ be a set of subsets of $ X_i $ ($ i = 1, 2 $) and $ \mathcal{S}_1 \times \mathcal{S}_2 $ the set of subsets of $ X_1 \times X_2 $ of the form $ A_1 \times A_2 $, where $ A_i \in \mathcal{S}_i, i = 1, 2 $. Then the canonical bijection
$$
\mathcal{F}(X_1 \times X_2; Y) \to \mathcal{F}(X_1; \mathcal{F}(X_2; Y))
$$
(Set Theory, R, § 4, no. 14) is an isomorphism of the uniform space
$$
\mathcal{F}_{\mathcal{S}_1 \times \mathcal{S}_2}(X_1 \times X_2; Y)
$$
onto $ \mathcal{F}_{\mathcal{S}_1}(X_1; \mathcal{F}_{\mathcal{S}_2}(X_2; Y)) $.

Let $ V $ be an entourage of $ Y $ and let $ A_i \in \mathcal{S}_i (i = 1, 2) $; then it follows immediately from the definitions that $ W(A_1 \times A_2, V) $ is identified with $ W(A_1, W(A_2, V)) $ by the canonical bijection, and the result is immediate.

#### Proposition 3 {#top-x-s1-prop-3 .statement}

a) Let $ X $ be a set; let $ \mathcal{S} $ be a set of subsets of $ X $; let $ Y, Y' $ be two uniform spaces; and let $ f : Y \to Y' $ be a uniformly continuous mapping. Then the mapping $ u \to f \circ u $ of $ \mathcal{F}_\mathcal{S}(X; Y) $ into $ \mathcal{F}_\mathcal{S}(X; Y') $ is uniformly continuous.

b) Let $ X, X' $ be two sets; let $ \mathcal{S} $ (resp. $ \mathcal{S}' $) be a set of subsets of $ X $ (resp. $ X' $); let $ Y $ be a uniform space; and let $ g : X' \to X $ be a mapping such that, for each $ A' \in \mathcal{S}' $, $ g(A') $ is contained in a finite union of sets of $ \mathcal{S} $. Then the mapping $ u \to u \circ g $ of $ \mathcal{F}_\mathcal{S}(X, Y) $ into $ \mathcal{F}_{\mathcal{S}'}(X'; Y) $ is uniformly continuous.

#### Proposition 4 {#top-x-s1-prop-4 .statement}

Let $ X, Y $ be two sets, let $ (X_\lambda)_{\lambda \in L} $ be a family of sets and let $ (Y_\mu)_{\mu \in M} $ be a family of uniform spaces. For each $ \lambda \in L $, let $ \mathcal{S}_\lambda $ be a set of subsets of $ X_\lambda $, let $ g_\lambda $ be a mapping of $ X_\lambda $ into $ X $, and let $ \mathcal{S} $ be the set of subsets of $ X $ which is the union of the sets $ g_\lambda(\mathcal{S}_\lambda) $. For each $ \mu \in M $, let $ f_\mu $ be a mapping of $ Y $ into $ Y_\mu $, and endow $ Y $ with the coarsest uniformity for which the $ f_\mu $ are uniformly continuous. Then the uniformity of $ \mathcal{S}$-convergence on $ \mathcal{F}(X; Y) $ is the coarsest uniformity which makes uniformly continuous the mappings $ u \to f_\mu \circ u \circ g_\lambda $ of $ \mathcal{F}(X; Y) $ into $ \mathcal{F}_{\mathcal{S}_\lambda}(X_\lambda, Y_\mu) $.

These propositions are immediate consequences of the description of a fundamental system of entourages for the uniformity of $ \mathcal{S}$-convergence given in no. 2, Remark 1; the details of the proofs are left to the reader. Proposition 4 implies, in particular:

#### Corollary {#top-x-s1-n4-cor-1 .statement}

Let $ X $ be a set, let $ (Y_i)_{i \in I} $ be a family of uniform spaces and let $ \mathcal{S} $ be a set of subsets of $ X $. If we endow $ \prod_{i \in I} Y_i $ with the product uniformity, the canonical bijection of the uniform space $ \mathcal{F}_\mathcal{S}(X, \prod_{i \in I} Y_i) $ onto the product uniform space $ \prod_{i \in I} \mathcal{F}_\mathcal{S}(X; Y_i) $ (Set Theory, R, § 4, no. 13) is an isomorphism.

### 5. COMPLETE SUBSETS OF $ \mathcal{F}_\mathcal{S}(X; Y) $

#### Proposition 5 {#top-x-s1-prop-5 .statement}

Let $ \Phi $ be a set, $ Y $ a uniform space and $ \mathcal{S} $ a set of subsets of $ X $. Then a filter $ \Phi $ on $ \mathcal{F}_\mathcal{S}(X; Y) $ converges to $ u_0 $ if and only if $ \Phi $ is a Cauchy filter with respect to the uniformity of $ \mathcal{S}$-convergence and converges pointwise to $ u_0 $ in $ B = \bigcup_{A \in \mathcal{S}} A $.

Since the structure of pointwise convergence in $ B $ is coarser than that of $ \mathcal{S}$-convergence, it is enough to show that for each $ A \in \mathcal{S} $ and each closed entourage $ V $ of $ Y $, $ W(A, V) $ is closed in $ B $ with respect to the topology of pointwise convergence (Chapter II, § 3, no. 3, Proposition 7). Now $ W(A, V) $ is the intersection of the inverse images of $ V $ under the mappings $ (u, v) \to (u(x), v(x)) $ as $ x $ runs through $ A $; these mappings are continuous with respect to the topology of pointwise convergence (no. 2, Remark 6), and the result follows.

#### Corollary 1 {#top-x-s1-prop-5-cor-1 .statement}

A subspace $ H $ of $ \mathcal{F}_\mathcal{S}(X; Y) $ is complete if and only if, for each Cauchy filter $ \Phi $ on $ H $, there exists $ u_0 \in H $ such that $ \Phi $ converges pointwise to $ u_0 $ in $ B = \bigcup_{A \in \mathcal{S}} A $.

This follows immediately from Proposition 5.

#### Corollary 2 {#top-x-s1-prop-5-cor-2 .statement}

Let $ \mathcal{S}_1, \mathcal{S}_2 $ be two sets of subsets of $ X $, whose union is the same and which are such that $ \mathcal{S}_1 \subset \mathcal{S}_2 $, and let $ H $ be a subset of $ \mathcal{F}(X; Y) $. Then if $ H $ is complete with respect to $ \mathcal{S}_1 $-convergence, it is complete with respect to $ \mathcal{S}_2 $-convergence.

For every Cauchy filter with respect to $ \mathcal{G}_2 $-convergence is also a Cauchy filter with respect to $ \mathcal{G}_1 $-convergence, and we may apply Corollary 1.

#### Corollary 3 {#top-x-s1-prop-5-cor-3 .statement}

*Let $ H $ be a subset of $ \mathcal{F}(X; Y) $ such that, for each*
$$
x \notin B = \bigcup_{A \in \mathcal{G}} A,
$$
*the closure of $ H(x) $ in $ Y $ is a complete subspace of $ Y $. Then the closure $ \overline{H} $ of $ H $ in $ \mathcal{F}_{\mathcal{G}}(X; Y) $ is a complete subspace.*

Let $ \Phi $ be a Cauchy filter on $ \overline{H} $, and define a mapping $ v : X \to Y $ as follows. If $ x \in B $, $ \Phi(x) $ is a Cauchy filter on $ \overline{H(x)} $ (no. 2, Remark 6), hence by hypothesis it has at least one limit point; take $ v(x) $ to be one of these limits. If $ x \notin B $, take $ v(x) $ to be any point of $ Y $. With this definition of $ v $, it is clear that $ \Phi $ converges pointwise to $ v $ in $ B $, and $ v $ is therefore a limit of $ \Phi $ in $ \mathcal{F}_{\mathcal{G}}(X; Y) $ by Proposition 5.

In particular, if $ Y $ is complete, the hypothesis of Corollary 3 of Proposition 5 is satisfied for every $ H \subset \mathcal{F}(X; Y) $; hence:

#### Theorem 1 {#top-x-s1-thm-1 .statement}

*Let $ X $ be a set, let $ \mathcal{G} $ be a set of subsets of $ X $, and let $ Y $ be a complete uniform space. Then the uniform space $ \mathcal{F}_{\mathcal{G}}(X; Y) $ is complete.*

### 6. $ \mathcal{E} $-CONVERGENCE IN SPACES OF CONTINUOUS MAPPINGS

Let $ X, Y $ be two topological spaces, and let $ \mathcal{C}(X; Y) $ denote the set of all *continuous mappings of $ X $ into $ Y $*. If $ \mathcal{G} $ is a set of subsets of $ X $ and if $ Y $ is a uniform space, we denote by $ \mathcal{C}_{\mathcal{G}}(X; Y) $ the set $ \mathcal{C}(X; Y) $ endowed with the uniformity of $ \mathcal{G} $-convergence. In particular $ \mathcal{C}_s(X; Y), \mathcal{C}_c(X; Y) $ and $ \mathcal{C}_u(X; Y) $ denote the set $ \mathcal{C}(X; Y) $ endowed respectively with the uniformity of pointwise convergence, compact convergence and uniform convergence.

#### Proposition 6 {#top-x-s1-prop-6 .statement}

*Let $ X $ be a topological space, $ Y $ a uniform space and $ \mathcal{G} $ a set of subsets of $ X $. For each $ A \in \mathcal{G} $ and each closed entourage $ V $ of $ Y $, the traces on $ \mathcal{C}(X; Y) \times \mathcal{C}(X; Y) $ of $ W(A, V) $ and $ W(\overline{A}, V) $ are the same.*

For if $ u, v $ are continuous mappings of $ X $ into $ Y $, the mapping $ x \mapsto (u(x), v(x)) $ of $ X $ into $ Y \times Y $ is continuous, and the hypothesis that $ (u(x), v(x)) \in V $ for all $ x \in A $ therefore implies that $ (u(x), v(x)) \in \overline{V} = V $ for all $ x \in \overline{A} $ (Chapter I, § 2, no. 1, Theorem 1).

If $ \bar{\mathcal{G}} $ denotes the set of closures in $ X $ of the sets of $ \mathcal{G} $, Proposition 6 shows that, *on* $ \mathcal{C}(X; Y) $, the structures of $ \mathcal{G} $-convergence and $ \bar{\mathcal{G}} $-convergence are identical.

**G-convergence in spaces of continuous mappings**

#### Corollary {#top-x-s1-n6-cor-1 .statement}

*Let B be a dense subset of X. On $ C(X; Y) $, the structure of uniform convergence is identical with the structure of uniform convergence in B.*

#### Proposition 7 {#top-x-s1-prop-7 .statement}

*Let X be a topological space, let $ \mathfrak{S} $ be a set of subsets of X and let Y be a uniform space. If Y is Hausdorff and if the union B of the sets of $ \mathfrak{S} $ is dense in X, then $ C_{\mathfrak{S}}(X; Y) $ is Hausdorff.*

For if $(u, v)$ belongs to all the sets $W(A, V)$, where $A \in \mathfrak{S}$ and V is an entourage of Y, the hypothesis that Y is Hausdorff tells us that $u(x) = v(x)$ for all $x \in B$; if $u$ and $v$ are continuous, then $u = v$ by the principle of extension of identities (Chapter I, § 8, no. 1, Proposition 2, Corollary 1).

In particular, on $C(X; Y)$, the topology of pointwise convergence in a *dense* subset of X is Hausdorff.

#### Proposition 8 {#top-x-s1-prop-8 .statement}

*Let X be a set, $ \mathfrak{T} $ a filter on X, and let Y be a uniform space. Then the set H of mappings $u : X \to Y$ such that $u(\mathfrak{T})$ is a Cauchy filter base on Y is closed in $F_u(X; Y)$.*

Let $u_0 : X \to Y$ lie in the closure of H in $F_u(X; Y)$. For each symmetric entourage V of Y, there is a mapping $u \in H$ such that $(u_0(x), u(x)) \in V$ for all $x \in X$; on the other hand, by hypothesis there is a set $M \in \mathfrak{T}$ such that $(u(x), u(x')) \in V$ whenever $x$ and $x'$ are in M. Since $(u_0(x), u(x)) \in V$ and $(u_0(x'), u(x')) \in V$, it follows that $(u_0(x), u_0(x')) \in V$ whenever $x$ and $x'$ are in M, and therefore $u_0(\mathfrak{T})$ is a Cauchy filter base on Y.

#### Corollary 1 {#top-x-s1-prop-8-cor-1 .statement}

*Let X be a topological space and Y a uniform space. The set of mappings of X into Y which are continuous at a point $x_0 \in X$ is closed in $F_u(X; U)$.*

If V is the neighbourhood filter of $x_0$ in X, $u(x_0)$ is a cluster point of $u(V)$; hence $u$ is continuous at $x_0$ if and only if $u(V)$ is a Cauchy filter base on Y (Chapter II, § 3, no. 2, Proposition 5, Corollary 2).

#### Corollary 2 {#top-x-s1-prop-8-cor-2 .statement}

*Let X, L be two sets filtered by filters $ \mathfrak{T}, \mathfrak{G} $ respectively, and let Y be a complete uniform space. For each $ \lambda \in L $, let $u_\lambda$ be a mapping of X into Y. Suppose that (i) the family $(u_\lambda)_{\lambda \in L}$ converges uniformly in X (with respect to the filter $ \mathfrak{G} $) to a mapping $v : X \to Y$; (ii) for each $ \lambda \in L $, $u_\lambda$ has a limit $y_\lambda$ with respect to the filter $ \mathfrak{T} $. Under these conditions, v has a limit with respect to $ \mathfrak{T} $, and every limit of v with respect to $ \mathfrak{T} $ is a limit of the family $(y_\lambda)_{\lambda \in L}$ with respect to $ \mathfrak{G} $.*

For v lies in the closure of the set of the $u_\lambda$ in $F_u(X; Y)$, and therefore $v(\mathfrak{T})$ is a Cauchy filter base on Y by virtue of Proposition 8; this shows that v has a limit y with respect to $ \mathfrak{T} $ because Y is complete. Let

X' = X \cup \{ \omega \} be the topological space associated with the filter $ \mathcal{F} $ (Chapter I, § 6, no. 5), and extend $ u_\lambda $ (resp. $ v $) to a mapping $ \bar{u}_\lambda $ (resp. $ \bar{v} $) of $ X' $ into $ Y $ by putting $ \bar{u}_\lambda(\omega) = y_\lambda $ [resp. $ \bar{v}(\omega) = y $]. Then the mappings $ \bar{u}_\lambda, \bar{v} $ are continuous on $ X' $, and $ \bar{u}_\lambda $ converges uniformly in $ X $ to $ \bar{v} $ with respect to $ \mathcal{G} $; since $ X $ is dense in $ X' $, the Corollary to Proposition 6 shows that $ \bar{u}_\lambda $ converges uniformly in $ X' $ to $ \bar{v} $, and in particular that $ y = \lim_{\mathcal{G}} y_\lambda $.

#### Theorem 2 {#top-x-s1-thm-2 .statement}

*Let $ X $ be a topological space, $ Y $ a uniform space. Then the set $ C(X; Y) $ of continuous mappings of $ X $ into $ Y $ is a closed subset of the space $ F(X; Y) $ endowed with the topology of uniform convergence.*

For each $ x \in X $, the set of mappings of $ X $ into $ Y $ which are continuous at $ x $ is closed in $ F_u(X; Y) $ (Proposition 8, Corollary 1); hence the intersection $ C(X; Y) $ of these sets is also closed.

This result may be expressed in the form that the *uniform limit of continuous functions is continuous*.

#### Corollary 1 {#top-x-s1-thm-2-cor-1 .statement}

*If $ Y $ is a complete uniform space, then $ C_u(X; Y) $ is complete.*

For, by Theorem 2, $ C_u(X; Y) $ is a closed uniform subspace of the uniform space $ F_u(X; Y) $, which is complete by Theorem 1 of no. 5.

#### Corollary 2 {#top-x-s1-thm-2-cor-2 .statement}

*Let $ X $ be a topological space, $ \mathcal{S} $ a set of subsets of $ X $, and $ Y $ a uniform space. Let $ \tilde{C}_\mathcal{S}(X; Y) $ denote the set of all mappings of $ X $ into $ Y $ whose restriction to each set of $ \mathcal{S} $ is continuous. Then $ \tilde{C}_\mathcal{S}(X; Y) $ is a closed subspace of the uniform space $ F_\mathcal{S}(X; Y) $ and is complete if $ Y $ is complete.*

Suppose that $ u $ lies in the closure of $ \tilde{C}_\mathcal{S}(X; Y) $ in $ F_\mathcal{S}(X; Y) $; then (no. 2), for each $ A \in \mathcal{S} $, $ u|A $ lies in the closure of $ C(A; Y) $ in $ F_u(A; Y) $, and is therefore continuous by Theorem 2.

#### Corollary 3 {#top-x-s1-thm-2-cor-3 .statement}

*Let $ X $ be a topological space which is either metrizable or locally compact, and let $ Y $ be a uniform space. Then $ C(X; Y) $ is closed in the uniform space $ F_c(X; Y) $; if in addition $ Y $ is complete, the uniform space $ C_c(X; Y) $ is complete.*

By virtue of Corollary 2 it is enough to show that, if we take $ \mathcal{S} $ to be the set of compact subsets of $ X $, we have $ \tilde{C}_\mathcal{S}(X; Y) = C(X; Y) $ in both cases under consideration. This is clear if $ X $ is locally compact. If $ X $ is metrizable, and $ u : X \to Y $ is a mapping whose restriction to every compact subset of $ X $ is continuous, then for each $ x \in X $ and each sequence $ (z_n) $ of points of $ X $ which converges to $ x $, we have $ u(x) = \lim_{n \to \infty} u(z_n) $, and therefore $ u $ is continuous at $ x $ (Chapter IX, § 2, no. 6, Proposition 10).

Note that the argument above applies whenever every point of $ x $ has a *countable* fundamental system of neighbourhoods.

#### Remark 1 {#top-x-s1-n6-rem-1 .statement}

In general, the set $ \mathcal{C}(X; Y) $ is not closed in $ \mathcal{F}(X; Y) $ with respect to the topology of *pointwise* convergence: in other words, a pointwise limit of continuous functions is not necessarily continuous [Exercise 5 a)].

#### Remark 2 {#top-x-s1-n6-rem-2 .statement}

A filter on $ \mathcal{C}(X; Y) $ can converge *pointwise* to a *continuous* function without converging uniformly to this function.

For example, on the interval $ I = [0, 1] $, let $ u_n $ be the real-valued function which is equal to 0 for $ x = 0 $ and $ 2/n \leq x \leq 1 $, equal to 1 for $ x = 1/n $, and linear in each of the intervals $[0, 1/n]$ and $[1/n, 2/n]$. The sequence $(u_n)$ converges pointwise to 0, but does not converge uniformly to 0 in $ I $ (cf. Exercise 6).

#### Remark 3 {#top-x-s1-n6-rem-3 .statement}

If $ X $ is a uniform space, a proof analogous to that of Proposition 8 shows that the set of *uniformly continuous* mappings of $ X $ into $ Y $ is *closed* in $ \mathcal{F}_u(X; Y) $.

#### Remark 4 {#top-x-s1-n6-rem-4 .statement}

Suppose that the uniform space $ Y $ carries a commutative and associative law of composition, written additively, such that the mapping $(y, y') \to y + y'$ is continuous on $ Y \times Y $. Then, if $(u_n)$ is a sequence of continuous mappings of $ X $ into $ Y $ such that the series whose general term is $ u_n $ is *uniformly convergent* in $ X $, the sum of the series is continuous on $ X $.

We leave it to the reader to state the corresponding result for *uniformly summable* families (no. 1, Remark 5) of continuous mappings.

#### Proposition 9 {#top-x-s1-prop-9 .statement}

*Let $ X $ be a topological space, $ Y $ a uniform space. Then the mapping $(f, x) \to f(x)$ of $ \mathcal{C}_u(X; Y) \times X $ into $ Y $ is continuous.*

Let $ f_0 : X \to Y $ be a continuous mapping, let $ x_0 $ be a point of $ X $ and let $ V $ be an entourage of $ Y $. The set $ T $ of continuous mappings $ f : X \to Y $ such that $(f(x), f(x_0)) \in V$ for all $ x \in X $ is a neighbourhood of $ f_0 $ in $ \mathcal{C}_u(X; Y) $. On the other hand, since $ f_0 $ is continuous, there is a neighbourhood $ U $ of $ x_0 $ in $ X $ such that $(f_0(x), f_0(x_0)) \in V$ for all $ x \in U $. Consequently we have $(f(x), f(x_0)) \in V$ whenever $(f, x) \in T \times U$, and the result is proved.

### Exercises {#top-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
