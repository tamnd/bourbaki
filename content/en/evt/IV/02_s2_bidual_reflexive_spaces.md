---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 2
section_title: Bidual. Reflexive spaces
lang: en
source: evt-i-v
book_pages: TVS IV.14-TVS IV.21, TVS IV.52-TVS IV.57
pdf_pages: 0196-0203, 0234-0239
extraction: ocr
subsections:
    - "no": 1
      title: Bidual
      page: 14
      pdf_page: 196
    - "no": 2
      title: Semi-reflexive spaces
      page: 15
      pdf_page: 197
    - "no": 3
      title: Reflexive spaces
      page: 16
      pdf_page: 198
    - "no": 4
      title: The case of normed spaces
      page: 17
      pdf_page: 199
    - "no": 5
      title: Montel spaces
      page: 18
      pdf_page: 200
statements: 30
exercises: 24
content_sha256: c8f008de2daf8653ce90dda0cbafdb04b9e1842cb6daff4312ae7ca854ca1ef6
---

## § 2. BIDUAL. REFLEXIVE SPACES

### 1. Bidual

#### Definition 1 {#evt-iv-s2-def-1 .statement}

— *Let $ E $ be a locally convex space and $ E'_b $ its strong dual. The dual of the locally convex space $ E'_b $ is called the bidual of $ E $ and is denoted by $ E'' $.*

For every $ x \in E $, let $ \tilde{x} $ be the linear form $ x' \mapsto \langle x, x' \rangle $ on $ E' $; it is continuous for the weak topology $ \sigma(E', E) $, hence *a fortiori*, for the strong topology on $ E' $; therefore $ \tilde{x} \in E'' $ for all $ x \in E $. The map $ c_E : x \mapsto \tilde{x} $ from $ E $ into $ E'' $ is a linear mapping, said to be *canonical*.

#### Proposition 1 {#evt-iv-s2-prop-1 .statement}

— *The kernel of $ c_E : E \to E'' $ is the closure of 0 in $ E $. If $ E $ is Hausdorff, $ c_E $ is injective.*

By construction, the kernel of $ c_E $ is the intersection of the kernels of the continuous linear forms on $ E $, *i.e.* the closure of $ \{0\} $ in $ E $ (II, p. 24, cor. 1).

When $ E $ is Hausdorff, we identify $ E $ with a subspace of $ E'' $, by means of the mapping $ c_E $.

BIDUAL. REFLEXIVE SPACES

TVS IV.15

The strong topology on $ E'' $ is the $ \mathcal{S} $-topology, where $ \mathcal{S} $ is the family of all strongly bounded subsets of $ E' $. Since every equicontinuous subset of $ E' $ is strongly bounded (III, p. 22, prop. 9), the initial topology on $ E $ is coarser than the topology obtained by taking the inverse image under $ c_E $ of the strong topology on $ E'' $; it can be strictly coarser (IV, p. 52, exerc. 1). However:

#### Proposition 2 {#evt-iv-s2-prop-2 .statement}

— Suppose that the space $ E $ is bornological or barrelled. The initial topological on $ E $ is the inverse image under $ c_E $ of the strong topology on $ E'' $.

For, every subset of $ E' $ which is strongly bounded is equicontinuous (III, p. 22, prop. 10 and III, p. 24).

#### Proposition 3 {#evt-iv-s2-prop-3 .statement}

— Let $ E $ be a locally convex Hausdorff space. In order that the strong dual $ E'_b $ of $ E $ be barrelled, it is necessary and sufficient that every subset of $ E'' $ which is bounded for $ \sigma(E'', E') $, is contained in the closure, for $ \sigma(E'', E') $, of a bounded subset of $ E $.

The equicontinuous subsets of $ E'' $ are the subsets contained in the bipolar (for the duality between $ E'' $ and $ E' $) of a bounded subset of the subspace $ E $ of $ E'' $. It is now enough to apply the theorem of bipolars (II, p. 45, cor. 3) and the definition of a barrelled space (III, p. 24).

#### Remark {#evt-iv-s2-n1-rem-1 .statement}

Let $ E $ be a locally convex Hausdorff space, $ E' $ its dual and $ E'' $ its bidual. We have $ E \subset E'' \subset E'^* $, where $ E'^* $ is the algebraic dual of $ E' $. If $ B $ is a bounded subset of $ E $, its closure $ \overline{B} $ in $ E'^* $ endowed with $ \sigma(E'^*, E') $ is contained in $ E'' $: for, the polar $ U = B^\circ $ of $ B $ in $ E' $ is a neighbourhood of 0 in $ E'_b $, and we have $ \overline{B} \subset U^\circ \subset E'' $.

### 2. Semi-reflexive spaces

#### Definition 2 {#evt-iv-s2-def-2 .statement}

— Let $ E $ be a locally convex space. We say that $ E $ is semi-reflexive if the canonical mapping $ c_E $ from $ E $ into $ E'' $ is bijective.

This implies that $ E $ is Hausdorff, and that every linear form on $ E' $, which is continuous for the strong topology $ \beta(E', E) $, is of the form $ x' \mapsto \langle x, x' \rangle $ with $ x \in E $, i.e. continuous for the weak topology $ \sigma(E', E) $.

#### Theorem 1 {#evt-iv-s2-thm-1 .statement}

— A locally convex Hausdorff space is semi-reflexive if and only if every bounded subset of $ E $ is relatively compact for the weakened topology $ \sigma(E, E') $. If $ E $ is semi-reflexive, the strong dual $ E'_b $ of $ E $ is barrelled.

The second assertion follows from prop. 3 (IV, p. 15), and the identity between bounded subsets for the initial topology and for the weakened topology of $ E $ (III, p. 27, cor. 3).

To say that $ E $ is semi-reflexive means that the topology on $ E'_b $ is compatible with the duality between $ E $ and $ E' $, in other words, by Mackey's theorem (IV, p. 2, th. 1) that the topology on $ E'_b $ is coarser than $ \tau(E', E) $ (and in fact is identical with it); by definition (IV, p. 2), this means that every closed, convex and bounded subset of $ E $ is compact for $ \sigma(E, E') $, and this is equivalent to saying that every bounded subset of E is relatively compact for $ \sigma(E, E') $, because the closed convex envelope of a bounded subset of E is bounded (III, p. 3, prop. 1).

#### Corollary {#evt-iv-s2-n2-cor-1 .statement}

— *Let E be a locally convex semi-reflexive space. Every closed vector subspace M of E is semi-reflexive; moreover, the strong topology on $ E'/M^\circ $ (considered as the dual of M) is the quotient of the strong topology on E'.

Let B be a bounded subset of M. Since B is bounded in E, and the weakened topology $ \sigma(M, M') $ on M is induced by $ \sigma(E, E') $ (IV, p. 10, prop. 11), the closure of B in M endowed with $ \sigma(M, M') $ is compact. Hence, by th. 1, M is semi-reflexive. The last assertion of the corollary follows from prop. 10 of IV, p. 9, applied to the set $ \mathcal{S} $ of all closed, convex and bounded subsets of E.

#### Remark 1 {#evt-iv-s2-n2-rem-1 .statement}

Suppose E is semi-reflexive. Every subset of E which is convex, closed and bounded for the initial topology is compact for the topology $ \sigma(E, E') $ (IV, p. 1, prop. 1). *On the other hand, the unit sphere (with the equation $ \|x\| = 1 $) of an infinite dimensional hilbertian space E is closed and bounded for the initial topology, but is not closed for the weakened topology, even if E is semi-reflexive. \*
2) By remark 3 of IV, p. 5, we can reformulate th. 1 as follows : *the Hausdorff space E is semi-reflexive if and only if it is quasi-complete for its weakened topology.* If it is semi-reflexive, then it is *quasi-complete for its initial topology* (IV, p. 5, Remark 2).
3) Under the hypotheses of the above corollary, the space E/M is not necessarily semi-reflexive (IV, p. 63, exerc. 10).

### 3. Reflexive spaces

#### Definition 3 {#evt-iv-s2-def-3 .statement}

— *A locally convex space E is said to be reflexive if the canonical mapping $ c_E $ from E into $ E'' $ is a topological vector space isomorphism from E onto the strong dual of $ E'_b $.*

In particular, a reflexive space is semi-reflexive, hence Hausdorff.

#### Proposition 4 {#evt-iv-s2-prop-4 .statement}

— *The strong dual of a reflexive space is reflexive.*

This follows immediately from def. 3.

#### Theorem 2 {#evt-iv-s2-thm-2 .statement}

— *In order that a locally convex Hausdorff space E be reflexive, it is necessary and sufficient that it is barrelled and that every bounded subset of E is relatively compact for the weakened topology $ \sigma(E, E') $.*

By th. 1 (IV, p. 15), this is the same as saying that E *is reflexive if and only if it is semi-reflexive and barrelled*.

If E is reflexive, $ E'_b $ is reflexive (prop. 4) and consequently E is barrelled (IV, p. 15, th. 1). Conversely, if E is semi-reflexive and barrelled, $ c_E $ is a bijection and is bicontinuous by IV, p. 15, prop. 2, hence E is reflexive.

#### Remark 1 {#evt-iv-s2-n3-rem-1 .statement}

Let E be an infinite dimensional real hilbertian space. Let F denote the space E endowed with the weakened topology. The spaces E and F have the same dual E', and E is a reflexive Banach space (V, p. 17). Consequently, F is *semi-reflexive*.

However, the strong topology and the weakened topology on E are distinct, hence F *is not reflexive*.

#### Remark 2 {#evt-iv-s2-n3-rem-2 .statement}

Let E be a reflexive space and M a closed vector subspace of E. It may happen that neither M nor E/M are reflexive spaces (IV, p. 63, exerc. 10). \* For the case of normed spaces, see prop. 7 of IV, p. 17. \*

### 4. The case of normed spaces

Let E be a normed space. The strong topology on the dual E' of E is defined by the norm

(1)
$$
\|x'\| = \sup_{x \in E, \|x\| \leq 1} |\langle x, x' \rangle|,
$$
and the strong dual of E is a Banach space (III, p. 24, cor. 2). Then the bidual E'' of E is also a Banach space, for the norm defined by

(2)
$$
\|x''\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x', x'' \rangle|.
$$

By prop. 8, (i) of IV, p. 7, the canonical linear mapping $ c_E : E \to E'' $ is an isometry. Henceforth, *we shall identify E with a normed subspace of its bidual E''*.

#### Proposition 5 {#evt-iv-s2-prop-5 .statement}

— *Let E be a normed space, E' its dual and E'' its bidual. The (closed) unit ball in E'' is the closure of the unit ball B in E for the weak topology $ \sigma(E'', E') $.*

By formulas (1) and (2), the unit ball in E'' is the bipolar $ B^{\circ \circ} $ of B. Prop. 5 then follows from the theorem of bipolars (II, p. 45, cor. 3).

#### Remark {#evt-iv-s2-n4-rem-1 .statement}

— A Banach space E is closed in its bidual E'' for the strong topology, but is dense for the weak topology (prop. 5).

In order that a normed space be *reflexive*, it is necessary and sufficient that it is *semi-reflexive*; for, the initial topology of E is always induced by the strong topology of E''. Th. 1 (IV, p. 15) then implies the following result :

#### Proposition 6 {#evt-iv-s2-prop-6 .statement}

— *In order that a normed space E be reflexive, it is necessary and sufficient that the unit ball in E be compact for the weakened topology $ \sigma(E, E') $.*

We observe that a reflexive normed space is complete hence a Banach space, and that its dual is a reflexive Banach space by prop. 4 of IV, p. 16.

#### Proposition 7 {#evt-iv-s2-prop-7 .statement}

— *Let E be a reflexive Banach space and M a closed vector subspace of E. Then M and E/M are reflexive Banach spaces.*

Let E' be the dual of E and $ M^\circ $ the orthogonal of M in E'. As a normed space, we can identify the space $ E'/M^\circ $ with the dual $ M' $ of M (IV, p. 9, prop. 10). Since M is semi-reflexive (IV, p. 16, corollary), it is reflexive, hence so is $ E'/M^\circ $; similarly $ M^\circ $ is reflexive, as also its dual $ E/M^{\circ \circ} = E/M $.

#### Example {#evt-iv-s2-n4-exa-1 .statement}

— 1) Let $ \ell^\infty(\mathbf{N}) $ denote the Banach space of bounded sequences $ x = (x_n)_{n \in \mathbf{N}} $ of scalars, with the norm

(3) $$
\| \mathbf{x} \| = \sup_{n \in \mathbf{N}} |x_n| \quad (\text{I, p. 4}) .
$$

Let $ c_0(\mathbf{N}) $ be the closed vector subspace of $ \ell^\infty(\mathbf{N}) $ consisting of sequences tending to 0. Finally, let $ \ell^1(\mathbf{N}) $ be the vector space of summable sequences, endowed with the norm

(4) $$
\| \mathbf{x} \|_1 = \sum_{n \in \mathbf{N}} |x_n| .
$$

We can show (IV, p. 47, exerc. 1) that the dual of $ c_0(\mathbf{N}) $ can be identified with $ \ell^1(\mathbf{N}) $ in such a way that we have

(5) $$
\langle \mathbf{x}, \mathbf{x}' \rangle = \sum_{n \in \mathbf{N}} x_n x'_n
$$

for all $ \mathbf{x} \in c_0(\mathbf{N}) $ and $ \mathbf{x}' \in \ell^1(\mathbf{N}) $. Similarly the dual of $ \ell^1(\mathbf{N}) $ can be identified with $ \ell^\infty(\mathbf{N}) $ in such a way that we have the relation (5) for all $ \mathbf{x} \in \ell^1(\mathbf{N}) $ and all $ \mathbf{x}' \in \ell^\infty(\mathbf{N}) $. Hence $ \ell^\infty(\mathbf{N}) $ is the bidual of $ c_0(\mathbf{N}) $, and this latter space is not reflexive.

* 2) Every hilbertian space is a reflexive Banach space (V, p. 17).
* 3) Let X be a Hausdorff topological space and $ \mu $ a complex measure on X. For every real number $ p > 1 $, the Banach space $ L^p(X, \mu) $ is reflexive, and its dual can be identified with $ L^q(X, \mu) $ with $ p^{-1} + q^{-1} = 1 $ (INT, V, 2nd edition, § 5, No. 8 and IX, § 1, No. 10).

### 5. Montel spaces

#### Definition 4 {#evt-iv-s2-def-4 .statement}

*A locally convex Hausdorff and barrelled space in which every bounded subset is relatively compact is called a Montel space.*

#### Example 1 {#evt-iv-s2-n5-exa-1 .statement}

Every finite dimensional Hausdorff space is a Montel space. A normed space which is a Montel space is locally compact, hence is finite dimensional (I, p. 15, th. 3).

#### Example 2 {#evt-iv-s2-n5-exa-2 .statement}

With the notations and hypothesis of prop. 7 of III, p. 6, the space E, being the inductive limit of Banach spaces, is barrelled (III, p. 25); moreover, every bounded subset of E is relatively compact (III, p. 6, prop. 7). In other words, E is a Montel space. In particular, Gevrey spaces (III, p. 10) are Montel spaces. * This is true for the space $ \mathcal{H}(K) $ consisting of germs of functions analytic in a neighbourhood of a compact subset K of $ \mathbf{C}^n $ (III, p. 10).*

#### Example 3 {#evt-iv-s2-n5-exa-3 .statement}

Every strict inductive limit E of a sequence $ (E_n) $ of Montel spaces (II, p. 33) such that $ E_n $ is closed in $ E_{n+1} $ for all n, is a Montel space; in fact, E is Hausdorff (II, p. 32, prop. 9 (i)), barrelled (III, p. 25, cor. 3) and every bounded subset of E is contained in one of the $ E_n $ (III, p. 5, prop. 6) hence is relatively compact in $ E_n $, and consequently also in E.

#### Example 4 {#evt-iv-s2-n5-exa-4 .statement}

Let U be an open set in $ \mathbf{R}^n $ and let $ \mathcal{C}^\infty(U) $ be the Fréchet space of infinitely differentiable functions on U (III, p. 9). We shall prove that this is a Montel space. Since $ \mathcal{C}^\infty(U) $ is a Fréchet space, it is barrelled (III, p. 25, corollary). Let B be a bounded subset of $ \mathcal{C}^\infty(U) $ and let K be a compact subset of U. For every $ \alpha \in \mathbf{N}^n $ let $ H_{\alpha, K} $ be the set of restrictions to K of the functions $ \partial^\alpha f $, as $ f $ runs through B. Let $ \alpha \in \mathbf{N}^n $; for every $ \beta \in \mathbf{N}^n $ such that $ |\beta| = |\alpha| + 1 $, the set $ H_{\alpha, K} $ is bounded in $ \mathcal{C}(K) $ since B is bounded in $ \mathcal{C}^\infty(U) $; by VAR, R., No. 2.2.3, the set $ H_{\alpha, K} $ is equicontinuous, hence (GT, X, § 2, No. 5) relatively compact in $ \mathcal{C}(K) $. But the topology of $ \mathcal{C}^\infty(U) $ is the coarsest among the topologies for which all the maps $ f \mapsto \partial^\alpha f|K $ from $ \mathcal{C}^\infty(U) $ into $ \mathcal{C}(K) $ are continuous, therefore B is relatively compact in $ \mathcal{C}^\infty(U) $ (GT, I, § 4, No. 1, prop. 3 and § 9, No. 5, corollary).

Similarly, *the space $ \mathcal{C}_0^\infty(U) $ of all infinitely differentiable functions with compact support in U* (III, p. 9) *is a Montel space*. For, $ \mathcal{C}_0^\infty(U) $ is the strict inductive limit of a sequence $ \mathcal{C}_{H_n}^\infty(U) $ of Fréchet spaces (III, p. 9), and it is enough to see that each of the spaces $ \mathcal{C}_{H_n}^\infty(U) $ is a Montel space (*Example 3*). But a bounded and closed subset of $ \mathcal{C}_0^\infty(U) $ is closed and bounded in $ \mathcal{C}^\infty(U) $, hence compact in $ \mathcal{C}^\infty(U) $, and consequently in $ \mathcal{C}_{H_n}^\infty(U) $. *

#### Proposition 8 {#evt-iv-s2-prop-8 .statement}

*Let E be a Montel space and $ \mathfrak{T} $ a filter on E, which converges to a point $ x_0 $ in E for the weakened topology. If $ \mathfrak{T} $ is a countable base, or contains a bounded set, then $ \mathfrak{T} $, converges to $ x_0 $ for the initial topology also.*

Assume first that there exists a bounded set $ \overline{B} $ in $ \mathfrak{T} $. The closure $ \overline{B} $ of B for the initial topology of E is bounded; in addition, $ \overline{B} $ is compact because E is a Montel space. The topology on $ \overline{B} $ induced by $ \sigma(E, E') $ is Hausdorff and coarser than the topology induced by the initial topology; they therefore coincide (GT, I, § 9, No. 4). This prove the proposition for this case.

Next assume that $ \mathfrak{T} $ has a countable base. It is enough (GT, I, § 6, No. 8, prop. 11) to consider the case of a sequence $ (x_n)_{n \geq 1} $ tending to $ x_0 $ for $ \sigma(E, E') $. Let B be the set of all $ x_n $ for $ n \geq 0 $. This set is bounded for $ \sigma(E, E') $, hence also for the initial topology (III, p. 27, cor. 3). Thus we have reduced to the first case of the proof.

*Every Montel space is reflexive*: this follows from def. 4 and from th. 2 of IV, p. 16. Further:

#### Proposition 9 {#evt-iv-s2-prop-9 .statement}

*The strong dual of a Montel space is a Montel space.*

Let E be a Montel space and $ E'_b $ its strong dual. Since E is reflexive, $ E'_b $ is barrelled (IV, p. 15, th. 1). Since every bounded subset of E is relatively compact the strong topology on $ E' $ coincides with the topology of compact convergence. Let B be a bounded subset of $ E'_b $; it is bounded for the weak topology $ \sigma(E', E) $, hence is equicontinuous because E is barrelled. Then Ascoli’s theorem (GT, X, § 2, No. 4, cor. and § 2, No. 5, cor. 1) implies that the closure of B for $ \sigma(E', E) $ is compact for the topology of compact convergence; therefore B is relatively compact in $ E'_b $.

#### Proposition 10 {#evt-iv-s2-prop-10 .statement}

*Every metrizable Montel space satisfies the first axiom of countability.*

Let E be a metrizable Montel space. We know (II, p. 5) that E can be identified with a subspace of the product $ F = \prod_{n \in \mathbf{N}} F_n $ of a sequence of normed spaces, and we can even assume that we have $ \mathrm{pr}_n(E) = F_n $ for all $ n \in \mathbf{N} $. If each of the metrizable spaces $ F_n $ satisfies the first axiom of countability, then so does F (GT, IX, § 2, No. 8), hence also E.

We argue by *reductio ad absurdum*. Assume for example that $ F_0 $ does not satisfy the first axiom of countability. Let $ B_0 $ be the unit ball (closed) in $ F_0 $; this is a metric space which does not satisfy the first axiom of countability. We shall use the following lemma :

#### Lemma 1 {#evt-iv-s2-lem-1 .statement}

*Suppose the metric space X does not satisfy the first axiom of countability. Then there exists a real number $ \varepsilon > 0 $ and an uncountable subset A in X such that $ d(x, y) \geq \varepsilon $ for all distinct $ x, y $ in A.*

For every integer $ n \geq 1 $, let $ \mathfrak{F}_n $ be the set (ordered by inclusion) of subsets D of X such that $ d(x, y) \geq \frac{1}{n} $ for distinct $ x, y $ in D. The set $ \mathfrak{F}_n $ is of finite character, hence possesses a maximal element $ D_n $ (S, III, § 4, No. 5). Then for all $ y \in X $, there exists a point $ x $ in $ D_n $ such that $ d(x, y) < \frac{1}{n} $, by virtue of the maximal character of $ D_n $.

Put $ D = \bigcup_n D_n $; the set D is then dense in X, and since X does not satisfy the first axiom of countability, D is not countable, and so one of the $ D_n $ is not countable.

Q.E.D.

By lemma 1, applied to $ B_0 $, there exists an uncountable subset $ A_0 $ of $ F_0 $ and a number $ \varepsilon > 0 $ such that $ \|x\| \leq 1 $ and $ \|x - y\| \geq \varepsilon $ for distinct $ x, y $ in $ A_0 $. We have $ \mathrm{pr}_0(E) = F_0 $ and hence there exists a subset A in E such that $ \mathrm{pr}_0 $ induces a bijection from A onto $ A_0 $.

#### Lemma 2 {#evt-iv-s2-lem-2 .statement}

*There exists a sequence $ (x_m)_{m \geq 0} $ consisting of distinct elements of A, which is bounded in E.*

We shall construct a sequence $ (x_m)_{m \geq 0} $ of points of A by induction; and a decreasing sequence $ (C_m)_{m \geq 0} $ of subsets of A satisfying the following conditions :
a) None of the sets $ C_m $ is countable.
b) For every $ n \geq 0 $, the set $ \mathrm{pr}_k(C_m) $ is bounded in $ F_k $ for $ 0 \leq k \leq m $.
c) For every $ m \geq 0 $, we have $ x_m \in C_m - C_{m+1} $.

We put $ C_0 = A $. Suppose the sets $ C_m $ for $ 0 \leq m \leq n $ have been defined, so as to satisfy a) and b) for $ 0 \leq m \leq n $, and also the points $ x_m $ in $ C_m - C_{m+1} $ for $ 0 \leq m < n $. For every integer $ r \geq 1 $, let $ C_{n,r} $ be the set of all $ x \in C_n $ such that

$$
r - 1 \leq \| \mathrm{pr}_{n+1}(x) \| < r .
$$

Since $ C_n $ is not countable, there exists an integer $ r \geq 1 $ such that $ C_{n,r} $ is not countable. We choose a point $ x_n $ in $ C_{n,r} $ and put $ C_{n+1} = C_{n,r} - \{ x_n \} $. Evidently $ C_{n+1} \subset C_n $ and $ x_n \in C_n - C_{n+1} $, the set $ C_{n+1} $ is not countable and $ \mathrm{pr}_k(C_{n+1}) $ is bounded in $ F_n $ for $ 0 \leq k \leq n + 1 $.

We have $ x_m \in C_m $, and so $ x_m \in C_n $ where $ m \geq n $. The projection of the sequence $ (x_m)_{m \geq 0} $ on $ F_n $ is therefore bounded for all $ n \geq 0 $; in other words, the sequence $ (x_m)_{m \geq 0} $ is bounded in E, and this establishes lemma 2.

Q.E.D.

With the notations of lemma 2, the bounded sequence $ (x_m)_{m \geq 0} $ has a limit point $ y $ in E. Therefore the sequence $ (\mathrm{pr}_0(x_m))_{m \geq 0} $ has a limit point $ \mathrm{pr}_0(y) $ in $ F_0 $, but this contradicts the construction of $ A_0 $.

#### Corollary {#evt-iv-s2-n5-cor-1 .statement}

— Let E be a metrizable Montel space. Then there exists a countable dense set in the strong dual of E.

On the dual E' of E, the strong topology is identical with that of compact convergence, since E is a Montel space. It is now enough to apply cor. 1 of prop. 6 of III, p. 18.

We can show that the strong dual of a metrizable Montel space E is not metrizable if E is infinite dimensional (IV, p. 57, exerc. 1).

### Exercises {#evt-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
