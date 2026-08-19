---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 1
section_title: Produits fibrés et carrés cartésiens
lang: fr
source: ta-i-iv-fr
book_pages: TA I.1-TA I.24, TA I.139
pdf_pages: 0017-0040, 0155-0155
extraction: native
subsections:
    - "no": 1
      title: Structure de B-espace
      page: 1
      pdf_page: 17
    - "no": 2
      title: Opérations sur les B-espaces
      page: 2
      pdf_page: 18
    - "no": 3
      title: Produit fibré de deux B-espaces
      page: 3
      pdf_page: 19
    - "no": 4
      title: Changement de base
      page: 4
      pdf_page: 20
    - "no": 5
      title: Produit fibré d’une famille de B-espaces
      page: 5
      pdf_page: 21
    - "no": 6
      title: Carrés cartésiens
      page: 6
      pdf_page: 22
    - "no": 7
      title: Carrés cartésiens construits par passage aux sous-espaces
      page: 9
      pdf_page: 25
    - "no": 8
      title: Carrés cartésiens construits par produits, produits fibrés et sommes
      page: 11
      pdf_page: 27
    - "no": 9
      title: Composition de carrés cartésiens
      page: 15
      pdf_page: 31
    - "no": 10
      title: Applications strictes
      page: 17
      pdf_page: 33
    - "no": 11
      title: Applications universellement strictes
      page: 20
      pdf_page: 36
statements: 44
exercises: 2
content_sha256: 3d812fa4803abbe5bd107374726b69bde6a21ada1b7be0aa98125d4d9ada3bb3
---

## § 1. PRODUITS FIBRÉS ET CARRÉS CARTÉSIENS

### 1. Structure de B-espace

Soit B un espace topologique.

#### Définition 1 {#ta-i-s1-def-1 .statement tag=01L9}

On appelle B-espace topologique (ou simplement B-espace) un espace topologique X, muni d’une application continue $p$ de X dans B. L’application $p$ s’appelle la projection du B-espace X.

Soient X, $X'$ des B-espaces et $p,p'$ leurs projections respectives. On appelle B-morphisme de X dans $X'$ une application continue $f$ de X dans $X'$ telle que $p'\circ f=p$.

Il est parfois commode de désigner par $(X, p)$ le B-espace obtenu en munissant l’espace topologique X de l’application $p$ continue.

Le composé de deux B-morphismes est un B-morphisme. Les isomorphismes de B-espaces, aussi appelés B-isomorphismes, sont les B-morphismes qui sont des homéomorphismes.

Ainsi, si l’on appelle structure de B-espace sur un ensemble X la donnée d’une topologie sur X et d’une application continue $p: X\rightarrow B$, on peut prendre les B-morphismes pour morphismes de la structure de B-espace (E, IV, p. 11).

© N. Bourbaki et Springer-Verlag Berlin Heidelberg 2  016

N. Bourbaki, Topologie algébrique, DOI 10.1007/978-3-662-49361-8_1  1

Soient X, $X'$ des B-espaces. On note $\mathscr{C}_B(X; X')$ l’ensemble des B-morphismes de X dans $X'$, Isom$_B(X; X')$ l’ensemble des B-isomorphismes de X dans $X'$ et Aut$_B(X)$ l’ensemble des B-automorphismes de X, c’est-à-dire des B-isomorphismes de X dans X.

Soient X un B-espace et $p$ sa projection. Si l’on munit B de la structure de B-espace dont la projection est Id$_B$, l’ensemble $\mathscr{C}_B(B; X)$ est l’ensemble des sections (E, II, p. 18, déf. 11) continues de $p$.

Soient X un B-espace, $p$ sa projection et $b$ un point de B. Le sous-espace $\overset{-1}{p}(b)$ de X est appelé la fibre de X en $b$ (ou la fibre de $p$ en $b$) et noté $X_b$. Pour qu’une application continue $f$ de X dans un B-espace $X'$ soit un B-morphisme, il faut et il suffit que $f(X_b)$ soit contenu dans $X'_b$ pour tout $b\in B$.

Soient X un B-espace et $p$ sa projection. Soit $f$ une application continue d’un espace topologique $B'$ dans B. Une application continue $g: B'\rightarrow X$ telle que $p\circ g=f$ est appelée un relèvement continu de $f$ à X. Autrement dit, si l’on munit $B'$ de la structure de B-espace de projection $f$, les relèvements continus de $f$ à X sont les B-morphismes de $B'$ dans X.

### 2. Opérations sur les B-espaces

Soit B un espace topologique.

Soient X un B-espace et $p$ sa projection. On munit tout sous-espace topologique Y de X de la structure de B-espace dont la projection est $p|Y$. Soit A un sous-espace de B; muni de l’application $p_A:\overset{-1}{p}(A)\rightarrow A$ déduite de $p$ par passage aux sous-ensembles, l’espace topologique $\overset{-1}{p}(A)$, est un A-espace. On l’appelle le A-espace induit par $(X, p)$ au-dessus de A et on le note parfois $X_A$.

Soit $(X_i)_{i\in I}$ une famille de B-espaces, et soit $p_i$ la projection de $X_i$. L’espace somme $X =\coprod_{i\in I}X_i$ (TG, I, p. 15), muni de l’application $p: X\rightarrow$ B définie par $p(i, x) =p_i(x)$ (pour $i\in$ I et $x\in X_i$), est un B-espace appelé la somme de la famille de B-espaces $(X_i)_{i\in I}$. Les injections canoniques $X_i\rightarrow X$ sont des B-morphismes.

Soient X un B-espace, $p$ sa projection et soit R une relation d’équivalence sur X. Notons $X/R$ l’espace quotient (TG, I, p. 20, déf. 3). Si l’application $p: X\rightarrow B$ est compatible avec la relation R (E, II, p. 44), l’application $p': X/R\rightarrow B$ déduite de $p$ par passage au quotient est continue (TG, I, p. 21, prop. 6) ; le B-espace obtenu en munissant $X/R$ de la projection $p'$ est alors appelé le B-espace quotient de X par la relation R.

### 3. Produit fibré de deux B-espaces

Soient B un espace topologique, X et $X'$ des B-espaces, $p$ et $p'$ leurs projections respectives. Notons $X\times_BX'$ le sous-espace topologique de $X\times X'$ formé des couples $(x, x')$ tels que $p(x) =p'(x')$. L’application $q: X\times_BX'\rightarrow B$ définie par $q(x, x') =p(x)$ est continue.

#### Définition 2 {#ta-i-s1-def-2 .statement tag=01LA}

L’espace topologique $X\times_BX'$ s’appelle le produit fibré de X et $X'$ au-dessus de B. Le B-espace obtenu en munissant $X\times_BX'$ de l’application $q$ s’appelle le B-espace produit de X et $X'$.

Les restrictions à $X\times_BX'$ des projections de $X\times X'$ dans X et dans $X'$ sont encore notées pr$_1$ et pr$_2$ et appelées première et seconde projections du produit fibré. Elles sont continues et sont des B-morphismes, car on a $q=p\circ$ pr$_1=p'\circ$ pr$_2$.

On prendra garde que $X\times_BX'$ peut être vide même si X et $X'$ sont non vides : en effet, la relation $X\times_BX'=\emptyset$ équivaut à dire que $p(X)$ et $p'(X')$ sont disjoints.

Soient Y un B-espace et $u: Y\rightarrow X,u': Y\rightarrow X'$ des B-morphismes. Il existe un unique B-morphisme $v: Y\rightarrow X\times_BX'$ tel que pr$_1\circ v=u$ et pr$_2\circ v$ = $u'$ (propriété universelle du B-espace produit de deux B-espaces) : c’est l’application $y\mapsto (u(y), u'(y))$ de Y dans $X\times_BX'$, que l’on note parfois $(u, u')$.

Soient $X,X',Y,Y'$ des B-espaces, soient $f: X\rightarrow Y,f': X'\rightarrow Y'$ des B-morphismes. L’application $(x, x')\mapsto (f(x), f'(x'))$ est un B-morphisme de $X\times_BX'$ dans $Y\times_BY'$, que l’on note $f\times_Bf'$ et que l’on appelle l’extension de $f$ et $f'$ aux produits fibrés.

#### Exemple 1 {#ta-i-s1-n3-exa-1 .statement tag=01LB}

Soient X et $X'$ des B-espaces, alors l’application $(x, x')\mapsto (x', x)$ définit un B-isomorphisme de $X\times_BX'$ sur $X'\times_BX$.

#### Exemple 2 {#ta-i-s1-n3-exa-2 .statement tag=01LC}

Soient X, $X',X''$ des B-espaces et $p,p',p''$ leurs projections respectives. Le B-espace produit $(X\times_BX')\times_BX''$ est le sous-espace topologique $X\times_BX'\times_BX''$ de $X\times X'\times X''$ formé des triplets $(x, x', x'')$ tels que $p(x) =p'(x') =p''(x'')$, muni de la projection $q: X\times_BX'\times_BX''\rightarrow B$ définie par $q(x, x', x'') =p(x)$.

#### Exemple 3 {#ta-i-s1-n3-exa-3 .statement tag=01LD}

Soient X un B-espace et $p$ sa projection. Le produit fibré $X\times_BX$ de X et X au-dessus de B est appelé le carré fibré de X. C’est le sous-espace de $X\times X$ formé des couples $(x, x')$ tels que $p(x) =p(x')$. Il est muni de la structure de B-espace dont la projection est l’application $(x, x')\mapsto$ $p(x)$. La diagonale $\Delta_X$ de $X\times X$ (E, II, p. 13) est contenue dans $X\times_BX$ ; on l’appelle encore la diagonale de $X\times_BX$. L’application $x\mapsto (x, x)$ de X dans $X\times_BX$ est un B-morphisme, appelé le B-morphisme diagonal et souvent noté $\delta_X$; il définit un B-isomorphisme de X sur $\Delta_X$ (TG, I, p. 25, cor. 2).

#### Exemple 4 {#ta-i-s1-n3-exa-4 .statement tag=01LE}

Soit $(B_i)_{i\in I}$ une famille d’espaces topologiques et soient, pour tout $i\in I$, $(X_i, p_i)$ et $(Y_i, q_i)$ des $B_i$-espaces. Posons $B =\prod_{i\in I}B_i$, $X =\prod_{i\in I}X_i$ et $Y =\prod_{i\in I}Y_i$. Muni de l’application continue $p=\prod_ip_i$ (resp. $q=\prod_iq_i$), l’espace topologique X (resp. Y) est un B-espace. Par l’isomorphisme d’associativité des produits topologiques de $\prod_i(X_i\times Y_i)$ sur $(\prod_iX_i)\times (\prod_iY_i) = X\times Y$ (TG, I, p. 25, prop. 2), le sous-espace $\prod_i(X_i\times_{B_i}Y_i)$ de $\prod_i(X_i\times Y_i)$ s’identifie à $X\times_BY$.

#### Exemple 5 {#ta-i-s1-n3-exa-5 .statement tag=01LF}

Soient $(X_i)_{i\in I}$ et $(Y_j)_{j\in J}$ des familles de B-espaces. Soient X et Y leurs sommes. Pour tout $(i, j)\in I\times J$, l’application $(x, y)\mapsto$ $((i, x),(j, y))$ est un B-isomorphisme de $X_i\times_BY_j$ sur le sous-espace $(\{i\} \times X_i)\times_B(\{j\} \times Y_j)$ de $X\times_BY$. Comme ces derniers forment une partition de $X\times_BY$ en sous-ensembles ouverts, l’application

$$
h:\coprod_{(i,j)\in I\times J}(X_i\times_BY_j)\rightarrow X\times_BY
$$

définie par $h((i, j),(x, y)) = ((i, x),(j, y))$ est un B-isomorphisme.

### 4. Changement de base

Soient B, $B'$ des espaces topologiques et $f: B'\rightarrow B$ une application continue. Soit X un B-espace. L’application $f$ munit $B'$ d’une structure de B-espace, ce qui permet de définir le produit fibré $B'\times_BX$. Celui-ci, muni de l’application pr$_1: B'\times_BX\rightarrow B'$ est un $B'$-espace appelé le $B'$-espace déduit du B-espace X par le changement de base $f: B'\rightarrow B$ (ou par changement de base de B à $B'$ suivant $f$). On l’appelle aussi le $B'$-espace image réciproque de X par $f$. On le note $f^*(X)$, ou parfois $X_{B'}$ lorsqu’il n’y a pas de confusion possible sur l’application $f$.

Lorsque $B'$ est un sous-espace de B et que $f: B'\rightarrow B$ est l’injection canonique, l’application $(b', x)\mapsto x$ de $B'\times_BX'$ dans $\overset{-1}{p}(B')$ (où $p$ est la projection de X) est un $B'$-isomorphisme de $f^*(X)$ sur le $B'$-espace induit par X au-dessus de $B'$.

Soient Y un second B-espace et $u: X\rightarrow Y$ un B-morphisme. L’application Id$_{B'}\times_Bu: B'\times_BX\rightarrow B'\times_BY$ est un $B'$-morphisme, appelé le $B'$-morphisme déduit du B-morphisme $u$ par le changement de base $f: B'\rightarrow B$ et parfois noté $f^*(u)$, ou $u_{B'}$ lorsqu’il n’y a pas de confusion possible sur l’application $f$. C’est l’unique $B'$-morphisme $v$ de $B'\times_BX$ dans $B'\times_BY$ tel que pr$_2\circ v=u\circ$ pr$_2$.

Soit $B''$ un espace topologique et soit $g: B''\rightarrow B'$ une application continue. Alors l’application donnée par $(b'',(b', x))\mapsto (b'', x)$ est un isomorphisme de $B''$-espaces de $g^*(f^*(X))$ sur $(f\circ g)^*(X)$, qu’on dira canonique.

### 5. Produit fibré d’une famille de B-espaces

Soit $(X_i)_{i\in I}$ une famille de B-espaces. Soient $p_i: X_i\rightarrow B$ leurs projections. Notons $\prod_BX_i$ le sous-espace topologique de $B\times \prod_{i\in I}X_i$ formé des couples $(b,(x_i)_{i\in I})$ tels que $p_i(x_i) =b$ pour tout $i\in I$. L’application $p:\prod_BX_i\rightarrow B$ définie par $p(b,(x_i)_{i\in I}) =b$ est continue.

#### Définition 3 {#ta-i-s1-def-3 .statement tag=01LG}

L’espace topologique $\prod_BX_i$ s’appelle le produit fibré de la famille $(X_i)_{i\in I}$ au-dessus de B. Le B-espace obtenu en munissant $\prod_BX_i$ de l’application $p$ s’appelle le B-espace produit de la famille $(X_i)_{i\in I}$.

Soit $j\in I$. L’application $(b, x)\mapsto$ pr$_j(x)$ de $\prod_BX_i$ dans $X_j$ est appelée la projection d’indice $j$ du produit fibré et encore notée pr$_j$. Elle est continue. C’est un B-morphisme, car on a $p=p_j\circ$ pr$_j$.

Soient Y un B-espace et $q$ sa projection. Pour tout $i\in$ I, soit $u_i: Y\rightarrow X_i$ un B-morphisme. Il existe un unique B-morphisme $v: Y\rightarrow$ $\prod_BX_i$ tel que pr$_i\circ v=u_i$ pour tout $i\in I$ (propriété universelle du B-espace produit) : c’est l’application de Y dans $\prod_BX_i$, définie par $y\mapsto (q(y),(u_i(y))_{i\in I})$, que l’on note parfois $(u_i)_{i\in I}$.

Soient $(X_i)_{i\in I}$ et $(Y_i)_{i\in I}$ des familles de B-espaces et, pour tout $i\in I$, soit $f_i: X_i\rightarrow Y_i$ un B-morphisme. L’application $(b,(x_i)_{i\in I})\mapsto$ $(b,(f_i(x_i))_{i\in I})$ est un B-morphisme de $\prod_BX_i$ dans $\prod_BY_i$ que l’on note $\prod_Bf_i$ et que l’on appelle l’extension de la famille $(f_i)_{i\in I}$ aux produits fibrés.

#### Exemple 1 {#ta-i-s1-n5-exa-1 .statement tag=01LH}

Lorsque l’ensemble I est vide, l’ensemble $\prod_{i\in I}X_i$ est réduit à un élément et le B-espace $\prod_BX_i$ s’identifie à B (muni de la projection Id$_B$).

#### Exemple 2 {#ta-i-s1-n5-exa-2 .statement tag=01LI}

Lorsque I n’est pas vide, on déduit de l’application $(b, x)\mapsto x$ de $B\times \prod_{i\in I}X_i$ dans $\prod_{i\in I}X_i$, par passage aux sous-espaces, un homéo-morphisme de $\prod_BX_i$ sur le sous-espace de $\prod_{i\in I}X_i$ formé des familles $(x_i)_{i\in I}$ telles que $p_i(x_i) =p_j(x_j)$ pour tous $i, j\in I$. Ce sous-espace sera appelé, par abus, le produit fibré de la famille $(X_i)_{i\in I}$.

#### Exemple 3 {#ta-i-s1-n5-exa-3 .statement tag=01LJ}

Lorsque l’ensemble I est un ensemble à un élément $\alpha$ (resp. à deux éléments $\alpha$ et $\beta$; resp. à trois éléments $\alpha ,\beta ,\gamma$ ), l’application pr$_{\alpha}$ (resp. (pr$_{\alpha}$, pr$_{\beta}$) ; resp. (pr$_{\alpha}$, pr$_{\beta}$, pr$_{\gamma}$)) de $\prod_BX_i$ dans $X_{\alpha}$ (resp. dans $X_{\alpha}\times_BX_{\beta}$; resp. dans $X_{\alpha}\times_BX_{\beta}\times_BX_{\gamma}$) est un B-isomorphisme. Cela nous permettra de déduire les propriétés du produit fibré de deux ou trois B-espaces de celles du produit fibré de familles de B-espaces.

Soit $(X_i)_{i\in I}$ une famille de B-espaces et soit J une partie de I. On déduit de l’application Id$_B\times$ pr$_J$ de $B\times \prod_{i\in I}X_i$ dans $B\times \prod_{i\in J}X_i$, par passage aux sous-ensembles, un B-morphisme $\prod_{i\in IB}X_i\rightarrow \prod_{i\in JB}X_i$. On le

note encore pr$_J$ et on l’appelle la projection d’indice J du produit fibré.

Soit $(X_i)_{i\in I}$ une famille de B-espaces. Soit $(J_{\lambda})_{\lambda\in L}$ une partition

de I. L’application (pr$_{J_{\lambda}}$)$_{\lambda\in L}$ de $\prod_{i\in IB}X_i\rightarrow \prod_{\lambda\in LB}(\prod_{i\in J_{\lambda}B}X_i)$ est un

B-isomorphisme (« associativité » des produits fibrés de B-espaces).

### 6. Carrés cartésiens

Soient B, $B'$, X, $X'$ des espaces topologiques et soient $f: B'\rightarrow B$, $f': X'\rightarrow X,p: X\rightarrow B,p': X'\rightarrow B'$ des applications continues. On peut représenter un tel quadruplet $(f, f', p, p')$ par un diagramme

${X'}^{f'}$ X

$$
p'p \tag{1}
$$

${B'}^f$ B

(E, II, p. 14). On dira alors : « Considérons le diagramme carré (1) », ou simplement « le carré (1) », au lieu de dire : « Considérons le quadruplet $(f, f', p, p')$ d’applications continues ». On dit que le carré (1) est commutatif, si l’égalité

$$
f\circ p'=p\circ f'
$$

est satisfaite. Dans ce cas, on munit souvent $B'$, X et $X'$ des structures de B-espaces définies par les applications $f,p$ et $f\circ p'=p\circ f'$ respectivement ; les applications $p'$ et $f'$ sont alors des B-morphismes.

#### Définition 4 {#ta-i-s1-def-4 .statement tag=01LK}

On dit que le carré (1) est un carré cartésien d’espaces topologiques (ou, simplement, qu’il est cartésien) s’il est commutatif et que, pour tout espace topologique Y et tout couple d’applications continues $u: Y\rightarrow B',v: Y\rightarrow X$ telles que $f\circ u=p\circ v$, il existe une unique application continue $w: Y\rightarrow X'$ telle que $p'\circ w=u$ et $f'\circ w=v$.

Pour que le carré (1) soit cartésien, il faut et il suffit que le carré

$$
{X'}^{p'}B'
$$

$$
(1')f'f
$$

X $^p$ B

soit cartésien.

#### Proposition 1 {#ta-i-s1-prop-1 .statement tag=01LL}

Pour que le carré (1) soit cartésien, il faut et il suffit qu’il soit commutatif et que, pour tout B-espace Y et tout couple de B-morphismes $u: Y\rightarrow B',v: Y\rightarrow X$, il existe un unique B-morphisme $w: Y\rightarrow X'$ tel que $p'\circ w=u$ et $f'\circ w=v$.

Supposons que le carré (1) est cartésien. Soit Y un B-espace et soient $u: Y\rightarrow B',v: Y\rightarrow X$ des B-morphismes. Les applications $f\circ u$ et $p\circ v$ sont toutes deux égales à la projection du B-espace Y ; l’unique application continue $w$ telle que $p'\circ w=u$ et $f'\circ w=v$ est alors un B-morphisme. Cela prouve la nécessité de la condition.

Inversement, supposons cette condition satisfaite. Soit Y un espace topologique et soient $u: Y\rightarrow B',v: Y\rightarrow X$ des applications continues telles que $f\circ u=p\circ v$. Lorsqu’on munit Y de la structure de B-espace définie par $f\circ u,u$ et $v$ sont des B-morphismes. Toute application continue $w: Y\rightarrow X'$ telle que $p'\circ w=u$ et $f'\circ w=v$ étant un B-morphisme, il en existe une et une seule.

#### Proposition 2 {#ta-i-s1-prop-2 .statement tag=01LM}

Soient B, $B'$ et X des espaces topologiques et $p: X\rightarrow B,f: B'\rightarrow B$ des applications continues.

a) Le carré

$B'\times_BX^{pr_2}$ X

(2) pr$_{_1}p$

${B'}^f$ B

est un carré cartésien.

b) Pour tout carré commutatif

${X'}^{f'}$ X

$$
p'p \tag{3}
$$

${B'}^f$ B

il existe une unique application continue $h: X'\rightarrow B'\times_BX$ telle que pr$_1\circ h=p'$ et pr$_2\circ h=f'$.

c) Le carré commutatif (3) est cartésien si et seulement si $h$ est un homéomorphisme.

L’assertion a) résulte de la prop. 1 et de la propriété universelle du B-espace produit de deux B-espaces (I, p. 3). L’assertion b) en découle.

Si le carré (3) est cartésien, il existe une unique application continue $h': B'\times_BX\rightarrow X'$ telle que $f'\circ h'$ = pr$_2$ et $p'\circ h'=$ pr$_1$. On a $f'\circ h'\circ h=f'$ et $p'\circ h'\circ h=p'$, d’où $h'\circ h=$ Id$_{X'}$ puisque le carré (3) est cartésien. On a pr$_1\circ h\circ h'$ = pr$_1$ et pr$_2\circ h\circ h'$ = pr$_2$, d’où $h\circ h'=$ Id$_{B'\times_BX}$ puisque le carré (2) est cartésien. Cela prouve que $h$ est un homéomorphisme.

Inversement, supposons que $h$ soit un homéomorphisme ; comme le carré (2) est cartésien, le carré (3) est aussi cartésien.

L’application $h: X'\rightarrow B'\times_BX$ dont l’existence et l’unicité est affirmée par l’assertion b) de la proposition précédente sera dite canonique : c’est l’application notée $(p', f')$ en I, p. 3.

#### Proposition 3 {#ta-i-s1-prop-3 .statement tag=01LN}

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien. Pour toute section continue $s$ de $p'$, l’application $f'\circ s$ est un relèvement continu de $f$ à X. L’application $s\mapsto f'\circ s$ est une bijection de $\mathscr{C}_{B'}(B'; X')$ sur $\mathscr{C}_B(B'; X)$.

Si $s: B'\rightarrow X'$ est une section continue de $p'$, on a $p\circ f'\circ s=$ $f\circ p'\circ s=f$, ce qui prouve que $f'\circ s$ est un relèvement continu de $f$ à X, i.e. un B-morphisme de $B'$ dans X. Inversement, soit $g: B'\rightarrow X$ un B-morphisme. On a $f\circ$ Id$_{B'}=p\circ g$; il existe donc, par définition d’un carré cartésien, une unique application continue $s: B'\rightarrow X'$ telle que $p'\circ s=$ Id$_{B'}$ et $f'\circ s=g$, d’où la proposition.

### 7. Carrés cartésiens construits par passage aux sous-espaces

#### Proposition 4 {#ta-i-s1-prop-4 .statement tag=01LO}

Soit

${X'}^{f'}$ X

$$
p'p \tag{4}
$$

${B'}^f$ B

un carré cartésien et soient $B_0,B'_0,X_0$ des sous-espaces de B, $B'$ et X respectivement. Supposons qu’on ait $f(B'_0)\subset B_0,p(X_0)\subset B_0$ et posons $X'_0=(\overset{-1}{p}')(B'_0)\cap (\overset{-1}{f}')(X_0)$. Alors, le carré

$$
{X'_0}^{f'_0}X_0
$$

$$
(4')p'_{_0}p_{_0}
$$

$$
{B'_0}^{f_0}B_0
$$

(où les applications $f_0,f'_0,p_0,p'_0$ sont déduites de $f,f',p,p'$ respectivement par passage aux sous-ensembles) est cartésien.

Considérons l’application canonique $h: X'\rightarrow B'\times_BX$ déduite du diagramme commutatif (4). Comme le carré (4) est cartésien, $h$ est un

homéomorphisme. Par construction, on a $X'_0=\overset{-1}{h}(B'_0\times_{B_0}X_0)$ et l’application $h_0: X'_0\rightarrow B'_0\times_{B_0}X_0$ déduite du diagramme commutatif ($4'$) est déduite de $h$ par passage aux sous-ensembles. C’est donc un homéomorphisme et le carré ($4'$)est cartésien (prop. 2).

#### Corollaire {#ta-i-s1-n7-cor-1 .statement tag=01LP}

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien.

a) Pour tout point $b'$ de $B'$, l’application $f'$ induit un homéomorphisme de la fibre $X'_{b'}$ de $p'$ sur la fibre $X_{f(b')}$ de $p$.

b) Si l’application $p$ est injective ( resp. surjective, resp. bijective), il en est de même de $p'$.

Soit $b'$ un point de $B'$. Posons $b=f(b')$. Pour tout $x'\in X'_{b'}$, on a $p(f'(x')) =f(p'(x')) =f(b') =b$, d’où $f'(x')\in X_b$. Cela prouve que

l’on a $X'_{b'}\subset (\overset{-1}{f}')(X_b)$. Dans la prop. 4, prenons $B_0=\{b\},B'_0=\{b'\}$ et $X_0= X_b$; on a alors $X'_0= X'_{b'}$, d’où l’assertion a).

Pour que l’application $p$ soit injective (resp. surjective, resp. bijective), il faut et il suffit que le cardinal de chacune de ses fibres soit inférieur (resp. supérieur, resp. égal) à 1. L’assertion b) en résulte.

#### Exemple {#ta-i-s1-n7-exa-1 .statement tag=01LQ}

Soient $(X, p)$ un B-espace et A un sous-espace de B. Le carré

$\overset{-1}{p}(A)^j$ X

$$
p_{_A}p \tag{5}
$$

A $^i$ B

(où $i$ et $j$ sont les injections canoniques) est cartésien.

En particulier, si A et $A'$ sont des sous-espaces de l’espace topologique B, le carré

$$
A\cap A'A'
$$

(6)

A B

(où les flèches sont les injections canoniques) est cartésien.

### 8. Carrés cartésiens construits par produits, produits fibrés et sommes

#### Proposition 5 {#ta-i-s1-prop-5 .statement tag=01LR}

Soit I un ensemble et, pour tout $i\in I$, soit

$$
{X'_i}^{f'_i}X_i
$$

$$
p'_{_i}p_{_i} \tag{7}
$$

$$
{B'_i}^{f_i}B_i
$$

un carré cartésien. Le carré

$$
\prod i\in IX'if'\prod i\in IXi
$$

$$
(7')p'p
$$

$$
\prod i\in IB'if\prod i\in IBi
$$

(où $f,f',p,p'$ sont les extensions des familles $(f_i)$, $(f'_i)$, $(p_i)$, $(p'_i)$ aux produits) est cartésien.

Soit Y un espace topologique, soient $u: Y\rightarrow \prod_iB'_i$ et $v: Y\rightarrow \prod_iX_i$ des applications continues telles que $f\circ u=p\circ v$. Pour $i\in I$, posons $u_i$ = pr$_i\circ u$ et $v_i=$ pr$_i\circ v$; on a $f_i\circ u_i=p_i\circ v_i$ et il existe une unique application continue $w_i: Y\rightarrow X'_i$ telle que $p'_i\circ w_i=u_i$ et $f'_i\circ w_i=v_i$. Alors, l’application $w= (w_i)$ est une application continue de Y dans $\prod_iX'_i$ telle que $p'\circ w=u$ et $f'\circ w=v$, et c’est la seule ayant ces propriétés.

#### Corollaire 1 {#ta-i-s1-prop-5-cor-1 .statement tag=01LS}

Soit X un B-espace, soit $p$ sa projection et soit F un espace topologique. Le carré

$$\begin{array}{ccc} X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array} \tag{8}$$

est cartésien.

Soit P un espace topologique réduit à un point. Le corollaire 1 résulte de la prop. 5 appliquée aux carrés cartésiens

$$\begin{array}{ccccccc} X & \overset{\mathrm{Id}_X}{\longrightarrow} & X & & F & \longrightarrow & P \\ {\scriptstyle p}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{et} & {\scriptstyle \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_P} \\ B & \overset{\mathrm{Id}_B}{\longrightarrow} & B & & F & \longrightarrow & P \end{array}.$$

Soient B et $B'$ des espaces topologiques et soit $f: B'\rightarrow$ B une application continue. Soit I un ensemble et, pour tout $i\in I$, soient $X_i$ un B-espace, $X'_i$ un $B'$-espace et $f'_i: X'_i\rightarrow X_i$ une application continue telle que le carré

$$
{X'_i}^{f'_i}X_i
$$

(9)

${B'}^f$ B

soit commutatif. Il existe une unique application continue

$$
f':\prod_{i\in IB'}X'_i\rightarrow \prod_{i\in IB}X_i
$$

telle que pr$_i\circ f'=f'_i\circ$ pr$_i$ pour tout $i\in I$ et telle que le carré

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
(9')
$$

${B'}^f$ B soit commutatif (cette dernière condition résultant des autres si I $=\not\emptyset$ ) $:$ c’est l’application déduite de l’application

$$
f\times \prod_{i\in I}f'_i: B'\times \prod_{i\in I}X'_i\rightarrow B\times \prod_{i\in I}X_i
$$

par passage aux sous-ensembles. Avec ces notations :

#### Corollaire 2 {#ta-i-s1-prop-5-cor-2 .statement tag=01LT}

Si le carré (9) est cartésien pour tout $i\in I$, le carré ($9'$) est cartésien.

On déduit de la prop. 5 un carré cartésien

$$
B'\times \prod_i{X'_i}^{Id_B\times}\prod_{_i}^{f'_i}B\times \prod_iX_i
$$

$$
B'\times (B')^{If\times}\prod_{_i}^fB\times B^I
$$

Notons $\Delta_{B'}$ et $\Delta_B$ les diagonales de $B'\times (B')^I$ et $B\times B^I$. Le diagramme

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
\Delta_{B'}\Delta_B
$$

déduit du précédent par passage aux sous-espaces est cartésien (I, p. 9, prop. 4). Il s’identifie au diagramme ($9'$).

#### Exemple 1 {#ta-i-s1-n8-exa-1 .statement tag=01LU}

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien. Alors le corollaire 2 fournit un carré cartésien

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

${B'}^f$ B .

On a la relation $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$. En effet, par la prop. 2 de I, p. 8, il suffit de considérer le cas où $X'= B'\times_BX$. Soit alors $((b, x),(b, x'))$ un élément de $X'\times_{B'}X'$ avec $b\in B'$ et $x, x'\in X$. Cet élément appartient à $\overset{-1}{\varphi}(\Delta_X)$ si et seulement si $x=x'$.

#### Proposition 6 {#ta-i-s1-prop-6 .statement tag=01LV}

Soit I un ensemble et, pour tout $i\in I$, soit

${X'_i}^{f'_i}$ X

$$
p'_{_i}p \tag{10}
$$

${B'_i}^{f_i}$ B

un carré cartésien. Soient $X'$ et $B'$ les espaces sommes des familles $(X'_i)$ et $(B'_i)$ respectivement. Soient $f: B'\rightarrow B,f': X'\rightarrow X$ et $p': X'\rightarrow B'$ les applications déduites des familles $(f_i)$, $(f'_i)$ et $(p'_i)$ respectivement. Le carré

${X'}^{f'}$ X

$$
(10')p'p
$$

${B'}^f$ B

est cartésien.

Les applications $f,f'$ et $p'$ sont continues. La commutativité du carré ($10'$)résulte de sa définition. Notons $h_i$ l’homéomorphisme canonique de $X'_i$ sur $B'_i\times_BX$ (I, p. 8, prop. 2) et $h: X'\rightarrow B'\times_BX$ l’application canonique (loc. cit.). On a $h=h''\circ h'$ où $h': X'\rightarrow \coprod(B'_i\times_BX)$ est l’homéomorphisme déduit des $h_i$ et $h'':\coprod(B'_i\times_BX)\rightarrow (\coprod B'_i)\times_BX$ est celui défini dans l’exemple 5 de I, p. 4. On conclut par la prop. 2 de I, p. 8.

#### Exemple 2 {#ta-i-s1-n8-exa-2 .statement tag=01LW}

Soit $(X, p)$ un B-espace et soit $(A_k)_{k\in K}$ une famille de sous-espaces de B. Soit A l’espace somme de la famille $(A_k)_{k\in K}$ et soit Y l’espace somme de la famille $(\overset{-1}{p}(A_k))_{k\in K}$; notons $i: A\rightarrow B$, $j: Y\rightarrow X$ et $p': Y\rightarrow A$ les applications déduites des injections canoniques de $A_k$ dans B, des injections canoniques de $\overset{-1}{p}(A_k)$ dans X, et des applications $p_{A_k}:\overset{-1}{p}(A_k)\rightarrow A_k$, pour $k\in K$. Le carré

Y $^j$ X

$$
p'p \tag{11}
$$

A $^i$ B est cartésien ; cela résulte de l’exemple de I, p. 10 et de la prop. 6.

### 9. Composition de carrés cartésiens

#### Proposition 7 {#ta-i-s1-prop-7 .statement tag=01LX}

Soient

${X''}^{g'}X'{X'}^{f'}$ X

(12) $p''p'$ et (13) $p'p$

${B''}^gB'{B'}^f$ B

des carrés commutatifs ; considérons le carré

${X''}^{f'\circ g'}$ X

$$
p''p \tag{14}
$$

${B''}^{f\circ g}$ B .

Il est commutatif. Si les carrés (12) et (13) sont cartésiens, il en est de même du carré (14). Si les carrés (13) et (14) sont cartésiens, il en est de même du carré (12).

Le carré (14) est commutatif, car on a $p\circ f'\circ g'=f\circ p'\circ g'=f\circ g\circ p''$.

Notons $h': X''\rightarrow B''\times_{B'}X',h: X'\rightarrow B'\times_BX$ et $h'': X''\rightarrow B''\times_BX$ les applications continues canoniques déduites des carrés commutatifs (12), (13) et (14). Par ailleurs, notons

$$
j: B''\times_BX\rightarrow B''\times_{B'}(B'\times_BX)
$$

l’application continue qui à $(b'', x)$ associe $(b'', g(b''), x)$. C’est un homéomorphisme et l’on a $j\circ h''=$ (Id$_{B''}\times_Bh$)$\circ h'$.

Supposons que le carré (13) soit cartésien. Alors, $h$ est un homéo-morphisme (I, p. 8, prop 2), donc l’application Id$_{B''}\times_Bh$ est un homéomorphisme, et $h''$ est un homéomorphisme si et seulement $h'$ en est un. Cela signifie que le carré (12) est cartésien si et seulement si le carré (14) est cartésien (loc. cit.).

Avec les notations de la proposition 7, on dit parfois que le carré (14) est le carré composé des carrés (13) et (12). La première assertion exprime que le carré composé de deux carrés cartésiens est cartésien. En particulier, les $B''$-espaces $g^*(f^*(X))$ et $(f\circ g)^*(X)$ sont isomorphes.

#### Remarque 1 {#ta-i-s1-n9-rem-1 .statement tag=01LY}

Il peut arriver que les carrés (12) et (14) soient cartésiens sans que le carré (13) le soit (I, p. 139, exerc. 2).

#### Remarque 2 {#ta-i-s1-n9-rem-2 .statement tag=01LZ}

Soient $p: X\rightarrow B$ et $f: B'\rightarrow B$ des applications continues. L’application $g: B'\rightarrow B'\times B$ définie par $g(b') = (b', f(b'))$ est un homéo-morphisme de $B'$ sur le graphe G de l’application $f$ (TG, I, p. 25, cor. 2) et le produit fibré $B'\times_BX$ s’identifie (I, p. 6) au sous-espace de $B'\times X$, image réciproque de G par l’application Id$_{B'}\times p: B'\times X\rightarrow B'\times B$. D’après l’exemple de I, p. 10 et le cor. 1 de la prop. 5 (I, p. 11), les carrés

$B'\times_BX^iB'\times XB'\times X^{pr_2}$ X

pr$_1$ Id$_{B'}\times p$ et Id$_{B'}\times pp$

${B'}^gB'\times BB'\times B^{pr_2}$ B

(où $i$ désigne l’injection canonique) sont cartésiens et le carré cartésien

$B'\times_BX^{pr_2}$ X

pr$_1p$

${B'}^f$ B

est leur composé. En d’autres termes, tout carré cartésien s’identifie au carré composé d’un carré cartésien obtenu par produit (I, p. 11, cor. 1 de la prop. 5, carré (8)) et d’un carré cartésien obtenu par passage aux sous-espaces (I, p. 10, exemple, carré (5)).

#### Remarque 3 {#ta-i-s1-n9-rem-3 .statement tag=01M0}

Soient

$X_1^{g_1}$ X $X_2^{g_2}$ X

(15) $p_{_1}p$ et (16) $p_{_2}p$

$B_1^{f_1}$ B $B_2^{f_2}$ B

des carrés cartésiens. Considérons le carré

$X_1\times_XX_2^g$ X

$$
p'p \tag{17}
$$

$B_1\times_BB_2^f$ B où $f$ (resp. $g$) est l’application qui définit la structure de B-espace (resp. de X-espace) du produit fibré $B_1\times_BB_2$ (resp. du produit fibré $X_1\times_XX_2$) et où $p'$ est l’application déduite de $p_1\times p_2$ par passage aux sous-ensembles. Il est cartésien (I, p. 13, cor. 2 de la prop. 5).

Considérons alors les deux carrés commutatifs suivants :

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & X_1 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_1} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & B_1 \end{array} \tag{18}$$

et

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & X_2 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_2} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & B_2 \end{array}. \tag{19}$$

Le carré (17) est composé des carrés (15) et (18), ainsi que des carrés (16) et (19). D’après la prop. 7, les carrés (18) et (19) sont cartésiens.

### 10. Applications strictes

#### Proposition 8 {#ta-i-s1-prop-8 .statement tag=01M1}

Soit

$$\begin{array}{ccc} X' & \overset{f'}{\longrightarrow} & X \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B' & \overset{f}{\longrightarrow} & B \end{array}$$

un carré cartésien. Si l’application $p$ est ouverte ( resp. est propre, resp. possède au voisinage de tout point une section continue), il en est de même de $p'$.

D’après la remarque 2, I, p. 16, il suffit de démontrer la proposition pour les carrés cartésiens du type suivant :

$$\begin{array}{ccccccc} \overset{-1}{p}(A) & \overset{j}{\longrightarrow} & X & & X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p_A}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{et} & {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ A & \overset{i}{\longrightarrow} & B & & B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array},$$

où F est un espace topologique, A un sous-espace de B et $i,j$ les injections canoniques. Si l’application $p$ est ouverte, les applications $p_A$ et $p\times$ Id$_F$ sont ouvertes (TG, I, p. 30, prop. 2 et TG, I, p. 34, prop. 8). Si l’application $p$ est propre, les applications $p_A$ et $p\times$ Id$_F$ sont propres (TG, I, p. 72, prop. 3 et TG, I, p. 72, déf. 1). Si U est un ouvert de B et $s: U\rightarrow X$ une section continue de $p$ sur U, l’application $s|(A\cap U)$ est une section continue de $p_A$ sur $A\cap U$ et l’application $s\times$ Id$_F$ est une section continue de $p\times$ Id$_F$ sur $U\times F$.

#### Remarque 1 {#ta-i-s1-n10-rem-1 .statement tag=01M2}

Avec les notations de la prop. 8, si $p$ est une application fermée, il n’en est pas nécessairement de même de $p'($cf. TG, I, p. 72, exemple). Cependant, si l’application $p$ est fermée et si A est un sous-espace de B, l’application $p_A:\overset{-1}{p}(A)\rightarrow A$ est fermée (TG, I, p. 30, prop. 2, a)).

#### Définition 5 {#ta-i-s1-def-5 .statement tag=01M3}

Soient X et Y des espaces topologiques et $f: X\rightarrow Y$ une application. Soient R la relation d’équivalence associée à $f$ et

$$
X\rightarrow X/R-\overset{g}{\rightarrow}f(X)\rightarrow Y
$$

la décomposition canonique de $f$ (E, II, p. 44). On dit que l’application $f$ est stricte si $g$ est un homéomorphisme, lorsqu’on munit $X/R$ de la topologie quotient et $f(X)$ de la topologie induite par celle de Y.

Une application stricte est continue.

Rappelons (TG, I, p. 22, prop. 8) que pour qu’une application $f$ soit stricte, il faut et il suffit que $f$ soit continue et que pour toute partie A de X ouverte (resp. fermée) et saturée, l’ensemble $f(A)$ soit ouvert (resp. fermé) dans $f(X)$.

#### Exemple 1 {#ta-i-s1-n10-exa-1 .statement tag=01M4}

La composée de deux applications strictes n’est pas nécessairement stricte. De fait, toute application continue $f: X\rightarrow Y$ est composée de l’application pr$_2: X\times Y\rightarrow$ Y et de l’application $x\mapsto (x, f(x))$ de X dans $X\times Y$ qui sont toutes deux strictes (TG, I, p. 26, prop. 5 et TG, I, p. 25, cor. 2). En revanche, l’application composée de deux applications strictes et injectives (resp. surjectives) est une application stricte.

#### Exemple 2 {#ta-i-s1-n10-exa-2 .statement tag=01M5}

Une application continue qui est ouverte, ou fermée ou qui possède une section continue, est stricte. Cela résulte de la prop. 3 de TG, I, p. 32 et de la prop. 9 de TG, I, p. 22.

#### Exemple 3 {#ta-i-s1-n10-exa-3 .statement tag=01M6}

Pour qu’un homomorphisme continu d’un groupe topologique dans un autre soit un morphisme strict (TG, III, p. 16, déf. 1), il faut et il suffit que ce soit une application stricte au sens de la définition 5.

#### Proposition 9 {#ta-i-s1-prop-9 .statement tag=01M7}

Soient X, Y et Z des espaces topologiques. Soient $f: X\rightarrow Y$ une application continue surjective et $g: Y\rightarrow Z$ une application.

a) Si $f$ est stricte et si $g\circ f$ est continue, l’application $g$ est continue.

b) Si $g$ est continue et si $g\circ f$ est stricte, l’application $g$ est stricte.

c) Si $f$ et $g\circ f$ sont strictes, $g$ est stricte.

Démontrons l’assertion a). Notons R la relation associée à $f$ dans X ; par hypothèse, l’application de $X/R$ sur Y déduite de $f$ par passage au quotient est un homéomorphisme. La première assertion résulte alors de la prop. 6 de I, p. 21.

Démontrons b). Soit B une partie fermée saturée de Y pour la relation définie par $g$ et soit $A =\overset{-1}{f}(B)$. Comme $f$ est continue, A est fermée dans X, et A est saturée pour la relation d’équivalence définie par $g\circ f$. Puisque $g\circ f$ est stricte et $f$ est surjective, $g(B) =g\circ f(A)$ est alors fermée dans Z. L’application continue $g$ est donc stricte.

L’assertion c) résulte immédiatement des assertions a) et b).

#### Proposition 10 {#ta-i-s1-prop-10 .statement tag=01M8}

Soit X un espace topologique et soit R une relation d’équivalence dans X. Soit Y un espace topologique localement compact. Soit S la relation d’équivalence dans $X\times Y$ produit de la relation d’équivalence R dans X et de la relation d’égalité dans Y. La bijection canonique $(X\times Y)/S\rightarrow (X/R)\times Y$ est un homéomorphisme.

Rappelons que si U et V sont des espaces topologiques, $\mathscr{C}_c(U; V)$ désigne l’ensemble des applications continues de U dans V, muni de la topologie de la convergence compacte (TG, X, p. 26, déf. 1).

Notons $p: X\rightarrow X/R$ et $q: X\times Y\rightarrow (X\times Y)/S$ les surjections canoniques. Notons $g: (X\times Y)/S\rightarrow (X/R)\times Y$ la bijection canonique. Elle est continue ; notons $h$ sa réciproque et démontrons qu’elle est continue.

L’application $i: X\rightarrow \mathscr{C}_c(Y; X\times Y)$ telle que, pour tout $x\in$ X, $i(x)$ est l’application définie par $y\mapsto (x, y)$, est continue (TG, X, p. 28, th. 3). L’application $\widetilde{q}:\mathscr{C}_c(Y; X\times Y)\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ qui, à une application continue $\varphi$, associe l’application $q\circ \varphi$, est continue (TG, X, p. 29, prop. 9). Par conséquent, l’application $\widetilde{q}\circ i: X\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ est continue. Elle est compatible à la relation d’équivalence R ; l’unique application $j: X/R\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ telle que $j\circ p=\widetilde{q}\circ i$ est donc continue. On a $h(\xi , y) =j(\xi )(y)$ pour tout couple $(\xi , y)\in (X/R)\times Y$. Comme Y est localement compact, il résulte alors de TG, X, p. 28, th. 3, que l’application $h$ est continue.

La conclusion de la proposition 10 n’est plus nécessairement vérifiée si Y n’est pas localement compact (TG, I, p. 96, exerc. 6).

#### Corollaire {#ta-i-s1-n10-cor-1 .statement tag=01M9}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une application continue. Soit T un espace topologique localement compact. Si l’application $f$ est stricte, il en est de même de l’application $f\times$ Id$_T$ de $X\times T$ dans $Y\times T$.

### 11. Applications universellement strictes

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien, où l’application $p$ est stricte. L’application $p'$ n’est pas nécessairement stricte (cf. TG, I, p. 96, exerc. 6). Cependant, si A est un sous-espace ouvert ou fermé de B, l’application $p_A:\overset{-1}{p}(A)\rightarrow A$ est stricte (TG, I, p. 23, cor. 1).

#### Définition 6 {#ta-i-s1-def-6 .statement tag=01MA}

Soit $p: X\rightarrow B$ une application continue. On dit que l’application $p$ est universellement stricte si pour tout carré cartésien

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

l’application $p'$ est stricte.

Une application universellement stricte est stricte. Avec les notations de la définition 6, si l’application $p$ est universellement stricte, il en est de même de $p'$. Cela résulte immédiatement de la déf. 6 et de la prop. 7 de I, p. 15.

#### Corollaire {#ta-i-s1-n11-cor-1 .statement tag=01MB}

Une application continue qui est ouverte, ou propre, ou qui admet au voisinage de tout point une section continue, est universellement stricte (prop. 8 et exemple 2).

#### Exemple {#ta-i-s1-n11-exa-1 .statement tag=01MC}

Soient B un espace topologique et $(A_i)_{i\in I}$ un recouvrement de B; on note A l’espace somme de la famille $(A_i)_{i\in I}$, et $p: A\rightarrow B$ l’application canonique. L’application $p$ est universellement stricte sous chacune des deux hypothèses suivantes :

(i) Pour tout point $b\in B$, il existe $i\in I$ tel que $b$ soit un point intérieur de $A_i$;

(ii) La famille $(A_i)$ est localement finie et les $A_i$ sont des parties fermées de B.

Sous l’hypothèse (i), l’application $p$ possède au voisinage de tout point une section continue. Sous l’hypothèse (ii), l’application $p$ est propre par définition de l’espace somme (resp. d’après TG, I, p. 6, prop. 4 et TG, I, p. 75, th. 1). Elle est donc universellement stricte.

#### Remarque {#ta-i-s1-n11-rem-1 .statement tag=01MD}

Une application fermée n’est pas nécessairement universellement stricte (cf. TG, I, p. 96, exerc. 6).

#### Proposition 11 {#ta-i-s1-prop-11 .statement tag=01ME}

Soit

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

un carré cartésien.

a) Supposons l’application $f$ stricte et surjective. Alors, si l’application $p'$ est ouverte ( resp. fermée, resp. propre), il en est de même de $p$.

b) Supposons que l’application $f$ soit fermée et surjective. Alors, si l’application $p'$ est stricte, il en est de même de $p$.

c) Supposons que l’application $f$ soit universellement stricte et surjective. Alors, si l’application $p'$ est stricte, il en est de même de $p$.

Remarquons au préalable que pour toute partie A de X, on a

$$
p'((\overset{-1}{f}')(A)) =\overset{-1}{f}(p(A)) \tag{20}
$$

En effet, si $x'\in (\overset{-1}{f}')(A)$, alors $f(p'(x')) =p\circ f'(x')\in p(A)$. Réciproquement, si $b'\in \overset{-1}{f}(p(A))$, soit $x\in A$ tel que $f(b') =p(x)$. Par définition d’un carré cartésien, il existe un unique $x'\in X'$ tel que $f'(x') =x$ et $p'(x') =b'$, si bien que $b'\in p'((\overset{-1}{f}')(A))$.

Démontrons a). Supposons d’abord que $p'$ soit une application ouverte (resp. fermée) et soit A un ensemble ouvert (resp. fermé) dans X. L’ensemble $(\overset{-1}{f}')(A)$ est ouvert (resp. fermé) dans $X'$. Par suite, l’ensemble $p'((\overset{-1}{f}')(A))$ est ouvert (resp. fermé) dans $B'$. D’après la relation (20), il est aussi saturé pour la relation d’équivalence définie par $f$. Puisque l’application $f$ est supposée surjective, on a alors $p(A) =$

$f(p'((\overset{-1}{f}')(A)))$, et comme elle est stricte, l’ensemble $p(A)$ est ouvert (resp. fermé) dans B. L’application $p$ est donc ouverte (resp. fermée).

Pour qu’une application continue soit propre, il faut et il suffit qu’elle soit fermée et que ses fibres soient quasi-compactes (TG, I, p. 75, th. 1). Si l’application $p'$ est propre, l’application $p$ est fermée d’après ce qui précède. Étudions ses fibres : si $b\in B$, soit $b'\in B'$ tel que $f(b') =b$. D’après le corollaire de I, p. 10, l’application $f'$ induit un homéomorphisme $X'_{b'}\rightarrow X_b$. Puisque $p'$ est propre, $X'_{b'}$ est quasi-compacte, donc $X_b$ l’est aussi. L’application $p$ est donc propre.

Démontrons b) et c). Posons Y = $p(X)$ et $Y'=p'(X')$ ; la relation (20) appliquée à X entraîne que $Y'=\overset{-1}{f}(Y)$. Notons $g$ l’application de $Y'$ dans Y induite par $f$. Dans le cas b), l’application $g$ est stricte d’après la remarque 1, I, p. 18. Dans le cas c), elle est stricte en vertu de la définition 6 puisque le carré

$Y'$ Y

$B'$ B

est cartésien.

Désignons par $q$ et $q'$ les applications de X dans Y et de $X'$ dans $Y'$ induites par $p$ et $p'$, de sorte que le carré

${X'}^{f'}$ X

$q'q$

${Y'}^g$ Y

est cartésien. Les applications $g$ et $q'$ étant toutes deux strictes et surjectives, leur composée $g\circ q'$ est stricte. Ainsi, $q\circ f'$ est stricte et $p\circ f'$ est elle-même stricte. Puisque $f$ est surjective, $f'$ l’est aussi et $p$ est stricte d’après la prop. 9, b) de I, p. 18.

#### Corollaire 1 {#ta-i-s1-prop-11-cor-1 .statement tag=01MF}

Supposons que l’application $f$ soit universellement stricte et surjective et que l’application $p'$ soit universellement stricte. Alors, l’application $p$ est universellement stricte.

Soit

Y $^{g'}$ X

$qp$

C $^g$ B

un carré cartésien ; il s’agit de démontrer que l’application $q$ est stricte. D’après la remarque 3 de I, p. 16, les carrés

$$
X'\times_XY^{pr_1}X'
$$

$rp'$

$$
B'\times_BC^{pr_1}B'
$$

et

$X'\times_XY^{pr_2}$ Y

$$
rq \tag{21}
$$

$B'\times_BC^{pr_2}$ C

sont cartésiens, où $r: X'\times_XY\rightarrow B'\times_BC$ désigne l’application induite par $(p', q)$. Comme l’application $f$ est universellement stricte et surjective, il en est de même de l’application pr$_2: B'\times_BC\rightarrow C$ (I, p. 20, déf. 6 et I, p. 10, cor. de la prop. 4). D’autre part, l’application $r$ est stricte, puisque $p'$ est supposée universellement stricte. D’après la prop. 11, c) appliquée au carré cartésien (21), l’application $q$ est stricte.

#### Corollaire 2 {#ta-i-s1-prop-11-cor-2 .statement tag=01MG}

Soient B et X des espaces topologiques et soit $p: X\rightarrow B$ une application continue. Soit $(A_i)_{i\in I}$ une famille de parties de B qui est un recouvrement ouvert de B, ou bien un recouvrement fermé localement fini de B. Si pour tout $i\in$ I, l’application $p_{A_i}:\overset{-1}{p}(A_i)\rightarrow A_i$ est stricte ( resp. universellement stricte), l’application $p$ est stricte ( resp. universellement stricte).

Pour tout $i\in I$, posons $Y_i=\overset{-1}{p}(A_i)$ et $p_i=p_{A_i}$. Soient A l’espace somme de la famille $(A_i)_{i\in I}$, Y l’espace somme de la famille $(Y_i)_{i\in I}$; notons $f: A\rightarrow B$ (resp. $g: Y\rightarrow X,q: Y\rightarrow A$) l’application déduite de la famille des injections canoniques $A_i\rightarrow B$ (resp. des injections canoniques $Y_i\rightarrow X$, des applications $p_i$). Le carré

Y $^g$ X

$qp$

A $^f$ B

est un carré cartésien (exemples, I, p. 10 et p. 14). D’après le corollaire, I, p. 20, l’application $f$ est universellement stricte. D’après la proposition 11, il suffit donc de démontrer que l’application $q$ est stricte (resp. universellement stricte) si les applications $p_i$, pour $i\in I$, le sont. On est ainsi ramené à démontrer le corollaire lorsque les ensembles $A_i$, $i\in I$, constituent une partition de l’espace B en parties ouvertes et fermées, ce que nous supposerons désormais.

Supposons que chacune des applications $p_i,i\in I$, soit stricte. Si U est une partie ouverte de X et saturée pour la relation d’équivalence définie par $p$, l’ensemble $p_i(X_i\cap U)$ est ouvert dans $A_i$ et $p(U) =$ $\bigcup_{i\in I}p_i(X_i\cap U)$ est ouvert dans B. L’application $p$ est donc stricte.

Supposons maintenant que chacune des applications $p_i,i\in I$, soit universellement stricte et montrons que l’application $p$ est universellement stricte. Soient C un espace topologique et $h: C\rightarrow B$ une application continue. Il s’agit de montrer que l’application pr$_1: X\times_BC\rightarrow C$ est stricte. L’espace C s’identifie à l’espace somme de la famille des $C_i=\overset{-1}{h}(A_i)$ et l’espace $X\times_BC$ s’identifie à l’espace somme de la famille des $X\times_BC_i= X_i\times_{A_i}C_i$. Comme $p_i$ est universellement stricte, l’application pr$_1: X_i\times_{A_i}C_i\rightarrow C_i$ est stricte. D’après ce qui précède, l’application pr$_1: X\times_BC\rightarrow C$ est stricte. Cela prouve que l’application $p$ est universellement stricte.

## EXERCICES {#ta-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
