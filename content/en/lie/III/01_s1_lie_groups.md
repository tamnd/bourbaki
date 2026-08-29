---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 1
section_title: Lie groups
lang: en
source: lie-i-iii
book_pages: 209-233, 370-372
pdf_pages: 0227-0251, 0388-0390
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A LIE GROUP
      page: 209
      pdf_page: 227
    - "no": 2
      title: MORPHISMS OF LIE GROUPS
      page: 213
      pdf_page: 231
    - "no": 3
      title: LIE SUBGROUPS
      page: 214
      pdf_page: 232
    - "no": 4
      title: SEMI-DIRECT PRODUCTS OF LIE GROUPS
      page: 215
      pdf_page: 233
    - "no": 5
      title: QUOTIENT OF A MANIFOLD BY A LIE GROUP
      page: 217
      pdf_page: 235
    - "no": 6
      title: HOMOGENEOUS SPACES AND QUOTIENT GROUPS
      page: 219
      pdf_page: 237
    - "no": 7
      title: ORBITS
      page: 222
      pdf_page: 240
    - "no": 8
      title: VECTOR BUNDLES WITH OPERATORS
      page: 223
      pdf_page: 241
    - "no": 9
      title: LOCAL DEFINITION OF A LIE GROUP
      page: 226
      pdf_page: 244
    - "no": 10
      title: GROUP GERMS
      page: 228
      pdf_page: 246
    - "no": 11
      title: LAW CHUNKS OF OPERATION
      page: 231
      pdf_page: 249
statements: 54
exercises: 10
content_sha256: 1d086b2132020ca1ae70342f05ee30e3bf32e38ffd0a0c2a6d1cdfbca1dc4cf8
---

## § 1. LIE GROUPS

### 1. DEFINITION OF A LIE GROUP

Let G be a set. A group structure and an analytic K-manifold structure on G are called compatible if the following condition holds:
(GL) The mapping $(g, h) \mapsto gh^{-1}$ of $G \times G$ into G is analytic.

#### Definition 1 {#lie-iii-s1-def-1 .statement}

*A Lie group over K is a set G with a group structure and an analytic K-manifold structure such that these two structures are compatible.*

A Lie group over $\mathbf{R}$ (resp. $\mathbf{C}$, $\mathbf{Q}_p$) is called a real (resp. complex, $p$-adic) Lie group.

Let G be a group with an analytic manifold structure. For $g, h, g_0, h_0$ in G,
$$
gh^{-1} = (g_0 h_0^{-1}) h_0 ((g_0^{-1} g)(h_0^{-1} h)^{-1}) h_0^{-1}.
$$
It follows that G is a Lie group if and only if the following three conditions hold:

(GL$_1$) for all $g_0 \in G$, the mapping $g \mapsto g_0 g$ of G into G is analytic;
(GL$_2$) for all $g_0 \in G$, the mapping $g \mapsto g_0 g g_0^{-1}$ of G into G is analytic in an open neighbourhood of $e$;
(GL$_3$) the mapping $(g, h) \mapsto gh^{-1}$ of $G \times G$ into G is analytic in an open neighbourhood of $(e, e)$.

Let G be a Lie group. For all $g \in G$, $\gamma(g)$ and $\delta(g)$ are automorphisms of the underlying manifold of G. It follows that this manifold is pure (*Differentiable and Analytic Manifolds*, R, 5.1.7). In particular, the dimension of G at $g$ is equal to $\dim G$ for all $g \in G$ (recall that $\dim G$ is an integer $\geqslant 0$ or $+\infty$).

Since an analytic mapping is continuous, a Lie group is a topological group with the underlying topology of its manifold structure. Let G be a set. A topological group structure and an analytic K-manifold structure on G are called *compatible* if the group structure and the manifold structure are compatible and the topology on G is the topology underlying the manifold structure.

#### Lemma 1 {#lie-iii-s1-lem-1 .statement}

*Let G be a Lie group, U an open neighbourhood of e, E a complete normed space and $\phi : U \to E$ a chart of the manifold G. There exists a neighbourhood W of e contained in U such that $\phi | W$ is an isomorphism of W (with the right uniform structure) onto $\phi(W)$ (with the uniform structure induced by that on E).*

It can be assumed that $\phi(e) = 0$. Let $U' = \phi(U)$. Let $\psi : U' \to U$ be the inverse mapping of $\phi$. Let V be a symmetric open neighbourhood of e such that $V^2 \subset U$ and let $V' = \phi(V)$. We define mappings $\theta_1, \theta_2$ of $V' \times V'$ into $V' \times U'$ as follows:
$$
\begin{align*}
\theta_1(x, y) &= (x, \phi(\psi(x)\psi(y)^{-1})) \\
\theta_2(x, y) &= (x, \phi(\psi(y)^{-1}\psi(x))).
\end{align*}
$$
It is immediately verified that $\theta_2(\theta_1(x, y)) = \theta_1(\theta_2(x, y)) = (x, y)$ for $x, y$ sufficiently close to 0. On the other hand, $\theta_1$ and $\theta_2$ are analytic and hence strictly differentiable at $(0, 0)$. Therefore (*Differentiable and Analytic Manifolds*, R, 1.2.2) there exist a neighbourhood $W'$ of 0 in $V'$ and constants $a > 0, b > 0$ such that
$$
a(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
\leq \|x_1 - x_2\| + \|y_1 - y_2\|
\leq b(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
$$

for all $x_1, x_2, y_1, y_2$ in $W'$. Writing $x_1 = x_2 = y_2$, we obtain

$$
(2) \quad a \| \phi(\psi(x_1)\psi(y_1)^{-1}) \| \leq \| x_1 - y_1 \| \leq b \| \phi(\psi(x_1)\psi(y_1)^{-1}) \|.
$$

For $\delta > 0$, let $N_\delta$ be the set of ordered pairs $(x, y) \in W' \times W'$ such that $\| x - y \| \leq \delta$. The $N_\delta$ form a fundamental system of entourages in $W'$. We write $W = \psi(W')$. Let $M_\delta$ be the set of ordered pairs $(u, v) \in W \times W$ such that $\| \phi(uv^{-1}) \| \leq \delta$. The $M_\delta$ form a fundamental system of entourages in $W$ with the right uniform structure. But relation (2) proves that

$$
N_\delta \subset (\phi \times \phi)(M_{a^{-1}\delta}), \qquad (\phi \times \phi)(M_\delta) \subset N_{b\delta}
$$

and hence $W$ has the property of the lemma.

#### Proposition 1 {#lie-iii-s1-prop-1 .statement}

*A Lie group is a complete metrizable topological group.*

Since $e$ admits an open neighbourhood homeomorphic to an open ball of a normed space, $e$ admits a countable fundamental system of neighbourhoods whose intersection is $\{e\}$. Hence $G$ is metrizable (*General Topology*, Chapter III, § 1, Corollary to Proposition 2 and Chapter IX, § 3, Proposition 1). By Lemma 1, there exists a neighbourhood of $e$ which is complete under the right uniform structure and hence $G$ is complete (*General Topology*, Chapter III, § 3, Proposition 4).

#### Proposition 2 {#lie-iii-s1-prop-2 .statement}

*Let $G$ be a Lie group.*
(i) *If $K = \mathbf{R}$ or $\mathbf{C}$, $G$ is locally connected.*
(ii) *If $K$ is distinct from $\mathbf{R}$ and $\mathbf{C}$, $G$ is zero-dimensional* (*General Topology*, Chapter IX, § 6, Definition 5).
(iii) *Suppose that $K$ is locally compact. For $G$ to be locally compact, it is necessary and sufficient that $G$ be finite-dimensional.*
(iv) *If $G$ is generated by a subspace whose topology admits a countable base, then the topology on $G$ admits a countable base.*

Let $U$ be a neighbourhood of $e$. There exists an open neighbourhood $U_1$ of $e$ contained in $U$ and homeomorphic to an open ball of a normed space $E$ over $K$. If $K = \mathbf{R}$ or $\mathbf{C}$, $U_1$ is connected, which proves (i). Suppose that $K$ is ultrametric. There exists a neighbourhood $U_2$ of $e$ which is closed in $G$ and such that $U_2 \subset U_1$. Then there exists a neighbourhood $U_3$ of $e$ such that $U_3 \subset U_2$ and $U_3$ is open and closed relative to $U_1$. Then $U_3$ is closed relative to $U_2$ and hence $G$ and open relative to $U_1$ and hence $G$. This proves (ii). For $G$ to be locally compact, it is necessary and sufficient that $E$ be locally compact; if $K$ is locally compact, this amounts to saying that $E$ is finite-dimensional (*Topological Vector Spaces*, Chapter I, § 2, Theorem 3), whence (iii). Suppose that $G$ is generated by a subset $V$ and let $W = V \cup V^{-1}$; then

$$
G = W \cup W^2 \cup W^3 \cup \ldots;
$$

if there exists a sequence dense in $V$, we see that there exists a sequence dense in G and, as G is metrizable (Proposition 1), the topology on G admits a countable base.

#### Corollary {#lie-iii-s1-n1-cor-1 .statement}

If K = R or C and G is connected and finite-dimensional, then G is locally connected and locally compact and its topology admits a countable base.

#### Lemma 2 {#lie-iii-s1-lem-2 .statement}

Let X be a manifold of class C^r, e a point of X, U and V open neighbourhoods of e and m a mapping of class C^r of U × U into X satisfying the following conditions:
(a) m(e, x) = m(x, e) = x for all x ∈ U;
(b) V ⊂ U, m(V × V) ⊂ U and m(m(x, y), z) = m(x, m(y, z)) for all x, y, z in V.

Then there exists an open neighbourhood W of e in V and an automorphism θ of the manifold W such that θ(e) = e, θ(θ(x)) = x and m(x, θ(x)) = m(θ(x), x) = e for all x ∈ W.

m(e, y) = y for all y ∈ U and hence, by the implicit function theorem, there exists an open neighbourhood W_1 of e in V and a mapping θ_1 of class C^r of W_1 into V such that θ_1(e) = e, m(x, θ_1(x)) = e for all x ∈ W_1. Similarly, there exists an open neighbourhood W_2 of e in V and a mapping θ_2 of class C^r of W_2 into V such that θ_2(e) = e, m(θ_2(x), x) = e for all x ∈ W_2. For x ∈ W_1 ∩ W_2,

$$
\begin{align*}
θ_2(x) &= m(θ_2(x), e) = m(θ_2(x), m(x, θ_1(x))) \\
&= m(m(θ_2(x), x), θ_1(x)) = m(e, θ_1(x)) = θ_1(x).
\end{align*}
$$

Let θ(x) be the common value of θ_1(x) and θ_2(x) for x ∈ W_1 ∩ W_2. Let W be the set of x ∈ W_1 ∩ W_2 such that θ(x) ∈ W_1 ∩ W_2. The set W is open. For x ∈ W,

$$
θ(θ(x)) = m(m(x, θ(x)), θ(θ(x))) = m(x, m(θ(x), θ(θ(x)))) = m(x, e) = x
$$

and hence θ(x) ∈ W. We see that θ | W defines an automorphism of the manifold W.

#### Proposition 3 {#lie-iii-s1-prop-3 .statement}

Let X be an analytic manifold and m an analytic associative law of composition on X admitting an identity element. The set G of invertible elements of X is open in X and G is a Lie group with m | (G × G) and the manifold structure induced by that on X.

By Lemma 2, G is a neighbourhood of the identity element. For all g ∈ G, the mapping x ↦ m(g, x) is an automorphism of the manifold X. Hence the image of G under this mapping is a neighbourhood of g, obviously contained in G. Therefore G is open in X. Clearly conditions (GL_1) and (GL_2) hold. Condition (GL_3) holds by Lemma 2.

Examples of Lie groups

(1) Let E be a complete normable space over K. The mapping (x, y) ↦ x − y of E × E into E is continuous and linear and hence analytic.

Hence E, with its additive group and analytic manifold structures, is a Lie group.

In particular, K is a Lie group.

(2) Let A be a complete normable unital associative algebra over K. The multiplication $(x, y) \mapsto xy$ of $A \times A$ into A is bilinear and continuous and hence analytic. Proposition 3 shows that the group $A^*$ of invertible elements of A is open in A (which also follows from *General Topology*, Chapter IX, § 3, Proposition 13) and that $A^*$ is a Lie group.

For example, let E be a complete normable space over K and let $A = \mathcal{L}(E)$ (*General Topology*, Chapter IX, § 3, Proposition 5). Then $A^*$ is the automorphism group $\mathbf{GL}(E)$ of E. *This group therefore has canonically a Lie group structure over K*. More particularly, $\mathbf{GL}(n, K)$, with the manifold structure induced by that on $\mathbf{M}_n(K)$, is a Lie group. For $n = 1$, we see that the multiplicative group $K^*$ is a Lie group with the manifold structure induced by that on K.

(3) Let G be a Lie group over K. Let $K' = \mathbf{R}$ or $\mathbf{C}$ or a non-discrete complete ultrametric field and $\sigma$ an isomorphism of the valued field $K'$ onto a valued subfield of K. Then the group G, with the $K'$-manifold structure obtained by restriction of scalars, is a Lie group over $K'$, which is said to be *derived from the Lie group G by restriction of scalars* (from K to $K'$ by means of $\sigma$). For example, every complex Lie group has canonically a real Lie group structure. Again, with every complex Lie group G is associated a complex Lie group called the *conjugate* of G, derived from G by means of the automorphism $z \mapsto \overline{z}$ of $\mathbf{C}$.

### 2. MORPHISMS OF LIE GROUPS

#### Definition 2 {#lie-iii-s1-def-2 .statement}

*Let G and H be Lie groups. A Lie group morphism of G into H (or simply a morphism of G into H if no confusion can arise) is a mapping of G into H which is a group homomorphism and is analytic. The automorphism group of G is denoted by $\operatorname{Aut}(G)$.*.

The identity mapping of G is a morphism. The composition of two morphisms is a morphism. If $f : G \to H$ and $f' : H \to G$ are two inverse morphisms, $f$ and $f'$ are Lie group isomorphisms.

#### Example {#lie-iii-s1-n2-exa-1 .statement}

(1) Let G be a Lie group. For all $x \in G$, $\operatorname{Int}(x)$ is an automorphism of the Lie group G.

(2) Let G be a Lie group. Let $G^\vee$ denote the opposite group to G, with the same manifold structure as G. It is immediate that $G^\vee$ is a Lie group (called the *opposite* Lie group to G) and that the mapping $g \mapsto g^{-1}$ is an isomorphism of the Lie group G onto the Lie group $G^\vee$.

(3) Let G be a Lie group and E a complete normable space. An *analytic linear representation* of G on E (or simply a linear representation of G on E when no confusion can arise) is a morphism of the Lie group G into the Lie group $\mathbf{GL}(E)$, in other words an analytic mapping $\pi$ of G into $\mathbf{GL}(E)$ such that $\pi(gg') = \pi(g)\pi(g')$ for $g, g'$ in G. Suppose that E admits a finite basis $(e_1, e_2, \ldots, e_n)$ over K; let $(e_1^*, e_2^*, \ldots, e_n^*)$ be the dual basis; let $\rho$ be a homomorphism of the group G into the group $\mathbf{GL}(E)$; then the following conditions are equivalent:
(i) $\rho$ is an analytic linear representation;
(ii) for all $x \in E$ and $x' \in E'$, the function $g \mapsto \langle \rho(g)x, x' \rangle$ on G is analytic;
(iii) for all i and j, the function $g \mapsto \langle \rho(g)e_i, e_j^* \rangle$ on G is analytic.
For the implications (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) are clear. On the other hand, the functions $u \mapsto \langle ue_i, e_j^* \rangle$ form a coordinate system on $\mathscr{L}(E)$; hence their restrictions to $\mathbf{GL}(E)$ form a coordinate system on $\mathbf{GL}(E)$, whence the implication (iii) $\Rightarrow$ (i).

Let G be a real Lie group, E a real complete normable space and $\rho$ a homomorphism of the group G into the group $\mathbf{GL}(E)$. We shall see in § 8, Theorem 1 that, if $\rho$ is continuous (when $\mathbf{GL}(E)$ has the topology derived from the norm on $\mathbf{L}(E)$), then $\rho$ is analytic. But note that this notion of continuity is different from that considered in Integration, Chapter VIII, § 2, Definition 1 (iii) (Exercise 1).

(4) Let G be a real Lie group and E a complex complete normable space. An analytic linear representation of G on E is a morphism of G into the underlying real Lie group of $\mathbf{GL}(E)$.

#### Proposition 4 {#lie-iii-s1-prop-4 .statement}

Let G and H be Lie groups and f a homomorphism of the group G into the group H. For f to be analytic, it is necessary and sufficient that there exist a non-empty open subset U of G such that $f|_U$ is analytic.

The condition is obviously necessary. Suppose that it holds. For all $x_0 \in G$, $f(x_0x) = f(x_0)f(x)$ for all $x \in U$ and hence $f|_{x_0U}$ is analytic. But the sets $x_0U$, where $x_0 \in G$, form an open covering of G.

#### Remark {#lie-iii-s1-n2-rem-1 .statement}

If f is an immersion at e (resp. a submersion at e), clearly f is an immersion (resp. a submersion).

### 3. LIE SUBGROUPS

Let G be a Lie group and H a subgroup of G which is at the same time a submanifold of G. Then the mapping $(x, y) \mapsto xy^{-1}$ of $H \times H$ into G is analytic and hence the mapping $(x, y) \mapsto xy^{-1}$ of $H \times H$ into H is analytic. (Differentiable and Analytic Manifolds, R, 5.8.5). Thus H, with the group and manifold structures induced by those on G, is a Lie group.

#### Definition 3 {#lie-iii-s1-def-3 .statement}

Let G be a Lie group. A subset H of G is called a Lie subgroup if H is a subgroup and a submanifold of G.

An open subgroup of G is a Lie subgroup of G. In particular, if G is a real or complex Lie group, its identity component is a Lie subgroup of G.

#### Proposition 5 {#lie-iii-s1-prop-5 .statement}

Let G be a Lie group and H a Lie subgroup of G.
(i) H is closed in G.
(ii) The canonical injection of H into G is a Lie group morphism.
(iii) Let L be a Lie group and f a mapping of L into G such that f(L) ⊂ H. For f to be a morphism of L into H, it is necessary and sufficient that f be a morphism of L into G.

By Differentiable and Analytic Manifolds, R, 5.8.3, H is locally closed. Hence H is closed (General Topology, Chapter III, § 2, Proposition 4). Assertion (ii) is obvious. Assertion (iii) follows from Differentiable and Analytic Manifolds, R, 5.8.5.

#### Proposition 6 {#lie-iii-s1-prop-6 .statement}

Let G be a Lie group and H a subgroup of G. For H to be a Lie subgroup of G, it is necessary and sufficient that there exist a point h ∈ H and an open neighbourhood U of h in G such that H ∩ U is a submanifold of G.

The condition is obviously necessary. Suppose that it holds. For all h' ∈ H, the translation γ(h'h^{-1}) is an automorphism of the manifold G and maps the submanifold H ∩ U of U into the submanifold (h'h^{-1}H) ∩ (h'h^{-1}U) of h'h^{-1}U. As h'h^{-1}H = H and h'h^{-1}U is an open neighbourhood of h' in G, we see that every point of H has an open neighbourhood V such that V ∩ H is a submanifold of G. Hence H is a submanifold of G.

Let G be a Lie group and H a Lie subgroup of G. If L is a Lie subgroup of H, L is a Lie subgroup of G by Differentiable and Analytic Manifolds, R, 5.8.6. Let M be a Lie subgroup of G such that M ⊂ H. Then M is a Lie subgroup of H, for the canonical injection of M into H is obviously an immersion.

Let k be a non-discrete closed subfield of K. A Lie k-subgroup of G is a Lie subgroup of the underlying Lie k-group of G.

#### Remark {#lie-iii-s1-n3-rem-1 .statement}

If "submanifold" is replaced by "quasi-submanifold" in Definition 3, we obtain the definition of Lie quasi-subgroups of G. (For finite-dimensional G, the Lie quasi-subgroups are just the Lie subgroups.) Suppose that K is of characteristic 0. Proposition 5 remains valid with the same proof for Lie quasi-subgroups. Proposition 6 remains valid with the same proof, replacing "Lie subgroup" by "Lie quasi-subgroup" and "submanifold" by "quasi-submanifold".

### 4. SEMI-DIRECT PRODUCTS OF LIE GROUPS

Let I be a finite set and (L_i)_{i \in I} a family of Lie groups. The group and manifold structures on L = \prod_{i \in I} L_i are compatible and L thus has a Lie group structure. L is called the product Lie group of the family of Lie groups (L_i)_{i \in I}.

Let L and M be Lie groups and σ a homomorphism of L into the automorphism group of the group M. Let S be the external semi-direct product of L by M relative to σ (Algebra, Chapter I, § 6, no. 1, Definition 2).

#### Proposition 7 {#lie-iii-s1-prop-7 .statement}

*If the mapping* $(m, l) \mapsto \sigma(l)m$ *of* $M \times L$ *into* $M$ *is analytic, the group* $S$, *with the product manifold structure of* $M$ *and* $L$, *is a Lie group*.

For $l, l'$ in $L$ and $m, m'$ in $M$,

$$
(m, l)(m', l')^{-1} = ml{l'}^{-1}{m'}^{-1} = m(\sigma(l{l'}^{-1}){m'}^{-1})l{l'}^{-1}
= (m(\sigma(l{l'}^{-1}){m'}^{-1}), l{l'}^{-1})
$$

whence the proposition.

If the conditions of Proposition 7 hold, the Lie group $S$ is called the (*external*) *semi-direct product Lie group of* $L$ *by* $M$ *relative to* $\sigma$.

Clearly the canonical injection of $L$ (resp. $M$) into $S$ is an isomorphism of $L$ (resp. $M$) onto a Lie subgroup of $S$ which we identify with $L$ (resp. $M$). The canonical mapping of $S$ onto $L$ is a Lie group morphism.

Conversely, let $G$ be a Lie group and $L$, $M$ two Lie subgroups such that the group $G$ is (algebraically) the semi-direct product of $L$ by $M$ (*Algebra*, Chapter I, § 6, no. 1). We write $\sigma(l)m = lml^{-1}$ for $l \in L$ and $m \in M$. Then $\sigma$ satisfies the conditions of Proposition 7. We can therefore form the semi-direct product Lie group $S$ of $L$ by $M$ relative to $\sigma$. The mapping $j: (m, l) \mapsto ml$ of $S$ onto $G$ is a group isomorphism and is analytic. If $j$ is a Lie group isomorphism, *the Lie group* $G$ *is called the* (*internal*) *semi-direct product of* $L$ *by* $M$ *and* $S$ *and* $G$ *are identified*. For all $g \in G$, we write $g = p(g)q(g)$, where $p(g) \in M$ and $q(g) \in L$. For the Lie group $G$ to be the semi-direct product of $L$ by $M$, it is necessary and sufficient that one of the mappings $p: G \to M$ and $q: G \to L$ be analytic, in which case both are analytic; or alternatively, it is necessary and sufficient that $T_e(G)$ be the topological direct sum of $T_e(M)$ and $T_e(L)$ (for, if this condition holds, $j$ is étale at $e_S$).

#### Example {#lie-iii-s1-n4-exa-1 .statement}

Let $E$ be a normable space, $G = \mathbf{GL}(E)$, $T$ the translation group of $E$ and $A$ the permutation group of $E$ generated by $G$ and $T$. The group $A$ is algebraically the semi-direct product of $G$ by $T$. (If $E$ is finite-dimensional, $A$ is the affine group of $E$, cf. *Algebra*, Chapter II, § 9, no. 4). Let $\sigma$ be the identity linear representation of $G$ on $E$ and $S$ the external semi-direct product of $G$ by $E$ relative to $\sigma$. For all $x \in E$, let $t_x$ be the translation of $E$ defined by $x$. The mapping $(x, u) \mapsto t_x \circ u$ is isomorphism $\Phi$ of the group $S$ onto the group $A$. The mapping $(x, u) \mapsto \sigma(u)x = u(x)$ of $E \times \mathcal{L}(E)$ into $E$ is continuous and bilinear and hence analytic; its restriction to $E \times G$ is therefore analytic. Thus the group $S$, with the product manifold structure of $E$ and $G$, is a Lie group. We transport this structure to $A$ by means of $\Phi$. Then $A$ becomes a Lie group, the internal semi-direct product of $G$ by $T$ as a Lie group.

#### Proposition 8 {#lie-iii-s1-prop-8 .statement}

*Let* $G$ *and* $H$ *be Lie groups, $p: G \to H$ and $s: H \to G$ Lie group morphisms such that* $p \circ s = \mathrm{id}_H$ *and* $N = \mathrm{Ker}\ p$. *Then* $N$ *is a Lie subgroup of* $G$, *s is an isomorphism of* $H$ *onto a Lie subgroup of* $G$ *and the Lie group* $G$ *is the internal semi-direct product of* $s(H)$ *by* $N$.

$T_e(p) \circ T_e(s) = \mathrm{id}_{T_{e(H)}}$ and hence $p$ (resp. $s$) is a submersion (resp. an immersion). By *Differentiable and Analytic Manifolds*, R, 5.10.5, N is a Lie subgroup of G. On the other hand, $s$ is a homeomorphism of H onto $s(H)$ and hence $s$ is an isomorphism of H onto a Lie subgroup of G (*Differentiable and Analytic Manifolds*, R, 5.8.3). Finally, for all $g \in G$, $g = (s \circ p)(g) \cdot n$ for some $n \in N$; as $s \circ p$ is analytic, the Lie group G is the semi-direct product of $s(H)$ by N.

### 5. QUOTIENT OF A MANIFOLD BY A LIE GROUP

Let G be a Lie group, X a manifold of class $C^r$ and $(g, x) \mapsto gx$ a law of left operation (*Algebra*, Chapter I, § 5, no. 1) of class $C^r$ of G on X. For all $g \in G$, let $\tau(g)$ denote the automorphism $x \mapsto gx$ of X defined by g. For all $x \in X$, let $\rho(x)$ denote the orbital mapping $g \mapsto gx$ of G into X defined by x. Then

$$
\rho(x) = \rho(gx) \circ \delta(g), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \gamma(g^{-1})
$$

for all $g \in G$ and $x \in X$. Hence

$$
T_g(\rho(x)) = T_e(\rho(gx)) \circ T_g(\delta(g))
$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\gamma(g^{-1}))
$$

#### Proposition 9 {#lie-iii-s1-prop-9 .statement}

*Let $x \in X$ and $g_0 \in G$.*

(i) *If $\rho(x)$ is an immersion (resp. a submersion, a subimmersion) at $g_0$, then, for all $g \in G$, $\rho(gx)$ is an immersion (resp. a submersion, a subimmersion).*

(ii) *If $\rho(x)$ is of rank k at $g_0$, then for all $g \in G$, $\rho(gx)$ is of constant rank equal to k.*

This follows immediately from formulae (4) and (5) since $T_g(\delta(g)), T_x(\tau(g))$ and $T_g(\gamma(g^{-1}))$ are isomorphisms.

#### Corollary {#lie-iii-s1-n5-cor-1 .statement}

*Let $x \in X$. If K is of characteristic 0 and X is finite-dimensional, $\rho(x)$ is a subimmersion. If further $\rho(x)$ is injective, $\rho(x)$ is an immersion.*

This follows from Proposition 9 and *Differentiable and Analytic Manifolds*, R, 5.10.6.

Observe that, if $\eta$ denotes the mapping $(g, x) \mapsto gx$ of $G \times X$ into X, then, for $g \in G, x \in X, u \in T_g(G), v \in T_x(X)$,

$$
T_{(g, x)}(\eta)(u, v) = T_{(g, x)}(\eta)(u, 0) + T_{(g, x)}(\eta)(0, x)
$$

that is

$$
T_{(g, x)}(\eta)(u, v) = T_g(\rho(x))u + T_x(\tau(g))v.
$$

#### Proposition 10 {#lie-iii-s1-prop-10 .statement}

*Let G be a Lie group and X a manifold of class $C^r$ with a law of left operation of class $C^r$ of G on X. Suppose that:*

(a) *the group G operates properly and freely on X;*

(b) *for all $x \in X$, $\rho(x)$ is an immersion (which is a consequence of (a) if K is of characteristic 0 and X is finite-dimensional).*

Then the equivalence relation defined by G on X is regular (Differentiable and Analytic Manifolds, R, 5.9.5). There exists on the quotient set X/G one and only one manifold structure such that the canonical mapping $\pi : X \to X/G$ is a submersion. The underlying topology of this manifold structure is the quotient topology of that on X; it is Hausdorff. Finally, $(X, G, X/G, \pi)$ is a principal left fibre bundle.\footnote{† The principal fibre bundles defined in Differentiable and Analytic Manifolds, R, 6.2.1 are principal right fibre bundles. The definition of principal left fibre bundles can be deduced from this in an obvious way.}

Let $\theta$ be the mapping $(g, x) \mapsto (x, gx)$ of $G \times X$ into $X \times X$. This mapping is of class $C^\tau$. We show that it is an immersion. For $u \in T_g(G)$ and $v \in T_x(X)$, by (6),

$$
T_{(g, x)}(\theta)(u, v) = (v, T_g(\rho(x))u + T_x(\tau(g))v).
$$

But $T_g(\rho(x))$ is injective by hypothesis (b) and hence $T_{(g, x)}(\theta)$ is injective. Its image is the topological direct sum of the subspace $H_{g, x}$ consisting of the vectors $(v, T_x(\tau(g))v)$ for $v \in T_x(X)$ and the subspace

$$
I_{g, x} = \{0\} \times T_g(\rho(x))(T_g(G)).
$$

By hypothesis (b), $T_g(\rho(x))(T_g(G))$ admits a topological supplement $J_{g, x}$ in $T_{gx}(X)$. Hence the image of $T_{(g, x)}(\theta)$ admits the topological supplement $\{0\} \times J_{g, x}$. Hence we have proved that $\theta$ is an immersion of $G \times X$ in $X \times X$.

As G operates freely on X, $\theta$ is injective. Let C be the graph of the equivalence relation R defined by G on X. As G operates properly, $\theta$ is a homeomorphism of $G \times X$ onto C (General Topology, Chapter I, § 10, Proposition 2). By Differentiable and Analytic Manifolds, R, 5.8.3, it is a submanifold of $X \times X$ and $\theta$ is an isomorphism of the manifold $G \times X$ onto the manifold C. The tangent space $T_{(x, gx)}(C)$ is identified with

$$
T_{(g, x)}(\theta)(T_{(g, x)}(G \times X)) = H_{g, x} \oplus I_{g, x} \subset T_{(x, gx)}(X \times X).
$$

Let pr$_1$ and pr$_2$ be the canonical projections of $X \times X$ onto the two factors. It is immediate that $T_{(x, gx)}(\mathrm{pr}_1)$ maps $H_{g, x}$ onto $T_x(X)$ and that the kernel of $T_{(x, gx)}(\mathrm{pr}_1) | T_{(x, gx)}(C)$ is $I_{g, x}$. Thus $\mathrm{pr}_1 | C$ is a submersion of C onto X. By Differentiable and Analytic Manifolds, R, 5.9.5, R is regular. By definition, there therefore exists on the quotient set X/G one and only one manifold structure such that $\pi$ is a submersion. The underlying topology of X/G is the quotient topology of that of X (Differentiable and Analytic Manifolds, R, 5.9.4). This topology is Hausdorff (General Topology, Chapter III, § 4, Proposition 3).

For all $b \in X/G$, there exist an open neighbourhood W of b and a morphism $\sigma : W \to X$ such that $\pi \circ \sigma = \mathrm{id}_W$ (Differentiable and Analytic Manifolds, R, 5.9.1). Let $\phi$ be the bijection $(g, w) \mapsto g\sigma(w)$ of $G \times W$ onto $\pi^{-1}(W)$. It is of class $C^\tau$. Then $\pi(g\sigma(w)) = w$ and

$$
\theta^{-1}(\sigma(w), g\sigma(w)) = (g, \sigma(w))
$$

and hence the inverse bijection of $\phi$ is of class $C^r$. Clearly $\phi(gg', w) = g\phi(g', w)$ for $w \in W,\ g \in G,\ g' \in G$. Hence $(X, G, X/G, \pi)$ is a principal left fibre bundle.

#### Remark {#lie-iii-s1-n5-rem-1 .statement}

With the above hypotheses, further let $H$ be a manifold of class $C^r$ and $(x, h) \mapsto m(x, h)$ a mapping of class $C^r$ of $X \times H$ into $X$ such that $m(gx, h) = gm(x, h)$ for $x \in X,\ g \in G,\ h \in H$. Let $n$ be the mapping of $(X/G) \times H$ into $X/G$ derived from $m$ by taking quotients. We show that $n$ *is of class* $C^r$. Consider the diagram

$$
\begin{array}{ccc}
X \times H & \xrightarrow{m} & X \\
\pi \times 1 \downarrow & & \downarrow \pi \\
(X/G) \times H & \xrightarrow{n} & X/G
\end{array}
$$

It is commutative, $\pi \circ m$ is of class $C^r$ and $\pi \times 1$ is a surjective submersion; it then suffices to apply *Differentiable and Analytic Manifolds*, R, 5.9.5.

Let $G$ be a Lie group, $X$ a manifold of class $C^r$ and $(g, x) \mapsto xg$ a law of right operation of class $C^r$ of $G$ on $X$. Let $\tau(g)x = \rho(x)g = xg$ for $g \in G,\ x \in X$. Then this time

$$(3')$$
$$
\rho(x) = \rho(xg) \circ \gamma(g^{-1}), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \delta(g)
$$
and hence
$$(4')$$
$$
T_g(\rho(x)) = T_e(\rho(xg)) \circ T_g(\gamma(g^{-1}))
$$
$$(5')$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\delta(g)).
$$

On the other hand, if $\eta$ denotes the mapping $(g, x) \mapsto xg$ of $G \times X$ into $X$, formula (6) remains valid. Proposition 9, its Corollary and Proposition 10 remain equally true (with "principal left fibre bundle" replaced by "principal right fibre bundle" in the last).

### 6. HOMOGENEOUS SPACES AND QUOTIENT GROUPS

#### Proposition 11 {#lie-iii-s1-prop-11 .statement}

*Let $X$ be a Lie group and $G$ a Lie subgroup of $X$.*

(i) *There exists on the homogeneous set $X/G$ one and only one analytic manifold structure such that the canonical projection $\pi$ of $X$ onto $X/G$ is a submersion. The law of operation of $X$ on $X/G$ is analytic. For all $x \in X$, the kernel of $T_x(\pi)$ is obtained from $T_e(G)$ by $T_e(\gamma(x))$.*

(ii) *If $G$ is normal in $X$, $X/G$ is a Lie group with its group structure and the manifold structure defined in (i). The mapping $\pi$ is a Lie group morphism.*

By *General Topology*, Chapter III, § 4, no. 1, *Example 1*, $G$ operates properly and freely on $X$ by right translation. Hence the first assertion of (i) follows from

Proposition 10 of no. 5. The second follows from the Remark of no. 5. Since $\pi$ is a submersion, the kernel of $T_x(\pi)$ is the tangent space at $x$ to
$$
\pi^{-1}(\pi(x)) = xG = \gamma(x)(G)
$$
and hence is obtained from $T_e(G)$ by $T_e(\gamma(x))$.

Suppose that $G$ is normal. Let $m$ be the mapping $(x, y) \mapsto xy^{-1}$ of $(X/G) \times (X/G)$ into $X/G$. Then $(m \circ (\pi \times \pi))(x, y) = \pi(xy^{-1})$ for all $x, y$ in $X$. Hence $m \circ (\pi \times \pi)$ is analytic. As $\pi \times \pi$ is a surjective submersion, $m$ is analytic (Differentiable and Analytic Manifolds, R. 5.9.5), whence (ii).

The homogeneous set $X/G$ with the manifold structure defined in (i) is called the quotient (left) Lie homogeneous space of $X$ by $G$. The (right) Lie homogeneous space $G \setminus X$ is defined analogously. When $G$ is normal, the Lie group $X/G$ defined in (ii) is called the quotient Lie group of $X$ by $G$.

#### Proposition 12 {#lie-iii-s1-prop-12 .statement}

Let $X$ be a Lie group and $Y$ a non-empty analytic manifold with a law of analytic left operation of $X$ on $Y$. For all $y \in Y$, let $\varphi(y)$ be the orbital mapping by $y$ and $X_y$ the stabilizer of $y$ in $X$. The following conditions are equivalent:
(i) there exists $y \in Y$ such that $\varphi(y)$ is a surjective submersion;
(i') for all $y \in Y$, $\varphi(y)$ is a surjective submersion;
(ii) there exists $y \in Y$ such that $X_y$ is a Lie subgroup of $X$ and the canonical mapping of $X/X_y$ into $Y$ is a manifold isomorphism;
(ii') for all $y \in Y$, $X_y$ is a Lie subgroup of $X$ and the canonical mapping of $X/X_y$ into $Y$ is a manifold isomorphism;
(iii) the mapping $(x, y) \mapsto (y, xy)$ of $X \times Y$ into $Y \times Y$ is a surjective submersion.

As the canonical mapping of $X$ onto $X/X_y$ is a submersion, the equivalences (i) $\Leftrightarrow$ (ii), (i') $\Leftrightarrow$ (ii') are immediate. (i) $\Leftrightarrow$ (i') by Proposition 9 of no. 5. The equivalence (i') $\Leftrightarrow$ (iii) follows from formula (7) of no. 5.

Under the conditions of Proposition 12, $Y$ is called a (left) Lie homogeneous space of $X$. Right Lie homogeneous spaces of $X$ are defined analogously.

#### Example {#lie-iii-s1-n6-exa-1 .statement}

Let $G$ be a Lie group. We make $G \times G$ operate on $G$ on the left by $(g_1, g_2)x = g_1xg_2^{-1}$. Let $\rho$ be the orbital mapping of $e$. Then the restrictions of $T_{(e, e)}(\rho)$ to $T_{(e, e)}(G \times \{e\}) = T_e(G) \times \{0\}$ and to
$$
T_{(e, e)}(\{e\} \times G) = \{0\} \times T_e(G)
$$
are isomorphisms of these spaces onto $T_e(G)$. Hence $T_{(e, e)}(\rho)$ is surjective and $\operatorname{Ker} T_{(e, e)}(\rho)$ admits for example the topological supplement $T_e(G) \times \{0\}$ in $T_{(e, e)}(G \times G)$. Thus $\rho$ is a submersion at $(e, e)$. Hence $G$ is a left Lie homogeneous space of $G \times G$.

#### Proposition 13 {#lie-iii-s1-prop-13 .statement}

Let $G$ be a Lie group, $H$ a normal Lie subgroup of $G$, $X$ a manifold of class $C^r$ and $(g, x) \mapsto gx$ a law of left operation of class $C^r$ of $G$ on $X$. Suppose that conditions (a) and (b) of Proposition 10 hold.

(i) The law of left operation $(h, x) \mapsto hx$ of $H$ on $X$ satisfies conditions (a) and (b) of Proposition 10 (so that we can consider the quotient manifolds $X/G$ and $X/H$).

(ii) The law of left operation of $G$ on $X$ defines on taking quotients a law of left operation of class $C^r$ of $G/H$ on $X/H$; this law satisfies conditions (a) and (b) of Proposition 10 (so that we can consider the quotient manifold $(X/H)/(G/H)$).

(iii) The canonical mapping of $X$ onto $X/H$ defines on taking quotients a bijection of $X/G$ onto $(X/H)/(G/H)$. This bijection is an isomorphism of manifolds of class $C^r$.

Clearly $H$ operates freely on $X$; it operates properly by *General Topology*, Chapter III, § 4, no. 1, *Example* 1. The orbital mappings of $H$ on $X$ are immersions since the canonical injection of $H$ into $G$ is an immersion. This proves (i).

The law of left operation of $G$ on $X$ obviously defines, on taking quotients, a law of left operation of $G/H$ on $X/H$. This law is of class $C^r$ by *Differentiable and Analytic Manifolds*, R, 5.9.6. Let $g \in G$ and $x \in X$ be such that $(Hg)(Hx) = Hx$; then $H(gx) = Hx$ and hence $gx \in Hx$ and $g \in H$; this proves that $G/H$ operates freely on $X/H$. The mapping $\theta : (g, x) \mapsto (x, gx)$ of $G \times X$ into $X \times X$ is closed; on the other hand, $\theta(Hg \times Hx) = Hx \times H(gx)$; it follows immediately that the mapping

$$(Hg, Hx) \mapsto (Hx, H(gx))$$

of $(G/H) \times (X/H)$ into $(X/H) \times (X/H)$ is closed; as moreover $G/H$ operates freely on $X/H$, Theorem 1 (c) of *General Topology*, Chapter I, § 10, no. 2 proves that $G/H$ operates properly on $X/H$.

Let $\pi$ be the canonical mapping of $X$ onto $X/H$, $\sigma$ the canonical mapping of $G$ onto $G/H$, $x$ an element of $X$ and $y = \pi(x)$.

$$
\begin{array}{ccc}
G & \xrightarrow{\rho(x)} & X \\
\downarrow \sigma & & \downarrow \pi \\
G/H & \xrightarrow{\rho(y)} & X/H
\end{array}
$$

Then $\pi \circ \rho(x) = \rho(y) \circ \sigma$ and hence

$$
T_x(\pi) \circ T_e(\rho(x)) = T_e(\rho(y)) \circ T_e(\sigma).
$$

Let $u \in T_e(G/H)$ be such that $T_e(\rho(y))u = 0$. There exists $v \in T_e(G)$ such that $u = T_e(\sigma)v$. Then $T_x(\pi)(T_e(\rho(x))v) = 0$, hence $T_e(\rho(x))v$ is tangent to $Hx$ (*Differentiable and Analytic Manifolds*, R, 5.10.5) and therefore is of the form $T_e(\rho(x) | H)v'$ for some $v' \in T_e(H)$. As $T_e(\rho(x))$ is injective, it follows that $v = v'$, whence $v \in T_e(H)$ and therefore $u = 0$. Thus $T_e(\rho(y))$ is injective. The image of $T_e(\rho(y))$ is equal to that of $T_x(\pi) \circ T_e(\rho(x))$; now the image of $T_e(\rho(x))$ admits a topological supplement in $T_x(X)$ and contains the kernel of $T_x(\pi)$. It is therefore seen that $\rho(y)$ is an immersion, which completes the proof of (ii).

Assertion (iii) follows from the above and Differentiable and Analytic Manifolds, R, 5.9.7.

#### Corollary {#lie-iii-s1-n6-cor-1 .statement}

Let G be a Lie group and H and L normal Lie subgroups of G with L ⊂ H. Then H/L is a normal Lie subgroup of G/L and the canonical bijection of G/H onto (G/L)/(H/L) is a Lie group isomorphism.

### 7. ORBITS

#### Proposition 14 {#lie-iii-s1-prop-14 .statement}

Let G be a Lie group, X an analytic manifold and (g, x) ↦ gx a law of analytic left operation of G on X. Let x ∈ X. Suppose that the corresponding orbital mapping ρ(x) is a subimmersion (which is always the case if K is of characteristic 0 and X is finite-dimensional (Corollary to Proposition 9)). Let G_x be the stabilizer of x in G.
(i) G_x is a Lie subgroup and T_e(G_x) = Ker T_e(ρ(x)).
(ii) The canonical mapping i_x of the homogeneous space G/G_x into X is an immersion with image Gx.
(iii) If further the orbit Gx is locally closed and the topology on G admits a countable base, then Gx is a submanifold of X, i_x is an isomorphism of the manifold G/G_x onto the manifold Gx and T_x(Gx) = Im T_e(ρ(x)).

The inverse image of x under ρ(x) is G_x. As ρ(x) is a subimmersion, G_x is a submanifold and, for all g ∈ G, the tangent space J to gG_x = ρ_{(x)}^{-1}(gx) at g is Ker T_g(ρ(x)) (Differentiable and Analytic Manifolds, R, 5.10.5), whence (i). Let π: G → G/G_x be the canonical mapping. Then i_x ∘ π = ρ(x). As G/G_x is a quotient manifold of G, this equality proves that i_x is analytic. Further, the kernels of T_g(ρ(x)) and T_g(π) are both equal to J. Hence T_{π(g)}(i_x) is injective. The image of T_{π(g)}(i_x) is equal to the image of T_g(ρ(x)) and hence admits a topological supplement. This proves (ii).

Suppose that Gx is locally closed. Every point of Gx then has a neighbourhood in Gx which is homeomorphic to a closed subspace of a complete metric space and hence is a Baire space. Hence Gx is a Baire space (General Topology, Chapter IX, § 5, Proposition 4). If G has a countable base, i_x is therefore a homeomorphism of G/G_x onto Gx (General Topology, Chapter IX, § 5). Then by (ii) and Differentiable and Analytic Manifolds, R, 5.8.3, i_x is an isomorphism of the manifolds G/G_x onto the manifold Gx and

$$
T_x(Gx) = \operatorname{Im} T_{π(e)}(i_x) = \operatorname{Im} T_e(ρ(x)).
$$

#### Remark {#lie-iii-s1-n7-rem-1 .statement}

Let G be a finite-dimensional Lie group, X a manifold of class C^r and (g, x) ↦ gx a law of left operation of class C^r of G on X. Then Proposition 14 remains valid. The only point which needs a different proof is the fact that G_x is a Lie subgroup. But if r ≠ ω, K = \mathbf{R}; as clearly G_x is closed, G_x is a Lie subgroup by § 8, Theorem 2.

#### Corollary {#lie-iii-s1-n7-cor-1 .statement}

Let G be a Lie group whose topology admits a countable base and X a non-empty finite-dimensional analytic manifold with a law of analytic left operation of G on X. Suppose that G operates transitivity on X and that K is of characteristic 0. Then X is a Lie homogeneous space for G.

Let x ∈ X. The orbit of x, equal to X, is closed and we can therefore apply Proposition 14 (iii).

### 8. VECTOR BUNDLES WITH OPERATORS

Let G be a Lie group, X a manifold of class C^r and (g, x) ↦ gx a law of left operation of class C^r of G on X. Let E be a vector bundle of class C^r, with base space X and π : E → X the projection of E onto X. For all x ∈ X, let E_x be the fibre of E at x. Let (g, u) ↦ gu be a law of left operation of G on E such that π is compatible with the operations of G on X and on E. For all g ∈ G and all x ∈ X, the restriction to E_x of the mapping u ↦ gu is a bijection ψ_{g, x} of E_x onto E_{gx}. We shall assume that, for all g ∈ G and all x ∈ X, ψ_{g, x} is continuous and linear and hence is an isomorphism of the normable space E_x onto the normable space E_{gx}.

Let φ be the automorphism (g, x) ↦ (g, gx) of the manifold G × X. Let p be the canonical projection of G × X onto X and E' the inverse image of E under p. Let ψ : E' → E' be the mapping the sum of the ψ_{g, x} : E'_{(g, x)} → E'_{(g, gx)}.

#### Definition 4 {#lie-iii-s1-def-4 .statement}

If ψ is a φ-morphism of vector bundles of class C^r, E is called a vector G-bundle of class C^r.

In other words, E is a vector G-bundle of class C^r if for all (g_0, x_0) ∈ G × X the following condition holds: there exists an open neighbourhood U of (g_0, x_0) in G × X such that, if E' | U (resp. E' | φ(U)) is identified with a trivial vector bundle of fibre M (resp. N) by means of a vector chart, the mapping (g, x) ↦ ψ_{g, x} of U into L(M, N) is of class C^r.

The mapping ψ is obviously bijective and it follows from the above local criterion that ψ^{-1} is a φ^{-1}-morphism of vector bundles so that ψ is a φ-isomorphism of vector bundles.

A trivial vector G-bundle of base X is a vector bundle X × F (where F is a complete normable space) with the law of operation (g, (x, f)) ↦ (gx, f) of G on X × F.

We again assume the hypotheses and notation preceding Definition 4 and further take τ to be a vector functor of class C^r for isomorphisms (Differentiable and Analytic Manifolds, R, 7.6.6). Then τE is a vector bundle with base space X. For all x ∈ X, its fibre (τE)_x is equal to τ(E_x). For all normable spaces N_1, N_2, let Isom(N_1, N_2) denote the set of isomorphisms of N_1 onto N_2. If g ∈ G, then

$$
\tau(\psi_{g, x}) \in \mathrm{Isom}((\tau E)_x, (\tau E)_{gx}).
$$

The τ(ψ_{g, x}) define a law of left operation (g, u) ↦ gu of G on τE and the canonical projection of τE onto X is compatible with the operations of G on X and τE.

#### Proposition 15 {#lie-iii-s1-prop-15 .statement}

*If E is a vector G-bundle of class C^r, τE is a vector G-bundle of class C^r*.

Let g_0, x_0, U, M, N be as in the paragraph following Definition 4. Then the mapping (g, x) ↦ τ(ψ_{g,x}) of U into $\mathcal{L}(\tau M, \tau N)$ is the composition of the mapping (g, x) ↦ ψ_{g,x} of U into $\mathcal{L}(M, N)$ and the mapping f ↦ τ(f) of Isom(M, N) into Isom(τM, τN); these two mappings are of class C^r and hence so is their composition, whence the proposition.

#### Proposition 16 {#lie-iii-s1-prop-16 .statement}

*Let G be a Lie group, X a manifold of class C^r (r ≥ 2) and (g, x) ↦ gx a law of left operation of class C^r of G on X, whence, by transporting the structure, there is a law of left operation of G on TX. Under this law, TX is a vector G-bundle of class C^{r-1}.*

Let pr_1 (resp. pr_2) be the canonical projection of G × X onto G (resp. X) and let E_1 (resp. E_2) be the inverse image of TG (resp. TX) relative to pr_1 (resp. pr_2). Then the vector bundle T(G × X) is the direct sum of E_1 and E_2. Let i: E_2 → T(G × X) and q: T(G × X) → E_2 be the canonical vector bundle morphisms defined by this decomposition into a direct sum. Let φ be the mapping (g, x) ↦ (g, gx) of G × X into G × X. Then the mapping denoted by ψ in Definition 4 (where we put E = TX) is just q ∘ T(φ) ∘ i. But T(φ) is a φ-morphism of vector bundles of class C^{r-1} (*Differentiable and Analytic Manifolds*, R, 8.1.2).

#### Corollary {#lie-iii-s1-n8-cor-1 .statement}

*If τ is a vector functor of class C^r for isomorphisms, τ(TX) is a vector G-bundle of class C^{r-1}.*

This follows from Propositions 15 and 16.

#### Remark 1 {#lie-iii-s1-n8-rem-1 .statement}

If τ is a vector functor of class C^r for isomorphisms *in finite dimension* and E is of finite rank, τE is defined similarly and Proposition 15 remains valid; the Corollary to Proposition 16 remains valid provided X is finite-dimensional.

#### Example {#lie-iii-s1-n8-exa-1 .statement}

With the hypotheses and notation of Proposition 16, let F be a complete normable space. Then $\mathcal{L}((TX)^p; F)$ is a vector G-bundle of class C^{r-1}; so is Alt^p(TX; F) if K is of characteristic zero or X is finite-dimensional (*Differentiable and Analytic Manifolds*, R, 7.7, 7.8). If X is finite-dimensional, $\bigotimes^p (TX) \otimes \bigotimes^q (TX)^*$ is a vector G-bundle of class C^{r-1}.

#### Proposition 17 {#lie-iii-s1-prop-17 .statement}

*Let G be a Lie group, X a left Lie homogeneous space of G, x_0 a point of X, G_0 the stabilizer of x_0 in G, E and E' left vector G-bundles of class C^r and base space X, E_0 (resp. E'_0) the fibre of E (resp. E') at x_0 and f an element of $\mathcal{L}(E_0, E'_0)$ such that f(gu) = gf(u) for all u ∈ E_0 and g ∈ G_0. Then there exists one and only one morphism of E into E' compatible with the operations of G and extending f.*

The uniqueness of this morphism is obvious. We prove its existence. Let g, g' elements of G and u ∈ E_0 be such that gu = g'u. Then g'^{-1}g ∈ G_0 and g'^{-1}gu = u and hence g'^{-1}gf(u) = f(u), that is gf(u) = g'f(u). Hence a mapping φ is defined of E into E' by writing φ(gu) = gf(u). Clearly this mapping extends f and it is compatible with the operations of G. We show that φ is a vector bundle morphism of class C^r. Let x_1 ∈ X. There exists an open neighbourhood V of x_1 in X and a submanifold W of G such that the mapping g ↦ gx_0 is an isomorphism θ of class C^r of W onto V. By shrinking V and W it can be assumed that:
(1) E | V (resp. E' | V) is identified with a trivial vector bundle of fibre M (resp. M');
(2) if ψ_g (resp. ψ'_g) denotes the mapping u ↦ gu of E_0 (resp. E'_0) into E_{gx_0} (resp. E'_{gx_0}), then the mappings g ↦ ψ_g and g ↦ ψ_g^{-1} (resp. g ↦ ψ'_g and g ↦ ψ'_g^{-1}) of W into 𝓛(E_0, M) and 𝓛(M, E_0) (resp. 𝓛(E'_0, M') and 𝓛(M', E'_0)) are of class C^r.

For x ∈ V, let φ_x : M → N be the restriction of φ to E_x = M. Then φ_x is obtained by composing the following mappings:
(1) the mapping (ψ_θ^{-1,x})^{-1} of M into E_0;
(2) the mapping f of E_0 into E_0;
(3) the mapping ψ'_θ^{-1,x} of E_0 into M'.
Hence we see that the mapping x ↦ φ_x of V into 𝓛(M, M') is of class C^r.

#### Corollary 1 {#lie-iii-s1-prop-17-cor-1 .statement}

Let E_0^{G_0} be the set of elements of E_0 which are invariant under G_0. For all u ∈ E_0^{G_0}, let σ_u be the mapping of X into E defined by σ_u(gx_0) = gu for all g ∈ G.
(i) The G-invariant sections† of E are of class C^r.
(ii) u ↦ σ_u is a bijection of E_0^{G_0} onto the set of G-invariant sections of E.

Assertion (ii) is obvious. To prove (i) it is sufficient to prove that each section σ_u is of class C^r. Let E' be the trivial G-bundle of base X and fibre E_0^{G_0}. Let f be the canonical injection of E_0^{G_0} into E_0. By Proposition 17 there exists a morphism φ of E' into E compatible with the operations of G and extending f. If u ∈ E_0^{G_0} and g ∈ G, then

$$
σ_u(gx_0) = gu = gf(u) = φ(gu) = φ((u, gx_0))
$$

and hence σ_u(x) = φ((u, x)) for all x ∈ X, which proves our assertion.

*For example, let G be a finite-dimensional real Lie group, G_0 a compact Lie subgroup of G and X the homogeneous space G/G_0. Let x_0 denote the canonical image of e in X. There exists a positive definite symmetric bilinear form on T_{x_0}(X) invariant under G_0 (Integration, Chapter VII, § 3, Proposition 1). Applying the above to (TX)* ⊗ (TX)*, we see that there exists on X an analytic Riemannian metric invariant under G_*.

† By a section of E we here mean a mapping σ (not necessarily of class C^r) of X into E such that p ∘ σ = Id_X, where p denotes the projection of E onto X.

#### Corollary 2 {#lie-iii-s1-prop-17-cor-2 .statement}

Suppose that $G_0$ operates trivially on $E_0$. Let $E'$ be the trivial $G$-bundle with base space $X$ and fibre $E_0$. There exists one and only one isomorphism of $E$ onto $E'$ compatible with the operations of $G$ and extending $\mathrm{Id}_{E_0}$.

This follows immediately from Proposition 17.

#### Remark 2 {#lie-iii-s1-n8-rem-2 .statement}

In this no., the laws of left operation can be replaced throughout by laws of right operation.

### 9. LOCAL DEFINITION OF A LIE GROUP

#### Proposition 18 {#lie-iii-s1-prop-18 .statement}

Let $G$ be a group and $U$ and $V$ two subsets of $G$ containing $e$. Suppose that $U$ has an analytic manifold structure satisfying the following conditions:
(i) $V = V^{-1}, V^2 \subset U, V$ is open in $U$;
(ii) the mapping $(x, y) \mapsto xy^{-1}$ of $V \times V$ into $U$ is analytic;
(iii) for all $g \in G$, there exists an open neighbourhood $V'$ of $e$ in $V$ such that $gV'g^{-1} \subset U$ and such that the mapping $x \mapsto gxg^{-1}$ of $V'$ into $U$ is analytic.

Then there exists one and only one analytic manifold structure on $G$ with the following properties:
(α) $G$ with this structure is a Lie group;
(β) $V$ is open in $G$;
(γ) the manifold structures on $G$ and $U$ induce the same structure on $V$.

(a) Let $A$ be an open subset of $V$ and $v_0$ an element of $V$ such that $v_0A \subset V$. Then $v_0A$ is the set of $v \in V$ such that $v_0^{-1}v \in A$ and hence is an open subset of $V$ (taking account of (ii)). Moreover, (ii) implies that the mappings $v \mapsto v_0v$ of $A$ onto $v_0A$ and $v \mapsto v_0^{-1}v$ of $v_0A$ onto $A$ are inverse analytic bijections and hence analytic isomorphisms.

(b) We choose an open neighbourhood $W$ of $e$ in $V$ such that $W = W^{-1}$, $W^3 \subset V$ and there exists a chart $(W, \phi, E)$ of the manifold $U$ with domain $W$. For all $g \in G$, let $\phi_g$ be the mapping $h \mapsto \phi(g^{-1}h)$ of $gW$ into $E$. We show that the charts $\phi_g$ of $G$ are analytically compatible. Let $g_1, g_2$ be elements of $G$ such that $g_1W \cap g_2W \neq \emptyset$, so that $g_2^{-1}g_1$ and $g_1^{-1}g_2$ belong to $W^2$. By (a), $W \cap g_1^{-1}g_2W$ is an open subset of $W$ and hence
$$
\phi_{g_1}(g_1W \cap g_2W) = \phi(W \cap g_1^{-1}g_2W)
$$
is an open subset $D$ of $E$. For $d \in D$,
$$
(\phi_{g_2} \circ \phi_{g_1}^{-1})(d) = \phi(g_2^{-1}g_1\phi^{-1}(d));
$$
by (a) we see that $\phi_{g_2} \circ \phi_{g_1}^{-1}$ is analytic.

(c) By (b) there exists on $G$ an analytic manifold structure such that $(\phi_g)_{g \in G}$ is an atlas on $G$. For all $g_0 \in G$, the mapping $g \mapsto g_0g$ ($g \in G$) leaves this atlas invariant and hence is an automorphism of $G$ with this manifold structure. In particular condition (GL₁) is satisfied.

(d) Let $v_0 \in V$. By (ii) there exists an open neighbourhood $A$ of $e$ in $W$ such that $v_0A \subset V$. This proves first that $V$ is open in $G$. By (a) the mapping $v \mapsto v_0v$ of $A$ onto $v_0A$ is an analytic isomorphism with the structures induced by U. By (c) we see that the manifold structures on G and U induce the same structure on v_0A and hence finally on V.

(e) by (d), (ii) and (iii), we see that conditions (GL_2) and (GL_3) hold. Hence G is a Lie group.

(f) If a manifold structure on G is compatible with the group structure of G and is such that V is an open submanifold of G, then (\phi_g)_{g\in G} is an atlas on G. Hence the uniqueness assertion of the proposition.

#### Proposition 19 {#lie-iii-s1-prop-19 .statement}

Let G be a topological group, H a Lie group and f a homomorphism of the group G into the group H. Suppose that there exist an open neighbourhood of e_G in G, a chart (V, \phi, E) of the manifold H at e_H and a closed vector subspace F of E admitting a topological supplement, such that f(U) \subset V and \phi \circ f)|U is a homeomorphism of U onto \phi(V) \cap F. Then there exists a unique manifold structure on G such that f is an immersion; this structure is the inverse image under f of the manifold structure on H. With this structure G is a Lie group.

As translations of G (resp. H) are homeomorphisms (resp. analytic isomorphisms), f satisfies condition (R) of Differentiable and Analytic Manifolds, R, 5.8.1. The first two assertions of the proposition then follow from Differentiable and Analytic Manifolds, R, loc. cit. Consider the commutative diagram

$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
f \times f \downarrow & & \downarrow f \\
H \times H & \xrightarrow{n} & H
\end{array}
$$

where m(x, y) = xy^{-1} (resp. n(x, y) = xy^{-1}) for x, y in G (resp. H). Then n \circ (f \times f) is analytic, hence f \circ m is analytic and hence m is analytic since f is an immersion. Therefore G is a Lie group.

The Lie group structure on G is called the inverse image of the Lie group structure on H under f.

#### Corollary {#lie-iii-s1-n9-cor-1 .statement}

Let G be a topological group, N a discrete normal subgroup of G and \pi the canonical mapping of G onto G/N. Suppose that an analytic manifold structure is given on G/N, compatible with the topological group structure on G/N. Then there exists a unique manifold structure on G such that \pi is an immersion; this structure is the inverse image under \pi of the manifold structure on G/N. With this structure, \pi is étale, G is a Lie group and G/N is the quotient Lie group of G by N.

#### Remark {#lie-iii-s1-n9-rem-1 .statement}

Let H be a connected real or complex Lie group, \tilde{H} its universal covering† and \pi the canonical mapping of \tilde{H} onto H. When we speak of \tilde{H}

† Cf. General Topology, Chapter XI; whilst awaiting the publication of this chapter, see for example L. S. Pontrjagin, Topological groups, 2nd edition translated from Russian, Gordon and Breach, 1966; or G. Hochschild, The structure of Lie groups, Holden-Day, 1965.

LIE GROUPS

as a Lie group, we shall always mean with the inverse image structure of that on H under $\pi$.

### 10. GROUP GERMS

#### Definition 5 {#lie-iii-s1-def-5 .statement}

*A Lie group germ over K* is a system $(G, e, \theta, m)$ satisfying the following conditions:
(i) $G$ is an analytic manifold over $K$;
(ii) $e \in G$;
(iii) $\theta$ is an analytic mapping of $G$ into $G$;
(iv) $m$ is an analytic mapping of an open subset $\Omega$ of $G \times G$ into $G$;
(v) for all $g \in G$, $(e, g) \in \Omega$, $(g, e) \in \Omega$, $m(e, g) = m(g, e) = g$;
(vi) for all $g \in G$, $(g, \theta(g)) \in \Omega$, $(\theta(g), g) \in \Omega$, $m(g, \theta(g)) = m(\theta(g), g) = e$;
(vii) if $g, h, k$ are elements of $G$ such that $(g, h) \in \Omega$, $(h, k) \in \Omega$, $(m(g, h), k) \in \Omega$, $(g, m(h, k)) \in \Omega$, then $m(m(g, h), k) = m(g, m(h, k))$.

$e$ is called the identity element of the group germ. We often write $gh$ instead of $m(g, h)$ and (by an abuse of notation) $g^{-1}$ instead of $\theta(g)$.

A Lie group $G$ is a Lie group germ with the obvious choice of $e, \theta, m$.

Let $G$ be a Lie group germ. Then $ee^{-1} = e$, that is

$$
e^{-1} = e.
$$

For all $g \in G$,

$$
g = eg = ((g^{-1})^{-1}g^{-1})g = (g^{-1})^{-1}(g^{-1}g) = (g^{-1})^{-1}e,
$$

that is

$$
(g^{-1})^{-1} = g.
$$

A subset of $G$ invariant under the mapping $g \mapsto g^{-1}$ is called symmetric.

The manifold $G$, with the point $e$, the mapping $g \mapsto g^{-1}$ and the mapping $(g, h) \mapsto hg$ is a Lie Group germ $G^\vee$ called the opposite of $G$.

The Lie group germ $G$ is called commutative if, for all $(g, h) \in G \times G$ such that $gh$ is defined, $hg$ is defined and equal to $gh$.

Let $G$ be a Lie group germ. The set of $(g, h) \in G \times G$ such that $gh$ is defined is a neighbourhood of $(e, e)$. On the other hand, the mappings $(g, h) \mapsto gh$ and $g \mapsto g^{-1}$ are continuous. Hence $(gh)k = g(hk)$ for $g, h, k$ sufficiently close to $e$. Similarly, $(h^{-1}g^{-1})(gh) = h^{-1}(eh) = h^{-1}h = e$ for $g, h$ sufficiently close to $e$, whence multiplying on the right by $(gh)^{-1}$,

$$
(gh)^{-1} = h^{-1}g^{-1} \quad \text{for } g, h \text{ sufficiently close to } e.
$$

#### Proposition 20 {#lie-iii-s1-prop-20 .statement}

*Let $G$ be a Lie group germ and $g \in G$. There exist an open neighbourhood $U$ of $e$ and an open neighbourhood $V$ of $g$ with the following properties:*
(a) $ug$ is defined for all $u \in U$;
(b) $vg^{-1}$ is defined for all $v \in V$;
(c) the mappings $u \mapsto ug,\ v \mapsto vg^{-1}$ are inverse analytic isomorphisms of one another of $U$ onto $V$ and of $V$ onto $U$.

§ 1.10

As the set of definition of the product is open in $G \times G$, there exist an open neighbourhood $U$ of $e$ and an open neighbourhood $V$ of $g$ with properties (a) and (b). Let $\eta(u) = ug$ for $u \in U$, $\eta'(v) = vg^{-1}$ for $v \in V$. By shrinking $U$ and $V$, it can be assumed that $(ug)g^{-1} = u$ and $(vg^{-1})g = v$ for $u \in U$ and $v \in V$. Then $\eta$ and $\eta'$ are injections. By shrinking $U$ further, it can be assumed that $\eta(U) \subset V$. Then $\eta'(V) \supset U$ and $\eta(U)$ is the inverse image of $U$ under $\eta'$ and hence is an open neighbourhood of $g$ in $V$. Replacing $V$ by $\eta(U)$, we finally arrive at the situation where $\eta$ and $\eta'$ are analytic inverse bijections.

Let $G_1, G_2$ be two Lie group germs with identity elements $e_1, e_2$. A mapping $f$ of $G_1$ into $G_2$ is called a *morphism* if $f$ satisfies the following conditions:
(i) $f$ is analytic;
(ii) $f(e_1) = e_2$;
(iii) if $g, h$ are elements of $G_1$ such that $gh$ is defined, then $f(g)f(h)$ is defined and is equal to $f(gh)$.

Let $g \in G_1$. As $gg^{-1}$ is defined and is equal to $e_1$, $f(g)f(g^{-1})$ is defined and is equal to $e_2$ and hence
$$
f(g)^{-1} = f(g)^{-1}(f(g)f(g^{-1})) = (f(g)^{-1}f(g))f(g^{-1})
$$
that is
$$
f(g)^{-1} = f(g^{-1}).
$$
(11)

The composition of two morphisms is a morphism.

If $f : G_1 \to G_2$ and $f' : G_2 \to G_1$ are two inverse morphisms of one another, they are isomorphisms (using in particular formula (11)).

Let $G_1, G_2$ be two Lie group germs, and $f$ a mapping of $G_1$ into $G_2$ satisfying conditions (ii) and (iii) above, which is analytic in an open neighbourhood of $e_1$. Using Proposition 20, it can be proved as in Proposition 4 that $f$ is a morphism.

Let $(G, e, \theta, m)$ be a Lie group germ and $\Omega$ the set of definition of $m$. Let $H$ be a submanifold of $G$ containing $e$, which is stable under $\theta$. Suppose that the set $\Omega_1$ of $(x, y) \in \Omega \cap (H \times H)$ such that $m(x, y) \in H$ is open in $H \times H$. Then $(H, e, \theta|H, m|\Omega_1)$ is a Lie group germ. Such a Lie group germ is called a *Lie subgroup germ of G*. The canonical injection of $H$ into $G$ is a morphism. If $f : L \to G$ is a morphism of Lie group germs such that $f(L) \subset H$, then $f : L \to H$ is a morphism of Lie group germs.

Suppose that $K$ is of characteristic 0. If we replace the hypothesis that $H$ is a submanifold of $G$ by the hypothesis that $H$ is a quasi-submanifold of $G$, the results of the above paragraph remain true (cf. *Differentiable and Analytic Manifolds*, R, 5.8.5). $H$ is then called a Lie quasi-subgroup germ of $G$.

If $G$ is a Lie group germ with identity element $e$, every symmetric open neighbourhood of $e$ in $G$ is a Lie subgroup germ of $G$. (This applies in particular when $G$ is a Lie group.) Let $H$ be a Lie subgroup germ of $G$; if $H$ is a neighbourhood of $e$ in $G$, then $H$ is open in $G$ by Proposition 20.

The *product* Lie group germ of a finite number of Lie group germs is defined in an obvious way.

#### Proposition 21 {#lie-iii-s1-prop-21 .statement}

*Let $G, H$ be two Lie group germs and $\phi$ a morphism of $G$ into $H$. The following conditions are equivalent:*

(i) $\phi$ is étale at $e$;
(ii) *there exist open Lie subgroup germs* $G', H'$ *of* $G, H$ *such that* $\phi|G'$ *is an isomorphism of* $G'$ *onto* $H'$.

The implication (ii) $\Rightarrow$ (i) is obvious. Suppose that $\phi$ is étale at $e$. There exists an open Lie subgroup germ $G_1$ of $G$ such that $\phi(G_1)$ is open in $H$ and $\phi|G_1$ is an isomorphism of the manifold $G_1$ onto the manifold $\phi(G_1)$. Then there exists an open Lie subgroup germ $G'$ of $G_1$ such that the product in $G$ of two elements of $G'$ is always defined and belongs to $G_1$. If $g, g'$ are elements of $G'$ such that $gg' \in G'$, then $\phi(g)\phi(g') = \phi(gg') \in \phi(G')$; if $g, g'$ are elements of $G'$ such that $gg' \in G_1 - G'$, then

$$
\phi(g)\phi(g') = \phi(gg') \in \phi(G_1) - \phi(G').
$$

Hence $\phi|G'$ is an isomorphism of the Lie group germ $G'$ onto the open Lie subgroup germ $\phi(G')$ of $H$.

If the conditions of Proposition 21 hold, $G$ and $H$ are called *locally isomorphic*.

#### Proposition 22 {#lie-iii-s1-prop-22 .statement}

*Let $H$ be a Lie group, $U$ a Lie subgroup germ of $H$ and $N$ the set of $g \in H$ such that $U$ and $gUg^{-1}$ have the same germ at $e$ (General Topology, Chapter I, § 6, no. 10). Then $N$ is a subgroup of $H$ containing $U$. There exists one and only one analytic manifold structure on $N$ with the following properties:*

(i) $N$ with this structure is a Lie group;
(ii) $U$ is an open submanifold of $N$;
(iii) *the canonical injection of* $N$ *into* $H$ *is an immersion*.

Clearly $N$ is a subgroup of $H$. If $g \in U$, then $ge \in U$ and $geg^{-1} \in U$, hence $gu \in U$ and $gug^{-1} \in U$ for $u$ sufficiently close to $e$ in $U$ and hence the germ of $gUg^{-1}$ at $e$ is contained in that of $U$; exchanging $g$ and $g^{-1}$, we see that the germs of $gUg^{-1}$ and $U$ at $e$ are equal. Hence $U \subset N$.

Let $V$ be an open neighbourhood of $e$ in $U$ such that $V = V^{-1}, V^2 \subset U$. Conditions (i), (ii), (iii) of Proposition 18 of no. 9 (where $G$ is replaced by $N$) are satisfied. Hence there exists an analytic manifold structure on $N$ with the following properties: ($\alpha$) $N$ with this structure is a Lie group; ($\beta$) $V$ is open in $N$; ($\gamma$) the manifold structures on $N$ and $U$ induce the same structure on $V$. Since $V$ is a submanifold of $H$, the canonical injection of $N$ into $H$ is an immersion at $e$ and hence at every point of $N$. Let $u \in U$. There exists an open neighbourhood V' of e in V such that the mapping $v \mapsto uv$ is an analytic isomorphism of V' onto an open neighbourhood of u in U (Proposition 20) and at the same time onto an open neighbourhood of u in N. Hence U is open in N and the identity mapping of U is an isomorphism with the given manifold structure on U and the open submanifold structure on N; in other words, U is an open submanifold of N.

Finally, we consider an analytic manifold structure on N with properties (i) and (ii) of the proposition and let N* be the Lie group thus obtained. Then the identity mapping of N into N* is étale at e and hence a Lie group isomorphism. This proves the uniqueness assertion of the proposition.

Let H be a Lie group, U a Lie quasi-subgroup germ of H and N the set of $g \in H$ such that U and $gUg^{-1}$ have the same germ at e. If K is of characteristic 0, there exists on G one and only one manifold structure with properties (i) and (ii) of Proposition 22. The proof is the same as for Proposition 22.

#### Corollary {#lie-iii-s1-n10-cor-1 .statement}

Preserving the notation of Proposition 22, let G be the subgroup of H generated by U. Then G is an open subgroup of N. There exists one and only one Lie group structure on G such that U is an open submanifold of G and the canonical injection of G into H is an immersion.

#### Remark {#lie-iii-s1-n10-rem-1 .statement}

Preserving the notation of Proposition 22 and its corollary, suppose that K is of characteristic 0, that H is finite-dimensional and that the topology on U admits a countable base. Even with all these hypotheses it is possible that G is not closed in H (Exercise 3). But, if G is closed, G is a Lie subgroup of H. For the mapping $(g, h) \mapsto gh$ is a law of analytic left operation of G on H. The orbit of e is G. Our assertion then follows from Propositions 2 (iv) and 14 (iii).

### 11. LAW CHUNKS OF OPERATION

Let $(G, e, \theta, m)$ be a Lie group germ and X a manifold of class $C^r$.

#### Definition 6 {#lie-iii-s1-def-6 .statement}

A law chunk of left operation of class $C^r$ of G on X is a mapping $\psi$ defined on an open subset $\Omega$ of $G \times X$ containing $\{e\} \times X$, with values in X and with the following properties:
(i) $\psi$ is of class $C^r$;
(ii) for all $x \in X$, $\psi(e, x) = x$;
(iii) there exists a neighbourhood $\Omega_1$ of $\{e\} \times \{e\} \times X$ in $G \times G \times X$ such that, for $(g, g', x) \in \Omega_1$, the elements of $m(g, g')$, $\psi(m(g, g'), x)$, $\psi(g, \psi(g', x))$ are defined and $\psi(g, \psi(g', x)) = \psi(m(g, g'), x)$.

Law chunks of right operation of class $C^r$ are defined similarly.
We often write $gx$ instead of $\psi(g, x)$.
Let G' be a Lie subgroup germ of G and X' a submanifold of X. Suppose that the set $\Omega'$ of $(g, x) \in \Omega \cap (G' \times X')$ such that $\psi(g, x) \in X'$ is open in $G' \times X'$ (a condition which is always fulfilled if $X'$ is open in $X$). Then $\psi|_{\Omega'}$ is a law chunk of left operation of class $C^r$ of $G'$ on $X'$, which is said to be derived from $\psi$ by restriction to $G'$ and $X'$.

#### Proposition 23 {#lie-iii-s1-prop-23 .statement}

*Let $(G, e, \theta, m)$ be a Lie group germ, $X$ a manifold of class $C^r$, $x_0$ a point of $X$, $\Omega$ an open neighbourhood of $(e, x_0)$ in $G \times X$ and $\psi$ a mapping of $\Omega$ into $X$ with the following properties:
(i) $\psi$ is of class $C^r$;
(ii) $\psi(e, x)$ is equal to $x$ for $x$ sufficiently close to $x_0$;
(iii) $\psi(m(g, g'), x) = \psi(g, \psi(g', x))$ for $(g, g', x)$ sufficiently close to $(e, e, x_0)$.
Then there exist an open neighbourhood $X'$ of $x_0$ in $X$ and an open subset $\Omega'$ of $\Omega \cap (G \times X')$ such that $\psi|_{\Omega'}$ is a law chunk of left operation of class $C^r$ of $G$ on $X'$.
There exist an open neighbourhood $X'$ of $x_0$ in $X$ and an open neighbourhood $G'$ of $e$ in $G$ such that $\psi(e, x) = x$ for all $x \in X$, and
$$
\psi(g, \psi(g', x)) = \psi(m(g, g'), x)
$$
for $(g, g', x) \in G' \times G' \times X'$. Let $\Omega'$ be the set of $(g, x) \in \Omega \cap (G' \times X')$ such that $\psi(g, x) \in X'$. Then $\Omega'$ is open in $G \times X'$ and $X'$, $\Omega'$ have the properties of the proposition.*

#### Lemma 3 {#lie-iii-s1-lem-3 .statement}

*Let $X$ be a normal space and $(X_i)_{i \in I}$ a locally finite open covering of $X$. For all $(i, j) \in I \times I$ and all $x \in X_i \cap X_j$, let $V_{ij}(x)$ be a neighbourhood of $x$ contained in $X_i \cap X_j$. Then we can associate with every $x \in X$ a neighbourhood $V(x)$ of $x$ such that the following conditions are fulfilled:
(a) the relation $x \in X_i \cap X_j$ implies $V(x) \subset V_{ij}(x)$;
(b) if $V(x)$ and $V(y)$ meet, there exists $i \in I$ such that $V(x) \cup V(y) \subset X_i$.
There exists an open covering $(X'_i)_{i \in I}$ of $X$ such that $\overline{X'_i} \subset X_i$ for all $i \in I$ (General Topology, Chapter IX, § 4, Theorem 3). Let $x \in X$. Let $V_1(x)$ be the intersection of the $V_{ij}(x)$ and the $X'_k$ which contain $x$; this is an open neighbourhood of $x$. Let $V_2(x)$ be a neighbourhood of $x$ contained in $V_1(x)$ and meeting only a finite number of $X_i$. Then $V_2(x)$ meets only a finite number of $\overline{X'_i}$ and hence the set
$$
V(x) = V_2(x) \cap \bigcap_{i \in I, x \notin \overline{X'_i}} (X - \overline{X'_i})
$$
is a neighbourhood of $x$. If $x \in X_i \cap X_j$, then $V_1(x) \subset X_i \cap X_j$ and hence $V(x) \subset X_i \cap X_j$. Let $x, y$ be in $X$ and suppose that $V(x)$ and $V(y)$ meet. There exists $i \in I$ such that $x \in X'_i$. Then $V_1(x) \subset X'_i$, hence $V(x) \subset X'_i$ and hence $V(y) \cap \overline{X'_i} \neq \emptyset$. Then $y \in \overline{X'_i}$ by definition of $V(y)$, whence $y \in X_i$ and $V(y) \subset X_i$. Thus $X_i$ contains $V(x)$ and $V(y)$.*

§ 2.1

#### Proposition 24 {#lie-iii-s1-prop-24 .statement}

Let G be a Lie group germ, X a manifold of class C^r and (X_i)_{i \in I} a locally finite open covering of X. For all i \in I, let $\psi_i$ be a law chunk of left operation of class C^r of G on X_i. Suppose that the underlying topological space of X is normal and that, for all (i, j) \in I \times I and all x \in X_i \cap X_j, $\psi_i$ and $\psi_j$ coincide on a neighbourhood of (e, x). There exists a law chunk $\psi$ of left operation of class C^r of G on X such that, for all i \in I and all x \in X_i, $\psi_i$ and $\psi$ coincide on a neighbourhood of (e, x).

For all (i, j) \in I \times I and all x \in X_i \cap X_j, choose an open neighbourhood V_{ij}(x) of x in X_i \cap X_j such that $\psi_i$ and $\psi_j$ are defined and equal on a neighbourhood of {e} \times V_{ij}(x) in G \times X. For all x \in X choose an open neighbourhood V(x) of x in X such that conditions (a) and (b) of Lemma 3 are fulfilled. Let I_x be the set of i \in I such that x \in X_i. This is a finite set. Let U_x be the set of (g, y) \in G \times V(x) such that the $\psi_i$ for i \in I_x are defined and coincide on a neighbourhood of (g, y). Then U_x is open and (e, x) \in U_x. The $\psi_i$ for i \in I_x all have the same restriction to U_x. Let x, y be in X. If U_x and U_y meet, V(x) and V(y) meet and hence there exists i \in I such that

$$
V(x) \cup V(y) \subset X_i.
$$

Then i \in I_x, i \in I_y, $\psi_i|U_x = \psi_x, \psi_i|U_y = \psi_y$ and hence

$$
\psi_x|(U_x \cap U_y) = \psi_y|(U_x \cap U_y).
$$

The $\psi_x$ therefore define a mapping $\psi$ of $U = \bigcup_{x \in X} U_x$ into X and U is an open neighbourhood of {e} \times X in G \times X. Clearly $\psi$ is of class C^r and $\psi(e, x) = x$ for all x \in X. For all i \in I and all x \in X_i, $\psi$ coincides with $\psi_x$ and hence with $\psi_i$ in a neighbourhood of (e, x) and hence $\psi$ satisfies condition (iii) of Definition 6.

### Exercises {#lie-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
