---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 6
section_title: Espaces classifiants
lang: fr
source: ta-i-iv-fr
book_pages: A IV.437-A IV.480
pdf_pages: 0453-0496
extraction: native
subsections:
    - "no": 1
      title: Prolongement des homotopies
      page: 437
      pdf_page: 453
    - "no": 2
      title: Espaces fibrés localement triviaux de base $B\times \mathbf{I}$
      page: 440
      pdf_page: 456
    - "no": 3
      title: Espaces fibrés principaux de base $B\times \mathbf{I}$
      page: 443
      pdf_page: 459
    - "no": 4
      title: Espaces fibrés universels
      page: 446
      pdf_page: 462
    - "no": 5
      title: Espace classifiant pour un groupe discret
      page: 449
      pdf_page: 465
statements: 32
exercises: 0
content_sha256: 3b307db5f56f78fbd3358c684b32354dac47a42c80020e9f4ec7d0750f1f841e
---

## § 6. ESPACES CLASSIFIANTS

### 1. Prolongement des homotopies

#### Proposition 1 {#ta-iv-s6-prop-1 .statement tag=023V}

Soit $X'$ un espace topologique normal, soit X un sous-espace de $X'$, soit A un sous-espace fermé de $X'$ contenu dans X et soit U un voisinage de A dans X.

Notons $i_A$ l’injection canonique de A dans X$,i_U$ l’injection canonique de U dans X ; notons $j_A$ et $j_U$ les injections correspondantes de Cyl($i_A$) et Cyl($i_U$) dans $X\times \mathbf{I}$.

Il existe une application continue $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) telle que $j_U\circ$ $r(x) =x$ pour tout point $x\in j_A$(Cyl($i_A$)).

Soit $U'$ un ouvert de $X'$ tel que $A\subset X\cap U'\subset U$. Par définition d’un espace normal (TG, IX, p. 41), il existe un voisinage ouvert $V'$ de A dans $X'$ tel que $A\subset V'\subset V'\subset U'$ et une fonction continue $\varphi ': X'\rightarrow \mathbf{I}$ qui soit égale à 1 en tout point de A et à 0 en tout point de $\complement V'$. Posons $\varphi =\varphi '|X$ et $V = X\cap V'$. Notons aussi $\alpha : U\times \mathbf{I}\rightarrow$ Cyl($i_U$) et $\beta : X\rightarrow$ Cyl($i_U$) les applications canoniques (III, p. 238).

Soit $r$ l’application de $X\times \mathbf{I}$ dans Cyl($i_U$) donnée par

$\alpha (x,1-(1-t)\varphi (x))$ pour $(x, t)\in U\times \mathbf{I}$,

$$
r(x, t) =
$$

$\beta (x)$ sinon.

L’application $r$ est continue sur $U\times \mathbf{I}$. Pour tout point $(x, t)\in U\times \mathbf{I}$ tel que $x\notin V$, on a $\varphi (x) = 0$, d’où $r(x, t) =\alpha (x,1) =\beta (x)$. Par suite, les applications $r$ et $\beta \circ$ pr$_1$ coïncident sur $(X-V)\times \mathbf{I}$, ce qui entraîne que $r$ est continue sur ce sous-espace. Comme U et l’intérieur de X-V recouvrent X, l’application $r$ est continue.

Soit $y$ un point de Cyl($i_A$) ; posons $(x, t) =j_A(y)$. Si $x\in$ A, $\varphi (x) = 1$ et $r(x, t) =\alpha (x, t)$, d’où $j_U(r(x, t)) = (x, t)$. Sinon, $t= 1$ et l’on a $r(x, t) =\alpha (x,1)$ si $x\in U$ et $r(x, t) =\beta (x)$ sinon ; par suite, $j_U(r(x, t)) = (x, t)$ dans ce cas. Cela entraîne que $j_U\circ r$ applique tout point de $j_A$(Cyl($i_A$)) sur lui-même, d’où la proposition.

#### Corollaire 1 {#ta-iv-s6-prop-1-cor-1 .statement tag=023W}

Soit X un espace topologique normal, soit $f$ une application continue de X dans un espace topologique Z. Soit A un sous-espace fermé de X, soit U un voisinage de A dans X et soit $\sigma : U\times$ $\mathbf{I}\rightarrow Z$ une homotopie dont le terme est l’application $f|U$. Il existe une homotopie $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ dont le terme est l’application $f$ et qui coïncide avec $\sigma$ dans $A\times \mathbf{I}$.

Posons $X'= X$ et soit $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) l’application continue donnée par la prop. 1. Avec les notations introduites dans la démonstration de cette proposition, il existe une unique application continue F: Cyl($i_U$)$\rightarrow Z$ telle que $F(\alpha (x, t)) =\sigma (x, t)$ pour $(x, t)\in U\times \mathbf{I}$ et $F(\beta (x)) =f(x)$ pour $x\in$ X (III, p. 238, prop. 4). L’application $F\circ r: X\times \mathbf{I}\rightarrow$ Z est une homotopie ; son terme applique un point $x\in$ X sur $F(r(x,1)) = F(\beta (x)) =f(x)$. Si $(x, t)\in A\times \mathbf{I}$, $F(r(x, t)) = F(\alpha (x, t)) =\sigma (x, t)$, donc cette homotopie coïncide avec $\sigma$ sur $A\times \mathbf{I}$.

#### Corollaire 2 {#ta-iv-s6-prop-1-cor-2 .statement tag=023X}

Soit X un espace topologique normal, soit A un sous-espace fermé de X et soit U un voisinage de A dans X. Soient $f$ et $f'$ des applications continues homotopes de U dans un espace topologique Z. Si $f$ possède un prolongement continu à X, il en est de même de l’application $f'|A$.

Soit F une application continue de X dans Z telle que $F|U =f$. Choisissons une homotopie $\sigma : A\times \mathbf{I}\rightarrow Z$ reliant $f'$ à $f$. D’après le cor. 1, il existe une homotopie $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ de terme F qui prolonge $\sigma$. L’origine de $\widetilde{\sigma}$ est alors une application continue de X dans Z qui coïncide avec $f'$ sur A.

#### Corollaire 3 {#ta-iv-s6-prop-1-cor-3 .statement tag=023Y}

Soit X un espace topologique normal, soit A un sous-espace fermé de X et soit U un voisinage de A dans X. Soit Z un espace topologique homéotope à un point et soit $g: U\rightarrow$ Z une application continue. Il existe une application continue $\widetilde{g}: X\rightarrow Z$ qui coïncide avec $g$ sur A.

Puisque Z est homéotope à un point, l’application $g$ est homéotope à une application constante $f$. L’application $f$ se prolonge continûment à X ; l’assertion résulte donc du cor. 2.

#### Corollaire 4 {#ta-iv-s6-prop-1-cor-4 .statement tag=023Z}

Soit X un espace topologique paracompact, soit A un sous-espace fermé de X. Soit $n$ un entier $\geqslant 0$ et soit V un ouvert de $\mathbf{R}^n$. Soit $f: X\rightarrow V$ une application continue et soit $\sigma : A\times \mathbf{I}\rightarrow V$ une homotopie de terme $f|A$. Il existe une homotopie $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ de terme $f$ qui prolonge $\sigma$.

Notons $i_A$ l’injection canonique de A dans X$,\alpha_A: A\times \mathbf{I}\rightarrow$ Cyl($i_A$) et $\beta_A: X\rightarrow$ Cyl($i_A$) les applications canoniques ainsi que $j_A:$ Cyl($i_A$)$\rightarrow$ $X\times \mathbf{I}$ l’injection canonique. Comme A est fermé dans X$,j_A$ définit un homéomorphisme de Cyl($i_A$) sur le sous-espace fermé $(A\times \mathbf{I})\cup (X\times \{1\})$ de $X\times \mathbf{I}$. Soit $\widetilde{\sigma}_0$ l’unique application de Cyl($i_A$) dans V telle que $\widetilde{\sigma}_0\circ \alpha_A=\sigma$ et $\widetilde{\sigma}_0\circ \beta_A=f$; elle est continue (III, p. 238, prop. 4).

Comme X est paracompact et que $\mathbf{I}$ est compact, l’espace $X\times \mathbf{I}$ est paracompact (TG, I, p. 70, prop. 17), donc normal (TG, IX, p. 49, prop. 4). Il existe donc une application continue $k: X\times \mathbf{I}\rightarrow \mathbf{R}^n$ telle que $k\circ j_A=\widetilde{\sigma}_0$ (TG, IX, p. 45, corollaire).

L’ensemble U des points $x\in$ X tels que $k(x, t)\in$ V pour tout $t\in \mathbf{I}$ est ouvert dans X (IV, p. 439, lemme 1). C’est donc un voisinage de A. D’après le corollaire 1, appliqué à l’application $f$ et à l’homotopie $k|U\times \mathbf{I}$, il existe une homotopie $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ d’origine $f$ qui coïncide avec $k$, donc avec $\sigma$, sur $A\times \mathbf{I}$.

#### Lemme 1 {#ta-iv-s6-lem-1 .statement tag=0240}

Soient Z un espace topologique, K un espace topologique compact et W une partie ouverte de $Z\times K$. L’ensemble U des points $z\in Z$ tels que $\{z\} \times K$ soit contenu dans W est ouvert dans Z.

La première projection pr$_1: Z\times K\rightarrow Z$ est propre (TG, I, p. 77, cor. 5), donc fermée. Par suite, $\complement U =$ pr$_1(\complement W)$ est fermé dans Z et U est ouvert.

#### Corollaire 5 {#ta-iv-s6-lem-1-cor-5 .statement tag=0241}

Soit $X'$ un espace topologique normal, soit X un sous-espace de $X'$, soit A un sous-espace fermé de $X'$ contenu dans X et soit U un voisinage de A dans X.

Soient Y et Z des espaces topologiques ; soit $f: X\times  \{1\} \times Y\rightarrow$ $X\times  \{1\} \times Z$ un $X\times  \{1\}$-morphisme et soit $g: U\times \mathbf{I}\times Y\rightarrow U\times \mathbf{I}\times Z$ un $U\times \mathbf{I}$-morphisme qui coïncide avec $f$ sur $U\times  \{1\} \times Y$.

Il existe alors un $X\times \mathbf{I}$-morphisme $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ qui coïncide avec $f$ sur $X\times  \{1\} \times Y$ et avec $g$ sur $A\times \mathbf{I}\times Y$.

En outre, si $f$ et $g$ sont des homéomorphismes, on peut choisir un homéomorphisme $h$ ayant les propriétés requises.

Soit $U'$ un voisinage ouvert de A dans $X'$ tel que $U'\cap X\subset U$. Comme l’espace $X'$ est normal, il existe un voisinage ouvert $V'$ de A dans $X'$ tel que $A\subset V'\subset V'\subset U'$ (TG, IX, p. 41). Quitte à remplacer U par $V'\cap X$, on peut ainsi supposer que U est fermé dans X. Reprenons alors les notations de la prop. 1 et de sa démonstration ; soit $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) une application continue telle que $j_U\circ r(x) =x$ pour tout point $x\in j_A$(Cyl($i_A$)).

Posons aussi $f'=$ pr$_3\circ f$ et $g'=$ pr$_3\circ g$. Comme $f'$ et $g'$ coïncident sur $U\times  \{1\} \times Y$, il existe une unique application

$\varphi :$ Cyl($i_U$)$\times Y\rightarrow$ Cyl($i_U$)$\times Z$

telle que $\varphi (\alpha (x, t), y) = (\alpha (x, t), g'(x, t, y))$ pour $(x, t, y)\in U\times \mathbf{I}\times Y$ et $\varphi (\beta (x), y) = (\beta (x), f'(x,1, y))$ pour $(x, y)\in X\times Y$. Comme U est fermé dans X, la surjection canonique $\pi$ de $(U\times \mathbf{I})\cup X$ dans Cyl($i_U$) est universellement stricte (III, p. 239, remarque 2). Comme l’application $\varphi \circ (\pi \times$ Id$_Y)$ est continue, l’application $\varphi$ est continue. C’est donc un morphisme de Cyl($i_U$)-espaces, et même un isomorphisme si $f$ et $g$ sont des homéomorphismes.

Soit alors $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ l’application $r^*(\varphi )$ déduite de $\varphi$ par le changement de base $r$. Elle est donnée par $h(x, t, y) =$ $(x, t$, pr$_2(\varphi (r(x, t), y)))$ pour $(x, t, y)\in X\times \mathbf{I}\times Y$. C’est un morphisme de $X\times \mathbf{I}$-espaces, et même un isomorphisme si $\varphi$ l’est. Pour $(x, t, y)\in$ $A\times \mathbf{I}\times Y$, on a $r(x, t) = (x, t)$, d’où

$h(x, t, y) = (x, t$, pr$_2(\varphi (x, t, y))) = (x, t, g'(x, t, y)) =g(x, t, y)$,

ce qui démontre que $h$ coïncide avec $g$ sur $A\times \mathbf{I}\times Y$. De même, pour $x\in X$ et $y\in Y$, on a $r(x,1) = (x,1)$, donc

$h(x,1, y) = (x,1$, pr$_2(\varphi (x,1, y))) = (x,1, f'(x,1, y)) =f(x,1, y)$

si bien que $h$ coïncide avec $f$ sur $X\times  \{1\} \times Y$. Le corollaire est ainsi démontré.

### 2. Espaces fibrés localement triviaux de base $B\times \mathbf{I}$

#### Proposition 2 {#ta-iv-s6-prop-2 .statement tag=0242}

Soit B un espace topologique paracompact et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré localement trivial. Posons $E_1=^-p^1(B\times \{1\})$ et notons $p_1: E_1\rightarrow B$ l’application pr$_1\circ p|E_1$. Alors, les $B\times \mathbf{I}$-espaces $(E, p)$ et $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ sont isomorphes.

Démontrons d’abord deux lemmes.

#### Lemme 2 {#ta-iv-s6-lem-2 .statement tag=0243}

Soient $\alpha ,\beta ,\gamma$ des nombres réels tels que $\alpha \leqslant \beta \leqslant \gamma$, soit B un espace topologique et soit $p: E\rightarrow B\times [\alpha , \gamma ]$ une application continue. Posons $B_0= B\times [\alpha , \beta ]$, $B_1= B\times [\beta , \gamma ]$, $E_0=^-p^1(B_0)$, $E_1=$ $^-p^1(B_1)$ et notons $p_0: E_0\rightarrow B_0,p_1: E_1\rightarrow B_1$ les applications déduites de $p$. Si $(E_0, p_0)$ et $(E_1, p_1)$ sont des espaces fibrés trivialisables, il en est de même de $(E, p)$.

Soient $g_0: E_0\rightarrow B_0\times F_0$ et $g_1: E_1\rightarrow B_1\times F_1$ des trivialisations de $E_0$ et $E_1$ respectivement. Notons $g'_0$ et $g_1'$ les trivialisations du $B\times  \{\beta \}$-espace fibré $^-p^1(B\times  \{\beta \})$ déduites de $g_0$ et $g_1$ par restriction. L’application $h=g_0'\circ (g_1')^{-1}$ est un $B\times  \{\beta \}$-isomorphisme de $B\times  \{\beta \} \times F_1$ sur $B\times  \{\beta \} \times F_0$. On définit une application continue $h'$ de $B\times F_1$ dans $F_0$ en posant $h'(a, y) =$ pr$_3\circ h(a, \beta , y)$ pour $(a, y)\in B\times F_1$. Pour $(a, t, y)\in B\times [\beta , \gamma ]\times F_1$, posons $H(a, t, y) = (a, t, h'(a, y))$. L’application H ainsi définie est un $(B\times [\beta , \gamma ])$-isomorphisme de $B\times [\beta , \gamma ]\times F_1$ sur $B\times [\beta , \gamma ]\times F_0$, et l’on a $g_0|^-p^1(B\times  \{\beta \}) = H\circ g_1|^-p^1(B\times  \{\beta \})$. Il existe donc une application continue $g: E\rightarrow B\times [\alpha , \gamma ]\times F_0$ telle que $g|E_0=g_0$ et $g|E_1= H\circ g_1$. L’application $g$ est un isomorphisme de $B\times [\alpha , \gamma ]$-espaces, donc E est trivialisable.

#### Lemme 3 {#ta-iv-s6-lem-3 .statement tag=0244}

Soit B un espace topologique et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré localement trivial. Tout point $a$ de B possède un voisinage V tel que le $V\times \mathbf{I}$-espace $E_{V\times\mathbf{I}}$ soit trivialisable.

Soit $a$ un point de B; pour tout point $t$ de $\mathbf{I}$, il existe un voisinage ouvert $W_t$ de $t$ dans $\mathbf{I}$ et un voisinage $V_t$ de $a$ dans B tels que E soit trivialisable au-dessus de $V_t\times W_t$. Il existe alors un entier $n >0$ et, pour tout entier $i$ tel que 1 $\leqslant i\leqslant n$, un point $t_i$ de $\mathbf{I}$ tel que l’intervalle $[^{i-1}_n,_n^i]$ soit contenu dans $W_{t_i}($III, p. 272, lemme 4). Posons $V =\cap_{1\leqslant i\leqslant n}V_{t_i}$. L’espace fibré E est trivialisable au-dessus de $V\times$ $[^{i-1}_n,_n^i]$ pour tout entier $i$ tel que $1\leqslant i\leqslant n$. Le lemme 3 résulte alors du lemme 2 par récurrence sur $n$.

Démontrons maintenant la proposition. D’après le lemme 3, il existe un recouvrement ouvert $(U_j)_{j\in J}$ de B tel que, pour tout $j\in J$, E soit trivialisable au-dessus de $U_j\times \mathbf{I}$. Comme l’espace B est paracompact, on peut supposer le recouvrement $(U_j)_{j\in J}$ localement fini (TG, IX, p. 49) et choisir un recouvrement $(A_j)_{j\in J}$ de B où, pour tout $j\in J$, l’ensemble $A_j$ est fermé dans B et contenu dans $U_j$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1).

Pour toute partie ouverte U de B, notons $\mathscr{F}(U)$ l’ensemble des $U\times \mathbf{I}$-isomorphismes de $^-p^1(U\times \mathbf{I})$ sur $^-p_1^1(U)\times \mathbf{I}$ qui induisent l’application identique de $^-p^1(U\times  \{1\})$ sur $^-p_1^1(U)\times  \{1\}$. Pour tout couple $(V,U)$ d’ouverts de B tels que $U\subset V$, notons $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ l’application qui, à un $(V\times \mathbf{I})$-isomorphisme $g:^-p^1(V\times \mathbf{I})\rightarrow^-p_0^1(V)\times \mathbf{I}$, associe le $(U\times \mathbf{I})$-isomorphisme déduit de $g$ par passage aux sous-espaces. Le couple $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ est un faisceau sur B (I, p. 45, exemple 4). Pour démontrer la proposition, il suffit de démontrer que le faisceau $\mathscr{F}$ est mou (I, p. 64).

Soit $j\in J$, soit A une partie fermée de $A_j$, soit V un ensemble ouvert dans B tel que $A\subset V\subset U_j$ et soit $g$ un élément de $\mathscr{F}(V)$. Il existe un voisinage ouvert W de A tel que $W\subset V$, car un espace paracompact est normal (TG, IX, p. 49, prop. 4). Nous allons démontrer qu’il existe un élément $g'$ de $\mathscr{F}(U_j)$ tel que $g'|W =g|W$. Le corollaire 2 (I, p. 65) de la prop. 6 entraîne alors que le faisceau $\mathscr{F}$ est mou.

Comme le $B\times \mathbf{I}$-espace E est trivialisable au-dessus de $U_j\times \mathbf{I}$, nous pouvons supposer que $^-p^1(U_j\times \mathbf{I}) = U_j\times \mathbf{I}\times F$, où F est un espace topologique. L’élément $g$ de $\mathscr{F}(V)$ est alors un $V\times \mathbf{I}$-isomorphisme de $V\times \mathbf{I}\times F$ sur lui-même qui induit l’application identique de $V\times$ $\{1\}\times F$. Appliquons le cor. 5 de IV, p. 439, aux espaces $X'= X$, $X = U_j$, A = W, U = V, et Y = Z = F, à l’application $g: V\times \mathbf{I}\times F\rightarrow V\times \mathbf{I}\times F$ et à l’application identique de $U_j\times  \{1\} \times F$. Il existe donc un $U_j\times \mathbf{I}$-isomorphisme $g'$ de $U_j\times \mathbf{I}\times F$ sur lui-même qui induit l’application identique de $U_j\times  \{1\} \times F$ et qui coïncide avec $g$ sur $W\times \mathbf{I}\times F$, et a fortiori sur $W\times \mathbf{I}\times F$. D’où la proposition.

#### Corollaire 1 {#ta-iv-s6-lem-3-cor-1 .statement tag=0245}

Soit B un espace topologique paracompact et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré localement trivial (I, p. 71, corollaire 2). Pour $t\in \mathbf{I}$, notons $(E_t, p_t)$ le B-espace fibré localement trivial $i^*_tE$, où $i_t: B\rightarrow B\times  \{t\}$ est l’application $b\mapsto (b, t)$. Les B-espaces fibrés localement triviaux $E_0$ et $E_t$ sont isomorphes pour tout $t\in \mathbf{I}$.

#### Corollaire 2 {#ta-iv-s6-lem-3-cor-2 .statement tag=0246}

Soient B et $B'$ des espaces topologiques, soit E un B-espace fibré localement trivial. Soient $f_0$ et $f_1$ des applications continues de $B'$ dans B. Supposons que l’espace $B'$ soit paracompact. Si les applications $f_0$ et $f_1$ sont homotopes, les $B'$-espaces fibrés localement triviaux $f_0^*E$ et $f_1^*E$ sont isomorphes.

Soit $\sigma : B'\times \mathbf{I}\rightarrow B$ une homotopie reliant $f_0$ à $f_1$ et notons $E'$ le $B'\times \mathbf{I}$-espace $\sigma^*E$ ; c’est un espace fibré localement trivial. Notons $i_0$ et $i_1$ les applications de $B'$ dans $B'\times \mathbf{I}$ données par $x\mapsto (x,0)$ et $x\mapsto (x,1)$. D’après le cor. 1, les $B'$-espaces fibrés $i^*_0E'$ et $i^*_1E'$ sont isomorphes. Comme $\sigma \circ i_0=f_0$, le $B'$-espace $i^*_0E'$ s’identifie à $f_0^*E$ ; de même, le $B'$-espace $i^*_1E'$ s’identifie à $f_1^*E$. Par suite, les $B'$-espaces fibrés $f_0^*E$ et $f_1^*E$ sont isomorphes, ce qu’il fallait démontrer.

#### Corollaire 3 {#ta-iv-s6-lem-3-cor-3 .statement tag=0247}

Soit B un espace topologique paracompact. Si B est homéotope à un point, tout espace fibré localement trivial de base B est trivialisable.

#### Corollaire 4 {#ta-iv-s6-lem-3-cor-4 .statement tag=0248}

Soient B et $B'$ des espaces topologiques, soit $(E, p)$ un B-espace fibré localement trivial, soit $f$ une application continue de $B'$ dans B, soit $\sigma : B'\times \mathbf{I}\rightarrow B$ une homotopie d’origine $f$ et soit $\widetilde{f}$ un relèvement continu de $f$ à E. Si l’espace $B'$ est paracompact, il existe une homotopie $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow E$ d’origine $\widetilde{f}$ qui est un relèvement de $\sigma$ à E.

Soit $(E', p')$ le $B'\times \mathbf{I}$-espace déduit de $(E, p)$ par changement de base par l’application $\sigma : B'\times \mathbf{I}\rightarrow B$. C’est un espace fibré localement trivial (I, p. 71, cor. 2) et l’application $s: B'\times  \{0\} \rightarrow E'$ définie par $s((a,0)) = ((a,0),\widetilde{f}(a))$ pour $a\in B'$ est une section continue de $p'$ au-dessus de $B'\times  \{0\}$. D’après la prop. 2, il existe une section continue $\widetilde{s}$ de $p'$ qui prolonge $s$. L’application $\widetilde{\sigma}=$ pr$_2\circ \widetilde{s}$ a la propriété requise.

### 3. Espaces fibrés principaux de base $B\times \mathbf{I}$

Soit G un groupe topologique. Nous allons voir que la proposition 2 et ses corollaires restent valables lorsqu’on remplace, dans chaque énoncé, « espace fibré localement trivial » par « espace fibré principal de groupe G ».

#### Lemme 4 {#ta-iv-s6-lem-4 .statement tag=0249}

Soit B un espace topologique, soit G un groupe topologique et soient E, $E'$ des espaces fibrés principaux de groupe G et de base B. Notons F l’espace topologique G muni de l’opération à gauche de $G\times G$ donnée par $(g, g')\cdot f=g'f g^{-1}$ et notons $M = (E\times_BE')\times^{G\times G}F$ l’espace fibré localement trivial de fibre-type F et de base B associé.

Le faisceau $\mathscr{S}$ sur B des sections de M est isomorphe au faisceau sur B des isomorphismes d’espaces fibrés principaux de E dans $E'$.

Notons $p,p'$ et $q$ les projections des B-espaces E, $E'$ et M. Pour $(x, x')\in E\times_BE'$ et $f\in F$, notons $[x, x', f]$ la classe dans M de l’élément $((x, x'), f)\in (E\times_BE')\times F$. Notons $\mathscr{M}$ le faisceau sur B des isomorphismes d’espaces fibrés principaux de E dans $E'$; ses sections au-dessus d’un ouvert U de B sont les isomorphismes d’espaces fibrés principaux de $E_U$ dans $E'_U$.

Notons $e$ l’élément neutre de G. Soit U un ouvert de B et soit $\varphi : E_U\rightarrow E'_U$ un isomorphisme d’espaces fibrés principaux de groupe G et de base U. L’application de $E_U$ dans $(E\times_BE')\times^{G\times G}F$ définie par $x\mapsto [x, \varphi (x), e]$ est continue. Pour $g\in G$ et $x\in E_U$, elle applique $x\cdot g$ sur $[x\cdot g, \varphi (x\cdot g), e] = [x, \varphi (x), geg^{-1}] = [x, \varphi (x), e]$. Il existe donc une unique application continue $\alpha_U(\varphi ): U\rightarrow M$ telle que $\alpha_U(\varphi )(p(x)) = [x, \varphi (x), e]$ pour tout $x\in E_U$; on a $\alpha_U(\varphi )\in \mathscr{S}(U)$.

Il est immédiat que les applications $\alpha_U$ définissent un morphisme de faisceaux $\alpha$ de $\mathscr{M}$ dans $\mathscr{S}$.

#### Lemme 5 {#ta-iv-s6-lem-5 .statement tag=024A}

Le morphisme de faisceaux $\alpha$ est un isomorphisme.

Supposons tout d’abord que les espaces fibrés principaux E et $E'$ soient tous deux trivialisables ; choisissons-en des sections $i: B\rightarrow E$ et $i': B\rightarrow E'$. Il existe alors une unique application continue $\theta$ de M dans $B\times G$ telle que l’on ait

$$
\theta ([i(b)\cdot g, i'(b)\cdot g', f]) = (b, g'f g^{-1})
$$

pour $b\in B,g\in G,g'\in G$ et $f\in$ F; c’est un isomorphisme de B-espaces. Soit $\varphi$ un isomorphisme d’espaces fibrés principaux de E dans $E'$; il existe une unique application continue $\gamma : B\rightarrow G$ telle que $\varphi (i(b)) =i'(b)\cdot \gamma (b)$ pour $b\in B$. L’image de $\varphi$ par l’application $\alpha_B$ est l’application $b\mapsto \theta^{-1}(b, \gamma (b))$ de B dans M. Ceci entraîne que $\alpha_B$ est une bijection.

Par conséquent, $\alpha_U$ est une bijection pour tout ouvert U de B tel que les espaces fibrés principaux $E_U$ et $E'_U$ soient trivialisables. D’après le corollaire 2 de I, p. 55, cela entraîne que $\alpha$ est un isomorphisme de faisceaux.

#### Proposition 3 {#ta-iv-s6-prop-3 .statement tag=024B}

Soit G un groupe topologique, soit B un espace topologique paracompact et soit $(E, p)$ un espace fibré principal de groupe G et de base $B\times \mathbf{I}$. Posons $E_1=^-p^1(B\times \{1\})$ et soit $p_1: E_0\rightarrow B$ l’application pr$_1\circ p|E_1$. Alors, $(E, p)$ et $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ sont des espaces fibrés principaux de groupe G et de base $B\times \mathbf{I}$ isomorphes.

Soit F l’espace topologique G muni de l’opération à gauche du groupe $G\times G$ donnée par $(g, g')\cdot f=g'f g^{-1}$. Soit $(M, q)$ l’espace fibré localement trivial de base $B\times \mathbf{I}$ et de fibre-type F associé à l’espace fibré principal $E\times_{B\times\mathbf{I}}(E_1\times \mathbf{I})$ de groupe $G\times G$. Posons $M_1=^-q^1(B\times \{1\})$ et $q_1=$ pr$_1\circ p|M_1$; le B-espace $(M_1, q_1)$ s’identifie à l’espace fibré localement trivial de fibre-type F associé à $E_1\times_BE_1$. D’après le lemme 4, où l’on prend pour espaces fibrés principaux E et $E'$ égaux à $E_1$, le B-espace $M_1$ possède une section. Comme les $B\times \mathbf{I}$-espaces $(M, q)$ et $(M_1\times \mathbf{I}, q_1\times$Id$_{\mathbf{I}})$ sont isomorphes (IV, p. 440, prop. 2), le $B\times \mathbf{I}$-espace $(M, q)$ possède une section, ce qui entraîne que les espaces fibrés principaux de groupe G, E et $E_1\times \mathbf{I}$, sont isomorphes.

#### Corollaire 1 {#ta-iv-s6-prop-3-cor-1 .statement tag=024C}

Soit B un espace topologique paracompact, soit G un groupe topologique et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré principal de groupe G. Pour $t\in \mathbf{I}$, notons $(E_t, p_t)$ le B-espace fibré principal $i^*_tE$, où $i_t: B\rightarrow B\times  \{t\}$ est l’application $b\mapsto (b, t)$. Les B-espaces fibrés principaux $E_0$ et $E_t$ sont isomorphes pour tout $t\in \mathbf{I}$.

#### Corollaire 2 {#ta-iv-s6-prop-3-cor-2 .statement tag=024D}

Soient B et $B'$ des espaces topologiques, soit G un groupe topologique, soit E un B-espace fibré principal de groupe G. Soient $f_0$ et $f_1$ des applications continues de $B'$ dans B. Supposons que l’espace $B'$ soit paracompact. Si les applications $f_0$ et $f_1$ sont homotopes, les $B'$-espaces fibrés principaux $f_0^*E$ et $f_1^*E$ sont isomorphes.

#### Corollaire 3 {#ta-iv-s6-prop-3-cor-3 .statement tag=024E}

Soit B un espace topologique paracompact et soit G un groupe topologique. Si B est homéotope à un point, tout espace fibré principal de groupe G est trivialisable.

#### Remarque {#ta-iv-s6-n3-rem-1 .statement tag=024F}

Une démonstration alternative de ces résultats consisterait à vérifier que les isomorphismes d’espaces fibrés construits dans la prop. 2 et ses corollaires sont des isomorphismes d’espaces fibrés principaux.

### 4. Espaces fibrés universels

Soit G un groupe topologique, soient B et $B'$ des espaces topologiques et soient $(E, p)$ et $(E', p')$ des espaces fibrés principaux de groupe G et de bases B et $B'$ respectivement.

Soit U une partie ouverte de B et soit $f':^-p^1(U)\rightarrow E'$ une application continue qui est compatible avec les opérations de G dans $^-p^1(U)$ et $E'$ respectivement. Il existe alors une unique application continue $f: U\rightarrow B'$ telle que $f\circ p_U=p'\circ f'$ et le carré commutatif

$$
E_U^{f'}E'
$$

$p_Up'$

U $^fB'$

est alors cartésien (I, p. 94, exemple (FP)).

Pour toute partie ouverte U de B, notons alors $\mathscr{F}(U)$ l’ensemble des applications continues $g: E_U\rightarrow E'$ qui sont compatibles avec les opérations de G dans $^-p^1(U)$ et $E'$ respectivement. Pour tout couple $(U,V)$ d’ouverts de B tels que $U\subset V$, on note $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ l’application définie par $r_{UV}(g) =g|E_U$. On vérifie immédiatement que l’on a défini ainsi un faisceau $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ sur B. Nous appellerons ce faisceau le faisceau sur B des morphismes d’espaces fibrés principaux de groupe G de E dans $E'$.

#### Proposition 4 {#ta-iv-s6-prop-4 .statement tag=024G}

Si l’espace B est paracompact et si l’espace $E'$ est homéotope à un point, le faisceau sur B des morphismes d’espaces fibrés principaux de groupe G de E dans $E'$ est un faisceau mou.

Il existe un recouvrement ouvert $(U_j)_{j\in J}$ de B tel que, pour tout $j\in J$, l’espace fibré $E_{U_j}$ soit trivialisable. Comme l’espace B est paracompact, on peut supposer le recouvrement $(U_j)_{j\in J}$ localement fini (TG, IX, p. 49) et choisir un recouvrement $(A_j)_{j\in J}$ de B où, pour tout $j\in J$, l’ensemble $A_j$ est fermé dans B et contenu dans $U_j$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1).

D’après I, p. 65, cor. 2 de la prop. 6, il suffit, pour démontrer la proposition, d’établir l’assertion suivante : soit U une partie ouverte de B telle que l’espace fibré principal $(E_U, p_U)$ soit trivialisable, soit A une partie fermée de B contenue dans U, soit V un voisinage ouvert de A contenu dans U et soit $f$ un élément de $\mathscr{F}(V)$, il existe alors un voisinage ouvert W de A dans V et un élément $f'$ de $\mathscr{F}(U)$ tel que $r_{WU}(f') =r_{WV}(f)$. Démontrons cette assertion.

Soit W une partie ouverte de B telle que $A\subset W\subset W\subset V$. Soit $s: U\rightarrow E_U$ une section de $(E_U, p_U)$. Appliquons le corollaire 3 (IV, p. 438) à l’espace B, au fermé W et au voisinage V de W et à l’application $g=f\circ (s|_V)$ de $E_V$ dans $E'$. Il existe donc une application continue $\widetilde{g}: B\rightarrow E'$ qui coïncide avec $g$ sur W. Soit $h=\widetilde{g}|_U$. On a $h|_W=g|_W=f\circ (s|_W)$.

L’application $H: U\times G\rightarrow E'$ définie par $H(x, g) =h(x)\cdot g$ pour $(x, g)\in U\times G$ est continue et compatible avec les opérations de G dans $U\times G$ et $E'$. Posons $f'= H\circ s^{-1}$; c’est un élément de $\mathscr{F}(U)$. Pour tout $x\in W$, les applications $f$ et $f'$ coïncident au point $s(x)$, donc en tout point de $^-p^1(x)$, car ce sont des morphismes d’espaces fibrés principaux. La proposition en résulte.

#### Théorème 1 {#ta-iv-s6-thm-1 .statement tag=024H}

Soit G un groupe topologique, soit $B_u$ un espace topologique, et soit $(E_u, p_u)$ un espace fibré principal de groupe G et de base $B_u$. On suppose que l’espace $E_u$ est homéotope à un point.

Soit B un espace topologique paracompact.

a) Tout espace fibré principal de groupe G et de base B est isomorphe à un espace fibré principal de la forme $f^*E_u$, où $f: B\rightarrow B_u$ est une application continue.

b) Soient $f_0$ et $f_1$ des applications continues de B dans $B_u$. Pour que $f_0^*E_u$ et $f_1^*E_u$ soient des espaces fibrés principaux de groupe G et de base B isomorphes, il faut et il suffit que les applications $f_0$ et $f_1$ soient homotopes.

En d’autres termes, il existe une application de $[B,B_u]$ dans P(B; G) qui, à la classe d’homotopie d’une application continue $f$ de B dans $B_u$, associe la classe d’isomorphisme de l’espace fibré principal $f^*E_u$. Cette application est bijective.

Soit E un espace fibré principal de groupe G et de base B. D’après la prop. 4, le faisceau $\mathscr{F}$ sur B des morphismes d’espaces fibrés principaux de E dans $E_u$ est mou. Par suite, $\mathscr{F}(B)$ n’est pas vide, d’où a).

Soient $f_0$ et $f_1$ des applications continues de B dans $B_u$. Si les applications $f_0$ et $f_1$ sont homotopes, les espaces fibrés principaux $f_0^*E_u$ et $f_1^*E_u$ sont isomorphes (IV, p. 445, cor. 2). Démontrons la réciproque. Pour $\alpha \in  \{0,1\}$, notons $E_{\alpha}$ le $B_u$-espace fibré principal $f_{\alpha}^*E_u$, $g_{\alpha}: E_{\alpha}\rightarrow E_u$ la première projection et $p_{\alpha}: E_{\alpha}\rightarrow B$ la seconde projection. Soit $i: E_0\rightarrow E_1$ un isomorphisme d’espaces fibrés principaux. Soit $p$ l’application $p_0\times$ Id$_{\mathbf{I}}: E_0\times \mathbf{I}\rightarrow B\times \mathbf{I}$.

Comme l’espace $B\times \mathbf{I}$ est paracompact (TG, IX, p. 70, prop. 17), le faisceau $\mathscr{G}$ sur $B\times \mathbf{I}$ des morphismes d’espaces fibrés principaux de $E_0\times \mathbf{I}$ dans $E_u$ est mou (IV, p. 446, prop. 4). Posons $A = B\times  \{0,1\}$, $U = B\times ([0,^1_2[\cup ]^1_2,1])$, et définissons un élément $g$ de $\mathscr{G}(U)$ en posant

$g_0(x)$ pour $(x, t)\in E_0\times [0,^1[$,

$g(x, t) =$ 2

$g_1\circ i(x)$ pour $(x, t)\in E_0\times ]^1_2,1]$.

Comme le faisceau $\mathscr{G}$ est mou, il existe un élément $h\in \mathscr{G}(B\times \mathbf{I})$ et un voisinage ouvert V de A dans U tel que $h|V =g|V$ ; un tel élément est une application continue $H: E_0\times \mathbf{I}\rightarrow E_u$, compatible avec les opérations de G et telle que $H(x,0) =g_0(x)$, $H(x,1) =g_1(i(x))$ pour tout $x\in E_0$. Il existe alors une application $h': B\times \mathbf{I}\rightarrow B_u$ telle que $h'(p_0(x), t) =p_u(H(x, t))$ pour $x\in E_0$ et $t\in \mathbf{I}$; cette application est continue, c’est une homotopie reliant $f_0$ à $f_1$.

#### Corollaire {#ta-iv-s6-n4-cor-1 .statement tag=024I}

Soit G un groupe topologique, soient B et $B'$ des espaces topologiques paracompacts. Soient $(E, p)$ et $(E', p')$ des espaces fibrés principaux de groupe G et de base B et $B'$ respectivement. Supposons que les espaces E et $E'$ soient tous deux homéotopes à un point. Les espaces B et $B'$ sont homéotopes.

Il existe en effet une application continue $f: B\rightarrow B'$ telle que l’espace fibré principal E soit isomorphe à l’espace fibré principal $f^*E'$ et une application continue $g: B'\rightarrow B$ telle que l’espace fibré principal $E'$ soit isomorphe à l’espace fibré principal $g^*E$ (théorème 1, a)). Les espaces fibrés principaux $(g\circ f)^*E$ et E sont alors isomorphes, donc l’application $g\circ f$ est homotope à l’application Id$_B$ (théorème 1, b)). De même, l’application $f\circ g$ est homotope à l’application Id$_{B'}$.

Soit G un groupe topologique, soit B un espace topologique et soit E un espace fibré principal de groupe G et de base B. Supposons que l’espace E soit homéotope à un point. On dit que l’espace fibré principal E est universel pour les espaces fibrés principaux de groupe G et de base paracompacte, et on dit que l’espace B est un espace classifiant pour G. Si deux espaces classifiants pour G sont paracompacts, ils sont homéotopes. Lorsqu’il existe un espace classifiant, l’étude des classes d’isomorphisme d’espaces fibrés principaux de groupe G et de base paracompacte peut être considérée comme un problème d’homotopie.

#### Exemple {#ta-iv-s6-n4-exa-1 .statement tag=024J}

Muni de l’application $p:\mathbf{R}\rightarrow \mathbf{S}^1,t\mapsto e^{2\pi it}$, et de l’opération de $\mathbf{Z}$ par translation, l’espace $\mathbf{R}$ est un revêtement principal de groupe $\mathbf{Z}$. L’espace $\mathbf{S}^1$ est ainsi un espace classifiant pour le groupe $\mathbf{Z}$.

Pour tout groupe discret G, nous construirons dans le numéro suivant un espace métrisable qui est un espace classifiant pour G.

### 5. Espace classifiant pour un groupe discret

Soit G un groupe topologique ; notons $e$ son élément neutre. Soit $G^*$ l’ensemble des applications $h: [0,1[\rightarrow G$ pour lesquelles il existe une suite finie $(t_i)_{0\leqslant i\leqslant n}$ avec $0 =t_0< t_1<\cdots < t_n= 1$ telle que $h$ soit constante sur les intervalles $[t_{i-1}, t_i[$ pour $1\leqslant i\leqslant n$. Une telle suite sera dite adaptée à $h$. Pour toute partie finie de $G^*$, il existe une suite adaptée à chacun de ses éléments.

L’ensemble $G^*$ est un sous-groupe de $G^{[0,1[}$. Nous notons $e^*$ son élément neutre ; l’inverse d’un élément $h\in G^*$ est l’application $t\mapsto$ $h(t)^{-1}$, notée $h^{-1}$.

Soit V un voisinage de $e$ dans G. Soit $h\in G^*$ et soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à $h$. L’ensemble des éléments $t\in [0,1[$ tels que $h(t)\notin V$ est réunion de certains des intervalles $[t_{i-1}, t_i[$; la somme des longueurs $t_i-t_{i-1}$ de ces intervalles ne dépend pas de la suite $(t_i)_{0\leqslant i\leqslant n}$ choisie ; notons-la $p_V(h)$. Pour tout nombre réel $\varepsilon$ tel que $\varepsilon  >0$, notons alors $V^*_{\varepsilon}$ l’ensemble des $h\in G^*$ tels que $p_V(h)< \varepsilon$.

#### Proposition 5 {#ta-iv-s6-prop-5 .statement tag=024K}

Il existe une unique topologie sur $G^*$ compatible avec sa structure de groupe pour laquelle les ensembles $V^*_{\varepsilon}$ forment une base des voisinages de l’élément neutre.

Vérifions que les ensembles $V_{\varepsilon}^*$ satisfont aux axiomes (GV$'_I)$, (GV$'_{II})$ et (GV$'_{III})$ de TG, III, p. 4.

Soit V un voisinage de $e$ dans G et soit $\varepsilon$ un nombre réel strictement positif. Soit W un voisinage de $e$ dans G tel que $W\cdot W\subset V$. Soient $h$ et $h'$ des éléments de $G^*$. Si $t\in [0,1[$ tel $h(t)h'(t)\notin V$, on a $h(t)\notin W$ ou $h'(t)\notin W$. Il en résulte que $p_V(hh')\leqslant p_W(h)+p_W(h')$. Par conséquent, $W^*_{\varepsilon /2}\cdot W^*_{\varepsilon /2}\subset V^*_{\varepsilon}$, ce qui démontre l’axiome (GV$'_I)$.

Soit W un voisinage de $e$ dans G tel que $W^{-1}\subset V$. Alors $(W^*_{\varepsilon})^{-1}=$ $(W^{-1})^*_{\varepsilon}\subset V^*_{\varepsilon}$, d’où l’axiome (GV$'_{II})$.

Soit $k$ un élément de $G^*$; comme la fonction $k$ ne prend qu’un nombre fini de valeurs, il existe un voisinage W de $e$ dans G tel que $k(t)Wk(t)^{-1}\subset V$ pour tout $t\in [0,1[$. Soit alors $h$ un élément de $G^*$. Pour $t\in [0,1[$, si $k(t)h(t)k(t)^{-1}\notin$ V, alors $h(t)\notin W$. Par conséquent, $p_V(khk^{-1})\leqslant p_W(h)$. Cela démontre que $kW^*_{\varepsilon}k^{-1}\subset V^*_{\varepsilon}$, d’où l’axiome (GV$'_{III})$.

#### Proposition 6 {#ta-iv-s6-prop-6 .statement tag=024L}

L’espace $G^*$ est contractile et localement contractile en chacun de ses points.

Pour $h\in G^*$ et $t\in \mathbf{I}$, notons $\sigma (h, t)$ l’application de $[0,1[$ dans G donnée par $\sigma (h, t)(x) =h(x)$ si $0\leqslant x < t$ et $\sigma (h, t) =e$ sinon.

Montrons que l’application $\sigma : G^*\times \mathbf{I}\rightarrow G^*$ ainsi définie est continue. Soit en effet $k\in G^*,u\in \mathbf{I}$, soit V un voisinage de $e$ dans G et soit $\varepsilon$ un nombre réel strictement positif. L’élément $\sigma (h, t)\sigma (k, u)^{-1}$ de $G^*$ est l’application $f$ de $[0,1[$ dans G donnée par

$h(x)k(x)^{-1}$ si $0\leqslant x <$ min($t, u$) ;

$h(x)$ si $u\leqslant x < t$;

$$
f(x) =
$$

$k(x)^{-1}$ si $t\leqslant x < u$;

$e$ sinon.

Par suite,

$$
p_V(\sigma (h, t)\sigma (k, u)^{-1})\leqslant p_V(hk^{-1}) +|t-u|
$$

autrement dit, pour que $\sigma (h, t)\in V^*_{\varepsilon}\sigma (k, u)$, il suffit que l’on ait $|t-u|\leqslant^{\varepsilon}_2$ et $h\in V^*_{\varepsilon /2}k$, ce qui démontre la continuité de $\sigma$ en $(k, u)$.

Pour tout $h\in G^*,\sigma (h,0)$ est l’application constante d’image $\{e\}$, tandis que $\sigma (h,1) =h$. En outre, $\sigma (e, t) =e$ pour tout $t\in \mathbf{I}$. Par conséquent, $\sigma$ est une homotopie pointée en $e\in G^*$ reliant l’application constante d’image $\{e\}$ à l’application identique de $G^*$. Cela démontre que $G^*$ est contractile en $e^*$.

En outre, pour tout voisinage V de $e$ dans G et tout nombre réel $\varepsilon  >0$, on a $\sigma (V^*_{\varepsilon}\times \mathbf{I})\subset V^*_{\varepsilon}$. Par suite, $V^*_{\varepsilon}$ est aussi contractile en $e^*\in$ $G^*$, si bien que $G^*$ est localement contractile en $e^*$.

Comme $G^*$ est un groupe topologique, il est contractile et localement contractile en chacun de ses points.

Soit $\iota$ l’application de G dans $G^*$ qui, à $g\in G$, associe l’application constante d’image $\{g\}$ de $[0,1[$ dans G. L’application $\iota$ est un homomorphisme injectif de groupes. Soit V un voisinage de $e$ dans G et soit $\varepsilon$ un nombre réel strictement positif. On a $^-\iota^1(V^*_{\varepsilon}) = V$ si $\varepsilon \leqslant 1$ et $^-\iota^1(V^*_{\varepsilon}) = G$ sinon. L’image réciproque d’un voisinage de l’élément neutre de $G^*$ est un voisinage de l’élément neutre de G, d’où la continuité de $\iota$. De plus, $\iota (V) = V^*_1\cap \iota (G)$ pour tout voisinage V de $e$ dans G. Par suite, $\iota$ définit un isomorphisme de groupes topologiques de G sur son image.

#### Remarque 1 {#ta-iv-s6-n5-rem-1 .statement tag=024M}

Si G est un groupe topologique séparé, $\iota (G)$ est fermé dans $G^*$.

Soit en effet $h\in G^*$ tel que $h\notin \iota (G)$, soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à $h$, posons $\varepsilon =$ min$_{1\leqslant i\leqslant n}(t_i-t_{i-1})$. Soit V un voisinage de $e$ dans G tel que $h(t_i)^{-1}h(t_j)\notin V$, pour tout couple $(i, j)$ d’entiers tels que $0\leqslant i, j\leqslant n-1$ et $h(t_i)=\not h(t_j)$ ; il en existe car G est séparé. Soit W un voisinage de $e$ dans G tel que $W\cdot W^{-1}\subset V$. Démontrons qu’alors $hW^*_{\varepsilon}$ ne rencontre pas $\iota (G)$.

Raisonnons par l’absurde. Soient $f$ un élément de $W^*_{\varepsilon}$ et $g$ un élement de G tels que $hf$ = $\iota (g)$. On a donc $f(t) =h(t)^{-1}g$ pour tout $t\in [0,1[$, si bien que la suite $(t_i)$ est aussi adaptée à la fonction $f$. Si la valeur prise par $f$ sur l’intervalle $[t_{i-1}, t_i[$ n’appartient pas à W, alors $t_i-t_{i-1}< \varepsilon$, car $f\in W^*_{\varepsilon}$. Cette inégalité étant fausse, par définition de $\varepsilon$, on a $f(t)\in W$ pour tout $t\in [0,1[$. Soient alors $i$ et $j$ des éléments de $\{0, . . . , n-1\}$ tels que $h(t_i)=\not h(t_j)$ ; on a

$$
h(t_i)^{-1}h(t_j) =f(t_i)g^{-1}gf(t_j)^{-1}=f(t_i)f(t_j)^{-1}\in W\cdot W^{-1}
$$

ce qui contredit le choix de W. Le sous-groupe $\iota (G)$ de $G^*$ est donc fermé.

Supposons que G soit un groupe topologique métrisable et soit $d$ une distance sur G qui définit sa topologie. Soient $h$ et $h'\in G^*$ et soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à $h$ et $h'$. Le nombre réel

$$
\sum_{i=1}^n(t_i-t_{i-1})d h(t_{i-1}), h'(t_{i-1})
$$

ne dépend pas de la suite $(t_i)$ choisie ; notons-le $d^*(h, h')$.

Démontrons que $d^*$ est une distance sur $G^*$. On a $d^*(h, h') =$ $d^*(h', h)$ pour $h,h'\in G^*$, et $d^*(h, h) = 0$ pour tout $h\in G^*$. Inversement, soient $h$ et $h'$ des éléments de $G^*$ tels que $d^*(h, h') = 0$. Soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à $h$ et $h'$. Comme

$$
0 =d^*(h, h') =\sum_{i=1}^n(t_i-t_{i-1})d h(t_{i-1}), h'(t_{i-1})
$$

et que tous les termes de cette somme sont positifs ou nuls, on a $d(h(t_{i-1}), h'(t_{i-1})) = 0$ pour tout $i\in  \{1, . . . , n\}$, d’où $h=h'$. Enfin, soient $h,h',h''$ des éléments de $G^*$ et soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à chacune d’entre elles. Alors,

$$
d^*(h, h'') =\sum_{i=1}^n(t_i-t_{i-1})d h(t_{i-1}), h''(t_{i-1})
$$

$$
\leqslant \sum_{i=1}^n(t_i-t_{i-1})d h(t_{i-1}), h'(t_{i-1})+d h(t_{i-1}), h''(t_{i-1})
$$

$$
=d^*(h, h') +d^*(h, h'')
$$

donc $d^*$ vérifie l’inégalité triangulaire.

Cette distance $d^*$ est invariante par translations à droite (resp. à gauche) si $d$ l’est.

#### Proposition 7 {#ta-iv-s6-prop-7 .statement tag=024N}

Supposons que G soit un groupe topologique métrisable. Alors, le groupe topologique $G^*$ est métrisable. Plus précisément, si $d$ est une distance bornée sur G qui définit sa topologie, la topologie de $G^*$ est définie par la distance $d^*$.

Soit $d$ une distance sur G qui définit sa topologie. Alors, l’application $d'$ donnée par $d'(h, h') =$ inf($d(h, h'),1$) est une distance bornée sur G qui définit aussi sa topologie (TG, IX, p. 3). Il suffit donc de démontrer que $d^*$ définit la topologie de $G^*$ sous l’hypothèse que $d$ est bornée.

Soit V un voisinage de $e$ dans G et soit $\varepsilon$ un nombre réel strictement positif. Soit $\delta$ un nombre réel strictement positif tel que V contienne la boule $B(e, \delta )$. Soit $h\in G^*$ et soit $(t_i)_{0\leqslant i\leqslant n}$ une suite adaptée à $h$. Alors,

$$
p_V(h) =\sum_{h(t_ii_-=1)\notin V}^{n_1}(t_i-t_{i-1})
$$

$$
^nd(h(t_{i-1}), e)
$$

$$
\leqslant \sum(t_i-t_{i-1})
$$

$$
\delta
$$

$$
i=1
$$

$d(h(t_{i-1}),e)\geqslant \delta$

$$
d^*(h, e^*)
$$

$$
\leqslant
$$

$$
\delta
$$

Par conséquent, la boule $B(e^*, \varepsilon \delta )$ dans $G^*$ est contenue dans $V_{\varepsilon}^*$.

Inversement, soit $\delta$ un nombre réel strictement positif et soit Δ un majorant strictement positif du diamètre de G. Soit V un voisinage de $e$ dans G contenu dans la boule $B(e, \delta /2)$. Pour une fonction $h\in G^*$ et une suite $(t_i)_{0\leqslant i\leqslant n}$ adaptée à $h$, on a

$$
d^*(h, e^*) =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)
$$

= $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)\leqslant \delta /2$

+ $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)>\delta /2$

$\leqslant \delta + \Delta \sum^n(t_i-t_{i-1})$

2 $i_{=1}$

$h(t_{i-1})\notin V$

$$
\leqslant \delta + \Delta p_V(h)
$$

2

L’inégalité précédente entraîne que, pour tout élément $h$ de $V_{\delta /2\Delta}^*$, on a $d^*(h, e^*)\leqslant \delta$. Par conséquent, toute boule de $G^*$ pour la distance $d^*$ contient un voisinage de l’élément neutre.

#### Remarque 2 {#ta-iv-s6-n5-rem-2 .statement tag=024O}

Soit $d$ une distance bornée qui définit la topologie de G. Lorsque l’on munit le groupe topologique $G^*$ de la distance $d^*$, l’homomorphisme $\iota : G\rightarrow G^*$ est une isométrie.

#### Remarque 3 {#ta-iv-s6-n5-rem-3 .statement tag=024P}

Supposons que G soit un groupe topologique discret. Le sous-groupe $\iota (G)$ est alors un sous-groupe discret de $G^*$. En effet, la topologie de G est définie par la distance $d$ sur G donnée par $d(g, g') = 1$ si $g=\not g'$ et $d(g, g') = 0$ sinon. L’assertion résulte alors de la remarque précédente.

#### Théorème 2 {#ta-iv-s6-thm-2 .statement tag=024Q}

Soit G un groupe topologique discret. Faisons opérer G à droite dans $G^*$ par $h\cdot g=h\iota (g)$ et notons B l’espace topologique quotient $G^*/G$.

L’espace $G^*$ est un revêtement de B, principal de groupe G; il est simplement connexe par arcs.

L’espace B est un espace topologique métrisable, connexe par arcs, localement contractile et son groupe de Poincaré en tout point est isomorphe à G.

Ainsi, l’espace B est un espace classifiant pour le groupe G.

Le groupe $G^*$ est contractile en son élément neutre (IV, p. 450, prop. 6). Il est en particulier connexe par arcs (III, p. 260) et simplement connexe par arcs (IV, p. 340).

Le groupe $\iota (G)$ est fermé dans $G^*$ (TG, III, p. 7, prop. 5), donc l’espace $G^*/G$ est métrisable (TG, III, p. 13, prop. 18 et TG, IX, p. 25, prop. 4). Il est aussi connexe par arcs (III, p. 258, prop. 3). Comme le groupe $\iota (G)$ est discret, il résulte du corollaire 2 de I, p. 100, que $G^*$ est un revêtement principal de groupe G de B. Le revêtement pointé $(G^*, e^*)$ est alors un revêtement universel de l’espace B pointé en l’image de $e^*$; le groupe de Poincaré de B (en chacun de ses points) est isomorphe à G.

# Exercices

§1

1) Soit S le graphe de l’application de $]0,1[$ dans $\mathbf{R}$ donnée par $t\mapsto$ sin($\pi /t$). Soit W la réunion de S et de l’image d’un chemin dans $\mathbf{R}^2-$ S reliant les points $(0,0)$ et $(1,0)$ (« cercle de Varsovie »).

a) Démontrer que l’espace W est simplement connexe par arcs mais qu’il n’est pas simplement connexe.

b) Pour tout entier $n\geqslant 0$, on pose $X_n=\mathbf{R}/2^n\mathbf{Z}$ et on note $f_n: X_{n+1}\rightarrow X_n$ la surjection canonique ; soit X l’espace lim$\leftarrow -_nX_n$. Démontrer que l’espace X est simplement connexe par arcs mais qu’il n’est pas simplement connexe.

2) Soit X l’espace topologique de l’exercice 4 de III, p. 331 et soit Y sa suspension (I, p. 149, exerc. 1). Démontrer que l’espace Y est simplement connexe mais que $\pi_1(Y, y)=\not\{e_y\}$ pour tout $y\in Y$.

3) Soit X un espace topologique et soit $x$ un point de X.

Soit $\mathscr{R}$ une catégorie de revêtements de X et $\mathscr{E}$ une catégorie d’ensembles (cf. II, p. 160, exemple 2).

a) On suppose que pour tout revêtement E de X qui est un objet de $\mathscr{R}$, la fibre $E_x$ de E en $x$ est un objet de $\mathscr{E}$; on pose alors $\Phi_x(E) = E_x$. Pour tout morphisme $f: E'\rightarrow E$ de revêtements de B qui sont des objets de $\mathscr{R}$, on note $\Phi_x(f)$ l’application de $E'_x$ dans $E_x$ déduite de $f$ par passage aux sous-ensembles. Démontrer que $\Phi_x$ est un foncteur de la catégorie $\mathscr{R}$ dans la catégorie $\mathscr{E}$. b) Soit $G(x)$ l’ensemble des familles $\varphi = (\varphi_E)$ où, pour tout objet E de $\mathscr{R}$, $\varphi_E$ est une permutation de l’ensemble $\Phi_x(E)$ telle que pour toute flèche $f: E'\rightarrow E$ de $\mathscr{R}$, on ait $f_*\circ \varphi_{E'}=\varphi_E\circ f_*$ (« automorphismes du foncteur $\Phi_x$ ».)

La relation donnée par $\varphi \cdot \psi = (\varphi_E\circ \psi_E)$ pour $\varphi , \psi \in G(x)$ munit l’ensemble $G(x)$ d’une structure de groupe. Pour tout objet E de $\mathscr{R}$, on note $G(x)_E$ l’ensemble des $\varphi \in G(x)$ tels que $\varphi_E=$ Id$_{\Phi_x(E)}$; c’est un sous-groupe de $G(x)$.

c) Démontrer qu’il existe une unique structure de groupe topologique sur $G(x)$ pour laquelle les groupes $G(x)_E$ forment une base de voisinages de l’élément neutre.

d) Soit T un sous-espace simplement connexe de X. Si $x, y$ sont des points de T, les groupes topologiques $G(x)$ et $G(y)$ sont isomorphes.

e) Démontrer que le relèvement des chemins définit un homomorphisme de groupes continu de $\pi_1(X, x)$ vers $G(x)$. Cet homomorphisme n’est pas forcément surjectif (exerc. 1 ; I, p. 146, exerc. 6) ni injectif (exerc. 2). C’est un isomorphisme si X est délaçable et si tout revêtement connexe de X est isomorphe à un objet de $\mathscr{R}$.

4) Pour tout entier $n\geqslant 1$, soit $X_n$ la réunion des trois segments du plan numérique $\mathbf{R}^2$ dont les extrémités sont $(0,1)$, $(1/2n,0)$ et $(1/(2n-1),0)$. Soit $X_0$ le segment d’extrémités $(0,1)$ et $(0,0)$. Soit X la réunion des ensembles $X_n$, pour $n\geqslant 1$, et soit Y = X. Soit $a= (0,1)$.

a) Démontrer que $Y = X\cup X_0$.

b) Démontrer que X est localement contractile.

c) Démontrer que l’injection canonique de X dans Y induit un isomorphisme de groupes de $\pi_1(X, a)$ sur $\pi_1(Y, a)$.

d) Démontrer que la topologie quotient de la convergence compacte sur $\pi_1(Y, a)$ n’est pas discrète.

5) Soit X le sous-espace de $\mathbf{R}^2$ réunion de $[0,1]\times  \{0,1\}$, de $\{0\} \times [0,1]$ et des segments $\{^1_n\} \times [0,1]$, pour $n\geqslant 1$.

a) Démontrer que tout point $a$ de X admet un voisinage V tel que l’image de $\pi_1(V, a)$ dans $\pi_1(X, a)$ soit triviale.

b) Démontrer que la topologie quotient de la topologie de la convergence compacte sur le groupe $\pi_1(X, a)$ n’est pas discrète.

6) Soit X l’espace $\mathbf{R}^2-\mathbf{Q}^2$.

a) Démontrer que l’espace X est connexe par arcs. b) Soient $a, b$ des points de $\mathbf{R}-\mathbf{Q}$. Soit $c_{a,b}:\mathbf{I}\rightarrow \mathbf{R}^2$ l’unique application qui vérifie $c(0) = (a, a),c(1/4) = (a, b),c(1/2) = (b, b),c(3/4) = (b, a)$ et $c(1) = (a, a)$ et dont les restrictions aux intervalles $[(m-1)/4, m/4]$ sont affines, pour $1\leqslant m\leqslant 4$. Démontrer que $c_{a,b}$ est un lacet dans X.

c) Soient $a, b, b'$ des éléments de $\mathbf{R}-\mathbf{Q}$ tels que $b=\not b'$. Démontrer que les lacets $c_{a,b}$ et $c_{a,b'}$ ne sont pas strictement homotopes.

d) En déduire que, pour tout $a\in \mathbf{R}-\mathbf{Q}$, le groupe $\pi_1(X,(a, a))$ a la puissance du continu.

§2

1) Soit X un espace de Lindelöf (TG, IX, appendice 1, p. 75, déf. 1) délaçable. Démontrer que, pour tout point $x\in X$, le groupe de Poincaré $\pi_1(X, x)$ est dénombrable.

2) Soit Y un espace uniforme et soit X un sous-espace de Y. Soit $(U_i)_{i\in I}$ un recouvrement ouvert de X.

a) Démontrer qu’il existe un voisinage ouvert V de X dans Y et un recouvrement ouvert $(V_i)_{i\in I}$ de V vérifiant les propriétés suivantes :

(i) Pour tout $i,U_i= V_i\cap X$ ;

(ii) Pour toute partie J de I telle que $\bigcap_{j\in J}V_j=\not\emptyset ,\bigcap_{j\in J}U_j=\not\emptyset$.

b) On suppose que Y est localement connexe et que les $U_i$ sont connexes. Démontrer qu’il existe un tel recouvrement où les $V_i$ sont des ouverts connexes de Y.

c) Supposons que les $U_i$ soient connexes et soit, pour tout $i\in I$, un point $x_i\in U_i$. Supposons que l’image de $\pi_1(U_i, x_i)$ dans $\pi_1(X, x_i)$ soit réduite à l’élément neutre. Montrer qu’il existe un voisinage V de X dans Y tel que, pour tout $x\in X$, l’homomorphisme canonique $\pi_1(X, x)\rightarrow \pi_1(V, x)$ admette une rétraction.

3) [^1] Soit X un espace topologique et soit $x$ un point de X.

Soit G un groupe et soit $\varphi :\pi_1(X, x)\rightarrow G$ un homomorphisme de groupes. Soit $(U_n)_{n\in\mathbf{N}}$ une suite décroissante de sous-espaces de X dont l’intersection est réduite au point $x$. Pour tout $n$, soit $G_n$ l’ensemble des éléments de G qui sont image par $\varphi$ de la classe d’un lacet contenu dans $U_n$. a) Si G est dénombrable, la suite $(G_n)$ est stationnaire. (Se ramener au cas où $(G_n: G_{n+1})\geqslant n+ 1$ pour tout $n$ et considérer une énumération $(\gamma_n)_n$ de G; construire par récurrence des éléments $\lambda_n\in G_n$ tels que, notant $w_n=\lambda_1. . . \lambda_n$, on ait $\gamma_i\notin w_nG_{n+1}$ pour $1\leqslant i\leqslant n$. Montrer alors que l’intersection $\bigcap_iw_iG_{i+1}$ n’est pas vide.)

b) Supposons que G soit abélien et que son élément neutre soit le seul élément indéfiniment divisible de G. Alors $\bigcap_nG_n$ est réduit à l’élément neutre. (Soit $a$ un élément de l’intersection ; pour tout $n$, soit $\gamma_n\in \pi_1(U_n, x)$ dont l’image par $\varphi$ soit égale à $a$. Construire par récurrence des classes de chemins $\lambda_n\in \pi_1(U_n, x)$ telles que $\lambda_n=\gamma_n\lambda^d_{n+1}$, où $d$ est un entier $\geqslant 2$ fixé. Montrer que $b= (d-1)\varphi (\lambda_1) +a$ est indéfiniment divisible. En déduire que $a= 0$.) c) Plus généralement, si G est abélien et si tout élément indéfiniment divisible de G est de torsion, alors l’intersection des $G_n$ est formée d’éléments de torsion.

4) Soit X un espace topologique connexe et localement connexe par arcs. Soit $x$ un point de X qui possède un système fondamental dénombrable de voisinages. Soit S un ensemble et soit $\varphi :\pi_1(X, x)\rightarrow \mathbf{Z}^{(S)}$ un homomorphisme de groupes surjectif.

a) Démontrer que S est dénombrable.

b) On suppose que X est compact ; démontrer que S est fini.

c) On suppose que $\pi_1(X, x)$ est un groupe abélien libre ; démontrer que X est délaçable.

d) On suppose que $\pi_1(X, x)$ est un groupe libre ; démontrer que X est délaçable. (Utiliser le fait que l’intersection des sous-groupes de la suite centrale descendante d’un groupe libre est réduite à l’élément neutre.)

5) Soit P la boucle d’oreille hawaïenne (III, p. 336, exerc. 6, dont on reprend les notations). Pour $n\in \mathbf{N}^*$, soit $\alpha_n\in \pi_1(P, o)$ la classe d’un lacet dans $C_n$ dont la classe engendre $\pi_1(C_n,0)$.

a) Démontrer que l’application Hom($\pi_1(P,0),\mathbf{Z}$)$\rightarrow \mathbf{Z}^{\mathbf{N}},\varphi \mapsto (\varphi (\alpha_n))_{n\in\mathbf{N}}$ est un homomorphisme injectif de groupes et que son image est égale à $\mathbf{Z}^{(\mathbf{N})}$.[^2]

b) Le groupe $\pi_1(P,0)$ n’est pas un groupe libre ; le quotient de $\pi_1(P,0)$ par son groupe dérivé n’est pas un groupe abélien libre.

c) Soit A l’archipel hawaïen (III, p. 338, exerc. 10). Démontrer que tout homomorphisme de $\pi_1(A, o)$ dans $\mathbf{Z}$ est trivial.

§3

1) Soit G le groupe topologique $O(2,\mathbf{R})$. On a $\pi_0(G)\simeq \mathbf{Z}/2\mathbf{Z}$ et $\pi_1(G)\simeq \mathbf{Z}$; l’élément non trivial de $\pi_0(G)$ agit sur $\pi_1(G)$ par l’application $t\mapsto  -t$.

2) On note $\mathbf{H}$ l’algèbre des quaternions de Hamilton (TG, VIII, p. 4) et $(1, i, j, k)$ sa base canonique. On note N la forme quadratique norme de $\mathbf{H}$; l’ensemble des quaternions de norme 1 est la sphère $\mathbf{S}_3$. Soit $\mathbf{H}_0$ le sous$\mathbf{R}$-espace vectoriel des quaternions de trace nulle et $N_0$ la restriction à $\mathbf{H}_0$ de N.

a) Démontrer que l’homomorphisme de la prop. 4 de TG, VIII, p. 4, fait de la sphère $\mathbf{S}_3$ un revêtement de degré 2 de $\mathbf{S}\mathbf{O}(N_0)$.

b) En déduire que le groupe de Poincaré de SO(3$,\mathbf{R})$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$. Expliciter un lacet en $I_3$ dans SO(3$,\mathbf{R})$ dont la classe d’homotopie stricte est l’unique élément non trivial de ce groupe de Poincaré.

c) Soit $\varphi$ l’application de $\mathbf{S}_3\times \mathbf{S}_3$ dans SO(4$,\mathbf{R})$ donnée par $\varphi (\mathbf{q}_1,\mathbf{q}_2)(\mathbf{x}) =$ $\mathbf{q}_1\mathbf{x}\mathbf{q}^{-1}_2$. Démontrer que $\varphi$ fait de $\mathbf{S}_3\times \mathbf{S}_3$ un revêtement de degré 2.

d) En déduire que le groupe de Poincaré de SO(4$,\mathbf{R})$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$.

3) Soit $n$ un entier naturel. On fait agir le groupe topologique SO($n+ 1,\mathbf{R}$) sur la sphère $\mathbf{S}_n$ de $\mathbf{R}^{n+1}$.

a) Démontrer que le fixateur du vecteur $\mathbf{e}_{n+1}$ s’identifie au groupe topologique SO($n,\mathbf{R}$).

b) Soit $f:\mathbf{I}\rightarrow \mathbf{S}_n$ une application continue. On suppose que $f(t)=\not$ $(0, . . . ,0,1)$ pour tout $t\in \mathbf{I}$. Démontrer qu’il existe une application continue $g:\mathbf{I}\rightarrow$ SO($n+ 1,\mathbf{R}$) telle que $f(t) =g(t)\cdot \mathbf{e}_{n+1}$ pour tout $t\in \mathbf{I}$.

c) Si $n\geqslant 3$, démontrer que l’injection de SO($n,\mathbf{R}$) dans SO($n+1,\mathbf{R}$) induit un isomorphisme entre groupes de Poincaré.

4) Soit $n$ un entier naturel. Soit $B_0$ le sous-groupe de $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ formé des matrices triangulaires supérieures dont les coefficients diagonaux sont tous strictement positifs.

a) Démontrer que l’application de SO($n,\mathbf{R}$)$\times B_0$ dans $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ donnée par $(g, u)\mapsto g\cdot u$ est un homéomorphisme (cf. INT, VII, p. 91, prop. 7).

b) Démontrer que l’inclusion de SO($n,\mathbf{R}$) dans $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ induit un isomorphisme entre groupes de Poincaré.

5) Soit G un groupe topologique connexe délaçable, soit $(\widetilde{G}, p)$ un revêtement universel de G; on munit $\widetilde{G}$ de sa structure de groupe topologique pour laquelle $p$ est un homomorphisme de groupes. On note Z le centre de G$,e$ son élément neutre, $\widetilde{Z}$ le centre de $\widetilde{G}$ et $\widetilde{e}$ son élément neutre. a) Soit $f$ un automorphisme continu du groupe G. Démontrer qu’il existe une unique application continue $\widetilde{f}:\widetilde{G}\rightarrow \widetilde{G}$ telle que $\widetilde{f}(\widetilde{e}) =\widetilde{e}$ et $p\circ \widetilde{f}$ = $f\circ p$. Démontrer que $\widetilde{f}$ est un automorphisme de groupes. Démontrer que l’application $\varphi :f\mapsto \widetilde{f}$ est un morphisme de groupes injectif de Aut(G) dans Aut($\widetilde{G}$).

b) On note Out(G) le quotient du groupe Aut(G) par le sous-groupe des automorphismes intérieurs ; on définit Out($\widetilde{G}$) de manière analogue. Démontrer que l’homomorphisme $\varphi$ induit, par passage aux quotients, un homomorphisme de groupes injectif $\psi :$ Out(G) $\rightarrow$ Out($\widetilde{G}$).

6) Soient G et H des groupes de Lie réels connexes et soit $f: G\rightarrow H$ un morphisme surjectif de groupes de Lie. On note $Z_G$ le centre de G et $Z_H$ celui de H.

a) Démontrer l’équivalence des assertions suivantes : (i) L’application $f$ fait de G un revêtement de H ; (ii) Ker($f$) est discret ; (iii) Le morphisme $L(f): L(G)\rightarrow L(H)$ déduit de $f$ par passage aux algèbres de Lie est un isomorphisme.

b) Démontrer qu’alors $f(Z_G) = Z_H$ et que $f^{-1}(Z_H) = Z_G$.

7) Soit G un groupe de Lie réel, notons $G_0$ sa composante neutre, $Z_0$ le centre de $G_0$ et $\pi_0(G) = G/G_0$. Soit $(\widetilde{G}_0, p_0)$ un revêtement universel de $G_0$, $\widetilde{Z}_0$ le centre de $\widetilde{G}_0$ et $\widetilde{e}$ son élément neutre.

a) Soit $\theta :\pi_0(G)\rightarrow$ Out(G$_0)$ l’homomorphisme associé à l’extension $\mathscr{E}: G_0\rightarrow G\rightarrow \pi_0(G)$ (A, X, §7, exerc. 5). Démontrer que la classe de cohomologie $\omega (\pi_0(G),Z_0, \theta )$ de $H^3(\pi_0(G),Z_0)$ définie dans loc. cit. est nulle. b) On suppose qu’il existe un groupe de Lie $\widetilde{G}$, une application surjective $p:\widetilde{G}\rightarrow G$ et un isomorphisme $j$ de $\widetilde{G}_0$ sur la composante neutre de $\widetilde{G}$ tels que $p_0=p\circ j$. Démontrer que l’on a $\omega (\pi_0(G),\widetilde{Z}_0, \psi \circ \theta ) = 0$ dans $H^3(\pi_0(G),\widetilde{Z}_0)$, où $\psi :$ Out(G$_0)\rightarrow$ Out($\widetilde{G}_0$) est l’homomorphisme défini dans l’exerc. 5.

c) On suppose que $\omega (\pi_0(G),\widetilde{Z}_0, \psi \circ \theta ) = 0$. Soit $\widetilde{\mathscr{E}}:\widetilde{G}_0\rightarrow E\rightarrow \pi_0(G)$ une extension de $\pi_0(G)$ par $\widetilde{G}_0$ dont l’homomorphisme associé est égal à $\psi \circ \theta$. Démontrer que $E/\pi_1(G_0)$ est une extension de $\pi_0(G)$ par $G_0$ dont l’homomorphisme associé est égal à $\theta$.

Soit alors $\gamma$ l’unique élément de $H^2(\pi_0(G),G_0)$ tel que $\gamma \cdot [E/\pi_1(G_0)] =$ [G] (loc. cit., e)). Considérons l’homomorphisme $\delta : H^2(\pi_0(G),Z_0)\rightarrow$ $H^3(\pi_0(G), \pi_1(G))$ associé à la suite exacte de groupes abéliens $1\rightarrow \pi_1(G_0)\rightarrow$ $\widetilde{Z}_0\rightarrow Z_0\rightarrow 1$ (exerc. 6). Démontrer que l’élément $\delta (\gamma )$ de $H^3(\pi_0(G), \pi_1(G))$ ne dépend pas du choix de l’extension $\widetilde{\mathscr{E}}$; on le note $\delta (G)$.

d) On suppose que $\omega (\pi_0(G),\widetilde{Z}_0, \psi \circ \theta ) = 0$. Pour qu’il existe un groupe de Lie $\widetilde{G}$, une application surjective $p:\widetilde{G}\rightarrow G$ et un isomorphisme $j$ de $\widetilde{G}_0$ sur la composante neutre de $\widetilde{G}$ tels que $p_0=p\circ j$, il faut et il suffit que l’on ait $\delta (G) = 0$. [^3]

8) Soit G un groupe de Lie et soit H un sous-groupe fermé de G; on note $H_0$ la composante neutre de H et $\pi_0(H)$ le groupe $H/H_0$. Notons aussi $p$ la surjection canonique de G sur $G/H$.

a) L’application $p$ possède la propriété de relèvement des chemins.

b) Si H est connexe, l’homomorphisme $p_*:\pi_1(G, e)\rightarrow \pi_1(G/H, p(e))$ est surjectif.

c) Il existe une unique application $\varphi :\pi_1(G/H, p(e))\rightarrow \pi_0(H)$ qui, pour tout chemin $\widetilde{c}$ d’origine $e$ dans G dont le terme appartient à H, associe à la classe du lacet $p\circ \widetilde{c}$ dans $G/H$ la classe de $\widetilde{c}(1)$ modulo $H_0$; c’est un morphisme de groupes.

d) Si G est simplement connexe, alors $\varphi$ est un isomorphisme. En particulier, H est connexe si et seulement si $G/H$ est simplement connexe.

9) Soit G un groupe de Lie connexe, soit $(\widetilde{G}, q)$ un revêtement universel de G et soit $\widetilde{e}$ l’élément neutre de $\widetilde{G}$. Soit H un sous-groupe fermé connexe de G ; on note $i: H\rightarrow G$ l’injection canonique et $p: G\rightarrow G/H$ la surjection canonique.

a) Soit $H_1$ la composante neutre de $^-q^1(H)$ et soit $q_1:\widetilde{G}/H_1\rightarrow G/H$ l’application déduite de $q$ par passage aux quotients. Démontrer que $q_1$ fait de $\widetilde{G}/H_1$ un revêtement de $G/H$ dont la fibre en $p(e)$ est isomorphe à $\pi_1(G/H, p(e))$. b) En déduire qu’il existe une suite exacte de groupes

$$
\pi_1(H_1,\widetilde{e})\longrightarrow^{q_*}\pi_1(H, e)\longrightarrow^{i_*}\pi_1(G, e)\longrightarrow^{p_*}\pi_1(G/H, p(e))
$$

10) a) Démontrer que, pour tout entier $n\geqslant 2$, le groupe SU($n,\mathbf{C}$) est simplement connexe. (L’espace SU(2$,\mathbf{C})$ est homéomorphe à $\mathbf{S}_3$. Faire opérer SU($n,\mathbf{C}$) sur la sphère unité de $\mathbf{C}^n$, identifier le fixateur du point $(0, . . . ,0,1)$ au groupe SU($n-1,\mathbf{C}$) et utiliser l’exercice 9.)

b) Démontrer que pour tout entier $n\geqslant 2$, le groupe $\mathbf{S}\mathbf{L}(n,\mathbf{C})$ est simplement connexe. (Soit $B_+$ le sous-groupe de $\mathbf{S}\mathbf{L}(n,\mathbf{C})$ formé des matrices triangulaires supérieures dont les coefficients diagonaux sont des nombres réels $>0$. Démontrer que l’application de SU($n,\mathbf{C}$)$\times B_+$ dans $\mathbf{S}\mathbf{L}(n,\mathbf{C})$ donnée par $(g, u)\mapsto g\cdot u$ est un homéomorphisme.)

§4

1) Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Soit $(T, p)$ un Y-espace. La donnée de descente canonique $\tau$ sur le X-espace $Z = X\times_YT$ est effective (IV, p. 385, prop. 1), l’application canonique $Z/R_{\tau}\rightarrow T$ est injective et continue. Elle n’est toutefois pas forcément surjective, ni stricte.

2) Soit Y un espace topologique obtenu par recollement d’espaces $X_i$; soit X l’espace topologique somme de la famille $(X_i)$ et soit $f: X\rightarrow Y$ l’application canonique (TG, I, p. 16). Pour tout $i$, posons $Y_i=f(X_i)$ et soit $f_i: X_i\rightarrow Y_i$ l’application déduite de $f$ par passage aux sous-espaces. L’application $f_i$ est bijective et continue. Si l’application $f_i$ n’est pas un homéomorphisme, la donnée de descente canonique sur X, relative à $f$, n’est pas effective. Pour un exemple, cf. TG, I, p. 94, exerc. 15.

3) Notons B l’ensemble des points $(x, y)$ du carré $[0,1]^2$ vérifiant $x= 0$, ou $x= 1$, ou $y= 0$, ou $y= 1$, ou il existe $n\in \mathbf{N}$ tel que $nx= 1$. Soient $B_1$ et $B_2$ les sous-ensembles de B formés des points $(x, y)$ de B pour lesquels $y\leqslant^1_2$ et $y\geqslant^1_2$ respectivement.

Construire un B-espace $(E, p)$ qui n’est pas un revêtement mais tel que le $B_1$-espace $(E_{B_1}, p_{B_1})$ et le $B_2$-espace $(E_{B_2}, p_{B_2})$ soient des revêtements.

4) On dit qu’un espace topologique est localement simplement connexe par arcs si tout point possède une base de voisinages simplement connexes par arcs.

a) Donner un exemple d’espace topologique simplement connexe par arcs qui n’est pas localement simplement connexe par arcs.

b) Soit X un espace topologique et soit G un groupe discret agissant proprement sur X. Si X est localement simplement connexe par arcs, il en est de même de $X/G$.

5) Soit G un groupe de Lie opérant proprement sur un espace topologique délaçable et complètement régulier X. On pose $Y = X/G$ et on note $f: X\rightarrow Y$ l’application canonique. Démontrer que le morphisme de groupoïdes canonique $\varpi (X)/G\rightarrow$ Coeg($f$) est un isomorphisme. (Utiliser LIE, IX, §9, exerc. 17 pour adapter la preuve du théorème 3 de IV, p. 403.)

6) Soit X un espace topologique connexe par arcs, soit G un groupe opérant continûment dans X et soit $x$ un point de X tel que $g\cdot x=x$ pour tout $g\in G$. Notons $p$ l’application canonique de X dans $X/G$. Soit H un groupoïde et soit $\varphi :\varpi (X)\rightarrow H$ un morphisme de groupoïdes. On suppose que pour tout chemin $c$ dans X et tout $g\in G$, on a $\varphi ([g\cdot c]) =\varphi ([c])$, et que pour tout lacet $c\in \Omega_x(X),\varphi ([c]) =e_{\varphi(x)}$.

Soient $c_1$ et $c_2$ des chemins dans X tels que $p\circ c_1$ et $p\circ c_2$ aient même origine et même terme. Démontrer que l’on a $\varphi ([c_1]) =\varphi ([c_2])$.

7) Soit X un espace topologique délaçable et soit G un groupe discret opérant proprement dans X ; on note $m: G\times X\rightarrow$ X l’opération de G, pr$_2: G\times X\rightarrow X$ la seconde projection, et $f: X\rightarrow X/G$ la surjection canonique.

a) Démontrer que le morphisme de groupoïdes $\varpi (f)$ est surjectif.

b) Soit H un groupoïde et soit $\varphi :\varpi (X)\rightarrow H$ un morphisme de groupoïdes tel que $\varphi \circ \varpi (m) =\varphi \circ \varpi$(pr$_2)$.

Soient $c_1$ et $c_2$ des chemins dans X tels que les chemins $f\circ c_1$ et $f\circ c_2$ dans $X/G$ soient strictement homotopes. Démontrer que l’on a $\varphi ([c_1]) =$ $\varphi ([c_2])$.

c) Démontrer qu’il existe un unique morphisme de groupoïdes $\varphi '$ de $\varpi (X/G)$ dans H tel que $\varphi =\varphi '\circ \varpi (f)$. En déduire une nouvelle démonstration du théorème 3 de IV, p. 403.

§5

1) Soit A une partie fermée et discrète de $\mathbf{R}^2$.

a) Pour $R>0$, soit $D_R$ l’ensemble des $z\in \mathbf{C}$ tels que $|z|<R$; montrer que le groupe fondamental de $D_R-(A\cap D_R)$ est isomorphe au groupe libre sur $A\cap D_R$.

b) Démontrer qu’il existe un homéomorphisme $f$ de $\mathbf{R}^2$ dans lui-même tel que $f(A)\subset \mathbf{N}\times  \{0\}$.

c) Montrer que le groupe fondamental de $\mathbf{R}^2-$ A est isomorphe à F(A).

2) Soit A l’ensemble des points de $\mathbf{R}^2$ de coordonnées $(1/n,0)$, pour $n\in \mathbf{N}^*$. Montrer que le groupe fondamental de $\mathbf{R}^2-$ A a la puissance du continu. Il n’est en particulier pas isomorphe au groupe F(A).

3) Soit $((X_i, x_i))_{i\in I}$ une famille d’espaces topologiques pointés ; notons $(X, x)$ le bouquet de cette famille (IV, p. 421, exemple 4). Supposons que, pour tout $i\in I$, le point $x_i$ soit fermé dans $X_i$ et possède un système fondamental de voisinages V tel que le groupe $\pi_1(V, x_i)$ soit réduit à l’élément neutre. Alors, l’homomorphisme canonique $_i*_{\in I}\pi_1(X_i, x_i)\rightarrow \pi_1(X, x)$ est un isomorphisme.

4) Soit P le sous-espace de $\mathbf{R}^2$ défini comme dans l’exercice 5, I, p. 146, b). Soit $a$ le point $(0,0,1)$ de $\mathbf{R}^3$ et soit C la réunion des segments $[a,(x,0)]$, pour $x\in P$.

a) Démontrer que l’espace C est localement connexe par arcs et simplement connexe par arcs.

b) Soit D la réunion de l’espace C et de son symétrique $-C$. Démontrer que l’espace D est simplement connexe, mais qu’il n’est pas simplement connexe par arcs.

c) Démontrer que le groupe de Poincaré $\pi_1(D,0)$ a la puissance du continu.

5) Soit P le sous-espace de $\mathbf{R}^2$ défini comme dans l’exercice 5, I, p. 146, b) ; notons aussi $P^+$ (resp. $P^-)$ l’ensemble des points $(x, y)\in P$ tels que $y\geqslant 0$ (resp. $y\leqslant 0$). Soit $a$ le point $(0,0,1)$ de $\mathbf{R}^3$ et soit A la réunion du segment $[a,0]$ et des segments $[a,(2r_n,0)]$, pour $n\in \mathbf{N}$, On pose $B^+= (P^+\times  \{0\})\cup A$, $B^-= (P^-\times  \{0\})\cup A$ et $B = (P\times  \{0\})\cup A$.

a) Démontrer que l’espace $B^+$ est délaçable et que le groupe de Poincaré $\pi_1(B^+, a)$ est un groupe libre sur $\mathbf{N}$.

b) Démontrer que A est contractile en $a$.

c) Démontrer que l’homomorphisme canonique de $\pi_1(B^+, a)*\pi_1(B^-, a)$ dans $\pi_1(B, a)$, déduit des inclusions canoniques de $B^+$ et $B^-$ dans B, n’est pas surjectif.

6) Soit X la droite numérique $\mathbf{R}$ et soit A une partie de X. Soit Y l’espace déduit de X par contraction de A en un point.

a) Si A est discret, le groupe de Poincaré de Y est un groupe libre.

b) Si A a un point d’accumulation, le groupe de Poincaré de Y a la puissance du continu et n’est pas libre.

c) Si A est l’adhérence de l’ensemble des points $1/n$, pour $n\in \mathbf{N}^*$, l’espace $X/A$ est homéomorphe à la boucle d’oreille hawaïenne.

7) Soit G un graphe, S l’ensemble de ses sommets et A l’ensemble de ses arêtes orientées. On note $|G|$ sa réalisation géométrique ; on identifie S à une partie de $|G|$ et on note $p:\mathbf{I}\times A\rightarrow  |G|$ l’application canonique.

a) Démontrer que l’espace $|G|$ est compact (resp. localement compact) si et seulement si le graphe G est fini (resp. localement fini).

b) Démontrer que l’application canonique de S dans $|G|$ induit une bijection de $\pi_0(G)$ sur $\pi_0(|G|)$.

c) Notons $\varpi (|G|)_S$ le sous-groupoïde plein de $\varpi (|G|)$ d’ensemble de sommets S. Démontrer qu’il existe un unique isomorphisme de groupoïdes $\varpi (G)\rightarrow \varpi (|G|)_S$ qui est l’identité sur l’ensemble des sommets et qui applique la classe d’une arête orientée $a\in A$ sur la classe du chemin $t\mapsto p(t, a)$

d) On suppose que le graphe G est connexe et fini ; soit $m= 1 +$ Card(S) $-$ Card(A). Démontrer que le groupe de Poincaré de $|G|$ est un groupe libre à $m$ générateurs.

8) Soit X l’espace quotient de l’espace $\mathbf{R}\times  \{0,1\}$ par la relation d’équivalence la moins fine qui identifie $(x,0)$ et $(x,1)$ pour tout $x\in \mathbf{R}^*$ (« droite numérique dont l’origine est dédoublée »).

a) Démontrer que $\pi_1(X, x)$ est isomorphe à $\mathbf{Z}$, pour tout point $x\in X$.

b) Soit X[^2] l’espace quotient de l’espace $X^2$ par l’opération du groupe symétrique $\mathfrak{S}_2$ sur l’espace $X^2$ agissant par permutation des coordonnées. Démontrer que $\pi_1(X$[^2]$, y) = 0$ pour tout $y\in X$[^2].

9) Soit X un espace topologique, soit R une relation d’équivalence dans X et soit $p: X\rightarrow X/R$ la surjection canonique. Soit $x\in X$.

a) On suppose que X est connexe et localement connexe par arcs, que les classes d’équivalence sont des ensembles connexes, et que l’espace $X/R$ est délaçable. Démontrer que l’homomorphisme $p_*:\pi_1(X, x)\rightarrow \pi_1(X/R, p(x))$ est surjectif.

b) On suppose que $X =\mathbf{I}$ et que $\{0,1\}$ est la seule classe d’équivalence qui ne soit pas réduite à un élément. Démontrer que l’homomorphisme $p_*$ n’est pas surjectif.

10) Soit W le cercle de Varsovie, défini dans l’exercice 1, IV, p. 455, dont on reprend les notations.

a) Soit R la relation d’équivalence dans W dont les seules classes non réduites à un seul élément sont B et S ; soit $p: W\rightarrow W/R$ la surjection canonique. Démontrer que l’espace quotient $W/R$ est homéotope, mais pas homéomorphe, au cercle $\mathbf{S}_1$. Démontrer que l’homomorphisme $p_*$ n’est pas surjectif.

b) Soit $R'$ la relation d’équivalence dans W dont $B\cup S$ est la seule classe d’équivalence non réduite à un élément ; soit $p': W\rightarrow W/R'$ la surjection canonique. Démontrer que l’espace $W/R'$ est homéomorphe à $\mathbf{S}_1$, que l’homomorphisme $p_*$ n’est pas surjectif, mais que les classes d’équivalences de $R'$ sont connexes.

11) Soit X un espace topologique connexe par arcs et soit $f: X\rightarrow X$ un homéomorphisme. Soit T l’espace quotient de $X\times \mathbf{I}$ par la relation d’équivalence la plus fine pour laquelle les points $(x,0)$ et $(f(x),1)$ sont équivalents, pour tout $x\in X$. On note $p: X\times \mathbf{I}\rightarrow T$ l’application canonique ; on note $j: X\rightarrow T$ l’application donnée par $x\mapsto p(x,1/2)$. Soit $a$ un point de X, soit $c\in \Lambda_{f(a),a}(X)$ un chemin d’origine $f(a)$ et de terme $a$, et soit $\gamma = [c]$.

a) Démontrer que l’application de $\mathbf{I}$ dans T donnée par $t\mapsto p(a,^1_2-t)$ pour $t\in [0,^1_2]$ et $t\mapsto p(c(2t-1),^3_2-t)$ pour $t\in ]^1_2,1]$ est un lacet en $j(a)$ dans T. On note $\delta$ sa classe.

b) Soit $\mathsf{S}$ l’unique homomorphisme de groupes de $\pi_1(X, a)*\mathbf{Z}$ dans $\pi_1(T, j(a))$ qui applique une classe $v\in \pi_1(X, a)$ sur $j_*(v)$ et l’élément $t= 1$ de $\mathbf{Z}$ sur la classe $\delta$. Démontrer que l’homomorphisme $\mathsf{S}$ est surjectif et que son noyau est le plus petit sous-groupe distingué qui contient les éléments $vt(\gamma^{-1}f_*(v)\gamma )^{-1}t^{-1}$, pour $v\in \pi_1(X, a)$.

c) Pour $v\in \pi_1(X, a)$, on pose $\varphi (v) =\gamma^{-1}f_*(v)\gamma$; démontrer que $\varphi$ est un automorphisme du groupe $\pi_1(X, a)$. Soit $\varphi :\mathbf{Z}\rightarrow$ Aut($\pi_1(X, a)$) l’unique homomorphisme de groupes qui applique 1 sur $\varphi$. Construire un isomorphisme du groupe $\pi_1(T, j(a))$ sur le produit semi-direct externe de $\mathbf{Z}$ par $\pi_1(X, a)$ relativement à $\varphi$.

12) a) Soit D une droite de $\mathbf{R}^3$ et soit $U =\mathbf{R}^3-$ D. Démontrer que U est connexe par arcs et que pour tout point $a\in U$, le groupe $\pi_1(U, a)$ est isomorphe à $\mathbf{Z}$.

b) Soit P un plan de $\mathbf{R}^3$, soit C un cercle contenu dans P et soit $V =\mathbf{R}^3-$ C. Démontrer que V est connexe par arcs et que, pour tout point $a\in V$, le groupe $\pi_1(V, a)$ est isomorphe à $\mathbf{Z}$. (Appliquer le théorème de van Kampen au recouvrement fermé de $\mathbf{R}^3$ formé des deux demi-espaces délimités par P; on peut aussi remarquer que les espaces U et V sont homéomorphes.)

13) Soient D et $D'$ deux droites de $\mathbf{R}^3$, distinctes, et soit $U =\mathbf{R}^3-(D\cup D')$. a) Démontrer que U est connexe par arcs.

b) On suppose que D et $D'$ sont disjointes ; démontrer que, pour tout point $a\in U$, le groupe $\pi_1(U, a)$ est un groupe libre à deux générateurs.

c) On suppose que D et $D'$ ont un point commun ; démontrer que, pour tout point $a\in U$, le groupe $\pi_1(U, a)$ est un groupe libre à trois générateurs.

14) Soit P un plan de $\mathbf{R}^3$, soit C un cercle contenu dans P et soit D une droite de $\mathbf{R}^3$. Soit $U =\mathbf{R}^3-(C\cup D)$ et soit $a$ un point de U.

a) Démontrer que U est connexe par arcs.

b) On suppose que D ne rencontre pas l’enveloppe convexe de C. Démontrer que $\pi_1(U, a)$ est un groupe libre à deux générateurs.

c) On suppose que D ne rencontre pas C mais qu’elle rencontre l’enveloppe convexe de C. Démontrer que $\pi_1(U, a)$ est isomorphe à $\mathbf{Z}^2$. d) On suppose que D rencontre C en un unique point. Démontrer que $\pi_1(U, a)$ est un groupe libre à deux générateurs.

e) On suppose que D rencontre C en deux points. Démontrer que $\pi_1(U, a)$ est un groupe libre à trois générateurs.

15) On dit qu’un espace topologique X possède la propriété de Phragmén-Brouwer s’il est connexe et si, pour tout couple $(A,B)$ de parties fermées de X, disjointes, telles que X-A et X-B soient connexes, alors $X-(A\cup B)$ est connexe.

a) Soit X un espace topologique localement connexe qui possède la propriété de Phragmén-Brouwer. Soit $(A,B)$ un couple de parties fermées de X, disjointes, soit $(a, b)$ un couple de points de $X-(A\cup B)$ qui appartiennent à une même composante connexe de X-A (resp. de X-B). Démontrer que $a$ et $b$ appartiennent à une même composante connexe de $X-(A\cup B)$.

b) Soit X un espace topologique connexe et localement connexe par arcs qui ne possède pas la propriété de Phragmén-Brouwer. Démontrer que, pour tout point $x\in X$, il existe un homomorphisme surjectif de $\pi_1(X, x)$ dans $\mathbf{Z}$. c) Soit X un espace topologique connexe et localement connexe par arcs qui est simplement connexe par arcs. Démontrer que X possède la propriété de Phragmén-Brouwer.

d) Soit X un espace topologique séparé et localement connexe tel que, pour tout point $x\in X$, l’espace X$-\{x\}$ possède la propriété de Phragmén-Brouwer. Soit A une partie de X qui est homéomorphe à $[0,1]$; démontrer que X-A est connexe. (Soit $c:\mathbf{I}\rightarrow A$ un homéomorphisme. Raisonner par l’absurde et construire une suite $(J_n)$ où, pour tout $n,J_n$ est un intervalle de $\mathbf{I}$ de longueur $2^{-n}$, contenu dans $J_{n-1}$ si $n\geqslant 1$, tel que X $-c(J_n)$ ne soit pas connexe ; soit $x$ l’unique point de X commun à tous les ensembles $c(J_n)$. Démontrer alors que X $-\{x\}$ n’est pas connexe.)

e) Soit $n$ un entier $\geqslant 1$ et soit A une partie de $\mathbf{S}_n$ qui est homéomorphe à $[0,1]$. Démontrer que $\mathbf{S}_n-$ A est connexe.

16) Soit A une partie de $\mathbf{S}_2$ qui est homéomorphe à $\mathbf{S}_1$. Soient $a$ et $b$ des points distincts de A, on note $A'$ et $A''$ les composantes connexes de A$-\{a, b\}$ et l’on pose $X =\mathbf{S}_2-\{a, b\},U = X-A'$ et $V = X-A''$.

a) Démontrer que U et V sont connexes. (Utiliser l’exercice 15.)

b) Démontrer que, pour tout point $x\in U$, l’homomorphisme de $\pi_1(U, x)$ dans $\pi_1(X, x)$ déduit de l’inclusion de U dans X est trivial.

c) Démontrer que $\mathbf{S}_2-$ A possède exactement deux composantes connexes et que leur frontière est égale à A. d) Soit S une partie de $\mathbf{R}^2$ qui est homéomorphe à $\mathbf{S}_1$; démontrer que $\mathbf{R}^2-$ S possède exactement deux composantes connexes et que leur frontière est égale à S (théorème de Jordan).

17) On identifie $\mathbf{S}_1$ à l’ensemble des nombres complexes de module 1, et la sphère $\mathbf{S}_3$ au sous-espace de $\mathbf{C}^2$ formé des points $(z, w)$ tels que $|z|^2+|w|^2= 1$. Soient B et C les sous-espaces de $\mathbf{S}_3$ définis par $|z|\leqslant |w|$ et $|z|\geqslant |w|$ respectivement.

a) Démontrer que B et C sont homéomorphes à $\mathbf{B}_2\times \mathbf{S}_1$.

b) Pour tout couple $(m, n)$ d’entiers relatifs premiers entre eux, on note $K_{m,n}$ l’image de l’application de $\mathbf{S}_1$ dans $\mathbf{S}_3$ donnée par $u\mapsto (u^m, u^n)$ (« nœud torique »).

c) Démontrer que $\mathbf{S}_3-K_{m,n}$ est connexe et que son groupe fondamental admet une présentation $\langle x, y;x^m=y^n\rangle$.

d) Démontrer qu’il existe un homéomorphisme $\varphi$ de $\mathbf{S}_3$ dans lui-même tel que $\varphi (K_{m,n}) = K_{1,0}$ si et seulement si $|m|\leqslant 1$ ou $|n|\leqslant 1$.

18) Soit $(m, n)$ un couple d’entiers naturels tels que $1< m < n$. Soit G le groupe défini par la présentation $\langle x, y;x^m=y^n\rangle$. Soit $z=x^m$ et soit C le sous-groupe de G engendré par $z$.

a) Démontrer que C est contenu dans le centre de G.

b) Démontrer que $G/C$ est isomorphe au produit libre $(\mathbf{Z}/m\mathbf{Z})*(\mathbf{Z}/n\mathbf{Z})$.

c) En déduire que C est le centre de G.

d) Soit $(p, q)$ un couple d’entiers naturels tels que $1< p < q$. On suppose que le groupe $G'$ défini par la présentation $\langle x, y;x^p=y^q\}$ est isomorphe à G. Démontrer que $(p, q) = (m, n)$.

e) Démontrer que le quotient de G par son groupe dérivé est isomorphe à $\mathbf{Z}$.

19) Soit G un graphe ; notons S l’ensemble de ses sommets, A celui de ses arêtes orientées et $|G|$ sa réalisation géométrique. Notons $j: S\rightarrow  |G|$ et $p:\mathbf{I}\times A\rightarrow  |G|$ les applications canoniques. On suppose que les ensembles S et A sont finis.

On dit qu’une application $f:|G| \rightarrow \mathbf{R}^n$ est affine (resp. affine par morceaux) si pour toute arête $a\in A$, l’application $t\mapstochar \rightarrow f\circ p(a, t)$ est affine (resp. affine par morceaux). (Cf. III, p. 331, exerc. 6.)

a) Démontrer qu’il existe une application injective et affine par morceaux de $|G|$ dans $\mathbf{R}^3$. (Commencer par démontrer qu’il existe un entier $n\geqslant 1$ et une application injective et affine par morceaux de $|G|$ dans $\mathbf{R}^n.)$ b) Pour toute application continue injective $f:|G| \rightarrow \mathbf{R}^n$, démontrer qu’il existe une application continue injective $g:|G| \rightarrow \mathbf{R}^n$ qui est affine par morceaux et homotope à $f$.

c) On suppose que l’application $(o, t): A\rightarrow S\times S$ est injective. Soit $f$ une application injective de S dans $\mathbf{R}$. Démontrer qu’il existe une unique application affine F de $|G|$ dans $\mathbf{R}^3$ qui applique tout sommet $s\in S$ sur le point $(f(s), f(s)^2, f(s)^3)$ de $\mathbf{R}^3$. Démontrer que F est injective.

On dit que le graphe G est planaire s’il existe une application continue injective de $|G|$ dans $\mathbf{R}^2$.

d) On suppose que le graphe G est planaire et que l’application $(o, t): A\rightarrow$ $S\times S$ est injective. Soit $f:|G| \rightarrow \mathbf{R}^2$ une application continue injective. Démontrer qu’il existe une application affine injective $g:|G| \rightarrow \mathbf{R}^2$ qui est homotope à $f$.

20) Soit $f:\mathbf{I}\rightarrow \mathbf{R}^2$ un lacet affine par morceaux dont la restriction à $[0,1[$ est injective ; notons $C =f(\mathbf{I})$.

a) Démontrer que $\mathbf{R}^2-$ C a au plus deux composantes connexes.

b) Pour $x\in \mathbf{R}^2-$ C et $v\in \mathbf{S}_1$, on note $n_v(x)$ le nombre de composantes connexes de $(\mathbf{R}^2-C)\cap (x+\mathbf{R}_+v)$. Démontrer qu’il existe une unique application localement constante $n:\mathbf{R}^2-C\rightarrow  \{0,1\}$ telle que $n(x)\equiv n_v(x)$ (mod$.2)$ pour tout $v\in \mathbf{S}_1$.

c) En déduire que $\mathbf{R}^2-$ C possède exactement deux composantes connexes et que leurs frontières sont égales à C.

d) Soit $g:\mathbf{I}\rightarrow \mathbf{R}^2$ une application affine par morceaux, injective telle que $^-g^1(C) =\{0,1\}$; on pose $P =g(\mathbf{I})$ et $D = C\cup P$. Démontrer que $C-(C\cap P)$ possède deux composantes connexes ; notons-les $P_1$ et $P_2$. Démontrer que $\mathbf{R}^2-$ D possède trois composantes connexes et que leurs frontières sont égales à C, $P_1\cup P$ et $P_2\cup P$.

e) Soit G un graphe fini planaire ; soit S l’ensemble de ses sommets et A l’ensemble de ses arêtes orientées. Soit $f:|G| \rightarrow \mathbf{R}^2$ une application continue injective affine par morceaux et soit P son image. Démontrer que le nombre de composantes connexes de $\mathbf{R}^2-$ P est égal à 1 + Card(S) $-$ Card(A) + Card($\pi_0(G)$).

21) Soit K le graphe associé au carquois dont l’ensemble des sommets est $\{1,2,3\} \times  \{0,1\}$, l’ensemble des flèches est l’ensemble des couples de la forme $((a,0),(b,1))$, pour $a, b\in  \{1,2,3\}$, et dont les applications origine et terme sont respectivment déduites de la première et de la seconde projection (« graphe de Kuratowski »). Démontrer que le graphe K n’est pas planaire.

22) Soit $n$ un entier naturel et soit $K_n$ un graphe complet dont l’ensemble des sommets est de cardinal $n($II, p. 220, exerc. 5).

a) Démontrer que les graphes $K_n$, pour $1\leqslant n\leqslant 4$, sont planaires.

b) Démontrer que le graphe $K_5$ n’est pas planaire.

23) Soient $u$ et $v$ deux points de $\mathbf{S}_1$ tels que $\mathscr{I}(v/u)>0$ ; on définit une famille $(a_j)_{j\in\mathbf{Z}/4\mathbf{Z}}$ par $a_1=u,a_2=v,a_3=-u$ et $a_4=-v$. Notons $Q_1$ et $Q_2$ les deux segments $[a_1, a_3]$ et $[a_2, a_4]$ dans le disque unité $\mathbf{B}_2$ et posons $Q = Q_1\cup Q_2$.

a) Démontrer que, pour tout $j\in \mathbf{Z}/4\mathbf{Z}$, il existe une unique composante connexe par arcs $A_j\in \pi_0(\mathbf{B}_2-$ Q) dont l’adhérence contient $a_j$ et $a_{j-1}$. Démontrer que la réunion de la famille $(A_j)$ est égale à $\mathbf{B}_2-$ Q.

Posons $C =\mathbf{B}_2\times [-1,1]$, $N = (0,0,1)$ et $S = (0,0,-1)$. Soit $f: [-1,1]\rightarrow$ $\mathbf{R}_+$ une application continue telle que $f(-1) =f(1) = 0$ et $0< f(t)<1$ pour tout $t\in ]-1; 1[$. Notons alors $L_1$ et $L_2$ les images des applications de $[-1,1]$ dans C données par $t\mapsto (ta_1,0)$ et $t\mapsto (ta_2, f(t))$ respectivement ; on pose enfin $L = L_1\cup L_2$.

b) Démontrer que C-L est connexe par arcs.

c) On dit qu’un chemin $c$ dans C-L, d’origine N et de terme S, est franc s’il existe des chemins juxtaposables $c_1$ et $c_2$ dans $\mathbf{B}_2$ tels que $c$ soit le chemin juxtaposé des chemins donnés par $t\mapsto (c_1(t),1),t\mapsto (c_1(1),1-2t)$ et $t\mapsto$ $(c_2(t),-1)$. Démontrer qu’alors $c_1(1)\notin Q$; on note $A_c$ la composante connexe par arcs de $\mathbf{B}_2-$ Q qui contient ce point.

d) Soient $c$ et $c'$ des chemins dans C-L, d’origine N et de terme S ; supposons qu’ils soient francs. Démontrer qu’ils sont strictement homotopes si et seulement si $A_c= A_{c'}$.

e) Pour tout $j\in \mathbf{Z}/4\mathbf{Z}$, soit $c_j$ un chemin dans C-L, d’origine N et de terme S, franc et tel que $A_{c_j}= A_j$. Démontrer la relation

$$
[c_1][c_4]^{-1}= [c_2][c_3]^{-1}
$$

dans le groupe $\pi_1(C-L,N)$.

f) Démontrer que l’homomorphisme canonique du groupe libre à deux générateurs $x, y$ dans $\pi_1(C-L,N)$ qui applique $x$ et $y$ sur $[c_1][c_2]^{-1}$ et $[c_2][c_3]^{-1}$ respectivement est un isomorphisme de groupes. (Appliquer le théorème de van Kampen au recouvrement de C - L formé des huit ensembles fermés délimités par les trois plans vectoriels de $\mathbf{R}^3$ contenant deux des points de l’ensemble $\{a_1, a_2,N\}.)$

24) Soit $m$ un entier $\geqslant 1$ et soit $(\theta_j)_{1\leqslant j\leqslant m}$ une suite de nombres réels telle que $0\leqslant \theta_1< \theta_2<\cdots < \theta_n<2\pi$. Pour $j\in \mathbf{Z}/m\mathbf{Z}$, on pose $a_j=$ exp($i\theta_k$), où $k$ est l’unique élément de $\{1, . . . , n\}$ appartenant à la classe $j$; on note aussi $Q_j$ le segment $[0, a_j]$ de $\mathbf{B}_2$. On pose enfin $Q = Q_1\cup  \cdots  \cup Q_m$.

a) Pour $j\in \mathbf{Z}/m\mathbf{Z}$, démontrer qu’il existe une unique composante connexe par arcs $A_j$ de $\mathbf{B}_2-$ Q qui contient tout point $b\in \mathbf{S}_1$ tel que $\mathscr{I}(b/a_j)>0$ et $\mathscr{I}(b/a_{j+1})<0$. Démontrer que la famille $(A_j)$ est formée d’ensembles deux à deux disjoints et que sa réunion est égale à $\mathbf{B}_2-$ Q.

b) On pose $C =\mathbf{B}_2\times [-1,1]$, $N = (0,0,1)$, $S = (0,0,-1)$, et $L = Q\times \{0\}$. On dit qu’un chemin dans C-L, d’origine N et de terme S, est franc s’il existe des chemins $c_1$ et $c_2$ dans $\mathbf{B}_2$, juxtaposables, tels que $c$ soit le chemin juxtaposé des chemins donnés par $t\mapsto (c_1(t),1),t\mapsto (c_1(1),1-2t)$ et $t\mapsto (c_2(t),-1)$. Démontrer qu’alors $c_1(1)\notin Q$; on note $A_c$ la composante connexe par arcs de $\mathbf{B}_2-$ Q qui contient ce point.

c) Soient $c$ et $c'$ des chemins dans C-L, d’origine N et de terme S ; supposons qu’ils soient francs. Démontrer qu’ils sont strictement homotopes si et seulement si $A_c= A_{c'}$.

d) Pour tout $j\in \mathbf{Z}/m\mathbf{Z}$, soit $c_j$ un lacet dans C-L, d’origine N et de terme S, qui est franc et tel que $A_{c_j}= A_j$. Démontrer que l’homomorphisme du groupe libre $F(\mathbf{Z}/m\mathbf{Z})$ dans $\pi_1(C-L,N)$ qui applique $x_j$ sur $[c_j][c_{j+1}]^{-1}$, pour $j\in \mathbf{Z}/m\mathbf{Z}$, est surjectif, et que son noyau est le plus petit sous-groupe distingué qui contient le produit $x_1x_2. . . x_m$.

25) On pose $C =\mathbf{B}_2\times [-1,1]$. Soit K un sous-espace fermé de $\mathbf{R}^3$ et soit P son image par la projection donnée par $(x, y, z)\mapsto (x, y)$. On suppose qu’il existe un ensemble fini I, une famille $(p_i)_{i\in I}$ de points de $\mathbf{R}^2$, une famille $(r_i)_{i\in I}$ de nombres réels strictement positifs et une famille $(m_i)_{i\in I}$ d’entiers naturels vérifiant les propriétés suivantes, où $\varphi_i$ désigne l’application de $\mathbf{R}^3$ dans $\mathbf{R}^3$ donnée par $x\mapsto (p_i,0) +r_ix$ et $C_i=\varphi_i(C)$ :

– Les ensembles $C_i$ sont deux à deux disjoints ;

– Pour tout $i\in I$, l’ensemble $L_i=^-\varphi^1_i(C_i\cap K)$ est le sous-espace L défini dans l’exercice 23 si $m_i= 0$ et dans l’exercice 24 (où l’on pose $m=m_i)$ si $m_i\geqslant 1$.

– L’ensemble $K'= K-\bigcup_i(\mathring{C}_i\cap K)$ est la réunion d’une famille finie de segments fermés deux à deux disjoints dans le plan $\mathbf{R}^2\times  \{0\}$.

Soient $N = (x_N, y_N, z_N)$ et $S = (x_S, y_S, z_S)$ des points de $\mathbf{R}^3$ tels que $z_N>$ sup($r_i$)$_{i\in I}$ et $z_S<-$ sup($r_i$)$_{i\in I}$.

a) On dit qu’un chemin $c$ dans $\mathbf{R}^3-$K d’origine N et de terme S est franc s’il existe des chemins $c_1$ et $c_2$ dans $\mathbf{R}^2$, juxtaposables, tels que $c$ soit le chemin juxtaposé des chemins donnés par $t\mapsto (c_1(t), z_N),t\mapsto (c_1(1),(1-t)z_N+tz_S)$, et $t\mapsto (c_2(t), z_S)$.

Démontrer qu’alors le point $c_1(1)$ n’appartient pas à P ; on note $A_c$ la composante connexe par arcs de $\mathbf{R}^2-$ P qui contient ce point. Démontrer que deux chemins francs $c$ et $c'$ sont strictement homotopes si et seulement si $A_c= A_{c'}$.

Pour toute composante connexe par arcs $\alpha$ de $\mathbf{R}^2-$ P, on fixe un chemin $c(\alpha )$ dans $\mathbf{R}^2-$ K, d’origine N et de terme S qui est franc et tel que $A_{c(\alpha)}=\alpha$.

b) Soit $i\in I$ tel que $m_i= 0$, de sorte que $^-\varphi^1_i(K\cap C_i)$ est l’ensemble L défini dans l’exercice 23, dont on reprend les notations ; on a $^-\varphi^1_i(P\times  \{0\} \cap$ $C_i) = Q\times  \{0\}$. Pour tout $j\in \mathbf{Z}/4\mathbf{Z}$, notons $\alpha_{i,j}$ la composante connexe par arcs de $\mathbf{R}^2-$ P qui contient l’image par $\varphi_i$ de la composante connexe $A_j$ de $\mathbf{B}_2-$ P. Démontrer que l’on a $[c(\alpha_{i,1})][c(\alpha_{i,4})]^{-1}= [c(\alpha_{i,2})][c(\alpha_{i,3})]^{-1}$ dans $\pi_1(\mathbf{R}^3-K,N)$.

c) Soit $\omega$ un élément de $\pi_0(\mathbf{R}^2-$ P). Soit $\lambda_{\omega}: F(\pi_0(\mathbf{R}^2-P))\rightarrow \pi_1(\mathbf{R}^3-K,N)$ l’unique homomorphisme de groupes qui, pour $\alpha \in \pi_0(\mathbf{R}^2-$ P), applique l’élément $x_{\alpha}$ sur $[c(\alpha )][c(\omega )]^{-1}$.

Démontrer que l’homomorphisme $\lambda_{\omega}$ est surjectif et que son noyau est le plus petit sous-groupe distingué de $F(\pi_0(\mathbf{R}^2-$ P)) qui contient l’élément $x_{\omega}$ et les éléments $x^{-1_1}_{\alpha_{i,}}x_{\alpha_{i,2}}x^{-1_3}_{\alpha_{i,}}x_{\alpha_{i,4}}$, pour $i\in I$ tel que $m_i= 0$.

d) Pour tout segment $s$ appartenant à $\pi_0(K')$, on choisit des éléments $\alpha_s$ et $\alpha '_s$ de $\pi_0(\mathbf{R}^2-$ P) tels que l’ensemble des composantes connexes de $\mathbf{R}^2-$ P dont l’adhérence contient $s$ soit égal à $\{\alpha_s, \alpha '_s\}$. Soit $\mu: F(\pi_0(K'))\rightarrow \pi_1(\mathbf{R}^3$ $K,N)$ l’unique homomorphisme de groupes qui, pour $s\in \pi_0(K')$, applique l’élément $x_s$ sur $[c(\alpha_s)][c(\alpha '_s)]^{-1}$. Démontrer que $\mu$ est surjectif. Pour $i\in I$ tel que $m_i= 0$ et $j\in  \{1,2,3,4\}$, on note $s_{i,j}$ l’unique segment de $\pi_0(K')$ tel que $\varphi_i(a_j)$ rencontre $s_{i,j}$. Prouver qu’il existe des éléments $u_i, v_i, w_i$ de $\{-1,1\}$ tels que $\mu(x_{s_{i,4}}) =\mu(x^w_{s_{i,}^i_2})$ et $\mu(x_{s_{i,3}}) =\mu(x^{-u_{2i}}_{s_{i,}}x^v_{s^i_{i,1}}x^u_{s_{i,}^i_2})$. Démontrer que le noyau de $\mu$ est le plus petit sous-groupe distingué de $F(\pi_0(K'))$ qui contient les éléments $x_{s_{i,3}}x^{-u_{2i}}_{s_{i,}}x^{-v_{1i}}_{s_{i,}}x^u_{s_{i,}^i_2}$ et $x_{s_{i,4}}x^{-w_{2i}}_{s_{i,}}$ pour $i\in I$.

e) On pose

1

$k=$ Card($\pi_0(K)$)$-$ Card($\{i\in I|m_i>0\}$) $+\sum m_i$.

$$
2_{i\in I}
$$

Prouver que $k\in \mathbf{N}$. Démontrer que le quotient de $\pi_1(\mathbf{R}^3-$ K) par son sous-groupe dérivé est isomorphe à $\mathbf{Z}^k$.

26) Dans le plan numérique $\mathbf{R}^2$, on note $D_0$ le disque de centre $(0,0)$ et de rayon 1 et $C_0$ sa frontière ; on pose $a_0= (-1,0)$. Soit $g$ un entier naturel $\geqslant 1$, soit $r$ un nombre réel strictement positif et soit $(v_1, . . . , v_g)$ une suite de nombres réels telle que $r <$ inf($v_1+ 1,(v_2-v_1)/2, . . . ,(v_g-v_{g-1})/2,1-v_g$). Pour tout $j\in  \{1, . . . , g\}$, on désigne par $D_j$ le disque fermé de centre $(0, v_j)$ et de rayon $r$ et par $C_j$ le cercle de centre $(0, v_j)$ et de rayon $r$; on pose aussi $a_j= (-r, v_j)$. Soit X l’espace D $-\bigcup^g_{j=1}\mathring{D}_j$.

Pour tout $j\in  \{1, . . . , j\}$, on note $u_j$ la classe dans $\varpi (X)$ d’un chemin d’origine $a_0$ et de terme $a_j$ dont l’image est le segment $[a_0, a_j]$; notons aussi $c_j\in \pi_1(X, a_j)$ la classe du lacet donné par $t\mapsto (-r$ cos(2$\pi t),-r$ sin(2$\pi t)+v_j)$ et $\gamma_j=u_jc_ju^{-1}_j$.

a) Soit $\gamma_0$ la classe du lacet dans X donné par $t\mapsto (-$ cos(2$\pi t),-$ sin(2$\pi t))$. Démontrer que l’on a $\gamma_0=\gamma_1. . . \gamma_g$.

b) Démontrer que l’unique homomorphisme du groupe libre à $g$ générateurs $x_1, . . . , x_j$ dans $\pi_1(X, a_0)$ qui applique $x_j$ sur $\gamma_j$ est un isomorphisme de groupes. (Appliquer le théorème de van Kampen au recouvrement de X défini par ses intersections avec les demi-plans $\mathbf{R}_+\times \mathbf{R}$ et $\mathbf{R}_-\times \mathbf{R}.)$

c) Soit $f: X\rightarrow \mathbf{R}_+$ une fonction continue telle que $^-f^1(0) =\bigcup^g_{j=0}C_j$ et soit Y le sous-espace de $\mathbf{R}^3$ formé des points $(x, y, z)$ tels que $z^2=f(x, y)$. On note $i_+$ (resp. $i_-)$ l’application continue de X dans Y donnée par $(x, y)\mapsto$ $(x, y,f(x, y))$ (resp. $(x, y)\mapsto (x, y,-f(x, y))$). Pour toute classe de chemin $\gamma$ dans X, on définit des classes de chemins dans $\varpi (Y)$ par $\gamma^+= (i_+)_*(\gamma )$ et $\gamma^-= (i_-)_*(\gamma )$.

Pour tout $j\in  \{1, . . . , g\}$, on définit enfin un élément de $\pi_1(Y, a_0)$ par $\delta_j=u^+_ju^-_j$. Démontrer que l’on a les relations $\gamma^+_j\delta_j=\delta_j\gamma_j^-$ pour $1\leqslant j\leqslant g$, et $\gamma_1^+. . . \gamma_g^+=\gamma_1^-. . . \gamma^-_g$.

d) Soit $\varphi$ l’unique homomorphisme d’un groupe libre F à $2g$ générateurs $x_1, . . . , x_g, y_1, . . . , y_g$ dans $\pi_1(Y, a_0)$ qui applique $x_j$ sur $\gamma_j^+$ et $y_j$ sur $\delta_j$. Démontrer que l’homomorphisme $\varphi$ est surjectif et que son noyau est le plus petit sous-groupe distingué de F qui contient l’élément

$$
(x^{-1}_1y_1x_1)(x^{-1}_2y_2x_2). . .(x^{-1}_gy_gx_g)(y_1. . . y_g)^{-1}
$$

(Appliquer le théorème de van Kampen au recouvrement de Y défini par ses intersections avec les demi-espaces $\mathbf{R}^2\times \mathbf{R}_+$ et $\mathbf{R}^2\times \mathbf{R}_-.)$

e) Soit $\varphi '$ l’unique homomorphisme d’un groupe libre F à $2g$ générateurs $x_1, . . . , x_g, y_1, . . . , y_g$ dans $\pi_1(Y, a_0)$ qui, pour tout $j$, applique $x_j$ sur

$$
(\gamma_1^+. . . \gamma_{j-1}^+)^{-1}\delta_j(\gamma_1^+. . . \gamma^+_{j-1})
$$

et $y_j$ sur $\gamma_j^+$. Démontrer que l’homomorphisme $\varphi '$ est surjectif et que son noyau est le plus petit sous-groupe distingué de F qui contient l’élément

$$
(x^{-1}_1y^{-1}_1x_1y_1). . .(x^{-1}_gy_g^{-1}x_gy_g)
$$

27) Soit D le disque unité dans $\mathbf{C}$ et soit X un sous-espace de D qui est un voisinage de $\mathbf{S}_1$. Soit R la relation d’équivalence la moins fine dans X qui, pour $u, v\in \mathbf{S}_1$, identifie les points $f(u)$ et $f(v)$ si $f(u) =f(v)$. Soit $p: X\rightarrow X/R$ la surjection canonique. Soit T un espace topologique compact et soit $f:\mathbf{S}_1\rightarrow T$ une application continue surjective. On pose $a=f(1)$ et on note $\alpha \in \pi_1(T, a)$ la classe du lacet $t\mapsto f(e^{2\pi it})$ dans T.

a) Démontrer qu’il existe une unique application $\sigma$ de T dans $X/R$ telle que $\sigma \circ f=p|_{\mathbf{S}_1}$. Démontrer que $\sigma$ définit un homéomorphisme de T sur son image $p(\mathbf{S}_1)$.

b) Soit $r$ un nombre réel tel que $0< r <1$ ; on suppose que X est l’ensemble des $z\in D$ tels que $r\leqslant |z|\leqslant 1$. Démontrer que $X/R$ est homéomorphe au cylindre de l’application $f$. En déduire que l’homomorphisme $\sigma_*$ est un isomorphisme de groupes de $\pi_1(T, a)$ sur $\pi_1(X/R, p(1))$.

c) On suppose que X = D. Démontrer que $X/R$ est homéomorphe au cône de l’application $f$. En déduire que l’homomorphisme de groupes $\sigma_*:\pi_1(T, a)\rightarrow \pi_1(X/R, p(1))$ est surjectif et que son noyau est le plus petit sous-groupe distingué de $\pi_1(T, a)$ qui contient $\alpha$.

d) Soit $r$ un nombre réel tel que $0< r <1$; soit $X_1$ l’ensemble des $z\in X$ tels que $|z|\leqslant r$ et $X_2$ l’ensemble des $z\in D$ tels que $r\leqslant |z|\leqslant 1$ ; on suppose que $X_2\subset X$. Soit $\beta \in \pi_1(X_2, r)$ la classe du lacet donné par $t\mapsto re^{2\pi it}$; soit $\delta \in \varpi_{p(r),p(1))}$ la classe du chemin donné par $t\mapsto p((1-t)r+t)$.

Démontrer qu’il existe un unique homomorphisme de groupes $\mu$ de $\pi_1(T, a)*\pi_1(X_2, r)$ dans $\pi_1(X/R, p(1))$ qui coïncide avec l’homomorphisme $\sigma_*$ dans $\pi_1(T, a)$ et avec l’homomorphisme $v\mapsto \delta^{-1}p_*(v)\delta$ dans $\pi_1(X_2, p(r))$. Démontrer que $\mu$ est surjectif et que son noyau est le plus petit sous-groupe distingué qui contient $\alpha \beta^{-1}$.

28) Soit X un espace topologique. On dit qu’une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ est une isotopie si, pour tout $t\in \mathbf{I}$, l’application $x\mapsto \sigma (x, t)$ déduite de $\sigma$ par passage au sous-espace est un homéomorphisme de X sur lui-même.

a) Soit $m$ un entier naturel et soit $f: X\rightarrow \mathbf{R}^n$ une application continue. Démontrer qu’il existe une isotopie dont l’origine est l’application identique de $X\times \mathbf{R}^n$ et dont le terme est l’application de $X\times \mathbf{R}^n$ dans $X\times \mathbf{R}^n$ donnée par $(x, y)\mapsto (x, y-f(x))$.

b) Soient A et B des sous-espaces de X; on dit que A est isotope à B s’il existe une isotopie $\sigma : X\times \mathbf{I}\rightarrow X$ dont l’origine est l’application identique de X et telle que $f(A\times  \{1\}) = B$.

Démontrer que la relation « A est isotope à B » est une relation d’équivalence dans l’ensemble des sous-espaces de X (resp. dans l’ensemble des sous-espaces fermés de X). c) Soient $m$ et $n$ des entiers naturels, soit A un sous-espace fermé de $\mathbf{R}^m$ et soit B un sous-espace fermé de $\mathbf{R}^n$. On suppose que A et B sont homéo-morphes. Démontrer que les sous-espaces $A\times  \{0\}$ et $\{0\} \times B$ de $\mathbf{R}^{m+n}$ sont isotopes.

29) Soit A une partie fermée de $\mathbf{R}^2$ homéomorphe à une partie fermée B de $\mathbf{R}$.

a) Démontrer que les sous-espaces $A\times  \{0\}$ et $\{(0,0)\} \times B$ de $\mathbf{R}^3$ sont isotopes.

b) On suppose que B $=\not\mathbf{R}$; démontrer que $\mathbf{R}^2-$ A est connexe par arcs. c) On suppose que $B =\mathbf{R}$; démontrer que $\mathbf{R}^2-$ A possède exactement deux composantes connexes par arcs et que A est la frontière de chacune d’elles. d) Soit A une partie de $\mathbf{S}_2$ homéomorphe à $\mathbf{S}_1$; démontrer que $\mathbf{S}_2-$ A possède exactement deux composantes connexes par arcs et que A est la frontière de chacune d’elles.

e) Soit A une partie de $\mathbf{R}^2$ homéomorphe à $\mathbf{S}_1$; démontrer que $\mathbf{R}^2-$ A possède exactement deux composantes connexes par arcs et que A est la frontière de chacune d’elles.

30) Soit $v= (v_1, . . . , v_n):\mathbf{R}^n\rightarrow \mathbf{R}^n$ une application de classe $C^1$ et soit $\delta$ un nombre réel $>0$ ; on fait les hypothèses suivantes :

– Le support de $v$ est contenu dans $[-\delta ,1 +\delta ]\times \mathring{\mathbf{B}}_{n-1}$;

– Pour tout $x\in [0,1-\delta [$, on a $v_1(x,0, . . . ,0)>0$, et $v_1(1,0, . . . ,0) = 0$;

– Pour tout $x\in [0,1]$, on a $v_2(x,0, . . . ,0) =\cdots =v_n(x,0, . . . ,0) = 0$. Soit $\Phi :\mathbf{R}^n\times \mathbf{R}\rightarrow \mathbf{R}^n$ le flot intégral de l’application $(x, t)\mapsto v(x)$ (VAR, 9.1.3) ; pour $t\in \mathbf{R}$, on note $\Phi_t$ l’application $x\mapsto \Phi (x, t)$.

a) Démontrer qu’il existe un nombre réel $\tau$ tel que $\Phi_{\tau}([0,1]\times  \{0\})\subset [1-$ $\delta ,1]\times  \{0\}$.

b) Soit $j: [-\delta ,1 +\delta ]\times \mathbf{B}_{n-1}\rightarrow \mathbf{R}^n$ une application continue injective. Pour tout $t\in [0,1]$, on pose $A_t=j([t,1]\times \{0\})$. Démontrer que, pour tout $t\in ]0,1[$, les sous-espaces $A_0$ et $A_t$ sont isotopes.

c) Soit P une partie de $\mathbf{R}^n$ homéomorphe à $[0,1]$ qui est la réunion d’une famille finie de segments. Démontrer que P est isotope à un segment.

31) Soit $f= (f_1, . . . , f_n):\mathbf{I}\rightarrow \mathbf{R}^n$ une application de classe $C^1$ telle que $f'(t)= 0\not$ pour tout $t\in \mathbf{I}$.

a) On fait l’hypothèse que $f_1'(t)>0$ pour tout $t\in \mathbf{I}$. Pour tout $j\in$ $\{2, . . . , n\}$, démontrer qu’il existe une application continue $g_j:\mathbf{R}\rightarrow \mathbf{R}$ telle que $f_j(x) =g_j(f_1(x))$ pour tout $x\in \mathbf{I}$. En déduire que $f(\mathbf{I})$ est isotope à un segment. b) Démontrer qu’il existe un nombre réel $\delta  >0$ et une application continue injective $j: [-\delta ,1 +\delta ]\times \mathbf{B}_{n-1}\rightarrow \mathbf{R}^n$ telle que $j(t,0) =f(t)$ pour tout $t\in \mathbf{I}$. Déduire de l’exercice 30 que, pour tout $\tau \in [0,1[$, l’ensemble $f(\mathbf{I})$ est isotope à $f([\tau ,1])$.

c) Démontrer que $f(\mathbf{I})$ est isotope à un segment.

32) Soit A une partie fermée de $\mathbf{R}^3$ homéomorphe à $[0,1]$. Les extrémités de A sont les deux points $p$ de A tels que A$-\{p\}$ soit connexe (cf. III, p. 280, th. 2) ; les autres points de A seront dits intérieurs.

Soit $p$ un point de A ; on dit que A est modéré en $p$ s’il existe un voisinage V de $p$ dans $\mathbf{R}^3$ et un homéomorphisme de V sur la boule unité de $\mathbf{R}^3$ qui applique $A\cap V$ sur un segment.

a) Soit $p$ un point de A tel que A soit modéré en $p$. Soit $(V_n)$ une suite décroissante de voisinages de $p$ dans $\mathbf{R}^3$ telle que $\bigcap_nV_n=\{p\}$; pour tout $n$, soit $a_n$ un point de $V_n-$ A et notons $j_n:\pi_1(V_n-A, a)\rightarrow \pi_1(V_1-A, a)$ l’homomorphisme de groupes déduit de l’injection de $V_n$ dans $V_1$. Si $p$ est une extrémité de A (resp. un point intérieur), démontrer qu’il existe un entier $m$ tel que pour tout entier $n\geqslant m$, l’image de l’homomorphisme $j_n$ soit réduite à l’élément neutre (resp. soit abélienne).

b) On suppose que A est modéré en tout point. Démontrer qu’il existe un homéomorphisme de $\mathbf{R}^3$ sur lui-même qui applique A sur un segment. En déduire que $\mathbf{R}^3-$ A est connexe et simplement connexe par arcs.

33) [^4] Soit L un sous-espace de$\surd \mathbf{R}^3$ comme défini dans l’exercice$\surd$ 23, où l’on prend $u= (1-i)/$ 2 et $v= (1 +i)/$ 2. Soient $a$ et $r$ des nombres réels tels que $0<2r < a <1-2r$. On pose $p_1= (0,-a),p_2= (0,0)$ et $p_3= (0, a);q_1= (-1,-a),q_2= (-1,0),q_3= (-1, a);q_1'= (1,-a)$, $q'_2= (1,0),q_3'= (1, a)$. Soit K la réunion des ensembles $p_1+rL,p_2+rL$, $p_3+rL$ et des segments $[q_1, p_1-rv]$, $[q_2, p_2-ru]$, $[q_3, p_3-ru]$, $[q'_1, p_1+ru]$, $[q'_2, p_3+ru]$, $[q'_3, p_3+rv]$.

Soit $(x_n)_{n\in\mathbf{Z}}$ une famille strictement croissante de nombres réels telle que $_{n\rightarrow -\infty}$lim $x_n=-1$ et $_{n\rightarrow}$lim$_{+\infty}x_n= 1$ ; pour $n\in \mathbf{Z}$, on pose $z_n=y_n= 1- |x_n|$. Pour $n\in \mathbf{Z}$, on note $f_n$ l’application de $[-1,1]^3$ dans $\mathbf{R}^3$ donnée par

$$
1-x1 +x
$$

$$
f_n(x, y, z) =(x_n, yy_n, zz_n) +(x_{n+1}, yy_{n+1}, zz_{n+1})
$$

2 2

et l’on pose $A_n=f_n(K)$ et $B_n=f_n([-1,1]^3)$. Soit A la réunion de la famille $(A_n)_{n\in\mathbf{Z}}$.

a) Démontrer que A est homéomorphe à $[0,1]$. b) Pour tout entier naturel $m$, on pose

$$
A'_m=\bigcup_{n<-m}B_n\cup \bigcup_{-m\leqslant n\leqslant m}A_m\cup \bigcup_{n>m}B_n
$$

Démontrer que $\mathbf{R}^3-A'_m$ est connexe par arcs et que son groupe fondamental est engendré par des éléments $a_n, b_n, c_n$ (pour $n\in \mathbf{Z}$ tel que $-m\leqslant n\leqslant m)$ sujets aux relations $b_{-m}=c_{-m}a_{-m},c_{n+1}a_{n+1}=c_nc_{n+1},c_{n+1}b_n=a_nc_{n+1}$, $b_nc_{n+1}=b_{n+1}b_n$ (pour $n\in \mathbf{Z}$ tel que $-m\leqslant n < m)$ et $c_ma_m=b_m$.

c) Démontrer que $\mathbf{R}^3-$ A est connexe par arcs et que son groupe fondamental est engendré par des éléments $a_n, b_n, c_n$ (pour $n\in \mathbf{Z})$ sujets aux relations

$$
b_n=c_na_n,c_{n+1}a_{n+1}=c_nc_{n+1},c_{n+1}b_n=a_nc_{n+1},b_nc_{n+1}=b_{n+1}b_n
$$

pour $n\in \mathbf{Z}$.

d) Démontrer qu’il existe un homomorphisme de $\pi_1(\mathbf{R}^3-$ A) dans le groupe $\mathfrak{S}_5$ qui applique la classe de $c_n$ sur la permutation $(1,2,3,4,5)\mapsto$ $(2,3,4,5,1)$ si $n$ est impair et sur la permutation $(1,2,3,4,5)\mapsto (4,3,5,2,1)$ si $n$ est pair. En déduire que $\mathbf{R}^3-$ A n’est pas simplement connexe par arcs.

34) Soit X un espace topologique connexe par arcs, soit G un groupe discret opérant continûment à gauche dans X. Soit M une partie ouverte de X telle que $G\cdot M = X$. On définit les ensembles S, T, le groupe F et l’homomorphisme de groupes $\varphi : F\rightarrow G$ comme dans la prop. 10 de I, p. 136. Soit $a$ un point de M.

a) Soit $c:\mathbf{I}\rightarrow X$ un lacet en $a$. Démontrer qu’il existe un unique élément $g(c)$ de F vérifiant la propriété suivante : pour tout entier $n$ et toute suite $(s_1, . . . , s_n)$ d’éléments de S tels que $c([(k-1)/n, k/n])\subset s_kM$ pour tout entier $k\in  \{1, . . . , n\}$, on a $g(c) =x_{s^-_n^1s_1}x_{s^-_1^1s_2}. . . x_{s^-_{n-}^1_1s_n}$.

b) Démontrer qu’il existe un unique homomorphisme de groupes $\gamma$ de $\pi_1(X, a)$ dans F tel que $\gamma ([c]) =g(c)$ pour tout lacet $c$ dans X en $a$.

c) Démontrer que le noyau de $\varphi$ est égal à l’image de l’homomorphisme $\gamma$. d) Démontrer que le noyau de $\gamma$ est engendré par la réunion des images des groupes $\pi_1(M\cup s\cdot M, a)$, pour $s\in S$.

§6

1) Soit K l’un des corps topologiques $\mathbf{R},\mathbf{C},\mathbf{H}$. Soit V un K-espace vectoriel possédant un système générateur dénombrable, muni de sa topologie la plus fine d’espace vectoriel topologique (EVT, I, §1, p. 11, cor. 4). Pour tout entier $n\geqslant 1$, on note $B_n(V)$ le sous-espace de $V^n$ formé des suites libres et $G_n(V)$ l’ensemble des sous-espaces de dimension $n$ de V. On note $p: B_n(V)\rightarrow$ $G_n(V)$ l’application qui associe à une suite $v\in B_n(V)$ le sous-espace vectoriel qu’elle engendre et on munit l’ensemble $G_n(V)$ de la topologie la moins fine pour laquelle l’application $p$ est continue.

a) Démontrer que l’on définit une action à droite du groupe $\mathbf{G}\mathbf{L}(n,K)$ dans $B_n(V)$ en posant $v\cdot g= (\sum^n_{i=1}v_ia_{i,j})_{1\leqslant j\leqslant n}$ pour $v= (v_1, . . . , v_n)\in$ $B_n(V)$ et $g= (a_{i,j})\in \mathbf{G}\mathbf{L}(n,K)$.

b) Démontrer que l’application $p$ induit un homéomorphisme de l’espace quotient $B_n(V)/\mathbf{G}\mathbf{L}(n,K)$ sur $G_n(V)$. En déduire que l’espace $G_n(V)$ est paracompact, et métrisable si V est de dimension finie.

c) Démontrer que $B_n(V)$ est un espace fibré principal de groupe $\mathbf{G}\mathbf{L}(n,K)$ et de base $G_n(V)$.

d) On suppose que V est de dimension infinie. Démontrer que l’espace $B_n(V)$ est contractile. En déduire que l’espace $G_n(V)$ est un espace classifiant pour le groupe $\mathbf{G}\mathbf{L}(n,K)$.

2) Soit H un espace préhilbertien séparé de dimension infinie. Soit $(e_i)_{i\geqslant 0}$ une famille orthonormale de vecteurs de H qui engendre un sous-espace dense de H. Pour tout entier $n\geqslant 1$, on note $V_n(H)$ le sous-espace de $H^n$ constitué des suites $(u_1, . . . , u_n)$ qui sont orthonormales.

a) Démontrer qu’il existe une application linéaire continue $T: H\rightarrow H$, et une seule, telle que $T(e_i) =e_{i+1}$ pour tout entier $i$. Démontrer que l’on a $\|T(x)\|=\|x\|$ pour tout $x\in H$.

b) Soit $H'$ le sous-espace de H formé des vecteurs orthogonaux à $e_i$, pour $i < n$. Démontrer que les conditions suivantes sont équivalentes : (i) $x$ et $T^n(x)$ sont linéairement dépendants ; (ii) $T(x) =x$; (iii) $x\in H'$.

c) Démontrer qu’il existe une unique homotopie $\sigma : V_n(H)\times \mathbf{I}\rightarrow V_n(H)$ telle que, pour tout $(u_1, . . . , u_n)\in V_n(H)$ et tout $t\in \mathbf{I},\sigma ((u_1, . . . , u_n), t)$ soit la suite déduite de la famille $(1-t)(u_1, . . . , u_n) +t(T^n(u_1), . . . ,T^n(u_n))$ par le procédé d’orthonormalisation (EVT, V, p. 23, prop. 6).

d) Démontrer qu’il existe une unique homotopie $\tau : V_n(H')\times \mathbf{I}\rightarrow V_n(H)$ telle que, pour tout $(u_1, . . . , u_n)\in V_n(H')$ et tout $t\in \mathbf{I},\sigma ((u_1, . . . , u_n), t)$ soit la suite déduite de la famille $(1-t)(u_1, . . . , u_n) +t(e_1, . . . , e_n)$ par le procédé d’orthonormalisation.

e) Démontrer que l’espace $V_n(H)$ est contractile.

3) Soit H un espace préhilbertien séparé. Soit $n$ un entier $\geqslant 1$ ; on note $V_n(H)$ le sous-espace de $H^n$ formé des suites orthonormales. Soit G un sous-groupe fermé de $O(n,\mathbf{R})$. a) Démontrer que l’on fait opérer le groupe orthogonal $O(n,\mathbf{R})$ (LIE, IX, §3, n$^o5$, p. 22) proprement et librement dans l’espace $V_n(H)$ par la formule

$$
(u_1, . . . , u_n)\cdot (a_{i,j}) =\sum_{i=1}^na_{i,j}u_i
$$

b) Soit G un sous-groupe fermé de $O(n,\mathbf{R})$. Prouver que la surjection canonique fait de $V_n(H)$ un espace fibré principal de groupe G et de base $V_n(H)/G$. (Commencer par traiter le cas où $G = O(n,\mathbf{R})$.)

c) Démontrer que l’espace quotient $V_n(H)/G$ est métrisable. (Munir $H^n$ de sa structure naturelle d’espace préhilbertien et considérer l’écart $d$ sur $V_n(H)$ donné par $d(u, v) =$ inf$_{g\in G}\|u-v\cdot g\|.)$

d) Démontrer que l’espace quotient $V_n(H)/G$ est un espace classifiant pour G.

e) En déduire que tout groupe de Lie compact possède un espace classifiant qui est un espace topologique métrisable. (Appliquer LIE, IX, §9, n$^o2$, p. 91, th. 1.)

4) En considérant un espace de Hilbert complexe, construire de manière analogue un espace classifiant métrisable pour le groupe unitaire $U(n,\mathbf{C})$ (LIE, IX, §, n$^o4$, p. 21)

5) a) Soit X un espace topologique paracompact. Démontrer que tout espace fibré principal de base X et de groupe $\mathbf{R}$ est trivialisable.

b) Soit X la demi-droite d’Alexandroff (TG, IV, p. 49, exerc. 12). Construire un espace fibré principal de base X et de groupe $\mathbf{R}$ qui n’est pas trivialisable.

6) Soit X l’espace quotient de l’espace $\mathbf{R}\times  \{0,1\}$ par la relation d’équivalence la plus fine pour laquelle les points $(t,0)$ et $(t,1)$ sont équivalents, pour tout $x\in \mathbf{R}^*_+$. On note $p:\mathbf{R}\times  \{0,1\} \rightarrow X$ la surjection canonique.

a) Démontrer que l’espace topologique X est homéotope à un point.

b) Pour quels points $x\in X$ l’espace pointé $(X, x)$ est-il contractile ?

c) Soit $U =p(\mathbf{R}\times  \{0\})$ et $V =p(\mathbf{R}\times  \{V\})$. Soit G un groupe topologique. Construire une bijection de l’ensemble $\mathscr{C}(\mathbf{R}^*_+; G)$ des applications continues de $\mathbf{R}^*_+$ dans G sur l’ensemble des classes d’isomorphisme de fibrés principaux de base X et de groupe G.

d) En déduire qu’il existe des fibrés principaux de base X et de groupe $\mathbf{R}$ qui ne sont pas trivialisables.

7) Soit G un groupe topologique et soit E un espace fibré principal de base $\mathbf{S}_2$ et de groupe G. On note $\mathbf{S}^+_2$ et $\mathbf{S}^-_2$ les deux hémisphères, intersections de $\mathbf{S}_2$ et des demi-espaces définis par les conditions $z\geqslant 0$ et $z\leqslant 0$ respectivement ; on identifie $\mathbf{S}^+_2\cap \mathbf{S}^-_2$ à $\mathbf{S}_1$.

a) Démontrer que le fibré E possède une section $s^+$ (resp. $s^-)$ au-dessus de $\mathbf{S}^+_2$ (resp. $\mathbf{S}^-_2)$. Démontrer qu’il existe une unique application continue $f:\mathbf{S}_1\rightarrow G$ telle que $s^+(x) =s^-(x)\cdot f(x)$ pour tout $x\in \mathbf{S}_1$.

b) Démontrer que la classe d’homotopie stricte de l’application de $\mathbf{S}_1$ dans G donnée par $x\mapsto c(x)c(1)^{-1}$ ne dépend pas du choix des sections $s^+$ et $s^-$; on la note $c(E)$.

c) Démontrer que deux espaces fibrés principaux E et $E'$, de base $\mathbf{S}_2$ et de groupe G, sont isomorphes si et seulement si $c(E) =c(E')$.

d) Démontrer que, pour toute classe $c\in \pi_1(G, e)$, il existe un espace fibré principal E, de base $\mathbf{S}_2$ et de groupe G tel que $c(E) =c$.

8) Soit X un espace topologique paracompact et soit S(X) sa suspension (I, p. 149, exerc. 1) ; on note $p: X\times [0,1]\rightarrow S(X)$ la surjection canonique. Soit $a$ un point de X.

a) Soit G un groupe topologique et soit E un espace fibré principal de groupe G et de base S(X). Démontrer que la restriction de E au sous-espace $p(X\times [0,1/2])$ admet une section continue $s_0$, et que la restriction de E au sous-espace $p(X\times [1/2,1])$ admet une section continue $s_1$.

b) Démontrer qu’il existe une unique application $f: X\rightarrow$ G telle que $s_1(x) =s_0(x)\cdot f(x)$ pour tout $x\in X$.

c) Démontrer que la classe d’homotopie stricte dans $[(X, a); (G, e)]$ de l’application pointée $x\mapsto f(x)f(a)^{-1}$ ne dépend pas du choix des sections $s_0$ et $s_1$; on la note $c(E)$.

d) Démontrer que deux espaces fibrés principaux E et $E'$, de base S(X) et de groupe G, sont isomorphes si et seulement si $c(E) =c(E')$.

e) Démontrer que, pour toute classe $c\in [(X, a); (G, e)$, il existe un espace fibré principal E, de base S(X) et de groupe G, tel que $c(E) =c$.

9) On identifie la droite projective complexe $\mathbf{P}^1(\mathbf{C})$ à l’ensemble des droites de $\mathbf{C}^2$. Soit E le sous-espace de $\mathbf{C}^2\times \mathbf{P}^1(\mathbf{C})$ formé des couples $((u, v), x)$ tels que $v\in x$ et $|u|^2+|v|^2= 1$. On munit E de l’action du groupe $\mathbf{S}_1$ donnée par $((u, v), x)\cdot z= ((zu, zv), x)$.

a) Démontrer que la seconde projection pr$_2: E\rightarrow \mathbf{P}^1(\mathbf{C})$ munit E d’une structure d’espace fibré principal de base $\mathbf{P}^1(\mathbf{C})$ et de groupe $\mathbf{S}_1$.

b) Soit $\varphi$ un homéomorphisme de $\mathbf{S}_2$ sur $\mathbf{P}^1(\mathbf{C})$; démontrer que le groupe $\pi_1(\mathbf{S}_1, e)$ est engendré par la classe $c(\varphi^*E)$.

[^1]: Les résultats de cet exercice et du suivant sont tirés de l’article de J. W. Cannon et G. R. Conner, « On the fundamental groups of one-dimensional spaces », Topology and its Applications **153** (2006), p. 2648–2672.
[^2]: Voir B. de Smit, « The fundamental group of the Hawaiian earring is not free », International Journal of Algebra and Computation, Vol. 2, No. 1 (1992), p. 33–37.
[^3]: Pour des exemples, voir l’article de R. L. Taylor, « Covering groups of nonconnected topological groups », Proc. Amer. Math. Soc **5** (1954), p. 753–768.
[^4]: Cet exemple est dû à E. Artin et R. Fox, « Some wild cells and spheres in three-dimensional space », Annals of Math. 49 (1948), p. 979–990.
