---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 4
section_title: Product of topological spaces
lang: en
source: top-i-iv
pdf_pages: 0049-0056, 0131-0133
extraction: ocr
subsections:
    - "no": 1
      title: PRODUCT SPACES
      page: 0
      pdf_page: 49
    - "no": 2
      title: SECTION OF AN OPEN SET; SECTION OF A CLOSED SET; PROJECTION OF AN OPEN SET. PARTIAL CONTINUITY
      page: 0
      pdf_page: 52
    - "no": 3
      title: CLOSURE IN A PRODUCT
      page: 0
      pdf_page: 53
    - "no": 4
      title: INVERSE LIMITS OF TOPOLOGICAL SPACES
      page: 0
      pdf_page: 54
statements: 21
exercises: 3
content_sha256: c92011a27ae84f64199bc5c751e4506bd05a79dad58b11cbcf6ac857846cfa96
---

## 4. PRODUCT OF TOPOLOGICAL SPACES

### 1. PRODUCT SPACES

#### Definition 1 {#top-i-s4-def-1 .statement}

*Given a family $ (X_i)_{i \in I} $ of topological spaces, the product space of this family is the product set $ X = \prod_{i \in I} X_i $ with the topology which is the product of the topologies of the $ X_i $ (\S 2, no. 3, Example 3). The spaces $ X_i (i \in I) $ are called the factors of X.*

By virtue of § 2, no. 3, Proposition 4, the product topology on $ X $ has as a base the set $ \mathcal{B} $ of finite intersections of sets of the form $ \overline{\mathrm{pr}}_i^{-1}(U_i) $, where $ U_i $ is open in $ X_i $; these sets are products $ \prod_{i \in I} A_i $, where $ A_i $ is open in $ X_i $ for each $ i \in I $ and $ A_i = X_i $ for all but a finite number of indices. These sets will be called elementary sets.

If $ \mathcal{B}_i $ is a base of the topology of $ X_i $ (for each $ i \in I $), it is clear that the elementary sets $ \prod_{i \in I} A_i $ such that $ A_i \in \mathcal{B}_i $ for each index $ i $ such that $ A_i \neq X_i $ form another base of the product topology. The elementary sets of this type which contain a given point $ x \in X $ thus form a fundamental system of neighbourhoods of $ x $ ($ \S 1 $, no. 3, Proposition 3).

If $ I $ is a finite set, the construction of the product topology from the topologies of the factors $ X_i $ is simpler: the elementary sets are just products $ \prod_{i \in I} A_i $, where $ A_i $ is any open subset of $ X_i $, for each $ i \in I $ (cf. Exercise 9).

#### Example {#top-i-s4-n1-exa-1 .statement}

\* The product $ \mathbf{R}^n $ of $ n $ spaces identical with the real line $ \mathbf{R} $ is called real number space of $ n $ dimensions; $ \mathbf{R}^2 $ is also called the real plane (cf. Chapter VI, § 1). Likewise, starting from the rational line $ \mathbf{Q} $, we define the rational number space of $ n $ dimensions $ \mathbf{Q}^n $ (rational plane for $ n = 2 $).

The topology of the space $ \mathbf{R}^n $ has as a base the set of all products of $ n $ open intervals in $ \mathbf{R} $, which are called open boxes of $ n $ dimensions. The open boxes which contain a point $ x \in \mathbf{R}^n $ form a fundamental system of neighbourhoods of this point. Likewise the products of $ n $ closed intervals in $ \mathbf{R} $ are called closed boxes of $ n $ dimensions. The closed boxes to which $ x $ is interior also form a fundamental system of neighbourhoods of $ x $. There are analogous results for $ \mathbf{Q}^n $. \*

#### Proposition 1 {#top-i-s4-prop-1 .statement}

Let $ f = (f_i) $ be a mapping of a topological space $ Y $ into a product space $ X = \prod_{i \in I} X_i $. Then $ f $ is continuous at a point $ a \in Y $ if and only if $ f_i $ is continuous at $ a $ for each $ i \in I $.

Since $ f_i = \mathrm{pr}_i \circ f $, this is just a particular case of Proposition 4 of § 2, no. 3.

#### Corollary 1 {#top-i-s4-prop-1-cor-1 .statement}

Let $ (X_i)_{i \in I}, (Y_i)_{i \in I} $ be two families of topological spaces with the same set of indices. For each $ i \in I $, let $ f_i $ be a mapping of $ X_i $ into $ Y_i $. In order that the product mapping $ f : (x_i) \to (f_i(x_i)) $ of
$$
\prod_{i \in I} X_i \text{ into } \prod_{i \in I} Y_i
$$
should be continuous at a point $ a = (a_i) $ it is necessary and sufficient that $ f_i $ is continuous at $ a_i $ for each $ i \in I $.

f can be written as $ x \to (f_i(\mathrm{pr}_i(x))) $, so that by Proposition 1 the condition is sufficient. Conversely, for each $ x \in I $ let $ g_x $ be the mapping of $ X_x $ into $ \prod_{i \in I} X_i $ such that $ \mathrm{pr}_x(g_x(x_x)) = x_x $ and $ \mathrm{pr}_i(g_x(x_x)) = a_i $ whenever $ i \neq x $; then $ g_x $ is continuous at the point $ a_x $, by Proposition 1. Since $ f_x = \mathrm{pr}_x \circ f \circ g_x $ it follows that if $ f $ is continuous at $ a $, then $ f_x $ is continuous at $ a_x $.

#### Corollary 2 {#top-i-s4-prop-1-cor-2 .statement}

*Let $ X, Y $ be two topological spaces. In order that a mapping $ f : X \to Y $ should be continuous it is necessary and sufficient that the mapping $ g : x \to (x, f(x)) $ is a homeomorphism of $ X $ onto the graph $ G $ of $ f $ (considered as a subspace of the product space $ X \times Y $).*

Since $ f = \mathrm{pr}_2 \circ g $, the condition is sufficient. It is also necessary, for if $ f $ is continuous, then $ g $ is bijective and continuous (Proposition 1) and the inverse of $ g $ is the restriction of $ \mathrm{pr}_1 $ to $ G $, which is continuous (cf. *Set Theory*, Chapter IV, § 2, no. 4, criterion CST 17).

#### Proposition 2 (Associativity of topological products) {#top-i-s4-prop-2 .statement}

*Let $ (X_i)_{i \in I} $ be a family of topological spaces, $ (J_x)_{x \in K} $ a partition of the set $ I $, and for each $ x \in K $ let $ X'_x = \prod_{i \in J_x} X_i $ be the product of the spaces $ X_i $ for $ i \in J_K $. Then the canonical mapping of the product space*
$$
\prod_{i \in I} X_i \text{ onto the product space } \prod_{x \in K} X'_x
$$
*is a homeomorphism.*

This is a particular case of transitivity of initial topologies ($ \S $ 2, no. 3, Proposition 5; cf. *Set Theory*, Chapter IV, § 2, no. 4, criterion CST 13).

Generally we *identify* the product spaces $ \prod_{i \in I} X_i $ and $ \prod_{x \in K} X'_x $ by means of the canonical mapping.

#### Corollary {#top-i-s4-n1-cor-1 .statement}

*Let $ \sigma $ be a permutation of the set $ I $. Then the mapping $ (x_i) \to (x_{\sigma(i)}) $ is a homeomorphism of*
$$
\prod_{i \in I} X_i \text{ onto } \prod_{i \in I} X_{\sigma(i)}.
$$

Take $ K = I $ and $ J_i = \{ \sigma(i) \} $ for each $ i \in I $ in Proposition 2.

#### Proposition 3 {#top-i-s4-prop-3 .statement}

*Let $ X $ be a set, $ (Y_i)_{i \in I} $ a family of topological spaces, and for each $ i \in I $ let $ f_i $ be a mapping of $ X $ into $ Y_i $. Let $ f $ be the mapping $ x \to (f_i(x)) $ of $ X $ into $ Y = \prod_{i \in I} Y_i $, and let $ \mathcal{T} $ be the coarsest topology on $ X $ for which the mappings $ f_i $ are continuous. Then $ \mathcal{T} $ is the inverse image under $ f $ of the topology induced on $ f(X) $ by the product topology on $ Y $.*

This is another particular case of transitivity of initial topologies (\S\ 2, no. 3, Proposition 5; cf. Set Theory, Chapter IV, \S\ 2, no. 4, criterion CST 15).

#### Corollary {#top-i-s4-n1-cor-2 .statement}

*For each $ i \in I $ let $ A_i $ be a subspace of $ Y_i $. Then the topology induced on $ A = \prod_{i \in I} A_i $ by the product topology on $ \prod_{i \in I} Y_i $ is the product of the topologies of the subspaces $ A_i $.*

Let $ j_i $ be the canonical injection $ A_i \to Y_i $, and apply Proposition 3 to the mappings $ f_i = j_i \circ \mathrm{pr}_i $ (cf. Set Theory, Chapter IV, \S\ 2, no. 4, criterion CST 14).

### 2. SECTION OF AN OPEN SET; SECTION OF A CLOSED SET; PROJECTION OF AN OPEN SET. PARTIAL CONTINUITY

#### Proposition 4 {#top-i-s4-prop-4 .statement}

*Let $ X_1, X_2 $ be two topological spaces; then for each $ a_1 \in X_1 $, the mapping $ x_2 \to (a_1, x_2) $ is a homeomorphism of $ X_2 $ onto the subspace $ \{a_1\} \times X_2 $ of $ X_1 \times X_2 $.*

This is a particular case of Corollary 1 of Proposition 1 of no. 1 applied to the constant function $ x_2 \to a_1 $.

The mapping $ x_2 \to (a_1, x_2) $ is a *continuous section* (\S\ 3, no. 5) with respect to the equivalence relation $ \mathrm{pr}_2 z = \mathrm{pr}_2 z' $ in $ X_1 \times X_2 $; the quotient space $ X_1 \times X_2 $ by this equivalence relation is therefore homeomorphic to $ X_2 $.

#### Corollary {#top-i-s4-n2-cor-1 .statement}

*The section $ A(x_1) $ of an open (resp. closed) set $ A $ of the product $ X_1 \times X_2 $ at an arbitrary point $ x_1 \in X_1 (*) $ is open (resp. closed) in $ X_2 $.*

#### Proposition 5 {#top-i-s4-prop-5 .statement}

*The projection of an open set $ U $ of the product $ X_1 \times X_2 $ onto either factor is an open set.*

For example, we have $ \mathrm{pr}_2 U = \bigcup_{x_1 \in X_1} U(x_1) $, and the proposition follows from the Corollary to Proposition 4 and axiom (O_1).

#### Remark 1 {#top-i-s4-n2-rem-1 .statement}

The projection of a *closed* subset of $ X_1 \times X_2 $ onto a factor *need not be closed*. For example, in the rational plane $ \mathbf{Q}^2 $, the hyperbola whose equation is $ x_1 x_2 = 1 $ is a closed set, but both its projections are equal to the complement of the point 0 in $ \mathbf{Q} $, and this is not a closed set.

(*) By the *section* $ A(x_1) $ of $ A $ at $ x_1 $ is meant the set of all $ x_2 \in X_2 $ such that $ (x_1, x_2) \in A $ (cf. Set Theory R, \S\ 3, no. 7).

#### Proposition 6 {#top-i-s4-prop-6 .statement}

Let $ X_1, X_2, Y $ be three topological spaces, $ f $ a mapping of the product space $ X_1 \times X_2 $ into $ Y $. If $ f $ is continuous at the point $ (a_1, a_2) $ then the partial mapping $ x_2 \to f(a_1, x_2) $ of $ X_2 $ into $ Y $ is continuous at the point $ a_2 $.

For this mapping is the composition of $ f $ and the mapping $ x_2 \to (a_1, x_2) $; hence the result follows from Proposition 4.

Proposition 6 is often expressed by saying that a continuous function of two variables is continuous with respect to each of them separately.

#### Remark 2 {#top-i-s4-n2-rem-2 .statement}

It is possible for all the partial mappings determined by a map $ f : X_1 \times X_2 \to Y $ to be continuous without $ f $ being continuous on $ X_1 \times X_2 $ (cf. Chapter IX, § 5, Exercise 23). \* For example if $ f $ is the mapping of the real plane $ \mathbf{R}^2 $ into $ \mathbf{R} $ defined by
$$
f(x, y) = xy/(x^2 + y^2) \quad \text{if} \quad (x, y) \neq (0, 0)
$$
and $ f(0, 0) = 0 $, then all the partial mappings are continuous; but $ f $ is not continuous at $ (0, 0) $, since $ f(x, x) = 1/2 $ if $ x \neq 0 $.

If $ g $ is a mapping of $ X_1 $ into $ Y $, continuous at a point $ a_1 $, then the mapping $ (x_1, x_2) \to g(x_1) $ of $ X_1 \times X_1 \to Y $ is continuous at all points $ (a_1, x_2) $, for it is the composition of $ g $ and the projection onto $ X_1 $.

The results of this subsection are easily extended to an arbitrary product $ \prod_{i \in I} X_i $ of topological spaces by remarking that this product is homeomorphic to the product $ \left( \prod_{i \in J} X_i \right) \times \left( \prod_{i \in K} X_i \right) $ for any partition $ (J, K) $ of $ I $ (no. 1, Proposition 2).

### 3. CLOSURE IN A PRODUCT

#### Proposition 7 {#top-i-s4-prop-7 .statement}

In a product space $ \prod_{i \in I} X_i $, the closure of a product of sets $ \prod_{i \in I} A_i $ is the same as the product $ \prod_{i \in I} \overline{A}_i $ of their closures.

Suppose that $ a = (a_i) $ lies in the closure of $ \prod_{i \in I} A_i $; then for each $ x \in I $, $ a_x = \operatorname{pr}_x a $ is in the closure of $ A_x $ because of the continuity of $ \operatorname{pr}_x $ (\S 2, no. 1, Theorem 1) and therefore $ a \in \prod_{i \in I} \overline{A}_i $. Conversely, let $ b = (b_i) \in \prod_{i \in I} \overline{A}_i $, and let $ \prod_{i \in I} V_i $ be any elementary set containing $ b $; for each $ i \in I $, $ V_i $ contains a point $ x_i \in A_i $; hence $ \prod_{i \in I} V_i $ contains the point $ (x_i) \in \prod_{i \in I} A_i $ and therefore $ b $ lies in the closure of $ \prod_{i \in I} A_i $.

#### Corollary {#top-i-s4-n3-cor-1 .statement}

*A product* $ \prod_{i \in I} A_i $ *of non-empty sets is closed in the product space* $ \prod_{i \in I} X_i $ *if and only if* $ A_i $ *is closed in* $ X_i $ *for each* $ i \in I $.

If $ I $ is *finite*, a product $ \prod_{i \in I} A_i $ is open provided that $ A_i $ is open in $ X_i $ for each $ i \in I $; but this is no longer so if $ I $ is infinite.

#### Proposition 8 {#top-i-s4-prop-8 .statement}

*Let* $ a = (a_i) $ *be any point of a product space* $ X = \prod_{i \in I} X_i $; *then the set* $ D $ *of points* $ x \in X $ *such that* $ \mathrm{pr}_i x = a_i $ *except for a finite number of indices* $ i $ *is dense in* $ X $.

For each $ x \in X $ and each elementary set $ V = \prod_{i \in I} U_i $ which contains $ x $, we have $ U_i = X_i $ except for indices $ i $ belonging to a finite subset $ J $ of $ I $; if we take $ y_i = x_i $ for $ i \in J $ and $ y_i = a_i $ for $ i \notin J $, it is clear that
$$
y = (y_i) \in D \quad \text{and} \quad y \in V;
$$
hence the result.

### 4. INVERSE LIMITS OF TOPOLOGICAL SPACES

Let $ I $ be a partially ordered (but not necessarily directed) set (*), in which the order relation is written $ \alpha \leq \beta $. For each $ \alpha \in I $, let $ X_\alpha $ be a topological space, and for each pair $ (\alpha, \beta) $ such that $ \alpha \leq \beta $ let $ f_{\alpha \beta} $ be a mapping of $ X_\beta $ into $ X_\alpha $. We say that $ (X_\alpha, f_{\alpha \beta}) $ is an *inverse system of topological spaces* if: 1) $ (X_\alpha, f_{\alpha \beta}) $ is an *inverse system of sets*; 2) $ f_{\alpha \beta} $ is a *continuous* mapping whenever $ \alpha \leq \beta $. Let $ X $ denote the set $ \varprojlim X_\alpha $, and for each $ \alpha \in I $ let $ f_\alpha $ be the canonical mapping $ X \to X_\alpha $; then the *coarsest* topology on $ X $ for which the $ f_\alpha $ are continuous is said to be the *inverse limit* (with respect to the $ f_{\alpha \beta} $) of the topologies of the $ X_\alpha $, and the set $ X $ with this topology is called the *inverse limit of the inverse system of topological spaces* $ (X_\alpha, f_{\alpha \beta}) $. Whenever we speak of $ \varprojlim X_\alpha $ as a topological space, it is always to be understood that the topology of this space is the inverse limit of the topologies of the $ X_\alpha $, unless the contrary is expressly stated.

The set $ X $ is the subset of the product $ \prod_{\alpha \in I} X_\alpha $ consisting of those points $ x $ such that
$$(1)$$
$$
\mathrm{pr}_\alpha(x) = f_{\alpha \beta}(\mathrm{pr}_\beta(x))
$$
whenever $ \alpha \leq \beta $. It follows from Proposition 3 of no. 1 that the inverse limit of the topologies of the $ X_\alpha $ is the same as the topology *induced* on $ X $ by the topology of the product space $ \prod_{\alpha \in I} X_\alpha $. If, for each $ \alpha \in I $, $ Y_\alpha $ is

(*) That is, a set endowed with a reflexive and transitive relation (*Set Theory* R, § 6, no. 1).

Let $ (X'_\alpha, f'_{\alpha\beta}) $ be another inverse system of topological spaces indexed by the same set $ I $, and for each $ \alpha \in I $ let $ u_\alpha : X_\alpha \to X'_\alpha $ be a *continuous* mapping such that $ (u_\alpha) $ is an *inverse system of mappings*; then $ u = \varprojlim u_\alpha $ is a continuous mapping of $ X = \varprojlim X_\alpha $ into $ X' = \varprojlim X'_\alpha $. For if $ f'_\alpha $ is the canonical mapping $ X' \to X'_\alpha $, we have $ f'_\alpha \circ u = u_\alpha \circ f_\alpha $, so that $ f'_\alpha \circ u $ is continuous for each $ \alpha \in I $, and the assertion follows from Proposition 4 of § 2, no. 3.

Finally, suppose $ I $ is a *directed* set, and let $ J $ be a *cofinal* subset of $ I $; let $ Z $ be the inverse limit of the inverse system of topological spaces $ (X_\alpha, f_{\alpha\beta})_{\alpha \in J, \beta \in J} $. Then the canonical bijection $ g : X \to Z $ (*Set Theory*, Chapter III, § 7, no. 2, proposition 3) is a *homeomorphism*. For we have $ \mathrm{pr}_\lambda(g(x)) = \mathrm{pr}_\lambda(x) $ for each $ \lambda \in J $; hence $ g $ is continuous (no. 1, Proposition 1); and if $ h $ is the inverse of $ g $, then for each $ \alpha \in I $ there exists $ \lambda \in J $ such that $ \alpha \leq \lambda $, and therefore $ \mathrm{pr}_\alpha(h(z)) = f_{\alpha\lambda}(\mathrm{pr}_\lambda(z)) $, which shows that $ h $ is continuous (no. 1, Proposition 1), since the $ f_{\alpha\lambda} $ are continuous.

#### Proposition 9 {#top-i-s4-prop-9 .statement}

*Let $ I $ be a directed set and $ J $ a cofinal subset of $ I $. Let $ (X_\alpha, f_{\alpha\beta}) $ be an inverse system of topological spaces indexed by $ I $; let $ X = \varprojlim X_\alpha $ and let $ f_\alpha : X \to X_\alpha $ be the canonical mapping. Then the family of sets $ f^{-1}_\alpha(U_\alpha) $, where $ \alpha $ runs through $ J $ and $ U_\alpha $ runs through a base $ \mathcal{B}_\alpha $ of the topology of $ X_\alpha $ for each $ \alpha \in J $, is a base of the topology of $ X $.*

From § 2, no. 3 we know that the *finite intersections* of sets of the form $ f^{-1}_\alpha(U_\alpha) $ ($ \alpha \in I, U_\alpha $ open in $ X_\alpha $) form a base of the topology of $ X $. If $ (\alpha_i)_{1 \leq i \leq n} $ is a finite family of indices of $ I $, then there exists $ \gamma \in J $ such that $ \alpha_i \leq \gamma $ for $ 1 \leq i \leq n $; hence $ f_{\alpha_i} = f_{\alpha_i\gamma} \circ f_\gamma $; if we put

$$
V_\gamma = \bigcap_i f^{-1}_{\alpha_i\gamma}(U_{\alpha_i}),
$$

then we have

$$
f^{-1}_\gamma(V_\gamma) = \bigcap_i f^{-1}_{\alpha_i}(U_{\alpha_i});
$$

but $ V_\gamma $ is open and is therefore a union of sets belonging to $ \mathcal{B}_\gamma $. Hence the result.

#### Corollary {#top-i-s4-n4-cor-1 .statement}

*Let $ A $ be a subset of $ X $ and let $ A_\alpha $ denote $ f_\alpha(A) $ for each $ \alpha \in I $. Then:*

(i) *The $ A_\alpha $ (resp. the $ \overline{A}_\alpha $) form an inverse system of subsets of the $ X_\alpha $, and*

$$
\overline{A} = \bigcap_\alpha f^{-1}_\alpha(\overline{A}_\alpha) = \varprojlim \overline{A}_\alpha.
$$

(ii) *If $ A $ is closed in $ X $, $ A = \varprojlim A_\alpha = \varprojlim \overline{A}_\alpha $.*

The first assertion of (i) follows from the relations $ f_\alpha = f_{\alpha\beta} \circ f_\beta $ for $ \alpha \leq \beta $ and from the continuity of the $ f_{\alpha\beta} $ (\S 2, no. 1, Theorem 1). Let $ A' $ denote
$$
\bigcap_\alpha \overline{f}_\alpha(\overline{A}_\alpha);
$$
then it is clear that $ A' $ is closed and contains $ A $, so that $ \overline{A} \subset A' $. Conversely, let $ x \in A' $; we have to show that $ x $ lies in the closure of $ A $. By virtue of Proposition 9 it is enough to prove that every neighbourhood of $ x $ which is of the form $ \overline{f}_\alpha(U_\alpha) $, with $ \alpha \in I $ and $ U_\alpha $ open in $ X_\alpha $, meets $ A $. Now, by hypothesis, $ f_\alpha(x) \in U_\alpha $, and since $ f_\alpha(x) \in \overline{A} $ we have $ U_\alpha \cap A_\alpha \neq \varnothing $, which means that $ A \cap \overline{f}_\alpha(U_\alpha) $ is not empty.

To establish (ii) it is enough to remark that, without any restriction on $ A $, we have $ A \subset \lim A_\alpha \subset \lim \overline{A}_\alpha $; now if $ A $ is closed, then from (i)
$$
A = \lim \overline{A}_\alpha
$$
and (ii) follows.

#### Example {#top-i-s4-n4-exa-1 .statement}

Let $ I $ be a directed set and $ (X_\alpha)_{\alpha \in I} $ a family of subsets of a set $ Y $, such that $ X_\alpha \supset X_\beta $ whenever $ \alpha \leq \beta $. For each $ \alpha \in I $ let $ \mathcal{T}_\alpha $ be a topology on $ X_\alpha $ such that $ \mathcal{T}_\beta $ is finer than the topology induced on $ X_\beta $ by $ \mathcal{T}_\alpha $ whenever $ \alpha \leq \beta $. If we take $ f_{\alpha\beta} $ to be the canonical injection $ X_\beta \to X_\alpha $ for $ \alpha \leq \beta $, then $ \lim X_\alpha $ may be identified canonically with the *intersection* $ X $ of the $ X_\alpha $, with the topology which is the *least upper bound* (\S 2, no. 3, Example 2) of the topologies induced on $ X $ by the $ \mathcal{T}_\alpha $.

### Exercises {#top-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
