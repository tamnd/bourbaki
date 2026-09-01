---
book: top
book_title: General Topology
chapter: VIII
chapter_title: NOMBRES COMPLEXES
section: 4
section_title: Espaces numériques et espaces projectifs complexes
lang: fr
source: top-v-x-fr
pdf_pages: 0104-0110, 0113-0115
extraction: ocr
subsections:
    - "no": 1
      title: L’espace vectoriel $\mathbf{C}^n$
      page: 18
      pdf_page: 104
    - "no": 2
      title: Topologie des espaces vectoriels et des algèbres sur le corps $\mathbf{C}$
      page: 19
      pdf_page: 105
    - "no": 3
      title: Espaces projectifs complexes
      page: 20
      pdf_page: 106
    - "no": 4
      title: Espaces de variétés linéaires projectives complexes
      page: 21
      pdf_page: 107
    - "no": 5
      title: Continuité des racines d’un polynôme
      page: 22
      pdf_page: 108
statements: 8
exercises: 8
content_sha256: 6dbd9a819bd23bef9ea6b374eb5491c118d9321564f8a7ae710591b73b00c279
---

## § 4. ESPACES NUMÉRIQUES ET ESPACES PROJECTIFS COMPLEXES

### 1. L’espace vectoriel $\mathbf{C}^n$

Le groupe topologique produit $\mathbf{C}^n$ de $n$ groupes égaux au groupe topologique $\mathbf{C}$ peut être identifié au groupe topologique $\mathbf{R}^{2n}$ par la bijection qui associe à l’élément $\mathbf{z} = (z_1, \ldots, z_n)$ de $\mathbf{C}^n$ l’élément $(\mathcal{R}(z_1), \mathcal{I}(z_1), \ldots, \mathcal{R}(z_n), \mathcal{I}(z_n))$ de $\mathbf{R}^{2n}$.

Mais, comme $\mathbf{C}$ est un corps, on peut définir sur $\mathbf{C}^n$ une structure d’espace vectoriel de dimension $n$ sur $\mathbf{C}$, le produit $az$ d’un nombre complexe $a$ et d’un point $\mathbf{z} = (z_i)$ de $\mathbf{C}^n$ étant le point $(az_i)$; il faut avoir soin de ne pas confondre cette structure et celle d’espace vectoriel de dimension $2n$ par rapport à $\mathbf{R}$, définie sur $\mathbf{R}^{2n}$ (VI, p. 2); on réservera la notation $\mathbf{C}^n$ à l’espace topologique produit de $n$ espaces identiques à $\mathbf{C}$, muni en outre de la structure d’espace vectoriel par rapport à $\mathbf{C}$ qui vient d’être définie; on le désignera sous le nom d’espace numérique complexe à $n$ dimensions. On notera que l’application $(t, \mathbf{z}) \mapsto t\mathbf{z}$ est continue dans $\mathbf{C} \times \mathbf{C}^n$.

Une application linéaire affine de $\mathbf{C}^n$ dans $\mathbf{C}^m$ est aussi une application linéaire affine de $\mathbf{R}^{2n}$ dans $\mathbf{R}^{2m}$, mais la réciproque n’est pas vraie.

Par exemple, l’application $z \mapsto \bar{z}$ est une application linéaire de l’espace vectoriel $\mathbf{R}^2$ sur lui-même, mais non une application linéaire de l’espace vectoriel $\mathbf{C}$ sur lui-même.

Toute application linéaire affine de $\mathbf{C}^n$ dans $\mathbf{C}^m$ est donc uniformément continue ; en particulier, toute application linéaire affine de $\mathbf{C}^n$ sur lui-même est un homéomorphisme.

Toute variété linéaire affine à $p$ dimensions ($p \leq n$) de l’espace vectoriel $\mathbf{C}^n$ est aussi une variété linéaire affine à $2p$ dimensions de l’espace vectoriel $\mathbf{R}^{2n}$; ici encore, la réciproque est inexacte. Pour éviter toute confusion, on désigne les variétés linéaires (affines) à $p$ dimensions de $\mathbf{C}^n$ sous le nom de variétés linéaires complexes à $p$ dimensions (les variétés linéaires de $\mathbf{R}^{2n}$ étant appelées variétés linéaires réelles quand on veut se garder de toute méprise). En particulier, on appellera droites complexes (resp. plans complexes) les variétés linéaires complexes à 1 dimension (resp. à 2 dimensions) de $\mathbf{C}^n$, hyperplans complexes les variétés linéaires complexes à $n - 1$ dimensions.

Il est souvent commode de considérer l’espace numérique $\mathbf{R}^n$ comme plongé dans l’espace numérique complexe $\mathbf{C}^n$, en l’identifiant à la partie de $\mathbf{C}^n$ définie par les relations $\mathcal{J}(z_k) = 0$ ($k = 1, 2, \ldots, n$), dont la structure de groupe topologique (induite par celle de $\mathbf{C}^n$) est isomorphe à celle de $\mathbf{R}^n$.

On notera que $\mathbf{R}^n$, ainsi plongé dans $\mathbf{C}^n$, n’est pas une variété linéaire complexe de $\mathbf{C}^n$.

Un système de $p$ vecteurs de $\mathbf{R}^n$, libre par rapport au corps $\mathbf{R}$, est encore libre par rapport au corps $\mathbf{C}$; toute variété linéaire réelle $V$ à $p$ dimensions de $\mathbf{R}^n$ engendre, dans $\mathbf{C}^n$, une variété linéaire complexe à $p$ dimensions $V'$, dont elle est la trace sur $\mathbf{R}^n$ (A, II, p. 120); si $V$ est définie par un système de $n - p$ équations linéaires $f_k(\mathbf{x}) = a_k$, où les $f_k$ sont des formes linéaires sur $\mathbf{R}^n$ (à coefficients réels, et linéairement indépendantes) et les $a_k$ des nombres réels, les mêmes équations, mais où l’on donne aux coordonnées de $\mathbf{x}$ des valeurs complexes, définissent $V'$.

Inversement, lorsqu’une variété linéaire complexe à $p$ dimensions a une intersection non vide avec $\mathbf{R}^n$, cette intersection est une variété linéaire réelle; mais la dimension de cette variété peut être $< p$.

### 2. Topologie des espaces vectoriels et des algèbres sur le corps $\mathbf{C}$

Toutes les définitions et tous les résultats des nos 5 et 6 du chap. VI, § 1, relatifs aux topologies des espaces vectoriels et des algèbres sur le corps $\mathbf{R}$, et en particulier des espaces et algèbres de matrices à éléments dans $\mathbf{R}$, sont valables sans aucune modification quand on remplace partout $\mathbf{R}$ par $\mathbf{C}$.

### 3. Espaces projectifs complexes

Avec les notations rappelées dans VI, p. 13, on pose la définition suivante, analogue à la définition des espaces projectifs réels:

#### Définition 1 {#top-viii-s4-def-1 .statement}

On appelle espace projectif complexe à n dimensions l’espace projectif $P_n(\mathbf{C})$ muni de la topologie quotient de celle de $\mathbf{C}_{n+1}^*$ par la relation d’équivalence $\Delta_n(\mathbf{C})$.

L’espace projectif $P_1(\mathbf{C})$ s’appelle droite projective complexe, l’espace projectif $P_2(\mathbf{C})$ plan projectif complexe.

Dans toute question où interviennent les espaces projectifs complexes, à l’exclusion des espaces projectifs réels, on écrit encore $P_n$ au lieu de $P_n(\mathbf{C})$.

La plupart des raisonnements relatifs aux espaces projectifs réels s’étendent avec de très légères modifications aux espaces projectifs complexes.

En premier lieu, on voit que l’espace topologique $P_n(\mathbf{C})$ est séparé, par le raisonnement de la prop. 1 de VI, p. 13, qui se transpose tel quel en remplaçant simplement $\mathbf{R}$ par $\mathbf{C}$. De même, le raisonnement de la prop. 2 de VI, p. 13, montre que $P_n(\mathbf{C})$ est compact et connexe, et homéomorphe à l’espace quotient de la sphère $S_{2n+1}$ (considérée comme plongée dans l’espace $\mathbf{C}_{n+1}^*$, identifié à $\mathbf{R}_{2n+2}^*$) par la relation d’équivalence induite sur cette sphère par $\Delta_n(\mathbf{C})$; on notera seulement que, si $n \geqslant 0$, les classes d’équivalence pour cette relation sont ici des ensembles homéomorphes au cercle $S_1$.

C’est pour cette raison que la prop. 3 de VI, p. 14, n’a pas d’analogue pour les espaces projectifs complexes.

On montre ensuite, comme dans VI, p. 15, que toute variété linéaire projective à $p$ dimensions de l’espace $P_n(\mathbf{C})$ est un ensemble fermé, homéomorphe à $P_p(\mathbf{C})$, et dont le complémentaire est partout dense si $p < n$. Le raisonnement de la prop. 5 de VI, p. 15, se transpose sans aucune modification par simple substitution de $\mathbf{C}$ à $\mathbf{R}$, et prouve que, dans $P_n(\mathbf{C})$ (pour $n \geqslant 0$), le complémentaire d’un hyperplan projectif est homéomorphe à $\mathbf{C}^n$, et par suite que tout point a un voisinage homéomorphe à $\mathbf{C}^n$. Cela permet de plonger l’espace numérique complexe $\mathbf{C}^n$ dans l’espace projectif complexe $P_n(\mathbf{C})$, en l’identifiant avec le complémentaire d’un hyperplan projectif, dit « hyperplan à l’infini » (le plus souvent, l’hyperplan d’équation $x_0 = 0$). Dans le cas particulier où $n = 1$, l’hyperplan à l’infini est un point; le th. d’Alexandroff montre alors que $P_1(\mathbf{C})$ est homéomorphe à l’espace $\tilde{\mathbf{C}}$ obtenu en rendant compact l’espace localement compact $\mathbf{C}$ par adjonction d’un « point à l’infini » noté $\infty$; le cor. 1 de VI, p. 11 prouve alors que la droite projective complexe $P_1(\mathbf{C})$ est homéomorphe à la sphère $S_2$.

Nous laissons au lecteur le soin d’énoncer les résultats analogues à ceux de VI, § 3, n° 4, pour les fonctions prenant leurs valeurs dans $\mathbf{C}$.

Considérons l’espace $\mathbf{R}^{n+1}$ comme plongé dans $\mathbf{C}^{n+1}$ (VIII, p. 19). Soit $f$ l’application canonique de $\mathbf{C}_{n+1}^*$ sur l’espace quotient $P_n(\mathbf{C})$. Le sous-espace $f(\mathbf{R}_{n+1}^*)$ se compose des points de $P_n(\mathbf{C})$ qui admettent au moins un système de coordonnées homogènes réelles; montrons que $f(\mathbf{R}_{n+1}^*)$ est homéomorphe à l’espace projectif réel $\mathbf{P}_n(\mathbf{R})$, ce qui permet, en l’identifiant à ce dernier, de considérer l’espace $\mathbf{P}_n(\mathbf{R})$ comme plongé dans $\mathbf{P}_n(\mathbf{C})$. Or, la relation induite par $\Delta_n(\mathbf{C})$ sur $\mathbf{R}_{n+1}^*$ n’est autre que $\Delta_n(\mathbf{R})$; l’application canonique $\varphi$ de $\mathbf{R}_{n+1}^*/\Delta_n(\mathbf{R}) = \mathbf{P}_n(\mathbf{R})$ sur $f(\mathbf{R}_{n+1}^*)$ est continue (I, p. 23, prop. 10); comme $\mathbf{P}_n(\mathbf{R})$ est compact, $\varphi$ est un homéomorphisme (I, p. 63, cor. 2).

On peut aussi démontrer que $\varphi$ est bicontinue sans utiliser la compacité de $\mathbf{P}_n(\mathbf{R})$, en se servant du critère de la prop. 10 de I, p. 23 (voir VIII, p. 28, exerc. 3).

Comme tout sous-espace vectoriel à $p + 1$ dimensions de $\mathbf{R}^{n+1}$ engendre, dans $\mathbf{C}^{n+1}$, un sous-espace vectoriel complexe à $p + 1$ dimensions, on voit que toute variété linéaire projective $V$ à dimensions de $\mathbf{P}_n(\mathbf{R})$ (dite variété linéaire projective réelle) engendre dans $\mathbf{P}_n(\mathbf{C})$ une variété linéaire projective $V'$ à $p$ dimensions (dite variété linéaire projective complexe), dont elle est la trace sur $\mathbf{P}_n(\mathbf{R})$; en outre, tout système d’équations (homogènes) de $V$ est un système d’équations (homogènes) de $V'$, en donnant aux variables des valeurs complexes.

### 4. Espaces de variétés linéaires projectives complexes

Avec les notations rappelées dans VI, p. 17, on définit de même les espaces de variétés linéaires projectives d’un espace projectif complexe:

#### Définition 2 {#top-viii-s4-def-2 .statement}

On appelle espace des variétés linéaires projectives à $p \geqslant 0$ dimensions de l’espace projectif $\mathbf{P}_n(\mathbf{C})$, l’espace $\mathbf{P}_{n,p}(\mathbf{C})$ quotient de l’espace topologique $\mathbf{L}_{n+1,p+1}(\mathbf{C})$ par la relation d’équivalence $\Delta_{n,p}(\mathbf{C})$.

La démonstration de la prop. 6 de VI, p. 18 se transpose sans modification pour l’espace $\mathbf{P}_{n,p}(\mathbf{C})$ et montre que cet espace est connexe, localement connexe, et que chacun de ses points possède un voisinage homéomorphe à $\mathbf{C}^{(p+1)(n-p)}$. On démontre ensuite que $\mathbf{P}_{n,p}(\mathbf{C})$ est compact, en remplaçant, dans la démonstration de la prop. 7 de VI, p. 19, le sous-espace $V_{n+1,p+1}$ par le sous-espace $W_{n+1,p+1}$ de $\mathbf{L}_{n+1,p+1}(\mathbf{C})$ formé des systèmes de $p + 1$ vecteurs formant une base hermitienne orthonormale du sous-espace vectoriel qu’elles engendrent (A, IX, § 6, n° 1): il revient au même de dire que $W_{n+1,p+1}$ se compose des matrices $X = (x_{ij})$ satisfaisant aux conditions

$$
\sum_{j=0}^n x_{ij} \overline{x}_{ij} = 1 \quad \text{pour } 1 \leq i \leq p + 1
$$
$$
\sum_{j=0}^n x_{ij} \overline{x}_{kj} = 0 \quad \text{pour } i \neq k.
$$

Enfin, le raisonnement de la prop. 8 de VI, p. 20 est aussi applicable sans modification, et on voit donc que la grassmannienne $G_{n+1,p+1}(\mathbf{C})$ est homomorphe à $\mathbf{P}_{n,p}(\mathbf{C})$.

#### Remarque {#top-viii-s4-n4-rem-1 .statement}

La plupart des propriétés communes aux espaces numériques (ou projectifs) réels et complexes sont encore exactes pour les espaces numériques (resp. projectifs) définis de manière analogue à partir du corps des quaternions $\mathbf{H}$; elles sont même susceptibles de s’étendre à beaucoup d’autres corps topologiques (cf. VIII, p. 27, exerc. 2 et VIII, p. 28, exerc. 6).

### 5. Continuité des racines d’un polynôme

Soient $K$ un corps commutatif et $n$ un entier $\geqslant 0$; notons $K[X]_n$ l’espace vectoriel des polynômes à coefficients dans $K$ et de degré $\leqslant n$. Soit $q$ l’application canonique de $K[X]_n - \{0\}$ sur l’espace projectif $P(K[X]_n)$ déduit de $K[X]_n$; la restriction de $q$ à l’ensemble des polynômes unitaires appartenant à $K[X]_n$ est bijective.

D’autre part, le groupe symétrique $S_n$ opère sur l’ensemble $P_1(K)^n$, produit de $n$ espaces égaux à $P_1(K)$, par permutation des facteurs. Notons $\Sigma_n(K)$ l’ensemble $P_1(K)^n / S_n$ des orbites de $S_n$ dans $P_1(K)^n$ (« puissance symétrique $n$-ième » de $P_1(K)$).

L’application de $(K^2 - \{0\})^n$ dans $K[X]_n - \{0\}$, qui associe à l’élément $((a_1, b_1), \ldots, (a_n, b_n))$ le polynôme $(b_1 X - a_1) \ldots (b_n X - a_n)$, définit par passage aux quotients une application de $P_1(K)^n$ dans $P(K[X]_n)$; cette application est constante sur chaque orbite de $S_n$ dans $P_1(K)^n$, donc définit par passage au quotient une application $f$ de $\Sigma_n(K)$ dans $P(K[X]_n)$. Soit $\xi \in \Sigma_n(K)$; il existe une suite $a_1, \ldots, a_p$, avec $p \leqslant n$, d’éléments de $K$ telle que $\xi$ soit l’image canonique de l’élément $(a_1, \ldots, a_p, \infty, \ldots, \infty)$ de $P_1(K)^n$; on a alors $f(\xi) = q(P)$, où $P$ est le polynôme unitaire $(X - a_1) \ldots (X - a_p)$. Il en résulte que l’application $f$ est injective, et qu’elle est bijective lorsque $K$ est algébriquement clos.

Supposons maintenant $K = \mathbf{C}$. Munissons $P_1(\mathbf{C})^n$ et $P(\mathbf{C}[X]_n)$ des topologies définies ci-dessus (VIII, p. 20 et VI, p. 14) et $\Sigma_n(\mathbf{C})$ de la topologie quotient de celle de $P_1(\mathbf{C})^n$.

#### Proposition 1 {#top-viii-s4-prop-1 .statement}

L’application $f$ de $\Sigma_n(\mathbf{C})$ dans $P(\mathbf{C}[X]_n)$ définie ci-dessus est un homéomorphisme.

L’application $f$ est bijective car $\mathbf{C}$ est algébriquement clos (VIII, p. 1, th. 1). Il est clair que l’application $((a_1, b_1), \ldots, (a_n, b_n)) \mapsto q((b_1 X - a_1) \ldots (b_n X - a_n))$ de $(\mathbf{C}^2 - \{0\})^n$ dans $P(\mathbf{C}[X]_n)$ est continue; d’après I, p. 34, cor. de la prop. 8 et I, p. 21, prop. 6, l’application $f$ est continue. Comme $\Sigma_n(\mathbf{C})$ est quasi-compact (I, p. 62, th. 2), et $P(\mathbf{C}[X]_n)$ séparé, la bijection $f$ est un homéomorphisme (I, p. 63, cor. 2 au th. 2).

#### Corollaire {#top-viii-s4-n5-cor-1 .statement}

L’espace projectif complexe à $n$ dimensions est homéomorphe à la puissance symétrique $n$-ième de la droite projective complexe.

Soient $P \in \mathbf{C}[X]_n$ un polynôme non nul et $a \in \mathbf{C}$; notons $v_a(P)$ la multiplicité de $a$ comme racine de $P$, c’est-à-dire le plus grand entier positif $m$ tel que $(X - a)^m$ divise P. On note $v_\infty(P)$ l’entier positif $n - \deg(P)$, et on dit que le point $\infty$ de $\mathbf{P}_1(\mathbf{C})$ est racine de P si $v_\infty(P) > 0$. On a (A, IV, § 2, n° 4, prop. 7 et A, V, § 4, n° 1, prop. 1)

$$
\sum_{a \in \mathbf{P}_1(\mathbf{C})} v_a(P) = n.
$$

Pour toute partie A de $\mathbf{P}_1(\mathbf{C})$, on note $v_A(P)$ le nombre des racines de P dans A comptées avec leur multiplicité, c’est-à-dire l’entier $\sum_{a \in A} v_a(P)$.

#### Proposition 2 {#top-viii-s4-prop-2 .statement}

*Soit A une partie ouverte (resp. fermée) de $\mathbf{P}_1(\mathbf{C})$. La fonction numérique $P \mapsto v_A(P)$ est semi-continue inférieurement (resp. supérieurement) en tout point de $\mathbf{C}[X]_n - \{0\}$* (IV, p. 28).

Soient P un point de $\mathbf{C}[X]_n - \{0\}$, A une partie ouverte de $\mathbf{P}_1(\mathbf{C})$; posons $v_A(P) = r$. La partie $A_1 \times \cdots \times A_n$ de $\mathbf{P}_1(\mathbf{C})^n$, où $A_1 = \cdots = A_r = A, A_{r+1} = \cdots = A_n = \mathbf{P}_1(\mathbf{C})$, est ouverte; son image U dans $\Sigma_n(\mathbf{C})$ est ouverte d’après III, p. 9, lemme 2; d’après la prop. 1, la partie $f(U)$ de $\mathbf{P}(\mathbf{C}[X]_n)$ est ouverte. Soit V son image réciproque dans $\mathbf{C}[X]_n - \{0\}$; c’est un ensemble ouvert contenant P; il se compose des polynômes de la forme $\Pi (b_i X - a_i)$, avec $(a_1, b_1), \ldots, (a_r, b_r)$ dans V; on a donc $v_A(Q) \geq r$ pour $Q \in V$. Ceci prouve que $v_A$ est semi-continue inférieurement lorsque A est ouvert; si A est fermé, son complémentaire B est ouvert, et la fonction $v_B = n - v_A$ est semi-continue supérieurement d’après ce qui précède.

#### Corollaire 1 {#top-viii-s4-prop-2-cor-1 .statement}

*Soient U une partie ouverte de $\mathbf{P}_1(\mathbf{C})$, F sa frontière. L’ensemble des polynômes $P \in \mathbf{C}[X]_n - \{0\}$ tels que $v_F(P) = 0$ est ouvert, et la fonction $v_U$ est localement constante dans cet ouvert. Pour tout entier r, l’ensemble des $P \in \mathbf{C}[X]_n - \{0\}$ tels que $v_F(P) = 0$ et $v_U(P) = r$ est ouvert.*

L’ensemble E des points P où la fonction semi-continue supérieurement $v_F$ est < 1 est ouvert (IV, p. 29, prop. 1). Pour P dans E, on a $v_U(P) = v_{\overline{U}}(P)$ où $\overline{U}$ désigne l’adhérence $U \cup F$ de U; la restriction de $v_U$ à E est semi-continue inférieurement et supérieurement, donc continue, c’est-à-dire localement constante. L’ensemble des points de E où elle prend la valeur r est donc ouvert.

#### Corollaire 2 {#top-viii-s4-prop-2-cor-2 .statement}

*Soient U et F comme dans le corollaire 1, et soit V l’ouvert de $\mathbf{C}[X]_n - \{0\}$ formé des polynômes P tels que $v_F(P) = 0, v_U(P) = 1$. À chaque $P \in V$ associons son unique racine dans U. L’application de V dans U ainsi définie est continue.*

Notons $\rho$ l’application précédente. Soit $U'$ une partie ouverte de U, et notons $F'$ sa frontière dans $\mathbf{P}_1(\mathbf{C})$. Comme $U' \cup F' \subset U \cup F$, les éléments P de V tels que $\rho(P) \in U'$, c’est-à-dire que $v_{U'}(P) > 0$, sont aussi les éléments P de V tels que $v_{U'}(P) = 1, v_{F'}(P) = 0$; il résulte alors du cor. 1 que $\rho^{-1}(U')$ est ouvert dans V.

Exercises

## EXERCICES {#top-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
