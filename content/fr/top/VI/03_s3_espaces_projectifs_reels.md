---
book: top
book_title: General Topology
chapter: VI
chapter_title: ESPACES NUMÉRIQUES ET ESPACES PROJECTIFS
section: 3
section_title: Espaces projectifs réels
lang: fr
source: top-v-x-fr
book_pages: TG VI.25-TG VI.27
pdf_pages: 0040-0049, 0053-0055
extraction: ocr
subsections:
    - "no": 1
      title: Topologie des espaces projectifs réels
      page: 13
      pdf_page: 41
    - "no": 2
      title: Variétés linéaires projectives
      page: 14
      pdf_page: 42
    - "no": 3
      title: Immersion de l’espace numérique dans l’espace projectif
      page: 16
      pdf_page: 44
    - "no": 4
      title: Application au prolongement des fonctions numériques
      page: 16
      pdf_page: 44
    - "no": 5
      title: Espaces de variétés linéaires projectives
      page: 17
      pdf_page: 45
    - "no": 6
      title: Grassmanniennes
      page: 19
      pdf_page: 47
statements: 12
exercises: 11
content_sha256: b1503459557945e980e161dffa3a02902fe2ed024069911159c065b37425bac6
---

## § 3. ESPACES PROJECTIFS RÉELS

Nous aurons constamment à faire usage, dans ce paragraphe, des notions et résultats relatifs aux *espaces quotients* (I, p. 20), et notamment des deux propriétés suivantes, que nous énoncerons pour plus de commodité sous forme de lemmes:

Soient E un espace topologique, R une relation d’équivalence dans E, A une partie de E, $R_A$ la relation d’équivalence induite sur A par R; soit enfin $f$ l’application canonique de E sur E/R. Avec ces notations:

*Lemme 1. — Si tout ensemble ouvert (resp. fermé) dans A et saturé pour $R_A$ est la trace sur A d’un ensemble ouvert (resp. fermé) dans E et saturé pour R, l’espace quotient $A/R_A$ est homéomorphe au sous-espace $f(A)$ de E/R. Il en est ainsi en particulier si A est ouvert ou fermé dans E et saturé pour R.*

Cela résulte de la prop. 10 de I, p. 23.

*Lemme 2. — S’il existe une application continue $g$ de E sur A, telle que, pour tout $x \in E$, $g(x)$ appartienne à la classe d’équivalence de $x$, l’espace $A/R_A$ est homéomorphe à E/R.*

Cela n’est autre que le cor. 2 de I, p. 23.

### 1. Topologie des espaces projectifs réels

Rappelons (A, II, p. 132) qu’étant donné un corps K et un entier $n \geq -1$, on appelle espace projectif à gauche à n dimensions sur le corps K et on note $\mathbf{P}_n(K)$ l’ensemble quotient de $K_{n+1}^*$ (complémentaire de $\{0\}$ dans l’espace vectoriel à gauche $K^{n+1}$) par la relation d’équivalence $\Delta_n(K)$ entre vecteurs $\mathbf{x}, \mathbf{y}$ de $K_{n+1}^*$: « il existe $t \in K$ tel que $t \neq 0$ et $\mathbf{y} = t \mathbf{x}$ ». Dans la théorie des espaces projectifs, on prend l’intervalle $(0, n)$ de $\mathbf{N}$ comme ensemble d’indices des coordonnées d’un point de $K_{n+1}^*$. Les coordonnées $x_i$ ($0 \leq i \leq n$) d’un quelconque des points de $K_{n+1}^*$ dont un point $\mathbf{x} \in \mathbf{P}_n(K)$ est l’image canonique, constituent ce qu’on appelle un système de coordonnées homogènes du point $\mathbf{x}$ (A, II, p. 133).

On appelle variété linéaire projective à p dimensions de $\mathbf{P}_n(K)$ (pour tout entier $p$ tel que $-1 \leq p \leq n$) l’image canonique dans $\mathbf{P}_n(K)$ d’un sous-espace vectoriel à $p + 1$ dimensions (privé de l’origine) de $K^{n+1}$. Un système de $p$ points de $\mathbf{P}_n(K)$ est dit libre s’il se compose des images canoniques de $p$ points de $K_{n+1}^*$ formant un système libre dans l’espace vectoriel $K^{n+1}$; la variété linéaire projective de $\mathbf{P}_n(K)$ engendrée par un système libre de $p + 1$ points (c’est-à-dire la plus petite variété linéaire projective contenant ces $p + 1$ points) a $p$ dimensions.

Lorsque K est le corps $\mathbf{R}$ des nombres réels, on peut munir les espaces projectifs correspondants de topologies dont nous allons faire l’étude.

#### Définition 1 {#top-vi-s3-def-1 .statement}

On appelle espace projectif réel à n dimensions l’espace projectif $\mathbf{P}_n(\mathbf{R})$ muni de la topologie quotient de celle de $\mathbf{R}_{n+1}^*$ par la relation d’équivalence $\Delta_n(\mathbf{R})$.

L’espace projectif $\mathbf{P}_1(\mathbf{R})$ s’appelle droite projective réelle, l’espace projectif $\mathbf{P}_2(\mathbf{R})$ plan projectif réel.

Lorsque aucune confusion ne sera possible, nous écrirons $\mathbf{P}_n$ et $\Delta_n$ au lieu de $\mathbf{P}_n(\mathbf{R})$ et $\Delta_n(\mathbf{R})$.

#### Proposition 1 {#top-vi-s3-prop-1 .statement}

L’espace projectif $\mathbf{P}_n$ est séparé.

Montrons d’abord que la relation $\Delta_n$ est ouverte (I, p. 31); soit A un ensemble ouvert dans $\mathbf{R}_{n+1}^*$; pour saturer A pour $\Delta_n$, il faut prendre la réunion des homothétiques $tA$ de A, $t$ parcourant l’ensemble des nombres réels $\neq 0$; chacun de ces ensembles étant ouvert, il en est de même de leur réunion.

D’après la prop. 8 de I, p. 55, la prop. 1 sera démontrée si on prouve que la partie M de $\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$, définie par la relation $\Delta_n$, est fermée. Or, soit $(\mathbf{x}, \mathbf{y})$ un point de $\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$ adhérent à M; si $\mathbf{x} = (x_i)$, il existe une coordonnée $x_i \neq 0$; il existe donc un voisinage V de $(\mathbf{x}, \mathbf{y})$ tel que pour tout point $(\mathbf{x}', \mathbf{y}') \in M \cap V$ la coordonnée $x'_i$ d’indice i de $\mathbf{x}'$ soit $\neq 0$; lorsque $(\mathbf{x}', \mathbf{y}')$ tend vers $(\mathbf{x}, \mathbf{y})$ en restant dans M, $y'_i {x'}^{-1}_i$ tend vers $t = y_i x^{-1}_i$; comme $\mathbf{y}' = (y'_i {x'}^{-1}_i) \mathbf{x}'$, on voit, en passant à la limite, que $\mathbf{y} = t \mathbf{x}$, ce qui prouve que $(\mathbf{x}, \mathbf{y}) \in M$.

#### Proposition 2 {#top-vi-s3-prop-2 .statement}

L’espace projectif $\mathbf{P}_n$ est un espace compact et connexe, homéomorphe à l’espace quotient de la sphère $\mathbf{S}_n$ par la relation d’équivalence induite sur cette sphère par $\Delta_n$.

Soit $\Delta'_n$ la relation d’équivalence induite sur $S_n$ par $\Delta_n$ (les classes d’équivalence pour $\Delta'_n$ sont les couples de points opposés de $S_n$). L’application $x \mapsto x / \|x\|$ de $\mathbf{R}_{n+1}^*$ sur $S_n$ est continue; donc (VI, p. 12, lemme 2) $P_n$ est homéomorphe à $S_n / \Delta'_n$. Comme, pour $n \neq 0$, $S_n$ est compact et connexe, tout espace quotient séparé de $S_n$ est aussi compact et connexe (cor. 1, I, p. 63, et I, p. 82, prop. 6). Enfin $P_0$ n’a qu’un point.

#### Proposition 3 {#top-vi-s3-prop-3 .statement}

*Pour $n \geqslant 0$, l’espace projectif $P_n$ est homéomorphe à l’espace quotient de la boule $B_n$ obtenu en identifiant chaque point de $S_{n-1}$ à son opposé.*

Soit $H$ l’hémisphère fermé de $S_n$ défini par $x_0 \leqslant 0$. L’espace $P_n$, homéomorphe au quotient de $S_n$ par la relation $\Delta''_n$ (prop. 2), est aussi homéomorphe au quotient de la partie $H$ de $S_n$ par la relation $\Delta''_n$ induite sur $H$ par $\Delta'_n$. En effet, toute classe suivant $\Delta'_n$ rencontre $H$ en un point au moins; il suffit alors (VI, p. 12, lemme 1) de vérifier que, si on sature pour $\Delta'_n$ un ensemble $U$ ouvert dans $H$ et saturé pour $\Delta''_n$, on obtient un ensemble $V$ ouvert dans $S_n$. Or, si $a = (a_i) \in U$ et si $a_0 < 0$, il existe un voisinage $W$ de $a$ dans $S_n$ contenu dans $U$; la réunion de $W$ et de $-W$ est un voisinage de $a$ saturé pour $\Delta'_n$ et contenu dans $V$. Si au contraire $a_0 = 0$, on $a - a \in U$, et il existe $r > 0$ tel que l’ensemble des points $x \in H$ satisfaisant à l’une ou l’autre des relations $\|x - a\| < r, \|x + a\| < r$, soit contenu dans $U$; l’ensemble des points $x \in S_n$ satisfaisant à l’une ou l’autre de ces relations est un voisinage de $a$ saturé pour $\Delta'_n$ et contenu dans $V$.

Observons que l’espace quotient $H / \Delta''_n$ s’obtient en identifiant, dans $H$, tout point de l’intersection $S_{n-1}$ de $H$ et de l’hyperplan $x_0 = 0$ avec son opposé. Pour achever la démonstration il suffit de remarquer que la projection stéréographique de point de vue $e_0$ (VI, p. 11) est un homéomorphisme de $H$ sur $B_n$, laissant invariants les points de $S_{n-1}$.

### 2. Variétés linéaires projectives

Rappelons (A, II, p. 136) que toute application linéaire injective $f$ de $\mathbf{R}^{n+1}$ dans $\mathbf{R}^{m+1}$ ($m \geqslant n$) définit, par restriction à $\mathbf{R}_{n+1}^*$, puis passage aux quotients pour les relations $\Delta_n$ et $\Delta_m$, une application injective $g$ de $P_n$ dans $P_m$, dite *application linéaire projective*. Si $\varphi$ est l’application canonique de $\mathbf{R}_{n+1}^*$ sur $P_n$, $\psi$ celle de $\mathbf{R}_{m+1}^*$ sur $P_m$, on a $g \circ \varphi = \psi \circ f$, ce qui prouve que $g$ est *continue* dans $P_n$ (I, p. 21, corollaire). En particulier, toute *transformation linéaire projective* de $P_n$ (application linéaire projective de $P_n$ sur lui-même) est un *homéomorphisme* de $P_n$ sur lui-même.

Soit $E$ un espace vectoriel de dimension $n + 1$ sur $\mathbf{R}$; à chaque base de $E$ sur $\mathbf{R}$ est associée une bijection $\mathbf{R}$-linéaire de $\mathbf{R}^{n+1}$ sur $E$, donc aussi une bijection de $P_n$ sur l’espace projectif $P(E)$ déduit de $E$ (A, II, p. 132); la topologie sur $P(E)$ transportée de celle de $P_n$ par cette bijection est indépendante de la base de $E$ choisie. C’est aussi la topologie quotient de la topologie induite sur $E - \{0\}$ par la topologie introduite sur $E$ dans VI, p. 6.

Rappelons aussi que, si $V$ et $V'$ sont deux variétés linéaires projectives à $p$ dimensions de $\mathbf{P}_n$, il existe une transformation linéaire projective de $\mathbf{P}_n$ transformant V en $V'$. En particulier, si $p \geqslant 0$, il existe une transformation linéaire projective transformant V en l’image canonique du sous-espace engendré par $e_0, e_1, \ldots, e_p$ $W'$ à $p + 1$ dimensions (privé du point 0) de $\mathbf{R}^{n+1}$. Si on identifie $W'$ à $\mathbf{R}_{p+1}^*$, la relation induite sur $W'$ par $\Delta_n$ n’est autre que $\Delta_p$; comme $W'$ est fermée et saturée pour $\Delta_n$, le lemme 1 (VI, p. 12) montre que $V'$ est homéomorphe à $\mathbf{P}_p$ et fermée dans $\mathbf{P}_n$; en outre, si $p < n$, son complémentaire dans $\mathbf{P}_n$ est dense (VI, p. 5, prop. 4). Donc:

#### Proposition 4 {#top-vi-s3-prop-4 .statement}

*Toute variété linéaire projective à p dimensions de l’espace projectif $\mathbf{P}_n$ est un ensemble fermé dans $\mathbf{P}_n$, homéomorphe à $\mathbf{P}_p$; si $p < n$, son complémentaire est dense dans $\mathbf{P}_n$.*

Rappelons que les variétés linéaires projectives à $n - 1$ dimensions de $\mathbf{P}_n$ ($n \geqslant 1$) sont appelées *hyperplans projectifs*; tout hyperplan projectif est l’ensemble des points dont les coordonnées homogènes satisfont à une relation de la forme
$$
\sum_{i=0}^n a_i x_i = 0,
$$
où les $a_i$ ne sont pas tous nuls (« équation » de l’hyperplan).

#### Proposition 5 {#top-vi-s3-prop-5 .statement}

*Dans l’espace projectif $\mathbf{P}_n$ (pour $n \geqslant 0$), le complémentaire d’un hyperplan projectif $H$ est homéomorphe à $\mathbf{R}^n$.*

Par une transformation linéaire projective, on se ramène au cas où $H$ est l’hyperplan d’équation $x_0 = 0$. L’ensemble A des points $x = (x_i)$ de $\mathbf{R}_{n+1}^*$ tels que $x_0 \neq 0$ est ouvert et saturé pour $\Delta_n$; son image canonique C dans $\mathbf{P}_n$, qui est le complémentaire de H dans $\mathbf{P}_n$, est par suite homéomorphe au quotient de A par la relation d’équivalence $\Theta$ induite sur A par $\Delta_n$ (VI, p. 12, lemme 1). Soit B l’hyperplan d’équation $x_0 = 1$ dans $\mathbf{R}^{n+1}$; à tout point $x \in A$, faisons correspondre le point $x_0^{-1} x$ où la droite passant par 0 et $x$ coupe B (fig. 4); on définit

![Figure 4](https://i.imgur.com/3Q5z5QG.png)

Figure 4

ainsi une application continue g de A sur B, telle que $g(x)$ soit le seul point de B congru à $x$ suivant $\Theta$; il en résulte que B est homéomorphe à $A/\Theta$ (VI, p. 12, lemme 2), donc à C; comme B est homéomorphe à $\mathbf{R}^n$, la proposition est démontrée.

#### Corollaire {#top-vi-s3-n2-cor-1 .statement}

Tout point de $\mathbf{P}_n$ possède un voisinage ouvert homéomorphe à $\mathbf{R}^n$.

On en conclut en particulier que les espaces projectifs réels sont localement connexes (ce qui résulte aussi de I, p. 85, prop. 12).

### 3. Immersion de l’espace numérique dans l’espace projectif

Supposons $n \geqslant 0$. Soit U le complémentaire dans $\mathbf{P}_n$ de l’hyperplan H d’équation $x_0 = 0$. On identifie souvent U à $\mathbf{R}^n$ par l’homéomorphisme qui applique le vecteur $\mathbf{x} = (x_i)$ de $\mathbf{R}^n$ sur le point de coordonnées homogènes $(1, x_1, \ldots, x_n)$; l’homéomorphisme réciproque applique le point de coordonnées homogènes $(x_0, \ldots, x_n)$ de U sur le vecteur $(x_1/x_0), \ldots, x_n/x_0)$ de $\mathbf{R}^n$. L’hyperplan H est alors appelé l’hyperplan à l’infini, les points de H étant appelés les « points à l’infini » de $\mathbf{P}_n$ (ou même de $\mathbf{R}^n$ par abus de langage).

Une fois faite cette identification, toute variété linéaire affine V à $p$ dimensions de $\mathbf{R}^n$ a pour adhérence dans $\mathbf{P}_n$ une variété linéaire projective à $p$ dimensions, non contenue dans l’hyperplan à l’infini, et identique à la variété linéaire projective engendrée par V. Réciproquement, toute variété linéaire projective à $p$ dimensions, non contenue dans l’hyperplan à l’infini, a pour trace sur $\mathbf{R}^n$ une variété linéaire affine à $p$ dimensions, dont elle est l’adhérence.

Dans le cas particulier où $n = 1$, l’hyperplan à l’infini est réduit à un point; comme $\mathbf{P}_1$ est compact, il résulte du th. d’Alexandroff (I, p. 67, th. 4) que $\mathbf{P}_1$ est homéomorphe à l’espace compact $\tilde{\mathbf{R}}$ obtenu à partir de l’espace localement compact $\mathbf{R}$ par adjonction d’un « point à l’infini ». D’après les cor. 1 de VI, p. 11 et 4 de VI, p. 12, on voit également que la droite projective réelle $\mathbf{P}_1(\mathbf{R})$ est homéomorphe au cercle $\mathbf{S}_1$ et au tore $\mathbf{T}$.

Au contraire, pour $n > 1$, $\mathbf{P}_n(\mathbf{R})$ n’est pas homéomorphe à $\mathbf{S}_n$ (cf. VI, p. 26, exerc. 4).

Le « point à l’infini » de l’espace $\tilde{\mathbf{R}}$ se note $\infty$, sans signe. Il importe de ne pas confondre l’espace $\tilde{\mathbf{R}}$, où est ainsi plongée la droite numérique, et la droite achevée $\overline{\mathbf{R}}$ définie dans IV, p. 13, qui possède deux « points à l’infini »; d’ailleurs $\tilde{\mathbf{R}}$ est homéomorphe à l’espace quotient de $\overline{\mathbf{R}}$ obtenu en identifiant les deux points $+\infty$ et $-\infty$.

### 4. Application au prolongement des fonctions numériques

Comme $\mathbf{R}$ peut être considéré comme une partie de $\tilde{\mathbf{R}}$, toute application d’un ensemble E dans $\mathbf{R}$ (fonction numérique) peut être considérée comme une application de E dans $\tilde{\mathbf{R}}$; en particulier, si E est une partie d’un espace topologique F, $f$ une application de E dans $\mathbf{R}$, il peut se faire qu’en certains points de l’adhérence $\overline{E}$ de E, $f(x)$ tende vers la limite $\infty$ lorsque $x$ tend vers un de ces points en restant dans E; on prolongera alors par continuité la fonction $f$ en lui donnant en ces points la valeur $\infty$ (I, p. 57, th. 1).

Considérons en particulier le cas où E est une partie de $\mathbf{R}^n$, l’espace $\mathbf{R}^n$ étant lui-même considéré comme plongé dans l’espace projectif $\mathbf{P}_n$; une fonction numérique $f$ définie dans E peut être identifiée à l’application qui associe à un point de E de coordonnées homogènes $x_0, x_1, \ldots, x_n$ l’élément

$$
f\left( \frac{x_1}{x_0}, \frac{x_2}{x_0}, \ldots, \frac{x_n}{x_0} \right)
$$

de $\tilde{\mathbf{R}}$; appliquant ce qui précède, on pourra éventuellement prolonger cette fonction par continuité, non seulement à certains des points de $\mathbf{R}^n$ adhérents à E, mais aussi à certains des « points à l’infini » de $\mathbf{P}_n$, adhérents à E.

Montrons qu’on retrouve ainsi, par exemple, le prolongement par continuité à $\tilde{\mathbf{R}}$ tout entier d’une fonction rationnelle d’une variable réelle, déjà défini en Algèbre (A, II, p. 136). Identifions $\tilde{\mathbf{R}}$ et $\mathbf{P}_1$, tout nombre réel $x \in \mathbf{R}$ étant identifié au point de coordonnées homogènes $(1, x)$, le point $\infty$ au point de coordonnées homogènes $(0, 1)$. Soit $u(x)/v(x)$ une fonction rationnelle, $u$ et $v$ étant deux polynômes premiers entre eux, de degrés respectifs $m$ et $n$; si l’on suppose par exemple $m \leq n$, et qu’on pose $u_1(x, y) = x^n u(y/x)$, $v_1(x, y) = x^n v(y/x)$, la fonction rationnelle $u/v$ est la restriction à l’ensemble des nombres réels n’annulant pas $v(x)$, de l’application $(x, y) \mapsto (v_1(x, y), u_1(x, y))$. En d’autres termes, on prolonge $u/v$ par continuité en lui donnant la valeur $\infty$ aux points $x \in \mathbf{R}$ où $v(x) = 0$, et en lui donnant au point $\infty$ la valeur $0$ si $m < n$, la valeur $\infty$ si $m > n$, la valeur du rapport des coefficients des termes de degré $n$ de $u$ et $v$ si $m = n$.

En particulier, la fonction $1/x$ se prolonge au point $0$ en y prenant la valeur $\infty$, au point $\infty$ en y prenant la valeur $0$; cette fonction est évidemment un homéomorphisme de $\tilde{\mathbf{R}}$ sur lui-même; il en est de même de la fonction homographique $(ax + b)/(cx + d)$ lorsque $ad - bc \neq 0$.

De même, pour $n$ entier $> 0$, la fonction $x^n$ se prolonge au point $\infty$ en y prenant la valeur $\infty$.

Par contre, on ne peut en général prolonger par continuité à l’espace $\mathbf{P}_1 \times \mathbf{P}_1$, ni à l’espace $\mathbf{P}_2$, une fonction rationnelle de deux variables réelles (cf. VI, p. 26, exerc. 5).

### 5. Espaces de variétés linéaires projectives

Étant donné un corps $K$, l’ensemble $\mathbf{P}_{n,p}(K)$ des variétés linéaires projectives de dimension $p \geq 0$ de l’espace projectif gauche $\mathbf{P}_n(K)$ est en correspondance biunivoque avec l’ensemble des sous-espaces vectoriels à $p + 1$ dimensions de l’espace vectoriel à gauche $K^{n+1}$. Désignons par $L_{n+1,p+1}(K)$ l’ensemble des systèmes libres $(\mathbf{x}_k)_{0 \leq k \leq p}$ de $p + 1$ vecteurs de $K^{n+1}$; l’ensemble $\mathbf{P}_{n,p}(K)$ est encore en correspondance biunivoque avec l’ensemble quotient de $L_{n+1,p+1}(K)$ par la relation d’équivalence $\Delta_{n,p}(K)$: « $(\mathbf{x}_k)$ et $(\mathbf{y}_k)$ engendrent le même sous-espace vectoriel à $p + 1$ dimensions de $K_s^{n+1}$ ». Nous identifierons $\mathbf{P}_{n,p}(K)$ avec cet ensemble quotient dans ce qui suit. D’autre part, si à tout système libre $(\mathbf{x}_k)$ de p + 1 vecteurs de $K^{n+1}$, on fait correspondre la matrice $X$ à $p + 1$ lignes et $n + 1$ colonnes dont $x_k$ est la ligne d’indice $k$ pour $0 \leq k \leq p$, on définit une correspondance biunivoque entre $L_{n+1, p+1}(K)$ et l’ensemble des matrices à $p + 1$ lignes et $n + 1$ colonnes et de rang $p + 1$; nous identifierons $L_{n+1, p+1}(K)$ avec cet ensemble de matrices; la relation $\Delta_{n, p}(K)$ entre deux matrices $X, Y$ est alors la suivante: « il existe une matrice carrée inversible $T$ d’ordre $p + 1$ telle que $Y = T.X$ ».

Nous allons supposer dans ce qui suit que $K$ est le corps $\mathbf{R}$, et nous omettrons l’indication du corps dans les notations précédentes. On peut définir sur $P_{n, p}$ une topologie par un procédé qui généralise la définition de la topologie des espaces projectifs réels. En effet, $L_{n+1, p+1}$ est contenu dans l’espace $M_{p+1, n+1}$ des matrices à $p + 1$ lignes et $n + 1$ colonnes, à éléments réels; nous munirons $L_{n+1, p+1}$ de la topologie induite par celle de cet espace de matrices (VI, p. 6).

#### Définition 2 {#top-vi-s3-def-2 .statement}

*On appelle espace des variétés linéaires projectives à $p \geq 0$ dimensions de l’espace projectif réel $P_n$, l’espace $P_{n, p}$ quotient de l’espace topologique $L_{n+1, p+1}$ par la relation d’équivalence $\Delta_{n, p}$.*

Soit $f : \mathbf{R}^{n+1} \to \mathbf{R}^{m+1}$ une application linéaire *injective* ($m \geq n \geq -1$). On en déduit une application projective $g$ de $P_n$ dans $P_m$ (VI, p. 14); si $V$ est une variété linéaire projective de dimension $p$ de $P_n$, $g(V)$ est une variété linéaire projective de dimension $p$ de $P_m$, et l’application $V \mapsto g(V)$ de $P_{n, p}$ dans $P_{m, p}$ ainsi définie est *continue*. En effet, elle se déduit par passage aux quotients d’une application continue $L_{n+1, p+1} \to L_{m+1, p+1}$.

En particulier, tout automorphisme $f \in \mathbf{GL}(n+1, \mathbf{R})$ induit un homéomorphisme de $P_{n, p}$ sur lui-même; comme on l’a déjà remarqué (VI, p. 15), l’opération de $\mathbf{GL}(n+1, \mathbf{R})$ sur $P_{n, p}$ ainsi définie est *transitive*.

#### Proposition 6 {#top-vi-s3-prop-6 .statement}

*Soit $V$ une variété linéaire projective de dimension $n - p - 1$ de $P_n$; la partie $U_V$ de $P_{n, p}$ formée des éléments dont l’intersection avec $V$ est vide, est un ouvert dense de $P_{n, p}$, homéomorphe à $\mathbf{R}^{(p+1)(n-p)}$.*

D’après ce qui précède, on peut supposer que $V$ est la variété linéaire projective définie par les équations $x_{n-p} = 0, \ldots, x_n = 0$. L’image réciproque de $U_V$ dans $L_{n+1, p+1}$ est l’ensemble des suites $(x_0, \ldots, x_p)$ d’éléments de $\mathbf{R}^{n+1}$ qui, avec $e_{p+1}, \ldots, e_n$, forment une base de $\mathbf{R}^{n+1}$, c’est-à-dire, vu les identifications faites, l’ensemble $U'$ des matrices $X$ à $p + 1$ lignes et $n + 1$ colonnes telles que la matrice carrée formée des $p + 1$ premières colonnes de $X$ soit inversible. D’après la prop. 2 de VI, p. 4, $U'$ est un ouvert dense de $L_{n+1, p+1}$, donc $U_V$ un ouvert dense de $P_{n, p}$ (lemme 1, p. 12). A toute matrice $X \in U'$, faisons correspondre la matrice carrée inversible $f(X)$ formée de ses $p + 1$ premières colonnes et la matrice $g(X) = f(X)^{-1}X$. Soit $A$ la partie de $U'$ formée des $X \in U'$ telles que $f(X) = I$; alors $A$ est homéomorphe à $\mathbf{R}^{(p+1)(n-p)}$, l’application $g : U' \to A$ est continue, et, pour $X \in U'$, $g(X)$ est l’unique élément de $A$ équalent à $X$ modulo $\Delta_{n,p}$. Appliquant le lemme 2, on en déduit que $U_V$ est homéomorphe à $A$, ce qui achève la démonstration.

#### Corollaire {#top-vi-s3-n5-cor-1 .statement}

*L’espace $P_{n,p}$ est un espace connexe et localement connexe, dont tout point possède un voisinage homéomorphe à $\mathbf{R}^{(p+1)(n-p)}$*.

Cela résulte de la proposition et du fait que les $U_V$ recouvrent $P_{n,p}$.

#### Proposition 7 {#top-vi-s3-prop-7 .statement}

*L’espace $P_{n,p}$ est compact*.

Montrons d’abord que $P_{n,p}$ est séparé. Soient $V_1$ et $V_2$ deux éléments de $P_{n,p}$; l’intersection de deux ouverts denses étant un ouvert dense, donc non vide, il résulte de la prop. 6 qu’il existe une sous-variété linéaire projective $V$ de $P_n$, de dimension $n - p - 1$, telle que $V \cap V_1 = \varnothing$, $V \cap V_2 = \varnothing$; il s’ensuit que $V_1$ et $V_2$ appartiennent toutes deux à l’ouvert $U_V$ de $P_{n,p}$. Comme $U_V$ est homéomorphe à un espace numérique, il est séparé, et il existe deux ouverts disjoints $U_1$ et $U_2$ de $U_V$, contenant $V_1$ et $V_2$ respectivement, et $P_{n,p}$ est séparé.

Pour démontrer que $P_{n,p}$ est compact, il suffit maintenant de construire un sous-espace compact de $L_{n+1,p+1}$ tel que toute classe d’équivalence suivant $\Delta_{n,p}$ rencontre ce sous-espace en un point au moins; $P_{n,p}$, image séparée de ce sous-espace par l’application canonique de $L_{n+1,p+1}$ sur $P_{n,p}$, sera compact (I, p. 62, th. 2).

Soit $V_{n+1,p+1}$ le sous-espace de $L_{n+1,p+1}$ dont les éléments sont les systèmes $(\mathbf{x}_k)$ de $p + 1$ vecteurs formant une *base euclidienne orthonormale* du sous-espace vectoriel qu’ils engendrent (A, IX, § 6, no 1), c’est-à-dire tels que $(\mathbf{x}_h \mid \mathbf{x}_k) = 0$ pour $h \neq k$, $(\mathbf{x}_h \mid \mathbf{x}_h) = 1$ pour $1 \leq h \leq p + 1$. On sait (A, IX, § 7, no 1) que tout sous-espace vectoriel à $p + 1$ dimensions de $\mathbf{R}^{n+1}$ admet une telle base; donc toute classe mod. $A_{n,p}$ rencontre $V_{n+1,p+1}$. D’autre part, les matrices $X = (x_{ij})$ de $V_{n+1,p+1}$ sont définies par les relations

$$
\sum_{j=0}^n x_{ij}^2 = 1 \quad \text{pour } 1 \leq i \leq p + 1
$$

$$
\sum_{j=0}^n x_{ij} x_{kj} = 0 \quad \text{pour } i \neq k.
$$

Elles forment donc un ensemble *fermé* dans $M_{p+1,n+1}$, et comme on tire de ces relations que $|x_{ij}| \leq 1$ pour tout couple d’indices $(i,j)$, cet ensemble est *borné*, donc *compact*.

### 6. Grassmanniennes

Rappelons (A, III, p. 172) qu’on définit une application injective de $P_{n,p}$ dans $\mathbf{P}(\Lambda^{p+1}(\mathbf{R}^{n+1}))$ de la manière suivante: si $V \in P_{n,p}$ est l’image du système libre $(\mathbf{x}_0, \ldots, \mathbf{x}_p)$ de $\mathbf{R}^{n+1}$, on lui associe l’image canonique dans $\mathbf{P}(\Lambda^{p+1}(\mathbf{R}^{n+1}))$ du $(p+1)$-vecteur $\mathbf{x}_0 \wedge \cdots \wedge \mathbf{x}_p$. L’image de cette application est notée $G_{n+1,p+1}$ et appelée *grassmannienne* d’indices $n+1, p+1$; on la munit de la topologie induite par celle de $\mathbf{P}(\Lambda^{p+1}(\mathbf{R}^{n+1}))$ (VI, p. 13). L’application définie ci-dessus de $\mathbf{P}_{n,p}$ dans $\mathbf{G}_{n+1,p+1}$ est continue et bijective; comme $\mathbf{P}_{n,p}$ est compact et $\mathbf{G}_{n-1,p+1}$ séparé, on déduit alors de I, p. 63, cor. 2 au th. 2:

#### Proposition 8 {#top-vi-s3-prop-8 .statement}

*La grassmannienne* $\mathbf{G}_{n+1,p+1}$ *est homéomorphe à l’espace* $\mathbf{P}_{n,p}$.

Notons enfin (*loc. cit.*) que les grassmanniennes $\mathbf{G}_{n+1,p+1}$ et $\mathbf{G}_{n+1,n-p}$ se déduisent l’une de l’autre par une application projective bijective de $\mathbf{P}(\Lambda^{p+1}(\mathbf{R}^{n+1}))$ sur $\mathbf{P}(\Lambda^{n-p}(\mathbf{R}^{n+1}))$, donc sont *homéomorphes*, ainsi par conséquent que les espaces $\mathbf{P}_{n,p}$ et $\mathbf{P}_{n,n-p-1}$.

Exercises

## EXERCICES {#top-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
