---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 13
section_title: Distributions ponctuelles
lang: en
source: var-fr
pdf_pages: 0152-0161
extraction: ocr
subsections:
    - "no": 1
      title: Tenseurs symétriques et espaces de Banach
      page: 0
      pdf_page: 152
    - "no": 2
      title: Distributions ponctuelles
      page: 0
      pdf_page: 153
    - "no": 3
      title: Distributions ponctuelles et espaces tangents
      page: 0
      pdf_page: 156
    - "no": 4
      title: Produit tensoriel de distributions ponctuelles
      page: 0
      pdf_page: 157
    - "no": 5
      title: Coproduits
      page: 0
      pdf_page: 159
    - "no": 6
      title: Distributions à support fini
      page: 0
      pdf_page: 160
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 161
statements: 0
exercises: 0
content_sha256: c08a2c7e88efd6da15237d6acfbddbe178e993d69a8ca0743673273708ddd20c
translated_from: content/fr/var/2/13_s13_distributions_ponctuelles.md
source_lang: fr
translation_method: machine
source_content_sha256: 4e1cfc6fb0ea10651026181a15c455ecd575a63746635f7a5b12e614beb9bb93
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-en-mt-c1a9b719
glossary_version: 34
glossary_terms_sha256: 33f969a1c77b7ec314de4d7b5a5740a8853f97bec0185201e00df79df823f748
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 13. Point distributions

### 13.1. Symmetric tensors and Banach spaces

### 13.1.1. Let E be a module over a commutative ring A. If n is an integer $\geq 0$, denote by $TS^n(E)$ the module of symmetric tensors of rank n of E (A, III, p. 71 and A, IV, § 5, no 2); the direct sum of the $TS^n(E)$ is denoted by $TS(E)$. If r is an integer, one of the symbols $\infty,\omega$, put

$$
TS^{(r)}(E)=\bigoplus_{n\leq r}TS^n(E)\quad\text{and}\quad TS^{(r)+}(E)=\bigoplus_{1\leq n\leq r}TS^n(E);
$$

consequently, if $r\geq 0$, $TS^{r}(E)$ is the direct sum of $TS^{(0)}(E)=A$ and of $TS^{(r)+}(E)$. One has $TS^{(1)+}(E)=E$ and $TS^{(\infty)}(E)=TS^{(\omega)}(E)=TS(E)$.

If $n$ is an integer $\geq 0$, and if $x\in E$, denote by $\gamma_n(x)$ the element $x\otimes\cdots\otimes x$ of $TS^n(E)$; for $n=0$, $\gamma_0(x)=1$.

### 13.1.2. (« Polynomial mappings »). Suppose that A is integral infinite and that E is a free a-module. Let F be an a-module. A mapping $f:E\rightarrow F$ is said to be homogeneous polynomial of degree n if it satisfies the following equivalent conditions (cf. A, IV, § 5, no 9):

a) There exists a linear mapping $\tilde f:TS^n(E)\rightarrow F$ such that $f(x)=\tilde f(\gamma_n(x))$ for all $x\in E$.

b) There exists a multilinear mapping $u:E^n\rightarrow F$ such that $f(x)=u(x,\ldots,x)$ for all $x\in E$.

Suppose that this is the case. The mapping $\tilde f$ satisfying a) is then unique; if $t\in TS^n(E)$, denote by $\langle f,t\rangle$ the element $\tilde f(t)$. If $u:E^n\rightarrow F$ satisfies b), the corresponding linear mapping of $\otimes^nE$ into F coincides in the submodule $TS^n(E)$. When $n!$ is invertible in A, one may choose $u$ symmetric, and this in a unique way.

### 13.1.3. Let E be a Banach space over K and F a separated polynomial space over K. Let U be an open neighbourhood of 0 in E, $f:U\rightarrow F$ a mapping of class $C^r$ ($r\in\mathbf{N}_K$), and $t$ an element of $TS^{(r)}(E)$, cf. 13.1.1 (applied to the ring $A=K$). Let $k$ be an integer $\leq r$ such that $t\in TS^{(k)}(E)$. One can decompose $t$ and $f$ uniquely into

$$
t=t_0+\cdots+t_k,\qquad \text{with }t_i\in TS^i(E)
$$

and

$$
f=f_0+\cdots+f_k+h,
$$

where $f_i$ is a homogeneous continuous polynomial of degree $i$ ($0 \leq i \leq k$) and where $h$ has contact of order $\geq k$ with 0 at the point 0. Put then

$$
\langle f, t \rangle = \sum_{i=0}^{k} \langle f_i, t_i \rangle;
$$

this is an element of F which does not depend on the choice of $k$.

13.1.4. Let E and E’ be two Banach spaces, U an open neighbourhood of 0 in E and $\varphi : U \to E'$ a mapping of class $C^r$ such that $\varphi(0) = 0$. Let $t \in TS^{(r)}(E)$. There exists one and only one element $t' \in TS^{(r)}(E')$ such that, for every separated polynormed space F, every open neighbourhood U’ of 0 in E’, and every mapping $f : U' \to F$ of class $C^r$, one has

(*) $$
\langle f, t' \rangle = \langle f \circ \varphi, t \rangle.
$$

This element $t'$ is denoted by $\varphi_*(t)$. The mapping

$$
\varphi_* : TS^{(r)}(E) \to TS^{(r)}(E')
$$

thus defined is linear.

### 13.2. Point distributions

In this No., X denotes a manifold of class $C^r$, and $x$ a point of X.

13.2.1. Let $\mathscr{A}$ be the set of pairs $(c, t)$, where $c = (U, \varphi, E)$ is a chart of X centred at $x$, and where $t \in TS^{(r)}(E)$. Two elements $((U, \varphi, E), t)$ and $((U', \varphi', E'), t')$ of $\mathscr{A}$ are said to be equivalent if $t' = \gamma_*(t)$, where $\gamma = \varphi' \circ \varphi^{-1}$. In this way one obtains an equivalence relation on $\mathscr{A}$; an equivalence class for this relation is called a point distribution at $x$ on X.

Let $T_x^{(r)}(X)$ be the set of point distributions at $x$ on X. If $c$ is a chart of X centred at $x$, the mapping

$$
\theta_c : TS^{(r)}(E) \to T_x^{(r)}(X)
$$

which associates with $t$ the class of $(c, t)$, is a bijection. In all that follows, $T_x^{(r)}(X)$ is endowed with the structure of a K-vector space obtained by transporting that of $TS^{(r)}(E)$ by means of $\theta_c$; this structure does not depend on the choice of $c$. Analogously, if $k \leq r$, $T_x^{(k)}(X)$ and $T_x^{(k)+}(X)$ denote the images of $TS^{(k)}(E)$ and $TS^{(k)+}(E)$ under $\theta_c$; they do not depend on the choice of $c$. An element of $T_x^{(r)}(X)$ is said to be of order $\leq k$ if it belongs to $T_x^{(k)}(X)$. One has

$$
T_x^{(k)}(X) = T_x^{(0)}(X) \oplus T_x^{(k)+}(X).
$$

There exists one and only one element $\varepsilon_x$ of $T_x^{(0)}(X)$ such that $\theta_c(1) = \varepsilon_x$ for every chart $c$ of X centred at $x$. If $t$ is a point distribution at $x$, the constant term of $t$ is the element $\lambda$ of K such that $t - \lambda \varepsilon_x \in T_x^{(r)+}(X)$; one says that $t$ is without constant term if its constant term is zero.

13.2.2. Let F be a separated polynormed space, and let $f$ be a function of class $C^r$ with values in F, defined on a neighbourhood of $x$. Let $t$ be a point-supported distribution at $x$ on X.

Consider a chart $c = (U, \varphi, E)$ of $X$ centred at $x$, and put $f_c = f \circ \varphi^{-1}$ and $t_c = \theta_c^{-1}(t)$; the element $\langle f_c, t_c \rangle$ of $F$ defined in 13.1.3 does not depend on the choice of $c$; we denote it by $\langle f, t \rangle$. One has $\varepsilon_x(f) = f(x)$.¹ The constant term of $t$ is $\langle 1, t \rangle$.

If $F'$ is a separated polynormed space and if $u : F \to F'$ is continuous linear, one has $\langle u \circ f, t \rangle = u(\langle f, t \rangle)$.

Suppose that $F$ is a Banach space, and that $t$ is of order $\leq k$, with $k$ finite. Let $j \in J_x^k(X, F)$, cf. 12.1.2, and let $f \in j$. Then $\langle f, t \rangle$ depends only on the jet $j$; we denote it by $\langle j, t \rangle$. The mapping from $T_x^{(k)}(X) \times J_x^k(X, F)$ into $F$ thus defined is bilinear. When $F = K$, we have put $J_x^k(X, F) = P_x^k(X)$, cf. 12.6.2, and we obtain a *bilinear form* on $T_x^{(k)}(X) \times P_x^k(X)$.

13.2.3. Let $\varphi : X \to Y$ be a morphism of manifolds of class $C^r$ and let $y = \varphi(x)$. Let $c = (U, \psi, E)$ be a chart of $X$ centred at $x$ and let $c' = (U', \psi', E')$ be a chart of $Y$ centred at $y$; let $\tilde{\varphi}$ be the expression of $\varphi$ in these charts (5.3.2), and let $\tilde{\varphi}_*$ be the corresponding mapping from $TS^{(r)}(E)$ into $TS^{(r)}(E')$, cf. 13.1.4. There exists one and only one linear mapping, denoted by $T_x^{(r)}(\varphi)$ or $\varphi_*$, from $T_x^{(r)}(X)$ into $T_y^{(r)}(Y)$, making the diagram commutative

$$
\begin{array}{ccc}
TS^{(r)}(E) & \xrightarrow{\tilde{\varphi}_*} & TS^{(r)}(E') \\
\downarrow_{\theta_c} & & \downarrow_{\theta_c} \\
T_x^{(r)}(X) & \xrightarrow{\varphi_*} & T_y^{(r)}(Y).
\end{array}
$$

This mapping does not depend on the choice of $c$ and $c'$. If $t \in T_x^{(r)}(X)$, $\varphi_*(t)$ is called the *image* of $t$ by $\varphi$. We have $\varphi_*(\varepsilon_x) = \varepsilon_y$. If $k \leq r$, we have
$$
\varphi_*(T_x^{(k)}(X)) \subset T_y^{(k)}(Y) \quad \text{and} \quad \varphi_*(T_x^{(k)+}(X)) \subset T_y^{(k)+}(Y).
$$

If $\varphi' : X \to Y$ is a morphism of class $C^r$ mapping $x$ onto $y$, we have $\varphi_* = \varphi'_*$ if and only if $j_x^r(\varphi) = j_x^r(\varphi')$, cf. 12.1.

If $\varphi$ is an immersion (resp. a submersion) at $x$, $\varphi_*$ is injective (resp. surjective); the converse is true if $\dim_y Y < +\infty$.

If $\varphi' : Y \to Z$ is a morphism of $C^r$ manifolds, and if $t \in T_x^{(r)}(X)$, we have $(\varphi' \circ \varphi)_*(t) = \varphi'_*(\varphi_*(t))$.

Let $F$ be a separated polynormed space, and let $f$ be a function of class $C^r$ with values in $F$, defined in a neighbourhood of $y$. We then have
$$(1)$$
$$
\langle f, \varphi_*(t) \rangle = \langle f \circ \varphi, t \rangle \quad \text{for all } t \in T_x^{(r)}(X).
$$
For given $t$, the relations (1) (for variable $f$ and $F$) *characterize* $\varphi_*(t)$; when $\dim_y Y < +\infty$, we may restrict ourselves to $F = K$.

13.2.4. Suppose that $X$ is an open submanifold of a *Banach space* $E$. Denote by $\varphi_x$ the mapping $y \mapsto y - x$ of $X$ into $E$; the chart $c = (X, \varphi_x, E)$ is centred

¹ When $K = \mathbf{R}$ or $\mathbf{C}$ and $X$ is locally compact, the preceding formula leads to identifying the point distribution $\varepsilon_x$ with the *Dirac measure* $\varepsilon_x$ defined in JNT, III, § 1, No. 3. More generally, every measure with finite support in $X$ is identified with a distribution with finite support in the sense of No. 13.6.

at $x$. We then identify $T_x^{(r)}(X)$ with $TS^{(r)}(E)$ by means of $\theta_c^{-1}$; in particular, we have $T_x^{(\infty)}(X) = TS(E)$.

Let $F$ be a Banach space, let $u : E \to F$ be a continuous linear mapping, and let $x \in E, y \in F$ be such that $u(x) = y$. Identify as above $T_x^{(\infty)}(E)$ with $TS(E)$ and $T_y^{(\infty)}(F)$ with $TS(F)$. The mapping
$$
u_* : TS(E) \to TS(F) \quad (\text{cf. } 13.2.3)
$$
coincides with the mapping $TS(u)$ induced by the canonical extension of $u$ to the tensor algebra.

13.2.5. If $k \leq r$, denote by $T^{(k)}(X)$ (resp. $T^{(k)+}(X)$) the sum set of the $T_a^{(k)}(X)$ (resp. of the $T_a^{(k)+}(X)$) for $a \in X$. A mapping $t : X \to T^{(k)}(X)$ such that $t(a) \in T_a^{(k)}(X)$ for all $a \in X$ is called a field of point distributions of order $\leq k$.

Suppose $k$ finite and $X$ locally of finite dimension. For every $a \in X$, the bilinear form $(j, t) \mapsto \langle j, t \rangle$ (cf. 13.2.2) defines an isomorphism $i_a$ of $T_a^{(k)}(X)$ onto the dual $P_a^k(X)^*$ of $P_a^k(X)$. The $i_a$ define a bijection $i : T^{(k)}(X) \to P^k(X)^*$, where $P^k(X)^*$ denotes the dual of the vector bundle $P^k(X)$; by transport of structure by means of $i^{-1}$, one endows $T^{(k)}(X)$ with a structure of vector bundle with base $X$ and of class $C^{r-k}$. A field of point distributions of order $\leq k$ is said to be of class $C^s$, with $s \leq r - k$, if it is a section of class $C^s$ of the vector bundle $T^{(k)}(X)$.

Let $\varphi : X \to Y$ be a morphism of manifolds of class $C^r$ and suppose that $Y$ is, like $X$, locally of finite dimension. Then $\varphi_* : T^{(k)}(X) \to T^{(k)}(Y)$ is a $\varphi$-morphism of vector bundles of class $C^{r-k}$.

13.2.6. Let $k$ be an integer such that $0 \leq k \leq r$. If $U$ is an open set of a Banach space $E$ of finite dimension, the vector bundle $T^{(k)}(U)$ is identified, thanks to 13.2.4, with the trivial bundle of fibre $TS^{(k)}(E)$.

Take in particular $E = K^n$, with $n \geq 0$, and let $(e_1, \ldots, e_n)$ be the canonical basis of $E$. If $\alpha = (\alpha_1, \ldots, \alpha_n)$ is an element of $\mathbf{N}^n$, denote by $\Delta^\alpha$ the element $\gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n)$ of $TS(E)$ (the product used being the symmetric product of symmetric tensors, cf. A, IV, § 5, No. 3).(1) The $\Delta^\alpha$, for $|\alpha| \leq k$, form a basis of $TS^{(k)}(E)$; if $a \in K^n$, denote by $\Delta_a^\alpha$ the corresponding elements of $T_a^{(k)}(E)$. Let $F$ be a separated polynormed space, and $f$ a function of class $C^r$, with values in $F$, defined in a neighbourhood of $a$; if $\alpha \in \mathbf{N}^n$, the element $\langle f, \Delta_a^\alpha \rangle$ coincides with the element $(\Delta^\alpha f)(a)$ defined in 2.5.3, 3.2.1 and 4.2.1.

Suppose $X$ is locally of finite dimension, and let $\xi = (\xi^1, \ldots, \xi^n)$ be a system of coordinates of $X$ in an open set $U$. If $a \in U$ and if $\alpha$ is a multi-index such that $|\alpha| \leq k$, denote by $(\Delta_\xi^\alpha)_a$ the point distribution at $a$ whose image by $\xi$ is the point distribution $\Delta_{\xi(a)}^\alpha$ on $K^n$; the fields of distributions
$$
\Delta_\xi^\alpha : a \mapsto (\Delta_\xi^\alpha)_a \quad (|\alpha| \leq k)
$$
form a frame on $U$ of the vector bundle $T^{(k)}(X)$. If $f : U \to F$ is of class $C^r$, put $\langle f, (\Delta_\xi^\alpha)_a \rangle = \Delta_\xi^\alpha f(a)$ and denote by $\Delta_\xi^\alpha f$ the function $a \mapsto \Delta_\xi^\alpha f(a)$; this is a function of class $C^{r-k}$ in $U$.

(1) If $m = |\alpha|$ and if $\Sigma$ is the set of mappings $\sigma$ of $\{1, \ldots, m\}$ into $\{1, \ldots, n\}$ such that $\mathrm{Card}\, \sigma^{-1}(i) = \alpha_i$, we have
$$
\Delta^\alpha = \gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n) = \sum_{\sigma \in \Sigma} e_{\sigma(1)} \otimes \cdots \otimes e_{\sigma(n)}, \quad \text{cf. A, IV, § 5, n° 4.}
$$

### 13.3. Point distributions and tangent spaces

In this No., $X$ denotes a variety of class $C^r$.

### 13.3.1. Let $x \in X$ and let $k$ be an integer $\leq r$. Let $c=(U,\varphi,E)$ be a chart of $X$ centred at $x$; the isomorphism $\theta_c:T^S(X)(E)\to T_x(X)$ defined in 13.2.1 maps $T^S{}^{(k)}(E)$ onto $T_x^{(k)}(X)$ and $T^S{}^{(k-1)}(E)$ onto $T_x^{(k-1)}(X)$; by restriction and passing to the quotient, it induces an isomorphism

$$
\theta_{c,k}:T^S{}^{(k)}(E)=T^S{}^{(k)}(E)/T^S{}^{(k-1)}(E)\longrightarrow T_x^{(k)}(X)/T_x^{(k-1)}(X).
$$

On the other hand, $c$ defines an isomorphism, already denoted by $\theta_c$, of $E$ onto the tangent space $T_x(X)$, cf. 5.5.1. Let $i_k$ denote the composite

$$
T_x^{(k)}(X)/T_x^{(k-1)}(X)\xrightarrow{\theta_{c,k}^{-1}}T^S{}^{(k)}(E)\xrightarrow{T^S(\theta_c)}T^S{}^{(k)}(T_x(X)).
$$

The isomorphism $i_k$ is independent of the choice of $c$; for $k=1$, it is used to identify $T_x^{(1)}(X)=T_x^{(1)}(X)/T_x^{(0)}(X)$ with the tangent space $T_x(X)$. If $t\in T_x^{(k)}(X)$, we allow ourselves to denote by $i_k(t)$ the image by $i_k$ of the class of $t$ modulo $T_x^{(k-1)}(X)$.

Put

$$
\operatorname{gr}_k T_x^{(r)}(X)=T_x^{(k)}(X)/T_x^{(k-1)}(X)
$$

and

$$
\operatorname{gr}T_x^{(r)}(X)=\bigoplus_{0\leq k\leq r}\operatorname{gr}_k T_x^{(r)}(X).
$$

We say that $\operatorname{gr}T_x^{(r)}(X)$ is the graded associated with the increasing filtration $(T_x^{(k)}(X))_{k\leq r}$ of $T_x^{(r)}(X)$. The $i_k$ define an isomorphism of graded vector spaces

$$
i:\operatorname{gr}T_x^{(r)}(X)\longrightarrow T^S{}^{(r)}(T_x(X)).
$$

If $r=\infty$ or $\omega$, $i$ is an isomorphism of $\operatorname{gr}T_x^{(r)}(X)$ onto $T^S(T_x(X))$. When one wishes to specify $x$ (or $X$, or both), one writes $i_x$ (or $i_X$, or $i_{x,X}$) in place of $i$.

### 13.3.2. In addition to the above hypotheses, suppose that $X$ is locally finite-dimensional. The isomorphisms $i_k$ corresponding to the different points of $X$ define an isomorphism of vector bundles

$$
i_k:T^{(k)}(X)/T^{(k-1)}(X)\longrightarrow TS^{(k)}(T(X))
$$

where $TS^{(k)}(T(X))$ denotes the vector bundle of class $C^{r-1}$ obtained from $T(X)$ by the finite-dimensional vector functor $TS^{(k)}$ (cf. 7.6.5). For $k\geq 1$, $i_k$ is an isomorphism of class $C^{r-k}$; for $k=0$, it is the identity mapping of the trivial bundle $K_X$.

### 13.3.3. **Example.** — The hypotheses being as above, let $\xi=(\xi^1,\ldots,\xi^n)$ be a system of coordinates of $X$ at $x$. Let $(\partial_i)_{1\leq i\leq n}$ be the basis of $T_x(X)$ defined by $\xi$ (cf. 5.5.8) and let $(\Delta^\alpha_x)_{|\alpha|\leq k}$ be that of $T_x^{(k)}(X)$ defined in 13.2.6. We have:

$$
i_k(\Delta^\alpha_x)=0 \qquad \text{if } |\alpha|<k
$$

$$
i_k(\Delta^\alpha_x)=\gamma_{\alpha_1}(\partial_1,x)\cdots\gamma_{\alpha_n}(\partial_n,x)
\qquad \text{if } |\alpha|=k.
$$

[^1]

13.3.4. Suppose that K is of characteristic zero or that X is locally of finite dimension. Let k be an integer such that $0 \leq k \leq r$ and let $x \in X$; let F be a Banach space. By 12.6.8, we have an exact sequence

(i)
$$
0 \to P_k(T_x(X); F) \xrightarrow{i} P_x^k(F_X) \xrightarrow{\sigma} P_x^{k-1}(F_X) \to 0,
$$
with $\sigma = r^{k, k-1}$. On the other hand, by 13.3.1, we have an exact sequence

(ii)
$$
0 \leftarrow TS^k(T_x(X)) \xleftarrow{i} T_x^{(k)}(X) \xleftarrow{s} T_x^{(k-1)}(X) \leftarrow 0,
$$
where s is the inclusion of $T_x^{(k-1)}(X)$ in $T_x^{(k)}(X)$ and $i = i_k$. These exact sequences are “coupled in F”. More precisely, write them in the form:

(i)
$$
0 \to A \xrightarrow{i} B \xrightarrow{\sigma} C \to 0
$$

(ii)
$$
0 \leftarrow A' \xleftarrow{i} B' \xleftarrow{s} C' \leftarrow 0.
$$

If $a \in A$ and $a' \in A'$, the element $\langle a, a' \rangle$ of F is defined by 13.1.2; if $b \in B$ and $b' \in B'$, (resp. if $c \in C$ and $c' \in C'$), the element $\langle b, b' \rangle$ (resp. $\langle c, c' \rangle$) of F is defined by 13.2.2; we then have:
$$
\langle ia, b' \rangle = \langle a, ib' \rangle \quad \text{and} \quad \langle \sigma b, c' \rangle = \langle b, sc' \rangle \quad \text{if} \quad a \in A,\ b \in B,\ b' \in B',\ c' \in C'.
$$

13.3.5. Let Y be a variety of class $C^r$, let $\varphi : X \to Y$ be a morphism of class $C^r$ and let $x \in X,\ y \in Y$ be such that $y = \varphi(x)$. The mapping $\varphi_* : T_x^{(r)}(X) \to T_y^{(r)}(Y)$ defined in 13.2.3 is compatible with the filtrations of these spaces; it defines by passing to the associated graded spaces a linear mapping
$$
\operatorname{gr}(\varphi_*) : \operatorname{gr}\ T_x^{(r)}(X) \to \operatorname{gr}\ T_y^{(r)}(Y).
$$
On the other hand, let $TS^{(r)}(T_x(\varphi))$ be the mapping of $TS^{(r)}(T_x(X))$ into $TS^{(r)}(T_y(Y))$ induced by the canonical extension $TS(T_x(\varphi))$ of $T_x(\varphi)$. The diagram

$$
\begin{array}{ccc}
\operatorname{gr}\ T_x^{(r)}(X) & \xrightarrow{\operatorname{gr}(\varphi_*)} & \operatorname{gr}\ T_y^{(r)}(Y) \\
\downarrow^{i_{X,x}} & & \downarrow^{i_{Y,y}} \\
TS^{(r)}(T_x(X)) & \xrightarrow{TS^{(r)}(T_x(\varphi))} & TS^{(r)}(T_y(Y))
\end{array}
$$

is commutative.

13.3.6. Suppose that K is of characteristic zero. Using the isomorphisms $\varphi_M : S^k(M) \to TS^k(M)$ defined in A, IV, § 5, No. 8, we can replace, in all that precedes, the $TS^k(T_x(X))$ by the k-th symmetric powers $S^k(T_x(X))$ of the tangent space $T_x(X)$.

### 13.4. Tensor product of point distributions

13.4.1. Let $X_1$ and $X_2$ be two manifolds of class $C^r$, let $x_1 \in X_1,\ x_2 \in X_2$ and $t_1 \in T_{x_1}^{(k_1)}(X_1),\ t_2 \in T_{x_2}^{(k_2)}(X_2)$ with $k_1 + k_2 \leq r$. Put $X = X_1 \times X_2,\ x = (x_1, x_2)$ and k = k_1 + k_2. For i = 1, 2, let c_i = (U_i, \varphi_i, E_i) be a chart of X_i centred at x_i and denote by $\tilde{t}_i$ the element of TS(E_i) such that $\theta_c(\tilde{t}_i) = t_i$, cf. 13.2.1. Let $\sigma$ be the canonical isomorphism of TS(E_1) $\otimes$ TS(E_2) onto TS(E_1 $\times$ E_2), cf. A, IV, § 5, no. 5. The element $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ is the symmetric product of $\tilde{t}_1$ and $\tilde{t}_2$ (identified with elements of TS(E_1 $\times$ E_2) by means of the canonical injections TS(E_i) $\to$ TS(E_1 $\times$ E_2)); it belongs to TS^{(k)}(E_1 $\times$ E_2). Put $c = c_1 \times c_2$; this is a chart of X centred at x. The image by $\theta_c$ of $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ is an element of T_x^{(k)}(X), which does not depend on the choice of the charts $c_i$. It is called the direct product, or the symmetric tensor product (or simply the tensor product) of $t_1$ and $t_2$ and is denoted by $t_1 \times t_2$ or $t_1 \otimes t_2$.

We have $\varepsilon_{x_1} \otimes \varepsilon_{x_2} = \varepsilon_x$. The constant term of $t_1 \otimes t_2$ is the product of the constant terms of $t_1$ and $t_2$.

The isomorphism $(y_1, y_2) \mapsto (y_2, y_1)$ of $X_1 \times X_2$ onto $X_2 \times X_1$ transforms $t_1 \otimes t_2$ into $t_2 \otimes t_1$.

13.4.2 (« Associativity and functoriality »). Let $X_i$ ($i = 1, 2, 3$) be manifolds of class $C^r$, and let $x_i \in X_i$, $t_i \in T^{(k_i)}_{x_i}(X_i)$ with $k_1 + k_2 + k_3 \leq r$. We have
$$
(t_1 \otimes t_2) \otimes t_3 = t_1 \otimes (t_2 \otimes t_3);
$$
we denote this point distribution by $t_1 \otimes t_2 \otimes t_3$. Finite tensor products of any number of factors are defined analogously.

Let $\varphi_1 : X_1 \to Y_1$ and $\varphi_2 : X_2 \to Y_2$ be morphisms of manifolds of class $C^r$, and let $t_1 \in T^{(k_1)}(X_1)$, $t_2 \in T^{(k_2)}(X_2)$ with $k_1 + k_2 \leq r$. We have
$$
(\varphi_1 \times \varphi_2)_*(t_1 \otimes t_2) = \varphi_{1*}(t_1) \otimes \varphi_{2*}(t_2).
$$

13.4.3. The notation being that of 13.4.1, let $F_1, F_2$ and F be separated polynormed spaces, and let $(u_1, u_2) \mapsto u_1 . u_2$ be a continuous bilinear mapping of $F_1 \times F_2$ into F. Let
$$
f_i : X_i \to F_i \quad (i = 1, 2)
$$
be a mapping of class $C^r$, and define $f_1 \otimes f_2 : X \to F$ by
$$
(f_1 \otimes f_2)(y_1, y_2) = f_1(y_1) . f_2(y_2).
$$
The mapping $f_1 \otimes f_2$ is of class $C^r$, and we have
$$
\langle f_1 \otimes f_2, t_1 \otimes t_2 \rangle = \langle f_1, t_1 \rangle . \langle f_2, t_2 \rangle.
$$

13.4.4. The notation being that of 13.4.1, let $f$ be a mapping of class $C^r$ of X into a separated polynormed space F. If $y_1 \in X_1$, denote by $f_{y_1}$ the mapping $y_2 \mapsto f(y_1, y_2)$ of $X_2$ into F and put $g(y_1) = \langle f_{y_1}, t_2 \rangle$. The function $g : X_1 \to F$ thus defined is of class $C^{r - k_1}$, and we have
$$
\langle f, t_1 \otimes t_2 \rangle = \langle g, t_1 \rangle,
$$
in other words
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_1 \mapsto \langle y_2 \mapsto f(y_1, y_2), t_2 \rangle, t_1 \rangle.
$$
Analogously
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_2 \mapsto \langle y_1 \mapsto f(y_1, y_2), t_1 \rangle, t_2 \rangle.
$$

13.4.5. The notation being that of 13.4.1, let

$$
\alpha_{k_1, k_2} : T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2) \to T^{(k)}_x(X)
$$

be the linear mapping defined by the bilinear mapping $(t_1, t_2) \mapsto t_1 \otimes t_2$; this mapping is injective; it is bijective if $k_1$ and $k_2$ are infinite.

If $n \leq r$, denote by $T^{(n)}_x(X_1, X_2)$ the vector subspace of $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$ generated by the subspaces $T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2)$ for $k_1 + k_2 \leq n$. There exists one and only one linear mapping

$$
\alpha_n : T^{(n)}_x(X_1, X_2) \to T^{(n)}_x(X)
$$

extending the mappings $\alpha_{k_1, k_2}$ defined above; it is an isomorphism. In what follows, we identify $T^{(n)}_x(X)$, by means of $\alpha_n^{-1}$, with the vector subspace $T^{(n)}_x(X_1, X_2)$ of $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$.

13.4.6. Retain the notation of 13.4.5 and 13.3.1. By passing to the quotient, $\alpha_{k_1, k_2}$ defines a linear mapping

$$
\varepsilon_{k_1, k_2} : \operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2) \to \operatorname{gr}_k T^{(r)}_x(X).
$$

The mappings $\varepsilon_{k_1, k_2}$ ($k_1 + k_2 \leq r$) are the components of a graded linear mapping of degree zero

$$
\varepsilon : \bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) \to \bigoplus_{k \leq r} \operatorname{gr}_k T^{(r)}_x(X)
$$

which is an isomorphism. The diagram

$$
\begin{array}{ccc}
\bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(r)}_x(X) \\
\downarrow i_{12} & & \downarrow i_X \\
\bigoplus_{k_1 + k_2 \leq r} (\mathrm{TS}^{k_1}(T_{x_1}(X_1)) \otimes \mathrm{TS}^{k_2}(T_{x_2}(X_2))) & \xrightarrow{\sigma} & \bigoplus_{k \leq r} \mathrm{TS}^k(T_{x_1}(X_1) \times T_{x_2}(X_2))
\end{array}
$$

is commutative (in this diagram, $i_{12}$ denotes the homomorphism induced by $i_{x_1} \otimes i_{x_2}$ and $\sigma$ is the isomorphism defined in A, IV, § 5, No. 5). If $r$ is infinite, this diagram is simply written:

$$
\begin{array}{ccc}
\operatorname{gr} T^{(\infty)}_{x_1}(X_1) \otimes \operatorname{gr} T^{(\infty)}_{x_2}(X_2) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(\infty)}_x(X) \\
\downarrow i_{x_1} \otimes i_{x_2} & & \downarrow i_X \\
\mathrm{TS}(T_{x_1}(X_1)) \otimes \mathrm{TS}(T_{x_2}(X_2)) & \xrightarrow{\sigma} & \mathrm{TS}(T_x(X)).
\end{array}
$$

### 13.5. Coproducts

In this number, $X$ denotes a variety of class $C^r$ and $x$ a point of $X$.

13.5.1. Let $k \leq r$. If $\Delta$ is the diagonal mapping $y \mapsto (y, y)$ of $X$ into $X \times X$, then $\Delta_*$ maps $T^{(k)}_x(X)$ into $T^{(k)}_{(x,x)}(X \times X)$, which is a vector subspace of

$T^{(k)}_x(X)\otimes T^{(k)}_x(X)$, cf. 13.4.5. One thus obtains a linear mapping, again denoted by $\Delta_*$ (or $c$):

$$
T^{(k)}_x(X)\longrightarrow T^{(k)}_x(X)\otimes T^{(k)}_x(X);
$$

it is called the coproduct attached to $T^{(k)}_x(X)$. Endowed with this coproduct, $T^{(k)}_x(X)$ is a coassociative and cocommutative cogebra (A, III, p. 144-145); its counit is the linear form which associates to a point distribution its constant term (13.2.1).
If $k'\leq k$, the inclusion of $T^{(k')}_x(X)$ in $T^{(k)}_x(X)$ is a morphism of cogebras.
If $c=(U,\varphi,\overline{E})$ is a chart of $X$ centred at $x$, the isomorphism

$$
\theta_c:T^{(k)}(E)\longrightarrow T^{(k)}_x(X)
$$

is an isomorphism of cogebras, $T^{(k)}(E)$ being endowed with the coproduct induced by that of $T(E)$, cf. A, IV, § 5, no 7.
If $\varphi:X\longrightarrow Y$ is a morphism of manifolds of class $C^r$, the mapping of $T^{(k)}(X)$ into $T^{(k)}_{\varphi(x)}(Y)$ induced by $\varphi_*$ is a morphism of cogebras.

### 13.5.2. Let $F_1$, $F_2$ and $F$ be separated polynomial spaces, and $(u_1,u_2)\mapsto u_1.u_2$ a continuous bilinear mapping of $F_1\times F_2$ into $F$. Let $t\in T^{(r)}_x(X)$ and let

$$
c(t)=\sum_j u_j\otimes v_j\quad(u_j,v_j\text{ in }T^{(r)}_x(X))
$$

be its image by the coproduct. Let $f_i:X\longrightarrow F_i$ $(i=1,2)$ be mappings of class $C^r$. We have

$$
\langle f_1.f_2,t\rangle=\sum_j\langle f_1,u_j\rangle\langle f_2,v_j\rangle,
$$

which we write, by abuse of notation:

$$
\langle f_1.f_2,t\rangle=\langle f_1\otimes f_2,c(t)\rangle.
$$

### 13.5.3. Let $t\in T^{(k)}_x(X)$, where $k\leq r$.

a) For $c(t)=t\otimes 1$, it is necessary and sufficient that $t$ be equal to $0$ or to $\varepsilon_x$.

b) For $c(t)=1\otimes t+\varepsilon_x\otimes t$, it is necessary and sufficient that $t$ be a tangent vector, i.e. that $t\in T^{(1)}_x(X)$.

### 13.6. Distributions with finite support

### 13.6.1. Let $X$ be a manifold of class $C^r$, and let $k\leq r$. We denote by $\mathscr{T}^{(k)}(X)$ the direct sum of the spaces $T^{(k)}_x(X)$, for $x\in X$. An element of $\mathscr{T}^{(k)}(X)$ is called a distribution with finite support on $X$, of order $\leq k$. If $f:X\longrightarrow F$ is a function of class $C^r$ with values in a separated polynomial space $F$, and if

$$
t=\sum_{x\in X}t_x,
$$

where $t_x\in T^{(k)}_x(X)$ for all $x\in X$ is a distribution with finite support, we put

$$
\langle f,t\rangle=\sum_{x\in X}\langle f,t_x\rangle.
$$

Analogously, we put

$$
c(t)=\sum_{x\in X}c(t_x),
$$

which equips $\mathscr{T}^{(k)}(X)$ with a coassociative, cocommutative cogebra structure, possessing a counit $t\mapsto\langle1,t\rangle$. The inclusions

$$
\mathscr{T}^{(k')}(X)\longrightarrow\mathscr{T}^{(k)}(X),
$$

where $k'\leq k$, are cogebra morphisms.

If $\varphi : X \to Y$ is a morphism of varieties of class $C^r$, the mappings $T_x^{(k)}(\varphi) : T_x^{(k)}(X) \to T_{\varphi(x)}^{(k)}(Y)$ relative to the various points $x$ of $X$ define a linear mapping $\varphi_*$ of $\mathscr{T}^{(k)}(X)$ into $\mathscr{T}^{(k)}(Y)$, which is a cogebra morphism.

If $X_1$ and $X_2$ are two varieties of class $C^r$, the mappings $\alpha_k^{-1}$ (cf. 13.4.5) define a linear mapping
$$
\mathscr{T}^{(k)}(X_1 \times X_2) \to \mathscr{T}^{(k)}(X_1) \otimes \mathscr{T}^{(k)}(X_2)
$$
which is injective; it is a cogebra morphism. If $k = \infty$ or $\omega$, it is an isomorphism of cogebras.

13.6.2. Let $X$ be a variety of class $C^r$, and let $V$ be a $K$-vector space of finite dimension. An element of $\mathscr{T}^{(r)}(X) \otimes V$ is called a distribution with finite support on $X$ with values in $V$. When $K = \mathbf{R}$, $V = \mathbf{C}$, such a distribution is also called a complex distribution with finite support on $X$. The definitions and results of the preceding No.s extend immediately, by linearity, to distributions with values in $V$.

### 13.7. Weakening of structure

Suppose $K = \mathbf{R}$. Let $r' \in \mathbf{N}_K$ such that $r' \leq r$. Let $X$ be a variety of class $C^r$, and let $X'$ be the variety of class $C^{r'}$ obtained by weakening of structure (5.13.1). Let $x \in X$, and let $t \in T_x^{(k)}(X)$, with $k \leq r'$. Choose a chart $c = (U, \varphi, E)$ of $X$ centred at $x$, and let $\tilde{t}$ be the element of $TS^{(k)}(E)$ such that $\theta_c(\tilde{t}) = t$. Since $c$ is a chart of $X'$ centred at $x$, the element $t' = \theta_c(\tilde{t})$ of $T_x^{(k)}(X')$ is defined; it is independent of the choice of $c$. The mapping $t \mapsto t'$ is a bijection of $T_x^{(k)}(X)$ onto $T_x^{(k)}(X')$ by which these two spaces are identified. The identifications thus obtained are compatible with the operations $\langle f, t \rangle, \varphi_*(t), t_1 \otimes t_2, c(t), \ldots$ of the preceding No.s.

[^1]: Here again, the product of the $\gamma_{\alpha_i}(\partial_i,x)$ is a symmetric product in $TS(T_x(X))$.
