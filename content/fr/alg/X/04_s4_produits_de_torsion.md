---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 4
section_title: Produits de torsion
lang: fr
source: alg-x-fr
book_pages: A X.61-A X.81, A X.184-A X.186
pdf_pages: 0067-0087, 0190-0192
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel de deux complexes
      page: 61
      pdf_page: 67
    - "no": 2
      title: Produits tensoriels et homotopie
      page: 64
      pdf_page: 70
    - "no": 3
      title: Produit tensoriel par un complexe plat borné à droite
      page: 66
      pdf_page: 72
    - "no": 4
      title: Définition et premières propriétés du produit de torsion
      page: 67
      pdf_page: 73
    - "no": 5
      title: Les homomorphismes de liaison et les suites exactes
      page: 71
      pdf_page: 77
    - "no": 6
      title: Modules plats et produits de torsion
      page: 74
      pdf_page: 80
    - "no": 7
      title: ' **Formule de Künneth**'
      page: 76
      pdf_page: 82
    - "no": 8
      title: Complexes bornés et plats sur un anneau noethérien
      page: 79
      pdf_page: 85
    - "no": 9
      title: Généralisation aux complexes de multimodules
      page: 80
      pdf_page: 86
statements: 39
exercises: 9
content_sha256: 0dd07ce8e9ce8109b1e39864b92a50b62e2990891ab5bf56dbf260ccfcff8d83
---

## § 4. PRODUIT DE TORSION

*Dans les paragraphes 4 à 8, on dénote par $k$ un anneau commutatif, et par $A$ une $k$-algèbre associative et unifère. Le rôle de $k$ est de nature auxiliaire ; on a en vue principalement les trois cas particuliers suivants :*

a) on considère un anneau quelconque $A$, on pose $k=\mathbf{Z}$ et on munit $A$ de sa structure naturelle de $\mathbf{Z}$-algèbre,

b) on considère un anneau quelconque $A$, on prend pour $k$ le centre de $A$,

c) on considère un anneau commutatif $A$ et on prend $k=A$.

### 1. Produit tensoriel de deux complexes

Soient $(C,d)$ un complexe de $A$-modules à droite et $(C',d')$ un complexe de $A$-modules à gauche.

Munissons le $k$-module $C\otimes_A C'$ de la graduation telle que

$$
(C\otimes_A C')_n=\sum_{p+q=n}(C_p\otimes C'_q)
$$

et notons $D$ l’unique endomorphisme $k$-linéaire de degré $(-1)$ de $C\otimes_A C'$ tel que

$$
\tag{1}
D(x\otimes x')=dx\otimes x'+(-1)^p x\otimes d'x',
\qquad x\in C_p,\ y\in C'_q,\ p,\ q\in\mathbf{Z}.
$$

On a $D\circ D=0$ puisque, avec les notations de (1)

$$
D^2(x\otimes x')=ddx\otimes x'+(-1)^{p-1}dx\otimes d'x'+(-1)^pdx\otimes d'x'-x\otimes d'd'x'.
$$

Le complexe de $k$-modules $(C\otimes_A C',D)$ est appelé le *complexe produit tensoriel* des complexes $(C,d)$ et $(C',d')$.

#### Remarque 1 {#alg-x-s4-n1-rem-1 .statement}

Lorsque $C'$ est réduit à $C'_0=M$, alors $(C\otimes_A C')_n=C_n\otimes_A M$ et $D=d\otimes 1_M$; par exemple $C\otimes_A A_s$ s’identifie naturellement à $C$. De même, lorsque $C$ est réduit à $C_0=P$, alors $(C\otimes_A C')_n=P\otimes_A C'_n$ et $D=1_P\otimes d$.

#### Remarque 2 {#alg-x-s4-n1-rem-2 .statement}

Pour tout entier $r$, on a $(C\otimes_A C')(r)=C(r)\otimes_A C'$, mais $(C\otimes_A C')(r)$ et $C\otimes_A C'(r)$ n’ont pas en général la même différentielle.

Soient $p, q$ deux entiers, $x \in Z_p(C), x' \in Z_q(C')$; alors l’élément $x \otimes x'$ de $C_p \otimes C'_q$ appartient à $Z_{p+q}(C \otimes C')$ d’après (1); de plus, si $y \in C_{p+1}, y' \in C'_{q+1}$, on a
$$
(x + dy) \otimes (x' + d'y') = x \otimes x' + D(y \otimes x' + (-1)^p (x + dy) \otimes y');
$$
par passage aux quotients, on en déduit une application $k$-linéaire, dite canonique
$$
\gamma_{p,q}(C, C') : H_p(C) \otimes_A H_q(C') \to H_{p+q}(C \otimes_A C');
$$
si on munit $H(C) \otimes_A H(C')$ de la graduation telle que
$$
(H(C) \otimes H(C'))_n = \sum_{p+q=n} H_p(C) \otimes_A H_q(C'),
$$
les $\gamma_{p,q}$ définissent une application $k$-linéaire graduée de degré 0
$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C').
$$
La prop. 6 de II, p. 59, se reformule ainsi :

#### Proposition 1 {#alg-x-s4-prop-1 .statement}

*Si les complexes $C$ et $C'$ sont nuls à droite, $C \otimes_A C'$ est nul à droite et l’application $k$-linéaire canonique*
$$
\gamma_{0,0}(C, C') : H_0(C) \otimes_A H_0(C') \to H_0(C \otimes_A C')
$$
*est bijective*.

Soient $u : (C, d) \to (C_1, d_1)$ un morphisme de complexes de $A$-modules à droite et $u' : (C', d') \to (C'_1, d'_1)$ un morphisme de complexes de $A$-modules à gauche; alors $u \otimes u' : C \otimes_A C' \to C_1 \otimes_A C'_1$ est un morphisme de complexes de $k$-modules; en effet, il est gradué de degré 0, et si l’on note $D$ et $D_1$ les différentielles de $C \otimes C'$ et $C_1 \otimes C'_1$, on a pour $p, q \in \mathbf{Z}, x \in C_p, x' \in C'_q$,
$$
(u \otimes u') (D(x \otimes x')) = u(dx) \otimes u'(x') + (-1)^p u(x) \otimes u'(d'x') =
= d_1 u(x) \otimes u'(x') + (-1)^p u(x) \otimes d'_1 u'(x') = D_1(u(x) \otimes u'(x')) .
$$
De plus le diagramme suivant est commutatif :
$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
H(u) \otimes H(u') \downarrow & & \downarrow H(u \otimes u') \\
H(C_1) \otimes_A H(C'_1) & \xrightarrow{\gamma(C_1, C'_1)} & H(C_1 \otimes_A C'_1)
\end{array}
$$

Soient $A^\circ$ la $k$-algèbre opposée à $A$, $C^\circ$ (resp. ${C'}^\circ$) le complexe $C$ (resp. $C'$) considéré comme complexe de $A^\circ$-modules à gauche (resp. droite). Notons
$$
\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_{A^\circ} C^\circ
$$
l’unique application $k$-linéaire graduée de degré 0 telle que, pour $x \in C_p, x' \in C'_q, p, q \in \mathbf{Z}$, on ait
$$
\sigma(C, C') (x \otimes x') = (-1)^{pq} x' \otimes x .
$$

#### Proposition 2 {#alg-x-s4-prop-2 .statement}

L’application $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ est un isomorphisme de complexes de $k$-modules, dont l’isomorphisme réciproque est $\sigma({C'}^\circ, C^\circ)$.

Comme les applications $\sigma(C, C')$ et $\sigma({C'}^\circ, C^\circ)$ sont réciproques l’une de l’autre, il suffit de prouver que $\sigma(C, C')$ est un morphisme de complexes. Or, pour
$$
x \in C_p = C_p^\circ, \quad x' \in C'_q = C_{q'}^\circ, \quad p, q \in \mathbf{Z},
$$
on a, notant $D'$ la différentielle de $C' \otimes_{A^\circ} C$,
$$
\begin{align*}
\sigma(C, C') \circ D(x \otimes x') &= \sigma(C, C') (dx \otimes x' + (-1)^p x \otimes d'x') = \\
&= (-1)^{(p+1)q} x' \otimes dx + (-1)^{p+p(q+1)} d'x' \otimes x = (-1)^{pq} d'x' \otimes x + (-1)^{pq+q} x' \otimes dx \\
&= (-1)^{pq} D'(x' \otimes x) = D^\circ \circ \sigma(C, C') (x \otimes x');
\end{align*}
$$
cela donne $\sigma(C, C') \circ D = D^\circ \circ \sigma(C, C')$, d’où l’assertion cherchée.

L’isomorphisme $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ est appelé *isomorphisme de commutation* du produit tensoriel des complexes $C$ et $C'$.

Si $u : C \to C_1$ et $v : C' \to C'_1$ sont deux morphismes de complexes comme ci-dessus, on a un diagramme commutatif :

$$
\begin{array}{ccc}
C \otimes_A C' & \xrightarrow{\sigma(C, C')} & {C'}^\circ \otimes_A C^\circ \\
u \otimes u' \downarrow & & \downarrow u' \otimes u \\
C_1 \otimes_A C'_1 & \xrightarrow{\sigma(C_1, C'_1)} & C'_1{}^\circ \otimes_A C_1^\circ.
\end{array}
$$

Supposons pour la fin de ce numéro que l’anneau $A$ soit *commutatif* (*cf.* n° 9 pour le cas général).

Soient $C, C', C''$ trois complexes de $A$-modules ; l’homomorphisme canonique de $A$-modules (III, p. 64)
$$
\varphi : (C \otimes_A C') \otimes_A C'' \to C \otimes_A (C' \otimes_A C'')
$$
est un *isomorphisme de complexes*, comme on le vérifie aussitôt à l’aide des définitions.

Plus généralement, soit $(C^{(i)}, d^{(i)})_{i \in I}$ une *famille de complexes* de $A$-modules, où l’ensemble $I$ est *fini et totalement ordonné* ; nous identifierons pour simplifier les notations $I$ à l’intervalle $[1, r]$ de $\mathbf{N}$. Munissons le $A$-module $C = \bigotimes_{i=1}^r C^{(i)}$ de la graduation telle que
$$
C_n = \sum_{p_1 + p_2 + \cdots + p_r = n} (C^{(1)})_{p_1} \otimes (C^{(2)})_{p_2} \otimes \cdots \otimes (C^{(r)})_{p_r},
$$
et définissons un $A$-endomorphisme gradué de degré $(-1)$ de $C$ par
$$
D(x_1 \otimes \ldots \otimes x_r) = \sum_{j=1}^r (-1)^{p_1 + \cdots + p_{j-1}} x_1 \otimes \ldots \otimes x_{j-1} \otimes d_j x_j \otimes x_{j+1} \otimes \ldots \otimes x_r
$$
où $x_i \in (C^{(i)})_{p_i}$ pour $i = 1, \ldots, n$. Alors $(C, D)$ est un complexe de $A$-modules appelé complexe produit tensoriel de la famille $(C_i, d_i)$. Pour toute suite strictement croissante $r_0, ..., r_k$ de $[0, r]$ telle que $r_0 = 0,\ r_k = r$, l’isomorphisme canonique d’associativité

$$
\bigotimes_{j=0}^{k-1} \left( \bigotimes_{i=r_j+1}^{r_{j+1}} C^{(i)} \right) \to \bigotimes_{i=1}^r C^{(i)}
$$

est un isomorphisme de complexes.

On définit comme ci-dessus un homomorphisme gradué de degré 0

$$
\gamma((C^{(i)})) : \bigotimes_{i \in I} H(C^{(i)}) \to H \left( \bigotimes_{i \in I} C^{(i)} \right)
$$

#### Remarque 3 {#alg-x-s4-n1-rem-3 .statement}

On peut définir le produit tensoriel d’une famille finie de complexes sans munir l’ensemble d’indices d’un ordre total (X, p. 185, exercice 3).

#### Remarque 4 {#alg-x-s4-n1-rem-4 .statement}

Supposons que chaque $C^{(i)}$ soit muni d’une structure d’algèbre graduée compatible avec sa graduation et telle que les $d^{(i)}$ soient des antidérivations (III, p. 117). Munissons alors $\bigotimes_{i \in I} C^{(i)}$ de la structure d’algèbre produit tensoriel gradué gauche des structures données (III, p. 49). Alors D est une antidérivation. En effet, utilisant l’associativité du produit tensoriel, on peut supposer que $I = \{1, 2\}$; soit alors $p_1,\ q_1,\ p_2,\ q_2 \in \mathbf{Z},\ x_1 \in (C^{(1)})_{p_1},\ y_1 \in (C^{(1)})_{q_1},\ x_2 \in (C^{(2)})_{p_2},\ y_2 \in (C^{(2)})_{q_2}$; on a

$$
(D(x_1 \otimes x_2))(y_1 \otimes y_2) + (-1)^{p_1+p_2} (x_1 \otimes x_2)(D(y_1 \otimes y_2)) =
$$
$$
= (dx_1 \otimes x_2 + (-1)^{p_1} x_1 \otimes dx_2)(y_1 \otimes y_2) +
$$
$$
+ (-1)^{p_1+p_2} (x_1 \otimes x_2)(dy_1 \otimes y_2 + (-1)^{q_1} y_1 \otimes dy_2) =
$$
$$
= (-1)^{p_2 q_1} (dx_1) y_1 \otimes x_2 y_2 + (-1)^{p_1+(p_2-1)q_1} x_1 y_1 \otimes (dx_2) y_2 +
$$
$$
+ (-1)^{p_1+p_2+p_2(q_1-1)} x_1 dy_1 \otimes x_2 y_2 + (-1)^{p_1+p_2+q_1+p_2 q_1} x_1 y_1 \otimes x_2 dy_2
$$
$$
= (-1)^{p_2 q_1} [(dx_1) y_1 + (-1)^{p_1} x_1 dy_1] \otimes x_2 y_2 +
$$
$$
+ (-1)^{p_1+q_1+p_2 q_1} x_1 y_1 \otimes ((dx_2) y_2 + (-1)^{p_2} x_2 dy_2)
$$
$$
= (-1)^{p_2 q_1} [d(x_1 y_1) \otimes x_2 y_2 + (-1)^{p_1+q_1} x_1 y_1 \otimes d(x_2 y_2)]
$$
$$
= (-1)^{p_2 q_1} D(x_1 y_1 \otimes x_2 y_2) = D((x_1 \otimes x_2)(y_1 \otimes y_2)).
$$

### 2. Produits tensoriels et homotopie

#### Proposition 3 {#alg-x-s4-prop-3 .statement}

Soient $C,\ C_1$ deux complexes de $A$-modules à droite, $C',\ C'_1$ deux complexes de $A$-modules à gauche, et $u : C \to C_1,\ v : C \to C_1,\ u' : C' \to C'_1,\ v' : C' \to C'_1$ des morphismes de complexes.

a) Si $u$ et $u'$ sont homotopes à $v$ et $v'$ respectivement, alors les deux morphismes $u \otimes u'$ et $v \otimes v'$ de $C \otimes_A C'$ dans $C_1 \otimes_A C'_1$ sont homotopes.

b) Si $u$ et $u'$ sont des homotopismes, $u \otimes u'$ est un homotopisme.

c) Si $C$ ou $C'$ est homotope à zéro, $C \otimes_A C'$ est homotope à zéro.

Notons par la même lettre $d$ les différentielles des complexes $C,\ C_1,\ C',\ C'_1$ et par $D$ les différentielles des complexes $C \otimes_A C'$ et $C_1 \otimes_A C'_1$.

Si $u$ (resp. $u'$) est homotope à $v$ (resp. $v'$), il existe un homomorphisme gradué
de degré 1 $s:C\to C_1$ (resp. $s':C'\to C'_1$) tel que

$$
(2)\qquad u-v=ds+sd\qquad\text{(resp. }u'-v'=ds'+s'd\text{)}.
$$

Soit $S:C\otimes_A C'\to C_1\otimes_A C'_1$ l’unique homomorphisme gradué de degré 1 tel
que, pour $x\in C_p,\ y\in C'_q,\ p,q\in\mathbf Z$, on ait

$$
(3)\qquad S(x\otimes y)=s(x)\otimes u'(y)+(-1)^p v(x)\otimes s'(y).
$$

On a alors, avec les notations précédentes :

$$
\begin{aligned}
(DS+SD)(x\otimes y)&=D(sx\otimes u'y)+(-1)^pD(vx\otimes s'y)+S(dx\otimes y)\\
&\quad+(-1)^pS(x\otimes dy)=\\
&=dsx\otimes u'y+(-1)^{p+1}sx\otimes du'y+(-1)^pdvx\otimes s'y+vx\otimes ds'y\\
&\quad+sdx\otimes u'y+(-1)^{p-1}vdx\otimes s'y+(-1)^psx\otimes u'dy+vx\otimes s'dy\\
&=(ds+sd)(x)\otimes u'y+vx\otimes(ds'+s'd)(y)\\
&=(ux-vx)\otimes u'y+vx\otimes(u'y-v'y)=ux\otimes u'y-vx\otimes v'y.
\end{aligned}
$$

Cela donne $DS+SD=u\otimes u'-v\otimes v'$, d’où a).

Démontrons b). Si $u$ et $u'$ sont des homotopismes, il existe des homomorphismes
de complexes $\alpha:C_1\to C$ et $\alpha':C'_1\to C'$ tels que $u\circ\alpha,\ \alpha\circ u',\ \alpha'\circ u'$ soient
homotopes respectivement à $\mathrm{Id}_{C_1},\ \mathrm{Id}_C,\ \mathrm{Id}_{C'_1},\ \mathrm{Id}_{C'}$. Alors $(u\otimes u')\circ(\alpha\otimes\alpha')$, qui
est égal à $(u\circ\alpha)\otimes(u'\circ\alpha')$, est homotope d’après a) à $\mathrm{Id}_{C_1}\otimes\mathrm{Id}_{C'_1}=\mathrm{Id}_{C_1\otimes C'_1}$,
tandis que $(\alpha\otimes\alpha')\circ(u\otimes u')$ est homotope à $\mathrm{Id}_{C\otimes C'}$, d’où b). Enfin, c) résulte
de b) appliqué au cas où $C_1$ ou $C'_1$ est nul.

#### Corollaire 1 {#alg-x-s4-prop-3-cor-1 .statement}

Soit $C'$ un complexe scindé de $A$-modules à gauche tel que $H(C')$
soit plat. Pour tout complexe $C$ de $A$-modules à droite, l’application canonique

$$
\gamma(C,C'):H(C)\otimes_AH(C')\longrightarrow H(C\otimes_A C')
$$

est bijective.

D’après X, p. 35, déf. 6, il existe un homotopisme $u':C'\to H(C')$. D’après
la prop. 3, $1_C\otimes u':C\otimes_A C'\to C\otimes_AH(C')$ est un homotopisme ; comme

$$
H(1_C\otimes u')\circ\gamma(C,C')=\gamma(C,H(C'))\circ(1_C\otimes H(u')),
$$

et que $H(1_C\otimes u')$ et $H(u')$ sont bijectifs, il suffit de prouver que $\gamma(C,H(C'))$ est
bijective, et on est ramené au cas où $C'$ est plat et à différentielle nulle. Dans ce cas
les suites exactes canoniques

$$
\mathrm{(I)}\qquad 0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\partial}B(C)\longrightarrow0
$$

$$
\mathrm{(II)}\qquad 0\longrightarrow B(C)\xrightarrow{j}Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

donnent des suites exactes :

$$
0 \longrightarrow Z(C) \otimes_A C' \xrightarrow{i\otimes 1} C \otimes_A C' \xrightarrow{\delta\otimes 1} B(C) \otimes_A C' \longrightarrow 0
$$

$$
0 \longrightarrow B(C) \otimes_A C' \xrightarrow{j\otimes 1} Z(C) \otimes_A C' \xrightarrow{\pi\otimes 1} H(C) \otimes_A C' \longrightarrow 0.
$$

Comme $d=i\circ j\circ\delta$, on a $D=d\otimes 1_{C'}=(i\otimes 1)\circ(j\otimes 1)\circ(\delta\otimes 1)$, ce qui montre que les applications canoniques $Z(C)\otimes_A C'\to Z(C\otimes_A C')$ et $B(C)\otimes_A C'\to B(C\otimes_A C')$ sont bijectives, donc aussi $\gamma(C,C')$ par passage aux quotients.

#### Corollaire 2 {#alg-x-s4-prop-3-cor-2 .statement}

Soit $\mathbf N$ un A-module à gauche plat. Pour tout complexe C de A-modules à droite, les homomorphismes canoniques

$$
\gamma_n(C,\mathbf N): H_n(C)\otimes_A \mathbf N \longrightarrow H_n(C\otimes_A \mathbf N)
$$

sont bijectifs.

#### Corollaire 3 {#alg-x-s4-prop-3-cor-3 .statement}

Soit $C'$ un complexe de A-modules à gauche tel que $B(C')$ et $H(C')$ soient projectifs. Pour tout complexe C de A-modules à droite, l’application $\gamma(C,C')$ est bijective.

En effet, $C'$ est scindé (X, p. 35, exemple 4) et $H(C')$ est projectif ; on peut donc appliquer le corollaire 1.

#### Remarque 1 {#alg-x-s4-n2-rem-1 .statement}

En utilisant les isomorphismes de commutation, on déduit des corollaires 1, 2 et 3 les énoncés analogues obtenus en échangeant les rôles des deux arguments des produits tensoriels.

#### Remarque 2 {#alg-x-s4-n2-rem-2 .statement}

Nous verrons ci-dessous (X, p. 79, cor. 4) que la conclusion du cor. 1 est également vraie lorsqu’on suppose $C'$ et $H(C')$ plats et $C'$ borné à droite.

### 3. Produit tensoriel par un complexe plat borné à droite

#### Lemme 1 {#alg-x-s4-lem-1 .statement}

Soient C un complexe de A-modules à droite et E un complexe de A-modules à gauche. On suppose que $H(C)=0$ et que E est plat et borné à droite. Alors $H(C\otimes_A E)=0$.

Pour $k\in\mathbf Z$, soit $T^{(k)}$ le sous-complexe de $C\otimes_A E$ tel que

$$
T_n^{(k)}=\sum_{\substack{p+q=n\\q\leq k}} C_p\otimes_A E_q\ ;
$$

alors $T^{(k-1)}\subset T^{(k)}$ et on a une suite exacte de complexes

$$
0\longrightarrow T^{(k-1)}\xrightarrow{i_k}T^{(k)}\xrightarrow{\pi}C\otimes_A E_k(-k)\longrightarrow 0
$$

où $i_k$ est l’injection canonique et où $\pi$ projette la somme directe précédente sur son facteur $C_{n-k}\otimes_A E_k=(C\otimes_A E_k(-k))_n$. D’après le cor. 2 ci-dessus, on a $H(C\otimes_A E_k(-k))=0$, donc $i_k$ est un homomorphisme. On a $T^{(k)}=0$ pour $k$ assez petit, puisque $E$ est borné à droite, donc $H(T^{(k)})=0$ pour tout $k$ par récurrence sur $k$. Enfin, le morphisme canonique $\underset{\longrightarrow}{\lim}\,T^{(k)}\to C\otimes_A E$ est évidemment un isomorphisme, donc $H(C\otimes_A E)=0$ (X, p. 28, prop. 1).

#### Lemme 2 {#alg-x-s4-lem-2 .statement}

Si $u:C\to C'$ est un morphisme de complexes de A-modules à droite et $E$ un complexe de A-modules à gauche, alors les complexes $\operatorname{Con}(u)\otimes_A E$ et $\operatorname{Con}(u\otimes 1_E)$ sont isomorphes.

Par définition, $\operatorname{Con}(u)\otimes_A E$ est le module gradué $(C'(-1)\oplus C)\otimes_A E$ muni de la différentielle $D$ telle que, pour $x\in C_p$, $y'\in C'(-1)_p=C'_{p-1}$, $z\in E_q$, on ait

(4)
$$
D(y',x)\otimes z=(-dy',dx-u(y'))\otimes z+(-1)^p(y',x)\otimes dz,
$$

tandis que $\operatorname{Con}(u\otimes 1_E)$ est le module gradué $(C'\otimes_A E)(-1)\oplus(C\otimes_A E)$ muni de la différentielle $D_1$ telle que, pour $x\in C_p$, $y'\in C'_{p-1}$, $z\in E_q$, on ait

$$
D_1(y'\otimes z,x\otimes z)=(-dy'\otimes z-(-1)^{p-1}y'\otimes dz,dx\otimes z+(-1)^p x\otimes dz-u(y')\otimes z)
$$

$$
=(-dy'\otimes z,(dx-u(y'))\otimes z)+(-1)^p(y'\otimes dz,x\otimes dz),
$$

d’où l’assertion.

#### Proposition 4 {#alg-x-s4-prop-4 .statement}

Soient $u:C\to C'$ un homologisme de complexes de A-modules à droite et $E$ un complexe de A-modules à gauche, plat et borné à droite. Alors

$$
u\otimes 1_E:C\otimes_A E\to C'\otimes_A E
$$

est un homologisme de complexes de $k$-modules.

En effet, d’après X, p. 38, cor., $u$ (resp. $u\otimes 1_E$) est un homologisme si et seulement si $H(\operatorname{Con}(u))=0$ (resp. $H(\operatorname{Con}(u\otimes 1_E))=0$). On conclut alors par les lemmes 1 et 2.

#### Remarque {#alg-x-s4-n3-rem-1 .statement}

En utilisant les isomorphismes de commutation, on déduit des énoncés précédents les énoncés analogues obtenus en échangeant les rôles des deux arguments des produits tensoriels.

### 4. Définition et premières propriétés du produit de torsion

Pour tout A-module $E$, on note $p_E:L(E)\to E$ la résolution libre canonique de $E$ (X, p. 50).

#### Définition 1 {#alg-x-s4-def-1 .statement}

Soit $M$ un A-module à droite et $N$ un A-module à gauche. On appelle produit de torsion de $M$ et $N$ le $k$-module gradué

(4)
$$
\operatorname{Tor}^A(M,N)=H(L(M)\otimes_A L(N)).
$$

Les composantes homogènes de $\operatorname{Tor}^A(M,N)$ sont notées

(5)
$$
\operatorname{Tor}^A_n(M,N)=H_n(L(M)\otimes_A L(N)).
$$

Comme $L(M)$ et $L(N)$ sont nuls à droite, on a

(6)
$$
\operatorname{Tor}_n^A(M, N) = 0 \quad \text{pour } n < 0 .
$$

#### Remarque 1 {#alg-x-s4-n4-rem-1 .statement}

Nous verrons ci-dessous (X, p. 107, prop. 6) des propriétés de finitude des modules $\operatorname{Tor}^A(M, N)$. Par exemple, si $A$ est commutatif noethérien et si $M$ et $N$ sont des $A$-modules de type fini, chaque $A$-module $\operatorname{Tor}_n^A(M, N)$ est de type fini.

Soient $f : M \to M'$ un homomorphisme de $A$-modules à droite et $g : N \to N'$ un homomorphisme de $A$-modules à gauche, on pose $\operatorname{Tor}^A(f, g) = H(L(f) \otimes_A L(g))$; c’est un homomorphisme de $k$-modules gradués

$$
\operatorname{Tor}^A(f, g) : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^A(M', N')
$$

dont les composantes homogènes sont notées

$$
\operatorname{Tor}_n^A(f, g) : \operatorname{Tor}_n^A(M, N) \to \operatorname{Tor}_n^A(M', N') .
$$

D’après la prop. 1 de X, p. 62, l’homomorphisme canonique

$$
\gamma_{0,0} : H_0(L(M)) \otimes_A H_0(L(N)) \to H_0(L(M) \otimes_A L(N))
$$

est bijectif ; utilisant les isomorphismes $M \to H_0(L(M))$ et $N \to H_0(L(N))$, on en tire un isomorphisme, dit *canonique*

(7)
$$
\gamma_{M,N} : M \otimes_A N \to \operatorname{Tor}_0^A(M, N) .
$$

Nous identifierons toujours $\operatorname{Tor}_0^A(M, N)$ à $M \otimes_A N$ par cet isomorphisme. Alors l’application $k$-linéaire $\operatorname{Tor}_0^A(f, g)$ s’identifie à $f \otimes g$.

#### Remarque 2 {#alg-x-s4-n4-rem-2 .statement}

Le morphisme de complexes $p_M \otimes p_N : L(M) \otimes_A L(N) \to M \otimes_A N$ induit sur l’homologie de degré 0 l’isomorphisme

$$
\gamma_{M,N}^{-1} : \operatorname{Tor}_0^A(M, N) \to M \otimes_A N
$$

réciproque de $\gamma_{M,N}$.

On a $L(1_M) = 1_{L(M)}$, $L(1_N) = 1_{L(N)}$, donc par passage à l’homologie :

(8)
$$
\operatorname{Tor}^A(1_M, 1_N) = 1_{\operatorname{Tor}^A(M, N)} .
$$

Si $f' : M' \to M''$ (resp. $g' : N' \to N''$) est un homomorphisme de $A$-modules à droite (resp. gauche), on a $L(g' \circ g) = L(g') \circ L(g)$ et $L(f' \circ f) = L(f') \circ L(f)$, donc

(9)
$$
\operatorname{Tor}^A(f' \circ f, g' \circ g) = \operatorname{Tor}^A(f', g') \circ \operatorname{Tor}^A(f, g) .
$$

Considérons les morphismes de $k$-complexes

$$
L(M) \otimes_A N \xleftarrow{1 \otimes p_N} L(M) \otimes_A L(N) \xrightarrow{p_M \otimes 1} M \otimes_A L(N)
$$

et les $k$-homomorphismes qu’ils induisent en homologie :

$$
H(L(M) \otimes_A N) \xleftarrow{\psi_{M(N)}} \mathrm{Tor}^A(M, N) \xrightarrow{\overline{\psi}_{N(M)}} H(M \otimes_A L(N)) ;
$$

d’après la prop. 4 de X, p. 67, $1 \otimes p_N$ et $p_M \otimes 1$ sont des homologismes. D’où :

**Proposition 5. — Les $k$-homomorphismes**

$$
\begin{aligned}
& \psi_M(N) : \mathrm{Tor}^A(M, N) \to H(L(M) \otimes_A N) \\
& \overline{\psi}_N(M) : \mathrm{Tor}^A(M, N) \to H(M \otimes_A L(N))
\end{aligned}
$$

sont *bijectifs*.

**Corollaire. — Si $M$ ou $N$ est plat, $\mathrm{Tor}_i^A(M, N) = 0$ pour $i \geqslant 0$.**

Supposons $N$ (resp. $M$) plat ; alors $p_M \otimes 1 : L(M) \otimes_A N \to M \otimes_A N$ (resp. $1 \otimes p_N : M \otimes_A L(N) \to M \otimes_A N$) est un homologisme (X, p. 67, prop. 4), donc $H_i(L(M) \otimes_A N)$ (resp. $H_i(M \otimes_A L(N))$) est nul pour $i > 0$.

*Remarque 3. — Si $g : N \to N'$ est un homomorphisme de A-modules à gauche, alors*

$$
(1_{L(M)} \otimes g) \circ (1_{L(M)} \otimes 1_N) = (1_{L(M)} \otimes 1_N) \circ (1_{L(M)} \otimes L(g)) ,
$$

donc le diagramme

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\psi_{M(N)}} & H(L(M) \otimes_A N) \\
\mathrm{Tor}^A(1, g) \downarrow & & \downarrow H(1 \otimes g) \\
\mathrm{Tor}^A(M, N') & \xrightarrow{\psi_{M(N')}} & H(L(M) \otimes_A N')
\end{array}
$$

est commutatif.

De même, si $f : M \to M'$ est un homomorphisme de A-modules à droite, on a un diagramme commutatif :

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\overline{\psi}_{N(M)}} & H(M \otimes_A L(N)) \\
\mathrm{Tor}^A(f, 1) \downarrow & & \downarrow H(f \otimes 1) \\
\mathrm{Tor}^A(M', N) & \xrightarrow{\overline{\psi}_{N(M')}} & H(M' \otimes_A L(N)) .
\end{array}
$$

**Proposition 6. — L’application** $(f, g) \mapsto \mathrm{Tor}^A(f, g) :$

$$
\mathrm{Hom}_A(M, M') \times \mathrm{Hom}_A(N, N') \to \mathrm{Hom}_k(\mathrm{Tor}^A(M, N), \mathrm{Tor}^A(M', N'))
$$

*est $k$*-bilinéaire.

Soient $f \in \mathrm{Hom}_A(M, M')$, $g_1, g_2 \in \mathrm{Hom}_A(N, N')$, $\lambda_1, \lambda_2 \in k$. Alors les morphismes

$$
\lambda_1(L(f) \otimes g_1) + \lambda_2(L(f) \otimes g_2) \quad \text{et} \quad L(f) \otimes (\lambda_1 g_1 + \lambda_2 g_2)
$$

de $L(M) \otimes_A N$ dans $L(M) \otimes_A N'$ coïncident ; d’après la prop. 5 et la remarque 3, on a donc

(10) $$
\mathrm{Tor}^A(f, \lambda_1 g_1 + \lambda_2 g_2) = \lambda_1 \mathrm{Tor}^A(f, g_1) + \lambda_2 \mathrm{Tor}^A(f, g_2).
$$

On raisonne de même pour l’application $f \mapsto \mathrm{Tor}^A(f, g)$.

#### Corollaire {#alg-x-s4-n4-cor-1 .statement}

*Soit $\lambda \in k$. Si $\lambda$ annule $M$ ou $N$, il annule $\mathrm{Tor}^A(M, N)$.*
En effet, $\lambda . 1_{\mathrm{Tor}(M, N)} = \mathrm{Tor}(\lambda . 1_M, 1_N) = \mathrm{Tor}(1_M, \lambda . 1_N)$.

#### Proposition 7 {#alg-x-s4-prop-7 .statement}

*Soient I et J deux ensembles, $(M_\alpha)_{\alpha \in I}$ une famille de A-modules à droite, $(N_\beta)_{\beta \in J}$ une famille de A-modules à gauche. L’homomorphisme*

$$
\bigoplus_{\alpha \in I, \beta \in J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \bigoplus_{\alpha \in I} M_\alpha, \bigoplus_{\beta \in J} N_\beta \right)
$$

*déduit des homomorphismes canoniques* $M_\alpha \to \bigoplus M_\alpha$ *et* $N_\beta \to \bigoplus N_\beta$ *est bijectif*.

Il suffit de prouver que pour tout module à droite $M$ (resp. tout module à gauche $N$), l’homomorphisme canonique

$$
\bigoplus_{\beta \in J} \mathrm{Tor}^A(M, N_\beta) \to \mathrm{Tor}^A(M, \bigoplus_{\beta \in J} N_\beta)
$$

(resp. $\bigoplus_{\alpha \in I} \mathrm{Tor}^A(M_\alpha, N) \to \mathrm{Tor}^A(\bigoplus_{\alpha \in I} M_\alpha, N)$) est bijectif. Or cela résulte de ce qui précède, de la proposition 1 de X, p. 28, et des isomorphismes canoniques :

$$
\bigoplus_{\beta} (L(M) \otimes_A N_\beta) \to L(M) \otimes_A (\bigoplus_{\beta} N_\beta),
$$
$$
\bigoplus_{\alpha} (M_\alpha \otimes_A L(N)) \to (\bigoplus_{\alpha} M_\alpha) \otimes_A L(N).
$$

Un raisonnement analogue donne :

#### Proposition 8 {#alg-x-s4-prop-8 .statement}

*Soient I (resp. J) un ensemble préordonné filtrant à droite, (($M_\alpha$, $u_{\alpha', \alpha}$) (resp. (($N_\beta$, $v_{\beta', \beta}$))) un système inductif de A-modules à droite (resp. gauche) relatif à I (resp. J). L’homomorphisme de k-modules gradués*

$$
\lim_{\longrightarrow (\alpha, \beta) \in I \times J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \lim_{\longrightarrow \alpha \in I} M_\alpha, \lim_{\longrightarrow \beta \in J} N_\beta \right),
$$

*déduit des A-homomorphismes canoniques* $M_\alpha \to \lim_{\longrightarrow} M_\alpha$ *et* $N_\beta \to \lim_{\longrightarrow} N_\beta$, *est bijectif*.

En particulier, prenant $J = I$ et remarquant que les $(\alpha, \alpha), \alpha \in I$, forment une partie cofinale de $I \times I$, on obtient :

#### Corollaire {#alg-x-s4-n4-cor-2 .statement}

Soient I un ensemble préordonné filtrant à droite, $(M_i, u_{ji})$ (resp. $(N_i, v_{ji})$) un système inductif de $A$-modules à droite (resp. à gauche) relatif à I. L’homomorphisme de $k$-modules gradués

$$
\lim_{\longrightarrow i \in I} \operatorname{Tor}^A(M_i, N_i) \to \operatorname{Tor}^A\left(\lim_{\longrightarrow i \in I} M_i, \lim_{\longrightarrow i \in I} N_i\right),
$$

déduit des $A$-homomorphismes canoniques $M_i \to \lim_{\longrightarrow} M_i$ et $N_j \to \lim_{\longrightarrow} N_j$ est bijectif.

Soient $M$ un $A$-module à droite, $N$ un $A$-module à gauche, $A^\circ$ l’anneau opposé à $A$, $M^\circ$ le $A^\circ$-module à gauche sous-jacent à $M$, $N^\circ$ le $A^\circ$-module à droite sous-jacent à $M$. On a $L(M^\circ) = L(M)^\circ$ et $L(N^\circ) = L(N)^\circ$, d’où un isomorphisme de commutation (X, p. 63, prop. 2)

$$
\sigma(L(M), L(N)) : L(M) \otimes_A L(N) \to L(N^\circ) \otimes_{A^\circ} L(M^\circ).
$$

Par passage à l’homologie, $\sigma(L(M), L(N))$ induit un isomorphisme gradué de degré 0 $\sigma_{M,N} : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^{A^\circ}(N^\circ, M^\circ)$ dit *isomorphisme de commutation des produits de torsion*.

Notons que $\sigma_{N^\circ, M^\circ} \circ \sigma_{M,N} = \mathrm{Id}_{\operatorname{Tor}(M,N)}$ et que $\sigma_{M,N}$ induit sur les termes de degré 0 l’homomorphisme de commutation du produit tensoriel. D’autre part, si $f : M \to M'$ et $g : N \to N'$ sont des homomorphismes de $A$-modules, on a

$$
\operatorname{Tor}^{A^\circ}(g, f) \circ \sigma_{M,N} = \sigma_{M', N'} \circ \operatorname{Tor}^A(f, g).
$$

### 5. Les homomorphismes de liaison et les suites exactes

Soit $M$ un $A$-module à droite. Rappelons que pour tout $A$-module à gauche $N$, on a défini au numéro précédent (X, p. 69, prop. 5) un isomorphisme

$$
\psi_M(N) : \operatorname{Tor}^A(M, N) \to H(L(M) \otimes_A N).
$$

Soit

$$(\mathcal{E})$$
$$
0 \to N' \xrightarrow{u} N \xrightarrow{v} N'' \to 0
$$

une suite exacte de $A$-modules à gauche ; la suite de $k$-complexes

$$(\mathcal{M}\mathcal{E})$$
$$
0 \longrightarrow L(M) \otimes_A N' \xrightarrow{1 \otimes u} L(M) \otimes_A N \xrightarrow{1 \otimes v} L(M) \otimes_A N'' \longrightarrow 0
$$

est alors exacte (X, p. 66, *lemme* 1); soit

$$
\partial^{(\mathcal{M}\mathcal{E})} : H(L(M) \otimes_A N'') \to H(L(M) \otimes_A N')
$$

l’homomorphisme de liaison correspondant (X, p. 29).

#### Définition 2 {#alg-x-s4-def-2 .statement}

On appelle homomorphisme de liaison des produits de torsion, relatif au module M et à la suite exacte $\mathcal{E}$, l’homomorphisme composé

$$
\partial(M, \mathcal{E}) = \psi_M(N')^{-1} \circ \partial^{(M\mathcal{E})} \circ \psi_M(N'') : \mathrm{Tor}^A(M, N'') \to \mathrm{Tor}^A(M, N')
$$

C’est un $k$-homomorphisme gradué de degré ($-1$), dont les composantes homogènes sont notées $\partial_n(M, \mathcal{E}) : \mathrm{Tor}_n^A(M, N'') \to \mathrm{Tor}_{n-1}^A(M, N')$.

#### Théorème 1 {#alg-x-s4-thm-1 .statement}

La suite illimitée à gauche d’homomorphismes de $k$-modules

$$
\cdots \longrightarrow \mathrm{Tor}_n^A(M, N') \xrightarrow{\mathrm{Tor}_n^A(1, u)} \mathrm{Tor}_n^A(M, N) \xrightarrow{\mathrm{Tor}_n^A(1, v)} \mathrm{Tor}_n^A(M, N'')
$$
$$
\xrightarrow{\partial_n(M, \mathcal{E})} \mathrm{Tor}_{n-1}^A(M, N') \xrightarrow{\mathrm{Tor}_{n-1}^A(1, u)} \cdots \xrightarrow{\mathrm{Tor}_1^A(1, v)} \mathrm{Tor}_1^A(M, N'')
$$
$$
\xrightarrow{\hat{c}_1(M, \mathcal{E})} M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

est exacte.

Considérons en effet le diagramme

$$
\begin{array}{ccccccccc}
\mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) & \xrightarrow{\mathrm{Tor}(1, v)} & \mathrm{Tor}(M, N'') & \xrightarrow{\partial(M, \mathcal{E})} & \mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) \\
\psi_M(N') \downarrow & & \psi_M(N) \downarrow & & \psi_M(N'') \downarrow & & \psi_M(N') \downarrow & & \psi_M(N') \downarrow \\
H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N) & \xrightarrow{H(1 \otimes v)} & H(L(M \otimes N'') & \xrightarrow{\partial^{(M\mathcal{E})}} & H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N)
\end{array}
$$

Il est commutatif d’après (X, p. 69, remarque 3) et la déf. 2. D’autre part, la ligne inférieure est exacte (X, p. 30, th. 1), et les différents $\psi_M$ sont bijectifs (X, p. 69, prop. 5).

#### Corollaire 1 {#alg-x-s4-thm-1-cor-1 .statement}

Si $\mathrm{Tor}_1^A(M, N'') = 0$, la suite

$$
0 \longrightarrow M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

est exacte.

#### Corollaire 2 {#alg-x-s4-thm-1-cor-2 .statement}

Soient $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ une suite exacte de complexes de $A$-modules à gauche et $E$ un complexe de $A$-modules à droite. Si $C''$ ou $E$ est plat, la suite

$$
0 \longrightarrow E \otimes_A C' \xrightarrow{1 \otimes u} E \otimes_A C \xrightarrow{1 \otimes v} E \otimes_A C'' \longrightarrow 0
$$

est exacte.

En effet, $\mathrm{Tor}_1^A(E, C'') = 0$ d’après X, p. 69, cor. à la prop. 5.

#### Exemple {#alg-x-s4-n5-exa-1 .statement}

Soit $a$ un idéal de $A$. La suite exacte

$$
0 \to a \to A_s \to A/a \to 0
$$

de A-modules à gauche, donne naissance à une suite exacte de produits de torsion, dans laquelle les termes Tor$_i^A$ (M, A) sont nuls pour $i > 0$. On en déduit des isomorphismes

$$
\operatorname{Tor}_{i+1}^A(M, A/\alpha) \to \operatorname{Tor}_i^A(M, \alpha), \quad i > 0
$$

et une suite exacte

$$
0 \to \operatorname{Tor}_1^A(M, A\alpha) \to M \otimes_A \alpha \to M \otimes_A A \to M \otimes A \alpha \to 0 :
$$

il en résulte que $\operatorname{Tor}_1^A(M, A/\alpha)$ s’identifie au noyau de l’homomorphisme canonique $M \otimes_A \alpha \to M$.

Par exemple, prenant pour M un module de la forme $A_d/b$, où b est un idéal à droite de A, on obtient un isomorphisme de $\operatorname{Tor}_1^A(A/b, A/\alpha)$ sur $(\alpha \cap b)/ba$.

#### Proposition 9 {#alg-x-s4-prop-9 .statement}

*Soient f : M → M$_1$ un homomorphisme de A-modules à droite et*

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N' & \xrightarrow{u} & N & \xrightarrow{v} & N'' & \longrightarrow & 0 \\
& & g' \downarrow & & g \downarrow & & g'' \downarrow & & \\
0 & \longrightarrow & N'_1 & \xrightarrow{u_1} & N_1 & \xrightarrow{v_1} & N''_1 & \longrightarrow & 0
\end{array}
$$

*(E$_1$)*

*un diagramme commutatif à lignes exactes d’homomorphismes de A-modules à gauche. Le diagramme de k-modules*

$$
\begin{array}{ccc}
\operatorname{Tor}^A(M, N'') & \xrightarrow{\partial(M, E)} & \operatorname{Tor}^A(M, N') \\
\operatorname{Tor}^A(f, g'') \downarrow & & \operatorname{Tor}^A(f, g') \downarrow \\
\operatorname{Tor}^A(M_1, N''_1) & \xrightarrow{\partial(M_1, E_1)} & \operatorname{Tor}^A(M_1, N'_1)
\end{array}
$$

*est commutatif.*

Cela résulte de X, p. 31, prop. 2, appliquée au diagramme commutatif

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L(M) \otimes_A N' & \xrightarrow{1 \otimes u} & L(M) \otimes_A N & \xrightarrow{1 \otimes v} & L(M) \otimes_A N'' & \longrightarrow & 0 \\
& & L(f) \otimes g' \downarrow & & L(f) \otimes g \downarrow & & L(f) \otimes g'' \downarrow & & \\
0 & \longrightarrow & L(M_1) \otimes_A N'_1 & \xrightarrow{1 \otimes u_1} & L(M_1) \otimes_A N_1 & \xrightarrow{1 \otimes v_1} & L(M_1) \otimes_A N''_1 & \longrightarrow & 0 .
\end{array}
$$

De manière analogue, si N est un A-module à gauche et

$$(F)$$
$$
0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
$$

une suite exacte de A-modules à droite, on définit des *homomorphismes de liaison*

$$
\partial(F, N) : \operatorname{Tor}^A(M'', N) \to \operatorname{Tor}^A(M', N)
$$
$$
\partial_n(F, N) : \operatorname{Tor}_n^A(M'', N) \to \operatorname{Tor}_{n-1}^A(M', N)
$$

par $\partial(\mathcal F,\mathbf N)=\overline{\psi}_{\mathbf N}(M')^{-1}\circ\partial(\mathcal F^{\mathbf N})\circ\overline{\psi}_{\mathbf N}(M'')$, où $\partial(\mathcal F^{\mathbf N})$ est l’homomorphisme de
liaison de la suite exacte

$$(\mathcal F_{\mathbf N})\qquad 0\longrightarrow M'\otimes_A L(N)\longrightarrow M\otimes_A L(N)\longrightarrow M''\otimes_A L(N)\longrightarrow 0$$

déduite de $\mathcal F$, et on a :

**THÉORÈME 1 bis.** — *La suite illimitée à gauche d’homomorphismes de $k$-modules*

$$\longrightarrow \operatorname{Tor}_n^A(M',N)\xrightarrow{\operatorname{Tor}_n^A(r,1)}\operatorname{Tor}_n^A(M,N)\xrightarrow{\operatorname{Tor}_n^A(s,1)}\operatorname{Tor}_n^A(M'',N)\xrightarrow{\partial_n(\mathcal F,N)}\operatorname{Tor}_{n-1}^A(M',N)$$

$$\cdots\longrightarrow \operatorname{Tor}_1^A(M'',N)\xrightarrow{\partial_1(\mathcal F,N)}M'\otimes_A N\xrightarrow{r\otimes1}M\otimes_A N\xrightarrow{s\otimes1}M''\otimes_A N\longrightarrow0$$

*est exacte.*

On laisse au lecteur le soin d’énoncer et de démontrer les propriétés analogues
aux corollaires du th. 1 et à la prop. 9. D’ailleurs :

#### Proposition 10 {#alg-x-s4-prop-10 .statement}

*Notons $(\mathcal F^\circ)$ la suite exacte de $A$-modules à gauche*

$$0\longrightarrow M'\xrightarrow{r}M\xrightarrow{s}M''\longrightarrow0.$$

*Le diagramme*

$$
\begin{array}{ccccc}
\operatorname{Tor}^A(M'',N)&\xrightarrow{\partial(\mathcal F,N)}&\operatorname{Tor}^A(M',N)\\
\Big\downarrow{\sigma_{M'',N}}&&\Big\downarrow{\sigma_{M',N}}\\
\operatorname{Tor}^{A^\circ}(N^\circ,{M''}^\circ)&\xrightarrow{\partial(N^\circ,\mathcal F^\circ)}&\operatorname{Tor}^{A^\circ}(N^\circ,{M'}^\circ)
\end{array}
$$

*est commutatif.*

En effet, cela résulte de X, p. 31, prop. 2, appliquée au diagramme commutatif

$$
\begin{array}{ccccccccc}
0&\longrightarrow&M'\otimes_A L(N)&\xrightarrow{r\otimes1}&M\otimes_A L(N)&\xrightarrow{s\otimes1}&M''\otimes_A L(N)&\longrightarrow&0\\
&&\Big\downarrow{\sigma(M',L(N))}&&\Big\downarrow{\sigma(M,L(N))}&&\Big\downarrow{\sigma(M'',L(N))}\\
0&\longrightarrow&L(N^\circ)\otimes_{A^\circ}{M'}^\circ&\xrightarrow{1\otimes r}&L(N^\circ)\otimes_{A^\circ}M^\circ&\xrightarrow{1\otimes s}&L(N^\circ)\otimes_{A^\circ}{M''}^\circ&\longrightarrow&0 .
\end{array}
$$

Nous verrons plus tard d’autres relations de commutation *(cf.* X, p. 131, cor. 1*).*

### 6. Modules plats et produits de torsion

#### Théorème 2 {#alg-x-s4-thm-2 .statement}

*Soit E un $A$-module à droite. Les conditions suivantes sont équi-*
*valentes :*

(i) E *est plat* ;

(ii) *pour tout* $A$-module à gauche F, *et tout entier* $n>0$, *on a*

$$\operatorname{Tor}_n^A(E,F)=0\,;$$

(iii) pour tout $A$-module à gauche monogène et de présentation finie $F$, on a
$$
\operatorname{Tor}_1^A(E, F) = 0 ;
$$
(iv) pour tout idéal à gauche de type fini $a$ de $A$, l’application canonique $E \otimes_A a \to E$ est injective ;
(v) pour toute suite exacte de $A$-modules à droite, de la forme
$$
0 \to G \xrightarrow{\nu} H \xrightarrow{w} E \to 0 ,
$$
et tout $A$-module à gauche $F$, la suite
$$
0 \longrightarrow G \otimes_A F \xrightarrow{\nu \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
est exacte.
(i) $\Rightarrow$ (ii) : c’est le cor. à la prop. 5 de X, p. 69.
(ii) $\Rightarrow$ (iii) : c’est trivial.
(iii) $\Leftrightarrow$ (iv) : tout $A$-module à gauche monogène de présentation finie est isomorphe à un quotient $A/a$, où $a$ est un idéal à gauche de type fini, de sorte que (iii) équivaut à (iv) d’après X, p. 72, exemple.
(iii) $\Rightarrow$ (i) : d’après X, p. 8, prop. 3, X, p. 72, th. 1, $E$ est plat dès que $\operatorname{Tor}_1^A(E, F) = 0$ pour tout $A$-module à gauche $F$. Si (iii) est satisfait, il en est ainsi dès que $F$ est monogène et de présentation finie. D’après X, p. 11, prop. 7, tout $A$-module (resp. tout $A$-module monogène) est limite inductive filtrante de modules de présentation finie (resp. de modules monogènes de présentation finie); on voit donc, d’après X, p. 70, prop. 8, qu’il suffit de prouver que si $\operatorname{Tor}_1^A(E, F) = 0$ lorsque $F$ est monogène, alors il en est ainsi dès que $F$ est de type fini. Raisonnons donc par récurrence sur le cardinal d’un système générateur $(f_1, \ldots, f_n)$ de $F$; la suite exacte
$$
0 \to Af_1 \to F \to F/Af_1 \to 0
$$
donne naissance à une suite exacte
$$
\operatorname{Tor}_1^A(E, Af_1) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E, F/Af_1) ,
$$
de sorte que $\operatorname{Tor}_1^A(E, F) = 0$ puisque $\operatorname{Tor}_1^A(E, Af_1) = 0$ et que $\operatorname{Tor}_1^A(E, F/Af_1) = 0$ par hypothèse de récurrence.
(i) $\Rightarrow$ (v) : c’est le cor. 2 au th. 1 (X, p. 72).
(v) $\Rightarrow$ (iii) : la suite exacte (X, p. 50)
$$
0 \longrightarrow Z_0(E) \xrightarrow{i_E} L_0(E) \xrightarrow{p_E} E \longrightarrow 0
$$
donne naissance pour tout $A$-module à gauche $F$ à une suite exacte
$$
0 \longrightarrow \operatorname{Tor}_1^A(E, F) \longrightarrow Z_0(E) \otimes_A F \xrightarrow{i_E \otimes 1} L_0(E) \otimes_A F \xrightarrow{p_E \otimes 1} E \otimes_A F \longrightarrow 0 .
$$
Si (v) est satisfait, on a $\operatorname{Tor}_1^A(E, F) = 0$ d’où (iii).

#### Corollaire 1 {#alg-x-s4-thm-2-cor-1 .statement}

Soit $0 \to E' \to E \to E'' \to 0$ une suite exacte de $A$-modules à droite. Supposons que $E''$ soit plat. Alors pour que $E$ soit plat, il faut et il suffit que $E'$ soit plat.

Soit F un A-module à gauche. Puisque $\operatorname{Tor}^A_i(E'', F)=0$ pour $i=1,2$ (th. 2, (i) $\Rightarrow$ (ii)), on a une suite exacte

$$
0\longrightarrow \operatorname{Tor}^A_1(E',F)\longrightarrow \operatorname{Tor}^A_1(E,F)\longrightarrow 0
$$

d’où l’assertion (th. 2, (i) $\Leftrightarrow$ (iii)).

**COROLLAIRE 2. —** *Soit $0\longrightarrow E_n\longrightarrow E_{n-1}\longrightarrow\cdots\longrightarrow E_1\longrightarrow0$ une suite exacte de A-modules à droite. Si $E_i$ est plat pour $i=1,\ldots,n-1$, alors $E_n$ est plat.*

### 7.  **Formule de Künneth**

Dans ce numéro, on considère un complexe $(C,d)$ de A-modules à droite et un complexe $(C',d')$ de A-modules à gauche. Considérons les suites exactes canoniques

(I)

$$
0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\delta}B(C)(-1)\longrightarrow0,
$$

(II)

$$
0\longrightarrow B(C)\xrightarrow{i}Z(C)\xrightarrow{p}H(C)\longrightarrow0;
$$

on déduit de $\delta$ un $k$-homomorphisme

$$
H(\delta\otimes 1):H(C\otimes_A C')\longrightarrow H(B(C)\otimes_A C')(-1);
$$

on déduit de (II) un homomorphisme de liaison

$$
\partial(\mathrm{II},H(C')):\operatorname{Tor}^A_1(H(C),H(C'))\longrightarrow B(C)\otimes_A H(C');
$$

si l’on munit $\operatorname{Tor}^A_1(H(C),H(C'))$ de la graduation dont le composant homogène de degré $n$ est

$$
\bigoplus_{p+q=n}\operatorname{Tor}^A_1(H_p(C),H_q(C')),
$$

cet homomorphisme de liaison est gradué de degré 0. On dispose par ailleurs d’un homomorphisme canonique (X, p. 62)

$$
\gamma(B(C),C'):B(C)\otimes_A H(C')\longrightarrow H(B(C)\otimes_A C').
$$

Avec ces notations :

**THÉORÈME 3. —** *Supposons les A-modules $B(C)$ et $Z(C)$ plats. Il existe un unique homomorphisme de $k$-modules gradués, de degré $-1$,*

$$
\alpha:H(C\otimes_A C')\longrightarrow\operatorname{Tor}^A_1(H(C),H(C'))
$$

*rendant commutatif le diagramme*

$$
\begin{array}{ccc}
H(C\otimes_A C') & \xrightarrow{\alpha} & \operatorname{Tor}^A_1(H(C),H(C'))(-1)\\
{\scriptstyle H(\delta\otimes1)}\downarrow & & \downarrow{\scriptstyle\partial(\mathrm{II},H(C'))}\\
H(B(C)\otimes_A C')(-1) & \xleftarrow{\gamma(B(C),C')} & (B(C)\otimes_A H(C'))(-1).
\end{array}
$$

La suite de k-modules gradués

$$
0 \longrightarrow \mathrm{H}(C) \otimes_A \mathrm{H}(C') \xrightarrow{\gamma(C,C')} \mathrm{H}(C \otimes_A C') \xrightarrow{\alpha} \mathrm{Tor}_1^A(\mathrm{H}(C), \mathrm{H}(C'))(-1) \longrightarrow 0
$$

est exacte.

On a donc pour chaque $n$ une suite exacte

(11)
$$
\begin{array}{cccccc}
0 & \longrightarrow & \bigoplus_{p+q=n} \mathrm{H}_p(C) \otimes_A \mathrm{H}_q(C') & \xrightarrow{\gamma_n(C,C')} & \mathrm{H}_n(C \otimes_A C') \\
& & & \xrightarrow{\alpha_n} & \bigoplus_{p+q=n-1} \mathrm{Tor}_1^A(\mathrm{H}_p(C), \mathrm{H}_q(C')) & \longrightarrow 0 .
\end{array}
$$

Posons pour simplifier $B = B(C)$, $Z = Z(C)$, $H = H(C)$ et $H' = H(C')$ :

Comme $B$ est plat, on déduit de (I) une suite exacte (X, p. 72, cor. 2)

(12)
$$
0 \longrightarrow Z \otimes_A C' \xrightarrow{j \otimes 1} C \otimes_A C' \xrightarrow{\delta \otimes 1} (B \otimes_A C')(-1) \longrightarrow 0 .
$$

#### Lemme 3 {#alg-x-s4-lem-3 .statement}

L’homomorphisme de liaison $\mathrm{H}(B \otimes_A C') \to \mathrm{H}(Z \otimes_A C')$ associé à la suite exacte (12) est égal à $\mathrm{H}(i \otimes 1)$.

En effet, soit $a \in Z(B \otimes_A C')$; comme $B$ est plat, $a$ appartient à l’image de $B \otimes_A Z(C')$, donc s’écrit $\sum_\lambda da_\lambda \otimes b_\lambda$, avec $a_\lambda \in C$, $b_\lambda \in C'$, $db_\lambda = 0$. L’image de la classe de $a$ par l’homomorphisme cherché est par définition la classe de $D(\sum a_\lambda \otimes b_\lambda) = \sum da_\lambda \otimes b_\lambda = (i \otimes 1)(a)$, d’où le lemme.

La suite exacte d’homologie associée à (12) est donc

$$
\mathrm{H}(B \otimes_A C') \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C') \xrightarrow{\mathrm{H}(j \otimes 1)} \mathrm{H}(C \otimes_A C')
$$
$$
\xrightarrow{\mathrm{H}(\delta \otimes 1)} \mathrm{H}(B \otimes_A C')(-1) \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C')(-1) .
$$

Par ailleurs, puisque $Z$ est plat, on tire de (II) une suite exacte de $k$-modules gradués

$$
0 \longrightarrow \mathrm{Tor}_1^A(H, H') \xrightarrow{\partial(\mathrm{II}, H')} B \otimes_A H' \xrightarrow{i \otimes 1} Z \otimes_A H' \xrightarrow{p \otimes 1} H \otimes_A H' \longrightarrow 0 ;
$$

enfin, on dispose des homomorphismes canoniques du n° 1

$$
\gamma_B = \gamma(B, C') : B \otimes_A H' \to \mathrm{H}(B \otimes_A C')
$$
$$
\gamma_Z = \gamma(Z, C') : Z \otimes_A H' \to \mathrm{H}(Z \otimes_A C')
$$
$$
\gamma_C = \gamma(C, C') : H \otimes_A H' \to \mathrm{H}(C \otimes_A C') ,
$$

d’où un diagramme de $k$-modules gradués, à *lignes exactes*

$$
\begin{array}{ccccccccc}
B \otimes H' & \xrightarrow{i \otimes 1} & Z \otimes H' & \xrightarrow{p \otimes 1} & H \otimes H' & \longrightarrow & 0 \\
\downarrow \gamma_B & & \downarrow \gamma_Z & & \downarrow \gamma_C & & \\
H(B \otimes C') & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C') & \xrightarrow{H(j \otimes 1)} & H(C \otimes C') & \xrightarrow{H(\delta \otimes 1)} & H(B \otimes C')(-1) & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C')(-1)
\end{array}
$$

$$
0 \longrightarrow \operatorname{Tor}_1^A(H, H')(-1) \xrightarrow{\partial(\Pi, H')} (B \otimes H')(-1) \xrightarrow{i \otimes 1} (Z \otimes H')(-1),
$$

qui est *commutatif* par définition des homomorphismes $\gamma$. Mais, les complexes $B$ et $Z$ étant scindés et plats, $\gamma_B$ et $\gamma_Z$ sont *bijectifs* (X, p. 65, cor. 1). On en déduit, d’une part que $\gamma_C$ est injectif et d’image égale à $\operatorname{Ker} H(\delta \otimes 1)$, d’autre part que $\gamma_B \circ \partial(\Pi, H')$ est injectif, d’image égale à $\operatorname{Im} H(\delta \otimes 1)$. Le théorème résulte immédiatement de là.

#### Corollaire 1 {#alg-x-s4-lem-3-cor-1 .statement}

*Si $B(C)$ et $Z(C)$ sont plats, on a pour tout $A$-module à gauche $N$ et tout entier $n$ une suite exacte*

(13) $$ 0 \longrightarrow H_n(C) \otimes_A N \xrightarrow{\gamma_n} H_n(C \otimes_A N) \xrightarrow{\alpha_n} \operatorname{Tor}_1^A(H_{n-1}(C), N) \longrightarrow 0 . $$

#### Corollaire 2 {#alg-x-s4-lem-3-cor-2 .statement}

*Supposons $B(C)$ et $B(C')$ projectifs et $Z(C)$ plat. Alors les suites de $k$-modules (11) et (13) sont exactes et scindées.*
Cela résulte du théorème et du lemme suivant :

#### Lemme 4 {#alg-x-s4-lem-4 .statement}

*Si $B(C)$ et $B(C')$ sont projectifs, alors l’homomorphisme canonique*
$$ \gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C') $$
*possède une rétraction $k$-linéaire.*
En effet d’après X, p. 65, *remarque b)*, il existe des homologismes $\varphi : C \to H(C)$ et $\varphi' : C' \to H(C')$ tels que $H(\varphi) = 1_{H(C)}$ et $H(\varphi') = 1_{H(C')}$. Dans le diagramme commutatif

$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
\downarrow H(\varphi) \otimes H(\varphi') & & \downarrow H(\varphi \otimes \varphi') \\
H(C) \otimes_A H(C') & \xrightarrow{\gamma(H(C), H(C'))} & H(C) \otimes_A H(C')
\end{array}
$$

$H(\varphi) \otimes H(\varphi')$ et $\gamma(H(C), H(C'))$ sont l’identité, d’où l’assertion.

**Corollaire 3** (*formule des coefficients universels*). — *Supposons l’anneau $A$ principal. Si les complexes $C$ et $C'$ sont libres, les suites de $A$-modules (11) sont exactes et scindées ; si le complexe $C$ est libre, les suites de $A$-modules (13) sont exactes et scindées pour tout $A$-module $N$.*
En effet, $B(C), Z(C)$ et $B(C')$ sont des sous-modules des modules libres $C, C, C'$, donc sont libres (VII, § 3, cor. 2 au th. 1), et on applique le cor. 2.

#### Corollaire 4 (« formule de Künneth ») {#alg-x-s4-lem-4-cor-4 .statement}

Supposons C borné à droite, C et H(C) plats ; alors l’homomorphisme canonique

$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C')
$$

est bijectif.

D’après le théorème, il suffit de prouver que B(C) et Z(C) sont plats. Or on a des suites exactes

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

d’où, d’après X, p. 75, cor. 1, des implications (B_{n-1}(C) est plat) $\Rightarrow$ (Z_n(C) est plat) $\Rightarrow$ (B_n(C) est plat) ; on conclut en remarquant que B_n(C) = 0 pour n assez petit.

#### Corollaire 5 {#alg-x-s4-lem-4-cor-5 .statement}

Soit u : C \to C' un homologisme de complexes de A-modules à droite, plats et bornés à droite. Pour tout complexe E de A-modules à gauche, le morphisme $u \otimes 1_E : C \otimes_A E \to C' \otimes_A E$ est un homologisme.

En effet, Con (u) est un complexe plat, borné à droite et d’homologie nulle ; on a donc H(Con (u) \otimes_A E) = 0 d’après le cor. 4, donc H(Con (u \otimes 1_E)) = 0 (X, p. 67, lemme 2), et $u \otimes 1_E$ est un homologisme.

### 8. Complexes bornés et plats sur un anneau noethérien

#### Proposition 11 {#alg-x-s4-prop-11 .statement}

Supposons A noethérien à gauche, et soit C un complexe borné et plat de A-modules à gauche tel que H(C) soit un A-module de type fini. Soient a et b deux entiers tels que a \leq b et que H_n(C) = 0 pour n < a, C_n = 0 pour n > b. Il existe un complexe P de A-modules à gauche tel que P_n soit projectif et de type fini pour chaque n, et que P_n = 0 pour n \notin [a, b], et un homologisme u : P \to C. De plus, pour tout complexe E de A-modules à droite, l’homomorphisme

$$
H(1_E \otimes u) : H(E \otimes_A P) \to H(E \otimes_A C) \quad \text{est bijectif}.
$$

D’après X, p. 53, prop. 7, il existe un complexe (L, d) tel que L_n soit libre et de type fini pour chaque n, et nul lorsque n < a, et un homologisme f : L \to C. Soit P le complexe quotient L/L', où L'_n = 0 pour n < b, L'_n = L_n pour n > b, L'_b = B_b(L). Comme C_n = 0 pour n > b, f(L') = 0, donc f se factorise par un morphisme de complexes u : P \to C.

$$
\begin{array}{ccccccccc}
\ldots & \longrightarrow & L_{b+1} & \xrightarrow{d_{b+1}} & L_b & \xrightarrow{d_b} & L_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow & & \downarrow & & \\
& & 0 & \longrightarrow & P_b & \longrightarrow & P_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow^{u_b} & & \downarrow^{u_{b-1}} & & \\
& & 0 & \longrightarrow & C_b & \longrightarrow & C_{b-1} & \longrightarrow & \ldots
\end{array}
$$

Comme $f$ est un homologisme, on a $H(\operatorname{Con}(f))=0$, d’où une suite exacte

$$
\cdots \longrightarrow L_{b+1} \xrightarrow{d_{b+1}} L_b \longrightarrow L_{b-1}\oplus C_b \longrightarrow L_{b-2}\oplus C_{b-1} \longrightarrow \cdots
$$

On a donc une suite exacte

$$
0\longrightarrow P_b\longrightarrow L_{b-1}\oplus C_b\longrightarrow L_{b-2}\oplus C_{b-1}\longrightarrow\cdots.
$$

Cela montre d’une part que le cône de $u$ est d’homologie nulle, donc que $u$ est un homologisme, d’autre part que le module $P_b$ est *plat* (X, p. 76, cor. 2) ; comme $P_b$ est de type fini comme quotient de $L_{b+1}$, il est *projectif* (X, p. 13, cor.). Le couple $(P,u)$ répond donc à la condition exigée. La dernière assertion résulte de X, p. 79, cor. 5.

\* **Exemple.** — Soient A un anneau commutatif noethérien, X un A-schéma propre et plat, $\mathcal F$ un $\mathcal C_X$-module cohérent, plat sur A. Il existe un complexe P borné formé de A-modules projectifs de type fini tel que pour tout A-module M, $H(X,\mathcal F\otimes_A M)$ s’identifie naturellement à $H(P\otimes_A M)$. En effet, soit $\mathcal U$ un recouvrement de X par un nombre fini d’ouverts affines, $\mathcal C(\mathcal U,\mathcal F)$ le complexe de Čech associé. On montre que $H^i(\mathcal C(\mathcal U,\mathcal F))$ est isomorphe au A-module $H^i(X,\mathcal F)$, et que ce dernier est de type fini ; de plus, pour tout A-module M, le complexe $\mathcal C(\mathcal U,\mathcal F)\otimes_A M$ est isomorphe à $\mathcal C(\mathcal U,\mathcal F\otimes_A M)$. En appliquant la prop. 11 au complexe $\mathcal C(\mathcal U,\mathcal F)$ (qui est borné), on obtient un complexe P qui répond à la question.

Pour tout point $y$ de Spec (A), notons $\kappa(y)$ le corps résiduel de A en $y$, $X_y=X\otimes_A\kappa(y)$ la fibre de X au-dessus de $y$, $\mathcal F_y=\mathcal F\otimes_A\kappa(y)$, et posons $h^p(y)=\dim_{\kappa(y)}H^p(X_y,\mathcal F_y)$ pour $p\geq 0$.

On déduit aisément de l’existence du complexe P les résultats suivants :

(i) la fonction $h^p$ est semi-continue supérieurement sur Spec (A) ;

(ii) la fonction $\displaystyle\sum_{p\geq 0}(-1)^p h^p$ est localement constante sur Spec (A). \*

### 9. Généralisation aux complexes de multimodules

Soient B et B′ deux anneaux, C un complexe de (B, A)-bimodules, C′ un complexe de (A, B′)-bimodules (X, p. 43) ; alors $(C\otimes_A C',D)$ (X, p. 61) est un complexe de (B, B′)-bimodules et l’homomorphisme canonique

$$
\gamma:H(C)\otimes_A H(C')\longrightarrow H(C\otimes_A C')
$$

est compatible avec les structures de (B, B′)-bimodules des deux membres.

Si B″ est un troisième anneau, et C″ un complexe de (B′, B″)-bimodules, l’homomorphisme canonique (II, p. 64, prop. 8)

$$
(C\otimes_A C')\otimes_{B'}C''\longrightarrow C\otimes_A(C'\otimes_{B'}C'')
$$

est un isomorphisme de complexes de (B, B″)-bimodules.

Plus généralement, nous laissons au lecteur le soin de développer la théorie des produits tensoriels de familles finies, totalement ordonnées de *complexes de multimodules* sur le modèle du n° 1 (X, p. 63) et de II, pp. 65 à 72 (isomorphismes d’associativité, de commutativité, …).

Soient B et B’ deux anneaux, M un (B, A)-bimodule, N un (A, B’)-bimodule :
alors $L(M)\otimes_A L(N)$ est un complexe de (B, B’)-bimodules, de sorte que $\operatorname{Tor}^A(M,N)$ est muni d’une structure naturelle de (B, B’)-bimodule gradué ; sur le terme de degré 0, cette structure coïncide avec celle de $M\otimes_A N$.

Si $\lambda\in B$, $\lambda'\in B'$, et si on note $\lambda_M,\lambda_N,\lambda_T,\lambda'_T$, les homothéties $x\mapsto\lambda x$, $y\mapsto y\lambda'$, $z\mapsto\lambda z$, $z\mapsto z\lambda'$ de $M$, $N$, $\operatorname{Tor}^A(M,N)$, $\operatorname{Tor}^A(M,N)$ respectivement, alors

$$
\lambda_T=\operatorname{Tor}^A(\lambda_M,1_N),\qquad
\lambda'_T=\operatorname{Tor}^A(1_M,\lambda_N'),
$$

ce qui fournit une autre description de la structure de bimodule de $\operatorname{Tor}^A(M,N)$.
Nous laissons au lecteur le soin de généraliser les nos 5 et 7 au cas des complexes de multimodules.

## EXERCICES {#alg-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
