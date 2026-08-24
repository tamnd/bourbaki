---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 4
section_title: Groups and groups with operators
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0054-0076, 0156-0164
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS
      page: 0
      pdf_page: 54
    - "no": 2
      title: GROUPS WITH OPERATORS
      page: 0
      pdf_page: 55
    - "no": 3
      title: SUBGROUPS
      page: 0
      pdf_page: 56
    - "no": 4
      title: QUOTIENT GROUPS
      page: 0
      pdf_page: 58
    - "no": 5
      title: DECOMPOSITION OF A HOMOMORPHISM
      page: 0
      pdf_page: 61
    - "no": 6
      title: SUBGROUPS OF A QUOTIENT GROUP
      page: 0
      pdf_page: 62
    - "no": 7
      title: THE JORDAN-HÖLDER THEOREM
      page: 0
      pdf_page: 65
    - "no": 8
      title: PRODUCTS AND FIBRE PRODUCTS
      page: 0
      pdf_page: 69
    - "no": 9
      title: RESTRICTED SUMS
      page: 0
      pdf_page: 71
    - "no": 10
      title: MONOGENOUS GROUPS
      page: 0
      pdf_page: 72
statements: 62
exercises: 26
content_sha256: a50766c7ea0e8e219f8957f7048dd6cedcb552a260a50e8a6c749a7d24a174ce
---

## § 4. GROUPS AND GROUPS WITH OPERATORS

### 1. GROUPS

Recall the following definition (§ 2, no. 3, Definition 6).

#### Definition 1 {#alg-i-s4-def-1 .statement}

*A set with an associative law of composition, possessing an identity element and under which every element is invertible, is called a group.*

In other words, a group is a *monoid* (§ 2, no. 1, Definition 1) in which every element is invertible. A law of composition on a set which determines a group structure on it is called a *group law*. If G and H are two groups, a magma homomorphism of G into H is also called a *group homomorphism*. Such a homomorphism $ f $ maps identity element to identity element; for, let $ e $ (resp. $ e' $) be the identity element of G (resp. H); writing the group laws of G and H multiplicatively, $ e \cdot e = e $, whence $ f(e) \cdot f(e) = f(e) $ and, multiplying by $ f(e)^{-1}, f(e) = e' $. Hence $ f $ is unital. It then follows from no. 3 of § 2 that $ f(x^{-1}) = f(x)^{-1} $ for all $ x \in G $.

#### Example {#alg-i-s4-n1-exa-1 .statement}

In any monoid E the set of invertible elements with the structure induced by that on E is a group. In particular, the set of bijective mappings of a set F onto itself (or set of *permutations* of F) is a group under the law $ (f, g) \mapsto f \circ g $, called the *symmetric group of the set* F and denoted by $ \mathfrak{S}_F $.

In this paragraph, unless otherwise indicated, the law of composition of a group will always be written *multiplicatively* and $ e $ will denote the identity element of such a group law.

A group G is called *finite* if the underlying set of G is finite; otherwise it is called *infinite*; the cardinal of a group is called the *order* of the group.

If a law of composition on G determines a group structure on G, so does the opposite law. The mapping of a group G onto itself which associates with each $ x \in G $ the inverse of $ x $ is an *isomorphism* of G onto the opposite group (§ 2, no. 3, Proposition 4).

Following our general conventions (*Set Theory*, II, § 3, no. 1), we shall denote by $ A^{-1} $ the image of a subset A of G under the mapping $ x \mapsto x^{-1} $. But it is important to note that, in spite of the analogy of notation, $ A^{-1} $ is definitely not the inverse element of A under the law of composition $ (X, Y) \mapsto XY $ between subsets of G (recall that XY is the set of $ xy $ with $ x \in X, y \in Y $): the identity element under this law is $ \{e\} $ and the only invertible elements of $ \mathcal{P}(G) $ under this law are the sets A consisting of a single element (such an A, moreover, certainly has inverse $ A^{-1} $). The identity

$(AB)^{-1}=B^{-1}A^{-1}$ holds for $A\subset G$, $B\subset G$. $A$ is called a symmetric subset of $G$ if $A=A^{-1}$. For all $A\subset G$, $A\cup A^{-1}$, $A\cap A^{-1}$ and $AA^{-1}$ are symmetric.

### 2. GROUPS WITH OPERATORS

#### Definition 2 {#alg-i-s4-def-2 .statement}

Let $\Omega$ be a set. A group $G$ together with an action of $\Omega$ on $G$ which is distributive with respect to the group law, is called a group with operators in $\Omega$.

In what follows $x^\alpha$ will denote the composition of $\alpha\in\Omega$ and $x\in G$. Distributivity is then expressed by the identity $(xy)^\alpha=x^\alpha y^\alpha$.

In a group with operators $G$, each operator defines an *endomorphism* of the underlying *group structure*; these endomorphisms will sometimes be called the *homotheties* of the group with operators $G$.

A group with operators $G$ is called *commutative* (or *Abelian*) if its group law is commutative.

In what follows a group $G$ will be identified with the group with operators in $\varnothing$ obtained by giving $G$ the unique action of $\varnothing$ on $G$. This allows us to consider groups as special cases of groups with operators and to apply to them the definitions and results relating to the latter which we shall state.

#### Example {#alg-i-s4-n2-exa-1 .statement}

In a commutative group $G$, written multiplicatively, $(xy)^n=x^ny^n$ for all $n\in\mathbf{Z}$ (§ 2, no. 8, equation (1)); the action $n\mapsto(x\mapsto x^n)$ of $\mathbf{Z}$ on $G$ therefore defines, together with the group law, the structure of a group with operators on $G$.

#### Definition 3 {#alg-i-s4-def-3 .statement}

Let $G$ and $G'$ be groups with operators in $\Omega$. A homomorphism of groups with operators of $G$ into $G'$ is a *homomorphism of the group* $G$ into the *group* $G'$ such that

$$
f(x^\alpha)=(f(x))^\alpha
$$

for all $\alpha\in\Omega$ and all $x\in G$.

An *endomorphism* of the group with operators $G$ is an endomorphism of the group $G$ which is *permutable* with all the *homotheties* of $G$.

As two homotheties of a group with operators $G$ are not necessarily permutable, *a homothety of $G$ is not in general an endomorphism of the group with operators $G$.*

The identity mapping of a group with operators is a homomorphism of groups with operators; the composition of two homomorphisms of groups with operators is also one. For a mapping to be an isomorphism of groups with operators, it is necessary and sufficient that it be a bijective homomorphism of groups with operators and the inverse mapping is then an isomorphism of groups with operators.

31

More generally, let G (resp. G') be a group with operators in $ \Omega $ (resp. $ \Omega' $). Let $ \phi $ be a mapping of $ \Omega $ into $ \Omega' $. A $ \phi $-homomorphism of G into G' is a homomorphism of the group G into the group G' such that

$$
f(x^\alpha) = (f(x))^{(\phi(\alpha))}
$$

for all $ \alpha \in \Omega $ and all $ x \in G $.

In the rest of this paragraph we shall be given a set $ \Omega $. Unless otherwise mentioned the groups with operators considered will admit $ \Omega $ as set of operators.

### 3. SUBGROUPS

#### Definition 4 {#alg-i-s4-def-4 .statement}

*Let G be a group with operators. A stable subgroup of G is a subset H of G with the following properties*:

(i) $ e \in H $;
(ii) $ x, y \in H \implies xy \in H $;
(iii) $ x \in H \implies x^{-1} \in H $;
(iv) $ x \in H $ and $ \alpha \in \Omega $ imply $ x^\alpha \in H $.

If H is a stable subgroup of G, the structure induced on H by the structure of a group with operators on G is the structure of a group with operators and the canonical injection of H into G is a homomorphism of groups with operators.

Let G be a group. A stable subgroup of G with the action of $ \varnothing $ (no. 2), which is a subset of G satisfying conditions (i), (ii), (iii) of Definition 4, is called a *subgroup* of G. When we speak of a subgroup of a group of operators we shall always mean a subgroup of the underlying group of G. A subgroup of a group with operators G is not necessarily a stable subgroup of G.

*Example* (1). Let $ \Sigma $ be a species of structure (*Set Theory*, IV, § 1, no. 4) and S a structure of species $ \Sigma $ on a set E (*loc. cit.*). The set of *automorphisms* of S is a subgroup of $ \mathcal{G}_E $.

#### Proposition 1 {#alg-i-s4-prop-1 .statement}

*Let G be a group with operators and H a subset of G which is stable under the homotheties of G. The following conditions are equivalent*:

(a) *H is a stable subgroup of G*.
(b) *H is non-empty and the relations* $ x \in H, y \in H \implies xy \in H $ *and* $ x^{-1} \in H $.
(c) *H is non-empty and the relations* $ x \in H, y \in H \implies xy^{-1} \in H $.
(d) *H is stable under the law on G and the law of composition induced on H by the law of composition on G is a group law*.

Clearly (a) implies (b). We show that (b) implies (a). It suffices to show that H contains the identity element of G. As the subset H is non-empty, let $ x \in H $. Then $ x^{-1} \in H $ and $ e = xx^{-1} \in H $. Clearly (b) implies (c). We show that (c) implies (b). First of all since H is non-empty it contains an element x. Hence xx^{-1} = e is an element of H. For every element x of H, $ x^{-1} = ex^{-1} $ belongs to H; hence the relations $ x \in H, y \in H $ imply $ x(y^{-1})^{-1} = xy \in H $. Clearly (a) implies (d). We show that (d) implies (a): the canonical injection of H into G is a group homomorphism; hence $ e \in H $ and the relation $ x \in H $ implies $ x^{-1} \in H $ (no. 1).

#### Remark {#alg-i-s4-n3-rem-1 .statement}

(1) Similarly it can be shown that condition (b) is equivalent to the condition
(c') $ H \neq \varnothing $ and the relations $ x \in H $ and $ y \in H $ imply $ y^{-1}x \in H $.
(2) For every subgroup H of G there are the following relations
$$(1)$$
$$H.H = H \quad \text{and} \quad H^{-1} = H.$$
For $ H.H \subset H $ and $ H^{-1} \subset H $ by (b). As $ e \in H, H.H \supset e.H = H $ and taking inverses transforms the inclusion $ H^{-1} \subset H $ into $ H \subset H^{-1} $, whence formulae (1).

If H is a stable subgroup of G and K is a stable subgroup of H, clearly K is a stable subgroup of G.

The set $ \{e\} $ is the smallest stable subgroup of G. The intersection of a family of stable subgroups of G is a stable subgroup. There is therefore a smallest stable subgroup H of G containing a given subset X of G; it is called the *stable subgroup generated by* X and X is called a *generating system* (or *generating set*) of H.

#### Proposition 2 {#alg-i-s4-prop-2 .statement}

*Let X be a non-empty subset of a group with operators G and $ \hat{X} $ the stable subset under the action of $ \Omega $ on G generated by X. The stable subgroup generated by X is the stable subset under the law on G generated by the set $ Y = \hat{X} \cup \hat{X}^{-1} $.*

The latter subset Z is the set of compositions of finite sequences all of whose terms are elements of $ \hat{X} $ or inverse of elements of $ \hat{X} $: the inverse of such a composition is a composition of the same form (\S 2, no. 3, Corollary 1 to Proposition 5) and Z is stable under the action of $ \Omega $, as is seen by applying \S 3, no. 4, Proposition 1 to the homotheties of G, hence (Proposition 1) Z is a *stable subgroup* of G. Conversely, every stable subgroup containing X obviously contains Y and hence Z.

#### Corollary 1 {#alg-i-s4-prop-2-cor-1 .statement}

*Let G be a group with operators and X a subset of G which is stable under the action of $ \Omega $. The subgroup generated by X and the stable subgroup generated by X coincide.*

#### Corollary 2 {#alg-i-s4-prop-2-cor-2 .statement}

*Let G be a group and X a subset of G consisting of pairwise permutable elements. The subgroup of G generated by X is commutative.*

The set $ Y = X \cup X^{-1} $ consists of pairwise permutable elements (\S 2, no. 3, Proposition 5) and the law induced on the stable subset generated by Y is commutative (\S 1, no. 5, Corollary 2).

If G is a group with operators, the stable subgroup generated by a subset of G consisting of pairwise permutable elements is not necessarily commutative.

#### Corollary 3 {#alg-i-s4-prop-2-cor-3 .statement}

Let $ f : G \to G' $ be a homomorphism of groups with operators and X a subset of G. The image under f of the stable subgroup of G generated by X is the stable subgroup of G' generated by $ f(X) $.

Let $ X' = f(X) $. Then $ \hat{X}' = f(\hat{X}) $ and $ X'^{-1} = f(X^{-1}) $. Hence
$$
f(\hat{X} \cup \hat{X}^{-1}) = \hat{X}' \cup \hat{X}'^{-1}.
$$
The corollary then follows from § 1, no. 4, Proposition 1.

Example (2). Let G be a group and x an element of G. The subgroup generated by $ \{x\} $ (called more simply the subgroup generated by x) is the set of $ x^n, n \in \mathbf{Z} $. The stable subset (under the law on G) generated by $ \{x\} $ is the set of $ x^n $ where $ n \in \mathbf{N}^* $. These two sets are in general distinct.

Thus, in the additive group $ \mathbf{Z} $, the subgroup generated by an element x is the set $ x.\mathbf{Z} $ of $ xn, n \in \mathbf{Z} $, and the stable subset generated by x is the set of $ xn, n \in \mathbf{N}^* $. These two sets are always distinct if $ x \neq 0 $.

The union of a right directed family of stable subgroups of G is obviously a stable subgroup. It follows that, if P is a subset of G and H a stable subgroup of G not meeting P, the set of stable subgroups of G containing H and not meeting P, ordered by inclusion, is inductive (Set Theory, III, § 2, no. 4). Applying Zorn's Lemma (Set Theory, III, § 2, no. 4), we obtain the following result:

#### Proposition 3 {#alg-i-s4-prop-3 .statement}

Let G be a group with operators, P a subset of G and H a stable subgroup G not meeting P. The set of stable subgroups of G containing H and not meeting P has a maximal element.

### 4. QUOTIENT GROUPS

#### Theorem 1 {#alg-i-s4-thm-1 .statement}

Let R be an equivalence relation on a group with operators G; if R is left (resp. right) compatible (§ 3, no. 3) with the group law on G and compatible with the action of $ \Omega $, the equivalence class of e is a stable subgroup H of G and the relation R is equivalent to $ x^{-1}y \in H $ (resp. $ yx^{-1} \in H $). Conversely, if H is a stable subgroup of G, the relation $ x^{-1}y \in H $ (resp. $ yx^{-1} \in H $) is an equivalence relation which is left (resp. right) compatible with the group law on G and compatible with the action of $ \Omega $ and under which H is the equivalence class of e.

We restrict our attention to the case where the relation R is left compatible with the law on G (the case of a right compatible relation follows by replacing the law on G by the opposite law). The relation $ y \equiv x \pmod{R} $ is equivalent to $ x^{-1}y \equiv e \pmod{R} $, for $ y \equiv x $ implies $ x^{-1}y \equiv x^{-1}x = e $ and conversely $ x^{-1}y \equiv e $ implies $ y = x(x^{-1}y) \equiv x $. If H denotes the equivalence class of e, the relation R is then equivalent to $ x^{-1}y \in H $. We show that H is a stable subgroup of G. For every operator $ \alpha $, the relation $ x \equiv e $ implies $ x^\alpha \equiv e^\alpha = e $, hence $ H^\alpha \subset H $ and H is stable under the action of $ \Omega $. It suffices to establish (Proposition 1) that $ x \in H $ and $ y \in H $ imply $ x^{-1}y \in H $, that is $ x \equiv e $ and $ y \equiv e $ imply $ x \equiv y $, which is a consequence of the transitivity of R.

Conversely, let H be a stable subgroup of G; the relation $ x^{-1}y \in H $ is reflexive since $ x^{-1}x = e \in H $; it is symmetric since $ x^{-1}y \in H $ implies $ y^{-1}x = (x^{-1}y)^{-1} \in H $; it is transitive, for $ x^{-1}y \in H $ and $ y^{-1}z \in H $ imply $ x^{-1}z = (x^{-1}y)(y^{-1}z) \in H $; it is left compatible with the law of composition on G, for $ x^{-1}y = (zx)^{-1}(zy) $ for all $ z \in G $; finally, for every operator $ \alpha $, the relation $ y \in xH $ implies $ y^\alpha \in x^\alpha H^\alpha \subset x^\alpha H $ and hence the equivalence relation $ x^{-1}y \in H $ is compatible with the action of $ \Omega $ on G.

Let G be a group and H a subgroup of G; the relation $ x^{-1}y \in H $ (resp. $ yx^{-1} \in H $) is also written in the equivalent form $ y \in xH $ (resp. $ y \in Hx $). Every subgroup H of G thus defines two equivalent relations on G, namely $ y \in xH $ and $ y \in Hx $: the equivalent classes under these relations are respectively the sets $ xH $, which are called *left cosets of H* (or *modulo H*), and the sets $ Hx $, which are called *right cosets of H* (or *modulo H*). By *saturating* a subset $ A \subset G $ with respect to these relations (*Set Theory*, II, § 6, no. 4), we obtain respectively the sets AH and HA. The mapping $ x \mapsto x^{-1} $ transforms left cosets modulo H into right cosets modulo H and conversely.

The cardinal of the set of left cosets (mod. H) is called the *index* of the subgroup H with respect to G and is denoted by $ (G:H) $; it is also equal to the cardinal of the set of right cosets.

If a subgroup K of G contains H, it is a union of left (or right) cosets of H. Since a left coset of K is obtained from K by left translation, the set of left cosets of H contained in a left coset of K has cardinal independent of the latter. Hence (*Set Theory*, III, § 5, no. 8, Proposition 9):

#### Proposition 4 {#alg-i-s4-prop-4 .statement}

*Let H and K be two subgroups of a group G such that H $ \subset $ K. Then*
$$
(G:H) = (G:K)(K:H).
$$
**Corollary.** *If G is a finite group of order g and H is a subgroup of G of order h, then*
$$
h \cdot (G:H) = g
$$
(in particular, the order and index of H are *divisors* of the order of G).

Theorem 1 allows us to determine the equivalence relations compatible with the laws on a group with operators G: if R is such a relation, it is both left and right compatible with the group law on G and with the action of $ \Omega $. Hence, if H is the class of $ e $ (mod. R), H is a stable subgroup such that the relations $ y \in xH $ and $ y \in Hx $ are equivalent (since both are equivalent to R); hence $ xH = Hx $ for all $ x \in G $. Conversely, if this is so, one or other of the equivalent relations $ y \in xH, y \in Hx $ is compatible with the group law, since it is both left and right compatible with this law ($ \S $ 3, no. 4) and is compatible with the action of $ \Omega $. Since the equation $ xH = Hx $ is equivalent to $ xHx^{-1} = H $, we make the following definition:

#### Definition 5 {#alg-i-s4-def-5 .statement}

*Let G be a group with operators. A stable subgroup H of G is called a normal (or invariant) stable subgroup of G if $ xHx^{-1} = H $ for all $ x \in G $.*

If $ \Omega = \varnothing $, a normal stable subgroup of G is called a *normal* (or *invariant*) *subgroup* of G. In a commutative group every subgroup is normal.

To verify that a stable subgroup H is normal, it suffices to show that $ xHx^{-1} \subset H $ for all $ x \in G $; for if so then $ x^{-1}Hx \subset H $ for all $ x \in G $, that is $ H \subset xHx^{-1} $, and hence $ H = xHx^{-1} $.

Let H be a normal stable subgroup of G and R the equivalence relation $ y \in xH $ defined by H; on the quotient set $ G/R $, the internal law, the quotient by R of the law of the group G, is associative; the class of e is the identity element of this quotient law; the classes of two inverse elements in G are inverses under the quotient law and the action of $ \Omega $, the quotient by R of the action of $ \Omega $ on G, is distributive with respect to the internal law on $ G/R $ ($ \S $ 3, no. 5). Hence, summarizing the results obtained:

#### Theorem 2 {#alg-i-s4-thm-2 .statement}

*Let G be a group with operators. For an equivalence relation R on G to be compatible with the group law and the action of $ \Omega $, it is necessary and sufficient that it be of the form $ x^{-1}y \in H $, where H is a normal stable subgroup of G (the relation $ x^{-1}y \in H $ being moreover equivalent to $ yx^{-1} \in H $ for such a subgroup). The law of composition on $ G/R $ the quotient of that on G and the action of $ \Omega $ on $ G/R $ the quotient of that of $ \Omega $ on G by such a relation R give $ G/R $ the structure of a group with operators, called the quotient structure, and the canonical mapping of the passage to the quotient is a homomorphism of groups with operators.*

#### Definition 6 {#alg-i-s4-def-6 .statement}

*The quotient of a group with operators G by the equivalence relation defined by a normal subgroup H of G, with the quotient structure, is called the quotient group with operators of G by H and is denoted by $ G/H $. The canonical mapping $ G \to G/H $ is called a canonical homomorphism*

Let G be a group and H a normal subgroup of G. The quotient $ G/H $, with its group structure, is called the *quotient group* of G by H. For a mapping from $ G/H $ to a group with operators to be a homomorphism of groups with operators, it is necessary and sufficient that its composition with the canonical mapping of G onto $ G/H $ be one: this justifies the name "quotient group" (*Set Theory*, IV, $ \S $ 2, no. 6).

The equivalence relation defined by a normal stable subgroup of G is denoted by $ x \equiv y \pmod{H} $ or $ x \equiv y(H) $.

#### Proposition 5 {#alg-i-s4-prop-5 .statement}

Let $ f : G \to G' $ be a homomorphism of groups with operators and $ H $ and $ H' $ normal stable subgroups of $ G $ and $ G' $ respectively such that $ f(H) \subset H' $. The mapping $ f $ is compatible with the equivalence relations defined by $ H $ and $ H' $. Let $ \pi : G \to G/H $ and $ \pi' : G' \to G'/H' $ be the canonical homomorphisms. The mapping $ \bar{f} : G/H \to G'/H' $ derived from $ f $ by passing to the quotients is a homomorphism.

If $ x \equiv y \pmod{H} $, then $ x^{-1}y \in H $, whence
$$
f(x)^{-1}f(y) = f(x^{-1})f(y) = f(x^{-1}y) \in f(H) \subset H'
$$
and hence $ f(x) \equiv f(y) \pmod{H'} $. The second assertion follows from the universal property of quotient laws ($ \S 1 $, no. 6).

#### Remark {#alg-i-s4-n4-rem-1 .statement}

(1) If $ A $ is any subset of a group $ G $ and $ H $ is a normal subgroup of $ G $, then $ AH = HA $; this set is obtained by saturating $ A $ with respect to the relation $ x \equiv y \pmod{H} $.

(2) If $ H $ is a normal subgroup of $ G $ of finite index, the quotient group $ G/H $ is a finite group of order $ (G:H) $.

Note that if $ H $ is a normal subgroup of a group $ G $ and $ K $ is a normal subgroup of $ H $, $ K $ is not necessarily a normal subgroup of $ G $ (I, $ \S 5 $, Exercise 10).

Let $ G $ be a group with operators. The intersection of every family of normal stable subgroups of $ G $ is a normal stable subgroup. Hence, for every subset $ X $ of $ G $, there exists a smallest normal stable subgroup containing $ X $, called the normal stable subgroup *generated by* $ X $.

In a group with operators $ G $, the stable subgroups $ G $ and $ \{e\} $ are normal.

#### Definition 7 {#alg-i-s4-def-7 .statement}

*A group with operators* $ G $ *is called simple if* $ G \neq \{e\} $ *and there exists no normal stable subgroup of* $ G $ *other than* $ G $ *and* $ \{e\} $.

### 5. DECOMPOSITION OF A HOMOMORPHISM

#### Proposition 6 {#alg-i-s4-prop-6 .statement}

*Let* $ G $ *be a group with operators and* $ G' $ *a magma with an action by* $ \Omega $, *written exponentially*. *Let* $ f : G \to G' $ *be a homomorphism of the magna* $ G $ *into the magma* $ G' $ *such that, for all* $ \alpha \in \Omega $ *and all* $ x \in G $, $ f(x^\alpha) = f(x)^\alpha $. *Then* $ f(G) $ *is a stable subset of* $ G' $ *under the law on* $ G' $ *and the action of* $ \Omega $; *the set* $ f(G) $ *with the induced laws is a group with operators and the mapping* $ x \mapsto f(x) $ *of* $ G $ *into* $ f(G) $ *is a homomorphism of groups with operators*.

By virtue of $ \S 1 $, no. 4, Proposition 1, $ f(G) $ is a stable subset of $ G' $ under the internal law on $ G' $. For every element $ x \in G $ and for every operator $ \alpha $,
$ f(x)^\alpha = f(x^\alpha) \in f(G) $ and therefore $ f(G) $ is stable under the action of $ \Omega $ on $ G' $. Writing the internal law of $ G' $ multiplicatively,
$$
(f(x)f(y))f(z) = f(xy)f(z) = f((xy)z) = f(x(yz)) = f(x)f(yz)
= f(x)(f(y)f(z))
$$
for all elements $ x, y, z $ in $ G $; therefore the induced law on $ f(G) $ is associative.

Let $ e $ be the identity element of $ G $. Its image $ f(e) $ is an identity element of $ f(G) $ ($ \S 2 $, no. 1). Every element of $ f(G) $ is invertible in $ f(G) $ ($ \S 2 $, no. 3). Therefore the law induced on $ f(G) $ by the internal law on $ G' $ is a group law. For all elements $ x $ and $ y $ in $ G $ and every operator $ \alpha $,

$$
(f(x)f(y))^\alpha = (f(xy))^\alpha = f((xy)^\alpha) = f(x^\alpha y^\alpha) = f(x^\alpha)f(y^\alpha) = (f(x))^\alpha(f(y))^\alpha
$$

which shows that the action of $ \Omega $ is distributive with respect to the group law on $ f(G) $. Therefore $ f(G) $ with the induced laws is a group with operators and clearly the mapping $ x \mapsto f(x) $ is a homomorphism of groups with operators.

#### Definition 8 {#alg-i-s4-def-8 .statement}

*Let $ f : G \to G' $ be a homomorphism of groups with operators. The inverse image of the identity element of $ G' $ is called the kernel of $ f $.*

The kernel of $ f $ is often denoted by $ \mathrm{Ker}(f) $ and the image $ f(G) $ of $ f $ is sometimes denoted by $ \mathrm{Im}(f) $.

#### Theorem 3 {#alg-i-s4-thm-3 .statement}

*Let $ f : G \to G' $ be a homomorphism of groups with operators.*
(a) *$ \mathrm{Ker}(f) $ is a normal stable subgroup of $ G $;*
(b) *$ \mathrm{Im}(f) $ is a stable subgroup of $ G' $;*
(c) *the mapping $ f $ is compatible with the equivalence relation defined on $ G $ by $ \mathrm{Ker}(f) $;*
(d) *the mapping $ \tilde{f} : G/\mathrm{Ker}(f) \to \mathrm{Im}(f) $ derived from $ f $ by passing to the quotient is an isomorphism of groups with operators;*
(e) *$ f = i \circ \tilde{f} \circ \pi $, where $ i $ is the canonical injection of $ \mathrm{Im}(f) $ into $ G' $ and $ \pi $ is the canonical homomorphism of $ G $ onto $ G/\mathrm{Ker}(f) $.*

Assertion (b) follows from Proposition 6. The equivalence relation $ f(x) = f(y) $ on $ G $ is compatible with the group with operators structure on $ G $. By Theorem 2 (no. 4), it is therefore of the form $ y \in xH $, where $ H $ is a normal stable subgroup of $ G $ and $ H $ is the class of the identity element, whence $ H = \mathrm{Ker}(f) $. Assertions (a), (c) and (d) then follow. Assertion (e) is obvious (*Set Theory*, II, § 6, no. 5).

### 6. SUBGROUPS OF A QUOTIENT GROUP

#### Proposition 7 {#alg-i-s4-prop-7 .statement}

*Let $ G $ and $ H $ be two groups with operators, $ f $ a homomorphism of $ G $ into $ H $ and $ N $ the kernel of $ f $.*
(a) *Let $ H' $ be a stable subgroup of $ H $. The inverse image $ G' = f^{-1}(H') $ is a stable subgroup of $ G $ and $ G' $ is normal in $ G $ if $ H' $ is normal in $ H $. Further, $ N $ is a normal subgroup of $ G' $. If $ f $ is surjective, then $ H' = f(G') $ and $ f $ defines an isomorphism of $ G'/N $ onto $ H' $ on passing to the quotient.*
(b) *Let $ G' $ be a stable subgroup of $ G $. The image $ H' = f(G') $ is a stable subgroup of $ H $ and $ f^{-1}(H') = G'N = NG' $. In particular, $ f^{-1}(H') = G' $ if and only if $ N \subset G' $. If $ f $ is surjective and $ G' $ is normal in $ G $, then $ H' $ is normal in $ H $.*

(a) Let $ x $ and $ y $ be in $ G' $ and $ \alpha \in \Omega $; then $ f(x) \in H' $ and $ f(y) \in H' $, whence $ f(xy^{-1}) = f(x)f(y)^{-1} \in H' $, that is $ xy^{-1} \in G' $; hence $ G' $ is a subgroup of $ G $. Now $ f(x^\alpha) = f(x)^\alpha \in H' $, whence $ x^\alpha \in G' $ and therefore $ G' $ is stable. Suppose $ H' $ is normal in $ H $ and let $ x \in G', y \in G $; then $ f(x) \in H' $ and
$$
f(yxy^{-1}) = f(y)f(x)f(y)^{-1} \in H'
$$
whence $ yxy^{-1} \in G' $; hence $ G' $ is normal in $ G $. For all $ n \in N, f(n) = e \in H' $, whence $ N \subset G' $; as $ N $ is normal in $ G $, it is normal in $ G' $. Finally, if $ f $ is surjective,
$$
f(f^{-1}(A)) = A \text{ for every subset } A \text{ of } H,
$$
whence $ H' = f(G') $; the restriction of $ f $ to $ G' $ is a homomorphism $ f' $ of $ G' $ onto $ H' $ of kernel $ N $, hence $ f' $ defines on passing to the quotient an isomorphism of $ G'/N $ onto $ H' $.

(b) Let $ a $ and $ b $ be in $ H' $ and $ \alpha $ in $ \Omega $; there exist $ x, y $ in $ G' $ with $ a = f(x) $ and $ b = f(y) $, whence $ ab^{-1} = f(xy^{-1}) \in H' $, hence $ H' $ is a subgroup of $ H $ which is stable, for $ a^\alpha = f(x^\alpha) \in H' $. Let $ x \in G $; then $ x \in f^{-1}(H') $ if and only if $ f(x) \in H' = f(G') $, that is if and only if there exists $ y $ in $ G' $ with $ f(x) = f(y) $; the relation $ f(x) = f(y) $ is equivalent to the existence of $ n \in N $ with $ x = yn $; finally, $ x \in f^{-1}(H') $ is equivalent to $ x \in G'N = NG' $. Clearly the relation $ G' = G'N $ is equivalent to $ G' \supset N $. Suppose finally that $ f $ is surjective and $ G' $ is normal in $ G $; let $ a \in H' $ and $ b \in H $; there exist $ x \in G' $ and $ y \in G $ with $ a = f(x) $ and $ b = f(y) $, whence $ bab^{-1} = f(yxy^{-1}) \in f(G') = H' $. Hence $ H' $ is normal in $ H $.

#### Corollary 1 {#alg-i-s4-prop-7-cor-1 .statement}

*Suppose that $ f $ is surjective. Let $ \mathcal{G} $ (resp. $ \mathcal{G}' $) be the set of stable (resp. normal stable) subgroups of $ G $ containing $ N $ and $ \mathfrak{H} $ (resp. $ \mathfrak{H}' $) the set of stable (resp. normal stable) subgroups of $ H $, these sets being ordered by inclusion. The mapping $ G' \mapsto f(G') $ is an ordered set isomorphism $ \Phi : \mathcal{G} \to \mathfrak{H} $; the inverse isomorphism $ \Psi : \mathfrak{H} \to \mathcal{G} $ is the mapping $ H' \mapsto f^{-1}(H') $. Further $ \Phi $ and $ \Psi $ induce isomorphisms $ \Phi' : \mathcal{G}' \to \mathfrak{H}' $ and $ \Psi' : \mathfrak{H}' \to \mathcal{G}' $.

#### Corollary 2 {#alg-i-s4-prop-7-cor-2 .statement}

*Let $ f : G \to H $ be a homomorphism of groups with operators, $ N $ the kernel of $ f $, $ G' $ a stable subgroup of $ G $ and $ L $ a normal stable subgroup of $ G' $. Then $ LN, L.(G' \cap N) $ and $ f(L) $ are normal stable subgroups of $ G'N, G' $ and $ f(G') $ respectively and the three quotient groups with operators $ G'N/LN, G'/L.(G' \cap N) $ and $ f(G')/f(L) $ are isomorphic.

Let $ H' = f(G') $ and $ f' $ denote the homomorphism of $ G' $ onto $ H' $ which coincides with $ f $ on $ G' $; the kernel of $ f' $ is $ G \cap N $ and $ f'(L) = f(L) $; by Proposition 7, $ f'(L) $ is a normal stable subgroup of $ H' $ and
$$
f'^{-1}(f'(L)) = L.(G' \cap N)
$$
is a normal stable subgroup of $ G' $. Let $ \lambda $ be the canonical homomorphism of $ H' $ onto $ H'/f'(L) = f(G')/f(L) $: as $ \lambda \circ f' $ is surjective with kernel
$$
f'^{-1}(f'(L)) = L.(G' \cap N),
$$

it defines an isomorphism of $G'/L\cdot(G'\cap N)$ onto $f(G')/f(L)$. By Proposition 7, (b), $f^{-1}(H')=G'N$; if $f''$ is the homomorphism of $G'N$ onto $H'$ which coincides with $f$ on $G'N$, the homomorphism $\lambda\circ f''$ of $G'N$ onto $f(G')/f(L)$ is surjective with kernel $f^{-1}(f(L))=LN$; this proves that $LN$ is a normal stable subgroup of $G'N$ and that $\lambda\circ f''$ defines an isomorphism of $G'N/LN$ onto $f(G')/f(L)$.

#### Corollary 3 {#alg-i-s4-prop-7-cor-3 .statement}

Let $f:G\to H$ be a homomorphism of groups with operators, $N$ its kernel, $X$ a subset of $G$ such that $f(X)$ generates $H$ and $Y$ a subset of $N$ which generates $N$. Then $X\cup Y$ generates $N$.

Let $G'$ be the stable subgroup of $G$ generated by $X\cup Y$. As $Y\subset G'$, $N\subset G'$.

As $f(X)\subset f(G')$, $f(G')=H$, whence $G'=f^{-1}(H)=G$.

#### Remark {#alg-i-s4-n6-rem-1 .statement}

In the notation of Proposition 7, the fact that the inverse image of a subgroup of $H$ is a subgroup of $G$ follows from the following more general fact.

If $A$ and $B$ are subsets of $H$ and $f$ is surjective, then

$$
f^{-1}(A\cdot B)=f^{-1}(A)\cdot f^{-1}(B),\qquad
f^{-1}(A^{-1})=f^{-1}(A)^{-1}.
$$

Obviously $f^{-1}(A)\cdot f^{-1}(B)\subset f^{-1}(A\cdot B)$; on the other hand, if $z\in f^{-1}(A\cdot B)$, there exists $a\in A$ and $b\in B$ such that $f(z)=ab$; as $f$ is surjective, there exists $x\in G$ such that $f(x)=a$; writing $y=x^{-1}z$, $f(y)=a^{-1}f(z)=b$ and $z=xy$, whence $z\in f^{-1}(A)\cdot f^{-1}(B)$. The relation $x\in f^{-1}(A^{-1})$ is equivalent to $f(x)\in A^{-1}$, hence to $f(x^{-1})\in A$, that is to $x^{-1}\in f^{-1}(A)$ and finally to $x\in f^{-1}(A)^{-1}$.

#### Proposition 8 {#alg-i-s4-prop-8 .statement}

Let $G$ be a group with operators and $A$ and $B$ two stable subgroups of $G$. Suppose that the relations $a\in A$ and $b\in B$ imply $aba^{-1}\in B^{*}$ (in other words, $A$ normalizes $B$)$^{*}$. Then $AB=BA$ is a stable subgroup of $G$, $A\cap B$ is a normal stable subgroup of $A$ and $B$ is a normal stable subgroup of $AB$. The canonical injection of $A$ into $AB$ defines on passing to the quotient an isomorphism of $A/(A\cap B)$ onto $AB/B$.

The formulae

$$
(ab)(a'b')=aa'(a'^{-1}ba'\cdot b')
$$

$$
(ab)^{-1}=a^{-1}(ab^{-1}a^{-1})
$$

$$
(ab)^\alpha=a^\alpha b^\alpha
$$

for $a,a'\in A$, $b,b'\in B$ and every operator $\alpha$ on $G$, show that $AB$ is a stable subgroup of $G$. Let $a\in A$ and $x\in A\cap B$; then $axa^{-1}\in B$ by the hypotheses made on $A$ and $B$ and clearly $axa^{-1}$ belongs to $A$, hence $A\cap B$ is normal in $A$. Let $a\in A$ and $b,b'$ be in $B$; the formula $(ab)b'(ab)^{-1}=a(bb'b^{-1})a^{-1}$ shows that $B$ is normal in $AB$. Let $\phi$ be the restriction to $A$ of the canonical homomorphism

40 of AB onto AB/B; then $ \phi(a) = aB $ and hence the kernel of $ \phi $ is equal to $ A \cap B $. Clearly $ \phi $ is surjective and hence defines an isomorphism of $ A/(A \cap B) $ onto $ AB/B $.

#### Theorem 4 {#alg-i-s4-thm-4 .statement}

*Let G be a group with operators and N a normal stable subgroup of G.*

(a) *The mapping $ G' \mapsto G'/N $ is a bijection of the set of stable subgroups of G containing N onto the set of stable subgroups of G/N.*

(b) *Let $ G' $ be a stable subgroup of G containing N. For $ G'/N $ to be normal in $ G/N $, it is necessary and sufficient that $ G' $ be normal in G and the groups $ G/G' $ and $ (G/N)/(G'/N) $ are then isomorphic.*

(c) *Let $ G' $ be a stable subgroup of G. Then $ G'N $ is a stable subgroup of G and N is normal in $ G'N $. Further $ G' \cap N $ is normal in $ G' $ and the groups $ G'/(G' \cap N) $ and $ G'N/N $ are isomorphic.*

Let $ f $ denote the canonical homomorphism of G onto $ G/N $. For all $ x \in G $, $ f(x) \in xN $; therefore, $ f(G') = G'/N $ for every subgroup $ G' $ of G containing N. As $ f $ is surjective, assertion (a) follows from Corollary 1 to Proposition 7; similarly for the equivalence "G' normal" $ \Leftrightarrow $ "G'/N normal". Suppose that $ G' $ is a normal stable subgroup of G containing N. By no. 4, Proposition 5 applied to $ \mathrm{Id}_G $, there exists a homomorphism $ u $ of $ G/N $ into $ G/G' $ defined by $ u(xN) = xG' $ for all $ x \in G $. It is immediate that $ u $ is surjective with kernel $ G'/N $ whence the desired isomorphism of $ (G/N)/(G'/N) $ onto $ G/G' $. Finally, (c) follows immediately from Proposition 8.

### 7. THE JORDAN-HÖLDER THEOREM

#### Definition 9 {#alg-i-s4-def-9 .statement}

*A composition series of a group with operators G is a finite sequence $ (G_i)_{0 \leq i \leq n} $ of stable subgroups of G, with $ G_0 = G $ and $ G_n = \{e\} $ and such that $ G_{i+1} $ is a normal subgroup of $ G_i $ for $ 0 \leq i \leq n-1 $. The quotients $ G_i/G_{i+1} $ are called the quotients of the series. A composition series $ \Sigma' $ is said to be finer than a composition series $ \Sigma $ if $ \Sigma $ is a series taken from $ \Sigma' $.

If $ (G_i)_{0 \leq i \leq n} $ and $ (H_j)_{0 \leq j \leq m} $ are respectively composition series of two groups with operators G and H, they are said to be equivalent if $ m = n $ and there exists a permutation $ \phi $ of the interval $ \{0, n-1\} $ of $ \mathbf{N} $, such that the groups with operators $ G_i/G_{i+1} $ and $ H_{\phi(i)}/H_{\phi(i)+1} $ are isomorphic for all $ i $.

Note that in general a series taken from a composition series $ (G_i) $ is not a composition series, since for $ j > i + 1 $, $ G_j $ is not in general a normal subgroup of $ G_i $.

**Theorem 5 (Schreier).** *Given two composition series $ \Sigma_1, \Sigma_2 $ of a group with operators G, there exist two equivalent composition series $ \Sigma'_1, \Sigma'_2 $, finer respectively than $ \Sigma_1 $ and $ \Sigma_2 $.

Let $ \Sigma_1 = (H_i)_{0 \leq i \leq n} $ and $ \Sigma_2 = (K_j)_{0 \leq j \leq p} $ be the two given composition series with respectively $ n + 1 $ and $ p + 1 $ terms; we shall see that the composition series $ \Sigma'_1 $ can be formed by inserting $ p - 1 $ subgroups $ H'_{i,j} $ (1 \leq j \leq p - 1) between H_i and H_{i+1} for 0 \leq i \leq n - 1 and the series \Sigma_2' by inserting n - 1 subgroups K_{j,i}' (1 \leq i \leq n - 1) between K_j and K_{j+1} for 0 \leq j \leq p - 1; thus two series of pn + 1 stable subgroups of G will be obtained; by choosing suitably the inserted stable subgroups, we shall show that these series are equivalent composition series.

To this end note that H_i \cap K_j is a stable subgroup of H_i and of K_j, and hence (Theorem 4) H_{i+1}.(H_i \cap K_j) is a stable subgroup of H_i containing H_{i+1} and K_{j+1}.(H_i \cap K_j) is a stable subgroup of K_j containing K_{j+1}. If we write H_{i,j}' = H_{i+1}.(H_i \cap K_j) and K_{j,i}' = K_{j+1}.(H_i \cap K_j), H_{i,j+1}' is a stable subgroup of H_{i,j}' (0 \leq j \leq p - 1) and K_{j,i+1}' is a stable subgroup of K_{j,i}' (0 \leq i \leq n - 1). Moreover H_{i,0}' = H_i, H_{i,p}' = H_{i+1}, K_{j,0}' = K_j and K_{j,p}' = K_{j+1}. To show the theorem, it suffices to show that H_{i,j+1}' (resp. K_{j,i+1}') is a normal stable subgroup of H_{i,j}' (resp. K_{j,i}') and that the quotient groups H_{i,j}'/H_{i,j+1}' and K_{j,i}'/K_{j,i+1}' are isomorphic (0 \leq i \leq n - 1, 0 \leq j \leq p - 1). This follows from the following lemma by taking H = H_i, H' = H_{i+1}, K = K_j, K' = K_{j+1}.

Lemma 1 (Zassenhaus). Let H and K be two stable subgroups of a group with operators G and H' and K' normal stable subgroups of H and K respectively; then H'.(H \cap K') is a normal stable subgroup of H'.(H \cap K), K'.(K \cap H') is a normal stable subgroup of K'.(K \cap H) and the quotient groups with operators (H'.(H \cap K))/(H'.(H \cap K')) and (K'.(K \cap H))/(K'.(K \cap H')) are isomorphic.

By Theorem 4, H' \cap K = H' \cap (H \cap K) is a normal stable subgroup of H \cap K; similarly K' \cap H is a normal stable subgroup of K \cap H; hence (no. 6, Corollary 2) (H' \cap K)(K' \cap H) is a normal stable subgroup of H \cap K. By Theorem 4 applied to the group H,

$$
H'.(H' \cap K).(K' \cap H) = H'.(H \cap K')
$$

is a normal stable subgroup of H'.(H \cap K) and the quotient group

$$
(H'.(H \cap K))/(H'.(H \cap K))
$$

is isomorphic to

$$
(H \cap K)/((H' \cap K).(K' \cap H)).
$$

In the last quotient, H and H' on the one hand and K and K' on the other appear symmetrically; permuting them the stated result is obtained.

#### Definition 10 {#alg-i-s4-def-10 .statement}

A Jordan-Hölder series of a group with operators G is a strictly decreasing decomposition series \Sigma such that there exists no strictly decreasing decomposition series distinct from \Sigma and finer than \Sigma.

#### Proposition 9 {#alg-i-s4-prop-9 .statement}

For a decomposition series of G to be a Jordan-Hölder series it is necessary and sufficient that all the quotients of the series be simple.

A decomposition series is strictly decreasing if and only if none of its successive quotients is reduced to the identity element. If a strictly decreasing composition series $ \Sigma $ is not a Jordan-Hölder series, there exists a strictly decreasing composition series $ \Sigma' $ which is finer than $ \Sigma $ and distinct from $ \Sigma $. There are therefore two consecutive terms $ G_i, G_{i+1} $ of $ \Sigma $ which are not consecutive in $ \Sigma' $; let $ H $ be the first term which follows $ G_i $ in $ \Sigma' $; $ H $ is a normal stable subgroup of $ G_i $, containing $ G_{i+1} $ and distinct from the latter; hence $ H/G_{i+1} $ is a normal stable subgroup of $ G_i/G_{i+1} $, distinct from the latter and from the identity element; therefore $ G_i/G_{i+1} $ is not simple. Conversely, if $ \Sigma $ is a strictly decreasing composition series one of whose quotients $ G_i/G_{i+1} $ is not simple, this quotient contains a normal stable subgroup other than itself and $ \{e\} $, whose inverse image in $ G_i $ is a normal stable subgroup $ H $ of $ G_i $, distinct from $ G_i $ and $ G_{i+1} $ (Theorem 4); it suffices to insert $ H $ between $ G_i $ and $ G_{i+1} $ to obtain a strictly decreasing composition series distinct from $ \Sigma $ and finer than $ \Sigma $.

**Theorem 6 (Jordan-Hölder).** *Two Jordan-Hölder series of a group with operators are equivalent.*

Let $ \Sigma_1, \Sigma_2 $ be two Jordan-Hölder series of a group with operators $ G $; by applying Theorem 5 two *equivalent* composition series $ \Sigma'_1, \Sigma'_2 $ are obtained which are respectively finer than $ \Sigma_1 $ and $ \Sigma_2 $; since the latter are Jordan-Hölder series, $ \Sigma'_1 $ is identical with $ \Sigma_1 $ or is derived from it by repeating certain terms; the series of quotients of $ \Sigma'_1 $ is derived from that for $ \Sigma_1 $ by inserting a number of terms isomorphic to the group $ \{e\} $; since $ \Sigma_1 $ is strictly decreasing, the series of quotients of $ \Sigma_1 $ is derived from that of $ \Sigma'_1 $ by suppressing in the latter *all* the terms isomorphic to $ \{e\} $. Similarly for $ \Sigma_2 $ and $ \Sigma'_2 $. As the series of quotients of $ \Sigma'_1 $ and $ \Sigma'_2 $ differ (up to isomorphism) only in the order of the terms, the same is true of $ \Sigma_1 $ and $ \Sigma_2 $; the theorem is proved.

#### Corollary {#alg-i-s4-n7-cor-1 .statement}

*Let $ G $ be a group with operators in which there exists a Jordan-Hölder series. If $ \Sigma $ is any strictly decreasing composition series of $ G $, there exists a Jordan-Hölder series finer than $ \Sigma $.*

Let $ \Sigma_0 $ be a Jordan-Hölder series of $ G $; by Theorem 5, there exist two equivalent composition series, $ \Sigma' $ and $ \Sigma'_0 $ respectively finer than $ \Sigma $ and $ \Sigma_0 $; the argument of Theorem 6 shows that, by suppressing from $ \Sigma' $ the repetitions, a sequence $ \Sigma'' $ is obtained which is equivalent to $ \Sigma_0 $ and hence a Jordan-Hölder series, since all its quotients are simple (Proposition 9). As $ \Sigma $ is strictly decreasing, $ \Sigma'' $ is finer than $ \Sigma $, whence the corollary.

#### Remark {#alg-i-s4-n7-rem-1 .statement}

A group with operators does not always possess a Jordan-Hölder series; an example is given by the additive group $ \mathbf{Z} $ of rational integers: the sequence $ (2^n \cdot \mathbf{Z})_{n \geq 0} $ is a strictly decreasing infinite sequence of (normal) subgroups of $ \mathbf{Z} $; for all $ p $, the first $ p $ terms of this sequence form with the group $\{0\}$ a strictly decreasing composition series; if there existed a Jordan-Hölder series for $\mathbf{Z}$, it would have at least $p+1$ terms, by the Corollary to Theorem 6; absurd, since $p$ is arbitrary.

On the other hand, there exists a Jordan-Hölder series in every *finite* group with operators G: if $G \ne \{e\}$, among the normal stable subgroups of G distinct from G, let $H_1$ be a maximal subgroup; similarly define $H_{n+1}$ by induction as a maximal element in the set of normal subgroups of $H_n$, distinct from $H_n$, when $H_n \ne \{e\}$; the sequence of orders of the $H_n$ is strictly decreasing, hence there exists $n$ such that $H_n = \{e\}$ and the sequence consisting of G and the $H_i$ ($1 \leq i \leq n$) is by its formation a Jordan-Hölder series.

#### Definition 11 {#alg-i-s4-def-11 .statement}

Let G be a group with operators; the length of G is the upper bound of the integers $n$ such that there exists a strictly decreasing composition series of G $(G_i)_{0\leq i\leq n}$.

If G admits a Jordan-Hölder series, the length of G is the number of successive quotients of this series, as follows from the Corollary to Theorem 6. If G does not admit a Jordan-Hölder series, its length is infinite; by Proposition 9, for every strictly decreasing series of G there exists a strictly finer strictly decreasing series. The group consisting of the identity element is the only group with operators of length zero. A group with operators is simple if and only if it is of length 1.

Let G be a group with operators, H a normal stable subgroup of G, K the quotient G/H and $\pi:G\to K$ the canonical homomorphism. Let

$$
\Sigma'=(H_i)_{0\leq i\leq n}
$$

be a decomposition series of H and

$$
\Sigma''=(K_j)_{0\leq j\leq p}
$$

be a composition series of K. Writing $G_i=\pi^{-1}(K_i)$ for $0\leq i\leq p$ and $G_i=H_{i-p}$ for $p\leq i\leq n+p$, a composition series

$$
\Sigma=(G_i)_{0\leq i\leq n+p}
$$

of G is obtained. The sequence of quotients of $\Sigma$ is obtained by juxtaposing the sequence of quotients of $\Sigma''$ and the sequence of quotients of $\Sigma'$. If $\Sigma'$ and $\Sigma''$ are Jordan-Hölder series, $\Sigma$ is a Jordan-Hölder series of G, by Proposition 9. If H or K admits composition series of arbitrary length, so does G. We have proved:

#### Proposition 10 {#alg-i-s4-prop-10 .statement}

Let G be a group with operators and H a normal stable subgroup of G. The length of G is the sum of the lengths of H and G/H.

#### Corollary {#alg-i-s4-n7-cor-2 .statement}

Let G be a group with operators and $(G_i)_{0\leq i\leq n}$ a composition series of G. The length of G is the sum of the lengths of the $G_i/G_{i+1}$, $0\leq i\leq n-1$.

If G and $G'$ are isomorphic groups with operators and G admits a Jordan-Hölder series, so does $G'$ and the Jordan-Hölder series of G and $G'$ are equivalent. However, non-isomorphic groups can have equivalent Jordan-Hölder series; such is true for $\mathbf{Z}/4\mathbf{Z}$ and $(\mathbf{Z}/2\mathbf{Z})\times(\mathbf{Z}/2\mathbf{Z})$, cf. no. 10.

44

### 8. PRODUCTS AND FIBRE PRODUCTS

Let $(G_i)_{i \in I}$ be a family of groups with operators. Let $G$ be the product monoid of the $G_i$. Consider the action of $\Omega$ on $G$ defined by

$$
((x_i)_{i \in I})^\alpha = (x_i^\alpha)_{i \in I} \quad (\alpha \in \Omega, x_i \in G_i).
$$

With this structure $G$ is a group with operators. For all $i \in I$, the projection mapping $\mathrm{pr}_i : G \to G_i$ is a homomorphism of groups with operators.

#### Definition 12 {#alg-i-s4-def-12 .statement}

*The group with operators* $G = \prod_{i \in I} G_i$ *defined above is the product group with operators of the* $G_i$. *The mappings* $\mathrm{pr}_i : G \to G_i$ *are called the* projection homomorphisms.

A particular case of the product of groups with operators is the group $G^E$ consisting of the mappings of a set $E$ into a group with operators $G$, the laws being defined by:

$$
(fg)(x) = f(x)g(x) \quad (f, g \in G^E, x \in E)
$$
$$
f^\alpha(x) = f(x)^\alpha \quad (f \in G^E, \alpha \in \Omega, x \in E).
$$

Let $(\phi_i : H \to G_i)_{i \in I}$ be a family of homomorphisms of groups with operators. The mapping $h \mapsto (\phi_i(h))_{i \in I}$ of $H$ into $\prod_{i \in I} G_i$ is a homomorphism of groups with operators. It is the only homomorphism $\Phi : H \to \prod_{i \in I} G_i$ satisfying $\mathrm{pr}_i \circ \Phi = \phi_i$ for all $i$. This justifies the name "product group with operators" (*Set Theory*, IV, § 2, no. 4).

Let $(\phi_i : H_i \to G_i)_{i \in I}$ be a family of homomorphisms of groups with operators. The mapping $\prod_{i \in I} \phi_i : (h_i)_{i \in I} \mapsto (\phi_i(h_i))_{i \in I}$ of $\prod_{i \in I} H_i$ into $\prod_{i \in I} G_i$ is a homomorphism of groups with operators.

#### Proposition 11 {#alg-i-s4-prop-11 .statement}

*Let* $(\phi_i : H_i \to G_i)_{i \in I}$ *be a family of homomorphisms of groups with operators and let* $\Phi = \prod_{i \in I} \phi_i$. *Then:*

(a) $\mathrm{Ker}(\Phi) = \prod_{i \in I} \mathrm{Ker}(\phi_i)$; *in particular, if all the* $\phi_i$ *are injective, $\Phi$ *is injective*.

(b) $\mathrm{Im}(\Phi) = \prod_{i \in I} \mathrm{Im}(\phi_i)$; *in particular, if all the* $\phi_i$ *are surjective, $\Phi$ *is surjective*.

This is immediate.

In particular, let $(G_i)_{i \in I}$ be a family of groups with operators and, for all $i$, let $ H_i $ be a stable (resp. normal stable) subgroup of $ G_i $. The product $ \prod_{i \in I} H_i $ is a stable (resp. normal stable) subgroup of $ \prod_{i \in I} G_i $ and the canonical mapping of $ \prod_{i \in I} G_i $ onto $ \prod_{i \in I} (G_i / H_i) $ defines when passing to the quotient an isomorphism of
$$
\left( \prod_{i \in I} G_i \right) / \left( \prod_{i \in I} H_i \right)
$$
onto $ \prod_{i \in I} (G_i / H_i) $. For example, let $ J $ be a subset of $ I $. The subgroup $ G_J $ of $ \prod_{i \in I} G_i $ consisting of the $ (x_i)_{i \in I} $ such that $ x_i = e_i $ for $ i \notin J $ is a normal stable subgroup. The mapping $ \iota_J $ which associates with $ x = (x_j)_{j \in J} $ the element $ y = (y_i)_{i \in I} $ such that $ y_i = e_i $ for $ i \notin J $ and $ y_i = x_i $ for $ i \in J $, is an isomorphism of $ \prod_{j \in J} G_j $ onto $ G_J $. The mapping $ \mathrm{pr}_{I-J} $ defines when passing to the quotient an isomorphism $ \theta_J $ of the quotient group $ G / G_J $ onto $ \prod_{i \in I-J} G_i $. The composition $ \mathrm{pr}_J \circ \iota_J $ is the identity mapping of $ \prod_{j \in J} G_j $. $ G / G_J $ is often identified with $ \prod_{i \in I-J} G_i $ because of $ \theta_J $ and $ \prod_{i \in J} G_i $ with $ G_J $ because of $ \iota_J $.

If $ J_1 $ and $ J_2 $ are disjoint subsets of $ I $, it follows from the definitions that every element of $ G_{J_1} $ commutes with every element of $ G_{J_2} $.

#### Definition 13 {#alg-i-s4-def-13 .statement}

*Let $ G $ be a group with operators and $ (H_i)_{i \in I} $ a family of normal stable subgroups of $ G $. Let $ p_i : G \to G / H_i $ be the canonical homomorphism. $ G $ is called the internal product (or product) of the family of quotient groups $ (G / H_i) $ if the homomorphism $ g \mapsto (p_i(g))_{i \in I} $ is an isomorphism of $ G $ onto $ \prod_{i \in I} G / H_i $.*

Let $ G $ and $ H $ be groups with operators and let $ \phi $ and $ \psi $ be two homomorphisms of $ G $ into $ H $. The set of elements $ x $ in $ G $ such that $ \phi(x) = \psi(x) $ is a stable subgroup of $ G $, called the *coincidence group* of $ \phi $ and $ \psi $. In particular, let $ \phi_1 : G_1 \to H $ and $ \phi_2 : G_2 \to H $ be homomorphisms of groups with operators; the coincidence group of the homomorphisms $ \phi_1 \circ \mathrm{pr}_1 $ and $ \phi_2 \circ \mathrm{pr}_2 $ of $ G_1 \times G_2 $ into $ H $ is called the *fibre product* of $ G_1 $ and $ G_2 $ over $ H $ relative to $ \phi_1 $ and $ \phi_2 $. It is denoted by $ G_1 \times_H G_2 $ when there is no ambiguity about $ \phi_1 $ and $ \phi_2 $ and the restrictions $ p_1 $ and $ p_2 $ of $ \mathrm{pr}_1 $ and $ \mathrm{pr}_2 $ to $ G_1 \times_H G_2 $ are also called projection homomorphisms. Then $ \phi_1 \circ p_1 = \phi_2 \circ p_2 $. The elements of $ G_1 \times_H G_2 $ are the ordered pairs $ (g_1, g_2) \in G_1 \times G_2 $ such that $ \phi_1(g_1) = \phi_2(g_2) $. If $ f_i $ is a homomorphism of a group with operators $ K $ into $ G_i $ ($ i = 1, 2 $) and $ \phi_1 \circ f_1 = \phi_2 \circ f_2 $, there exist one and only one homomorphism $ f $ of $ K $ into $ G_1 \times_H G_2 $ such that $ f_i = p_i \circ f $ for $ i = 1, 2 $.

### 9. RESTRICTED SUMS

Let $(G_i)_{i \in I}$ be a family of groups with operators and, for $i \in I$, let $H_i$ be a stable subgroup of $G_i$. The subset of $\prod_{i \in I} G_i$ consisting of the $(x_i)_{i \in I}$ such that the set of $i \in I$ with $x_i \notin H_i$ is finite is a stable subgroup of $\prod_{i \in I} G_i$ equal to $\prod_{i \in I} G_i$ if $I$ is finite. It is called the *restricted sum of the $G_i$ with respect to the $H_i$*. When, for all $i$ except for a finite number, $H_i$ is a normal stable subgroup of $G_i$, the restricted sum is a normal stable subgroup of the product. When, for all $i$, the subgroup $H_i$ is reduced to the identity element of $G_i$, the direct sum of the $G_i$ with respect to the $H_i$ is called simply the *restricted sum of the $G_i$* and is sometimes denoted by $\prod_{i \in I} G_i$. For all $i_0 \in I$, the mapping $\iota_{i_0}: G_{i_0} \to \prod_{i \in I} G_i$ defined by $\iota_{i_0}(x) = (x_i)_{i \in I}$, where $x_{i_0} = x$ and $x_i = e_i$ if $i \neq i_0$, is an injective homomorphism of groups with operators called the *canonical injection*. $G_i$ is identified with the stable subgroup $\operatorname{Im}(\iota_i)$. The subgroups $G_i$ are normal. For $i \neq j$, the elements of $G_i$ and $G_j$ commute and $G_i \cap G_j = \{e\}$. The group $\prod_{i \in I} G_i$ is generated by the set $\bigcup_{i \in I} G_i$.

#### Proposition 12 {#alg-i-s4-prop-12 .statement}

*Let $(\phi_i: G_i \to K)_{i \in I}$ be a family of homomorphisms of groups with operators such that, for all $i \in I$ and $j \in I$ with $i \neq j$, $x \in G_i$, $y \in G_j$, the elements $\phi_i(x)$ and $\phi_j(y)$ of $K$ commute; there exists one and only one homomorphism of groups with operators $\Phi$ of $\prod_{i \in I} G_i$ into $K$ such that $\phi_i = \Phi \circ \iota_i$ for all $i \in I$. For every element $x = (x_i)_{i \in I}$ of $\prod_{i \in I} G_i$, $\Phi(x) = \prod_{i \in I} \phi_i(x_i)$.*

If $\Phi$ and $\Phi$ are solutions to the problem, they coincide on $\bigcup_{i \in I} G_i$ and hence on $\prod_{i \in I} G_i$, whence the uniqueness of $\Phi$. We now show the existence of $\Phi$: for every element $x = (x_i)_{i \in I}$ of $\prod_{i \in I} G_i$, let $\Phi(x) = \prod_{i \in I} \phi_i(x_i)$ (\S 1, no. 5). Clearly $\Phi \circ \iota_i = \phi_i$ for all $i$ and $\Phi$ commutes with homotheties; the formula $\Phi(xy) = \Phi(x)\Phi(y)$ follows from \S 1, no. 5, formula (9).

#### Definition 14 {#alg-i-s4-def-14 .statement}

*Let $G$ be a group with operators and $(H_i)_{i \in I}$ a family of stable subgroups of $G$. $G$ is called the internal restricted sum (or restricted sum) of the family of subgroups $(H_i)$ if every element of $H_i$ is permutable with every element of $H_j$ for $j \neq i$ and the unique homomorphism of $\prod_{i \in I} H_i$ into $G$ whose restriction to each of the $H_i$ is the canonical injection is an isomorphism.*

When $I$ is finite, we also say, by an abuse of language, *internal direct product* (or *direct product*, or *product*) instead of internal restricted sum. Every stable subgroup H of G for which there exists a stable subgroup H' of G such that G is the direct product of H and H' is called a *direct factor* of G.

#### Proposition 13 {#alg-i-s4-prop-13 .statement}

*Let G be a group with operators and $(H_i)_{i \in I}$ a family of stable subgroups of G such that every element of $H_i$ is permutable with every element of $H_j$ for $j \neq i$. For G to be the restricted sum of the family of subgroups $(H_i)_{i \in I}$, it is necessary and sufficient that every element x of G be expressible uniquely in the form $\prod_{i \in I} y_i$, where $(y_i)_{i \in I}$ is a family with finite support of elements of G with $y_i \in H_i$ for all i.*

Obvious.

#### Proposition 14 {#alg-i-s4-prop-14 .statement}

*Let G be a group with operators and $(H_i)_{i \in I}$ a finite family of stable subgroups of G. For G to be the restricted sum of the family of subgroups $(H_i)$, it is necessary and sufficient that each $H_i$ be normal and that G be the product of the quotient groups $(G/H^i)$, where $H^i$ is the subgroup generated by the $H_j$ for $j \neq i$.*

The condition is obviously necessary. Conversely, suppose G is the product of the $K_i = G/H^i$ and let G be identified with the product of the $K_i$. Then $H_i$ is identified with a subgroup of $K_i$, so that, for $i \neq j$, every element of $H_i$ is permutable with every element of $H_j$; on the other hand, $H^i$ is identified with the product of the $K_j$ for $j \neq i$, hence $H_i = K_i$ for all $i$ and G is the direct product of the $H_i$.

#### Proposition 15 {#alg-i-s4-prop-15 .statement}

*Let G be a group with operators and $(H_i)_{1 \leq i \leq n}$ a sequence of normal stable subgroups of G such that*
$$
(H_1 H_2 \ldots H_i) \cap H_{i+1} = \{e\} \quad \text{for } 1 \leq i \leq n-1,
$$
*the set $H_1 H_2 \ldots H_n$ is a normal stable subgroup of G, the restricted sum of the $H_i$.*

By induction on $n$, this is immediately reduced to proving the proposition for $n = 2$. We show first that, if $x \in H_1$ and $y \in H_2$, x and y are *permutable*; for $xyx^{-1}y^{-1} = (xyx^{-1})y^{-1} = x(yx^{-1}y^{-1})$ and hence (since $H_1$ and $H_2$ are normal) $xyx^{-1}y^{-1} \in H_1 \cap H_2$, that is $xyx^{-1}y^{-1} = e$, by the hypothesis. Moreover $H_1 H_2$ is a subset of G which is stable under the homotheties of G. It follows (by no. 3, Proposition 1) that $H_1 H_2$ is a stable subgroup of G and it is immediately verified that this subgroup is normal. Suppose finally that $xy = x'y'$, with $x \in H_1, x' \in H_1, y \in H_2, y' \in H_2$; then $x'^{-1}x = y'y^{-1}$, hence $x'^{-1} \in H_1 \cap H_2 = \{e\}$, $x' = x$ and similarly $y' = y$; $H_1 H_2$ is thus the direct product of $H_1$ and $H_2$.

When the group considered are commutative, the term *direct sum* is used instead of direct product.

### 10. MONOGENOUS GROUPS

Let $a \in \mathbf{Z}$; since $a\mathbf{Z}$ is a subgroup of $\mathbf{Z}$, the relation between elements $x, y$ of $\mathbf{Z}$ which states "there exists $z \in \mathbf{Z}$ such that $x - y = az$" is an equivalence relation, which we agree, once and for all, to write as $ x \equiv y \pmod{a} $ or $ x \equiv y(a) $ and which is called *congruence modulo* $ a $. Replacing $ a $ by $ -a $ an equivalent relation is obtained, hence it may be supposed that $ a \geqslant 0 $; for $ a = 0 $, $ x \equiv y(0) $ means $ x = y $, hence a relation distinct from equality is obtained only if $ a \neq 0 $: we shall therefore suppose in what follows that $ a > 0 $ unless otherwise indicated.

For $ a > 0 $, the quotient of $ \mathbf{Z} $ by the congruence $ x \equiv y(a) $, that is the group $ \mathbf{Z}/a\mathbf{Z} $, is called the *group of rational integers modulo* $ a $.

#### Proposition 16 {#alg-i-s4-prop-16 .statement}

*Let $ a $ be an integer $ > 0 $. The integers $ r $ such that $ 0 \leqslant r < a $ form a system of representatives of the equivalence relation $ x \equiv y \pmod{a} $ on $ \mathbf{Z} $.*

If $ x $ is an integer $ \geqslant 0 $, there exist (*Set Theory*, III, § 5, no. 6) integers $ q $ and $ r $ such that $ x = aq + r $ and $ 0 \leqslant r < a $ and $ x \equiv r \pmod{a} $. If $ x $ is an integer $ \leqslant 0 $, the integer $ -x $ is $ \geqslant 0 $ and by the above there exists an integer $ r $ such that $ 0 \leqslant r < a $ and $ -x \equiv r \pmod{a} $. Writing $ r' = 0 $ if $ r = 0 $ and $ r' = a - r $ if $ r > 0 $, then

$$
x \equiv -r \equiv r' \pmod{a}
$$

and $ 0 \leqslant r' < a $. We now show that if $ 0 \leqslant r < r' < a $, then $ r \not\equiv r' \pmod{a} $. Now $ r' - r < na $ for $ n \geqslant 1 $ and $ r' - r > na $ for $ n \leqslant 0 $, whence $ r' - r \notin a\mathbf{Z} $.

#### Corollary {#alg-i-s4-n10-cor-1 .statement}

*Let $ a $ be an integer $ > 0 $. The group $ \mathbf{Z}/a\mathbf{Z} $ of rational integers modulo $ a $ is a group of order $ a $.*

#### Proposition 17 {#alg-i-s4-prop-17 .statement}

*Let $ \mathrm{H} $ be a subgroup of $ \mathbf{Z} $. There exists one and only one integer $ a \geqslant 0 $ such that $ \mathrm{H} = a\mathbf{Z} $.*

If $ \mathrm{H} = \{0\} $, then $ \mathrm{H} = 0\mathbf{Z} $. Suppose that $ \mathrm{H} \neq \{0\} $. The subgroup $ \mathrm{H} $ has an element $ x \neq 0 $. Then $ x > 0 $ or $ -x > 0 $, and therefore $ \mathrm{H} $ has elements $ > 0 $. Let $ a $ be the smallest element $ > 0 $ in $ \mathrm{H} $. The subgroup $ a\mathbf{Z} $ generated by $ a $ is contained in $ \mathrm{H} $; we show that $ \mathrm{H} \subset a\mathbf{Z} $. Let $ y \in \mathrm{H} $. By Proposition 16, there exists an integer $ r $ such that $ y \equiv r \pmod{a} $ and $ 0 \leqslant r < a $. *A fortiori* $ y \equiv r \pmod{\mathrm{H}} $, whence $ r \in \mathrm{H} $. But this is only possible if $ r = 0 $ and therefore $ y \in a\mathbf{Z} $. The integer $ a $ is unique: if $ \mathrm{H} = \{0\} $, then necessarily $ a = 0 $, and if $ \mathrm{H} \neq \{0\} $, the integer $ a $ is the order of $ \mathbf{Z}/\mathrm{H} $.

#### Definition 15 {#alg-i-s4-def-15 .statement}

*A group is called monogenous if it admits a system of generators consisting of a single element. A finite monogenous group is called cyclic.*

Every monogenous group is commutative (no. 3, Corollary 2 to Proposition 2). Every quotient group of a monogenous group is monogenous (no. 3, Corollary 3 to Proposition 2).

The additive group $ \mathbf{Z} $ is monogenous: it is generated by $ \{1\} $. For every positive integer $ a $, the group $ \mathbf{Z}/a\mathbf{Z} $ is monogenous, for it is a quotient of $ \mathbf{Z} $.

#### Proposition 18 {#alg-i-s4-prop-18 .statement}

*A finite monogenous group of order a is isomorphic to $ \mathbf{Z}/a\mathbf{Z} $. An infinite monogenous group is isomorphic to $ \mathbf{Z} $.*

Let G be a monogenous group (written multiplicatively) and x a generator of G. The identity $ x^m x^n = x^{m+n} $ (\S 1, no. 3, formula (1)) shows that the mapping $ n \mapsto x^n $ is a homomorphism of $ \mathbf{Z} $ into G. Its image is a subgroup of G containing x and hence it is G. By no. 5, Theorem 3, the group G is isomorphic to the quotient of $ \mathbf{Z} $ by a subgroup, which is necessarily of the form $ a\mathbf{Z} $ (Proposition 17). If $ a > 0 $, the group G is finite of order a and if $ a = 0 $, the group G is isomorphic to $ \mathbf{Z} $.

#### Proposition 19 {#alg-i-s4-prop-19 .statement}

*Let a be an integer > 0. Let H be a subgroup of $ \mathbf{Z}/a\mathbf{Z} $, b the order of H and c its index in $ \mathbf{Z}/a\mathbf{Z} $. Then $ a = bc $, $ H = c\mathbf{Z}/a\mathbf{Z} $ and H is isomorphic to $ \mathbf{Z}/b\mathbf{Z} $.

Conversely, let b and c be two integers > 0 such that $ a = bc $. Then $ a\mathbf{Z} \subset c\mathbf{Z} $ and $ c\mathbf{Z}/a\mathbf{Z} $ is a subgroup of $ \mathbf{Z}/a\mathbf{Z} $, of order b and index c.

$ a = bc $ by no. 4, Corollary to Proposition 4. By no. 7, Theorem 4, H is of the form $ H'/a\mathbf{Z} $, where $ H' $ is a subgroup of $ \mathbf{Z} $ and $ \mathbf{Z}/H' $ is isomorphic to $ (\mathbf{Z}/a\mathbf{Z})/H $ and hence of order c. By Proposition 17 and the Corollary to Proposition 16, $ H' = c\mathbf{Z} $ and hence H is monogenous. Finally, H is isomorphic to $ \mathbf{Z}/b\mathbf{Z} $ by Proposition 18. Conversely, if $ a = bc $, then $ a\mathbf{Z} \subset c\mathbf{Z} $ for $ a \in c\mathbf{Z} $: the quotient group $ (\mathbf{Z}/a\mathbf{Z})/(c\mathbf{Z}/a\mathbf{Z}) $ is isomorphic to $ \mathbf{Z}/c\mathbf{Z} $ (no. 7, Theorem 4) and hence of order c (no. 4, Corollary to Proposition 4) and index b (no. 4, Corollary to Proposition 4).

#### Corollary {#alg-i-s4-n10-cor-2 .statement}

*Every subgroup of a monogenous group is monogenous.*

Let a and b be two integers $ \neq 0 $. The relation $ b \in a\mathbf{Z} $ is also written: *b is a multiple of a*, and also *a divides b* or *a is a divisor of b*.

#### Definition 16 {#alg-i-s4-def-16 .statement}

*An integer $ p > 0 $ is called prime if $ p \neq 1 $ and it admits no divisor > 1 other than p.*

#### Proposition 20 {#alg-i-s4-prop-20 .statement}

*An integer $ p > 0 $ is prime if and only if the group $ \mathbf{Z}/p\mathbf{Z} $ is a simple group.*

This follows from Proposition 19.

#### Corollary {#alg-i-s4-n10-cor-3 .statement}

*Every commutative simple group is cyclic of prime order.*

Let G be such a group. Then $ G \neq \{e\} $; let $ a \neq e $ be an element of G. The subgroup generated by a is normal since G is commutative, it is not reduced to $ \{e\} $ and hence is equal to G. Therefore G is monogenous and hence isomorphic to a group of the form $ \mathbf{Z}/p\mathbf{Z} $ with $ p > 0 $, since $ \mathbf{Z} $ is not simple, and $ p $ is necessarily prime.

#### Remark {#alg-i-s4-n10-rem-1 .statement}

A finite group G of prime order is necessarily cyclic. G admits no subgroup other than G and $ \{e\} $ and hence it is generated by every element $ \neq e $.

#### Lemma 2 {#alg-i-s4-lem-2 .statement}

Let $ a $ be an integer $ > 0 $. By associating with every composition series $ (\mathbf{H}_i)_{0 \leq i \leq n} $ of the group $ \mathbf{Z}/a\mathbf{Z} $ the sequence $ (s_i)_{1 \leq i \leq n} $, where $ s_i $ is the order of $ \mathbf{H}_{i-1}/\mathbf{H}_i $, a one-to-one correspondence is obtained between the composition series of $ \mathbf{Z}/a\mathbf{Z} $ and the finite sequences $ (s_i) $ of integers $ > 0 $ such that $ a = s_1 \ldots s_n $. The composition series $ (\mathbf{H}_i)_{0 \leq i \leq n} $ is a Jordan-Hölder series if and only if the $ s_i $ are prime.

If $ (\mathbf{H}_i)_{0 \leq i \leq n} $ is a composition series of $ \mathbf{Z}/a\mathbf{Z} $, it follows, by induction on $ n $, from no. 4, Proposition 4, that $ a = \prod_{i=1}^n (\mathbf{H}_{i-1} : \mathbf{H}_i) $.

Conversely, let $ (s_i)_{1 \leq i \leq n} $ be a sequence of integers $ > 0 $ such that $ a = s_1 \ldots s_n $. If $ (\mathbf{H}_i)_{0 \leq i \leq n} $ is a composition series of $ \mathbf{Z}/a\mathbf{Z} $ such that $ (\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i $ for $ 1 \leq i \leq n $, then necessarily $ ((\mathbf{Z}/a\mathbf{Z}) : \mathbf{H}_i) = \prod_{1 \leq j \leq i} s_j $ as is seen by induction on $ i $, whence $ \mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z} $ (Proposition 19), which shows the injectivity of the mapping in question. We now show its surjectivity. Writing $ \mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z} $ for $ 0 \leq i \leq n $, a composition series of $ \mathbf{Z}/a\mathbf{Z} $ is obtained such that $ (\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i $ (Proposition 19). The second assertion follows from Proposition 20 and no. 7, Proposition 9.

Let $ \mathfrak{P} $ denote the set of prime numbers.

#### Theorem 7 (decomposition into prime factors) {#alg-i-s4-thm-7 .statement}

*Let $ a $ be a strictly positive integer. There exists one and only one family $ (v_p(a))_{p \in \mathfrak{P}} $ of integers $ > 0 $ such that the set of $ p \in \mathfrak{P} $ with $ v_p(a) \neq 0 $ is finite and*

$$
a = \prod_{p \in \mathfrak{P}} p^{v_p(a)}.
$$

As the group $ \mathbf{Z}/a\mathbf{Z} $ is finite, it admits a Jordan-Hölder series. Lemma 2 then implies that $ a $ is a product of prime integers, whence the existence of the family $ (v_p(a)) $; further, for every family $ (v_p(a))_{p \in \mathfrak{P}} $ satisfying the conditions of Theorem 7, the integer $ v_p(a) $ is, for all $ p \in \mathfrak{P} $, equal to the number of factors of a Jordan-Hölder series of $ \mathbf{Z}/a\mathbf{Z} $ isomorphic to $ \mathbf{Z}/p\mathbf{Z} $ (Lemma 2). The uniqueness of the family $ (v_p(a)) $ therefore follows from the Jordan-Hölder theorem (no. 7, Theorem 6).

#### Corollary {#alg-i-s4-n10-cor-4 .statement}

*Let $ a $ and $ b $ be two integers $ > 0 $. Then $ v_p(ab) = v_p(a) + v_p(b) $. For $ a $ to divide $ b $, it is necessary and sufficient that $ v_p(a) \leq v_p(b) $ for every prime number $ p $.*

In any group $ G $, if the (monogenous) subgroup generated by an element $ x \in G $ is of finite order $ d $, $ x $ is called an element of *order* $ d $; the number $ d $ is therefore the least integer $ > 0 $ such that $ x^d = e $; if the subgroup generated by $ x $ is infinite, $ x $ is said to be of *infinite order*. These definitions, together with Proposition 4 (no. 4), imply in particular that in a finite group G the order of every element of G is a divisor of the order of G.

#### Proposition 21 {#alg-i-s4-prop-21 .statement}

In a finite group G of order n, $ x^n = e $ for all $ x \in G $.

If $ p $ is the order of $ x $, then $ n = pq $, with $ q $ an integer, and hence $ x^n = (x^p)^q = e $.

### Exercises {#alg-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
