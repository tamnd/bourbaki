---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 2
section_title: Group of tangent vectors to a Lie group
lang: en
source: lie-i-iii
book_pages: 233-238
pdf_pages: 0251-0256
extraction: ocr
subsections:
    - "no": 1
      title: TANGENT LAWS OF COMPOSITION
      page: 233
      pdf_page: 251
    - "no": 2
      title: GROUP OF TANGENT VECTORS TO A LIE GROUP
      page: 235
      pdf_page: 253
    - "no": 3
      title: CASE OF GROUP GERMS
      page: 237
      pdf_page: 255
statements: 10
exercises: 0
content_sha256: 7845b7e2bd4a655ddc90c51d69de092ba1cf892797854eb6ec7e8069c2d39675
---

## § 2. GROUP OF TANGENT VECTORS TO A LIE GROUP

### 1. TANGENT LAWS OF COMPOSITION

Let X and Y be manifolds of class C^r. We know (Differentiable and Analytic Manifolds, R, 8.1.4) that X \times Y is a manifold of class C^r and that the mapping (T(pr_1), T(pr_2)), the product of the tangent mappings to the canonical projections, is an isomorphism of class C^{r-1} of T(X \times Y) onto T(X) \times T(Y).\footnote{For r = 1, this means that (T(pr_1), T(pr_2)) is a homomorphism of T(X \times Y) onto T(X) \times T(Y).} This isomorphism is compatible with the vector bundle structures with base space X \times Y and allows us to identify T(X \times Y) with T(X) \times T(Y). Let a ∈ X, b ∈ Y, u ∈ T_a(X), v ∈ T_b(Y); the above identification allows us to consider (u, v) as an element of T_{(a, b)}(X × Y); then

$$(u, v) = (u, 0) + (0, v)$$

and (u, 0) (resp. (0, v)) is the image of u (resp. v) under the tangent mapping to the immersion x ↦ (x, b) (resp. y ↦ (a, y)) of X (resp. Y) into X × Y. When it is necessary to be precise, we shall write 0_a for the zero element of T_a(x).

Now let X, Y, Z be manifolds of class C^r and f a mapping of class C^r of X × Y into Z. The tangent mapping is, using the above identification, a mapping of class C^{r-1} of T(X) × T(Y) into T(Z). For u ∈ T_a(X) and v ∈ T_b(Y),

(1)
$$T(f)(u, v) = T(f)(u, 0_b) + T(f)(0_a, v),$$
(2)
$$T(f)(0_a, 0_b) = 0_{f(a, b)}.$$

On the other hand, the mapping y ↦ f(a, y) is the composition of the immersion y ↦ (a, y) and f; it follows that

(3) $T(f)(0, v)$ is the image of v under the tangent mapping to $y ↦ f(a, y)$.

Similarly

(4) $T(f)(u, 0)$ is the image of u under the tangent mapping to $x ↦ f(x, b)$.

If the mapping f of X × Y into Z is denoted by (x, y) ↦ xy, uv is often used to denote the element T(f)(u, v) for u ∈ T(X), v ∈ T(Y).

Let X be a manifold of class C^r and m: X × X → X a law of composition of class C^r on X. Then T(m) is a law of composition of class C^{r-1} on T(X). It is called the law of composition tangent to m. The canonical projection p of T(X) onto X is compatible with the laws m and T(m); in other words,

(5)
$$p \circ T(m) = m \circ (p \times p).$$

It follows from (2) that

(6)
$$T(m)(0_x, 0_y) = 0_{m(x, y)}$$

for all x, y in X; in other words, the zero section $x ↦ 0_x$ of T(X) is compatible with the laws m and T(m).

#### Proposition 1 {#lie-iii-s2-prop-1 .statement}

*Let X be a manifold of class C^r and m a law of composition of class C^r on X. If m is associative (resp. commutative), then T(m) is associative (resp. commutative).*

If m is associative, then $m \circ (m \times \mathrm{Id}_X) = m \circ (\mathrm{Id}_X \times m)$, whence

$$T(m) \circ (T(m) \times \mathrm{Id}_{T(X)}) = T(m) \circ (\mathrm{Id}_{T(X)} \times T(m))$$

and hence $T(m)$ is associative. Let $s$ be the mapping $(x, y) \mapsto (y, x)$ of $X \times X$ into $X \times X$. If $m$ is commutative, then $m \circ s = m$ and hence

$$
T(m) \circ T(s) = T(m).
$$

But $T(s)$ is the mapping $(u, v) \mapsto (v, u)$ of $T(X) \times T(X)$ into $T(X) \times T(X)$. Hence $T(m)$ is commutative.

#### Proposition 2 {#lie-iii-s2-prop-2 .statement}

*Let $X$ be a manifold of class $C^r$, $m$ a law of composition of class $C^r$ on $X$ and $e$ an identity element for $m$.

(i) *The vector $0_e$ is an identity element for $T(m)$.
(ii) *$T_e(X)$ is stable under $T(m)$ and the law of composition induced on $T_e(X)$ by $T(m)$ is the vector space addition on $T_e(X)$.
(iii) *Let $U$ be an open subset of $X$ and $\alpha$ a mapping of class $C^r$ of $U$ into $X$ such that, for all $x \in U$, $\alpha(x)$ is the inverse of $x$ under $m$. Then, for all $u \in T(U)$, $T(\alpha)u$ is the inverse of $u$ under $T(m)$.

Properties (3) and (4) show that $T(m)(0_e, u) = T(m)(u, 0_e) = u$ for all $u \in T(X)$, whence (i). For $u, v$ in $T_e(X)$,

$$
T(m)(u, v) = T(m)(u, 0_e) + T(m)(0_e, v) = u + v,
$$

whence (ii). Finally the relations $m(x, \alpha(x)) = m(\alpha(x), x) = e$ for all $x \in U$ imply

$$
T(m)(u, T(\alpha)(u)) = T(m)(T(\alpha)u, u) = 0_e
$$

for all $u \in T(U)$, whence (iii).

#### Proposition 3 {#lie-iii-s2-prop-3 .statement}

*Let $X_1, X_2, \ldots, X_p, Y$ be manifolds of class $C^r$, $i$ an integer of $\{1, p\}$, $m_i$ (resp. $n$) a law of composition of class $C^r$ on $X_i$ (resp. $Y$) and $u$ a mapping of class $C^r$ of $X_1 \times X_2 \times \cdots \times X_p$ into $Y$. If $u$ is distributive relative to the variable of index $i$, then $T(u)$ is distributive relative to the variable of index $i$.

The proof is analogous to that of Proposition 1.

### 2. GROUP OF TANGENT VECTORS TO A LIE GROUP

#### Proposition 4 {#lie-iii-s2-prop-4 .statement}

*Let $G$ be a Lie group. Then $T(G)$, with the law of composition tangent to the multiplication of $G$, is a Lie group. The identity element of $T(G)$ is the vector $0_e$.

This follows from Propositions 1 and 2.

#### Proposition 5 {#lie-iii-s2-prop-5 .statement}

*Let $G$ and $H$ be Lie groups and $f$ a morphism of $G$ into $H$. Then $T(f)$ is a morphism of the Lie group $T(G)$ into the Lie group $T(H)$.

We know that $T(f')$ is analytic. On the other hand, let $m$ (resp. $n$) denote the multiplication on $G$ (resp. $H$). Then $f \circ m = n \circ (f \times f)$, whence

$$
T(f) \circ T(m) = T(n) \circ (T(f) \times T(f)),
$$

which expresses the fact that $T(f)$ is a group homomorphism.

#### Corollary {#lie-iii-s2-n2-cor-1 .statement}

*Let $G_1, \ldots, G_n$ be Lie groups. The canonical isomorphism of the manifold $T(G_1 \times \cdots \times G_n)$ onto the manifold $T(G_1) \times \cdots \times T(G_n)$ is a Lie group isomorphism.*

$\mathrm{pr}_i$ is a morphism of $G_1 \times \cdots \times G_n$ into $G_i$ and hence $T(\mathrm{pr}_i)$ is a morphism of $T(G_1 \times \cdots \times G_n)$ into $T(G_i)$.

#### Proposition 6 {#lie-iii-s2-prop-6 .statement}

*Let $G$ be a Lie group.*
  (i) *The canonical projection $p : T(G) \to G$ is a Lie group morphism.*
  (ii) *The kernel of $p$ is $T_e(G)$. It is a Lie subgroup of $T(G)$. The Lie group structure induced on $T_e(G)$ by that on $T(G)$ is the Lie group structure of the complete normable space $T_e(G)$.*
  (iii) *The zero section $s$ is an isomorphism of the Lie group $G$ onto a Lie subgroup $s(G)$ of $T(G)$ (which subgroup we identify with $G$).*
  (iv) *The Lie group $T(G)$ is the semi-direct product of $G$ by $T_e(G)$.*

Assertion (i) follows from (5). Assertion (ii) is obvious taking account of Proposition 2 (ii). Assertions (iii) and (iv) follow from (6) and § 1, Proposition 8.

Let $u \in T(G)$ and $g \in G$. By (3) and (4), the products $ug, gu$ calculated in the group $T(G)$ are the images of $u$ under $T(\delta(g^{-1}))$ and $T(\gamma(g))$. It follows from § 1, Corollary 2 to Proposition 17 that the mapping $(g, u) \mapsto gu$ of $G \times T_e(G)$ into $T(G)$ is an isomorphism of the trivial vector bundle $G \times T_e(G)$ with base space $G$ onto the vector bundle $T(G)$. The inverse isomorphism is called the *left trivialization* of $T(G)$. By considering the mapping $(g, u) \mapsto ug$, the *right trivialization* of $T(G)$ is defined similarly.

#### Proposition 7 {#lie-iii-s2-prop-7 .statement}

*Let $G$ be a Lie group, $M$ a manifold of class $C^r$ and $f$ and $g$ mappings of class $C^r$ of $M$ into $G$, so that $fg$ is a mapping of class $C^r$ of $M$ into $G$. Let $m \in M, x = f(m), y = g(m), u \in T_m(M)$. Then*

$$
(T fg)u = T(f)u.y + x.T(g)u.
$$

Let $m$ be the multiplication of $G$. Then $fg = m \circ (f, g)$. Now

$$
T(f, g)(u) = (T(f)u, T(g)u),
$$

hence $T(fg)u = T(f)u.T(g)u$. It then suffices to apply (1) with $f$ replaced by $m$.

#### Corollary {#lie-iii-s2-n2-cor-2 .statement}

*Let $n \in \mathbf{Z}$. The tangent mapping at $e$ to the mapping $g \mapsto g^n$ of $G$ into $G$ is the mapping $x \mapsto nx$ of $T_e(G)$ into $T_e(G)$.*

For $n \geqslant 0$, this follows by induction on $n$ from Proposition 7. On the other hand, the tangent mapping at $e$ to the mapping $g \mapsto g^{-1}$ is the mapping $x \mapsto -x$ (no. 1, Proposition 2).

Let G be a Lie group, X a manifold of class C^r and (g, x) \mapsto gx a law of left operation of class C^r of G on X. Arguing as for Proposition 1, we derive a law of left operation of class C^{r-1} of T(G) on T(X), which we shall also denote by (u, v) \mapsto uv. Identifying G (resp. X) with the image of the zero section of T(G) (resp. T(X)), we see by (6) that the law of left operation of T(G) on T(X) extends the law of left operation of G on X. For all u \in T_g(G) and v \in T_x(X), by (1),

$$
uv = gv + ux.
$$

If g \in G and v \in T_x(X), gv is, by (3), the image of v under the tangent mapping at x to the mapping y \mapsto gy of X into X. This tangent mapping is an isomorphism of T_x(X) onto T_{gx}(X). In particular,

$$
g(v + v') = gv + gv', \quad g(\lambda v) = \lambda(gv) \quad \text{for } v, v' \text{ in } T_x(X), \lambda \in K.
$$

If x \in X and u \in T_g(G), ux is by (4) the image of u under the tangent mapping at g to the mapping h \mapsto hx of G into X. Hence

$$
(u + u')x = ux + u'x, \quad (\lambda u)x = \lambda(ux) \quad \text{for } u, u' \text{ in } T_g(G), \lambda \in K.
$$

The above can be applied to the case of a Lie group operating on itself by left (resp. right) translation. The corresponding law of operation of T(G) on T(G) is defined by left (resp. right) translation of the Lie group T(G). Formulae (7), (8) and (9) are therefore valid in T(G).

#### Proposition 8 {#lie-iii-s2-prop-8 .statement}

Let G_1 and G_2 be Lie groups, X_1 and X_2 manifolds of class C^r and f_i a law of left operation of class C^r of G_i on X_i (i = 1, 2). Let \phi be a morphism of G_1 into G_2 and \psi a \phi-morphism of X_1 into X_2. Then T(\psi) is a T(\phi)-morphism of T(X_1) into T(X_2).

f_2 \circ (\phi \times \psi) = \psi \circ f_1, whence

$$
T(f_2) \circ (T(\phi) \times T(\psi)) = T(\psi) \circ T(f_1).
$$

Let G be a Lie group, X a manifold of class C^r and (g, x) \mapsto gx a law of left operation of class C^r of G on X. Let I be an open subset of K containing 0 and \gamma: I \to G a mapping of class C^r such that \gamma(0) = e. Let

$$
a = T_0(\gamma)1 \in T_e(G).
$$

Let x \in X. Using (4), ax is the image under the tangent mapping to \lambda \mapsto \gamma(\lambda)x of the tangent vector 1 to I at 0. Hence *the vector field* x \mapsto ax on X *is the vector field defined by the mapping* (\lambda, x) \mapsto \gamma(\lambda)x *in the sense of Differentiable and Analytic Manifolds*, R, 8.4.5.

### 3. CASE OF GROUP GERMS

Let (G, e, \theta, m) be a Lie group germ and \Omega the set of definition of m. Then T(\Omega) is identified with an open subset of T(G) \times T(G) and T(m) is an analytic mapping of $T(\Omega)$ into $T(G)$. It can be verified as in no. 2 that $(T(G), 0_e, T(\theta), T(m))$ is a Lie group germ. The products of $G$ and $T(G)$ are often written multiplicatively. The canonical projection of $T(G)$ onto $G$ is a morphism of Lie group germs. The restriction of $T_e(m)$ to $T_e(G)$ is the vector space addition of $T_e(G)$. The zero section of $T(G)$ is an isomorphism of the Lie group germ $G$ onto a Lie subgroup germ of $T(G)$ which we identify with $G$. If $f$ is a morphism of $G$ into a Lie group germ $H$, $T(f): T(G) \to T(H)$ is a morphism of Lie group germs.

The mapping $\phi: (g, u) \mapsto gu$ of $G \times T_e(G)$ into $T(G)$ is an isomorphism of the trivial vector bundle $G \times T_e(G)$ with base space $G$ onto the vector bundle $T(G)$; for $\phi$ and $\phi^{-1}$ are analytic and are vector bundle morphisms, so that it suffices to apply *Differentiable and Analytic Manifolds*, R, 7.2.1. (The proof of no. 2 could also be adapted.) The isomorphism $\phi^{-1}$ is called the left trivialization of $T(G)$. The inverse isomorphism of the mapping $(g, u) \mapsto ug$ is called the right trivialization.

Let $X$ be a manifold of class $C^r$ and $\psi$ a law chunk of left operation of class $C^r$ of $G$ on $X$. Then $T(\psi)$ is a law chunk of left operation of class $C^{r-1}$ of $T(G)$ on $T(X)$ extending $\psi$. Formulae (7), (8) and (9) remain valid if $gx$ is defined. If $I$ is an open subset of $K$ containing 0, if $\gamma: I \to G$ is a mapping of class $C^r$ such that $\gamma(0) = e$ and if $a = T_0(\gamma)1$, the vector field $x \mapsto ax$ defined on $X$ is the vector field defined by the mapping $(\lambda, x) \mapsto \gamma(\lambda)x$ in the sense of *Differentiable and Analytic Manifolds*, R, 8.4.5.
