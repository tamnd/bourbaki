---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 8
section_title: Le calcul différentiel d’ordre 1
lang: en
source: var-fr
pdf_pages: 0099-0115
extraction: ocr
subsections:
    - "no": 1
      title: Fibré tangent
      page: 0
      pdf_page: 99
    - "no": 2
      title: Champs de vecteurs
      page: 0
      pdf_page: 100
    - "no": 3
      title: Formes différentielles, différentiation extérieure
      page: 0
      pdf_page: 102
    - "no": 4
      title: Transformations infinitésimales
      page: 0
      pdf_page: 104
    - "no": 5
      title: Le crochet
      page: 0
      pdf_page: 106
    - "no": 6
      title: Relèvements
      page: 0
      pdf_page: 108
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 110
    - "no": 8
      title: Variétés presque complexes et variétés complexes
      page: 0
      pdf_page: 110
statements: 0
exercises: 0
content_sha256: 5480527fe97e663fdd949ef6b0415b3bfc5a05ba2b0dfc094ad038236b442035
translated_from: content/fr/var/2/08_s8_le_calcul_differentiel_d_ordre_1.md
source_lang: fr
translation_method: machine
source_content_sha256: 8e5eb0df8ca06a478d639eada2c7d5b89876793e8c3fe822ad7724a41e0f6db2
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-en-mt-97fbc83a
glossary_version: 34
glossary_terms_sha256: 9ac6d349ded73414d25362144697b9eebad6b1acb1deed7cec418507492dbbe5
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 8. The differential calculus of order 1

Starting from No. 8.3, we suppose

— either that $K$ is of characteristic zero,

— or that the varieties under consideration are locally of finite dimension.

In the latter case, the expressions “Banach space, vector bundle, vector functor” mean respectively “finite-dimensional vector space, vector bundle of finite rank, vector functor in finite dimension with values of finite dimension”.

### 8.1. Tangent bundle

### 8.1.1. — Let $r\in \mathbf{N}_K$ and let $X$ be a $K$-variety of class $C^r$. We denote by $T(X)$ the sum set of the tangent spaces $T_x(X)$ (5.5.1) for $x\in X$, and by $\pi$ the canonical mapping of $T(X)$ onto $X$. Let $c=(U,\varphi,E)$ be a chart of the variety $X$; for $x\in U$ and $t\in T_x(X)$, put $\zeta_c(x,t)=(x,\theta_c^{-1}(t))$, the mapping $\theta_c$ being that defined in 5.5.1. The triplet $c'=(U,\zeta_c,E)$ is a vector chart (7.1.1) of $T(X)$ (endowed with the mapping $\pi:T(X)\longrightarrow X$). There exists on $T(X)$ one and only one structure of vector bundle with base $X$ and of class $C^{r-1}$ such that, for every chart $c$ of $X$, the corresponding vector chart $c'$ is a vector chart of $T(X)$[^1]. Endowed with this structure, $T(X)$ is called the tangent bundle of $X$. In particular, $T(X)$ is endowed with a structure of variety of class $C^{r-1}$ and the triplet $(T(X),X,\pi)$ is a fibration (7.1.4).

Let $U$ be an open subset of a Banach space $E$ and let $i$ be the canonical injection of $U$ into $E$. The vector chart $c'=(U,\zeta_c,E)$ associated with the chart $c=(U,i,E)$ of $U$ defines an isomorphism of $T(U)$ onto the trivial bundle $E_U$ (7.1.5); these two bundles are identified by means of this isomorphism.

If $X$ is a purely variety of type $E$ (5.1.7), $T(X)$ is a purely variety of type $E\times E$.

### 8.1.2. — Let $f:X\longrightarrow Y$ be a morphism of varieties of class $C^r$. We define an $f$-morphism $T(f):T(X)\longrightarrow T(Y)$ of vector bundles of class $C^{r-1}$ by
$$
T(f)(x,t)=(f(x),T_xf(t))
$$
for $x\in X$ and $t\in T_x(X)$.

If $f=\mathrm{Id}_X$, one has $T(f)=\mathrm{Id}_{T(X)}$. For $f:X\longrightarrow Y$ and $g:Y\longrightarrow Z$, one has
$$
T(g\circ f)=T(g)\circ T(f).
$$

### 8.1.3. — Let $f:X\longrightarrow Y$ be a morphism of manifolds of class $C^r$, and let $f':T(X)\longrightarrow f^*T(Y)$

be the unique X-morphism such that T(f) = g ∘ f', where g is the canonical morphism f*T(Y) → T(Y) (cf. 7.2.4).

For f to be an immersion (resp. a submersion), it is necessary and sufficient that 0 → T(X) $\xrightarrow{f'} f^*T(Y)$ (resp. T(X) $\xrightarrow{f'} f^*T(Y) \to 0$) be a locally direct exact sequence (7.5.6). If f is an immersion, the cokernel bundle of f' is called the normal or transverse bundle of f. If f is a submersion, the kernel bundle of f is called the tangent bundle to the fibres of f, or the relative tangent bundle of X over Y, and is denoted T(X/Y). Its fibre T_x(X/Y) at x ∈ X is the tangent space at x to the submanifold $f^{-1}(f(x))$ of X. The sequence

$$
0 \longrightarrow T_x(X/Y) \xrightarrow{i} T_x(X) \xrightarrow{T_{x(f)}} T_{f(x)}(Y) \longrightarrow 0
$$

where i is the canonical injection, is exact.

For f to be étale, it is necessary and sufficient that f' be an isomorphism.

When K has characteristic 0, for f to be a subimmersion, it is necessary and sufficient that f' be locally direct.

8.1.4. Let X_1 and X_2 be two manifolds. We have T(X_1 × X_2) = p_1^*T(X_1) ⊕ p_2^*T(X_2), where p_1 and p_2 are the canonical projections (5.6.3).

8.1.5. Let n be an integer $\geqslant 0$; the tangent bundle T(K^n) of K^n is identified with the trivial bundle with fibre K^n (8.1.1). The constant sections defined by the elements of the canonical basis of K^n form a frame of T(K^n).

If X is a manifold and (u^1, ..., u^n) a system of coordinates of X in an open set U of X (5.1.10), the preceding frame defines by transport of structure a frame of T(X) on U; it is called the tangent frame defined by (u^1, ..., u^n) and is denoted (\partial/\partial u^1, ..., \partial/\partial u^n) (cf. 5.5.8).

### 8.2. Vector fields

Let X be a manifold of class C^r, and let U be an open set of X.

8.2.1. A section (not necessarily continuous, cf. Notations and Conventions) of the tangent bundle T(X) above U is called a vector field on U.

8.2.2. The dual bundle T'(X) (7.7.3) of T(X) is called the cotangent bundle of X. Its sections are called covector fields. If f is a function of class C^k on X (with 1 ≤ k ≤ r), with values in K, its differential df : x ↦ d_x f (5.5.6) is a covector field of class C^{k-1}. More generally, if f is a function of class C^k on X (1 ≤ k ≤ r), with values in a Banach space E, its differential df is a section of class C^{k-1} of the bundle $\mathscr{L}(T(X); E_X)$.

8.2.3. Let $\xi$ be a vector field of class C^{r-1} on X, and let $f \in \mathscr{C}^r(X; F)$ be a function of class C^r with values in a Banach space F. We denote by $\langle \xi, df \rangle$, or D_\xi(f), or again $\xi(f)$ the function $x \mapsto d_x f(\xi(x))$; it is an element of $\mathscr{C}^{r-1}(X; F)$. For fixed f, the mapping $\xi \mapsto D_\xi(f)$ is $\mathscr{C}^{r-1}(X)$-linear. If $D_\xi f = 0$ for every function f of class C^r with values in a Banach space, defined in an open set of X, we have $\xi = 0$.

Let E, F, G be Banach spaces and let (u, v) ↦ u . v be a continuous bilinear mapping of $E \times F$ into $G$. Let $f \in \mathscr{C}^r(X; E)$, $g \in \mathscr{C}^r(X; F)$ and let $f.g \in \mathscr{C}^r(X; G)$ be their product. If $\xi$ is a vector field of class $C^{r-1}$ on $X$, we have
$$
D_\xi(f.g) = D_\xi(f).g + f.D_\xi(g).
$$
In particular, the mapping $D_\xi : \mathscr{C}^r(X) \to \mathscr{C}^{r-1}(X)$ is a derivation of the algebra $\mathscr{C}^r(X)$ into the $\mathscr{C}^r(X)$-module $\mathscr{C}^{r-1}(X)$.

8.2.4. Suppose that $X$ is locally of *finite dimension* and that one of the following two hypotheses is satisfied:

(i) $r = \infty$ and $X$ is separated;
(ii) $r = \omega$ and $X$ is isomorphic to an open polydisc of $K^n$.

Then, for every derivation $D$ of the algebra $\mathscr{C}^r(X)$, there exists one and only one vector field $\xi$ of class $C^r$ such that $D = D_\xi$.

8.2.5. Let $(u^1, \ldots, u^n)$ be a system of coordinates of $X$ in $U$, and $\xi$ a vector field on $U$. The $i$-th coordinate of $\xi$ in the tangent frame (8.1.5) defined by $(u^1, \ldots, u^n)$ is $D_\xi(u^i)$. In other words, we have
$$
\xi = \sum_{1 \leq i \leq n} D_\xi(u^i) \cdot \partial/\partial u^i.
$$

8.2.6. Let $\varphi : X \to Y$ be a morphism of manifolds of class $C^r$, $\xi$ a vector field on $X$ and $\eta$ a vector field on $Y$. We say that $\xi$ is $\varphi$-*related* to $\eta$ if, for every $x \in X$, we have $\eta(\varphi(x)) = T_x(\varphi)(\xi(x))$. Suppose this is so, and that $\xi$ and $\eta$ are of class $C^{r-1}$. Then, for every Banach space $E$, the diagram

$$
\begin{array}{ccc}
\mathscr{C}^r(Y; E) & \xrightarrow{\varphi^*} & \mathscr{C}^r(X; E) \\
\downarrow D_\eta & & \downarrow D_\xi \\
\mathscr{C}^{r-1}(Y; E) & \xrightarrow{\varphi^*} & \mathscr{C}^{r-1}(X; E)
\end{array}
$$

where $\varphi^*(f) = f \circ \varphi$, is commutative.

When $\varphi$ is étale, for every vector field $\eta$ on $Y$, there exists one and only one vector field on $X$ which is $\varphi$-*related* to $\eta$; it is denoted by $\varphi^*\eta$.

8.2.7. Let $\varphi : X \to Y$ be a morphism of manifolds of class $C^r$. If $\omega$ is a covector field$^{(1)}$ on $Y$, we define a covector field $\varphi^*\omega$ on $X$ by
$$
(\varphi^*\omega)(x) = t(T_x(\varphi))(\omega(\varphi(x))) \quad (x \in X).
$$
More generally, let $\tau$ be a vector functor (7.6) of class $C^{r-1}$, of type $(I_+, I_-)$ with $I_+ = \emptyset$ and $I_-$ reduced to one element (such a functor is said to be *contravariant*). If $\omega$ is a section of class $C^{r-1}$ of the vector bundle $\tau(T(Y))$ based on $Y$, we define a section $\varphi^*\omega$ of $\tau(T(X))$ by $(\varphi^*\omega)(x) = \tau(T_x(\varphi))(\omega(\varphi(x)))$ $(x \in X)$.

$^1$ The reader should take care not to confuse this use of the letter $\omega$ with that defined in Notations and Conventions.

### 8.3. Differential forms, exterior differentiation

Let us recall that, in this number and the following ones, it is assumed either that K is of characteristic 0, or that the manifolds considered are locally of finite dimension.

8.3.1. Let X be a manifold of class C' and F a vector bundle of class C^k based on X, with k + 1 \in \mathbf{N}_K and k + 1 \leq r. Let p be an integer $\geq 0$ and let Alt^p(T(X); F) be the vector bundle of class C^k of alternating p-linear mappings of T(X) into F (7.8.1 and Errata to No. 7.8). A section of this bundle over an open set U of X is called an alternating differential form (or simply differential form) of degree p on U, with values in F. Those of these sections which are of class C^k form a $\mathscr{C}^k(U)$-module, denoted ^k\Omega^p(U; F). If E is a Banach space, we write ^k\Omega^p(U; E) instead of ^k\Omega^p(U; E_X) and speak of differential forms with values in E. In this notation, k (resp. E) is sometimes omitted when it is equal to r − 1 (resp. K).

A differential form of degree 0 (resp. 1) with scalar values is a function (resp. a covector field).

Let $\varphi : Y \to X$ be a morphism of manifolds of class C', and let $\omega \in ^k\Omega^p(X; F). There then exists one and only one form $\varphi^*\omega \in ^k\Omega^p(Y; \varphi^*F) such that

(1)
$$(\varphi^*\omega)_y(v_1, \ldots, v_p) = \omega_{\varphi(y)}(T_y(\varphi).v_1, \ldots, T_y(\varphi).v_p)$$

for every y \in Y and every family v_1, \ldots, v_p of elements of T_y(Y).

If $\psi : Z \to Y$ is a morphism of manifolds of class C', we have

(2)
$$(\varphi \circ \psi)^*\omega = \psi^*(\varphi^*\omega).$$

When Y is a submanifold of X and $\varphi$ is the canonical injection, we sometimes write $\omega|Y$ instead of $\varphi^*\omega$ and say that $\omega|Y$ is induced on Y by $\omega$.

8.3.2. The definitions and results of No. 7.8 apply to differential forms. In particular, a pairing of vector bundles F' \times_X F'' \to F gives rise to an exterior product ^k\Omega^{p'}(U; F) \times ^k\Omega^{p''}(U; F'') \to ^k\Omega^p(U; F), where p = p' + p'' (7.8.2); it is denoted by $(\omega', \omega'') \mapsto \omega' \wedge \omega''$. The direct sum of the ^k\Omega^p(U; K) for p \geq 0 is thus endowed with a structure of associative and alternating graded algebra (A, III, p. 53).

Let $\xi$ be a vector field on X and $\omega$ a differential form of degree p \geq 1 on X, with values in a vector bundle F; the interior product of $\xi$ and $\omega$ is the differential form i(\xi, \omega) of degree p − 1 on X, with values in F, defined by

(3)
$$i(\xi, \omega)_x(v_1, \ldots, v_{p-1}) = \omega_x(\xi(x), v_1, \ldots, v_{p-1})$$

for every x \in X and every family v_1, \ldots, v_{p-1} of elements of T_x(X). If $\omega$ is a differential form of degree 0, we put i(\xi, \omega) = 0. We also write i(\xi)\omega or i_\xi\omega instead of i(\xi, \omega). When F = K_X, the definition given above coincides with that of 7.8.4.

Let F' \times_X F'' \to F be a pairing of vector bundles. For $\omega' \in ^k\Omega^{p'}(U; F') and $\omega'' \in ^k\Omega^{p''}(U; F''), we have

(4)
$$i(\xi)(\omega' \wedge \omega'') = (i(\xi)\omega') \wedge \omega'' + (-1)^{p'\omega'} \wedge i(\xi)\omega''.$$

8.3.3. Let $(u^1, \ldots, u^n)$ be a system of coordinates in the open set $U$ of $X$. Every element $\omega$ of $^{k}\Omega^p(U; F)$ is written in a unique way
$$
\omega = \sum_{i_1 < \cdots < i_p} f_{i_1, \ldots, i_p} \cdot du^{i_1} \wedge \cdots \wedge du^{i_p}
$$
where the $f_{i_1, \ldots, i_p}$ are sections of class $C^k$ of $F$ on $U$; in this formula, the sign $\wedge$ is relative to the canonical pairing $K_X \times_X K_X \to K_X$ and the point designating the product is relative to the canonical pairing $F \times_X K_X \to F$.

8.3.4. Let $p$ be an integer $\geqslant 0$ and $r$ an element of $N_K$. Let $E$ and $F$ be Banach spaces, $U$ an open set of $E$ and $\alpha \in {}^r\Omega^p(U; F)$. Let $\tilde{\alpha} \in C^r(U; Alt^p(E; F))$ be the element corresponding to $\alpha$. If $x \in U$, the differential $d_x \tilde{\alpha}$ of $\tilde{\alpha}$ at $x$ (5.5.6) is an element of $\mathscr{L}(E; Alt^p(E; F))$; if $t \in E$, we have $(d_x \tilde{\alpha})(t) \in Alt^p(E; F)$, and, if $t_1, \ldots, t_p$ are in $E$, we have $(d_x \tilde{\alpha})(t)(t_1, \ldots, t_p) \in F$. There exists one and only one element $d\alpha$ of ${}^{r-1}\Omega^{p+1}(U; F)$ such that one has
$$
(d\alpha)_x(t_0, \ldots, t_p) = \sum_{i=0}^p (-1)^i (d_x \tilde{\alpha})(t_i)(t_0, \ldots, \hat{t}_i, \ldots, t_p) \tag{1}
$$
whatever $x \in U$ and $t_0, \ldots, t_p$ in $E$ may be.

8.3.5. Let $p$ be an integer $\geqslant 0$ and $r$ an element of $N_K$. Let $X$ be a variety of class $C^{r+1}$, $F$ a Banach space, and $\omega \in {}^r\Omega^p(X; F)$. There exists one and only one differential form $\pi \in {}^{r-1}\Omega^{p+1}(X; F)$ such that, for every chart $c = (U, \varphi, E)$ of $X$, if $\omega_c$ is the differential form on $\varphi(U)$ such that $\omega|U = \varphi^*(\omega_c)$, one has $\pi_c = d\omega_c$, where $d\omega_c$ is defined by formula (5) of 8.3.4.

The differential form $\pi$ is called the *exterior differential* of $\omega$; it is denoted $d\omega$. It has the following properties:

(6) If $\psi : Y \to X$ is a morphism of manifolds of class $C^{r+1}$, and if $\omega \in {}^r\Omega^p(X; F)$, one has $\psi^*(d\omega) = d(\psi^*\omega)$; in particular, $d$ commutes with the operation of restriction to a submanifold.
(7) For $p = 0$, the mapping $d : {}^r\Omega^0(X; F) \to {}^{r-1}\Omega^1(X; F)$ coincides with that defined in 8.2.2.
(8) If $r \geqslant 2$ and if $\omega \in {}^r\Omega^p(X; F)$, one has $d(d\omega) = 0$.\footnote{The sign $\wedge$ indicates that the symbol above which it is placed is to be omitted (cf. 7.8.4).}
(9) For every continuous linear mapping $u : F \to F'$ of Banach spaces, one has $d(u(\omega)) = u(d(\omega))$ for $\omega \in {}^r\Omega^p(U; F)$.
(10) For every continuous bilinear mapping $F' \times F'' \to F$ of Banach spaces, one has
$$
d(\omega' \wedge \omega'') = (d\omega') \wedge \omega'' + (-1)^{p'} \omega' \wedge d\omega''
$$
for $\omega' \in {}^r\Omega^{p'}(X; F')$ and $\omega'' \in {}^r\Omega^{p''}(X; F'')$.

8.3.6. Let $(u^1, \ldots, u^n)$ be a system of coordinates of $X$ in $U$. Let
$$
\omega = \sum_{i_1 < \cdots < i_p} f_{i_1, \ldots, i_p} \cdot du^{i_1} \wedge \cdots \wedge du^{i_p}
$$

1 The sign $\wedge$ indicates that the symbol above which it is placed is to be omitted (cf. 7.8.4).
2 If $\omega \in {}^1\Omega^p(X; F)$ and if $d\omega \in {}^1\Omega^{p+1}(X; F)$, one still has $d(d\omega) = 0$.

a differential form on U (with $f_{i_1, ..., i_p} \in \mathscr{C}^r(U; F)$). One then has

$$
d\omega = \sum_{i_1 < ... < i_p} df_{i_1, ..., i_p} \wedge du^{i_1} \wedge \cdots \wedge du^{i_p}.
$$

8.3.7. Suppose that K is of characteristic zero. Let $\omega \in {}^r\Omega^p(X; F)$ be a differential form of degree $p \geq 1$ such that $d\omega = 0$. For every $x \in X$, there exists an open neighbourhood U of $x$ and a differential form $\pi \in {}^r\Omega^{p-1}(U; F)$ such that $d\pi = \omega$ on U.

**8.4. Infinitesimal transformations**

Let $r \in \mathbf{N}_K$ and X be a manifold of class $C^{r+1}$.

### 8.4. Infinitesimal transformations

8.4.1. Let $\tau$ be a vector functor for isomorphisms (7.6.6), of class $C^r$. If E is a Banach space, denote by $\mathbf{GL}(E)$ the open subset of $\mathscr{L}(E; E)$ consisting of the automorphisms of E. Denote by $\tau'_E$ the tangent linear mapping at the identity element $\mathrm{Id}_E$ of the morphism $\tau : \mathbf{GL}(E) \to \mathbf{GL}(\tau(E))$; it is a continuous linear mapping of $\mathscr{L}(E; E)$ into $\mathscr{L}(\tau(E); \tau(E))$.

8.4.2. Let E be a Banach space and put $F = \tau(E)$. Let U be an open subset of E, $\xi$ a vector field on U of class $C^r$, $\tilde{\xi} : U \to E$ the corresponding mapping (obtained by identifying T(U) and $U \times E$ (8.1.1)), and $f : U \to F$ a mapping of class $C^r$. For $x \in U$, define an element $(\theta_{\xi}.f)(x)$ of F by the formula

$$
(\theta_{\xi}.f)(x) = d_x f(\tilde{\xi}(x)) - \tau'_E(d_x \tilde{\xi})(f(x)).
$$

(Let us remark that on the one hand $\tilde{\xi}(x) \in E$ and $d_x f \in \mathscr{L}(E; F)$, whence $d_x f(\tilde{\xi}(x)) \in F$, and on the other hand, $d_x \tilde{\xi} \in \mathscr{L}(E; E)$, $\tau'_E(d_x \tilde{\xi}) \in \mathscr{L}(F; F)$ and $f(x) \in F$, whence $\tau'_E(d_x \tilde{\xi})(f(x)) \in F$. The function $\theta_{\xi}.f : x \mapsto (\theta_{\xi}.f)(x)$ is of class $C^{r-1}$ in U.

8.4.3. Let F denote the vector bundle $\tau(T(X))$ (7.6.2 and 7.6.6). Let $\xi$ be a vector field on X and $f$ a section of F, both of class $C^r$. Let $x$ be a point of X and $c = (U, \varphi, E)$ a chart of X at $x$. Let $c' = (U, \zeta_c, E)$ be the corresponding vector chart of T(X) (8.1.1) and $\tau(c') = (U, \psi_c, \tau(E))$ the corresponding vector chart of F (7.6.2). Put $x_c = \varphi(x)$; let $\xi_c$ be the mapping of $\varphi(U)$ into E such that $\zeta_c(\xi(u)) = (u, \xi_c(\varphi(u)))$ and $f_c$ the mapping of $\varphi(U)$ into $\tau(E)$ such that $\psi_c(f(u)) = (u, f_c(\varphi(u)))$ for all $u \in U$. Let $a_c$ be the element $(\theta_{\xi_c}.f_c)(x_c)$ of $\tau(E)$ defined in 8.4.2. There exists one and only one element $a$ of $F_x$ such that $\psi_c(a) = (x, a_c)$ for every chart $c$ of X at $x$. We denote it by $(\theta_{\xi}.f)(x)$. It depends only on the germs of $\xi$ and $f$ at $x$ (and even only on their jet of order 1 (12.1.2)).

The mapping $\theta_{\xi}.f : x \mapsto (\theta_{\xi}.f)(x)$ is a section of class $C^{r-1}$ of F; it depends K-bilinearly on the pair $(\xi, f)$.

8.4.4. Let us retain the preceding hypotheses and notations. There exists (7.6.4) one and only one morphism of vector bundles $\tau'$ from $\mathscr{L}(T(X); T(X))$ into $\mathscr{L}(F; F)$ such that, for every $x \in X$, the restriction of $\tau'$ to the fibre $\mathscr{L}(T(X); T(X))_x = \mathscr{L}(T_x(X); T_x(X))$ is equal to $\tau'_{T(x)}$ (8.4.1). If $g$ is a function of class $C^r$ in $X$, with values in $K$, we have
$$
\theta_{g\xi}.f = g \theta_\xi.f - \tau'(dg \otimes \xi)(f)
$$
(in this formula, we identify $dg \otimes \xi$, which is a section of $T'(X) \otimes T(X)$, with a section of $\mathscr{L}(T(X); T(X))$; its image $\tau'(dg \otimes \xi)$ is a section of $\mathscr{L}(F; F)$ and transforms $f$ into a section of $F$).

8.4.5. Let $I$ be an open set in $K$ containing $0$, $U$ an open set in $X$ and $\varphi$ a mapping of class $C^r$ from $I \times U$ into $X$. For $(t, x) \in I \times U$, denote by $\varepsilon_{t,x}$ the vector $(1, 0) \in K \times T_x(X) = T_{(t,x)}(I \times U)$. For $t \in I$, denote by $\varphi_t$ the mapping from $U$ into $X$ defined by $\varphi_t(x) = \varphi(t, x)$ ($x \in U$). We suppose that the following three conditions are satisfied:

a) $\varphi_0$ is the canonical injection of $U$ into $X$;
b) for every $t \in T$, the mapping $\varphi_t$ is an isomorphism of $C^r$ class manifolds of $U$ onto an open set of $X$;
c) the section $(t, x) \mapsto T_{(t, x)}(\varphi)(\varepsilon_{t, x})$ of the vector bundle $\varphi^*T(X)$ is of class $C^r$.
Moreover, put:
d) $\xi(x) = T_{(0, x)}(\varphi)(\varepsilon_{0, x})$ for every $x \in U$.

The mapping $\xi : x \mapsto \xi(x)$ is a vector field of class $C^r$ on $U$. We call it the initial (or starting) vector field of $\varphi$.

Let $\tau$ be a vector functor for isomorphisms, of class $C^r$; put $F = \tau(T(X))$ and let $f$ be a section of class $C^r$ of $F$ over $X$. For $x \in U$ and $t \in I$, put $\varphi_t^*f(x) = \tau(T_x(\varphi_t)^{-1})(f(\varphi_t(x)))$; this is an element of $F_x$. The mapping $t \mapsto \varphi_t^*f(x)$ of $I$ into $F_x$ is of class $C^{r-1}$ for all $x \in U$ and one has
$$
\frac{d}{dt} (\varphi_t^*f(x))_{t=0} = (\theta_\xi.f)(x) \quad \text{pour tout } x \in U.
$$

8.4.6. Given a vector field $\xi$ of class $C^r$ on $X$ and a point $x_0$ of $X$, there exists an open set $I$ of $K$, containing $0$, an open set $U$ of $X$ containing $x_0$ and a mapping $\varphi : I \times U \to X$ of class $C^r$ satisfying conditions $a), b)$ and c) of 8.4.5 and such that the initial field of $\varphi$ is the restriction $\xi|U$ of $\xi$ to $U$.

8.4.7. *Example.* — Let $F$ be a Banach space and let $p$ be an integer $\geqslant 0$. If $V$ is a Banach space, put $\alpha_p(V) = \mathrm{Alt}^p(V; F)$; if $u$ is an isomorphism of $V$ onto a Banach space $V'$, denote by $\alpha_p(u)$ the isomorphism of $\alpha_p(V)$ onto $\alpha_p(V')$ deduced from $u$ by transport of structure. We thus obtain a vector functor for isomorphisms, denoted by $\alpha_p$ (7.8.1 and *Errata* to No. 7.8). We can apply to it what precedes; we have
$$
\alpha_p(T(X)) = \mathrm{Alt}^p(T(X); F).
$$
The sections of $\alpha_p(T(X))$ are the differential forms of degree $p$ on $X$, with values in $F$; if $\omega$ is such a form and if $\xi$ is a vector field on $X$, both of class $C^r$, $\theta_\xi.\omega$ is a differential form of degree $p$ on $X$, with values in $F$ and of class $C^{r-1}$. We have
$$
\theta_\xi.\omega = d(i(\xi)\omega) + i(\xi)d\omega
$$

and, when $r \geq 2$,

$$
\theta_\xi \cdot d\omega = d(\theta_\xi \cdot \omega).
$$

When $p = 0$, the functor $\alpha_p$ is the constant vector functor defined by $F$; the bundle $\alpha_0(T(X))$ is identified with the trivial bundle $F_X$, and the sections of this bundle are identified with the functions on $X$ with values in $F$. If $\xi$ is a vector field of class $C^r$ on $X$ and if $f \in \mathscr{C}^r(X; F)$, we have

$$
\theta_\xi \cdot f = \langle \xi, df \rangle = D_\xi(f) \quad (8.2.3);
$$

it is an element of $\mathscr{C}^{r-1}(X; F)$.

8.4.8. Let $\tau$ and $\tau_1$ be two vector functors for isomorphisms. A morphism of vector functors $h : \tau_1 \to \tau$ defines a morphism of vector bundles, also denoted by $h$, from $\tau_1(T(X))$ into $\tau(T(X))$ (7.6.4), and makes correspond to a section $f$ of $\tau_1(T(X))$ a section $h(f)$ of $\tau(T(X))$. If $\xi$ is a vector field on $X$, and if $f$ and $\xi$ are of class $C^r$, we have $\theta_\xi \cdot h(f) = h(\theta_\xi \cdot f)$.

More generally, let $\tau, \tau_1, \ldots, \tau_d$ be vector functors for isomorphisms and let $h : (\tau_1, \ldots, \tau_d) \to \tau$ be a $d$-linear morphism (7.6.4). Let $f_i \in \mathscr{S}_{\tau_i(T(X))}^r(X)$ (for $i = 1, \ldots, d$), and let $\xi$ be a vector field of class $C^r$ on $X$. We have

$$
\theta_\xi \cdot h(f_1, \ldots, f_d) = \sum_{1 \leq i \leq d} h(f_1, \ldots, f_{i-1}, \theta_\xi \cdot f_i, f_{i+1}, \ldots, f_d).
$$

For example, if $f$ is a section of $\tau(T(X))$ and $g$ a function on $X$, with values in $K$, both of class $C^r$, we have

$$
\theta_\xi \cdot (gf) = (\theta_\xi \cdot g)f + g(\theta_\xi \cdot f).
$$

If $\omega_1$ and $\omega_2$ are two differential forms of class $C^r$, with values in Banach spaces $F_1$ and $F_2$ respectively, we have

$$
\theta_\xi \cdot (\omega_1 \wedge \omega_2) = (\theta_\xi \cdot \omega_1) \wedge \omega_2 + \omega_1 \wedge (\theta_\xi \cdot \omega_2),
$$

the exterior product being taken with respect to a continuous bilinear mapping of $F_1 \times F_2$ into a Banach space $F$.

8.4.9. Let $\tau$ be a vector functor for isomorphisms, contravariant (8.2.7), of class $C^r$, $\varphi : X \to Y$ a morphism of manifolds of class $C^{r+1}$, $\xi$ (resp. $\eta$) a vector field of class $C^r$ on $X$ (resp. $Y$) such that $\xi$ is $\varphi$-related to $\eta$ (8.2.6). For every section $f$ of $\tau(T(Y))$, of class $C^r$, we have

$$
\varphi^*(\theta_\eta \cdot f) = \theta_\xi \cdot \varphi^*f.
$$

### 8.5. The bracket

Let $r \in \mathbf{N}_k$ and let $X$ be a manifold of class $C^{r+1}$.

8.5.1. Apply the definitions of No. 8.4 taking for $\tau$ the identity functor: $\tau(V) = V$ for every Banach space $V$ and $\tau(u) = u$ for every isomorphism $u$ of Banach spaces. We then have $\tau(T(X)) = T(X)$. If $\xi$ and $\eta$ are two vector fields of class $C^r$ on $X$, we put

(1)
$$
[\xi, \eta] = \theta_{\xi} \cdot \eta;
$$
this is a vector field of class $C^{r-1}$ on $X$, called the bracket of $\xi$ and $\eta.

8.5.2. The mapping $(\xi, \eta) \mapsto [\xi, \eta]$ is K-bilinear and alternating. If $f$ and $g$ are functions of class $C^r$ on $X$, with values in $K$, one has:

(2)
$$
[f\xi, g\eta] = fg[\xi, \eta] + (fD_{\xi}g)\eta - (gD_{\eta}f)\xi.
$$

8.5.3. Let $F$ be a Banach space. One has

(3)
$$
D_{[\xi, \eta]} = D_{\xi} \circ D_{\eta} - D_{\eta} \circ D_{\xi}
$$
in the space of mappings from $\mathscr{C}^{r+1}(X; F)$ into $\mathscr{C}^{r-1}(X; F)$.

If $r \geqslant 2$ and if $\zeta$ is a third vector field of class $C^r$ on $X$, one has

(4)
$$
[[\xi, \eta], \zeta] = [\xi, [\eta, \zeta]] - [\eta, [\xi, \zeta]] \tag{1}
$$
or equivalently
$$
[\xi, [\eta, \zeta]] + [\eta, [\zeta, \xi]] + [\zeta, [\xi, \eta]] = 0.
$$

More generally, if $r \geqslant 2$ and if $\tau$ is a vector functor for isomorphisms, one has

(5)
$$
\theta_{[\xi, \eta]} = \theta_{\xi} \circ \theta_{\eta} - \theta_{\eta} \circ \theta_{\xi}
$$
in the space of mappings from $\mathscr{S}_{F}^{r}(X)$ into $\mathscr{S}_{F}^{r-2}(X)$ (with $F = \tau(T(X))$).

If $r \geqslant \infty$, the vector fields of class $C^r$ on $X$ form a K-Lie algebra for the bracket (LIE, I, § 1, No. 2).

8.5.4. Let $E$ be a Banach space, $U$ an open subset of $E$, $\xi$ and $\eta$ two vector fields of class $C^r$ on $U$, identified with elements of $\mathscr{C}^r(U; E)$. Their bracket is given by the formula:

(6)
$$
[\xi, \eta] = D_{\xi}\eta - D_{\eta}\xi.
$$

8.5.5. Let $(u^1, \ldots, u^n)$ be a coordinate system of $X$ in an open subset $U$. Let $\xi = \sum a^i \frac{\partial}{\partial u^i}$ and $\eta = \sum b^i \frac{\partial}{\partial u^i}$ be two vector fields of class $C^r$ on $U$. Put
$$
[\xi, \eta] = \sum c^i \frac{\partial}{\partial u^i}.
$$
One has

(7)
$$
c^i = \sum_{1 \leq j \leq n} \left( a^j \frac{\partial b^i}{\partial u^j} - b^j \frac{\partial a^i}{\partial u^j} \right).
$$

8.5.6. Let $\varphi : X \to Y$ be a morphism of varieties of class $C^{r+1}$, $\xi_1$ and $\xi_2$ two vector fields

1 The formula (4) is still exact if one assumes only that the vector fields $\xi, \eta, \zeta, [\xi, \eta], [\eta, \zeta], [\zeta, \xi]$ are all of class $C^1$.

of vector fields on X, $\eta_1$ and $\eta_2$ two vector fields on Y, all of class $C^r$. If $\xi_1$ and $\xi_2$ are $\varphi$-related to $\eta_1$ and $\eta_2$ respectively, $[ \xi_1, \xi_2 ]$ is $\varphi$-related to $[ \eta_1, \eta_2 ]$.

8.5.7. Let $\omega$ be a differential form of degree $p$ on X, with values in a Banach space F and of class $C^r$, and let $\xi_0, \ldots, \xi_p$ be vector fields of class $C^r$ on X. We have

(8) $$
(\theta_{\xi_0} \cdot \omega)(\xi_1, \ldots, \xi_p) = D_{\xi_0} \omega(\xi_1, \ldots, \xi_p) - \sum_{i=1}^p \omega(\xi_1, \ldots, [\xi_0, \xi_i], \ldots, \xi_p)
$$
and
(9) $$
d\omega(\xi_0, \ldots, \xi_p) = \sum_{i=0}^p (-1)^i D_{\xi_i} \omega(\xi_0, \ldots, \hat{\xi}_i, \ldots, \xi_p)
+ \sum_{i<j} (-1)^{i+j} \omega([\xi_i, \xi_j], \xi_0, \ldots, \hat{\xi}_i, \ldots, \hat{\xi}_j, \ldots, \xi_p).
$$

If $\xi$ and $\eta$ are vector fields of class $C^r$, we have
(10) $$
\theta_{\xi} \circ i(\eta) - i(\eta) \circ \theta_{\xi} = i([\xi, \eta])
$$
in the space of mappings from $r\Omega^p(X; F)$ into $r-1\Omega^{p-1}(X; F)$.
For $p = 1$, formula (9) reads:
(11) $$
d\omega(\xi, \eta) = D_{\xi} \langle \eta, \omega \rangle - D_{\eta} \langle \xi, \omega \rangle - \langle [\xi, \eta], \omega \rangle.
$$

### 8.6. Liftings

Let $r \in \mathbf{N}_k$ and let $g : X \to Y$ be a morphism of class $C^{r+1}$ manifolds.

8.6.1. A lifting of $g$ into $T(Y)$ is a mapping $\psi : X \to T(Y)$ such that the diagram

$$
\begin{array}{ccc}
& & T(Y) \\
& \nearrow \psi & \downarrow \pi \\
X & \xrightarrow{g} & Y
\end{array}
$$

is commutative, $\pi$ denoting the canonical projection of $T(Y)$ onto Y. The data of $\psi$ is equivalent to that of a section of the vector bundle $g^*T(Y)$ inverse image by $g$ of $T(Y)$.

The notion of lifting generalizes that of vector field (to which it reduces when $g = \mathrm{Id}_X$); an important part of the definitions and results concerning $\theta_{\xi}$ and $i(\xi)$ extends to liftings; we shall restrict ourselves to briefly indicating a few of them.

8.6.2. Let $\psi : X \to T(Y)$ be a lifting of $g : X \to Y$, and let $\omega$ be a differential form of degree $p$ on Y, with values in a vector bundle F with base Y. When $p \geqslant 1$, we denote by $i(\psi, \omega)$ or $i(\psi)\omega$ or $i_\psi(\omega)$ the differential form on X, of degree $p - 1$, with values in $g^* F$, such that

(1)
$$
i(\psi, \omega)_x(v_1, \ldots, v_{p-1}) = \omega_{g(x)}(\psi(x), T_x(g).v_1, \ldots, T_x(g).v_{p-1})
$$
for every $x \in X$ and every family $v_1, \ldots, v_{p-1}$ of elements of $T_x(X)$. When $p = 0$, we set $i(\psi, \omega) = 0$. We say that $i(\psi, \omega)$ is the interior product of $\psi$ and $\omega$; if $\psi$ and $\omega$ are of class $C^r$, the same is true of $i(\psi, \omega)$. Let $F' \times_Y F'' \to F$ be a pairing of vector bundles over Y. For $\omega' \in {}^r\Omega^{p'}(Y; F')$ and $\omega'' \in {}^r\Omega^{p''}(Y; F'')$, we have

(2)
$$
i(\psi)(\omega' \wedge \omega'') = (i(\psi)\omega') \wedge g^*\omega'' + (-1)^{p'}g^*\omega' \wedge i(\psi)\omega''.
$$

8.6.3. *Examples*

a) A vector field $\xi$ on X defines a lifting $T(g) \circ \xi$ of $g$ into $T(Y)$, and we have:

(3)
$$
i(T(g) \circ \xi) = i(\xi) \circ g^*.
$$

b) A vector field $\eta$ on Y defines a lifting $\eta \circ g$ of $g$ into $T(Y)$, and we have:

(4)
$$
i(\eta \circ g) = g^* \circ i(\eta).
$$

c) More generally, let $h : Y \to Z$ be a morphism of varieties of class $C^{r+1}$. If $\psi$ is a lifting of $g$ into $T(Y)$, then $T(h) \circ \psi$ is a lifting of $h \circ g$ into $T(Z)$ and we have:

(5)
$$
i(T(h) \circ \psi) = i(\psi) \circ h^*.
$$

If $\varphi$ is a lifting of $h$ into $T(Z)$, then $\varphi \circ g$ is a lifting of $h \circ g$ into $T(Z)$ and we have:

(6)
$$
i(\varphi \circ g) = g^* \circ i(\varphi).
$$

8.6.4 (*Infinitesimal transformations*). Let $\psi$ be a lifting of class $C^r$ of $g$ and let $\omega$ be a differential form of degree $p$ on Y, with values in a Banach space F, and of class $C^r$. The differential form on X

(7)
$$
d(i(\psi)\omega) + i(\psi)d\omega
$$
is of degree $p$ and of class $C^{r-1}$; we denote it by $\theta_{\psi}.\omega$.

If $f$ is a function of class $C^r$ on X, we have

(8)
$$
\theta_{f\psi}.\omega = df \wedge i(\psi)\omega + f\theta_{\psi}.\omega.
$$

8.6.5 (*Characterization of $\theta_{\psi}.\omega$ as a derivative*). Retain the hypotheses of 8.6.4. Let $x \in X$. There then exists an open neighbourhood U of $x$, an open neighbourhood I of 0 in K, and a morphism $G : I \times U \to Y$, of class $C^r$, having the following two properties:

a) For every $x \in U$, we have $G(0, x) = g(x)$.

b) For every $x \in U$, the image by $T_{(0, x)}(G)$ of the tangent vector $(1, 0)$ is equal to $\psi(x)$.

Suppose that (U, I, G) satisfies these conditions; for every $t \in I$, denote by $G_t$ the mapping $x \mapsto G(t, x)$ from X into Y; put $\omega_t = G_t^*(\omega)$. For every $x \in X$, the mapping $t \mapsto \omega_t(x)$ from I into $\mathrm{Alt}^p(T_x(X), F)$ is of class $C^r$, and its derivative at the origin is given by the formula

$$
\frac{d}{dt} (\omega_t(x))_{t=0} = (\theta_\psi \cdot \omega)(x).
$$

### 8.7. Weakening of structure

In this no., we suppose $K = \mathbf{R}$.

8.7.1. Let X be a manifold of class $C^s$, and let F be a vector bundle over X, of class $C^k$, with $0 \leq k \leq s$. If $0 \leq k' \leq k$, there exists on F one and only one structure $F_{k'}$ of vector bundle with base X and of class $C^{k'}$ such that every vector bundle chart of F is a vector bundle chart of $F_{k'}$. We say that $F_{k'}$ is obtained from F by weakening the bundle structure of F.

8.7.2. Let $r \in \mathbf{N}_\mathbf{R}$ with $r \leq s$, and let $X_r$ be the manifold of class $C^r$ underlying X (5.13.1). The tangent bundle $T(X_r)$ is of class $C^{r-1}$; it is the bundle obtained by weakening the structure from the tangent bundle $T(X)$, which is of class $C^{s-1}$.

Let F be a vector bundle over X, of class $C^k$, for $0 \leq k \leq r - 1$. The differential forms of class $C^k$ on X with values in F are canonically identified with the corresponding differential forms on $X_r$. The various operations on these forms described in the remainder of this paragraph are compatible with this identification.

In what follows in this fascicle, we shall often leave it to the reader to make explicit the other results of this kind.

### 8.8. Almost complex manifolds and complex manifolds

In this no., we suppose $K = \mathbf{R}$ and denote by X a (real) manifold of class $C^r$, with $r \in \mathbf{N}_\mathbf{R}$.

8.8.1 (« Complex vector bundles »). A vector bundle over C with base X (7.3.4) is also called a complex vector bundle with base X. If M is such a vector bundle, we call a complex vector bundle chart of M a triple $(U, \varphi, E)$, where U is an open set in X, E a complex Banach space and $\varphi$ an isomorphism of complex vector bundles of $M|U$ onto the trivial bundle $E_U = U \times E$. A family $(U_i, \varphi_i, E_i)$ of complex vector bundle charts of M whose domains of definition $U_i$ cover X is called a complex vector bundle atlas of M; every complex vector bundle possesses a complex vector bundle atlas (7.3.3).

We sometimes say C-vectorial instead of complex vectorial. Analogously, we sometimes say, when we wish to speak of a vector bundle over $\mathbf{R}$, of an ordinary vector bundle chart of this bundle, etc., « real vectorial » or « R-vectorial » instead of « vectorial ».

Let M be a complex vector bundle with base X. There exists one and only one automorphism $j$ of the underlying (real) vector bundle of M (7.3.3) whose restriction to each fibre is multiplication by the element i of C; the square of j is equal to −1. Conversely, if M is a (real) vector bundle with base X and j an automorphism of M such that $j^2 = -1$, there exists on M a unique structure of complex vector bundle admitting M as its underlying (real) vector bundle and for which j is multiplication by i.

8.8.2 (« Complexification of a vector bundle »). We define a vectorial functor τ by setting $\tau(E) = E \otimes \mathbf{C}$ for every (real) Banach space E, and $\tau(u) = u \otimes \mathrm{Id}_\mathbf{C}$ for every morphism $u : E \to E'$ of (real) Banach spaces.

If $F$ is a vector bundle with base $X$ and of class $C^k$ ($0 \leq k \leq r$), its transform by the vector bundle functor $\tau$ is denoted $F \otimes \mathbf{C}$. There exists on $F \otimes \mathbf{C}$ a unique structure of complex vector bundle with base $X$ and of class $C^k$, compatible with its structure as a (real) vector bundle and inducing on each fibre $(F \otimes \mathbf{C})_x = F_x \otimes \mathbf{C}$ its canonical structure as a complex Banach space (EVT, II, § 8, No. 1, Example). Endowed with this structure, $F \otimes \mathbf{C}$ is called the complexification of $F$.

Let $U$ be an open subset of $X$; the canonical mapping

$$
\mathscr{S}_F^k(U) \otimes \mathbf{C} \to \mathscr{S}_{F \otimes \mathbf{C}}^k(U)
$$

is an isomorphism, by which these two spaces are identified. If $s \in \mathscr{S}_{F \otimes \mathbf{C}}^k(U)$, the elements $\sigma, \tau$ of $\mathscr{S}_F^k(U)$ such that $s = \sigma + i \tau$ are called the real part and the imaginary part of $s$; the section $\bar{s} = \sigma - i \tau$ is called the conjugate of $s.

In particular, a section of the bundle $T(X) \otimes \mathbf{C}$ is called a complex vector field on $X$.

Let $H$ be a complex vector bundle with base $X$. The canonical isomorphisms $\mathrm{Alt}_\mathbf{R}^p(T_x(X); H) \to \mathrm{Alt}_\mathbf{C}^p(T_x(X) \otimes \mathbf{C}; H)$ define an isomorphism of complex vector bundles, called canonical, of $\mathrm{Alt}_\mathbf{R}^p(T(X); H)$ onto $\mathrm{Alt}_\mathbf{C}^p(T(X) \otimes \mathbf{C}; H)$ (7.8.5), by means of which we shall identify these two bundles. Let $\omega$ be a section of this bundle, in other words a differential form of degree p on $X$, with values in $H$, and let $\zeta$ be a complex vector field, with real part $\xi$ and imaginary part $\eta$. We then put:

$$
i(\zeta, \omega) = i(\xi, \omega) + i.i(\eta, \omega).
$$

If $H$ is a trivial bundle, we put

$$
\theta_\zeta.\omega = \theta_\xi.\omega + i \theta_\eta.\omega.
$$

Analogously, we extend the bracket by linearity to complex vector fields. The formulas of the preceding Nos. remain valid.

8.8.3. A structure of class $C^k$ ($k \leq r - 1$) on $X$ is called an almost complex structure if it is the datum of a complex vector bundle structure on $T(X)$, of class $C^k$, whose underlying real structure is the natural structure of $T(X)$. Such a structure is equivalent to the datum of an automorphism j of class $C^k$ of $T(X)$ such that $j^2 = -1$.

Let us give ourselves such a structure. Extend j to a $\mathbf{C}$-automorphism of $T(X) \otimes \mathbf{C}$. There exists one and only one decomposition of $T(X) \otimes \mathbf{C}$ into a direct sum of two complex subbundles:

(1)

$$
T(X) \otimes \mathbf{C} = T'(X) \oplus T''(X)
$$

such that $j$ coincides with multiplication by $i$ on $T'(X)$ and by $-i$ on $T''(X)$. The projector $p'$ of $T(X) \otimes \mathbf{C}$ onto $T'(X)$ is equal to $\frac{1}{2}(1 - ij)$; the projector $p'' = 1 - p'$ of $T(X) \otimes \mathbf{C}$ onto $T''(X)$ is equal to $\frac{1}{2}(1 + ij)$. The composites
$$
\pi': \quad T(X) \to T(X) \otimes \mathbf{C} \xrightarrow{p'} T'(X)
$$
$$
\pi'': \quad T(X) \to T(X) \otimes \mathbf{C} \xrightarrow{p''} T''(X)
$$
are $\mathbf{R}$-isomorphisms; the first transforms $j$ into multiplication by $i$, the second into multiplication by $-i$.

8.8.4 (“Forms of type $(p, q)$”). Retain the hypotheses and notations of the preceding no. Let $F$ be a complex vector bundle with base $X$, let $p$ and $q$ be two integers $\geqslant 0$, and let $n = p + q$. Let $\omega$ be a differential form of degree $n$ on an open set $U$ of $X$, with values in $F$; identify (8.8.2) $\omega$ with a section of $\mathrm{Alt}_c^n(T(X) \otimes \mathbf{C}; F)$. We say that $\omega$ is *of type* $(p, q)$ if, for every $x \in U$, one has
$$
\omega_x(v_1, \ldots, v_n) = 0
$$
as soon as $p + 1$ of the vectors $v_i$ belong to $T'_x(X)$ or $q + 1$ of the vectors $v_i$ belong to $T''_x(X)$. If one identifies $\bigwedge^n T_x(X) \otimes \mathbf{C}$ with the direct sum of the spaces $\bigwedge^{m'} T'_x(X) \otimes \bigwedge^{m''} T''_x(X)$ for $m' + m'' = n$ (A, III, p. 85) and $\omega_x$ with a $\mathbf{C}$-linear form on $\bigwedge^n T_x(X)$, it amounts to saying that $\omega_x$ is zero on $\bigwedge^{m'} T'_x(X) \otimes \bigwedge^{m''} T''_x(X)$ for $(m', m'') \neq (p, q)$.

For every pair $(p, q)$ of integers $\geqslant 0$ with $p + q = n$, there exists one and only one complex vector subbundle $\mathrm{Alt}^{p,q}(T(X); F)$ of $\mathrm{Alt}^n(T(X); F)$ such that its sections on an open set $U$ of $X$ are the differential forms of type $(p, q)$ on $X$, with values in $F$. The vector bundle $\mathrm{Alt}^n(T(X); F)$ is the direct sum of the vector bundles $\mathrm{Alt}^{p,q}(T(X); F)$ for $p \geqslant 0,\ q \geqslant 0$ and $p + q = n$. Every differential form $\omega$ of degree $n$ with values in $F$ decomposes uniquely into
$$
\omega = \sum_{p+q=n} \omega_{p,q}
$$
where $\omega_{p,q}$ is a form of type $(p, q)$, called the *component of type* $(p, q)$ of $\omega$. If $\omega$ is of class $\mathbf{C}^h$, with $0 \leq h \leq k$, the same is true of its components.

*Examples*

(a) A differential form of degree $n$ is of type $(n, 0)$ if and only if it is $\mathbf{C}$-multilinear.

(b) Let $F', F''$ and $F$ be three complex vector bundles and let $F' \times_X F'' \to F$ be a $\mathbf{C}$-bilinear pairing. If $\omega'$ (resp. $\omega''$) is a differential form of type $(p', q')$ (resp. $(p'', q'')$) with values in $F'$ (resp. $F''$), the differential form $\omega' \wedge \omega''$ is of type $(p' + p'', q' + q'')$.

(c) Suppose that $F$ is the complexification of a (real) vector bundle (8.8.2). If $\omega$ is a differential form of type $(p, q)$ with values in $F$, its conjugate $\overline{\omega}$ (8.8.2) is of type $(q, p)$.

8.8.5. In addition to the preceding hypotheses, suppose that $k \geqslant 1$. The following three conditions are then equivalent:

(i) For every open set U of X and for every pair $(\xi, \eta)$ of complex vector fields on U, of class $C^k$, such that $\xi(x)$ and $\eta(x)$ belong to $T'_x(X)$ for every $x \in U$, one has $[\xi, \eta](x) \in T'_x(X)$ for every $x \in U$.

(ii) For every open set U of X and every pair $(\xi, \eta)$ of (real) vector fields on U, of class $C^k$, one has
$$
[\xi, \eta] + j[j\xi, \eta] + j[\xi, j\eta] - [j\xi, j\eta] = 0.
$$

(iii) For every open set U of X and for every complex differential form $\omega$ of type $(1, 0)$ on U, of class $C^k$, the component of type $(0, 2)$ of $d\omega$ is zero.

Suppose that these conditions are satisfied. Let $\omega$ be a differential form of type $(p, q)$ on an open set U of X, of class $C^h$ with $1 \leq h \leq k$, with values in a complex Banach space F. We denote by $d'\omega$ (resp. $d''\omega$) the component of type $(p+1, q)$ (resp. $(p, q+1)$) of $d\omega$; the other components of $d\omega$ are then zero and we have
$$
d\omega = d'\omega + d''\omega.
$$
If $k \geq 2$, we have
$$
d'(d'\omega) = 0 \quad , \quad d''(d''\omega) = 0 \quad , \quad d'(d''\omega) + d''(d'\omega) = 0.
$$
With the notation of 8.8.4, example b), we have
$$
d'(\omega' \wedge \omega'') = d'(\omega') \wedge \omega'' + (-1)^{p'+q'} \omega' \wedge d'(\omega'')
$$
$$
d''(\omega' \wedge \omega'') = d''(\omega') \wedge \omega'' + (-1)^{p'+q'} \omega' \wedge d''(\omega'').
$$
With that of 8.8.4, example c), we have
$$
d'(\overline{\omega}) = \overline{d''(\omega)}.
$$
In formulas (4) and (5) (resp. (6)), the differential forms $\omega'$ and $\omega''$ (resp. $\omega$) are assumed to be of class $C^1$.

8.8.6 (« Almost complex structure of a complex manifold »). Let $X^c$ be a complex analytic manifold, having X as underlying real analytic manifold (5.14.2.a)). The bundle $T(X)$ is identified with the underlying (real) vector bundle of the complex vector bundle $T(X^c)$, which endows X with an almost complex structure of class $C^\omega$, said to be defined by the complex analytic manifold structure given on X. This almost complex structure satisfies conditions (i) to (iii) of 8.8.5; in particular, the operators $d'$ and $d''$ of 8.8.5 are defined. If $f : X^c \to Y^c$ is a morphism of complex analytic manifolds, $f^*$ commutes with the operators $d'$ and $d''$.

8.8.7. Retain the hypotheses and notations of 8.8.6. Let $\overline{X}^c$ be the conjugate of $X^c$ (5.14.2.b)). Embed X by the diagonal mapping $x \mapsto (x, x)$ in the complex manifold $X^c \times \overline{X}^c$, and let g be the anti-automorphism $(x, y) \mapsto (y, x)$ of $X^c \times \overline{X}^c$. The pair $(X^c \times \overline{X}^c, g)$ is a *complexification* of X (5.14.8). In particular, for every $x \in X$, the tangent space $T_x(X^c \times \overline{X}^c)$ is identified with $T_x(X) \otimes \mathbf{C}$; under this identification, $T_x(X^c \times \{x\})$ corresponds to $T'_x(X)$ and $T_x(\{x\} \times \overline{X}^c)$ corresponds to $T''_x(X)$.

8.8.8. Suppose $r = \omega$; every almost complex structure of class $C^\omega$ on $X$ satisfying the equivalent conditions (i) to (iii) of 8.8.5 is the almost complex structure defined by one and only one complex analytic manifold structure on $X$.¹

8.8.9 (« Holomorphic forms »). Let us take up the hypotheses and notations of 8.8.6, and let $F$ be a complex Banach space. Morphic (in other words complex analytic) differential forms on $X^c$, with values in $F$, are also called *holomorphic* differential forms; the identification of $T(X^c)$ with $T(X)$ identifies them with (real analytic) differential forms on $X$. For a differential form $\omega$ of degree $p$ on $X$, with values in $F$ and of class $C^k$ with $k \geqslant 1$, to be holomorphic, it is necessary and sufficient that it be of type $(p, 0)$ and that $d''\omega = 0$.

Let $\xi$ be a vector field on $X$. We say that $\xi$ is *holomorphic* if it is a complex analytic mapping of $X^c$ into $T(X^c) = T(X)$, in other words a complex analytic vector field on $X^c$. If this is the case, and if $\omega$ is a holomorphic differential form on $X$ with values in $F$, the form $\theta_\xi.\omega$ (resp. $i(\xi)\omega$) is the same, whether we consider $\xi$ as a complex analytic vector field on $X^c$ and $\omega$ as an element of $\Omega^p(X^c; F)$, or $\xi$ as a vector field on $X$ and $\omega$ as an element of $\Omega^p(X; F)$. Moreover, let $\xi' = \pi'(\xi)$ and $\xi'' = \pi''(\xi)$ be the components of $\xi$ in $T'(X)$ and $T''(X)$ respectively (8.8.3); we have

$$
\theta_\xi.\omega = \theta_{\xi'}.\omega \quad , \quad \theta_{\xi''}.\omega = 0 \tag{7}
$$
$$
i(\xi)\omega = i(\xi')\omega \quad , \quad i(\xi'')\omega = 0. \tag{8}
$$

8.8.10. *Example.* — Suppose that $X^c$ is an open set in $\mathbf{C}^n$ and denote by $z^1, \ldots, z^n$ the coordinate functions on $X^c$. For $1 \leqslant k \leqslant n$, put $z^k = x^k + iy^k$, where $x^k$ and $y^k$ are real-valued. Consider the tangent frame $(\partial/\partial z^k)$ of $T(X^c)$ defined by the coordinate system $(z^k)$ and the tangent frame $(\partial/\partial x^k, \partial/\partial y^k)$ of $T(X)$ defined by the coordinate system $(x^k, y^k)$ (8.1.5). We have $j(\partial/\partial x^k) = \partial/\partial y^k$ and the image of $\partial/\partial z^k$ by the mapping $\pi': T(X) = T(X^c) \to T'(X)$ (8.8.3) is equal to
$$
\frac{1}{2}(\partial/\partial x^k - i \partial/\partial y^k);
$$
we shall still denote it in general by $\partial/\partial z^k$.² The complex conjugate vector field of this field $\partial/\partial z^k$ is denoted by $\partial/\partial \bar{z}^k$; we have
$$
\partial/\partial \bar{z}^k = \frac{1}{2}(\partial/\partial x^k + i \partial/\partial y^k). \tag{9}
$$

If $f$ is a function of class $C^1$ on $X$, with values in a complex Banach space $F$, the differential forms $d'f$ and $d''f$ (8.8.5) are given by
$$
d'f = \sum_{1 \leqslant k \leqslant n} \frac{\partial f}{\partial z^k} \, dz^k \quad , \quad d''f = \sum_{1 \leqslant k \leqslant n} \frac{\partial f}{\partial \bar{z}^k} \, d\bar{z}^k. \tag{10}
$$

¹ If $X$ is finite-dimensional, this remains true for an almost complex structure of class $C^k$ with $k \geqslant \dim X$ (cf. A. NEWLANDER and L. NIRENBERG, *Complex analytic coordinates in almost complex manifolds*, Ann. of Math. LXV (1957), p. 391–404).
² Care must be taken that the canonical identification of $T(X^c)$ with $T(X)$ does not transform the vector field $\partial/\partial z^k$ on $X^c$ into the vector field $\partial/\partial z^k$ on $X$, but into the vector field $\partial/\partial z^k + \partial/\partial \bar{z}^k$. However, the two vector fields denoted by $\partial/\partial z^k$ take the same value on holomorphic differential forms (8.8.9), which are moreover the only forms to which a vector field of $X^c$ can be applied.

Let us recall that we have

$$
df = d'f + d''f
$$

$$
dz^k = dx^k + i\ dy^k \qquad d\bar{z}^k = dx^k - i\ dy^k.
$$

If $A = (i_1, \ldots, i_p)$ is a strictly increasing sequence of integers belonging to the interval $[1, n]$, put

$$
dz^A = dz^{i_1} \wedge \cdots \wedge dz^{i_p}
$$

and denote by $d\bar{z}^A$ the conjugate of $dz^A$. Every differential form $\omega$ of type $(p, q)$ with values in $F$ can be written uniquely

(11)
$$
\omega = \sum_{A, B} f_{A, B}\ dz^A \wedge d\bar{z}^B
$$

where $A$ (resp. $B$) runs through the set of strictly increasing sequences of $p$ (resp. $q$) elements of $[1, n]$, the $f_{A, B}$ being functions with values in $F$. If $\omega$ is of class $C^k$, with $k \geqslant 1$, the same is true of the functions $f_{A, B}$ and we have

(12)
$$
d'\omega = \sum_{A, B} d'f_{A, B} \wedge dz^A \wedge d\bar{z}^B
$$

(13)
$$
d''\omega = \sum_{A, B} d''f_{A, B} \wedge dz^A \wedge d\bar{z}^B.
$$

[^1]: When $K=\mathbf{R}$ and $r=1$, $T(X)$ is a topological vector bundle (cf. Notations and conventions).
