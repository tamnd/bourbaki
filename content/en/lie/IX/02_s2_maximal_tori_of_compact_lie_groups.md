---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Maximal tori of compact Lie groups
lang: en
source: lie-vii-ix
book_pages: 287-295, 391-394
pdf_pages: 0294-0302, 0398-0401
extraction: native+ocr
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS OF COMPACT ALGEBRAS
      page: 287
      pdf_page: 294
    - "no": 2
      title: MAXIMAL TORI
      page: 288
      pdf_page: 295
    - "no": 3
      title: MAXIMAL TORI OF SUBGROUPS AND QUOTIENT GROUPS
      page: 291
      pdf_page: 298
    - "no": 4
      title: SUBGROUPS OF MAXIMAL RANK
      page: 292
      pdf_page: 299
    - "no": 5
      title: WEYL GROUP
      page: 293
      pdf_page: 300
    - "no": 6
      title: MAXIMAL TORI AND COVERING OF HOMOMORPHISMS
      page: 295
      pdf_page: 302
statements: 32
exercises: 11
content_sha256: 9b6059c982564aa4235b7c9c109f70040d2fb6db104dd21086418462dc06fb2f
---

## § 2. MAXIMAL TORI OF COMPACT LIE GROUPS

### 1. CARTAN SUBALGEBRAS OF COMPACT ALGEBRAS

#### Lemma 1 {#lie-ix-s2-lem-1 .statement tag=019Z}

Let G be a Lie group, K a compact subgroup of G, and F an invariant bilinear form on L(G). Let $x, y\in L(G)$. There exists an element $k$ of K such that $F(u$,[(Ad $k$)$(x), y]) = 0$ for all $u\in L(K)$.

The function $v \rightarrow$ F((Ad $v$)$(x), y$) from K to $\mathbf{R}$ is continuous, and hence has a minimum at some point $k\in K$. Let $u\in L(K)$ and put

$h(t) =$ F((Ad exp($tu$)$.k$)$(x), y$)$,t\in \mathbf{R}$.

We have $h(t)\geq h(0)$ for all $t$; moreover, by Chap. III, §3, no. 12, Prop. 44,

$\frac{dh}{dt}(0) = F([u$,(Ad $k$)$(x)], y) = F(u$,[(Ad $k$)$(x), y])$,

hence the lemma (Functions of a Real Variable, Chap. I, §1, no. 7, Prop. 7).

#### Theorem 1 {#lie-ix-s2-thm-1 .statement tag=01A0}

Let $\mathfrak{g}$ be a compact Lie algebra. The Cartan subalgebras of $\mathfrak{g}$ (Chap. VII, §2, no. 1, Def. 1) are its maximal commutative subalgebras; in particular, $\mathfrak{g}$ is the union of its Cartan subalgebras. The group Int($\mathfrak{g}$) operates transitively on the set of Cartan subalgebras of $\mathfrak{g}$.

Since $\mathfrak{g}$ is reductive, its Cartan subalgebras are commutative (Chap. VII, §2, no. 4, Cor. 3 of Th. 2). Conversely, let $\mathfrak{t}$ be a commutative subalgebra of $\mathfrak{g}$. By §1, no. 3, Prop. 1, ad $x$ is semi-simple for all $x\in \mathfrak{t}$; by Chap. VII, §2, no. 3, Prop. 10, there exists a Cartan subalgebra of $\mathfrak{g}$ containing $\mathfrak{t}$. This proves the first assertion of the theorem.

Now let $\mathfrak{t}$ and $\mathfrak{t}'$ be two Cartan subalgebras of $\mathfrak{g}$. We prove that there exists $u\in$ Int($\mathfrak{g}$) such that $u(\mathfrak{t}) =\mathfrak{t}'$. By Prop. 1 of §1, no. 3, we can assume that $\mathfrak{g}$ is of the form L(G), where G is a connected compact Lie group, and can choose a separating invariant symmetric bilinear form F on $\mathfrak{g}$. Let $x$ (resp. $x'$) be a regular element of $\mathfrak{g}$ such that $\mathfrak{t}=\mathfrak{g}^0(x)$ (resp. $\mathfrak{t}'=\mathfrak{g}^0(x')$) (Chap. VII, §3, no. 3, Th. 2). Applying Lemma 1 with K = G, we see that there exists $k\in G$ such that [(Ad $k$)$(x), x']$ is orthogonal to $\mathfrak{g}$ with respect to F, and hence is zero; then (Ad $k$)$(x)\in \mathfrak{g}^0(x') =\mathfrak{t}'$, so $\mathfrak{g}^0$((Ad $k$)$(x)$) $=\mathfrak{t}'$ since (Ad $k$)$(x)$ is regular. We conclude that (Ad $k$)$(\mathfrak{t}) =\mathfrak{t}'$, hence the theorem.

#### Corollary {#lie-ix-s2-n1-cor-1 .statement tag=01A1}

Let $\mathfrak{t}$ and $\mathfrak{t}'$ be Cartan subalgebras of $\mathfrak{g},\mathfrak{a}$ a subset of $\mathfrak{t}$, and $u$ an automorphism of $\mathfrak{g}$ that takes $\mathfrak{a}$ into $\mathfrak{t}'$. There exists an element $v$ of Int($\mathfrak{g}$) such that $u\circ v$ takes $\mathfrak{t}$ to $\mathfrak{t}'$, and coincides with $u$ on $\mathfrak{a}$.

Put G = Int($\mathfrak{g}$), and consider the fixer $Z_G(\mathfrak{a})$ of $\mathfrak{a}$ in G; this is a Lie subgroup of G, whose Lie algebra $\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$ consists of the elements of $\mathfrak{g}$ that commute with every element of $\mathfrak{a}$ (Chap. III, §9, no. 3, Prop. 7). Then $\mathfrak{t}$ and $u^{-1}(\mathfrak{t}')$ are two Cartan subalgebras of the compact Lie algebra $\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$. By Th. 1, there exists an element $v$ of $Z_G(\mathfrak{a})$ such that $v(\mathfrak{t}) =u^{-1}(\mathfrak{t}')$; any such element has the desired properties.

### 2. MAXIMAL TORI

Let G be a Lie group. A torus of G is a closed subgroup that is a torus (§1, no. 2), in other words any commutative connected compact subgroup. The maximal elements of the set of tori of G, ordered by inclusion, are called the maximal tori of G.

#### Theorem 2 {#lie-ix-s2-thm-2 .statement tag=01A2}

Let G be a connected compact Lie group.

a) The Lie algebras of the maximal tori of G are the Cartan subalgebras of L(G).

b) Let $T_1$ and $T_2$ be two maximal tori of G. There exists $g\in G$ such that $T_2=gT_1g^{-1}$.

c) G is the union of its maximal tori.

Let $\mathfrak{t}$ be a Cartan subalgebra of L(G); the integral subgroup of G whose Lie algebra is $\mathfrak{t}$ is closed (Chap. VII, §2, no. 1, Cor. 4 of Prop. 4) and commutative (Th. 1), and hence is a torus of G. If T is a maximal torus of G, its Lie algebra is commutative, hence is contained in a Cartan subalgebra of L(G) (Th. 1). It follows that the maximal tori of G are exactly the integral subgroups of G associated to the Cartan subalgebras of L(G), hence a). Assertion b) follows from Th. 1, since the canonical homomorphism $G\rightarrow$ Int(L(G)) is surjective (Chap. III, §6, no. 4, Cor. 4 of Prop. 10).

Denote by X the union of the maximal tori of G, and let T be a maximal torus of G. The continuous map $(g, t) \rightarrow gtg^{-1}$ from $G\times T$ to G has image X, which is therefore closed in G; thus, to prove c), it suffices to prove that X is open in G; since X is invariant under inner automorphisms, it suffices to show that, for all $a\in T, X$ is a neighbourhood of $a$. We argue by induction on the dimension of G and distinguish two cases:

$1)a$ is not central in G. Let H be the identity component of the centralizer of $a$ in G; this is a connected compact subgroup of G distinct from G, which contains T, and hence $a$. Since Ad $a$ is semi-simple (§1, no. 1), the Lie algebra of H is the nilspace of Ad $a-1$; it now follows from Chap. VII, §4, no. 2, Prop. 4, that the union Y of the conjugates of H is a neighbourhood of $a$. By the induction hypothesis, $H\subset X$, and hence $Y\subset X$; thus, X is a neighbourhood of $a$.

$2)a$ is central in G. It suffices to prove that $a$ exp $x$ belongs to X for all $x$ in L(G). Now every element $x$ of L(G) belongs to a Cartan subalgebra of G (Th. 1); the corresponding integral subgroup $T'$ contains exp $x$; since it is conjugate to T, it contains $a$ and hence $a$ exp $x$, as required.

#### Corollary 1 {#lie-ix-s2-thm-2-cor-1 .statement tag=01A3}

a) The exponential map of G is surjective.

b) For all $n\geq 1$, the map $g \rightarrow g^n$ from G to itself is surjective.

Indeed, exp(L(G)) contains all the maximal tori of G, hence a). Assertion b) follows from the formula (exp $x$)$^n=$ exp $nx$ for $x$ in L(G).

#### Remark 1 {#lie-ix-s2-n2-rem-1 .statement tag=01A4}

There exists a compact subset K of L(G) such that exp$_G(K) = G$. Indeed, if T is a maximal torus of G, there exists a compact subset $C\subset L(T)$ such that exp$_T(C) = T$; it suffices to take $K =\bigcup_{g\in G}$(Ad $g$)$(C)$.

#### Corollary 2 {#lie-ix-s2-thm-2-cor-2 .statement tag=01A5}

The intersection of the maximal tori of G is the centre of G.

Let $x$ be an element of the centre of G; by Th. $2c)$, there exists a maximal torus T of G containing $x$; then $x$ belongs to all the conjugates of T, hence to all the maximal tori of G. Conversely, if $x$ belongs to all the maximal tori of G, it commutes with every element of G by Th. $2c)$.

#### Corollary 3 {#lie-ix-s2-thm-2-cor-3 .statement tag=01A6}

Let $g\in G$, and let C be its centralizer. Then $g$ belongs to $C_0$; the group $C_0$ is the union of the maximal tori of G containing $g$.

There exists a maximal torus T of G containing $g$ (Th. $2c$)$)$, and hence contained in $C_0$. Moreover, the group $C_0$ is a connected compact Lie group, and hence the union of its maximal tori (Th. $2c$)$)$; these all contain $g$ (Cor. 2), hence are exactly the maximal tori of G containing $g$.

#### Corollary 4 {#lie-ix-s2-thm-2-cor-4 .statement tag=01A7}

Let $g\in G$. If $g$ is regular (Chap. VII, §4, no. 2, Def. 2), it belongs to a unique maximal torus, which is the identity component of its centralizer. Otherwise, it belongs to infinitely-many maximal tori.

Since Ad $g$ is semi-simple, the dimension of the nilspace of Ad $g-1$ is also that of the centralizer C of $g$. By loc. cit., Prop. 8, and Th. $1,g$ is regular if and only if $C_0$ is a maximal torus of G. The conclusion now follows from Cor. 3.

#### Corollary 5 {#lie-ix-s2-thm-2-cor-5 .statement tag=01A8}

a) Let S be a torus of G. The centralizer of S is connected; it is the union of the maximal tori of G containing S.

b) Let $\mathfrak{s}$ be a commutative subalgebra of L(G). The fixer of $\mathfrak{s}$ in G is connected; it is the union of the maximal tori of G whose Lie algebras contain $\mathfrak{s}$.

To prove a), it suffices to prove that if an element $g$ of G centralizes S, there exists a maximal torus of G containing S and $g$. Now, if C is the centralizer of $g$, we have $g\in C_0$ (Cor. 3) and $S\subset C_0$; if T is a maximal torus of the connected compact Lie group $C_0$ containing S, we have $g\in T$ (Cor. 2), hence a). Assertion b) follows from a) applied to the closure of the integral subgroup with Lie algebra $\mathfrak{s}$, in view of Chap. III, §9, no. 3, Prop. 9.

#### Remark 2 {#lie-ix-s2-n2-rem-2 .statement tag=01A9}

It follows from Cor. 5 that a maximal torus of G is a maximal commutative subgroup. The converse is not true: for example, in the group $\mathbf{S}\mathbf{O}(3,\mathbf{R})$, the maximal tori are of dimension 1, and thus cannot contain the subgroup of diagonal matrices, which is isomorphic to $(\mathbf{Z}/2\mathbf{Z})^2$. Moreover, if $g\in \mathbf{S}\mathbf{O}(3,\mathbf{R})$ is a non-scalar diagonal matrix, $g$ is a regular element of $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ whose centralizer is not connected (cf. Cor. 4).

#### Corollary 6 {#lie-ix-s2-thm-2-cor-6 .statement tag=01AA}

The maximal tori of G are their own centralizers, and are the fixers of their Lie algebras.

Let T be a maximal torus of G and C its centralizer; since L(T) is a Cartan subalgebra of L(G), we have L(T) = L(C), hence C = T since C is connected (Cor. 5).

#### Corollary 7 {#lie-ix-s2-thm-2-cor-7 .statement tag=01AB}

Let T and $T'$ be two maximal tori of G, A a subset of T and $s$ an automorphism of G that takes A into $T'$. There exists $g\in G$ such that $s\circ$ (Int $g$) takes T to $T'$ and coincides with $s$ on A.

Let C be the centralizer of A. Then T and $s^{-1}(T')$ are two maximal tori of $C_0$; every element $g$ of $C_0$ such that (Int $g$)$(T) =s^{-1}(T')$ has the desired properties.

#### Corollary 8 {#lie-ix-s2-thm-2-cor-8 .statement tag=01AC}

Let H be a compact Lie group, T a maximal torus of H. Then $H = N_H(T).H_0$, and the injection of $N_H(T)$ into H induces an isomorphism from $N_H(T)/N_{H_0}(T)$ to $H/H_0$.

Let $h\in H$. Then $h^{-1}Th$ is a maximal torus of $H_0$, hence (Th. 2) there exists $g\in H_0$ such that $hg\in N_H(T)$; thus $h$ belongs to $N_H(T).H_0$, hence the first assertion. The second follows immediately.

#### Remark 3 {#lie-ix-s2-n2-rem-3 .statement tag=01AD}

Let G be a connected Lie group whose Lie algebra is compact. The Cartan subgroups of G are the integral subgroups whose Lie algebras are the Cartan subalgebras of L(G) (the Cartan subgroups of a connected compact group are thus its maximal tori). Theorem 2 and its corollaries remain valid for G, if we replace everywhere the expression “maximal torus” by “Cartan subgroup”. This follows immediately from the fact that, in view of Prop. 5 of §1, no. 4, G is the direct product of a vector group V and a connected compact group K and that the Cartan subgroups of G are the products of V with the maximal tori of K. Moreover, note that it follows from Cor. 6 above that the Cartan subgroups of G can also be defined as the fixers of the Cartan subalgebras of L(G).

$^*4)$ Part c) of Theorem 2 can also be proved in the following way. Give G an invariant riemannian metric (§1, no. 3, Prop. 3). Then, for any element $g$ of G, there exists a maximal geodesic passing through $g$ and the identity element of G (Hopf-Rinow theorem), and it can be verified that the closure of such a geodesic is a subtorus of $G._*$

### 3. MAXIMAL TORI OF SUBGROUPS AND QUOTIENT GROUPS

#### Proposition 1 {#lie-ix-s2-prop-1 .statement tag=01AE}

Let G and $G'$ be two connected compact Lie groups.

a) Let $f: G\rightarrow G'$ be a surjective morphism of Lie groups. The maximal tori of $G'$ are the images under $f$ of the maximal tori of G. If the kernel of $f$ is central in G (for example discrete), the maximal tori of G are the inverse images under $f$ of the maximal tori of $G'$.

b) Let H be a connected closed subgroup of G. Every maximal torus of H is the intersection with H of a maximal torus of G.

c) Let H be a connected closed normal subgroup of G. The maximal tori of H are the intersections with H of the maximal tori of G.

a) Let T be a maximal torus of G; then L(T) is a Cartan subalgebra of L(G) (no. 2, Th. $2a$)$)$, so $L(f(T))$ is a Cartan subalgebra of $L(G')$ (Chap. VII, §2, no. 1, Cor. 2 of Prop. 4); it follows that $f(T)$ is a maximal torus of $G'$ (no. 2, Th. $2a$)$)$. If Ker $f$ is central in G, it is contained in T (Cor. 2 of Th. 2), so $T =f^{-1}(f(T))$.

Conversely, let $T'$ be a maximal torus of $G'$; we show that there exists a maximal torus T of G such that $f(T) = T'$. Let $T_1$ be a maximal torus of G; then $f(T_1)$ is a maximal torus of $G'$ and there exists $g'\in G'$ such that $T'=g'f(T_1)g^{'-1}$ (Th. $2b$)$)$; if $g\in G$ is such that $f(g) =g'$, we have $T'=f(T)$ with $T =gT_1g^{-1}$.

b) Let S be a maximal torus of H; this is a torus of G so there exists a maximal torus T of G containing S. Then $T\cap H$ is a commutative subgroup of H containing S, hence is equal to S (no. 2, Remark 2).

c) By §1, no. 3, Prop. $2c), L(G)$ is the direct product of L(H) with an ideal; thus, the Cartan subalgebras of L(H) are the intersections with L(H) of the Cartan subalgebras of L(G). Thus, for any maximal torus T of $G, T\cap H$ contains a maximal torus S of H and $S = T\cap H$ (no. 2, Remark 2).

#### Remark 1 {#lie-ix-s2-n3-rem-1 .statement tag=01AF}

Proposition 1 generalizes immediately to connected groups with compact Lie algebras. In particular, if G is a connected Lie group whose Lie algebra is compact, the Cartan subgroups of G (cf. Remark 3, no. 2) are exactly the inverse images of the maximal tori of the connected compact Lie group Ad(G) (under the canonical homomorphism from G to Ad(G)).

#### Remark 2 {#lie-ix-s2-n3-rem-2 .statement tag=01AG}

Let G be a connected compact Lie group, $\widetilde{D}(G)$ the universal covering of the group D(G) and $f: \widetilde{D}(G)\rightarrow G$ the composite of the canonical morphisms from $\widetilde{D}(G)$ to D(G) and from D(G) to G. Then the map $T\rightarrow f^{-1}(T)$ is a bijection from the set of maximal tori of G to the set of maximal tori of $\widetilde{D}(G)$; the inverse bijection associates to a maximal torus $\widetilde{T}$ of $\widetilde{D}(G)$ the maximal torus $C(G)_0.f( \widetilde{T})$ of G.

### 4. SUBGROUPS OF MAXIMAL RANK

We shall call the rank of a connected Lie group G the rank of its Lie algebra, and we shall denote it by rk G. By Th. 2 a), the rank of a connected compact Lie group is the common dimension of its maximal tori.

Let G be a connected compact Lie group and H a closed subgroup of G. If H is connected, then rk $H\leq$ rk G (since the maximal tori of H are tori in G). By Th. 2 c), to say that H is connected and of maximal rank (that is, of rank rk G) means that H is a union of maximal tori of G. We deduce immediately from Proposition 1:

#### Proposition 2 {#lie-ix-s2-prop-2 .statement tag=01AH}

Let $f$ : G $\rightarrow G'$ be a surjective morphism of connected compact Lie groups whose kernel is central. The maps $H \rightarrow f(H)$ and $H' \rightarrow f^{-1}(H')$ are inverse bijections between the set of connected closed subgroups of G of maximal rank and the analogous set for $G'$.

#### Proposition 3 {#lie-ix-s2-prop-3 .statement tag=01AI}

Let G be a connected compact Lie group, and H a connected closed subgroup of maximal rank.

a) The compact manifold $G/H$ is simply-connected.

b) The homomorphism $\pi_1(H)\rightarrow \pi_1(G)$, induced by the canonical injection of H into G, is surjective.

Since H is connected, we have an exact sequence (General Topology, Chap. XI, in preparation)

$$
\pi_1(H)\rightarrow \pi_1(G)\rightarrow \pi_1(G/H,\overline{e})\rightarrow 0
$$

where $\overline{e}$ is the image in $G/H$ of the identity element of G. Since $G/H$ is connected, this immediately implies the equivalence of assertions a) and b). Moreover, if $f: G'\rightarrow G$ is a surjective morphism of connected compact Lie groups whose kernel is central, proving the proposition (in the form $a$)$)$ for G is the same as proving it for $G'$ (Prop. 2). Thus, we can first of all replace G by Ad(G), then assume that G is semi-simple, and then by replacing G by a universal covering (§1, no. 4, Cor. 2), assume that G is simply-connected. But then assertion b) is trivial.

#### Proposition 4 {#lie-ix-s2-prop-4 .statement tag=01AJ}

Let G be a compact Lie group, H a connected closed subgroup of G of maximal rank and N the normalizer of H in G. Then H is of finite index in N and is the identity component of N.

Indeed, the Lie algebra of H contains a Cartan subalgebra of L(G). Thus, by Chap. VII, §2, no. 1, Cor. 4 of Prop. 4, H is the identity component of N. Since N is compact, H is of finite index in N.

#### Remark 1 {#lie-ix-s2-n4-rem-1 .statement tag=01AK}

Every integral subgroup H of G such that rk H = rk G is closed: indeed, the preceding proof shows that H is the identity component of its normalizer, which is a closed subgroup of G.

#### Remark 2 {#lie-ix-s2-n4-rem-2 .statement tag=01AL}

With the notations of Prop. 4, every closed subgroup $H'$ of G containing H and such that $(H': H)$ is finite normalizes H, and hence is contained in N; similarly, the normalizer of $H'$ is contained in N. In particular, N is its own normalizer.

### 5. WEYL GROUP

Let G be a connected compact Lie group and T a maximal torus of G. Denote by $N_G(T)$ the normalizer of T in G; by Prop. 4 (no. 4), the quotient group $N_G(T)/T$ is finite. We denote it by $W_G$(T), or by W(T), and call it the Weyl group of the maximal torus T of G, or the Weyl group of G relative to T. Since T is commutative, the operation of $N_G(T)$ on T by inner automorphisms of G induces by passage to the quotient an operation, called the canonical operation, of the group $W_G(T)$ on the Lie group T. By Cor. 6 of Th. 2 of no. 2, this operation is faithful: the associated homomorphism $W_G(T)\rightarrow$ Aut T is injective.

If $T'$ is another maximal torus of G and if $g\in G$ is such that Int $g$ maps T to $T'$ (no. 2, Th. $2b$)$)$, then Int $g$ induces an isomorphism $a_g$ from $W_G(T)$ to $W_G(T')$ and $a_g(s)(gtg^{-1}) =gs(t)g^{-1}$ for all $s\in W_G(T)$ and all $t\in T$.

#### Proposition 5 {#lie-ix-s2-prop-5 .statement tag=01J9}

$a)$ Every conjugacy class of G meets T.

b) The intersections with T of the conjugacy classes of G are the orbits of the Weyl group.

Let $g\in G$; by Th. 2 of no. 2, there exists $h\in G$ such that $g\in hTh^{-1}$, hence a). By definition of the Weyl group, any two elements in the same orbit of $W_G(T)$ on T are conjugate in G; conversely, let $a, b$ be two elements of T conjugate under G. There exists $h\in G$ such that $b=hah^{-1}$; applying Cor. 7 of Th. 2 (no. 2) with $A =\{a\},s=$ Int $h, T'= T$, we see that there exists $g\in G$ such that Int $hg$ maps T to T and $a$ to $b$. The class of $hg$ in $W_G(T)$ then maps $a$ to $b$, hence the proposition.

#### Corollary 1 {#lie-ix-s2-prop-5-cor-1 .statement tag=01JA}

The canonical injection of T into G defines by passage to the quotient a homeomorphism from $T/W_G(T)$ to the space $G/$Int(G) of conjugacy classes of G.

Indeed, this is a bijective continuous map between two compact spaces (cf. General Topology, Chap. III, p. 29, Cor. 1).

#### Corollary 2 {#lie-ix-s2-prop-5-cor-2 .statement tag=01JB}

Let E be a subset of G stable under inner automorphisms. Then E is open (resp. closed, resp. dense) in G if and only if $E\cap T$ is open (resp. closed, resp. dense) in T.

This follows from Cor. 1 and the fact that the canonical maps $\mathrm{T}\to \mathrm{T}/\mathrm{W}_{G}(\mathrm{T})$ and $\mathrm{G}\to \mathrm{G}/\mathrm{Int}(\mathrm{G})$ are open (*General Topology*, Chap. III, p. 10, Lemma 2).

Denote the Lie algebra of $\mathrm{G}$ by $\mathfrak{g}$, and that of $\mathrm{T}$ by $\mathfrak{t}$. The operation of $\mathrm{W}_{G}(\mathrm{T})$ on $\mathrm{T}$ induces a representation, called the *canonical representation*, of the group $\mathrm{W}_{G}(\mathrm{T})$ on the $\mathbf{R}$-vector space $\mathfrak{t}$.

#### Proposition 6 {#lie-ix-s2-prop-6 .statement tag=01JC}

a) *Every orbit of $\mathrm{G}$ on $\mathfrak{g}$ (for the adjoint representation) meets $\mathfrak{t}$.*

b) *The intersections with $\mathfrak{t}$ of the orbits of $\mathrm{G}$ are the orbits of $\mathrm{W}_{G}(\mathrm{T})$ on $\mathfrak{t}$.*

Assertion a) follows from Th. 1 (no. 1). Let $x,y$ be two elements of $\mathfrak{t}$ conjugate under $\mathrm{Ad}(\mathrm{G})$, and let $h\in\mathrm{G}$ be such that $(\mathrm{Ad}\,h)(x)=y$. Applying the corollary of Th. 1 (no. 1) with $\mathfrak{a}=\{x\}$, $u=\mathrm{Ad}\,h$, $\mathfrak{t}'=\mathfrak{t}$, we see that there exists $g\in\mathrm{G}$ such that $\mathrm{Ad}\,hg$ maps $\mathfrak{t}$ to $\mathfrak{t}$ and $x$ to $y$. Then $hg\in\mathrm{N}_{G}(\mathrm{T})$ (Chap. III, §9, no. 4, Prop. 11), and the class of $hg$ in $\mathrm{W}_{G}(\mathrm{T})$ maps $x$ to $y$, hence the proposition.

#### Corollary {#lie-ix-s2-n5-cor-1 .statement tag=01JD}

*The canonical injection of $\mathfrak{t}$ into $\mathfrak{g}$ defines by passage to the quotient a homomorphism from $\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T})$ to $\mathfrak{g}/\mathrm{Ad}(\mathrm{G})$.*

Denote this map by $j$; it is bijective and continuous (Prop. 6). We have a commutative diagram

$$
\begin{array}{ccc}
\mathfrak{t} & \xrightarrow{\ i\ } & \mathfrak{g} \\
{\scriptstyle p}\downarrow\phantom{{\scriptstyle p}} & & \phantom{{\scriptstyle q}}\downarrow{\scriptstyle q} \\
\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T}) & \xrightarrow{\ j\ } & \mathfrak{g}/\mathrm{Ad}(\mathrm{G})
\end{array}
$$

where $p$ and $q$ are quotient maps, and $i$ is the canonical injection. Since $i$ and $q$ are proper (*General Topology*, Chap. I, §10, no. 1, Prop. 2 and *General Topology*, Chap. III, §4, no. 1, Prop. 2 c)) and since $p$ is surjective, it follows that $j$ is proper (*General Topology*, Chap. I, §10, no. 1, Prop. 5), and hence is a homeomorphism.

#### Proposition 7 {#lie-ix-s2-prop-7 .statement tag=01JE}

*Let $H$ be a closed subgroup of $\mathrm{G}$ containing $\mathrm{T}$.*

a) *Denote by $\mathrm{W}_{H}(\mathrm{T})$ the subgroup $\mathrm{N}_{H}(\mathrm{T})/\mathrm{T}$ of $\mathrm{W}_{G}(\mathrm{T})$; the group $H/H_{0}$ is isomorphic to the quotient group $\mathrm{W}_{H}(\mathrm{T})/\mathrm{W}_{H_{0}}(\mathrm{T})$.*

b) *$H$ is connected if and only if every element of $\mathrm{W}_{G}(\mathrm{T})$ that has a representative in $H$ belongs to $\mathrm{W}_{H_{0}}(\mathrm{T})$.*

Assertion a) follows from Cor. 8 of Th. 2 (no. 2), and assertion b) is a particular case of a).

### 6. MAXIMAL TORI AND COVERING OF HOMOMORPHISMS

Let G be a connected compact Lie group, T a maximal torus of G. Consider the derived group D(G) of G and its universal covering $\widetilde{D}(G)$; let $p: \widetilde{D}(G)\rightarrow G$ be the composite of the canonical morphisms $\widetilde{D}(G)\rightarrow D(G)$ and $D(G)\rightarrow G$. Then $\widetilde{D}(G)$ is a connected compact Lie group (§1, no. 4, Cor. 2 of Prop. 4); moreover, the inverse image $\widetilde{T}$ of T under $p$ is a maximal torus of $\widetilde{D}(G)$ (no. 3, Prop. 1).

#### Lemma 2 {#lie-ix-s2-lem-2 .statement tag=01AO}

Let H be a Lie group, $f_T: T\rightarrow H$ and $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ morphisms of Lie groups such that $f_T(p(t)) = \widetilde{f}(t)$ for all $t\in \widetilde{T}$. There exists a unique morphism of Lie groups $f: G\rightarrow H$ such that $f\circ p= \widetilde{f}$ and such that the restriction of $f$ to T is $f_T$.

Put $Z = C(G)_0$; by §1, no. 4, Cor. 1 of Prop. 4, the morphism of Lie groups $g: Z\times \widetilde{D}(G)\rightarrow G$ such that $g(z, x) =z^{-1}p(x)$ is a covering; its kernel consists of the pairs $(z, x)$ such that $p(x) =z$, for which $x\in p^{-1}(Z)\subset \widetilde{T}$. Since the morphism $(z, x) \rightarrow f_T(z^{-1}) \widetilde{f}(x)$ from $Z\times \widetilde{D}(G)$ to H maps Ker $g$ to $\{e\}$, there exists a morphism $f$ from G to H such that $f\circ p= \widetilde{f}$ and $f(z) =f_T(z)$ for $z\in Z$. But we also have $f(t) =f_T(t)$ for $t\in p( \widetilde{T})$; since $T = Z.p( \widetilde{T})$, the restriction of $f$ to T is indeed $f_T$.

#### Proposition 8 {#lie-ix-s2-prop-8 .statement tag=01AP}

Let G be a connected compact Lie group, T a maximal torus of G, H a Lie group and $\varphi : L(G)\rightarrow L(H)$ a homomorphism of Lie algebras. There exists a morphism of Lie groups $f: G\rightarrow H$ such that $L(f) =\varphi$ if and only if there exists a morphism of Lie groups $f_T: T\rightarrow H$ such that $L(f_T) =\varphi |L(T)$; then $f_T=f|T$.

If $f: G\rightarrow H$ is a morphism of Lie groups such that $L(f) =\varphi$, the restriction $f_T$ of $f$ to T is the unique morphism from T to H such that $L(f_T) =\varphi |L(T)$. Conversely, let $f_T: T\rightarrow H$ be a morphism of Lie groups such that $L(f_T) =\varphi |L(T)$. Let $\widetilde{D}(G)$ and $p$ be as above; the map $L(p)$ induces an isomorphism from $L( \widetilde{D}(G))$ to the derived algebra $\mathfrak{b}$ of L(G). There exists a morphism of Lie groups $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ such that $L( \widetilde{f}) = (\varphi |\mathfrak{b})\circ L(p)$ (Chap. III, §6, no. 1, Th. 1). The morphisms $t \rightarrow \widetilde{f}(t)$ and $t \rightarrow f_T(p(t))$ from $\widetilde{T}$ to H induce the same homomorphism of Lie algebras, and hence coincide. Applying Lemma 2, we deduce the existence of a morphism $f: G\rightarrow H$ such that $L(f)$ and $\varphi$ coincide on L(T) and $\mathfrak{b}$. Since $L(G) =\mathfrak{b}+ L(T)$, we have $L(f) =\varphi$.

#### Proposition 9 {#lie-ix-s2-prop-9 .statement tag=01AQ}

Let G be a connected compact Lie group, T a maximal torus of G, H a Lie group and $f: G\rightarrow H$ a morphism. Then $f$ is injective if and only if its restriction to T is injective.

Indeed, by Th. 2 (no. 2) the normal subgroup Ker $f$ of G reduces to the identity element if and only if its intersection with T reduces to the identity element.

### Exercises {#lie-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
