---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 4
section_title: Root system associated to a compact group
lang: en
source: lie-vii-ix
book_pages: 304-324, 396-405
pdf_pages: 0311-0331, 0403-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: THE GROUP X(H)
      page: 304
      pdf_page: 311
    - "no": 2
      title: NODAL GROUP OF A TORUS
      page: 305
      pdf_page: 312
    - "no": 3
      title: WEIGHTS OF A LINEAR REPRESENTATION
      page: 307
      pdf_page: 314
    - "no": 4
      title: ROOTS
      page: 309
      pdf_page: 316
    - "no": 5
      title: NODAL VECTORS AND INVERSE ROOTS
      page: 311
      pdf_page: 318
    - "no": 6
      title: FUNDAMENTAL GROUP
      page: 314
      pdf_page: 321
    - "no": 7
      title: SUBGROUPS OF MAXIMAL RANK
      page: 316
      pdf_page: 323
    - "no": 8
      title: ROOT DIAGRAMS
      page: 317
      pdf_page: 324
    - "no": 9
      title: COMPACT LIE GROUPS AND ROOT SYSTEMS
      page: 319
      pdf_page: 326
    - "no": 10
      title: AUTOMORPHISMS OF A CONNECTED COMPACT LIE GROUP
      page: 322
      pdf_page: 329
statements: 60
exercises: 22
content_sha256: 78aa365c4ece2d56abd81140632766ec3df87d38b97b4dc5d6d9fda5d7866513
---

## § 4. ROOT SYSTEM ASSOCIATED TO A COMPACT GROUP

In paragraphs 4 to 8, we denote by G a connected compact Lie group and by T a maximal torus of G. We denote by $\mathfrak{g}$ (resp. $\mathfrak{t}$) the Lie algebra of G (resp. T), by $\mathfrak{g}_{\mathbf{C}}$ (resp. $\mathfrak{t}_{\mathbf{C}}$) the complexified Lie algebra of $\mathfrak{g}$ (resp. $\mathfrak{t}$), and by W the Weyl group of G relative to T (§2, no. 5).

### 1. THE GROUP X(H)

Let H be a compact Lie group. Denote by X(H) the (commutative) group of continuous homomorphisms from H to the topological group $\mathbf{C}^*$. By Chap. III, §8, no. 1, Th. 1, the elements of X(H) are morphisms of Lie groups; for all $a\in X(H)$, the differential of $a$ is an $\mathbf{R}$-linear map $L(a) : L(H)\rightarrow L(\mathbf{C}^*)$. From now on we identify the Lie algebra of $\mathbf{C}^*$ with $\mathbf{C}$ in such a way that the exponential map of $\mathbf{C}^*$ coincides with the map $z \rightarrow e^z$ from $\mathbf{C}$ to $\mathbf{C}^*$. Then, to any element $a\in X(H)$ is associated an element $L(a)\in$ Hom$_{\mathbf{R}}(L(H),\mathbf{C})$; we denote by $\delta (a)$ the element of Hom$_{\mathbf{C}}(L(H)_{(\mathbf{C})},\mathbf{C})$ that corresponds to it (that is, whose restriction to $L(H)\subset L(H)_{(\mathbf{C})}$ is equal to $L(a)$).

For all $x\in L(H)$ and all $a\in X(H)$, we have

$a$(exp$_Hx$) $=e^{\delta(a)(x)}$,

by functoriality of the exponential map (Chap. III, §6, no. 4, Prop. 10).

We shall often denote the group X(H) additively; in that case, we denote the element $a(g)$ of $\mathbf{C}^*$ by $g^a$. With this notation, we have the formulas

$$
g^{a+b}=g^ag^b,g\in H, a, b\in X(H)
$$

and

(exp$_Hx$)$^a=e^{\delta(a)(x)}, x\in L(H), a\in X(H)$.

Since H is compact, the elements of X(H) take values in the subgroup $\mathbf{U}=\mathbf{U}(1,\mathbf{C})$ of complex numbers of absolute value 1, so that X(H) can be identified with the group of continuous (or analytic) homomorphisms from H to $\mathbf{U}$. It follows that, for all $a\in L(H)$, the map $L(a)$ takes values in the subspace $\mathbf{R}i$ of $\mathbf{C}$, so $\delta (a)$ maps L(H) to $\mathbf{R}i$.

If H is commutative, X(H) is simply the (discrete) dual group of H (Spectral Theories, Chap. II, §1, no. 1). If H is commutative and finite, X(H) can be identified with the dual finite group D(H) = Hom$_{\mathbf{Z}}(H,\mathbf{Q}/\mathbf{Z})$ (where, as in Algebra, Chap. VII, §4, no. 9, Example 1, we identify $\mathbf{Q}/\mathbf{Z}$ with a subgroup of $\mathbf{C}^*$ by the homomorphism $r \rightarrow$ exp(2$\pi ir$)).

For any morphism $f: H\rightarrow H'$ of compact Lie groups, we denote by $X(f)$ the homomorphism $a \rightarrow a\circ f$ from $X(H')$ to X(H). If K is a closed

normal subgroup of the compact Lie group H, we have an exact sequence of $\mathbf Z$-modules
$$
0\longrightarrow X(H/K)\longrightarrow X(H)\longrightarrow X(K).
$$

#### Proposition 1 {#lie-ix-s4-prop-1 .statement tag=01JH}

— *For any compact Lie group* H, *the* $\mathbf Z$-*module* $X(H)$ *is of finite type. It is free if* H *is connected.*

Assume first that H is connected; every element of $X(H)$ vanishes on the derived group $D(H)$ of H, hence we have a homomorphism $X(H/D(H))\longrightarrow X(H)$. But $H/D(H)$ is connected and commutative, hence is a torus, and $X(H/D(H))$ is a free $\mathbf Z$-module of finite type (*Spectral Theories*, Chap. II, §2, no. 1, Cor. 2 of Prop. 1). In the general case, it follows from the exactness of the sequence
$$
0\longrightarrow X(H/H_0)\longrightarrow X(H)\longrightarrow X(H_0),
$$
where $X(H_0)$ is free of finite type and $X(H/H_0)$ is finite, that $X(H)$ is of finite type.

#### Proposition 2 {#lie-ix-s4-prop-2 .statement tag=01JI}

— *Let* H *be a commutative compact Lie group, and* $(a_i)_{i\in I}$ *a family of elements of* $X(H)$; *the* $a_i$ *generate* $X(H)$ *if and only if the intersection of the* $\operatorname{Ker}a_i$ *reduces to the identity element.*

By *Spectral Theories*, Chap. II, §1, no. 7, Th. 4, the orthogonal complement of the kernel of $a_i$ is the subgroup $A_i$ of $X(H)$ generated by $a_i$; by *loc. cit.*, Cor. 2 of Th. 4, the orthogonal complement of $\bigcap\operatorname{Ker}a_i$ is the subgroup of $X(H)$ generated by the $A_i$, hence the proposition.

### 2. NODAL GROUP OF A TORUS

The *nodal group* of a torus S, denoted by $\Gamma(S)$, is the kernel of the exponential map $\mathscr L(S)\longrightarrow S$. This is a discrete subgroup of $\mathscr L(S)$, whose rank is equal to the dimension of S, and the $\mathbf R$-linear map $\mathbf R\otimes_{\mathbf Z}\Gamma(S)\longrightarrow\mathscr L(S)$ that extends the canonical injection of $\Gamma(S)$ into $\mathscr L(S)$ is bijective. It induces by passage to the quotient an isomorphism
$$
\mathbf R/\mathbf Z\otimes_{\mathbf Z}\Gamma(S)\longrightarrow S.
$$

For example, the nodal group $\Gamma(\mathbf U)$ of $\mathbf U$ is the subgroup $2\pi i\mathbf Z$ of $\mathscr L(\mathbf U)=i\mathbf R$.

For any morphism of tori $f:S\longrightarrow S'$, denote by $\Gamma(f)$ the homomorphism $\Gamma(S)\longrightarrow\Gamma(S')$ induced by $L(f)$. We have a commutative diagram
$$
\begin{array}{ccccccccc}
0&\longrightarrow&\Gamma(S)&\longrightarrow&\mathscr L(S)&\xrightarrow{\exp_S}&S&\longrightarrow&0\\
&&\downarrow{\Gamma(f)}&&\downarrow{\mathscr L(f)}&&\downarrow f&&\\
0&\longrightarrow&\Gamma(S')&\longrightarrow&\mathscr L(S')&\xrightarrow{\exp_{S'}}&S'&\longrightarrow&0.
\end{array}
\tag{1}
$$

Let $a\in X(S)$; applying the preceding to the morphism from S to $\mathbf U$ defined by a, we see that the $\mathbf C$-linear map $\delta(a):\mathscr L(S)_{\mathbf C}\longrightarrow\mathbf C$ of no. 1 maps $\Gamma(S)$ to $2\pi i\mathbf Z$. Thus, we can define a $\mathbf Z$-bilinear form on $X(S)\times\Gamma(S)$ by putting
$$
\langle a,X\rangle=\frac{1}{2\pi i}\delta(a)(X),\qquad a\in X(S),\quad X\in\Gamma(S).
\tag{2}
$$

#### Proposition 3 {#lie-ix-s4-prop-3 .statement tag=01BP}

The bilinear form $(a, X) \rightarrow  \langle a, X\rangle$ on $X(S)\times \Gamma (S)$ is invertible.

Recall (Algebra, Chap. IX) that, by definition, this means that the linear maps $X(S)\rightarrow$ Hom$_{\mathbf{Z}}(\Gamma (S),\mathbf{Z})$ and $\Gamma (S)\rightarrow$ Hom$_{\mathbf{Z}}(X(S),\mathbf{Z})$ associated to this bilinear form are bijective.

It is immediate that if the conclusion of the proposition is true for two tori, it is also true for their product. Thus, since every torus of dimension $n$ is isomorphic to $\mathbf{U}^n$, we are reduced to the case in which $S =\mathbf{U}$. In this particular case, the assertion is immediate.

Let $f: S\rightarrow S'$ be a morphism of tori. Then, each of the linear maps $X(f) : X(S')\rightarrow X(S)$ and $\Gamma (f) :\Gamma (S)\rightarrow \Gamma (S')$ is the transpose of the other: for all $a'\in X(S')$ and all $X\in \Gamma$(S),

$$
\langle X(f)(a'), X\rangle =\langle a', \Gamma (f)(X)\rangle \tag{3}
$$

#### Proposition 4 {#lie-ix-s4-prop-4 .statement tag=01BQ}

Let S and $S'$ be tori. Denote by $M(S,S')$ the group of morphisms of Lie groups from S to $S'$. The maps $f \rightarrow X(f)$ and $f \rightarrow \Gamma (f)$ are isomorphisms of groups from $M(S,S')$ to Hom$_{\mathbf{Z}}(X(S'),X(S))$ and to Hom$_{\mathbf{Z}}(\Gamma (S), \Gamma (S'))$, respectively.

If $f$ is a morphism of Lie groups from S to $S'$, the homomorphism $X(f)$ is simply the dual of $f$ in the sense of Spectral Theories, Chap. II, §1, no. 7. The map $\varphi  \rightarrow \widehat{\varphi}$ from Hom$_{\mathbf{Z}}(X(S'),X(S))$ to $M(S,S')$ defined in loc. cit. is the inverse of the map $f \rightarrow X(f)$ from $M(S,S')$ to Hom$_{\mathbf{Z}}(X(S'),X(S))$; the latter is thus bijective. If we identify $\Gamma (S)$ (resp. $\Gamma (S')$) with the dual $\mathbf{Z}$-module of X(S) (resp. $X(S')$) (Prop. $3$)$,\Gamma (f)$ coincides with the transpose of the homomorphism $X(f)$, hence the proposition.

#### Remark 1 {#lie-ix-s4-n2-rem-1 .statement tag=01BR}

Let $f$ : S $\rightarrow S'$ be a morphism of tori. The snake diagram (Algebra, Chap. X, §1, no. 2) associated to (1) gives an exact sequence

0 $\longrightarrow$ Ker$\Gamma (f)\longrightarrow$ Ker $L(f)\longrightarrow$ Ker $f\longrightarrow^d$ (4)

$\longrightarrow^d$ Coker $\Gamma (f)\longrightarrow$ Coker $L(f)\longrightarrow$ Coker $f\longrightarrow 0$.

In particular, assume that $f$ is surjective, with finite kernel N, so that we have an exact sequence

0 $\longrightarrow$ N $\longrightarrow^i$ S $\longrightarrow^fS'\longrightarrow 0$,

where $i$ is the canonical injection. Then, $L(f)$ is bijective, and (4) gives an isomorphism $N\rightarrow$ Coker $\Gamma (f)$, hence an exact sequence

0 $\longrightarrow \Gamma (S)\overset{\Gamma(f)}{\longrightarrow}\Gamma (S')\longrightarrow$ N $\longrightarrow 0$. (5)

Moreover, by Spectral Theories, Chap. II, §1, no. 7, Th. 4, the sequence

0 $\longrightarrow X(S')\overset{X(f)}{\longrightarrow}$ X(S) $\longrightarrow^{X(i)}$ X(N) $\longrightarrow$ 0 (6)

is exact.

#### Remark 2 {#lie-ix-s4-n2-rem-2 .statement tag=01BS}

By Prop. 4, the map $f \rightarrow \Gamma (f)(2\pi i)$ from $M(\mathbf{U},S)$ to $\Gamma (S)$ is an isomorphism; if $a\in X(S) = M(S,\mathbf{U})$ and $f\in M(\mathbf{U},S)$, then the composite $a\circ f\in M(\mathbf{U},\mathbf{U})$ is the endomorphism $u \rightarrow u^r$, where $r=\langle a, \Gamma (f)(2\pi i)\rangle$. We shall identify $M(\mathbf{U},\mathbf{U}) = X(\mathbf{U})$ with $\mathbf{Z}$ from now on, the element $r$ of $\mathbf{Z}$ being associated to the endomorphism $u \rightarrow u^r$; thus, with the notations above,

$$
a\circ f=\langle a, \Gamma (f)(2\pi i)\rangle
$$

#### Remark 3 {#lie-ix-s4-n2-rem-3 .statement tag=01BT}

To the exact sequence $0\rightarrow \Gamma (S)\rightarrow L(S)\longrightarrow^{exp_S}S\rightarrow 0$ is associated an isomorphism from $\Gamma (S)$ to the fundamental group of S, called canonical in the sequel. For any morphism of tori $f: S\rightarrow S',\Gamma (f)$ can then be identified via the canonical isomorphisms $\Gamma (S)\rightarrow \pi_1(S)$ and $\Gamma (S')\rightarrow \pi_1(S')$ with the homomorphism $\pi_1(f) :\pi_1(S)\rightarrow \pi_1(S')$ induced by $f$. Note that this gives another interpretation of the exact sequence (5) (cf. General Topology, Chap. XI, in preparation).

#### Remark 4 {#lie-ix-s4-n2-rem-4 .statement tag=01BU}

The homomorphisms of $\mathbf{Z}$-modules $\delta : X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$ and $\iota :\Gamma (S)\rightarrow L(S)_{(\mathbf{C})}(\iota$ is induced by the canonical injection of $\Gamma (S)$ into L(S)) extend to isomorphisms of $\mathbf{C}$-vector spaces

$u:\mathbf{C}\otimes X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$

$$
v:\mathbf{C}\otimes \Gamma (S)\rightarrow L(S)_{(\mathbf{C})}
$$

which we shall call canonical in the sequel. Note that, if we extend the pairing between X(S) and $\Gamma (S)$ by $\mathbf{C}$-linearity to a bilinear form $\ll ,\gg$ on $(\mathbf{C}\otimes X(S))\times (\mathbf{C}\otimes \Gamma$(S)), then

$$
\langle u(a), v(b)\rangle = 2\pi i\ll a, b\gg
$$

### 3. WEIGHTS OF A LINEAR REPRESENTATION

In this number $k$ denotes one of the fields $\mathbf{R}$ or $\mathbf{C}$.

Let V be a finite dimensional vector space over $k$, and $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ a continuous (hence real-analytic, Chap. III, §8, no. 1, Th. 1) representation of the connected compact Lie group G on V. Define a complex vector space $\widetilde{V}$ and a continuous representation $\widetilde{\rho}: G\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ as follows: if $k=\mathbf{C}$, set $\widetilde{V} = V, \widetilde{\rho}=\rho$; if $k=\mathbf{R}$, set $\widetilde{V} = V_{(\mathbf{C})}$ and $\widetilde{\rho}$ to be the composite of $\rho$ with the canonical homomorphism $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$.

For all $\lambda \in X(G)$, denote by $\widetilde{V}_{\lambda}(G)$ the vector subspace of $\widetilde{V}$ consisting of the $v\in \widetilde{V}$ such that $\widetilde{\rho}(g)v=g^{\lambda}v$ for all $g\in G$ (cf. Chap. VII, §1, no. 1). By loc. cit., Prop. 3, the sum of the $\widetilde{V}_{\lambda}(G)$ (for $\lambda$ belonging to X(G)) is direct. Moreover:

#### Lemma 1 {#lie-ix-s4-lem-1 .statement tag=01BV}

If G is commutative, $\widetilde{V}$ is the direct sum of the $\widetilde{V}_{\lambda}(G)$ for $\lambda \in X(G)$.

Since $\rho$ is semi-simple (§1, no. 1), it suffices to prove the lemma in the case in which $\rho$ is simple. In that case, the commutant Z of $\rho (G)$ in End( $\widetilde{V}$) reduces to homotheties (Algebra, Chap. VIII, §3, no. 2, Th. 1); thus, the image of the homomorphism $\widetilde{\rho}$ is contained in the subgroup $\mathbf{C}^*.1_V$ of GL( $\widetilde{V}$), and there exists $\lambda \in X(G)$ such that $\widetilde{V} = \widetilde{V}_{\lambda}(G)$.

#### Definition 1 {#lie-ix-s4-def-1 .statement tag=01BW}

The weights of the representation $\rho$ of G, relative to a maximal torus T of G, are the elements $\lambda$ of X(T) such that $\widetilde{V}_{\lambda}(T)\not= 0$.

Denote by $P(\rho ,T)$, or by $P(\rho )$ if there is no possibility of confusion over the choice of T, the set of weights of $\rho$ relative to T. By Lemma 1,

$$
\widetilde{V} =\bigoplus_{\lambda\in P(\rho ,T)}\widetilde{V}_{\lambda}(T) \tag{7}
$$

Let $T'$ be another maximal torus of G and $g$ an element of G such that (Int $g$)$T = T'($§2, no. 2, Th. 2). For all $\lambda \in X(T)$,

$\widetilde{\rho}(g)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{\lambda'}(T')$, where $\lambda '=$ X(Int $g^{-1}$)$(\lambda )$. (8)

Consequently,

X(Int $g$)$(P(\rho ,T')) = P(\rho ,T)$. (9)

The Weyl group $W = W_G(T)$ operates on the left on the $\mathbf{Z}$-module X(T) by $w \rightarrow X(w^{-1})$; thus, for $t\in T, \lambda \in X(T), w\in W$, we have $t^{w\lambda}= (w^{-1}(t))^{\lambda}$.

#### Proposition 5 {#lie-ix-s4-prop-5 .statement tag=01BX}

The set $P(\rho ,T)$ is stable under the operation of the Weyl group W. Let $n\in N_G(T)$, and let $w$ be its class in W; for $\lambda \in X(T)$, we have $\rho (n)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{w\lambda}(T)$ and dim $\widetilde{V}_{w\lambda}(T) =$ dim $\widetilde{V}_{\lambda}(T)$.

Formula (9), with $T'= T, g=n$, implies that $P(\rho ,T)$ is stable under $w$; further, $\widetilde{\rho}(n)$ induces an isomorphism from $\widetilde{V}_{\lambda}(T)$ to $\widetilde{V}_{w\lambda}(T)$ (formula (8)), hence the proposition.

#### Proposition 6 {#lie-ix-s4-prop-6 .statement tag=01BY}

The homomorphism $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ is injective if and only if $P(\rho ,T)$ generates the $\mathbf{Z}$-module X(T).

The homomorphism $\rho$ is injective if and only if its restriction to T is injective (§2, no. 6, Prop. 9). Further, since the canonical homomorphism $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ is injective, we can replace $\rho$ by $\widetilde{\rho}$. It then follows from (7) that the kernel of the restriction of $\rho$ to T is the intersection of the kernels of the elements of $P(\rho ,T)$. Thus, the conclusion follows from Prop. 2 of no. 1.

The linear representation $L(\rho )$ of $\mathfrak{t}$ in $\mathfrak{g}\mathfrak{l}( \widetilde{V})$ extends to a homomorphism of $\mathbf{C}$-Lie algebras

$$
\widetilde{L}(\rho ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}( \widetilde{V})
$$

Moreover, recall (no. 1) that we have associated to every element $\lambda$ of X(T) a linear form $\delta (\lambda )$ on $\mathfrak{t}_{\mathbf{C}}$ such that

(exp$_Tx$)$^{\lambda}=e^{\delta(\lambda)(x)},x\in \mathfrak{t}$. (10)

Recall finally (Chap. VII, §1, no. 1) that, for any map $\mu:\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$, we denote by $\widetilde{V}_\mu(\mathfrak{t}_{\mathbf{C}})$ the vector subspace of $\widetilde{V}$ consisting of the $v$ such that $(\widetilde{L}(\rho )(u))(v) =\mu(u).v$ for all $u\in \mathfrak{t}_{\mathbf{C}}$.

We now deduce from (7) and loc. cit., Prop. 3:

#### Proposition 7 {#lie-ix-s4-prop-7 .statement tag=01BZ}

a) For all $\lambda \in X(T)$, we have $\widetilde{V}_{\lambda}(T) = \widetilde{V}_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$.

b) The map $\delta : X(T)\rightarrow$ Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$ induces a bijection from $P(\rho ,T)$ to the set of weights of $\mathfrak{t}_{\mathbf{C}}$ on $\widetilde{V}$.

Note first that, if W operates on $\mathfrak{t}_{\mathbf{C}}$ by associating to any element $w$ of W the endomorphism $L(w)_{(\mathbf{C})}$ of $\mathfrak{t}_{\mathbf{C}}$, the map $\delta$ is compatible with the operation of W on X(T) and Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$.

Assume now that $k=\mathbf{R}$. Denote by $\sigma$ the conjugation of $\widetilde{V}$ relative to V, defined by $\sigma (x+iy) =x-iy$ for $x, y$ in V; for every complex vector subspace E of $\widetilde{V}$, the smallest subspace of $\widetilde{V}$ rational over $\mathbf{R}$ and containing E is $E +\sigma (E)$. In particular, for all $\lambda \in X(T)$, there exists a real vector subspace $V(\lambda )$ of V such that the subspace $V(\lambda )_{(\mathbf{C})}$ of $\widetilde{V}$ is $\widetilde{V}_{\lambda}(T) + \widetilde{V}_{-\lambda}(T)$ (note that $\sigma ( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{-\lambda}(T)$). We have $V(\lambda ) = V(-\lambda )$, and the $V(\lambda )$ are the isotypical components of the representation of T on V induced by $\rho$.

### 4. ROOTS

The roots of G relative to T are the non-zero weights of the adjoint representation of G. The set of roots of G relative to T is denoted by $R(G,T)$, or simply by R if there is no risk of confusion. By Prop. 6, the map

$$
\delta : X(T)\rightarrow \mathfrak{t}^*_{\mathbf{C}}
$$

$(\mathfrak{t}^*_{\mathbf{C}}$ denotes the dual of the complex vector space $\mathfrak{t}_{\mathbf{C}})$ maps $R(G,T)$ bijectively onto the set $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ of roots of the split reductive algebra $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ (Chap. VIII, §2, no. 2, Remark 4). If we put

$$
\mathfrak{g}^{\alpha}= (\mathfrak{g}_{\mathbf{C}})_{\alpha}(T) = (\mathfrak{g}_{\mathbf{C}})_{\delta(\alpha)}(\mathfrak{t}_{\mathbf{C}}) \tag{11}
$$

for all $\alpha \in R$, then each $\mathfrak{g}^{\alpha}$ is of dimension 1 over $\mathbf{C}($loc. cit., Th. 1) and

$$
\mathfrak{g}_{\mathbf{C}}=\mathfrak{t}_{\mathbf{C}}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha} \tag{12}
$$

For each $\alpha \in R$, denote by $V(\alpha )$ the 2-dimensional subspace of $\mathfrak{g}$ such that $V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$; the non-zero isotypical components of $\mathfrak{g}$ for the adjoint representation of T are $\mathfrak{t}$ and the $V(\alpha )$. Further, let K be the quadratic form associated to the Killing form of $\mathfrak{g}$; it is negative (§1, no. 3, Prop. 1) and its restriction $K(\alpha )$ to $V(\alpha )$ is negative and separating. For each element $t$ of T, Ad $t$ leaves $K(\alpha )$ stable, and hence gives a morphism of Lie groups

$$
\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))
$$

There exists a unique isomorphism $\rho_{\alpha}:\mathbf{U}\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$ such that $\iota_{\alpha}=\rho_{\alpha}\circ \alpha$. Indeed, let $X$ be a non-zero element of $\mathfrak{g}^{\alpha}$, and let $Y$ be the image of $X$ under the conjugation of $\mathfrak{g}_{\mathbf{C}}$ relative to $\mathfrak{g}$; then $Y\in \mathfrak{g}^{-\alpha}$, and we obtain a basis $(U, V)$ of $V(\alpha )$ by putting $U=X+Y, V=i(X-Y)$; the matrix of the endomorphism of $V(\alpha )$ induced by Ad $t,t\in T$, with respect to the basis $(U, V)$ is

$$
(\mathscr{R}(t^{\alpha})-\mathscr{I}(t^{\alpha}))
$$

$$
\mathscr{I}(t^{\alpha})\mathscr{R}(t^{\alpha})
$$

hence the assertion.

#### Proposition 8 {#lie-ix-s4-prop-8 .statement tag=01C0}

Let Q(R) be the subgroup of X(T) generated by the roots of G.

a) The centre C(G) of G is a closed subgroup of T, equal to the intersection of the kernels of the roots. The canonical map $X(T/C(G))\rightarrow X(T)$ is injective with image Q(R).

b) The compact group C(G) is isomorphic to the dual of the discrete group $X(T)/Q(R) ($Spectral Theories, Chap. II, §1, no. 1, Def. 2).

c) C(G) reduces to the identity element if and only if Q(R) is equal to X(T).

By §2, no. 2, Cor. 2 of Th. 2, C(G) is contained in T. Since this is the kernel of the adjoint representation, it is the intersection of the kernels of the roots, in other words the orthogonal complement of the subgroup Q(R) of X(T). Thus, the proposition follows from Spectral Theories, Chap. II, §1, no. 7, Th. 4 and no. 5, Th. 2.

#### Proposition 9 {#lie-ix-s4-prop-9 .statement tag=01C1}

Every automorphism of the Lie group G that induces the identity on T is of the form Int $t$, with $t\in T$.

Assume first of all that C(G) reduces to the identity element, in other words that X(T) = Q(R) (Prop. 8). Let $f$ be an automorphism of G inducing the identity on T, and $\varphi = L(f)_{(\mathbf{C})}$; then $\varphi$ is an automorphism of $\mathfrak{g}_{\mathbf{C}}$ inducing the identity on $\mathfrak{t}_{\mathbf{C}}$. By Chap. VIII, §5, no. 2, Prop. 2, there exists a unique homomorphism $\theta : Q(R)\rightarrow \mathbf{C}^*$ such that $\varphi$ induces on each $\mathfrak{g}^{\alpha}$ the homothety with ratio $\theta (\alpha )$. Since $\varphi$ leaves stable the real form $\mathfrak{g}$ of $\mathfrak{g}_{\mathbf{C}}$, it commutes with the conjugation $\sigma$ of $\mathfrak{g}_{\mathbf{C}}$ with respect to $\mathfrak{g}$; but $\sigma (\mathfrak{g}^{\alpha}) =\mathfrak{g}^{-\alpha}$, so $\theta (-\alpha ) =\overline{\theta(\alpha)}$ for all $\alpha \in R$. This implies that $\theta (\alpha )\theta (\alpha ) =\theta (\alpha )\theta (-\alpha ) = 1$. It follows that $\theta$ takes values in $\mathbf{U}$, and hence corresponds by duality to an element $t$ of T such that (Ad $t$)$_{(\mathbf{C})}=\varphi$, so Int $t=f$.

In the general case, the preceding applies to the group $G/C(G)$, whose centre reduces to the identity element, and to its maximal torus $T/C(G)$. It follows that, if $f$ is an automorphism of G inducing the identity on T, there exists an element $t$ of T such that $f$ and Int $t$ induce by passage to the quotient the same automorphism of $G/C(G)$. But, since the canonical morphism $D(G)\rightarrow G/C(G)$ is a finite covering (§1, no. 4, Cor. 1 of Prop. 4), $f$ and Int $t$ induce the same automorphism of D(G), hence of $D(G)\times C(G)$, and hence also of G (loc. cit.).

#### Corollary {#lie-ix-s4-n4-cor-1 .statement tag=01C2}

Let $u$ be an automorphism of G and H the closed subgroup of G consisting of the fixed points of $u$. Then, the automorphism $u$ is inner if and only if $H_0$ is of maximal rank.

If $u$ is equal to Int $g$, with $g\in G$, the subgroup $H_0= Z(g)_0$ is of maximal rank (§2, no. 2, Cor. 3). Conversely, if H contains a maximal torus S, the automorphism $u$ is of the form Int $s$ with $s\in S$ (Prop. 9).

### 5. NODAL VECTORS AND INVERSE ROOTS

#### Lemma 2 {#lie-ix-s4-lem-2 .statement tag=01C3}

Let S be a closed subgroup of T and Z(S) its normalizer in G.

(i) $R(Z(S)_0,T)$ is the set of $\alpha \in R(G,T)$ such that $\alpha (S) =\{1\}$.

(ii) The centre of $Z(S)_0$ is the intersection of the Ker$\alpha$ for $\alpha \in R(Z(S)_0,T)$.

(iii) If S is connected, Z(S) is connected.

The Lie algebra $L(Z(S))_{(\mathbf{C})}$ consists of the invariants of S on $\mathfrak{g}_{\mathbf{C}}$ (Chap. III, §9, no. 3, Prop. 8), and hence is the direct sum of $\mathfrak{t}_{\mathbf{C}}$ and the $\mathfrak{g}^{\alpha}$ for which $\alpha (S) =\{1\}$, hence (i). Assertion (ii) follows from Prop. 8 (no. 4), and assertion (iii) has already been proved (§2, no. 2, Cor. 5 of Th. 2).

#### Theorem 1 {#lie-ix-s4-thm-1 .statement tag=01C4}

Let $\alpha \in R(G,T)$. The centralizer $Z_{\alpha}$ of the kernel of $\alpha$ is a connected closed subgroup of G; its centre is Ker $\alpha$; its derived group $D(Z_{\alpha}) = S_{\alpha}$ is a connected closed semi-simple subgroup of G of rank 1. We have $R(Z_{\alpha},T) =\{\alpha ,-\alpha \}$ and dim $Z_{\alpha}=$ dim T + 2.

Let $Z'_{\alpha}$ be the centralizer of (Ker $\alpha$ )$_0$. By Lemma 2, this is a connected closed subgroup of G, and $R(Z'_{\alpha},T)$ is the set of $\beta \in R(G,T)$ such that $\beta$((Ker$\alpha$ )$_0$) $=\{1\}$. Clearly, $\{\alpha ,-\alpha \} \subset R(Z'_{\alpha},T)$. Conversely, let $\beta \in R(Z'_{\alpha},T)$; since (Ker $\alpha$ )$_0$ is of finite index in Ker $\alpha$, there exists an integer $r\not= 0$ such that $t^{r\beta}= 1$ for $t\in$ Ker $\alpha$. From the exactness of the sequence

$0\longrightarrow \mathbf{Z}\longrightarrow X(T)\longrightarrow$ X(Ker $\alpha$ )$\longrightarrow 0$

corresponding by duality to the exact sequence

0 $\longrightarrow$ Ker$\alpha \longrightarrow$ T $\longrightarrow^{\alpha}\mathbf{U}\longrightarrow 0$,

it follows that $r\beta$ is a multiple of $\alpha$; by Chap. VIII, §2, no. 2, Th. 2 (i), this implies that $\beta \in  \{\alpha ,-\alpha \}$. Thus, $R(Z'_{\alpha},T) =\{\alpha ,-\alpha \}$. It follows (Lemma 2) that the centre of $Z'_{\alpha}$ is Ker$\alpha$, so $Z'_{\alpha}= Z_{\alpha}$. Finally, by Cor. 1 of Prop. 4 (§1, no. 4), $D(Z_\alpha)$ is a connected closed semi-simple subgroup of $G$; it is of rank $1$ because $\mathscr{L}(Z_\alpha)(\mathbf C)=\mathfrak{g}^\alpha+\mathfrak{g}^{-\alpha}+[\mathfrak{g}^\alpha,\mathfrak{g}^{-\alpha}]$.

#### Corollary {#lie-ix-s4-n5-cor-1 .statement tag=01C7}

— *There exists a morphism of Lie groups* $\nu:\mathbf{SU}(2,\mathbf C)\to G$ *with the following properties:*

a) *The image of* $\nu$ *commutes with the kernel of* $\alpha$.

b) *For all* $a\in\mathbf U$, *we have*
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
\quad\text{and}\quad
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}=a^2.
$$

*If* $\nu_1$ *and* $\nu_2$ *are two morphisms from* $\mathbf{SU}(2,\mathbf C)$ *to* $G$ *with the preceding properties, there exists* $a\in\mathbf U$ *such that*
$$
\nu_2=\nu_1\circ\operatorname{Int}
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}.
$$

By Th. 1 and Prop. 6 of §3, no. 6, there exists a morphism of Lie groups
$$
\nu:\mathbf{SU}(2,\mathbf C)\to S_\alpha
$$
that is surjective with discrete kernel. Then $\nu^{-1}(\mathbf T\cap S_\alpha)$ is a maximal torus of $\mathbf{SU}(2,\mathbf C)$ (§2, no. 3, Prop. 1). Since the maximal tori of $\mathbf{SU}(2,\mathbf C)$ are conjugate (§2, no. 2, Th. 2), we can assume, replacing $\nu$ by $\nu\circ\operatorname{Int}s$ (with $s\in\mathbf{SU}(2,\mathbf C)$) if necessary, that $\nu^{-1}(\mathbf T\cap S_\alpha)$ is the group of diagonal matrices in $\mathbf{SU}(2,\mathbf C)$. Then
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
$$
for all $a\in\mathbf U$, and the map
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
\longmapsto
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
is a root of $\mathbf{SU}(2,\mathbf C)$, and hence is equal to one of the two maps
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^2
$$
or
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^{-2}
$$
(§3, no. 6, formulas (19)). In the first case, the homomorphism $\nu$ has the required properties; in the second case, the homomorphism $\nu\circ\operatorname{Int}\theta$ has them (loc. cit., formulas (18)).

If $\nu_1$ and $\nu_2$ are two morphisms from $\mathbf{SU}(2,\mathbf C)$ to $G$ satisfying the stated conditions, they both map $\mathbf{SU}(2,\mathbf C)$ into $S_\alpha$ (condition a)), hence are both universal coverings of $S_\alpha$. Hence, there exists an automorphism $\varphi$ of $\mathbf{SU}(2,\mathbf C)$ such that $\nu_2=\nu_1\circ\varphi$, and we conclude by using Prop. 9 of no. 4.

It follows from the preceding corollary that the homomorphism $\nu_{\mathbf T}$ from $\mathbf U$ to $\mathbf T$, defined by
$$
\nu_{\mathbf T}(a)=\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
for $a\in\mathbf U$, is independent of the choice of $\nu$. Denote by $K_\alpha\in\Gamma(\mathbf T)$ the image under $\Gamma(\nu_{\mathbf T})$ of the element $2\pi i$ of $\Gamma(\mathbf U)=2\pi i\mathbf Z$; it is called the *nodal vector associated to the root* $\alpha$. We have $\langle\alpha,K_\alpha\rangle=2$, in other words (no. 2, formula (2)) $\delta(\alpha)(K_\alpha)=4\pi i$; since $K_\alpha$ belongs to the intersection of $\mathfrak t$ and the $\mathscr L(S_\alpha)(\mathbf C)$, we have
$$
K_\alpha=2\pi iH_{\delta(\alpha)},
\tag{13}
$$
where $H_{\delta(\alpha)}$ is the *inverse root associated to the root* $\delta(\alpha)$ of $(\mathfrak g_{\mathbf C},\mathfrak t_{\mathbf C})$ (Chap. VIII, §2, no. 2). In other words, when $\Gamma(\mathbf T)\otimes\mathbf R$ is identified with the dual of $X(T)\otimes \mathbf{R}$ via the pairing $\langle ,\rangle ,K_{\alpha}$ is identified with the inverse root $\alpha^{\vee}\in (X(T)\otimes \mathbf{R})^*$.

#### Remark {#lie-ix-s4-n5-rem-1 .statement tag=01C5}

For all $x\in \mathbf{R}$, we have

$($ exp(2$\pi ix$) 0 $)_{2\pi ix}$

$\nu$ 0 exp($-2\pi ix$)$=\nu_T(e$ ) = exp($xK_{\alpha}$). (14)

In particular:

$\nu (-0$1 $-01)=\nu_T(-1) =$ exp$(\frac{1}{2}K_{\alpha})$. (15)

It follows that $\nu$ is injective if and only if $K_{\alpha}\in /2\Gamma$(T), in other words if there exists $\lambda \in X(T)$ such that $\langle \lambda , K_{\alpha}\rangle \in /2\mathbf{Z}$. When $\mathfrak{g}_{\mathbf{C}}$ is simple, $\nu$ is injective unless $\mathfrak{g}_{\mathbf{C}}$ is of type $B_n, C(G) =\{1\}$ and $\alpha$ is a short root (cf. Chap. VI, Plates).

In the remainder of this paragraph we denote by $R^{\vee}(G,T)$ the set of nodal vectors $K_{\alpha}$ for $\alpha \in R(G,T)$. This is a subset of $\Gamma (T)$ that the canonical injection of $\Gamma (T)$ into $\mathfrak{t}_{\mathbf{C}}$ identifies with the homothety with ratio $2\pi i$ of the inverse root system $R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) =\{H_{\delta(\alpha)}\}$ of $\delta (R)$. It follows that $R^{\vee}(G,T)$ generates the $\mathbf{R}$-vector space $L(T\cap D(G))$, and hence that its orthogonal complement in X(T) is $X(T/(T\cap D(G)))$.

Denote by Aut(T) the group of automorphisms of the Lie group T; the Weyl group $W = W_G(T) ($§2, no. 5) can be identified with a subgroup of Aut(T). On the other hand, recall (Chap. VIII, §2, no. 2, Remark 4) that the Weyl group $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ of the split reductive algebra $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ operates on $\mathfrak{t}_{\mathbf{C}}$, and thus is canonically identified with a subgroup of $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$.

#### Proposition 10 {#lie-ix-s4-prop-10 .statement tag=01C6}

The map $u \rightarrow L(u)_{(\mathbf{C})}$ from Aut(T) to $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ induces an isomorphism from W to the Weyl group of the split reductive Lie algebra $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. For all $\alpha \in R$, $W_{Z_{\alpha}}(T)$ is of order 2, and the image under the preceding isomorphism of the non-identity element of $W_{Z_{\alpha}}(T)$ is the reflection $s_{H_{\delta(\alpha)}}$.

The map under consideration is injective. It remains to show that its image is equal to $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

Let $g\in N_G(T)$. With the notations in Chap. VIII, §5, no. 2, we have Ad $g\in$ Aut($\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}$)$\cap$ Int($\mathfrak{g}_{\mathbf{C}}$), so Ad $g\in$ Aut$_0(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) ($loc. cit., no. 5, Prop. 11). By loc. cit., no. 2, Prop. 4, the automorphism of $\mathfrak{t}_{\mathbf{C}}$ induced by Ad $g$ belongs to $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. Thus, the image of W in $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ is contained in $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

Let $\alpha \in R(G,T)$, and let $\nu :\mathbf{S}\mathbf{U}(2,\mathbf{C})\rightarrow G$ be a morphism of Lie groups having the properties in the Cor. of Th. 1. The image under $\nu$ of the element $\theta$ of $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ has the following properties (§3, no. 6, formulas (17)):

$a)$ (Int$\nu (\theta )$)$(t) =t$ if $t\in$ Ker$\alpha$,

$b)$ (Int$\nu (\theta )$)$(t) =t^{-1}$ if $t\in T\cap S_{\alpha}$.

It follows that Ad $\nu (\theta )$ induces the identity on Ker $\delta (\alpha )\subset \mathfrak{t}_{\mathbf{C}}$, and induces the map $x \rightarrow  -x$ on $[\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$, hence coincides with the reflection $s_{H_{\delta(\alpha)}}$. Thus, the image of W contains all the $s_{H_{\delta(\alpha)}}$, and hence is equal to $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. In particular $W_{Z_{\alpha}}(T)$ is of order 2, and hence consists of the identity and Int $\nu (\theta )$. This completes the proof of the proposition.

#### Corollary {#lie-ix-s4-n5-cor-2 .statement tag=01JJ}

Assume that G is semi-simple. Then every element of G is the commutator of two elements of G.

Let $c$ be a Coxeter transformation of the Weyl group $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ (Chap. V, §6, no. 1), and let $n$ be an element of $N_G(T)$ whose class in W is identified with $c$ by the isomorphism defined in the proposition. Denote by $f_c$ the morphism $t \rightarrow (n, t)$ from T to T; for $x\in \mathfrak{t}_{\mathbf{C}}$, we have $L(f_c)_{(\mathbf{C})}(x) =$ (Ad $n$)$(x)-x=$ $c(x)-x$.

By Th. 1 of Chap. V, §6, no. 2, the endomorphism $c$ of $\mathfrak{t}_{\mathbf{C}}$ has no eigenvalue equal to 1. Consequently, $L(f_c)$ is surjective, and hence so is $f_c$. It follows that every element of T is the commutator of two elements of G, which implies the corollary in view of Th. 2, §2, no. 2.

### 6. FUNDAMENTAL GROUP

In the following proposition, $f(G,T)$ denotes the homomorphism from $\Gamma (T)$ to $\pi_1(G)$ that is the composite of the canonical isomorphism from $\Gamma (T)$ to $\pi_1(T)$ (no. 2, Remark 3) and the homomorphism $\pi_1(\iota )$, where $\iota$ is the canonical injection $T\rightarrow G$.

#### Proposition 11 {#lie-ix-s4-prop-11 .statement tag=01C8}

The homomorphism $f(G,T) :\Gamma (T)\rightarrow \pi_1(G)$ is surjective. Its kernel is the subgroup $N(G,T)$ of $\Gamma (T)$ generated by the family of nodal vectors $(K_{\alpha})_{\alpha\in R(G,T)}$.

The homomorphism $f(G,T)$ is surjective by Prop. 3 (§2, no. 4). We denote by $A(G,T)$ the assertion: “the kernel of $f(G,T)$ is generated by the $K_{\alpha}$” which it remains to prove, and distinguish several cases:

$a) G$ is simply-connected. Let $\rho :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ be a linear representation of $\mathfrak{g}_{\mathbf{C}}$ on a finite dimensional complex vector space V. Restricting to $\mathfrak{g}$, we obtain a representation of $\mathfrak{g}$ on the real vector space $V_{(\mathbf{R})}$; since G is simply-connected, there exists an analytic linear representation $\pi$ of G on $V_{(\mathbf{R})}$ such that $\rho = L(\pi )$. It follows from Prop. 7 of no. 3 that the image $\delta (X(T))$ of X(T) in $\mathfrak{t}^*_{\mathbf{C}}$ contains all the weights of $\rho$ on V. This being true for every representation $\rho$ of $\mathfrak{g}_{\mathbf{C}}$, it follows from Chap. VIII, §7, no. 2, Th. 1 that $\delta (X(T))$ contains the group of weights of $\delta$(R), which is by definition the set of $\lambda \in \mathfrak{t}^*_{\mathbf{C}}$ such that $\lambda (H_{\delta(\alpha)})\in \mathbf{Z}$ for all $\alpha \in R$, in other words, $\lambda (K_{\alpha})\in 2\pi i\mathbf{Z}$ for all $\alpha \in R$. Thus, the group X(T) contains all the elements $\lambda$ of $X(T)\otimes \mathbf{Q}$ such that $\langle \lambda , K_{\alpha}\rangle  \in \mathbf{Z}$ for all $\alpha \in R$, which implies by duality that $\Gamma (T)$ is generated by the $K_{\alpha}$, hence the assertion $A(G,T)$.

$b) G$ is the direct product of a simply-connected group $G'$ and a torus S. Then T is the direct product of a maximal torus $T'$ of $G'$ with $S,\Gamma (T)$ can be identified with $\Gamma (T')\times \Gamma$(S), $\pi_1(G)$ with $\pi_1(G')\times \pi_1$(S), and $f(G,T)$ with the homomorphisms with components $f(G',T')$ and $f(S,S)$. Since $f(S,S)$ is bijective, the canonical map $\Gamma (T')\rightarrow \Gamma (T)$ maps Ker $f(G',T')$ bijectively onto Ker $f(G,T)$. Moreover, the $K_{\alpha}$ belong to the Lie algebra of the derived group $G'$ of G, hence to the image of $\Gamma (T')$, so it is immediate that $A(G',T')$ implies $A(G,T)$, hence assertion $A(G,T)$, in view of $a)$.

$c)$ General case. There exists a surjective morphism $p: G'\rightarrow G$ with finite kernel, where $G'$ is the direct product of a simply-connected group by a torus (§1, no. 4, Prop. 4). If $T'$ is the inverse image of T in $G'$ (this is a maximal torus of $G'$ by §2, no. 3, Prop. 1), and N the kernel of $p$, we have exact sequences $0\rightarrow N\rightarrow G'\rightarrow G\rightarrow 0$ and $0\rightarrow N\rightarrow T'\rightarrow T\rightarrow 0$, hence a commutative diagram with exact rows (no. 2, Remark 1 and General Topology, Chap. XI, in preparation)

0 $\longrightarrow \Gamma (T')\longrightarrow \Gamma (T)\longrightarrow$ N $\longrightarrow$ 0

$f(G',T')f(G,T)$ Id$_N$

0 $\longrightarrow \pi_1(G')\longrightarrow \pi_1(G)\longrightarrow$ N $\longrightarrow 0$.

It follows immediately from the snake diagram (Algebra, Chap. X, p. 4, Prop. 2) that $A(G',T')$ implies $A(G,T)$, hence the proposition, in view of $b)$.

#### Corollary 1 {#lie-ix-s4-prop-11-cor-1 .statement tag=01C9}

G is simply-connected if and only if the family $(K_{\alpha})_{\alpha\in R(G,T)}$ generates $\Gamma (T)$.

#### Corollary 2 {#lie-ix-s4-prop-11-cor-2 .statement tag=01CA}

Let H be a connected closed subgroup of G containing T; there is an exact sequence

$$
0\longrightarrow N(H,T)\longrightarrow N(G,T)\longrightarrow \pi_1(H)\longrightarrow \pi_1(G)\longrightarrow 0
$$

This follows from Algebra, Chap. X, p. 4, Prop. 2 (snake diagram), applied to the commutative diagram

0 $\longrightarrow N(H,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(H)\longrightarrow$ 0

0 $\longrightarrow N(G,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(G)\longrightarrow 0$.

#### Remark {#lie-ix-s4-n6-rem-1 .statement tag=01CB}

It can be shown (cf. Exercise 2 of §5) that $\pi_2(G/H)$ is zero. The exactness of the preceding sequence then gives an isomorphism from $\pi_2(G/H)$ to $N(G,T)/N(H,T)$.

#### Corollary 3 {#lie-ix-s4-prop-11-cor-3 .statement tag=01CC}

The homomorphism $\pi_1(D(G))\rightarrow \pi_1(G)$ corresponding to the inclusion of D(G) into G induces an isomorphism from $\pi_1(D(G))$ to the torsion subgroup of $\pi_1(G)$.

Indeed, $T\cap D(G)$ is a maximal torus of D(G) (§2, no. 3, Prop. $1c$)$)$; from the exact sequence

$$
0\longrightarrow \Gamma (T\cap D(G))\longrightarrow \Gamma (T)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

and Proposition 11, we obtain an exact sequence

$$
0\longrightarrow \pi_1(D(G))\longrightarrow \pi_1(G)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

hence the corollary, since $\pi_1(D(G))$ is finite and $\Gamma (T/(T\cap D(G)))$ is free.

### 7. SUBGROUPS OF MAXIMAL RANK

Recall (Chap. VI, §1, no. 7) that a subset P of $R = R(G,T)$ is said to be closed if $(P + P)\cap R\subset P$, and symmetric if $P =-P$.

#### Proposition 12 {#lie-ix-s4-prop-12 .statement tag=01CD}

Let $\mathscr{H}$ be the set of connected closed subgroups of G containing T, ordered by inclusion. The map $H \rightarrow R(H,T)$ is an increasing bijection from $\mathscr{H}$ to the set of symmetric closed subsets of $R(G,T)$, ordered by inclusion.

If $H\in \mathscr{H}$, then $L(H)_{(\mathbf{C})}$ is the direct sum of $\mathfrak{t}_{\mathbf{C}}$ and the $\mathfrak{g}^{\alpha}$ for $\alpha \in R(H,T)$; since this is a reductive subalgebra in $\mathfrak{g}_{\mathbf{C}}$, the subset $R(H,T)$ of R satisfies the stated conditions (Chap. VIII, §3, no. 1, Lemma 2 and Prop. 2). Conversely, if P is a subset of R satisfying these conditions, then $\mathfrak{t}_{\mathbf{C}}\oplus \sum_{\alpha\in P}\mathfrak{g}^{\alpha}$ is a subalgebra

of $\mathfrak{g}_{\mathbf{C}}($loc. cit.) which is rational over $\mathbf{R}$ (no. 3), and hence of the form $\mathfrak{h}_{(\mathbf{C})}$, where $\mathfrak{h}$ is a subalgebra of $\mathfrak{g}$. Let H(P) be the integral subgroup of G defined by $\mathfrak{h}$; it is closed (§2, no. 4, Remark 1). We verify immediately that the maps $H \rightarrow R(H,T)$ and $P \rightarrow H(P)$ are increasing and inverses of each other.

#### Corollary 1 {#lie-ix-s4-prop-12-cor-1 .statement tag=01CE}

There are only finitely-many closed subgroups of G containing T.

Let H be such a subgroup; then $H_0\in \mathscr{H}$, and $\mathscr{H}$ is finite. Moreover, H is a subgroup of $N_G(H_0)$ containing $H_0$, and $N_G(H_0)/H_0$ is finite (§2, no. 4, Prop. 4 and Remark 2).

#### Corollary 2 {#lie-ix-s4-prop-12-cor-2 .statement tag=01CF}

Let H be a connected closed subgroup of G containing T, and let $W^H_G(T)$ be the stabilizer in $W_G(T)$ of the subset $R(H,T)$ of R. The group $N_G(H)/H$ is isomorphic to the quotient group $W^H_G(T)/W_H(T)$.

Indeed, it follows from Prop. 7 of §2, no. 5, applied to $N_G$(H), that $N_G(H)/H$ is isomorphic to $W_{N(H)}(T)/W_H$(T), where $W_{N(H)}(T)$ is the set of elements of $W_G(T)$ whose representatives in $N_G(T)$ normalize H. Let $n\in N_G$(T), and let $w$ be its class in $W_G(T)$. By Chap. III, §9, no. 4, Prop. 11, $n$ normalizes H if and only if (Ad $n$)$(L(H)) = L(H)$; in view of Prop. 5 of no. 3, this also means that the subset $R(H,T)$ of R is stable under $w$, hence the corollary.

#### Remark 1 {#lie-ix-s4-n7-rem-1 .statement tag=01CG}

The group $W^H_G(T)$ is also the stabilizer in $W_G(T)$ of the subgroup C(H) of T: this follows from Prop. 8 of no. 4.

#### Proposition 13 {#lie-ix-s4-prop-13 .statement tag=01CH}

Let H be a connected closed subgroup of G of maximal rank, and C its centre. Then C contains the centre of G, and H is the identity component of the centralizer of C.

Let S be a maximal torus of H. Since the centre of G is contained in S, it is contained in C. Put $L = Z(C)_0$; this is a connected closed subgroup of G containing H, hence is of maximal rank, and its centre is equal to C. Denote by $R_H$ and $R_L$ the root systems of H and L, respectively, relative to S; then $R_H\subset R_L\subset R(G,S)$. Since C(H) = C(L), Prop. 8 (no. 4) implies the equality $Q(R_H) = Q(R_L)$; but $Q(R_H)\cap R_L= R_H$ (Chap. VI, §1, no. 7, Prop. 23), so $R_H= R_L$ and H = L (Prop. 12).

#### Remark 2 {#lie-ix-s4-n7-rem-2 .statement tag=01CI}

Say that a subgroup C of G is radical if there exists a maximal torus S of G and a subset P of $R(G,S)$ such that $C =\bigcap_{\alpha\in P}$ Ker$\alpha$. It follows from Prop. 13 and Lemma 2 of no. 5 that the map $H \rightarrow C(H)$ induces a bijection from the set of connected closed subgroups of maximal rank to the set of radical subgroups of G. The inverse bijection is the map $C \rightarrow Z(C)_0$.

#### Corollary {#lie-ix-s4-n7-cor-1 .statement tag=01CJ}

The set of $g\in G$ such that $T\cap gTg^{-1}\not= C(G)$ is the union of a finite number of closed analytic submanifolds of G distinct from G.

Indeed, put $A_g= T\cap gTg^{-1}$; we have $T\subset Z(A_g)$ and $gTg^{-1}\subset Z(A_g)$. Hence, there exists $x\in Z(A_g)$ such that $xTx^{-1}=gTg^{-1}($§2, no. 2, Th. 2), which implies that $g\in Z(A_g).N_G(T)$. Denote by $\mathscr{A}$ the finite (Cor. 1) set of closed subgroups of G containing T and distinct from G, and put X = $\bigcup_{H\in\mathscr{A}}H.N_G(T)$; this is a finite union of closed submanifolds of G, distinct from G. If $A_g\not= C(G)$, then $Z(A_g)\in \mathscr{A}$, and $g$ belongs to X. Conversely, if $g\in H.N_G$(T), with $H\in \mathscr{A}$, then $A_g$ contains C(H), so $A_g\not= C(G)$ (Prop. 13).

#### Proposition 14 {#lie-ix-s4-prop-14 .statement tag=01CK}

Let X be a subset of T, and let $R_X$ be the set of roots $\alpha \in R(G,T)$ such that $\alpha (X) =\{1\}$. The group $Z_G(X)/Z_G(X)_0$ is isomorphic to the quotient of the subgroup of $W_G(T)$ fixing X by the subgroup generated by the reflections $s_{\alpha}$ for $\alpha \in R_X$.

Put $H = Z_G(X)$; since $L(H)_{(\mathbf{C})}$ is the set of points of $\mathfrak{g}_{\mathbf{C}}$ fixed by Ad(X), it is the sum of $\mathfrak{t}_{\mathbf{C}}$ and the $\mathfrak{g}^{\alpha}$ for which $\alpha (X) =\{1\}$. Consequently, $R(H_0,T) =$ $R_X$, so $W_{H_0}(T)$ is generated by the reflections $s_{\alpha}$ for $\alpha \in R_X$. It now suffices to apply Prop. 7 of §2, no. 5.

We shall see below (§5, no. 3, Th. 1) that if G is simply-connected and X reduces to a point, the centralizer Z(X) is connected.

### 8. ROOT DIAGRAMS

#### Definition 2 {#lie-ix-s4-def-2 .statement tag=01CL}

A root diagram (or simply a diagram, if there is no risk of confusion) is a triple $D = (M,M_0,R)$ where:

(RD$_0$) $M$ is a free $\mathbf{Z}$-module of finite type and the submodule $M_0$ is a direct factor of M;

(RD$_I$) $R$ is a finite subset of $M; R\cup M_0$ generates the $\mathbf{Q}$-vector space $\mathbf{Q}\otimes M$;

(RD$_{II}$) for all $\alpha \in R$, there exists an element $\alpha^{\vee}$ of $M^*=$ Hom$_{\mathbf{Z}}(M,\mathbf{Z})$ such that $\alpha^{\vee}(M_0) = 0,\alpha^{\vee}(\alpha ) = 2$ and the endomorphism $x \rightarrow x-\alpha^{\vee}(x)\alpha$ of M leaves R stable.

By Chap. VI, §1, no. 1, for all $\alpha \in R$ the element $\alpha^{\vee}$ of $M^*$ is uniquely determined by $\alpha$; we denote by $s_{\alpha}$ the endomorphism $x \rightarrow x-\alpha^{\vee}(x)\alpha$ of M. Moreover (loc. cit.), the $\mathbf{Q}$-vector space $\mathbf{Q}\otimes M$ is the direct sum of $\mathbf{Q}\otimes M_0$ and the vector subspace V(R) generated by R, and R is a root system in V(R) (loc. cit., Def. 1).

The elements of R are called the roots of the root diagram D, and the elements $\alpha^{\vee}$ of $M^*$ the inverse roots. The group generated by the automorphisms $s_{\alpha}$ of M is called the Weyl group of D and is denoted by W(D); the elements of W(D) induce the identity on $M_0$, and induce on V(R) the transformations of the Weyl group of the root system R.

#### Example 1 {#lie-ix-s4-n8-exa-1 .statement tag=01CM}

For every free $\mathbf{Z}$-module of finite type M, the triple $(M,M,\emptyset )$ is a root diagram.

#### Example 2 {#lie-ix-s4-n8-exa-2 .statement tag=01CN}

If $D = (M,M_0,R)$ is a root diagram, let $M^*_0$ be the orthogonal complement of V(R) in $M^*$, and let $R^{\vee}$ be the set of inverse roots of D. Then $D^{\vee}= (M^*,M^*_0,R^{\vee})$ is a root diagram, called the inverse of D. For all $\alpha \in R$, the symmetry $s_{\alpha^{\vee}}$ of $M^*$ is the contragredient automorphism of the symmetry $s_{\alpha}$ of M; the map $w \rightarrow^tw^{-1}$ is an isomorphism from W(D) to $W(D^{\vee})$. Moreover, $V(R^{\vee})$ can be naturally identified with the dual of the $\mathbf{Q}$-vector space $V(R), R^{\vee}$ then being identified with the inverse root system of R.

If the dual of $M^*$ is identified with M, the inverse diagram of $D^{\vee}$ is identified with D.

#### Example 3 {#lie-ix-s4-n8-exa-3 .statement tag=01CO}

Let $(\mathfrak{g},\mathfrak{h})$ be a split reductive $\mathbf{Q}$-Lie algebra, and $M\subset \mathfrak{h}$ a permissible lattice (Chap. VIII, §12, no. 6, Def. 1). Let $M_0$ be the subgroup of M orthogonal to the roots of $(\mathfrak{g},\mathfrak{h})$ and $R^{\vee}$ the set of the $H_{\alpha},\alpha \in R(\mathfrak{g},\mathfrak{h})$. Then $(M,M_0,R^{\vee})$ is a root diagram, and $(M^*,M^*_0,R(\mathfrak{g},\mathfrak{h}))$ is the inverse diagram.

#### Example 4 {#lie-ix-s4-n8-exa-4 .statement tag=01CP}

Let V be a vector space over $\mathbf{Q}$ and R a root system in V; denote by P(R) the group of weights of R and by Q(R) the group of radical weights of R (Chap. VI, §1, no. 9). Then $(Q(R),0,R)$ and $(P(R),0,R)$ are root diagrams. A root diagram $(M,M_0,S)$ is isomorphic to a diagram of the form $(Q(R),0,R)$ (resp. $(P(R),0,R)$) if and only if M is generated by S (resp. $M^*$ is generated by $S^{\vee}$).

For every subgroup X of P(R) containing $Q(R), (X,0,R)$ is a root diagram and, up to isomorphism, every diagram $(M,M_0,S)$ such that $M_0= 0$, in other words such that S generates a subgroup of M of finite index, arises in this way.

The root diagram $(M,M_0,R)$ is said to be reduced if the root system R is reduced (in other words (Chap. VI, §1, no. 4) if the relations $\alpha , \beta \in R,\lambda \in \mathbf{Z}$, $\beta =\lambda \alpha$ imply that $\lambda = 1$ or $\lambda =-1$). The diagrams in Examples 1) and 3) are reduced.

### 9. COMPACT LIE GROUPS AND ROOT SYSTEMS

With the terminology introduced in the preceding number, an important part of the results of numbers 4 and 5 can be summarized in the following theorem:

#### Theorem 2 {#lie-ix-s4-thm-2 .statement tag=01CQ}

a$) (X(T),X(T/(T\cap D(G)),R(G,T)))$ is a reduced root diagram; its Weyl group consists of the $X(w)$ for $w\in W$; the group X(C(G)) is isomorphic to the quotient of X(T) by the subgroup generated by $R(G,T)$.

b$) (\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$ is a reduced root diagram; its Weyl group consists of the $\Gamma (w)$, for $w\in W$; the group $\pi_1(G)$ is isomorphic to the quotient of $\Gamma (T)$ by the subgroup generated by $R^{\vee}(G,T)$.

c) If each of the $\mathbf{Z}$-modules X(T) and $\Gamma (T)$ is identified with the dual of the other (no. 2, Prop. 3), each of the preceding root diagrams is identified with the inverse of the other.

Denote by $D^*(G,T)$ the diagram $(X(T),X(T/(T\cap D(G)),R(G,T)))$ and by $D_*(G,T)$ the diagram $(\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$; these are called the contravariant diagram and the covariant diagram of G (relative to T), respectively.

#### Example 1 {#lie-ix-s4-n9-exa-1 .statement tag=01CR}

If G is semi-simple of rank 1, then $D^*(G,T)$ and $D_*(G,T)$ are necessarily isomorphic to one of the two diagrams $\Delta_2= (\mathbf{Z},0,\{2,-2\})$, $\Delta_1= (\mathbf{Z},0,\{1,-1\})$. If G is isomorphic to $\mathbf{S}\mathbf{U}(2,\mathbf{C}), D_*(G,T)$ is isomorphic to $\Delta_1$ (since G is simply-connected) so $D^*(G,T)$ is isomorphic to $\Delta_2$. If G is isomorphic to $\mathbf{S}\mathbf{O}(3,\mathbf{R}), D^*(G,T)$ is isomorphic to $\Delta_1$ (since $C(G) =\{1\}$), so $D_*(G,T)$ is isomorphic to $\Delta_2$.

#### Example 2 {#lie-ix-s4-n9-exa-2 .statement tag=01CS}

If G and $G'$ are two connected compact Lie groups, with maximal tori T and $T'$, respectively, and if $D^*(G,T) = (M,M_0,R)$ and $D^*(G',T') =$ $(M',M'_0,R')$, then $D^*(G\times G',T\times T')$ can be identified with $(M\oplus M',M_0\oplus$ $M'_0,R\cup R')$. Similarly for the covariant diagrams.

#### Example 3 {#lie-ix-s4-n9-exa-3 .statement tag=01CT}

Let N be a closed subgroup of T, central in G, and let $(M,M_0,R)$ be the contravariant diagram of G relative to T. Then the contravariant diagram of $G/N$ relative to $T/N$ can be identified with $(M',M'_0,R)$, where $M'$ is the subgroup of M consisting of the $\lambda$ such that $\lambda (N) =\{1\}$ and $M'_0= M'\cap M_0$.

#### Example 4 {#lie-ix-s4-n9-exa-4 .statement tag=01CU}

Similarly, let N be a finite abelian group, and $\varphi :\pi_1(G)\rightarrow N$ a surjective homomorphism. Let $G'$ be the covering of G associated to this homomorphism; this is a connected compact Lie group, of which N is a central subgroup (General Topology, Chap. XI, in preparation), and G can be naturally identified with $G'/N$. Let $T'$ be the maximal torus of $G'$ that is the inverse image of T. If $(P,P_0,S)$ is the covariant diagram of G relative to T, the covariant diagram of $G'$ relative to $T'$ can be identified with $(P',P'_0,S)$, where $P'$ is the kernel of the composite homomorphism $\varphi \circ f(G,T) : P\rightarrow N$ (cf. no. 6, Prop. 11), and $P'_0= P_0\cap P'$.

#### Remark 1 {#lie-ix-s4-n9-rem-1 .statement tag=01CV}

Let $\mathfrak{c}$ be the centre of $\mathfrak{g}_{\mathbf{C}}$; then $\mathfrak{c}= L(C(G))_{(\mathbf{C})}$. We have the following relations between the diagrams of G relative to T and the direct and inverse root systems of the split reductive algebra $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}):$

$a)$ The canonical isomorphism from $\mathbf{C}\otimes \Gamma (T)$ to $\mathfrak{t}_{\mathbf{C}}$ induces a bijection from $\mathbf{C}\otimes \Gamma (C(G)_0)$ to $\mathfrak{c}$ and a bijection from $1\otimes R^{\vee}(G,T)$ to $2\pi i.R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

$b)$ The canonical isomorphism from $\mathbf{C}\otimes X(T)$ to the dual $\mathfrak{t}^*_{\mathbf{C}}$ of $\mathfrak{t}_{\mathbf{C}}$ induces a bijection from $\mathbf{C}\otimes X(T/(T\cap D(G)))$ to the orthogonal complement of $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}(\mathfrak{g})_{\mathbf{C}}$, and a bijection from $1\otimes R(G,T)$ to $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

#### Remark 2 {#lie-ix-s4-n9-rem-2 .statement tag=01CW}

Assume that the group G is semi-simple; denote by R (resp. $R^{\vee}$) the root system $R(G,T)$ (resp. $R^{\vee}(G,T)$), so that we have inclusions

$$
Q(R)\subset X(T)\subset P(R)Q(R^{\vee})\subset \Gamma (T)\subset P(R^{\vee})
$$

The finite abelian groups $P(R)/Q(R)$ and $P(R^{\vee})/Q(R^{\vee})$ are in duality (Chap. VI, §1, no. 9); if $\widehat{M}$ denotes the dual group of the finite abelian group M, we deduce from the preceding canonical isomorphisms

$$
\Gamma (T)/Q(R^{\vee})\rightarrow \pi_1(G)P(R^{\vee})/\Gamma (T)\rightarrow C(G)
$$

$$
P(R)/X(T)\rightarrow (\pi_1(G)\widehat{)}X(T)/Q(R)\rightarrow (C(G))\widehat{.}
$$

In particular, the product of the orders of $\pi_1(G)$ and C(G) is equal to the connection index $f$ of $R(G,T) ($loc. cit.).

Now let $G'$ be another connected compact Lie group, $T'$ a maximal torus of $G'$. Let $f: G\rightarrow G'$ be an isomorphism of Lie groups such that $f(T) = T'$; denote by $f_T$ the isomorphism from T to $T'$ that it defines. Then $X(f_T)$ is an isomorphism from $D^*(G',T')$ to $D^*(G,T)$, denoted by $D^*(f)$, and $\Gamma (f_T)$ is an isomorphism from $D_*(G,T)$ to $D_*(G',T')$, denoted by $D_*(f)$. If $t\in T$, and if we put $g=f\circ$ Int $t=$ (Int $f(t)$)$\circ f$, then $D^*(g) = D^*(f), D_*(g) = D_*(f)$.

#### Proposition 15 {#lie-ix-s4-prop-15 .statement tag=01CX}

Let $\varphi$ be an isomorphism from $D^*(G',T')$ to $D^*(G,T)$ (resp. from $D_*(G,T)$ to $D_*(G',T')$). There exists an isomorphism $f: G\rightarrow G'$ such that $f(T) = T'$ and $\varphi = D^*(f)$ (resp. $\varphi = D_*(f)$); if $f_1$ and $f_2$ are two such isomorphisms, there exists an element $t$ of T such that $f_2=f_1\circ$ Int $t$.

The second assertion follows immediately from Prop. 9 (no. 4); we prove the first for the covariant diagrams, for example. Denote by $\mathfrak{g}'$ (resp. $\mathfrak{t}'$) the Lie algebra of $G'$ (resp. $T'$), and by $\mathfrak{g}'_{\mathbf{C}}$ (resp. $\mathfrak{t}'_{\mathbf{C}}$) its complexified Lie algebra. By Chap. VIII, §4, no. 4, Th. 2 (i), there exists an isomorphism $\psi :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}'_{\mathbf{C}}$ that maps $\mathfrak{t}_{\mathbf{C}}$ to $\mathfrak{t}'_{\mathbf{C}}$ and induces on $\Gamma (T)\subset \mathfrak{t}_{\mathbf{C}}$ the given isomorphism $\varphi :\Gamma (T)\rightarrow \Gamma (T')$. Then $\mathfrak{g}$ and $\psi^{-1}(\mathfrak{g}')$ are two compact forms of $\mathfrak{g}_{\mathbf{C}}$ that have the same intersection $\mathfrak{t}$ with $\mathfrak{t}_{\mathbf{C}}$; by §3, no. 2, Prop. 3, there exists an inner automorphism $\theta$ of $\mathfrak{g}_{\mathbf{C}}$ inducing the identity on $\mathfrak{t}_{\mathbf{C}}$ and such that $\theta (\mathfrak{g}) =\psi^{-1}(\mathfrak{g}')$. By replacing $\psi$ by $\psi \circ \theta$, we can assume that $\psi$ maps $\mathfrak{g}$ to $\mathfrak{g}'$. Further, by Prop. 4 of no. 2, there exists a unique morphism $f_T: T\rightarrow T'$ such that $\Gamma (f_T) =\varphi$. Then the restriction of $\psi$ to $\mathfrak{t}$ is $L(f_T)$, and by §2, no. 6, Prop. 8, there exists a unique morphism $f: G\rightarrow G'$ that induces $f_T$ on T and $\psi$ on $\mathfrak{g}_{\mathbf{C}}$. Applying the preceding to $\varphi^{-1}$ and $\psi^{-1}$ we obtain an inverse morphism to $f$, which is therefore an isomorphism. Then $D_*(f) =\Gamma (f_T) =\varphi$, hence the proposition.

Note that, if T and $T'$ are two maximal tori of G, the diagrams $D^*(G,T)$ and $D^*(G,T')$ are isomorphic (if $g\in G$ is such that $gTg^{-1}= T'$, then Int $g$ is an isomorphism from G to G that maps T to $T'$). Denote by $D^*(G)$ the isomorphism class of $D^*(G,T)$ (cf. Theory of Sets, Chap. II, §6, no. 2); this is a root diagram that depends only on G and is called the contravariant diagram of G. The covariant diagram $D_*(G)$ of G is defined similarly, and we obtain:

#### Corollary {#lie-ix-s4-n9-cor-1 .statement tag=01CY}

Two connected compact Lie groups G and $G'$ are isomorphic if and only if the diagrams $D^*(G)$ and $D^*(G')$ (resp. $D_*(G)$ and $D_*(G')$) are equal.

#### Proposition 16 {#lie-ix-s4-prop-16 .statement tag=01CZ}

For every reduced root diagram D, there exists a connected compact Lie group G such that $D^*(G)$ (resp. $D_*(G)$) is isomorphic to D.

$a)$ By replacing D, if necessary, by its inverse diagram, we are reduced to constructing G such that $D^*(G)$ is isomorphic to D. Put $D = (M,M_0,R)$; then $\mathbf{Q}\otimes M$ is the direct sum of $\mathbf{Q}\otimes M_0$ and the vector subspace V(R) generated by R. Moreover, since the inverse roots take integer values on M, the projection of M on V(R) parallel to $\mathbf{Q}\otimes M_0$ is contained in the group of weights P(R) of R, so that M is a subgroup of $M_0\oplus P(R)$ of finite index. Denote by $D'$ the diagram $(M_0\oplus P(R),M_0,R)$.

$b)$ Let $\mathfrak{a}$ be a complex semi-simple Lie algebra whose canonical root system is isomorphic to $R\subset \mathbf{C}\otimes V(R)$ (Chap. VIII, §4, no. 3), and let $\mathfrak{g}_1$ be a compact real form of $\mathfrak{a}($§3, no. 2, Th. 1). Let $G_1$ be a simply-connected real Lie group whose Lie algebra is isomorphic to $\mathfrak{g}_1$; then $G_1$ is compact (§1, no. 4, Th. 1). Let $T_1$ be a maximal torus of $G_1$. By Th. 1, the diagram $D^*(G_1,T_1)$ is isomorphic to $(P(R),0,R)$.

$c)$ Let $T_0$ be a torus of dimension equal to the rank of $M_0$; then $D^*(T_0,T_0)$ is isomorphic to $(M_0,M_0,\emptyset )$, so $D^*(G_1\times T_0,T_1\times T_0)$ is isomorphic to $D'$ (Example 2).

$d)$ Finally, let N be the finite subgroup of $T_1\times T_0$ orthogonal to M. Put $G = (G_1\times T_0)/N, T = (T_1\times T_0)/N$. Then G is a connected compact Lie group, T a maximal torus of G, and $D(G,T)$ is isomorphic to D (Example 3).

#### Scholium {#lie-ix-s4-n9-sch-1 .statement tag=01D0}

The classification of connected compact Lie groups up to isomorphism is thus reduced to that of reduced root diagrams. The connected compact semi-simple Lie groups correspond to the reduced root diagrams $(M,M_0,R)$ such that $M_0= 0$; giving such a diagram is equivalent to giving a reduced root system R in a vector space V over $\mathbf{Q}$ and a subgroup M of V such that $Q(R)\subset M\subset P(R)$.

#### Remark 3 {#lie-ix-s4-n9-rem-3 .statement tag=01D1}

Let $T'$ be another maximal torus of G, B (resp. $B'$) a basis of the root system $R(G,T)$ (resp. $R(G',T')$) (Chap. VI, §1, no. 5, Def. 2). There exist elements $g\in G$ such that Int $g$ maps T onto $T'$ and B onto $B'$, and these elements form a unique coset modulo Int(T) (since T and $T'$ are conjugate, we can assume that $T = T'$, and it suffices to apply Chap. VI, §1, no. 5, Remark 4 and Prop. 9 of no. 4). It follows that the isomorphism from T to $T'$ induced by Int $g$ is independent of the choice of $g$; consequently the same is true of $D_*$(Int $g$) and $D^*$(Int $g$). Paraphrasing Chap. VIII, §5, no. 3, Remark 2, mutatis mutandis, we can now define the canonical maximal torus of G, the canonical covariant and contravariant root diagrams of $G,. .$..

### 10. AUTOMORPHISMS OF A CONNECTED COMPACT LIE GROUP

Denote by Aut(G) the Lie group of automorphisms of G (Chap. III, §10, no. 2), and by Aut(G$,T$) the closed subgroup of Aut(G) consisting of the elements $u$ such that $u(T) = T$. We have seen (§1, no. 4, Cor. 5 of Prop. 4) that the identity component of Aut(G) is the subgroup Int(G) of inner automorphisms; denote by Int$_G(H)$ the image in Int(G) of a subgroup H of G.

Let D be the covariant diagram of G relative to T; denote by Aut(D) the group of its automorphisms, and by W(D) its Weyl group. The map $u \rightarrow D_*(u)$ is a homomorphism from Aut(G$,T$) to Aut(D). Prop. 15 of no. 9 immediately gives:

#### Proposition 17 {#lie-ix-s4-prop-17 .statement tag=01D2}

The homomorphism Aut(G$,T$)$\rightarrow$ Aut(D) is surjective, with kernel Int$_G(T)$.

Note that Aut(G$,T$)$\cap$ Int(G) = Int$_G(N_G(T))$ and that the image of Int$_G(N_G(T))$ in Aut(D) is W(D) (no. 5, Prop. 10). Thus, Proposition 17 gives an isomorphism

Aut(G$,T$)$/$(Aut(G$,T$)$\cap$ Int(G)) $\rightarrow$ Aut(D)$/W(D)$.

Further, Aut(G) = Int(G).Aut(G$,T$). Indeed, if $u$ belongs to Aut(G), $u(T)$ is a maximal torus of T, hence is conjugate to T, and there exists an inner automorphism $v$ of G such that $u(T) =v$(T), in other words $v^{-1}u\in$ Aut(G$,T$). It follows that Aut(G)$/$Int(G) can be identified with Aut(G$,T$)$/$(Aut(G$,T$)$\cap$Int(G)), so in view of the preceding we have an exact sequence

$1\rightarrow$ Int(G) $\rightarrow$ Aut(G) $\rightarrow$ Aut(D)$/W(D)\rightarrow 1$. (16)

Consequently:

#### Proposition 18 {#lie-ix-s4-prop-18 .statement tag=01K9}

The group Aut(G)$/$Int(G) is isomorphic to Aut(D)$/W(D)$.

In particular, assume that G is semi-simple; the group Aut(D) can then be identified with the subgroup of $A(R(G,T))$ (Chap. VI, §1, no. 1) consisting of the elements $u$ such that $u(X(T))\subset X(T)$, and the subgroup W(D) can be identified with $W(R(G,T))$.

#### Corollary {#lie-ix-s4-n10-cor-1 .statement tag=01D3}

If G is simply-connected, or if C(G) reduces to the identity element, the group Aut(G)$/$Int(G) is isomorphic to the group of automorphisms of the Dynkin graph of $R(G,T)$.

This follows from the preceding and Chap. VI, §4, no. 2, Cor. of Prop. 1.

We are now going to show that the extension (16) admits sections.

For all $\alpha \in R(G,T)$, denote by $V(\alpha )$ the 2-dimensional vector subspace of $\mathfrak{g}$ such that $V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$; denote by K the quadratic form associated to the Killing form of $\mathfrak{g}$.

#### Definition 3 {#lie-ix-s4-def-3 .statement tag=01D4}

A framing of $(G,T)$ is a pair $(B,(U_{\alpha})_{\alpha\in B})$, where B is a basis of $R(G,T)$ (Chap. VI, §1, no. 5, Def. 2) and where, for all $\alpha \in B,U_{\alpha}$ is an element of $V(\alpha )$ such that $K(U_{\alpha}) =-1$.

A framing of G is a maximal torus T of G together with a framing of $(G,T)$.

#### Lemma 3 {#lie-ix-s4-lem-3 .statement tag=01D5}

Let $B_0$ be a basis of $R(G,T)$. The group Int$_G(T)$ operates simply-transitively on the set of framings of $(G,T)$ of the form $(B_0,(U_{\alpha})_{\alpha\in B_0})$.

For all $\alpha \in B_0$, denote by $K(\alpha )$ the restriction of the quadratic form K to $V(\alpha )$; the operation of T on $V(\alpha )$ defines a morphism $\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$. We have seen in no. 4 that $\mathbf{S}\mathbf{O}(K(\alpha ))$ can be identified with $\mathbf{U}$ in such a way that $\iota_{\alpha}$ is identified with the root $\alpha$. Since $B_0$ is a basis of R, it is a basis of the $\mathbf{Z}$-module Q(R) generated by the roots, hence a basis of the submodule $X(T/C(G))$ of X(T). It follows that the product of the morphisms $\iota_{\alpha}$ induces an isomorphism from $T/C(G)$ to the product of the groups $\mathbf{S}\mathbf{O}(K(\alpha ))$. But the latter group operates simply-transitively on the set of framings of $(G,T)$ whose first component is $B_0$.

#### Proposition 19 {#lie-ix-s4-prop-19 .statement tag=01D6}

The group Int(G) operates simply-transitively on the set of framings of G.

Let $e= (T,B,(U_{\alpha}))$ and $e'= (T',B',(U'_{\alpha}))$ be two framings of G. There exist elements $g$ in G such that (Int $g$)$(T) = T'$, and these elements form a single coset modulo $N_G(T)$. Thus, we can assume that $T = T'$, and we must prove that there exists a unique element of Int$_G(N_G(T))$ that transforms $e$ to $e'$. By Chap. VI, §1, no. 5, Remark 4, there exists a unique element $w$ of W(R) such that $w(B) = B'$. Since W(R) can be identified with $N_G(T)/T$, there exists $n\in N_G(T)$ such that $w=$ Int $n$, and $n$ is uniquely determined modulo T. Thus, we can assume that $B = B'$, and we must prove that there exists a unique element of Int$_G(T)$ that transforms $e$ to $e'$, which is simply Lemma 3.

#### Corollary {#lie-ix-s4-n10-cor-2 .statement tag=01D7}

Let $e$ be a framing of $(G,T)$ and let E be the group of automorphisms of G that leave $e$ stable. Then Aut(G) is the semi-direct product of E by Int(G), and Aut(G$,T$) is the semi-direct product of E by Int(G) $\cap$ Aut(G$,T$) $=$ Int$_G(N_G(T))$.

Indeed, every element of Aut(G) transforms $e$ into a framing of G. By Prop. 19, every coset of Aut(G) modulo Int(G) meets E in a single point, hence the first assertion. The second is proved in the same way.

#### Remark {#lie-ix-s4-n10-rem-1 .statement tag=01D8}

Let G and $G'$ be two connected compact Lie groups, and let $e=$ $(T,B,(U_{\alpha}))$ and $e'= (T',B',(U'_{\alpha}))$ be framings of G and $G'$, respectively. Let X be the set of isomorphisms from G to $G'$ that take $e$ to $e'$. The map $f \rightarrow D^*(f)$ (resp. $D_*(f)$) is a bijection from X to the set of isomorphisms from $D^*(G',T')$ to $D^*(G,T)$ (resp. $D_*(G,T)$ to $D_*(G',T')$) that map $B'$ to B (resp. B to $B'$). Indeed, this follows immediately from Prop. 15 and Lemma 3.

### Exercises {#lie-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
