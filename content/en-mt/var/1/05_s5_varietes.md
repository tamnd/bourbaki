---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 5
section_title: Variétés
lang: en
source: var-fr
pdf_pages: 0033-0058
extraction: ocr
subsections:
    - "no": 1
      title: Cartes et atlas. Variétés
      page: 0
      pdf_page: 33
    - "no": 2
      title: Exemples de variétés
      page: 0
      pdf_page: 35
    - "no": 3
      title: Fonctions de classe $C^r$ et morphismes de variétés
      page: 0
      pdf_page: 36
    - "no": 4
      title: Caractérisation des variétés par leurs faisceaux de fonctions
      page: 0
      pdf_page: 38
    - "no": 5
      title: Espaces tangents, applications linéaires tangentes
      page: 0
      pdf_page: 39
    - "no": 6
      title: Produits de variétés
      page: 0
      pdf_page: 42
    - "no": 7
      title: Immersions, morphismes étales
      page: 0
      pdf_page: 43
    - "no": 8
      title: Images inverses de structures de variété, sous-variétés
      page: 0
      pdf_page: 45
    - "no": 9
      title: Submersions et variétés quotients
      page: 0
      pdf_page: 48
    - "no": 10
      title: Subimmersions
      page: 0
      pdf_page: 50
    - "no": 11
      title: Produits fibrés et images réciproques
      page: 0
      pdf_page: 51
    - "no": 12
      title: Variétés de groupes
      page: 0
      pdf_page: 54
    - "no": 13
      title: Affaiblissement de structure
      page: 0
      pdf_page: 56
    - "no": 14
      title: Restriction du corps de base
      page: 0
      pdf_page: 56
statements: 0
exercises: 0
content_sha256: de22b9b5756c12da2b4ad3436a436907dc19032fe6854a0c443ce26f695214a5
translated_from: content/fr/var/1/05_s5_varietes.md
source_lang: fr
translation_method: machine
source_content_sha256: dd71956a97de3213da051d44a027f3c8f14a9f8fda6946fb9eaa04f9cbbd04ed
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5-6
translation_run: translate-en-mt-a3ab744f
glossary_version: 34
glossary_terms_sha256: ca8871fbd0c5712f16ffb5131388cf6a3690954e6ee1ba6091a8564a157259db
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. Manifolds

### 5.1. Charts and atlases. Manifolds

5.1.1. Let X be a set. A chart of X is a triple c = (U, φ, E), where U is a subset of X, E a Banach space and φ a bijection of U onto an open subset of E. We say that U is the domain of the chart c. If E is of finite dimension n, we say that c is of dimension n. Otherwise, we set dim c = +∞.

5.1.2. We say that two charts c = (U, φ, E) and c' = (U', φ', E') of X are C^r-compatible (or simply compatible when there can be no ambiguity about r) when the following conditions are satisfied:
(a) φ(U ∩ U') (resp. φ'(U ∩ U')) is open in E (resp. E');
(b) the mapping φ ∘ φ'^{-1} (resp. φ' ∘ φ^{-1}) of φ'(U ∩ U') onto φ(U ∩ U') (resp. of φ(U ∩ U') onto φ'(U ∩ U')) is of class C^r (cf. 2.3.1, 3.2.1 and 4.2.1).

5.1.3. A C^r-atlas (or simply atlas) of a set X is a set of pairwise C^r-compatible charts of X whose domains have X itself as their union. Two atlases A and B of X are said to be C^r-equivalent if A ∪ B is an atlas. The relation of C^r-equivalence between atlases is an equivalence relation.

5.1.4. Let S be a set of Banach spaces. We say that an atlas A is of type S if E ∈ S for every chart c = (U, φ, E) of A. In an analogous manner, we say that an atlas A is of Hilbert type (resp. of countable-dimensional Hilbert type) if E is a Hilbert space (resp. a Hilbert space of countable type) for every chart (U, φ, E) of A.

5.1.5. A K-manifold of class C^r (or a manifold of class C^r over K, or simply a manifold when there can be no ambiguity about K and r) is a set X endowed with a class of equivalent atlases (Ens., chap. II, § 6, No. 9) for the relation of C^r-equivalence. An atlas of this class is called an atlas of the manifold X. A chart belonging to an atlas of X is called a chart of the manifold X. A chart of X whose domain contains a point a ∈ X is called a chart of X at a. A chart centred at a is a chart (U, φ, E) of X at a such that φ(a) = 0.

If X is a set and A an atlas of X, the set X endowed with the equivalence class of A is called the manifold defined by A.

When r ≠ ω (hence K = R), a manifold of class C^r is sometimes called a differential manifold. A manifold of class C^ω is also called an analytic manifold over K (or K-analytic manifold).

When in addition $K = \mathbf{R}$ (resp. $\mathbf{C}$, $\mathbf{Q}_p$), we also say real analytic manifold (resp. complex analytic manifold, $p$-adic analytic manifold).

5.1.6. Let $X$ be a manifold. The subsets of $X$ which are unions of domains of charts of $X$ form the set of open subsets for a topology on $X$, called the topology underlying the manifold structure of $X$. For every chart $c = (U, \varphi, E)$ of $X$, the mapping $\varphi$ is a homeomorphism of the open subset $U$ endowed with the topology induced by that of $X$ onto the open subset $\varphi(U)$ of $E$.

The topological space underlying $X$ is a Baire space. When $K$ is equal to $\mathbf{R}$ or $\mathbf{C}$, it is locally connected.

Let $X$ be a manifold and let $\mathcal{A}$ be an atlas of $X$. For the topological space $X$ to be separated, it is necessary and sufficient that the following condition be satisfied: whatever the charts $(U, \varphi, E)$ and $(V, \psi, F)$ belonging to the atlas $\mathcal{A}$, the graph of the mapping $\psi \circ \varphi^{-1}$ of $\varphi(U \cap V)$ into $\psi(U \cap V)$ is closed in $\varphi(U) \times \psi(V)$.

Let $X$ be a manifold; suppose that the topological space $X$ is regular. Then for every point $a \in X$, there exists a chart $(U, \varphi, E)$ of $X$ at $a$ having the following property: for a subset $Y$ of $U$ to be closed in $X$, it is necessary and sufficient that its image $\varphi(Y)$ be closed in $E$. If the space $X$ is paracompact, there exists on $X$ a distance compatible with the topology of $X$ and making $X$ a complete metric space.

5.1.7. Let $\mathfrak{S}$ be a set of Banach spaces. We say that a manifold is of type $\mathfrak{S}$ (resp. of Hilbert type, resp. of countable-dimensional Hilbert type) if it possesses an atlas of type $\mathfrak{S}$ (resp. of Hilbert type, resp. of countable-dimensional Hilbert type). If $\mathfrak{S}$ is reduced to a single element $E$, a manifold of type $\mathfrak{S}$ is also called a purely manifold of type $E$.

A pure manifold of dimension $n$ is a pure manifold of type $K^n$. We say that a manifold is locally of finite dimension if it is of type $\mathfrak{S}$ with $\mathfrak{S} = \{ K^n ; n \in \mathbf{N} \}$.

5.1.8. Let $X$ be a manifold and let $x \in X$. The dimension (finite or $+\infty$) of a chart of $X$ at $x$ depends only on $x$. It is called the dimension of $X$ at $x$ and is denoted by $\dim_x X$. The dimension of $X$, denoted by $\dim X$, is the supremum of the $\dim_x X$ for $x \in X$.

The mapping $x \mapsto \dim_x X$ is locally constant. The manifold $X$ is locally of finite dimension (resp. purely of dimension $n$) if and only if $\dim_x X < +\infty$ (resp. $\dim_x X = n$) for every $x \in X$.

5.1.9. Suppose $K$ is locally compact. Let $X$ be a separated manifold. Then, for $X$ to be locally of finite dimension, it is necessary and sufficient that $X$ be locally compact.

No. 5.2

5.1.10. Let X be a manifold and let $\xi^1, \ldots, \xi^n$ be mappings of a subset U of X into K. We say that $\xi = (\xi^1, \ldots, \xi^n)$ is a system of coordinates of X in U if the triplet $(U, \xi, K^n)$ is a chart of X; this chart is also denoted by $(U; \xi)$ or $(U; \xi^1, \ldots, \xi^n)$. If $a \in U$, we also say that $\xi$ is a system of coordinates of X at $a$; if in addition $\xi^i(a) = 0$ for $i = 1, 2, \ldots, n$, we say that the system of coordinates $\xi$ is centred at $a$.

### 5.2. Examples of manifolds

5.2.1. Let X be a set; there exists on X one and only one manifold structure for which the underlying topological space is discrete; this structure is a purely 0-dimensional manifold structure.

5.2.2. Let E be a Banach space. The triplet $c = (E, \mathrm{Id}_E, E)$ is a chart of E and $\mathcal{A} = \{c\}$ is an atlas of E, and hence defines a purely manifold structure of type E on E; the underlying topology is the topology given on E. Whenever in what follows we speak of the manifold structure on E, it will always be the preceding structure to which we refer.

In particular, this applies to every finite-dimensional vector space over K, endowed with the unique separated topology compatible with its vector structure (Esp. Vect. Top., chap. I, § 2, No. 3).

5.2.3. Let X be a manifold and U an open subset of X. There exists on U a manifold structure whose charts are the charts of the manifold X with domain contained in U. This structure is said to be induced by that of X (cf. No. 5.3.4); endowed with this structure, U is called an open submanifold of X.

In particular, every open subset of a Banach space E is endowed with a canonical purely manifold structure of type E. Let X be a manifold; for a triplet $(U, \varphi, E)$ to be a chart of X, it is necessary and sufficient that U be open in X and that $\varphi$ be an isomorphism of the open submanifold U of X onto an open submanifold of E.

5.2.4. Let X be a set, and $(X_i)_{i \in I}$ a covering of X. Suppose that each $X_i$ is endowed with a manifold structure such that the following condition is fulfilled:

For any $i$ and $j$ in I, the set $X_i \cap X_j$ is open in $X_i$ and $X_j$ and the manifold structures induced on $X_i \cap X_j$ by those of $X_i$ and $X_j$ coincide.

There then exists on X one and only one manifold structure such that $X_i$ is an open submanifold of X for every $i$ in I. We say that the manifold X is obtained by gluing the manifolds $X_i$.

5.2.5. Let X be a manifold. The set $X_n$ of points $x$ of X such that dim_x X = n (n integer $\geq 0$) is an open submanifold of X, which is purely of dimension n.

5.2.6. Let E be a Banach space. The set G(E) of vector subspaces of E admitting a topological supplement can be endowed with an analytic manifold structure in the following way: for every pair (F_0, G_0) $\in G(E) \times G(E)$ such that E = F_0 $\oplus$ G_0, let U_{G_0} denote the set of F $\in G(E)$ admitting G_0 as a supplement, and define a bijection $\varphi_{F_0, G_0}$ of U_{G_0} onto the Banach space $\mathcal{L}(F_0; G_0)$ by associating to each F $\in U_{G_0}$ the mapping from F_0 into G_0 having as graph the subspace F of E = F_0 $\times$ G_0. The charts (U_{G_0}, $\varphi_{F_0, G_0}$, $\mathcal{L}(F_0; G_0)$) form an atlas of G(E). Endowed with the manifold structure defined by this atlas, G(E) is called the Grassmann manifold of E.

The topological space G(E) is metrisable. If K is locally compact and E finite-dimensional, G(E) is compact.

For every integer $n \geq 0$, the set G_n(E) (resp. G^n(E)) of F $\in G(E)$ of dimension (resp. codimension) n is open and closed in G(E) and is a purely open submanifold of G(E). If K = R or C, G_n(E) is connected for every n.

The mapping which to F $\in G(E)$ associates its orthogonal in the dual E’ of E is a morphism of G(E) into G(E’) which induces an isomorphism of G^n(E) onto G_n(E’) for every integer n.

If K = R or C, or if E is finite-dimensional, G_1(E) is nothing other than the projective space deduced from E, which is thus endowed with an analytic manifold structure.

### 5.3. Functions of class $C^r$ and morphisms of manifolds

5.3.1. Let X be a manifold of class C', F a separated polynormed space and f a mapping from X into F. One says that f is of class C' if for every chart (V, $\varphi$, E) of X, the mapping $f \circ \varphi^{-1}$ of $\varphi(V)$ into F is of class C'. For this, it is enough that this condition be satisfied for the charts of an atlas of X. The set of mappings of class C' from X into F forms a vector subspace of the space of all mappings from X into F. It is denoted by $\mathcal{C}'(X; F)$.

When F = K, one sets $\mathcal{C}'(X; K) = \mathcal{C}'(X)$; this is a sub-K-algebra of the algebra of mappings from X into K. The elements of $\mathcal{C}'(X)$ are also called morphic functions.

When X is an open subset of a Banach space, this terminology agrees with that of Nos. 2.3.1, 3.2.1 and 4.2.1.

5.3.2. Let X and Y be two manifolds of class C' and let f be a mapping from X into Y. One says that f is of class C' or is a morphism of manifolds (of class C') if it is continuous and if, for every chart (V, $\psi$, F) of Y, the mapping $\psi \circ f$ of the open submanifold $f^{-1}(V)$ into the Banach space F is of class $C'$. For this, it is enough that there exist an atlas $\mathcal{A}$ of Y such that, for every chart $(V, \psi, F) \in \mathcal{A}$, the set $f^{-1}(V)$ be open in X and the mapping $\psi \circ f$ of the open submanifold $f^{-1}(V)$ of X into F be of class $C'$. The set of morphisms from X into Y is denoted by $\mathcal{C}'(X; Y)$. When Y is a Banach space endowed with its canonical manifold structure, the definitions of 5.3.1. and 5.3.2 are coherent. A mapping of class $C^\omega$ is also called a *K-analytic mapping* (or simply analytic). When $K = \mathbf{C}$, one also says holomorphic mapping.

Let $(U, \varphi, E)$ be a chart of X and $(V, \psi, F)$ a chart of Y such that $f(U) \subset V$. The mapping $\psi \circ f \circ \varphi^{-1}$ of the open set $\varphi(U)$ of E into the open set $\psi(V)$ of F is called *the expression of f* in the given charts.

5.3.3. Suppose X and Y finite-dimensional; let $a \in X,\ b \in Y$ and $f$ a mapping from X into Y with $f(a) = b$. Suppose first that $f$ is of class $C'$ and consider coordinate systems $(U; \xi^1, \ldots, \xi^m)$ of X at $a$ and $(V; \eta^1, \ldots, \eta^n)$ of Y at $b$ respectively, with $f(U) \subset V$. Let $\xi$ be the mapping $(\xi^1, \ldots, \xi^m)$ of U into $K^m$. Then there exist functions $u^j$ of class $C'$ on the open set $\xi(U)$ of $K^m$, with values in K, such that the coordinates of a point $y = f(x)$ of Y, (for x in U), are given by the formulae:

(1)
$$
\eta^j(y) = u^j(\xi^1(x), \ldots, \xi^m(x)) \quad \text{for } 1 \leq j \leq n
$$
which is equivalent to:

(2)
$$
\eta^j \circ f = u^j(\xi^1, \ldots, \xi^m) \quad \text{for } 1 \leq j \leq n.
$$
One says that the preceding formulae constitute *the expression* of $f$ by means of the chosen coordinate systems.

*faisceau de fonctions à valeurs dans* $Y$ if it satisfies the following condition:

*Let* $(U_i)_{i \in I}$ *be a family of open sets of* $X$, *with union* $U$, *and let* $f$ *be a mapping of* $U$ *into* $Y$; *in order that* $f$ *belong to* $\mathcal{L}(U)$, *it is necessary and sufficient that* $f|U_i$ *belong to* $\mathcal{L}(U_i)$ *for every* $i$ *in* $I$.

5.4.2. Let $X$ and $Y$ be two manifolds; for every open set $U \subset X$, let $\mathcal{L}(U)$ be the set of morphisms of $U$ into $Y$; then $\mathcal{L}$ is a sheaf of mappings with values in $Y$.

When $Y = K$, the sheaf thus defined is denoted by $\mathscr{C}_X^{r'}$.

5.4.3. Let $X$ be a topological space and let $\mathcal{S}$ be a set of Banach spaces. For every $E \in \mathcal{S}$, let $\mathcal{F}_E$ be a sheaf of mappings on $X$ with values in $E$. Suppose that the family of the $\mathcal{F}_E$, for $E \in \mathcal{S}$, satisfies the following condition:

For every $x \in X$, there exist an open neighbourhood $U$ of $x$, a space

$E_0 \in \mathcal{S}$, and a homeomorphism $\varphi$ of U onto an open set of E_0, such that, for every open set $V \subset U$ and every $E \in \mathcal{S}$, the set $\mathcal{F}_E(V)$ consists of the functions $g \circ \varphi$, where $g$ ranges over the space $\mathcal{C}^r(\varphi(V); E)$.

Then there exists on X a structure of manifold of class $C^r$ and of type $\mathcal{S}$, and only one, compatible with the given topology on X and for which $\mathcal{F}_E$ is the sheaf of functions of class $C^r$ on X with values in E.

5.4.4. Let X be a topological space and let $\mathcal{F}$ be a sheaf of functions with values in K, satisfying the following condition: for every point x of X, there exist an integer n, an open neighbourhood U of x and a homeomorphism $\varphi$ of U onto an open set of $K^n$, such that, for every open set V of U, the set $\mathcal{F}(V)$ consists of the functions $g \circ \varphi$ where $g$ ranges over the set of functions of class $C^r$ with values in K on the open set $\varphi(V)$ of $K^n$.

Then there exists on X a structure of locally finite-dimensional manifold of class $C^r$ and only one such that $\mathcal{F} = \mathcal{C}^r_X$.

5.4.5. Let $X$ and $X'$ be two $C^r$-class varieties, locally of finite dimension, and let $f$ be a continuous mapping of X into X'. For $f$ to be a morphism, it is necessary and sufficient that for every open set U' of X' and every function $g \in \mathcal{C}^r(U'; K)$, the function $g \circ f$ belong to $\mathcal{C}^r(U; K)$, where $U = f^{-1}(U')$.

### 5.5. Tangent spaces, tangent linear mappings

5.5.1. Let X be a variety and let $a \in X$. Consider the pairs $(c, h)$ where $c = (U, \varphi, E)$ is a chart of the variety X at $a$ and where $h$ is an element of E. Two such pairs $(c, h)$ and $(c', h')$ are said to be equivalent if the derivative at $\varphi(a)$ of the mapping $\varphi' \circ \varphi^{-1}$ (which is defined on a neighbourhood of $\varphi(a)$) transforms $h$ into $h'$. We thus obtain an equivalence relation between pairs $(c, h)$ and call a tangent vector at $a$ to X a class of equivalent pairs $(c, h)$ (Ens., Chapter II, § 6, No. 9).

The tangent vectors at $a$ to X form a set denoted by $T_a(X)$. If $c = (U, \varphi, E)$ is a chart of the variety X at $a$, the mapping $\theta_c$ of E into $T_a(X)$ which associates to an element $h$ of E the tangent vector represented by the pair $(c, h)$ is a bijection. If one transports to $T_a(X)$, by means of $\theta_c$, the structure of topological K-vector space of E, the structure thus obtained does not depend on the choice of $c$ and makes $T_a(X)$ a Banach space, called the tangent space to X at $a$. The dimension (finite or $+\infty$) of $T_a(X)$ is equal to the dimension of X at $a$.

5.5.2. Let X, Y be two manifolds, $f$ a morphism of X into Y and $a$ a point of X. Consider a chart $c = (U, \varphi, E)$ of X at $a$ and a chart $c' = (V, \psi, F)$ of Y at $b$ with $f(U) \subset V$; the mapping $\Phi = \psi \circ f \circ \varphi^{-1}$ of $\varphi(U)$ into F is of class $C^r$, and its derivative $D\Phi(\varphi(a))$ at the point $\varphi(a)$ is a continuous linear mapping of E into F. The continuous linear mapping $\theta_{c'} \circ D\Phi(\varphi(a)) \circ \theta_c^{-1}$ of $T_a(X)$ into $T_b(Y)$ does not depend on the charts $c$ and $c'$ chosen; it is denoted by $T_a(f)$ and is called the tangent linear mapping to $f$ at $a$. If $g$ is a morphism of $Y$ into a manifold $Z$, we have:

$$
T_a(g \circ f) = T_{f(a)}(g) \circ T_a(f).
$$

5.5.3. Let $f : X \to Y$ be a morphism of manifolds. If $f$ is locally constant, we have $T_a(f) = 0$ for every $a$ in $X$. Conversely, if $T_a(f) = 0$ for every $a \in X$ and if the field $K$ is of characteristic 0, then $f$ is locally constant.

5.5.4. Let $U$ be an open set of a manifold $X$ and $f$ the canonical injection of $U$ into $X$; for every point $a$ of $U$, the mapping $T_a(f)$ of $T_a(U)$ into $T_a(X)$ is an isomorphism of topological vector spaces, by means of which these two spaces will henceforth be identified.

5.5.5. Let $U$ be an open set of a Banach space $E$; if $\iota$ is the canonical injection of $U$ into $E$, the triple $c = (U, \iota, E)$ is a chart of $U$, and the atlas $\{c\}$ defines the manifold structure of $U$. Given a point $a$ of $U$, the mapping $\theta_c$ is an isomorphism of topological vector spaces of $E$ onto $T_a(U)$; the inverse isomorphism will be denoted by $\zeta_E(a)$.

Let $f$ be a mapping of class $C^r$ of $U$ into an open set $V$ of a Banach space $F$; for every point $a$ of $U$, we have:

$$
Df(a) \circ \zeta_E(a) = \zeta_F(f(a)) \circ T_a(f)
$$

where $Df(a)$ is the derivative of $f$ at $a$ (1.2.1). In other words, the diagram:

$$
\begin{array}{ccc}
T_a(U) & \xrightarrow{T_a(f)} & T_{f(a)}(V) \\
\downarrow \zeta_E(a) & & \downarrow \zeta_F(f(a)) \\
E & \xrightarrow{Df(a)} & F
\end{array}
$$

is commutative.

5.5.6. A cotangent vector to $X$ at $a$, or also a tangent covector or simply a covector at $a$, is any continuous linear form on the topological vector space $T_a(X)$; these covectors are therefore the elements of the topological dual $T_a(X)'$ of the tangent space to $X$ at $a$. This space will be endowed with the topology of uniform convergence on the bounded subsets of $T_a(X)$: endowed with this topology, $T_a(X)'$ is a Banach space which is called the cotangent space to $X$ at $a$. It is also denoted by $T'_a(X)$.

Let $f$ be a morphism of $X$ into a Banach space $E$. The differential of $f$ at $a$, denoted by $d_a f$ or $df_a$, is the continuous linear mapping $\zeta_E(f(a)) \circ T_a(f)$ of $T_a(X)$ into $E$. For $t \in T_a(X)$, one sometimes denotes by t(f) or t . f the value $d_a f(t)$ of the linear mapping $d_a f$ at the point $t$. The mapping $f \mapsto d_a f$ is linear.

If $E = K$, the differential $d_a f$ of $f$ at $a$ is a covector of $X$ at $a$.

Let $E, F, G$ be three Banach spaces and let $(u, v) \mapsto u . v$ be a continuous bilinear mapping of $F \times G$ into $E$. Let $f$ (resp. $g$) be a morphism of $X$ into $F$ (resp. $G$). Then the mapping $f . g : x \mapsto f(x) . g(x)$ is a morphism of $X$ into $E$ and, for every $t \in T_a(X)$, we have:

$$
d_a(f . g)(t) = f(a) . d_a g(t) + d_a f(t) . g(a).
$$

Take in particular $G = E$ and $F = K$, the bilinear mapping considered being multiplication. We then have:

$$
d_a(fg) = f(a)d_ag + g(a)\ d_af.
$$

5.5.7. Let $X$ be a locally finite-dimensional variety and let $\xi^1, \ldots, \xi^m$ be morphic functions defined in an open neighbourhood $U$ of a point $a$ of $X$. The following conditions are equivalent:

(i) there exists an open neighbourhood $V$ of $a$ contained in $U$, such that the functions $\xi^i|V$ (for $1 \leq i \leq m$) form a system of coordinates of $X$ in $V$;

(ii) the differentials $d_a \xi^i$ for $1 \leq i \leq m$ form a basis of $T_a(X)'$;

(iii) the mapping $\xi = (\xi^1, \ldots, \xi^m)$ of $U$ into $K^m$ is étale at $a$ (see No. 5.7.6).

For the differentials $d_a \xi^1, \ldots, d_a \xi^m$ to be linearly independent, it is necessary and sufficient that there exist a neighbourhood $V$ of $a$, contained in $U$, such that the functions $\xi^i|V$ form part of a system of coordinates of $X$ in $V$.

5.5.8. Let $X$ be a locally finite-dimensional variety and let $\xi = (\xi^1, \ldots, \xi^m)$ be a system of coordinates of $X$ in an open set $U$. Let $a \in U$: we denote by $(\partial_{1,a}, \ldots, \partial_{m,a})$ the basis of the tangent space $T_a(X)$ dual to the basis $(d_a \xi^1, \ldots, d_a \xi^m)$ of $T_a(X)'$. We therefore have:

$$
\partial_{i,a}(\xi^j) = \delta_{i,j} \quad \text{(Kronecker index)}.
$$

The tangent vector $\partial_{i,a}$ is also denoted by $(\partial/\partial \xi^i)_a$.

Let $f$ be a function of class $C^r$ on $U$, with values in a Banach space $E$. We denote by $\partial_i f$ or $\partial f/\partial \xi^i$ the function $a \mapsto \partial_{i,a}(f)$: this is a function of class $C^{r-1}$ on $U$ with values in $E$ (a continuous function if $r = 1$). Its value at a point $a$ of $U$ is sometimes denoted by $(\partial f/\partial \xi^i)_a$. For all $t \in T_a(X)$, we have:

$$
d_a f(t) = \sum_{i=1}^m d_a \xi^i(t) \frac{\partial f}{\partial \xi^i}(a),
$$

which may also be written:

$$
d_a f = \sum_{i=1}^m \frac{\partial f}{\partial \xi^i}(a) d_a \xi^i.
$$

These notations are consistent with those of 1.6.3.

5.5.9. Let $X$ and $Y$ be two varieties and $f$ a morphism of $X$ into $Y$. The *rank of* $f$ at a point $a$ of $X$, denoted $\mathrm{rg}_a f$, is the rank (finite or equal to $+\infty$) of the linear mapping $T_a(f)$. The mapping $a \mapsto \mathrm{rg}_a f$ is lower semicontinuous.

### 5.6. Products of varieties

5.6.1. Let $X$ and $X'$ be two sets and let $c = (U, \varphi, E)$ (resp. $c' = (U', \varphi, E')$) be a chart of $X$ (resp. $X'$). The triple

$$
(U \times U', \varphi \times \varphi', E \times E')
$$

is a chart of the product set $X \times X'$, denoted $c \times c'$.

5.6.2. Let $X$ and $X'$ be two varieties of class $C^r$. There exists on the product set $X \times X'$ one and only one structure of a variety of class $C^r$ such that $c \times c'$ is a chart of $X \times X'$ for every chart $c$ of $X$ and every chart $c'$ of $X'$. Endowed with this structure, $X \times X'$ is called the *product variety* of the varieties $X$ and $X'$. One defines analogously the product of any finite number of varieties. The topology of the variety $X \times X'$ is the product topology of the topologies of $X$ and $X'$. For $a \in X$ and $b \in X'$, one has:

$$
\dim_{(a,b)}(X \times X') = \dim_a X + \dim_b X'.
$$

5.6.3. Let $X$ and $X'$ be two varieties, and let $X \times X'$ be their product. Let $a \in X$ and let $a' \in X'$. The canonical projections

$$
\mathrm{pr}_1 : X \times X' \to X \quad \text{and} \quad \mathrm{pr}_2 : X \times X' \to X'
$$

are morphisms. Let $\pi_i \ (i = 1, 2)$ be their tangent linear mappings at the point $(a, a')$. The mapping

$$
(\pi_1, \pi_2) : T_{(a,a')}(X \times X') \to T_a(X) \times T_{a'}(X')
$$

is an *isomorphism*, which makes it possible *to identify the tangent space to* $X \times X'$ *at* $(a, a')$ *with the product* $T_a(X) \times T_{a'}(X')$.

The injection of $T_a(X)$ into $T_{(a,a')}(X \times X')$ resulting from this identification is the tangent linear mapping at $a$ of the morphism $x \mapsto (x, a')$ of $X$ into $X \times X'$; there is an analogous result for the injection of $T_{a'}(X')$ into $T_{(a,a')}(X \times X')$.

5.6.4. Let $W, X$ and $X'$ be three varieties, and let $f : W \to X, f' : W \to X'$ be two mappings. For the mapping

$$
(f, f') : W \to X \times X'
$$

to be a morphism, it is necessary and sufficient that $f$ and $f'$ be morphisms (this justifies the use of the term « product », cf. Ens., Chap. IV, § 2, No. 4). In this case, if $a$ is a point of $W$, we have:

$$
T_a(f, f') = (T_a(f), T_a(f'))
$$

taking into account the identification made above.

5.6.5. Let $f : X \to Y$ and $f' : X' \to Y'$ be morphisms of varieties. Then $f \times f' : X \times X' \to Y \times Y'$ is a morphism. If $a \in X$ and $a' \in X'$, we have:

$$
T_{(a, a')}(f \times f') = T_a(f) \times T_{a'}(f')
$$
$$
\mathrm{rg}_{(a, a')}(f \times f') = \mathrm{rg}_a f + \mathrm{rg}_{a'} f'.
$$

5.6.6. Let $X_1, X_2$ and $Z$ be three varieties and $f$ a morphism of $X_1 \times X_2$ into $Z$. Let $a \in X_1$ and $b \in X_2$. The tangent linear mapping to the partial mapping $x \mapsto f(x, b)$ (resp. $y \mapsto f(a, y)$) of $X_1$ (resp. $X_2$) into $Z$ is denoted by $T^1_{(a, b)}(f)$ (resp. $T^2_{(a, b)}(f)$). If we identify $T_{(a, b)}(X_1 \times X_2)$ with $T_a(X_1) \times T_b(X_2)$, we have:

$$
T_{(a, b)}(f) \cdot (u, v) = T^1_{(a, b)}(f) \cdot u + T^2_{(a, b)}(f) \cdot v
$$

for every $u \in T_a(X_1)$ and every $v \in T_b(X_2)$.

5.6.7. (« Theorem on implicit functions »). With the hypotheses and notation of the preceding number, suppose in addition that $T^2_{(a, b)}(f)$ is bijective. There then exists an open neighbourhood $U$ of $a$ in $X_1$ and an open neighbourhood $V$ of $b$ in $X_2$ having the following property: for every $x \in U$, there exists one and only one point $g(x)$ of $V$ such that $f(x, g(x)) = f(a, b)$, and the mapping $g$ is a morphism of $U$ into $V$. For every $x \in U$, we have:

$$
T_x(g) = - (T^2_{(x, g(x))}(f))^{-1} \circ T^1_{(x, g(x))}(f).
$$

### 5.7. Immersions, étale morphisms

5.7.1. Let $X$ and $Y$ be two manifolds, $f$ a morphism of $X$ into $Y$ and $a$ a point of $X$. Put $b = f(a)$. The following conditions are equivalent:
(i) The linear mapping $T_a(f)$ is injective and its image is a closed vector subspace of $T_b(Y)$ admitting a topological supplement $^1$;

(ii) There exist a Banach space $F$, a closed vector subspace $E$ of $F$ admitting a topological supplement, and charts $(U, \varphi, E)$ of $X$ at $a$ and $(V, \psi, F)$ of $Y$ at $b$ such that $f(U) \subset V$ and $\varphi = \psi \circ (f|U)$.

(iii) There exist an open neighbourhood $U$ of $a$, an open neighbourhood $V$ of $b$ containing $f(U)$, a manifold $Z$, a point $c$ of $Z$, and an isomorphism of manifolds $g$ of $U \times Z$ onto $V$ such that $f(x) = g(x, c)$ for all $x \in U$.

(iv) There exist an open neighbourhood $U$ of $a$, an open neighbourhood $V$ of $b$ and a morphism $q$ of $V$ into $X$ with $f(U) \subset V$, and $q(f(x)) = x$ for all $x \in U$.

When $X$ and $Y$ are finite-dimensional, the preceding conditions are also equivalent to the following:

(v) There exist an open neighbourhood $U$ of $a$, a coordinate system $(\eta^1, \ldots, \eta^n)$ of $Y$ in an open neighbourhood $V$ of $b$ containing $f(U)$ and an integer $m \leq n$ such that $\eta^j \circ f = 0$ for $m < j \leq n$ and the functions $\eta^1 \circ f, \ldots, \eta^m \circ f$ form a coordinate system of $X$ in $U$.

If properties (i) to (iv) are satisfied, we say that $f$ is an immersion at $a$.

The set of points where $f$ is an immersion is open in $X$; if this open set is all of $X$, we say that $f$ is an immersion.

For $f$ to be an immersion, it is necessary and sufficient that $X$ can be covered by open sets $U_i$ such that, for every $i, f|U_i$ is an isomorphism of $U_i$ onto a subvariety of $Y$ (cf. No. 5.8.3).

5.7.2. Examples:
(a) If $X$ is an open set in a variety $Y$, the canonical injection of $X$ into $Y$ is an immersion.
(b) Let $E$ and $F$ be two Banach spaces and let $u$ be a continuous linear mapping of $E$ into $F$. Then $u$ is an immersion if and only if $u$ is an isomorphism of $E$ onto a closed vector subspace of $F$ admitting a topological supplement.

5.7.3. Let $f : X \to Y$ and $g : Y \to Z$ be two morphisms. If $f$ and $g$ are immersions, $g \circ f$ is an immersion. Conversely, if $g \circ f$ is an immersion, then $f$ is an immersion. If $f : X \to Y$ and $f' : X' \to Y'$ are immersions, $f \times f'$ is an immersion.

5.7.4 Suppose that $X$ and $Y$ are varieties of finite dimension over a field $K$ of characteristic 0. If $f : X \to Y$ is an injective morphism, the set of points of $X$ where $f$ is an immersion is an open dense set

$^1$ Every closed vector subspace of finite codimension of a Banach space admits a topological supplement; if $K = \mathbf{R}$ or $\mathbf{C}$, the same is true of every finite-dimensional vector subspace (necessarily closed).

in $X$. If K = R or C, this result remains true if one supposes only that X is of finite dimension.

5.7.5. Let $f : X \to Y$ be an immersion and let $g$ be a continuous mapping of a variety Z into X. For $g$ to be a morphism, it is necessary and sufficient that $f \circ g$ be a morphism.

5.7.6. Let $f : X \to Y$ be a morphism, and let $a$ be in X. The following two properties are equivalent:
(i) $T_a(f)$ is bijective.
(ii) There exists an open neighbourhood U of $a$ and an open neighbourhood V of $f(a)$ such that $f$ induces an isomorphism of U onto V.
When these properties are satisfied, one says that $f$ is a local isomorphism at $a$, or that $f$ is étale at $a$. If this holds for every $a \in X$, one says that $f$ is étale, or is an étalement, or that X is étalé in Y (by means of $f$). For a morphism to be étale, it is necessary and sufficient that it be both an immersion (No. 5.7.1) and a submersion (No. 5.9.1.).

5.7.7. Let $f : X \to Y$ be an immersion; suppose the variety X is purely finite-dimensional. Then $f$ is étale in each of the following two cases:
(i) $\dim Y = \dim X$;
(ii) $f$ is surjective and the topology of X has a countable basis of open sets.

5.7.8. For a morphism $f$ to be an isomorphism onto an open subvariety (resp. an isomorphism), it is necessary and sufficient that $f$ be étale and injective (resp. étale and bijective).

### 5.8. Inverse images of structures of variety, subvarieties

5.8.1. Let X be a topological space, Y a variety and $f$ a mapping of X into Y. Consider the following conditions:
(QR) (resp. (R)) For every $a \in X$, there exists an open neighbourhood U of a in X and a chart $(V, \varphi, E)$ of the variety Y at $f(a)$ such that $f(U) \subset V$ and $\varphi \circ f$ induces a homeomorphism of U onto the intersection of $\varphi(V)$ with a closed vector subspace (resp. closed and admitting a topological complement) F of E.
If condition (QR) is satisfied, there exists on X one and only one structure of variety for which the triples $(U, \varphi \circ f, F)$ (with the notation of (QR)) are charts of X. It is called the inverse image structure of the structure of variety of Y by $f$. Its topology is that of X.
For there to exist on X a structure of variety compatible with the given topology and for which $f$ be an immersion, it is necessary and sufficient that condition (R) be satisfied. This structure is then unique: it is the inverse image by $f$ of the structure of variety of $Y$.

5.8.2. The condition (R) above is in particular satisfied when, for every $a \in X$, there exists an open neighbourhood $U$ of $a$ such that $f|U$ is a homeomorphism of $U$ onto an open set of $Y$. In this case, the variety $X$ obtained is étalé over $Y$ (5.7.6).

5.8.3. Suppose now that $X$ is a topological subspace of $Y$, $f$ being the canonical injection. If $f$ satisfies condition (R) (resp. (QR)) of No. 5.8.1, one says that $X$, endowed with the inverse image structure of the structure of variety of $Y$ by $f$, is a subvariety (resp. quasi-subvariety) of $Y$. A subvariety is a quasi-subvariety.

Every quasi-subvariety is locally closed; every open set is a subvariety and its structure is that defined in No. 5.2.3.

celle de $Y$ (Ens., ch. IV, § 2, No. 4).

5.8.6. If $X$ is a submanifold (resp. quasi-submanifold) of $Y$ and if $Y$ is a submanifold of a manifold $Z$, then $X$ is a submanifold (resp. quasi-submanifold) of $Z$.

5.8.7. Let $X_i$ (for $i = 1, 2$) be a manifold and let $Y_i$ be a submanifold (resp. quasi-submanifold) of $X_i$ (for $i = 1, 2$). Then $Y_1 \times Y_2$ is a submanifold (resp. quasi-submanifold) of $X_1 \times X_2$.

5.8.8. Let X be a quasi-submanifold of a manifold Y; let x be a point of X, and denote by f the canonical injection of X into Y. The map T_x(f) : T_x(X) → T_x(Y) is injective and enables us to identify the space T_x(X) with a closed vector subspace of T_x(Y). The quotient topological vector space T_x(Y)/T_x(X) is a Banach space, called the transverse space to X (in Y) at x. Its dimension (finite or +∞) is called the codimension of X in Y at the point x.

If moreover X is a submanifold of Y, then the space T_x(X) admits a topological complement in T_x(Y).

5.8.9. Let f be a mapping of a manifold X into a manifold Y, and let Γ be its graph. In order that f be a morphism, it is necessary and sufficient that the following two conditions be satisfied:
(i) Γ is a submanifold of X × Y.
(ii) For every (x, y) ∈ Γ, one has
$$
T_{(x,y)}(X \times Y) = T_{(x,y)}(\Gamma) \oplus T_y(Y).
$$
If this is so, the mapping $\mathrm{pr}_1$ induces an isomorphism of $\Gamma$ onto X, and $T_{(x,y)}(\Gamma)$ is identified with the graph of $T_x(f)$.

In particular, the diagonal of X × X is a submanifold of X × X.

5.8.10. Let Y be a manifold, and let (f_i)_{i∈I} be a finite family of morphic functions on Y. Let X be the set of x ∈ Y such that f_i(x) = 0 for every i. Make the following assumption:
(J) For every x ∈ X, the differentials d_x f_i are linearly independent in T'_x(Y).

Then X is a closed submanifold of Y, the tangent space T'_x(X) is the subspace of T_x(Y) formed by the α such that α . f_i = 0 for every i in I. Moreover, the codimension of X in Y is equal to Card (I) at each of its points.

5.8.11. (Simple zeros of an ideal). Let a be an ideal of the algebra of polynomials K[X_1, ..., X_n]. A point x = (x_1, ..., x_n) of K^n is called a zero of a if f(x) = 0 for every f ∈ a. If x ∈ K^n, let S_x denote the subalgebra of K(X_1, ..., X_n) formed by the fractions f/g, with f, g ∈ K[X_1, ..., X_n], and g(x) ≠ 0; let a_x denote the ideal of S_x generated by a in S_x. A point x is called a simple zero of a if it is a zero of a and if the following condition is satisfied:
(S) There exists a finite sequence (f_1, ..., f_m) of elements of a which generate the ideal a_x and whose differentials at x are linearly independent. (This condition is equivalent to saying that the local ring S_x/a_x is regular (Alg. Comm., to appear).)
Let Z (resp. Z_s) be the set of zeros (resp. of simple zeros) of a. The set Z is closed in K^n, Z_s is open in Z, and Z_s is a submanifold of $K^n$. If $x \in Z_s$, the ideal $K[X_1, \ldots, X_n] \cap a_x$ consists of the polynomials $f$ vanishing in a neighbourhood of $x$ in $Z_s$.

Let $\bar{a}$ be the ideal of polynomials vanishing on $Z$. If $K$ is algebraically closed, the set of simple zeros of $a$ is dense in $Z$.

5.8.12. Let $X$ be a manifold and $L$ the set of pairs $(x, Z)$ where $x$ is a point of $X$ and $Z$ a submanifold of $X$ containing $x$. Given two pairs $\pi = (x, Z)$ and $\pi' = (x', Z')$, we shall denote by $R\{\pi, \pi'\}$ the relation:

« If $x = x'$ and there exists a neighbourhood $U$ of $x$ such that $U \cap Z = U \cap Z'$ ». Then $R$ is an equivalence relation in $L$; we denote by $\gamma_x(Z)$ the equivalence class of the pair $(x, Z) \in L$. On the set $J = L/R$, there exists one and only one manifold structure satisfying the following condition:
For every subvariety $Z$ of $X$, the mapping $x \mapsto \gamma_x(Z)$ from $Z$ into $J$ is an isomorphism of $Z$ onto an open subvariety of $J$.
We say that $J$ is the manifold of germs of subvarieties of $X$ (cf. Top. Gén., Chapter I, 4th ed., § 6, No. 10).
The mapping $\rho : J \to X$ defined by $\rho(\gamma_x(Z)) = x$ is an immersion; we call it the canonical immersion of $J$ into $X$.
If $X$ is a separated analytic manifold of finite dimension, the same is true of $J$.

### 5.9. Submersions and quotient manifolds

5.9.1. Let $f : X \to Y$ be a morphism of varieties, let $a$ be a point of $X$, and put $b = f(a)$. The following conditions are equivalent:
(i) The linear mapping $T_a(f)$ is surjective, and its kernel admits a topological complement in $T_a(X)$.
(ii) There exist a chart $(U, \varphi, E)$ of $X$ at $a$, a chart $(V, \psi, F)$ of $Y$ at $b$, and a surjective continuous linear mapping $u$ of $E$ into $F$ such that
$$
f(U) \subset V, \quad \psi \circ f = u \circ \varphi
$$
and such that the kernel of $u$ admits a topological complement in $E$.
(iii) There exist an open neighbourhood $U$ of $a$, an open neighbourhood $V$ of $b$ containing $f(U)$, and a morphism $g$ of $U$ into a variety $Z$ such that the mapping $(f, g)$ of $U$ into $V \times Z$ is an isomorphism.
(iv) There exist an open neighbourhood $V$ of $b$ and a morphism $s$ of $V$ into $X$ such that $s(b) = a$ and $f(s(y)) = y$ for every $y$ in $V$ ("local section").
When $X$ and $Y$ are finite-dimensional, the preceding conditions are equivalent to the following condition:
(v) There exist an open neighbourhood $U$ of $a$, an open neighbourhood $V$ of $b$ containing $f(U)$, and a coordinate system $(\eta^1, \ldots, \eta^n)$ on $V$ such that the functions $\eta^i \circ f$ on $U$ form part of a coordinate system on $U$.
If properties (i) to (iv) are satisfied, one says that $f$ is a submersion at $a$. The set of points where $f$ is a submersion is open in $X$; if this open set is the whole of $X$, one says that $f$ is a submersion.

5.9.2. Let $f : X \to Y$ and $g : Y \to Z$ be two morphisms. If $f$ and $g$ are submersions, then so is $g \circ f$; conversely, if $g \circ f$ is a submersion and $f$ is surjective, then $g$ is a submersion.

5.9.3. If $f : X \to Y$ and $f' : X' \to Y'$ are submersions, $f \times f'$ is a submersion.

5.9.4. A submersion $f : X \to Y$ is an open mapping (cf. Top. gén., chap. I, 4e éd., § 5, n° 1); in particular, the equivalence relation R defined by $f$ is open, $f$ defines by passing to the quotient a homeomorphism of $X/R$ onto $f(X)$, and $f(X)$ is open in $Y$.

5.9.5. Let $R$ be an equivalence relation on a variety $X$. We say that $R$ is regular if there exists on the quotient space $X/R$ a structure of a variety such that the canonical projection $p : X \to X/R$ is a submersion; this structure of a variety is then unique; it is the quotient of that of $X$ (Ens., ch. IV, § 2, n° 6): in other words, in order that a mapping $g$ of $X/R$ into a variety $Y$ be a morphism, it is necessary and sufficient that $g \circ p$ be a morphism of $X$ into $Y$.

Let $C \subset X \times X$ be the graph of $R$. In order that $R$ be regular, it is necessary and sufficient that the following two conditions be satisfied:
(i) $C$ is a subvariety of $X \times X$.
(ii) The mapping $\mathrm{pr}_1$ of $C$ into $X$ is a submersion.

Condition (ii) also means that if $a$ and $b$ are congruent modulo $R$, there exists an open neighbourhood $U$ of $a$ and a morphism $s$ of $U$ into $X$ such that $s(a) = b$ and such that $s(x)$ is congruent to $x$ modulo $R$ for every $x \in U$.

Suppose that $R$ is regular. In order that the quotient variety $X/R$ be separated, it is necessary and sufficient that the graph of $R$ be closed in $X \times X$.

5.9.6. Let $X$ and $X'$ be two manifolds, $R$ and $R'$ regular equivalence relations on $X$ and $X'$, and let $f : X \to X'$ be a morphism compatible with the relations $R$ and $R'$. The mapping $\tilde{f} : X/R \to X'/R'$ deduced from $f$ by passing to the quotients is then a morphism.

5.9.7. (« Transitivity of quotients ») Let $R$ and $S$ be two equivalence relations on a manifold $X$ such that $R$ entails $S$, and let $S/R$ be the quotient equivalence relation on $X/R$. Suppose that $R$ is regular. Then, for $S$ to be regular, it is necessary and sufficient that $S/R$ be so; if this is the case, the canonical bijection

$$
(X/R)/(S/R) \to X/S
$$

is an isomorphism of manifolds.

5.9.8. (« Products of quotients ») Let $(X_i)_{i \in I}$ be a finite family of manifolds, each endowed with a regular equivalence relation $R_i$. Let $X = \prod_{i \in I} X_i$, and let $R$ be the equivalence relation on $X$ which is the product of the $R_i$ (cf. Top. Gén., chap. I, 4e éd., § 5, n° 3, cor. de la prop. 8). Then $R$ is regular, and the canonical bijection of $X/R$ onto $\prod_{i \in I} (X_i/R_i)$ is an isomorphism of manifolds.

### 5.10. Subimmersions

5.10.1. Let $f : X \to Y$ be a morphism of manifolds and let $\Gamma$ be the graph of $f$. The mapping $j : x \mapsto (x, f(x))$ is an immersion of $X$ into $X \times Y$, whose image is the submanifold $\Gamma$, and $f = \mathrm{pr}_2 \circ j$ is the composite of the immersion $j$ followed by the submersion $\mathrm{pr}_2$.

Let $a \in X$. We say that $f$ is a submersion at $a$ if there exists an open neighbourhood $U$ of $a$, a manifold $Z$, a submersion $s$ of $U$ into $Z$ and an immersion $i$ of $Z$ into $Y$ such that $f|U = i \circ s$. The set of points of $X$ at which $f$ is a submersion is an open set of $X$; if this open set is all of $X$, we say that $f$ is a submersion.

5.10.2. Immersions and submersions are submersions. If $f : X \to Y$ is a submersion, $g : Y \to Z$ an immersion and $h : W \to X$ a submersion, then $g \circ f \circ h$ is a submersion.

If $f$ and $f'$ are submersions, $f \times f'$ is a submersion.

5.10.3. In order that $f : X \to Y$ be a submersion at a point $a$ of $X$, it is necessary and sufficient that there exist a chart $(U, \varphi, E)$ of $X$ at $a$, a chart $(V, \psi, F)$ of $Y$ at the point $f(a)$ and a continuous linear mapping $g$ of $E$ into $F$ such that:
(i) $f(U) \subset V,\ g(\varphi(U)) \subset \psi(V)$ and $f|U = \psi^{-1} \circ g \circ \varphi$;
(ii) the kernel (resp. the image) of $g$ is a closed subspace of $E$ (resp. $F$) admitting a topological complement.

5.10.4. Let $X$ and $Y$ be two finite-dimensional manifolds. In order that a morphism $f$ of $X$ into $Y$ be a submersion at a point $a$ of $X$, it is necessary and sufficient that there exist a coordinate system $(\xi^1, \ldots, \xi^m)$ of $X$ at $a$, a coordinate system $(\eta^1, \ldots, \eta^n)$ of $Y$ at $f(a)$ and an integer $k \leq \inf(m, n)$ such that
$$
\eta^i \circ f = \xi^i \quad \text{for } 1 \leq i \leq k \\
\eta^i \circ f = 0 \quad \text{for } k < i \leq n.
$$

5.10.5. Let $f : X \to Y$ be a submersion. For every $b \in Y$, $f^{-1}(b)$ is a submanifold of $X$; the subspace of $T_a(X)$ tangent to the submanifold $f^{-1}(b)$ at the point $a \in f^{-1}(b)$ is the kernel of $T_a(f)$.

5.10.6. (“Constant rank theorem”) Let $f : X \to Y$ be a morphism of manifolds and let $a \in X$. If $f$ is a subimmersion at $a$, then $\mathrm{rg}_x f = \mathrm{rg}_a f$ for $x$ in a neighbourhood of $a$.

Conversely, suppose that the field $K$ is of characteristic zero. Let $(U, \varphi, E)$ be a chart of $X$ at $a$ and let $(V, \psi, F)$ be a chart of $Y$ at $f(a)$, with $f(U) \subset V$. Put $g = \psi \circ f \circ \varphi^{-1}$. If there exist a closed vector subspace $E_1$ of $E$ and a closed vector subspace $F_1$ of $F$ such that for every $x \in U$, the subspace $E_1$ (resp. $F_1$) is a topological complement of the kernel (resp. of the image) of the derivative $Dg(\varphi(x))$ of $g$ at the point $\varphi(x)$, then $f$ is a subimmersion at $a$.

If $K$ is of characteristic zero (resp. $K = \mathbf{R}$ or $\mathbf{C}$) and if $Y$ is finite-dimensional (resp. $\mathrm{rg}_a f < +\infty$), then $f$ is a subimmersion at $a$ if and only if $\mathrm{rg}_x f = \mathrm{rg}_a f$ for every $x$ sufficiently near $a$.

If $K$ is of characteristic zero (resp. $K = \mathbf{R}$ or $\mathbf{C}$) and $Y$ (resp. $X$) is finite-dimensional, the set of points $x \in X$ where $f$ is a subimmersion is an open dense set in $X$.

5.10.7. ("Canonical factorization of a subimmersion") Every subimmersion is the composite of a submersion and an immersion. More precisely, let $f : X \to Y$ be a subimmersion, and let $J$ be the manifold of germs of submanifolds of $Y$ (5.8.12). Let $x$ be in $X$ and $y = f(x)$; there exist open neighbourhoods $U$ of $x$ such that $f|U$ is a submersion of $U$ onto a submanifold $Z$ of $Y$; the element $\gamma_y(Z)$ of $J$ depends only on $x$ and not on the neighbourhood $U$ chosen, and, if it is denoted by $\lambda(x)$, the mapping $\lambda$ is a submersion of $X$ into $J$; if $\rho$ denotes the canonical immersion of $J$ into $Y$, one has $f = \rho \circ \lambda$. If $f$ is an immersion, the morphism $\lambda$ of $X$ into $J$ is étale.

If $g$ is a surjective submersion of $X$ onto a manifold $Z$ and $h$ a morphism of $Z$ into $Y$ such that $f = h \circ g$, there exists a unique submersion $\mu$ of $Z$ into $J$ such that $\lambda = \mu \circ g$.

### 5.11. Fibered products and inverse images

5.11.1. Let $F$ be a Banach space, $(E_i)_{i \in I}$ a finite family of Banach spaces, and $f = (f_i)_{i \in I}$ a family of continuous linear mappings $f_i$ of $E_i$ into $F$. Let $E$ be the product of the $E_i$ and $f$ the continuous linear mapping of $E$ into $F^I$ product of the $f_i$. Finally, let $D$ be the closed subspace of $F^I$ consisting of the $(y_i)_{i \in I}$ such that $y_i$ is independent of $i$ (the “diagonal” of $F^I$). One says that the family $f$ is transversal if the continuous linear mapping obtained by composing $f$ with the canonical projection of $F^I$ onto the quotient $F^I/D$ is surjective and if its kernel $f^{-1}(D)$ admits a topological complement.

If the spaces $E_i$ and $F$ are all finite-dimensional, the family $f$ is transversal if and only if one has:

$$
\operatorname{codim} \left( \bigcap_i \operatorname{Im} f_i \right) = \sum_i \operatorname{codim} (\operatorname{Im} f_i)
$$

If $I = \{1, 2\}$, the pair $(f_1, f_2)$ is transversal if and only if the mapping

$$
f_1 + f_2 : E_1 \oplus E_2 \to F
$$

is surjective and if its kernel admits a topological complement (if $E_1$ and $E_2$ are finite-dimensional, it comes to the same thing to say that

$$
\operatorname{Im} f_1 + \operatorname{Im} f_2 = F).
$$

5.11.2. Let $S$ be a manifold, $(X_i)_{i \in I}$ a finite family of manifolds, and $f = (f_i)_{i \in I}$ a family of morphisms $f_i$ of $X_i$ into $S$. Let $P$ be the subset of the product $X$ of the $X_i$ consisting of the points $(x_i)_{i \in I}$ such that $f_i(x_i)$ is independent of $i$. Let $x \in P$ and let $y = f_i(x_i) \in F$. One says that the family $f$ is *transversal* at the point $x$ of $P$ if the mappings $T_x(f_i)$ form a transversal family of continuous linear mappings with values in the Banach space $T_y(S)$. One says that $f$ is *transversal* if it is transversal at every point of $P$.

If $f$ is transversal, then $P$ is a *submanifold* of $X$, called the *fibred product of the family of the $X_i$ over $S$* (relative to the family $f$), and denoted by $\prod_{i \in I} X_i$ (or more simply $X_1 \times_S X_2$ when $I = \{1, 2\}$, for example). For every point $x = (x_i)$ of $P$, the tangent space $T_x(\prod_{i \in I} X_i)$ is the subspace of $\prod T_{x_i}(X_i)$ formed by the tangent vectors $t = (t_i)$ such that $T_{x_i}(f_i) \cdot t_i$ is independent of the index $i$.

If $f_1 : X_1 \to Y$ is a *submersion* and $f_2 : X_2 \to Y$ a morphism, the pair $(f_1, f_2)$ is transversal.

5.11.3. (*Universal property of fibred products*) Let $f = (f_i)_{i \in I}$ be a transversal family of morphisms $f_i : X_i \to S$, and let $P$ be the fibred product of the $X_i$ over $S$; for every $i \in I$, let $\pi_i$ denote the morphism from $P$ into $X_i$ obtained by restriction to $P$ of the projection of $X$ onto $X_i$; then $f_i \circ \pi_i$ is a morphism from $P$ into $S$ independent of $i$. Let $T$ be a manifold, and let $g_i : T \to X_i$ be morphisms of manifolds such that $f_i \circ g_i$ is a morphism from $T$ into $S$ independent of $i \in I$; then there exists one and only one morphism $h$ from $T$ into $P$ such that $g_i = \pi_i \circ h$ for every $i \in I$.

5.11.4. (*Associativity of the fibred product*) Let $f = (f_i)_{i \in I}$ be a finite family of morphisms of manifolds $f_i : X_i \to S$, and let $(J_\lambda)_{\lambda \in \Lambda}$ be a partition of $I$. Suppose that, for every $\lambda$ in $\Lambda$, the family $f_\lambda = (f_i)_{i \in J_\lambda}$ is transversal, and let $P_\lambda$ denote the fibred product of this family; for every point $x = (x_i)_{i \in J_\lambda}$ of $P_\lambda$, the element $f_i(x_i)$ of $S$ is independent of $i \in J_\lambda$ and will be denoted by $u_\lambda(x)$;

then $u_\lambda$ is a morphism of $P_\lambda$ into $S$. For the family $u = (u_\lambda)$ to be transverse, it is necessary and sufficient that the family $f$ be so. The canonical bijection of $\prod_{\lambda \in \Lambda} \prod_{i \in J_\lambda} X_i$ onto $\prod_{i \in I} X_i$ then yields by restriction an isomorphism of the fibred product $\prod_{\lambda \in \Lambda} \prod_{s} P_\lambda$ onto the fibred product $\prod_{i \in I} \prod_{s} X_i$.

5.11.5. Let $S$ be a variety. A *variety over* $S$ is a variety $X$ endowed with a morphism $\lambda : X \to S$. Let $(X, \lambda)$ be a variety over $S$ and let $f : S' \to S$ be a morphism of varieties such that the pair $(f, \lambda)$ is transverse. We then denote by $f^*(X)$ the variety $S' \times_S X$, endowed with the morphism $f^*(\lambda) : S' \times_S X$ defined by $f^*(\lambda)(s', x) = s'$. One says that $f^*(X)$ is deduced from $X$ by base change from $S$ to $S'$ along $f$. If $\lambda$ is a submersion (resp. an immersion, a subimmersion, an étale morphism), the same is true of $f^*(\lambda)$.

5.11.6. Let $f : X \to Y$ be a morphism of manifolds and let $W$ be a submanifold of $Y$; let $i$ be the canonical injection of $W$ into $Y$. One says that $f$ is *transversal to* $W$ *at a point* $x \in f^{-1}(W)$ if the pair $(f, i)$ is transversal at the point $(x, f(x))$ of $X \times W$. For this, it is necessary and sufficient that the following conditions be satisfied:
(i) the tangent space $T_{f(x)}(Y)$ is the sum of $T_{f(x)}(W)$ and of the image of $T_x(f)$;
(ii) the inverse image $T_x(f)^{-1}(T_{f(x)}(W))$ of the tangent space to $W$ at $f(x)$ admits a topological complement.
One says that $f$ is *transversal to* $W$ if it is transversal to $W$ at every point of $f^{-1}(W)$.
For a morphism $f$ of $X$ into $Y$ to be a submersion, it is sufficient that it be transversal to every point of $Y$, and it is necessary that it be transversal to every submanifold of $Y$. For a finite family of morphisms $f_i : X_i \to S$ to be transversal, it is necessary and sufficient that the morphism $g$ of $\prod_{i \in I} X_i$ into $S^I$ defined by $g((x_i)_{i \in I}) = (f_i(x_i))_{i \in I}$ be transversal to the diagonal of $S^I$.

5.11.7. Suppose that the morphism $f : X \to Y$ is transversal to the submanifold $W$ of $Y$. Then $f^{-1}(W)$ is a submanifold of $X$, and for $x$ in $f^{-1}(W)$ the subspace of $T_x(X)$ tangent to $f^{-1}(W)$ is the inverse image under $T_x(f)$ of the subspace $T_{f(x)}(W)$. By passing to the quotient, the linear mapping $T_x(f)$ defines an isomorphism of topological vector spaces from the transversal space to $f^{-1}(W)$ at $x$ onto the transversal space to $W$ at $y = f(x)$. If $W$ is of codimension $d$ at $y$ in $Y$, the submanifold $f^{-1}(W)$ of $X$ is of codimension $d$ at every point of $f^{-1}(W)$. Finally, the mapping $x \mapsto (x, f(x))$ is an isomorphism of manifolds of $f^{-1}(W)$ onto the fibre product $X \times_Y W$.

5.11.8. Let $Y_1$ and $Y_2$ be two subvarieties of a variety $X$, and let $\iota_j$ be the injection of $Y_j$ into $X$. We say that $Y_1$ and $Y_2$ are transverse if the pair $(\iota_1, \iota_2)$ is transverse; equivalently, it is enough to suppose that, for every point $x$ of $Y_1 \cap Y_2$, the subspaces $T_x(Y_1)$ and $T_x(Y_2)$ of $T_x(X)$ have $T_x(X)$ as their sum, and that their intersection admits a topological complement in $T_x(X)$. Under these conditions, $Y_1 \cap Y_2$ is a subvariety of $X$ and for every $x$ in $Y_1 \cap Y_2$, we have:

$$
T_x(Y_1 \cap Y_2) = T_x(Y_1) \cap T_x(Y_2);
$$

if, moreover, $Y_i$ is of codimension $d_i$ at $x$, then $Y_1 \cap Y_2$ is of codimension $d_1 + d_2$ at $x$.

5.11.9. Let $f$ and $g$ be two morphisms of a variety $X$ into a variety $Y$. If the morphism $(f, g) : X \to Y \times Y$ is transverse to the diagonal of $Y \times Y$, the subset $N$ of $X$ formed by the points $x$ such that $f(x) = g(x)$ is a subvariety of $X$; we call it the *kernel* of the double arrow

$$
f, g : X \twoheadrightarrow Y.
$$

### 5.12. Group varieties

5.12.1. Let $G$ be a group. A variety structure on $G$ is said to be *compatible* with the group structure of $G$ if the mapping $(x, y) \mapsto xy$ of $G \times G$ into $G$ is a morphism. The mapping $x \mapsto x^{-1}$ is then a morphism of $G$ into itself. The set $G$, endowed with its group structure and its variety structure, is called a *group variety* (« of class $C^r$ » if one wishes to be precise), or also a *Lie group*. If $r = \omega$, it is also called an *analytic group*. If $K = \mathbf{R}$ (resp. $\mathbf{C}, \mathbf{Q}_p$), it is also called a *real Lie group* (resp. *complex*, *p-adic*). Every group variety is purely. We call *homomorphism of group varieties* (or simply *homomorphism*) any mapping of one group variety into another which is both a group homomorphism and a *morphism* of varieties.

If $G$ is a group variety, the topological structure underlying the variety structure of $G$ makes it a *metrizable and complete topological group*; it is locally compact if $K$ is locally compact and $G$ finite-dimensional.

5.12.2. *Examples* :
(i) If $V$ is a Banach space, the canonical manifold structure of $V$ is compatible with its structure of a commutative group.
(ii) Let $A$ be a complete normed $K$-algebra, possessing a unit element, and let $A^*$ be the group of invertible elements of $A$. This is an open subspace of $A$ and the manifold structure induced on this open set by the canonical manifold structure of the $K$-vector space $A$ is compatible with the group structure in $A^*$. In particular, let us take for $A$ the algebra

L(E) of continuous endomorphisms of a Banach space E; the group $A^*$ consists of the automorphisms of the topological vector space E; we denote by $\mathrm{GL}(E)$ the group manifold thus resulting. When $A = M_n(K)$, we obtain a group manifold structure on $\mathrm{GL}(n, K)$.

(iii) If $G_1, \ldots, G_n$ are group manifolds, the product group $G = G_1 \times \cdots \times G_n$ is a group manifold, when it is endowed with the product manifold structure of those of the $G_i$.

5.12.3. Let $G$ be a group manifold, let $H$ be a topological group and let $f : H \to G$ be a continuous homomorphism satisfying condition (QR) of No. 5.8.1. The inverse image manifold structure of that of $G$ by $f$ then makes $H$ a group manifold. This applies in particular when $H$ is a *subgroup of $G$ which is a submanifold* (resp. quasi-submanifold); such a subgroup is called a *submanifold* (resp. quasi-submanifold) *of the group* $G$; it is necessarily *closed* in $G$.

If $H_i (i = 1, \ldots, n)$ is a submanifold of the group $G_i$, then $H_1 \times \cdots \times H_n$ is a submanifold of the group $G_1 \times \cdots \times G_n$.

5.12.4. Let $G$ be a group manifold and let $H$ be a submanifold of the group $G$. The equivalence relation $x^{-1} y \in H$ is regular, which makes it possible to endow the space $G/H$ of the left cosets $xH$ with a manifold structure called the *quotient* of that of $G$. The canonical mapping $(g, x) \mapsto g \cdot x$ of $G \times (G/H)$ into $G/H$ is a morphism. There are analogous results for the homogeneous space $H\backslash G$ of the right cosets $Hx$. If $H$ is normal, the manifold structure of $G/H$ is compatible with its group structure.

5.12.5. Let $G$ be a group manifold and let $X$ be a manifold. A *left operation law of the group $G$ on the manifold $X$* is any morphism $(s, x) \mapsto sx$ of $G \times X$ into $X$ such that

$$
s(tx) = (st)x \quad \text{if} \quad s, t \in G, x \in X \\
ex = x \quad \text{if} \quad x \in X \ (\text{$ e $ being the identity element of } G).
$$

The group manifold $G$ is also said to *operate on the left* on $X$; right operation laws are defined analogously.

Let $x \in X$ and let $G_x$ be its stabilizer in $G$. Suppose that the mapping $g \mapsto g \cdot x$ is a *subimmersion* (an assumption automatically satisfied if the characteristic of $K$ is 0 and $X$ is finite-dimensional). Then $G_x$ is a subgroup submanifold of $G$ and the mapping of $G/G_x$ into $X$ obtained by passing to the quotient from $g \mapsto g \cdot x$ is an immersion. If, moreover, the orbit $G \cdot x$ of $x$ is locally closed and if the topology of $G$ has a countable basis, $G \cdot x$ is a submanifold of $X$ and the mapping $G/G_x \to G \cdot x$ is an isomorphism of manifolds.

### 5.13. Weakening of structure

Throughout this No., the letters $r, s, r', s'$ denote either integers $\geqslant 1$, or one of the symbols $\infty$ and $\omega$. We suppose that $K = \mathbf{R}$.

5.13.1. Let $r \leqslant s$, and let $X$ be a manifold of class $C^s$. There exists on the topological space $X$ a structure of a manifold of class $C^r$ and only one such that every chart of $X$ for the given structure is a chart of $X$ for this new structure. Let $X_r$ be the manifold of class $C^r$ thus defined. We say that it is obtained from $X$ by weakening the manifold structure of $X$, or also that its manifold structure underlies that of $X$. The notion of weakening is transitive: if $r' \leqslant r$, we have $X_{r'} = (X_r)_{r'}$; it commutes with products: if $Y$ is of class $C^s$, we have $(X \times Y)_r = X_r \times Y_r$; there is an analogous result for $X \times_s Y$ under the hypotheses of No. 5.11.2.

Let $a \in X$ and let $c$ be a chart of $X$ at $a$; it is also a chart of $X_r$ at $a$. From (5.5.1) we deduce isomorphisms

$$
\theta_c : E \to T_a(X), \quad \theta'_c : E \to T_a(X_r),
$$

whence an isomorphism $\theta'_c \circ \theta_c^{-1} : T_a(X) \to T_a(X_r)$. This isomorphism is independent of the choice of $c$; it permits us to identify the tangent spaces to $X$ and to $X_r$ at $a$.

5.13.2. Let $X$ (resp. $X'$) be a manifold of class $C^s$ (resp. $C^{s'}$), and let $r$ be such that $r \leqslant \inf(s, s')$. A mapping $f : X \to X'$ is said to be of class $C^r$ if it is a morphism from $X_r$ into $X'_r$; such a mapping is of class $C^{r'}$ for every $r' \leqslant r$. Moreover, the tangent linear mapping to $f : X_r \to X'_r$ at a point $a \in X$ coincides with the tangent linear mapping to $f$ considered as a morphism from $X_r$ into $X'_r$.

Most often, the same symbol will be used to denote the manifolds $X$ and $X_r$; thus, if $X$ is of class $C^s$, the expression "a submanifold of $X$ of class $C^r$" ($r \leqslant s$) means "a submanifold of $X_r$".

### 5.14. Restriction of the base field

In this number, two complete non-discrete valued commutative fields $K$ and $L$ are given, together with an isomorphism $\sigma$ of the valued field $K$ onto a subfield of $L$. If $E$ is a Banach space over $L$, $\sigma_*(E)$ denotes the vector space over $K$ obtained by restriction of scalars (cf. Alg., chap. II, 3rd ed., § 8); the topology given on $E$ is compatible with the structure of $K$-vector space, and $\sigma_*(E)$ is a Banach space over $K$.

5.14.1. Let $X$ be an analytic manifold over $L$ and let $c = (U, \varphi, E)$ be a chart of $X$. The mapping $\varphi$ is a bijection of $U$ onto an open subset of $\sigma_*(E)$ and the triple $c_\sigma = (U, \varphi, \sigma_*(E))$ is a chart of $X$. There exists on $X$ one and only one structure of analytic manifold over K for which $c_\sigma$ is a chart for every chart $c$ of the L-analytic manifold X. The analytic manifold over K thus obtained is denoted by $X_\sigma$, and it is said that $X_\sigma$ is obtained from X by restriction of scalars (from L to K by means of $\sigma$). The underlying topological space of $X_\sigma$ is the same as that underlying X.

5.14.2. Examples:
(a) Take $K = \mathbf{R},\ L = \mathbf{C},\ \sigma$ to be the canonical injection of R into C. Thus every complex analytic manifold is canonically endowed with a structure of a real analytic manifold; this real analytic structure itself defines differential structures of class $C^r$ for every r.
(b) Take $K = \mathbf{C},\ L = \mathbf{C},\ \sigma$ to be the conjugation $x \mapsto \bar{x}$. Thus to every complex analytic manifold X one associates a complex analytic manifold $\overline{X}$, called the conjugate of X. If $f$ is a complex-valued function, defined on an open set U of X, $f$ is analytic for the structure of $\overline{X}$ if and only if the conjugate function $\bar{f}$ is analytic for the structure of X. The manifolds X and $\overline{X}$ define by restriction of scalars the same real analytic manifold.

5.14.3. Let X be an analytic manifold over K, and Y an analytic manifold over L. A mapping $f : X \to Y$ is said to be $\sigma$-analytic if it is a morphism of X into $Y_\sigma$. If $K \subset L,\ \sigma$ is the injection of K into L, and X is an analytic manifold over L, a K-analytic mapping is called a $\sigma$-analytic mapping of $X_\sigma$ into Y.

5.14.4. Let V be an L-Banach space. We have $V_\sigma = \sigma_*(V)$: the canonical structure of an analytic manifold over K on $\sigma_*(V)$ is obtained by restriction of scalars from the canonical structure of an analytic manifold over L on V.

5.14.5. Let X be an analytic manifold over L, and let $a \in X$. Let c be a chart of X at a; then $c_\sigma$ is a chart of $X_\sigma$ at a and we deduce from it the isomorphisms
$$
\theta_c : E \to T_a(X), \quad \theta_{c_\sigma} : \sigma_*(E) \to T_a(X_\sigma)
$$
whence an isomorphism $\theta_{c_\sigma} \circ \sigma_*(\theta_c)^{-1}$ of $\sigma_*(T_a(X))$ onto $T_a(X_\sigma)$; this isomorphism does not depend on the choice of c; it allows us to identify $T_a(X_\sigma)$ with $\sigma_*(T_a(X))$ and even with $T_a(X)$ by abuse of notation.
If $f$ is an analytic mapping over L of X into a manifold Y, the tangent linear mapping to $f$ at a ($f$ being regarded as a morphism of $X_\sigma$ into $Y_\sigma$) is equal to $\sigma_*(T_a(f))$.

5.14.6. Let X and Y be two analytic manifolds over L, and let $f : X_\sigma \to Y$ be a $\sigma$-analytic mapping. Suppose that the characteristic of K is 0. Then, for $f$ to be analytic over L, it is necessary and sufficient that, for every $a \in X$, the mapping $T_a(f)$ be L-linear.

When $K = \mathbf{R},\ L = \mathbf{C}$ (case (a) of No. 5.14.2), we have a more precise result: if $X$ and $Y$ are finite-dimensional and if $f : X \to Y$ is a mapping of class $C^1$ whose tangent mapping at every point of $x$ is $\mathbf{C}$-linear, then $f$ is complex analytic.

5.14.7. Let $X$ be a *complex analytic* manifold and $g$ a mapping of $X$ into itself satisfying the conditions:
(i) We have $g \circ g = \mathrm{Id}_X$.
(ii) The mapping $g$ is an isomorphism of the analytic manifold $X$ onto the conjugate manifold $\overline{X}$ (5.14.2).

The set $X_0$ of points $x$ of $X$ such that $g(x) = x$ is a closed analytic submanifold of the underlying real analytic manifold of $X$. For $x \in X_0$, one has $T_x(X) = T_x(X_0) \oplus i T_x(X_0)$.

Let $U$ be a *connected* open set of $X$ and let $f$ and $g$ be two complex analytic mappings of $U$ into a separated locally convex complex space or into a separated complex analytic manifold. If $f$ and $g$ coincide on a nonempty subset of $U \cap X_0$, open in $X_0$, then $f = g$.

Assume $X_0$ paracompact. If $f$ is a real analytic mapping of $X_0$ into a separated locally convex space or into a separated complex analytic manifold, there exists an open neighbourhood $U$ of $X_0$ in $X$ and a complex analytic mapping of $U$ into the value space of $f$, extending $f$. Two such extensions coincide on a neighbourhood of $X_0$ in $X$.

Assume $X$ finite-dimensional. For every point $a \in X_0$, there exists a system of (complex) coordinates $\zeta^1, \ldots, \zeta^n$ in an open neighbourhood $U$ of $a$, such that $\zeta^i \circ g = \bar{\zeta}^i$ for $1 \leq i \leq n$; the restriction $\zeta^i$ of $\zeta^i$ to $U \cap X_0$ is then real-valued and $(\xi^1, \ldots, \xi^n)$ is a system of coordinates at $a$ of the real analytic manifold $X_0$.

5.14.8. For every real analytic manifold $Y$, *paracompact*, there exists a pair $(X, g)$ consisting of a complex analytic manifold $X$ and a mapping $g$ of $X$ into itself satisfying conditions (i) and (ii) of 5.14.7, and an isomorphism $f$ of $Y$ onto $X_0$. One says that $X$ (equipped with $f$ and $g$) is a *complexification* of $Y$.
