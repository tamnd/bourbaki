---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 9
section_title: Complexes de Koszul
lang: fr
source: alg-x-fr
book_pages: A X.147-A X.168, A X.206-A X.209
pdf_pages: 0153-0174, 0212-0215
extraction: ocr
subsections:
    - "no": 1
      title: Les complexes $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$
      page: 147
      pdf_page: 153
    - "no": 2
      title: Fonctorialité
      page: 150
      pdf_page: 156
    - "no": 3
      title: 'Exemple 1 : le complexe $S(L) \otimes_A \Lambda(L)$'
      page: 151
      pdf_page: 157
    - "no": 4
      title: 'Exemple 2 : le cas d’un module libre'
      page: 153
      pdf_page: 159
    - "no": 5
      title: 'Exemple 3 : le cas $L = A$'
      page: 156
      pdf_page: 162
    - "no": 6
      title: Familles complètement sécantes
      page: 157
      pdf_page: 163
    - "no": 7
      title: Un critère pour les suites complètement sécante
      page: 159
      pdf_page: 165
    - "no": 8
      title: 'Démonstration du théorème 1 : première partie'
      page: 161
      pdf_page: 167
    - "no": 9
      title: 'Démonstration du théorème 1 : deuxième partie'
      page: 163
      pdf_page: 169
    - "no": 10
      title: Classe d’extensions associée à une suite régulière
      page: 165
      pdf_page: 171
statements: 35
exercises: 10
content_sha256: 234fe2945aa4e961036016372d407d506dc8b4e0d5b9dad9251bdb87e41d0c74
---

## § 9. COMPLEXES DE KOSZUL

Dans ce paragraphe, tous les anneaux considérés sont commutatifs.

### 1. Les complexes $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$

Soient $A$ un anneau, $L$ un $A$-module, $u : L \to A$ une forme linéaire, et $\Lambda(L)$ l’algèbre extérieure du $A$-module $L$. Pour $x \in \Lambda(L)$, notons $d_u(x)$ le produit intérieur $x \cdot u$ (III, p. 161, exemple). D’après loc. cit., p. 162, formule (60), on a

$$
(1)\quad d_u(e_1 \wedge \ldots \wedge e_n) = \sum_{i=1}^n (-1)^{i+1} u(e_i) \; e_1 \wedge \ldots \wedge e_{i-1} \wedge e_{i+1} \wedge \ldots \wedge e_n
$$

pour $e_1, \ldots, e_n$ dans $L$. D’après III, p. 164 et 165, l’application $d_u : \Lambda(L) \to \Lambda(L)$ est une antidérivation de degré $(-1)$ et de carré nul. C’est l’unique antidérivation de la $A$-algèbre $\Lambda(L)$ qui prolonge $u : \Lambda^1(L) \to \Lambda^0(L)$.

#### Définition 1 {#alg-x-s9-def-1 .statement}

Le complexe $(\Lambda(L), d_u)$ se note $\mathbf{K}^A(u)$ ou $\mathbf{K}(u)$.

On prendra garde que $\mathbf{K}_n(u) = \Lambda^n(L) = \mathbf{K}^{-n}(u)$. Il est clair que $\mathbf{K}(u)$ est nul à droite et que $H_0(\mathbf{K}(u)) = \mathrm{Coker}\,(u) = A/q$ où $q$ est l’idéal $u(L)$ de $A$.

Pour tout complexe de $A$-modules $C$, on pose

$$
\begin{aligned}
\mathbf{K}^A(u, C) &= C \otimes_A \mathbf{K}^A(u), \\
H^A(u, C) &= H(C \otimes_A \mathbf{K}^A(u)) \\
H_r^A(u, C) &= H_r(C \otimes_A \mathbf{K}^A(u)),
\end{aligned}
$$
$$
\begin{aligned}
\mathbf{K}^*_A(u, C) &= \mathrm{Homgr}_A(\mathbf{K}^A(u), C), \\
H^*_A(u, C) &= H(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)), \\
H^r_A(u, C) &= H^r(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)).
\end{aligned}
$$

On a donc des homomorphismes canoniques de $A$-modules (X, p. 62 et p. 82)

$$
\begin{aligned}
\gamma_0 : H_0(C) \otimes_A A/q &\to H^A_0(u, C), \\
\lambda^0 : H^0_A(u, C) &\to \mathrm{Hom}_A(A/q, H^0(C)).
\end{aligned}
$$

#### Lemme 1 {#alg-x-s9-lem-1 .statement}

Si le complexe $C$ est nul à droite (resp. à gauche), alors $\mathbf{K}^A(u, C)$ (resp. $\mathbf{K}^*_A(u, c)$) est nul à droite (resp. à gauche), et $\gamma_0$ (resp. $\lambda^0$) est bijectif.

Cela résulte de X, p. 62, prop. 1 et p. 82, prop. 1.

#### Proposition 1 {#alg-x-s9-prop-1 .statement}

Soit $x \in L$; notons $R_x : y \mapsto x \wedge y$ la multiplication à gauche par $x$ dans l’algèbre $\Lambda(L)$. Alors $d_u \circ R_x + R_x \circ d_u = u(x) \cdot 1_{\Lambda(L)} = u(x)_{\Lambda(L)}$.

En effet $(d_u \circ R_x + R_x \circ d_u)(y) = d_u(x \wedge y) + x \wedge d_u(y)$; puisque $d_u$ est une antidérivation, $d_u(x \wedge y) + x \wedge d_u(y) = d_u(x) \wedge y = u(x) \cdot y$.

#### Corollaire 1 {#alg-x-s9-prop-1-cor-1 .statement}

Si $u$ est surjectif, $K(u)$ est homotope à zéro (X, p. 34) ainsi que $K^A(u, C)$ et $K_A^*(u, C)$ pour tout complexe $C$.

En effet, il existe $x \in L$ tel que $u(x) = 1$. Alors $K(u)$ est homotope à zéro d’après la prop. 1, donc aussi $K^A(u, C)$ (X, p. 64, prop. 3) et $K_A^*(u, C)$ (X, p. 83, prop. 3).

#### Corollaire 2 {#alg-x-s9-prop-1-cor-2 .statement}

Soient $C$ un complexe, Ann (C) son annulateur. Alors $q + \mathrm{Ann}(C)$ annule $H^A(u, C)$ et $H_A^*(u, C)$.

Pour tout $\lambda \in q$, l’homothétie $\lambda_{K(u)}$ est homotope à zéro d’après la proposition, donc aussi $1_C \otimes \lambda_{K(u)}$ et Homgr ($\lambda_{K(u)}, 1_C$) d’après X, p. 64, prop. 3 et X, p. 83, prop. 3 ; il s’ensuit que $\lambda$ annule $H(u, C)$ et $H^*(u, C)$. Si $\lambda \in \mathrm{Ann}(C)$, alors $1_{K(u)} \otimes \lambda_C$ et Homgr ($1_{K(u)}, \lambda_C$) sont nuls.

Supposons $L$ projectif (resp. $K(u)$ acyclique en degrés > 0). Alors le complexe $\Lambda(L)$ est projectif d’après III, p. 87, cor. 2 (resp. est une résolution de $A/q$) ; d’après X, p. 102 (resp. p. 100), on a donc, pour tout $A$-module $M$, des homomorphismes

(2) $H_r^A(u, M) \to \mathrm{Tor}_r^A(A/q, M)$, $\mathrm{Ext}_A^r(A/q, M) \to H_r^A(u, M)$
resp.
(3) $\mathrm{Tor}_r^A(A/q, M) \to H_r^A(u, M)$, $H_r(u, M) \to \mathrm{Ext}_A^r(A/q, M)$.

Si $L$ est projectif et $K(u)$ acyclique en degrés > 0, les homomorphismes (2) et (3) ci-dessus sont bijectifs et réciproques les uns des autres (X, p. 102, prop. 1).

#### Proposition 2 {#alg-x-s9-prop-2 .statement}

Soit $(L_i)_{i \in I}$ une famille de $A$-modules, où l’ensemble $I$ est fini et totalement ordonné. Soient $u$ une forme linéaire sur $\bigoplus_{i \in I} L_i$, $u_i$ sa restriction à $L_i$.

L’isomorphisme canonique de $A$-algèbres (III, p. 84)

$$
g : \bigotimes_{i \in I} \Lambda(L_i) \to \Lambda(\bigoplus_{i \in I} L_i)
$$

est un isomorphisme du complexe $\bigotimes_{i \in I} K(u_i)$ (X, p. 63) sur le complexe $K(u)$.

En effet, d’après X, p. 64, remarque 4, la différentielle $D$ du complexe $\bigotimes_{i \in I} K(u_i)$ est une antidérivation ; les antidérivations $d_u$ et $g \circ D \circ g^{-1}$ de $\Lambda(\bigoplus L_i)$ coïncident sur $\bigoplus L_i$ avec l’application $x \mapsto u(x).1$ de $\bigoplus L_i$ dans $\Lambda(\bigoplus L_i)$, donc sont égales (III, p. 128, cor.).

Soient $C$ et $C'$ deux complexes de $A$-modules. On a (X, p. 63 et p. 99) des isomorphismes canoniques de complexes

$$
C \otimes_A (C' \otimes_A K(u)) \to (C \otimes_A C') \otimes_A K(u)
$$
$$
\mathrm{Homgr}_A(C', \mathrm{Homgr}_A(K(u), C)) \to \mathrm{Homgr}_A(C' \otimes_A K(u), C),
$$

c'est-à-dire des *isomorphismes*

(4) $$
C \otimes_A K^A(u, C') \to K^A(u, C \otimes_A C')
$$

(5) $$
\operatorname{Homgr}_A(C', K^i_A(u, C)) \to \operatorname{Homgr}_A(K^A(u, C'), C)
$$

Dans (4) et (5), prenons $C' = K(u')$, où $u' : L' \to A$ est une forme linéaire sur un $A$-module $L'$, et notons que $K^A(u, K(u'))$ qui est égal par définition à $K(u') \otimes_A K(u)$ s’identifie d’après la prop. 2 à $K(u' \oplus u)$ où $u' \oplus u : L' \oplus L \to A$ est la forme linéaire $(x', x) \mapsto u'(x') + u(x)$. On obtient alors des isomorphismes de complexes

(6) $$
K^A(u' \oplus u, C) \to K^A(u, K^A(u', C))
$$

(7) $$
K^i_A(u', K^i_A(u, C)) \to K^i_A(u' \oplus u, C)
$$

Par passage à l’homologie, on en déduit des isomorphismes de $A$-modules

$$
H^A_r(u' \oplus u, C) \to H^A_r(u, K^A(u', C)) , \qquad r \in \mathbf{Z} ,
$$
$$
H^r_A(u', K^i_A(u, C)) \to H^r_A(u' \oplus u, C) , \qquad r \in \mathbf{Z} .
$$

Notons enfin que l’homomorphisme déduit du produit dans l’algèbre $\Lambda(L)$

$$
m : K^A(u) \otimes_A K^A(u) \to K^A(u)
$$

est un morphisme de *complexes* (puisque $d_u$ est une antidérivation). Supposant $L$ *libre de rang n* et composant avec le morphisme de complexes $K^A(u) \to \Lambda^n L(-n)$ qui est l’identité en degré $n$, on en déduit un morphisme de complexes

$$
\chi : K^A(u) \otimes_A K^A(u) \to \Lambda^n L(-n) ;
$$

à ce morphisme correspond canoniquement, d’après X, p. 99, prop. 12, un morphisme de complexes

$$
\varphi : K^A(u) \to \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n))
$$

qui est *bijectif* (III, p. 87, formule (20)). Pour tout complexe $C$, on en déduit un isomorphisme composé

$$
K^A(u, C) = C \otimes_A K^A(u) \xrightarrow{1 \otimes \varphi} C \otimes \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n)) \to \\
\to \operatorname{Homgr}_A(K^A(u), C \otimes_A \Lambda^n L(-n)) = K^i_A(u, C \otimes_A \Lambda^n L(-n)) .
$$

Par passage à l’homologie, on a donc des isomorphismes *canoniques*

(8) $$
H^A_r(u, C) \to H^{n-r}_A(u, C \otimes_A \Lambda^n L) , \qquad r \in \mathbf{Z} .
$$

*Remarques. — 1)* \* Ce qui précède reste valable lorsque $L$ est projectif de rang $n$. \*

2) Puisque $L$ est libre de rang $n$, $\Lambda^n L$ est isomorphe à $A$, on a des isomorphismes non canoniques $H^A_r(u,C)\to H^{n-r}_A(u,C)$.

### 2. Fonctorialité

Soit $f:C\to C'$ un morphisme de complexes. On note

$$
K^A(u,f):K^A(u,C)\to K^A(u,C'),
$$

$$
K_A(u,f):K_A(u,C)\to K_A(u,C'),
$$

les morphismes de complexes $f\otimes 1_{K(u)}$ et $\operatorname{Hom}_{A}(1_{K(u)},f)$.

On note $H^A(u,f):H^A(u,C)\to H^A(u,C')$, $H_A(u,f):H_A(u,C)\to H_A(u,C')$,
$H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$, $H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$ les morphismes induits en homologie. L’application $f\mapsto K^A(u,f)$ est linéaire ; si $g:C'\to C''$ est un autre morphisme de complexes, on a $K^A(u,g\circ f)=K^A(u,g)\circ K^A(u,f)$; de même pour $K_A$, $H^A$, $H_A$, $H^A_r$, $H^A_r$.

Soit $0\to C'\xrightarrow{f}C\xrightarrow{g}C''\to0$ une suite exacte de complexes.

a) Supposons $L$ plat ; alors $\Lambda(L)$ est plat (X, p. 15, cor.). La suite

$$
0\to K^A(u,C')\xrightarrow{K^A(u,f)}K^A(u,C)\xrightarrow{K^A(u,g)}K^A(u,C'')\to0
$$

est alors exacte, et donne naissance (X, p. 30) à une suite exacte d’homologie

$$
\cdots\to H^A_n(u,C')\xrightarrow{H_n(u,f)}H^A_n(u,C)
\xrightarrow{H_n(u,g)}H^A_n(u,C'')
\xrightarrow{\partial_n}H^A_{n-1}(u,C')\to\cdots .
$$

b) Supposons $L$ projectif ; alors $\Lambda(L)$ est projectif. La suite

$$
0\to K_A(u,C')\xrightarrow{K_A(u,f)}K_A(u,C)
\xrightarrow{K_A(u,g)}K_A(u,C'')\to0
$$

est alors exacte, et donne naissance à une suite exacte d’homologie

$$
\cdots\to H^n_A(u,C')\xrightarrow{H^n(u,f)}H^n_A(u,C)
\xrightarrow{H^n(u,g)}H^n_A(u,C'')
\xrightarrow{\delta^n}H^{n+1}_A(u,C')\to\cdots .
$$

Soient $\rho:A\to A'$ un homomorphisme d’anneaux, $L'$ le $A'$-module $A'\otimes_A L$, $u':L'\to A'$ la forme linéaire $1\otimes u$. L’homomorphisme canonique bijectif (III, p. 83, prop. 8)

$$
\psi:\Lambda_{A'}(A'\otimes_A L)\to A'\otimes_A\Lambda_A(L)
$$

est un isomorphisme de complexes de $A'$-modules. On en déduit :

1) pour tout complexe de $A'$-modules $C'$, un isomorphisme de complexes de $A$-modules

$$
K^{A'}_{A}(u',C')\to K^A_A(u,C'),
$$

composé du diagramme

$$
C' \otimes_{A'} (\Lambda_A(A' \otimes_A L)) \xrightarrow{1_C \otimes \psi} C' \otimes_{A'} A' \otimes_A \Lambda_A(L) \to C' \otimes_A \Lambda_A(L)
$$

où $\varphi$ est la bijection canonique (III, p. 85, prop. 14);

2) pour tout complexe de $A$-modules $C$, un *isomorphisme* de complexes de $A'$-modules

$$
K^A(u, A' \otimes_A C) \to A' \otimes_A K^A(u, C),
$$

d'où des homomorphismes de $A'$-modules

$$
A' \otimes_A H_n^A(u, C) \to H_n^{A'}(u', A' \otimes_A C),
$$

qui sont bijectifs lorsque $A'$ est *plat* sur $A$ (X, p. 66, cor. 2).

Soient $L'$ un $A$-module, $u' : L' \to A$ une forme linéaire, $f : L \to L'$ un $A$-homomorphisme tel que $u' \circ f = u$. Il résulte de III, p. 161, formule (55), que l’homomorphisme $\Lambda(f) : \Lambda(L) \to \Lambda(L')$ satisfait à $d_u \circ \Lambda(f) = \Lambda(f) \circ d_{u'}$, donc définit un *morphisme de complexes* $\Lambda(u) : K^A(u) \to K^A(u')$. Si $C$ est un $A$-complexe, on en déduit des morphismes de complexes

$1_C \otimes \Lambda(u) : K^A(u, C) \to K^A(u', C)$ et $\mathrm{Homgr}(\Lambda(u), 1_C) : K_A^*(u', C) \to K_A^*(u, C)$.

Si $f$ est bijectif, tous ces morphismes sont des isomorphismes.

### 3. Exemple 1 : le complexe $S(L) \otimes_A \Lambda(L)$

Soient $A$ un anneau, $L$ un $A$-module, $S(L)$ son algèbre symétrique, $S(L) \otimes_A L$ le $S(L)$-module déduit par extension des scalaires, $u : S(L) \otimes_A L \to S(L)$ la forme linéaire telle que $u(s \otimes x) = sx$ pour $s \in S(L), x \in L$. Par l’isomorphisme canonique de $S(L)$-modules (III, p. 83, prop. 8)

$$
\Lambda_{S(L)}(S(L) \otimes_A L) \to S(L) \otimes_A \Lambda(L),
$$

la différentielle du complexe $K^{S(L)}(u)$ est transportée en l’application

$$
d : S(L) \otimes_A \Lambda(L) \to S(L) \otimes_A \Lambda(L)
$$

telle que, pour $x_1, ..., x_p, y_1, ..., y_q$ dans $L$, on ait

$$
\begin{align}
(9) \quad d((x_1 ... x_p) \otimes (y_1 \wedge ... \wedge y_q)) \\
&= \sum_{i=1}^q (-1)^{i+1} y_i x_1 ... x_p \otimes (y_1 \wedge ... \wedge y_{i-1} \wedge y_{i+1} \wedge ... \wedge y_q).
\end{align}
$$

Notons que $d$ applique $S^p(L) \otimes \Lambda^q(L)$ dans $S^{p+1}(L) \otimes \Lambda^{q-1}(L)$, donc que le *complexe de $A$-modules* $S(L) \otimes \Lambda(L)$ se décompose en la somme directe des complexes décrits par les diagrammes suivants :

$$
(\mathcal{E}_n) : 0 \to S^0 L \otimes_A \Lambda^n L \to S^1 L \otimes_A \Lambda^{n-1} L \to ... \to S^n L \otimes_A \Lambda^0 L \to 0, \quad n \in \mathbf{N}.
$$

Si le A-module L est somme directe d'une famille finie $(L_i)_{i \in I}$ où I est totalement ordonné, la bijection canonique

$$
\bigotimes_{i \in I} (\mathbf{S}(L_i) \otimes_A \Lambda(L_i)) \to \mathbf{S}(L) \otimes_A \Lambda(L)
$$

est un isomorphisme de complexes de A-modules (cela résulte de la prop. 2 de X, p. 148 ou de la formule (9) ci-dessus).

#### Proposition 3 {#alg-x-s9-prop-3 .statement}

*Si le A-module L est plat, les suites $(\mathcal{E}_n)$ ci-dessus sont exactes pour $n > 0$.*

*a)* Notons d'abord que, si $p_L$ est l'homomorphisme composé

$$
\mathbf{S}(L) \otimes \Lambda(L) \xrightarrow{\alpha} \mathbf{S}^0(L) \otimes \Lambda^0(L) \xrightarrow{\beta} A,
$$

où $\alpha$ est le produit tensoriel des projections canoniques et $\beta$ l'isomorphisme canonique, il s'agit de prouver que $H(p_L)$ est *bijectif*.

*b)* Si $L = 0$ ou si $L = A$, la proposition est évidente.

*c)* Supposons L libre de rang fini ; écrivons-le comme somme directe $L_1 \oplus ... \oplus L_n$ de A-modules libres de rang 1. D'après la remarque qui précède la proposition, le complexe $\mathbf{S}(L) \otimes \Lambda(L)$ est isomorphe au produit tensoriel des $n$ complexes *libres* $\mathbf{S}(L_i) \otimes \Lambda(L_i)$ dont d'après *b)* l'homologie est *libre*. D'après X, p. 79, cor. 4, l'homomorphisme canonique

$$
\gamma : \bigoplus_{i=1}^n H(\mathbf{S}(L_i) \otimes \Lambda(L_i)) \to H(\mathbf{S}(L) \otimes \Lambda(L))
$$

est bijectif. D'après *b)* $H(p_{L_i})$ est bijectif pour tout $i$. Comme $\bigotimes_{i=1}^n H(p_{L_i}) = H(p_L) \circ \gamma$,

$$
H(p_L) \text{ est bijectif}.
$$

*d)* Dans le cas général, L est limite inductive d'un système inductif filtrant $(L_i)_{i \in I}$ de modules libres de rang fini (X, p. 14, th. 1). Comme l'homomorphisme bijectif canonique

$$
\varprojlim \mathbf{S}(L_i) \otimes \Lambda(L_i) \to \mathbf{S}(L) \otimes \Lambda(L)
$$

est un isomorphisme de complexes, la proposition résulte de X, p. 28, prop. 1.

#### Remarque 1 {#alg-x-s9-n3-rem-1 .statement}

Nous verrons ci-dessous (X, p. 158, exemple) une autre démonstration de la partie *c)* ci-dessus.

#### Remarque 2 {#alg-x-s9-n3-rem-2 .statement}

Si A est une $\mathbf{Q}$-algèbre, la conclusion de la prop. 3 reste vraie sans hypothèse sur L (*cf.* X, p. 206, exercice 1).

#### Remarque 3 {#alg-x-s9-n3-rem-3 .statement}

Soient G un groupe et $\rho : G \to \mathbf{GL}(L)$ une représentation linéaire de G dans un A-module plat L. Alors les $(\mathcal{E}_n)$ sont des suites exactes de représentations linéaires. Supposons L projectif de type fini, et notons $R_A(G)$ l'anneau des représentations de G dans les A-modules projectifs de type fini. Il résulte de la prop. 3 que l’on a dans R_A(G) les relations

$$
\sum_{i=0}^{n} (-1)^i [\mathbf{S}^i(L)] [\Lambda^{n-i}(L)] = 0 , \quad n > 0 .
$$

Si on considère les séries formelles

$$
s(T) = \sum_{i=0}^{\infty} [\mathbf{S}^i(L)] T^i \in R_A(G)[[T]] ,
$$
$$
\lambda(T) = \sum_{i=0}^{\infty} [\Lambda^i(L)] T^i \in R_A(G)[[T]] ,
$$

les relations (10) s’écrivent

$$
s(T) \lambda(-T) = 1_* .
$$

### 4. Exemple 2 : le cas d’un module libre

Soient k un anneau, M un k-module, I un ensemble et p un entier $\geqslant 0$. Une application $m : I^p \to M$ est dite *alternée* si elle satisfait aux deux conditions suivantes :

a) pour toute permutation $\sigma \in S_p$ et toute suite $(\alpha_1, ..., \alpha_p) \in I^p$, on a

$$
m(\alpha_{\sigma(1)}, ..., \alpha_{\sigma(p)}) = \varepsilon_{\sigma} m(\alpha_1, ..., \alpha_p) ,
$$

b) pour toute suite $(\alpha_1, ..., \alpha_p) \in I^p$ telle que deux des indices $\alpha_1, ..., \alpha_p$ soient égaux, on a $m(\alpha_1, ..., \alpha_p) = 0$.
(Dans le cas où I est un k-module et m est multilinéaire, on retrouve la notion introduite en III, p. 80.)

*Supposons I fini* et notons $C_I^p(M)$ le k-module des applications alternées de $I^p$ dans M.

Soient $L_0$ un k-module, $(e_i)_{i \in I}$ une famille d’éléments de $L_0$; on définit deux applications k-linéaires

$$
g : \mathrm{Hom}_k (\Lambda^p L_0, M) \to C_I^p(M)
$$
$$
h : C_I^p(M) \to M \otimes_k \Lambda^p L_0
$$

comme suit : si $f \in \mathrm{Hom}_k (\Lambda^p L_0, M)$, on pose

$$
g(f)(\alpha_1, ..., \alpha_p) = f(e_{\alpha_1} \wedge ... \wedge e_{\alpha_p}) ;
$$

soit $m \in C_I^p(M)$, définissons $h(m) \in M \otimes_k \Lambda^p L_0$. Pour tout élément $(\alpha_1, ..., \alpha_p)$ de $I^p$, l’élément $m(\alpha_1, ..., \alpha_p) \otimes (e_{\alpha_1} \wedge ... \wedge e_{\alpha_p})$ de $\Lambda^p L_0 \otimes_k M$ est nul si $\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} < p$ et est indépendant de l’ordre des indices $\alpha_1, ..., \alpha_p$ si
$$
\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} = p .
$$
Il ne dépend que de la partie $J = (\alpha_1, ..., \alpha_p)$ de $I$; notons-le $h_J(m)$; on a $h_J(m) = 0$ si $\mathrm{Card}(J) < p$; on pose alors :
$$
h(m) = \sum_J h_J(m) ,
$$
où $J$ parcourt les parties de $I$ ayant $p$ éléments.

#### Lemme 2 {#alg-x-s9-lem-2 .statement}

*Si le k-module $L_0$ est libre de base $(e_i)_{i \in I}$, les applications k-linéaires g et h sont bijectives.*
Cela résulte de III, p. 79, th. 1.

Soient maintenant $M$ un $k$-module, et $x = (x_i)_{i \in I}$ une famille de $k$-endomorphismes de $M$, deux à deux permutables. Considérons l’anneau de polynômes $A = k[(X_i)_{i \in I}]$ et munissons $M$ de la structure de $A$-module telle que $P(X_i) m = P(x_i) m$ pour $P \in A$ et $m \in M$. Soient d’autre part $L$ le $A$-module libre $A^I$, $(e_i)_{i \in I}$ sa base canonique et $u : L \to A$ la forme linéaire qui applique $e_i$ sur $X_i$ pour tout $i \in I$. Considérons les complexes de $k$-modules $K_A^*(u, M)$ et $K_A^*(u, M)$; on a des *isomorphismes canoniques*
$$
K_A^p(u, M) = \mathrm{Hom}_A(\Lambda_A^p(A^I), M) \to \mathrm{Hom}_k(\Lambda_k^p(k^I), M) ,
$$
$$
M \otimes_k \Lambda_k^p(k^I) \to M \otimes_A \Lambda_A^p(A^I) = K_A^p(u, M) ;
$$
d’où par composition avec les isomorphismes $g$ et $h$ des *isomorphismes de k-modules*
$$
\theta^p : K_A^p(u, M) \to C_I^p(M) ,
$$
$$
\theta_p : C_I^p(M) \to K_A^p(u, M) .
$$
On note
$$
\partial^p : C_I^p(M) \to C_I^{p+1}(M) ,
$$
$$
\partial_p : C_I^p(M) \to C_I^{p-1}(M) ,
$$
les $k$-homomorphismes obtenus en transportant les différentielles de $K_A^*(u, M)$ et $K_A^*(u, M)$ par les isomorphismes $\theta$. On a par exemple :
(12) $$
(\partial^p m)(\alpha_1, ..., \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, ..., \alpha_{j-1}, \alpha_{j+1}, ..., \alpha_{p+1}) .
$$
Le complexe formé des $C_I^p(M)$ et des $\partial^p$ (resp. des $\partial_p$) se note $K^*(x, M)$ (resp. $K.(x, M)$) et s’appelle *le complexe de Koszul* ascendant (resp. descendant) associé au module M et à la suite d’endomorphismes $(x_1, ..., x_n)$. On a donc des isomorphismes de complexes de $k$-modules

$$
\theta^*: K_A^*(u, M) \to K^*(x, M),
$$
$$
\theta_*: K_*(x, M) \to K_A^*(u, M).
$$

#### Remarque {#alg-x-s9-n4-rem-1 .statement}

Inversement, soient B une $k$-algèbre, L un B-module libre de base $(e_i)_{i \in I}$, et M un B-module. La donnée d’une forme linéaire $u : L \to B$ équivaut à celle d’une famille $x = (x_i)_{i \in I}$ d’éléments de B, par la relation $x_i = u(e_i)$. Le complexe de $k$-modules sous-jacent à $K_B^*(u, M)$ (resp. $K^B(u, M)$) s’identifie alors, par l’isomorphisme $\theta^*$ (resp. $\theta_*$) au complexe de Koszul $K^*(x, M)$ (resp. $K_*(x, M)$). Par exemple $K^B(u)$ s’identifie à $K^*(x, B)$.

On introduit comme au n° 1 (X, p. 147) les notations $H_*(x, M)$, $H_*(x, M)$, etc., et tous les résultats des n°s 1 et 2 s’appliquent mutatis mutandis, le module $A^I$ étant libre. On a par exemple des isomorphismes

$$
H_0(x, M) \to M/(x) M
$$
$$
H^0(x, M) \to \operatorname{Hom}_A(A/(x), M),
$$

où $(x)$ désigne l’idéal $\sum A x_i$ de A. Par exemple aussi, si $K_*(x, A)$ est acyclique en degrés $> 0$, on a des isomorphismes

$$
H_r(x, M) \to \operatorname{Tor}_r^A(k, M),
$$
$$
\operatorname{Ext}_A^r(k, M) \to H^r(x, M).
$$

Enfin, supposons I (fini et) totalement ordonné, par exemple $I = \{ 1, ..., n \}$; identifions $\Lambda^n(A^I)$ à A grâce à l’élément de base $e_1 \wedge ... \wedge e_n$ et traduisons l’isomorphisme $K_p^A(u, M) \to K_A^{n-p}(u, M)$ de X, p. 149. Il devient, par transport par $(\theta_p)$ et $(\theta^{n-p})$, l’isomorphisme

$$
C_1^p(M) \to C_1^{n-p}(M)
$$

qui associe à $m \in C_1^p(M)$ l’élément $\tilde{m}$ de $C_1^{n-p}(M)$ tel que

$$
m(\alpha_1, ..., \alpha_p) = \tilde{m}(\beta_1, ..., \beta_{n-p})
$$

si $(\alpha_1, ..., \alpha_p, \beta_1, ..., \beta_{n-p})$ est une permutation *paire* de $\{ 1, ..., n \}$. Remarquons aussi que lorsque $I = \{ 1, ..., n \}$, on peut identifier $C_1^p(M)$ à l’ensemble des familles $m(\alpha_1, ..., \alpha_p)$ d’éléments de M où $\alpha_1 < \alpha_2 < ... < \alpha_p$; la formule (12) reste valable, ainsi que la relation (13).

#### Exemple {#alg-x-s9-n4-exa-1 .statement}

Prenons $M = k[T_1, ..., T_n]$; le complexe de Koszul $K (\partial/\partial T, M)$ associé à la suite d’endomorphismes $(\partial/\partial T_1, ..., \partial/\partial T_n)$ s’identifie au complexe de de Rham de $k[x_1, ..., x_n]$ sur $k$ (X, p. 44) : à $m \in C_{\{1,...,n\}}^p(M)$, on associe la forme différentielle

$$
\omega(m) = \sum_{\alpha_1 < ... < \alpha_p} m(\alpha_1, ..., \alpha_p)\ dx_{\alpha_1} \wedge ... \wedge dx_{\alpha_p},
$$

cf. formule (12) et exemple 1, p. 44.

### 5. Exemple 3 : le cas $L = A$

Si $L = A$, posons $u(1) = x \in A$. Le complexe $K(u)$ est alors de longueur 1, on a $K_0(u) = K_1(u) = A$ et $d_1(a) = xa$, donc pour tout $A$-module $M$, $K_0(u, M)$, $K_1(u, M)$, $K^0(u, M)$ et $K^1(u, M)$ s'identifient à $M$, les différentielles

$$
d_1 : K_1(u, M) \to K_0(u, M) \quad \text{et} \quad d^0 : K^0(u, M) \to K^1(u, M)
$$

étant $m \mapsto xm$. On a donc des isomorphismes

$$
H_0(x, M) \to A/xA \otimes_A M \leftarrow H^1(x, M),
$$
$$
H_1(x, M) \to \mathrm{Hom}_A(A/xA, M) \leftarrow H^0(x, M).
$$

#### Lemme 3 {#alg-x-s9-lem-3 .statement}

Soit $K$ un complexe tel que $K_i = 0$ pour $i \neq 0, 1$, et soient $C$ un complexe et $p$ un entier.

a) Si $K$ est plat, on a pour tout $p \in \mathbf{N}$ une suite exacte

$$
0 \to H_0(K \otimes_A H_p(C)) \to H_p(K \otimes_A C) \to H_1(K \otimes_A H_{p-1}(C)) \to 0.
$$

b) Si $K$ est projectif, on a pour tout $p \in \mathbf{N}$ une suite exacte

$$
0 \to H^1(\mathrm{Homgr}_A(K, H^{p-1}(C))) \to H^p(\mathrm{Homgr}_A(K, C))
$$
$$
\to H^0(\mathrm{Homgr}_A(K, H^p(C))) \to 0.
$$

Démontrons a), la démonstration de b) étant analogue. Pour tout $i$, notons $K_{(i)}$ le complexe $K_i(-i)$. On a une suite exacte de complexes, scindée comme suite de $A$-modules

$$
0 \to K_{(0)} \xrightarrow{\alpha} K \xrightarrow{\beta} K_{(1)} \to 0;
$$

la suite

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & K_{(0)} \otimes_A C & \xrightarrow{\alpha \otimes 1} & K \otimes_A C & \xrightarrow{\beta \otimes 1} & K_{(1)} \otimes_A C & \longrightarrow & 0
\end{array}
$$

est exacte, et $K$ étant plat, les homomorphismes

$$
\gamma_{0,p}(K_{(0)}, C) : K_{(0)} \otimes_A H_p(C) \to H_p(K_{(0)} \otimes_A C)
$$
$$
\gamma_{1,p-1}(K_{(1)}, C) : K_{(1)} \otimes_A H_{p-1}(C) \to H_p(K_{(1)} \otimes_A C)
$$

sont bijectifs (X, p. 66, cor. 2). Calculons l’homomorphisme de liaison $\partial(\alpha \otimes 1,\beta \otimes 1)$; par définition, il applique la classe du cycle $\sum a_i \otimes b_i$ sur celle de $\sum d a_i \otimes b_i$, ce qui signifie que

$$
\partial(\alpha \otimes 1,\beta \otimes 1)\circ\gamma(K_{(1)},\mathbf C)=\gamma(K_{(0)},\mathbf C)\circ(d_K\otimes 1).
$$

La suite exacte d’homologie associée à (14) prend donc la forme

$$
K_1\otimes H_p(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_p(\mathbf C)\longrightarrow H_p(K\otimes\mathbf C)
$$

$$
\hspace{7cm}\longrightarrow K_1\otimes H_{p-1}(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_{p-1}(\mathbf C),
$$

d’où a).

Appliquant le lemme 3, a) au complexe $K(u)$, et utilisant les isomorphismes de commutation, on obtient :

#### Proposition 4 {#alg-x-s9-prop-4 .statement}

*Pour tout complexe $C$, on a des suites exactes .*

$$
0\longrightarrow A/xA\otimes_A H_p(C)\longrightarrow H_p(x,C)\longrightarrow \operatorname{Hom}_A(A/xA,H_{p-1}(C))\longrightarrow 0.
$$

#### Corollaire 1 {#alg-x-s9-prop-4-cor-1 .statement}

*Pour que $H_p(x,C)=0$, il faut et il suffit que l’homothétie de rapport $x$ dans $H_p(C)$ soit surjective et que l’homothétie de rapport $x$ dans $H_{p-1}(C)$ soit injective.*

#### Corollaire 2 {#alg-x-s9-prop-4-cor-2 .statement}

*Soient $x=(x_1,\ldots,x_n)$ une suite d’éléments de $A$, $M$ un $A$-module, $x'$ la suite $(x_1,\ldots,x_{n-1})$. On a des suites exactes*

$$
0\longrightarrow A/x_nA\otimes_A H_p(x',M)\longrightarrow H_p(x,M)\longrightarrow \operatorname{Hom}_A(A/x_nA,H_{p-1}(x',M))\longrightarrow 0.
$$

#### Corollaire 3 {#alg-x-s9-prop-4-cor-3 .statement}

*Pour que $H_i(x,M)$ soit nul pour tout $i>0$, il faut et il suffit que l’homothétie de rapport $x_n$ dans $H_i(x',M)$ soit bijective pour $i>0$, et que l’homothétie de rapport $x_n$ dans $M/(x')M$ soit injective.*

### 6. Familles complètement sécantes

Soient $A$ un anneau, $M$ un $A$-module, $x=(x_i)_{i\in I}$ une famille d’éléments de $A$.

#### Définition 2 {#alg-x-s9-def-2 .statement}

*La famille $x$ est dite complètement sécante pour $M$ si on a $H_i(x,M)=0$ pour $i>0$.*

Si $I$ est fini, il revient au même (X, p. 150) de dire qu’on a $H^i(x,M)=0$ pour $i<\operatorname{Card}(I)$.

La proposition suivante permet de donner des exemples de familles complètement sécantes.

#### Proposition 5 {#alg-x-s9-prop-5 .statement}

*Soit $x=(x_1,\ldots,x_n)$ une suite d’éléments de $A$. Si pour $i=1,\ldots,n$, l’homothétie de rapport $x_i$ dans le $A$-module $M/(x_1M+\cdots+x_{i-1}M)$ est injective, la suite $x$ est complètement sécante pour $M$.*

Une suite vérifiant les conditions de la proposition est dite régulière pour M, ou M-régulière. On notera que cette propriété dépend en général de l’ordre des $x_i$; par exemple la suite $(1, 0)$ est toujours M-régulière, tandis que la suite $(0, 1)$ ne l’est que si M est nul. En revanche, le fait qu’une suite soit complètement sécante ne dépend pas de l’ordre des termes.

Démontrons la proposition par récurrence sur $n$, le cas $n = 0$ étant immédiat. Posons $x' = (x_1, ..., x_{n-1})$; si la suite $x$ est M-régulière, la suite $x'$ est M-régulière et la multiplication par $x_n$ dans $M/(x')M$ est injective; d’après l’hypothèse de récurrence, on a $H_i(x', M) = 0$ pour $i > 0$; il résulte alors du cor. 3 de X, p. 157, que $H_i(x, M) = 0$ pour $i > 0$.

#### Exemple {#alg-x-s9-n6-exa-1 .statement}

Soit $k$ un anneau; prenons $A = k[X_1, ..., X_n]$ et $x = (X_1, ..., X_n)$. La suite $x$ est A-régulière et la proposition redonne l’acyclicité en degrés $> 0$ du complexe $S_k(k^n) \otimes_k \Lambda_k(k^n)$ (cf. X, p. 152, prop. 3).
De même dans l’anneau de séries formelles $\hat{A} = k[[X_1, ..., X_n]]$, la suite $(X_1, ..., X_n)$ est $\hat{A}$-régulière, donc complètement sécante pour $\hat{A}$.

#### Proposition 6 {#alg-x-s9-prop-6 .statement}

a) Si $\sum_{i \in I} x_i A = A$, la famille $(x_i)_{i \in I}$ est complètement sécante pour M.
b) Soit $x = (x_1, ..., x_n)$ une suite d’éléments de A. Soit $(a_{ij}) \in \mathrm{GL}_n(A)$; posons
$$
y_i = \sum_j a_{ij} x_j.
$$
Si la suite $x$ est complètement sécante pour M, il en est de même de la suite $(y_1, ..., y_n)$.
c) Soient $k_1, ..., k_n$ des entiers $\geqslant 1$; pour que la suite $(x_1^{k_1}, ..., x_n^{k_n})$ soit complètement sécante pour M, il faut et il suffit que la suite $x$ soit complètement sécante pour M.
L’assertion a) résulte du cor. 1, p. 148.
Démontrons b). Soit $f : A^n \to A^n$ l’isomorphisme défini par la matrice $^t(a_{ij})$; il résulte de X, p. 151, que $1_M \otimes \Lambda(f)$ est un isomorphisme du complexe $K.(y, M)$ sur le complexe $K.(x, M)$, d’où b).
Pour démontrer c), il suffit évidemment de prouver que si $k$ est un entier $\geqslant 1$, la suite $(x_1, ..., x_{n-1}, x_n^k)$ est complètement sécante pour M si et seulement si il en est de même pour la suite $x$. Soit $x' = (x_1, ..., x_{n-1})$; d’après le cor. 3, p. 157, la première condition (resp. la seconde) signifie que l’homothétie de rapport $x_n^k$ (resp. $x_n$) est bijective dans $H_i(x', M)$ pour $i \geqslant 1$ et injective dans $M/(x')M$. Ces deux conditions sont clairement équivalentes, d’où c).

#### Remarque 1 {#alg-x-s9-n6-rem-1 .statement}

L’assertion analogue à c) pour les suites régulières est vraie (X, p. 207, exercice 5).

#### Proposition 7 {#alg-x-s9-prop-7 .statement}

a) Soit N un A-module plat. Si la famille x est complètement sécante pour M, elle l’est pour $M \otimes_A N$.

b) Soit $0 \to M' \to M \to M'' \to 0$ une suite exacte de $A$-modules. Si la famille $x$ est complètement sécante pour $M'$ et pour $M''$, elle l’est pour $M$.

Le complexe $K.(x, M \otimes_A N)$ est isomorphe par définition à $K.(x, M) \otimes_A N$; comme $N$ est plat, on en déduit un isomorphisme $H.(x, M) \otimes_A N \to H.(x, M \otimes_A N)$ (X, p. 66, cor. 2), d’où a).

Le complexe $K.(x)$ étant plat, on a une suite exacte de complexes

$$
0 \to K.(x, M') \to K.(x, M) \to K.(x, M'') \to 0 ;
$$

l’assertion b) résulte de la suite exacte d’homologie associée.

#### Remarque 2 {#alg-x-s9-n6-rem-2 .statement}

Les assertions analogues à a) et b) pour les suites régulières sont immédiates.

#### Remarque 3 {#alg-x-s9-n6-rem-3 .statement}

Si la famille $x$ est complètement secante pour $A$, le complexe $K.(x, A)$ définit une résolution libre du $A$-module $A/x$, avec $x = \sum_{i \in I} x_i A$; on a donc pour tout entier $i \geqslant 0$ et pour tout $A$-module $M$ des isomorphismes

$$
\text{Ext}_A^{n-i}(A/x, M) \to H^{n-i}(x, M) \to H_i(x, M) \to \operatorname{Tor}_i^A(A/x, M) .
$$

#### Remarque 4 {#alg-x-s9-n6-rem-4 .statement}

On dit que la suite $x = (x_1, ..., x_n)$ est $M$-corégulière si (notant $(x_i)_M$ l’homothétie de rapport $x_i$ dans $M$) l’homothétie de rapport $x_i$ dans le module

$$
\operatorname{Ker}(x_1)_M \cap ... \cap \operatorname{Ker}(x_{i-1})_M
$$

est surjective pour $i = 1, ..., n$. *On a alors* $H_i(x, M) = 0$ pour $i < n$: cela se démontre de la même manière que la prop. 5.

Prenons par exemple $A = k[D_1, ..., D_n]$, où $k$ est une $\mathbf{Q}$-algèbre, et $M = k[T_1, ..., T_n]$, muni de la structure de $A$-module telle que $D_i P = \partial P / \partial T_i$ pour tout $P \in M$ ($1 \leqslant i \leqslant n$). On vérifie aussitôt que la suite $(D_1, ..., D_n)$ est $M$-corégulière; compte tenu de l’exemple p. 155, on en déduit que *le complexe de de Rham de* $k[T_1, ..., T_n]$ *sur* $k$ *est acyclique en degrés* $> 0$.

### 7. Un critère pour les suites complètement sécante

Soient $A$ un anneau, $M$ un $A$-module, $x$ un idéal de $A$. On appelle *topologie* $x$*-adique* sur $M$ la topologie compatible avec la structure de groupe de $M$ pour laquelle l’ensemble des sous-modules $x^r M$ ($r \geqslant 0$) est un système fondamental de voisinages de zéro (TG, III, p. 5, exemple). Cette topologie est séparée si et seulement si

$$
\bigcap_{r \geqslant 0} x^r = 0 .
$$

Supposons maintenant que l’idéal $x$ soit engendré par une suite $x = (x_1, ..., x_n)$ d’éléments de A. Considérons le A-module gradué $\bigoplus_{r \geq 0} x^r M$ et le A-homomorphisme gradué de degré 0

$$
a_M^x : A[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} x^r M
$$

tel que $a_M^x(P \otimes m) = P(x_1, ..., x_n) m$ si P est un polynôme homogène en $X_1, ..., X_n$ et $m \in M$. Notons $\mathfrak{d}$ l’idéal de $A[X_1, ..., X_n]$ engendré par les éléments $(x_i X_j - x_j X_i)$ pour $1 \leq i < j \leq n$. On a $P(x_1, ..., x_n) = 0$ si $P \in \mathfrak{d}$, de sorte que $a_M^x$ donne par passage au quotient un A-homomorphisme gradué de degré 0

$$
\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M .
$$

Par produit tensoriel avec $A/x$, on déduit de $\alpha_M^x$ un A-homomorphisme gradué de degré 0

$$
\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M) .
$$

Les homomorphismes $a_M^x, \alpha_M^x$ et $\beta_M^x$ sont surjectifs.

#### Théorème 1 {#alg-x-s9-thm-1 .statement}

Considérons les conditions suivantes :
(i) La suite $x$ est M-régulière (X, p. 158).
(ii) La suite $x$ est complètement sécante pour M (X, p. 157, déf. 2).
(iii) On a $H_1(x, M) = 0$.
(iv) L’homomorphisme $\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M$ est bijectif.
(v) L’homomorphisme $\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M)$ est bijectif.

On a alors les implications (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) $\Leftrightarrow$ (iv) $\Rightarrow$ (v). Si pour $1 \leq i \leq n$ le A-module $M/(x_1 M + \cdots + x_{i-1} M)$ est séparé pour la topologie $x$-adique, les conditions (i) à (v) sont équivalentes.

Le théorème sera démontré aux nos 8 et 9.

*COROLLAIRE 1. — Si A est noethérien, si le A-module M est de type fini et si les $x_i$ appartiennent au radical de A, les conditions (i) à (v) du théorème sont équivalentes.
En effet, sur chacun des modules $M/(x_1 M + \cdots + x_{i-1} M)$ la topologie $x$-adique est séparée (AC III, § 3, no 3, prop. 6).

#### Corollaire 2 {#alg-x-s9-thm-1-cor-2 .statement}

Supposons que A soit un anneau gradué à degrés positifs, M un A-module gradué borné inférieurement, et les $x_i$ des éléments homogènes de degré > 0 de A. Alors les conditions (i) à (v) du théorème sont équivalentes.
La topologie $x$-adique est en effet séparée pour tout A-module gradué N borné inférieurement, puisque si $N_n = 0$ pour $n < n_0$ on a $x^a N \subset \sum_{j \geq n_0 + a} N_j$ pour tout $a \geq 0$.

#### Corollaire 3 {#alg-x-s9-thm-1-cor-3 .statement}

Supposons que les modules $M/(x_1M+\cdots+x_{i-1}M)$ soient séparés pour la topologie $\mathfrak{x}$-adique $(1\leq i\leq n)$ ; soit $p$ un entier compris entre $1$ et $n$. Pour que la suite $\mathfrak{x}$ soit complètement sécante pour $M$, il faut et il suffit que la suite $(x_1,\ldots,x_p)$ soit complètement sécante pour $M$ et que la suite $(x_{p+1},\ldots,x_n)$ soit complètement sécante pour $M/(x_1M+\cdots+x_pM)$.

En effet le corollaire est évident si on remplace dans l’énoncé « suites complètement sécantes » par « suites régulières » ; or les deux notions coïncident ici d’après le théorème.

#### Remarque {#alg-x-s9-n7-rem-1 .statement}

Soit $\mathfrak{x}=(x_1,\ldots,x_n)$ une suite d’éléments de $A$ telle que $H_1(\mathfrak{x},A)=0$ ; alors le noyau de l’homomorphisme surjectif $u:A^n\to\mathfrak{x}$ tel que
$$
u\left(\sum a_i e_i\right)=\sum a_i x_i
$$
est engendré par les éléments $X_j e_i-X_i e_j$ ; par conséquent, la $A$-algèbre $A[X_1,\ldots,X_n]/\mathfrak{d}$ est isomorphe à l’algèbre symétrique $S_A(\mathfrak{x})$ (III, p. 69, prop. 4). Il résulte donc du théorème 1 que l’homomorphisme d’algèbres
$$
S_A(\mathfrak{x})\longrightarrow\bigoplus_n \mathfrak{x}^n
$$
déduit de l’injection canonique de $\mathfrak{x}$ dans $\bigoplus_n\mathfrak{x}^n$ est un isomorphisme. Il en va de même pour l’homomorphisme
$$
S_A(\mathfrak{x}/\mathfrak{x}^2)\longrightarrow\bigoplus_n\mathfrak{x}^n/\mathfrak{x}^{n+1}.
$$

### 8. Démonstration du théorème 1 : première partie

L’implication (i) $\Rightarrow$ (ii) a déjà été démontrée (X, p. 157, prop. 5). L’implication (ii) $\Rightarrow$ (iii) est évidente ; il en est de même de (iv) $\Rightarrow$ (v), puisque $\beta_M^x$ s’identifie à $\alpha_M^x\otimes 1_{A/\mathfrak{x}}$.

Pour montrer que (iv) entraîne (iii), considérons l’homomorphisme $(\alpha_M^x)_1$ induit sur les composantes de degré 1. Notons $E$ le $A$-module gradué $A[X_1,\ldots,X_n]$ ; le $A$-module $E_1$ est libre de base $X_1,\ldots,X_n$ et $\mathfrak{d}_1$ est le sous-$A$-module de $E_1$ engendré par les éléments $(x_iX_j-x_jX_i)$ pour $1\leq i<j\leq n$. Par suite $((E/\mathfrak{d})\otimes_A M)_1$ s’identifie à $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$, l’homomorphisme $(\alpha_M^x)_1$ s’identifiant à l’application de $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$ sur $B_0(K_\bullet(\mathfrak{x},M))$ induite par $d_1$. Ainsi la nullité de $H_1(\mathfrak{x},M)$ est équivalente à l’injectivité de $(\alpha_M^x)_1$, d’où l’implication (iv) $\Rightarrow$ (iii).

Pour démontrer que (iii) entraîne (iv), nous utiliserons le lemme suivant :

#### Lemme 4 {#alg-x-s9-lem-4 .statement}

Soit $A_0$ l’anneau $\mathbf{Z}[T_1,\ldots,T_n]$, et soit $u:A_0[X_1,\ldots,X_n]\to A_0[U]$ l’homomorphisme de $A_0$-algèbres tel que $u(X_i)=T_iU$. Le noyau de $u$ est l’idéal $\mathfrak{d}_0$ de $A_0[X_1,\ldots,X_n]$ engendré par les éléments $(T_iX_j-T_jX_i)$ pour $1\leq i<j\leq n$. Si $t$ est l’idéal de $A_0$ engendré par $(T_1,\ldots,T_n)$, $u$ induit un isomorphisme
$$
\bar{u}:A_0[X_1,\ldots,X_n]/\mathfrak{d}_0\longrightarrow\bigoplus_{r\geq0}t^r.
$$

Il suffit évidemment de démontrer la première assertion. Pour toute suite d’entiers naturels $\alpha=(\alpha_1,\ldots,\alpha_n)$ et tout entier $k\in[0,n]$, notons $P_{\alpha,k}$ le monôme
$$
T_1^{\alpha_1}\cdots T_k^{\alpha_k}X_{k+1}^{\alpha_{k+1}}\cdots X_n^{\alpha_n};
$$

soit $N$ le sous-$\mathbf{Z}$-module de $A_0[X_1, ..., X_n]$ engendré par les $P_{\alpha, k}$ pour $\alpha \in \mathbf{N}^n$ et $0 \leq k \leq n$. Nous allons montrer que la restriction de $u$ à $N$ est injective et que $A_0[X_1, ..., X_n] = \mathfrak{d}_0 + N$; comme on a $\mathfrak{d}_0 \subset \mathrm{Ker}\,u$, cela entraînera le lemme.

Observons que $N$ est engendré par l’ensemble $S$ formé de $P_{0,0} = 1$ et de ceux des $P_{\alpha, k}$ pour lesquels $\alpha_k \neq 0$. Pour prouver l’injectivité de la restriction de $u$ à $N$, il suffit de montrer que deux éléments distincts de $S$ ont pour image par $u$ des monômes distincts dans $A_0[U]$. Or on a $u(P_{\alpha, k}) = T^\alpha U^{\sum \alpha_i}_{i \geq k}$, de sorte que l’égalité $u(P_{\alpha, k}) = u(P_{\alpha', k'})$ entraîne $\alpha = \alpha'$ et $\sum_{i \geq k} \alpha_i = \sum_{i \geq k'} \alpha_i$. Supposons que $P_{\alpha, k}$ et $P_{\alpha', k'}$ appartiennent à $S$. Si $\alpha = 0$, on a alors $k = k' = 0$; si $\alpha \neq 0$, on obtient $k = k'$ puisque $\alpha_k$ et $\alpha_{k'}$ sont différents de zéro, d’où le résultat.

Montrons que tout monôme $T^\alpha X^\beta \in A_0[X_1, ..., X_n]$ est congru modulo $\mathfrak{d}_0$ à un $P_{\eta, k}$. Pour toute suite $\lambda \in \mathbf{N}^n$, on notera $i(\lambda)$ (resp. $j(\lambda)$) le plus petit (resp. le plus grand) entier $k \in [1, n]$ tel que $\lambda_k \neq 0$. Dans l’ensemble des monômes $T^\gamma X^\delta$ qui sont congrus à $T^\alpha X^\beta$ modulo $\mathfrak{d}_0$, choisissons-en un pour lequel l’entier rationnel $j(\gamma) - i(\delta)$ soit minimum ; montrons qu’on a alors $j(\gamma) - i(\delta) < 0$. Supposons qu’on ait $j(\gamma) \geq i(\delta)$; notons $j = j(\gamma), i = i(\delta)$, et soit $\varepsilon = \inf (\gamma_j, \delta_i)$. Comme $(T_j^\varepsilon X_i^\varepsilon - T_i^\varepsilon X_j^\varepsilon)$ est divisible par $(T_j X_i - T_i X_j)$, donc appartient à $\mathfrak{d}_0$, on voit que $T^\gamma X^\delta$ est congru modulo $\mathfrak{d}_0$ à $T^{\gamma'} X^{\delta'}$, où $\gamma'_i = \gamma_i + \varepsilon, \gamma'_j = \gamma_j - \varepsilon, \gamma'_k = \gamma_k$ pour $k \neq i, j$, et $\delta'_i = \delta_i - \varepsilon, \delta'_j = \delta_j + \varepsilon, \delta'_k = \delta_k$ pour $k \neq i, j$. Comme $\gamma'_j$ ou $\delta'_i$ est nul, on a $j(\gamma') - i(\delta') < j(\gamma) - i(\delta)$ ce qui contredit le caractère minimal de $j(\gamma) - i(\delta)$.

Par conséquent on a $j(\gamma) < i(\delta)$, d’où $T^\gamma X^\delta \in N$, ce qui achève de prouver le lemme.

Démontrons que (iii) implique (iv). Considérons l’anneau $A_0 = \mathbf{Z}[T_1, ..., T_n]$ et l’idéal t de $A_0$ engendré par $T_1, ..., T_n$. Munissons $M$ de la structure de $A_0$-module pour laquelle $T_i m = x_i m$ pour $m \in M, 1 \leq i \leq n$. D’après X, p. 155, $H_i(x, M)$ s’identifie canoniquement à $H_i(T, M)$.

Comme la suite $T$ est régulière pour $A_0$, il résulte de l’implication (i) $\Rightarrow$ (ii) que le complexe $K.(T, A_0)$ définit une résolution libre du $A_0$-module $A_0/t$. Remarquons que celui-ci s’identifie à $\mathbf{Z}$, muni de la structure de $A_0$-module telle que $T_i \mathbf{Z} = 0$ pour $1 \leq i \leq n$. Ainsi la condition (iii) est équivalente à $\mathrm{Tor}_1^{A_0}(M, \mathbf{Z}) = 0$.

Montrons que (iii) entraîne $\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0$ pour tout $r \geq 1$. Cela résulte de ce qui précède pour $r = 1$. Dans le cas général, considérons la suite exacte

$$
0 \to t^r/t^{r+1} \to A_0/t^{r+1} \to A_0/t^r \to 0,
$$

Le $A_0$-module $t^r/t^{r+1}$ est isomorphe à un produit fini d’exemplaires de $\mathbf{Z}$; on a donc $\mathrm{Tor}_1^{A_0}(M, t^r/t^{r+1}) = 0$. On en déduit, par récurrence sur $r$, que

$$
\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0 \quad \text{pour tout } r,
$$

La suite exacte (16) fournit donc, par produit tensoriel avec $M$, une suite exacte

$$
0 \to (t^r/t^{r+1}) \otimes_{A_0} M \to M/x^{r+1} M \to M/x^r M \to 0
$$

d'où un isomorphisme de $(t'/{t'}^{r+1}) \otimes_{A_0} M$ sur $x' M/{x'}^{r+1} M$. En considérant la suite exacte $0 \to {t'}^{r+1} \to t' \to t'/{t'}^{r+1} \to 0$, on voit alors par récurrence sur $r$ que l’application $m_r : t' \otimes_{A_0} M \to x' M$, induite par l’opération de $A_0$ dans $M$, est un isomorphisme.

Pour démontrer (iv), il reste à observer que le diagramme

$$
\begin{array}{ccc}
(A_0[X_1, ..., X_n]/\mathcal{D}_0) \otimes_{A_0} M & \xrightarrow{\bar{u} \otimes 1_M} & \bigoplus_{r \geq 0} (t' \otimes_{A_0} M) \\
\downarrow e & & \downarrow \oplus m_r \\
(A[X_1, ..., X_n]/\mathcal{D}) \otimes_A M & \xrightarrow{\alpha_M^x} & \bigoplus_{r \geq 0} x' M
\end{array}
$$

où $e$ est l’isomorphisme canonique d’extension des scalaires (II, p. 85, prop. 6), est commutatif, et à appliquer le lemme 4.

### 9. Démonstration du théorème 1 : deuxième partie

Considérons de nouveau la suite exacte

(16)
$$
0 \longrightarrow t'/{t'}^{r+1} \xrightarrow{i_r} A_0/{t'}^{r+1} \xrightarrow{p_r} A_0/t' \longrightarrow 0
$$

et la suite exacte de modules de torsion associée

(18)
$$
\begin{array}{cccccc}
\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(A_0/t', M) \\
\longrightarrow (t'/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{i_r \otimes 1_M} & (A_0/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{p_r \otimes 1_M} & (A_0/t') \otimes_{A_0} M & \longrightarrow 0 .
\end{array}
$$

Le noyau de $p_r \otimes 1_M$ s’identifie à $x' M/{x'}^{r+1} M$; par ailleurs $t'/{t'}^{r+1}$ est annulé par les $T_i$ et s’identifie au composant homogène de degré $r$ de $A_0$, de sorte que l’homomorphisme $(t'/{t'}^{r+1}) \otimes_{A_0} M \to x' M/{x'}^{r+1} M$ déduit de $i_r \otimes 1_M$ s’identifie à la composante homogène de degré $r$ de l’homomorphisme $\beta_M^x$. Il résulte donc de la suite exacte (18) que la condition (v) est équivalente à

(v') : *l’homomorphisme* $\mathrm{Tor}_1^{A_0}(p_r, 1_M)$ : $\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) \to \mathrm{Tor}_1^{A_0}(A_0/t', M)$ *est surjectif pour tout* $r \geq 1$.

Il nous reste à prouver l’implication (v) $\Rightarrow$ (i) lorsque les modules
$$
M/(x_1 M + \cdots + x_{i-1} M)
$$
sont séparés pour la topologie $x$-adique ($1 \leq i \leq n$). Notons $\overline{M}$ le $A$-module $M/x_1 M$. Par définition, la suite $x$ est régulière pour $M$ si et seulement si $(x_1)_M$ est injectif et la suite $x' = (x_2, ..., x_n)$ est régulière pour $\overline{M}$. Raisonnant par récurrence sur $n$, il suffit donc de prouver que, si $M$ est séparé pour la topologie $x$-adique et si $\beta_M^x$ est bijectif, alors $(x_1)_M$ est injectif et $\beta_M^{x'}$ est bijectif. Or la bijectivité de $\beta_M^x$ implique en particulier que l’homothétie de rapport $x_1$ dans $\bigoplus r x' M/{x'}^{r+1} M$ est injective, donc que $\mathrm{Ker}\,(x_1)_M \subset \bigcap_i x^i M$ et par conséquent que $(x_1)_M$ est injectif si la topologie $x$-adique sur $M$ est séparée.

On est ainsi ramené à démontrer que si $(x_1)_M$ est injectif et si $M$ vérifie la condition (v'), alors $\overline{M}$ vérifie la condition (v') relativement à la suite $x'$.

On a par hypothèse une suite exacte
$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0;
$$
posons $\overline{A}_0 = A_0 / T_1 A_0,\ \overline{t} = t \overline{A}_0$. Soit $q : L \to M$ une résolution libre du $A_0$-module $M$; comme l’homothétie de rapport $T_1$ est injective dans $A_0$, elle est injective dans $L$, et on a une suite exacte de complexes
$$
0 \longrightarrow L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0
$$
avec $\overline{L} = L / x_1 L$, et un diagramme commutatif
$$
\begin{array}{ccc}
0 & \longrightarrow & L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0 \\
   &                & \downarrow q        \downarrow q        \downarrow \overline{q} \\
0 & \longrightarrow & M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0 .
\end{array}
$$

Comme $q$ est un homologisme, $\overline{q} : \overline{L} \to \overline{M}$ est une résolution libre du $\overline{A}_0$-module $\overline{M}$ (cor. 1, p. 30). Pour tout $\overline{A}_0$-module $P$, on a un isomorphisme canonique
$$
P \otimes_{A_0} L \to P \otimes_{\overline{A}_0} \overline{L},
$$
d’où par passage à l’homologie un isomorphisme
$$
\varphi_P : \mathrm{Tor}_1^{A_0}(P, M) \to \mathrm{Tor}_1^{\overline{A}_0}(P, \overline{M}) .
$$
Si $u : P \to P'$ est un $\overline{A}$-homomorphisme, alors
$$
\varphi_{P'} \circ \mathrm{Tor}_1^{A_0}(u, 1_M) = \mathrm{Tor}_1^{\overline{A}_0}(u, 1_M) \circ \varphi_P .
$$
Cela étant, supposons la condition (v') vérifiée pour $M$, et démontrons qu’elle est vraie pour $\overline{M}$. Soit $r$ un entier $\geqslant 1$; on a un diagramme commutatif à lignes exactes
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & A_0 / t^r & \xrightarrow{T_1} & A_0 / t^{r+1} & \longrightarrow & \overline{A}_0 / \overline{t}^{r+1} & \longrightarrow & 0 \\
   &                  & \downarrow p_{r-1} &           & \downarrow p_r &           & \downarrow \overline{p}_r &           & \\
0 & \longrightarrow & A_0 / t^{r-1} & \xrightarrow{T_1} & A_0 / t^r & \longrightarrow & \overline{A}_0 / \overline{t}^r & \longrightarrow & 0
\end{array}
$$
d’où l’on déduit un diagramme commutatif à lignes exactes
$$
\begin{array}{ccccccccccc}
\mathrm{Tor}_1^{A_0}(A_0 / t^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^{r+1}, M) & \longrightarrow & M / x^r M & \xrightarrow{x_1} & M / x^{r+1} M \\
\mathrm{Tor}_1(p_{r, r'}) & \downarrow & \mathrm{Tor}_1(\overline{p}_{r, 1}) & \downarrow & & & \downarrow \\
\mathrm{Tor}_1(A_0 / t^r, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^r, M) & \longrightarrow & M / x^{r-1} M & \xrightarrow{x_1} & M / x^r M .
\end{array}
$$
Or la multiplication par $x_1$ définit une injection de $M / x^r M$ dans $M / x^{r+1} M$: cela résulte aussitôt, par récurrence sur $r$, de la suite exacte
$$
0 \to x^{r-1} M / x^r M \to M / x^r M \to M / x^{r-1} M \to 0
$$

et de l’injectivité de l’homothétie de rapport $x_1$ dans $\bigoplus_{r \geq 0} (x^r M / x^{r+1} M)$. La condition (v) entraîne donc que l’homomorphisme $\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M)$ est surjectif pour tout $r \geq 1$. Par composition avec les isomorphismes $(\varphi_{\overline{A}_0/\overline{t}^{r+1}})^{-1}$ et $\varphi_{\overline{A}_0/\overline{t}^r}$, on en déduit que l’homomorphisme

$$
\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M) : \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^{r+1}, M) \to \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^r, M)
$$

est surjectif pour $r \geq 1$, d’où la condition (v’) pour $\overline{M}$. Ceci achève la démonstration du théorème.

### 10. Classe d’extensions associée à une suite régulière

Soient $A$ un anneau, $M$ un $A$-module, $x = (x_1, ..., x_n)$ une suite d’éléments de $A$. Notons $M_i$ le $A$-module $M / (x_1 M + \cdots + x_{i-1} M)$ pour $i = 0, ..., n+1$, de sorte que $M_0$ et $M_1$ s’identifient à $M$ et que $M_{n+1} = M / (x) M$. Notons

$$
\overline{x}_i : M_{i-1} \to M_i , \quad i = 1, ..., n ,
$$

le $A$-homomorphisme composé de l’homothétie de $M_{i-1}$ de rapport $x_i$ et de la projection canonique de $M_{i-1}$ sur $M_i$. Notons enfin $p : M_n \to M / (x) M$ la projection canonique. Le diagramme

(19)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_n} M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

est une suite exacte si et seulement si la suite $x$ est $M$-régulière. Supposons désormais la suite $x$ régulière pour $M$. L’élément $\theta_x \in \operatorname{Ext}_A^n (M / (x) M, M)$ associé à la suite exacte (19) est aussi dit associé à la suite $M$-régulière $x$.

Soit $i$ un entier, $1 \leq i \leq n$. Notons que la suite (19) peut se décomposer en les deux suites exactes

(20)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_i} M_i \longrightarrow M / (x_1 M + \cdots + x_i M) \longrightarrow 0
$$

(21)

$$
0 \longrightarrow M / (x_1 M + \cdots + x_i M) \xrightarrow{\overline{x}_{i+1}} M_{i+1} \longrightarrow \cdots \longrightarrow M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

qui ne sont autres que les suites exactes associées à la suite $(x_1, ..., x_i)$ qui est régulière pour $M$ et à la suite $(x_{i+1}, ..., x_n)$ qui est régulière pour $M / (x_1 M + \cdots + x_i M)$. Notant

$$
\theta_{(x_1, ..., x_i)} \in \operatorname{Ext}_A^i (M / (x_1 M + \cdots + x_i M), M)
$$
$$
\theta_{(x_{i+1}, ..., x_n)} \in \operatorname{Ext}_A^{n-i} (M / (x) M, M / (x_1 M + \cdots + x_i M)) ,
$$

les classes d’extensions associées à (20) et (21), on a d’après X, p. 118, prop. 3

(22)
$$
\theta_{(x_1, \ldots, x_n)} = \theta_{(x_1, \ldots, x_i)} \circ \theta_{(x_{i+1}, \ldots, x_n)} .
$$

Par ailleurs, d’après la prop. 5 (X, p. 157), le complexe de Koszul $\mathbf{K}.(x, M)$ est acyclique en degrés $\neq n$, d’où une suite exacte

(23)
$$
0 \longrightarrow M \xrightarrow{\partial^0} \mathbf{K}^1(x, M) \xrightarrow{\partial^1} \mathbf{K}^2(x, M) \xrightarrow{\partial^2} \cdots \longrightarrow \mathbf{K}^n(x, M) \xrightarrow{q} M/(x)M \longrightarrow 0 ,
$$
où on a identifié $\mathbf{K}^0(x, M)$ à $M$ et où $q$ applique chaque élément $m \in \mathbf{K}^n(x, M)$ sur la classe dans $M/(x)M$ de $m(1, 2, \ldots, n) \in M$.

#### Proposition 8 {#alg-x-s9-prop-8 .statement}

*Supposons la suite x régulière pour M. L’élément de $\mathrm{Ext}_A^n(M/(x)M, M)$ associé à la suite exacte (23) est $(-1)^{n(n+1)/2} \theta_x$.*
Pour $i = 0, 1, \ldots, n$, définissons une application A-linéaire
$$
a^i : \mathbf{K}^i(x, M) \to M_i = M/(x_1 M + \cdots + x_{i-1} M)
$$
comme suit : si $m \in \mathbf{K}^i(x, M)$, $a^i(m)$ est la classe dans $M_i$ de l’élément $m(1, 2, \ldots, i)$ de $M$. Il est clair que $a^0$ est l’application identique de $M$ et que $p \circ a^n = q$. Par ailleurs $a^{i+1} \circ \partial^i(m)$ est l’image dans $M_{i+1}$ de l’élément
$$
\sum_{k=1}^{i+1} (-1)^{k+1} x_k m(1, 2, \ldots, k-1, k+1, \ldots, i+1) .
$$
Comme $x_k$ annule $M_{i+1}$ pour $k = 1, \ldots, i$, $a^{i+1} \circ \partial^i(m)$ est aussi l’image de
$$
(-1)^i x_{i+1} m(1, 2, \ldots, i) ,
$$
donc
$$
a^{i+1} \circ \partial^i = (-1)^i \overline{x}_{i+1} \circ a^i .
$$
D’après X, p. 120, cor. 1 et 2, l’élément de $\mathrm{Ext}_A^n(M/(x)M, M)$ associé à (23) est égal à $\prod_{i=1}^n (-1)^i \cdot \theta_x$, d’où l’assertion.

#### Corollaire {#alg-x-s9-n10-cor-1 .statement}

*Supposons de plus les modules $M/(x_1 M + \cdots + x_{i-1} M)$ séparés pour la topologie (x)-adique, et soit $(a_{ij}) \in \mathrm{GL}_n(A)$. Posons*
$$
y_i = \sum_j a_{ij} x_j \quad \text{et} \quad y = (y_1, \ldots, y_n) .
$$
*Alors la suite y est régulière pour M, et on a $\theta_y = \det(a_{ij})^{-1} \theta_x$.*
En effet, la suite y est régulière pour M d’après la prop. 6 (X, p. 158) et le théorème 1 (X, p. 160) ; la dernière assertion résulte de la prop. 8, et de la prop. 4 de X, p. 119.

#### Proposition 9 {#alg-x-s9-prop-9 .statement}

*Supposons la suite x régulière pour M. Si N est un A-module tel que $(x)N = 0$, on a $\mathrm{Ext}_A^i(N, M) = 0$ pour $i < n$, et l’application $\alpha \mapsto \theta_x \circ \alpha$* de Hom_A (N, M/(x) M) dans Ext^n_A (N, M) (qui est aussi l’homomorphisme de liaison itéré associé à (19), cf. X, p. 127, cor. 3) est bijective.

Il s’agit de prouver que l’homomorphisme $\psi^i : \alpha \mapsto \theta_x \circ \alpha$ de $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ dans $\mathrm{Ext}_A^i(N, M)$ est bijectif pour $i \leq n$. Raisonnons par récurrence sur $n$, l’assertion étant triviale pour $n = 0$. Posons $M_1 = M/x_1 M$, $x' = (x_2, ..., x_n)$, de sorte que $x'$ est $M_1$-régulière. D’après l’hypothèse de récurrence, l’homomorphisme

$$
\overline{\psi}^{i-1} : \alpha \mapsto \theta_{x'} \circ \alpha
$$

de $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ dans $\mathrm{Ext}_A^{i-1}(N, M_1)$ est bijectif pour $i < n$. Par ailleurs, considérons la suite exacte

$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow M_1 \longrightarrow 0 ;
$$

l’homomorphisme de liaison $\mathrm{Ext}_A^i(N, M_1) \to \mathrm{Ext}_A^{i+1}(N, M)$ associé est $\varphi^i : \beta \mapsto \theta_{x_1} \circ \beta$ (X, p. 125, prop. 5) ;

comme on a $\mathrm{Ext}^i(1_N, (x_1)_M) = \mathrm{Ext}^i((x_1)_N, 1_M) = 0$, on en déduit des suites exactes

$$
0 \longrightarrow \mathrm{Ext}_A^i(N, M) \longrightarrow \mathrm{Ext}_A^i(N, M_1) \xrightarrow{\varphi^i} \mathrm{Ext}_A^{i+1}(N, M) \longrightarrow 0 .
$$

Comme $\mathrm{Ext}_A^i(N, M_1) = 0$ pour $i < n - 1$, on en déduit que $\mathrm{Ext}_A^{i+1}(N, M) = 0$ pour $i < n - 1$, c’est-à-dire $i + 1 < n$; il s’ensuit que $\varphi^i$ est bijectif pour $i < n$. Comme $\psi^i(\alpha) = \theta_x \circ \alpha = \theta_{x_1} \circ \theta_{x'} \circ \alpha = \varphi^{i-1} \circ \overline{\psi}^i(\alpha)$ pour $\alpha \in \mathrm{Ext}_A^{i-n}(N, M/(x) M)$, $\psi^i$ est bien bijectif pour $i \leq n$.

EXERCICES

## EXERCICES {#alg-x-s9-exercises}

See the [exercises for § 9](exercises/s9/).
