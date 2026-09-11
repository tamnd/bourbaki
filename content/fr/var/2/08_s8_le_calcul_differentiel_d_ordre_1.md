---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 8
section_title: Le calcul différentiel d’ordre 1
lang: fr
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
content_sha256: 8e5eb0df8ca06a478d639eada2c7d5b89876793e8c3fe822ad7724a41e0f6db2
---

## § 8. Le calcul différentiel d’ordre 1

A partir du no 8.3, on suppose

— soit que $K$ est de caractéristique zéro,

— soit que les variétés considérées sont localement de dimension finie.

Dans ce dernier cas, les expressions «espace de Banach, fibré vectoriel, foncteur vectoriel» signifient respectivement «espace vectoriel de dimension finie, fibré vectoriel de rang fini, foncteur vectoriel en dimension finie à valeurs de dimension finie».

### 8.1. Fibré tangent

### 8.1.1. — Soit $r\in \mathbf{N}_K$ et soit $X$ une $K$-variété de classe $C^r$. On note $T(X)$ l’ensemble somme des espaces tangents $T_x(X)$ (5.5.1) pour $x\in X$, et $\pi$ l’application canonique de $T(X)$ sur $X$. Soit $c=(U,\varphi,E)$ une carte de la variété $X$; pour $x\in U$ et $t\in T_x(X)$, posons $\zeta_c(x,t)=(x,\theta_c^{-1}(t))$, l’application $\theta_c$ étant celle définie en 5.5.1. Le triplet $c'=(U,\zeta_c,E)$ est une carte vectorielle (7.1.1) de $T(X)$ (muni de l’application $\pi:T(X)\longrightarrow X$). Il existe sur $T(X)$ une structure de fibré vectoriel de base $X$ et de classe $C^{r-1}$ et une seule, telle que, pour toute carte $c$ de $X$, la carte vectorielle $c'$ correspondante soit une carte vectorielle de $T(X)$[^1]. Muni de cette structure, $T(X)$ est appelé le fibré tangent de $X$. En particulier, $T(X)$ est muni d’une structure de variété de classe $C^{r-1}$ et le triplet $(T(X),X,\pi)$ est une fibration (7.1.4).

Soit $U$ un ouvert d’un espace de Banach $E$ et soit $i$ l’injection canonique de $U$ dans $E$. La carte vectorielle $c'=(U,\zeta_c,E)$ associée à la carte $c=(U,i,E)$ de $U$ définit un isomorphisme de $T(U)$ sur le fibré trivial $E_U$ (7.1.5); on identifie ces deux fibrés au moyen de cet isomorphisme.

Si $X$ est une variété pure de type $E$ (5.1.7), $T(X)$ est une variété pure de type $E\times E$.

### 8.1.2. — Soit $f:X\longrightarrow Y$ un morphisme de variétés de classe $C^r$. On définit un $f$-morphisme $T(f):T(X)\longrightarrow T(Y)$ de fibrés vectoriels de classe $C^{r-1}$ par
$$
T(f)(x,t)=(f(x),T_xf(t))
$$
pour $x\in X$ et $t\in T_x(X)$.

Si $f=\mathrm{Id}_X$, on a $T(f)=\mathrm{Id}_{T(X)}$. Pour $f:X\longrightarrow Y$ et $g:Y\longrightarrow Z$, on a
$$
T(g\circ f)=T(g)\circ T(f).
$$

### 8.1.3. — Soit $f:X\longrightarrow Y$ un morphisme de variétés de classe $C^r$, et soit $f':T(X)\longrightarrow f^*T(Y)$

l’unique X-morphisme tel que T(f) = g ∘ f', où g est le morphisme canonique f*T(Y) → T(Y) (cf. 7.2.4).

Pour que f soit une immersion (resp. une submersion), il faut et il suffit que 0 → T(X) $\xrightarrow{f'} f^*T(Y)$ (resp. T(X) $\xrightarrow{f'} f^*T(Y) \to 0$) soit une suite exacte localement directe (7.5.6). Si f est une immersion, le fibré conoyau de f' est appelé fibré normal ou transverse de f. Si f est une submersion, le fibré noyau de f est appelé fibré tangent aux fibres de f, ou fibré tangent relatif de X sur Y, et noté T(X/Y). Sa fibre T_x(X/Y) en x ∈ X est l’espace tangent en x à la sous-variété $f^{-1}(f(x))$ de X. La suite

$$
0 \longrightarrow T_x(X/Y) \xrightarrow{i} T_x(X) \xrightarrow{T_{x(f)}} T_{f(x)}(Y) \longrightarrow 0
$$

où i est l’injection canonique, est exacte.

Pour que f soit étale, il faut et il suffit que f' soit un isomorphisme.

Lorsque K est de caractéristique 0, pour que f soit une subimmersion, il faut et il suffit que f' soit localement direct.

8.1.4. Soient X_1 et X_2 deux variétés. On a T(X_1 × X_2) = p_1^*T(X_1) ⊕ p_2^*T(X_2), où p_1 et p_2 sont les projections canoniques (5.6.3).

8.1.5. Soit n un entier $\geqslant 0$; le fibré tangent T(K^n) de K^n s’identifie au fibré trivial de fibre K^n (8.1.1). Les sections constantes définies par les éléments de la base canonique de K^n forment un repère de T(K^n).

Si X est une variété et (u^1, ..., u^n) un système de coordonnées de X dans un ouvert U de X (5.1.10), le repère précédent définit par transport de structure un repère de T(X) sur U; on l’appelle le repère tangent défini par (u^1, ..., u^n) et on le note (\partial/\partial u^1, ..., \partial/\partial u^n) (cf. 5.5.8).

### 8.2. Champs de vecteurs

Soit X une variété de classe C^r, et soit U un ouvert de X.

8.2.1. Une section (non nécessairement continue, cf. Notations et Conventions) du fibré tangent T(X) au-dessus de U s’appelle un champ de vecteurs sur U.

8.2.2. Le fibré dual T'(X) (7.7.3) de T(X) s’appelle le fibré cotangent de X. Ses sections s’appellent champs de covecteurs. Si f est une fonction de classe C^k sur X (avec 1 ≤ k ≤ r), à valeurs dans K, sa différentielle df : x ↦ d_x f (5.5.6) est un champ de covecteurs de classe C^{k-1}. Plus généralement, si f est une fonction de classe C^k sur X (1 ≤ k ≤ r), à valeurs dans un espace de Banach E, sa différentielle df est une section de classe C^{k-1} du fibré $\mathscr{L}(T(X); E_X)$.

8.2.3. Soit $\xi$ un champ de vecteurs de classe C^{r-1} sur X, et soit $f \in \mathscr{C}^r(X; F)$ une fonction de classe C^r à valeurs dans un espace de Banach F. On note $\langle \xi, df \rangle$, ou D_\xi(f), ou encore $\xi(f)$ la fonction $x \mapsto d_x f(\xi(x))$; c’est un élément de $\mathscr{C}^{r-1}(X; F)$. Pour f fixée, l’application $\xi \mapsto D_\xi(f)$ est $\mathscr{C}^{r-1}(X)$-linéaire. Si $D_\xi f = 0$ pour toute fonction f de classe C^r à valeurs dans un espace de Banach, définie dans un ouvert de X, on a $\xi = 0$.

Soient E, F, G des espaces de Banach et soit (u, v) ↦ u . v une application bilinéaire continue de $E \times F$ dans $G$. Soient $f \in \mathscr{C}^r(X; E)$, $g \in \mathscr{C}^r(X; F)$ et soit $f.g \in \mathscr{C}^r(X; G)$ leur produit. Si $\xi$ est un champ de vecteurs de classe $C^{r-1}$ sur $X$, on a
$$
D_\xi(f.g) = D_\xi(f).g + f.D_\xi(g).
$$
En particulier, l’application $D_\xi : \mathscr{C}^r(X) \to \mathscr{C}^{r-1}(X)$ est une dérivation de l’algèbre $\mathscr{C}^r(X)$ dans le $\mathscr{C}^r(X)$-module $\mathscr{C}^{r-1}(X)$.

8.2.4. Supposons que $X$ soit localement de *dimension finie* et que l’une des deux hypothèses suivantes soit vérifiée:

(i) $r = \infty$ et $X$ est séparée;
(ii) $r = \omega$ et $X$ est isomorphe à un polydisque ouvert de $K^n$.

Alors, pour toute dérivation $D$ de l’algèbre $\mathscr{C}^r(X)$, il existe un champ de vecteurs $\xi$ de classe $C^r$ et un seul tel que $D = D_\xi$.

8.2.5. Soient $(u^1, \ldots, u^n)$ un système de coordonnées de $X$ dans $U$, et $\xi$ un champ de vecteurs sur $U$. La $i$-ième coordonnée de $\xi$ dans le repère tangent (8.1.5) défini par $(u^1, \ldots, u^n)$ est $D_\xi(u^i)$. Autrement dit, on a
$$
\xi = \sum_{1 \leq i \leq n} D_\xi(u^i) \cdot \partial/\partial u^i.
$$

8.2.6. Soient $\varphi : X \to Y$ un morphisme de variétés de classe $C^r$, $\xi$ un champ de vecteurs sur $X$ et $\eta$ un champ de vecteurs sur $Y$. On dit que $\xi$ est $\varphi$-*lié* à $\eta$ si, pour tout $x \in X$, on a $\eta(\varphi(x)) = T_x(\varphi)(\xi(x))$. Supposons qu’il en soit ainsi, et que $\xi$ et $\eta$ soient de classe $C^{r-1}$. Alors, pour tout espace de Banach $E$, le diagramme

$$
\begin{array}{ccc}
\mathscr{C}^r(Y; E) & \xrightarrow{\varphi^*} & \mathscr{C}^r(X; E) \\
\downarrow D_\eta & & \downarrow D_\xi \\
\mathscr{C}^{r-1}(Y; E) & \xrightarrow{\varphi^*} & \mathscr{C}^{r-1}(X; E)
\end{array}
$$

où $\varphi^*(f) = f \circ \varphi$, est commutatif.

Lorsque $\varphi$ est étale, pour tout champ de vecteurs $\eta$ sur $Y$, il existe un champ de vecteurs et un seul sur $X$ qui est $\varphi$-lié à $\eta$; on le note $\varphi^*\eta$.

8.2.7. Soit $\varphi : X \to Y$ un morphisme de variétés de classe $C^r$. Si $\omega$ est un champ de covecteurs$^{(1)}$ sur $Y$, on définit un champ de covecteurs $\varphi^*\omega$ sur $X$ par
$$
(\varphi^*\omega)(x) = t(T_x(\varphi))(\omega(\varphi(x))) \quad (x \in X).
$$
Plus généralement, soit $\tau$ un foncteur vectoriel (7.6) de classe $C^{r-1}$, de type $(I_+, I_-)$ avec $I_+ = \emptyset$ et $I_-$ réduit à un élément (un tel foncteur est dit *contravariant*). Si $\omega$ est une section de classe $C^{r-1}$ du fibré vectoriel $\tau(T(Y))$ de base $Y$, on définit une section $\varphi^*\omega$ de $\tau(T(X))$ par $(\varphi^*\omega)(x) = \tau(T_x(\varphi))(\omega(\varphi(x)))$ $(x \in X)$.

$^1$ Le lecteur aura soin de ne pas confondre cet emploi de la lettre $\omega$ avec celui défini dans les Notations et Conventions.

### 8.3. Formes différentielles, différentiation extérieure

Rappelons que, dans ce numéro et les suivants, on suppose, ou bien que K est de caractéristique 0, ou bien que les variétés considérées sont localement de dimension finie.

8.3.1. Soient X une variété de classe C' et F un fibré vectoriel de classe C^k de base X, avec k + 1 \in \mathbf{N}_K et k + 1 \leq r. Soit p un entier \geq 0 et soit Alt^p(T(X); F) le fibré vectoriel de classe C^k des applications p-linéaires alternées de T(X) dans F (7.8.1 et Errata au n° 7.8). Une section de ce fibré au-dessus d’un ouvert U de X s’appelle une forme différentielle alternée (ou simplement forme différentielle) de degré p sur U, à valeurs dans F. Celles de ces sections qui sont de classe C^k forment un \mathscr{C}^k(U)-module, noté ^k\Omega^p(U; F). Si E est un espace de Banach, on écrit ^k\Omega^p(U; E) au lieu de ^k\Omega^p(U; E_X) et on parle de formes différentielles à valeurs dans E. Dans ces notations, on omet parfois k (resp. E) lorsqu’il est égal à r − 1 (resp. K).

Une forme différentielle de degré 0 (resp. 1) à valeurs scalaires est une fonction (resp. un champ de covecteurs).

Soit \varphi : Y \to X un morphisme de variétés de classe C', et soit \omega \in ^k\Omega^p(X; F). Il existe alors une forme \varphi^*\omega \in ^k\Omega^p(Y; \varphi^*F) et une seule telle que

(1)
$$(\varphi^*\omega)_y(v_1, \ldots, v_p) = \omega_{\varphi(y)}(T_y(\varphi).v_1, \ldots, T_y(\varphi).v_p)$$

pour tout y \in Y et toute famille v_1, \ldots, v_p d’éléments de T_y(Y).

Si \psi : Z \to Y est un morphisme de variétés de classe C', on a

(2)
$$(\varphi \circ \psi)^*\omega = \psi^*(\varphi^*\omega).$$

Lorsque Y est une sous-variété de X et que \varphi est l’injection canonique, on écrit parfois \omega|Y au lieu de \varphi^*\omega et l’on dit que \omega|Y est induite sur Y par \omega.

8.3.2. Les définitions et résultats du n° 7.8 s’appliquent aux formes différentielles. En particulier, un accouplement de fibrés vectoriels F' \times_X F'' \to F donne naissance à un produit extérieur ^k\Omega^{p'}(U; F) \times ^k\Omega^{p''}(U; F'') \to ^k\Omega^p(U; F), où p = p' + p'' (7.8.2); on le note (\omega', \omega'') \mapsto \omega' \wedge \omega''. La somme directe des ^k\Omega^p(U; K) pour p \geq 0 est ainsi munie d’une structure d’algèbre graduée associative et alternée (A, III, p. 53).

Soient \xi un champ de vecteurs sur X et \omega une forme différentielle de degré p \geq 1 sur X, à valeurs dans un fibré vectoriel F; le produit intérieur de \xi et \omega est la forme différentielle i(\xi, \omega) de degré p − 1 sur X, à valeurs dans F, définie par

(3)
$$i(\xi, \omega)_x(v_1, \ldots, v_{p-1}) = \omega_x(\xi(x), v_1, \ldots, v_{p-1})$$

pour tout x \in X et toute famille v_1, \ldots, v_{p-1} d’éléments de T_x(X). Si \omega est une forme différentielle de degré 0, on pose i(\xi, \omega) = 0. On écrit également i(\xi)\omega ou i_\xi\omega à la place de i(\xi, \omega). Lorsque F = K_X, la définition donnée ci-dessus coïncide avec celle de 7.8.4.

Soit F' \times_X F'' \to F un accouplement de fibrés vectoriels. Pour \omega' \in ^k\Omega^{p'}(U; F') et \omega'' \in ^k\Omega^{p''}(U; F''), on a

(4)
$$i(\xi)(\omega' \wedge \omega'') = (i(\xi)\omega') \wedge \omega'' + (-1)^{p'\omega'} \wedge i(\xi)\omega''.$$

8.3.3. Soit $(u^1, \ldots, u^n)$ un système de coordonnées dans l’ouvert $U$ de $X$. Tout élément $\omega$ de $^{k}\Omega^p(U; F)$ s’écrit de façon unique
$$
\omega = \sum_{i_1 < \cdots < i_p} f_{i_1, \ldots, i_p} \cdot du^{i_1} \wedge \cdots \wedge du^{i_p}
$$
où les $f_{i_1, \ldots, i_p}$ sont des sections de classe $C^k$ de $F$ sur $U$; dans cette formule, le signe $\wedge$ est relatif à l’accouplement canonique $K_X \times_X K_X \to K_X$ et le point désignant le produit est relatif à l’accouplement canonique $F \times_X K_X \to F$.

8.3.4. Soient $p$ un entier $\geqslant 0$ et $r$ un élément de $N_K$. Soient $E$ et $F$ des espaces de Banach, $U$ un ouvert de $E$ et $\alpha \in {}^r\Omega^p(U; F)$. Soit $\tilde{\alpha} \in C^r(U; Alt^p(E; F))$ l’élément correspondant à $\alpha$. Si $x \in U$, la différentielle $d_x \tilde{\alpha}$ de $\tilde{\alpha}$ en $x$ (5.5.6) est un élément de $\mathscr{L}(E; Alt^p(E; F))$; si $t \in E$, on a $(d_x \tilde{\alpha})(t) \in Alt^p(E; F)$, et, si $t_1, \ldots, t_p$ sont dans $E$, on a $(d_x \tilde{\alpha})(t)(t_1, \ldots, t_p) \in F$. Il existe un élément $d\alpha$ de ${}^{r-1}\Omega^{p+1}(U; F)$ et un seul tel que l’on ait
$$
(d\alpha)_x(t_0, \ldots, t_p) = \sum_{i=0}^p (-1)^i (d_x \tilde{\alpha})(t_i)(t_0, \ldots, \hat{t}_i, \ldots, t_p) \tag{1}
$$
quels que soient $x \in U$ et $t_0, \ldots, t_p$ dans $E$.

8.3.5. Soient $p$ un entier $\geqslant 0$ et $r$ un élément de $N_K$. Soient $X$ une variété de classe $C^{r+1}$, $F$ un espace de Banach, et $\omega \in {}^r\Omega^p(X; F)$. Il existe une forme différentielle $\pi \in {}^{r-1}\Omega^{p+1}(X; F)$ et une seule telle que, pour toute carte $c = (U, \varphi, E)$ de $X$, si $\omega_c$ est la forme différentielle sur $\varphi(U)$ telle que $\omega|U = \varphi^*(\omega_c)$, on ait $\pi_c = d\omega_c$, où $d\omega_c$ est définie par la formule (5) de 8.3.4.

La forme différentielle $\pi$ s’appelle la *différentielle extérieure* de $\omega$; on la note $d\omega$. Elle jouit des propriétés suivantes:

(6) Si $\psi : Y \to X$ est un morphisme de variétés de classe $C^{r+1}$, et si $\omega \in {}^r\Omega^p(X; F)$, on a $\psi^*(d\omega) = d(\psi^*\omega)$; en particulier, $d$ commute à l’opération de restriction à une sous-variété.
(7) Pour $p = 0$, l’application $d : {}^r\Omega^0(X; F) \to {}^{r-1}\Omega^1(X; F)$ coïncide avec celle définie en 8.2.2.
(8) Si $r \geqslant 2$ et si $\omega \in {}^r\Omega^p(X; F)$, on a $d(d\omega) = 0$.\footnote{Le signe $\wedge$ indique que le symbole qu’il surmonte doit être omis (cf. 7.8.4).}
(9) Pour toute application linéaire continue $u : F \to F'$ d’espaces de Banach, on a $d(u(\omega)) = u(d(\omega))$ pour $\omega \in {}^r\Omega^p(U; F)$.
(10) Pour toute application bilinéaire continue $F' \times F'' \to F$ d’espaces de Banach, on a
$$
d(\omega' \wedge \omega'') = (d\omega') \wedge \omega'' + (-1)^{p'} \omega' \wedge d\omega''
$$
pour $\omega' \in {}^r\Omega^{p'}(X; F')$ et $\omega'' \in {}^r\Omega^{p''}(X; F'')$.

8.3.6. Soit $(u^1, \ldots, u^n)$ un système de coordonnées de $X$ dans $U$. Soit
$$
\omega = \sum_{i_1 < \cdots < i_p} f_{i_1, \ldots, i_p} \cdot du^{i_1} \wedge \cdots \wedge du^{i_p}
$$

1 Le signe $\wedge$ indique que le symbole qu’il surmonte doit être omis (cf. 7.8.4).
2 Si $\omega \in {}^1\Omega^p(X; F)$ et si $d\omega \in {}^1\Omega^{p+1}(X; F)$, on a encore $d(d\omega) = 0$.

une forme différentielle sur U (avec $f_{i_1, ..., i_p} \in \mathscr{C}^r(U; F)$). On a alors

$$
d\omega = \sum_{i_1 < ... < i_p} df_{i_1, ..., i_p} \wedge du^{i_1} \wedge \cdots \wedge du^{i_p}.
$$

8.3.7. Supposons K de caractéristique zéro. Soit $\omega \in {}^r\Omega^p(X; F)$ une forme différentielle de degré $p \geq 1$ telle que $d\omega = 0$. Pour tout $x \in X$, il existe un voisinage ouvert U de $x$ et une forme différentielle $\pi \in {}^r\Omega^{p-1}(U; F)$ tel que $d\pi = \omega$ sur U.

**8.4. Transformations infinitésimales**

Soient $r \in \mathbf{N}_K$ et X une variété de classe $C^{r+1}$.

### 8.4. Transformations infinitésimales

8.4.1. Soit $\tau$ un foncteur vectoriel pour les isomorphismes (7.6.6), de classe $C^r$. Si E est un espace de Banach, on note $\mathbf{GL}(E)$ l’ouvert de $\mathscr{L}(E; E)$ constitué par les automorphismes de E. On note $\tau'_E$ l’application linéaire tangente à l’élément neutre $\mathrm{Id}_E$ du morphisme $\tau : \mathbf{GL}(E) \to \mathbf{GL}(\tau(E))$; c’est une application linéaire continue de $\mathscr{L}(E; E)$ dans $\mathscr{L}(\tau(E); \tau(E))$.

8.4.2. Soit E un espace de Banach et posons $F = \tau(E)$. Soient U un ouvert de E, $\xi$ un champ de vecteurs sur U de classe $C^r$, $\tilde{\xi} : U \to E$ l’application correspondante (obtenue en identifiant T(U) et $U \times E$ (8.1.1)), et $f : U \to F$ une application de classe $C^r$. Pour $x \in U$, on définit un élément $(\theta_{\xi}.f)(x)$ de F par la formule

$$
(\theta_{\xi}.f)(x) = d_x f(\tilde{\xi}(x)) - \tau'_E(d_x \tilde{\xi})(f(x)).
$$

(Remarquons que l’on a d’une part $\tilde{\xi}(x) \in E$ et $d_x f \in \mathscr{L}(E; F)$, d’où $d_x f(\tilde{\xi}(x)) \in F$, d’autre part, $d_x \tilde{\xi} \in \mathscr{L}(E; E)$, $\tau'_E(d_x \tilde{\xi}) \in \mathscr{L}(F; F)$ et $f(x) \in F$, d’où $\tau'_E(d_x \tilde{\xi})(f(x)) \in F$. La fonction $\theta_{\xi}.f : x \mapsto (\theta_{\xi}.f)(x)$ est de classe $C^{r-1}$ dans U.

8.4.3. Notons F le fibré vectoriel $\tau(T(X))$ (7.6.2 et 7.6.6). Soient $\xi$ un champ de vecteurs sur X et $f$ une section de F, tous deux de classe $C^r$. Soient $x$ un point de X et $c = (U, \varphi, E)$ une carte de X en $x$. Soient $c' = (U, \zeta_c, E)$ la carte vectorielle correspondante de T(X) (8.1.1) et $\tau(c') = (U, \psi_c, \tau(E))$ la carte vectorielle correspondante de F (7.6.2). Posons $x_c = \varphi(x)$; soient $\xi_c$ l’application de $\varphi(U)$ dans E telle que $\zeta_c(\xi(u)) = (u, \xi_c(\varphi(u)))$ et $f_c$ l’application de $\varphi(U)$ dans $\tau(E)$ telle que $\psi_c(f(u)) = (u, f_c(\varphi(u)))$ pour tout $u \in U$. Notons $a_c$ l’élément $(\theta_{\xi_c}.f_c)(x_c)$ de $\tau(E)$ défini en 8.4.2. Il existe un élément $a$ de $F_x$ et un seul tel que $\psi_c(a) = (x, a_c)$ pour toute carte $c$ de X en $x$. On le note $(\theta_{\xi}.f)(x)$. Il ne dépend que des germes de $\xi$ et $f$ en $x$ (et même seulement de leur jet d’ordre 1 (12.1.2)).

L’application $\theta_{\xi}.f : x \mapsto (\theta_{\xi}.f)(x)$ est une section de classe $C^{r-1}$ de F ; elle dépend de façon K-bilinéaire du couple $(\xi, f)$.

8.4.4. Conservons les hypothèses et notations précédentes. Il existe (7.6.4) un morphisme de fibrés vectoriels $\tau'$ et un seul de $\mathscr{L}(T(X); T(X))$ dans $\mathscr{L}(F; F)$ tel que, pour tout $x \in X$, la restriction de $\tau'$ à la fibre $\mathscr{L}(T(X); T(X))_x = \mathscr{L}(T_x(X); T_x(X))$ soit égale à $\tau'_{T(x)}$ (8.4.1). Si $g$ est une fonction de classe $C^r$ dans $X$, à valeurs dans $K$, on a
$$
\theta_{g\xi}.f = g \theta_\xi.f - \tau'(dg \otimes \xi)(f)
$$
(dans cette formule, on identifie $dg \otimes \xi$, qui est une section de $T'(X) \otimes T(X)$, à une section de $\mathscr{L}(T(X); T(X))$; son image $\tau'(dg \otimes \xi)$ est une section de $\mathscr{L}(F; F)$ et transforme $f$ en une section de $F$).

8.4.5. Soient $I$ un ouvert de $K$ contenant $0$, $U$ un ouvert de $X$ et $\varphi$ une application de classe $C^r$ de $I \times U$ dans $X$. Pour $(t, x) \in I \times U$, on note $\varepsilon_{t,x}$ le vecteur $(1, 0) \in K \times T_x(X) = T_{(t,x)}(I \times U)$. Pour $t \in I$, on note $\varphi_t$ l’application de $U$ dans $X$ définie par $\varphi_t(x) = \varphi(t, x)$ ($x \in U$). On suppose que les trois conditions suivantes sont vérifiées:

a) $\varphi_0$ est l’injection canonique de $U$ dans $X$;
b) pour tout $t \in T$, l’application $\varphi_t$ est un isomorphisme de variétés de classe $C^r$ de $U$ sur un ouvert de $X$;
c) la section $(t, x) \mapsto T_{(t, x)}(\varphi)(\varepsilon_{t, x})$ du fibré $\varphi^*T(X)$ est de classe $C^r$.
De plus, on pose:
d) $\xi(x) = T_{(0, x)}(\varphi)(\varepsilon_{0, x})$ pour tout $x \in U$.

L’application $\xi : x \mapsto \xi(x)$ est un champ de vecteurs de classe $C^r$ sur $U$. On dit que c’est le champ initial (ou de départ) de $\varphi$.

Soit $\tau$ un foncteur vectoriel pour les isomorphismes, de classe $C^r$; posons $F = \tau(T(X))$ et soit $f$ une section de classe $C^r$ de $F$ sur $X$. Pour $x \in U$ et $t \in I$, posons $\varphi_t^*f(x) = \tau(T_x(\varphi_t)^{-1})(f(\varphi_t(x)))$; c’est un élément de $F_x$. L’application $t \mapsto \varphi_t^*f(x)$ de $I$ dans $F_x$ est de classe $C^{r-1}$ pour tout $x \in U$ et l’on a
$$
\frac{d}{dt} (\varphi_t^*f(x))_{t=0} = (\theta_\xi.f)(x) \quad \text{pour tout } x \in U.
$$

8.4.6. Etant donnés un champ de vecteurs $\xi$ de classe $C^r$ sur $X$ et un point $x_0$ de $X$, il existe un ouvert $I$ de $K$, contenant $0$, un ouvert $U$ de $X$ contenant $x_0$ et une application $\varphi : I \times U \to X$ de classe $C^r$ satisfaisant aux conditions $a), b)$ et c) de 8.4.5 et telle que le champ initial de $\varphi$ soit la restriction $\xi|U$ de $\xi$ à $U$.

8.4.7. *Exemple.* — Soient $F$ un espace de Banach et $p$ un entier $\geqslant 0$. Si $V$ est un espace de Banach, posons $\alpha_p(V) = \mathrm{Alt}^p(V; F)$; si $u$ est un isomorphisme de $V$ sur un espace de Banach $V'$, désignons par $\alpha_p(u)$ l’isomorphisme de $\alpha_p(V)$ sur $\alpha_p(V')$ déduit de $u$ par transport de structure. On obtient ainsi un foncteur vectoriel pour les isomorphismes, que l’on note $\alpha_p$ (7.8.1 et *Errata* au n° 7.8). On peut lui appliquer ce qui précède; on a
$$
\alpha_p(T(X)) = \mathrm{Alt}^p(T(X); F).
$$
Les sections de $\alpha_p(T(X))$ sont les formes différentielles de degré $p$ sur $X$, à valeurs dans $F$; si $\omega$ est une telle forme et si $\xi$ est un champ de vecteurs sur $X$, tous deux de classe $C^r$, $\theta_\xi.\omega$ est une forme différentielle de degré $p$ sur $X$, à valeurs dans $F$ et de classe $C^{r-1}$. On a
$$
\theta_\xi.\omega = d(i(\xi)\omega) + i(\xi)d\omega
$$

et, lorsque $r \geq 2$,

$$
\theta_\xi \cdot d\omega = d(\theta_\xi \cdot \omega).
$$

Lorsque $p = 0$, le foncteur $\alpha_p$ est le foncteur vectoriel constant défini par $F$; le fibré $\alpha_0(T(X))$ s'identifie au fibré trivial $F_X$, et les sections de ce fibré s'identifient aux fonctions sur $X$ à valeurs dans $F$. Si $\xi$ est un champ de vecteurs de classe $C^r$ sur $X$ et si $f \in \mathscr{C}^r(X; F)$, on a

$$
\theta_\xi \cdot f = \langle \xi, df \rangle = D_\xi(f) \quad (8.2.3);
$$

c'est un élément de $\mathscr{C}^{r-1}(X; F)$.

8.4.8. Soient $\tau$ et $\tau_1$ deux foncteurs vectoriels pour les isomorphismes. Un morphisme de foncteurs vectoriels $h : \tau_1 \to \tau$ définit un morphisme de fibrés vectoriels, noté encore $h$, de $\tau_1(T(X))$ dans $\tau(T(X))$ (7.6.4), et fait correspondre à une section $f$ de $\tau_1(T(X))$ une section $h(f)$ de $\tau(T(X))$. Si $\xi$ est un champ de vecteurs sur $X$, et si $f$ et $\xi$ sont de classe $C^r$, on a $\theta_\xi \cdot h(f) = h(\theta_\xi \cdot f)$.

Plus généralement, soient $\tau, \tau_1, \ldots, \tau_d$ des foncteurs vectoriels pour les isomorphismes et soit $h : (\tau_1, \ldots, \tau_d) \to \tau$ un morphisme $d$-linéaire (7.6.4). Soit $f_i \in \mathscr{S}_{\tau_i(T(X))}^r(X)$ (pour $i = 1, \ldots, d$), et soit $\xi$ un champ de vecteurs de classe $C^r$ sur $X$. On a

$$
\theta_\xi \cdot h(f_1, \ldots, f_d) = \sum_{1 \leq i \leq d} h(f_1, \ldots, f_{i-1}, \theta_\xi \cdot f_i, f_{i+1}, \ldots, f_d).
$$

Par exemple, si $f$ est une section de $\tau(T(X))$ et $g$ une fonction sur $X$, à valeurs dans $K$, toutes deux de classe $C^r$, on a

$$
\theta_\xi \cdot (gf) = (\theta_\xi \cdot g)f + g(\theta_\xi \cdot f).
$$

Si $\omega_1$ et $\omega_2$ sont deux formes différentielles de classe $C^r$, à valeurs dans des espaces de Banach $F_1$ et $F_2$ respectivement, on a

$$
\theta_\xi \cdot (\omega_1 \wedge \omega_2) = (\theta_\xi \cdot \omega_1) \wedge \omega_2 + \omega_1 \wedge (\theta_\xi \cdot \omega_2),
$$

le produit extérieur étant pris par rapport à une application bilinéaire continue de $F_1 \times F_2$ dans un espace de Banach $F$.

8.4.9. Soient $\tau$ un foncteur vectoriel pour les isomorphismes, contravariant (8.2.7), de classe $C^r$, $\varphi : X \to Y$ un morphisme de variétés de classe $C^{r+1}$, $\xi$ (resp. $\eta$) un champ de vecteurs de classe $C^r$ sur $X$ (resp. $Y$) tels que $\xi$ soit $\varphi$-lié à $\eta$ (8.2.6). Pour toute section $f$ de $\tau(T(Y))$, de classe $C^r$, on a

$$
\varphi^*(\theta_\eta \cdot f) = \theta_\xi \cdot \varphi^*f.
$$

### 8.5. Le crochet

Soit $r \in \mathbf{N}_k$ et soit $X$ une variété de classe $C^{r+1}$.

8.5.1. Appliquons les définitions du n° 8.4 en prenant pour $\tau$ le foncteur identique: $\tau(V) = V$ pour tout espace de Banach $V$ et $\tau(u) = u$ pour tout isomorphisme $u$ d’espaces de Banach. On a alors $\tau(T(X)) = T(X)$. Si $\xi$ et $\eta$ sont deux champs de vecteurs de classe $C^r$ sur $X$, on pose

(1)
$$
[\xi, \eta] = \theta_{\xi} \cdot \eta;
$$
c’est un champ de vecteurs de classe $C^{r-1}$ sur $X$, appelé le crochet de $\xi$ et de $\eta$.

8.5.2. L’application $(\xi, \eta) \mapsto [\xi, \eta]$ est K-bilinéaire et alternée. Si $f$ et $g$ sont des fonctions de classe $C^r$ sur $X$, à valeurs dans $K$, on a:

(2)
$$
[f\xi, g\eta] = fg[\xi, \eta] + (fD_{\xi}g)\eta - (gD_{\eta}f)\xi.
$$

8.5.3. Soit $F$ un espace de Banach. On a

(3)
$$
D_{[\xi, \eta]} = D_{\xi} \circ D_{\eta} - D_{\eta} \circ D_{\xi}
$$
dans l’espace des applications de $\mathscr{C}^{r+1}(X; F)$ dans $\mathscr{C}^{r-1}(X; F)$.

Si $r \geqslant 2$ et si $\zeta$ est un troisième champ de vecteurs de classe $C^r$ sur $X$, on a

(4)
$$
[[\xi, \eta], \zeta] = [\xi, [\eta, \zeta]] - [\eta, [\xi, \zeta]] \tag{1}
$$
ou encore
$$
[\xi, [\eta, \zeta]] + [\eta, [\zeta, \xi]] + [\zeta, [\xi, \eta]] = 0.
$$

Plus généralement, si $r \geqslant 2$ et si $\tau$ est un foncteur vectoriel pour les isomorphismes, on a

(5)
$$
\theta_{[\xi, \eta]} = \theta_{\xi} \circ \theta_{\eta} - \theta_{\eta} \circ \theta_{\xi}
$$
dans l’espace des applications de $\mathscr{S}_{F}^{r}(X)$ dans $\mathscr{S}_{F}^{r-2}(X)$ (avec $F = \tau(T(X))$).

Si $r \geqslant \infty$, les champs de vecteurs de classe $C^r$ sur $X$ forment une K-algèbre de Lie pour le crochet (LIE, I, § 1, n° 2).

8.5.4. Soient $E$ un espace de Banach, $U$ un ouvert de $E$, $\xi$ et $\eta$ deux champs de vecteurs de classe $C^r$ sur $U$, identifiés à des éléments de $\mathscr{C}^r(U; E)$. Leur crochet est donné par la formule:

(6)
$$
[\xi, \eta] = D_{\xi}\eta - D_{\eta}\xi.
$$

8.5.5. Soit $(u^1, \ldots, u^n)$ un système de coordonnées de $X$ dans un ouvert $U$. Soient $\xi = \sum a^i \frac{\partial}{\partial u^i}$ et $\eta = \sum b^i \frac{\partial}{\partial u^i}$ deux champs de vecteurs de classe $C^r$ sur $U$. Posons
$$
[\xi, \eta] = \sum c^i \frac{\partial}{\partial u^i}.
$$
On a

(7)
$$
c^i = \sum_{1 \leq j \leq n} \left( a^j \frac{\partial b^i}{\partial u^j} - b^j \frac{\partial a^i}{\partial u^j} \right).
$$

8.5.6. Soient $\varphi : X \to Y$ un morphisme de variétés de classe $C^{r+1}$, $\xi_1$ et $\xi_2$ deux champs

1 La formule (4) est encore exacte si l’on suppose seulement que les champs de vecteurs $\xi, \eta, \zeta, [\xi, \eta], [\eta, \zeta], [\zeta, \xi]$ sont tous de classe $C^1$.

de vecteurs sur X, $\eta_1$ et $\eta_2$ deux champs de vecteurs sur Y, tous de classe $C^r$. Si $\xi_1$ et $\xi_2$ sont $\varphi$-liés à $\eta_1$ et $\eta_2$ respectivement, $[ \xi_1, \xi_2 ]$ est $\varphi$-lié à $[ \eta_1, \eta_2 ]$.

8.5.7. Soit $\omega$ une forme différentielle de degré $p$ sur X, à valeurs dans un espace de Banach F et de classe $C^r$, et soient $\xi_0, \ldots, \xi_p$ des champs de vecteurs de classe $C^r$ sur X. On a

(8) $$
(\theta_{\xi_0} \cdot \omega)(\xi_1, \ldots, \xi_p) = D_{\xi_0} \omega(\xi_1, \ldots, \xi_p) - \sum_{i=1}^p \omega(\xi_1, \ldots, [\xi_0, \xi_i], \ldots, \xi_p)
$$
et
(9) $$
d\omega(\xi_0, \ldots, \xi_p) = \sum_{i=0}^p (-1)^i D_{\xi_i} \omega(\xi_0, \ldots, \hat{\xi}_i, \ldots, \xi_p)
+ \sum_{i<j} (-1)^{i+j} \omega([\xi_i, \xi_j], \xi_0, \ldots, \hat{\xi}_i, \ldots, \hat{\xi}_j, \ldots, \xi_p).
$$

Si $\xi$ et $\eta$ sont des champs de vecteurs de classe $C^r$, on a
(10) $$
\theta_{\xi} \circ i(\eta) - i(\eta) \circ \theta_{\xi} = i([\xi, \eta])
$$
dans l’espace des applications de $r\Omega^p(X; F)$ dans $r-1\Omega^{p-1}(X; F)$.
Pour $p = 1$, la formule (9) s’écrit:
(11) $$
d\omega(\xi, \eta) = D_{\xi} \langle \eta, \omega \rangle - D_{\eta} \langle \xi, \omega \rangle - \langle [\xi, \eta], \omega \rangle.
$$

### 8.6. Relèvements

Soit $r \in \mathbf{N}_k$ et soit $g : X \to Y$ un morphisme de variétés de classe $C^{r+1}$.

8.6.1. Un relèvement de $g$ dans $T(Y)$ est une application $\psi : X \to T(Y)$ telle que le diagramme

$$
\begin{array}{ccc}
& & T(Y) \\
& \nearrow \psi & \downarrow \pi \\
X & \xrightarrow{g} & Y
\end{array}
$$

soit commutatif, $\pi$ désignant la projection canonique de $T(Y)$ sur Y. La donnée de $\psi$ équivaut à celle d’une section du fibré vectoriel $g^*T(Y)$ image réciproque par $g$ de $T(Y)$.

La notion de relèvement généralise celle de champ de vecteurs (à laquelle elle se réduit lorsque $g = \mathrm{Id}_X$); une partie importante des définitions et résultats relatifs aux $\theta_{\xi}$ et $i(\xi)$ s’étendent aux relèvements; nous nous bornerons à en indiquer brièvement quelques-uns.

8.6.2. Soit $\psi : X \to T(Y)$ un relèvement de $g : X \to Y$, et soit $\omega$ une forme différentielle de degré $p$ sur Y, à valeurs dans un fibré vectoriel F de base Y. Lorsque $p \geqslant 1$, on note $i(\psi, \omega)$ ou $i(\psi)\omega$ ou $i_\psi(\omega)$ la forme différentielle sur X, de degré $p - 1$, à valeurs dans $g^* F$, telle que

(1)
$$
i(\psi, \omega)_x(v_1, \ldots, v_{p-1}) = \omega_{g(x)}(\psi(x), T_x(g).v_1, \ldots, T_x(g).v_{p-1})
$$
pour tout $x \in X$ et toute famille $v_1, \ldots, v_{p-1}$ d'éléments de $T_x(X)$. Lorsque $p = 0$, on pose $i(\psi, \omega) = 0$. On dit que $i(\psi, \omega)$ est le produit intérieur de $\psi$ et de $\omega$; si $\psi$ et $\omega$ sont de classe $C^r$, il en est de même de $i(\psi, \omega)$. Soit $F' \times_Y F'' \to F$ un accouplement de fibrés vectoriels de base Y. Pour $\omega' \in {}^r\Omega^{p'}(Y; F')$ et $\omega'' \in {}^r\Omega^{p''}(Y; F'')$, on a

(2)
$$
i(\psi)(\omega' \wedge \omega'') = (i(\psi)\omega') \wedge g^*\omega'' + (-1)^{p'}g^*\omega' \wedge i(\psi)\omega''.
$$

8.6.3. *Exemples*

a) Un champ de vecteurs $\xi$ sur X définit un relèvement $T(g) \circ \xi$ de $g$ dans $T(Y)$, et l'on a:

(3)
$$
i(T(g) \circ \xi) = i(\xi) \circ g^*.
$$

b) Un champ de vecteurs $\eta$ sur Y définit un relèvement $\eta \circ g$ de $g$ dans $T(Y)$, et l'on a:

(4)
$$
i(\eta \circ g) = g^* \circ i(\eta).
$$

c) Plus généralement, soit $h : Y \to Z$ un morphisme de variétés de classe $C^{r+1}$. Si $\psi$ est un relèvement de $g$ dans $T(Y)$, alors $T(h) \circ \psi$ est un relèvement de $h \circ g$ dans $T(Z)$ et l'on a:

(5)
$$
i(T(h) \circ \psi) = i(\psi) \circ h^*.
$$

Si $\varphi$ est un relèvement de $h$ dans $T(Z)$, alors $\varphi \circ g$ est un relèvement de $h \circ g$ dans $T(Z)$ et l'on a:

(6)
$$
i(\varphi \circ g) = g^* \circ i(\varphi).
$$

8.6.4 (*Transformations infinitésimales*). Soit $\psi$ un relèvement de classe $C^r$ de $g$ et soit $\omega$ une forme différentielle de degré $p$ sur Y, à valeurs dans un espace de Banach F, et de classe $C^r$. La forme différentielle sur X

(7)
$$
d(i(\psi)\omega) + i(\psi)d\omega
$$
est de degré $p$ et de classe $C^{r-1}$; on la note $\theta_{\psi}.\omega$.

Si $f$ est une fonction de classe $C^r$ sur X, on a

(8)
$$
\theta_{f\psi}.\omega = df \wedge i(\psi)\omega + f\theta_{\psi}.\omega.
$$

8.6.5 (*Caractérisation de $\theta_{\psi}.\omega$ comme dérivée*). Conservons les hypothèses de 8.6.4. Soit $x \in X$. Il existe alors un voisinage ouvert U de $x$, un voisinage ouvert I de 0 dans K, et un morphisme $G : I \times U \to Y$, de classe $C^r$, ayant les deux propriétés suivantes:

a) Pour tout $x \in U$, on a $G(0, x) = g(x)$.

b) Pour tout $x \in U$, l'image par $T_{(0, x)}(G)$ du vecteur tangent $(1, 0)$ est égale à $\psi(x)$.

Supposons que (U, I, G) vérifie ces conditions; pour tout $t \in I$, notons $G_t$ l’application $x \mapsto G(t, x)$ de X dans Y; posons $\omega_t = G_t^*(\omega)$. Pour tout $x \in X$, l’application $t \mapsto \omega_t(x)$ de I dans $\mathrm{Alt}^p(T_x(X), F)$ est de classe $C^r$, et sa dérivée à l’origine est donnée par la formule

$$
\frac{d}{dt} (\omega_t(x))_{t=0} = (\theta_\psi \cdot \omega)(x).
$$

### 8.7. Affaiblissement de structure

Dans ce n°, on suppose $K = \mathbf{R}$.

8.7.1. Soit X une variété de classe $C^s$, et soit F un fibré vectoriel sur X, de classe $C^k$, avec $0 \leq k \leq s$. Si $0 \leq k' \leq k$, il existe sur F une structure $F_{k'}$ et une seule de fibré vectoriel de base X et de classe $C^{k'}$ telle que toute carte vectorielle de F soit une carte vectorielle de $F_{k'}$. On dit que $F_{k'}$ se déduit de F par affaiblissement de la structure de fibré de F.

8.7.2. Soit $r \in \mathbf{N}_\mathbf{R}$ avec $r \leq s$, et soit $X_r$ la variété de classe $C^r$ sous-jacente à X (5.13.1). Le fibré tangent $T(X_r)$ est de classe $C^{r-1}$; c’est le fibré obtenu par affaiblissement de structure à partir du fibré tangent $T(X)$, qui est de classe $C^{s-1}$.

Soit F un fibré vectoriel sur X, de classe $C^k$, pour $0 \leq k \leq r - 1$. Les formes différentielles de classe $C^k$ sur X à valeurs dans F s’identifient canoniquement aux formes différentielles correspondantes sur $X_r$. Les diverses opérations sur ces formes décrites dans le reste de ce paragraphe sont compatibles avec cette identification.

Dans la suite de ce fascicule, nous laisserons souvent au lecteur le soin d’expliciter les autres résultats de ce genre.

### 8.8. Variétés presque complexes et variétés complexes

Dans ce n°, on suppose $K = \mathbf{R}$ et on désigne par X une variété (réelle) de classe $C^r$, avec $r \in \mathbf{N}_\mathbf{R}$.

8.8.1 (« Fibrés vectoriels complexes »). Un fibré vectoriel sur C de base X (7.3.4) est aussi appelé un fibré vectoriel complexe de base X. Si M est un tel fibré vectoriel, on appelle carte vectorielle complexe de M un triplet $(U, \varphi, E)$, où U est un ouvert de X, E un espace de Banach complexe et $\varphi$ un isomorphisme de fibrés vectoriels complexes de $M|U$ sur le fibré trivial $E_U = U \times E$. Une famille $(U_i, \varphi_i, E_i)$ de cartes vectorielles complexes de M dont les domaines de définition $U_i$ recouvrent X est appelée un atlas vectoriel complexe de M; tout fibré vectoriel complexe possède un atlas vectoriel complexe (7.3.3).

On dit parfois C-vectoriel au lieu de vectoriel complexe. De manière analogue, on dit parfois, lorsqu’on veut parler d’un fibré vectoriel sur $\mathbf{R}$, d’une carte vectorielle ordinaire de ce fibré, etc., « vectoriel réel » ou « R-vectoriel » au lieu de « vectoriel ».

Soit M un fibré vectoriel complexe de base X. Il existe un automorphisme $j$ et un seul du fibré vectoriel (réel) sous-jacent à M (7.3.3) dont la restriction à chaque fibre est la multiplication par l’élément i de C ; le carré de j est égal à −1. Réciproquement, si M est un fibré vectoriel (réel) de base X et j un automorphisme de M tel que $j^2 = -1$, il existe sur M une unique structure de fibré vectoriel complexe admettant M comme fibré vectoriel (réel) sous-jacent et pour laquelle j est la multiplication par i.

8.8.2 (« Complexification d’un fibré vectoriel »). On définit un foncteur vectoriel τ en posant $\tau(E) = E \otimes \mathbf{C}$ pour tout espace de Banach (réel) E, et $\tau(u) = u \otimes \mathrm{Id}_\mathbf{C}$ pour tout morphisme $u : E \to E'$ d’espaces de Banach (réels).

Si F est un fibré vectoriel de base X et de classe $C^k$ ($0 \leq k \leq r$), son transformé par le foncteur vectoriel $\tau$ se note $F \otimes \mathbf{C}$. Il existe sur $F \otimes \mathbf{C}$ une unique structure de fibré vectoriel complexe de base X et de classe $C^k$, compatible avec sa structure de fibré vectoriel (réel) et induisant sur chaque fibre $(F \otimes \mathbf{C})_x = F_x \otimes \mathbf{C}$ sa structure canonique d’espace de Banach complexe (EVT, II, § 8, n° 1, Exemple). Muni de cette structure, on dit que $F \otimes \mathbf{C}$ est le complexifié de F.

Soit U un ouvert de X ; l’application canonique

$$
\mathscr{S}_F^k(U) \otimes \mathbf{C} \to \mathscr{S}_{F \otimes \mathbf{C}}^k(U)
$$

est un isomorphisme, par lequel on identifie ces deux espaces. Si $s \in \mathscr{S}_{F \otimes \mathbf{C}}^k(U)$, les éléments $\sigma, \tau$ de $\mathscr{S}_F^k(U)$ tels que $s = \sigma + i \tau$ s’appellent la partie réelle et la partie imaginaire de s ; la section $\bar{s} = \sigma - i \tau$ s’appelle la conjuguée de s.

En particulier, une section du fibré $T(X) \otimes \mathbf{C}$ s’appelle un champ de vecteurs complexe sur X.

Soit H un fibré vectoriel complexe de base X. Les isomorphismes canoniques $\mathrm{Alt}_\mathbf{R}^p(T_x(X); H) \to \mathrm{Alt}_\mathbf{C}^p(T_x(X) \otimes \mathbf{C}; H)$ définissent un isomorphisme de fibrés vectoriels complexes, dit canonique, de $\mathrm{Alt}_\mathbf{R}^p(T(X); H)$ sur $\mathrm{Alt}_\mathbf{C}^p(T(X) \otimes \mathbf{C}; H)$ (7.8.5), grâce auquel nous identifierons ces deux fibrés. Soit $\omega$ une section de ce fibré, autrement dit une forme différentielle de degré p sur X, à valeurs dans H, et soit $\zeta$ un champ de vecteurs complexes, de partie réelle $\xi$ et de partie imaginaire $\eta$. On pose alors:

$$
i(\zeta, \omega) = i(\xi, \omega) + i.i(\eta, \omega).
$$

Si H est un fibré trivial, on pose

$$
\theta_\zeta.\omega = \theta_\xi.\omega + i \theta_\eta.\omega.
$$

De même, on étend par linéarité le crochet aux champs de vecteurs complexes. Les formules des n°s précédents restent valables.

8.8.3. On appelle structure presque complexe de classe $C^k$ ($k \leq r - 1$) sur X la donnée d’une structure de fibré vectoriel complexe sur T(X), de classe $C^k$, ayant pour structure réelle sous-jacente la structure naturelle de T(X). Une telle structure équivaut à la donnée d’un automorphisme j de classe $C^k$ de T(X) tel que $j^2 = -1$.

Donnons-nous une telle structure. Prolongeons j en un $\mathbf{C}$-automorphisme de $T(X) \otimes \mathbf{C}$. Il existe une décomposition et une seule de $T(X) \otimes \mathbf{C}$ en somme directe de deux sous-fibrés complexes:

(1)

$$
T(X) \otimes \mathbf{C} = T'(X) \oplus T''(X)
$$

telle que $j$ coïncide avec la multiplication par $i$ sur $T'(X)$ et par $-i$ sur $T''(X)$. Le projecteur $p'$ de $T(X) \otimes \mathbf{C}$ sur $T'(X)$ est égal à $\frac{1}{2}(1 - ij)$; le projecteur $p'' = 1 - p'$ de $T(X) \otimes \mathbf{C}$ sur $T''(X)$ est égal à $\frac{1}{2}(1 + ij)$. Les composés
$$
\pi': \quad T(X) \to T(X) \otimes \mathbf{C} \xrightarrow{p'} T'(X)
$$
$$
\pi'': \quad T(X) \to T(X) \otimes \mathbf{C} \xrightarrow{p''} T''(X)
$$
sont des $\mathbf{R}$-isomorphismes; le premier transforme $j$ en la multiplication par $i$, le second en la multiplication par $-i$.

8.8.4 (« Formes de type $(p, q)$ »). Conservons les hypothèses et notations du n° précédent. Soit $F$ un fibré vectoriel complexe de base $X$, soient $p$ et $q$ deux entiers $\geqslant 0$, et soit $n = p + q$. Soit $\omega$ une forme différentielle de degré $n$ sur un ouvert $U$ de $X$, à valeurs dans $F$; identifions (8.8.2) $\omega$ à une section de $\mathrm{Alt}_c^n(T(X) \otimes \mathbf{C}; F)$. On dit que $\omega$ est *de type* $(p, q)$ si, pour tout $x \in U$, on a
$$
\omega_x(v_1, \ldots, v_n) = 0
$$
dès que $p + 1$ des vecteurs $v_i$ appartiennent à $T'_x(X)$ ou que $q + 1$ des vecteurs $v_i$ appartiennent à $T''_x(X)$. Si l’on identifie $\bigwedge^n T_x(X) \otimes \mathbf{C}$ à la somme directe des espaces $\bigwedge^{m'} T'_x(X) \otimes \bigwedge^{m''} T''_x(X)$ pour $m' + m'' = n$ (A, III, p. 85) et $\omega_x$ à une forme $\mathbf{C}$-linéaire sur $\bigwedge^n T_x(X)$, il revient au même de dire que $\omega_x$ est nulle sur $\bigwedge^{m'} T'_x(X) \otimes \bigwedge^{m''} T''_x(X)$ pour $(m', m'') \neq (p, q)$.

Pour tout couple $(p, q)$ d’entiers $\geqslant 0$ avec $p + q = n$, il existe un sous-fibré vectoriel complexe $\mathrm{Alt}^{p,q}(T(X); F)$ de $\mathrm{Alt}^n(T(X); F)$ et un seul tel que ses sections sur un ouvert $U$ de $X$ soient les formes différentielles de type $(p, q)$ sur $X$, à valeurs dans $F$. Le fibré vectoriel $\mathrm{Alt}^n(T(X); F)$ est somme directe des fibrés vectoriels $\mathrm{Alt}^{p,q}(T(X); F)$ pour $p \geqslant 0,\ q \geqslant 0$ et $p + q = n$. Toute forme différentielle $\omega$ de degré $n$ à valeurs dans $F$ se décompose de manière unique en
$$
\omega = \sum_{p+q=n} \omega_{p,q}
$$
où $\omega_{p,q}$ est une forme de type $(p, q)$, appelée *composante de type* $(p, q)$ de $\omega$. Si $\omega$ est de classe $\mathbf{C}^h$, avec $0 \leq h \leq k$, il en est de même de ses composantes.

*Exemples*

a) Une forme différentielle de degré $n$ est de type $(n, 0)$ si et seulement si elle est $\mathbf{C}$-multilinéaire.

b) Soient $F', F''$ et $F$ trois fibrés vectoriels complexes et soit $F' \times_X F'' \to F$ un accouplement $\mathbf{C}$-bilinéaire. Si $\omega'$ (resp. $\omega''$) est une forme différentielle de type $(p', q')$ (resp. $(p'', q'')$) à valeurs dans $F'$ (resp. $F''$), la forme différentielle $\omega' \wedge \omega''$ est de type $(p' + p'', q' + q'')$.

c) Supposons que $F$ soit le complexifié d’un fibré vectoriel (réel) (8.8.2). Si $\omega$ est une forme différentielle de type $(p, q)$ à valeurs dans $F$, sa conjuguée $\overline{\omega}$ (8.8.2) est de type $(q, p)$.

8.8.5. Outre les hypothèses précédentes, on suppose $k \geqslant 1$. Les trois conditions suivantes sont alors équivalentes:

(i) Pour tout ouvert U de X et pour tout couple $(\xi, \eta)$ de champs de vecteurs complexes sur U, de classe $C^k$, tel que $\xi(x)$ et $\eta(x)$ appartiennent à $T'_x(X)$ pour tout $x \in U$, on a $[\xi, \eta](x) \in T'_x(X)$ pour tout $x \in U$.

(ii) Pour tout ouvert U de X et tout couple $(\xi, \eta)$ de champs de vecteurs (réels) sur U, de classe $C^k$, on a
$$
[\xi, \eta] + j[j\xi, \eta] + j[\xi, j\eta] - [j\xi, j\eta] = 0.
$$

(iii) Pour tout ouvert U de X et pour toute forme différentielle complexe $\omega$ de type $(1, 0)$ sur U, de classe $C^k$, la composante de type $(0, 2)$ de $d\omega$ est nulle.

Supposons que ces conditions soient vérifiées. Soit $\omega$ une forme différentielle de type $(p, q)$ sur un ouvert U de X, de classe $C^h$ avec $1 \leq h \leq k$, à valeurs dans un espace de Banach complexe F. On note $d'\omega$ (resp. $d''\omega$) la composante de type $(p+1, q)$ (resp. $(p, q+1)$) de $d\omega$; les autres composantes de $d\omega$ sont alors nulles et l’on a
$$
d\omega = d'\omega + d''\omega.
$$
Si $k \geq 2$, on a
$$
d'(d'\omega) = 0 \quad , \quad d''(d''\omega) = 0 \quad , \quad d'(d''\omega) + d''(d'\omega) = 0.
$$
Avec les notations de 8.8.4, exemple b), on a
$$
d'(\omega' \wedge \omega'') = d'(\omega') \wedge \omega'' + (-1)^{p'+q'} \omega' \wedge d'(\omega'')
$$
$$
d''(\omega' \wedge \omega'') = d''(\omega') \wedge \omega'' + (-1)^{p'+q'} \omega' \wedge d''(\omega'').
$$
Avec celles de 8.8.4, exemple c), on a
$$
d'(\overline{\omega}) = \overline{d''(\omega)}.
$$
Dans les formules (4) et (5) (resp. (6)), les formes différentielles $\omega'$ et $\omega''$ (resp. $\omega$) sont supposées de classe $C^1$.

8.8.6 (« Structure presque complexe d’une variété complexe »). Soit $X^c$ une variété analytique complexe, admettant X comme variété analytique réelle sous-jacente (5.14.2.a)). Le fibré $T(X)$ s’identifie au fibré vectoriel (réel) sous-jacent au fibré vectoriel complexe $T(X^c)$, ce qui munit X d’une structure presque complexe de classe $C^\omega$, dite définie par la structure de variété analytique complexe donnée sur X. Cette structure presque complexe satisfait aux conditions (i) à (iii) de 8.8.5; en particulier, les opérateurs $d'$ et $d''$ de 8.8.5 sont définis. Si $f : X^c \to Y^c$ est un morphisme de variétés analytiques complexes, $f^*$ commute aux opérateurs $d'$ et $d''$.

8.8.7. Conservons les hypothèses et notations de 8.8.6. Soit $\overline{X}^c$ la conjuguée de $X^c$ (5.14.2.b)). Plongeons X par l’application diagonale $x \mapsto (x, x)$ dans la variété complexe $X^c \times \overline{X}^c$, et soit g l’anti-automorphisme $(x, y) \mapsto (y, x)$ de $X^c \times \overline{X}^c$. Le couple $(X^c \times \overline{X}^c, g)$ est une *complexification* de X (5.14.8). En particulier, pour tout $x \in X$, l’espace tangent $T_x(X^c \times \overline{X}^c)$ s’identifie à $T_x(X) \otimes \mathbf{C}$; dans cette identification, $T_x(X^c \times \{x\})$ correspond à $T'_x(X)$ et $T_x(\{x\} \times \overline{X}^c)$ correspond à $T''_x(X)$.

8.8.8. Supposons $r = \omega$; toute structure presque complexe de classe $C^\omega$ sur $X$ satisfaisant aux conditions équivalentes (i) à (iii) de 8.8.5 est la structure presque complexe définie par une structure de variété analytique complexe et une seule sur $X$.¹

8.8.9 (« Formes holomorphes »). Reprenons les hypothèses et notations de 8.8.6, et soit $F$ un espace de Banach complexe. Les formes différentielles morphiques (autrement dit analytiques complexes) sur $X^c$, à valeurs dans $F$, sont encore appelées formes différentielles *holomorphes*; l’identification de $T(X^c)$ à $T(X)$ les identifie à des formes différentielles (analytiques réelles) sur $X$. Pour qu’une forme différentielle $\omega$ de degré $p$ sur $X$, à valeurs dans $F$ et de classe $C^k$ avec $k \geqslant 1$, soit holomorphe, il faut et il suffit qu’elle soit de type $(p, 0)$ et que $d''\omega = 0$.

Soit $\xi$ un champ de vecteurs sur $X$. On dit que $\xi$ est *holomorphe* si c’est une application analytique complexe de $X^c$ dans $T(X^c) = T(X)$, autrement dit un champ de vecteurs analytique complexe sur $X^c$. Si tel est le cas, et si $\omega$ est une forme différentielle holomorphe sur $X$ à valeurs dans $F$, la forme $\theta_\xi.\omega$ (resp. $i(\xi)\omega$) est la même, que l’on considère $\xi$ comme champ de vecteurs analytique complexe sur $X^c$ et $\omega$ comme un élément de $\Omega^p(X^c; F)$, ou $\xi$ comme un champ de vecteurs sur $X$ et $\omega$ comme un élément de $\Omega^p(X; F)$. De plus, soient $\xi' = \pi'(\xi)$ et $\xi'' = \pi''(\xi)$ les composantes de $\xi$ dans $T'(X)$ et $T''(X)$ respectivement (8.8.3); on a

$$
\theta_\xi.\omega = \theta_{\xi'}.\omega \quad , \quad \theta_{\xi''}.\omega = 0 \tag{7}
$$
$$
i(\xi)\omega = i(\xi')\omega \quad , \quad i(\xi'')\omega = 0. \tag{8}
$$

8.8.10. *Exemple.* — Supposons que $X^c$ soit un ouvert de $\mathbf{C}^n$ et notons $z^1, \ldots, z^n$ les fonctions coordonnées sur $X^c$. Pour $1 \leqslant k \leqslant n$, posons $z^k = x^k + iy^k$, où $x^k$ et $y^k$ sont à valeurs réelles. Considérons le repère tangent $(\partial/\partial z^k)$ de $T(X^c)$ défini par le système de coordonnées $(z^k)$ et le repère tangent $(\partial/\partial x^k, \partial/\partial y^k)$ de $T(X)$ défini par le système de coordonnées $(x^k, y^k)$ (8.1.5). On a $j(\partial/\partial x^k) = \partial/\partial y^k$ et l’image de $\partial/\partial z^k$ par l’application $\pi': T(X) = T(X^c) \to T'(X)$ (8.8.3) est égale à
$$
\frac{1}{2}(\partial/\partial x^k - i \partial/\partial y^k);
$$
on la note encore en général $\partial/\partial z^k$.² Le champ de vecteurs complexe conjugué de ce champ $\partial/\partial z^k$ est noté $\partial/\partial \bar{z}^k$; on a
$$
\partial/\partial \bar{z}^k = \frac{1}{2}(\partial/\partial x^k + i \partial/\partial y^k). \tag{9}
$$

Si $f$ est une fonction de classe $C^1$ sur $X$, à valeurs dans un espace de Banach complexe $F$, les formes différentielles $d'f$ et $d''f$ (8.8.5) sont données par
$$
d'f = \sum_{1 \leqslant k \leqslant n} \frac{\partial f}{\partial z^k} \, dz^k \quad , \quad d''f = \sum_{1 \leqslant k \leqslant n} \frac{\partial f}{\partial \bar{z}^k} \, d\bar{z}^k. \tag{10}
$$

¹ Si $X$ est de dimension finie, ceci reste vrai pour une structure presque complexe de classe $C^k$ avec $k \geqslant \dim X$ (cf. A. NEWLANDER and L. NIRENBERG, *Complex analytic coordinates in almost complex manifolds*, Ann. of Math. LXV (1957), p. 391–404).
² On prendra garde que l’identification canonique de $T(X^c)$ avec $T(X)$ ne transforme pas le champ de vecteurs $\partial/\partial z^k$ sur $X^c$ en le champ de vecteurs $\partial/\partial z^k$ sur $X$, mais en le champ de vecteurs $\partial/\partial z^k + \partial/\partial \bar{z}^k$. Cependant, les deux champs de vecteurs notés $\partial/\partial z^k$ prennent la même valeur sur les formes différentielles holomorphes (8.8.9), qui sont d’ailleurs les seules auxquelles l’on puisse appliquer un champ de vecteurs de $X^c$.

Rappelons que l’on a

$$
df = d'f + d''f
$$

$$
dz^k = dx^k + i\ dy^k \qquad d\bar{z}^k = dx^k - i\ dy^k.
$$

Si $A = (i_1, \ldots, i_p)$ est une suite strictement croissante d’entiers appartenant à l’intervalle $[1, n]$, on pose

$$
dz^A = dz^{i_1} \wedge \cdots \wedge dz^{i_p}
$$

et l’on note $d\bar{z}^A$ la conjuguée de $dz^A$. Toute forme différentielle $\omega$ de type $(p, q)$ à valeurs dans $F$ s’écrit de façon unique

(11)
$$
\omega = \sum_{A, B} f_{A, B}\ dz^A \wedge d\bar{z}^B
$$

où $A$ (resp. $B$) parcourt l’ensemble des suites strictement croissantes de $p$ (resp. $q$) éléments de $[1, n]$, les $f_{A, B}$ étant des fonctions à valeurs dans $F$. Si $\omega$ est de classe $C^k$, avec $k \geqslant 1$, il en est de même des fonctions $f_{A, B}$ et l’on a

(12)
$$
d'\omega = \sum_{A, B} d'f_{A, B} \wedge dz^A \wedge d\bar{z}^B
$$

(13)
$$
d''\omega = \sum_{A, B} d''f_{A, B} \wedge dz^A \wedge d\bar{z}^B.
$$

[^1]: Lorsque $K=\mathbf{R}$ et $r=1$, $T(X)$ est un fibré vectoriel topologique (cf. Notations et conventions).
