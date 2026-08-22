---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 9
section_title: Compact spaces and locally compact spaces
lang: en
source: top-i-iv
pdf_pages: 0089-0103, 0147-0156
extraction: ocr
subsections:
    - "no": 1
      title: QUASI-COMPACT SPACES AND COMPACT SPACES
      page: 0
      pdf_page: 89
    - "no": 2
      title: REGULARITY OF A COMPACT SPACE
      page: 0
      pdf_page: 91
    - "no": 3
      title: QUASI-COMPACTS SETS; COMPACT SETS; RELATIVELY COMPACT SETS
      page: 0
      pdf_page: 91
    - "no": 4
      title: IMAGE OF A COMPACT SPACE UNDER A CONTINUOUS MAPPING
      page: 0
      pdf_page: 93
    - "no": 5
      title: PRODUCT OF COMPACT SPACES
      page: 0
      pdf_page: 94
    - "no": 6
      title: INVERSE LIMITS OF COMPACT SPACES
      page: 0
      pdf_page: 95
    - "no": 7
      title: LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 96
    - "no": 8
      title: EMBEDDING OF A LOCALLY COMPACT SPACE IN A COMPACT SPACE
      page: 0
      pdf_page: 98
    - "no": 9
      title: LOCALLY COMPACT $ \sigma $-COMPACT SPACES
      page: 0
      pdf_page: 99
    - "no": 10
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 100
statements: 50
exercises: 4
content_sha256: ea4e6b44516b83eeb3c2d7eac50490f302ca8fe98e1658cd11ee7efac69f4df3
---

## 9. COMPACT SPACES AND LOCALLY COMPACT SPACES

### 1. QUASI-COMPACT SPACES AND COMPACT SPACES

#### Definition 1 {#top-i-s9-def-1 .statement}

*A topological space* $ X $ *is said to be quasi-compact if it satisfies the following axiom*:

(C) *Every filter on* $ X $ *has at least one cluster point*.

*A topological space is said to be compact if it is quasi-compact and Hausdorff*.

It follows immediately from this axiom that if $ f $ is a mapping of a set $ Z $ into a quasi-compact space $ X $, and $ \mathfrak{F} $ is any filter on $ Z $, then $ f $ has at least one cluster point with respect to $ \mathfrak{F} $. In particular, every sequence of points of a quasi-compact space has at least one cluster point; but this condition is not equivalent to (C) (Exercise 11).

We give three axioms each of which is *equivalent to axiom* (C):

(C') *Every ultrafilter on* $ X $ *is convergent*.

(C') $ \Longrightarrow $ (C): If $ \mathfrak{F} $ is a filter on $ X $ then there is an ultrafilter finer than $ \mathfrak{F} $ (\S 6, no. 4, Theorem 1). Since this ultrafilter converges to a point $ x $, $ x $ is a cluster point of $ \mathfrak{F} $.

(C) $ \Longrightarrow $ (C'): For if an ultrafilter has a cluster point then it converges to this point (\S 7, no. 2, Corollary to Proposition 4).

If $ f $ is a mapping of a set $ Z $ into a quasi-compact space $ X $, and $ \mathfrak{U} $ is an ultrafilter on $ Z $, $ f $ has at least one limit point with respect to $ \mathfrak{U} $ (\S 6, no. 6, Proposition 10).

(C'') *Every family of closed subsets of* $ X $ *whose intersection is empty contains a finite subfamily whose intersection is empty*.

(C) $ \Longrightarrow $ (C''): Let $ \mathcal{G} $ be a family of closed subsets of $ X $ with empty intersection. If every finite subfamily of $ \mathcal{G} $ has a non-empty intersection, then $ \mathcal{G} $ generates a filter (\S 6, no. 2, Proposition 1) which has a cluster point by hypothesis. This point belongs to all the sets of $ \mathcal{G} $ (since they are closed); so we have a contradiction.

$(C'') \implies (C)$: For if $(C)$ is false then there is a filter $ \mathfrak{F} $ on $ X $ which has no cluster point; hence the closures of the sets of $ \mathfrak{F} $ form a family of closed subsets of $ X $ contradicting axiom $(C'')$.

$(C''')$ (Axiom of Borel-Lebesgue) *Every open covering of* $ X $ *contains a finite open covering of* $ X $.

$(C''') \iff (C'')$ by taking complements.

If $ X $ is quasi-compact, then every *locally finite* covering $ \mathfrak{R} $ of $ X $ is *finite*. For each point of $ X $ has an open neighbourhood which meets only a finite number of sets of $ \mathfrak{R} $, and by $(C''')$ a finite number of these neighbourhoods covers $ X $.

#### Example 1 {#top-i-s9-n1-exa-1 .statement}

Every *finite* space is *quasi-compact*, and more generally every space in which there is only a finite number of open sets is quasi-compact. A finite space is compact if and only if it is discrete, for a finite Hausdorff space is discrete ($ \S 8 $, no. 1, Corollary to Proposition 3). Conversely, *every compact discrete space is finite*, for in such a space the sets consisting of a single point are open; hence the space is finite by $(C''')$.

#### Example 2 {#top-i-s9-n1-exa-2 .statement}

Let $ X $ be a set, and give $ X $ the topology in which the closed sets are $ X $ and all finite subsets of $ X $ [this set of subsets clearly satisfies axioms $(O'_1)$ and $(O'_{II})$ of $ \S 1 $, no. 4]. The topological space so defined is *quasi-compact*. For if $(F_i)_{i \in I}$ is a family of closed subsets of $ X $ with empty intersection, then $ F_\alpha $ is finite for some $ \alpha \in I $. Let $ a_k $ ($ 1 \leq k \leq n $) be the elements of $ F_\alpha $; then by hypothesis for each index $ k $ there is an index $ i_k \in I $ such that $ a_k \notin F_{i_k} $; the intersection of the $ F_{i_k} $ ($ 1 \leq k \leq n $) and $ F_\alpha $ is therefore empty, whence axiom $(C'')$ is satisfied. If $ X $ is infinite it is not Hausdorff.

#### Remark {#top-i-s9-n1-rem-1 .statement}

Quasi-compact (non-Hausdorff) spaces are of use mainly in applications of topology to algebraic geometry and are seldom featured in other mathematical theories, where on the contrary compact spaces play an important role.

#### Theorem 1 {#top-i-s9-thm-1 .statement}

*Let* $ \mathfrak{F} $ *be a filter on a quasi-compact space* $ X $ *and let* $ A $ *be the set of cluster points of* $ \mathfrak{F} $. *Then every neighbourhood of* $ A $ *belongs to* $ \mathfrak{F} $.

Let $ V $ be a neighbourhood of $ A $ and suppose it possible that every set of $ \mathfrak{F} $ meets $ \complement V $. The intersections of the sets of $ \mathfrak{F} $ with $ \complement V $ then form a base of a filter $ \mathcal{G} $ on $ X $; $ X $ is quasi-compact, so that $ \mathcal{G} $ has at least one cluster point $ y $, which does not belong to $ A $, because the neighbourhood $ V $ of $ A $ does not meet some of the sets of $ \mathcal{G} $. But since $ \mathcal{G} $ is *finer* than $ \mathfrak{F} $, $ y $ is also a cluster point of $ \mathfrak{F} $, which is contrary to hypothesis.

#### Corollary {#top-i-s9-n1-cor-1 .statement}

For a filter on a compact space to converge it is necessary and sufficient that it has a single cluster point.

Necessity by § 8, no. 1, Proposition 1; sufficiency by Theorem 1 above.

### 2. REGULARITY OF A COMPACT SPACE

#### Proposition 1 {#top-i-s9-prop-1 .statement}

Let X be a compact space, x a point of X. In order that a filter base B formed of closed neighbourhoods of x should be a fundamental system of neighbourhoods of x it is necessary and sufficient that the intersection of the sets of B consists of x alone.

The condition is necessary since X is Hausdorff (§ 8, no. 1, Proposition 1). It is sufficient, for it signifies that x is the only cluster point of B; hence B converges to x by the Corollary to Theorem 1 of no. 1.

#### Corollary {#top-i-s9-n2-cor-1 .statement}

Every compact space is regular.

For it follows from axiom (Hi) (§ 8, no. 1, Proposition 1) that the filter base formed by all the closed neighbourhoods of an arbitrary point of the space satisfies the condition of Proposition 1.

The following proposition amplifies the Corollary to Proposition 1:

#### Proposition 2 {#top-i-s9-prop-2 .statement}

Let X be a compact space and let A, B be two disjoint closed subsets of X. Then there exist two open sets U, V, such that U ∩ V = ∅ and A ⊂ U and B ⊂ V.

Suppose the conclusion is false. If every neighbourhood U of A meets every neighbourhood V of B, then the sets U ∩ V form a filter base B on X, which therefore has a cluster point x ∈ X. Now x must lie in A, since if y is any point of X not in A there is a neighbourhood of y and a neighbourhood of A which do not intersect, since X is regular, and thus y cannot be a cluster point of B. Similarly x must lie in B and we have a contradiction.

This proposition has important consequences which will be examined in Chapter IX, § 4.

The non-Hausdorff quasi-compact space X of Example 2 of no. 1 does not satisfy axiom (O_{III}), nor a fortiori the property stated in Proposition 2, since any two non-empty open sets of this space always intersect.

### 3. QUASI-COMPACTS SETS; COMPACT SETS; RELATIVELY COMPACT SETS

#### Definition 2 {#top-i-s9-def-2 .statement}

A subset A of a topological space X is said to be a quasi-compact (resp. compact) set if the subspace A is quasi-compact (resp. compact).

A subset $ A $ of a topological space $ X $ is a quasi-compact set if and only if every covering of $ A $ by *open sets of* $ X $ contains a finite covering of $ A $; this follows from axiom $(C''')$. In a Hausdorff space, the notions of quasi-compact and compact sets are the same, since every subspace is Hausdorff.

#### Example 1 {#top-i-s9-n3-exa-1 .statement}

In a topological space $ X $, every finite subset is quasi-compact; the empty set and every set consisting of one point are compact.
2) In a topological space $ X $, let $ (x_n)_{n \in \mathbf{N}} $ be an infinite sequence of points which converges to a point $ a $; then the set $ A $ consisting of the points $ x_n $ ($ n \in \mathbf{N} $) and $ a $ is quasi-compact. For if $ (U_i) $ is a covering of $ A $ by open sets of $ X $, then $ a \in U_x $ for some index $ x $. $ U_x $ is a neighbourhood of $ a $ and therefore there is only a finite number of indices $ n_k $ such that $ x_{n_k} \notin U_x $. For each index $ k $ let $ i_k $ be an index such that $ x_{n_k} \in U_{i_k} $; then $ U_x $ and the $ U_{i_k} $ form a finite open covering of $ A $.

#### Proposition 3 {#top-i-s9-prop-3 .statement}

*Every closed subset of a quasi-compact* (resp. *compact*) *space is quasi-compact* (resp. *compact*).

This is an immediate consequence of axiom $(C'')$ if we remark that if $ A $ is closed in $ X $ then every set which is closed in $ A $ is closed in $ X $.

#### Proposition 4 {#top-i-s9-prop-4 .statement}

*Every compact subset of a Hausdorff space is closed.*

Let $ A $ be a compact subset of a Hausdorff space $ X $, and let $ x $ be any point of $ \overline{A} $; we have to show that $ x \in A $. By hypothesis, every neighbourhood of $ x $ meets $ A $, and therefore the neighbourhood filter $ \mathcal{B} $ of $ x $ in $ X $ induces a filter $ \mathcal{B}_A $ on $ A $; $ A $ is compact whence $ \mathcal{B}_A $ has a cluster point $ y \in A $. Since the filter $ \mathcal{B} $ is coarser than the filter on $ X $ generated by $ \mathcal{B}_A $ (considered as a filter base on $ X $), $ y $ is also a cluster point of $ \mathcal{B} $; hence $ y = x $, because $ \mathcal{B} $ converges to $ x $ in $ X $ and $ X $ is Hausdorff (\S 8, no. 1, Proposition 1).

#### Corollary {#top-i-s9-n3-cor-1 .statement}

*In a compact space* $ X $ *a subset* $ A $ *is compact if and only if it is closed in* $ X $.

#### Proposition 5 {#top-i-s9-prop-5 .statement}

*The union of a finite family of quasi-compact subsets of a topological space is quasi-compact.*

It is sufficient to show that if $ A $ and $ B $ are two quasi-compact subsets of a topological space $ X $, then $ A \cup B $ is quasi-compact. Let $ \mathcal{R} $ be covering of $ A \cup B $; then $ \mathcal{R} $ is a covering of $ A $ and a covering of $ B $; hence $ \mathcal{R} $ contains a finite covering $ \mathcal{R}_1 $ of $ A $ and a finite covering $ \mathcal{R}_2 $ of $ B $; $ \mathcal{R}_1 \cup \mathcal{R}_2 $ is thus a finite covering of $ A \cup B $ contained in $ \mathcal{R} $.

#### Definition 3 {#top-i-s9-def-3 .statement}

*A subset* $ A $ *of a topological space* $ X $ *is said to be relatively quasi-compact* (resp. *relatively compact*) *in* $ X $ *if* $ A $ *is contained in a quasi-compact* (resp. *compact*) *subset of* $ X $.

To abbreviate, we say also that $ A $ is a "relatively quasi-compact set" (resp. "relatively compact set") when there is no ambiguity about $ X $. In a *Hausdorff* space the notions of relatively quasi-compact set and relatively compact set are the same.

#### Proposition 6 {#top-i-s9-prop-6 .statement}

*If $ X $ is a Hausdorff space, a subset $ A $ of $ X $ is relatively compact if and only if $ \overline{A} $ is compact.*

If $ A $ is relatively compact, then $ \overline{A} $ is compact by Proposition 4 and its corollary; the reverse implication is self-evident.

#### Proposition 7 {#top-i-s9-prop-7 .statement}

*If $ A $ is a relatively quasi-compact subset of a topological space $ X $, then every filter base on $ A $ has a cluster point in $ X $.*

For if $ A \subset K $, where $ K $ is a quasi-compact subset of $ X $, then every filter base on $ A $ has a cluster point in $ K $.

The converse of this proposition is not valid without restriction on $ X $ (Exercise 22).

#### Remark {#top-i-s9-n3-rem-1 .statement}

In a non-Hausdorff space, a compact set need not be closed, and its closure need not be quasi-compact (Exercise 5); the intersection of two compact sets need not be quasi-compact (Exercise 5); the union of two compact sets need not be compact (Exercise 5).

### 4. IMAGE OF A COMPACT SPACE UNDER A CONTINUOUS MAPPING

#### Theorem 2 {#top-i-s9-thm-2 .statement}

*If $ f $ is a continuous mapping of a quasi-compact space $ X $ into a topological space $ X' $, then the set $ f(X) $ is quasi-compact.*

Let $ \mathcal{R} $ be a covering of $ f(X) $ by open sets in $ X' $; then $ \overline{f}^{-1}(\mathcal{R}) $ is an open covering of $ X $ (\S 2, no. 1, Theorem 1); hence there is a finite subset $ \mathcal{S} $ of $ \mathcal{R} $ such that $ (\mathcal{S} \overline{f}) $ is a covering of $ X $; but then $ \mathcal{S} $ is a covering of $ f(X) $ and the theorem is proved.

#### Corollary 1 {#top-i-s9-thm-2-cor-1 .statement}

*Let $ f $ be a continuous mapping of a topological space $ X $ into a Hausdorff space $ X' $. Then the image under $ f $ of any quasi-compact (resp. relatively quasi-compact) set in $ X $ is a compact (resp. relatively compact) set in $ X' $.*

#### Corollary 2 {#top-i-s9-thm-2-cor-2 .statement}

*Every continuous mapping $ f $ of a quasi-compact space $ X $ into a Hausdorff space $ X' $ is closed. If also $ f $ is bijective, then $ f $ is a homeomorphism.*

This follows immediately from Corollary 1 and Proposition 4 of no. 3.

In particular:

#### Corollary 3 {#top-i-s9-thm-2-cor-3 .statement}

*A Hausdorff topology which is coarser than the topology of a quasi-compact space must coincide with the latter.*

#### Corollary 4 {#top-i-s9-thm-2-cor-4 .statement}

*Let $ X $ be a topological space and $ R $ a Hausdorff equivalence relation on $ X $.*

a) *If there is a quasi-compact set $ K $ in $ X $ which meets every equivalence class mod $ R $, then $ X/R $ is compact and the canonical mapping of $ K/R_K $ onto $ X/R $ is a homeomorphism.*

b) *If $ K $ also meets each equivalence class in only one point, then $ K $ is a continuous section of $ X $ with respect to the relation $ R $* (\$ 3, no. 5).

Let $ f $ be the restriction to $ K $ of the canonical mapping $ X \to X/R $. Since $ X/R $ is Hausdorff it follows from Corollary 1 that $ X/R $ is compact and from Corollary 2 that $ f $ is closed; hence the bijection $ K/R_K \to X/R $ associated with $ f $ is a homeomorphism (\$ 5, no. 2, Proposition 3). This deals with a); b) follows immediately, since we now have $ K/R_K = K $.

### 5. PRODUCT OF COMPACT SPACES

#### Theorem 3 (Tychonoff) {#top-i-s9-thm-3 .statement}

*Every product of quasi-compact (resp. compact) spaces is quasi-compact (resp. compact). Conversely, if a product of non-empty spaces is quasi-compact (resp. compact) then each of the factors is quasi-compact (resp. compact).*

In view of the characterization of Hausdorff product spaces given in \$ 8, no. 2, Proposition 7 it is enough to prove the assertions for quasi-compact spaces. If $ X = \prod_{i \in I} X_i $ is quasi-compact and non-empty, then $ X_i = \operatorname{pr}_i(X) $ is quasi-compact by reason of Theorem 2 of no. 4. Conversely, suppose the $ X_i $ are quasi-compact and let $ \mathcal{U} $ be an ultrafilter on $ X $; then for each $ i \in I $, $ \operatorname{pr}_i(\mathcal{U}) $ is an ultrafilter base on $ X_i $ (\$ 6, no. 6, Proposition 10) which therefore converges by reason of axiom (C'); hence $ \mathcal{U} $ is convergent (\$ 7, no. 6, Corollary 1 of Proposition 10) and therefore $ X $ is quasi-compact.

#### Corollary {#top-i-s9-n5-cor-1 .statement}

*For a subset of a product of topological spaces to be relatively quasi-compact it is necessary and sufficient that each of its projections should be relatively quasi-compact in the corresponding factor.*

Necessity follows from Theorem 2 of \$ 4. To prove sufficiency, let $ A $ be a subset of $ \prod_i X_i $ such that, for each index $ i $, $ \operatorname{pr}_i(A) $ is contained in a quasi-compact subset $ K_i $ of $ X_i $; then $ A $ is contained in the quasi-compact subset $ \prod_i K_i $ of $ \prod_i X_i $.

### 6. INVERSE LIMITS OF COMPACT SPACES

#### Proposition 8 {#top-i-s9-prop-8 .statement}

Let $(X_\alpha, f_{\alpha\beta})$ be an inverse system of compact spaces indexed by a directed set $I$ such that $f_{\alpha\alpha}$ is the identity mapping for each $\alpha \in I$. Let $X = \varprojlim X_\alpha$ be the inverse limit and $f_\alpha : X \to X_\alpha$ the canonical mapping (\S 4, no. 4). Then
a) $X$ is compact and for each $\alpha \in I$ we have
$$
f_\alpha(X) = \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta).
$$
b) *If the* $X_\alpha$ *are all non-empty then* $X$ *is non-empty*.

$X$ is a closed subspace of $\prod_\alpha X_\alpha$ (\S 8, no. 2, Proposition 7, Corollary 2) which is compact by Theorem 3 of no. 5 and Proposition 3 of no. 3. The other assertions are consequences of *Set Theory*, chap. III, \S 7, no. 4, th. 1. We apply this theorem by taking $\mathcal{S}_\alpha$ to be the set of closed subsets of $X_\alpha$. The conditions (i) and (ii) are just axioms $(O'_1)$ and $(C'')$ respectively; condition (iii) is satisfied since $\{x_\alpha\}$ is closed and $f_{\alpha\beta}$ continuous (\S 2, no. 1, Theorem 1), and lastly condition (iv) is satisfied by reason of Corollary 2 of Theorem 2 of no. 4.

#### Corollary 1 {#top-i-s9-prop-8-cor-1 .statement}

*Let* $(X_\alpha, f_{\alpha\beta})$ *be an inverse system of topological spaces indexed by a directed set, such that for each pair of indices* $\alpha, \beta$ *for which* $\alpha \leq \beta$ *and for each* $x_\alpha \in X_\alpha$, $\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$ *is compact*. *Then equation (1) is valid and* $\overline{f}_{\alpha}^{-1}(x_\alpha)$ *is compact for each index* $\alpha$ *and each* $x_\alpha \in X_\alpha$.

For each $x_\alpha \in \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta)$ and each $\beta \geq \alpha$, let $L_\beta$ denote $\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$. If $\alpha \leq \beta \leq \gamma$, then we have $f_{\beta\gamma}(L_\gamma) \subset L_\beta$ and the set of all indices $\beta \geq \alpha$ is cofinal in the index set. It follows immediately that the $L_\beta$ ($\beta \geq \alpha$) form an inverse system of topological spaces (with the restrictions of the $f_{\beta\gamma}$ as mappings), whose inverse limit $L$ is homeomorphic to $\overline{f}_{\alpha}^{-1}(x_\alpha)$. Since by hypothesis the $L_\beta$ are compact and not empty, the corollary follows from Proposition 8.

#### Corollary 2 {#top-i-s9-prop-8-cor-2 .statement}

*Let* $(X_\alpha, f_{\alpha\beta})$ *and* $(X'_\alpha, f'_{\alpha\beta})$ *be two inverse systems of topological spaces indexed by the same directed set* $I$, *and let* $(u_\alpha)$ *be an inverse system of mappings* $u_\alpha : X_\alpha \to X'_\alpha$. *Let* $X = \varprojlim X_\alpha$, $X' = \varprojlim X'_\alpha$, $u = \varprojlim u_\alpha$. *Then*:
a) *If* $x' = (x'_\alpha) \in X'$ *is such that* $\overline{u'}_{\alpha}^{-1}(x'_\alpha)$ *is compact and non-empty for each* $\alpha \in I$, *then* $\overline{u}^{-1}(x')$ *is compact and non-empty*.

b) *If the $ X_\alpha $ are compact, the $ X'_\alpha $ Hausdorff and the $ u_\alpha $ surjective and continuous, then $ u $ is surjective.*

Let $ L_\alpha $ denote $ \overline{u}_\alpha^{-1}(x'_\alpha) $; then clearly the $ L_\alpha $ form an inverse system of topological spaces (with the restrictions of the $ f_{\alpha\beta} $ as maps) and $ \overline{u}^{-1}(x' = L) $ is the inverse limit of the $ L_\alpha $; assertion a) therefore follows from Proposition 8. Assertion b) is an immediate consequence, in view of Proposition 3 of no. 3.

### 7. LOCALLY COMPACT SPACES

#### Definition 4 {#top-i-s9-def-4 .statement}

*A topological space $ X $ is said to be locally compact if it is Hausdorff and if every point of $ X $ has a compact neighbourhood.*

Clearly a compact space is locally compact, but the converse is false; for example, every *discrete* space is locally compact, but not compact if *infinite*.

\* As we shall see in Chapter IV, § 2, the real line $ \mathbf{R} $ is locally compact, but not compact. \*

#### Proposition 9 {#top-i-s9-prop-9 .statement}

*Every locally compact space is regular.*

Let $ X $ be a locally compact space, then every point $ x \in X $ has a compact neighbourhood $ V $; since $ X $ is Hausdorff, $ V $ is closed (no. 3, Proposition 4). On the other hand, $ V $ is a regular subspace of $ X $ (no. 2, Corollary to Proposition 1) and therefore $ X $ is regular (\S 8, no. 4, Proposition 13).

#### Corollary {#top-i-s9-n7-cor-1 .statement}

*In a locally compact space every point has a fundamental system of compact neighbourhoods.*

For the intersection of a closed neighbourhood of $ x $ and a compact neighbourhood of $ x $ is a compact neighbourhood of $ x $ (no. 3, Proposition 3).

There exist *non-Hausdorff* topological spaces in which every point has a fundamental system of compact neighbourhoods (Exercise 5).

The Corollary to Proposition 9 may be generalized as follows:

#### Proposition 10 {#top-i-s9-prop-10 .statement}

*In a locally compact space $ X $, every compact set $ K $ has a fundamental system of compact neighbourhoods.*

Let $ U $ be any neighbourhood of $ K $. For each $ x \in K $ there is a compact neighbourhood $ W(x) $ of $ x $ contained in $ U $. The interiors of the sets

W(x) form an open covering of K as x runs through K; hence there exist a finite number of points $ x_i \in K $ ($ 1 \leq i \leq n $) such that the interiors of the W(x_i) cover K. The union V of the W(x_i) is therefore a compact neighbourhood of K contained in U (no. 3, Proposition 5).

#### Proposition 11 {#top-i-s9-prop-11 .statement}

*Let X be a locally compact space and F a subset of X such that F \cap K is compact whenever K is a compact subset of X. Then F is closed in X.*

In view of Proposition 4 of no. 3, this follows from Proposition 3 a) of § 3, no. 1.

#### Proposition 12 {#top-i-s9-prop-12 .statement}

*In a Hausdorff space X, every locally compact subspace A is locally closed.*

By hypothesis, for every $ x \in A $ there is a neighbourhood V of x in X such that $ V \cap A $ is compact and therefore closed in V (no. 3, Proposition 4).

#### Proposition 13 {#top-i-s9-prop-13 .statement}

*Every locally closed subspace of a locally compact space X is locally compact.*

Let A be a locally closed subspace of X; then for each $ x \in A $ there is a neighbourhood U of x in X such that $ U \cap A $ is closed in U. Let $ V \subset U $ be a compact neighbourhood of x in X; $ V \cap A = V \cap (U \cap A) $ is closed in V and therefore compact (no. 3, Proposition 3). Since $ V \cap A $ is a neighbourhood of x in A, the result is proved (it is clear that A is Hausdorff).

Theorem 1 (no. 1) and Corollary 2 of Theorem 2 (no. 4) *do not extend* to locally compact spaces which are not compact.

For example, in an infinite discrete space X, the filter consisting of those sets which contain a given point $ x \in X $ and have a finite complement has x as its only cluster point but does not converge to x. Since any mapping f of X into a Hausdorff space X' is continuous, the image under f of an arbitrary subset of X (which is closed in X, since X is discrete) will not in general be a closed subset of X'.

The proposition corresponding to Theorem 3 of no. 5 is the following:

#### Proposition 14 {#top-i-s9-prop-14 .statement}

a) *Let $ (X_i)_{i \in I} $ be a family of locally compact spaces such that $ X_i $ is compact for all but a finite number of indices. Then the product space $ X = \prod_{i \in I} X_i $ is locally compact.*

b) *Conversely, if the product of a family $ (X_i)_{i \in I} $ of non-empty topological spaces is locally compact, then the factors $ X_i $ are compact for all but a finite number of indices, and the factors which are not compact are locally compact.*

b) If $ X = \prod_{i \in I} X_i $ is locally compact and the $ X_i $ non-empty, then each of the $ X_i $ is homeomorphic to a closed subspace of $ X $ ($ \S 4 $, no. 2, Proposition 4 and $ \S 4 $, no. 3, Corollary to Proposition 7), hence locally compact by Proposition 13. Let $ a = (a_i) $ be a point of $ X $ and let $ V $ be a compact neighbourhood of $ a $; since we have $ \operatorname{pr}_i V = X_i $ for all but a finite number of indices ($ \S 4 $, no. 1), it follows from no. 4, Corollary 1 to Theorem 2, that the $ X_i $ are compact except for a finite number of indices.

### 8. EMBEDDING OF A LOCALLY COMPACT SPACE IN A COMPACT SPACE

#### Theorem 4 (Alexandroff) {#top-i-s9-thm-4 .statement}

*If $ X $ is any locally compact space, there exists a compact space $ X' $ and a homeomorphism $ f $ of $ X $ onto the complement of a point in $ X' $. Furthermore, if $ X'_1 $ is another compact space such that there is a homeomorphism $ f_1 $ of $ X $ onto the complement of a point in $ X'_1 $, then there is a unique homeomorphism $ g $ of $ X' $ onto $ X'_1 $ such that $ f_1 = g \circ f $.*

Let us begin by proving the second assertion of the theorem. Let
$$
f(X) = X' - \{ \omega \} \quad \text{and} \quad f_1(X) = X'_1 - \{ \omega_1 \}.
$$
If the homeomorphism $ g $ exists it must be unique, for by definition we have $ g(x') = f_1(\overline{f}(x')) $ if $ x' \neq \omega $ and therefore $ g(\omega) = \omega_1 $. It remains to show that the bijection $ g : X' \to X'_1 $ thus defined is bicontinuous; since $ X' $ and $ X'_1 $ are interchangeable we need only show that the image under $ g $ of a neighbourhood of a point $ x' \in X' $ is a neighbourhood of $ g(x') $ in $ X'_1 $. This is obvious from the definition of $ g $ if $ x' \neq \omega $. If $ x' = \omega $, let $ V' $ be an open neighbourhood of $ \omega $ in $ X' $; then $ X' - V' = K $ is closed in $ X' $ and therefore compact (no. 3, Proposition 3) and is contained in $ f(X) $; hence $ g(K) = f_1(\overline{f}(K)) $ is compact (no. 4, Theorem 2, Corollary 1). It follows that $ g(V') = X'_1 - g(K) $ is an open neighbourhood of $ \omega_1 $ (no. 3, Proposition 4). Hence $ g $ is a homeomorphism.

To prove the first part of the theorem, let $ X' $ be a set which is the sum of $ X $ and a set consisting of a single point $ \omega $. We define a topology on $ X' $ by taking the set $ \mathcal{O} $ of open subsets of $ X' $ to consist of all open subsets of $ X $ and all subsets of the form $ (X - K) \cup \{ \omega \} $, where $ K $ is a compact subset of $ X $. Since any intersection of compact subsets of $ X $ is compact (no. 3, Propositions 3 and 4) and since any closed subset of a compact set is compact (no. 3, Proposition 3), it follows that $ \mathfrak{D} $ satisfies axiom $(O_I)$; and since any finite union of compact subsets of $ X $ is compact (no. 3, Proposition 5), $ \mathfrak{D} $ also satisfies $(O_{II})$. Every compact subset of $ X $ is closed in $ X $ (no. 3, Proposition 4) and therefore the topology induced on $ X $ by that of $ X' $ is the original topology on $ X $. Thus it remains to show that $ X' $ is compact. In the first place, $ X' $ is *Hausdorff*. For if $ x, y $ are any two distinct points of $ X $, they have disjoint open neighbourhoods $ V, W $ respectively in $ X $, and $ V, W $ are open in $ X' $; on the other hand each $ x \in X $ has a compact neighbourhood $ K $ in $ X $, which is also a neighbourhood of $ x $ in $ X' $, while

$$
(X - K) \cup \{ \omega \}
$$

is a neighbourhood of $ \omega $ in $ X' $ and manifestly does not meet $ K $. Finally, $ X' $ is *quasi-compact*. Let $ (U_\lambda)_{\lambda \in L} $ be an open covering of $ X' $; then for at least one index $ \mu \in L $ we have $ U_\mu = (X - K_\mu) \cup \{ \omega \} $ where $ K_\mu $ is a compact subset of $ X $. Hence there is a finite subset $ H $ of $ L $ such that the sets $ U_\lambda $ (for $ \lambda \in H $) cover $ K_\mu $; if $ J = H \cup \{ \mu \} $, then $ (U_\lambda)_{\lambda \in J} $ is a finite open covering of $ X' $, and the proof is complete.

Notice that if $ X $ is already *compact*, then $ \omega $ is an *isolated* point of the compact space $ X' $; hence $ X' $ is the *sum* ($ \S $ 2, no. 4, Example 3) of the space $ X $ and the space $ \{ \omega \} $.

When a compact space $ X' $ has been constructed as above from a locally compact space $ X $ by adjoining an element $ \omega $, it is often said that $ \omega $ is the "point at infinity" of $ X' $, and that $ X' $ is obtained from $ X $ by adjoining a point at infinity. $ X' $ is also called the *Alexandroff compactification* or the *one-point compactification* of the locally compact space $ X $.

\* Example. If we apply Alexandroff's theorem to the real plane $ \mathbf{R}^2 $, we get a compact space homeomorphic to the sphere $ S_2 $ whose equation is $ x_1^2 + x_2^2 + x_3^2 = 1 $ in $ \mathbf{R}^3 $. A homeomorphism of these two spaces may be described as follows: the point $ \omega $ (the point at infinity) adjoined to $ \mathbf{R}^2 $ is mapped to $ (0, 0, 1) \in S_2 $, and every point $ (x_1, x_2) $ of $ \mathbf{R}^2 $ is mapped to the point where the line joining the points $ (0, 1, 1) $ and $ (x_1, x_2, 0) $ in $ \mathbf{R}^3 $ meets $ S_2 $ again. This homeomorphism is known as *stereographic projection*.

### 9. LOCALLY COMPACT $ \sigma $-COMPACT SPACES

#### Definition 5 {#top-i-s9-def-5 .statement}

*A locally compact space $ X $ is said to be $ \sigma $-compact or countable at infinity if it is a countable union of compact subsets.*

#### Example 1 {#top-i-s9-n9-exa-1 .statement}

A discrete space is $ \sigma $-compact if and only if it is countable.
\* 2) The real line $ \mathbf{R} $ is locally compact and $ \sigma $-compact, since it is the union of the compact intervals $[ -n, +n ]$ for $ n \in \mathbf{N} $. \*

#### Remark {#top-i-s9-n9-rem-1 .statement}

A Hausdorff space can be a countable union of compact subspaces without being locally compact. \* An example is Hilbert space with the weak topology, as we shall show in a later volume.

#### Proposition 15 {#top-i-s9-prop-15 .statement}

*If $ X $ is a locally compact $ \sigma $-compact space, there is a sequence $ (U_n) $ of relatively compact open subsets of $ X $ which cover $ X $, such that $ \overline{U}_n \subset U_{n+1} $ for each $ n $.

Let $ X $ be the union of a sequence $ (K_n) $ of compact sets. Let $ U_1 $ be a relatively compact open neighbourhood of $ K_1 $ (no. 7, Proposition 10) and define $ U_n $ inductively for $ n > 1 $ to be a relatively compact open neighbourhood of $ \overline{U}_{n-1} \in K_n $ (no. 3, Proposition 5; no. 7, Proposition 10). The sequence $ (U_n) $ clearly has the required properties.

#### Corollary 1 {#top-i-s9-prop-15-cor-1 .statement}

*With the notation of Proposition 15, every compact subset $ K $ of $ X $ is contained in some $ U_n $.

For $ K $ can be covered by a finite number of the $ U_k $, by axiom (C''').

#### Corollary 2 {#top-i-s9-prop-15-cor-2 .statement}

*Let $ X $ be a locally compact space and let $ X' $ be the compact space obtained by adjoining a point at infinity $ \omega $ to $ X $ (no. 8). Then $ X $ is $ \sigma $-compact if and only if the point $ \omega $ has a countable fundamental system of neighbourhoods in $ X' $.

If $ X $ is $ \sigma $-compact we can construct a sequence of subsets $ U_n $ of $ X $ as in Proposition 15, and the neighbourhoods $ X' - \overline{U}_n $ of $ \omega $ in $ X' $ form a fundamental system of neighbourhoods of $ \omega $ by reason of Corollary 1. The converse follows from the fact that the complements of open neighbourhoods of $ \omega $ are compact subsets of $ X $.

Clearly every closed subspace of a locally compact $ \sigma $-compact space is locally compact and $ \sigma $-compact. Likewise any finite product of locally compact $ \sigma $-compact spaces is locally compact and $ \sigma $-compact.

Notice, however, that an open subspace of a compact space need not be $ \sigma $-compact, as Alexandroff's theorem (no. 8, Theorem 4) shows.

### 10. PARACOMPACT SPACES

#### Definition 6 {#top-i-s9-def-6 .statement}

*A topological space is said to be paracompact if it is Hausdorff and satisfies the following axiom:

(PC) *Every open covering $ \mathcal{R} $ of $ X $ has a locally finite open refinement $ \mathcal{R}' $.*
(Set Theory, Chapter II, § 4, no. 6, Definition 5).

Every *compact* space is clearly paracompact. Every *discrete* space $ X $ is paracompact, for the open covering formed by all sets consisting of a single point of $ X $ is locally finite and is finer than every open covering of $ X $.

#### Proposition 16 {#top-i-s9-prop-16 .statement}

*Every closed subspace* $ F $ *of a paracompact space* $ X $ *is paracompact*.

Certainly $ F $ is Hausdorff. On the other hand, if $ (V_i) $ is an open covering in the subspace $ F $, then each $ V_i $ is of the form $ V_i = U_i \cap F $, where $ U_i $ is open in $ X $. Consider the open covering $ \mathcal{R} $ of $ X $ formed by $ CF $ and the $ U_i $; since $ X $ is paracompact, $ \mathcal{R} $ has a locally finite refinement $ \mathcal{R}' $, and the intersections with $ F $ of the sets belonging to $ \mathcal{R}' $ form a locally finite open covering of $ F $ which is finer than the given covering $ (V_i) $.

On the other hand an open subspace of a compact space need not be paracompact (Exercise 11).

#### Proposition 17 {#top-i-s9-prop-17 .statement}

*The product of a paracompact space and a compact space is paracompact*.

Let $ X $ be a paracompact space, $ Y $ a compact space, $ \mathcal{R} $ an open covering of $ X \times Y $. For each $ (x, y) \in X \times Y $ there is an open neighbourhood $ V(x, y) $ of $ x $ in $ X $ and an open neighbourhood $ W(x, y) $ of $ y $ in $ Y $ such that $ V(x, y) \times W(x, y) $ is contained in some set belonging to $ \mathcal{R} $. For each $ x \in X $, the sets $ W(x, y) $ as $ y $ runs through $ Y $ form an open covering of $ Y $; hence there exist a finite number of points
$$
y_i \in Y \quad (1 \leq i \leq n(x))
$$
such that the $ W(x, y_i) $ cover $ Y $. Let $ U(x) $ denote
$$
\bigcap_{i=1}^{n(x)} V(x, y_i);
$$
then each of the open sets $ U(x) \times W(x, y_i) $ is contained in a set of $ \mathcal{R} $. Now let $ (T_i)_{i \in I} $ be a locally finite open covering of $ X $ which refines the covering $ (U(x))_{x \in X} $. For each $ i \in I $, let $ x_i $ be a point of $ X $ such that $ T_i \subset U(x_i) $, and let us denote by $ S_{i, k} $ the sets $ W(x_i, y_k) $ corresponding to this point $ x_i $ ($ 1 \leq k \leq n(x_i) $). Clearly the sets
$$
T_i \times S_{i, k} \quad (i \in I, \ 1 \leq k \leq n(x_i) \text{ for each } i \in I)
$$
form an open covering of $ X \times Y $ which refines $ \mathcal{R} $, and the proof will be complete if we show that this covering is locally finite. Let $ (x, y) $ be any point of $ X \times Y $; there is a neighbourhood $ Q $ of $ x $ which meets only a finite number of sets $ T_i $, and therefore the neighbourhood $ Q \times Y $ of $ (x, y) $ meets only a finite number of sets $ T_i \times S_{i, k} $.

#### Proposition 18 {#top-i-s9-prop-18 .statement}

*The sum* (\S 2, no. 4, Example 3) *of a family* $(X_i)_{i \in I}$ *of paracompact spaces is paracompact*.

Let $X$ be the sum of the $X_i$, and let $(V_\lambda)_{\lambda \in L}$ be an open covering of $X$. The covering formed by the open sets $X_i \cap Y_\lambda$ is finer than $(V_\lambda)$. For each $i \in I$, let $(U_{i,\mu})_{\mu \in M_i}$ be a locally finite open refinement of the covering $(V_\lambda \cap X_i)_{\lambda \in L}$; then the open covering of $X$ formed by the

$$
U_{i,\mu} \quad (i \in I, \ \mu \in M_i \text{ for each } i \in I)
$$

is locally finite and refines the original covering $(V_\lambda)$.

#### Theorem 5 {#top-i-s9-thm-5 .statement}

*A locally compact space* $X$ *is paracompact if and only if* $X$ *is the sum of a family of locally compact $\sigma$-compact spaces*.

Suppose $X$ is paracompact, and for each $x \in X$ let $V_x$ be a relatively compact open neighbourhood of $x$ in $X$. Then by hypothesis there exists a locally finite open covering $(U(\alpha))_{\alpha \in A}$ of $X$ which refines the covering $(V_x)_{x \in X}$. The $U(\alpha)$ are therefore relatively compact. Every compact subset $K$ of $X$ meets only a finite number of the sets $U(\alpha)$, for the non-empty sets $U(\alpha) \cap K$ form a locally finite open covering of the compact space $X$; hence they must be finite in number (no. 1). Now let $R$ be the following relation between two points $x, y$ of $X$: "there exists a finite sequence $(\alpha_i)_{1 \leq i \leq n}$ of indices in $A$ such that $x \in U(\alpha_1), \ y \in U(\alpha_n)$ and $U(\alpha_i)$ meets $U(\alpha_{i+1})$ for $1 \leq i \leq n - 1$".

It is immediately verified that $R$ is an equivalence relation, and that each equivalence class mod $R$ is an *open* subset of $X$ [since the $U(\alpha)$ are open sets]. $X$ is therefore the *sum* of the locally compact subspaces (no. 7, Proposition 13) formed by the equivalence classes mod $R$, and it remains to show that each of these subspaces is the union of a *countable* subfamily of the family $(U(\alpha))$.

Let $x$ be any point of $X$, and define a sequence $(C_n)$ of relatively compact open subsets of $X$ by induction on $n$ as follows; $C_1$ is the union of the sets $U(\alpha)$ which contain $x$, and for each $n > 1$, $C_n$ is the union of the sets $U(\alpha)$ which meet $C_{n-1}$. It is immediately verified by induction on $n$ that each of the $C_n$ is relatively compact and is the union of a *finite* number of sets $U(\alpha)$. Furthermore, the equivalence class of $x$ with respect to $R$ is the *union* of the $C_n$: for if $(\alpha_i)_{1 \leq i \leq n}$ is a sequence of indices such that $x \in U(\alpha_1)$ and $U(\alpha_i)$ meets $U(\alpha_{i+1})$ for $1 \leq i \leq n - 1$, then one sees by induction on $i$ that $U(\alpha_i) \subset C_i$ for $1 \leq i \leq n$. It follows that the equivalence classes mod $R$ are $\sigma$-compact, and this completes the proof of the first part of the theorem.

To prove the converse, we may assume (by Proposition 18) that $ X $ is $ \sigma $-compact. Let $ \mathcal{H} = (G_\lambda)_{\lambda \in L} $ be any open covering of $ X $, and let $ (U_n) $ be a sequence of relatively compact open sets in $ X $ which have the properties stated in Proposition 15 of no. 9. Let $ K_n $ denote the compact set $ \overline{U}_n - U_{n-1} $ ($ U_n = \emptyset $ if $ n \leq 0 $). The open set $ U_{n+1} - \overline{U}_{n-2} $ is a neighbourhood of $ K_n $ by construction; hence for each $ x \in K_n $ there is a neighbourhood $ W_x $ of $ x $ contained in one of the sets $ G_\lambda $ and contained also in $ U_{n+1} - \overline{U}_{n-2} $. Since $ K_n $ is compact, a finite number of the sets $ W_x $ cover $ K_n $; let $ H_{ni} (1 \leq i \leq p_n) $ be these sets. Then the family $ \mathcal{H}' $ of sets $ H_{ni} (n \geq 1, 1 \leq i \leq p_n \text{ for each } n) $ is an open covering of $ X $ which refines $ \mathcal{H} $, and hence to complete the proof we have to show that $ \mathcal{H}' $ is *locally finite*. Let $ z $ be any point of $ X $, $ n $ the smallest integer such that $ z \in U_n $; then since $ z \notin U_{n-1} $, there is a neighbourhood $ T $ of $ z $ which is contained in $ U_n $ and does not meet $ U_{n-2} $. It follows that $ T $ meets only those sets $ H_{mi} $ for which $ n - 2 \leq m \leq n + 1 $, i.e. $ T $ meets only a finite number of sets of $ \mathcal{H}' $.

In the course of the proof we have also established the following result:

#### Corollary {#top-i-s9-n10-cor-1 .statement}

*Let $ X $ be a locally compact paracompact space. Then every open covering $ \mathcal{H} $ of $ X $ has a locally finite open refinement $ \mathcal{H}' $ formed of relatively compact sets. If $ X $ is $ \sigma $-compact then $ \mathcal{H}' $ can be taken to be countable.*

### Exercises {#top-i-s9-exercises}

See the [exercises for § 9](exercises/s9/).
