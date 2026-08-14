---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 1
section_title: Homotopies, homéotopies
lang: fr
source: ta-i-iv-fr
book_pages: A III.229-A III.256
pdf_pages: 0245-0272
extraction: native
subsections:
    - "no": 1
      title: Applications continues homotopes
      page: 229
      pdf_page: 245
    - "no": 2
      title: Homotopies pointées
      page: 231
      pdf_page: 247
    - "no": 3
      title: Espaces homéotopes
      page: 232
      pdf_page: 248
    - "no": 4
      title: Homéotopies relatives
      page: 234
      pdf_page: 250
    - "no": 5
      title: Rétractions et contractions
      page: 235
      pdf_page: 251
    - "no": 6
      title: Cylindre d’une application
      page: 237
      pdf_page: 253
    - "no": 7
      title: La propriété d’extension des homotopies
      page: 240
      pdf_page: 256
    - "no": 8
      title: Attachement d’un espace topologique
      page: 247
      pdf_page: 263
    - "no": 9
      title: Espace obtenu par contraction d’un sous-espace
      page: 251
      pdf_page: 267
    - "no": 10
      title: Cône d’une application
      page: 253
      pdf_page: 269
statements: 55
exercises: 0
content_sha256: dcb0b3df1f7b9c7e39c8bfb778a0ef557f55897f2df784366f8644b3fd7321a6
---

## § 1. HOMOTOPIES, HOMÉOTOPIES

Dans ce paragraphe et ceux qui suivent, $\mathbf{I}$ désigne l’intervalle $[0,1]$ de $\mathbf{R}$.

### 1. Applications continues homotopes

#### Définition 1 {#ta-iii-s1-def-1 .statement tag=01V4}

Soient X et Y des espaces topologiques et soient $f$ et $g$ des applications continues de X dans Y. On appelle homotopie reliant $f$ à $g$ une application continue $\sigma : X\times \mathbf{I}\rightarrow Y$ telle que, pour tout $x\in X$, on a $\sigma (x,0) =f(x)$ et $\sigma (x,1) =g(x)$. On dit que $f$ est homotope à $g$ s’il existe une homotopie reliant $f$ à $g$.

On dit que $f$ est l’origine et $g$ le terme de l’homotopie $\sigma ($cf. ci-dessous, III, p. 257, remarque 2).

Soit A une partie de X. On dit que l’homotopie $\sigma$ est fixe sur A si, pour tout $a\in A$, l’application $t\mapsto \sigma (a, t)$ de $\mathbf{I}$ dans Y est constante. Dans ce cas, l’origine et le terme de $\sigma$ coïncident en tout point de A.

Soient X et Y des espaces topologiques. On dit que des homotopies $\sigma : X\times \mathbf{I}\rightarrow Y$ et $\tau : X\times \mathbf{I}\rightarrow Y$ sont juxtaposables si le terme de $\sigma$ est

N. Bourbaki et Springer-Verlag Berlin Heidelberg 2   016

N.©  Bourbaki, Topologie algébrique, DOI 10.1007/978-3-662-49361-8_3  229 l’origine de $\tau$, autrement dit si l’on a $\sigma (x,1) =\tau (x,0)$ pour tout $x\in X$. Dans ce cas, l’application $\sigma *\tau$ de $X\times \mathbf{I}$ dans Y définie par

$\sigma (x,2t)$ pour $0\leqslant t\leqslant 1/2$

$$
(\sigma *\tau )(x, t) = \tag{1}
$$

$\tau (x,2t-1)$ pour $1/2\leqslant t\leqslant 1$

est continue (TG, I, p. 19, prop. 4) et est une homotopie reliant l’origine de $\sigma$ au terme de $\tau$. On l’appelle l’homotopie juxtaposée des homotopies $\sigma$ et $\tau$.

Si $\sigma : X\times \mathbf{I}\rightarrow Y$ est une homotopie, l’application $\sigma : X\times \mathbf{I}\rightarrow Y$ définie par $(x, t)\mapsto \sigma (x,1-t)$ est une homotopie reliant le terme de $\sigma$ à l’origine de $\sigma$. On a $\sigma =\sigma$. Si $\sigma$ et $\tau$ sont des homotopies juxtaposables de $X\times \mathbf{I}$ dans Y, les homotopies $\tau$ et $\sigma$ sont juxtaposables et l’on a $\sigma *\tau =\tau *\sigma$.

#### Proposition 1 {#ta-iii-s1-prop-1 .statement tag=01V5}

Soient X et Y des espaces topologiques. La relation « $f$ est homotope à $g$ » est une relation d’équivalence dans l’ensemble $\mathscr{C}(X; Y)$ des applications continues de X dans Y.

Soit $f$ un élément de $\mathscr{C}(X; Y)$. L’application $f\circ$ pr$_1: X\times \mathbf{I}\rightarrow Y$ est une homotopie reliant $f$ à $f$; cette relation est donc réflexive.

Soient $f$ et $g$ des éléments de $\mathscr{C}(X; Y)$ et $\sigma : X\times \mathbf{I}\rightarrow Y$ une homotopie reliant $f$ à $g$. L’application $\sigma : X\times \mathbf{I}\rightarrow Y$ est alors une homotopie reliant $g$ à $f$; la relation considérée est donc symétrique.

Démontrons enfin qu’elle est transitive. Si $f,g$ et $h$ sont des éléments de $\mathscr{C}(X; Y),\sigma$ une homotopie reliant $f$ à $g$ et $\tau$ une homotopie reliant $g$ à $h$, alors $\sigma$ et $\tau$ sont juxtaposables et $\sigma *\tau$ est une homotopie reliant $f$ à $h$.

Soient X et Y des espaces topologiques. La relation d’équivalence « $f$ est homotope à $g$ » dans $\mathscr{C}(X; Y)$ (prop. 1) s’appelle la relation d’homotopie. L’ensemble quotient de $\mathscr{C}(X; Y)$ par cette relation est noté [X; Y]. Ses éléments sont appelés classes d’homotopie d’applications continues de X dans Y. La classe d’homotopie d’une application continue $f: X\rightarrow Y$ sera souvent notée $[f]$.

#### Proposition 2 {#ta-iii-s1-prop-2 .statement tag=01V6}

Soient X, Y et Z des espaces topologiques, $f$ et $f'$ des applications continues de X dans Y$,g$ et $g'$ des applications continues de Y dans Z. Si $f$ est homotope à $f'$ et si $g$ est homotope à $g'$, alors $g\circ f$ est homotope à $g'\circ f'$.

Soient $\sigma$ une homotopie reliant $f$ à $f'$ et $\tau$ une homotopie reliant $g$ à $g'$. Alors, l’application $\theta : X\times \mathbf{I}\rightarrow Z$ définie par $\theta (x, t) =\tau (\sigma (x, t), t)$ est une homotopie reliant $g\circ f$ à $g'\circ f'$.

Soient X, Y et Z des espaces topologiques. Étant données des classes d’homotopie $\varphi \in [X; Y]$ et $\psi \in [Y; Z]$, les applications $g\circ f: X\rightarrow Z$, où $f\in \varphi ,g\in \psi$, appartiennent toutes à une même classe d’homotopie (prop. 2) que l’on note $\psi \circ \varphi$ et que l’on appelle la classe d’homotopie composée des classes $\psi$ et $\varphi$. L’application $[X; Y]\times [Y; Z]\rightarrow [X; Z]$ qui à $(\varphi , \psi )$ associe $\psi \circ \varphi$ est appelée application de composition.

Soit $\varphi \in [X; Y]$ ; on a $\varphi =\varphi \circ$ [Id$_X] =$ [Id$_Y]\circ \varphi$.

Soient X, Y, Z et T des espaces topologiques, soient $\varphi \in [X; Y]$, $\psi \in [Y; Z]$ et $\chi \in [Z; T]$. La classe d’homotopie $\chi \circ (\psi \circ \varphi )$ est égale à $(\chi \circ \psi )\circ \varphi$; on la note $\chi \circ \psi \circ \varphi$.

#### Proposition 3 {#ta-iii-s1-prop-3 .statement tag=01V7}

Soit X un espace topologique et soit $(Y_j)_{j\in J}$ une famille d’espaces topologiques. L’application de $[X;\prod_{j\in J}Y_j]$ dans l’ensemble produit $\prod_{j\in J}[X; Y_j]$ définie par $\varphi \mapsto$ ([pr$_j]\circ \varphi )_{j\in J}$ est bijective.

La surjectivité résulte immédiatement de I, p. 25, prop. 1. Démontrons l’injectivité. Soient $f$ et $g$ des applications continues de X dans $\prod_{j\in J}Y_j$. Pour tout $j\in J$, posons $f_j=$ pr$_j\circ f$ et $g_j=$ pr$_j\circ g$; supposons $f_j$ homotope à $g_j$ et soit $\sigma_j$ une homotopie reliant $f_j$ à $g_j$. L’application $\sigma = (\sigma_j)$ de $X\times \mathbf{I}$ dans $\prod_{j\in J}Y_j$ est continue (loc. cit.) ; c’est une homotopie reliant $f$ à $g$, d’où la proposition.

#### Corollaire {#ta-iii-s1-n1-cor-1 .statement tag=01V8}

Soient $(X_j)_{j\in J}$ et $(Y_j)_{j\in J}$ des familles d’espaces topologiques ayant même ensemble d’indices. Pour tout $j\in J$, soient $f_j$ et $g_j$ des applications continues de $X_j$ dans $Y_j$. Si, pour tout $j\in J$, les applications $f_j$ et $g_j$ sont homotopes, il en est de même des applications produit $f: (x_j)\mapsto (f_j(x_j))$ et $g: (x_j)\mapsto (g_j(x_j))$ de $\prod_{j\in J}X_j$ dans $\prod_{j\in J}Y_j$.

Supposons que l’on ait $[f_j] = [g_j]$ pour tout $j\in J$. On a [pr$_j]\circ [f] =$ $[f_j\circ$ pr$_j]$ et [pr$_j]\circ [g] = [g_j\circ$ pr$_j]$, donc [pr$_j]\circ [f] =$ [pr$_j]\circ [g]$ d’après la prop. 2, d’où $[f] = [g]$ d’après la prop. 3.

### 2. Homotopies pointées

Soient X et Y des espaces topologiques et soit $x$ un point de X. Une homotopie $\sigma : X\times \mathbf{I}\rightarrow Y$ est dite pointée en $x$ si elle est fixe sur $\{x\}$, c’est-à-dire si l’application $t\mapsto \sigma (x, t)$ de $\mathbf{I}$ dans Y est constante. La juxtaposée de deux homotopies pointées en $x$ est pointée en $x$. L’origine et le terme d’une homotopie pointée en $x$ prennent une même valeur $y$ en $x$; ce sont donc des applications continues pointées de $(X, x)$ dans $(Y, y)$.

Soient $(X, x)$ et $(Y, y)$ des espaces topologiques pointés (I, p. 120, définition 1). La relation « $f$ est reliée à $g$ par une homotopie pointée en $x$ » est une relation d’équivalence dans l’ensemble $\mathscr{C}((X, x); (Y, y))$,appelée relation d’homotopie pointée. L’ensemble quotient de $\mathscr{C}((X, x); (Y, y))$ par cette relation d’équivalence est noté $[(X, x); (Y, y)]$. Ses éléments sont appelés classes d’homotopie pointée d’applications continues pointées de $(X, x)$ dans $(Y, y)$.

L’ensemble $\mathscr{C}((X, x); (Y, y))$ est un sous-ensemble de $\mathscr{C}(X; Y)$. On notera que l’homotopie pointée est une relation d’équivalence plus fine que la relation induite par l’homotopie dans $\mathscr{C}(X; Y)$. C’est en général une relation strictement plus fine (voir III, p. 321, exerc. 1 et III, p. 234, exemple 3).

Soit également $(Z, z)$ un espace topologique pointé. Soient $f$ et $f'$ des applications continues pointées de $(X, x)$ dans $(Y, y),g$ et $g'$ des applications continues pointées de $(Y, y)$ dans $(Z, z)$. Si $f$ et $f'$ sont reliées par une homotopie $\sigma$ pointée en $x$, et si $g$ et $g'$ sont reliées par une homotopie $\tau$ pointée en $y$, alors $g\circ f$ et $g'\circ f'$ sont reliées par l’homotopie $\theta : X\times \mathbf{I}\rightarrow Z$, $(u, t)\mapsto \tau (\sigma (u, t), t)$, qui est pointée en $x$. Comme ci-dessus, cela permet de définir l’application de composition de $[(X, x); (Y, y)]\times [(Y, y); (Z, z)]$ dans $[(X, x); (Z, z)]$. Nous laissons au lecteur le soin de formuler et de démontrer pour les applications et homotopies pointées les énoncés analogues à la prop. 3 et à son corollaire.

### 3. Espaces homéotopes

#### Définition 2 {#ta-iii-s1-def-2 .statement tag=01V9}

Soient X et Y des espaces topologiques. On dit qu’une classe d’homotopie $\varphi \in$ [X; Y] est inversible s’il existe une classe d’homotopie $\psi \in [Y; X]$ telle que $\psi \circ \varphi =$ [Id$_X]$ et $\varphi \circ \psi =$ [Id$_Y]$. On dit qu’une application continue est une homéotopie si sa classe d’homotopie est inversible.

Soit $\varphi \in$ [X; Y] une classe d’homotopie inversible. Il existe une unique classe d’homotopie $\psi \in [Y; X]$ ayant les propriétés de la définition 2. Soient en effet $\psi ,\psi '$ des classes ayant ces propriétés ; on a

$\psi =\psi \circ$ [Id$_Y] =\psi \circ \varphi \circ \psi '=$ [Id$_X]\circ \psi '=\psi '$.

Cette unique classe est appelée l’inverse de la classe d’homotopie $\varphi$ et est notée $\varphi^{-1}$.

Soit Z un espace topologique. On a $\chi \circ \varphi \circ \varphi^{-1}=\chi$ pour tout $\chi \in$ [Y; Z] et $\theta \circ \varphi^{-1}\circ \varphi =\theta$ pour tout $\theta \in [X; Z]$. Il en résulte que les applications $\chi \mapsto \chi \circ \varphi$ de [Y; Z] dans [X; Z] et $\theta \mapsto \theta \circ \varphi^{-1}$ de [X; Z] dans [Y; Z] sont des bijections réciproques l’une de l’autre. De même, l’application $\chi \mapsto \varphi \circ \chi$ de [Z; X] dans [Z; Y] est bijective et sa bijection réciproque est l’application $\theta \mapsto \varphi^{-1}\circ \theta$ de [Z; Y] dans [Z; X].

Soient X, Y, Z des espaces topologiques, $\varphi \in [X; Y]$ et $\psi \in [Y; Z]$ des classes d’homotopie inversibles. Alors la classe $\psi \circ \varphi$ est inversible, d’inverse $\varphi^{-1}\circ \psi^{-1}$. En effet, on a

$$
(\psi \circ \varphi )\circ (\varphi^{-1}\circ \psi^{-1}) =\psi \circ (\varphi \circ \varphi^{-1})\circ \psi^{-1}
$$

$=\psi \circ$ [Id$_Y]\circ \psi^{-1}$

$=\psi \circ \psi^{-1}=$ [Id$_Z]$

et, de même, $(\varphi^{-1}\circ \psi^{-1})\circ (\psi \circ \varphi ) =$ [Id$_X]$.

Soient X, Y des espaces topologiques et soit $f: X\rightarrow Y$ une homéo-topie. Toute application continue $g: Y\rightarrow X$ dont la classe est l’inverse de celle de $f$ est dite réciproque (ou inverse) de $f$ à homotopie près. Une telle application $g$ est une homéotopie.

Un homéomorphisme $f$ est une homéotopie, et $[f]^{-1}= [f^{-1}]$. L’application composée de deux homéotopies est une homéotopie. La relation « X et Y sont des espaces topologiques et il existe une homéotopie de X dans Y » est une relation d’équivalence.

#### Définition 3 {#ta-iii-s1-def-3 .statement tag=01VA}

On dit que des espaces topologiques X et Y sont homéotopes s’il existe une homéotopie de X dans Y.

#### Exemple 1 {#ta-iii-s1-n3-exa-1 .statement tag=01VB}

L’espace topologique vide n’est homéotope qu’à lui-même.

#### Exemple 2 {#ta-iii-s1-n3-exa-2 .statement tag=01VC}

Soit X un espace topologique non vide. Pour que X soit homéotope à un espace réduit à un point, il faut et il suffit qu’il existe une application constante $p: X\rightarrow$ X qui soit homotope à l’application identique de X. (Il en est alors ainsi pour toute application constante $q: X\rightarrow X$, car $[p] = [p]\circ [q] =$ [Id$_X]\circ [q] = [q]$.) Soient en effet P un espace réduit à un point, $f: P\rightarrow X$ une application et $g: X\rightarrow P$ l’unique application de X dans P. On a $g\circ f=$ Id$_P$; pour que $f$ soit une homéotopie, il faut et il suffit que $f\circ g$ soit homotope à Id$_X$. Or, $f\circ g$ est constante, d’image $f(P)$.

#### Exemple 3 {#ta-iii-s1-n3-exa-3 .statement tag=01VD}

On dit qu’un espace topologique pointé $(X, x)$ est contractile, ou que l’espace topologique X est contractile en $x$, s’il existe une homotopie pointée en $x$ reliant Id$_X$ à l’application constante de X dans X d’image $\{x\}$. Un tel espace est homéotope à un point. Il existe cependant des espaces homéotopes à un point qui ne sont contractiles en aucun de leurs points, et des espaces contractiles en un point, mais pas en tout point (III, p. 321, exerc. 1).

#### Exemple 4 {#ta-iii-s1-n3-exa-4 .statement tag=01VE}

Soit E l’espace numérique à $n$ dimensions (ou, plus généralement, un espace vectoriel topologique sur $\mathbf{R})$ et soit X un sous-ensemble de E. On dit que l’ensemble X est étoilé en un point $x$ de X si, pour tout $y\in X$ et tout $t\in \mathbf{I}$, le point $tx+ (1-t)y$ appartient à X. Une partie convexe (I, p. 122) de E est étoilée en chacun de ses points.

Un sous-espace topologique X de E étoilé en un de ses points $x$ est contractile en ce point. En effet, l’application $\sigma : X\times \mathbf{I}\rightarrow X$ définie par $\sigma (y, t) =tx+ (1-t)y$ est une homotopie pointée en $x$ reliant Id$_X$ à l’application constante d’image $\{x\}$.

En particulier, tout intervalle de $\mathbf{R}$, toute partie convexe d’un espace numérique ou, plus généralement, d’un espace vectoriel topologique sur $\mathbf{R}$ est contractile en chacun de ses points.

#### Exemple 5 {#ta-iii-s1-n3-exa-5 .statement tag=01VF}

Nous démontrerons ultérieurement (TA, V) que les sphères euclidiennes $\mathbf{S}_n,n\geqslant 1$, ne sont pas des espaces homéotopes à un point. La sphère unité d’un espace hilbertien de type dénombrable et de dimension infinie est contractile en chacun de ses points (EVT, V, p. 71, exerc. 13).

### 4. Homéotopies relatives

Soient X, Y des espaces topologiques, soit A un sous-espace de X et soit B un sous-espace de Y.

Soit $f: X\rightarrow Y$ une application continue telle que $f(A)\subset B$. On dit que $f$ est une homéotopie du couple $(X,A)$ sur le couple $(Y,B)$ s’il existe une application continue $g: Y\rightarrow X$ telle que $g(B)\subset A$, une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$, fixe sur A, reliant Id$_X$ à $g\circ f$, et une homotopie $\tau : Y\times \mathbf{I}\rightarrow Y$, fixe sur B, reliant Id$_Y$ à $f\circ g$.

Supposons ces conditions satisfaites. Alors :

a) L’application $f$ est une homéotopie de X dans Y, l’application $g$ est une homéotopie de Y dans X, et ces homéotopies sont inverses l’une de l’autre à homotopie près.

b) L’application $g$ est alors une homéotopie du couple $(Y,B)$ sur le couple $(X,A)$, dite inverse de $f$ à homotopie près.

c) Les applications $f$ et $g$ définissent par passage aux sous-espaces des homéomorphismes de A sur B réciproques l’un de l’autre.

On dit que les couples $(X,A)$ et $(Y,B)$ sont homéotopes s’il existe une homéotopie du couple $(X,A)$ sur le couple $(Y,B)$. La relation « X, Y sont des espaces topologiques, A est un sous-espace de X, B est un sous-espace de Y et les couples $(X,A)$ et $(Y,B)$ sont homéotopes » est une relation d’équivalence.

### 5. Rétractions et contractions

#### Définition 4 {#ta-iii-s1-def-4 .statement tag=01VG}

Soit X un espace topologique et soit A une partie de X.

On appelle rétraction de X sur A une application continue de X dans A qui est une rétraction de l’injection canonique de A dans X. S’il existe une rétraction de X sur A, on dit que X peut se rétracter sur A, ou encore que A est un rétracte de X.

Soit X un espace topologique et soit A un sous-espace de X.

Supposons qu’il existe une rétraction $r$ de X sur A. Le sous-espace A s’identifie à l’ensemble des points $x\in X$ tels que $x=r(x)$. Si X est un espace séparé, A est alors fermé dans X.

D’après le lemme suivant, pour qu’un sous-espace A soit un rétracte de X, il faut et il suffit que toute application continue de A dans un espace topologique Y s’étende en une application continue de X dans Y.

#### Lemme 1 {#ta-iii-s1-lem-1 .statement tag=01VH}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Les conditions suivantes sont équivalentes :

(i) Pour tout espace topologique Z et toute application continue $g: X\rightarrow Z$, il existe une application continue $g': Y\rightarrow Z$ telle que $g=$ $g'\circ f$;

(ii) L’application $f$ est injective et possède une rétraction continue ;

(iii) L’application $f$ définit un homéomorphisme de X sur son image $f(X)$, laquelle est un rétracte de Y.

Supposons que $f$ soit injective et soit $r: Y\rightarrow$ X une rétraction continue de l’application $f$. Pour toute application continue $g: X\rightarrow Z$, l’application $g'=g\circ r: Y\rightarrow Z$ vérifie $g'\circ f=g\circ r\circ f=g$. Cela démontre que (ii)$\Rightarrow$(i).

Supposons que la condition (i) soit satisfaite. Soit $g: X\rightarrow X$ l’application identique. Par hypothèse, il existe une application continue $g': Y\rightarrow X$ telle que $g'\circ f=g$. Cela entraîne que l’application $f$ est injective et que $g'$ est une rétraction continue de $f$.

L’équivalence des propriétés (ii) et (iii) est immédiate.

#### Définition 5 {#ta-iii-s1-def-5 .statement tag=01VI}

Soit X un espace topologique et soit A une partie de X. On appelle contraction de X sur A une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ fixe sur A dont l’origine est l’application identique de X et dont le terme est une rétraction de X sur A. S’il existe une contraction de X sur A, on dit que X peut se contracter sur A, ou encore que A est un contracté de X.

#### Remarque {#ta-iii-s1-n5-rem-1 .statement tag=01VJ}

En d’autres termes, une contraction de X sur A est une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ ayant les propriétés suivantes :

(i) $\sigma (x,0) =x$ pour tout $x\in X$ ;

(ii) $\sigma (x,1)\in A$ pour tout $x\in X$ ;

(iii) $\sigma (x, t) =x$ pour tout $x\in A$ et tout $t\in \mathbf{I}$.

Pour qu’il existe une contraction de X sur A, il faut et il suffit que l’injection canonique de A dans X soit une homéotopie du couple $(A,A)$ sur le couple $(X,A)$.

Soit $a$ un point de X. Une contraction de X sur le sous-espace $\{a\}$ n’est autre qu’une homotopie pointée en $a$ reliant l’application Id$_X$ à l’application constante d’image $\{a\}$. Par suite, X se contracte sur $\{a\}$ si et seulement si X est contractile en $a$ (exemple 3 de III, p. 234).

Soit X un espace topologique et soit A une partie de X. Soit $\sigma$ une contraction de X sur A. L’application $r$ de X dans A définie par $r(x) =\sigma (x,1)$ est une rétraction de X sur A et $\sigma$ est une homotopie reliant Id$_X$ à $r$. Les relations $r\circ i=$ Id$_A$ et $i\circ r=r$ entraînent alors que les applications $i$ et $r$ sont des homéotopies, réciproques l’une de l’autre à homotopie près.

#### Définition 6 {#ta-iii-s1-def-6 .statement tag=01VK}

Avec les notations qui précèdent, on dit que $\sigma$ est une contraction forte si, de plus, on a $r(\sigma (x, t)) =r(x)$ pour tout $x\in X$ et tout $t\in \mathbf{I}$,

#### Exemple {#ta-iii-s1-n5-exa-1 .statement tag=01VL}

Soit X le complémentaire de l’origine dans $\mathbf{B}_n$. L’application de $X\times \mathbf{I}$ dans X donnée par $(x, t)\mapsto ((1-t) +t_{\|x\|}^1)x$ est une contraction forte de X sur $\mathbf{S}_{n-1}$. La rétraction de X sur $\mathbf{S}_{n-1}$ qui lui est associée est l’application donnée par $x\mapsto x/\|x\|$.

#### Lemme 2 {#ta-iii-s1-lem-2 .statement tag=01VM}

Soit X un espace topologique, soit U un ouvert de X et soit $\sigma$ une contraction forte de X sur X-U. Alors, $\sigma (U\times \mathbf{I})\subset U$. En particulier, $\sigma (U\times  \{1\})$ est contenu dans la frontière de U.

Soit $x\in U$. L’ensemble des nombres réels $t\in \mathbf{I}$ tels que $\sigma (x, t)\in U$ est ouvert dans $\mathbf{I}$ et contient 0 ; soit $s$ sa borne supérieure. On a $\sigma (x, s)\in U$. Si $s <1,\sigma (x, s)\notin U$, par définition de $s$; il en est de même si $s= 1$ car $\sigma (x,1)\in X-U$. Par suite, $\sigma (x, s)\in$ Fr(U). Par définition d’une contraction forte, on a alors $\sigma (x, s) =\sigma (\sigma (x, s),1) =\sigma (x,1)$; en particulier, $\sigma (x,1)\in U$. Par conséquent, $\sigma (x,1)$ appartient à la frontière $U\cap (X-U)$ de U.

Soit $t\in \mathbf{I}$; si $\sigma (x, t)\notin U$, il vient encore $\sigma (x, t) =\sigma (\sigma (x, t),1) =$ $\sigma (x,1)$, donc $\sigma (x, t)\in U$, d’où le lemme.

### 6. Cylindre d’une application

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. Notons U l’espace topologique somme de l’espace $U_1= X\times \mathbf{I}$ et de l’espace $U_2$ = Y et identifions $U_1$ et $U_2$ à des sous-espaces de U par les injections canoniques. Soit R la relation d’équivalence sur U la plus fine pour laquelle les points $(x,1)$ de $U_1$ et $f(x)$ de $U_2$ sont équivalents, pour tout $x\in X$.

#### Définition 7 {#ta-iii-s1-def-7 .statement tag=01VN}

On appelle cylindre de l’application $f$ et on note Cyl($f$) l’espace topologique quotient $U/R$.

Notons $\alpha_f: X\times \mathbf{I}\rightarrow$ Cyl($f$) et $\beta_f: Y\rightarrow$ Cyl($f$) les restrictions à $U_1$ et $U_2$ de la surjection canonique de U sur $U/R$. L’application $\alpha_f$ est une homotopie et son terme est $\beta_f\circ f$.

Proposition 4 (Propriété universelle des cylindres)

Soit Z un espace topologique, soit $\beta : Y\rightarrow Z$ une application continue et soit $\alpha : X\times \mathbf{I}\rightarrow Z$ une homotopie dont le terme est $\beta \circ f$. Il existe une unique application continue $\varphi$ de Cyl($f$) dans Z telle que $\alpha =\varphi \circ \alpha_f$ et $\beta =\varphi \circ \beta_f$.

L’application $\psi$ de U dans Z qui coïncide avec $\alpha$ dans $X\times \mathbf{I}$ et avec $\beta$ dans Y est continue. On a $\alpha (x,1) =\beta (f(x))$ pour tout $x\in X$, donc $\psi$ définit par passage au quotient une application continue $\varphi$ de Cyl($f$) dans Z telle que $\alpha =\varphi \circ \alpha_f$ et $\beta =\varphi \circ \beta_f$. Comme les images de $\alpha_f$ et de $\beta_f$ recouvrent Cyl($f$)$,\varphi$ est la seule application de Cyl($f$) dans Z satisfaisant ces relations.

#### Exemple 1 {#ta-iii-s1-n6-exa-1 .statement tag=01VO}

Soient $X',Y'$ des espaces topologiques et $f': X'\rightarrow Y'$ une application continue. Soient $u: X\rightarrow X'$ et $v: Y\rightarrow Y'$ des applications continues telles que $f'\circ u=v\circ f$. Il existe une unique application continue $w:$ Cyl($f$)$\rightarrow$ Cyl($f'$) telle que $w\circ \alpha_f=\alpha_{f'}\circ (u\times$ Id$_{\mathbf{I}})$ et $w\circ \beta_f=\beta_{f'}\circ v$.

D’après la prop. 4, appliquée à Z = Y et $\beta =$ Id$_Y$, il existe une unique application continue $\gamma_f:$ Cyl($f$)$\rightarrow Y$ telle que $\gamma_f(\alpha_f(x, s)) =f(x)$ et $\gamma_f(\beta_f(y)) =y$ pour $x\in X,s\in \mathbf{I}$ et $y\in Y$.

#### Proposition 5 {#ta-iii-s1-prop-5 .statement tag=01VP}

L’application $\alpha_f$ induit un homéomorphisme de $X\times [0,1[$ sur une partie ouverte de Cyl($f$). L’application $\beta_f$ définit un homéomorphisme de Y sur le complémentaire de cet ouvert. L’application $\beta_f\circ \gamma_f$ est une rétraction continue de Cyl($f$) sur $\beta_f(Y)$.

L’ensemble $X\times [0,1[$ est un ouvert de U, saturé pour la relation R, et la relation d’équivalence induite par R dans $X\times [0,1[$ est la relation d’égalité. La première assertion en résulte (TG, I, p. 23, cor. 10).

Le complémentaire de $\alpha_f(X\times [0,1[)$ est $\beta_f(Y)$. Comme on a $\gamma_f\circ \beta_f=$ Id$_Y,\beta_f$ définit un homéomorphisme de Y sur $\beta_f(Y)$ et $\beta_f\circ \gamma_f$ est une rétraction continue de l’injection canonique de $\beta_f(Y)$ dans Cyl($f$).

Le sous-espace fermé $\beta_f(Y)$ de Cyl($f$) s’appelle la base du cylindre de $f$. L’application $\beta_f\circ \gamma_f$ s’appelle la rétraction canonique de Cyl($f$) sur sa base.

Considérons les applications $\sigma_1: U_1\times \mathbf{I}\rightarrow$ Cyl($f$) et $\sigma_2: U_2\times \mathbf{I}\rightarrow$ Cyl($f$) définies par

$\sigma_1((x, s), t) =\alpha_f(x,(1-t)s+t)$ pour $(x, s)\in X\times \mathbf{I}$ et $t\in \mathbf{I}$

$\sigma_2(y, t) =\beta_f(y)$ pour $y\in Y$ et $t\in \mathbf{I}$.

Elles sont continues. Pour $x\in X$ et $t\in \mathbf{I}$, on a

$$
\sigma_1((x,1), t) =\alpha_f(x,1) =\beta_f(f(x)) =\sigma_2(f(x), t)
$$

Il existe donc une unique application $\sigma_f$ de Cyl($f$)$\times \mathbf{I}$ dans Cyl($f$) telle que $\sigma_f\circ (\alpha_f\times$ Id$_{\mathbf{I}}) =\sigma_1$ et $\sigma_f\circ (\beta_f\times$ Id$_{\mathbf{I}}) =\sigma_2$. L’application $\sigma_f$ est continue (I, p. 19, prop. 10).

#### Proposition 6 {#ta-iii-s1-prop-6 .statement tag=01VQ}

L’application $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) est une contraction forte de Cyl($f$) sur sa base. Son terme est la rétraction canonique de Cyl($f$) sur sa base.

L’application $\sigma_f$ est une homotopie. Les relations $\sigma_f(\alpha_f(x, s),0) =$ $\alpha_f(x, s)$ et $\sigma_f(\beta_f(y),0) =\beta_f(y)$ entraînent que l’origine de $\sigma_f$ est l’application identique de Cyl($f$). Notons $r_f$ le terme de $\sigma_f$. Les relations

$$
\sigma_f(\alpha_f(x, s),1) =\alpha_f(x,1) =\beta_f(f(x)) = (\beta_f\circ \gamma_f)(\alpha_f(x, s))
$$

et $\sigma_f(\beta_f(y),1) =\beta_f(y) = (\beta_f\circ \gamma_f)(\beta_f(y))$ entraînent que $r_f$ est la rétraction canonique $\beta_f\circ \gamma_f$ de Cyl($f$) sur sa base.

Pour $(x, s)\in X\times \mathbf{I}$ et $t\in \mathbf{I}$, on a

$$
r_f(\sigma_f(\alpha_f(x, s), t)) =r_f(\alpha_f(x, s(1-t) +t)) =\beta_f(f(x)) =r_f(\alpha_f(x, s))
$$

Pour $y\in Y$ et $t\in \mathbf{I}$, on a $r_f(\sigma_f(\beta_f(y), t)) =r_f(\beta_f(y))$. Par conséquent, $\sigma_f$ est une contraction forte de Cyl($f$) sur sa base.

L’application $\sigma_f$ est appelée la contraction canonique du cylindre de $f$ sur sa base.

#### Remarque 1 {#ta-iii-s1-n6-rem-1 .statement tag=01VR}

Soit A une partie de $X\times \mathbf{I}$ et soit $A_1$ l’ensemble des points $x\in X$ tels que $(x,1)\in A$. On a $\alpha^{-1}_f(\alpha_f(A)) = A\cup^-f^1(f(A_1))\times \{1\}$ et $\beta^{-1}_f(\alpha_f(A)) =f(A_1)$. Par suite, l’application $\alpha_f$ est fermée (resp. ouverte) si $f$ l’est.

#### Remarque 2 {#ta-iii-s1-n6-rem-2 .statement tag=01VS}

Supposons que l’application $f$ soit propre. Soit P un point de Cyl($f$). Si P = $\alpha_f(x, t)$, avec 0 $\leqslant t <$ 1 et $x\in$ X, on a $\alpha^{-1}_f(P) = (x, t)$. Dans le cas contraire, il existe $y\in Y$ tel que $P =\beta_f(y)$ et $\alpha^-_f^1(P) =^-f^1(y)\times  \{1\}$. Cela démontre que les fibres de l’application $\alpha_f$ sont quasi-compactes. L’application $\alpha_f$ est alors propre (TG, I, p. 75, th. 1), car elle est fermée.

D’après la prop. 5 et TG, I, p. 72, prop. 2, l’application $\beta_f$ est elle-même propre. Par suite, si $f$ est propre, la surjection canonique de U sur Cyl($f$) est propre donc, en particulier, universellement stricte (I, p. 20, corollaire).

#### Remarque 3 {#ta-iii-s1-n6-rem-3 .statement tag=01VT}

Si les espaces X et Y sont séparés, il en est de même du cylindre de l’application $f$. En effet, soient $z$ et $z'$ deux points distincts de Cyl($f$) et démontrons qu’ils possèdent des voisinages disjoints. Distinguons trois cas.

– Il existe $(x, t)$ et $(x', t')\in X\times [0,1[$ tels que $z=\alpha_f(x, t)$ et $z'=\alpha_f(x', t')$.

Dans ce cas, l’assertion résulte de ce que l’espace $X\times [0,1[$ est séparé (TG, I, p. 54, prop. 7) et que l’application $\alpha_f$ induit un homéo-morphisme de cet espace sur un sous-espace ouvert de Cyl($f$).

– Il existe $(x, t)\in X\times [0,1[$ tel que $z=\alpha_f(x, t)$ et $y'\in Y$ tel que $z'=\beta_f(y')$.

Alors, $\alpha_f(X\times [0,^{t+1}_2$ [) et Cyl($f$)$-\alpha_f(X\times [0,^{t+1}_2$ ]) sont des voisinages ouverts disjoints de $z$ et $z'$ dans Cyl($f$).

– Il existe $y$ et $y'\in Y$ tels que $z=\beta_f(y),z'=\beta_f(y')$.

Dans ce cas, $y=\not y'$; comme Y est séparé, il existe un voisinage ouvert V de $y$ dans Y et un voisinage ouvert $V'$ de $y'$ dans Y tels que $V\cap V'=\emptyset$. Alors, $(\beta_f\circ \gamma_f)^{-1}(V)$ et $(\beta_f\circ \gamma_f)^{-1}(V')$ sont des parties ouvertes disjointes de Cyl($f$) contenant respectivement $y$ et $y'$.

### 7. La propriété d’extension des homotopies

#### Définition 8 {#ta-iii-s1-def-8 .statement tag=01VU}

Soit X un espace topologique et soit A une partie de X. On dit que le couple $(X,A)$ possède la propriété d’extension des homotopies si, pour tout espace topologique Y, toute application continue $f: X\rightarrow Y$ et toute homotopie $\sigma : A\times \mathbf{I}\rightarrow Y$ dont le terme est l’application $f|A$, il existe une homotopie $\tau : X\times \mathbf{I}\rightarrow Y$ prolongeant $\sigma$ et dont le terme est l’application $f$.

#### Remarque 1 {#ta-iii-s1-n7-rem-1 .statement tag=01VV}

Soit X un espace topologique et soit A une partie de X telle que le couple $(X,A)$ possède la propriété d’extension des homotopies. Soit Y un espace topologique, soit $f: X\rightarrow Y$ une application continue et soit $\sigma : A\times \mathbf{I}\rightarrow Y$ une homotopie dont l’origine est l’application $f|A$. L’application $\sigma : A\times \mathbf{I}\rightarrow Y$ définie par $(a, t)\mapsto \sigma (a,1-t)$ est une homotopie de terme $f|A$; soit $\tau : X\times \mathbf{I}\rightarrow Y$ une homotopie de terme $f$ qui prolonge $\sigma$. L’application $\tau : X\times \mathbf{I}\rightarrow Y$ donnée par $(x, t)\mapsto \tau (x,1-t)$ est alors une homotopie qui prolonge $\sigma$ et dont l’origine est l’application $f$.

Soit X un espace topologique, soit A un sous-espace de X et soit $i: A\rightarrow X$ l’injection canonique. Notons $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) et $\beta_i: X\rightarrow$ Cyl($i$) les applications canoniques. Soit $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ l’unique application continue telle que $j(\alpha_i(a, s)) = (i(a), s)$ et $j(\beta_i(x)) = (x,1)$ pour $a\in A,s\in \mathbf{I}$ et $x\in X$. Elle est injective ; son image est le sous-espace $(A\times \mathbf{I})\cup (X\times  \{1\})$ de $X\times \mathbf{I}$. L’application $j$ est fermée si A est fermé dans X. Elle n’est pas toujours stricte (III, p. 325, exerc. 17).

#### Proposition 7 {#ta-iii-s1-prop-7 .statement tag=01VW}

Avec les notations ci-dessus, les assertions suivantes sont équivalentes :

(i) Le couple $(X,A)$ possède la propriété d’extension des homotopies ;

(ii) Pour tout espace topologique Y et toute application continue $g:$ Cyl($i$)$\rightarrow Y$, il existe une application continue $g': X\times \mathbf{I}\rightarrow Y$ telle que $g=g'\circ j$;

(iii) L’injection $j$ possède une rétraction continue ;

(iv) L’application $j$ est stricte et il existe une contraction de $X\times \mathbf{I}$ sur l’image de $j$.

Supposons que le couple $(X,A)$ possède la propriété d’extension des homotopies. Soit $g:$ Cyl($i$)$\rightarrow Y$ une application continue ; posons $\sigma =g\circ \alpha_i$ et $f=g\circ \beta_i$. L’application $f: X\rightarrow$ Y est continue et $\sigma : A\times \mathbf{I}\rightarrow Y$ est une homotopie dont le terme est l’application $f|A$. Il existe donc une homotopie $g': X\times \mathbf{I}\rightarrow Y$ de terme $f$ qui prolonge $\sigma$. On a $g'\circ j(\alpha_i(a, s)) =g'(a, s) =\sigma (a, s) =g(\alpha_i(a, s))$ et $g'\circ j(\beta_i(x)) =$ $g'(x,1) =f(x) =g(\beta_i(x))$ pour $a\in A,s\in \mathbf{I}$ et $x\in X$. Par suite, $g'\circ j=g$, d’où (ii).

Inversement, supposons que l’assertion (ii) soit vérifiée et démontrons que le couple $(X,A)$ possède la propriété d’extension des homotopies. Soit Y un espace topologique, soit $f: X\rightarrow Y$ une application continue et soit $\sigma : A\times \mathbf{I}\rightarrow Y$ une homotopie dont le terme est égal à $f|A$. Il existe une unique application continue $g:$ Cyl($i$)$\rightarrow Y$ telle que $g\circ \alpha_i=\sigma$ et $g\circ \beta_i=f$ (III, p. 238, prop. 4). Toute application $g': X\times \mathbf{I}\rightarrow Y$ telle que $g=g'\circ j$ est alors une homotopie de terme $f$ qui prolonge $\sigma$.

L’équivalence des assertions (ii) et (iii) est un cas particulier du lemme 1 de III, p. 235.

Supposons que l’injection $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ admette une rétraction continue $r$. L’application $j$ définit donc un homéomorphisme de Cyl($i$) sur le sous-espace $T = (A\times \mathbf{I})\cup (X\times  \{1\})$ de $X\times \mathbf{I}($loc. cit.). Elle est donc stricte.

Posons $\rho =$ pr$_1\circ j\circ r$ et $\theta =$ pr$_2\circ j\circ r$. Si $x\in A$ ou si $s= 1$, on a $\rho (x, s) =x$ et $\theta (x, s) =s$ Pour $(x, s)\in X\times \mathbf{I}$ et $t\in \mathbf{I}$, posons

$$
\sigma ((x, s), t) = (\rho (x,(1-t) +st),(1-t)s+t\theta (x, s))
$$

L’application $\sigma : (X\times \mathbf{I})\times \mathbf{I}\rightarrow X\times \mathbf{I}$ est continue. Pour $(x, s)\in X\times \mathbf{I}$, on a

$$
\sigma ((x, s),0) = (\rho (x,1), s) = (x, s)
$$

et

$$
\sigma ((x, s),1) = (\rho (x, s), \theta (x, s)) =j\circ r(x, s)
$$

pour $x\in X$ et $t\in \mathbf{I}$, on a

$$
\sigma ((x,1), t) = (\rho (x,1),(1-t) +t\theta (x,1)) = (x,1)
$$

tandis que, pour $(x, s)\in A\times \mathbf{I}$ et $t\in \mathbf{I}$, on a

$$
\sigma ((x, s), t) = (x,(1-t)s+ts) = (x, s)
$$

Par suite, $\sigma$ est une contraction de $X\times \mathbf{I}$ sur T. Cela montre que l’assertion (iii) implique l’assertion (iv).

L’implication (iv)$\Rightarrow$(iii) est évidente.

#### Remarque 2 {#ta-iii-s1-n7-rem-2 .statement tag=01VX}

Soit X un espace topologique séparé et soit A une partie de X telle que le couple $(X,A)$ possède la propriété d’extension des homotopies. Notons $i: A\rightarrow$ X l’injection canonique. Soit $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ l’injection canonique et soit $r$ une rétraction continue de l’application $j$. Le sous-espace $j$(Cyl($i$)) est égal à l’ensemble des couples $(x, t)\in X\times \mathbf{I}$ tels que $j(r(x, t)) = (x, t)$. Comme l’espace $X\times \mathbf{I}$ est séparé, le sous-ensemble $j$(Cyl($i$)) est fermé dans $X\times \mathbf{I}$. L’ensemble A, égal à l’ensemble des $x\in X$ tels que $(x,0)\in j$(Cyl($i$)), est alors une partie fermée de X.

#### Lemme 3 {#ta-iii-s1-lem-3 .statement tag=01VY}

Soient X et Y des espaces topologiques, soit $p: X\rightarrow Y$ une application continue propre et ouverte, et soit $f: X\rightarrow \mathbf{R}$ une application continue. L’application $g: Y\rightarrow \mathbf{R}$ donnée par $y\mapsto$ sup $f(x)$ est continue.

$x\in^-p^1(y)$

Soit $b\in Y$. Comme $p$ est propre, sa fibre $^-p^1(b)$ est un espace quasi-compact ; on a donc $g(b)\in \mathbf{R}\cup  \{-\infty \}$.

Soit $m\in \mathbf{R}$ tel que $g(b)< m$. Pour tout $a\in^-p^1(b)$, on a $f(a)\leqslant$ $g(b)< m$; soit $V_a$ un voisinage de $a$ dans X tel que $f(x)< m$ pour tout $x\in V_a$. La réunion V des ensembles $V_a$ est un voisinage de $^-p^1(b)$ dans X. D’après le lemme 5 (I, p. 75), il existe un voisinage W de $b$ dans Y tel que $^-p^1(W)\subset V$. Pour tout $y\in W$, on a $g(y)\leqslant m$. Cela prouve que $g$ est semi-continue supérieurement en $b$.

Démontrons maintenant que $g$ est semi-continue inférieurement en $b$. On peut supposer $g(b)\in \mathbf{R}$. Soit $m\in \mathbf{R}$ tel que $m < g(b)$. Soit $a\in^-p^1(b)$ tel que $m < f(b)$ ; soit alors V un voisinage de $a$ dans X tel que $f(x)> m$ pour tout $x\in V$. Il s’ensuit que $g(y)> m$ pour tout $y\in p(V)$. Comme $p$ est ouverte, $p(V)$ est un voisinage de $b$, si bien que $g$ est semi-continue inférieurement.

Le lemme est ainsi démontré.

#### Théorème 1 {#ta-iii-s1-thm-1 .statement tag=01VZ}

Soit X un espace topologique et soit A un sous-espace fermé de X ; notons $i: A\rightarrow X$ l’injection canonique. Les assertions suivantes sont équivalentes :

(i) Le couple $(X,A)$ possède la propriété d’extension des homotopies ;

(ii) Il existe une application continue $\varphi : X\rightarrow \mathbf{I}$ telle que $A =^-\varphi^1(0)$ et une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ fixe sur A dont le terme est l’application identique de X et telle que $\sigma (x,0)\in A$ pour tout point $x\in X$ tel que $\varphi (x)= 1\not$ .

(iii) Il existe une application continue $\varphi : X\rightarrow \mathbf{R}_+$ telle que $A =^-\varphi^1(0)$ et une homotopie $\sigma :^-\varphi^1(\mathbf{I})\times \mathbf{I}\rightarrow X$, fixe sur A, telle que $\sigma (x,1) =x$ et $\sigma (x,0)\in A$ pour tout $x\in^-\varphi^1(\mathbf{I})$.

(iv) Il existe une application continue $\varphi : X\rightarrow \mathbf{R}_+$ telle que $A\subset^-\varphi^1(0)$ et une application continue

$$
\sigma :\{(x, t)\in X\times \mathbf{I}|t+\varphi (x)\geqslant 1\} \rightarrow X
$$

telle que $\sigma (x,1) =x$ pour tout $x\in X$ et $\sigma (x,1-\varphi (x))\in A$ pour tout $x\in X$ tel que $\varphi (x)\leqslant 1$.

Nous noterons $i$ l’injection canonique de A dans X$,\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) et $\beta_i: X\rightarrow$ Cyl($i$) les applications canoniques, et $j$ l’application de Cyl($i$) dans $X\times \mathbf{I}$ telle que $j(\alpha_i(x, s)) = (x, s)$ pour $(x, s)\in A\times \mathbf{I}$ et $j(\beta_i(x)) = (x,1)$ pour $x\in X$.

Supposons que le couple $(X,A)$ possède la propriété d’extension des homotopies et soit $r: X\times \mathbf{I}\rightarrow$ Cyl($i$) une rétraction continue de l’application $j($III, p. 241, prop. 7). Notons $\sigma$ l’application continue pr$_1\circ j\circ r$ de $X\times \mathbf{I}$ dans X. Pour tout $(x, t)\in X\times \mathbf{I}$, on a $|$pr$_2(j(r(x, t)))-t|\leqslant 1$. Comme $\mathbf{I}$ est compact, la première projection pr$_1: X\times \mathbf{I}\rightarrow X$ est une application propre ; elle est aussi ouverte. D’après le lemme 3, l’application $\varphi : X\rightarrow \mathbf{I}$ donnée par

$x\mapsto$ sup$_{t\in\mathbf{I}}(|$pr$_2(j(r(x, t)))-t|)$

est donc continue.

Pour $x\in X$, on a $\sigma (x,1) =x$. Soit $x\in X$ tel que $\sigma (x,0)\notin A$ ; alors pr$_2(j(r(x,0))) = 1$ et $\varphi (x)\geqslant 1$. Pour $x\in A$ et $t\in \mathbf{I}$, on a $j(r(x, t)) = (x, t)$ ; par suite, $\sigma (x, t) =x$ et $\varphi (x) = 0$. Inversement, soit $x\in X$ tel que $\varphi (x) = 0$. On a donc pr$_2(j(r(x, t))\leqslant t$ pour tout $t\in \mathbf{I}$; si $t <1$, cela entraîne $j(r(x, t))\in A\times \mathbf{I}$; comme A est fermé dans X, on a donc $j(r(x,1))\in A\times \mathbf{I}$, donc $x\in A$.

Cela démontre que (i) entraîne (ii).

Soient $\varphi$ et $\sigma$ des applications vérifiant les propriétés de l’assertion (ii). Posons $\varphi_1= 2\varphi$ et soit $\sigma_1$ la restriction de $\sigma$ à $^-\varphi^1_1(\mathbf{I})\times \mathbf{I}$. On a $^-\varphi^1_1(0) = A$; pour $a\in A,\sigma_1(a, t) =a$ pour tout $a\in A$. Soit $x\in X$ tel que $\varphi_1(x)\leqslant 1$ ; on a $\sigma_1(x,1) =x$; en outre, $\varphi (x) =\varphi_1(x)/2<1$, donc $\sigma_1(x,0)\in A$. Ainsi, (ii) implique (iii).

Démontrons que (iii) entraîne (iv). Soient $\varphi : X\rightarrow \mathbf{R}$ et $\sigma :^-\varphi^1(\mathbf{I})\times$ $\mathbf{I}\rightarrow X$ comme dans l’énoncé ; posons $B =^-\varphi^1(\mathbf{I})$ et $C =^-\varphi^1([1,+\infty [)$.

Soit $u_1$ l’application de $B\times \mathbf{I}$ dans X telle que $u_1(x, t) =\sigma (x,1-$ $(1-t)/2\varphi (x))$ si $t+ 2\varphi (x)\geqslant 1$ et $\varphi (x)>0$ et $u_1(x, t) =\sigma (x,0)$ sinon. D’après le lemme 4 ci-dessous, elle est continue.

Soit $u_2$ l’application de $B\times \mathbf{I}$ dans X telle que $u_2(x, t) =$ $\sigma (x$, sup(0$,1-2(1-t)(1-\varphi (x))))$. Elle est continue. Pour $x\in B$ tel que $\varphi (x) = 1/2$ et $t\in \mathbf{I}$, on a $u_1(x, t) =\sigma (x, t) =u_2(x, t)$. Notons $u: B\times \mathbf{I}\rightarrow X$ l’application telle que $u(x, t) =u_1(x, t)$ si $\varphi (x)\leqslant 1/2$ et $u(x, t) =u_2(x, t)$ si $1/2< x\leqslant 1$ ; elle est continue car ses restrictions aux sous-espaces fermés $^-\varphi^1([0,1/2])\times \mathbf{I}$ et $^-\varphi^1([1/2,1])\times \mathbf{I}$ de $B\times \mathbf{I}$ sont continues (TG, I, p. 19, prop. 4).

Pour $x\in X$ tel que $\varphi (x) = 1$ et $t\in \mathbf{I}$, on a $u(x, t) =u_2(x, t) =$ $\sigma (x,1) =x$. Il existe donc une unique application $\tau : X\times \mathbf{I}\rightarrow X$ qui coïncide avec $u$ dans $B\times \mathbf{I}$ et avec l’application pr$_1$ dans $C\times \mathbf{I}$; elle est continue (loc. cit.).

Soit $x\in X$ ; on vérifie que l’on a $\tau (x,1) = 1$. Si, de plus, $x\in A$, alors on a $\varphi (x) = 0$, donc $\tau (x, t) =u_1(x, t) =\sigma (x,0) =x$. Enfin, si $2\varphi (x)\leqslant 1$, alors $\varphi (x)\leqslant 1/2$, donc $\tau (x,1-2\varphi (x)) =\sigma (x,0)\in A$.

Cela prouve que l’assertion (iv) est vérifiée.

Supposons enfin l’assertion (iv) satisfaite et démontrons que le couple $(X,A)$ possède la propriété d’extension des homotopies.

Notons $C_1$ (resp. $C_2)$ l’ensemble des couples $(x, t)\in X\times \mathbf{I}$ tels que $t+\varphi (x)\leqslant 1$ (resp. $t+\varphi (x)\geqslant$ 1). Ce sont des ensembles fermés. Pour $(x, t)\in C_1$, on a $\sigma (x,1-\varphi (x))\in A$ ; soit alors $\rho_1: C_1\rightarrow$ Cyl($i$) l’application donnée par $(x, t)\mapsto \alpha_i(\sigma (x,1-\varphi (x)), t+\varphi (x))$ ; elle est continue. Soit aussi $\rho_2: C_2\rightarrow$ Cyl($i$) l’application continue donnée par $(x, t)\mapsto \beta_i(\sigma (x, t))$. Pour $(x, t)\in C_1\cap C_2$, on a $t+\varphi (x) = 1$, donc

$$
\rho_1(x, t) =\alpha_i(\sigma (x,1-\varphi (x)),1) =\beta_i(\sigma (x,1-\varphi (x)) =\rho_2(x, t)
$$

Il existe donc une unique application $\rho : X\times \mathbf{I}\rightarrow$ Cyl($i$) qui coïncide avec $\rho_1$ dans $C_1$ et avec $\rho_2$ dans $C_2$; elle est continue (TG, I, p. 19, prop. 4).

Pour $x\in A$ et $t\in \mathbf{I}$, on a $\varphi (x) = 0$, donc $t+\varphi (x)\leqslant 1$

$$
\rho (j(\alpha_i(x, t))) =\rho (x, t) =\alpha_i(\sigma (x,1), t) =\alpha_i(x, t)
$$

Pour $x\in X$, on a aussi

$$
\rho (j(\beta_i(x))) =\rho (x,1) =\beta_i(\sigma (x,1)) =\beta_i(x)
$$

Comme les images des applications $\alpha_i$ et $\beta_i$ recouvrent Cyl($i$), il en résulte que l’application $\rho$ est une rétraction continue de l’application $j$. Par suite, le couple $(X,A)$ possède la propriété d’extension des homotopies (III, p. 241, prop. 7), ce qui conclut la preuve du théorème.

#### Lemme 4 {#ta-iii-s1-lem-4 .statement tag=01W0}

Soient X et Y des espaces topologiques, soit $\varphi : X\rightarrow \mathbf{R}_+$ une application continue, posons $A =^-\varphi^1(0)$. Soit $\sigma : X\times \mathbf{I}\rightarrow Y$ une homotopie qui est fixe sur A. L’application $\sigma ': X\times \mathbf{I}\rightarrow Y$ qui applique $(x, s)$ sur $\sigma (x, s/\varphi (x))$ si $s < \varphi (x)$ et sur $\sigma (x,1)$ si $s\geqslant \varphi (x)$ est continue.

L’application $\sigma '$ est continue en tout point de la partie fermée $^-\varphi^1([1,+\infty [)\times \mathbf{I}$; il suffit donc de démontrer que sa restriction à $^-\varphi^1(\mathbf{I})\times \mathbf{I}$ est continue. On peut donc supposer que $\varphi (X)\subset \mathbf{I}$. Soient C et $C'$ les sous-espaces de $X\times \mathbf{I}$ formés des couples $(x, s)$ tels que $s\leqslant \varphi (x)$ et $s\geqslant \varphi (x)$ respectivement. Ils sont fermés et recouvrent $X\times \mathbf{I}$. L’application $\sigma '$ est continue sur $C'$; démontrons qu’elle est continue sur C.

Soit $\alpha : X\times \mathbf{I}\rightarrow X\times \mathbf{I}$ l’application continue donnée par $\alpha (x, t) =$ $(x, t\varphi (x))$. Son image est égale à C et $\sigma '\circ \alpha$ est l’application continue $\sigma$. Démontrons que $\alpha$ est une application propre. Considérons en effet un ultrafiltre $\mathfrak{U}$ sur $X\times \mathbf{I}$ et un point $(x, t)\in X\times \mathbf{I}$ qui est adhérent à la base d’ultrafiltre $\alpha (\mathfrak{U})$. Puisque pr$_1\circ \alpha =$ pr$_1$, la base d’ultrafiltre pr$_1(\mathfrak{U})$ sur X converge vers $x$. Comme $\mathbf{I}$ est compact, il existe un point $s\in \mathbf{I}$ tel que la base d’ultrafiltre pr$_2(\mathfrak{U})$ converge vers $s$. Alors $\mathfrak{U}$ converge vers $(x, s)$. Comme $\alpha$ est continue, la base d’ultrafiltre $\alpha (\mathfrak{U})$ converge vers $(x, s\varphi (x))$. Comme $\mathbf{I}$ est séparé, on a $s\varphi (x) =t$, d’où $\alpha (x, s) = (x, t)$, si bien que $\alpha$ est propre (TG, I, p. 75, th. 1). Il résulte alors de I, p. 18, exemple 2 et prop. 9 que $\sigma '|C$ est continue.

#### Corollaire 1 {#ta-iii-s1-lem-4-cor-1 .statement tag=01W1}

Soit X un espace topologique normal et soit A un sous-espace fermé de X. On suppose qu’il existe un voisinage V de A dans X et une contraction de V sur A, ainsi qu’une application continue $f: X\rightarrow \mathbf{R}$ telle que $^-f^1(0) = A$. Alors, le couple $(X,A)$ possède la propriété d’extension des homotopies.

Soit $\rho : V\times \mathbf{I}\rightarrow V$ une contraction de V sur A. Par définition d’un espace normal (TG, IX, p. 41, définition 1), il existe une application continue $g: X\rightarrow \mathbf{I}$ qui vaut 0 sur A et 1 en tout point de X - V. Soit $\varphi : X\rightarrow \mathbf{R}$ l’application donnée par $\varphi (x) =|f(x)|+g(x)$ pour $x\in X$ ; elle est continue. On a $^-\varphi^1(0) = A$ et $^-\varphi^1(\mathbf{I})\subset V$. Soit $\sigma$ l’application de $^-\varphi^1(\mathbf{I})\times \mathbf{I}$ dans X donnée par $\sigma (x, t) =\rho (x,1-t)$ pour $x\in^-\varphi^1(\mathbf{I})$ et $t\in \mathbf{I}$. Pour $x\in^-\varphi^1(\mathbf{I})$, on a $\sigma (x,1) =\rho (x,0) =x$ et $\sigma (x,0) =\rho (x,1)\in A$.

Les applications $\varphi$ et $\sigma$ vérifient les conditions de l’assertion (iii) du th. 1 de III, p. 243 ; par suite, le couple $(X,A)$ possède la propriété d’extension des homotopies.

#### Exemple 1 {#ta-iii-s1-n7-exa-1 .statement tag=01W2}

Prenons pour espace X la boule $\mathbf{B}_n$ et pour sous-espace A la sphère $\mathbf{S}_{n-1}$. Si V = X$-\{0\}$, il existe une contraction forte de V sur $\mathbf{S}_{n-1}($III, p. 237, exemple). Par suite, le couple $(\mathbf{B}_n,\mathbf{S}_{n-1})$ possède la propriété d’extension des homotopies.

#### Corollaire 2 {#ta-iii-s1-lem-4-cor-2 .statement tag=01W3}

Soient X et Y des espaces topologiques, soit A un sous-espace fermé de X, soit B un sous-espace fermé de Y. Si les couples $(X,A)$ et $(Y,B)$ possèdent la propriété d’extension des homotopies, il en est de même du couple $(X\times Y,(X\times B)\cup (A\times Y))$.

Soient $\varphi : X\rightarrow \mathbf{R}_+$ et $\sigma :^-\varphi^1(\mathbf{I})\times \mathbf{I}\rightarrow$ X, resp. $\varphi ': Y\rightarrow \mathbf{R}_+$

et $\sigma ':^-\psi^1(\mathbf{I})\times \mathbf{I}\rightarrow Y$, vérifiant les conditions de l’assertion (iv) du théorème 1 pour le couple $(X,A)$, resp. pour le couple $(Y,B)$. Soit $\psi : X\times Y\rightarrow \mathbf{R}_+$ l’application donnée par $(x, y)\mapsto$ inf($\varphi (x), \varphi '(x)$) ; elle est continue ; on a aussi $\psi (x, y) = 0$ pour tout $(x, y)\in X\times Y$ tel que $x\in A$ ou $y\in B$. Pour $(x, y, t)\in X\times Y\times \mathbf{I}$ tel que $t+\psi (x)\geqslant 1$, on a $t+\varphi (x)\geqslant 1$ et $t+\varphi '(x)\geqslant 1$. On définit ainsi une application continue

$$
\tau :\{(x, y, t)\in X\times Y\times \mathbf{I}|t+\psi (x)\geqslant 1\} \rightarrow X\times Y
$$

en posant $\tau (x, y, t) = (\sigma (x, t), \sigma '(y, t))$. Pour tout $(x, y)\in X\times Y$, on a $\tau (x, y,1) = (\sigma (x,1), \sigma '(y,1)) = (x, y)$. Si, de plus, $\psi (x, y)\leqslant 1$, alors $\varphi (x)\leqslant 1$ ou $\varphi '(y)\leqslant 1$, si bien que $\sigma (x,1)\in A$ ou $\sigma '(y,1)\in B$; cela entraîne que $\tau (x, y,1-\psi (x))$ appartient à $(A\times Y)\cup (X\times B)$. Cela vérifie l’assertion (iv) du théorème 1, d’où le corollaire.

#### Exemple 2 {#ta-iii-s1-n7-exa-2 .statement tag=01W4}

*Voici d’autres cas où le couple $(X,A)$ possède la propriété d’extension des homotopies.

(i) L’espace X est une variété différentielle paracompacte de classe $C^1$ et A une sous-variété fermée de X. Compte tenu du corollaire1, cela découle de ce que X est parfaitement normal (IX, p. 103, exerc. 11) et que A possède un voisinage tubulaire dans X ;

(ii) L’espace X est un espace cellulaire et A un sous-espace plein relativement à une décomposition cellulaire donnée de X.*

### 8. Attachement d’un espace topologique

Soient $X,B$ des espaces topologiques, soit A un sous-espace de B et soit $f: A\rightarrow X$ une application continue. Notons Y l’espace topologique somme des espaces $Y_1= X$ et $Y_2= B$ et identifions $Y_1$ et $Y_2$ à des sous-espaces de Y par les injections canoniques. Soit R la relation d’équivalence dans Y la plus fine pour laquelle les éléments $a$ de $Y_2$ et $f(a)$ de $Y_1$ sont équivalents, pour tout $a\in A$. La relation R est la relation d’égalité dans $Y_1$. Soit $x\in Y_1$ et soit $b\in Y_2$; on a $xRb$ si et seulement si $b\in A$ et $f(b) =x$. Soient $b, b'\in Y_2$; pour que l’on ait $bRb'$, il faut et il suffit que $b=b'$, ou que $b, b'\in A$ et $f(b) =f(b')$.

#### Définition 9 {#ta-iii-s1-def-9 .statement tag=01W5}

L’espace topologique quotient $Y/R$ est appelé l’espace obtenu en attachant à l’espace X l’espace B le long de l’application $f$. On le note $X\cup_fB$.

Notons $\alpha_f: X\rightarrow X\cup_fB$ et $\beta_f: B\rightarrow X\cup_fB$ les restrictions à $Y_1$ et $Y_2$ de la surjection canonique de Y sur $Y/R$. On a $\alpha_f\circ f=\beta_f|A$.

#### Remarque 1 {#ta-iii-s1-n8-rem-1 .statement tag=01W6}

L’application $\alpha_f$ est injective. Pour toute partie U

de X, on a $\alpha^{-1}_f(\alpha_f(U)) = U$ et $\beta^{-1}_f(\alpha_f(U)) =^-f^1(U)$. Si A est une partie ouverte (resp. fermée) de B, ces relations entraînent que $\alpha_f$ est une application ouverte (resp. fermée) de X dans $X\cup_fB$.

Soit U une partie ouverte de X et soit V un ouvert de B tel que $^-f^1(U) = V\cap A$. La réunion des parties U de $Y_1$ et V de $Y_2$ est un ouvert saturé de Y ; son image dans $X\cup_fB$ est donc ouverte et sa trace sur $\alpha_f(X)$ est $\alpha_f(U)$. Par suite, l’application $\alpha_f$ définit un homéomorphisme de X sur son image dans $X\cup_fB$.

#### Remarque 2 {#ta-iii-s1-n8-rem-2 .statement tag=01W7}

Soit V une partie de B. On a $\alpha^{-1}_f(\beta_f(V)) =f(V\cap A)$ et

$\beta^{-1}_f(\beta_f(V)) = V\cup^-f^1(f(V\cap A))$. Si A est fermé dans B et si l’application $f$ est fermée, l’application $\beta_f$ est donc fermée. De même, si A est ouvert dans B et si l’application $f$ est ouverte, l’application $\beta_f$ est ouverte.

Dans ces deux cas, l’application $\beta_f$ induit alors un homéomorphisme de B-A sur son image.

#### Remarque 3 {#ta-iii-s1-n8-rem-3 .statement tag=01W8}

Supposons que A soit fermé et que l’application $f$ soit propre. On vient de voir que l’application $\beta_f$ est fermée. Pour tout $x\in X$,

$\beta^{-1}_f(\alpha_f(x)) =^-f^1(x)$. C’est donc une partie quasi-compacte de A (TG,

I, p. 75, théorème 1), donc aussi de B. Pour tout $b\in B,\beta^{-1}_f(\beta_f(b))$

égale $\{b\}$ si $b\in B-A$, et $^-f^1(f(b))$ si $b\in A$ ; dans les deux cas, c’est une partie quasi-compacte de B. Les fibres de l’application $\beta_f$ sont donc quasi-compactes ; par suite (loc. cit.), l’application $\beta_f$ est propre.

L’application $\alpha_f$ est également propre (TG, I, p. 72, prop. 2). Il en résulte que l’application canonique de Y sur $X\cup_fB$ est propre.

#### Exemple 1 {#ta-iii-s1-n8-exa-1 .statement tag=01W9}

Soient X et Y des espaces topologiques et $f: X\rightarrow Y$ une application continue. Le cylindre Cyl($f$) n’est autre que l’espace obtenu en attachant à l’espace Y l’espace $X\times \mathbf{I}$ le long de l’application $f\circ$ pr$_1$ de $X\times  \{1\}$ dans Y.

#### Exemple 2 {#ta-iii-s1-n8-exa-2 .statement tag=01WA}

Soit X un espace topologique, soit B un espace topologique et soit A un sous-espace de B, soit $f: A\rightarrow X$ une application continue qui induit un homéomorphisme de A sur son image.

Posons $A'=f(A)$ ; soit $f'$ l’application de $A'$ dans B qui associe à tout $x\in A'$ l’unique antécédent de $x$ par $f$. L’application $f'\circ f$ est continue ; comme $f$ est stricte, l’application $f'$ est continue. Il existe une unique application continue $u$ de l’espace $X\cup_fB$ dans l’espace $B\cup_{f'}X$ qui applique $\alpha_f(x)$ sur $\beta_{f'}(x)$ pour $x\in X$ et $\beta_f(b)$ sur $\alpha_{f'}(b)$ pour $b\in B$; c’est un homéomorphisme qui applique le sous-espace $\alpha_f(X)$ sur le sous-espace $\beta_{f'}(X)$.

#### Proposition 8 {#ta-iii-s1-prop-8 .statement tag=01WB}

Soit Z un espace topologique.

a) Soient $u: X\rightarrow Z$ et $v: B\rightarrow Z$ des applications continues telles que $v(a) =u(f(a))$ pour tout $a\in A$. Il existe alors une unique application continue $w: X\cup_fB\rightarrow Z$ telle que $w\circ \alpha_f=u$ et $w\circ \beta_f=v$.

b) Soient $\sigma : X\times \mathbf{I}\rightarrow Z$ et $\tau : B\times \mathbf{I}\rightarrow Z$ des homotopies. On suppose que $\tau$ est fixe sur A et que $\sigma (f(a), t) =\tau (a, t)$ pour tout $a\in A$ et tout $t\in \mathbf{I}$. Il existe alors une unique homotopie $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ telle que $\eta (\alpha_f(x), t) =\sigma (x, t)$ et $\eta (\beta_f(b), t) =\tau (b, t)$ pour $x\in X,b\in B$ et $t\in \mathbf{I}$. Cette homotopie est fixe sur $\beta_f(A)$.

La proposition résulte immédiatement de la définition d’un espace quotient et de la prop. 10 (I, p. 19).

#### Corollaire 1 {#ta-iii-s1-prop-8-cor-1 .statement tag=01WC}

Soit $B'$ un espace topologique, soit $A'$ un sous-espace de $B'$ et soit $f': A'\rightarrow$ X une application continue. Soit $v: B\rightarrow B'$ une application continue telle que $v(A)\subset A'$ et $f$ = $f'\circ (v|A)$. Soit $w: X\cup_fB\rightarrow X\cup_{f'}B'$ l’unique application continue telle que $w\circ \alpha_f=\alpha_{f'}$ et $w\circ \beta_f=\beta_{f'}\circ v$. Si $v$ définit une homéotopie du couple $(B,A)$ sur le couple $(B',A')$, alors $w$ définit une homéotopie du couple $(X\cup_fB, \alpha_f(X))$ sur le couple $(X\cup_{f'}B', \alpha_{f'}(X))$.

Soit $v': B'\rightarrow B$ une application continue, soit $\tau : B\times \mathbf{I}\rightarrow B$ une homotopie fixe sur A reliant Id$_B$ à $v'\circ v$ et soit $\tau ': B'\times \mathbf{I}\rightarrow B'$ une homotopie fixe sur $A'$ reliant Id$_{B'}$ à $v\circ v'$. Pour $a'\in A'$ et $a=v'(a')$, on a les relations $a'=v(a)$ et $\beta_f(v'(a')) =\beta_f(a) =\alpha_f(f(a)) =\alpha_f(f'(a'))$. D’après la prop. 8, a), il existe une unique application $w': X\cup_{f'}B'\rightarrow$ $X\cup_fB$ telle que $w'\circ \alpha_{f'}=\alpha_{f'}$ et $w'\circ \beta_{f'}=\beta_f\circ v'$. D’après la prop. 8, b), il existe une unique homotopie $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow X\cup_{f'}B'$ telle que $\eta (\alpha_f(x), t) =\alpha_{f'}(x)$ et $\eta (\beta_f(b), t) =\beta_{f'}(\tau (b, t))$ pour $x\in X,b\in B$ et $t\in \mathbf{I}$. Il existe de même une unique homotopie $\eta ': (X\cup_{f'}B')\times \mathbf{I}\rightarrow$ $X\cup_fB$ telle que $\eta '(\alpha_{f'}(x), t) =\alpha_f(x)$ et $\eta '(\beta_{f'}(b), t) =\beta_f(\tau '(b, t))$ pour $x\in X,b\in B'$ et $t\in \mathbf{I}$. L’application de $(X\cup_fB)\times \mathbf{I}$ dans $X\cup_fB$ donnée par $(x, t)\mapsto \eta '(\eta (x, t), t)$ est alors une homotopie fixe sur $\alpha_f(X)$ reliant l’application identique de $X\cup_fB$ à l’application $w'\circ w$. De même, l’application de $(X\cup_{f'}B')\times \mathbf{I}$ dans $X\cup_{f'}B'$ donnée par $(x, t)\mapsto \eta (\eta '(x, t), t)$ est une homotopie fixe sur $\alpha_{f'}(X)$ reliant l’application identique de $X\cup_{f'}B'$ à l’application $w\circ w'$. Le corollaire en résulte.

#### Exemple 3 {#ta-iii-s1-n8-exa-3 .statement tag=01WD}

Notons $i$ l’injection canonique de A dans B et prenons pour espace $B'$ le cylindre de l’application $i$; notons $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) et $\beta_i: B\rightarrow$ Cyl($i$) les applications canoniques et $r_i:$ Cyl($i$)$\rightarrow B$ la rétraction canonique du cylindre Cyl($i$) sur sa base. Soit $A_0$ le sous-espace $\alpha_i(A\times  \{0\})$ de Cyl($i$) et notons $f_0: A_0\rightarrow X$ l’application $f\circ r_i$. Pour $a\in A$, on a

$$
\beta_f\circ r_i(\alpha_i(a,0)) =\beta_f(a) =\alpha_f(f_0(\alpha_i(a,0))) =\alpha_f(f(a))
$$

Soit $\eta : X\cup_{f_0}$ Cyl($i$)$\rightarrow X\cup_fB$ l’unique application continue telle que $\eta \circ \alpha_{f_0}=\alpha_f$ et $\eta \circ \beta_{f_0}=\beta_f\circ r_i$. Supposons que le couple $(B,A)$ possède la propriété d’extension des homotopies. Alors, l’application $r_i$ définit une homéotopie du couple (Cyl($i$)$,A_0)$ sur le couple $(B,A)$ (III, p. 243, th. 1). D’après le corollaire 1, l’application $\eta$ définit alors une homéotopie du couple $(X\cup_{f'}B', \alpha_{f'}(X))$ sur le couple $(X\cup_fB, \alpha_f(X))$. En particulier, $\eta$ est une homéotopie.

#### Corollaire 2 {#ta-iii-s1-prop-8-cor-2 .statement tag=01WE}

Soit $X'$ un espace topologique, soit $u: X\rightarrow X'$ une application continue, posons $f'=u\circ f$. Soit $w: X\cup_fB\rightarrow X'\cup_{f'}B$ l’unique application continue telle que $w\circ \alpha_f=\alpha_{f'}\circ u$ et $w\circ \beta_f=\beta_{f'}$. Si $u$ définit une homéotopie du couple $(X, f(A))$ sur le couple $(X', f'(A))$, alors $w$ définit une homéotopie du couple $(X\cup_fB, \beta_f(B))$ sur le couple $(X'\cup_{f'}B, \beta_{f'}(B))$.

La démonstration est analogue à celle du corollaire 1.

#### Proposition 9 {#ta-iii-s1-prop-9 .statement tag=01WF}

Soient X et B des espaces topologiques, soit A un sous-espace de B et soit $f: A\rightarrow X$ une application continue.

a) Si le couple $(B,A)$ possède la propriété d’extension des homotopies, il en est de même du couple $(X\cup_fB, \alpha_f(X))$.

b) Supposons que l’application $f$ soit injective et stricte. Si le couple $(X, f(A))$ possède la propriété d’extension des homotopies, il en est de même du couple $(X\cup_fB, \beta_f(B))$.

a) Supposons que le couple $(B,A)$ possède la propriété d’extension des homotopies. Soit Z un espace topologique, soit $u: X\cup_fB\rightarrow Z$ une application continue et soit $\sigma :\alpha_f(X)\times \mathbf{I}\rightarrow Z$ une homotopie dont le terme est la restriction de $u$ au sous-espace $\alpha_f(X)$.

Posons $v_1=u\circ \alpha_f$ et notons $\tau_1: X\times \mathbf{I}\rightarrow Z$ l’application donnée par $(x, t)\mapsto \sigma (\alpha_f(x), t)$. Posons $v_2=u\circ \beta_f$. Comme $\beta_f|A =\alpha_f\circ f$, l’application de $A\times \mathbf{I}$ dans Z qui applique $(a, t)$ sur $\sigma (\alpha_f(f(a)), t)$ pour $a\in A$ et $t\in \mathbf{I}$ est une homotopie dont le terme est égal à l’application $v_2|A$. Puisque le couple $(B,A)$ possède la propriété d’extension des homotopies, il existe une homotopie $\tau_2: B\times \mathbf{I}\rightarrow Z$ dont le terme est l’application $v_2$ et telle que $\tau_2(a, t) =\sigma (\alpha_f(f(a)), t)$ pour $(a, t)\in A\times \mathbf{I}$.

Pour $a\in A$ et $t\in \mathbf{I}$, on a $\tau_2(a, t) =\tau_1(f(a), t)$. D’après la proposition 8, il existe une unique application continue $\sigma : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ telle que $\sigma (\alpha_f(x), t) =\sigma_1(x, t)$ et $\sigma (\beta_f(b), t) =\sigma_2(b, t)$, pour $x\in X$, $b\in B$ et $t\in \mathbf{I}$. C’est une homotopie de terme $u$ qui prolonge $\tau$, d’où l’assertion a).

b) Compte tenu de l’exemple 2 (III, p. 249), l’assertion b) résulte de l’assertion a).

### 9. Espace obtenu par contraction d’un sous-espace

Soit X un espace topologique et soit A une partie de X. Considérons la relation d’équivalence R dans X la plus fine pour laquelle tous les éléments de A sont équivalents : deux éléments de X sont équivalents suivant cette relation s’ils sont égaux ou s’ils appartiennent tous deux à A.

#### Définition 10 {#ta-iii-s1-def-10 .statement tag=01WG}

L’espace quotient de X par R se note $X/A$ et s’appelle l’espace obtenu à partir de X par contraction du sous-ensemble A.

Notons $\rho : X\rightarrow X/A$ la surjection canonique. Soit Y un espace topologique et soit $f: X\rightarrow Y$ une application continue. Pour qu’il existe une application continue $g: X/A\rightarrow Y$ telle que $g\circ \rho =f$, il faut et il suffit que $f$ soit constante sur A.

Si l’ensemble A est fermé (resp. ouvert) dans X, l’application $\rho$ est fermée (resp. ouverte) et induit un homéomorphisme de X-A sur son image. Si A est une partie fermée et quasi-compacte de X, l’application $\rho$ est propre (TG, I, p. 75, th. 1).

Si l’ensemble A est vide, $\rho$ est un homéomorphisme. S’il n’est pas vide, A est un point de $X/A$ que l’on appelle le point-base de $X/A$ et que l’on note $s_{X/A}$. L’espace $X/A$ s’identifie alors à l’espace obtenu en attachant à l’espace $\{s_{X/A}\}$ l’espace X au moyen de l’unique application de A dans $\{s_{X/A}\}$.

#### Proposition 10 {#ta-iii-s1-prop-10 .statement tag=01WH}

Soit X un espace topologique et soit A une partie de $x$. Supposons qu’il existe une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ d’origine Id$_X$, constante sur $A\times  \{1\}$ et telle que $\sigma (A\times \mathbf{I})\subset A$. Alors, l’application canonique $\rho$ de X dans $X/A$ est une homéotopie.

Notons $f$ le terme de $\sigma$. C’est une application continue de X dans X, homotope à Id$_X$. Elle est constante sur A ; il existe donc une unique application continue $g: X/A\rightarrow X$ telle que $g\circ \rho =f$. D’autre part, comme $\sigma (A\times \mathbf{I})\subset A$, il existe une application $\sigma '$ de $X/A\times \mathbf{I}$ dans $X/A$ telle que $\sigma '(\rho (x), t) =\rho (\sigma (x, t))$ pour tout $x\in X$ et tout $t\in \mathbf{I}$. D’après I, p. 19, prop. 10, l’application $\sigma '$ est continue. C’est une homotopie reliant l’application identique de $X/A$ à l’application $\rho \circ g$. Par suite, les applications $g$ et $\rho$ sont des homéotopies réciproques l’une de l’autre à homotopie près.

#### Remarque {#ta-iii-s1-n9-rem-1 .statement tag=01WI}

Soit X un espace topologique et soit A une partie de X.

1) Si l’application canonique de X sur $X/A$ est une homéotopie, il existe une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ d’origine Id$_X$ qui est constante sur $A\times  \{1\}$. Mais il se peut qu’il n’en existe aucune satisfaisant en outre à la condition $\sigma (A\times \mathbf{I})\subset A$ (III, p. 322, exerc. 4).

2) Il peut exister une homotopie reliant l’application identique de X à une application de X dans X qui est constante sur A sans que les espaces X et $X/A$ soient homéotopes (III, p. 325, exerc. 14).

3) Supposons que A soit contractile. Si le couple $(X,A)$ possède la propriété d’extension des homotopies, l’application canonique de X sur $X/A$ est une homéotopie. Soit en effet $\sigma : A\times \mathbf{I}\rightarrow A$ une homotopie dont l’origine est l’application identique de A et dont le terme est une application constante. Il existe alors une homotopie $\sigma '$ d’origine Id$_X$ qui étend $\sigma$. L’assertion résulte ainsi de la proposition 10.

4) Soient X et Y des espaces topologiques, soit A un sous-espace non vide de X et soit B un sous-espace de Y. Soit $f: X\rightarrow Y$ une application continue telle que $f(A)\subset B$. Notons $\varphi : X/A\rightarrow Y/B$ l’application continue déduite de $f$ par passage aux quotients. Si $f$ définit une homéotopie du couple $(X,A)$ sur le couple $(Y,B)$, l’application $\varphi$ est une homéotopie du couple $(X/A, s_{X/A})$ sur le couple $(Y/B, s_{Y/B})$. Soit P un espace topologique réduit à un point, soient $\alpha$ et $\beta$ les applications constantes de A et B dans P. Observons que l’application $\varphi$ s’identifie à l’application de $P\cup_{\alpha}X$ dans $P\cup_{\beta}Y$ déduite de $f$ et de l’application identique de P. L’assertion découle alors du corollaire 1 de III, p. 249.

### 10. Cône d’une application

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. Soit Cyl($f$) le cylindre de l’application $f$. Notons $\alpha_f$ l’application canonique de $X\times \mathbf{I}$ dans Cyl($f$) et $f_0$ l’application $x\mapsto \alpha_f(x,0)$ de X dans Cyl($f$) ; ces applications induisent des homéo-morphismes de $X\times \mathbf{I}$ et X respectivement sur leurs images dans Cyl($f$).

#### Définition 11 {#ta-iii-s1-def-11 .statement tag=01WJ}

On appelle cône de l’application $f$ et on note Côn$(f)$ l’espace topologique déduit de Cyl($f$) par contraction de $f_0(X)$.

Notons $\beta_f': Y\rightarrow$ Côn$(f)$ la composition de l’application canonique $\beta_f: Y\rightarrow$ Cyl($f$) et de la surjection canonique de Cyl($f$) sur Côn$(f)$. L’application $\beta_f'$ est continue et définit un homéomorphisme de Y sur une partie fermée de Côn$(f)$, appelée base du cône, et que nous identifierons ainsi à Y.

Notons $\alpha '_f: X\times \mathbf{I}\rightarrow$ Côn$(f)$ la composition de l’application $\alpha_f$ et de la surjection canonique de Cyl($f$) sur Côn$(f)$. L’application $\alpha '_f$ est une homotopie dont l’origine est une application constante et dont le terme est l’application $\beta_f'\circ f$.

Si X est vide, l’application $\beta_f'$ est un homéomorphisme de Y sur Côn$(f)$.

Supposons que X ne soit pas vide. Notons alors $s$ le point-base de l’espace Cyl($f$)$/f_0(X)$; on dit que c’est le sommet du cône Côn$(f)$. Comme $f_0(X)$ est fermé dans Cyl($f$), l’application canonique $\pi :$ Cyl($f$)$\rightarrow$ Côn$(f)$ induit un homéomorphisme de Cyl($f$)$-f_0(X)$ sur Côn$(f)-\{s\}($III, p. 252). Le sommet du cône Côn$(f)$ n’appartient pas à sa base ; l’injection canonique de Y dans Côn$(f)-\{s\}$ est une homéotopie (III, p. 239, prop. 6).

Soit $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) la contraction canonique du cylindre de $f$ sur sa base. Pour $c\in$ Cyl($f$)$-f_0(X)$ et $t\in \mathbf{I}$, on a $\sigma_f(c, t)\notin f_0(X)$. Par suite, il existe une unique application $\sigma '_f: ($Côn$(f)-\{s\})\times \mathbf{I}\rightarrow$ Côn$(f)-\{s\}$ telle que $\sigma '_f(\pi (c), t) =\pi (\sigma_f(c, t))$ pour $c\in$ Cyl($f$)$-f_0(X)$ et $t\in \mathbf{I}$. Elle est continue et c’est une contraction forte de Côn$(f)-\{s\}$ sur Y. On dit que c’est la contraction canonique de Côn$(f)-\{s\}$ sur sa base. Son terme est une rétraction de Côn$(f)-\{s\}$ sur Y qu’on appelle la rétraction canonique du cône privé de son sommet sur sa base.

Proposition 11 (Propriété universelle des cônes)

Soit Z un espace topologique, soit $\beta : Y\rightarrow Z$ une application continue et soit $\alpha : X\times \mathbf{I}\rightarrow Z$ une homotopie dont l’origine est une application constante et dont le terme est égal à $\beta \circ f$. Il existe une unique application continue $\varphi$ de Côn$(f)$ dans Z telle que $\alpha =\varphi \circ \alpha '_f$ et $\beta =\varphi \circ \beta_f'$.

D’après la propriété universelle des cylindres (III, p. 238, prop. 4), il existe une unique application continue $h:$ Cyl($f$)$\rightarrow$ Z telle que $\alpha =h\circ \alpha_f$ et $\beta =h\circ \beta_f$. Comme l’origine de $\alpha$ est une application constante, la restriction de $h$ au sous-espace $\alpha_f(X\times \{0\})$ est constante. Il existe donc une unique application continue $\varphi :$ Côn$(f)\rightarrow Z$ telle que $h=\varphi \circ \pi$, où $\pi$ désigne la surjection canonique de Cyl($f$) sur Côn$(f)$. L’application $\varphi$ vérifie $\alpha =\varphi \circ \alpha '_f$ et $\beta =\varphi \circ \beta_f'$ et c’est la seule ayant ces propriétés, car les images de $\alpha '_f$ et $\beta '_f$ recouvrent Côn$(f)$.

#### Exemple 1 {#ta-iii-s1-n10-exa-1 .statement tag=01WK}

Soit X un espace topologique. On note C(X), et on appelle cône de l’espace X, le cône de l’application Id$_X$; c’est l’espace déduit de $X\times \mathbf{I}$ par contraction de $X\times  \{0\}$. Soit $\pi$ l’application canonique de $X\times \mathbf{I}$ dans C(X) ; l’image $C'(X)$ de $X\times [0,1[$ par $\pi$ est appelé le cône ouvert de l’espace X.

Supposons que X n’est pas vide. Alors, le cône C(X) n’est pas vide et son point-base est encore appelé le sommet du cône.

L’application $((x, t), u)\mapsto (x, t(1-u))$ de $(X\times \mathbf{I})\times \mathbf{I}$ dans $X\times \mathbf{I}$ est une homotopie reliant l’application identique de $X\times \mathbf{I}$ à l’application $(x, t)\mapsto (x,0)$. On en déduit, par passage aux ensembles quotients, une application $\sigma : C(X)\times \mathbf{I}\rightarrow C(X)$ telle que $\sigma (\pi (x, t), u) =\pi (x, t(1-u))$ pour $x\in X,t, u\in \mathbf{I}$. L’application $\sigma$ est continue d’après I, p. 19, prop. 10. L’application $\sigma$ est alors une homotopie pointée en $s$ reliant l’application identique de C(X) à l’application constante d’image $\{s\}$. Par suite, le cône C(X) est contractile en son sommet $s$. Comme $\sigma (C'(X)\times \mathbf{I})$ est contenu dans $C'(X)$, l’application $\sigma$ définit, par passage aux sous-espaces, une homotopie pointée en $s$ reliant l’application identique de $C'(X)$ à l’application constante d’image $\{s\}$; le cône ouvert $C'(X)$ est donc contractile en $s$.

#### Remarque 1 {#ta-iii-s1-n10-rem-1 .statement tag=01WL}

Soit X un espace topologique et soit A un sous-espace de X ; notons $i$ l’injection canonique de A dans X. La rétraction canonique $r_i$ du cylindre Cyl($i$) sur sa base applique le sous-espace $\alpha_i(A\times  \{0\})$ dans A. Soit $\rho :$ Côn$(i)\rightarrow X/A$ l’application continue qui s’en déduit par passage aux quotients. Supposons que le couple $(X,A)$ possède la propriété d’extension des homotopies. D’après III, p. 243, théorème 1, l’application $r_i$ définit une homéotopie du couple (Cyl($i$)$, \alpha_i(A\times  \{0\}))$ sur le couple $(X,A)$. D’après la remarque 4 de III, p. 253, l’application $\rho$ est alors une homéotopie du couple (Côn$(i), s)$ sur le couple $(X, s_{X/A})$. C’est en particulier une homéotopie.

#### Remarque 2 {#ta-iii-s1-n10-rem-2 .statement tag=01WM}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. L’application canonique $\alpha '_f: X\times \mathbf{I}\rightarrow$ Côn$(f)$ est constante sur $X\times  \{0\}$ donc définit une application continue $\gamma_f: C(X)\rightarrow$ Côn$(f)$. La restriction à $C'(X)$ de l’application $\gamma_f$ est injective et stricte et définit par passage aux sous-espaces un homéomorphisme du cône ouvert $C'(X)$ sur le complémentaire de Y dans Côn$(f)$.

Identifions la base du cône C(X) à l’espace X et notons $u$ l’application continue de $Y\cup_fC(X)$ dans Côn$(f)$ déduite des applications $\beta '_f: Y\rightarrow$ Côn$(f)$ et $\gamma_f: C(X)\rightarrow$ Côn$(f)$. Inversement, soit $v:$ Côn$(f)\rightarrow Y\cup_fC(X)$ l’unique application continue telle que $v\circ \alpha '_f$ soit l’application canonique de $X\times \mathbf{I}$ sur C(X) et $v\circ \beta_f'$ soit l’application canonique de Y sur $Y\cup_fC(X)$. Les applications $u$ et $v$ sont des homéomorphismes réciproques l’un de l’autre.
