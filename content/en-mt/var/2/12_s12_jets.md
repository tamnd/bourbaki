---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 12
section_title: Jets
lang: en
source: var-fr
pdf_pages: 0143-0151
extraction: ocr
subsections:
    - "no": 1
      title: Jets d’applications
      page: 0
      pdf_page: 143
    - "no": 2
      title: Jets d’applications d’espaces de Banach
      page: 0
      pdf_page: 144
    - "no": 3
      title: Variétés de jets
      page: 0
      pdf_page: 144
    - "no": 4
      title: Repères et fibrations principales
      page: 0
      pdf_page: 146
    - "no": 5
      title: Jets de sections
      page: 0
      pdf_page: 147
    - "no": 6
      title: Jets de sections d’un fibré vectoriel
      page: 0
      pdf_page: 148
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 150
statements: 1
exercises: 0
content_sha256: 6a78df6ef6f5cba7d9349c6327ba42a6324ad921a394aeb47acd6d730a4fa2b8
translated_from: content/fr/var/2/12_s12_jets.md
source_lang: fr
translation_method: machine
source_content_sha256: 3cef1d15729f7411300863edad308e8143c54cc5db300a69be7628ab5c76eb0f
translation_model: gpt-5-6
translation_run: translate-en-mt-bb272c86
glossary_version: 34
glossary_terms_sha256: bf21981394d71b7e4d3682f12dd06d9dc2364427efdd16a8a4b52dcd2c7301d2
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 12. Jets

In this paragraph, we denote by $X$ and $Y$ two varieties of class $C^r$, where $r \in \mathbf{N}_k$, and $k$ an integer such that $0 \leq k \leq r$.

From No. 12.3 onwards, we assume:

— either that $K$ is of characteristic zero;

— or that the varieties, Banach spaces and vector bundles considered are locally of finite dimension.

### 12.1. Jets of mappings

### 12.1.1. Let $x \in X$ and let $f, g$ be two continuous mappings defined in a neighbourhood of $x$ and taking values in $Y$. We say that $f$ and $g$ have contact of order $\geq k$ at $x$ if $f(x)=g(x)$ and if there exist charts $(U,\varphi,E)$ of $X$ at $x$ and $(V,\psi,F)$ of $Y$ at $f(x)$ such that the mappings $\psi \circ f \circ \varphi^{-1}$ and $\psi \circ g \circ \varphi^{-1}$, defined in a neighbourhood of $\varphi(x)$ in $E$ and taking values in $F$, have contact of order $\geq k$ at $\varphi(x)$ (1.1.2). This property is then satisfied by all charts of $X$ at $x$ and of $Y$ at $f(x)$.

### 12.1.2. Let $x \in X$, $y \in Y$. In the set of mappings of class $C^r$ defined in a neighbourhood of $x$, taking values in $Y$, and mapping $x$ onto $y$, the relation « $f$ and $g$ have contact of order $\geq k$ » is an equivalence relation; the class of $f$ for this relation is denoted by $j^k_x(f)$ and is called the jet of order $k$ of $f$ with source $x$ and target $y$. The source of a jet is denoted by $s(j)$ and its target by $b(j)$.

The set of jets of order $k$ from $X$ into $Y$ (resp. with source $x$, resp. with target $y$) is denoted by $J^k(X,Y)$ (resp. $J^k_x(X,Y)$, resp. $J^k(X,Y)_y$) and we put

$$
J^k(X,Y)_y^x = J^k_x(X,Y) \cap J^k(X,Y)_y.
$$

### 12.1.3. If $U$ and $V$ are open subsets of $X$ and $Y$ respectively, one identifies in an obvious way $J^k(U,V)$ with the inverse image of $U \times V$ by the mapping

$$
(s,b): J^k(X,Y) \longrightarrow X \times Y.
$$

### 12.1.4. Let $Z$ be a variety of class $C^r$, and let $(x,y,z) \in X \times Y \times Z$. Let $j \in J^k(X,Y)_y$ and let $j' \in J^k(Y,Z)_z$. The mappings $f' \circ f$, with $f \in j$ and $f' \in j'$, have the same jet of order $k$ at $x$; this jet is called the composite of $j$ and $j'$ and is denoted by $j' \circ j$; one has $s(j' \circ j)=s(j)$ and $b(j' \circ j)=b(j')$. If $T$ is a variety of class $C^r$ and if $j'' \in J^k_z(Z,T)$, one has

$$
j'' \circ (j' \circ j)=(j'' \circ j')\circ j.
$$

12.1.5. Let $j \in J_x^k(X, Y)$, with $x \in X$, and let $k'$ be an integer such that $0 \leq k' \leq k$. The jets $j_x^{k'}(f)$, for $f \in j$, are equal; the jet thus defined is denoted by $r^{k', k}(j)$; the mapping $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ is surjective.

12.1.6. Suppose that $r$ is equal to $\infty$ or to $\omega$. Let $f$ and $g$ be two mappings of class $C^r$ defined in a neighbourhood of a point $x \in X$, and with values in $Y$. If $j_x^m(f) = j_x^m(g)$ for every integer $m \geq 0$, one says that $f$ and $g$ have contact of infinite order at $x$. One thus obtains an equivalence relation whose classes are called the jets of infinite order at $x$; the jet of infinite order of $f$ is denoted by $j_x^\infty(f)$ or $j_x^\omega(f)$. The definitions and results which precede extend without modification to jets of infinite order.

### 12.2. Jets of mappings of Banach spaces

In this No., E and F denote two Banach spaces. If $m$ is an integer $\geq 0$, we denote by $P_m(E; F)$ the Banach space of continuous homogeneous polynomials of degree $m$ on E with values in F (Part 1, Appendix, A.2).

12.2.1. Let U be an open subset of E, let $f : U \to F$ be a mapping of class $C^r$, and let $a \in U$. There exists one and only one continuous polynomial
$$
\tilde{f} = f_0 + \cdots + f_k \quad (\text{avec } f_m \in P_m(E; F))
$$
of degree $\leq k$, which has at the origin the same jet of order $k$ as $x \mapsto f(x - a)$. If $0 \leq m \leq k$, the $m$-th component $f_m$ of $\tilde{f}$ is denoted by $\Delta^m f(a)$ or $\Delta_a^m(f)$. When $r = \omega$, this notation coincides with that of 3.2.1 and 4.2.1; when $r \leq \infty$, we have
$$
m! \Delta^m f(a)(h) = D^m f(a)(h, \ldots, h) = D^m f(a) . h^m.
$$
The mapping $f \mapsto \tilde{f}$ defines by passing to the quotient a bijection of $J_a^k(E, F)$ onto $\prod_{0 \leq m \leq k} P_m(E; F)$ by means of which these two spaces are identified; in particular, $J_a^k(E, F)$ is endowed with a Banach space structure over K. If $j \in J_a^k(E, F)$, we denote by $\Delta_a^m(j)$ the $m$-th component of $j$; we have
$$
\Delta_a^m(j) \in P_m(E; F) \quad \text{pour} \quad 0 \leq m \leq k, \quad \text{et} \quad \Delta_a^0(j) = b(j) \in F.
$$

12.2.2. Let U (resp. V) be an open subset of E (resp. F). Let $Q^k(E, F)$ denote the product Banach space of the $P_m(E; F)$ for $1 \leq m \leq k$. The mapping
$$
j \mapsto (s(j), b(j), \Delta_{s(j)}^1(j), \ldots, \Delta_{s(j)}^k(j))
$$
is a bijection of $J^k(U, V)$ onto $U \times V \times Q^k(E, F)$, by means of which these two sets are identified. In particular, $J_0^k(E, F)_0$ is identified with $Q^k(E, F)$.

### 12.3. Jet manifolds

12.3.1. Let $c = (U, \varphi, E)$ and $c' = (V, \psi, F)$ be charts of X and Y respectively. The mappings $\varphi$ and $\psi$ define, by transport of structure, a bijection $\pi$ of $J^k(U, V)$ onto
$$
J^k(\varphi(U), \psi(V)) = \varphi(U) \times \psi(V) \times Q^k(E, F),
$$
cf. 12.2.2. If we put $W = J^k(U, V)$ and $G = E \times F \times Q^k(E, F)$, the triple $(W, \pi, G)$ is a chart of $J^k(X, Y)$. The charts so obtained form a $C^{r-k}$-atlas and this endows $J^k(X, Y)$ with a *structure of a K-manifold of class $C^{r-k}$*[^1]

If $(x, y) \in X \times Y$, the sets $J_x^k(X, Y), J^k(X, Y)_y$ and $J_x^k(X, Y)_y$ are closed submanifolds of $J^k(X, Y)$.

12.3.2. If $X$ and $Y$ are pure (resp. finite-dimensional, resp. separated, resp. connected), the same is true of $J^k(X, Y)$.

If $U$ (resp. $V$) is open in $X$ (resp. in $Y$), $J^k(U, V)$ is an open submanifold of $J^k(X, Y)$, cf. 12.1.3.

12.3.3. The mappings $s : J^k(X, Y) \to X, b : J^k(X, Y) \to Y$ and $(s, b) : J^k(X, Y) \to X \times Y$ are fibrations (6.1.1) of class $C^{r-k}$. When $k = 0$, $(s, b)$ is an isomorphism.

12.3.4. Let $T_X$ and $T_Y$ denote the vector bundles $pr_1^* T(X)$ and $pr_2^* T(Y)$ on $X \times Y$, and let $\mathscr{L}(T_X; T_Y)$ be the bundle of homomorphisms from $T_X$ into $T_Y$ (7.7.3); if $(x, y) \in X \times Y$, we have
$$
\mathscr{L}(T_X; T_Y)_{(x, y)} = \mathscr{L}(T_x(X); T_y(Y)).
$$
Let $j \in J^k(X, Y), k \geqslant 1$, and let $f \in j$. The tangent mapping to $f$ at $x = s(j)$ depends only on $j$; we denote it by $T(j)$; it is an element of $\mathscr{L}(T_x(X); T_y(Y))$, where $y = b(j)$. When $k = 1$ the mapping
$$
T : J^1(X, Y) \to \mathscr{L}(T_X; T_Y)
$$
resulting is an isomorphism of varieties of class $C^{r-1}$.

For $X = K$, this isomorphism identifies $J_0^1(K, Y)$ with $T(Y)$; for $Y = K$, it identifies $J^1(X, K)_0$ with the dual $T'(X)$ of $T(X)$.

12.3.5. Let $k'$ be an integer such that $0 \leqslant k' \leqslant k$. The mapping
$$
\rho^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)
$$
is a fibration of class $C^{r-k}$.

12.3.6. Let $Z$ be a variety of class $C^r$, and let $T$ be the set of pairs
$$
(j, j') \in J^k(X, Y) \times J^k(Y, Z)
$$
such that $b(j) = s(j')$. Then $T$ is a subvariety of $J^k(X, Y) \times J^k(Y, Z)$ and the mapping $(j, j') \mapsto j' \circ j$ is a morphism of class $C^{r-k}$ from $T$ into $J^k(X, Z)$.

12.3.7. If $f : X \to Y$ is a morphism of class $C^r$, the mapping $x \mapsto j_x^k(f)$ is a morphism $j^k(f)$ of class $C^{r-k}$ from $X$ into $J^k(X, Y)$.

12.3.8. Let $k'$ and $k''$ be positive integers whose sum is $k$. Let $x \in X$, let $U$ be an open neighbourhood of $x$, and let $f : U \to Y$ be a morphism of class $C^r$. The mapping
$$
x \mapsto j_x^{k'}(f) : U \to J^{k'}(X, Y)
$$
is of class $C^{r-k'}$ and its jet of order $k''$ at $x$ depends only on $j_x^k(f)$. We thus obtain a canonical mapping
$$
\alpha : J^k(X, Y) \to J^{k''}(X, J^{k'}(X, Y))
$$
which is of class $C^{r-k}$; if $K$ is of characteristic zero, it is an embedding.

12.3.9. Let $X', Y'$ be manifolds of class $C^r$, let $f : X \to X'$ and $g : Y' \to Y$ be morphisms, and let $(x, y') \in X \times Y'$, $x' = f(x)$, $y = g(y')$. If $u \in J_{x'}^k(X', Y')_{y'}$, put
$$
J_{x'}^k(f, g)_y(u) = j_y^k(g) \circ u \circ j_x^k(f).
$$
We thus obtain a mapping
$$
J^k(f, g) : J^k(X', Y') \times_{X'} X \to J^k(X, Y)
$$
which is of class $C^{r-k}$.

12.3.10. Let $A$ be a compact subset of $X$. Let $\mathscr{C}^k(X; Y)$ be the set of mappings of class $C^k$ from $X$ into $Y$. For every $f \in \mathscr{C}^k(X; Y)$, the mapping $j^k(f)|A$ belongs to the set $\mathscr{C}(A; J^k(X, Y))$ of continuous mappings from $A$ into $J^k(X, Y)$. We have thus defined a mapping $\lambda$ from $\mathscr{C}^k(X; Y)$ into $\mathscr{C}(A; J^k(X, Y))$. The inverse image by $\lambda$ of the topology of compact convergence on $\mathscr{C}(A; J^k(X, Y))$ (TG, X, § 3, Def. 1) is a topology on $\mathscr{C}^k(X; Y)$; it is called the *topology of uniform $C^k$-convergence on $A$*.

### 12.4. Frames and principal fibrations

12.4.1. Let $j \in J^k(X, Y)$ and let $x = s(j)$, $y = b(j)$. We say that $j$ is *invertible* if there exists $j' \in J_y^k(Y, X)_x$ such that $j' \circ j = j_x^k(\mathrm{Id}_X)$ and $j \circ j' = j_y^k(\mathrm{Id}_Y)$; the jet $j'$ is then determined uniquely; we denote it by $j^{-1}$. If $k = 0$, every jet is invertible. If $k \geqslant 1$, the following conditions are equivalent:
a) $j$ is invertible;
b) the mapping $T(j) : T_x(X) \to T_y(Y)$ (cf. 12.3.4) is an isomorphism;
c) there exists an isomorphism $g$ of class $C^r$ of an open neighbourhood of $x$ onto an open neighbourhood of $y$, such that $j_x^k(g) = j$.

12.4.2. Let $E$ be a Banach space. We denote by $\mathbf{GL}^k(E)$ the set of jets of order $k$ from $E$ into $E$ which are invertible and have $0$ as source and target; it is an open set of $J_0^k(E, E)_0$. Endowed with the law of composition of jets, and with the structure of variety induced by that of the Banach space $J_0^k(E, E)_0 = Q^k(E, E)$, it is a group variety of class $C^\omega$.

We have $\mathbf{GL}^0(E) = \{ e \}$. The group $\mathbf{GL}^1(E)$ is identified, by means of $T$, with the group $\mathbf{GL}(E)$ of automorphisms of $E$.

If $k' \leqslant k$, the mapping $r^{k, k'} : \mathbf{GL}^k(E) \to \mathbf{GL}^{k'}(E)$ is a homomorphism of class $C^\omega$ and is a surjective submersion. The mapping $f \mapsto \mathrm{Id}_E + f$ is an isomorphism of group varieties from $P_k(E, E)$ onto the kernel of $r^{k, k-1}$.

12.4.3. Let E be a Banach space. For every $x \in X$, an E-frame of order k of X at x is called any invertible element of $J_0^k(E, X)_x$. The set of E-frames of order k of X is an open subvariety $R^k(E, X)$ of $J_0^k(E, X)$; the mapping b has as its restriction a morphism, still denoted by b, from $R^k(E, X)$ into X; analogously, if $k' \leq k$, we still denote by $r^{k, k'}$ the morphism from $R^k(E, X)$ into $R^{k'}(E, X)$, restriction of the mapping $r^{k, k'}$ of 12.1.5.

12.4.4. We suppose that X is purely of type E (5.1.7). The group $GL^k(E)$ operates on the right on $R^k(E, X)$ by the law $(\rho, u) \mapsto \rho \circ u$ and the quadruplet $\lambda_X = (R^k(E, X), GL^k(E), X, b)$ is a principal fibration (6.2.1) with structural group $GL^k(E)$, basis X and of class $C^{r-k}$.

If $k' \leq k$, let H be the kernel of $r^{k, k'} : GL^k(E) \to GL^{k'}(E)$; the quadruplet $(R^k(E, X), H, R^{k'}(E, X), r^{k, k'})$ is a principal fibration of class $C^{r-k}$.

The manifold $J^k(X, Y)$ is provided with a structure of associated fibre space to $\lambda_X$ (6.5.1): the type fibre is $J_0^k(E, Y)$ on which $GL^k(E)$ operates on the left by the law $(u, j) \mapsto j \circ u^{-1}$; the frame mapping $R^k(E, X) \times J_0^k(E, Y) \to J^k(X, Y)$ transforms $(\rho, j)$ into $j \circ \rho^{-1}$. The projection $J^k(X, Y) \to X$ corresponding to this structure of associated fibre space is s.

12.4.5. Let F be a Banach space, and suppose that Y is purely of type F. Then $J^k(X, Y)$ is provided with a structure of associated fibre space to $\lambda_Y$: the type fibre is $J^k(X, F)_0$ on which $GL^k(F)$ operates on the left by the law $(v, j) \mapsto v \circ j$; the frame mapping is $(\sigma, j) \mapsto \sigma \circ j$; the projection $J^k(X, Y) \to Y$ is b.

12.4.6. The hypotheses being those of 12.4.4 and 12.4.5, let $\mu$ be the principal fibration
$$
(R^k(E, X) \times R^k(F, Y), GL^k(E) \times GL^k(F), X \times Y, b \times b),
$$
product of $\lambda_X$ and $\lambda_Y$. Then $J^k(X, Y)$ is provided with a structure of associated fibre space to $\mu$: the type fibre is $J_0^k(E, F)_0$ on which $GL^k(E) \times GL^k(F)$ operates on the left by the law $((u, v), j) \mapsto v \circ j \circ u^{-1}$; the frame mapping is $((\rho, \sigma), j) \mapsto \sigma \circ j \circ \rho^{-1}$; the projection $J^k(X, Y) \to X \times Y$ is $(s, b)$.

### 12.5. Jets of sections

12.5.1. Let $\pi : Y \to X$ be a submersion, let $x \in X$, and let $s \in J_x^k(X, Y)$. We say that s is a jet of section (of order k) of $\pi$ if s is of the form $j_x^k(f)$, where f is a section of class $C^r$ of $\pi$ above an open neighbourhood of x; this condition is equivalent to
$$
j_{b(s)}^k(\pi) \circ s = j_x^k(\mathrm{Id}_X).
$$
We denote by $P_x^k(\pi)$ (resp. $P^k(\pi)$) the set of jets $s \in J_x^k(X, Y)$ (resp. $J^k(X, Y)$) which are jets of section of $\pi$; it is a submanifold of class $C^{r-k}$ of $J^k(X, Y)$. The mappings
$$
s : P^k(\pi) \to X \quad \text{and} \quad b : P^k(\pi) \to Y
$$
are submersions; if $\pi$ is a fibration, they are fibrations. For $k = 0$, b is an isomorphism, by which we identify $P^0(\pi)$ with Y.

If $k' \leq k$, the mapping $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ applies $P^k(\pi)$ into $P^{k'}(\pi)$; the mapping from $P^k(\pi)$ into $P^{k'}(\pi)$ deduced from $r^{k, k'}$ is a fibration of class $C^{r-k}$.

12.5.2. Let $Z$ be a variety of class $C^r$; suppose that $Y = X \times Z$ and let $\pi = \mathrm{pr}_1 : Y \to X$. The restriction of $J^k(\mathrm{Id}_X, \mathrm{pr}_2)$ (cf. 12.3.9) to $P^k(\pi)$ is an isomorphism of $P^k(\pi)$ onto $J^k(X, Z)$, by which we identify these two varieties.

12.5.3. Let $Y'$ be a variety of class $C^r$, let $\pi : Y \to X$ and $\pi' : Y' \to X$ be submersions and let $g : Y \to Y'$ be a morphism such that $\pi' \circ g = \pi$. The mapping $J^k(\mathrm{Id}_X, g)$ has as its restriction a mapping

$$
P^k(g) : P^k(\pi) \to P^k(\pi')
$$

which is of class $C^{r-k}$.

Let $X'$ be a variety of class $C^r$, and let $f : X' \to X$ be a morphism; put $(Y', \pi') = f^*(Y, \pi)$, cf. 5.11.5. The mapping $J^k(f, \mathrm{Id}_Y)$ (cf. 12.3.9) defines a mapping of class $C^{r-k}$ from $f^*P^k(\pi)$ into $P^k(\pi')$.

### 12.6. Jets of sections of a vector bundle

12.6.1. Let $E$ be a vector bundle of class $C^r$ with base $X$, and let $\pi$ be its projection. Let $c_0 = (U, \varphi, F_0)$ be a vector bundle chart of $E$ and $c_1 = (U, \psi, F_1)$ be a chart of the variety $X$, with the same domain $U$. These charts define a bijection $\theta$ of $P^k(\pi)|U$ onto $J^k(\psi(U), F_0) = \psi(U) \times F_0 \times Q^k(F_1, F_0)$, cf. 12.2.2 and 12.3.1, whence a vector bundle chart

$$
d = (U, \theta, G), \quad \text{with} \quad G = F_0 \times Q^k(F_1, F_0) = \prod_{m=0}^k P_m(F_1; F_0)
$$

of $P^k(\pi)$. The charts so obtained form a vector bundle $C^{r-k}$-atlas, which equips $P^k(\pi)$ with the structure of a vector bundle of class $C^{r-k}$, with base $X$. This vector bundle is denoted by $P^k(E)$; the underlying variety structure is the one defined in 12.5.1.

Let $U$ be an open subset of $X$, and let $f \in \mathscr{S}_E^r(U)$ be a section of class $C^r$ of $E$ over $U$. The mapping $j^k(f) : x \mapsto j_x^k(f)$ is a section of class $C^{r-k}$ of $P^k(E)$ over $U$. The mapping $j^k : \mathscr{S}_E^r(U) \to \mathscr{S}_{P^k(E)}^{r-k}(U)$ is $K$-linear.

12.6.2. If $F$ is a Banach space, the identification (12.5.2) of $P^k(F_X)$ with $J^k(X, F)$ equips the latter variety with a structure of vector bundle of class $C^{r-k}$, with base $X$. When $F = K$, we write $P^k(X)$ instead of $P^k(K_X)$.

#### Example {#var-2-s12-n6-exa-1 .statement}

Take $X = K^n$, and denote by $u_1, \ldots, u_n$ the coordinate functions on $K^n$; then the fibre $P^k_0(X)$ of $P^k(X)$ at 0 has as basis the family of jets of order $k$ of the monomials $u_1^{m_1} \ldots u_n^{m_n}$, with $m_i \geqslant 0, \sum_{i=0}^n m_i \leqslant k$.

12.6.3. Let $d$ be an integer $\geqslant 0$, let $E_1, \ldots, E_d, F$ be vector bundles of class $C^r$ with base $X$, and let $u : E_1 \times_X \cdots \times_X E_d \to F$ be a multilinear morphism (7.3.1) of class $C^r$. There then exists one and only one multilinear morphism

$$
P^k(u) : P^k(E_1) \times_X \cdots \times_X P^k(E_d) \to P^k(F)
$$

such that

$$
P^k(u)(j^k(s_1), \ldots, j^k(s_d)) = j^k(u(s_1, \ldots, s_d))
$$

for every open set U of X and every sequence of sections $s_i \in \mathscr{S}_{E_i}'(U)$ for $1 \leq i \leq d$.

If A is a bundle of algebras (7.3.2) with base X, the morphism from $P^k(A) \times_X P^k(A)$ into $P^k(A)$ induced by the multiplication $A \times_X A \to A$ makes $P^k(A)$ a bundle of algebras; if A is a bundle of associative algebras, $P^k(A)$ is a bundle of associative algebras; if, in addition, M is a bundle of A-modules (7.3.3), $P^k(M)$ is a bundle of $P^k(A)$-modules. In particular, $P^k(X)$ is an *associative, commutative and unital bundle of algebras*; if E is a vector bundle, $P^k(E)$ is a *bundle of $P^k(X)$-modules*. If $u : E \to F$ is a morphism of vector bundles, then $P^k(u) : P^k(E) \to P^k(F)$ is a $P^k(X)$-homomorphism.

12.6.4. If $E \xrightarrow{u} F \xrightarrow{v} G$ is a locally split exact sequence of vector bundles with base X, then the same is true of the sequence

$$
P^k(E) \to P^k(F) \to P^k(G)
$$

where the homomorphisms in question are $P^k(u)$ and $P^k(v)$.

12.6.5. Let $k'$ and $k''$ be two positive integers whose sum is $k$, and let E be a vector bundle of class $C^r$ with base X. The morphism

$$
\alpha : J^k(X, E) \to J^{k''}(X, J^{k'}(X, E)) \quad (\text{cf. } 12.3.8)
$$

induces a morphism of vector bundles

$$
\beta : P^k(E) \to P^{k''}(P^{k'}(E))
$$

which is of class $C^{r-k}$. If U is an open set of X and $f \in \mathscr{S}_E'(U)$, we have

$$
\beta(j^{k}(f)) = j^{k''}(j^{k'}(f)).
$$

When K is of characteristic zero, $\beta$ is an isomorphism of $P^k(E)$ onto a vector subbundle of $P^{k''}(P^{k'}(E))$.

12.6.6. Let $k'$ be an integer such that $0 \leq k' \leq k$, and let E be a vector bundle of class $C^r$ with base X. The mapping

$$
r^{k, k'} : P^k(E) \to P^{k'}(E)
$$

is a locally direct surjective morphism of class $C^{r-k}$. Its kernel $N^{k, k'}(E)$ consists of section jets of E having contact of order $\geq k'$ with the zero section.

12.6.7 (*The vectorial functor $P_m$*). With the notation of 7.6, 7.7, 7.8, put $I_+ = \{0\}, I_- = \{1\}$ and let m be an integer $\geq 0$. If $\mathscr{V} = (V_0, V_1)$ is a pair of Banach spaces, denote by $\tau_m(\mathscr{V})$ the Banach space $P_m(V_1; V_0)$ of *homogeneous continuous polynomials* of degree m on $V_1$ with values in $V_0$ (A.2). Similarly, if $f = (f_0, f_1)$. where $f_0 : V_0 \to V'_0$ and $f_1 : V'_1 \to V_1$ are morphisms of Banach spaces, denote by $\tau_m(f)$ the morphism $p \mapsto f_0 \circ p \circ f_1$ from $P_m(V_1; V_0)$ into $P_m(V'_1; V'_0)$. We thus obtain a vectorial *functor* $\tau_m$ of class $C^\omega$. If $E_0$ and $E_1$ are two vector bundles with base $X$, denote by $P_m(E_1; E_0)$ the vector bundle deduced from $(E_0, E_1)$ by means of $\tau_m$ (7.6.2).

12.6.8. Let us resume the notation and hypotheses of 12.6.1. There exists one and only one morphism of vector bundles

$$
\iota : P_k(T(X); E) \to P^k(E) \quad (\text{cf. } 12.6.6),
$$

such that, whatever the vectorial chart $c_0 = (U, \varphi, F_0)$ of $E$ and the chart $c_1 = (U, \psi, F_1)$ of $X$, the following diagram is commutative:

$$
\begin{array}{ccc}
P_k(T(X), E)|U & \xrightarrow{\iota|U} & P^k(E)|U \\
\downarrow \eta & & \downarrow \theta \\
U \times P_k(F_1; F_0) & \xrightarrow{i} & U \times \prod_{m=0}^k P_m(F_1; F_0)
\end{array}
$$

where: 1) $\iota|U$ is the restriction of $\iota$ to $P_k(T(X), E)|U$;
   2) $\theta$ is the bijection defined in 12.6.1;
   3) $i$ is the mapping $(u, p) \mapsto (u, 0, \ldots, 0, p)$;
   4) $\eta$ is deduced, by means of the vectorial functor $\tau_k$, from the vectorial chart $c'_1$ of $T(X)$ (cf. 8.1.1) and the vectorial chart $c_0$ of $E$.

The morphism $\iota$ is an isomorphism of $P_k(T(X); E)$ onto the vector subbundle $N^{k, k-1}(E)$ of $P^k(E)$ (cf. 12.6.6); the sequence

$$
0 \to P_k(T(X); E) \xrightarrow{\iota} P^k(E) \xrightarrow{\tau^{k, k-1}} P^{k-1}(E) \to 0
$$

is a locally direct exact sequence of vector bundles.

More generally, put $N_0 = P^k(E)$, $N_m = N^{k, m-1}(E)$ for $m \geq 1$, so that the $N_m$ form a decreasing sequence of vector subbundles of $P^k(E)$:

$$
P^k(E) = N_0 \supset N_1 \supset \cdots \supset N_k \supset N_{k+1} = 0.
$$

For $0 \leq m \leq k$, the projection $r^{k, m} : P^k(E) \to P^m(E)$ defines an isomorphism of $N_m/N_{m+1}$ onto $N^{m, m-1}(E)$; viewed in the light of the foregoing, we thus obtain isomorphisms

$$
\iota_m : N_m/N_{m+1} \to P_m(T(X); E) \quad (0 \leq m \leq k).
$$

In particular, $N_0/N_1 \simeq E$ and $N_1/N_2 \simeq \mathscr{L}(T(X); E)$. For $k = 1$, this gives an exact sequence:

$$
0 \to \mathscr{L}(T(X); E) \to P^1(E) \to E \to 0.
$$

### 12.7. Weakening of structure

Suppose $K = \mathbf{R}$. Let $r' \in N_k$ with $k \leq r' \leq r$ and let $X'$ and $Y'$ be the manifolds of class $C^{r'}$ obtained from $X$ and $Y$ by weakening of structure (5.13.1). Let $x \in X$ and $j \in J_x^k(X, Y)$; let $U$ be an open subset of $X$ containing $x$ and $f$ a mapping of class $C^k$ from $U$ into $Y$, such that $j_x^k(f) = j$. Consider $f$ as a germ of morphism from X' into Y'; its jet $j' \in J_x^k(X', Y')$ depends only on $j$. The mapping $j \mapsto j'$ is an isomorphism of class $C^{r'-k}$ from $J^k(X, Y)$ onto $J^k(X', Y')$; it allows us to identify $J^k(X', Y')$ with the manifold of class $C^{r'-k}$ deduced from the manifold $J^k(X, Y)$ of class $C^{r-k}$ by weakening of structure. An analogous result applies to the manifolds $P^k(\pi)$ and $P^k(E)$ of Nos. 12.5 and 12.6.

[^1]: When $k = r$ (which is possible only if $K = \mathbf{R}$), $J^k(X, Y)$ is provided with a structure of *topological manifold* (cf. *Conventions and Notations*) and the morphisms and fibrations considered below are to be understood in a purely topological sense (cf. footnote to §6).
