---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 6
section_title: Topological groups with operators; topological rings division rings and fields
lang: en
source: top-i-iv
book_pages: 271-283, 315-324
pdf_pages: 0277-0289, 0321-0330
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS WITH OPERATORS
      page: 271
      pdf_page: 277
    - "no": 2
      title: TOPOLOGICAL DIRECT SUM OF STABLE SUBGROUPS
      page: 272
      pdf_page: 278
    - "no": 3
      title: TOPOLOGICAL RINGS
      page: 274
      pdf_page: 280
    - "no": 4
      title: SUBRINGS; IDEALS; QUOTIENT RINGS; PRODUCTS OF RINGS
      page: 276
      pdf_page: 282
    - "no": 5
      title: COMPLETION OF A TOPOLOGICAL RING
      page: 276
      pdf_page: 282
    - "no": 6
      title: TOPOLOGICAL MODULES
      page: 278
      pdf_page: 284
    - "no": 7
      title: TOPOLOGICAL DIVISION RINGS AND FIELDS
      page: 281
      pdf_page: 287
    - "no": 8
      title: UNIFORMITIES ON A TOPOLOGICAL DIVISION RING
      page: 282
      pdf_page: 288
statements: 23
exercises: 26
content_sha256: dcb0cb1caa65d1aeec0e6b82e7da15c59c5cd47bbe0e662c7ae93d14fa42ae2e
---

## 6. TOPOLOGICAL GROUPS WITH OPERATORS; TOPOLOGICAL RINGS, DIVISION RINGS AND FIELDS

### 1. TOPOLOGICAL GROUPS WITH OPERATORS

On a set $G$, a structure of a group with operators and a topology are said to be compatible if the topology and the group structure of $G$ are compatible (§ 1, no. 1) and if in addition the endomorphisms of $G$ produced by the operators are continuous. The set $G$, together with the given topology and structure of group with operators, is then said to be a topological group with operators.

If $H$ is a stable subgroup of a topological group $G$ with operators, then the topology induced on $H$ by the topology of $G$ is compatible with the structure of group with operators on $H$. Furthermore:

#### Proposition 1 {#top-iii-s6-prop-1 .statement}

*If $H$ is a stable subgroup of a topological group $G$ with operators, then the closure $\overline{H}$ of $H$ in $G$ is a stable subgroup of $G$.*

We know already (§ 2, no. 1, Proposition 1) that $\overline{H}$ is a subgroup of $G$. Also if $\alpha$ is any operator on $G$, the image of $H$ under the continuous mapping $x \to x^\alpha$ is contained in $H$, and therefore the image of $\overline{H}$ is contained in $\overline{H}$ (Chapter I, § 2, no. 1, Theorem 1).

Let $H$ be a stable normal subgroup of a topological group $G$ with operators. Then for each operator $\alpha$ on $G$, the mapping of $G/H$ into itself induced by $x \to x^\alpha$ is continuous (§ 2, no. 8, Remark 3), and the structure of group with operators on $G/H$ is therefore compatible with the quotient topology on $G/H$.

Let $(G_i)_{i \in I}$ be a family of topological groups with operators, where each $G_i$ is assumed to have the same operator set $\Omega$. For each $\alpha \in \Omega$, the mapping $x \to ((\mathrm{pr}_i x)^\alpha)$ of $G = \prod_{i \in I} G_i$ into itself is continuous (Chapter I, § 4, no. 1, Proposition 1), and the structure of groups with operators on $G$ is therefore compatible with the product topology on $G$.

If $G$ is a Hausdorff topological group with operators and if $G$ has a completion $\hat{G}$ (§ 3, no. 4), then every endomorphism $x \to x^\alpha$ of $G$ defined by an operator on $G$ can be extended by continuity to an endomorphism of $\hat{G}$ (§ 3, no. 3, Proposition 5). Hence $\hat{G}$ has the structure of a topological group with operators, and the operator set is the same for $\hat{G}$ as for $G$.

### 2. TOPOLOGICAL DIRECT SUM OF STABLE SUBGROUPS

Since the study of commutative groups with operators is equivalent to the study of modules we shall sometimes allow ourselves to use the terminology proper to modules for arbitrary commutative groups with operators; thus we may speak of *linear mappings* instead of homomorphisms of commutative groups with operators, and we may use the word *projector* to denote an idempotent endomorphism of a commutative group with operators.

If a commutative topological group $E$ with operators (written additively) is the direct sum of a *finite* family $(M_i)_{1 \leq i \leq n}$ of stable subgroups, then the canonical bijection $(x_i) \to \sum_{i=1}^n x_i$ of the product group $\prod_{i=1}^n M_i$ onto $E$ is *continuous*, but is *not necessarily a homeomorphism*.

#### Definition 1 {#top-iii-s6-def-1 .statement}

*Let $E$ be a commutative topological group with operators, and let $(M_i)_{1 \leq i \leq n}$ be a finite family of stable subgroups of $E$, such that $E$ is the direct sum of the $M_i$. Then $E$ is said to be the topological direct sum of the $M_i$ if the canonical mapping $(x_i) \to \sum_{i=1}^n x_i$ of the product group $\prod_{i=1}^n M_i$ onto $E$ is a homeomorphism* (and therefore an isomorphism of topological groups with operators).

#### Proposition 2 {#top-iii-s6-prop-2 .statement}

*Let $E$ be a commutative topological group with operators which is the direct sum of stable subgroups $M_i$ ($1 \leq i \leq n$). Let $(p_i)_{1 \leq i \leq n}$ be the family of projectors associated with the decomposition $E = \sum_{i=1}^n M_i$. Then $E$ is the topological direct sum of the $M_i$ if and only if the $p_i$ are continuous.*

For the mapping $x \to (p_i(x))$ is the inverse of the mapping $(x_i) \to \sum_{i=1}^n x_i$.

Since $1 = \sum_{i=1}^n P_i$ (where $1$ denotes the identity mapping of $E$) it is sufficient for $n - 1$ of the projectors $p_i$ to be continuous in order that the $n$ th should also be continuous.

If $E$ is the topological direct sum of two stable subgroups $M, N$, then $N$ is said to be a *topological complement* of $M$ in $E$; this is the case if and only if the canonical mapping of $E/M$ onto is an *isomorphism* of topological groups with operators.

#### Corollary {#top-iii-s6-n2-cor-1 .statement}

*Let $E$ be a commutative topological group with operators, and let $M$ be a stable subgroup of $E$. Then the following conditions are equivalent:*

a) $M$ has a topological complement in $E$.

b) *There is a continuous projector $p$ of $E$ into $E$ such that $p(E) = M$.*

c) *The identity mapping of $M$ can be extended to a continuous linear mapping of $E$ onto $M$.*

It follows from Proposition 2 that a) implies b), and it is clear that b) implies c). Finally, if $p$ is a continuous linear mapping of $E$ onto $M$ which extends the identity mapping of $M$, then $p$ is a continuous projector, and the projectors $p$ and $1 - p$ are associated with the direct sum decomposition $E = M + N$, where $N = \overline{p}(0)$.

#### Remark 1 {#top-iii-s6-n2-rem-1 .statement}

To avoid confusion, we shall sometimes say that a stable subgroup of $E$ which is a complement of $M$ (in the sense of the structure of group with operators, without a topology) is an *algebraic complement* of $M$.

#### Remark 2 {#top-iii-s6-n2-rem-2 .statement}

If a *Hausdorff* commutative topological group with operators is the topological direct sum of a family $(M_i)_{1 \leq i \leq n}$ of stable subgroups, then each of the subgroups $M_i$ is *closed* in $E$, for $M_i$ is the set of all $x \in E$ such that $p_i(x) = x$ (Chapter I, § 8, no. 1, Proposition 2).

#### Proposition 3 {#top-iii-s6-prop-3 .statement}

*Let $E, F$ be two commutative topological groups with operators, and let $u$ be a continuous linear mapping of $E$ into $F$. In order that there should exist a continuous linear mapping $v$ of $F$ into $E$ such that $u \circ v$ is the identity mapping of $F$ (in which case $u$ is said to be right invertible and $v$ is said to be a *right inverse* of $u$) it is necessary and sufficient that $u$ is a strict morphism (§ 2, no. 8) of $E$ onto $F$ and that $\overline{u}(0)$ has a topological complement in $E$.*

The conditions are *necessary*. For we have then $u(v(F)) = F$ and *a fortiori* $u(E) = F$; furthermore, if $p = v \circ u$, then $p$ is a continuous linear mapping of $E$ into itself such that $p^2 = p$; therefore (Corollary to Proposition 2) $p(E) = v(u(E)) = v(F)$ has a topological complement $\overline{p}(0)$ in $E$; but since $u(p(x))) = u(x)$ by hypothesis, we have $\overline{u}(0) = \overline{p}(0)$. Finally, the bijective mapping of $E/\overline{u}(0)$ onto $F$, associated with $u$, is the composition of the bijective mapping of $E/\overline{u}(0)$ onto $v(F)$, associated with $p$, and the restriction of $u$ to $v(F)$; since $v$ is continuous, both these mappings are isomorphisms, and therefore $u$ is a strict morphism of $E$ onto $F$.

The conditions are *sufficient*. For if $\varphi$ is the canonical homomorphism of E onto $E/\overline{u}^1(o)$, to say that $\overline{u}^1(o)$ has a topological complement M in E is to say that the restriction of $\varphi$ to M is an isomorphism of M onto $E/\overline{u}^1(o)$. Since on the other hand $u = w \circ \varphi$, where w is an isomorphism of $E/\overline{u}^1(o)$ onto F, we see that the restriction of u to M is an isomorphism of M onto F, and the inverse isomorphism v is therefore such that $u \circ v$ is the identity mapping of F onto itself.

#### Proposition 4 {#top-iii-s6-prop-4 .statement}

*Let E, F be two commutative topological groups with operators, and let u be a continuous linear mapping of E into F. In order that there should exist a continuous linear mapping v of F into E such that $v \circ u$ is the identity mapping of E onto itself* (in which case u is said to be *left invertible* and v is said to be a *left inverse* of u) *it is necessary and sufficient that u is a (topological) isomorphism of E onto u(E), and that u(E) has a topological complement in F.*

The conditions are *sufficient*, for if they are satisfied we obtain a left inverse v of u by taking the composition of the isomorphism of u(E) onto E which is the inverse of u, with a continuous projector of F onto u(E).

The conditions are *necessary*. For the relation $v(u(x)) = x$ shows that $\overline{u}^1(o) = \{ o \}$; u is therefore a bijection of E onto u(E), and since the restriction of v to u(E) is continuous, it follows that u is an isomorphism of E onto u(E). On the other hand, if we put $q = u \circ v$, then q is a continuous linear mapping of F onto u(E) such that $q^2 = q$, which proves (Corollary to Proposition 2) that u(E) has a topological complement in F.

### 3. TOPOLOGICAL RINGS

#### Definition 2 {#top-iii-s6-def-2 .statement}

*A topological ring is a set A which carries a ring structure and a topology satisfying the following axioms:*

*(AT$_\mathrm{I}$)*. *The mapping* $(x, y) \to x + y$ *of* $A \times A$ *into* A *is continuous.*
*(AT$_\mathrm{II}$)*. *The mapping* $x \to -x$ *of* A *into* A *is continuous.*
*(AT$_\mathrm{III}$)*. *The mapping* $(x, y) \to xy$ *of* $A \times A$ *into* A *is continuous.*

The first two axioms express that the topology of A is compatible with its *additive group* structure (§ 1, no. 1).

If a ring structure and a topology are given on a set A, they are said to be *compatible* if they satisfy axioms (AT$_\mathrm{I}$), (AT$_\mathrm{II}$) and (AT$_\mathrm{III}$).

#### Example 1 {#top-iii-s6-n3-exa-1 .statement}

On any ring A, the *discrete* topology is compatible with the ring structure. A topological ring whose topology is discrete is called a *discrete* ring.

#### Example 2 {#top-iii-s6-n3-exa-2 .statement}

We shall see in Chapter IV that the topology of the rational line Q (resp. the real line R) is compatible with the ring structure of Q (resp. R).*

In a topological ring every left homothety $x \to ax$ (resp. every right homothety $x \to xa$) is continuous (and is a homeomorphism if $a$ is a unit of $A$).

Since we can write identically
$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0)
$$
the axiom (AT_{III}) [in view of (AT_I) and (AT_{II})] is equivalent to the conjunction of the following two axioms:
(AT_{III a}). *Given any* $x_0 \in A$, *the mappings* $x \to x_0 x$ *and* $x \to xx_0$ *are continuous at the point* $x = 0$.
(AT_{III b}). *The mapping* $(x, y) \to xy$ *of* $A \times A$ *into* $A$ *is continuous at the point* $(0, 0)$.

From this we can deduce a necessary and sufficient set of conditions which the filter $\mathcal{B}$ of neighbourhoods of $0$ in a ring $A$ must satisfy in order to define a topology on $A$ compatible with its ring structure: $\mathcal{B}$ must satisfy axioms (GA_I) and (GA_{II}) of § 1, and also the following two axioms:
(AV_I). *For all* $x_0 \in A$ *and all* $V \in \mathcal{B}$, *there exists* $W \in \mathcal{B}$ *such that* $x_0 W \subset V$ *and* $W x_0 \subset V$.
(AV_{II}). *For all* $V \in \mathcal{B}$, *there exists* $W \in \mathcal{B}$ *such that* $WW \subset V$.

#### Remark {#top-iii-s6-n3-rem-1 .statement}

In analysis one fairly often meets rings which satisfy axioms (AT_I), (AT_{II}) and (AT_{III a}), but not (AT_{III b}). *An example is the ring of measures on a compact group, where multiplication is convolution and the topology is the vague topology.*

*Example 3).* Let $\mathcal{B}$ be a filter base on a ring $A$, consisting of *two-sided ideals*. $\mathcal{B}$ is a fundamental system of neighbourhoods of $0$ for a topology compatible with the additive group structure of $A$, and it follows immediately from (AV_I) and (AV_{II}) that this topology is compatible with the *ring* structure of $A$.

Let $X$ be a topological space, and let $f$ and $g$ be two mappings of $X$ into a topological ring $A$. If $f$ and $g$ are continuous at a point $x_0 \in X$, then $f + g$, $-f$ and $fg$ are continuous at this point. It follows that the continuous mappings of $X$ into $A$ form a *subring* of the ring $A^X$ of all mappings of $X$ into $A$. We see also that, if $A$ is *commutative*, then every *polynomial in n variables*, with coefficients in $A$ and defined on $A^n$, is *continuous* on $A^n$. Again, let $f$ and $g$ be two mappings of a set $X$, *filtered* by a filter $\mathfrak{F}$, into a *Hausdorff* topological ring $A$; if $\lim_{\mathfrak{F}} f$ and $\lim_{\mathfrak{F}} g$ exist, then so do $\lim_{\mathfrak{F}} (f + g)$, $\lim_{\mathfrak{F}} (-f)$ and $\lim_{\mathfrak{F}} (fg)$, and we have (Chapter I, § 7, no. 4, Proposition 9, Corollary 1, and § 8, no. 1, Proposition 1)

(1) $$ \lim_{\mathfrak{F}} (f + g) = \lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g, $$
(2) $$ \lim_{\mathfrak{F}} (-f) = -\lim_{\mathfrak{F}} f, $$
(3) $$ \lim_{\mathfrak{F}} (fg) = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g). $$

### 4. SUBRINGS; IDEALS; QUOTIENT RINGS; PRODUCTS OF RINGS

If $H$ is a subring of a topological ring $A$, then the topology induced on $H$ by that of $A$ is compatible with the ring structure of $H$. The topological ring structure thus defined on $H$ is said to be *induced* by that of $A$.

#### Proposition 5 {#top-iii-s6-prop-5 .statement}

*Let $H$ be a dense subring of a topological ring $A$, and let $K$ be a subring (resp. left ideal, right ideal, two-sided ideal) of $H$. Then the closure $\overline{K}$ of $K$ in $A$ is a subring (resp. left ideal, right ideal, two-sided ideal) of $A$.*

The proof is the same as for Proposition 8 of § 2, n. 3 : if for example $K$ is a left ideal in $H$, then the mapping $(z, x) \to zx$ is continuous on $A \times A$ and maps $H \times K$ into $K$; hence it maps $A \times K = \overline{H} \times K$ into $\overline{H}$.

Let $H$ be a *two-sided* ideal in a topological ring $A$. By the same argument as for quotient groups, we see that the *quotient* of the topology of $A$ by the relation $x - y \in H$ is compatible with the ring structure of $A/H$. In particular, if $A$ is not Hausdorff, then the closure $N$ of $\{0\}$ in $A$ is a *closed two-sided ideal*, by Proposition 5; the quotient ring, which is Hausdorff ($\S$ 2, no. 5, Proposition 13) is called the *Hausdorff ring associated with* $A$.

Let $(A_i)_{i \in I}$ be a family of topological rings. On the set $A = \prod_{i \in I} A_i$, the *product* of the topologies of the $A_i$ is compatible with the product of the ring structures of the $A_i$ (same proof as for product groups); the topological ring $A$ thus defined is called the *product* of the topological rings $A_i$.

### 5. COMPLETION OF A TOPOLOGICAL RING

When we speak of *the* uniformity of a topological ring, we always mean the uniformity of its *additive group*, unless the contrary is expressly stated; in particular, $A$ is said to be a *complete* ring if the additive group of $A$ is complete.

Let $A$ be a *Hausdorff* topological ring; as an additive group $A$ can be considered as a dense subgroup of a *complete Hausdorff commutative* group $\hat{A}$, which is determined up to isomorphism ($\S$ 3, no. 5, Theorem 2). In order that we should be able to consider $A$ as a *subring* of a *complete ring*, it is necessary to be able to extend the function $xy$ by continuity to the space $\hat{A} \times \hat{A}$. The possibility of this extension will follow from the following more general theorem :

#### Theorem 1 {#top-iii-s6-thm-1 .statement}

Let E, F, G be three complete Hausdorff commutative groups; let A be a dense subgroup of E and let B be a dense subgroup of F. If f is a $\mathbf{Z}$ continuous $\mathbf{Z}$-bilinear (*) mapping of $A \times B$ into G, then f can be extended by continuity to a continuous $\mathbf{Z}$-bilinear mapping of $E \times F$ into G.

Let $(x_0, y_0)$ be an arbitrary point of $E \times F$, and let $\mathfrak{U}, \mathfrak{B}$ be the traces on A, B respectively of the neighbourhood filters of $x_0, y_0$ ($\mathfrak{U}, \mathfrak{B}$ are filters, by hypothesis). To show that f can be extended by continuity, it is enough to show that $f(\mathfrak{U} \times \mathfrak{B})$ is a Cauchy filter-base on G (Chapter II, § 3, no. 6, Proposition 11). Consider the identity

$$
f(x', y') - f(x, y) = f(x' - x, y_1) + f(x_1, y' - y) + f(x' - x, y' - y_1).
$$

We shall show that by taking $(x, y)$ and $(x', y')$ in a sufficiently small set of $\mathfrak{U} \times \mathfrak{B}$, and by choosing $x_1$ and $y_1$ suitably, we can make each of the terms on the right-hand side very small. Let W be any neighbourhood of 0 in G; since f is continuous at $(0, 0) \in A \times B$, there is a set $U \in \mathfrak{B}$ and a set $V \in \mathfrak{B}$ such that $f(x' - x, y' - y) \in W$ whenever $x \in U, x' \in U, y \in V, y' \in V$. Take a point $x_1 \in U$ and a point $y_1 \in V$; then for all $x, x'$ in U and all $y, y'$ in V we shall have

$$
f(x' - x, y' - y_1) + f(x - x_1, y' - y) \in W + W.
$$

On the other hand, the partial mapping $x \to f(x, y_1)$ is continuous on A; hence there is a set $U' \subset U$, belonging to $\mathfrak{U}$, and such that, whenever $x$ and $x'$ belong to $U'$, we have $f(x' - x, y_1) \in W$. Likewise there exists $V' \subset V$ belonging to $\mathfrak{B}$ such that, whenever $y$ and $y'$ belong to $V'$, we have $f(x_1, y' - y) \in W$. Consequently, if $(x, y)$ and $(x', y')$ are any two points of $U' \times V'$, then

$$
f(x', y') - f(x, y) \in W + W + W + W;
$$

this proves the existence of the extension $\overline{f}$ of f. The fact that $\overline{f}$ is $\mathbf{Z}$-bilinear is an immediate consequence of the principle of extension of identities (Chapter I, § 8, no. 1, Corollary 1 to Proposition 2).

Q.E.D.

In the application of this theorem to a Hausdorff topological ring A, we take E, F and G to be $\hat{A}$, A and B to be the ring A, and f to be

(*) $f$ is said to be $\mathbf{Z}$-bilinear if, for all elements $x, x'$ of A and all elements $y, y' \in B$ we have

$$
f(x + x', y) = f(x, y) + f(x', y)
$$
and
$$
f(x, y + y') = f(x, y) + f(x, y').
$$

the $\mathbf{Z}$-bilinear mapping $(x, y) \to xy$, which by hypothesis is continuous. We denote again by $xy$ the value of the extended function on $\hat{A} \times \hat{A}$; this function is a law of composition on $\hat{A}$, and to say that it is $\mathbf{Z}$-bilinear means that it is distributive on both sides with respect to addition; and it is also *associative*, by the principle of extension of identities. Consequently:

#### Proposition 6 {#top-iii-s6-prop-6 .statement}

*A Hausdorff topological ring* $A$ *is isomorphic to a dense subring of a complete Hausdorff ring* $\hat{A}$, *which is determined up to isomorphism* (and is called the *completion* of $A$).

If $A$ is *commutative* (resp. *has an identity element*) then the same is true of $\hat{A}$ (principle of extension of identities).

Let $A$ be a topological ring, not necessarily Hausdorff; let $N$ be the closure of $\{0\}$ in $A$, and let $A' = A/N$ be the Hausdorff ring associated with $A$. Then $\hat{A}'$, the completion of $A'$, is called the *Hausdorff completion* of $A$ and is also denoted by $\hat{A}$. One shows as in § 3, no. 4, Proposition 8 that every continuous ring homomorphism $u$ of $A$ with a *complete Hausdorff* topological ring $C$ can be uniquely factorized as $u = v \circ \varphi$, where $v$ is a continuous homomorphism of $\hat{A}$ into $C$ and $\varphi$ is the canonical mapping of $A$ into $\hat{A}$. If $A, B$ are two topological rings, and $u : A \to B$ is a continuous homomorphism, there is therefore a unique continuous homomorphism $\hat{u} : \hat{A} \to \hat{B}$ such that the diagram

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
\varphi \downarrow & & \psi \downarrow \\
\hat{A} & \xrightarrow{\hat{u}} & \hat{B}
\end{array}
$$

is commutative ($\varphi$ and $\psi$ being the canonical mappings); we have only to apply the preceding result to $\psi \circ u$.

### 6. TOPOLOGICAL MODULES

#### Definition 3 {#top-iii-s6-def-3 .statement}

*Given a topological ring* $A$ *with an identity element, a topological left* $A$*-module is a set* $E$, *together with*:

1) *a left* $A$*-module structure*;
2) *a topology compatible with the additive group structure of* $E$, *and satisfying the following axiom*:
(MT) *The mapping* $(\lambda, x) \to \lambda x$ *of* $A \times E$ *into* $E$ *is continuous*.

We define similarly the notion of a topological right $A$-module; since every right $A$-module can be considered as a left $A^0$-module, where $A^0$ is the opposite ring of $A$, and since the topology of $A$ is compatible with the ring structure of $A^0$, there is no need to distinguish between topological right $A$-modules and topological left $A^0$-modules.

#### Example 1 {#top-iii-s6-n6-exa-1 .statement}

A topological vector space over $\mathbf{R}$ (resp. $\mathbf{C}$) is a topological $\mathbf{R}$ (resp. $\mathbf{C}$) module.

#### Example 2 {#top-iii-s6-n6-exa-2 .statement}

Let $A$ be a ring and let $\mathcal{B}$ be a filter base on $A$ consisting of two-sided ideals of $A$; let $E$ be a left $A$-module. If we give $A$ the topology (compatible with its ring structure) for which $\mathcal{B}$ is a fundamental system of neighbourhoods of $0$ (no. 3, Example 3), and $E$ the topology (compatible with its additive group structure) in which the sets $aE$, as $a$ runs through $\mathcal{B}$, form a fundamental system of neighbourhoods of $0$ ($§ 1$, no. 2, Example), it is immediately verified that $E$ is a topological $A$-module.

#### Remark {#top-iii-s6-n6-rem-1 .statement}

Given a topological ring $A$, consider, on a left $A$-module $E$, a topology compatible with the additive group structure of $E$. By virtue of the identity
$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0)x_0 + \lambda_0(x - x_0) + (\lambda - \lambda_0)(x - x_0)
$$
the axiom (MT) is equivalent to the conjunction of the following three axioms:
(MT$_I'$). *For each* $x_0 \in E$, *the mapping* $\lambda \to \lambda x_0$ *is continuous at the point* $\lambda = 0$.
(MT$_{II}'$). *For each* $\lambda_0 \in A$, *the mapping* $x \to \lambda_0 x$ *is continuous at the point* $x = 0$.
(MT$_{III}'$). *The mapping* $(\lambda, x) \to \lambda x$ *is continuous at the point* $(0, 0)$.

We deduce from this a necessary and sufficient set of conditions that the *filter* $\mathcal{B}$ *of neighbourhoods of* $0$ *in an* $A$*-module* $E$ *must satisfy in order to define a topology on* $E$ *compatible with its module structure;* $\mathcal{B}$ *must satisfy the axioms* (GA$_I$) *and* (GA$_{II}$) *of* $§ 1$, *no. 2*, *and in addition must satisfy the following three axioms:*
(MV$_I$). *For each* $x_0 \in E$ *and* $V \in \mathcal{B}$, *there is a neighbourhood* $S$ *of* $0$ *in* $A$ *such that* $S.x_0 \subset V$.
(MV$_{II}$). *For each* $\lambda_0 \in A$ *and* $V \in \mathcal{B}$, *there exists* $W \in \mathcal{B}$ *such that* $\lambda_0 W \subset V$.
(MV$_{III}$). *For each* $V \in \mathcal{B}$ *there exists* $U \in \mathcal{B}$ *and a neighbourhood* $T$ *of* $0$ *in* $A$ *such that* $T.U \subset V$.

Every commutative topological group is a topological $\mathbf{Z}$-module when the ring $\mathbf{Z}$ is given the discrete topology.

If $M$ is a submodule of a topological $A$-module $E$, it is clear that the topology induced on $M$ by the topology of $E$ is compatible with the module structure of $M$. Moreover, on the quotient $A$-module $E/M$, the topology which is the quotient by $M$ of the topology of $E$ is compatible with the $A$-module structure. To see this it is enough to show that the mapping $(\lambda, x) \to \lambda x$ of $A \times (E/M)$ onto $E/M$ is continuous (where $x \to x'$ denotes the canonical mapping of $E$ onto $E/M$). Now, since we may identify the additive topological groups $A \times (E/M)$ and $(A \times E)/(\{0\} \times M)$ (§ 2, no. 9, Corollary to Proposition 26), it is enough to show that the mapping $(\lambda, x) \to \lambda x'$ of $A \times E$ into $E/M$ is continuous; and this is immediate, since the mapping in question is the composition of $x \to x'$ and $(\lambda, x) \to \lambda x$.

Let $(E_i)_{i \in I}$ be an arbitrary family of topological $A$-modules, and let $E = \prod_{i \in I} E_i$ be the $A$-module which is the product of the $E_i$. Then the product topology on $E$ is compatible with the $A$-module structure of $E$. To prove this it is enough to show that the mapping $(\lambda, x) \to (\lambda \cdot \mathrm{pr}_i x)_{i \in I}$ of $A \times E$ into $E$ is continuous, or (by Proposition 1 of Chapter I, § 4, no. 1) that for each index $x \in I$ the mapping $(\lambda, x) \to \lambda \cdot \mathrm{pr}_x x$ is a continuous mapping of $A \times E$ into $E_x$; but this mapping is the composition of $(\lambda, x_x) \to \lambda x_x$ and $(\lambda, x) \to (\lambda, \mathrm{pr}_x x)$, both of which are continuous.

Let $A$ be a Hausdorff topological ring and $E$ a Hausdorff topological $A$-module. Let $\hat{E}$ be the additive group which is the completion of the commutative topological group $E$ (§ 3, no. 5, Theorem 2). The $\mathbf{Z}$-bilinear mapping $(\lambda, x) \to \lambda x$ of the product $A \times E$ of the additive groups $A, E$ into the additive group $E$ can be extended by continuity to a $\mathbf{Z}$-bilinear mapping of $\hat{A} \times \hat{E}$ into $\hat{E}$ (no. 5, Theorem 1), and this mapping we continue to denote by $(\lambda, x) \to \lambda x$. By virtue of the principle of extension of identities, we have $\lambda (\mu x) = (\lambda \mu) x$ for $\lambda \in \hat{A}, \mu \in \hat{A}$ and $x \in \hat{E}$, and $1 \cdot x = x$ for all $x \in \hat{E}$; the external law $(\lambda, x) \to \lambda x$ therefore defines an $\hat{A}$-module structure on $\hat{E}$ compatible with its topology. The topological $\hat{A}$-module $\hat{E}$ thus defined is called the *completion* of the topological $A$-module $E$.

Let $E$ be a topological module over a topological ring $A$, where neither $A$ nor $E$ is necessarily Hausdorff. Let $N$ (resp. $F$) be the closure of $\{0\}$ in $A$ (resp. $E$). $N$ is a two-sided ideal of $A$ (no. 4, Proposition 5) and $F$ is a sub-$A$-module of $E$ (no. 1, Proposition 1); furthermore, by continuity we have $\lambda x \in F$ whenever $\lambda \in N$ or $x \in F$. We can therefore define, by passing to the quotients, a mapping $(\dot{\lambda}, \dot{x}) \to \dot{\lambda} \dot{x}$ of $(A/N) \times (E/F)$ into $E/F$; it is easily verified (by use of the Corollary to Proposition 26 of § 2, no. 9) that this mapping is continuous, and therefore defines a structure of a topological $(A/N)$-module on $E/F$. If we put $B = A/N$ and $L = E/F$, then the $B$-module $L$ is called the Hausdorff module *associated* with $E$; its completion $\hat{L}$ is a topological module over the Hausdorff completion $\hat{A}$ (equal by definition to $\hat{B}$) of $A$ (no. 5), and this module $\hat{L}$ is called the *Hausdorff completion* of $E$ and is denoted

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow \varphi & & \downarrow \varphi' \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{E}'
\end{array}
$$

is commutative, $\varphi$ and $\varphi'$ being the canonical mappings.

The definitions and results of this section apply equally well to *pseudo-modules* over an arbitrary topological ring, by deleting all mention of the identity element of the ring.

### 7. TOPOLOGICAL DIVISION RINGS AND FIELDS

In what follows, and in Chapters IV and V, if $K$ is a *division ring* we shall denote by $K^*$ the *multiplicative group* of non-zero elements of $K$.

#### Definition 4 {#top-iii-s6-def-4 .statement}

*A topological division ring is a set* $K$ *carrying a division ring structure and a topology compatible with the ring structure of* $K$, *and satisfying in addition the following axiom:*

(KT) *The mapping* $x \to x^{-1}$ *of* $K^*$ *into* $K^*$ *is continuous.*

*A commutative topological division ring is called a topological field.*

A division ring structure and a topology on a set $K$ are said to be *compatible* if the corresponding ring structure and the topology are compatible and if in addition axiom (KT) is satisfied.

#### Example 1 {#top-iii-s6-n7-exa-1 .statement}

On any division ring $K$, the *discrete* topology is compatible with the division ring structure. A topological division ring whose topology is discrete is called a *discrete* division ring.
\* 2) The topology of the rational line $Q$ (resp. the real line $R$) is compatible with the field structure of $R$ (resp. $R$) (see Chapter IV, § 3). \*

Definition 4 shows that, if $K$ is a topological division ring, then the topology *induced* by that of $K$ on the multiplicative group $K^*$ is compatible with the group structure of $K^*$.

If $a \neq 0$, the homotheties $x \to ax$ and $x \to xa$ are homeomorphisms of $K$ onto itself; and so is the mapping $x \to ax + b$ for all $b \in K$. Note that the homotheties $x \to ax$ and $x \to xa$ are *automorphisms* of the (topological) *additive group* of $K$ if $a \neq 0$. If $V$ is any neighbourhood of $o$ in $K$, it follows therefore that $aV$ and $Va$ are neighbourhoods of $o$ for all $a \neq 0$.

Let $X$ be a topological space, and let $f$ be a mapping of $X$ into a topological division ring $K$. If $f$ is continuous at a point $x_0 \in X$ and if $f(x_0) \neq 0$, then $f^{-1}$ is continuous at $x_0$. In particular, if $K$ is a topological *field*, then every *rational function* in $n$ variables with coefficients in $K$ is continuous at every point of $K^n$ where its denominator does not vanish.

Likewise, if $f$ is a mapping of a set $X$, filtered by a filter $\mathfrak{F}$, into a Hausdorff topological division ring $K$, and if $\lim_{\mathfrak{F}} f$ exists and is not $0$, then $\lim_{\mathfrak{F}} f^{-1}$ exists and we have

$$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}.
$$

If $H$ is a *division subring* of a topological division ring $K$, then the topology induced on $H$ by the topology of $K$ is compatible with the division ring structure of $H$. The structure of a topological division ring thus defined on $H$ is said to be *induced* by that of $K$. Furthermore, $\overline{H}$ is also a *division subring* of $K$ (the proof is analogous to that of Proposition 5).

In a topological division ring $K$, the closure of the set $\{0\}$ is a two-sided ideal, by Proposition 5, and hence must be either $\{0\}$ or $K$. In other words, if the topology of $K$ is not the coarsest topology (Chapter I, § 2, no. 2) then it is Hausdorff (§ 1, no. 2, Proposition 2).

### 8. UNIFORMITIES ON A TOPOLOGICAL DIVISION RING

If $K$ is a topological division ring it is necessary to distinguish between:
1) the uniformity of the *additive group* of $K$, which is defined on $K$ and is called the *additive uniformity* of $K$; and 2) the left and right uniformities of the *multiplicative group* $K^*$, which are defined on $K^*$ and are called (by abuse of language) the *multiplicative* uniformities of $K$.

The uniformity *induced* on $K^*$ by the additive uniformity of $K$ is in general *distinct* from the multiplicative uniformities of $K$ (see Exercise 17).

By Proposition 6, a Hausdorff topological division ring $K$ can be considered as a *dense subring* of a *complete Hausdorff ring* $\hat{K}$. In order that $\hat{K}$ should be a *topological division ring* it is necessary that the mapping

#### Proposition 7 {#top-iii-s6-prop-7 .statement}

*The completion $\hat{K}$ of a Hausdorff topological division ring K is a topological division ring if and only if the image under the mapping $x \to x^{-1}$ of every Cauchy filter (with respect to the additive structure) which does not have a cluster point at 0, is a Cauchy filter (with respect to the additive structure).*

There are topological division rings in which this condition is not satisfied and in which the ring $\hat{K}$ has zero divisors (see Exercise 26). Moreover, even if the completion $\hat{K}$ is a topological division ring, there is no *a priori* reason to assume that the *multiplicative* structures of $\hat{K}$ are structures of a *complete* space. However, this will be the case for division rings K such that $\hat{K}$ is *locally compact* (see Chapter I, § 9, no. 7, Proposition 13, and Chapter III, § 3, no. 3, Proposition 4) and for topological *fields*; for the latter, we have the following proposition:

#### Proposition 8 {#top-iii-s6-prop-8 .statement}

*If the additive uniform structure of a topological field K is a structure of a complete Hausdorff space, then the multiplicative structure on K* is a structure of a complete space.*

We shall show that if $\mathfrak{F}$ is a Cauchy filter with respect to the *multiplicative* structure on K*, then $\mathfrak{F}$ is a Cauchy filter with respect to the *additive* structure on K, and does not converge to 0; this will establish the result. Let U be any neighbourhood of 0 in K, let V be a closed neighbourhood of 0 such that $V \subset U, VV \subset U$ [axiom (AV$_\text{II}$)] and $-1 \notin V$; then by hypothesis there is a set $A \in \mathfrak{F}$ such that, for all $x \in A$ and $y \in A$, we have $x^{-1}y \in 1 + V$. Let $a \in A$, then $A \subset a + aV$, and $a + aV$ is a closed set which does not contain 0; hence 0 is not in the closure of A and is therefore not a cluster point of $\mathfrak{F}$. Let W be a neighbourhood of 0 such that $aW \subset V$ [axiom (AV$_\text{I}$)]; then by hypothesis there is a set $B \in \mathfrak{F}$ such that $B \subset A$ and, for all $x \in B$ and $y \in B$, we have $x^{-1}y \in 1 + W$; hence $y - x \in xW \subset AW \subset aW + aVW$; but K is commutative, and therefore $aVW = aWV \subset VW \subset U$; consequently $y - x \in U + U$ and the Proposition is proved.

The same proof shows that Proposition 8 can be extended to the case in which every Cauchy filter with respect to *one* of the multiplicative structures of K is also a Cauchy filter with respect to the other multiplicative structure.

### Exercises {#top-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
