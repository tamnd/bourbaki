---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 8
section_title: Déterminants
lang: fr
source: alg-i-iii-fr
book_pages: A III.90-A III.107, A III.191-A III.196
pdf_pages: 0477-0494, 0578-0583
extraction: ocr
subsections:
    - "no": 1
      title: Déterminant d’un endomorphisme
      page: 90
      pdf_page: 477
    - "no": 2
      title: Caractérisation des automorphismes d’un module libre de dimension finie
      page: 91
      pdf_page: 478
    - "no": 3
      title: Déterminant d’une matrice carrée
      page: 92
      pdf_page: 479
    - "no": 4
      title: Calcul d’un déterminant
      page: 93
      pdf_page: 480
    - "no": 5
      title: Mineurs d’une matrice
      page: 95
      pdf_page: 482
    - "no": 6
      title: Développements d’un déterminant
      page: 97
      pdf_page: 484
    - "no": 7
      title: Application aux équations linéaires
      page: 101
      pdf_page: 488
    - "no": 8
      title: Cas d’un corps commutatif
      page: 102
      pdf_page: 489
    - "no": 9
      title: Le groupe unimodulaire $\mathbf{SL}(n, A)$
      page: 104
      pdf_page: 491
    - "no": 10
      title: Le $A[X]$-module associé à un endomorphisme de $A$-module
      page: 105
      pdf_page: 492
    - "no": 11
      title: Polynôme caractéristique d’un endomorphisme
      page: 107
      pdf_page: 494
statements: 38
exercises: 26
content_sha256: f14742f5d87ea50c10c3c63903bc1086452d4e9b2213b7d83714481f7b4af3cf
---

## § 8. DÉTERMINANTS

### 1. Déterminant d’un endomorphisme

Soient $M$ un $A$-module ayant une *base finie* de $n$ éléments, $u$ un endomorphisme de $M$. Le $A$-module $\wedge^n(M)$ est un module libre monogène, c’est-à-dire isomorphe à $A$ (III, p. 87, cor. 1); $\wedge^n(u)$ est un endomorphisme de ce module, et est par suite une homothétie $z \mapsto \lambda z$ de rapport $\lambda \in A$ déterminé de façon unique (II, p. 41, prop. 5).

#### Définition 1 {#alg-iii-s8-def-1 .statement}

*On appelle déterminant d’un endomorphisme $u$ d’un $A$-module libre $M$ de dimension finie $n$* (II, p. 98, corollaire et *Remarque 1*), *et on note* $\det u$, *le scalaire* $\lambda$ *tel que* $\wedge^n(u)$ *soit l’homothétie de rapport* $\lambda$.

D’après la formule (4) de III, p. 78, $\det u$ est l’unique scalaire tel que l’on ait
$$
u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n) = (\det u)\, x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$
pour toute suite $(x_i)_{1 \leq i \leq n}$ de $n$ éléments de $M$. Si $\det(u) = 1$, on dit que $u$ est *unimodulaire*.

#### Proposition 1 {#alg-iii-s8-prop-1 .statement}

(i) *Si $u$ et $v$ sont deux endomorphismes d’un $A$-module libre $M$ de dimension finie, on a*
$$
\det(u \circ v) = (\det u)(\det v).
$$
(ii) *On a* $\det(1_M) = 1$; *pour tout automorphisme* $u$ *de* $M$, *$\det u$ est inversible dans* $A$ *et l’on a*
$$
\det(u^{-1}) = (\det u)^{-1}.
$$

Si $n$ est la dimension de $M$, cela résulte aussitôt de la relation $\wedge^n(u \circ v) = (\wedge^n(u)) \circ (\wedge^n(v))$ (III, p. 78, formule (3)).

Soit $M$ un $A$-module libre ayant une base finie $(e_i)_{1 \leq i \leq n}$; étant donnée une suite $(x_i)_{1 \leq i \leq n}$ de $n$ éléments de $M$, on appelle *déterminant* de cette suite *par rapport à la base donnée* $(e_i)$, et on note $\det(x_1, x_2, \ldots, x_n)$ lorsqu’aucune confusion sur la base n’est possible, le déterminant de l’endomorphisme $u$ de $M$ tel que $u(e_i) = x_i$ pour $1 \leq i \leq n$. En vertu de la formule (1), on a donc
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \det(x_1, x_2, \ldots, x_n)\, e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
et cette relation caractérise l’application $(x_i) \mapsto \det(x_1, \ldots, x_n)$ de $M^n$ dans $A$. Elle montre que cette application est une *forme n-linéaire alternée*. Comme, en vertu de III, p. 80, prop. 7, le $A$-module des formes $n$-linéaires alternées est canoniquement isomorphe au dual de $\wedge^n(M)$, et que $\wedge^n(M)$ est isomorphe à $A$, on voit que toute forme $n$-linéaire alternée sur $M^n$ est de la forme

$$
(x_1, \ldots, x_n) \mapsto \alpha \det(x_1, x_2, \ldots, x_n)
$$

pour un $\alpha \in A$.

#### Proposition 2 {#alg-iii-s8-prop-2 .statement}

*Soient M un A-module libre ayant une base finie* $(e_i)_{1 \leq i \leq n}$, *v un endomorphisme de M. Pour toute suite* $(x_i)_{1 \leq i \leq n}$ *de n éléments de M, on a*

(5)

$$
\det(v(x_1), \ldots, v(x_n)) = (\det v) \det(x_1, \ldots, x_n).
$$

En effet, si $u$ est l’endomorphisme de M tel que $u(e_i) = x_i$ pour tout $i$, on a $v(x_i) = (v \circ u)(e_i)$, et (5) résulte donc de (2) (III, p. 90).

### 2. Caractérisation des automorphismes d’un module libre de dimension finie

#### Théorème 1 {#alg-iii-s8-thm-1 .statement}

*Soit M un A-module libre de dimension finie, u un endomorphisme de M. Les conditions suivantes sont équivalentes*:

a) *u est bijectif*;
b) *u est inversible à droite* (II, p. 21, cor. 1);
c) *u est inversible à gauche* (II, p. 21, cor. 2);
d) *u est surjectif*;
e) *det u est inversible dans A*.

Soit $(e_i)_{1 \leq i \leq n}$ une base de M. Si $x_i = u(e_i)$ pour $1 \leq i \leq n$, on a

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det u) e_1 \wedge e_2 \wedge \cdots \wedge e_n.
$$

En vertu de III, p. 89, th. 2, une condition nécessaire et suffisante pour que les $x_i$ forment une base de M est que $\det u$ soit un élément inversible de A; ceci prouve l’équivalence de a) et de e). Observons que a) entraîne évidemment chacune des conditions b), c) et d); il reste à prouver que chacune des conditions b), c) et d) entraîne e). Or, s’il existe un endomorphisme $v$ de M tel que $v \circ u = 1_M$ ou $u \circ v = 1_M$, on a $(\det v)(\det u) = 1$, donc $\det u$ est inversible dans A. Si $u$ est surjectif, il en est de même de $\wedge^n(u)$ (III, p. 78, prop. 3), autrement dit l’homothétie de rapport $\det u$ dans A est surjective, ce qui entraîne aussitôt que $\det u$ est inversible.

#### Proposition 3 {#alg-iii-s8-prop-3 .statement}

*Soit M un A-module libre de dimension finie. Pour tout endomorphisme u de M, les conditions suivantes sont équivalentes*;

f) *u est injectif*;
g) *det u n’est pas diviseur de zéro dans A*.

Avec les mêmes notations que dans la démonstration du th. 1, pour que $u$ soit injectif, il faut et il suffit que les $x_i$ soient linéairement indépendants. D’après III, p. 88, prop. 12, il faut et il suffit pour cela que la relation $\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$ (avec $\lambda \in A$) entraîne $\lambda = 0$. Mais cela équivaut à $\lambda(\det u) = 0$ puisque $e_1 \wedge \cdots \wedge e_n$ est une base de $\wedge^n(M)$; d’où la proposition.

#### Remarque {#alg-iii-s8-n2-rem-1 .statement}

Lorsque A est un corps, la condition e) du th. 2 est équivalente à la condition g) de la prop. 3 puisqu’elles signifient toutes deux que det $u \neq 0$. Il y a donc dans ce cas équivalence entre toutes les conditions du th. 1 et de la prop. 3 (cf. II, p. 101, corollaire).

### 3. Déterminant d’une matrice carrée

#### Définition 2 {#alg-iii-s8-def-2 .statement}

Soient I un ensemble fini, A un anneau commutatif, X une matrice carrée de type (I, I) sur l’anneau A (II, p. 149). On appelle déterminant de X et on note det X le déterminant de l’endomorphisme u du A-module $A^I$, dont X est la matrice par rapport à la base canonique de $A^I$.

Si $X = (\xi_{ij})_{(i,j) \in I \times I}$, et si $(e_i)_{i \in I}$ est la base canonique de $A^I$, l’endomorphisme u est donc donné par

$$
u(e_i) = \sum_{j \in I} \xi_{ji} e_j.
$$

Lorsque $I = \{1, n\} \subset \mathbf{N}$, si l’on pose $x_i = u(e_i)$ pour $i \in I$, le déterminant de X est donc défini par la relation

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det X) \, e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

autrement dit, $\det X$ est égal au déterminant $\det(x_1, x_2, \ldots, x_n)$ par rapport à la base canonique de $A^n$. Par conséquent:

#### Proposition 4 {#alg-iii-s8-prop-4 .statement}

Pour n vecteurs $x_1, \ldots, x_n$ de $A^n$, notons $X(x_1, \ldots, x_n)$ la matrice carrée d’ordre n dont la i-ème colonne est $x_i$, pour $1 \leq i \leq n$. Alors l’application

$$
(x_1, \ldots, x_n) \mapsto \det(X(x_1, \ldots, x_n))
$$

de $(A^n)^n$ dans A est n-linéaire alternée.

En particulier, le déterminant d’une matrice dont deux colonnes sont égales est nul. Si l’on effectue une permutation $\sigma$ sur les colonnes d’une matrice, le déterminant de la nouvelle matrice est égal à celui de l’ancienne multiplié par $\varepsilon_\sigma$. Si l’on ajoute à une colonne d’une matrice un multiple scalaire d’une colonne d’indice différent, le déterminant de la nouvelle matrice est égal à celui de l’ancienne.

Plus généralement, soit M un A-module libre de dimension finie n, et soit $(e_i)_{i \in I}$ une base de M; pour tout endomorphisme u de M, si X est la matrice de u par rapport à la base $(e_i)$, on a

$$
\det(u) = \det(X)
$$

comme cela résulte aussitôt des définitions.

Lorsque $I = \{1, n\}$, le déterminant de $X$ se note aussi $\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ ou simplement $\det(\xi_{ij})$ si cela ne crée pas de confusion, ou encore

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} & \cdots & \xi_{1n} \\
\xi_{21} & \xi_{22} & \cdots & \xi_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
\xi_{n1} & \xi_{n2} & \cdots & \xi_{nn}
\end{vmatrix}
$$

Lorsque $\det X = 1$, on dit que la matrice $X$ est unimodulaire.

#### Exemple 1 {#alg-iii-s8-n3-exa-1 .statement}

Le déterminant de la matrice vide est égal à 1 ; le déterminant d’une matrice carrée d’ordre 1 est égal à l’unique élément de cette matrice. Pour une matrice d’ordre 2

$$
\begin{pmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{pmatrix}
$$

on a, avec les notations précédentes

$$
x_1 \wedge x_2 = (\xi_{11} e_1 + \xi_{21} e_2) \wedge (\xi_{12} e_1 + \xi_{22} e_2) = \xi_{11} \xi_{22} e_1 \wedge e_2 + \xi_{21} \xi_{12} e_2 \wedge e_1
$$

d’où

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{vmatrix} = \xi_{11} \xi_{22} - \xi_{12} \xi_{21}.
$$

Traduisons dans le langage des matrices quelques-uns des résultats des n°s 1 et 2 :

#### Proposition 5 {#alg-iii-s8-prop-5 .statement}

*Si $X$ et $Y$ sont deux matrices carrées sur un anneau commutatif $\mathbf{A}$, ayant même ensemble fini d’indices, on a*

(8)
$$
\det(XY) = (\det X)(\det Y).
$$
*Pour que $X$ soit inversible, il faut et il suffit que $\det X$ soit un élément inversible de $\mathbf{A}$, et on a alors*

(9)
$$
\det(X^{-1}) = (\det X)^{-1}.
$$

Cela résulte aussitôt de III, p. 90, prop. 1 et de III, p. 91, th. 1.

#### Corollaire {#alg-iii-s8-n3-cor-1 .statement}

*Deux matrices carrées semblables ont des déterminants égaux.*
En effet, si $P$ est une matrice carrée inversible, on a $\det(PXP^{-1}) = \det X$ d’après (8) et (9).

#### Proposition 6 {#alg-iii-s8-prop-6 .statement}

*Pour que les colonnes d’une matrice carrée $X$ d’ordre fini soient linéairement indépendantes, il faut et il suffit que $\det X$ ne soit pas un diviseur de zéro dans $\mathbf{A}$.*
Cela résulte de III, p. 91, prop. 3.

### 4. Calcul d’un déterminant

#### Lemme 1 {#alg-iii-s8-lem-1 .statement}

*Soient $\mathbf{A}$ un anneau commutatif, $M$ un $\mathbf{A}$-module libre ayant une base $(e_j)_{j \in J}$, où l’ensemble d’indices $J$ est totalement ordonné. Pour tout entier $p \leq \mathrm{Card}(J)$, toute fonction $p$-linéaire alternée $f : M^p \to N$ (où $N$ est un $A$-module), et toute famille de $p$ éléments $x_i = \sum_{j \in J} \xi_{ji} e_j$ de $M$ ($1 \leq i \leq p$), on a

$$
f(x_1, x_2, \ldots, x_p)
$$
$$
= \sum_{j_1 < j_2 < \ldots < j_p} \left( \sum_{\sigma \in S_p} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(p)}, p} \right) f(e_{j_1}, \ldots, e_{j_p})
$$

où $(j_k)_{1 \leq k \leq p}$ parcourt l’ensemble des suites strictement croissantes de $p$ éléments de $J$.

On a en effet

$$
f(x_1, \ldots, x_p) = \sum_{(j_k)} \xi_{j_1, 1} \xi_{j_2, 2} \cdots \xi_{j_p, p} f(e_{j_1}, e_{j_2}, \ldots, e_{j_p})
$$

où $(j_k)_{1 \leq k \leq p}$ parcourt toutes les suites de $p$ éléments de $J$; il suffit alors d’appliquer à $f$ le cor. 1 de III, p. 81.

En particulier, si $J$ est fini et a $n$ éléments, et si $x_i = \sum_{j \in J} \xi_{ji} e_j$ ($1 \leq i \leq n$) sont $n$ éléments de $M$, on a

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \left( \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n} \right) e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_n}
$$

où $(j_k)_{1 \leq k \leq n}$ est l’unique suite des $n$ éléments de $J$ rangés par ordre croissant, d’où

$$
\det(x_1, x_2, \ldots, x_n) = \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n}.
$$

Les notations étant celles du lemme 1, la comparaison des formules (10) et (11) permet d’écrire

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathcal{F}_p(J)} \det(x_{H, 1}, x_{H, 2}, \ldots, x_{H, p}) e_H
$$

où $\mathcal{F}_p(J)$ est l’ensemble des parties de $J$ ayant $p$ éléments et, pour toute partie $H \in \mathcal{F}_p(J)$, on pose $x_{H, i} = \sum_{j \in H} \xi_{ji} e_j$ et $e_H = e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_p}$, $(j_k)_{1 \leq k \leq p}$ étant la suite des éléments de $H$ rangés par ordre croissant, étant entendu que $\det(x_{H, 1}, \ldots, x_{H, p})$ est pris par rapport à la base $(e_{j_k})_{1 \leq k \leq p}$.

#### Proposition 7 {#alg-iii-s8-prop-7 .statement}

*Soient $I$ un ensemble fini, $X = (\xi_{ji})_{(j, i) \in I \times I}$ une matrice carrée de type $(I, I)$ sur un anneau commutatif $A$. On a alors*

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{\sigma(i), i} \right)
$$

où $\sigma$ parcourt le groupe $S_I$ des permutations de $I$, et où $\varepsilon_\sigma$ est la signature de $\sigma$ (I, p. 62).

On peut se borner au cas où $I = \{1, n\} \subset \mathbf{N}$, et il suffit alors d’appliquer la formule (12), où $(e_i)_{1 \leq i \leq n}$ est la base canonique de $A^n$, et les $x_i$ les colonnes de $X$ (cf. III, p. 92, formule (6)).

En particulier, pour le déterminant d’une matrice d’ordre 3

$$
X = \begin{pmatrix}
\xi_{11} & \xi_{12} & \xi_{13} \\
\xi_{21} & \xi_{22} & \xi_{23} \\
\xi_{31} & \xi_{32} & \xi_{33}
\end{pmatrix}
$$

on a

$$
\det(X) = \xi_{11} \xi_{22} \xi_{33} + \xi_{12} \xi_{23} \xi_{31} + \xi_{21} \xi_{32} \xi_{13} - \xi_{13} \xi_{22} \xi_{31} - \xi_{12} \xi_{21} \xi_{33} - \xi_{11} \xi_{23} \xi_{32}.
$$

#### Proposition 8 {#alg-iii-s8-prop-8 .statement}

*Pour toute matrice carrée $X$ sur un anneau commutatif, le déterminant de la matrice transposée $tX$ est égal au déterminant de $X$.*

Supposons que $X$ soit de type (I, I). Pour tout couple de permutations $\sigma, \tau$ de $\mathfrak{S}_I$, on a (la multiplication étant commutative)

$$
\prod_{i \in I} \xi_{\sigma(i), i} = \prod_{j \in I} \xi_{\sigma(\tau(j)), \tau(j)}.
$$

Prenons en particulier $\tau = \sigma^{-1}$; utilisant le fait que $\varepsilon_{\sigma^{-1}} = \varepsilon_\sigma$, on voit qu’on a

$$
\det X = \sum_{\sigma \in \mathfrak{S}_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{i, \sigma(i)} \right)
$$

ce qui démontre la proposition.

#### Corollaire 1 {#alg-iii-s8-prop-8-cor-1 .statement}

*Pour $n$ vecteurs $x_1, \ldots, x_n$ de $A^n$, notons $Y(x_1, \ldots, x_n)$ la matrice carrée d’ordre $n$ dont la $i$-ème ligne est $x_i$, pour $1 \leq i \leq n$. Alors l’application*

$$
(x_1, \ldots, x_n) \mapsto \det(Y(x_1, \ldots, x_n))
$$

*de $(A^n)^n$ dans $A$ est $n$-linéaire alternée.*

#### Corollaire 2 {#alg-iii-s8-prop-8-cor-2 .statement}

*Pour une matrice carrée $X$ d’ordre fini sur un anneau commutatif $A$, les conditions suivantes sont équivalentes :*
*(i)* les lignes de $X$ sont linéairement indépendantes ;
*(ii)* les colonnes de $X$ sont linéairement indépendantes ;
*(iii)* $\det X$ n’est pas diviseur de zéro dans $A$.

Cela résulte de III, p. 93, prop. 6 et III, p. 95, prop. 8.

#### Corollaire 3 {#alg-iii-s8-prop-8-cor-3 .statement}

*Soient $u$ un endomorphisme d’un $A$-module libre $M$ de dimension finie, $t u$ l’endomorphisme transposé du dual $M^*$ (II, p. 42, déf. 5); on a*

$$
\det(t u) = \det(u).
$$

En effet, si $X$ est la matrice de $u$ par rapport à une base de $M$, $t X$ est la matrice de $t u$ par rapport à la base duale (II, p. 145, prop. 3); comme $\det(u) = \det(X)$ et $\det(t u) = \det(t X)$, la conclusion résulte de la prop. 8.

### 5. Mineurs d’une matrice

Soit $X$ une matrice rectangulaire $(\xi_{ij})_{(i,j) \in I \times J}$ de type (I, J), dont les ensembles d’indices $I$ et $J$ sont *totalement ordonnés*. Si $H \subset I$ et $K \subset J$ sont des parties finies ayant même nombre $p$ d’éléments, il existe une unique bijection croissante $\varphi : H \to K$ (E, III, p. 38, prop. 6); nous noterons $X_{H, K}$ la matrice carrée de type $(H, H)$ égale à $(\xi_{i, \varphi(j)})_{(i, j) \in H \times H}$. Si les éléments de $X$ appartiennent à un anneau commutatif $A$, le déterminant $\det(X_{H, K})$ s’appelle le mineur d’indices $H, K$ de la matrice $X$; on dit aussi que ces déterminants (pour tous les couples $(H, K)$ de parties à $p$ éléments de $I$ et $J$ respectivement) sont les mineurs d’ordre $p$ de $X$. Avec ces notations:

#### Proposition 9 {#alg-iii-s8-prop-9 .statement}

*Soit $M$ un $A$-module ayant une base $(e_i)_{i \in J}$ (finie ou non) dont l’ensemble d’indices $J$ est totalement ordonné. Pour tout entier $p > 0$, soit $(e_H)_{H \in \mathcal{F}_p(J)}$ la base correspondante de $\wedge^p(M)$ (III, p. 86). Soit $(x_i)_{1 \leq i \leq p}$ une suite de $p$ éléments de $M$; posons*

$$
x_i = \sum_{j \in J} \xi_{ji} e_j \quad \text{pour } i \in I = \{1, p\}
$$

*et notons $X$ la matrice $(\xi_{ji})$ de type $(J, I)$. On a alors*

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathcal{F}_p(J)} (\det X_{H, I}) e_H,
$$

$H$ parcourant l’ensemble $\mathcal{F}_p(J)$ des parties à $p$ éléments de $J$.

Cela résulte en effet de la formule (12) de III, p. 94 et de la formule (6) de III, p. 92.

#### Proposition 10 {#alg-iii-s8-prop-10 .statement}

*Soient $M$ et $N$ deux $A$-modules libres de dimensions respectives $m$ et $n$, $u : M \to N$ une application linéaire, $X$ la matrice de $u$ par rapport à une base $(e_i)_{1 \leq i \leq m}$ de $M$ et une base $(f_j)_{1 \leq j \leq n}$ de $N$. Alors, pour tout entier $p \leq \inf(m, n)$, la matrice de $\wedge^p(u)$ par rapport à la base $(e_K)_{K \in \mathcal{F}_p(I)}$ de $\wedge^p(M)$ et à la base $(f_H)_{H \in \mathcal{F}_p(J)}$ de $\wedge^p(N)$ (où l’on a posé $I = \{1, m\}$ et $J = \{1, n\}$) est la matrice $(\det(X_{H, K}))$ de type $(\mathcal{F}_p(J), \mathcal{F}_p(I))$ (donc à $\binom{n}{p}$ lignes et $\binom{m}{p}$ colonnes).

En effet, pour une partie $K \subset J$ à $p$ éléments, soit $(j_k)_{1 \leq k \leq p}$ la suite des éléments de $K$ rangés par ordre croissant; par définition de $\wedge^p(u)$, on a (III, p. 78, formule (4))

$$
\wedge^p(u)(e_K) = u(e_{j_1}) \wedge u(e_{j_2}) \wedge \cdots \wedge u(e_{j_p}).
$$

Donc l’élément de la matrice de $\wedge^p(u)$ qui se trouve dans la ligne d’indice $H$ et dans la colonne d’indice $K$ est la composante d’indice $H$ de l’élément $u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p})$; il est donc égal à $\det(X_{H, K})$ en vertu de la prop. 9.

On dit que la matrice $(\det(X_{H, K}))$ est la puissance extérieure $p$-ème de la matrice $X$ et on la note $\wedge^p(X)$. Lorsque $p = m = n$, $\wedge^n(X)$ est la matrice à un seul élément $\det(X)$.

#### Proposition 11 {#alg-iii-s8-prop-11 .statement}

*Soit $M$ un $A$-module libre de dimension finie $n$; pour tout endomorphisme $u$ de $M$ et tout couple d’éléments $\xi, \eta$ de $A$, on a*

$$
\det(\xi 1_M + \eta u) = \sum_{k \geq 0} \operatorname{Tr}(\wedge^k(u)) \xi^{n-k} \eta^k.
$$

Soit $(e_i)_{1 \leq i \leq n}$ une base de $M$, et posons $I = \{1, n\}$; pour calculer le premier membre de (18), on doit former le produit

$$
(\xi e_1 + \eta u(e_1)) \wedge (\xi e_2 + \eta u(e_2)) \wedge \cdots \wedge (\xi e_n + \eta u(e_n))
$$

qui est égal à la somme des termes $\xi^{n-p} \eta^p z_K$, où

$$
z_K = x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

avec $x_i = u(e_i)$ pour $i \in K$, $x_i = e_i$ pour $i \in H = I - K$, l’entier $p$ parcourant l’intervalle $[0, n]$ et, pour chaque $p$, $K$ parcourant l’ensemble des parties à $p$ éléments de $I$. Si $i_1 < i_2 < \cdots < i_{n-p}$ (resp. $j_1 < j_2 < \cdots < j_p$) sont les éléments de $H$ (resp. $K$) rangés par ordre croissant, on peut écrire (III, p. 87, cor. 1 et formule (19))

$$
z_K = \rho_{H, K} e_{i_1} \wedge e_{i_2} \wedge \cdots \wedge e_{i_{n-p}} \wedge u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}).
$$

Mais si $X$ est la matrice de $u$ par rapport à la base $(e_i)$, on a, en vertu de la prop. 10 (III, p. 96)

$$
u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) = \sum_{L \in \mathfrak{S}_p(I)} (\det X_{L, K}) e_L
$$

donc

$$
z_K = \rho_{H, K} \sum_{L \in \mathfrak{S}_p(I)} (\det X_{L, K}) e_H \wedge e_L.
$$

Or, on a $H \cap L \neq \varnothing$ sauf pour $L = K$; il résulte donc de III, p. 87, formule (20) que l’on a $z_K = (\det X_{K, K}) e_1 \wedge e_2 \wedge \cdots \wedge e_n$ et la formule (18) résulte donc de la prop. 10 de III, p. 96, et de la définition de la trace d’une matrice (II, p. 158, formules (49) et (50)).

#### Corollaire {#alg-iii-s8-n5-cor-1 .statement}

*Sous les mêmes hypothèses que dans la prop. 11, on a, pour l’endomorphisme $\wedge(u)$ du A-module $\wedge(M)$*

(19)
$$
\operatorname{Tr}(\wedge(u)) = \det(l_M + u).
$$

Il suffit de remplacer $\xi$ et $\eta$ par 1 dans (18), et d’observer que la matrice de $\wedge(u)$ par rapport à la base des $e_H$ ($H \in \mathfrak{S}(I)$) est la matrice diagonale des matrices des $\wedge^k(u)$ pour $k \geq 0$ (II, p. 152, *Exemple IV*).

### 6. Développements d’un déterminant

Soit $I$ un ensemble d’indices fini totalement ordonné. Pour toute partie $H$ de $I$, notons $H'$ le complémentaire $I - H$. Soit $X = (\xi_{ji})$ une matrice carrée de type $(I, I)$, qu’on peut considérer comme matrice d’un endomorphisme $u$ de $M = A^I$ par rapport à la base canonique $(e_i)_{i \in I}$ de $M$. Soit $n = \mathrm{Card}(I)$, et soient $H$ une partie de I à $q \leq n$ éléments, K une partie de I à $n - q$ éléments; on peut alors écrire (III, p. 96, prop. 10)

$$
(\wedge^q(u))(e_H) = \sum_R \det(X_{R,H}) e_R
$$

$$
(\wedge^{n-q}(u))(e_K) = \sum_S \det(X_{S,K}) e_S
$$

où R (resp. S) parcourt l’ensemble des parties de I à $q$ (resp. $n - q$) éléments. Il résulte de III, p. 87, formules (19) et (20) que l’on a $e_R \wedge e_S = 0$ sauf si $S = R'$, d’où la formule

(20)
$$
(\wedge^q(u)(e_H)) \wedge (\wedge^{n-q}(u)(e_K)) = \sum_R \rho_{R,R'} \det(X_{R,H}) \det(X_{R',K}) e_I
$$

où R parcourt l’ensemble $\mathfrak{F}_q(I)$ des parties à $q$ éléments de I.

Si l’on prend $K = H'$, il résulte de la définition de $\wedge^n(u)$ (III, p. 78, formule (4)) et de III, p. 79, cor. 1, que le premier membre de (20) est $\rho_{H,H'} \wedge^n(u)(e_I)$. Donc (III, p. 90, formule (1) et III, p. 78, formule (4))

(21)
$$
\det(X) = \rho_{H,H'} \sum_{R \in \mathfrak{F}_q(I)} \rho_{R,R'} \det(X_{R,H}) \det(X_{R',H'})
$$

Si au contraire $K \neq H'$, on a $H \cap K \neq \varnothing$; comme le premier membre de (20) est $\pm \wedge^n(u)(e_H \wedge e_K)$, il est *nul*, d’où

(22)
$$
\sum_R \rho_{R,R'} \det(X_{R,H}) \det(X_{R',K}) = 0 \quad \text{pour } K \neq H'.
$$

Le second membre de (21) est appelé *développement de Laplace* du déterminant de la matrice $X$ suivant les $q$ colonnes dont les indices appartiennent à $H$ et les $n - q$ colonnes dont les indices appartiennent au complémentaire $H'$ de $H$. Les mineurs $\det(X_{R,H})$ et $\det(X_{R',H'})$ sont parfois dits *complémentaires*.

Un cas simple et important du développement de Laplace est celui où $I = \{1, n\}$ et $q = 1$, donc $H = \{i\}$; pour toute partie $R = \{j\}$ à un élément de I, on a alors $\det X_{R,H} = \xi_{ji}$. Le mineur $\det X_{R',H'}$ est le déterminant de la matrice carrée déduite canoniquement (III, p. 96) de la matrice obtenue en supprimant dans $X$ la ligne d’indice $j$ et la colonne d’indice $i$. Notons $X^{ji}$ cette matrice carrée. On a évidemment $\rho_{H,H'} = (-1)^{i-1}$ et $\rho_{R,R'} = (-1)^{j-1}$; par suite (21) devient dans ce cas

(23)
$$
\det X = \sum_{j=1}^n (-1)^{i+j} \xi_{ji} \det(X^{ji})
$$

et on déduit de même de (22)

(24)
$$
\sum_{j=1}^n (-1)^{j} \xi_{ji} \det(X^{jk}) = 0 \quad \text{pour } k \neq i.
$$

La formule (23) est connue sous le nom de *développement du déterminant de X* suivant la colonne d’indice i. Le scalaire $(-1)^{i+j} \det(X^{ji})$ est appelé le cofacteur d’indices $j$ et $i$ (ou, par abus de langage, le cofacteur de $\xi_{ji}$) dans $X$.

On appelle matrice des cofacteurs de $X$ la matrice
$$
Y = ((-1)^{i+j} \det(X^{ji}))
$$
dont l’élément appartenant à la $j$-ème ligne et la $i$-ème colonne est le cofacteur d’indices $j$ et $i$. Les formules (23) et (24) équivalent à la formule
$$
{}^t Y . X = (\det X) I_n.
$$

Par suite:

#### Proposition 12 {#alg-iii-s8-prop-12 .statement}

*Pour toute matrice carrée inversible $X$ de type $(n, n)$, l’inverse de $X$ est donnée par la formule*
$$
X^{-1} = (\det X)^{-1} \cdot {}^t Y
$$
*où $Y$ est la matrice des cofacteurs de $X$.*

En considérant la *transposée* de $X$ et en utilisant la prop. 8 de III, p. 95, on obtiendrait les développements de Laplace relatifs à deux ensembles complémentaires de lignes, et en particulier, le développement de $\det X$ suivant une ligne; on a ainsi des formules équivalent à
$$
X \cdot {}^t Y = (\det X) I_n,
$$
avec les notations précédentes.

On vérifie aisément que si $X$ est la matrice d’un endomorphisme $u$ d’un A-module libre $M$ de dimension $n$ par rapport à une base $(e_i)_{1 \leq i \leq n}$, ${}^t Y$ est la matrice de l’endomorphisme $\tilde{u}$ de $M$ défini par la condition suivante: quels que soient les $n$ éléments $x, y_2, \ldots, y_n$ de $M$, on a
$$
\tilde{u}(x) \wedge y_2 \wedge \cdots \wedge y_n = x \wedge u(y_2) \wedge \cdots \wedge u(y_n).
$$
On dit que $\tilde{u}$ est le *cotransposé* de $u$ (cf. III, p. 169, corollaire).

#### Exemple 1 {#alg-iii-s8-n6-exa-1 .statement}

*Déterminant de Vandermonde.* Etant donnée une suite $(\zeta_i)_{1 \leq i \leq n}$ de $n$ éléments de $A$, on appelle *déterminant de Vandermonde* de cette suite le déterminant
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
\zeta_1 & \zeta_2 & \ldots & \zeta_n \\
\zeta_1^2 & \zeta_2^2 & \ldots & \zeta_n^2 \\
\vdots & \vdots & \ddots & \vdots \\
\zeta_1^{n-1} & \zeta_2^{n-1} & \ldots & \zeta_n^{n-1}
\end{vmatrix}
$$

Nous allons montrer que l’on a
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \prod_{i < j} (\zeta_j - \zeta_i).
$$

La proposition étant immédiate pour $n = 1$, raisonnons par récurrence sur $n$. Pour chaque indice $k \geq 2$, retranchons de la ligne d’indice $k$ la ligne d’indice k - 1 multipliée par $\zeta_1$; la valeur du déterminant n’est pas modifiée et l’on a donc

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
0 & \zeta_2 - \zeta_1 & \ldots & \zeta_n - \zeta_1 \\
0 & \zeta_2(\zeta_2 - \zeta_1) & \ldots & \zeta_n(\zeta_n - \zeta_1) \\
\ldots & \ldots & \ldots & \ldots \\
0 & \zeta_2^{n-2}(\zeta_2 - \zeta_1) & \ldots & \zeta_n^{n-2}(\zeta_n - \zeta_1)
\end{vmatrix}
$$

d’où, en développant suivant la première colonne, puis mettant en facteur $\zeta_k - \zeta_1$ dans la colonne d’indice $k - 1$ du mineur ainsi obtenu ($2 \leq k \leq n$)

$$
V(\zeta_1, \ldots, \zeta_n) = (\zeta_2 - \zeta_1)(\zeta_3 - \zeta_1) \ldots (\zeta_n - \zeta_1)V(\zeta_2, \ldots, \zeta_n)
$$

ce qui établit (29) par récurrence.

#### Exemple 2 {#alg-iii-s8-n6-exa-2 .statement}

Considérons une matrice carrée d’ordre $n$ qui se présente sous forme d’une « matrice triangulaire supérieure de matrices » (II, p. 152, Exemple IV)

$$
X = \begin{pmatrix} Y & T \\ 0 & Z \end{pmatrix}
$$

Montrons que l’on a

(30) $$
\det X = (\det Y)(\det Z).
$$

Soient $n$ l’ordre de la matrice $X$, $h$ celui de la matrice $Y$, $(e_i)_{1 \leq i \leq n}$ la base canonique de $\mathbf{A}^n$, $x_i$ ($1 \leq i \leq n$) les colonnes de $X$; l’hypothèse entraîne que les colonnes $x_1, \ldots, x_h$ appartiennent au sous-module de $\mathbf{A}^n$ ayant pour base $e_1, \ldots, e_h$ et l’on a par définition (III, p. 92, formule (6))

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_h = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h.
$$

D’autre part, pour tout indice $i > h$, on peut écrire $x_i = y_i + z_i$, où $y_i$ est une combinaison linéaire de $e_1, e_2, \ldots, e_h$ et $z_i$ une combinaison linéaire de $e_{h+1}, \ldots, e_n$. D’après (30), on a $x_1 \wedge x_2 \wedge \cdots \wedge x_h \wedge y_i = 0$ pour tout $i > h$, donc

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)\, e_1 \wedge e_2 \wedge \cdots \wedge e_h \wedge z_{h+1} \wedge \cdots \wedge z_n.
$$

Mais par définition on a

$$
z_{h+1} \wedge z_{h+2} \wedge \cdots \wedge z_n = (\det Z)\, e_{h+1} \wedge e_{h+2} \wedge \cdots \wedge e_n
$$

d’où la formule (30).

Par récurrence sur $p$, on en déduit que si $X$ est sous forme d’une matrice triangulaire supérieure de matrices:

$$
X = \begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
0 & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X_{pp}
\end{pmatrix}
$$

on a

(31) $\det X = (\det X_{11})(\det X_{22}) \ldots (\det X_{pp})$.

Ceci s’applique en particulier à une matrice triangulaire (toutes les $X_{ii}$ étant d’ordre 1) et plus particulièrement à une matrice diagonale:

(32) $\det(\operatorname{diag}(\alpha_1, \alpha_2, \ldots, \alpha_n)) = \alpha_1 \alpha_2 \ldots \alpha_n.$

#### Exemple 3 {#alg-iii-s8-n6-exa-3 .statement}

Soient M, M’ deux A-modules libres de dimensions respectives $n, n'$, u un endomorphisme de M, $u'$ un endomorphisme de M’. Alors on a

(33) $\det(u \otimes u') = (\det u)^{n'} (\det u')^n.$

En effet, on peut écrire $u \otimes u' = (u \otimes 1_{M'}) \circ (1_M \otimes u')$ et on est ramené au cas où l’un des deux endomorphismes $u, u'$ est l’identité. Par exemple si $u' = 1_{M'}$, et si $X$ est la matrice de $u$ par rapport à une base $(e_i)$ de M, alors la matrice de $u \otimes 1_{M'}$ par rapport au produit tensoriel de $(e_i)$ et d’une base de M’ s’écrit comme matrice (à $n'$ lignes et $n'$ colonnes) de matrices à $n$ lignes et $n$ colonnes

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

d’où, en vertu de l’Exemple 2

$$ \det(u \otimes 1_{M'}) = (\det X)^{n'} = (\det u)^{n'} $$

ce qui donne aussitôt la formule (33).

### 7. Application aux équations linéaires

Considérons un système de $n$ équations linéaires scalaires à $n$ inconnues sur un anneau (commutatif) A (II, p. 50):

(34) $\sum_{j=1}^n \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq n).$

Soit $L$ la matrice carrée $(\lambda_{ij})$ d’ordre $n$; en identifiant comme d’ordinaire la matrice à une colonne formée des $\xi_i$ (resp. des $\eta_i$) à l’élément $x = (\xi_i)$ de $\mathbf{A}^n$ (resp. l’élément $y = (\eta_i)$ de $\mathbf{A}^n$), le système (34) s’écrit aussi (II, p. 144, prop. 2)

(35) $L.x = y.$

Soit $u$ l’endomorphisme $x \mapsto L.x$ de $\mathbf{A}^n$, ayant $L$ pour matrice par rapport à la base canonique; dire que l’équation (35) a une solution (au moins) pour tout $y \in \mathbf{A}^n$ signifie que $u$ est surjectif; le th. 1 de III, p. 91 entraîne donc la proposition suivante:

#### Proposition 13 {#alg-iii-s8-prop-13 .statement}

Pour qu’un système de n équations linéaires à n inconnues sur un anneau commutatif admette au moins une solution quels que soient les seconds membres, il faut et il suffit que le déterminant de la matrice du système soit inversible; dans ce cas le système admet une seule solution.

Si det $L$ n’est pas diviseur de zéro dans $A$, l’équation (34) est équivalente à l’équation
$$
(\det L)L.x = (\det L)y.
$$
Si $M$ est la matrice des cofacteurs de $L$, on déduit de (34) et de la formule (26) de III, p. 99, la relation
$$
(\det L)x = {}^tM.y
$$
qui s’écrit aussi
$$
(\det L)\xi_i = \sum_{j=1}^n (-1)^{i+j}(\det L^{ij})\eta_j = \det L_i \quad (1 \leq i \leq n)
$$
en désignant par $L_i$ la matrice obtenue en remplaçant par $y$ la colonne d’indice $i$ de $L$. Les formules (37) s’appellent les *formules de Cramer* pour le système (34); toute solution de (34) est aussi solution de (37). Inversement, on déduit de (36), compte tenu de la formule (28) de III, p. 99,
$$
(\det L)(L.x - y) = 0
$$
donc, si det $L$ n’est pas diviseur de zéro dans $A$, les systèmes (34) et (37) sont *équivalents*; si det $L$ est inversible, l’unique solution de (34) est donnée par
$$
\xi_i = (\det L)^{-1}(\det L_i) \quad (1 \leq i \leq n).
$$
On dit encore qu’un système (34) tel que det $L$ soit inversible est un *système de Cramer*.

Faisons en particulier $y = 0$; il résulte alors de III, p. 91, prop. 3 que:
PROPOSITION 14. — Pour qu’un système linéaire homogène de n équations à n inconnues sur un anneau commutatif admette une solution non nulle, il faut et il suffit que le déterminant de sa matrice soit diviseur de zéro.

### 8. Cas d’un corps commutatif

Tout ce qui précède s’applique lorsque l’anneau $A$ est un corps commutatif; mais il y a des simplifications et l’on peut apporter des compléments.
Ainsi la prop. 12 de III, p. 88 se formule dans ce cas comme suit:

#### Proposition 15 {#alg-iii-s8-prop-15 .statement}

Soit $E$ un espace vectoriel sur un corps commutatif; pour que $p$ vecteurs $x_i \in E$ $(1 \leq i \leq p)$ soient linéairement indépendants, il faut et il suffit que $x_1 \wedge x_2 \wedge \cdots \wedge x_p \neq 0$.

#### Corollaire {#alg-iii-s8-n8-cor-1 .statement}

Soit $X$ une matrice de type $(m, n)$ sur un corps commutatif. Le rang de $X$ est égal au plus grand des entiers $p$ tels qu’il existe au moins un mineur d’ordre $p$ de $X$ qui soit $\neq 0$.

En effet, le rang de $X$ est le nombre maximum des colonnes de $X$ linéairement indépendantes (II, p. 159, déf. 7). Le corollaire résulte donc de la prop. 15, et de la formule (17) de III, p. 96.

Considérons maintenant le cas d’un système de $m$ équations linéaires à $n$ inconnues sur un corps commutatif $K$:

$$
\sum_{j=1}^{n} \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq m).
$$

#### Proposition 16 {#alg-iii-s8-prop-16 .statement}

Soit $L = (\lambda_{ij})$ la matrice (de type $(m, n)$) du système (41). Soit $M$ la matrice de type $(m, n+1)$ obtenue en bordant $L$ par la $(n+1)$-ème colonne $(\eta_i)$ (II, p. 139). Soit $p$ le rang de $L$ (calculé par application du cor. de la prop. 15). Supposons que le mineur $\Delta$ de $L$, déterminant de la matrice obtenue en supprimant les lignes et les colonnes d’indice $\geq p + 1$ dans $L$, soit $\neq 0$ (ce que l’on peut toujours faire au moyen d’une permutation convenable sur les lignes de $L$ et d’une permutation convenable sur les colonnes de $L$). Alors, pour que le système (41) ait au moins une solution, il faut et il suffit que tous les mineurs d’ordre $p + 1$ de $M$, déterminants des sous-matrices d’ordre $p + 1$ de $M$ dont les colonnes ont pour indices $1, 2, \ldots, p$ et $n + 1$, soient nuls. S’il en est ainsi, les solutions du système (41) sont celles du système formé des $p$ premières équations ; si on les écrit

$$
\sum_{j=1}^{p} \lambda_{ij} \xi_j = \eta_i - \sum_{k=p+1}^{n} \lambda_{ik} \xi_k \quad (1 \leq i \leq p)
$$

on obtient toutes les solutions de ce système en prenant pour les $\xi_k$ d’indice $k > p$ des valeurs arbitraires et en appliquant les formules de Cramer (III, p. 102, formules (37)) pour calculer les $\xi_j$ d’indice $j \leq p$.

On sait (II, p. 160, prop. 12) que pour que le système (41) ait au moins une solution, il faut et il suffit que les matrices $L$ et $M$ aient même rang. Les lignes et les colonnes de $L$ ayant été permutées de façon à satisfaire à la condition de l’énoncé, désignons par $a_i$ ($1 \leq i \leq p$) les $p$ premières colonnes de $L$, par $y = (\eta_i)$ la $(n+1)$-ème colonne de $M$; toutes les colonnes de $L$ étant par hypothèse combinaisons linéaires des $a_i$, dire que $M$ a même rang $p$ que $L$ signifie que $y$ est combinaison linéaire des $a_i$, ou encore (III, p. 102, prop. 15) que l’on a $a_1 \wedge \cdots \wedge a_p \wedge y = 0$. La condition de possibilité de l’énoncé est la traduction de cette dernière relation, compte tenu de la formule (17) de III, p. 96. En outre, puisque les $p$ premières lignes de $M$ sont linéairement indépendantes, les lignes d’indice $> p$ en sont des combinaisons linéaires, donc toute solution de (42) est aussi solution de (41). La dernière assertion de l’énoncé est alors une conséquence immédiate de la prop. 13 de III, p. 102.

### 9. Le groupe unimodulaire $\mathbf{SL}(n, A)$

Soit $\mathbf{M}_n(A)$ l’anneau des matrices carrées d’ordre $n$ sur $A$. Considérons l’application $\det : \mathbf{M}_n(A) \to A$. Le groupe $\mathbf{GL}(n, A)$ des éléments inversibles de $\mathbf{M}_n(A)$ (isomorphe au groupe des automorphismes du $A$-module $A^n$ (II, p. 150)) n’est autre que l’image réciproque par cette application du groupe multiplicatif $A^*$ des éléments inversibles de $A$ (III, p. 93, prop. 5). Notons d’autre part que l’application $\det : \mathbf{GL}(n, A) \to A^*$ est un homomorphisme de groupes (III, p. 93, prop. 5).

L’application $\det : \mathbf{M}_n(A) \to A$ est d’ailleurs *surjective* (et par suite il en est de même de l’homomorphisme $\det : \mathbf{GL}(n, A) \to A^*$) : en effet, pour tout $\lambda \in A$, on a $\det(\operatorname{diag}(\lambda, 1, \ldots, 1)) = \lambda$ en vertu de la formule (32) de III, p. 101.

Le *noyau* de l’homomorphisme surjectif $\det : \mathbf{GL}(n, A) \to A^*$ est un sous-groupe distingué de $\mathbf{GL}(n, A)$, qui se compose des matrices *unimodulaires* ; on le note $\mathbf{SL}_n(A)$ ou $\mathbf{SL}(n, A)$ et on l’appelle souvent le *groupe unimodulaire* ou *groupe linéaire spécial* des matrices carrées d’ordre $n$ sur $A$.

Dans ce n° nous allons examiner le cas où $A$ est un *corps*. Rappelons que pour $1 \leq i \leq n, 1 \leq j \leq n$, on note $E_{ij}$ la matrice carrée d’ordre $n$ dont tous les éléments sont nuls sauf celui appartenant à la ligne d’indice $i$ et à la colonne d’indice $j$, qui est égal à 1 ; $I_n$ désignant la matrice unité d’ordre $n$, on pose $B_{ij}(\lambda) = I_n + \lambda E_{ij}$ pour tout couple d’indices *distincts* $i, j$ et tout $\lambda \in A$ (II, p. 161).

#### Proposition 17 {#alg-iii-s8-prop-17 .statement}

*Soit $K$ un corps commutatif. Le groupe unimodulaire $\mathbf{SL}(n, K)$ est engendré par les matrices $B_{ij}(\lambda)$ pour $i \neq j$ et $\lambda \in K$.*

En vertu de II, p. 161, prop. 14, on sait que toute matrice de $\mathbf{GL}(n, K)$ est produit de matrices de la forme $B_{ij}(\lambda)$ et d’une matrice de la forme $\operatorname{diag}(1, 1, \ldots, 1, \alpha)$ avec $\alpha \in K^*$. Or il est immédiat que $\det(B_{ij}(\lambda)) = 1$ et $\det(\operatorname{diag}(1, \ldots, 1, \alpha)) = \alpha$ (III, p. 100, *Exemple 2*) ; d’où la proposition.

#### Corollaire {#alg-iii-s8-n9-cor-1 .statement}

*Le groupe $\mathbf{SL}(n, K)$ est le groupe des commutateurs de $\mathbf{GL}(n, K)$, sauf dans le cas où $n = 2$ et où $K$ est un corps à 2 éléments.*

Comme $\mathbf{SL}(n, K)$ est le noyau de l’homomorphisme $\det$ de $\mathbf{GL}(n, K)$ dans le groupe commutatif $K^*$, $\mathbf{SL}(n, K)$ contient le groupe des commutateurs $\Gamma$ de $\mathbf{GL}(n, K)$ (I, p. 67). Pour prouver que $\mathbf{SL}(n, K) = \Gamma$, il suffira, en vertu de la prop. 17, de montrer que, pour tout $\lambda \in K^*$, $B_{ij}(\lambda)$ appartient à $\Gamma$. Or, $B_{ij}(\lambda)$ est conjugué de $B_{ij}(1)$ dans $\mathbf{GL}(n, K)$ car on a $B_{ij}(\lambda) = Q . B_{ij}(1) . Q^{-1}$, où $Q$ désigne la matrice par rapport à la base canonique $(e_i)$ de l’automorphisme $v$ de $K^n$ tel que $v(e_i) = \lambda e_i, v(e_k) = e_k$ pour $k \neq i$. D’autre part, soit $u_{ij}$ (pour $i \neq j$) l’automorphisme de $K^n$ tel que $u_{ij}(e_i) = -e_j, \ u_{ij}(e_j) = e_i, \ u_{ij}(e_k) = e_k$ pour $k \notin \{i, j\}$, qui appartient à $\mathbf{SL}(n, K)$ ; on a $B_{ji}(\lambda) = U_{ij} B_{ij}(-\lambda) U_{ij}^{-1}$, où $U_{ij}$ est la matrice de $u_{ij}$ par rapport à la base canonique. De même, si $1 < i < j$, on a $B_{1j}(\lambda) = U_{1i} B_{ij}(\lambda) U_{1i}^{-1}$ : et enfin pour $2 < j$, $B_{12}(\lambda) = U_{2j} B_{1j}(\lambda) U_{2j}^{-1}$. Ceci prouve que tous les $B_{ij}(\lambda)$ ont même image $s$ dans $\mathbf{GL}(n, K)/\Gamma$, et il reste à montrer que $s$ est l’élément neutre.

Supposons d’abord que $K$ contienne un élément $\lambda$ distinct de 0 et de 1 ; on a donc $1 = \lambda + (1 - \lambda)$, les deux termes du second membre étant $\neq 0$; la relation $B_{12}(1) = B_{12}(\lambda)B_{12}(1 - \lambda)$ montre que $s^2 = s$, donc $s$ est bien l’élément neutre.

Supposons maintenant que $n \geq 3$. Le produit $B_{21}(1)B_{31}(1)$ est la matrice d’un automorphisme $u$ de $K^n$ tel que $u(e_1) = e_1 + e_2 + e_3, u(e_i) = e_i$ pour $i \neq 1$. Si $S$ est la matrice de l’automorphisme $u'$ de $K^n$ tel que $u'(e_2) = e_2 + e_3, u'(e_i) = e_i$ pour $i \neq 2$, on a $S.B_{21}(1)B_{31}(1).S^{-1} = B_{21}(1)$; on en déduit encore $s^2 = s$, ce qui achève la démonstration.

#### Remarque 1 {#alg-iii-s8-n9-rem-1 .statement}

On a $\mathbf{GL}(2, \mathbf{F}_2) = \mathbf{SL}(2, \mathbf{F}_2)$; c’est un groupe résoluble d’ordre 6, dont le groupe des commutateurs est d’indice 2 (II, p. 208, exerc. 14).

#### Remarque 2 {#alg-iii-s8-n9-rem-2 .statement}

Avec les mêmes notations que ci-dessus, on prouve comme dans I, p. 61, prop. 9 que l’on a, pour $i < j, j - i > 1$, $u_{ij} = u_{j-1,j}u_{i,j-1}u_{j-1,i}^{-1}$; donc le groupe $\mathbf{SL}(n, K)$ est engendré par les matrices $B_{12}(\lambda)$ et $U_{i,i+1}$ pour $1 \leq i \leq n - 1$.

### 10. Le $A[X]$-module associé à un endomorphisme de $A$-module

Soit $M$ un $A$-module, $u$ un endomorphisme de $M$. Considérons l’anneau $A[X]$ des polynômes à une indéterminée $X$ sur $A$. Pour tout polynôme $p \in A[X]$ et tout $x \in M$, posons

$$
p.x = p(u)(x).
$$

Comme $(pq)(u) = p(u) \circ q(u)$ pour deux polynômes $p, q$ de $A[X]$, on définit ainsi sur $M$ une structure de $A[X]$-module; l’ensemble $M$, muni de cette structure, est noté $M_u$; la structure de $A$-module donnée sur $M$ s’obtient par restriction à $A$ de l’anneau d’opérateurs de $M_u$. On notera que les sous-modules de $M_u$ ne sont autres que les sous-modules de $M$ qui sont stables pour $u$.

Comme l’application $(p, x) \mapsto p.x$ de $A[X] \times M$ dans $M$ est $A$-bilinéaire, elle définit canoniquement une application $A$-linéaire $\varphi : A[X] \otimes_A M \to M$ telle que

$$
\varphi(p \otimes x) = p.x = p(u)(x).
$$

D’autre part, $A[X] \otimes_A M$ est canoniquement muni d’une structure de $A[X]$-module (II, p. 81); nous noterons ce $A[X]$-module $M[X]$; l’application $\varphi : M[X] \to M_u$ est $A[X]$-linéaire, car pour $p, q$ dans $A[X]$ et $x \in M$, on a

$$
\varphi(q(p \otimes x)) = \varphi((qp) \otimes x) = (qp).x = q(u)(p(u)(x)) = q.\varphi(p \otimes x).
$$

En outre, $u$ est un $A[X]$-endomorphisme de $M_u$, car on a

$$
u(p.x) = u(p(u)(x)) = (up(u))(x) = p.u(x).
$$

Enfin, on déduit canoniquement de $u$ un $A[X]$-endomorphisme $\bar{u}$ de $M[X]$ en posant (II, p. 82)
$$
\bar{u}(p \otimes x) = p \otimes u(x).
$$
Il résulte d’ailleurs des formules (44) et (45) que les applications $A[X]$-linéaires $u, \bar{u}$ et $\varphi$ sont liées par la relation
$$
\varphi \circ \bar{u} = u \circ \varphi.
$$
Notons $\psi$ le $A[X]$-endomorphisme $X - \bar{u}$ de $M[X]$, de sorte que $\psi(p \otimes x) = (Xp) \otimes x - p \otimes u(x)$. On a la proposition suivante:

#### Proposition 18 {#alg-iii-s8-prop-18 .statement}

*La suite de $A[X]$*-homomorphismes
$$
M[X] \xrightarrow{\psi} M[X] \xrightarrow{\varphi} M_u \longrightarrow 0
$$
*est exacte*.

Comme $\varphi(1 \otimes x) = x$ pour tout $x \in M$, il est clair que $\varphi$ est surjective; d’autre part, on a $\varphi(X(p \otimes x)) = X.\varphi(p \otimes x) = u(\varphi(p \otimes x))$, autrement dit, $\varphi \circ X = u \circ \varphi = \varphi \circ \bar{u}$ en vertu de (46); ceci prouve que $\varphi \circ \psi = 0$. Il reste à voir que $\mathrm{Ker}\ \varphi \subset \mathrm{Im}\ \psi$. Notons pour cela que, puisque les monômes $X^k$ ($k \geqslant 0$) forment une base du $A$-module $A[X]$, tout élément $z \in M[X]$ s’écrit d’une seule manière sous la forme $z = \sum_k X^k \otimes x_{k}$, où $(x_{k})$ est une famille d’éléments de $M$, de support fini. Si $z \in \mathrm{Ker}\ \varphi$, on a $\varphi(z) = \sum_k u^{k}(x_{k}) = 0$, et l’on peut écrire
$$
z = \sum_k (X^k \otimes x_{k} - 1 \otimes u^{k}(x_{k})) = \sum_k (X^k - \bar{u}^k)(1 \otimes x_{k}).
$$
Mais comme les $A[X]$-endomorphismes $X$ et $\bar{u}$ de $M[X]$ sont permutables, on a $X^k - \bar{u}^k = (X - \bar{u}) \circ \left( \sum_{j=0}^{k-1} X^j \bar{u}^{k-j-1} \right)$, ce qui prouve qu’il existe un $y \in M[X]$ tel que $z = \psi(y)$.

Soient maintenant $M'$ un second $A$-module, $u'$ un endomorphisme de $M'$; notons $M'_u, \varphi', \bar{u}', \psi'$ le module et les applications obtenus à partir de $M'$ et $u'$ comme $M_u, \varphi, \bar{u}, \psi$ le sont à partir de $M$ et $u$. Alors:

#### Proposition 19 {#alg-iii-s8-prop-19 .statement}

*Pour qu’une application g de M dans M’ soit un $A[X]$*-homomorphisme de $M_u$ dans $M'_u$, il faut et il suffit que g soit un $A$*-homomorphisme de $M$ dans $M'$ tel que $g \circ u = u' \circ g$. *Lorsqu’il en est ainsi, si $\bar{g}$ est le $A[X]$*-homomorphisme de $M[X]$ dans $M'[X]$ égal à $1_{A[X]} \otimes g$ (II, p. 82), le diagramme
$$
\begin{array}{ccccc}
M[X] & \xrightarrow{\psi} & M[X] & \xrightarrow{\varphi} & M_u \longrightarrow 0 \\
\bar{g} \downarrow & & \bar{g} \downarrow & & g \downarrow \\
M'[X] & \xrightarrow{\psi'} & M'[X] & \xrightarrow{\varphi'} & M'_u \longrightarrow 0
\end{array}
$$
*(48)*
*est commutatif*.

La condition $g \circ u = u' \circ g$ est évidemment nécessaire en vertu de (43) pour que $g$ soit un $A[X]$*-homomorphisme; elle est suffisante, car elle entraîne par récurrence que $g \circ u^n = u^n \circ g$ pour tout entier $n > 0$. D’autre part, pour tout $x \in M$ et tout $p \in A[X]$, on a
$$
\varphi'(\bar{g}(p \otimes x)) = \varphi'(p \otimes g(x)) = p(u')(g(x)) = g(p(u)(x)) = g(\varphi(p \otimes x))
$$
et
$$
\bar{u}'(\bar{g}(p \otimes x)) = \bar{u}'(p \otimes g(x)) = p \otimes u'(g(x)) = p \otimes g(u(x)) = \bar{g}(\bar{u}(p \otimes x))
$$
ce qui prouve la commutativité du diagramme (48).

### 11. Polynôme caractéristique d’un endomorphisme

Soient $M$ un $A$-module libre de dimension $n$, $u$ un endomorphisme de $M$. Considérons l’anneau de polynômes à deux indéterminées $A[X, Y]$ et le $A[X, Y]$-module $M[X, Y] = A[X, Y] \otimes_A M$; soit $\bar{u}$ l’endomorphisme du $A[X, Y]$-module $M[X, Y]$ déduit canoniquement de $u$ (II, p. 82). Il résulte de III, p. 96, prop. 11, que l’on a
$$
\det(X - Y \bar{u}) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j} Y^j
$$
car si $U$ est la matrice de $u$ par rapport à une base $(e_i)_{1 \leq i \leq n}$ de $M$, $U$ est la matrice de $\bar{u}$ par rapport à la base $(1 \otimes e_i)_{1 \leq i \leq n}$ de $M[X, Y]$, donc $\operatorname{Tr}(\wedge^j(\bar{u})) = \operatorname{Tr}(\wedge^j(u))$.

#### Définition 3 {#alg-iii-s8-def-3 .statement}

Soient $M$ un $A$-module libre de dimension finie, $u$ un endomorphisme de $M$. On appelle polynôme caractéristique de $u$ et on note $\chi_u(X)$ le déterminant de l’endomorphisme $X - \bar{u}$ du $A[X]$-module libre $M[X]$.

Si $M$ est de rang $n$, il résulte de (49) que l’on a
$$
\chi_u(X) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j}
$$
car on a $\det(X - Y \bar{u}) = \det(X . I_n - YU)$ et $\det(X - \bar{u}) = \det(X . I_n - U)$. On voit donc que $\chi_u(X)$ est un polynôme unitaire de degré $n$, dans lequel le coefficient de $X^{n-1}$ est $-\operatorname{Tr}(u)$ et le terme constant est $(-1)^n \det(u)$.

#### Proposition 20 (« théorème de Hamilton-Cayley ») {#alg-iii-s8-prop-20 .statement}

Pour tout endomorphisme $u$ d’un $A$-module libre de dimension finie, on a $\chi_u(u) = 0$.

En effet, avec les notations de la prop. 18 (III, p. 106), pour tout $x \in M$, $\chi_u(u)(x)$ est l’image par $\varphi$ de $\chi_u(X) \otimes x$. Mais si $v$ est l’endomorphisme de $M[X]$, cotransposé de $X - \bar{u}$ (III, p. 99), on a
$$
\chi_u(X) \otimes x = \chi_u(X)(1 \otimes x) = (X - \bar{u})(v(1 \otimes x))
$$
et la conclusion résulte de la prop. 18 de III, p. 106.

## EXERCICES {#alg-iii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
