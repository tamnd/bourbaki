---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 1
section_title: Uniform spaces
lang: en
source: top-i-iv
pdf_pages: 0175-0180, 0212-0213
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A UNIFORM STRUCTURE
      page: 0
      pdf_page: 175
    - "no": 2
      title: TOPOLOGY OF A UNIFORM SPACE
      page: 0
      pdf_page: 177
statements: 12
exercises: 4
content_sha256: 30414f7ac83e4f792549b3475521e040386f0105427eada0ac0293018d056ba2
---

## 1. UNIFORM SPACES

### 1. DEFINITION OF A UNIFORM STRUCTURE

#### Definition 1 {#top-ii-s1-def-1 .statement}

*A uniform structure* (or *uniformity*) *on a set* $ X $ *is a structure given by a set* $ \mathcal{U} $ *of subsets of* $ X \times X $ *which satisfies axioms* $ (\mathrm{F}_1) $ *and* $ (\mathrm{F}_{\mathrm{II}}) $ *of Chapter I, § 6, no. 1 and also satisfies the following axioms*:

(U₁) *Every set belonging to* $ \mathcal{U} $ *contains the diagonal* $ \Delta $.

(U₂) *If* $ V \in \mathcal{U} $ *then* $ \overline{V}^{-1} \in \mathcal{U} $.

(U₃) *For each* $ V \in \mathcal{U} $ *there exists* $ W \in \mathcal{U} $ *such that* $ W \circ W \subset V $.

![Figure 2](../images/chapter_ii_uniform_structures.png)

The sets of $ \mathcal{U} $ are called entourages of the uniformity defined on $ X $ by $ \mathcal{U} $. A set endowed with a uniformity is called a uniform space.

If $ V $ is an entourage of a uniformity on $ X $, we may express the relation $ (x, x') \in V $ by saying that "$ x $ and $ x' $ are $ V $-close".

#### Remark 1 {#top-ii-s1-n1-rem-1 .statement}

To make the language more expressive we may use the expressions "$ x $ is close enough to $ y $" and "$ x $ and $ y $ are as close as we please" in some statements. For example, we shall say that a relation

R $ \{ x, y \} $ is true whenever $ x $ and $ y $ are close enough if there is an entourage $ V $ such that the relation $ (x, y) \in V $ implies $ R \{ x, y \} $.

#### Remark 2 {#top-ii-s1-n1-rem-2 .statement}

The conjunction of axioms (U_{II}) and (U_{III}) is equivalent (assuming the other axioms of uniform structures) to the following axiom:

(U_a) For each $ V \in \mathcal{U} $ there exists $ W \in \mathcal{U} $ such that $ W \circ \overline{W} \subset V $ (*).

Clearly (U_{II}) and (U_{III}) imply (U_a). Conversely, if (U_a) is satisfied we have $ \overline{W} = \Delta \circ W \subset V $, by (U_I); hence $ W \subset \overline{V} $ and therefore [by (F_1)] $ \overline{V} \in \mathcal{U} $. Let $ W' = W \cap \overline{W} $; then $ W' \in \mathcal{U} $ by what has just been proved and axiom (F_{II}), and we have $ W' \circ W' \subset W \circ \overline{W} \subset V $.

Throughout this chapter we shall write $ \overline{V}^2 $ instead of $ V \circ V $, and in general $ \overline{V}^{n-1} = \overline{V} \circ V = V \circ \overline{V}^{n-1} $, for each integer $ n > 1 $ and each subset $ V $ of $ X \times X $.

#### Remark 3 {#top-ii-s1-n1-rem-3 .statement}

If $ X $ is not empty, then axiom (U_I) implies that no set of $ \mathcal{U} $ is empty, and therefore $ \mathcal{U} $ is a filter on $ X \times X $. There is only one uniformity on the empty set, namely $ \mathcal{U} = \{ \emptyset \} $.

Definition 2. A fundamental system of entourages of a uniformity is any set $ \mathcal{B} $ of entourages such that every entourage contains a set belonging to $ \mathcal{B} $.

Axiom (U_{III}) shows that if $ n $ is any integer $ > 0 $ and $ V $ runs through a fundamental system of entourages, then the sets $ \overline{V}^n $ again form a fundamental system of entourages.

Entourages $ V $ such that $ V = \overline{V}^1 $ are called symmetric. If $ V $ is any entourage, then $ V \cap \overline{V}^1 $ and $ V \cup \overline{V}^1 $ are symmetric entourages, and axioms (F_{II}) and (U_{II}) show that the symmetric entourages form a fundamental system of entourages.

A set $ \mathcal{B} $ of subsets of $ X \times X $ is a fundamental system of entourages of a uniformity on $ X $ if and only if $ \mathcal{B} $ satisfies axiom (B_I) of Chapter I, § 6, no. 3, and also satisfies the following axioms:

(U'_I) Every set of $ \mathcal{B} $ contains the diagonal $ \Delta $.

(U'_II) For each $ V \in \mathcal{B} $ there exists $ V' \in \mathcal{B} $ such that $ V' \subset \overline{V}^1 $.

(U'_III) For each $ V \in \mathcal{B} $ there exists $ W \in \mathcal{B} $ such that $ \overline{W}^2 \subset V $.

If $ X $ is not empty, a fundamental system of entourages of a uniform structure on $ X $ is a base of the filter formed by the entourages of this structure (Chapter I, § 6, no. 3, Proposition 3).

(*) We recall (Set Theory, R, § 3, nos. 4 and 10) that if $ V $ and $ W $ are two subsets of $ X \times X $, then the set of pairs $ (x, y) \in X \times X $, such that $ (x, z) \in W $ and $ (z, y) \in V $ for some $ z \in X $, is denoted by $ V \circ W $ or $ VW $, and that the set of pairs $ (x, y) \in X \times X $ such that $ (y, x) \in V $ is denoted by $ \overline{V}^1 $.

Examples of uniformities. \* 1) On the set $ \mathbf{R} $ of real numbers we can define a uniformity, called the *additive uniformity*, as follows: for each $ \alpha > 0 $ let $ V_\alpha $ be the subset of $ \mathbf{R} \times \mathbf{R} $ consisting of all pairs $ (x, y) $ such that $ |x - y| < \alpha $; as $ \alpha $ runs through the set of all real numbers $ > 0 $, the $ V_\alpha $ form a fundamental system of entourages for the additive uniformity on $ \mathbf{R} $. Similarly we can define a uniformity (again called the *additive uniformity*) on the set $ \mathbf{Q} $ of rational numbers; we shall study these structures, and analogous uniform structures on *groups*, in Chapters III and IV. \*
2) Let $ X $ be a set and let $ R $ be an *equivalence relation* on $ X $; let $ C $ be the graph of $ R $ in $ X \times X $. Then $ \Delta \subset C $ and $ \overset{2}{C} = \overset{-1}{C} = C $; (*Set Theory, R, § 5, no. 1*); the set of subsets of $ X \times X $ which consists of the set $ C $ alone is therefore a fundamental system of entourages of a uniformity on $ X $. In particular, if we take $ R $ to be the relation of equality, then $ C = \Delta $ and the entourages of the corresponding uniformity are *all the subsets* of $ X \times X $ which contain $ \Delta $; this uniformity is called the *discrete* uniformity on $ X $, and the set $ X $ endowed with this uniformity is called a *discrete uniform space*.
3) On the set $ \mathbf{Z} $ of rational integers we can define a uniformity, important in the theory of numbers, as follows: given a prime number $ p $, let $ W_n $ be the set of all pairs $ (x, y) \in \mathbf{Z} \times \mathbf{Z} $ such that $ x \equiv y \pmod{p^n} $, for each integer $ n > 0 $. It is easily verified that the sets $ W_n $ (for a fixed $ p $) form a fundamental system of entourages of a uniformity on $ \mathbf{Z} $, called the *$ p $-adic* uniformity (cf. Chapter III, § 6, Exercises 23 ff., and Chapter IX, § 3, no. 2).

In accordance with the general definitions (*Set Theory, R, § 8, no. 5*), if $ X $ and $ X' $ are two sets each endowed with uniformities whose sets of entourages are $ U $ and $ U' $ respectively, then a bijection $ f $ of $ X $ onto $ X' $ is an *isomorphism* of the uniformity of $ X $ onto that of $ X' $ if $ g(U) = U' $, where $ g = f \times f $.

For example, if $ X $ and $ X' $ are two equipotent sets, then every bijection of $ X $ onto $ X' $ is an isomorphism of the discrete uniformity of $ X $ onto the discrete uniformity of $ X' $.

### 2. TOPOLOGY OF A UNIFORM SPACE

#### Proposition 1 {#top-ii-s1-prop-1 .statement}

*Let $ X $ be a set endowed with a uniform structure $ U $, and for each $ x \in X $ let $ \mathcal{B}(x) $ be the set of subsets $ V(x) $ of $ X (*) $, where $ V $ runs through the set of entourages of $ U $. Then there is a unique topology on $ X $ such that, for each $ x \in X $, $ \mathcal{B}(x) $ is the neighbourhood filter of $ x $ in this topology.*

We have to show that the $ \mathcal{B}(x) $ satisfy conditions (V_I), (V_{II}), (V_{III}) and (V_{IV}) of Chapter I, § 1, no. 2. That this is so for the first three of

(*) We recall (*Set Theory, R, § 3, no. 7*) that if $ V $ is any subset of $ X \times X $ and $ x $ is any element of $ X $, then $ V(x) $ denotes the set of all $ y \in X $ such that $ (x, y) \in V $.

these conditions follows immediately from the fact that the entourages of $ \mathcal{U} $ satisfy $ (\mathbf{F}_I),\ (\mathbf{F}_{II}) $ and $ (\mathbf{U}_I) $. As to $ (\mathbf{V}_{IV}) $, let $ V $ be an entourage of $ \mathcal{U} $, $ W $ an entourage of $ \mathcal{U} $ such that $ \dot{W} \subset V $; then if $ (x, y) \in W $ and $ (y, z) \in W $ we have $ (x, z) \in V $, so that $ W(y) \subset V(x) $ for all $ y \in W(x) $, and therefore $ V(x) \in \mathfrak{B}(y) $ for all $ y \in W(x) $. This completes the proof.

#### Definition 3 {#top-ii-s1-def-3 .statement}

*The topology defined in Proposition 1 is called the topology induced by the uniform structure $ \mathcal{U} $.*

#### Example 1 {#top-ii-s1-n2-exa-1 .statement}

The topology induced by the additive uniformity on the set of real numbers is the topology of the real line (Chapter I, § 1, no. 2); similarly the topology induced by the additive uniformity on the set of rational numbers is the topology of the rational line.*
2) On any set $ X $, the topology induced by the discrete uniformity (no. 1, Example 2) is the discrete topology.

In the future, when we speak of the topology of a uniform space $ X $, we shall always mean the topology induced by the uniform structure of the space, unless the contrary is expressly stated. The topological space obtained by putting this topology on the set $ X $ is sometimes called the topological space *underlying* the uniform space in question. For example, when we say that a uniform space is *Hausdorff*, or *compact*, or *locally compact*, etc., we mean that the underlying topological space has this property.

If $ X $ and $ X' $ are two uniform spaces, any isomorphism $ f $ of the uniform structure of $ X $ onto that of $ X' $ is also a *homeomorphism* of $ X $ onto $ X' $; we say that $ X $ is an *isomorphism* of the uniform space $ X $ onto the uniform space $ X' $. It should be noted that a homeomorphism of $ X $ onto $ X' $ is not necessarily an isomorphism of the uniform structure of $ X $ onto that of $ X' $.

In other words, *distinct* uniformities on the same set $ X $ can induce the same topology. *For example, on ]0, +∞[, the *additive* and the *multiplicative* uniformities (which are distinct : Chapter III, § 6, Exercise 17) induce the same topology.*
For another example see § 2, no. 2, Remark 1.

#### Proposition 2 {#top-ii-s1-prop-2 .statement}

*Let $ X $ be a uniform space. For every symmetric entourage $ V $ of $ X $ and every subset $ M $ of $ X \times X $, $ VMV $ is a neighbourhood of $ M $ in the product space $ X \times X $, and the closure of $ M $ in this space is given by the formula*

$$
\overline{M} = \bigcap_{V \in \mathcal{S}} VMV
$$

*where $ \mathcal{S} $ denotes the set of symmetric entourages of $ X $.*

Let $ V $ be a symmetric entourage of $ X $. The relation $ (x, y) \in VMV $ means that there is an element $ (p, q) $ of $ M $ such that $ (x, p) \in V $ and $ (q, y) \in V $: in other words ($ V $ being symmetric) $ x \in V(p) $ and $ y \in V(q) $, that is $ (x, y) \in V(p) \times V(q) $. Since $ V(p) \times X(q) $ is a neighbourhood of $ (p, q) $ in $ X \times X $, the first part of the proposition is proved. The relations $ (x, p) \in V, (y, q) \in V $ can also be written $ p \in V(x), q \in V(y) $ or $ (p, q) \in V(x) \times V(y) $. As $ V $ runs through $ \mathcal{S} $, the sets $ V(x) \times V(y) $ form a fundamental system of neighbourhoods of $ (x, y) $ in $ X \times X $; for if $ U, U' $ are any two entourages there is always a symmetric entourage $ V \subset U \cap U' $, so that $ V(x) \times V(y) \subset U(x) \times U'(y) $. Hence $ V(x) \times V(y) $ meets $ M $ for each $ V \in \mathcal{S} $ if and only if $ (x, y) \in \overline{M} $, and formula (1) follows.

#### Corollary 1 {#top-ii-s1-prop-2-cor-1 .statement}

*If $ A $ is any subset of $ X $ and $ V $ is any symmetric entourage of $ X $, then $ V(A) $ is a neighbourhood of $ A $ in $ X $, and*

$$
\overline{A} = \bigcap_{V \in \mathcal{S}} V(A) = \bigcap_{U \in \mathfrak{U}} V(A)
$$

*where $ \mathfrak{U} $ denotes the set of all entourages in $ X $.*

If $ M = A \times A $, then $ VMV = V(A) \times V(A) $ for any $ V \in \mathcal{S} $; for the relation "there exists $ p \in A $ such that $ (x, p) \in V $" is by definition equivalent to $ x \in V(A) $. The corollary now follows from Chapter I, § 4, no. 2, Proposition 5 and no. 3, Proposition 7.

$ V(A) $ is said to be the *V-neighbourhood of* $ A $.

If $ V $ is an entourage which is *open* in $ X \times X $, then $ V(x) $ is open in $ X $ for each $ x \in X $ (Chapter I, § 4, no. 2, Corollary to Proposition 4) and therefore $ V(A) $, being the union of the $ V(x) $ as $ x $ runs through $ A $, is *open* in $ X $. On the other hand, if $ V $ is a closed entourage in $ X \times X $, $ V(A) $ need not be closed in $ X $ for every subset $ A $ of $ X $ (Exercise 3).

It should also be remarked that as $ V $ runs through the set of entourages of $ X $, the sets $ V(A) $ do not necessarily form a fundamental system of neighbourhoods of $ A $ in $ X $ (Exercise 2).

#### Corollary 2 {#top-ii-s1-prop-2-cor-2 .statement}

*The interiors (resp. the closures) of the entourages of $ X $ in $ X \times X $ form a fundamental system of entourages of $ X $.*

If $ V $ is any entourage of $ X $, there is a symmetric entourage $ W $ such that $ W \subset V $; since $ W $ is a neighbourhood of $ W $ (Proposition 2), the interior of $ V $ in $ X \times X $ contains $ W $ and is therefore an entourage. Furthermore, we have $ W \subset W \subset W \subset V $ by Proposition 2, and hence $ V $ contains the closure of an entourage.

#### Corollary 3 {#top-ii-s1-prop-2-cor-3 .statement}

*Every uniform space satisfies axiom* $ (O_{III}) $.

#### Proposition 3 {#top-ii-s1-prop-3 .statement}

*A uniform space $ X $ is Hausdorff if and only if the intersection of all the entourages of its uniform structure is the diagonal $ \Delta $ of $ X \times X $. Every Hausdorff uniform space is regular.*

The latter statement follows immediately from Corollary 3 to Proposition 2. We have seen that the closed entourages form a fundamental system of entourages (Proposition 2, Corollary 2); if their intersection is $ \Delta $, then $ \Delta $ is closed in $ X \times X $ and consequently $ X $ is Hausdorff (Chapter I, § 8, no. 1, Proposition 1). Conversely, if $ X $ is Hausdorff then for every point $ (x, y) \notin \Delta $ there is an entourage $ V $ of $ X $ such that $ y \notin V(x) $, or equivalently $ (x, y) \notin V $; hence $ \Delta $ is the intersection of all the entourages.

If a uniform space $ X $ is Hausdorff, we say that the uniform structure of $ X $ is *Hausdorff*. If $ \mathcal{B} $ is a fundamental system of entourages for this structure; then $ X $ is Hausdorff if and only if the intersection of all the sets of $ \mathcal{B} $ is $ \Delta $.

### Exercises {#top-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
