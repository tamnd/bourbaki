---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 17
section_title: Normes et traces réduites
lang: fr
source: alg-viii-fr
book_pages: A VIII.329-A VIII.346
pdf_pages: 0332-0349
extraction: native
subsections:
    - "no": 1
      title: Compléments sur les polynômes caractéristiques
      page: 329
      pdf_page: 332
    - "no": 2
      title: Normes et traces réduites
      page: 332
      pdf_page: 335
    - "no": 3
      title: Propriétés des normes et traces réduites
      page: 335
      pdf_page: 338
    - "no": 4
      title: La norme réduite est une fonction polynomiale
      page: 338
      pdf_page: 341
    - "no": 5
      title: Transitivité des normes et traces réduites
      page: 340
      pdf_page: 343
    - "no": 6
      title: Normes réduites et déterminants
      page: 342
      pdf_page: 345
statements: 31
exercises: 7
content_sha256: b9634ee5e08be21d698f37ef6fdb5ac8a82f2817fee987456b8d1b6d148de5a4
---

## § 17. NORMES ET TRACES RÉDUITES

Dans ce paragraphe on désigne par K un corps commutatif et par A une K-algèbre centrale simple de degré fini. On note $n$ le degré réduit de A.

### 1. Compléments sur les polynômes caractéristiques

Soient L un anneau commutatif et M un L-module libre de dimension finie $m$. Si $u$ est un endomorphisme de M et $r$ un entier positif, on note $c_r(u)$ la trace de

l’endomorphisme $\wedge^r(u)$ du L-module libre $\wedge^r(M)$. On a en particulier

(1) $c_0(u) = 1,c_1(u) =$ Tr($u$)$,c_m(u) =$ det($u$)

et $c_r(u) = 0$ pour $r > m$. D’après la prop. 7 de III, p. 94, L’application $u\rightarrow$ det($u$) de End(M) dans L est polynomiale homogène de degré $m$ (IV, p. 52). Plus généralement, pour tout entier $r$ tel que $0\leqslant r\leqslant m$, l’application $c_r$ de End(M) dans L est polynomiale homogène de degré $r$; cela résulte de la prop. 10 de III, p. 96.

Soient $u$ un endomorphisme de M et $u$ l’endomorphisme du L[X]-module M[X] = $M\otimes_LL[X]$ déduit de $u$ par extension des scalaires (II, p. 83). On rappelle (III, p. 107, déf. 3 et (50)) que le polynôme caractéristique de $u$ est le déterminant $\chi_u(X)$ du L[X]-endomorphisme $X-u$ de M[X] et que l’on a la relation

$$
\chi_u(X) =\sum_r^m_{=0}(-1)^rc_r(u) X^{m-r} \tag{2}
$$

#### Proposition 1 {#alg-viii-s17-prop-1 .statement tag=00KD}

Soient L un anneau commutatif, M un L-module libre de dimension finie $m\geqslant 1$et $u$ un endomorphisme de M. Il existe un endomorphisme $\widetilde{u}$ de M, et un seul, satisfaisant à la relation

(3) $\widetilde{u}(x)\wedge w=x\wedge \wedge^{m-1}(u)(w)$ pour $x\in M$et $w\in \wedge^{m-1}(M)$. De plus, on a les relations

(4) $u\circ \widetilde{u}=\widetilde{u}\circ u=$ det($u$)$_M$, (5) det($\widetilde{u}$) $=$ det($u$)$^{m-1}$, (6) $\widetilde{u}=^m\sum_{r=0}^{-1}(-1)^rc_{m-1-r}(u)u^r$.

#### Lemme 1 {#alg-viii-s17-lem-1 .statement tag=00KE}

Soit $p$ un entier tel que $0\leqslant p\leqslant m$. Pour tout $w$ dans $\wedge^p(M)$, soit $h_p(w)$l’application linéaire $w'\rightarrow w\wedge w'$ de $\wedge^{m-p}(M)$dans $\wedge^m(M)$. L’application linéaire $h_p:w\rightarrow h_p(w)$de $\wedge^p(M)$dans Hom$_L(\wedge^{m-p}(M),\wedge^m(M))$est un isomor-

phisme.

Soit $(e_i)_{i\in I}$ une base de M ; munissons l’ensemble I d’une relation d’ordre total. Pour toute partie J de I, posons $e_J=e_{i_1}\wedge  \cdots  \wedge e_{i_r}$, où $(i_1, . . . , i_r)$ est la suite des

éléments de J rangés par ordre croissant. Le L-module $\wedge^{m-p}(M)$ admet pour base

les éléments $e_S$, où S parcourt l’ensemble des parties à $m-p$ éléments de I ; de

plus $\wedge^m(M)$ a pour base $\{e_I\}$. Il existe donc une base de Hom$_L(\wedge^{m-p}(M),\wedge^m(M))$

formée des applications linéaires $e^*_J$ caractérisées par la formule

$_*e_I$ si $I = J\cup S$

$$
e(e) = \tag{7}
$$

J S

0 sinon

où J parcourt l’ensemble des parties à $p$ éléments de I. Il résulte de la formule (20) de III, p. 87 que, pour toute partie J à $p$ éléments de I, on a $h_p(e_J)\in  \{e^*_J,-e^*_J\}$; comme

les éléments $e_J$ forment une base de $\wedge^p$(M), l’application linéaire $h_p$ est bijective.

Démontrons maintenant la proposition 1. Soient $u$ et $\widetilde{u}$ des endomorphismes de M. La relation (3) équivaut à

(8) $h_1\circ \widetilde{u}=$ Hom($\wedge^{m-1}(u),1\wedge^{^m}_{(M)}$)$\circ h_1$; d’après le lemme 1$,h_1$ est un isomorphisme de M sur Hom$_L(\wedge^{m-1}(M),\wedge^m(M))$.

Par suite, pour tout endomorphisme $u$ de M, il existe un unique endomorphisme $\widetilde{u}$ de M satisfaisant à la relation (3).

Soient $x_1, . . . , x_m$ des éléments de M. Remplaçons $x$ par $u(x_1)$ et $w$ par $x_2\wedge  \cdots  \wedge x_m$ dans (3) ; on obtient

$$
\widetilde{u}(u(x_1))\wedge x_2\wedge  \cdots  \wedge x_m=u(x_1)\wedge  \cdots  \wedge u(x_m)
$$

= det($u$)$x_1\wedge  \cdots  \wedge x_m$.

Par suite, $h_1(\widetilde{u}\circ u(x_1)) =h_1$(det($u$)$x_1)$, d’où la relation $\widetilde{u}\circ u=$ det($u$)$_M$ d’après le lemme 1.

Notons U l’endomorphisme $X-u$ du L[X]-module M[X] (VIII, p. 329). D’après ce qui précède, appliqué à U, il existe un endomorphisme $\widetilde{U}$ du L[X]-module M[X] qui satisfait aux relations

$$
\widetilde{U}(x_1)\wedge x_2\wedge  \cdots  \wedge x_m=x_1\wedge (Xx_2-u(x_2))\wedge  \cdots  \wedge (Xx_m-u(x_m)) \tag{9}
$$

pour $x_1, . . . , x_m$ dans M et

(10) $\widetilde{U}\circ U =$ det(X $-u)_{M[X]}$.

Considérons $\widetilde{U}$ comme un élément de End(M)[X](VIII, p. 9) ; d’après la formule (9) et le lemme 1, il est de degré $\leqslant m-1$ et on peut donc l’écrire sous la forme

$$
\widetilde{U} =^m\sum_{r=0}^{-1}(-1)^ru_rX^{m-1-r} \tag{11}
$$

où les $u_r$ sont des endomorphismes de M. D’après la formule (2) de VIII, p. 329, la relation (10) fournit l’égalité

$$
(^m\sum_{r=0}^{-1}(-1)^ru_rX^{m-1-r})(X-u) =\sum_r^m_{=0}(-1)^rc_r(u)X^{m-r} \tag{12}
$$

dans l’anneau End(M)[X]. Identifiant les coefficients des monômes en X, on obtient les relations suivantes

(13) $u_r+u_{r-1}\circ u=c_r(u)_M$ pour $1\leqslant r\leqslant m-1$,

et

$$
u_0=c_0(u)_M,u_{m-1}\circ u=c_m(u)_M \tag{14}
$$

De là, on déduit

$$
u_{m-1}=^m\sum_{r=0}^{-1}(-1)^rc_{m-1-r}(u)u^r \tag{15}
$$

or, en identifiant les termes constants, les égalités (9) et (11) entraînent $u_{m-1}=\widetilde{u}$, d’où la formule (6).

En particulier, $\widetilde{u}$ appartient à la sous-algèbre de End(M) engendrée par $u$, et il commute donc à $u$. On a déjà établi la relation $\widetilde{u}\circ u=$ det($u$)$_M$, d’où la formule (4).

Enfin, soient $x_1, . . . , x_m$ des éléments de M. Remplaçons $x$ par $x_1$ et $w$ par $\widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m)$ dans la formule (3). On obtient

$$
\widetilde{u}(x_1)\wedge \widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m) =x_1\wedge u\circ (\widetilde{u}(x_2))\wedge  \cdots  \wedge u\circ (\widetilde{u}(x_m))
$$

= det($u$)$^{m-1}x_1\wedge x_2\wedge  \cdots  \wedge x_m$, d’où la formule (5).

#### Remarque 1 {#alg-viii-s17-n1-rem-1 .statement tag=00KF}

L’endomorphisme $\widetilde{u}$ de M coïncide avec celui que nous avons appelé le cotransposé de $u$ en III, p. 99.

#### Remarque 2 {#alg-viii-s17-n1-rem-2 .statement tag=00KG}

Des formules (1), (2), (4) et (6), on déduit la relation $\chi_u(u) = 0$, d’où une autre démonstration du théorème de Hamilton-Cayley (III, p. 107).

#### Remarque 3 {#alg-viii-s17-n1-rem-3 .statement tag=00KH}

Comme l’application $c_r$ de End(M) dans L est polynomiale homogène de degré $r$ pour $0\leqslant r\leqslant m-1$, il résulte de la formule (6) que l’application $u\rightarrow \widetilde{u}$ de End(M) dans End(M) est polynomiale homogène de degré $m-1$.

Soit B une algèbre sur l’anneau L ; on suppose que B est un L-module libre de dimension $m\geqslant 1$ et l’on identifie L au sous-anneau $L\cdot 1$ de B. Soit $b$ un élément de B. Appliquons ce qui précède à l’endomorphisme $\gamma (b) :x\rightarrow bx$ du L-module B. Posons $\gamma_r(b) =c_r(\gamma (b))$ pour $0\leqslant r\leqslant m$; on a en particulier $\gamma_n(b) = N_{B/L}(b)$ (III, p. 110). Le polynôme caractéristique de $b($loc. cit.) s’écrit sous la forme

(16) Pc$_{B/L}(b; X) =\sum_r^m_{=0}(-1)^r\gamma_r(b) X^{m-r}$

Comme l’application $\gamma$ de B dans End$_L(B)$ est L-linéaire, l’application $\gamma_r$ de B dans L est polynomiale homogène de degré $r$; en particulier, l’application $b\rightarrow N_{B/L}(b)$ de B dans L est polynomiale homogène de degré $m$.

Pour tout élément $b$ de B, posons

$$
\widetilde{b}=^m\sum_{r=0}^{-1}(-1)^r\gamma_{m-1-r}(b)b^r \tag{17}
$$

D’après la proposition 1 (VIII, p. 329), l’application linéaire $\gamma (\widetilde{b})$ de B dans B est cotransposée de l’application $\gamma (b)$, et l’on en déduit

$$
b\widetilde{b}=\widetilde{b}b= N_{B/L}(b) \tag{18}
$$

De plus l’application $b\rightarrow \widetilde{b}$ de B dans B est polynomiale homogène de degré $m-1$.

### 2. Normes et traces réduites

Rappelons qu’on désigne par A une algèbre centrale simple sur le corps commutatif K, de degré réduit $n$.

#### Proposition 2 {#alg-viii-s17-prop-2 .statement tag=00KI}

Soient $a$ un élément de A et Pc($a; X$)son polynôme caractéristique. Il existe un polynôme unitaire P dans K[X], et un seul, tel que l’on ait Pc($a; X$) $= P(X)^n$.

A) L’unicité de P résulte du lemme suivant :

#### Lemme 2 {#alg-viii-s17-lem-2 .statement tag=00KJ}

Soient P et Q des polynômes unitaires de K[X] et $s$ un entier strictement positif. Si l’on a $P^s= Q^s$, on a P = Q.

Soit $\mathscr{I}$ l’ensemble des polynômes unitaires irréductibles dans K[X]. Comme P et Q sont unitaires, il existe des éléments $(a_F)$ et $(b_F)$ de $\mathbf{N}^{(\mathscr{I})}$ tels que l’on ait $P =\prod_{F\in\mathscr{I}}F^{a_F}$ et $Q =\prod_{F\in\mathscr{I}}F^{b_F}$. Il résulte de l’égalité $P^s= Q^s$ et de l’unicité de la décomposition en facteurs extrémaux qu’on a $sa_F=sb_F$ pour tout $F\in \mathscr{I}$. Comme $s$ est strictement positif, on en déduit $a_F=b_F$ pour tout $F\in \mathscr{I}$, d’où P = Q.

B) Démontrons maintenant l’existence de P.

D’après le th. 1 de VIII, p. 248, il existe une extension L de K, galoisienne et de degré fini, et un isomorphisme de L-algèbres $\theta : A_{(L)}\rightarrow \mathbf{M}_n(L)$. D’après la formule (12) de III, p. 108, le polynôme Pc($a; X$) est aussi le polynôme caractéristique de l’élément $1\otimes a$ de la L-algèbre $A_{(L)}$, donc de l’élément $\theta (1\otimes a)$ de la L-algèbre $\mathbf{M}_n(L)$.

Posons P(X) = det(X$I_n-\theta (1\otimes a))$; c’est un polynôme unitaire de L[X]. D’après l’exemple 3 de III, p. 111, on a

(19) Pc($a; X$) $= P(X)^n$.

Soit G le groupe de Galois de L sur K. Pour $\sigma \in G$, notons $\sigma$ l’automorphisme de l’anneau L[X] qui coïncide avec $\sigma$ dans L et fixe X. Alors K[X] est l’ensemble des polynômes Q de L[X] tels que l’on ait $\sigma (Q) = Q$ pour tout $\sigma \in G$ (V, p. 54, th. 1). Comme le polynôme Pc($a; X$) $= P(X)^n$ appartient à K[X], on a $\sigma (P)^n= P^n$ pour tout $\sigma \in G$. D’après le lemme 2, on a donc $\sigma (P) = P$ pour tout $\sigma \in G$; ainsi P appartient à K[X].

#### Définition 1 {#alg-viii-s17-def-1 .statement tag=00RM}

Soit $a$ un élément de l’algèbre A. On appelle polynôme caractéristique réduit de $a$ (relativement à A) l’unique polynôme unitaire de K[X], que l’on note Pcrd$_{A/K}(a; X)$, qui satisfait à la relation

(20) Pc$_{A/K}(a; X) =$ Pcrd$_{A/K}(a; X)^n$.

Soit $a$ un élément de A. Comme A est de degré $n^2$ sur K, le polynôme Pc$_{A/K}(a; X)$ est de degré $n^2$, donc Pcrd$_{A/K}(a; X)$ est un polynôme unitaire de degré $n$; écrivons-le sous la forme

(21) Pcrd$_{A/K}(a; X) = X^n+^n\sum_r^-_{=0}^1(-1)^rb_r(a)X^{n-r}$.

On pose

(22) Trd$_{A/K}(a) =b_1(a)$, Nrd$_{A/K}(a) =b_n(a)$.

#### Définition 2 {#alg-viii-s17-def-2 .statement tag=00KK}

On dit que Trd$_{A/K}(a)$est la trace réduite de $a$ et Nrd$_{A/K}(a)$sa norme réduite (relativement à la K-algèbre A).

Lorsqu’il n’y a pas de risque de confusion, on omet A et K dans les notations précédentes et l’on écrit simplement Pcrd($a; X$), Trd($a$) et Nrd($a$).

Les formules suivantes résultent des formules (20), (22) et des formules (7) et (8) de III, p. 108 :

(23) Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$

(24) $N_{A/K}(a) =$ (Nrd$_{A/K}(a))^n$.

#### Proposition 3 {#alg-viii-s17-prop-3 .statement tag=00KL}

Pour qu’un élément $a$ de A soit inversible, il faut et il suffit que sa norme réduite soit non nulle. En particulier, A est un corps si et seulement si l’on a Nrd$_{A/K}(a)\not= 0$pour tout élément non nul $a$ de A.

Pour qu’un élément $a$ de A soit inversible, il faut et il suffit que sa norme soit non nulle (III, p. 111, prop. 3). La prop. 3 résulte donc de la formule (24).

#### Remarque {#alg-viii-s17-n2-rem-1 .statement tag=00KM}

Soit L le corps K(X) des fractions rationnelles en une indéterminée X. Le polynôme caractéristique réduit d’un élément $a$ de A n’est autre que la norme réduite de l’élément $X\otimes 1-1\otimes a$ de la L-algèbre $A_{(L)}$. Cela résulte de la définition du polynôme caractéristique réduit et de la formule suivante (III, p. 111)

(25) Pc$_{A/K}(a; X) = N_{A_{(L)}/L}(X\otimes 1-1\otimes a)$.

#### Exemple 1 {#alg-viii-s17-n2-exa-1 .statement tag=00RN}

D’après le th. 1 de VIII, p. 116, il existe un entier $r\geqslant 1$ et un corps D tels que A soit isomorphe à $\mathbf{M}_r(D)$; soit $d$ le degré réduit de D sur K ; on a $r=n/d$. Soit M un A-module de longueur finie $\ell$; nous allons prouver la formule

(26) Pc$_{M/K}(a_M; X) =$ Pcrd$_{A/K}(a; X)^{d\ell}$

pour tout élément $a$ de A. Le A-module $A_s$ est de longueur $r$ (VIII, p. 117, lemme 2) ; les A-modules $M^r$ et $A^{\ell}_s$ ont même longueur, donc ils sont isomorphes, et l’on a

Pc$_{M/K}(a_M; X)^r=$ Pc$_{A/K}(a; X)^{\ell}$

d’après la formule (15) de III, p. 109. Comme on a $rd=n$, la formule (26) résulte de la formule (20) et du lemme 2 (VIII, p. 333).

#### Exemple 2 {#alg-viii-s17-n2-exa-2 .statement tag=00RO}

Considérons le cas particulier où A est l’algèbre End$_K(V)$ des endomorphismes d’un K-espace vectoriel V de dimension finie sur K. Prenant pour M le A-module simple V, on obtient les relations

(27) Pcrd$_{A/K}(u; X) =\chi_u(X)$, Nrd$_{A/K}(u) =$ det($u$) et Trd$_{A/K}(u) =$ Tr($u$)

pour tout endomorphisme $u$ de V.

### 3. Propriétés des normes et traces réduites

#### Proposition 4 {#alg-viii-s17-prop-4 .statement tag=00KN}

Soient L une extension de K et $a$ un élément de l’algèbre centrale et simple A. On a les relations

(28) Pcrd$_{A_{(L)}/L}(1\otimes a; X) =$ Pcrd$_{A/K}(a; X)$

(29) Trd$_{A_{(L)}/L}(1\otimes a) =$ Trd$_{A/K}(a)$

(30) Nrd$_{A_{(L)}/L}(1\otimes a) =$ Nrd$_{A/K}(a)$,

(« invariance par extension des scalaires » ).

Les deux membres de l’égalité (28) ont même puissance $n$-ème en vertu de la définition (formule (20) de VIII, p. 333) et de la relation

Pc$_{A_{(L)}/L}(1\otimes a; X) =$ Pc$_{A/K}(a; X)$

(III, p. 110, formule (21)). L’égalité (28) résulte donc du lemme 2 de VIII, p. 333. Les formules (29) et (30) se déduisent de (28), (21) et (22).

#### Corollaire 1 {#alg-viii-s17-prop-4-cor-1 .statement tag=00KO}

Soient L une extension de K, V un espace vectoriel de dimension $n$ sur L et $\theta$ un homomorphisme de K-algèbres de A dans End$_L(V)$. Pour tout élément $a$ de A, on a

(31) Pcrd$_{A/K}(a; X) =\chi_{\theta(a)}(X)$

(32) Trd$_{A/K}(a) =$ Tr($\theta (a)$)

(33) Nrd$_{A/K}(a) =$ det($\theta (a)$).

Soit $\theta '$ l’homomorphisme de L-algèbres de $A_{(L)}$ dans End$_L(V)$ tel que $\theta '(\lambda \otimes a) =\lambda \theta (a)$ pour $\lambda \in$ L et $a\in$ A. L’algèbre $A_{(L)}$ est simple d’après le cor. 2 de VIII, p. 217, et l’homomorphisme $\theta '$ est donc injectif. Mais les algèbres $A_{(L)}$ et End$_L(V)$ sur le corps L ont même degré, égal à $n^2$, donc $\theta '$ est un isomorphisme. Le cor. 1 résulte alors de la prop. 4 et de l’exemple 2 ci-dessus.

#### Corollaire 2 {#alg-viii-s17-prop-4-cor-2 .statement tag=00KP}

Soient $a$ et $a'$ des éléments de A et $\lambda$ un élément de K. On a les relations

(34) Pcrd$_{A/K}(a;a) = 0$,

(35) Pcrd$_{A/K}(\lambda a;\lambda X) =\lambda^n$ Pcrd$_{A/K}(a; X)$,

(36) Trd$_{A/K}(a+a') =$ Trd$_{A/K}(a) +$ Trd$_{A/K}(a')$, Trd$_{A/K}(\lambda a) =\lambda$ Trd$_{A/K}(a)$,

(37) Trd$_{A/K}(aa') =$ Trd$_{A/K}(a'a)$,

(38) Nrd$_{A/K}(aa') =$ Nrd$_{A/K}(a)\cdot$ Nrd$_{A/K}(a')$, Nrd$_{A/K}(\lambda a) =\lambda^n$ Nrd$_{A/K}(a)$,

(39) Trd$_{A/K}(1) =n$, Nrd$_{A/K}(1) = 1$.

Comme A est centrale, simple et de degré réduit $n$ sur K, il existe une extension L de K et un espace vectoriel V de dimension $n$ sur L tels que $A_{(L)}$ soit isomorphe à l’algèbre End$_L(V)$ (VIII, p. 248, th. 1) Le corollaire 2 résulte alors du corollaire 1 et des propriétés de la trace et du déterminant d’un endomorphisme. En particulier, la formule (34) résulte du théorème de Hamilton-Cayley (III, p. 107, prop. 20).

#### Corollaire 3 {#alg-viii-s17-prop-4-cor-3 .statement tag=00RP}

Soit $A^o$ l’algèbre opposée de A. Pour tout $a$ dans A, on a

(40) Pcrd$_{A^o/K}(a; X) =$ Pcrd$_{A/K}(a; X)$

(41) Trd$_{A^o/K}(a) =$ Trd$_{A/K}(a)$

(42) Nrd$_{A^o/K}(a) =$ Nrd$_{A/K}(a)$.

Choisissons une extension L de K, un espace vectoriel V de dimension $n$ sur L et un homomorphisme $\theta$ de A dans End$_L(V)$ (VIII, p. 248, th. 1). Soit $V^*$ l’espace vectoriel dual de V. L’application qui associe à un élément $a$ de A l’endomorphisme $^t\theta (a)$ de $V^*$ est un homomorphisme de K-algèbres de $A^o$ dans End$_L(V^*)$. Le corollaire 3 résulte alors du cor. 1 et du cor. 3 de III, p. 95.

La trace, la norme et le polynôme caractéristique de $a$ sont donc les mêmes, $\dbend$ qu’on considère $a$ comme élément de A ou de $A^o$. Cette propriété n’est pas toujours satisfaite lorsque A n’est plus supposée centrale et simple (III, p. 196, exerc. 1 du § 9).

#### Proposition 5 {#alg-viii-s17-prop-5 .statement tag=00KQ}

Pour tout x dans A, soit $t_x$ la forme linéaire $y\rightarrow$ Trd$_{A/K}(xy)$ sur A.

a) L’application $t:x\rightarrow t_x$ est un isomorphisme de $(A,A)$-bimodules de A sur son dual Hom$_K(A,K)$.

b) Soit $h$ une forme linéaire sur A. Les conditions suivantes sont équivalentes :

(i) Il existe un élément $\lambda$ de K tel que $h(x) =\lambda$ Trd$_{A/K}(x)$pour tout $x\in A$;

(ii) On a $h(xy) =h(yx)$quels que soient $x, y$ dans A.

Rappelons (II, p. 34) que la structure de $(A$, A)-bimodule sur $A^*=$ Hom$_K(A,K)$ est définie par la relation

$$
\langle atb, c\rangle =\langle t, bca\rangle \tag{43}
$$

pour $a, b, c\in A$ et $t\in A^*$. En particulier, pour tout $x$ dans A, on a

$\langle at_xb, c\rangle =\langle t_x, bca\rangle =$ Trd$_{A/K}(xbca)$

$\langle t_{axb}, c\rangle =$ Trd$_{A/K}(axbc)$

et ces deux éléments sont égaux d’après la formule (37) de VIII, p. 336. On a donc $at_xb=t_{axb}$, ce qui signifie que $t$ est un homomorphisme de $(A$, A)-bimodules de A dans $A^*$.

Choisissons une extension L du corps K et un isomorphisme $\theta$ de la L-algèbre $A_{(L)}$ sur l’algèbre des matrices $\mathbf{M}_n(L)$ (VIII, p. 248, th. 1). Identifions l’espace vectoriel $(A^*)_{(L)}$ au dual de l’espace vectoriel $A_{(L)}$ sur le corps L. D’après la prop. 4 de VIII, p. 335, on a, avec ces conventions,

(44) Trd$_{A_{(L)}/L}= 1_L\otimes$ Trd$_{A/K}$.

Soit $t_{(L)}$ l’application L-linéaire de $A_{(L)}$ dans $A^*_{(L)}$ déduite de $t$ par extension des scalaires ; d’après la formule (44) et le cor. 1 de VIII, p. 335, on a

(45) $\langle t_{(L)}(x), y\rangle =$ Trd$_{A_{(L)}/L}(xy) =$ Tr($\theta (x)\theta (y)$)

pour $x, y$ dans $A_{(L)}$. D’après la prop. 7 de II, p. 158, l’application $t_{(L)}$ est bijective, d’où il résulte que $t$ est bijective. On a prouvé a).

Soit $h$ dans $A^*$; d’après ce qui précède, il existe un élément $a$ de A tel que $h$ soit égal à $t_a$. D’après a), on a

$$
h(xy)-h(yx) =t_a(xy-yx) =t_{ax}(y)-t_{xa}(y)
$$

Par suite, la relation « $h(xy) =h(yx)$ pour $x, y$ dans A » équivaut à « $t_{ax-xa}= 0$ pour tout $x\in A$ », et d’après la partie a) de la démonstration, ceci signifie que $a$ appartient au centre K de A. Cela prouve b), compte tenu de la formule (36).

#### Corollaire {#alg-viii-s17-n3-cor-1 .statement tag=00KR}

Le sous-espace vectoriel de A engendré par les éléments de la forme $xy-yx$, où $x$ et $y$ parcourent A, est un hyperplan, noyau de la forme linéaire non nulle Trd$_{A/K}$.

#### Remarque {#alg-viii-s17-n3-rem-1 .statement tag=00KS}

D’après la formule (23) de VIII, p. 334, on a

Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$ pour tout $a\in A$. Si la caractéristique du corps K est égale à 0 ou à un nombre premier $p$ ne divisant pas $n$, on peut remplacer la trace réduite par la trace dans la prop. 5. Par contre, si la caractéristique de K est un nombre premier divisant $n$, on a Tr$_{A/K}(a) = 0$ pour tout $a\in A$.

### 4. La norme réduite est une fonction polynomiale

#### Lemme 3 {#alg-viii-s17-lem-3 .statement tag=00KT}

Soient L une extension de K, I un ensemble, $\mathbf{T} = (T_i)_{i\in I}$ une famille d’indéterminées. On a $K(\mathbf{T})\cap L[\mathbf{T}] = K[\mathbf{T}]$.

Soient P et Q des éléments de $K[\mathbf{T}]$, avec $Q\not= 0$. Les coefficients des polynômes $R\in L[\mathbf{T}]$ tels que P = QR sont les solutions d’un système d’équations linéaires à coefficients dans K. Par suite, s’il existe un polynôme $R\in L[\mathbf{T}]$ tel que P = QR, il en existe un aussi dans $K[\mathbf{T}]$ (II, p. 123, prop. 6). Cela prouve l’inclusion $K(\mathbf{T})\cap L[\mathbf{T}]\subset K[\mathbf{T}]$; l’inclusion opposée est évidente.

Rappelons que le polynôme caractéristique réduit d’un élément $a$ de A s’écrit (46) Pcrd$_{A/K}(a; X) =\sum_{r=0}^n(-1)^rb_r(a) X^{n-r}$

et que l’on a

$b_0(a) = 1,b_1(a) =$ Trd$_{A/K}(a),b_n(a) =$ Nrd$_{A/K}(a)$.

#### Proposition 6 {#alg-viii-s17-prop-6 .statement tag=00KU}

Pour tout entier $r$ tel que $0\leqslant r\leqslant n$, l’application $b_r$ de A dans K est polynomiale homogène de degré $r$. En particulier, la norme réduite est une application polynomiale homogène de degré $n$ de A dans K.

Soit $(e_i)_{i\in I}$ une base de A sur K et $\mathbf{T} = (T_i)_{i\in I}$ une famille d’indéterminées.

#### Lemme 4 {#alg-viii-s17-lem-4 .statement tag=00KV}

Soit $u$ l’élément $\sum_{i\in I}T_i\otimes e_i$ de la $K(\mathbf{T})$-algèbre centrale et simple $A_{(K(\mathbf{T}))}$. Soit P le polynôme caractéristique réduit de cet élément $u$. Alors P appartient à l’anneau $K[\mathbf{T}][X]$;considéré comme élément de l’anneau $K[\mathbf{T},X]$, il est homogène de degré $n$.

Choisissons une extension L de K et un isomorphisme $\theta$ de L-algèbres de $A_{(L)}$ sur $\mathbf{M}_n(L)$. Notons $\theta : A_{(L(\mathbf{T}))}\rightarrow \mathbf{M}_n(L(\mathbf{T}))$ l’isomorphisme de $L(\mathbf{T}$)-algèbres déduit de $\theta$ par extension des scalaires. D’après le cor. 1 de VIII, p. 335, on a

(47) $P(X) =\chi_{\theta(u)}(X) =$ det(X$I_n-\theta (u)) =$ det$(XI_n-\sum_{i\in I}T_i\theta (1\otimes e_i))$.

Comme les matrices $\theta (1\otimes e_i)$ appartiennent à $\mathbf{M}_n$(L), cette formule montre que P est un polynôme homogène de degré $n$ dans $L[\mathbf{T},X]$. Il appartient aussi à $K(\mathbf{T})[X]$ et il s’écrit sous la forme $P(X) =\sum_{j\geqslant 0}c_jX^j$, où chaque $c_j$ appartient à $K(\mathbf{T})\cap L[\mathbf{T}]$. D’après le lemme 3, chacun des éléments $c_j$ appartient à $K[\mathbf{T}]$, d’où le lemme 4.

#### Lemme 5 {#alg-viii-s17-lem-5 .statement tag=00KW}

Pour toute extension $K'$ de K et tout élément $(t_i)_{i\in I}$ de $K'^I$, on a

(48) Pcrd$_{A_{(K')}/K'}(\sum t_i\otimes e_i)= P((t_i)_{i\in I},X)$.

Soit $\varphi : K[\mathbf{T}]\rightarrow K'$ l’unique homomorphisme de K-algèbres qui transforme$^{i\in I}$ $T_i$ en $t_i$ pour tout $i\in$ I ; il définit sur $K'$ une structure de $K[\mathbf{T}$]-algèbre. La $K'$-algèbre $A_{(K[}(\sum_{\mathbf{T}])(K')}$ s’identifie à $A)_{(K')}$ (transitivité de l’extension des scalaires), l’élément $1\otimes T_i\otimes e_i$ s’identifiant à l’élément $\sum t_i\otimes e_i$ de $A_{(K')}$. Notons $\varphi : K[\mathbf{T}][X]\rightarrow K'[X]$ l’homomorphisme de K-algèbres déduit de $\varphi$. D’après la formule (21) de III, p. 110, le polynôme caractéristique de $\sum t_i\otimes e_i$ relativement à la $K'$-algèbre $A_{(K')}$ est l’image par $\varphi$ du polynôme caractéristique de $\sum T_i\otimes e_i$ relativement à la $K[\mathbf{T}$]-algèbre $A_{(K[\mathbf{T}])}$, c’est-à-dire de $P^n$. Autrement dit, on a

(49) Pc$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i; X) = P((t_i)_{i\in I},X)^n$;

le lemme 5 résulte alors du lemme 2 de VIII, p. 333.

Considérons le cas particulier $K'= K$ du lemme 5. On a

(50) Pcrd$_{A/K}(\sum_{i\in I}t_ie_i; X)= P((t_i)_{i\in I},X)$

quel que soit l’élément $(t_i)_{i\in I}$ de $K^I$. Comme le polynôme P de $K[\mathbf{T},X]$ est homogène de degré $n$, il se développe sous la forme

$$
P(\mathbf{T},X) =\sum_{r=0}^n(-1)^rB_r(\mathbf{T}) X^{n-r} \tag{51}
$$

où $B_r$ est un polynôme homogène de degré $r$ dans $K[\mathbf{T}]$. D’après les formules (46), (50) et (51), on a

$$
b_r(\sum_{i\in I}t_ie_i)= B_r((t_i)_{i\in I})
$$

quel que soit l’élément $(t_i)_{i\in I}$ de $K^I$, d’où la proposition 6.

#### Remarque {#alg-viii-s17-n4-rem-1 .statement tag=00KX}

Soit $K'$ une K-algèbre commutative. Tout élément $t$ de $A_{(K')}$ s’écrit sous la forme $\sum_{i\in I}t_i\otimes e_i$, avec $(t_i)\in K'^I$. Il ressort de la démonstration du lemme 5 que le polynôme caractéristique Pc$_{A_{(K')}/K'}(t; X)$ est égal à $P((t_i),X)^n$.

### 5. Transitivité des normes et traces réduites

#### Proposition 7 {#alg-viii-s17-prop-7 .statement tag=00KY}

Soient L une sous-algèbre semi-simple commutative maximale de A et $a$ un élément de L. On a

(52) Pcrd$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(53) Trd$_{A/K}(a) =$ Tr$_{L/K}(a)$,

(54) Nrd$_{A/K}(a) = N_{L/K}(a)$.

D’après la prop. 3 de VIII, p. 258, les L-modules A et $L^n$ sont isomorphes, d’où la relation

Pc$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)^n$

Comme le polynôme Pc$_{L/K}(a; X)$ est unitaire, il est donc égal au polynôme caractéristique réduit Pcrd$_{A/K}(a; X)$ (VIII, p. 333, lemme 2), d’où la formule (52). En comparant dans les deux membres de (52) les coefficients de $X^{n-1}$ (resp. les termes constants), on obtient la formule (53) (resp. (54)).

#### Corollaire {#alg-viii-s17-n5-cor-1 .statement tag=00KZ}

Soit D un corps de centre K, et de degré fini sur K. Soient $a$ un élément de K et L un sous-corps commutatif maximal de D contenant $a$. On a

(55) Pcrd$_{D/K}(a; X) =$ Pc$_{L/K}(a; X)$, Tr$_{D/K}(a) =$ Tr$_{L/K}(a)$, Nrd$_{D/K}(a) = N_{L/K}(a)$.

En effet, un sous-corps commutatif maximal L de D est une sous-algèbre semi-simple commutative maximale de D d’après le cor. 2 de VIII, p. 261.

#### Proposition 8 {#alg-viii-s17-prop-8 .statement tag=00L0}

Soit B une sous-algèbre simple de A. Notons L le centre de B et $B'$ le commutant de B dans A. Alors $B'$ est une algèbre centrale et simple sur le corps L ; notons $r$ son degré réduit. Pour tout élément $b$ de B, on a les relations

(56) Pcrd$_{A/K}(b; X) = N_{L[X]/K[X]}$(Pcrd$_{B/L}(b; X))^r$

(57) Trd$_{A/K}(b) =r$ Tr$_{L/K}$(Trd$_{B/K}(b))$

(58) Nrd$_{A/K}(b) = N_{L/K}$(Nrd$_{B/L}(b))^r$.

#### Lemme 6 {#alg-viii-s17-lem-6 .statement tag=00L1}

Soient $K'$ une algèbre commutative de degré fini $d$ sur K et

$$
P(X) = X^s+a_1X^{s-1}+\cdots +a_s
$$

un polynôme unitaire à coefficients dans $K'$. Le polynôme $Q = N_{K'[X]/K[X]}(P)$de K[X] est unitaire de degré $sd$, le coefficient de $X^{sd-1}$ dans Q(X) est égal à Tr$_{K'/K}(a_1)$, et son terme constant est $N_{K'/K}(a_s)$.

Notons $K''$ la $K'$-algèbre $K'[T]/(P(T))$ et $t$ la classe de canonique de T dans $K''$. La suite $(1, t, . . . , t^{s-1})$ est une base de $K''$ sur $K'$ et la matrice de la multiplication par $t$ dans cette base est de la forme

0 0 $. .$. 0 $-a_s$

1 0 $. .$. 0 $-a_{s-1}$

(59) $\tau =$ 0 1 $. .$. 0 $-a_{s-2}$.

$$
\cdot  \cdot . . .\cdot \cdot
$$

$$
\cdot  \cdot . . .\cdot \cdot
$$

0 $\cdot . .$. 1 $-a_1$

Le calcul du déterminant de X$I_n-\tau$ se fait par récurrence sur $s$, en développant selon la première ligne. On trouve det(X$I_n-\tau ) = P(X)$. Autrement dit, on a P(X) = Pc$_{K''/K'}(t; X)$. En particulier, Tr$_{K''/K'}(t) =-a_1$ et $N_{K''/K'}(t) = (-1)^sa_s$. Compte tenu de la formule de transitivité (III, p. 114, cor.), on a

Tr$_{K''/K}(t) =-$ Tr$_{K'/K}(a_1),N_{K''/K}(t) = (-1)^{sd}N_{K'/K}(a_s)$ et Q(X) = Pc$_{K''/K}(t; X)$.

D’autre part, $[K'': K] = [K'': K'][K': K] =sd$, donc Q(X) est un polynôme unitaire de degré $sd$. Le lemme 6 résulte de là.

Démontrons la prop. 8. Comme l’anneau B est simple, son centre L est un corps (VIII, p. 117, cor. 1). D’après le th. 5 de VIII, p. 255, le commutant $B'$ de B dans A est un anneau simple de centre L et l’on a $[A : K] = [B : K][B': K]$. Notons $r$ le degré réduit de $B'$ sur $L,s$ celui de B sur L et $d$ le degré de L sur K. On a

$$
[A : K] =n^2,[B': K] =r^2d,[B : K] =s^2d
$$

d’où $n^2=r^2s^2d^2$, c’est-à-dire $n=rsd$.

Soit $b$ un élément de B et soit P(X) son polynôme caractéristique réduit dans la L-algèbre B ; il est unitaire de degré $s$. D’après le lemme 6, le polynôme $Q = N_{L[X]/K[X]}(P)$ est unitaire de degré $sd$. Le polynôme $R = Q^r$ est donc unitaire de degré $rsd=n$. Toujours d’après le lemme 6, le coefficient de $X^{n-1}$ dans R(X) est égal à $-r$ Tr$_{L/K}$(Trd$_{B/L}(b))$ et le terme constant de R(X) est $(N_{L/K}((-1)^s$ Nrd$_{B/L}(b)))^r= (-1)^nN_{L/K}$(Nrd$_{B/L}(b))^r$.

Comme $[A : K] =r^2d[B : K]$, le B-module à gauche A est libre de dimension $r^2d$ (VIII, p. 120, prop. 5). On a donc

(60) Pc$_{A/K}(b; X) =$ Pc$_{B/K}(b; X)^{dr^2}$;

d’après le corollaire de III, p. 114, on a

(61) Pc$_{B/K}(b; X) = N_{L[X]/K[X]}$(Pc$_{B/L}(b; X))$ et comme P(X) est le polynôme caractéristique réduit de $b$ dans la L-algèbre B, on a

(62) Pc$_{B/L}(b; X) = P(X)^s$.

Compte tenu des formules (60) à (62) et de la définition de R(X), on a finalement

(63) Pc$_{A/K}(b; X) = N_{L[X]/K[X]}(P(X))^{dr^2s}= Q(X)^{dr^2s}= R(X)^{rsd}= R(X)^n$,

donc R(X) est le polynôme caractéristique réduit de $b$ dans la K-algèbre A.

On a prouvé la formule (56). Les formules (57) et (58) résultent aussitôt de la formule (56) et du lemme 6 puisque le coefficient de $X^{n-1}$ dans Pcrd$_{A/K}(b; X)$ est égal à $-$ Trd$_{A/K}(b)$, et que son terme constant est $(-1)^n$ Nrd$_{A/K}(b)$.

### 6. Normes réduites et déterminants

Dans ce numéro, on note D un corps de centre K et de degré fini sur K. On note $D^*_{ab}$ le quotient du groupe multiplicatif $D^*$ par son groupe dérivé et $\pi$ l’homomorphisme canonique de $D^*$ sur $D^*_{ab}$. L’application Nrd$_{D/K}$ induit un homomorphisme de groupes de $D^*$ dans $K^*$; le noyau de cet homomorphisme contient le groupe dérivé de $D^*$ puisque K est commutatif. Il existe donc un homomorphisme Nrd de $D^*_{ab}$ dans $K^*$, et un seul, tel que Nrd$_{D/K}(x) =$ Nrd $\circ \pi (x)$ pour tout $x\in D^*$.

#### Proposition 9 {#alg-viii-s17-prop-9 .statement tag=00L2}

Soit V un espace vectoriel à droite sur le corps D, de dimension finie. Soit E l’algèbre End$_D(V)$sur le corps K ; elle est centrale, simple et de degré fini. Pour tout élément inversible $u$ de E, on a

(64) Nrd$_{E/K}(u) =$ Nrd(det $u)$

(cf. VIII, p. 442, prop. 2 pour la définition du déterminant det $u$ de $u)$.

Notons $n$ la dimension de V sur D et identifions E à l’algèbre de matrices $\mathbf{M}_n(D)$ au moyen d’une base de V sur D. Le groupe multiplicatif GL$_n(D)$ de l’algèbre E est engendré par les matrices diagonales et les matrices $B_{ij}(\lambda )$ (II, p. 162, cor. 1). La prop. 9 résulte donc des deux cas particuliers ci-dessous.

A) Supposons que $u$ soit la matrice diagonale diag($a_1, . . . , a_n$). Pour $1\leqslant i\leqslant n$, soit $L_i$ un sous-corps commutatif maximal de D contenant $a_i$; soit L la sous-algèbre de E formée des matrices diagonales diag($t_1, . . . , t_n$) avec $t_i\in L_i$ pour $1\leqslant i\leqslant n$. Soit $d$ le degré réduit de D sur K. On a $[L_i: K] =d$ pour $1\leqslant i\leqslant n$ (VIII, p. 261, cor. 2). La K-algèbre L est isomorphe à $L_1\times  \cdots  \times L_n$, donc est semi-simple de degré $nd$; or on a $[E : K] =n^2[D : K] =n^2d^2= [L : K]^2$. Il en résulte que L est une sous-algèbre semi-simple commutative maximale de E (VIII, p. 258, prop. 3). D’après la prop. 7 de VIII, p. 340, on a Nrd$_{E/K}(u) = N_{L/K}(u)$, d’où, compte tenu de la formule (18) de III, p. 110,

Nrd$_{E/K}(u) =_i\prod_{=1}^nN_{L_i/K}(a_i) =\prod_{i=1}^n$ Nrd$_{D/K}(a_i)$

= Nrd$_{D/K}(a_1. . . a_n) =$ Nrd($\pi (a_1. . . a_n)$).

Par ailleurs, on a det $u=\pi (a_1. . . a_n)$ d’après la prop. 3 de VIII, p. 443, d’où la formule (64) dans ce cas.

B) Supposons que $u$ soit égal à $B_{ij}(\lambda )$, où $\lambda$ est un élément de D et $i, j$ des entiers distincts dans l’intervalle $[1, n]$. Notons $d$ le degré réduit de D sur K et M l’espace vectoriel sur K déduit de V par restriction des scalaires de D à K. Alors M est un E-module simple et l’on a

(65) Pc$_{M/K}(u; X) =$ Pcrd$_{E/K}(u; X)^d$

d’après la formule (26) de VIII, p. 334. Par ailleurs, M est un espace vectoriel de dimension $nd^2$ sur K, et $u-1_M$ est un endomorphisme nilpotent de M ; on a donc (66) Pc$_{M/K}(u; X) = (X-1)^{nd^2}$.

Par comparaison des formules (65) et (66), on trouve

(67) Pcrd$_{E/K}(u; X) = (X-1)^{nd}$

et en particulier Nrd$_{E/K}(u) = 1$. Par ailleurs, on a det $u= 1$ d’après la prop. 3 de VIII, p. 443 ; la formule (64) est donc établie dans ce cas.

#### Remarque {#alg-viii-s17-n6-rem-1 .statement tag=00L3}

On a Nrd$_{E/K}(u) = 0$ si l’élément $u$ de E n’est pas inversible (VIII, p. 334, prop. 3).

## EXERCICES {#alg-viii-s17-exercises}

See the [exercises for § 17](exercises/s17/).
