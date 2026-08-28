---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 4
section_title: Passage from Lie algebras to Lie groups
lang: en
source: lie-i-iii
pdf_pages: 0297-0315, 0394-0400
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 0
      pdf_page: 297
    - "no": 2
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 0
      pdf_page: 299
    - "no": 3
      title: EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 302
    - "no": 4
      title: FUNCTORIZATION OF EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 306
    - "no": 5
      title: STRUCTURE INDUCED ON A SUBGROUP
      page: 0
      pdf_page: 307
    - "no": 6
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 0
      pdf_page: 309
    - "no": 7
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 0
      pdf_page: 312
statements: 40
exercises: 8
content_sha256: dc59481a501f40d45c0742b137c5851b6eca2830d1e1723f2728e33fa3a87a07
---

## § 4. PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS

Recall that, until the end of the chapter, K is assumed to be of characteristic 0.

### 1. PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS

#### Lemma 1 {#lie-iii-s4-lem-1 .statement}

*Let G be a Lie group germ and $\mathfrak{h}$ a Lie subalgebra of $L(G)$ admitting a topological supplement. The union of the $g\mathfrak{h}$ (resp. $\mathfrak{h}g$) for $g \in G$ is an integrable vector subbundle of $T(G)$.*

By considering the left trivialization of $T(G)$ (§ 2, no. 3), it is seen immediately that the $g\mathfrak{h}$, for $g \in G$, are the fibres of a vector subbundle E of $T(G)$. Let $g \in G$. The set of $(L_a)_g$, where $a \in \mathfrak{h}$, is equal to $g\mathfrak{h}$. Now, if $a$ and $b$ belong to $\mathfrak{h}$, then $[L_a, L_b] = L_{[a, b]}$ and $[a, b] \in \mathfrak{h}$. Hence E is integrable (*Differentiable and Analytic Manifolds*, R, 9.3.3 (iv)). The argument is similar for the $\mathfrak{h}g$.

The integral foliation (*Differentiable and Analytic Manifolds*, R, 9.3.2) of the union of the $g\mathfrak{h}$ (resp. $\mathfrak{h}g$) is called the *left* (resp. *right*) *foliation* of G associated with $\mathfrak{h}$.

#### Theorem 1 {#lie-iii-s4-thm-1 .statement}

*Let G and H be Lie group germs and f a continuous morphism of $L(G)$ into $L(H)$.
(i) There exist an open Lie subgroup germ $G'$ of G and a morphism $\phi$ of $G'$ into H such that $f = L(\phi)$.
(ii) Let $G_1, G_2$ be open Lie subgroup germs of G and $\phi_i$ a morphism of $G_i$ into H such that $f = L(\phi_i)$ for $i = 1, 2$. Then $\phi_1$ and $\phi_2$ coincide on a neighbourhood of e.
Let $p_1 : G \times H \to G, p_2 : G \times H \to H$ be the canonical projections. For all $(g, h) \in G \times H$, let $f_{g, h}$ be the mapping $ga \mapsto hf(a)$ of $T_g(G) = gL(G)$ into $T_h(H) = hL(H)$. By considering the left trivializations of $T(G)$ and $T(H)$, it is seen immediately that the $f_{g, h}$ define a morphism of $p_1^*T(G)$ into* $p_2^*T(H)$. Let $a$ be the graph of $f$; it is a closed Lie subalgebra of $L(G) \times L(H)$ which admits $\{0\} \times L(H)$ as topological supplement. For all $(g, h) \in G \times H$, the graph of $f_{g,h}$ is $(g, h) \cdot a$. The union of these graphs is an integrable vector subbundle of $T(G \times H)$ (Lemma 1). Then there exist (Differentiable and Analytic Manifolds, R, 9.3.7) an open neighbourhood $U$ of $e_G$ in $G$ and an analytic mapping $\phi$ of $U$ into $H$ such that $\phi(e_G) = e_H$ and $T_g(\phi) = f_{g, \phi(g)}$ for all $g \in U$. In particular, $T_{e_G}(\phi) = f$.

Let $V$ be an open neighbourhood of $e_G$ in $G$ such that, for $(s, t) \in V \times V$, the products $st$ and $\phi(s)\phi(t)$ are defined and $st \in U$. Consider the mappings $\alpha_1, \alpha_2$ of $V \times V$ into $H$ defined by

$$
\alpha_1(s, t) = \phi(ts), \quad \alpha_2(s, t) = \phi(t)\phi(s).
$$

Then $\alpha_1(t, e) = \phi(t) = \alpha_2(t, e)$. On the other hand, let $t$ be fixed in $V$ and $\beta_i$ be the mapping $s \mapsto \alpha_i(s, t)$ of $V$ into $H$. Then, for all $s \in V$ and all $a \in L(G)$,

$$
\begin{align*}
T_s(\beta_1)(sa) &= T_{ts}(\phi)(tsa) = f_{ts, \phi(ts)}(tsa) \\
&= \phi(ts)f(a) = f_{s, \beta_1(s)}(sa) \\
T_s(\beta_2)(sa) &= \phi(t)T_s(\phi)(sa) = \phi(t)f_{s, \phi(s)}(sa) \\
&= \phi(t)\phi(s)f(a) = f_{s, \beta_2(s)}(sa).
\end{align*}
$$

Hence (Differentiable and Analytic Manifolds, R, 9.3.7) $\alpha_1$ and $\alpha_2$ coincide on a neighbourhood of $(e_G, e_G)$. The restriction of $\phi$ to a sufficiently small symmetric open neighbourhood of $e_G$ is therefore a morphism of Lie group germs, whence (i).

Let $G_1, G_2, \phi_1, \phi_2$ be as in (ii) and let us prove that $\phi_1, \phi_2$ coincide on a neighbourhood of $e_G$. There exists an open neighbourhood $W$ of $e_G$ such that $\phi_1(ts) = \phi_1(t)\phi_1(s)$, $\phi_2(ts) = \phi_2(t)\phi_2(s)$ for all $s, t$ in $W$. Then, if $s \in W$ and $a \in L(G)$,

$$
T_s(\phi_i)(sa) = \phi_i(s)T_e(\phi_i)(a) = \phi_i(s)f(a) = f_{s, \phi_i(s)}(sa)
$$

for $i = 1, 2$. As $\phi_1(e_G) = e_H = \phi_2(e_G)$, it follows from Differentiable and Analytic Manifolds, R, 9.3.7 that $\phi_1$ and $\phi_2$ coincide on a neighbourhood of $e_G$.

#### Corollary 1 {#lie-iii-s4-thm-1-cor-1 .statement}

Let $G$ and $H$ be two Lie group germs. If $L(G)$ and $L(H)$ are isomorphic, $G$ and $H$ are locally isomorphic.

This follows from Theorem 1 and § 1, no. 10, Proposition 21.

#### Corollary 2 {#lie-iii-s4-thm-1-cor-2 .statement}

Let $G$ be a Lie group germ. If $L(G)$ is commutative, $G$ is locally isomorphic to the additive Lie group $L(G)$.

The Lie algebra of the additive group $L(G)$ is isomorphic to $L(G)$. Hence it suffices to apply Corollary 1.

#### Corollary 3 {#lie-iii-s4-thm-1-cor-3 .statement}

Let $G$ be a Lie group. If $L(G)$ is commutative, $G$ contains a commutative open subgroup.

There exists an open Lie subgroup germ U of G which is commutative (Corollary 2). Let V be a neighbourhood of e such that V^2 ⊂ U. Then xy = yx for all x, y in V. Hence the subgroup of G generated by V is commutative; it is obviously open.

### 2. PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS

We shall denote the Hausdorff series by H(X, Y) (Chapter II, § 6, no. 4, Definition 1).

#### Lemma 2 {#lie-iii-s4-lem-2 .statement}

Let L be a complete normed Lie algebra over $\mathbf{R}$ or $\mathbf{C}$. Let G be the set of $x \in L$ such that $\|x\| < \frac{1}{3} \log \frac{3}{2}$. Let $\theta$ be the mapping $x \mapsto -x$ of G into G. Let H be the restriction to $G \times G$ of the Hausdorff function of L (Chapter II, § 7, no. 2).
(i) $(G, 0, \theta, H)$ is a Lie group germ.
(ii) Let $\phi$ be the identity mapping of G into L. The differential of $\phi$ at 0 is an isomorphism of the normable Lie algebra $L(G)$ onto L.
(i) follows from Chapter II, § 7, no. 2.
As $\phi$ is a chart on G, the differential $\psi$ of $\phi$ at 0 is an isomorphism of normable spaces. On the other hand, the expansion as an integral series $H = \sum_{i,j \geq 0} H_{ij}$ of the mapping H is such that $H_{11}(x, y) = \frac{1}{2}[x, y]$. By § 3, Proposition 24, for all $a, b$ in $L(G)$,
$$
\psi([a, b]) = H_{11}(\psi(a), \psi(b)) - H_{11}(\psi(b), \psi(a)) = [\psi(a), \psi(b)]
$$
which proves (ii).

G is called the *Lie group germ defined by L*.

Suppose that K is ultrametric. Let $p$ be the characteristic of the residue field of K. If $p \neq 0$, let $\lambda = |p|^{1/(p-1)}$; if $p = 0$, let $\lambda = 1$.

#### Lemma 3 {#lie-iii-s4-lem-3 .statement}

Let L be a complete normed Lie algebra over K. Let G be the set of $x \in L$ such that $\|x\| < \lambda$. Let $H : G \times G \to G$ be the Hausdorff function of L (Chapter II, § 8, no. 3).
(i) With the law of composition H, G is a Lie group in which 0 is identity element and $-x$ the inverse of x for all $x \in G$.
(ii) Let $\phi$ be the identity mapping of G into L. The differential of $\phi$ at 0 is an isomorphism of the normable Lie algebra $L(G)$ onto L.
(iii) For all $\mu \in \mathbf{R}_+^*$, let $G_\mu$ be the set of $x \in L$ such that $\|x\| < \mu$. Then the $G_\mu$, for $\mu < \lambda$, form a fundamental system of open and closed neighbourhoods of 0 and are subgroups of G.
Assertions (i) and (iii) follow from Chapter II, § 8, no. 3, Proposition 3 and (ii) can be proved as in Lemma 2.

G is called the *Lie group defined by L*.

#### Theorem 2 {#lie-iii-s4-thm-2 .statement}

Let L be a complete normable Lie algebra. There exists a Lie group germ G such that L(G) is isomorphic to L. Two such Lie group germs are locally isomorphic.

The first assertion follows from Lemmas 2 and 3. The second assertion follows from Corollary 1 to Theorem 1 of no. 1.

#### Corollary 1 {#lie-iii-s4-thm-2-cor-1 .statement}

Let G be a Lie group. There exists a neighbourhood of e which contains no finite subgroup distinct from {e}. If K = R or C, there exists an open neighbourhood of e which contains no subgroup distinct from {e}.

We write L(G) = L. Choose a norm on L defining the topology on L and such that $\| [x, y] \| \leq \| x \| \| y \|$ for all x, y in L.

Suppose that K = R or C. Let G' be the Lie group germ defined by L. There exist an open ball U' of centre 0 in G' and an isomorphism $\phi$ of the Lie group germ U' onto an open neighbourhood U of e in G. Let V' = $\frac{1}{2} U'$, $V = \phi(V')$, H be a subgroup of G contained in V and $h \in H$. Let $x = \phi^{-1}(h) \in V'$. If $x \neq 0$, there exists an integer $n > 0$ such that $x, 2x, \ldots, nx$ are in V', $(n+1)x \in U'$, $(n+1)x \notin V'$. Then $h, h^2, \ldots, h^n$ are in V,

$$
h^{n+1} \in U, \qquad h^{n+1} \notin V,
$$

which is absurd. Hence H = {e}.

Suppose that K is ultrametric. It suffices to prove the corollary when G is the Lie group associated with L. If $g \in G$, the powers of g evaluated in G are the elements of $\mathbf{Z}g$ evaluated in L. These are distinct if $g \neq e$. Hence G contains no finite subgroup distinct from {e}.

#### Corollary 2 {#lie-iii-s4-thm-2-cor-2 .statement}

Let k be a non-discrete closed subfield of K, G a Lie group over k and L = L(G). Suppose that L has a normable Lie K-algebra structure L', compatible with the normable Lie k-algebra structure and invariant under the adjoint representation of G. Then there exists on G one and only one Lie K-group structure compatible with the Lie k-group structure and for which the Lie algebra is L'.

There exists a Lie group germ $G_1$ over K such that $L(G_1) = L'$ (Theorem 2). By Corollary 1 to Theorem 1 of no. 1, G and $G_1$, considered as Lie k-group germs, are locally isomorphic. Hence there exist an open neighbourhood G' of e in G and a Lie K-group germ structure on G', with Lie algebra L, which is compatible with the Lie group germ structure over k. Let V be a symmetric open neighbourhood of e in G such that $V^2 \subset G'$. Let $g \in G$. Then $\phi = \operatorname{Int} g$ is a k-isomorphism of a sufficiently small open Lie subgroup germ of G' onto an open Lie subgroup germ of G'; and $T_e(\phi)$ is K-linear and hence $T_x(\phi)$ is K-linear for x sufficiently close to e; therefore the restriction of Int g to a sufficiently small open neighbourhood of e in V is K-analytic (Differentiable and Analytic Manifolds, R, 5.14.6). By § 1, no. 9, Proposition 18, there exists on G an analytic K-manifold structure with which G is a Lie

K-group and V is an open sub-K-manifold of G. By translation, it is seen that the underlying k-manifold structure of G is the given structure. The Lie algebra of the Lie K-group G is the same as that of the open Lie K-subgroup germ V and hence is L'. Finally, the uniqueness stated in the corollary follows from § 3, no. 8, Proposition 32.

#### Theorem 3 {#lie-iii-s4-thm-3 .statement}

Let G be a Lie group germ and $\mathfrak{h}$ a Lie subalgebra of $L(G)$ admitting a topological supplement. There exists a Lie subgroup germ H of G such that $L(H) = \mathfrak{h}$. If $H_1$ and $H_2$ are Lie subgroup germs of G such that

$$
L(H_1) = L(H_2) = \mathfrak{h},
$$

then $H_1 \cap H_2$ is open in $H_1$ and $H_2$.

There exists a Lie group germ $H'$ with Lie algebra isomorphic to $\mathfrak{h}$ (Theorem 2). Shrinking $H'$ if necessary, it can be assumed that there exists a morphism $\phi$ of $H'$ into G such that $L(\phi)$ is an isomorphism of $L(H')$ onto $\mathfrak{h}$ (no. 1, Theorem 1). As $\mathfrak{h}$ admits a topological supplement, $\phi$ is an immersion at e. Hence, shrinking $H'$ further, it can be assumed that $\phi$ is an isomorphism of the manifold $H'$ onto a submanifold of G. This proves the existence of H. The second assertion follows from the following proposition:

#### Proposition 1 {#lie-iii-s4-prop-1 .statement}

Let G be a Lie group germ and H and $H'$ two Lie subgroup germs. In order that $L(H) \supset L(H')$, it is necessary and sufficient that $H \cap H'$ be open in $H'$.

If $H \cap H'$ is open in $H'$, then $L(H') = L(H \cap H') \subset L(H)$. Suppose that $L(H) \supset L(H')$. Let i, $i'$ be the canonical injections of H, $H'$ into G. By shrinking $H'$ if necessary, it can be assumed that there exists a morphism $\psi$ of $H'$ into H such that $L(\psi)$ is the canonical injection of $L(H')$ into $L(H)$ (no. 1, Theorem 1). Then $L(i \circ \psi) = L(i')$ and hence there exists a neighbourhood V of $e_{H'}$ in $H'$ such that $i \circ \psi$ and $i'$ coincide on V (Theorem 1). Therefore $V \subset H$, hence $V \subset H \cap H'$ and $H \cap H'$ is open in $H'$ (§ 1, no. 10).

#### Proposition 2 {#lie-iii-s4-prop-2 .statement}

Let G be a Lie group over K, k a non-discrete closed subfield of K and H a Lie subgroup of the Lie k-group G. Suppose that $L(H)$ is a vector sub-K-space of $L(G)$ which admits a topological supplement. Then H is a Lie subgroup of the Lie K-group G.

There exists a Lie subgroup germ $H'$ of the Lie K-group G such that $L(H') = L(H)$ (Theorem 3). Consider G, H, $H'$ as Lie k-group germs; Theorem 3 then proves that $H \cap H'$ is open in H and $H'$. Hence there exists an open neighbourhood U of e in G such that $U \cap H$ is a submanifold of G over K. Therefore, H is a Lie subgroup of the Lie K-group G (§ 1, no. 3, Proposition 6).

### 3. EXPONENTIAL MAPPINGS

#### Theorem 4 {#lie-iii-s4-thm-4 .statement}

Let G be a Lie group germ, L its Lie algebra, V an open neighbourhood of 0 in L, φ an analytic mapping of V into G such that φ(0) = 0 and T_0(φ) = Id_L. The following conditions are equivalent:
(i) For all b ∈ L, φ((λ + λ')b) = φ(λb)φ(λ'b) for |λ| and |λ'| sufficiently small.
(ii) For all b ∈ L and every integer n > 0, φ_*(b^n) is homogeneous of degree n in U(G) (T_0^{(∞)}(L) is identified with TS(L) and b^n is evaluated in TS(L)).
(iii) The mapping φ_* of TS(L) into U(G) is compatible with the graduations of TS(L) and U(G).
(iv) The mapping φ_* of TS(L) into U(G) is the canonical mapping of TS(L) into the enveloping algebra of L.
(v) There exist a norm on L defining the topology of L and such that
$$
\|[x, y]\| \leq \|x\|\|y\|
$$
for all x, y in L and an open subgroup germ W ⊂ V of the Lie group germ defined by L (no. 2) such that φ|W is an isomorphism of W onto an open Lie subgroup germ of G.

(v) ⇒ (i): obvious, for (λb).(λ'b) = (λ + λ')b in W for |λ| and |λ'| sufficiently small.
(i) ⇒ (ii): suppose that condition (i) is satisfied. Let b ∈ L. Let ψ be the restriction of φ to V ∩ Kb. By hypothesis, there exists a symmetric neighbourhood T of 0 in the additive Lie group Kb such that ψ|T is a morphism of the Lie group germ T into G. Hence
$$
φ_*(b^n) = (ψ|T)_*(b^n) = ((ψ|T)_*(b))^n = (φ_*(b))^n,
$$
so that φ_*(b^n) is homogeneous of degree n in U(G).
(ii) ⇒ (iii): this follows from the fact that TS^n(L) is the vector subspace of TS(L) generated by the n-th powers of the elements of L (Algebra, Chapter IV, § 5, Proposition 5).
(iii) ⇒ (iv): the canonical mapping of TS(L) into the enveloping algebra of L is the unique morphism of graded cogebras mapping 1 to 1 and extending Id_L (Chapter II, § 1, no. 5, Remark 3). Now φ_* is a cogebra morphism and φ_*|L = Id_L by hypothesis. If condition (iii) holds, it is seen that condition (iv) also holds.
(iv) ⇒ (v): suppose that condition (iv) is satisfied. Choose a norm on L defining the topology of L and such that \|[x, y]\| \leq \|x\|\|y\| for all x, y in L. Let H be the Lie group germ defined by the normed Lie algebra L. By Theorem 1, there exist an open subgroup germ S ⊂ V of H and an isomorphism φ' of S onto an open subgroup germ of G. As we know already that (v) ⇒ (iv), the mapping φ_* of TS(L) into U(G) is the canonical mapping of TS(L) into the enveloping algebra of L. Thus φ_*(t) = φ'_*(t) for all t ∈ T_0^{(∞)}(L). As φ and φ' are analytic, φ and φ' coincide on a neighbourhood of 0.

#### Definition 1 {#lie-iii-s4-def-1 .statement}

Let G be a Lie group germ and L its Lie algebra. An exponential mapping of G is any analytic mapping $\phi$ defined on an open neighbourhood of 0 in L, with values in G and satisfying the conditions of Theorem 4.

Theorem 4 implies immediately that, for every Lie group germ G, there exists an exponential mapping of G and that two exponential mappings of G coincide on a neighbourhood of 0.

#### Example {#lie-iii-s4-n3-exa-1 .statement}

(1) Let G be the additive group of a complete normable space E. The canonical isomorphism of L(G) onto E satisfies condition (i) of Theorem 4 and is therefore an exponential mapping of G.

(2) Let A be a complete normed unital associative algebra. Let A* be the Lie group consisting of the invertible elements of A. We identify L(A*) with A (§ 3, no. 9, Corollary to Proposition 33). If K = \mathbf{R} or \mathbf{C}, we know that the mapping exp of A into A* defined in Chapter II, § 7, no. 3 satisfies condition (i) of Theorem 4 and hence is an exponential mapping. Now let K be ultrametric. Let $p$ be the characteristic of the residue field of K. If $p \neq 0$, let $\lambda = |p|^{1/(p-1)}$; if $p = 0$, let $\lambda = 1$. Let U be the set of $x \in A$ such that $\|x\| < \lambda$. We know (Chapter II, § 8, no. 4) that the mapping exp of U into A* satisfies condition (i) of Theorem 4 and hence is an exponential mapping. Note that U is an additive subgroup of A.

This example explains the terminology adopted in Definition 1.

Let G be a Lie group germ and $\phi$ an exponential mapping of G. Then $\phi$ is étale at 0 and hence there exists an open neighbourhood U of 0 in L(G) such that $\phi(U)$ is open in G and $\phi|U$ is an isomorphism of the analytic manifold U onto the analytic manifold $\phi(U)$.

A canonical chart (of the first species) on G is a chart $\psi$ on the analytic manifold G whose inverse mapping is an exponential mapping. If further G is finite-dimensional and a basis of L(G) is chosen, the coordinate system defined by $\psi$ and this basis in the domain of $\psi$ is called a canonical coordinate system (of the first species).

#### Proposition 3 {#lie-iii-s4-prop-3 .statement}

Let G be a Lie group germ, L its Lie algebra and $\phi$ an exponential mapping of G. Let $L_1, \ldots, L_n$ be vector subspaces of L such that L is the topological direct sum of $L_1, \ldots, L_n$. The mapping

$$
(b_1, b_2, \ldots, b_n) \mapsto \theta(b_1, b_2, \ldots, b_n) = \phi(b_1)\phi(b_2)\cdots\phi(b_n),
$$

defined on an open subset of $L_1 \times L_2 \times \cdots \times L_n$, is analytic. The tangent mapping at $(0, 0, \ldots, 0)$ to $\theta$ is the canonical mapping of $L_1 \times \cdots \times L_n$ into L.

Let $k_i$ be the canonical injection of $L_i$ into $L_1 \times L_2 \times \cdots \times L_n$. Then, for all $b \in L_i$, $(T_{(0, \ldots, 0)}\theta)(T_0k_i)(b) = (T_0\phi)(b) = b$ and hence $(T_{(0, \ldots, 0)}\theta)|L_i$ is the canonical injection of $L_i$ into L.

In particular, $\theta$ is étale at $(0, 0, \ldots, 0)$. Its restriction to a sufficiently small

LIE GROUPS

open neighbourhood U of $(0, 0, \ldots, 0)$ has an open image in G and is an isomorphism of the manifold U onto the manifold $\theta(U)$. The inverse mapping $\eta$ of $\theta(U)$ onto U is called a *canonical chart of the second species* of G, associated with the given decomposition of L as a direct sum. If further G is finite-dimensional and each $L_i$ is generated by a non-zero vector $e_i$, the coordinate system on $\theta(U)$ defined by $\eta$ and the $e_i$ is called a *canonical coordinate system of the second species*.

#### Proposition 4 {#lie-iii-s4-prop-4 .statement}

*Let G be a Lie group germ and $\phi$ an injective exponential mapping of G. For all x, y in $L(G)$,*

(1)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))
$$
(2)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2} \phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))
$$
(note that $\phi^{-1}(\phi(\lambda x) \phi(\lambda y))$ and $\phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))$ are defined for $|\lambda|$ sufficiently small).

Let $L = L(G)$ be given a norm defining the topology of L and such that $\| [x, y] \| \leq \| x \| \| y \|$ for all $x, y$ in L. Using Theorems 2 and 4, it can be assumed that G is the Lie group germ defined by L and that $\phi = \mathrm{Id}_G$. Let $(x, y) \mapsto x \cdot y$ denote the product in the group G. The formulae to be proved can then be written
(3)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1}((\lambda x) \cdot (\lambda y))
$$
(4)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2}((\lambda x) \cdot (\lambda y) \cdot (-\lambda x) \cdot (-\lambda y)).
$$

There exists an open neighbourhood V of 0 in K such that the function
$$
\lambda \mapsto f(\lambda) = (\lambda x) \cdot (\lambda y)
$$
is defined and analytic on V. By Chapter II, § 6, no. 4, *Remark 2*, the expansion of $f$ as an integral series about the origin is
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] + \cdots
$$
and this proves (3). On the other hand, for $u, v$ in G and $\|u\|, \|v\|$ sufficiently small, $u \cdot v$ is an analytic function of $(u, v)$ and the terms of degrees 1 and 2 in the expansion of this function as an integral series about the origin are $u + v + \frac{1}{2}[u, v]$. By *Differentiable and Analytic Manifolds*, R, 3.2.7 and 4.2.3, the terms of degrees 1 and 2 in the expansion of the function $f(\lambda) \cdot f(-\lambda)$ as an integral series about the origin are the terms of degrees 1 and 2 in
$$
f(\lambda) + f(-\lambda) + \frac{1}{2}[f(\lambda), f(-\lambda)]
$$
or also in
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] - \lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] \\
+ \frac{1}{2} [\lambda(x + y), -\lambda(x + y)] = \lambda^2 [x, y]
$$
and this proves (4).

EXponential mappings

§ 4.3

#### Proposition 5 {#lie-iii-s4-prop-5 .statement}

Let G be a Lie group, k a non-discrete closed subfield of K, G' the group G considered as a Lie group over k and $\phi$ (resp. $\phi'$) an exponential mapping of G (resp. G'). Then $\phi$ and $\phi'$ coincide on a neighbourhood of 0.

$\phi$ satisfies hypothesis (i) of Theorem 4 relative to G' and is therefore an exponential mapping of G'.

#### Proposition 6 {#lie-iii-s4-prop-6 .statement}

Let G be a Lie group germ, L its Lie algebra and $\phi : V \to G$ an exponential mapping of G. For all $x \in V$, let $T_x(L)$ be identified with L, so that the right differential $\varpi(x)$ of $\phi$ at x is a linear mapping of L into L. For x sufficiently close to 0,

$$
\varpi(x) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\operatorname{ad} x)^n.
$$

Let L be given a norm compatible with its topology and such that $\| [x, y] \| \leq \| x \| \| y \|$ for all $x, y \in L$. It suffices to consider the case where G is the Lie group germ defined by L and $\phi = \operatorname{Id}_G$. By definition, $\varpi(x)$ is then the tangent mapping at x to the mapping $y \mapsto y . x^{-1}$ of G into G. If $H(X, Y)$ denotes the Hausdorff series, $\varpi(x)$ is therefore, for $\| x \|$ sufficiently small, the tangent mapping at 0 to the mapping $y \mapsto H(x, +y, -x)$ of G into G. In $H(X + Y, -X)$, the sum of terms of the first degree in Y is

$$
\sum_{m \geq 0} \frac{1}{(m+1)!} (\operatorname{ad} X)^m Y
$$

(Chapter II, § 6, no. 5, Proposition 5). The proposition then follows from Differentiable and Analytic Manifolds, R, 3.2.4 and 4.2.3.

Let G be a Lie group germ and $t \in K$. A *t-th power mapping of G* is any mapping, defined and analytic on an open neighbourhood of e, with values in G and coinciding on a neighbourhood of e with a mapping

$$
g \mapsto \phi(t \phi^{-1}(g))
$$

where $\phi$ is an injective exponential mapping of G.

#### Proposition 7 {#lie-iii-s4-prop-7 .statement}

(i) *If $t \in \mathbf{Z}$, a t-th power mapping coincides on a neighbourhood of e with the mapping $g \mapsto g^t$.*

(ii) *The tangent mapping at e to a t-th power mapping is the homothety of ratio t.*

(iii) *If h is a t-th power mapping and h' a t'-th power mapping of G, $h \circ h'$ is a (tt')-th power mapping and $g \mapsto h(g)h'(g)$ is a (t + t')-th power mapping.*

(iv) *If h is a t-th power mapping and $u \in U^n(G)$, then $h_*(u) = t^n u$.*

It suffices to prove the proposition when G is the Lie group germ defined by a complete normed Lie algebra and when the t-th power mappings considered are constructed using the exponential mapping $\phi = \operatorname{Id}_G$. But in that case everything is obvious.

### 4. FUNCTORIZATION OF EXPONENTIAL MAPPINGS

#### Proposition 8 {#lie-iii-s4-prop-8 .statement}

Let G and H be Lie group germs, h a morphism of G into H and $\phi_G$ and $\phi_H$ exponential mappings of G and H. There exists a neighbourhood V of 0 in $L(G)$ such that $h \circ \phi_G$ and $\phi_H \circ L(h)$ coincide on V.

Let $L(G)$ and $L(H)$ be given norms defining their topologies and such that $\| [x, y] \| \leq \| x \| \| y \|$ for all x and y. It can be assumed that G (resp. H) is the Lie group germ defined by $L(G)$ (resp. $L(H)$), so that $\phi_G$ (resp. $\phi_H$) coincides with $\mathrm{Id}_G$ (resp. $\mathrm{Id}_H$) in a neighbourhood of 0. On the other hand, there exists a symmetric open neighbourhood W of 0 in $L(G)$ such that $L(h)$ is a morphism of the Lie group germ W into H. By Theorem 1, $L(h)$ coincides with h on a neighbourhood of 0, whence the proposition.

Loosely speaking, if G and H are identified in a neighbourhood of the identity element with $L(G)$ and $L(H)$ by means of exponential mappings, every morphism of G into H is *linear* in a neighbourhood of 0.

#### Corollary 1 {#lie-iii-s4-prop-8-cor-1 .statement}

Let G be a Lie group germ, G' a Lie subgroup germ of G and $\phi$ an exponential mapping of G.

(i) There exists an open neighbourhood V of 0 in $L(G')$ such that $\phi|V$ is an isomorphism of the manifold V onto an open neighbourhood of e in G'.

(ii) Let $x \in L(G)$. The following conditions are equivalent: (a) $x \in L(G')$; (b) $\phi(\lambda x) \in G'$ for $|\lambda|$ sufficiently small.

(i) is obtained by applying Proposition 8 to the canonical injection of G' into G and (ii) follows from (i).

#### Corollary 2 {#lie-iii-s4-prop-8-cor-2 .statement}

Let G be a Lie group, $\rho$ an analytic linear representation of G and $\phi$ an exponential mapping of G. There exists a neighbourhood V of 0 in $L(G)$ such that
$$
\rho(\phi(x)) = \exp(L(\rho)x)
$$
for all $x \in V$.

This follows from Proposition 8 and Example 2 of no. 3.

#### Corollary 3 {#lie-iii-s4-prop-8-cor-3 .statement}

Let G be a Lie group and $\phi$ an exponential mapping of G.

(i) There exists a neighbourhood V of 0 in $L(G)$ such that
$$
\mathrm{Ad}(\phi(x)) = \exp \mathrm{ad}\ x.
$$
for all $x \in V$.

(ii) If $g \in G$, there exists a neighbourhood W of 0 in $L(G)$ such that
$$
g \phi(x) g^{-1} = (\mathrm{Ad}\ g.x)
$$
for all $x \in W$.

(i) follows from Corollary 2 and § 3, no. 12, Proposition 44.
(ii) follows from Proposition 8 applied to Int g.

### 5. STRUCTURE INDUCED ON A SUBGROUP

#### Lemma 4 {#lie-iii-s4-lem-4 .statement}

Let G be a finite-dimensional Lie group, $\Omega$ a symmetric open neighbourhood of e in G and H a subset of $\Omega$ containing e such that the conditions $x \in H, y \in H, xy^{-1} \in \Omega$ imply $xy^{-1} \in H$. Let $r \in N_K$. For all $x \in H$, let $h_x$ be the set of $a \in T_x(G)$ with the following property: there exist an open neighbourhood I of 0 in K and a mapping f of class $C^r$ of I into G such that $f(0) = x, f(I) \subset H, (T_0f)(1) = a$.

(i) Let $h_e = h$. Then h is a Lie subalgebra of $L(G)$ which is invariant under $\mathrm{Ad}_{L(G)}(H)$.

(ii) $h_x = xh = hx$ for all $x \in H$ (where $xh$ and $hx$ are evaluated in $T(G)$).

(iii) Let V be a manifold of class $C^r$, $v_0$ a point of V and f a mapping of class $C^r$ of V into G such that $f(v_0) = e$ and $f(V) \subset H$. For every Lie subgroup germ $H'$ of G with Lie algebra h, $f(v) \in H'$ for v sufficiently close to $v_0$.

(iv) For every Lie subgroup germ $H'$ of G with Lie algebra h, $H' \cap H$ is a neighbourhood of e in $H'$.

(v) For all $x \in H$ and all $a \in h_x$, there exist an open neighbourhood I of 0 in K and a mapping f of class $C^a$ of I into G such that $f(0) = x, f(I) \subset H, (T_0f)(1) = a$. Clearly $Kh = h$ and $xh_yz = h_{xyz}$ for $x, y, xy, xyz$ in H. This implies (ii) and the fact that h is invariant under $\mathrm{Ad}_{L(G)}(H)$.

Let $a_1, a_2$ be in h. Let I be an open neighbourhood of 0 in K and $f_1, f_2$ mappings of class $C^r$ of I into G such that $f_j(0) = e, f_j(I) \subset H, (T_0f_j)(1) = a_j$ ($j = 1, 2$). We define $f : I \to G$ by $f(\lambda) = f_1(\lambda)f_2(\lambda)$. Then f is of class $C^r$ and $f(0) = e$. By shrinking I if necessary, we have $f(I) \subset H$. On the other hand, the mapping of $T_e(G) \times T_e(G)$ into $T_e(G)$ tangent to the mapping $(g, g') \to gg'$ is addition; hence $(T_0f) = a_1 + a_2$. Hence $a_1 + a_2 \in h$ and h is a vector subspace of $L(G)$. Since $xhx^{-1} = h$ for all $x \in H$, $(\mathrm{Ad}_{f_1(\lambda)}) . a_2 \in h$ for all $\lambda \in I$. The tangent mapping at 0 to the mapping $\lambda \mapsto \mathrm{Ad}f_1(\lambda)$ is, by Proposition 44 of § 3, no. 12, the mapping $\lambda \mapsto \mathrm{ad}(a_1\lambda)$; hence

$$
[a_1, a_2] = (\mathrm{ad}\, a_1) . a_2 \in h
$$

since h is closed in $L(G)$. Hence we have proved (i). In the rest of the proof we fix a Lie subgroup germ $H'$ of G with Lie algebra h.

Let V, $v_0, f$ be as in (iii). Let Y be the left foliation of G associated with h (no. 1). For all $y \in H'$, $T_y(H') = yh$. On the other hand, for all $v \in V$, the image of $T_v(V)$ under $T_v(f)$ is contained in $h_{f(v)} = f(v)h$ (by definition of $h_{f(v)}$). By *Differentiable and Analytic Manifolds*, R, 9.3.2, f is a morphism of V into Y. As $H'$ is a leaf of Y (*Differentiable and Analytic Manifolds*, R, 9.2.8), $f(v) \in H'$ for v sufficiently close to $v_0$.

Let $(a_1, \ldots, a_s)$ be a basis of h. There exist an open neighbourhood I of 0 in K and mappings $f_1, \ldots, f_s$ of class $C^r$ of I into G such that $f_j(0) = e, f_j(I) \subset H, (Tf_j)1 = a_j$ for all j. By (iii), $f_j(\lambda) \in H'$ for $|\lambda|$ sufficiently small. Hence the $f_1(\lambda_1)f_2(\lambda_2)\ldots f_s(\lambda_s)$ constitute, for $|\lambda_1|, |\lambda_2|, \ldots, |\lambda_s|$ sufficiently small, a neighbourhood of $e$ in $H'$; and this neighbourhood is contained in $H$. Hence (iv).

If $a \in \mathfrak{h}$, there exist an open neighbourhood $I$ of $0$ in $K$ and a mapping $f$ of class $C^\omega$ of $I$ into $G$ such that $f(0) = e, f(I) \subset H', (T_0 f)1 = a$. This, with (iv), implies (v).

#### Definition 2 {#lie-iii-s4-def-2 .statement}

$\mathfrak{h}$ is called the subalgebra tangent to $H$ at $e$.

#### Proposition 9 {#lie-iii-s4-prop-9 .statement}

Let $G$ be a finite-dimensional Lie group and $H$ a subgroup of $G$.

(i) There exists on $H$ one and only one analytic manifold structure with the following property: for all $r$ between 1 and $\omega$, for every manifold $V$ of class $C^r$ and for every mapping $f$ of $V$ into $H$, $f$ is of class $C^r$ as a mapping of $V$ into $H$ if and only if $f$ is of class $C^r$ as a mapping of $V$ into $G$.

(ii) With this structure, $H$ is a Lie group, the canonical injection $i$ of $H$ into $G$ is an immersion and $L(i)(L(H))$ is the Lie subalgebra tangent at $e$ to $H$.

In (i) the uniqueness is obvious. We prove the existence. Let $\mathfrak{h}$ be the Lie algebra tangent at $e$ to $H$. Let $H'$ be a Lie subgroup germ of $G$ with Lie algebra $\mathfrak{h}$. By replacing $H'$ by an open subgroup germ of $H'$, it can be assumed that $H' \subset H$ (Lemma 4 (iv)). For all $x \in H$, $xH'x^{-1}$ is a Lie subgroup germ of $G$ with Lie algebra $x\mathfrak{h}x^{-1} = \mathfrak{h}$. Hence $H' \cap (xH'x^{-1})$ is open in $H'$ (no. 2, Theorem 3) and the mapping $y \mapsto xyx^{-1}$ is an isomorphism of $H' \cap x^{-1}H'x$ onto $xH'x^{-1} \cap H'$. Using Proposition 18 of § 1, no. 9, there exist an open Lie subgroup germ $W$ of $H'$ and a Lie group structure on $H$ with the following properties: $W$ is open in $H$ and the manifold structures on $H$ and $H'$ induce the same structure on $W$. It then follows that the canonical injection $i$ of $H$ into $G$ is an immersion and that $L(i)(L(H)) = L(H') = \mathfrak{h}$. Moreover, let $V$ and $f$ be as in (i). If $f : V \to H$ is of class $C^r$, $i \circ f : V \to G$ is of class $C^r$. Suppose that $i \circ f : V \to G$ is of class $C^r$; then we prove that $f : V \to H$ is of class $C^r$. By translation, it suffices to consider the case where there exists $v_0 \in V$ such that $f(v_0) = e$ and to prove that $f : V \to H$ is of class $C^r$ in an open neighbourhood of $v_0$. Now, by Lemma 4 (iii), $f(v) \in H'$ for $v$ sufficiently close to $v_0$, whence our assertion. Thus we have proved (i) and (ii) has been obtained on the way.

#### Definition 3 {#lie-iii-s4-def-3 .statement}

The Lie group structure on $H$ defined in Proposition 9 is called the structure induced on $H$ by the Lie group structure on $G$.

If $H$ is a Lie subgroup of $G$, its Lie group structure is induced by that on $G$ (Differentiable and Analytic Manifolds, R, 5.8.5).

If $G = \mathbf{R}$ and $H = \mathbf{Q}$, then $\mathfrak{h} = \{0\}$ and hence the structure induced on $H$ is the discrete Lie group structure. Similarly if $G = \mathbf{C}$ (considered as a complex Lie group) and $H = \mathbf{R}$.

### 6. PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA

#### Lemma 5 {#lie-iii-s4-lem-5 .statement}

Let $X$ be a manifold of class $C^r$, $F$ and $F'$ vector bundles of class $C^r$ with base space $X$ and $\phi$ a morphism of $F$ into $F'$. For all $x \in X$, let $S_x$ be the set of
$$
(a, \phi(a)) \in F_x \oplus F'_x
$$
for $a \in F_x$. Then the union $S$ of the $S_x$ is a vector subbundle of $F \oplus F'$.

Let $\theta$ and $\theta'$ be the mappings of $F \oplus F'$ into itself defined as follows: if $(u, v) \in F_x \oplus F'_x$, then
$$
\theta(u, v) = (u, v + \phi(u)), \qquad \theta'(u, v) = (u, v - \phi(u)).
$$
By *Differentiable and Analytic Manifolds*, R, 7.7.1, $\theta$ and $\theta'$ are morphisms of $F \oplus F'$ into itself. Clearly $\theta \circ \theta' = \theta' \circ \theta = \mathrm{Id}_{F \oplus F'}$. Hence $\theta$ and $\theta'$ are automorphisms of $F \oplus F'$. Therefore, $S = \theta(F \oplus \{0\})$ is a vector subbundle of $F \oplus F'$.

#### Lemma 6 {#lie-iii-s4-lem-6 .statement}

Let $G$ be a Lie group germ, $\omega$ the canonical left differential form of $G$ (§ 3, no. 18.9), $M$ a manifold of class $C^r$ ($r \geq 2$) and $\alpha$ a differential form of class $C^{r-1}$ and degree 1 on $M$ with values in $L(G)$.

(i) The elements of $T(M \times G)$ at which the differential form
$$
\theta = \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega
$$
is zero constitute a vector subbundle $S$ of $T(M \times G)$ of class $C^{r-1}$.

(ii) For all $(x, g) \in M \times G$, $T(\mathrm{pr}_1)|S_{(x, g)}$ is an isomorphism of $S_{(x, g)}$ onto $T_x(M)$.

(iii) *If* $d\alpha + [\alpha]^2 = 0$ (cf. § 3, no. 14) *the vector subbundle* $S$ *is integrable*.

If $(x, g) \in M \times G$ and $(u, v) \in T_x(M) \times T_g(G)$, then
$$
\theta_{(x, g)}(u, v) = \alpha(u) - g^{-1}v.
$$
Hence the kernel of $\theta_{(x, g)}$ is the set $S_{(x, g)}$ of $(u, g\alpha(u))$ for $u \in T_x(M)$, whence (ii). We consider $T(M \times G)$ as the direct sum of two vector bundles $F$ and $F'$ with $F_{(x, g)} = T_x(M) \times \{0\}$ and $F'_{(x, g)} = \{0\} \times T_g(G)$ for all
$$
(x, g) \in M \times G.
$$
For $u \in T_x(M) \times \{0\}$, we write $\phi(u) = (0, g\alpha(u))$. Using the left trivialization of $T(G)$, it is seen that $\phi$ is a morphism of $F$ into $F'$, whence (i) (Lemma 5). Finally, if $d\alpha + [\alpha]^2 = 0$, then
$$
\begin{align*}
d\theta &= \mathrm{pr}_1^*(d\alpha) - \mathrm{pr}_2^*(d\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha \wedge \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega \wedge \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega) \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}\theta \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega)
\end{align*}
$$
and hence $S$ is integrable (*Differentiable and Analytic Manifolds*, R, 9.3.6).

#### Theorem 5 {#lie-iii-s4-thm-5 .statement}

Let G be a Lie group germ, M a manifold of class $C^r$ ($r \geq 2$) and $\alpha$ a differential form of class $C^{r-1}$ and degree 1 on M with values in $L(G)$, such that $d\alpha + [\alpha]^2 = 0$. For all $x \in M$ and all $g \in G$, there exists a mapping $f$, defined and of class $C^{r-1}$ on an open neighbourhood of $x$, with values in $G$, such that $f(x) = g$ and $f^{-1}.df = \alpha$. Two mappings which satisfy these conditions coincide on a neighbourhood of $x$.

Let $x \in M$ and $g \in G$. By Lemma 6 (whose notation we adopt) and Differentiable and Analytic Manifolds, R, 9.3.7, there exist an open neighbourhood U of $x$ in M and a mapping $m \mapsto \phi(m) = (m, f(m))$ of class $C^{r-1}$ of U into $M \times G$ such that $f(x) = g$ and $\phi^*(0) = 0$. Then

$$
f^{-1}.df = f^*(\omega) \quad (§ 3, \text{no. 18.9}) \\
= (\mathrm{pr}_2 \circ \phi)^*(\omega) \quad (\text{for } f = \mathrm{pr}_2 \circ \phi) \\
= \phi^*(\mathrm{pr}_1^*\alpha - \theta) \quad (\text{Lemma 6}) \\
= \phi^*(\mathrm{pr}_1^*\alpha) \quad (\text{for } \phi^*(\theta) = 0) \\
= \alpha \quad (\text{for } \mathrm{pr}_1 \circ \phi = \mathrm{Id}_U).
$$

Let $f'$ be a mapping of class $C^{r-1}$ of U into G such that $f'(x) = g$ and ${f'}^{-1}df' = \alpha$. By § 3, 18.9, ${f'}^{-1}$ is locally constant and hence $f' = f$ in a neighbourhood of $x$.

#### Proposition 10 {#lie-iii-s4-prop-10 .statement}

Let M be an analytic manifold, $\mathfrak{g}$ a complete normable Lie algebra and $\alpha$ an analytic differential form of degree 1 on M, with values in $\mathfrak{g}$, with the following properties:
(a) for all $m \in M$, $\alpha_m$ is an isomorphism of $T_m(M)$ onto $\mathfrak{g}$;
(b) $d\alpha + [\alpha]^2 = 0$.

Then, for all $m_0 \in M$, there exist an open neighbourhood $M'$ of $m_0$ in M and a Lie group germ structure on $M'$, compatible with the manifold structure on $M'$, with identity element $m_0$ and with the following properties:
(i) $\alpha_{m_0}$ is an isomorphism of $L(M')$ onto $\mathfrak{g}$;
(ii) the differential form $m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$ is the left canonical differential form of $M'$.
If $M'_1$ and $M'_2$ are two such group germs, $M'_1$ and $M'_2$ have a common open subgroup germ.

There exists a Lie group germ G such that $L(G) = \mathfrak{g}$. Let $m_0 \in M$. By Theorem 5, there exist an open neighbourhood $M'$ of $m_0$ in M and an analytic mapping $f$ of $M'$ into G such that $f(m_0) = e$ and $f^{-1}.df = \alpha$. Then $T_{m_0}(f) = \alpha_{m_0}$ is an isomorphism of $T_{m_0}(M)$ onto $\mathfrak{g}$; hence, shrinking $M'$ and G, it can be assumed that $f$ is an isomorphism of the manifold $M'$ onto the manifold G. We transport to $M'$ the Lie group germ structure on G by means of $f^{-1}$. Then $T_{m_0}(f)$ becomes an isomorphism of $L(M')$ onto $L(G) = \mathfrak{g}$, whence (i). On the other hand, if $\omega$ denotes the left canonical differential form of $G$, then
$$
\alpha_{m_0}^{-1} \circ \alpha_m = (\mathrm{T}_{m_0} f)^{-1} \circ (f^{-1}.df)(m)
= (\mathrm{T}_m f)^{-1} \circ \omega(f(m)) \circ \mathrm{T}_m f
$$
and hence $m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$ is the left canonical differential form of $M'$.

Let $M''$ be an open neighbourhood of $m_0$, with a Lie group germ structure, with identity element $m_0$ and with the analogous properties to properties (i) and (ii). Then $\alpha_{m_0}$ is an isomorphism of $L(M')$ onto $g$ and also of $L(M'')$ onto $g$ and hence $L(M') = L(M'')$. Therefore, shrinking $M'$ and $M''$, it can be assumed that there exists an isomorphism $\phi$ of the group germ $M'$ onto the group germ $M''$ (no. 1, Corollary 1 to Theorem 1). Then $\phi^{-1}.d\phi$ is the canonical left differential of $M'$. On the other hand, let $\psi$ be the canonical injection of the manifold $M' \cap M''$ into the Lie group germ $M''$; clearly $\psi^{-1}.d\psi$ is a restriction of the canonical left differential of $M''$. Hence $(\psi^{-1}.d\psi)(m) = \alpha_{m_0}^{-1} \circ \alpha_m = (\phi^{-1}.d\phi)(m)$ for all $m \in M' \cap M''$. Therefore $\phi$ and $\psi$ coincide on a neighbourhood of $m_0$ (§ 3, 18.9). This proves the last assertion of the proposition.

#### Corollary {#lie-iii-s4-n6-cor-1 .statement}

Let $M$ be an analytic manifold of finite dimension $n$. Let $\omega_1, \ldots, \omega_n$ be analytic differential forms of degree 1 on $M$, with scalar values, which are linearly independent at each point of $M$ and such that, for all $k = 1, \ldots, n$, $d\omega_k$ is a linear combination with constant coefficients of the $\omega_i \wedge \omega_j$. Then, for all $m_0 \in M$, there exists an open neighbourhood $M'$ of $m_0$ in $M$ and a Lie group germ structure on $M'$ compatible with the manifold structure on $M'$, with identity element $m_0$ and such that $\omega_1|_{M'}, \ldots, \omega_n|_{M'}$ form a basis of the space of left invariant differential forms on $M'$ of degree 1 with scalar values.

If $M'_1$ and $M'_2$ are two such group germs, $M'_1$ and $M'_2$ have a common open subgroup germ.

Let $X_1, \ldots, X_n$ be the vector fields on $M$ such that, at each point $m$ of $M$, the $(X_t)_m$ constitute the basis of $T_m(M)$ dual to $((\omega_1)_m, \ldots, (\omega_n)_m)$. These fields are analytic. By hypothesis, there exist $c_{ijk} \in \mathbf{K}$ ($1 \leq i, j, k \leq n$) such that $c_{ijk} = -c_{jik}$ and $d\omega_k = \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j$. By *Differentiable and Analytic Manifolds*, R, 8.5.7, formula (11),
$$
\langle [X_i, X_j], \omega_k \rangle = -(d\omega_k)(X_i, X_j) = -\left( \sum_{r < s} c_{rsk} \omega_r \wedge \omega_s \right)(X_i, X_j) = -c_{ijk}
$$
and hence $[X_i, X_j] = -\sum_k c_{ijk} X_k$. It then follows that the $-c_{ijk}$ are the constants of structure of a Lie algebra $g$ relative to a basis $(e_1, \ldots, e_n)$. For all $m \in M$, let $\alpha_m$ be the linear mapping of $T_m(M)$ into $g$ which maps $(X_1)_m$ to $e_1, \ldots, (X_n)_m$ to $e_n$. Then $\alpha$ is an analytic differential form on $M$ of degree 1 with values in $g$ and $\alpha_m$ is an isomorphism of $T_m(M)$ onto $g$. On the other hand, $\alpha = \sum_{k=1}^n \omega_k e_k$ and hence
$$
d\alpha = \sum_{k=1}^n (d\omega_k)e_k = \sum_{k=1}^n \left( \sum_{i<j} c_{ijk}\omega_i \wedge \omega_j \right)e_k
$$
and
$$
\begin{align*}
[\alpha]^2 &= \sum_{k=1}^n [\omega_k e_k]^2 + \sum_{i<j} (\omega_i e_i) \wedge (\omega_j e_j) \quad (§ 3, \text{formula (30)}) \\
&= \sum_{i<j} (\omega_i \wedge \omega_j)[e_i, e_j] \\
&= -\sum_{k=1}^n \sum_{i<j} (c_{ijk}\omega_i \wedge \omega_j)e_k \\
&= -d\alpha.
\end{align*}
$$
It then suffices to apply Proposition 10.

### 7. PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION

#### Proposition 11 {#lie-iii-s4-prop-11 .statement}

Let $G_1$ and $G_2$ be Lie group germs and $X_1$ and $X_2$ manifolds of class $C^r$ ($r \geq 2$). For $i = 1, 2$, let $\psi_i$ be a law chunk of left operation of class $C^r$ of $G_i$ on $X_i$ and $D_i$ the associated law of infinitesimal operation. Let $\mu : G_1 \to G_2$ be a morphism and $\phi : X_1 \to X_2$ a mapping of class $C^r$. Suppose that, for all $a \in L(G)$, the vector fields $(D_1)_a$ and $(D_2)_{L(\mu)a}$ are $\phi$-related (Differentiable and Analytic Manifolds, R, 8.2.6). Then there exists a neighbourhood $\Omega$ of $\{e\} \times X_1$ in $G_1 \times X_1$ such that $\phi(\psi_1(g, x)) = \psi_2(\mu(g), \phi(x))$ for all $(g, x) \in \Omega$.

Let $p_1 : G_1 \times X_2 \to G_1, p_2 : G_1 \times X_2 \to X_2$ be the canonical projections. For all $(g_1, x_2) \in G_1 \times X_2$, let $f_{g_1, x_2}$ be the mapping $g_1 a \mapsto (D_2)_{L(\mu)a}(x_2)$ of $T_{g_1}(G_1) = g_1 L(G_1)$ into $T_{x_2}(X_2)$. The $f_{g_1, x_2}$ define a morphism of $p_1^*T(G_1)$ into $p_2^*T(X_2)$.

Let $x_0 \in X_1$. There exist an open neighbourhood $G$ of $e$ in $G_1$ and an open neighbourhood $X$ of $x_0$ in $X_1$ such that $\psi_1(g, x)$ and $\psi_2(\mu(g), \phi(x))$ are defined for $(g, x) \in G \times X$. We write, for $(g, x) \in G \times X$,
$$
\alpha(g, x) = \phi(\psi_1(g, x)) \in X_2, \qquad \beta(g, x) = \psi_2(\mu(g), \phi(x)) \in X_2.
$$
If $G$ and $X$ are sufficiently small, then, for all $(a, g, x) \in L(G_1) \times G \times X$,
$$
\begin{align*}
(T\alpha)(ag, 0_x) &= (T\phi)((D_1)_a(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}(\phi(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}\alpha(g, x), \\
(T\beta)(ag, 0_x) &= (T\psi_2)(L(\mu)a.\mu(g), \phi(x)) \\
&= (D_2)_{L(\mu)a}(\psi_2(\mu(g), \phi(x))) \\
&= (D_2)_{L(\mu)a}\beta(g, x).
\end{align*}
$$

Hence for $x \in X$, the morphisms $g \mapsto \alpha(g, x)$ and $g \mapsto \beta(g, x)$ are integrals of $f$; as
$$
\beta(e, x) = \phi(x) = \alpha(e, x)
$$
for all $x \in X$, it follows from *Differentiable and Analytic Manifolds*, R, 9.3.7, that $\alpha$ and $\beta$ coincide on a neighbourhood of $(e, x_0)$. Hence the proposition.

#### Corollary {#lie-iii-s4-n7-cor-1 .statement}

*Let G be a Lie group germ and X a manifold of class $C^r$. Consider two law chunks of left operation of class $C^r$ of G on X. Suppose that, for all $a \in L(G)$, the corresponding vector field $D_a$ on X is the same for both law chunks. Then these two law chunks coincide on a neighbourhood of $\{e\} \times X$.*

#### Theorem 6 {#lie-iii-s4-thm-6 .statement}

*Let G be a Lie group germ, X a manifold of class $C^r$ ($r \geq 2$) and $x_0$ a point of X. Let $a \mapsto D_a$ be a law of left infinitesimal operation of class $C^{r-1}$ of $L(G)$ on X.*

(i) *There exists an open neighbourhood $X'$ of $x_0$ in X and a law chunk of left operation of class $C^{r-1}$ of G on $X'$ such that the associated law of infinitesimal operation is $a \mapsto D_a|X'$.*

(ii) *Let there be two law chunks of left operation of class $C^{r-1}$ of G on an open neighbourhood $X''$ of $x_0$; if they admit $a \mapsto D_a|X''$ as associated law of infinitesimal operation, they coincide on a neighbourhood of $(e, x_0)$.*

Assertion (ii) follows from the Corollary to Proposition 11. We prove (i). For all $(g, x) \in G \times X$ and all $a \in L(G)$, we write
$$
Q_a(g, x) = (ag, D_a(x)) \in T_g(G) \times T_x(X).
$$
Let $S_{(g, x)}$ be the set of $Q_a(g, x)$ for $a \in L(G)$. By Lemma 5 of no. 6, the $S_{(g, x)}$ are the fibres of a vector subbundle S of $T(G) \times T(X)$. Let $a, b$ be in $L(G)$; then
$$
\begin{align*}
[Q_a, Q_b](g, x) &= ([R_a, R_b](g), [D_a, D_b](x)) \\
&= (-R_{[a, b]}(g), -D_{[a, b]}(x)) \quad (§ 3, 18.6) \\
&= Q_{-[a, b]}(g, x)
\end{align*}
$$
and hence S is integrable (*Differentiable and Analytic Manifolds*, R, 9.3.3, (iv)).

By *Differentiable and Analytic Manifolds*, R, 9.3.7, there exist an open neighbourhood $G_1$ of e in G, an open neighbourhood $X_1$ of $x_0$ in X and a mapping $(g, x) \mapsto gx$ of class $C^{r-1}$ of $G_1 \times X_1$ into X such that $ex = x$ for all $x \in X_1$ and
$$
(ag)x = D_a(gx) \quad \text{for } a \in L(G), g \in G_1, x \in X_1.
$$
In particular
$$
ax = D_a(x).
$$
Let $G_2$ be an open neighbourhood of e in $G_1$ and $X_2$ an open neighbourhood of $x_0$ in $X_1$ such that $gg'$ is defined and belongs to $G_1$ for $g, g'$ in $G_2$ and $gx$ is defined and belongs to $X_1$ for $(g, x) \in G_2 \times X_2$. Consider the mappings $\alpha_1, \alpha_2$ of $G_2 \times (G_2 \times X_2)$ into $X$ defined by
$$
\alpha_1(g, (h, x)) = g(hx), \quad \alpha_2(g, (h, x)) = (gh)x.
$$
They are of class $C^{r-1}$. Then
$$
\alpha_1(e, (h, x)) = hx = \alpha_2(e, (h, x)).
$$
On the other hand
$$
\begin{align*}
T(\alpha_1)(ag, 0_{(h, x)}) &= (ag)(hx) \\
&= D_a(g(hx)) \qquad \text{by (6)} \\
&= D_a(\alpha_1(g, (h, x))), \\
T(\alpha_2)(ag, 0_{(h, x)}) &= (agh)x \\
&= D_a((gh)x) \qquad \text{by (6)} \\
&= D_a(\alpha_2(g, (h, x))).
\end{align*}
$$
By *Differentiable and Analytic Manifolds*, R, 9.3.7, $\alpha_1$ and $\alpha_2$ coincide on a neighbourhood of $(e, (e, x_0))$. Then (i) follows from (7) and Proposition 23 of § 1, no. 11.

#### Corollary 1 {#lie-iii-s4-thm-6-cor-1 .statement}

*Let $G$ be a Lie group germ and $X$ a paracompact manifold of class $C^r$ ($r \geq 2$). Let $a \mapsto D_a$ be a law of left infinitesimal operation of class $C^{r-1}$ of $L(G)$ on $X$.

(i) There exists a law chunk of left operation of class $C^{r-1}$ of $G$ on $X$ such that the associated law of infinitesimal operation is $a \mapsto D_a$.

(ii) Two laws of left operation of class $C^{r-1}$ of $G$ on $X$ which admit $a \mapsto D_a$ as associated law of infinitesimal operation coincide on a neighbourhood of $\{e\} \times X$.

Assertion (ii) follows from the Corollary to Proposition 11. By Theorem 6 (i), there exist an open covering $(X_i)_{i \in I}$ of $X$ and, for all $i \in I$, a law chunk of left operation $\psi_i$ of Class $C^{r-1}$ of $G$ on $X_i$ such that the associated law of infinitesimal operation is $a \mapsto D_a|_{X_i}$. As $X$ is paracompact, the covering $(X_i)_{i \in I}$ can be assumed to be locally finite. For all $(i, j) \in I \times I$ and all $x \in X_i \cap X_j$, $\psi_i$ and $\psi_j$ coincide on a neighbourhood of $(e, x)$ (Corollary to Proposition 11). As $X$ is normal, we can apply Proposition 24 of § 1, no. 11, which proves (i).

#### Corollary 2 {#lie-iii-s4-thm-6-cor-2 .statement}

*Let $X$ be a paracompact manifold of class $C^r$ ($r \geq 2$) and $\xi$ a vector field of class $C^{r-1}$ on $X$. There exists a law chunk of operation $\psi$ of class $C^{r-1}$ of $K$ on $X$ such that for all $x \in X$, $\xi(x)$ is the image under $t \mapsto (t, x)$ of the tangent vector 1 to $K$ at 0. Two law chunks of operation with the above property coincide on a neighbourhood of $\{0\} \times X$.

This is a special case of Corollary 1.*

§ 5.1

#### Remark {#lie-iii-s4-n7-rem-1 .statement}

Laws of left operation can of course be replaced, throughout this no., by laws of right operation.

### Exercises {#lie-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
