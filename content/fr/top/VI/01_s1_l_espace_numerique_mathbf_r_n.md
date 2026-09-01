---
book: top
book_title: General Topology
chapter: VI
chapter_title: ESPACES NUMÉRIQUES ET ESPACES PROJECTIFS
section: 1
section_title: L’espace numérique $\mathbf{R}^n$
lang: fr
source: top-v-x-fr
pdf_pages: 0029-0035, 0049-0051
extraction: ocr
subsections:
    - "no": 1
      title: Topologie de $\mathbf{R}^n$
      page: 0
      pdf_page: 29
    - "no": 2
      title: Le groupe additif $\mathbf{R}^n$
      page: 2
      pdf_page: 30
    - "no": 3
      title: L’espace vectoriel $\mathbf{R}^n$
      page: 2
      pdf_page: 30
    - "no": 4
      title: Variétés linéaires affines de $\mathbf{R}^n$
      page: 4
      pdf_page: 32
    - "no": 5
      title: Topologie des espaces vectoriels et des algèbres sur le corps $\mathbf{R}$.
      page: 5
      pdf_page: 33
    - "no": 6
      title: Topologie des espaces de matrices sur $\mathbf{R}$
      page: 6
      pdf_page: 34
statements: 10
exercises: 13
content_sha256: 6c8b00eea805e2e9590c224ec25f0716f7940b73fa91717b3d62f1569d54110c
---

## § 1. L’ESPACE NUMÉRIQUE $\mathbf{R}^n$

### 1. Topologie de $\mathbf{R}^n$

#### Définition 1 {#top-vi-s1-def-1 .statement}

On appelle espace numérique à n dimensions ou de dimension n (plan numérique lorsque $n = 2$), et on note $\mathbf{R}^n$, l’espace topologique produit de n espaces identiques à la droite numérique $\mathbf{R}$.

#### Remarque {#top-vi-s1-n1-rem-1 .statement}

L’espace $\mathbf{R}^0$ est réduit à un point.

On sait (E, III, p. 49, cor. 1) que, si E est un ensemble infini, $E^n$ est équipotent à E pour tout entier $n > 0$; donc, pour $n > 0$, $\mathbf{R}^n$ est équipotent à $\mathbf{R}$, autrement dit, *a la puissance du continu* (cf. VI, p. 21, exerc. 1 et 2).

#### Définition 2 {#top-vi-s1-def-2 .statement}

On appelle pavé ouvert (resp. pavé fermé) de $\mathbf{R}^n$ toute partie de $\mathbf{R}^n$ qui est le produit de n intervalles ouverts (resp. de n intervalles fermés) de $\mathbf{R}$.

Les pavés ouverts de $\mathbf{R}^n$ forment une base de la topologie de $\mathbf{R}^n$ (I, p. 24); les pavés fermés sont des parties fermées pour cette topologie; l’adhérence d’un pavé ouvert est un pavé fermé; l’intérieur d’un pavé fermé est un pavé ouvert; les pavés ouverts contenant un point $\mathbf{x} = (x_i)_{1 \leq i \leq n}$ de $\mathbf{R}^n$ forment un système fondamental de voisinages de $\mathbf{x}$; il en est de même des pavés fermés de $\mathbf{R}^n$ dont $\mathbf{x}$ est point intérieur.

Tout pavé ouvert non vide de $\mathbf{R}^n$ est *homéomorphe* à $\mathbf{R}^n$ (IV, p. 13, prop. 1).

On en conclut que, lorsque $n \geq 1$, tout ensemble ouvert non vide de $\mathbf{R}^n$ a la puissance du continu.

On appelle *cube ouvert* (resp. *fermé*) de $\mathbf{R}^n$ un pavé ouvert (resp. fermé) qui est le produit de n intervalles *bornés* et de *longueurs égales* (pour $n = 2$, on dit *carré* ouvert (resp. fermé)); la longueur commune de ces intervalles est appelée le côté du cube. Les cubes ouverts $K_m = \prod_{1 \leq i \leq n} ]x_i - \frac{1}{m}, x_i + \frac{1}{m}[$ forment (lorsque $m$ parcourt l’ensemble des entiers > 0, ou une suite d’entiers croissant indéfiniment) un système fondamental dénombrable de voisinages du point $\mathbf{x} = (x_i)$.

Tout pavé ouvert (ou fermé) de $\mathbf{R}^n$ est connexe (I, p. 83, prop. 8); en particulier, $\mathbf{R}^n$ est un espace connexe et localement connexe.

Si A est un ensemble ouvert non vide dans $\mathbf{R}^n$, ses composantes connexes sont donc des ensembles ouverts (I, p. 85, prop. 11); en outre, l’ensemble de ces composantes est dénombrable, car $\mathbf{R}^n$ contient une partie dénombrable dense (par exemple $\mathbf{Q}^n$).

Cherchons la condition pour qu’une partie A de $\mathbf{R}^n$ soit relativement compacte; d’après le th. de Tychonoff (I, p. 63, th. 3), il faut et il suffit que les projections de A sur les espaces facteurs de $\mathbf{R}^n$ soient relativement compactes; d’après le th. de Borel-Lebesgue (IV, p. 6, th. 2), cela équivaut à dire que ces projections sont des parties bornées de $\mathbf{R}$; lorsqu’il en est ainsi, on dit que A est une partie bornée de $\mathbf{R}^n$; donc:

#### Proposition 1 {#top-vi-s1-prop-1 .statement}

*Pour qu’une partie A de $\mathbf{R}^n$ soit relativement compacte, il faut et il suffit qu’elle soit bornée.*

#### Corollaire {#top-vi-s1-n1-cor-1 .statement}

*L’espace $\mathbf{R}^n$ est localement compact, et, pour $n \geq 1$, non compact.*

### 2. Le groupe additif $\mathbf{R}^n$

L’ensemble $\mathbf{R}^n$ muni de la structure de groupe produit des structures de groupe additif des n facteurs de $\mathbf{R}^n$, est un groupe commutatif qu’on note additivement, la somme de $\mathbf{x} = (x_i)$ et de $\mathbf{y} = (y_i)$ étant donc $\mathbf{x} + \mathbf{y} = (x_i + y_i)$. La topologie de l’espace numérique est compatible avec cette structure de groupe; muni de ces deux structures, $\mathbf{R}^n$ est un groupe topologique qu’on appelle *groupe additif de l’espace numérique à n dimensions*.

La structure uniforme de ce groupe, dite *structure uniforme additive* de $\mathbf{R}^n$, est le produit des structures uniformes des groupes facteurs de $\mathbf{R}^n$ (III, p. 21); si, pour chaque entier $p > 0$, on désigne par $V_p$ l’ensemble des couples $(\mathbf{x}, \mathbf{y})$ de points de $\mathbf{R}^n$ tels que $\max_{1 \leq i \leq n} |x_i - y_i| \leq 1/p$, les ensembles $V_p$ forment un *système fondamental d’entourages* de cette structure uniforme. Lorsque nous considérons $\mathbf{R}^n$ comme un espace uniforme, ce sera toujours, sauf mention expresse du contraire, de la structure uniforme additive qu’il sera question. Muni de cette structure, $\mathbf{R}^n$ est un espace uniforme *complet* (II, p. 17, prop. 10).

### 3. L’espace vectoriel $\mathbf{R}^n$

Comme $\mathbf{R}$ est un *corps*, on peut définir sur $\mathbf{R}^n$ une structure d’*espace vectoriel* sur $\mathbf{R}$ (A, II, p. 3), le produit $t \mathbf{x}$ d’un scalaire $t \in \mathbf{R}$ et d’un point (ou vecteur) $\mathbf{x} = (x_i)$ de $\mathbf{R}^n$ étant le point $(tx_i)$; on notera que l’homothétie $(t, \mathbf{x}) \mapsto t\mathbf{x}$ est continue dans $\mathbf{R} \times \mathbf{R}^n$. Si $\mathbf{e}_i$ désigne le vecteur de $\mathbf{R}^n$ dont toutes les coordonnées sont nulles, à l’exception de celle d’indice $i$, qui est égale à 1, les $\mathbf{e}_i$ forment une base de l’espace vectoriel $\mathbf{R}^n$, dite base canonique de cet espace (A, II, p. 25); tout vecteur

$$
\mathbf{x} = (x_i) \in \mathbf{R}^n
$$

s’écrit $\mathbf{x} = \sum_{i=1}^n x_i \mathbf{e}_i$, et la relation $\sum_{i=1}^n t_i \mathbf{e}_i = 0$ entraîne $t_i = 0$ pour $1 \leq i \leq n$.

L’espace vectoriel $\mathbf{R}^n$ est donc de dimension $n$ par rapport au corps $\mathbf{R}$, au sens défini en Algèbre (A, II, p. 97), d’où son nom d’espace numérique à $n$ dimensions.

Soit $f$ une application affine (A, II, p. 130) de l’espace vectoriel $\mathbf{R}^n$ dans l’espace vectoriel $\mathbf{R}^m$ ($m$ et $n$ entiers $\geq 0$). Si on pose $g(\mathbf{x}) = f(\mathbf{x}) - f(0)$, $g$ est une application linéaire de $\mathbf{R}^n$ dans $\mathbf{R}^m$. Soient $a_{ij}$ ($1 \leq j \leq m$) les coordonnées de $g(\mathbf{e}_i)$ dans $\mathbf{R}^m$, $b_j$ ($1 \leq j \leq m$) celles de $f(0)$; si $x_i$ ($1 \leq i \leq n$) est la coordonnée d’indice $i$ de $\mathbf{x} \in \mathbf{R}^n$, $y_j$ ($1 \leq j \leq m$) la coordonnée d’indice $j$ de $\mathbf{y} = f(\mathbf{x})$, on a

$$
y_j = \sum_{i=1}^n a_{ij} x_i + b_j \quad (1 \leq j \leq m).
$$

Toute application affine de $\mathbf{R}^n$ dans $\mathbf{R}^m$ est uniformément continue dans $\mathbf{R}^n$ car c’est la somme d’une fonction constante et d’un homomorphisme continu, donc uniformément continu (III, p. 21).

En particulier, on sait que toute application affine de $\mathbf{R}^n$ sur lui-même est bijective, et que son application réciproque est encore une application affine (A, II, p. 101, corollaire); donc, toute application affine de $\mathbf{R}^n$ sur lui-même est un homéomorphisme (et un automorphisme de la structure uniforme de $\mathbf{R}^n$).

Soit $(\mathbf{a}_i)_{1 \leq i \leq n}$ un système libre de $n$ vecteurs de $\mathbf{R}^n$ (ou, ce qui revient au même (A, II, p. 97, prop. 1), une base de l’espace vectoriel $\mathbf{R}^n$); si $\mathbf{b}$ est un point quelconque de $\mathbf{R}^n$, l’ensemble $P$ des points $\mathbf{x} = \mathbf{b} + \sum_{i=1}^n u_i \mathbf{a}_i$, tels que $-1 \leq u_i \leq 1$ pour $1 \leq i \leq n$, est un voisinage compact de $\mathbf{b}$; en effet, il existe une application affine bijective $f$ de $\mathbf{R}^n$ sur lui-même, telle que $f(\mathbf{b}) = 0$, $f(\mathbf{b} + \mathbf{a}_i) = \mathbf{e}_i$ pour $1 \leq i \leq n$, et $f(P)$ est le cube produit des $n$ intervalles $(-1, +1)$ dans les espaces facteurs de $\mathbf{R}^n$. On dit que $P$ est le parallélétope fermé de centre $\mathbf{b}$, construit sur les vecteurs de base $\mathbf{a}_i$. L’intérieur de $P$ est formé des points $\mathbf{b} + \sum_{i=1}^n u_i \mathbf{a}_i$ tels que $-1 < u_i < 1$ pour $1 \leq i \leq n$; on dit que c’est le parallélétope ouvert de centre $\mathbf{b}$, construit sur les $\mathbf{a}_i$.

Soit $P \in \mathbf{R}[X_1, \ldots, X_n]$ un polynôme à $n$ indéterminées à coefficients réels. La fonction polynomiale associée à $P$ est l’application $f : \mathbf{R}^n \to \mathbf{R}$ qui, à tout vecteur $\mathbf{x} = (x_i) \in \mathbf{R}^n$, fait correspondre le nombre réel $P(x_1, \ldots, x_n)$ (cf. A, IV, §2, no 3). Comme $\mathbf{R}$ est infini, à deux polynômes distincts sont associées deux fonctions polynomiales distinctes (A, IV, §2, no 5, prop. 9).

#### Proposition 2 {#top-vi-s1-prop-2 .statement}

Soit $f : \mathbf{R}^n \to \mathbf{R}$ une fonction polynomiale. L’application $f$ est continue. Si $f$ n’est pas identiquement nulle, le complémentaire de l’ensemble $f^{-1}(0)$ est un ouvert dense de $\mathbf{R}^n$.

L’application $f$ est continue d’après III, p. 47; l’ensemble $f^{-1}(0)$ est donc fermé. Supposons $f$ non identiquement nulle. Soit $\mathbf{x}$ un point quelconque de $\mathbf{R}^n$ et $\mathbf{y}$ un point de $\mathbf{R}^n$ tel que $f(\mathbf{y}) \neq 0$. La fonction $\varphi(t) = f(\mathbf{x} + t(\mathbf{y} - \mathbf{x}))$ est une fonction polynomiale non identiquement nulle de la variable réelle $t$. L’ensemble de ses zéros est fini (A, IV, §2, n° 4, th. 2); il existe donc des valeurs de $t$, arbitrairement petites, telles que $\varphi(t) \neq 0$, ce qui prouve que $\mathbf{x}$ est adhérent au complémentaire de $f^{-1}(0)$.

### 4. Variétés linéaires affines de $\mathbf{R}^n$

Etant donnée une variété linéaire affine non vide $V$ de $\mathbf{R}^n$, de dimension $p$, il existe une application affine $f$ de $\mathbf{R}^n$ sur lui-même, qui transforme $V$ en le sous-espace vectoriel $V'$ engendré par $e_1, \ldots, e_p$ (A, II, p. 129). Comme $V'$ est un pavé fermé et est homéomorphe à $\mathbf{R}^p$, on en conclut:

#### Proposition 3 {#top-vi-s1-prop-3 .statement}

Toute variété linéaire affine non vide de dimension $p$ de $\mathbf{R}^n$ est un ensemble fermé dans $\mathbf{R}^n$, homéomorphe à $\mathbf{R}^p$.

Rappelons (A, II, p. 129) qu’on nomme droites, plans, hyperplans de $\mathbf{R}^n$ les variétés linéaires affines de dimension $1, 2, n - 1$ (lorsque $n \geqslant 1$).

Les $n$ droites passant par $0$ et respectivement par les $n$ points $e_i$, sont appelées axes de coordonnées. Pour $n = 2$ l’axe passant par $e_1$ est dit axe des abscisses, l’axe passant par $e_2$ axe des ordonnées; la première coordonnée d’un point $\mathbf{x} \in \mathbf{R}^2$ s’appelle son abscisse, la seconde son ordonnée.

Toute droite $D$ passant par un point $\mathbf{a}$ admet une représentation paramétrique $t \mapsto \mathbf{a} + t \mathbf{b}$, où $t$ parcourt $\mathbf{R}$, et $\mathbf{b} \neq 0$; cette application est un homéomorphisme de $\mathbf{R}$ sur $D$; le vecteur $\mathbf{b}$ est appelé vecteur directeur de $D$, ses composantes $b_i$ ($1 \leq i \leq n$) paramètres directeurs (ou simplement paramètres) de $D$; si $\mathbf{b}'$ est un autre vecteur directeur de $D$, il existe un nombre réel $h \neq 0$ tel que $\mathbf{b}' = h \mathbf{b}$.

L’ensemble des points $\mathbf{a} + t \mathbf{b}$, où $t$ parcourt l’ensemble des nombres réels $\geq 0$, est appelé demi-droite fermée (ou simplement demi-droite) d’origine $\mathbf{a}$ et de vecteur directeur $\mathbf{b}$ (ou de paramètres directeurs $b_i$). C’est un ensemble fermé dans $\mathbf{R}^n$, homéomorphe à l’intervalle $]0, +\infty[$ de $\mathbf{R}$, donc connexe. La droite $D$ est réunion des deux demi-droites d’origine $\mathbf{a}$ et de vecteurs directeurs $\mathbf{b}$ et $-\mathbf{b}$ respectivement, qui sont dites opposées.

Par abus de langage, on appelle demi-droite ouverte d’origine $\mathbf{a}$ et de vecteur directeur $\mathbf{b}$, l’ensemble des points $\mathbf{a} + t \mathbf{b}$ où $t$ parcourt l’ensemble des nombres $> 0$; c’est un ensemble homéomorphe à l’intervalle $]0, +\infty[$ (donc à $\mathbf{R}$ lui-même), qui n’est pas ouvert dans $\mathbf{R}^n$ si $n > 1$, mais est ouvert par rapport à la droite qui le contient.

Une droite passant par deux points distincts $x$ et $y$ admet aussi la représentation paramétrique $(u, v) \mapsto u x + v y$, où $(u, v)$ parcourt l’ensemble des couples de nombres réels tels que $u + v = 1$. Étant donnés deux points quelconques $x, y$ (distincts ou non), on appelle segment fermé (ou simplement segment) d’extrémités $x, y$ l’ensemble des points $u x + v y$, où $(u, v)$ parcourt l’ensemble des couples de nombres réels tels que $u \geqslant 0, v \geqslant 0$ et $u + v = 1$; un segment fermé est compact et connexe, car si ses extrémités sont distinctes, il est homéomorphe à l’intervalle $[0, 1]$ de $\mathbf{R}$.

Si $x \neq y$, on appelle de même (par abus de langage) segment ouvert d’extrémités $x, y$, l’ensemble des points $u x + v y$ tels que $u > 0, v > 0, u + v = 1$; c’est un ensemble homéomorphe à l’intervalle ouvert ]$0, 1[$ (donc à $\mathbf{R}$ lui-même). Enfin, on appelle parfois segment ouvert en $x$, fermé en $y$, la réunion de $y$ et du segment ouvert d’extrémités $x, y$; c’est un ensemble homéomorphe à l’intervalle $[0, 1[$. Tous les segments d’extrémités $x, y$ sont connexes et ont pour adhérence le segment fermé de mêmes extrémités.

#### Proposition 4 {#top-vi-s1-prop-4 .statement}

*Dans $\mathbf{R}^n$, le complémentaire d’une variété linéaire affine $V$ de dimension $p < n$ est un ouvert dense. Si $p < n - 1$, il est connexe. Si $p = n - 1$, il a deux composantes connexes, homéomorphes à $\mathbf{R}^n$*.

Il existe une application affine de $\mathbf{R}^n$ sur lui-même, qui transforme $V$ en le sous-espace vectoriel $E_p$ engendré par $e_1, \ldots, e_p$. Il suffit donc de traiter le cas où $V = E_p$. L’ensemble $E_p$ est un pavé fermé, d’intérieur vide puisque $p < n$; son complémentaire $U_p$ est donc un ouvert dense. Lorsque $p = n - 1$, l’ensemble $U_p$ est la réunion des deux pavés ouverts définis respectivement par les relations $x_n > 0, x_n < 0$; ces pavés sont connexes, non vides, et disjoints, donc sont les composantes connexes de $U_p$. Lorsque $p < n - 1$, l’ensemble $U_p$ contient la réunion $A$ des trois pavés ouverts $A_1, A_2, A_3$ définis par $x_n > 0, x_{n-1} < 0, x_n < 0$; les intersections $A_1 \cap A_2$ et $A_2 \cap A_3$ ne sont pas vides; l’ensemble $A$ est donc connexe (I, p. 81, cor. de la prop. 2). L’ensemble $A$ contient $U_{n-1}$; il est donc dense dans $\mathbf{R}^n$, et par suite dans $U_p$, ce qui entraîne que $U_p$ est connexe (*loc. cit.* prop. 1).

Les composantes connexes $E_1$ et $E_2$ du complémentaire $G H$ d’un hyperplan sont appelées les *demi-espaces ouverts* déterminés par $H$.

Les adhérences de $E_1$ et $E_2$, qui sont respectivement $E_1 \cup H$ et $E_2 \cup H$, sont appelées les *demi-espaces fermés* déterminés par $H$.

### 5. Topologie des espaces vectoriels et des algèbres sur le corps $\mathbf{R}$.
Soit $E$ un espace vectoriel à $n$ dimensions sur le corps $\mathbf{R}$; si $(a_i)_{1 \leq i \leq n}$ est une *base* de cet espace, tout point $x \in E$ se met d’une seule manière sous la forme $x = \sum_{i=1}^n x_i a_i$, où les $x_i$ sont des nombres réels; l’application $(x_i) \mapsto \sum_{i=1}^n x_i a_i$ est donc une application linéaire bijective de $\mathbf{R}^n$ sur $E$. Si on *transporte* à $E$ la topologie de $\mathbf{R}^n$ par cette

application, E se trouve muni d’une topologie compatible avec sa structure de groupe additif, et pour laquelle l’application $(t, x) \mapsto t x$ de $\mathbf{R} \times E$ dans $E$ est continue. Cette topologie est *indépendante de la base* choisie dans $E$; en effet, si $(a'_i)$ est une autre base de $E$, et si $x = \sum_{i=1}^n x'_i a'_i = \sum_{i=1}^n x_i a_i$, l’application $(x_i) \mapsto (x'_i)$ de $\mathbf{R}^n$ sur lui-même est une application linéaire, donc un homéomorphisme.

Nous verrons ultérieurement que la topologie ainsi définie peut être aussi caractérisée de la manière suivante: c’est la *seule* topologie séparée sur $E$, pour laquelle les fonctions $x - y$ et $t x$ soient continues (dans $E \times E$ et $\mathbf{R} \times E$ respectivement) (EVT, I, §2, th. 2).

Si maintenant $A$ est une *algèbre* de dimension finie $n$ sur le corps $\mathbf{R}$, la topologie précédente sur $A$ (considéré comme espace vectoriel à $n$ dimensions sur $\mathbf{R}$) est non seulement compatible avec la structure de groupe additif de $A$, mais aussi avec sa structure d'*anneau*. Cela résulte de la proposition plus générale suivante:

#### Proposition 5 {#top-vi-s1-prop-5 .statement}

*Soient* $E$, $F$, $G$ *trois espaces vectoriels de dimensions finies sur le corps* $\mathbf{R}$; *toute application bilinéaire*¹ $f$ *de* $E \times F$ *dans* $G$ *est continue*.

En effet, on peut supposer que $E = \mathbf{R}^m$, $F = \mathbf{R}^n$, $G = \mathbf{R}^p$; tout revient à prouver que les coordonnées dans $\mathbf{R}^p$ de $f(x, y)$ sont fonctions continues de $(x, y) \in E \times F$ (I, p. 25, prop. 1); autrement dit, il suffit de montrer que toute *forme bilinéaire* $g$ est continue dans $E \times F$, ce qui est immédiat, puisque $g(x, y)$ est un polynôme par rapport aux coordonnées de $x$ et de $y$.

### 6. Topologie des espaces de matrices sur $\mathbf{R}$

Comme exemple important d’espace vectoriel sur $\mathbf{R}$, citons l’espace $\mathbf{M}_{m, n}(\mathbf{R})$ des *matrices à m lignes et n colonnes* dont les éléments appartiennent à $\mathbf{R}$; c’est un espace de dimension $mn$ sur $\mathbf{R}$, donc homéomorphe à $\mathbf{R}^{mn}$. D’après la prop. 5 de VI, p. 6, le *produit* $X \cdot Y$ de deux matrices $X \in \mathbf{M}_{m, n}(\mathbf{R})$, $Y \in \mathbf{M}_{n, p}(\mathbf{R})$ est fonction continue de $(X, Y)$. En particulier, la topologie de l’espace $\mathbf{M}_n(\mathbf{R})$ des matrices *carrées* d’ordre $n$ (cf. A, II, p. 149) est compatible avec la structure d’anneau sur $\mathbf{M}_n(\mathbf{R})$. En outre:

#### Proposition 6 {#top-vi-s1-prop-6 .statement}

*Dans l’anneau* $\mathbf{M}_n(\mathbf{R})$, *le groupe* $\mathbf{GL}_n(\mathbf{R})$ *des matrices inversibles* est un ensemble ouvert dense, et la topologie induite sur cet ensemble est compatible avec sa structure de groupe.

En effet, $\mathbf{GL}_n(\mathbf{R})$ est le complémentaire de l’ensemble des matrices carrées $X$ dont le déterminant est nul; comme le déterminant de $X$ est un polynôme par

¹ Rappelons (A, II, p. 56) que, si $E$, $F$, $G$ sont trois espaces vectoriels sur $\mathbf{R}$, une application $f$ de $E \times F$ dans $G$ est dite *bilinéaire* si l’on a identiquement $f(x + x', y) = f(x, y) + f(x', y)$, $f(x, y + y') = f(x, y) + f(x, y')$, $f(\lambda x, y) = f(x, \lambda y) = \lambda f(x, y)$, quels que soient les éléments $x$, $x'$ de $E$, $y$, $y'$ de $F$ et $\lambda \in \mathbf{R}$.

rapport aux éléments de $X$, la prop. 2 de VI, p. 4 prouve que $\mathbf{GL}_n(\mathbf{R})$ est ouvert et dense dans $\mathbf{M}_n(\mathbf{R})$.

Montrons enfin que l’application $X \to X^{-1}$ de $\mathbf{GL}_n(\mathbf{R})$ dans lui-même est continue. Les éléments de $X^{-1}$ sont les quotients de fonctions polynomiales des éléments de $X$ par le déterminant de $X$, donc dépendent continûment de $X$ (VI, p. 4, prop. 2).

## EXERCICES {#top-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
