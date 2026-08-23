---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 11
section_title: Connectedness
lang: en
source: top-i-iv
pdf_pages: 0113-0122, 0161-0167
extraction: ocr
subsections:
    - "no": 1
      title: CONNECTED SPACES AND CONNECTED SETS
      page: 0
      pdf_page: 113
    - "no": 2
      title: IMAGE OF A CONNECTED SET UNDER A CONTINUOUS MAPPING
      page: 0
      pdf_page: 115
    - "no": 3
      title: QUOTIENT SPACES OF A CONNECTED SPACE
      page: 0
      pdf_page: 116
    - "no": 4
      title: PRODUCT OF CONNECTED SPACES
      page: 0
      pdf_page: 116
    - "no": 5
      title: COMPONENTS
      page: 0
      pdf_page: 116
    - "no": 6
      title: LOCALLY CONNECTED SPACES
      page: 0
      pdf_page: 118
    - "no": 7
      title: 'APPLICATION : THE POINCARÉ-VOLTERRA THEOREM'
      page: 0
      pdf_page: 120
statements: 28
exercises: 25
content_sha256: 49e623cd592377d1f90b814606ff58adaeff059b1eb51901b6753b81790419ce
---

## 11. CONNECTEDNESS

### 1. CONNECTED SPACES AND CONNECTED SETS

#### Definition 1 {#top-i-s11-def-1 .statement}

A topological space X is said to be connected if it is not the union of two disjoint non-empty open sets.

An equivalent definition is obtained by replacing the words "open sets" by "closed sets". X is connected if and only if the only subsets of X which are both open and closed are the empty set and the whole space X.

If X is connected and if A, B are two non-empty open (resp. closed) subsets such that A \cup B = X, then A \cap B \neq \emptyset.

#### Example 1 {#top-i-s11-n1-exa-1 .statement}

We shall see in Chapter IV, § 2, no. 5 that the real line is connected, and that the rational line is not. \*
2) A discrete space which has more than one point is not connected.

#### Definition 2 {#top-i-s11-def-2 .statement}

*A subset $ A $ of a topological space $ X $ is said to be a connected set if the subspace $ A $ of $ X $ is connected.*

For $ A $ to be a connected subset of $ X $ it is necessary and sufficient that, for each covering of $ A $ by two open (or closed) subsets $ B, C $ of $ X $ such that $ A \cap B $ and $ A \cap C $ are non-empty, we have $ A \cap B \cap C \neq \emptyset $.

#### Example {#top-i-s11-n1-exa-2 .statement}

In any topological space, the empty set and every set consisting of a single point are connected. In a Hausdorff space $ X $, every finite set consisting of more than one point is not connected, and more generally every subset of $ X $ which has more than one point and which has at least one isolated point is not connected.

If a dense subset $ A $ is connected, then the whole space $ X $ is connected; otherwise there would exist two non-empty disjoint open subsets $ M, N $ of $ X $ such that $ M \cup N = X $, and $ M \cap A, N \cap A $ would be two disjoint non-empty open subsets of $ A $ whose union is $ A $. Hence we have

#### Proposition 1 {#top-i-s11-prop-1 .statement}

*If $ A $ is a connected set, then every set $ B $ such that $ A \subset B \subset \overline{A} $ is connected.*

#### Proposition 2 {#top-i-s11-prop-2 .statement}

*The union of a family of connected sets whose intersection is non-empty is connected.*

Let $ (A_i)_{i \in I} $ be a family of connected subsets of $ X $, all of which contain the same point $ x $; we have to show that

$$
A = \bigcup_i A_i
$$

is connected. If not, there are two open sets $ B $ and $ C $ such that $ B \cap A $ and $ C \cap A $ are non-empty, and $ A \subset B \cup C $ and $ A \cap B \cap C = \emptyset $. $ x $ belongs to one of the sets $ B, C $, say $ x \in B $; on the other hand one of the sets $ A_i $, say $ A_x $, meets $ C $; we have therefore $ A_x \subset B \cup C $, $ A_x \cap B \cap C = \emptyset $ and $ B \cap A_x $ and $ C \cap A_x $ are non-empty. Hence $ A_x $ is not connected, which is a contradiction.

#### Corollary {#top-i-s11-n1-cor-1 .statement}

*Let $ (A_n)_{n \geq 0} $ be an infinite sequence of connected sets such that $ A_{n+1} \cap A_n \neq \emptyset $ for all $ n \geq 0 $. Then the union $ \bigcup_{n=0}^\infty A_n $ is connected.*

By induction on $ n $ we see immediately that the set $ B_n = \bigcup_{i=0}^n A_i $ is connected for all $ n $, by Proposition 2. The sets $ B_n $ have a non-empty intersection; hence their union, equal to $ \bigcup_{n=0}^\infty A_n $, is connected by Proposition 2.

#### Proposition 3 {#top-i-s11-prop-3 .statement}

*Let $ A $ be a subset of a topological space $ X $. If $ B $ is a connected subset of $ X $ which meets both $ A $ and $ \complement A $, then $ B $ meets the frontier of $ A $.*

For otherwise the intersections of $ B $ with the interior and exterior of $ A $ would be two open subsets of $ B $ which form a partition of $ B $, and $ B $ would not be connected.

#### Corollary {#top-i-s11-n1-cor-2 .statement}

*In a connected space $ X $, every non-empty set other than $ X $ itself has at least one frontier point.*

### 2. IMAGE OF A CONNECTED SET UNDER A CONTINUOUS MAPPING

#### Proposition 4 {#top-i-s11-prop-4 .statement}

*Let $ A $ be a connected subset of a topological space $ X $, and let $ f $ be a continuous mapping of $ X $ into a topological space $ X' $. Then $ f(A) $ is connected.*

Suppose $ f(A) $ is not connected. Then there exist two sets $ M', N' $ which are open in $ f^{-1}(A) $ and which form a partition of $ f(A) $; hence $ A \cap f^{-1}(M') $ and $ A \cap f^{-1}(N') $ are open in $ A $ and form a partition of $ A $; this contradicts the hypothesis that $ A $ is connected.

The *inverse image* of a connected set under a continuous mapping need not be connected; consider for example a mapping of a discrete space into a space consisting of one point.

From Proposition 4 we derive another characterization of *non-connected spaces*:

#### Proposition 5 {#top-i-s11-prop-5 .statement}

*For a topological space $ X $ to be not connected it is necessary and sufficient that there exists a surjective continuous mapping of $ X $ onto a discrete space containing more than one point.*

The condition is sufficient by Proposition 4. Conversely, if $ X $ is not connected, there exist two non-empty disjoint open subsets $ A, B $ whose union is $ X $, and the mapping $ f $ of $ X $ onto a discrete space of two elements $ \{a, b\} $, defined by $ f(A) = \{a\} $ and $ f(B) = \{b\} $, is continuous.

### 3. QUOTIENT SPACES OF A CONNECTED SPACE

#### Proposition 6 {#top-i-s11-prop-6 .statement}

Every quotient space of a connected space is connected.

This is an immediate consequence of Proposition 4 of no. 2.

#### Proposition 7 {#top-i-s11-prop-7 .statement}

Let $ X $ be a topological space and $ R $ an equivalence relation on $ X $. If the quotient space $ X/R $ is connected, and if each equivalence class mod $ R $ is connected, then $ X $ is connected.

Suppose $ X $ is not connected. Then there is a partition of $ X $ into two open sets $ A, B $. The sets $ A, B $ are saturated with respect to $ R $; for if $ x \in A $ then the equivalence class $ M $ of $ x $ cannot meet $ B $, otherwise the sets $ A \cap M, B \cap M $ would form a partition of $ M $ into two sets open in $ M $, which is impossible since $ M $ is connected. The canonical images of $ A $ and $ B $ are therefore open sets in $ X/R $ and form a partition of $ X/R $; this contradicts the assumption that $ X/R $ is connected.

### 4. PRODUCT OF CONNECTED SPACES

#### Proposition 8 {#top-i-s11-prop-8 .statement}

Every product of connected spaces is connected. Conversely, if a product of non-empty spaces is connected, then each of the factors is connected.

Let $ X = \prod_{i \in I} X_i $ be a product of topological spaces. If the $ X_i $ are non-empty, we have $ X_i = \operatorname{pr}_i X $ for each $ i \in I $; hence if $ X $ is connected so are the $ X_i $ (no. 2, Proposition 4). Conversely, suppose that each of the $ X_i $ is connected and $ X $ is not. By Proposition 5 of no. 2, there exists a continuous surjective mapping $ f : X \to X' $, where $ X' $ is a discrete space which contains more than one point. Let $ a = (a_i) $ be any point of $ X $, and $ x $ any index; the partial mapping $ f_x : X_x \to X' $, defined by $ f_x(x) = f((y_i)) $ where $ y_x = x $ and $ y_i = a_i $ if $ i \neq x $, is continuous on $ X_x $; since $ X_x $ is connected, $ f_x $ must be constant on $ X_x $. It follows immediately by induction that $ f(x) = f(a) $ for all points $ x = (x_i) $ such that $ x_i = a_i $ for all but a finite number of indices $ i \in I $. But these points $ x $ form a dense subset of $ X $ (\S 4, no. 3, Proposition 8). Hence $ f $ is continuous on $ X $ and constant on a dense subset of $ X $, and therefore constant on $ X $ (\S 8, no. 1, Proposition 2, Corollary 1). But this contradicts the definition of $ f $.

### 5. COMPONENTS

Given a point $ x $ of a topological space $ X $, the union of the connected subsets of $ X $ which contain $ x $ is connected (no. 1, Proposition 2); it is therefore the largest connected subset of $ X $ which contains $ x $.

#### Definition 3 {#top-i-s11-def-3 .statement}

The component (or connected component) of a point of a topological space $ X $ is the largest connected subset of $ X $ which contains this point. The components of a subset $ A $ of $ X $ are the components of the points of $ A $, relative to the subspace $ A $ of $ X $.

If a space is connected, the component of each point is the whole space. If a space $ X $ is such that for each pair $ (x, y) $ of points of $ X $ there is a connected set containing $ x $ and $ y $, then $ X $ is connected.

A space $ X $ is said to be *totally disconnected* if the component of each point of $ X $ consists of the point alone. A subset $ A $ of $ X $ is a *totally disconnected set* if the subspace $ A $ of $ X $ is totally disconnected.

A *discrete* space is totally disconnected, but one should beware of confusing these two notions; for example, we shall see in Chapter IV, § 2, no. 5, that the rational line, which is not a discrete space, is totally disconnected.

A set which is *both open and closed* contains the component of each of its points, whence *the component of a point is contained in the intersection of the sets which are both open and closed and which contain this point*. However, the component of a point is not necessarily equal to this intersection (cf. Exercise 9 and Chapter II, § 4, no. 4, Proposition 6).

#### Proposition 9 {#top-i-s11-prop-9 .statement}

*The component of any point in a topological space $ X $ is a closed set. The relation "y belongs to the component of x" is an equivalence relation $ R \{ x, y \} $ on $ X $, and the equivalence classes are the components of $ X $. The quotient space $ X/R $ is totally disconnected.*

The first part of the proposition is an immediate consequence of Definition 3 and the fact that the closure of a connected set is connected (no. 1, Proposition 1). Since the union of connected sets which have a point in common is connected (no. 1, Proposition 2), the relation $ R $ is transitive, hence is an equivalence relation (since it is obviously reflexive and symmetric) and the equivalence class of $ x $ with respect to $ R $ is the component of $ x $. It remains to show that $ X/R $ is totally disconnected. Let $ f : X \to X/R $ be the canonical mapping, and let $ F $ be a closed set in $ X/R $ *containing at least two distinct points*; the inverse image $ f^{-1}(F) $ of $ F $ is closed in $ X $, saturated with respect to $ R $, and contains at least two distinct components of $ X $ and hence is *not connected*. Hence there exist two non-empty closed sets $ B, C $ in $ X $ such that $ B \cap C = \varnothing $ and $ B \cup C = f^{-1}(F) $. The component of any point $ x $ of $ f^{-1}(F) $ *in* $ f^{-1}(F) $ is the same as the component of $ x $ *in* $ X $ (by the definition of $ R $) and therefore $ B $ and $ C $, which are both open and closed *in* $ f^{-1}(F) $, are saturated with respect to $ R $. Hence $ f(B) $ and $ f(C) $ are closed in $ X/R $, and $ f(B) \cup f(C) = F $ and $ f(B) \cap f(C) = \varnothing $; this shows that $ F $ is *not connected* and consequently that $ X/R $ is totally disconnected.

#### Proposition 10 {#top-i-s11-prop-10 .statement}

In a product space $ X = \prod_{i \in J} X_i $, the component of $ x = (x_i) $ in $ X $ is the product of the components of $ x_i $ in the factors $ X_i $.

This product set is connected (no. 4, Proposition 8). Conversely, if $ A $ is a connected subset of $ X $ which contains $ x $, then $ \operatorname{pr}_i(A) $ is a connected set (no. 2, Proposition 4) which contains $ x $; since $ A \subset \prod_i \operatorname{pr}_i(A) $, it follows that $ A $ is contained in the product of the components of the $ x_i $.

### 6. LOCALLY CONNECTED SPACES

#### Definition 4 {#top-i-s11-def-4 .statement}

A topological space $ X $ is said to be locally connected if each point of $ X $ has a fundamental system of connected neighbourhoods.

\* We shall see in Chapter IV, § 2, no. 5, that the real line is a locally connected space. \*
The existence, at each point $ x $ of a space $ X $, of one connected neighbourhood of $ x $ by no means implies that $ X $ is locally connected. In particular, $ X $ can be connected but not locally connected (Exercises 2 and 13). Conversely, a space can be locally connected but not connected (e.g. a discrete space which contains more than one point).

#### Proposition 11 {#top-i-s11-prop-11 .statement}

A necessary and sufficient condition for a space $ X $ to be locally connected is that every component of an open set in $ X $ is open in $ X $.

The condition is sufficient, since the component of $ x $ relative to an open neighbourhood of $ x $ is then a neighbourhood of $ x $ in $ X $.

Conversely, let $ A $ be an open subset of a locally connected space $ X $, let $ B $ be a component of $ A $, and let $ x \in B $. Let $ V $ be a connected neighbourhood of $ x $ contained in $ A $; by the definition of components, $ V $ is contained in $ B $; hence $ B $ is open in $ X $ (\S 1, no. 2, Proposition 1).

The components of a locally connected space $ X $ therefore form a partition of $ X $ into open sets, and hence $ X $ is the sum (\S 2, no. 4, Example 3) of its components.

#### Corollary {#top-i-s11-n6-cor-1 .statement}

Let $ U $ be an open subset of a locally connected space $ X $, and let $ V $ be a component of $ U $. Then the frontier of $ V $ (relative to $ X $) is contained in the frontier of $ U $.

For $ V $ is open and closed in $ U $, hence a frontier point of $ V $ (relative to $ X $) cannot belong to $ U $, for it would also be a frontier point of $ V $ relative to $ U $, and there is none.

#### Proposition 12 {#top-i-s11-prop-12 .statement}

Every quotient space of a locally connected space is locally connected.

Let $ X $ be a locally connected space, $ R $ an equivalence relation on $ X $, $ \varphi : X \to X/R $ the canonical mapping. Let $ A $ be an open subset of

X/R and C a component of A. Then $ \overline{\varphi}^1(C) $ is a union of components of $ \overline{\varphi}^1(A) $; for if $ x \in \overline{\varphi}^1(C) $ and if K is the component of x in $ \overline{\varphi}^1(A) $ then $ \varphi(K) $ is connected (no. 2, Proposition 4), is contained in A, and contains $ \varphi(x) $; hence $ \varphi(K) \subset C $ by the definition of C, and therefore $ K \subset \overline{\varphi}^1(C) $. Since X is locally connected and $ \overline{\varphi}^1(A) $ is open in X, it follows from Proposition 11 that $ \overline{\varphi}^1(C) $ is open in X; consequently C is open in X/R and hence, by Proposition 11 again, X/R is locally connected.

#### Proposition 13 {#top-i-s11-prop-13 .statement}

a) Let $ (X_i)_{i \in I} $ be a family of locally connected spaces such that $ X_i $ is connected for all but a finite number of indices $ i \in I $. Then the product space $ X = \prod_{i \in I} X_i $ is locally connected.

b) Conversely, if the product of a family $ (X_i) $ of non-empty topological spaces is locally connected, then each $ X_i $ is locally connected, and $ X_i $ is connected for all but a finite number of indices.

a) Let J be the finite subset of I such that $ X_i $ is not connected if and only if $ i \in J $. Let
$$
U = \prod_{i \in I} U_i
$$
be an elementary set containing a point $ x = (x_i) $ of X and let K be the finite subset of I such that $ U_i \neq X_i $ if and only if $ i \in K $. Let $ V_i $ be $ X_i $ for $ i \notin J \cup K $, and let $ V_i $ be a connected neighbourhood of $ x_i $ contained in $ U_i $ for $ i \in J \cup K $; then
$$
V = \prod_{i \in I} V_i
$$
is connected (by Proposition 8 of no. 4) and is a neighbourhood of $ x $ contained in U. Hence X is locally connected.

b) Let $ a = (a_i) $ be a point of X and let V be a connected neighbourhood of $ a $ in X. Since we have $ \mathrm{pr}_i V = X_i $ except for a finite number of indices (\S 4, no. 1) it follows from no. 2, Proposition 4 that the $ X_i $ are connected, for all but a finite number of indices. On the other hand, for each $ x \in I $, each $ a_x \in X_x $ and each neighbourhood $ V_x $ of $ a_x $ in $ X_x $, there is a point $ x $ of X such that $ \mathrm{pr}_x x = a_x $, and
$$
V = V_x \times \prod_{i \neq x} X_i
$$
is a neighbourhood of $ x $ in X; V therefore contains a connected neighbourhood W of $ x $, whose projection $ \mathrm{pr}_x W $ is a connected neighbourhood of $ a_x $ contained in $ V_x $ (no. 2, Proposition 4 and \S 4, no. 2, Proposition 5). Hence each $ X_x $ is locally connected.

### 7. APPLICATION : THE POINCARÉ-VOLTERRA THEOREM

#### Theorem 1 {#top-i-s11-thm-1 .statement}

Let $ X $ be a topological space satisfying axiom $(O_{III})$ (but not necessarily Hausdorff), and suppose $ X $ is connected and locally connected. Let $ Y $ be a topological space whose topology has a countable base, and let $ p : X \to Y $ be a continuous mapping such that, for each $ y \in Y $, $ \overline{p}^{-1}(y) $ is a discrete subspace of $ X $. Finally let $ \mathcal{B} $ be a set of subsets of $ X $ whose interiors cover $ X $ and such that:
(i) *The restriction of* $ p $ *to each* $ V \in \mathcal{B} $ *is a closed mapping of* $ V $ *into* $ Y $.
(ii) *Every* $ V \in \mathcal{B} $ *has a countable subset which is dense in* $ V $.

*Then the space* $ X $ *is the union of a countable family of open sets each of which is contained in a set of* $ \mathcal{B} $.

Let $ \mathcal{B} $ be a countable base of the topology of $ Y $. We shall say that a pair $ (W, U) $ is *distinguished* if (i) $ U \in \mathcal{B} $ and (ii) $ W $ is a component of $ \overline{p}^{-1}(U) $ contained in a set of $ \mathcal{B} $.

#### Lemma 1 {#top-i-s11-lem-1 .statement}

*If* $ x $ *is any point of* $ X $, *there is a distinguished pair* $ (W, U) $ *such that* $ x \in W $.

The inverse image $ \overline{p}^{-1}(p(x)) $ is discrete and therefore there is a neighbourhood of $ x $ in $ X $ all of whose points $ x' $ other than $ x $ have an image $ p(x') \neq p(x) $; since $ X $ satisfies $(O_{III})$, there is a *closed* neighbourhood $ V $ of $ x $ with this property, and we may assume also that $ V $ is contained in a set of $ \mathcal{B} $. Let $ F $ be the frontier of $ V $ in $ X $. By condition (i) of the theorem, $ p(F) $ is closed in $ Y $; and since $ p(F) $ does not contain $ p(x) $, there is a set $ U \in \mathcal{B} $ which contains $ p(x) $ and does not meet $ p(F) $. Let $ W $ be the component of $ x $ in $ \overline{p}^{-1}(U) $; then it is enough to show that $ W \subset \mathbb{A} $. If this were not so, then $ W $ would meet $ F $ (no. 1, Proposition 3) and therefore $ p(F) $ would meet $ U $, contrary to the definition of $ U $.

#### Lemma 2 {#top-i-s11-lem-2 .statement}

*If* $ (W, U) $ *is a distinguished pair then the set of all distinguished pairs* $ (W', U') $ *such that* $ W' $ *meets* $ W $ *is countable*.

Since $ \mathcal{B} $ is countable it is enough to show that, given $ U' \in \mathcal{B} $, the set of distinguished pairs $ (W', U') $ such that $ W' $ meets $ W $ is countable. Now these sets $ W' $ are open, since $ X $ is locally connected (no. 6, Proposition 11) and mutually disjoint since they are components of $ \overline{p}^{-1}(U') $; hence the sets $ W' \cap W $ are open and mutually disjoint. But $ W $ contains a countable subset which is dense in $ W $; hence the set of $ W' $ such that $ W' \cap W $ is not empty is also countable.

To prove Theorem 1, consider the following relation R between two points x, x' of X: "There exists a finite sequence of distinguished pairs (W_i, U_i) (1 \leq i \leq n) such that x \in W_1 and x' \in W_n and that W_i \cap W_{i+1} \neq \emptyset for \leq 1 i \leq n — 1."

Lemma 1 states that R is reflexive, and it is readily verified that R is symmetric and transitive, so that R is an equivalence relation; also, since the W_i are open, every equivalence class mod R is open in X. But X is connected; hence there can be only one equivalence class, i.e. any two points of X are congruent mod R. We shall deduce from this that X is the union of a countable family of first elements of distinguished pairs, and this will prove Theorem 1. For this, let x be any point of X, and define by induction on n a sequence (C_n) of open subsets of X as follows: by Lemma 1 there is a distinguished pair (W_1, U_1) such that x \in W_1, and we take C_1 = W_1; if n > 1 then C_n is to be the union of all first elements W of distinguished pairs (W, U) such that W meets C_{n-1}. By induction on n one shows immediately, by virtue of Lemma 2, that C_n is a countable union of first elements of distinguished pairs. Finally, every x' \in X belongs to some C_n; for there is a finite sequence

$$(W'_i, U'_i)_{1 \leq i \leq m}$$

of distinguished pairs such that x \in W'_1, x' \in W'_m and W'_i \cap W'_{i+1} \neq \emptyset for 1 \leq i \leq m — 1, and by induction on i we see that W'_i \subset C_{i+1} for all i, so that x' \in C_{m+1}.

Q.E.D.

#### Corollary 1 {#top-i-s11-lem-2-cor-1 .statement}

Let Y be a regular space whose topology has a countable base (*). Let X be a connected and locally connected space, and let p : X \to Y be a continuous mapping with the following property: for each x \in X there is a closed neighbourhood V of x in X such that the restriction of p to V is a homeomorphism of V onto a closed subspace of Y. Then X is regular and the topology of X has a countable base.

First, the hypotheses imply that X is regular (§ 8, no. 4, Proposition 13). Let us show that the conditions of Theorem 1 are satisfied if we take \mathfrak{B} to be the set of all closed subsets V of X such that the restriction of p to V is a homeomorphism of V onto a closed subspace of Y. By hypothesis, the interiors of the sets of \mathfrak{B} cover Y and, by virtue of the assumption on Y, each V \in \mathfrak{B} has a countable base and therefore contains a countable dense subset (§ 1, no. 6, Proposition 6). Furthermore, if x \in p^{-1}(y), there is a neighbourhood V \in \mathfrak{B} of x in X such that V con-

(*) \* It can be shown that these conditions imply that the topology of Y is metrizable (Chapter IX, § 4, Exercise 22). \* tains no point of $ \overline{p}^{-1}(y) $ other than $ x $, and hence $ \overline{p}^{-1}(y) $ is a discrete space. We may therefore apply Theorem 1, which shows that $ X $ is the union of a countable family $ (T_n)_{n \geq 0} $ of open sets, such that each subspace $ T_n $ has a countable base $ (U_{mn})_{m \geq 0} $. Then the $ U_{mn} $ ($ m \geq 0, n \geq 0 $) form a base of the topology of $ X $ ($ \S 3 $, no. 1, Remark).

#### Corollary 2 {#top-i-s11-lem-2-cor-2 .statement}

*Let $ X $ be locally compact, connected and locally connected, and suppose each point of $ X $ has a neighbourhood which has a countable base. Let $ Y $ be a Hausdorff space whose topology has a countable base, and let $ p : X \to Y $ be a continuous mapping such that, for each $ y \in Y $, $ \overline{p}^{-1}(y) $ is a discrete subspace of $ X $. Then the topology of $ X $ has a countable base.*

For each $ x \in X $, let $ V_x $ be a compact neighbourhood of $ x $ in $ X $ which has a countable base. It follows from $ \S 9 $, no. 4, Theorem 2, Corollary 2, that the set $ \mathcal{B} $ of the $ V_x $ satisfies the conditions of Theorem 1, and we complete the proof as in Corollary 1.

Notice that, in this corollary, it can happen that the restriction of $ p $ to an arbitrarily small neighbourhood $ V $ of a point of $ X $ *is not a homeomorphism of $ V $ onto $ p(V) $*.

#### Corollary 3 (Poincaré-Volterra Theorem) {#top-i-s11-lem-2-cor-3 .statement}

*Let $ Y $ be a locally compact, locally connected space whose topology has a countable base. Let $ X $ be a connected Hausdorff space, and let $ p : X \to Y $ be a continuous mapping which has the following property : for each $ x \in X $ there is an open neighbourhood $ U $ of $ x $ in $ X $ such that the restriction of $ p $ to $ U $ is a homeomorphism of $ U $ onto an open subspace of $ Y $. Then $ X $ is locally compact and locally connected, and the topology of $ X $ has a countable base.*

Clearly $ X $ is locally connected. Also each $ x \in X $ has an open neighbourhood $ U $ in $ X $ such that the restriction of $ p $ to $ U $ maps $ U $ homeomorphically onto an open subspace $ p(U) $ of $ Y $. Since $ p(U) $ is a locally compact subspace of $ Y $ ($ \S 9 $, no. 7, Proposition 13), there is a compact neighbourhood $ W $ of $ p(x) $ contained in $ p(U) $, whence $ U \cap \overline{p}^{-1}(W) $ is a compact neighbourhood of $ x $ contained in $ U $; thus $ X $ is locally compact, since by hypothesis $ X $ is Hausdorff. $ U \cap \overline{p}^{-1}(W) $, being compact, is closed in $ X $ ($ \S 9 $, no. 3, Proposition 4) and the conditions of Corollary 1 are therefore satisfied; hence the topology of $ X $ has a countable base.

### Exercises {#top-i-s11-exercises}

See the [exercises for § 11](exercises/s11/).
