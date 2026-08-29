---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 9
section_title: Normes et traces
lang: fr
source: alg-i-iii-fr
book_pages: A III.107-A III.116, A III.196
pdf_pages: 0494-0503, 0583-0583
extraction: ocr
subsections:
    - "no": 1
      title: Normes et traces relatives à un module
      page: 108
      pdf_page: 495
    - "no": 2
      title: Propriétés des traces et normes relatives à un module
      page: 109
      pdf_page: 496
    - "no": 3
      title: Norme et trace dans un algèbre
      page: 110
      pdf_page: 497
    - "no": 4
      title: Propriétés des normes et traces dans une algèbre
      page: 111
      pdf_page: 498
    - "no": 5
      title: Discriminant d’une algèbre
      page: 115
      pdf_page: 502
statements: 19
exercises: 1
content_sha256: 5fd5332d97634f65f0700d65e62ddf4fb51bdfdab9e4d726d3944f066bc41ebd
---

## § 9. NORMES ET TRACES

Dans tout ce paragraphe, on note $K$ un anneau commutatif, $A$ une $K$-algèbre, associative et unifère. Tout $A$-module sera supposé muni de la structure de $K$-module obtenue par restriction des scalaires à $K$.

### 1. Normes et traces relatives à un module

#### Définition 1 {#alg-iii-s9-def-1 .statement}

Soit $M$ un $A$-module admettant une base finie en tant que $K$-module. Pour tout $a \in A$, soit $a_M$ l’endomorphisme $x \mapsto ax$ du $K$-module $M$. La trace, le déterminant et le polynôme caractéristique de $a_M$ sont appelés respectivement la trace, la norme et le polynôme caractéristique de $a$ relativement à $M$.

La trace et la norme de $a$ sont donc des éléments de $K$, notés respectivement $\mathrm{Tr}_{M/K}(a)$ et $N_{M/K}(a)$; le polynôme caractéristique de $a$ est un élément de $K[X]$, noté $\mathrm{Pc}_{M/K}(a; X)$. On omet $K$ dans les notations précédentes lorsqu’il n’y a pas risque de confusion.

D’après les propriétés de la trace et du déterminant d’un endomorphisme (II, p. 78 et III, p. 90), on a les relations

(1)
$$
\mathrm{Tr}_M(a + a') = \mathrm{Tr}_M(a) + \mathrm{Tr}_M(a')
$$
(2)
$$
\mathrm{Tr}_M(aa') = \mathrm{Tr}_M(a'a)
$$
(3)
$$
N_M(aa') = N_M(a)N_M(a')
$$

quels que soient $a, a'$ dans $A$.

Soient $(e_i)_{1 \leq i \leq n}$ une base du $K$-module $M$, et $(m_{ij}(a))$ la matrice de l’endomorphisme $a_M$ par rapport à cette base. Les fonctions $m_{ij}$ sont des formes linéaires sur le $K$-module $A$, et l’on a

(4)
$$
\mathrm{Tr}_M(a) = \sum_{i=1}^n m_{ii}(a)
$$
(5)
$$
N_M(a) = \det(m_{ij}(a))
$$
(6)
$$
\mathrm{Pc}_M(a; X) = \det(\delta_{ij}X - m_{ij}(a)).
$$

Il résulte de III, p. 107, formule (50), que l’on a

(7)
$$
\mathrm{Pc}_M(a; X) = X^n + c_1 X^{n-1} + \cdots + c_n
$$

avec

(8)
$$
c_1 = -\mathrm{Tr}_M(a), \quad c_n = (-1)^n N_M(a).
$$

Pour $\lambda \in K$, on a

(9)
$$
\mathrm{Tr}_M(\lambda) = n.\lambda, \quad N_M(\lambda) = \lambda^n, \quad \mathrm{Pc}_M(\lambda; X) = (X - \lambda)^n.
$$

Soit $K'$ une $K$-algèbre commutative. Posons $M' = K' \otimes_K M$ et $A' = K' \otimes_K A$, de sorte que $M'$ est muni d’une structure de $A'$-module (III, p. 40, Exemple 2). En tant que $K'$-module, $M'$ admet la base formée des $1 \otimes e_i$ ($1 \leq i \leq n$) et la matrice de $a_M$ par rapport à $(e_i)$ est égale à la matrice de $(1 \otimes a)_{M'}$ par rapport à $(e'_i)$. On a donc

(12)
$$
\mathrm{Tr}_{M'}(1 \otimes a) = \mathrm{Tr}_M(a).1, \quad N_{M'}(1 \otimes a) = N_M(a).1
$$
$$
\mathrm{Pc}_{M'}(1 \otimes a; X) = \mathrm{Pc}_M(a; X).1
$$

pour tout $a \in A$, où $1$ désigne l’élément unité de $K'$. Si l’on prend en particulier $K' = K[X]$, on a
$$
(13) \quad \mathrm{Pc}_{M/K}(a; X) = N_{M[X]/K[X]}(X - a).
$$

### 2. Propriétés des traces et normes relatives à un module

Si $M$ et $M'$ sont deux $A$-modules *isomorphes*, ayant des bases finies sur $K$, on a, pour tout $a \in A$
$$
(14) \quad \mathrm{Tr}_{M'}(a) = \mathrm{Tr}_M(a), \quad N_{M'}(a) = N_M(a), \quad \mathrm{Pc}_{M'}(a; X) = \mathrm{Pc}_M(a; X)
$$
car si $f$ est un isomorphisme de $M$ sur $M'$, la matrice de $a_M$ par rapport à une base $B$ de $M$ sur $K$ est la même que la matrice de $a_M$ par rapport à la base $f(B)$ de $M'$.

#### Proposition 1 {#alg-iii-s9-prop-1 .statement}

*Soit $M = M_0 \supset M_1 \supset \ldots \supset M_r = \{0\}$ une suite décroissante de sous-modules d’un $A$-module $M$, telle que chacun des $K$-modules $P_i = M_{i-1}/M_i$ ($1 \leq i \leq r$) admette une base finie. Alors le $K$-module $M$ admet une base finie et l’on a*
$$
\mathrm{Tr}_M(a) = \sum_{i=1}^r \mathrm{Tr}_{P_i}(a), \qquad N_M(a) = \prod_{i=1}^r N_{P_i}(a)
$$
$$
(15) \qquad \mathrm{Pc}_M(a; X) = \prod_{i=1}^r \mathrm{Pc}_{P_i}(a; X).
$$
Soit $B'_i$ une base de $P_i$ sur $K$; alors un système de représentants $B_i$ de $B'_i$ (mod. $M_i$) est une base d’un supplémentaire du $K$-module $M_i$ dans le $K$-module $M_{i-1}$ (II, p. 27, prop. 21). La réunion $B$ des $B_i$ ($1 \leq i \leq r$) est une base de $M$ sur $K$. Soit $X_{ii}$ la matrice de l’endomorphisme $a_{P_i}$ par rapport à la base $B'_i$. Il est immédiat que la matrice de $a_M$ par rapport à la base $B$ est de la forme
$$
\begin{pmatrix}
X_{rr} & X_{r,r-1} & \ldots & X_{r,1} \\
0 & X_{r-1,r-1} & \ldots & X_{r-1,1} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \ldots & X_{11}
\end{pmatrix}
$$
et la proposition résulte des formules (4), (5) et (6) de III, p. 108 et de la formule (31) de III, p. 101.

#### Proposition 2 {#alg-iii-s9-prop-2 .statement}

*Soient $A, A'$ deux $K$-algèbres, $M$ un $A$-module et $M'$ un $A'$-module. On suppose que $M$ et $M'$ sont des $K$-modules libres de dimensions respectives $n$ et $n'$, et on considère $M \otimes_K M'$ comme un $(A \otimes_K A')$-module (III, p. 40, Exemple 2). Alors, pour $a \in A$ et $a' \in A_1$, on a*
$$
(16) \qquad \mathrm{Tr}_{M \otimes M'}(a \otimes a') = \mathrm{Tr}_M(a) \mathrm{Tr}_{M'}(a')
$$

(17) $N_{M \otimes M'}(a \otimes a') = (N_M(a))^{n'}(N_{M'}(a'))^n.$

En effet, la formule (16) résulte de II, p. 80, formule (26) et la formule (17) de III, p. 101, formule (33).

### 3. Norme et trace dans un algèbre

#### Définition 2 {#alg-iii-s9-def-2 .statement}

Soit $A$ une $K$-algèbre qui soit un $K$-module libre de dimension finie. Pour tout élément $a \in A$, on appelle trace (resp. norme,$^1$ resp. polynôme caractéristique) de $a$ relativement à $A$ et à $K$ la trace (resp. le déterminant, resp. le polynôme caractéristique) de l’endomorphisme $x \mapsto ax$ du $K$-module $A$.

On note $\mathrm{Tr}_{A/K}(a)$, $N_{A/K}(a)$ et $\mathrm{Pc}_{A/K}(a; X)$ la trace, la norme et le polynôme caractéristique de $a \in A$ relativement à $A$ et $K$; on omet $K$ (et même $A$) dans ces notations lorsqu’il n’y a pas risque de confusion. On notera que la trace (resp. la norme, le polynôme caractéristique) de $a \in A$ n’est autre que la trace (resp. la norme, le polynôme caractéristique) de $a$ relativement au $A$-module $A_s$.

Supposons que $A$ soit le produit $A_1 \times A_2 \times \cdots \times A_m$ d’un nombre fini d’algèbres qui soient des $K$-modules libres de dimensions finies sur $K$. Utilisant la remarque précédente et la prop. 1 de III, p. 109, on a, pour tout élément $a = (a_1, \ldots, a_m) \in A$

$$
\mathrm{Tr}_{A/K}(a) = \sum_{i=1}^m \mathrm{Tr}_{A_i/K}(a_i), \quad N_{A/K}(a) = \prod_{i=1}^m N_{A_i/K}(a_i)
$$
$$
\mathrm{Pc}_{A/K}(a; X) = \prod_{i=1}^m \mathrm{Pc}_{A_i/K}(a_i; X).
$$

De même, la prop. 2 de III, p. 109 montre que si $A$ et $A'$ sont deux algèbres qui soient des $K$-modules libres de dimensions finies $n, n'$ respectivement sur $K$, on a, pour $a \in A, a' \in A'$,

$$
\mathrm{Tr}_{A \otimes A'}(a \otimes a') = \mathrm{Tr}_A(a) \mathrm{Tr}_{A'}(a')
$$
$$
N_{A \otimes A'}(a \otimes a') = (N_A(a))^{n'}(N_{A'}(a'))^n.
$$

Enfin, soient $A$ une algèbre qui soit un $K$-module libre de dimension finie sur $K$, $h$ un homomorphisme de $K$ dans un anneau commutatif $K'$, $A' = A_{(K')}$, la $K'$-algèbre déduite de $A$ par extension des scalaires au moyen de $h$. Il résulte de la formule (12) de III, p. 108 que, pour tout $a \in A$, on a

$$
\mathrm{Tr}_{A'/K'}(1 \otimes a) = h(\mathrm{Tr}_{A/K}(a)), \quad N_{A'/K'}(1 \otimes a) = h(N_{A/K}(a))
$$
$$
\mathrm{Pc}_{A'/K'}(1 \otimes a; X) = h(\mathrm{Pc}_{A/K}(a; X))
$$

$^1$ On ne confondra pas cette notion avec la notion de norme dans une algèbre sur un corps valué (TG, IX, § 3, no 7).

h étant l’homomorphisme K[X] → K'[X] déduit de h. En particulier, pour K' = K[X], on a, en posant A[X] = A ⊗_K K[X],

$$
\mathrm{Pc}_{A/K}(a; X) = N_{A[X]/K[X]}(X - a).
$$

Plus généralement, si K' est une K-algèbre commutative et A' = A ⊗_K K', on a, pour tout x ∈ A',

$$
\mathrm{Pc}_{A/K}(a; x) = N_{A'/K'}(x - a).
$$

#### Exemple 1 {#alg-iii-s9-n3-exa-1 .statement}

Soient A une algèbre quadratique sur K de type (\alpha, \beta), (e_1, e_2) une base de type (\alpha, \beta) (III, p. 12 et 13). Pour x = \xi e_1 + \eta e_2, on a Tr_{A/K}(x) = 2\xi + \beta\eta et N_{A/K}(x) = \xi^2 + \beta\xi\eta - \alpha\eta^2; ces fonctions sont donc identiques à la trace et à la norme cayleyennes de x (III, p. 14 et p. 15).

#### Exemple 2 {#alg-iii-s9-n3-exa-2 .statement}

Soit A une algèbre de quaternions sur K. Un calcul direct permet de vérifier que l’on a Tr_{A/K}(x) = 2 T(x) et N_{A/K}(x) = (N(x))^2, où T et N sont la trace et la norme cayleyennes (III, p. 15).

#### Exemple 3 {#alg-iii-s9-n3-exa-3 .statement}

Soit A = M_n(K), et rangeons la base canonique (E_{ij}) de A (II, p. 142) dans l’ordre lexicographique. On voit alors aussitôt que pour toute matrice X = \sum_{i,j} \xi_{ij} E_{ij}, la matrice (d’ordre n^2) de l’endomorphisme Y \to XY a la forme

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

d’où Tr_{A/K}(X) = n \cdot \mathrm{Tr}(X) et N_{A/K}(X) = (\det(X))^n.

### 4. Propriétés des normes et traces dans une algèbre

#### Proposition 3 {#alg-iii-s9-prop-3 .statement}

*Soit A une K-algèbre admettant une base finie. Pour qu’un élément a \in A soit inversible, il faut et il suffit que sa norme N_{A/K}(a) soit inversible dans K.*

Si a admet un inverse a' dans A, on a

$$
N_{A/K}(a) N_{A/K}(a') = N_{A/K}(aa') = N_{A/K}(1) = 1
$$

d’après la formule (3) de III, p. 108. Réciproquement, si N_{A/K}(a) est inversible, l’endomorphisme h : x \mapsto ax est bijectif (III, p. 91, th. 1). Il existe donc a' \in A tel que aa' = 1 ; on a alors $h(a'a - 1) = aa'a - a = (aa' - 1)a = 0$, d’où $a'a = 1$ puisque h est injectif. Donc a' est l’inverse de a.

#### Proposition 4 {#alg-iii-s9-prop-4 .statement}

*Soit A une K-algèbre admettant une base finie. Pour tout a \in A, on a*

$$
\mathrm{Pc}_{A/K}(a; a) = 0.
$$

Cela résulte immédiatement du th. de Hamilton-Cayley (III, p. 107, prop. 20).

#### Proposition 5 {#alg-iii-s9-prop-5 .statement}

*Soient A une K-algèbre, m un idéal bilatère de A. On suppose que A_0 = A/m est un K-module libre de dimension finie n, qu’il existe un entier r > 0 tel que m^r = \{0\}, et que m^{i-1}/m^i est un A_0-module libre de dimension finie s_i pour 1 \leq i \leq r.*

Posons $s = s_1 + \cdots + s_r$ et pour tout $a \in A$, notons $a_0$ la classe de $a$ mod. m. Alors $A$ est un $K$-module libre de dimension $ns$, et pour tout $a \in A$, on a
$$
\text{Tr}_A(a) = s \cdot \text{Tr}_{A_0}(a_0), \quad N_A(a) = (N_{A_0}(a_0))^s \\
\text{Pc}_A(a; X) = (\text{Pc}_{A_0}(a_0; X))^s
$$
En vertu de II, p. 31, prop. 25, $m^{i-1}/m^i$ est un $K$-module libre de dimension $ns_i$. On peut donc appliquer la prop. 1 de III, p. 109 avec $P_i = m^{i-1}/m^i$; cela montre en premier lieu que $A$ est un $K$-module libre de dimension $n(s_1 + \cdots + s_r) = ns$. En outre, l’hypothèse entraîne que le $A$-module $P_i$ est isomorphe à une somme directe de $s_i$ sous-modules isomorphes au $A$-module $A_0$; en vertu de la prop. 1 de III, p. 109, on a donc $N_{P_i}(a) = N_{A_0}(a)^{s_i}$; finalement, on a donc
$$
N_A(a) = N_{A_0}(a)^s.
$$
Dans cette formule, $N_{A_0}(a)$ est défini en considérant $A_0$ comme $A$-module à gauche, et il est égal au déterminant de l’application $K$-linéaire $x \mapsto ax$ de $A_0$ dans lui-même; mais comme $ax = a_0 x$ pour $x \in A_0$, on a $N_{A_0}(a) = N_{A_0}(a_0)$, ce qui achève de prouver la formule (23) relative à la norme. Les deux autres se démontrent de façon analogue.

#### Proposition 6 {#alg-iii-s9-prop-6 .statement}

Soient $A$ une $K$-algèbre commutative admettant une base finie sur $K$, $V$ un $A$-module admettant une base finie sur $A$. Alors $V$ admet une base finie sur $K$, et pour tout $A$-endomorphisme $u$ de $V$, si $u_K$ est l’application $u$ considérée comme $K$-endomorphisme de $V$ on a
$$
\text{Tr}(u_K) = \text{Tr}_{A/K}(\text{Tr}(u)), \quad \det(u_K) = N_{A/K}(\det(u)) \\
\text{Pc}(u_K; X) = N_{A[X]/K[X]}(\text{Pc}(u; X))
$$
Soient $(a_i)_{1 \leq i \leq m}$ une base de $A$ sur $K$, $(e_j)_{1 \leq j \leq n}$ une base de $V$ sur $A$; alors $(a_i e_j)$ est une base de $V$ sur $K$ (II, p. 31, prop. 25). D’autre part la troisième des formules (24) se déduit de la seconde appliquée à l’endomorphisme $X - \bar{u}$ du $A[X]$-module $A[X] \otimes_A V$ (III, p. 106). Il suffira donc de démontrer les deux premières formules (24). Nous établirons d’abord le lemme suivant:

#### Lemme 1 {#alg-iii-s9-lem-1 .statement}

Soient $X_{ij}$ ($1 \leq i \leq n, 1 \leq j \leq n$) $n^2$ indéterminées, $X$ la matrice carrée $(X_{ij})$ d’ordre $n$, $D(X_{11}, \ldots, X_{nn}) \in \mathbf{Z}[X_{11}, \ldots, X_{nn}]$ le déterminant $\det(X)$. Soient d’autre part $A$ un anneau commutatif, $M_{ij}$ ($1 \leq i \leq n, 1 \leq j \leq n$) $n^2$ matrices carrées d’ordre $m$ sur $A$, deux à deux permutables, et $M$ la matrice carrée d’ordre $mn$ sur $A$ qui se met sous la forme d’une matrice carrée de matrices (II, p. 152)
$$
M = \begin{pmatrix}
M_{11} & M_{12} & \cdots & M_{1n} \\
M_{21} & M_{22} & \cdots & M_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
M_{n1} & M_{n2} & \cdots & M_{nn}
\end{pmatrix}
$$

Alors le déterminant de $M$ est égal au déterminant de la matrice carrée $D(M_{11}, \ldots, M_{nn})$ d’ordre $m$.

Nous procéderons par récurrence sur $n$, les cas $n = 0$ et $n = 1$ étant triviaux. Soient $Z$ un nouvelle indéterminée, et $N_{ij}$ la matrice $M_{ij} + \delta_{ij} Z I_m$ ($\delta_{ij}$ indice de Kronecker). Si $D^{ij}(X_{11}, \ldots, X_{nn})$ est le cofacteur de $X_{ij}$ dans la matrice $X$ (III, p. 99), on a
$$
\sum_{i=1}^n X_{ji} D^{ki}(X_{11}, \ldots, X_{nn}) = \delta_{jk} D(X_{11}, \ldots, X_{nn})
$$
(III, p. 99, formule (28)). Posons $N'_{ij} = D^{ij}(N_{11}, \ldots, N_{nn})$, qui est une matrice carrée d’ordre $m$ sur $A[Z]$, et considérons le produit $N.U$ où
$$
U = \begin{pmatrix}
N'_{11} & 0 & \cdots & 0 \\
N'_{12} & I_m & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
N'_{1n} & 0 & \cdots & I_m
\end{pmatrix}
\quad
N = \begin{pmatrix}
N_{11} & N_{12} & \cdots & N_{n1} \\
N_{21} & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
N_{n1} & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$
En effectuant ce produit par blocs (II, p. 148) et utilisant les formules (25), il vient
$$
N.U = \begin{pmatrix}
P & N_{12} & \cdots & N_{1n} \\
0 & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
0 & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$
où on a posé $P = D(N_{11}, \ldots, N_{nn})$. Soit
$$
Q = \begin{pmatrix}
N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots \\
N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$
qui est une matrice d’ordre $m(n-1)$; on a (III, p. 101, formule (31)) $(\det N)(\det U) = (\det P)(\det Q)$ et $\det U = \det N'_{11}$. Mais d’après l’hypothèse de récurrence, on a $\det Q = \det(D^{11}(N_{11}, \ldots, N_{nn})) = \det N'_{11}$, et en vertu de la définition des $N_{ij}$, il est clair que $\det Q$ est un polynôme de $A[Z]$, de degré $m(n-1)$, dont le terme en $Z^{m(n-1)}$ a pour coefficient 1 ; on en déduit aussitôt que $\det Q$ n’est pas diviseur de zéro dans l’algèbre graduée $A[Z]$. On en conclut donc que $\det N = \det(D(N_{11}, \ldots, N_{nn}))$ dans $A[Z]$; si on substitue 0 à $Z$ dans ces polynômes, il vient $\det M = \det(D(M_{11}, \ldots, M_{nn}))$.

Ce lemme étant démontré, le K-module V est somme directe des K-modules $Ae_j$ ($1 \leq j \leq n$); posons $u(e_j) = \sum_{k=1}^n c_{jk} e_k$. Pour tout élément $x e_j \in Ae_j$, avec $x \in A$, la composante de $u(x e_j)$ dans $Ae_k$ est $x c_{jk} e_k$; on en conclut que la matrice de $u_K$ par rapport à la base $(a_i e_j)$ du K-module V se met sous forme d’une matrice carrée de matrices $(M_{jk})$, où $M_{jk}$ est la matrice de l’application K-linéaire $x e_j \mapsto x c_{j k} e_k$ de $A e_j$ dans $A e_k$, par rapport aux bases $(a_i e_j)_{1 \leq i \leq m}$ et $(a_i e_k)_{1 \leq i \leq m}$ de ces deux $K$-modules (II, p. 147). Si pour tout $t \in A$, on note $M(t)$ la matrice, pour rapport à la base $(a_i)_{1 \leq i \leq m}$ de $A$ sur $K$, de l’endomorphisme $x \mapsto xt$ de $A$, on a $M_{jk} = M(c_{jk})$; comme $t \mapsto M(t)$ est un homomorphisme d’anneaux les matrices $M_{jk}$ sont deux à deux permutables. On a donc $\det u_K = \det(D(M_{11}, \ldots, M_{nn}))$ en vertu du lemme 1. Mais comme $t \mapsto M(t)$ est un homomorphisme d’anneaux, $D(M_{11}, \ldots, M_{nn})$ est la matrice du $K$-endomorphisme $x \mapsto x.\det(c_{jk})$ de $A$ par rapport à la base $(a_i)$; par définition son déterminant est donc $N_{A/K}(\det(u))$, ce qui prouve la seconde formule (24). D’autre part, on a $\operatorname{Tr}(u_K) = \sum_{j=1}^n \operatorname{Tr}(M_{jj}) = \sum_{j=1}^n \operatorname{Tr}_{A/K}(c_{jj}) = \operatorname{Tr}_{A/K}\left( \sum_{j=1}^n c_{jj} \right) = \operatorname{Tr}_{A/K}(\operatorname{Tr}(u))$, et la prop. 6 est ainsi complètement démontrée.

#### Corollaire {#alg-iii-s9-n4-cor-1 .statement}

Soient $A$ une $K$-algèbre commutative admettant une base finie sur $K$, $B$ une $A$-algèbre admettant une base finie sur $A$. Alors $B$ admet une base finie sur $K$, et pour tout $b \in B$, on a (« formules de transitivité »)

$$
\operatorname{Tr}_{B/K}(b) = \operatorname{Tr}_{A/K}(\operatorname{Tr}_{B/A}(b)), \quad N_{B/K}(b) = N_{A/K}(N_{B/A}(b))
$$
$$
\mathrm{Pc}_{B/K}(b; X) = N_{A[X]/K[X]}(\mathrm{Pc}_{B/A}(b; X)).
$$

Cela résulte immédiatement de la prop. 6, où l’on fait $V = B$ et $u(x) = bx$.

#### Remarque {#alg-iii-s9-n4-rem-1 .statement}

Supposons que l’homomorphisme $\lambda \mapsto \lambda . 1$ de $K$ dans $A$ soit injectif, et identifions $K$ à son image dans $A$; supposons que $A$ admette une base finie $(e_i)_{1 \leq i \leq n}$ en tant que $K$-module. Soit $s$ un automorphisme de $A$ tel que $s(K) = K$. Soit $a$ un élément de $A$; on a, par transport de structure,

$$
\operatorname{Tr}_{A/K}(s(a)) = s(\operatorname{Tr}_{A/K}(a))
$$
$$
N_{A/K}(s(a)) = s(N_{A/K}(a)).
$$

\* Considérons par ailleurs une dérivation $D$ de $A$ (III, p. 118) telle que $D(K) \subset K$, et posons $D(e_i) = \sum_{j=1}^n e_j \mu_{ji}$ avec $\mu_{ji} \in K$; posons
$$
ae_i = \sum_{j=1}^n e_j \lambda_{ji} \quad \text{avec } \lambda_{ji} \in K.
$$
On a
$$
D(a)e_i + aD(e_i) = D(ae_i) = \sum_{j=1}^n (D(e_j)\lambda_{ji} + e_j D(\lambda_{ji})).
$$
On en déduit que l’on a
$$
D(a)e_i = \sum_{j=1}^n e_j v_{ji}
$$

avec $v_{ji} = D(\lambda_{ji}) + \sum_{k=1}^{n} (\mu_{jkl}\lambda_{ki} - \lambda_{jkl}\mu_{ki})$. Comme $\sum_{i,k} (\mu_{ik}\lambda_{ki} - \lambda_{ik}\mu_{ki}) = 0$, on a donc $\mathrm{Tr}_{A/\mathbf{K}}(D(a)) = \sum_{i=1}^{n} D(\lambda_{ii})$, autrement dit
$$
\mathrm{Tr}_{A/\mathbf{K}}(D(a)) = D(\mathrm{Tr}_{A/\mathbf{K}}(a)).*
$$

### 5. Discriminant d’une algèbre

#### Définition 3 {#alg-iii-s9-def-3 .statement}

Soit $A$ une $\mathbf{K}$-algèbre admettant une base finie de $n$ éléments. On appelle discriminant d’une suite $(x_1, \ldots, x_n)$ de $n$ éléments de $A$, par rapport à $\mathbf{K}$, et l’on note $D_{A/\mathbf{K}}(x_1, \ldots, x_n)$ le déterminant de la matrice carrée $(\mathrm{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}$.

Considérons d’abord une base $(e_i)_{1 \leq i \leq n}$ de $A$ sur $\mathbf{K}$, et posons
$$
e_i e_j = \sum_{k=1}^{n} c_{ijl} e_k \quad \text{avec } c_{ijl} \in \mathbf{K}.
$$
On a donc $\mathrm{Tr}_{A/\mathbf{K}}(e_i) := \sum_{s=1}^{n} c_{iss}$, d’où $\mathrm{Tr}_{A/\mathbf{K}}(e_i e_j) = \sum_{k,s} c_{ijk} c_{kss}$, et par suite
$$
D_{A/\mathbf{K}}(e_1, \ldots, e_n) = \det((\sum_{k,s} c_{ijk} c_{kss})_{1 \leq i \leq n, 1 \leq j \leq n}).
$$
Soient maintenant $(x_i)_{1 \leq i \leq n}$, $(x'_i)_{1 \leq i \leq n}$ deux suites de $n$ éléments de $A$, et supposons qu’il existe une matrice carrée d’ordre $n$, $M = (m_{ij})$ à coefficients dans $\mathbf{K}$, telle que $x_i = \sum_{j=1}^{n} m_{ij} x'_j$ pour $1 \leq i \leq n$. Posons
$$
T = (\mathrm{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}, \qquad T' = (\mathrm{Tr}_{A/\mathbf{K}}(x'_i x'_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
On a $\mathrm{Tr}_{A/\mathbf{K}}(x_i x_j) = \sum_{p,q} m_{ip} m_{jq} \mathrm{Tr}_{A/\mathbf{K}}(x'_p x'_q)$, d’où $T = M . T . {}^t M$; la règle de multiplication des déterminants donne donc
$$
\det T = \det M . \det T' . \det {}^t M = (\det M)^2 \det T'
$$
d’où finalement
$$
D_{A/\mathbf{K}}(x_1, \ldots, x_n) = (\det M)^2 D_{A/\mathbf{K}}(x'_1, \ldots, x'_n).
$$
La formule précédente montre en particulier que les discriminants de deux bases de $A$ sur $\mathbf{K}$ diffèrent par multiplication par le carré d’un élément inversible de $\mathbf{K}$, et engendrent donc le même idéal (principal) de $\mathbf{K}$. Cet idéal $\Delta_{A/\mathbf{K}}$ s’appelle l’idéal discriminant de $A$ sur $\mathbf{K}$; en vertu de la formule (32), le discriminant de toute suite de $n$ éléments de $A$ appartient à $\Delta_{A/\mathbf{K}}$. On notera que deux suites de $n$ éléments de $A$ qui ne diffèrent que par l’ordre des termes ont même discriminant, car le déterminant d’une matrice de permutation est égal à $\pm 1$.

#### Exemple 1 {#alg-iii-s9-n5-exa-1 .statement}

Si $A$ est une algèbre quadratique de type $(\alpha, \beta)$ sur $\mathbf{K}$, on a (avec les notations de III, p. 12) $\operatorname{Tr}(e_1) = 2,\ \operatorname{Tr}(e_2) = \beta,\ \operatorname{Tr}(e_2^2) = \alpha \operatorname{Tr}(e_1) + \beta \operatorname{Tr}(e_2) = 2\alpha + \beta^2$, d’où $D_{A/K}(e_1, e_2) = \beta^2 + 4\alpha$.

#### Exemple 2 {#alg-iii-s9-n5-exa-2 .statement}

Soit $A = K[X]/K[X]P$, où $P(X) = X^3 + pX + q$, de sorte que si $x$ est l’image de $X$ dans $A$, $1, x, x^2$ forment une base de $A$ sur $K$ et $x^3 = -px - q$. On voit aussitôt que $\operatorname{Tr}(1) = 3,\ \operatorname{Tr}(x) = 0,\ \operatorname{Tr}(x^2) = -2p$, et en tenant compte de la relation $x^3 = -px - q,\ \operatorname{Tr}(x^3) = -3q$ et $\operatorname{Tr}(x^4) = 2p^2$, d’où facilement $D_{A/K}(1, x, x^2) = -4p^3 - 27q^2$.

#### Exemple 3 {#alg-iii-s9-n5-exa-3 .statement}

Soit $A$ une algèbre de quaternions de type $(\alpha, \beta, \gamma)$ sur $K$, $(1, i, j, k)$ une base de $A$ de type $(\alpha, \beta, \gamma)$; compte tenu de III, p. 18, formule (30), on trouve aisément $\operatorname{Tr}(1) = 4,\ \operatorname{Tr}(i) = 2\beta,\ \operatorname{Tr}(j) = \operatorname{Tr}(k) = 0$, puis
$$
D_{A/K}(1, i, j, k) = -16\gamma^2(\beta^2 + 4\alpha)^2.
$$

#### Exemple 4 {#alg-iii-s9-n5-exa-4 .statement}

Soit $A = M_n(K)$, et considérons la base canonique $(E_{ij})_{1 \leq i \leq n,\ 1 \leq j \leq n}$ de $A$ sur $K$ (II, p. 142). Il est immédiat que $\operatorname{Tr}_{A/K}(E_{ij}) = 0$ si $j \neq i$ et $\operatorname{Tr}_{A/K}(E_{ii}) = n$ pour tout $i$; on en déduit sans peine que la matrice $(\operatorname{Tr}(E_{ij}E_{hk}))$ d’ordre $n^2$ est de la forme $n.P$, où $P$ est une matrice de permutation, d’où $D_{A/K}((E_{ij})) = \pm n^{n^2}$.

## EXERCICES {#alg-iii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
