---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 9
section_title: Equations différentielles et feuilletages
lang: en
source: var-fr
pdf_pages: 0116-0125
extraction: ocr
subsections:
    - "no": 1
      title: Courbes intégrales
      page: 0
      pdf_page: 116
    - "no": 2
      title: Feuilletages
      page: 0
      pdf_page: 119
    - "no": 3
      title: Sous-fibrés intégrables
      page: 0
      pdf_page: 121
    - "no": 4
      title: Fibrés intégrables en caractéristique p ≠ 0
      page: 0
      pdf_page: 124
statements: 2
exercises: 0
content_sha256: e3c377f68c06b091929ac36db234b8f79caaef31ed09f6a129b1ece0caf8c8f1
translated_from: content/fr/var/2/09_s9_equations_differentielles_et.md
source_lang: fr
translation_method: machine
source_content_sha256: a65d2285e0ec3b5e8e51427bcedc796fffee8d546e725662827c97e254fda4a1
translation_model: gpt-5-6
translation_run: translate-en-mt-f70be58f
glossary_version: 34
glossary_terms_sha256: 2bafc16945a08bb62363a768a453ae9ef23f82271d655a04fedb1f7e5a758c86
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 9. Differential equations and foliations

In nos. $^{\mathrm{os}}$ 9.1, 9.2 and 9.3, K is assumed to be of characteristic 0. In no. $^\circ$ 9.4, K is assumed to be of characteristic $p \ne 0$.

### 9.1. Integral curves

In this no. $^\circ$, X denotes a variety of class $C^r$ and $\xi$ a vector field of class $C^s$ on X, with $r$, $s$ in $\mathbf{N}_K$, $s \leq r - 1$.

9.1.1. Let I be an open subset of K, and let $f : I \to X$ be a mapping of class $C^k$ ($k \in \mathbf{N}_K$, $k \leq r$) from I into X. For $t \in I$, we denote by $f'(t)$ the vector $T_t(f)(1) \in T_{f(t)}(X)$; this vector is sometimes called the velocity of $f$ at the instant $t$. When X is a Banach space, $f'(t)$ is the derivative of $f$ at $t$.

One says that $f$ is an integral curve of $\xi$ if one has

$$(1)\qquad f'(t)=\xi(f(t))$$

for all $t \in I$. Such a curve is of class $C^{s+1}$.

If $x$ is a point of X, one calls integral curve of $\xi$ with origin $x$ an integral curve $f : I \to X$ of $\xi$ such that $0 \in I$ and $f(0)=x$; for every $x \in X$, there exists an integral curve of $\xi$ with origin $x$, defined in a suitable open neighborhood of 0 in K.

If $f : I \to X$ is an integral curve of $\xi$ and if $a \in K$, the mapping $t \mapsto f(t-a)$ from $I+a$ into X is an integral curve of $\xi$.

Let $f_1 : I_1 \to X$ and $f_2 : I_2 \to X$ be two integral curves of $\xi$, and $t \in I_1 \cap I_2$. If $f_1(t)=f_2(t)$, the mappings $f_1$ and $f_2$ coincide in a neighborhood of $t$.

9.1.2 (« Flows »). Let W be an open set of $X \times K$. For every $x \in X$, denote by $W_x$ the set of $t \in K$ such that $(x,t) \in W$. An integral flow of $\xi$ with domain W is called a mapping $f$ of class $C^k$ ($k \leq r$) from W into X such that, for every $x \in X$, the mapping $f_x : W_x \to X$ defined by $f_x(t)=f(x,t)$ is an integral curve of $\xi$, and such that for $(x,0) \in W$ one has $f(x,0)=x$.

For every point $x \in X$, there exists an integral flow of $\xi$ of class $C^s$ whose domain is a neighbourhood of $(x,0)$ in $X \times K$. Two integral flows of $\xi$ defined in a neighbourhood of $(x,0)$ coincide on a neighbourhood of $(x,0)$.

Let $x \in X$ and let $f$ be an integral flow of $\xi$ whose domain W is a neighbourhood of (x, 0). There exists a neighbourhood V of (x, 0, 0) in X × K × K such that, if (x, t_1, t_2) ∈ V, one has
$$(x, t_1) \in W,\quad (f(x, t_1), t_2) \in W,\quad (x, t_1 + t_2) \in W$$
and
(2)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$
If X is paracompact, or if X is separated and K = R or C, there exists an integral flow of $\xi$ whose domain is a neighbourhood of X × {0}.

9.1.3 (« The real case »). We suppose that K = R and that X is separated. An *integral arc* of $\xi$ is any integral curve of $\xi$ whose domain is an open interval of R. Two integral arcs $f_1$ and $f_2$ of $\xi$, defined on intervals $I_1$ and $I_2$, and coinciding at a point of $I_1 \cap I_2$, coincide in $I_1 \cap I_2$.

For every point $x \in X$, there exists one and only one integral arc with origin x, $f_x : I_x \to X$, such that, for every integral arc $f : I \to X$ with origin x, one has $I \subset I_x$ and $f = f_x|I$. The arc $f_x$ is called *the maximal integral arc* of $\xi$ with origin x, and its domain $I_x$ is sometimes called *the interval of life* of the point x for the field $\xi$.

If $I_x = ] -a_-, a_+ [$ and if $a_+$ is finite, the restriction of $f_x$ to the interval $[0, a_+ [$ is a proper mapping of $[0, a_+ [$ into X. In particular, $f(t)$ has no limit when t tends to $a_+$.

9.1.4. With the notations and hypotheses of 9.1.3, the set $\Omega$ of pairs $(x, t) \in X \times \mathbf{R}$ such that $t \in I_x$ is open in $X \times \mathbf{R}$ and the mapping $f : \Omega \to X$ defined by $f(x, t) = f_x(t)$ is of class $C^s$; it is an integral flow of $\xi$ with domain $\Omega$.

The functions $\alpha_+$ and $\alpha_- : X \to ]0, +\infty]$ defined by $I_x = ] -\alpha_-(x), \alpha_+(x)[$ are lower semi-continuous. For $(x, t) \in \Omega$ and $y = f(x, t)$, one has $\alpha_+(y) = \alpha_+(x) - t$ and $\alpha_-(y) = \alpha_-(x) + t$.

If $t_1 \in I_x$ and if $t_2 \in I_{f(x, t_1)}$, one has $t_1 + t_2 \in I_x$ and
(3)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$

If the function $\alpha_+$ (resp. $\alpha_-$) is bounded below on X by a constant > 0, it is constant and equal to $+\infty$.

One has $\alpha_+ = \alpha_- = +\infty$ (in other words, one has $\Omega = X \times \mathbf{R}$) in each of the following cases:

(i) the field $\xi$ has compact support (for example if X is compact);
(ii) there exists a group of automorphisms of X, transitive, and preserving $\xi$;
*(iii) there exists on X a riemannian structure for which X is complete and $\xi$ bounded.*

If $\Omega = X \times \mathbf{R}$, the mapping $f : X \times \mathbf{R} \to X$ is a right operation law of class $C^s$ of the group variety $\mathbf{R}$ in the variety X, cf. 5.12.5.

9.1.5 (« The complex case »). One supposes that K = C and that X is separated. For every $a \in ]0, +\infty]$, denote by $D_a$ the open disk of center 0 and radius a in C. For every $x \in X$, there exists one and only one number $\rho(x) \in ]0, +\infty]$, one and only one integral curve $f_x : D_{\rho(x)} \to X$ with origin $x$ such that, for every $a \in ]0, +\infty]$ and every integral curve $f : D_a \to X$ with origin $x$, one has $a \leq \rho(x)$ and $f = f_x|D_a$.

For every $\lambda \in \mathbf{C}$, let $\alpha_\lambda(x)$ be the supremum of the interval of existence of $x$ for the vector field $\lambda \xi$ on the real variety deduced from $X$ by restriction of scalars. One has $\rho(x) = \inf_{|\lambda|=1} \alpha_\lambda(x)$.

The set $\Delta$ of pairs $(x, t) \in X \times \mathbf{C}$ such that $t \in D_{\rho(x)}$ is open in $X \times \mathbf{C}$ and the mapping $f$ from $\Delta$ into $X$ defined by $f(x, t) = f_x(t)$ is an integral flow of $\xi$. The function $\rho : X \to ]0, +\infty]$ is lower semi-continuous. For $(x, t) \in \Delta$ and $y = f(x, t)$, one has $\rho(y) \geq \rho(x) - |t|$. If $\rho$ is bounded below on $X$ by a constant $> 0$, one has $\rho = +\infty$ and $\Delta = X \times \mathbf{C}$.

When $\Delta = X \times \mathbf{C}$, the mapping $f : X \times \mathbf{C} \to X$ is a right operation law of the group variety $\mathbf{C}$ on the variety $X$.

9.1.6. Let $\varphi : X \to Y$ be a morphism of varieties and $\eta$ a vector field on $Y$ such that $\xi$ is $\varphi$-related to $\eta$ (cf. 8.2.6). If $f : I \to X$ is an integral curve of $\xi$, the mapping $\varphi \circ f : I \to Y$ is an integral curve of $\eta$. If $K = \mathbf{R}$ and if $X$ and $Y$ are separated, for every $x \in X$, the interval of existence of $x$ for $\xi$ is contained in the interval of existence of $\varphi(x)$ for $\eta$. If, moreover, $\varphi$ is proper, these intervals are equal.

9.1.7 (“Time-dependent equations”). Let $W$ be an open subset of $X \times K$ and let $\Xi : W \to T(X)$ be a $C^s$ lifting of $\mathrm{pr}_1 : W \to X$, that is, a mapping of class $C^s$ from $W$ into $T(X)$ such that $\Xi(x, t)$ belongs to $T_x(X)$ for every $(x, t) \in W$. An integral curve of $\Xi$ is a mapping $f$ of class $C^k$ (with $k \in \mathbf{N}_K$ and $k \leq r$), from an open subset $I$ of $K$ into $X$ such that, for every $t \in I$, one has

$$
(f(t), t) \in W \text{ and } f'(t) = \Xi(f(t), t).
$$

Let $\eta$ be the vector field of class $C^s$ on $W$ defined by $\eta(x, t) = (\Xi(x, t), (t, 1))$. For a mapping $f$ from an open subset $I$ of $K$ into $X$ to be an integral curve of $\Xi$, it is necessary and sufficient that $t \mapsto (f(t), t)$ be an integral curve of $\eta$ in the sense of 9.1.1.

Let $g : I \to W$ be an integral curve of $\eta$ and $t_0$ a point of $I$ such that $\mathrm{pr}_2(g(t_0)) = t_0$. The set of elements $t \in I$ such that $\mathrm{pr}_2(g(t)) = t$ is a neighbourhood of $t_0$ which coincides with $I$ if $I$ is connected.

9.1.8 (“Parameters and initial conditions”). Let $Z$ be a variety of class $C^r$, let $W$ be an open subset of $X \times K \times Z$, and let $\Xi$ be a $C^s$ lifting of $\mathrm{pr}_1 : W \to X$ (8.6.1). If $z \in Z$, we denote by $W_z$ the set of $(x, t) \in X \times K$ such that $(x, t, z) \in W$, and we denote by $\Xi_z$ the mapping $(x, t) \mapsto \Xi(x, t, z)$ from $W_z$ into $T(X)$.

Let $(x_0, t_0, z_0)$ be a point of $W$. There then exists an open neighbourhood $X_1 \times I_1 \times Z_1$ of $(x_0, t_0, z_0)$ in $W$ and a mapping of class $C^s$

$$
f : X_1 \times I_1 \times I_1 \times Z_1 \to X
$$

such that, for every $(x_1, t_1, z_1) \in X_1 \times I_1 \times Z_1$, the mapping $t \mapsto f(x_1, t_1, t, z_1)$ is an integral curve of $\Xi_{z_1}$ (in the sense of 9.1.7) satisfying the relation $f(x_1, t_1, t_1, z_1) = x_1$.

Two mappings

$$
f_1 : X_1 \times I_1 \times I_1 \times Z_1 \to X \quad \text{and} \quad f_2 : X_2 \times I_2 \times I_2 \times Z_2 \to X
$$

satisfying the above conditions coincide in a neighbourhood of $(x_0, t_0, t_0, z_0)$.

### 9.2. Foliations

In this No., X denotes a variety of class $C^r$, with $r \in \mathbf{N}_K$. Unless otherwise stated, all varieties and all morphisms considered are assumed to be of class $C^r$.

9.2.1. Let S be a variety, and let $p : X \to S$ be a submersion. For each $s \in S$, endow $X_s = p^{-1}(s)$ with the variety structure induced by that of X (5.10.5); the set X is the disjoint union of the $X_s$. Denote by $X_p$ the variety structure on X obtained by gluing the $X_s$, for $s \in S$ (5.2.4); it is the unique variety structure on X for which the $X_s$ are open subvarieties. The topological space $X_p$ is the sum of the spaces $X_s$.

Let V be a variety and $f$ a mapping from V into X. For $f$ to be a morphism from V into $X_p$, it is necessary and sufficient that $f$ be a morphism from V into X and that $p \circ f$ be locally constant.

9.2.2. A foliation of X is called a variety Y having the same underlying set as X and satisfying the following condition:

(F) For every $x \in X$, there exists an open subvariety U of X containing x, a variety S and a submersion $p : U \to S$ such that the variety $U_p$ is an open subvariety of Y.

The pair (X, Y) is also called a foliated variety. If (X, Y) and (X', Y') are foliated varieties, a morphism from (X, Y) into (X', Y') is any mapping $f : X \to X'$ which is both a morphism of the variety X into the variety X' and a morphism of the variety Y into the variety Y'.

Let (X, Y) be a foliated variety. The identity mapping $Y \to X$ is a bijective immersion. A subset U of X is called a leaf if it is an open set of Y; in this case, U is endowed with the topological structure and the variety structure induced by those of Y; for example, U is said to be a connected leaf if it is an open and connected subset of Y. The leaves which are subvarieties of X form a basis of the topology of Y. When $K = \mathbf{R}$ or $\mathbf{C}$, the connected components of Y are leaves, called maximal connected leaves of (X, Y).

9.2.3. If $s \in \mathbf{N}_K, s \leq r$, a foliation of class $C^s$ of X is called a foliation of the variety of class $C^s$ underlying X.

9.2.4. Examples

a) The variety X is a foliation of X, called the coarse foliation of X.

b) If $p : X \to S$ is a submersion, $X_p$ is a foliation of X, called the foliation of X defined by p. The foliation of X defined by the identity mapping is the set X endowed with its purely variety structure of dimension 0 (5.2.1); it is called the discrete foliation of X.

c) Let E be a Banach space, F a closed vector subspace of E having a topological complement, and $p$ the canonical projection $E \to E/F$. The foliation $E_p$ of E is called the foliation of E defined by F.

d) Let $\Gamma$ be a discrete group acting properly and freely on the topological space $X$ (TG, III, § 4, n° 4). Let $Y$ be a foliation of $X$, and suppose that, for every $s \in \Gamma$, the mapping $x \mapsto sx$ is an automorphism of $(X, Y)$. The equivalence relation on $X$ (resp. $Y$) whose classes are the orbits of $\Gamma$ is regular (5.9.5). If $X/\Gamma$ (resp. $Y/\Gamma$) is denoted the corresponding quotient variety, the pair $(X/\Gamma, Y/\Gamma)$ is a foliated variety, called the quotient of $(X, Y)$ by $\Gamma$.

9.2.5. Let $Y$ be a foliation of $X$ and $U$ an open subset of $X$. Then $U$ is open in $Y$ and $U$, endowed with the structure of variety induced by that of $Y$, is a foliation of $X$, called the foliation induced by $Y$.

More generally, let $f : X' \to X$ be a morphism such that $f$ and the identity mapping $Y \to X$ form a transversal pair (5.11.1). The fibred product $Y' = X' \times_X Y$ identifies canonically with a foliation of $X'$ called the inverse image foliation of $Y$ by $f$.

9.2.6. Let $p : X \to S$ and $p' : X' \to S'$ be two submersions, and let $f$ be a morphism from $X$ to $X'$. In order that $f$ be a morphism from $X_p$ to $X_{p'}$, it is necessary and sufficient that, for every $x \in X$, there exist an open neighbourhood $U$ of $x$ in $X$ and a morphism $g$ from $p(U)$ to $S'$ such that $g \circ p = p' \circ f$ on $U$.

9.2.7. Let $Y$ be a foliation of $X$. A foliated chart of $(X, Y)$ is called a quadruple $(U, \varphi, E, F)$ such that $(U, \varphi, E)$ is a chart of $X$, that $F$ is a closed vector subspace of the Banach space $E$ admitting a topological complement and that $\varphi$ is an isomorphism of the foliation of $U$ induced by $Y$ onto the foliation of $\varphi(U)$ defined by the canonical mapping of $E$ onto $E/F$. For every point $x \in X$, there exists a foliated chart $(U, \varphi, E, F)$ of $(X, Y)$ such that $x \in U$. Let $n = \dim_x X$ and let $m = \dim_x Y$. If $n$ is finite, there exists an open neighbourhood $U$ of $x$ and a system of coordinates $\zeta^1, \ldots, \zeta^n$ of $X$ on $U$ such that the foliation of $U$ induced by $Y$ coincides with the foliation defined by the mapping $(\zeta^{m+1}, \ldots, \zeta^n)$ of $U$ into $K^{n-m}$.

9.2.8. Let $Y$ be a foliation of $X$. When $x$ runs through $X$, the spaces $T_x(Y)$ are the fibres of a vector subbundle of class $C^{r-1}$ of $T(X)$ which is called the subbundle of $T(X)$ tangent to the foliation $Y$ and which is denoted by $T(X, Y)$. If the foliation $Y$ is defined by a submersion $p : X \to S$, then $T(X, Y) = \mathrm{Ker}\, T(p)$ is the relative tangent bundle $T(X/S)$ of $X$ over $S$ (8.1.3).

Let $(X, Y)$ and $(X', Y')$ be two foliated manifolds, and let $f$ be a morphism of $X$ into $X'$. For $f$ to be a morphism of foliated manifolds, it is necessary and sufficient that $T(f)$ map $T(X, Y)$ into $T(X', Y')$. In particular, let $f : Z \to X$ be a morphism of manifolds; for $f$ to be a morphism of $Z$ into $Y$, it is necessary and sufficient that $T(f)$ map $T(Z)$ into $T(X, Y)$. For a submanifold $Z$ of $X$ to be a leaf of $(X, Y)$, it is necessary and sufficient that

$$
T_z(Z) = T_z(X, Y) \quad \text{for all } z \in Z.
$$

Let $Y$ be a foliation of $X$ and let $U$ be a leaf of $Y$, having a countable basis of open sets. Let $Z$ be a manifold and $f$ a mapping of $Z$ into $U$. For $f$ to be a morphism of manifolds from Z into U, it is necessary and sufficient that the composite of f and the canonical injection of U into X be a morphism of manifolds from Z into X. If X is locally compact and countable at infinity, every connected leaf of (X, Y) has a countable basis of open sets (cf. TG, I, 3e éd., §11, No. 7, cor. 2 du th. 1).

9.2.9. Suppose that K = R or C. Let Y be a foliation of X. The following conditions are equivalent:

a) There exists a manifold S and a submersion $p : X \to S$ such that $Y = X_p$.

b) For every $x \in X$, there exists a submanifold $S_x$ of X possessing the following two properties:
   b₁) The tangent space $T_x(S_x)$ to $S_x$ at $x$ is a topological supplement of $T_x(X, Y)$ in $T_x(X)$.
   b₂) Every connected leaf of (X, Y) meets $S_x$ in at most one point.

Suppose these conditions are satisfied and let $R \{x, y\}$ be the relation on X “x and y belong to the same connected leaf”; then R is a regular equivalence relation (5.9.5) on X, and, if p denotes the canonical projection $X \to X/R$, one has $Y = X_p$.

#### Example {#var-2-s9-n2-exa-1 .statement}

Let $K = R$ and $X = R^2$. Let the discrete group $\Gamma = Z^2$ operate on X by translations. Let $m \in R$ and let $(X, Y_m)$ be the foliation defined by the submersion $p : (x_1, x_2) \mapsto x_2 - mx_1$ of X onto R. Put $X' = X/\Gamma$ and $Y'_m = Y_m/\Gamma$; then $Y'_m$ is a foliation of the torus $X'$ (cf. 9.2.4, example d)). If m is rational, there exists a submersion $p'$ of $X'$ onto $R/Z$ such that $Y'_m = X'_{p'}$. If m is irrational, every maximal connected leaf of $(X', Y'_m)$ is dense in $X'$, and there does not exist a submersion $p'$ of $X'$ into a manifold S such that $Y'_m = X'_{p'}$.

9.2.10. Let Y be a foliation of X, and let $\pi : X \to S$ be a morphism of manifolds such that the composite $Y \to X \xrightarrow{\pi} S$ is étale. If S’ is an open subset of S, a section $\sigma : S' \to X$ of $\pi$ over S’ is said to be horizontal (with respect to the foliation Y) if it is a morphism from S’ into Y; it amounts to saying that $\sigma(S')$ is a leaf of (X, Y), or again that $T(\sigma)$ maps $T(S')$ into $T(X, Y)$. For every $s_0 \in S$ and every $x_0 \in \pi^{-1}(s_0)$, there exists a horizontal section defined in a neighbourhood of $s_0$ and taking the value $x_0$ at $s_0$; two such sections coincide on a neighbourhood of $s_0$.

More generally, let $s_0 \in S$, let T be a manifold, let f be a morphism from T into the submanifold $\pi^{-1}(s_0)$ of X, and let $t_0 \in T$. There then exists an open neighbourhood T’ (resp. S’) of $t_0$ in T (resp. of $s_0$ in S), and a morphism
$$
F : S' \times T' \to X
$$
satisfying the following condition: for every $t \in T'$, the mapping $s \mapsto F(s, t)$ is a horizontal section of $\pi$ over S’ taking the value $f(t)$ at the point $s_0$. Two such mappings F coincide on a neighbourhood of $(s_0, t_0)$.

### 9.3. Integrable subbundles

In this no., X denotes a manifold of class $C^r$ and F a vector subbundle of class $C^s$ of $T(X)$, with $r, s$ in $N_K, s \leq r - 1$.

9.3.1. Let V be a manifold of class $C^k$ ($k \in \mathbf{N}_K, k \leq r$) and let $f$ be a morphism of class $C^k$ from V into X. One says that $f$ is an integral of F if $T(f)$ maps $T(V)$ into F.

A submanifold Z of class $C^k$ of X is called an integral submanifold of F if the injection $Z \to X$ is an integral of F in the above sense, i.e. if one has $T_x(Z) \subset F_x$ for all $x \in Z$.

Let $x \in X$. If $Z_1$ and $Z_2$ are two integral submanifolds of X containing $x$ and if $T_x(Z_1) = F_x$, there exists a neighbourhood U of $x$ such that $U \cap Z_2 \subset Z_1$. If in addition $T_x(Z_2) = F_x$, the germs of $Z_1$ and $Z_2$ at $x$ coincide.

9.3.2. We say that F is integrable if there exists a foliation Y of X of class $C^s$ such that $F = T(X, Y)$ (9.2.8). Such a foliation is then unique; it is called the integral foliation of F. In order that a morphism $f : V \to X$ of class $C^s$ be an integral of F, it is necessary and sufficient that $f$ be a morphism of V into Y.

#### Example {#var-2-s9-n3-exa-1 .statement}

If F has rank 1 at every point, F is integrable, and defines on X a pure foliation of dimension 1. Suppose in addition that $K = \mathbf{R}$, that X is separated, and that F has as a frame a vector field $\xi$ everywhere nonzero. Then, for every $x \in X$, the maximal connected leaf containing $x$ is the image of the maximal integral arc of $\xi$ with origin $x$ (9.1.3).

9.3.3 (« Integrability Criteria »). The following conditions are equivalent:

(i) The vector subbundle F of $T(X)$ is integrable.

(ii) For every $x \in X$, there exists an integral submanifold Z of class $C^s$ of F such that $x \in Z$ and $T_x(Z) = F_x$.

(iii) Whatever the open set U of X and the vector fields $\xi$ and $\eta$ belonging to $\mathscr{J}_F^s(U)$ (7.4.1), one has $[\xi, \eta] \in \mathscr{J}_F^{s-1}(U)$.

Let $(\xi_i)_{i \in I}$ be a family of sections of F of class $C^s$ such that, for every $x \in X$, the set of the $\xi_i(x)$ is a total subset of the Banach space $F_x$ (EVT, I, § 2, No. 1). The conditions (i), (ii), (iii) are then equivalent to:

(iv) for every pair $(i, j)$ of elements of I, and every $x \in X$, one has $[\xi_i, \xi_j](x) \in F_x$.

When I is finite, and the family $(\xi_i)$ is a frame of F, the preceding conditions are also equivalent to:

(v) there exists a family $(c_{ij}^k)_{(i, j, k) \in I \times I \times I}$ of functions on X with values in K such that $[\xi_i, \xi_j] = \sum_k c_{ij}^k \xi_k$ for all $i, j$ in I.

(If this is the case, the functions $c_{i,j}^k$ are of class $C^{s-1}$.)

9.3.4. Let $s' \in \mathbf{N}_K$, with $s' \leq s$, and let $F'$ be the vector bundle of class $C^{s'}$ deduced from F by weakening of structure (8.7.1). In order that F be integrable, it is necessary and sufficient that $F'$ be so. In this case, the integral foliation of $F'$ is deduced from that of F by weakening of structure.

9.3.5. Let E be a Banach space and $p$ an integer $\geq 0$. For every $x \in X$, let us denote

N(p, E)_x the vector subspace of Alt^p(T_x(X); E) formed by the elements u such that $u(v_1, \ldots, v_p) = 0$ for $v_1, \ldots, v_p$ in $F_x$. The spaces N(p, E)_x, for $x \in X$, are the fibres of a vector subbundle of class C^s of Alt^p(T(X); E). Let us denote it by N(p, E). If F is integrable, we have:

(vi) for every open U of X and every form $\omega \in \mathscr{S}_{N(p, E)}^s(U)$, one has $d\omega \in \mathscr{S}_{N(p+1, E)}^{s-1}(U)$.

Conversely, if (vi) is satisfied for $p = 1$ and for every Banach space E, the bundle F is integrable; when K = R or C, it is even enough to verify (vi) for $p = 1$ and E = K.

Suppose that the dual of T(X)/F admits a frame $(\omega_1, \ldots, \omega_n)$. The integrability of F is then equivalent to the following condition:

(vii) $d\omega_i \wedge \omega_1 \wedge \cdots \wedge \omega_n = 0$ for $1 \leq i \leq n$.

If in addition there exists a vector subbundle G of class C^s of T(X) such that T(X) is the direct sum of F and G, condition (vii) is equivalent to:

(viii) there exist differential forms $\alpha_i^j$ (i, j in I) of degree 1 on X, of class C^{s-1}, such that $d\omega_i = \sum_j \alpha_i^j \wedge \omega_j$ for all $i \in I$.

9.3.6. Let L be a Banach space and let $\omega$ be a differential form of degree 1 on X with values in L, of class C^s. We make the following two hypotheses:

a) for every $x \in X$, $\omega_x$ is a surjective homomorphism from $T_x(X)$ into L, and the kernel of $\omega_x$ is $F_x$;
b) there exists a vector subbundle G of T(X) such that T(X) is the direct sum of F and G.

The integrability of F is then equivalent to:

(ix) there exists a differential form $\alpha$ of degree 1 on X with values in End(L) such that $d\omega = \alpha \wedge \omega$, the exterior product being defined by the canonical pairing End(L) $\times$ L $\to$ L (7.8.2 and 8.3.2).

9.3.7 (« Equations in total differentials »). Suppose that X is the product of two manifolds A and B of class C^r; denote by $p_1 : X \to A$ and $p_2 : X \to B$ the two projections. Let f be a morphism of class C^s from $p_1^*T(A)$ into $p_2^*T(B)$. The graphs of the mappings $f_{(a, b)} : T_a(A) \to T_b(B)$ are the fibres of a vector subbundle of class C^s of T(X); denote it by F^f.

Let A’ be an open subset of A, and let $\varphi : A' \to B$ be a morphism of class C^k ($k \in \mathbf{N}_K, k \leq r$). We say that $\varphi$ is an integral of f if, for every $a \in A'$, one has $T_a(\varphi) = f_{a, \varphi(a)}$; this is equivalent to saying that the mapping $a \mapsto (a, \varphi(a))$ from A’ into X is an integral of F^f (9.3.1). Such a mapping is of class C^{s+1}. If $\varphi_1$ and $\varphi_2$ are two integrals of f and take the same value at a point $a \in A$, they coincide in a neighbourhood of a.

More generally, let Z be a manifold of class C^k, let A’ be an open subset of A, let $a \in A'$ and let $\Phi_1, \Phi_2$ be morphisms of class C^k from Z $\times$ A’ into B. Suppose that

Φ₁ and Φ₂ coincide on Z × {a} and that, for every z ∈ Z, the morphisms
$$
a \mapsto \Phi_1(z, a) \quad \text{and} \quad a \mapsto \Phi_2(z, a)
$$
are integrals of f. Then Φ₁ and Φ₂ coincide in a neighbourhood of Z × {a}.

Suppose that F^f is integrable. Let Z be a manifold of class C^k (k ∈ N_K, k ≤ s), let (z₀, a₀) be a point of Z × A, and let ρ be a morphism of class C^k from Z into B. There exists an open neighbourhood Z' × A' of (z₀, a₀) in Z × A and a morphism Φ : Z' × A' → B of class C^k such that, for every z ∈ Z', the mapping a ↦ Φ(z, a) from A' into B has f as its tangent mapping and takes the value ρ(z) at the point a₀.

9.3.8. Retain the hypotheses and notations of 9.3.7 and suppose that A (resp. B) is an open submanifold of a Banach space E (resp. M). The mapping f is then identified with a morphism of class C^s from X = A × B into the Banach space $\mathscr{L}(E; M)$. Denote by D₁f (resp. D₂f) the first (resp. second) partial derivative of f (1.6.2); this is a morphism of class C^{s-1} from X into $\mathscr{L}(E; \mathscr{L}(E; M))$ (resp. into $\mathscr{L}(M; \mathscr{L}(E; M))$), a space which is identified in the obvious way with $\mathscr{L}_2(E; M)$ (resp. with $\mathscr{L}(M, E; M)$). For F to be integrable, it is necessary and sufficient that, for every x ∈ X, the bilinear mapping
$$
\Delta_x : (h_1, h_2) \mapsto D_1f(x)(h_1, h_2) + D_2f(x)(f(x)h_1, h_2)
$$
from E × E into M be symmetric. Under this condition, if φ is an integral of f defined in an open subset A' of A, the second derivative of φ at a point a of A' is $\Delta_{(a, \varphi(a))}$.

If E = K^n, and if we denote by (x¹, ..., xⁿ) the coordinate functions on K^n, the mapping f is defined by a family (f₁, ..., fₙ) of mappings from A × B into M, and the integrability condition is written:
$$
\frac{\partial f_i}{\partial x^j} + (D_2f_i) \cdot f_j = \frac{\partial f_j}{\partial x^i} + (D_2f_j) \cdot f_i
$$
whatever the integers i, j in {1, n}. A mapping φ from an open subset A' of A into B is an integral of f if and only if one has
$$
\frac{\partial \varphi}{\partial x^i} = f_i(x, \varphi(x)) \quad \text{pour tout } x \in A' \text{ et tout } i \in \{1, n\},
$$
in other words, if one has
$$
d\varphi = \sum_{1 \leq i \leq n} f_i(x, \varphi(x)) \, dx^i.
$$

### 9.4. Integrable bundles in characteristic p ≠ 0

In this no., K is assumed to have characteristic p ≠ 0. Let X be a K-analytic manifold locally of finite dimension.

9.4.1 (« p-th Powers »). Let ξ be a vector field on an open subset U of X. There exists one and only one vector field ξ^p on U such that
$$
D_{\xi^p}(f) = (D_\xi)^p(f) = \underbrace{D_\xi(D_\xi(\ldots(D_\xi(f))\ldots))}_{p \text{ times}}
$$
for every analytic function f defined in an open subset of U.

If $\varphi$ is an analytic function on $U$, one has
$$
(\varphi \xi)^p = \varphi^p \xi^p + (\mathrm{D}_{\varphi \xi})^{p-1}(\varphi) \cdot \xi
$$
and if $\eta$ is a vector field on $U$, one has
$$
[\xi^p, \eta] = \mathrm{ad}(\xi)^p(\eta) = [\xi, [\xi, \ldots, [\xi, \eta]\ldots]].
$$

9.4.2 (« Jacobson Identity »). Let $L$ be the free $F_p$-Lie algebra (LIE, II, § 2, No. 2) on a set $\{x, y\}$ with two elements. There exists one and only one element $\Lambda_p(x, y)$ of $L$ such that one has
$$
(x + y)^p = x^p + y^p + \Lambda_p(x, y)
$$
in the enveloping algebra of $L$. Examples:
$$
\Lambda_2(x, y) = [x, y]; \quad \Lambda_3(x, y) = [x, [x, y]] - [y, [x, y]].
$$
If $\xi$ and $\eta$ are vector fields on $X$, one has
$$
(\xi + \eta)^p = \xi^p + \eta^p + \Lambda_p(\xi, \eta).
$$

9.4.3. *Example.* — Let us take $X = K$ (resp. $K^*$) and denote by $x$ the canonical mapping $X \to K$. Let $\xi$ (resp. $\eta$) be the vector field $\partial / \partial x$ (resp. $x \cdot \partial / \partial x$); it is invariant under the translations of the additive (resp. multiplicative) group $X$. One has
$$
\xi^p = 0 \quad \text{and} \quad \eta^p = \eta.
$$

9.4.4 (« Integrable bundles »). Let $F$ be a vector subbundle of $T(X)$. We say that $F$ is *integrable* if, for every $x \in X$, there exists a system of coordinates $(\zeta^1, \ldots, \zeta^n)$ of $X$ at $x$ and an integer $m \leq n$ such that $(\partial / \partial \zeta^1, \ldots, \partial / \partial \zeta^m)$ is a frame of $F$ in a neighbourhood of $x$.
For $F$ to be integrable, it is necessary and sufficient that it satisfy the following condition:
*For every open set $U$ of $X$, $\mathscr{S}_F^\omega(U)$ is a Lie subalgebra of $\mathscr{S}_{T(X)}^\omega(U)$ stable under the operation $\xi \mapsto \xi^p$.*
