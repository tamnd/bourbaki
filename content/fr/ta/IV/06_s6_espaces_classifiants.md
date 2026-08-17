---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 6
section_title: Espaces classifiants
lang: fr
source: ta-i-iv-fr
book_pages: A IV.437-A IV.454, A IV.477-A IV.480
pdf_pages: 0453-0470, 0493-0496
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
exercises: 9
content_sha256: a2870b304efe50fc74eb2f4defc511a3177c203720e574519b617cf05e9df6e3
---

## § 6. ESPACES CLASSIFIANTS

### 1. Prolongement des homotopies

#### Proposition 1 {#ta-iv-s6-prop-1 .statement tag=023V}

Soit $X'$ un espace topologique normal, soit X un sous-espace de $X'$, soit A un sous-espace fermé de $X'$ contenu dans X et soit U un voisinage de A dans X.

Notons $i_A$ l’injection canonique de A dans X$,i_U$ l’injection canonique de U dans X ; notons $j_A$ et $j_U$ les injections correspondantes de Cyl($i_A$) et Cyl($i_U$) dans $X\times \mathbf{I}$.

Il existe une application continue $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) telle que $j_U\circ$ $r(x) =x$ pour tout point $x\in j_A$(Cyl($i_A$)).

Soit $U'$ un ouvert de $X'$ tel que $A\subset X\cap U'\subset U$. Par définition d’un espace normal (TG, IX, p. 41), il existe un voisinage ouvert $V'$ de A dans $X'$ tel que $A\subset V'\subset \overline{V'}\subset U'$ et une fonction continue $\varphi ': X'\rightarrow \mathbf{I}$ qui soit égale à 1 en tout point de A et à 0 en tout point de $\complement V'$. Posons $\varphi =\varphi '|X$ et $V = X\cap V'$. Notons aussi $\alpha : U\times \mathbf{I}\rightarrow$ Cyl($i_U$) et $\beta : X\rightarrow$ Cyl($i_U$) les applications canoniques (III, p. 238).

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

Soit $U'$ un voisinage ouvert de A dans $X'$ tel que $U'\cap X\subset U$. Comme l’espace $X'$ est normal, il existe un voisinage ouvert $V'$ de A dans $X'$ tel que $A\subset V'\subset \overline{V'}\subset U'$ (TG, IX, p. 41). Quitte à remplacer U par $\overline{V'}\cap X$, on peut ainsi supposer que U est fermé dans X. Reprenons alors les notations de la prop. 1 et de sa démonstration ; soit $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) une application continue telle que $j_U\circ r(x) =x$ pour tout point $x\in j_A$(Cyl($i_A$)).

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

Soit B un espace topologique paracompact et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré localement trivial. Posons $E_1=\overset{-1}{p}(B\times \{1\})$ et notons $p_1: E_1\rightarrow B$ l’application pr$_1\circ p|E_1$. Alors, les $B\times \mathbf{I}$-espaces $(E, p)$ et $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ sont isomorphes.

Démontrons d’abord deux lemmes.

#### Lemme 2 {#ta-iv-s6-lem-2 .statement tag=0243}

Soient $\alpha ,\beta ,\gamma$ des nombres réels tels que $\alpha \leqslant \beta \leqslant \gamma$, soit B un espace topologique et soit $p: E\rightarrow B\times [\alpha , \gamma ]$ une application continue. Posons $B_0= B\times [\alpha , \beta ]$, $B_1= B\times [\beta , \gamma ]$, $E_0=\overset{-1}{p}(B_0)$, $E_1=$ $\overset{-1}{p}(B_1)$ et notons $p_0: E_0\rightarrow B_0,p_1: E_1\rightarrow B_1$ les applications déduites de $p$. Si $(E_0, p_0)$ et $(E_1, p_1)$ sont des espaces fibrés trivialisables, il en est de même de $(E, p)$.

Soient $g_0: E_0\rightarrow B_0\times F_0$ et $g_1: E_1\rightarrow B_1\times F_1$ des trivialisations de $E_0$ et $E_1$ respectivement. Notons $g'_0$ et $g'_1$ les trivialisations du $B\times  \{\beta \}$-espace fibré $\overset{-1}{p}(B\times  \{\beta \})$ déduites de $g_0$ et $g_1$ par restriction. L’application $h=g'_0\circ (g'_1)^{-1}$ est un $B\times  \{\beta \}$-isomorphisme de $B\times  \{\beta \} \times F_1$ sur $B\times  \{\beta \} \times F_0$. On définit une application continue $h'$ de $B\times F_1$ dans $F_0$ en posant $h'(a, y) =$ pr$_3\circ h(a, \beta , y)$ pour $(a, y)\in B\times F_1$. Pour $(a, t, y)\in B\times [\beta , \gamma ]\times F_1$, posons $H(a, t, y) = (a, t, h'(a, y))$. L’application H ainsi définie est un $(B\times [\beta , \gamma ])$-isomorphisme de $B\times [\beta , \gamma ]\times F_1$ sur $B\times [\beta , \gamma ]\times F_0$, et l’on a $g_0|\overset{-1}{p}(B\times  \{\beta \}) = H\circ g_1|\overset{-1}{p}(B\times  \{\beta \})$. Il existe donc une application continue $g: E\rightarrow B\times [\alpha , \gamma ]\times F_0$ telle que $g|E_0=g_0$ et $g|E_1= H\circ g_1$. L’application $g$ est un isomorphisme de $B\times [\alpha , \gamma ]$-espaces, donc E est trivialisable.

#### Lemme 3 {#ta-iv-s6-lem-3 .statement tag=0244}

Soit B un espace topologique et soit $(E, p)$ un $B\times \mathbf{I}$-espace fibré localement trivial. Tout point $a$ de B possède un voisinage V tel que le $V\times \mathbf{I}$-espace $E_{V\times\mathbf{I}}$ soit trivialisable.

Soit $a$ un point de B; pour tout point $t$ de $\mathbf{I}$, il existe un voisinage ouvert $W_t$ de $t$ dans $\mathbf{I}$ et un voisinage $V_t$ de $a$ dans B tels que E soit trivialisable au-dessus de $V_t\times W_t$. Il existe alors un entier $n >0$ et, pour tout entier $i$ tel que 1 $\leqslant i\leqslant n$, un point $t_i$ de $\mathbf{I}$ tel que l’intervalle $[\frac{i-1}{n},\frac{i}{n}]$ soit contenu dans $W_{t_i}($III, p. 272, lemme 4). Posons $V =\cap_{1\leqslant i\leqslant n}V_{t_i}$. L’espace fibré E est trivialisable au-dessus de $V\times$ $[\frac{i-1}{n},\frac{i}{n}]$ pour tout entier $i$ tel que $1\leqslant i\leqslant n$. Le lemme 3 résulte alors du lemme 2 par récurrence sur $n$.

Démontrons maintenant la proposition. D’après le lemme 3, il existe un recouvrement ouvert $(U_j)_{j\in J}$ de B tel que, pour tout $j\in J$, E soit trivialisable au-dessus de $U_j\times \mathbf{I}$. Comme l’espace B est paracompact, on peut supposer le recouvrement $(U_j)_{j\in J}$ localement fini (TG, IX, p. 49) et choisir un recouvrement $(A_j)_{j\in J}$ de B où, pour tout $j\in J$, l’ensemble $A_j$ est fermé dans B et contenu dans $U_j$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1).

Pour toute partie ouverte U de B, notons $\mathscr{F}(U)$ l’ensemble des $U\times \mathbf{I}$-isomorphismes de $\overset{-1}{p}(U\times \mathbf{I})$ sur $\overset{-1}{p_{1}}(U)\times \mathbf{I}$ qui induisent l’application identique de $\overset{-1}{p}(U\times  \{1\})$ sur $\overset{-1}{p_{1}}(U)\times  \{1\}$. Pour tout couple $(V,U)$ d’ouverts de B tels que $U\subset V$, notons $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ l’application qui, à un $(V\times \mathbf{I})$-isomorphisme $g:\overset{-1}{p}(V\times \mathbf{I})\rightarrow \overset{-1}{p_{0}}(V)\times \mathbf{I}$, associe le $(U\times \mathbf{I})$-isomorphisme déduit de $g$ par passage aux sous-espaces. Le couple $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ est un faisceau sur B (I, p. 45, exemple 4). Pour démontrer la proposition, il suffit de démontrer que le faisceau $\mathscr{F}$ est mou (I, p. 64).

Soit $j\in J$, soit A une partie fermée de $A_j$, soit V un ensemble ouvert dans B tel que $A\subset V\subset U_j$ et soit $g$ un élément de $\mathscr{F}(V)$. Il existe un voisinage ouvert W de A tel que $\overline{W}\subset V$, car un espace paracompact est normal (TG, IX, p. 49, prop. 4). Nous allons démontrer qu’il existe un élément $g'$ de $\mathscr{F}(U_j)$ tel que $g'|W =g|W$. Le corollaire 2 (I, p. 65) de la prop. 6 entraîne alors que le faisceau $\mathscr{F}$ est mou.

Comme le $B\times \mathbf{I}$-espace E est trivialisable au-dessus de $U_j\times \mathbf{I}$, nous pouvons supposer que $\overset{-1}{p}(U_j\times \mathbf{I}) = U_j\times \mathbf{I}\times F$, où F est un espace topologique. L’élément $g$ de $\mathscr{F}(V)$ est alors un $V\times \mathbf{I}$-isomorphisme de $V\times \mathbf{I}\times F$ sur lui-même qui induit l’application identique de $V\times$ $\{1\}\times F$. Appliquons le cor. 5 de IV, p. 439, aux espaces $X'= X$, $X = U_j$, A = W, U = V, et Y = Z = F, à l’application $g: V\times \mathbf{I}\times F\rightarrow V\times \mathbf{I}\times F$ et à l’application identique de $U_j\times  \{1\} \times F$. Il existe donc un $U_j\times \mathbf{I}$-isomorphisme $g'$ de $U_j\times \mathbf{I}\times F$ sur lui-même qui induit l’application identique de $U_j\times  \{1\} \times F$ et qui coïncide avec $g$ sur $\overline{W}\times \mathbf{I}\times F$, et a fortiori sur $W\times \mathbf{I}\times F$. D’où la proposition.

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

Soit G un groupe topologique, soit B un espace topologique paracompact et soit $(E, p)$ un espace fibré principal de groupe G et de base $B\times \mathbf{I}$. Posons $E_1=\overset{-1}{p}(B\times \{1\})$ et soit $p_1: E_0\rightarrow B$ l’application pr$_1\circ p|E_1$. Alors, $(E, p)$ et $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ sont des espaces fibrés principaux de groupe G et de base $B\times \mathbf{I}$ isomorphes.

Soit F l’espace topologique G muni de l’opération à gauche du groupe $G\times G$ donnée par $(g, g')\cdot f=g'f g^{-1}$. Soit $(M, q)$ l’espace fibré localement trivial de base $B\times \mathbf{I}$ et de fibre-type F associé à l’espace fibré principal $E\times_{B\times\mathbf{I}}(E_1\times \mathbf{I})$ de groupe $G\times G$. Posons $M_1=\overset{-1}{q}(B\times \{1\})$ et $q_1=$ pr$_1\circ p|M_1$; le B-espace $(M_1, q_1)$ s’identifie à l’espace fibré localement trivial de fibre-type F associé à $E_1\times_BE_1$. D’après le lemme 4, où l’on prend pour espaces fibrés principaux E et $E'$ égaux à $E_1$, le B-espace $M_1$ possède une section. Comme les $B\times \mathbf{I}$-espaces $(M, q)$ et $(M_1\times \mathbf{I}, q_1\times$Id$_{\mathbf{I}})$ sont isomorphes (IV, p. 440, prop. 2), le $B\times \mathbf{I}$-espace $(M, q)$ possède une section, ce qui entraîne que les espaces fibrés principaux de groupe G, E et $E_1\times \mathbf{I}$, sont isomorphes.

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

Soit U une partie ouverte de B et soit $f':\overset{-1}{p}(U)\rightarrow E'$ une application continue qui est compatible avec les opérations de G dans $\overset{-1}{p}(U)$ et $E'$ respectivement. Il existe alors une unique application continue $f: U\rightarrow B'$ telle que $f\circ p_U=p'\circ f'$ et le carré commutatif

$$
E_U^{f'}E'
$$

$p_Up'$

U $^fB'$

est alors cartésien (I, p. 94, exemple (FP)).

Pour toute partie ouverte U de B, notons alors $\mathscr{F}(U)$ l’ensemble des applications continues $g: E_U\rightarrow E'$ qui sont compatibles avec les opérations de G dans $\overset{-1}{p}(U)$ et $E'$ respectivement. Pour tout couple $(U,V)$ d’ouverts de B tels que $U\subset V$, on note $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ l’application définie par $r_{UV}(g) =g|E_U$. On vérifie immédiatement que l’on a défini ainsi un faisceau $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ sur B. Nous appellerons ce faisceau le faisceau sur B des morphismes d’espaces fibrés principaux de groupe G de E dans $E'$.

#### Proposition 4 {#ta-iv-s6-prop-4 .statement tag=024G}

Si l’espace B est paracompact et si l’espace $E'$ est homéotope à un point, le faisceau sur B des morphismes d’espaces fibrés principaux de groupe G de E dans $E'$ est un faisceau mou.

Il existe un recouvrement ouvert $(U_j)_{j\in J}$ de B tel que, pour tout $j\in J$, l’espace fibré $E_{U_j}$ soit trivialisable. Comme l’espace B est paracompact, on peut supposer le recouvrement $(U_j)_{j\in J}$ localement fini (TG, IX, p. 49) et choisir un recouvrement $(A_j)_{j\in J}$ de B où, pour tout $j\in J$, l’ensemble $A_j$ est fermé dans B et contenu dans $U_j$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1).

D’après I, p. 65, cor. 2 de la prop. 6, il suffit, pour démontrer la proposition, d’établir l’assertion suivante : soit U une partie ouverte de B telle que l’espace fibré principal $(E_U, p_U)$ soit trivialisable, soit A une partie fermée de B contenue dans U, soit V un voisinage ouvert de A contenu dans U et soit $f$ un élément de $\mathscr{F}(V)$, il existe alors un voisinage ouvert W de A dans V et un élément $f'$ de $\mathscr{F}(U)$ tel que $r_{WU}(f') =r_{WV}(f)$. Démontrons cette assertion.

Soit W une partie ouverte de B telle que $A\subset W\subset \overline{W}\subset V$. Soit $s: U\rightarrow E_U$ une section de $(E_U, p_U)$. Appliquons le corollaire 3 (IV, p. 438) à l’espace B, au fermé $\overline{W}$ et au voisinage V de $\overline{W}$ et à l’application $g=f\circ (s|_V)$ de $E_V$ dans $E'$. Il existe donc une application continue $\widetilde{g}: B\rightarrow E'$ qui coïncide avec $g$ sur $\overline{W}$. Soit $h=\widetilde{g}|_U$. On a $h|_W=g|_W=f\circ (s|_W)$.

L’application $H: U\times G\rightarrow E'$ définie par $H(x, g) =h(x)\cdot g$ pour $(x, g)\in U\times G$ est continue et compatible avec les opérations de G dans $U\times G$ et $E'$. Posons $f'= H\circ s^{-1}$; c’est un élément de $\mathscr{F}(U)$. Pour tout $x\in W$, les applications $f$ et $f'$ coïncident au point $s(x)$, donc en tout point de $\overset{-1}{p}(x)$, car ce sont des morphismes d’espaces fibrés principaux. La proposition en résulte.

#### Théorème 1 {#ta-iv-s6-thm-1 .statement tag=024H}

Soit G un groupe topologique, soit $B_u$ un espace topologique, et soit $(E_u, p_u)$ un espace fibré principal de groupe G et de base $B_u$. On suppose que l’espace $E_u$ est homéotope à un point.

Soit B un espace topologique paracompact.

a) Tout espace fibré principal de groupe G et de base B est isomorphe à un espace fibré principal de la forme $f^*E_u$, où $f: B\rightarrow B_u$ est une application continue.

b) Soient $f_0$ et $f_1$ des applications continues de B dans $B_u$. Pour que $f_0^*E_u$ et $f_1^*E_u$ soient des espaces fibrés principaux de groupe G et de base B isomorphes, il faut et il suffit que les applications $f_0$ et $f_1$ soient homotopes.

En d’autres termes, il existe une application de $[B,B_u]$ dans P(B; G) qui, à la classe d’homotopie d’une application continue $f$ de B dans $B_u$, associe la classe d’isomorphisme de l’espace fibré principal $f^*E_u$. Cette application est bijective.

Soit E un espace fibré principal de groupe G et de base B. D’après la prop. 4, le faisceau $\mathscr{F}$ sur B des morphismes d’espaces fibrés principaux de E dans $E_u$ est mou. Par suite, $\mathscr{F}(B)$ n’est pas vide, d’où a).

Soient $f_0$ et $f_1$ des applications continues de B dans $B_u$. Si les applications $f_0$ et $f_1$ sont homotopes, les espaces fibrés principaux $f_0^*E_u$ et $f_1^*E_u$ sont isomorphes (IV, p. 445, cor. 2). Démontrons la réciproque. Pour $\alpha \in  \{0,1\}$, notons $E_{\alpha}$ le $B_u$-espace fibré principal $f_{\alpha}^*E_u$, $g_{\alpha}: E_{\alpha}\rightarrow E_u$ la première projection et $p_{\alpha}: E_{\alpha}\rightarrow B$ la seconde projection. Soit $i: E_0\rightarrow E_1$ un isomorphisme d’espaces fibrés principaux. Soit $p$ l’application $p_0\times$ Id$_{\mathbf{I}}: E_0\times \mathbf{I}\rightarrow B\times \mathbf{I}$.

Comme l’espace $B\times \mathbf{I}$ est paracompact (TG, IX, p. 70, prop. 17), le faisceau $\mathscr{G}$ sur $B\times \mathbf{I}$ des morphismes d’espaces fibrés principaux de $E_0\times \mathbf{I}$ dans $E_u$ est mou (IV, p. 446, prop. 4). Posons $A = B\times  \{0,1\}$, $U = B\times ([0,\frac{1}{2}[\cup ]\frac{1}{2},1])$, et définissons un élément $g$ de $\mathscr{G}(U)$ en posant

$g_0(x)$ pour $(x, t)\in E_0\times [0,^1[$,

$g(x, t) =$ 2

$g_1\circ i(x)$ pour $(x, t)\in E_0\times ]\frac{1}{2},1]$.

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

autrement dit, pour que $\sigma (h, t)\in V^*_{\varepsilon}\sigma (k, u)$, il suffit que l’on ait $|t-u|\leqslant \frac{\varepsilon}{2}$ et $h\in V^*_{\varepsilon /2}k$, ce qui démontre la continuité de $\sigma$ en $(k, u)$.

Pour tout $h\in G^*,\sigma (h,0)$ est l’application constante d’image $\{e\}$, tandis que $\sigma (h,1) =h$. En outre, $\sigma (e, t) =e$ pour tout $t\in \mathbf{I}$. Par conséquent, $\sigma$ est une homotopie pointée en $e\in G^*$ reliant l’application constante d’image $\{e\}$ à l’application identique de $G^*$. Cela démontre que $G^*$ est contractile en $e^*$.

En outre, pour tout voisinage V de $e$ dans G et tout nombre réel $\varepsilon  >0$, on a $\sigma (V^*_{\varepsilon}\times \mathbf{I})\subset V^*_{\varepsilon}$. Par suite, $V^*_{\varepsilon}$ est aussi contractile en $e^*\in$ $G^*$, si bien que $G^*$ est localement contractile en $e^*$.

Comme $G^*$ est un groupe topologique, il est contractile et localement contractile en chacun de ses points.

Soit $\iota$ l’application de G dans $G^*$ qui, à $g\in G$, associe l’application constante d’image $\{g\}$ de $[0,1[$ dans G. L’application $\iota$ est un homomorphisme injectif de groupes. Soit V un voisinage de $e$ dans G et soit $\varepsilon$ un nombre réel strictement positif. On a $\overset{-1}{\iota}(V^*_{\varepsilon}) = V$ si $\varepsilon \leqslant 1$ et $\overset{-1}{\iota}(V^*_{\varepsilon}) = G$ sinon. L’image réciproque d’un voisinage de l’élément neutre de $G^*$ est un voisinage de l’élément neutre de G, d’où la continuité de $\iota$. De plus, $\iota (V) = V^*_1\cap \iota (G)$ pour tout voisinage V de $e$ dans G. Par suite, $\iota$ définit un isomorphisme de groupes topologiques de G sur son image.

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

## EXERCICES {#ta-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
