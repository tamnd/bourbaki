---
book: alg
book_title: Algebra
chapter: VII
chapter_title: Modules sur les anneaux principaux
section: 5
section_title: ENDOMORPHISMES DES ESPACES VECTORIELS
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0361-0381, 0399-0426
extraction: ocr
subsections:
    - "no": 1
      title: Le module associé à un endomorphisme
      page: 28
      pdf_page: 361
    - "no": 2
      title: Valeurs propres et vecteurs propres
      page: 29
      pdf_page: 362
    - "no": 3
      title: Invariants de similitude d’un endomorphisme
      page: 30
      pdf_page: 363
    - "no": 4
      title: Endomorphismes trigonalisables
      page: 34
      pdf_page: 367
    - "no": 5
      title: 'Propriétés du polynôme caractéristique : trace et déterminant'
      page: 36
      pdf_page: 369
    - "no": 6
      title: Polynôme caractéristique du produit tensoriel de deux endomorphismes
      page: 38
      pdf_page: 371
    - "no": 7
      title: Endomorphismes diagonalisables
      page: 39
      pdf_page: 372
    - "no": 8
      title: Endomorphismes semi-simples et absolument semi-simples
      page: 41
      pdf_page: 374
    - "no": 9
      title: Décomposition de Jordan
      page: 42
      pdf_page: 375
statements: 65
exercises: 4
content_sha256: f9b4389165b3aff0d28d3f30c5e51547f8dbd83f9fed82d55c0b7cdda6e5fdd0
---

## § 5. ENDOMORPHISMES DES ESPACES VECTORIELS

Notations. — Étant donnés un module M, un élément $x \in M$, et deux endomorphismes $u$ et $v$ de M, nous écrirons dans ce paragraphe $u.x, uv.x, uv$, au lieu de $u(x), (u \circ v)(x), u \circ v$ respectivement ; nous désignerons par 1 l’application identique de M sur lui-même, lorsqu’il n’en résultera pas de confusion.

### 1. Le module associé à un endomorphisme

Soient A un anneau commutatif, M un A-module, $u$ un A-endomorphisme de M. Rappelons (III, p. 105) que l’application $(p(X), x) \mapsto p(u).x$ de $A[X] \times M$ dans M munit M d’une structure de $A[X]$-module, notée $M_u$. Rappelons aussi (III, p. 105 et 106) que si l’on note $M[X]$ le $A[X]$-module obtenu par extension des scalaires du A-module M de A à $A[X]$, et si $\overline{u}$ désigne le $A[X]$-endomorphisme de $M[X]$ déduit de $u$, on a une suite exacte de $A[X]$-modules $^1$

$$
0 \to M[X] \xrightarrow{\psi} M[X] \xrightarrow{\varphi} M_u \to 0,
$$

où $\varphi(p(X) \otimes x) = p(u).x$ et $\psi = X - \overline{u}$.

On dit qu’un endomorphisme $u$ d’un A-module M et un endomorphisme $u'$ d’un A-module $M'$ sont semblables s’il existe un isomorphisme $g$ de M sur $M'$ tel que $u' \circ g = g \circ u$, c’est-à-dire (III, p. 106, prop. 19) un isomorphisme $g$ de $M_u$ sur $M_{u'}$. Si M (resp. $M'$) est libre de base finie B (resp. $B'$), et si $M(u)$ (resp. $M(u')$) est la matrice de $u$ (resp. $u'$) par rapport à B (resp. $B'$), $u$ et $u'$ sont semblables si et seulement si les matrices $M(u)$ et $M(u')$ sont semblables (II, p. 155, déf. 6). Les polynômes caractéristiques (III, p. 107, déf. 3) de deux endomorphismes semblables de modules libres de type fini sont égaux (III, p. 106, prop. 19).

Soit K un corps commutatif ; la donnée d’un couple $(E, u)$ formé d’un espace vectoriel E sur K, et d’un endomorphisme $u$ de E, est donc équivalente à celle du $K[X]$-module $E_u$. Comme l’anneau $K[X]$ est un anneau principal (IV, p. 11, prop. 11), on peut appliquer à $E_u$ les résultats des paragraphes précédents.

Traduisons d’abord certaines notions, du langage des modules dans celui des endomorphismes d’espaces vectoriels :

« V est un sous-module de $E_u$ » signifie : « V est un sous-espace vectoriel de E, stable pour $u$ ».

$^1$ L’injectivité de $\psi$, qui n’est pas énoncée dans la prop. 18 de III, p. 106, se démontre comme suit : avec les notations de loc. cit., on a

$$
\psi(\sum (X^k \otimes x_k)) = \sum X^k \otimes (x_{k-1} - u(x_k)).
$$

Si $\sum X^k \otimes x_k$ appartient au noyau de $\psi$, on a donc $x_{k-1} = u(x_k)$ pour tout $k$, et les $x_k$ sont tous nuls, puisque la famille $(x_k)$ est à support fini.

« V est un sous-module monogène de $E_u$ » signifie : « il existe $x \in V$ tel que le sous-espace vectoriel $V$ soit engendré par les éléments $u^i.x \ (i \in \mathbf{N})$ ». On dit alors que $V$ est *monogène* (pour $u$), et que $x$ en est un générateur.

« V est un sous-module indécomposable de $E_u$ » signifie : « $V$ est non nul et n’est pas somme directe de deux sous-espaces non nuls stables pour $u$. »

« $a$ est l’annulateur du sous-module $V$ » signifie : « $a$ est l’idéal des polynômes $p(X) \in K[X]$ tels que, pour tout $x \in V$, $p(u).x = 0$ ».

Le polynôme unitaire $g$ tel que $a$ soit égal à l’idéal principal ($g$) est appelé le *polynôme minimal* de la restriction de $u$ à $V$.

« $E_u$ est monogène et d’annulateur $a = (g)$ »

$$(\text{avec } g(X) = X^n + \alpha_{n-1}X^{n-1} + \cdots + \alpha_0)$$

signifie : « il existe $x \in E$ tel que $(u^i.x) \ (0 \leq i \leq n-1)$ soit une base de l’espace vectoriel $E$, et que l’on ait $g(u).x = 0$ ». Autrement dit, on peut trouver une base de $E$ telle que la matrice $U$ de $u$ par rapport à cette base soit

$$
U = \begin{pmatrix}
0 & 0 & 0 & \ldots & 0 & -\alpha_0 \\
1 & 0 & 0 & \ldots & 0 & -\alpha_1 \\
0 & 1 & 0 & \ldots & 0 & -\alpha_2 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & \ldots & 0 & -\alpha_{n-2} \\
0 & 0 & 0 & \ldots & 1 & -\alpha_{n-1}
\end{pmatrix}.
$$

« $E_u$ est un module de torsion » signifie d’après la caractérisation des modules de torsion monogènes donnée ci-dessus : « tout sous-module monogène de $E_u$ est de dimension finie sur $K$ ». En particulier :

« $E_u$ est un module de torsion de type fini » signifie : « $E$ est de dimension finie sur $K$ ».

### 2. Valeurs propres et vecteurs propres

#### Définition 1 {#alg-vii-s5-def-1 .statement}

Soient $E$ un espace vectoriel sur un corps commutatif $K$, $u$ un endomorphisme de $E$. On dit qu’un élément $x$ de $E$ est un vecteur propre de $u$ s’il existe $\alpha \in K$ tel que $u.x = \alpha x$; si $x \neq 0$, le scalaire $\alpha$ est appelé valeur propre de $u$ correspondant à $x$. Pour tout scalaire $\alpha$, le sous-espace vectoriel $V_\alpha$ formé des $x \in E$ tels que $u.x = \alpha x$ est appelé le sous-espace propre de $E$ relatif à $\alpha$.

La multiplicité géométrique de la valeur propre $\alpha$ est le cardinal $\dim V_\alpha$.

Supposons $E$ de dimension finie. Les valeurs propres de $u$ sont les éléments $\alpha$ de $K$ tels que l’endomorphisme $\alpha.1 - u$ de $E$ ne soit pas injectif, c’est-à-dire (III, p. 91, prop. 3) tels que det(\alpha .1 - u) = 0. Mais, d’après la définition du polynôme caractéristique $\chi_u$ de $u$ (III, p. 107, déf. 3), on a det(\alpha .1 - u) = $\chi_u(\alpha)$. Par conséquent :

#### Proposition 1 {#alg-vii-s5-prop-1 .statement}

*Supposons E de dimension finie. Pour qu’un élément $\alpha \in \mathbf{K}$ soit valeur propre de l’endomorphisme $u$, il faut et il suffit qu’il soit racine du polynôme caractéristique de $u$.*

Si L est une extension du corps K, les racines de $\chi_u$ dans L sont les valeurs propres de l’endomorphisme $1_L \otimes u$ du L-espace vectoriel $L \otimes_K E$. On dit souvent que ce sont les *valeurs propres de u dans L*. On dit par abus de langage que toutes les valeurs propres de $u$ appartiennent à L s’il en est ainsi de toutes les valeurs propres de $u$ dans une extension algébriquement close de L ; cela signifie donc que $\chi_u$ se décompose dans $L[X]$ en facteurs linéaires.

Soit $U$ une matrice carrée d’ordre $n$ à coefficients dans K. Le polynôme caractéristique de $U$ est par définition

$$
\chi_U(X) = \det(X . I_n - U);
$$

les *valeurs propres* de $U$ (dans une extension L de K) sont les racines (dans L) du polynôme $\chi_U$; ce sont aussi les scalaires $\alpha$ (dans L) tels qu’il existe une solution non nulle du système d’équations linéaires $UX = \alpha X$, où $X$ est une matrice colonne d’ordre $n$; une matrice colonne $X$ satisfaisant à l’équation précédente est appelée un vecteur propre de $U$ relatif à la valeur propre $\alpha$.

Si $U$ est la matrice d’un endomorphisme $u$ d’un espace vectoriel de dimension $n$ par rapport à une base B, on a $\chi_U = \chi_u$, les valeurs propres de $U$ sont les valeurs propres de $u$, et les vecteurs propres de $U$ sont les matrices des vecteurs propres de $u$ par rapport à la base B.

#### Proposition 2 {#alg-vii-s5-prop-2 .statement}

*Soit u un endomorphisme d’un espace vectoriel E sur un corps commutatif K ; pour chaque scalaire $\alpha$, soit $V_\alpha$ le sous-espace propre relatif à $\alpha$. Les sous-espaces $V_\alpha$ sont stables pour u et la somme des sous-espaces $V_\alpha$ est directe.*

La première assertion est claire. Par définition, le sous-espace $V_\alpha$ est annulé par l’élément $X - \alpha$ de $K[X]$; les $X - \alpha, \alpha \in K$, sont extrémaux et deux à deux non associés ; la seconde assertion résulte donc de VII, p. 8, th. 1.

### 3. Invariants de similitude d’un endomorphisme

Si l’on traduit la décomposition d’un module de torsion de type fini qui fait l’objet de VII, p. 8, th. 1 et p. 9, prop. 2, on obtient :

#### Proposition 3 {#alg-vii-s5-prop-3 .statement}

*Soient E un espace vectoriel de dimension finie n sur un corps commutatif K, et u un endomorphisme de E ; pour tout polynôme unitaire irréductible $p(X)$, soit $M_p$ le sous-espace vectoriel formé des éléments x de E tels qu’il existe un entier k pour lequel $(p(u))^k . x = 0$. Alors $M_p$ est stable pour u, E est somme directe des $M_p$, et il existe des polynômes $s_p$ tels que, pour tout $x \in E$, le composant de $x$ dans $M_p$ soit égal à $s_p(u).x$.

#### Remarque 1 {#alg-vii-s5-n3-rem-1 .statement}

Il est clair que le polynôme minimal de la restriction de $u$ à $M_p$ est la plus grande puissance de $p$ qui divise le polynôme minimal de $u$. Par ailleurs, on a $s_p(u).x = x$ pour $x \in M_p$, d’où il résulte aussitôt que, si $M_p \neq 0$, $s_p$ est étranger à $p$.

De même, d’après le th. 2 de VII, p. 19, le module $E_u$ est isomorphe à une somme directe de modules monogènes $F_j = K[X]/a_j$ ($1 \leq j \leq r$), où les idéaux $a_j$ sont distincts de $K[X]$ et tels que $a_j \subset a_{j+1}$; et les $a_j$ sont déterminés par ces conditions. Comme, en outre, $E_u$ est un module de torsion, on a $a_1 \neq (0)$; comme $E$ est de dimension $n$, on a $r \leq n$. Posons $a_j = (h_j)$ ($1 \leq j \leq r$), $h_j$ étant un polynôme unitaire, et considérons la suite de polynômes $(q_i)$ ($1 \leq i \leq n$) définie par :

$$
\left\{
\begin{array}{ll}
q_i(X) = 1 & \text{si } i \leq n - r \\
q_i(X) = h_{n-i+1}(X) & \text{si } n - r < i \leq n .
\end{array}
\right.
$$

Il est clair que la connaissance des polynômes $q_i$ est équivalente à celle des polynômes $h_j$, et que $E_u$ est isomorphe à la somme directe des $n$ modules $K[X]/(q_i)$ ($1 \leq i \leq n$), dont les $n - r$ premiers sont réduits à 0.

En d’autres termes :

#### Proposition 4 {#alg-vii-s5-prop-4 .statement}

Soient $E$ un espace vectoriel de dimension finie $n$ sur un corps commutatif $K$, et $u$ un endomorphisme de $E$. Il existe $n$ polynômes unitaires $q_i(X) \in K[X]$ ($1 \leq i \leq n$) tels que $q_i$ divise $q_{i+1}$ pour $1 \leq i \leq n - 1$, et que $E$ soit somme directe de $n$ sous-espaces $V_i$ ($1 \leq i \leq n$) stables pour $u$, monogènes (pour $u$) et tels que le polynôme minimal de la restriction de $u$ à $V_i$ soit égal à $q_i$ ($1 \leq i \leq n$). Les polynômes $q_i$ sont déterminés de façon unique par ces conditions, et $q_n$ est le polynôme minimal $q$ de $u$.

#### Remarque 2 {#alg-vii-s5-n3-rem-2 .statement}

En vertu de la proposition précédente, il existe une base de $E$ par rapport à laquelle la matrice $U$ de $u$ est de la forme

$$
\begin{pmatrix}
A_{n-r+1} & 0 & \ldots & 0 & 0 \\
0 & A_{n-r+2} & \ldots & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & A_{n-1} & 0 \\
0 & 0 & 0 & 0 & A_n
\end{pmatrix}
$$

chaque matrice $A_i$ étant de la forme (2) (où l’on prend $g(X) = q_i(X)$) (cf. VII, p. 29).

#### Définition 2 {#alg-vii-s5-def-2 .statement}

Les notations étant celles de la prop. 4, les $n$ polynômes unitaires $q_i(X)$ ($1 \leq i \leq n$) sont appelés les invariants de similitude de l’endomorphisme $u$.

Le n-ième invariant de similitude $q_n$ est donc le polynôme minimal de $u$ (prop. 4); autrement dit, pour qu’un polynôme $p(X) \in K[X]$ soit tel que $p(u) = 0$, il faut et il suffit que $p$ soit multiple de $q_n$.

#### Corollaire 1 {#alg-vii-s5-def-2-cor-1 .statement}

Soient $K$ un corps commutatif, $E$ et $E'$ deux espaces vectoriels de dimension finie sur $K$, $u$ (resp. $u'$) un endomorphisme de $E$ (resp. $E'$). Pour que $u$ et $u'$ soient semblables (VII, p. 28), il faut et il suffit qu’ils aient mêmes invariants de similitude.

En effet, $u$ et $u'$ sont semblables si et seulement si les $K[X]$-modules $E_u$ et $E_{u'}$ sont isomorphes.

#### Corollaire 2 {#alg-vii-s5-def-2-cor-2 .statement}

Soient $u$ un endomorphisme d’un espace vectoriel $E$ de dimension finie sur un corps commutatif $K$, $(q_1, \ldots, q_n)$ la famille des invariants de similitude de $u$, $L$ une extension de $K$, $E_{(L)} = L \otimes_K E$ le $L$-espace vectoriel déduit de $E$ par extension des scalaires et $u_{(L)} = 1_L \otimes u$ l’endomorphisme de $E_{(L)}$ déduit de $u$. Les invariants de similitude de $u_{(L)}$ sont les images $\overline{q}_1, \ldots, \overline{q}_n$ de $q_1, \ldots, q_n$ dans $L[X]$.

Cela résulte directement de la proposition 4 et du fait que les $L[X]$-modules $E_{(L), u_{(L)}}$ et $(K[X]/(q_i))_{(L)}$ s’identifient respectivement à $L[X] \otimes_{K[X]} E_u$ et $L[X]/(\overline{q}_i)$.

Soit $U$ une matrice carrée d’ordre $n$ à coefficients dans un corps commutatif $K$. On appelle invariants de similitude de la matrice $U$ les invariants de similitude de l’endomorphisme de $K^n$ défini par $u$. Il résulte alors du cor. 1 précédent que deux matrices carrées sont semblables si et seulement si elles ont mêmes invariants de similitude, et que, si $u$ est un endomorphisme d’un espace vectoriel de dimension finie sur $K$, et $U$ la matrice de $u$ relativement à une base $B$ de $E$, les invariants de similitude de $u$ et $U$ coïncident. D’après les cor. 1 et 2 ci-dessus, on a :

#### Corollaire 3 {#alg-vii-s5-def-2-cor-3 .statement}

Soient $U$ et $V$ deux matrices carrées d’ordre $n$ dont les éléments appartiennent à un corps commutatif $K$. S’il existe une matrice carrée inversible $P$, dont les éléments appartiennent à une extension $K'$ de $K$, et telle que $V = PUP^{-1}$, alors il existe une matrice carrée inversible $Q$, dont les éléments appartiennent à $K$, et telle que $V = QUQ^{-1}$.

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$, $(e_i)_{1 \leq i \leq n}$ une base de $E$ et $u$ un endomorphisme de $E$. D’après la suite exacte (1) de VII, p. 28, le $K[X]$-module $E_u$ associé à $u$ est isomorphe au quotient du $K[X]$-module libre $E[X]$, de base $(1 \otimes e_i)$, par le sous-module $M$ image de $E[X]$ par l’application $K[X]$-linéaire $X - \overline{u}$. Les invariants de similitude $q_i(X)$ de $u$ (VII, p. 31, déf. 2) sont donc les facteurs invariants de $X - \overline{u}$ (VII, p. 21). La prop. 6 de VII, p. 22, entraîne donc :

#### Proposition 5 {#alg-vii-s5-prop-5 .statement}

Soient $E$ un espace vectoriel de dimension finie $n$ sur un corps commutatif $K$, $u$ un endomorphisme de $E$, $U$ sa matrice par rapport à une base quelconque de E. Pour tout entier m tel que $1 \leq m \leq n$, le produit

$$
d_m(X) = q_1(X)\ q_2(X)\ \ldots\ q_m(X)
$$

des m premiers invariants de similitude de u est égal au pgcd des mineurs d’ordre m de la matrice $XI_n - U$.

#### Corollaire 1 {#alg-vii-s5-prop-5-cor-1 .statement}

Soient u un endomorphisme d’un espace vectoriel de dimension finie n sur un corps commutatif K, $\chi_u(X)$ son polynôme caractéristique et $q_i(X)$ ($1 \leq i \leq n$) ses invariants de similitude. On a alors

$$
\chi_u(X) = q_1(X)\ q_2(X)\ \ldots\ q_n(X)\ .
$$

#### Corollaire 2 {#alg-vii-s5-prop-5-cor-2 .statement}

Les notations étant celles du cor. 1, soit $q(X)$ le polynôme minimal de u ; alors $q(X)$ divise $\chi_u(X)$ et $\chi_u(X)$ divise $q(X)^n$. En particulier le polynôme minimal et le polynôme caractéristique de u ont les mêmes racines, qui sont les valeurs propres de u.

Comme $q(X) = q_n(X)$, il est clair que $q(X)$ divise $\chi_u(X)$. D’autre part, puisque chaque $q_i$ divise $q$, leur produit $\chi_u$ divise $q^n$.

#### Corollaire 3 {#alg-vii-s5-prop-5-cor-3 .statement}

Pour qu’un endomorphisme u soit nilpotent, il faut et il suffit que son polynôme caractéristique soit de la forme $X^n$.

Ceci résulte aussitôt du cor. 2.

Traduisons maintenant la prop. 9 de VII, p. 24, donnant la décomposition d’un module en somme directe de sous-modules indécomposables :

#### Proposition 6 {#alg-vii-s5-prop-6 .statement}

Soient E un espace vectoriel de dimension finie n sur un corps commutatif K, et u un endomorphisme de E. Alors E est somme directe de sous-espaces $E_k$, stables pour u, monogènes pour u, tels que le polynôme minimal de la restriction de u à $E_k$ soit de la forme $p_k^{n(k)}$, où $p_k$ est un polynôme irréductible, et que $E_k$ ne puisse être somme directe de deux sous-espaces stables pour u, et non réduits à 0. Pour tout polynôme unitaire irréductible $p \in \mathbf{K}[X]$ et pour tout entier $n \geq 1$, le nombre $m(p^n)$ des sous-espaces $E_k$ d’une telle décomposition tels que $p^n$ soit le polynôme minimal de la restriction de u à $E_k$, est déterminé de façon unique.

La connaissance des $p_k^{n(k)}$ est équivalente à celle des invariants de similitude de u : on passe des uns aux autres par le procédé expliqué en VII, p. 24, remarques 2 et 3. En outre, on passe immédiatement de la décomposition considérée dans la prop. 6 à celles considérées dans les prop. 3 et 4.

On notera que les polynômes unitaires irréductibles $p \in \mathbf{K}[X]$ tels que $m(p^n) > 0$ pour un entier $n \geq 1$, ne sont autres que les facteurs unitaires irréductibles du polynôme minimal de u. Donc, contrairement aux invariants de similitude, ces polynômes dépendent en général du corps K dans lequel on se place.

### 4. Endomorphismes trigonalisables

Dans ce numéro, nous nous intéressons au cas où le polynôme minimal $p(X)$ de $u$ se décompose dans $K[X]$ en produit de facteurs linéaires, c’est-à-dire (VII, p. 33, cor. 2) au cas où toutes les valeurs propres de $u$ appartiennent à $K$. Ce sera en particulier le cas lorsque $K$ est algébriquement clos. La prop. 3 de VII, p. 30, donne aussitôt :

#### Proposition 7 {#alg-vii-s5-prop-7 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$, $u$ un endomorphisme de $E$ dont toutes les valeurs propres sont dans $K$. Pour toute valeur propre $\alpha$ de $u$, soit $M_{\alpha}$ le sous-espace vectoriel de $E$ formé des éléments $x$ pour lesquels il existe un entier $k \geqslant 1$ tel que $(u - \alpha)^k \cdot x = 0$. Alors $M_{\alpha}$ est stable pour $u$, $E$ est somme directe des $M_{\alpha}$, et il existe des polynômes $s_{\alpha} \in K[X]$ tels que, pour tout $x \in E$, le composant de $x$ dans $M_{\alpha}$ soit égal à $s_{\alpha}(u) \cdot x$.

Le sous-module $M_{\alpha}$ étant un $K[X]$-module de type fini, admet alors un annulateur de la forme $(X - \alpha)^r$; autrement dit, il existe un entier $r \geqslant 1$ tel que
$$
(u - \alpha)^r \cdot x = 0
$$
pour tout $x \in M_{\alpha}$; la restriction à $M_{\alpha}$ de $u - \alpha$ est un endomorphisme nilpotent.

Supposant toujours que les valeurs propres de $u$ soient dans $K$, appliquons maintenant à $u$ la prop. 6 de VII, p. 33. Les polynômes $p_k$ ne sont autres que les $X - \alpha$ (où $\alpha$ parcourt l’ensemble des valeurs propres de $u$), et l’on voit que $E$ est somme directe de sous-espaces $E_i$ stables pour $u$, monogènes (pour $u$), et tels que le polynôme minimal de la restriction de $u$ à $E_i$ soit de la forme $(X - \alpha)^m$. Soit $E'_i$ le $K[X]$-module associé à $E_i$; $E'_i$ est donc isomorphe à l’un des modules $K[X]/((X - \alpha)^m)$. Or les classes mod.$(X - \alpha)^m$ des éléments $(X - \alpha)^k$ ($0 \leqslant k \leqslant m - 1$) forment une base de $K[X]/((X - \alpha)^m)$ par rapport à $K$ (IV, p. 10, cor.), et l’on a
$$
X(X - \alpha)^k = \alpha(X - \alpha)^k + (X - \alpha)^{k+1}
$$
pour $0 \leqslant k \leqslant m - 1$; on en déduit que si $E_i$ est de dimension $m$, et si $\alpha$ est l’unique valeur propre de la restriction $u_i$ de $u$ à $E_i$, il existe une base de $E_i$ par rapport à laquelle la matrice de $u_i$ est la matrice d’ordre $m$

$$
U_{m,\alpha} = \begin{pmatrix}
\alpha & 0 & 0 & \ldots & 0 & 0 \\
1 & \alpha & 0 & \ldots & 0 & 0 \\
0 & 1 & \alpha & \ldots & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & \ldots & \alpha & 0 \\
0 & 0 & 0 & \ldots & 1 & \alpha
\end{pmatrix}.
$$

#### Définition 3 {#alg-vii-s5-def-3 .statement}

Pour tout corps $K$, tout entier $m \geqslant 1$ et tout $\alpha \in K$, la matrice $U_{m,\alpha}$ est dite matrice de Jordan d’ordre $m$ de valeur propre $\alpha$.

#### Proposition 8 {#alg-vii-s5-prop-8 .statement}

Soient E un espace vectoriel de dimension finie sur un corps commutatif K, u un endomorphisme de E. Les conditions suivantes sont équivalentes :
(i) les valeurs propres de u (dans une extension algébriquement close de K) appartiennent à K ;
(ii) il existe une base de E par rapport à laquelle la matrice de u est triangulaire inférieure (resp. supérieure) ;
(iii) il existe une base de E par rapport à laquelle la matrice de u est un tableau diagonal de matrices de Jordan.
On a (i) ⇒ (iii) d’après la prop. 7 et les remarques précédentes, et les assertions (iii) ⇒ (ii) et (ii) ⇒ (i) sont triviales.

#### Définition 4 {#alg-vii-s5-def-4 .statement}

On appelle trigonalisables les endomorphismes satisfaisant aux conditions (i), (ii), (iii) de la prop. 8.

En particulier, si K est algébriquement clos, tout endomorphisme d’un K-espace vectoriel de dimension finie est trigonalisable.
Pour des matrices, la prop. 8 entraîne :

#### Corollaire {#alg-vii-s5-n4-cor-1 .statement}

Soit U une matrice carrée sur un corps commutatif K telle que toutes les valeurs propres de U soient dans K ; il existe une matrice semblable à U et qui est un tableau diagonal de matrices de Jordan.

#### Remarque 1 {#alg-vii-s5-n4-rem-1 .statement}

Il résulte de la prop. 6 de VII, p. 33, que, si U est semblable à un tableau diagonal de matrices de Jordan (J_k), le nombre des J_k de la forme U_{m,\alpha} (pour m et α donnés) est déterminé de façon unique par U.
2) Plus généralement, si U est semblable à un tableau diagonal de matrices de Jordan U_{m_i,\alpha_i} on calcule immédiatement les invariants de similitude de U par une méthode calquée sur celle exposée en VII, p. 24, remarque 3 : on écrit sur une même ligne les (X − α_i)^{m_i} relatifs à un même α par ordre décroissant des exposants, et on complète par des 1, pour avoir des lignes de longueur égale à l’ordre de U ; ceci fait, on obtient les invariants de similitude de U, rangés dans l’ordre des indices décroissants, en formant les produits des termes qui sont dans une même colonne. Par exemple, pour la matrice

$$
\begin{pmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 1 & 3
\end{pmatrix}
$$

on écrit

(X − 2), 1, 1
(X − 3)^2, 1, 1

et les invariants de similitude sont 1,1, et (X − 2)(X − 3)^2.

En remarquant que le polynôme minimal de la matrice de Jordan U_{m,\alpha} est (X − α)^m et qu’il est égal à son polynôme caractéristique, on obtient le résultat suivant :

#### Proposition 9 {#alg-vii-s5-prop-9 .statement}

Si la matrice carrée U est semblable à un tableau diagonal de matrices de Jordan (U_{m_i,\alpha_i}), le polynôme minimal de U est le ppcm des (X − α_i)^{m_i}, le polynôme caractéristique de U est le produit des (X − α_i)^{m_i}.

#### Corollaire {#alg-vii-s5-n4-cor-2 .statement}

Avec les notations de la prop. 7, la dimension du sous-espace $M_\alpha$ est la multiplicité de la valeur propre $\alpha$ comme racine du polynôme caractéristique de $u$.

### 5. Propriétés du polynôme caractéristique : trace et déterminant

Soient $E$ un espace vectoriel de dimension finie $n$ sur un corps commutatif $K$, et $u$ un endomorphisme de $E$. D’après III, p. 107, le polynôme caractéristique de $u$ est de la forme :

$$
\chi_u(X) = X^n - \operatorname{Tr}(u)\ X^{n-1} + \cdots + (-1)^n \det(u) .
$$

#### Proposition 10 {#alg-vii-s5-prop-10 .statement}

Soient $E$ un espace vectoriel de dimension finie $n$ sur un corps commutatif $K$, $u$ un endomorphisme de $E$, et $\chi_u(X) = \prod_{i=1}^n (X - \alpha_i)$ une décomposition en facteurs linéaires de son polynôme caractéristique (dans une extension convenable de $K$, cf. V, p. 21). Si $q$ est un polynôme à coefficients dans $K$, le polynôme caractéristique de $q(u)$ est donné par

$$
\chi_{q(u)}(X) = \prod_{i=1}^n (X - q(\alpha_i)) ,
$$

sa trace et son déterminant par

$$
\operatorname{Tr}(q(u)) = \sum_{i=1}^n q(\alpha_i) ,
$$
$$
\det(q(u)) = \prod_{i=1}^n q(\alpha_i) .
$$

Il est clair que (7) et (8) résultent de (6) en vertu de (5). Pour prouver la formule (6), on peut supposer $K$ algébriquement clos. Prenons alors une base de $E$ par rapport à laquelle la matrice $U$ de $u$ est triangulaire inférieure (VII, p. 35, cor. à la prop. 8) ; nous nous appuierons sur le lemme immédiat suivant :

#### Lemme 1 {#alg-vii-s5-lem-1 .statement}

Si $B$ et $C$ sont des matrices triangulaires inférieures d’ordre $n$ et de diagonales $(\beta_i)$ et $(\gamma_i)$, les matrices $B + C$ et $BC$ sont triangulaires inférieures et ont pour diagonales $(\beta_i + \gamma_i)$ et $(\beta_i \gamma_i)$.

Comme la matrice $U$ de $u$ est une matrice triangulaire de diagonale $(\alpha_i)$, il résulte du lemme 1 que $q(U)$ est une matrice triangulaire de diagonale $(q(\alpha_i))$. Alors $X.I_n - q(U)$ est une matrice triangulaire de diagonale $(X - q(\alpha_i))$, ce qui démontre (6).

#### Corollaire 1 {#alg-vii-s5-lem-1-cor-1 .statement}

Pour que $q(u)$ soit inversible, il faut et il suffit que $q$ soit étranger à $\chi_u$.

En effet, dire que $q$ et $\chi_u$ sont étrangers équivaut à dire qu’ils n’ont pas de racine commune dans une extension algébriquement close de $K$, c’est-à-dire, d’après (8), que $\det(q(u)) \neq 0$.

#### Remarque 1 {#alg-vii-s5-n5-rem-1 .statement}

Être étranger à $\chi_u$ équivaut à être étranger au polynôme minimal de $u$ (VII, p. 33, cor. 2).

#### Corollaire 2 {#alg-vii-s5-lem-1-cor-2 .statement}

Soit $r \in K(X)$ une fraction rationnelle sur $K$. Pour que $u$ soit substituable dans $r$ (IV, p. 20) il faut et il suffit que chacune des valeurs propres $\alpha_i$ de $u$ le soit. Lorsqu’il en est ainsi, on a les formules :

$$
\chi_{r(u)}(X) = \prod_{i=1}^n (X - r(\alpha_i)) , \quad \operatorname{Tr}(r(u)) = \sum_{i=1}^n r(\alpha_i) , \quad \det(r(u)) = \prod_{i=1}^n r(\alpha_i) .
$$

Écrivons $r = p/q$, où $p$ et $q$ sont des polynômes étrangers. Pour que $u$ soit substituable dans $r$, il faut et il suffit que $\det(q(u)) \neq 0$, d’où la première assertion en vertu de la formule (8). Supposons donc, en vertu du cor. 1, que $q$ soit étranger à $\chi_u$. D’après l’identité de Bezout, il existe des polynômes $g$ et $h$ tels que $qg + h\chi_u = 1$. On a alors $q(\alpha_i)\, g(\alpha_i) = 1$, et $q(u)\, g(u) = 1$ en vertu du théorème de Hamilton-Cayley (III, p. 107). Il suffit alors d’appliquer les formules (6), (7) et (8) à $p(u)\, g(u) = r(u)$ pour obtenir les formules annoncées.

#### Corollaire 3 {#alg-vii-s5-lem-1-cor-3 .statement}

Pour tout entier $s \geq 0$, on a $\operatorname{Tr}(u^s) = \sum_{i=1}^n \alpha_i^s$; cette formule est valable pour $s < 0$ pourvu que $u$ soit inversible.

Ceci est un cas particulier du corollaire précédent.

#### Corollaire 4 {#alg-vii-s5-lem-1-cor-4 .statement}

Supposons le corps $K$ de caractéristique nulle ; pour que l’endomorphisme $u$ soit nilpotent, il faut et il suffit que l’on ait $\operatorname{Tr}(u^s) = 0$ pour $1 \leq s \leq n$.

Si $u$ est nilpotent, les $\alpha_i$ sont nuls, et l’on a $\operatorname{Tr}(u^s) = 0$ pour tout $s > 0$ (cor. 3). Si, réciproquement, on a $\operatorname{Tr}(u^s) = 0$ pour $1 \leq s \leq n$, les $\alpha_i$ sont nuls puisque $K$ est de caractéristique nulle (IV, p. 67, cor.), et $u$ est nilpotent (VII, p. 33).

#### Corollaire 5 {#alg-vii-s5-lem-1-cor-5 .statement}

Soit $Y$ une indéterminée. Notons $\tilde{u}$ l’endomorphisme du $K(Y)$-espace vectoriel $K(Y) \otimes_K E$ déduit de $u$ par extension des scalaires de $K$ au corps $K(Y)$ des fractions rationnelles en $Y$ à coefficients dans $K$. L’endomorphisme $Y.1 - \tilde{u}$ est inversible. En outre, si $\chi'_u$ désigne la dérivée du polynôme $\chi_u$, on a

$$
\operatorname{Tr}((Y.1 - \tilde{u})^{-1}) = \chi'_u(Y)/\chi_u(Y) .
$$

L’endomorphisme $Y.1 - \tilde{u}$ est inversible, puisque son déterminant est l’élément non nul $\chi_u(Y)$ de $K(Y)$. Il s’ensuit que $\tilde{u}$ est substituable dans la fraction rationnelle $r(X) = (Y - X)^{-1}$ de $K(Y)(X)$. La seconde assertion résulte alors du cor. 2, compte tenu de la relation

$$
\chi'_u(Y)/\chi_u(Y) = \sum_i (Y - \alpha_i)^{-1} = \sum_i r(\alpha_i) .
$$

#### Corollaire 6 {#alg-vii-s5-lem-1-cor-6 .statement}

Supposons le corps $\mathbf{K}$ de caractéristique nulle. Dans l’anneau de séries formelles $\mathbf{K}[[T]]$, on a

$$
- T \frac{d}{dT} \log \det(1 - Tu) = \sum_{m \geq 1} \operatorname{Tr}(u^m) T^m .
$$

Plaçons-nous d’abord dans le corps de fractions rationnelles $\mathbf{K}(T)$, et posons $P(T) = \det(I_n - T \cdot U)$, où $U$ est la matrice de $u$ relativement à une base de $E$. On a

$$
P(T) = \det(T(T^{-1} \cdot I_n - U)) = T^n \chi_U(T^{-1}) ,
$$
donc $P'(T)/P(T) = n/T - \chi'_U(T^{-1})/T^2 \chi_U(T^{-1})$. Par ailleurs, d’après le cor. 5, on a

$$
\chi'_U(T^{-1})/T \chi_U(T^{-1}) = \operatorname{Tr}((T^{-1} \cdot I_n - U)^{-1})/T = \operatorname{Tr}((I_n - T \cdot U)^{-1}) .
$$

On en tire $- TP'(T)/P(T) = -n + \operatorname{Tr}((I_n - TU)^{-1})$. Prenant le développement en série formelle des deux membres de cette égalité, on obtient le corollaire.

#### Remarque 2 {#alg-vii-s5-n5-rem-2 .statement}

D’après IV, p. 75, cor. 1 et la formule (8), on a, pour tout polynôme $q \in \mathbf{K}[X]$

$$
\det q(u) = \operatorname{res}(\chi_u, q) ,
$$
où $\operatorname{res}(\chi_u, q)$ est le résultant des polynômes $\chi_u$ et $q$. En particulier, si l’on prend $q = \chi'_u$, on obtient

$$
\det \chi'_u(u) = (-1)^{n(n-1)/2} \operatorname{dis}(\chi_u) ,
$$
où $\operatorname{dis}(\chi_u)$ est le discriminant du polynôme $\chi_u$ (IV, p. 78, formule (47)). De plus :

#### Corollaire 7 {#alg-vii-s5-lem-1-cor-7 .statement}

On a $\det(\operatorname{Tr}(u^{i+j})_{0 \leq i,j \leq n-1}) = \operatorname{dis}(\chi_u)$.

Soit $D$ la matrice de Vandermonde $(\alpha_j^{i-1})_{1 \leq i,j \leq n}$. On a (III, p. 99, formule (29))

$$
\det(D)^2 = \prod_{i < j} (\alpha_i - \alpha_j)^2 = \operatorname{dis}(\chi_u) .
$$

Par ailleurs, le terme d’indices $(i, j)$ de $D \cdot {}^tD$ est $\sum_k \alpha_k^{i+j-2} = \operatorname{Tr}(u^{i+j-2})$, d’où le corollaire.

### 6. Polynôme caractéristique du produit tensoriel de deux endomorphismes

#### Proposition 11 {#alg-vii-s5-prop-11 .statement}

Soient $E$ (resp. $E'$) un espace vectoriel de dimension finie sur un corps commutatif $\mathbf{K}$, $u$ (resp. $u'$) un endomorphisme de $E$ (resp. $E'$). Soient

$$
\chi_u(X) = \prod_i (X - \alpha_i) , \quad \chi_{u'}(X) = \prod_j (X - \beta_j)
$$
des décompositions en facteurs linéaires des polynômes caractéristiques de $u$ et $u'$

dans une extension convenable de $K$. Alors le polynôme caractéristique de l’endomorphisme $u \otimes u'$ de l’espace vectoriel $E \otimes_K E'$ est donné par la formule

$$
\chi_{u \otimes u'}(X) = \prod_{i,j} (X - \alpha_i \beta_j) .
$$

Raisonnant comme dans la démonstration de la prop. 10 de VII, p. 36, on voit qu’il suffit de démontrer le lemme suivant :

#### Lemme 2 {#alg-vii-s5-lem-2 .statement}

Soient $B$ et $C$ deux matrices triangulaires inférieures d’ordres respectifs $m$ et $n$ et de diagonales $(\beta_i)_{1 \leq i \leq m}$, $(\gamma_j)_{1 \leq j \leq n}$. Identifions le produit lexicographique des ensembles ordonnés $\{1, 2, ..., m\}$ et $\{1, 2, ..., n\}$ à l’intervalle $\{1, 2, ..., mn\}$. Alors la matrice produit tensoriel (II, p. 157) $B \otimes C$ est triangulaire inférieure de diagonale $(\beta_i \gamma_j)$.

Cela résulte aussitôt de la définition du produit tensoriel de deux matrices (*loc. cit.*) et du produit lexicographique (E, III, p. 23).

### 7. Endomorphismes diagonalisables

#### Définition 5 {#alg-vii-s5-def-5 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$ et $\mathfrak{F}$ un ensemble d’endomorphismes de $E$. On dit que $\mathfrak{F}$ est diagonal par rapport à une base $(e_i)$ de $E$ si les matrices de tous les $u \in \mathfrak{F}$ par rapport à $(e_i)$ sont diagonales. On dit que $\mathfrak{F}$ est diagonalisable s’il existe une base de $E$ telle que $\mathfrak{F}$ soit diagonal par rapport à cette base.

Cette définition s’applique en particulier au cas où $\mathfrak{F}$ est réduit à un élément $u$; on dit alors que $u$ est diagonal (diagonalisable). Notons aussi que $\mathfrak{F}$ est diagonal par rapport à une base $(e_i)$ si et seulement si les $(e_i)$ sont des vecteurs propres communs aux éléments de $\mathfrak{F}$; il en résulte que $\mathfrak{F}$ est diagonalisable si et seulement si $E$ est engendré par les vecteurs propres communs aux éléments de $\mathfrak{F}$.

Soit $A$ une sous-algèbre de $\mathrm{End}_K(E)$ contenant $\mathrm{Id}_E$. Alors $A$ est diagonalisable si et seulement si elle est isomorphe à une algèbre $K'$ (c’est-à-dire est diagonalisable au sens de V, p. 28, déf. 1); en effet, si $A$ est isomorphe à $K'$, alors $A$ est diagonalisable d’après V, p. 28, prop. 1; inversement, si $A$ est diagonalisable, elle est isomorphe à une sous-algèbre de l’algèbre des matrices diagonales, algèbre qui est isomorphe à $K^n, n = \dim(E)$, donc $A$ est isomorphe à une algèbre $K'$ (V, p. 29, prop. 3).

#### Proposition 12 {#alg-vii-s5-prop-12 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$ et $u$ un endomorphisme de $E$. Les conditions suivantes sont équivalentes :
(i) $u$ est diagonalisable.
(ii) $E$ est somme directe des sous-espaces propres de $u$.
(iii) Le polynôme minimal de $u$ a toutes ses racines dans $K$, et ces racines sont simples.

De plus, si ces conditions sont satisfaites, tout sous-espace de $E$ stable pour $u$ est somme directe de ses intersections avec les sous-espaces propres de $u$.

L’équivalence de (i) et (ii) résulte des remarques qui précèdent et de VII, p. 30, prop. 2. Supposons $u$ diagonalisable, et soit $(\alpha_i)$ la famille des valeurs propres de $u$ et $(V_i)$ la famille des sous-espaces propres correspondants ; comme la restriction de $u$ à $V_i$ est l’homothétie de rapport $\alpha_i$, elle annule le polynôme $X - \alpha_i$; il s’ensuit que $u$ annule le polynôme $\prod_i (X - \alpha_i)$ qui est donc un multiple du polynôme minimal, donc coïncide avec celui-ci, ce qui démontre (iii). Inversement, si (iii) est satisfaite, il existe une base de $E$ par rapport à laquelle la matrice $U$ de $u$ est un tableau diagonal de matrices de Jordan $U_{m,\alpha}$ (VII, p. 35, prop. 8); alors d’après la prop. 9, tous les entiers $m$ sont égaux à 1 et $U$ est diagonale. Enfin, la dernière assertion résulte de ce que, si $u$ est diagonalisable, les sous-espaces propres sont les composants primaires de $E_u$ et de VII, p. 8, cor. 1.

#### Corollaire {#alg-vii-s5-n7-cor-1 .statement}

*Si le polynôme caractéristique de $u$ a toutes ses racines dans $K$, et si elles sont simples, $u$ est diagonalisable.*
En effet le polynôme minimal divise le polynôme caractéristique.

#### Proposition 13 {#alg-vii-s5-prop-13 .statement}

*Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$, $\mathfrak{F}$ un ensemble d’endomorphismes de $E$, et $A$ la sous-algèbre de $\mathrm{End}_K(E)$ engendrée par $\mathfrak{F}$ et $\mathrm{Id}_E$. Les conditions suivantes sont équivalentes :
(i) $\mathfrak{F}$ est diagonalisable.
(ii) La $K$-algèbre $A$ est diagonalisable.
(iii) Les éléments de $\mathfrak{F}$ sont diagonalisables et deux à deux permutables.*
Si $(e_i)$ est une base de $E$ par rapport à laquelle $\mathfrak{F}$ est diagonal, alors $A$ est contenu dans l’algèbre des endomorphismes diagonaux par rapport à cette base, donc est aussi diagonalisable; si $A$ est diagonalisable, le même raisonnement montre que $\mathfrak{F}$ est diagonalisable. Cela montre l’équivalence de (i) et (ii). Comme deux matrices diagonales sont permutables, on a (i) $\Rightarrow$ (iii) et il reste à prouver la réciproque. Supposons donc les éléments de $\mathfrak{F}$ diagonalisables et deux à deux permutables. Nous utiliserons le lemme suivant :

*Lemme 3. — Soient $g$ et $h$ deux endomorphismes permutables d’un espace vectoriel $E$. Tout sous-espace propre de $g$ est stable pour $h$.
En effet, si $W_\lambda$ est le sous-espace propre de $g$ relatif à la valeur propre $\lambda$, la relation $x \in W_\lambda$ entraîne
$$
gh.x = hg.x = h.\lambda x = \lambda h.x,
$$
ce qui exprime que $h.x \in W_\lambda$.

Revenons à la démonstration de la prop. 13. Parmi toutes les décompositions de $E$ en somme directe de sous-espaces non nuls stables pour tous les éléments de $\mathfrak{F}$, choisissons-en une qui ait le nombre maximum d’éléments (ce nombre est majoré par la dimension de $E$), soit $E = \sum_{i \in I} E_i$. Soit $u \in \mathfrak{F}$ et soit $E = \sum_\alpha V_\alpha$ la décomposition de $E$ en somme directe des sous-espaces propres de $u$. D’après le lemme 3, chacun des $V_\alpha$ est stable pour $\mathfrak{F}$, donc aussi chacun des $V_\alpha \cap E_i$; d’après la prop. 12, chaque

E_i est somme directe des $V_\alpha \cap E_i$. Le choix des $E_i$ impose donc que chaque $E_i$ soit contenu dans un des $V_\alpha$; la restriction de $u$ à chacun des $E_i$ est donc une homothétie. Comme cela est vrai pour tous les éléments de $\mathfrak{F}$, $\mathfrak{F}$ est diagonalisable.

#### Corollaire {#alg-vii-s5-n7-cor-2 .statement}

*La somme et le composé de deux endomorphismes diagonalisables permutables de E sont diagonalisables.*

### 8. Endomorphismes semi-simples et absolument semi-simples

#### Définition 6 {#alg-vii-s5-def-6 .statement}

*Soit E un espace vectoriel de dimension finie sur un corps commutatif K. Un endomorphisme u de E est dit semi-simple si tout sous-espace de E stable pour u possède un supplémentaire stable pour u.*

Cela signifie donc que tout sous-module du K[X]-module $E_u$ est facteur direct, c’est-à-dire que le K[X]-module $E_u$ est semi-simple (VII, p. 9).

#### Proposition 14 {#alg-vii-s5-prop-14 .statement}

*Pour qu’un endomorphisme u d’un espace vectoriel de dimension finie sur un corps commutatif soit semi-simple, il faut et il suffit que le polynôme minimal de u soit sans facteur multiple.*
Cela résulte aussitôt de VII, p. 9, cor. 4 et p. 31, remarque 1.

Soient E un espace vectoriel sur un corps commutatif K, L une extension de K, et $u$ un endomorphisme de E ; on note $u_{(L)}$ le L-endomorphisme $1_L \otimes u$ du L-espace vectoriel $E_{(L)} = L \otimes_K E$ déduit de E par extension des scalaires. De même, si $\mathfrak{F}$ est un ensemble d’endomorphismes de E, on note $\mathfrak{F}_{(L)}$ l’ensemble des $u_{(L)}$, pour $u$ dans $\mathfrak{F}$.

#### Corollaire {#alg-vii-s5-n8-cor-1 .statement}

*Soient u un endomorphisme d’un espace vectoriel de dimension finie sur un corps commutatif K et L une extension de K. Si $u_{(L)}$ est semi-simple, u est semi-simple. Si u est semi-simple et L séparable sur K, $u_{(L)}$ est semi-simple.*
Cela résulte aussitôt de la prop: 14 et de V, p. 115, cor. 1 (noter que les polynômes minimaux de $u$ et $u_{(L)}$ coïncident).

#### Proposition 15 {#alg-vii-s5-prop-15 .statement}

*Soient E un espace vectoriel de dimension finie sur un corps commutatif K, u un endomorphisme de E et q(X) son polynôme minimal. Les conditions suivantes sont équivalentes :
(i) Pour toute extension L de K, l’endomorphisme $u_{(L)}$ est semi-simple.
(ii) Il existe une extension L de K telle que l’endomorphisme $u_{(L)}$ soit diagonalisable.
(iii) Le polynôme q(X) est séparable sur K.*
En effet, la condition (i) signifie que le polynôme $1 \otimes q(X)$ de L[X] est sans facteur multiple pour toute extension L de K (prop. 14), la condition (ii) signifie qu’il existe une extension L de K telle que $q(X)$ ait toutes ses racines dans L et qu’elles soient simples (VII, p. 39, prop. 12), et ces conditions équivalent à (iii) par définition (V, p. 37).

#### Définition 7 {#alg-vii-s5-def-7 .statement}

Un endomorphisme u satisfaisant aux conditions (i), (ii) et (iii) de la prop. 15 est dit absolument semi-simple.

#### Corollaire {#alg-vii-s5-n8-cor-2 .statement}

Pour que u soit absolument semi-simple, il faut et il suffit qu’il existe une extension L de K, qui soit un corps parfait, et telle que $u_{(L)}$ soit semi-simple.

En effet, la condition du corollaire signifie qu’il existe une extension L de K, qui soit un corps parfait, telle que $q(X)$ soit sans facteur multiple dans L[X] (prop. 14) ; cette condition équivaut à (iii) d’après V, p. 37, cor. 2.

#### Proposition 16 {#alg-vii-s5-prop-16 .statement}

Soient E un espace vectoriel de dimension finie sur un corps commutatif K, $\mathfrak{F}$ un ensemble d’endomorphismes de E, A la sous-algèbre de $\mathrm{End}_K(E)$ engendrée par $\mathfrak{F}$ et $\mathrm{Id}_E$. Les conditions suivantes sont équivalentes :
(i) Il existe une extension L de K telle que $\mathfrak{F}_{(L)}$ soit diagonalisable.
(ii) La K-algèbre A est étale (V, p. 28, déf. 1).
(iii) Les éléments de $\mathfrak{F}$ sont absolument semi-simples et deux à deux permutables.

Notons d’abord que, pour toute extension L de K, la L-algèbre engendrée par $\mathfrak{F}_{(L)}$ et $\mathrm{Id}_{E(L)}$ coïncide avec $L \otimes_K A$ ; d’après la prop. 13, $\mathfrak{F}_{(L)}$ est donc diagonalisable si et seulement si la L-algèbre $L \otimes_K A$ est diagonalisable. L’équivalence des conditions (i) et (ii) résulte donc de V, p. 28, déf. 1. D’autre part, on a aussitôt (i) $\Rightarrow$ (iii). Supposons enfin (iii) vérifiée, et soit L une clôture algébrique de K ; les éléments de $\mathfrak{F}_{(L)}$ sont diagonalisables (VII, p. 39, prop. 12) et deux à deux permutables ; $\mathfrak{F}_{(L)}$ est donc diagonalisable d’après VII, p. 40, prop. 13.

#### Corollaire {#alg-vii-s5-n8-cor-3 .statement}

La somme et le produit de deux endomorphismes permutables et absolument semi-simples sont absolument semi-simples.

#### Remarque {#alg-vii-s5-n8-rem-1 .statement}

Supposons les conditions de la prop. 16 vérifiées et soit L une extension de K. D’après la prop. 13, l’ensemble $\mathfrak{F}_{(L)}$ est diagonalisable si et seulement si l’algèbre $L \otimes_K A$ est diagonalisable. On en conclut par V, p. 29, prop. 2, qu’il existe une extension finie L de K telle que $\mathfrak{F}_{(L)}$ soit diagonalisable. En fait, on peut même supposer L galoisienne ; en effet, prenant une partie finie $\mathfrak{F}'$ de $\mathfrak{F}$ qui engendre A, on peut prendre pour L un corps de décomposition des polynômes minimaux des éléments de $\mathfrak{F}'$ (prop. 12 et 13).

### 9. Décomposition de Jordan

#### Définition 8 {#alg-vii-s5-def-8 .statement}

Soient E un espace vectoriel de dimension finie sur un corps commutatif et u un endomorphisme de E. On appelle décomposition de Jordan de u un couple $(u_s, u_n)$, où $u_s$ est un endomorphisme absolument semi-simple de E et $u_n$ un endomorphisme nilpotent de E, tels que $u_s u_n = u_n u_s$ et $u = u_s + u_n$.

#### Théorème 1 {#alg-vii-s5-thm-1 .statement}

Soient E un espace vectoriel de dimension finie sur un corps commutatif K et u un endomorphisme de E. Pour que u possède une décomposition de Jordan $(u_s, u_n)$, il faut et il suffit que les valeurs propres de u soient séparables sur K. De plus, celle-ci est uniquement déterminée, les polynômes caractéristiques de u et $u_s$ coïncident, et il existe des polynômes $P, Q \in K[X]$, sans terme constant, tels que $u_s = P(u)$, $u_n = Q(u)$.

A) Démontrons d’abord le cas particulier suivant :

#### Lemme 4 {#alg-vii-s5-lem-4 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$ et $u$ un endomorphisme trigonalisable de $E$. Il existe un endomorphisme diagonalisable $v$ de $E$, et un seul, qui commute à $u$ et soit tel que $u - v$ soit nilpotent. De plus, sous ces conditions, les polynômes caractéristiques de $u$ et $v$ coïncident, et il existe un polynôme $P \in K[X]$ tel que $v = P(u)$.

Soit $v$ un endomorphisme diagonalisable de $E$ tel que $uv = vu$ et que $v - u$ soit nilpotent ; soit $\alpha$ une valeur propre de $v$ et soit $V_\alpha$ le sous-espace propre correspondant. D’après le lemme 3 (VII, p. 40), $V_\alpha$ est stable pour $u$, et la restriction de $u - \alpha$ à $V_\alpha$ est aussi la restriction de $u - v$, donc est nilpotente ; $V_\alpha$ est donc contenu dans le sous-espace $M_\alpha$ formé des $x \in E$ annulés par une puissance de $u - \alpha$. Comme $E$ est somme directe des $V_\alpha$ et aussi des $M_\alpha$ (VII, p. 34, prop. 7), cela montre que $V_\alpha = M_\alpha$ pour tout $\alpha$. D’après le cor. à la prop. 9 (VII, p. 36), il s’ensuit que $\chi_u = \chi_v$; on en conclut aussi que $v$ est bien déterminé par $u$ : sa restriction à chaque $M_\alpha$ est l’homothétie de rapport $\alpha$.

Inversement, définissons $v$ par la condition précédente ; il est clair que $v$ est diagonalisable et $u - v$ nilpotent. D’après la prop. 7 de VII, p. 34, il existe des polynômes $q_\alpha$ tels que, pour tout $x \in E$, le composant de $x$ dans $M_\alpha$ soit $q_\alpha(u) \cdot x$. On a alors $v = \sum \alpha q_\alpha(u)$; cela implique que $u$ et $v$ commutent et achève la démonstration.

B) Revenons à la démonstration du th. 1.

Supposons d’abord que $u$ s’écrive sous la forme $s + n$, où $s$ est absolument semi-simple, $n$ nilpotent et où $s$ et $n$ commutent. Soit $\Omega$ une clôture algébrique de $K$; on a $u_{(\Omega)} = s_{(\Omega)} + n_{(\Omega)}$, où $s_{(\Omega)}$ est diagonalisable, $n_{(\Omega)}$ est nilpotent, et $s_{(\Omega)}$ et $n_{(\Omega)}$ commutent ; d’après le lemme 4, il en résulte que $s_{(\Omega)}$ et donc $s$ sont uniquement déterminés, que les polynômes $\chi_{u_{(\Omega)}}$ et $\chi_{s_{(\Omega)}}$ de $\Omega[X]$ coïncident, donc aussi les polynômes $\chi_u$ et $\chi_s$, et que $s$ s’exprime comme un polynôme en $u$ à coefficients dans $\Omega$. Cela montre d’abord que les valeurs propres de $u$ sont aussi celles de $s$, donc sont séparables sur $K$ (VII, p. 41, prop. 15) ; par ailleurs, $s$ étant combinaison linéaire à coefficients dans $\Omega$ de puissances de $u$ est aussi combinaison linéaire de ces mêmes puissances à coefficients dans $K$ (II, p. 113, prop. 19), et il existe un polynôme $P \in K[X]$ tel que $s = P(u)$, donc $n = Q(u)$ avec $Q(X) = X - P(X)$. Montrons que l’on peut choisir $Q$ (et donc $P$) sans terme constant. Si $u$ est inversible, son polynôme caractéristique possède un terme constant non nul, et le th. de Hamilton-Cayley (III, p. 107, prop. 20) montre que 1 peut s’exprimer comme un polynôme en $u$ sans terme constant, d’où l’assertion dans ce cas. Si $u$ n’est pas inversible, son noyau $W$ n’est pas réduit à 0 et est stable pour $n$ (VII, p. 40, lemme 3) ; comme la restriction de $n$ à $W$ est nilpotente, il existe un vecteur $x \neq 0$ dans $W$ tel que $u(x) = n(x) = 0$, ce qui montre que $Q$ ne peut avoir de terme constant.

Inversement, supposons maintenant que les valeurs propres de $u$ soient séparables sur $K$, et soit $L$ une extension galoisienne finie de $K$ contenant ces valeurs propres. D’après le lemme 4, on peut écrire $u_{(L)} = v + w$, où $v$ est diagonalisable, $w$ est nilpotent et $vw = wv$. Soient $B$ une base de $E$, $B'$ la base correspondante de $L \otimes_K E$, $U, V, W$ les matrices de $u_{(L)}, v, w$ relativement à $B'$; notons que $U$ est aussi la matrice de $u$ par rapport à $B$, donc est à coefficients dans $K$. Pour tout $K$-automorphisme $\sigma$ de $L$, et toute matrice $A$ à éléments dans $L$, notons $A^\sigma$ la matrice obtenue en appliquant $\sigma$ aux éléments de $A$. Soit $\sigma$ un $K$-automorphisme de $L$; on a $U = U^\sigma = (V + W)^\sigma = V^\sigma + W^\sigma,\ V^\sigma W^\sigma = (VW)^\sigma = (VV)^\sigma = W^\sigma V^\sigma$; comme $V^\sigma$ est la matrice d’un endomorphisme diagonalisable et $W^\sigma$ est nilpotente, il résulte du lemme 4 que $V^\sigma = V,\ W^\sigma = W$. Comme cela est valable pour tout $\sigma$, $V$ et $W$ sont à coefficients dans $K$; si $u_s$ et $u_n$ sont les endomorphismes de $E$ de matrices $V$ et $W$ par rapport à $B$, on a $(u_s)_{(L)} = v,\ (u_n)_{(L)} = w$. Il s’ensuit que $u_s$ est absolument semi-simple, que $u_n$ est nilpotent, que $u_s$ et $u_n$ commutent et que $u = u_s + u_n$. Cela achève la démonstration.

Lorsqu’un endomorphisme $f$ possède une décomposition de Jordan, on note celle-ci $(f_s, f_n)$ et les endomorphismes $f_s$ et $f_n$ sont appelés respectivement la composante absolument semi-simple et la composante nilpotente de $f$. Lorsque $K$ est parfait, tout endomorphisme possède une décomposition de Jordan ; par ailleurs, il y a alors identité entre endomorphismes absolument semi-simples et endomorphismes semi-simples et on dit aussi « composante semi-simple » au lieu de « composante absolument semi-simple ».

#### Corollaire 1 {#alg-vii-s5-lem-4-cor-1 .statement}

Supposons que $u$ possède une décomposition de Jordan, et soit $L$ une extension de $K$. Alors l’endomorphisme $u_{(L)}$ de $E_{(L)}$ possède une décomposition de Jordan, et l’on a $(u_{(L)})_s = (u_s)_{(L)},\ (u_{(L)})_n = (u_n)_{(L)}$.

#### Corollaire 2 {#alg-vii-s5-lem-4-cor-2 .statement}

Supposons que $u$ possède une décomposition de Jordan. Tout endomorphisme de $E$ qui commute à $u$ commute aussi à $u_s$ et $u_n$.

#### Corollaire 3 {#alg-vii-s5-lem-4-cor-3 .statement}

Soient $u$ et $v$ deux endomorphismes permutables de $E$ possédant des décompositions de Jordan.
a) Les endomorphismes $u, v, u_s, v_s, u_n, v_n$ sont deux à deux permutables.
b) Les endomorphismes $u + v$ et $uv$ possèdent des décompositions de Jordan et on a $(u + v)_s = u_s + v_s,\ (u + v)_n = u_n + v_n,\ (uv)_s = u_s v_s,\ (uv)_n = u_s v_n + u_n v_s + u_n v_n$.
La partie a) résulte du cor. 2. Pour démontrer la partie b), il suffit de remarquer que $u_s + v_s$ et $u_s v_s$ sont absolument semi-simples (VII, p. 42, cor.) et $u_n + v_n$ et $u_s v_n + u_n v_s + u_n v_n$ sont nilpotents (comme somme d’endomorphismes nilpotents permutables).

#### Corollaire 4 {#alg-vii-s5-lem-4-cor-4 .statement}

Supposons que $u$ possède une décomposition de Jordan, et soit $R$ un polynôme de $K[X]$. Alors l’endomorphisme $R(u)$ possède une décomposition de Jordan et on a $R(u)_s = R(u_s)$.

#### Remarque 1 {#alg-vii-s5-n9-rem-1 .statement}

On a $\det(u_s) = \det(u)$, $\operatorname{Tr}(u_s) = \operatorname{Tr}(u)$.

#### Remarque 2 {#alg-vii-s5-n9-rem-2 .statement}

Pour que $u$ soit trigonalisable, il faut et il suffit que $u$ possède une décomposition de Jordan et que $u_s$ soit diagonalisable. Il existe alors une base de $E$ par rapport à laquelle la matrice de $u$ est triangulaire inférieure, celle de $u_s$ est diagonale et à même diagonale que la matrice de $u$ ($cf.$ lemme 4 et ci-dessous prop. 19).

On notera cependant que si la matrice de $u$ par rapport à une base est triangulaire, la matrice de $u_s$ par rapport à cette même base n’est pas en général diagonale.

#### Remarque 3 {#alg-vii-s5-n9-rem-3 .statement}

On définit de façon analogue la notion de décomposition de Jordan pour une matrice carrée. Par exemple, pour la matrice de Jordan $U_{m,\alpha}$, on a

$$
(U_{m,\alpha})_s = \alpha \cdot I_m , \quad (U_{m,\alpha})_n = U_{m,0} .
$$

#### Remarque 4 {#alg-vii-s5-n9-rem-4 .statement}

Si $u$ est semi-simple, mais non absolument semi-simple, il ne possède pas de décomposition de Jordan.

Un endomorphisme $u$ d’un espace vectoriel $V$ sur un corps commutatif est dit unipotent si l’endomorphisme $u - \operatorname{Id}_V$ est nilpotent, c’est-à-dire s’il existe un entier $r$ tel que $(u - \operatorname{Id}_V)^r = 0$; $u$ est alors un automorphisme de $V$, puisque si $u = \operatorname{Id}_V - n$ avec $n^r = 0$, on a

$$
(\operatorname{Id}_V + n + \cdots + n^{r-1})\, u = u(\operatorname{Id}_V + n + \cdots + n^{r-1}) = \operatorname{Id}_V .
$$

Si $V$ est de dimension finie $m$, alors $u$ est unipotent si et seulement si $\chi_u(X) = (X - 1)^m$ (VII, p. 33, cor. 3).

#### Proposition 17 {#alg-vii-s5-prop-17 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif, et $f$ un endomorphisme de $E$. Les conditions suivantes sont équivalentes :

(i) $f$ possède une décomposition de Jordan et est un automorphisme ;
(ii) $f$ possède une décomposition de Jordan et $f_s$ est un automorphisme ;
(iii) il existe un automorphisme absolument semi-simple $a$ de $E$ et un automorphisme unipotent $u$ de $E$ tels que $f = ua = au$.

De plus, sous ces conditions, et avec les notations de (iii), on a nécessairement $a = f_s$, $u = 1 + f_s^{-1}f_n$.

(i) $\Rightarrow$ (ii) : cela résulte de la remarque 1.
(ii) $\Rightarrow$ (iii) : prenons $a = f_s$, $u = 1 + f_s^{-1}f_n$; alors $f = ua = au$, $a$ est un automorphisme absolument semi-simple, et $u$ est unipotent.
(iii) $\Rightarrow$ (i) : avec les notations de (iii), posons $n = a(u - 1) = (u - 1)a$. Alors $an = na$, $f = a + n$, et $n$ est nilpotent. Il en résulte que $(a, n)$ est la décomposition de Jordan de $f$; cela implique (i) ainsi que les relations $a = f_s$, $u = 1 + f_s^{-1}f_n$.

On pose $f_u = f_s^{-1}f = ff_s^{-1} = 1 + f_s^{-1}f_n$, et on dit que c’est la composante unipotente de $f$. Le couple $(f_s, f_u)$ est souvent appelé la décomposition de Jordan multiplicative de l’automorphisme $f$.

#### Proposition 18 {#alg-vii-s5-prop-18 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$, $E'$ un sous-espace de $E$ et $u$ un endomorphisme de $E$ laissant $E'$ stable.

Soit $u'$ (resp. $u''$) l’endomorphisme de $E'$ (resp. $E/E'$) déduit de $u$. On a $\chi_u = \chi_{u'} \cdot \chi_{u''}$.

Pour que $u$ possède une décomposition de Jordan, il faut et il suffit qu’il en soit de même pour $u'$ et $u''$; de plus, sous ces conditions, les composantes absolument semi-simples (resp. nilpotentes) de $u'$ et $u''$ sont les endomorphismes de $E'$ et $E/E'$ déduits de la composante absolument semi-simple (resp. nilpotente) de $u$.

Soient $B$ une base de $E$ contenant une base $B'$ de $E'$ et $B''$ la base de $E''$ image de $B - B'$. Notons $U, U', U''$ les matrices de $u, u', u''$ par rapport à $B, B', B''$ respectivement. Alors $U$ est de la forme

$$
\begin{pmatrix}
U' & Z \\
0 & U''
\end{pmatrix}
$$

et on a $\chi_u = \chi_U = \chi_{U'} \chi_{U''} = \chi_{u'} \chi_{u''}$ (cf. III, p. 100, exemple 2). On en déduit que l’ensemble des valeurs propres de $u$ est la réunion des ensembles de valeurs propres de $u'$ et $u''$. Si $u'$ et $u''$ possèdent des décompositions de Jordan, alors les valeurs propres de $u'$ et $u''$ sont séparables sur $K$, donc aussi les valeurs propres de $u$, et $u$ possède une décomposition de Jordan (VII, p. 42, th. 1). Inversement, si $u$ possède la décomposition de Jordan ($s, n$), $s$ et $n$ laissent stable $E'$ car ce sont des polynômes en $u$; notons $s', n', s'', n''$ les endomorphismes de $E', E', E/E', E/E'$ déduits respectivement de $s, n, s, n$. Comme les polynômes minimaux de $s'$ et $s''$ divisent celui de $s, s'$ et $s''$ sont absolument semi-simples (VII, p. 41, prop. 15) ; par ailleurs, $n'$ et $n''$ sont nilpotents. Enfin, on a $u' = s' + n', u'' = s'' + n''$ et $s'n' = n's', s''n'' = n''s''$, ce qui achève la démonstration.

#### Proposition 19 {#alg-vii-s5-prop-19 .statement}

Soient $E$ un espace vectoriel de dimension finie sur un corps commutatif $K$, et $\mathfrak{F}$ un ensemble d’endomorphismes trigonalisables de $E$ deux à deux permutables. Alors il existe une base de $E$ telle que, par rapport à cette base, la matrice de tout élément $u$ de $\mathfrak{F}$ soit triangulaire inférieure et que la matrice de $u_s$ soit diagonale et ait mêmes éléments diagonaux que celle de $u$.

D’après le cor. 3 de VII, p. 44, l’ensemble $\mathfrak{F}_s$ des composantes absolument semi-simples des éléments de $\mathfrak{F}$ est formé d’éléments diagonalisables deux à deux permutables, donc est diagonalisable (VII, p. 40, prop. 13), l’ensemble $\mathfrak{F}_n$ des composantes nilpotentes des éléments de $\mathfrak{F}$ est formé d’éléments nilpotents deux à deux permutables, et chaque élément de $\mathfrak{F}_n$ commute à chaque élément de $\mathfrak{F}_s$. Raisonnant alors comme dans la démonstration de la prop. 13 (VII, p. 40), on voit qu’il existe une décomposition de $E$ en somme directe de sous-espaces $E_i$, qui sont stables pour $\mathfrak{F}_s$ et $\mathfrak{F}_n$ et tels que chaque élément de $\mathfrak{F}_s$ induise sur chaque $E_i$ une homothétie. Remplaçant $E$ par chacun des $E_i$, on peut donc supposer que les éléments de $\mathfrak{F}_s$ sont des homothéties ; il nous suffit de démontrer qu’il existe une base de $E$ par rapport à laquelle les éléments de $\mathfrak{F}_n$ sont représentés par des matrices triangulaires inférieures à éléments diagonaux nuls ; on est donc ramené au cas où $\mathfrak{F}$ est formé d’éléments nilpotents.

Supposons alors $E \neq 0$, et soit $F$ un sous-espace non nul de $E$, stable pour $\mathfrak{F}$, et de dimension minimum. Pour tout $u \in \mathfrak{F}$, le noyau de la restriction de $u$ à $F$ est non nul et stable pour $\mathfrak{F}$ (VII, p. 40, lemme 3) ; d’après le choix de F, la restriction de $u$ à F est donc nulle pour tout $u \in \mathfrak{F}$. Soit alors $x \in F, x \neq 0$; on a $u(x) = 0$ pour tout $u \in \mathfrak{F}$; raisonnant par récurrence sur la dimension de E, on peut supposer qu’il existe une base $(\overline{e}_1, ..., \overline{e}_{n-1})$ du quotient $E' = E/Kx$ telle que, pour tout $u \in \mathfrak{F}$, l’endomorphisme $\overline{u}$ de $E'$ déduit de $u$ ait par rapport à cette base une matrice triangulaire inférieure à coefficients diagonaux nuls ; si $e_i \in E$ se projette sur $\overline{e}_i$ pour $i = 1, ..., n-1$, la base $(e_1, ..., e_{n-1}, x)$ répond aux conditions exigées.

Exercises

## EXERCICES {#alg-vii-s5-exercises}

Sauf mention expresse du contraire, tous les corps intervenant dans les exercices de ce paragraphe sont supposés commutatifs.

See the [exercises for § 5](exercises/s5/).
