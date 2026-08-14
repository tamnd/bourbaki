---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 4
section_title: Théorie de la descente
lang: fr
source: ta-i-iv-fr
book_pages: A IV.382-A IV.405
pdf_pages: 0398-0421
extraction: native
subsections:
    - "no": 1
      title: Données de descente
      page: 382
      pdf_page: 398
    - "no": 2
      title: Données de descente effectives
      page: 384
      pdf_page: 400
    - "no": 3
      title: Descente de morphismes
      page: 387
      pdf_page: 403
    - "no": 4
      title: 'Descente : cas des espaces étalés'
      page: 388
      pdf_page: 404
    - "no": 5
      title: 'Descente : cas des revêtements'
      page: 390
      pdf_page: 406
    - "no": 6
      title: Descente de groupoïdes
      page: 394
      pdf_page: 410
    - "no": 7
      title: Descente par une application étale et surjective
      page: 399
      pdf_page: 415
    - "no": 8
      title: Groupoïde de Poincaré d’un espace quotient
      page: 402
      pdf_page: 418
statements: 29
exercises: 0
content_sha256: 6bcb0dbabba5c5daffe7d92252651adcb290ae73aaf48cfb78c91fe6d0ece0e9
---

## § 4. THÉORIE DE LA DESCENTE

### 1. Données de descente

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Soit $(Z, p)$ un X-espace.

#### Définition 1 {#ta-iv-s4-def-1 .statement tag=0227}

On appelle donnée de descente relative à $f$ sur le X-espace $(Z, p)$ une application continue $\tau : Z\times_YX\rightarrow Z$ vérifiant les deux propriétés suivantes :

(i) Pour tout couple $(x, x')\in X\times_YX$, l’application $z\mapsto \tau (z, x')$ induit par restriction une bijection $\tau_{x,x'}$ de $Z_x$ sur $Z_{x'}$;

(ii) Pour tout triplet $(x, x', x'')$ de points de X tels que $f(x) =$ $f(x') =f(x'')$, on a

$$
\tau_{x,x''}=\tau_{x',x''}\circ \tau_{x,x'}
$$

Si $\tau$ est une donnée de descente sur $(Z, p)$, la famille $(\tau_{x,x'})$, pour $(x, x')\in X\times_YX$, est ainsi une loi d’opération (à droite) du groupoïde $X\times_YX$ sur le X-espace $(Z, p)$ (II, p. 167). En particulier, on a $\tau_{x,x}=$ Id$_{Z_x}$ pour tout $x\in X$, ce qui s’écrit aussi $\tau (z, p(z)) =z$ pour tout $z\in Z$. Inversement, étant donnée une loi d’opération (à droite) du groupoïde $X\times_YX$ sur $(Z, p)$, l’application de $Z\times_YX$ dans Z définie par $(z, x)\mapsto z\cdot (p(z), x)$ vérifie les relations (i) et (ii) de la définition.

Soient X et Y des espaces topologiques, $f: X\rightarrow Y$ une application continue et soit $(Z, p)$ un X-espace. Si $\tau$ est une donnée de descente relative à $f$ sur $(Z, p)$, la relation $R_{\tau}(z_1, z_2)$ définie par « $f(p(z_1)) =$ $f(p(z_2))$ et $\tau (z_1, p(z_2)) =z_2$ » est la relation d’équivalence dans Z déduite de l’opération du groupoïde $X\times_YX$ définie par $\tau$; elle est compatible avec l’application $f\circ p$. On dit que c’est la relation d’équivalence associée à la donnée de descente $\tau$. La bijection canonique $(z_1, z_2)\mapsto (z_1, p(z_2))$ du graphe Γ de la relation d’équivalence $R_{\tau}$ sur $Z\times_YX$ est un homéomorphisme, l’homéomorphisme réciproque applique un élément $(z_1, x_2)\in Z\times_YX$ sur $(z_1, \tau (z_1, x_2))$.

Inversement, soit R une relation d’équivalence dans Z compatible avec l’application $f\circ p: Z\rightarrow Y$ et soit Γ le graphe de R. Supposons de plus que l’application $p_2: (z_1, z_2)\mapsto (z_1, p(z_2))$ définisse un homéo-morphisme de Γ sur $Z\times_YX$. L’application $\tau : Z\times_YX\rightarrow Z$ donnée par pr$_2\circ p^{-1}_2$ est continue ; c’est une donnée de descente relative à $f$ sur $(Z, p)$ et la relation R est la relation d’équivalence associée à $\tau$.

#### Exemple 1 {#ta-iv-s4-n1-exa-1 .statement tag=0228}

Soient X et Y des espaces topologiques, soit $f: X\rightarrow Y$ une application continue et soit $(T, q)$ un Y-espace. Posons $Z = X\times_YT$. L’application $\tau$ de $Z\times_YX$ dans Z qui, à $((x, t), x')$ associe $(x', t)$, est une donnée de descente relative à $f$ sur le X-espace $(X\times_YT$, pr$_1)$, appelée donnée de descente canonique. Pour $z_1= (x_1, t_1)$ et $z_2= (x_2, t_2)\in Z$, la relation $R_{\tau}\{z_1, z_2\}$ équivaut à $t_1=t_2$.

#### Exemple 2 {#ta-iv-s4-n1-exa-2 .statement tag=0229}

Soient Y un espace topologique, $(V_i)_{i\in I}$ une famille de parties de Y, et pour tout $i\in I$, soit $(Z_i, p_i)$ un $V_i$-espace. Notons X l’espace topologique somme de la famille $(V_i)_{i\in I}$ et $(Z, p)$ le X-espace somme de la famille $(Z_i)_{i\in I}$. Soit $f: X\rightarrow Y$ l’application canonique.

L’espace $X\times_YX$ s’identifie alors à l’espace somme de la famille $(V_i\cap$ $V_j)_{(i,j)\in I\times I}($I, p. 4, exemple 5). Soit $\tau$ une donnée de descente relative à $f$ sur $(Z, p)$. Pour tout couple $(i, j)\in I\times I$, on définit une application continue $\tau_{i,j}:\overset{-1}{p_{i}}(V_i\cap V_j)\rightarrow \overset{-1}{p_{j}}(V_i\cap V_j)$ par $z\mapsto \tau (z,(p_i(z), j))$. La famille $(\tau_{i,j})$ vérifie les propriétés suivantes :

(i) Pour tout $i\in I$, on a $\tau_{i,i}=$ Id$_{Z_i}$;

(ii) Pour tout couple $(i, j)\in I\times I,\tau_{i,j}$ est un isomorphisme de $(V_i\cap V_j)$-espaces ;

(iii) Pour tout triplet $(i, j, k)\in I\times I\times I$ et tout $z\in \overset{-1}{p_{i}}(V_i\cap V_j\cap V_k)$, on a $\tau_{j,k}(\tau_{i,j}(z)) =\tau_{i,k}(z)$.

Inversement, toute famille $(\tau_{i,j})$ possédant les propriétés ci-dessus provient d’une unique donnée de descente relative à $f$ sur $(Z, p)$.

### 2. Données de descente effectives

Soient X et Y des espaces topologiques, $f: X\rightarrow Y$ une application continue et $(Z, p)$ un X-espace. Soit $\tau$ une donnée de descente relative à $f$ sur $(Z, p)$, soit $R_{\tau}$ la relation d’équivalence associée et soit $g: Z\rightarrow Z/R_{\tau}$ l’application canonique. Comme la relation $R_{\tau}$ est compatible avec l’application $f\circ p$, il existe une unique application continue $q: Z/R_{\tau}\rightarrow Y$ telle que le diagramme

Z $^gZ/R_{\tau}$

$$
pq \tag{1}
$$

X $^f$ Y

soit un carré commutatif. Le Y-espace $(Z/R_{\tau}, q)$ est appelé l’espace quotient de $(Z, p)$ par la donnée de descente $\tau$. Notons $h: Z\rightarrow X\times_Y$ $(Z/R_{\tau})$ l’application définie par $h(z) = (p(z), g(z))$ pour $z\in Z$. Elle est continue. Soit $(x, u)\in X\times_Y(Z/R_{\tau})$ et soit $z\in Z$ tel que $g(z) =u$; on a $(z, x)\in Z\times_YX$ et le point $z'=\tau (z, x)$ est l’unique élément de Z tel que $h(z') = (x, u)$ ; par suite, l’application $h$ est bijective.

On dit que la donnée de descente $\tau$ relative à $f$ sur $(Z, p)$ est effective si le diagramme (1) est un carré cartésien, c’est-à-dire si la bijection continue $h$ est un homéomorphisme. Pour que la donnée de descente $\tau$ soit effective, il faut et il suffit que les ensembles $\overset{-1}{p}(U)\cap V$, où U est une partie ouverte de X et V une partie ouverte de Z saturée pour $R_{\tau}$, constituent une base de la topologie de Z. En particulier, la condition, pour une donnée de descente relative à $f$, d’être effective est de nature locale dans Y.

#### Exemple 1 {#ta-iv-s4-n2-exa-1 .statement tag=022A}

Soient X et Y des espaces topologiques et $f: X\rightarrow Y$ une application continue. Soit $(T, q)$ un Y-espace. Soit Z le X-espace $X\times_YT$, muni de l’application pr$_1$; notons $\tau$ sa donnée de descente canonique relative à $f$ (IV, p. 383, exemple 1). Les parties de Z de la forme $X\times_YV$, où V est une partie ouverte de T, sont ouvertes dans Z et saturées pour la relation $R_{\tau}($loc. cit.). Par définition de la topologie produit, les ensembles $U\times_Y$ pr$^{-1}_2(V)$, où U est ouvert dans X et V est ouvert dans T, forment une base de la topologie de $X\times_YZ$. Par conséquent, la donnée de descente canonique sur un produit fibré $X\times_YT$ est effective.

L’application canonique $Z/R_{\tau}\rightarrow T$ est injective et continue. Elle n’est toutefois pas forcément surjective, ni stricte (IV, p. 462, exerc. 1).

#### Exemple 2 {#ta-iv-s4-n2-exa-2 .statement tag=022B}

Reprenons les notations de l’exemple 2 (IV, p. 383). L’espace topologique $Z/R_{\tau}$ est alors l’espace topologique obtenu par recollement des espaces $Z_i$ le long des $\overset{-1}{p_{i}}(V_i\cap V_j)$ au moyen des bijections $\tau_{i,j}$ (TG, I, p. 16). Par suite, si pour tout $i\in I$, l’ensemble $V_i$ est ouvert (resp. fermé) dans Y, l’ensemble $g(Z_i)$ est ouvert (resp. fermé) dans $Z/R_{\tau}$ et la restriction de $g$ à $Z_i$ induit un homéomorphisme de $Z_i$ sur $g(Z_i)$ (TG, I, p. 17, prop. 9). L’espace Z est l’espace somme des espaces $Z_i$; l’espace $X\times_Y(Z/R_{\tau})$ est l’espace somme des espaces $V_i\times_Y$ $(Z/R_{\tau}) =g(Z_i)$. L’application $h$ s’identifie à l’application somme des applications $g|Z_i: Z_i\rightarrow g(Z_i)$. C’est donc un homéomorphisme, ce qui démontre que la donnée de descente $\tau$ est effective.

Sans hypothèse particulière sur les parties $V_i$, il n’est pas toujours vrai que la restriction de $g$ à $Z_i$ induise un homéomorphisme de $Z_i$ sur son image ; dans ce cas, la donnée de descente $\tau$ n’est pas effective (IV, p. 462, exerc. 2).

#### Proposition 1 {#ta-iv-s4-prop-1 .statement tag=022C}

Soient X et Y des espaces topologiques, soit $f: X\rightarrow Y$ une application continue. Supposons que tout point de Y possède un voisinage au-dessus duquel il existe une section continue de l’application $f$. Toute donnée de descente relative à $f$ sur un X-espace est alors effective.

Soit $(Z, p)$ un X-espace et soit $\tau$ une donnée de descente relative à $f$ sur $(Z, p)$. L’assertion que $\tau$ est une donnée de descente effective est locale dans Y, ce qui permet de supposer que l’application $f$ possède une section continue $s$. Notons $g: Z\rightarrow Z/R_{\tau}$ et $q: Z/R_{\tau}\rightarrow Y$ les applications canoniques et soit $h: Z\rightarrow X\times_Y(Z/R_{\tau})$ l’application donnée par $z\mapsto (p(z), g(z))$. L’application $h$ est bijective et continue ; il suffit de montrer qu’elle est un homéomorphisme.

L’application de Z dans Z qui, à $z$, associe $\tau (z, s(f(p(z))))$ est continue et applique tout élément de Z sur l’unique élément $z'$ de Z qui lui est équivalent pour la relation $R_{\tau}$ et tel que $p(z')$ appartienne à l’image de $s$. Elle définit donc par passage au quotient une application continue $t: Z/R_{\tau}\rightarrow Z$ qui est une section de l’application $g$. En particulier, on a $f\circ p\circ t=q\circ g\circ t=q$.

Pour tout $(x, u)\in X\times_Y(Z/R_{\tau})$, on a $f(p(t(u))) =f(x)$ ; posons alors $h'(x, u) =\tau (t(u), x)$. L’application $h'$ de $X\times_Y(Z/R_{\tau})$ dans Z ainsi définie est continue. Pour tout $(x, u)\in X\times_Y(Z/R_{\tau})$, on a

$$
h(h'(x, u)) = (p(h'(x, u)), g(h'(x, u)))
$$

$$
= (p(\tau (t(u), x)), g(\tau (t(u), x)))
$$

$$
= (x, u)
$$

car $\tau (t(u), x)$ est équivalent à $t(u)$ pour la relation $R_{\tau}$. Cela démontre que l’application $h\circ h'$ est l’application identique de $X\times_Y(Z/R_{\tau})$. Pour $z\in Z$, on a alors $t(g(z)) =\tau (z, s(f(p(z)))$ et $f(p(t(g(z)))) =f(p(z))$, d’où $z=\tau (t(g(z)), p(z))$, par définition de la relation d’équivalence $R_{\tau}$. On a donc $h'(h(z)) =z$ et $h'\circ h=$ Id$_Z$. L’application $h$ est donc un homéomorphisme, ce qu’il fallait démontrer.

#### Proposition 2 {#ta-iv-s4-prop-2 .statement tag=022D}

Soit $f: X\rightarrow$ Y une application continue, soit $(Z, p)$ un X-espace et soit $\tau$ une donnée de descente relative à $f$ sur Z. La relation d’équivalence $R_{\tau}$ est fermée si $f$ est propre ; elle est ouverte si $f$ est ouverte.

L’application $\widetilde{\tau}: Z\times_YX\rightarrow$ X $\times_Y$ Z donnée par $(z, x)\mapsto$ $(p(z), \tau (z, x))$ est un homéomorphisme, d’application réciproque $(x, z)\mapsto (\tau (z, x), p(z))$. On a $\tau$ = pr$_2\circ \widetilde{\tau}$, où pr$_2: X\times_YZ\rightarrow$ Z est la seconde projection. Si $f$ est propre, pr$_2$ est propre ; si $f$ est ouverte, pr$_2$ est ouverte (I, p. 17, prop. 8). Il en résulte que $\tau$ est propre (resp. ouverte) si $f$ l’est. Le saturé d’une partie A de Z par la relation $R_{\tau}$ est l’image de $A\times_YX$ par $\tau$. Par suite, si $f$ est propre, le saturé d’une partie fermée est fermé ; si $f$ est ouverte, le saturé d’une partie ouverte est ouvert.

### 3. Descente de morphismes

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. Soient $(Z, p)$ et $(Z', p')$ des X-espaces munis de données de descente relatives à $f$, notées respectivement $\tau$ et $\tau '$. On dit qu’un X-morphisme $\varphi : Z\rightarrow Z'$ est compatible avec les données de descente $\tau$ et $\tau '$ si l’on a

$$
\tau '(\varphi (z), x) =\varphi (\tau (z, x))
$$

pour tout $(z, x)\in Z\times_YX$. Il revient au même de dire que les images par $\varphi$ de deux points équivalents suivant la relation $R_{\tau}$ sont équivalents suivant la relation $R_{\tau'}$. Un tel morphisme $\varphi$ définit, par passage aux quotients, une application continue $\varphi : Z/R_{\tau}\rightarrow Z'/R_{\tau'}$; c’est un morphisme de Y-espaces.

Notons $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ l’ensemble des X-morphismes de Z dans $Z'$ qui sont compatibles avec les données de descente $\tau$ et $\tau '$.

#### Proposition 3 {#ta-iv-s4-prop-3 .statement tag=022E}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une application continue. Soient $(Z, p)$ et $(Z', p')$ des X-espaces munis de données de descente relatives à $f$, notées respectivement $\tau$ et $\tau '$. Si la donnée de descente $\tau '$ est effective, l’application $\varphi \mapsto \varphi$ est une bijection de $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ sur $\mathscr{C}_Y(Z/R_{\tau}; Z'/R_{\tau'})$.

Pour tout X-morphisme $\varphi$ de Z dans $Z'$ compatible avec les données de descente, l’application $\varphi$ est un Y-morphisme. Inversement, notons $g: Z\rightarrow Z/R_{\tau}$ et $g': Z'\rightarrow Z'/R_{\tau'}$ les applications canoniques et soit $\psi : Z/R_{\tau}\rightarrow Z'/R_{\tau'}$ un Y-morphisme. Les applications $p: Z\rightarrow X$ et $\psi \circ g: Z\rightarrow Z'/R_{\tau'}$ sont des Y-morphismes. L’hypothèse que la donnée de descente $\tau '$ est effective signifie que le diagramme

$$
{Z'}^{g'}Z'/R_{\tau'}
$$

$p'q'$

X $^f$ Y

est un carré cartésien. Il existe donc une unique application continue $\varphi : Z\rightarrow Z'$ telle que $p'\circ \varphi =p$ et $g'\circ \varphi =\psi \circ g$. La première égalité signifie que $\varphi$ est un X-morphisme, la seconde égalité signifie que $\varphi$ est compatible avec les données de descente et que $\varphi =\psi$, d’où la proposition.

### 4. Descente : cas des espaces étalés

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Soient T et $T'$ des Y-espaces ; munissons les X-espaces $X\times_YT$ et $X\times_YT'$ de leurs données de descente canoniques et notons $\mathscr{C}_f(X\times_YT; X\times_YT')$ l’ensemble des X-morphismes de $X\times_YT$ dans $X\times_YT'$ qui sont compatibles avec ces données de descente. Pour tout Y-morphisme $\varphi : T\rightarrow T'$, le X-morphisme $f^*(\varphi ): (x, t)\mapsto$ $(x, \varphi (t))$ de $X\times_YT$ dans $X\times_YT'$ est compatible aux données de descente canoniques. On notera $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ l’application ainsi définie.

#### Proposition 4 {#ta-iv-s4-prop-4 .statement tag=022F}

Supposons que l’application $f$ soit stricte et surjective et que T soit un Y-espace étalé. Alors, l’application $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ est bijective.

Notons $\tau$ (resp. $\tau ')$ la relation d’équivalence sur $X\times_YT$ (resp. sur $X\times_YT')$ qui est associée à la donnée de descente canonique. Comme l’application $f$ est surjective, la projection pr$_2: X\times_YT\rightarrow T$ est surjective et l’application canonique $(X\times_YT)/R_{\tau}\rightarrow T$ est bijective. En particulier, l’application $f^*$ est injective. Démontrons qu’elle est surjective. Soit $\varphi : X\times_YT\rightarrow X\times_YT'$ un X-morphisme compatible avec les données de descente canoniques. Pour $(x, t)\in X\times_YT$, on a donc $\varphi (x, t) = (x, \varphi (t))$, où $\varphi$ est une application de T dans $T'$.

Par définition de $\varphi$, l’application $\varphi \circ$ pr$_2: X\times_YT\rightarrow T'$ est égale à pr$_2\circ \varphi$, elle est donc continue. Comme l’application $f$ est surjective et stricte et que T est un Y-espace étalé, la projection pr$_2: X\times_YT\rightarrow T$ est stricte (I, p. 32, remarque 3). D’après la proposition 9 de I, p. 18, l’application $\varphi$ est donc continue. C’est un Y-morphisme tel que $f^*(\varphi ) =\varphi$, ce qui démontre la proposition.

#### Corollaire {#ta-iv-s4-n4-cor-1 .statement tag=022G}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application stricte et surjective. Soient T et $T'$ des Y-espaces étalés. S’il existe un X-isomorphisme $X\times_YT\rightarrow X\times_YT'$ qui est compatible aux données de descente canoniques, les Y-espaces T et $T'$ sont isomorphes.

Soit $\psi : X\times_YT\rightarrow X\times_YT'$ un X-isomorphisme d’espaces étalés. D’après la proposition 4, il existe un unique morphisme de Y-espaces $\varphi : T\rightarrow T'$ tel que $\psi =f^*(\varphi )$. Comme $f$ est surjective, l’application $\varphi$ est bijective. Il résulte alors du cor. 2 de I, p. 30 que $\varphi$ est un isomorphisme, car les Y-espaces T et $T'$ sont étalés.

#### Proposition 5 {#ta-iv-s4-prop-5 .statement tag=022H}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Supposons que l’application $f$ soit propre et séparée, ou bien ouverte. Toute donnée de descente relative à $f$ sur un X-espace étalé est effective. En outre, si $f$ est surjective, l’espace quotient est un Y-espace étalé.

Soit $(Z, p)$ un X-espace étalé et soit $\tau$ une donnée de descente relative à $f$ sur $(Z, p)$. Notons $R_{\tau}$ la relation d’équivalence dans Z associée à $\tau$, soit $g: Z\rightarrow Z/R_{\tau}$ la surjection canonique et notons $h$ l’application de Z dans $X\times_Y(Z/R_{\tau})$ définie par $z\mapsto (p(z), g(z))$. Elle est continue et bijective ; démontrons que c’est un homéomorphisme.

a) Supposons d’abord que l’application $f$ soit ouverte.

Soit $z_0$ un point de Z ; posons $x_0=p(z_0)$. Comme $p$ est étale, il existe un voisinage U de $x_0$ dans X et une section continue $s: U\rightarrow Z$ de $p$ au-dessus de U telle que $s(x_0) =z_0$. L’application $p\times p: Z\times_YZ\rightarrow$ $X\times_YX$ est étale, et les applications de $U\times_YU$ dans $Z\times_YZ$ définies par $(x, x')\mapsto (s(x), s(x'))$ et $(x, x')\mapsto (s(x), \tau (s(x), x'))$ en sont des sections continues au-dessus de $U\times_YY$. Comme elles coïncident en tout point de $U\times_YU$ de la forme $(x, x)$, elles coïncident alors sur un voisinage ouvert V de $\Delta_U$ contenu dans $U\times_YU$. Soit $U_0$ un voisinage de $x_0$ dans X tel que $U_0\times_YU_0$ soit contenu dans V. Soit $(x, u)$ un point de $U_0\times_Yg(s(U_0))$ ; soit $x'\in U_0$ tel que $u=g(s(x'))$. On a donc $s(x) =\tau (s(x'), x)$, d’où $R_{\tau}\{s(x), s(x')\}$ et $(x, u) = (x, g(s(x'))) =$ $(x, g(s(x))) =h(s(x))$.

Comme l’application $g$ est ouverte (IV, p. 386, prop. 2), l’ensemble $U_0\times_Yg(s(U_0))$ est une partie ouverte de $X\times_Y(Z/R_{\tau})$ sur laquelle l’application $h^{-1}$ est égale à l’application continue $s\circ$ pr$_1$. L’application $h$ est donc un homéomorphisme.

b) Supposons maintenant que l’application $f$ soit propre et séparée.

Soit $z_0$ un point de Z; posons $x_0=p(z_0)$ et $y_0=f(x_0)$. L’application $s$ donnée par $x\mapsto \tau (z_0, x)$ est une section de $p$ au-dessus de $\overset{-1}{f}(y_0)$.

L’ensemble $\overset{-1}{f}(y_0)$ est compact (TG, I, p. 75, th. 1 et I, p. 26, remarque 2) et deux points distincts de $\overset{-1}{f}(y_0)$ possèdent des voisinages disjoints dans X, car $f$ est séparée (I, p. 25, prop. 1). D’après le théo-rème 2 de I, p. 37, il existe donc un voisinage $U_0$ de $\overset{-1}{f}(y_0)$ dans X et une section $s_0$ de $p$ au-dessus de $U_0$ qui prolonge $s$. L’ensemble $s_0(U_0)$ est un ouvert de Z, car $p$ est étale (I, p. 30, cor. 3), et contient le saturé de l’ensemble $\{z_0\}$ pour la relation $R_{\tau}$. L’application $g$ est fermée (IV, p. 386, prop. 2). Il existe alors un ouvert V de $Z/R_{\tau}$ tel que $W =\overset{-1}{g}(V)\cap \overset{-1}{p}(U_0)$ soit un voisinage de $z_0$ contenu dans $s_0(U_0)$ (I, p. 75, lemme).

Soit alors $(x, u)\in U_0\times_YV$ et soit $z$ l’unique point de Z tel que $h(z) = (x, u)$ ; par définition, on a $z\in W$. Puisque $W\subset s_0(U_0)$, on a $z=s_0(p(x))$. Cela montre que la restriction de $h^{-1}$ à l’ouvert $U_0\times_YV$ de $X\times_Y(Z/R_{\tau})$ est égale à $s_0\circ p\circ$ pr$_1$. Par suite, $h$ est un homéomorphisme.

Nous avons ainsi montré que la donnée de descente $\tau$ est effective. L’application $f$ est universellement stricte (I, p. 20, corollaire). Sous l’hypothèse que $f$ est surjective, il résulte alors de la prop. 8 de I, p. 31 que $q: Z/R_{\tau}\rightarrow Y$ est étale.

### 5. Descente : cas des revêtements

Soient X, Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue surjective. Soit $(Z, p)$ un revêtement de X et soit $\tau$ une donnée de descente relative à $f$ sur Z.

Si $f$ est propre et séparée (resp. si $f$ est ouverte), la donnée de descente $\tau$ est effective et le Y-espace $Z/R_{\tau}$ est un espace étalé (IV, p. 389, prop. 5). C’est même un revêtement de Y si $f$ possède une section continue au voisinage de chaque point (I, p. 72, prop. 3) ou si Z est un revêtement localement fini de X (I, p. 77, cor. 4). Ce numéro est consacré à mettre en évidence d’autres conditions sous lesquelles $Z/R_{\tau}$ est un revêtement de Y.

Démontrons au préalable un lemme.

#### Lemme 1 {#ta-iv-s4-lem-1 .statement tag=022I}

Soient B, $B'$ des espaces topologiques et soit $f: B'\rightarrow B$ une application continue. Si le carré fibré $B'\times_BB'$ est localement connexe, l’espace topologique $B'$ est localement connexe.

Soit $a$ un point de $B'$ et soit V un voisinage de $a$. Supposons que le carré fibré $B'\times_BB'$ soit localement connexe et soit W un voisinage connexe de $(a, a)$ dans $B'\times_BB'$ qui est contenu dans $V\times V$. Posons U = pr$_1(W)$. L’ensemble U est contenu dans V, et est connexe puisque l’image d’un ensemble connexe par une application continue est connexe. Si $\Delta_{B'}$ désigne la diagonale de $B'\times_BB'$, l’application pr$_1|\Delta_{B'}: \Delta_{B'}\rightarrow B'$ est un homéomorphisme. Comme U contient pr$_1(W\cap \Delta_{B'})$ et que $W\cap \Delta_{B'}$ est un voisinage de $(a, a)$ dans $\Delta_{B'}$, U est un voisinage de $a$ dans $B'$. Cela prouve le lemme.

#### Proposition 6 {#ta-iv-s4-prop-6 .statement tag=022J}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. On suppose que l’application $f$ est propre, séparée et surjective, et on fait l’une des hypothèses suivantes :

(i) Les fibres de $f$ sont localement connexes et le carré fibré $B'\times_BB'$ est localement connexe.

(ii) Les fibres de $f$ sont finies, la diagonale $\Delta_{B'}$ de $B'\times_BB'$ est ouverte dans $B'\times_BB'$ et $B'\times_BB'-\Delta_{B'}$ est un espace localement connexe.

Alors, si $(E', p')$ est un revêtement, $(E, p)$ est un revêtement.

Comme l’application $f$ est universellement stricte (I, p. 20, corollaire), l’application $p$ est étale (I, p. 31, prop. 8) et séparée (I, p. 27, prop. 4). Nous supposerons, ce qui est loisible, que $E'= B'\times_BE$.

Soit $a$ un point de B ; il s’agit de démontrer que le point $a$ possède un voisinage W tel que le W-espace $(E_W, p_W)$ soit un revêtement

trivialisable. Posons $B'_a$ = $\overset{-1}{f}(a)$ et notons $E'_a$ = $(^-{p'}^1)(E_a)$. L’application $t_a: E'_a\rightarrow B'_a\times E_a$ définie par $t_a(y) = (p'(y), f'(y))$ est un $B'_a$-isomorphisme (I, p. 9, prop. 4), donc $E'_a$ est un revêtement trivialisable de $B'_a$ et $t_a$ est une trivialisation de ce revêtement.

Démontrons qu’il existe un voisinage $V'$ de $B'_a$ dans $B'$ et une trivialisation continue $t$ du revêtement $(E'_{V'}, p_{V'})$ qui prolonge $t_a$. Sous l’hypothèse (ii), $B'_a$ est fini et ses points possèdent des voisinages ouverts deux à deux disjoints au-dessus desquels le revêtement $E'$ est trivialisable, d’où l’assertion dans ce cas. Sous l’hypothèse (i), $B'_a$ est localement connexe, de même que $B'($IV, p. 390, lemme 1) ; comme l’application $f$ est propre et séparée, $B'_a$ est compact et deux points distincts possèdent des voisinages disjoints dans $B'$, si bien que le couple $(B',B'_a)$ satisfait la propriété (PCV) ( I, p. 37, lemme 1). L’assertion résulte donc du cor. 2 de I, p. 90.

Comme $f$ est propre, il existe un voisinage V de $a$ dans B tel que $V'$ contienne $\overset{-1}{f}(V)$ (lemme, I, p. 75). On peut ainsi supposer que

$$
V'=\overset{-1}{f}(V)
$$

Munissons les $V'$-espaces $V'\times E_a$ et $E'_{V'}= V'\times_BE$ de leurs données de descente canoniques relatives à $f_V: V'\rightarrow V$. Nous allons montrer que, quitte à diminuer V et $V'$, l’isomorphisme de $V'$-espaces $t: E'_{V'}\rightarrow$ $V'\times E_a$ que nous venons de définir est compatible aux données de descentes, c’est-à-dire que l’on a $t(b'_1, x) =t(b'_2, x)$ si $(b'_1, b'_2)\in V'\times_VV'$ et $x\in E_{f(b'_1)}$. Notons $\widetilde{t}$ l’application pr$_2\circ t: E'_{V'}\rightarrow E_a$.

Posons $V''= V'\times_VV'$; considérons-le comme un $V'$-espace au moyen de la première projection. L’application $((b'_1, b'_2), x)\mapsto ((b'_1, b'_2),(b'_1, x))$ de $V''\times_VE$ dans $V''\times_{V'}E'$ est un isomorphisme de $V''$-espaces ; cela montre que $V''\times_VE$ est un revêtement de $V''$.

Pour $i= 1$, 2, définissons une application $u_i: V''\times_VE\rightarrow V''\times E_a$ en posant $u_i(b'_1, b'_2, x) = (b'_1, b'_2,\widetilde{t}(b'_i, x))$; ce sont des trivialisations du revêtement $V''\times_VE$. Soit $W''$ l’ensemble des points $w\in V''$ au-dessus desquels ces trivialisations $u_1$ et $u_2$ coïncident ; il contient $B'_a\times B'_a$, ainsi que la diagonale $\Delta_{V'}$. Démontrons que $W''$ est un voisinage de $B'_a\times B'_a$. Sous l’hypothèse (i), cela résulte du cor. 2 de I, p. 80, car $B'\times B'$ est localement connexe. Sous l’hypothèse (ii), $W''$ contient un voisinage de $(B'_a\times B'_a)-\Delta_{B'_a}$ dans $(B'\times_BB')-\Delta_{B'}$, car cet ensemble est localement connexe (loc. cit.). Comme $\Delta_{V'}$ est ouvert dans $B'\times_BB',W''$ est un voisinage de $B'_a\times B'_a$ dans $V''$.

Comme $f$ est propre, l’application canonique $f''$ de $B'\times_BB'$ dans B est propre, car c’est la composée de la projection pr$_1: B'\times_BB'\rightarrow B'$ et de l’application $f$.

D’après le lemme de I, p. 75, il existe un voisinage W de $a$ dans V

tel que $(f\overset{-1}{''})(W)$ soit contenu dans $W''$; posons $W'=(\overset{-1}{f}')(W)$, c’est une partie de $V'$ et l’isomorphisme d’espaces étalés $t: E'_{W'}\rightarrow W'\times E_a$ est compatible aux données de descente canoniques relatives à l’application $f_W: W'\rightarrow W$. Il résulte du corollaire (IV, p. 388) que les W-espaces étalés $E_W$ et $W\times E_a$ sont isomorphes. En particulier, $E_W$ est un revêtement trivialisable, d’où la proposition.

#### Corollaire 1 {#ta-iv-s4-prop-6-cor-1 .statement tag=022K}

Soient E et B des espaces topologiques, $p: E\rightarrow B$ une application continue et $(A_i)_{i\in I}$ un recouvrement fermé localement fini de B tel que pour tout couple $(i, j)\in I\times I,i=\not j$, l’intersection $A_i\cap A_j$ soit un espace localement connexe. Alors, pour que le B-espace $(E, p)$ soit un revêtement, il faut et il suffit que, pour tout $i\in I$, le $A_i$-espace $(\overset{-1}{p}(A_i), p_{A_i})$ soit un revêtement de $A_i$.

La condition est nécessaire (cf. I, p. 69). Inversement, notons $B'$ l’espace topologique somme de la famille $(A_i)_{i\in I}$ et $f: B'\rightarrow B$ l’application canonique. L’application $f$ est fermée (TG, I, p. 6, prop. 4), séparée (I, p. 27, remarque 5), à fibres finies, donc propre (TG, I, p. 75, th. 1), elle est aussi surjective. La diagonale $\Delta_{B'}$, étant égale à $\bigcup_{i\in I}A_i\times_BA_i$, est ouverte dans $B'\times_BB'$. Enfin, l’espace $(B'\times_BB')-\Delta_{B'}$ est homéomorphe à l’espace somme de la famille $(A_i\cap A_j)$, $(i, j)\in I\times I$, $i=\not j$; il est donc localement connexe. L’hypothèse (ii) de la proposition 6 est satisfaite. Si pour tout $i,\overset{-1}{p}(A_i)$ est un revêtement de $A_i,E'$ est alors un revêtement de $B'$, donc E est un revêtement de B.

#### Corollaire 2 {#ta-iv-s4-prop-6-cor-2 .statement tag=022L}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application propre, séparée et surjective. On fait de plus l’une des hypothèses suivantes :

(i) Les fibres de $f$, ainsi que l’espace $X\times_YX$, sont localement connexes ;

(ii) Les fibres de $f$ sont finies, la diagonale $\Delta_X$ de $X\times_YX$ est ouverte dans $X\times_YX$ et l’espace $(X\times_YX)-\Delta_X$ est localement connexe. Alors, toute donnée de descente relative à $f$ sur un revêtement de X est effective, et l’espace quotient est un revêtement de Y.

Soit Z un revêtement de X et soit $\tau$ une donnée de descente relative à $f$ sur Z. D’après la proposition 5 (IV, p. 389), la donnée de descente $\tau$ est effective, autrement dit le carré

Z $Z/R_{\tau}$

X $^f$ Y

est un carré cartésien. Les hypothèses de la proposition 6 (IV, p. 391) sont alors satisfaites. Par conséquent, $Z/R_{\tau}$ est un revêtement de Y.

#### Proposition 7 {#ta-iv-s4-prop-7 .statement tag=022M}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue et surjective. Supposons que l’espace Y soit délaçable et que l’application $f$ soit ouverte et possède la propriété de relèvement des chemins. Alors, toute donnée de descente relative à $f$ sur un revêtement de X est effective, et l’espace quotient est un revêtement de Y.

Soit $(Z, p)$ un revêtement de X et soit $\tau$ une donnée de descente relative à $f$ sur Z. Comme l’application $f$ est surjective et ouverte, il résulte de la prop. 5 de IV, p. 389, que la donnée de descente $\tau$ est effective. Notons $T = Y/R_{\tau}$ le Y-espace quotient ; sa projection $q$ est étale (loc. cit.), elle est aussi séparée (I, p. 27, prop. 4).

Par hypothèse, l’application $f$ possède la propriété de relèvement des chemins, de même que l’application $p$, car Z est un revêtement de X (III, p. 302, corollaire 2 de la prop. 3). Il en est par suite de même de l’application $p\circ f$, donc de l’application $q$. Par conséquent (cf. IV, p. 341, remarque 2), T est un revêtement de Y. La proposition est ainsi démontrée.

#### Remarque {#ta-iv-s4-n5-rem-1 .statement tag=022N}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application. Pour que toute donnée de descente relative à $f$ sur un revêtement de X soit effective, et que l’espace quotient soit un revêtement de Y, il est nécessaire que $f$ soit stricte et que $f(X)$ soit une partie ouverte et fermée de X.

En effet, identifions le X-espace X à $X\times_YY$ et munissons-le de sa donnée de descente canonique relative à $f$. L’espace quotient s’identifie à $f(X)$, muni de la topologie quotient de la topologie de X pour la relation d’équivalence définie par $f$. Si c’est un revêtement de Y, l’espace $f(X)$ s’identifie alors à une partie ouverte et fermée de Y et l’application $f$ est stricte.

### 6. Descente de groupoïdes

Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Notons $p_1$ et $p_2$ les deux projections de $X\times_YX$ dans X, Coeg($f$) le groupoïde coégalisateur du couple $(\varpi (p_1), \varpi (p_2))$ de morphismes de groupoïdes de $\varpi (X\times_YX)$ dans $\varpi (X)$ et $\gamma :\varpi (X)\rightarrow$ Coeg($f$) le morphisme de groupoïdes canonique (II, p. 199, déf. 2). Comme $f\circ p_1=f\circ p_2$, on a $\varpi (f)\circ \varpi (p_1) =\varpi (f)\circ \varpi (p_2)$. Il résulte alors de la propriété universelle des coégalisateurs (II, p. 199, prop. 3) qu’il existe un unique morphisme de groupoïdes $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ tel que $\varpi (f) =\varpi '(f)\circ \gamma$.

L’ensemble des sommets de Coeg($f$) est l’ensemble quotient de l’ensemble X = Som($\varpi (X)$) par la relation d’équivalence définie par $f($II, p. 200, remarque 1). On l’identifie à $f(X)$.

#### Proposition 8 {#ta-iv-s4-prop-8 .statement tag=022O}

Soient X et Y des espaces topologiques non vides et soit $f$ une application continue de X dans Y. On suppose que l’espace X est localement connexe par arcs, que l’espace Y est connexe et que l’application $f$ est stricte et surjective. Alors, le groupoïde Coeg($f$) est transitif.

Soit Γ le carquois dont l’ensemble des sommets est X et dont l’ensemble des flèches est l’ensemble somme de Fl($\varpi (X)$) et de $X\times_YX$, les applications origine et terme étant celles de $\varpi (X)$ dans Fl($\varpi (X)$) et les applications $p_1$ et $p_2$ dans $X\times_YX$. D’après la définition de l’armature du couple $(\varpi$(pr$_1), \varpi$(pr$_2))$ (II, p. 185, déf. 3) et la remarque 2 de II, p. 200, l’ensemble des orbites de Coeg($f$) s’identifie à l’ensemble des composantes connexes du carquois Γ. Comme l’espace X n’est pas vide, il suffit de prouver que le graphe Γ est connexe.

Les composantes connexes de Γ sont saturées pour la relation d’équivalence « il existe un chemin joignant $x$ à $x'$ », donc sont ouvertes dans X, car X est localement connexe par arcs. Elles sont alors également fermées. Elles sont aussi saturées pour la relation d’équivalence R définie par $f$. Par hypothèse, l’application $f$ induit un homéomorphisme de $X/R$ sur Y, si bien que l’image par $f$ de toute composante connexe de Γ est une partie ouverte et fermée de Y, donc est égale à Y puisque l’espace Y est supposé connexe.

Soit C une composante connexe de Γ, soit $x$ un point de X. D’après ce qui précède, il existe un point $x'\in C$ tel que $f(x') =f(x)$. Par définition du carquois Γ, on a $x'\in C$. On a ainsi C = X et le carquois Γ est donc connexe.

#### Proposition 9 {#ta-iv-s4-prop-9 .statement tag=022P}

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. On suppose que l’espace X est localement connexe par arcs, que l’espace Y est délaçable et que l’application $f$ est stricte et surjective. Alors, le groupoïde $\varpi (Y)$ est engendré par l’image de $\varpi (X)$ par $\varpi (f)$.

On peut supposer que les espaces X et Y sont non vides. Notons G le sous-groupoïde de $\varpi (Y)$ engendré par l’image de $\varpi (X)$ par $\varpi (f)$. Comme l’application $f$ est surjective, l’ensemble des sommets de G est égal à Y. D’après la prop. 8, Coeg($f$) est un groupoïde transitif. Comme $\varpi '(f)$ induit l’identité sur les sommets, l’image de Coeg($f$) par $\varpi '(f)$ est un sous-groupoïde transitif de $\varpi (Y)$. L’image de $\varpi (X)$ par $\gamma$ engendre Coeg($f$) (II, p. 200, corollaire) ; comme on a $\varpi (f) =$ $\varpi '(f)\circ \gamma$, le groupoïde G est transitif.

Soit $y_0$ un point de Y et notons H le sous-groupe $G_{y_0}$ de $\pi_1(Y, y_0)$. D’après le th. 1 de IV, p. 342, il existe un revêtement connexe $(T, p)$ de Y et un point $t_0$ de la fibre $T_{y_0}$ dont H soit le fixateur.

Si $x$ est un point de X, l’ensemble Fl$_{y_0,f(x)}(G)$ n’est pas vide, car G est transitif. Pour $u\in$ Fl$_{y_0,f(x)}(G)$, le point $t_0\cdot u$ est un point de la fibre $T_{f(x)}$, indépendant de $u$ puisque le groupe H, groupe d’isotropie de G en $y_0$, fixe $t_0$. Notons $\sigma (x)$ ce point ; notons $\sigma : X\rightarrow T$ l’application ainsi définie et $s: X\rightarrow X\times_YT$ l’application $x\mapsto (x, \sigma (x))$. Par construction, l’application $s$ est compatible avec les opérations canoniques de $\varpi (X)$ dans X et $X\times_YT$. Il résulte alors du lemme 1 de III, p. 312 que $s$ est continue. L’application $\sigma$ est donc continue ; elle est en outre compatible à la relation d’équivalence définie par $f$, car $\sigma (x)$ ne dépend que de $f(x)$. Puisque $f$ est stricte et surjective, il existe une unique application continue $\sigma : Y\rightarrow T$ telle que $\sigma \circ f=\sigma$, si bien que le revêtement T admet une section. Comme T est connexe, l’application $p: T\rightarrow Y$ est un homéomorphisme (I, p. 31, cor. 4 de la prop. 6) et l’on a $H =\pi_1(Y, y_0)$, d’où $G_{y_0}=\pi_1(Y, y_0)$. Comme G est transitif, il en résulte que $G =\varpi (Y)$.

#### Proposition 10 {#ta-iv-s4-prop-10 .statement tag=022Q}

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. On suppose que l’espace X est délaçable, que l’espace $X\times_YX$ est localement connexe par arcs, et que toute donnée de descente relative à $f$ sur un revêtement de X est effective et l’espace quotient est un revêtement de Y. Alors, le morphisme de groupoïdes $\varpi '(f)$ de Coeg($f$) dans $\varpi (Y)$ est injectif.

Sous les hypothèses de la proposition, $f$ est stricte ( IV, p. 394, remarque) ; on peut en outre supposer qu’elle est surjective.

#### Lemme 2 {#ta-iv-s4-lem-2 .statement tag=022R}

Conservons les notations et les hypothèses de la proposition. Soit T un ensemble muni d’une opération du groupoïde Coeg($f$) relativement à une application $q: T\rightarrow Y$. Il existe alors une unique topologie sur T pour laquelle $q$ fait de T un revêtement de Y de sorte que pour toute classe de chemin d’origine $c$ dans X et tout point $t$ de T, on ait $t\cdot \gamma (c) =t\cdot f_*(c)$. En particulier, l’opération de Coeg($f$) sur T se factorise par une opération du groupoïde $\varpi (Y)$.

L’unicité d’une telle topologie sur T résulte du lemme 1 (III, p. 312) ; démontrons son existence. Munissons l’ensemble $X\times_YT$ d’une loi d’opération de $\varpi (X)$ en posant $(x, t)\cdot u= (x\cdot u, t\cdot \gamma (u))$ pour tout $(x, t)\in X\times_YT$ et toute flèche $u$ d’origine $x$ dans $\varpi (X)$. Comme l’espace X est délaçable, cette loi d’opération de $\varpi (X)$ est sans monodromie locale (III, p. 313, remarque). Il existe donc sur l’ensemble $X\times_YT$ une unique topologie qui fasse du X-espace $(X\times_YT$, pr$_1)$ un revêtement de X et telle que l’opération canonique de $\varpi (X)$ dans ce revêtement coïncide avec l’opération donnée (III, p. 313, prop. 3). Notons $(Z, p)$ ce revêtement. Montrons que l’application $\tau : ((x_1, t), x_2)\mapsto (x_2, t)$ de $Z\times_YX$ dans Z est une donnée de descente sur Z relative à l’application $f$. Il suffit de vérifier qu’elle est continue, les autres conditions de la définition 1 de IV, p. 382, étant évidentes.

L’application $\tau$ est un relèvement de l’application pr$_2: Z\times_YX\rightarrow X$ au revêtement Z de X. Comme l’espace $X\times_YX$ est localement connexe par arcs, l’espace $Z\times_YX$, qui en est un revêtement, est aussi localement connexe par arcs. D’après le corollaire (III, p. 269), pour montrer que l’application $\tau$ est continue, il suffit de démontrer qu’elle est continue par arcs.

Soit donc $\widetilde{c}= ((c, g), c')$ un chemin dans $Z\times_YX$ et montrons que l’application $\tau \circ \widetilde{c}:t\mapsto (c'(t), g(t))$ de $\mathbf{I}$ dans Z est continue. Pour tout $s\in [0,1]$, notons $c_s$ et $c'_s$ les chemins dans X définis par $t\mapsto c(st)$ et $t\mapsto c'(st)$. Pour tout $s\in [0,1]$, on a ainsi $c(s) =c(0)\cdot [c_s]$, $c'(s) =c'(0)\cdot [c'_s]$ et $(c, g)(s) = (c(0), g(0))\cdot [c_s]$, où $[u]$ désigne la classe d’homotopie stricte d’un chemin $u($III, p. 304, remarque). L’application $t\mapsto (c_s(t), c'_s(t))$ est un chemin dans $X\times_YX$ ; par définition du coégalisateur Coeg($f$), on a donc $\gamma ([c_s]) =\gamma ([c'_s])$ et $g(s) =g(0)\cdot \gamma ([c_s]) =$ $g(0)\cdot \gamma ([c'_s])$. Par définition de l’opération de $\varpi (X)$ sur Z, on a donc

$$
(\tau \circ \widetilde{c})(s) = (c'(s), g(s)) = (c'(0)\cdot [c'_s], g(0)\cdot \gamma ([c'_s]))
$$

$$
= (c'(0), g(0))\cdot [c'_s] = (\tau \circ \widetilde{c})(0)\cdot [c'_s]
$$

Cela montre que $\tau \circ \widetilde{c}$ est un relèvement continu à Z du chemin $c'($loc. cit.). Par suite, l’application $\tau$ est continue par arcs, donc continue ; c’est une donnée de descente relative à $f$ sur le X-espace Z.

Désignons par $R_{\tau}$ la relation d’équivalence définie par la donnée de descente $\tau$. L’application $f$ étant surjective, l’application pr$_2: Z\rightarrow T$ induit, par passage au quotient, une bijection de $Z/R_{\tau}$ sur T. Munissons T de la topologie déduite de celle de $Z/R_{\tau}$ par transport de structure, de sorte que $(T, q)$ est un Y-espace. Par hypothèse, T est donc un revêtement de Y et le diagramme

Z $^{pr_2}$ T

$pq$

X $^f$ Y

est un carré cartésien.

Soient $(x, t)$ un point de Z$,c$ un chemin d’origine $x$ dans X et soit $\widetilde{c}$ le relèvement continu de $c$ à Z d’origine $(x, t)$. Le chemin pr$_2\circ \widetilde{c}$ est le relèvement d’origine $t$ du chemin $f\circ c$ de Y, de sorte que $t\cdot \gamma ([c]) =$ $t\cdot [f\circ c] =t\cdot f_*([c])$. Cela conclut la démonstration du lemme.

Démontrons maintenant la proposition. Soient $u$ et $v$ deux flèches de Coeg($f$) dont les images dans $\varpi (Y)$ sont égales. Le morphisme de groupoïdes $\varpi '(f)$ étant l’identité sur les ensembles de sommets, les flèches $u$ et $v$ ont même origine et même terme. Notons $y$ l’origine de $u$; soit T l’ensemble des flèches de Coeg($f$) d’origine $y$ et soit $q: T\rightarrow Y$ la restriction à T de l’application terme. Le groupoïde Coeg($f$) opère par composition à droite sur l’ensemble T, relativement à $q$. D’après le lemme 2, les actions de $u$ et $v$ sur T sont identiques. On a donc $u=$ $e_y\cdot u=e_y\cdot v=v$. Cela prouve que le morphisme de groupoïdes $\varpi '(f)$ est injectif.

#### Théorème 1 {#ta-iv-s4-thm-1 .statement tag=022S}

Soient X et Y des espaces topologiques, soit $f: X\rightarrow$ Y une application continue et surjective. Supposons que les espaces X et Y soient délaçables. Supposons enfin que l’une des propriétés suivantes soit satisfaite :

(i) L’application $f$ est propre, séparée, à fibres localement connexes, l’espace $X\times_YX$ est localement connexe par arcs ;

(ii) L’application $f$ est propre, séparée, à fibres finies, la diagonale $\Delta_X$ est ouverte dans $X\times_YX$ et son complémentaire est localement connexe ;

(iii) L’application $f$ est ouverte et possède la propriété de relèvement des chemins. Alors, le morphisme de groupoïdes $\varpi '(f)$ est un isomorphisme du groupoïde Coeg($f$) sur le groupoïde de Poincaré $\varpi (Y)$.

Notons d’abord que sous ces hypothèses, l’application $f$ est surjective et stricte (I, p. 18, exemple 2). De plus, toute donnée de descente relative à $f$ sur un revêtement de X est effective, et l’espace quotient est un revêtement de Y ; cela résulte en effet de IV, p. 393, corollaire 2 de la prop. 4 sous les hypothèses (i) et (ii), et de la prop. 7 de IV, p. 394 sous l’hypothèse (iii). D’après la prop. 10, le morphisme de groupoïdes $\varpi '(f)$ est donc injectif et son image est un sous-groupoïde de $\varpi (Y)$.

D’après la prop. 9 de IV, p. 395, cette image est égale à $\varpi (Y)$ sous les hypothèses (i) et (ii), mais aussi sous l’hypothèse (iii) puisque le morphisme de groupoïdes $\varpi (f)$ est alors surjectif.

Par suite, $\varpi '(f)$ est un isomorphisme.

#### Exemple {#ta-iv-s4-n6-exa-1 .statement tag=022T}

Voici deux exemples où les hypothèses du théorème 1 sont satisfaites.

1) Soit Y un espace topologique délaçable. Soit $(A_i)_{i\in I}$ un recouvrement localement fini de Y par des ensembles fermés. On suppose que, pour tout $i\in I$, l’espace $A_i$ est délaçable et que, pour tout couple $(i, j)\in I\times I$, l’espace $A_i\cap A_j$ est localement connexe par arcs. On peut prendre pour X l’espace somme de la famille $(A_i)_{i\in I}$ et pour $f: X\rightarrow Y$ l’application déduite de la famille des injections canoniques.

2) Soit G un groupe discret opérant proprement dans un espace topologique délaçable X, posons $Y = X/G$ et soit $f: X\rightarrow Y$ l’application canonique. Elle est ouverte (TG, III, p. 10, lemme 2) et possède la propriété de relèvement des chemins en vertu du théorème 4 de III, p. 287. L’espace Y est délaçable d’après IV, p. 349, prop. 8, b). Par hypothèse, l’application de $G\times X$ dans $X\times X$ donnée par $(g, x)\mapsto (g\cdot x, x)$ est propre, donc stricte (I, p. 18, exemple 2) et son image est $X\times_YX$. Il résulte alors de III, p. 261, prop. 8 que $X\times_YX$ est localement connexe par arcs.

### 7. Descente par une application étale et surjective

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. On conserve les notations du n$^o$ précédent.

#### Théorème 2 {#ta-iv-s4-thm-2 .statement tag=022U}

Supposons que tout point de Y possède un voisinage au-dessus duquel il existe une section continue de l’application $f$. Le morphisme de groupoïdes $\varpi '(f)$ de Coeg($f$) dans $\varpi (Y)$ est un isomorphisme.

Par hypothèse, il existe un recouvrement $(U_j)_{j\in J}$ de Y par des ensembles ouverts et, pour tout $j\in J$, une section continue $s_j$ de $f_{U_j}$.

Si $c$ est un chemin dans X, on notera $[c]$ sa classe d’homotopie stricte dans $\varpi (X)$ et $\{c\}$ l’image de $[c]$ dans Coeg($f$) par le morphisme de groupoïdes $\varpi '(f)$. Si $c$ et $c'$ sont deux chemins dans X$,\{c\}$ et $\{c'\}$ sont composables dans Coeg($f$) si et seulement si les chemins $f\circ c$ et $f\circ c'$ dans Y sont juxtaposables.

Soit $c'$ un chemin dans Y. D’après le lemme 4 de III, p. 272, appliqué

à l’espace compact $\mathbf{I}$ et au recouvrement ($(^-{c'}^1)(U_j)$)$_{j\in J}$ de $\mathbf{I}$, il existe un entier $n$ tel que, pour tout entier $k$ vérifiant $1\leqslant k\leqslant n$, l’image de l’intervalle $[^{k-1}_n,^k_n]$ par $c'$ soit contenue dans un ouvert $U_{j(k)}$. Pour tout entier $k,1\leqslant k\leqslant n$, soit $c'_k$ le chemin dans Y défini par $s\mapsto c'(^{k+s-1}_n)$ ; on a $[c'] = [c'_1][c'_2]. . .[c'_n]$ (cf. III, p. 291, remarque 1), et $c'$ est le chemin noté $c'_1*c'_2* \cdots  *c'_n$. Pour tout $k\in  \{1, . . . , n\}$, notons $c_k$ le chemin $s_{j(k)}\circ c'_k$ dans X et posons $\{c_k\}=\gamma ([c_k])$. Comme pour tout $k$, les chemins $c'_{k-1}=f\circ c_{k-1}$ et $c'_k=f\circ c_k$ sont juxtaposables, la suite $(\{c_1\}, . . . ,\{c_n\})$ est composable dans Coeg($f$). Par construction,

$$
\varpi '(f)(\{c_1\}. . .\{c_n\}) =\varpi '(f)(\{c_1\}). . . \varpi '(f)(\{c_n\})
$$

$$
=\varpi (f)([c_1]). . . \varpi (f)([c_n])
$$

$$
= [f\circ c_1]. . .[f\circ c_n]
$$

$$
= [c'_1]* \cdots  *[c'_n] = [c']
$$

ce qui prouve que le morphisme de groupoïdes $\varpi '(f)$ est surjectif.

Soient $u$ et $v$ des flèches de Coeg($f$). Comme le groupoïde Coeg($f$) est engendré par l’image de $\varpi (X)$ (II, p. 200, corollaire), il existe des suites finies $(c_1, . . . , c_n)$ et $(d_1, . . . , d_n)$ de chemins dans X telles que l’on ait $u=\{c_1\}. . .\{c_n\}$ et $v=\{d_1\}. . .\{d_n\}$. Les chemins $(f\circ c_1, . . . , f\circ c_n)$ dans Y sont alors juxtaposables et l’on a $\varpi '(f)(u) = [(f\circ c_1)]. . .[(f\circ$ $c_n)]$; de même, $\varpi '(f)(v) = [(f\circ d_1)]. . .[(f\circ d_n)]$.

Supposons que l’on ait $\varpi '(f)(u) =\varpi '(f)(v)$. Il existe alors une homotopie stricte $\sigma$ reliant $(f\circ c_1)* \cdots  *(f\circ c_n)$ à $(f\circ d_1)* \cdots  *(f\circ d_n)$. D’après le lemme 4 de III, p. 272, appliqué à l’espace compact $\mathbf{I}\times \mathbf{I}$ et au recouvrement $(\overset{-1}{\sigma}(U_i))_{i\in I})$ de $\mathbf{I}\times \mathbf{I}$, il existe un entier $m\geqslant 1$ tel que, pour tout couple d’entiers $(j, k)$ vérifiant $1\leqslant j\leqslant m$ et $1\leqslant k\leqslant m$, l’image de $[^{j-1}_m,_m^j]\times [^{k-1}_m,_m^k]$ par $\sigma$ soit contenue dans un ouvert $U_{i(j,k)}$ du recouvrement $(U_i)_{i\in I}$.

Tout chemin $c$ dans X est de la forme $c_1* \cdots  *c_m$, où $c_k$ est le chemin $t\mapsto c(^{k-1+t}_m)$. Quitte à remplacer les entiers $m$ et $n$ par leur produit $mn$, on peut donc supposer que $m=n$.

Pour tout couple $(j, k)$ d’entiers de $\{1, . . . , n\}$ et tout couple $(s, t)\in$ $\mathbf{I}\times \mathbf{I}$, posons

$$
s+j-1t+k-1
$$

$\sigma_{j,k}(s, t) =s_{i(j,k)}\circ \sigma$,.

$$
nn
$$

Pour $t\in \mathbf{I}$, posons aussi $h^0_{j,k}(t) =\sigma_{j,k}(t,0)$, $h^1_{j,k}(t) =\sigma_{j,k}(t,1)$, $v^0_{j,k}(t) =\sigma_{j,k}(0, t)$ et $v_{j,k}^1(t) =\sigma_{j,k}(1, t)$. D’après le lemme 1 de III, p. 295, les chemins $h^0_{j,k}*v_{j,k}^1$ et $v_{j,k}^0*h^1_{j,k}$ sont strictement homotopes, d’où la relation

$$
[h^0_{j,k}][v_{j,k}^1] = [v_{j,k}^0][h^1_{j,k}] \tag{2}
$$

dans $\varpi (X)$, pour tout couple $(j, k)\in  \{1, . . . , n\}^2$. D’autre part, pour tout couple d’entiers $(j, k)$, avec 2 $\leqslant j\leqslant n$ et 1 $\leqslant k\leqslant n$, on a $f\circ v_{j,k}^0=f\circ v_{j-1,k}^1$, d’où la relation

$$
\{v^0_{j,k}\}=\{v_{j-1,k}^1\} \tag{3}
$$

dans Coeg($f$). De même, pour tout couple d’entiers $(j, k)$ tels que $1\leqslant j\leqslant n$ et $2\leqslant k\leqslant n$, on a

$$
\{h^0_{j,k}\}=\{h^1_{j,k-1}\} \tag{4}
$$

Pour $j\in  \{1, . . . , n\}$, les chemins $f\circ c_j$ et $f\circ h^0_{j,1}$ coïncident. Par définition du coégalisateur Coeg($f$), on a donc $\{c_j\}=\{h^0_{j,1}\}$. De même, pour tout $j\in  \{1, . . . , n\},\{d_j\}=\{h^1_{j,n}\}$. Par suite, on a les relations

$$
u=\{h^0_{1,1}\}. . .\{h^0_{n,1}\},v=\{h^1_{1,n}\}. . .\{h^1_{n,n}\}
$$

D’après le lemme 3 ci-dessous, on a

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}\{v_{1,n}^1\}. . .\{v^1_{n,n}\}=\{v_{1,1}^0\}. . .\{v_{n,1}^0\}\{h^1_{n,1}\}. . .\{h^1_{n,n}\}
$$

Comme les chemins $t\mapsto \sigma (0, t)$ et $t\mapsto \sigma (1, t)$ sont constants, on a, pour $1\leqslant k\leqslant n,\{v^0_{1,k}\}=e_a$ et $\{v^1_{n,k}\}=e_b$ où $a$ et $b\in Y$ sont l’origine et le terme des flèches $u$ et $v$ de Coeg($f$). Il en résulte l’égalité

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}=\{h^0_{n,1}\}. . .\{h^1_{n,n}\}
$$

c’est-à-dire $u=v$.

#### Lemme 3 {#ta-iv-s4-lem-3 .statement tag=022V}

Soit G un groupoïde et soient $p, q$ des entiers $\geqslant 1$. Pour tout couple $(j, k)$ d’entiers tels que $0\leqslant j\leqslant p$ et $0\leqslant k\leqslant q$, soit $x_{j,k}$ un sommet de G ; pour tout couple $(j, k)$ tel que $1\leqslant j\leqslant p$ et $0\leqslant k\leqslant q$, soit $h_{j,k}$ une flèche de G reliant $x_{j-1,k}$ à $x_{j,k}$; pour tout couple $(j, k)$ tel que $0\leqslant j\leqslant p$ et $1\leqslant k\leqslant q$, soit $v_{j,k}$ une flèche de G reliant $x_{j,k-1}$ à $x_{j,k}$.

On suppose que, pour tout couple $(j, k)$ d’entiers tels que $1\leqslant j\leqslant p$ et $1\leqslant k\leqslant q$, les flèches $v_{j-1,k}$ et $h_{j,k}$ sont composables, de même que les flèches $h_{j,k-1}$ et $v_{j,k}$, et que l’on a $v_{j-1,k}h_{j,k}=h_{j,k-1}v_{j,k}$. Alors,

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q}h_{1,q}h_{2,q}. . . h_{p,q}
$$

Traitons d’abord le cas particulier où $q= 1$ et démontrons le résultat par récurrence sur $p$. Si $p= 1$, l’assertion à démontrer est vérifiée par hypothèse ; supposons-la vérifiée pour $p-1$ ; on a alors

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}=h_{1,0}h_{2,0}. . . h_{p-1,0}v_{p-1,1}h_{p,1}=v_{0,1}h_{1,1}. . . h_{p,1}
$$

par l’hypothèse de récurrence, d’où la relation pour $p$.

Démontrons maintenant le résultat par récurrence sur $q$. Il est vrai pour $q= 1$ d’après ce qui précède ; s’il est vrai pour $q-1$, on a alors

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q-1}h_{1,q-1}. . . h_{p,q-1}v_{p,q}
$$

D’après le cas $q= 1$, on a

$$
h_{1,q-1}. . . h_{p,q-1}v_{p,q}=v_{0,q}h_{1,q}. . . h_{p,q}
$$

d’où la relation voulue.

#### Exemple 1 {#ta-iv-s4-n7-exa-1 .statement tag=022W}

Le théorème s’applique lorsque l’application $f$ est étale et surjective.

#### Exemple 2 {#ta-iv-s4-n7-exa-2 .statement tag=022X}

Il s’applique aussi lorsque l’espace X est l’espace somme d’une famille $(V_i)_{i\in I}$ de parties de Y dont les intérieurs recouvrent Y, et que $f$ est l’application déduite des injections canoniques de chacun des $V_i$ dans Y.

### 8. Groupoïde de Poincaré d’un espace quotient

Soit X un espace topologique muni d’une opération continue d’un groupe discret G ; posons $Y = X/G$ et notons $f: X\rightarrow$ Y l’application canonique. Notons $|G|$ le groupoïde $\varpi (G)$; l’ensemble de ses sommets est G; pour $g, g'\in G$, il existe une unique flèche reliant $g$ à $g'$ si $g'=g'$, et aucune sinon. Par passage aux groupoïdes fondamentaux, l’opération $m: G\times X\rightarrow X$ induit un morphisme de groupoïdes $\varpi (m):|G| \times \varpi (X)\rightarrow \varpi (X)$. Soit $\varpi (X)/G$ le coégalisateur des deux morphismes de groupoïdes $\varpi (m)$ et $\varpi$(pr$_2)$ de $|G| \times \varpi (X)$ dans $\varpi (X)$ ; notons $\beta :\varpi (X)\rightarrow \varpi (X)/G$ le morphisme de groupoïdes canonique. On a $f\circ m=f\circ$ pr$_2$, donc $\varpi (f)\circ \varpi (m) =\varpi (f)\circ \varpi$(pr$_2)$. D’après la propriété universelle des coégalisateurs, il existe donc un unique morphisme de groupoïdes $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)$ tel que l’on ait $\varpi (f) =\varpi ''(f)\circ \beta$.

#### Théorème 3 {#ta-iv-s4-thm-3 .statement tag=022Y}

Soit X un espace topologique délaçable et soit G un groupe discret opérant proprement dans X ; soit $f: X\rightarrow X/G$ la surjection canonique. Le morphisme de groupoïdes canonique $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (X/G)$ introduit ci-dessus est un isomorphisme.

Notons Coeg($f$) le coégalisateur des deux morphismes de groupoïdes de $\varpi (X\times_YX)$ dans $\varpi (X)$ induits par les projections pr$_1$ et pr$_2$; soit $\gamma :\varpi (X)\rightarrow$ Coeg($f$) le morphisme de groupoïdes canonique. L’image de l’application $(m$, pr$_2): G\times X\rightarrow X\times X$ étant le sous-espace $X\times_YX$ de $X\times X$, les deux morphismes de groupoïdes $\gamma \circ \varpi (m)$ et $\gamma \circ \varpi$(pr$_2)$, de $|G|\times \varpi (X)$ dans Coeg($f$) sont égaux. D’après la propriété universelle de $\varpi (X)/G$, il existe un unique morphisme de groupoïdes $\alpha :\varpi (X)/G\rightarrow$ Coeg($f$) tel que $\gamma =\alpha \circ \beta$.

Notons aussi $\varpi '(f)$ l’unique morphisme de groupoïdes de Coeg($f$) dans $\varpi (Y)$ tel que $\varpi (f) =\varpi '(f)\circ \gamma$. D’après IV, p. 399, exemple 2, les hypothèses du th. 1 de IV, p. 398 sont vérifiées et le morphisme $\varpi '(f)$ est un isomorphisme. Comme

$$
\varpi (f) =\varpi '(f)\circ \gamma =\varpi '(f)\circ \alpha \circ \beta =\varpi ''(f)\circ \beta
$$

on a $\varpi ''(f) =\varpi '(f)\circ \alpha$. Ainsi, pour démontrer le théorème 3, il suffit de prouver que le morphisme $\alpha$ est un isomorphisme.

#### Lemme 4 {#ta-iv-s4-lem-4 .statement tag=022Z}

Pour tout chemin $c= (c_1, c_2)$ dans $X\times_YX$, on a $\beta ([c_1]) =\beta ([c_2])$.

Soit $c$ un tel chemin.

Soit $x\in X$, soit $K_x$ son fixateur dans G. D’après TG, III, p. 32, prop. 8, il existe un voisinage ouvert $U_x$ de $x$ dans X tel que $K_x\cdot U_x=$ $U_x,g\cdot U_x\cap U_x$ = $\emptyset$ pour tout $g\in$ G - $K_x$, et tel que l’application $f$ induise un homéomorphisme de $U_x/K_x$ sur un voisinage ouvert $V_x$ de $f(x)$ dans Y. Comme X est délaçable et que la restriction à $U_x$ de l’application $f$ est ouverte et fermée, on peut en outre supposer que $U_x$ est connexe et que l’image de l’homomorphisme canonique $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ est réduite à l’élément neutre. Les ouverts $(V_x)_{x\in X}$ ainsi construits forment un recouvrement ouvert de Y. D’après le lemme 4 de III, p. 272, appliqué à l’espace compact $\mathbf{I}$ et aux ouverts $(f\circ c_1)^{-1}(V_x)$ pour $x\in X$, il existe un entier $n\geqslant 1$ tel que pour tout $i\in  \{1, . . . , n\}$, il existe un point $x_i$ dans X tel que $c_1([^{i-1}_n,_n^i])$

soit contenu dans $\overset{-1}{f}(V_{x_i})$. Comme $f\circ c_1=f\circ c_2,c_2([^{i-1}_n,_n^i])$ est aussi

contenu dans $\overset{-1}{f}(V_{x_i})$.

Pour $j= 1$ ou 2 et pour $i\in  \{1, . . . , n\}$, notons $c_{j,i}$ le chemin dans X défini par $t\mapsto c_j(^{i+t-1}_n)$ ; on a $c_j=c_{j,1}* \cdots  *c_{j,n}($III, p. 291, remarque 1). Par suite, pour montrer que $\beta ([c_1]) =\beta ([c_2])$, il suffit de montrer que $\beta ([c_{1,i}]) =\beta ([c_{2,i}])$ pour tout entier $i\in  \{1, . . . , n\}$. Quitte à remplacer le chemin $(c_1, c_2)$ par le chemin $(c_{1,i}, c_{2,i})$, on suppose ainsi qu’il existe $x\in X$ tel que $(f\circ c_1)([0,1])\subset V_x$.

L’image réciproque de $V_x$ par $f$ est la réunion disjointe des parties connexes $g\cdot U_x$, où $g$ parcourt un système de représentants dans G de $G/K_x$. Pour $i= 1$ ou 2, soit $g_i$ un élément de G tel que le point $x_i=$ $g_i\cdot c_i(0)$ appartienne à $U_x$. L’image du chemin $g_i\cdot c_i$ est alors contenue dans $U_x$. Par définition du groupoïde $\varpi (X)/G$, on a $\beta ([g_i\cdot c_i]) =\beta ([c_i])$, ce qui permet de supposer que les images des chemins $c_1$ et $c_2$ sont contenues dans $U_x$ et que $g_1=g_2=e$.

Pour $s= 0$ ou 1, soit $d_s$ un chemin dans $U_x$ reliant $x$ à $c_1(s)$ et soit $g_s$ un élément de $K_x$ tel que $g_s\cdot c_2(s) =c_1(s)$. Les chemins $d_0*c_1*d_1$ et $d_0*(g_0\cdot c_2)*(g_0g_1^{-1}\cdot d_1)$ sont des lacets en $x$ dans $U_x$. Ils sont donc strictement homotopes dans X au lacet constant en $x$, car l’image de l’homomorphisme canonique $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ est réduite à l’élément neutre. Leurs classes ont en particulier même image par le morphisme de groupoïdes $\beta$, d’où

$$
\beta ([d_0])\beta ([c_1])\beta ([d_1])^{-1}=\beta ([d_0])\beta ([g_0\cdot c_2])\beta ([g_0g_1^{-1}\cdot d_1])^{-1}
$$

Puisque $\beta ([g\cdot c]) =\beta ([c])$ pour tout élément $g\in G$ et tout chemin $c$ dans X, il en résulte l’égalité $\beta ([c_1]) =\beta ([c_2])$, ainsi qu’il fallait démontrer.

D’après le lemme, les deux morphismes de groupoïdes $\beta \circ \varpi$(pr$_1)$ et $\beta \circ \varpi$(pr$_2)$ de $\varpi (X\times_YX)$ dans Coeg($f$) sont égaux. D’après la propriété universelle du coégalisateur, il existe donc un unique morphisme de groupoïdes $\alpha ':$ Coeg($f$)$\rightarrow \varpi (X)/G$ tel que $\beta =\alpha '\circ \gamma$. Le morphisme $\alpha '\circ \alpha$ est l’unique morphisme de groupoïdes $\varphi$ de $\varpi (X)/G$ dans lui-même tel que $\varphi \circ \beta =\beta$; on a donc $\alpha '\circ \alpha$ = Id$_{\varpi(X)/G}$. De même, $\alpha \circ \alpha '=$ Id$_{Coeg(f)}$. Par suite, $\alpha$ est un isomorphisme.
