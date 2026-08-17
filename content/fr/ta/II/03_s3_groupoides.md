---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 3
section_title: Groupoïdes
lang: fr
source: ta-i-iv-fr
book_pages: TA II.159-TA II.179, TA II.223-TA II.227
pdf_pages: 0175-0195, 0239-0243
extraction: native
subsections:
    - "no": 1
      title: Catégories
      page: 159
      pdf_page: 175
    - "no": 2
      title: Foncteurs
      page: 161
      pdf_page: 177
    - "no": 3
      title: Groupoïdes
      page: 162
      pdf_page: 178
    - "no": 4
      title: Orbites d’un groupoïde
      page: 162
      pdf_page: 178
    - "no": 5
      title: Exemples de groupoïdes
      page: 163
      pdf_page: 179
    - "no": 6
      title: Sous-groupoïdes
      page: 164
      pdf_page: 180
    - "no": 7
      title: Opérations d’un groupoïde
      page: 167
      pdf_page: 183
    - "no": 8
      title: Sous-groupoïdes distingués ; quotients de groupoïdes
      page: 168
      pdf_page: 184
    - "no": 9
      title: Groupoïde des classes de chemins d’un graphe
      page: 171
      pdf_page: 187
    - "no": 10
      title: Groupoïdes libres
      page: 174
      pdf_page: 190
    - "no": 11
      title: Contraction de flèches d’un groupoïde
      page: 175
      pdf_page: 191
    - "no": 12
      title: Groupe de Poincaré d’un graphe
      page: 178
      pdf_page: 194
statements: 40
exercises: 12
content_sha256: 4dfe715249b961d96e905eb455b131622f7a232e95b9449e4111e563d625299f
---

## § 3. GROUPOÏDES

### 1. Catégories

#### Définition 1 {#ta-ii-s3-def-1 .statement tag=01SZ}

Soit C un carquois. Notons J l’ensemble des couples $(f, g)$ de flèches de C tels que $t(f) =o(g)$. Une loi de composition dans C est une application $m: J\rightarrow$ Fl(C) telle que, pour tout couple $(f, g)\in J$, l’origine de la flèche $m(f, g)$ soit celle de $f$ et son terme celle de $g$.

Soit C un carquois muni d’une loi de composition $m$. Deux flèches $f$ et $g$ telles que $t(f) =o(g)$ sont dites composables ; la flèche $m(f, g)$ s’appelle leur composée, ou leur produit, et se note souvent $f\cdot g$, voire $f g$.

Pour tout sommet $a$ de C, l’ensemble $C_{a,a}$ = Fl$_{a,a}(C)$, muni de l’application déduite de $m$ par passage aux sous-ensembles, est un magma (A, I, p. 1, déf. 1).

On dit qu’une famille $(f_i)_{i\in I}$ de flèches de C, indexée par un ensemble fini non vide totalement ordonné I, est composable si, pour tout couple $(i, j)$ d’éléments consécutifs de I, les flèches $f_i$ et $f_j$ sont composables. On définit le produit $\prod_{i\in I}f_i$ d’une telle famille par récurrence sur le cardinal de I de la façon suivante (cf. A, I, p. 3) :

(i) si I a un seul élément $\omega ,\prod_{i\in I}f_i=f_{\omega}$;

(ii) si I a au moins deux éléments et si $\omega$ est le plus petit élément de I, on pose $\prod_{i\in I}f_i=f_{\omega}\cdot \prod_{i\in I-\{\omega\}}f_i$.

La loi de composition $m$ est dite associative si l’on a $f\cdot (g\cdot h) =$ $(f\cdot g)\cdot h$ pour tout triplet $(f, g, h)$ composable de flèches de C. Lorsque la loi $m$ est associative, le produit d’une suite $(f_1, . . . , f_n)$ de $n$ flèches composables, où $n$ est un entier $\geqslant 1$, se note $f_1f_2. . . f_n$.

Soit $a$ un sommet de C. On dit qu’une flèche $e\in C_{a,a}$ est un élément neutre de $m$ en $a$ si l’on a $ef=f$ pour toute flèche $f$ d’origine $a$ et $ge=g$ pour toute flèche $g$ de terme $a$. Il existe au plus un élément neutre de $m$ en $a:$ si $e$ et $e'$ en sont deux, on a $e'=ee'=e$. Lorsqu’un tel élément neutre existe, on le note souvent $e_a$; c’est alors un élément neutre du magma $C_{a,a}$ (A, I, p. 12).

#### Définition 2 {#ta-ii-s3-def-2 .statement tag=01T0}

Une catégorie est un carquois muni d’une loi de composition associative pour laquelle il existe en chaque sommet un élément neutre.

#### Exemple 1 {#ta-ii-s3-n1-exa-1 .statement tag=01T1}

Soit C un carquois. Notons Ch(C) l’ensemble des chemins dans C et $o:$ Ch(C) $\rightarrow$ Som(C)$,t:$ Ch(C) $\rightarrow$ Som(C) les applications qui, à un chemin, associent son origine et son terme. Le quadruplet $\Omega_C=$ (Som(C), Ch(C)$, o, t)$ est un carquois. Munissons-le de la loi de composition définie par la juxtaposition des chemins. Cette loi de composition est associative ; pour tout sommet $a$ de C, le lacet constant $e_a= (a)$ d’origine $a$ est un élément neutre en $a$. Ainsi, $\Omega_C$ est une catégorie. On dit que c’est la catégorie des chemins du carquois C.

#### Exemple 2 {#ta-ii-s3-n1-exa-2 .statement tag=01T2}

Soit Σ une espèce de structure dans une théorie $\mathscr{T}$ plus forte que la théorie des ensembles et soit $\sigma (x, y, s, u)$ un terme de $\mathscr{T}$ vérifiant les conditions (MO$_I)$, (MO$_{II})$ et (MO$_{III})$ de E, IV, p. 11. Soit S un ensemble ; on suppose que tout élément de S est un couple $(x, s)$, où $x$ est un ensemble et $s$ une structure d’espèce Σ sur $x$. Soit F l’ensemble des applications $f$ telles qu’il existe $(x, s)$ et $(y, t)$ dans S de sorte que $f$ soit un $\sigma$-morphisme de $x$, muni de la structure $s$, dans $y$, muni de la structure $t$; on pose alors $o(f) = (x, s)$ et $t(f) = (y, t)$. Muni de la loi de composition donnée par $m(f, g) =g\circ f$, le carquois $(S,F, o, t)$ est une catégorie. Dans ce contexte, les éléments de S sont plutôt appelés objets.

Soit C une catégorie.

Pour tout sommet $a$ de C, l’ensemble $C_{a,a}$, muni de la loi de composition $(f, g)\mapsto f g$, est un monoïde d’élément neutre $e_a$.

On dit qu’une flèche $f$ de C est inversible s’il existe une flèche $g$ de C telle que $o(g) =t(f),t(g) =o(f)$ et telle que $f g$ et $gf$ soient des éléments neutres en $o(f)$ et $t(f)$ respectivement. Une telle flèche $g$ est unique (si $f g=e_{o(f)}$ et $g'f=e_{t(f)}$, on a $g=e_{t(f)}g= (g'f)g=$ $g'(f g) =g'e_{o(f)}=g')$ et est appelée inverse de $f$; l’inverse d’une flèche inversible $f$ est notée $f^{-1}$.

### 2. Foncteurs

#### Définition 3 {#ta-ii-s3-def-3 .statement tag=01T3}

Soient C et $C'$ des catégories. On appelle foncteur de C dans $C'$ un morphisme de carquois $\varphi : C\rightarrow C'$ tel que $\varphi (f g) =$ $\varphi (f)\varphi (g)$ pour tout couple $(f, g)$ de flèches composables de C.

Soient C et $C'$ des catégories et soit $\varphi : C\rightarrow C'$ un foncteur. Soient $f$ une flèche de C$,a$ son origine et $b$ son terme ; alors, $\varphi (f)$ est une flèche de $C'$ d’origine $\varphi (a)$ et de terme $\varphi (b)$.

Soient C, $C',C''$ des catégories et soient $\varphi : C\rightarrow C'$ et $\varphi ': C'\rightarrow C''$ des foncteurs. Alors, $\varphi '\circ \varphi$ est un foncteur.

Soit C une catégorie. Alors le morphisme de carquois Id$_C$ est un foncteur.

Soit $\varphi : C\rightarrow C'$ un foncteur. Pour que $\varphi$ soit un isomorphisme, il faut et il suffit que les applications Som($\varphi$ ) et Fl($\varphi$ ) soient bijectives.

Ainsi, si l’on appelle structure de catégorie sur des ensembles S et F la donnée d’une structure de carquois sur ces ensembles et d’une loi de composition associative pour laquelle il existe en chaque sommet un élément neutre, on peut prendre les foncteurs pour morphismes de la structure de catégorie (E, IV, p. 11).

### 3. Groupoïdes

#### Définition 4 {#ta-ii-s3-def-4 .statement tag=01T4}

Un groupoïde est une catégorie dont chaque flèche est inversible.

Soit G un groupoïde et soit $a$ un sommet de G. Le monoïde $G_{a,a}$ est un groupe, que l’on note $G_a$ et qu’on appelle le groupe d’isotropie de G en $a$.

Soient $a,b$ des sommets de G et soit $f\in G_{a,b}$ une flèche reliant $a$ à $b$. L’application $g\mapsto f gf^{-1}$ est un isomorphisme de groupes de $G_b$ dans $G_a$, que l’on note Int($f$). Si $f$ et $f'$ sont des flèches composables de G, on a Int($f f'$) $=$ Int($f$)$\circ$ Int($f'$) ; l’inverse de l’isomorphisme Int($f$) est l’isomorphisme Int($f^{-1}$).

Un morphisme de groupoïdes $\varphi : G\rightarrow G'$ est un morphisme de catégories. De plus, $\varphi$ est un isomorphisme de groupoïdes si et seulement si c’est un isomorphisme de catégories.

Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes. Pour tout sommet $a$ de G, l’application $f\mapsto \varphi (f)$ de $G_a$ dans $(G')_{\varphi(a)}$ est un homomorphisme de groupes que l’on note $\varphi_a$. On a en particulier $\varphi (e_a) =e_{\varphi(a)}$.

Pour toute flèche $f$ de G$,\varphi (f^{-1})$ est l’inverse de $\varphi (f)$. Si $f$ est une flèche de G reliant un sommet $a$ à un sommet $b$, on a ainsi, pour tout élément $g\in G_b$, la relation Int($\varphi (f)$)$(\varphi (g)) =\varphi$(Int($f$)$(g))$.

### 4. Orbites d’un groupoïde

Soit G un groupoïde. Les composantes connexes du carquois sous-jacent à G sont appelées orbites de G. L’ensemble des orbites de G est noté Orb(G); si $\varphi : G\rightarrow G'$ est un morphisme de groupoïdes, l’application $\pi_0(\varphi )$ déduite de $\varphi$ par passage aux composantes connexes des graphes associés est en général notée Orb($\varphi$ ) et appelée l’application déduite de $\varphi$ par passage aux orbites.

Un groupoïde qui a exactement une orbite est dit transitif . Si G est un groupoïde transitif, les groupes $G_a$, pour $a\in$ Som(G), sont isomorphes. On dit que le groupoïde G est simplement transitif s’il est transitif et si, de plus, les groupes d’isotropie $G_a$ sont tous réduits à leur élément neutre.

#### Proposition 1 {#ta-ii-s3-prop-1 .statement tag=01T5}

Soit G un groupoïde. La relation « il existe une flèche de G reliant $a$ à $b$ » est une relation d’équivalence dans l’ensemble des sommets de G dont les classes d’équivalence sont les orbites de G.

Soient $a,b,c$ des sommets de G. On a $e_a\in G_{a,a}$; si $f\in G_{a,b}$, $f^{-1}\in G_{b,a}$; si $f\in G_{a,b}$ et $g\in G_{b,c}$, on a $f g\in G_{a,c}$. Cela montre que la relation indiquée est réflexive, symétrique et transitive ; c’est donc une relation d’équivalence. La seconde assertion résulte alors de la définition des composantes connexes d’un carquois.

### 5. Exemples de groupoïdes

1) Soit G un groupe. Notons $\mathscr{G}$ le carquois dont l’ensemble des sommets est réduit à un élément et dont l’ensemble des flèches est G. Muni de la loi de composition induite par celle de G$,\mathscr{G}$ est un groupoïde, appelé groupoïde associé au groupe G.

2) Soit X un ensemble. Soit G le carquois $(X,X\times X$, pr$_1$, pr$_2)$ ; définissons une loi de composition dans G en posant $(x, x')\cdot (x', x'') = (x, x'')$, si $x, x', x''$ sont des éléments de X. Cette loi est associative ; pour tout $x\in X$, $(x, x)$ est l’élément neutre en $x$; l’inverse de la flèche $(x, x')$ est la flèche $(x', x)$. Le groupoïde ainsi défini est appelé groupoïde des couples de l’ensemble X. Si X n’est pas vide, il est simplement transitif.

3) Soient X et S des ensembles et soit $p: X\rightarrow S$ une application. Pour $a\in S$, on note $X_a=\overset{-1}{p}(a)$. Pour $a$ et $b$ dans S, soit $G_{a,b}$ l’ensemble $\mathscr{B}(X_a; X_b)$ des bijections de $X_a$ dans $X_b$ et soit G l’ensemble somme des ensembles $G_{a,b}$. Soient $o$ et $t$ les applications de G dans S telles que $o(f) =a$ et $t(f) =b$ pour tout élément $f\in G_{a,b}$. Le quadruplet $(S,G, o, t)$ est un carquois. Munissons-le de la loi de composition définie par $m(f, g) =g\circ f$ si $f\in \mathscr{B}(X_a; X_b)$ et $g\in \mathscr{B}(X_b; X_c)$, où $a, b, c$ sont des points de S. C’est un groupoïde ; on le note $\mathscr{B}(X, p)$ et on l’appelle le groupoïde des permutations de X relativement à $p$.

4) Soit $(G_i)_{i\in I}$ une famille de groupoïdes. Notons G le carquois produit de la famille des carquois sous-jacents ; pour tout $i\in I$, soit pr$_i: G\rightarrow G_i$ le morphisme de carquois canonique. Il existe une unique loi de composition dans G pour laquelle G est un groupoïde et telle que, pour tout $i\in I$, pr$_i$ soit un morphisme de groupoïdes. Soient $f= (f_i)_{i\in I}$ et $g= (g_i)_{i\in I}$ des flèches de G ; elles sont composables si et seulement si les flèches $f_i$ et $g_i$ sont composables, pour $i\in I$. On a alors $f g= (f_ig_i)_{i\in I}$.

Le carquois G, muni de cette loi de composition, est appelé le groupoïde produit de la famille $(G_i)_{i\in I}$. Il vérifie la propriété universelle suivante : pour tout groupoïde $G'$ et toute famille $(\varphi_i)_{i\in I}$, où $\varphi_i$ est un morphisme de groupoïdes de $G'$ dans $G_i$, il existe un unique morphisme de groupoïdes $\varphi : G'\rightarrow G$ tel que $\varphi_i=$ pr$_i\circ \varphi$ pour tout $i\in I$.

5) Soit $((G_i)_{i\in I},(\varphi_{i,j})_{i\prec j})$ un système inductif de groupoïdes, indexé par un ensemble préordonné filtrant à droite $(I,\prec )$, les $\varphi_{i,j}$ étant des morphismes de groupoïdes. Soit G le carquois dont l’ensemble des sommets est lim$\longrightarrow_i$ Som(G$_i)$, l’ensemble des flèches est lim$\longrightarrow_i$ Fl(G$_i)$, les applications origine et terme étant les applications lim$\longrightarrow_io_{G_i}$ et lim$\longrightarrow_it_{G_i}$ respectivement. Les lois de composition des $G_i$ induisent une loi de composition dans G qui en fait un groupoïde (cf. A, I, p. 114). Les applications canoniques Som(G$_i)\rightarrow$ Som(G) et Fl(G$_i)\rightarrow$ Fl(G) définissent un morphisme de groupoïdes $\varphi_i$ de $G_i$ dans G. Si $i,j$ sont des éléments de I tels que $i\prec j$, on a $\varphi_j\circ \varphi_{i,j}=\varphi_i$. Le groupoïde G est appelé la limite inductive de la famille des groupoïdes $G_i$ et est noté lim$\longrightarrow_iG_i$. Il vérifie la propriété universelle suivante : pour tout groupoïde H et toute famille $(\psi_i)_{i\in I}$, où, pour $i\in I,\psi_i: G_i\rightarrow H$ est un morphisme de groupoïdes, telle que $\psi_j\circ \varphi_{i,j}=\psi_i$ pour tout couple $(i, j)$ d’éléments de I tels que $i\prec j$, il existe un unique morphisme de groupoïdes $\psi : G\rightarrow H$ tel que $\psi_i=\psi \circ \varphi_i$.

Pour l’existence d’un groupoïde vérifiant cette propriété universelle lorsque l’on ne suppose pas que l’ensemble I est filtrant à droite, cf. II, p. 228, exerc. 3.

### 6. Sous-groupoïdes

#### Définition 5 {#ta-ii-s3-def-5 .statement tag=01T6}

Soit C une catégorie. Une sous-catégorie de C est un sous-carquois D de C satisfaisant aux conditions suivantes :

(i) Pour tout sommet $a$ de D$,e_a$ est une flèche de D ;

(ii) Pour tout couple composable $(f, g)$ de flèches de C appartenant à D, le produit $f g$ est une flèche de D;

Soit C une catégorie et soit D une sous-catégorie de D; muni de la loi de composition déduite de celle de C par passage aux sous-ensembles, D est une catégorie.

Tout sous-carquois plein de C est une sous-catégorie de C. L’intersection d’une famille de sous-catégories de C est une sous-catégorie de C.

#### Définition 6 {#ta-ii-s3-def-6 .statement tag=01T7}

Soit G un groupoïde. Un sous-groupoïde de G est une sous-catégorie H de G telle que l’inverse de toute flèche de G appartenant à H soit une flèche de H.

Soit G un groupoïde. Tout sous-groupoïde de G est un groupoïde. Tout sous-carquois plein de G est un sous-groupoïde de G. L’intersection d’une famille de sous-groupoïdes de G est un sous-groupoïde de G.

Soit H un sous-carquois de G. L’intersection des sous-groupoïdes de G dont H est un sous-carquois s’appelle le sous-groupoïde de G engendré par H. L’ensemble de ses sommets est égal à celui de H et ses orbites sont les composantes connexes de H.

#### Exemple 1 {#ta-ii-s3-n6-exa-1 .statement tag=01T8}

Soit X un ensemble ; notons $X\times X$ le groupoïde des couples de X (II, p. 163, exemple 2). Soit R une relation d’équivalence dans X. Le sous-carquois du groupoïde $X\times X$ dont l’ensemble des sommets est X et dont l’ensemble des flèches est le graphe de la relation d’équivalence R est un sous-groupoïde de $X\times X$. Ses orbites sont les classes d’équivalence de la relation R.

Inversement, tout sous-groupoïde de $X\times X$ dont l’ensemble des sommets est X est de cette forme.

Soient X et S des ensembles et soit $p: X\rightarrow$ S une application. L’application $p$ définit une relation d’équivalence dans X (E, II, p. 41). On note $X\times_SX$ le sous-groupoïde de $X\times X$ défini par cette relation d’équivalence et on l’appelle le groupoïde des couples de $(X, p)$.

#### Exemple 2 {#ta-ii-s3-n6-exa-2 .statement tag=01T9}

Soient G et $G'$ des groupoïdes, soient $\varphi$ et $\psi$ des morphismes de groupoïdes de G dans $G'$. L’égalisateur de $\varphi$ et $\psi ($cf. II, p. 153) est un sous-groupoïde de G.

#### Exemple 3 {#ta-ii-s3-n6-exa-3 .statement tag=01TA}

Soient X un ensemble et Γ un groupe. Notons $X\times \Gamma \times X$ le carquois dont l’ensemble des sommets est X, l’ensemble des flèches est $X\times \Gamma \times X$, les applications origine et terme étant respectivement pr$_1$ et pr$_3$. Muni de la loi de composition $(x, \gamma , x')\cdot (x', \gamma ', x'') = (x, \gamma \gamma ', x'')$, c’est un groupoïde. C’est d’ailleurs le groupoïde déduit par transport de structure du groupoïde $(X\times X)\times \Gamma$, produit du groupoïde des couples $X\times X$ et du groupoïde associé au groupe Γ (II, p. 163, exemple 1), au moyen de la bijection $(x, x', \gamma )\mapsto (x, \gamma , x')$ de $X\times X\times \Gamma$ dans $X\times \Gamma \times X$.

Soit $m: X\times \Gamma \rightarrow X$ une opération (à droite) du groupe Γ sur X. Le graphe F de l’application $m$, c’est-à-dire l’ensemble des triplets $(x, \gamma , x')\in X\times \Gamma \times X$ tels que $x'=x\gamma$, est l’ensemble des flèches d’un unique sous-groupoïde G de $X\times \Gamma \times X$. Les orbites de ce groupoïde sont les orbites de Γ dans X ; si $x\in X$, le groupe d’isotropie de G en $x$ est l’ensemble des $(x, \gamma , x)$, où $\gamma$ décrit le fixateur de $x$ dans Γ.

Inversement, tout sous-groupoïde G du groupoïde $X\times \Gamma \times X$ tel que l’application (pr$_1$, pr$_2)$ de Fl(G) dans $X\times \Gamma$ soit une bijection est de cette forme.

#### Exemple 4 {#ta-ii-s3-n6-exa-4 .statement tag=01TB}

Soit G un groupoïde, soit X un ensemble et soit $\varphi : X\rightarrow$ Som(G) une application. Définissons un carquois $G'$ de la façon suivante. L’ensemble Som(G$')$ est l’ensemble X ; pour tout couple $(x, y)$ d’éléments de X, l’ensemble Fl$_{x,y}(G')$ est l’ensemble des triplets $(x, f, y)\in X\times$ Fl(G) $\times X$, où $f$ est un élément de Fl$_{\varphi(x),\varphi(y)}(G)$. Soient $x,y,z$ des éléments de X$,f\in$ Fl$_{\varphi(x),\varphi(y)}(G)$ et $g\in$ Fl$_{\varphi(y),\varphi(z)}(G)$ des flèches de G, on pose $(x, f, y)\cdot (y, g, z) = (x, f g, z)$. Cela définit une loi de composition dans le carquois $G'$ qui en fait un groupoïde. On l’appelle groupoïde image réciproque du groupoïde G par l’application $\varphi$ et on le note $\varphi^*(G)$.

Le couple $(\varphi , \psi )$, où $\psi :$ Fl($\varphi^*(G)$)$\rightarrow$ Fl(G) est l’application définie par $(x, f, y)\mapsto f$ est un morphisme de groupoïdes de $\varphi^*(G)$ dans G, appelé morphisme canonique.

#### Exemple 5 {#ta-ii-s3-n6-exa-5 .statement tag=01TC}

Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes. Soit H le sous-carquois de G d’ensemble de sommets Som(G) et dont l’ensemble des flèches est formé des $f\in$ Fl(G) tels que $\varphi (f)$ soit un élément neutre de $G'$. Pour tout $a\in$ Som(G)$,e_a\in H_{a,a}$. Pour tout $f\in$ Fl(H), $\varphi (f^{-1}) =\varphi (f)^{-1}$ donc $f^{-1}\in$ Fl(H). De plus, si $f$ et $g$ sont des flèches composables de H, on a $\varphi (f g) =\varphi (f)\varphi (g) =e_{t(\varphi(f))}e_{o(\varphi(g))}=$ $e_{t(\varphi(f))}$, donc $f g$ est une flèche de H. Cela démontre que H est un sous-groupoïde de G. On l’appelle le noyau de $\varphi$ et on le note Ker($\varphi$ ).

#### Exemple 6 {#ta-ii-s3-n6-exa-6 .statement tag=01TD}

Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes. Le carquois $\varphi (G)$ dont l’ensemble des sommets est $\varphi$(Som(G)) et dont l’ensemble des flèches est $\varphi$(Fl(G)) n’est en général pas un sous-groupoïde de $G'$. C’est néanmoins le cas si l’application Som($\varphi$ ) est injective (II, p. 225, exerc. 5).

### 7. Opérations d’un groupoïde

Soit G un groupoïde ; notons S l’ensemble de ses sommets. Soit X un ensemble et soit $p: X\rightarrow S$ une application. Une opération (à droite) $\varphi$ du groupoïde G sur l’ensemble X, relativement à $p$, est un morphisme de groupoïdes $\varphi$ de G dans le groupoïde $\mathscr{B}(X, p)$ des permutations de l’ensemble X relativement à $p($II, p. 163) qui induit l’identité sur l’ensemble des sommets. En d’autres termes, $\varphi$ est la donnée, pour tout couple $(a, b)$ de points de S et pour toute flèche $g\in G$ reliant $a$ à $b$, d’une application $\varphi (g): X_a\rightarrow X_b$, telle que l’on ait, pour tout couple $(f, g)$ de flèches composables de G,

$$
\varphi (f g) =\varphi (g)\circ \varphi (f)
$$

et telle que, pour tout $a\in S,\varphi (e_a)$ soit l’identité de $X_a$.

Soient $\varphi$ et $\varphi '$ des opérations du groupoïde G sur un ensemble X, relativement à une application $p: X\rightarrow S$. Pour que l’on ait $\varphi =\varphi '$, il suffit qu’il existe un sous-carquois H de G, engendrant G, tel que $\varphi (f) =\varphi '(f)$ pour tout $f\in$ Fl(H). En effet, l’ensemble des flèches $f$ de G telles que $\varphi (f) =\varphi '(f)$ est l’ensemble des flèches d’un sous-groupoïde de G, d’ensemble de sommets S.

Soit G un groupoïde d’ensemble de sommets S, soit X un ensemble, soit $p: X\rightarrow S$ une application et soit $\varphi$ une opération de G sur X relativement à $p$. Soit $G_{\varphi}$ le sous-carquois de $p^*(G)$ dont l’ensemble des sommets est X et dont l’ensemble des flèches est l’ensemble des triplets $(x, f, y)\in X\times$ Fl(G) $\times X$ tels que $\varphi (f)(x) =y$. C’est un sous-groupoïde de $p^*(G)$.

Inversement, soit Γ un sous-groupoïde de $p^*(G)$; supposons que l’application $(x, f, y)\mapsto (x, f)$ de Fl(Γ) dans $X\times$ Fl(G) soit injective et que son image soit l’ensemble des couples $(x, f)$ tels que $p(x) =o(f)$. Il existe alors une unique opération $\varphi$ du groupoïde G sur X telle que l’on ait $\Gamma  = G_{\varphi}$.

Les orbites du groupoïde $G_{\varphi}$ s’appellent les orbites de l’opération de G sur X. Par définition, ce sont les classes d’équivalence de la relation dans X donnée par $R\{x, y\}$ si et et seulement s’il existe $f\in$ Fl(G) telle que $\varphi (f)(x) =y$.

#### Exemple 1 {#ta-ii-s3-n7-exa-1 .statement tag=01TE}

Soit G un groupe, soit $\mathscr{G}$ le groupoïde associé à G (II, p. 163, exemple 1). Si X est un ensemble, une opération (à droite) du groupoïde $\mathscr{G}$ sur X n’est autre qu’une opération (à droite) du groupe G sur X. En outre, les orbites de l’opération de $\mathscr{G}$ coïncident avec celles du groupe G.

#### Exemple 2 {#ta-ii-s3-n7-exa-2 .statement tag=01TF}

Soit $G = (S,F, o, t)$ un groupoïde. Il existe une unique opération de G sur l’ensemble S, relativement à Id$_S$. Elle est donnée par $\varphi (f)(a) =b$ si $f\in G_{a,b}$. Les orbites pour cette opération sont les orbites de G au sens défini p. 162.

Soit G un groupoïde, soit S l’ensemble de ses sommets, soit X un ensemble et soit $p: X\rightarrow S$ une application. Soit $\varphi$ une opération de G sur X relativement à $p$. On dit que le groupoïde G opère sans monodromie sur X, si pour tout point $a\in S$ et tout élément $f\in G_a,\varphi (f)$ est l’identité de $X_a$. Si le groupoïde G est transitif, il suffit qu’il en soit ainsi pour un point de S.

Soit $a$ un point de S et supposons que l’on ait $\varphi (f) =$ Id$_{X_a}$ pour tout $f\in G_a$. Soit $b$ un point de S appartenant à l’orbite de $a$ et soit $g$ une flèche de G reliant $a$ à $b$. Pour tout $f\in G_b$, Int($g$)$(f) =gf g^{-1}$ est un élément de $G_a$; on a donc Id$_{X_a}=\varphi (gf g^{-1}) =\varphi (g)\varphi (f)\varphi (g)^{-1}$, si bien que $\varphi (f) =$ Id$_{X_b}$. Soit $b$ un point de S appartenant à l’orbite de $a$ et soient $g,g'$ des flèches de G reliant $a$ à $b$; alors $g'g^{-1}$ est un lacet en $a$, d’où $\varphi (g'g^{-1}) =$ Id$_{X_a}$ et $\varphi (g) =\varphi (g')$.

### 8. Sous-groupoïdes distingués ; quotients de groupoïdes

#### Définition 7 {#ta-ii-s3-def-7 .statement tag=01TG}

Soit G un groupoïde. On dit qu’un sous-groupoïde H de G est distingué si Som(H) = Som(G) et si pour tout couple $(a, b)$ de sommets de H et toute flèche $f\in G_{a,b}$, on a Int($f$)$(H_b) = H_a$.

Soit G un groupoïde et soit H un sous-groupoïde de G dont l’ensemble des sommets est égal à Som(G). Pour vérifier que H est distingué, il suffit de démontrer que $fH_bf^{-1}\subset H_a$ pour tout $a\in$ Som(G), tout $b\in$ Som(G) et tout $f\in G_{a,b}$. En effet, s’il en est ainsi, on a aussi $f^{-1}H_af\subset H_b$ pour toute flèche $f\in G_{b,a}$, c’est-à-dire $H_a\subset fH_bf^{-1}$, et, par suite, $fH_bf^{-1}= H_a$.

Soit G un groupoïde et soit H un sous-groupoïde distingué de G. Pour tout sommet $a$ de G, le sous-groupe $H_a$ de $G_a$ est un sous-groupe distingué de $G_a$.

Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes. Le noyau de $\varphi ($II, p. 166, exemple 5) est un sous-groupoïde distingué de G. En effet, soit $f$ une flèche dans G reliant $a$ à $b$ et soit $g\in$ Ker($\varphi$ )$_b$; on a alors $\varphi (f gf^{-1}) =\varphi (f)\varphi (g)\varphi (f^{-1}) =\varphi (f)e_{\varphi(b)}\varphi (f)^{-1}=e_{\varphi(a)}$, d’où l’inclusion $f$Ker($\varphi$ )$_bf^{-1}\subset$ Ker($\varphi$ )$_a$.

Soit G un groupoïde. Le groupoïde G et le sous-groupoïde de G dont l’ensemble des flèches est l’ensemble des éléments neutres de G sont des sous-groupoïdes distingués de G. L’intersection d’une famille de sous-groupoïdes distingués de G est un sous-groupoïde distingué de G. En particulier, pour toute partie $F\subset$ Fl(G), il existe un plus petit sous-groupoïde distingué de G dont l’ensemble des flèches contient F. On l’appelle le sous-groupoïde distingué engendré par F.

Soit H un sous-groupoïde distingué de G. Soit $\mathscr{R}$ la relation d’équivalence dans Fl(G) définie par $\mathscr{R}\{f, g\}$ si et seulement s’il existe des flèches $x$ et $y$ dans Fl(H) telles que $f=xgy$. Si $f$ et $g$ sont des flèches de G équivalentes modulo $\mathscr{R}$, leurs origines (resp. leurs termes) appartiennent à la même orbite de H. Posons $F'=$ Fl(G)$/\mathscr{R}$ et notons $o'$ et $t'$ les applications de $F'$ dans Orb(H) déduites de $o$ et $t$ par passage aux quotients. Notons $G/H$ le carquois (Orb(H)$,F', o', t')$.

#### Lemme {#ta-ii-s3-n8-lem-1 .statement tag=01TH}

Étant données des flèches composables $u$ et $v$ de $G/H$, on peut choisir des représentants $f$ et $g$ de $u$ et $v$ dans Fl(G) qui soient composables. La classe modulo $\mathscr{R}$ du produit $f g$ ne dépend pas du choix de $f$ et $g$.

Soient $f$ et $g$ des représentants arbitraires de $u$ et $v$ dans Fl(G). Le terme de $f$ et l’origine de $g$ appartiennent à une même orbite de H, donc peuvent être reliées par une flèche $x$ de H (II, p. 162, prop. 1). Les flèches $f x$ et $g$ sont alors des représentants de $u$ et $v$ dans F qui sont composables dans G. Cela prouve la première assertion.

Soient maintenant $f,g$ d’une part, et $f',g'$ d’autre part, des représentants de $u$ et $v$ qui sont composables dans G. Par hypothèse, il existe des flèches $x,y,z,t$ dans H telles que l’on ait $f'=xf y$ et $g'=zgt$. On a alors $yz\in H_{t(f)}$ et $f'g'=xf yzgt=xf(yz)f^{-1}f gt$. Comme H est un sous-groupoïde distingué de G, la flèche $f(yz)f^{-1}$ est une flèche de H. Il en est donc de même de la flèche $xf(yz)f^{-1}$, ce qui démontre que $f'g'$ et $f g$ sont équivalentes modulo $\mathscr{R}$.

En vertu de ce lemme, il existe une unique loi de composition $m$ dans le carquois $G/H$ telle que, pour tout couple $(u, v)$ de flèches composables, $m(u, v)$ soit la classe modulo $\mathscr{R}$ du produit $f g$, pour tout couple $(f, g)$ de flèches composables de G tel que $u$ soit la classe de $f$ et $v$ celle de $g$. Muni de cette loi de composition, $G/H$ est un groupoïde. Soient $p_1:$ Som(G) $\rightarrow$ Som(G$/H)$ et $p_2:$ Fl(G) $\rightarrow$ Fl(G$/H)$ les surjections canoniques. Le couple $p= (p_1, p_2)$, est un morphisme de groupoïdes de G dans $G/H$ dont le noyau est le sous-groupoïde distingué H.

#### Définition 8 {#ta-ii-s3-def-8 .statement tag=01TI}

On dit que $G/H$ est le groupoïde quotient de G par H et que $p: G\rightarrow G/H$ est le morphisme canonique.

#### Remarque 1 {#ta-ii-s3-n8-rem-1 .statement tag=01TJ}

L’application Som($p$) définit, par passage aux quotients, une bijection de l’ensemble des orbites de G sur l’ensemble des orbites de $G/H$. En particulier, G est transitif si et seulement si $G/H$ l’est.

#### Remarque 2 {#ta-ii-s3-n8-rem-2 .statement tag=01TK}

Soient $a$ et $b$ des sommets de G. L’application de $G_{a,b}$ dans $(G/H)_{p(a),p(b)}$ déduite de $p$ est surjective. Soit en effet $u$ une flèche de $G/H$ reliant $p(a)$ à $p(b)$ ; c’est la classe modulo $\mathscr{R}$ d’une flèche $f$ de G. L’origine $o(f)$ de $f$ appartient à l’orbite de $a$ dans H ; il existe donc une flèche $x$ dans H reliant $a$ à $o(f)$. De même, il existe une flèche $y$ dans H qui relie $t(f)$ à $b$. Alors, $f'=xf y$ est un élement de $G_{a,b}$ dont la classe modulo $\mathscr{R}$ est $u$.

#### Proposition 2 {#ta-ii-s3-prop-2 .statement tag=01TL}

Soit $a$ un sommet de G. L’homomorphisme de groupes $p_a: G_a\rightarrow (G/H)_{p(a)}$ déduit de $p$ par passage aux groupes d’isotropie est surjectif ; son noyau est $H_a$.

L’homomorphisme $p_a$ est surjectif en vertu de la remarque précédente. Son noyau contient $H_a$ par construction du groupoïde $G/H$. Soit $f$ un élément de $G_a$ tel que $p_a(f) =e_{p(a)}$. Cela signifie que $f$ et $e_a$ sont équivalents modulo $\mathscr{R}$; il existe alors des flèches $x$ et $y$ de H telles que $f=xe_ay$. Nécessairement, $x$ et $y$ appartiennent à $H_a$, d’où $f\in H_a$.

#### Proposition 3 {#ta-ii-s3-prop-3 .statement tag=01TM}

Soit G un groupoïde, soit H un sous-groupoïde distingué de G et soit $p: G\rightarrow G/H$ le morphisme canonique. Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes tel que $H\subset$ Ker($\varphi$ ). Il existe un unique morphisme de groupoïdes $\overline{\varphi}: G/H\rightarrow G'$ tel que $\overline{\varphi}\circ p=\varphi$.

On dit que $\overline{\varphi}$ est le morphisme de groupoïdes déduit de $\varphi$ par passage au quotient.

L’unicité d’un tel morphisme est évidente, car les applications Som($p$) et Fl($p$) sont surjectives.

Soient $a$ et $b$ des sommets de G. S’ils sont dans la même orbite de H, il existe une flèche $f$ reliant $a$ à $b$ dans H et l’on a $\varphi (f) =e_{\varphi(a)}$. En particulier, $\varphi (a) =\varphi (b)$. Par suite, l’application Som($\varphi$ ) définit, par passage au quotient, une application $\overline{\varphi}_1:$ Orb(H) $\rightarrow$ Som(G$')$. Soient $f$ et $g$ des flèches dans G. Si $f$ et $g$ sont équivalentes modulo $\mathscr{R}$, il existe des flèches $x$ et $y$ dans H telles que $f$ = $xgy$. Par suite, $\varphi (f) =\varphi (x)\varphi (g)\varphi (y) =\varphi (g)$ puisque $\varphi (x)$ et $\varphi (y)$ sont des éléments neutres. L’application Fl($\varphi$ ) définit donc, par passage au quotient, une application $\overline{\varphi}_2:$ Fl(G)$/\mathscr{R}\rightarrow$ Fl(G$')$.

Soient $f$ et $g$ des flèches de G qui sont composables ; notons $u$ et $v$ leurs classes dans Fl(G$/H)$. On a $\overline{\varphi}_2(uv) =\varphi (f g) =\varphi (f)\varphi (g) =$ $\overline{\varphi}_2(u)\overline{\varphi}_2(v)$.

Le couple $\overline{\varphi}= (\overline{\varphi}_1, \varphi_2)$ est un morphisme de groupoïdes de $G/H$ dans $G'$ et l’on a $\overline{\varphi}\circ p=\varphi$.

### 9. Groupoïde des classes de chemins d’un graphe

Soit G un graphe. Notons $\Omega_G$ la catégorie des chemins du carquois sous-jacent à G (II, p. 160, exemple 1). Considérons la relation d’équivalence $\mathscr{R}$ la plus fine dans Ch(G) telle que l’on ait :

(i) Pour tout couple $(a, b)$ de sommets de G et toute flèche $f$ dans G reliant $a$ à $b$, les chemins $(a, f, b, f , a)$ et $e_a$ sont équivalents modulo $\mathscr{R}$;

(ii) Si $(c, d)$ et $(c', d')$ sont des couples de chemins juxtaposables dans G tels que $\mathscr{R}\{c, c'\}$ et $\mathscr{R}\{d, d'\}$, les chemins $c*d$ et $c'*d'$ sont équivalents modulo $\mathscr{R}$.

Deux chemins équivalents modulo $\mathscr{R}$ ont même origine et même terme. Les applications $o$ et $t$ de Ch(G) dans Som(G) définissent, par passage au quotient, des applications $o'$ et $t'$ de Ch(G)$/\mathscr{R}$ dans Som(G). Notons $\varpi_G$ le carquois (Som(G), Ch(G)$/\mathscr{R}, o', t')$. Le couple $\varphi$ formé de l’identité de Som(G) et de la projection canonique de Ch(G) sur Ch(G)$/\mathscr{R}$ est un morphisme de carquois de $\Omega_G$ dans $\varpi_G$. La juxtaposition des chemins dans Ch(G) définit, par passage aux quotients, une loi de composition dans $\varpi_G$.

#### Proposition 4 {#ta-ii-s3-prop-4 .statement tag=01TN}

Muni de cette loi de composition, $\varpi_G$ est un groupoïde.

Par construction, on a la relation $\varphi (cc') =\varphi (c)\varphi (c')$, pour tout couple de chemins $(c, c')$ juxtaposables dans G. Toute flèche de $\varpi_G$ est de la forme $\varphi (c)$, où $c$ est un chemin dans G. Cela entraîne que la loi de composition de $\varpi_G$ est associative et que $\varphi (e_a)$ est un élément neutre en $a$, pour tout sommet $a$ de $\varpi_G$. Il reste à démontrer que toute flèche de $\varpi_G$ est inversible. Soit $c$ un chemin dans G et démontrons par récurrence sur la longueur de $c$ que l’on a $\varphi (c)\varphi (\overline{c}) =\varphi (e_{o(c)})$. Cette égalité est vraie si $c$ est de longueur 0. Si $c$ est de longueur $n\geqslant 1$, on peut écrire $c=c_1c_2$, avec $c_1$ de longueur 1 et $c_2$ de longueur $n-1$. Alors, $\overline{c}=\overline{c_2}\overline{c_1}$ et l’on a

$$
\varphi (c)\varphi (\overline{c}) =\varphi (c_1)\varphi (c_2)\varphi (\overline{c_2})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (e_{o(c_2)})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (\overline{c_1})
$$

$$
=\varphi (c_1\overline{c_1}) =\varphi (e_{o(c_1)})
$$

par définition de la relation $\mathscr{R}$.

En appliquant cette égalité au chemin $\overline{c}$, on voit que $\varphi (\overline{c})\varphi (c) =$ $\varphi (e_{t(c)})$. Ainsi, $\varphi (c)$ est inversible, d’inverse $\varphi (\overline{c})$.

Les classes d’équivalence de la relation $\mathscr{R}$ s’appellent les classes de chemins dans le graphe G ; le groupoïde $\varpi_G$ s’appelle le groupoïde des classes de chemins du graphe G. Il a même ensemble de sommets que G et ses orbites sont les composantes connexes du graphe G.

Notons $v$ l’application qui, à une flèche $f$ de G, associe la classe du chemin $(o(f), f, t(f))$ de G. Le couple $j$ = (Id$_{Som(G)}, v)$ est un morphisme, dit canonique, de carquois de G dans $\varpi_G$. Son image engendre $\varpi_G$; pour toute flèche $f$ de G, on a $j(\overline{f}) =j(f)^{-1}$.

Soient G et $G'$ des graphes, soit $\varphi : G\rightarrow G'$ un morphisme de graphes. Notons $j: G\rightarrow \varpi_G$ et $j': G'\rightarrow \varpi_{G'}$ les morphismes canoniques. Si $c= (a_0, f_1, a_1, . . . , a_n)$ est un chemin dans G, la classe du chemin $\varphi (c) = (\varphi (a_0), \varphi (f_1), \varphi (a_1), . . . , \varphi (a_n))$ ne dépend que de la classe de $c$. On définit ainsi par passage aux classes d’équivalence un morphisme de carquois $\varpi (\varphi ):\varpi_G\rightarrow \varpi_{G'}$ tel que $\varpi (\varphi )\circ j=j'\circ \varphi$. C’est un morphisme de groupoïdes.

#### Proposition 5 {#ta-ii-s3-prop-5 .statement tag=01TO}

Soit G un graphe ; notons $j$ le morphisme canonique de carquois de G dans $\varpi_G$. Soit $\varphi$ un morphisme de carquois de G dans un groupoïde $G'$ tel que $\varphi (\overline{f}) =\varphi (f)^{-1}$ pour toute flèche $f$ de G. Il existe alors un unique morphisme de groupoïdes $\varphi '$ de $\varpi_G$ dans $G'$ tel que $\varphi '\circ j=\varphi$.

On définit une application $u:$ Ch(G) $\rightarrow$ Fl(G$')$ en posant, pour tout chemin $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ dans G$,u(c) =e_{a_0}\varphi (f_1). . . \varphi (f_n)$. Pour tout couple $(c, c')$ de chemins juxtaposables dans G, on a $u(cc') =$ $u(c)u(c')$. L’application $u$ est compatible avec la relation d’équivalence $\mathscr{R}$ définie ci-dessus, d’où, par passage au quotient, une application $u':$ Ch(G)$/\mathscr{R}\rightarrow$ Fl(G$')$. Posons alors $\varphi '=$ (Som($\varphi$ )$, u')$. C’est un morphisme de groupoïdes de $\varpi_G$ dans $G'$ tel que $\varphi '\circ j=\varphi$.

Soit $\psi$ un morphisme de groupoïdes de $\varpi_G$ dans $G'$ tel que $\psi \circ j=\varphi$. L’égalisateur de $\varphi '$ et $\psi$ est un sous-groupoïde de $\varpi_G$ qui contient $j(G)$. Il est donc égal à $\varpi_G$, car $\varpi_G$ est engendré par $j(G)$, et l’on a $\psi =\varphi '$.

#### Corollaire 1 {#ta-ii-s3-prop-5-cor-1 .statement tag=01TP}

Dans un graphe, toute classe de chemins contient un unique chemin sans aller-retour.

Soit G un graphe. Notons $j: G\rightarrow \varpi_G$ le morphisme de carquois canonique.

L’existence, pour tout chemin $c$ de G, d’un chemin équivalent qui soit sans aller-retour est immédiate par récurrence sur la longueur de $c$ (cf. II, p. 157).

Soit A une orientation de G et soit $G'$ le groupoïde associé au groupe libre F(A) construit sur A (II, p. 163, exemple 1). Soit $\psi$ le morphisme de carquois de G dans $G'$ tel que, pour tout $f\in A,\psi (f)$ soit l’élément $f$ de F(A) et $\psi (\overline{f})$ soit l’élément $f^{-1}$ de F(A). Soit $\psi '$ l’unique morphisme de groupoïdes de $\varpi_G$ dans $G'$ tel que $\psi '\circ j=\psi$.

Soient $c,c'$ des chemins sans aller-retour équivalents modulo $\mathscr{R}$. Ils ont même source et même but. Pour démontrer qu’ils sont égaux, il suffit de démontrer que les suites $(f_1, . . . , f_n)$ et $(g_1, . . . , g_m)$ de leurs flèches sont égales. L’image par $\psi '$ de la classe commune de $c$ et $c'$ est égale à $\psi (f_1). . . \psi (f_n)$ et à $\psi (g_1). . . \psi (g_m)$. Or les termes des suites $(\psi (f_1), . . . , \psi (f_n))$ et $(\psi (g_1), . . . , \psi (g_m))$ appartiennent au sous-ensemble $A\cup A^{-1}$ de F(A) et deux éléments consécutifs de ces suites ne sont pas inverses l’un de l’autre. D’après A, I, p. 84, prop. 7, ces deux suites sont égales. Il en résulte que les suites $(f_1, . . . , f_n)$ et $(g_1, . . . , g_m)$ sont égales, et donc que $c=c'$, d’où l’unicité.

#### Corollaire 2 {#ta-ii-s3-prop-5-cor-2 .statement tag=01TQ}

Le morphisme canonique de G dans $\varpi_G$ est injectif.

Cela résulte aussitôt du corollaire 1.

#### Corollaire 3 {#ta-ii-s3-prop-5-cor-3 .statement tag=01TR}

Soit $G'$ un sous-graphe de G. Le morphisme de $\varpi_{G'}$ dans $\varpi_G$ déduit de l’injection de $G'$ dans G est injectif.

Notons $i$ le morphisme d’inclusion de $G'$ dans G et $\varpi (i)$ le morphisme de $\varpi_{G'}$ dans $\varpi_G$ qui s’en déduit. Les applications Som($i$) et Som($\varpi (i)$) coïncident. En outre, si $c$ est un chemin sans aller-retour dans $G'$, le chemin $i(c)$ est un chemin sans aller-retour dans G. L’assertion résulte donc du corollaire 1.

#### Corollaire 4 {#ta-ii-s3-prop-5-cor-4 .statement tag=01TS}

Un graphe non vide G est un arbre si et seulement si le groupoïde $\varpi_G$ est simplement transitif.

Soit $a$ un point de G. D’après le corollaire 1, les propriétés suivantes sont équivalentes :

(i) Le groupe d’isotropie de $\varpi_G$ en $a$ est réduit à l’élément neutre ;

(ii) Le seul lacet de G d’origine $a$ qui soit sans aller-retour est le lacet constant d’origine $a$.

Le groupoïde $\varpi_G$ est simplement transitif si et seulement s’il est transitif et s’il possède la propriété (i) pour tout $a$. Le graphe G est un arbre si et seulement s’il est connexe et possède la propriété (ii) pour tout point $a$. Comme les orbites de $\varpi_G$ s’identifient aux composantes connexes de G, le corollaire en résulte.

### 10. Groupoïdes libres

#### Définition 9 {#ta-ii-s3-def-9 .statement tag=01TT}

Soit C un carquois. On appelle groupoïde libre construit sur C, et on note Grp(C), le groupoïde $\varpi_{\widetilde{C}}$ des classes de chemins du graphe $\widetilde{C}$ associé à C.

L’ensemble des sommets de Grp(C) est égal à celui des sommets de C; les orbites de Grp(C) sont les composantes connexes de C.

Soit C un carquois non vide. D’après le corollaire 4, p. 174, le graphe $\widetilde{C}$ associé à C est un arbre si et seulement si le groupoïde libre Grp(C) construit sur C est simplement transitif.

Le composé des morphismes de carquois canoniques $i: C\rightarrow \widetilde{C}$ et $j:\widetilde{C}\rightarrow \varpi_C$ est un morphisme de carquois de C dans Grp(C) qu’on appelle l$\widetilde{e}$ morphisme canonique de C dans Grp(C). Notons-le $\theta$. Pour tout sommet $a$ de C, on a $\theta (a) =a$. Si $f$ est une flèche de C$,\theta (f)$ est la classe du chemin $(o(f),(f,1), t(f))$ de $\widetilde{C}$. Le morphisme $\theta$ est injectif (II, p. 174, cor. 2) et son image engendre le groupoïde Grp(C).

Soit $\varphi : C\rightarrow C'$ un morphisme de carquois. Notons $\theta_C$ (resp. $\theta_{C'})$ le morphisme canonique de C dans Grp(C) (resp. de $C'$ dans Grp(C$')$). Le morphisme $\varpi (\widetilde{\varphi})$ est l’unique morphisme de groupoïdes $\psi$ de Grp(C) dans Grp(C$')$ tel que $\psi \circ \theta_C=\theta_{C'}\circ \varphi$.

#### Proposition 6 {#ta-ii-s3-prop-6 .statement tag=01TU}

Soit C un carquois, soit G un groupoïde et soit $\varphi$ un morphisme de carquois de C dans G. Il existe un unique morphisme de groupoïdes $\varphi '$ de Grp(C) dans G tel que $\varphi '\circ \theta_C=\varphi$.

Soit $\psi$ le morphisme de carquois de $\widetilde{C}$ dans G tel que $\psi (a) =\varphi (a)$ pour tout sommet $a$ de C et $\psi (f, \varepsilon ) =\varphi (f)^{\varepsilon}$ pour toute flèche $f$ de C et tout $\varepsilon \in  \{-1,1\}$. On a $\psi \circ i=\varphi$. D’après la proposition 5, p. 173, il existe un morphisme $\varphi '$ de Grp(C) $=\varpi_C$ dans G tel que $\varphi '\circ j=\psi$. On a alors $\varphi '\circ \theta_C=\varphi '\circ j\circ i=\psi \circ i\widetilde{=}\varphi$. Comme dans la démonstration de la prop. 5, l’unicité de $\varphi '$ résulte de ce que $\theta_C(C)$ engendre le groupoïde Grp(C).

Sous les hypothèses de la prop. 6, on dit parfois que $\varphi '$ est le morphisme de groupoïdes de Grp(C) dans G prolongeant le morphisme de carquois $\varphi$.

#### Exemple {#ta-ii-s3-n10-exa-1 .statement tag=01TV}

Soit C un carquois ayant un unique sommet $s$ et soit A l’ensemble de ses flèches. Le groupoïde Grp(C) est alors le groupoïde associé au groupe libre F(A) construit sur A. En effet, il possède un unique sommet $s$ et il résulte immédiatement de la prop. 6 que l’application canonique de A dans Grp(C)$_s$ déduite du morphisme canonique de C dans Grp(C) vérifie la propriété universelle des groupes libres (A, I, p. 85, prop. 8).

### 11. Contraction de flèches d’un groupoïde

Soit G un groupoïde et soit F une partie de l’ensemble des flèches de G. Soit H le sous-groupoïde distingué de G engendré par F. Le groupoïde $G/H$ est appelé groupoïde déduit de G par contraction de l’ensemble de flèches F et est noté $G/F$. Si $p$ désigne le morphisme canonique de G dans $G/F$, on a $p(o(f)) =p(t(f))$ et $p(f) =e_{p(o(f))}$ pour toute flèche $f\in F$.

Ce morphisme vérifie la propriété universelle suivante.

#### Proposition 7 {#ta-ii-s3-prop-7 .statement tag=01TW}

Pour tout morphisme de groupoïdes $\varphi : G\rightarrow G'$ qui applique toute flèche appartenant à F sur un élément neutre de $G'$, il existe un unique morphisme de groupoïdes $\varphi ': G/F\rightarrow G'$ tel que $\varphi '\circ p=\varphi$.

Le noyau de $\varphi$ est un sous-groupoïde distingué de G et l’ensemble de ses flèches contient F. Par définition, H est le plus petit sous-groupoïde distingué de G dont l’ensemble des flèches contient F; il est donc contenu dans le noyau de $\varphi$. La proposition résulte alors de II, p. 170, prop. 3.

Notons Γ le sous-carquois de G d’ensemble de sommets Som(G) et d’ensemble de flèches F. Les orbites de H s’identifient aux composantes connexes du carquois Γ. Par définition du quotient d’un groupoïde par un sous-groupoïde distingué, l’ensemble des sommets de $G/F$ s’identifie à l’ensemble des composantes connexes de Γ ; autrement dit, c’est l’ensemble quotient de Som(G) par la relation d’équivalence la plus fine telle que $o(f)$ soit équivalent à $t(f)$ pour toute flèche $f\in F$.

L’application $p$ induit, par passage aux quotients, une bijection de l’ensemble des orbites de G sur l’ensemble des orbites de $G/F$ (II, p. 170, remarque 1).

Le but de ce n$^o$ est de calculer les homomorphismes déduits de $p$ par passage aux groupes d’isotropie, ce qui revient, d’après la prop. 2 (II, p. 170), à calculer les groupes d’isotropie du sous-groupoïde H.

#### Proposition 8 {#ta-ii-s3-prop-8 .statement tag=01TX}

Soit $\delta$ le morphisme canonique du groupoïde libre Grp(Γ) dans G qui prolonge le morphisme injectif canonique de Γ dans G. Soit $a$ un sommet de G et soit A l’orbite de $a$ dans G. Pour tout $b\in A$, soit $f_{ab}$ une flèche de G reliant $a$ à $b$. Le groupe d’isotropie $H_a$ est le sous-groupe distingué de $G_a$ engendré par les éléments Int($f_{ab}$)$(\delta (c))$, où $b$ parcourt l’ensemble A et $c$ parcourt les éléments de Grp(Γ)$_b$.

Si $x$ et $y$ sont des sommets de G appartenant à la même orbite, avec $x=\not a$, fixons en outre une flèche $f_{xy}$ de G qui relie $x$ à $y$. Pour tout point $x$ de G, soit $N_x$ le sous-groupe distingué de $G_x$ engendré par les éléments Int($f_{xy}$)$(\delta (c))$, où $y$ parcourt l’orbite de $x$ dans G et $c$ parcourt le groupe Grp(Γ)$_y$. Pour tout $f\in G_{xy}$ et tout $g\in N_y$, on a $f gf^{-1}\in N_x$. Soit $x\in$ Som(G). On a $\delta$(Grp(Γ)$_x)\subset N_x$, par définition de $N_x$. Par définition du groupoïde H$,\delta (f)$ est une flèche de H pour toute flèche $f$ de Grp(Γ) ; par suite, $\delta$(Grp(Γ)$_x)$ est contenu dans $H_x$. Comme H est un sous-groupoïde distingué de G, on a alors

Int($f_{xy}$)$(\delta (c))\in$ Int($f_{xy}$)$(N_y)\subset$ Int($f_{xy}$)$(H_y)\subset H_x$

pour tout $y\in$ Som(G), puis $N_x\subset H_x$.

Soient $x$ et $y$ des sommets de Γ. Posons $N_{x,y}=\emptyset$ si $x$ et $y$ n’appartiennent pas à une même composante connexe de Γ. Dans le cas contraire, soient $c$ et $c'$ des classes de chemins reliant $x$ à $y$ dans le graphe $\widetilde{\Gamma}$ associé à Γ. Soit $z$ un sommet de G appartenant à l’orbite de $y$ et soit $\ell$ un élément de Grp(Γ)$_z$; dans le groupe $G_x$, on a l’égalité :

$$
\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}
$$

$$
=\delta (c)f_{yz}f_{xz}^{-1}f_{xz}\delta (\ell )f_{xz}^{-1}f_{xz}f_{yz}^{-1}\delta (c)^{-1}\delta (c(c')^{-1})
$$

La flèche $\delta (c(c')^{-1})$ est la classe d’un lacet en $x$ dans le carquois Γ, donc appartient à $N_x$, de même que la flèche $f_{xz}\delta (\ell )f_{xz}^{-1}$. Comme $\delta (c)f_{yz}f_{xz}^{-1}$ appartient à $G_x$ et que $N_x$ est un sous-groupe distingué de $G_x$, il en résulte que $\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}$ appartient à $N_x$. Par conséquent, $\delta (c)N_y\subset N_x\delta (c')$. Par symétrie, on a $\delta (c)N_y= N_x\delta (c')$. Cela entraîne que cet ensemble ne dépend pas des choix de $c$ et $c'$; on le note $N_{x,y}$.

Soit N le sous-carquois de G dont l’ensemble des sommets est Som(G) et dont l’ensemble des flèches reliant $x$ à $y$ est égal à $N_{x,y}$ pour tout couple $(x, y)$ de sommets de G. C’est un sous-groupoïde distingué de G dont l’ensemble des flèches contient F; par suite, H est un sous-groupoïde de N. En particulier, $H_a\subset N_a$, d’où l’égalité.

#### Corollaire 1 {#ta-ii-s3-prop-8-cor-1 .statement tag=01TY}

Supposons de plus que, pour toute flèche $f$ de F, on ait $o(f) =t(f)$. Alors, l’origine et le terme de tout chemin dans le carquois Γ coïncident. Soit $a$ un sommet de G et soit A son orbite dans G. Pour tout élément $c$ de F dont l’origine $b$ appartient à A, fixons une flèche $f_c$ de G reliant $a$ à $b$ et posons $\kappa (c) =$ Int($f_c$)$(\delta (c)) =$ $f_c\delta (c)f_c^{-1}$.

Le groupe $H_a$ est alors le sous-groupe distingué de $G_a$ engendré par les flèches $\kappa (c)$.

D’après la prop. 8, les flèches $\kappa (c)$ sont contenues dans le groupe $H_a$. Notons $N_a$ le plus petit sous-groupe distingué de $G_a$ qui les contient. D’après cette proposition, il suffit de démontrer que, pour tout sommet $b$ de G appartenant à A, toute flèche $f_{ab}$ reliant $a$ à $b$ dans G et tout élément $c$ de Grp(Γ)$_b$, Int($f_{ab}$)$(\delta (c))$ appartient à $N_a$. Comme l’origine et le terme de chaque élément de F sont égaux, un lacet en un sommet $b$ dans le graphe $\widetilde{\Gamma}$ est de la forme $(b,(f_1, \varepsilon_1), b, . . . ,(f_n, \varepsilon_n), b)$, où pour tout $i\in  \{1, . . . , n\},f_i$ est un élément de F d’origine $b$ et $\varepsilon_i\in  \{-1,1\}$. On a

Int($f_{ab}$)$(\delta (c)) =f_{ab}f_c^{-1}\kappa (f_1)^{\varepsilon_1}. . . \kappa (f_n)^{\varepsilon_n}f_cf_{ab}^{-1}$.

Comme $f_{ab}f_c^{-1}\in G_a$, il en résulte que Int($f_{ab}$)$(\delta (c))$ appartient à $N_a$.

#### Corollaire 2 {#ta-ii-s3-prop-8-cor-2 .statement tag=01TZ}

Si le graphe associé au carquois Γ est une forêt, l’homomorphisme $p_a$ de $G_a$ dans $(G/F)_{p(a)}$ est bijectif, pour tout sommet $a$ de G.

En effet, sous cette hypothèse, on a Grp(Γ)$_b=\{e_b\}$ pour tout sommet $b$ de G (corollaire 1 de II, p. 173). Il résulte alors de la proposition 8 que, pour tout sommet $a$ de G, le groupe $H_a$ est réduit à l’élément neutre.

### 12. Groupe de Poincaré d’un graphe

Soit G un graphe. Soit $a$ un sommet de G; le groupe d’isotropie en $a$ du groupoïde Grp(G) est appelé groupe de Poincaré de G en $a$ et est noté $\pi_1(G, a)$. Soit $c$ une classe de chemins dans G, soient $a$ son origine et $b$ son terme. L’application Int($c$)$:\pi_1(G, b)\rightarrow \pi_1(G, a)$ définie par $c'\mapsto cc'c^{-1}$ est un isomorphisme de groupes. Soit $\varphi : G\rightarrow H$ un morphisme de graphes. Notons $\theta_G: G\rightarrow$ Grp(G) et $\theta_H: H\rightarrow$ Grp(H) les morphismes canoniques. Si $\overline{\varphi}$ désigne l’unique morphisme de groupoïdes Grp(G) $\rightarrow$ Grp(H) tel que $\overline{\varphi}\circ \theta_G=\theta_H\circ \varphi$, l’homomorphisme de groupes $\overline{\varphi}_a:\pi_1(G, a)\rightarrow \pi_1(H, \varphi (a))$ est noté $\pi_1(\varphi , a)$.

Soit G un graphe connexe, soit S une orientation de G et soit A un arbre orienté maximal de G (II, p. 157, prop. 1). Étant donnés des sommets $a$ et $b$ de G, il existe une unique classe de chemins $\gamma_{a,b}$ dans le graphe $\widetilde{A}$ associé à A qui relie $a$ à $b($II, p. 174, cor. 4 de la prop. 5). Si $a,b$ et $c$ sont des sommets de G, on a $\gamma_{a,b}\gamma_{b,c}=\gamma_{a,c}$, ces deux classes de chemins étant égales à l’unique classe de chemins reliant $a$ à $c$ dans $\widetilde{A}$.

#### Proposition 9 {#ta-ii-s3-prop-9 .statement tag=01U0}

Soit $a$ un sommet de G. Il existe un unique homomorphisme $\lambda$ du groupe libre F(S-Fl(A)) dans $\pi_1(G, a)$ tel que

$$
\lambda (f) =\gamma_{a,o(f)}\cdot f\cdot \gamma_{t(f),a} \tag{1}
$$

pour $f\in S$ - Fl(A). L’homomorphisme $\lambda$ est un isomorphisme de groupes.

Notons L le groupe F(S-Fl(A)). L’existence et l’unicité de l’homomorphisme $\lambda : L\rightarrow \pi_1(G, a)$ vérifiant les relations (1) résulte de A, I, p. 85, prop. 8. Soit $\mathscr{L}$ le groupoïde associé au groupe L (II, p. 163, exemple 1) ; notons $s$ son unique sommet. Il existe un unique morphisme de groupoïdes $\mu:$ Grp(G) $\rightarrow \mathscr{L}$ tel que $\mu(\theta_G(f)) =f$ pour toute flèche $f\in$ S-Fl(A) et $\mu(\theta_G(f)) =e_s$ pour toute flèche $f\in$ Fl(A) (II, p. 173, prop. 5). Pour $f\in$ S-Fl(A), on a $\mu(\theta_G(f)) =f$; l’homomorphisme $\mu_a\circ \lambda$ est donc l’isomorphisme identique du groupe L (A, I, p. 85, prop. 8). Il en résulte que $\lambda$ est injectif.

Soit $\varpi_G/A$ le groupoïde déduit de $\varpi_G$ par contraction des flèches de A et soit $p:\varpi_G\rightarrow \varpi_G/A$ le morphisme de groupoïdes canonique. Il est surjectif et l’homomorphisme de groupes $p_a$ déduit de $p$ par passage aux groupes d’isotropie est un isomorphisme (II, p. 178, cor. 2 de la prop. 8). Comme le graphe G est supposé connexe et que A en est un arbre maximal, le groupoïde $\varpi_G/A$ possède un unique sommet (II, p. 176). En outre, $\varpi_G$ est engendré par $\theta_G(G)$ ; par suite, $\varpi_G/A$ est engendré par les lacets $p(f)$, pour $f\in S$, et le groupe $(\varpi_G/A)_{p(a)}$ est engendré par les éléments de la forme $p(\theta_G(f))$, pour $f\in$ S-Fl(A). L’homomorphisme $p_a\circ \lambda$ est donc surjectif. Par suite, $\lambda$ est surjectif.

#### Remarque 1 {#ta-ii-s3-n12-rem-1 .statement tag=01U1}

L’homomorphisme $\mu_a$ est l’isomorphisme réciproque de $\lambda$.

#### Remarque 2 {#ta-ii-s3-n12-rem-2 .statement tag=01U2}

Il existe un unique homomorphisme $\lambda :$ F(Fl(G)) $\rightarrow \pi_1(G, a)$ défini par les relations (1) pour tout $f\in$ Fl(G). Il résulte de la proposition 8 que l’homomorphisme $\lambda$ est surjectif et que son noyau est le plus petit sous-groupe distingué de F(Fl(G)) contenant les éléments $f$, pour $f\in$ Fl(A), et les éléments $f\cdot \overline{f}$, pour $f\in$ Fl(G).

## EXERCICES {#ta-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
