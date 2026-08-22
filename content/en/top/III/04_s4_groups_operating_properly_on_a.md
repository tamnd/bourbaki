---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 4
section_title: Groups operating properly on a topological space; compact ness in topological groups and spaces with operators
lang: en
source: top-i-iv
pdf_pages: 0256-0267, 0314-0320
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS OPERATING PROPERLY ON A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 256
    - "no": 2
      title: PROPERTIES OF GROUPS ACTING PROPERLY
      page: 0
      pdf_page: 259
    - "no": 3
      title: GROUPS OPERATING FREELY ON A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 260
    - "no": 4
      title: LOCALLY COMPACT GROUPS OPERATING PROPERLY
      page: 0
      pdf_page: 261
    - "no": 5
      title: GROUPS OPERATING CONTINUOUSLY ON A LOCALLY COMPACT SPACE
      page: 0
      pdf_page: 263
    - "no": 6
      title: LOCALLY COMPACT HOMOGENEOUS SPACES
      page: 0
      pdf_page: 265
statements: 33
exercises: 8
content_sha256: 98bbe11fdf6749e206e1e4299f5988df931a0fc935bdd492e0606a77dcab9459
---

## 4. GROUPS OPERATING PROPERLY ON A TOPOLOGICAL SPACE; COMPACTNESS IN TOPOLOGICAL GROUPS AND SPACES WITH OPERATORS

### 1. GROUPS OPERATING PROPERLY ON A TOPOLOGICAL SPACE

#### Definition 1 {#top-iii-s4-def-1 .statement}

Let $ G $ be a topological group operating continuously on a topological space $ X $. $ G $ is said to operate properly on $ X $ if the mapping

$$
\theta : (s, x) \to (x, s.x) \text{ of } G \times X \text{ into } X \times X
$$

is proper (Chapter I, § 10, no. 1, Definition 1).

Let $ \Gamma \subset G \times X \times X $ be the graph of the mapping $ \rho : (s, x) \to s.x $. Since $ \rho $ is continuous, the mapping $ \sigma : (s, x) \to (s, x, s.x) $ is a homeomorphism of $ G \times X $ onto $ \Gamma $, and the composite mapping

$$
G \times X \xrightarrow{\sigma} \Gamma \xrightarrow{\mathrm{pr}_{23}} X \times X
$$

is just $ \theta $. Definition 1 is therefore equivalent to saying that the restriction of $ \mathrm{pr}_{23} $ to $ \Gamma $ is a proper mapping of $ \Gamma $ into $ X \times X $.

Theorem 1 of Chapter I, § 10, no. 2 shows that G operates properly on X if and only if the following condition is satisfied:
For each set A filtered by an ultrafilter $ \mathfrak{F} $, and each mapping
$$
\alpha \to (s_\alpha, x_\alpha)
$$
of A into $ G \times X $, if the mapping $ \alpha \to (s_\alpha \cdot x_\alpha, x_\alpha) $ has a limit $(b, a)$ with respect to $ \mathfrak{F} $, then $ \alpha \to s_\alpha $ has a limit $ t \in G $ with respect to $ \mathfrak{F} $, such that $ t.a = b $.

#### Example 1 {#top-iii-s4-n1-exa-1 .statement}

Let H be a closed subgroup of a topological group G. If G operates properly on X, then so does H, since $ H \times X $ is closed in $ G \times X $ (Chapter I, § 10, no. 1, Proposition 5, Corollary 1). If for example we take $ X = G $, with G operating on itself by left translations, then the mapping $ G \times X \to X \times X $ is a homeomorphism, hence proper; thus H operates properly on G by left translations.

#### Example 2 {#top-iii-s4-n1-exa-2 .statement}

If G operates properly on X, then it operates properly on every subspace $ X' $ of X which is a union of orbits of points of X (in other words, $ X' $ is saturated with respect to the equivalence relation defined by G). For the inverse image of $ X' \times X' $ in $ G \times X $ is $ G \times X' $, and we can apply Proposition 3 of Chapter I, § 10, no. 1.

#### Proposition 1 {#top-iii-s4-prop-1 .statement}

Let G be a topological group operating continuously on a topological space X, and let K be a quasi-compact subset of G. Then the mapping $ \rho : (s, x) \to s.x $ of $ K \times X $ into X is proper.

$ \rho $ factorizes into $ K \times X \to K \times X \xrightarrow{\mathrm{pr}_2} X $, where $ \alpha(s, x) = (s, s.x) $. $ \alpha $ is a homeomorphism, for $ \alpha^{-1} : (s, y) \to (s, s^{-1}.y) $ is continuous. Since K is quasi-compact, $ \mathrm{pr}_2 $ is proper (Chapter I, § 10, no. 2, Theorem 1, Corollary 5); hence $ \rho $ is proper (Chapter I, § 10, no. 1, Proposition 5).

#### Corollary 1 {#top-iii-s4-prop-1-cor-1 .statement}

If A is a closed (resp. compact) subset of X, then K.A is closed in X (resp. compact if X is Hausdorff).

The assertion concerning closed sets follows from Proposition 1 and the fact that a proper mapping is closed (Chapter I, § 10, no. 1, Proposition 1). The assertion concerning compact sets is trivial.

It should be noted that if L is a compact subset of X, and F a closed subset of G, then F.L is not necessarily closed in X ($ \S 2 $, Exercise 29; cf. no. 5, Corollary to Proposition 12).

#### Corollary 2 {#top-iii-s4-prop-1-cor-2 .statement}

If K is a quasi-compact subgroup of a topological group G, then the equivalence relation $ x^{-1}y \in K $ is closed, and the canonical mapping $ \varphi : G \to G/K $ is proper.

#### Corollary 3 {#top-iii-s4-prop-1-cor-3 .statement}

Let K be a quasi-compact normal subgroup of a topological group G, and let φ be the canonical mapping G → G/K. Then for each closed subgroup A of G the canonical bijection of A/A ∩ K onto φ(A) is an isomorphism of topological groups.

Since x⁻¹y ∈ K is a closed equivalence relation (Corollary 2), the Corollary follows from Chapter I, § 5, no. 2, Proposition 4.

#### Proposition 2 {#top-iii-s4-prop-2 .statement}

Let K be a compact group operating continuously on a Hausdorff space X. Then:

a) K operates properly on X.
b) The mapping (s, x) → s.x of K × X into X is proper.
c) The canonical mapping of X onto X/K is proper.

b) is a consequence of Proposition 1. As to a), since K is compact, pr₂ : (s, x) → x is proper (Chapter I, § 10, no. 2, Theorem 1, Corollary 5); hence, X being Hausdorff, (s, x) → (x, s.x) is proper (Chapter I, § 10, no. 1, Proposition 5, Corollary 3). It remains to prove c). By Corollary 1 to Proposition 1, the canonical mapping φ : X → X/K is closed. If Z is any topological space and if we make K operate trivially on Z, then K operates continuously on X × Z and hence the canonical mapping X × Z → (X × Z)/K is closed. But (X × Z)/K can be canonically identified with (X/K) × Z (§ 2, no. 4, Lemma 2 and Chapter I, § 5, no. 3, Corollary to Proposition 8); hence the canonical mapping X × Z → (X × Z)/K can be identified with φ × 1, and since it is closed for all Z it follows that φ is proper.

#### Corollary 1 {#top-iii-s4-prop-2-cor-1 .statement}

Under the hypotheses of Proposition 2, X is compact (resp. locally compact) if and only if X/K is compact (resp. locally compact).

This follows from the fact that the canonical mapping X → X/K is proper, in view of Proposition 9 of Chapter I, § 10, no. 4.

#### Corollary 2 {#top-iii-s4-prop-2-cor-2 .statement}

Let G be a Hausdorff topological group and let K be a compact subgroup of G. Then G is compact (resp. locally compact) if and only if G/K is compact (resp. locally compact).

Apply Corollary 1 to K operating on G by right translations.

### 2. PROPERTIES OF GROUPS ACTING PROPERLY

#### Proposition 3 {#top-iii-s4-prop-3 .statement}

*If a topological group* $ G $ *operates properly on a topological space* $ X $, *then the orbit space* $ X/G $ *is Hausdorff*. *If also* $ G $ *is Hausdorff*, *then* $ X $ *is Hausdorff*.

Let $ C \subset X \times X $ be the graph of the equivalence relation $ R $ defined by $ G $ on $ X $; then $ C $ is the image of $ G \times X $ under the mapping $ \theta : (s, x) \to (x, s.x) $. Since $ \theta $ is proper, $ C $ is closed in $ X \times X $ (Chapter I, § 10, no. 1, Proposition 1). Since the relation $ R $ is open ($ \S 2 $, no. 4, Lemma 2), it follows that $ X/G $ is Hausdorff (Chapter I, § 8, no. 3, Proposition 8).

Now suppose that $ G $ is Hausdorff. Then the mapping $ x \to (e, x) $ of $ X $ into $ G \times X $ is a homeomorphism of $ X $ onto a closed subspace of $ G \times X $, and is therefore proper (Chapter I, § 10, no. 1, Proposition 2). If we compose this mapping with the mapping $ (s, x) \to (x, s.x) $ of $ G \times X $ into $ X \times X $, which by hypothesis is proper, we obtain a proper mapping of $ X $ into $ X \times X $, namely the diagonal mapping $ x \to (x, x) $. Hence the diagonal $ \Delta $ of $ X \times X $ is closed in $ X $, and therefore $ X $ is Hausdorff.

#### Proposition 4 {#top-iii-s4-prop-4 .statement}

*Let* $ G $ *be a topological group operating properly on a topological space* $ X $, *and let* $ x $ *be a point of* $ X $. *Let* $ G.x $ *denote the orbit of* $ x $, *and let* $ K_x $ *denote the stabilizer of* $ x $. *Then*:

a) *The mapping* $ s \to s.x $ *of* $ G $ *into* $ X $ *is proper*.

b) $ K_x $ *is quasi-compact*.

c) *The canonical mapping of* $ G/K_x $ *onto* $ G.x $ *is a homeomorphism*.

d) *The orbit* $ G.x $ *is closed in* $ X $.

The inverse image of $ \{ x \} \times X $ under $ \theta : (s, x) \to (x, s.x) $ is $ G \times \{ x \} $; hence, by Proposition 3 of Chapter I, § 10, no. 1, the restriction of $ \theta $ to $ G \times \{ x \} $ is a proper mapping of $ G \times \{ x \} $ into $ \{ x \} \times X $, whence a) follows. Since $ K_x $ is the inverse image of $ x $ under $ s \to s.x $, b) follows from Chapter I, § 10, no. 2, Theorem 1. c) and d) are consequences of a), by virtue of Chapter I, § 10, no. 1, Propositions 2 and 5 b).

#### Remark {#top-iii-s4-n2-rem-1 .statement}

Proposition 4 shows that if a topological group $ G $ operates properly on a homogeneous space $ G/H $, then the subgroup $ H $ is quasi-compact (and therefore compact if $ G $ is Hausdorff). It can be shown that this is also a sufficient condition for $ G $ to operate properly on $ G/H $ (Exercise 3).

#### Proposition 5 {#top-iii-s4-prop-5 .statement}

*Let* $ G $ *(resp.* $ G' $) *be a topological group operating continuously on a topological space* $ X $ *(resp.* $ X' $). *Let* $ \varphi $ *be a continuous homomorphism* of $ G $ into $ G' $ and let $ \psi $ be a continuous mapping of $ X $ into $ X' $ compatible with $ \varphi $ (\S 2, no. 4). Then:

(i) *If $ \varphi $ is surjective and $ \psi $ is surjective and proper, and if $ G $ operates properly on $ X $, then $ G' $ operates properly on $ X' $.*

(ii) *If $ \varphi $ is proper, if $ G' $ operates properly on $ X' $ and if $ X $ is Hausdorff, then $ G $ operates properly on $ X $.*

To prove (i), consider the commutative diagram

$$
\begin{array}{ccc}
G \times X & \xrightarrow{\theta} & X \times X \\
\alpha \downarrow & & \downarrow \beta \\
G' \times X' & \xrightarrow{\theta'} & X' \times X'
\end{array}
$$

where $ \alpha = \varphi \times \psi $ and $ \beta = \psi \times \psi $. By hypothesis, $ \theta $ is proper; so is $ \beta $ [Chapter I, \S 10, no. 1, Proposition 4 a)]; hence $ \beta \circ \theta = \theta' \circ \alpha $ is proper [Chapter I, \S 10, no. 1, Proposition 5 a)]. Since $ \alpha $ is surjective it follows that $ \theta' $ is proper [Chapter I, \S 10, no. 1, Proposition 5 b)].

To prove (ii) consider an ultrafilter $ U $ on $ G \times X $, such that the mappings

$$
(s, x) \to s.x \quad \text{and} \quad (s, x) \to x
$$

converge with respect to $ U $ to $ y_0 $ and $ x_0 $ respectively. It follows that $ (s, x) \to \varphi(s).\psi(x) $ and $ (s, x) \to \psi(x) $ converge with respect to $ U $. Since $ G' $ operates properly on $ X' $, this implies (no. 1) that $ (s, x) \to \varphi(s) $ converges with respect to $ U $ to a point $ s'_0 \in G' $. Since $ \varphi $ is proper, we deduce (Chapter I, \S 10, no. 2, Theorem 1) that $ (s, x) \to s $ converges with respect to $ U $ to a point $ s_0 \in G $. The uniqueness of the limit in $ X $ then shows that $ y_0 = s_0 x_0 $, and hence that $ G $ operates properly on $ X $ (no. 1).

### 3. GROUPS OPERATING FREELY ON A TOPOLOGICAL SPACE

#### Definition 2 {#top-iii-s4-def-2 .statement}

*Let $ G $ be a group operating on a set $ X $. $ G $ is said to operate freely on $ X $ if the stabilizer of every element of $ X $ is $ \{e\} $, in other words if the relations $ s.x = x,\ s \in G,\ x \in X $ imply $ s = e $.*

#### Example {#top-iii-s4-n3-exa-1 .statement}

Let $ G $ be a group and let $ H $ be a subgroup of $ G $. Then $ H $ operates freely by (left or right) translations on $ G $.

Let $ G $ be a group operating freely on a set $ X $, let $ R $ be the equivalence relation defined by $ G $ on $ X $, and let $ C \subset X \times X $ be the graph of $ R $. If $ (x, y) \in C $, then there exists $ s \in G $ such that $ s.x = y $; and $ s $ is *unique*, since $ s.x = s'.x $ implies $ s'^{-1}s.x = x $, and therefore $ s'^{-1}s = e $ (as $ G $ operates freely). If we make correspond to $ (x, y) \in C $ the unique $ s \in G $ such that $ s.x = y $, we define a mapping $ \varphi : C \to G $, which we shall call the canonical mapping of $ C $ into $ G $. With this notation:

#### Proposition 6 {#top-iii-s4-prop-6 .statement}

*Let $ G $ be a topological group operating continuously on a topological space $ X $, and suppose that $ G $ operates freely on $ X $. Then $ G $ operates properly on $ X $ if and only if the following condition is satisfied:*

(FP) *The graph $ C $ of the equivalence relation defined by $ G $ is closed in $ X \times X $, and the canonical mapping $ \varphi : C \to G $ is continuous.*

The set $ C $ is the image of the mapping $ \theta : (s, x) \to (x, s.x) $ of $ G \times X $ into $ X \times X $. We know (Chapter I, § 10, no. 1, Proposition 2) that $ \theta $ is proper if and only if $ C $ is closed in $ X \times X $ and (if $ \theta' $ denotes the mapping $ \theta $ considered as a mapping of $ G \times X $ into $ C $) $ \theta' $ is a homeomorphism. Now the hypothesis implies that $ \theta' $ is bijective and that its inverse is the mapping $ (x, y) \to (\varphi(x, y), x) $. Hence $ \theta' $ is a homeomorphism if and only if $ \varphi $ is continuous.

### 4. LOCALLY COMPACT GROUPS OPERATING PROPERLY

#### Proposition 7 {#top-iii-s4-prop-7 .statement}

*Let $ G $ be a locally compact group operating continuously on a Hausdorff space $ X $. Then $ G $ operates properly on $ X $ if and only if, for each pair of points $ x, y $ of $ X $, there is a neighbourhood $ V_x $ of $ x $ and a neighbourhood $ V_y $ of $ y $ such that the set $ K $ of all $ s \in G $ for which $ s.V_x \cap V_y \neq \emptyset $ is relatively compact in $ G $.*

Let $ F $ be the compact space obtained by adjoining a point at infinity $ \omega $ to $ G $, and let $ \Gamma $ be the graph of $ \rho : (s, x) \to s.x $ considered as a subset of $ F \times X \times X $. Let us show that if the restriction of $ \mathrm{pr}_{23} $ to $ \Gamma $ is proper, then $ \Gamma $ is *closed in* $ F \times X \times X $. Indeed, this hypothesis implies that the map $ u : (t, s, x, y) \to (t, x, y) $ of $ F \times \Gamma $ into $ F \times X \times X $ is closed. If $ \Gamma' $ is the set of points $ (s, s) $ in $ F \times G $, where $ s \in G $, then $ \Gamma' $ is closed in $ F \times G $, since it is the graph of the canonical injection $ G \to F $ (Chapter I, § 8, no. 1, Corollary 2 to Proposition 2); hence the intersection $ (\Gamma' \times X \times X) \cap (F \times \Gamma) $ is closed in $ F \times \Gamma $, and it is immediately seen that its image under $ u $ is the set $ \Gamma $ considered as a subset of $ F \times X \times X $; hence $ \Gamma $ is closed in $ F \times X \times X $. Now, we have $ (\{\omega\} \times X \times X) \cap \Gamma = \emptyset $. From the definition of $ F $, therefore, for every point $ (x, y) \in X \times X $ there is a neighbourhood $ W $ of $ (x, y) $ in $ X \times X $ and a compact subset $ K $ of $ G $ such that

$$
((G - K) \times W) \cap \Gamma;
$$

is empty; and since we may take $ W $ to be a neighbourhood $ V_x \times V_y $, where $ V_x $ and $ V_y $ are neighbourhoods of $ x $ and $ y $ respectively in $ X $, the statement “((G — K) × W) ∩ Γ = ∅” becomes “if s ∉ K, then s · V_x ∩ V_y = ∅”. We have thus proved the necessity of the condition stated in the proposition. Conversely, suppose this condition is satisfied; let A be a set filtered by an ultrafilter 𝔾, and let α → (s_α, x_α) be a mapping of A into G × X such that lim_𝔖 x_α = x and lim_𝔖 s_α · x_α = y. Suppose that K, V_x and V_y satisfy the condition of the proposition. By hypothesis there is a set M ∈ 𝔾 such that if α ∈ M then x_α ∈ V_x and s_α · x_α ∈ V_y, hence s_α ∈ K. This shows that α → s_α converges with respect to 𝔾, and the proof is complete.

If G is compact, the condition of Proposition 7 is trivially satisfied; we thus retrieve Proposition 2 a).

Proposition 7 shows in particular that a discrete group G, operating continuously on a Hausdorff space X, operates properly on X if and only if, for each pair (x, y) of points of X, there is a neighbourhood V_x of x and a neighbourhood V_y of y such that the set of points s ∈ G for which s · V_x ∩ V_y ≠ ∅ is finite.

#### Proposition 8 {#top-iii-s4-prop-8 .statement}

Let G be a discrete group operating properly on a Hausdorff space X. Let x be a point of X and let K_x be the stabilizer of x. Then:

a) The subgroup K_x is finite and there is an open set U ⊂ X, containing x, which is stable under K_x, and on which the equivalence relation induced by the relation defined by G is the equivalence relation defined by K_x.

b) The canonical mapping U/K_x → X/G is a homeomorphism of U/K_x onto an open neighbourhood of the class of x in X/G.

By Proposition 7, K_x is finite. To construct an open set U which satisfies the required conditions, notice first that by Proposition 7 there is an open set U_0 containing x and such that the set K of s ∈ G for which s · U_0 ∩ U_0 ≠ ∅ is finite. Clearly K_x ⊂ K; let s_1, ..., s_n be the elements of K — K_x. If we put x_i = s_i · x (1 ≤ i ≤ n), then x_i ≠ x for each i; since X is Hausdorff, there is for each index i an open neighbourhood V_i of x and an open neighbourhood V'_i of s_i · x such that V_i ∩ V'_i = ∅. Let U_i = V_i ∩ s_i^{-1} · V'_i; then U_i is clearly open and contains x, and we have U_i ∩ s_i · U_i ⊂ V_i ∩ V'_i = ∅. Let U' = U_0 ∩ U_1 ∩ ... ∩ U_n; U' is open, contains x and is such that U' ∩ s · U' = ∅ for s ∉ K_x. Putting U = ⋂_{t ∈ K_x} t · U' we finally obtain an open set, stable under K_x, containing x and such that U ∩ s · U = ∅ for s ∉ K_x: U is the open set required.

The fact that the canonical mapping U/K_x → X/G is a homeomorphism of U/K_x onto an open set in X/G follows from Chapter I, § 5, no. 2, Proposition 4, since U is open and the equivalence relation defined by G is open (§ 2, no. 4, Lemma 2).

#### Corollary {#top-iii-s4-n4-cor-1 .statement}

*If we suppose in addition that $ K_x = \{ e \} $, then the point $ x $ has an open neighbourhood $ U $ such that the restriction to $ U $ of the canonical mapping $ X \to X/G $ is a homeomorphism of $ U $ onto an open subset of $ X/G $.*

### 5. GROUPS OPERATING CONTINUOUSLY ON A LOCALLY COMPACT SPACE

#### Proposition 9 {#top-iii-s4-prop-9 .statement}

*Let $ G $ be a topological group operating continuously on a locally compact space $ X $. Then if $ X/G $ is Hausdorff it is locally compact.*

Since the equivalence relation on $ X $ defined by $ G $ is open ($ \S 2 $, no. 4, Lemma 2), the proposition results from Chapter I, $ \S 10 $, no. 4, Proposition 10.

#### Proposition 10 {#top-iii-s4-prop-10 .statement}

*Let $ G $ be a topological group operating continuously on a locally compact space $ X $, and suppose that $ X/G $ is Hausdorff. Let $ \varphi $ be the canonical mapping of $ X $ onto $ X/G $. Then if $ K' $ is any compact subset of $ X/G $, there is a compact subset $ K $ of $ X $ such that $ \varphi(K) = K' $.*

Since the equivalence relation defined by $ G $ is open ($ \S 2 $, no. 4, Lemma 2), the proposition is a particular case of Proposition 10 of Chapter I, $ \S 10 $, no. 4.

#### Proposition 11 {#top-iii-s4-prop-11 .statement}

*Let $ G $ be a Hausdorff topological group operating properly on a non-empty space $ X $. If $ X $ is compact (resp. locally compact) then so are $ G $ and $ X/G $.*

By hypothesis, the mapping $ \theta : (s, x) \to (x, s.x) $ of $ G \times X $ into $ X \times X $ is proper; if $ X \times X $ is compact (resp. locally compact) then the Corollary to Proposition 9 of Chapter I, $ \S 10 $, no. 4 shows that $ G \times X $ is also compact (resp. locally compact), and therefore so is $ G $ since $ X \neq \emptyset $. Since $ X/G $ is Hausdorff (no. 2, Proposition 3), the compactness (resp. local compactness) of $ X $ implies the compactness (resp. local compactness) of $ X/G $ [Chapter I, $ \S 10 $, no. 4, Proposition 8 (resp. Proposition 9)] (see $ \S 2 $, Exercise 29).

We shall now give criteria which allow us to assert that a Hausdorff topological group $ G $ operates properly on a locally compact space $ X $. For each pair of subsets $ K, L $ of $ X $ we denote by $ P(K, L) $ the set of all $ s \in G $ such that $ s.K \cap L \neq \emptyset $.

#### Theorem 1 {#top-iii-s4-thm-1 .statement}

*Let $ G $ be a Hausdorff topological group which operates continuously on a topological space $ X $. Let $ K $ be a compact subset of $ X $ and let $ L $ be a closed subset of $ X $. Then:
a) The set $ P(K, L) $ is closed in $ G $.*

b) *If G operates properly on X and if L is compact, then P(K, L) is compact.*

c) *Conversely, if X is locally compact and if, for each pair K, L of compact subsets of X, P(K, L) is relatively compact in G [and therefore compact by a)]; then G operates properly on X (and if X is not empty, G is locally compact by Proposition 11).*

The mapping $(s, x) \to s.x$ of $G \times K$ into $X$ is continuous, and the inverse image $L'$ of $L$ under this mapping is therefore closed. Since $K$ is compact, the projection $\operatorname{pr}_1 : G \times K \to G$ is proper (Chapter I, § 10, no. 2, Corollary 5 of Theorem 1) and the image of $L'$ under $\operatorname{pr}_1$ is therefore closed. This image is $P(K, L)$, hence a) is proved.

To prove b): $X$ is Hausdorff (no. 2, Proposition 3). By hypothesis the mapping $\theta : (s, x) \to (x, s.x)$ of $G \times X$ into $X \times X$ is proper; since $K \times L$ is compact, so is $\overline{\theta}(K \times L)$ since $X$ is Hausdorff (Chapter I, § 10, no. 2, Proposition 6). Hence the projection $P(K, L)$ of $\overline{\theta}(K \times L)$ into $G$ is a compact set.

To prove c): since $K \times L$ is closed in $X \times X$, it follows that $\overline{\theta}(K \times L)$ is closed in $P(K, L) \times K$ and is therefore compact under the hypotheses of c). Since every compact subset of $X \times X$ is contained in a compact subset of the form $K \times L$, it follows that the inverse image of any compact subset of $X \times X$ under $\theta$ is compact, and since $X \times X$ is locally compact, this shows that $\theta$ is proper (Chapter I, § 10, no. 3, Proposition 7) [see Chapter IV, § 1, Exercise 4c)].

#### Remark {#top-iii-s4-n5-rem-1 .statement}

Clearly, we have $P(K, L) \subset P(K \cup L, K \cup L)$; therefore for $G$ to operate properly on a locally compact space $X$, it is sufficient that, for each compact subset $K$ of $X$, the set $P(K, K)$ is relatively compact in $G$. In particular, a *discrete* group $G$ operates properly on a locally compact space $X$ if and only if, for each compact subset $K$ of $X$, the set of $s \in G$ such that $s.K \cap K \neq \emptyset$ is *finite*.

#### Example {#top-iii-s4-n5-exa-1 .statement}

Let $X$ be a complex analytic manifold, analytically isomorphic to a bounded open subset of $\mathbf{C}^n$, and let $G$ be the group of analytic automorphisms of $X$. The topology of compact convergence is compatible with the group structure of $G$, and it can be shown that $G$ operates properly on $X$. In particular, every discrete subgroup of $G$ operates properly on $X$.

Take for example $X$ to be the upper half-plane $\mathcal{J}(z) > 0$, which is analytically isomorphic to an open disc in $\mathbf{C}$. Then $G$ is the group of all transformations $z \to (az + b)/(cz + d)$, where $a, b, c, d$ are real and $ad - bc \neq 0$. The subgroup $H$ of $G$ which consists of all such transformations for which $a, b, c, d$ are integers and $ad - bc = 1$ is a discrete subgroup of $G$, called the *modular group*. By what has been said above, it operates properly on the upper half-plane $\mathcal{J}(z) > 0$.*

#### Proposition 12 {#top-iii-s4-prop-12 .statement}

Let G be a Hausdorff topological group which operates continuously on a topological space X. Let K be a compact subset of X, and let $ \rho_K $ be the mapping $ (s, x) \to s.x $ of $ G \times K $ into X. Then:

a) If G operates properly on X, $ \rho_K $ is proper.

b) If X is locally compact and $ \rho_K $ is proper for each compact subset K of X, G operates properly on X.

The mapping $ \rho_K $ factorizes as $ G \times K \xrightarrow{\theta_K} K \times X \xrightarrow{\mathrm{pr}_2} X $, where $ \theta_K $ is the restriction to $ G \times K $ of the mapping $ \theta : (s, x) \to (x, s.x) $ of $ G \times X $ into $ X \times X $. Since $ \theta^{-1}(K \times X) = G \times K $, $ \theta_K $ is proper if $ \theta $ is proper (Chapter I, § 10, no. 1, Proposition 3). On the other hand, since K is compact, the projection $ \mathrm{pr}_2 : K \times X \to X $ is proper (Chapter I, § 10, no. 2, Theorem 1, Corollary 5), hence $ \rho_K $ is proper (ibid., no. 1, Proposition 5).

Suppose conversely that $ \rho_K $ is proper for each compact $ K \subset X $. If L is a compact subset of X, then $ \rho_K^{-1}(L) $ is a compact subset of $ G \times K $, whose projection into G is $ P(K, L) $; therefore $ P(K, L) $ is compact. Hence if X is locally compact it follows from Theorem 1 that G operates properly on X.

#### Corollary {#top-iii-s4-n5-cor-1 .statement}

Let G be a Hausdorff topological group operating properly on a topological space X. If K is any compact subset of X and if F is any closed subset of G, then F.K is closed in X.

This follows from Proposition 12 and from Chapter I, § 10, no. 1, Proposition 1.

### 6. LOCALLY COMPACT HOMOGENEOUS SPACES

#### Proposition 13 {#top-iii-s4-prop-13 .statement}

Let G be a locally compact group and let H be a closed subgroup of G. Then the homogeneous space $ G/H $ is locally compact and paracompact.

Since $ G/H $ is Hausdorff (\S 2, no. 5, Proposition 13) it is locally compact, by Proposition 9 of no. 5 applied to H operating on G on the right. Thus it remains to show that $ G/H $ is paracompact. Let V be a symmetric compact neighbourhood of e in G, and let $ G_0 = V^\infty $ be the subgroup of G generated by V. $ G_0 $ is open (\S 2, no. 1, Corollary to Proposition 4) and operates continuously on $ G/H $ (\S 2, no. 5, Proposition 12). If we can show that each of the orbits $ G_0.z \ (z \in G/H) $ is an open subset of $ G/H $ and a countable union of compact sets, then it will follow that $ G/H $ is the *topological sum* of the distinct orbits $ G_0.z $ and is

#### Proposition 14 {#top-iii-s4-prop-14 .statement}

*In a locally compact group $ G $, the identity component $ C $ is the intersection of the open subgroups of $ G $.*

$ C $ is a closed normal subgroup of $ G $ ($ \S 2 $, no. 2, Proposition 7), and hence $ G/C $ is locally compact (Proposition 13) and totally disconnected (Chapter I, $ \S 11 $, no. 5, Proposition 9). Since the inverse image of an open subgroup of $ G/C $, under the canonical mapping of $ G $ onto $ G/C $, is an open subgroup of $ G $ containing $ C $, we see that we can restrict ourselves to proving the proposition for the group $ G/C $. In other words, we may assume that $ G $ is totally disconnected. We know then (Chapter II, $ \S 4 $, no. 4, Corollary to Proposition 6) that every compact neighbourhood $ V $ of $ e $ contains a neighbourhood $ U $ of $ e $ which is both open and closed. Since $ U $ is compact and $ B = C U $ is closed, there is a symmetric open neighbourhood $ W $ of $ e $ such that $ W \subset U $ and $ UW \cap BW = \varnothing $ ($ \S 3 $, no. 1 and Chapter II, $ \S 4 $, no. 3, Proposition 4), and *a fortiori* $ UW \subset U $. By induction on $ n $ it follows that $ W^n \subset U $ for every integer $ n > 0 $. Hence the subgroup $ W^\infty = \bigcup_{n > 0} W^n $, generated by $ W $, is contained in $ U $; but $ W^\infty $ is open in $ G $ ($ \S 2 $, no. 1, Corollary to Proposition 4). This completes the proof.

We have also proved:

#### Corollary 1 {#top-iii-s4-prop-14-cor-1 .statement}

*If $ G $ is a totally disconnected locally compact group, then every neighbourhood of $ e $ in $ G $ contains an open subgroup of $ G $.*

#### Corollary 2 {#top-iii-s4-prop-14-cor-2 .statement}

*A locally compact group is connected if it is generated by each neighbourhood of the identity element.*

#### Corollary 3 {#top-iii-s4-prop-14-cor-3 .statement}

*Let $ G $ be a locally compact group, let $ H $ be a closed subgroup of $ G $, and let $ \varphi $ be the canonical mapping of $ G $ onto $ G/H $. Then the components of $ G/H $ are the closures of the images under $ \varphi $ of the components of $ G $.*

Let $ C $ be the identity component of $ G $. The components of $ G $ are the sets $ sC $, where $ s \in G $ ($ \S 2 $, no. 2, Proposition 7); $ \varphi(sC) $ is clearly connected, hence so is $ \varphi(sC) $ (Chapter I, $ \S 11 $, no. 1, Proposition 1). But $ \varphi(sC) = \varphi(sCH) $, and since $ sCH $ is saturated with respect to the equivalence relation defined by $ H $, and since this equivalence relation is open (§ 2, no. 4, Lemma 2), we have $ \overline{\varphi(sCH)} = \varphi(\overline{sCH}) = \varphi(s.\overline{CH}) $ (Chapter I, § 5, no. 3, Proposition 7).

Put $ L = CH $. $ L $ is a closed subgroup of $ G $ which contains $ C $ and $ H $; hence to prove that the sets $ \varphi(s.L) = s.\varphi(L) $ are the components of $ G/H $ it is enough to show that the quotient space of $ G/H $ by the equivalence relation whose classes are the sets $ s.\varphi(L) $ is totally disconnected. Now this quotient space is homeomorphic to the homogeneous space $ G/L $ (Chapter I, § 3, no. 4, Proposition 7); we are thus reduced to proving that when $ C \subset H $, $ G/H $ is *totally disconnected*. Since $ G/H $ may be identified with $ (G/C)/(H/C) $ (§ 2, no. 7, Proposition 22), we may even assume that $ G $ itself is totally disconnected. Every neighbourhood of $ \varphi(e) $ in $ G/H $ contains a neighbourhood of the form $ \varphi(V) $, where $ V $ is a neighbourhood of $ e $ in $ G $, and therefore (Corollary 1) contains a neighbourhood of the form $ \varphi(K) $, where $ K $ is a *compact open* subgroup of $ G $. $ \varphi(K) $ is therefore both open and closed in $ G/H $, and this shows that the component of $ \varphi(e) $ in $ G/H $ consists of $ \varphi(e) $ alone. By translation, the same is true for the component of every point of $ G/H $, and the corollary is proved.

### Exercises {#top-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
