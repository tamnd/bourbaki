---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 3
section_title: Uniform structures on groups
lang: en
source: top-i-iv
pdf_pages: 0248-0256, 0312-0313
extraction: ocr
subsections:
    - "no": 1
      title: THE RIGHT AND LEFT UNIFORMITIES ON A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 248
    - "no": 2
      title: UNIFORMITIES ON SUBGROUPS, QUOTIENT GROUPS AND PRODUCT GROUPS
      page: 0
      pdf_page: 250
    - "no": 3
      title: COMPLETE GROUPS
      page: 0
      pdf_page: 251
    - "no": 4
      title: COMPLETION OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 252
    - "no": 5
      title: UNIFORMITY AND COMPLETION OF A COMMUTATIVE TOPOLOGICAL GROUP
      page: 0
      pdf_page: 254
statements: 17
exercises: 6
content_sha256: 8008ce640cebd669d9cf4b61aa73bcb16f18db8f57c6b4daef416edbe820a182
---

## 3. UNIFORM STRUCTURES ON GROUPS

### 1. THE RIGHT AND LEFT UNIFORMITIES ON A TOPOLOGICAL GROUP

In a topological group G we can perceive the possibility of defining a notion of "sufficiently near points" and hence a uniform structure, by operating as follows: if x and y are any two points of G, we apply to both points the translation which sends one of them, say x, to the identity element e; the "proximity" of x and y is then evaluated in some sense by the neighbourhood V of e into which y is translated. This translation, which consists in multiplying both x and y by $ x^{-1} $, can be carried out on the right or on the left, and we shall see that in either case we obtain effectively a uniformity on G which is compatible with the topology of G. Let us take the case in which the translations are performed on the right; then to each neighbourhood V of e there corresponds the set $ V_d $ of pairs $ (x, y) \in G \times G $ such that $ yx^{-1} \in V $. Let $ \mathcal{G}_d $ be the family of sets $ V_d $, as V runs through the neighbourhood filter $ \mathfrak{B} $ of e. Then $ \mathcal{G}_d $ is a fundamental system of entourages (Chapter II, § 1, no. 1). For since $ e \in V $, the diagonal $ \Delta $ of $ G \times G $ is contained in $ V_d $ for each $ V \in \mathfrak{B} $, hence $ \mathcal{G}_d $ is a filter base and satisfies axiom $ (U'_1) $; since the relations $ yx^{-1} \in V $ and $ xy^{-1} \in V^{-1} $ are equivalent, we have $ \overline{V}_d^1 = (V^{-1})_d $, hence $ \overline{V}_d^1 \in \mathcal{G}_d $ by (GV$_{\text{II}}$), so that (U'$_{\text{II}}$) is satisfied; and finally, the relations $ zx^{-1} \in V $ and $ yz^{-1} \in V $ imply $ yx^{-1} \in V.V $; hence $ V_d \circ V_d $ is contained in (V.V)$_d$, and (GV$_{\text{I}}$) shows that $ \mathcal{G}_d $ satisfies (U'$_{\text{III}}$).

The uniformity defined by $ \mathcal{G}_d $ is compatible with the topology of G, for the relations $ y \in V_d(x) $ and $ y \in V.x $ are equivalent by definition; in other words $ V_d(x) = V.x $.

The argument is analogous when the translations are on the left, and we may therefore make the following definition:

#### Definition 1 {#top-iii-s3-def-1 .statement}

*The right (resp. left) uniformity on a topological group G is the uniformity for which a fundamental system of entourages is obtained by making correspond to each neighbourhood V of the identity element e, the set V$_d$ (resp. V$_s$) of pairs $(x, y)$ such that $yx^{-1} \in V$ (resp. $x^{-1}y \in V$).*

If V runs through a fundamental system of neighbourhoods of e, the sets V$_d$ (resp. V$_s$) form a fundamental system of entourages of the right (resp. left) uniformity.

To each proposition on the topology of a uniform space there corresponds a proposition on the topology of a group; the translation is made according to Definition 1 and the formulae $ V_d(x) = V.x,\ V_d(A) = V.A,\ V_s(x) = x.V,\ V_s(A) = A.V, $ which are immediate consequences of the definition. For example, if A is any non-empty subset of G then we have (Chapter II, § 1, no. 2, Corollary 1 to Proposition 2)

$$
\overline{A} = \bigcap_{V \in \mathcal{B}} V.A = \bigcap_{V \in \mathcal{B}} A.V.
$$

Again (Chapter II, § 1, no. 2, Corollary 3 to Proposition 2), *every Hausdorff group is regular*.

The right and left uniformities on a topological group are in general distinct (see Exercise 4). Obviously they coincide if the group is *commutative*, for then $ V_d = V_s $; also they coincide if the group is *compact* (Chapter II, § 4, no. 1, Theorem 1).

In general, we shall denote by $ G_s $ (resp. $ G_d $) the *uniform space* obtained by giving the set G its left (resp. right) uniformity.

#### Proposition 1 {#top-iii-s3-prop-1 .statement}

*The left and right translations are isomorphisms of the right uniformity onto itself.*

As to the right translations, the result is clear, since the relation $ yx^{-1} \in V $ is equivalent to $(ya)(xa)^{-1} \in V$ [in other words, the mapping $(x, y) \to (xa, ya)$ leaves $V_d$ fixed]. For the left translations, the result follows from $ (GV_{\text{III}}) $; for $ yx^{-1} \in V $ if and only if $ (ay)(ax)^{-1} \in aV a^{-1} $; hence $ x \to ax $ is uniformly continuous on $ G_d $.

Similarly, the right and left translations are isomorphisms of the left uniformity onto itself.

Every *inner automorphism* $ x \to axa^{-1} $ of $ G $ is therefore an automorphism for the group structure of $ G $, for the topology of $ G $, and for both the uniformities of $ G $.

#### Proposition 2 {#top-iii-s3-prop-2 .statement}

*The symmetry* $ x \to x^{-1} $ *is an isomorphism of the right uniformity onto the left uniformity.*

This is an immediate consequence of Definition 1.

The reader should beware of supposing that the mapping $ (x, y) \to xy $ of the uniform space $ G_d \times G_d $ into the uniform space $ G_d $ is in general uniformly continuous. Similarly, the symmetry $ x \to x^{-1} $, considered as a mapping of $ G_d $ onto $ G_d $, is not in general uniformly continuous (see Exercises 3 and 4).

#### Proposition 3 {#top-iii-s3-prop-3 .statement}

*Every continuous homomorphism* $ f $ *of a topological group* $ G $ *into a topological group* $ G' $ *is uniformly continuous when considered as a mapping of* $ G_d $ *into* $ G'_d $ *(or of* $ G_s $ *into* $ G'_s $).

For if $ V' $ is a neighbourhood of the identity element in $ G' $, and $ V = \overline{f}^{-1}(V') $, then the relation $ yx^{-1} \in V $ implies
$$
f(y)(f(x))^{-1} = f(yx^{-1}) \in V'.
$$

### 2. UNIFORMITIES ON SUBGROUPS, QUOTIENT GROUPS AND PRODUCT GROUPS

If $ H $ is a subgroup of a topological group $ G $, then the uniformity induced on $ H $ by the right uniformity of $ G $ is none other than the right uniformity of the topological group $ H $.

If $ H $ is a normal subgroup of $ G $, and if $ \varphi $ is the canonical mapping of $ G $ onto $ G/H $, we obtain a fundamental system of entourages of the right uniformity of the quotient group $ G/H $ by associating with each neighbourhood $ V $ of the identity element in $ G $, the set of all pairs $ (\dot{x}, \dot{y}) $ of $ G/H $ such that $ \dot{x}\dot{y}^{-1} \in \varphi(V) $ (\S 2, no. 6, Proposition 17). This condition means that there is at least one point $ x \in \dot{x} $ and at least one point $ y \in \dot{y} $ such that $ yx^{-1} \in V $ [i.e. such that $ (x, y) \in V_d $]. In particular, if $ N $ is the closure of the subset $ \{e\} $ of $ G $, then the right uniformity on $ G/N $ is isomorphic to the Hausdorff uniformity *associated* with the right uniformity on $ G $ (cf. Chapter II, \S 3, no. 8).

There are analogous results for the left uniformity.

The left and right uniformities on the product group $\prod_{i \in I} G_i$ are identical if and only if the left and right uniformities on each factor $G_i$ coincide. This will always be the case if some of the $G_i$ are commutative and the others are compact.

### 3. COMPLETE GROUPS

#### Definition 2 {#top-iii-s3-def-2 .statement}

*A topological group is said to be complete if its left and right uniformities are structures of complete spaces.*

From Proposition 2 of no. 1, for a group to be complete it is sufficient that *one* of its uniformities is a structure of a complete space. $G$ is complete if and only if its associated Hausdorff group ($§\ 2$, no. 6) is complete.

Every *closed* subgroup of a complete group is complete (Chapter II, § 3, no. 4, Proposition 8). Every product of complete groups is complete (Chapter II, § 3, no. 5, Proposition 10).

On the other hand, if $G$ is a complete group and $H$ is a closed normal subgroup of $G$, then the quotient group $G/H$ is not necessarily complete (however, see Chapter IX, § 3, no. 1, Proposition 4).

#### Proposition 4 {#top-iii-s3-prop-4 .statement}

*If, in a topological group $G$, there is a neighbourhood $V$ of $e$ which is complete with respect to either the right or the left uniformity, then $G$ is complete.*

Suppose for example that $V$ is complete with respect to the right uniformity, and let $\mathfrak{F}$ be a Cauchy filter on $G_d$; then $\mathfrak{F}$ contains a $V_d$-small set $M$, and if $x_1 \in M$ we therefore have $M \subset Vx_1$. Hence the trace of $\mathfrak{F}$ on the complete subspace $Vx_1$ of $G_d$ is a Cauchy filter, which converges to a point $x_0$; since $x_0$ is a cluster point of $\mathfrak{F}$, it is a limit of $\mathfrak{F}$ (Chapter II, § 3, no. 2, Corollary 2 to Proposition 5).

#### Corollary 1 {#top-iii-s3-prop-4-cor-1 .statement}

*A locally compact group is complete.*

For every compact space is complete with respect to its unique uniformity (Chapter II, § 4, no. 1, Theorem 1).

#### Corollary 2 {#top-iii-s3-prop-4-cor-2 .statement}

*Every locally compact subgroup of a Hausdorff topological group $G$ is closed in $G$.*

#### Proposition 5 {#top-iii-s3-prop-5 .statement}

Let $ G_1 $ be a topological group, let $ G_2 $ be a complete Hausdorff topological group, and let $ H_1 $ (resp. $ H_2 $) be a dense subgroup of $ G_1 $ (resp. $ G_2 $). Then every continuous homomorphism $ u $ of $ H_1 $ into $ H_2 $ can be uniquely extended to a continuous homomorphism $ \bar{u} $ of $ G_1 $ into $ G_2 $. Furthermore, if $ G_1 $ is Hausdorff and complete, and if $ u $ is an isomorphism of $ H_1 $ onto $ H_2 $, then $ \bar{u} $ is an isomorphism of $ G_1 $ onto $ G_2 $.

$ \bar{u} $ is uniformly continuous with respect to the right uniformities of $ H_1 $ and $ H_2 $ (no. 1, Proposition 3), hence admits a unique extension to a mapping $ \bar{u} $ of $ G_1 $ into $ G_2 $ which is uniformly continuous with respect to the right uniformities of these groups (Chapter II, § 3, no. 6, Theorem 2). Moreover, by virtue of the principle of extension of identities (Chapter I, § 8, no. 1, Corollary 1 to Proposition 2), $ \bar{u} $ is a homomorphism of $ G_1 $ into $ G_2 $, whence the first assertion of the Proposition. To prove the second assertion, it is enough to consider the isomorphism $ v $ of $ H_2 $ onto $ H_1 $, which is the inverse of $ u $, and its extension $ \bar{v} $ to a continuous homomorphism of $ G_2 $ into $ G_1 $; by reason of the uniqueness of the extension, $ \bar{v} \circ \bar{u} $ and $ \bar{u} \circ \bar{v} $ are the identity mappings of $ G_1 $ and $ G_2 $ respectively, and therefore (Set Theory, R, § 2, no. 12) $ \bar{u} $ is bijective.

#### Remark {#top-iii-s3-n3-rem-1 .statement}

If the continuous homomorphism $ u $ is bijective, it does not follow in general that $ \bar{u} $ is either injective or surjective (cf. Exercise 12); but see no. 5, Proposition 9.

### 4. COMPLETION OF A TOPOLOGICAL GROUP

Let $ G $ be a Hausdorff topological group. The uniform space $ G_d $ may be considered as a dense subspace of its completion $ \hat{G}_d $. We shall investigate whether $ G $ can be considered as a dense subgroup of a complete Hausdorff group $ G' $. If so, then the uniform space $ G'_d $ must be isomorphic to $ \hat{G}_d $ (Chapter II, § 3, no. 6, Corollary to Theorem 2), and we must therefore be able to define on $ \hat{G}_d $ a topological group structure which induces the given topological group structure on $ G $. Consequently we have to examine:
1) Whether we can extend by continuity the functions $ xy $ and $ x^{-1} $ to $ \hat{G}_d \times \hat{G}_d $ and $ \hat{G}_d $ respectively; 2) whether the functions thus extended do indeed define a group structure on $ \hat{G}_d $ (they will then necessarily define a topological group structure on $ \hat{G}_d $ inducing the given structure on $ G $). We have next to establish that 3) when the preceding operations are possible, the topological group which they define is complete. Finally, we shall see that 4) if there is a complete group satisfying the given conditions, then it is unique up to isomorphism.

1) Extension of $ xy $ and $ x^{-1} $ by continuity. Since the functions $ xy $ and $ x^{-1} $ are not in general uniformly continuous, we cannot apply the theorem of extension of uniformly continuous functions (Chapter II, § 3, no. 6, Theorem 2). Nevertheless, we can extend $ xy $, by virtue of Proposition 11 of Chapter II, § 3, no. 6 and the following Proposition:

Proposition 6. Let $ \mathfrak{F} $ and $ \mathfrak{G} $ be two Cauchy filters on $ G_d $. Then the image of the filter $ \mathfrak{F} \times \mathfrak{G} $ under the mapping $ (x, y) \to xy $ is a Cauchy filter base on $ G_d $.

Let us evaluate the "proximity" of $ xy $ and $ x'y' $ in $ G_d $; in other words, let us form the product $ (x'y')(xy)^{-1} = x'y'y^{-1}x^{-1} $. For each $ a \in G $, we can also write $ (x'y')(xy)^{-1} = (x'a^{-1})(ay'y^{-1}a^{-1})(ax^{-1}) $. We shall see that by suitable choice of $ a $, each of the three factors of this product is very small whenever the pairs $ (x, y) $ and $ (x', y') $ belong to a sufficiently small set of $ \mathfrak{F} \times \mathfrak{G} $. Let $ V $ be any neighbourhood of $ e $ in $ G $; then there is a $ V_d $-small set $ A \in \mathfrak{F} $. Choose $ a $ in $ A $, then if $ x $ and $ x' $ are any two points of $ A $, we have $ x'a^{-1} \in V $ and $ ax^{-1} \in V $. On the other hand, the relation $ ay'y^{-1}a^{-1} \in V $ is equivalent to
$$
y'y^{-1} \in a^{-1}Va = W,
$$
and since $ W $ is a neighbourhood of $ e $, there is a $ W_d $-small set $ B \in \mathfrak{G} $. Hence for all $ (x, y) $ and $ (x', y') $ in $ A \times B $, we have $ (x'y')(xy)^{-1} \in V^3 $, and this completes the proof.

In order that $ x^{-1} $ can be extended by continuity to $ \hat{G}_d $ it is necessary and sufficient that *the image, under the symmetry* $ x \to x^{-1} $, *of a Cauchy filter on $ G_d $ is a Cauchy filter on $ G_d $* (Chapter II, § 3, no. 6, Proposition 11). There are examples of topological groups in which this condition is not satisfied (cf. Chapter X, § 3, Exercise 16); we shall suppose that it is satisfied for the remainder of this proof.

2) *The extended functions* $ xy $ and $ x^{-1} $ *define a group structure on* $ \hat{G}_d $. For if we apply the principle of extension of identities (Chapter I, § 8, no. 1, Proposition 2, Corollary 1) to the functions $ x(yz) $ and $ (xy)z $, defined on $ \hat{G}_d \times \hat{G}_d \times \hat{G}_d $ and equal on the dense subspace $ G_d \times G_d \times G_d $, we see that the law of composition $ (x, y) \to xy $ is *associative* on $ \hat{G}_d $. For the same reason, the functions $ x, ex, xe $ are identical on $ \hat{G}_d $, and the functions $ e, xx^{-1}, x^{-1}x $ are identical on $ \hat{G}_d $.

3) *The topological group* $ \hat{G}_d $ *is complete*. Let $ \mathcal{U}_d $ be its *right uniformity*, and let $ \mathcal{U} $ be the uniformity on $ \hat{G}_d $ obtained by *completing* the right uniformity of $ G $. Then $ \mathcal{U} $ and $ \mathcal{U}_d $ induce the *same* uniformity on $ G $, and therefore every Cauchy filter base $ \mathcal{B} $ *on* $ G $ *with respect to* $ \mathcal{U}_d $ *is also a Cauchy filter base with respect to* $ \mathcal{U} $. Now $ \mathcal{B} $ converges in $ \hat{G}_d $,

4) *Uniqueness.* This follows from Proposition 5 of no. 3.

To sum up, we have proved the following theorem:

#### Theorem 1 {#top-iii-s3-thm-1 .statement}

*A Hausdorff topological group $ G $ is isomorphic to a dense subgroup of a complete group $ \hat{G} $ if and only if the image, under the symmetry $ x \to x^{-1} $, of a Cauchy filter with respect to the right uniformity of $ G $ is a Cauchy filter with respect to this uniformity. The complete group $ \hat{G} $ (which is called the completion of $ G $) is then unique (up to isomorphism).*

#### Proposition 7 {#top-iii-s3-prop-7 .statement}

*Let $ G $ be a Hausdorff topological group which has a completion $ \hat{G} $. Then the closures in $ \hat{G} $ of the neighbourhoods of the identity element in $ G $ form a fundamental system of neighbourhoods of the identity element in $ \hat{G} $.*

Since $ \hat{G} $ is regular, every neighbourhood of the identity element in $ \hat{G} $ contains the closure $ V $ of an open neighbourhood $ U $ of $ e $ in $ \hat{G} $, and $ V $ is also the closure of the trace of $ U $ on $ G $.

Let $ G $ be a group which is not necessarily Hausdorff; let $ N = \overline{\{e\}} $, and let $ G' = G/N $ be the Hausdorff group associated with $ G $ (\S 2, no. 6). If $ G' $ has a completion $ \hat{G}' $, this completion is called the *Hausdorff completion* of $ G $ and is denoted by $ \hat{G} $; $ \hat{G}'_d $ (resp. $ \hat{G}'_s $) is then the *Hausdorff completion* (Chapter II, § 3, no. 7) of the uniform space $ G_d $ (resp. $ G_s $).

#### Proposition 8 {#top-iii-s3-prop-8 .statement}

*Let $ G $ be a topological group which has a Hausdorff completion $ \hat{G}' $. Then every continuous homomorphism $ u $ of $ G $ into a complete Hausdorff group $ H $ can be uniquely factorized into $ u = v \circ \varphi $, where $ v $ is a continuous homomorphism of $ \hat{G}' $ into $ H $ and $ \varphi $ is the canonical mapping of $ G $ into $ \hat{G}' $ (the composition of the canonical injection of $ G' $ into $ \hat{G}' $ and the canonical homomorphism $ \psi $ of $ G $ onto $ G/N = G' $).*

Since the kernel of $ u $ is closed and contains $ e $, it contains $ N $, and hence $ u $ can be written as $ u = w \circ \psi $, where $ w $ is a continuous homomorphism of $ G' $ into $ H $; now apply Proposition 5 of no. 3 to $ w $.

### 5. UNIFORMITY AND COMPLETION OF A COMMUTATIVE TOPOLOGICAL GROUP

We have already remarked that the left and right uniformities coincide on a commutative topological group $ G $; whenever we speak of *the uniformity* of $ G $, it is this unique uniformity to which we refer.

#### Theorem 2 {#top-iii-s3-thm-2 .statement}

Let $ G $ be a commutative topological group. Then the functions $ x^{-1} $ and $ xy $ are uniformly continuous on $ G $ and $ G \times G $ respectively. Moreover $ G $ admits a Hausdorff completion $ \hat{G} $, and $ \hat{G} $ is commutative.

The uniform continuity of $ x^{-1} $ follows from Proposition 2 of no. 1, and that of $ xy $ from Proposition 3 of no. 1, since $ (x, y) \to xy $ is a continuous homomorphism of $ G \times G $ into $ G $. If $ G $ is Hausdorff, it satisfies the condition of Theorem 1 of no. 4 (as does every Hausdorff group whose left and right uniformities coincide); moreover the functions $ xy $ and $ yx $ are equal on $ \hat{G} \times \hat{G} $ by the principle of extension of identities; hence the second part of the theorem, by considering in the general case the Hausdorff group associated with $ G $.

It follows in particular from this theorem that if $ f $ and $ g $ are two uniformly continuous mappings of a uniform space $ X $ into a commutative group $ G $, written additively, then the functions $ -f $ and $ f + g $ are uniformly continuous.

#### Proposition 9 {#top-iii-s3-prop-9 .statement}

Let $ G $ be a commutative group, and let $ \mathcal{T}_1, \mathcal{T}_2 $ be two Hausdorff topologies compatible with the group structure of $ G $. Suppose that $ \mathcal{T}_1 $ is finer than $ \mathcal{T}_2 $ and that there is a fundamental system of neighbourhoods of $ o $ for $ \mathcal{T}_1 $ which are closed for $ \mathcal{T}_2 $. Let $ G_1, G_2 $ be the completions of $ G $ with respect to the topologies $ \mathcal{T}_1, \mathcal{T}_2 $ respectively, and let $ f : G_1 \to G_2 $ be the continuous homomorphism which extends the identity mapping of $ G $ (no. 3, Proposition 5). Then $ f $ is injective.

Suppose that $ G $ is written additively. Let $ \mathcal{U}_1 $ be the uniformity on $ G $ corresponding (no. 1) to the topology $ \mathcal{T}_1 $: it will suffice to show that if $ \mathfrak{F} $ and $ \mathfrak{F}' $ are two minimal Cauchy filters (Chapter II, § 3, no. 2) with respect to $ \mathcal{U}_1 $, which converge in $ G_2 $ to the same point $ a $, then $ \mathfrak{F} = \mathfrak{F}' $ (Chapter II, § 3, no. 7). For this, it is enough to show that $ \mathfrak{F} \cap \mathfrak{F}' $ is a Cauchy filter with respect to $ \mathcal{U}_1 $. Let $ V $ be a neighbourhood of $ o $ in $ G $ with respect to $ \mathcal{T}_1 $, such that $ V $ is closed in $ \mathcal{T}_2 $, and let $ W $ be a symmetric neighbourhood of $ o $ in $ G $ with respect to $ \mathcal{T}_1 $, such that $ W + W \subset V $. By hypothesis, there is a $ W_d $-small set $ M $ (resp. $ M' $) in $ \mathfrak{F} $ (resp. $ \mathfrak{F}' $); if $ x \in M $ and $ y \in M $ we have $ y - x \in W $, i.e. $ y \in x + W $. If $ \overline{W} $ and $ \overline{V} $ are the closures of $ W $ and $ V $ in $ G_2 $, it follows that $ y \in x + \overline{W} $, and therefore, since $ a $ is in the closure of $ M $, that $ a \in x + \overline{W} $ for each $ x \in M $. Similarly, $ a \in x' + \overline{W} $ for each $ x' \in M' $, and hence $ x - x' \in \overline{W} + \overline{W} $; but since $ (x, y) \to x + y $ is a continuous mapping of $ G_2 \times G_2 $ into $ G_2 $, we have $ \overline{W} + \overline{W} \subset \overline{W} + \overline{W} \subset \overline{V} $. It follows that if $ x \in M $ and $ x' \in M' $, then $ x - x' \in \overline{V} \cap G = V $, because $ V $ is closed in $ \mathcal{T}_2 $; and this completes the proof.

#### Corollary 1 {#top-iii-s3-prop-9-cor-1 .statement}

Under the hypotheses of Proposition 9, if $ A $ is a subset of $ G $ which is a complete subspace with respect to the uniformity $ U_2 $ corresponding to $ \mathcal{T}_2 $, then $ A $ is also a complete subspace with respect to the uniformity $ U_1 $ corresponding to $ \mathcal{T}_1 $.

If $ A_1 $ is the closure of $ A $ in $ G_1 $, then $ f(A_1) $ is contained in the closure of $ A $ in $ G_2 $, which by hypothesis is equal to $ A $. Since $ f(A) = A $ by definition and $ f $ is injective, we have $ A_1 = A $.

#### Corollary 2 {#top-iii-s3-prop-9-cor-2 .statement}

Let $ G $ be a commutative group and let $ \mathcal{T}_1, \mathcal{T}_2 $ be two topologies compatible with the group structure of $ G $. Suppose that $ \mathcal{T}_1 $ is finer than $ \mathcal{T}_2 $ and that there is a fundamental system $ \mathcal{B} $ of neighbourhoods of $ O $ with respect to $ \mathcal{T}_1 $ which are complete with respect to the uniformity $ U_2 $ corresponding to $ \mathcal{T}_2 $. Then $ G $ is complete with respect to the uniformity $ U_1 $ corresponding to $ \mathcal{T}_1 $.

The sets of $ \mathcal{B} $ are closed in the topology $ \mathcal{T}_2 $, hence complete for the uniformity $ U_1 $ by Corollary 1; the result therefore follows from Proposition 4 of no. 3.

### Exercises {#top-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
