---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 10
section_title: Mesures définies par des formes différentielles
lang: en
source: var-fr
pdf_pages: 0126-0135
extraction: ocr
subsections:
    - "no": 1
      title: Mesure module d’une forme différentielle
      page: 0
      pdf_page: 126
    - "no": 2
      title: Orientations
      page: 0
      pdf_page: 128
    - "no": 3
      title: Formes différentielles M-tordues
      page: 0
      pdf_page: 131
    - "no": 4
      title: Mesure associée à une forme différentielle tordue
      page: 0
      pdf_page: 132
statements: 0
exercises: 0
content_sha256: 48948108d489270e2fea55f10b68791137abacd00a974022c223abd1f8be7413
translated_from: content/fr/var/2/10_s10_mesures_definies_par_des_formes.md
source_lang: fr
translation_method: machine
source_content_sha256: 0c1bcecfea38bc2fc1272b64c6d5313be25d53ad6f0919550db0761e5da947f0
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-en-mt-783309b2
glossary_version: 34
glossary_terms_sha256: 55d92649a5db8221400077d13b0b26259023fcf14e8b564bb673d1831210a6b3
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 10. Measures defined by differential forms

In this paragraph, it is assumed that $K$ is locally compact. Starting with No. 10.2, it is assumed that $K=\mathbf{R}$. In Nos. 10.1 and 10.4, all the varieties considered are assumed to be locally finite-dimensional; when they are separated, they are locally compact.

### 10.1. Module measure of a differential form

**Notations.** — We denote by $\mu$ a Haar measure (INT, VII, § 1, No. 2) on the additive group of $K$. We denote by $\mu^{\otimes n}$ the measure $\mu\otimes\cdots\otimes\mu$ on $K^n$ and by $\mu^{\otimes n}_U$ its restriction to an open subset $U$ of $K^n$. For $a\in K$, we denote by $\operatorname{mod}(a)$ the module of $a$ (INT, VII, § 1, No. 10 and AC, VI, § 9, No. 1). If $K=\mathbf{R}$, we have $\operatorname{mod}(a)=|a|$; if $K=\mathbf{C}$, we have $\operatorname{mod}(a)=|a|^2$; if $K$ is ultrametric, we have $\operatorname{mod}(a)=q^{-\nu(a)}$, where $q$ denotes the number of elements of the residue field of $K$ and $\nu$ the named valuation of $K$ (AC, VI, § 9, No. 1, prop. 1).

### 10.1.1. Let $U$ and $V$ be open subsets of $K^n$, and let $f:U\to V$ be a mapping of class $C^r$, with $r\in\mathbf{N}$. Let $x\in U$; the Jacobian of $f$ at $x$, denoted by $\operatorname{Jac}_x(f)$, is called the determinant of the linear mapping $Df(x)$ derived from $f$ at $x$. We denote by $\operatorname{Jac}(f)$ the function $x\mapsto\operatorname{Jac}_x(f)$; the function $\operatorname{mod}(\operatorname{Jac}(f))$ is a continuous function in $U$ with positive real values.

### 10.1.2 (« Change of variable in integrals »). Under the hypotheses of 10.1.1, suppose that $f$ is an isomorphism of class $C^r$ of the variety $U$ onto the variety $V$. Then the image by $f$ of the measure $\operatorname{mod}(\operatorname{Jac}(f))\mu^{\otimes n}_U$ is $\mu^{\otimes n}_V$; for every continuous function with compact support $\varphi:V\to\mathbf{C}$, we have

$$
\int_V \varphi(y)\mu^{\otimes n}(y)=\int_U \varphi(f(x)).\operatorname{mod}(\operatorname{Jac}_x(f))\mu^{\otimes n}(x).
$$

### 10.1.3. Let $X$ be a variety of class $C^r$, and let $A$ be a subset of $X$. We say that $A$ is locally negligible if, for every chart $(U,\varphi,K^n)$ of the variety $X$, the set $\varphi(A\cap U)$ is $\mu^{\otimes n}$-negligible (INT, IV, § 2, No. 2); this condition does not depend on the choice of $\mu$, and it is sufficient to verify it for a family of charts whose domains cover $A$. Every set contained in the union of a countable family of locally negligible sets is locally negligible.

Examples

a) Any subvariety of X which is of codimension $\geq 1$ at every point (i.e. of empty interior) is locally negligible.

b) Let g be a function of class $C^r$ on X, and let $A_g$ be the set of points $x \in X$ such that $g(x) = 0$; suppose that the interior of $A_g$ is empty, and that $r = \omega$; then $A_g$ is locally negligible.

c) Let $f : Y \to X$ be a morphism of varieties of class $C^r$, the variety Y being a countable union of compact subsets. Suppose that one has $\dim_y Y \leq \dim_{f(y)} X$ for every $y \in Y$. The image by $f$ of every locally negligible subset of Y is a locally negligible subset of X. The same is true of the image by $f$ of the set of points where $f$ is not étale ("first theorem of Sard"); in particular, if $\dim_y Y < \dim_{f(y)} X$ for every $y \in Y, f(Y)$ is a locally negligible subset of X.

d) Suppose that K is of characteristic zero. Let $f : Y \to X$ be a morphism of varieties of class $C^r$ ($r \in \mathbf{N}_K, r \geq \infty$), Y being a countable union of compact subsets. Let C be the set of points of Y where $f$ is not a submersion ("critical points"). Then $f(C)$ is a locally negligible subset of X ("second theorem of Sard").[^1]

10.1.4. Let X be a paracompact variety of class $C^r$. There exists on X a class M of equivalent measures (INT, V, § 5, No. 6) and only one such that, for every $\nu \in M$ and every chart $c = (U, \varphi, K^n)$ of X, the image by $\varphi$ of the restriction of $\nu$ to U is equivalent to $\mu_{\varphi(U)}^{\otimes n}$. The class M is called the canonical class of measures on X. For a subset A of X to be locally negligible (10.1.3), it is necessary and sufficient that it be locally negligible (INT, IV, § 2, No. 2) for one (resp. every) measure $\nu \in M$.

If $K = \mathbf{R}$ and $r \neq \omega$ (resp. $K = \mathbf{R}$ or $C$ and $r = \omega$, resp. K is ultrametric), there exists $\nu \in M$ such that, for every chart $c = (U, \varphi, K^n)$ of X, the density of $\varphi(\nu_U)$ with respect to $\mu_{\varphi(U)}^{\otimes n}$ is everywhere $> 0$ and of class $C^{r-1}$ (resp. of class $C^\infty$, resp. locally constant). If $\nu$ and $\nu'$ are two such measures, the density of $\nu'$ with respect to $\nu$ is everywhere $> 0$ and of class $C^{r-1}$ (resp. of class $C^\infty$, resp. locally constant).

10.1.5. Let $X$ be a variety of class $C^r$; let $T'(X)$ be the cotangent bundle of X (8.2.2) and put $\Omega = \det(T'(X))$ (7.9.9). The vector bundle $\Omega$ is of rank 1 at each point; when X is pure of dimension $n$, it is identified with the vector bundle $\mathrm{Alt}^n(T(X); K_X)$. Let $\omega$ be a section of $\Omega$ on X; one says, by abuse of language, that $\omega$ is a differential form of maximum degree on X. Let $c = (U, \varphi, K^n)$ be a chart of X; denote by $u^1, \ldots, u^n$ the coordinate functions on $K^n$. There exists one and only one function $f_c$ on $\varphi(U)$ such that $\omega|U = \varphi^*(f_c du^1 \wedge \cdots \wedge du^n)$. One says that $\omega$ is locally of integrable modulus if, for every chart $c = (U, \varphi, K^n)$ of X, the real function $\mathrm{mod}(f_c) : \varphi(U) \to \mathbf{R}$ is locally integrable for $\mu_{\varphi(U)}^{\otimes n}$ (INT, IV, § 4, No. 1); it suffices to verify this property for the charts of an atlas of X. If $\omega$ is continuous, and in particular if $\omega$ is of class $C^s$, with $s \in \mathbf{N}_K, s \leq r - 1$, then $\omega$ is locally of integrable modulus.

10.1.6 (“Positive measure defined by a differential form of maximum degree”). Retain the notation of 10.1.5 and suppose in addition that X is separated and that $\omega$ is locally of integrable modulus. If $c = (U, \varphi, K^n)$ is a chart of X, denote by $\nu_c$ the measure on $\varphi(U)$ product of the measure $\mu_{\varphi(U)}^{\otimes n}$ by the function mod$(f_c)$ (INT, V, § 5, No. 2, def. 2) and let $\alpha_c$ be the image of $\nu_c$ by $\varphi^{-1}$. There exists on X one and only one measure $\alpha$ such that, for every chart $c = (U, \varphi, K^n)$ of X, the restriction of $\alpha$ to U is equal to $\alpha_c$. One says that the measure $\alpha$ is the modulus of $\omega$ and denotes it by mod$(\omega)_\mu$. It is a positive measure. When $K = \mathbf{R}$ and $\mu$ is Lebesgue measure, one writes $|\omega|$ instead of mod$(\omega)_\mu$.

If X is pure of dimension $n$, and if $a$ is a real number $> 0$, one has $\mathrm{mod}(\omega)_{a\mu} = a^n \mathrm{mod}(\omega)_\mu$.

Let A be a subset of X. In order that A be locally negligible (10.1.3), it is necessary and sufficient that, for every open set U of X and every differential form of maximum degree $\omega$ on U which is locally of integrable modulus, the set $A \cap U$ be locally negligible for the measure $\mathrm{mod}(\omega)_\mu$.

Suppose in addition that X is paracompact and let $\nu$ be a measure on X belonging to the canonical equivalence class M (10.1.4). The measure $\mathrm{mod}(\omega)_\mu$ is based on $\nu$ (INT, V, § 5, No. 2, def. 2). In order that $\mathrm{mod}(\omega)_\mu$ belong to M, it is necessary and sufficient that the set of $x \in X$ such that $\omega(x) = 0$ be locally negligible.

10.1.7. Example. — Let G be a Lie group over K, of finite dimension $n$, and let $\omega$ be a differential form of degree $n$ on G, invariant under left translations, and nonzero. The corresponding measure $\mathrm{mod}(\omega)_\mu$ is then a left Haar measure on the locally compact group G.

When G is the multiplicative group $K^*$, one can take for $\omega$ the form $dx/x$, and one has $\mathrm{mod}(\omega)_\mu = (\mathrm{mod})^{-1}.\mu$, cf. INT, VII, § 1, No. 10, prop. 14.

### 10.2. Orientations

Let us recall that, in this number and the following ones, we suppose that $K = \mathbf{R}$.

10.2.1 (« Orientation of a real vector space »). Let E be a real vector space of finite dimension $n$. We denote by Or(E) the set of orientations of E (A, VI, § 2, No. 7); the elements of Or(E) are the two closed half-lines of the vector space $\det(E) = \bigwedge^n E$. If $\xi \in \mathrm{Or}(E)$, the other element of Or(E) is called the orientation opposite to $\xi$, and denoted $-\xi$.

Let $0 \to E' \xrightarrow{\alpha} E \xrightarrow{\beta} E'' \to 0$ be an exact sequence of (real) vector spaces of finite dimension; put $p' = \dim E',\ p'' = \dim E''$ and let $\xi'$ (resp. $\xi''$) be an orientation of E' (resp. E''). We denote by $\xi'\xi''$ (resp. $\xi''\xi'$) the orientation of E containing a $(p' + p'')$-nonzero vector $u' \wedge u''$ (resp. $u'' \wedge u'$), where $u'$ is the image under $\wedge^\alpha$ of a $p'$-vector of E' belonging to $\xi'$ and where $u''$ is a $p''$-vector of E whose image under $\wedge^\beta$ belongs to $\xi''$ (cf. A, VI,§ 2, No. 7). If $E = E' \times E''$, $\alpha$ and $\beta$ being the canonical mappings, we say that $\xi'\xi''$ is the product of the orientation $\xi'$ and of the orientation $\xi''$.

10.2.2 (« Space of orientations »). Let B be a topological space and M a real vector bundle with base B (in the topological sense — cf. § 6, p. 61, Note (*)), of finite rank

(7.1.6). Let $\mathrm{Or}_M$ be the disjoint union of the $\mathrm{Or}(M_b)$, for $b \in B$, and let $\pi : \mathrm{Or}_M \to B$ be the mapping such that $\pi(\mathrm{Or}(M_b)) = \{b\}$. There exists on $\mathrm{Or}_M$ a structure of topological space and only one such that:

a) $\pi$ is continuous.

b) If $s$ is a continuous and everywhere nonzero section of $\det(M)$ on an open set $U$ of $B$, and if $\xi(s(b))$ is the orientation of $M_b$ defined by the element $s(b)$ of $\det(M_b)$, the mapping $b \mapsto \xi(s(b))$ of $U$ into $\mathrm{Or}_M$ is continuous.

The space $\mathrm{Or}_M$ is called the space of orientations of $M$. The group $\{\pm 1\}$ operates on $\mathrm{Or}_M$ by $\xi \mapsto \pm \xi$ (10.2.1). The quadruplet $(\mathrm{Or}_M, \{\pm 1\}, B, \pi)$ is a principal fibration (6.2.1) with base $B$ and structural group $\{\pm 1\}$; the projection $\pi : \mathrm{Or}_M \to B$ defines an isomorphism of $\mathrm{Or}_M/\{\pm 1\}$ onto $B$, cf. No. 6.2.

When $B$ is endowed with a structure of variety, $\mathrm{Or}_M$ is endowed with the inverse image structure of that of $B$ by $\pi$ (5.8.1); the fibration defined above is then a fibration of varieties and the morphism $\pi$ is étale.

10.2.3. Retain the hypotheses of 10.2.2. An orientation of the vector bundle $M$ is called a continuous section $\xi : B \to \mathrm{Or}_M$ of the projection $\pi : \mathrm{Or}_M \to B$. We say that $M$ is orientable if it possesses an orientation; this is equivalent to saying that the bundle $\mathrm{Or}_M$ is trivializable, i.e. isomorphic to $B \times \{\pm 1\}$. If $B$ is connected and nonempty, every orientable vector bundle with base $B$ possesses two orientations, opposite to one another.

When $M$ is reduced to 0, the bundle $\det(M)$ is the trivial bundle $R_B$ and $\mathrm{Or}_M$ is identified with $\mathrm{Or}(R) \times B$; the bundle $M$ possesses a canonical orientation, corresponding to the positive half-line of $R$.

10.2.4 (« Orientation of a variety »). Let $X$ be a locally finite-dimensional variety over $R$ of class $C^r$, and let $T(X)$ be its tangent bundle. We denote by $\tilde{X}$ the variety $\mathrm{Or}_{T(X)}$; the group $\{\pm 1\}$ operates properly and freely on $\tilde{X}$ and $\tilde{X}/\{\pm 1\}$ is identified with $X$; the fibres of the projection $\pi : \tilde{X} \to X$ are the sets $\mathrm{Or}(T_x(X))$, for $x \in X$. An orientation of $X$ is called an orientation of the bundle $T(X)$, in other words a continuous section of the bundle $\tilde{X}$; such a section is of class $C^r$. We say that $X$ is orientable if it possesses an orientation. Every variety of dimension zero is orientable and possesses a canonical orientation (10.2.3).

Let $\xi \in \tilde{X}$ and let $x = \pi(\xi)$ be its image in $X$; the mapping $T_\xi(\pi) : T_\xi(\tilde{X}) \to T_x(X)$ is an isomorphism; it allows $\xi$ to be identified with an element $\tilde{\xi}$ of $\mathrm{Or}(T_\xi(\tilde{X}))$. The mapping $\xi \mapsto \tilde{\xi}$ is an orientation of $\tilde{X}$, called canonical; in particular, $\tilde{X}$ is orientable.

10.2.5 (« Orientation of a morphism »). Let $X$ and $Y$ be two locally finite-dimensional varieties and let $f : X \to Y$ be a morphism of varieties. An orientation of $f$ is called a morphism $\tilde{f} : \tilde{X} \to \tilde{Y}$ rendering commutative the diagram

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
| & & | \\
X & \xrightarrow{f} & Y
\end{array}
$$

and compatible with the action of the group $\{\pm 1\}$.

If $\tilde{f}$ is an orientation of $f$ and if $\eta$ is an orientation of $Y$, there exists one and only one orientation $\xi$ of $X$ such that the diagram

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
\xi \downarrow & & \eta \downarrow \\
X & \xrightarrow{f} & Y
\end{array}
$$

is commutative. We say that $\xi$ is associated with $\eta$ by $\tilde{f}$.

**Examples**

a) If $Y$ is reduced to a point, an orientation of $f$ is equivalent to an orientation of $X$.

b) Suppose that $f$ is étale. For every $x \in X$, the mapping $T_x(f)$ is an isomorphism of $T_x(X)$ onto $T_{f(x)}(Y)$, and defines (by transport of structure) a bijection

$$
\tilde{f}_x : \mathrm{Or}(T_x(X)) \to \mathrm{Or}(T_{f(x)}(Y)).
$$

The family of the $\tilde{f}_x$ defines an orientation $\tilde{f} : \tilde{X} \to \tilde{Y}$ of $f$, called canonical.

c) More generally, suppose that $f$ is a submersion, and let $\alpha$ be an orientation of the bundle $T(X/Y)$ (8.1.3). Let $x \in X$ and $\xi$ be an orientation of $T_x(X)$. Put $y = f(x)$; one has an exact sequence (8.1.3)

$$
0 \to T_x(X/Y) \to T_x(X) \xrightarrow{T_x(f)} T_y(Y) \to 0
$$

and there exists therefore one and only one orientation $\tilde{f}_\alpha(\xi)$ of $T_y(Y)$ such that $\xi = \tilde{f}_\alpha(\xi)\alpha(x)$ (10.2.1). The mapping $\tilde{f}_\alpha : \tilde{X} \to \tilde{Y}$ is an orientation of $f$, called associated with $\alpha$. The mapping $\alpha \mapsto \tilde{f}_\alpha$ is a bijection of the set of orientations of $T(X/Y)$ onto the set of orientations of $f$.

d) If $f : X \to Y$ is an immersion, the orientations of $f$ correspond to the orientations of the normal bundle to $f$.

10.2.6 (« Orientation of a product »). Let $X_1$ (resp. $X_2$) be a locally finite-dimensional manifold and $\xi_1$ (resp. $\xi_2$) an orientation of $X_1$ (resp. $X_2$). Let $X = X_1 \times X_2$. The mapping $(x_1, x_2) \mapsto \xi_1(x_1)\xi_2(x_2)$ (10.2.1) is an orientation of $X_1 \times X_2$, called the *product* of the orientations $\xi_1$ and $\xi_2$, and denoted by $\xi_1 \xi_2$, or $\xi_1 \otimes \xi_2$.

Suppose that $X_i$ ($i = 1, 2$) is purely of dimension $n_i$. The canonical isomorphism $X_1 \times X_2 \to X_2 \times X_1$ transforms $\xi_1 \otimes \xi_2$ into $\xi_2 \otimes \xi_1$ (resp. into $-\xi_2 \otimes \xi_1$) if one of the $n_i$ is even (resp. if $n_1$ and $n_2$ are odd).

10.2.7 (« Complex case »). Let $F$ be a finite-dimensional complex vector space and let $F_\mathbf{R}$ be the underlying real vector space. Let $\{e_1, \ldots, e_m\}$ be a basis of $F$; then $\{e_1, ie_1, e_2, ie_2, \ldots, e_m, ie_m\}$ is a basis of $F_\mathbf{R}$ and the orientation of $F_\mathbf{R}$ defined by the $2m$-vector

$$
e_1 \wedge ie_1 \wedge e_2 \wedge ie_2 \wedge \cdots \wedge e_m \wedge ie_m
$$

is independent of the choice of the basis $\{e_1, \ldots, e_m\}$ of $F$; this is called *the orientation of $F_\mathbf{R}$* defined *by the given complex structure*. If $F$ is the direct sum of two subspaces $G$ and $H$, the orientation of $F_\mathbf{R} = G_\mathbf{R} \oplus H_\mathbf{R}$ is the product of the orientations of $G_\mathbf{R}$ and $H_\mathbf{R}$.

Let X be a real locally finite-dimensional manifold, endowed with an almost complex structure (8.8.3). For every $x \in X$, let $\xi(x)$ be the orientation of $T_x(X)$ defined by its complex structure. The mapping $x \mapsto \xi(x)$ is an orientation of X, said to be defined by the almost complex structure. In particular, we shall endow the real analytic manifold X underlying a complex analytic manifold $X^c$, locally finite-dimensional, with the orientation defined by the associated almost complex structure (8.8.6). If the given complex analytic manifold structure on X is replaced by its conjugate (5.4.12.b)), this orientation is multiplied by the function $x \mapsto (-1)^{\dim_{\mathbf{R}} X^c}$.

10.2.8. Examples

a) Let E be a finite-dimensional real vector space. The real analytic manifold defined by E (5.2.2) is orientable. More precisely, the mapping $\xi \mapsto \xi(0)$ is a bijection from the set of orientations of this manifold onto Or(E).

In particular, the manifold $\mathbf{R}^n$ has a canonical orientation $\xi^n$ defined by the half-line $\mathbf{R}_+ e_1 \wedge \cdots \wedge e_n$ of Or($\mathbf{R}^n$).

(b) Let $X$ be a *sphere* with centre 0 and radius $> 0$ in $\mathbf{R}^n$; it is a submanifold of $\mathbf{R}^n$. For every $x \in X$, the space $T_x(\mathbf{R}^n) = \mathbf{R}^n$ is the direct sum of the right line Rx and the hyperplane $T_x(X)$. Let $\eta_x$ be the orientation $\mathbf{R}_+ x$ of Rx (“outward normal”) and let $\xi_x$ be the unique orientation of $T_x(X)$ such that the product of $\eta_x$ and $\xi_x$ is the orientation $\xi^n$ of $\mathbf{R}^n$. The mapping $x \mapsto \xi_x$ is an orientation of $X$, called canonical.

(c) Let $X$ be a connected manifold, and let $G$ be a discrete group acting properly and freely on $X$. For $X/G$ to be orientable, it is necessary and sufficient that $X$ be orientable and that the action of $G$ on the set of orientations of $X$ be trivial.

(d) *The real projective space* $P_{n-1}(\mathbf{R})$ is identified with the quotient of the sphere $S_{n-1}$ by the group $\{ \pm 1 \}$ acting by $x \mapsto \pm x$; it is orientable if $n$ is even, and non-orientable if $n$ is odd.

(e) Every quotient of a Lie group by a *connected* Lie subgroup is orientable.

### 10.3. M-twisted differential forms

10.3.1. Let $X$ be a real manifold of class $C^r$, and let $M$ be a vector bundle with base $X$, of finite rank and of class $C^k$, with $0 \leq k \leq r$. Let $\lambda_M = (\mathrm{Or}_M, \{ \pm 1 \}, X, \pi)$ be the principal fibration associated with the manifold of orientations of $M$ (10.2.2). Let the structural group $\{ \pm 1 \}$ act on $\mathbf{R}$ by multiplication. Denote by $\tilde{R}_M$ the fibre bundle associated with $\lambda_M$ with typical fibre $\mathbf{R}$ (endowed with the law of operation defined above) (6.5.1); it is endowed (7.10.2) with a structure of vector bundle with base $X$, of rank 1 and of class $C^k$; it is called the *bundle of M-twisted scalars*.

10.3.2. We have a commutative diagram:

$$
\begin{array}{ccc}
\mathrm{Or}_M \times \mathbf{R} & \xrightarrow{\rho} & \tilde{R}_M \\
\downarrow \mathrm{pr}_1 & & \downarrow p \\
\mathrm{Or}_M & \xrightarrow{\varphi} & X
\end{array}
$$

where $p$ denotes the canonical projection of $\tilde{\mathbf{R}}_M$ onto $X$, $\rho$ the frame mapping (6.5.1) of $\tilde{\mathbf{R}}_M$ and where $\varphi(\xi) = \rho(\xi, 1)$ for $\xi \in \mathrm{Or}_M$. In particular, the inverse image of the bundle $\tilde{\mathbf{R}}_M$ by $\pi$ is identified with the trivial bundle $\mathrm{Or}_M \times \mathbf{R}$. An element $\xi$ of $\mathrm{Or}_M$ is also identified with its image in $\tilde{\mathbf{R}}_M$ by $\varphi$; with this convention, we have $\rho(\xi, a) = a\xi$ for every $(\xi, a) \in \mathrm{Or}_M \times \mathbf{R}$; we have $a\xi = b\eta$ if and only if there exists $e \in \{ \pm 1 \}$ such that $b = ea$ and $\eta = e\xi$. An orientation $\xi$ of $M$ thus defines a section $x \mapsto \xi(x)$ of $\tilde{\mathbf{R}}_M$.

There exists one and only one isomorphism $j$ of $\tilde{\mathbf{R}}_M \otimes \tilde{\mathbf{R}}_M$ onto the trivial bundle $R_X = X \times \mathbf{R}$ such that $j(\xi \otimes \xi) = (\pi(\xi), 1)$ for all $\xi \in \mathrm{Or}_M$; this allows the vector bundle $\tilde{\mathbf{R}}_M$ to be identified with its dual.

10.3.3. Let moreover $F$ be a vector bundle with base $X$ and of class $C^{r-1}$. A differential form on $X$ with values in $\tilde{\mathbf{R}}_M \otimes F$ is called an $M$-twisted differential form with values in $F$. Such a form of degree $p$ is a section of the bundle $\mathrm{Alt}^p(T(X); \tilde{\mathbf{R}}_M \otimes F)$, which is identified in an obvious manner with $\tilde{\mathbf{R}}_M \otimes \mathrm{Alt}^p(T(X); F)$. When $F$ is the trivial bundle defined by a Banach space $E$, one simply speaks of an $M$-twisted form with values in $E$; when $E = \mathbf{C}$ (resp. $\mathbf{R}$), one says complex $M$-twisted form (resp. real $M$-twisted form, or $M$-twisted form).

Let $\omega$ be an $M$-twisted form of degree $p$ with values in $F$. The fact that $\pi : \mathrm{Or}_M \to X$ is étale and that $\pi^*(\tilde{\mathbf{R}}_M) = \mathrm{Or}_M \times \mathbf{R}$ allows $\pi^*(\mathbf{R}_M \otimes \mathrm{Alt}^p(T(X); F))$ to be identified with $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ and $\omega$ defines a section $\tilde{\omega}$ of $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ (7.4.3), in other words, a differential form of degree $p$ on $\mathrm{Or}_M$ with values in $\pi^*(F)$. One thus obtains a bijection from the space of $M$-twisted forms of degree $p$ on $X$ with values in $F$, onto the space of forms $\tilde{\omega}$ of degree $p$ on $\mathrm{Or}_M$ with values in $\pi^*(F)$ such that
$$
\tilde{\omega}(-\xi) = -\tilde{\omega}(\xi) \quad \text{pour tout } \xi \in \mathrm{Or}_M.
$$
When $M$ is endowed with an orientation $\xi$, the mapping $\omega \mapsto \xi \otimes \omega$ allows the sections of $\mathrm{Alt}^p(T(X); F)$ (in other words the usual differential forms of degree $p$) to be identified with the $M$-twisted forms of degree $p$ with values in $F$.

10.3.4. Let $\omega$ be an $M$-twisted differential form of degree $p$ on $X$, with values in a Banach space $E$, and of class $C^s$ ($1 \leq s \leq \inf(k, r-1)$). There exists one and only one $M$-twisted differential form $d\omega$, of degree $p+1$ on $X$, with values in $E$, such that, for every open set $U$ of $X$, orientation $\xi$ of $M|U$ and differential form $\alpha$ on $U$ such that $\omega|U = \xi \otimes \alpha$, one has $d\omega|U = \xi \otimes d\alpha$. The form $d\omega$ is of class $C^{s-1}$; it is called the exterior differential of $\omega$.

If $\tilde{\omega}$ (resp. $\tilde{d\omega}$) denotes the differential form on $\mathrm{Or}_M$ corresponding to $\omega$ (resp. to $d\omega$) as in 10.3.3, one has $d(\tilde{\omega}) = \tilde{d\omega}$.

If $\zeta$ is a vector field of class $C^s$ on $X$, one defines analogously the $M$-twisted form $\theta_\zeta.\omega$. One has
$$
\theta_\zeta.\omega = d(i(\zeta)\omega) + i(\zeta)d\omega
$$
and $\theta_\zeta.\omega$ is of class $C^{s-1}$.

### 10.4. Measure associated with a twisted differential form

Let us recall that, in this number, we suppose $K = \mathbf{R}$ and that all the varieties considered are locally of finite dimension.

10.4.1. Let X be a variety of class C'. We can apply the definitions and results of 10.3 by taking for vector bundle M the tangent bundle T(X). We then have Or_M = $\tilde{X}$ (10.2.4); we denote $\tilde{R}_X$ and simply call the bundle of twisted scalars the bundle $\tilde{R}_{T(X)}$ (10.3.1)[^2]; a T(X)-twisted differential form with values in a vector bundle F is simply called a twisted (or odd) differential form with values in F. When X is endowed with an orientation, the mapping $\omega \mapsto \xi \otimes \omega$ makes it possible to identify the usual differential forms (sometimes called «pairs») with twisted forms.

10.4.2. Let $f : X \to Y$ be a morphism of manifolds of class C' and let $\tilde{f} : \tilde{X} \to \tilde{Y}$ be an orientation of $f$ (10.2.5). There exists one and only one isomorphism $j$ of $f^*(\tilde{R}_Y)$ onto $\tilde{R}_X$ such that $\tilde{x} = j(\pi(\tilde{x}), \tilde{f}(\tilde{x}))$ for every $\tilde{x} \in \tilde{X}$. We identify these two bundles by means of $j$. If $\omega$ is a twisted form of degree $p$ on Y with values in a vector bundle F, the inverse image $f^*(\omega)$ is identified with a twisted differential form of degree $p$ on X with values in $f^*(F)$. If we denote by $\tilde{\omega}$ (resp. $\tilde{f}^*(\omega)$) the differential form on $\tilde{Y}$ (resp. $\tilde{X}$) corresponding to $\omega$ (resp. $f^*(\omega)$) as in 10.3.3, we have $\tilde{f}^*(\tilde{\omega}) = \tilde{f}^*(\omega)$.

When F is the trivial bundle defined by a Banach space, the operation $f^*$ commutes with exterior differentiation (10.3.4).

10.4.3. Let X be a pure manifold of dimension n, and let $\omega$ be a twisted differential form of degree n on X, with values in a Banach space E. Let $c = (U, \varphi, \mathbf{R}^n)$ be a chart of X and let $\xi^n$ be the canonical orientation of $\mathbf{R}^n$; let $u^1, \ldots, u^n$ denote the coordinate functions on $\mathbf{R}^n$. There exists one and only one function $f_c$ on $\varphi(U)$, with values in E, such that

$$
\omega|U = \varphi^*(\xi^n \otimes f_c . du^1 \wedge \cdots \wedge du^n).
$$

We say that $\omega$ is locally integrable if, for every chart $c = (U, \varphi, \mathbf{R}^n)$ of X, the corresponding function $f_c$ is locally integrable with respect to $\lambda_{\varphi(U)}^{\otimes n}$ (where $\lambda$ denotes Lebesgue measure on $\mathbf{R}$). Suppose that this is the case and that X is separated. There exists on X one and only one vector measure $\alpha(\omega)$ with values in E having the following property: for every chart $c = (U, \varphi, \mathbf{R}^n)$ of X, the image by $\varphi$ of the restriction to U of the measure $\alpha(\omega)$ is the measure $f_c . \lambda_{\varphi(U)}^{\otimes n}$ (INT, VI, § 2, No. 4). We say that $\alpha(\omega)$ is the measure defined by $\omega$ and we usually denote it simply by $\omega$. The support of $\alpha(\omega)$ is contained in the support Supp $\omega$ of $\omega$ (where the support of a differential form $\omega$ is defined to be the closure of the set of $x \in X$ such that $\omega(x) \neq 0$).

If $f$ is a real function on X, locally integrable with respect to the measure $\alpha(\omega)$, then the differential form $f \omega$ is locally integrable and we have $\alpha(f \omega) = f . \alpha(\omega)$.

If $g$ is a real function on $X$ essentially integrable for $\alpha(\omega)$, its integral is generally denoted $\int_X g \omega$, or $\int g \omega$, or $\int g(x) \omega(x)$; one avoids denoting it $\int g \, d\omega$, because of the risks of confusion with the exterior differential $d\omega$ of $\omega$, which is defined (and is moreover equal to 0) if $\omega$ is of class $C^1$. If A is a subset of X whose characteristic function $\varphi_A$ is essentially integrable for $\alpha(\omega)$, the integral of $\varphi_A$ is denoted

∫_A ω. If the constant 1 is essentially integrable for α(ω), one says that ω is integrable.

Let now p be an integer, with 0 ≤ p ≤ n, and let ω be a twisted differential form of degree p on X, with values in a Banach space E. Let moreover Y be a pure submanifold of dimension p of X; suppose that the canonical injection i : Y → X is provided with an orientation. The inverse image i*(ω) (10.4.2) is then sometimes denoted ω|Y. If ω|Y is integrable, one sets

$$
\int_Y \omega = \int_Y \omega|Y.
$$

10.4.4. Let X be a pure manifold of dimension n, provided with an orientation ξ. The identification ω ↦ ξ ⊗ ω between ordinary differential forms and twisted differential forms makes it possible to apply what precedes to forms of degree n on X; thus, to every locally integrable form ω, of degree n, there corresponds a measure on X, again denoted ω. If E = R, such a form ω is locally of integrable modulus (10.1.5) and the corresponding measure mod(ω)_μ (10.1.6) is none other than the absolute value |ω| of the measure ω (INT, III, § 1, No. 6).

10.4.5. Example. — Let X be a pure real manifold of dimension 1, oriented, separated, and let z : X → C be a differentiable mapping of X into C. The complex differential form dz defines on X a complex measure also denoted dz. This applies in particular when X is a pure differential submanifold of dimension 1 of C, z being the injection of X into C.

More particularly, take for X a circle with center 0 and radius ρ > 0; orient X as indicated in 10.2.8, b), taking account of the usual identification of C with R²; if x ∈ X, the tangent space T_x(X) is identified with the right Rix of T_x(C) = C and the chosen orientation is the half-right R_+ ix. If f is a continuous function on X, with values in a complex Banach space, the integral of f for the measure dz is given by the formula

$$
\int_X f(z)\,dz = i\rho \int_0^{2\pi} f(\rho e^{i\alpha})\,e^{i\alpha}\,d\alpha.
$$

For example, if n is an integer, we have

$$
\int_X z^n\,dz = i\rho^{n+1} \int_0^{2\pi} e^{(n+1)i\alpha}\,d\alpha = \begin{cases} 0 & \text{if } n \neq -1 \\ 2i\pi & \text{if } n = -1. \end{cases}
$$

10.4.6 (« Complex case »). Let X^c be a separated complex analytic manifold, pure of dimension m, and let ω be a holomorphic differential form of degree m on X^c. Let X be the real analytic manifold underlying X^c; the form ω is identified with a form of type (m, 0) on X (8.8.9); let $\overline{\omega}$ be its conjugate (8.8.2). The form $i^{m^2} \omega \wedge \overline{\omega}$ is a real differential form of degree 2m on X; taking account of the canonical orientation of X (10.2.7), this form is identified with a measure on X, which is none other than the positive measure mod(ω)_μ defined in 10.1.6, where μ is the measure defined by the differential form $i\,dz\wedge d\bar z$, in other words twice the Lebesgue measure $\lambda^{\otimes 2}$ on $\mathbf{C}$ (identified with $\mathbf{R}^2$ in the usual manner).

Let H be the space of holomorphic forms $\omega$ of degree m on $X^c$ such that the measure $\omega\wedge\bar\omega$ is bounded. For $\alpha,\beta$ in H, the complex measure $\alpha\wedge\bar\beta$ is bounded; by setting

$$
(\alpha|\beta)=i^{m^2}\int_X \alpha\wedge\bar\beta,
$$

one obtains a Hermitian form on H, which makes H a Hilbert space.

[^1]: When $K = \mathbf{R}$, it suffices to suppose that $r > \sup_{y \in Y} (\dim_{f(y)} X - \dim_y Y)$; cf. for example A. SARD, Bull. Am. Math. Soc., XLVIII (1943), p. 883–890.
[^2]: One should take care that this notation is contradictory with the notation $\tilde{R}_M$ when one considers X as provided with its structure of a vector bundle of rank 0 over itself.
