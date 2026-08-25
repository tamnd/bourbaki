---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 2
section_title: Subgroups, quotient groups, homomorphisms homogeneous spaces, product groups
lang: en
source: top-i-iv
pdf_pages: 0231-0248, 0304-0311
extraction: ocr
subsections:
    - "no": 1
      title: SUBGROUPS OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 231
    - "no": 2
      title: COMPONENTS OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 233
    - "no": 3
      title: DENSE SUBGROUPS
      page: 0
      pdf_page: 234
    - "no": 4
      title: SPACES WITH OPERATORS
      page: 0
      pdf_page: 234
    - "no": 5
      title: HOMOGENEOUS SPACES
      page: 0
      pdf_page: 237
    - "no": 6
      title: QUOTIENT GROUPS
      page: 0
      pdf_page: 238
    - "no": 7
      title: SUBGROUPS AND QUOTIENT GROUPS OF A QUOTIENT GROUP
      page: 0
      pdf_page: 239
    - "no": 8
      title: CONTINUOUS HOMOMORPHISMS AND STRICT MORPHISMS
      page: 0
      pdf_page: 241
    - "no": 9
      title: PRODUCTS OF TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 243
    - "no": 10
      title: SEMI-DIRECT PRODUCTS
      page: 0
      pdf_page: 245
statements: 45
exercises: 31
content_sha256: d048e3e902c53078e76ce604d90a76e6a56ed1642651f4bb530f314542961a5e
---

## 2. SUBGROUPS, QUOTIENT GROUPS, HOMOMORPHISMS, HOMOGENEOUS SPACES, PRODUCT GROUPS

### 1. SUBGROUPS OF A TOPOLOGICAL GROUP

Let G be a topological group and let H be a subgroup of G. By (GT'), the topology induced on H by the topology of G is compatible with the group structure of H. The structure of a topological group thus defined on $H$ is said to be *induced* by that of $G$. Whenever we consider a subgroup $H$ of $G$ as a topological group, it is always this induced structure which is under consideration, unless the contrary is expressly stated.

#### Proposition 1 {#top-iii-s2-prop-1 .statement}

*The closure $\overline{H}$ of a subgroup $H$ of a topological group $G$ is a subgroup of $G$. If $H$ is a normal subgroup of $G$, then so is $\overline{H}$.*

If $a, b \in \overline{H}$ then $ab^{-1} \in \overline{H}$, because the mapping $(x, y) \to xy^{-1}$ is continuous on $G \times G$ and transforms $H \times H$ into $H$ (Chapter I, § 2, no. 1, Theorem 1). In the same way, the continuity of the mapping $x \to axa^{-1}$ shows that if $H$ is normal then $\overline{H}$ is normal.

In particular, the closure $N$ of the set $\{ e \}$ consisting only of the identity element of $G$, is a *normal subgroup* of $G$; and $N = \{ e \}$ if and only if $G$ is *Hausdorff* ($\S$ 1, no. 2, Proposition 2).

#### Proposition 2 {#top-iii-s2-prop-2 .statement}

*If $G$ is a Hausdorff topological group, then the closure of a commutative subgroup of $G$ is a commutative subgroup of $G$.*

By reason of Proposition 1, we may limit ourselves to the case where $H$ is dense in $G$. The continuous functions $xy$ and $yx$ are equal on $H \times H$, and are therefore equal on $G \times G$, by virtue of the principle of extension of identities (Chapter I, § 8, no. 1, Proposition 2, Corollary 1).

#### Proposition 3 {#top-iii-s2-prop-3 .statement}

*Let $G$ be a Hausdorff topological group and let $M$ be any subset of $G$. Then the set $M'$ of elements of $G$ which commute with each element of $M$ is a closed subgroup of $G$. In particular, the centre of $G$ is closed in $G$.*

For $M'$ is the intersection of the sets $F_m (m \in M)$, where $F_m$ is the set of all $x \in G$ such that $xm = mx$; and $F_m$ is closed (Chapter I, § 8, no. 1, Proposition 2).

#### Proposition 4 {#top-iii-s2-prop-4 .statement}

*Let $G$ be a topological group and let $H$ be a subgroup of $G$ which is locally closed at one point of $H$ (Chapter I, § 3, no. 3, Definition 2). Then $H$ is closed in $G$.*

By translation, $H$ is locally closed at each of its points, i.e. $H$ is locally closed in $G$. Let $V$ be a symmetric open neighbourhood of $e$ in $G$ such that $V \cap H$ is closed in $V$. If $x \in \overline{H}$, then $xV$ meets $H$; if $y \in xV \cap H$, we have $x \in yV$, and $y(V \cap H) = (yV) \cap H$ is closed in $yV$. But $x$ lies in the closure of $(yV) \cap H$, hence $x \in H$.

#### Corollary {#top-iii-s2-n1-cor-1 .statement}

*A subgroup of a topological group is open if and only if it has an interior point. Every open subgroup is closed.*

If a subgroup $H$ has an interior point, then by translation all the points of $H$ are interior and so $H$ is open. The second assertion of the corollary is a particular case of Proposition 4.

#### Proposition 5 {#top-iii-s2-prop-5 .statement}

*A subgroup $H$ of a topological group $G$ is discrete if and only if $H$ has an isolated point. Every discrete subgroup of a Hausdorff group is closed.*

If $H$ is discrete, every point of $H$ is isolated. Conversely if $H$ has an isolated point, then by translation every point of $H$ is isolated and therefore $H$ is discrete. If $H$ is discrete and $G$ is Hausdorff, then there is a neighbourhood $V$ of $e$ such that $V \cap H = \{e\}$; $\{e\}$ is closed in $G$ and therefore *a fortiori* in $V$, so that $H$ is locally closed at $e$. Hence $H$ is closed in $G$ by Proposition 4.

#### Remark {#top-iii-s2-n1-rem-1 .statement}

Let $H$ be any subgroup of a topological group $G$. For each $x \in \overline{H}$ we have $x \overline{H} = x$. $\overline{H} = \overline{H}$, since translation by $x$ is a homeomorphism of $G$ onto $G$. In other words, for each $x \in \overline{H}$, $xH$ is *dense* in $\overline{H}$. It follows that if $H$ is not closed, then $\overline{H} \cap CH$ is *dense* in $\overline{H}$.

### 2. COMPONENTS OF A TOPOLOGICAL GROUP

Let $V$ be a *symmetric* neighbourhood of $e$ in $G$. The subgroup generated by $V$, which is denoted by $V^\infty$ consists of all products $\prod_{i=1}^n x_i$ of finite sequences of elements of $V$. $V^\infty$ is *open*, since it has $e$ as an interior point, and is therefore *closed* by Proposition 4 of no. 1. It follows that:

#### Proposition 6 {#top-iii-s2-prop-6 .statement}

*A connected topological group is generated by every neighbourhood of the identity element.*

The converse of this proposition is in general false, as we shall see in Chapter IV (\$ 2, no. 5). If a topological group $G$ is generated by each neighbourhood of the identity element, the most we can say is that $G$ contains *no open subgroup* other than $G$.

\* As an example of a non-connected group $G$ which has an open subgroup distinct from $G$, we may cite the *multiplicative group* $\mathbf{R}^*$ of non-zero real numbers, in which the subgroup $\mathbf{R}_+^*$ of real numbers $> 0$ is both open and closed (see Chapter IV, \$ 3, no. 2). \*

#### Proposition 7 {#top-iii-s2-prop-7 .statement}

*In a topological group $G$, the component $K$ of the identity element $e$ is a closed normal subgroup. The component of any point $x \in G$ is the coset $x.K = K.x$.*

The component of the identity element $e$ of $G$ is called the *identity component* of $G$.

### 3. DENSE SUBGROUPS

The following Proposition generalizes Proposition 1 of no. 1:

#### Proposition 8 {#top-iii-s2-prop-8 .statement}

*Let $H$ be a dense subgroup of a topological group $G$, and let $K$ be a normal subgroup of $H$. Then the closure $\overline{K}$ of $K$ in $G$ is a normal subgroup of $G$.*

For the mapping $(z, x) \to zxz^{-1}$ is continuous on $G \times G$, and maps $H \times K$ into $K$; hence (Chapter I, § 2, no. 1, Theorem 1) it maps $G \times \overline{K} = \overline{H} \times K$ into $\overline{K}$.

#### Proposition 9 {#top-iii-s2-prop-9 .statement}

*Let $H$ be a dense subgroup of a topological group $G$. If $H$ is generated by every neighbourhood of the identity element in $H$, then $G$ is generated by every neighbourhood of the identity element in $G$.*

Let $V$ be any symmetric neighbourhood of $e$ in $G$. Then $V \cap H$ is a neighbourhood of $e$ in $H$, and hence generates $H$. It follows that $V$ generates a subgroup $H'$ which contains $H$; but $H'$ is open and closed (no. 1, Corollary to Proposition 4), and therefore contains $\overline{H} = G$.

### 4. SPACES WITH OPERATORS

Let $X$ be a topological space and let $G$ be a topological group. $G$ is said to *operate continuously* on $X$ if the following conditions are satisfied:

1) $X$ has $G$ as a group of operators; in other words $X$ is endowed with an external law of composition $(s, x) \to s.x$ for which $G$ is the set of operators, and which is such that $s.(t.x) = (st).x$ and $e.x = x$ for all $s, t \in G$ and all $x \in X$.

2) The mapping $(s, x) \to s.x$ of $G \times X$ into $X$ is *continuous*.

#### Lemma 1 {#top-iii-s2-lem-1 .statement}

*If a topological group* $G$ *operates continuously on a topological space* $X$, *then for each* $s \in G$ *the mapping* $x \to s.x$ *is a homeomorphism of* $X$ *onto* $X$.

For this mapping is a continuous bijection whose inverse $x \to s^{-1}.x$ is also continuous.

We recall that for each $x \in X$ the set $G.x$ of transforms $s.x$ of $x$ by the elements $s$ of $G$ is called the *orbit* of $x$ (with respect to the group of operators $G$), and that the set of all $s \in G$ such that $s.x = x$ is a subgroup of $G$ called the *stabilizer* of $x$. The relation $R(x, y) : "y$ belongs to the orbit of $x"$ is an equivalence relation on $X$, called the equivalence relation *defined by* $G$; the equivalence classes with respect to this relation are the orbits of the points of $X$. The topological space $X/R$ is called the *orbit space* of $X$ (with respect to $G$), or the *quotient space of* $X$ *by the group* $G$, and is denoted by $X/G$; and the topology of $X/G$ is said to be the *quotient of the topology of* $X$ *by* $G$.

#### Lemma 2 {#top-iii-s2-lem-2 .statement}

*If a topological group* $G$ *operates continuously on a topological space* $X$, *then the equivalence relation* $R$ *defined by* $G$ *is open*.

For the saturation with respect to $R$ of an open subset $U$ of $X$ is the set $\bigcup_{s \in G} s.U$, and each $s.U$ is open by Lemma 1.

#### Example 1 {#top-iii-s2-n4-exa-1 .statement}

Let $H$ be a subgroup of a topological group $G$. $H$ operates continuously on $G$ by the external law $(s, x) \to sx$. $H$ also operates continuously on $G$ by the external law $(x, s) \to sxs^{-1}$.

#### Example 2 {#top-iii-s2-n4-exa-2 .statement}

\* If $K$ is a topological division ring ($\S 6$, no. 7), the multiplicative group $K^*$ operates continuously on $K$ by the external law $(s, x) \to sx$. \*

#### Example 3 {#top-iii-s2-n4-exa-3 .statement}

Let $G$ be a topological group, $X$ a topological space. Then the mapping $(s, x) \to x$ of $G \times X$ into $X$ is an external law of composition on $X$, and $G$ operates continuously on $X$ with respect to this law; $G$ is then said to operate *trivially* on $X$.

#### Remark {#top-iii-s2-n4-rem-1 .statement}

Instead of saying that a topological group $G$ operates continuously on a topological space $X$, it is often said that $G$ operates continuously *on the left* on $X$. When the topological group $G^0$ opposite to $G$ operates continuously on $X$, we say that $G$ operates continuously *on the right* on $X$. It comes to the same thing to say that $X$ has a continuous external law of composition $(s, x) \to s.x$ with $G$ as set of operators, such that $s.(t.x) = (ts).x$ and $e.x = x$. Such a law is often written *on the right* : $(s, x) \to x.s$ (whence the terminology), and we have then $(x.t).s = x.(ts)$. If $G$ operates continuously on the right on $X$ by the law $(s, x) \to x.s$, then also $G$ operates continuously on the left on $X$ according to the external law $(s, x) \to x.s^{-1}$, by virtue of axiom (GT$_{II}$).

Let $G$ be a topological group operating continuously on a topological space $X$, and let $\varphi$ be the canonical mapping of $X$ onto the orbit space $X/G$. Let $A$ be any subset of $X$, and let $A'$ be the subspace of $X$ which is the saturation of $A$ with respect to the equivalence relation $R$ defined by $G$ (thus $A'$ is the union of the orbits of points of $A$, and is said to be the *saturation of $A$ with respect to $G$*). $G$ operates continuously on $A'$ by the restriction of $(s, x) \to s.x$ to $G \times A'$. Moreover, since $R$ is open (Lemma 2) and $A'$ is saturated, it follows from Proposition 4 of Chapter I, § 5, no. 2, and from the relation $\varphi(A) = \varphi(A')$, that:

#### Proposition 10 {#top-iii-s2-prop-10 .statement}

*The canonical bijection of the subspace $\varphi(A)$ of $X/G$ onto the orbit space $A'/G$ is a homeomorphism.*

Now let $S$ be an equivalence relation on $X$ such that, for each $s \in G$, the mapping $x \to s.x$ is *compatible* with $S$ [in other words, such that the relation $x \equiv y \pmod{S}$ implies $s.x \equiv s.y \pmod{S}$]; for the sake of brevity we shall say that the relation $S$ is *compatible with the group* $G$. If $\psi$ is the canonical mapping of $X$ onto $X/S$, and if $s.\psi(x)$ denotes the class mod $S$ of $s.x$, then $X/S$ has $G$ as groups of operators with respect to the external law $(s, \psi(x)) \to s.\psi(x) = \psi(s.x)$. Moreover:

#### Proposition 11 {#top-iii-s2-prop-11 .statement}

*If the equivalence relation $S$ on $X$ is open and compatible with $G$, then $G$ operates continuously on $X/S$.*

Since the relation of equality on $G$ and the relation $S$ on $X$ are open, it is enough to show that the mapping $(s, x) \to s.\psi(x) = \psi(s.x)$ of $G \times X$ into $X/S$ is continuous (Chapter I, § 5, no. 3, Corollary to Proposition 8); but this follows from the continuity of $\psi$ and of the mapping

$$
(s, x) \to s.x.
$$

#### Remark {#top-iii-s2-n4-rem-2 .statement}

Let $G'$ be another topological group operating continuously on $X$, and suppose that $s.(s'x) = s'(s.x)$ for all $s \in G, s' \in G'$ and x \in X. Then the equivalence relation S defined by G' is compatible with G, and since S is open (Lemma 2) it follows that G operates continuously on X/G'. Similarly, G' operates continuously on X/G. In these circumstances the two operations of the two groups G and G' on X are said to commute.

### 5. HOMOGENEOUS SPACES

Let G be a topological group and H a subgroup of G. H operates continuously on the right on G according to the external law $(t, x) \to xt$, and the orbit of a point $x \in G$ is the left coset $xH$. The set of orbits is therefore what we have called in algebra the homogeneous space $G/H$. Whenever we speak of $G/H$ as a topological space, we shall always mean the orbit space of G (with respect to H) unless the contrary is expressly stated; i.e. the quotient space of G by the equivalence relation $x^{-1}y \in H$. In conformity with the general definitions, we say that the topology of this space is the quotient by H of the topology of G.

#### Proposition 12 {#top-iii-s2-prop-12 .statement}

The group G operates continuously on every homogeneous space $G/H$.

Since the equivalence relation $x^{-1}y \in H$ is open (no. 4, Lemma 2) this is a particular case of Proposition 11 of no. 4.

#### Proposition 13 {#top-iii-s2-prop-13 .statement}

Let G be a topological group and let H be a subgroup of G. Then the homogeneous space $G/H$ is Hausdorff if and only if H is closed in G.

H is an equivalence class for the relation $x^{-1}y \in H$ and therefore, if $G/H$ is Hausdorff, H is closed in G. Conversely, if H is closed, then the graph of this relation is closed in $G \times G$, since it is the inverse image of H under the continuous mapping $(x, y) \to x^{-1}y$. Since the relation $x^{-1}y \in H$ is open, it follows from Chapter I, § 8, no. 3, Proposition 8 that $G/H$ is Hausdorff.

#### Proposition 14 {#top-iii-s2-prop-14 .statement}

Let G be a topological group and let H be a subgroup of G. Then the homogeneous space $G/H$ is discrete if and only if H is open in G.

For the inverse images in G of the points of $G/H$ under the canonical mapping are the cosets $xH$ ($x \in G$); and these sets are open in G if and only if H is open in G.

Let X be a topological space on which a topological group G operates continuously and transitively; X is then (in the algebraic sense) a homogeneous space of G. Let x be a point of X, H_x its stabilizer. The continuous surjection s → s.x of G onto X factorizes canonically as

$$
G \xrightarrow{f_x} G/H_x \xrightarrow{g_x} X
$$

where f_x is the canonical mapping of G onto the homogeneous space G/H_x, and g_x is the bijection s.H_x → s.x of G/H_x onto X; moreover (Chapter I, § 3, no. 4, Proposition 6) g_x is a continuous mapping. But g_x is not necessarily a homeomorphism of G/H_x onto X (Exercise 29). If g_x is a homeomorphism for each x ∈ X, then we say that X is a topological homogeneous space (of the topological group G); for this to be so it is necessary and sufficient that, for each x ∈ E, the mapping s → s.x of G into X should be open.

#### Proposition 15 {#top-iii-s2-prop-15 .statement}

Let X be a topological space on which a topological group G operates continuously and transitively. For X to be a topological homogeneous space (relative to G) it is sufficient that for some point x_0 ∈ X the mapping s → s.x_0 transforms each neighbourhood of e in G into a neighbourhood of x_0 in X.

Every x ∈ X can be written as x = t.x_0 for some t ∈ G. If V is a neighbourhood of e, then V.x = (Vt).x_0 is a neighbourhood of x, for we can write (Vt).x_0 = t((t^{-1}Vt).x_0), and the assertion follows from the facts that t^{-1}Vt is a neighbourhood of e in G and that y → t.y is a homeomorphism of X onto itself (no. 4, Lemma 1). It follows that if U is any open subset of G and if x is any point of X, then U.x is open in X; for if t ∈ U, then t^{-1}U is a neighbourhood of e, hence (t^{-1}U).x is a neighbourhood of x, and t.((t^{-1}U).x) = U.x is a neighbourhood of t.x. Hence U.x is open in X, so that the mapping s → s.x of G into X is open. This completes the proof.

### 6. QUOTIENT GROUPS

#### Proposition 16 {#top-iii-s2-prop-16 .statement}

Let G be a topological group and let H be a normal subgroup of G. Then the quotient by H of the topology of G is compatible with the group structure of G/H.

If x → x̂ is the canonical mapping of G onto G/H, then we have to show that (x̂, ŷ) → x̂ŷ^{-1} is a continuous mapping of (G/H) × (G/H) into G/H. Since the equivalence relation x^{-1}y ∈ H is open (no. 4, Lemma 2), it is enough to show that (x, y) → x̂ŷ^{-1} is a continuous mapping of G × G into G/H (Chapter I, § 5, no. 3, Corollary to Proposition 8, and § 3, no. 4, Proposition 6). But (x, y) → x̂ŷ^{-1} is the composition of the continuous mappings x → x̂ and (x, y) → xy^{-1}, hence is continuous.

Whenever in the sequel we consider a quotient group $G/H$ of a topological group $G$ as a topological group, it is always to be understood that the topology of $G/H$ is the quotient by $H$ of the topology of $G$, unless the contrary is expressly stated.

#### Proposition 17 {#top-iii-s2-prop-17 .statement}

*Let $\varphi$ be the canonical mapping of a topological group $G$ onto a quotient group $G/H$. If $\mathcal{B}$ is a fundamental system of neighbourhoods of $e$ in $G$, then $\varphi(\mathcal{B})$ is a fundamental system of neighbourhoods of the identity element $\varphi(e)$ of $G/H$.*

This is a particular case of Proposition 5 of Chapter I, § 5, no. 3.

Propositions 13 and 14 give in particular, for quotient groups:

#### Proposition 18 {#top-iii-s2-prop-18 .statement}

*Let $G$ be a topological group and let $H$ be a normal subgroup of $G$.
a) *The quotient group $G/H$ is Hausdorff if and only if $H$ is closed in $G$.
b) *The quotient group $G/H$ is discrete if and only if $H$ is open in $G$.*

If $G$ is a topological group and $N$ is the closure of $\{e\}$ in $G$, then $N$ is a closed normal subgroup of $G$ (no. 1, Proposition 1), hence $G/N$ is Hausdorff; $G/N$ is called the *Hausdorff group associated with* $G$.

#### Proposition 19 {#top-iii-s2-prop-19 .statement}

*If $H$ is a discrete normal subgroup of a topological group $G$, then $G/H$ is locally isomorphic to $G$.*

Let $V$ be a neighbourhood of $e$ in $G$ which does not contain any point of $H$ other than $e$, and let $W$ be a symmetric open neighbourhood of $e$ in $G$ such that $W^2 \subset V$. Then the restriction to $W$ of the canonical mapping $\varphi$ of $G$ onto $G/H$ is *injective*; for if $x, y \in W$ and $\varphi(x) = \varphi(y)$, then $x^{-1}y \in W^2 \subset V$ and $x^{-1}y \in H$, so that $x = y$. By Proposition 17 it follows that the restriction of $\varphi$ to $W$ is a homeomorphism of $W$ onto $\varphi(W)$; since moreover $\varphi(xy) = \varphi(x)\varphi(y)$ for all $x, y \in W$, we conclude that $G$ and $G/H$ are locally isomorphic (\S 1, no. 3, Proposition 3).

### 7. SUBGROUPS AND QUOTIENT GROUPS OF A QUOTIENT GROUP

Let $G$ be a topological group, let $H$ be a normal subgroup of $G$, and let $\varphi : G \to G/H$ be the canonical mapping. We know that if $A'$ is a subgroup of $G/H$, then $\overline{\varphi}(A')$ is a subgroup of $G$ which contains $H$. Conversely, if $A$ is a subgroup of $G$, then $\varphi(A)$ is a subgroup of $G/H$; moreover, there is a canonical bijection of the quotient group $A/(A \cap H)$ onto the subgroup $\varphi(A)$ of $G/H$, and a canonical bijection of $\varphi(A)$ onto the quotient group $AH/H$, and both these bijections are isomorphisms *for the group structures*.

#### Proposition 20 {#top-iii-s2-prop-20 .statement}

Let $A$ be a subgroup of a topological group $G$, let $H$ be a normal subgroup of $G$, and let $\varphi$ denote the canonical mapping of $G$ onto $G/H$. Then the canonical bijection of $\varphi(A)$ onto $AH/H$ is an isomorphism of topological groups.

This follows from the preceding remarks, and from Proposition 10 of no. 4.

The canonical bijection of $A/(A \cap H)$ onto $\varphi(A)$ is a continuous homomorphism, since it arises from the restriction of $\varphi$ to $A$ by passing to the quotients; but in general the topological groups $A/(A \cap H)$ and $AH/H$ are not isomorphic (cf. § 4, no. 1, Proposition 1, Corollary 3).

\* For example, take $G$ to be the additive group $\mathbf{R}$ of real numbers, take $H$ to be the group $\mathbf{Z}$ of integers, and take $A$ to be the group $\theta \mathbf{Z}$ of integer multiples of an irrational number $\theta$. Then $A \cap H = \{0\}$, so that $A/(A \cap H)$ is a discrete group, isomorphic to $\mathbf{Z}$; on the other hand, $A + H$ is dense in $\mathbf{R}$ (as we shall see in Chapter V, § 1, no. 1, Proposition 1), hence $(A + H)/H$, which is locally isomorphic to $A + H$ (no. 6, Proposition 19), is not a discrete group and consequently is not isomorphic to $A/(A \cap H)$. \*

Nevertheless, we have the following proposition:

#### Proposition 21 {#top-iii-s2-prop-21 .statement}

Let $G$ be a topological group, $G_0$ a dense subgroup of $G$, $H_0$ a normal subgroup of $G_0$, $H$ the closure of $H_0$ in $G$ and $\varphi$ the canonical mapping $G \to G/H$. Then the canonical bijection $G_0/H_0 \to \varphi(G_0)$ is an isomorphism of the topological group $G_0/H_0$ onto a dense subgroup of $G/H$.

Since $H_0 = H \cap G_0$, it is enough to show that if $U_0$ is any open subset of $G_0$ which is saturated with respect to the relation $x^{-1}y \in H_0$, then $U_0$ is the intersection of $G_0$ and an open subset of $G$ which is saturated with respect to the relation $x^{-1}y \in H$ (Chapter I, § 3, no. 6, Proposition 10). Let $U$ be an open subset of $G$ such that $U_0 = U \cap G_0$. Since $U_0 = U_0 H_0$, it is easily seen that $U_0 = U H_0 \cap G_0$; but $U H_0$ is open in $G$, so we may suppose that $U = U H_0$. The set $U H$ is open in $G$ and is saturated with respect to the relation $x^{-1}y \in H$; hence the proposition will be proved if we show that $U H \cap G_0 = U_0$. Now, if $u \in U$ and $h \in H$ are such that $u h \in G_0$, then there is a symmetric neighbourhood $V$ of $e$ in $G$ such that $u V \subset U$; since $V h$ is a neighbourhood of $h$ in $G$, there exists $z \in V$ such that $z h \in H_0$. But then we have $u z^{-1} \in U$, and $u h = (u z^{-1})(z h)$; therefore $U H \cap G_0 \subset U H_0$. But $U H_0 = U$, hence $U H \cap G_0 \subset U \cap G_0 = U_0$. This completes the proof.

Let $G$ be a topological group operating continuously on a topological space $X$, and let $K$ be a normal subgroup of $G$ which is contained in the stabilizer of each point of $X$. For each $x \in X$, the relation $s \equiv t \pmod{K}$ therefore implies $s.x = t.x$, and passing to the quotient we define a mapping $s \to s.x$ of $G/K$ into $X$. It is immediately verified that with respect to the external law $(s', x) \to s'.x$, X has G/K as a group of operators. Moreover, G/K operates continuously on X with respect to this law; for the relation of equality on X and the relation $s \equiv t \pmod{K}$ on G are both open equivalence relations, and therefore the result follows from the continuity of the mapping

$$(s, x) \to s'.x = s.x$$

of $G \times X$ into X (Chapter I, § 5, no. 3, Corollary to Proposition 8, and § 3, no. 4, Proposition 6).

Now let G be a topological group operating continuously on a topological space X, and let H be any normal subgroup of G; then H operates continuously on X. Let S be the equivalence relation defined by H on X; then S is open (no. 4, Lemma 2). The relation S is compatible with the group G (no. 4); for if $y \equiv x \pmod{S}$ then there exists $t \in H$ such that $y = t.x$; hence for all $s \in G$ we have $s.y = (sts^{-1}).s.x$, and $sts^{-1} \in H$ since H is normal in G; thus $s.y \equiv s.x \pmod{S}$. If $\psi$ is the canonical mapping of X onto X/S, the group G therefore operates continuously on X/S with respect to the external law

$$(s, \psi(x)) \to \psi(s.x)$$

(no. 4, Proposition 11). Moreover, the group H is contained in the stabilizer of each of the points of X/S; as we have seen above, G/H operates continuously on $X/S = X/H$ with respect to the external law $(s', \psi(x)) \to \psi(s.x)$. If R denotes the equivalence relation on X defined by G, then the relation S implies R, and the equivalence relation R/S on X/S is that defined by the group G/H. Hence (Chapter I, § 3, no. 4, Proposition 7):

#### Proposition 22 {#top-iii-s2-prop-22 .statement}

*Let G be a topological group operating continuously on a topological space X, and let H be a normal subgroup of G. Then the canonical bijection of X/G onto $(X/H)/(G/H)$ is a homeomorphism.*

#### Corollary {#top-iii-s2-n7-cor-1 .statement}

*Let G be a topological group, H a normal subgroup of G, and K a normal subgroup of G which contains H. Then the canonical bijection of G/K onto $(G/H)/(K/H)$ is an isomorphism of topological groups.*

We know already that this bijection is an isomorphism of groups, and Proposition 22 (applied to the group K operating on the right on G) shows that it is a homeomorphism.

### 8. CONTINUOUS HOMOMORPHISMS AND STRICT MORPHISMS

#### Proposition 23 {#top-iii-s2-prop-23 .statement}

*A homomorphism f of a topological group G into a topological group $G'$ is continuous on G if and only if it is continuous at one point of G.*

Suppose $f$ is continuous at a point $a \in G$; then if $V'$ is any neighbourhood of $f(a)$, $V = \overline{f^{-1}}(V')$ is a neighbourhood of $a$. Hence if $x$ is any point of $G$, we have
$$
f(xa^{-1}V) = f(x)[f(a)]^{-1}f(V) \subset f(x)[f(a)]^{-1}V',
$$
and therefore $f$ is continuous at $x$.

A continuous homomorphism of a topological group $G$ into a topological group $G'$ is also called a *morphism* of $G$ into $G'$ for the topological group structures.

Let $f$ be a continuous homomorphism of a topological group $G$ into a topological group $G'$; the inverse image $H = \overline{f^{-1}}(e')$ of the identity element $e'$ of $G'$ is a *normal subgroup* of $G$, and $f(G)$ is a *subgroup* of $G'$. Consider the canonical factorization $f = \psi \circ \dot{f} \circ \varphi$, where $\varphi$ is the canonical mapping $G \to G/H$, $\psi$ is the canonical injection $f(G) \to G'$ and lastly $\dot{f}$ is a *continuous bijective homomorphism* of the quotient group $G/H$ onto the subgroup $f(G)$ (Chapter I, § 3, no. 5); $\dot{f}$ is said to be the bijective homomorphism *associated* with $f$. In general, $\dot{f}$ is not an isomorphism of topological groups.

For example, let $G'$ be a non-discrete topological group, and $G$ the topological group obtained by giving $G'$ the discrete topology; then the identity mapping of $G$ into $G'$ is a continuous bijective homomorphism, but is not bicontinuous.

#### Definition 1 {#top-iii-s2-def-1 .statement}

*A continuous homomorphism of a topological group $G$ into a topological group $G'$ is said to be a strict morphism of $G$ into $G'$ if the bijective homomorphism $\dot{f}$ of $G/\overline{f^{-1}}(e')$ onto $f(G)$, associated with $f$, is an isomorphism of topological groups (in other words, if $\dot{f}$ is bicontinuous).*

An isomorphism of a topological group $G$ onto a topological group $G'$ is therefore a bijective strict morphism of $G$ onto $G'$.

#### Proposition 24 {#top-iii-s2-prop-24 .statement}

*Let $f$ be a continuous homomorphism of a topological group $G$ into a topological group $G'$. Then the following three statements are equivalent:*
a) $f$ *is a strict morphism.*
b) *The image under $f$ of every open set in $G$ is an open set in $f(G)$.*
c) *The image under $f$ of every neighbourhood of the identity element in $G$ is a neighbourhood of the identity element in $G'$.*

In view of Lemma 2 of no. 4, the equivalence of a) and b) follows immediately from the definitions (Chapter I, § 5, no. 3, Proposition 5). The equivalence of b) and c) is a particular case of Proposition 15 of no. 5, if we observe that $G$ operates continuously on $f(G)$ by the external law $(s, f(t)) \to f(st)$.

#### Remark 1 {#top-iii-s2-n8-rem-1 .statement}

From condition b) of Proposition 24 it follows that every continuous homomorphism of a topological group into a discrete group is a strict morphism.

If G is compact and $f(G)$ is Hausdorff, then the bijective homomorphism $f$ associated with $f$ is bicontinuous (Chapter I, § 10, no. 2, Theorem 1, Corollary 2, and no. 1, Proposition 5, Corollary 4). Hence every continuous homomorphism of a compact group into a Hausdorff group is a strict morphism.

#### Remark 2 {#top-iii-s2-n8-rem-2 .statement}

Let $f$ be a strict morphism of G into $G'$ and let $g$ be a strict morphism of $G'$ into $G''$. If $f$ is surjective or if $g$ is injective, it follows immediately from Proposition 24 that $g \circ f$ is a strict morphism of G into $G''$. But this conclusion is no longer necessarily valid if neither of the two preceding conditions is satisfied, even if $f$ is injective and $g$ surjective (Exercise 19).

#### Remark 3 {#top-iii-s2-n8-rem-3 .statement}

Let $f$ be a continuous homomorphism of a topological group G into a topological group $G'$, and let H be a normal subgroup of G. $f$ induces a homomorphism $g$ of the group $G/H$ onto the quotient group $f(G)/f(H)$. This homomorphism $g$ is continuous. Moreover, if $f$ is a strict morphism of G into $G'$, then $g$ is a strict morphism of $G/H$ onto $f(G)/f(H)$; for if U is open in $G/H$, and if $\varphi$ (resp. $\varphi'$) denotes the canonical mapping of G onto $G/H$ [resp. of $f(G)$ onto $f(G)/f(H)$], then we have $g(u) = \varphi'(f(\overline{\varphi}^{-1}(u)))$, and since $\overline{\varphi}^{-1}(u)$ is open in G, it follows that $g(u)$ is open in $f(G)/f(H)$, which proves our assertion.

### 9. PRODUCTS OF TOPOLOGICAL GROUPS

Let $(G_i)_{i \in I}$ be a family of topological groups. Then we can define a group structure on the product set

$$
G = \prod_{i \in I} G_i
$$

(the product of the group structures of the $G_i$) by defining $(x_i).(y_i) = (x_i y_i)$. If $e_i$ is the identity element of $G_i$, then $e = (e_i)$ is the identity element of G, and we have $(x_i)^{-1} = (x_i^{-1})$. The product topology (Chapter I, § 2, no. 3) of the topologies of the $G_i$ is compatible with this group structure. For the mapping $((x_i), (y_i)) \to (x_i, y_i^{-1})$ of $G \times G$ into G is the composition of the mapping $((x_i, y_i)) \to (x_i y_i^{-1})$ of

$$
\prod_{i \in I} G_i \times G_i \text{ into } G,
$$

and the canonical mapping $((x_i), (y_i)) \to ((x_i, y_i))$ of

$$
G \times G \text{ onto } \prod_{i \in I} (G_i \times G_i);
$$

and both these mappings are continuous (Chapter I, § 4, no. 1, Corollary 1 of Proposition 1, and Proposition 2).

#### Definition 2 {#top-iii-s2-def-2 .statement}

*The topological group obtained by giving the product set*

$$
G = \prod_{i \in I} G_i
$$

*the group structure which is the product of the group structures of the $G_i$ and the topology which is the product of the topologies of the $G_i$ is called the product of the topological groups $G_i$.*

If $(J_x)_{x \in K}$ is a *partition* of $I$, then $G$ is isomorphic to the product of the topological groups $\prod_{i \in J_x} G_i$ (associativity of the product).

If $H_i$ is a subgroup of $G_i$, then the product of the topological groups $H_i$ is isomorphic to the subgroup $\prod_{i \in J} H_i$ of $\prod_{i \in I} G_i$. In particular, if $J$ is any subset of $I$, and $J' = C J$, then the topological group $\prod_{i \in J} G_i$ is isomorphic to the normal subgroup $G'_J = (\prod_{i \in J} G_i) \times (\prod_{i \in J'} \{e_i\})$ of $G$. Since the projection of every open set is an open set, the projection $\mathrm{pr}_J$ of $G$ onto $\prod_{i \in J} G_i$ is a *strict morphism*, and consequently the quotient group $G/G'$ is isomorphic to $G'_J$; $G$ is isomorphic to the product $G'_J \times (G/G'_J)$.

#### Proposition 25 {#top-iii-s2-prop-25 .statement}

*Let $(G_i)_{i \in I}$ be a family of topological groups, and let $H$ be the normal subgroup of $G = \prod_{i \in I} G_i$ consisting of all $x = (x_i)$ such that the $x_i$ are equal to the identity element $e_i$ of $G_i$ except for a finite number of indices. Then the subgroup $H$ is dense in $G$.*

This is a particular case of Chapter I, § 4, no. 3, Proposition 8.

Let $(X_i)_{i \in I}$ be a family of topological spaces, and for each $i \in I$ let $G_i$ be a topological group operating continuously on $X_i$. It is clear that the product group $G = \prod_{i \in I} G_i$ then operates continuously on the product space $X = \prod_{i \in I} X_i$ according to the law

$$
((s_i), (x_i)) \to (s_i \cdot x_i)
$$

(Chapter I, § 4, no. 1, Proposition 1, Corollary 1, and Proposition 2). Moreover the orbit under $G$ of a point $x = (x_i)$ of $X$ is the product of the orbits of the $x_i$ (with respect to the groups $G_i$). Let $\varphi_i$ be the canonical mapping of $X_i$ onto $X_i/G_i$, and let $\varphi = (\varphi_i)$ be the product mapping of $X$ onto $\prod_{i \in I} (X_i/G_i)$; then the preceding remark shows that the bijection canonically associated with $\varphi$ maps the orbit space $X/G$ onto $\prod_{i \in I} (X_i/G_i)$. Moreover:

#### Corollary {#top-iii-s2-n9-cor-1 .statement}

*Let* $(G_i)_{i \in I}$ *be a family of topological groups, and for each* $i \in I$ *let* $H_i$ *be a normal subgroup of* $G_i$; *let* $\varphi_i$ *denote the canonical mapping of* $G_i$ *onto* $G_i/H_i$. *Let* $G = \prod_{i \in I} G_i, \ H = \prod_{i \in I} H_i$. *Then the bijective homomorphism of* $G/H$ *onto* $\prod_{i \in I} (G_i/H_i)$ *associated with the continuous homomorphism* $(x_i) \to (\varphi_i(x_i))$ *is an isomorphism of topological groups.*

For this homomorphism is an isomorphism of group structures.

#### Remark {#top-iii-s2-n9-rem-1 .statement}

If $G$ is a *commutative* topological group, written additively, then the mapping $(x, y) \to x + y$ of $G \times G$ onto $G$ is a *strict morphism*. For since $(x + x') + (y + y') = (x + y) + (x' + y')$ it is a *homomorphism* of $G \times G$ onto $G$; also it is continuous, and the image of a neighbourhood $V \times V$ of the origin in $G \times G$ under this mapping is the neighbourhood $V + V$ of the origin in $G$.

### 10. SEMI-DIRECT PRODUCTS

Let $L, N$ be two subgroups of a group $G$, such that $LN = NL$; then $LN$ is a *subgroup* of $G$, since

$$
(LN)(LN)^{-1} = LNN^{-1}L^{-1} = LNL = LLN = LN
$$

Moreover, the mapping $\varphi : (x, y) \to xy$ of $N \times L$ into $G$ is *injective* if and only if $N \cap L = \{e\}$. For it is clear that if $\varphi$ is injective, then $N \cap L = \{e\}$; and conversely, the relation $x'y' = xy$, where $x, x' \in N$ and $y, y' \in L$, implies that $x^{-1}x' = {yy'}^{-1} \in N \cap L$; hence if $N \cap L = \{e\}$, then $\varphi$ is injective. Thus $\varphi$ is *bijective* if and only if $LN = G$ and $N \cap L = \{e\}$.

If $N$ is a *normal* subgroup of $G$ (or more generally is normal in some subgroup of $G$ containing $N \cup L$), the condition $LN = NL$ is automatically satisfied. Moreover, for each $y \in L$ the mapping $\sigma_y : x \to yxy^{-1}$ is an *automorphism* of the group $N$, and for any two elements $u, v$ of $L$ we have

$$(1)$$
$$
\sigma_{uv} = \sigma_u \circ \sigma_v;
$$

and for any $x, x'$ in $\mathbf{N}$ and $y, y'$ in $\mathbf{L}$ we have also

$$(2)$$
$$(xy)(x'y') = (x\sigma_y(x'))(yy').$$

Conversely:

#### Proposition 27 {#top-iii-s2-prop-27 .statement}

*Let $\mathbf{N}$ and $\mathbf{L}$ be two groups, $e'$ and $e''$ their respective identity elements. Suppose that we are given a homomorphism $y \to \sigma_y$ of $\mathbf{L}$ into the group $\Gamma$ of automorphisms of $\mathbf{N}$. Then:*

1) *On the product set $S = \mathbf{N} \times \mathbf{L}$, the internal law of composition*
$$(3)$$
$$(x, y)(x', y') = (x\sigma_y(x'), yy')$$
*defines a group structure, for which $j_1 : x \to (x, e'')$ is an isomorphism of $\mathbf{N}$ onto a normal subgroup of $S$, $j_2 : y \to (e', y)$ is an isomorphism of $\mathbf{L}$ onto a subgroup of $S$, and $\mathrm{pr}_2 : S \to \mathbf{L}$ is a surjective homomorphism whose kernel is $j_1(\mathbf{N})$ and which is such that $\mathrm{pr}_2 \circ j_2$ is the identity automorphism of $\mathbf{L}$.*

2) *Let $f : \mathbf{N} \to G$, $g : \mathbf{L} \to G$ be two homomorphisms into a group $G$, such that*
$$(4)$$
$$f(\sigma_y(x)) = g(y)f(x)g(y^{-1})$$
*for all $x \in \mathbf{N}$ and all $y \in \mathbf{L}$. Then there is a unique homomorphism $h : S \to G$ such that $f = h \circ j_1$, and $g = h \circ j_2$.*

If $x, x', x''$ are elements of $\mathbf{N}$ and $y, y', y''$ are elements of $\mathbf{L}$, then
$$
((x, y)(x', y'))(x'', y'') = (x\sigma_y(x'), yy')(x'', y'')
= (x\sigma_y(x')\sigma_{y'}(x''), yy'y'')
$$
and
$$
(x, y)((x', y')(x'', y'')) = (x, y)(x'\sigma_{y'}(x''), y'y'')
= (x\sigma_y(x'\sigma_{y'}(x'')), yy', y'')
$$
and therefore the associativity of the law (3) follows from the facts that $y \to \sigma_y$ is a homomorphism of $\mathbf{L}$ into $\Gamma$ and that $\sigma_y$ is an automorphism of $\mathbf{N}$. Clearly $(e', e'')$ is the identity element of (3), and finally
$$(x, y)(\sigma_{y^{-1}}(x^{-1}), y^{-1}) = (\sigma_{y^{-1}}(x^{-1}), y^{-1})(x, y) = (e', e'')$$
so that $(x, y)$ has an inverse in $S$. The other assertions of 1) are clear. On the other hand, since $(x, y) = (x, e'') (e', y)$, a homomorphism $h$ which satisfies the conditions of 2) must necessarily satisfy
$$h(x, y) = f(x)g(y),$$
hence is unique if it exists; moreover it is immediate from (4) that
$$f(x\sigma_y(x'))g(yy') = f(x)g(y)f(x')g(y^{-1})g(y)g(y') = f(x)g(y)f(x')g(y')$$

which shows that $(x, y) \to f(x)g(y)$ is indeed a homomorphism of S into G satisfying the conditions of 2).

#### Corollary {#top-iii-s2-n10-cor-1 .statement}

*The homomorphism h defined in 2) of Proposition 27 is injective if and only if f and g are injective and $f(N) \cap g(L) = \{e\}$; and h is surjective if and only if $f(N)g(L) = G$.

Since $h(x, y) = f(x)g(y)$, the second assertion is obvious; moreover it follows from (4) that $f(N)g(L) = g(L)f(N)$, and the first assertion follows from the remarks at the beginning of this sub-section.

The group S defined in Proposition 27 is said to be the *external semi-direct product* of N and L (relative to $\sigma$); we shall generally identify N (resp. L) with the normal subgroup $j_1(N)$ [resp. the subgroup $j_2(L)$] of S. If $\sigma_y$ is the identity element of $\Gamma$ for all $y \in L$, we retrieve the usual notion of the *product* of two groups.

Now let G be a group, and let L and N be two subgroups of G such that LN = NL and such that N is *normal* in NL, so that for each $y \in L$, $\sigma_y : x \to yxy^{-1}$ is an automorphism of N, and $y \to \sigma_y$ is a homomorphism of L into the automorphism group $\Gamma$ of N. It follows then from Proposition 27 that if S is the external semi-direct product of N and L (relative to $\sigma$), then $h : (x, y) \to xy$ is a *homomorphism* of S into G. h is bijective if and only if we have $N \cap L = \{e\}$ and $NL = G$ (Corollary to Proposition 27); G is then said to be the *semi-direct product* of its normal subgroup N and its subgroup L, and we often identify G with S by means of h.

#### Proposition 28 {#top-iii-s2-prop-28 .statement}

*Let L, N be two topological groups, let $y \to \sigma_y$ be a homomorphism of L into the group of automorphisms $\Gamma$ of the (non-topological) group structure of N; and suppose that the mapping $(x, y) \to \sigma_y(x)$ of $N \times L$ into N is continuous. Then:

1) *On the external semi-direct product S of N and L, relative to $\sigma$, the product of the topologies of N and L is compatible with the group structure; the canonical injections $j_1 : N \to S$ and $j_2 : L \to S$ are isomorphisms of the topological groups N and L respectively onto the subgroups $j_1(N)$ and $j_2(L)$ of S, and $pr_2$ is a strict morphism of S onto L.*

2) *Let $f : N \to G$ and $g : L \to G$ be two continuous homomorphisms into a topological group G, satisfying (4); then the homomorphism*

$$
(x, y) \to f(x)g(y)
$$

*of S into G is continuous.*

This is an immediate consequence of the definitions and of the properties of the product topology.

The topological group S thus defined is said to be the external topological semi-direct product of N and L (relative to σ); notice that the condition imposed on σ implies that L operates continuously on the left on N according to the external law $(x, y) \to \sigma_y(x)$ [no. 4].

Now let G be a topological group and let N and L be two subgroups of G such that G is the semi-direct product of N and L, qua non-topological group; it is then clear that the mapping $(x, y) \to \sigma_y(x)$ is continuous on $N \times L$, and that the canonical bijective homomorphism

$$
h : (x, y) \to xy
$$

of S onto G is continuous. But this homomorphism is not necessarily bicontinuous; when it is bicontinuous, G is said to be the topological semi-direct product of N and L. For this to be so it is necessary and sufficient that, if $p : G \to N$ and $q : G \to L$ are the mappings which make correspond to $z \in G$ the unique elements $p(z) \in N$ and $q(z) \in L$ such that $z = p(z)q(z)$, then one of the mappings $p, q$ is continuous (in which case both are continuous). It comes to the same thing to say that the restriction to L of the canonical mapping $G \to G/N$ is an isomorphism of the topological group L onto the topological group G/N.

### Exercises {#top-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
