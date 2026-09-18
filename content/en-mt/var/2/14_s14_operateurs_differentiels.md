---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 14
section_title: Opérateurs différentiels
lang: en
source: var-fr
pdf_pages: 0162-0173
extraction: ocr
subsections:
    - "no": 1
      title: Opérateurs différentiels
      page: 0
      pdf_page: 162
    - "no": 2
      title: Symboles
      page: 0
      pdf_page: 166
    - "no": 3
      title: Transposition
      page: 0
      pdf_page: 169
    - "no": 4
      title: Exemples
      page: 0
      pdf_page: 172
statements: 2
exercises: 0
content_sha256: 5c066a3a7c489633b6dc0c6772b855625588fe75961eda95b9df4cb8b5ca50c8
translated_from: content/fr/var/2/14_s14_operateurs_differentiels.md
source_lang: fr
translation_method: machine
source_content_sha256: 1392eb42732e48e986a4b120baebb41eb1413b70e59d35e31a21984b15deb2b5
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-en-mt-ae4be300
glossary_version: 34
glossary_terms_sha256: 236d60ab96e4f7ac8bfa6874cd6d8fb56e0d2f60f979943591f4552c30402f3a
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 14. Differential Operators

In this paragraph, X denotes a locally finite-dimensional manifold of class $C^r$, where $r \in \mathbf{N}_k$; E and F denote two vector bundles of finite rank of class $C^r$ and with basis X.

All manifolds and vector bundles considered are assumed to be locally finite-dimensional.

### 14.1. Differential Operators

### 14.1.1. Let k be an integer such that $0 \leq k \leq r$, and let $P^k(E)$ be the bundle of jets of sections of order k of E (12.6.1). Put

$$
D^k(E,F)=\mathscr{L}(P^k(E);F).
$$

This is a vector bundle with basis X and of class $C^{r-k}$. A section of this bundle over an open set U of X is identified with a mapping

$$
D:P^k(E)|U\longrightarrow F|U
$$

which commutes with the projection onto U and is linear on each fibre; such a section is called a differential operator on U, of type $E \rightarrow F$, and of order $\leq k$. Let $h \in \mathbf{N}_k \cup \{0\}$, with $0 \leq h \leq r-k$. We denote by $\mathscr{D}^{k,h}_U(E,F)$ the set of differential operators on U, of type $E \rightarrow F$ and of order $\leq k$, which are of class $C^h$ (as sections of $D^k(E,F)$, or as morphisms of $P^k(E)|U$ into $F|U$, this amounts to the same thing). If $M=D^k(E,F)$, we have $\mathscr{D}^{k,h}_U(E,F)=\mathscr{F}^h_M(U)$; this is a module over $\mathscr{C}^h(U)$, cf. 7.4.1.

If $0 \leq k' \leq k$, the morphism $r^{k,k'}:P^k(E)\longrightarrow P^{k'}(E)$ (cf. 12.6.6) defines an injection of $D^{k'}(E,F)$ into $D^k(E,F)$; every differential operator of order $\leq k'$ is thus identified with a differential operator of order $\leq k$. A differential operator of order $\leq k$ which is not of order $\leq k-1$ is sometimes said to be of order k. If $h \in \mathbf{N}_k \cup \{0\}$ and $h \leq r-k$, and if U is an open set of X, we have:

$$
0 \subset \mathscr{D}^{0,h}_U(E,F) \subset \mathscr{D}^{1,h}_U(E,F) \subset \cdots \subset \mathscr{D}^{k,h}_U(E,F).
$$

If $r=\infty$ or $\omega$, we denote by $\mathscr{D}^{\omega,h}_U(E,F)$ the union of the $\mathscr{D}^{k,h}_U(E,F)$ for $k \geq 0$; an element of this union is called a differential operator on U of bounded order (of type $E \rightarrow F$, of class $C^h$) or sometimes simply a differential operator on U.

### 14.1.2 (« Operators of order zero »). We have $P^0(E)=E$ (12.5.1) and $D^0(E,F)=\mathscr{L}(E;F)$. If U is open in X, and if $h \in \mathbf{N}_k \cup \{0\}$ and $h \leq r$, an element of $\mathscr{D}^{0,h}_U(E,F)$ is a morphism of class $C^h$ of $E|U$ into $F|U$.

14.1.3 (“Weakening of structure”). Suppose that $K = \mathbf{R}$, and let $r' \in \mathbf{N}_\mathbf{R}$ with $r' \leq r$. Let $X', E'$ and $F'$ be the manifold and the vector bundles of class $C^{r'}$ obtained by weakening of structure from $X, E,$ and $F$ respectively. Let $k$ be an integer such that $0 \leq k \leq r'$. Then $P^k(E')$ is the bundle of class $C^{r'-k}$ deduced from $P^k(E)$ by weakening of structure, and there is an analogous result for $D^k(E', F')$. In particular, if $U$ is open in $X$, and if $0 \leq h \leq r - k'$, one has $\mathscr{D}_U^{k',h}(E', F') = \mathscr{D}_U^{k,h}(E, F)$.

14.1.4. Let $D$ be a differential operator on $X$, of type $E \to F$, of order $\leq k$ (where $0 \leq k \leq r$). Let $U$ be an open set in $X$, and let $s$ be a section, of class $C^m$, of $E$ over $U$, with $m \in \mathbf{N}_K \cup \{0\}$ and $k \leq m \leq r$. Then $j^k(s)$ is a section of class $C^{m-k}$ of $P^k(E)$ over $U$ (12.6.1); its image under $D$ is denoted by $D_U(s)$, or $D(s)$. It is a section of $F|U$. Suppose that $D$ is of class $C^h$, where $h = m - k$. Then $D_U(s)$ is of class $C^h$, and the mappings
$$
D_U : \mathscr{S}_E^m(U) \to \mathscr{S}_F^h(U)
$$
thus obtained enjoy the following properties:

(1) $D_U$ is $K$-linear.
(2) For every $s \in \mathscr{S}_E^m(U)$ and every open set $V$ of $U$, one has $D_V(s|V) = D_U(s)|V$.
(3) For every $s \in \mathscr{S}_E^m(U)$ and every $x \in U$ such that $j_x^k(s) = 0$, one has $D_U(s)(x) = 0$.
(3') For every coordinate system $\xi = (\xi^1, \ldots, \xi^n)$ in $U$ and every frame $s = (s_1, \ldots, s_d)$ of $E$ over $U$ (7.4.4), there exist sections $n_{i,\alpha} (1 \leq i \leq d, \alpha \in \mathbf{N}^n, |\alpha| \leq k)$ of $F$ over $U$, of class $C^h$ and such that, for every family $(f_i)_{1 \leq i \leq d}$ of elements of $\mathscr{C}^m(U)$, one has
$$
D_U \left( \sum_{1 \leq i \leq d} f_i . s_i \right) = \sum_{1 \leq i \leq d, |\alpha| \leq k} \Delta_\xi^\alpha(f_i) . n_{i,\alpha}, \quad \text{(cf. 13.2.6).}
$$
(4) For every function $f \in \mathscr{C}^m(U)$ and every mapping $\theta$ of $\mathscr{S}_U^m(E)$ into $\mathscr{S}_U^h(F)$, let $\operatorname{ad}(f)\theta$ denote the mapping
$$
s \mapsto f . \theta(s) - \theta(f.s)
$$
of $\mathscr{S}_U^m(E)$ into $\mathscr{S}_U^h(F)$. Then, for every function $f \in \mathscr{C}^m(U)$, there exists a differential operator $L$ on $U$, of type $E \to F$, of order $\leq k - 1$ and of class $C^h$ such that
$$
(\operatorname{ad}(f)D_U)(s) = L_U(s) \quad \text{for every } s \in \mathscr{S}_U^m(E).
$$
(5) One has
$$
\operatorname{ad}(f_0) \ldots \operatorname{ad}(f_k) D_U = 0 \quad \text{for arbitrary } f_0, \ldots, f_k \text{ in } \mathscr{C}^m(U).
$$
If one sets $I = \{0, \ldots, k\}$ and $f_H = \prod_{i \in H} f_i$ for every subset $H$ of $I$, the preceding relation is equivalent to:
$$
\sum_{H \subset I} (-1)^{\operatorname{Card}(H)} f_H . D_U(f_{I-H}.s) = 0
$$
for arbitrary $f_0, \ldots, f_k$ in $\mathscr{C}^m(U)$ and $s$ in $\mathscr{S}_E^m(U)$.

14.1.5 ("Characterization of differential operators"). Let $k, m$ and $h = m - k$ be as in 14.1.4. For every open set $U$ of $X$, let $D_U$ be a mapping of $\mathscr{S}_E^m(U)$ into $\mathscr{S}_F^h(U)$. Suppose that conditions 1, 2, 3 (resp. 1, 2, 3') of 14.1.4 are satisfied for every open subset U of X. Then there exists an element D of $\mathscr{D}_X^{k,h}(E, F)$, and only one, such that the $D_U$ are the corresponding mappings.$^{(1)}$ In what follows, D is identified with the family of the $D_U$.

When $m = \infty$ or $\omega$, we have $h = m$ and one may replace conditions (3) and (3') by either of conditions (4) and (5).

14.1.6 (“Scalar differential operators”). Suppose that E and F are equal to the trivial vector bundle $K_X$. A differential operator of type $E \to F$ is then called a *scalar* differential operator or simply a differential operator; if it is of order $\leq k$, it is a section of the vector bundle $\mathscr{L}(P^k(X); K_X) = P^k(X)^*$, *dual* of the vector bundle $P^k(X)$; using the isomorphism
$$
i^{-1} : P^k(X)^* \to T^{(k)}(X) \quad (\text{cf. } 13.2.5),
$$
one sees that a scalar differential operator of order $\leq k$ is identified with a *section* of the vector bundle $T^{(k)}(X)$, i.e. with a *field of point distributions of order* $\leq k$.

Take in particular for X an open subset of $K^n$, where n is an integer $\geq 0$. The fields of point distributions
$$
\Delta^\alpha : x \mapsto \Delta_x^\alpha \quad (\text{cf. } 13.2.6)
$$
are scalar differential operators of class $C^\omega$. For every $h \in N_K$, the $\Delta^\alpha$ for $(|\alpha| \leq k)$ form a *basis* of the $C^h(X)$-module $\mathscr{D}_X^{k,h}(K_X, K_X)$.

14.1.7 (“Complex differential operators on a real manifold”). Suppose $K = \mathbf{R}$ and that the vector bundles E and F are endowed with *complex structures* (8.8.1); let k be an integer such that $0 \leq k \leq r$. The vector bundle $P^k(E)$ is then endowed with a complex structure (12.6.3); the vector bundle $\mathscr{L}_c(P^k(E); F)$ (7.8.5) of *complex* linear mappings from $P^k(E)$ into F is a vector subbundle of $\mathscr{L}(P^k(E); F) = D^k(E, F)$; we denote it by $D_c^k(E, F)$. A section of $D_c^k(E, F)$ is called a *complex* differential operator, of type $E \to F$ and of order $\leq k$. If $h \in N_K$ and $h \leq r - k$, and if U is an open subset of X, we denote likewise by $\mathscr{D}_U^{k,h}(E, F)_c$ the space of sections of class $C^h$ of $D_c^k(E, F)$ over U; it is a C-vector space. The other definitions and results of this paragraph extend analogously to complex differential operators; we leave their formulation to the reader.

14.1.8 (« Composition »). Let G be a vector bundle of class $C^r$ and with base X. Let $k'$ and $k''$ be positive integers with sum $k \leq r$, and let $D'$ (resp. $D''$) be a differential operator on X, of type $E \to F$ (resp. of type $F \to G$), of order $\leq k'$ (resp. $\leq k''$). Suppose $D' : P^{k'}(E) \to F$ is of class $C^{h'}$, with $h' \in N_K \cup \{0\}$ and $k'' \leq h' \leq r - k'$; the mapping
$$
D'_* = P^{k''}(D') : P^{k''}(P^{k'}(E)) \to P^{k''}(F)
$$
is of class $C^{h'-k''}$ (12.6.3). Let $\beta$ be the canonical homomorphism from $P^{k}(E)$ into $P^{k''}(P^{k'}(E))$, cf. 12.6.5. By composing the mappings
$$
P^k(E) \xrightarrow{\beta} P^{k''}(P^{k'}(E)) \xrightarrow{D'_*} P^{k''}(F) \xrightarrow{D''} G,
$$
one obtains a differential operator of type $E \to G$ and of order $\leq k$. This operator is called the *composite* of $D''$ and $D'$; it is denoted by $D'' \circ D'$.

$^1$ It is in fact sufficient that condition (3') be satisfied for a family $(\xi_\lambda)$ of systems of coordinates and a family of frames $(s_\lambda)$ whose domains cover X.

If U is an open subset of X, and if s ∈ $\mathscr{S}_E^{k}(U)$, one has
$$
(D'' \circ D')(s) = D''(D'(s))
$$
(where the two members are sections of G over U); this justifies the terminology and notation adopted.

Suppose now that D'' is of class $C^{h''}$, with $h'' \in \mathbf{N}_K \cup \{0\}$ and $h'' \leq r - k''$. Then $D'' \circ D'$ is of class $C^h$, with $h = \inf(h' - k'', h'')$.

Suppose that one has $E = F = G$, and that $k' \leq h''$, in which case $D' \circ D''$ is defined. Then $D' \circ D'' - D'' \circ D'$ is a differential operator of type $E \to E$ and of order $\leq k - 1$; it is denoted by $[D', D'']$.

14.1.9 (« Associativity »). With the notation and hypotheses of 14.1.8, let H be a vector bundle of class $C^r$ and with base X, and let $D'''$ be a differential operator on X, of type $G \to H$ and of order $\leq k'''$, with $k' + k'' + k''' \leq r$. Suppose that $D'$ is of class $C^{h'}$, with $h' \in \mathbf{N}_K \cup \{0\}$ and $k'' + k''' \leq h' \leq r - k'$ and that $D''$ is of class $C^{h''}$, with $h'' \in \mathbf{N}_K \cup \{0\}$ and $k''' \leq h'' \leq r - k''$. Then the composites
$$
D''' \circ (D'' \circ D') \quad \text{and} \quad (D''' \circ D'') \circ D'
$$
are defined and are equal.

14.1.10. Examples

a) Let U be an open subset of X, let $D \in \mathscr{D}_U^{k,h}(E, F)$ with $h \in \mathbf{N}_K \cup \{0\}$ and $h \leq r - k$, and let $f \in \mathscr{C}^{h+k}(U)$ (resp. $f \in \mathscr{C}^h(U)$). Multiplication by f in E (resp. F) is a differential operator on U of order $\leq 0$, and of type $E \to E$ (resp. $F \to F$), cf. 14.1.2. The composites $D \circ f$ and $f \circ D$ are defined and belong to $\mathscr{D}_U^{k,h}(E; F)$; we put
$$
\operatorname{ad}(f)D = f \circ D - D \circ f \in \mathscr{D}_U^{k-1,h}(E, F),
$$
cf. 14.1.4, (4). Thus $\mathscr{D}_U^{k,h}(E, F)$ is endowed with a $\mathscr{C}^{h+k}(U)$-module structure on the right (resp. a $\mathscr{C}^h(U)$-module structure on the left). The left module structure coincides with that of 14.1.1.

b) Suppose $r = \infty$ or $r = \omega$. The differential operators of type $E \to E$ and of class $C^r$ form an associative K-algebra with unit element.

c) Take for X an open subset of $K^n$. The scalar differential operators $\Delta^\alpha$ (14.1.6) satisfy the formulas
$$
\Delta^\alpha \circ \Delta^\beta = ((\alpha, \beta)) \Delta^{\alpha+\beta}.
$$
They commute with one another. Denote by $D_i$ the operator $\Delta^{\varepsilon_i}$ (« i-th partial derivative »). If K is of characteristic 0, we have
$$
\Delta^\alpha = \frac{1}{\alpha!} D_1^{\alpha_1} \ldots D_n^{\alpha_n}.
$$
If K is of characteristic $p \neq 0$, we have $D_i^p = 0$ for every $i$.

14.1.11 (« Multidifferential operators »). Let $E_1, \ldots, E_n$ be vector bundles of class $C^r$ and with base X, and let $k, k_1, \ldots, k_n$ be integers belonging to $[0, r]$. Put
$$
L(k_1, \ldots, k_n) = \mathscr{L}(P^{k_1}(E_1) \otimes \cdots \otimes P^{k_n}(E_n); F).
$$

If $k_i \leq k$ for all $i$, the projections $r^{k_i, k_i} : P^k(E_i) \to P^{k_i}(E_i)$ make it possible to identify the bundle $L(k_1, \ldots, k_n)$ with a sub-bundle of the bundle $L(k) = L(k, \ldots, k)$. There exists a smallest sub-bundle $M(k)$ of $L(k)$ containing all the sub-bundles $L(k_1, \ldots, k_n)$, for $k_1 + \cdots + k_n = k$. A section $H$ of $M(k)$ is called an $n$-differential (or multidifferential) operator of type $(E_1, \ldots, E_n) \to F$ and of order $\leq k$. If $s_i$ ($1 \leq i \leq n$) is a section of class $C^m$ ($m \in \mathbf{N}_K, m \geq k$) of $E_i$ over an open set $U$ of $X$, one defines $H_U(s_1, \ldots, s_n) = H(s_1, \ldots, s_n)$ as the image under $H$ of the section $j^k(s_1) \otimes \cdots \otimes j^k(s_n)$ of the bundle
$$
P^k(E_1) \otimes \cdots \otimes P^k(E_n).
$$
It is a section of $F|U$. If $H$ is of class $C^h$, this section is of class $C^p$ with $p = \inf(m - k, h)$.

When $E_1, \ldots, E_n$ and $F$ are equal to $K_X$, one says that $H$ is a scalar $n$-differential (or multidifferential) operator.

#### Example {#var-2-s14-n1-exa-1 .statement}

Let $J$ be a finite set, and $X$ an open set of $K^J$. Let $H$ be a scalar $n$-differential operator of order $\leq k$ on $X$. There exists a unique family of scalar functions
$$
c(\alpha(1), \ldots, \alpha(n))_{(\alpha(1), \ldots, \alpha(n)) \in \mathbf{N}^J}, \quad \sum_{i=1}^n |\alpha(i)| \leq k
$$
on $X$ such that
$$
H_X(f_1, \ldots, f_n) = \sum_{\alpha(1), \ldots, \alpha(n)} c(\alpha(1), \ldots, \alpha(n)) \Delta^{\alpha(1)}(f_1) \ldots \Delta^{\alpha(n)}(f_n)
$$
for every family $(f_1, \ldots, f_n)$ of functions of class $C^k$ on $X$. In order that $H$ be of class $C^h$, it is necessary and sufficient that the functions $c(\alpha(1), \ldots, \alpha(n))$ be of class $C^h$.

### 14.2. Symbols

14.2.1. Let $k$ be a positive integer $\leq r$. Consider the exact sequence
$$
0 \to P_k(T(X); E) \xrightarrow{i'} P^k(E) \xrightarrow{j'} P^{k-1}(E) \to 0
$$
of No. 12.6.8, where $j = r^{k, k-1}$. Applying the vector bundle functor $M \mapsto \mathscr{L}(M; F)$ to this sequence, we obtain the exact sequence
$$
0 \to \mathscr{L}(P^{k-1}(E); F) \xrightarrow{j''} \mathscr{L}(P^k(E); F) \xrightarrow{\sigma_k} \mathscr{L}(P_k(T(X); E); F) \to 0
$$
which can be written:
$$
0 \to D^{k-1}(E, F) \xrightarrow{j''} D^k(E, F) \xrightarrow{\sigma_k} S^k(E, F) \to 0
$$
by putting
$$
S^k(E, F) = \mathscr{L}(P_k(T(X); E); F).
$$
The homomorphism $j' = \mathscr{L}(j; \mathrm{Id}_F)$ is the canonical inclusion of $D^{k-1}(E, F)$ in $D^k(E, F)$; the homomorphism $\sigma_k$ is, by definition, equal to $\mathscr{L}(i; \mathrm{Id}_F)$. If $D$ is a differential operator of type $E \to F$ and of order $\leq k$, its image under $\sigma_k$ is a section $\sigma_k(D)$ of $S^k(E, F)$ which is called the $k$-symbol (or simply the symbol) of $D$; we have $\sigma_k(D) = 0$ if and only if $D$ is of order $\leq k-1$. If $D$ is of class $C^h$, the same is true of its symbol.

14.2.2 (« Identifications of the symbol bundle »). The bundle $S^k(E, F) = \mathscr{L}(P_k(T(X); E); F)$ can be written in various ways. First, if $x \in X$, an element of $P_k(T_x(X); E_x)$ is identified (13.1.2) with an element of $\mathscr{L}(TS^k(T_x(X)); E_x)$. We thus obtain identifications of vector bundles

$$
P_k(T(X); E) = \mathscr{L}(TS^k(T(X)); E) = (TS^k(T(X)))* \otimes E
$$

and, applying the vector bundle functor $M \mapsto \mathscr{L}(M; F) = M^* \otimes F$, we obtain:

$$
S^k(E, F) = TS^k(T(X)) \otimes E^* \otimes F = TS^k(T(X)) \otimes \mathscr{L}(E; F).
$$

The preceding expression can be transformed further. If $M$ and $N$ are two vector bundles, let $\mathrm{Sym}^k(M; N)$ denote the subbundle of $\mathscr{L}(M, \ldots, M; N)$ formed by symmetric $k$-linear mappings. We have a canonical isomorphism

$$
\mathrm{Sym}^k(M; N) \to \mathrm{Sym}^k(M; K_X) \otimes N;
$$

on the other hand, the duality between $\otimes^k M$ and $\otimes^k M^*$ identifies $\mathrm{Sym}^k(M; K_X)$ with $TS^k(M^*)$. We thus obtain an identification

$$
\mathrm{Sym}^k(M; N) = TS^k(M^*) \otimes N.
$$

Applying this formula to $M = T(X)^*$ and $N = \mathscr{L}(E; F)$, we have:

$$
S^k(E, F) = TS^k(T(X)) \otimes \mathscr{L}(E; F) = \mathrm{Sym}^k(T(X)^*; \mathscr{L}(E; F)).
$$

Suppose $K$ is of characteristic 0 or $> k$. If $u$ is a symmetric $k$-linear mapping, let $\tilde{u}$ denote the polynomial mapping

$$
x \mapsto \frac{1}{k!} u(x, \ldots, x)
$$

corresponding to it. The mapping $u \mapsto \tilde{u}$ defines an isomorphism

$$
S^k(E, F) = \mathrm{Sym}^k(T(X)^*, \mathscr{L}(E; F)) \to P_k(T(X)^*; \mathscr{L}(E; F)).
$$

Thus, every element $\sigma$ of $S^k(E, F)_x$, with $x \in X$, may be identified with a homogeneous polynomial mapping $\tilde{\sigma}$ of degree $k$ from $T_x(X)^*$ into $\mathscr{L}(E_x; F_x)$.

14.2.3 (“Calculation of the symbol of a differential operator”). Let $x \in X$ and let $D$ be a differential operator of type $E \to F$, of order $\leq k$, defined in an open neighbourhood of $x$ and of class $C^{r-k}$. We shall make explicit the value $\sigma_k(D)(x)$ of the symbol of $D$ at $x$. Consider it as an element of $\mathrm{Sym}^k(T_x(X)^*; \mathscr{L}(E_x; F_x))$ (cf. 14.2.2). Let $\omega_1, \ldots, \omega_k$ be covectors at $x$ and choose functions $f_1, \ldots, f_k$ of class $C^r$ in an open neighbourhood $U$ of $x$ such that $d_x f_i = \omega_i$ for $i = 1, \ldots, k$. Put

$$
D' = (-1)^k \mathrm{ad}\,(f_k) \ldots \mathrm{ad}(f_1)D \quad (\text{cf. } 14.1.10, a).
$$

The operator $D'$ is of order $\leq 0$; it is a section of $\mathscr{L}(E; F)|U$. The value of $D'$ at $x$ is an element $\lambda(\omega_1, \ldots, \omega_k)$ of $\mathscr{L}(E_x; F_x)$ which depends only on $(\omega_1, \ldots, \omega_k)$. The resulting mapping $\lambda$ is symmetric. *It is equal to the symbol $\sigma_k(D)(x)$ of $D$ at $x$*.

Suppose that $K = \mathbf{R}$ or $\mathbf{C}$, and let us make explicit $\sigma_k(D)(x)$ considered as a homogeneous polynomial mapping of degree $k$ from $T_x(X)^*$ into $\mathscr{L}(E_x; F_x)$ (cf. 14.2.2). Let $\omega \in T_x(X)^*$ and $v \in E_x$; choose a function $f$ of class $C^r$ in an open neighbourhood U of x such that $d_x f = \omega$, and a section s of class $C^r$ of E in U such that $s(x) = v$. There exists a family $(\varphi_0, \varphi_1, \ldots, \varphi_k)$ of sections of F in U, and only one, such that
$$
e^{-tf} D(e^{tf}s) = \sum_{j=0}^k t^j \varphi_j \quad \text{for all } t \in K.
$$
Then $\varphi_k(x)$ does not depend on the choice of f and s such that $d_x f = \omega, v(x) = s$; the mapping $v \mapsto \varphi_k(x)$ is an element $\lambda(\omega)$ of $\mathscr{L}(E_x; F_x)$, and $\lambda$ is a homogeneous polynomial mapping of degree k from $T_x(X)^*$ into $\mathscr{L}(E_x; F_x)$. *This mapping is equal to the symbol $\sigma_k(D)(x)$ of D at x.*

14.2.4 ("The scalar case"). Take $E = F = K_X$, in which case one identifies $D^k(E, F)$ with the bundle $T^{(k)}(X)$ of point distributions of order $\leq k$, cf. 14.1.6. One has
$$
S^k(E, F) = TS^k(T(X))
$$
and the symbol
$$
\sigma_k : T^{(k)}(X) \to TS^k(T(X))
$$
is none other than the composite
$$
T^{(k)}(X) \to T^{(k)}(X)/T^{(k-1)}(X) \xrightarrow{i_k} TS^k(T(X)),
$$
where $i_k$ is the isomorphism defined in 13.3.2.

Take for example X to be an open subset of $K^n$, and let $\{e_1, \ldots, e_n\}$ be the canonical basis of $K^n$ (identified with the tangent spaces $T_x(X)$). If $\alpha \in \mathbf{N}^n$ is such that $|\alpha| \leq k$, the symbol of the operator $\Delta^\alpha$ is given by the formulas (cf. 13.3.3):
$$
\begin{aligned}
\sigma_k(\Delta^\alpha)(x) &= 0 & \text{if } |\alpha| < k \\
\sigma_k(\Delta^\alpha)(x) &= \gamma_{\alpha_1}(e_1) \cdots \gamma_{\alpha_n}(e_n) & \text{if } |\alpha| = k,
\end{aligned}
$$
the product of the $\gamma_{\alpha_i}(e_i)$ being the *symmetric product*, cf. 13.2.6 and 13.3.3.

14.2.5 ("Symbol of a composite"). The notations and hypotheses are those of 14.1.8. The composition of linear mappings defines a pairing
$$
\mathscr{L}(F; G) \times \mathscr{L}(E; F) \to \mathscr{L}(E; G).
$$
On the other hand, the operation of *symmetric product* defines a pairing
$$
TS^{k''}(T(X)) \times TS^{k'}(T(X)) \to TS^k(T(X)).
$$
Since one has
$$
\begin{aligned}
S^{k''}(F, G) &= TS^{k''}(T(X)) \otimes \mathscr{L}(F; G) \\
S^{k'}(E, F) &= TS^{k'}(T(X)) \otimes \mathscr{L}(E; F) \\
S^k(E, G) &= TS^k(T(X)) \otimes \mathscr{L}(E; G)
\end{aligned}
$$
cf. 14.2.2,
one deduces from this, by tensor product, a pairing
(*) $$
S^{k''}(F, G) \times S^{k'}(E, F) \to S^k(E, G).
$$
One then has the formula
$$
\sigma_k(D'' \circ D') = \sigma_{k''}(D'') \cdot \sigma_{k'}(D'),
$$

where the product occurring in the right-hand term is defined by the pairing (*) above.

Now suppose K of characteristic zero, and let $x \in X$. Denote by $\sigma$ (resp. $\sigma', \sigma''$) the k-symbol (resp. the $k'$-symbol, the $k''$-symbol) of $D'' \circ D'$ (resp. $D', D''$) at $x$. For every $\omega \in T_x(X)^*$, one then has (with the notations at the end of 14.2.2):

$$
\tilde{\sigma}(\omega) \in \mathscr{L}(E_x; G_x), \quad \tilde{\sigma}'(\omega) \in \mathscr{L}(E_x; F_x), \quad \tilde{\sigma}''(\omega) \in \mathscr{L}(F_x; G_x)
$$

and

$$
\tilde{\sigma}(\omega) = \tilde{\sigma}''(\omega) \circ \tilde{\sigma}'(\omega).
$$

**14.3. Transposition**

In this No., it is assumed that X is purely of dimension $n$.

### 14.3. Transposition

14.3.1. Let $\Omega = \det(T(X)^*)$, cf. 7.9.9; it is a vector bundle of rank 1 at each point, with base X, and of class $C^{r-1}$. One has

$$
\Omega = \wedge^n T(X)^* = \mathrm{Alt}^n(T(X); K_X).
$$

Let M be a vector bundle with base X. Put

$$
\tilde{M} = \mathscr{L}(M; \Omega) = M^* \otimes \Omega.
$$

[^1]

If M is of class $C^n$, with $h \in N_K \cup \{0\}$ and $h \leq r - 1$, the same is true of $\tilde{M}$. The canonical mapping of M into $\tilde{M} = \mathscr{L}(\mathscr{L}(M; \Omega); \Omega)$ is an isomorphism; it is used to identify M with $\tilde{M}$.

14.3.2 ("Definition of the transpose"). Let $k$ be a positive integer $\leq r - 1$, and let D be a differential operator on X, of type $E \to F$, of order $\leq k$, and of class $C^n$, with $h \in N_K \cup \{0\}$ and $k \leq h \leq r - k$. Then there exists a differential operator $^tD$ on X, of type $\bar{F} \to \bar{E}$ and of order $\leq k$, having the following property:

Let $\xi = (\xi^1, \ldots, \xi^n)$ be a system of coordinates in an open set U of X and let $s = (s_i)_{1 \leq i \leq e}$ (resp. $t = (t_j)_{1 \leq j \leq f}$) be a frame of E (resp. of F) on U. Let $(s_i^*)$ (resp. $(t_j^*)$) be the frame of $E^*$ (resp. of $F^*$) such that $\langle s_i, s_j^* \rangle = \delta_{ij}$ (resp. $\langle t_i, t_j^* \rangle = \delta_{ij}$), and let $(\tilde{s}_i)$ (resp. $(\tilde{t}_j)$) be the frame of $\bar{E}$ (resp. $\bar{F}$) on U obtained by forming the tensor product of $(s_i^*)$ (resp. of $(t_j^*)$) with the frame $\omega = d\xi^1 \wedge \cdots \wedge d\xi^n$ of $\Omega$. Let $c_{\alpha}^{ij}$ ($1 \leq i \leq e$, $1 \leq j \leq f$, $|\alpha| \leq k$) be the functions of class $C^n$ on U such that one has

$$
D \left( \sum_i f_i s_i \right) = \sum_{i,j,\alpha} c_{\alpha}^{ij} \Delta_{\xi}^{\alpha}(f_i) \cdot t_j
$$

for arbitrary functions $f_i$ in $C^{h+k}(U)$, cf. 14.1.4, (3'). One then has

$$
{}^tD \left( \sum_j g_j \tilde{t}_j \right) = \sum_{i,j,\alpha} (-1)^{|\alpha|} \Delta_{\xi}^{\alpha}(c_{\alpha}^{ij} g_j) \tilde{s}_i
$$

for arbitrary functions $g_j$ in $C^{h+k}(U)$.

80
DIFFERENTIAL AND ANALYTIC MANIFOLDS § 14

The preceding property (which must be verified whatever $\xi$, $s$ and $t$ may be) determines $^{t}D$ uniquely.[^2] The operator $^{t}D$ is called the transpose of $D$; it is of class $C^{h-k}$. If $h\geq 2k$, the transpose of $^{t}D$ is defined and equal to $D$ (taking into account the identifications of $\widetilde{E}$ and $\widetilde{F}$ with $E$ and $F$ respectively).

The mapping $D\mapsto{}^{t}D$ is $K$-linear. If $k=0$, i.e. if $D$ is a morphism from $E$ into $F$, $^{t}D$ is the morphism $\mathscr{L}(D;\operatorname{Id}_{\Omega})$ from $\widetilde{F}$ into $\widetilde{E}$.

The symbol of $^{t}D$ is deduced from the symbol of $D$ by means of the isomorphism

$$
\operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(E;F)\longrightarrow \operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(\widetilde{F};\widetilde{E})
$$

which is the tensor product of the automorphism $(-1)^k$ of $\operatorname{TS}^{k}(T(X))$ and the isomorphism $u\mapsto\mathscr{L}(u;\operatorname{Id}_{\Omega})$ of $\mathscr{L}(E;F)$ onto $\mathscr{L}(\widetilde{F};\widetilde{E})$.

### 14.3.3 (“Transpose of a Composite”). With the notation and hypotheses of 14.1.8, suppose that $D'$ is of class $C^{h'}$ and $D''$ of class $C^{h''}$, with $h',h''$ in $\mathbf{N}_K\cup\{0\}$, $h'\geq k'+2k''$ and $h''\geq k''+2k'$.

Then the transposes of $D'$, $D''$ and $D''\circ D'$ are defined, as is the composite of $^{t}D'$ and $^{t}D''$, and one has

$$
^{t}(D''\circ D')={}^{t}D'\circ{}^{t}D''.
$$

In particular, with the hypotheses and notation of 14.3.2, and $f$ a function of class $C^{h'}$ on $X$ with $2k\leq h'$, one has $^{t}(D\circ f)=f\circ{}^{t}D$.

#### Example {#var-2-s14-n3-exa-1 .statement}

Let $X$ be an open subset of $K^n$, let $\xi^1,\ldots,\xi^n$ denote the coordinate functions on $X$, and identify $\Omega$ with $K_X$ by means of the frame $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$. If $E=F=K_X$, one has

$$
\widetilde{E}=\widetilde{F}=\mathscr{L}(K_X;\Omega)=\mathscr{L}(K_X;K_X)=K_X,
$$

and the operation $D\mapsto{}^{t}D$ transforms scalar differential operators into scalar differential operators. One has, for example,

$$
{}^{t}(\Delta^\alpha)=(-1)^{|\alpha|}\Delta^\alpha\qquad\text{for every }\alpha\in\mathbf{N}^n.
$$

If $r$ is infinite, transposition is an anti-automorphism of the algebra $\mathscr{D}^{\infty}_{K_X}(K_X,K_X)$.

### 14.3.4. Let $k$ be a positive integer such that $K$ is of characteristic $0$ or $>k$. Let $\Omega_1$ be the vector bundle $\bigwedge^{n-1}T(X)^*=\mathscr{L}(T(X);K_X)$. The notation and hypotheses being those of 14.3.2, let moreover $D'$ be a differential operator on $X$, from $\widetilde{F}\rightarrow\widetilde{E}$, of order $\leq k$; a Green operator for $(D,D')$ is defined to be any multidifferential operator $G$ (cf. 14.1.11) of type $(E,\widetilde{F})\rightarrow\Omega_1$, of order $\leq k-1$[^3] and of class $C^h$ (with $h\geq1$), such that one has the identity

(1)

$$
\langle D(u),v\rangle-\langle u,D'(v)\rangle=d(G(u,v))
$$

for every open set $U$ of $X$ and every elements $u\in\mathscr{S}^k_E(U)$, $v\in\mathscr{S}^k_F(U)$. Let us specify that, in this formula, $d$ denotes exterior differentiation (8.3.5) and $\langle D(u),v\rangle$ (resp.

$\langle u, D'(v) \rangle$) denotes the section of $\Omega$ on $U$ obtained from the pair $(D(u), v)$ (resp. from the pair $(u, D'(v))$) by the canonical pairing of $F \times \tilde{F}$ (resp. of $E \times \tilde{E}$) into $\Omega$. The existence of $G$ implies $D' = {}^tD$; one also says that $G$ is a Green operator for $D$.

14.3.5. Let $D$ be a differential operator on $X$, of type $E \to F$, of order $\leq k$, of class $C^h$ with $h \in N_K$ and $k \leq h \leq r - k$. There exists a Green operator of class $C^{h-k+1}$ for $D$ in each of the following cases:

a) $K = \mathbf{R}$, $r = \infty$ and $X$ is paracompact.
b) $K$ is of characteristic $0$ or $> k$, $X$ is isomorphic to an open set of a space $K^n$, and the bundles $E$ and $F$ are isomorphic to trivial bundles.
c) The operator $D$ is of order $\leq 1$ (cf. 14.3.7).

14.3.6. The hypotheses and notations of 14.3.3 are retained. If $G'$ (resp. $G''$) is a Green operator for $D'$ (resp. $D''$), there exists one and only one Green operator $H$ for $D'' \circ D'$ such that one has

$$
H(u, v) = G''(D'(u), v) + G'(u, {}^tD''(v))
$$

for all open sets $U$ of $X$ and elements $u \in \mathscr{S}_E^k(U)$ and $v \in \mathscr{S}_{\tilde{G}}^k(U)$.

14.3.7. One has $S^1(E, F) = T(X) \otimes E^* \otimes F$ (cf. 14.2.2). On the other hand, the right interior product $(\xi, \omega) \mapsto i(\xi)\omega$ (cf. A, III, p. 158) defines an isomorphism of $T(X) \otimes \Omega$ onto $\Omega_1$; by tensor product with the dual $\Omega^*$ of $\Omega$, one thus obtains an isomorphism of $T(X)$ onto $\Omega^* \otimes \Omega_1$, whence identifications of vector bundles

$$
\begin{align*}
S^1(E, F) &= \Omega^* \otimes \Omega_1 \otimes E^* \otimes F = (E \otimes F^* \otimes \Omega)^* \otimes \Omega_1 \\
&= (E \otimes \tilde{F})^* \otimes \Omega_1 = \mathscr{L}(E \otimes \tilde{F}; \Omega_1).
\end{align*}
$$

This being set, let $D$ be a differential operator on $X$, of type $E \to F$, of order $\leq 1$, of class $C^h$ with $h \in N_K \cup \{0\}$ and $h \leq r - 1$. There exists a unique Green operator for $D$; it is of order $0$; it is a morphism of class $C^h$ from $E \otimes \tilde{F}$ into $\Omega_1$, and it is deduced from the symbol of $D$ by the preceding identification.

14.3.8. Suppose that one has $K = \mathbf{R}$, that $X$ is separated and oriented (10.2.4) and let $A$ be a closed piece (11.1.2) of $X$. Equip $A$ with the orientation induced by that of $X$, and $\partial A$ with the corresponding orientation (11.2.1). Let $k$ be an integer such that $2k \leq r$, $D$ a differential operator on $X$, of type $E \to F$, of order $\leq k$ and of class $C^k$. Let $G$ be a Green operator for $D$. Let $U$ be an open set of $X$, $u \in \mathscr{S}_E^k(U)$, $v \in \mathscr{S}_{\tilde{F}}^k(U)$ and suppose that the supports of $u$ and $v$ meet $A$ in a compact set. One then has

$$
\int_A \langle D(u), v \rangle - \int_A \langle u, {}^tD(v) \rangle = \int_{\partial A} G(u, v)
$$

(*Green's formula*). In particular, if $\partial A = \varnothing$, one has

$$
\int_A \langle D(u), v \rangle = \int_A \langle u, {}^tD(v) \rangle.
$$

### 14.4. Examples

Suppose X purely of finite dimension n. Suppose it is also endowed with a structure of manifold of class C^{r+1} compatible with the given structure of class C^r.

14.4.1 (« Infinitesimal transformations »). Let $\tau$ be a vector functor in finite dimension for isomorphisms, of class C^r; suppose that, for every finite-dimensional vector space V, $\tau(V)$ is finite-dimensional. We denote by $E_{\tau}$ the vector bundle $\tau(T(X))$; it is of class C^r.

Let $\xi$ be a vector field of class C^r on X. There exists a differential operator D of type $E_{\tau} \to E_{\tau}$ and of order $\leq 1$ such that

$$
D_U(s) = \theta_{\xi}.s
$$

for every open set U of X and every $s \in \mathscr{S}_{E_{\tau}}(U)$, cf. 8.4.3. Such a differential operator D is unique; we denote it by $(\theta_{\xi})_{\tau}$ or simply $\theta_{\xi}$. Its symbol is the section $\xi \otimes \mathrm{Id}_{E_{\tau}}$ of the vector bundle

$$
S^1(E_{\tau}, E_{\tau}) = T(X) \otimes \mathscr{L}(E_{\tau}; E_{\tau}).
$$

If V is a finite-dimensional K-vector space, put

$$
\tilde{\tau}(V) = \mathscr{L}(\tau(V); \mathrm{Alt}^n(V; K)) = \tau(V)^* \otimes \wedge^n V^*,
$$

and if $u : V_1 \to V_2$ is an isomorphism, define $\tilde{\tau}(u) : \tilde{\tau}(V_1) \to \tilde{\tau}(V_2)$ by transport of structure. We thus obtain a vector functor in finite dimension $\tilde{\tau}$. The bundle $E_{\tilde{\tau}} = \tilde{\tau}(T(X))$ identifies in the obvious way with the bundle $(E_{\tau})^*$; the transpose of $(\theta_{\xi})_{\tau}$ is $-(\theta_{\xi})_{\tilde{\tau}}$ and formula (1) of no. 14.3.4 takes the form

$$
\langle \theta_{\xi}.u, v \rangle + \langle u, \theta_{\xi}.v \rangle = d(i(\xi)(u.v)).
$$

14.4.2 (« Exterior differential »). For every integer $p \geq 0$ put

$$
\Omega^p = \mathrm{Alt}^p(T(X); K_X).
$$

There exists a differential operator D of type $\Omega^p \to \Omega^{p+1}$ and of order $\leq 1$ such that

$$
D_U(\omega) = d\omega
$$

for every open set U of X and every $\omega \in \mathscr{S}_{\Omega^p}(U)$. Such a differential operator D is unique; we denote it by d (or $d_p$ if we wish to specify the integer p).

Its symbol is the element of $S^1(\Omega^p, \Omega^{p+1})$ obtained as follows: first of all we have

$$
S^1(\Omega^p, \Omega^{p+1}) = T(X) \otimes \mathscr{L}(\Omega^p; \Omega^{p+1})
$$
$$
= \mathscr{L}(\Omega^1; \mathscr{L}(\Omega^p; \Omega^{p+1})) = \mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1}),
$$

where $\mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1})$ denotes the bundle of bilinear mappings of $\Omega^1 \times \Omega^p$ into $\Omega^{p+1}$. Now the exterior product $(\alpha, \beta) \mapsto \alpha \wedge \beta$ defines a canonical section of this latter bundle; this section is the symbol of $d_p$.

To determine the transpose of $d_p$, we first remark that the exterior product defines a pairing $\Omega^p \times \Omega^{n-p} \to \Omega^n = \Omega$ which permits identifying $(\Omega^p)^*$ with $\Omega^{n-p}$. We identify $(\Omega^{p+1})^*$ with $\Omega^{n-p-1}$ in the same way. With these conventions, the transpose of $d_p$ is $(-1)^{p+1} d_{n-p-1}$ and the corresponding Green operator, of type

$(\Omega^p,\Omega^{n-p-1})\longrightarrow\Omega_1=\Omega^{n-1}$, is simply the exterior product (on each fibre).

### 14.4.3 (« Laplacian »).

Let $K=\mathbf{R}$, $r=\infty$, $X=\mathbf{R}^n$, $E=F=K_X$; let $\xi^i$ $(1\leq i\leq n)$ denote the coordinate functions on $X$; put $D_i=\partial/\partial\xi^i$, and $L=\sum_{i=1}^n D_i^2$. The operator $L$ is a scalar differential operator of order $\leq 2$. If we identify $\Omega$ with $K_X$ by means of the frame $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$, we have $\tilde E=\tilde F=K_X$ (cf. 14.3.3, example) and $\tilde L=L$.

For $1\leq i\leq n$, put $\omega_i=(-1)^{i-1}d\xi^1\wedge\cdots\wedge d\xi^{i-1}\wedge d\xi^{i+1}\wedge\cdots\wedge d\xi^n$. The $\omega_i$ form a frame of $\Omega_1=\Omega^{n-1}$. If $f\in\mathscr C^1(X)$, let $\operatorname{grad}(f)$ denote the section $\sum_{i=1}^n D_i(f)\omega_i$ of $\Omega_1$. There exists a Green operator $G$ for $L$ such that

$$G(u,v)=v.\operatorname{grad}(u)-u.\operatorname{grad}(v)$$

for every open set $U$ of $X$ and $u,v$ in $\mathscr C^1(U)$.

In particular, let $A$ be a compact piece of $\mathbf{R}^n$. Orient $\mathbf{R}^n$, endow $A$ with the orientation induced by that of $\mathbf{R}^n$, and $\partial A$ with the corresponding orientation (11.2.1). We have

$$\int_A(Lu).v\omega-\int_Au.(Lv)\omega=\int_{\partial A}(v.\operatorname{grad}(u)-u.\operatorname{grad}(v))$$

for $u,v$ in $\mathscr C^1(X)$.

[^1]: Care should be taken not to confuse $\tilde{M}$ with the covering of M defined in 10.2.4 and denoted in the same way.
[^2]: In fact, it is sufficient to verify the property in question for triples $(\xi^\lambda,s^\lambda,t^\lambda)$ such that the domains of the $\xi^\lambda$ cover $X$.
[^3]: When $k=0$, it is agreed that this means that $G=0$.
