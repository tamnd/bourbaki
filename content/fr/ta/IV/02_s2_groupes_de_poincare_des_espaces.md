---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 2
section_title: Groupes de Poincaré des espaces délaçables
lang: fr
source: ta-i-iv-fr
book_pages: TA IV.351-TA IV.368, TA IV.457-TA IV.458
pdf_pages: 0367-0384, 0473-0474
extraction: native
subsections:
    - "no": 1
      title: Propriétés des homomorphismes $\pi_1(f, a)$
      page: 351
      pdf_page: 367
    - "no": 2
      title: Applications relativement connexes
      page: 353
      pdf_page: 369
    - "no": 3
      title: Présentation des groupes de Poincaré
      page: 359
      pdf_page: 375
    - "no": 4
      title: Compléments sur les espaces polonais
      page: 360
      pdf_page: 376
    - "no": 5
      title: Relations d’équivalence maigres dans les espaces polonais
      page: 363
      pdf_page: 379
    - "no": 6
      title: Cardinal des groupes de Poincaré
      page: 365
      pdf_page: 381
statements: 30
exercises: 5
content_sha256: 73be7faacaad596224ce51c812b7b813c35e21521a9b0c6735de21f9cd9783bf
---

## § 2. GROUPES DE POINCARÉ DES ESPACES DÉLAÇABLES

### 1. Propriétés des homomorphismes $\pi_1(f, a)$

Soient A et B des espaces topologiques, soit $(E, p)$ un revêtement de A, soit $(E', p')$ un revêtement de B, soient $f: A\rightarrow B$ et $g: E\rightarrow E'$ des applications continues telles que $p'\circ g=f\circ p$. Soit $a$ un point de A et soit $b=f(a)$. Pour tout $\gamma \in \pi_1(A, a)$ et tout $x\in E_a$, on a $g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma )$, d’après la relation (3), III, p. 304. Si le diagramme

E $^gE'$

$pp'$

A $^f$ B

est un carré cartésien, l’application $g$ induit une bijection de $E_a$ sur $E'_b$. L’opération de $\pi_1(A, a)$ dans la fibre $E_a$ est alors la composée de l’opération du groupe $\pi_1(B, b)$ dans $E'_b$ et de l’homomorphisme $\pi_1(f, a)$ de $\pi_1(A, a)$ dans $\pi_1(B, b)$.

#### Proposition 1 {#ta-iv-s2-prop-1 .statement tag=020S}

Soient A un espace topologique délaçable, B un espace topologique localement connexe par arcs et soit $f: A\rightarrow B$ une application continue. Soient $a$ un point de A et $b=f(a)$. Supposons que tout revêtement de A soit isomorphe à l’image réciproque par $f$ d’un revêtement de B. Alors, l’homomorphisme $\pi_1(f, a):\pi_1(A, a)\rightarrow$ $\pi_1(B, b)$ est injectif.

Comme l’espace A est délaçable, il existe un revêtement E de A dont la fibre $E_a$ est un $\pi_1(A, a)$-ensemble principal homogène (IV, p. 342, théorème 1). Par hypothèse, cette opération se déduit par l’homomorphisme $\pi_1(f, a)$ d’une opération de $\pi_1(B, b)$ sur $\pi_1(A, a)$. Ceci implique l’injectivité de l’homomorphisme $\pi_1(f, a)$.

#### Proposition 2 {#ta-iv-s2-prop-2 .statement tag=020T}

Soient A un espace topologique connexe et localement connexe par arcs, B un espace topologique délaçable, et soit $f: A\rightarrow B$ une application continue. Soient $a$ un point de A et $b=$ $f(a)$. Les assertions suivantes sont équivalentes :

(i) L’homomorphisme $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ est surjectif.

(ii) Pour tout couple $(E,E')$ de revêtements de B, l’application

$$
f^*:\mathscr{C}_B(E; E')\rightarrow \mathscr{C}_A(A\times_BE; A\times_BE')
$$

qui, à un B-morphisme $g: E\rightarrow E'$, associe le A-morphisme

$$
f^*(g): A\times_BE\rightarrow A\times_BE',(x, y)\mapsto (x, g(y))
$$

est bijective.

Au moyen de l’homomorphisme $\pi_1(f, a)$, tout $\pi_1(B, b)$-ensemble est muni d’une structure de $\pi_1(A, a)$-ensemble. La condition (i) est alors équivalente à la condition (i$')$ suivante :

(i$')$ Pour tout couple $(F,F')$ de $\pi_1(B, b)$-ensembles, tout $\pi_1(A, a)$-morphisme de F dans $F'$ est un $\pi_1(B, b)$-morphisme.

En effet, si l’homomorphisme $\pi_1(f, a)$ est surjectif, tout $\pi_1(A, a)$-morphisme de $\pi_1(B, b)$-ensembles est un $\pi_1(B, b)$-morphisme. Inversement, prenons un $\pi_1(B, b)$-ensemble F réduit à un point et posons $F'=\pi_1(B, b)/f_*(\pi_1(A, a))$. L’application de F dans $F'$ dont l’image est $f_*(\pi_1(A, a))$ est un $\pi_1(A, a)$-morphisme mais n’est pas un $\pi_1(B, b)$-morphisme si $F'$ n’est pas réduit à un point, c’est-à-dire si $\pi_1(f, a)$ n’est pas surjectif.

Comme l’espace B est délaçable, tout $\pi_1(B, b)$-ensemble est isomorphe au $\pi_1(B, b)$-ensemble $E_b$, où E est un revêtement de B (IV, p. 344, remarque 1). L’équivalence de (i$')$ et (ii) résulte donc de la prop. 2 de III, p. 310.

#### Proposition 3 {#ta-iv-s2-prop-3 .statement tag=020U}

Soit B un espace topologique délaçable et soit A un sous-espace connexe et localement connexe par arcs de B (par exemple une partie ouverte et connexe). Soit $a$ un point de A. Les propriétés suivantes sont équivalentes :

(i) Tout revêtement de B est trivialisable au-dessus de A.

(ii) L’image de l’homomorphisme de $\pi_1(A, a)$ dans $\pi_1(B, a)$ déduit de l’injection canonique est réduite à l’élément neutre.

L’implication (ii)$\Rightarrow$(i) résulte du corollaire 3 (III, p. 309).

Inversement, supposons que tout revêtement de B soit trivialisable au-dessus de A. C’est en particulier le cas du revêtement simplement connexe par arcs $(\lambda_a(B), \varepsilon_B)$ (IV, p. 342, th. 1), si bien que l’homomorphisme $\pi_1(A, a)\rightarrow \pi_1(B, a)$ est trivial (III, p. 309, cor. 3 de la prop. 1).

### 2. Applications relativement connexes

#### Définition 1 {#ta-iv-s2-def-1 .statement tag=020V}

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. On dit que l’application $f$ est relativement connexe si tout point de Y possède un système fondamental

de voisinages constitué d’ensembles V tels que $\overset{-1}{f}(V)$ soit connexe et non vide.

Soit $f: X\rightarrow Y$ une application continue ; pour que $f$ soit relativement connexe, il faut et il suffit que tout point de Y possède un voisinage V tel que l’application $f_V:\overset{-1}{f}(V)\rightarrow V$ déduite de $f$ soit relativement connexe.

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue relativement connexe. L’image de $f$ est dense dans Y. Pour toute partie ouverte de Y, l’application $f_V:\overset{-1}{f}(V)\rightarrow V$ est relativement connexe.

#### Proposition 4 {#ta-iv-s2-prop-4 .statement tag=020W}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue relativement connexe.

a) Pour toute composante connexe U de X$,\overline{f(U)}$ est une partie

connexe, ouverte et fermée de Y, et l’on a $\overset{-1}{f}(f(U)) = U$.

b) Pour toute composante connexe V de Y, il existe une composante connexe U de X telle que $V =f(U)$. L’application de U dans V déduite de $f$ par passage aux sous-ensembles est relativement connexe.

c) Les composantes connexes de X ( resp. de Y) sont ouvertes et fermées.

a) Soit V l’ensemble des $y\in Y$ qui possèdent un voisinage W tel que

$\overset{-1}{f}(W)$ soit connexe et rencontre U ; c’est un ouvert de Y. Il contient $\overline{f(U)}$ car $f$ est relativement connexe. Inversement, soit $y\in V$ ; soit

W un voisinage de $y$ tel que $\overset{-1}{f}(W)$ soit connexe et rencontre U. Pour

tout voisinage $W'$ de $y$ tel que $\overset{-1}{f}(W')$ soit connexe, $\overset{-1}{f}(W\cap W')$ n’est

pas vide, donc $\overset{-1}{f}(W\cup W')$ est connexe (TG, I, p. 81, prop. 2). Par

hypothèse, $\overset{-1}{f}(W\cup W')$ rencontre U ; on a donc $\overset{-1}{f}(W\cup W')\subset U$ et, a fortiori, $W'\cap f(U)=\not\emptyset$. Cela démontre que $y\in \overline{f(U)}$; par suite, $V =\overline{f(U)}$. En particulier, l’ensemble $\overline{f(U)}$ est ouvert et fermé dans Y ; la prop. 1 (TG, I, p. 81) entraîne en outre qu’il est connexe.

Les arguments qui précèdent montrent de plus que $\overset{-1}{f}(f(U))\subset U$,

d’où l’égalité $\overset{-1}{f}(f(U)) = U$, l’autre inclusion étant évidente. En particulier, U est ouvert et fermé dans X.

b) Soit V la composante connexe d’un point $y$ de Y, soit W un

voisinage de $y$ tel que $\overset{-1}{f}(W)$ soit connexe et non vide et soit U la

composante connexe de X qui contient $\overset{-1}{f}(W)$. Comme $y\in \overline{f(U)}$, il résulte de a) et de la définition de la composante connexe de $y$ que $V =\overline{f(U)}$. Par suite, V est ouvert et fermé dans Y.

#### Corollaire 1 {#ta-iv-s2-prop-4-cor-1 .statement tag=020X}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue et relativement connexe. Par passage aux composantes connexes, l’application $f$ induit une bijection de l’ensemble des composantes connexes de X sur l’ensemble des composantes connexes de Y.

#### Corollaire 2 {#ta-iv-s2-prop-4-cor-2 .statement tag=020Y}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une application continue. Pour que $f$ soit relativement connexe, il faut et il suffit que les trois propriétés suivantes soient satisfaites :

a) L’image $f(X)$ est dense dans Y ;

b) L’espace Y est localement connexe ; $-_1$

c) Pour tout ensemble ouvert et connexe V de Y, l’ensemble $f(V)$ est connexe.

Supposons que l’application $f$ soit relativement connexe. La densité de $f(X)$ dans Y résulte de la définition d’une application relativement

connexe. Soit V un ouvert de Y ; l’application $f_V:\overset{-1}{f}(V)\rightarrow$ V est relativement connexe. D’après la prop. 4, les composantes connexes de V sont ouvertes et fermées dans V. Il en résulte que Y est localement connexe (TG, I, p. 85, prop. 11). Pour démontrer l’assertion c), il suffit de démontrer que X est connexe si Y l’est. D’après le lemme, il existe

une composante connexe U de X telle que $Y =\overline{f(U)}$ et $\overset{-1}{f}(f(U)) = U$, d’où U = X et X est connexe.

Inversement, supposons que les conditions a), b), c) sont vérifiées et montrons que $f$ est relativement connexe. Soit $y$ un point de Y ; puisque Y est localement connexe, $y$ admet un système fondamental de voisinages ouverts connexes. Si W est un tel voisinage, les conditions

c) et a) impliquent que $\overset{-1}{f}(W)$ est connexe et non vide. Par suite, l’application $f$ est relativement connexe.

#### Corollaire 3 {#ta-iv-s2-prop-4-cor-3 .statement tag=020Z}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue et relativement connexe. Soit F un ensemble et soit $g: X\rightarrow F$ une application localement constante. Il existe une unique application localement constante $h: Y\rightarrow F$ telle que $g=h\circ f$.

La restriction de $g$ à toute composante connexe de X est constante. D’après le corollaire 1, il existe une application $h: Y\rightarrow F$, constante sur chaque composante connexe de Y, telle que $g=h\circ f$. L’application $h$ est localement constante, car les composantes connexes de Y sont ouvertes. L’unicité d’une telle application résulte de ce que $f(X)$ est dense dans Y.

#### Exemple 1 {#ta-iv-s2-n2-exa-1 .statement tag=0210}

Soit X un espace topologique et soit R une relation d’équivalence dans X. Notons Y l’espace topologique quotient $X/R$ et $f: X\rightarrow Y$ l’application canonique. Supposons que les classes d’équivalences de R soient connexes. Alors, pour toute partie ouverte et

connexe V de Y, l’ensemble $\overset{-1}{f}(V)$ est connexe (TG, I, p. 23, corollaire 1 et p. 82, proposition 7). Si l’espace Y est localement connexe, l’application $f$ est ainsi relativement connexe.

#### Exemple 2 {#ta-iv-s2-n2-exa-2 .statement tag=0211}

Soit Y un espace topologique localement connexe par arcs et soit X une partie ouverte de Y. L’espace $\mathscr{C}_c(\mathbf{I}; X)$ des chemins dans X s’identifie à un sous-espace de l’espace $\mathscr{C}_c(\mathbf{I}; Y)$ des chemins dans Y ; supposons qu’il soit dense. L’injection canonique de X dans Y est alors une application relativement connexe.

Il suffit en effet de démontrer que, pour tout ouvert connexe et non vide V de Y, l’ensemble $V\cap X$ est connexe et non vide. L’espace $\mathscr{C}_c(\mathbf{I}; V)$ est un ouvert non vide de $\mathscr{C}_c(\mathbf{I}; Y)$ ; il rencontre $\mathscr{C}_c(\mathbf{I}; X)$, ce qui prouve que $V\cap X=\not\emptyset$. Soient $x$ et $x'$ des points de $V\cap X$. Comme $V\cap X$ est localement connexe par arcs, les points $x$ et $x'$ ont des voisinages ouverts U et $U'$, connexes par arcs et contenus dans $V\cap X$. Comme V est connexe par arcs (III, p. 260, prop. 7), il existe un chemin dans V qui relie $x$ à $x'$. Par l’hypothèse de densité et la définition de la topologie de la convergence compacte, il existe un chemin dans $V\cap X$ reliant un point de U à un point de $U'$. Il existe alors un chemin reliant $x$ à $x'$ dans $V\cap X$, ce qui prouve que l’ensemble $V\cap X$ est connexe.

#### Proposition 5 {#ta-iv-s2-prop-5 .statement tag=0212}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une application continue et relativement connexe. Pour tout couple $(T,T')$ de revêtements de Y, l’application $f^*:\mathscr{C}_Y(T; T')\rightarrow$ $\mathscr{C}_X(X\times_YT; X\times_YT')$ est bijective.

Soient $\mathscr{F}$ le faisceau sur X des X-morphismes de $X\times_YT$ dans $X\times_YT'$ et soit $\mathscr{G}$ le faisceau sur Y des Y-morphismes de T dans $T'($I, p. 45, exemple 4). Pour tout ouvert U de Y, posons $\varphi_U= (f_U)^*:\mathscr{G}(U)\rightarrow$

$\mathscr{F}(\overset{-1}{f}(U))$. Les applications $\varphi_U$ définissent un morphisme de faisceaux $\varphi :\mathscr{G}\rightarrow \varphi_*(\mathscr{F})$ et il suffit de démontrer que $\varphi$ est un isomorphisme de faisceaux.

Comme Y est localement connexe (IV, p. 354, cor. 2), les ensembles ouverts connexes au-dessus desquels T et $T'$ sont trivialisables forment une base de la topologie de Y. D’après le corollaire 2 de I, p. 55, il suffit de démontrer que pour un tel ouvert U, l’application $\varphi_U$ est bijective, ce qui nous permet de supposer que Y est connexe et que les revêtements T et $T'$ sont les revêtements triviaux $Y\times F$ et $Y\times F'$ où F et $F'$ sont des ensembles munis de la topologie discrète. L’application $(x,(y, t))\mapsto (x, t)$ identifie le X-espace $X\times_Y(Y\times F)$ à $X\times F$ (resp. le X-espace $X\times_Y(Y\times F')$ à $X\times F')$. Comme l’espace X est connexe (IV, p. 354, cor. 2), les ensembles $\mathscr{C}_Y(Y\times F; Y\times F')$ et $\mathscr{C}_X(X\times F; X\times F')$ s’identifient tous deux à l’ensemble $\mathscr{F}(F; F')$ des applications de F dans $F'$, et l’application $f^*$ s’identifie à l’application identique de $\mathscr{F}(F; F')$. Cela conclut la démonstration.

#### Corollaire 1 {#ta-iv-s2-prop-5-cor-1 .statement tag=0213}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue relativement connexe. Soient T et $T'$ des revêtements de Y. Si les revêtements $X\times_YT$ et $X\times_YT'$ de X sont isomorphes, les revêtements T et $T'$ sont isomorphes.

Soient en effet $h: X\times_YT\rightarrow X\times_YT'$ et $h': X\times_YT'\rightarrow X\times_YT$ des X-isomorphismes réciproques l’un de l’autre. D’après la proposition 5, il existe des Y-morphismes $g: T\rightarrow T'$ et $g': T'\rightarrow T$ tels que $f^*(g) =h$ et $f^*(g') =h'$. On a alors $f^*(g'\circ g) =f^*(g')\circ f^*(g) =$ Id$_{X\times_YT}$, donc $g'\circ g=$ Id$_T$, car l’application $f^*$ est injective. De même, $g\circ g'=$ Id$_{T'}$. Les revêtements T et $T'$ sont donc isomorphes.

#### Corollaire 2 {#ta-iv-s2-prop-5-cor-2 .statement tag=0214}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue et relativement connexe. Si l’espace X est simplement connexe, il en est de même de l’espace Y.

D’après le corollaire 1, tout revêtement de Y est en effet trivialisable.

#### Corollaire 3 {#ta-iv-s2-prop-5-cor-3 .statement tag=0215}

Soient X un espace topologique localement connexe par arcs, Y un espace topologique délaçable et soit $f: X\rightarrow$ Y une application continue relativement connexe. Pour tout point $x$ de X, l’homomorphisme $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ est surjectif.

D’après IV, p. 353, prop. 4, on peut supposer que les espaces X et Y sont connexes. Le corollaire résulte alors de la proposition 5 et de la proposition 2 de IV, p. 352.

#### Proposition 6 {#ta-iv-s2-prop-6 .statement tag=0216}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue et relativement connexe. Supposons que tout point de Y possède un voisinage ouvert V dont l’image réciproque $\overset{-1}{f}(V)$ soit simplement connexe. Alors, pour tout revêtement Z de X, il existe un revêtement T de Y tel que $X\times_YT$ soit X-isomorphe à Z.

Soit $\mathscr{U}$ l’ensemble des ouverts de Y dont l’image réciproque dans X

est simplement connexe. Pour tout $V\in \mathscr{U}$, le revêtement $\overset{-1}{f}(V)\times_XZ$

de $\overset{-1}{f}(V)$ est trivialisable ; il existe ainsi un espace discret $F_V$ et un

isomorphisme de revêtements $g_V:\overset{-1}{f}(V)\times_XZ\rightarrow \overset{-1}{f}(V)\times F_V$. Pour tout

couple $(V,V')$ d’ouverts appartenant à $\mathscr{U}$, l’application $f_{V\cap V'}:\overset{-1}{f}(V\cap$ $V')\rightarrow V\cap V'$ est relativement connexe. D’après la proposition 5 de IV, p. 356, il existe un unique isomorphisme de revêtements de $V\cap V'$, $h_{V',V}: (V\cap V')\times F_V\rightarrow (V\cap V')\times F_{V'}$, tel que l’on ait $f^*(h_{V',V})(x, t) =$ $g_{V'}(g_V^{-1}(x, t))$ pour tout $x\in V\cap V'$ et tout $t\in F_V$. Si V, $V',V''$ sont des éléments de $\mathscr{U}$, on a $h_{V'',V}(x, t) =h_{V'',V'}(h_{V',V}(x, t))$ pour tout $x\in V\cap V'\cap V''$ et tout $t\in F_V$. Il existe alors un unique Y-espace T et, pour tout $V\in \mathscr{U}$, un isomorphisme $h_V: T_V\rightarrow V\times F_V$, tel que l’on ait $h_{V',V}(x, t) =h_{V'}\circ h^{-1}_V(x, t)$ pour tout couple $(V,V')$ d’ouverts appartenant à $\mathscr{U}$, tout $x\in V\cap V'$ et tout $t\in F_V($cf. TG, I, p. 16). L’espace T est en particulier un revêtement de Y. Il existe en outre une

unique application de $X\times_YT$ sur Z dont la restriction à $\overset{-1}{f}(V)\times_YT$ est donnée par $g^{-1}_V\circ f^*(h_V)$ et c’est un isomorphisme de X-espaces, d’où la proposition.

#### Corollaire {#ta-iv-s2-n2-cor-1 .statement tag=0217}

Soient X et Y des espaces topologiques délaçables et soit $f: X\rightarrow Y$ une application continue et relativement connexe. Supposons que tout point de Y possède un voisinage V dont l’image

réciproque $\overset{-1}{f}(V)$ soit simplement connexe. Alors, pour tout point $x$ de X, l’homomorphisme $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ est bijectif.

On peut supposer les espaces X et Y connexes (IV, p. 353, prop. 4). D’après le corollaire 3 (IV, p. 357), l’homomorphisme $\pi_1(f, x)$ est surjectif. La proposition 6 et la proposition 1 de IV, p. 351 entraînent qu’il est injectif.

#### Remarque {#ta-iv-s2-n2-rem-1 .statement tag=0218}

Soit Y un espace topologique, soient X, $X'$ et $Y'$ des sous-espaces de Y tels que $X\subset X'\subset Y'\subset Y$. Supposons que l’injection canonique de X dans Y soit relativement connexe. Pour toute partie ouverte connexe V de Y, l’ensemble $V\cap X$ est connexe et dense dans V (IV, p. 354, cor. 2) ; par suite, l’ensemble $V\cap X'$ est connexe (TG, I, p. 81, prop. 1). Cela démontre que l’injection canonique de $X'$ dans $Y'$ est relativement connexe.

Soit V une partie ouverte de Y ; d’après ce qui précède, l’injection canonique de $V\cap X$ dans $V\cap X'$ est relativement connexe. Si l’ensemble $V\cap X$ est simplement connexe, $V\cap X'$ l’est aussi, en vertu du corollaire 2 de IV, p. 357. Par suite, si l’injection canonique de X dans Y satisfait aux hypothèses de la proposition 6, il en est de même de l’injection canonique de $X'$ dans $Y'$.

#### Exemple {#ta-iv-s2-n2-exa-3 .statement tag=0219}

Soit Y une variété différentielle localement de dimension finie et soit Z une sous-variété fermée de Y (VAR, R, 5.8.3). Posons X = Y-Z.

a) Si la codimension de Z est au moins 2 en tout point, l’injection canonique de X dans Y est relativement connexe. Soit en effet $z$ un point de Z ; il existe un voisinage ouvert V de $z$ dans Y et un homéomorphisme $\varphi$ de V sur un espace vectoriel E de dimension finie sur $\mathbf{R}$ tel que $\varphi (V\cap Z)$ soit un sous-espace vectoriel F de E dont la codimension est $\geqslant 2$. L’ensemble E-F est connexe (TG, VI, p. 5, proposition 4), d’où l’assertion.

b) Supposons de plus que la codimension de Z soit au moins égale à 3 en tout point ; les hypothèses de la proposition 6 et de son corollaire sont alors satisfaites car, avec les notations de l’alinéa précédent, E-F est simplement connexe (I, p. 128, exemple 4).

Les variétés différentielles étant des espaces délaçables (IV, p. 347), les résultats de ce n$^o$ admettent le cas particulier suivant.

Soient Y une variété différentielle localement de dimension finie, Z une sous-variété fermée de Y et $i$ l’injection canonique de Y-Z dans Y.

a) Si la codimension de Z dans Y est $\geqslant 1$ en tout point, la variété Y-Z est dense dans Y et l’application $\pi_0(i)$ est surjective.

b) Si la codimension de Z dans Y est $\geqslant 2$ en tout point, l’application $\pi_0(i)$ est bijective et, pour tout point $x$ de Y-Z, l’application $\pi_1(i, x)$ est surjective.

c) Si la codimension de Z dans Y est $\geqslant 3$ en tout point, les applications $\pi_0(i)$ et $\pi_1(i, x)$ sont bijectives, pour tout point $x$ de Y-Z.

### 3. Présentation des groupes de Poincaré

#### Théorème 1 {#ta-iv-s2-thm-1 .statement tag=021A}

Soit X un espace topologique compact délaçable et soit $x$ un point de X. Le groupe de Poincaré $\pi_1(X, x)$ est de présentation finie.

La composante connexe par arcs de $x$ dans X est ouverte, fermée et est délaçable ; cela permet de supposer que l’espace X est connexe. Comme l’espace X est délaçable, le X-espace $E =\lambda_x(X)$, muni de l’application terme, est un revêtement non vide et simplement connexe par arcs (IV, p. 342, th. 1). Le groupe G = Aut$_X(E)$ est isomorphe à $\pi_1(X, x)$ ; il s’agit donc de démontrer que le groupe G est de présentation finie.

Comme X est compact, tout point $x$ de X possède un voisinage compact $K_x$ au-dessus duquel le revêtement E est trivialisable (TG, I, p. 65, corollaire). Comme X est localement connexe, tout $x\in X$ possède un voisinage ouvert $W_x$, connexe et contenu dans $K_x$. Soit F une partie finie de X telle que les $W_x$, pour $x\in F$, recouvrent X. Soit $n$ le cardinal de F.

Montrons par récurrence qu’il existe, pour tout entier $k$ tel que 1 $\leqslant k\leqslant n$, une partie A de cardinal $k$ contenue dans F et, pour $x\in A$, une section $s_x$ de $p$ au-dessus de $K_x$, telles que la réunion des $s_x(W_x)$, pour $x\in A$, soit une partie connexe de E. L’assertion est vraie pour $k= 1$. Supposons-la vraie pour un entier $k$ tel que $1\leqslant k < n$ et démontrons qu’elle est vraie pour $k+ 1$. Soit A une partie de F de cardinal $k$ et, pour tout $x\in A$, soit $s_x$ une section de E au-dessus de $K_x$, telles que $\bigcup_{x\in A}s_x(W_x)$ soit connexe. Les ouverts $\bigcup_{x\in A}W_x$ et $\bigcup_{x\in F-A}W_x$ ne sont pas vides et recouvrent X ; leur intersection n’est donc pas vide, car X est connexe. Il existe ainsi $x\in A,y\in F-A$ et $z\in W_x\cap W_y$. Posons $A'= A\cup  \{y\}$ et choisissons une section $s_y$ de E au-dessus de $K_y$ telle que $s_y(z) =s_x(z)$. Les ouverts connexes $\bigcup_{p\in A}s_p(W_p)$ et $s_y(W_y)$ ne sont pas vides et ont un point commun ; leur réunion est donc connexe. Cela démontre l’assertion pour $k+ 1$. Par récurrence, elle est donc vraie pour tout entier $k\in  \{1, . . . , n\}$.

Appliquons ce qui précède à $k=n$; il existe alors, pour tout $x\in F$, une section $s_x$ de E au-dessus de $K_x$, de sorte que $U =\bigcup_{x\in F}s_x(W_x)$ soit un ouvert connexe de E. On a $p(U) = X$. Comme le groupe G opère transitivement dans chaque fibre du revêtement E, on a GU = E.

L’adhérence de U est contenue dans $\bigcup_{x\in F}s_x(K_x)$ donc est compacte. L’opération de G dans E est propre (I, p. 96, cor. 1), donc l’ensemble des couples $(g, x)\in G\times E$ tels que $x\in \overline{U}$ et $gx\in \overline{U}$ est une partie compacte de $G\times E$ (TG, I, p. 77, prop. 6). Il s’ensuit que l’ensemble des $g\in G$ tels que $\overline{U}\cap g\overline{U}=\not\emptyset$ est compact. Comme il est discret, il est fini. A fortiori, l’ensemble des $g\in G$ tels que $U\cap gU=\not\emptyset$ est fini. Le théorème découle ainsi de la prop. 10 de I, p. 136.

### 4. Compléments sur les espaces polonais

#### Lemme 1 {#ta-iv-s2-lem-1 .statement tag=021B}

Soit X un espace topologique et soit A une partie de X. Pour que A soit maigre, il faut et il suffit qu’il existe un recouvrement ouvert $(U_i)_{i\in I}$ de X tel que $A\cap U_i$ soit maigre dans $U_i$ pour tout $i\in I$.

Soit $\mathscr{O}$ l’ensemble des parties ouvertes U de X telles que $A\cap U$ soit maigre. L’ensemble des parties de $\mathscr{O}$ formées d’ouverts deux à deux disjoints, ordonné par l’inclusion, est inductif. Soit $\mathfrak{U}$ un élément maximal ; il en existe d’après E, III, p. 20, th. 2.

Soit O la réunion des ouverts de X appartenant à $\mathfrak{U}$. Pour tout ouvert $U\in \mathfrak{U}$, soit $(B_{U,n})$ une suite de parties rares de U dont $A\cap U$ soit la réunion. Pour tout entier $n$, la réunion $B_n$ des parties $B_{U,n}$, pour U parcourant $\mathfrak{U}$, est rare relativement à O (TG, IX, p. 52, prop. 1). D’après TG, IX, p. 53, prop. 2, $B_n$ est une partie rare de X, car O est ouvert dans X. Par conséquent, l’ensemble $A\cap O$, égal à la réunion des $B_n$, est une partie maigre de X.

Soit F le complémentaire de O. C’est une partie fermée de X ; démontrons qu’elle est d’intérieur vide. Dans le cas contraire, soit $x$ un point intérieur de F. Par hypothèse, il existe un voisinage ouvert V de $x$, qu’on peut supposer contenu dans F, tel que $A\cap V$ soit maigre. Alors V est disjoint des ouverts de X appartenant à $\mathfrak{U}$ et $\mathfrak{U}\cup  \{V\}$ est un ensemble d’ouverts deux à deux disjoints appartenant à $\mathscr{O}$, ce qui contredit la maximalité de $\mathfrak{U}$. La relation

$$
A = (A\cap F)\cup (A\cap O)
$$

entraîne alors que A est maigre, ce qu’il fallait démontrer.

Soit X un espace topologique.

Rappelons (TG, IX, p. 69) qu’une partie A de X est dite approchable s’il existe un ouvert U de X tel que $U\cap \complement A$ et $A\cap \complement U$ soient maigres dans X. L’ensemble des parties approchables de X est une tribu qui contient la tribu borélienne (TG, IX, p. 69, lemme 8 et sa démonstration). Une partie maigre est approchable.

Pour toute partie A de X, soit D(A) l’ensemble des points $x\in X$ tels que pour tout voisinage V de $x,A\cap V$ ne soit pas maigre. On pose aussi $D^*(A) = A\cup D(A)$.

#### Lemme 2 {#ta-iv-s2-lem-2 .statement tag=021C}

Soit X un espace topologique et soit A une partie de X.

a) L’ensemble D(A) est fermé dans X ; son complémentaire est le plus grand ouvert U de X tel que $A\cap U$ soit un ensemble maigre.

b) Pour que A soit maigre, il faut et il suffit que D(A) soit vide.

c) L’ensemble $D^*(A)$ est approchable.

d) Pour tout ensemble approchable B de X contenant A, $D^*(A)\cap$ $\complement B$ est maigre.

Soit U la réunion des ouverts V de X tels que $A\cap V$ soit maigre. Pour qu’un point $x$ appartienne à U, il faut et il suffit qu’il possède un voisinage V tel que $A\cap V$ soit maigre. On a ainsi $U =\complement D(A)$ et D(A) est donc une partie fermée de X. Par construction, le sous-espace U possède un recouvrement par des parties ouvertes dont l’intersection avec A est maigre. D’après le lemme 1, appliqué à l’espace topologique U et au sous-ensemble $A\cap U$, $A\cap U$ est maigre dans U, donc aussi dans X. Cela démontre l’assertion a), car, par construction, tout ouvert V de X tel que $A\cap V$ soit maigre est contenu dans U.

L’assertion b) en découle immédiatement.

c) On a $D^*(A) = A\cup D(A) = (A\cap U)\cup D(A)$. L’ensemble D(A) est fermé, donc approchable (IV, p. 361) ; la partie maigre $A\cap U$ l’est aussi. Par suite, $D^*(A)$ est approchable (loc. cit.).

d) Soit B une partie approchable de X qui contient A. Son complémentaire $\complement B$ est alors une partie approchable de X (loc. cit.) et il existe donc un ouvert V de X tel que $V\cap B$ et $\complement V\cap \complement B$ soient maigres. Comme $A\subset B$, $V\cap A$ est encore maigre, d’où $V\subset U$. Puisque $\complement U\cap \complement B$ est contenu dans $\complement V\cap \complement B$, c’est aussi une partie maigre de X. Finalement, les inclusions

$$
D^*(A)\cap \complement B = (A\cap U)\cap \complement B\cup \complement U\cap \complement B\subset (A\cap U)\cup (\complement U\cap \complement B)
$$

démontrent que $D^*(A)\cap \complement B$ est une partie maigre de X.

#### Remarque 1 {#ta-iv-s2-n4-rem-1 .statement tag=021D}

Soit G un groupe topologique et soit A une partie maigre de G. Supposons que A contienne un ouvert non vide U de G et soit $y$ un point de U. Alors, U est maigre et pour tout $x\in G,xy^{-1}U$ est un voisinage de $x$ dans G. Par suite, tout point de G possède un voisinage maigre, donc G est maigre (IV, p. 360, lemme 1).

Inversement, si G n’est pas maigre, toute partie maigre est d’intérieur vide et G est un espace de Baire. Comme un espace de Baire n’est pas maigre, cela démontre l’assertion suivante : Pour qu’un groupe topologique soit un espace de Baire, il faut et il suffit qu’il ne soit pas maigre.

#### Proposition 7 {#ta-iv-s2-prop-7 .statement tag=021E}

Soit X un espace séparé. Tout sous-espace souslinien (TG, IX, p. 59, déf. 2) de X est approchable.

Soit S un sous-espace souslinien de X. Par définition, il existe un espace métrique complet de type dénombrable P et une application continue et surjective $g$ de P dans S. D’après TG, IX, p. 64, lemme 3, il existe un criblage $C = (C_n, p_n, \varphi_n)_{n\in\mathbf{N}}$ de l’espace métrique P.

Pour tout entier $n$ et tout $c\in C_n$, notons $F_n(c)$ l’image de l’ensemble $\varphi_n(c)$ par $g$; posons aussi $F^*_n(c) = D^*(F_n(c))$ et

$$
G_n(c) = F^*_n(c)\cap \complement \bigcup_{c'\in\overset{-1}{p_{n}}(c)}F^*_{n+1}(c') \tag{1}
$$

Pour tout $c\in C_n,F^*_n(c)$ est approchable (IV, p. 361, lemme 2, c)). Comme $C_{n+1}$ est dénombrable, la réunion des parties approchables $F^*_{n+1}(c')$, pour $c'$ parcourant $\overset{-1}{p_{n}}(c)$, est encore une partie approchable de X. Elle contient la réunion des $F_{n+1}(c')$ qui est égale à $F_n(c)$. Par suite (loc. cit., d)), $G_n(c)$ est une partie maigre de X. La réunion G des parties $G_n(c)$, pour $n\in \mathbf{N}$ et $c\in C_n$, est donc une partie maigre de X.

Soit $c_0\in C_0$ et soit $x$ un élément de $F^*_0(c_0)\cap \complement G$ ; démontrons que $x\in F_0(c_0)$. Puisque $x\notin G_0(c_0)$ et que $x\in F^*_0(c_0)$, il existe $c_1\in \overset{-1}{p_{0}}(c_0)$ tel que $x\in F^*_1(c_1)$, d’après la relation (1). Par récurrence, il existe un élément $c= (c_n)_n$ de $\prod_nC_n$ tel que, pour tout entier $n\in \mathbf{N}$, on ait $x\in F^*_n(c_n)$ et $p_n(c_{n+1}) =c_n$.

Les parties $\varphi_n(c_n)$ forment une base d’un filtre de Cauchy dans P; ce filtre converge vers un point $p$ de P, puisque P est complet. L’image de ce filtre par $g$ est un filtre F sur X, de base l’ensemble des $F_n(c_n)$ pour $n\in \mathbf{N}$, qui converge vers $g(p)$. Comme $F^*_n(c_n)$ est contenu dans $\overline{F_n(c_n)}$ et que $x$ appartient à chacun des $F_n(c_n),x$ est un point adhérent à F, donc $x=g(p)$ car l’espace X est séparé (TG, I, p. 52, prop. 1). Le point $p$ appartient à $\overline{\varphi_1(c_1)}$, donc à $\varphi_0(c_0)$. Par suite, $x\in F_0(c_0)$.

Par conséquent, l’ensemble $F^*_0(c_0)$ - $F_0(c_0)$ est contenu dans G. C’est ainsi une partie maigre de X, donc aussi une partie approchable. Puisque $F_0(c_0) = F^*_0(c_0)$ - $(F^*_0(c_0)$ - $F_0(c_0))$ et que $F^*_0(c_0)$ est approchable, $F_0(c_0)$ est approchable, car les parties approchables de X forment une tribu. Comme $C_0$ est dénombrable, l’ensemble S qui est la réunion des $F_0(c_0)$, pour $c_0\in C_0$, est encore approchable.

### 5. Relations d’équivalence maigres dans les espaces polonais

#### Lemme 3 {#ta-iv-s2-lem-3 .statement tag=021F}

Soit $(U_i)_{i\in I}$ une famille finie d’ouverts non vides d’un espace topologique X et soit O une partie ouverte et dense de $X\times X$. Il existe une famille $(V_i)_{i\in I}$ d’ouverts non vides de X tels que $V_i\subset U_i$ pour tout $i\in I$ et tels que $V_i\times V_{i'}\subset O$ pour tout couple $(i, i')$ d’éléments distincts de I.

Pour tout couple $(j_1, j_2)$ d’éléments distincts de I, l’ensemble des familles $(x_i)\in X^I$ tels que $(x_{j_1}, x_{j_2})\in O$ est un ouvert dense de $X^I$. L’intersection Ω de ces ouverts, lorsque $(j_1, j_2)$ parcourt l’ensemble fini des couples d’éléments distincts de I est donc un ouvert dense de $X^I$. Par suite, $\Omega \cap \prod_{i\in I}U_i$ est un ouvert non vide de $X^I$, donc contient un ouvert de $X^I$ de la forme $\prod_{i\in I}V_i$, où pour tout $i\in I$, $V_i$ est une partie ouverte, non vide, de $U_i$. Cela démontre le lemme.

#### Proposition 8 {#ta-iv-s2-prop-8 .statement tag=021G}

Soit P un espace topologique polonais non vide et soit R une relation d’équivalence dans P dont le graphe est une partie maigre de $P\times P$. Il existe une application continue injective de l’ensemble $\{0,1\}^{\mathbf{N}}$, muni de la topologie produit des topologies discrètes, dans P dont l’image rencontre chaque classe d’équivalence suivant R en au plus un point.

Munissons l’espace P d’une distance $d$ compatible avec sa topologie pour laquelle il est complet. Soit $(A_n)_{n\in\mathbf{N}}$ une suite croissante de parties fermées de $P\times P$, d’intérieurs vides, telles que le graphe $\Gamma_R$ de la relation R soit contenue dans la réunion des $A_n$.

Soit $\mathscr{O}$ l’ensemble des parties ouvertes non vides de P. Nous allons construire par récurrence une suite $(f_n)_{n\in\mathbf{N}}$, où pour tout $n,f_n$ est une application de $\{0,1\}^n$ dans $\mathscr{O}$, vérifiant les propriétés suivantes :

(i) Pour tout $n\geqslant 1$, tout $x\in  \{0,1\}^{n-1}$ et tout $t\in  \{0,1\}$, l’adhérence de l’ouvert $f_n(x, t)$ est contenue dans $f_{n-1}(x)$ ;

(ii) Pour tout $x\in  \{0,1\}^n$, on a diam($f_n(x)$)$\leqslant 2^{-n}$;

(iii) Pour tout $n\geqslant 1$ et tout couple $(x, x')$ d’éléments distincts de $\{0,1\}^n,f_n(x)\times f_n(x')$ ne rencontre pas $A_{n-1}$.

On choisit un ouvert non vide U de X de diamètre $\leqslant 1$ et on définit $f_0$ comme l’application constante d’image $\{U\}$. Supposons les applications $f_0, . . . , f_n$ construites.

Soit $p:\{0,1\}^{n+1}\rightarrow  \{0,1\}^n$ l’application définie par $p(x_0, . . . , x_n) =$ $(x_0, . . . , x_{n-1})$. D’après le lemme 3 ci-dessus, appliqué à la famille des ouverts $(f_n(p(x)))$ pour $x\in  \{0,1\}^{n+1}$ et à l’ouvert dense $\complement A_n$ de $P\times P$, il existe une famille $(g(x))_{x\in \{0,1\}^{n+1}}$ d’ouverts non vides de P telle que $g(x)\subset f_n(p(x))$ pour tout $x$ et telle que $(g(x)\times g(x'))\cap A_n$ soit vide pour tout couple $(x, x')$ d’éléments distincts de $\{0,1\}^{n+1}$. On définit alors l’application $f_{n+1}$ en choisissant, pour chaque élément $x\in  \{0,1\}^{n+1}$, une partie ouverte et non vide de $g(x)$ dont le diamètre est $\leqslant 2^{-n-1}$ et dont l’adhérence est contenue dans $g(x)$.

Pour tout élément $x= (x_n)_{n\in\mathbf{N}}$ de $\{0,1\}^{\mathbf{N}}$, la suite d’ensembles $(f_n(x_0, . . . , x_{n-1}))_{n\in\mathbf{N}}$ est une suite décroissante de parties ouvertes de X dont chacune contient l’adhérence de la suivante et dont le diamètre tend vers 0 ; l’intersection de cette suite d’ensembles est donc réduite à un point (TG, II, p. 15) que l’on note $f(x)$. Si deux points $x,x'$ de $\{0,1\}^{\mathbf{N}}$ vérifient $x_i=x'_i$ pour $i\leqslant n$, on a $d(f(x), f(x'))\leqslant 2^{-n}$. Par conséquent, l’application $f:\{0,1\}^{\mathbf{N}}\rightarrow P$ est continue. Soient $x$ et $x'$ des éléments distincts de $\{0,1\}^{\mathbf{N}}$. Pour $n\in \mathbf{N}$ tel que $(x_0, . . . , x_n)=\not$ $(x'_0, . . . , x'_n)$, l’ouvert $f_{n+1}(x_0, . . . , x_n)\times f_{n+1}(x'_0, . . . , x'_n)$ est disjoint de $A_n$, par définition de $f_{n+1}$, donc le couple $(f(x), f(x'))$ n’appartient pas à $A_n$. Il en résulte que $f(x)$ et $f(x')$ ne sont pas équivalents pour la relation R. Par conséquent, $f$ est injective et son image rencontre chaque classe d’équivalence suivant R en au plus un point. La proposition est ainsi démontrée.

### 6. Cardinal des groupes de Poincaré

#### Proposition 9 {#ta-iv-s2-prop-9 .statement tag=021H}

Soit X un espace topologique délaçable et soit $\mathscr{W}$ une base de la topologie de X. Pour tout point $x$ de X, le cardinal du groupe $\pi_1(X, x)$ est majoré par sup(Card($\mathscr{W}$), Card($\mathbf{N}$)). En particulier, le groupe de Poincaré d’un espace métrique de type dénombrable et délaçable est dénombrable.

En effet, l’espace $\lambda_x(X)$ muni de l’application terme est un revêtement connexe de X dont la fibre en $x$ est $\pi_1(X, x)$. L’assertion résulte alors de I, p. 40, th. 3.

#### Lemme 4 {#ta-iv-s2-lem-4 .statement tag=021I}

Soit X un espace de Baire, soit G un groupe topologique opérant continûment dans X et soit B une partie approchable de X qui n’est pas maigre. L’ensemble des points $g\in G$ tels que $B\cap gB=\not\emptyset$ est un voisinage de l’élement neutre de G.

Comme B est approchable, $\complement B$ est aussi approchable, car l’ensemble des parties approchables de X est une tribu. Il existe donc une partie ouverte U de X telle que $U\cap \complement B$ et $B\cap \complement U$ soient maigres dans X.

Soient V un voisinage de l’élément neutre de G et W un ouvert non vide de X contenu dans U tels que $V\cdot W\subset U$. Pour tout $g\in V$, $U\cap gU$ n’est pas vide.

Soit $g\in G$ tel que $B\cap gB$ soit vide. Les relations

$$
U\cap gU = (U\cap gU)\cap \complement (B\cap gB)
$$

$$
= (U\cap gU)\cap (\complement B\cup g\complement B)
$$

$$
= (U\cap gU\cap \complement B)\cup (U\cap gU\cap g\complement B)
$$

$$
\subset (U\cap \complement B)\cup g(U\cap \complement B)
$$

entraînent que $U\cap gU$ est maigre dans X. Comme c’est une partie ouverte et que X est un espace de Baire, elle est vide. On a donc $g\notin V$, d’où le lemme.

#### Théorème 2 (Shelah[^1]) {#ta-iv-s2-thm-2 .statement tag=021J}

Soit X un espace polonais connexe et localement connexe par arcs et soit $x$ un point de X. Si X n’est pas délaçable, le groupe $\pi_1(X, x)$ a la puissance du continu.

Soit $d$ une distance définissant la topologie de X pour laquelle il est complet. Supposons que X n’est pas délaçable. Il existe alors un point $a\in X$ et, pour tout entier $n\geqslant 0$, un lacet $c_n$ en $a$ dans X dont l’image est de diamètre $\leqslant 2^{-n}$ et dont la classe dans $\pi_1(X, a)$ n’est pas triviale.

Notons K l’ensemble $\{0,1\}^{\mathbf{N}}$ et munissons-le de la topologie produit, l’espace $\{0,1\}$ étant muni de la topologie discrète. Pour tout élément $\varepsilon = (\varepsilon_n)$ de K, soit $c_{\varepsilon}$ l’application de $\mathbf{I}$ dans X définie par $c_{\varepsilon}(0) =a$ et, pour $2^{-n-1}\leqslant t\leqslant 2^{-n},c_{\varepsilon}(t) =c_n(2^{n+1}t-1)$ si $\varepsilon_n= 1$ et $c_{\varepsilon}(t) =a$ sinon. On a $c_{\varepsilon}(0) =c_{\varepsilon}(1) =a$. L’application $c_{\varepsilon}$ est continue en tout point $t\in ]0,1]$. Elle l’est aussi en 0 car $d(a, c_{\varepsilon}(t))\leqslant 2^{-n}$ si $t\in [0,2^{-n}]$. L’application $c_{\varepsilon}$ est donc un lacet dans X en $a$.

Si $\varepsilon$ et $\varepsilon '$ sont des éléments de K tels que $(\varepsilon_0, . . . , \varepsilon_n) = (\varepsilon '_0, . . . , \varepsilon '_n)$, alors $c_{\varepsilon}(t) =c_{\varepsilon'}(t)$ pour tout $t\in [2^{-n-1},1]$ et $d(c_{\varepsilon}(t), c_{\varepsilon'}(t))\leqslant$ $d(a, c_{\varepsilon}(t)) +d(a, c_{\varepsilon'}(t))\leqslant 2^{-n}$ si $t\in [0,2^{-n-1}]$. Il en résulte que l’application $\varepsilon \mapsto c_{\varepsilon}$ de K dans l’espace $\Omega_a(X)$ est continue, lorsqu’on munit l’espace $\Omega_a(X)$ de la topologie de la convergence compacte.

Notons $\Gamma \subset K\times K$ l’ensemble des couples $(\varepsilon , \varepsilon ')$ tels que $c_{\varepsilon}$ soit strictement homotope à $c_{\varepsilon'}$. C’est le graphe d’une relation d’équivalence R dans K.

#### Lemme 5 {#ta-iv-s2-lem-5 .statement tag=021K}

L’ensemble Γ est une partie maigre de $K\times K$.

Notons Z l’espace $K\times K\times \mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$. La topologie de l’espace $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ est définie par la distance $\delta$ donnée par $\delta (h, h') =$ sup$_{u\in\mathbf{I}\times\mathbf{I}}d(h(u), h'(u))$ et il est complet pour cette distance (TG, X, p. 20, corollaire et TG, X, p. 9, cor. 1) ; d’après TG, X, p. 24, th. 1, cette topologie est de type dénombrable. L’espace $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ est donc un espace polonais. Il en est de même de l’espace Z, car K est un espace polonais (TG, IX, p. 57, prop. 1).

Soit H le sous-ensemble de Z formé des triplets $(\varepsilon , \varepsilon ', h)$ tels que $h$ soit une homotopie stricte reliant $c_{\varepsilon}$ à $c_{\varepsilon'}$. Les applications de Z dans $X^2$ données par $a_t: (\varepsilon , \varepsilon ', h)\mapsto (c_{\varepsilon}(t), h(t,0)),b_t: (\varepsilon , \varepsilon ', h)\mapsto$ $(c_{\varepsilon'}(t), h(t,1))$ et $c_t: (\varepsilon , \varepsilon ', h)\mapsto (h(0, t), h(1, t))$ sont continues, pour tout $t\in \mathbf{I}$, car l’application $\varepsilon \mapsto c_{\varepsilon}$ de K dans $\Omega_a(X)$ est continue, de même que les applications $h\mapsto h(s, t)$ de $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ dans X.

Par définition, H est l’intersection des ensembles $\overset{-1}{a_{t}}(\Delta_X),\overset{-1}{b_{t}}(\Delta_X)$ et $\overset{-1}{c_{t}}((a, a))$, pour $t\in \mathbf{I}$, où $\Delta_X$ désigne la diagonale de X. Cela démontre que H est une partie fermée de Z.

Par suite, H est un espace polonais. Soit $p: Z\rightarrow K\times K$ la projection canonique ; on a $\Gamma  =p(H)$ par définition. Comme $K\times K$ est séparé, Γ est un sous-ensemble souslinien de $K\times K$ (TG, IX, p. 59, déf. 2). D’après IV, p. 362, prop. 7, c’est une partie approchable de $K\times K$.

Supposons que Γ ne soit pas maigre. L’espace $K\times K$ est un espace topologique compact donc un espace de Baire (TG, IX, p. 55, th. 1). Munissons le groupe $G_0$ des permutations de l’ensemble $\{0,1\}$ de la topologie discrète ; faisons opérer diagonalement le groupe topologique produit $G = G^{\mathbf{N}}_0$ dans $K =\{0,1\}^{\mathbf{N}}$. Le groupe G opère alors continûment dans $K\times K$ par l’application $(g,(x, y))\mapsto (x, g\cdot y)$. D’après le lemme 4, l’ensemble V des éléments $g\in G$ tels que $\Gamma \cap g\cdot \Gamma =\not\emptyset$ est un voisinage de l’élément neutre de G.

Soit $g\in V$ ; soit $(\varepsilon , \varepsilon ')\in \Gamma \cap g\Gamma$. Comme $(\varepsilon , \varepsilon ')\in \Gamma$, on a $R\{\varepsilon , \varepsilon '\}$; comme $(\varepsilon , \varepsilon ')\in g\Gamma ,g^{-1}\cdot (\varepsilon , \varepsilon ') = (\varepsilon , g^{-1}\varepsilon ')\in \Gamma$, si bien que $R\{\varepsilon , g^{-1}\varepsilon '\}$. Nous avons ainsi démontré que, pour tout $g\in V$, il existe $\varepsilon \in K$ tel que $\varepsilon$ et $g\varepsilon$ soient équivalents pour R.

Pour $m\in \mathbf{N}$, désignons par $\tau_m$ l’élément de G dont tous les termes sont égaux à $e$ sauf celui d’indice $m$ qui est égal à l’élément non trivial $\tau$ de $G_0$. Il existe un entier $m$ tel que $\tau_m$ appartienne à V ; soit alors $\varepsilon \in K$ tel que $\varepsilon$ et $\varepsilon '=\tau_m\cdot \varepsilon$ soient équivalents pour R. Cela entraîne que les lacets $c_{\varepsilon}$ et $c_{\varepsilon'}$ sont strictement homotopes. Par construction, ces lacets coïncident sur les intervalles $[0,2^{-m-1}]$ et $[2^{-m},1]$ ; sur l’intervalle $[2^{-m-1},2^{-m}]$, l’un est l’application constante d’image $a$ et l’autre est l’application $t\mapsto c_m(2^{m+1}t-1)$. Il en résulte que $c_m$ est strictement homotope au lacet constant d’image $\{a\}$, d’où une contradiction. Le lemme 5 est ainsi démontré.

Terminons maintenant la démonstration du théorème 2. D’après la prop. 8, il existe une application continue injective $\gamma$ de $\{0,1\}^{\mathbf{N}}$ dans K dont l’image rencontre toute classe d’équivalence suivant R en au plus un point. Si $k$ et $k'$ sont des éléments distincts de $\{0,1\}^{\mathbf{N}}$, les lacets $c_{\gamma(k)}$ et $c_{\gamma(k')}$ ne sont pas strictement homotopes dans X et l’application $\{0,1\}^{\mathbf{N}}\rightarrow \pi_1(X, a)$ donnée par $k\mapsto [c_{\gamma(k)}]$ est injective. En particulier, Card($\pi_1(X, a)$)$\geqslant$ Card($\{0,1\}^{\mathbf{N}}$) $=$ Card($\mathfrak{P}(\mathbf{N})$). Comme X est un espace topologique métrisable de type dénombrable, il en est de même de $\Omega_a(X)$ (TG, X, p. 24, th. 1). Par suite, $\Omega_a(X)$ est homéomorphe à un sous-espace de $[0,1]^{\mathbf{N}}$ (TG, IX, p. 18, prop. 12) et

Card(Ω$_a(X))\leqslant$ Card([0$,1]^{\mathbf{N}}) =$ Card($\mathfrak{P}(\mathbf{N})^{\mathbf{N}}$)

= Card($\mathfrak{P}(\mathbf{N}\times \mathbf{N})$) $=$ Card($\mathfrak{P}(\mathbf{N})$).

A fortiori, Card($\pi_1(X, a)$)$\leqslant$ Card($\mathfrak{P}(\mathbf{N})$). Il résulte alors du cor. 2 de E, III, p. 25, que $\pi_1(X, a)$ a la puissance du continu, ce qu’il fallait démontrer.

#### Exemple {#ta-iv-s2-n6-exa-1 .statement tag=021L}

Soit P l’espace topologique réunion des cercles de centre $(2/n,0)$ passant par l’origine du plan $\mathbf{R}^2$, pour $n\geqslant$ 1 (III, p. 336, exerc. 6). Le groupe de Poincaré de P a la puissance du continu (III, p. 338, exerc. 9).

## EXERCICES {#ta-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: Voir « Can the fundamental (homotopy) group of a space be the rationals ? », Proc. Amer. Math. Soc. 103 (1988), no. 2, p. 627–632. La preuve qui suit est basée sur l’article de J. Pawlikowski, « The fundamental group of a compact metric space », Proc. Amer. Math. Soc. 126 (1998), no. 10, p. 3083–3087.
