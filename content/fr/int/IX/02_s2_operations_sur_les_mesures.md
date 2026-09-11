---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 2
section_title: Opérations sur les mesures
lang: fr
source: int-ix-fr
pdf_pages: 0024-0040, 0099-0100
extraction: ocr
subsections:
    - "no": 1
      title: Mesure induite sur un sous-espace mesurable
      page: 0
      pdf_page: 24
    - "no": 2
      title: Mesures définies par des densités numériques
      page: 0
      pdf_page: 25
    - "no": 3
      title: Image d’une mesure
      page: 0
      pdf_page: 27
    - "no": 4
      title: Relèvement de mesures
      page: 0
      pdf_page: 30
    - "no": 5
      title: Produit de deux mesures
      page: 0
      pdf_page: 32
    - "no": 6
      title: Intégration par rapport au produit de deux mesures
      page: 0
      pdf_page: 34
    - "no": 7
      title: Un résultat sur la désintégration des mesures
      page: 0
      pdf_page: 37
statements: 40
exercises: 3
content_sha256: 66020068ded1ac45c1a2eb80c727490afc00ca33f16b07ac3958bb16389ce06a
---

## § 2. Opérations sur les mesures

Comme dans le paragraphe précédent, $T$ désigne un espace topologique séparé, et $\mu$ une mesure sur $T$. On rappelle que toutes les mesures sont supposées positives, sauf mention du contraire.

### 1. Mesure induite sur un sous-espace mesurable

Soit $X$ une partie de $T$, et soit $\nu$ la restriction de l’application $\mu : K \mapsto \mu_K$ à l’ensemble des parties compactes de $X$; il est clair que $\nu$ est une prémesure sur $X$. D’autre part, soient $x \in X$ et $V$ un voisinage ouvert de $x$ dans $T$ tel que $\mu^*(V) < +\infty$; on a
$$
\nu^*(X \cap V) = \sup_{\substack{K \text{ compact} \\ K \subset X \cap V}} \mu^*(K) \leq \mu^*(V) < +\infty
$$
d’après la Remarque 3 du § 1, n° 2, de sorte que $\nu$ est une mesure.

Lorsque $X$ n’est pas $\mu$-mesurable, les encombrements $\nu^*$ et $(\mu^*)_x$ ne sont pas nécessairement égaux et la mesure $\nu$ ne présente pas d’intérêt.

#### Définition 1 {#int-ix-s2-def-1 .statement}

Soit $X$ une partie $\mu$-mesurable de $T$. On appelle mesure induite par $\mu$ sur le sous-espace $X$, et on note $\mu_X$ ou $\mu|X$, la restriction de $\mu : K \mapsto \mu_K$ à l’ensemble des parties compactes de $X$.

#### Proposition 1 {#int-ix-s2-prop-1 .statement}

Soit $X$ une partie $\mu$-mesurable de $T$. L’encombrement $(\mu_X)^*$ est égal à l’encombrement $(\mu^*)_x$ induit par $\mu^*$ sur $X$ (§ 1, n° 1). Autrement dit, on a $(\mu_X)^*(g) = \mu^*(g^0)$ pour toute fonction $g \in \mathcal{F}_+(X)$.
Soient $f \in \mathcal{F}_+(X)$ et $f^0$ le prolongement par 0 de $f$ à $T$. On a $(\mu^*)_x(f) =$ n° 2.2.

$\mu^*(f^0) = \sup_L \mu^*(f^0 \varphi_L)$, L parcourant l’ensemble des parties compactes de T ($§ 1$, n° 2, prop. 2); de même, on a $(\mu_X)^*(f) = \sup_K \mu_K^*(f_K) = \sup_K \mu^*(f^0 \varphi_K)$, K parcourant l’ensemble des parties compactes de X. Tout revient donc à montrer que $\mu^*(f^0 \varphi_L) = \sup_K \mu^*(f^0 \varphi_K)$ pour tout compact L de T, K parcourant l’ensemble des compacts de $L \cap X$. Or soit $(K_n)$ une suite croissante d’ensembles compacts contenus dans $L \cap X$, telle que $(L \cap X) - \bigcup_n K_n$ soit localement $\mu$-négligeable ($§ 1$, n° 8, prop. 11); $f^0$ étant nulle hors de X, $f^0 \varphi_L$ est nulle hors de $L \cap X$, et donc égale localement presque partout à l’enveloppe supérieure de la suite $(f^0 \varphi_{K_n})$. Cela entraîne $\mu^*(f^0 \varphi_L) = \sup_n \mu^*(f^0 \varphi_{K_n})$, d’où le résultat cherché.

#### Remarque 1 {#int-ix-s2-n1-rem-1 .statement}

La relation $(\mu_X)^* = (\mu^*)_X$ permet d’utiliser sans ambiguïté la notation $\mu_X^*$; nous le ferons dans toute la suite. La prop. 1 précédente et la prop. 2 du $§ 1$, n° 2 montrent que les mesures notées $\mu_K$ jusqu’à présent, pour K compact, sont bien des mesures induites au sens de la déf. 1. De même, si T est localement compact, et si X est un sous-espace localement compact de T, la prop. 1 ci-dessus et la prop. 1 du chap. V, 2e éd., $§ 7$, n° 1 montrent que la déf. 1 coïncide avec celle du chap. IV, 2e éd., $§ 5$, n° 7.

#### Remarque 2 {#int-ix-s2-n1-rem-2 .statement}

La déf. 1 s’étend au cas où $\mu$ est une mesure complexe sur T. Pour montrer dans ce cas que la prémesure $\mu_X$ est une mesure, il suffit de remarquer que $|\mu_K| = |\mu|_K$ pour tout compact K de X ($§ 1$, n° 2).

D’après la prop. 1, une partie Y de X est $\mu_X$-mesurable (resp. localement $\mu_X$-négligeable) si et seulement si elle est $\mu$-mesurable (resp. localement $\mu$-négligeable). Si Y est $\mu_X$-mesurable, et donc $\mu$-mesurable, les mesures induites $(\mu_X)_Y$ et $\mu_Y$ sont évidemment égales en vertu de la prop. 1 (« transitivité des mesures induites »).

Remarque 3). — Soit X une partie $\mu$-mesurable de T. D’après la prop. 10 du $§ 1$, n° 8, appliquée à $g = \varphi_X$ il existe un concassage $(K_\alpha)_{\alpha \in A}$ de T tel que l’on ait $K_\alpha \subset X$ ou $K_\alpha \subset \complement X$ pour tout $\alpha \in A$. Si l’on modifie la topologie de T suivant le procédé du scholie du $§ 1$, n° 8, l’espace X’ obtenu en munissant X de la topologie induite par T’ est localement compact, et l’on sait associer à $\mu$ (resp. à $\mu_X$) une mesure $\mu'$ (resp. $\nu$) sur T’ (resp. X’) qui admet la même intégrale supérieure essentielle que $\mu$ (resp. que $\mu_X$): ceci entraîne $\mu'_X = \nu$. Comme les ensembles localement négligeables, les applications mesurables, les fonctions essentiellement intégrables à valeurs dans les espaces de Banach, sont les mêmes pour $\mu$ et $\mu'$, pour $\mu_X$ et pour $\mu'_X$, la théorie de l’intégration par rapport à une mesure induite se trouve ramenée à celle qui a été traitée au chap. V, 2e éd., $§ 7$, dans le cas particulier des espaces localement compacts. Nous laisserons au lecteur le soin de transcrire les résultats.

### 2. Mesures définies par des densités numériques

#### Définition 2 {#int-ix-s2-def-2 .statement}

On dit qu’une fonction $f$ définie dans T, à valeurs dans $\overline{\mathbf{R}}$ ou dans un espace de Banach, est localement $\mu$-intégrable si $f$ est $\mu$-mesurable, et si tout point $x \in T$ admet un voisinage $V$ tel que $\mu^*(|f|\varphi_V) < +\infty$.

Cette définition coïncide avec celle qui a été donnée au chap. V, 2e éd., § 5, n° 1, dans le cas où $T$ est localement compact.

Soit $f$ une fonction positive localement $\mu$-intégrable; l’application $K \mapsto f_K \cdot \mu_K$ est une prémesure (chap. V, 2e éd., § 7, n° 1, cor. 2 du th. 1), que nous noterons $f.\mu$.

#### Proposition 2 {#int-ix-s2-prop-2 .statement}

*Si $f$ est une fonction localement $\mu$-intégrable positive, on a, pour toute fonction $g \in \mathcal{F}_+(T)$, la relation*

$$
(f.\mu)^*(g) = \mu^*(fg).
$$

En effet, on a pour tout ensemble compact $K$ dans $T$

$$
(f.\mu)_K^*(g_K) = (f_K \cdot \mu_K)^*(g_K) = \mu_K^*(f_K g_K) = \mu_K^*((f g)_K),
$$

en utilisant la définition de $f.\mu$ et la prop. 3 du chap. V, 2e éd., § 5, n° 3. La prop. 2 s’en déduit en passant à la borne supérieure sur $K$.

Soient alors $x \in T$ et $V$ un voisinage de $x$ tel que $\mu^*(f \varphi_V) < +\infty$ (déf. 2); on a alors $(f.\mu)^*(V) = \mu^*(f \varphi_V) < +\infty$, et $f.\mu$ est donc une mesure.

#### Définition 3 {#int-ix-s2-def-3 .statement}

*Soit $f$ une fonction positive localement $\mu$-intégrable. La mesure $f.\mu$: $K \mapsto f_K \cdot \mu_K$ est appelée la mesure de densité $f$ par rapport à $\mu$, ou la mesure produit de $\mu$ par la fonction $f$. Toute mesure de la forme $f.\mu$, où $f$ est positive et localement intégrable, est appelée mesure de base $\mu$.*

*Remarques. —* 1) La définition de $f.\mu$ s’étend au cas où $f$ est une fonction localement intégrable complexe; on a alors $|f.\mu| = |f|.\mu$, ce qui entraîne aussitôt que $f.\mu$ est une mesure, et non une simple prémesure. On conserve l’expression « mesures de base $\mu$ » pour désigner les mesures complexes ainsi définies.

2) De même, si $\theta$ est une mesure complexe, on dira que $f$ est localement $\theta$-intégrable si elle est localement $|\theta|$-intégrable, et on définira la mesure $f.\theta$: $K \mapsto f_K \cdot \theta_K$. On a $|f.\theta| = |f|.|f|$ (chap. V, 2e éd., § 5, n° 2, prop. 2). Nous laisserons de côté dans ce n° tout ce qui touche aux mesures non positives.

#### Proposition 3 {#int-ix-s2-prop-3 .statement}

*Soit $\nu$ une mesure sur $T$. Pour que $\nu$ soit de la forme $f.\mu$, où $f$ est une fonction positive localement $\mu$-intégrable, il faut et il suffit que tout ensemble compact $\mu$-négligeable soit $\nu$-négligeable. Si $f'$ est une seconde fonction localement $\mu$-intégrable telle que $\nu = f'.\mu$, on a $f = f'$ localement $\mu$-presque partout.*

La condition est évidemment nécessaire (prop. 2). Inversement, supposons que tout ensemble compact $\mu$-négligeable soit $\nu$-négligeable. Introduisons un concassage $(K_\alpha)_{\alpha \in A}$ de $T$ pour la mesure $\mu + \nu$ et posons $N = T - \bigcup_{\alpha \in A} K_\alpha$. Il est clair que $(K_\alpha)_{\alpha \in A}$ est un concassage pour $\mu$ et pour $\nu$, et la prop. 9 du § 1, n° 8 entraîne donc les relations suivantes pour tout $g \in \mathcal{F}_+$:

$$
\mu^*(g) = \sum_{\alpha \in A} \mu_{K_\alpha}^*(g_{K_\alpha}), \quad \nu^*(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^*(g_{K_\alpha}).
$$

n° 2.3.

Considérons un compact $C \subset K_\alpha$ qui soit $\mu_{K_\alpha}$-négligeable; alors $C$ est localement $\mu$-négligeable, donc localement $\nu$-négligeable, et enfin $\nu_{K_\alpha}$-négligeable par définition de $\nu$. Il résulte alors du th. de Lebesgue–Nikodym (chap. V, 2e éd., § 5, n° 5, th. 2) que $\nu_{K_\alpha}$ admet une densité $f_\alpha$ par rapport à $\mu_{K_\alpha}$. Soit $f$ la fonction qui coïncide avec $f_\alpha$ dans chacun des ensembles $K_\alpha$, et avec 0 dans $\mathbf{N}$; la fonction $f$ est $\mu$-mesurable (chap. IV, 2e éd., § 5, n° 10, prop. 16), et on a pour toute fonction $g \in \mathcal{F}_+$, d’après les relations ci-dessus, et la prop. 3 du chap. V, 2e éd., § 5, n° 3,

$$
\nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_\alpha g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet((f g)_{K_\alpha}) = \mu^\bullet(fg).
$$

Il en résulte d’abord que $f$ est localement $\mu$-intégrable: si $x$ est un point de $T$, et si $V$ est un voisinage de $x$ tel que $\nu^\bullet(V) < +\infty$, on a $\mu^\bullet(f \varphi_V) < +\infty$. Ensuite, la prop. 2 montre que les mesures $\nu$ et $f.\mu$ ont même intégrale supérieure essentielle. Elles sont donc égales ($§ 1$, n° 2, cor. de la prop. 2). L’unicité de $f$ étant évidente à partir du cas des espaces compacts, la proposition est établie.

Remarque 3). — La théorie de l’intégration par rapport à une mesure $\nu = f.\mu$ se ramène aussitôt à la théorie traitée au chap. V. Soit en effet $(K_\alpha)_{\alpha \in A}$ un concassage de $T$ pour $\mu$, donc pour $\nu$, et soit $T'$ l’espace localement compact défini dans le scholie du $§ 1$, n° 8; nous pouvons associer à $\mu$ (resp. à $\nu$) une mesure $\mu'$ (resp. $\nu'$) sur $T'$, de telle sorte que les fonctions mesurables, les fonctions essentiellement intégrables à valeurs dans un espace de Banach, les intégrales supérieures essentielles des fonctions positives, soient les mêmes pour $\mu$ et $\mu'$ (resp. pour $\nu$ et $\nu'$). La fonction $f$ est donc $\mu'$-mesurable; elle est localement $\mu'$-intégrable, car $T'$ est localement compact, et un ensemble compact de $T'$ ne rencontre qu’un nombre fini de compacts $K_\alpha$ ($\alpha \in A$). La relation ${\nu'}^\bullet(g) = \nu^\bullet(g) = \mu^\bullet(fg) = {\mu'}^\bullet(fg)$ prouve enfin que $\nu' = f.\mu'$ (chap. V, 2e éd., § 5, n° 3, prop. 3). Nous laissons au lecteur le soin de transcrire les résultats du chap. V, 2e éd., § 5.

### 3. Image d’une mesure

#### Définition 4 {#int-ix-s2-def-4 .statement}

Soit $\pi$ une application de $T$ dans un espace topologique $X$. On dit que $\pi$ est $\mu$-propre si $\pi$ est $\mu$-mesurable, et si tout point $x$ de $X$ admet un voisinage $V$ tel que $\mu^\bullet(\pi^{-1}(V)) < +\infty$.

#### Remarque 1 {#int-ix-s2-n3-rem-1 .statement}

Lorsque $T$ et $X$ sont localement compacts, cette définition est équivalente à celle du chap. V, 2e éd., § 6, n° 1.

#### Remarque 2 {#int-ix-s2-n3-rem-2 .statement}

Une application continue propre (Top. gén., 4e éd., chap. I, § 10, n° 1, déf. 1) de $T$ dans $X$ est $\mu$-propre pour toute mesure $\mu$. En effet, soit $x \in X$; comme $\pi^{-1}(x)$ est compact (loc. cit., n° 2, th. 1), l’ensemble $\pi^{-1}(x)$ possède un voisinage ouvert $H$ tel que $\mu^\bullet(H) < +\infty$. Posons $V = X - \pi(T - H)$; comme $\pi$ est fermée, $V$ est ouvert dans $X$, contient $x$, et on a $\pi^{-1}(V) \subset H$ d’où $\mu^\bullet(\pi^{-1}(V)) \leq \mu^\bullet(H) < +\infty$.

#### Remarque 3 {#int-ix-s2-n3-rem-3 .statement}

Si $\mu$ est bornée, toute application $\mu$-mesurable de $T$ dans $X$ est $\mu$-propre.

#### Remarque 4 {#int-ix-s2-n3-rem-4 .statement}

Si $\theta$ est une mesure complexe sur $T$, on dira que $\pi$ est $\theta$-propre si $\pi$ est propre pour la mesure positive $|\theta|$.

#### Proposition 4 {#int-ix-s2-prop-4 .statement}

Soit $\pi$ une application $\mu$-propre de $T$ dans un espace topologique $X$. Il existe sur $X$ une mesure $\nu$ et une seule telle que $\nu^*$ soit égal à l’encombrement image $\pi(\mu^*)$ ($§ 1, n^o 1$), autrement dit, telle que $\nu^*(g) = \mu^*(g \circ \pi)$ pour tout $g \in \mathcal{F}_+(X)$.

L’unicité est évidente ($§ 1, n^o 2$, cor. de la prop. 2). Pour établir l’existence, nous traiterons d’abord le cas où $\mu$ est portée par un ensemble compact $K$, tel que la restriction de $\pi$ à $K$ soit continue. Alors $L = \pi(K)$ est compact; soit $\pi'$ l’application continue de $K$ dans $L$ induite par $\pi$, et soient $\nu'$ la mesure image $\pi'(\mu_K)$ sur $L$, $\nu$ la mesure sur $X$ définie par $\nu'$ ($§ 1, n^o 3$, Exemple 2). On a, pour tout $g \in \mathcal{F}_+(X)$,

$$
\nu^*(g) = {\nu'}^*(g_L) = \mu_K^*(g_L \circ \pi') = \mu_K^*((g \circ \pi)_K) = \mu^*((g \circ \pi)_K^o) = \mu^*(g \circ \pi)
$$

(on a utilisé successivement la formule (3) du $§ 1, n^o 3$, la prop. 2 du chap. V, 2e éd., $§ 6, n^o 2$, la définition de $\mu_K^*$, et le fait que $\mu$ est portée par $K$). Autrement dit, on a $\nu^* = \pi(\mu^*)$.

Passons maintenant au cas général; d’après les prop. 10 et 9 du $§ 1, n^o 8$, $\mu$ est somme d’une famille sommable $(\mu_\alpha)_{\alpha \in A}$ de mesures à support compact, telles que la restriction de $\pi$ au support $K_\alpha$ de $\mu_\alpha$ soit continue pour tout $\alpha \in A$. Le cas particulier traité plus haut permet d’associer à chaque mesure $\mu_\alpha$ sur $T$ une mesure $\nu_\alpha$ sur $X$ telle que $\nu_\alpha^* = \pi(\mu_\alpha^*)$. On a alors, pour $g \in \mathcal{F}_+(X)$,

$$
\sum_{\alpha \in A} \nu_\alpha^*(g) = \sum_{\alpha \in A} \mu_\alpha^*(g \circ \pi) = \mu^*(g \circ \pi).
$$

L’encombrement $\pi(\mu^*)$ est localement borné, puisque $\pi$ est $\mu$-propre; la famille $(\nu_\alpha)_{\alpha \in A}$ est donc sommable ($§ 1, n^o 7$, prop. 7), et sa somme $\nu$ satisfait à l’énoncé.

#### Définition 5 {#int-ix-s2-def-5 .statement}

Si $\pi$ est une application $\mu$-propre de $T$ dans un espace topologique $X$, l’unique mesure $\nu$ sur $X$ telle que $\nu^*(g) = \mu^*(g \circ \pi)$ pour tout $g \in \mathcal{F}_+(X)$ est appelée la mesure image de $\mu$ par $\pi$, et notée $\pi(\mu)$.

#### Exemple {#int-ix-s2-n3-exa-1 .statement}

Soient $K$ un sous-espace compact de $T$, $i$ l’injection canonique de $K$ dans $T$, $\lambda$ une mesure sur $K$; $i$ étant continue, et $\lambda$ étant bornée, $i$ est $\lambda$-propre. La formule (3) du $§ 1, n^o 3$ montre que la « mesure sur $T$ définie par $\lambda$ » est la mesure image $i(\lambda)$.

Remarque 5). — Si $\theta$ est une mesure réelle, et si $\pi$ est $\theta$-propre, $\pi$ est propre pour les mesures $\theta^+$ et $\theta^-$; on posera alors $\pi(\theta) = \pi(\theta^+) - \pi(\theta^-)$. Si $\theta$ est une mesure complexe, et si $\pi$ est $\theta$-propre, elle est propre pour les mesures réelles $\Re(\theta)$ et $\Im(\theta)$; on posera alors

$$
\pi(\theta) = \pi(\Re(\theta)) + i \pi(\Im(\theta)).
$$

#### Proposition 5 {#int-ix-s2-prop-5 .statement}

Soit $\pi$ une application $\mu$-propre de $T$ dans un espace topologique $X$, et soit $f$ une application de $X$ dans un espace topologique $F$ (séparé ou non). Pour que $f$ soit $\pi(\mu)$-mesurable, il faut et il suffit que $f \circ \pi$ soit $\mu$-mesurable.

Reprenons la démonstration de la prop. 4, et commençons par le cas particulier traité au début, avec les mêmes notations ; g est mesurable pour la mesure $\pi(\mu) = \nu$ si et seulement si $g_L$ est $\nu'$-mesurable ($§ 1$, no 5, Exemple) ; or cela équivaut à dire que $g_L \circ \pi' = (g \circ \pi)_K$ est $\mu_K$-mesurable (chap. V, 2e éd., $§ 6$, no 2, prop. 3), et finalement que $g \circ \pi$ est $\mu$-mesurable ($§ 1$, no 5, Exemple). Passons ensuite au cas général, avec les mêmes notations que dans la démonstration de la prop. 4 ; $f$ est $\nu$-mesurable si et seulement si $f$ est $\nu_\alpha$-mesurable pour tout $\alpha \in A$ ($§ 1$, no 7, prop. 8), donc si et seulement si $f \circ \pi$ est $\mu_\alpha$-mesurable pour tout $\alpha \in A$ (cas particulier précédent) et enfin si et seulement si $f \circ \pi$ est $\mu$-mesurable ($§ 1$, no 7, prop. 8).

#### Corollaire {#int-ix-s2-n3-cor-1 .statement}

Soient $X$ et $Y$ deux espaces topologiques, $\pi$ une application $\mu$-propre de $T$ dans $X$, $\pi'$ une application $\pi(\mu)$-propre de $X$ dans $Y$. L’application $\pi'' = \pi' \circ \pi$ est alors $\mu$-propre et $\pi''(\mu) = \pi'(\pi(\mu))$ (« transitivité des images de mesures »).

En effet, $\pi''$ est $\mu$-mesurable (prop. 5). Posons $\mu' = \pi(\mu)$; l’encombrement image $\pi'({\mu'}^*) = \pi'(\pi(\mu^*))$ est évidemment égal à $\pi''(\mu^*)$. Comme il est localement borné, $\pi''$ est $\mu$-propre. Les mesures $\pi''(\mu)$ et $\pi'(\mu')$ ont alors même intégrale supérieure essentielle, et sont donc égales.

#### Proposition 6 {#int-ix-s2-prop-6 .statement}

Soit $\pi$ une application $\mu$-propre de $T$ dans un espace topologique $X$, et soit $B$ une partie $\pi(\mu)$-mesurable de $X$. Posons $A = \pi^{-1}(B)$, et désignons par $\pi'$ l’application de $A$ dans $B$ qui coïncide avec $\pi$ dans $A$. L’ensemble $A$ est alors $\mu$-mesurable, $\pi_A$ et $\pi'$ sont $\mu_A$-propres, et on a

$$
(\pi(\mu))_B = (\pi_A(\mu_A))_B = \pi'(\mu_A).
$$

L’ensemble $A$ est $\mu$-mesurable d’après la prop. 5 appliquée à $\varphi_B$; l’application $\pi_A$ est évidemment $\mu_A$-mesurable d’après la définition des mesures induites (no 1), et il en résulte que $\pi'$ est mesurable. Soit $f$ un élément de $\mathcal{F}_+(B)$; en désignant par des exposants zéros les prolongements par 0 dans $X$ et dans $T$, on a

$$
(\pi(\mu)_B)^*(f) = \pi(\mu)^*(f^0) = \mu^*(f^0 \circ \pi) = \mu^*((f \circ \pi')^0) = \mu_A^*(f \circ \pi'),
$$

d’où $(\pi(\mu)_B)^* = \pi'(\mu_A^*)$. Comme l’encombrement $(\pi(\mu)_B)^*$ est localement borné, il en est de même de $\pi'(\mu_A^*)$ et $\pi'$ est donc $\mu_A$-propre. Les mesures $\pi'(\mu_A)$ et $(\pi(\mu))_B$ ont même intégrale supérieure essentielle, et sont donc égales. L’autre relation s’établit de manière analogue.

#### Proposition 7 {#int-ix-s2-prop-7 .statement}

Soit $T$ un sous-espace d’un espace topologique $X$, et soit $i$ l’injection de $T$ dans $X$.

a) Si $\mu$ est une mesure sur $T$, et si $i$ est $\mu$-propre, la mesure $i(\mu)$ est concentrée sur $T$, et on a $(i(\mu))_T = \mu$.

b) Si $\lambda$ est une mesure sur $X$, telle que $T$ soit $\lambda$-mesurable, $i$ est $\lambda_T$-propre, et on a $i(\lambda_T) = \varphi_T \cdot \lambda$.

a) Posons $\nu = i(\mu)$; la relation $\nu^*(A) = \mu^*(A \cap T)$, appliquée à $A = X - T$, montre que $\nu$ est concentrée sur $T$. La relation $\nu_T = \mu$ est un cas particulier de la relation (2), en prenant $B = T = A$.

b) Soit $f$ une fonction positive définie dans $X$; si l’on pose $\mu = \lambda_T$, on a $\mu^*(f \circ i) = \lambda_T^*(f_T) = \lambda^*(f_{\varphi_T}) \leq \lambda^*(f)$ (prop. 1); il en résulte que $i$ est $\mu$-propre. D’autre part, $\mu^*(f \circ i)$ (resp. $\lambda^*(f_{\varphi_T})$) est l’intégrale supérieure essentielle de $f$ par rapport à $i(\mu)$ (resp. $\varphi_T \cdot \lambda$). Ces deux mesures sont donc égales.

Remarque 6). — Soit $\pi$ une application $\mu$-propre de $T$ dans un espace topologique $X$. On ramène la théorie de l’intégration par rapport à la mesure image $\nu = \pi(\mu)$ à la théorie traitée au chap. V, 2e éd., § 6, de la manière suivante. Soit $(K_\alpha)_{\alpha \in A}$ (resp. $(L_\beta)_{\beta \in B}$) un concassage de $T$ (resp. de $X$) pour $\mu$ (resp. pour $\nu$), et posons $N = T - \bigcup_{\alpha \in A} K_\alpha, P = X - \bigcup_{\beta \in B} L_\beta$. Nous pouvons supposer que la restriction de $\pi$ à chacun des $K_\alpha$ est continue ($§ 1, n° 8,$ prop. 10). Soient $T', X'$ les espaces localement compacts construits comme dans le scholie du $§ 1, n° 8$ et soient $\mu'$ et $\nu'$ les mesures sur ces espaces associées à $\mu$ et $\nu$. La topologie de $T'$ étant somme des topologies des sous-espaces $K_\alpha$ et de la topologie discrète sur $N$, $\pi$ est une application continue de $T'$ dans $X$ et la relation ${\mu'}^*(g \circ \pi) = \mu^*(g \circ \pi) = \nu^*(g)$ (pour $g \in \mathcal{F}_+(X)$) montre que $\pi$ est $\mu'$-propre et que $\pi(\mu') = \nu$. D’autre part, l’application identique $i$ de $X$ sur $X'$ est $\nu$-propre, et on a $i(\nu) = \nu'$. Il en résulte que $\pi$ est une application $\mu'$-propre de $T'$ dans $X'$, et que l’image de $\mu'$ par $\pi$ est $\nu'$ (cor. de la prop. 5). Nous laissons au lecteur le soin de transcrire les résultats du chap. V, 2e éd., § 6.

### 4. Relèvement de mesures

#### Proposition 8 {#int-ix-s2-prop-8 .statement}

Soient $T$ et $X$ deux espaces topologiques, $\pi$ une application de $T$ dans $X$.

a) Soit $\nu$ une mesure bornée sur $X$. Pour qu’il existe sur $T$ une mesure $\mu$, telle que $\pi$ soit $\mu$-propre et que $\pi(\mu) = \nu$, il faut et il suffit qu’il existe, pour tout nombre $\varepsilon > 0$, un ensemble compact $K_\varepsilon \subset T$ tel que la restriction de $\pi$ à $K_\varepsilon$ soit continue et que $\nu^*(X - \pi(K_\varepsilon)) < \varepsilon$.

b) Supposons que $\pi$ soit injective; soient $\mu$ et $\mu'$ deux mesures sur $T$, telles que $\pi$ soit propre pour $\mu$ et $\mu'$, et que $\pi(\mu) = \pi(\mu')$. On a alors $\mu = \mu'$.

La condition énoncée en a) est nécessaire. En effet, si $\pi$ est $\mu$-propre et $\pi(\mu) = \nu$, la relation $\mu^*(1) = \nu^*(1) < +\infty$ entraîne que $\mu$ est bornée. La prop. 2 du $§ 1, n° 2$, appliquée à la fonction 1, entraîne l’existence d’une partie compacte $K$ de $T$ telle que $\mu^*(T - K) < \varepsilon/2$. Comme $\pi$ est $\mu$-mesurable, il existe un ensemble compact $K_\varepsilon \subset K$ tel que la restriction de $\pi$ à $K_\varepsilon$ soit continue, et que $\mu^*(K - K_\varepsilon) < \varepsilon/2$. On a alors (n° 3, prop. 4)
$$
\nu^*(X - \pi(K_\varepsilon)) = \mu^*(T - \pi^{-1}(\pi(K_\varepsilon))) < \varepsilon.
$$

Pour montrer que la condition est suffisante, nous traiterons d’abord un cas particulier.

#### Lemme 1 {#int-ix-s2-lem-1 .statement}

Soient U et V deux espaces compacts, h une application continue de U sur V. L’application $\lambda \mapsto h(\lambda)$ de $\mathcal{M}_+(U)$ dans $\mathcal{M}_+(V)$ est alors surjective.

En effet, soit a l’application linéaire $f \mapsto f \circ h$ de $\mathcal{C}(V)$ dans $\mathcal{C}(U)$; comme h est surjective, a est une isométrie de $\mathcal{C}(V)$ sur un sous-espace H de $\mathcal{C}(U)$. Soit $\theta$ une mesure positive sur V; alors $\theta \circ a^{-1}$ est une forme linéaire continue sur H, qui est prolongeable en une forme linéaire $\eta$ sur $\mathcal{C}(U)$ de même norme, en vertu du th. de Hahn–Banach (*Esp. vect. top.*, chap. II, 2e éd., § 3, n° 2, cor. 1 du th. 1); $\eta$ est alors une mesure sur U, et on a $\theta(f) = \eta(f \circ h)$ pour tout $f \in \mathcal{C}(V)$, de sorte que $\theta = h(\eta)$. Enfin on a $\theta(1) = \| \theta \| = \| \eta \|$, et $\theta(1) = \eta(1)$, de sorte que $\eta$ est positive (chap. V, 2e éd., § 5, n° 5, prop. 9).

Démontrons alors la suffisance de la condition énoncée dans a). Cette condition entraîne l’existence d’une suite $(K_n)_{n \geq 1}$ de parties compactes de T, telle que la restriction de $\pi$ à chacun des $K_n$ soit continue, et qu’on ait, pour tout n, $\nu^*(X - \pi(K_n)) < 1/n$. La suite $(K_n)$ peut-être supposée croissante. Posons $L_n = \pi(K_n)$ et désignons par $\nu'_n$ la mesure $\varphi_{L_n - L_{n-1}} \cdot \nu_{L_n}$ sur $L_n$, en convenant que $L_0 = \emptyset$.

La restriction $\pi_{K_n}$ étant continue, il existe une mesure $\mu'_n$ sur $K_n$ telle que $\pi_{K_n}(\mu'_n) = \nu'_n$ (lemme 1). Soit $\mu_n$ l’image de $\mu'_n$ par l’injection canonique de $K_n$ dans T, et soit g un élément de $\mathcal{F}_+(X)$. En utilisant successivement le fait que $\nu$ est concentrée sur $\bigcup_n L_n$, la prop. 4 du § 1, n° 5, la prop. 2 du § 1, n° 2, la prop. 4 du n° 3 et enfin la prop. 7 du n° 3, il vient

$$
\nu^*(g) = \sum_n \nu^*(\varphi_{L_n - L_{n-1}} g) = \sum_n {\nu'_n}^*(g_{L_n}) = \sum_n {\mu'_n}^*(g_{L_n} \circ \pi_{K_n})
$$
$$
= \sum_n {\mu'_n}^*((g \circ \pi)_{K_n}) = \sum_n \mu_n^*(g \circ \pi).
$$

En prenant $g = 1$ dans cette formule, on voit que la famille $(\mu_n)$ est sommable et que sa somme est une mesure bornée $\mu$ (§ 1, n° 7, prop. 7). D’après la prop. 5 du n° 3, l’application $\pi$ est $\mu_n$-mesurable pour tout n, car $\pi_{K_n}$ est continue, donc $\mu'_n$-mesurable; il en résulte que $\pi$ est $\mu$-mesurable (§ 1, n° 7, prop. 8), donc $\mu$-propre puisque $\mu$ est bornée. Les relations ci-dessus prouvent alors que les mesures $\pi(\mu)$ et $\nu$ ont même intégrale supérieure essentielle, et sont donc égales (§ 1, n° 2, cor. de la prop. 2).

Supposons enfin que $\pi$ soit injective, et démontrons b). Soit f un élément de $\mathcal{F}_+(T)$; comme $\pi$ est injective, il existe une fonction $g \in \mathcal{F}_+(X)$ telle que $f = g \circ \pi$, et on a, d’après la prop. 4 du n° 3, en posant $\nu = \pi(\mu) = \pi(\mu')$,

$$
\mu^*(f) = \mu^*(g \circ \pi) = \nu^*(g) = {\mu'}^*(g \circ \pi) = {\mu'}^*(f).
$$

Les deux mesures $\mu$ et $\mu'$ ont donc même intégrale supérieure essentielle, ce qui entraîne leur égalité (§ 1, n° 2, cor. de la prop. 2).

#### Remarque {#int-ix-s2-n4-rem-1 .statement}

Supposons que $\pi$ soit injective. Soit $\theta$ une mesure complexe telle que $\pi$ soit $\theta$-propre, et que $\pi(\theta) = 0$; on a alors $\theta = 0$. En effet, on se ramène, en séparant les parties réelles et imaginaires, au cas où θ est réelle. On a alors π(θ⁺) = π(θ⁻), donc θ⁺ = θ⁻ (prop. 8) et finalement θ = 0.

Voici un cas important où la condition a) de la prop. 8 est toujours vérifiée.

#### Proposition 9 {#int-ix-s2-prop-9 .statement}

*Soient T un espace souslinien (Top. gén., chap. IX, 3e éd., § 6, n° 2, déf. 2), X un espace séparé, π une application continue de T sur X, et ν une mesure bornée sur X. Il existe alors une mesure bornée μ sur T telle que π(μ) = ν.*

Les hypothèses entraînent évidemment que X est souslinien.

Considérons la fonction d’ensemble $c : A \mapsto \nu^*(\pi(A))$ sur $\mathfrak{P}(T)$. La relation $A \subset B$ entraîne $c(A) \leq c(B)$; si $(A_n)$ est une suite croissante de parties de T, et si $A = \bigcup_{n \in \mathbf{N}} A_n$, on a $c(A) = \sup_n c(A_n)$ du fait que $\nu^*$ est un encombrement. Enfin, soient $A \subset T$, et ε un nombre > 0; choisissons un ouvert G de X contenant $\pi(A)$, et tel que $\nu^*(G) \leq \nu^*(\pi(A)) + \varepsilon$ (§ 1, n° 9, prop. 13); l’ouvert $H = \pi^{-1}(G)$ de T contient A, et on a $c(H) \leq c(A) + \varepsilon$. La fonction c est donc une capacité continue à droite sur T (*Top. gén.*, chap. IX, 3e éd., § 6, n° 9, déf. 9) et le théorème de capacitabilité (*loc. cit.*, th. 5) entraîne l’égalité $c(T) = \sup_K c(K)$, K parcourant l’ensemble des parties compactes de T. La proposition 8 entraîne alors l’existence de la mesure μ cherchée.

### 5. Produit de deux mesures

Soient S et T deux espaces topologiques, munis respectivement de deux prémesures (positives) λ et μ, et soit X l’espace produit S × T. Soit K une partie compacte de X; désignons par A et B les projections de K sur S et T respectivement, et posons

$$(3)$$
$$\nu_K = (\lambda_A \otimes \mu_B)_K.$$

Nous définissons ainsi une prémesure sur X. En effet, soit L une partie compacte de X contenant K, et soient C et D ses deux projections; on a $A \subset C, B \subset D$, et par conséquent, en utilisant la transitivité des mesures induites et la prop. 12 du chap. V, 2e édit., § 8, n° 5

$$(\nu_L)_K = ((\lambda_C \otimes \mu_D)_L)_K = (\lambda_C \otimes \mu_D)_K = ((\lambda_C \otimes \mu_D)_{A \times B})_K = (\lambda_A \otimes \mu_B)_K = \nu_K.$$

#### Définition 6 {#int-ix-s2-def-6 .statement}

*La prémesure ν définie par (3) est appelée la prémesure produit de λ et μ, et notée $\lambda \otimes \mu$.*

Cette définition s’étend évidemment au cas où λ et μ sont des prémesures complexes, et on a alors $|\lambda \otimes \mu| = |\lambda| \otimes |\mu|$ (chap. III, 2e éd., § 4, n° 2, prop. 3 et chap. IV, 2e éd., § 5, n° 7, lemme 3).

Nous conserverons les notations du chap. III, 2e éd., § 4 et du chap. V, 2e éd., § 8, relatives aux produits de mesures et aux intégrales itérées. En particulier, si f et g sont deux fonctions définies respectivement dans S et dans T, à n° 2.5.

valeurs dans $\overline{\mathbf{R}}_+$ ou dans $\mathbf{C}$, la fonction $(s, t) \mapsto f(s)g(t)$ sur $S \times T$ sera notée $f \otimes g$.

#### Proposition 10 {#int-ix-s2-prop-10 .statement}

*Soit $\nu$ la prémesure produit de $\lambda$ et $\mu$; on a, pour toute fonction $f \in \mathcal{F}_+(S)$ et toute fonction $g \in \mathcal{F}_+(T)$,*

$$
\nu^*(f \otimes g) = \lambda^*(f)\mu^*(g).
$$

*La prémesure $\nu$ est la seule prémesure sur $S \times T$ qui satisfasse à (4).*

Nous avons en effet, lorsque $K$ (resp. $L$) parcourt l’ensemble des parties compactes de $S$ (resp. de $T$)

$$
\begin{align*}
\nu^*(f \otimes g) &= \sup_{K, L} \nu^*_{K \times L}((f \otimes g)_{K \times L}) = \sup_{K, L} (\lambda_K \otimes \mu_L)^*(f_K \otimes g_L) \\
&= \sup_{K, L} \lambda_K^*(f_K) \cdot \mu_L^*(g_L) = (\sup_K \lambda_K^*(f_K))(\sup_L \mu_L^*(g_L)) \\
&= \lambda^*(f)\mu^*(g),
\end{align*}
$$

d’après la prop. 8 du chap. V, § 8, n° 3.

Soit $\eta$ une seconde prémesure sur $S \times T$ satisfaisant à (4), et soient $K$ et $L$ deux parties compactes de $S$ et $T$ respectivement, $f$ et $g$ deux éléments de $\mathcal{F}_+(K)$ et de $\mathcal{F}_+(L)$ respectivement. On a la relation $(f \otimes g)^0 = f^0 \otimes g^0$ entre les prolongements par 0, et donc (§ 1, n° 2, prop. 2)

$$
\eta_{K \times L}^*(f \otimes g) = \eta^*((f \otimes g)^0) = \eta^*(f^0 \otimes g^0) = \lambda^*(f^0)\mu^*(g^0) = \lambda_K^*(f)\mu_L^*(g).
$$

En particulier, si l’on prend $f \in \mathcal{K}_+(K)$, $g \in \mathcal{K}_+(L)$, on voit que $\eta_{K \times L}$ possède la propriété caractéristique de la mesure produit $\lambda_K \otimes \mu_L$ (chap. III, 2e éd., § 4, n° 1, th. 1). On a donc $\eta_{K \times L} = \nu_{K \times L}$; comme toute partie compacte de $S \times T$ est contenue dans un ensemble de la forme $K \times L$, la transitivité des mesures induites entraîne que $\eta = \nu$.

#### Corollaire 1 {#int-ix-s2-prop-10-cor-1 .statement}

*Si $\lambda$ et $\mu$ sont des mesures, $\nu$ est une mesure.*

En effet, soit $x = (s, t)$ un point de $X$, et soient $U$ et $V$ deux voisinages de $s, t$ respectivement, tels que $\lambda^*(U) < +\infty, \mu^*(V) < +\infty$; l’ensemble $U \times V$ est un voisinage de $x$, et on a $\nu^*(U \times V) = \lambda^*(U)\mu^*(V) < +\infty$ d’après (4); l’encombrement $\nu^*$ est donc localement borné, et la prémesure $\nu$ est une mesure.

Ce résultat s’étend aussitôt aux mesures complexes.

#### Corollaire 2 {#int-ix-s2-prop-10-cor-2 .statement}

*Si $A$ est une partie de $S$ localement négligeable pour $\lambda$, $A \times T$ est localement $\nu$-négligeable.*

#### Corollaire 3 {#int-ix-s2-prop-10-cor-3 .statement}

*Supposons que $\lambda$ (resp. $\mu$) soit somme d’une famille sommable $(\lambda_\alpha)_{\alpha \in A}$ (resp. $(\mu_\beta)_{\beta \in B}$) de mesures sur $S$ (resp. $T$). La famille $(\lambda_\alpha \otimes \mu_\beta)_{(\alpha, \beta) \in A \times B}$ est alors sommable, et sa somme est $\lambda \otimes \mu$.*

En effet, soit $p$ l’encombrement $\sum_{\alpha, \beta} (\lambda_\alpha \otimes \mu_\beta)^*$; si $f \in \mathcal{F}_+(S)$, $g \in \mathcal{F}_+(T)$, on a évidemment $p(f \otimes g) = \lambda^*(f)\mu^*(g)$. La démonstration du cor. 1 montre alors que $p$ est localement borné, de sorte que la famille $(\lambda_\alpha \otimes \mu_\beta)$ est sommable (§ 1, n° 7, prop. 7). Sa somme $\eta$ est alors telle que $\eta^* = p$ (§ 1, n° 7, prop. 7), et la prop. 10 entraîne $\eta = \nu$.

### 6. Intégration par rapport au produit de deux mesures

Dans tout ce n°, $\lambda$ et $\mu$ désignent deux mesures sur $S$ et $T$ respectivement, et $\nu$ désigne la mesure produit $\lambda \otimes \mu$ sur $S \times T$. En outre, si $f$ est une fonction positive sur $S \times T$, on notera $f_s$ la fonction $t \mapsto f(s, t)$ sur $T$ pour tout $s \in S$, et on notera $I_f$ la fonction $s \mapsto \mu^*(f_s)$ sur $S$.

#### Lemme 2 {#int-ix-s2-lem-2 .statement}

Soit $f$ une fonction positive $\nu$-mesurable sur $S \times T$; pour toute partie compacte $L$ de $T$, soit $I_f^L$ la fonction $s \mapsto \mu^*(f_s \varphi_L)$ sur $S$. La fonction $I_f^L$ est alors $\lambda$-mesurable et on a :
$$
(5) \quad I_f = \sup_L I_f^L
$$
$$
(6) \quad \nu^*(f) = \sup_L \lambda^*(I_f^L),
$$
$L$ parcourant l’ensemble des parties compactes de $T$.

Notons d’abord que l’inclusion $L \subset L'$ entraîne $I_f^L \leq I_f^{L'}$; on a d’autre part $I_f^L(s) = \mu_L^*((f_s)_L)$ pour tout $s \in S$. La formule (5) est donc une conséquence immédiate de la définition de l’encombrement $\mu^*$ donnée au § 1, n° 2. Si $K$ est une partie compacte de $S$ et $L$ une partie compacte de $T$, on a $\nu_{K \times L} = \lambda_K \otimes \mu_L$ par construction, et la prop. 7 du chap. V, 2e éd., § 8, n° 3 entraîne la relation
$$
(7) \quad \nu^*(f \varphi_{K \times L}) = \lambda_K^*(I_f^L).
$$

Par ailleurs, toute partie compacte de $S \times T$ est contenue dans un ensemble compact de la forme $K \times L$; passant à l’enveloppe supérieure sur $K$ et $L$ dans la formule précédente, on obtient donc
$$
(8) \quad \nu^*(f) = \sup_L \sup_K \lambda_K^*(I_f^L) = \sup_L \lambda^*(I_f^L),
$$
c’est-à-dire (6).

Enfin, la prop. 7 du chap. V, 2e éd., § 8, n° 3, entraîne que la restriction de $I_f^L$ à tout compact $K$ de $T$ est $\lambda_K$-mesurable; cela équivaut à dire que $I_f^L$ est $\lambda$-mesurable.

#### Proposition 11 {#int-ix-s2-prop-11 .statement}

Soit $f$ une fonction semi-continue inférieurement $\geq 0$ définie dans $X = S \times T$.
a) La fonction $f_s : t \mapsto f(s, t)$ est semi-continue inférieurement dans $T$ pour tout $s \in S$.
b) La fonction $I_f : s \mapsto \int^\cdot f(s, t) \, d\mu(t)$ est semi-continue inférieurement dans $S$, et l’on a :
$$
(9) \quad \iint_X f(s, t) \, d\nu(s, t) = \int_S d\lambda(s) \int_T f(s, t) \, d\mu(t).
$$

La propriété a) est évidente, car l’application $t \mapsto f(s, t)$ de $T$ dans $\overline{\mathbf{R}}$ est composée de $f$ et de l’application continue $t \mapsto (s, t)$ de $T$ dans $X$. Pour établir b), nous utiliserons un lemme:

#### Lemme 3 {#int-ix-s2-lem-3 .statement}

Soient $X$ un espace topologique (séparé ou non), $f$ une fonction semi-continue inférieurement $\geqslant 0$ définie dans $X$; alors $f$ est limite d’une suite croissante $(f_n)_{n \in \mathbf{N}}$ de fonctions semi-continues inférieurement dans $X$, telle que chaque fonction $f_n$ soit une combinaison linéaire, à coefficients positifs, de fonctions caractéristiques d’ensembles ouverts.

Etant donnés deux entiers $k \geqslant 1$ et $n \geqslant 1$, notons $J_{kn}$ la fonction caractéristique de l’intervalle $[k/2^n, +\infty)$ de $\overline{\mathbf{R}}$. Pour tout $x \in \overline{\mathbf{R}}_+$, posons $u_n(x) = 2^{-n} \sum_{k=1}^{n \cdot 2^n} J_{kn}(x)$; il est immédiat que la suite $(u_n(x))_{n \geqslant 1}$ est croissante et admet $x$ pour limite. La suite des fonctions $f_n = u_n \circ f$ est donc croissante et converge vers $f$, et on a $f_n = 2^{-n} \sum_{k=1}^{n \cdot 2^n} \varphi_{U(k, n)}$ où $U(k, n)$ est l’ensemble ouvert $f^{-1}([k/2^n, +\infty))$ de $X$.

Passons à la démonstration de b). La fonction $I_f$ étant l’enveloppe supérieure de la famille filtrante croissante des fonctions $I^L_f$, où $L$ parcourt l’ensemble des parties compactes de $T$ (lemme 2), il nous suffit de montrer que les fonctions $I^L_f$ sont semi-continues inférieurement; la formule (9) se déduit alors de (6) en passant à l’enveloppe supérieure sur $L$ (§ 1, no 6, prop. 5).

Soit donc $\mathcal{H}$ l’ensemble des fonctions semi-continues inférieurement positives $f$ sur $S \times T$ telles que $I^L_f$ soit semi-continue inférieurement pour tout compact $L$ de $T$. D’après la prop. 5 du § 1, no 6, la borne supérieure de tout ensemble filtrant croissant d’éléments de $\mathcal{H}$ appartient à $\mathcal{H}$. D’après le lemme 3, il nous suffit donc de prouver que la fonction caractéristique d’un ouvert $W$ de $S \times T$ appartient à $\mathcal{H}$. De plus, d’après la définition de la topologie produit sur $S \times T$, l’ouvert $W$ est réunion d’une famille filtrante croissante $(W_\alpha)_{\alpha \in A}$ d’ouverts de la forme

$$
W = \bigcup_{1 \leq i \leq n} (U_i \times V_i)
$$

où les $U_i$ sont ouverts dans $S$ et les $V_i$ ouverts dans $T$; d’après les remarques faites plus haut, il nous suffit de montrer que la fonction caractéristique d’un tel ouvert appartient à $\mathcal{H}$. Soient alors $s \in S$, et $U$ l’intersection de la famille (éventuellement vide) formée des ouverts $U_i$ contenant $s$; on voit immédiatement que $\varphi_W(s, t) \leq \varphi_W(s', t)$ pour tout $s' \in U$ et tout $t \in T$, d’où par intégration $I^L_{\varphi_W}(s) \leq I^L_{\varphi_W}(s')$ pour tout $s' \in U$. Par conséquent $I^L_{\varphi_W}$ est semi-continue inférieurement, et la proposition est établie.

#### Corollaire 1 {#int-ix-s2-lem-3-cor-1 .statement}

Soit $f$ une fonction numérique positive définie dans $X = S \times T$; on a

$$
\int \int_X^* f(s, t) \, d\nu(s, t) \geq \int_S^* d\lambda(s) \int_T^* f(s, t) \, d\mu(t).
$$

Soit en effet $g$ une fonction semi-continue inférieurement sur $X$ majorant $f$; on a, d’après la prop. 11,

$$
\iint^* g(s, t)\ dv(s, t) = \int \int^* g(s, t)\ dv(s, t) = \int^* d\lambda(s) \int^* g(s, t)\ d\mu(t)
$$
$$
= \int^* d\lambda(s) \int^* g(s, t)\ d\mu(t) \geq \int^* d\lambda(s) \int^* f(s, t)\ d\mu(t).
$$

L’inégalité (10) s’obtient en passant à l’enveloppe inférieure sur $g$.

#### Corollaire 2 {#int-ix-s2-lem-3-cor-2 .statement}

*Soit $f$ une fonction numérique définie dans $S \times T$ et $\nu$-négligeable. La fonction $f_s : t \mapsto f(s, t)$ est alors $\mu$-négligeable pour $\lambda$-presque tout $s \in S$.*

#### Proposition 12 {#int-ix-s2-prop-12 .statement}

*Soit $f$ une fonction positive $\nu$-mesurable définie dans $X = S \times T$. Supposons que $f$ soit $\nu$-modérée (resp. que $\mu$ soit modérée). Alors
a) L’ensemble $N$ des $s \in S$ tels que la fonction $f_s : t \mapsto f(s, t)$ ne soit pas $\mu$-mesurable est négligeable (resp. localement négligeable) pour $\lambda$.
b) L’application $s \mapsto \int^* f(s, t)\ d\mu(t)$ est $\lambda$-mesurable, et on a*
$$
\iint_X f(s, t)\ dv(s, t) = \int_S d\lambda(s) \int_T^* f(s, t)\ d\mu(t).
$$

Nous commencerons par établir b) lorsque $f$ est $\nu$-modérée. D’après le lemme 2, cette partie de l’énoncé est valable lorsqu’il existe une partie compacte $L$ de $T$ telle que $f$ soit nulle en dehors de $S \times L$; on a en effet dans ce cas $I_f = I_f^{L'}$ pour tout compact $L'$ de $T$ contenant $L$, et la formule (11) se réduit à (6). En particulier, b) est établie pour une fonction $f$ nulle hors d’un compact de $S \times T$. D’autre part, le corollaire 1 de la prop. 11 entraîne que b) est vraie lorsque $f$ est $\nu$-négligeable. Comme toute fonction $\nu$-modérée est somme d’une fonction $\nu$-négligeable et d’une suite de fonctions à support compact ($§ 1,$ n° 9, cor. 3 de la prop. 14), l’assertion b) est vraie lorsque $f$ est $\nu$-modérée.

De même, l’assertion b) est évidente lorsque $\mu$ est portée par une partie compacte $L$ de $T$ (lemme 2). Supposons que $\mu$ soit modérée; il existe alors une suite $(\mu_n)_{n \in \mathbf{N}}$ de mesures à support compact sur $T$, telle que $\mu = \sum_n \mu_n$ ($§ 1,$ n° 9, cor. 5 de la prop. 14), d’où $\nu = \sum_n \lambda \otimes \mu_n$ (n° 5, cor. 3 de la prop. 10). L’assertion b), étant valable pour chacune des mesures $\nu_n = \lambda \otimes \mu_n$, est aussi valable pour $\nu = \sum_n \nu_n$.

Démontrons a); notons $N$ l’ensemble des $s \in S$ tels que $f_s$ ne soit pas $\mu$-mesurable; pour toute partie compacte $L$ de $T$, notons de même $N_L$ l’ensemble des $s \in S$ tels que $f_s \varphi_L$ ne soit pas $\mu$-mesurable. Si $K$ et $L$ sont des ensembles compacts dans $S$ et $T$ respectivement, $f_{K \times L}$ est mesurable par rapport à la mesure $\nu_{K \times L} = \lambda_K \otimes \mu_L$, et la prop. 2 du chap. V, 2e éd., § 8, n° 2 montre que l’ensemble $N_L$ est localement négligeable pour $\lambda_K$; comme $K$ est arbitraire, $N_L$ est localement $\lambda$-négligeable.

Supposons que $f$ soit nulle hors d’un ensemble compact de la forme $K \times L$; alors $N = N_L$, et $N$ est contenu dans $K$; il en résulte que $N$ est $\lambda$-négligeable. De même, si $f$ est $\nu$-négligeable, le corollaire 2 de la prop. 11 entraîne que $N$ est $\lambda$-négligeable. Le cas où $f$ est $\nu$-modérée se traite alors comme ci-dessus, en combinant les deux cas précédents.

Supposons que $\mu$ soit portée par une partie compacte $L$ de $T$; alors, on a encore $N = N_L$, et $N$ est donc localement $\lambda$-négligeable. Toute mesure modérée étant somme d’une suite de mesures à support compact ($§ 1$, n° 9, cor. 5 de la prop. 14), ce résultat s’étend aussitôt au cas où $\mu$ est modérée en utilisant la prop. 8 du $§ 1$, n° 7.

#### Remarque {#int-ix-s2-n6-rem-1 .statement}

Soient $(K_\alpha)_{\alpha \in A}$ un concassage de $S$ pour $\lambda$ et $M = S - \bigcup_{\alpha \in A} K_\alpha$; définissons de manière analogue $(L_\beta)_{\beta \in B}$ et $N$ pour la mesure $\mu$ sur $T$. On note $S'$ l’espace localement compact somme des sous-espaces $K_\alpha$ de $S$ et de l’espace discret $M$; l’espace $T'$ est défini de manière analogue, et l’on pose $X' = S' \times T'$. L’espace localement compact $X'$ est somme de la famille $(K_\alpha \times L_\beta)_{(\alpha, \beta) \in A \times B}$ de sous-espaces compacts de $X$, et d’un sous-espace $P = (M \times T) \cup (S \times N)$ qui est une partie localement $\nu$-négligeable de $X$ (on notera que $P$ n’est pas un espace discret en général). On a vu dans le Scholie du $§ 1$, n° 8 qu’il existe une mesure $\lambda'$ sur $S'$ telle que les fonctions mesurables, l’intégrale supérieure essentielle des fonctions positives, les fonctions essentiellement intégrables et leurs intégrales soient les mêmes pour $\lambda$ et $\lambda'$. Associons la mesure $\mu'$ sur $T'$ à $\mu$ et la mesure $\nu'$ sur $X'$ à $\nu$, conformément au Scholie cité; on voit immédiatement que l’on a $\nu'(f \otimes g) = \lambda'(f) \mu'(g)$ pour $f \in \mathcal{F}_+(S)$ et $g \in \mathcal{F}_+(T)$; on a donc $\nu' = \lambda' \otimes \mu'$ d’après la prop. 10 du n° 5. Comme la topologie de $X'$ est plus fine que celle de $X$, toute fonction $\nu$-modérée est $\nu'$-modérée. Ce procédé permet d’étendre sans nouvelle démonstration le th. de Lebesgue–Fubini (chap. V, 2e éd., § 8, n° 4, th. 1) à la situation présente.

### 7. Un résultat sur la désintégration des mesures

#### Proposition 13 {#int-ix-s2-prop-13 .statement}

Soient $X$ un espace topologique, $\nu$ une mesure modérée sur $X$, $p$ une application $\nu$-propre de $X$ dans un espace topologique $T$, et $\mu = p(\nu)$. On suppose que tout sous-espace compact de $X$ est métrisable. Il existe alors une application $t \mapsto \lambda_t$ de $T$ dans $\mathcal{M}_+(X)$ ayant les propriétés suivantes:
a) pour tout $t \in T$, la mesure $\lambda_t$ est portée par $p^{-1}(t)$;
b) pour toute fonction universellement mesurable$^{(1)}$ positive $f$ sur $X$, la fonction $t \mapsto \lambda_t^*(f)$ est universellement mesurable sur $T$ et l’on a

$$
\int_X^* f(x)\, d\nu(x) = \int_T^* d\mu(t) \int_X^* f(x)\, d\lambda_t(x);
$$

(1) On dit qu’une application d’un espace topologique $X$ dans un espace topologique $Y$ est universellement mesurable si elle est $\mu$-mesurable pour toute mesure $\mu$ sur $X$ (cf. chap. V, 2e éd., § 3, n° 4).

c) l’ensemble des $t \in T$ tels que $\lambda_t(1) \neq 1$ est localement $\mu$-négligeable.
De plus, si $t \mapsto \lambda'_t$ est une application de $T$ dans $\mathcal{M}_+(\mathbf{X})$ satisfaisant aux conditions a) et b), l’ensemble des $t \in T$ tels que $\lambda_t \neq \lambda'_t$ est localement $\mu$-négligeable.
Nous aurons besoin d’un résultat auxiliaire:

#### Lemme 4 {#int-ix-s2-lem-4 .statement}

Soient $X$ un espace topologique, $\nu$ une mesure sur $X$ et $f$ une application $\nu$-mesurable de $X$ dans un espace topologique $F$ (séparé ou non). Il existe une application universellement mesurable $f'$ de $X$ dans $F$, égale à $f$ localement $\nu$-presque partout.
La démonstration est identique à celle de la prop. 7 du chap. V, 2e éd., § 3, n° 4, compte tenu de la prop. 10 du § 1, n° 8.
Passons à la démonstration de la prop. 13.
A) On suppose que $X$ est compact et métrisable et que $p$ est continue et surjective:
L’espace $T$ est alors compact et métrisable (Top. gén., chap. IX, 3e éd., § 2, n° 10). D’après le th. 1 du chap. VI, § 3, n° 1, il existe une application vaguement $\mu$-mesurable et scalairement essentiellement $\mu$-intégrable $H : t \mapsto \eta_t$ de $T$ dans $\mathcal{M}_+(X)$ telle que $\nu = \int_T \eta_t \, d\mu(t)$ et que $\eta_t$ soit de masse totale 1 et portée par $p^{-1}(t)$ pour tout $t \in T$. Soit $(S_n)_{n \in \mathbf{N}}$ un concassage de $T$ pour $\mu$, tel que la restriction de $H$ à chacun des ensembles $S_n$ soit continue (§ 1, n° 8, prop. 10 et 11); on notera $\Lambda : t \mapsto \lambda_t$ l’application de $T$ dans $\mathcal{M}_+(X)$ égale à $H$ sur $S = \bigcup_{n \in \mathbf{N}} S_n$ et à 0 sur $T - S$. Il est clair que l’on a $\nu = \int_T \lambda_t \, d\mu(t)$ et que $\Lambda$ satisfait à la condition a) de l’énoncé; la formule (12) résulte de la prop. 5 du chap. V, 2e éd., § 3, n° 2.
Soit $\theta$ une mesure sur $T$; l’application $\Lambda$ est vaguement $\theta$-mesurable et scalairement essentiellement $\theta$-intégrable, donc aussi $\theta$-adéquate (chap. V, 2e éd., § 3, n° 1, prop. 2, b)). Soit $f$ une fonction positive universellement mesurable sur $X$; d’après la prop. 5 du chap. V, 2e éd., § 3, n° 2, appliquée à $\int \lambda_t d\theta(t)$ l’application $t \mapsto \lambda_t^*(f)$ est $\theta$-mesurable, donc universellement mesurable vu l’arbitraire de $\theta$.
B) On suppose qu’il existe une partie compacte $X'$ de $X$ portant la mesure $\nu$ et telle que $p_{X'}$ soit continue:
Posons alors $T' = p(X')$, et $p' = p_{X'}$; nous noterons $\nu'$ la mesure $\nu_{X'}$ et $\mu'$ la mesure image $p'(\nu')$ sur $T'$. Comme $p'$ est continue et surjective et que $X'$ est compact et métrisable, il existe d’après A) une application $\Lambda' : t' \mapsto \lambda'_{t'}$ de $T'$ dans $\mathcal{M}_+(X')$ satisfaisant aux conditions suivantes:
a') pour tout $t' \in T'$, la mesure $\lambda'_{t'}$ est portée par $X' \cap {p'}^{-1}(t')$;
b') pour toute fonction positive universellement mesurable $f'$ sur $X'$, la fonction $t' \mapsto {\lambda'_{t'}}^*(f')$ est universellement mesurable sur $T'$ et l’on a
$$
\int_{X'} f'(x') \, d\nu'(x') = \int_{T'} d\mu'(t') \int_{X'} f'(x') \, d\lambda'_{t'}(x').
$$
Soit $t \in T$; si $t$ appartient à $T'$, nous noterons $\lambda_t$ l’image de $\lambda'_{t'}$ par l’injection canonique de $X'$ dans $X$, et si $t$ appartient à $T - T'$ nous poserons $\lambda_t = 0$. Le lecteur vérifiera sans peine que l’application $t \mapsto \lambda_t$ satisfait aux conditions a) et b) de l’énoncé.

C) *Existence dans le cas général*:

La mesure $\nu$ sur $X$ étant modérée, nous pouvons choisir un recouvrement $(\mathbf{U}_m)_{m \in \mathbf{N}}$ de $X$ formé d’ouverts $\nu$-intégrables. Soit par ailleurs $(X_n)_{n \in \mathbf{N}}$ un $\nu$-concassage de $X$ tel que la restriction de $p$ à chaque ensemble $X_n$ soit continue ($§ 1$, n° 8, prop. 10 et 11); on notera $\nu_n$ la mesure $\varphi_{X_n} \cdot \nu$ sur $X$ et $\mu_n$ son image par $p$. D’après B), il existe, pour tout entier $n \in \mathbf{N}$, une application $t \mapsto \alpha^n_t$ de $T$ dans $\mathcal{M}_+(X)$ satisfaisant aux conditions suivantes:
$a'')$ La mesure $\alpha^n_t$ est portée par $p^{-1}(t)$ pour tout $t \in T$.
$b'')$ Si $f$ est une fonction positive universellement mesurable sur $X$, la fonction positive $t \mapsto (\alpha^n_t)^*(f)$ sur $T$ est universellement mesurable et l’on a

$$
\int_X f(x) \, d\nu_n(x) = \int_T d\mu_n(t) \int_X f(x) \, d\alpha^n_t(x).
$$

On a $\nu = \sum_{n \in \mathbf{N}} \nu_n$ et $\mu = \sum_{n \in \mathbf{N}} \mu_n$; il résulte immédiatement de la prop. 3 du n° 2 et du lemme 4 ci-dessus qu’il existe une suite $(g_n)_{n \in \mathbf{N}}$ de fonctions positives universellement mesurables sur $T$ telle que $\mu_n = g_n \cdot \mu$ pour tout $n \in \mathbf{N}$ et $\sum_{n \in \mathbf{N}} g_n = 1$.

Pour tout $t \in T$, nous noterons $\beta^n_t$ la mesure $g_n(t) \cdot \alpha^n_t$ sur $X$ et $q_t$ l’encombrement $\sum_{n \in \mathbf{N}} (\beta^n_t)^*$ sur $X$. Soit $f$ une fonction positive universellement mesurable sur $X$; utilisant la prop. 2 du n° 2 et sommant sur $n$ dans (13), on obtient

$$
\int_X f(x) \, d\nu(x) = \int_T q_t(f) \, d\mu(t);
$$

il est clair par ailleurs que la fonction $t \mapsto q_t(f)$ sur $T$ est universellement mesurable.

Pour tout $m \in \mathbf{N}$, soit $E_m$ l’ensemble des $t \in T$ tels que $q_t(\mathbf{U}_m) = +\infty$; l’ensemble $E_m$ est universellement mesurable car il en est ainsi de l’application $t \mapsto q_t(\mathbf{U}_m)$, et $E_m$ est localement $\mu$-négligeable d’après la formule (14) appliquée à $f = \varphi_{\mathbf{U}_m}$, puisque $\nu^*(\mathbf{U}_m)$ est fini. L’ensemble $E = \bigcup_{m \in \mathbf{N}} E_m$ est donc universellement mesurable et localement $\mu$-négligeable. Nous poserons $\lambda_t = 0$ pour $t \in E$. Par ailleurs, soit $t \in T - E$; l’encombrement $q_t$ est localement borné puisque les ouverts $\mathbf{U}_m$ recouvrent $X$ et que $q_t(\mathbf{U}_m)$ est fini; d’après la prop. 7 du $§ 1$, n° 7, il existe une mesure $\lambda_t$ sur $X$ telle que $q_t = \lambda_t^*$ et $\lambda_t = \sum_{n \in \mathbf{N}} \beta^n_t$. Il est immédiat que l’application $t \mapsto \lambda_t$ satisfait aux conditions a) et b) de l’énoncé.

D) *Démonstration de c)*:

Soit $f$ une fonction universellement mesurable, positive et bornée sur $X$; nous allons montrer que la fonction universellement mesurable $h_f : t \mapsto \lambda_t^*(f)$ sur $T$ est une densité de la mesure $\mu_f = p(f \cdot \nu)$ par rapport à $\mu = p(\nu)$. Soit $K$ une partie compacte de T et soit $A = p^{-1}(K)$. Pour tout $t \in T$, la mesure $\lambda_t$ est portée par $p^{-1}(t)$; si $t$ appartient à $K$, on a $p^{-1}(t) \subset A$, d'où $\lambda_t^*(f \varphi_A) = \lambda_t^*(f)$; en revanche, si $t$ appartient à $T - K$, on a $p^{-1}(t) \subset X - A$, d'où $\lambda_t^*(f \varphi_A) = 0$. Appliquant la formule (12) à $f \cdot \varphi_A$, on trouve alors

$$
\mu_f(K) = \int_A^* f(x) \, d\nu(x) = \int_K^* d\mu(t) \int_X^* f(x) \, d\lambda_t(x) = \int_K^* h_f(t) \, d\mu(t),
$$

ce qui établit la relation $\mu_f = h_f \cdot \mu$.

Faisant $f = 1$, on voit que la fonction $h_1 : t \mapsto \| \lambda_t \|$ est une densité de la mesure $\mu_1 = \mu$ par rapport à $\mu$, donc est égale à 1 localement $\mu$-presque partout sur $T$.

E) Unicité:
Soient $t \mapsto \lambda_t^i$ (pour $i = 1, 2$) deux applications de $T$ dans $\mathcal{M}_+(X)$ satisfaisant aux conditions a) et b) de l'énoncé. Comme dans C), choisissons un $\mu$-concassage $(X_n)_{n \in \mathbf{N}}$ de $X$ tel que $p_{X_n}$ soit continue pour tout $n \in \mathbf{N}$, et posons $N = X - \bigcup_{n \in \mathbf{N}} X_n$.

Pour tout entier $n \in \mathbf{N}$, choisissons un ensemble dénombrable $D_n$ de fonctions positives sur $X$, nulles hors de $X_n$, dont les restrictions à $X_n$ forment un ensemble dense dans l'espace normé $\mathcal{C}(X_n)$ (appliquer le th. 1 de Top. gén., chap. X, 2e éd., § 3, n° 3 à l'espace compact métrisable $X_n$). Nous poserons $D = \bigcup_{n \in \mathbf{N}} D_n$.

Soit $f \in D$; d'après D), les fonctions $t \mapsto (\lambda_t^1)^*(f)$ et $t \mapsto (\lambda_t^2)^*(f)$ sont des densités de la mesure $\mu_f$ par rapport à $\mu$, et il existe donc un ensemble localement $\mu$-négligeable $E_f$ dans $T$ tel que $(\lambda_t^1)^*(f) = (\lambda_t^2)^*(f)$ pour $t \in T - E_f$. De plus, d'après (12), l'ensemble $F_i$ des $t \in T$ tels que $(\lambda_t^i)^*(N) \neq 0$ est localement $\mu$-négligeable pour $i = 1, 2$. Comme $D$ est dénombrable, l'ensemble $G = (\bigcup_{f \in D} E_f) \cup F_1 \cup F_2$ est localement $\mu$-négligeable; pour $t \in T - G$ on a $(\lambda_t^1)^*(N) = (\lambda_t^2)^*(N) = 0$ et $(\lambda_t^1)_{X_n} = (\lambda_t^2)_{X_n}$, d'où $\lambda_t^1 = \lambda_t^2$ d'après la prop. 9 du § 1, n° 8.

C.Q.F.D.

#### Remarque 1 {#int-ix-s2-n7-rem-1 .statement}

Si $X$ est un espace souslinien, tout sous-espace compact de $X$ est souslinien, donc métrisable (Top. gén., 3e édit., chap. IX, Appendice I, cor. 2 de la prop 3), et toute mesure sur $X$ est modérée (§ 1, n° 9, Remarque 1). D'après la prop. 13, toute mesure $\nu$ sur $X$ admet donc une désintégration par rapport à toute application $\nu$-propre.

#### Remarque 2 {#int-ix-s2-n7-rem-2 .statement}

Avec les notations de la prop. 13, soit $f$ une fonction $\nu$-mesurable positive. On peut prouver comme au chap. V, 2e éd., § 3, n° 2, prop. 5 que l'ensemble des $t \in T$ tels que $f$ ne soit pas $\lambda_t$-mesurable est localement $\mu$-négligeable, que $t \mapsto \lambda_t^*(f)$ est $\mu$-mesurable, et que l'on a encore la relation (12).

## EXERCICES {#int-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
