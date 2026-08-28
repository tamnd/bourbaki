---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 10
section_title: Matrices
lang: fr
source: alg-i-iii-fr
pdf_pages: 0316-0339, 0382-0386
extraction: ocr
subsections:
    - "no": 1
      title: Définition des matrices
      page: 0
      pdf_page: 316
    - "no": 2
      title: Matrices sur un groupe commutatif
      page: 140
      pdf_page: 317
    - "no": 3
      title: Matrices sur un anneau
      page: 142
      pdf_page: 319
    - "no": 4
      title: Matrices et applications linéaires
      page: 143
      pdf_page: 320
    - "no": 5
      title: Produit par blocs
      page: 146
      pdf_page: 323
    - "no": 6
      title: Matrice d’une application semi-linéaire
      page: 148
      pdf_page: 325
    - "no": 7
      title: Matrices carrées
      page: 149
      pdf_page: 326
    - "no": 8
      title: Changements de bases
      page: 152
      pdf_page: 329
    - "no": 9
      title: Matrices équivalentes; matrices semblables
      page: 155
      pdf_page: 332
    - "no": 10
      title: Produit tensoriel de matrices sur un anneau commutatif
      page: 156
      pdf_page: 333
    - "no": 11
      title: Trace d’une matrice
      page: 158
      pdf_page: 335
    - "no": 12
      title: Matrices sur un corps
      page: 158
      pdf_page: 335
    - "no": 13
      title: Équivalence des matrices sur un corps
      page: 160
      pdf_page: 337
statements: 38
exercises: 17
content_sha256: 76410c99c15d209b17769ce2ba680c239cb11617ff2dfbd57b3ff2cf866b1ca4
---

## § 10. MATRICES

### 1. Définition des matrices

#### Définition 1 {#alg-ii-s10-def-1 .statement}

Soient $I, K, H$ trois ensembles; on appelle matrice de type $(I, K)$ à éléments dans $H$ (ou matrice de type $(I, K)$ sur $H$) toute famille $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$ d’éléments de $H$ dont l’ensemble d’indices est le produit $I \times K$. Pour tout $\iota \in I$, la famille $(m_{\iota \kappa})_{\kappa \in K}$ est appelée la ligne d’indice $\iota$ de $M$; pour tout $\kappa \in K$, la famille $(m_{\iota \kappa})_{\iota \in I}$ est appelée la colonne d’indice $\kappa$ de $M$.

Si $I$ (resp. $K$) est fini, on dit que $M$ est une matrice ayant un nombre fini de lignes (resp. de colonnes). L’ensemble des matrices de type $(I, K)$ sur $H$ s’identifie au produit $H^{I \times K}$.

Les dénominations de « ligne » et de « colonne » proviennent de ce que, dans le cas où $I$ et $K$ sont des intervalles $[1, p], [1, q]$ de $\mathbf{N}$, on imagine les éléments de la matrice disposés dans les cases d’un tableau rectangulaire ayant $p$ lignes (rangées horizontales) et $q$ colonnes (rangées verticales):

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdot & \cdot & \cdot & \cdot \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

Lorsque $p$ et $q$ sont des entiers explicités assez petits pour que ce soit praticable, on convient que le tableau précédent est un symbole qui note effectivement la matrice considérée; cette écriture permet de se dispenser de noter les indices, étant entendu que les indices d’un élément sont déterminés par sa place dans le tableau; par exemple, lorsqu’on parlera de la matrice

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

il s’agira de la matrice $(m_{ij})_{1 \leq i \leq 2, 1 \leq j \leq 3}$ telle que

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

Au lieu de matrice de type $([1, p], [1, q])$ on dira aussi matrice de type $(p, q)$, ou matrice à $p$ lignes et $q$ colonnes s’il n’en résulte pas de confusion; on note parfois $\mathbf{M}_{p, q}(H)$ l’ensemble des matrices de type $(p, q)$ sur $H$.

Toute matrice sur $H$ dont l’un des ensembles d’indices $I, K$ est vide est identique à la famille vide d’éléments de $H$; on l’appelle encore la matrice vide. Lorsque $I = \{i_0\}$ (resp. $K = \{k_0\}$) est un ensemble réduit à un seul élément, on dit que $M$ est une matrice ligne (resp. une matrice colonne), et on peut alors supprimer dans la notation l’indice de ligne (resp. de colonne); lorsque $I$ et $K$ sont tous deux des ensembles à un élément, on identifie souvent une matrice de type $(I, K)$ à l’unique élément de cette matrice.

Une sous-famille $M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L}$ d’une matrice $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$ dont l’ensemble d’indices est produit d’une partie $J$ de $I$ et d’une partie $L$ de $K$, est dite sous-matrice de la matrice $M$; on dit qu’elle s’obtient en supprimant dans $M$ les lignes d’indice $\iota \notin J$ et les colonnes d’indice $\kappa \notin L$; inversement, on dit que $M$ s’obtient en bordant $M'$ par les lignes d’indice $\iota \notin J$ et les colonnes d’indice $\kappa \notin L$.

#### Définition 2 {#alg-ii-s10-def-2 .statement}

On appelle transposée d’une matrice $M = (m_{\iota k})_{(\iota, k) \in I \times K}$ et on note ${}^t M$ la matrice $(m'_{k \iota})_{(k, \iota) \in K \times I}$ sur $\mathbf{H}$ donnée par $m'_{k \iota} = m_{\iota k}$ pour tout $(\iota, k) \in I \times K$.

Il résulte de cette définition que la transposée d’une matrice de type $(I, K)$ est une matrice de type $(K, I)$ et que l’on a
$$
{}^t({}^t M) = M.
$$

### 2. Matrices sur un groupe commutatif

Soit $G$ un groupe commutatif (noté additivement). L’ensemble des matrices sur $G$, ayant des ensembles d’indices donnés $I, K$, est muni d’une structure de *groupe commutatif*, puisque c’est l’ensemble des applications de $I \times K$ dans $G$; ce groupe est noté additivement, de sorte que si $M = (m_{\iota k})$ et $M' = (m'_{\iota k})$ sont deux de ses éléments, on a $M + M' = (m_{\iota k} + m'_{\iota k})$; l’élément neutre de ce groupe est donc la matrice dont tous les éléments sont *nuls* (dite *matrice nulle*). Il est clair que l’on a
$$
{}^t(M + M') = {}^t M + {}^t M'.
$$
La somme de deux matrices n’est donc définie que si les ensembles d’indices des lignes et des colonnes sont les *mêmes* pour les deux matrices.

Soient $H', H''$ deux ensembles, $G$ un groupe commutatif (noté additivement), et $f : (h', h'') \mapsto h'h''$ une application de $H' \times H''$ dans $G$. Étant données deux matrices
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \qquad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
sur $H'$ et $H''$ respectivement, telles que l’ensemble $K$ des indices des colonnes de $M'$ soit *fini* et égal à l’ensemble des indices des lignes de $M''$, on appelle *produit de $M'$ et $M''$ suivant $f$* et on note $M'M''$ ou $f(M', M'')$ la matrice
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
sur $G$.

La définition précédente suppose que l’ensemble des indices des colonnes de $M'$ est égal à l’ensemble des indices des lignes de $M''$; en particulier le produit $M''M'$ *n’a pas de sens si* $I \neq L$. Dans la formule (3) figurent les éléments d’une même *ligne* de $M'$, multipliés à droite par les éléments d’une même *colonne* de $M''$; on dit que la multiplication se fait « lignes par colonnes ».

Soit $f^0$ l’application $(h'', h') \mapsto h'h''$ de $H'' \times H'$ dans $G$; il résulte aussitôt des définitions que l’on a
$$
{}^t(M'M'') = {}^t M''. {}^t M'
$$
où le produit dans le premier (resp. second) membre est calculé suivant $f$ (resp. suivant $f^0$).

Lorsque $H'$ et $H''$ sont eux-mêmes des groupes commutatifs (notés additivement) et que $f$ est **Z-bilinéaire** (II, p. 50), on vérifie aussitôt les formules de *distributivité*

$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$

les ensembles d’indices étant tels que les sommes et produits écrits soient définis.

Soient maintenant $H_1, H_2, H_3, H_{12}, H_{23}$ et $H$ des groupes commutatifs (notés additivement), $f_{12}: H_1 \times H_2 \to H_{12}$, $f_{23}: H_2 \times H_3 \to H_{23}$ des applications, $f_3: H_{12} \times H_3 \to H, f_1: H_1 \times H_{23} \to H$ des applications **Z-bilinéaires**; supposons en outre que l’on ait, quels que soient les $x_i \in H_i$ ($i = 1, 2, 3$)

$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$

(ce qu’on écrit aussi comme ci-dessus $(x_1 x_2)x_3 = x_1(x_2 x_3)$); alors, si $M' = (m'_{rs})$, $M'' = (m''_{st})$, $M''' = (m'''_{tu})$ sont des matrices sur $H_1, H_2, H_3$ respectivement, on a

$$
(M'M'')M''' = M'(M''M'''')
$$

lorsque les produits des deux membres (calculés respectivement suivant $f_{12}, f_3, f_{23}$ et $f_1$) sont définis; en effet, on a

$$
\sum_t (\sum_s m'_{rs} m''_{st}) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} (\sum_t m''_{st} m'''_{tu})
$$

en vertu des hypothèses faites.

On note encore $MM'M''$ les deux membres de (6). On fera des conventions analogues pour les produits de plus de trois facteurs.

#### Remarque {#alg-ii-s10-n2-rem-1 .statement}

Les formules précédentes s’étendent à une situation plus générale. De façon précise:

a) Supposons $H = \bigcup_{(i, \kappa) \in I \times K} G_{i\kappa}$, où chaque $G_{i\kappa}$ est un groupe commutatif noté additivement; alors on peut définir la somme $M + M'$ lorsque, pour tout couple $(i, \kappa)$, on a $m_{i\kappa} \in G_{i\kappa}$ et $m'_{i\kappa} \in G_{i\kappa}$.

b) Soient $I, K, L$ trois ensembles, $K$ étant supposé fini, et soient $H' = \bigcup_{(i, k) \in I \times K} H'_{ik}$, $H'' = \bigcup_{(k, l) \in K \times L} H''_{kl}$, $H = \bigcup_{(i, l) \in I \times L} H_{il}$ trois ensembles; supposons que chaque $H_{il}$ soit un groupe commutatif noté additivement, et pour chaque triplet $(i, k, l)$, soit

$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$

une application. Alors si $M' = (m'_{ik})_{(i, k) \in I \times K}$, $M'' = (m''_{kl})_{(k, l) \in K \times L}$ sont des matrices telles que $m'_{ik} \in H'_{ik}$ et $m''_{kl} \in H''_{kl}$ quels que soient $i, k, l$ on peut définir le produit $M'M''$ suivant les $f_{ikl}$. Nous laissons au lecteur le soin d’écrire et de démontrer les formules analogues à (4), (5) et (6).

### 3. Matrices sur un anneau

Les matrices qui sont les plus importantes en Mathématique sont les matrices sur un anneau. L’ensemble $A^{I \times K}$ des matrices sur $A$, correspondant à des ensembles d’indices $I, K$, est alors canoniquement muni d’une structure de (A, A)-bimodule (II, p. 33).

Pour tout couple $(i, k) \in I \times K$, soit $E_{ik}$ la matrice $(a_{ji})$ telle que $a_{ik} = 1$ et $a_{jl} = 0$ pour $(j, l) \neq (i, k)$; on dit que les $E_{ik}$ sont les unités matricielles dans l’ensemble de matrices $A^{I \times K}$; si $I$ et $K$ sont finis, elles forment la base canonique de cet ensemble pour sa structure de A-module à gauche ou à droite (II, p. 25). Il est clair que l’on a

$$
{}^tE_{ik} = E_{ki}.
$$

Sauf mention expresse du contraire, le produit $M'M''$ de deux matrices sur $A$ (supposé défini) sera toujours entendu relativement à la multiplication $(x, y) \mapsto xy$ dans $A$ (ou, comme on dit encore, sera « calculé dans $A$ »). On a donc (II, p. 141) les formules d’associativité et de distributivité

(7)
$$(XY)Z = X(YZ)$$
(8)
$$\begin{cases}
X(Y + Z) = XY + XZ \\
(X + Y)Z = XZ + YZ
\end{cases}$$

pour trois matrices $X, Y, Z$ sur $A$, chaque fois que les sommes et produits écrits dans ces formules sont définis.

En particulier, si $E_{ik}$ (resp. $E'_{kl}, E''_{il}$) sont les unités matricielles dans $A^{I \times K}$ (resp. $A^{K \times L}, A^{I \times L}$) respectivement, avec $I = \{1, p\}, K = \{1, q\}, L = \{1, r\}$, on a les formules

(9)
$$\begin{cases}
E_{ik}E'_{jl} = 0 & \text{si } k \neq j \\
E_{ik}E'_{kl} = E''_{il}
\end{cases}$$

Soit $A^0$ l’anneau opposé de $A$, et notons $a * b \ (= ba)$ le produit de $a$ et $b$ dans $A^0$; on a alors, pour deux matrices $X, Y$ sur $A$ dont le produit est défini,

(10)
$$
{}^t(XY) = {}^tY * {}^tX
$$

où au second membre ${}^tY$ et ${}^tX$ sont considérées comme des matrices à éléments dans $A^0$ et le signe $*$ note le produit de matrices sur cet anneau; lorsque $A$ est commutatif, on a donc

(11)
$$
{}^t(XY) = {}^tY. {}^tX.
$$

#### Proposition 1 {#alg-ii-s10-prop-1 .statement}

Soient $A, B$ deux anneaux, $M = (m_{ik})_{(i, k) \in I \times K}$ et $M' = (m'_{ik})_{(i, k) \in I \times K}$ deux matrices à ensembles d’indices finis, sur un (A, B)-bimodule G. Supposons que pour toute unité matricielle $L = (a_i)_{i \in I}$ à une ligne, à éléments dans $A$, et toute unité matricielle $C = (b_k)_{k \in K}$ à une colonne, à éléments dans $B$, on ait $L.M.C = L.M'.C$ (les produits étant calculés suivant les lois externes du (A, B)-bimodule G); alors $M = M'$.

En effet, si on prend pour $L$ l’unité matricielle $(a_s)$ avec $a_i = 1$, $a_s = 0$ pour $s \neq i$, pour $C$ l’unité matricielle $(b_t)$ avec $b_k = 1$, $b_t = 0$ pour $t \neq k$, les produits $L.M.C$ et $L.M'.C$ sont des matrices à un seul élément respectivement égal à $m_{ik}$ et $m'_{ik}$.

Soient A, B deux anneaux, $\sigma : A \to B$ un homomorphisme.
Pour toute matrice $M = (m_{ik})$ sur A, nous noterons $\sigma(M)$ la matrice $(\sigma(m_{ik}))$ sur B; il est clair que l’on a $\sigma(aM) = \sigma(a)\sigma(M)$, $\sigma(Ma) = \sigma(M)\sigma(a)$ pour $a \in A$, ainsi que $\sigma(^tM) = (^t(\sigma(M)))$ et

$$
\begin{cases}
\sigma(M + M') = \sigma(M) + \sigma(M') \\
\sigma(MM') = \sigma(M)\sigma(M')
\end{cases}
$$

lorsque les opérations considérées sont définies, les produits du premier et du second membre de la seconde équation (12) étant calculés dans A et dans B respectivement. Lorsque $\sigma$ est noté $x \mapsto x^\sigma$, on écrit $M^\sigma$ au lieu de $\sigma(M)$.

Considérons en particulier un antiendomorphisme $\sigma$ de A, c’est-à-dire un homomorphisme de A dans l’anneau opposé $A^0$, ou encore une application de A dans lui-même telle que

$$
\sigma(a + a') = \sigma(a) + \sigma(a'), \quad \sigma(aa') = \sigma(a')\sigma(a)
$$

quels que soient $a, a'$ dans A; alors, pour deux matrices $M, M'$ sur A dont le produit $MM'$ est défini, on a

$$
\sigma(MM') = (^t(\sigma(^tM')).\sigma(^tM))
$$

où les produits des deux membres sont calculés dans A; cela résulte aussitôt de (10) et (12).

### 4. Matrices et applications linéaires

Soient A un anneau, E un A-module (à droite ou à gauche) admettant une base $(e_i)_{i \in I}$. Pour tout élément $x \in E$, on appelle matrice de $x$ par rapport à la base $(e_i)$ et on note $M(x)$ ou $x$ (ou même parfois $x$ lorsqu’il n’en résulte pas de confusion), la matrice colonne formée des composantes $x_i$ ($i \in I$) de $x$ par rapport à $(e_i)$ (II, p. 25); dans les calculs, il sera parfois commode, afin de rappeler que l’indice $i$ est un indice de ligne, de lui adjoindre un indice de colonne susceptible de prendre une seule valeur, et d’écrire $(x_{i0})$ la matrice $M(x)$.

Considérons maintenant deux A-modules (à gauche ou à droite) E et F ayant des bases $(e_i)_{i \in I}$ et $(f_k)_{k \in K}$ respectivement; soit $(f_k^*)$ la famille des formes coordonnées correspondant à $(f_k)$. Pour une application $u$ de E dans F, nous allons définir la matrice de $u$ par rapport aux bases $(e_i), (f_k)$, dans chacun des cas suivants:
(D) E et F sont des A-modules à droite, $u$ est A-linéaire.
(G) E et F sont des A-modules à gauche, $u$ est A-linéaire.

Dans la suite, nous affecterons de la lettre (D) (resp. (G)) les formules s’appliquant aux modules à droite (resp. à gauche).

#### Définition 3 {#alg-ii-s10-def-3 .statement}

Dans chacun des deux cas précédents, on appelle matrice de u par rapport aux bases $(e_i), (f_k)$ la matrice $M(u) = (u_{ki})_{(k, i) \in K \times I}$ telle que
$$
u_{ki} = f_k^*(u(e_i))
$$
ce qui s’écrit suivant les cas
$$
\begin{align*}
(14\text{ D}) \quad & u_{ki} = \langle f_k^*, u(e_i) \rangle \\
(14\text{ G}) \quad & u_{ki} = \langle u(e_i), f_k^* \rangle.
\end{align*}
$$
La colonne d’indice $i$ de $M(u)$ est donc égale à $M(u(e_i))$.

Il est clair que si $u, v$ sont deux applications linéaires de $E$ dans $F$, $M(u)$, $M(v)$ leurs matrices par rapport aux mêmes bases, on a, par rapport à ces bases,
$$
M(u + v) = M(u) + M(v)
$$
et
$$
M(\gamma u) = \gamma M(u)
$$
pour tout élément $\gamma$ du centre $\Gamma$ de $A$. En d’autres termes, une fois les bases $(e_i), (f_k)$ fixées, l’application $u \mapsto M(u)$ est un isomorphisme de $\Gamma$-modules de $\mathrm{Hom}_A(E, F)$ sur une partie de l’ensemble $A^{K \times I}$, égale à $A^{K \times I}$ si $K$ est fini.

#### Proposition 2 {#alg-ii-s10-prop-2 .statement}

Supposons $I$ et $K$ finis. Pour tout élément $x \in E$, la matrice $M(u(x))$ par rapport à la base $(f_k)$ est donnée par la formule
$$
\begin{align*}
(17\text{ D}) \quad & M(u(x)) = M(u) \cdot M(x) \\
(17\text{ G}) \quad & {}^tM(u(x)) = {}^tM(x) \cdot {}^tM(u).
\end{align*}
$$
Vérifions par exemple (17 G). Posons $x = \sum_i x_{i0} e_i$, $u(x) = \sum_k y_{k0} f_k$ avec $x_{i0} \in A$, $y_{k0} \in A$; on a $u(x) = u(\sum_i x_{i0} e_i) = \sum_i x_{i0} u(e_i) = \sum_{i, k} x_{i0} u_{ki} f_k$; d’où $y_{k0} = \sum_i x_{i0} u_{ki}$. Afin d’amener l’un à côté de l’autre les deux indices $i$, considérons les matrices transposées ${}^tM(x) = (x'_{0i})$ où $x'_{0i} = x_{i0}$ et ${}^tM(u) = (u'_{ik})$ où $u'_{ik} = u_{ki}$; on a alors $y_{k0} = \sum_i x'_{0i} u'_{ik}$, et le second membre est l’élément d’indice $k$ de la matrice à une ligne ${}^tM(x) \cdot {}^tM(u)$, d’où (17 G).

Lorsque $A$ est commutatif, (17 G) se ramène à (17 D) au moyen de la formule (4) de II, p. 140.

#### Corollaire {#alg-ii-s10-n4-cor-1 .statement}

Soient $E, F, G$ trois modules à droite (resp. à gauche) sur un anneau $A$, $(e_i)_{i \in I}, (f_k)_{k \in K}, (g_l)_{l \in L}$ des bases finies respectives de $E, F, G$, $u : E \to F$, $v : F \to G$ deux applications linéaires, $M(u)$ la matrice de $u$ relative aux bases $(e_i), (f_k)$, $M(v)$ la

matrice de v relative aux bases $(f_k), (g_l)$, $M(v \circ u)$ la matrice de $v \circ u$ relative aux bases $(e_i), (g_l)$; on a alors
(18 D)
$$
M(v \circ u) = M(v)M(u)
$$
(18 G)
$$
{}^tM(v \circ u) = {}^tM(u).{}^tM(v).
$$

Démontrons par exemple (18 G). Quel que soit $x \in E$, on a en vertu de (17 G):
$$
{}^tM(x).{}^tM(v \circ u) = {}^tM(v(u(x)))
$$
$$
= {}^tM(u(x)).{}^tM(v) = {}^tM(x).{}^tM(u).{}^tM(v)
$$
par associativité; le corollaire résulte donc de la prop. 1 (II, p. 142), la matrice à une ligne ${}^tM(x)$ étant arbitraire.

Remarque 1). — La formule (17 D) peut être considérée comme un cas particulier de (18 D). En effet, à tout $x \in E$ correspond canoniquement l’application linéaire $\theta_x : A_d \to E$ qui à tout $\alpha \in A$ fait correspondre $x\alpha$ (II, p. 36). Il est immédiat que la matrice $M(\theta_x)$ par rapport à la base 1 de $A_d$ et à la base $(e_i)$ de $E$ n’est autre que la matrice $M(x)$; de même on a $M(\theta_{u(x)}) = M(u(x))$ et on peut donc considérer que la formule (17 D) est une traduction de la relation $\theta_{u(x)} = u \circ \theta_x$.

#### Proposition 3 {#alg-ii-s10-prop-3 .statement}

Soient $E, F$ deux $A$-modules à droite (resp. à gauche), $(e_i)_{i \in I}$, $(f_k)_{k \in K}$ des bases finies de $E$ et $F$ respectivement. Pour toute application linéaire $u$ de $E$ dans $F$, soit $M(u)$ la matrice de $u$ par rapport aux bases $(e_i)$ et $(f_k)$. Alors la matrice de ${}^t u : F^* \to E^*$ par rapport aux bases duales $(f_k^*)$ et $(e_i^*)$ est égale à ${}^tM(u)$.

En effet, $E$ est canoniquement identifié à son bidual $E^{**}$ et $(e_i)$ à la base duale de $(e_i^*)$; on a alors (en supposant par exemple que $E$ et $F$ soient des modules à droite) $\langle {}^t u(f_k^*), e_i \rangle = \langle f_k^*, u(e_i) \rangle$, d’où la proposition.

#### Remarque 2 {#alg-ii-s10-n4-rem-2 .statement}

Soient $E$ et $F$ deux $A$-modules à gauche ayant des bases $(e_i)_{i \in I}$ et $(f_k)_{k \in K}$ respectivement. Pour toute application $A$-linéaire $u : E \to F$, on a, d’après (14 G), $u(e_i) = \sum_k u_{ki} f_k$; ces relations peuvent encore s’interpréter en disant que la matrice colonne $(u(e_i))_{i \in I}$ à éléments dans $F$ est égale au produit ${}^tM(u).(f_k)$, où $(f_k)_{k \in K}$ est considéré comme une matrice colonne à éléments dans $F$, et le produit est calculé pour l’application $A \times F \to F$ définissant la loi d’action du $A$-module $F$ (II, p. 140).

#### Remarque 3 {#alg-ii-s10-n4-rem-3 .statement}

Soient $A, B$ deux anneaux commutatifs, $\sigma : A \to B$ un homomorphisme d’anneaux. Les notations étant celles de la prop. 3, $(e_i \otimes 1)$ et $(f_k \otimes 1)$ sont des bases respectives de $E_{(B)} = E \otimes_A B$ et $F_{(B)} = F \otimes_A B$ (II, p. 84, prop. 4); en outre, si $(e_i^*)$ et $(f_k^*)$ sont respectivement les bases duales de $(e_i)$ et $(f_k)$, alors $(e_i^* \otimes 1)$ et $(f_k^* \otimes 1)$ sont respectivement les bases duales de $(e_i \otimes 1)$ et $(f_k \otimes 1)$ (II, p. 88). Pour toute application $A$-linéaire $u : E \to F$, soient $M(u)$ et $M(u \otimes 1)$ la matrice de $u$ par rapport à $(e_i)$ et $(f_k)$ et la matrice de l’application $B$-linéaire $u \otimes 1$ par rapport à $(e_i \otimes 1)$ et $(f_k \otimes 1)$. Il résulte de II, p. 87, formule (20) que l’on a
$$
M(u \otimes 1) = \sigma(M(u)).
$$

Considérons un système d’un nombre fini d’équations linéaires scalaires à droite à un nombre fini d’inconnues
$$
\sum_{i \in I} a_{ki} x_i = b_k \quad (k \in K)
$$
avec $a_{ki}, x_i, b_k$ dans $A$.

Soient $(e_i)_{i \in I}, (f_k)_{k \in K}$ les bases canoniques de $E = A_d^I$ et $F = A_d^K$; le système (19) est équivalent à l’équation $u(x) = b$, où $x = \sum_i e_i x_i$, $b = \sum_k f_k b_k$ et $u : E \to F$ est l’application linéaire telle que la matrice $M(u)$, par rapport aux bases $(e_i)$ et $(f_k)$, soit égale à $A = (a_{ki})_{(k, i) \in K \times I}$. On dit cette matrice est la matrice du système d’équations linéaires (19). Rappelons (II, p. 49, Remarques 2 et 3) que si on pose $c_i = \sum_k f_k a_{ki}$, le système (19) équivaut à l’unique équation vectorielle

$$
\sum_i c_i x_i = b,
$$

et comme $c_i$ est la colonne d’indice $i$ de la matrice $A$, on voit que dire que le système (19) admet une solution revient à dire que la matrice à une colonne $b = (b_{k0})$ est combinaison linéaire des colonnes de la matrice $A$.

Nous laissons au lecteur le soin de formuler les définitions et remarques analogues pour les systèmes d’équations linéaires à gauche.

### 5. Produit par blocs

Les définitions du n° 4 se généralisent de la façon suivante. Soit $E$ un $A$-module (à droite ou à gauche), somme directe d’une famille $(E_i)_{i \in I}$ de sous-modules. Pour tout $x \in E$, soit $x = \sum_{i \in I} x_i$ avec $x_i \in E_i$ pour tout $i \in I$; nous dirons que la matrice colonne $M(x) = (x_i)_{i \in I}$ à éléments dans $E$ est la matrice de $x$ par rapport à la décomposition $(E_i)_{i \in I}$ de $E$ en somme directe.

Soit $F$ un second $A$-module ($E$ et $F$ étant tous deux des $A$-modules à droite ou tous deux des $A$-modules à gauche), et supposons que $F$ soit somme directe d’une famille $(F_k)_{k \in K}$ de sous-modules. Pour tout $u \in \mathrm{Hom}(E, F)$ et tout $x_i \in E_i$, posons $u(x_i) = \sum_k u_{ki}(x_i)$ avec $u_{ki}(x_i) \in F_k$ pour tout $k \in K$; on a $u_{ki} \in \mathrm{Hom}(E_i, F_k)$; nous dirons que la matrice $M(u) = (u_{ki})_{(k, i) \in K \times I}$ de type $(K, I)$, à éléments dans l’ensemble $H$ somme des $\mathrm{Hom}(E_i, F_k)$, est la matrice de $u$ par rapport aux décompositions $(E_i)$ et $(F_k)$ de $E$ et $F$ en sommes directes.

Avec ces définitions, il est évident que si $u, v$ sont deux applications $A$-linéaires de $E$ dans $F$, on a, pour les matrices par rapport aux mêmes décompositions en sommes directes

$$
M(u + v) = M(u) + M(v), \quad M(\gamma u) = \gamma M(u)
$$

pour tout élément $\gamma$ du centre de $A$ (cf. II, p. 141, Remarque).

En outre, la définition des $u_{ki}$ montre que si $K$ est fini, on peut écrire

$$
M(u(x)) = M(u) \cdot M(x)
$$

où $M(u(x))$ est la matrice de $u(x)$ par rapport à la décomposition $(F_k)$, le produit du second membre de (22) étant calculé pour les applications $(t, z) \mapsto t(z)$ de $\operatorname{Hom}(E_i, F_k) \times E_i$ dans $F_k$ (II, p. 141, Remarque).

Soit G un troisième A-module, somme directe d’une famille $(G_l)_{l \in L}$ de sous-modules, de sorte qu’à toute application A-linéaire $v : F \to G$ correspond une matrice $M(v) = (v_{lk})$ par rapport aux décompositions $(F_k)$ et $(G_l)$. Si I, K et L sont finis, on a alors

$$(23)$$
$$
M(v \circ u) = M(v) \cdot M(u)
$$

où le premier membre est la matrice $(w_{li})$ de $w = v \circ u$ par rapport aux décompositions $(E_i)$ et $(G_l)$, et le produit du second membre est calculé pour les applications $(t, s) \mapsto t \circ s$ de $\operatorname{Hom}(F_k, G_l) \times \operatorname{Hom}(E_i, F_k)$ dans $\operatorname{Hom}(E_i, G_l)$ (II, p. 141, Remarque). Cela n’est en effet autre chose que la formule (32) de II, p. 19, exprimée en termes de matrices.

Enfin, si on suppose I et K finis, $E^*$ (resp. $F^*$) s’identifie canoniquement à la somme directe des modules $E_i^*$ (resp. $F_k^*$) (II, p. 44, prop. 10). On vérifie alors aussitôt que la matrice de $^t u$ par rapport aux décompositions $(F_k^*)$ et $(E_i^*)$ n’est autre que $(^t u_{ki})_{(i,k) \in I \times K}$.

Supposons maintenant que I et K soient finis et en outre que chacun des $E_i$ (resp. $F_k$) admette une base finie. Il revient au même de dire que E (resp. F) admet une base $(e_r)_{r \in R}$ (resp. $(f_s)_{s \in S}$) et que R (resp. S) admet une partition $(R_i)_{i \in I}$ (resp. $(S_k)_{k \in K}$) telle que pour tout $i \in I$ (resp. $k \in K$), $(e_r)_{r \in R_i}$ soit une base de $E_i$ (resp. $(f_s)_{s \in S_k}$ une base de $F_k$). Alors, si $X = M(u)$ est la matrice de $u$ par rapport aux bases $(e_r)_{r \in R}$ et $(f_s)_{s \in S}$, la matrice $X_{ki} = M(u_{ki})$ par rapport aux bases $(e_r)_{r \in R_i}$ et $(f_s)_{s \in S_k}$ n’est autre que la sous-matrice de $X$ obtenue en supprimant les lignes d’indice $s \notin S_k$ et les colonnes d’indice $r \notin R_i$. On définit ainsi une application bijective

$$(24)$$
$$
X \mapsto (X_{ki})_{(i,k) \in I \times K}
$$

de l’ensemble des matrices de type (S, R) à éléments dans A sur l’ensemble des matrices de matrices $(X_{ki})_{(k, i) \in K \times I}$ de type $K \times I$, où chaque $X_{ki}$ est une matrice sur A de type $(S_k, R_i)$. Supposons que de plus G admette une base finie $(g_t)_{t \in T}$, et que $T = (T_l)_{l \in L}$ soit une partition de T telle que pour chaque $l \in L$, $(g_t)_{t \in T_l}$ soit une base de $G_l$; soient $Y = M(v)$ la matrice de $v$ par rapport aux bases $(f_s)_{s \in S}$ et $(g_t)_{t \in T}$, $Y_{lk} = M(v_{lk})$ celle de $v_{lk}$ par rapport aux bases $(f_s)_{s \in S_k}$ et $(g_t)_{t \in T_l}$, $Z = M(w)$ la matrice de $w = v \circ u$ par rapport aux bases $(e_r)_{r \in R}$ et $(g_t)_{t \in T}$, $Z_{li} = M(w_{li})$ celle de $w_{li}$ par rapport aux bases $(e_r)_{r \in R_l}$ et $(g_t)_{t \in T_l}$; on déduit alors de (23) que les sous-matrices $Z_{li}$ de $Z = YX$ sont données par

$$(25)$$
$$
Z_{li} = \sum_k Y_{lk} X_{ki}
$$

autrement dit, l’application bijective (24) transforme les produits en produits lorsque tous les produits considérés sont définis (les produits de matrices de matrices étant définis au sens de II, p. 141, Remarque); lorsqu’on calcule ainsi les sous-matrices $Z_{li}$ du produit $YX$, on dit qu’on effectue ce produit « par blocs ».

Ce nom provient de ce que, lorsque $I = (1, p)$ et $K = (1, q)$, on imagine le tableau représentant la matrice $X$ comme partagé en « blocs » formant un « tableau de matrices »

$$
\begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
X_{21} & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
X_{q1} & X_{q2} & \cdots & X_{qp}
\end{pmatrix}
$$

que l’on considère comme un symbole notant $X$ lorsque $p$ et $q$ sont des entiers explicités assez petits pour que ce soit praticable.

### 6. Matrice d’une application semi-linéaire

Soient $A, B$ deux anneaux, $\sigma : A \to B$ un homomorphisme de $A$ dans $B$, $E$ un $A$-module à droite (resp. à gauche) ayant une base $(e_i)_{i \in I}$, $F$ un $B$-module à droite (resp. à gauche) ayant une base $(f_k)_{k \in K}$. Soit $u : E \to F$ une application semi-linéaire relative à $\sigma$ et soit $u(e_i) = \sum_{k \in K} f_k u_{ki}$ (resp. $u(e_i) = \sum_{k \in K} u_{ki} f_k$), où les $u_{ki}$ sont donc des éléments de $B$; par définition, la matrice $M(u) = (u_{ki})$ de type $K \times I$ est encore appelée la matrice de $u$ par rapport aux bases $(e_i)$ et $(f_k)$. Par le même calcul que pour la prop. 2 de II, p. 144, on vérifie aussitôt que pour tout $x \in E$, on a, si $I$ et $K$ sont finis,

(26 D)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
(resp.
(26 G)
$$
{}^t M(u(x)) = \sigma({}^t M(x)) \cdot {}^t M(u).
$$)

Soient $C$ un troisième anneau, $\tau : B \to C$ un homomorphisme, $G$ un $C$-module à droite (resp. à gauche) ayant une base $(g_l)_{l \in L}$, $v$ une application semi-linéaire de $F$ dans $G$ relative à $\tau$; si $M(v)$ est la matrice de $v$ par rapport à $(f_k)$ et $(g_l)$, $M(v \circ u)$ la matrice de $v \circ u$ relative à $(e_k)$ et $(g_l)$, on a cette fois, si $I, K, L$ sont finis,

(27 D)
$$
M(v \circ u) = M(v) \cdot \tau(M(u))
$$
(resp.
(27 G)
$$
{}^t M(v \circ u) = \tau({}^t M(u)) \cdot {}^t M(v).
$$)

En effet, pour démontrer par exemple (27 D), notons que pour tout $x \in E$, on a par (26 D),
$$
M(v \circ u) \cdot \tau(\sigma(M(x))) = M(v(u(x))) = M(v) \cdot \tau(M(u(x))) =
M(v) \cdot \tau(M(u)) \cdot \tau(\sigma(M(x))),
$$
d’où (27 D) par la prop. 1 de II, p. 142.

Supposons enfin que $\sigma : A \to B$ soit un isomorphisme; rappelons alors que $^t u : F^* \to E^*$ est une application semi-linéaire relative à $\sigma^{-1}$ (II, p. 43); lorsque I et K sont finis, la matrice de $^t u$ par rapport aux bases duales $(f_k^*)$ et $(e_i^*)$ est donnée par

$$
M(^t u) = \sigma^{-1}(^t M(u))
$$

car on a ici, par définition, en supposant par exemple que E et F soient des modules à droite, $\langle ^t u(f_k^*), e_i \rangle^\sigma = \langle f_k^*, u(e_i) \rangle$ lorsque $\sigma$ est noté $x \mapsto x^\sigma$.

#### Remarque {#alg-ii-s10-n6-rem-1 .statement}

Soient A un anneau, $\sigma$ un antiendomorphisme de A (II, p. 143); considérons les deux situations suivantes:
(GD) E est un A-module à gauche, F un A-module à droite, $u$ une application $\mathbf{Z}$-linéaire de E dans F telle que $u(ax) = u(x)\sigma(a)$ pour $a \in A, x \in E$; en d’autres termes, $u$ est une application *semi-linéaire* relative à $\sigma$ du $A^0$-module à droite E dans le A-module à droite F.
(DG) E est un A-module à droite, F un A-module à gauche, $u$ une application $\mathbf{Z}$-linéaire de E dans F telle que $u(xa) = \sigma(a)u(x)$ pour $a \in A, x \in E$; en d’autres termes, $u$ est une application *semi-linéaire* relative à $\sigma$ du $A^0$-module à gauche E dans le A-module à gauche F.
Dans les deux cas, la matrice $M(u)$ de $u$ relative à des bases de E et F a ses éléments dans A; si ces bases sont finies, on a, pour tout $x \in E$, les formules respectives
(17 GD)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
(17 DG)
$$
^t M(u(x)) = \sigma(^t M(x)) \cdot ^t M(u),
$$
les produits des deux membres étant calculés *dans* A. Cela résulte aussitôt de (26 D) et (26 G) respectivement.

### 7. Matrices carrées

#### Définition 4 {#alg-ii-s10-def-4 .statement}

*On appelle matrice carrée une matrice dont les lignes et les colonnes ont même ensemble d’indices*.

On dit qu’une matrice carrée ayant $n$ lignes et $n$ colonnes est une *matrice d’ordre n*.

#### Remarque {#alg-ii-s10-n7-rem-1 .statement}

On aura soin de noter qu’une matrice dont les ensembles des indices de lignes et des indices de colonnes ont *même cardinal*, mais *ne sont pas identiques*, ne doit pas être considérée comme une matrice carrée; en particulier, le produit de deux telles matrices sur un anneau *n’est pas défini*.

Il est clair que l’addition et la multiplication des matrices carrées sur A, ayant un ensemble fini I pour ensemble d’indices des lignes et des colonnes, définissent sur l’ensemble de ces matrices une structure *d’anneau*, en raison des formules (7), (8) et (9) (II, p. 142): la matrice $(\delta_{ij})$ où $\delta_{ij}$ est l’indice de Kronecker (pour $i \in I, j \in I$) est l’élément unité de cet anneau et se note $I_n$ ou $1_n$ lorsque I a $n$ éléments. Lorsque $I = \{1, n\}$, on désignera simplement par $\mathbf{M}_n(A)$ l’anneau de matrices ainsi défini; le groupe des éléments inversibles de $\mathbf{M}_n(A)$ se désigne par $\mathbf{GL}_n(A)$ ou $\mathbf{GL}(n, A)$.
Pour qu’une matrice carrée $U = (a_{ij})$ d’ordre $n$ sur A soit inversible à droite (resp. à gauche), il faut et il suffit que pour tout système $(b_i)_{1 \leq i \leq n}$ d’éléments de $A$, le système de $n$ équations à $n$ inconnues

$$
\sum_{j=1}^n a_{ij} x_j = b_i \qquad (1 \leq i \leq n)
$$

(resp. $\sum_{j=1}^n x_j a_{ji} = b_i$)

ait une solution $(x_i)$ dans $A$.

Soient $I$ un ensemble d’indices fini, $A$ un anneau, $E$ un $A$-module à droite (resp. à gauche) ayant une base $(e_i)_{i \in I}$. Pour tout endomorphisme $u$ de $E$, la matrice $M(u)$ de $u$ par rapport aux deux bases identiques à $(e_i)$, est une matrice carrée; pour abréger, on dit que c’est la matrice de $u$ par rapport à la base $(e_i)$.

Supposons que $I = \{1, n\}$. L’application $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) est un isomorphisme de l’anneau $\mathrm{End}_A(E)$ sur $\mathbf{M}_n(A)$ (resp. sur l’anneau opposé à $\mathbf{M}_n(A)$), comme il résulte des formules (18 D) (resp. (18 G)) (II, p. 145). Les éléments inversibles de l’anneau $\mathbf{M}_n(A)$, dits matrices inversibles, correspondent par l’application $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) aux automorphismes de $E$; le groupe $\mathbf{GL}(n, A)$ s’identifie donc canoniquement au groupe $\mathbf{GL}(A_d^n)$.

Si $u$ est un automorphisme de $E$, son contragrédient $\check{u}$ est un automorphisme du $A$-module à gauche (resp. à droite) $E^*$, tel que $\check{u} = ({}^t u)^{-1} = {}^t (u^{-1})$ (II, p. 43, déf. 6); si $M(\check{u})$ est la matrice de $\check{u}$ par rapport à la base duale $(e_i^*)$, on a donc, en vertu de II, p. 145, prop. 3

$$
M(\check{u}) = ({}^t M(u))^{-1} = {}^t M(u^{-1}).
$$

Pour toute matrice inversible $X$, on a donc ${}^t (X^{-1}) = ({}^t X)^{-1}$; on note encore cette matrice ${}^t X^{-1}$, et on l’appelle la contragrédiente de la matrice $X$.

Soit $\sigma$ un automorphisme de l’anneau $A$; pour toute application semi-linéaire $u : E \to E$ relative à $\sigma$, la matrice $M(u)$ de cette application par rapport à une base $(e_i)$ de $E$ est encore une matrice carrée. Il résulte aussitôt de (27 D) (II, p. 148) que si $u$ est bijective, on a

$$
M(u^{-1}) = (\sigma^{-1}(M(u)))^{-1}.
$$

Soit $E$ un $A$-module somme directe d’une famille finie $(E_i)_{i \in I}$ de sous-modules; pour tout endomorphisme $u$ de $E$, la matrice $M(u) = (u_{ki})$ de $u$ par rapport aux deux décompositions de $E$ identiques à $(E_i)$ (II, p. 146) est une matrice carrée d’applications linéaires. Pour que $u(E_i) \subset E_i$ pour tout $i \in I$, il faut et il suffit que $u_{ki} = 0$ pour $k \neq i$. Lorsque $I = \{1, n\}$, les relations

$$
u(E_i) \subset E_i + E_{i+1} + \cdots + E_n \qquad (1 \leq i \leq n)
$$

équivalent aux relations $u_{ki} = 0$ pour $k < i$.

Exemples de matrices carrées. — I. Matrices diagonales. Dans une matrice carrée $M = (m_{ik})_{(i, k) \in I \times I}$, les éléments dont les deux indices sont égaux sont appelés éléments diagonaux et la famille $(m_{\iota k})_{\iota \in I}$ est appelée la diagonale de $M$; une matrice carrée $M = (m_{\iota k})$ sur un anneau, dont les éléments autres que les éléments diagonaux sont nuls, est appelée matrice diagonale. Pour toute famille $(a_\iota)_{\iota \in I}$ d’éléments d’un anneau $A$, on note $\operatorname{diag}(a_\iota)_{\iota \in I}$ (ou $\operatorname{diag}(a_1, a_2, \ldots, a_n)$ lorsque $I = \{1, n\}$) la matrice diagonale $(m_{\iota k})$ telle que $m_{\iota \iota} = a_\iota$ pour tout $\iota \in I$. Dans l’ensemble $\mathbf{M}_n(A)$ des matrices carrées d’ordre $n$ sur $A$, la matrice unité $I_n$ est une matrice diagonale, ainsi que tout multiple $aI_n = I_n a$ de cette matrice par un scalaire $a$ (matrice diagonale (dite scalaire) dont tous les éléments diagonaux sont égaux à $a$).

Pour toute famille $(d_i)_{i \leq 1 \leq n}$ d’éléments de $A$ et toute matrice $X = (x_{ij})$ de type $(n, q)$ (resp. $(p, n)$) sur $A$, on a, en posant $D = \operatorname{diag}(d_i)$

$$
\begin{cases}
DX = (d_i x_{ij}) \\
XD = (x_{ij} d_j).
\end{cases}
$$

En particulier, pour deux matrices diagonales d’ordre $n$, on a

$$
\begin{cases}
\operatorname{diag}(a_i) + \operatorname{diag}(b_i) = \operatorname{diag}(a_i + b_i) \\
\operatorname{diag}(a_i) \cdot \operatorname{diag}(b_i) = \operatorname{diag}(a_i b_i).
\end{cases}
$$

Les matrices diagonales forment donc un sous-anneau de $\mathbf{M}_n(A)$ isomorphe à l’anneau produit $A^n$; les matrices scalaires forment un sous-anneau isomorphe à $A$.

II. Matrices de permutations; matrices monomiales. Soit $\pi$ une permutation quelconque d’un ensemble fini $I$, et soit $(e_i)_{i \in I}$ la base canonique du $A$-module $E = A^I_d$; il existe un endomorphisme $u_\pi$ de $E$ et un seul tel que pour tout $i \in I$, $u_\pi(e_i) = e_{\pi(i)}$ (II, p. 25, cor. 3). Pour tout $i \in I$, la colonne d’indice $i$ de la matrice $M(u_\pi)$ par rapport à la base $(e_i)$ a tous ses éléments nuls, sauf celui qui se trouve dans la ligne d’indice $\pi(i)$ et qui est égal à 1. Par abus de langage, on dit que $M(u_\pi)$ est la matrice de la permutation $\pi$. Il est immédiat que pour deux permutations quelconques $\sigma, \tau$ de $I$, on a $u_{\sigma \tau} = u_\sigma \circ u_\tau$, et que pour la permutation identique $\varepsilon$, $u_\varepsilon$ est l’identité; l’application $\pi \mapsto M(u_\pi)$ est donc un isomorphisme du groupe symétrique $\mathfrak{S}_I$ sur le groupe des matrices de permutation.

Chaque ligne et chaque colonne d’une matrice de permutation ne contient qu’un seul élément $\neq 0$. Une matrice carrée finie $R$ sur un anneau $A$ non réduit à 0, ayant cette propriété, est dite matrice monomiale; soit $r_i$ l’unique élément $\neq 0$ de la colonne d’indice $i$ de $R$, et soit $\pi(i)$ l’indice de la ligne où se trouve cet élément; il est clair que $\pi$ est une permutation de l’ensemble $I$ des indices et que l’on a $R = M(u_\pi) D$, où $D = \operatorname{diag}(r_i)$.

III. Matrices triangulaires. Dans l’anneau $\mathbf{M}_n(A)$ des matrices carrées d’ordre $n$ sur un anneau $A$, on appelle matrice triangulaire supérieure (resp. inférieure) toute matrice $(a_{ij})$ telle que $a_{ij} = 0$ pour $i > j$ (resp. $i < j$); on dit encore qu’une telle matrice n’a que des zéros au-dessous (resp. au-dessus) de sa diagonale. On constate aussitôt que les matrices triangulaires supérieures (resp. inférieures) forment un sous-anneau S (resp. T) de $\mathbf{M}_n(A)$, S $\cap$ T étant évidemment l’anneau des matrices diagonales.

L’ensemble S’ (resp. T’) des matrices de S (resp. T) dont les éléments diagonaux sont *inversibles* est un *groupe* multiplicatif de matrices dit *groupe trigonal large supérieur* (resp. *inférieur*) ; cela résulte aussitôt de II, p. 27, *Remarque* 5. L’ensemble S$_1$ (resp. T$_1$) des matrices de S (resp. T) dont les éléments diagonaux sont tous égaux à 1 est un *sous-groupe* du précédent, appelé *groupe trigonal strict supérieur* (resp. *inférieur*) et toute matrice $M \in S'$ (resp. $M \in T'$) dont ($d_i$) est la diagonale, s’écrit $M = D M_1 = M'_1 D$, où $D = \operatorname{diag} (d_i)$ et $M_1$ et $M'_1$ des matrices appartenant à S$_1$ (resp. T$_1$).

**IV. Matrices diagonales et matrices triangulaires de matrices.** Soit $(I_k)_{1 \leq k \leq p}$ une partition de l’ensemble fini I ; toute matrice carrée sur un anneau A ayant I pour ensemble d’indices peut s’écrire sous forme de *matrice carrée de matrices* correspondant à *la même partition* ($I_k$) de l’ensemble d’indices des lignes et de l’ensemble d’indices des colonnes (II, p. 147)

$$
\begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
X_{21} & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
X_{p1} & X_{p2} & \cdots & X_{pp}
\end{pmatrix}
$$

où chaque $X_{lclc}$ est une matrice carrée ayant $I_k$ pour ensemble d’indices des lignes et des colonnes.

Cela étant, on dira que (32) est une *matrice diagonale* (resp. *triangulaire supérieure*, resp. *triangulaire inférieure*) *de matrices* si toutes les matrices $X_{ij}$ telles que $i \neq j$ (resp. $i > j$, resp. $i < j$) sont *nulles*. On a vu plus haut comment s’interprètent les endomorphismes $u$ dont la matrice est une matrice diagonale, resp. triangulaire inférieure, de matrices, en considérant la matrice correspondante $M(u)$ d’applications linéaires. Les matrices triangulaires inférieures (resp. triangulaires supérieures, diagonales) de matrices pour une partition donnée ($I_k$) de I forment un *sous-anneau* de l’anneau de matrices $A^{I \times I}$. En particulier l’anneau des matrices diagonales de matrices relatif à la partition ($I_k$) est isomorphe au produit $\prod_{k=1}^p \operatorname{End}_A(E_k)$.

### 8. Changements de bases

#### Proposition 4 {#alg-ii-s10-prop-4 .statement}

*Soit E un A-module à droite ayant une base finie* $(e_i)_{1 \leq i \leq n}$ *de n éléments. Pour qu’une famille de n éléments* $e'_i = \sum_{j=1}^n e_j a_{ji}$ (*$1 \leq i \leq n$*) *soit une base de E, il faut et il suffit que la matrice carrée* $P = (a_{ji})$ *d’ordre n soit inversible.*

En effet, $P$ n’est autre que la matrice, par rapport à la base $(e_i)$, de l’endomorphisme $u$ de E défini par $u(e_i) = e'_i$ (*$1 \leq i \leq n$*). Or, pour que $u$ soit un automorphisme de E, il faut et il suffit que $(u(e_i))$ soit une base de E (II, p. 25, cor. 3) ; d’où la proposition.

On dit que la matrice inversible $P$ est la *matrice de passage de la base* $(e_i)$ *à la base* $(e'_i)$. On peut aussi l’interpréter comme la matrice de l’application identique l_E par rapport aux bases (e'_i) et (e_i) (dans cet ordre); il est clair alors que la matrice de passage de la base (e'_i) à la base (e_i) est l’inverse P^{-1} de P.

#### Proposition 5 {#alg-ii-s10-prop-5 .statement}

Soient (e_i), (e'_i) deux bases de n éléments de E, P la matrice de passage de (e_i) à (e'_i). Si (e_i^*) et (e'_i^*) sont les bases duales respectives de (e_i) et (e'_i), la matrice de passage de (e_i^*) à (e'_i^*) est la contragrédiente tP^{-1} de P.

En effet, la transposée de l’application identique l_E est l’application identique l_{E*}; en vertu de la prop. 3 de II, p. 145, la matrice de l_{E*}, par rapport aux bases (e'_i^*) et (e_i^*) (dans cet ordre) est la transposée de la matrice de l_E par rapport aux bases (e_i) et (e'_i) (dans cet ordre), c’est-à-dire la transposée de P^{-1}.

#### Proposition 6 {#alg-ii-s10-prop-6 .statement}

Soient E et F deux A-modules à droite, (e_i) et (e'_i) deux bases de E ayant n éléments, (f_j) et (f'_j) deux bases de F ayant m éléments, P la matrice de passage de (e_i) à (e'_i), Q la matrice de passage de (f_j) à (f'_j). Pour toute application linéaire u de E dans F, soient M(u) la matrice de u par rapport aux bases (e_i) et (f_j), M'(u) la matrice de u par rapport aux bases (e'_i) et (f'_j); on a alors
(33 D)
$$
M'(u) = Q^{-1} M(u) P.
$$
En effet, on peut écrire $u = 1_F \circ u \circ 1_E$. La formule (33) résulte aussitôt de II, p. 144, corollaire, lorsqu’on prend la matrice de l_E par rapport à (e'_i) et (e_i), celle de u par rapport à (e_i) et (f_j) et celle de 1_F par rapport à (f_j) et (f'_j).

#### Corollaire 1 {#alg-ii-s10-prop-6-cor-1 .statement}

Si u est un endomorphisme de E, M(u) et M'(u) ses matrices par rapport aux bases (e_i) et (e'_i) respectivement, on a
(34 D)
$$
M'(u) = P^{-1} M(u) P.
$$

#### Corollaire 2 {#alg-ii-s10-prop-6-cor-2 .statement}

Si M(x) et M'(x) sont les matrices à une colonne d’un même élément $x \in E$ par rapport aux bases (e_i) et (e'_i) respectivement, on a
(35 D)
$$
M(x) = P . M'(x).
$$
C’est un cas particulier de la prop. 6, où l’on prend pour u l’application $\theta_x : a \mapsto xa$ de $A_d$ dans E (II, p. 145, Remarque 1).

Si $P = (a_{ij})$, la formule (35 D) équivaut à
(36 D)
$$
x_i = \sum_{j=1}^n a_{ij} x'_j \qquad (1 \leq i \leq n)
$$
pour les éléments $x_i$ et $x'_i$ des matrices $M(x)$ et $M'(x)$ respectivement. Les formules (36 D) sont dites formules de changement de coordonnées. On observera qu’elles expriment les composantes de x relatives à l'« ancienne » base (e_i) en fonction des composantes de x relatives à la « nouvelle » base (e'_i) et des éléments de P, c’est-à-dire des composantes de la « nouvelle » base relatives à l'« ancienne » base.

#### Remarque 1 {#alg-ii-s10-n8-rem-1 .statement}

Partons maintenant d’un A-module à gauche E ayant deux bases (e_i), (e'_i) de n éléments chacune; si on pose $e'_i = \sum_{j=1}^n a_{ji} e_j$ on dit encore que $P = (a_{ji})$ est la matrice de passage de (e_i) à (e'_i); c’est encore la matrice de l’automorphisme u de E tel que $u(e_i) = e'_i$, par rapport à la base $(e_i)$, et aussi la matrice de $l_E$ prise par rapport aux bases $(e'_i)$ et $(e_i)$ dans cet ordre. Les résultats précédents subsistent alors avec les seules modifications suivantes : les formules (33 D) à (36D) sont respectivement remplacées par

(33 G) $$ ^tM'(u) = ^tP . ^tM(u) . ^tQ^{-1} $$
(34 G) $$ ^tM'(u) = ^tP . ^tM(u) . ^tP^{-1} $$
(35 G) $$ ^tM(x) = ^tM'(x) . ^tP. $$
(36 G) $$ x_i = \sum_{j=1}^n x_j' a_{ij} \quad (1 \leq i \leq n). $$

#### Remarque 2 {#alg-ii-s10-n8-rem-2 .statement}

Sous les hypothèses de II, p. 152, prop. 4, considérons un élément $x^* \in \mathbf{E}^*$; comme la matrice de passage de $(e_i^*)$ à $(e_{i'}^*)$ est $^tP^{-1}$ (II, p, 153, prop. 5) on a, pour les matrices $M(x^*)$ et $M'(x^*)$ de $x^*$ par rapport à ces deux bases respectivement,
$$
^tM(x^*) = ^tM'(x^*) . P^{-1}
$$
ou encore
(37 D) $$ ^tM'(x^*) = ^tM(x^*) . P $$
ce qui est équivalent au système d’équations
(38 D) $$ x_{i'}^* = \sum_{j=1}^n x_j^* a_{ji} \quad (1 \leq i \leq n) $$
pour les éléments $(x_i^*)$ et $(x_{i'}^*)$ des matrices $M(x^*)$ et $M'(x^*)$. Les formules correspondantes pour un A-module à gauche E sont
(37 G) $$ M'(x^*) = ^tP . M(x^*) $$
(38 G) $$ x_{i'}^* = \sum_{j=1}^n a_{ji} x_j^* \quad (1 \leq i \leq n). $$

#### Remarque 3 {#alg-ii-s10-n8-rem-3 .statement}

Soient A, B deux anneaux, $\sigma : A \to B$ un homomorphisme de A dans B, E un A-module à droite (resp. à gauche), $(e_i), (e_i')$ deux bases de $n$ éléments de E, F un B-module à droite (resp. à gauche), $(f_j), (f_j')$ deux bases de $m$ éléments de F, $P$ (resp. $Q$) la matrice de passage de $(e_i)$ à $(e_i')$ (resp. de $(f_j)$ à $(f_j')$).

Pour toute application semi-linéaire $u : E \to F$, relative à $\sigma$, soient $M(u)$ la matrice de $u$ rapport à $(e_i)$ et $(f_j)$, $M'(u)$ sa matrice par rapport à $(e_i')$ et $(f_j')$. Alors on a
(39 D) $$ M'(u) = Q^{-1} M(u) \sigma(P) $$
(resp.
(39 G) $$ ^tM'(u) = \sigma(^tP) . ^tM(u) . ^tQ^{-1}). $$

La démonstration est la même que pour (33 D) et (33 G), en utilisant cette fois les formules (27 D) et (27 G) (II, p. 148).

### 9. Matrices équivalentes; matrices semblables

#### Définition 5 {#alg-ii-s10-def-5 .statement}

On dit que deux matrices $X, X'$ à $m$ lignes et $n$ colonnes sur un anneau $\mathbf{A}$ sont équivalentes s’il existe une matrice carrée inversible $P$ d’ordre $m$ et une matrice carrée inversible $Q$ d’ordre $n$ telles que

$$
X' = PXQ.
$$

Il est clair que la relation « $X$ et $X'$ sont équivalentes » est bien une relation d’équivalence (E, II, p. 40) dans l’ensemble $\mathbf{A}^{mn}$ des matrices de type $(m, n)$ sur $\mathbf{A}$, ce qui justifie la terminologie.

Avec cette définition, la prop. 6 de II, p. 153 implique que lorsqu’on change de bases dans deux $\mathbf{A}$-modules à droite $\mathbf{E}, \mathbf{F}$ (ayant des bases finies), la matrice d’une application linéaire $u : \mathbf{E} \to \mathbf{F}$, par rapport aux nouvelles bases, est équivalente à la matrice de $u$ par rapport aux anciennes bases.

Réciproquement, si on a la relation (40) et si $u : \mathbf{A}_d^n \to \mathbf{A}_d^m$ est l’application linéaire dont la matrice est $X$ par rapport aux bases canoniques $(e_i)$ et $(f_j)$ respectives de $\mathbf{A}_d^n$ et $\mathbf{A}_d^m$, alors $X'$ est la matrice de $u$ par rapport aux bases $(e'_i)$ et $(f'_j)$ telles que $Q$ soit la matrice de passage de $(e_i)$ à $(e'_i)$ et $P^{-1}$ la matrice de passage de $(f_j)$ à $(f'_j)$.

Exemples de matrices équivalentes. — 1) On dit que deux matrices $X = (x_{ij})$ et $X' = (x'_{ij})$ à $m$ lignes et $n$ colonnes « ne diffèrent que par l’ordre des lignes » s’il existe une permutation $\sigma$ de l’intervalle $\{1, m\}$ de $\mathbf{N}$, telle que l’on ait, pour tout couple d’indices $(i, j)$, $x'_{ij} = x_{\sigma(i), j}$ (on dit encore que $X'$ s’obtient en effectuant la permutation $\sigma^{-1}$ sur les lignes de $X$). Les matrices $X$ et $X'$ sont alors équivalentes, car on a $X' = PX$, où $P$ est la matrice de la permutation $\sigma^{-1}$ (cf. II, p. 151, Exemple II).

On dit de même que $X$ et $X'$ ne diffèrent que par l’ordre des colonnes s’il existe une permutation $\tau$ de $\{1, n\}$ telle que $x'_{ij} = x_{i, \tau(j)}$ pour tout couple d’indices ; $X$ et $X'$ sont encore équivalentes, car on a $X' = XQ$, où $Q$ est la matrice de la permutation $\tau$.

On notera qu’avec les notations précédentes, $P$ est la matrice de passage d’une base $(f_i)_{1 \leq j \leq n}$ à la base $(f_{\sigma^{-1}(j)})_{1 \leq j \leq m}$ et $Q$ la matrice de passage d’une base $(e_i)_{1 \leq i \leq n}$ à la base $(e_{\tau(i)})_{1 \leq i \leq n}$.

2) Soient $j, k$ deux éléments distincts de $\{1, n\}$ et soit $a \in \mathbf{A}$.

Supposons que pour $1 \leq i \leq m$, on ait $x'_{ij} = x_{ij} + x_{ik}a$ et $x'_{il} = x_{il}$ pour $l \neq j$; on dit que $X'$ se déduit de $X$ en ajoutant à la colonne d’indice $j$ de $X$ la colonne d’indice $k$ multipliée à droite par $a$. Dans ce cas $X$ et $X'$ sont encore équivalentes : en effet, si $Q = I_n + aE_{kj}$ (matrice triangulaire inversible, comme on l’a vu dans II, p. 152), on a $X' = XQ$.

De même, soient $h, i$ deux éléments distincts de $\{1, m\}$, $a$ un élément de $\mathbf{A}$; si $X'$ se déduit de $X$ en ajoutant à la ligne d’indice $i$ de $X$ la ligne d’indice $h$ multipliée à gauche par $a$, $X$ et $X'$ sont équivalentes, car on a $X' = PX$, avec $P = I_m + aE_{ih}$.

3) Enfin, si, pour un indice donné $j$, on a $x'_{ij} = x_{ij}c$ pour $1 \leq i \leq m$, où $c \in \mathbf{A}$ est inversible, et si $x'_{il} = x_{il}$ pour $1 \leq i \leq m$ et $l \neq j$, $X$ et $X'$ sont encore équivalentes ; en effet, on a $X' = XQ$, où $Q$ est la matrice $\operatorname{diag}(a_k)$ avec $a_j = c$, $a_k = 1$ pour $k \neq j$. On dit alors que $X'$ se déduit de $X$ en multipliant à droite par $c$ la colonne d’indice $j$ de $X$.

De même, si $X'$ se déduit de $X$ en multipliant à gauche la ligne d’indice $i$ de $X$ par un élément inversible $c \in \mathbf{A}$, $X'$ et $X$ sont équivalentes, car $X' = PX$ où $P$ est la matrice $\operatorname{diag}(b_h)$ avec $b_i = c$, $b_h = 1$ pour $h \neq i$.

#### Définition 6 {#alg-ii-s10-def-6 .statement}

On dit que deux matrices carrées $X, X'$ d’ordre $n$ sur un anneau $\mathbf{A}$ sont semblables s’il existe une matrice carrée inversible $P$ d’ordre $n$ telle que

$$(41)$$
$$
X' = PXP^{-1}.
$$

Il est clair que la relation « $X$ et $X'$ sont semblables » est une *relation d’équivalence* dans $\mathbf{M}_n(\mathbf{A})$, signifiant que $X$ et $X'$ sont transformées l’une de l’autre par un *automorphisme intérieur* de cet anneau.

Avec cette définition, le cor. 1 de II, p. 153 implique que lorsqu’on change de base dans un $\mathbf{A}$-module $E$ (ayant une base finie), la matrice d’un endomorphisme $u$ de $E$ par rapport à la nouvelle base est *semblable* à la matrice de $u$ par rapport à l’ancienne base.

#### Remarque 1 {#alg-ii-s10-n9-rem-1 .statement}

Deux matrices carrées qui ne diffèrent que par l’ordre des lignes (ou l’ordre des colonnes) sont équivalentes, mais *non semblables* en général. On obtient une matrice semblable à une matrice carrée $X = (x_{ij})$ en effectuant *la même permutation* $\sigma^{-1}$ sur les lignes et les colonnes, c’est-à-dire en considérant la matrice $X' = (x'_{ij})$, où $x'_{ij} = x_{\sigma(i), \sigma(j)}$ pour tout couple d’indices ; en effet, si $X$ est la matrice d’un endomorphisme $u$ de $A^n_d$ par rapport à une base $(e_i)_{1 \leq i \leq n}$, $X'$ est la matrice de $u$ par rapport à la base $(e_{\sigma(i)})_{1 \leq i \leq n}$.

#### Remarque 2 {#alg-ii-s10-n9-rem-2 .statement}

Soient $X$ et $X'$ deux matrices carrées d’ordre $n$, qui s’écrivent sous forme de matrices diagonales de matrices carrées (II, p. 152, *Exemple IV*) :

$$
X = \begin{pmatrix}
X_1 & 0 & \cdots & 0 \\
0 & X_2 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X_p
\end{pmatrix}
\qquad
X' = \begin{pmatrix}
X'_1 & 0 & \cdots & 0 \\
0 & X'_2 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X'_p
\end{pmatrix}
$$

correspondant à la *même* partition de l’ensemble d’indices $\{1, n\}$ pour $X$ et $X'$. Si, pour $1 \leq i \leq p$, $X_i$ et $X'_i$ sont équivalentes (resp. semblables), alors $X$ et $X'$ sont équivalentes (resp. semblables) : en effet, si $X'_i = P_i X_i Q_i$ pour $1 \leq i \leq p$, on a $X' = PXQ$ avec

$$
P = \begin{pmatrix}
P_1 & 0 & \cdots & 0 \\
0 & P_2 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & P_p
\end{pmatrix}
\qquad
Q = \begin{pmatrix}
Q_1 & 0 & \cdots & 0 \\
0 & Q_2 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & Q_p
\end{pmatrix}
$$

comme il résulte du calcul du produit « par blocs » (II, p. 147). En outre, si $Q_i = P_i^{-1}$ pour tout $i$, on a $Q = P^{-1}$.

### 10. Produit tensoriel de matrices sur un anneau commutatif

Soient $C$ un anneau *commutatif*, $E, F, U, V$ quatre $C$-modules, $\varphi : E \to U$, $\psi : F \to V$ deux applications $C$-linéaires. Supposons que $E, F, U, V$ aient respectivement des bases finies $(e_\lambda)_{\lambda \in L}, (f_\mu)_{\mu \in M}, (u_\rho)_{\rho \in R}, (v_\sigma)_{\sigma \in S}$; soient $A = (a_{\rho \lambda})$ la matrice de $\varphi$ par rapport à $(e_\lambda)$ et $(u_\rho)$, $B = (b_{\sigma \mu})$ celle de $\psi$ par rapport à $(f_\mu)$ et $(v_\sigma)$. Pour tout couple $(\lambda, \mu) \in L \times M = N$, posons $g_{\lambda \mu} = e_\lambda \otimes f_\mu$; pour tout couple $(\rho, \sigma) \in R \times S = T$, posons $w_{\rho \sigma} = u_\rho \otimes v_\sigma$; les $g_{\lambda \mu}$ forment alors une base de $E \otimes F$ et les $w_{\rho \sigma}$ une base de $U \otimes V$ (II, p. 62, cor. 2). On appelle produit tensoriel de $A$ par $B$ et on note $A \otimes B$ la matrice $X = (x_{\tau v})_{(\tau, v) \in T \times N}$ dont les éléments sont donnés par

(42)
$$
x_{(\rho, \sigma), (\lambda, \mu)} = a_{\rho \lambda} b_{\sigma \mu}.
$$

Alors $A \otimes B$ est la matrice de $\varphi \otimes \psi$ par rapport aux bases $(g_{\lambda \mu})$ et $(w_{\rho \sigma})$. En effet, on a par définition (II, p. 52, formule (3))

$$
(\varphi \otimes \psi)(g_{\lambda \mu}) = (\varphi \otimes \psi)(e_{\lambda} \otimes f_{\mu}) = \varphi(e_{\lambda}) \otimes \psi(f_{\mu})
$$
$$
= \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} (u_{\rho} \otimes v_{\sigma}) = \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} w_{\rho \sigma}.
$$

La définition (42) des éléments de $A \otimes B$ montre que cette matrice correspond biunivoquement à la matrice de matrices $(a_{\rho \lambda} B)_{(\rho, \lambda) \in \mathbf{R} \times \mathbf{L}}$ et aussi à la matrice de matrices $(A b_{\sigma \mu})_{(\sigma, \mu) \in \mathbf{S} \times \mathbf{M}}$ (II, p. 147).

Le fait que $(\varphi, \psi) \mapsto \varphi \otimes \psi$ est une application $\mathbf{C}$-bilinéaire et la formule (9) de II, p. 56 se traduisent par les identités

(43)
$$
\begin{cases}
A \otimes (B_1 + B_2) = A \otimes B_1 + A \otimes B_2 \\
(A_1 + A_2) \otimes B = A_1 \otimes B + A_2 \otimes B
\end{cases}
$$

(44)
$$(cA) \otimes B = A \otimes (cB) = c(A \otimes B) \quad \text{pour } c \in \mathbf{C}$$

(45)
$$(A_1 \otimes B_1)(A_2 \otimes B_2) = (A_1 A_2) \otimes (B_1 B_2)$$

lorsque les opérations écrites sont définies. La transposée d’un produit tensoriel de matrices est donnée par

(46)
$$^t(A \otimes B) = (^tA) \otimes (^tB).$$

Si $A$ et $B$ sont des matrices carrées inversibles sur $\mathbf{C}$, $A \otimes B$ est inversible et l’on a

(47)
$$(A \otimes B)^{-1} = (A^{-1}) \otimes (B^{-1}).$$

Soient $(e'_\lambda)_{\lambda \in L}$ une seconde base de $E$, $(f'_\mu)_{\mu \in M}$ une seconde base de $F$; si $P$ est la matrice de passage de la base $(e_\lambda)$ à la base $(e'_\lambda)$, $Q$ la matrice de passage de la base $(f_\mu)$ à la base $(f'_\mu)$, la matrice de passage de la base $(e_\lambda \otimes f_\mu)$ à la base $(e'_\lambda \otimes f'_\mu)$ est $P \otimes Q$. Si $A'$ est équivalente (resp. semblable) à $A$, $B'$ équivalente (resp. semblable) à $B$, alors $A' \otimes B'$ est équivalente (resp. semblable) à $A \otimes B$.

On généralise de façon évidente la définition du produit tensoriel de matrices à un nombre fini quelconque de matrices sur $\mathbf{C}$; on a en particulier la formule d’associativité

(48)
$$\left( \bigotimes_{i \in I_1} X_i \right) \otimes \left( \bigotimes_{i \in I_2} X_i \right) = \bigotimes_{i \in I} X_i$$

pour toute partition $(I_1, I_2)$ de l’ensemble fini d’indices $I$.

### 11. Trace d’une matrice

Soit $\mathbf{C}$ un anneau *commutatif*; pour toute matrice carrée $X = (x_{ij})$ sur $\mathbf{C}$, correspondant à l’ensemble d’indices fini $\mathbf{I}$, on appelle *trace* de $X$ l’élément

$$
\operatorname{Tr}(X) = \sum_{i \in \mathbf{I}} x_{ii}.
$$

Soit $E$ un $\mathbf{C}$-module admettant une base finie $(e_i)_{i \in \mathbf{I}}$; pour tout endomorphisme $u$ de $E$, on a

$$
\operatorname{Tr}(u) = \operatorname{Tr}(M(u))
$$

$M(u)$ étant la matrice de $u$ par rapport à la base $(e_i)$; cela résulte aussitôt de II, p. 78, formule (17) lorsqu’on applique cette formule à l’endomorphisme $x \mapsto \langle x, e_i^* \rangle e_j$ (où $(e_i^*)$ est la base duale de $(e_i)$); on passe de là au cas général par linéarité. La formule (49) montre que l’on a

$$
\operatorname{Tr}(u) = \sum_i \langle u(e_i), e_i^* \rangle
$$

pour toute base $(e_i)$ de $E$ (cf. II, p. 78, formule (17)).

Si $X$ est une matrice de type $(m, n)$ sur $\mathbf{C}$, $Y$ une matrice de type $(n, m)$ sur $\mathbf{C}$, on a

$$
\operatorname{Tr}(XY) = \operatorname{Tr}(YX)
$$

comme il résulte de ce qui précède et de la prop. 3 de II, p. 78; on peut aussi obtenir (52) directement, car si $X = (x_{ij}),\ Y = (y_{ji})\ (1 \leq i \leq m,\ 1 \leq j \leq n)$, on a

$$
\operatorname{Tr}(XY) = \sum_{i,j} x_{ij} y_{ji}
$$

en vertu de (49). Cette dernière formule prouve en outre:

#### Proposition 7 {#alg-ii-s10-prop-7 .statement}

*Soit $\mathbf{C}$ un anneau commutatif, et pour toute matrice $P \in \mathbf{M}_n(\mathbf{C})$, soit $f_P$ la forme linéaire $X \mapsto \operatorname{Tr}(PX)$ sur $\mathbf{M}_n(\mathbf{C})$; l’application $P \mapsto f_P$ est une bijection $\mathbf{C}\text{-linéaire de } \mathbf{M}_n(\mathbf{C})$ sur son dual.*

#### Proposition 8 {#alg-ii-s10-prop-8 .statement}

*Si $g$ est une forme linéaire sur le $\mathbf{C}$-module $\mathbf{M}_n(\mathbf{C})$ telle que $g(XY) = g(YX)$ quelles que soient les matrices $X, Y$ de $\mathbf{M}_n(\mathbf{C})$, il existe un scalaire $c \in \mathbf{C}$ et un seul tel que $g(X) = c \cdot \operatorname{Tr}(X)$ pour toute matrice $X \in \mathbf{M}_n(\mathbf{C})$.

La proposition étant triviale pour $n = 1$, on peut se borner au cas où $n \geq 2$. En prenant $X = E_{ij},\ Y = E_{jk}$ avec $i \neq k$, il vient $g(E_{ik}) = 0$; prenant ensuite $X = E_{ij},\ Y = E_{ji}$ on trouve $g(E_{ii}) = g(E_{jj})$; la proposition en résulte aussitôt, les $E_{ij}$ formant une base de $\mathbf{M}_n(\mathbf{C})$.*

### 12. Matrices sur un corps

Les matrices finies à $m$ lignes et $n$ colonnes sur un corps $K$ correspondent biunivoquement aux applications linéaires de l’espace vectoriel à droite $E = K^n$ dans l’espace vectoriel à droite $F = K_d^m$, lorsqu’on prend les matrices de ces applications par rapport aux bases canoniques de $E$ et $F$. Par définition, le *rang* d’une telle matrice $X$ est le rang de l’application linéaire $u : E \to F$ qui lui correspond; comme ce nombre est par définition la dimension du sous-espace $u(E)$ de $F$, il revient au même (en identifiant les colonnes de $X$ aux images par $u$ de la base canonique de $E$) de donner la définition suivante:

#### Définition 7 {#alg-ii-s10-def-7 .statement}

*Étant donnée une matrice $X$ à $m$ lignes et $n$ colonnes sur un corps $K$, on appelle rang de $X$ par rapport à $K$, et on note $\mathrm{rg}(X)$, la dimension du sous-espace de $K_d^m$ engendré par les $n$ colonnes de $X$.*

On peut dire aussi que le rang de $X$ est le *nombre maximum de colonnes de $X$ linéairement indépendantes* (en tant qu’éléments de $K_d^m$). On a évidemment $\mathrm{rg}(X) \leq \inf(m, n)$; pour toute sous-matrice $Y$ de $X$, on a $\mathrm{rg}(Y) \leq \mathrm{rg}(X)$.

Si $E$ et $F$ sont deux espaces vectoriels de dimension finie sur $K$, $u$ une application linéaire de $E$ dans $F$, le rang de la matrice $M(u)$ par rapport à deux bases quelconques est égal au rang de $u$.

#### Proposition 9 {#alg-ii-s10-prop-9 .statement}

*Si les éléments d’une matrice $X$ à $m$ lignes et $n$ colonnes appartiennent à un sous-corps $K_0$ d’un corps $K$, le rang de $X$ par rapport à $K_0$ est égal au rang de $X$ par rapport à $K$.*

En effet, soit $F_0$ le $K_0$-espace vectoriel à droite engendré par la base canonique du $K$-espace vectoriel à droite $F = K_d^m$; par hypothèse les colonnes de $X$ appartiennent à $F_0$. Soit $V_0$ (resp. $V$) le sous-$K_0$-espace vectoriel de $F_0$ (resp. le sous-$K$-espace vectoriel de $F$) engendré par ces colonnes. On a $V = V_0 \otimes_{K_0} K$ (II, p. 120, prop. 2), donc $\dim_K V = \dim_{K_0} V_0$.

#### Proposition 10 {#alg-ii-s10-prop-10 .statement}

*Le rang d’une matrice $X$ sur un corps $K$ est égal au rang de sa transposée ${}^t X$ sur le corps opposé $K^o$.*

En effet, avec les notations introduites avant la déf. 7, le rang de $u$ est égal à celui de ${}^t u$ (II, p. 104, prop. 10) et la proposition résulte donc de II, p. 145, prop. 3.

On voit donc que le rang de $X$ peut aussi être défini comme le *nombre maximum de lignes de $X$ linéairement indépendantes* (quand on les considère comme des éléments du $K$-espace vectoriel à gauche $K_s^n$).

Les matrices carrées d’ordre $n$ sur un corps $K$ correspondent biunivoquement aux endomorphismes de $E = K_d^n$ et forment un anneau isomorphe à l’anneau $\mathrm{End}_K(E)$ (II, p. 150); aux automorphismes de $E$ correspondent les matrices carrées inversibles.

#### Proposition 11 {#alg-ii-s10-prop-11 .statement}

*Soit $X$ une matrice carrée d’ordre $n$ sur un corps $K$. Les propriétés suivantes sont équivalentes:
a) $X$ est inversible dans $\mathbf{M}_n(K)$.
b) $X$ est inversible à droite dans $\mathbf{M}_n(K)$.*

c) $X$ est inversible à gauche dans $\mathbf{M}_n(\mathbf{K})$.
d) $X$ est de rang $n$.
Cela ne fait que traduire II, p. 101, corollaire.

#### Proposition 12 {#alg-ii-s10-prop-12 .statement}

Pour qu’un système de $m$ équations linéaires à $n$ inconnues

$$
\sum_{j=1}^n a_{ij} x_j = b_i \qquad (1 \leq i \leq m)
$$

sur un corps $\mathbf{K}$, ait au moins une solution, il faut et il suffit que la matrice $A = (a_{ij})$ du système et la matrice $B$ obtenue en bordant $A$ par une $(n+1)$-ème colonne égale à $(b_i)$, soient des matrices de même rang.

On a vu en effet (II, p. 146) que l’existence d’une solution de (54) équivaut au fait que la colonne $(b_i)$ est combinaison linéaire des colonnes de $A$, et la proposition résulte donc de II, p. 99, cor. 4.

On notera que la condition de la prop. 12 est toujours remplie lorsque $m = n$ et que $A$ est inversible, c’est-à-dire de rang $n$ (prop. 11). Si $x$ et $b$ désignent alors les matrices à une colonne $(x_i)$ et $(b_i)$ respectivement, le système (54) est équivalent à $A.x = b$, et son unique solution est $x = A^{-1}.b$.

### 13. Équivalence des matrices sur un corps

#### Proposition 13 {#alg-ii-s10-prop-13 .statement}

Soient $E, F$ deux espaces vectoriels sur un corps $\mathbf{K}$, de dimensions finies. Si $u : E \to F$ est une application linéaire de rang $r$, il existe des bases de $E$ et $F$ telles que, par rapport à ces bases, on ait

$$
M(u) = \begin{pmatrix} I_r & 0 \\ 0 & 0 \end{pmatrix}.
$$

Toute matrice de type $(m, n)$ sur $\mathbf{K}$ et de rang $r$ est équivalente à une matrice de la forme (55).

La seconde assertion est trivialement équivalente à la première. Pour démontrer celle-ci, soient $\dim E = n$, $\dim F = m$. Le noyau $N = \overline{u}(0)$ est de dimension $n - r$ (II, p. 101, formule (11)); soient $V$ un supplémentaire de $N$ dans $E$, $(e_i)_{1 \leq i \leq n}$ une base de $E$ telle que $(e_i)_{1 \leq i \leq r}$ soit une base de $V$ et $(e_i)_{r+1 \leq i \leq n}$ une base de $N$. Alors les $u(e_j)$ ($1 \leq j \leq r$) forment une base de $u(E)$; il existe donc une base $(f_j)_{1 \leq j \leq m}$ de $F$ telle que $f_j = u(e_j)$ pour $1 \leq j \leq r$ (II, p. 95, th. 2), et il est clair que par rapport aux bases $(e_i)$ et $(f_j)$, la matrice $M(u)$ est donnée par (55).

#### Corollaire {#alg-ii-s10-n13-cor-1 .statement}

Pour que deux matrices sur un corps, de type $(m, n)$, soient équivalentes, il faut et il suffit qu’elles aient même rang.

Nous allons retrouver la prop. 13 par un autre procédé plus explicite. Pour tout anneau A, tout $\lambda \in A$, tout entier $m > 1$ et tout couple d’entiers distincts $i, j$ dans $\{1, m\}$, nous poserons

$$
B_{ij}(\lambda) = I_m + \lambda E_{ij}
$$

matrice inversible d’ordre $m$ d’après ce qu’on a vu dans II, p. 152.

#### Lemme 1 {#alg-ii-s10-lem-1 .statement}

*Soit $X = (\xi_{ij})$ une matrice de type $(m, n)$ sur un anneau A. Supposons que $m \geq 2$ et qu’il existe un élément $\xi_{i1}$ de la première colonne de $X$ qui soit inversible dans A. Alors il existe deux matrices carrées inversibles $P \in \mathbf{M}_m(A)$, $Q \in \mathbf{M}_n(A)$ et une matrice Y de type $(m - 1, n - 1)$ sur A, telles que $P$ (resp. $Q$) soit produit de matrices de la forme $B_{ij}(\lambda)$ d’ordre $m$ (resp. $n$), et que l’on ait*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 \\
0 & & & \\
\vdots & & Y & \\
0 & & &
\end{pmatrix}.
$$

En effet, la matrice $B_{ij}(\lambda)X$ s’obtient en ajoutant à la ligne d’indice $i$ de $X$ la ligne d’indice $j$ multipliée à gauche par $\lambda$ (II, p. 155, *Exemple 2*); si $\xi_{i1}$ est inversible, il existe donc $\lambda \in A$ tel que pour la matrice $X' = B_{1i}(\lambda)X = (\xi'_{kl})$ on ait $\xi'_{11} = 1$; multipliant à gauche $X'$ par des matrices $B_{k1}(\mu_k)$ d’ordre $m$ convenablement choisies (pour $2 \leq k \leq m$), on obtient une matrice $X'' = (\xi''_{kl})$ telle que $\xi''_{11} = 1,\ \xi''_{k1} = 0$ pour $k \neq 1$. On multiplie ensuite *à droite* la matrice obtenue successivement par des matrices $B_{1j}(\nu_j)$ d’ordre $n$ convenables $(2 \leq j \leq n)$, et on obtient bien une matrice de la forme (57).

#### Proposition 14 {#alg-ii-s10-prop-14 .statement}

*Soit $X$ une matrice de type $(m, n)$ sur un corps K. Si $X$ est de rang r, il existe deux matrices carrées inversibles $P \in \mathbf{M}_m(K)$, $Q \in \mathbf{M}_n(K)$ telles que $P$ (resp. $Q$) soit produit de matrices d’ordre $m$ (resp. $n$) de la forme $B_{ij}(\lambda)$ et que l’on ait*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \delta_r & 0 & \cdots & 0 \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0
\end{pmatrix}
$$

*(matrice $(\eta_{ij})$ dont tous les termes sont nuls sauf les $\eta_{ii}$ pour $1 \leq i \leq r$, avec $\eta_{ii} = 1$* pour $1 \leq i \leq r - 1, \eta_{rr} = \delta_r \neq 0$. Si $r \neq m$ ou $r \neq n$, on peut en outre supposer que $\delta_r = 1$.

La proposition est évidente si $X = 0$; supposons donc $X \neq 0$. Si $m = n = 1$ la proposition est évidente (avec $P = I_m, Q = I_n, \delta_1 \neq 0$ arbitraire). Si $n = 1, m \geq 2$, on peut appliquer le lemme 1 (puisque $X \neq 0$), qui donne la forme vouluue (58) avec $r = 1, \delta_r = 1$. Raisonnons par récurrence sur $n > 1$; il existe un élément $\xi_{ij} \neq 0$ dans $X$; si $j = 1$, on peut appliquer le lemme 1 et se ramener au cas où $X$ a la forme (57). L’hypothèse de récurrence s’applique alors à $Y$ et il y a donc des matrices inversibles $P' \in \mathbf{M}_{m-1}(\mathbf{K}), Q' \in \mathbf{M}_{n-1}(\mathbf{K})$ produits de matrices de la forme $B_{ij}(\lambda)$ d’ordre $m - 1$ (resp. $n - 1$), telles que $P'YQ'$ soit de la forme (58). Or, si $B_{ij}(\lambda)$ appartient par exemple à $\mathbf{M}_{m-1}(\mathbf{K})$, on a $\begin{pmatrix} 1 & 0 \\ 0 & B_{ij}(\lambda) \end{pmatrix} = B_{i+1, j+1}(\lambda)$; la formule (58) résulte alors de la formule du produit par blocs en posant $P = \begin{pmatrix} 1 & 0 \\ 0 & P' \end{pmatrix}$ et $Q = \begin{pmatrix} 1 & 0 \\ 0 & Q' \end{pmatrix}$. Si enfin on avait $j \neq 1$, il suffirait de considérer la matrice $XB_{j1}(1)$ pour être ramené au cas précédent.

La prop. 14 redonne aussitôt la prop. 13.

#### Corollaire 1 {#alg-ii-s10-prop-14-cor-1 .statement}

*Si $X$ est une matrice carrée inversible d’ordre $n$ sur un corps $\mathbf{K}$, il existe trois matrices inversibles $P, Q, D$ d’ordre $n$ telles que $X = PDQ$, $P$ et $Q$ étant produits de matrices de la forme $B_{ij}(\lambda)$, et $D$ une matrice diagonale de la forme $D = \operatorname{diag}(1, 1, \ldots, 1, \delta)$ avec $\delta \neq 0$ (cf. II, p. 207, exerc. 13).

#### Corollaire 2 {#alg-ii-s10-prop-14-cor-2 .statement}

*Pour tout corps $\mathbf{K}$, le groupe de matrices inversibles $\mathbf{GL}(n, \mathbf{K})$ est engendré par les matrices de permutation (II, p. 151, Exemple 2), les matrices diagonales $\operatorname{diag}(a, 1, \ldots, 1)$ ($a \neq 0$ dans $\mathbf{K}$) et les matrices $B_{12}(\lambda)$ ($\lambda \in \mathbf{K}$).

On a vu (II, p. 155) que le produit à droite (resp. à gauche) d’une matrice par la matrice d’une transposition convenable échange deux colonnes (resp. deux lignes) quelconques. On en conclut que la matrice $\operatorname{diag}(1, \ldots, 1, a)$ est égale au produit de $\operatorname{diag}(a, 1, \ldots, 1)$ et de matrices de permutation, et que toute matrice $B_{ij}(\lambda)$ est égale au produit de $B_{12}(\lambda)$ et de matrices de permutation, d’où le corollaire.

*Remarques. —* 1) Au chap. III, on verra que si $m = n = r$ et si $\mathbf{K}$ est *commutatif*, alors, pour tous les choix de $P$ et $Q$ satisfaisant aux conditions de la prop. 14, l’élément $\delta_r$ est toujours le même et est égal au *déterminant* de $X$ (III, p. 101).

2) Le raisonnement de la prop. 14, légèrement modifié, montre qu’il y a une matrice de permutation $R$ telle que l’on ait (avec les mêmes conditions pour $P$)

$$
PXR = \begin{pmatrix} I_r & N \\ 0 & 0 \end{pmatrix}
$$

si l’on n’a pas $m = n = r$, et

$$
PXR = \operatorname{diag}(1, \ldots, 1, \delta)
$$

dans le cas contraire. On observera aussi que la méthode de démonstration donne une détermination explicite des matrices $P, Q, R$ lorsque $X$ est donnée explicitement.

## EXERCICES {#alg-ii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
