---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 2
section_title: Homotopie et chemins
lang: fr
source: ta-i-iv-fr
book_pages: TA III.256-TA III.289, TA III.330-TA III.333
pdf_pages: 0272-0305, 0346-0349
extraction: native
subsections:
    - "no": 1
      title: Chemins
      page: 256
      pdf_page: 272
    - "no": 2
      title: Espaces connexes par arcs
      page: 258
      pdf_page: 274
    - "no": 3
      title: Espaces localement connexes par arcs
      page: 260
      pdf_page: 276
    - "no": 4
      title: Liens entre connexité et connexité par arcs
      page: 264
      pdf_page: 280
    - "no": 5
      title: Applications continues par arcs
      page: 267
      pdf_page: 283
    - "no": 6
      title: Compléments sur les espaces topologiques compacts métrisables
      page: 269
      pdf_page: 285
    - "no": 7
      title: Propriétés topologiques de l’image d’un chemin
      page: 272
      pdf_page: 288
    - "no": 8
      title: Caractérisations de l’intervalle
      page: 274
      pdf_page: 290
    - "no": 9
      title: Chemins injectifs
      page: 282
      pdf_page: 298
    - "no": 10
      title: Relèvement de chemins
      page: 284
      pdf_page: 300
statements: 63
exercises: 14
content_sha256: 7cd85effc05cceb599f6fbd00c47f8adf6d1b44ae268c4c9331ea9ff51987a57
---

## § 2. HOMOTOPIE ET CHEMINS

### 1. Chemins

#### Définition 1 {#ta-iii-s2-def-1 .statement tag=01WN}

Soit X un espace topologique. On appelle chemin dans X toute application continue $c$ de $\mathbf{I}$ dans X. Le point $c(0)$ est appelé l’ origine, le point $c(1)$ le terme du chemin $c$. On appelle lacet dans X un chemin dans X dont l’origine est égale au terme.

Soient $x$ et $y$ des points de X. On dit qu’un chemin $c$ dans X relie $x$ à $y$ si $x$ est son origine et $y$ son terme.

#### Définition 2 {#ta-iii-s2-def-2 .statement tag=01WO}

Soit X un espace topologique. On dit que des chemins $c$ et $d$ dans X sont juxtaposables si l’on a $c(1) =d(0)$. On appelle alors chemin juxtaposé de $c$ et $d$ le chemin $c*d$ défini par la formule :

$c(2t)$ pour $0\leqslant t\leqslant 1/2$,

$$
(c*d)(t) = \tag{1}
$$

$d(2t-1)$ pour $1/2\leqslant t\leqslant 1$.

Son origine est l’origine de $c$, son terme celle de $d$.

Soit $c$ un chemin dans X ; on appelle chemin opposé à $c$ et on note $\overline{c}$le chemin défini par $\overline{c}(t) =c(1-t)$ pour $t\in \mathbf{I}$.

Si $c$ et $d$ sont deux chemins juxtaposables dans X$,\overline{d}$ et $\overline{c}$ le sont, et l’on a $\overline{c*d}=\overline{d}*\overline{c}$. Pour tout chemin $c$ dans X, on a $\overline{\overline{c}}=c$.

#### Remarque 1 {#ta-iii-s2-n1-rem-1 .statement tag=01WP}

Soit X un espace topologique et soit P un espace topologique réduit à un point. Identifions $P\times \mathbf{I}$ à $\mathbf{I}$ par la projection pr$_2$. L’ensemble $\mathscr{C}(P\times \mathbf{I}; X)$ des homotopies entre applications (nécessairement continues) de P dans X s’identifie alors à l’ensemble $\mathscr{C}(\mathbf{I}; X)$ des chemins dans X. À une homotopie reliant l’application constante d’image $x$ à l’application constante d’image $y$ correspond un chemin d’origine $x$ et de terme $y$. Les identifications précédentes sont compatibles avec les notions de juxtaposition et de passage à l’opposé (cf. III, p. 230).

#### Remarque 2 {#ta-iii-s2-n1-rem-2 .statement tag=01WQ}

Soient X et Y des espaces topologiques. L’application canonique

$$
\mathscr{C}(X\times \mathbf{I}; Y)\rightarrow \mathscr{C}(\mathbf{I};\mathscr{C}_c(X; Y))
$$

associe à toute homotopie $\sigma : X\times \mathbf{I}\rightarrow Y$ reliant deux applications $f$ et $g$ de X dans Y un chemin d’origine $f$, de terme $g$, dans l’espace $\mathscr{C}_c(X; Y)$. Si X est un espace localement compact, cette application canonique est bijective (TG, X, p. 28, théorème 3).

Soit X un espace topologique. On appelle espace des chemins de X, et on note Λ(X), l’espace topologique $\mathscr{C}_c(\mathbf{I}; X)$ dont les éléments sont les chemins dans X et dont la topologie est celle de la convergence compacte (cf. TG, X, p. 27). Si $x$ est un point de X, on note $\Lambda_x(X)$ le sous-espace de Λ(X) formé des chemins d’origine $x$. Si $y$ est un second point de X, on note $\Lambda_{x,y}(X)$ le sous-espace de Λ(X) formé des chemins d’origine $x$ et de terme $y$.

#### Proposition 1 {#ta-iii-s2-prop-1 .statement tag=01WR}

Soient X et Z des espaces topologiques. Pour qu’une application $\varphi$ de Z dans l’espace des chemins $\mathscr{C}_c(\mathbf{I}; X)$ soit continue, il faut et il suffit que l’application $(z, t)\mapsto \varphi (z)(t)$ soit une application continue de $Z\times \mathbf{I}$ dans X. En particulier, l’application $(c, t)\mapsto c(t)$ de $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ dans X est continue.

L’espace topologique $\mathbf{I}$ étant localement compact, la proposition résulte de TG, X, p. 28, th. 3.

On note $o$ et on appelle application origine l’application $c\mapsto c(0)$ de Λ(X) dans X ; on note $e$ et on appelle application terme l’application $c\mapsto c(1)$ de Λ(X) dans X. Les applications $o$ et $e$ sont continues (TG, X, p. 27, remarque 1). Les couples de chemins juxtaposables dans X sont les éléments du produit fibré des X-espaces $(\Lambda (X), e)$ et $(\Lambda (X), o)$.

#### Proposition 2 {#ta-iii-s2-prop-2 .statement tag=01WS}

Soit X un espace topologique. L’application qui à un chemin $c$ associe le chemin opposé $\overline{c}$ est un homéomorphisme de Λ(X) sur lui-même. La juxtaposition des chemins $(c, d)\mapsto c*d$ est un homéomorphisme de l’espace $(\Lambda (X), e)\times_X(\Lambda (X), o)$ sur Λ(X).

L’application $t\mapsto 1-t$ est un homéomorphisme de l’espace $\mathbf{I}$ sur lui-même ; la première assertion en résulte.

Notons C le produit fibré $(\Lambda (X), e)\times_X(\Lambda (X), o)$. Notons $\gamma : C\rightarrow$ Λ(X) l’application $(c, d)\mapsto c*d$ et $\delta : C\times \mathbf{I}\rightarrow$ X l’application $((c, d), t)\mapsto (c*d)(t)$. Les restrictions de l’application $\delta$ à $C\times [0,\frac{1}{2}]$ et $C\times [\frac{1}{2},1]$ sont continues en vertu de la formule (1) et de la prop. 1. L’application $\delta$ est donc continue (TG, I, p. 19, prop. 4), ainsi que l’application $\gamma$ (prop. 1). On a $c(t) = (c*d)(\frac{t}{2})$ et $d(t) = (c*d)(\frac{1+t}{2})$, donc $\gamma$ est injective.

Soit $g$ un chemin dans X ; pour $t\in \mathbf{I}$, posons

$$
t1 +t
$$

$c_g(t) =g$ et $d_g(t) =g$.

2 2

Les applications $c_g$ et $d_g$ ainsi définies sont des chemins juxtaposables dans X et l’on a $c_g*d_g=g$. En outre, les applications $g\mapsto c_g$ et $g\mapsto d_g$ sont des applications continues de l’espace Λ(X) dans lui-même (prop. 1). Il en résulte que l’application $\gamma$ est un homéomorphisme.

#### Corollaire {#ta-iii-s2-n1-cor-1 .statement tag=01WT}

Soit X un espace topologique et soient $x,y,z$ des points de X. Les applications $c\mapsto \overline{c}$ de $\Lambda_{x,y}(X)$ dans $\Lambda_{y,x}(X)$ et $(c, d)\mapsto$ $c*d$ de $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ dans $\Lambda_{x,z}(X)$ sont continues.

### 2. Espaces connexes par arcs

#### Définition 3 {#ta-iii-s2-def-3 .statement tag=01WU}

Un espace topologique X est dit connexe par arcs si pour tout couple $(x, y)$ de points de X, il existe un chemin d’origine $x$ et de terme $y$.

#### Exemple 1 {#ta-iii-s2-n2-exa-1 .statement tag=01WV}

Tout intervalle de $\mathbf{R}$, toute partie convexe d’un espace numérique ou, plus généralement, d’un espace vectoriel topologique sur $\mathbf{R}$ est connexe par arcs.

#### Proposition 3 {#ta-iii-s2-prop-3 .statement tag=01WW}

L’image par une application continue d’un espace connexe par arcs est connexe par arcs.

Soient X un espace connexe par arcs, $f: X\rightarrow Y$ une application continue. Soient $x$ et $y$ deux points de $f(X)$ ; soient $x'$ et $y'$ des points de X tels que $f(x') =x$ et $f(y') =y$. Il existe un chemin $c$ dans X dont l’origine est $x'$ et le terme $y'$. Alors, $f\circ c$ est un chemin dans $f(X)$ d’origine $x$ et de terme $y$.

#### Proposition 4 {#ta-iii-s2-prop-4 .statement tag=01WX}

Un espace topologique connexe par arcs est connexe.

Comme tout intervalle de $\mathbf{R}$ est connexe, l’image d’un chemin est connexe (TG, I, p. 82, prop. 4). L’espace vide est connexe. Puisqu’un espace connexe par arcs non vide est réunion des images des chemins issus de l’un de ses points, il est connexe (TG, I, p. 81, prop. 2).

Compte tenu de l’identification (III, p. 256, remarque 1) des chemins dans X aux homotopies entre applications d’un espace topologique P réduit à un point dans X, la proposition 1 de III, p. 230 entraîne :

#### Proposition 5 {#ta-iii-s2-prop-5 .statement tag=01WY}

Dans un espace topologique, la relation « il existe un chemin d’origine $x$ et de terme $y$ » est une relation d’équivalence.

On appelle composantes connexes par arcs d’un espace topologique X les classes d’équivalence pour la relation ci-dessus. Une composante connexe par arcs est un espace connexe par arcs. Soit $x$ un point de X. La composante connexe par arcs de $x$ est la réunion des sous-espaces connexes par arcs de X contenant $x$. C’est aussi la réunion des images des chemins d’origine $x$ dans X.

#### Exemple 2 {#ta-iii-s2-n2-exa-2 .statement tag=01WZ}

La réunion d’une famille d’ensembles connexes par arcs, dont l’intersection n’est pas vide, est connexe par arcs (cf. TG, I, p. 81, prop. 2).

#### Exemple 3 {#ta-iii-s2-n2-exa-3 .statement tag=01X0}

Une partie d’un espace numérique (ou, plus généralement, un espace vectoriel topologique sur $\mathbf{R})$ qui est étoilée en un de ses points est connexe par arcs.

Soit X un espace topologique. On désigne par $\pi_0(X)$ l’ensemble des composantes connexes par arcs de X. Soit P un espace topologique réduit à un point. L’application de X dans [P; X] qui, à tout point $x$ de X, associe la classe d’homotopie $\varphi_x$ de l’application $f_x: P\rightarrow X$ d’image $x$, définit par passage au quotient une bijection, dite canonique, de $\pi_0(X)$ sur [P; X]. On a $\pi_0(\emptyset ) =\emptyset$. Pour qu’un espace topologique non vide soit connexe par arcs, il faut et il suffit que $\pi_0(X)$ soit un ensemble à un élément.

Soient X et Y des espaces topologiques et $f: X\rightarrow Y$ une application continue. L’image $f(C)$ de toute composante connexe par arcs C de X est connexe par arcs (III, p. 258, prop. 3), donc contenue dans une composante connexe par arcs de Y. On note $\pi_0(f):\pi_0(X)\rightarrow \pi_0(Y)$ l’application qui, à une composante connexe par arcs C de X, associe l’unique composante connexe par arcs $C'$ de Y telle que $f(C)\subset C'$. Si l’on identifie $\pi_0(X)$ et $\pi_0(Y)$ à [P; X] et [P; Y] respectivement, l’application $\pi_0(f)$ s’identifie à l’application $\chi \mapsto [f]\circ \chi$ de [P; X] dans [P; Y]. En particulier, si $f$ et $g$ sont des applications homotopes de X dans Y, on a $\pi_0(f) =\pi_0(g)$ (III, p. 230, prop. 2).

Soit Z un espace topologique et soit $g: Y\rightarrow$ Z une application continue ; on a $\pi_0(g\circ f) =\pi_0(g)\circ \pi_0(f)$. En particulier, si Z = X et si $f$ et $g$ sont des homéotopies réciproques l’une de l’autre à homotopie près, on a $\pi_0(g)\circ \pi_0(f) =\pi_0$(Id$_X) =$ Id$_{\pi_0(X)}$ et $\pi_0(f)\circ \pi_0(g) =\pi_0$(Id$_Y) =$ Id$_{\pi_0(Y)}$, ce qui prouve que $\pi_0(f)$ et $\pi_0(g)$ sont des bijections réciproques l’une de l’autre. Un espace homéotope à un espace connexe par arcs est donc lui-même connexe par arcs. En particulier, un espace homéotope à un point est connexe par arcs.

#### Proposition 6 {#ta-iii-s2-prop-6 .statement tag=01X1}

Soit $(Y_j)_{j\in J}$ une famille d’espaces topologiques. L’application

$(\pi_0$(pr$_j)):\pi_0(\prod_{j\in J}Y_j)\rightarrow \prod_{j\in J}\pi_0(Y_j)$

est bijective. En particulier, l’espace produit d’une famille d’espaces connexes par arcs est connexe par arcs.

Cela résulte de la proposition 3 de III, p. 231 où l’on prend pour X un espace réduit à un point.

### 3. Espaces localement connexes par arcs

#### Définition 4 {#ta-iii-s2-def-4 .statement tag=01X2}

Un espace topologique est dit localement connexe par arcs si chacun de ses points possède un système fondamental de voisinages connexes par arcs.

#### Proposition 7 {#ta-iii-s2-prop-7 .statement tag=01X3}

Un espace topologique localement connexe par arcs est localement connexe. Ses composantes connexes coïncident avec ses composantes connexes par arcs. En particulier, si un espace topologique localement connexe par arcs est connexe, il est connexe par arcs.

La première assertion résulte de la prop. 4. Démontrons la seconde assertion. Soit X un espace topologique localement connexe par arcs et soit C une composante connexe par arcs de X. Tout point de C possède un voisinage connexe par arcs, donc contenu dans C ; par suite, C est une partie ouverte de X. Les composantes connexes par arcs formant une partition de X, une telle composante est aussi fermée. Comme elle est connexe (III, p. 258, prop. 4), c’est une composante connexe (TG, I, p. 83). La troisième assertion résulte de la seconde.

Remarquons ainsi qu’il n’y a pas d’ambiguïté à dire qu’un espace topologique est connexe et localement connexe par arcs.

#### Corollaire 1 {#ta-iii-s2-prop-7-cor-1 .statement tag=01X4}

Tout ouvert connexe d’un espace topologique localement connexe par arcs est connexe par arcs.

#### Corollaire 2 {#ta-iii-s2-prop-7-cor-2 .statement tag=01X5}

Soit B un espace topologique localement connexe par arcs et soit E un B-espace étalé. L’espace E est localement connexe par arcs. S’il est connexe, il est connexe par arcs.

La première assertion découle aussitôt de la déf. 4 et de la définition d’une application étale (I, p. 28, déf. 2). La seconde s’en déduit par la prop. 7.

Pour qu’un espace topologique X soit localement connexe par arcs, il faut et il suffit que toute composante connexe par arcs d’un ensemble ouvert de X soit un ensemble ouvert de X (cf. I, p. 85, démonstration de la prop. 11). Si l’espace X est localement connexe par arcs, tout point de X possède donc un système fondamental de voisinages ouverts connexes par arcs.

#### Proposition 8 {#ta-iii-s2-prop-8 .statement tag=01X6}

Tout espace quotient d’un espace localement connexe par arcs est localement connexe par arcs.

Soit X un espace localement connexe par arcs, soit R une relation d’équivalence dans X et soit $\varphi : X\rightarrow X/R$ l’application canonique. Il suffit de démontrer que les composantes connexes par arcs d’un ouvert de $X/R$ sont ouvertes. Soit ainsi A une partie ouverte de $X/R$ et soit C une composante connexe par arcs de A. Soit $x\in \overset{-1}{\varphi}(C)$, et soit K la composante connexe par arcs de $x$ dans $\overset{-1}{\varphi}(A)$. L’ensemble $\varphi (K)$ est connexe par arcs (III, p. 258, prop. 3), contenu dans A et contient $\varphi (x)$ ; on a donc $\varphi (K)\subset C$, d’où $K\subset \overset{-1}{\varphi}(C)$. Cela prouve que $\overset{-1}{\varphi}(C)$ est réunion de composantes connexes par arcs de $\overset{-1}{\varphi}(A)$. Comme X est localement connexe par arcs et que $\overset{-1}{\varphi}(A)$ est ouvert dans X$,\overset{-1}{\varphi}(C)$ est ouvert dans X. Par suite, C est ouvert dans $X/R$. Cela démontre la proposition.

#### Proposition 9 {#ta-iii-s2-prop-9 .statement tag=01X7}

Le produit d’une famille d’espaces localement connexes par arcs, connexes à l’exception d’un nombre fini d’entre eux, est localement connexe par arcs.

Soit $(X_j)_{j\in J}$ une famille d’espaces localement connexes par arcs qui soient connexes, à l’exception d’un nombre fini d’entre eux. Soit $x=$ $(x_j)_{j\in J}$ un point de l’espace produit X = $\prod_{j\in J}X_j$. Par hypothèse, un système fondamental de voisinages de $x$ dans X est constitué des ensembles de la forme $V =\prod_{j\in J}V_j$ où, pour tout $j\in J$, $V_j$ est un voisinage connexe par arcs de $x_j$ dans $X_j$ et où $V_j= X_j$ sauf pour un ensemble fini d’indices $j\in J$ (TG, I, p. 24). Ces ensembles étant connexes par arcs (III, p. 260, prop. 6), X est localement connexe par arcs.

#### Corollaire {#ta-iii-s2-n3-cor-1 .statement tag=01X8}

Toute partie ouverte d’un espace numérique est localement connexe par arcs.

Tout point de $\mathbf{R}$ possède une base de voisinages formée d’intervalles ; par suite, $\mathbf{R}$ est localement connexe par arcs. D’après la proposition 9, l’espace numérique $\mathbf{R}^n$ est localement connexe par arcs, pour tout entier $n\geqslant 1$. En outre, un ouvert d’un espace topologique localement connexe par arcs est encore connexe par arcs, d’où le corollaire.

#### Exemple {#ta-iii-s2-n3-exa-1 .statement tag=01X9}

Soit G le sous-groupe de $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ formé des matrices carrées d’ordre $n$ dont le déterminant est strictement positif. Le groupe G est connexe et localement connexe par arcs.

D’après A, III, p. 104, prop. 17, le groupe $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ est engendré par les éléments $B_{ij}(\lambda )$ (pour $1\leqslant i, j\leqslant n$ tels que $i=\not j$ et $\lambda \in \mathbf{R})$. Les applications $\lambda \mapsto B_{ij}(\lambda )$ de $\mathbf{R}$ dans $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ sont continues, leurs images sont des parties connexes de $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ ; comme elles contiennent toutes la matrice identité $I_n$, leur réunion est connexe (TG, I, p. 81, prop. 2). Par suite, le groupe $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ est connexe (TG, III, p. 8, prop. 7). Soit A le sous-groupe de G formé des matrices de la forme diag(1$, . . . ,1, \lambda )$, avec $\lambda \in \mathbf{R}_+^*$; il est connexe et l’on a $\mathbf{G}\mathbf{L}(n,\mathbf{R}) = A\cdot \mathbf{S}\mathbf{L}(n,\mathbf{R})$. Il en résulte que le groupe G est connexe. Comme c’est l’image réciproque de $\mathbf{R}_+^*$ par l’application déterminant de $\mathbf{M}_n(\mathbf{R})$ dans $\mathbf{R}$, c’est un ouvert de $\mathbf{M}_n(\mathbf{R})$ ; il est donc localement connexe par arcs (corollaire ci-dessus), ainsi que connexe par arcs (III, p. 261, corollaire 1).

#### Proposition 10 {#ta-iii-s2-prop-10 .statement tag=01XA}

Soit X un espace topologique. L’application $(o, e)$ de $\Lambda (X) =\mathscr{C}_c(\mathbf{I}; X)$ dans $X\times X$, qui à un chemin $c$ dans X associe le couple $(c(0), c(1))$, est continue. Si l’espace X est localement connexe par arcs, cette application est ouverte.

Nous savons déjà que les applications origine $o$ et terme $e$ de Λ(X) dans X sont continues (III, p. 257), d’où la première assertion.

#### Lemme {#ta-iii-s2-n3-lem-1 .statement tag=01XB}

Soit $c:\mathbf{I}\rightarrow X$ un chemin et soit W un voisinage de $c$ dans l’espace $\mathscr{C}_c(\mathbf{I}; X)$. Il existe un nombre réel $\varepsilon \in ]0,1/2]$, un voisinage $V_0$ de $c(0)$ et un voisinage $V_1$ de $c(1)$ dans X ayant les propriétés suivantes : on a $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1$, et tout chemin $c':\mathbf{I}\rightarrow X$ tel que

$c'(t)\in V_0$ pour $0\leqslant t\leqslant \varepsilon$,

(2) $c'(t) =c(t)$ pour $\varepsilon \leqslant t\leqslant 1-\varepsilon$,

$c'(t)\in V_1$ pour $1-\varepsilon \leqslant t\leqslant 1$,

appartient à W.

Par définition de la topologie de la convergence compacte (TG, X, p. 26, déf. 1), il existe un ensemble fini J, une famille $(U_j)_{j\in J}$ d’ensembles ouverts dans X et une famille $(K_j)_{j\in J}$ de parties compactes de $\mathbf{I}$ tels que l’ensemble $W'$ des chemins $c'$ vérifiant $c'(K_j)\subset U_j$ pour tout indice $j$ soit un voisinage de $c$ contenu dans W. Notons alors $A_0$ (resp. $A_1)$ l’ensemble des indices $j$ tels que $0\in K_j$ (resp. $1\in K_j)$; posons $V_0=\bigcap_{j\in A_0}U_j$ et $V_1=\bigcap_{j\in A_1}U_j$.

Comme l’application $c$ est continue, il existe un nombre réel $\varepsilon \in$ $]0,1/2]$ tel que $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1,[0, \varepsilon ]\cap K_j=\emptyset$ pour tout $j\notin A_0$ et $[1-\varepsilon ,1]\cap K_j=\emptyset$ pour tout $j\notin A_1$. Soit alors $c'$ un chemin satisfaisant aux conditions (2). Démontrons que $c'\in W'$. Soit $j\in J$ et soit $t\in K_j$. Si $\varepsilon \leqslant t\leqslant 1-\varepsilon ,c'(t) =c(t)$ appartient à $U_j$. Si $0\leqslant t\leqslant \varepsilon ,c'(t)\in V_0$; par le choix de $\varepsilon$, on a $j\in A_0$, donc $c'(t)\in U_j$. De même, si $1-\varepsilon \leqslant t\leqslant 1$, on a $j\in A_1$ et $c'(t)\in V_1\subset U_j$. Ainsi, $c'(K_j)\subset U_j$ et $c'$ appartient à $W'$, donc à W.

Démontrons maintenant la seconde assertion de la prop. 10. Supposons l’espace X localement connexe par arcs. Soit $c$ un chemin dans X et soit W un voisinage de $c$ dans $\mathscr{C}_c(\mathbf{I}; X)$. Soient $\varepsilon ,V_0$ et $V_1$ comme dans le lemme. Soient $T_0$ et $T_1$ des voisinages connexes par arcs de $c(0)$ et $c(1)$ contenus dans $V_0$ et $V_1$ respectivement. Il existe un nombre réel $\theta$ tel que $0< \theta  < \varepsilon$ et tel que $c([0, \theta ])\subset T_0,c([1-\theta ,1])\subset T_1$. Soient $x_0\in T_0$ et $x_1\in T_1$; soit $c_0$ un chemin d’origine $x_0$ et de terme $c(\theta )$ dans $T_0$ et soit $c_1$ un chemin d’origine $x_1$ et de terme $c(1-\theta )$ dans $T_1$. Posons

$c_0(t/\theta )$ pour $0\leqslant t\leqslant \theta$,

$c'(t) =c(t)$ pour $\theta \leqslant t\leqslant 1-\theta$,

$c_1((1-t)/\theta )$ pour $1-\theta \leqslant t\leqslant 1$.

On définit ainsi un chemin $c'$ reliant $x_0$ à $x_1$ et satisfaisant aux conditions (2). Cela prouve que l’image de W dans $X\times X$ par l’application $(o, e)$ contient le voisinage $T_0\times T_1$ de $(c(0), c(1))$, d’où la proposition.

#### Corollaire {#ta-iii-s2-n3-cor-2 .statement tag=01XC}

Soit X un espace topologique localement connexe par arcs et soit $x$ un point de X. L’application $c\mapsto c(1)$ de $\Lambda_x(X)$ dans X est ouverte.

D’après la proposition, l’application $\varphi : \Lambda (X)\rightarrow X\times X$ définie par $\varphi (c) = (c(0), c(1))$ est ouverte et l’on a $\Lambda_x(X) =\overset{-1}{\varphi}(\{x\} \times X)$. Par suite, l’application $\Lambda_x(X)\rightarrow  \{x\} \times X$ déduite de $\varphi$ est ouverte (TG, I, p. 30, prop. 2), ainsi que sa composée avec la seconde projection pr$_2$.

### 4. Liens entre connexité et connexité par arcs

Un espace connexe par arcs est connexe (III, p. 258, prop. 4). Il existe des espaces connexes, même localement connexes, qui ne sont pas connexes par arcs (cf. III, p. 331, exerc. 2 et 4). Cependant :

#### Proposition 11 {#ta-iii-s2-prop-11 .statement tag=01XD}

Un espace topologique connexe et localement connexe, dont la topologie peut être définie par une distance pour laquelle il est complet, est connexe par arcs.

Soit X un espace topologique. Appelons train dans X toute suite finie non vide $T = (W_i)_{1\leqslant i\leqslant n}$ de parties ouvertes connexes de X telles que $W_i\cap W_{i+1}=\not\emptyset$ pour $1\leqslant i\leqslant n-1$. On dit que $n$ est la longueur du train T et que les $W_i$ sont ses wagons. Si X est muni d’une distance compatible avec sa topologie, on appelle largeur du train T le maximum des diamètres de ses wagons. On dit que le train joint un point $a$ à un point $b$ si $a$ appartient au premier et $b$ au dernier wagon. On appelle raffinement de T tout couple $(T', f)$ formé d’un train $T'= (W'_j)_{1\leqslant j\leqslant m}$ et d’une application strictement croissante $f:\{0,1, . . . , n\} \rightarrow  \{0,1, . . . , m\}$ telle que $f(0) = 0,f(n) =m$ et $W'_j\subset W_i$ pour $1\leqslant i\leqslant n$ et $f(i-1)< j\leqslant f(i)$.

#### Lemme 1 {#ta-iii-s2-lem-1 .statement tag=01XE}

Soit X un espace métrique connexe et localement connexe, soient $a$ et $b$ des points de X et soit $\varepsilon$ un nombre réel $>0$. Il existe dans X un train de largeur $\leqslant \varepsilon$ joignant $a$ à $b$.

Plus précisément, tout train T joignant $a$ à $b$ possède un raffinement $(T', f)$, où $T'$ est un train de largeur $\leqslant \varepsilon$ joignant $a$ à $b$.

La relation « il existe un train de largeur $\leqslant \varepsilon$ joignant $x$ à $y$ » est une relation d’équivalence entre $x$ et $y$ dans X. La classe d’équivalence d’un point $x$ contient tout voisinage ouvert connexe de $x$ de diamètre $\leqslant \varepsilon$, et $x$ possède un tel voisinage puisque X est localement connexe. Les classes d’équivalence suivant cette relation sont donc ouvertes, et par suite aussi fermées. Il y en a au plus une, puisque X est connexe. Cela démontre la première assertion.

Soit $T = (W_i)_{1\leqslant i\leqslant n}$ un train dans X joignant $a$ à $b$. Posons $x_0=a$, $x_n=b$ et choisissons pour $1\leqslant i\leqslant n-1$ un point $x_i$ dans l’ensemble non vide $W_i\cap W_{i+1}$. Pour $1\leqslant i\leqslant n$, l’ensemble ouvert $W_i$ est connexe et localement connexe et $x_{i-1},x_i$ sont deux de ses points ; il existe d’après l’alinéa précédent un train $(W_{i,k})_{1\leqslant k\leqslant m_i}$ dans $W_i$, de largeur $\leqslant \varepsilon$, joignant $x_{i-1}$ à $x_i$.

Posons $m=m_1+\cdots +m_n$. Pour $1\leqslant j\leqslant m$, posons $W'_j= W_{i,k}$, où $(i, k)$ est l’unique couple d’entiers tel que $1\leqslant i\leqslant n,1\leqslant k\leqslant m_i$ et $j=m_1+\cdots +m_{i-1}+k$. Pour $0\leqslant i\leqslant n$, posons $f(i) =m_1+\cdots +m_i$. Alors $T'= (W'_j)_{1\leqslant j\leqslant m}$ est un train de largeur $\leqslant \varepsilon$ dans X joignant $a$ à $b$, et $(T', f)$ est un raffinement de T.

Démontrons maintenant la proposition 11. Munissons l’espace connexe et localement connexe X d’une distance $d$, compatible avec sa topologie, pour laquelle il est complet. Soient $a$ et $b$ des points de X. Le lemme 1 permet de construire par récurrence des suites $(T_s)_{s\geqslant 0}$ et $(f_s)_{s\geqslant 1}$ telles que, pour tout $s\geqslant 0$, $T_s= (W_{s,i})_{1\leqslant i\leqslant n_s}$ soit un train de largeur $\leqslant 2^{-s}$ joignant $a$ à $b$ et $(T_{s+1}, f_{s+1})$ soit un raffinement de $T_s$.

Nous pouvons choisir par récurrence, pour $s\geqslant 0$, une application strictement croissante $g_s:\{0,1, . . . , n_s\} \rightarrow \mathbf{I}$ telle que $g_s(0) = 0$ et $g_s(n_s) = 1$, de telle sorte que $g_{s+1}\circ f_s=g_s$. Définissons, pour $s\geqslant 0$, une partie $A_s$ de $\mathbf{I}\times X$ en posant

$$
A_s=\bigcup_{1\leqslant i\leqslant n_s}([g_s(i-1), g_s(i)]\times W_{s,i})
$$

La suite $(A_s)_{s\geqslant 0}$ est décroissante : en effet, pour tout entier $j\in  \{1, . . . , n_{s+1}\}$, il existe un unique entier $i\in  \{1, . . . , n_s\}$ tel que $f_s(i-1)< j\leqslant f_s(i)$, et l’on a

$$
[g_{s+1}(j-1), g_{s+1}(j)]\subset [g_s(i-1), g_s(i)],W_{s+1,j}\subset W_{s,i}
$$

Soit $t\in \mathbf{I}$. Pour tout $s\geqslant 0$, notons $A_s(t)$ l’ensemble des $x\in X$ tels que $(t, x)\in A_s$. L’ensemble $A_s(t)$ est soit l’un des wagons, soit la réunion de deux wagons consécutifs du train $T_s$; c’est donc une partie non vide de X, de diamètre $\leqslant 2^{1-s}$. La suite $(A_s(t))_{s\geqslant 0}$ est décroissante. L’ensemble de ses termes est une base de filtre de Cauchy. Celle-ci converge vers un point $c(t)$ puisque l’espace métrique X est complet.

Comme $a$ appartient à chacun des ensembles $A_s(0) = W_{s,1}$, on a $c(0) =a$; on a de même $c(1) =b$. Soit $t\in \mathbf{I}$ et soit $s$ un entier $\geqslant 0$. Le point $t$ possède dans $\mathbf{I}$ un voisinage V de l’une des formes suivantes : $[g_s(0), g_s(1)[$, $]g_s(i-1), g_s(i+ 1)[$ pour un entier $i$ tel que $1\leqslant i\leqslant$ $n_s-1$, ou $]g_s(n_s-1), g_s(n_s)]$. Suivant le cas, l’ensemble $c(V)$ est contenu dans l’adhérence du premier wagon, de la réunion de deux wagons consécutifs, ou du dernier wagon du train $T_s$. Il est donc de diamètre $\leqslant 2^{1-s}$, et l’on a $d(c(t), c(t'))\leqslant 2^{1-s}$ pour $t'\in V$. Cela prouve que l’application $c:\mathbf{I}\rightarrow$ X est continue. Ainsi $c$ est un chemin dans X reliant $a$ à $b$, et X est connexe par arcs.

#### Corollaire 1 {#ta-iii-s2-lem-1-cor-1 .statement tag=01XF}

Un espace topologique localement connexe, dont la topologie peut être définie par une distance pour laquelle il est complet, est localement connexe par arcs.

Soit X un tel espace et soit U une partie ouverte et connexe de X. D’après le lemme 2 ci-dessous, il existe une distance sur U compatible avec sa topologie pour laquelle U est complet. Comme U est localement connexe, il résulte de la proposition 11 que U est connexe par arcs.

#### Lemme 2 {#ta-iii-s2-lem-2 .statement tag=01XG}

Soit X un espace métrique complet et soit U une partie ouverte de X. Il existe une distance sur U compatible avec sa topologie pour laquelle U est complet.

Nous reprendrons les arguments de la démonstration de la prop. 2 de TG, IX, p. 57. Nous pouvons supposer U distinct de X. Soit V la partie du produit $\mathbf{R}\times X$ formée des points $(t, x)$ tels que $t d(x,X-U) = 1$ ; le sous-espace V de $\mathbf{R}\times X$ est fermé et l’application $(t, x)\mapsto x$ de V dans U est un homéomorphisme (TG, IX, p. 13, prop. 3). Il existe sur $\mathbf{R}\times X$ une distance $d'$ compatible avec sa topologie pour laquelle $\mathbf{R}\times X$ est complet (TG, IX, p. 15, cor. 2 et TG, II, p. 17, prop. 10). L’espace V est complet pour la distance induite par $d'$ (TG, II, p. 16, prop. 8), d’où le lemme.

#### Corollaire 2 {#ta-iii-s2-lem-2-cor-2 .statement tag=01XH}

Un espace topologique localement compact, localement connexe et métrisable est localement connexe par arcs. S’il est connexe, il est connexe par arcs.

Il suffit de démontrer la première assertion (III, p. 260, prop. 7). Soit X un espace métrique localement compact et localement connexe. Les ensembles ouverts, connexes et relativement compacts de X constituent une base de la topologie de X. Soit U un tel ensemble ; comme U est un ouvert de son adhérence, laquelle est un espace métrique compact, donc complet, il existe d’après le lemme 2 une distance sur U compatible avec sa topologie pour laquelle U est complet. Il résulte de la prop. 11 de III, p. 264 que U est connexe par arcs, d’où le corollaire.

### 5. Applications continues par arcs

#### Définition 5 {#ta-iii-s2-def-5 .statement tag=01XI}

Soient X et Y des espaces topologiques. On dit qu’une application $f: X\rightarrow Y$ est continue par arcs si, pour tout chemin $c$ dans X, l’application $f\circ c:\mathbf{I}\rightarrow Y$ est continue.

#### Remarque {#ta-iii-s2-n5-rem-1 .statement tag=01XJ}

Supposons que l’espace X soit connexe par arcs. Soit $x$ un point de X. Pour que $f$ soit continue par arcs, il suffit que, pour tout chemin $c$ d’origine $x$, l’application $f\circ c$ soit continue. Soit en effet $d$ un chemin quelconque dans X et soit $c$ un chemin dans X d’origine $x$ et de terme $d(0)$. Si l’application $f\circ (c*d)$ est continue, il en est de même de l’application $f\circ d$ car on a $f\circ d(t) =f\circ (c*d)((t+ 1)/2)$.

Une application continue est continue par arcs. La réciproque n’est pas toujours vraie ; les propositions 12 et 13 ci-dessous fournissent des critères permettant d’affirmer qu’une application continue par arcs est continue.

#### Proposition 12 {#ta-iii-s2-prop-12 .statement tag=01XK}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application. Supposons que l’espace X soit localement connexe par arcs et que tout point de X possède un système fondamental dénombrable de voisinages. Si l’application $f$ est continue par arcs, elle est continue.

D’après (TG, IX, p. 18), il suffit de démontrer que, pour tout point $x$ de X et toute suite $(x_n)_{n\geqslant 1}$ de points de X qui tend vers $x$, la suite $(f(x_n))_{n\geqslant 1}$ tend vers $f(x)$. En supprimant éventuellement les premiers termes de la suite $(x_n)_{n\geqslant 1}$, on se ramène au cas où les termes de la suite appartiennent tous à un même voisinage connexe par arcs de $x$ dans X. D’après le lemme ci-dessous, il existe alors un chemin $c:\mathbf{I}\rightarrow X$ tel que $c(0) =x$ et $c(1/n) =x_n$ pour $n\geqslant 1$. Si l’application $f$ est continue par arcs, l’application $f\circ c$ est continue et l’élément $f(x) =f(c(0))$ est limite de la suite $(f(c(1/n)))_{n\geqslant 1}$, c’est-à-dire de la suite $(f(x_n))_{n\geqslant 1}$, d’où le corollaire.

#### Lemme {#ta-iii-s2-n5-lem-1 .statement tag=01XL}

Soit X un espace topologique connexe et localement connexe par arcs et soit $x$ un point de X. Supposons que le point $x$ possède un système fondamental dénombrable de voisinages. Alors, pour toute suite $(x_n)_{n\geqslant 1}$ de points de X tendant vers $x$, il existe un chemin $c$ dans X tel que $c(0) =x$ et $c(1/n) =x_n$ pour $n\geqslant 1$.

Soit $(W_m)_{m\geqslant 1}$ un système fondamental de voisinages de $x$. Posons $V_0= X$ et pour tout $m\geqslant 1$, soit $V_m$ un voisinage connexe par arcs de $x$ contenu dans $V_{m-1}\cap W_m$.

Pour tout entier $n\geqslant 1$, notons $m_n$ le plus grand entier $m\leqslant n$ tel que $x_k\in V_m$ pour tout $k\geqslant n$. La suite $(m_n)_{n\geqslant 1}$ est croissante par définition ; elle tend vers l’infini, car la suite $(x_n)_{n\geqslant 1}$ tend vers $x$. Pour tout entier $n\geqslant 1$, soit $c_n:\mathbf{I}\rightarrow V_{m_n}$ un chemin d’origine $x_{n+1}$ et de terme $x_n$ dans $V_{m_n}$. Définissons une application $c:\mathbf{I}\rightarrow X$ en posant $c(0) =x$ et $c(t) =c_n(n(n+ 1)t-n)$ si $1/(n+ 1)< t\leqslant$ $1/n$. On a $c(1/n) =x_n$ pour tout $n\geqslant 1$. L’application $c$ est donc continue sur tout intervalle de la forme $[1/(n+ 1),1/n]$ avec $n\geqslant 1$, donc sur l’intervalle $]0,1]$. Si $t\leqslant 1/n$, le point $c(t)$ appartient à $V_{m_n}$; l’application $c$ est donc continue en 0.

#### Proposition 13 {#ta-iii-s2-prop-13 .statement tag=01XM}

Soit $p: E\rightarrow B$ une application étale et séparée et soit $s: B\rightarrow E$ une section de $p$. Si l’espace B est localement connexe par arcs et si la section $s$ est continue par arcs, elle est continue.

Soit $b$ un point de B; démontrons que $s$ est continue au point $b$. Comme $p$ est une application étale, il existe un voisinage V de $b$ et une section locale continue $s'$ de $p$ définie dans V telle que $s'(b) =s(b)$ (I, p. 33, prop. 9). Comme B est localement connexe par arcs, on peut supposer que V est connexe par arcs. Pour tout chemin $c$ dans V, d’origine $b$, les applications $s\circ c$ et $s'\circ c$ sont deux relèvements continus à B de l’application $c:\mathbf{I}\rightarrow X$ et l’on a $s\circ c(0) =s'\circ c(0) =s(b)$. D’après le corollaire 1 de I, p. 34, on a $s\circ c=s'\circ c$ et en particulier $s\circ c(1) =s'\circ c(1)$. Comme tout point de V est terme d’un chemin dans V d’origine $b$, les applications $s$ et $s'$ coïncident dans V. L’application $s$ est donc continue dans V.

#### Corollaire {#ta-iii-s2-n5-cor-1 .statement tag=01XN}

Soit B un espace topologique, soient $(E, p)$ et $(E', p')$ deux B-espaces. On suppose que l’application $p$ est étale et séparée et que l’espace $E'$ est localement connexe par arcs. Alors toute application continue par arcs $f: E'\rightarrow E$ telle que $p\circ f=p'$ est continue.

L’application pr$_1: E'\times_BE\rightarrow E'$ est étale et séparée (I, p. 31, prop. 8 et I, p. 27, prop. 4) et l’application $x\mapsto (x, f(x))$ en est une section continue par arcs. D’après la proposition 13, elle est continue, donc $f$ est continue.

### 6. Compléments sur les espaces topologiques compacts métrisables

Munissons l’ensemble à deux éléments $\{0,1\}$ de la topologie discrète et l’ensemble $\{0,1\}^{\mathbf{N}}$ de la topologie produit. L’espace topologique $\{0,1\}^{\mathbf{N}}$ est compact (TG, I, p. 63, th. 3), métrisable (TG, IX, p. 15, cor. 2), non vide, totalement discontinu (TG, I, p. 84, prop. 10) et n’a pas de point isolé.

#### Proposition 14 {#ta-iii-s2-prop-14 .statement tag=01XO}

Tout espace topologique compact, métrisable, non vide, totalement discontinu et sans point isolé est homéomorphe à $\{0,1\}^{\mathbf{N}}$.

Soit X un tel espace topologique. Munissons-le d’une distance compatible avec sa topologie. Comme l’espace X est compact, il est complet pour cette distance (TG, II, p. 27, th. 1).

#### Lemme 3 {#ta-iii-s2-lem-3 .statement tag=01XP}

Soit $\varepsilon$ un nombre réel $>0$. Il existe un entier $m\geqslant 1$ tel que, pour tout entier $n\geqslant m$, X admette une partition formée de $n$ ensembles ouverts et fermés non vides de diamètre $\leqslant \varepsilon$.

Tout point de X admet un voisinage ouvert et fermé de diamètre $\leqslant \varepsilon$ (TG, II, p. 32, corollaire de la prop. 6). Comme l’espace X est compact, il possède un recouvrement fini par de tels ensembles. Choisissons-en un, $(U_i)_{1\leqslant i\leqslant m}$, pour lequel $m$ est minimal. On a $m\geqslant 1$ puisque X n’est pas vide. Pour $1\leqslant i\leqslant m$, notons $V_i$ l’intersection de $U_i$ et des $X-U_k$ pour $k < i$. Alors $(V_i)_{1\leqslant i\leqslant m}$ est une partition de X, formée de $m$ ensembles ouverts et fermés non vides de diamètre $\leqslant \varepsilon$.

Puisque X n’a pas de point isolé, toute partie V ouverte et fermée, non vide, de X contient au moins deux points. Comme en outre X est compact et totalement discontinu, V est réunion de deux parties ouvertes et fermées non vides disjointes (loc. cit.). Il en résulte, par récurrence, que pour tout entier $n\geqslant m$, X admet une partition formée de $n$ ensembles ouverts et fermés non vides de diamètre $\leqslant \varepsilon$.

Terminons maintenant la démonstration de la prop. 14. Tout sous-espace ouvert et fermé non vide de X est un espace métrique compact, totalement discontinu et sans point isolé. Le lemme 3 permet donc de construire par récurrence une suite $(J_n)_{n\geqslant 0}$ d’ensembles finis et pour tout $n\geqslant 0$ une application $\varphi_n$ de l’ensemble $C_n= J_0\times  \cdots  \times J_n$ dans l’ensemble des parties ouvertes et fermées non vides de X de diamètre $\leqslant 2^{-n}$, de manière que :

(i) Pour tout $n\geqslant 0$, il existe un entier $m_n\geqslant 1$ tel que Card(J$_n) =$ $2^{m_n}$;

(ii) La famille $(\varphi_0(c))_{c\in C_0}$ soit une partition de X ;

(iii) Pour tout $n\geqslant 0$ et tout $c\in C_n$, la famille $(\varphi_{n+1}(c, j))_{j\in J_{n+1}}$ soit une partition de $\varphi_n(c)$.

Notons $p_n$ la projection canonique de $C_{n+1}$ sur $C_n$. La suite C = $(C_n, p_n)_{n\geqslant 0}$ est un crible (TG, IX, p. 63, déf. 8). L’espace topologique associé à ce crible (TG, IX, p. 63) s’identifie à l’espace topologique J, produit des espaces topologiques discrets $J_n$. Le crible C et la suite d’applications $(\varphi_n)_{n\geqslant 0}$ définissent un criblage strict de l’espace métrique X (TG, IX, p. 63 et p. 64). L’application $f: J\rightarrow X$ déduite de ce criblage est continue et bijective (TG, IX, p. 65). Comme l’espace topologique J est compact (TG, I, p. 63, th. 3) et que X est séparé, $f$ est un homéomorphisme (TG, I, p. 63, cor. 2). Comme $J_n$ est homéomorphe à $\{0,1\}^{m_n}$ pour tout $n\geqslant 0$, J est homéomorphe à $\{0,1\}^{\mathbf{N}}$ (TG, I, p. 25, prop. 2).

#### Exemple {#ta-iii-s2-n6-exa-1 .statement tag=01XQ}

Soit K l’ensemble triadique de Cantor (TG, IV, p. 9, exemple). Pour tout $n\geqslant 0$, posons $J_n=\{0,1\}$ et définissons une application $K_n$ de l’ensemble $C_n= J_0\times  \cdots  \times J_n$ dans l’ensemble des intervalles fermés de $[0,1]$ de la manière suivante : on pose $K_0(0) = [0,\frac{1}{3}]$ et $K_0(1) = [\frac{2}{3},1]$; pour tout $n\geqslant 0$ et tout $c\in C_n,K_{n+1}(c,0)$ et $K_{n+1}(c,1)$ sont respectivement le « tiers gauche » et le « tiers droit » de $K_n(c)$. Si $c= (j_0, j_1, . . . , j_n)\in C_n,K_n(c)$ est l’intervalle noté $K_{n,p}$ dans loc. cit., avec $p= 2^nj_0+2^{n-1}j_1+\cdots +j_n+1$, c’est aussi l’intervalle $[a, a+\frac{1}{3^{n+1}}]$, où $a= 2(\frac{j_0}{3}+\frac{j_1}{3^2}+\cdots +\frac{j_n}{3^{n+1}})$. Pour $n\geqslant 0$ et $c\in C_n$, posons $\varphi_n(c) = K_n(c)\cap K$. La famille $(\varphi_n(c))_{c\in C_n}$ est une partition de K formée d’ensembles fermés. Ces ensembles sont donc aussi ouverts dans K; ils sont non vides et de diamètre $\frac{1}{3^{n+1}}$, car les extrémités des intervalles $K_n(c)$ appartiennent à K. La suite $C = (C_n, p_n)_{n\geqslant 0}$, où $p_n: C_{n+1}\rightarrow C_n$ est la projection canonique $(c, j)\mapsto c$, est un crible, et l’espace topologique associé à ce crible s’identifie à $\{0,1\}^{\mathbf{N}}$. Le crible C et la suite d’applications $(\varphi_n)_{n\geqslant 0}$ définissent un criblage strict de l’espace métrique K. L’application $f:\{0,1\}^{\mathbf{N}}\rightarrow K$ déduite de ce criblage est un homéomorphisme, donné par la formule

$$
f((j_n)_{n\geqslant 0}) = 2\sum^{\infty}j^n
$$

$$
n=03n+1
$$

#### Corollaire {#ta-iii-s2-n6-cor-1 .statement tag=01XR}

Soit X un espace topologique métrisable, compact et non vide. Il existe une application continue et surjective de $\{0,1\}^{\mathbf{N}}$ dans X.

Tout espace topologique compact et métrisable est homéomorphe à un sous-espace, nécessairement fermé, de l’espace topologique $\mathbf{I}^{\mathbf{N}}$ (TG, IX, p. 18, prop. 12 et p. 21, prop. 16). Soient donc A un sous-espace fermé de $\mathbf{I}^{\mathbf{N}}$ et $h$ un homéomorphisme de A sur X.

Posons K = $\{0,1\}^{\mathbf{N}}$ et, pour $\alpha = (a_n)\in$ K, posons $f(\alpha ) =$ $\sum^{\infty}_{n=0}a_n2^{-n-1}$; on a $f(\alpha )\in \mathbf{I}$. L’application $f: K\rightarrow \mathbf{I}$ ainsi définie est surjective (TG, IV, p. 42) et continue. En effet, si deux éléments $\alpha$ et $\beta$ de K ont les mêmes coordonnées d’indice $< n$, on a $|f(\beta )-f(\alpha )|\leqslant 2^{-n}$. Notons $g$ l’application $(\alpha_n)\mapsto (f(\alpha_n))$ de $K^{\mathbf{N}}$ dans $\mathbf{I}^{\mathbf{N}}$; elle est continue et surjective. L’espace topologique $K^{\mathbf{N}}$ est compact (TG, I, p. 63, th. 3), métrisable (TG, IX, p. 15, cor. 2) et totalement discontinu (TG, I, p. 84, prop. 10) et il en est de même de son sous-espace fermé $\overset{-1}{g}(A)$ ; ce dernier est non vide puisque les applications $g$ et $h$ sont surjectives.

Alors, l’espace $\overset{-1}{g}(A)\times K$ est homéomorphe à $\{0,1\}^{\mathbf{N}}$ (prop. 14), puisque c’est un espace topologique compact, métrisable, totalement discontinu et sans point isolé et l’application $(x, y)\mapsto h(g(x))$ de $\overset{-1}{g}(A)\times K$ dans X est continue surjective.

### 7. Propriétés topologiques de l’image d’un chemin

#### Proposition 15 {#ta-iii-s2-prop-15 .statement tag=01XS}

L’image d’un chemin dans un espace topologique séparé est un espace topologique compact, métrisable, connexe et localement connexe par arcs.

Soient X un espace topologique séparé et $c:\mathbf{I}\rightarrow X$ une application continue. Notons R la relation d’équivalence $c(s) =c(t)$ dans $\mathbf{I}$. L’espace topologique $c(\mathbf{I})$ est séparé (TG, I, p. 63, cor. 1), l’espace $\mathbf{I}/R$ est quasi-compact (TG, I, p. 62, th. 2), donc la bijection $\mathbf{I}/R\rightarrow c(\mathbf{I})$ déduite de $c$ est un homéomorphisme (TG, I, p. 63, cor. 2). Par suite, l’espace $c(\mathbf{I})$ est compact, métrisable (TG, IX, p. 22, prop. 17), connexe (TG, I, p. 82, prop. 6) et localement connexe par arcs (III, p. 261, prop. 8).

#### Théorème 1 (Hahn et Mazurkiewicz) {#ta-iii-s2-thm-1 .statement tag=01XT}

Tout espace topologique métrisable, compact, non vide, connexe et localement connexe, est homéo-morphe à un espace quotient du segment $[0,1]$.

#### Lemme 4 {#ta-iii-s2-lem-4 .statement tag=01XU}

Soit K un espace topologique compact et soit $\mathscr{R}$ un ensemble d’ouverts de K recouvrant K. Il existe un entourage V de la structure uniforme de K (TG, II, p. 27, th. 1) tel que, pour tout $x\in K$, $V(x)$ soit contenu dans l’un des ensembles appartenant à $\mathscr{R}$.

Pour tout point $x$ de K, il existe un entourage $W_x$ de la structure uniforme de K tel que $W_x(x)$ soit contenu dans un des ensembles appartenant à $\mathscr{R}$. Soit $V_x$ un entourage de la structure uniforme de K tel que $\overset{2}{V_{x}}$ soit contenu dans $W_x$. Les intérieurs des $V_x(x)$ recouvrent K ; comme l’espace K est compact, il existe une partie finie F de K telle que la famille $(V_y(y))_{y\in F}$ soit un recouvrement de K (TG, I, p. 59). Notons V l’intersection de la famille $(V_y)_{y\in F}$; l’ensemble V est un entourage de la structure uniforme de K. Pour tout point $x\in K$, il existe un point $y\in F$ tel que $x$ appartienne à $V_y(y)$. Par suite, l’ensemble

$V(x)$ est contenu dans $\overset{2}{V_{y}}(y)$, donc dans un des ensembles appartenant à $\mathscr{R}$.

#### Lemme 5 {#ta-iii-s2-lem-5 .statement tag=01XV}

Soient X et Y des espaces uniformes et $f$ une application de X dans Y. Soit $\mathscr{F}$ un ensemble de parties fermées de X recouvrant X et possédant les propriétés suivantes :

(i) Il existe un ensemble $F_0\in \mathscr{F}$ qui rencontre tous les ensembles $F\in \mathscr{F}$;

(ii) Pour tout entourage U de la structure uniforme de X, il n’y a qu’un nombre fini d’ensembles $F\in \mathscr{F}$ qui ne sont pas petits d’ordre U ;

(iii) Pour tout entourage V de la structure uniforme de Y, il n’y a qu’un nombre fini d’ensembles $F\in \mathscr{F}$ tels que $f(F)$ ne soit pas petit d’ordre V.

Alors, si la restriction de $f$ à chacun des ensembles $F\in \mathscr{F}$ est continue, $f$ est continue.

Soit $x$ un point de X. Démontrons que $f$ est continue en $x$. Il existe un ensemble $F_1\in \mathscr{F}$ tel que $x\in F_1$. La restriction de $f$ à $F_0\cup F_1$ est continue (TG, I, p. 19, prop. 4). En remplaçant $F_0$ par $F_0\cup F_1$, on se ramène au cas où $x\in F_0$.

Soit V un entourage de la structure uniforme de Y. Choisissons

un entourage $V'$ de cette même structure uniforme tel que $\overset{2}{V'}\subset V$. Comme la restriction de $f$ à $F_0$ est continue, il existe un entourage U de la structure uniforme de X tel que $f(z)\in V'(f(x))$ pour tout $z\in F_0\cap U(x)$. Soit $U'$ un entourage de la structure uniforme de X

tel que $\overset{2}{U'}\subset U$. Notons A la réunion de $F_0$, des ensembles $F\in \mathscr{F}$ qui ne sont pas petits d’ordre $U'$ et de ceux tels que $f(F)$ ne soit pas petit d’ordre $V'$. Par hypothèse, A est la réunion d’un nombre fini d’ensembles appartenant à $\mathscr{F}$, et la restriction de $f$ à A est continue (loc. cit.). Il existe donc un voisinage W de $x$ dans X, contenu dans $U'(x)$, tel que $f(y)\in V(f(x))$ pour $y\in A\cap W$. Pour conclure, il nous suffira de prouver que l’on a aussi $f(y)\in V(f(x))$ pour tout point $y\in (X-A)\cap W$. Soit $y$ un tel point. Soit F un élément de $\mathscr{F}$ tel que $y\in F$. Par définition de A, F est petit d’ordre $U'$ et $f(F)$ est petit d’ordre $V'$. Par hypothèse, F rencontre $F_0$. Soit $z\in F\cap F_0$. On a $z\in U'(y)$ puisque F est petit d’ordre $U'$ et $y\in U'(x)$ puisque W

est contenu dans $U'(x)$, d’où $z\in \overset{2}{U'}(x)$ et a fortiori $z\in U(x)$. Mais alors, comme $z$ appartient à $F_0$, on a $f(z)\in V'(f(x))$. Par ailleurs $f(F)$ est petit d’ordre $V'$, d’où $f(y)\in V'(f(z))$. Il en résulte que l’on a

$f(y)\in \overset{2}{V'}(f(x))$ et finalement $f(y)\in V(f(x))$. Cela conclut la preuve du lemme 5.

Démontrons maintenant le théorème 1. Soit X un espace métrique compact non vide, connexe et localement connexe. Un tel espace est connexe par arcs et localement connexe par arcs (III, p. 267, corollaire 2). D’après le corollaire et l’exemple de III, p. 270, il existe une application continue et surjective $f$ de l’ensemble triadique de Cantor K (TG, IV, p. 9, exemple) dans X. Nous allons construire un prolongement continu $g$ de $f$ à $[0,1]$, ce qui démontrera le théorème 1.

Soit $\varepsilon$ un nombre réel $>0$. Les parties ouvertes et connexes par arcs de X de diamètre $\leqslant \varepsilon$ recouvrent X. Notons $\mathscr{R}$ l’ensemble de leurs images réciproques par $f$ : c’est un ensemble d’ouverts de K recouvrant K. D’après le lemme 4 de III, p. 272, il existe un nombre réel $\alpha  >0$ tel que toute boule fermée de K de rayon $\alpha$ soit contenue dans un élément de $\mathscr{R}$. En particulier, si $t$ et $t'$ sont des points de K tels que $|t-t'|\leqslant \alpha$, il existe un chemin dans X reliant $f(t)$ à $f(t')$ dont l’image est de diamètre $\leqslant \varepsilon$.

L’alinéa précédent permet de construire par récurrence une suite strictement croissante $(n_k)_{k\geqslant 0}$ d’entiers $\geqslant$ 0 possédant la propriété suivante : pour tout entier $k\geqslant 0$ et tout couple $(t, t')$ de points de K tels que $|t-t'|\leqslant 3^{-n_k}$, il existe un chemin dans X reliant $f(t)$ à $f(t')$ dont l’image est de diamètre $\leqslant 2^{-k}$. Le complémentaire de K dans $[0,1]$ est la réunion d’une famille $(I_{n,p})$ d’intervalles ouverts deux à deux disjoints, où $n$ parcourt l’ensemble des entiers $\geqslant 0$ et $p$ l’ensemble des entiers compris entre 1 et $2^n$ (TG, IV, p. 9, exemple). Considérons un de ces intervalles $I_{n,p}$ et écrivons-le $]a, b[$. Les points $a$ et $b$ appartiennent à K et l’on a $b-a= 3^{-n-1}$. On définit la fonction $g$ sur l’intervalle $I_{n,p}$ de la façon suivante : on choisit un chemin $c$ dans X reliant $f(a)$ à $f(b)$, dont l’image soit de diamètre $\leqslant 2^{-k}$ si $n_k\leqslant n < n_{k+1}$, et l’on pose $g(t) =c(\frac{t-a}{b-a})$ pour $t\in I_{n,p}$. La fonction $g: [0,1]\rightarrow X$ ainsi définie prolonge $f$. Elle est continue sur K ainsi que sur chacun des intervalles fermés $\overline{I_{n,p}}$. Ces derniers rencontrent K. De plus, pour tout nombre réel $\varepsilon  >0$, il n’y a qu’un nombre fini d’intervalles $\overline{I_{n,p}}$ de longueur $> \varepsilon$, et il n’y a qu’un nombre fini d’intervalles $\overline{I_{n,p}}$ dont les images par $g$ soient de diamètre $> \varepsilon$. D’après le lemme 5, l’application $g$ est continue.

### 8. Caractérisations de l’intervalle

#### Lemme 6 {#ta-iii-s2-lem-6 .statement tag=01XW}

Soit D un ensemble totalement ordonné dénombrable, non réduit à un élément, possédant un plus petit et un plus grand élément. On suppose que D est sans trou (E, III, p. 73, exerc. 19), c’està-dire que tout intervalle ouvert $]x, y[$, où $x$ et $y$ sont des éléments de D tels que $x < y$, est non vide. Il existe alors un isomorphisme d’ensembles ordonnés de $\mathbf{I}\cap \mathbf{Q}$ sur D.

Soient $a$ le plus petit élément et $b$ le plus grand élément de D. Par hypothèse, on a $b=\not a$ et $]a, x[=\not\emptyset$ pour tout $x\in D-\{a\}$. L’ensemble D$-\{a\}$ est totalement ordonné, n’est pas vide et n’a pas de plus petit élément ; il est donc infini (E, III, p. 34, cor. 1 de la prop. 3). Les ensembles $\mathbf{I}\cap \mathbf{Q}$ et D, infinis et dénombrables, sont équipotents à $\mathbf{N}$.

Choisissons des bijections $n\mapsto a_n$ et $n\mapsto b_n$ de $\mathbf{N}$ sur $\mathbf{I}\cap \mathbf{Q}$ et D respectivement, telles que $a_0= 0,a_1= 1,b_0=a,b_1=b$. Il existe une unique application strictement croissante $f:\mathbf{I}\cap \mathbf{Q}\rightarrow D$ possédant les propriétés suivantes : on a $f(0) =a$ et $f(1) =b$; pour $n\geqslant 2$, on a $f(a_n) =b_m$, où $m$ est le plus petit entier naturel pour lequel l’application de $\{a_0, . . . , a_n\}$ dans D qui coïncide avec $f$ dans $\{a_0, . . . , a_{n-1}\}$ et applique $a_n$ sur $b_m$ est strictement croissante. Ces propriétés définissent en effet $f(a_n)$ par récurrence sur $n$, l’existence de l’entier $m$ étant assurée par le fait que D est sans trou.

Comme l’application $f$ est strictement croissante et que $\mathbf{I}\cap \mathbf{Q}$ est totalement ordonné, $f$ définit un isomorphisme d’ensembles ordonnés de $\mathbf{I}\cap \mathbf{Q}$ sur son image (E, III, p. 14, prop. 11). Il nous reste à démontrer que $f$ est surjective. Pour cela, démontrons par récurrence que $b_m$ appartient à l’image de $f$ pour tout $m\in \mathbf{N}$.

On a $b_0=f(0)$ et $b_1=f(1)$. Supposons que l’on ait $m\geqslant 2$ et que, pour $0\leqslant k\leqslant m-1$, il existe $c_k\in \mathbf{I}\cap \mathbf{Q}$ tel que $f(c_k) =b_k$. On a $c_0= 0$ et $c_1= 1$, car $f$ est injective. Considérons le plus petit entier $n\in \mathbf{N}$ pour lequel $a_n$ n’appartient pas à $\{c_0, . . . , c_{m-1}\}$ et l’application $g$ de $\{c_0, . . . , c_{m-1}, a_n\}$ dans D qui coïncide avec $f$ dans $\{c_0, . . . , c_{m-1}\}$ et applique $a_n$ sur $b_m$ est strictement croissante ; un tel entier existe car $\mathbf{I}\cap \mathbf{Q}$ est sans trou. Soit $f'$ l’application de $\{a_0, . . . , a_n\}$ dans D qui coïncide avec $f$ dans $\{a_0, . . . , a_{n-1}\}$ et qui applique $a_n$ sur $b_m$. Démontrons qu’elle est strictement croissante. Soit $j\in  \{0, . . . , n-1\}$; par définition de l’entier $n$, il existe $k\in  \{0, . . . , m-1\}$ tel que $a_j=c_k$, ou $a_j< c_k$ et $b_m\geqslant f(c_k)$, ou $a_j> c_k$ et $b_m\leqslant f(c_k)$. Supposons $b_k< b_m$; on a alors $g(c_k) =f(c_k) =b_k< b_m=g(a_n)$, d’où $c_k< a_n$ car $g$ est strictement croissante, puis $a_j\leqslant c_k< a_n$; en outre, $f'(a_j) =$ $f(a_j)\leqslant f(c_k) =b_k< b_m=f'(a_n)$. De même, si $b_k> b_m$, il vient $a_n< c_k\leqslant a_j$ et $f'(a_j) =f(a_j)\geqslant f(c_k) =b_k> b_m=f'(a_n)$. Comme $f$ est elle-même strictement croissante, il en résulte que l’application $f'$ est strictement croissante.

Si $m'$ est l’entier tel que $f(a_n) =b_{m'}$, on a $m'\leqslant m$, par définition de $f$. Si l’on avait $m'< m$, on aurait $f(a_n) =b_{m'}=f(c_{m'})$, d’où $a_n=c_{m'}$, car $f$ est injective, ce qui contredit la définition de $a_n$. Ainsi, $m'=m$ et $f(a_n) =b_m$, ce qui démontre que $b_m$ appartient à l’image de $f$ et termine par récurrence la démonstration de la surjectivité de $f$.

#### Proposition 16 {#ta-iii-s2-prop-16 .statement tag=01XX}

Soit E un ensemble totalement ordonné non réduit à un élément. On suppose que toute partie de E a une borne supérieure et qu’il existe une partie dénombrable de E qui rencontre tout intervalle ouvert $]x, y[$, où $x$ et $y$ sont des éléments de E tels que $x < y$. Il existe alors un isomorphisme d’ensembles ordonnés de $\mathbf{I}$ sur E.

Comme $\emptyset$ et E ont chacun une borne supérieure dans E, E a un plus petit élément $a$ et un plus grand élément $b$. Ceux-ci sont distincts puisque E n’est pas réduit à un élément. Soit $D'$ une partie dénombrable de E qui rencontre tout intervalle ouvert de E de la forme $]x, y[$, avec $x < y$. Posons $D = D'\cup  \{a, b\}$. L’ensemble D est totalement ordonné et sans trou. D’après le lemme 6, il existe un isomorphisme d’ensembles ordonnés $f$ de $\mathbf{I}\cap \mathbf{Q}$ sur D.

Pour tout $t\in \mathbf{I}$, soit $g(t)$ la borne supérieure de $f([0, t]\cap \mathbf{Q})$ dans E. Pour tout $x\in E$, soit $h(x)$ la borne supérieure de $f^{-1}([a, x]\cap D)$ dans $\mathbf{I}$. Les applications $g:\mathbf{I}\rightarrow E$ et $h: E\rightarrow \mathbf{I}$ ainsi définies sont croissantes, $g$ coïncide avec $f$ dans $\mathbf{I}\cap \mathbf{Q}$ et $h$ coïncide avec $f^{-1}$ dans D.

On a donc $g(h(y)) =y$ pour tout $y\in D$. Soit $x\in E$. Si l’on avait $g(h(x))> x$, l’intervalle $]x, g(h(x))[$ contiendrait un point $y$ de D et les relations $g(h(y)) =y < g(h(x))$ contrediraient le fait que $g\circ h$ est croissante. De même, on n’a pas $g(h(x))< x$. On a donc $g(h(x)) =x$, ce qui démontre que $g\circ h$ est l’application identique de E. On démontre de même que $h\circ g$ est l’application identique de $\mathbf{I}$. Ainsi, $g:\mathbf{I}\rightarrow E$ et $h: E\rightarrow \mathbf{I}$ sont des isomorphismes d’ensembles ordonnés réciproques l’un de l’autre.

#### Remarque {#ta-iii-s2-n8-rem-1 .statement tag=01XY}

Soit E un ensemble totalement ordonné. L’ensemble des intervalles ouverts de E (limités ou non) est stable par intersection finie. C’est une base d’une topologie $\mathscr{T}_0(E)$ sur E (TG, I, p. 91, exerc. 5). La topologie $\mathscr{T}_0(\mathbf{I})$ est identique à la topologie induite sur $\mathbf{I}$ par celle de $\mathbf{R}$. Il s’ensuit que, dans la prop. 16, tout isomorphisme d’ensembles ordonnés de $\mathbf{I}$ sur E est un homéomorphisme de $\mathbf{I}$ sur l’espace topologique obtenu en munissant E de la topologie $\mathscr{T}_0(E)$.

#### Corollaire {#ta-iii-s2-n8-cor-1 .statement tag=01XZ}

Soit R une relation d’équivalence dans $\mathbf{I}$. Les conditions suivantes sont équivalentes :

(i) Toute classe d’équivalence suivant R est un intervalle fermé de $\mathbf{I}$, distinct de $\mathbf{I}$;

(ii) Il existe une application croissante et surjective $u:\mathbf{I}\rightarrow \mathbf{I}$ telle que R soit la relation d’équivalence associée à $u$.

Une telle application $u$, lorsqu’elle existe, est continue et définit par passage au quotient un homéomorphisme de $\mathbf{I}/R$ sur $\mathbf{I}$.

Nous noterons $p:\mathbf{I}\rightarrow \mathbf{I}/R$ la surjection canonique.

Supposons la condition (i) satisfaite. Pour A et B des classes d’équivalence suivant R, écrivons $A<B$ si l’on a $a < b$ pour tout $a\in A$ et tout $b\in B$. Dans $\mathbf{I}/R$, la relation « A = B ou $A<B$ » est une relation d’ordre. En effet, elle est réflexive ; elle est antisymétrique car on ne peut avoir simultanément $A<B$ et $B<A$ ; elle est transitive car les relations $A<B$ et $B<C$ entraînent $A<C$. Si A et B sont des éléments distincts de $\mathbf{I}/R$, ce sont des intervalles fermés de $\mathbf{I}$, disjoints, et l’on a alors soit $A<B$, soit $B<A$. Muni de la relation d’ordre ainsi définie, $\mathbf{I}/R$ est donc totalement ordonné. L’application $p:\mathbf{I}\rightarrow \mathbf{I}/R$ est croissante.

L’ensemble $\mathbf{I}/R$ n’est pas réduit à un élément, en vertu de (i).

Soit F une partie de $\mathbf{I}/R$. Démontrons que F possède une borne supérieure dans $\mathbf{I}/R$. Posons $F'=\overset{-1}{p}(F)$ ; notons $a$ la borne supérieure de $F'$ dans $\mathbf{I}$ et A la classe d’équivalence de $a$ suivant R. Comme $a$ majore $F'$ dans $\mathbf{I}$, A majore F dans $\mathbf{I}/R$. Inversement, soit $B\in \mathbf{I}/R$ un majorant de F ; posons $b=$ sup(B). Tout élément de $F'$ est alors majoré par $b$. On a donc $a\leqslant b$. Comme les classes d’équivalence suivant R sont des intervalles fermés, $a$ appartient à A et $b$ à B. On a par suite $A =p(a)\leqslant p(b) = B$. Cela démontre que A est la borne supérieure de F.

Soient A et B des éléments de $\mathbf{I}/R$ tels que $A<B$. Soit $a$ la borne supérieure de A et $b$ la borne inférieure de B. Comme $a\in A$ et $b\in B$, on a $a < b$. La classe d’équivalence suivant R d’un élément quelconque de $]a, b[$ est un élément de l’intervalle $]A,B[$ de $\mathbf{I}/R$. Comme $\mathbf{I}\cap \mathbf{Q}$ rencontre $]a, b[$, son image par $p$ rencontre $]A,B[$.

Nous avons ainsi démontré que l’ensemble totalement ordonné $\mathbf{I}/R$ satisfait aux hypothèses de la prop. 16. Il existe donc un isomorphisme d’ensembles ordonnés $f:\mathbf{I}/R\rightarrow \mathbf{I}$. L’application $u=f\circ p$ est une application surjective et croissante de $\mathbf{I}$ sur $\mathbf{I}$ et la relation d’équivalence associée à $u$ est la relation R ; cela démontre que la condition (ii) est satisfaite.

Supposons inversement que la condition (ii) soit satisfaite. Soit $u:\mathbf{I}\rightarrow \mathbf{I}$ une application croissante et surjective telle que R soit la relation d’équivalence associée à $u$.

Soit $a$ un point de $\mathbf{I}$. L’ensemble $A =\overset{-1}{u}(a)$ est un intervalle de $\mathbf{I}$, car l’application $u$ est croissante. Comme $u$ est surjective, A n’est ni vide, ni égal à $\mathbf{I}$. Soit $b$ la borne supérieure de A dans $\mathbf{I}$. On a $u(b)\geqslant a$. Si $u(b)> a$, il existe $c\in ]a, u(b)[$ et $d\in \mathbf{I}$ tel que $u(d) =c$ puisque $u$ est surjective. Comme $u$ est croissante et que $a < u(d)< u(b),d$ majore tout élément de A et on a $d < b$, ce qui contredit l’hypothèse que $b$ est la borne supérieure de A. On a donc $u(b) =a$, c’est-à-dire $b\in A$. On démontre de même que A contient sa borne inférieure. L’ensemble A est donc un intervalle fermé de $\mathbf{I}$, distinct de $\mathbf{I}$. Cela démontre que la condition (i) est satisfaite.

Démontrons maintenant que l’application $u$ est continue. Il suffit pour cela de démontrer que, pour tout $a\in \mathbf{I}$, les ensembles $\overset{-1}{u}(]a,\rightarrow [)$ et $\overset{-1}{u}(]\leftarrow , a[)$ sont ouverts. Soit $b$ la borne supérieure de $\overset{-1}{u}(a)$ ; on a $u(b) =a$. Si $x\in \mathbf{I}$ vérifie $u(x)> a$, on a nécessairement $x > b$; inversement, si $x > b$, on a $u(x)\geqslant a$ et $u(x)=\not a$ puisque $b$ est la borne supérieure de $\overset{-1}{u}(a)$. On a par conséquent $\overset{-1}{u}(]a,\rightarrow [) = ]b,\rightarrow [$, ce qui démontre que l’image réciproque par $u$ de l’intervalle $]a,\rightarrow [$ est ouverte. On démontre de même que celle de $]\leftarrow , a[$ est ouverte. Il s’ensuit que l’application $u$ est continue.

L’application $v:\mathbf{I}/R\rightarrow \mathbf{I}$ déduite de $u$ par passage au quotient est alors continue et bijective. Comme $\mathbf{I}$ est compact, $\mathbf{I}/R$ est quasi-compact (TG, I, p. 62, th. 2) et $v$ est un homéomorphisme (TG, I, p. 63, cor. 2).

#### Proposition 17 {#ta-iii-s2-prop-17 .statement tag=01Y0}

Soit X un espace topologique connexe et compact. Soit $a$ un point de X, soit U une partie ouverte et fermée non vide de X $-\{a\}$.

a) L’adhérence $\overline{U}$ de U dans X est égale à $U\cup  \{a\}$ et est connexe.

b) Soit $a'$ un point de X distinct de $a$, soit $U'$ une partie ouverte et fermée non vide de X $-\{a'\}$. Si $a\notin U'$ et que $\overline{U}\cap \overline{U'}=\not\emptyset$, on a $\overline{U'}\subset U$. Inversement, si $a\in U'$ et que X $= U\not\cup U'$, on a $\overline{U}\subset U'$.

c) Il existe un point $b$ de U tel que X $-\{b\}$ soit connexe.

Démontrons l’assertion a). Notons V le complémentaire de U dans X $-\{a\}$. Comme U est fermé dans X $-\{a\}$, V est ouvert dans X$-\{a\}$ et a fortiori dans X. On a donc $U\subset \overline{U}\subset X-V = U\cup \{a\}$. De même, U est une partie ouverte de X. Comme X est connexe, U n’est pas fermé dans X, d’où l’égalité $U = U\cup  \{a\}$. On a de même $V = V\cup  \{a\}$.

Soient F et G des parties fermées disjointes de $\overline{U}$ telles que $U = F\cup G$. Supposons que $a\in G$ et démontrons que F est vide ; on raisonnerait de même si $a\in F$. L’ensemble $G\cup V = G\cup \overline{V}$ est une partie fermée de X, disjointe de F, et l’on a $X = U\cup V = F\cup (G\cup V)$. Comme X est connexe et que G n’est pas vide, F est vide. Cela démontre que $\overline{U}$ est connexe.

Démontrons b). Supposons que $a\notin U'$ et que $\overline{U}\cap \overline{U'}=\not\emptyset$. D’après l’assertion a), on a $U = U\cup  \{a\}$ et $\overline{U'}= U'\cup  \{a'\}$. Comme $a\notin U'$ et $a=\not a'$, les parties U et $\overline{U'}$ ont un point commun. Toujours d’après a), $\overline{U'}$ est une partie connexe de X ; comme elle est contenue dans X$-\{a\}$ et qu’elle en rencontre la partie ouverte et fermée U, on a $\overline{U'}\subset U$, ce qu’il fallait démontrer. La seconde assertion découle de la première en considérant les complémentaires dans X de $\overline{U}$ et $\overline{U'}$ respectivement.

Démontrons enfin l’assertion c). Supposons par l’absurde que, pour tout $x\in U$, l’ensemble X $-\{x\}$ ne soit pas connexe et choisissons des parties $U_x$ et $V_x$, ouvertes et fermées dans X $-\{x\}$, disjointes et non vides, telles que X $-\{x\}= U_x\cup V_x$ et $a\in V_x$. D’après l’assertion b), appliquée aux parties ouvertes et fermées U, $U_x$ de X$-\{a\}$ et X$-\{x\}$ respectivement, on a $\overline{U_x}\subset U$ pour tout $x\in U$. Soient $x$ et $y$ des points de U tels que $x\in U_y$; on a donc $x=\not y$. Toujours d’après l’assertion b), appliquée aux parties ouvertes et fermées $U_x$ et $U_y$ de X $-\{x\}$ et X $-\{y\}$, la relation $x\in U_y$ entraîne la relation $\overline{U_x}\subset \overline{U_y}$. Par suite, les relations $x\in U_y$ et $\overline{U_x}\subset \overline{U_y}$ sont équivalentes.

L’ensemble des parties S de U telles que $\bigcap_{x\in S}\overline{U_x}=\not\emptyset$ est de caractère fini (E, III, p. 34), car l’espace X est compact. D’après E, III, p. 35, th. 1, il existe une partie maximale S de U telle que $C =\bigcap_{x\in S}\overline{U_x}$ ne soit pas vide. Soit $c$ un point de C. Pour tout élément $x$ de S, on a $c\in \overline{U_x}$, d’où $c\in U$ puis $\overline{U_c}\subset \overline{U_x}$. Par conséquent, on a $\overline{U_c}\subset C$ puis, par maximalité de S, $C = U_c$. Pour tout $x\in C$ tel que $x=\not c$, on a aussi $\overline{U_x}\subset \overline{U_c}$ et $\overline{U_x}= U\not_c$. Par maximalité de S, $C =\{c\}$, donc $\overline{U_c}=\{c\}$, ce qui contredit l’hypothèse que $U_c$ est une partie ouverte et fermée non vide de X $-\{c\}$.

#### Corollaire {#ta-iii-s2-n8-cor-2 .statement tag=01Y1}

Soit X un espace topologique compact connexe, soit N l’ensemble des points de X dont le complémentaire est connexe. L’ensemble X est l’unique partie connexe et compacte de X qui contient N.

Soit S une partie connexe et compacte de X telle que $N\subset S$. Supposons que S $= X\not$ et soit $x\in X-S$. Par hypothèse, X $-\{x\}$ n’est pas connexe ; il existe donc des parties U et V ouvertes et fermées de X $-\{x\}$, disjointes et non vides, telles que X $-\{x\}= U\cup V$. On peut supposer que $S\subset V$. On a $U = U\cup \{x\}$ et $V = V\cup  \{x\}$ et ces espaces sont connexes (III, p. 278, prop. 17, a)). D’après l’assertion c) de cette proposition, il existe $y\in U$ tel que X $-\{y\}$ soit connexe, ce qui contredit les inclusions $N\subset S\subset V$.

#### Lemme 7 {#ta-iii-s2-lem-7 .statement tag=01Y2}

Soit T un espace topologique localement connexe. Soit $\mathscr{U}$ un ensemble filtrant croissant de parties ouvertes de T, de réunion T. Pour $t\in T$ et $U\in \mathscr{U}$, notons $U_t$ la composante connexe de $t$ dans U si $t\in U$ et posons $U_t=\emptyset$ si $t\notin U$. Pour tout $t\in T,\bigcup_{U\in\mathscr{U}}U_t$ est la composante connexe de $t$ dans T.

Pour $t\in T$, posons $C_t=\bigcup_{U\in\mathscr{U}}U_t$. On a $t\in C_t$. Les ensembles $U_t$ sont ouverts et connexes et il en est de même de $C_t$ car on a $t\in U_t$ si $U_t=\not\emptyset$ (TG, I, p. 81, prop. 2). Soient $u,v$ des points de T tels que $C_u\cap C_v=\not\emptyset$. Soit $t$ un point de $C_u\cap C_v$; soit $U\in \mathscr{U}$ tel que $t\in U_u$ et soit $V\in \mathscr{U}$ tel que $v\in V_v$. Comme $\mathscr{U}$ est filtrant croissant, il existe $W\in \mathscr{U}$ qui contient $U\cup V$. Alors, $W_u\cap W_v=\not\emptyset$, donc $W_u= W_v$. Plus généralement, on a $W'_u= W'_v$ pour tout $W'\in \mathscr{U}$ tel que $W\subset W'$, donc $C_u= C_v$. Cela démontre que les ensembles de la forme $C_t$ forment une partition de T en sous-ensembles ouverts connexes. Par suite, pour tout $t\in T$, $C_t$ est la composante connexe de $t$ dans T.

#### Théorème 2 {#ta-iii-s2-thm-2 .statement tag=01Y3}

Soit X un espace topologique connexe compact possédant une partie dénombrable partout dense. Soient $a,b$ des points distincts de X. Les conditions suivantes sont équivalentes :

(i) Il existe un homéomorphisme $f:\mathbf{I}\rightarrow X$ tel que $f(0) =a$ et $f(1) =b$;

(ii) Tout sous-ensemble connexe de X qui contient $\{a, b\}$ est égal à X ;

(iii) L’espace X est localement connexe et tout sous-ensemble connexe et compact de X qui contient $\{a, b\}$ est égal à X ;

(iv) Pour tout $x\in X-\{a, b\}$, l’espace X $-\{x\}$ n’est pas connexe.

L’assertion (i) entraîne toutes les autres.

Soit $x$ un point de X $-\{a, b\}$. Comme X $-\{x\}$ contient $\{a, b\}$, l’assertion (ii) entraîne que ce n’est pas une partie connexe de X, si bien que (ii) implique (iv).

Montrons que (iii) entraîne (iv). Supposons satisfaites les hypothèses de (iii). Soit $x\in X-\{a, b\}$ et supposons que X$-\{x\}$ soit connexe. Soit T l’espace X $-\{x\}$ et soit $\mathscr{U}$ l’ensemble des parties de T de la forme X-V, où V est un voisinage compact de $x$. D’après le lemme 7, il existe un voisinage compact V de $x$ tel que $a$ et $b$ appartiennent à une même composante connexe de X-V. Ils appartiennent en particulier à une même composante connexe de $X-\mathring{V}$; celle-ci est un ensemble compact, connexe de X, distinct de X, ce qui contredit l’hypothèse (iii).

Il reste à démontrer que l’assertion (iv) implique la condition (i).

Soit $x$ un point de X $-\{a, b\}$ et soient U, V des parties ouvertes et fermées, disjointes et non vides, de X$-\{x\}$, telles que X$-\{x\}= U\cup V$. D’après III, p. 278, prop. 17, c), il existe un point de U (resp. de V) dont le complémentaire dans X est connexe. Comme X n’admet que deux tels points, $a$ et $b$, l’un d’eux, disons $a$, est contenu dans U et l’autre dans V. D’après loc. cit., une partie ouverte et fermée, non vide, $U'$ de U, contient un point de $\{a, b\}$, donc contient $a$. Appliquant ceci à $U-U'$, il vient que $U = U'$. Par suite, U est connexe ; c’est la composante connexe de $a$ dans X$-\{x\}$. De même, V est la composante connexe de $b$ dans X $-\{x\}$.

Pour tout $x\in X-\{a, b\}$, notons ainsi $U_x$ et $V_x$ les composantes connexes de $a$ et $b$ dans X $-\{x\}$. D’après ce qui précède, elles sont ouvertes et fermées dans X $-\{x\}$, disjointes, et leur réunion est égale à X $-\{x\}$.

Notons $\preccurlyeq$ la relation dans X définie de la façon suivante : d’une part, $a\preccurlyeq x$ et $x\preccurlyeq b$ pour tout $x\in X$, d’autre part, si $x$ et $y$ appartiennent à X $-\{a, b\}$, alors $x\preccurlyeq y$ si $x\in \overline{U_y}$. Pour $x$ et $y$ dans X $-\{a, b\}$, les parties $V_x$ et $V_y$, ont en commun le point $b$, la relation $x\preccurlyeq y$ équivaut en fait à l’assertion $\overline{U_x}\subset \overline{U_y}($III, p. 278, prop. 17, b)). Il en résulte que la relation $\preccurlyeq$ est une relation d’ordre dans X.

Soient $x$ et $y$ des points de X tels que l’on n’ait pas $x\preccurlyeq y$. Nécessairement, $x=\not a$ et $y=\not b$, et $x\in V_y$. Si $x=b$ ou $y=a$, on a $y\preccurlyeq x$. Supposons alors que $x$ et $y$ sont distincts de $a$ et $b$. Comme les parties $U_x$ et $U_y$ ont en commun le point $a$, on a l’inclusion $\overline{V_x}\subset \overline{V_y}($loc. cit.), d’où, prenant les adhérences des complémentaires, $\overline{U_y}\subset \overline{U_x}$ et, a fortiori, $y\preccurlyeq x$. La relation $\preccurlyeq$ dans l’espace X est donc une relation d’ordre total. Pour tout $x\in X-\{a, b\}$, on a de plus $U_x= ]\leftarrow , x[$ et $V_x= ]x,\rightarrow [$; pour $x, y\in X-\{a, b\}$, on a $]x, y[ = U_y\cap V_x$. Lorsque $x, y$ parcourent les points de X $-\{a, b\}$, les ensembles $U_y\cap V_x$, les ensembles $U_y$ et les ensembles $V_x$ forment une base d’une topologie sur X. Notons $\widetilde{X}$ l’espace topologique correspondant et $i: X\rightarrow \widetilde{X}$ l’application identique de X. Comme, pour tout $x\in X$, les ensembles $U_x$ et $V_x$ sont ouverts dans X, l’application $i$ est continue.

L’espace $\widetilde{X}$ est séparé. En effet, soient $x$ et $y$ des points distincts de $\widetilde{X}$ tels que $x\preccurlyeq y$. Les parties $]\leftarrow , y[$ et $]x,\rightarrow [$ sont des voisinages ouverts de $x$ et $y$; s’ils ont un point commun $z,]\leftarrow , z[$ et $]z,\rightarrow [$ sont alors des voisinages ouverts disjoints de $x$ et $y$. Comme X est compact, l’application $i$ est donc un homéomorphisme (TG, I, p. 63, cor. 2).

Par suite, l’image par $i$ d’une partie dénombrable partout dense de X rencontre chaque intervalle ouvert non vide de l’ensemble ordonné $(X,\preccurlyeq )$. Il résulte alors de la prop. 16 de III, p. 276 qu’il existe un isomorphisme $c$ de l’ensemble ordonné $\mathbf{I}$ sur $(X,\prec )$. D’après la remarque qui suit cette proposition, cet isomorphisme est un homéomorphisme de $\mathbf{I}$ sur l’espace topologique $\widetilde{X}$. L’application $f=i^{-1}\circ c$ est alors un homéomorphisme de $\mathbf{I}$ sur X qui applique 0 sur $a$ et 1 sur $b$.

### 9. Chemins injectifs

#### Proposition 18 {#ta-iii-s2-prop-18 .statement tag=01Y4}

Soit X un espace topologique séparé. Soient $a$ et $b$ des points distincts de X qui appartiennent à la même composante connexe par arcs de X. Il existe un chemin injectif reliant $a$ à $b$ dans X.

Soit $f:\mathbf{I}\rightarrow X$ un chemin reliant $a$ à $b$ dans X. Soit $\mathscr{U}$ l’ensemble des parties ouvertes U de $]0,1[$ telles que $f(x) =f(y)$ pour toute composante connexe $]x, y[$ de U.

#### Lemme 8 {#ta-iii-s2-lem-8 .statement tag=01Y5}

L’ensemble $\mathscr{U}$, ordonné par inclusion, est inductif.

Soit $\mathscr{V}$ une partie totalement ordonnée de $\mathscr{U}$. Démontrons que la réunion V des ensembles appartenant à $\mathscr{V}$ est un élément de $\mathscr{U}$, c’est-àdire que, pour toute composante connexe $]u, v[$ de V, on a $f(u) =f(v)$.

Soit $x$ un point de $]u, v[$. Soit $\mathscr{V}_x$ l’ensemble des $U\in \mathscr{V}$ tels que $x\in U$ ; pour un tel U, notons $]u_U, v_U[$ la composante connexe de $x$ dans U. On a $u_{U'}\leqslant u_U< v_U\leqslant v_{U'}$ si U et $U'$ sont des éléments de $\mathscr{V}_x$ tels que $U\subset U'$. Comme la réunion pour $U\in \mathscr{U}_x$ des $]u_U, v_U[$ est égale à $]u, v[$ d’après le lemme 7 de III, p. 280, on a $u=$ lim $u_U$ et $v=$ lim $v_U$, où les limites sont prises suivant l’ensemble filtrant $\mathscr{V}_x$. Comme l’application $f$ est continue et que l’espace topologique X est séparé, les égalités $f(u_U) =f(v_U)$ pour tout $U\in \mathscr{V}_x$ entraînent que $f(u) =f(v)$, ce qu’il fallait démontrer.

En vertu de E, III, p. 20, th. 2, il existe une partie ouverte U appartenant à $\mathscr{U}$ qui est maximale pour la relation d’inclusion.

Soit $g:\mathbf{I}\rightarrow X$ l’application définie de la façon suivante. Si $t\notin U$, on pose $g(t) =f(t)$ ; sinon, notant $]u, v[$ la composante connexe de $t$ dans U, on pose $g(t) =f(u) =f(v)$, de sorte que l’application $g|[u, v]$ est constante d’image $f(u)$.

La prop. 18 résulte du lemme suivant.

#### Lemme 9 {#ta-iii-s2-lem-9 .statement tag=01Y6}

Il existe une application continue, croissante et surjective $u:\mathbf{I}\rightarrow \mathbf{I}$ et un chemin injectif $c:\mathbf{I}\rightarrow X$ reliant $a$ à $b$ tels que $g=c\circ u$.

Démontrons d’abord que l’application $g$ est continue. Soit $t$ un point de $\mathbf{I}$. Si $t\in U,g$ est constante au voisinage de $t$, donc continue en $t$. Supposons $t\notin U$ et soit W un voisinage ouvert de $g(t)$ dans X. Soit V un intervalle ouvert dans $\mathbf{I}$ contenant $t$ tel que $f(V)\subset W$; il en existe puisque $f$ est continue en $t$. Démontrons que $g(V)\subset W$. Soit $x\in V$ ; si $x\notin U$, on a $g(x) =f(x)$, donc $g(x)\in W$. Supposons alors $x\in U$ et soit $]u, v[$ la composante connexe de $x$ dans U. Observons que $]u, v[$ ne contient pas $t$. Par suite, si $x < t$, on a $x < v\leqslant t$ d’où $v\in V$ et $g(x) =g(v) =f(v)\in f(V)\subset W$. On démontre de même que $g(x)\in W$ si $x > t$. Ainsi, $g$ est continue en $t$.

Soient $u$ et $v$ des points de $\mathbf{I}$ tels que $g(u) =g(v)$ et $u < v$. Démontrons que $]u, v[\subset U$. Posons $U'= U\cup ]u, v[$; c’est une partie ouverte de $]0,1[$.

Si $u$ appartient à U, notons $u'$ la borne inférieure dans $\mathbf{I}$ de la composante connexe de $u$ dans U ; posons $u'=u$ si $u$ n’appartient pas à U. De même, si $v$ appartient à U, notons $v'$ la borne supérieure dans $\mathbf{I}$ de la composante connexe de $v$ dans U ; posons $v'=v$ si $v$ n’appartient pas à U. Alors, $]u', v'[$ est une composante connexe de $U'$ et l’on a $f(u') =g(u) =g(v) =f(v')$. Comme les composantes connexes de $U'$ distinctes de $]u', v'[$ sont des composantes connexes de U, l’ouvert $U'$ est un élément de $\mathscr{U}$. Puisque U est un élément maximal de $\mathscr{U}$ pour la relation d’inclusion, on a $U'= U$ et $]u, v[$ est contenu dans U. Cela démontre que $g$ est constante sur l’intervalle $[u, v]$. Les fibres de $g$ sont donc des intervalles de $\mathbf{I}$, et ces intervalles sont fermés car $g$ est continue.

Notons R la relation d’équivalence associée à $g$ et $p$ la surjection canonique de $\mathbf{I}$ sur $\mathbf{I}/R$. Il existe une unique application continue $g'$ de $\mathbf{I}/R$ dans X telle que $g=g'\circ p$; cette application est injective. D’après le corollaire, III, p. 276, de la prop. 16, il existe une application $u$, croissante, continue et surjective, telle que R soit la relation d’équivalence associée à $u$. Comme l’espace $\mathbf{I}$ est compact et que l’espace X est séparé, l’application $u$ est fermée, donc stricte (I, p. 18, exemple 2). Elle définit par passage au quotient un homéomorphisme $u'$ de $\mathbf{I}/R$ sur $\mathbf{I}$. Alors, l’application $g'\circ (u')^{-1}$ de $\mathbf{I}$ dans X est un chemin injectif d’origine $a$ et de terme $b$.

### 10. Relèvement de chemins

#### Théorème 3 {#ta-iii-s2-thm-3 .statement tag=01Y7}

Soit I un intervalle de $\mathbf{R}$ et soit X un espace topologique non vide et séparé. Soit $p: X\rightarrow I$ une application continue, ouverte et propre dont les fibres sont totalement discontinues (TG, I, p. 83). L’application $p$ est surjective. Pour tout point $x$ de X, elle possède une section continue $s$ telle que $s(p(x)) =x$.

L’ensemble $p(X)$ est une partie ouverte, fermée (TG, I, p. 72, prop. 1), non vide de I. Comme I est connexe, on a $p(X) = I$ ; l’application $p$ est donc surjective.

Pour tout couple $(a, b)\in I\times I$ tel que $a\leqslant b$, notons $F_{a,b}$ l’ensemble des couples $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ tels que $y$ et $z$ appartiennent à une même composante connexe de $\overset{-1}{p}([a, b])$.

#### Lemme 10 {#ta-iii-s2-lem-10 .statement tag=01Y8}

Soient $a,b$ des points de I tels que $a\leqslant b$.

a) L’ensemble $F_{a,b}$ est fermé dans $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$.

b) On a pr$_1(F_{a,b}) =\overset{-1}{p}(a)$ et pr$_2(F_{a,b}) =\overset{-1}{p}(b)$.

c) Soit $c\in I$ tel que $b\leqslant c$. Si $(y, z)$ appartient à $F_{a,b}$ et $(z, t)$ appartient à $F_{b,c}$, alors $(y, t)$ appartient à $F_{a,c}$.

L’ensemble $\overset{-1}{p}([a, b])$ est compact (TG, I, p. 77, prop. 7). Par suite, pour qu’un couple $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ appartienne à $F_{a,b}$, il faut et il suffit que toute partie ouverte et fermée de $\overset{-1}{p}([a, b])$ qui contient $y$ contienne $z$ (TG, II, p. 32, prop. 6).

Posons $Y =\overset{-1}{p}([a, b])$. Pour toute partie ouverte et fermée U de Y, l’ensemble $(U\times U)\cup (Y-U)\times (Y-U)\cap \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ est fermé dans $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$. L’intersection de ces ensembles est égale à $F_{a,b}$, d’où a).

Soit $y\in \overset{-1}{p}(a)$. Notons $\mathscr{U}$ l’ensemble des voisinages ouverts et fermés de $y$ dans Y. L’application de Y dans $[a, b]$ déduite de $p$ par passage aux sous-espaces est ouverte et propre (I, p. 17, prop. 8), donc aussi fermée. Il en résulte que, pour tout ensemble U appartenant à $\mathscr{U},p(U)$ est une partie ouverte et fermée non vide de $[a, b]$; comme l’intervalle $[a, b]$ est connexe, on a $p(U) = [a, b]$ et en particulier $U\cap \overset{-1}{p}(b)=\not\emptyset$. Par suite, $U\cap \overset{-1}{p}(b)_{U\in\mathscr{U}}$ est une famille filtrante décroissante de parties fermées non vides de l’espace compact $\overset{-1}{p}(b)$. L’intersection de cette famille n’est pas vide (TG, I, p. 59) ; soit $z$ un de ses éléments. On a $(y, z)\in F_{a,b}$. Nous avons démontré la relation pr$_1(F_{a,b}) =\overset{-1}{p}(a)$. La relation pr$_2(F_{a,b}) =\overset{-1}{p}(b)$ s’en déduit en remplaçant $p$, I$,a,b$ par $-p$, $-I,-b,-a$.

Sous les hypothèses de c), le couple $(y, t)$ appartient à $\overset{-1}{p}(a)\times \overset{-1}{p}(c)$, l’ensemble $\{y, z\}$ est contenu dans une partie connexe C de $\overset{-1}{p}([a, b])$ et l’ensemble $\{z, t\}$ est contenu dans une partie connexe $C'$ de $\overset{-1}{p}([b, c])$. Alors, $C\cup C'$ est une partie connexe de $\overset{-1}{p}([a, c])$ (TG, I, p. 81, prop. 2) et contient $\{y, t\}$, d’où la relation $(y, t)\in F_{a,c}$.

Revenons à la démonstration du th. 3. Chaque fibre de l’application $p$ est compacte (TG, I, p. 77, prop. 7). D’après le théorème de Tychonoff (TG, I, p. 63, th. 3), l’espace produit $K =\prod_{a\in I}\overset{-1}{p}(a)$ est compact. Soit $K'$ l’ensemble des éléments $(y_a)_{a\in I}$ de K tels que $y_{p(x)}$ soit égal à $x$ et que l’on ait $(y_a, y_b)\in F_{a,b}$ pour tout couple $(a, b)$ d’éléments de I tels que $a < b$. Le théorème 3 résulte du lemme suivant.

#### Lemme 11 {#ta-iii-s2-lem-11 .statement tag=01Y9}

a) L’ensemble $K'$ n’est pas vide.

b) Soit $(s_a)_{a\in I}$ un élément de $K'$. L’application $s:a\mapsto s_a$ de I dans X est une section continue de $p$ telle que $s(p(x)) =x$.

Pour toute partie finie S de I contenant le point $p(x)$, notons $K_S$ l’ensemble des éléments $(y_a)_{a\in I}$ de K satisfaisant la relation $y_{p(x)}=x$ et les relations $(y_a, y_b)\in F_{a,b}$ pour tout couple $(a, b)$ d’éléments de S tels que $a < b$. Les ensembles $K_S$ sont fermés dans K (lemme 10, a)) et forment une famille filtrante décroissante de parties de K, d’intersection $K'$. Pour démontrer que $K'$ n’est pas vide, il suffit de démontrer que, pour toute partie finie S de I contenant le point $p(x)$, l’ensemble $K_S$ n’est pas vide (TG, I, p. 59).

Soit S une telle partie ; ordonnons ses éléments en une suite strictement croissante $(a_1, . . . , a_n)$ et notons $i$ l’entier tel que $p(x) =a_i$. Posons $y_{a_i}=x$. Le lemme 10, b), permet de construire par récurrence des éléments $y_{a_j}\in \overset{-1}{p}(a_j)$, pour $i < j\leqslant n$, et par récurrence descendante des éléments $y_{a_j}\in \overset{-1}{p}(a_j)$ pour $1\leqslant j < i$, de sorte que l’on ait $(y_{a_j}, y_{a_{j+1}})\in F_{a_j,a_{j+1}}$ pour tout entier $j$ tel que $1\leqslant j < n$. D’après le lemme 10, c), on a $(y_a, y_b)\in F_{a,b}$ pour tout couple $(a, b)$ d’éléments de S tels que $a < b$. Comme l’application $p$ est surjective, nous pouvons choisir pour tout $a\in I-S$ un élément $y_a\in \overset{-1}{p}(a)$. La famille $(y_a)_{a\in I}$ ainsi construite appartient à $K_S$, donc $K_S$ n’est pas vide.

Démontrons b). Par définition de $K',s$ est une section de $p$ telle que $s(p(x)) =x$. Soit $a\in I$; démontrons la continuité de $s$ au point $a$. Soit U un voisinage ouvert de $s_a$ dans X. Comme $\overset{-1}{p}(a)$ est un espace compact (TG, I, p. 77, prop. 7) et totalement discontinu, $s_a$ possède dans $\overset{-1}{p}(a)$ un voisinage ouvert et fermé C, contenu dans U (TG, II, p. 32, corollaire). Les ensembles C et $\overset{-1}{p}(a)-C$ sont fermés dans $\overset{-1}{p}(a)$, donc compacts, et ils sont disjoints. Puisque X est séparé, ils possèdent dans X des voisinages ouverts et disjoints V et $V'$ (TG, I, p. 61, prop. 3). L’ensemble $(V\cap U)\cup V'$ est un voisinage ouvert de la fibre $\overset{-1}{p}(a)$ dans X ; comme l’application $p$ est fermée (TG, I, p. 72, prop. 1), $(V\cap U)\cup V'$ contient un ensemble de la forme $\overset{-1}{p}(J)$, où $J\subset I$ est un intervalle ouvert contenant $a($I, p. 75, lemme). Posons $W = V\cap U\cap \overset{-1}{p}(J)$. L’ensemble W est ouvert dans $\overset{-1}{p}(J)$ ; il est aussi fermé dans $\overset{-1}{p}(J)$ puisque l’on a $\overset{-1}{p}(J)-W = V'\cap \overset{-1}{p}(J)$. Soit $b\in J$. L’intervalle fermé de I d’extrémités $a$ et $b$ est contenu dans J. Par hypothèse, $(s_a, s_b)$ appartient à $F_{a,b}$ si $a\leqslant b$ et $(s_b, s_a)$ appartient à $F_{b,a}$ si $b\leqslant a$. Il existe donc une partie connexe de $\overset{-1}{p}(J)$ contenant $\{s_a, s_b\}$. Par suite, le point $s_b$ appartient à toute partie ouverte et fermée de $\overset{-1}{p}(J)$ qui contient $s_a$, donc en particulier à W; a fortiori, $s_b$ appartient à U. On a donc $s(J)\subset U$, ce qui démontre la continuité de $s$ au point $a$.

#### Corollaire {#ta-iii-s2-n10-cor-1 .statement tag=01YA}

Soient X et B des espaces topologiques et $p: X\rightarrow B$ une application continue, ouverte, propre et séparée dont les fibres sont totalement discontinues. Soit I un intervalle de $\mathbf{R}$, soit $f: I\rightarrow B$ une application continue, soit $a$ un point de I et soit $x$ un point de X tel que $f(a) =p(x)$. Il existe une application continue $g: I\rightarrow X$ telle que $p\circ g=f$ et $g(a) =x$.

Posons $X'= I\times_BX$ et notons $p': X'\rightarrow$ I et $f': X'\rightarrow$ X les projections canoniques. L’application $p'$ est continue, ouverte, propre et séparée (I, p. 17, prop. 8 et p. 27, prop. 4). Comme l’espace I est séparé, l’espace $X'$ est séparé (I, p. 26, remarque 3). Les fibres de $p'$ sont totalement discontinues ( I, p. 10, corollaire, a)). D’après le th. 3, il existe une section continue $s'$ de $p'$ qui prend en $a$ la valeur $(a, x)$. L’application $g=f'\circ s'$ de I dans X est continue, on a $p\circ g=p\circ f'\circ s'=f\circ p'\circ s'=f$ et $g(a) =x$, d’où le corollaire.

#### Théorème 4 {#ta-iii-s2-thm-4 .statement tag=01YB}

Soit X un espace topologique, soit G un groupe discret opérant proprement dans X et soit $p: X\rightarrow X/G$ l’application canonique. Soit I un intervalle de $\mathbf{R}$, soit $f: I\rightarrow X/G$ une application continue, soit $a$ un point de I et soit $x$ un point de X tel que $f(a) =p(x)$. Il existe une application continue $\varphi : I\rightarrow X$ telle que $p\circ \varphi =f$ et $\varphi (a) =x$.

Traitons d’abord le cas où I est un intervalle fermé borné de $\mathbf{R}$.

D’après TG, III, p. 29, prop. 3, l’espace X est séparé.

Soit $y$ un point de $X/G$ et soit $x\in X$ tel que $y=p(x)$. Le stabilisateur $K_x$ de $x$ est un sous-groupe fini de G ; de plus, il existe des voisinages $U_x$ de $x$ dans X et $V_y$ de $y$ dans $X/G$ tels que $U_x$ soit stable par $K_x,gU_x\cap U_x=\emptyset$ si $g\notin K_x$ et $p$ induise un homéomorphisme de $U_x/K_x$ sur $V_y$ (TG, III, p. 32, proposition 8). De plus, pour tout $g\in G,p$ induit un homéomorphisme de $gU_x$ sur $V_y$. Comme I est compact, il existe des entiers $m$ et $n$ tels que $m\leqslant 0\leqslant n$ et une suite finie $(a_i)_{m\leqslant i\leqslant n}$ d’éléments de I tels que $a_0=a,I = [a_m, a_n]$, et tels que, pour tout $i\in  \{m, . . . , n-1\},f([a_i, a_{i+1}])$ soit contenu dans un ouvert $V_{y_i}$ de $X/G$ construit comme ci-dessus.

Soit $x_0$ l’unique élément de $\overset{-1}{p}(y_0)$ tel que $x\in U_{x_0}$. Soit $q_0$ l’application canonique de $U_{x_0}$ sur $U_{x_0}/K_{x_0}$; par passage au quotient, l’application $p$ induit un homéomorphisme $i_0$ de $U_{x_0}/K_{x_0}$ sur $V_{y_0}$ tel que $i_0\circ q_0=p|U_{x_0}$. L’application $q_0$ est propre (TG, III, p. 29, prop. 3), ouverte (TG, I, p. 31, exemple 1) et séparée, car X est séparé. Ses fibres sont totalement discontinues, car elles sont finies. D’après le corollaire, III, p. 286, il existe une application continue $\varphi_0: [a_0, a_1]\rightarrow U_{x_0}$ telle que $p\circ \varphi_0=f|[a_0, a_1]$.

On construit de même, par récurrence sur l’entier $i\in  \{0, . . . , n-1\}$, un point $x_i\in \overset{-1}{p}(y_i)$, une application continue $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ dont l’image est contenue dans $U_{x_i}$ telle que $p\circ \varphi_i=f|[a_i, a_{i+1}]$ et telle que $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ si $0\leqslant i < n-1$.

De manière analogue, on construit par récurrence décroissante sur l’entier $i\in  \{m, . . . ,-1\}$ un point $x_i\in \overset{-1}{p}(y_i)$, une application continue $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ dont l’image est contenue dans $U_{x_i}$ telle que $p\circ \varphi_i=$ $f|[a_i, a_{i+1}]$ et telle que $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ si $m\leqslant i <0$.

Il existe une unique application $\varphi : I\rightarrow$ X qui coïncide avec $\varphi_i$ dans $[a_i, a_{i+1}]$ pour $m\leqslant i < n$. Elle est continue (TG, I, p. 19, prop. 4). C’est un relèvement continu de $f$ à X tel que $\varphi (a) =x$.

Cela prouve le théorème lorsque I est compact. Dans le cas général, il existe des suites $(a_n)_{n\in\mathbf{N}}$ et $(b_n)_{n\in\mathbf{N}}$ telles que $(a_n)$ soit stationnaire de limite inf(I), $(b_n)$ soit stationnaire de limite sup(I)$,a=a_0=b_0$, et telle que $(a_n)$ (resp. $(b_n)$) soit constante si I possède un plus petit (resp. un plus grand) élément. D’après ce qui précède, il existe pour tout entier $n\in \mathbf{N}$ un relèvement continu $\varphi_n$ de $f|[a_n, a_{n+1}]$ à X, un relèvement continu $\varphi '_n$ de $f|[b_{n+1}], b_n]$ à X tels que $\varphi_0(a_0) =\varphi '_0(b_0) =x$ $\varphi_{n+1}(a_{n+1}) =\varphi_n(a_{n+1}),\varphi '_{n+1}(b_{n+1}) =\varphi '_n(b_{n+1})$. Il existe une unique application $\varphi : I\rightarrow X$ qui coïncide avec $\varphi_n$ dans $[a_n, a_{n+1}]$ et avec $\varphi '_n$ dans $[b_{n+1}, b_n]$, pour tout $n\in \mathbf{N}$. Elle est continue (loc. cit.) et c’est un relèvement continu de $f$ à X tel que $phi(a) =x$. Le théorème est ainsi démontré.

#### Exemple 1 {#ta-iii-s2-n10-exa-1 .statement tag=01YC}

Soit X un espace topologique séparé et soit G un groupe fini, muni de la topologie discrète, qui opère continûment dans X. L’opération est alors propre (TG, III, p. 28, prop. 2). L’assertion du théorème 4 découle alors directement du corollaire du théorème 3.

#### Exemple 2 {#ta-iii-s2-n10-exa-2 .statement tag=01YD}

Soit $n$ un entier $\geqslant 0$. Notons $P_n$ l’ensemble des polynômes $P\in$ $\mathbf{C}[X]$ unitaires de degré $n$, muni de la topologie pour laquelle l’application $(c_0, . . . , c_{n-1})\mapsto X^n+c_{n-1}X^{n-1}+\cdots +c_0$ est un homéo-morphisme de $\mathbf{C}^n$ sur $P_n$. L’application $p$ de $\mathbf{C}^n$ dans $P_n$ définie par $p(z_1, . . . , z_n) = (X-z_1). . .(X-z_n)$ est continue. Le groupe symétrique $\mathfrak{S}_n$ opère sur $\mathbf{C}^n$ par permutation des facteurs et $p$ définit par passage au quotient un homéomorphisme de $\mathbf{C}^n/\mathfrak{S}_n$ sur $P_n$ (TG, VIII, p. 22, prop. 1, I, p. 23, cor. 1 et TG, VIII, p. 20). On en déduit donc l’énoncé suivant :

Soit I un intervalle de $\mathbf{R}$, soit $(c_0, . . . , c_{n-1})$ une suite d’applications continues de I dans $\mathbf{C}$, soit $a$ un point de I et soit $(z_1, . . . , z_n)$ une suite de nombres complexes telle que l’on ait $(X-z_1). . .(X-z_n) = X^n+$ $c_{n-1}(a)X^{n-1}+\cdots +c_0(a)$. Il existe une suite $(\lambda_1, . . . , \lambda_n)$ d’applications continues de I dans $\mathbf{C}$ telle que l’on ait $\lambda_i(a) =z_i$ pour $1\leqslant i\leqslant n$ et $(X-\lambda_1(t)). . .(X-\lambda_n(t)) = X^n+c_{n-1}(t)X^{n-1}+\cdots +c_0(t)$ pour tout $t\in I$.

## EXERCICES {#ta-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
