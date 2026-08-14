---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 2
section_title: Applications étales
lang: fr
source: ta-i-iv-fr
book_pages: A I.25-A I.42
pdf_pages: 0041-0058
extraction: native
subsections:
    - "no": 1
      title: Applications séparées
      page: 25
      pdf_page: 41
    - "no": 2
      title: Applications étales
      page: 28
      pdf_page: 44
    - "no": 3
      title: Sections locales des applications étales
      page: 32
      pdf_page: 48
    - "no": 4
      title: Relèvements continus des applications étales
      page: 33
      pdf_page: 49
    - "no": 5
      title: Construction de sections continues d’applications étales
      page: 35
      pdf_page: 51
    - "no": 6
      title: Majoration du cardinal des fibres d’une application étale et séparée
      page: 40
      pdf_page: 56
statements: 47
exercises: 0
content_sha256: 5cfdec0eb7df3953fa42f07be84325ebb574c1c81149dc28afde0318feaeb974
---

## § 2. APPLICATIONS ÉTALES

### 1. Applications séparées

#### Proposition 1 {#ta-i-s2-prop-1 .statement tag=01MH}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une application continue. Les propriétés suivantes sont équivalentes :

(i) La diagonale $\Delta_X$ du produit fibré $X\times_YX$ est un sous-espace fermé ;

(ii) Pour tout espace topologique W et tout couple d’applications continues $(g_1, g_2)$ de W dans X tel que $f\circ g_1=f\circ g_2$, l’ensemble des points $w\in W$ tels que $g_1(w) =g_2(w)$ est fermé dans W ;

(iii) Pour tout couple $(x_1, x_2)$ de points de X tel que $x_1=\not x_2$ et $f(x_1) =f(x_2)$, il existe un voisinage $V_1$ de $x_1$ dans X et un voisinage $V_2$ de $x_2$ dans X tels que $V_1\cap V_2=\emptyset$.

(i)$\Rightarrow$(ii) : Soient $g_1,g_2$ des applications continues de W dans X telles que $f\circ g_1=f\circ g_2$, et $g: W\rightarrow X\times_YX$ l’application déduite de $g_1$ et $g_2$. L’ensemble des points $w\in W$ tels que $g_1(w) =g_2(w)$ est $\overset{-1}{g}(\Delta_X)$. Puisque $g$ est continue, il est donc fermé si la diagonale $\Delta_X$ est fermée.

(ii)$\Rightarrow$(i) : La diagonale $\Delta_X$ est l’ensemble des points $z\in X\times_YX$ tels que pr$_1(z) =$ pr$_2(z)$. Il résulte de (ii) appliqué à $W = X\times_YX$ et au couple d’applications (pr$_1$, pr$_2)$ que la diagonale $\Delta_X$ est fermée dans $X\times_YX$.

(i)$\Leftrightarrow$(iii) : Soit $(x_1, x_2)$ un point de $X\times_YX$ et soient $V_1$ et $V_2$ des voisinages de $x_1$ et $x_2$ respectivement. La condition $V_1\cap V_2=\emptyset$ équivaut à la condition $(V_1\times V_2)\cap \Delta_X=\emptyset$, c’est-à-dire à $(V_1\times V_2)\cap$ $(X\times_YX)\cap \Delta_X=\emptyset$. Puisque les ensembles $(V_1\times V_2)\cap (X\times_YX)$ forment une base de voisinages de $(x_1, x_2)$ dans $X\times_YX$, cela prouve l’équivalence de (i) et (iii).

#### Définition 1 {#ta-i-s2-def-1 .statement tag=01MI}

Soient X et Y des espaces topologiques. On dit qu’une application continue $f: X\rightarrow Y$ est séparée si elle satisfait aux conditions équivalentes de la proposition 1.

#### Proposition 2 {#ta-i-s2-prop-2 .statement tag=01MJ}

Soient X, Y, Z des espaces topologiques et soient $f: X\rightarrow Y$ et $g: Y\rightarrow Z$ des applications continues.

a) Si $f$ et $g$ sont séparées, alors $g\circ f$ est séparée.

b) Si $g\circ f$ est séparée, alors $f$ est séparée.

c) Supposons de plus que l’application $f$ soit propre et surjective. Alors, si $g\circ f$ est séparée, $g$ est séparée.

Considérons, dans $X\times X$, les sous-espaces $\Delta_X$ (diagonale), $X\times_YX$ et $X\times_ZX$. Ce sont respectivement les ensembles des points $u$ de $X\times X$ tels que pr$_1(u) =$ pr$_2(u),f\circ$pr$_1(u) =f\circ$pr$_2(u),g\circ f\circ$pr$_1(u) =g\circ f\circ$pr$_2(u)$. Si $g\circ f$ est séparée, $\Delta_X$ est fermé dans $X\times_ZX$, donc aussi dans $X\times_YX$, d’où b).

D’après la prop. 1, (ii), appliquée à $W = X\times_ZX,g_1=f\circ$ pr$_1$ et $g_2=f\circ$ pr$_2,X\times_YX$ est fermé dans $X\times_ZX$ si $g$ est séparée. Si de plus $f$ est séparée, $\Delta_X$ est fermé dans $X\times_YX$ (prop. 1, (i)), donc dans $X\times_ZX$, d’où a).

Démontrons enfin c). L’application $(f, f): X\times X\rightarrow Y\times Y$ est propre (TG, I, p. 73, prop. 4). Le sous-espace $X\times_ZX$ est l’image réciproque de $Y\times_ZY$ par $(f, f)$ ; d’après TG, I, p. 72, prop. 3, l’application $u: X\times_Z$ $X\rightarrow Y\times_ZY$ déduite de $(f, f)$ est propre. Comme $g\circ f$ est séparée, la diagonale $\Delta_X$ est fermée dans $X\times_ZX$. Par suite, $u(\Delta_X)$ est fermé dans $Y\times_ZY$. Comme $f$ est surjective, $u(\Delta_X)$ est la diagonale de $Y\times_ZY$. Cela montre que $g$ est séparée.

#### Remarque 1 {#ta-i-s2-n1-rem-1 .statement tag=01MK}

Une application continue injective est séparée.

#### Remarque 2 {#ta-i-s2-n1-rem-2 .statement tag=01ML}

Pour qu’un espace topologique X soit séparé (TG, I, p. 52, déf. 1), il faut et il suffit que l’application de X dans un espace réduit à un point soit séparée. Dans ce cas, toute application continue de X dans un espace topologique est séparée (prop. 1, (iii)).

Soit $f: X\rightarrow$ Y une application continue et séparée. Pour tout point $y$ de Y, la fibre $\overset{-1}{f}(y)$ est un espace topologique séparé (loc. cit.). Il existe toutefois des applications continues qui ne sont pas séparées mais dont toutes les fibres sont des espaces topologiques séparés (I, p. 140, exerc. 1).

#### Remarque 3 {#ta-i-s2-n1-rem-3 .statement tag=01MM}

Soit $f: X\rightarrow Y$ une application continue et séparée. Si l’espace Y est séparé, l’espace X est séparé. Cela résulte de la remarque 2 et de la proposition 2 appliquée avec un espace Z réduit à un point.

#### Remarque 4 {#ta-i-s2-n1-rem-4 .statement tag=01MN}

Soient $f: X\rightarrow Y$ une application continue et séparée, $y$ un point

de Y et A une partie finie de $\overset{-1}{f}(y)$. Démontrons qu’il existe une famille $(V_a)_{a\in A}$ d’ensembles deux à deux disjoints telle que pour chaque $a\in A$, l’ensemble $V_a$ soit un voisinage de $a$ dans X. Pour cela, pour chaque partie $\{a, b\}$ de A à deux éléments, choisissons un voisinage $V_{(a,b)}$ de $a$ et un voisinage $V_{(b,a)}$ de $b$ dans X tels que $V_{(a,b)}\cap V_{(b,a)}=\emptyset$ (prop. 1, (iii)). Notons $V_a$ l’intersection de la famille formée par X et les ensembles $V_{(a,b)}$ pour $b\in A,b=\not a$. L’ensemble $V_a$ est un voisinage de $a$ dans X, et si $a,b$ sont deux éléments distincts de A, l’ensemble $V_a\cap V_b$ est contenu dans $V_{(a,b)}\cap V_{(b,a)}$, donc est vide.

#### Remarque 5 {#ta-i-s2-n1-rem-5 .statement tag=01MO}

Soit Y un espace topologique. Soit $(A_i)_{i\in I}$ une famille de parties de Y et soit X l’espace somme de la famille $(A_i)_{i\in I}$. L’application canonique de X dans Y est séparée.

#### Proposition 3 {#ta-i-s2-prop-3 .statement tag=01MP}

Soit $f: X\rightarrow Y$ une application continue et séparée. Toute section continue de $f$ induit un homéomorphisme de Y sur une partie fermée de X.

Soit $s: Y\rightarrow X$ une section continue de $f$. L’application $s$ induit un homéomorphisme de Y sur le sous-espace $s(Y)$ de X (TG, I, p. 22, prop. 9). L’application identique de X et l’application $s\circ f$ sont continues et l’on a $f\circ$ Id$_X=f\circ (s\circ f)$. Puisque l’application $f$ est séparée, l’ensemble $s(Y)$, qui est l’ensemble des points $x$ de X tels que $x=s\circ f(x)$, est fermé dans X (prop. 1, (ii)).

#### Proposition 4 {#ta-i-s2-prop-4 .statement tag=01MQ}

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien. Si l’application $p$ est séparée, il en est de même de $p'$. Inversement, si $p'$ est séparée et si $f$ est universellement stricte et surjective, alors $p$ est séparée.

Considérons le carré

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

$q'q$

${B'}^f$ B

où l’application $\varphi$ est induite par l’application $f'\times f': X'\times X'\rightarrow X\times X$. Rappelons (I, p. 13, exemple 1) que ce carré est cartésien et que l’on a $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$.

Si l’application $p$ est séparée, l’ensemble $\Delta_X$ est fermé dans $X\times_BX$ ; par suite, $\Delta_{X'}$ est une partie fermée de $X'\times_{B'}X'$, ce qui prouve que l’application $p'$ est séparée.

Si l’application $f$ est surjective, l’application $\varphi$ est surjective (I, p. 10, cor.) ; si $f$ est universellement stricte, $\varphi$ est stricte (I, p. 20, déf. 6). Supposons l’application $p'$ séparée. Alors, $\Delta_{X'}$ est fermé dans $X'\times_{B'}X'$. Comme $\Delta_{X'}=\overset{-1}{\varphi}(\Delta_X)$ et comme $\varphi$ est surjective et stricte, $\Delta_X$ est fermé dans $X\times_BX$, ce qui prouve que l’application $p$ est séparée.

#### Proposition 5 {#ta-i-s2-prop-5 .statement tag=01MR}

Soient X, Y, Z des espaces topologiques et soient $f: X\rightarrow Y,g: Y\rightarrow Z$ des applications continues. Supposons l’application $g$ séparée et l’application $g\circ f$ propre. L’application $f$ est alors propre.

Considérons le carré cartésien suivant :

$X\times_ZY^{pr_2}$ Y

pr$_1g$

X $^{g\circ f}Z$.

Soit $s: X\rightarrow X\times_ZY$ l’application $x\mapsto (x, f(x))$. C’est une section continue de pr$_1: X\times_ZY\rightarrow X$. D’après la prop. 4, l’application pr$_1$ est séparée ; il en résulte que l’application $s$ est propre (I, p. 27, prop. 3 et TG, I, p. 72, prop. 2). D’autre part, l’application pr$_2$ est propre (I, p. 17, prop. 8). Donc l’application $f$, qui est égale à pr$_2\circ s$, est propre (TG, I, p. 73, prop. 5).

### 2. Applications étales

#### Définition 2 {#ta-i-s2-def-2 .statement tag=01MS}

Soient E et B des espaces topologiques, soit $p: E\rightarrow B$ une application et soit $x$ un point de E. On dit que l’application $p$ est topologiquement étale en $x$ s’il existe un voisinage U de $x$ dans E et un voisinage V de $p(x)$ dans B tels que $p$ induise un homéomorphisme de U sur V.

On dit que l’application $p$ est topologiquement étale si elle est topologiquement étale en tout point $x$ de E.

Lorsqu’il n’y a pas de confusion possible, cf. l’exemple 3, ci-dessous, on dira étale au lieu de topologiquement étale. Au lieu de dire que $p: E\rightarrow B$ est une application étale, on dit aussi que le B-espace $(E, p)$ est un B-espace étalé, ou simplement que E est un espace étalé sur B, lorsqu’aucun doute n’est possible quant à l’application $p$.

#### Remarque 1 {#ta-i-s2-n2-rem-1 .statement tag=01MT}

L’ensemble des points de E en lesquels une application $p: E\rightarrow B$ est étale est un ouvert U de E et la restriction de $p$ à U est une application étale de U dans B.

#### Remarque 2 {#ta-i-s2-n2-rem-2 .statement tag=01MU}

Une application étale est continue et ouverte (TG, I, p. 33, prop. 5) ; en particulier, l’image d’une application étale est ouverte. Inversement, si $p: E\rightarrow B$ est une application continue et ouverte, et si tout point $x$ de E possède un voisinage V tel que l’application $p|V$ soit injective, l’application $p$ est étale. Les fibres d’une application étale sont discrètes.

#### Exemple 1 {#ta-i-s2-n2-exa-1 .statement tag=01MV}

Soient B un espace topologique et $(U_i)_{i\in I}$ une famille de parties de B. Notons E l’espace somme de la famille $(U_i)_{i\in I}$ et $p: E\rightarrow B$ l’application déduite des injections canoniques des $U_i$ dans B. Pour que l’application $p$ soit étale, il faut et il suffit que les $U_i,i\in I$, soient tous ouverts.

#### Exemple 2 {#ta-i-s2-n2-exa-2 .statement tag=01MW}

Soit U un ouvert de $\mathbf{C}$. Pour qu’une fonction holomorphe $f: U\rightarrow \mathbf{C}$ soit une application étale, il faut et il suffit que sa dérivée ne s’annule pas.

#### Exemple 3 {#ta-i-s2-n2-exa-3 .statement tag=01MX}

Un morphisme étale de variétés (VAR, R, 5.7.8) est une application topologiquement étale, mais il existe des morphismes de variétés réelles qui sont topologiquement étales et qui ne sont pas des morphismes étales. C’est le cas par exemple de l’application $x\mapsto x^3$ de $\mathbf{R}$ dans $\mathbf{R}$. Cependant, un morphisme de variétés analytiques complexes qui est topologiquement étale est un morphisme étale (I, p. 141, exerc. 6).

#### Proposition 6 {#ta-i-s2-prop-6 .statement tag=01MY}

Soient X, Y, Z des espaces topologiques et soient $f: X\rightarrow Y,g: Y\rightarrow Z$ des applications.

a) Supposons que $f$ et $g$ sont étales ; alors $g\circ f$ est étale.

b) Supposons que $g$ est étale, $f$ est continue et $g\circ f$ est ouverte. Alors $f$ est ouverte.

c) Supposons que $g\circ f$ et $g$ sont étales et que $f$ est continue. L’application $f$ est alors étale.

d) Supposons que $g\circ f$ est étale et que l’application $f$ est continue et ouverte ; alors, $f$ est étale et $g$ est étale en tout point de $f(X)$.

Démontrons a). Supposons les applications $f$ et $g$ étales. Elles sont alors continues et ouvertes, donc l’application $g\circ f$ est continue et ouverte. Soit $x$ un point de X. Il existe un voisinage W de $f(x)$ dans Y tel que l’application $g|W$ soit injective, et un voisinage V de $x$

dans X, contenu dans $\overset{-1}{f}(W)$, tel que l’application $f|V$ soit injective ; l’application $(g\circ f)|V$ est alors injective. Cela prouve que l’application $g\circ f$ est étale (remarque 2).

Démontrons b). Soient $x$ un point de X et W un voisinage ouvert de $f(x)$ tel que $g$ induise un homéomorphisme de W sur l’ouvert $g(W)$. Soit V un voisinage de $x$ tel que $f(V)$ soit contenu dans W; alors, $g\circ f(V)$ est un voisinage de $g\circ f(x)$, donc $f(V)$ est un voisinage de $f(x)$ dans l’ouvert W, et aussi dans Y. Ceci prouve que l’application $f$ est ouverte (TG, I, p. 33, prop. 5).

Démontrons c). D’après b$),f$ est ouverte. Soit $x$ un point de X. Comme $g\circ f$ est étale, il existe un voisinage V de $x$ dans X tel que $g\circ f|V$ soit injective. Ainsi, $f|V$ est injective et $f$ est étale (I, p. 29, remarque 2).

Démontrons d). Soit $x$ un point de X et posons $y=f(x)$. Il existe un voisinage ouvert V de $x$ tel que $g\circ f$ induise un homéomorphisme de V sur l’ouvert $g\circ f(V)$. Comme l’application $f$ est ouverte, $f(V)$ est un voisinage ouvert de $y$. L’application $f|V: V\rightarrow f(V)$ déduite de $f$ par passage aux sous-espaces est continue, ouverte et bijective ; c’est donc un homéomorphisme, si bien que $f$ est étale en $x$. De plus, l’application $g$ induit un homéomorphisme de $f(V)$ sur $g\circ f(V)$, donc est étale en $y$.

#### Corollaire 1 {#ta-i-s2-prop-6-cor-1 .statement tag=01MZ}

Soit B un espace topologique. Un B-morphisme d’un B-espace étalé dans un autre est étale.

Cela découle de l’assertion c) de la prop. 6.

#### Corollaire 2 {#ta-i-s2-prop-6-cor-2 .statement tag=01N0}

Soit B un espace topologique ; un B-morphisme bijectif d’un B-espace étalé dans un autre est un B-isomorphisme.

D’après le corollaire 1, un tel morphisme est étale ; il est donc ouvert (I, p. 29, remarque 2). S’il est bijectif, c’est un B-isomorphisme.

#### Corollaire 3 {#ta-i-s2-prop-6-cor-3 .statement tag=01N1}

Soit $p: E\rightarrow B$ une application étale. Toute section continue de $p$ induit un homéomorphisme de B sur une partie ouverte de E.

En effet, une telle section est étale (corollaire 1), donc ouverte.

#### Corollaire 4 {#ta-i-s2-prop-6-cor-4 .statement tag=01N2}

Soit $p: E\rightarrow B$ une application étale et séparée. Supposons que E soit connexe et que $p$ admette une section. Alors $p$ est un homéomorphisme.

Soit $s$ une section de $p$; comme $p$ est étale, l’image de $s$ est ouverte dans E (corollaire 3) ; elle est aussi fermée, car $p$ est séparée (I, p. 27, prop. 3). Puisque E est connexe, on a $s(B) = E$ et $p$ est un homéomorphisme.

#### Proposition 7 {#ta-i-s2-prop-7 .statement tag=01N3}

Soit $p: E\rightarrow B$ une application continue. Pour que l’application $p$ soit étale, il faut et il suffit qu’elle soit ouverte et que la diagonale $\Delta_E$ de $E\times_BE$ soit ouverte dans $E\times_BE$.

Supposons d’abord que l’application $p$ soit étale. Alors elle est ouverte et tout point de E possède un voisinage V tel que $p|V$ soit injectif, ce qui revient à dire que l’on a $(V\times V)\cap (E\times_BE)\subset \Delta_E$. Donc $\Delta_E$ est une partie ouverte de $E\times_BE$.

Inversement, supposons que $p$ soit une application ouverte et que $\Delta_E$ soit une partie ouverte de $E\times_BE$. Soit $x$ un point de E. Soit V un voisinage ouvert de $x$ dans E tel que $(V\times V)\cap (E\times_BE)$ soit contenu dans $\Delta_E$. Alors, $p|V$ est injective. D’après la remarque 2, I, p. 29, l’application $p$ est étale.

#### Proposition 8 {#ta-i-s2-prop-8 .statement tag=01N4}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Si l’application $p$ est étale, l’application $p'$ est étale. Inversement, si l’application $p'$ est étale et que l’application $f$ est universellement stricte et surjective, l’application $p$ est étale.

Supposons que l’application $p$ soit étale. Elle est en particulier ouverte et $p'$ est ouverte (I, p. 17, prop 8). Considérons alors le carré cartésien (I, p. 13, exemple 1)

$$
E'\times_{B'}{E'}^{\varphi}E\times_BE
$$

$q'q$

${B'}^fB$. On a $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ (loc. cit.). De plus, la diagonale $\Delta_E$ est ouverte dans $E\times_BE$ (prop. 7), donc la diagonale $\Delta_{E'}$ est ouverte dans $E'\times_{B'}E'$. Cela prouve que l’application $p'$ est étale (loc. cit.).

Supposons maintenant que l’application $f$ soit surjective et universellement stricte et que l’application $p'$ soit étale. Alors, $p'$ est ouverte, donc $p$ est ouverte (I, p. 21, prop. 11, a)). D’autre part $\Delta_{E'}$ est une partie ouverte de $E'\times_{B'}E'$. Puisque $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ et que l’application $\varphi$ est surjective et stricte (I, p. 20, déf. 6), $\Delta_E$ est ouverte dans $E\times_BE$. D’après la prop. 7, l’application $p$ est étale.

#### Corollaire {#ta-i-s2-n2-cor-1 .statement tag=01N5}

Soit B un espace topologique. Le produit fibré de deux B-espaces étalés est un B-espace étalé.

Soient $(E, p)$ et $(E', p')$ des B-espaces étalés. L’application pr$_1: E\times_B$ $E'\rightarrow E$ est étale (prop. 8), donc l’application $p\circ$ pr$_1: E\times_BE'\rightarrow B$ est étale (prop. 6, a)).

#### Remarque 3 {#ta-i-s2-n2-rem-3 .statement tag=01N6}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Si l’application $p$ est étale et si l’application $f$ est stricte, l’application $f'$ est stricte. En effet, sous ces hypothèses, tout point de E possède un voisinage ouvert U tel que $p$ induise un homéomorphisme de U sur l’ouvert $p(U)$. L’application $p'$ induit alors

un homéomorphisme de $(\overset{-1}{f}')(U)$ sur $\overset{-1}{f}(p(U))$. L’application $f$ induit

une application stricte de $\overset{-1}{f}(p(U))$ sur $p(U)$ (I, p. 20) et l’application

$f'$ induit donc une application stricte de $(\overset{-1}{f}')(U)$ dans U. Il en résulte que l’application $f'$ est stricte ( I, p. 23, corollaire 2).

### 3. Sections locales des applications étales

Soient E et B des ensembles, A une partie de B et $p: E\rightarrow B$ une application. On appelle section de $p$ au-dessus de A (ou sur A) une application $s: A\rightarrow E$ telle que $p\circ s$ soit l’injection canonique de A dans B. La donnée d’une section $s$ de $p$ au-dessus de A équivaut à la donnée d’une section de l’application $p_A:\overset{-1}{p}(A)\rightarrow A$ déduite de $p$. Si $s$ est une section de $p$ au-dessus de A et si $A'$ est une partie de A, la restriction $s'$ de $s$ à $A'$ est une section de $p$ au-dessus de $A'$. On dit alors que $s$ est un prolongement de $s'$ à A.

Lorsque E et B sont des espaces topologiques et $p: E\rightarrow$ B une application continue, l’ensemble $\mathscr{C}_B(A; E)$ (I, p. 2) des sections continues de $p$ au-dessus de A est aussi noté $\mathscr{S}(A;p)$ ou $\mathscr{S}(A; E)$. Soit $s$ une section continue de $p$ au-dessus de A. L’application $s$ induit un homéo-morphisme de A sur $s(A)$, et $p$ induit l’homéomorphisme réciproque. D’après la définition 2, I, p. 28, on a donc :

#### Proposition 9 {#ta-i-s2-prop-9 .statement tag=01N7}

Soit $p: E\rightarrow B$ une application continue. Pour que l’application $p$ soit étale, il faut et il suffit que tout point de E possède un voisinage ouvert qui soit l’image d’une section continue de $p$ au-dessus d’une partie ouverte de B.

#### Remarque 1 {#ta-i-s2-n3-rem-1 .statement tag=01N8}

Soit $p: E\rightarrow B$ une application continue et ouverte. Pour qu’un ensemble ouvert U de E soit l’image d’une section continue de $p$ au-dessus d’un ensemble ouvert de B, il faut et il suffit que la restriction de $p$ à U soit injective.

#### Remarque 2 {#ta-i-s2-n3-rem-2 .statement tag=01N9}

Soit $p: E\rightarrow$ B une application continue. Supposons que tout point de B possède un voisinage ouvert V tel qu’il existe une section continue de $p$ au-dessus de V. Une telle application $p$ n’est pas nécessairement étale, ni même ouverte. Elle est toutefois surjective et universellement stricte (I, p. 20, corollaire).

### 4. Relèvements continus des applications étales

Soient $p: E\rightarrow B$ et $f: Z\rightarrow B$ des applications continues. On appelle relèvement continu de $f$ à E une application continue $g: Z\rightarrow E$ telle que $p\circ g=f$. L’ensemble des relèvements continus de $f$ à E n’est autre que $\mathscr{C}_B(Z; E)$. Il s’identifie aussi à l’ensemble $\mathscr{S}(Z; Z\times_BE)$ des sections continues de la projection du Z-espace $(Z\times_BE$, pr$_1)$.

Si T est une partie de Z, on appelle relèvement continu de $f$ à E défini sur T un relèvement continu de $f|T$ à E :

$$
\begin{array}{ccc}
 &  & E\\
 & \nearrow & \Big\downarrow{\scriptstyle p}\\
T\subset Z & \xrightarrow{\ f\ } & B.
\end{array}
$$

#### Proposition 10 {#ta-i-s2-prop-10 .statement tag=01NA}

Soient E, B et Z des espaces topologiques, $p: E\rightarrow B$ une application étale et $f: Z\rightarrow B$ une application continue.

Soient $z\in Z$ et $x\in E$ des points tels que $f(z) =p(x)$. Il existe un voisinage W de $z$ dans Z et un relèvement continu $g$ de $f$ à E, défini sur W, tel que $g(z) =x$.

Il existe un voisinage ouvert V de $p(x)$ dans B et une section continue $s$ de $p$ au-dessus de V telle que $s(p(x)) =x$ (prop. 9). L’ensemble

$W =\overset{-1}{f}(V)$ est un voisinage ouvert de $z$ et l’application $g=s\circ (f|W)$ est un relèvement continu de $f$ à E, défini sur W et tel que $g(z) =x$.

#### Proposition 11 {#ta-i-s2-prop-11 .statement tag=01NB}

Soient E, B et Z des espaces topologiques, $p: E\rightarrow B$ et $f: Z\rightarrow B$ des applications continues. Soient $g$ et $g'$ des relèvements continus de $f$ à E. Soit W l’ensemble des points de Z où $g$ et $g'$ coïncident.

a) Si l’application $p$ est séparée, W est fermé.

b) Si l’application $p$ est étale, W est ouvert.

Notons $h$ l’application continue $(g, g'): Z\rightarrow E\times E$. L’image de $h$ est contenue dans $E\times_BE$ puisque $p\circ g=f=p\circ g'$ et l’ensemble W des points de Z où $g$ et $g'$ coïncident est l’image réciproque par $h$ de la diagonale $\Delta_E$.

Si l’application $p$ est étale, la diagonale $\Delta_E$ est ouverte dans $E\times_BE$ (I, p. 31, prop. 7), donc l’ensemble W est ouvert dans Z.

Si l’application $p$ est séparée, la diagonale $\Delta_E$ est fermée dans $E\times_BE$ (I, p. 25, déf. 1) et l’ensemble W est fermé dans Z.

#### Corollaire 1 {#ta-i-s2-prop-11-cor-1 .statement tag=01NC}

Si l’espace Z est connexe et si l’application $p$ est étale et séparée, des relèvements continus de $f$ à E qui coïncident en un point sont égaux.

#### Corollaire 2 {#ta-i-s2-prop-11-cor-2 .statement tag=01ND}

Soit $p: E\rightarrow B$ une application étale et séparée. Si l’espace E est connexe, le groupe Aut$_B(E)$ opère librement sur E.

En effet, si $f: E\rightarrow E$ est un B-morphisme, l’ensemble des points où coïncident $f$ et Id$_E$ est égal à E ou à l’ensemble vide par le cor. 1.

#### Corollaire 3 {#ta-i-s2-prop-11-cor-3 .statement tag=01NE}

Soient E, B et Z des espaces topologiques, soit $p: E\rightarrow B$ une application étale et séparée, et soit $f: Z\rightarrow B$ une application continue. Pour $i= 1$, 2, soient $U_i$ une partie ouverte ( resp. fermée) de Z et $g_i: U_i\rightarrow E$ un relèvement continu de $f$ défini sur $U_i$. On suppose que l’intersection $U_1\cap U_2$ est connexe et qu’il existe un point $z$ de $U_1\cap U_2$ tel que $g_1(z) =g_2(z)$. Il existe alors un relèvement continu de $f$ défini sur $U_1\cup U_2$ qui prolonge $g_1$ et $g_2$.

D’après le corollaire 1, les restrictions à $U_1\cap U_2$ de $g_1$ et $g_2$ sont égales. L’application $g: U_1\cup U_2\rightarrow E$ définie par $g(z) =g_i(z)$ pour $z\in U_i(i= 1$, 2) est un relèvement continu de $f$ défini sur $U_1\cup U_2$ (TG, I, p. 19, prop. 4).

Dans les résultats précédents, le cas particulier où Z = B et $f=$ Id$_B$ est important : les relèvements continus de $f$ sont alors les sections continues de $p$.

#### Proposition 12 {#ta-i-s2-prop-12 .statement tag=01NF}

Soit $p: E\rightarrow B$ une application étale. Pour que l’application $p$ soit séparée, il faut et il suffit que pour toute partie ouverte V de B et tout couple $(s, s')$ de sections continues de $p$ au-dessus de V, l’ensemble des points où $s$ et $s'$ coïncident soit fermé dans V.

La condition est nécessaire (proposition 11, I, p. 34). Démontrons qu’elle est suffisante. Soit $b$ un point de B, soient $x$ et $x'$ deux points distincts de E tels que $p(x) =p(x') =b$. Soient V un voisinage ouvert de $b$ et $s,s'$ des sections continues de $p$ au-dessus de V telles que $s(V)$ et $s'(V)$ soient des voisinages ouverts de $x$ et $x'$ respectivement (prop. 9). Par hypothèse, l’ensemble W des points $x\in V$ tels que $s(x)=\not s'(x)$ est ouvert dans V, donc dans B. Les ensembles $s(W)$ et $s'(W)$ sont des voisinages ouverts de $x$ et $x'$ respectivement ; ils sont disjoints par construction. Cela prouve que l’application $p$ est séparée (I, p. 25, définition 1).

### 5. Construction de sections continues d’applications étales

#### Théorème 1 {#ta-i-s2-thm-1 .statement tag=01NG}

Soient X, Y, Z des espaces topologiques, soit $f: Z\rightarrow$ $X\times Y$ une application étale et séparée, et soit $y_0$ un point de Y. Soit $s: X\times Y\rightarrow Z$ une section de $f$. On suppose que la restriction de $s$ à $X\times  \{y_0\}$ est continue, de même que les restrictions de $s$ à $\{x\} \times Y$ pour tout $x\in X$. Si l’espace Y est connexe et localement connexe (TG, I, p. 84, déf. 4), l’application $s$ est continue.

#### Lemme {#ta-i-s2-n5-lem-1 .statement tag=01NH}

Soit U un ouvert de X, soit V un ouvert connexe de Y et soit $(x_1, y_1)\in U\times V$. On suppose que la restriction de $s$ à $U\times  \{y_1\}$ est continue. Soit $\sigma$ une section continue de $f$ au-dessus de $U\times V$ telle que $\sigma (x_1, y_1) =s(x_1, y_1)$. Il existe un voisinage $U'$ de $x_1$ tel que $s=\sigma$ sur $U'\times V$. En particulier, $s$ est continue au voisinage de $(x_1, y_1)$.

Comme la restriction de $s$ à $U\times  \{y_1\}$ est continue et que l’application $f$ est étale, il existe un voisinage $U'$ de $x_1$ tel que $s(x, y_1) =\sigma (x, y_1)$ pour tout $x\in U'($I, p. 34, prop. 11, b)). Soit $x\in U'$; puisque la restriction de $s$ à $\{x\} \times V$ est continue et que l’application $f$ est étale et séparée, il résulte du cor. 1, I, p. 34. que $\sigma (x, y) =s(x, y)$ pour tout $y\in V$. Ainsi, $s$ et $\sigma$ coïncident sur $U'\times V$.

Démontrons maintenant le théorème. Démontrons d’abord que l’application $s$ est continue au voisinage de tout point de $X\times  \{y_0\}$. Soit $x_0\in$ X ; on peut choisir un voisinage ouvert U de $x_0$ dans X, un voisinage ouvert connexe V de $y_0$ dans Y et une section continue $\sigma : U\times V\rightarrow Z$ de $f$ telle que $\sigma (x_0, y_0) =s(x_0, y_0)$. D’après le lemme ci-dessus, $s$ est continue au voisinage de $(x_0, y_0)$.

Démontrons maintenant que l’application $s$ est continue en tout point de $X\times Y$. Pour $x_0\in X$, notons $C(x_0)$ l’ensemble des points $y\in$ Y tels que $s$ soit continue au voisinage de $(x_0, y)$. L’ensemble $C(x_0)$ est ouvert dans Y par définition, et contient $y_0$ d’après ce qui précède.

Démontrons qu’il est fermé dans Y. Considérons un point $y_1$ de Y adhérent à $C(x_0)$, un voisinage ouvert U de $x_0$ dans X, un voisinage ouvert V de $y_1$ dans Y, et une section continue $\sigma : U\times V\rightarrow Z$ de $f$ telle que $\sigma (x_0, y_1) =s(x_0, y_1)$. Puisque la restriction de $s$ à $\{x_0\} \times V$ est continue et que $f$ est étale, il existe un voisinage ouvert $V'$ de $y_1$ dans Y tel que $\sigma (x_0, y) =s(x_0, y)$ pour tout $y\in V'$ (prop. 11 de I, p. 34). Comme Y est localement connexe, on peut supposer que $V'$ est connexe. Comme $y_1$ est adhérent à $C(x_0)$, l’ensemble $C(x_0)\cap V'$ n’est pas vide ; soit $y_2$ un point de $C(x_0)\cap V'$. D’après le lemme appliqué à $(x_0, y_2)$, il existe un voisinage $U'$ de $x_0$ contenu dans U tel que $s=\sigma$ au-dessus de $U'\times V'$. Cela prouve que $C(x_0)$ est fermé, car $U'\times V'$ est un voisinage de $(x_0, y_1)$. Comme Y est connexe, on a $C(x_0) = Y$, et cela pour tout $x_0\in X$, d’où le théorème.

#### Corollaire 1 {#ta-i-s2-thm-1-cor-1 .statement tag=01NI}

Soient X, Y, E, B des espaces topologiques. Soit $p: E\rightarrow B$ une application étale et séparée, soit $h: X\times Y\rightarrow B$ une application continue et soit $y_0$ un point de Y. Soit $g: X\times Y\rightarrow E$ une application telle que $p\circ g=h$. On suppose que les restrictions de $g$ à $X\times  \{y_0\}$ d’une part et, pour tout $x\in X$, à $\{x\} \times Y$ d’autre part, sont continues. Si l’espace Y est connexe et localement connexe, l’application $g$ est continue.

Notons Z le produit fibré $(X\times Y)\times_BE$ et $f: Z\rightarrow X\times Y,h': Z\rightarrow E$ les projections canoniques. L’application $f$ est étale (I, p. 31, prop. 8) et séparée (I, p. 27, prop. 4). L’application $s: X\times Y\rightarrow$ Z définie par $s(x, y) = ((x, y), g(x, y))$ est une section de $f$ qui satisfait aux hypothèses du théorème 1. Elle est donc continue ainsi que $g=h'\circ s$.

#### Remarque {#ta-i-s2-n5-rem-1 .statement tag=01NJ}

Si, dans le théorème 1, on ne suppose pas que l’espace Y est localement connexe, la conclusion du théorème n’est plus nécessairement exacte (I, p. 141, exerc. 7).

#### Théorème 2 {#ta-i-s2-thm-2 .statement tag=01NK}

Soient B un espace topologique et A un sous-espace de B. Faisons l’une des hypothèses suivantes :

(i) A admet un système fondamental de voisinages paracompacts ;

(ii) B est paracompact et A fermé ;

(iii) B est métrisable ;

(iv) A est compact et deux points distincts de A possèdent dans B des voisinages disjoints.

Alors, toute section continue au-dessus de A d’une application étale $p: E\rightarrow B$ se prolonge en une section continue de $p$ au-dessus d’un voisinage de A.

Considérons la propriété (PCV) suivante du couple $(B,A)$ :

(PCV) Pour tout recouvrement $(U_i)_{i\in I}$ de A par des parties ouvertes

de B, il existe un voisinage V de A et une famille localement

finie $(F_j)_{j\in J}$ de parties fermées de V recouvrant V, telle que

chacun des $F_j$ soit contenu dans l’un des $U_i$.

Le théorème 2 résulte des lemmes 1 et 3 ci-dessous.

#### Lemme 1 {#ta-i-s2-lem-1 .statement tag=01NL}

Chacune des propriétés (i) à (iv) du théorème 2 implique la propriété (PCV).

Soit $(U_i)_{i\in I}$ un recouvrement de A par des ouverts de B. Sous l’hypothèse (i), il existe un voisinage paracompact V de A contenu dans la réunion des $U_i$, un recouvrement ouvert $(U'_j)_{j\in J}$ de l’espace V, localement fini et plus fin que le recouvrement $(V\cap U_i)_{i\in I}$ et un recouvrement ouvert $(U''_j)_{j\in J}$ de l’espace V tel que pour tout $j\in J$, l’adhérence $F_j$ de $U''_j$ dans V soit contenue dans $U'_j$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1 au th. 3). D’où la propriété (PCV) dans ce cas.

La condition (ii) implique la condition (i) d’après le corollaire 2 de TG, IX, p. 50. De même, la condition (iii) implique la condition (i) : en effet, si B est métrisable, tout voisinage de A est métrisable, donc paracompact (TG, IX, p. 51, th. 4).

Supposons enfin la condition (iv) satisfaite et montrons que la propriété (PCV) est vérifiée. Comme A est compact, il suffit de considérer le cas d’un recouvrement fini $(U_i)_{0\leqslant i\leqslant n}$. Construisons alors par récurrence des ouverts $V_0, . . . ,V_n$ de B satisfaisant aux conditions suivantes pour $0\leqslant i\leqslant n:$

$$
\alpha )A\subset V_0\cup  \cdots  \cup V_i\cup U_{i+1}\cup  \cdots  \cup U_n
$$

$$
\beta )V_i\cap A\subset U_i
$$

Supposons construits $V_0, . . . ,V_{r-1}$ satisfaisant aux conditions ci-dessus pour $0\leqslant i\leqslant r-1$ et construisons $V_r$. Les ensembles K = $A\cap \complement U_r$ et $L = A\cap \complement (V_0\cup \cdots \cup V_{r-1}\cup U_{r+1}\cup \cdots \cup U_n)$ sont fermés dans A, donc compacts. En raison de $(\alpha )$, ils sont disjoints. Par hypothèse, pour tout point $a$ de L et tout point $b$ de K, il existe des voisinages de $a$ et $b$ dans B disjoints. D’après le lemme 2 ci-dessous, il existe des ensembles ouverts $V_r$ et W dans B, disjoints et tels que $L\subset V_r$ et $K\subset W$. Des inclusions $L\subset V_r$ et $A\subset V_0\cup  \cdots  \cup V_{r-1}\cup U_r\cup  \cdots  \cup U_n$ et de la définition de L, on en déduit que l’on a $(\alpha )$ pour $i=r$. D’autre part, on a $V_r\cap K =\emptyset$, d’où $V_r\cap A\subset U_r$.

L’ensemble $M =\bigcup_{0\leqslant i\leqslant n}(V_i\cap \complement U_i)$ est fermé et ne rencontre pas A d’après $(\beta )$. D’après $(\alpha )$, l’ensemble V = $\bigcup_{0\leqslant i\leqslant n}V_i$ - M est un voisinage de A dans B. Pour $i= 0, . . . , n$, posons $F_i= V\cap V_i:$ c’est une partie fermée de V, contenue dans $U_i$. La famille $(F_i)_{0\leqslant i\leqslant n}$ est un recouvrement de V, d’où la propriété (PCV).

#### Lemme 2 {#ta-i-s2-lem-2 .statement tag=01NM}

Soit B un espace topologique et soient K et L des parties quasi-compactes de B. On suppose que pour tout point $a$ de K et tout point $b$ de L, il existe des voisinages disjoints de $a$ et $b$ dans B. Alors, il existe deux ouverts disjoints U et V dans B tels que $K\subset U$ et $L\subset V$.

Soit $a$ un point de K. Pour tout $b\in L$, soient $U_{a,b}$ et $V_{a,b}$ des voisinages ouverts disjoints de $a$ et de $b$. Pour $a$ fixé, la famille $(V_{a,b})_{b\in L}$ est un recouvrement ouvert de L. Comme cet espace est quasi-compact, il existe une famille finie $T_a\subset L$ telle que la réunion $V_b$ des $V_{a,b}$ pour $b\in T_a$ contienne L. L’intersection $U_a$ des $U_{a,b}$ pour $b\in T_a$ est un voisinage ouvert de $a$, car $T_a$ est fini ; de plus, $U_a$ et $V_a$ sont disjoints. Les $(U_a)_{a\in A}$ forment un recouvrement ouvert de K. Comme K est quasi-compact, il existe une famille finie $S\subset K$ telle que $U =\bigcup_{a\in S}U_a$ contienne K. Alors, $V =\bigcap_{a\in S}V_a$ est un ouvert de B qui contient L. Le lemme est démontré.

#### Lemme 3 {#ta-i-s2-lem-3 .statement tag=01NN}

Soient B un espace topologique et A un sous-espace de B tels que le couple $(B,A)$ vérifie la propriété (PCV) de I, p. 37. Alors, toute section continue au-dessus de A d’une application étale $p: E\rightarrow B$ se prolonge en une section continue de $p$ au-dessus d’un voisinage de A.

Soient $p: E\rightarrow B$ une application étale et $s: A\rightarrow E$ une section continue de $p$ au-dessus de A. Pour tout point $a$ de A, il existe un voisinage ouvert $U_a$ de $a$ et une section continue $s_a: U_a\rightarrow E$ qui coïn-cide avec $s$ sur $U_a\cap A$ (I, p. 34, prop. 10 et I, p. 34, prop. 11). La famille $(U_a)_{a\in A}$ est un recouvrement de A par des ensembles ouverts de B. Soit V un voisinage de A dans B, soit $(F_j)_{j\in J}$ une famille localement finie de parties fermées de V recouvrant V et soit $a: J\rightarrow A$ une application telle que $F_j$ soit contenu dans $U_{a(j)}$ pour tout $j\in J$ (propriété (PCV)). Notons $s_j$ la restriction de $s_{a(j)}$ à $F_j$. Soit W l’ensemble des points $b\in V$ satisfaisant à $s_j(b) =s_k(b)$ pour tout couple $(j, k)\in J\times J$ tel que $b\in F_j\cap F_k$. On définit une section $s': W\rightarrow E$ par $s'(b) =s_j(b)$ si $b\in F_j$. On a $A\subset W$ et $s'|A =s$. La section $s'$ est continue d’après la prop. 4 de I, p. 19.

Il reste à démontrer que W est un voisinage de A dans B. Pour tout couple $(j, k)\in J\times J$, notons $T_{jk}$ l’ensemble des points $b\in F_j\cap F_k$ tels que $s_j(b)=\not s_k(b)$. L’ensemble $T_{jk}$ est fermé dans $F_j\cap F_k$ (prop. 11, b) de I, p. 34), donc dans V et les ensembles $T_{jk}$ constituent une famille localement finie de parties de V. La réunion T de la famille $(T_{jk})$ est donc un ensemble fermé de V (TG, I, p. 6, prop. 4). Or W est, par définition, le complémentaire de T dans V. C’est donc un voisinage de A dans V et par suite, dans B.

### 6. Majoration du cardinal des fibres d’une application étale et séparée

#### Théorème 3 {#ta-i-s2-thm-3 .statement tag=01NO}

Soient E et B des espaces topologiques et $p: E\rightarrow B$ une application étale et séparée. On suppose que E est connexe et que B est localement connexe. Soit $\mathscr{W}$ une base de la topologie de B. Alors, pour tout point $a$ de B, on a Card(E$_a)\leqslant$ sup(Card($\mathscr{W}$), Card($\mathbf{N}$)).

Comme l’espace B est localement connexe, sa topologie possède une base $\mathscr{W}'$ constituée d’ouverts connexes, par exemple les composantes connexes des ouverts de $\mathscr{W}$ (TG, I, p. 85, prop. 11). En vertu du lemme 4 ci-dessous, il existe une base $\mathscr{V}$ de la topologie de B composée d’ouverts connexes et telle que Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

#### Lemme 4 {#ta-i-s2-lem-4 .statement tag=01NP}

Soit B un espace topologique et soient $\mathscr{W}$ et $\mathscr{W}'$ des bases de la topologie de B. Il existe un sous-ensemble $\mathscr{V}$ de $\mathscr{W}'$ qui est une base de la topologie de B et tel que Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

Soit $\mathscr{A}\subset \mathscr{W}\times \mathscr{W}$ l’ensemble des couples $(W_1,W_2)$ pour lesquels il existe $W'\in \mathscr{W}'$ tel que $W_1\subset W'\subset W_2$; soit $\varphi :\mathscr{A}\rightarrow \mathscr{W}'$ une application telle que l’on ait $W_1\subset \varphi (W_1,W_2)\subset W_2$ pour tout couple $(W_1,W_2)\in \mathscr{A}$, et soit $\mathscr{V}\subset \mathscr{W}'$ l’image de $\varphi$. On a

Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{A}$)$\leqslant$ Card($\mathscr{W}\times \mathscr{W}$)

(E, III, p. 25, prop. 3). Démontrons que $\mathscr{V}$ est une base de la topologie de B. Soient $x$ un point de B et U un voisinage de $x$. Par hypothèse, $x$ admet un voisinage $W_2\in \mathscr{W}$ contenu dans U, un voisinage $W'\in \mathscr{W}'$ contenu dans $W_2$ et un voisinage $W_1\in \mathscr{W}$ contenu dans $W'$. On a ainsi $W_1\subset W'\subset W_2\subset U$. Alors, $(W_1,W_2)\in \mathscr{A}$ et $\varphi (W_1,W_2)$ est un voisinage de $x$ contenu dans U. D’après la prop. 3 de TG, I, p. 5, l’ensemble $\mathscr{V}$ est une base de la topologie de B.

Soit $\mathscr{V}$ une base de la topologie de B constituée d’ouverts connexes non vides et telle que Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$. Soit $\mathscr{U}$ l’ensemble des ouverts U de E tels que $p$ induise un homéomorphisme de U sur un ouvert V appartenant à $\mathscr{V}$. Tout élément de $\mathscr{U}$ est un ouvert connexe et non vide. Comme l’application $p$ est étale, d’après la définition 2 (I, p. 28) et la prop. 3 de TG, I, p. 5, l’ensemble $\mathscr{U}$ est une base de la topologie de E. Appelons chenille toute suite finie $(U_0, . . . ,U_n)$ d’éléments de $\mathscr{U}$ telle que pour $1\leqslant i\leqslant n,U_{i-1}\cap U_i$ soit non vide et $p(U_{i-1})\cap p(U_i)$ soit connexe. Notons S l’ensemble des suites finies d’éléments de $\mathscr{V}$ et, pour toute chenille $c= (U_0, . . . ,U_n)$, notons $p(c)$ la suite $(p(U_0), . . . , p(U_n))$.

#### Lemme 5 {#ta-i-s2-lem-5 .statement tag=01NQ}

a) Soient $c= (U_0, . . . ,U_n)$ et $c'= (U'_0, . . . ,U'_m)$ des chenilles telles que $U_0= U'_0$ et $p(c) =p(c')$. Alors, $c=c'$.

b) Soient U et $U'$ des éléments de $\mathscr{U}$. Il existe alors une chenille $c= (U_0, . . . ,U_n)$ telle que $U_0= U$ et $U_n= U'$.

a) On a nécessairement $m=n$. Pour tout entier $i$ tel que $0\leqslant i\leqslant n$, posons $V_i=p(U_i)$ et notons $s_i$ et $s'_i$ les sections continues de $p$ au-dessus de $V_i$ d’images respectives $U_i$ et $U'_i$. Pour démontrer l’égalité $c=c'$, nous allons démontrer, par récurrence sur $i$, l’égalité $s_i=s'_i$ pour tout entier $i$ tel que $0\leqslant i\leqslant n$. Par hypothèse, on a $s_0=s'_0$. Soit $i$ tel que $1\leqslant i\leqslant n$ et $s_{i-1}=s'_{i-1}$. Comme $U_{i-1}\cap U_i$ contient un point $x$, les sections continues $s_{i-1}$ et $s_i$ coïncident en $p(x)$, donc en tout point de $V_{i-1}\cap V_i$, puisqu’il est connexe (corollaire 1 de I, p. 34). Il en est de même pour $s'_{i-1}$ et $s'_i$. Pour la même raison, $s_i$ et $s'_i$ qui coïncident dans $V_{i-1}\cap V_i$ coïncident aussi dans $V_i$, d’où le résultat.

b) Si $x$ et $y$ sont des points de E, on dit qu’une chenille $c= (U_0, . . . ,U_n)$ relie $x$ à $y$ si $x\in U_0$ et $y\in U_n$. Dans l’ensemble E, soit R la relation « il existe une chenille qui relie $x$ à $y$ ». La relation R est réflexive puisque $\mathscr{U}$ est un recouvrement de E. Elle est évidemment symétrique. Démontrons qu’elle est transitive : soient $x,y,z$ trois points de E, $(U_0, . . . ,U_n)$ et $(U'_0, . . . ,U'_m)$ des chenilles reliant $x$ à $y$ et $y$ à $z$ respectivement. Soit $U\in \mathscr{U}$ un voisinage de $y$ contenu dans $U_n\cap U'_0$; on a $p(U_n)\cap p(U) =p(U'_0)\cap p(U) =p(U)$, et, comme U est connexe , la suite $(U_0, . . . ,U_n,U,U'_0, . . . ,U'_m)$ est une chenille qui relie $x$ à $z$. Les classes d’équivalence suivant R sont ouvertes, donc aussi fermées. Puisque E est connexe, il en résulte que deux points de E sont toujours reliés par une chenille.

Soient maintenant U et $U'$ des éléments de $\mathscr{U},x$ un point de U et $x'$ un point de $U'$. Il existe une chenille $(U_2, . . . ,U_{n-2})$ reliant $x$ à $x'$. Soient $U_1$ et $U_{n-1}$ des ouverts de $\mathscr{U}$ tels que $x\in U_1,x'\in U_{n-1}$, $U_1\subset U\cap U_2,U_{n-1}\subset U'\cap U_{n-2}$. Posons $U_0= U$, $U_n= U'$. Alors la suite $(U_0, . . . ,U_n)$ est une chenille.

Démontrons maintenant le théorème. Soit U un élément de $\mathscr{U}$ et soit C l’ensemble des chenilles $(U_0, . . . ,U_n)$ telles que $U_0= U$. L’application de C dans S qui, à une chenille $c= (U_0, . . . ,U_n)$ de C, associe la suite $p(c) = (p(U_0), . . . , p(U_n))$ est injective (lemme 5, a)), donc

(1) Card(C) $\leqslant$ Card(S).

L’application de C dans $\mathscr{U}$ qui, à $c= (U_0, . . . ,U_n)\in C$, associe l’ouvert $U_n$ est surjective d’après la deuxième partie du lemme 5, donc (2) Card($\mathscr{U}$)$\leqslant$ Card(C).

Pour tout point $x$ de E, choisissons un ensemble ouvert $U_x$ de $\mathscr{U}$ tel que $x\in U_x$. Si $x$ et $y$ sont des points distincts d’une même fibre $E_a$ de $p$, on a $U_x= U\not_y$ puisque $p|U_x$ est injective. On a donc, pour $a\in B$, (3) Card(E$_a)\leqslant$ Card($\mathscr{U}$).

Enfin, si $\mathscr{V}$ est un ensemble fini, l’ensemble S des suites finies d’éléments de $\mathscr{V}$ est dénombrable (E, III, p. 49, prop. 1), donc

(4) Card(S) $\leqslant$ Card($\mathbf{N}$).

Si $\mathscr{V}$ est infini, on a

(5) Card(S) = Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2=$ Card($\mathscr{W}$)

d’après le corollaire de E, III, p. 50 et le corollaire 1 de E, III, p. 49. Le théorème résulte des relations (1) à (5) ci-dessus.

#### Remarque {#ta-i-s2-n6-rem-1 .statement tag=01NR}

D’après ce qui précède, si la topologie de B admet une base dénombrable, il en est de même de celle de E et les fibres de E sont dénombrables (cf. TG, I, p. 88, théorème de Poincaré-Volterra).
