---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 9
section_title: Compact Lie groups operating on manifolds
lang: en
source: lie-vii-ix
book_pages: 369-381, 419-424
pdf_pages: 0376-0388, 0426-0431
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING OF A MANIFOLD IN THE NEIGHBOURHOOD OF A COMPACT SET
      page: 369
      pdf_page: 376
    - "no": 2
      title: EQUIVARIANT EMBEDDING THEOREM
      page: 373
      pdf_page: 380
    - "no": 3
      title: TUBES AND TRANSVERSALS
      page: 375
      pdf_page: 382
    - "no": 4
      title: ORBIT TYPES
      page: 377
      pdf_page: 384
statements: 19
exercises: 21
errata:
    - says: §5, no. 2, Cor. of Prop. 2
      read: §5, no. 2, Cor. 1 of Prop. 2
      why: No. 2 of section 5 prints three numbered corollaries of Proposition 2 and the reference does not say which. The sentence citing it has G simply-connected and A an alcove, and says that the composite map from A to $G_r/$Int(G) is a homeomorphism. That is Corollary 1 b), whose homeomorphisms run $A/H_A$ to $T_r/W$ to $G_r/$Int(G) and whose $H_A$ is trivial for a simply-connected group. Corollary 2 is the same statement for the Lie algebra, over a chamber rather than an alcove, and Corollary 3 is about existence and uniqueness and names no map at all.
content_sha256: b8936dcc268d7bea36184c52ccdb7af0532e90195e7dcf0f7b65dfb8f7462b9f
---

## § 9. COMPACT LIE GROUPS OPERATING ON MANIFOLDS

In this paragraph, X denotes a separated, locally finite dimensional, real manifold of class $C^r(1\leq r\leq \omega )$.

### 1. EMBEDDING OF A MANIFOLD IN THE NEIGHBOURHOOD OF A COMPACT SET

#### Lemma 1 {#lie-ix-s9-lem-1 .statement tag=01HE}

Let T and $T'$ be two topological spaces, A and $A'$ compact subsets of T and $T'$, respectively, W a neighbourhood of $A\times A'$ in $T\times T'$. There exists an open neighbourhood U of A in T and an open neighbourhood $U'$ of $A'$ in $T'$ such that $U\times U'\subset W$.

Let $x\in A$; there exist open subsets $U_x$ of T and $U'_x$ of $T'$ such that $\{x\} \times A'\subset U_x\times U'_x\subset W:$ indeed, the compact subset $\{x\} \times A'$ of $T\times T'$ can be covered by a finite number of open sets contained in W, of the form $U_i\times U'_i$, with $x\in U_i$; it suffices to take $U_x=\bigcap_iU_i$ and $U'_x=\bigcup_iU'_i$.

Since A is compact, there exist points $x_1, . . . , x_m$ of A such that $A\subset \bigcup_iU_{x_i}$; put $U =\bigcup_iU_{x_i}$ and $U'=\bigcap_iU'_{x_i}$. Then $A\times A'\subset U\times U'\subset W$, hence the lemma.

In the remainder of this number, Y denotes a separated manifold of class $C^r$.

#### Proposition 1 {#lie-ix-s9-prop-1 .statement tag=01HF}

Let $\varphi : X\rightarrow Y$ be a morphism of class $C^r$, A a compact subset of X. The following conditions are equivalent:

(i) The restriction of $\varphi$ to A is injective, and $\varphi$ is an immersion at every point of A;

(ii) there exists an open neighbourhood U of A such that $\varphi$ induces an embedding of U into Y.

When these conditions are satisfied, $\varphi$ is said to be an embedding in the neighbourhood of A.

We prove that (i) implies (ii), the other implication being clear. Assuming (i), there exists an open neighbourhood V of X containing A such that the restriction of $\varphi$ to V is an immersion (Differentiable and Analytic Manifolds, Results, 5.7.1). Denote by $\Gamma$ the set of points $(x, y)$ in $V\times V$ such that $\varphi (x) =\varphi (y)$, and by $\Delta$ the diagonal in $V\times V$. Then $\Delta$ is an open subset of $\Gamma :$ indeed, for all $x\in V$, there exists an open neighbourhood $U_x$ of $x$ such that the restriction of $\varphi$ to $U_x$ is injective, that is, such that $\Gamma \cap (U_x\times U_x) =$ $\Delta \cap (U_x\times U_x)$.

Since Y is separated, $\Gamma$ is closed in $V\times V$; consequently the complement W of $\Gamma$ **--** $\Delta$ in $V\times V$ is open. By assumption, W contains $A\times A$; Lemma 1 implies that there exists an open subset $U'$ of V containing A such that $U'\times U'\subset W$, that is, such that the restriction of $\varphi$ to $U'$ is injective. Moreover, there exists an open neighbourhood U of A whose closure is compact and contained in $U'($General Topology, Chap. I, §9, no. 7, Prop. 10). Then $\varphi$ induces a homeomorphism from U to $\varphi$(U), and consequently from U to $\varphi (U)$; it follows that the restriction of $\varphi$ to U is an embedding (Differentiable and Analytic Manifolds, Results, 5.8.3).

#### Proposition 2 {#lie-ix-s9-prop-2 .statement tag=01HG}

Assume that the manifold Y is paracompact; let A be a subset of X, and let $\varphi :X\rightarrow Y$ be a morphism of class $C^r$ that induces a homeomorphism from A to $\varphi (A)$, and that is étale at every point of A. Then there exists an open neighbourhood U of A such that $\varphi$ induces an isomorphism from U to an open submanifold of Y.

Restricting X and Y if necessary, we can assume that $\varphi$ is étale and surjective. Denote by $\sigma :\varphi (A)\rightarrow A$ the inverse homeomorphism of $\varphi |A$. Since Y is metrizable (Differentiable and Analytic Manifolds, Results, 5.1.6), $\varphi (A)$ admits a fundamental system of paracompact neighbourhoods; hence, by General Topology, Chap. XI, there exist an open neighbourhood V of $\varphi (A)$ in Y and a continuous map $s: V\rightarrow X$, that coincides with $\sigma$ on $\varphi (A)$ and is such that $\varphi (s(y)) =y$ for all $y\in V$. Moreover, $s$ is topologically étale, so $s(V)$ is an open set U containing A. Then $\varphi$ induces a homeomorphism $\varphi '$ from U to V; by Differentiable and Analytic Manifolds, Results$, 5.7.8,\varphi '$ is an isomorphism.

In the remainder of this number, we assume that $r\not=\omega$.

#### Proposition 3 {#lie-ix-s9-prop-3 .statement tag=01HH}

Let A be a compact subset of X. The set $\mathscr{P}$ of morphisms $\varphi \in \mathscr{C}^r(X;Y)$ that are embeddings in the neighbourhood of A is open in $\mathscr{C}^r(X;Y)$ in the topology of compact $C^r$-convergence (§ 6, no. 4).

Clearly, it suffices to prove the proposition for $r= 1$.

$a)$ We show first that the subset J of $\mathscr{C}^1(X;Y)$ consisting of the morphisms that are immersions at every point of A is open. Consider the map $j_A:\mathscr{C}^1(X;Y)\times A\rightarrow J^1(X;Y)$ such that $j_A(\varphi , x) =j_x^1(\varphi ) ($Differentiable and Analytic Manifolds, Results, 12.1).

By definition of the topology on $\mathscr{C}^1$(X;Y), the map $\widetilde{j}_A:\varphi \rightarrow j_A(\varphi , .)$ from $\mathscr{C}^1(X;Y)$ to $\mathscr{C}(A;J^1(X;Y))$ is continuous; it now follows from General Topology, Chap. X, §3, no. 4, Th. 3, that $j_A$ is continuous.

On the other hand, let M be the set of jets $j$ in $J^1(X;Y)$ whose tangent map $T(j) : T_{\mathbf{s}(j)}(X)\rightarrow T_{\mathbf{b}(j)}(Y) ($Differentiable and Analytic Manifolds, Results, 12.3.4) is injective. The set M is open in $J^1(X;Y)$; indeed, it suffices to verify this assertion when X is an open subset of a finite dimensional vector space E, and Y is an open subset of a Banach space F; we are then reduced (Differentiable and Analytic Manifolds, Results, 12.3.1) to proving that the set of injective continuous linear maps is open in $\mathscr{L}$(E;F), which follows from Spectral Theory, Chap. III, §2, no. 7, Prop. 16.

We conclude from the preceding that the set $j_A^{-1}(M)$ is open in $\mathscr{C}^1(X;Y)\times A$, hence that its complement $\mathscr{F}$ is closed. Since A is compact, the projection pr$_1:\mathscr{C}^1(X;Y)\times A\rightarrow \mathscr{C}^1(X;Y)$ is a proper morphism, hence closed; consequently, the set J, which is equal to $\mathscr{C}^1(X;Y)$ **--** pr$_1(\mathscr{F})$, is open in $\mathscr{C}^1(X;Y)$.

$b)$ Let H be the subset of $J\times A\times A$ consisting of the elements $(f, x, y)$ such that $f(x) =f(y)$. It is clear that H contains $J\times \Delta$, where $\Delta$ denotes the diagonal in the product $A\times A$; we show that $H'= H$ **--** $(J\times \Delta )$ is closed in $J\times A\times A$. Since $\mathscr{P}$ is the complement in J of the image of $H'$ under the proper projection pr$_1: J\times A\times A\rightarrow J$, this will imply the proposition.

The topology of $\mathscr{C}^1(X;Y)$ being finer than the topology of compact convergence, the map $(\varphi , x) \rightarrow \varphi (x)$ from $\mathscr{C}^1(X;Y)\times A$ to Y is continuous (General Topology, Chap. X, §3, no. 4, Cor. 1 of Th. 3); it follows that H is closed in $J\times A\times A$. Hence, it suffices to show that $J\times \Delta$ is open in H, in other words, that for all $\varphi \in J$ and all $x\in A$ there exists a neighbourhood $\Omega$ of $\varphi$ in J and a neighbourhood B of $x$ in X such that, for any morphism $\psi$ in $\Omega$, the restriction of $\psi$ to $A\cap B$ is injective.

Thus, the proposition follows from the following lemma:

#### Lemma 2 {#lie-ix-s9-lem-2 .statement tag=01HI}

Let $x$ be a point of X$,\varphi : X\rightarrow Y$ a morphism of class $C^1$ that is an immersion at $x$. There exists a neighbourhood $\Omega$ of $\varphi$ in $\mathscr{C}^1(X;Y)$ and a neighbourhood B of $x$ in X such that, for all $\psi \in \Omega$, the restriction of $\psi$ to B is injective.

Let U be a relatively compact open neighbourhood of $x$ isomorphic to a finite dimensional vector space, and such that $\varphi (U)$ is contained in the domain V of a chart. The set $\Omega_0$ of $\psi \in \mathscr{C}^1(X;Y)$ such that $\psi (U)\subset V$ is open in $\mathscr{C}^1$(X;Y), and the restriction map $\Omega_0\rightarrow \mathscr{C}^1(U;V)$ is continuous; we are thus reduced to proving the lemma when X = U and Y = V, in other words, we can assume that X is a finite dimensional vector space and Y is a Banach space. Choose norms on X and Y.

The linear map $D\varphi (x) : X\rightarrow$ Y is injective; denote its conorm by $q($Spectral Theory, Chap. III, §2, no. 6), so that, by definition, we have $\|D\varphi (x).t\| \geq q\|t\|$ for all $t\in X$. Let $\varepsilon \in \mathbf{R}$ be such that $0< \varepsilon  < q/2$, and let B be a closed ball with centre $x$ such that $\|D\varphi (u)-D\varphi (x)\| \leq \varepsilon$ for all $u\in B$. Denote by $\Omega$ the subset of $\mathscr{C}^1(X;Y)$ consisting of the morphisms $\psi$ such that $\|D\psi (u)-D\varphi (u)\| \leq \varepsilon$ for all $u\in B$; it is open by definition of the topology of $\mathscr{C}^1(X;Y)$. For $\psi \in \Omega$, put $\psi_0=\psi -D\varphi (x)$. We have $\|D\psi_0(u)\| \leq 2\varepsilon$ for all $u\in B$, and consequently $\|\psi_0(u)-\psi_0(v)\| \leq 2\varepsilon \|u-v\|$ for all $u$ and $v$ in B (Differentiable and Analytic Manifolds, Results, 2.2.3). It follows that

$$
\|\psi (u)-\psi (v)\| \geq  \|D\varphi (x).(u-v)\| - \|\psi_0(u)-\psi_0(v)\| \geq (q-2\varepsilon )\|u-v\|
$$

Consequently, the restriction of $\psi$ to B is injective, hence the lemma.

#### Proposition 4 {#lie-ix-s9-prop-4 .statement tag=01HJ}

Let A be a compact subset of X. There exist a finite dimensional vector space E and a morphism $\varphi \in \mathscr{C}^r(X;E) (r\not=\omega )$ that is an embedding in the neighbourhood of A.

Let $(U_i, \varphi_i,E_i)_{i\in I}$ be a finite family of charts of X whose domains cover A. We extend $\varphi_i$ to a map from X to $E_i$ (also denoted by $\varphi_i)$ by putting $\varphi_i(x) = 0$ for $x /\in U_i$. Let $(V_i)_{i\in I}$ be a covering of A by open subsets of X such that $\overline{V}_i\subset U_i$ for all $i\in I$ (the existence of such a covering follows from General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3, applied to the compact space $X'$ obtained by adjoining to X a point at infinity and the covering of $X'$ consisting of the open sets $U_i(i\in I)$ and $X'$ **--** A). For all $i\in I$, let $\alpha_i$ be a numerical function of class $C^r$ on X, equal to 1 at every point of $V_i$, and with support contained in $U_i($Differentiable and Analytic Manifolds, Results, 5.3.6).

Consider the map $\varphi : X\rightarrow \bigoplus_{i\in I}(E_i\oplus \mathbf{R})$ defined by

$$
\varphi (x) = (\alpha_i(x)\varphi_i(x), \alpha_i(x))_{i\in I}
$$

For all $i\in I$, the map $\alpha_i\varphi_i$ is of class $C^r$ (since its restrictions to $U_i$ and to the complement of the support of $\alpha_i$ are), and its restriction to $V_i$ is an embedding; it follows that $\varphi$ is a morphism of class $C^r$ and is an immersion at every point of A. We show that the restriction of $\varphi$ to A is injective. Let $x, y$ be two points of A such that $\varphi (x) =\varphi (y)$, and let $i\in I$ be such that $x\in V_i$. Then $\alpha_i(x) = 1$, so $\alpha_i(y) = 1$, which implies that $y\in U_i$; but we also have $\varphi_i(x) =\varphi_i(y)$, so $x=y$ since $\varphi_i$ induces an embedding of $U_i$ into $E_i$.

It can be shown$^9$ that every separated manifold, countable at infinity and of

pure dimension $n$, embeds in $\mathbf{R}^{2n}$; for a weaker result, cf. Exercise 2.

$^9$ See H. WHITNEY, The self-intersections of a smooth $n$-manifold in $2n$-space,

Ann. of Math., 45 (1944), pp. 220-246.

### 2. EQUIVARIANT EMBEDDING THEOREM

In this number, we assume that $r\not=\omega$.

#### Lemma 3 {#lie-ix-s9-lem-3 .statement tag=01HK}

Let G be a compact topological group operating continuously on a topological space X; let A be a subset of X, stable under G, and W a neighbourhood of A. Then, there exists an open neighbourhood V of A stable under G and contained in$_{\circ}W$.

Put F = X **--** W and V = X**--** GF. Then V is open (General Topology, Chap. III, §4, no. 1, Cor. 1 of Prop. 1), stable under G, and $A\subset V\subset W$.

#### Theorem 1 {#lie-ix-s9-thm-1 .statement tag=01HL}

Let G be a compact Lie group, $(g, x) \rightarrow gx$ a law of left operation of class $C^r$ of G on X, and A a compact subset of X. There exists an analytic linear representation $\rho$ of G on a finite dimensional vector space E, a morphism $\varphi : X\rightarrow E$ of class $C^r$, compatible with the operations of G, and an open neighbourhood U of A, stable under G, such that the restriction of $\varphi$ to U is an embedding.

Replacing A by the compact set GA, we are reduced to the case in which A is stable under G.

Let $E_0$ be a finite dimensional vector space such that there exists an element of $\mathscr{C}^r(X;E_0)$ that is an embedding in the neighbourhood of A (no. 1, Prop. 4); the set $\mathscr{P}$ of morphisms having this property is a non-empty open subset of $\mathscr{C}^r(X;E_0)$ (no. 1, Prop. 3). Consider the continuous linear representation of the compact group G on the space $\mathscr{C}^r(X;E_0) ($§6, no. 4, Lemma 4). By the Peter-Weyl theorem (Spectral Theory, in preparation), the union of the finite dimensional subspaces stable under G is dense in $\mathscr{C}^r(X;E_0)$; hence, there exists an element $\varphi_0$ of $\mathscr{P}$ such that the maps $x \rightarrow \varphi_0(gx)$, for $g\in G$, generate a finite dimensional vector subspace $E_1$ of $\mathscr{C}^r(X;E_0)$, which is clearly stable under the operation of G.

Take E to be the space Hom$_{\mathbf{R}}(E_1,E_0),\rho$ to be the representation of G on E induced by the action on $E_1$, and $\varphi : X\rightarrow E$ to be the map that associates to $x\in X$ the linear map $\psi  \rightarrow \psi (x)$ from $E_1$ to $E_0$. This is a morphism of class $C^r$; for $x\in X,g\in G,\psi \in E_1$, we have (denoting by $\tau (g)$ the automorphism $x \rightarrow gx$ of X):

$$
\varphi (gx)(\psi )-\psi (gx) =\varphi (x)(\psi \circ \tau (g)) = (\rho (g)\varphi (x))(\psi )
$$

Let $\alpha :$ Hom$_{\mathbf{R}}(E_1,E_0)\rightarrow E_0$ be the linear map $u \rightarrow u(\varphi_0)$; we have $\alpha \circ \varphi =\varphi_0$, so $\varphi$ is an embedding in the neighbourhood of A because $\varphi_0$ is one. Hence, there exists an open neighbourhood U of A such that the restriction of $\varphi$ to U is an embedding; we can choose U stable under G by Lemma 3, hence the theorem.

#### Corollary 1 {#lie-ix-s9-thm-1-cor-1 .statement tag=01HM}

Assume that X is compact. There exists an analytic linear representation $\rho$ of G on a finite dimensional vector space E and an embedding $\varphi : X\rightarrow E$ such that $\varphi (gx) =\rho (g)\varphi (x)$ for $g\in G, x\in X$.

#### Corollary 2 {#lie-ix-s9-thm-1-cor-2 .statement tag=01HN}

Let H be a closed subgroup of G. There exists an analytic linear representation of G on a finite dimensional vector space E and a point $v\in E$ with fixer H.

Apply Cor. 1 to the canonical operation of G on the compact manifold $G/H$. This gives an analytic linear representation $\rho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ and an embedding $\varphi : G/H\rightarrow E$ such that $\varphi (gx) =\rho (g)\varphi (x),g\in G, x\in G/H$. Let $\overline{e}\in G/H$ be the class of $e\in G$, and $v=\varphi (\overline{e})$ its image. For all $g\in G$, we have $\rho (g)v=v\Leftarrow \Rightarrow \varphi (g\overline{e}) =\varphi (\overline{e})\Leftarrow \Rightarrow g\overline{e}= \overline{e}\Leftarrow \Rightarrow g\in H$.

#### Corollary 3 {#lie-ix-s9-thm-1-cor-3 .statement tag=01HO}

Assume that X is paracompact. There exists a real Hilbert space E, a continuous unitary representation $^{10}\rho$ of G on E and an embedding $\varphi : X\rightarrow E$ of class $C^r$ such that $\varphi (gx) =\rho (g)\varphi (x)$ for all $g\in G$ and all $x\in X$.

The space $X/G$ is locally compact (General Topology, Chap. III, §4, no. 5, Prop. 11). Its connected components are the images of the connected components of X, which are countable at infinity (General Topology, Chap. I, §9, no. 10, Th. 5); thus, they are themselves countable at infinity, which implies that $X/G$ is paracompact (loc. cit.). Hence, there exists a locally finite covering $(U'_{\alpha})_{\alpha\in I}$ of $X/G$ by relatively compact open sets, and a covering $(V'_{\alpha})_{\alpha\in I}$ such that $\overline{V}'_{\alpha}\subset U'_{\alpha}$ for all $\alpha \in I ($General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3); taking the inverse image, we obtain two locally finite coverings $(U_{\alpha})_{\alpha\in I}$ and $(V_{\alpha})_{\alpha\in I}$ of X by relatively compact open sets stable under G, such that $\overline{V}_{\alpha}\subset U_{\alpha}$ for all $\alpha \in I$.

For all $\alpha \in I$, there exists a representation $\rho_{\alpha}$ of G on a finite dimensional real vector space $E_{\alpha}$ and a morphism $\varphi_{\alpha}\in \mathscr{C}^r(X;E_{\alpha})$, compatible with the operations of G, whose restriction to $U_{\alpha}$ is an embedding (Th. 1). For $\alpha \in I$, let $a_{\alpha}$ be a numerical function of class $C^r$ on X, equal to 1 on $V_{\alpha}$ and to 0 outside $U_{\alpha}($Differentiable and Analytic Manifolds, Results, 5.3.6). Put $b_{\alpha}(x) =\int_Ga_{\alpha}(gx)dg$ for $x\in X$. The function $b_{\alpha}$ is of class $C^r$, invariant under G (§6, no. 4, Cor. 2), equal to 1 on $V_{\alpha}$ and to 0 outside $U_{\alpha}$. Give each $E_{\alpha}$ a Hilbert scalar product invariant under G (§1, no. 1), and $\mathbf{R}$ its canonical Hilbert structure; let E be the Hilbert sum of the family $(E_{\alpha}\oplus \mathbf{R})_{\alpha\in I}$, and let $\rho$ be the representation of G on E induced by the $\rho_{\alpha}$ and the trivial action of G on $\mathbf{R}$. For $x\in X$, put $\varphi (x) = (b_{\alpha}(x)\varphi_{\alpha}(x), b_{\alpha}(x))_{\alpha\in I}$. Then $\varphi$ is a morphism of class $C^r$ from X to E, compatible with the operations of G; we verify as in the proof of Prop. 4 (no. 1) that $\varphi$ is an embedding, which implies the corollary.

$^{10}$That is (Spectral Theory, in preparation) a continuous linear representation (Integration, Chap. VIII, §2, no. 1) such that the operator $\rho (g)$ is unitary for all

$$
g\in G
$$

### 3. TUBES AND TRANSVERSALS

#### Lemma 4 {#lie-ix-s9-lem-4 .statement tag=01HP}

Let H be a compact Lie group, $\rho : H\rightarrow \mathbf{G}\mathbf{L}(V)$ a continuous (hence analytic) representation of H on a finite dimensional real vector space, and W a neighbourhood of the origin in V. There exists an open neighbourhood B of the origin, contained in W and stable under H, and an analytic isomorphism $u: V\rightarrow B$, compatible with the operations of H, such that $u(0) = 0$ and $Du(0) =$ Id$_V$.

Choose a scalar product on V invariant under H (§1, no. 1). There exists a real number $r >0$ such that the open ball B of radius $r$ is contained in W; it is clearly stable under H. Put $u(v) =r(r^2+\|v\|^2)^{-1/2}v$ for all $v\in V$; then $u$ is a bijective analytic map from V to B, compatible with the operations of H, and its inverse map $w \rightarrow r(r^2- \|w\|^2)^{-1/2}w$ is analytic. Moreover, $u(0) = 0$ and $Du(0) =$ Id$_V$.

#### Proposition 5 {#lie-ix-s9-prop-5 .statement tag=01HQ}

Let H be a compact Lie group, $(h, x) \rightarrow hx$ a law of left operation of class $C^r$ of H on X, and $x$ a point of X fixed under the operation of H. Then the group H operates linearly on the vector space $T = T_x(X)$; there exists an open embedding $\varphi : T\rightarrow X$ of class $C^r$, compatible with the operations of H, such that $\varphi (0) =x$ and $T_0(\varphi )$ is the identity map of T.

Let $(U, \psi ,E)$ be a chart of X at $x$, such that U is stable under H (no. 2, Lemma 3) and such that $\psi (x) = 0$. Identify E with T by means of $T_x(\psi )$, and put

$\psi^{\sharp}(y) =\int_Hh.\psi (h^{-1}y)dh$ for $y\in U$,

where $dh$ is the Haar measure on H of total mass 1.

Then (§6, no. 4, Cor. $1)\psi^{\sharp}$ is a morphism of class $C^r$ from U to T, compatible with the operations of H, such that $\psi^{\sharp}(x) = 0$ and $d_x\psi^{\sharp}=$ Id$_T$. Hence, there exists an open set $U'\subset U$ containing $x$, and an open neighbourhood V of 0 in T, such that $\psi^{\sharp}$ induces an isomorphism $\theta : U'\rightarrow V$. Restricting $U'$ and V if necessary, we can assume that they are stable under H and that there exists an isomorphism $u: T\rightarrow V$ compatible with the operations of H (Lemma 4). It now suffices to take $\varphi =\theta^{-1}\circ u$.

Recall (Differentiable and Analytic Manifolds, Results, 6.5.1) that if G is a Lie group, H a Lie subgroup of G and Y a manifold on which H operates on the left, we denote by $G\times^HY$ the quotient of the product manifold $G\times Y$ by the right operation $((g, y), h) \rightarrow (gh, h^{-1}y)$ of H; this is a manifold on which the Lie group G operates naturally on the left; the projection $G\times^HY\rightarrow G/H$ is a bundle with fibre Y. Further, if Y is a finite dimensional vector space on which H operates linearly, $G\times^HY$ has a natural structure of vector G-bundle with base $G/H ($Differentiable and Analytic Manifolds, Results, 7.10.2).

Let G be a Lie group operating properly on the manifold X (General Topology, Chap. III, §4, no. 1, Def. 1) such that the law of operation $(g, x) \rightarrow gx$ is of class $C^r$. Then, for every point $x$ of X, the orbit $Gx$ of $x$ is a closed submanifold of X, isomorphic to the Lie homogeneous space $G/G_x$, where $G_x$ is the fixer of $x$ in G (cf. Chap. III, §1, no. 7, Prop. 14 (ii), and General Topology, Chap. III, §4, no. 2, Prop. 4); this is a compact Lie group (loc. cit.).

#### Proposition 6 {#lie-ix-s9-prop-6 .statement tag=01HR}

Assume that the manifold X is paracompact; let $x$ be a point of X, $G_x$ its fixer. There exists a finite dimensional analytic linear representation $\tau : G_x\rightarrow \mathbf{G}\mathbf{L}(W)$, and an open embedding $\alpha : G\times^{G_x}W\rightarrow X$ of class $C^r$, compatible with the operations of G, that maps the class of $(e,0)\in G\times W$ to $x$.

Put $T = T_x(X)$. Let W be a complementary subspace of $T_x(Gx)$ in T, stable under $G_x$ (for example, the orthogonal complement of $T_x(Gx)$ with respect to a scalar product on T invariant under $G_x)$. On the other hand, let $\varphi : T\rightarrow X$ be a morphism with the properties stated in Prop. 5 (relative to $H = G_x)$. Consider the morphism $\lambda : G\times W\rightarrow X$ defined by $\lambda (g, w) =g\varphi (w)$. It induces by passage to the quotient a morphism $\mu: G\times^{G_x}W\rightarrow X$ of class $C^r$, compatible with the operations of G, that maps the class $z$ of $(e,0)$ to $x$.

We show that $\mu$ is étale at the point $z$. We have

dim(G $\times^{G_x}W) =$ dim(G) + dim(W) $-$ dim(G$_x)$

= dim(G$x) +$ dim(W) = dim(T),

so it suffices to show that $\mu$ is submersive at $z$, or equivalently that $\lambda$ is submersive at $(e,0)$. But, the tangent map $T_{(e,0)}(\lambda ) : T_e(G)\oplus W\rightarrow T$ is equal to $T_e(\rho (x)) +i$, where $\rho (x)$ is the orbital map $g \rightarrow gx$ and $i$ the canonical injection from W to T; since Im $T_e(\rho (x)) = T_x(Gx)$, the map $T_{(e,0)}(\lambda )$ is surjective, and $\mu$ is étale at $z$.

We are going to show that there exists an open neighbourhood $\Omega$ of $Gz$ in $G\times^{G_x}W$, stable under G, such that $\mu$ induces an isomorphism from $\Omega$ onto an open subset of X. This will imply the proposition: indeed, the inverse image of $\Omega$ in $G\times W$ is stable under G, and hence is of the form $G\times B$, where B is an open subset of W containing the origin and stable under $G_x$; restricting $\Omega$ if necessary, we can assume that there exists an isomorphism $u: W\rightarrow B$, compatible with the operations of $G_x$ (Lemma 4). It is clear that the composite morphism $\alpha : G\times^{G_x}W\overset{(Id,u)}{\longrightarrow}G\times^{G_x}B\longrightarrow^\mu$ X satisfies the conditions in the statement of the proposition.

Thus, the proposition is a consequence of the following lemma:

#### Lemma 5 {#lie-ix-s9-lem-5 .statement tag=01HS}

Let Z be a separated manifold of class $C^r$, equipped with a law of left operation $m: G\times Z\rightarrow Z$ of class $C^r$, and $\mu: Z\rightarrow X$ a morphism (of class $C^r)$ compatible with the operations of G. Let $z$ be a point of Z, and $x=\mu(z)$. Assume that $\mu$ is étale at $z$, and that the fixer of $z$ in G is equal to the fixer $G_x$ of $x$. Then, there exists an open neighbourhood $\Omega$ of the orbit $Gz$, stable under G, such that $\mu$ induces an isomorphism from $\Omega$ onto an open subset of X.

Since $\mu$ is compatible with the operations of G, it is étale at every point of $Gz$; since the canonical map $G/G_x\rightarrow Gx$ is a homeomorphism, so is the map from $Gz$ to $Gx$ induced by $\mu$. Hence, it follows from Prop. 2 of no. 1 that there exists an open neighbourhood U of $Gz$ in Z such that $\mu$ induces an open embedding of U into X.

Since G operates properly on X, there exists an open neighbourhood V of $x$ and a compact subset K of G such that $gV\cap V =\emptyset$ for $g /\in K ($General Topology, Chap. III, §4, no. 4, Prop. 7); in particular, $e\in K$. The set $W_1$ of points $y\in Z$ such that $Ky\subset U$ is open in Z: indeed, Z**--** $W_1$ is the image of the closed set $(K\times Z)$ **--** $m^{-1}(U)$ under the proper projection pr$_2: K\times Z\rightarrow Z$. Put $W = W_1\cap \mu^{-1}(V)$; this is an open subset of Z, containing $z$, and satisfying the following conditions:

(i) KW $\subset U$, and in particular $W\subset U$;

(ii) $\mu(W)\subset V$.

Put $\Omega =$ GW and consider the restriction of $\mu$ to $\Omega$. This is an étale morphism, since every point of $\Omega$ is conjugate under G to a point of U. We show that it is injective: let $g, h$ in G and $u, v$ in W be such that $\mu(gu) =$ $\mu(hv)$. Put $k=g^{-1}h$; then $\mu(u) =k\mu(v)$, so $k\in K$ by (ii). But $kv$ and $u$ belong to U by (i); thus, $u=kv$ because the restriction of $\mu$ to V is injective, so $gu=hv$. Hence, the restriction of $\mu$ to $\Omega$ is injective, and consequently (Differentiable and Analytic Manifolds, Results, 5.7.8) is an isomorphism onto an open submanifold of X, which completes the proof.

Under the conditions of Prop. 6, the image of $\alpha$ is an open neighbourhood T of the orbit A of $x$, equipped with the structure of vector bundle with base A, for which the zero section is the orbit A itself. Such a neighbourhood is called a linear tube (around the orbit in question). For each point $a\in A$, the fibre $Y_a$ of this vector bundle is a submanifold of X, stable under the fixer $G_a$ of $a$, and such that the morphism from $G\times^{G_a}Y_a$ to X that maps the class of $(g, y)\in G\times Y_a$ to $gy\in X$ induces a morphism of class $C^r$ from $G\times^{G_a}Y_a$ to T. Then $Y_a$ is said to be the transversal at $a$ of the tube T. We remark that the tangent space at $a$ of $Y_a$ is canonically isomorphic to $Y_a$ and that it is a complement of $T_a(A)$ in $T_a(X)$; thus, the vector bundle T with base A is canonically isomorphic to the normal bundle of A in X (Differentiable and Analytic Manifolds, Results, 8.1.3).

### 4. ORBIT TYPES

Let G be a topological group operating continuously on a separated topological space E. For every point $x$ of E, denote by $G_x$ the fixer of $x$ in G, and assume that the canonical map $G/G_x\rightarrow Gx$ is a homeomorphism; this is notably the case in the following two situations:

$a)$ the topologies of G and E are discrete;

$b) G$ operates properly on E (General Topology, Chap. III, §4, no. 2, Prop. 4), for example, G is compact (General Topology, Chap. III, §4, no. 1, Prop. 2).

Denote by $\mathscr{T}$ the set of conjugacy classes of closed subgroups of G. For every $x\in E$, we call the orbit type of $x$, or sometimes the type of $x$, the class of $G_x$ in $\mathscr{T}$; two points of the same orbit are of the same orbit type (Algebra, Chap. I, §5, no. 2, Prop. 2); two orbits are of the same type if and only if they are isomorphic as G-sets (Algebra, Chap. I, §5, no. 5, Th. 1). For every $t\in \mathscr{T}$, denote by $E_{(t)}$ the set of points of E of type $t$, that is, the union of the orbits of type $t$; this is a stable subset of E. For $H\in t$, we also write $E_{(H)}$ for $E_{(t)}$; for example, $E_{(G)}$ is the closed subspace of E consisting of the points fixed by G.

Give $\mathscr{T}$ the following preorder relation:

$t\leq t'\Leftarrow \Rightarrow$ there exists $H\in t$ and $H'\in t'$ such that $H\supset H'$.

Let $\Omega$ and $\Omega '$ be two orbits of G on $E,t$ and $t'$ their types; then $t\leq t'$ if and only if there exists a G-morphism (necessarily surjective and continuous) from $\Omega '$ to $\Omega$.

Let $x, x'$ be in E, and $t, t'$ their types; then $t\leq t'$ if and only if there exists $a\in G$ such that $aG_{x'}a^{-1}\subset G_x$.

#### Lemma 6 {#lie-ix-s9-lem-6 .statement tag=01HT}

Let G be a Lie group.

a) Every decreasing sequence of compact subgroups of G is stationary.

b) Let H and $H'$ be two compact subgroups of G such that $H\subset H'$ and such that there exists an isomorphism (of topological groups) from $H'$ to H. Then $H = H'$.

c) With the relation $t\leq t'$, the set $\mathscr{T}$ is a noetherian ordered set (Theory of Sets, Chap. III, §6, no. 5, text preceding Prop. 7).

$a)$ Let $(H_i)_{i\geq 1}$ be a decreasing sequence of compact subgroups of G; these are Lie subgroups of G (Chap. III, §8, no. 2, Th. 2). The sequence of integers (dim $H_i)_{i\geq 1}$ is decreasing, hence stationary, so there exists an integer N such that the subgroups $H_i$ have the same identity component for $i\geq N$. Then the decreasing sequence of positive integers $(H_i: (H_i)_0)_{i\geq N}$ is stationary, so $H_i= H_{i+1}$ for $i$ sufficiently large.

$b)$ Let $f$ be an isomorphism from $H'$ to H. The sequence $(f^n(H))_{n\geq 0}$ is a decreasing sequence of compact subgroups of G, so $f^n(H) =f^{n+1}(H)$ for $n$ sufficiently large, by $a)$. Since $f$ is an isomorphism, this implies that $f(H) = H =f(H')$, so $H = H'$.

$c)$ Let $t, t'\in \mathscr{T}$ be such that $t\leq t'$ and $t'\leq t$. Then, there exist $H,H_1\in t$ and $H',H'_1\in t'$ such that $H\supset H'$ and $H_1\subset H'_1$. Let $g$ and $g'$ be two elements of G such that $H_1=gHg^{-1}$ and $H'_1=g'H'g^{'-1}$; put $u=g^{'-1}g$. Then

$$
uHu^{-1}\subset H'\subset H
$$

by $b)$, this implies that $uHu^{-1}= H$, so $H'= H$ and $t'=t$. Thus, the set $\mathscr{T}$ is ordered, and it is noetherian by $a)$.

#### Theorem 2 {#lie-ix-s9-thm-2 .statement tag=01HU}

Let G be a Lie group operating properly on X, such that the law of operation $(g, x) \rightarrow gx$ is of class $C^r$. Assume that X is paracompact.

a) The map which associates to any point of X its orbit type has the following semi-continuity property: let $x\in X$ and let $t\in \mathscr{T}$ be its orbit type; there exists a stable open neighbourhood U of $x$ such that, for any $u\in U$, the type of $u$ is $\geq t$.

b) For all $t\in \mathscr{T},X_{(t)}$ is a submanifold of X, the equivalence relation on $X_{(t)}$ induced by the operation of G is regular (Differentiable and Analytic Manifolds, Results, 5.9.5), and the morphism $X_{(t)}\rightarrow X_{(t)}/G$ is a bundle.

c) Assume that $X/G$ is connected. Then the set of orbit types of elements of X has a largest element $\tau$; moreover, $X_{(\tau)}$ is a dense open subset of X and $X_{(\tau)}/G$ is connected.

Let $x$ be a point of X and $t\in \mathscr{T}$ its type. To prove $a)$ and $b)$, we can replace X by a stable open set containing $x$, and hence (Prop. 6) can assume that X is of the form $G\times^HW$, where W is the space of a finite dimensional analytic linear representation of a compact subgroup H of G, the point $x$ being the image $p(e,0)$ of $(e,0)\in G\times W$ under the canonical projection $p: G\times W\rightarrow G\times^HW$. If $u=p(g, y)\in G\times^HW$ and $a\in G$, then $au=u$ if and only if there exists $h\in H$ with $(ag, y) = (gh^{-1}, hy)$, that is, if $a\in gH_yg^{-1}$. Thus, $G_u=gH_yg^{-1}$; in particular, $G_x= H$, so $G_u$ is conjugate to a subgroup of $G_x$, which proves that the type of $u$ is $\geq t$, hence $a)$.

Moreover, $u$ is of type $t$ if and only if $G_u$ is conjugate to H in G, or equivalently that $H_y$ is conjugate to H in G; by Lemma $6b)$, this means that $H_y= H$, and hence that $y$ is fixed by H. If $W'$ is the vector subspace of W consisting of the elements fixed by H, it follows that $X_{(t)}$ can be identified with $G\times^HW'$, and hence also with $G/H\times W'$, hence $b)$.

To prove $c)$, observe that the assumption that $X/G$ is connected implies that X is pure of finite dimension: indeed, for all $k\geq 0$, denote by $X_k$ the set of points $x\in X$ such that dim$_xX =k$; then $X_k$ is open and closed in X, and stable under G, so X is equal to one of the $X_k$.

We now prove $c)$ by induction on the dimension of X, the assertion being clear for dim X = 0. Let $\tau$ be a maximal element among the orbit types of the points of X (such an element exists by Lemma $6c))$. We shall prove the following:

$c')$ For every subset A of $X_{(t)}$, open and closed in $X_{(\tau)}$ and stable under G, the closure $\overline{A}$ of A in X is open.

This assertion implies $c)$. Indeed, note first that $X_{(\tau)}$ is open in X, by $a)$; assertion $c')$ implies that $\overline{X}_{(\tau)}$ is open and closed in X, hence equal to X since it is stable under G and $X/G$ is connected. Let A be a non-empty open and closed subset of $X_{(\tau)}$ stable under G; by $c'),\overline{A}$ is open and closed in X and stable under G, hence equal to X; this implies that A is dense in $X_{(\tau)}$, hence equal to $X_{(\tau)}$. Consequently, every non-empty open and closed subset of $X_{(\tau)}/G$ is equal to $X_{(\tau)}/G$, which proves that $X_{(\tau)}/G$ is connected. Finally, since $X_{(\tau)}$ is dense in X, it follows from $a)$ that every point of X is of type $\leq \tau$; in other words, $\tau$ is the largest element among the orbit types of the points of X.

We now prove $c')$. We can assume that A is non-empty; let $x\in A$. It suffices to prove that A is a neighbourhood of $x$. For this we can, as above, assume that $X = G\times^HW$ with H compact, $x$ being the canonical image of $(e,0)$. Assume first that H operates trivially on W: then X can be identified with $(G/H)\times W$, and $X_{(\tau)}/G = X/G$ is homeomorphic to W, hence connected; thus, $A/G = X/G$, so A = X. Assume from now on that H does not operate trivially on W. Choose a scalar product on W invariant under the compact group H; let S be the unit sphere in W (the set of vectors of norm 1). Note that $S/H$ is connected: indeed, if dim(W) $\geq 2, S$ is connected, and if dim(W) = 1, S is a space of two points on which H operates non-trivially. Put $Y = G\times^HS$; this is a closed submanifold of X, stable under G, of codimension 1, and $Y/G$, which is homeomorphic to $S/H$, is connected. Thus, by the induction hypothesis, there exists a maximal orbit type $\theta$ for Y, the set $Y_{(\theta)}$ is open and dense in Y, and $Y_{(\theta)}/G$ is connected.

Consider the operation of $\mathbf{R}^*_+$ on X induced by passage to the quotient by the law of operation $(\lambda ,(g, w)) \rightarrow (g, \lambda w)$ of $\mathbf{R}^*_+$ on $G\times W$. Two points of X conjugate under this operation are of the same orbit type; consequently, $X_{(\theta)}$ contains $\mathbf{R}^*_+Y_{(\theta)}$, which is a dense open subset of X. But $X_{(\tau)}$ is open by $a)$, and hence meets $X_{(\theta)}$, so $\theta =\tau$.

On the other hand, the homeomorphism $(\lambda , w) \rightarrow \lambda w$ from $\mathbf{R}^*_+\times S$ to W **--** $\{0\}($General Topology, Chap. VI, §2, no. 3, Prop. 3) induces a homeomorphism from $\mathbf{R}^*_+\times (S/H)$ to $(\mathbf{R}^*_+S)/H$, hence also from $\mathbf{R}^*_+\times (Y/G)$ to $(\mathbf{R}^*_+Y)/G$, and from $\mathbf{R}^*_+\times (Y_{(\theta)}/G)$ to $(\mathbf{R}^*_+Y_{(\theta)})/G$. Thus, $(\mathbf{R}^*_+Y_{(\theta)})/G$ is connected, and $X_{(\tau)}/G$, which contains a connected dense subset, is itself connected (General Topology, Chap. I, §11, no. 1, Prop. 1). Consequently, A is equal to $X_{(\tau)}$, hence is dense in X, and A is a neighbourhood of $x$. This completes the proof of the theorem.

With the notations in Th. $2c)$, the points of $X_{(\tau)}$ are said to be principal and their orbits are called principal orbits. If $x$ is a point of X, and if $G\times^{G_x}W$ is a linear tube in X around the orbit of $x$, the point $x$ is principal if and only if $G_x$ operates trivially on W, that is, if the tube is of the form $(G/G_x)\times W$.

#### Example 1 {#lie-ix-s9-n4-exa-1 .statement tag=01HV}

Let G be a connected compact Lie group, operating on itself by inner automorphisms. The fixer of an element $x$ of G is simply the centralizer $Z(x)$ of $x$ in G; it contains every maximal torus containing $x$. It follows that the largest orbit type $\tau$ is the conjugacy class of the maximal tori of G. The open set $G_{(\tau)}$ is the set of very regular elements of G (§5, no. 1, Remark). Assume that G is simply-connected. Then $G_{(\tau)}$ is equal to the set $G_r$ of regular elements of G (§5, no. 2, Remark 2); if A is an alcove of a Cartan subalgebra $\mathfrak{t}$ of $\mathfrak{g}= L(G)$, the composite map $\pi : A\longrightarrow^{exp}G_r\longrightarrow G_r/$Int(G) is an isomorphism of analytic manifolds. Indeed, this is a homeomorphism (§5, no. 2, Cor. of Prop. 2); let $a\in A$, put $t=$ exp $a$ and identify $T_t(G)$ with $\mathfrak{g}$ by means of the translation $\gamma (t)$. The tangent map $T_a(\pi )$ can then be identified with the composite of the canonical injection $\mathfrak{t}\rightarrow \mathfrak{g}$ and the quotient map $\mathfrak{g}\rightarrow \mathfrak{g}/$Im(Ad $t^{-1}-1)$. Since $t$ is regular, $T_a(\pi )$ is an isomorphism, hence the stated result (Differentiable and Analytic Manifolds, Results, 5.7.8).

#### Example 2 {#lie-ix-s9-n4-exa-2 .statement tag=01HW}

Let E be a real euclidean affine space, $\mathfrak{H}$ a set of hyperplanes of E, W the group of displacements of E generated by the orthogonal reflections with respect to the hyperplanes of $\mathfrak{H}$. Assume that $\mathfrak{H}$ is stable under W and that the group W, with the discrete topology, operates properly on E.

The preceding can be applied to the operation of W on E. The fixer of a point $x$ of E is the subgroup of W generated by the reflections with respect to the hyperplanes of $\mathfrak{H}$ containing $x$ (Chap. V, §3, no. 3, Prop. 2). Consequently, the largest orbit type $\tau$ is the class of the subgroup $\{$Id$_E\}$, and $E_{(\tau)}$ is the union of the chambers of E. Note that in this case the covering $E_{(\tau)}\rightarrow E_{(\tau)}/W$ is trivial, and in particular $E_{(\tau)}$ is not connected if $\mathfrak{H}$ is non-empty.

### Exercises {#lie-ix-s9-exercises}

See the [exercises for § 9](exercises/s9/).
