---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 5
section_title: Mesures sur les espaces complètement réguliers
lang: fr
source: int-ix-fr
pdf_pages: 0053-0068, 0104-0108
extraction: ocr
subsections:
    - "no": 1
      title: Mesures et fonctions continues bornées
      page: 0
      pdf_page: 53
    - "no": 2
      title: Mesures bornées et formes linéaires sur $C^b(T)$
      page: 0
      pdf_page: 56
    - "no": 3
      title: Convergence étroite des mesures bornées
      page: 0
      pdf_page: 57
    - "no": 4
      title: 'Application: propriétés topologiques de l’espace $\mathcal{M}^b_+(T)$'
      page: 0
      pdf_page: 59
    - "no": 5
      title: Critère de compacité pour la convergence étroite
      page: 0
      pdf_page: 61
    - "no": 6
      title: Convergence étroite des mesures et convergence compacte des fonctions
      page: 0
      pdf_page: 63
    - "no": 7
      title: 'Application: transformation de Laplace'
      page: 0
      pdf_page: 64
statements: 33
exercises: 13
content_sha256: bde2f8b9cc3196f90c2fc45cac28dee6c891f97b0926f20cbde64149e358dd83
---

## § 5. Mesures sur les espaces complètement réguliers

*Si T est un espace topologique, et F un espace de Banach, la notation $C^b(T; F)$ désigne l'espace des fonctions continues bornées sur T à valeurs dans F, muni de la norme de la convergence uniforme. Si F = R, cette notation est abrégée en $C^b(T)$, ou $C^b$ s'il n'y a pas d'ambiguïté, et l'on désigne par $C^b_+(T)$ ou $C^b_+$ le cône des fonctions positives dans $C^b(T)$. L'espace des mesures complexes bornées sur T sera noté $M^b(T, \mathbf{C})$, l'espace des mesures réelles bornées $M^b(T)$ ou $M^b$, et le cône des mesures positives bornées $M^b_+(T)$ ou $M^b_+$.*

### 1. Mesures et fonctions continues bornées

Rappelons (*Top. gén.*, chap. IX, 3e éd., § 1, n° 5, déf. 4) qu'un espace topologique T est dit *complètement régulier* s'il est uniformisable et séparé. Cela équivaut à dire (*loc. cit.*, prop. 3) que T est homéomorphe à un sous-espace d'un espace compact. Si T est complètement régulier, toute fonction semi-continue inférieurement positive f sur T est l'enveloppe supérieure de l'ensemble filtrant croissant des éléments de $C^b_+(T)$ majorés par f, toute fonction semi-continue supérieurement positive et bornée g est l'enveloppe inférieure de l'ensemble filtrant décroissant des éléments de $C^b_+(T)$ qui majorent g (*loc. cit.*, § 1, n° 7, prop. 7). Nous aurons aussi besoin du lemme suivant:

*Lemme 1. — Soient T un espace complètement régulier, K une partie compacte de T et U une partie ouverte de T contenant K.*

a) Il existe une partie ouverte $U'$ de $T$ tel que $K \subset U' \subset \overline{U}' \subset U$.

b) Soit $f$ une fonction continue définie sur $K$ à valeurs dans un intervalle $I$ de $\mathbf{R}$ (resp. dans $\mathbf{C}$). Il existe une fonction $f'$ continue et bornée sur $T$, à valeurs dans $I$ (resp. dans $\mathbf{C}$) qui prolonge $f$ et s’annule dans $T - U$.

Il suffit de traiter le cas où $T$ est un sous-espace d’un espace compact $X$. Soit $V$ une partie ouverte de $X$ tel que $V \cap T = U$; désignons par $V'$ un ensemble ouvert dans $X$ contenant $K$ tel que $\overline{V}' \subset V$, par $g$ une fonction continue sur $X$, à valeurs dans $I$ (resp. dans $\mathbf{C}$) prolongeant $f$ et nulle sur $X - V$ (*Top. gén.*, chap. IX, 3\textsuperscript{e} éd., § 4, n° 1, prop. 1). On satisfait à *a*) en prenant $U' = V' \cap T$, et à *b*) en prenant pour $f'$ la restriction de $g$ à $T$.

#### Proposition 1 {#int-ix-s5-prop-1 .statement}

*Soit $T$ un espace complètement régulier.*

*a*) *Soient $\mu$ une mesure positive sur $T$, et $f$ une fonction numérique $\geqslant 0$ définie dans $T$ et semi-continue inférieurement (resp. semi-continue supérieurement finie à support compact). On a alors*

$$
\mu^\bullet(f) = \sup_{g \in I_f} \mu^\bullet(g) \quad (\text{resp. } \mu^\bullet(f) = \inf_{g \in S_f} \mu(g))
$$

$I_f$ (resp. $S_f$) désignant l’ensemble des fonctions continues bornées telles que $0 \leqslant g \leqslant f$ (resp. $g \geqslant f$).

*b*) *Soient $\theta$ une mesure complexe sur $T$, et $f$ une fonction numérique $\geqslant 0$ définie dans $T$ et semi-continue inférieurement. On a alors*

$$
|\theta|^\bullet(f) = \sup_g |\theta(g)|,
$$

$g$ parcourant l’ensemble des fonctions complexes, continues, bornées et $|\theta|$-intégrables telles que $|g| \leqslant f$.

La première des formules (1) est évidente, car $I_f$ est un ensemble filtrant croissant de fonctions continues dont l’enveloppe supérieure est $f$, et on peut appliquer la prop. 5 du § 1, n° 6. La même proposition entraînera la seconde formule, si nous montrons que $S_f$ contient une fonction continue bornée $\mu$-intégrable. Soient donc $K$ le support de $f$ et $M$ la borne supérieure de $f$; comme $K$ est compact, $M$ est fini (*Top. gén.*, chap. IV, 3\textsuperscript{e} éd., § 6, n° 2, th. 3). Soit $U$ un ensemble ouvert contenant $K$ et tel que $\mu^\bullet(U) < +\infty$; il existe (lemme 1) une fonction continue $g$ à valeurs dans $[0, M]$, égale à $M$ sur $K$ et nulle hors de $U$; on a alors $g \in S_f$ et $\mu^\bullet(g) \leqslant M \mu^\bullet(U) < +\infty$.

Passons à *b*). Il suffit évidemment de montrer que l’on a $|\theta|^\bullet(f) \leqslant \sup_g |\theta(g)|$.

Soient deux nombres réels $a$ et $b$ tels que $a < b < |\theta|^\bullet(f)$. D’après (1), il existe une fonction $h \in \mathcal{C}_+^b(T)$ telle que $h \leqslant f$ et $|\theta|^\bullet(h) > b$; désignons par $M$ la borne supérieure de $h$. D’après la définition de $|\theta|^\bullet$ (§ 1, n° 2, déf. 4), il existe une partie compacte $K$ de $T$ telle que $|\theta|_K^\bullet(h_K) > b$. Il existe alors une fonction continue complexe $j$ sur $K$ telle que $|j| \leqslant h_K$ et que $|\theta_K(j)| > b$ (chap. III, 2\textsuperscript{e} édit., § 1, n° 6). Choisissons un ensemble ouvert $U$ contenant $K$ et tel que $|\theta|^\bullet(U - K) \leq \frac{b - a}{M}$ (§ 1, n° 9, prop. 13 et 14); prolongeons j en une fonction complexe k continue sur T, nulle hors de U (lemme 1); pour tout $t \in T$, posons

(3)
$$
g(t) = \begin{cases}
k(t) & \text{si } |k(t)| \leq h(t) \\
\frac{k(t)}{|k(t)|} h(t) & \text{si } |k(t)| > h(t).
\end{cases}
$$

On a évidemment $|g| \leq h \leq f$, et $g = j$ dans K, donc $||\theta_K(j)|| - |\theta(g)|| = ||\theta(j^0)| - |\theta(g)|| \leq |\theta|^\bullet(|j^0 - g|) \leq M. |\theta|^\bullet(U - K) \leq b - a$, et par conséquent $|\theta(g)| > a$. Montrons d'autre part que g est une fonction continue: comme a est assujetti seulement à la condition $a < |\theta|^\bullet(f)$, cela entraînera que le second membre de (2) majore le premier, d'où la proposition. Or soit F (resp. F') l'ensemble des $t \in T$ tels que $|k(t)| \leq h(t)$ (resp. $|k(t)| \geq h(t)$). Ces ensembles étant fermés, et leur réunion étant T, il nous suffit de montrer que $g_F$ et $g_{F'}$ sont continues: or cette propriété est évidente pour $g_F = k_F$, et elle l'est pour $g_{F'}$ aux points où $k(t) \neq 0$; d'autre part, si $t \in F'$ est tel que $k(t) = 0$, on a aussi $h(t) = 0$, et l'inégalité $|g| \leq h$ entraîne que g est continue au point t.

#### Remarque 1 {#int-ix-s5-n1-rem-1 .statement}

Soit f une fonction semi-continue inférieurement positive, et soit $J_f$ l'ensemble des fonctions continues bornées positives *nulles hors d'un ouvert* $\mu$-intégrable et majorées par f. On peut montrer que f est l'enveloppe supérieure de $J_f$ et que $\mu^\bullet(f) = \sup_{g \in J_f} \mu(g)$.

#### Remarque 2 {#int-ix-s5-n1-rem-2 .statement}

Si la mesure $\mu$ est bornée, la formule $\mu^\bullet(f) = \inf_{g \in S_f} \mu(g)$ est évidemment valable pour toute fonction f, semi-continue supérieurement, positive et bornée.

#### Proposition 2 {#int-ix-s5-prop-2 .statement}

Soient $\eta$ et $\eta'$ deux mesures complexes sur un espace complètement régulier T, telles que l'on ait $\eta(f) = \eta'(f)$ pour toute fonction $f \in C^b(T)$, intégrable pour $|\eta|$ et $|\eta'|$. On a alors $\eta = \eta'$.

Reprenons la démonstration de la seconde partie de la proposition 1, en posant $\theta = \eta - \eta'$. Nous pouvons imposer à l'ouvert U d'être intégrable pour $|\eta|$ et $|\eta'|$. La fonction g est alors intégrable pour ces deux mesures, et la relation $\theta(g) = 0$ entraîne $a < 0$; on a donc $|\theta|^\bullet(f) = 0$ pour toute fonction f semi-continue inférieurement positive, d'où finalement $|\theta| = 0$, en prenant $f = +\infty$.

#### Proposition 3 {#int-ix-s5-prop-3 .statement}

Soit $\mu$ une mesure positive sur un espace complètement régulier T, et soit $p \in [1, +\infty[$. L'espace $\mathcal{H}$ des fonctions $f \in C^b(T)$, dont le support est contenu dans un ouvert $\mu$-intégrable, est dense dans $L^p(\mu)$.

D'après la prop. 15 du § 1, n° 10, il nous suffit de montrer que si K est compact dans T, et si g est le prolongement par 0 à T d'une fonction de $C^+(K)$, comprise entre 0 et 1, il existe une fonction $f \in C^b_+(T)$, à support contenu dans un ouvert $\mu$-intégrable, et telle que $\|f - g\|_p$ soit arbitrairement petit. Or soient $\varepsilon$ un nombre $> 0$, U un voisinage ouvert de K tel que $\mu^\bullet(U - K) < \varepsilon$, V un voisinage ouvert de K tel que $\overline{V} \subset U$, f une fonction à valeurs dans $[0, 1]$, continue, égale à g sur K et à 0 hors de V (lemme 1). La fonction $|f - g|^p$ est alors majorée par $\varphi_{U-K}$; on a donc $\|f - g\|_p \leq \varepsilon^{1/p}$, ce qui établit la proposition.

Remarque 3). — On a un énoncé analogue pour les fonctions à valeurs dans un espace de Banach F : le sous-espace $\mathcal{H} \otimes F$ de $C^b(T; F)$ est dense dans $\mathcal{L}_F^p(\mu)$.

#### Proposition 4 {#int-ix-s5-prop-4 .statement}

Pour qu'une mesure complexe bornée $\theta$ sur un espace complètement régulier T soit positive, il faut et il suffit qu'on ait $\theta(f) \geq 0$ pour toute fonction $f \in C^b_+(T)$.

La nécessité est évidente. Pour établir la suffisance, reprenons la démonstration de la proposition précédente, en prenant $p = 1$ et $\mu = |\theta|$; les notations étant les mêmes, la relation $\mu^*(|f - g|) \leq \varepsilon$ et l'inégalité $\theta(f) \geq 0$ entraînent $\theta_K(g_K) = \theta(g) \geq -\varepsilon$; comme $g_K$ est un élément de $C(K)$ compris entre 0 et 1 arbitraire, la mesure $\theta_K$ est positive; l'ensemble compact K étant arbitraire, cela signifie que $\theta$ est positive.

### 2. Mesures bornées et formes linéaires sur $C^b(T)$

#### Proposition 5 {#int-ix-s5-prop-5 .statement}

Soient T un espace complètement régulier, et I une forme linéaire complexe continue sur l'espace normé $C^b(T; \mathbf{C})$. Pour qu'il existe une mesure complexe bornée $\theta$ sur T telle que $\theta(f) = I(f)$ pour tout $f \in C^b(T; \mathbf{C})$, il faut et il suffit que la condition suivante soit vérifiée :
(M) Pour tout nombre $\varepsilon > 0$, il existe une partie compacte K de T telle que les relations $g \in C^b(T, \mathbf{C}), |g| \leq 1, g_K = 0$ entraînent $|I(g)| \leq \varepsilon$.
La mesure $\theta$ est alors unique.

L'unicité résulte de la prop. 2 du n° 1. Montrons que la condition (M) est nécessaire. Soit $\theta$ une mesure complexe bornée; soit K un ensemble compact tel que $|\theta|^*(T - K) \leq \varepsilon$ (§ 1, n° 2, Remarque 3). Les hypothèses $|g| \leq 1, g_K = 0$ entraînent $|g| \leq \varphi_{CK}$, donc $|\theta(g)| \leq |\theta|^*(\varphi_{CK}) \leq \varepsilon$.

Passons à la démonstration de la suffisance. Soit X le compactifié de Stone-Čech de T (Top. gén., chap. IX, 3e éd., § 1, n° 6). Pour toute fonction $f \in C^b(X, \mathbf{C})$, posons $\nu(f) = I(f_T)$; nous définissons ainsi une forme linéaire continue $\nu$ sur $C^b(X, \mathbf{C})$, c'est-à-dire une mesure complexe sur l'espace compact X. Soient $\varepsilon$ un nombre $> 0$, K un ensemble compact satisfaisant à (M); la fonction $\varphi_{CK}$ étant semi-continue inférieurement et positive dans X, la formule (2) nous donne les relations suivantes, où $\mathcal{G}$ désigne l'ensemble des fonctions $g \in C^b(X, \mathbf{C})$ telles que $|g| \leq \varphi_{CK}$:

$$
|\nu|^*(X - K) = \sup_{g \in \mathcal{G}} |\nu(g)| = \sup_{g \in \mathcal{G}} |I(g_T)| \leq \varepsilon.
$$

Soit $(K_n)_{n \geq 1}$ une suite de parties compactes de T, telle que chaque $K_n$ satisfasse à (M) pour $\varepsilon = 1/n$, et soit $S = \bigcup_n K_n$; S est borélien dans X, contenu dans T, et on a $|\nu|^*(X - T) \leq |\nu|^*(X - S) \leq |\nu|^*(X - K_n) \leq 1/n$ pour tout n, de sorte que T est $\nu$-mesurable et que $\nu$ est concentrée sur T. Soit $f$ une fonction continue et bornée sur T; comme X est le compactifié de Stone–Čech de T, f se prolonge par continuité en une fonction g ∈ C^b(X; \mathbf{C}). Soit alors μ la mesure induite par ν sur T; on a $\mu(f) = \nu(f^0)^{(1)}$. Comme ν est concentrée sur T, les fonctions $f^0$ et g sont égales ν-presque partout, et on a donc $\mu(f) = \nu(g) = \mathrm{I}(g_T) = \mathrm{I}(f)$, ce qui achève la démonstration.

#### Corollaire {#int-ix-s5-n2-cor-1 .statement}

Avec les notations de la prop. 5, supposons qu’il existe une mesure positive bornée μ sur T telle que $|\mathrm{I}(f)| \leq \mu(|f|)$ pour tout $f \in C^b(T; \mathbf{C})$; alors il existe une mesure complexe θ sur T telle que $\theta(f) = \mathrm{I}(f)$ pour tout $f \in C^b(T; \mathbf{C})$.

### 3. Convergence étroite des mesures bornées

Soit T un espace complètement régulier; la forme bilinéaire $(f, \mu) \mapsto \int f(t) d\mu(t)$ sur $C^b(T) \times M^b(T)$ met ces deux espaces en dualité séparante. Il est clair en effet que la dualité est séparante en $C^b(T)$ du fait que les mesures $\varepsilon_x$ ($x \in T$) appartiennent à $M^b(T)$; elle est séparante en $M^b(T)$ d’après la prop. 2 du n° 1.

#### Définition 1 {#int-ix-s5-def-1 .statement}

La topologie faible sur $M^b(T)$ associée à la dualité précédente entre $C^b(T)$ et $M^b(T)$ est appelée la topologie de la convergence étroite (ou la topologie étroite) sur $M^b(T)$.

La topologie étroite est séparée, d’après les remarques précédant la définition. Nous emploierons souvent l’adverbe « étroitement » pour signifier « au sens de la topologie étroite ». Sauf mention du contraire, $M^b(T)$ sera muni de la topologie étroite dans toute la suite de ce paragraphe.

Tout élément de $C^b(T)$ est combinaison linéaire d’éléments de $C^b_+(T)$. Pour qu’un filtre $\mathfrak{F}$ sur $M^b(T)$ converge étroitement vers une mesure bornée λ, il faut et il suffit qu’on ait

$$
\lim_{\mu} \mu(f) = \lambda(f) \quad \text{suivant } \mathfrak{F} \text{ pour toute } f \in C^b_+(T).
$$

#### Remarque 1 {#int-ix-s5-n3-rem-1 .statement}

Si T est localement compact, la topologie étroite est plus fine que la topologie induite sur $M^b(T)$ par la topologie vague, et ces deux topologies ne coïncident que si T est compact. En effet, si T n’est pas compact, l’application $t \mapsto \varepsilon_t$ converge vaguement vers 0 suivant le filtre des complémentaires des parties relativement compactes de T, mais ne converge pas étroitement vers 0, car la fonction 1 appartient à $C^b(T)$ (pour les relations entre convergence vague et convergence étroite, voir la prop. 9).

#### Remarque 2 {#int-ix-s5-n3-rem-2 .statement}

Il résulte aussitôt de la prop. 4 que $M^b_+(T)$ est fermé dans $M^b(T)$.

#### Remarque 3 {#int-ix-s5-n3-rem-3 .statement}

Si T est complètement régulier, l’application $t \mapsto \varepsilon_t$ de T dans $M^b(T)$ est un homéomorphisme (Top. gén., chap. IX, 3e éd., § 1, n° 5).

#### Proposition 6 {#int-ix-s5-prop-6 .statement}

Soit T un espace complètement régulier.
a) Soit f une fonction numérique $\geq 0$ semi-continue inférieurement définie dans T; la fonction $\mu \mapsto |\mu|^*(f)$ est alors semi-continue inférieurement dans $M^b(T)$.

(1) Cette relation n’a été établie plus haut (§ 2, n° 1, prop. 1) que dans le cas où f et ν sont positives. L’extension à la situation présente, où f et ν sont complexes et bornées, est immédiate par linéarité.

b) Soit $f$ une fonction semi-continue supérieurement et bornée définie dans $T$; la fonction $\mu \mapsto \mu(f)$ est alors semi-continue supérieurement dans $\mathcal{M}_+^b(T)$.

On voit en effet, d’après la prop. 1, b) du n° 1, que $\mu \mapsto |\mu|^*(f)$ est l’enveloppe supérieure d’une famille de fonctions de la forme $\mu \mapsto |\mu(g)|$ avec $g \in \mathcal{C}^b(T)$, donc continues pour la topologie étroite. Ceci établit a). Pour prouver b), il suffit de choisir une constante $C$ majorant $f$, et d’écrire $\mu(f) = \mu(C) - \mu(C - f)$; la fonction $\mu \mapsto \mu(C)$ est continue, et la fonction $\mu \mapsto \mu(C - f)$ est semi-continue inférieurement dans $\mathcal{M}_+^b(T)$ d’après ce qui précède.

#### Proposition 7 {#int-ix-s5-prop-7 .statement}

Soit $T$ un espace complètement régulier. Soit $\mu$ une mesure positive bornée sur $T$, et soit $f$ une fonction positive bornée sur $T$, telle que l’ensemble des points de $T$ où $f$ n’est pas continue soit localement $\mu$-négligeable. L’application $\lambda \mapsto \lambda^*(f)$ de $\mathcal{M}_+^b(T)$ dans $\mathbf{R}$ est alors continue au point $\mu$.

Pour tout $t \in T$, posons $f'(t) = \liminf_{s \to t} f(s), f''(t) = \limsup_{s \to t} f(s)$. On a évidemment $f' \leq f \leq f''$, avec l’égalité en tout point de $T$ où $f$ est continue (donc $\mu$-presque partout). D’autre part, $f'$ est semi-continue inférieurement, $f''$ est semi-continue supérieurement et bornée ($Top.$ gén., chap. IV, 3e éd., § 6, n° 2, prop. 4). On a donc les relations suivantes d’après la prop. 6,

$$
\mu^*(f') \leq \liminf_{\lambda \to \mu} \lambda^*(f') \leq \liminf_{\lambda \to \mu} \lambda^*(f) \leq \mu^*(f) \leq \limsup_{\lambda \to \mu} \lambda^*(f)
$$
$$
\leq \limsup_{\lambda \to \mu} \lambda^*(f'') \leq \mu^*(f'').
$$

On conclut en remarquant que $\mu^*(f') = \mu^*(f'')$, car $f'$ et $f''$ sont égales localement $\mu$-presque partout.

#### Proposition 8 {#int-ix-s5-prop-8 .statement}

Soient $X$ un espace complètement régulier, $T$ un sous-espace de $X$, i l’injection canonique de $T$ dans $X$. Désignons par $W$ l’ensemble des mesures positives bornées sur $X$ concentrées sur $T$, muni de la topologie induite par $\mathcal{M}^b(X)$. L’application $\mu \mapsto i(\mu)$ de $\mathcal{M}_+^b(T)$ dans $\mathcal{M}^b(X)$ est alors un homéomorphisme de $\mathcal{M}_+^b(T)$ sur $W$.

Notons encore $i$ l’application $\mu \mapsto i(\mu)$ de $\mathcal{M}_+^b(T)$ dans $\mathcal{M}_+^b(X)$; $i$ est injective (§ 2, n° 4, prop. 8), et applique $\mathcal{M}_+^b(T)$ dans $W$ (§ 2, n° 3, prop. 7). Si $\lambda \in W$, on a $\lambda = i(\lambda_T)$ (§ 2, n° 3, prop. 7, b)). Par conséquent, $i$ est une bijection de $\mathcal{M}_+^b(T)$ sur $W$, et la bijection réciproque de $i$ est l’application $r : \lambda \mapsto \lambda_T$ sur $W$. D’autre part, $i$ est continue: en effet, si $f \in \mathcal{C}^b(X)$, on a $\langle i(\mu), f \rangle = \langle \mu, f \circ i \rangle$, et $f \circ i$ appartient à $\mathcal{C}^b(T)$. Tout revient donc à montrer que l’on a, pour toute mesure $\mu \in W$ et toute fonction $f \in \mathcal{C}_+^b(T)$,

$$
\lim_{\substack{\lambda \to \mu \\ \lambda \in W}} \lambda_T(f) = \mu_T(f),
$$

ou encore

$$
\lim_{\substack{\lambda \to \mu \\ \lambda \in W}} \lambda(f^0) = \mu(f^0).
$$

Soit $f^\infty$ la fonction sur $X$ qui coïncide avec $f$ dans $T$, avec $+\infty$ dans $X - T$, et soient $f'$ et $f''$ respectivement la régularisée semi-continue supérieurement de $f^0$, et la régularisée semi-continue inférieurement de $f^\infty$ (*Top. gén.*, chap. IV, 3e éd., § 6, n° 2). Les relations $f'(x) = \limsup_{y \to x} f^0(y), f''(x) = \liminf_{y \to x} f^\infty(y)$ entraînent aussitôt que $f'$ et $f''$ coïncident toutes deux avec $f$ et $f^0$ dans $T$. La prop. 6 donne alors
$$
\mu^*(f') \geq \limsup_{\substack{\lambda \to \mu \\ \lambda \in W}} \lambda^*(f')
$$
$$
\mu^*(f'') \leq \liminf_{\substack{\lambda \to \mu \\ \lambda \in W}} \lambda^*(f'').
$$
Mais on peut remplacer $f'$ et $f''$ par $f^0$ dans ces deux formules, puisque les mesures $\lambda$ et $\mu$ sont portées par $T$; on a donc obtenu la relation cherchée.

L'énoncé de la prop. 8 ne vaut que pour des mesures *positives*: l’application $\mu \mapsto i(\mu)$ de $\mathcal{M}^b(T)$ dans $\mathcal{M}^b(X)$ est injective et continue, mais n’est en général pas un homéomorphisme de $\mathcal{M}^b(T)$ sur son image. Prenons par exemple $X = \mathbf{R}, T = \mathbf{R} - \{0\}$; les mesures $\lambda_t = \varepsilon_t - \varepsilon_{-t}$ ($t > 0$) convergent étroitement vers 0 dans $X$ lorsque $t$ tend vers 0, mais ne convergent pas étroitement vers 0 dans $T$ (la fonction caractéristique de ]0, $+\infty[$ appartient à $\mathcal{C}^b(T)$) (cf. cependant le cor. du th. 1 du n° 5).

#### Proposition 9 {#int-ix-s5-prop-9 .statement}

*Soit T un espace localement compact, et soit $\mathfrak{F}$ un filtre sur $\mathcal{M}^b_+(T)$ qui converge vaguement vers une mesure bornée $\mu$. Pour que $\mathfrak{F}$ converge étroitement vers $\mu$, il faut et il suffit que l’on ait $\lim_{\lambda} \lambda(1) = \mu(1)$ suivant $\mathfrak{F}$.*

La condition est évidemment nécessaire. Pour montrer qu’elle est suffisante, désignons par $X$ le compactifié d’Alexandroff de $T$ (*Top. gén.*, chap. I, 4e éd., § 9, n° 8) et par $i$ l’injection canonique de $T$ dans $X$. D’après la prop. 8, tout revient à montrer que $\lambda \mapsto i(\lambda)$ converge étroitement vers $i(\mu)$ dans $\mathcal{M}^b(X)$ suivant $\mathfrak{F}$. Comme $\mu(1) < +\infty$, il existe un ensemble $A \in \mathfrak{F}$ tel que les masses totales des mesures de $A$ soient bornées par un nombre $M$; il nous suffit donc de vérifier que l’on a
$$
\lim_{\lambda, \mathfrak{F}} \int_X g \, d(i(\lambda)) = \int_X g \, d(i(\mu))
$$
pour des fonctions $g \in \mathcal{C}^b(X)$ qui forment un ensemble total dans $\mathcal{C}^b(X)$. Or cette égalité est satisfaite lorsque $g$ a un support compact dans $T$, en raison de la convergence vague de $\mathfrak{F}$ vers $\mu$, et d’autre part lorsque $g$ est une fonction constante sur $X$, du fait que $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. Les fonctions des deux types précédents formant un ensemble total dans $\mathcal{C}^b(X)$ (chap. III, 2e éd., § 1, n° 2, prop. 3), cela termine la démonstration.

### 4. Application: propriétés topologiques de l’espace $\mathcal{M}^b_+(T)$

Remarquons d’abord que, si $T$ est complètement régulier, $\mathcal{M}^b(T)$ est un espace vectoriel topologique séparé, donc complètement régulier. Par suite, $\mathcal{M}_+^b(T)$ est complètement régulier.

#### Proposition 10 {#int-ix-s5-prop-10 .statement}

*Soit T un espace polonais; l’espace $\mathcal{M}_+^b(T)$ est alors polonais pour la topologie étroite.*

Nous commencerons par traiter le cas où T est polonais et *compact*. L’ensemble U des mesures positives de masse $\leq 1$ est alors compact (chap. III, 2e éd., § 1, n° 9, cor. 2 de la prop. 15), et la topologie induite sur U par la topologie étroite (qui coïncide ici avec la topologie vague) est aussi induite par la topologie de la convergence simple dans un ensemble total de $\mathcal{C}(T)$ (*loc. cit.*, n° 10, prop. 17). Or, il existe dans $\mathcal{C}(T)$ un ensemble total dénombrable (*Top. gén.*, chap. X, 2e éd., § 3, n° 3, th. 1); par suite, U est un espace compact métrisable. L’ensemble V des mesures positives de masse $< 1$ est ouvert dans U, donc est un espace localement compact polonais. Or l’application $\mu \mapsto \frac{1}{1 + \mu(1)} \mu$ de $\mathcal{M}_+^b(T)$ sur V est un homéomorphisme, l’application $\lambda \mapsto \frac{1}{1 - \lambda(1)} \lambda$ étant l’homéomorphisme réciproque.

Passons au cas où T est polonais; on peut supposer que T est l’intersection d’une suite décroissante $(G_n)$ d’ouverts dans un espace compact métrisable X (*Top. gén.*, chap. IX, 3e éd., § 6, n° 1, cor. 1 du th. 1); l’espace $\mathcal{M}_+^b(T)$ est alors homéomorphe au sous-espace W de $\mathcal{M}_+^b(X)$ constitué par les mesures concentrées sur T (n° 3, prop. 8), et il nous suffit de montrer que W est l’intersection d’une suite d’ouverts dans l’espace polonais $\mathcal{M}_+^b(X)$ (*loc. cit.*, cor. 1 du th. 1). Or, soit $W_n$ l’ensemble des mesures $\mu \in \mathcal{M}_+^b(X)$ concentrées sur $G_n$; l’application $h_n : \mu \mapsto \mu^*(X - G_n)$ sur $\mathcal{M}_+^b(X)$ est semi-continue supérieurement (n° 3, prop. 6), et l’ensemble $A_k^n$ des mesures $\mu \in \mathcal{M}_+^b(X)$ telles que $h_n(\mu) < 1/k$ est donc ouvert pour tout $k \geq 1$ et tout $n \in \mathbf{N}$. On achève alors la démonstration en remarquant que $W = \bigcap_n W_n = \bigcap_{n, k} A_k^n$.

#### Corollaire 1 {#int-ix-s5-prop-10-cor-1 .statement}

*Si T est un espace métrisable de type dénombrable, $\mathcal{M}_+^b(T)$ est métrisable de type dénombrable pour la topologie étroite.*

En effet, soit $\hat{T}$ le complété de T pour une métrique définissant la topologie de T; l’espace $\hat{T}$ est polonais, et $\mathcal{M}_+^b(\hat{T})$ est homéomorphe au sous-espace de l’espace polonais $\mathcal{M}_+^b(\hat{T})$, constitué par les mesures concentrées sur T (n° 3, prop. 8). Or tout sous-espace d’un espace polonais est métrisable de type dénombrable (*Top. gén.*, chap. IX, 3e éd., § 2, n° 8, cor. de la prop. 11).

#### Corollaire 2 {#int-ix-s5-prop-10-cor-2 .statement}

*Si T est un espace souslinien (resp. lusinien) complètement régulier, l’espace $\mathcal{M}_+^b(T)$ est souslinien (resp. lusinien).*

Considérons en effet un espace polonais P et une application continue $f$ de P sur T (Top. gén., chap. IX, 3e éd., § 6, n° 2, déf. 2). Soit $\tilde{f}$ l’application continue $\mu \mapsto f(\mu)$ de $\mathcal{M}_+^b(P)$ dans $\mathcal{M}_+^b(T)$; l’espace $\mathcal{M}_+^b(P)$ est polonais d’après la prop. 10, et $\tilde{f}$ est surjective ($§ 2,$ n° 4, prop. 9); l’espace $\mathcal{M}_+^b(T)$ est donc sous-linien. De même, si T est lusinien, $f$ peut être supposée injective (*loc. cit.*, n° 4, prop. 11); alors $\tilde{f}$ est injective ($§ 2,$ n° 4, prop. 8), et $\mathcal{M}_+^b(T)$ est donc lusinien (*loc. cit.*, n° 4, prop. 11).

Soit T un espace souslinien complètement régulier (rappelons qu’il suffit pour cela que T soit souslinien et *régulier* (*loc. cit.*, Appendice, cor. de la prop. 2)), et soit H une partie compacte de $\mathcal{M}_+^b(T)$; alors H est compacte et souslinienne, donc *métrisable* pour la topologie étroite (*loc. cit.*, Appendice, cor. 2 de la prop. 3).

### 5. Critère de compacité pour la convergence étroite

#### Définition 2 {#int-ix-s5-def-2 .statement}

*Soit T un espace topologique, et soit H une partie de $\mathcal{M}^b(T)$; on dit que H satisfait à la condition de Prokhorov si*
a) *on a* $\sup_{\mu \in H} |\mu|(1) < +\infty;$
b) *pour tout nombre* $\varepsilon > 0$, *il existe un ensemble compact* $K_\varepsilon$ *de T tel que l’on ait*
$$
|\mu|(T - K_\varepsilon) \leq \varepsilon \quad \text{pour tout mesure } \mu \in H.
$$
(6)

On peut montrer que, si T est complètement régulier, l’ensemble des conditions a) et b) est équivalent à la condition suivante: il existe une fonction réelle $f \geq 1$ sur T, telle que l’ensemble des points t de T satisfaisant à $f(t) \leq c$ soit compact pour tout $c \in \mathbf{R}_+$ (ce qui entraîne en particulier que $f$ est semi-continue inférieurement), et telle que l’on ait $\sup_{\mu \in H} |\mu|(f) < +\infty$. De plus, lorsque T est localement compact, on obtient un énoncé équivalent en imposant à $f$ d’être continue (cf. exerc. 10).

#### Proposition 11 {#int-ix-s5-prop-11 .statement}

*Soit T un espace complètement régulier, et soit H une partie de $\mathcal{M}^b(T)$ qui satisfait à la condition de Prokhorov; son adhérence $\overline{H}$ dans $\mathcal{M}^b(T)$ satisfait alors à la condition de Prokhorov.*

En effet, les fonctions $\mu \mapsto |\mu|^\bullet(1), \mu \mapsto |\mu|^\bullet(T - K_\varepsilon)$ sont semi-continues inférieurement dans $\mathcal{M}^b(T)$ d’après la prop. 6 du n° 3.

L’intérêt de la condition de Prokhorov vient du théorème suivant, dont on étudiera la réciproque plus loin (th. 2).

#### Théorème 1 (Prokhorov) {#int-ix-s5-thm-1 .statement}

*Soit T un espace complètement régulier, et soit H une partie de $\mathcal{M}^b(T)$ qui satisfait à la condition de Prokhorov; H est alors relativement compacte dans $\mathcal{M}^b(T)$ pour la topologie étroite.*

Nous pouvons supposer que T est un sous-espace d’un espace compact X; soit i l’injection canonique de T dans X. Nous pouvons supposer d’autre part que H est *fermée* dans $\mathcal{M}^b(T)$, d’après la prop. 11. Il nous suffit alors de montrer que tout ultrafiltre $\mathcal{U}$ sur H converge dans $\mathcal{M}^b(T)$.

Nous commencerons par le cas où $H \subset \mathcal{M}_+^b(T)$. Les masses totales des mesures μ ∈ H étant bornées par hypothèse, i(μ) converge vaguement suivant U, dans $\mathcal{M}_+(X)$, vers une mesure $v \in \mathcal{M}_+(X)$ (chap. III, 2e éd., § 1, n° 9, cor. 2 de la prop. 15); d’après la prop. 8 du n° 3, tout revient à prouver que v est concentrée sur T. Or, soit ε un nombre > 0, et soit $K_\varepsilon$ une partie compacte de T satisfaisant à la formule (6). Comme $X - K_\varepsilon$ est ouvert dans X, on a d’après la prop. 6 du n° 3 appliquée dans X les inégalités
$$
v^*(X - T) \leq v^*(X - K_\varepsilon) \leq \liminf_{\mu, U} i(\mu)^*(X - K_\varepsilon) = \liminf_{\mu, U} \mu^*(T - K_\varepsilon) \leq \varepsilon;
$$
comme $\varepsilon > 0$ est arbitraire, le théorème est établi dans le cas particulier considéré.

Passons au cas général; pour toute mesure $\mu$ sur T, posons $a_1(\mu) = \Re(\mu)^+$, $a_2(\mu) = \Re(\mu)^-$, $a_3(\mu) = \Im(\mu)^+$, $a_4(\mu) = \Im(\mu)^-$; comme on a $\mu = a_1(\mu) - a_2(\mu) + ia_3(\mu) - ia_4(\mu)$, il suffit de montrer que les applications $a_j$ ($j = 1, 2, 3, 4$) convergent étroitement suivant U. Mais l’ensemble $H_j$ des mesures $a_j(\mu)$, où $\mu$ parcourt H, satisfait à la condition de Prokhorov en vertu de la relation $|a_j(\mu)| \leq |\mu|$, et il est contenu dans $\mathcal{M}_+^b(T)$; il est donc relativement compact dans $\mathcal{M}_+^b(T)$ d’après le cas particulier, et le théorème en résulte aussitôt.

#### Corollaire {#int-ix-s5-n5-cor-1 .statement}

*Soit T un sous-espace d’un espace complètement régulier X, et soit H une partie de $\mathcal{M}_+^b(T)$, qui satisfait à la condition de Prokhorov. Si i désigne l’injection canonique de T dans X, la restriction à H de l’application $\mu \mapsto i(\mu)$ de $\mathcal{M}_+^b(T)$ dans $\mathcal{M}_+^b(X)$ est un homéomorphisme de H sur son image.*

Il suffit de traiter le cas où H est fermée (prop. 11), donc compacte; cela résulte alors du fait que $\mu \mapsto i(\mu)$ est continue et injective.

Rappelons que ce résultat vaut aussi pour une partie quelconque de $\mathcal{M}_+^b(T)$ (n° 3, prop. 8).

#### Théorème 2 {#int-ix-s5-thm-2 .statement}

*Soit T un espace localement compact, ou un espace polonais, et soit H une partie relativement compacte de $\mathcal{M}_+^b(T)$; H satisfait alors à la condition de Prokhorov.*

On peut se borner au cas où H est fermé, donc compact. Les masses totales des mesures $\mu \in H$ sont évidemment bornées, car l’application $\mu \mapsto \mu(1)$ est continue, et tout revient à prouver l’assertion b) de la déf. 2.

Supposons d’abord que T soit localement compact. Soit ε un nombre > 0. Associons à toute mesure $\mu \in H$ un ensemble compact $K_\mu$ dans T tel que $\mu^*(T - K_\mu) < \varepsilon$, puis un voisinage ouvert relativement compact $U_\mu$ de $K_\mu$. La fonction $\lambda \mapsto \lambda^*(T - U_\mu)$ étant semi-continue supérieurement dans $\mathcal{M}_+^b(T)$ (n° 3, prop. 6), l’ensemble $V^\mu$ des mesures $\lambda \in H$ telles que $\lambda^*(T - U_\mu) < \varepsilon$ est un voisinage de $\mu$ dans H. Il existe donc une partie finie $H'$ de H telle que les ensembles $V^\mu$ ($\mu \in H'$) recouvrent H. Si l’on désigne alors par K l’ensemble compact $\bigcup_{\mu \in H'} \overline{U}_\mu$, on a $\lambda^*(T - K) < \varepsilon$ pour tout $\lambda \in H$.

Supposons ensuite que T soit polonais. Nous ne restreindrons pas la généralité en supposant que T est l’intersection d’une suite décroissante $(T_p)_{p \geq 1}$ d’ensembles ouverts d’un espace compact X (*Top. gén.*, chap. IX, 3e éd., § 6, n° 1, cor. du th. 1). Soit $i_p$ l’injection de $T$ dans $T_p$, et soit $H_p$ l’ensemble des mesures de la forme $i_p(\lambda)$ pour $\lambda \in H$; comme $H_p$ est compact dans $\mathcal{M}_+^b(T_p)$, il existe donc un ensemble compact $K_p \subset T_p$ tel qu’on ait $\nu^*(T_p - K_p) \leq \varepsilon 2^{-p}$ pour toute mesure $\nu \in H_p$, d’après le résultat précédent appliqué à l’espace localement compact $T_p$. On a donc aussi $\nu^*(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$, et finalement $\lambda^*(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$ pour toute mesure $\lambda \in H$. Posons alors $K = \bigcap_p K_p$; l’ensemble $K$ est compact et contenu dans $T$, et on a, pour toute mesure $\lambda \in H$,
$$
\lambda^*(T - K) \leq \sum_p \lambda^*(T - (T \cap K_p)) \leq \sum_p \varepsilon 2^{-p} = \varepsilon.
$$
La condition de Prokhorov est donc vérifiée.

### 6. Convergence étroite des mesures et convergence compacte des fonctions

#### Proposition 12 {#int-ix-s5-prop-12 .statement}

Soit $T$ un espace complètement régulier, et soit $B$ la boule unité de l’espace normé $\mathcal{C}^b(T, \mathbf{C})$. Soit $I$ une forme linéaire sur $\mathcal{C}^b(T, \mathbf{C})$. Pour qu’il existe une mesure complexe bornée $\theta$ sur $T$ telle que $I(f) = \theta(f)$ pour tout $f \in \mathcal{C}^b(T, \mathbf{C})$, il faut et il suffit que la restriction de $I$ à $B$ soit continue pour la topologie de la convergence compacte. La mesure $\theta$ est alors unique.

Montrons que la condition de l’énoncé est nécessaire. Soient $\theta$ une mesure complexe bornée sur $T$, $\varepsilon$ un nombre $> 0$, et $K$ une partie compacte de $T$ telle que $|\theta|^*(T - K) < \varepsilon$. Soit $f \in B$; nous noterons $U$ le voisinage de $f$ dans $B$ pour la topologie de la convergence compacte, formé des fonctions $g \in B$ telles que $\sup_{x \in K} |g(x) - f(x)| \leq \varepsilon$. On a, pour tout $g \in U$
$$
|\theta(g) - \theta(f)| \leq \int_T |g - f| \, d|\theta| \leq \varepsilon |\theta|^*(K) + 2|\theta|^*(T - K) \leq (\|\theta\| + 2)\varepsilon,
$$
car $|g - f|$ est majorée par $\varepsilon$ sur $K$ et par $2$ sur $T - K$.

Réciproquement, considérons une forme linéaire $I$ sur $\mathcal{C}^b(T, \mathbf{C})$, dont la restriction à $B$ soit continue pour la topologie de la convergence compacte. Pour tout nombre $\varepsilon > 0$, il existe alors un nombre $a > 0$ et une partie compacte $K$ de $T$ tels que les relations $f \in B, \sup_{x \in K} |f(x)| \leq a$ entraînent $|I(f)| \leq \varepsilon$. La prop. 5 du n° 2 entraîne alors l’existence d’une mesure complexe bornée $\theta$, unique, telle que $I(f) = \theta(f)$ pour tout $f \in \mathcal{C}^b(T, \mathbf{C})$.

#### Proposition 13 {#int-ix-s5-prop-13 .statement}

Soient $T$ un espace localement compact, et $H$ une partie bornée de l’espace normé $\mathcal{C}^b(T, \mathbf{C})$. L’application $(\mu, f) \mapsto \mu(f)$ de $\mathcal{M}_+^b(T) \times H$ dans $\mathbf{C}$ est alors continue lorsqu’on munit $\mathcal{M}_+^b(T)$ de la topologie étroite, et $H$ de la topologie de la convergence compacte.

Soient $\mu \in \mathcal{M}_+^b(T), f \in H$, et $M$ un nombre réel tel que l’on ait $\|\mu\| < M$, et $|g| \leq M$ pour tout $g \in H$. Désignons par $\varepsilon$ un nombre $> 0$, et choisissons une partie compacte $K$ de $T$ telle que $\mu^*(T - K) < \varepsilon$ et un voisinage ouvert relativement compact S de K. L’ensemble U des mesures $\lambda \in \mathcal{M}_+^b(T)$ satisfaisant aux inégalités
$$
\lambda^*(T) < M, \quad \lambda^*(T - S) < \varepsilon, \quad |\lambda(f) - \mu(f)| < \varepsilon,
$$
est alors un voisinage de $\mu$ dans $\mathcal{M}_+^b(T)$ (n° 3, prop. 6). Par ailleurs, soit V le voisinage de $f$ dans H constitué par les fonctions $g \in H$ telles que
$$
\sup_{x \in S} |g(x) - f(x)| < \varepsilon.
$$
Soient $\lambda \in U$ et $g \in V$; la fonction $|g - f|$ étant majorée par $\varepsilon$ dans S, par $2M$ dans $T - S$, on a
$$
|\lambda(g) - \lambda(f)| \leq \int_T |g - f| \, d\lambda \leq \varepsilon \lambda^*(S) + 2M \lambda^*(T - S) \leq 3M \varepsilon,
$$
et on en déduit
$$
|\lambda(g) - \mu(f)| \leq |\lambda(g) - \lambda(f)| + |\lambda(f) - \mu(f)| \leq (3M + 1)\varepsilon.
$$
Ceci prouve la continuité de l’application $(\lambda, g) \mapsto \lambda(g)$ au point $(\mu, f)$ de $\mathcal{M}_+^b(T) \times H$.

#### Remarque {#int-ix-s5-n6-rem-1 .statement}

Soient T un espace complètement régulier, M une partie de $\mathcal{M}^b(T)$ qui satisfait à la condition de Prokhorov, H une partie bornée de $C^b(T)$. Un raisonnement très voisin de celui qui vient d’être fait permet de prouver que l’application $(\lambda, g) \mapsto \lambda(g)$ de $M \times H$ dans $\mathbf{C}$ est continue lorsqu’on munit M de la topologie étroite et H de la topologie de la convergence compacte.

#### Corollaire {#int-ix-s5-n6-cor-1 .statement}

Soient T un espace complètement régulier, X un espace topologique, f une fonction à valeurs complexes définie dans $T \times X$, continue et bornée. Pour toute mesure bornée $\mu$ sur T, soit $F_\mu$ la fonction sur X définie par $F_\mu(x) = \int_T f(t, x) \, d\mu(t)$ pour tout $x \in X$.
a) La fonction $F_\mu$ est continue et bornée pour toute mesure bornée $\mu$.
b) Supposons T localement compact. L’application $\mu \mapsto F_\mu$ de $\mathcal{M}_+^b(T)$ dans $C^b(X, \mathbf{C})$ est alors continue, si l’on munit $\mathcal{M}_+^b(T)$ de la topologie étroite, et $C^b(X, \mathbf{C})$ de la topologie de la convergence compacte.
Pour tout $x \in X$, notons $f_x$ la fonction continue et bornée $t \mapsto f(t, x)$ sur T; l’application $x \mapsto f_x$ de X dans $C^b(T, \mathbf{C})$ a une image bornée, et elle est continue si l’on munit $C^b(T, \mathbf{C})$ de la topologie de la convergence compacte (Top. gén., chap. X, 2e éd., § 3, n° 4, th. 3). Comme on a $F_\mu(x) = \mu(f_x)$, la fonction $F_\mu$ est continue d’après la prop. 12. Supposons T localement compact; la prop. 13 montre que l’application $(\mu, x) \mapsto F_\mu(x)$ de $\mathcal{M}_+^b(T) \times X$ dans $\mathbf{C}$ est continue; l’assertion b) résulte de là (loc. cit.).

### 7. Application: transformation de Laplace

Dans ce n°, on note M un monoïde commutatif, dont la loi de composition est notée additivement, muni d’une topologie d’espace localement compact pour laquelle l’application $(m, m') \mapsto m + m'$ de $M \times M$ dans $M$ est continue. On note 0 l’élément neutre de $M$. On appelle caractère de $M$ toute fonction continue complexe bornée $\chi$ dans $M$ satisfaisant aux relations

$$(7)$$
$$
\chi(m + m') = \chi(m) \cdot \chi(m'), \quad \chi(0) = 1, \quad |\chi(m)| \leq 1
$$

pour $m, m'$ dans $M$. Si $\chi$ et $\chi'$ sont deux caractères, il en est de même de $\chi \chi'$. L’ensemble des caractères de $M$ est un monoïde noté $X$; on le munira de la topologie de la convergence compacte, pour laquelle l’application $(\chi, \chi') \mapsto \chi \chi'$ de $X \times X$ dans $X$ est continue. L’élément neutre de $X$ est la fonction constante 1.

Pour toute mesure complexe bornée $\mu$ sur $M$, on appelle transformée de Laplace de $\mu$ la fonction $\mathcal{L}\mu$ sur $X$ définie par

$$(8)$$
$$
(\mathcal{L}\mu)(\chi) = \int_M \chi(m) \, d\mu(m).
$$

D’après le th. 3 de Top. gén., 2e éd., chap. X, § 3, n° 4, l’application $(m, \chi) \mapsto \chi(m)$ de $M \times X$ dans $\mathbf{C}$ est continue et bornée. Le corollaire de la prop. 13 du n° 6 entraîne alors le résultat suivant:

#### Proposition 14 {#int-ix-s5-prop-14 .statement}

*Pour toute mesure complexe bornée $\mu$ sur $M$, la fonction $\mathcal{L}\mu$ sur $X$ est continue et bornée. Si l’on munit $\mathcal{M}_+^b(M)$ de la topologie étroite et $\mathcal{C}^b(X; \mathbf{C})$ de la topologie de la convergence compacte, l’application $\mu \mapsto \mathcal{L}\mu$ de $\mathcal{M}_+^b(M)$ dans $\mathcal{C}^b(X; \mathbf{C})$ est continue.*

L’ensemble des caractères de $M$ qui tendent vers 0 à l’infini sera noté $X_0$; cet ensemble est stable par multiplication. Nous dirons qu’un sous-monoïde $S$ de $X$ est *plein* si $S$ est stable pour l’application $\chi \mapsto \overline{\chi}$, si $S \cap X_0$ sépare les points de $M$ (*Top. gén.*, chap. X, 2e éd., § 4, n° 1, déf. 1) et si quel que soit $m \in M$, il existe un élément $\chi$ de $S \cap X_0$ tel que $\chi(m) \neq 0$.

Supposons de plus que $M$ soit un groupe commutatif non compact. Soit $f$ une fonction dans $M$ qui tend vers 0 à l’infini; il en est alors de même de la fonction $x \mapsto f(x)f(-x)$ dans $M$, alors que tout caractère $\chi$ de $M$ satisfait à $\chi(x)\chi(-x) = \chi(0) = 1$. Il en résulte que $X_0$ est vide, et que $X$ ne contient aucun sous-monoïde plein. Le théorème 3 ci-dessous ne s’applique donc pas aux groupes localement compacts, mais non compacts.

#### Théorème 3 {#int-ix-s5-thm-3 .statement}

*Soit $S$ un sous-monoïde plein de $X$.
a) Si $\mu$ et $\mu'$ sont deux mesures complexes bornées sur $M$, telles que $\mathcal{L}\mu$ et $\mathcal{L}\mu'$ aient même restriction à $S \cap X_0$, on a $\mu = \mu'$.
b) Soit $\mathfrak{F}$ un filtre sur $\mathcal{M}_+^b(M)$, tel que $\mathcal{L}\lambda(s)$ ait une limite $\Phi(s) \in \mathbf{C}$ suivant $\mathfrak{F}$ pour tout $s \in S$. Alors le filtre $\mathfrak{F}$ converge vaguement vers une mesure positive bornée $\mu$, et l’on a $\Phi(s) = \mathcal{L}\mu(s)$ pour tout $s \in S \cap X_0$.
c) Sous les hypothèses de b), supposons de plus que 1 soit adhérent à $S \cap X_0$, et que la*

(1) Rappelons qu’un sous-monoïde d’un monoïde $A$ contient par définition l’élément neutre de $A$ (Alg. chap. I, 4e édition, § 1).

fonction $\Phi$ sur $S$ soit continue au point 1. Alors $\mathfrak{F}$ converge étroitement vers $\mu$, et $\Phi(s) = \mathcal{L}\mu(s)$ pour tout $s \in S$.

Nous noterons $E$ l’algèbre des fonctions continues complexes tendant vers 0 à l’infini sur $M$ et $\mathfrak{A}$ le sous-espace de $E$ engendré par $S \cap X_0$; alors $\mathfrak{A}$ est une sous-algèbre de $E$ stable par l’application $f \mapsto \bar{f}$; comme $S$ est un sous-monoïde plein de $X$, le cor. 2 de la prop. 7 de Top. gén., chap. X, § 4, n° 4 entraîne que $\mathfrak{A}$ est dense dans $E$.

Démontrons a): on a par hypothèse $\mu(f) = \mu'(f)$ pour tout $f \in \mathfrak{A}$; comme $\mu$ et $\mu'$ sont des formes linéaires continues sur $E$, cela entraîne $\mu(f) = \mu'(f)$ pour $f \in E$, et en particulier pour toute fonction $f$ continue à support compact, d’où $\mu = \mu'$.

Plaçons-nous sous les hypothèses de b). Le nombre $\Phi(1) = \lim_{\lambda, \mathfrak{F}} \lambda(1)$ est réel positif; soit un nombre réel $a > \Phi(1)$; comme on a $\| \lambda \| = \mathcal{L}\lambda(1)$ pour $\lambda \in \mathcal{M}_+^b(M)$, la relation $\lim_{\lambda, \mathfrak{F}} \mathcal{L}\lambda(1) = \Phi(1)$ entraîne que l’ensemble $H$ des mesures $\lambda \in \mathcal{M}_+^b(M)$ telles que $\| \lambda \| \leq a$ appartient à $\mathfrak{F}$. Comme $\mathcal{M}_+^b(M, \mathbf{C})$ s’identifie au dual de l’espace normé $E$ (chap. III, 2e éd., § 1, n° 8 & § 1, n° 2, prop. 3), l’espace $H$ est compact pour la topologie $\sigma(\mathcal{M}_+^b(M, \mathbf{C}), E)$. D’autre part (Esp. vect. top., chap. III, § 3, n° 5, prop. 5), cette topologie coïncide sur $H$ avec la topologie de la convergence simple dans une partie totale quelconque de $E$. En particulier, comme $\mathfrak{A}$ est dense dans $E$, et qu’il en est de même de l’espace des fonctions continues à support compact (chap. III, 2e éd., § 1, n° 2, prop. 3), la topologie de la convergence simple dans $S \cap X_0$ coïncide sur $H$ avec la topologie vague, et $H$ est compact pour cette topologie. Il en résulte aussitôt que $\mathfrak{F}$ converge vaguement vers une mesure $\mu \in H$, et que $\mathcal{L}\mu(s) = \lim_{\lambda, \mathfrak{F}} \mathcal{L}\lambda(s)$ pour tout $s \in S \cap X_0$.

Passons enfin à c). Comme les fonctions $\Phi$ et $\mathcal{L}\mu$ sont continues au point $1 \in S$, égales dans $S \cap X_0$, et comme 1 est adhérent à $S \cap X_0$, on a $\Phi(1) = \mathcal{L}\mu(1)$. Autrement dit, on a $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. La prop. 9 du n° 3 montre alors que $\mu$ est limite étroite du filtre $\mathfrak{F}$. Tout élément de $S$ étant une fonction continue bornée sur $M$, cela entraîne $\Phi(s) = \lim_{\lambda, \mathfrak{F}} \lambda(s) = \mu(s) = \mathcal{L}\mu(s)$ pour tout $s \in S$.

#### Corollaire {#int-ix-s5-n7-cor-1 .statement}

Soit $S$ un sous-monoïde plein de $X$, tel que 1 soit adhérent à $S \cap X_0$. Soit $L$ le sous-ensemble de $C^b(S; \mathbf{C})$ constitué par les restrictions à $S$ des transformées de Laplace des mesures $\lambda \in \mathcal{M}_+^b(M)$.

a) L’ensemble $L$ est fermé dans l’espace $C^b(S; \mathbf{C})$ muni de la topologie de la convergence simple.

b) L’application $\lambda \mapsto (\mathcal{L}\lambda)_S$ est un homéomorphisme de $\mathcal{M}_+^b(M)$ sur $L$, si l’on munit $\mathcal{M}_+^b(M)$ de la topologie étroite et $L$ de la topologie de la convergence simple.

c) La topologie de la convergence simple et la topologie de la convergence compacte coïncident dans $L$.

Les assertions a) et b) sont des conséquences immédiates du th. 3 ; l’assertion c) résulte de b) et de la prop. 14, car la topologie de la convergence compacte est plus fine que celle de la convergence simple.

On prendra garde que $L$ n’est pas fermé dans l’ensemble de toutes les fonctions complexes bornées sur $S$, muni de la topologie de la convergence simple. Prenons par exemple les notations de l’Exemple 2 ci-dessous ($M = \mathbf{R}_+$, $S$ identifié à $\mathbf{R}_+$). Les transformées de Laplace des mesures $\varepsilon_n$ ($n \in \mathbf{N}$) sont les fonctions $t \mapsto e^{-nt}$ sur $\mathbf{R}_+$; lorsque $n$ tend vers $+\infty$, ces fonctions convergent simplement vers la fonction égale à 1 pour $t = 0$, à 0 pour $t \neq 0$, qui n’appartient pas à $L$.

*Exemple 1).* — Prenons pour $M$ l’ensemble $\mathbf{N}$ des entiers positifs, muni de la loi d’addition et de la topologie discrète. Soit $D$ le disque unité de $\mathbf{C}$ (ensemble des nombres complexes de module $\leq 1$) muni de la topologie induite par $\mathbf{C}$ et de la loi induite par la multiplication. Pour tout $z \in D$, notons $f(z)$ le caractère $n \mapsto z^n$ de $\mathbf{N}$. Pour tout caractère $\chi$ de $\mathbf{N}$, notons $g(\chi)$ le nombre complexe $\chi(1) \in D$. On vérifie aussitôt que $f$ et $g$ sont des homéomorphismes réciproques entre $D$ et $X$, et cela nous permettra, dans la suite, d’*identifier* $X$ et $D$. L’ensemble des caractères tendant vers 0 à l’infini s’identifie alors à l’ensemble $D_0$ des nombres complexes de valeur absolue < 1. Enfin, l’intervalle ]$0, 1$] de $\mathbf{R}$ est un sous monoïde plein de $D$ et 1 est adhérent à ]$0, 1$] $\cap D_0 = ]0, 1[$.

Toute mesure $\mu$ sur $\mathbf{N}$ s’écrit de manière unique sous la forme $\mu = \sum_{n \in \mathbf{N}} u_n \cdot \varepsilon_n$ et $\mu$ est bornée si et seulement si $\sum_n |u_n| < +\infty$; on a alors $\mathcal{L}\mu(z) = \sum_{n \in \mathbf{N}} u_n z^n$ pour $z \in D$. Cette fonction est continue sur $D$; il est d’usage de l’appeler la *fonction génératrice* de la suite sommable $(u_n)_{n \in \mathbf{N}}$. Transcrit dans ce langage, le th. 3 nous donne le résultat suivant (compte tenu de la prop. 9 du n° 3):

#### Proposition 15 {#int-ix-s5-prop-15 .statement}

*Soit $A$ un ensemble muni d’un filtre $\mathfrak{F}$. Pour tout $\alpha \in A$, soit $(u_{\alpha, n})_{n \in \mathbf{N}}$ une suite sommable de nombres positifs, et soit $\Phi_\alpha$ la fonction définie dans l’intervalle ]$0, 1$] de $\mathbf{R}$ par $\Phi_\alpha(x) = \sum_{n \in \mathbf{N}} u_{\alpha, n} x^n$. Pour qu’il existe une suite sommable $(u_n)_{n \in \mathbf{N}}$ de nombres positifs telle que l’on ait*

$$
\lim_{\alpha, \mathfrak{F}} u_{\alpha, n} = u_n \text{ pour tout } n, \quad \lim_{\alpha, \mathfrak{F}} \sum_{n \in \mathbf{N}} u_{\alpha, n} = \sum_{n \in \mathbf{N}} u_n,
$$

*il faut et il suffit que $\Phi_\alpha$ converge simplement dans ]$0, 1$], suivant $\mathfrak{F}$, vers une fonction $\Phi$ continue au point 1. On a dans ce cas $\Phi(x) = \sum_{n \in \mathbf{N}} u_n x^n$ pour tout $x \in ]0, 1[$.*

On a des résultats analogues en prenant pour $M$ le monoïde $\mathbf{N}^n$, où $n$ désigne un entier > 1; l’espace $X$ s’identifie alors à $D^n$, et l’on peut choisir ]$0, 1$^n comme sous-monoïde plein. Nous laisserons au lecteur le soin de transcrire le th. 3 dans ce cas.

*Exemple 2).* — Prenons pour $M$ l’ensemble $\mathbf{R}_+$, muni de la loi d’addition et de la topologie usuelle. Soit $P$ l’ensemble des nombres complexes $z$ de partie réelle positive, muni de la topologie induite par $\mathbf{C}$ et de la loi induite par l’addition dans $\mathbf{C}$. Pour tout $p \in P$, désignons alors par $f(p)$ le caractère $x \mapsto e^{-px}$ de $\mathbf{R}_+$; il est aisé de vérifier que $f$ est un isomorphisme de la structure de monoïde topologique de $P$ sur celle de $X$; nous identifierons $X$ à $P$ au moyen de $f$. Il est clair que $\mathbf{R}_+$ est un sous-monoïde plein de $P$, et le th. 3 nous donne le résultat suivant.

#### Proposition 16 {#int-ix-s5-prop-16 .statement}

*Soit $A$ un ensemble muni d’un filtre $\mathcal{F}$. Pour tout $\alpha \in A$, soit $\mu_\alpha$ une mesure positive bornée sur $\mathbf{R}_+$, et soit $\Phi_\alpha$ la fonction définie sur $\mathbf{R}_+$ par $\Phi_\alpha(p) = \int_0^{+\infty} e^{-px} d\mu_\alpha(x)$. Pour que l’application $\alpha \mapsto \mu_\alpha$ converge étroitement suivant $\mathcal{F}$ vers une mesure positive bornée $\mu$, il faut et il suffit que $\Phi_\alpha$ converge simplement dans $\mathbf{R}_+$, suivant $\mathcal{F}$, vers une fonction $\Phi$ continue au point 0. On a dans ce cas $\Phi(p) = \int_0^{+\infty} e^{-px} d\mu(x)$ pour tout $p \in \mathbf{R}_+$.*

On a des résultats analogues pour les monoïdes additifs $\mathbf{R}_+^n$ ($n$ entier $> 1$); nous laisserons au lecteur la transcription du th. 3 dans ce cas.

## EXERCICES {#int-ix-s5-exercises}

See the [exercises for § 5](exercises/s5/).
