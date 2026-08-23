---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 8
section_title: Hausdorff spaces and regular spaces
lang: en
source: top-i-iv
pdf_pages: 0081-0089, 0140-0147
extraction: ocr
subsections:
    - "no": 1
      title: HAUSDORFF SPACES
      page: 0
      pdf_page: 81
    - "no": 2
      title: SUBSPACES AND PRODUCTS OF HAUSDORFF SPACES
      page: 0
      pdf_page: 83
    - "no": 3
      title: HAUSDORFF QUOTIENT SPACES
      page: 0
      pdf_page: 84
    - "no": 4
      title: REGULAR SPACES
      page: 0
      pdf_page: 86
    - "no": 5
      title: EXTENSION BY CONTINUITY; DOUBLE LIMIT
      page: 0
      pdf_page: 87
    - "no": 6
      title: EQUIVALENCE RELATIONS ON A REGULAR SPACE
      page: 0
      pdf_page: 88
statements: 28
exercises: 24
content_sha256: 5be2c158ce26c70a533de7a2831009bf912d2b3aabc5a32fe8dabbb703de423d
---

## 8. HAUSDORFF SPACES AND REGULAR SPACES

### 1. HAUSDORFF SPACES

#### Proposition 1 {#top-i-s8-prop-1 .statement}

Let $ X $ be a topological space. Then the following statements are equivalent:

(H) Any two distinct points of $ X $ have disjoint neighbourhoods.
(Hi) The intersection of the closed neighbourhoods of any point of $ X $ consists of that point alone.
(Hii) The diagonal of the product space $ X \times X $ is a closed set.
(Hiii) For every set $ I $, the diagonal of the product space $ Y = X^I $ is closed in $ Y $.
(Hiv) No filter on $ X $ has more than one limit point.
(Hv) If a filter $ \mathfrak{F} $ on $ X $ converges to $ x $, then $ x $ is the only cluster point of $ \mathfrak{F} $.

We shall prove the implications

$$
\begin{array}{cccccc}
(H) & \Longrightarrow & (Hi) & \Longrightarrow & (Hv) & \Longrightarrow (Hiv) \Longrightarrow (H)
\\
(H) & \Longrightarrow & (Hiii) & \Longrightarrow & (Hii) & \Longrightarrow (H).
\end{array}
$$

and

(H) $ \Longrightarrow $ (Hi): If $ x \neq y $ there is an open neighbourhood $ U $ of $ x $ and an open neighbourhood $ V $ of $ y $ such that $ U \cap V = \varnothing $; hence $ y \notin \overline{U} $.

(Hi) $ \Longrightarrow $ (Hv): Let $ y \neq x $; then there is a closed neighbourhood $ V $ of $ x $ such that $ y \notin V $, and by hypothesis there exists $ M \in \mathfrak{F} $ such that $ M \subset V $; thus $ M \cap C_V = \varnothing $. But $ C_V $ is a neighbourhood of $ y $; hence $ y $ is not a cluster point of $ \mathfrak{F} $.

(Hv) $ \Longrightarrow $ (Hiv): Clear, since every limit point of a filter is also a cluster point.

(Hiv) $ \Longrightarrow $ (H): Suppose $ x \neq y $ and that every neighbourhood $ V $ of $ x $ meets every neighbourhood $ W $ of $ y $. Then the sets $ V \cap W $ form a base of a filter which has both $ x $ and $ y $ as limit points, which is contrary to hypothesis.

(H) $ \Longrightarrow $ (Hiii): Let $ (x) = (x_i) $ be a point of $ X^I $ which does not belong to the diagonal $ \Delta $. Then there are at least two indices $ \lambda, \mu $ such that $ x_\lambda \neq x_\mu $. Let $ V_\lambda $ (resp. $ V_\mu $) be a neighbourhood of $ x_\lambda $ (resp. $ x_\mu $) in $ X $, such that $ V_\lambda \cap V_\mu = \varnothing $; then the set $ W = V_\lambda \times V_\mu \times \prod_{i \neq \lambda, \mu} X_i $ (where $ X_i = X $ if $ i \neq \lambda, \mu $) is a neighbourhood of $ x $ in $ X^I $ (\S 4, no. 1) which does not meet $ \Delta $. Hence $ \Delta $ is closed in $ X^I $.

(Hiii) $ \Longrightarrow $ (Hii): Obvious.

(Hii) $ \Longrightarrow $ (H): If $ x \neq y $ then $ (x, y) \in X \times X $ is not in the diagonal $ \Delta $, hence (\$ 4, no. 1) there is a neighbourhood $ V $ of $ x $ and a neighbourhood $ W $ of $ y $ in $ X $ such that $ (V \times W) \cap \Delta = \varnothing $, which means that
$$
V \cap W = \varnothing.
$$

#### Definition 1 {#top-i-s8-def-1 .statement}

*A topological space satisfying the conditions of Proposition 1 is called a Hausdorff or separated space; the topology of such a space is said to be a Hausdorff topology.*

Axiom (H) is *Hausdorff’s axiom*.

#### Example {#top-i-s8-n1-exa-1 .statement}

Any discrete space is Hausdorff. The rational line $ Q $ is Hausdorff, for if $ x, y $ are two rational numbers such that $ x < y $ then there is a rational number $ z $ such that $ x < z < y $, and the neighbourhoods ]$ \leftarrow, z[ $ of $ x $ and ]$ z, \rightarrow[ $ of $ y $ do not intersect.

A set $ X $ having at least two points and carrying the coarsest topology (\$ 2, no. 2) is not a Hausdorff space.

Let $ f : X \to Y $ be a mapping of a set $ X $ into a *Hausdorff* space $ Y $; then it follows immediately from Proposition 1 that $ f $ can have *at most one limit* with respect to a filter $ \mathfrak{F} $ on $ X $, and that if $ f $ has $ y $ as a limit with respect to $ \mathfrak{F} $, then $ y $ is *the only cluster point* of $ f $ with respect to $ \mathfrak{F} $.

#### Proposition 2 {#top-i-s8-prop-2 .statement}

*Let $ f, g $ be two continuous mappings of a topological space $ X $ into a Hausdorff space $ Y $; then the set of all $ x \in X $ such that $ f(x) = g(x) $ is closed in $ X $.*

For this set is the inverse image of the diagonal of $ Y \times Y $ under the mapping $ x \mapsto (f(x), g(x)) $, which is continuous (\$ 4, no. 1, Proposition 1). The result therefore follows from (Hii) and \$ 2, no. 1, Theorem 1.

#### Corollary 1 (Principle of extension of identities) {#top-i-s8-prop-2-cor-1 .statement}

*Let $ f, g $ be two continuous mappings of a topological space $ X $ into a Hausdorff space $ Y $. If $ f(x) = g(x) $ at all points of a dense subset of $ X $, then $ f = g $.*

In other words, a continuous map of $ X $ into $ Y $ (Hausdorff) is uniquely determined by its values at all points of a dense subset of $ X $.

#### Corollary 2 {#top-i-s8-prop-2-cor-2 .statement}

*If $ f $ is a continuous mapping of a topological space $ X $ into a Hausdorff space $ Y $, then the graph of $ f $ is closed in $ X \times Y $.*

For this graph is the set of all $ (x, y) \in X \times Y $ such that $ f(x) = y $, and the two mappings $ (x, y) \to y $ and $ (x, y) \to f(x) $ are continuous.

#### Proposition 3 {#top-i-s8-prop-3 .statement}

*Let $ (x_i)_{1 \leq i \leq n} $ be a finite family of distinct points of a Hausdorff space $ X $; then each $ x_i $ has a neighbourhood $ V_i $ in $ X $ such that the $ V_i $ ($ 1 \leq i \leq n $) are mutually disjoint.*

The proof is by induction on $ n $: the case $ n = 2 $ is just the axiom (H). Let then $ W_i $ ($ 1 \leq i \leq n - 1 $) be a neighbourhood of $ x_i $ such that the $ W_i $ are mutually disjoint. On the other hand, for $ 1 \leq i \leq n - 1 $ there is a neighbourhood $ T_i $ of $ x_i $ and a neighbourhood $ U_i $ of $ x_n $ which do not intersect. If we take $ V_i $ to be $ W_i \cap T_i $ for $ 1 \leq i \leq n - 1 $ and
$$
V_n = \bigcap_{i=1}^{n-1} U_i,
$$
the conditions of the proposition are satisfied.

#### Corollary {#top-i-s8-n1-cor-1 .statement}

*Every finite Hausdorff space is discrete.*

#### Proposition 4 {#top-i-s8-prop-4 .statement}

*Every finite subset of a Hausdorff space is closed.*

For every subset consisting of a single point is closed by reason of axiom (H\textsuperscript{i}).

#### Proposition 5 {#top-i-s8-prop-5 .statement}

*Let $ X $ be a topological space and suppose that for each pair of distinct points $ x, y $ of $ X $ there is a continuous mapping $ f $ of $ X $ into a Hausdorff space $ X' $ such that $ f(x) \neq f(y) $. Then $ X $ is Hausdorff.*

Let $ V' $ and $ W' $ be disjoint neighbourhoods of $ f(x) $ and $ f(y) $ respectively in $ X' $; then $ \overline{f}^{-1}(V') $ and $ \overline{f}^{-1}(W') $ are disjoint neighbourhoods of $ x $ and $ y $ respectively in $ X $.

#### Corollary {#top-i-s8-n1-cor-2 .statement}

*Every topology which is finer than a Hausdorff topology is Hausdorff.*

### 2. SUBSPACES AND PRODUCTS OF HAUSDORFF SPACES

*A subspace $ A $ of a Hausdorff space $ X $ is Hausdorff*, as we see by applying Proposition 5 of no. 1 to the canonical injection $ A \to X $. Conversely, we have

#### Proposition 6 {#top-i-s8-prop-6 .statement}

*If every point of a topological space $ X $ has a closed neighbourhood which is a Hausdorff subspace of $ X $, then $ X $ is Hausdorff.*

Let $ x \in X $ and let $ V $ be a closed neighbourhood of $ x $ in $ X $ such that the subspace $ V $ is Hausdorff. Then the closed neighbourhoods of $ x $ in $ V $ have $ \{x\} $ as their intersection (axiom (H\textsuperscript{'})); but they are also closed neighbourhoods of $ x $ in $ X $ (\S 3, no. 1) and therefore $ X $ satisfies (H\textsuperscript{i}).

There exist *non-Hausdorff* spaces in which every point has a Hausdorff neighbourhood (Exercise 7).

#### Proposition 7 {#top-i-s8-prop-7 .statement}

*Every product of Hausdorff spaces is Hausdorff. Conversely, if a product of non-empty spaces is Hausdorff, then each factor is a Hausdorff space.*

Let $ X = \prod_{i \in I} X_i $ be a product of topological spaces. Then if $ x, y $ are two distinct points of $ X $, we have $ \operatorname{pr}_i x \neq \operatorname{pr}_i y $ for some index $ i $, and Proposition 5 of no. 1 shows that $ X $ is Hausdorff if the $ X_i $ are. Conversely, if $ X $ is Hausdorff and the $ X_i $ are non-empty, then each $ X_i $ is homeomorphic to a subspace of $ X $ (\S 4, no. 2, Proposition 4) and is therefore Hausdorff.

#### Corollary 1 {#top-i-s8-prop-7-cor-1 .statement}

*Let $ X $ be a set, let $ (Y_i)_{i \in I} $ be a family of Hausdorff topological spaces, and for each $ i \in I $ let $ f_i $ be a mapping of $ X $ into $ Y_i $. Let $ X $ carry the coarsest topology $ \mathcal{T} $ for which the $ f_i $ are continuous. Then a necessary and sufficient condition for $ X $ to be Hausdorff is that for each pair of distinct points $ x, y $ of $ X $ we have $ f_i(x) \neq f_i(y) $ for some index $ i \in I $.*

The condition is sufficient by reason of Proposition 5 of no. 1. Conversely, suppose $ X $ is Hausdorff; let $ Y = \prod_{i \in I} Y_i $ and let $ f = (f_i)_{i \in I} $ be the mapping $ x \to (f_i(x)) $. By Proposition 7 above $ Y $ is Hausdorff, and by Proposition 3 of \S 4, no. 1, $ \mathcal{T} $ is the inverse image under $ f $ of the topology of $ Y $. If $ f(x) = f(y) $ for two distinct points $ x, y $ of $ X $ it is clear that every open set (in the topology $ \mathcal{T} $) which contains $ x $ also contains $ y $, contrary to the hypothesis that $ X $ is Hausdorff.

#### Corollary 2 {#top-i-s8-prop-7-cor-2 .statement}

*Let $ (X_\alpha, f_{\alpha \beta}) $ be an inverse system of topological spaces. If the $ X_\alpha $ are Hausdorff, then $ X = \varprojlim X_\alpha $ is Hausdorff and is a closed subspace of $ \prod_\alpha X_\alpha $.

The first assertion follows from the fact that $ X $ is a subspace of the Hausdorff space $ \prod_\alpha X_\alpha $ (Proposition 7). To show that $ X $ is closed in the product space, let $ F_{\alpha \beta} $ ($ \alpha \leq \beta $) be the subset of $ \prod_\alpha X_\alpha $ consisting of points $ x $ for which $ \operatorname{pr}_\alpha x = f_{\alpha \beta}(\operatorname{pr}_\beta x) $; the $ F_{\alpha \beta} $ are closed in $ \prod_\alpha X_\alpha $ (no. 1, Proposition 2), hence so is their intersection $ X $.

Evidently, any *sum* of Hausdorff spaces (\S 2, no. 4, Example 3) is a Hausdorff space.

### 3. HAUSDORFF QUOTIENT SPACES

Let us look for conditions under which a quotient space $ X/R $ is *Hausdorff* (in which case the equivalence relation $ R $ is said to be *Hausdorff*). In the first place, if $ X/R $ is Hausdorff, then the subsets of $ X/R $ consisting of a single point are *closed* (no. 1, Proposition 4) and hence *each equivalence class* mod $ R $ *is closed in* $ X $. But this necessary condition is not sufficient.

The definition of open sets in $ X/R $ gives rise to the following necessary and sufficient condition: $ X/R $ is Hausdorff if and only if any two distinct equivalence classes in $ X $ are contained in disjoint saturated open subsets of $ X $. We shall give other more usable conditions.

#### Proposition 8 {#top-i-s8-prop-8 .statement}

*A necessary condition for the quotient space $ X/R $ to be Hausdorff is that the graph $ C $ of $ R $ is closed in $ X \times X $. If the equivalence relation $ R $ is open, this condition is also sufficient.*

Let $ \varphi : X \to X/R $ be the canonical mapping; then $ C $ is the inverse image under $ \varphi \times \varphi : X \times X \to (X/R) \times (X/R) $ of the diagonal $ \Delta $ of $ (X/R) \times (X/R) $. The first part of the proposition therefore follows from the continuity of $ \varphi \times \varphi $ [Axiom (Hii) and Theorem 1 of § 2, no. 1]. If $ R $ is open then $ (X/R) \times (X/R) $ can be identified with the quotient space $ (X \times X)/(R \times R) $ ($ \S 5 $, no. 3, corollary to Proposition 8), and $ \Delta $ is then identified with the canonical image in $ (X \times X)/(R \times R) $ of the set $ C $, which is saturated with respect to $ R \times R $. Hence $ \Delta $ is closed in $ X \times X $ and therefore $ X $ is Hausdorff.

If $ R $ is not open, there are examples where $ C $ is closed but $ R $ is not Hausdorff (Exercises 10 and 28).

To show that $ X/R $ is Hausdorff we can also apply Proposition 5 of no. 1: $ M $ and $ N $ being two distinct equivalence classes of $ R $ it is sufficient that there should be a continuous mapping $ f $ of an open subset $ A $ of $ X $, saturated with respect to $ R $ and containing $ M $ and $ N $, into a Hausdorff space $ X' $, such that 1) $ f $ is constant on each equivalence class mod $ R $ contained in $ A $, 2) $ f $ takes distinct values on $ M $ and $ N $. For since $ A/R_A $ can be identified with an open subset of $ X/R $ ($ \S 3 $, no. 6, Proposition 10, Corollary 1), we can apply Proposition 5 of no. 1 to the mapping $ g : A/R_A \to X' $ induced by $ f $, since $ g $ is continuous ($ \S 3 $, no. 4, Proposition 6).

In particular:

#### Proposition 9 {#top-i-s8-prop-9 .statement}

*If $ f $ is a continuous mapping of a topological space $ X $ into a Hausdorff space $ X' $, and $ R $ is the equivalence relation $ f(x) = f(y) $, then the quotient space $ X/R $ is Hausdorff.*

#### Proposition 10 {#top-i-s8-prop-10 .statement}

*If $ X $ is a Hausdorff space, and if $ X $ has a continuous section $ s $ with respect to the equivalence relation $ R $, then $ X/R $ is Hausdorff and $ s(X/R) $ is closed in $ X $.*

For ($ \S 3 $, no. 5) $ X/R $ is homeomorphic to the subspace $ s(X/R) $ of $ X $, which is Hausdorff. Furthermore $ s(X/R) $ is the set of all $ x \in X $ such that $ s(\varphi(x)) = x $, where $ \varphi : X \to X/R $ is the canonical mapping; hence the second assertion follows from no. 1, Proposition 2.

### 4. REGULAR SPACES

#### Proposition 11 {#top-i-s8-prop-11 .statement}

The following properties of a topological space $ X $ are equivalent:

(O_{III}) The set of closed neighbourhoods of any point of $ X $ is a fundamental system of neighbourhoods of the point.

(O'_{III}) Given any closed subset $ F $ of $ X $ and any point $ x \notin F $ there is a neighbourhood of $ x $ and a neighbourhood of $ F $ which do not intersect.

(O_{III}) \Longrightarrow (O'_{III}): If $ F $ is closed and $ x \notin F $, then there is a closed neighbourhood $ V $ of $ x $ contained in the neighbourhood $ C_F $ of $ x $; $ V $ and $ C_V $ are neighbourhoods of $ x $ and $ F $ respectively, and have no point in common.

(O'_{III}) \Longrightarrow (O_{III}): If $ W $ is an open neighbourhood of $ x \in X $, then there is a neighbourhood $ U $ of $ x $ and a neighbourhood $ V $ of $ C_W $ which are disjoint, and therefore $ \overline{U} \subset W $.

#### Definition 2 {#top-i-s8-def-2 .statement}

A topological space is said to be regular if it is Hausdorff and satisfies axiom (O_{III}); its topology is then said to be regular.

A discrete space is regular. \* We shall see in § 9 that every locally compact space (in particular the real line $ \mathbf{R} $) is regular. \*

#### Proposition 12 {#top-i-s8-prop-12 .statement}

Every subspace of a regular space is regular.

Let $ A $ be a subspace of a regular space $ X $. Since $ X $ is Hausdorff, so is $ A $ (no. 2); on the other hand, every neighbourhood of a point $ x \in A $ with respect to $ A $ is of the form $ V \cap A $, where $ V $ is a neighbourhood of $ x $ in $ X $. Since $ X $ is regular there is a neighbourhood $ W $ of $ x $ in $ X $ which is closed in $ X $ and contained in $ V $; $ W \cap A $ is then a neighbourhood of $ x $ in $ A $, closed in $ A $ and contained in $ V \cap A $. Hence the result. Conversely:

#### Proposition 13 {#top-i-s8-prop-13 .statement}

If every point $ x $ of a topological space $ X $ has a closed neighbourhood which is a regular subspace of $ X $, then $ X $ is regular.

$ X $ is Hausdorff by Proposition 6 of no. 2. Let $ x $ be any point of $ X $ and let $ V $ be a closed regular neighbourhood of $ x $. If $ U $ is any neighbourhood of $ x $ contained in $ V $, then $ U $ is a neighbourhood of $ x $ relative to $ V $; hence by hypothesis there is a neighbourhood $ W $ of $ x $ in $ V $ which is closed in $ V $ and contained in $ U $. But $ W $ is a neighbourhood of $ x $ in $ X $ since $ V $ is a neighbourhood of $ x $ in $ X $, and $ W $ is closed in $ X $ since $ V $ is closed in $ X $.

#### Remark 1 {#top-i-s8-n4-rem-1 .statement}

There are examples of non-Hausdorff spaces in which every point has a regular neighbourhood (Exercise 7).
2) There are spaces which are Hausdorff but not regular (Exercise 20).
3) A topology which is finer than a regular topology need not be regular (Exercise 20).

### 5. EXTENSION BY CONTINUITY; DOUBLE LIMIT

#### Theorem 1 {#top-i-s8-thm-1 .statement}

Let X be a topological space, A a dense subset of X, f : A → Y a mapping of A into a regular space Y. A necessary and sufficient condition for f to extend to a continuous mapping $ \overline{f} : X \to Y $ is that, for each $ x \in X $, $ f(y) $ tends to a limit in Y when y tends to x while remaining in A. The continuous extension $ \overline{f} $ of f to X is then unique.

The uniqueness of $ \overline{f} $ follows from the principle of extension of identities (no. 1, Proposition 2, Corollary 1). It is clear that the condition is necessary, for if $ \overline{f} $ is continuous on X, then for each $ x \in X $ we have
$$
\overline{f}(x) = \lim_{y \to x, y \in A} \overline{f}(y) = \lim_{y \to x, y \in A} f(y)
$$
(§ 7, no. 5). Conversely, suppose that the condition is satisfied and define
$$
\overline{f}(x) = \lim_{y \to x, y \in A} f(y)
$$
for each $ x \in X $; $ \overline{f}(x) $ is a well-defined element of Y, since Y is Hausdorff. We have to show that $ \overline{f} $ is continuous at each point $ x \in X $. Let then V' be a closed neighbourhood of $ \overline{f}(x) $ in Y; then by hypothesis there is an open neighbourhood V of x in X such that $ f(V \cap A) \subset V' $. Since V is a neighbourhood of each of its points, we have
$$
\overline{f}(z) = \lim_{y \to z, y \in V \cap A} f(y)
$$
for each $ z \in V $, and from this it follows that $ \overline{f}(z) \in \overline{f}(V \cap A) \subset V' $, since V' is closed. The result now follows from the fact that the closed neighbourhoods of $ f(x) $ form a fundamental system of neighbourhoods of $ f(x) $ in Y.

The mapping $ \overline{f} $ is said to be obtained by extending f by continuity to X.

In the statement of Theorem 1 the hypothesis that Y is regular cannot be weakened without imposing additional restrictions on X, A or f (Exercise 19).

#### Corollary {#top-i-s8-n5-cor-1 .statement}

Let $ \mathfrak{F}_1 $ be a filter on a set $ X_1 $, and $ \mathfrak{F}_2 $ a filter on a set $ X_2 $; let $ \mathfrak{F}_1 \times \mathfrak{F}_2 $ be the product filter (§ 6, no. 7) on $ X = X_1 \times X_2 $, and let f be a mapping of X into a regular space Y. Suppose that
a) $ \lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f $ exists.

b) $ \lim_{x_2, \mathfrak{F}_2} f(x_1, x_2) = g(x_1) $ exists for all $ x_1 \in X_1 $.

Then $ \lim_{x_1, \mathfrak{F}_1} g(x_1) $ exists and is equal to $ \lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f $.

Let $ X'_1 = X_1 \cup \{\omega_1\} $ (resp. $ X'_2 = X_2 \cup \{\omega_2\} $) be the topological space *associated with the filter* $ \mathfrak{F}_1 $ (resp. $ \mathfrak{F}_2 $) (\S 6, no. 5, Example). In the product space $ X' = X'_1 \times X'_2 $ let $ X'' $ be the union of the subspaces $ X_1 \times X'_2 $ and $ \{(\omega_1, \omega_2)\} $. $ X $ is clearly a dense subspace of $ X'' $, and the hypotheses imply that $ f(y_1, y_2) $ tends to a limit when $ (y_1, y_2) $ tend to any point $ (x_1, x_2) $ of $ X'' $ whilst remaining in $ X $. The existence of the extension of $ f $ by continuity to $ X'' $ then follows from Theorem 1. Since also $ (\omega_1, \omega_2) $ lies in the closure of $ X_1 \times \{\omega_2\} $ relative to $ X'' $, the result follows immediately (\S 7, no. 5).

### 6. EQUIVALENCE RELATIONS ON A REGULAR SPACE

#### Proposition 14 {#top-i-s8-prop-14 .statement}

*Let* $ X $ *be a regular space*, $ R $ *a closed equivalence relation on* $ X $. *Then the graph* $ C $ *of* $ R $ *in* $ X \times X $ *is closed*.

Let $ (a, b) $ be a point of $ X \times X $ in the closure of $ C $, and let $ V $ (resp. $ W $) be a *closed* neighbourhood of $ a $ (resp. a neighbourhood of $ b $) in $ X $; then there is a point $ (x, y) \in C \cap (V \times W) $. Since $ x \in V $, $ y $ belongs to the saturation $ S $ of $ V $ with respect to $ R $; hence each neighbourhood $ W $ of $ b $ meets $ S $. By hypothesis $ S $ is *closed*, and therefore $ b \in S $. Now let $ B $ be the saturation of $ \{b\} $ with respect to $ R $, then each closed neighbourhood $ V $ of $ a $ meets $ B $; since by hypothesis $ B $ is *closed* and $ X $ is *regular*, it follows that $ a \in B $ and therefore that $ (a, b) \in C $. This completes the proof.

#### Corollary {#top-i-s8-n6-cor-1 .statement}

*On a regular space, every equivalence relation which is both open and closed is Hausdorff*.

This follows from Proposition 14 and Proposition 8 of no. 3.

#### Proposition 15 {#top-i-s8-prop-15 .statement}

*Let* $ X $ *be a regular space*, $ F $ *a closed subset of* $ X $, $ R $ *the equivalence relation on* $ X $ *obtained by identifying all the points of* $ F $ *[in other words, the equivalence relation whose equivalence classes are* $ F $ *(if* $ F \neq \emptyset $*) and the sets* $ \{x\} $ *where* $ x \in CF $*]. *Then the quotient space* $ X/R $ *is Hausdorff*.

Let $ M $ and $ N $ be two distinct equivalence classes in $ X $. If each of them consists of a single point in the complement of $ F $, then there exist two disjoint open neighbourhoods of $ M $ and $ N $ in the Hausdorff subspace $ CF $; these are neighbourhoods of $ M $ and $ N $ in $ X $ and are saturated with respect to $ R $. If $ M = F $ (so that $ F \neq \emptyset $) and $ N = \{ b \} $ where $ b \notin F $, then since $ X $ is regular there is an open neighbourhood of $ b $ and an open neighbourhood of $ F $ which do not intersect; these neighbourhoods are saturated with respect to $ R $, and the proposition is proved.

Note that the quotient space $ X/R $ is not necessarily regular (Chapter IX, § 4, Exercise 14).

### Exercises {#top-i-s8-exercises}

See the [exercises for § 8](exercises/s8/).
