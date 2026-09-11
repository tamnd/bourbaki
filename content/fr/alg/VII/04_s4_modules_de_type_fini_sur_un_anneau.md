---
book: alg
book_title: Algebra
chapter: VII
chapter_title: Modules sur les anneaux principaux
section: 4
section_title: MODULES DE TYPE FINI SUR UN ANNEAU PRINCIPAL
lang: fr
source: alg-iv-vii-fr
book_pages: A VII.15-A VII.27, A VII.60-A VII.66
pdf_pages: 0348-0360, 0393-0399
extraction: ocr
subsections:
    - "no": 1
      title: Sommes directes finies de modules monogènes
      page: 15
      pdf_page: 348
    - "no": 2
      title: Contenu d’un élément d’un module libre
      page: 16
      pdf_page: 349
    - "no": 3
      title: Facteurs invariants d’un sous-module
      page: 17
      pdf_page: 350
    - "no": 4
      title: Structure des modules de type fini
      page: 19
      pdf_page: 352
    - "no": 5
      title: Calcul des facteurs invariants
      page: 20
      pdf_page: 353
    - "no": 6
      title: Applications linéaires de modules libres, et matrices sur un anneau principal
      page: 21
      pdf_page: 354
    - "no": 7
      title: Groupes commutatifs de type fini
      page: 22
      pdf_page: 355
    - "no": 8
      title: Modules indécomposables. Diviseurs élémentaires
      page: 23
      pdf_page: 356
    - "no": 9
      title: Dualité des modules de longueur finie sur un anneau principal
      page: 25
      pdf_page: 358
statements: 41
exercises: 25
content_sha256: 87df1f6594332ddfc8ec38a4fe31e67f6610f4eb582f81b52c94da4aaa95c4b5
---

## § 4. MODULES DE TYPE FINI SUR UN ANNEAU PRINCIPAL

### 1. Sommes directes finies de modules monogènes

Soit A un anneau commutatif. Rappelons (II, p. 29, prop. 22) qu’un A-module monogène est isomorphe à un module quotient $A/\alpha$, où $\alpha$ est un idéal de A. Nous verrons plus loin dans ce paragraphe (n° 4) que tout module de type fini sur un anneau principal est somme directe d’un nombre fini de modules monogènes.

#### Proposition 1 {#alg-vii-s4-prop-1 .statement}

Soit E un module sur un anneau commutatif A ; supposons que E soit somme directe de n modules monogènes $A/\alpha_k$ ($1 \leq k \leq n$), les $\alpha_k$ étant des idéaux de A ; alors, pour tout entier $p > 0$, le A-module $\bigwedge^p E$ est isomorphe à la somme directe des modules $A/\alpha_H$, $\alpha_H$ désignant, pour toute partie $H = \{k_1, ..., k_p\}$ à p éléments de $\{1, n\}$, l’idéal $\sum_{j=1}^p \alpha_{k_j}$ de A.

Soit $x_k$ le générateur de $A/\alpha_k$ image canonique de l’élément unité de A, de sorte que E est somme directe des $Ax_i$ ($1 \leq i \leq n$). On sait alors (III, p. 84, prop. 10) que l’algèbre extérieure $\Lambda E$, en tant que A-module, est isomorphe au produit tensoriel $\bigotimes_{i=1}^n (\Lambda (Ax_i))$. Or $\Lambda (Ax_i)$ se réduit à la somme directe $A \oplus Ax_i$, tout produit extérieur de deux éléments de $Ax_i$ étant nul, et $\Lambda^p E$ est donc somme directe des modules $M_H = (Ax_{k_1}) \otimes ... \otimes (Ax_{k_p})$, $H = \{k_1, ..., k_p\}$ parcourant l’ensemble des parties à p éléments de $\{1, n\}$ (avec $k_1 < k_2 < ... < k_p$) ; or, on sait que $M_H$ est isomorphe à $A/\alpha_H$ (II, p. 60, cor. 4), ce qui achève la démonstration.

Nous allons maintenant voir que, avec les notations de la prop. 1, si les idéaux $a_k$ forment une suite croissante, ils sont entièrement déterminés par la connaissance du module $E$; de façon plus précise :

#### Proposition 2 {#alg-vii-s4-prop-2 .statement}

*Soient $A$ un anneau commutatif, et $E$ un $A$-module somme directe de $n$ modules monogènes $A/a_k$, les $a_k$ étant tels que $a_1 \subset a_2 \subset \ldots \subset a_n$. Alors, pour $1 \leq p \leq n$, $a_p$ est l’annulateur de $\bigwedge^p E$; si $a_n \neq A$, le module $\bigwedge^p E$ n’est pas réduit à $0$ pour $1 \leq p \leq n$ et on a $\bigwedge^m E = 0$ pour $m > n$.

En effet, avec les notations de la prop. 1, on a $a_H = a_{s(H)}$, $s(H)$ désignant le plus grand élément de la partie $H$. Comme $s(H) \geq p$ pour toute partie $H$ à $p$ éléments, et que $s(H) = p$ pour $H = \{1, 2, \ldots, p\}$, $a_p$ est l’intersection des $a_H$, $H$ parcourant l’ensemble des parties à $p$ éléments de $\{1, n\}$; l’idéal $a_p$ est donc bien, en vertu de la prop. 1, l’annulateur de $\bigwedge^p E$.

#### Corollaire {#alg-vii-s4-n1-cor-1 .statement}

*Les notations étant celles de la prop. 2 avec $a_n \neq A$, si $E$ est aussi isomorphe à la somme directe de $m$ modules monogènes $A/a'_j$ avec $a'_1 \subset \ldots \subset a'_m \neq A$, on a $m = n$ et $a_k = a'_k$ pour $1 \leq k \leq n$* (« unicité des $a_k$ »).

### 2. Contenu d’un élément d’un module libre

Soient $A$ un anneau principal, $L$ un $A$-module libre, et $x$ un élément de $L$. Lorsque $f$ parcourt l’ensemble $L^*$ des formes linéaires sur $L$, les éléments $f(x)$ forment un idéal $c_L(x)$ de $A$, que l’on appelle le *contenu* de $x$ dans $L$. Un élément $c$ de $A$ est appelé un *contenu* de $x$ dans $L$ s’il engendre l’idéal $c_L(x)$; cela revient à dire qu’il existe une forme linéaire $f$ sur $L$ telle que $f(x) = c$ et que $c$ divise $g(x)$ pour toute forme linéaire $g$ sur $L$. Soit $(e_i)_{i \in I}$ une base de $L$; posons $x = \sum a_i e_i$, $a_i \in A$; l’idéal $c_L(x)$ est formé des sommes $\sum a_i b_i$, où $(b_i)$ parcourt l’ensemble $A^I$; il en résulte aussitôt qu’un élément $c$ de $A$ est un contenu de $x$ dans $L$ si et seulement si c’est un pgcd de la famille $(a_i)$ des coordonnées de $x$.

On dit que $x$ est *indivisible* si $c_L(x) = A$, c’est-à-dire si les coordonnées de $x$ par rapport à une base de $L$ sont étrangères dans leur ensemble.

#### Lemme 1 {#alg-vii-s4-lem-1 .statement}

*Soient $L$ un module libre sur un anneau principal $A$ et $x$ un élément de $L$. Les conditions suivantes sont équivalentes :*
(i) $x$ est indivisible ;
(ii) *il existe une forme linéaire $f$ sur $L$ telle que $f(x) = 1$ ;
(iii) $x$ est non nul et le sous-module $Ax$ de $L$ est facteur direct ;
(iv) $x$ fait partie d’une base de $L$.

(i) $\Rightarrow$ (ii) : cela résulte de la définition.
(ii) $\Rightarrow$ (iii) : soit $f$ une forme linéaire sur $L$ telle que $f(x) = 1$; alors $x \neq 0$ et l’application $y \mapsto f(y) x$ est un projecteur de $L$, d’image $Ax$.
(iii) $\Rightarrow$ (iv) : soit $L'$ un supplémentaire de $Ax$ dans $L$, et soit $B'$ une base de $L'$ (VII, p. 14, cor. 2) ; alors $B' \cup \{x\}$ est une base de $L$.
(iv) $\Rightarrow$ (i) : c’est trivial.

#### Remarque 1 {#alg-vii-s4-n2-rem-1 .statement}

Si x est un élément non nul de L et c un contenu de x, il existe un unique élément y de L tel que $x = cy$; on le note $x/c$; c’est un élément indivisible de L.

#### Remarque 2 {#alg-vii-s4-n2-rem-2 .statement}

Le contenu $c_L(x)$ est l’annulateur du module de torsion de $L/Ax$.

Soient L un module libre sur un anneau principal A et M un sous-module de L ; d’après VII, p. 4, lemme 1, la famille des idéaux $c_L(x),\ x \in M$, possède un élément maximal ; si $M \neq \{0\}$, un tel élément maximal est non nul.

#### Proposition 3 {#alg-vii-s4-prop-3 .statement}

Soient L un module libre sur un anneau principal A et M un sous-module non nul de L. Soient x un élément de M tel que $c_L(x)$ soit maximal parmi les contenus des éléments de M, c un contenu de x dans L et f une forme linéaire sur L telle que $f(x) = c$.

a) L est somme directe de $A(x/c)$ et du noyau K de f.
b) M est somme directe de Ax et de $K \cap M$.
c) Pour toute forme linéaire g sur L, on a $g(M) \subset Ac$.

Posons $y = x/c$; il est clair que $Ay \cap K = \{0\}$, puisque $f(y) = 1$. Par ailleurs, pour tout $u \in L$, on a

$$
u = f(u)\ y + (u - f(u)\ y),
$$

avec $f(u)\ y \in Ay$ et $u - f(u)\ y \in K$; cela prouve a). Notons maintenant que pour $u \in M$, on a $f(u) \in Ac$ : en effet, soit $u \in M$, et soit d un pgcd de $f(u)$ et c ; il existe $\lambda, \mu \in A$ avec $d = \lambda f(u) + \mu c = f(\lambda u + \mu x)$; le contenu de l’élément $\lambda u + \mu x$ de M divise donc d ; d’après le caractère maximal de c, cela implique que d est associé à c, donc que $f(u) \in Ac$. Pour tout $u$ dans M, on peut donc écrire

$$
u = (f(u)/c)\ x + (u - (f(u)/c)\ x) \in Ax + (K \cap M),
$$

d’où b). Soit enfin g une forme linéaire sur L ; d’après a), il existe un scalaire $\alpha \in A$ et une forme linéaire h sur K tels que l’on ait $g(u) = \alpha f(u) + h(u - f(u)\ y)$; d’après b), on a donc $g(M) \subset Ac + h(K \cap M)$. Pour prouver c), il suffit donc de démontrer que pour toute forme linéaire h sur K, ou, ce qui revient au même, pour toute forme linéaire h sur L telle que $h(x) = 0$, on a $h(K \cap M) \subset Ac$; or, si $u \in K \cap M$ et si d est un pgcd de $h(u)$ et c, il existe $\lambda, \mu \in A$ avec $d = \lambda h(u) + \mu c$; on a alors $(f + h)(\lambda u + \mu x) = d$, ce qui implique comme ci-dessus $h(u) \in Ac$, d’où c).

### 3. Facteurs invariants d’un sous-module

#### Théorème 1 {#alg-vii-s4-thm-1 .statement}

Soient L un module libre sur un anneau principal A, et M un sous-module de rang fini n de L. Il existe alors une base B de L, n éléments $e_i$ de B, et n éléments non nuls $\alpha_i$ de A ($1 \leq i \leq n$) tels que :
a) les $\alpha_i e_i$ forment une base de M ;
b) $\alpha_i$ divise $\alpha_{i+1}$ pour $1 \leq i \leq n-1$.
De plus le module M' ayant pour base $(e_i)$ et les idéaux principaux $A \alpha_i$ sont déterminés de façon unique par les conditions précédentes ; $M'/M$ est le sous-module de torsion de $L/M$, et est isomorphe à la somme directe des $A$-modules $A/A\alpha_i$; enfin $L/M$ est somme directe de $M'/M$ et d’un module libre isomorphe à $L/M'$.

1) *Existence des $e_i$ et des $\alpha_i$*.

Si $M = \{0\}$, le théorème est trivial. Si $M \neq \{0\}$, il résulte de la prop. 3 qu’il existe un élément $e_1$ de $L$, un élément $\alpha_1$ de $A$, non nuls, et un sous-module $L_1$ de $L$, tels que $L$ soit somme directe de $Ae_1$ et $L_1$, que $M$ soit somme directe de $A\alpha_1e_1$ et du sous-module $M_1 = M \cap L_1$ de $L_1$, et que pour toute forme linéaire $g$ sur $L$, on ait $g(M) \subset A\alpha_1$.

On peut alors procéder par récurrence sur le rang $n$ de $M$. Comme $L_1$ est un module libre (VII, p. 14, cor. 2), et comme $M_1$ est de rang $n - 1$, il existe une base $B_1$ de $L_1$, $n - 1$ éléments $e_2, ..., e_n$ de $B_1$, et des éléments non nuls $\alpha_2, ..., \alpha_n$ de $A$ tels que $(\alpha_2e_2, ..., \alpha_ne_n)$ soit une base de $M_1$, et que $\alpha_i$ divise $\alpha_{i+1}$ pour $2 \leq i \leq n-1$. Si $L'$ est le sous-module de $L_1$ engendré par les éléments de $B_1$ distincts de $e_2, ..., e_n$, $L$ est somme directe de $L'$ et du module $M'$ engendré par $e_1, ..., e_n$; $(e_1, ..., e_n)$ est une base de $M'$, et $(\alpha_1e_1, ..., \alpha_ne_n)$ une base de $M$. Il ne reste plus qu’à montrer que $\alpha_1$ divise $\alpha_2$; or, $A\alpha_2$ est de la forme $g(M_1)$, où $g$ est la forme linéaire sur $L$ définie par $g(e_2) = 1, g(e_i) = 0$ pour $i \neq 2$, et $g(L') = \{0\}$; et l’on a vu ci-dessus que $g(M_1) \subset A\alpha_1$.

2) *Propriétés d’unicité*.

Comme les $\alpha_i$ sont différents de 0, $M'$ est l’ensemble des $x \in L$ pour lesquels il existe $\beta \neq 0$ dans $A$ tel que $\beta x \in M$; autrement dit $M'/M$ est le sous-module de torsion de $L/M$. Ceci détermine $M'$ de façon unique.

Il est clair que $M'/M$ est isomorphe à la somme directe des $n$ modules monogènes $A/A\alpha_i$ (II, p. 14, formule (26)). Soit $r$ le nombre des idéaux $A\alpha_i$ qui sont distincts de $A$ : les $n - r$ premiers idéaux $A\alpha_i$ sont ainsi égaux à $A$, les $r$ derniers en étant distincts. Alors $M'/M$ est aussi isomorphe à la somme directe des modules $A/A\alpha_n, ..., A/A\alpha_{n-r+1}$, où $A\alpha_n \subset A\alpha_{n-1} \subset ... \subset A\alpha_{n-r+1} \neq A$.

Nous sommes donc dans les conditions d’application du cor. de la prop. 2 (VII, p. 16) : les idéaux $A\alpha_i$ ($1 \leq i \leq n$) sont déterminés de façon unique par $M'/M$.

Comme $L$ est somme directe de $M'$ et de $L'$, $L/M$ est somme de $M'/M$ et de $(L' + M)/M$, somme qui est directe puisque $M' \cap (L' + M) = M$; d’autre part $(L' + M)/M$ est isomorphe à $L'/(M \cap L')$ (I, p. 39, th. 4, c)), c’est-à-dire à $L'$, ce qui montre que $(L' + M)/M$ est un module libre isomorphe à $L/M'$.

#### Corollaire {#alg-vii-s4-n3-cor-1 .statement}

*Pour qu’un sous-module de rang fini $M$ d’un module libre $L$ sur un anneau principal $A$ admette un supplémentaire, il faut et il suffit que $L/M$ soit sans torsion*.

Avec les notations du th. 1, si $L/M$ est sans torsion, on a $M = M'$, et $M'$ admet un supplémentaire $L'$ dans $L$. Si réciproquement $M$ admet un supplémentaire $L'$ dans $L$, $L/M$ est isomorphe à $L'$, qui est libre (VII, p. 14, cor. 2), et *a fortiori* sans torsion.

#### Remarque {#alg-vii-s4-n3-rem-1 .statement}

Il peut se faire qu’un sous-module M de rang infini d’un module libre L soit tel que L/M soit sans torsion, mais que M n’admette pas de supplémentaire dans L (VII, p. 58, exerc. 6, b)).

#### Définition 1 {#alg-vii-s4-def-1 .statement}

Les hypothèses et les notations étant celles du th. 1, les idéaux $A\alpha_i$ de A sont appelés les facteurs invariants du sous-module M par rapport au module L.

Dans le cas où A est, soit l’anneau $\mathbf{Z}$ des entiers rationnels, soit l’anneau K[X] des polynômes à une indéterminée sur un corps K, on peut choisir de façon canonique un générateur dans chaque idéal de A : un entier positif dans le cas de $\mathbf{Z}$, un polynôme unitaire dans celui de K[X] (VII, p. 5). Dans chacun de ces cas, le générateur canonique du facteur invariant $A\alpha_i$ est aussi appelé, par abus de langage, facteur invariant de M par rapport à L.

### 4. Structure des modules de type fini

#### Théorème 2 {#alg-vii-s4-thm-2 .statement}

Tout module de type fini E sur un anneau principal A est isomorphe à une somme directe de modules monogènes $A/\alpha_k$, en nombre fini m, où les $\alpha_k$ sont des idéaux de A (dont certains peuvent être nuls), tels que $\alpha_1 \subset \alpha_2 \ldots \subset \alpha_m \neq A$, et qui sont déterminés de façon unique par ces conditions.

Si E peut être engendré par q générateurs, il est isomorphe à un module quotient L/M où $L = A^q$ (II, p. 27). Comme M est de rang fini $n \leq q$ (VII, p. 14, prop. 1), nous sommes dans les conditions d’application du th. 1 (VII, p. 17). Avec les notations de ce dernier, L/M est isomorphe à la somme directe d’un supplémentaire L’ de M’ dans L, et du module de torsion M’/M. Le module L’ est libre et de rang fini $p = q - n$, donc isomorphe à $A^p$. Si r est le plus petit indice tel que $A\alpha_r \neq A$, M’/M est isomorphe à la somme directe des modules $A/A\alpha_i$ pour $r \leq i \leq n$. On satisfera alors aux conditions énoncées en prenant $m = p + (n - r + 1)$, $\alpha_k = (0)$ pour $1 \leq k \leq p$, et $\alpha_{p+j} = A\alpha_{n-j+1}$ pour $1 \leq j \leq n - r + 1$. Quant à l’unicité, elle résulte du cor. de VII, p. 16.

#### Corollaire 1 {#alg-vii-s4-thm-2-cor-1 .statement}

Tout module de type fini E sur un anneau principal est somme directe du sous-module de torsion de E et d’un module libre.

Le sous-module de torsion de E admet en général plusieurs supplémentaires distincts. Par exemple si $E = \mathbf{Z} \times (\mathbf{Z}/(2))$, le sous-module de torsion de E est $\{0\} \times (\mathbf{Z}/(2))$; il admet pour supplémentaire le sous-module $\mathbf{Z} \times \{0\}$, et aussi le sous-module formé des éléments $(n, \bar{n})$, où n parcourt $\mathbf{Z}$ et $\bar{n}$ est la classe de n mod. 2.

#### Corollaire 2 {#alg-vii-s4-thm-2-cor-2 .statement}

Sur un anneau principal, tout module sans torsion et de type fini est un module libre de rang fini.

Ceci résulte aussitôt du cor. 1.

L’hypothèse que le module est de type fini est essentielle. Par exemple le groupe additif du corps des fractions K de A, considéré comme A-module, est sans torsion ; cependant ce n’est pas un module libre si $A \neq K$, car, d’une part, toute famille d’au moins 2 éléments de K est liée, et d’autre part K n’est pas un A-module monogène, sinon on aurait $K = ab^{-1}A$ ($a \in A, b \in A$), d’où $b^{-2} = acb^{-1}$ ($c \in A$), $b^{-1} = ac \in A$, et $K = A$.

#### Définition 2 {#alg-vii-s4-def-2 .statement}

Les hypothèses et les notations étant celles du th. 2, les idéaux $\alpha_k$ sont appelés les facteurs invariants du module E.

Comme dans la déf. 1 (VII, p. 19), lorsque $A = \mathbf{Z}$ ou $A = K[X]$, le générateur canonique de l’idéal $\alpha_k$ (entier positif, ou polynôme unitaire) est aussi appelé, par abus de langage, facteur invariant du module de type fini E.

On aura soin de ne pas confondre les facteurs invariants d’un module E, avec ceux d’un sous-module M d’un module libre L par rapport au module L (déf. 1).

### 5. Calcul des facteurs invariants

#### Proposition 4 {#alg-vii-s4-prop-4 .statement}

Soient A un anneau principal, L un A-module libre de base finie $(u_j)$ ($1 \leq j \leq k$), M un sous-module de L, $(x_i)$ un système de générateurs de M, et $A\alpha_i$ ($1 \leq i \leq n$) les facteurs invariants de M par rapport à L. Alors, pour $1 \leq m \leq n$, le produit $\delta_m = \alpha_1 \ldots \alpha_m$ est un pgcd des mineurs d’ordre m de la matrice dont les colonnes sont formées avec les coordonnées des $x_i$ par rapport à la base $(u_j)$.

D’après le th. 1, il est clair que l’on a $M \subset \alpha_1 L$; donc les coordonnées d’un élément quelconque de M sont toutes multiples de $\alpha_1$. D’autre part, il existe un élément $x$ de M dont $\alpha_1$ est un contenu dans L. En exprimant $x$ comme combinaison linéaire des $x_i$, on en déduit que $\alpha_1$ est élément de l’idéal engendré par les coordonnées des $x_i$. Comme celles-ci sont toutes multiples de $\alpha_1$, il en résulte que $\alpha_1$ est bien leur pgcd, et notre assertion est démontrée pour $m = 1$.

Pour m quelconque, considérons le module $\bigwedge^m M$, puissance extérieure m-ième de M (III, p. 76). Avec les notations du th. 1, M admet pour base $(a_i)$ où $a_i = \alpha_i e_i$ ($1 \leq i \leq n$); donc $\bigwedge^m M$ admet une base formée des éléments $a_{i_1} \wedge \ldots \wedge a_{i_m}$, $(i_1, \ldots, i_m)$ parcourant l’ensemble des suites strictement croissantes de m indices de $[1, n]$. Or les éléments $e_{i_1} \wedge \ldots \wedge e_{i_m}$ appartiennent à une base $B_m$ de $\bigwedge^m L$. Donc l’application canonique de $\bigwedge^m M$ dans $\bigwedge^m L$ est un isomorphisme de $\bigwedge^m M$ sur le sous-module de $\bigwedge^m L$ ayant pour base les éléments $(\alpha_{i_1} \ldots \alpha_{i_m}) e_{i_1} \wedge \ldots \wedge e_{i_m}$, sous-module que l’on identifie à $\bigwedge^m M$. Comme $\alpha_j$ est multiple de $\alpha_k$ pour $j \geq k$, les éléments $\alpha_{i_1} \ldots \alpha_{i_m}$ sont tous multiples de $\delta_m = \alpha_1 \ldots \alpha_m$, et l’un d’eux lui est égal ; donc $\delta_m$ est un pgcd de l’ensemble des coordonnées, par rapport à la base $B_m$ de $\bigwedge^m L$, des éléments d’un système de générateurs de $\bigwedge^m M$. La première partie du raisonnement montre alors que $\delta_m$ est un pgcd de l’ensemble des coordonnées d’un système quelconque de générateurs de $\bigwedge^m M$, par rapport à une base quelconque de $\bigwedge^m L$. En prenant pour base de $\bigwedge^m L$ celle qui est canoniquement déduite de la base $(u_j)$ de L, et pour système de générateurs de $\bigwedge^m M$ celui formé par les produits extérieurs des $(x_i)$, l’expression des coordonnées de ces produits au moyen de déterminants (III, p. 96, prop. 9) donne le résultat annoncé.

### 6. Applications linéaires de modules libres, et matrices sur un anneau principal

Soit A un anneau principal. Considérons une application linéaire f d’un A-module libre L de rang m dans un A-module libre L’ de rang n. Les résultats précédents permettent, par un choix convenable des bases de L et L’, de mettre la matrice de f sous une forme particulièrement simple, dite forme canonique de cette matrice.

#### Proposition 5 {#alg-vii-s4-prop-5 .statement}

Soient A un anneau principal, et f une application linéaire de rang r d’un A-module libre L de rang m dans un A-module libre L’ de rang n. Il existe alors des bases (e_i) (1 \leq i \leq m) de L et (e_j’) (1 \leq j \leq n) de L’ telles que f(e_i) = \alpha_i e_i’ pour 1 \leq i \leq r et f(e_i) = 0 pour i > r, les \alpha_i étant des éléments non nuls de A dont chacun divise le suivant ; les idéaux A\alpha_i sont les facteurs invariants de f(L) dans L’, et sont donc déterminés de façon unique.

Soit L_0 = \overline{f}(0) le noyau de f ; le quotient L/L_0 est isomorphe au module f(L), qui est libre en tant que sous-module de L’ (VII, p. 14, cor. 2) ; donc L_0 admet un supplémentaire L_1 dans L (II, p. 27, prop. 21), et la restriction de f à L_1 est un isomorphisme de L_1 sur f(L) = M’. Si les idéaux A\alpha_i (1 \leq i \leq r) sont les facteurs invariants de M’ dans L’, le th. 1 de VII, p. 17 montre qu’il existe une base (e_j’) (1 \leq j \leq n) de L’ telle que (\alpha_i e_i’) (1 \leq i \leq r) soit une base de M’. Comme la restriction de f à L_1 est un isomorphisme de L_1 sur M’, il existe une base (e_i) (1 \leq i \leq r) de L_1 telle que f(e_i) = \alpha_i e_i’. On complète cette base de L_1 en une base (e_k) (1 \leq k \leq m) de L au moyen d’une base (e_s) (r + 1 \leq s \leq m) du noyau L_0.

#### Corollaire 1 {#alg-vii-s4-prop-5-cor-1 .statement}

Soit X une matrice de rang r, à n lignes et m colonnes, sur un anneau principal A ; il existe alors une matrice X_0 équivalente à X (II, p. 155) de la forme

$$
\begin{pmatrix}
\alpha_1 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & \alpha_2 & \ldots & 0 & 0 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & \alpha_r & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0
\end{pmatrix}
$$

les \alpha_i étant des éléments non nuls de A dont chacun divise le suivant. Dans ces conditions les \alpha_i sont déterminés à des facteurs inversibles près.

Étant données que deux matrices X et X’ sont équivalentes s’il existe des matrices carrées inversibles P et Q, d’ordres n et m, sur A, telles que X’ = PXQ, le corollaire 1 n’est que la traduction en termes de matrices de la prop. 5.

Avec les notations de la prop. 5 et du cor. 1, les idéaux (non nuls) A\alpha_i sont appelés les facteurs invariants de l’application linéaire f, ou de la matrice X. Il résulte alors aussitôt du cor. 1 que :

#### Corollaire 2 {#alg-vii-s4-prop-5-cor-2 .statement}

Pour que deux matrices $X$ et $X'$ à $n$ lignes et $m$ colonnes sur un anneau principal $\mathbf{A}$ soient équivalentes, il faut et il suffit qu’elles aient mêmes facteurs invariants.

On remarquera que, lorsque $\mathbf{A}$ est un corps, on peut prendre les $\alpha_i$ égaux à 1, et l’on retrouve alors la prop. 13 de II, p. 160.

Si $X$ est la matrice de l’application linéaire $f$ par rapport à une base quelconque de $L$ et une base quelconque de $L'$, les colonnes de $X$ sont formées avec les coordonnées, par rapport à la base de $L'$, d’éléments de $L'$ qui constituent un système générateur de $f(L)$. On déduit donc aussitôt de la prop. 4 le résultat suivant :

#### Proposition 6 {#alg-vii-s4-prop-6 .statement}

Soient $X$ une matrice de rang $r$ sur un anneau principal $\mathbf{A}$, et $\mathbf{A} \alpha_i$ ($1 \leq i \leq r$) la suite de ses facteurs invariants. Alors $\alpha_1$ est un pgcd des éléments de $X$; et le produit $\alpha_1 \ldots \alpha_q$ est un pgcd des mineurs d’ordre $q$ de $X$ pour tout $q \leq r$.

### 7. Groupes commutatifs de type fini

Dans le cas où $\mathbf{A} = \mathbf{Z}$, les résultats du no 4 s’écrivent :

#### Théorème 3 {#alg-vii-s4-thm-3 .statement}

Tout groupe commutatif $G$ de type fini est somme directe de son sous-groupe de torsion $F$ (sous-groupe des éléments d’ordre fini de $G$) et d’un groupe commutatif libre de rang fini $p$ (isomorphe à $\mathbf{Z}^p$). Le groupe $F$ est somme directe d’un nombre fini de groupes cycliques d’ordres $n_1, n_2, \ldots, n_q$, où les $n_i$ sont des entiers $> 1$ dont chacun divise le précédent ; en outre, les entiers $p, q$ et $n_i$ ($1 \leq i \leq q$) sont déterminés de façon unique par $G$.

#### Remarque {#alg-vii-s4-n7-rem-1 .statement}

Tandis que les ordres $n_1, \ldots, n_q$ des groupes cycliques dont $F$ est la somme directe sont bien déterminés par la condition de divisibilité du th. 3, il n’en est pas ainsi de ces sous-groupes eux-mêmes : par exemple, dans le produit $G$ de $\mathbf{Z}/(p)$ par lui-même ($p$ premier), les sous-groupes sont identiques aux sous-espaces vectoriels sur le corps $\mathbf{F}_p$, et $G$ est somme directe de deux sous-espaces de dimension 1 de $p(p+1)$ façons différentes.

#### Corollaire 1 {#alg-vii-s4-thm-3-cor-1 .statement}

Dans un groupe commutatif fini $G$, il existe un élément dont l’ordre est le ppcm des ordres de tous les éléments de $G$; cet ordre $n_1$ est le premier facteur invariant de $G$.

#### Corollaire 2 {#alg-vii-s4-thm-3-cor-2 .statement}

Tout groupe commutatif fini $G$ dont l’ordre n’est pas divisible par le carré d’un entier $> 1$ est cyclique.

Conservons les notations du th. 3. On a $p = 0$ car $G$ est fini et $q \leq 1$, car sinon l’ordre de $G$ serait divisible par $n_q^2$. Donc $G$ est cyclique.

#### Corollaire 3 {#alg-vii-s4-thm-3-cor-3 .statement}

Soient $L, M$ deux $\mathbf{Z}$-modules libres de rang $n$, $(e_i)$ une base de $L$, $(f_i)$ une base de $M$ ($1 \leq i \leq n$), $u$ un homomorphisme de $L$ dans $M$, $U$ sa matrice par rapport aux bases $(e_i)$ et $(f_i)$. Pour que $\mathrm{Coker}(u) = M/u(L)$ soit fini, il faut et il suffit que $\det(U) \neq 0$, et on a alors $\mathrm{Card}(\mathrm{Coker}(u)) = |\det(U)|$.

En changeant au besoin de bases dans L et M on peut supposer que U est de la forme décrite dans VII, p. 21, cor. 1 de la prop. 5 (les $\alpha_i$ étant ici des entiers); le corollaire devient alors évident, l’ordre d’une somme directe de $\mathbf{Z}$-modules $\mathbf{Z}/\alpha_i\mathbf{Z}$ ($1 \leq i \leq n$) étant infini si l’un des $\alpha_i$ est nul et égal à $|\alpha_1 \alpha_2 \ldots \alpha_n|$ sinon.

### 8. Modules indécomposables. Diviseurs élémentaires

#### Définition 3 {#alg-vii-s4-def-3 .statement}

Un module à gauche M sur un anneau A est dit décomposable s’il est somme directe d’une famille de sous-modules distincts de M et de $\{0\}$, indécomposable dans le cas contraire.

Un module réduit à 0 est donc décomposable, étant somme directe de la famille vide de sous-modules.

Soit a un idéal à gauche de l’anneau A ; les sous-modules de $A_s/a$ sont les quotients b/a, où b est un idéal de A contenant a (I, p. 39, th. 4); si b et c sont deux idéaux de A contenant a, le module $A/a$ est somme directe de ses sous-modules b/a et c/a si et seulement si on a $A = b + c$ et $b \cap c = a$. Par conséquent :

#### Lemme 2 {#alg-vii-s4-lem-2 .statement}

Pour que le module $A/a$ soit indécomposable, il faut et il suffit que $a \neq A$, et qu’il n’existe pas de couple (b, c) d’idéaux de A, distincts de A et de a, et tels que $A = b + c, a = b \cap c$.

#### Proposition 7 {#alg-vii-s4-prop-7 .statement}

Soient A un anneau commutatif, p un idéal premier de A (I, p. 111, déf. 3) et q un idéal de A contenu dans p. On suppose qu’il existe pour tout $x \in p$ un entier $n > 0$ tel que $x^n \in q$. Alors le A-module $A/q$ est indécomposable.

Soient b et c deux idéaux de A, tels que $A = b + c$ et $b \cap c = q$. On a $bc \subset b \cap c = q \subset p$; si $x \notin p$ et $x \in c$, alors $xb \subset p$, donc $b \subset p$ (I, p. 111, prop. 4); on a donc, soit $b \subset p$, soit $c \subset p$. Supposons par exemple $c \subset p$, donc $b + p = A$; il existe $x \in b$ et $y \in p$ tels que $1 = x + y$; soit $n \in \mathbf{N}$ tel que $y^n \in q$; on a $1 = (x + y)^n$, donc $1 \in xA + y^nA \subset b + q \subset b$, donc $b = A$. Appliquant le lemme 2, on en déduit que $A/q$ est indécomposable.

Supposons maintenant A principal ; d’après VII, p. 2, prop. 2, les idéaux premiers de A sont les idéaux ($p$), où $p$ est un élément extrémal de A, et l’idéal 0 ; d’après la proposition précédente, les modules A et $A/(p^n)$, $p$ extrémal, $n > 0$, sont indécomposables. Comme tout module monogène est somme directe de modules du type précédent (VII, p. 3, prop. 4) et que tout A-module de type fini est somme directe de modules monogènes (VII, p. 19, th. 2), on en conclut :

#### Proposition 8 {#alg-vii-s4-prop-8 .statement}

Soient A un anneau principal et M un A-module de type fini.

a) Pour que M soit indécomposable, il faut et il suffit qu’il soit isomorphe à A où à un module de la forme $A/(p^n)$, où $p$ est un élément extrémal de A et n un entier $> 0$.

b) M est somme directe d’une famille finie de sous-modules indécomposables.

On peut préciser la partie b) de la proposition précédente comme suit :

#### Proposition 9 {#alg-vii-s4-prop-9 .statement}

Soient $\mathbf{A}$ un anneau principal, $\mathbf{P}$ un système représentatif d’éléments extrémaux de $\mathbf{A}$ et $\mathbf{M}$ un $\mathbf{A}$-module de type fini. Il existe des entiers positifs $m(0)$ et $m(p^n)$, $p \in \mathbf{P}$, $n > 0$, uniquement déterminés, nuls à l’exception d’un nombre fini et tels que $\mathbf{M}$ soit isomorphe à la somme directe de $\mathbf{A}^{m(0)}$ et des $(\mathbf{A}/(p^n))^{m(p^n)}$, $p \in \mathbf{P}$, $n > 0$.

L’existence des entiers $m(0)$ et $m(p^n)$, $p \in \mathbf{P}$, $n > 0$ résulte de la prop. 8. L’entier $m(0)$ est uniquement déterminé : c’est le rang du module libre quotient de $\mathbf{M}$ par son sous-module de torsion. Enfin, le composant $p$-primaire de $\mathbf{M}$ est isomorphe à la somme directe des $(\mathbf{A}/(p^n))^{m(p^n)}$ ; comme la famille des idéaux $(p^n)$ ($n \geqslant 1$) est totalement ordonnée par inclusion, l’unicité des $m(p^n)$ résulte du cor. de la prop. 2 de VII, p. 16.

#### Définition 4 {#alg-vii-s4-def-4 .statement}

Les notations étant celles de la prop. 9, les idéaux $(p^n)$ ($p \in \mathbf{P}$, $n$ entier $\geqslant 1$) tels que $m(p^n) > 0$ sont appelés les diviseurs élémentaires du module $\mathbf{M}$, et les entiers $m(p^n)$ leurs multiplicités ; si l’entier $m(0)$ est $> 0$, on l’appelle la multiplicité du diviseur élémentaire 0.

Comme pour les facteurs invariants (VII, p. 19, déf. 1), lorsque $\mathbf{A} = \mathbf{Z}$, ou $\mathbf{A} = \mathbf{K}[X]$ ($\mathbf{K}$ corps commutatif), le générateur canonique de l’idéal $(p^n)$ (entier positif ou polynôme unitaire) est aussi appelé; par abus de langage, diviseur élémentaire du module de type fini $\mathbf{M}$.

#### Remarque 1 {#alg-vii-s4-n8-rem-1 .statement}

Si $\mathbf{M}$ est un groupe commutatif fini, on décrit sa structure en écrivant successivement ses diviseurs élémentaires, chacun autant de fois que l’indique sa multiplicité. On dira, par exemple, que le groupe $\mathbf{M}$ est « de type $(2, 2, 4, 27, 27, 25)$ » (ou que c’est « un groupe $(2, 2, 4, 27, 27, 25)$ ») s’il est isomorphe au produit de deux groupes $\mathbf{Z}/(2)$, d’un groupe $\mathbf{Z}/(2^2)$, de deux groupes $\mathbf{Z}/(3^3)$ et d’un groupe $\mathbf{Z}/(5^2)$.

#### Remarque 2 {#alg-vii-s4-n8-rem-2 .statement}

Si un module de torsion de type fini $\mathbf{M}$ sur un anneau principal $\mathbf{A}$ est donné comme somme directe de modules monogènes isomorphes à des $\mathbf{A}/(a_i)$ (et en particulier lorsqu’on connaît les facteurs invariants de $\mathbf{M}$), on détermine les diviseurs élémentaires de $\mathbf{M}$, ainsi que leurs multiplicités, en remarquant que $\mathbf{A}/(a)$ est isomorphe au produit des $\mathbf{A}/(p^{n(p)})$, si $a = \varepsilon \prod_{p \in \mathbf{P}} p^{n(p)}$ est la décomposition de $a$ en facteurs extrémaux (VII, p. 3). Étudions par exemple le groupe multiplicatif $G(464\,600)$, où $G(n)$ désigne pour simplifier le groupe multiplicatif $(\mathbf{Z}/n\mathbf{Z})^*$ (VII, p. 11). Comme $464\,600 = 2^3 \cdot 5^2 \cdot 23 \cdot 101$, ce groupe est isomorphe au produit des groupes $G(2^3)$, $G(5^2)$, $G(23)$ et $G(101)$ (VII, p. 13, th. 3) ; or, les trois derniers groupes sont cycliques d’ordres 20, 22 et 100, et $G(2^3)$ est produit de deux groupes cycliques d’ordre 2 (*loc. cit.*); comme $20 = 2^2 \cdot 5$, $22 = 2 \cdot 11$ et $100 = 2^2 \cdot 5^2$, le groupe $G(464\,600)$ est du type $(2, 2, 2, 2^2, 2^2, 5, 5^2, 11)$.

#### Remarque 3 {#alg-vii-s4-n8-rem-3 .statement}

Pour le calcul des facteurs invariants d’un module de torsion dont on suppose connus les diviseurs élémentaires, on s’appuie encore sur le fait que, si les $a_i$ sont des éléments de $\mathbf{A}$ étrangers deux à deux, le produit $\prod_i \mathbf{A}/(a_i)$ est un module monogène isomorphe à $\mathbf{A}/(a_1 a_2 \ldots a_n)$ (VII, p. 3, prop. 4). Exposons la méthode sur l’exemple du groupe $\mathbf{M} = G(464\,600)$ : on écrit sur une même ligne les diviseurs élémentaires $p^n$ de $\mathbf{M}$ relatifs au même élément extrémal $p$, en commençant par ceux d’exposant le plus élevé ; chaque ligne ainsi formée est complétée (si nécessaire) par des 1, de façon à avoir des lignes de même longueur :

$$
\begin{array}{cccccc}
2^2, & 2^2, & 2, & 2, & 2 \\
5^2, & 5, & 1, & 1, & 1 \\
11, & 1, & 1, & 1, & 1
\end{array}
$$

Les facteurs invariants sont alors les produits des éléments d’une même colonne : 1 100, 20, 2, 2, 2. En effet, M est isomorphe à un produit de groupes cycliques d’ordres 1 100, 20, 2, 2, 2 d’après la prop. 4 de VII, p. 3 ; comme chacun de ces ordres est multiple du suivant, ce sont les facteurs invariants de M (VII, p. 22, th. 3).

#### Remarque 4 {#alg-vii-s4-n8-rem-4 .statement}

Un A-module est dit simple (I, p. 36) s’il est non nul et s’il ne possède pas d’autres sous-modules que lui-même et 0 ; il est alors nécessairement monogène, donc de type fini, et indécomposable ; comme les modules $A/(p^n)$ pour $n \neq 1$ ne sont pas simples, que les modules $A/(p)$ le sont, et que A n’est simple que si l’anneau A est un corps, on en conclut que les A-modules simples sont :
   a) lorsque A est un corps, les modules libres de rang 1 ;
   b) lorsque A n’est pas un corps, les modules isomorphes à des quotients $A/(p)$, où $p$ est un élément extrémal de A.

### 9. Dualité des modules de longueur finie sur un anneau principal

Dans ce n°, A désigne un anneau principal qui n’est pas un corps (et a donc au moins un élément extrémal), K le corps des fractions de A. Pour tout A-module M, on posera

$$
D(M) = \operatorname{Hom}_A(M, K/A);
$$

on sait que D(M) est canoniquement muni d’une structure de A-module, telle que, pour tout homomorphisme $u : M \to K/A$ et tout $\alpha \in A$, $\alpha u$ soit l’homomorphisme $x \mapsto \alpha u(x) = u(\alpha x)$. À tout homomorphisme de A-modules $f : M \to N$, on associe l’homomorphisme $D(f) : D(N) \to D(M)$ tel que $D(f)(v) = v \circ f$ (II, p. 6). Pour $x \in M,\ x' \in D(M)$, nous poserons $\langle x, x' \rangle = x'(x) \in K/A ;\ (x, x') \mapsto \langle x, x' \rangle$ est une application A-bilinéaire de $M \times D(M)$ dans $K/A$, dite canonique.

Si M et N sont deux A-modules, à toute application A-bilinéaire $\varphi : M \times N \to K/A$ sont associées l’application A-linéaire $d_\varphi : N \to D(M)$ et l’application A-linéaire $s_\varphi : M \to D(N)$ telles que $d_\varphi(y)(x) = \varphi(x, y)$ et $s_\varphi(x)(y) = \varphi(x, y)$ (II, p. 74, cor. de la prop. 1). En particulier, l’application A-bilinéaire canonique $M \times D(M) \to K/A$ définit ainsi une application A-linéaire (dite aussi canonique).

$$
c_M : M \to D(D(M))
$$

telle que $\langle x', c_M(x) \rangle = \langle x, x' \rangle$ pour $x \in M,\ x' \in D(M)$.

#### Proposition 10 {#alg-vii-s4-prop-10 .statement}

Si M est un A-module de longueur finie, D(M) est isomorphe (non canoniquement, en général) à M, et l’application canonique $c_M : M \to D(D(M))$ est un isomorphisme.

Utilisant VII, p. 19, th. 2 et II, p. 13, cor. 1, on se ramène au cas où M est monogène. On peut donc supposer $M = A/tA$, avec $t \neq 0$. Notons que tout homomorphisme $u : A/tA \to K/A$ est entièrement déterminé par l’image $\xi \in K/A$ par $u$ de la classe $\varepsilon$ de 1 mod. $tA$, cet élément devant satisfaire à la relation $t\xi = 0$; inversement, pour tout $\xi \in K/A$ tel que $t\xi = 0$, il existe un homomorphisme $u : A/tA \to K/A$ tel que $u(\varepsilon) = \xi$. On en conclut que D(M) est isomorphe à $t^{-1}A/A$, et comme l’homothétie de rapport $t$ est bijective dans K, D(M) est aussi isomorphe à $A/tA$, ce qui démontre la première assertion. Cela montre que M et D(D(M)) sont isomorphes, donc ont même longueur ; d’autre part, $c_M$ est injective, car si $y \in A$ est tel que la relation $tz \in A$ (pour $z \in K$) entraîne $yz \in A$, on a, en prenant $z = t^{-1}$, $y \in tA$. On en conclut que l’image $c_M(M)$ est nécessairement égale à $D(D(M))$.

#### Corollaire {#alg-vii-s4-n9-cor-1 .statement}

*Soient M, N deux A-modules de longueur finie, φ une application A-bilinéaire de M × N dans K/A, telle que : 1° la relation $\varphi(x, y) = 0$ pour tout $y \in N$ entraîne $x = 0$; 2° la relation $\varphi(x, y) = 0$ pour tout $x \in M$ entraîne $y = 0$. Alors les applications A-linéaires $s_\varphi : M \to D(N)$ et $d_\varphi : N \to D(M)$ associées à $\varphi$ sont des isomorphismes.*

En effet, les hypothèses sur $\varphi$ signifient que $s_\varphi$ et $d_\varphi$ sont *injectives*, et comme $\operatorname{long}(D(N)) = \operatorname{long}(N)$ et $\operatorname{long}(D(M)) = \operatorname{long}(M)$ en vertu de la prop. 10, cela entraîne que $\operatorname{long}(M) = \operatorname{long}(N)$, et par suite $s_\varphi$ et $d_\varphi$ sont bijectives.

#### Proposition 11 {#alg-vii-s4-prop-11 .statement}

*Si $M' \xrightarrow{u} M \xrightarrow{v} M''$ est une suite exacte de A-modules de longueur finie, la suite $D(M'') \xrightarrow{D(v)} D(M) \xrightarrow{D(u)} D(M')$ est exacte*¹.

Montrons d’abord que si l’on a une suite exacte

(1)
$$
0 \to M' \to M \to M'' \to 0
$$

la suite correspondante
$$
0 \to D(M'') \to D(M) \to D(M') \to 0
$$
est exacte ; on sait en effet que la suite
$$
0 \to D(M'') \to D(M) \to D(M')
$$
est exacte (II, p. 36, th. 1) ; d’autre part, on tire de (1) que l’on a
$$
\operatorname{long}(M) = \operatorname{long}(M') + \operatorname{long}(M'')
$$
(II, p. 21, prop. 16) ; compte tenu de la prop. 10, on a donc
$$
\operatorname{long}(D(M)) = \operatorname{long}(D(M')) + \operatorname{long}(D(M'')),
$$
autrement dit, $\operatorname{long}(D(M')) = \operatorname{long}(D(M)/D(M''))$. Comme $D(M)/D(M'')$ s’identifie canoniquement à un sous-module de $D(M')$, il est nécessairement identique à $D(M')$, ce qui prouve notre assertion.

Cela entraîne aussitôt que si $u : M' \to M$ est injectif, $D(u) : D(M) \to D(M')$ est surjectif ; la conclusion résulte alors de II, p. 9, remarque 4.

Pour tout A-module M, désignons par $\mathfrak{S}(M)$ l’ensemble des sous-modules de M. Pour tout sous-module N de M (resp. tout sous-module N’ de D(M)), désignons par $N^0$ (resp. ${N'}^0$) le sous-module de D(M) (resp. de M) formé des $x' \in D(M)$ (resp. $x \in M$) tels que $\langle y, x' \rangle = 0$ pour tout $y \in N$ (resp. $\langle x, y' \rangle = 0$ pour tout $y' \in N'$).

¹ Nous verrons plus tard (A, X, p. 18) que le A-module K/A est injectif. Par suite, la prop. 11 reste valable pour des A-modules quelconques M, M’ et M''.

#### Proposition 12 {#alg-vii-s4-prop-12 .statement}

Soit $M$ un $A$-module de longueur finie. Alors l’application qui, à tout sous-module $N$ de $M$, fait correspondre $N^0$, est une bijection de $\mathfrak{S}(M)$ sur $\mathfrak{S}(D(M))$, et la bijection réciproque fait correspondre à tout sous-module $N'$ de $D(M)$ le sous-module ${N'}^0$ de $M$; $D(N)$ s’identifie canoniquement à $D(M)/N^0$ et $D(M/N)$ à $N^0$. En outre, on a

$$
(N_1 + N_2)^0 = N_1^0 \cap N_2^0, \quad (N_1 \cap N_2)^0 = N_1^0 + N_2^0
$$

quels que soient les sous-modules $N_1, N_2$ de $M$.

Pour tout sous-module $N$ de $M$, on a la suite exacte

$$
0 \to N \to M \to M/N \to 0
$$

d’où la suite exacte (prop. 11)

$$
0 \to D(M/N) \to D(M) \to D(N) \to 0
$$

et comme l’image de $D(M/N)$ dans $D(M)$ est évidemment $N^0$, on voit (prop. 10) que l’on a $\operatorname{long}(N^0) = \operatorname{long}(M) - \operatorname{long}(N)$; comme $M$ s’identifie à $D(D(M))$ par la prop. 10, on a de même

$$
\operatorname{long}(N^{00}) = \operatorname{long}(M) - \operatorname{long}(N^0) = \operatorname{long}(N);
$$

d’ailleurs on a évidemment $N \subset N^{00}$, d’où $N^{00} = N$. De plus la première relation (2) est évidente, et en l’appliquant aux sous-modules $N_1^0$ et $N_2^0$ de $D(M)$, il vient $(N_1^0 + N_2^0)^0 = N_1 \cap N_2$, d’où $N_1^0 + N_2^0 = (N_1^0 + N_2^0)^{00} = (N_1 \cap N_2)^0$. Ceci achève de démontrer la proposition.

#### Exemple 1 {#alg-vii-s4-n9-exa-1 .statement}

Pour $A = \mathbf{Z}$, les $\mathbf{Z}$-modules de longueur finie ne sont autres que les groupes commutatifs finis ; on a alors $K = \mathbf{Q}$, donc $K/A = \mathbf{Q}/\mathbf{Z}$. Pour définir alors $D(M)$, on prend parfois, au lieu de $\mathbf{Q}/\mathbf{Z}$, un $\mathbf{Z}$-module qui lui est isomorphe, par exemple (V, p. 75, prop. 2) le groupe $R$ des racines de l’unité (noté multiplicativement) dans un corps algébriquement clos de caractéristique 0 ; on pose alors $D(M) = \operatorname{Hom}_{\mathbf{Z}}(M, R)$. Nous laissons au lecteur le soin de traduire les résultats qui précèdent dans ce cas particulier et avec les notations correspondantes.

#### Exemple 2 {#alg-vii-s4-n9-exa-2 .statement}

Soit $a$ un élément non nul de $A$. L’application $x \mapsto x/a$ de $A$ dans $K$ induit par passage au quotient un isomorphisme de $A$-modules de $A/(a)$ sur le sous-module $(K/A)(a)$ de $K/A$ formé des éléments annulés par $a$. Si $M$ est un $A$-module annulé par $a$, ou, ce qui revient au même, un $A/(a)$-module, le $A$-module $D(M)$ s’identifie donc à $\operatorname{Hom}_{A/(a)}(M, A/(a))$. Nous laissons au lecteur le soin de traduire les résultats qui précèdent dans ce cas particulier et avec les notations correspondantes (cf. V, p. 82).

## EXERCICES {#alg-vii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
