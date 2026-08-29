---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 0
section_title: Points fixes des groupes de transformations affines
appendix: true
lang: fr
source: evt-i-v-fr
book_pages: EVT IV.72-EVT IV.76
pdf_pages: 0225-0233, 0258-0262
extraction: ocr
subsections:
    - "no": 1
      title: Cas des groupes résolubles
      page: 0
      pdf_page: 225
    - "no": 2
      title: Moyennes invariantes
      page: 40
      pdf_page: 226
    - "no": 3
      title: Le théorème de Ryll-Nardzewski
      page: 41
      pdf_page: 227
    - "no": 4
      title: Applications
      page: 44
      pdf_page: 230
statements: 10
exercises: 8
content_sha256: a50fe53e1e92cccf208144f33d5cc8cae97d257dd48338d2315f380c2f77246b
---

## APPENDICE

# Points fixes des groupes de transformations affines

### 1. Cas des groupes résolubles

Soient E un espace vectoriel réel, et K une partie convexe de E. On appelle transformation affine dans K toute application $u : K \to K$ telle que l’on ait

$$
u(t x + (1 - t) y) = t u(x) + (1 - t) u(y)
$$

pour $x, y$ dans K et tout nombre réel $t$ dans $[0, 1]$. De la relation (1), on déduit par récurrence

$$
u(\sum_{i \in I} t_i x_i) = \sum_{i \in I} t_i u(x_i)
$$

quels que soient l’ensemble fini I, les points $x_i$ de K et les nombres réels positifs $t_i$ tels que $\sum_{i \in I} t_i = 1$.

Si $u$ et $v$ sont deux transformations affines dans K, l’application $u \circ v$ est une transformation affine dans K. Si $v : E \to E$ est une application linéaire telle que $v(K) \subset K$, l’application $u : K \to K$ qui coïncide avec $v$ sur K est une transformation affine.

#### Théorème 1 (Markoff-Kakutani) {#evt-iv-a0-thm-1 .statement}

Soient E un espace vectoriel localement convexe séparé sur le corps $\mathbf{R}$, et K une partie convexe, compacte et non vide de E. Soit $\Gamma$ un ensemble de transformations affines dans K, continues, deux à deux permutables. Il existe un point a de K tel que $u(a) = a$ pour tout $u \in \Gamma$.

Pour tout $u \in \Gamma$, soit $K_u$ l’ensemble des $x \in K$ tels que $u(x) = x$. Montrons que $K_u$ est non vide. Soit $x$ un point de K ; pour tout entier $n \geq 1$, notons $x_n$ l’élément $\frac{1}{n} \sum_{i=0}^{n-1} u^i(x)$ de E. Comme K est convexe et stable par $u$, les points $x_n$ appartiennent à K et comme K est compact, il existe une valeur d’adhérence $a$ de la suite $(x_n)_{n \geq 1}$. L’application $y \mapsto u(y) - y$ de K dans E est continue, donc $u(a) - a$ est valeur d’adhérence de la suite $(u(x_n) - x_n)_{n \geq 1}$. Or on a $u(x_n) - x_n = \frac{1}{n} (u^n(x) - x)$. Comme

K est compact, donc borné (III, p. 3, prop. 2), la suite $(u^n(x) - x)_{n \geq 1}$ est bornée ; par suite, la suite $\left( \frac{1}{n} (u^n(x) - x) \right)_{n \geq 1}$ tend vers 0 (III, p. 3, prop. 3), et comme E est séparé, on a $u(a) - a = 0$. On a donc $a \in K_u$.

Chacun des ensembles $K_u$ est une partie fermée et convexe de l’espace compact K, et il s’agit de prouver que l’intersection $\bigcap_{u \in \Gamma} K_u$ est non vide. Il suffit donc de prouver que, pour $n \geq 1$, et $u_1, \ldots, u_n$ dans $\Gamma$, l’ensemble $K_{u_1} \cap \ldots \cap K_{u_n}$ n’est pas vide. Raisonnons par récurrence sur $n$, le cas $n = 1$ ayant été traité. Supposons alors $n \geq 2$ et posons $L = K_{u_1} \cap \ldots \cap K_{u_{n-1}}$. Par l’hypothèse de récurrence, L est une partie compacte et convexe non vide de E. Comme $u_n$ commute à $u_1, \ldots, u_{n-1}$, on a $u_n(L) \subset L$. Appliquant la première partie de la démonstration à la transformation affine induite par $u_n$ dans L, on conclut qu’il existe un point $a$ de L tel que $u_n(a) = a$; alors $a$ appartient à $K_{u_1} \cap \ldots \cap K_{u_n}$, qui est donc non vide.

#### Corollaire {#evt-iv-a0-n1-cor-1 .statement}

Soit G un groupe résoluble de transformations affines continues dans K. Il existe un point de K invariant par G.

D’après la définition d’un groupe résoluble (A, I, p. 71), il existe une suite finie décroissante $(G_i)_{0 \leq i \leq n}$ de sous-groupes distingués de G, telle que $G_0 = G, G_n = \{e\}$ et que le groupe $G_{i-1}/G_i$ soit commutatif pour $1 \leq i \leq n$. Notons $K_i$ l’ensemble des points fixes de $G_i$ dans K. On a $K_n = K$. De plus, pour $1 \leq i \leq n$, tout élément de $G_i$ induit la transformation identique sur $K_i$; on en déduit une action du groupe commutatif $G_{i-1}/G_i$ sur $K_i$; si $K_i$ est non vide, il résulte du th. 1 que l’ensemble $K_{i-1}$ des points fixes de $G_{i-1}/G_i$ dans $K_i$ est non vide. Par récurrence descendante sur $i$, on en déduit que $K_0$ n’est pas vide, d’où le corollaire.

### 2. Moyennes invariantes

Soit X un espace topologique. Notons $\mathcal{B}(X; \mathbf{R})$ l’espace vectoriel réel formé des applications continues et bornées de X dans $\mathbf{R}$. Muni de la norme $\|f\| = \sup_{x \in X} |f(x)|$, c’est un espace de Banach (TG, X, p. 21); c’est aussi un espace vectoriel ordonné, la relation $f \geq g$ signifiant « $f(x) \geq g(x)$ pour tout $x \in X$ ».

#### Définition 1 {#evt-iv-a0-def-1 .statement}

On appelle moyenne sur l’espace topologique X une forme linéaire positive $\mu$ sur l’espace $\mathcal{B}(X; \mathbf{R})$ telle que $\mu(1) = 1$.

\* Lorsque X est compact, une moyenne sur X est donc une mesure positive sur X telle que $\mu(X) = 1$. \*

#### Lemme 1 {#evt-iv-a0-lem-1 .statement}

L’ensemble K des moyennes sur X est la partie de la boule unité du dual de l’espace de Banach $E = \mathcal{B}(X; \mathbf{R})$ dont les éléments sont les formes linéaires $\mu$ telles que $\mu(1) = 1$. C’est une partie de $E'$, convexe et compacte pour $\sigma(E', E)$.

Soit $\mu$ une forme linéaire sur E, telle que $\mu(1) = 1$. Pour toute fonction $f \in E$, on définit la fonction $f' \in E$ par $f'(x) = \|f\| - f(x)$ ($x \in X$). Supposons d’abord que $\mu$ soit une moyenne ; pour tout $f \in E$, on a $f' \geq 0$, d’où $\mu(f') \geq 0$, c’est-à-dire $\mu(f) \leq \|f\|$; on a donc $\|\mu\| \leq 1$. Réciproquement, supposons que $\mu$ appartienne à $E'$, et que $\|\mu\| \leq 1$; pour toute fonction positive $f \in E$, on a $\mu(f') \leq \|f'\|$, d’où
$$
\|f\| - \mu(f) = \mu(f') \leq \|f'\| \leq \|f\|,
$$
et finalement $\mu(f) \geq 0$; par suite, $\mu$ est une moyenne.

Il est clair que $K$ est convexe ; qu’il soit compact pour $\sigma(E', E)$ résulte du cor. 3 de III, p. 17.

Soit $\Gamma$ un ensemble d’applications continues de $X$ dans $X$, commutant deux à deux. Soit $\gamma \in \Gamma$. Pour toute fonction $f \in E$, on a $f \circ \gamma \in E$; on définit donc une transformation affine $u_\gamma$ dans l’ensemble $K$ des moyennes sur $X$ par
$$
u_\gamma \mu(f) = \mu(f \circ \gamma) \quad (\mu \in K, f \in E).
$$
Si l’on munit $K$ de la topologie induite par $\sigma(E', E)$, l’application $u_\gamma$ est continue. Si $\gamma$ est un homéomorphisme, $u_\gamma \mu$ se déduit de $\mu$ par transport de structure. Enfin, on a $u_\gamma u_{\gamma'} = u_{\gamma' \gamma} u_\gamma$ quels que soient $\gamma, \gamma'$ dans $\Gamma$. D’après le th. de Markoff-Kakutani (IV, p. 39, th. 1), *il existe donc une moyenne $\mu$ sur $X$, telle que $u_\gamma \mu = \mu$ pour tout $\gamma \in \Gamma$ ; autrement dit, $\mu$ satisfait à la relation $\mu(f) = \mu(f \circ \gamma)$ pour $f \in E$ et $\gamma \in \Gamma$.

Le corollaire du th. 1 (IV, p. 40) entraîne de manière analogue le résultat suivant :

#### Proposition 1 {#evt-iv-a0-prop-1 .statement}

*Soient $X$ un espace topologique et $G$ un groupe résoluble. On suppose que $G$ opère à gauche sur $X$, de sorte que, pour tout $g \in G$, l’application $x \mapsto g.x$ de $X$ dans $X$ soit continue. Il existe alors sur $X$ une moyenne invariante par $G$.

#### Corollaire {#evt-iv-a0-n2-cor-1 .statement}

*Soit $G$ un groupe topologique résoluble. Il existe sur $G$ une moyenne invariante par les translations à gauche et à droite.

Il suffit d’appliquer la prop. 1 au groupe résoluble $G \times G$ agissant sur $G$ par $(g, g').x = gx{g'}^{-1}$.

### 3. Le théorème de Ryll-Nardzewski

Dans ce numéro, on note $E$ un espace *normé* sur le corps $\mathbf{R}$ et $\mathcal{T}$ une topologie localement convexe séparée sur $E$, pour laquelle la norme de $E$ soit *semi-continue inférieurement*. Ces hypothèses sont notamment remplies dans les cas suivants :
  a) $\mathcal{T}$ est la topologie déduite de la norme de l’espace normé $E$.
  b) $\mathcal{T}$ est la topologie affaiblie $\sigma(E, E')$ de l’espace normé $E$.
  c) $E$ est le dual d’un espace normé $F$ et l’on a $\mathcal{T} = \sigma(F', F)$.
  d) Il existe deux espaces normés $F_1$ et $F_2$ tels que $E = \mathscr{L}(F_1; F_2)$ et que $\mathcal{T}$ soit la topologie de la convergence simple.

Sauf mention expresse du contraire, les notions topologiques se réfèrent à la topologie $\mathcal{T}$.

Soit K une partie convexe de E. On suppose que K est compacte (pour la topologie $\mathcal{T}$), et que c’est un espace de type dénombrable pour la distance déduite de la norme de E.

#### Lemme 2 {#evt-iv-a0-lem-2 .statement}

On suppose que K contient au moins deux points. Pour tout $\varepsilon > 0$, il existe une partition de K en deux sous-ensembles non vides $K_1$ et $K_2$, ayant les propriétés suivantes :

a) $K_1$ est convexe et compact ;
b) on a $\|x_1 - x_2\| < \varepsilon$ quels que soient $x_1$ et $x_2$ dans $K_2$.

Soit L l’adhérence de l’ensemble des points extrémaux de K. D’après le th. de Krein-Milman (II, p. 59, th. 1), K est l’enveloppe fermée convexe de L. Comme K contient au moins deux points, il en est de même de L. Pour tout $x \in L$, soit $A_x$ l’ensemble des $y \in L$ tels que $\|x - y\| \leq \varepsilon/4$. D’après l’hypothèse faite sur K, il existe une partie dénombrable D de L telle que $L = \bigcup_{x \in D} A_x$. Comme la norme est semi-continue inférieurement, chacun des ensembles $A_x$ est fermé. Appliquons le th. de Baire (TG, IX, p. 55, th. 1) à l’espace compact L : il existe un point $a$ de D et une partie ouverte U de E tels que $L \cap U$ soit non vide et contenu dans $A_a$. Comme L contient au moins deux points, et que E est séparé, on peut choisir U de sorte que $L \notin U$.

Soit M l’enveloppe fermée convexe de $L \cap \complement U$. Pour tout nombre réel $t$ tel que $0 < t < 1$, notons $M_t$ l’ensemble des vecteurs de la forme $tx_1 + (1-t)x_2$ avec $x_1 \in M$ et $x_2 \in K$ ; c’est une partie non vide, convexe et compacte de K. *Démontrons par l’absurde qu’on a* $M_t \neq K$. Supposons qu’on ait $M_t = K$ ; alors tout point extrémal $x$ de K appartient à $M_t$, donc s’écrit sous la forme $x = tx_1 + (1-t)x_2$ avec $x_1 \in M$ et $x_2 \in K$. Ceci entraîne $x = x_1 = x_2$, d’où $x \in M$. D’après le th. de Krein-Milman (II, p. 59, th. 1), on a donc $K = M$, et K est l’enveloppe fermée convexe de $L \cap \complement U$. D’après II, p. 59, corollaire, ceci entraîne $L \subset L \cap \complement U$, en contradiction avec la relation $L \cap U \neq \varnothing$.

Posons $d = \sup_{x \in K, y \in K} \|x - y\|$ et choisissons un nombre réel $t$ tel que $0 < t < 1$ et $t < \varepsilon/4d$. Posons $K_1 = M_t$ et $K_2 = K - M_t$. D’après ce qui précède, les ensembles $K_1$ et $K_2$ sont non vides, et $K_1$ est convexe et compact. Soit $M'$ l’enveloppe fermée convexe de $L \cap U$. Comme K est l’enveloppe fermée convexe de l’ensemble $L = (L \cap \complement U) \cup (L \cap U)$, c’est aussi l’enveloppe fermée convexe de $M \cup M'$. Soient $x_1$ et $x_2$ deux points de $K_2$ ; pour $i = 1, 2$, il existe donc $y_i \in M, z_i \in M'$ et un nombre réel $\alpha_i$ tels que $0 \leq \alpha_i \leq 1$ et $x_i = \alpha_i y_i + (1-\alpha_i) z_i$. Si l’on avait $\alpha_i \geq t$, on aurait $x_i = ty_i + (1-t) \left\{ \frac{\alpha_i - t}{1-t} y_i + \frac{1-\alpha_i}{1-t} z_i \right\}$ contrairement à l’hypothèse $x_i \notin M_t$. On a donc $\alpha_i < t$ pour $i = 1, 2$, d’où

$$
\|x_i - z_i\| = \|\alpha_i (y_i - z_i)\| = \alpha_i \|y_i - z_i\| \leq \alpha_i d < dt < \varepsilon/4 .
$$

Pour tout point z de M', on a $\|z - a\| \leq \varepsilon/4$ puisque $L \cap U \subset A_a$, d’où en particulier $\|z_i - a\| \leq \varepsilon/4$. On a donc

$$
\|x_1 - x_2\| \leq \sum_{i=1}^2 (\|x_i - z_i\| + \|z_i - a\|) < \varepsilon .
$$

Ceci achève la démonstration.

#### Lemme 3 {#evt-iv-a0-lem-3 .statement}

Soit G un groupe de transformations affines continues (pour $\mathcal{T}$) dans K. On suppose que K est non vide et qu’on a $\|gx - gy\| = \|x - y\|$ pour x, y dans K et g dans G. Il existe un point de K invariant par G.

Soit $\mathfrak{J}$ l’ensemble des parties de K qui sont non vides, convexes, fermées et stables pour G. Si $(L_\alpha)_{\alpha \in I}$ est une famille totalement ordonnée par inclusion d’éléments de $\mathfrak{J}$, l’ensemble $L = \bigcap_{\alpha \in I} L_\alpha$ appartient à $\mathfrak{J}$. Par suite (E, III, p. 20, th. 2), il existe un élément L de $\mathfrak{J}$, minimal pour la relation d’inclusion. Il s’agit de prouver que L est réduit à un point.

Raisonnons par l’absurde, en supposant que L contienne au moins deux points distincts $x_1$ et $x_2$; posons $x = (x_1 + x_2)/2$ et $\varepsilon = \|x_1 - x_2\|/2$. L’ensemble convexe et compact L est de type dénombrable pour la distance déduite de la norme (TG, IX, p. 19, corollaire). On peut donc lui appliquer le lemme 2 et trouver une partie convexe et compacte $L_1$ de L, distincte de $\varnothing$ et de L, possédant la propriété suivante :

(A) Quels que soient $y_1$ et $y_2$ dans $L - L_1$, on a $\|y_1 - y_2\| < \varepsilon$.

Montrons par l’absurde qu’on a $gx \in L_1$ pour tout $g \in G$. Soit donc $g \in G$ tel que $gx \in L - L_1$; pour $i = 1, 2$, on a

$$
\|gx_i - gx\| = \|x_i - x\| = \|x_1 - x_2\|/2 = \varepsilon .
$$

D’après la propriété (A), on a donc $gx_i \in L_1$. Comme $L_1$ est convexe, on en déduit que $gx = (gx_1 + gx_2)/2$ appartient à $L_1$, contrairement à l’hypothèse faite.

Soit $L'$ l’enveloppe fermée convexe de l’orbite $Gx$ de x. L’ensemble $L'$ appartient à $\mathfrak{J}$. D’après ce qui précède, on a $L' \subset L_1$, d’où $L' \subset L$, $L' \neq L$. Ceci contredit le caractère minimal de L et achève la démonstration.

#### Théorème 2 (Ryll-Nardzewski) {#evt-iv-a0-thm-2 .statement}

Soient E un espace normé et K une partie convexe non vide de E, compacte pour la topologie affaiblie $\sigma(E, E')$. Soit G un groupe de transformations affines isométriques de K. Il existe un point de K invariant par G.

Pour tout $g \in G$, notons $K_g$ l’ensemble des points x de K tels que $gx = x$; munissons K de la topologie affaiblie ; chaque ensemble $K_g$ est convexe et fermé dans l’espace compact K. Il s’agit de prouver que l’intersection $\bigcap_{g \in G} K_g$ est non vide ; pour cela, il suffit de prouver que l’ensemble $K_{g_1} \cap \ldots \cap K_{g_n}$ est non vide quels que soient $g_1, \ldots, g_n$ dans G. Fixons $g_1, \ldots, g_n$ et notons H le sous-groupe de G engendré par $\{g_1, \ldots, g_n\}$. Choisissons un point a de K et notons L l’enveloppe fermée convexe de l’orbite Ha de a. Soit D l’ensemble dénombrable des éléments de la forme $\lambda_1 h_1 a + \cdots + \lambda_m h_m a$, où $\lambda_1, \ldots, \lambda_m$ sont des nombres rationnels positifs tels que $\lambda_1 + \cdots + \lambda_m = 1$, et $h_1, \ldots, h_m$ des éléments de $H$. L’adhérence $\overline{D}$ de $D$ pour la topologie forte est convexe, donc elle est fermée pour $\sigma(E, E')$ (IV, p. 4, prop. 2) ; on a donc $\overline{D} = L$, ce qui prouve que $L$ est un espace métrique de type dénombrable pour la distance $(x, y) \mapsto \| x - y \|$. On peut donc appliquer le lemme 2. Il existe un point $b$ de $L$ invariant par $H$, d’où $b \in K_{g_1} \cap \ldots \cap K_{g_n}$.

#### Corollaire {#evt-iv-a0-n3-cor-1 .statement}

*Soient E un espace de Banach réflexif, G un groupe d’automorphismes de l’espace normé E, et K une partie de E. On suppose que K est convexe, fermée, non vide, bornée, et stable par G. Il existe alors dans K un point invariant par G.*

Comme E est réflexif, K est compacte pour $\sigma(E, E')$ (IV, p. 15, th. 1). De plus, tout élément de G appartient à $\mathcal{L}(E)$.

### 4. Applications

\* A) Représentations unitaires des groupes :

Soient E un espace hilbertien complexe, G un groupe et $\pi$ une représentation unitaire de G dans E, c’est-à-dire un homomorphisme de G dans le groupe des automorphismes de E. Notons $E^G$ le sous-espace hilbertien de E formé des vecteurs invariants par $\pi(G)$. Pour tout $x \in E$, soit $K_x$ l’enveloppe fermée convexe de l’orbite de $x$. Fixons un point $x$ de E.

Montrons qu’il existe dans $K_x$ un unique point invariant par $\pi(G)$, à savoir la projection de $x$ sur $E^G$. D’après IV, p. 44, corollaire (appliqué à l’espace vectoriel réel sous-jacent à E), il existe un point de $K_x$ invariant par $\pi(G)$; soit $a$ un tel point, d’où $a \in E^G$. Soit P l’ensemble des $y \in E$ tels que $y - x$ soit orthogonal à $E^G$; on voit aussitôt que P est convexe, fermé et invariant par $\pi(G)$; on a $x \in P$, d’où $K_x \subset P$ et finalement $a \in P$. Autrement dit, $a - x$ est orthogonal à $E^G$; par suite $a$ est la projection de $x$ sur $E^G$. \*

\* B) Trace d’un opérateur dans un espace hilbertien :

Supposons maintenant que la représentation $\pi$ soit *irréductible*, c’est-à-dire qu’il n’existe aucun sous-espace hilbertien de E, distinct de $\{0\}$ et de E, et invariant par $\pi(G)$. Soit $F = \mathcal{L}^2(E)$ l’espace hilbertien des endomorphismes de Hilbert-Schmidt de E, avec le produit scalaire $\langle u|v \rangle = \mathrm{Tr}(u^*v)$. Définissons une représentation unitaire $\lambda$ de G dans F par la formule

(3)
$$
\lambda(g).u = \pi(g)\, u \pi(g)^{-1} \quad (u \in F,\ g \in G)
$$

L’espace $F^G$ des éléments de E invariants par $\lambda(G)$ se compose des endomorphismes $u$ de Hilbert-Schmidt de E qui commutent à $\pi(g)$ pour tout $g \in G$. D’après le lemme de Schur, un tel $u$ est une homothétie. On doit donc distinguer deux cas :
1) si E est de dimension infinie, on a $F^G = \{0\}$;
2) si E est de dimension finie, on a $F = \mathcal{L}(E)$ et $F^G = \mathbf{C}.1_E$.

Par application du résultat de A) à la représentation unitaire $\lambda$, on obtient le théorème suivant :

Soit $u \in \mathcal{L}^2(E)$, et soit $A_u$ l’enveloppe fermée convexe dans $\mathcal{L}^2(E)$ de l’ensemble des endomorphismes $\pi(g)\ u\pi(g)^{-1}$ de $E$, où $g$ parcourt $G$. Si $E$ est de dimension infinie, on a $0 \in A_u$. Si $E$ est de dimension finie $d$, il existe une unique homothétie dans $A_u$, à savoir la projection $\frac{1}{d}\ \mathrm{Tr}(u).\ 1_E$ de $u$ sur le sous-espace $\mathbf{C}.1_E$ de $\mathcal{L}^2(E)$.

C) Mesure de Haar d’un groupe compact :

Soit $G$ un groupe compact, et soit $E = \mathcal{C}(X ; \mathbf{R})$ l’espace de Banach des fonctions continues $f$ sur $G$, à valeurs réelles, muni de la norme

$$
\|f\| = \sup_{x \in G} |f(x)| .
$$

Pour tout $x \in G$, on définit les automorphismes $\gamma_x$ et $\delta_x$ de $E$ par les formules

$$
\gamma_x f(y) = f(x^{-1}y) , \quad \delta_x f(y) = f(yx)
$$

(pour $y \in G,\ f \in E$).

Soit $f \in E$; on note $\Gamma_f$ (resp. $\Delta_f$) l’enveloppe fermée convexe, dans $E$, de l’ensemble des fonctions $\gamma_x f$ (resp. $\delta_x f$) pour $x$ parcourant $G$. Nous allons prouver qu’il existe une unique fonction constante $\mu(f)$ appartenant à $\Gamma_f$, une unique fonction constante $\mu'(f)$ appartenant à $\Delta_f$ et que ces constantes sont égales.

Il est clair qu’une fonction continue sur $G$ est invariante par les automorphismes $\gamma_x$ (resp. $\delta_x$) de $E$ si et seulement si elle est constante. Par ailleurs, l’ensemble des fonctions $\gamma_x f$ (resp. $\delta_x f$) pour $x$ dans $G$, est compact dans $E$, car l’application $x \mapsto \gamma_x f$ (resp. $x \mapsto \delta_x f$) de $G$ dans $E$ est continue (TG, X, p. 28, th. 3). Il en résulte (II, p. 27, prop. 3) que $\Gamma_f$ (resp. $\Delta_f$) est un ensemble compact dans $E$ pour la topologie déduite de la norme, donc pour $\sigma(E, E')$. D’après le th. de Ryll-Nardzewski (IV, p. 43, th. 2), il existe des fonctions constantes dans $\Gamma_f$ et $\Delta_f$. Il reste à prouver que, si $c_1 \in \Gamma_f$ et $c_2 \in \Delta_f$ sont constantes, on a $c_1 = c_2$.

Soit $\varepsilon > 0$. Par hypothèse, il existe des points $x_1, \ldots, x_n,\ y_1, \ldots, y_m$ de $G$ et des nombres réels positifs $\lambda_1, \ldots, \lambda_n,\ \mu_1, \ldots, \mu_m$ tels que

$$
\lambda_1 + \cdots + \lambda_n = \mu_1 + \cdots + \mu_m = 1 .
$$

$$
\sup_{x \in G} \left| \sum_{i=1}^n \lambda_i f(x_i x) - c_1 \right| \leq \varepsilon ,
$$

$$
\sup_{x \in G} \left| \sum_{j=1}^m \mu_j f(xy_j) - c_2 \right| \leq \varepsilon .
$$

Posons $r = \sum_{i,j} \lambda_i \mu_j f(x_i y_j)$. On a $r - c_1 = \sum_{j=1}^m \mu_j a_j$ avec $a_j = \sum_{i=1}^n \lambda_i f(x_i y_j) - c_1$; d’après (7), on a $|a_j| \leq \varepsilon$ pour $1 \leq j \leq m$, d’où $|r - c_1| \leq \varepsilon$. On démontre de manière analogue l’inégalité $|r - c_2| \leq \varepsilon$, d’où $|c_1 - c_2| \leq 2\varepsilon$. Vu l’arbitraire de $\varepsilon$, on a $c_1 = c_2$ comme annoncé.

D’après la définition de $\mu(f)$, on peut trouver pour tout $\varepsilon > 0$ des nombres positifs $\lambda_1, ..., \lambda_n$, de somme 1 et des éléments $x_1, ..., x_n$ de $G$ tels que l’on ait
$$
| \sum_{i=1}^n \lambda_i f(x_i x) - \mu(f) | \leq \varepsilon \text{ pour tout } x \in G.
$$
Il est immédiat que, pour $f, g$ dans $E$ et tout scalaire $\lambda$, on a $\Gamma_{f+g} \subset \Gamma_f + \Gamma_g$ et $\Gamma_{\gamma_f} = \lambda \Gamma_f$, d’où l’on déduit aussitôt les relations $\mu(f+g) = \mu(f) + \mu(g)$ et $\mu(\lambda f) = \lambda \mu(f)$. Donc l’application $\mu : f \mapsto \mu(f)$ de $E$ dans $\mathbf{R}$ est une moyenne sur l’espace compact $G$ (IV, p. 40); \* autrement dit, $\mu$ est une mesure positive sur $G$ telle que $\mu(G) = 1$*. Il est immédiat que $\mu$ est invariante par les translations à gauche de $G$, et l’égalité $\mu(f) = \mu'(f)$ implique que $\mu$ est aussi invariante par les translations à droite. \* Autrement dit $\mu$ est une mesure de Haar à gauche et à droite sur $G$ (INT, VII, § 1, no 2, déf. 2). \*

\* D) Existence de mesures invariantes :

Soient $X$ un espace topologique séparé, $\mu$ une mesure positive et bornée sur $X$, et $G$ un groupe d’homéomorphismes de $X$. On suppose que, pour tout $g \in G$, la mesure $g.\mu$ image de $\mu$ par l’application $g : X \to X$ est de base $\mu$. Soit $u_g$ une fonction positive $\mu$-intégrable sur $X$ telle que $g.\mu = u_g.\mu$. On suppose aussi qu’il existe deux fonctions $\mu$-intégrables positives $\varphi$ et $\psi$ sur $X$, non $\mu$-négligeables et telles que l’on ait $\varphi \leq u_g \leq \psi$ $\mu$-presque partout quel que soit $g \in G$. Nous allons prouver qu’il existe une mesure positive et bornée $v \neq 0$ sur $X$, de base $\mu$, invariante par $G$.

Soit $P$ la partie de l’espace de Banach $E = L^1(X, \mu)$ formée des classes des fonctions $f$ telles que l’on ait $\varphi \leq f \leq \psi$ $\mu$-presque partout. Alors $P$ est compacte pour la topologie affaiblie $\sigma(E, E')$. L’application $h \mapsto h.\mu$ de $P$ dans l’espace de Banach $F = \mathcal{M}^b(X)$ des mesures réelles bornées sur $X$, est une bijection de $P$ sur un sous-ensemble $P_1$ de $F$, convexe et compact pour la topologie $\sigma(F, F')$. Par hypothèse, on a $g.\mu \in P_1$ pour tout $g \in G$. Soit $K$ l’enveloppe fermée convexe de l’ensemble des mesures $g.\mu$. Pour tout $g \in G$, l’application $v \mapsto g.v$ est une transformation affine isométrique de $K$. D’après le th. de Ryll-Nardzewski (IV, p. 43, th. 2), il existe donc une mesure $v \in K$ invariante par $G$. On a $\varphi.\mu \leq v$, d’où $v \neq 0$. \*

Exercises

## EXERCICES {#evt-iv-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
