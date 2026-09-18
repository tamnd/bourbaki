---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 11
section_title: Formule de Stokes
lang: en
source: var-fr
pdf_pages: 0136-0142
extraction: ocr
subsections:
    - "no": 1
      title: Pièces
      page: 0
      pdf_page: 136
    - "no": 2
      title: Formule de Stokes pour les pièces
      page: 0
      pdf_page: 137
    - "no": 3
      title: Formule de Stokes pour les ensembles localement polyédraux[^1]
      page: 0
      pdf_page: 138
    - "no": 4
      title: Formule de Stokes relative (intégration sur les fibres)
      page: 0
      pdf_page: 139
statements: 1
exercises: 0
content_sha256: dd75a45f272b35f901b1a2d1405444b8385e25ecaa6feb881fa35299d399d447
translated_from: content/fr/var/2/11_s11_formule_de_stokes.md
source_lang: fr
translation_method: machine
source_content_sha256: f1165c8a6f12721343d74c911068a2aca50a9171ac61b24075e228a251000002
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-f61888af
glossary_version: 34
glossary_terms_sha256: 487971cdc27f798e1f403179fd7e75714e64cc0a73b358dbc8807c7a8a596ecf
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 11. Stokes Formula

In this paragraph, we suppose $\mathbf{K}=\mathbf{R}$.

### 11.1. Pieces

### 11.1.1. Let E be a Banach space. A subset S of E is called a closed half-space if there exists a continuous linear form $h\neq 0$ and a real number $k$ such that $S=\{x|h(x)\leq k\}$ (cf. EVT, II, § 2, No. 6); the boundary of S is then the closed hyperplane $\{x|h(x)=k\}$; it is also called the boundary of S, and is denoted by $\partial S$.

### 11.1.2. Let X be a variety of class $C^r$ and A a subset of X. We say that A is a piece of X if, for every $a\in A$, there exists a chart $c=(U,\varphi,E)$ of X at a such that $\varphi(A\cap U)$ is an open set of a closed half-space of E. We put $\partial A=A-\mathring{A}$ (set of non-interior points of A). This is a subvariety of A, which is called the boundary of A.[^1] If $a\in\partial A$, there exists a chart $c=(U,\varphi,E)$ of X centred at a and a closed hyperplane H of E such that $\varphi(A\cap U)$ is an open neighbourhood of 0 in one of the closed half-spaces $S_c$ of E defined by H (EVT, II, § 2, No. 6), and such that $\varphi(\partial A\cap U)=H\cap\varphi(A\cap U)$. Such a chart is said to be adapted to A at a. The closed half-space $S_c$ is then the unique closed half-space of E of which $\varphi(A\cap U)$ is an open set.

For a closed subset A of X to be a piece of X, it is necessary and sufficient that $\mathring{A}$ be dense in A and that $A-\mathring{A}$ be a subvariety of X of codimension 1 at each of its points.

### 11.1.3. Examples

a) In $\mathbf{R}^n$, a closed ball of radius $>0$ is a piece; its boundary is the corresponding sphere.

b) If A is a piece of the variety X and B is a closed subset of $\partial A$, then $A-B$ is a piece of X.

c) Let $\varphi:X\rightarrow X'$ be a morphism of varieties of class $C^r$, and let $A'$ be a piece of $X'$. If $\varphi$ is transverse to $\partial A'$ (5.11.6), $\varphi^{-1}(A')$ is a piece of X whose boundary is $\varphi^{-1}(\partial A')$.

In particular, let $h : X \to \mathbf{R}$ be a function of class $C^r$, and let $a \in \mathbf{R}$; suppose that there is no $x \in X$ such that $h(x) = a$ and $d_x h = 0$. The set $\{ x | h(x) \leq a \}$ is a closed piece of $X$ with boundary $h^{-1}(a)$.

d) If $r = \infty$ and if $X$ is locally compact, every compact subset of $X$ admits a fundamental system of neighbourhoods consisting of compact pieces.

11.1.4. Let $X$ be a $C^r$-class manifold and $A$ a piece of $X$. Let $a \in \partial A$ and $v \in T_a(X)$. Let $c = (U, \varphi, E)$ be a chart of $X$ adapted to $A$ at $a$ (11.1.2) and let $h = \theta_c^{-1}(v)$ be the element of $E$ corresponding to $v$ (5.5.1). Let $S_c$ be the closed half-space of $E$ of which $\varphi(A \cap U)$ is an open set (11.1.2). We say that $v$ is an *inward vector* (resp. *strictly inward*, resp. *outward*, resp. *strictly outward*) for $A$ at $a$ if $h$ belongs to $S_c$ (resp. $\dot{S}_c, -S_c, -\dot{S}_c$), a condition which is independent of the choice of the adapted chart $c$. We denote by $T_a^+(A)$ (resp. $T_a^-(A)$) the set of outward (resp. inward) vectors of $T_a(X)$ for $A$. These are closed half-spaces of $T_a(X)$, whose boundary contains 0. We have
$$
T_a(\partial A) = T_a^+(A) \cap T_a^-(A).
$$

**11.2. Stokes formula for pieces**

In this No., let $X$ be a separated, pure $C^r$-class manifold ($r \geq 2$) of finite dimension $n$. Let $A$ be a piece of $X$ and $i$ the canonical injection of $\partial A$ into $X$. Let $E$ be a Banach space.

### 11.2. Stokes formula for pieces

11.2.1. Let $x \in \partial A$ and let $\xi$ be an orientation of $T_x(\partial A)$; we denote by $\tilde{i}_x(\xi)$ the orientation of $T_x(X)$ containing the elements $v \wedge u$, where $v$ is a vector strictly outward for $A$ at $x$ (11.1.4) and where $u$ is a nonzero element of $\wedge^{n-1} T_x(\partial A)$ belonging to the orientation $\xi$. The mapping $\tilde{i}_x$ is a bijection of $\mathrm{Or}(T_x(\partial A))$ onto $\mathrm{Or}(T_x(X))$. The mappings $\tilde{i}_x$ for $x \in \partial A$, define a morphism $\tilde{i} : \tilde{\partial A} \to \tilde{X}$ which is an *orientation* of $i$ (10.2.5). If $\xi$ is an orientation of $X$, the orientation of $\partial A$ associated with $\xi$ by $\tilde{i}$ (10.2.5) is said to be *defined by* $\xi$.

#### Example {#var-2-s11-n2-exa-1 .statement}

When $X = \mathbf{R}^n$, $\xi$ is the usual orientation of $\mathbf{R}^n$ and $A$ is a closed ball of radius $> 0$, the orientation of the sphere $\partial A$ defined by $\xi$ is the canonical orientation (10.2.8, b)).

11.2.2. Let $\omega$ be a twisted differential form of degree $p$ on $X$ with values in $E$ (10.4.1); the inverse image $i^*(\omega)$ of $\omega$ by the oriented morphism $i : \partial A \to X$ is denoted by $\omega|_{\partial A}$ and is called the *form induced by* $\omega$ *on* $\partial A$ (cf. 10.4.3).

11.2.3. Let us make one of the following two hypotheses:

(i) $\omega$ is a twisted differential form of degree $n-1$ on $X$, with values in $E$;
(ii) $X$ is oriented, $\partial A$ is provided with the corresponding orientation (11.2.1) and $\omega$ is a differential form of degree $n-1$ on $X$ with values in $E$.

Suppose in addition that $\omega$ is *of class* $C^1$ and that the intersection of $A$ and the support of $\omega$ is compact. The exterior differential $d\omega$ of $\omega$ is continuous (8.3.5 and 10.3.4).

The characteristic function of $A$ is essentially integrable for the vector measure defined by $d\omega$ on $X$ and the differential form $\omega|_{\partial A}$ of degree $n - 1$ on $\partial A$ is integrable (10.4.3 and 10.4.4). One has
$$
\int_A d\omega = \int_{\partial A} \omega \quad \text{(« Stokes formula »)}.
$$
11.2.4. Let $\alpha$ be a twisted differential form of degree $n$ on $X$ with values in $E$, with compact support, and of class $C^1$. In order that there exist a twisted differential form $\omega$ of degree $n - 1$ on $X$, with values in $E$, with compact support and of class $C^1$, such that $\alpha = d\omega$, it is necessary that $\int_X \alpha = 0$; if $X$ is connected, this condition is sufficient; if in addition $\alpha$ is of class $C^k$ ($k \leq r - 1, k \neq \omega$), one can choose $\omega$ of class $C^k$.

11.2.5. Suppose that $X$ is the real variety underlying $\mathbf{C}$, that $E$ is a complex Banach space and that $A$ is a *compact* piece of $X$. Equip $X$ with the orientation defined by its complex structure (10.2.7). Let $f$ be a *continuous* mapping from $A$ into $E$ whose restriction to the interior $\mathring{A}$ of $A$ is holomorphic. Let $dz$ denote the differential of the injection $z : \partial A \to \mathbf{C}$. The form $f.dz$, product of $f$ and $dz$, is a differential form of degree 1 on $\partial A$, with values in $E$, of class $C^0$, and one has:
$$
\int_{\partial A} f.dz = 0 \quad \text{(« Cauchy formula »)}.
$$
When $f$ extends to a holomorphic mapping, still denoted $f$, of an open neighbourhood $U$ of $A$, with values in $E$, the differential form $f.dz$ (where $z$ denotes this time the canonical injection of $U$ into $\mathbf{C}$) is of class $C^\infty$ on $U$ and its exterior differential is zero.

11.2.6 (*Derivative of an integral*). Suppose $X$ is oriented. Let $Y$ be a variety of class $C^r$, and let $\alpha$ be a differential form of degree $n$ on $Y$, with values in $E$, of class $C^1$, and with compact support. Let $I$ be an open subset of $\mathbf{R}$ containing 0 and let $g : I \times X \to Y$ be a morphism of class $C^r$; for $t \in I$, denote by $g_t$ the mapping $x \mapsto g(t, x)$ from $X$ into $Y$. Denote by $\psi$ the morphism from $X$ into $T(Y)$ defined by $\psi(x) = T_{(0, x)}(g)(1, 0)$; it is a *lifting* of $g_0$ (8.6.5). Suppose that the restriction of $\mathrm{pr}_1 : I \times A \to I$ to the intersection of $I \times A$ and the support of $g^*(\alpha)$ is *proper* (TG, I, § 10). For every $t \in I$, the intersection of $A$ and the support of $g_t^*(\alpha)$ is then compact; the mapping $t \mapsto \int_A g_t^*(\alpha)$ is of class $C^1$ on $I$ and its derivative at the origin is given by the formula
$$
\frac{d}{dt} \left( \int_A g_t^*(\alpha) \right)_{t=0} = \int_A \theta_\psi \cdot \alpha = \int_A i(\psi) \, d\alpha + \int_{\partial A} i(\psi) \, \alpha,
$$
cf. No. 8.6.

### 11.3. Stokes formula for locally polyhedral sets[^2]

In this No., $X$ denotes a real purely finite-dimensional variety of class $C^r$ ($r \geq 2$); we suppose $X$ separated.

11.3.1. Let $A$ be a subset of a real finite-dimensional vector space. We say that $A$ is polyhedral if it is a finite union of finite intersections of closed half-spaces. A subset $A$ of $X$ is said to be locally polyhedral if, for every $x\in X$, there exists a chart $c=(U,\varphi,E)$ of $X$ at $x$ and a polyhedral subset $A_c$ of $E$ such that $\varphi(A\cap U)=\varphi(U)\cap A_c$. A piece of $X$ is a locally polyhedral subset.

11.3.2. Let $A$ be a closed subset of $X$, and let $\operatorname{Fr}(A)=A-\mathring{A}$ be its frontier. A point $x\in\operatorname{Fr}(A)$ is said to be regular if there exists an open neighbourhood $U$ of $x$ such that $A\cap U$ is a piece of the manifold $U$ (in which case $x$ belongs to the boundary of $A\cap U$). We denote by $\partial A$ the set of regular points of $\operatorname{Fr}(A)$ and call it the regular boundary (or simply the boundary) of $A$. The set $A'=\mathring{A}\cup\partial A$ is a piece of $X$, with boundary $\partial A$.

11.3.3. *\** **Example.** — Let $\mathscr{H}$ be a locally finite set of hyperplanes of a finite-dimensional real affine space $E$, and let $C$ be a chamber of $E$ with respect to $\mathscr{H}$ (LIE, V, § 1, No. 3). The closure $\overline{C}$ of $C$ is a locally polyhedral subset of the manifold $E$; the regular boundary of $\overline{C}$ is the union of the faces of $C$ (loc. cit., No. 4). In particular, if $C$ is an open simplex (loc. cit., No. 6) with vertices $a_0,\ldots,a_n$, the boundary of $\overline{C}$ is the union of the $C_{(i)}$ ($0\leq i\leq n$), where $C_{(i)}$ is the open simplex with vertices $a_0,\ldots,a_{i-1},a_{i+1},\ldots,a_n$ in the affine space generated by these vertices.*\*

11.3.4. Let $A$ be a locally polyhedral subset of $X$, and let $\omega$ be a twisted differential form of degree $n-1$ on $X$ with values in a Banach space $E$; suppose that $\omega$ is of class $C^1$ and that the intersection of its support with $A$ is compact. Then the characteristic function of $A$ (resp. $A'$, $\hat{A}$) is essentially integrable for the vector measure defined by $d\omega$ on $X$ and one has

$$
\int_A d\omega=\int_{A'}d\omega=\int_{\hat{A}}d\omega.
$$

The differential form $\omega|\partial A$ (for the canonical orientation of the canonical injection of $\partial A$, considered as the boundary of the piece $A'$, into $X$) is integrable in $\partial A$ and one has

$$
\int_A d\omega=\int_{\partial A}\omega
\qquad\text{(« Stokes formula »).}
$$

When $X$ is provided with an orientation, and $\partial A$ is provided with the corresponding orientation (11.2.1), this formula is still valid if $\omega$ is an ordinary differential form of degree $n-1$ with values in $E$, of class $C^1$ and such that $A\cap\operatorname{Supp}\omega$ is compact.

### 11.4. Relative Stokes formula (integration over the fibres)

In this number, let $X$ and $S$ be two (real) manifolds of class $C^r$ and let $\pi:X\to S$ be a submersion. Let $n$ be an integer and suppose that, for every $s\in S$, the fibre $X_s=\pi^{-1}(s)$ of $\pi$ at $s$ (which is a submanifold of $X$ (5.10.5)) is purely of dimension $n$.

4—B.

11.4.1. Let E and H be two vector spaces and let F be a finite-dimensional vector subspace of dimension n of H. Let p be an integer $\geqslant 0$, let u be an alternating $(n + p)$-linear mapping of $H^{n+p}$ into E and let $t_1, \ldots, t_p$ be elements of H/F; let $t'_1, \ldots, t'_p$ be representatives of $t_1, \ldots, t_p$ in H. The mapping

$$
(x_1, \ldots, x_n) \mapsto u(t'_1, \ldots, t'_p, x_1, \ldots, x_n)
$$

is an alternating $n$-linear mapping of $F^n$ into E, which depends only on u and the $t_i$; it is denoted by $u \perp (t_1, \ldots, t_p)$ (cf. A, III, p. 158 for the particular case $E = K$). The mapping

$$
(t_1, \ldots, t_p) \mapsto u \perp (t_1, \ldots, t_p)
$$

is alternating $p$-linear.

11.4.2 (« $\pi$-torsion »). Consider the vector bundle T(X/S) on X (8.1.3); it is of finite rank n at every point of X. Put $\tilde{R}_\pi = \tilde{R}_{T(X/S)}$ (10.3.1) and $\tilde{X}_\pi = \mathrm{Or}_{T(X/S)}$ (10.2.2). Let $s \in S$; in view of the natural identification of $T(X/S)|_{X_s}$ with $T(X_s)$ (8.1.3), the fibre at s of the mapping $\tilde{\pi}: \tilde{X}_\pi \to S$ composed of $\pi$ and the canonical mapping $\tilde{X}_\pi \to X$, is $\tilde{X}_s$ (10.2.4). A differential form $\pi$-twisted on X is called a $T(X/S)$-twisted differential form (10.3.3).

11.4.3 (« S-orientation of an S-morphism »). Let $X'$ be a manifold provided with a submersion $\pi': X' \to S$ whose fibres $X_s$ are purely of finite dimension $n'$, and let $\varphi: X' \to X$ be a morphism such that $\pi' = \pi \circ \varphi$. An S-orientation of $\varphi$ is called a morphism $\tilde{\varphi}: \tilde{X}'_\pi \to \tilde{X}_\pi$, commuting with the action of the group $\{ \pm 1 \}$ and such that the diagram

$$
\begin{array}{ccc}
\tilde{X}'_\pi & \xrightarrow{\tilde{\varphi}} & \tilde{X}_\pi \\
| & & | \\
X' & \xrightarrow{\varphi} & X
\end{array}
$$

is commutative. The data of an S-orientation of $\varphi$ makes it possible, as in 10.4.2, to identify the bundles $\tilde{R}_{\pi'}$ and $\varphi^*(\tilde{R}_\pi)$ and to define the inverse image of a $\pi$-twisted differential form by the S-oriented morphism $\varphi$: it is a $\pi'$-twisted differential form on $X'$.

11.4.4. Let A be a piece of X such that the restriction of $\pi$ to $\partial A$ is a submersion. For every $s \in S$, the fibre $X_s = \pi^{-1}(s)$ is a submanifold of X transverse to $\partial A$ and $A \cap X_s$ is a piece of $X_s$, denoted by $A_s$, with boundary $\partial A \cap X_s$.

Let i be the canonical injection of $\partial A$ into X. There exists one and only one S-orientation $\tilde{i}$ of i such that, for every $s \in S$, the restriction of $\tilde{i}$ to $(\partial A_s)^*$ (identified with the fibre at s of the submersion $\partial \tilde{A}_{\pi|\partial A} \to S$) is the orientation defined in 11.2.1 of the canonical injection of $\partial A_s$ into $X_s$. If $\omega$ is a $\pi$-twisted differential form on X, the inverse image of $\omega$ by the morphism i thus oriented is denoted by $\omega|\partial A$ (cf. 11.2.2).

11.4.5 (« Interior product »). Let $p$ be an integer $\geqslant 0$ and let $\omega$ be an $n$-twisted differential form of degree $n + p$ on $X$, with values in a vector bundle $E$ with base $X$. Let $s \in S$ and $x \in X_s$; we have $\omega(x) = \xi \otimes u$, where $\xi$ is an orientation of $T_x(X_s) = T(X/S)_x$, identified with an element of $(\tilde{R}_{X_s})_x = (\tilde{R}_\pi)_x$ (10.3.2), and where $u$ is an alternating $(n + p)$-linear mapping of $T_x(X)$ into $E_x$. Let $t_1, \ldots, t_p$ be tangent vectors to $S$ at $s$. Put

$$
\theta(x) = \xi \otimes (u \wedge (t_1, \ldots, t_p)) \in (\tilde{R}_{X_s})_x \otimes (\mathrm{Alt}^n(T(X); E))_x
$$

(cf. 11.4.1). This defines a twisted differential form $\theta : x \mapsto \theta(x)$ of degree $n$ on $X_s$, with values in $E|X_s$. We denote it by $\omega \wedge (t_1, \ldots, t_p)$.

In particular, let $M$ be a vector bundle of class $C^{r-1}$ over $S$ and take $E = \pi^*(M)$. The bundle $E|X_s$ is naturally identified with the trivial bundle over $X_s$ defined by the Banach space $M_s$, and the form $\omega \wedge (t_1, \ldots, t_p)$ is identified with a twisted differential form on $X_s$, with values in $M_s$.

11.4.6. Retain the preceding notation (in particular $E = \pi(*M)$) and suppose in addition that $X$ is separated and $\omega$ continuous. Let $A$ be a piece of $X$ such that the restriction of $\pi$ to $\partial A$ is a submersion and the restriction of $\pi$ to the intersection of $A$ and the support of $\omega$ is proper. For $s \in S$ and $t_1, \ldots, t_p$ in $T_s(S)$, the form $\omega \wedge (t_1, \ldots, t_p)$ (11.4.5) is a continuous twisted differential form of degree $n$ on $X_s$, with values in the Banach space $M_s$, and its support meets $A_s$ in a compact set. There exists one and only one differential form $\alpha$ of degree $p$ on $S$, with values in the vector bundle $M$, such that

$$
\alpha(s)(t_1, \ldots, t_p) = \int_{A_s} \omega \wedge (t_1, \ldots, t_p)
$$

for all $s \in S$ and $t_1, \ldots, t_p$ in $T_s(S)$. The form $\alpha$ is denoted by $\int_{\pi|A} \omega$ (or simply $\int_\pi \omega$ when $A = X$); it is said to be obtained by integrating $\omega$ over $A$ along the fibres of $\pi$. If $\omega$ is of class $C^k$ ($0 \leq k \leq r - 1, k \leq \infty$), the same is true of $\int_{\pi|A} \omega$.

When $\omega$ is a form of degree $< n$, we agree that $\int_{\pi|A} \omega = 0$.

11.4.7. Retain the preceding hypotheses and notation.

a) For every continuous scalar differential form $\beta$ on $S$, we have

$$
\int_{\pi|A} (\pi^*\beta) \wedge \omega = \beta \wedge \int_{\pi|A} \omega.
$$

b) Let $\eta$ be a continuous vector field on $X$ and $\zeta$ a continuous vector field on $S$, such that $\eta$ is $\pi$-related to $\zeta$ (8.2.6). We have

$$
i(\zeta) \int_{\pi|A} \omega = \int_{\pi|A} i(\eta)\omega.
$$

c) Suppose in addition that $\eta, \zeta$ and $\omega$ are of class $C^1$, that $\eta(x) \in T_x(\partial A)$ for all $x \in \partial A$ and that $M$ is the trivial vector bundle defined by a Banach space $E$. We have

$$
\theta_\zeta \cdot \int_{\pi|A} \omega = \int_{\pi|A} \theta_\eta \cdot \omega,
$$

(cf. 8.4.2 and 10.3.4).

d) If $\omega$ is of degree $n + p$ and of class $C^1$, we have
$$
d \left( \int_{\pi|A} \omega \right) = \int_{\pi|A} d\omega + (-1)^p \int_{\pi|\partial A} \omega|_{\partial A}.
$$
e) Suppose that S is reduced to a point. The $\pi$-twisted forms on X are then the ordinary twisted forms (10.4.1). If $\omega$ is of degree $n$, the form $\int_{\pi|A} \omega$ of degree 0 on S is the constant $\int_A \omega$ (10.4.3).

11.4.8. Let $\pi': S \to S'$ be a submersion such that the fibres of $\pi'$ are pure submanifolds of constant finite dimension $n'$. Put $\pi'' = \pi' \circ \pi$; it is a submersion of X onto S' whose fibres are pure submanifolds of dimension $m = n + n'$.

Let $x \in X$. The sequence
$$
0 \longrightarrow T(X/S)_x \xrightarrow{\mathrm{Id}} T(X/S')_x \xrightarrow{T_x(\pi)} T(S/S')_{\pi(x)} \longrightarrow 0
$$
is exact. There exists one and only one isomorphism $j$ of the vector bundle $\tilde{R}_{\pi} \otimes \pi^*(\tilde{R}_{\pi'})$ onto $\tilde{R}_{\pi''}$ such that, if $\xi$ (resp. $\eta$) is an orientation of $T(X/S)_x$ (resp. of $(\pi^*T(S/S'))_x$) identified with $T(S/S')_{\pi(x)}$, we have $j(\xi \otimes \eta) = \eta \xi$ (the product being defined by the preceding exact sequence (10.2.1)).

Let $M'$ be a vector bundle with base $S'$; put $M = {\pi'}^*(M')$, and $E = \pi^*(M) = {\pi''}^*(M')$. If $\omega$ is a $\pi''$-twisted differential form on X with values in E, the isomorphism $j$ allows it to be identified with a $\pi$-twisted form with values in $\pi^*(\tilde{R}_{\pi'}) \otimes E$, or equivalently with values in $\pi^*(\tilde{R}_{\pi'} \otimes M)$.

Soit de plus A une pièce de X telle que $\pi|\partial A : \partial A \to S$ soit une submersion ; the same then holds for $\pi''|\partial A : \partial A \to S'$. Suppose in addition that $\omega$ is continuous and that the restriction of $\pi''$ to $A \cap \operatorname{Supp} \omega$ is proper; the same then holds for the restriction of $\pi$ to $A \cap \operatorname{Supp} \omega$. One can consider on the one hand the differential form $\int_{\pi''|A} \omega$ on $S'$, which is a form with values in $M'$, and on the other hand the differential form $\int_{\pi|A} \omega$ on S, which is a form with values in $\tilde{R}_{\pi'} \otimes M$, or equivalently a $\pi'-$twisted form with values in $M = {\pi'}^*(M')$. Moreover, $\pi(A)$ is an open submanifold of S and the restriction of $\pi'$ to $\pi(A) \cap \operatorname{Supp} \int_{\pi|A} \omega$ is proper. The differential form $\int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega$ is defined; it is a differential form on $S'$, with values in $M'$. We have
$$
\int_{\pi' \circ \pi|A} \omega = \int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega.
$$
If $A = X$, we have
$$
\int_{\pi' \circ \pi} \omega = \int_{\pi'} \int_{\pi} \omega.
$$

[^1]: This terminology comes from the fact that A is naturally endowed with a structure of a “manifold with boundary”, with boundary $\partial A$. For the definition of this category, as well as for that, more generally, of the category of “manifolds with corners”, the reader may refer to H. CARTAN, Séminaire 1961/62, Topologie Différentielle, exposés 1-2-3 (par A. DOUADY), Benjamin, New York, 1969. Let us point out that one can show that every “manifold with boundary” whose boundary is paracompact is isomorphic to a closed piece of a manifold.
[^2]: The reader interested in more general cases may consult H. WHITNEY, Geometric Integration Theory, Chap. III, § 18 (Princeton Univ. Press, 1957).
