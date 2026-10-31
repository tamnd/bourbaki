---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 15
section_title: Variétés d’applications
lang: en
source: var-fr
pdf_pages: 0174-0180
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions de classe $C^{r,s}$
      page: 0
      pdf_page: 174
    - "no": 2
      title: Variété de classe $C^{r,s}$ au-dessus d’une variété de classe $C^r$
      page: 0
      pdf_page: 176
    - "no": 3
      title: Variétés de sections et variétés d’applications
      page: 0
      pdf_page: 178
statements: 0
exercises: 0
content_sha256: 20c4e2333445f2264703c72388bb9d2747fd98e25d5adf1f72012ea48360267e
translated_from: content/fr/var/2/15_s15_varietes_d_applications.md
source_lang: fr
translation_method: google
source_content_sha256: 47894c25c40367c68b455261d80abc0b0ca0569826499d939d8b09720496f1ec
translation_model: google-translate
translation_quality: low
translation_run: translate-en-mt-05be1646
glossary_version: 34
glossary_terms_sha256: ddbd5ffda9cdad0d5aeeeda563c381c69b73cbb532987a711feb63cbd81175fe
prompt_sha256: 319f34f48397471bcb54ffcda78e44eabf7ce41db1e47352727fbb4621669210
---

## § 15. Varieties of applications[^1]

In this paragraph, we assume $K=\mathbf{R}$ or $\mathbf{C}$. The letter $r$ designates an integer $\geq 1$ and the letter $s$ an element of $\mathbf{N}_K$ such as $s\geq r$; we have $s=\omega$ if $K=\mathbf{C}$.

### 15.1. Class functions $C^{r,s}$

In this number, $E$ designates a real Banach space, $F_1$ and $F_2$ Banach spaces on $K$, $V$ an open of $E\times F_1$ and $f$ a map of $V$ in $F_2$. We equip $E$, $F_1$ and $F_2$ with norms compatible with their Banach space structures.

### 15.1.1 (“Differentiable Case”).

We assume $K=\mathbf{R}$ and $s\neq\omega$. We say that $f$ is of class $C^{r,s}$ (or simply $C^{r,s}$) if it has continuous iterated partial derivatives $D_E^pD_{F_1}^qf$ (1.7.2) for any pair of positive integers $(p,q)$ such as $p\leq r$ and $p+q\leq s$. It is the same to say that the iterated partial derivatives $D_{F_1}^qf$ exist and are of class $C^r$ for any integer $q$ such as $0\leq q\leq s-r$. If $s=r$, this is equivalent to saying that $f$ is of class $C^r$; if $s\geq r+1$, this is equivalent to saying that $f$ is of class $C^r$ and $D_{F_1}f$ of class $C^{r,s-1}$.

If $f$ is of class $C^{r,s}$, and if $p\leq r$, $p+q+1\leq s$, the function $D_E^pD_{F_1}^qf$ has a partial derivative with respect to $F_1$ given by:

$$
D_{F_1}(D_E^pD_{F_1}^qf)=D_E^pD_{F_1}^{q+1}f.
$$

### 15.1.2 (“Analytical case”).

We assume $s=\omega$. For any integer $k\geq 0$, let $P_k(F_1;F_2)$ be the space of homogeneous continuous polynomials of degree $k$ on $F_1$ with values ​​in $F_2$, provided with the norm defined in the Appendix of the first fascicle, p. 88, A.2.

We say that $f$ is of class $C^{r,\omega}$ (or simply $C^{r,\omega}$ if there is no ambiguity about $K$) if, for any point $(x_0,y_0)\in V$, there exists a neighborhood $U$ of $x_0$ in $E$, real numbers $R>0$ and $M\geq 0$ and functions $h_k:U\to P_k(F_1;F_2)$ ($k\in\mathbf{N}$), of class $C^r$ (for the differential manifold structure underlying the K-manifold structure of $P_k(F_1; F_2)$), such that:

(i) $U \times (y_0 + B(R)) \subset V$, where $B(R)$ is the open ball of radius $R$ in $F_1$;

(ii) if $x \in U$ and $p \leq r$, we have $\sum_{k=0}^{\infty} \| D^p h_k(x) \| R^k \leq M$;

(iii) if $x \in U$ and $t \in B(R)$, we have $\sum_{k=0}^{\infty} h_k(x)(t) = f(x, y_0 + t)$.

These properties result in:

(iv) For all $t \in B(R)$, the function $x \mapsto f(x, y_0 + t)$ is of class $C^r$ in $U$, and we have

$$
D_E^p f(x, y_0 + t) = \sum_{k=0}^{\infty} D^p h_k(x)(t) \quad \text{si } p \leq r \text{ et } x \in U.
$$

We do not change the definition of class functions $C^{r,\omega}$ if we replace condition (ii) above by one of the following two conditions:

(ii’) The $h_k$ define a class morphism $C^r$ of $U$ in the real Banach space underlying the Banach K-space $\mathscr{H}_R(F_1; F_2)$ (3.1.1 and 3.1.2).

(ii’’) The $h_k$ define a class morphism $C^r$ of $U$ in the real Banach space underlying the Banach K-space $\tilde{\mathscr{H}}_R(F_1; F_2)$ (3.1.5).

15.1.3. Suppose $K = \mathbf{R}$. For $f$ to be of class $C^{r,\omega}_R$, it is necessary and sufficient that $f$ be of class $C^{r,\infty}$ (15.1.1) and that, for all $(x_0, y_0) \in V$, there exists a neighborhood $V_0$ of $(x_0, y_0)$ in $V$ and positive real numbers $A$ and $M$ such that

$$
\frac{1}{q!} \| D_E^p D_{F_1}^q f(x, y) \| \leq A \cdot M^q
$$

for all $p \leq r$, all $q \geq 0$ and all $(x, y) \in V_0$.

15.1.4. Suppose $K = \mathbf{C}$. For $f$ to be of class $C^{r,\omega}_C$, it is necessary and sufficient that the following two conditions are verified:

a) $f$ is of class $C^{r,\omega}_R$ for the real structures underlying $F_1$ and $F_2$.

b) For all $(x, y) \in V$, $D_{F_1} f(x, y)$ is a $\mathbf{C}$-linear map of $F_1$ into $F_2$.

When $F_1$ is of finite dimension, we can replace a) by:

a’) $f$ is of class $C^r$.

15.1.5. The set of applications of class $C^{r,s}$ of $V$ in $F_2$ does not depend on the choose of standards on $E, F_1, F_2$.

15.1.6. Let $B$ be a differential variety of class $C^r$, let $W$ be an open of $B \times F_1$, and let $\rho$ be a map of $W$ into $F_2$. Let $c = (U, \varphi, E_c)$ be a card of the variety $B$. Let us denote $W_c$ the opening of $E_c \times F_1$ image by $\varphi \times \mathrm{Id}_{F_1}$ of $W \cap (U \times F_1)$ and $\rho_c$ the application of $W_c$ in $F_2$ such that

$$
\rho_c(\varphi(x), y) = \rho(x, y) \quad \text{si } (x, y) \in W \cap (U \times F_1).
$$

The application $\rho : W \to F_2$ is said to be of class $C^{r,s}$ if, for any card $c$ of the variety $B$, the application $\rho_c : W_c \to F_2$ is of class $C^{r,s}$ within the meaning of 15.1.1 and 15.1.2; it is enough that this condition is fulfilled for a family of cards whose domains cover $B$. Such a $\rho$ map is of class $C^r$ (for the underlying real structures of $B \times F_1$ and $F_2$); its restriction to the set $W \cap (\{b\} \times F_1)$ is a K-morphism of class $C^s$ for all $b \in B$.

15.1.7. Let $B_1$ and $B_2$ be differential varieties of class $C^r$, and $g : B_1 \to B_2$ be a morphism of class $C^r$. Let $W_1$ (resp. $W_2$) be an open of $B_1 \times F_1$ (resp. of $B_2 \times F_2$) and let $h$ be an application of $W_1$ in $W_2$. We say that $h$ is a $g$-morphism of class $C^{r,s}$ if $pr_1 \circ h = g \circ pr_1$ and if $pr_2 \circ h$ is a map of class $C^{r,s}$ (15.1.6) of $W_1$ into $F_2$.

Likewise, let $B_3$ be a variety of class $C^r$, $W_3$ be an open of $B_3 \times F_3$, where $F_3$ is a Banach K-space, and $g'$ be a morphism of class $C^r$ of $B_2$ into $B_3$. If $h$ (resp. $h'$) is a $g$-morphism (resp. $g'$-morphism) of class $C^{r,s}$ of $W_1$ in $W_2$ (resp. of $W_2$ in $W_3$), the compound $h' \circ h$ is a $(g' \circ g)$-morphism of class $C^{r,s}$ from $W_1$ into $W_3$.

### 15.2. Class variety $C^{r,s}$ above a class variety $C^r$

Throughout this number, we note $B$ a differential variety of class $C^r$.

15.2.1. Let $X$ be a set equipped with an application $p : X \to B$. We call a map of $X$ above $B$ a triplet $\theta = (V, \psi, F)$, where $V$ is a subset of $X$, $F$ a Banach K-space, and $\psi$ a bijection of $V$ on an open of $B \times F$ such than $pr_1 \circ \psi = p|V$.

Let $(\theta_i)_{i \in I} = ((V_i, \psi_i, F_i))_{i \in I}$ be a family of cards from $X$ above $B$. We say that the $\theta_i$ are $C^{r,s}$-compatible if, for any pair of elements $i, j$ of $I$, the following two conditions are satisfied:

a) $\psi_i(V_i \cap V_j)$ is open in $B \times F_i$ and $\psi_j(V_i \cap V_j)$ is open in $B \times F_j$;
b) the map $\psi_i \circ \psi_j^{-1}$ of $\psi_j(V_i \cap V_j)$ in $\psi_i(V_i \cap V_j)$ is a $\mathrm{Id}_B$-morphism of class $C^{r,s}$ (15.1.7).

A $((V_i, \psi_i, F_i))_{i \in I}$ family of maps of $X$ above $B$ that are $C^{r,s}$-compatible and whose domains $V_i$ overlap $X$ is called a $C^{r,s}$-atlas of $X$ (above $B$). Two $C^{r,s}$-atlases are said to be equivalent if their union is a $C^{r,s}$-atlas; the $C^{r,s}$-equivalence relation between atlases is an equivalence relation. An equivalence class of $C^{r,s}$-atlas is called a manifold structure of class $C^{r,s}$ above $B$ on the set $X$; when you want to specify $K$, you write $C_K^{r,s}$ instead of $C^{r,s}$. If $X$ is a variety of class $C^{r,s}$ above $B$, we say that $p : X \to B$ is the projection of $X$; if $\theta$ is a map of $X$ above $B$, we say that $\theta$ is a map of the $C^{r,s}$-variety $X$ if $\theta$ belongs to an atlas of the equivalence class defining the structure of $X$.

15.2.2. Let $X$ be a variety of class $C^{r,s}$ above $B$, of projection $p$. There exists on $X$ a structure of differential manifold of class $C^r$ and only one, such that, for any map $(V, \psi, F)$ of the $C^{r,s}$-manifold $X$, the set $V$ is open in $X$ and that $\psi$ is an $C^r$-isomorphism of the open submanifold $V$ of $X$ on the open submanifold $\psi(V)$ of $B \times F$. If we equip $X$ with this structure, the application $p : X \to B$ is a submergence of class $C^r$.

Let $b \in B$ and let $X_b = p^{-1}(b)$. There exists a structure of $K$-variety of class $C^s$ on $X_b$, and only one, such that, for any map $\theta = (V, \psi, F)$ of the $C^{r,s}$-variety $X$, the triplet $\theta_b = (V \cap X_b, \operatorname{pr}_2 \circ \psi|_{(V \cap X_b)}, F)$ is a map of the variety $X_b$. The differential manifold structure of class $C^r$ underlying this structure is induced by the differential manifold structure of class $C^r$ over $X$ defined above.

15.2.3. Examples

(i) When $B$ is reduced to a point, the notion of variety of class $C_K^{r,s}$ above $B$ is equivalent to that of $K$-variety of class $C^s$.

(ii) Let $Z$ be a $K$-manifold of class $C^s$; let's take $X = B \times Z$ and $p = \operatorname{pr}_1$. There exists on $X$ a structure of variety of class $C^{r,s}$ above $B$, and only one, such that, for any card $(U, \psi, L)$ of $Z$, $(B \times U, \operatorname{Id}_B \times \psi, L)$ is a card of $C^{r,s}$-variety $X$.

(iii) Let $X$ be a variety of class $C^{r,s}$ above $B$, and $Y$ be an open of $X$. The class variety structure $C^{r,s}$ of $Y$ *induced* by that of $X$ is defined as in the case of varieties (cf. 5.2.3).

(iv) Let $M$ be a vector bundle on $K$ with base $B$ and class $C^r$ (7.3.4), and let $\pi$ be its projection on $B$. There exists on $M$ a structure of variety of class $C_K^{r,\omega}$ above $B$, and only one, such that, if $(U, \psi, F)$ is a $K$-vector map of $M$ (8.8.1), the triplet $(\pi^{-1}(U), \psi, F)$ is a map of the $C_K^{r,\omega}$-manifold $M$.

15.2.4. Let $X$ be a variety of class $C^{r,s}$ above $B$, $p$ its projection, $L$ a $K$-Banach space, and $f$ a map of $X$ into $L$. We say that $f$ is of class $C^{r,s}$ if, for any map $(V, \psi, F)$ of the $C^{r,s}$-variety $X$, the map $(f|V) \circ \psi^{-1}$ of $\psi(V)$ in $L$ is of class $C^{r,s}$ (15.1.6). Such an application is of class $C^r$ and its restriction to $X_b$ for $b \in B$, is of class $C^s$.

15.2.5. Let $g : B \to B'$ be a morphism of differential varieties of class $C^r$, let $X$ (resp. $X'$) be a variety of class $C^{r,s}$ above $B$ (resp. $B'$), and let $h$ be an application of $X$ into $X'$. We say that $h$ is a *g-morphism of class* $C^{r,s}$ if the following three conditions are satisfied:

a) $p' \circ h = g \circ p$;
b) $h$ is continuous;
c) for any card $(V', \psi', F')$ of the $C^{r,s}$-variety $X'$, the application $\operatorname{pr}_2 \circ \psi' \circ h$ of $V = h^{-1}(V')$ in $F'$ is of class $C^{r,s}$ (in the sense of 15.2.4) when we equip the open $V$ with the structure induced by that of $X$ (15.2.3, (iii)).

When $B = B'$ and $g = \operatorname{Id}_B$, we also say that $h$ is a *B-morphism of class* $C^{r,s}$.

For a B-morphism of class $C^{r,s}$ to be a B-isomorphism of class $C^{r,s}$, it suffices that it be an isomorphism of class $C^1$.

Let $g': B' \to B''$ be a morphism of varieties of class $C^r$ and let $X''$ be a variety of class $C^{r,s}$ above $B''$. If $h: X \to X'$ is a $g$-morphism of class $C^{r,s}$ and $h': X' \to X''$ is a $g'$-morphism of class $C^{r,s}$, then $h' \circ h$ is a $(g' \circ g)$-morphism of class $C^{r,s}$.

15.2.6. Let $X$ be a class variety $C^{r,s_j}_R$ above $B$ and $p$ its projection; we assume $s \neq \omega$, $X$ separated and $p$ proper (TG, I, § 10, n° 1). Then, for any $b \in B$, there exists an open neighborhood $U$ of $b$ and a $C^{r,s}$-isomorphism of $p^{-1}(U)$ on $U \times X_b$, where $X_b = p^{-1}(b)$.

15.2.7. Let $X$ be a variety of class $C^{r,s}_K$ above $B$, $p$ its projection, and $\sigma : B \to X$ a section of class $C^r$. We call *tubular neighborhood* of class $C^{r,s}_K$ of $\sigma$ a triplet $(M, N, \varphi)$ where $M$ is a $K$-vector bundle, of base $B$ and of class $C^r$, $N$ is an open neighborhood of $\sigma(B)$ into $X$, and $\varphi$ is a $B$-isomorphism of class $C^{r,s}_K$ of $N$ over an open of $M$ (cf. 15.2.3 (iv)), transforming the section $\sigma$ into the null section of $M$.

Suppose that $s \geq r + 1$ and that the variety $B$ is paracompact and admits partitions of the class unity $C^r$ (5.3.6); there then exist tubular neighborhoods of class $C^{r,s}_K$ of $\sigma$.

### 15.3. Varieties of sections and varieties of applications

15.3.1 (“Structure of Banach space on a space of sections”). Let $B$ be a *compact* differential variety of class $C^r$; let $M$ be a vector bundle on $K$ (7.3.4) with base $B$ and class $C^r$; let $M_r$ be the differential manifold of class $C^r$ underlying $M$, and let $\mathscr{S}_M^r(B)$ be the $K$-vector space of sections of class $C^r$ of $M$ (7.4.1). The topology induced on $\mathscr{S}_M^r(B)$ by the topology of the $C^r$-uniform convergence of $\mathscr{C}^r(B; M_r)$ (12.3.10) makes $\mathscr{S}_M^r(B)$ a $K$-*Banach space*.

Let $(U_i)_{i \in I}$ be a *finite* open covering of $B$ and, for all $i \in I$, let $c_i = (U_i, \varphi_i, E_i)$ be a map of $B$ and $t_i = (U_i, \psi_i, F_i)$ be a $K$-vector map of $M$ (8.8.1). Let us equip each of the $E_i$ (resp. $F_i$) with a norm compatible with its Banach space structure on $\mathbf{R}$ (resp. $K$) and let $(V_i)_{i \in I}$ be a closed covering of $B$, such that $V_i \subset U_i$ for all $i \in I$. For $f \in \mathscr{S}_M^r(B)$ and $i \in I$, let $f_i$ be the application of $\varphi_i(U_i)$ in $F_i$ obtained by composition:

$$
\varphi_i(U_i) \xrightarrow{\phi_i^{-1}} U_i \xrightarrow{f} M|U_i \xrightarrow{\psi_i} U_i \times F_i \xrightarrow{\mathrm{pr}_2} F_i.
$$

Let's ask
$$
\|f\| = \operatorname{Sup}_{i \in I,\ p \leq r,\ x \in V_i} \|D^p f_i(\varphi_i(x))\|.
$$
The map $f \mapsto \|f\|$ is a *norm* on $\mathscr{S}_M^r(B)$, which defines the Banach space structure on $K$ of $\mathscr{S}_M^r(B)$.

If $N$ is an open in space $M$, the set $\mathscr{S}^r(B; N)$ of sections $f \in \mathscr{S}_M^r(B)$ such that $f(B) \subset N$ is open in $\mathscr{S}_M^r(B)$.

15.3.2. Let $B$ be a compact differential variety of class $C^r$, and let $X$ be a variety of class $C^{r,s}_K (s \geq r + 1)$ above B. If N is an open of X, let $\mathscr{S}'(B; N)$ be the set of sections of class $C^r$ of There exists on $\mathscr{S}'(B; X)$ a K-manifold structure of class $C^{s-r}$, and only one, such that, for any section $\sigma \in \mathscr{S}'(B; X)$ and any tubular neighborhood $(M, N, \varphi)$ of class $C^{r,s}_K$ of $\sigma$ (15.2.7), the triplet $(\mathscr{S}'(B; N), \varphi^*, \mathscr{S}'_M(B))$, where $\varphi^*$ is the map $f \mapsto \varphi \circ f$, i.e. a map of the K-manifold $\mathscr{S}'(B; X)$.

In what follows, we equip $\mathscr{S}'(B; X)$ with this structure.

15.3.3. Let X be a compact differential variety of class $C^r$, and let Y be a K-manifold of class $C^s (s \geq r + 1)$. Soit $\mathscr{C}^r(X; Y)$ l’ensemble des applications de classe $C^r$ de X dans Y (autrement dit, à valeurs dans la variété de classe $C^r$ sous-jacente à Y, cf. 5.13.1 et 5.14.2). We provide $\mathscr{C}^r(X; Y)$ with the K-manifold structure of class $C^{s-r}$ obtained by identifying it with $\mathscr{S}'(X; X \times Y)$, cf. 15.2.3, (ii) and 15.3.2. We call it the variety of maps of class $C^r$ from X to Y. Its topology is that of $C^r$-uniform convergence (12.3.10).

Let Y be separated; it is then the same for $\mathscr{C}^r(X; Y)$. Moreover, the set of immersions (resp. embeddings, submersions, surjective submersions, splayed morphisms, isomorphisms) of class $C^r$ of X in Y is an open of $\mathscr{C}^r(X; Y)$.

Let $X'$ be a compact differential variety of class $C^r$, $\varphi : X' \to X$ be a morphism of differential varieties of class $C^r$ and $\psi : Y \to Y'$ be a morphism of K-manifolds of class $C^s$. The map $f \mapsto \psi \circ f \circ \varphi$ is a class morphism $C^{s-r}$ from $\mathscr{C}^r(X; Y)$ into $\mathscr{C}^r(X'; Y')$.

15.3.4 (“Structural weakening”). Let us keep the hypotheses and notations of 15.3.3. Let $s' \in \mathbf{N}_R$ with $r < s' \leq s$ and let $Y_{s'}$ be the real variety of class $C^{s'}$ underlying Y (5.13 and 5.14.2). The real manifold structure of class $C^{s'-r}$ of $\mathscr{C}^r(X; Y_{s'})$ underlies the K-manifold structure of class $C^{s-r}$ of $\mathscr{C}^r(X; Y)$.

15.3.5. Let X and $X'$ be compact differential varieties of class $C^r$ and $C^{r'}$ respectively, with $r' < r$; and let Y be a K-manifold of class $C^s$, with $s \geq r + 1$. Or $t = \operatorname{Inf}(r - r', s - r)$. The map $(f, g) \mapsto g \circ f$ is a class morphism $C^t$ from $\mathscr{C}^{r'}(X'; X) \times \mathscr{C}^r(X; Y)$ into $\mathscr{C}^{r'}(X'; Y)$.

15.3.6 (“Space tangent to $\mathscr{C}^r(X; Y)$”). The hypotheses being those of 15.3.3, let $f \in \mathscr{C}^r(X; Y)$ and let $\xi$ be a tangent vector in $f$ to the variety $\mathscr{C}^r(X; Y)$. If $x \in X$, let $\varepsilon_x$ be the application $g \mapsto g(x)$ of $\mathscr{C}^r(X; Y)$ in Y; it is a morphism of class $C^{s-r}$. The image by $T_f(\varepsilon_x)$ of $\xi$ is an element $\xi_x$ of $T_{f(x)}(Y)$; the map $x \mapsto \xi_x$ is a raising of class $C^r$ of $f$ in $T(Y)$ (cf. 8.6.1) and we can identify it with a section of class $C^r$ of the vector bundle $f^*T(Y)$ of base X. We obtain in this way an isomorphism of the tangent space $T_f(\mathscr{C}^r(X; Y))$ on the Banach space $\mathscr{S}'_{f^*T(Y)}(X)$.

15.3.7 (“Interpretation of $\mathscr{C}^p(X; \mathscr{C}^q(Y; Z))$”). Soient X et Y des variétés différentielles compactes de classe $C^p$ et $C^q$ respectivement ($1 \leq p \leq +\infty, 1 \leq q < +\infty$), et soit Z une K-variété de classe $C^s$, avec $s \geq p + q$. Let $f : X \times Y \to Z$ be a continuous application; for all $x \in X$, let $f_x$ be the application $y \mapsto f(x, y)$ of $Y$ in $Z$. The following two properties are equivalent:

a) Whatever the cards $c = (U, \varphi, E)$ of $X$, $d = (V, \psi, F)$ of $Y$ and $e = (W, \theta, G)$ of $Z$ such as $f(U \times V) \subset W$, the partial derivatives $D_E^{p'} D_F^{q'} f'$ of the expression $f'$ of $f$ in the cards $c \times d$ and $e$ (5.3.2) exist and are continuous for $p' \leq p$ and $q' \leq q$.

b) For all $x \in X$, the map $f_x$ is of class $C^q$ and the map $x \mapsto f_x$ is a morphism of class $C^p$ of $X$ in the variety $\mathscr{C}^q(Y ; Z)$.

15.3.8. Let $Y$ be a $K$-compact variety of class $C^s$, with $s \geq r + 1$, and let $\mathrm{Diff}'(Y)$ be the automorphism group of class $C^r$ of the real variety $Y_r$, of class $C^r$ underlying $Y$. The set $\mathrm{Diff}'(Y)$ is open in $\mathscr{C}^r(Y ; Y) = \mathscr{C}^r(Y_r ; Y)$; we provide it with the structure of $K$-variety of class $C^{s-r}$ induced by that of $\mathscr{C}^r(Y ; Y)$. The composition law $(f, g) \mapsto g \circ f$ makes $\mathrm{Diff}'(Y)$ a topological group. On the other hand, the class variety structure $C^{s-r}$ is not generally compatible with the group structure of $\mathrm{Diff}'(Y)$. For $f \in \mathrm{Diff}'(Y)$, the mapping $g \mapsto g \circ f$ of $\mathrm{Diff}'(Y)$ into itself is of class $C^{s-r}$, but the mapping $g \mapsto f \circ g$ is not in general of class $C^1$. In particular, $\mathrm{Diff}'(Y)$ is not in general a Lie group.$^{(1)}$

$^1$ Suppose $s = \infty$. Let $\mathrm{Diff}^\infty(Y)$ be the group of class automorphisms $C^\infty$ of $Y$; let us provide it with the least fine topology making the canonical injections $\mathrm{Diff}^\infty(Y) \to \mathrm{Diff}'(Y)$ continuous for any integer $r \geq 1$. On the other hand, let $\mathrm{Diff}^0(Y)$ be the group of homeomorphisms of $Y$, equipped with the topology of uniform convergence (TG, X, § 3, n° 5, prop. 11). If dim $Y \geq 1$, it is impossible to find a Lie group $G$ and continuous homomorphisms of $\mathrm{Diff}^\infty(Y)$ in $G$ and of $G$ in $\mathrm{Diff}^0(Y)$ whose compound is the canonical injection (cf. LIE, III, § 4, exerc. 7).

[^1]: The definitions and results of this paragraph extend without essential modifications to the case where the Banach space $E$ of n° 15.1 is replaced by a closed half-space and to the case where the variety $B$ of n° 15.1.6 to 15.3.2 (resp. the variety $X$ of n° 15.3.3) is replaced by a coin of a variety (11.1.2). In particular, the space of maps of class $C^r$ of segment $\{0,1\}$ in a $K$-manifold $Y$ of class $C^s$ ($s>r$) has a natural structure of $K$-manifold of class $C^{r,s}$. Another possible generalization consists of replacing $E$ and $B$ (resp. $X$) by topological spaces (resp. by a compact topological space) and taking $r=0$. Thus, if $X$ is a compact space and $Y$ a $K$-manifold of class $C^s$, the set $C^0(X;Y)$ of continuous maps of $X$ in $Y$ has a natural structure of $K$-manifold of class $C^s$ (the underlying topology being that of uniform convergence). We leave it to the reader to develop these brief indications.
