---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 3
section_title: Passage from a Lie group to its Lie algebra
lang: en
source: lie-i-iii
book_pages: 238-279, 372-376
pdf_pages: 0256-0297, 0390-0394
extraction: ocr
subsections:
    - "no": 1
      title: CONVOLUTION OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 238
      pdf_page: 256
    - "no": 2
      title: FUNCTIORAL PROPERTIES
      page: 241
      pdf_page: 259
    - "no": 3
      title: CASE OF A GROUP OPERATING ON A MANIFOLD
      page: 244
      pdf_page: 262
    - "no": 4
      title: CONVOLUTION OF POINT DISTRIBUTIONS AND FUNCTIONS
      page: 245
      pdf_page: 263
    - "no": 5
      title: FIELDS OF POINT DISTRIBUTIONS DEFINED BY THE ACTION OF A GROUP ON A MANIFOLD
      page: 248
      pdf_page: 266
    - "no": 6
      title: INVARIANT FIELDS OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 249
      pdf_page: 267
    - "no": 7
      title: LIE ALGEBRA OF A LIE GROUP
      page: 251
      pdf_page: 269
    - "no": 8
      title: FUNCTIORIAL PROPERTIES OF THE LIE ALGEBRA
      page: 254
      pdf_page: 272
    - "no": 9
      title: LIE ALGEBRA OF THE GROUP OF INVERTIBLE ELEMENTS OF AN ALGEBRA
      page: 257
      pdf_page: 275
    - "no": 10
      title: LIE ALGEBRAS OF CERTAIN LINEAR GROUPS
      page: 258
      pdf_page: 276
    - "no": 11
      title: LINEAR REPRESENTATIONS
      page: 259
      pdf_page: 277
    - "no": 12
      title: ADJOINT REPRESENTATION
      page: 264
      pdf_page: 282
    - "no": 13
      title: TENSORS AND INVARIANT FORMS
      page: 268
      pdf_page: 286
    - "no": 14
      title: MAURER–CARTAN FORMULAE
      page: 269
      pdf_page: 287
    - "no": 15
      title: CONSTRUCTION OF INVARIANT DIFFERENTIAL FORMS
      page: 271
      pdf_page: 289
    - "no": 16
      title: HAAR MEASURE ON A LIE GROUP
      page: 271
      pdf_page: 289
    - "no": 17
      title: LEFT DIFFERENTIAL
      page: 274
      pdf_page: 292
    - "no": 18
      title: LIE ALGEBRA OF A LIE GROUP GERM
      page: 276
      pdf_page: 294
statements: 111
exercises: 9
content_sha256: 5762aa9c03ccb6cefa82b2dc514fd62774faa93aeda563194756642698c12f55
---

## § 3. PASSAGE FROM A LIE GROUP TO ITS LIE ALGEBRA

### 1. CONVOLUTION OF POINT DISTRIBUTIONS ON A LIE GROUP

#### Definition 1 {#lie-iii-s3-def-1 .statement}

*Let $G$ be a Lie group, $g$ and $g'$ two points of $G$ and let $t \in T_g^{(\infty)}(G)$ $t' \in T_{g'}^{(\infty)}(G)$ be two point distributions at $g$ and $g'$ on $G$ (*Differentiable and Analytic Manifolds*, R, 13.2.1). The convolution product of $t$ and $t'$, denoted by $t * t'$, is the image of $t \otimes t'$ under the mapping $(h, h') \mapsto hh'$ of $G \times G$ into $G$ (*Differentiable and Analytic Manifolds*, R, 13.2.3).*

#### Proposition 1 {#lie-iii-s3-prop-1 .statement}

(i) *If $t \in T_g^{(s)}(G)$ and $t' \in T_{g'}^{(s')}(G)$, then $t * t' \in T_{gg'}^{(s+s')}(G)$.*

(ii) *If $t$ or $t$ has no constant term, $t * t'$ has no constant term.*

(iii) $\varepsilon_g * \varepsilon_{g'} = \varepsilon_{gg'}$.

(iv) *Let $t \in T_g^{(s)}(G)$, $t' \in T_{g'}^{(s')}(G)$ and let $f$ be a function of class $C^{s+s'}$ in an open neighbourhood of $gg'$ with values in a Hausdorff polynormed space. Then*

$$
\langle t * t', f \rangle = \langle t', h' \mapsto \langle t, h \mapsto f(hh') \rangle \rangle \\
= \langle t, h \mapsto \langle t', h' \mapsto f(hh') \rangle \rangle.
$$

This follows from Differentiable and Analytic Manifolds, R, 13.4.1, 13.2.3 and 13.4.4.

Suppose that K = \mathbf{R} or \mathbf{C} and that G is finite-dimensional. Then G is locally compact. If t, t' are point measures, the definition of t \* t' agrees with that of Integration, Chapter VIII, § 1. We shall see later that the convolution product of measures and that of point distributions are two special cases of the convolution product of distributions which are not necessarily point distributions.

Let \mathcal{T}^{(\infty)}(G) be the direct sum of the T_g^{(\infty)}(G) for g \in G (cf. Differentiable and Analytic Manifolds, R, 13.6.1). We define the convolution product in \mathcal{T}^{(\infty)}(G) as the bilinear mapping of \mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G) into \mathcal{T}^{(\infty)}(G) extending the convolution product of Definition 1. We also denote it by *. Thus \mathcal{T}^{(\infty)}(G) has an algebra structure filtered by the \mathcal{T}^{(s)}(G). The subalgebra \mathcal{T}^{(0)}(G) = \bigoplus_{g \in G} T_g^{(0)}(G) is identified with the algebra K^{(G)} of the group G over K.

#### Proposition 2 {#lie-iii-s3-prop-2 .statement}

The algebra \mathcal{T}^{(\infty)}(G) is associative. It is commutative if and only if G is commutative.

Let t \in \mathcal{T}^{(\infty)}(G), t' \in \mathcal{T}^{(\infty)}(G), t'' \in \mathcal{T}^{(\infty)}(G). Then t \* (t' \* t'') is the image of t \otimes t' \otimes t'' under the mapping (g, g', g'') \mapsto g(g'g'') of G \times G \times G into G and (t \* t') \* t'' is the image of t \otimes t' \otimes t'' under the mapping (g, g', g'') \mapsto (gg')g'' of G \times G \times G into G. Hence (t \* t') \* t'' = t \* (t' \* t''). It is seen similarly that, if G is commutative, t \* t' = t' \* t. If the convolution product is commutative, G is commutative by Proposition 1 (iii).

#### Proposition 3 {#lie-iii-s3-prop-3 .statement}

If t \in \mathcal{T}^{(\infty)}(G) and g \in G, then $\gamma(g)_* t = \varepsilon_g * t, \delta(g)_* t = t * \varepsilon_{g^{-1}}$, (Int g)_* t = $\varepsilon_g * t * \varepsilon_{g^{-1}}$. In particular, $\varepsilon_e$ is the unit element of \mathcal{T}^{(\infty)}(G).

Consider the diagram

$$
\begin{array}{ccccc}
G & \xrightarrow{\phi} & G \times G & \xrightarrow{\psi} & G \\
\end{array}
$$

where $\phi$ is the mapping $h \mapsto (g, h)$ and $\psi$ is the mapping $(h', h) \mapsto h'h$. Then $\gamma(g) = \psi \circ \phi$ and hence $\gamma(g)_* t = \psi_*(\phi_*(t))$. But $\phi_*(t) = \varepsilon_g \otimes t$ and hence $\psi_*(\phi_*(t)) = \varepsilon_g * t$. The argument is similar for $\delta(g)_* t$. Finally,

$$
\operatorname{Int} g = \gamma(g) \circ \delta(g)
$$

and hence $(\operatorname{Int} g)_* = \gamma(g)_* \circ \delta(g)_*$.

It is therefore seen that, for $t \in T(G)$, $\varepsilon_g * t$ and $t * \varepsilon_g$ are equal to $gt$ and $tg$ calculated in the group T(G) (§ 2, no. 2). But it should be noted that, for $t, t'$ in T(G), the product $tt'$ in the sense of § 2 is in general different from $t * t'$.

#### Definition 2 {#lie-iii-s3-def-2 .statement}

Let G be a Lie group. The subalgebra of $\mathcal{T}^{(\infty)}(G)$ consisting of the distributions with support contained in e is denoted by $U(G)$.

This algebra is filtered by the subspaces
$$
U_s(G) = U(G) \cap \mathcal{T}^{(s)}(G) = T_e^{(s)}(G).
$$
We write $U^+(G) = T_e^{(\infty)+}(G)$, $U_s^+(G) = U^+(G) \cap U_s(G)$ (cf. Differentiable and Analytic Manifolds, R, 13.2.1). Recall that $U_0(G)$ is identified with K and $U_1^+(G)$ with the tangent space $T_e(G)$. In $U(G)$, $U^+(G)$ is a two-sided ideal supplementary to $U_0(G)$.

#### Example {#lie-iii-s3-n1-exa-1 .statement}

Let E be a complete normable space considered as a Lie group. Then the vector space $U(E)$ is canonically identified with the vector space TS(E) (Differentiable and Analytic Manifolds, R, 13.2.4). Let $m : E \times E \to E$ be addition on E. Then
$$
m_* : TS(E \times E) \to TS(E)
$$
is equal to TS(m) (Differentiable and Analytic Manifolds, R, 13.2.4). For $t, t'$ in $U(E) = TS(E)$, the image $t * t'$ of the symmetric tensor product $t \otimes t'$ under $m_*$ is therefore TS(m)($t \otimes t'$). By Algebra, Chapter IV, § 5, no. 6, Proposition 7, this image is just the product $tt'$ in the algebra TS(E). Thus the algebra $U(E)$ is identified with the algebra TS(E).

#### Proposition 4 {#lie-iii-s3-prop-4 .statement}

Consider the bilinear mapping $(u, v) \mapsto u * v$ (resp. $(u, v) \mapsto v * u$) of $U(G) \otimes K^{(G)}$ into $\mathcal{T}^{(\infty)}(G)$. The corresponding linear mapping of $U(G) \otimes K^{(G)}$ into $\mathcal{T}^{(\infty)}(G)$ is a vector space isomorphism.

$K^{(G)}$ is the direct sum of the $K_{e_x}$ for $x \in G$. On the other hand, the mapping $u \mapsto u * \varepsilon_g$ (resp. $u \mapsto \varepsilon_g * u$) is an isomorphism of the vector space $U(G) = \mathcal{T}_e^{(\infty)}(G)$ onto the vector space $\mathcal{T}_g^{(\infty)}(G)$ by Proposition 3. Finally, $\mathcal{T}^{(\infty)}(G)$ is the direct sum of the $T_g^{(\infty)}(G)$ for $g \in G$.

Let X be a manifold of class $C^r$ ($r \geq \infty$) and $x \in X$. We have defined (Differentiable and Analytic Manifolds, R, 13.3.1) a canonical filtration on the vector space $\mathcal{T}_x^{(\infty)}(X)$ and a canonical isomorphism $i_{X,x}$ of the associated graded vector space onto the graded vector space TS(T_x(X)). In particular, let $T_e(G) = L$; then $i_{G,e}$ is an isomorphism of the graded vector space gr U(G) onto the graded vector space TS(L). But U(G) is a filtered algebra, from which we obtain a graded algebra structure on gr U(G).

#### Proposition 5 {#lie-iii-s3-prop-5 .statement}

The isomorphism $i_{G,e} : \mathrm{gr}\ U(G) \to \mathrm{TS}(L)$ is an algebra isomorphism.

Let $p$ be the mapping $(t, t') \mapsto t \otimes t'$ of $U(G) \times U(G)$ into $U(G \times G)$. Let c be the mapping $(t, t') \mapsto t * t'$ of $U(G) \times U(G)$ into $U(G)$. Let m be the mapping $(g, g') \mapsto gg'$ of $G \times G$ into G. Then by Definition 1
$$
c = m_* \circ p.
$$

Consider the diagram
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}\,\mathrm{U}(G \times G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G \times G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{q} & \mathrm{TS}(L \times L) \\
& & \xrightarrow{\mathrm{TS}(T(m))} \mathrm{TS}(L)
\end{array}
$$
where $q$ is the mapping derived from the canonical isomorphism of $\mathrm{TS}(L) \times \mathrm{TS}(L)$ onto $\mathrm{TS}(L \times L)$. By *Differentiable and Analytic Manifolds*, R, 13.4.6 and 13.3.5, the two squares of the diagram are commutative. Hence by (1) the diagram
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(c)} & \mathrm{gr}\,\mathrm{U}(G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{\mathrm{TS}(T(m)) \circ q} & \mathrm{TS}(L)
\end{array}
$$
is commutative. Now $T(m): L \times L \to L$ maps $(x, y)$ to $x + y$ (§ 2, no. 1, Proposition 2 (ii)). By *Algebra*, Chapter IV, § 5, no. 6, Proposition 7, $\mathrm{TS}(T(m)) \circ q$ is therefore the multiplication of the algebra $\mathrm{TS}(L)$.

### 2. FUNCTIORAL PROPERTIES

#### Proposition 6 {#lie-iii-s3-prop-6 .statement}

Let $G, H$ be Lie groups and $\phi$ a morphism of $G$ into $H$. For $t, t'$ in $\mathcal{T}^{(\infty)}(G)$, $\phi_*(t * t') = \phi_*(t) * \phi_*(t')$.

Consider the diagram
$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
\phi \times \phi \downarrow & & \downarrow \phi \\
H \times H & \xrightarrow{n} & H
\end{array}
$$
where $m(g, g') = gg'$, $n(h, h') = hh'$. This diagram is commutative. Hence
$$
\begin{align*}
\phi_*(t * t') &= \phi_*(m_*(t \otimes t')) = n_*((\phi \times \phi)_*(t \otimes t')) \\
&= n_*(\phi_*(t) \otimes \phi_*(t')) = \phi_*(t) * \phi_*(t').
\end{align*}
$$

The Lie groups $G$ and $G^\vee$ have the same underlying manifold and hence the vector spaces $\mathcal{T}^{(\infty)}(G)$ and $\mathcal{T}^{(\infty)}(G^\vee)$ are the same. Let $\theta$ be the mapping $g \mapsto g^{-1}$, which is an isomorphism of the Lie group $G$ onto the Lie group $G^\vee$. Then $\theta^*$ is an automorphism of the vector space $\mathcal{T}^{(\infty)}(G)$, which automorphism we denote by $t \mapsto t^\vee$. Then $(\varepsilon_g)^\vee = \varepsilon_{g^{-1}}$. If $t \in T_e(G)$, then
$$
t^\vee = -t \quad (§ 2, \text{Proposition 2}).
$$

#### Example {#lie-iii-s3-n2-exa-1 .statement}

Suppose that $G$ is the Lie group defined by a complete normable space $E$. Then $\mathrm{U}(G)$ is identified with $\mathrm{TS}(E)$ and the restriction $\theta_*$ to $\mathrm{U}(G)$ is identified with $\mathrm{TS}(T_e(\theta))$ (*Differentiable and Analytic Manifolds*, R, 13.2.4). Therefore, if $t \in \mathrm{TS}^s(E)$, $t^\vee = (-1)^s t$.

#### Proposition 7 {#lie-iii-s3-prop-7 .statement}

Let G be a Lie group. Let t, t' be in $\mathcal{T}^{(\infty)}(G)$.

(i) The product $t * t'$ calculated relative to $G^\vee$ is equal to the product $t' * t$ calculated relative to G.

(ii) $(t * t')^\vee = {t'}^\vee * t^\vee$.

Consider the diagram

$$
\begin{array}{ccc}
(G_1 \times G_2) \times (G_1 \times G_2) & \xrightarrow{m} & G_1 \times G_2 \\
\downarrow n & & \uparrow p_1 \times p_2 \\
(G_1 \times G_1) \times (G_2 \times G_2)
\end{array}
$$

where $s(g, g') = (g', g)$, $m(g, g') = gg'$, $n(g, g') = g'g$ for all $g, g'$ in G. This diagram is commutative. Hence $n_*(t \otimes t') = m_*(s_*(t \otimes t')) = m_*(t' \otimes t)$. This equality is precisely (i). Assertion (ii) follows from (i) and Proposition 6.

#### Proposition 8 {#lie-iii-s3-prop-8 .statement}

Let G, H be Lie groups and $\phi$ a morphism of G into H. If $t \in \mathcal{T}^{(\infty)}(G)$, then $\phi_*(t^\vee) = (\phi_*(t))^\vee$.

Let $\theta$ (resp. $\theta'$) be the mapping $g \mapsto g^{-1}$ of G into G (resp. of H into H). Then $\phi \circ \theta = \theta' \circ \phi$, whence $\phi_*(\theta_*(t)) = \theta'_*(\phi_*(t))$.

#### Proposition 9 {#lie-iii-s3-prop-9 .statement}

Let $G_1, \ldots, G_n$ be Lie groups and $G = G_1 \times \cdots \times G_n$. If the vector spaces $\mathcal{T}^{(\infty)}(G)$ and $\mathcal{T}^{(\infty)}(G_1) \otimes \cdots \otimes \mathcal{T}^{(\infty)}(G_n)$ are canonically identified, the algebra $\mathcal{T}^{(\infty)}(G)$ is the tensor product of the algebras $\mathcal{T}^{(\infty)}(G_1), \ldots, \mathcal{T}^{(\infty)}(G_n)$. If $t_i \in \mathcal{T}^{(\infty)}(G_i)$ for $i = 1, \ldots, n$, then

$$
(t_1 \otimes \cdots \otimes t_n)^\vee = t_1^\vee \otimes \cdots \otimes t_n^\vee.
$$

It suffices to consider the case $n = 2$. Let $t_1, t_1'$ be in $\mathcal{T}^{(\infty)}(G_1)$, $t_2, t_2'$ in $\mathcal{T}^{(\infty)}(G_2)$. We need to show that $(t_1 \otimes t_2) * (t_1' \otimes t_2') = (t_1 * t_1') \otimes (t_2 * t_2')$ and that $(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$. Consider the diagram

$$
\begin{array}{ccc}
G \times G & \xrightarrow{s} & G \times G \\
\downarrow n & & \downarrow m \\
G & & G
\end{array}
$$

where $m((x_1, x_2), (x_1', x_2')) = (x_1 x_1', x_2 x_2')$,

$$
n((x_1, x_2), (x_1', x_2')) = ((x_1, x_1'), (x_2, x_2')),
$$

$p_1(x_1, x_1') = x_1 x_1'$, $p_2(x_2, x_2') = x_2 x_2'$. This diagram is commutative. Hence

$$
m_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2')) = (p_1 \otimes p_2)_*(n_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2'))),
$$

that is

$$
\begin{align*}
(t_1 \otimes t_2) * (t_1' \otimes t_2') &= (p_1 \otimes p_2)_*((t_1 \otimes t_1') \otimes (t_2 \otimes t_2')) \\
&= p_1*(t_1 \otimes t_1') \otimes p_2*(t_2 \otimes t_2') \\
&= (t_1 * t_1') \otimes (t_2 * t_2').
\end{align*}
$$

It is seen analogously that $(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$.

#### Proposition 10 {#lie-iii-s3-prop-10 .statement}

Let H be a Lie subgroup of G and $i : H \to G$ the canonical injection. Then $i_*$ is an injective homomorphism of the algebra $\mathcal{T}^{(\infty)}(H)$ into the algebra $\mathcal{T}^{(\infty)}(H)$ and $i_*(t^\vee) = (i_*(t))^\vee$ for all $t \in \mathcal{T}^{(\infty)}(H)$.

This follows from Propositions 6 and 8 and Differentiable and Analytic Manifolds, R, 13.2.3.

$\mathcal{T}^{(\infty)}(H)$ is identified with a subalgebra of $\mathcal{T}^{(\infty)}(G)$ by means of the isomorphism of Proposition 10.

#### Remark {#lie-iii-s3-n2-rem-1 .statement}

Proposition 10 remains valid if H is a Lie quasi-subgroup.

We recall (Differentiable and Analytic Manifolds, R, 13.5.1) that, if V is an analytic manifold over K, $\mathcal{T}^{(\infty)}(V)$ has canonically a cogebra structure over K with a counit; the counit is the linear mapping of $\mathcal{T}^{(\infty)}(G)$ into K which associates with each element of $T_x^{(\infty)}(V)$ its constant term.

#### Proposition 11 {#lie-iii-s3-prop-11 .statement}

Let G be a Lie group.
(i) The cogebra $\mathcal{T}^{(\infty)}(G)$, with convolution, is a bigebra (Algebra, Chapter III, § 11, no. 4).
(ii) Let c be the coproduct on $\mathcal{T}^{(\infty)}(G)$. Let $t \in \mathcal{T}^{(\infty)}(G)$ and write
$$
c(t) = \sum_{i=1}^n t_i \otimes t_i'.
$$
Then $c(t^\vee) = \sum_{i=1}^n t_i^\vee \otimes t_{i'}^\vee$.

We prove (i). In the definition of bigebra referred to, condition (1) follows from Propositions 2 and 3 and condition (2) follows from Differentiable and Analytic Manifolds, R, 13.5.1. Let d be the mapping $g \mapsto (g, g)$ of G into $G \times G$. Then $c = d_*$ and hence c is an algebra morphism (Propositions 6 and 9), which is condition (3). Let $t \in T_g^{(\infty)}(G)$, $t' \in T_{g'}^{(\infty)}(G)$ have no constant term and $\lambda, \lambda'$ be elements of K; then $\varepsilon_g \otimes t', t \otimes \varepsilon_{g'}, t \otimes t'$ are without constant term (Differentiable and Analytic Manifolds, R, 13.4.1) and hence the constant term of $(\lambda \varepsilon_g + t) * (\lambda' \varepsilon_{g'} + t')$ is $\lambda \lambda'$; hence condition (4) holds.

We prove (ii). By Propositions 8 and 9,
$$
c(t^\vee) = d_*(t^\vee) = (d_*(t))^\vee = \left( \sum_{i=1}^n t_i \otimes t_i' \right)^\vee = \sum_{i=1}^n t_{i'}^\vee \otimes t_{i'}^\vee.
$$

#### Proposition 12 {#lie-iii-s3-prop-12 .statement}

Let G, H be two Lie groups and $\phi$ a morphism of G into H. Then $\phi_*$ is a bigebra morphism of $\mathcal{T}^{(\infty)}(G)$ into $\mathcal{T}^{(\infty)}(H)$.

This follows from Proposition 6 and Differentiable and Analytic Manifolds, R, 13.5.1.

Let G be a Lie group. The restrictions of the convolution and the coproduct to U(G) define a bigebra structure on U(G). We have U(G)^{\vee} = U(G). If $\phi : G \to H$ is a Lie group morphism, we denote by U($\phi$) the mapping $t \mapsto \phi_*(t)$ of U(G) into U(H); this is a bigebra morphism. If $\psi : H \to L$ is another Lie group morphism, then U($\psi \circ \phi$) = U($\psi$) \circ U($\phi$). If $\phi$ is an immersion (resp. a submersion), U($\phi$) is injective (resp. surjective) by *Differentiable and Analytic Manifolds*, R, 13.2.3. In particular, if H is a Lie subgroup of G, U(H) is identified with a subalgebra of U(G), the coproduct on U(H) being the restriction of the coproduct on U(G). If H is open in G, then U(H) = U(G). If G_1, G_2 are Lie groups, U(G_1 \times G_2) is identified with U(G_1) \times U(G_2). The primitive elements of U(G) are those of T_e(G) (*Differentiable and Analytic Manifolds*, R, 13.5.3).

Again let $\phi : G \to H$ be a Lie group morphism. If gr U(G) is identified TS(T_e(G)) and gr U(H) with TS(T_e(H)), then gr U($\phi$) is identified with TS(T_e($\phi$)) (*Differentiable and Analytic Manifolds*, R, 13.3.5). We apply this to the isomorphism $g \mapsto g^{-1}$ of G onto G^{\vee}; then T_e($\phi$) = -1 and hence

$$
t \in U_s(G) \Rightarrow t^{\vee} \equiv (-1)^s t \mod U_{s-1}(G).
$$

### 3. CASE OF A GROUP OPERATING ON A MANIFOLD

Let G be a Lie group, X a manifold of class C^r and f a law of left operation of class C^r of G on X. If $t \in T^{(s)}_g(G)$ and $u \in T^{(s')}_x(X)$ and $s + s' \leq r$, we denote by $t * u$ the image of $t \otimes u$ under $f_*$. We extend the product \* to a bilinear mapping also denoted by *, of $\mathcal{T}^{(s)}(G) + \mathcal{T}^{(s')}(X)$ into $\mathcal{T}^{(s+s')}(X)$. Proposition 1 of no. 1 can be extended with obvious modifications to the present situation.

When G operates on itself by left translation, we recover Definition 1 of no. 1.

#### Proposition 13 {#lie-iii-s3-prop-13 .statement}

Let $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$, $u \in \mathcal{T}^{(s'')}(X)$, such that

$$
s + s' + s'' \leq r.
$$

Then $(t * t') * u = t * (t' * u)$.

This can be proved as is Proposition 2 of no. 1.

In particular, if $r \leq \infty$, the vector space $\mathcal{T}^{(\infty)}(X)$ is a left module over the algebra $\mathcal{T}^{(\infty)}(G)$ with the product *.

#### Proposition 14 {#lie-iii-s3-prop-14 .statement}

(i) Let $g_0 \in G$ and $\tau(g_0)$ be the mapping $x \mapsto f(g_0, x)$ of X into X. If $u \in \mathcal{T}^{(r)}(X)$, then $\tau(g_0)*u = \varepsilon_{g_0}*u$.

(ii) Let $x_0 \in X$ and $\varrho(x_0)$ be the mapping $g \mapsto f(g, x_0)$ of G into X. If $t \in T^{(r)}(G)$, then $\varrho(x_0)*t = t*\varepsilon_{x_0}$.

This can be proved as is Proposition 3 of no. 1.

In particular, if $u \in T(X)$ and $t \in T(G)$, $\varepsilon_{g_0} * u$ and $t * \varepsilon_{x_0}$ are equal to the products $g_0u$ and $tx_0$ defined in § 2, no. 2.

#### Proposition 15 {#lie-iii-s3-prop-15 .statement}

Let G (resp. G') be a Lie group and X (resp. X') a manifold of class C^r. Suppose that a law of left operation of class C^r of G (resp. G') on X (resp. X') is given. Let $\phi$ be a morphism of G into G' and $\psi$ a $\phi$-morphism of X into X'. Let $t \in \mathcal{T}^{(s)}(G)$, $u \in T^{(s')}(X)$ be such that $s + s' \leq r$. Then
$$
\psi_*(t * u) = \phi_*(t) * \psi_*(u).
$$
This can be proved as is Proposition 6 of no. 2.

#### Remark {#lie-iii-s3-n3-rem-1 .statement}

Let f be a law of right operation of class C^r of G on X. If $t \in \mathcal{T}^{(s)}(G)$ and $u \in \mathcal{T}^{(s')}(X)$, with $s + s' \leq r$, we denote by $u * t$ the image of $u \otimes t$ under $f_*$. Propositions 13, 14, 15 go over to this situation in an obvious way.

#### Proposition 16 {#lie-iii-s3-prop-16 .statement}

Let G, G' be Lie groups, X a manifold of class C^r and suppose that G (resp. G') operates on X on the left (resp. right), with $(gx)g' = g(xg')$ for all $x \in X, g \in G, g' \in G'$. Let $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G')$, $t'' \in T^{(s'')}(X)$, with $s + s' + s'' \leq r$. Then
$$
(t * t'') * t' = t * (t'' * t').
$$
$(t * t'') * t'$ (resp. $t * (t'' * t')$) is the image of $t \otimes t'' \otimes t'$ under the mapping $(g, x, g') \mapsto (gx)g'$ (resp. $g(xg')$) of $G \times X \times G'$ into X.

### 4. CONVOLUTION OF POINT DISTRIBUTIONS AND FUNCTIONS

Let G be a Lie group, X a manifold of class C^r and $(g, x) \mapsto gx$ a law of left operation of class C^r of G on X. For all $x \in X$, let $\varrho(x)$ denote the orbital mapping of x.

#### Definition 3 {#lie-iii-s3-def-3 .statement}

Let $t \in \mathcal{T}^{(s)}(G)$ with $s \leq r$. Let $f : X \to F$ be a function of class C^r with values in a Hausdorff polynormed space (for example $F = \mathbf{K}$). The convolution of t and f, denoted by $t * f$, is the function on X with values in F defined by
$$
(t * f)(x) = \langle t^\vee * \varepsilon_x, f \rangle.
$$
Then
$$
\begin{align*}
(t * f)(x) &= \langle \varrho(x)_*(t^\vee), f \rangle \quad \text{(no. 3, Proposition 14 (ii))} \\
&= \langle t^\vee, f \circ \varrho(x) \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)} \\
&= \langle t, (f \circ \varrho(x))^\vee \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$
Note that Definition 3 can also be written in the more symmetric form
$$
\langle \varepsilon_x, t * f \rangle = \langle t^\vee * \varepsilon_x, f \rangle.
$$
The function $(g, x) \mapsto f(gx) = (f \circ \varrho(x))(g)$ on $G \times X$ is of class C^r. By Differentiable and Analytic Manifolds, R, 13.4.4, the function $x \mapsto \langle t^\vee, f \circ \varrho(x) \rangle$ is therefore of class $C^{r-s}$ if $s < \infty$. In other words, if $s < \infty$, $t * f$ is of class $C^{r-s}$.

Clearly $t * f$ depends linearly on $t$ and $f$.

Formula (4) implies in particular, for $g \in G$,
$$
(\varepsilon_g * f)(x) = f(g^{-1}x)
$$
that is
$$
\varepsilon_g * f = \gamma(g)f.
$$

Suppose that $K = \mathbf{R}$ or $\mathbf{C}$, that $G$ and $X$ are finite-dimensional and that $X$ has a positive measure invariant under $G$. The definition of $\varepsilon_g * f$ agrees with that of Integration, Chapter VIII, § 4, no. 1 (cf. formula (2), loc. cit.).

#### Proposition 17 {#lie-iii-s3-prop-17 .statement}

Let $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(X)$ and $f : X \to F$ a function of class $C^r$ with $s + s' \leq r$. Then
$$
\langle t', t * f \rangle = \langle t^\vee * t', f \rangle.
$$
$$
\begin{align*}
\langle t', t * f \rangle &= \langle t', x \mapsto \langle t, g \mapsto f(g^{-1}x) \rangle \rangle \quad \text{by (4)} \\
&= \langle t \otimes t', (g, x) \mapsto f(g^{-1}x) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.4.4}) \\
&= \langle t^\vee \otimes t', (g, x) \mapsto f(gx) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \langle t^\vee * t', f \rangle.
\end{align*}
$$

#### Proposition 18 {#lie-iii-s3-prop-18 .statement}

Let $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$ and $f : X \to F$ a function of class $C^r$, with $s + s' \leq r$. Then
$$
(t * t') * f = t * (t' * f).
$$
For all $x \in X$,
$$
\begin{align*}
\langle \varepsilon_x, (t * t') * f \rangle &= \langle ((t * t')^\vee * \varepsilon_x), f \rangle \quad \text{by (5)} \\
&= \langle {t'}^\vee * (t^\vee * \varepsilon_x), f \rangle \quad (\text{Propositions 2 and 7}) \\
&= \langle t^\vee * \varepsilon_x, t' * f \rangle \quad (\text{Proposition 17}) \\
&= \langle \varepsilon_x, t * (t' * f) \rangle \quad (\text{Proposition 17}).
\end{align*}
$$

If $r \geq \infty$, we see that the set of functions of class $C^\infty$ on $X$ with values in $F$ is a left module over the algebra $\mathcal{T}^{(\infty)}(G)$.

#### Proposition 19 {#lie-iii-s3-prop-19 .statement}

Let $t \in \mathcal{T}^{(s)}(G)$, with $s \leq r$. Let $f$ (resp. $f'$) be a function of class $C^r$ on $X$ with values in a Hausdorff polynormed space $F$ (resp. $F'$). Let $(u, u') \mapsto uu'$ be a continuous bilinear mapping of $F \times F'$ into a Hausdorff polynormed space $F''$, so that $ff'$ is a function of class $C^r$ on $X$ with values in $F''$. Let
$$
\sum_{i=1}^n t_i \otimes t'_i \text{ be the image of } t \text{ in } \mathcal{T}^{(s)}(G) \otimes \mathcal{T}^{(s)}(G) \text{ under the coproduct. Then}
$$
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

Let $x \in X$ and let $\rho(x)$ denote the orbital mapping of $x$. Then
$$
\langle \varepsilon_x, t * (ff') \rangle = \langle t^\vee, (ff') \circ \rho(x) \rangle \quad \text{by (4)} \\
= \langle t^\vee, (f \circ \rho(x))(f' \circ \rho(x)) \rangle \\
= \sum_{i=1}^n \langle t_i^\vee, f \circ \rho(x) \rangle \langle t_{i'}^\vee, f' \circ \rho(x) \rangle \tag{Diff. \& Man. Anal., R, 13.5.2} \\
= \sum_{i=1}^n \langle \varepsilon_x, t_i * f \rangle \langle \varepsilon_x, t_i' * f' \rangle \quad \text{by (4).}
$$

#### Remark 1 {#lie-iii-s3-n4-rem-1 .statement}

Let G be a Lie group, X a manifold of class $C^r$ and $(x, g) \mapsto xg$ a law of right operation of class $C^r$ of G on X. If $t \in \mathcal{T}^{(s)}(G)$ with $s \leq r$ and $f : X \to F$ is a function of class $C^r$ on X, we denote by $f * t$ the function on X defined by
$$
\langle \varepsilon_x, f * t \rangle = \langle \varepsilon_x * t^\vee, f \rangle \\
= \langle \rho(x) * (t^\vee), f \rangle \\
= \langle t^\vee, f \circ \rho(x) \rangle \\
= \langle t, (f \circ \rho(x))^\vee \rangle.
$$
In particular
$$
(f * \varepsilon_g)(x) = f(xg^{-1})
$$
that is
$$
f * \varepsilon_g = \delta(g)^{-1} f.
$$
Propositions 17, 18, 19 become, in the obvious notation,
$$
\langle t', f * t \rangle = \langle t' * t^\vee, f \rangle \tag{11}
$$
$$
f * (t * t') = (f * t) * t' \tag{12}
$$
$$
(ff') * t = \sum_{i=1}^n (f * t_i)(f' * t_i') \tag{13}
$$

#### Proposition 20 {#lie-iii-s3-prop-20 .statement}

*Let G, G' be Lie groups, X a manifold of class $C^r$ and $(g, x) \mapsto gx$ (resp. $(x, g') \mapsto xg'$) a law of left (resp. right) operation of class $C^r$ of G (resp. G') on X. Suppose that $(gx)g' = g(xg')$ for all $x \in X, g \in G, g' \in G'$. Let $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G')$ and $f : X \to F$ be a function of class $C^r$ such that $s + s' \leq r$. Then*
$$
(t * f) * t' = t * (f * t').
$$
For all $x \in X$,
$$
\langle \varepsilon_x, (t * f) * t' \rangle = \langle \varepsilon_x * {t'}^\vee, t * f \rangle \quad \text{by (8)} \\
= \langle t^\vee * (\varepsilon_x * {t'}^\vee), f \rangle \quad \text{(Proposition 17)} \\
= \langle t^\vee * \varepsilon_x, f * t' \rangle \quad \text{(Proposition 2 and (11))} \\
= \langle \varepsilon_x, t * (f * t') \rangle \quad \text{by (5).}
$$

In particular, consider G as operating on itself by left and right translations. If $f : G \to F$ is a function of class $C^r$ on G and $t \in \mathcal{T}^{(s)}(G)$ (with $s \leq r$), $t * f$ and $f * t$ are, if $s < \infty$, functions of class $C^{r-s}$ on G. Further, let $t' \in \mathcal{T}^{(s')}(G)$, with $s + s' \leq r$. Then
$$
(t * f) * t' = t * (f * t').
$$
In particular, $\mathcal{C}^\infty(G)$ is a $(\mathcal{T}^{(\infty)}(G), \mathcal{T}^{(\infty)}(G))$-bimodule. Formulae (5) and (8) admit as special cases
$$
\langle t, f \rangle = \langle \varepsilon_e, t^\vee * f \rangle = \langle \varepsilon_e, f * t^\vee \rangle.
$$

#### Remark 2 {#lie-iii-s3-n4-rem-2 .statement}

Let $(g, x) \mapsto gx$ be a law of left operation of class $C^r$ of G on X. Let $t \in U_s(G)$ with $s \leq r$, $\Omega$ be an open subset of X and $f : \Omega \to F$ a function of class $C^r$. $t * f$ can also be defined by formula (4) or (5); it is a function defined on $\Omega$ with values in F, of class $C^{r-s}$ if $s < \infty$. The results of this no. extend in an obvious way to this situation.

### 5. FIELDS OF POINT DISTRIBUTIONS DEFINED BY THE ACTION OF A GROUP ON A MANIFOLD

Let $(g, x) \mapsto \lambda(g, x) = gx$ be a law of left operation of class $C^r$ of G on X. Let $s \leq r$ and $t \in U_s(G)$. For all $x \in X$, $t * \varepsilon_x \in T^{(s)}_x(X)$. The mapping $x \mapsto t * \varepsilon_x$ is called the field of point distributions defined by t and the action of G on X and denoted sometimes by $D_t^\lambda$ or simply $D_t$. Let $\Omega$ be an open subset of X and F a Hausdorff polynormed space. If $f : \Omega \to F$ is of class $C^r$ and $s \leq r$, the function $t^\vee * f$ on $\Omega$ is also denoted by $D_t f$. Then
$$
(D_t f)(x) = \langle t * \varepsilon_x, f \rangle.
$$
If $s < \infty$, then $D_t f \in \mathcal{C}^{r-s}(\Omega, F)$ by no. 4. Thus $f \mapsto D_t f$ is a mapping of $\mathcal{C}^r(\Omega, F)$ into $\mathcal{C}^{r-s}(\Omega, F)$ (often denoted by $D_t$ by an abuse of notation).
If $t \in U_s(G)$, $t' \in U_{s'}(G)$ and $s + s' \leq r$, then, by Proposition 18 of no. 4,
$$
D_{t*t'} = D_{t'}(D_t f)
$$
and hence, using the abuse of notation indicated above,
$$
D_{t*t'} = D_{t'} \circ D_t.
$$
Suppose that G and X are finite-dimensional. The mapping $(t, x) \mapsto t \otimes \varepsilon_x$ of $T^{(s)}(G) \times X$ into the vector bundle $T^{(s)}(G \times X)$ (cf. Differentiable and Analytic Manifolds, R, 13.2.5) is of class $C^{r-s}$. Hence (Differentiable and Analytic Manifolds, R, 13.2.5) the mapping $(t, x) \mapsto t * \varepsilon_x$ of $T^{(s)}(G) \times X$ into the vector bundle $T^{(s)}(X)$ is of class $C^{r-s}$. In particular, $D_t$ is a differential operator of order $\leq s$ and class $C^{r-s}$ in the sense of Differentiable and Analytic Manifolds, R, 14.1.6. By formula (16), the function $D_t f$ is then the image of $f$ under this differential operator (Differentiable and Analytic Manifolds, R, 14.1.4).

We now no longer suppose that G and X are finite-dimensional. Let $\psi$ be an automorphism of the manifold X and $\Delta$ a field of point distributions on X. Conforming with the general definitions, the transform of $\Delta$ under $\psi$ is the field of point distributions on X whose value at $\psi(x)$ is $\psi_*(\Delta(x))$; we denote this mapping by $\psi(\Delta)$. If $g \in G$ and $\tau(g)$ denotes the automorphism $x \mapsto gx$ of X, the transform of $\Delta$ under $\tau(g)$ is also called the transform of $\Delta$ under g.

#### Proposition 21 {#lie-iii-s3-prop-21 .statement}

*Let $\psi$ be an automorphism of X commuting with the operations of G. Then $D_t$ is invariant under $\psi$.*

For all $x \in X$,

$$
\begin{align*}
(\psi(D_t))(\psi(x)) &= \psi_*(D_t(x)) = \psi_*(t * \varepsilon_x) \\
&= t * \psi_*(\varepsilon_x) \tag{Proposition 15} \\
&= t * \varepsilon_{\psi(x)} = D_t(\psi(x)).
\end{align*}
$$

#### Proposition 22 {#lie-iii-s3-prop-22 .statement}

*If $g \in G$, the transform of $D_t$ under g is $D_{\varepsilon_g * t * \varepsilon_g^{-1}}$.*

The value of this transform at $gx$ is

$$
\begin{align*}
\tau(g)_*(D_t(x)) &= \tau(g)_*(t * \varepsilon_x) \\
&= \varepsilon_g * (t * \varepsilon_x) \quad \text{(Proposition 14 (i))} \\
&= (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_{gx} \quad \text{(Propositions 1 and 2)} \\
&= D_{\varepsilon_g * t * \varepsilon_g^{-1}}(gx).
\end{align*}
$$

Let $(x, g) \mapsto \mu(x, g) = xg$ be a law of right operation of class $C'$ of G on X. Let $s \leq r$ and $t \in U_s(G)$. For all $x \in X$, $\varepsilon_x * t \in T^{(s)}_x(X)$. The mapping $x \mapsto \varepsilon_x * t$ is called the field of distributions defined by t and the action of G on X and is sometimes denoted by $D_t^u$ or simply $D_t$. Let $\Omega$ be an open subset of X. If $f : \Omega \to F$ is of class $C'$, the function $f * t^\vee$ is denoted by $D_t f$. Then

$$(19)$$
$$(D_t f)(x) = \langle \varepsilon_x * t, f \rangle$$

and, in the obvious notation,

$$(20)$$
$$D_{t * t'} f = D_t(D_{t'} f)$$

$$(21)$$
$$D_{t * t'} = D_t \circ D_{t'}.$$

Proposition 21 remains valid. Let $g \in G$. The transform of $D_t$ under g (that is under the automorphism $x \mapsto xg$ of X) is $D_{\varepsilon_g^{-1} * t * \varepsilon_g}$.

### 6. INVARIANT FIELDS OF POINT DISTRIBUTIONS ON A LIE GROUP

#### Definition 4 {#lie-iii-s3-def-4 .statement}

*Let G be a Lie group. A field of distributions on G is called left (resp. right) invariant if it is invariant under left (resp. right) translations of G.*

In other words, a field of distributions $g \mapsto \Delta_g$ on $G$ is left invariant if
$$
\Delta_{gg'} = \gamma(g) * \beta_{g'}
$$
for $g, g'$ in $G$,
or again if
$$
\Delta_{gg'} = \varepsilon_g * \Delta_{g'}
$$
for $g, g'$ in $G$.
It is right invariant if
$$
\Delta_{gg'} = \delta({g'}^{-1}) * \Delta_g
$$
for $g, g'$ in $G$,
or again if:
$$
\Delta_{gg'} = \Delta_g * \varepsilon_g,
$$
for $g, g'$ in $G$.

#### Definition 5 {#lie-iii-s3-def-5 .statement}

*Let $G$ be a Lie group and $t \in U(G)$. Let $L_t$ denote the field of distributions $g \mapsto \varepsilon_g * t$ on $G$ and $R_t$ the field of distributions $g \mapsto t * \varepsilon_g$ on $G$.*

In other words, $L_t$ (resp. $R_t$) is the field of distributions defined by $t$ and $G$ operating on $G$ on the right (resp. left) by means of the mapping $(g, g') \mapsto gg'$. Let $\Omega$ be an open subset of $G$ and $F$ a Hausdorff polynormed space; if $f \in C^\omega(\Omega, F)$, then $L_t f = f * t^\vee \in C^\omega(\Omega, F)$ and
$$
R_t f = t^\vee * f \in C^\omega(\Omega, F)
$$
(no. 5). If $G$ is finite-dimensional, the differential operators $L_t$ and $R_t$ are of class $C^\omega$ (no. 5).

#### Proposition 23 {#lie-iii-s3-prop-23 .statement}

(i) *The mapping $t \mapsto L_t$ (resp. $t \mapsto R_t$) is an isomorphism of the vector space $U(G)$ onto the vector field of left (resp. right) invariant distributions on $G$.*
(ii) *For $t, t'$ in $U(G)$, $L_{t*t'} = L_t \circ L_{t'}$, $R_{t*t'} = R_{t'} \circ R_t$, $L_t \circ R_{t'} = R_{t'} \circ L_t$ (with the abuse of notation of no. 5).*
(iii) *If $\theta$ is the mapping $g \mapsto g^{-1}$ of $G$ onto $G$, then $\theta(L_t) = R_{t^\vee}$.*
(iv) *If $t \in U(G)$ and $g \in G$, then $(L_t)_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g$.*

In $G$ every right translation commutes with every left translation. By Proposition 21 of no. 5, $L_t$ is therefore left invariant. As $(L_t)_e = t$, the mapping $t \mapsto L_t$ is injective. Let $\Delta$ be a field of left invariant distributions on $G$; let $t = \Delta_e$; then $\Delta$ and $L_t$ have the same value at $e$ and are left invariant and hence $\Delta = L_t$. This proves (i) for $L_t$ and the argument is similar for $R_t$. The formulae $L_{t*t'} = L_t \circ L_{t'}$, $R_{t*t'} = R_{t'} \circ R_t$ follow from (21) and (18). Let $t \in U_s(G)$, $t' \in U_{s'}(G)$, $f \in C^r(\Omega, F)$, where $\Omega$ is open in $G$ and $s + s' \leq r$; then
$$
\begin{align*}
L_t R_{t'} f &= L_t ({t'}^\vee * f) = ({t'}^\vee * f) * t \\
&= {t'}^\vee * (f * t^\vee) \tag{Proposition 20} \\
&= R_{t'} L_t f
\end{align*}
$$
and hence $L_t \circ R_{t'} = R_{t'} \circ L_t$. As $\theta$ is an isomorphism of $G$ onto $G^\vee$, $\theta(L_t)$ is a field of right invariant distributions on $G$; its value at $e$ is $\theta(t) = t^\vee$; hence $\theta(L_t) = R_{t^\vee}$. Finally,
$$
(L_t)_g = \varepsilon_g * t = (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g.
$$

#### Remark 1 {#lie-iii-s3-n6-rem-1 .statement}

It is the action of G on itself by right translation which defines the fields of left invariant distributions.

#### Remark 2 {#lie-iii-s3-n6-rem-2 .statement}

Suppose that G is finite-dimensional. The mapping

$$(t, g) \mapsto (\mathbf{R}_t)_g = t * \varepsilon_g$$

of $U_s(G) \times G$ into $T^{(s)}(G)$ is an isomorphism of analytic vector bundles; for this mapping is bijective, linear on each fibre and analytic (no. 5); on the other hand, let $\phi : T^{(s)}(G) \to U_s(G) \times G$ be the inverse bijection; if $t \in T^{(s)}_g(G)$, then $\phi(t) = (t * \varepsilon_{g^{-1}}, g)$ and hence $\phi$ is analytic. The isomorphism $\phi$ is called the right trivialization of $T^{(s)}(G)$. Similarly, consider the mapping $(t, g) \mapsto (\mathbf{L}_t)_g = \varepsilon_g * t$ of $U_g(G) \times G$ into $T^{(s)}(G)$; the inverse isomorphism is called the left trivialization of $T^{(s)}(G)$. By restriction we recover the right and left trivializations of $T(G)$ (§ 2, no. 2).

### 7. LIE ALGEBRA OF A LIE GROUP

Let G be a Lie group. In $U(G)$, as in any associative algebra, we write $[t, t'] = t * t' - t' * t$. As $T_e(G)$ is the set of primitive elements of $U(G)$, $[T_e(G), T_e(G)] \subset T_e(G)$ (Chapter II, § 1, no. 2, Proposition 4). The restriction of the bracket to $T_e(G)$ therefore defines on $T_e(G)$ a Lie algebra structure.

#### Lemma 1 {#lie-iii-s3-lem-1 .statement}

Let X and $X'$ be complete normable spaces, $X_0$ an open neighbourhood of 0 in X and f an analytic mapping of $X_0$ into $X'$ such that $f(0) = 0$. Let $f = f_1 + f_2 + f_3 + \cdots$ be the expansion of f as an integral series about 0, where $f_i$ is a homogeneous continuous-polynomial of degree i on X with values in $X'$. Let t be an element of TS$^2(X)$, considered as a point distribution on X with support contained in \{0\}. Let $t' = f_*(t) \in TS(X')$. The homogeneous component of $t'$ of degree 1 is $\langle f_2, t \rangle$.

Let $t'_1$ be this component. Then, for every continuous linear mapping u of $X'$ into a polynormed space,

$$
u(t'_1) = \langle t', u \rangle \quad \text{because } u \text{ is continuous and linear}
$$
$$
= \langle t, u \circ f \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3})
$$
$$
= \langle t, u \circ f_2 \rangle \quad \text{because } t \in TS^2(X)
$$
$$
= u(\langle t, f_2 \rangle) \quad (\text{Diff. \& Anal. Man., R, 13.2.2}),
$$

whence the lemma.

#### Proposition 24 {#lie-iii-s3-prop-24 .statement}

Let G be a Lie group and $(U, \phi, E)$ a chart on G such that $\phi(e) = 0$. Let V be an open neighbourhood of e such that $V^2 \subset U$. Let m be the analytic mapping $(a, b) \mapsto \phi(\phi^{-1}(a)\phi^{-1}(b))$ of $\phi(V) \times \phi(V)$ into E. Let

$$
m = \sum_{i, j \geq 0} m_{i, j}
$$

be the expansion of m as an integral series about (0, 0), where $m_{i,j}$ is a bihomogeneous continuous-polynomial of bidegree $(i, j)$ on $E \times E$ with values in $E$.

(i) $m_{i,0} = m_{0,j} = 0$ for all $i \neq 1$ and $j \neq 1$.
(ii) $m_{1,0}(a, b) = a$ and $m_{0,1}(a, b) = b$ for all $a \in E, b \in E$.
(iii) *Let $\psi : T_e(G) \to E$ be the differential of $\phi$ at e. For all $u, v$ in $T_e(G)$,

$$
\psi([u, v]) = m_{1,1}(\psi(u), \psi(v)) - m_{1,1}(\psi(v), \psi(u)).
$$

$m(a, 0) = a,\ m(0, b) = b$ for all $a, b$ in $\phi(V)$, which proves (i) and (ii).
Let $u, v$ be in $T_e(G)$. Let $T_0(E)$ be identified with $E$ and hence $\psi$ with $T_e(\phi)$:
The images of $u$ and $v$ under $T_e(\phi)$ are $\psi(u)$ and $\psi(v)$. The tensor product point distribution of these images is the symmetric product of $(\psi(u), 0)$ and $(0, \psi(v))$ in $TS(E \times E) = TS(E) \times TS(E)$, that is

$$
(\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0).
$$

Hence $\phi * (u * v)$ is the image of the above element under the mapping $m$ of $\phi(V) \times \phi(V)$ into $E$. Its component of degree 1 in $TS(E)$ is, by Lemma 1,

$$
x = \langle m_{1,1}, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle.
$$

We define a bilinear mapping $n : (E \times E)^2 \to E$ by

$$
n((a, b), (a', b')) = m_{1,1}(a, b').
$$

Then $n((a, b), (a, b)) = m_{1,1}(a, b)$ and hence

$$
x = \langle n, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle \\
= m_{1,1}(\psi(u), \psi(v)) + m_{1,1}(0, 0) = m_{1,1}(\psi(u), \psi(v)).
$$

Similarly, $\phi * (v * u)$ admits $m_{1,1}(\phi(v), \phi(u))$ as component of degree 1 in $TS(E)$. As $\phi([u, v])$ is of degree 1, this proves (iii).

#### Corollary {#lie-iii-s3-n7-cor-1 .statement}

*The normable space $T_e(G)$ together with the bracket, is a normable Lie algebra.*

#### Definition 6 {#lie-iii-s3-def-6 .statement}

*The normable space $T_e(G)$, together with the bracket, is called the normable Lie algebra of G, or simply the Lie algebra of G, and is denoted by $L(G)$.*

#### Proposition 25 {#lie-iii-s3-prop-25 .statement}

*Let G be a Lie group and $E(G)$ the enveloping algebra of $L(G)$. The canonical injection of $L(G)$ into $E(G)$ defines a homomorphism $\theta$ of the algebra $E(G)$ into the algebra $U(G)$. If K is of characteristic 0, $\eta$ is a bigebra isomorphism.*

The bigebra $U(G)$ is cocommutative (*Differentiable and Analytic Manifolds*, R, 13.5.1) and the filtration $(U_s(G))$ is compatible with the bigebra structure. The set of primitive elements of $U(G)$ is $L(G)$. It then suffices to apply chapter II, § 1, no. 6, Theorem 1.

When K is of characteristic 0 we shall in future identify $U(G)$ with the enveloping algebra of $L(G)$. By (2) and Proposition 7 (ii), the mapping $t \mapsto t^\vee$ of $U(G)$ into $U(G)$ is then identified with the principal antiautomorphism of $U(G)$ (Chapter I, § 2, no. 4).

#### Proposition 26 {#lie-iii-s3-prop-26 .statement}

*Suppose that K is of characteristic $p > 0$. For all $a \in L(G)$, $a^p \in L(G)$ and $\operatorname{ad}(a^p) = (\operatorname{ad} a)^p$ (the power $a^p$ being calculated in $U(G)$).*

If $a \in L(G)$, $a$ is primitive in $U(G)$, hence $a^p$ is primitive in $U(G)$ (Chapter II, § 1, no. 2, *Remark 1*) and hence $a^p \in L(G)$. Let $\sigma_a$ (resp. $\tau_a$) be the linear mapping $x \mapsto a * x$ (resp. $x \mapsto x * a$) of $U(G)$ into $U(G)$. For all $x \in U(G)$, $(\operatorname{ad} a)(x) = (\sigma_a - \tau_a)(x)$ and hence $(\operatorname{ad} a)^p = (\sigma_a - \tau_a)^p$. But $\sigma_a$ and $\tau_a$ commute and therefore $(\sigma_a - \tau_a)^p = (\sigma_a)^p - (\tau_a)^p = \tau_a^p - \sigma_a^p$, whence the second assertion.

#### Definition 7 {#lie-iii-s3-def-7 .statement}

*Let X be a manifold of class $C^r$ ($r \geq 2$) and $g$ a complete normable Lie algebra. A law of infinitesimal left (resp. right) operation of class $C^{r-1}$ of $g$ on X is a mapping $a \mapsto D_a$ of $g$ into the set of vector fields on X with the following properties:*

(a) *the mapping $(a, x) \mapsto D_a(x)$ is a morphism of class $C^{r-1}$ of the trivial vector bundle $g \times X$ into the vector bundle $T(X)$;*

(b) $[D_a, D_b] = -D_{[a, b]}$ (resp. $[D_a, D_b] = D_{[a, b]}$ for all $a, b$ in $g$).

In particular, each vector field $D_a$ is of class $C^{r-1}$.

#### Remark {#lie-iii-s3-n7-rem-1 .statement}

Let X be a manifold of class $C^r$, $g$ a finite-dimensional Lie algebra and $a \mapsto D_a$ a linear mapping of $g$ into the vector space of vector fields of class $C^{r-1}$ on X. Then condition (a) of Definition 7 holds. For, by considering a basis of $g$ and applying *Differentiable and Analytic Manifolds*, R, 7.7.1, the problem is reduced to the case $\dim g = 1$ and our assertion is then obvious.

#### Proposition 27 {#lie-iii-s3-prop-27 .statement}

*Let G be a Lie group and X a manifold of class $C^r$. Suppose that a law of left (resp. right) operation of class $C^r$ of G on X is given. For all $a \in L(G)$, let $D_a$ be the field of point distributions defined by a on X.*

(i) *The mapping $(a, x) \mapsto D_a(x)$ is a morphism of class $C^{r-1}$ of the trivial vector bundle $L(G) \times X$ into the vector bundle $T(X)$.*

(ii) *Let I be an open subset of K containing 0 and $\gamma : I \to G$ a mapping of class $C^r$ such that $\gamma(0) = e$. Let $a = T_0(\gamma)1 \in L(G)$. If f is a function of class $C^r$ on an open subset of X, then*
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)) \quad \text{if G operates on the left,}
$$
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(x\gamma(k)) - f(x)) \quad \text{if G operates on the right.}
$$

(iii) *If $r \geq 2$, the mapping $a \mapsto D_a$ is a law of infinitesimal left (resp. right) operation of class $C^{r-1}$ of $L(G)$ on X.*

Suppose that G operates on X on the left. Let $\phi : G \times X \to X$ be the law of operation. Then $T(\phi)$ is a $\phi$-morphism of class $C^{r-1}$ of the vector bundle $T(G) \times T(X)$ into the vector bundle $T(X)$ (*Differentiable and Analytic*

Manifolds, R, 8.1.2). The induced vector bundle $(\mathrm{T}(G) \times \mathrm{T}(X))|_{\{\epsilon\} \times X}$ is identified with $E = L(G) \times T(X)$. Hence $T(\phi)|E$ is a vector bundle morphism of class $C^{r-1}$. For $(a, x) \in L(G) \times X, T(\phi)(a, x) = D_a(x)$, whence (i).

The formula giving $(D_a f)(x)$ follows from § 2, the end of no. 2, and Differentiable and Analytic Manifolds, R, 8.4.5.

Suppose that $r \geqslant 2$. Let $a, b$ be in $L(G)$ and $f$ be a function of class $C^r$ on an open subset of $X$. Then
$$
\begin{align*}
D_{[a, b]}f &= D_b(D_a f) - D_a(D_b f) \quad \text{by (17)} \\
&= [D_b, D_a]f \tag{Diff. \& Anal. Man., R, 8.5.3}.
\end{align*}
$$
Let $x \in X$. By taking $f$ to be a chart on an open neighbourhood of $x$, it follows that $D_{[a, b]}(x) = [D_b, D_a](x)$, whence (iii). The argument is similar if $G$ operates on $X$ on the right.

When $r \geqslant 2$, the mapping $a \mapsto D_a$ is called the law of infinitesimal operation associated with the given law of operation.

### 8. FUNCTIORIAL PROPERTIES OF THE LIE ALGEBRA

Let $G$ and $H$ be Lie groups and $\phi$ a morphism of $G$ into $H$. The restriction of $U(\phi)$ to $L(G)$, which is just $T_e(\phi)$, is a continuous morphism of $L(G)$ into $L(H)$, which we denote by $L(\phi)$. If $\psi$ is a morphism of $H$ into a Lie group, then $L(\psi \circ \phi) = L(\psi) \circ L(\phi)$.

For $\phi$ to be an immersion, it is necessary and sufficient that $L(\phi)$ be an isomorphism of $L(G)$ onto a subalgebra of $L(H)$ admitting a topological supplement. In particular, if $G$ is a Lie subgroup of $H$ and $\phi$ is the canonical injection, $L(G)$ is identified with a Lie subalgebra of $L(H)$ by means of $L(\phi)$. More particularly, if $G$ is an open subgroup of $H$, $L(G) = L(H)$.

If $G$ is a Lie quasi-subgroup of $H$, $L(G)$ is also identified with a closed Lie subgroup of $L(H)$.

For $\phi$ to be a submersion, it is necessary and sufficient that $L(\phi)$ be surjective and that its kernel admit a topological supplement. In that case, the kernel $N$ of $\phi$ is a Lie subgroup of $G$ and $L(N) = \operatorname{Ker} L(\phi)$. In particular, if $H$ is the quotient Lie group of $G$ by a normal Lie subgroup $P$, $L(P)$ is an ideal of $L(G)$ and, if $\phi$ is the canonical surjection of $G$ onto $H$, $L(G/P)$ is identified with $L(G)/L(P)$ by means of the morphism derived from $L(\phi)$ when passing to the quotient.

Let $I$ be a finite set, $(G_i)_{i \in I}$ a family of Lie groups, $G$ their product and $p_i$ the canonical morphism of $G$ onto $G_i$. Then $(L(p_i))_{i \in I}$ is a morphism of the Lie algebra $L(G)$ into the Lie algebra $\prod_{i \in I} L(G_i)$ and is an isomorphism of normable spaces. $L(G)$ is therefore identified with $\prod_{i \in I} L(G_i)$ by means of $(L(p_i))_{i \in I}$.

#### Proposition 28 {#lie-iii-s3-prop-28 .statement}

Let G and H be Lie groups and φ a morphism of G into H. Suppose that K is of characteristic 0 and that H is finite-dimensional.

(i) The kernel N of φ is a Lie subgroup of G and L(N) = Ker L(φ).

(ii) The morphism ψ of G/N into H derived from φ when passing to the quotient is an immersion.

(iii) If φ(G) is closed in H and the topology of G has a countable base, φ(G) is a Lie subgroup of H, ψ is an isomorphism of the Lie group G/N onto the Lie group φ(G) and L(φ(G)) = Im L(φ).

Let G operate on H on the left by the mapping (g, h) ↦ φ(g)h. It suffices to apply Proposition 14 of § 1, no. 7, to the orbit of e.

#### Proposition 29 {#lie-iii-s3-prop-29 .statement}

Let G and H be Lie groups and φ a morphism of G into H. Suppose that K is of characteristic 0 and that H is finite-dimensional. If H' is a Lie subgroup of H, then G' = φ⁻¹(H') is a Lie subgroup of G and L(G') = L(φ)⁻¹(L(H')).

Let π be the canonical mapping of H into the homogeneous space X = H/H'. Let G operate on X on the left by the mapping (g, x) ↦ φ(g)x. The stabilizer of π(e) is G', which is therefore a Lie subgroup of G (§ 1, no. 7, Proposition 14). The orbital mapping of π(e) is π ∘ φ. By Proposition 14 of § 1, L(G') is the kernel of L(π ∘ φ) = T_e(π) ∘ L(φ). The kernel of T_e(π) is L(H') (§ 1, no. 6, Proposition 11 (i)) and hence Ker L(π ∘ φ) = L(φ)⁻¹(L(H')).

#### Corollary 1 {#lie-iii-s3-prop-29-cor-1 .statement}

Let G, H be Lie groups and φ₁ and φ₂ morphisms of G into H. Suppose that K is of characteristic 0 and that H is finite-dimensional. The set of g ∈ G such that φ₁(g) = φ₂(g) is a Lie subgroup G' of G and L(G') is the set of x ∈ L(G) such that L(φ₁)x = L(φ₂)x.

We write φ(g) = (φ₁(g), φ₂(g)) for all g ∈ G, so that φ is a morphism of G into H × H. Let Δ be the diagonal subgroup of H × H. Then G' = φ⁻¹(Δ) and L(φ)x = (L(φ₁)x, L(φ₂)x) for all x ∈ L(G). It now suffices to apply Proposition 29.

#### Corollary 2 {#lie-iii-s3-prop-29-cor-2 .statement}

Let G be a finite-dimensional Lie group and G₁ and G₂ two Lie subgroups of G. Suppose that K is of characteristic 0. Then G₁ ∩ G₂ is a Lie subgroup of G with Lie algebra L(G₁) ∩ L(G₂).

We apply Proposition 29 to the canonical injection of G₁ into G and the subgroup G₂.

#### Corollary 3 {#lie-iii-s3-prop-29-cor-3 .statement}

Let G, G', H be Lie groups and φ : G → H and φ' : G' → H Lie group morphisms. Suppose that K is of characteristic 0 and that H is finite-dimensional. Let F be the set of (g, g') ∈ G × G' such that φ(g) = φ'(g'). Then F is a Lie subgroup of G × G' and L(F) is the set of (x, x') ∈ L(G) × L(G') such that L(φ)x = L(φ')x'.

We apply Corollary 1 to the morphisms (g, g') ↦ φ(g) and (g, g') ↦ φ'(g') of G × G' into H.

#### Proposition 30 {#lie-iii-s3-prop-30 .statement}

Let G be a finite-dimensional Lie group with a countable base and

H and H' Lie subgroups of G. Suppose that K is of characteristic 0 and that HH' is locally closed in G.

(i) HH' is a submanifold of G and $T_e(HH') = L(H) + L(H')$.

(ii) Suppose that every element of H commutes with every element of H'. Then HH' is a Lie subgroup of G. Let $\phi$ be the mapping $(h, h') \mapsto hh'$ of $H \times H'$ onto HH'. The kernel of $\phi$ is the set of $(m, m^{-1})$ where $m \in H \cap H'$ and the morphism of $(H \times H')/\mathrm{Ker}\ \phi$ onto HH' derived from $\phi$ by passing to the quotient is a Lie group isomorphism.

Let $H \times H'$ operate on G on the right by the mapping $((h, h'), g) \mapsto hg{h'}^{-1}$. The orbital mapping $\rho$ of e is $(h, h') \mapsto h{h'}^{-1}$. By Proposition 14 (iii) of § 1, no. 7, HH' is a submanifold of G and $T_e(HH') = \mathrm{Im}\ T_e(\rho)$. Now

$$
T_e(\rho)(L(H) \times \{0\}) = L(H) \quad \text{and} \quad T_e(\rho)(\{0\} \times L(H')) = L(H')
$$

and hence $T_e(HH') = L(H) + L(H')$. Suppose that every element of H commutes with every element of H'. Then HH' is a subgroup of G. By (i), it is a Lie subgroup of G. The rest of the statement follows from Proposition 28.

#### Proposition 31 {#lie-iii-s3-prop-31 .statement}

Let G be a finite-dimensional Lie group with countable base, H a normal Lie subgroup of G and A a Lie subgroup of G. Suppose that K is of characteristic 0 and that AH is closed. Let $\phi$ be the canonical morphism of G onto G/H. Then the canonical mappings

$$
A/(H \cap A) \to \phi(A), \qquad AH/H \to \phi(A)
$$

are Lie group isomorphisms.

By Proposition 30, AH is a Lie subgroup of G. By Corollary 2 to Proposition 29, $H \cap A$ is a Lie subgroup of G. It is therefore meaningful to speak of the groups $AH/H$ and $A/(H \cap A)$. On the other hand, $\phi(A)$, which is the canonical image of AH in G/H, is closed and hence is a Lie subgroup of G/H (Proposition 28 (iii)). Proposition 28, applied to the composite morphisms $A \to G \to G/H$ and $AH \to G \to G/H$, proves that the canonical mappings of the proposition are Lie group isomorphisms.

#### Proposition 32 {#lie-iii-s3-prop-32 .statement}

Let G and H be Lie groups, k a non-discrete closed subfield of K and $\phi$ a morphism of G into H for the Lie group structures over k. Suppose that K is of characteristic 0. If $L(\phi)$ is K-linear, $\phi$ is a morphism for the Lie group structures over K.

For all $g \in G$,

$$
T_g(\phi) = T_e(\gamma(\phi(g))) \circ L(\phi) \circ T_g(\gamma(g)^{-1})
$$

and hence $T_g(\phi)$ is K-linear. The proposition then follows from Differentiable and Analytic Manifolds, R, 5.14.6.

### 9. LIE ALGEBRA OF THE GROUP OF INVERTIBLE ELEMENTS OF AN ALGEBRA

Let $A$ be a complete normable associative algebra with unit element $e$. Let $A^*$ be the group of invertible elements of $A$. We have seen (§ 1, no. 1) that $A^*$ is an open submanifold of $A$ and is a Lie group. Let $G$ be a Lie group and $f$ a morphism of the Lie group $G$ into the Lie group $A^*$. $f$ can be considered as an analytic mapping of $G$ into the complete normable space $A$. Hence, if $t \in \mathcal{T}^{(\infty)}(G)$, we can form $\langle t, f \rangle$, which is an element of $A$.

#### Proposition 33 {#lie-iii-s3-prop-33 .statement}

*The mapping $t \mapsto \langle t, f \rangle$ is a morphism of the algebra $\mathcal{T}^{(\infty)}(G)$ into the algebra $A$.*

It suffices to verify that, if $t$ and $t'$ are point distributions on $G$, then $\langle t * t', f \rangle = \langle t, f \rangle \langle t', f \rangle$. But
$$
\begin{align*}
\langle t * t', f \rangle &= \langle t \otimes t', (g, g') \mapsto f(gg') \rangle \\
&= \langle t \otimes t', (g, g') \mapsto f(g)f(g') \rangle \\
&= \langle t, f \rangle \langle t', f \rangle
\end{align*}
$$
*(Diff. & Anal. Man., R, 13.4.3)*.

The morphism of Proposition 33 is said to be *associated* with $f$.

Take $G$ to be the group $A^*$ itself and $f$ to be the identity mapping $i$ of $A^*$. We obtain a morphism, called *canonical*, of the algebra $\mathcal{T}^{(\infty)}(A^*)$ into the algebra $A$. The tangent space $T_e(A^*)$ is canonically identified with $A$; and if $t \in T_e(A^*)$, the definition of this identification is such that $\langle t, i \rangle = t$. Then Proposition 33 implies the following corollary:

#### Corollary {#lie-iii-s3-n9-cor-1 .statement}

*The canonical mapping $\zeta$ of $L(A^*)$ into $A$ is an isomorphism of the Lie algebra, $L(A^*)$ onto the Lie algebra $A$. In other words,
$$
\zeta([a, b]) = \zeta(a)\zeta(b) - \zeta(b)\zeta(a)
$$
for all $a, b$ in $L(A^*)$. If $K$ is of characteristic $p > 0$, then $\zeta(a^p) = \zeta(a)^p$ for all $a \in L(A^*)$.*

Henceforth $L(A^*)$ and $A$ are identified by means of the isomorphism $\zeta$.

The canonical morphism of $\mathcal{T}^{(\infty)}(A^*)$ into $A$ has been obtained as a special case of the morphism of Proposition 33. But it is possible to argue in the opposite direction:

#### Proposition 34 {#lie-iii-s3-prop-34 .statement}

*Let $H$ be a Lie group, $A$ a unital complete normable associative algebra and $\phi : H \to A^*$ a Lie group morphism. The associated morphism $\phi'$ of $\mathcal{T}^{(\infty)}(H)$ into $A$ is obtained by composing $\phi_*$ with the canonical morphism of $\mathcal{T}^{(\infty)}(A^*)$ into $A$. In particular, $\phi'(x) = L(\phi)(x)$ for all $x \in L(H)$.*

Let $i$ be the identity mapping of $A^*$ into $A$. Then, for all $t \in \mathcal{T}^{(\infty)}(H)$,
$$
\begin{align*}
\phi'(t) &= \langle t, \phi \rangle = \langle t, i \circ \phi \rangle \\
&= \langle \phi_*(t), i \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$

### 10. LIE ALGEBRAS OF CERTAIN LINEAR GROUPS

Let E be a complete normable space. Then $\mathcal{L}(E)$ is a unital complete normable algebra and $\mathbf{GL}(E)$ is a Lie group. By the Corollary to Proposition 33, no. 9, if $T_1(\mathbf{GL}(E))$ is canonically identified with $\mathcal{L}(E)$, the Lie algebra structure on $\mathbf{L}(\mathbf{GL}(E))$ is given by the bracket $(x, y) \mapsto xy - yx$ of two elements of $\mathcal{L}(E)$. In particular, $\mathbf{L}(\mathbf{GL}(n, K))$ is canonically identified with $\mathfrak{gl}(n, K)$ (Chapter I, § 1, no. 2).

#### Proposition 35 {#lie-iii-s3-prop-35 .statement}

*Let E be a finite-dimensional vector space. Let $\phi$ be the morphism $g \mapsto \det g$ of the Lie group $\mathbf{GL}(E)$ into the Lie group $K^*$. The mapping $\mathbf{L}(\phi)$ of $\mathcal{L}(E)$ into K is the mapping $x \mapsto \operatorname{Tr} x$. The kernel $\mathbf{SL}(E)$ of $\phi$ is a Lie subgroup of $\mathbf{GL}(E)$ with Lie algebra $\mathfrak{sl}(E)$.*

We choose a norm and a basis of E. The expansion of the determinant proves that
$$
\det(1 + u) \in 1 + \operatorname{Tr} u + o(\|u\|)
$$
when $u$ tends to 0 in $\mathcal{L}(E)$. Hence, using Proposition 34, no. 9, for $x \in \mathcal{L}(E) = \mathbf{L}(\mathbf{GL}(E))$:
$$
\mathbf{L}(\phi)(x) = \langle x, \phi \rangle = \operatorname{Tr} x.
$$
It follows that $\phi$ is a submersion. Therefore, $\operatorname{Ker} \phi = \mathbf{SL}(E)$ is a Lie subgroup of $\mathbf{GL}(E)$ whose Lie algebra is $\operatorname{Ker} \mathbf{L}(\phi) = \mathfrak{sl}(E)$.

Let $E_1, \ldots, E_n$ be complete normable spaces and E their direct sum. Every $x \in \mathcal{L}(E)$ can be represented by a matrix $(x_{ij})_{1 \leq i, j \leq n}$, where $x_{ij} \in \mathcal{L}(E_i, E_j)$.

#### Proposition 36 {#lie-iii-s3-prop-36 .statement}

*Let I be a subset of $\{1, 2, \ldots, n\}$ and G the subgroup of $\mathbf{GL}(E)$ consisting of the $g = (g_{ij})_{1 \leq i, j \leq n} \in \mathbf{GL}(E)$ such that $g_{ij} = 0$ for $i < j$ and $g_{ii} = 1$ for $i \in I$. Then G is a Lie subgroup of $\mathbf{GL}(E)$ and $\mathbf{L}(G)$ is the set of $x = (x_{ij})_{1 \leq i, j \leq n} \in \mathcal{L}(E)$ such that $x_{ij} = 0$ for $i < j$ and $x_{ii} = 0$ for $i \in I$.

Let S be the set of $(x_{ij}) \in \mathcal{L}(E)$ such that $x_{ij} = 0$ for $i < j$ and $x_{ii} = 0$ for $i \in I$. Then G is the intersection of $\mathbf{GL}(E)$ and the affine subspace $1 + S$ of $\mathcal{L}(E)$. Hence G is a submanifold of $\mathbf{GL}(E)$ and the tangent space to G at 1 is identified with S.*

In particular, in $\mathbf{GL}(n, K)$, the total lower triangular subgroup and the lower strict triangular subgroup, defined as in Integration, Chapter VII, § 3, no. 3, are Lie subgroups with Lie algebras $t(n, K)$ and $n(n, K)$ (Chapter I, § 1, no. 2).

#### Proposition 37 {#lie-iii-s3-prop-37 .statement}

*Let A be a complete normable unital associative algebra and $x \mapsto x^t$ a continuous linear mapping of A into A such that $(x^t)^t = x$ and $(xy)^t = y^t x^t$ for all $x, y$ in A. Suppose that K is of characteristic $\neq 2$. Let G be the subgroup of $A^*$ consisting of the $x \in A$ such that $xx^t = x^t x = 1$. Then G is a Lie subgroup of $A^*$ and $\mathbf{L}(G)$ is the set of $y \in A$ such that $y^t = -y$.*

Let S (resp. S') be the set of $y \in A$ such that $y = y^t$ (resp. $y = -y^t$). Then S, S' are closed vector subspaces of A. The formula

$$
y = \frac{1}{2}(y + y^t) + \frac{1}{2}(y - y^t)
$$

proves that A is the topological direct sum of S and S'. Let f be the mapping of A into S defined by $f(x) = xx^t$. This mapping is analytic. For all $y \in A$, $f(1 + y) = 1 + y + y^t + yy^t$; choose a norm on A compatible with its algebra structure; then

$$
f(1 + y) \in 1 + y + y^t + o(\|y\|) \quad \text{for } y \text{ tending to } 0.
$$

Thus, $T_1(f)(y) = y + y^t$, so that f is a submersion at 1. Therefore, there exists an open neighbourhood U of 1 in A such that $U \cap G$ is a submanifold of U. Hence (§ 1, no. 3, Proposition 6) G is a Lie subgroup of A*. Moreover, $L(G) = T_e(G) = \operatorname{Ker} T_1(f)$.

#### Corollary 1 {#lie-iii-s3-prop-37-cor-1 .statement}

*Suppose that K is of characteristic $\neq 2$. Let E be a finite-dimensional vector space over K and $\phi$ a non-degenerate symmetric (resp. alternating) bilinear form on E. For all $u \in \mathcal{L}(E)$, let $u^*$ be the adjoint of u relative to $\phi$. Let G be the orthogonal (resp. symplectic) group of $\phi$. Then G is a Lie subgroup of $\mathbf{GL}(E)$ and $L(G)$ is the set of $x \in \mathcal{L}(E)$ such that $x^* = -x$.

We apply Proposition 37 with $A = \mathcal{L}(E)$ and $x^t = x^*$.*

#### Remark {#lie-iii-s3-n10-rem-1 .statement}

Let B be a basis of E and J the matrix of $\phi$ with respect to B. Then $L(G)$ is the set of elements of $\mathcal{L}(E)$ whose matrix X with respect to B satisfies the equation

$$
{}^tX = -JXJ^{-1}.
$$

This follows from *Algebra*, Chapter IX, § 1, formula (50).

#### Corollary 2 {#lie-iii-s3-prop-37-cor-2 .statement}

*Let E be a complex (resp. real) Hilbert space and U the unitary group of E. Then U is a real subgroup of $\mathbf{GL}(E)$ and $L(U)$ is the set of $x \in \mathcal{L}(E)$ such that $x^* = -x$.

We apply Proposition 37 with $A = \mathcal{L}(E)$ considered as an algebra over $\mathbf{R}$ and $x^t = x^*$.*

#### Corollary 3 {#lie-iii-s3-prop-37-cor-3 .statement}

*Let E be a finite-dimensional complex vector space, $\phi$ a non-degenerate Hermitian sesquilinear form on E and U the unitary group of $\phi$. Then U is a real Lie subgroup of $\mathbf{GL}(E)$ and $L(U)$ is the set of $x \in \mathcal{L}(E)$ such that $ix$ is Hermitian.*

When $E \neq \{0\}$, U is *not* a Lie subgroup of the complex Lie group $\mathbf{GL}(E)$, for $L(U)$ is not a complex vector subspace of $\mathcal{L}(E)$.

### 11. LINEAR REPRESENTATIONS

Let G be a Lie group, E a complete normable space and $\pi$ an analytic linear representation of G on E (§ 1, no. 2). The associated morphism $t \mapsto \langle t, \pi \rangle$ of $\mathcal{T}^{(\infty)}(G)$ into $\mathcal{L}(E)$ is an algebra morphism (no. 9, Proposition 33) and its restriction to $L(G)$ is $L(\pi)$. Hence $L(\pi)$ is a representation of $L(G)$ on $E$ (Chapter I, § 3, Definition 1).

#### Proposition 38 {#lie-iii-s3-prop-38 .statement}

Consider $G$ as operating on $E$ on the left by the mapping $(g, x) \mapsto \pi(g)x$. Let $b \in E$ and $\varphi(b)$ be its orbital mapping. Let $T_b(E)$ be canonically identified with $E$. For all $t \in L(G)$,

$$
(L(\pi)t)(b) = \langle t, \varphi(b) \rangle = \varphi(b)*t = t * \varepsilon_b.
$$

In particular, the vector field defined by $t$ on $E$ is the field $b \mapsto (L(\pi)t)(b)$.

$L(\pi)t = \langle t, \pi \rangle$ (no. 9, Proposition 34). As the mapping $A \mapsto Ab$ of $\mathcal{L}(E)$ into $E$ is continuous and linear, it follows that

$$
\begin{align*}
(L(\pi)t)(b) &= \langle t, g \mapsto \pi(g)b \rangle \\
&= \langle t, \mathrm{Id}_E \circ \varphi(b) \rangle \\
&= \langle \varphi(b)*t, \mathrm{Id}_E \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \varphi(b)*t.
\end{align*}
$$

Finally, $\varphi(b)*t = t * \varepsilon_b$ (no. 3, Proposition 14 (ii)).

#### Proposition 39 {#lie-iii-s3-prop-39 .statement}

Suppose that $K$ is of characteristic 0. Let $G$ be a Lie group, $E$ a finite-dimensional vector space and $\pi$ an analytic linear representation of $G$ on $E$. Let $E_1, E_2$ be vector subspaces of $E$ such that $E_2 \subset E_1$. The set $G_1$ of $g \in G$ such that $\pi(g)x \equiv x$ (mod. $E_2$) for all $x \in E_1$ is a Lie subgroup of $G$ and $L(G_1)$ is the set of $a \in L(G)$ such that $L(\pi)a$ maps $E_1$ into $E_2$.

This follows from Propositions 29 (no. 8) and 36 (no. 10).

#### Corollary 1 {#lie-iii-s3-prop-39-cor-1 .statement}

In the notation of Proposition 39, the set of $g \in G$ such that $\pi(g)(E_1) \subset E_1$ is a Lie subgroup of $G$ and its Lie algebra is the set of $a \in L(G)$ such that $L(\pi)a$ maps $E_1$ into $E_1$.

We apply Proposition 39 with $E_1 = E_2$.

#### Corollary 2 {#lie-iii-s3-prop-39-cor-2 .statement}

Let $G, E, \pi$ be as in Proposition 39. Let $F$ be a subset of $E$. The set of $g \in G$ such that $\pi(g)x = x$ for all $x \in F$ is a Lie subgroup of $G$ and its Lie algebra is the set of $a \in L(G)$ such that $(L(\pi)a)(x) = 0$ for all $x \in F$.

We apply Proposition 39 with $E_2 = \{0\}$ and $E_1$ the vector subspace of $E$ generated by $F$.

Let $\pi_1, \pi_2, \ldots, \pi_n$ be analytic linear representations of $G$. Clearly the direct sum $\pi$ of the $\pi_i$ (Algebra, Chapter VIII, § 13, no. 1) is an analytic linear representation of $G$ and $L(\pi)$ is the direct sum of $L(\pi_1), L(\pi_2), \ldots, L(\pi_n)$ (Chapter I, § 3, no. 1).

#### Proposition 40 {#lie-iii-s3-prop-40 .statement}

Let $G$ be a Lie group, $E$ a complete normable space, $\pi$ an analytic linear representation of $G$ on $E$ and $F$ a closed vector subspace of $E$ stable under $\pi(G)$. Suppose that $K$ is of characteristic 0, or that $F$ is a direct factor of $E$.

(i) *The subrepresentation* $\pi_1$ *and the quotient representation* $\pi_2$ *of* $\pi$ *defined by* $F$ *are analytic representations*.

(ii) $F$ *is stable under* $L(\pi)(L(G))$.

(iii) *Let* $\varrho_1$ *and* $\varrho_2$ *be the subrepresentation and quotient representation of* $L(\pi)$ *defined by* $F$. *Then* $L(\pi_1) = \varrho_1, L(\pi_2) = \varrho_2$.

Let $A$ be the set of $u \in \mathcal{L}(E)$ such that $u(F) \subset F$. Then $A$ is a closed vector subspace of $\mathcal{L}(E)$ and $\pi$ takes its values in $A$. By virtue of the hypotheses on $K$ and $F$, the mapping $\pi': G \to A$ with the same graph as $\pi$ is analytic (*Differentiable and Analytic Manifolds*, R, 5.8.5). The canonical mappings $\theta_1 : A \to \mathcal{L}(F)$ and $\theta_2 : A \to \mathcal{L}(E/F)$ are continuous and linear and hence analytic. This proves (i). The mappings $T_e(\pi)$ and $T_e(\pi')$ have the same graph and hence $L(\pi)(L(G)) \subset A$, which proves (ii). We have
$$
T_e(\pi_1) = T_e(\theta_1 \circ \pi') = \theta_1 \circ T_e(\pi') = \varrho_1 \\
T_e(\pi_2) = T_e(\theta_2 \circ \pi') = \theta_2 \circ T_e(\pi') = \varrho_2.
$$

#### Proposition 41 {#lie-iii-s3-prop-41 .statement}

*Let* $G$ *be a Lie group and* $\pi_1, \pi_2, \ldots, \pi_n, \pi$ *analytic linear representation of* $G$ *on complete normable spaces* $E_1, E_2, \ldots, E_n, E$. *Let*
$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$
*be a continuous multilinear mapping of* $E_1 \times E_2 \times \cdots \times E_n$ *into* $E$. *Suppose that*
$$
\pi(g)(x_1 x_2 \ldots x_n) = (\pi_1(g)x_1)(\pi_2(g)x_2) \ldots (\pi_n(g)x_n)
$$
*for all* $g \in G, x_1 \in E_1, \ldots, x_n \in E_n$. *Then*
$$
(L(\pi)a)(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 x_2 \ldots x_{i-1} ((L(\pi_i)a)x_i) x_{i+1} \ldots x_n
$$
*for all* $a \in L(G), x_1 \in E_1, \ldots, x_n \in E_n$.

As an example we perform the calculation for $n = 2$.
$$
\begin{align*}
(L(\pi)a)(x_1 x_2) &= \langle a, g \mapsto \pi(g)(x_1 x_2) \rangle & \text{(Proposition 38)} \\
&= \langle a, (g \mapsto \pi_1(g)x_1)(g \mapsto \pi_2(g)x_2) \rangle \\
&= \langle a, g \mapsto \pi_1(g)x_1 \rangle \cdot x_2 + x_1 \cdot \langle a, g \mapsto \pi_2(g)x_2 \rangle & \text{(*Diff.* \& *Anal.* *Man.*, R, 5.5.6)} \\
&= ((L(\pi_1)a)x_1) \cdot x_2 + x_1 \cdot ((L(\pi_2)a)x_2) & \text{(Proposition 38)}.
\end{align*}
$$

#### Corollary 1 {#lie-iii-s3-prop-41-cor-1 .statement}

*Let* $G$ *be a Lie group,* $E_1, \ldots, E_{n+1}$ *complete normable spaces and* $\pi_1, \ldots, \pi_{n+1}$ *analytic linear representations of* $G$ *on* $E_1, \ldots, E_{n+1}$. *Let*
$$
E = \mathcal{L}(E_1, \ldots, E_n; E_{n+1})
$$
*the complete normable space of continuous multilinear mappings of* $E_1 \times \cdots \times E_n$ *into* $E_{n+1}$ *(General Topology, Chapter X, § 3, no. 2)*. *For all* $g \in G$, *let* $\pi(g)$ *be the automorphism of* $E$ *defined by*
$$
(\pi(g)u)(x_1, \ldots, x_n) = \pi_{n+1}(g)(u(\pi_1(g)^{-1}x_1, \ldots, \pi_n(g)^{-1}x_n)).
$$

Then $\pi$ is an analytic linear representation of $G$ on $E$ and
$$
((L(\pi)a)u)(x_1, \ldots, x_n) = -\sum_{i=1}^n u(x_1, \ldots, x_{i-1}, (L(\pi_i)a)x_i, x_{i+1}, \ldots, x_n)
$$
$$
\quad + (L(\pi_{n+1})a)(u(x_1, \ldots, x_n))
$$
for all $a \in L(G)$, $u \in E$, $x_1 \in E_1, \ldots, x_n \in E_n$.

Every element $(A_1, \ldots, A_{n+1})$ of $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ defines a continuous endomorphism $\theta(A_1, \ldots, A_{n+1})$ of $E$ by the formula
$$
(\theta(A_1, \ldots, A_{n+1})u)(x_1, \ldots, x_n) = A_{n+1}(u(A_1x_1, \ldots, A_nx_n)).
$$
The mapping $\theta$ of $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ into $\mathcal{L}(E)$ is continuous and multilinear. Then, for all $g \in G$,
$$
\pi(g) = \theta(\pi_1(g^{-1}), \ldots, \pi_n(g^{-1}), \pi_{n+1}(g))
$$
and hence $\pi$ is analytic. We apply Proposition 41 to the mapping
$$
(x_1, \ldots, x_n, u) \mapsto u(x_1, \ldots, x_n)
$$
of $E_1 \times \cdots \times E_n \times E$ into $E_{n+1}$. Then
$$
\pi_{n+1}(g)(u(x_1, \ldots, x_n)) = (\pi(g)u)(\pi_1(g)x_1, \ldots, \pi_n(g)x_n)
$$
and hence
$$
(L(\pi_{n+1})a)(u(x_1, \ldots, x_n)) = \sum_{i=1}^n u(x_1, \ldots, (L(\pi_i)a)x_i, \ldots, x_n)
$$
$$
\quad + ((L(\pi)a)u)(x_1, \ldots, x_n).
$$

When the $E_i$ are finite-dimensional, the representation $L(\pi)$ of $L(G)$ is derived from the representations $L(\pi_1), \ldots, L(\pi_{n+1})$ under the procedure of Chapter I, § 3, Proposition 3.

#### Corollary 2 {#lie-iii-s3-prop-41-cor-2 .statement}

Let $G$ be a Lie group and $\pi$ an analytic linear representation of $G$ on a complete normable space $E$. Then $g \mapsto {}^t\pi(g)^{-1}$ is an analytic linear representation $\rho$ of $G$ on the complete normable space $\mathcal{L}(E, K)$\footnote{As when $K = \mathbf{R}$ or $\mathbf{C}$, the transpose ${}^t\pi(g)$ considered here is the restriction to $\mathcal{L}(E, K)$ of the transpose of $\pi(g)$ in the purely algebraic sense.} and $L(\rho)a = -{}^t(L(\pi)a)$ for all $a \in L(G)$.

This is a special case of Corollary 1.

$\rho$ is called the *contragredient* representation of $\pi$.

When $E$ is finite-dimensional, $L(\rho)$ is the dual representation of $L(\pi)$ in the sense of Chapter I, § 3, no. 3.

#### Corollary 3 {#lie-iii-s3-prop-41-cor-3 .statement}

Let $G$ be a Lie group and $\pi_1, \ldots, \pi_n$ analytic linear representations of $G$ on finite-dimensional vector spaces $E_1, \ldots, E_n$. Then the representation $\pi_1 \otimes \cdots \otimes \pi_n$ of $G$ (Appendix) is analytic and $L(\pi_1 \otimes \cdots \otimes \pi_n)$ is the tensor product of $L(\pi_1), \ldots, L(\pi_n)$.

The mapping $(A_1, \ldots, A_n) \mapsto A_1 \otimes \cdots \otimes A_n$ of $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_n)$ into $\mathcal{L}(E_1 \otimes \cdots \otimes E_n)$ is multilinear, whence the fact that $\pi$ is analytic. Consider the mapping $(x_1, \ldots, x_n) \mapsto x_1 \otimes \cdots \otimes x_n$ of $E_1 \times \cdots \times E_n$ into
$$
E_1 \otimes \cdots \otimes E_n.
$$
By Proposition 41, we see that
$$
(L(\pi)a)(x_1 \otimes \cdots \otimes x_n) = \sum_{i=1}^n x_1 \otimes \cdots \otimes (L(\pi_i)a)x_i \otimes \cdots \otimes x_n
$$
for all $a \in L(G)$, $x_i \in E_i$ for $1 \leq i \leq n$. Hence $L(\pi)$ is the tensor product of the $L(\pi_i)$.

#### Corollary 4 {#lie-iii-s3-prop-41-cor-4 .statement}

Let $G$ be a Lie group and $\pi$ an analytic linear representation of $G$ on a finite-dimensional vector space $E$. Then the representations $T^n(\pi)$, $S^n(\pi)$ and $\wedge^n(\pi)$ of $G$ (Appendix) are analytic and
$$
L(T^n(\pi)) = T^n(L(\pi)), \quad L(S^n(\pi)) = S^n(L(\pi)), \quad L(\wedge^n(\pi)) = \wedge^n(L(\pi)).
$$
This follows from Corollary 3 and Proposition 40.

#### Corollary 5 {#lie-iii-s3-prop-41-cor-5 .statement}

Let $A$ be a finite-dimensional algebra. Suppose that $K$ is of characteristic 0. The automorphism group $\mathrm{Aut}(A)$ of $A$ is a Lie subgroup of $\mathbf{GL}(A)$ and $L(\mathrm{Aut}(A))$ is the Lie algebra of derivation of $A$.

This follows from Corollary 1 (applied to $E = \mathcal{L}(A, A; A)$) and Corollary 2 of Proposition 39 (applied to the subset of $E$ consisting only of multiplication on $A$).

#### Remark {#lie-iii-s3-n11-rem-1 .statement}

We apply Corollary 1 with $G = \mathbf{GL}(F)$ ($F$ a complete normable space), $\pi_1 = \pi_2 = \mathrm{Id}_G$ and $\pi_3$ the trivial representation of $G$ on $K$. We obtain an analytic representation $\pi$ of $\mathbf{GL}(F)$ on $\mathcal{L}(F, F; K)$. We assume that $F$ is finite-dimensional and that $K$ is of characteristic 0. Applying Corollary 2 to Proposition 39 to $\pi$, we recover part of Corollary 1 to Proposition 37.

#### Proposition 42 {#lie-iii-s3-prop-42 .statement}

Let $G$ be a Lie group, $X$ an analytic manifold, $(g, x) \mapsto gx$ (resp. $xg$) a law of analytic left (resp. right) operation of $G$ on $X$ and $x_0$ a point of $X$ which is invariant under $G$. For all $g \in G$, let $\tau(g)$ be the automorphism $x \mapsto gx$ (resp. $xg$) of $X$ and let $\pi(g)$ be the automorphism of $T_{x_0}(X)$ tangent at $x_0$ to $\tau(g)$.
(i) $\pi$ is an analytic representation of $G$ (resp. $G^\vee$) on $T_{x_0}(X)$.
(ii) For all $a \in L(G)$ and all $\xi_0 \in T_{x_0}(X)$, $L(\pi)a.\xi_0$ can be calculated as follows: let $D_a$ be the vector field defined by $a$ on $X$ and $\xi$ a vector field of class $C^1$ in an open neighbourhood of $x_0$ such that $\xi(x_0) = \xi_0$; then
$$
L(\pi)a.\xi_0 = -[D_a, \xi](x_0).
$$

$\tau(gg') = \tau(g)\tau(g')$ (resp. $\tau(g')\tau(g)$) and hence $\pi(gg') = \pi(g)\pi(g')$ (resp. $\pi(g')\pi(g)$). On the other hand, since $TX$ is a vector G-bundle of class $C^\omega$ (§ 1, no. 8, Proposition 16), $\pi$ is analytic, whence (i).

To prove (ii), suppose that G operates on the left. There exists an open neighbourhood I of 0 in K and an analytic mapping $\gamma$ of I into G such that $\gamma(0) = e, T_0(\gamma)1 = a$. Then $D_a$ is the vector field on X defined by the mapping $\phi : (\lambda, x) \mapsto \gamma(\lambda)x$ of $I \times X$ into X (§ 2, no. 2). If $\phi_\lambda$ denotes the bijection $x \mapsto \gamma(\lambda)x$ of X into X, then

$$
[D_a, \xi](x_0) = \left( \frac{d}{d\lambda} (T_{\phi_\lambda(x_0)}(\phi_\lambda^{-1})\xi(\phi_\lambda(x_0))) \right)_{\lambda=0} \quad (\text{Diff. \& Anal. Man., R,}
$$
$$
= \left( \frac{d}{d\lambda} (T_{x_0}(\phi_\lambda^{-1})\xi_0) \right)_{\lambda=0}
$$
$$
= \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))^{-1}\xi_0) \right)_{\lambda=0}.
$$

As the mappings $\lambda \mapsto \gamma(\lambda)^{-1}$ and $\lambda \mapsto \gamma(-\lambda)$ are tangent at 0, this is also equal to
$$
- \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))\xi_0) \right)_{\lambda=0}
$$
$$
= - \left( \frac{d}{d\lambda} (\pi \circ \gamma)(\lambda) \right)_{\lambda=0} \xi_0
$$
$$
= -L(\pi)a.\xi_0.
$$

### 12. ADJOINT REPRESENTATION

Let G be a Lie group. Consider the law of analytic left operation
$$
(g, g') \mapsto gg'g^{-1} = (\operatorname{Int} g)g'
$$
of G into G. This law of operation defines, by no. 3, a bilinear mapping of $\mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G)$ into $\mathcal{T}^{(\infty)}(G)$, which we shall denote by $\tau$ in this no. By Proposition 13 of no. 3,
$$
(t * t') \tau t'' = t \tau (t' \tau t'')
$$
for all $t, t', t''$ in $\mathcal{T}^{(\infty)}(G)$. By Proposition 14 (i) of no. 3,
$$
\varepsilon_g \tau t = (\operatorname{Int} g)_*t
$$
for all $g \in G$ and $t \in \mathcal{T}^{(\infty)}(G)$. In particular, the mapping $t \mapsto \varepsilon_g \tau t$ of $\mathcal{T}^{(\infty)}(G)$ into $\mathcal{T}^{(\infty)}(G)$ is an automorphism of the bigebra $\mathcal{T}^{(\infty)}(G)$. Its restrictions to $U(G), U_s(G), L(G)$ are denoted by $\operatorname{Ad}_{U(G)}(g), \operatorname{Ad}_{U_s(G)}(g), \operatorname{Ad}_{L(G)}(g)$. We often write $\operatorname{Ad}(g)$ instead of $\operatorname{Ad}_{L(G)}(g)$ when no confusion is possible. By (23), $\operatorname{Ad}(g)$ is the tangent mapping at e to $\operatorname{Int}(g)$. It is an automorphism of the normable

Lie algebra $\mathbf{L}(G)$. When $K$ is of characteristic 0, $\mathrm{Ad}_{\mathbf{U}(G)}(g)$ is the unique automorphism of $\mathbf{U}(G)$ which extends $\mathrm{Ad}(g)$.

If $\phi$ is a morphism of the Lie group $G$ into a Lie group $H$, then
$$
\phi_*(t \top t') = \phi_*(t) \top \phi_*(t')
$$
for all $t, t'$ in $\mathcal{T}^{(\infty)}(G)$; this follows from Proposition 15 of no. 3.

#### Proposition 43 {#lie-iii-s3-prop-43 .statement}

*Let $t, u$ be in $\mathcal{T}^{(\infty)}(G)$. Let $\sum_{i=1}^n t_i \otimes t'_i$ be the image of $t$ under the coproduct. Then*
$$
t \top u = \sum_{i=1}^n t_i * u * {t'_i}^\vee.
$$

By definition, $t \top u$ is the image of $t \otimes u$ under the mapping $(g, g') \mapsto gg'g^{-1}$ of $G \times G$ into $G$. Now this mapping is obtained by composing the following mappings:
$$
\begin{aligned}
\alpha & : (g, g') \mapsto (g, g, g') & \text{of } G \times G \text{ into } G \times G \times G \\
\beta & : (g, g', g'') \mapsto (g, {g'}^{-1}, g'') & \text{of } G \times G \times G \text{ into } G \times G \times G \\
\gamma & : (g, g', g'') \mapsto gg''g' & \text{of } G \times G \times G \text{ into } G.
\end{aligned}
$$

On the other hand:
$$
\begin{aligned}
\alpha_*(t \otimes u) &= \sum_{i=1}^n (t_i \otimes t'_i) \otimes u = \sum_{i=1}^n t_i \otimes t'_i \otimes u \\
\beta_* \left( \sum_{i=1}^n t_i \otimes t'_i \otimes u \right) &= \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \\
\gamma_* \left( \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \right) &= \sum_{i=1}^n t_i * u * {t'_i}^\vee.
\end{aligned}
$$

#### Corollary 1 {#lie-iii-s3-prop-43-cor-1 .statement}

*Let $u \in \mathbf{L}(G)$ and $u' \in \mathcal{T}^{(\infty)}(G)$. Then $u \top u' = u * u' - u' * u$.*

The image of $u$ under the coproduct is $u \otimes \varepsilon_e + \varepsilon_e \otimes u$, whence
$$
u \top u' = u * u' * \varepsilon_e + \varepsilon_e * u' * u^\vee = u * u' - u' * u.
$$

#### Corollary 2 {#lie-iii-s3-prop-43-cor-2 .statement}

*Let $t \in \mathcal{T}^{(\infty)}(G)$ and $g \in G$. Then $\varepsilon_g \top t = \varepsilon_g * t * \varepsilon_{g^{-1}}$. If $t \in \mathbf{L}(G)$, then $\varepsilon_g \top t = gtg^{-1}$ (where the latter product is evaluated in the group $\mathbf{T}(G)$).*

The image of $\varepsilon_g$ under the coproduct is $\varepsilon_g \otimes \varepsilon_g$.

#### Corollary 3 {#lie-iii-s3-prop-43-cor-3 .statement}

*Let $a \in \mathbf{L}(G)$. The vector field defined by $a$ and the left operation $g \mapsto \mathrm{Int}\, g$ of $G$ on $G$ is the field $\mathbf{R}_a - \mathbf{L}_a$.*

The value of this field at $g$ is
$$
\begin{aligned}
a \top \varepsilon_g &= a * \varepsilon_g - \varepsilon_g * a & \text{(Corollary 1)} \\
&= (\mathbf{R}_a)_g - (\mathbf{L}_a)_g & \text{(Definition 5)}.
\end{aligned}
$$

For all $g \in G$ and all $t \in L(G)$,
$$
(\mathrm{Ad}\,g)(t) = \varepsilon_g \top t = \varepsilon_g * t * \varepsilon_g^{-1} = gtg^{-1}.
$$
Since $\mathrm{Ad}\,g = T_e(\mathrm{Int}\,g)$, Proposition 42 of no. 11 proves that $\mathrm{Ad}$ is an analytic linear representation of $G$ on the normable space $L(G)$.

#### Definition 8 {#lie-iii-s3-def-8 .statement}

*The representation Ad of G on L(G) is called the adjoint representation of G.*

#### Proposition 44 {#lie-iii-s3-prop-44 .statement}

*For all $a \in L(G)$,*
$$
(L(\mathrm{Ad}))(a) = \mathrm{ad}_{L(G)}a.
$$
Let $b \in L(G)$. By Proposition 42 (ii) of no. 11 and Corollary 3 to Proposition 43,
$$
(L(\mathrm{Ad}))(a).b = -[R_a - L_{a_1}L_b](e).
$$
Now $R_a \circ L_b = L_b \circ R_a$ (no. 6, Proposition 23 (ii)), whence $[R_a, L_b] = 0$; then, using Proposition 23 (ii),
$$
(L(\mathrm{Ad}))(a).b = [L_a, L_b](e) = L_{[a, b]}(e) = [a, b] = (\mathrm{ad}_{L(G)}a)b.
$$

#### Proposition 45 {#lie-iii-s3-prop-45 .statement}

*Suppose that G is finite-dimensional and that K is of characteristic 0. Let s be an integer $\geqslant 0$. Then the mapping $\pi : g \mapsto \mathrm{Ad}_{U_s(G)}(g)$ is an analytic linear representation of G on $U_s(G)$ and $L(\pi)a = \mathrm{ad}_{U_s(G)}a$ for all $a \in L(G)$.*

The linear representation $\pi$ is a quotient of $\bigoplus_{r=0}^s \mathrm{Tr}(\mathrm{Ad})$ and is hence analytic. For $a \in L(G)$ and $x_1, x_2, \ldots, x_s$ in $L(G)$,
$$
\begin{align*}
(L(\pi)a)(x_1x_2\ldots x_s) &= \sum_{i=1}^s x_1 \ldots (L(\mathrm{Ad})a.x_i) \ldots x_s & \text{(Proposition 41)} \\
&= \sum_{i=1}^s x_1 \ldots ([a, x_i]) \ldots x_s & \text{(Proposition 44)} \\
&= (\mathrm{Ad}_{U_s(G)}a)(x_1x_2\ldots x_s).
\end{align*}
$$

#### Proposition 46 {#lie-iii-s3-prop-46 .statement}

*Let $h \in G, x \in T_h(G)$ and $a \in L(G)$. Let $\phi$ be the mapping $(g, g') \mapsto gg'g^{-1}$ of $G \times G$ into $G$. The image y of $(a, x) \in T_e(G) \times T_h(G)$ under $T_{(e, h)}(\phi)$ is $y = x + h((\mathrm{Ad}\,h^{-1})a - a)$.
We have*
$$
\begin{align*}
y &= (T_{(e, h)}\phi)(a \otimes \varepsilon_h + \varepsilon_e \otimes x) \\
&= a \top \varepsilon_h + \varepsilon_e \top x \\
&= a * \varepsilon_h - \varepsilon_h * a + x \\
&= h((\mathrm{Ad}\,h^{-1})a) - ha + x.
\end{align*}
$$

#### Proposition 47 {#lie-iii-s3-prop-47 .statement}

Let G be a Lie group, H and E Lie subgroups of G and suppose that hEh$^{-1}$ = E for all h \in H. Then $\mathcal{T}^{(\infty)}(H) \subset \mathcal{T}^{(\infty)}(E) \subset \mathcal{T}^{(\infty)}(E)$. In particular, $\mathrm{Ad}(H)(L(E)) \subset L(E)$ and $[L(H), L(E)] \subset L(E)$.

If $t \in \mathcal{T}^{(\infty)}(H)$ and $t' \in \mathcal{T}^{(\infty)}(E)$, then $t \otimes t' \in \mathcal{T}^{(\infty)}(H \times E)$ and the image of $H \times E$ under the mapping $(g, g') \mapsto gg'g^{-1}$ is contained in E.

#### Proposition 48 {#lie-iii-s3-prop-48 .statement}

Let G be a Lie group and H and E Lie subgroups of G. Suppose that G is, as a Lie group, the semi-direct product of H by E. Let $\varphi$ be the linear representation $g \mapsto (\mathrm{Ad}\, g) \mid L(E)$ of the Lie group G on $L(E)$ (cf. Proposition 47) and let $\sigma$ be the restriction of $\varphi$ to H. Then:
(i) $L(G)$ is the topological direct sum of $L(H)$ and $L(E)$;
(ii) $L(H)$ is a subalgebra of $L(G)$ and $L(E)$ is an ideal of $L(G)$;
(iii) $L(\sigma)$ is a linear representation of $L(H)$ on the Lie algebra of derivations of $L(E)$;
(iv) $L(G)$ is the semi-direct product of $L(H)$ by $L(E)$ defined by $L(\sigma)$ (Chapter I, § 1, no. 8).

(i) is obvious and (ii) follows from Proposition 47. $L(\sigma) = L(\varphi) \mid L(H)$. Now by Propositions 40 (no. 11) and 44 (no. 12), $L(\varphi)(t)$ is, for all $t \in L(G)$, the restriction of $\mathrm{ad}_{L(G)} t$ to $L(E)$. This proves (iii). Using (i) and (ii), this also proves (iv).

#### Corollary {#lie-iii-s3-n12-cor-1 .statement}

Let G be a Lie group. Let $T_e(G)$ be given its unique commutative Lie algebra structure. Let $\tau$ be an adjoint representation of $L(G)$. Then the Lie algebra of $T(G)$ is the semi-direct product of $L(G)$ by $T_e(G)$ defined by $\tau$. In other words, for $x, x'$ in $L(G)$ and $y, y'$ in $T_e(G)$,

$$
[(x, y), (x', y')] = ([x, x'], [x, y'] + [y, x'])
$$

(where the bracket on the left is evaluated in $L(T(G))$ and the brackets on the right in $L(G)$).

This follows from Proposition 48 and Proposition 6 of § 2, no. 2.

#### Proposition 49 {#lie-iii-s3-prop-49 .statement}

Let A be a complete normable unital associative algebra. We identify A with $L(A^*)$. Then, if $g \in A^*$ and $y \in A$, $(\mathrm{Ad}\, g)y = gyg^{-1}$.

Recall that $\mathrm{Ad}\, g = T_1(\mathrm{Int}\, g)$. Let $u_g$ be the mapping $x \mapsto gxg^{-1}$ of A into A. The identity chart of $A^*$ into A transforms $\mathrm{Int}\, g$ into $u_g \mid A^*$. The tangent mapping at each point of $A^*$ to this mapping is equal to $u_g$, whence the proposition.

#### Corollary {#lie-iii-s3-n12-cor-2 .statement}

For all $g \in A^*$, let $i(g)$ be the automorphism $y \mapsto gyg^{-1}$ of A, so that $i$ is an analytic linear representation of $A^*$ on A. For all $z \in L(A^*) = A, L(i)z$ is the inner derivation $y \mapsto zy - yz$ of A.

This follows from Propositions 49 and 44.

### 13. TENSORS AND INVARIANT FORMS

Let G be a Lie group. We consider G as operating on itself by left (resp. right) translation. Let $\lambda$ be a vector functor of class $C^\omega$ for isomorphisms. Then $\lambda(\mathrm{TG})$ is an analytic left (resp. right) vector G-bundle (§ 1, no. 8, Corollary to Proposition 16). The mapping $(g, u) \mapsto gu$ (resp. $ug$) of $G \times \lambda(\mathrm{L}(G))$ onto $\lambda(\mathrm{TG})$ is an isomorphism $\phi$ (resp. $\psi$) of vector G-bundles (§ 7, no. 8, Corollary 2 to Proposition 17). Every G-invariant section of $\lambda(\mathrm{TG})$ is analytic and determined by its value at $e$ (§ 1, no. 8, Corollary 1 to Proposition 17). Such a section is called *left* (resp. *right*) *invariant*. Let $\sigma$ be a left invariant section of $\lambda(\mathrm{TG})$; the transform $\sigma'$ of $\sigma$ under a right translation $\delta(g)$ is defined by $\sigma'(\delta(g)h) = \lambda(\mathrm{T}_h(\delta(g)))\sigma(h)$ for all $h \in G$; it is also left invariant; it is also derived from $\sigma$ by $\gamma(g) \circ \delta(g) = \mathrm{Int}(g)$ and hence

$$
\sigma'(e) = \lambda(\mathrm{Ad}\ g)\cdot \sigma(e).
$$

Similarly, let $\tau$ be a right invariant section of $\lambda(\mathrm{TG})$; the transform $\tau'$ of $\tau$ under a left translation $\gamma(g)$ is also right variant and

$$
\tau'(e) = \lambda(\mathrm{Ad}\ g)\cdot \tau(e).
$$

We now consider $G \times G$ as operating on $G$ on the left by

$$
((g, g'), g'') \mapsto gg''{g'}^{-1}.
$$

Then G is a left Lie homogeneous space of $G \times G$ (§ 1, no. 6, *Example*). Hence $\lambda(\mathrm{TG})$ is an analytic left vector $(G \times G)$-bundle. A section of $\lambda(\mathrm{TG})$ is called *biinvariant* if it is invariant under the action of $G \times G$ on $\lambda(\mathrm{TG})$, in other words if it is invariant under left and right translations. Let $\lambda(\mathrm{L}(G))_0$ be the set of elements of $\lambda(\mathrm{L}(G))$ invariant under $\lambda(\mathrm{Ad}(G))$. For all $u \in \lambda(\mathrm{L}(G))_0$, let $\sigma_u$ be the mapping of $G$ into $\lambda(\mathrm{TG})$ defined by $\sigma_u(g) = gu = ug$. Then $u \mapsto \sigma_u$ is a bijection of $\lambda(\mathrm{L}(G))_0$ onto the set of biinvariant sections of $\lambda(\mathrm{TG})$ (§ 1, no. 8, Corollary 1 to Proposition 17).

#### Proposition 50 {#lie-iii-s3-prop-50 .statement}

*Let G be a Lie Group (assumed to be finite-dimensional if K is of characteristic > 0). Let E be the vector space of continuous alternating multilinear forms of degree k on $\mathrm{T}_e(G)$. For all $u \in E$, let $\omega^u$ be the differential form of degree k on G such that $(\omega^u)_g$ is the multilinear form on $\mathrm{T}_g(G)$ derived from u by the translation $h \mapsto gh$ (resp. $h \mapsto hg$). Then $\omega^u$ is analytic and left (resp. right) invariant on G. The mapping $u \mapsto \omega^u$ is an isomorphism of E onto the vector space of left (resp. right) invariant differential forms of degree k on G.*

This is a special case of what we have said above.

Let F be a complete normable space. Proposition 50 remains true if differential forms on G with values in K are replaced by differential forms on G with values in F. For every continuous linear mapping $u$ of $\mathrm{T}_e(G)$ into F, there exists a differential form $\omega^u$ of degree 1 on G, with values in F, such that $(\omega^u)_g = u \circ \mathrm{T}_g(\gamma(g)^{-1})$. In particular, take $F = \mathrm{T}_e(G)$ and $u = \mathrm{Id}_{\mathrm{T}_e(G)}$. We then obtain the differential form $\omega$ on $G$ such that $\omega_g = T_g(\gamma(g^{-1}))$; this differential form is left invariant and analytic; it is called the *left canonical differential form* of $G$. $\omega_g(t) = g^{-1}t$ for all $t \in T_g(G)$.

If $F$ is again an arbitrary complete normable space and $u \in \mathcal{L}(T_e(G), F)$, then $\omega^u = u \circ \omega$. In particular (taking $F = K$), the mapping $v \mapsto v \circ \omega$ is a linear bijection of the dual of $T_e(G)$ onto the vector space of differential forms of degree 1 with values in $K$ which are left invariant under $G$.

Similarly, the differential form $\omega'$ on $G$ such that $\omega'_g = T_g(\delta(g))$ is called the *right canonical differential form* of $G$. There are analogous properties to those of $\omega$, which we leave to the reader to state. The mapping $g \mapsto g^{-1}$ of $G$ onto $G$ transforms $\omega$ into $\omega'$.

### 14. MAURER–CARTAN FORMULAE

Let $X$ be a manifold of class $C^r$, of finite dimension if $K$ is of characteristic $> 0$, and let $L$ be a complete normable Lie algebra. Let $\alpha$ be a differential form of degree 1 on $X$ with values in $L$ of class $C^{r-1}$. Let $x \in X$. The mapping

$$
(u_1, u_2) \mapsto [\alpha_x(u_1), \alpha_x(u_2)]
$$

of $T_x(X) \times T_x(X)$ into $L$ is a continuous alternating bilinear form on $T_x(X)$ with values in $L$. We shall denote it by $[\alpha]^2_x$, so that $[\alpha]^2$ is a differential form of degree 2 on $X$ with values in $L$. Identifying an open neighbourhood of $x$ in $X$ with an open subset of a Banach space, we see immediately that $[\alpha]^2$ is of class $C^{r-1}$. If $X'$ is a manifold of class $C^r$ and $f : X' \to X$ is a morphism, then

$$
[f^*(\alpha)]^2 = f([\alpha]^2).
$$

Let $\alpha, \beta$ be two differential forms of degree 1 on $X$ with values in $L$ of class $C^{r-1}$. The exterior product $\alpha \wedge \beta$ of $\alpha$ and $\beta$ (*Differentiable and Analytic Manifolds*, R, 7.8.2) is a differential form of degree 2 on $X$ with values in $L$ of class $C^{r-1}$; we have

$$
(\alpha \wedge \beta)_x(u_1, u_2) = [\alpha_x(u_1), \beta_x(u_2)] - [\alpha_x(u_2), \beta_x(u_1)]
$$

for $u_1, u_2$ in $T_x(X)$. It is immediate that

$$
[\alpha + \beta]^2 = [\alpha]^2 + [\beta]^2 + \alpha \wedge \beta
$$
$$
\alpha \wedge \alpha = 2[\alpha]^2.
$$

#### Proposition 51 {#lie-iii-s3-prop-51 .statement}

*Let $G$ be a Lie group, of finite dimension if $K$ is of characteristic $> 0$, and let $a_1, \ldots, a_p$ be elements of $L(G)$, $F$ a complete normable space and $\alpha$ a differential form of degree $p-1$ on $G$ with values in $F$. If $\alpha$ is left invariant, then*

$$
(d\alpha)_e(a_1, \ldots, a_p) = \sum_{i<j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$

If $\alpha$ is right invariant, then
$$
(d\alpha)_e(a_1, \ldots, a_p)
= - \sum_{i < j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$
Suppose that $\alpha$ is left invariant. By *Differentiable and Analytic Manifolds*, R, 8.5.7, then
$$
(d\alpha)(L_{a_1}, \ldots, L_{a_p}) = \sum_i (-1)^{i-1} L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})
+ \sum_{i < j} (-1)^{i+j} \alpha([L_{a_i}, L_{a_j}], L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_{j-1}}, L_{a_{j+1}}, \ldots, L_{a_p}).
$$
But the functions $\alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})$ on G are left invariant and therefore constant. Hence
$$
L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p}) = 0.
$$
Moreover, $[L_{a_i}, L_{a_j}] = L_{[a_i, a_j]}$ (Proposition 23), whence the first formula of Proposition 51. The second can be established analogously, this time using the relation $[R_{a_i}, R_{a_j}] = -R_{[a_i, a_j]}$.

#### Corollary 1 {#lie-iii-s3-prop-51-cor-1 .statement}

*Let G be a Lie group, of finite dimension if K is of characteristic > 0, and $\omega$ and $\omega'$ the left and right canonical differential forms of G. Then*
$$
d\omega + [\omega]^2 = 0, \qquad d\omega' - [\omega']^2 = 0.
$$
By Proposition 51,
$$
(d\omega)_e(a_1, a_2) = -\omega_e([a_1, a_2]) = -[a_1, a_2] = -[\omega_e(a_1), \omega_e(a_2)]
= -[\omega]^2_e(a_1, a_2)
$$
whence the first formula. The second can be established analogously.

#### Corollary 2 {#lie-iii-s3-prop-51-cor-2 .statement}

*Suppose that G is finite-dimensional. Let $(e_1, \ldots, e_n)$ be a basis of $L(G)$, $(e_1^*, \ldots, e_n^*)$ the dual basis, $(c_{ijk})$ the constants of structure of $L(G)$ relative to the basis $(e_1, \ldots, e_n)$ and $\omega_i$ (resp. $\omega'_i$) the left (resp. right) invariant differential form on G with values in K such that $(\omega_i)_e = e_i^*$ (resp. $(\omega'_i)_e = e_i^*$). Then*
$$
d\omega_k + \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j = 0 \quad (k = 1, 2, \ldots, n)
$$
$$
d\omega'_k - \sum_{i < j} c_{ijk} \omega'_i \wedge \omega'_j = 0 \quad (k = 1, 2, \ldots, n).
$$
If $r < s$,
$$
(d\omega_k)_e(e_r, e_s) = -(\omega_k)_e([e_r, e_s])
= -\sum_i c_{rsi} (\omega_k)_e(e_i)
= -c_{rsk}
= -\sum_{i < j} c_{ijk} (\omega_i \wedge \omega_j)_e(e_r, e_s).
$$
The argument is similar for the $\omega'_k$.

### 15. CONSTRUCTION OF INVARIANT DIFFERENTIAL FORMS

#### Lemma 2 {#lie-iii-s3-lem-2 .statement}

Let G be a Lie group, U a symmetric open neighbourhood of e in G, E a complete normable space and $\phi : U^2 \to E$ an analytic mapping. For all $g \in U$, let $\omega_g$ be the differential at the point g of the mapping $h \mapsto \phi(g^{-1}h)$. Then $\omega$ is the restriction to U of the left invariant differential form on G whose value at e is $d_e \phi$.

Clearly $\omega_e = d_e \phi$. For all $g \in U$ and all $t \in T_e(G)$,

$$
\langle \omega_g, T_e(\gamma(g))t \rangle = \langle d_g(\phi \circ \gamma(g)^{-1}), T_e(\gamma(g))t \rangle \\
= \langle d_e \phi \circ T_g(\gamma(g)^{-1}), T_e(\gamma(g))t \rangle = \langle d_e \phi, t \rangle
$$

and hence $\omega_g$ is derived from $d_e \phi$ by $T_e(\gamma(g))$.

#### Proposition 52 {#lie-iii-s3-prop-52 .statement}

Let n be an integer > 0, G an n-dimensional Lie group, U a symmetric open neighbourhood of e in G and $\psi : U^2 \to K^n$ a chart of G such that $\psi(e) = 0$. If $(x_1, \ldots, x_n)$ are the coordinates of $x \in \psi(U)$ and $(y_1, \ldots, y_n)$ the coordinates of $y \in \psi(U)$, we denote by

$$
m_1(x_1, \ldots, x_n, y_1, \ldots, y_n), \ldots, m_n(x_1, \ldots, x_n, y_1, \ldots, y_n)
$$

the coordinates of $\psi(\psi^{-1}(x)^{-1}\psi^{-1}(y))$. Then, if we write, for $1 \leq k \leq n$,

$$
\varpi_k(x_1, \ldots, x_n) = D_{n+1} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_1 + \cdots \\
+ D_{2n} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_n,
$$

the differential forms $\varpi_k$ on $\psi(U)$ are derived through $\psi$ from left invariant differential forms on G and are such that $\varpi_k(0, \ldots, 0) = dx_k$.

We apply Lemma 2 with $E = K$, taking $\phi(g)$ to be the coordinate of $\psi(g)$ of index k. We obtain a differential form $\omega_k$; let $\varpi_k$ be its transform under $\psi$. The value of $\varpi_k$ at $(x_1, \ldots, x_n)$ is the differential at $(x_1, \ldots, x_n)$ of the function $y \mapsto m_k(x_1, \ldots, x_n, y_1, \ldots, y_n)$; this value is therefore given by formula (32). It then suffices to use the conclusion to Lemma 2.

#### Proposition 53 {#lie-iii-s3-prop-53 .statement}

Let G be a Lie group, A a complete normable algebra and $\phi$ a Lie group morphism of G into $A^*$. For all $g \in G$, let $\omega_g = \phi(g)^{-1} d_g \phi$. Then $\omega$ is the left invariant differential form on G whose value at e is $d_e \phi$.

We apply Lemma 2 with $E = A$ and $U = G$. The differential at g of the mapping $h \mapsto \phi(g^{-1}h) = \phi(g)^{-1} \phi(h)$ is $\phi(g)^{-1} d_g \phi$.

### 16. HAAR MEASURE ON A LIE GROUP

Let G be a Lie group of finite dimension n. Then $\bigwedge^n(T_e(G))$ is of dimension 1. Hence (no. 13) the vector space S of left invariant differential forms of degree n on G is of dimension 1. Let $(\omega_1, \ldots, \omega_n)$ be a basis of the space of left invariant differential forms of degree 1 on G; then $\omega_1 \wedge \omega_2 \wedge \cdots \wedge \omega_n$ is a basis of S.

#### Proposition 54 {#lie-iii-s3-prop-54 .statement}

Let G be a Lie group of finite dimension n, ω a left invariant differential form of degree n on G and φ an endomorphism of G. Then

$$
\phi^*(\omega) = (\det L(\phi)) \omega.
$$

We write $L(\phi) = u$, $w_e = f$ and $\phi^*(\omega)_e = g$. For all $x_1, \ldots, x_n$ in $L(G)$,

$$
g(x_1, \ldots, x_n) = f(ux_1, \ldots, ux_n) = (\det u)f(x_1, \ldots, x_n)
$$

and hence $\phi^*(\omega)_e = \det L(\phi) \cdot w_e$. On the other hand, if $g \in G$,

$$
\phi \circ \gamma(g) = \gamma(\phi(g)) \circ \phi
$$

and hence $\gamma(g)^*\phi^*(\omega) = \phi^*(\omega)$. Thus $\phi^*(\omega)$ is left invariant, whence the proposition.

#### Corollary {#lie-iii-s3-n16-cor-1 .statement}

For all $g \in G$,

$$
\delta(g)^*\omega = (\det \mathrm{Ad}\, g) \omega.
$$

$$
\delta(g)^*\omega = \delta(g)^*\gamma(g)^*\omega = (\mathrm{Int}\, g)^*\omega \text{ and } L(\mathrm{Int}\, g) = \mathrm{Ad}\, g.
$$

Let G be a locally compact group and φ an endomorphism of G. Suppose that there exist open neighbourhoods V, $V'$ of e such that $\phi(V) = V'$ and $\phi|V$ is a local isomorphism of G into G. Let μ be a left Haar measure on G. By Integration, Chapter VII, § 1, Corollary to Proposition 9, there exists a unique number $a > 0$ such that $\phi(\mu|V) = a^{-1}\mu|V'$. Clearly a is independent of the choice of V, $V'$ and μ. It is called the modulus of φ and is denoted by $\mathrm{mod}_G \phi$ or simply $\mathrm{mod}\, \phi$. When φ is an automorphism of G, we recover Definition 4 of Integration, Chapter VII, § 1.

#### Proposition 55 {#lie-iii-s3-prop-55 .statement}

Suppose that K is locally compact. Let μ be a Haar measure on the additive group of K. Let G be a Lie group of finite dimension n.

(i) Let ω be a non-zero left invariant differential form of degree n on G. Then the measure $\mathrm{mod}(\omega)_\mu$ (Differentiable and Analytic Manifolds, R, 10.1.6) is a left Haar measure on G. If $K = \mathbf{R}$ and G has the orientation defined by ω, the measure defined by ω (Differentiable and Analytic Manifolds, R, 10.4.3) is a left Haar measure on G.

(ii) Let φ be an étale endomorphism of G. Then $\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$.

(i) is obvious. Let V, $V'$ be open neighbourhoods of e such that $\phi(V) = V'$ and $\phi|V$ is a local isomorphism of G into G. Then

$$
\phi^{-1}(\mathrm{mod}(\omega)_\mu|V') = \mathrm{mod}(\phi^*(\omega))_\mu|V) \quad \text{by transport of structure}
$$
$$
= \mathrm{mod}(\det L(\phi)\omega|V)_\mu \quad \text{(Proposition 54)}
$$
$$
= \mathrm{mod}\, \det L(\phi)(\mathrm{mod}(\omega)_\mu|V)
$$

whence $\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$ by definition of $\mathrm{mod}\, \phi$.

#### Corollary {#lie-iii-s3-n16-cor-2 .statement}

For all $g \in G$, $\Delta_G(g) = (\operatorname{mod} \det \operatorname{Ad} g)^{-1}$. In particular, for $G$ to be unimodular, it is necessary and sufficient that $\operatorname{mod} \det \operatorname{Ad} g = 1$ for all $g \in G$.

$$
\Delta_G(g) = (\operatorname{mod} \operatorname{Int} g)^{-1} \quad \text{(Integration, Chapter VII, § 1, formula (33))}
= (\operatorname{mod} \det L(\operatorname{Int} g))^{-1} \quad \text{(Proposition 55)}
= (\operatorname{mod} \det \operatorname{Ad} g)^{-1}.
$$

#### Remark {#lie-iii-s3-n16-rem-1 .statement}

Preserving the hypotheses and notation of Proposition 52, suppose that $K$ is locally compact. Let $\mu$ be the measure
$$
\operatorname{mod} \det(D_{n+i}m_k(x_1, \ldots, x_n, x_1, \ldots, x_n))_{1 \leq i, k \leq n} dx_1 \ldots dx_n
$$
on $\psi(U)$. Then $\psi^{-1}(\mu)$ is the restriction to $U$ of a Haar measure on $G$.

#### Proposition 56 {#lie-iii-s3-prop-56 .statement}

Let $G$ be a Lie group of finite dimension $n$, $H$ a $p$-dimensional Lie subgroup and $X$ the Lie homogeneous space $G/H$. Suppose that
$$
\det \operatorname{Ad}_{L(G)} h = \det \operatorname{Ad}_{L(H)} h
$$
for all $h \in H$. Then:
(i) The differential forms of degree $n - p$ on $X$ which are invariant under $G$ are analytic.
(ii) The vector space of these forms is of dimension 1.
(iii) If $\omega$ is such a non-zero form and $K$ is locally compact, $\operatorname{mod}(\omega)_\mu$ is a non-zero measure on $X$ which is invariant under $G$.

By § 1, no. 8, Examples, $\operatorname{Alt}^{n-p}(TX, K)$ is an analytic vector $G$-bundle. Let $x_0$ be the canonical image of $e$ in $X$; its stabilizer is $H$. The fibre of $\operatorname{Alt}^{n-p}(TX, K)$ at $x_0$ is $\bigwedge^{n-p} T_{x_0}(X)^*$ and $T_{x_0}(X)$ is canonically identified with $L(G)/L(H)$. If $h \in H$, the automorphism $\tau_h$ of $X$ defined by $h$ is derived when passing to the quotient from the automorphism $g \mapsto hgh^{-1}$ of $G$. Hence the automorphism $T_{x_0}(\tau_h)$ is derived when passing to the quotient from $\operatorname{Ad}_{L(G)}(h)$. As
$$
\det \operatorname{Ad}_{L(G)} h = (\det \operatorname{Ad}_{L(H)} h) \cdot (\det T_{x_0}(\tau_h)),
$$
the hypothesis implies that $\det T_{x_0}(h) = 1$. Thus, every element of $\bigwedge^{n-p} T_{x_0}(X)^*$ is invariant under $H$. Then (i) and (ii) follow from § 1, no. 8, Corollary 1 to Proposition 17 and (iii) is obvious.

The existence of a non-zero positive measure on $X$ invariant under $G$ follows from Integration, Chapter VII, § 2, Corollary 2 to Theorem 3, for the hypothesis of Proposition 56 implies $\Delta_G|H = \Delta_H$ (Corollary to Proposition 55).

#### Proposition 57 {#lie-iii-s3-prop-57 .statement}

Let $G$ be a Lie group of finite dimension $n$. Choose a basis for $\bigwedge^n T_e(G)^*$; by means of the right (resp. left) trivialization of $\bigwedge^n T(G)^*$, we can identify this vector bundle with the trivial vector bundle $G \times K$, so that the transpose of a scalar differential operator is identified with a scalar differential operator.

Then, if $u \in U(G)$, the transpose of $L_u$ (resp. $R_u$) is $L_u^\nu$ (resp. $R_u^\nu$).

We shall consider the case where $\Lambda^n T(G)^*$ has been trivialized using a right invariant form $\omega$.

Suppose that the proposition has been proved for elements $u_1, u_2$ of $U(G)$. Then,

$$
\begin{align*}
t(L_{u_1 * u_2}) &= t(L_{u_1} \circ L_{u_2}) & \text{(Proposition 23)} \\
&= t(L_{u_2}) \circ t(L_{u_1}) & \text{(\emph{Diff. \& Anal. Man.}, R, 14.3.3)} \\
&= L_{u_2}^\nu \circ L_{u_1}^\nu & \text{by hypothesis} \\
&= L_{u_2 * u_1}^{\nu \nu} & \text{(Proposition 23)} \\
&= L_{(u_1 * u_2)^\nu} & \text{(Proposition 7)}
\end{align*}
$$

and hence the proposition is true for $u_1 * u_2$. It therefore suffices to prove the proposition when $u \in T_e(G)$. Now $L_u$ is defined by $G$ operating on $G$ on the right (no. 6) and hence $\theta_{L_u} \omega = 0$ since $\omega$ is right invariant (\emph{Differentiable and Analytic Manifolds}, R, 8.4.5); therefore, if $f$ is an analytic function in an open neighbourhood of $e$ with values in $K$, then $\theta_{L_u}(f \omega) = (\theta_{L_u} f) \omega$ (\emph{Differentiable and Analytic Manifolds}, R, 8.4.8). Using the identifications made and \emph{Differentiable and Analytic Manifolds}, R, 14.4.1, the transpose of $L_u$ is $-L_u$, that is $L_u^\nu$.

#### Corollary {#lie-iii-s3-n16-cor-3 .statement}

Let $G$ be a finite-dimensional real Lie group, $\mu$ (resp. $\nu$) a left (resp. right) Haar measure on $G$, $k$ an integer $\geqslant 0$, $u \in U_k(G)$ and $f$ and $g$ real-valued functions of class $C^k$ on $G$ with compact support. Then

$$
\int_G (R_u f) g \, d\mu = \int_G f (R_u^\nu g) \, d\mu
$$
$$
\int_G (L_u f) g \, d\nu = \int_G f (L_u^\nu g) \, d\nu.
$$

This follows from Proposition 57 and \emph{Differentiable and Analytic Manifolds}, R, 14.3.8.

### 17. LEFT DIFFERENTIAL

#### Definition 9 {#lie-iii-s3-def-9 .statement}

Let $G$ be a Lie group, $M$ a manifold of class $C^r$ and $f$ a mapping of class $C^r$ of $M$ into $G$. The left (resp. right) differential of $f$ is the differential form of degree 1 on $M$ with values in $L(G)$ which associates with every vector $u \in T_m(M)$ the element $f(m)^{-1} \cdot (T_m f)(u)$ (resp. $(T_m f)(u) \cdot f(m)^{-1}$).

In this chapter we shall only consider the left differential, which we shall denote by $f^{-1}.df$, and leave to the reader the task of translating the results for the right differential.

If $f$ is the identity mapping of $G$, $f^{-1}.df$ is the canonical left differential form $\omega$ of $G$. Returning to the general case of Definition 8,

$$
(f^{-1}.df)_m = \omega_{f(m)} \circ T_m(f)
$$

and hence $f^{-1}.df = f^*(\omega)$. This implies that $f^{-1}.df$ is of class $C^{r-1}$.

#### Example {#lie-iii-s3-n17-exa-1 .statement}

(1) If $G$ is the additive group of a complete normable space and $T_0(E)$ is canonically identified with $E$, $f^{-1}.df$ is the differential $df$ defined in Differentiable and Analytic Manifolds, R, 8.2.2.

(2) Suppose that $G$ is the multiplicative group $A^*$ associated with a complete normable algebra $A$. Then $f$ can be considered as a mapping of $M$ into $A$ and hence the differential $df$ in the sense of Differentiable and Analytic Manifolds, R, 8.2.2 is defined and the product $f^{-1}df$ in the sense of Differentiable and Analytic Manifolds, R, 8.3.2 is defined. Clearly the latter form is identical with the left differential of $f$.

#### Proposition 58 {#lie-iii-s3-prop-58 .statement}

Let $G$ and $H$ be two Lie groups, $M$ a manifold of class $C^r$, $f$ a mapping of class $C^r$ of $M$ into $G$ and $h$ a morphism of $G$ into $H$. Then

$$
(h \circ f)^{-1}.d(h \circ f) = L(h) \circ (f^{-1}.df) = (h^{-1}.dh) \circ T(f).
$$

For all $x \in M$ and $u \in T_x(M)$,

$$
(h \circ f)^{-1}.d(h \circ f)(u) = ((h \circ f)(x))^{-1}.T(h \circ f)(u).
$$

The latter expression is equal, on the one hand, to

$$
T(h)(f(x)^{-1}.T(f)(u)) \quad (§ 2, \text{Proposition 5})
$$
$$
= T_e(h)((f^{-1}.df)(u))
$$

and, on the other hand, to

$$
h(f(x))^{-1}T(h)(T(f)u)
$$
$$
= (h^{-1}.dh)(T(f)u).
$$

#### Proposition 59 {#lie-iii-s3-prop-59 .statement}

Let $G$ be a Lie group, $M$ a manifold of class $C^r$, $f$ and $g$ mappings of class $C^r$ of $M$ into $G$ and $p$ the canonical surjection of $TM$ onto $M$.

(i) $(fg)^{-1}.d(fg) = (\mathrm{Ad} \circ g \circ p)^{-1} \circ (f^{-1}.df) + g^{-1}.dg.$

(ii) Writing $h(m) = f(m)^{-1}$ for all $m \in M$,

$$
h^{-1}.dh = -(\mathrm{Ad} \circ f \circ p) \circ (f^{-1}.df).
$$

Assertion (i) follows from § 2, no. 2, Proposition 7. Assertion (ii) follows from (i) by putting $g = h$.

#### Corollary 1 {#lie-iii-s3-prop-59-cor-1 .statement}

Let $s \in G$ and $sg$ be the mapping $x \mapsto sg(x)$ of $M$ into $G$. Then

$$
(sg)^{-1}.d(sg) = g^{-1}.dg.
$$

This follows from Proposition 59 (i) taking $f$ to be the constant mapping $x \mapsto s$ of $M$ into $G$.

#### Corollary 2 {#lie-iii-s3-prop-59-cor-2 .statement}

*If the mappings $f$ and $g$ of $M$ into $G$ have the same left differential, the tangent mapping to $fg^{-1}$ is everywhere zero. If further $K$ is of characteristic 0, then $fg^{-1}$ is locally constant.*

By Proposition 59,

$$
(fg^{-1})^{-1} \cdot d(fg^{-1}) = (\mathrm{Ad} \circ g \circ p) \circ (f^{-1}.df) - (\mathrm{Ad} \circ g \circ p) \circ (g^{-1}.dg).
$$

If $f^{-1}.df = g^{-1}.dg$, then $(fg^{-1})^{-1} \cdot d(fg^{-1}) = 0$, that is $T_x(fg^{-1}) = 0$ for all $x \in M$. This proves the first assertion. The second follows from it by *Differentiable and Analytic Manifolds*, R, 5.5.3.

#### Proposition 60 {#lie-iii-s3-prop-60 .statement}

*Let $G$ be a Lie group, of finite dimension if $K$ is of characteristic > 0, $M$ a manifold of class $C^r$, $f$ a mapping of class $C^r$ of $M$ into $G$ and $\alpha$ the left differential of $f$. Then $d\alpha + [\alpha]^2 = 0$.*

Let $\omega$ be the canonical left differential form of $G$. Using Corollary 1 to Proposition 51, no. 14, we have

$$
d\alpha = d(f^*(\omega)) = f^*(d\omega) = f^*(-[\omega]^2)
= -[f^*(\omega)]^2 = -[\alpha]^2.
$$

### 18. LIE ALGEBRA OF A LIE GROUP GERM

In this no. $(G, e, \theta, m)$ denotes a Lie group germ. A large part of the results of the § are still true with the same proof. We shall review those which we shall find useful.

18.1. Let $\Omega$ be the set of definition of $m$. Let $(g, g') \in \Omega,\ t \in T_e^{(\infty)}(G),\ t' \in T_{g'}^{(\infty)}(G)$. As in no. 1, the convolution product of $t$ and $t'$, denoted by $t * t'$, is the image of $t \otimes t'$ under $m$. We write $U(G) = T_e^{(\infty)}(G),\ U_s(G) = T_e^{(s)}(G),\ U^+(G) = T_e^{(\infty)+}(G),\ U_s^+(G) = T_e^{(s)+}(G)$. For $t, t'$ in $U(G)$, $t * t'$ is defined and belongs to $U(G)$. With the convolution product, $U(G)$ is an associative algebra with unit element $\varepsilon_e$, filtered by the $U_s(G)$. The canonical isomorphism $i_{G,e}$ of gr $U(G)$ onto $TS(T_e(G))$ is an algebra isomorphism.

18.2. Let $G, H$ be Lie group germs and $\phi : G \to H$ a morphism. If $t \in U(G)$, the image $U(\phi)(t)$ of $t$ under $\phi_*$ is an element of $U(H)$ and $U(\phi)$ is a morphism of the algebra $U(G)$ into the algebra $U(H)$. The mapping $\theta : x \mapsto x^{-1}$ of $G$ into $G$ defines a mapping $t \mapsto t^\vee$ of $U(G)$ into $U(G)$. For $t, t'$ in $U(G)$, the product $t * t'$ evaluated relative to $G^\vee$ is equal to the product $t' * t$ evaluated relative to $G$ and $(t * t')^\vee = {t'}^\vee * t^\vee$. Then $U(\phi)(t^\vee) = (U(\phi)t)^\vee$. If $G_1, \ldots, G_n$ are Lie group germs and $G = G_1 \times \cdots \times G_n$, the canonical isomorphism of $U(G_1) \otimes \cdots \otimes U(G_n)$ onto $U(G)$ is an algebra isomorphism;

for $t_1, \ldots, t_n$ in $U(G)$, $(t_1 \otimes \cdots \otimes t_n)^{\vee} = t_1^{\vee} \otimes \cdots \otimes t_n^{\vee}$. Let $H$ be a Lie subgroup germ of $G$ and $i : H \to G$ the canonical injection. Then $U(i)$ is an injective homomorphism of the algebra $U(H)$ into $U(G)$ and
$$
U(i)(t^{\vee}) = (U(i)(t))^{\vee}
$$
for all $t \in U(H)$. With the convolution product and the coproduct defined by the manifold structure on $G$, $U(G)$ is a bigebra and $U(\phi)$ is a bigebra morphism.

18.3. Let $G$ be a Lie group germ, $X$ a manifold of class $C^r$ and $\psi$ a law chunk of left operation of class $C^r$ of $G$ on $X$. Let $\Omega$ be the set of definition of $\psi$. If $t \in T^{(s)}_g(G)$, $u \in T^{(s')}_x(X)$, $(g, x) \in \Omega$ and $s + s' \leq r$, let $t * u$ denote the image of $t \otimes u$ under $\psi_*$. Let $t \in T^{(s)}_g(G)$, $t' \in T^{(s')}_x(G)$, $u \in T^{(s'')}_x(X)$; if $s + s' + s'' \leq r$ and $gg'$, $(gg')x$, $g'x$, $g(g'x)$ are defined, then
$$
(t * t') * u = t * (t' * u).
$$
Let $x_0 \in X$ and $\rho(x_0)$ be the mapping $g \mapsto gx_0$, which is defined in an open neighbourhood of $e$. If $t \in U_r(G)$, then $\rho(x_0)_*t = t * \varepsilon_{x_0}$. Here and in the rest of this no., we shall leave to the reader the task of translating the results for law chunks of right operation.

18.4. Preserving the notation of 18.3, let $t \in U_s(G)$ with $s \leq r$. Let $f$ be a function of class $C^r$ on $X$ with values in a Hausdorff polynormed space. Let $t * f$ denote the function on $X$ defined by
$$
\begin{align*}
(t * f)(x) &= \langle t, g \mapsto f(\psi(\theta(g), x)) \rangle \\
&= \langle t^{\vee}, f \circ \rho(x) \rangle = \langle \rho(x)_*(t^{\vee}), f \rangle = \langle t^{\vee} * \varepsilon_x, f \rangle.
\end{align*}
$$
If $t \in U_s(G)$, $t' \in U_{s'}(G)$ and $s + s' \leq r$, then $\langle t', t * f \rangle = \langle t^{\vee} * t', f \rangle$ and $(t * t') * f = t * (t' * f)$. Let $t \in U_s(G)$, $f$ and $f'$ be functions of class $C^r$ on $X$ with values in Hausdorff polynormed spaces $F, F'$ and $(u, u') \mapsto u.u'$ be a continuous bilinear mapping of $F \times F'$ into a Hausdorff polynormed space; let
$$
\sum_{i=1}^n t_i \otimes t'_i
$$
be the image of $t$ under the coproduct; if $s \leq r$, then
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

18.5. Preserving the notation of 18.3, let $t \in U_s(G)$ with $s \leq r$. The mapping $x \mapsto t * \varepsilon_x$ is called the field of point distributions defined by $t$ and the law chunk of operation and is sometimes denoted by $D_t^{\psi}$ or $D_t$. If $f : X \to F$ is a function of class $C^r$, the function $t^{\vee} * f$ on $X$ is also denoted by $D_t f$; it is of class $C^{r-s}$ if $s < \infty$. If $t \in U_s(G)$, $t' \in U_{s'}(G)$ and $s + s' \leq r$, then $D_{t*t'} f = D_{t'}(D_t f)$. If $G$ and $X$ are finite-dimensional, $D_t$ is a differential operator on $X$ of order $\leq s$ and of class $C^{r-s}$ (if $s < \infty$). The function $D_t f$ is then the transform of $f$ under this differential operator.

18.6. Let G be a Lie group germ and $t \in U(G)$. $L_t$ denotes the field of point distributions $g \mapsto \varepsilon_g * t$ on G and $R_t$ the field of point distributions $g \mapsto t * \varepsilon_g$ on G. If $f \in C^\omega(G, F)$, then $L_t f \in C^\omega(G, F)$ and $R_t f \in C^\omega(G, F)$. For $t, t'$ in $U(G)$, $L_{t \circ t'} = L_t \circ L_{t'}$, $R_{t \circ t'} = R_{t'} \circ R_t$, $L_t \circ R_{t'} = R_{t'} \circ L_t$, $\theta(L_t) = R_t^V$.

18.7. As $T_e(G)$ is the set of primitive elements of $U(G)$,

$$
[T_e(G), T_e(G)] \subset T_e(G).
$$

The normable space $T_e(G)$, together with the bracket, is a normable Lie algebra, called the normable Lie algebra of G (or Lie algebra of G) and denoted by $L(G)$. Let $E(G)$ be the enveloping algebra of $L(G)$. The canonical injection of $L(G)$ into $U(G)$ defines a homomorphism $\eta$ of the algebra $E(G)$ into the algebra $U(G)$; if K is of characteristic 0, $\eta$ is a bigebra isomorphism, by means of which $U(G)$ is identified with $E(G)$. Using the notation of 18.3, for all $a \in L(G)$, let $D_a$ be the field of point distributions defined by $a$ on X. The mapping $(a, x) \mapsto D_a(x)$ is a morphism of class $C^{r-1}$ of the trivial vector bundle $L(G) \times X$ into the vector bundle $T(X)$. Let I be an open subset of K containing 0 and $\gamma : I \to G$ a mapping of class $C^r$ such that $\gamma(0) = e$. Let $a = T_0(\gamma) l \in L(G)$. If $f : X \to F$ is a function of class $C^r$, then

$$
(D_a f)(x) = \lim_{k \in K^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)).
$$

If $r \geq 2$, the mapping $a \mapsto D_a$ is a law of left infinitesimal operation of class $C^{r-1}$ of $L(G)$ on X.

18.8. Let G and H be Lie group germs and $\phi$ a morphism of G into H. The restriction of $U(\phi)$ to $L(G)$, which is just $T_e(\phi)$, is a continuous morphism of $L(G)$ into $L(H)$, which we denote by $L(\phi)$. If $\psi$ is a morphism of H into a Lie group germ, then $L(\psi \circ \phi) = L(\psi) \circ L(\phi)$. For $\phi$ to be an immersion, it is necessary and sufficient that $L(\phi)$ be an isomorphism of $L(G)$ onto a Lie subalgebra of $L(H)$ which admits a topological supplement. In particular, if G is a Lie subgroup germ of H and $\phi$ is the canonical injection, $L(G)$ is identified with a Lie subalgebra of $L(H)$ by means of $L(\phi)$. If $(G_i)_{i \in I}$ is a finite family of Lie group germs and G is their product, $L(G)$ is canonically identified with $\prod_{i \in I} L(G_i)$.

18.9. Let G be a Lie group germ, of finite dimension if K is of characteristic > 0. Let F be a complete normable space. Let $\alpha$ be a differential form of degree k on G with values in F. $\alpha$ is called left invariant on G if $\alpha_g$ is derived from $\alpha_e$ by the mapping $h \mapsto gh$ of a neighbourhood of e onto a neighbourhood of g. If $\alpha$ is left invariant, $\alpha$ is analytic. The mapping $\alpha \mapsto \alpha_e$ is a bijection of the set of left invariant differential forms of degree k on G with values in F onto the set of continuous alternating k-linear mappings of $T_e(G)$ into F. If $\alpha_e = \mathrm{Id}_{T_e(G)}$, $\alpha$ is called the *left canonical differential form of G*. The definitions of right invariant differential forms and the right canonical differential form of G are analogous. If $\omega$ is the left canonical differential form of G, then $d\omega + [\omega]^2 = 0$. Let M be a manifold of class $C^r$ and $f$ a mapping of class $C^r$ of M into G. The left differential of $f$, denoted by $f^{-1}.df$, is the differential form of degree 1 on M with values in $L(G)$ which associates with each vector $u \in T_m(M)$ the element $f(m)^{-1}.(T_{m,f})(u)$. Then $f^{-1}.df = f^*(\omega)$ and $d\alpha + [\alpha]^2 = 0$. If two mappings $f$ and $g$ of M into G have the same left differential and K is of characteristic 0, then $fg^{-1}$ is locally constant.

### Exercises {#lie-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
