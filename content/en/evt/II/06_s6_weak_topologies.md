---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 6
section_title: Weak topologies
lang: en
source: evt-i-v
book_pages: TVS II.40-TVS II.53, TVS II.81-TVS II.86
pdf_pages: 0077-0090, 0118-0123
extraction: ocr
subsections:
    - "no": 1
      title: Dual vector spaces
      page: 40
      pdf_page: 77
    - "no": 2
      title: Weak topologies
      page: 42
      pdf_page: 79
    - "no": 3
      title: Polar sets and orthogonal subspaces
      page: 44
      pdf_page: 81
    - "no": 4
      title: Transposition of a continuous linear mapping
      page: 46
      pdf_page: 83
    - "no": 5
      title: Quotient spaces and subspaces of a weak space
      page: 48
      pdf_page: 85
    - "no": 6
      title: Products of weak topologies
      page: 50
      pdf_page: 87
    - "no": 7
      title: Weakly complete spaces
      page: 51
      pdf_page: 88
    - "no": 8
      title: Complete convex cones in weak spaces
      page: 52
      pdf_page: 89
statements: 39
exercises: 20
content_sha256: 1049b16ea7f3d1d52a3697fbbb8908ee491814e70eb0fc2b3e5904bc50517937
---

## § 6. WEAK TOPOLOGIES

### 1. Dual vector spaces

Let $ F $ and $ G $ be two real vector spaces and let $ (x, y) \mapsto B(x, y) $ be a *bilinear* form on $ F \times G $. We say that the bilinear form $ B $ *puts the vector spaces* $ F $ *and* $ G $ *in duality*, or that F and G are in duality (relative to B). Recall that we say that $ x \in F $ and $ y \in G $ are orthogonal (for the duality defined by B) if $ B(x, y) = 0 $; we say that a subset M of F and a subset N of G are orthogonal if every $ x \in M $ is orthogonal to every $ y \in N $ (A, IX, § 1.2).

We say that the duality defined by B is separating in F (resp. in G) if it satisfies the following condition :

(D_I) *For every $ x \neq 0 $ in F, there exists $ y \in G $ such that $ B(x, y) \neq 0 $.* (resp.

(D_{II}) *For every $ y \neq 0 $ in G, there exists $ x \in F $ such that $ B(x, y) \neq 0 $.)

The duality defined by B is said to be separating if it is both separating in F and in G. For this to be so, it is necessary and sufficient that the bilinear form B should be separating in the sense of A, IX, § 1.1. More precisely we have the following result :

#### Proposition 1 {#evt-ii-s6-prop-1 .statement}

*Let F, G be two real vector spaces and B a bilinear form on $ F \times G $. Let*

$$
d_B : y \mapsto B(., y),
$$
$$
s_B : x \mapsto B(x, .)
$$

*be linear mappings of G in the dual $ F^* $ of F and of F in the dual $ G^* $ of G, associated respectively to the right and to the left of B* (A, IX, § 1.1). Then B puts F and G in a duality separating in G (resp. in F), if and only if $ d_B $ (resp. $ s_B $) is injective.*

When F and G are put in separating duality by B, we often identify F (resp. G) with a subspace of $ G^* $ (resp. $ F^* $) by means of $ s_B $ (resp. $ d_B $). When we consider F (resp. G) as a subspace of $ G^* $ (resp. $ F^* $) without specifying how this identification is to be made, we are always using the preceding identifications; the bilinear form B is then identified with the restriction to $ F \times G $ of the canonical bilinear form :

$$
(x^*, x) \mapsto \langle x, x^* \rangle \quad (\text{resp. } (x, x^*) \mapsto \langle x, x^* \rangle).
$$

#### Example {#evt-ii-s6-n1-exa-1 .statement}

— 1) Let E be a vector space and let E* be its dual. The canonical bilinear form $ (x, x^*) \mapsto \langle x, x^* \rangle $ on $ E \times E^* $ (A, II, § 2.3) puts E and E* in separating duality : for (D_{II}) is true because of the definition of the relation $ x^* \neq 0 $, and we know on the other hand, that for all $ x \neq 0 $ in E, there exists a linear form $ x^* \in E^* $ such that $ \langle x, x^* \rangle \neq 0 $ (A, II, § 7.5, th. 6), which proves (D_I); the identifications of E with a subspace of $ E^{**} $ is made here by the canonical mapping $ c_E $ (*loc. cit.*).

When E is of *finite* dimension, the *only* subspace G of E* that is in separating duality by the restriction to $ E \times G $ of the canonical bilinear form, is the space E* itself ; for, E being then canonically identified with $ E^{**} $ (*loc. cit.*), if we had $ G \neq E^* $, there would exist $ a \neq 0 $ in E such that $ \langle a, x^* \rangle = 0 $ for all $ x^* \in G $ (A, II, § 7.5, th. 7), which contradicts the hypothesis.

2) When E is an *infinite* dimensional vector space, and E' is a vector subspace of E*, the duality between E and E' defined by the restriction to $ E \times E' $ of the canonical bilinear form is always separating in E' ; it can be separating in E even if $ E' \neq E^* $. The most important case occurs where E is a topological vector space.

#### Definition 1 {#evt-ii-s6-def-1 .statement}

— *By the dual of a topological vector space E, we mean the subspace E' of E*, the dual of the vector space E, formed by the continuous linear forms on E.*

When E is a *Hausdorff locally convex* space, the duality between E and its dual E' is separating : this follows from the Hahn-Banach theorem (II, p. 24, cor. 1) that for every $ x \neq 0 $ in E, there exists $ x' \in E' $ such that $ \langle x, x' \rangle \neq 0 $.

#### Remark {#evt-ii-s6-n1-rem-1 .statement}

— 1) When E is a *topological* vector space, the dual $ E^* $ of the *vector space* E will be called the *algebraic dual* of E to avoid confusion. We note also that $ E^* $ is the dual of the topological vector space obtained by giving E the *finest* locally convex topology (II, p. 25, *Example* 2).
2) The dual E' of a topological vector space does not itself carry a topology, unless this is expressly stated.
3) If F and $ G \subset F^* $ are in separating duality by the canonical bilinear form, then this is also true of F and $ G_1 $, for every subspace $ G_1 $ of $ F^* $ such that $ G \subset G_1 $.

### 2. Weak topologies

#### Definition 2 {#evt-ii-s6-def-2 .statement}

— *Let F and G be two vector spaces put in duality by the bilinear form B. The coarsest topology on F that makes all the linear forms $ B(., y): x \mapsto B(x, y) $ continuous, where y varies in G, is called the weak topology on F defined by the duality between F and G, and we denote it by $ \sigma(F, G) $.*

Similarly we define the weak topology $ \sigma(G, F) $ on G, interchanging F and G in definition 1 ; this possibility of interchanging F and G applies to all the results and definitions that follow in this paragraph.

We use the adjective « weak » and the adverb « weakly » to denote properties relative to a weak topology $ \sigma(F, G) $ provided there is no possibility of confusion. We shall speak, for example, of « weak convergence » and « weakly continuous functions » etc.

When $ G \subset F^* $, the notation $ \sigma(F, G) $ will always denote the weak topology defined by the duality corresponding to the restriction to $ F \times G $ of the canonical bilinear form $ (x, x^*) \mapsto \langle x, x^* \rangle $.

Without extra hypotheses on F and G, we often write $ \langle x, y \rangle $ for the value $ B(x, y) $ of the bilinear form B at $ (x, y) $, provided there is no ambiguity ; we shall adopt this convention in the rest of this paragraph.

A vector space F carrying a weak topology of $ \sigma(F, G) $ will be called a *weak space*.

A weak topology $ \sigma(F, G) $ is *locally convex* (II, p. 26, prop. 4) ; more precisely, it is the inverse image of the *product* topology of $ \mathbf{R}^G $ by the linear mapping $ \phi : x \mapsto (\langle x, y \rangle)_{y \in G} $ of F in $ \mathbf{R}^G $. It is defined by the set of *semi-norms* $ x \mapsto |\langle x, y \rangle| $ when y varies in G (II, p. 5). For every $ \alpha > 0 $, and every finite family $ (y_i)_{1 \leq i \leq n} $ of points of G, let $ W(y_1, ..., y_n; \alpha) $ be the set of the $ x \in F $ such that $ |\langle x, y_i \rangle| \leq \alpha $ for $ 1 \leq i \leq n $; these sets (for $ \alpha, n $ and $ y_i $ arbitrary) form a *fundamental system of neighbourhoods of* 0 for $ \sigma(F, G) $. Note that $ W(y_1, ..., y_n; \alpha) $ contains that *vector subspace* of F, of *finite* codimension, which is defined by the equations $ \langle x, y_i \rangle = 0 $ for $ 1 \leq i \leq n $.

#### Proposition 2 {#evt-ii-s6-prop-2 .statement}

— *The weak topology* $ \sigma(F, G) $ *is Hausdorff if and only if the duality between* $ F $ *and* $ G $ *is separating in* $ F $.

This is a particular case of II, p. 3, prop. 2.

#### Proposition 3 {#evt-ii-s6-prop-3 .statement}

— *Let* $ F $ *and* $ G $ *be two real vector spaces in duality. Every linear form on* $ F $, *that is continuous for* $ \sigma(F, G) $, *can be written as* $ x \mapsto \langle x, y \rangle $ *for some* $ y \in G $. *The element* $ y \in G $ *is unique when the duality is separating in* $ G $.

For, to say that the linear form $ f $ on $ F $ is continuous for $ \sigma(F, G) $ means that there exists a finite set of points $ y_i \in G $ ($ 1 \leq i \leq n $) such that, for all $ x $ in $ F $, $ |f(x)| \leq \sup_{1 \leq i \leq n} |\langle x, y_i \rangle| $ (II, p. 6, prop. 5). The $ n $ relations $ \langle x, y_i \rangle = 0 $ ($ 1 \leq i \leq n $) imply therefore $ f(x) = 0 $, and hence (A, II, § 7.5, cor. 1), there exists a linear combination $ y = \sum_{i=1}^n \lambda_i y_i $ such that $ f(x) = \langle x, y \rangle $ for all $ x \in F $. The uniqueness follows from (D$_\text{II}$).

In other words, when the duality is separating in $ G $, and $ F $ has the topology $ \sigma(F, G) $, then we can identify $ G $ canonically with the dual of $ F $ for this topology (II, p. 42, def. 1).

#### Corollary 1 {#evt-ii-s6-prop-3-cor-1 .statement}

— *A family* $ (a_i) $ *of points of* $ F $ *is total for the topology* $ \sigma(F, G) $ *if, and only if, for every* $ y \neq 0 $ *in* $ G $, *there exists an index* $ i $ *such that* $ \langle a_i, y \rangle \neq 0 $.

For using prop. 3 and I, p. 13, th. 1, the property expresses the fact that for $ \sigma(F, G) $ no closed hyperplane contains all the $ a_i $; the corollary follows therefore from cor. 3 of II, p. 38.

#### Corollary 2 {#evt-ii-s6-prop-3-cor-2 .statement}

— *A family* $ (a_i) $ *of points of* $ F $ *is topologically independent for the topology* $ \sigma(F, G) $, *if, and only if, for every index* $ i $, *there exists an element* $ b_i \in G $ *such that* : $ \langle a_i, b_i \rangle \neq 0 $ *and* $ \langle a_\kappa, b_i \rangle = 0 $ *for all* $ \kappa \neq i $.

This means, that for all $ i $, there exists a closed hyperplane in $ \sigma(F, G) $, which contains all the $ a_\kappa $ with index $ \kappa \neq i $ but does not contain $ a_i $.

#### Corollary 3 {#evt-ii-s6-prop-3-cor-3 .statement}

— *Let* $ G_1 $ *and* $ G_2 $ *be two vector subspaces of* $ F^* $, *in duality with* $ F $ *(for the restriction of the canonical bilinear form)*. *Then* $ \sigma(F, G_2) $ *is finer than* $ \sigma(F, G_1) $ *if and only if* $ G_1 \subset G_2 $.

The condition is obviously sufficient; conversely, if $ \sigma(F, G_2) $ is finer than $ \sigma(F, G_1) $, then every linear form that is continuous for $ \sigma(F, G_1) $ is also continuous for $ \sigma(F, G_2) $, hence $ G_1 \subset G_2 $ by prop. 3.

#### Corollary 4 {#evt-ii-s6-prop-3-cor-4 .statement}

— *Let* $ G $ *be a vector subspace of the dual* $ F^* $, *of the vector space* $ F $. *Then* $ F $ *and* $ G $ *are in separating duality* (for the canonical bilinear form) *if, and only if,* $ G $ *is dense in* $ F^* $ *in the topology* $ \sigma(F^*, F) $.

This follows from cor. 1.

### 3. Polar sets and orthogonal subspaces

Definition 2. — Let F and G be two (real) vector spaces in duality. For every set M of F we call the polar of M, the set of those y ∈ G for which $ \langle x, y \rangle \geq -1 $ for all $ x \in M $. (For complex vector spaces, cf. II, p. 64.)

If $ G_1, G_2 $ are two subspaces of $ F^* $ such that $ G_1 \subset G_2 $, then the polar of M in $ G_1 $ is the intersection of $ G_1 $ with the polar of M in $ G_2 $.

When there is no danger of confusion we use $ M^\circ $ to denote the polar, in G, of the subset M of F. Similarly we define the polar in F of a set in G.

Obviously, for every scalar $ \lambda \neq 0 $ and all $ M \subset F $, we have $ (\lambda M)^\circ = \lambda^{-1} M^\circ $. The relation $ M \subset N \subset F $ implies $ N^\circ \subset M^\circ $; if N absorbs M then $ M^\circ $ absorbs $ N^\circ $; for every family $ (M_\alpha) $ of sets of F, the polar set of $ \bigcup \alpha M_\alpha $ is the intersection of the polar sets $ M_\alpha^\circ $. Since, for $ y \in M^\circ $, the closed half-spaces defined by the relations $ \langle x, y \rangle \geq -1 $ contain 0 and M, we see that if $ M_1 $ is the convex envelope of $ M \cup \{0\} $, then $ M_1^\circ = M^\circ $.

Clearly $ M \subset M^{\circ \circ} $. Hence
$$
(M^{\circ \circ})^\circ \subset M^\circ \subset (M^\circ)^{\circ \circ} = (M^{\circ \circ})^\circ
$$
i.e. $ M^{\circ \circ \circ} = M^\circ $ (cf. S, III, § 1.5, prop. 2).

If M is a symmetric subset of F, $ M^\circ $ is a symmetric subset of G; $ M^\circ $ is also in this case the set of $ y \in G $ such that $ |\langle x, y \rangle| \leq 1 $ for all $ x \in M $.

Proposition 4. — (i) For any set M of F, the polar set $ M^\circ $ is a convex set that contains 0 and is closed in G for the topology $ \sigma(G, F) $.

(ii) If M is a cone of vertex 0, then $ M^\circ $ is a cone of vertex 0 and it is also the set of $ y \in G $ such that $ \langle x, y \rangle \geq 0 $ for all $ x \in M $.

(iii) If M is a vector subspace of F, then $ M^\circ $ is a vector subspace of G, and it is also the set of $ y \in G $ such that $ \langle x, y \rangle = 0 $ for all $ x \in M $.

(i) Since the linear forms $ y \mapsto \langle x, y \rangle $ are continuous for $ \sigma(G, F) $ the statement follows immediately from the definitions and the fact that a half-space determined by a hyperplane is convex.

(ii) If M is a cone with vertex 0 and if $ x \in M, y \in M^\circ $, then as $ \lambda x \in M $, for all $ \lambda > 0 $, we have $ \langle \lambda x, y \rangle \geq -1 $, i.e. $ \lambda \langle x, y \rangle \geq -1 $. Since this holds for all $ \lambda > 0 $, it follows that $ \langle x, y \rangle \geq 0 $, and (ii) is proved.

(iii) Similarly, if M is a vector subspace of F, the relations $ x \in M, y \in M^\circ $ imply, this time, that $ \lambda \langle x, y \rangle \geq -1 $ for all real $ \lambda $ which is possible only if $ \langle x, y \rangle = 0 $.

If M is a vector subspace of F we say that $ M^\circ $ is the orthogonal of M in G; if $ G \subset F^* $, then $ M^\circ $ is the intersection of G, and of the subspace orthogonal to M in the algebraic dual $ F^* $ of F (A, II, § 2.4, def. 4).

For a vector subspace M of F and a vector subspace N of G we say that M and N are orthogonal if $ M \subset N^o $ (or, equivalently, if $ N \subset M^\circ $).

#### Theorem 1 (The bipolar theorem) {#evt-ii-s6-thm-1 .statement}

Let F, G be two real vector spaces in duality. For every subset M of F the polar set $ M^{\circ \circ} $ in F of the polar set $ M^\circ $ of M in G is the closed convex envelope (for $ \sigma(F, G) $) of $ M \cup \{0\} $.

We have seen that we need only consider the case where $ M $ is convex and $ 0 \in M $. Denote the closure, in topology $ \sigma(F, G) $ of $ M $ by $ \overline{M} $, then $ \overline{M} $ is a convex set in $ F $; prop. 4 of II, p. 44 shows that $ M^{\circ\circ} \supseteq \overline{M} $. On the other hand if $ a \in F $ does not belong to $ \overline{M} $ then there exists a closed hyperplane $ H $ in $ F $ which separates $ a $ strictly from $ \overline{M} $ (II, p. 38, prop. 4); since $ H $ does not contain 0, there exists $ y \in G $ such that $ H $ has the equation $ \langle x, y \rangle = -1 $ (II, p. 43, prop. 3); thus $ \langle x, y \rangle > -1 $ for all $ x \in \overline{M} $ and $ \langle a, y \rangle < -1 $. This implies that $ y \in M^\circ $ and $ a \notin M^{\circ\circ} $, and the relation $ M^{\circ\circ} = \overline{M} $ follows.

#### Corollary 1 {#evt-ii-s6-thm-1-cor-1 .statement}

*For any family* $ (M_\alpha) $ *of closed convex sets of* $ F $ *(in the topology* $ \sigma(F, G) $*), each containing* 0, *the polar set of the intersections* $ M = \bigcap \limits_{\alpha} M_\alpha $ *is the convex closed envelope* (*for* $ \sigma(G, F) $) *of the union of the* $ M_\alpha^\circ $.

For, if $ N $ is this convex closed envelope, then

$$
N^\circ = \bigcap \limits_{\alpha} M_\alpha^{\circ\circ} = \bigcap \limits_{\alpha} M_\alpha = M
$$

whence $ N = N^{\circ\circ} = M^\circ $.

The conclusion of cor. 1 does not necessarily hold if the $ M_\alpha $ are not convex.

#### Corollary 2 {#evt-ii-s6-thm-1-cor-2 .statement}

*For every vector subspace* $ M $ *of* $ F $, *the subspace* $ M^{\circ\circ} $ *is the closure of* $ M $ *in the topology* $ \sigma(F, G) $.

#### Remark {#evt-ii-s6-n3-rem-1 .statement}

— Every neighbourhood of 0 in $ G $ in the topology $ \sigma(G, F) $ contains a neighbourhood $ V $ defined by a finite number of inequalities of the form $ |\langle x_i, y \rangle| \leq 1 $ ($ 1 \leq i \leq n $), where the $ x_i $ are arbitrary points of $ F $. If $ A $ is the *symmetric convex envelope* of the set of the $ x_i $, then $ V $ is the *polar set* $ A^\circ $ of $ A $ in $ G $. We can say that the *polars in* $ G $ *of finite symmetric sets in* $ F $ (or of their convex envelopes) form a fundamental system of neighbourhoods of 0 in $ G $ for $ \sigma(G, F) $. If the duality is separating in $ F $, these convex envelopes are *compact* for $ \sigma(F, G) $ (II, p. 14, cor. 1 of prop. 15), and of finite dimensions. Conversely every *compact, convex set of finite dimension* $ C $ in $ F $ (with the $ \sigma(F, G) $ topology) is contained in the convex envelope of a *finite subset* of $ F $. For, let $ M $ be a vector subspace of finite dimension containing $ C $. If $ (e_i)_{1 \leq i \leq n} $ is a basis of $ M $, we can suppose that $ C $ is contained in the closed parallelope centre 0 and constructed on the vectors of the basis $ e_i $ (GT, VI, § 1.3); now it is immediate that this parallelope is the convex envelope of the points $ \sum \limits_{i=1}^n \varepsilon_i e_i $ with $ \varepsilon_i = \pm 1 $.

Thus we can say that (if $ \sigma(F, G) $ is Hausdorff) *the polars of finite dimensional, convex, compact sets in* $ F $ (for $ \sigma(F, G) $ or for any Hausdorff locally convex topology finer than $ \sigma(F, G) $ on $ F $) form a fundamental system of neighbourhoods of 0 for $ \sigma(G, F) $.

#### Corollary 3 {#evt-ii-s6-thm-1-cor-3 .statement}

*Let* $ \mathcal{T} $ *be the topology of a locally convex space* $ E $ *and let* $ E' $ *be its dual* (II, p. 42, def. 1).

(i) *The closed convex sets in E are the same for the topology $ \mathcal{T} $ and for the weak topology $ \sigma(E, E') $.

(ii) *For every subset M of E, the polar set $ M^{\circ\circ} $ in E of the polar set $ M^\circ $ of M in $ E' $, is the convex closed envelope of $ M \cup \{0\} $ for the topology $ \mathcal{T} $.

Clearly, (ii) follows from (i) and th. 1. From the definition of the dual $ E' $, it follows from II, p. 43, prop. 3 that the continuous linear forms on E for the topology $ \mathcal{T} $ are the same as the continuous linear forms for $ \sigma(E, E') $. The closed half-spaces in E are therefore the same for $ \mathcal{T} $ and for $ \sigma(E, E') $ (II, p. 15, prop. 17) and the assertion (i) follows therefore from II, p. 38, cor. 1.

### 4. Transposition of a continuous linear mapping

In this No., we suppose that (F, G) and $ (F_1, G_1) $ are two vector spaces in duality.

#### Proposition 5 {#evt-ii-s6-prop-5 .statement}

*Let u be a linear mapping of F in $ F_1 $. The following properties are equivalent :*

a) *u is continuous for the weak topologies $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $;*

b) *there exists a mapping $ v : G_1 \to G $ such that*

$$
\langle u(y), z_1 \rangle = \langle y, v(z_1) \rangle
$$

for all $ y \in F $ and $ z \in G_1 $.

*If these properties hold and if the duality between F and G is separating in G, then the mapping v satisfying (1) is unique, and v is linear.*

If u is continuous for the weak topologies, then, for all $ z_1 \in G_1 $, the linear form $ y \mapsto \langle u(y), z_1 \rangle $ on F is continuous for $ \sigma(F, G) $, thus (II, p. 43, prop. 3) can be written as $ y \mapsto \langle y, v(z_1) \rangle $ with $ v(z_1) \in G $, which shows that a) implies b). Conversely, if b) is true, for all $ z_1 \in G_1 $, the linear form

$$
y \mapsto \langle y, v(z_1) \rangle = \langle u(y), z_1 \rangle
$$

is continuous for $ \sigma(F, G) $ : it follows from the definition of weak topologies that u is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $ (I, p. 10, cor. 1). The uniqueness of v follows from (D_{II}) and this uniqueness implies that v is linear.

#### Remark {#evt-ii-s6-n4-rem-1 .statement}

— Suppose that the duality between F and G is separating in G and that the duality between $ F_1 $ and $ G_1 $ is separating in $ G_1 $. If we identify G and $ G_1 $ with subspaces of $ F^* $ and $ F_1^* $ respectively, the conditions a) and b) are equivalent to $ ^t u(G_1) \subset G $; v is the restriction of the transpose $ ^t u $ of u (A, II, § 2.5) to $ G_1 $.

We say, simply (when there is no chance of confusion) that v is the *transpose* of u (relative to the duality on the one hand between F and G and on the other hand between $ F_1 $ and $ G_1 $) and we again use $ ^t u $ to denote it.

#### Corollary {#evt-ii-s6-n4-cor-1 .statement}

*Suppose that the duality between F and G is separating in G. If u is a linear mapping of F in $ F_1 $, that is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $, then its* transpose is a linear mapping of $ G_1 $ in $ G $, that is continuous for $ \sigma(G_1, F_1) $ and $ \sigma(G, F) $. Further if the duality between $ F_1 $ and $ G_1 $ is separating in $ F_1 $ then $ {}^t({}^t u) = u $.

It is sufficient to exchange $ F $ and $ F_1 $ with $ G $ and $ G_1 $ in prop. 5.

#### Proposition 6 {#evt-ii-s6-prop-6 .statement}

*Suppose that the duality between $ F $ and $ G $ (resp. $ F_1 $ and $ G_1 $) is separating in $ G $ (resp. $ F_1 $). Let $ u $ be a linear mapping of $ F $ in $ F_1 $ that is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $. Let $ A $ be a set in $ F $ and $ A_1 $ a set in $ F_1 $; then*:

(i) *We have $ (u(A))^{\circ} = {}^t u^{-1}(A^{\circ}) $.*

(ii) *We have $ {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} $; further, if $ A $ is closed, (for $ \sigma(F_1, G_1) $) convex, and contains the origin, then we have $ {}^t u(A_1^{\circ}) = (u^{-1}(A_1))^{\circ} $.*

Let $ z_1 \in G_1 $, the relation $ z_1 \in (u(A))^{\circ} $ is equivalent to $ \langle u(y), z_1 \rangle \geq -1 $ for all $ y \in A $, and the relation $ {}^t u(z_1) \in A^{\circ} $ is equivalent to $ \langle y, {}^t u(z_1) \rangle \geq -1 $ for all $ y \in A $ and our assertion (i) follows using (1). Next interchanging $ u $ and $ {}^t u $ and applying (i) to the set $ A_1^{\circ} $ of $ G_1 $ we get

$$
({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ}) \supset u^{-1}(A_1)
$$

from which, on taking polars

$$
({}^t u(A_1^{\circ}))^{\circ \circ} \subset (u^{-1}(A_1))^{\circ} .
$$

We have $ {}^t u(A_1^{\circ}) \subset ({}^t u(A_1^{\circ}))^{\circ \circ} $ by the bipolar theorem (II, p. 44, th. 1); the final statement follows from (2) and the bipolar theorem since then $ A_1^{\circ \circ} = A_1 $ and $ {}^t u(A_1^{\circ}) $ is convex and contains the origin.

#### Corollary 1 {#evt-ii-s6-prop-6-cor-1 .statement}

*With the notations of prop. 6, the relation $ u(A) \subset A_1 $ implies $ {}^t u(A_1^{\circ}) \subset A^{\circ} $; if further $ A_1 $ is convex, closed (for $ \sigma(F_1, G_1) $) and contains the origin, then these two relations are equivalent.*

In fact, the relation $ u(A) \subset A_1 $ equivalent to $ A \subset u^{-1}(A_1) $, therefore implies

$$
{}^t u(A_1^{\circ}) \subset {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} \subset A^{\circ}
$$

and conversely the relation $ {}^t u(A_1^{\circ}) \subset A^{\circ} $ implies

$$
A^{\circ \circ} \subset ({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ})
$$

from (2). When $ A_1 = A_1^{\circ \circ} $, we deduce that $ A \subset u^{-1}(A_1) $.

#### Corollary 2 {#evt-ii-s6-prop-6-cor-2 .statement}

*Let $ u $ be a linear mapping of $ F $ in $ F_1 $ that is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $. We have then*

(3)

$$
\operatorname{Ker}({}^t u) = (\operatorname{Im}(u))^{\circ} ,
$$

(4)

$$
\overline{\operatorname{Im}({}^t u)} = (\operatorname{Ker}(u))^{\circ} .
$$

*Suppose that the dualities between $ F $ and $ G $ and between $ F_1 $ and $ G_1 $ are separating; then $ u(F) $ is dense in $ F_1 $ (for $ \sigma(F_1, G_1) $), if and only if $ {}^t u $ is injective.*

Apply prop. 6 with $ A = F $ and $ A_1 = \{0\} $, using the fact that the weak topologies $ \sigma(G, F) $ and $ \sigma(F_1, G_1) $ are Hausdorff. The last assertion results from (4), interchanging $ u $ and $ ^t u $.

### 5. Quotient spaces and subspaces of a weak space

Let $ F, G $ be two real vector spaces in duality. Let $ M $ be a vector subspace of $ F $, and consider the subspace $ N $ of the orthogonal $ M^\circ $ in $ G $; if $ y_1, y_2 $ are two points of $ G $ that are congruent mod. $ N $ then $ \langle x, y_1 \rangle = \langle x, y_2 \rangle $ for all $ x \in M $. For each class $ \dot{y} $ mod. $ N $, denote the common value of $ \langle x, y \rangle $ when $ y $ varies in $ \dot{y} $ by $ \langle x, \dot{y} \rangle $; clearly $ (x, \dot{y}) \mapsto \langle x, \dot{y} \rangle $ is a bilinear form on $ M \times (G/N) $.

#### Proposition 7 {#evt-ii-s6-prop-7 .statement}

— *Let $ M $ be a vector subspace of $ F $ and $ N $ a vector subspace of $ G $ where $ F $ and $ G $ are two vector spaces in duality. Suppose that $ M $ and $ N $ are orthogonal (which is equivalent to saying that $ N \subset M^\circ $, or $ M \subset N^\circ $). The vector spaces $ M $ and $ G/N $ are then in duality by the bilinear form* $ (x, \dot{y}) \mapsto \langle x, \dot{y} \rangle $.

(i) *The topology $ \sigma(M, G/N) $ for this duality is induced by $ \sigma(F, G) $ (and in particular we have $ \sigma(F, G) = \sigma(F, G/F^\circ) $).

(ii) *The topology $ \sigma(G/N, M) $ for this duality is coarser than the quotient topology of $ \sigma(G, F) $ by $ N $; these topologies are identical if and only if $ M + G^\circ = N^\circ $.

(i) Every element of $ G/N $ is a class mod. $ N $ of an element of $ G $; if $ z_i (1 \leq i \leq n) $ are elements of $ G $ and $ \dot{z}_i (1 \leq i \leq n) $ is the class of $ z_i $ in $ G/N $ then the set of $ y \in M $ such that $ |\langle y, \dot{z}_i \rangle| \leq \alpha $ for $ 1 \leq i \leq n $ is the trace on $ M $ of the set of those $ x \in F $ such that $ |\langle x, z_i \rangle| \leq \alpha $ for $ 1 \leq i \leq n $; the conclusion follows from the definition of neighbourhoods of 0 for the weak topology.

(ii) Let $ p : G \to G/N $ be the canonical surjection. We show that the *quotient topology* $ \mathcal{T} $ *of* $ \sigma(G, F) $ *by* $ N $ *is identical with* $ \sigma(G/N, N^\circ) $. As, for $ z \in G, y \in N^\circ $, we have $ \langle y, p(z) \rangle = \langle y, z \rangle $, it follows that every neighbourhood of 0 for $ \sigma(G/N, N^\circ) $ is of the form $ p(V) $, where $ V $ is a neighbourhood of 0 for $ \sigma(G, F) $ saturated for the relation $ z - z' \in N $, therefore $ \mathcal{T} $ is finer than $ \sigma(G/N, N^\circ) $. Conversely let $ U = W(y_1, ..., y_n; \alpha) $ be a neighbourhood of 0 in $ G $ for $ \sigma(G, F) $, where $ y_i \in F $ for $ 1 \leq i \leq n $ and $ \alpha > 0 $; we are going to see that for $ 1 \leq i \leq n $, there exist elements $ t_i \in N^\circ $ such that if one puts $ U' = W(t_1, ..., t_n; \alpha) $, then $ p(U') \subset p(U) $; this will show that $ \sigma(G/N, N^\circ) $ is finer than $ \mathcal{T} $ and therefore is actually identical with $ \mathcal{T} $. Now, let $ L $ be the vector subspace of $ F $ generated by $ N^\circ $ and the $ y_i $, and denote by $ P $ the complementary subspace of $ N^\circ $ in $ L $; it is of finite dimension, say $ m $. Let $ (x_j)_{1 \leq j \leq m} $ be a basis of $ P $; the restrictions to $ N $ of the linear forms $ x \mapsto \langle x_j, z \rangle $ are linearly independent, since otherwise there exists $ x \neq 0 $ in $ P $ such that $ \langle x, z \rangle = 0 $ for all $ z \in N $, that is to say $ x \in N^\circ $, which contradicts the definition of $ P $. Thus we conclude that for all $ z' \in G $, there exists $ s \in N $ such that $ \langle x_j, z' \rangle = \langle x_j, s \rangle $ for all $ j $; if $ z' = z + s $, we have $ \langle x, z \rangle = 0 $ for all $ x \in P $. This being so, put $ y_i = t_i + w_i $, where $ t_i \in N^\circ $ and $ w_i \in P $; we have $ \langle y_i, z \rangle = \langle t_i, z \rangle = \langle t_i, z' \rangle $ for $ 1 \leq i \leq n $; therefore, for all $ z' \in U' $, there exists $ z \in U $ such that $ z' - z \in N $, that is to say we have $ p(U') \subset p(U) $.

Returning to the case where M is any subspace of N°, note that evidently $ \sigma(G/N, M) = \sigma(G/N, M + G^\circ) $; further, from prop. 3 of II, p. 43, we see that, if $ y \in N^\circ $ is such that the linear form $ \dot{z} \mapsto \langle y, \dot{z} \rangle $ is continuous for $ \sigma(G/N, M) $, then necessarily $ y \in M + G^\circ $. We conclude that the condition $ M + G^\circ = N^\circ $ is necessary and sufficient for the quotient topology $ \mathcal{T} $ to be equal to $ \sigma(G/N, M) $.

#### Remark {#evt-ii-s6-n5-rem-1 .statement}

— The duality between M and G/N (where M and N are two orthogonal subspaces) is separating in M, if and only if $ M \cap G^\circ = \{0\} $; it is separating in G/N, if and only if $ N = M^\circ $.

#### Corollary 1 {#evt-ii-s6-prop-7-cor-1 .statement}

— Suppose that the duality between F and G is separating in F. For a vector subspace M of F the topology $ \sigma(G/M^\circ, M) $ is identical with quotient topology of $ \sigma(G, F) $ by $ M^\circ $, if and only if M is closed for the topology $ \sigma(F, G) $.

This follows from prop. 7 putting $ N = M^\circ $, and recalling that $ M^{\circ \circ} $ is the closure of M for $ \sigma(F, G) $ (II, p. 45, cor. 2).

#### Corollary 2 {#evt-ii-s6-prop-7-cor-2 .statement}

— If M is of finite dimension n and the duality is separating in F, then $ M^\circ $ is of codimension n in G. If M is closed for $ \sigma(F, G) $ and of finite codimension n and if the duality is separating in G, then $ M^\circ $ is of dimension n.

For, $ G/M^0 $ is in separating duality with M; if M is of dimension n, the same is therefore true of $ G/M^\circ $ (II, p. 41, example 1). If M is closed, $ F/M = F/M^{\circ \circ} $ is in separating duality with $ M^\circ $; if F/M is of dimension n, it is therefore the same for $ M^\circ $ (II, p. 41, example 1).

#### Corollary 3 {#evt-ii-s6-prop-7-cor-3 .statement}

— Let (F, G), (F_1, G_1) be two pairs of spaces in separating duality and let u be a linear mapping of F in F_1, which is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $. Then u is a strict morphism of F in F_1, if and only if, Im($ ^t u $) is a closed subspace in G for $ \sigma(G, F) $.

Let $ N = \operatorname{Im}(^t u) \subset G $; we know that $ N^0 = \operatorname{Ker}(u) $ in F (II, p. 47, formula (3)). Let $ p : F \to F/N^\circ $ be the canonical mapping so that u factorises as

$$
u : F \xrightarrow{p} F/N^\circ \xrightarrow{w} F_1,
$$

where w is injective. The spaces $ F/N^\circ $ and N are in separating duality and by formula (1) of II, p. 48, we have $ \langle w(\dot{y}), z_1 \rangle = \langle \dot{y}, ^t u(z_1) \rangle $ for all $ \dot{y} \in F/N^\circ $ and $ z_1 \in G_1 $. This relation shows that w is an isomorphism of $ F/N^\circ $, carrying the topology $ \sigma(F/N^\circ, N) $, on $ u(F) $ with the topology induced by $ \sigma(F_1, G_1) $. The conclusion results therefore from cor. 1 and the definition of a strict morphism.

#### Corollary 4 {#evt-ii-s6-prop-7-cor-4 .statement}

— Let (F, G), (F_1, G_1) be two pairs in separating duality, and let u be a linear mapping of F in F_1 that is continuous for $ \sigma(F, G) $ and $ \sigma(F_1, G_1) $. Then u is surjective, if and only if, $ ^t u $ is an isomorphism of $ G_1 $ (with topology $ \sigma(G_1, F_1) $) on $ ^t u(G_1) $ with the topology induced by $ \sigma(G, F) $.

For, to say that $ u(F) = F_1 $ is equivalent to saying that $ u(F) $ is closed and everywhere dense in $ F_1 $ for $ \sigma(F_1, G_1) $; cor. 4 follows then from cor. 3 applied to $ ^t u $ and of II, p. 47, cor. 2.

#### Remark {#evt-ii-s6-n5-rem-2 .statement}

— 1) Let $ (F_1, G_1), (F_2, G_2), (F_3, G_3) $ be three pairs of spaces in separating duality and consider a sequence of two linear mappings

$$
F_1 \xrightarrow{u} F_2 \xrightarrow{v} F_3
$$

that are continuous for the weak topologies corresponding respectively with $ G_1, G_2, G_3 $; we consider the sequence of transposed mappings

$$
G_3 \xrightarrow{^tv} G_2 \xrightarrow{^tu} G_1 .
$$

It is clear that $ ^t(v \circ u) = ^t u \circ ^t v $, therefore the relation $ v \circ u = 0 $ is equivalent to $ ^t u \circ ^t v = 0 $. The sequence (5) is exact if, and only if, the three following conditions are satisfied

a) $ ^t u \circ ^t v = 0 $;
b) $ \operatorname{Im}(^t v) $ is dense in $ \operatorname{Ker}(^t u) $;
c) $ ^t u $ is a strict morphism of $ G_2 $ in $ G_1 $.

This follows in effect from cor. 3 of II, p. 49 and formulae (3) and (4) of II, p. 47.

2) It must not be thought that when $ u $ is a strict morphism of $ F $ in $ F_1 $, then $ ^t u $ is necessarily a strict morphism of $ G_1 $ in $ G $; in other words $ u $ can be a strict morphism without $ u(F) $ being closed in $ F_1 $ for $ \sigma(F_1, G_1) $. This is shown by the example where $ F $ is a non-closed subspace of $ F_1 $ and $ G = G_1 / F^\circ $, $ u $ being the canonical injection. Similarly, the fact that the sequence (5) is exact does not necessarily imply that (6) is exact, however, if the sequence (5) is exact and if $ v $ is a strict morphism, then the sequence (6) is exact, by the remark 1 and by II, p. 49, cor. 3.

### 6. Products of weak topologies

#### Proposition 8 {#evt-ii-s6-prop-8 .statement}

— Let $ (F_i, G_i)_{i \in I} $ be a family of pairs of spaces in duality. Let $ F = \prod_{i \in I} F_i $ be the product space of the $ F_i $ and $ G = \bigoplus_{i \in I} G_i $ be the direct sum of the $ G_i $. If, for all $ x = (x_i) \in F $ and all $ y = (y_i) \in G $, we write $ \langle x, y \rangle = \sum_{i \in I} \langle x_i, y_i \rangle $ (a sum which has only finitely many non-zero terms) then the topology $ \sigma(F, G) $ (relative to the bilinear form $ (x, y) \mapsto \langle x, y \rangle $) is the product of the topologies $ \sigma(F_i, G_i) $.

For, given a topology $ \mathcal{T} $ on $ F $; in order that, for all $ y \in G $, the linear form $ x \mapsto \langle x, y \rangle $ should be continuous for $ \mathcal{T} $, it is necessary and sufficient, by the definition of $ \langle x, y \rangle $, that each of the mappings $ x \mapsto \langle \operatorname{pr}_i x, y_i \rangle $ should be continuous for $ \mathcal{T} $, where $ i $ is arbitrary in $ I $ and $ y_i $ in $ G_i $; but this means that each of the mappings $ \operatorname{pr}_i $ of $ F $ in $ F_i $ is continuous for $ \mathcal{T} $ and for $ \sigma(F_i, G_i) $ (I, p. 10, cor. 1); this completes the demonstration.

#### Remark {#evt-ii-s6-n6-rem-1 .statement}

— The duality between $ F $ and $ G $ is separating in $ F $ (resp. in $ G $) if and only if for all $ i \in I $, the duality between $ F_i $ and $ G_i $ is separating in $ F_i $ (resp. in $ G_i $). If the duality between $ F $ and $ G $ is separating in $ F $ (resp. $ G $), then, in $ F $ (resp. $ G $), the subspace orthogonal to one $ G_i $ (resp. $ F_i $), canonically identified with a subspace of $ G $ (resp. $ F $) is the subspace of the product of the $ F_\kappa $ where $ \kappa \neq i $ (resp. the direct sum of the $ G_\kappa $ such that $ \kappa \neq i $).

#### Corollary 1 {#evt-ii-s6-prop-8-cor-1 .statement}

— Let F and G be two vector spaces in separating duality. If the space F (with $ \sigma(F, G) $) is the direct topological sum of two subspaces M, N then the space G (with $ \sigma(G, F) $) is the direct topological sum of the subspaces $ M^\circ, N^\circ $ orthogonal respectively to M and N.

For let $ p : F \to M, q : F \to N $ be the projectors corresponding to the decomposition of F into the direct sum of M and N; in these conditions the mapping $ (p, q) : F \to M \times N $ is a topological isomorphism. If $ M_1 = G/M^\circ, N_1 = G/N^\circ $, then the topologies on M and N (induced by that of F) are identical with $ \sigma(M, M_1) $, $ \sigma(N, N_1) $ respectively (II, p. 48, prop. 7). The mapping $ ^t(p, q) : M_1 \times N_1 \to G $ is a topological isomorphism when we give $ M_1, N_1 $ and G the topologies $ \sigma(M_1, M) $, $ \sigma(N_1, N) $ and $ \sigma(G, F) $, by prop. 8. Under this mapping $ M_1 $ (resp. $ N_1 $) has as its image in G the subspace $ N^\circ $ (resp. $ M^\circ $), and the topology $ \sigma(M_1, M) $ (resp. $ \sigma(N_1, N) $) has as its image the topology induced on $ N^\circ $ (resp. $ M^\circ $) by $ \sigma(G, F) $, from which the corollary follows.

#### Corollary 2 {#evt-ii-s6-prop-8-cor-2 .statement}

— Let $ (e_i)_{i \in J} $ be a basis of the vector space F with dual $ F^* $, and let $ u : \mathbf{R}^{(I)} \to F $ be an (algebraic) isomorphism defined by this basis. Then the transposed mapping $ ^t u : F^* \to \mathbf{R}^I $ is a topological isomorphism when $ F^* $ carries the topology $ \sigma(F^*, F) $ and $ \mathbf{R}^I $ the product topology.

We know (A, II, § 2.6, prop. 10) that $ ^t u $ is a bijection, and that if for a $ x^* \in F^* $, we put $ \langle e_i, x^* \rangle = \xi_i^* $ for all $ i \in I $, then the image $ ^t u(x^*) $ is the vector $ (\xi_i^*) $ of $ \mathbf{R}^I $, so that, for all $ x = \sum_i \xi_i e_i $ in F, we have $ \langle x, x^* \rangle = \sum_i \xi_i \xi_i^* $. The corollary then follows from this formula and prop. 8.

### 7. Weakly complete spaces

#### Proposition 9 {#evt-ii-s6-prop-9 .statement}

— Let F, G be two vector spaces in separating duality. If $ \hat{F} $ is the completion of the space F for the topology $ \sigma(F, G) $ and if we consider the canonical injection $ j : F \to G^* $, where $ G^* $ has the topology $ \sigma(G^*, G) $, then the continuous extension $ \hat{j} : \hat{F} \to G^* $ of j is an isomorphism of topological vector spaces.

For, we see that $ G^* $, endowed with $ \sigma(G^*, G) $, is Hausdorff and complete (II, p. 51, cor. 2); if we identify F by j with a vector subspace of $ G^* $ then the topology induced on F by $ \sigma(G^*, G) $ is $ \sigma(F, G) $, and F is dense in $ G^* $ in the topology $ \sigma(G^*, G) $ (II, p. 43, cor. 4); from which the proposition follows.

Vector spaces that are complete for a weak topology are therefore the duals $ G^* $ of arbitrary vector spaces G endowed with $ \sigma(G^*, G) $; after II, p. 51, cor. 2, they are (topologically) isomorphic to products $ \mathbf{R}^I $ of real lines. To simplify the language, we shall call them products of lines (for an intrinsic characterisation of these spaces see II, p. 85, exerc. 13 and II, p. 81, exerc. 1).

We note that on $ G^* $, the $ \sigma(G^*, G) $ topology is minimal among the weak topologies that are Hausdorff; for, a weak topology that is coarser than $ \sigma(G^*, G) $ is necessarily of the form $ \sigma(G^*, H) $ where $ H \subset G $ (II, p. 43, cor. 3); but if $ H \neq G $, then there exists a linear form $ x^* \in G^* $ that is non null and is orthogonal to $ H $ (A, II, § 7.3, prop. 8), therefore $ \sigma(G^*, H) $ is not Hausdorff.

We deduce from this remark that, if $ F, G $ are two vector spaces, then a *linear bijection* $ u : G^* \to F^* $, that is continuous for the topologies $ \sigma(G^*, G) $ and $ \sigma(F^*, F) $, is necessarily *bicontinuous*.

#### Proposition 10 {#evt-ii-s6-prop-10 .statement}

*Let $ G $ be a real vector space and $ F = G^* $ its dual with the topology $ \sigma(G^*, G) $.*

(i) *The mapping $ V \mapsto V^\circ $ is a bijection of the set of vector subspaces of $ G $ on the set of closed vector subspaces of $ F $.*

(ii) *Every closed vector subspace of $ F $ is a product of lines and has a topological complement.*

By the bipolar theorem (II, p. 45, cor. 2) $ V \mapsto V^\circ $ is a bijection of the set of vector subspaces $ V $ of $ G $, *closed* for $ \sigma(G, G^*) $ on the set of closed vector subspaces of $ F $. But, by definition, *every* linear form on $ G $ is continuous for $ \sigma(G, G^*) $, therefore every vector subspace in $ G $ is closed, being defined by a system of equations $ \langle y, y_\lambda^* \rangle = 0 $ (where $ y_\lambda^* \in G^* $); this proves (i).

Now let $ W $ be a closed subspace of $ F $; we have then $ W = V^\circ $ with $ V = W^\circ $ in $ G $. Let $ V' $ be a complement of $ V $ in $ G $. We know that $ F = G^* $ can be canonically identified with $ V^* \oplus V'^* $, and $ V'^* $ identified with $ V^\circ = W $ (A, II, § 2.6, cor. to prop. 10); further (II, p. 50, prop. 8) the topology $ \sigma(G^*, G) $ can be identified with the product of the topologies $ \sigma(V^*, V) $ and $ \sigma(V'^*, V') $; this proves assertion (ii).

Though, for the topology $ \sigma(G, G^*) $, every vector subspace of $ G $ is closed, we note that if $ G $ is of infinite dimension then the topology $ \sigma(G, G^*) $ is not the finest locally convex topology on $ G $, every neighbourhood of 0 for $ \sigma(G, G^*) $ containing a vector subspace of infinite dimension : it is however the finest of the *weak* topologies on $ G $ (II, p. 43, cor. 3).

### 8. Complete convex cones in weak spaces

#### Lemma 1 {#evt-ii-s6-lem-1 .statement}

*Let $ E $ be a Hausdorff weak space and $ C $ a proper cone with vertex 0 in $ E $, that is complete for the uniform structure induced by that of $ E $. Every continuous linear form in $ E $ is then the difference between two continuous linear forms in $ E $ that are positive in $ C $.*

Let $ E' $ be the dual of $ E $ and $ F $ be the algebraic dual of $ E' $, with the topology $ \sigma(F, E') $. Let $ H = C^\circ - C^\circ $ be the vector subspace of $ E' $ formed by the differences of linear forms that are continuous in $ E $ and positive in $ C $ (II, p. 44, prop. 4). It is sufficient to show that the orthogonal to $ H $ in $ F $ is $ \{0\} $ (II, p. 41, *Example* 1). Then let $ a \in F $ be orthogonal to $ H $; as $ a $ is orthogonal to $ C^\circ $, it must belong to the bipolar of $ C $ in $ F $. But $ E $ is identifiable as a subspace of $ F $, and since $ C $ is complete, thus closed in $ F $, we have $ a \in C $ (II, p. 44, th. 1). Similarly $ a $ is orthogonal to $ -C^\circ $ and therefore $ a \in -C $. As $ C $ is proper, we have $ a = 0 $.

#### Proposition 11 {#evt-ii-s6-prop-11 .statement}

*Let $ E $ be a Hausdorff weak space, and $ C $ be a proper convex cone with vertex 0 in $ E $ and which is complete in the uniform structure induced by that of $ E $.*

Then there exists a set I and a continuous linear mapping u of E in the product space $ \mathbf{R}^I $ with the following properties:

a) u is an isomorphism of C on $ u(C) $ for the uniform structures induced respectively by those of E and of $ \mathbf{R}^I $.

b) We have $ u(C) \subset \mathbf{R}_+^I $.

Further, if the uniform structure induced on C by that of E is metrisable, then we can take $ I = \mathbf{N} $.

Let $ (f_i)_{i \in I} $ be a family of continuous linear forms in E such that the finite sums of pseudometrics of the form $ (x, y) \mapsto |f_i(x - y)| $ on $ C \times C $ define the uniform structure of C. (If the structure is metrisable we can take $ I = \mathbf{N} $.) By lemma 1 we can suppose further that each of the $ f_i $ is positive in C. Let u be the linear mapping $ x \mapsto (f_i(x))_{i \in I} $ of E in $ \mathbf{R}^I $. It is clear that u is continuous and that $ u(C) \subset \mathbf{R}_+^I $. The restriction $ u|C $ is a uniformly continuous mapping that is surjective from C on $ u(C) $. Further if $ x, y $ in C are such that $ f_i(x) = f_i(y) $ for all $ i \in I $, then $ x = y $ since the uniform structure of C is Hausdorff; therefore $ u|C $ is bijective. Finally, if W is an entourage of the uniform structure of C, then there exists a finite set J of I and a number $ \varepsilon > 0 $ such that the relations $ |f_i(x) - f_i(y)| \leq \varepsilon $ for $ i \in J $ imply $ (x, y) \in W $; therefore $ u|C $ is an isomorphism of C on $ u(C) $ for the uniform structures being considered.

#### Corollary 1 {#evt-ii-s6-prop-11-cor-1 .statement}

— Let E be a Hausdorff weak space and C a proper convex cone of vertex 0 in E that is complete for the uniform structure induced by that of E. Then the mapping $ (x, y) \mapsto x + y $ of $ C \times C $ in C is proper.

Because of prop. 11, we can suppose that $ E = \mathbf{R}^I $ and that $ C = \mathbf{R}_+^I $ (GT, I, § 10.1, cor. 1 and 4). But then the mapping $ (x, y) \mapsto x + y $ of $ C \times C $ in C is written as $ ((\xi_i), (\eta_i)) \mapsto (\xi_i + \eta_i) $, and we can restrict ourselves to proving that the continuous mapping $ f : (\xi, \eta) \mapsto \xi + \eta $ of $ \mathbf{R}_+ \times \mathbf{R}_+ $ in $ \mathbf{R}_+ $, is proper (GT, I, § 10.1, cor.3), Now, for all $ \zeta \in \mathbf{R}_+ $, we see that $ f(\zeta) $ is the set of pairs $ (\xi, \zeta - \xi) $ such that $ 0 \leq \xi \leq \zeta $, therefore the inverse image by f of the interval $ [0, \zeta] $ is the set of the $ (\xi, \eta) \in \mathbf{R}_+ \times \mathbf{R}_+ $ such that $ \xi + \eta \leq \zeta $, which is compact. The conclusion follows applying (GT, I, § 10.3, prop. 7).

#### Corollary 2 {#evt-ii-s6-prop-11-cor-2 .statement}

— Let E be a Hausdorff weak space, and C a proper convex cone with vertex 0 in E, that is complete for the uniform structure induced by that of E.

(i) For every point a of E, the intersection $ C \cap (a - C) $ is compact.

(ii) Let A, B be two closed sets in C. Then $ A + B $ is a closed set in C.

(i) The set of the $ (x, y) \in C \times C $ such that $ x + y = a $ is compact from cor. 1 and from GT, I, § 10.2, th. 1, b). Now this set is also the set of the $ (x, a - x) $ for $ x \in C \cap (a - C) $, which proves (i).

(ii) If A and B are closed in C, then $ A \times B $ is closed in $ C \times C $, therefore $ A + B $ is closed in C after cor. 1 and GT, I, § 10.1, prop. 1.

### Exercises {#evt-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
