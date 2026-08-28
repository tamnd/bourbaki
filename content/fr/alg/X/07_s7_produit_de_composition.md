---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 7
section_title: Produit de composition
lang: fr
source: alg-x-fr
book_pages: A X.113-A X.134, A X.197-A X.202
pdf_pages: 0119-0140, 0203-0208
extraction: ocr
subsections:
    - "no": 1
      title: L’homomorphisme $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$
      page: 113
      pdf_page: 119
    - "no": 2
      title: Les sept calculs du produit de composition
      page: 115
      pdf_page: 121
    - "no": 3
      title: La classe associée à une suite exacte
      page: 116
      pdf_page: 122
    - "no": 4
      title: Propriétés de la classe associée à une suite exacte
      page: 118
      pdf_page: 124
    - "no": 5
      title: Relation entre suites exactes et éléments de $\mathrm{Ext}_A(M, N)$
      page: 121
      pdf_page: 127
    - "no": 6
      title: Produit de composition et homomorphismes de liaison des modules d’extensions
      page: 125
      pdf_page: 131
    - "no": 7
      title: L’homomorphisme $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$
      page: 128
      pdf_page: 134
    - "no": 8
      title: Produits de composition et homomorphismes de liaison des produits de torsion
      page: 130
      pdf_page: 136
    - "no": 9
      title: Calcul des produits de composition par décalage de résolutions
      page: 132
      pdf_page: 138
statements: 34
exercises: 11
content_sha256: 8030f2c6ec5b3b69eb251de1fd3bb272ebbe075c7b637f8643776b9f19219334
---

## § 7. PRODUIT DE COMPOSITION

*On reprend les conventions générales du § 4.*

### 1. L’homomorphisme $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$

Soient $M$ et $N$ deux $A$-modules à gauche. Considérons les homologismes $p_M : L(M) \to M, e_M : M \to I(M)$ et $e_M \circ p_M : L(M) \to I(M)$; d’après la prop. 4 de X, p. 86, on en déduit un homomorphisme *bijectif*

$$
a_{M,N} = H(\mathrm{Homgr}_A(e_M \circ p_M, 1)) : H(\mathrm{Homgr}_A(I(M), I(N))) \to \mathrm{Ext}_A(M, N) .
$$

Rappelons d’ailleurs (X, p. 82) que $H^n(\mathrm{Homgr}_A(I(M), I(N)))$ est l’ensemble des classes d’homotopie des morphismes de degré ascendant $n$ du complexe $I(M)$ dans le complexe $I(N)$. Par exemple, si $f \in \mathrm{Hom}_A(M, N)$, la classe d’homotopie de $I(f)$ est envoyée par $a_{M,N}$ sur $f$.

Si P est un troisième A-module à gauche, on a d’après X, p. 99, un k-homomorphisme canonique

$$
H(\mathrm{Homgr}_A(I(N), I(P))) \otimes_k H(\mathrm{Homgr}_A(I(M), I(N))) \to H(\mathrm{Homgr}_A(I(M), I(P)))
$$

dont on déduit par transport par les isomorphismes $a_{N,P}, a_{M,N}, a_{M,P}$ un k-homomorphisme (*homomorphisme de composition*) :

$$
c_{M,N,P}: \mathrm{Ext}_A(N, P) \otimes_k \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

Celui-ci correspond à une *application k-bilinéaire*

(1)

$$
\mathrm{Ext}_A(N, P) \times \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

qui se décompose en composantes homogènes

(2)

$$
\mathrm{Ext}_A^i(N, P) \times \mathrm{Ext}_A^j(M, N) \to \mathrm{Ext}_A^{i+j}(M, P)
$$

Si $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, l’image de $(u, v)$ par (1) s’appelle le *produit de composition de u et v et se note* $u \circ v$. Si $g$ (resp. $f$) est un morphisme de complexes de degré ascendant $j$ (resp. $i$) de $I(M)$ dans $I(N)$ (resp. de $I(N)$ dans $I(P)$), de classe d’homotopie $\bar{g}$ (resp. $\bar{f}$), alors le produit de composition $a_{N,P}(\bar{f}) \circ a_{M,N}(\bar{g})$ est l’image par $a_{M,P}$ de la classe d’homotopie du morphisme $f \circ g$ de $I(M)$ dans $I(P)$.

#### Exemple 1 {#alg-x-s7-n1-exa-1 .statement}

Si $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, $u \circ v$ est le composé de $u$ et de $v$.

#### Exemple 2 {#alg-x-s7-n1-exa-2 .statement}

Si $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, alors

$$
u \circ v = \mathrm{Ext}_A(l_M, u)(v) \in \mathrm{Ext}_A(M, P):
$$

de même, si $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, alors

$$
u \circ v = \mathrm{Ext}_A(v, l_P)(u) \in \mathrm{Ext}_A(M, P).
$$

Cela résulte des définitions et des remarques de X. p. 88.

Si Q, M, N, P sont quatre A-modules à gauche, et si

$$
u \in \mathrm{Ext}_A(N, P), \quad v \in \mathrm{Ext}_A(M, N), \quad w \in \mathrm{Ext}_A(Q, M),
$$

alors $(u \circ v) \circ w = u \circ (v \circ w)$ : le produit de composition est *associatif* ; on notera donc les composés de plusieurs éléments sans parenthèses. En particulier, d’après l’exemple 2 :

#### Exemple 3 {#alg-x-s7-n1-exa-3 .statement}

Soient M, N, M', N' quatre A-modules à gauche. Si $u \in \mathrm{Ext}_A(M, N)$, $f \in \mathrm{Hom}_A(M', M)$, $g \in \mathrm{Hom}_A(N, N')$, alors

(3)

$$
\mathrm{Ext}_A(f, g)(u) = g \circ u \circ f \in \mathrm{Ext}_A(M', N').
$$

Cela donne une nouvelle démonstration de la $k$-bilinéarité de l’application $(f, g) \to \mathrm{Ext}_A(f, g)$ (X, p. 88, prop. 6).

### 2. Les sept calculs du produit de composition

Soient $M$, $M'$ et $M''$ trois $A$-modules à gauche, $a : R \to M$, $a' : R' \to M'$ et $a'' : R'' \to M''$ des résolutions projectives, $c : M \to E$, $c' : M' \to E'$ et $c'' : M'' \to E''$ des résolutions injectives. Il résulte de X, p. 100, th. 1 et p. 103, prop. 2, que le diagramme :

$$
\begin{array}{cccccc}
H(\mathrm{Homgr}_A(M, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, M')) \\
\uparrow & & \downarrow & & \uparrow \\
H(\mathrm{Homgr}_A(E, E')) & \xrightarrow{\varphi(E, E')} & \mathrm{Ext}_A(M, M') & \xleftarrow{\varphi(R, R')} & H(\mathrm{Homgr}_A(R, R')) \\
& \swarrow_{\varphi(M, E')} & & \searrow^{\varphi(R, M')} & \\
& & H(\mathrm{Homgr}_A(R, E')) & &
\end{array}
$$

où les flèches non désignées sont déduites canoniquement de $c, a, c', a'$, est commutatif, et que toutes les flèches sont des isomorphismes, ce qui donne cinq descriptions de $\mathrm{Ext}_A(M, M')$. On obtient de même cinq descriptions de $\mathrm{Ext}_A(M', M'')$, et autant de $\mathrm{Ext}_A(M, M'')$.

Considérons maintenant les sept homomorphismes de composition

$$
H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(\mathrm{Homgr}_A(C, C')) \to H(\mathrm{Homgr}_A(C, C''))
$$

où l’on prend successivement pour $(C, C', C'')$ les sept triplets $(R, R', R''), (R, R', M''), (R, R', E''), (R, M', E''), (R, E', E''), (M, E', E''), (E, E', E'')$.

![Diagramme des sept calculs du produit de composition](https://i.imgur.com/3Q5z5QG.png)

Fig. 1.

Identifiant $H(\mathrm{Homgr}_A(C, C'))$ à $\mathrm{Ext}(M, M')$ par l’isomorphisme ci-dessus, et de même pour $H(\mathrm{Homgr}_A(C', C''))$ et $H(\mathrm{Homgr}_A(C, C''))$, on obtient *sept homomorphismes*

$$
\mathrm{Ext}_A(M', M'') \otimes_k \mathrm{Ext}_A(M, M') \to \mathrm{Ext}_A(M, M'')
$$

Ces sept homomorphismes coïncident, et sont indépendants du choix des résolutions.
En particulier, ils coïncident avec l’homomorphisme qui a été défini au n° 2, via le triplet $(I(M), I(M'), I(M''))$. Cela résulte en effet de l’interprétation des modules H(Homgr $(C, C')$) comme module des classes d’homotopie de morphismes de complexes de C dans C’, et du fait que si dans un diagramme de complexes

$$
\begin{array}{ccccc}
C & \xrightarrow{\ f\ } & C' & \xrightarrow{\ g\ } & C''\\
\downarrow\scriptstyle{\alpha} & & \downarrow\scriptstyle{\alpha'} & & \downarrow\scriptstyle{\alpha''}\\
C_1 & \xrightarrow{\ f_1\ } & C'_1 & \xrightarrow{\ g_1\ } & C''_1
\end{array}
$$

$\alpha'' \circ g$ est homotope à $g_1 \circ \alpha'$ et $\alpha' \circ f$ homotope à $f_1 \circ \alpha$, alors $\alpha'' \circ g \circ f$ est homotope à $g_1 \circ f_1 \circ \alpha$ (X, p. 33, prop. 4 et cor.).

Dans ce qui suit, nous utiliserons suivant le cas l’une ou l’autre des sept constructions précédentes des homomorphismes de composition.

### 3. La classe associée à une suite exacte

#### Proposition 1 {#alg-x-s7-prop-1 .statement}

Soient $(C,d)$ et $(C',d')$ deux complexes de $A$-modules à gauche et $n,p,q$ trois entiers tels que $p \geq q$. Pour $p \geq i \geq q-1$, soit $f_i:C_i\longrightarrow C'_{i+n+1}$ un homomorphisme de $A$-modules tel que $f_p\circ d=0$, $f_i\circ d=d'\circ f_{i+1}$ pour $p>i\geq q-1$, et $d'\circ f_{q-1}=0$ (voir fig. 2).

$$
\begin{array}{ccccccccccccc}
C_{p+1}&\xrightarrow{\ d\ }&C_p&\xrightarrow{\ d\ }&C_{p-1}&\xrightarrow{\ d\ }&\cdots&\xrightarrow{\ d\ }&C_q&\xrightarrow{\ d\ }&C_{q-1}&\xrightarrow{\ d\ }&C_{q-2}\\
0\downarrow&&\downarrow f_p&&\downarrow f_{p-1}&&&&\downarrow f_q&&\downarrow f_{q-1}&&\downarrow 0\\
C'_{p+n+2}&\xrightarrow{\ d'\ }&C'_{p+n+1}&\xrightarrow{\ d'\ }&C'_{p+n}&\xrightarrow{\ d'\ }&\cdots&\xrightarrow{\ d'\ }&C'_{q+n+1}&\xrightarrow{\ d'\ }&C'_{q+n}&\xrightarrow{\ d'\ }&C'_{q+n-1}
\end{array}
$$

Fig. 2.

Posons $\alpha=f_{p-1}\circ d=d'\circ f_p$, $\beta=f_{q-1}\circ d=d'\circ f_q$, et soit $a$ (resp. $b$) le $A$-homomorphisme gradué de degré $n$ de $C$ dans $C'$ dont la seule composante bi-homogène non nulle est $\alpha$ (resp. $\beta$). Alors on a $a\in Z_n(\operatorname{Homgr}_A(C,C'))$, $b\in Z_n(\operatorname{Homgr}_A(C,C'))$ et

$$
a-(-1)^{(n+1)(p-q)}b\in B_n(\operatorname{Homgr}_A(C,C')).
$$

On a $d'\circ\alpha=d'\circ f_{p-1}\circ d=0$, $\alpha\circ d=f_{p-1}\circ d\circ d=0$, donc

$$
a\in Z_n(\operatorname{Homgr}_A(C,C')) ;
$$

de même $b\in Z_n(\operatorname{Homgr}_A(C,C'))$. Posons $\varepsilon=(-1)^{n+1}$. On a, dans le complexe $\operatorname{Homgr}_A(C,C')$ les relations

$$
Df_{p-1}=d'\circ f_{p-1}-\varepsilon f_{p-1}\circ d=f_{p-2}\circ d-\varepsilon\alpha
$$

$$
Df_i=d'\circ f_i-\varepsilon f_i\circ d=f_{i-1}\circ d-\varepsilon f_{i+1}\circ d\qquad (p-1>i>q)
$$

$$
Df_q=d'\circ f_q-\varepsilon f_q\circ d=\beta-\varepsilon f_q\circ d .
$$

donc

$$
\sum_{i=1}^{p-q} \varepsilon^i Df_{p-i} = \varepsilon^{p-q} \beta - \alpha,
$$

ce qui démontre le lemme.

Considérons deux A-modules à gauche M et N et une suite exacte de A-modules

(4)
$$
0 \to N \to R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0.
$$

D’après les prop. 3 et 3 bis de X, p. 49, il existe un diagramme commutatif :

(5)

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots & \longrightarrow & I^{n-1}(N) & \xrightarrow{\delta^{n-1}} & I^n(N) & \xrightarrow{\delta^n} & I^{n+1}(N) \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
L_{n+1}(M) & \xrightarrow{d_{n+1}} & L_n(M) & \xrightarrow{d_n} & L_{n-1}(M) & \longrightarrow & \ldots & \xrightarrow{d_1} & L_0(M) & \xrightarrow{p_M} & M & \longrightarrow & 0.
\end{array}
$$

Considérons les deux éléments $b$ et $a$ de $\mathrm{Homgr}_A(L(M), I(N))$ dont les seules composantes bihomogènes non nulles sont

$$
b^n = e_N \circ u_n : L_n(M) \to I^0(N) \quad \text{et} \quad a^n = v^n \circ p_M : L_0(M) \to I^n(N)
$$

respectivement.

#### Proposition 2 {#alg-x-s7-prop-2 .statement}

*On a* $a, b \in Z^n(\mathrm{Homgr}_A(L(M), I(N)))$. *De plus*, les classes $\overline{a}$ et $\overline{b}$ de $a$ et $b$ dans $H^n(\mathrm{Homgr}_A(L(M), I(N))) = \mathrm{Ext}_A^n(M, N)$ ne dépendent que de la suite exacte (4) et sont égales.

D’après la prop. 1, appliquée aux deux lignes extrêmes de (5) et aux flèches verticales composées, avec $p = n, q = 0$, on a $a, b \in Z^n(\mathrm{Homgr}_A(I(M), L(N)))$ et

$$
a - b = a - (-1)^{(n+1)n} b \in B^n(\mathrm{Homgr}_A(L(M), I(N))) .
$$

Puisque $a$ (resp. $b$) est indépendant du choix de $u$ (resp. $v$), l’élément $\overline{a} = \overline{b}$ de $\mathrm{Ext}_A^n(M, N)$ est indépendant du choix des morphismes $u$ et $v$, d’où la proposition.

#### Définition 1 {#alg-x-s7-def-1 .statement}

*On appelle classe associée à la suite exacte* (4) *l’élément* $\theta$ *de* $\mathrm{Ext}_A^n(M, N)$ *défini par* $\theta = (-1)^{n(n+1)/2} \overline{a} = (-1)^{n(n+1)/2} \overline{b}$.

#### Remarque 1 {#alg-x-s7-n3-rem-1 .statement}

Soit (P, p) une résolution projective de M. D’après X, p. 49. prop. 3, il existe un diagramme commutatif

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
P_n & \longrightarrow & P_{n-1} & \longrightarrow & \ldots & \longrightarrow & P_0 & \xrightarrow{p} & M & \longrightarrow & 0.
\end{array}
$$

Avec les notations du § 6, θ est l’image par φ(P, N) de la classe d’homotopie du morphisme P → N défini par (−1)^{n(n+1)/2} \tilde{u}_n. De même si (e, E) est une résolution injective de N, il existe un diagramme commutatif

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \longrightarrow & E^0 & \longrightarrow & \ldots \longrightarrow & E^{n-1} & \longrightarrow & E^n \\
& & ^{1_N}\uparrow & & ^{\tilde{v}^0}\uparrow & & & ^{\tilde{v}^{n-1}}\uparrow & & ^{\tilde{v}^n}\uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

et θ est l’image par φ(M, E) de la classe d’homotopie du morphisme M → E défini par (−1)^{n(n+1)/2} v^n. Ceci résulte de la construction de θ et des définitions de φ(P, N) et φ(M, E).

#### Remarque 2 {#alg-x-s7-n3-rem-2 .statement}

Lorsque $n = 0$, la suite exacte (4) s’écrit $0 \to N \xrightarrow{f} M \to 0$, et la classe associée est $f^{-1} \in \mathrm{Hom}_A(M, N) = \mathrm{Ext}^0_A(M, N)$.

### 4. Propriétés de la classe associée à une suite exacte

#### Proposition 3 {#alg-x-s7-prop-3 .statement}

Soient

(6)
$$
0 \to P \to S_m \to S_{m-1} \to \ldots \to S_1 \xrightarrow{\lambda} N \to 0
$$
(7)
$$
0 \to N \twoheadrightarrow R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0
$$
deux suites exactes de A-modules à gauche de classes respectives θ ∈ Ext^m_A(N, P) et θ' ∈ Ext^n_A(M, N). La classe dans Ext^{m+n}_A(M, P) associée à la suite exacte
(8)
$$
0 \to P \to S_m \to \ldots \to S_1 \xrightarrow{\mu \circ \lambda} R_n \to \ldots \to R_1 \to M \to 0
$$
est le produit de composition θ ∘ θ'.

Choisissons des diagrammes commutatifs

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & P & \longrightarrow & I^0(P) & \longrightarrow & \ldots \longrightarrow & I^{m-1}(P) & \xrightarrow{\delta_P^{m-1}} & I^m(P) \\
& & ^{l_P}\uparrow & & ^{w^0}\uparrow & & & ^{w^{m-1}}\uparrow & & ^{w^m}\uparrow \\
0 & \longrightarrow & P & \longrightarrow & S_m & \longrightarrow & \ldots \longrightarrow & S_1 & \xrightarrow{\lambda} & N & \longrightarrow & 0 ,
\end{array}
$$
$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots \longrightarrow & I^{n-1}(N) & \longrightarrow & I^n(N) \\
& & ^{1_N}\uparrow & & ^{v^0}\uparrow & & & ^{v^{n-1}}\uparrow & & ^{v^n}\uparrow \\
0 & \longrightarrow & N & \xrightarrow{\mu} & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

Puisque I^m(P) est injectif, il existe un homomorphisme h^0 : I^0(N) → I^m(P) tel que w^m = h^0 ∘ e_N ; d’après X, p. 49, prop. 3 bis, h^0 se prolonge en un morphisme de complexes h : I(N) → I(P) (− m). Alors w^m = h^0 ∘ e_N = h^0 ∘ v^0 ∘ μ, donc
$$
\delta_I^{m-1} \circ w^{m-1} = w^m \circ \lambda = h^0 \circ v^0 \circ (\mu \circ \lambda),
$$

et le diagramme suivant est commutatif :

$$
\begin{array}{ccccccccccccccccccc}
0&\longrightarrow&P&\longrightarrow&I^0(P)&\longrightarrow&\cdots&\longrightarrow&I^{m-1}(P)&\longrightarrow&I^m(P)&\longrightarrow&I^{m+1}(P)&\longrightarrow&\cdots&\longrightarrow&I^{m+n}(P)\\
&&\uparrow^{i_P}&&\uparrow^{w^0}&&&&\uparrow^{w^{m-1}}&&\uparrow^{t^0}&&\uparrow^{t^1}&&&&\uparrow^{t^n}\\
0&\longrightarrow&P&\longrightarrow&S_m&\longrightarrow&\cdots&\longrightarrow&S_1&\xrightarrow[\mu\circ\lambda]{}&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&M&\longrightarrow&0
\end{array}
$$

où $t^0=h^0\circ v^0$, $t^1=(-1)^m h^1\circ v^1$, $\ldots$, $t^i=(-1)^{mi}h^i\circ v^i$, $\ldots$, $t^n=(-1)^{mn}h^n\circ v^n$.

La classe $\theta$ associée à (6) est celle de $(-1)^{m(m+1)/2}w^m\in\operatorname{Homgr}_A^m(N,I(P))$, donc correspond par l’isomorphisme $\alpha_{N,P}$ à la classe de $(-1)^{m(m+1)/2}h\in\operatorname{Homgr}_A^m(I(N),I(P))$; la classe $\theta'$ associée à (7) est celle de $(-1)^{n(n+1)/2}v^n\in\operatorname{Homgr}^n(M,I(N))$, la classe associée à (8) est celle de $(-1)^{(m+n)(m+n+1)/2}t^n\in\operatorname{Homgr}^{m+n}(M,I(P))$, d’où la conclusion, d’après la définition du produit de composition (X, p. 114) et la formule

$$
m(m+1)/2+n(n+1)/2=(m+n)(m+n+1)/2-mn.
$$

4. — Considérons un diagramme commutatif de $A$-modules à lignes exactes

$$
\begin{array}{ccccccccccccccc}
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{f}&&\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&R'_{n-1}&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0.
\end{array}
$$

Soit $\theta$ (resp. $\theta'$) la classe de la première (resp. seconde) ligne dans

$$
\operatorname{Ext}_A^n(M,N)\quad\text{(resp. }\operatorname{Ext}_A^n(M',N')\text{)}.
$$

Dans $\operatorname{Ext}_A^n(M,N')$, on a $\theta'\circ f=g\circ\theta$.

Considérons en effet un diagramme commutatif

$$
\begin{array}{ccccccccccccc}
L_n(M)&\xrightarrow{d_n}&L_{n-1}(M)&\longrightarrow&\cdots&\longrightarrow&L_0(M)&\xrightarrow{p_M}&M&\longrightarrow&0\\
\downarrow^{u_n}&&\downarrow&&&&\downarrow&&\downarrow^{1}\\
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&&&\downarrow&&\downarrow^{f}\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0\\
&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{v^n}\\
0&\longrightarrow&N'&\xrightarrow{\epsilon_{N'}}&I^0(N')&\xrightarrow{\delta^0}&\cdots&\longrightarrow&I^{n-1}(N')&\xrightarrow{\delta^{n-1}}&I^n(N')
\end{array}
$$

Par définition $\theta'\circ f$ est la classe de $(-1)^{n(n+1)/2}v^n\circ f\circ p_M\in\operatorname{Homgr}^n(L(M),I(N'))$, tandis que $g\circ\theta$ est la classe de $(-1)^{n(n+1)/2}\epsilon_{N'}\circ g\circ u_n$. D’après le lemme 1, appliqué aux deux lignes extrêmes du diagramme, ces deux classes sont égales.

#### Corollaire 1 {#alg-x-s7-prop-3-cor-1 .statement}

Considérons un diagramme commutatif à lignes exactes

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \cdots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
\downarrow & & \downarrow & & \downarrow & & & \downarrow & & \downarrow & & \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \cdots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 ;
\end{array}
$$

les deux lignes du diagramme ont même classe associée dans $\mathrm{Ext}_A^n(M, N)$.

#### Corollaire 2 {#alg-x-s7-prop-3-cor-2 .statement}

Soient

$$
0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} R_{n-1} \to \cdots \xrightarrow{f_2} R_1 \xrightarrow{f_1} M \to 0
$$

une suite exacte, $\theta \in \mathrm{Ext}_A^n(M, N)$ la classe associée, $a_1, \ldots, a_{n+1}$ des éléments invisibles de $k$. La classe associée à la suite exacte

$$
0 \to N \xrightarrow{a_{n+1} f_{n+1}} R_n \xrightarrow{a_n f_n} R_{n-1} \to \cdots \xrightarrow{a_2 f_2} R_1 \xrightarrow{a_1 f_1} M \to 0
$$

est $(a_1^{-1}\ a_2^{-1}\ \ldots\ a_{n+1}^{-1})\ \theta$.

En effet, on a un diagramme commutatif

$$
\begin{array}{ccccccccccccccc}
0 & \rightarrow & N & \xrightarrow{a_{n+1} f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{a_2 f_2} & R_1 & \xrightarrow{a_1 f_1} & M & \rightarrow & 0 \\
& & \downarrow a_1 \ldots a_{n+1} & & \downarrow a_1 \ldots a_n & & & \downarrow a_1 a_2 & & \downarrow a_1 & & \downarrow 1 \\
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{f_2} & R_1 & \xrightarrow{f_1} & M & \rightarrow & 0 .
\end{array}
$$

et on applique la proposition.

#### Corollaire 3 {#alg-x-s7-prop-3-cor-3 .statement}

Soient $0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} \cdots \to R_1 \xrightarrow{f_1} M \to 0$ une suite exacte, $\theta$ sa classe dans $\mathrm{Ext}_A^n(M, N)$, $u : M' \to M$ et $v : N \to N'$ deux homomorphismes de $A$-modules.

a) L’élément $v \circ \theta$ de $\mathrm{Ext}_A^n(M, N')$ est égal à la classe de la suite exacte

$$
0 \to N' \xrightarrow{f_{n'+1}} R'_n \xrightarrow{f_{n'}} R_{n-1} \xrightarrow{f_{n-1}} \cdots \to R_1 \to M \to 0 ,
$$

où $R'_n$ est le $A$-module quotient de $R_n \oplus N'$ par le sous-module formé des couples $(f_{n+1}(x), -v(x))$ pour $x \in N$, et où $f_{n'+1}'$ (resp. $f_{n'}'$) est déduit de l’injection canonique (resp. de $(f_n, 0)$) par passage aux quotients.

b) L’élément $\theta \circ u$ de $\mathrm{Ext}_A^n(M', N)$ est la classe de la suite exacte

$$
0 \to N \to R_n \to \cdots \to R_2 \xrightarrow{f_2''} R'_1 \xrightarrow{f_1''} M' \to 0 ,
$$

où $R'_1$ est le produit fibré $R_1 \times_M M'$, c’est-à-dire (I, p. 44) le sous-module de $R_1 \times M'$ formé des couples $(x, y)$ tels que $f_1(x) = u(y)$, et où $f_2''$ (resp. $f_1''$) est déduit de $(f_2, 0)$ (resp. de la seconde projection).

Démontrons par exemple $a$. Soit $z$ un élément de $R'_n$ tel que $f'_n(z) = 0$; si $z$ est la classe d’un couple $(x, y)$, avec $x \in R_n$, $y \in N'$, on a $f_n(x) = 0$, de sorte qu’il existe un élément $t \in N$ tel que $x = f_{n+1}(t)$. On a alors $z = f'_{n+1}(y + v(t))$, ce qui prouve que $\mathrm{Ker}\ f'_n = \mathrm{Im}\ f'_{n+1}$. L’injectivité de $f'_{n+1}$ résulte de celle de $f_{n+1}$.

Soit $j : R_n \to R'_n$ l’homomorphisme déduit de l’injection canonique; on a un diagramme commutatif de suites exactes :

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \xrightarrow{f_n} & R_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow v & & \downarrow j & & \downarrow 1 & & & & \downarrow 1 & & \\
0 & \longrightarrow & N' & \xrightarrow{f'_{n+1}} & R'_n & \xrightarrow{f'_n} & R'_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 ;
\end{array}
$$

l’assertion $a$ résulte alors de la proposition.

La démonstration de $b$ est analogue.

#### Remarque {#alg-x-s7-n4-rem-1 .statement}

Soit $\theta \in \mathrm{Ext}^n_A(M, N)$, resp. $\theta' \in \mathrm{Ext}^n_A(M', N')$, la classe d’une suite exacte

$$
0 \to N \xrightarrow{f_{n+1}} R_n \to \ldots \to R_1 \xrightarrow{f_1} M \to 0,
$$
resp. $0 \to N' \xrightarrow{f'_{n+1}} R'_n \to \ldots \to R'_1 \xrightarrow{f'_1} M' \to 0.$

Soient $i_N,\ i_{N'}$, les injections canoniques de $N$ et $N'$ dans $N \oplus N'$, $q_M,\ q_{M'}$, les projections de $M \oplus M'$ sur $M$ et $M'$. Considérons l’homomorphisme

$$
m = \mathrm{Ext}\,(q_M,\ i_N) \oplus \mathrm{Ext}\,(q_{M'},\ i_{N'})
$$

de $\mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M', N')$ dans $\mathrm{Ext}_A(M \oplus M', N \oplus N')$. *L’élément*

$$
m(\theta, \theta') = i_N \circ \theta \circ q_M + i_{N'} \circ \theta' \circ q_{M'}
$$

*est la classe de la suite exacte*

$$
0 \to N \oplus N' \xrightarrow{f_{n-1} \oplus f'_{n-1}} R_n \oplus R'_n \to \ldots \to R_1 \oplus R'_1 \xrightarrow{f_1 \oplus f'_1} M \oplus M' \to 0 .
$$

En effet, si l’on désigne cette classe par $\theta''$, il résulte de la prop. 4 qu’on a

$$
\theta'' \circ i_M = i_N \circ \theta = m(\theta, \theta') \circ i_M \quad \text{et} \quad \theta'' \circ i_{M'} = i_{N'} \circ \theta = m(\theta, \theta') \circ i_{M'} ;
$$

d’après X, p. 89, prop. 7, cela entraîne $\theta'' = m(\theta, \theta')$.

### 5. Relation entre suites exactes et éléments de $\mathrm{Ext}_A(M, N)$

#### Théorème 1 {#alg-x-s7-thm-1 .statement}

*Soient $n$ un entier $\geqslant 1$, $M$ et $N$ deux $A$-modules.*

a) *Tout élément de $\mathrm{Ext}^n_A(M, N)$ est la classe d’une suite exacte* (X, p. 117, déf. 1).

b) *Soient* $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \xrightarrow{f_1} M \to 0$ et $0 \to N \xrightarrow{f_{n+1}} R'_n \xrightarrow{f_n} \ldots \to R'_1 \xrightarrow{f_1} M \to 0$

des suites exactes, $\theta$ et $\theta'$ les classes associées. Les conditions suivantes sont équivalentes :

(i) $\theta = \theta'$;

(ii) il existe un diagramme commutatif à lignes exactes :

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 ;
\end{array}
$$

(iii) il existe un diagramme commutatif à lignes exactes :

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 .
\end{array}
$$

Démontrons $a$. Soit $\alpha \in \mathrm{Ext}_A^n(M, N)$, et soit $P$ une résolution projective de $M$. Soit $a : P(n) \to N$ un morphisme de complexes représentant $\alpha$; son unique composante non nulle est un $A$-homomorphisme $u : P_n \to N$ qui vérifie $u \circ d_{n+1} = 0$, donc se factorise en $u = \overline{u} \circ \delta_n$, où $\delta_n : P_n \to Z_{n-1}$ est l’application induite par $d_n$ (on pose $Z_{n-1} = \mathrm{Im}\, d_n$) et $\overline{u}$ est un $A$-homomorphisme de $Z_{n-1}$ dans $N$. D’après la remarque 1, p. 117, la classe $\theta \in \mathrm{Ext}_A^n(M, Z_{n-1})$ de la suite exacte

$$
0 \to Z_{n-1} \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

est égale à la classe d’homotopie du morphisme $(-1)^{n(n+1)/2} \delta_n$. On a donc

$$
\alpha = (-1)^{n(n+1)/2} \overline{u} \circ \theta ,
$$

ce qui permet d’après le cor. 3, p. 120 de représenter $\alpha$ comme la classe d’une suite exacte.

Démontrons $b$. Il résulte du cor. 1 de X, p. 120 que (ii) $\Rightarrow$ (i) et que (iii) $\Rightarrow$ (i). Supposons (i) satisfaite, et soit $P$ une résolution projective de $M$. Il existe un diagramme commutatif

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & u_n \uparrow & & u_{n-1} \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
& & P_n & \xrightarrow{d_n} & P_{n-1} & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & u'_n \downarrow & & u'_{n-1} \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 .
\end{array}
$$

Les morphismes de $P(n)$ dans $N$ définis par $u_n$ et $u'_n$ sont homotopes, car ils appartiennent tous deux à la classe $(-1)^{n(n+1)/2} \theta$, donc $u'_n - u_n$ est de la forme $w \circ d_n$, où $w : P_{n-1} \to N$ est un A-homomorphisme. En remplaçant $u'_{n-1}$ par $u'_{n-1} - f'_{n+1} \circ w$ et $u'_n$ par $u_n$, on se ramène au cas où $u_n = u'_n$. Ceci permet de construire un nouveau diagramme commutatif à lignes exactes :

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & v \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & N' & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v' \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

où $N'$ est le quotient de $P_{n-1} \oplus N$ par le sous-module formé des couples $(d_n(x), -u_n(x))$ pour $x \in P_n$, et où $v$ (resp. $v'$) est défini par passage au quotient à partir de l’application $u_{n-1} \oplus f_{n+1}$ (resp. $u'_{n-1} \oplus f'_{n+1}$). La condition (ii) est donc satisfaite.

Supposons de nouveau la condition (i) satisfaite, et soit E une résolution injective de N. Il existe un diagramme commutatif

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v_0 \downarrow & & & & & & & \\
0 & \rightarrow & N' & \rightarrow & E^0 & \xrightarrow{\delta^0} & \ldots \rightarrow & E^{n-1} & \xrightarrow{\delta^{n-1}} & E^n \\
& & 1_N \uparrow & & v'_0 \uparrow & & & & & & \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

et on montre comme ci-dessus que l’on peut supposer $v'_n = v_n$. On a alors un diagramme commutatif à lignes exactes

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_2 & \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & E^0 & \rightarrow & \ldots \rightarrow & E^{n-2} & \rightarrow & M' & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_2 & \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

avec $M' = M \times_{\mathbf{R}_1} E_{n-1}$ (cf. X, p. 120, cor. 3, b)). La condition (iii) est donc satisfaite, ce qui achève la démonstration du théorème.

#### Remarque 1 {#alg-x-s7-n5-rem-1 .statement}

Si l’anneau A est nœthérien, et si les A-modules M et N sont de type fini, il résulte de la démonstration de a) que tout élément de $\mathrm{Ext}_A^n(M, N)$ est la classe associée à une suite exacte $0 \to N \to R_n \to \ldots \to R_1 \to M \to 0$ où les $R_i$ sont de type fini.

#### Corollaire {#alg-x-s7-n5-cor-1 .statement}

*Soit* $0 \to N \xrightarrow{f} R \xrightarrow{g} M \to 0$ *et* $0 \to N \xrightarrow{f'} R' \xrightarrow{g'} M \to 0$ *deux suites exactes*, $\theta$ *et* $\theta'$ *les classes associées dans* $\mathrm{Ext}^1(M, N)$. *Pour que* $\theta = \theta'$, *il faut et il suffit qu’il existe un* A-homomorphisme $h : R \to R'$ *rendant le diagramme*

$$
\begin{array}{ccc}
& & R \\
N & \xrightarrow{f} & R \\
& \downarrow h & \downarrow g \\
& & M \\
& \xrightarrow{f'} & R' \\
& & \xrightarrow{g'}
\end{array}
$$

*commutatif. Un tel homomorphisme est nécessairement un isomorphisme.*

La condition est suffisante d’après le cor. 1 de la prop. 4. Si $\theta = \theta'$, on a un diagramme commutatif à lignes exactes :

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N & \longrightarrow & R & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h'} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R'' & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h''} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R' & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

Les morphismes $h'$ et $h''$ sont des isomorphismes d’après X, p. 7, cor. 3, et $h = h'' \circ {h'}^{-1}$ répond à la question. La dernière assertion résulte de *loc. cit*.

#### Remarque 2 {#alg-x-s7-n5-rem-2 .statement}

Le théorème 1 donne une description de $\mathrm{Ext}_A^n(M, N)$ comme ensemble de classes d’équivalence de suites exactes ; il est facile de décrire la loi de groupe qu’on obtient sur cet ensemble par transport de structure. Soit en effet $\theta$ (resp. $\theta'$) la classe d’une suite exacte $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \to M \to 0$ (resp. $0 \to N \xrightarrow{f'_{n+1}} R'_n \xrightarrow{f'_n} \ldots \to R'_1 \to M \to 0$). Soient $\Delta : M \to M \oplus M$ et $\nabla : N \oplus N \to N$ les applications A-linéaires définies par $\Delta(x) = (x, x)$ pour $x \in M$ et $\nabla(y, z) = y + z$ pour $y, z \in N$. Considérons l’application

$$
m : \mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M \oplus M, N \oplus N)
$$

définie dans la *remarque*, p. 121. Avec les notations de *loc. cit.*, on a $\nabla \circ i_N = 1_N$ et $q_M \circ \Delta = 1_M$, et par suite $\theta + \theta' = \nabla \circ m(\theta, \theta') \circ \Delta$. Compte tenu de *loc. cit.* et du cor. 3, p. 120, ceci fournit une suite exacte de classe $\theta+\theta'$ : si par exemple $n\geq 2$, on peut prendre la suite

$$
0\longrightarrow \mathbf{N}\longrightarrow R_n''\longrightarrow R_{n-1}\oplus R'_{n-1}\xrightarrow{\,f_{n-1}\oplus f'_{n-1}\,}\cdots\longrightarrow R_2\oplus R'_2\longrightarrow R'_1\longrightarrow M\longrightarrow0
$$

où $R_n''$ est le quotient de $R_n\oplus R'_n$ par le sous-module formé des couples

$$
\left(f_{n+1}(x),-f'_{n+1}(x)\right)\quad\text{pour }x\in\mathbf{N},
$$

et où $R''_1=R_1\times_M R'_1$.

### 6. Produit de composition et homomorphismes de liaison des modules d’extensions

#### Proposition 5 {#alg-x-s7-prop-5 .statement}

Soient

$$(\mathcal{E})\qquad 0\longrightarrow M'\xrightarrow{\,f\,}M\xrightarrow{\,g\,}M''\longrightarrow0$$

une suite exacte de $A$-modules à gauche, $\theta\in\operatorname{Ext}^1_A(M'',M')$ la classe associée, $N$ un $A$-module à gauche, $n$ un entier.

a) L’homomorphisme de liaison $\delta^n(N,\mathcal{E}):\operatorname{Ext}^n_A(N,M'')\longrightarrow\operatorname{Ext}^{n+1}_A(N,M')$ est le produit de composition $\alpha\mapsto\theta\circ\alpha$ par $\theta$.

b) L’homomorphisme de liaison $\delta^n(\mathcal{E},N):\operatorname{Ext}^n_A(M',N)\longrightarrow\operatorname{Ext}^{n+1}_A(M'',N)$ est le produit de composition $\alpha\mapsto(-1)^{n+1}\alpha\circ\theta$ par $(-1)^{n+1}\theta$.

a) Considérons un diagramme commutatif

$$
\begin{array}{ccccccccc}
0&\longrightarrow&M'&\xrightarrow{\,f\,}&M&\xrightarrow{\,g\,}&M''&\longrightarrow&0\\
&&\downarrow\scriptstyle{1_{M'}}&&\downarrow\scriptstyle{v^0}&&\downarrow\scriptstyle{v^1}\\
0&\longrightarrow&M'&\xrightarrow{\,e_{M'}\,}&I^0(M')&\xrightarrow{\,\delta^0\,}&I^1(M').
\end{array}
$$

Par définition, $\theta$ est la classe de $-v^1\in\operatorname{Homgr}^1_A(M'',I(M'))$. Soit d’autre part $\alpha\in\operatorname{Ext}^n_A(N,M'')$, représenté par un élément $a$ de $\operatorname{Homgr}^n_A(L(N),M'')$. Par construction, $\delta^n(\alpha)$ s’obtient comme suit : on relève $a^n\in\operatorname{Hom}_A(L_n(N),M'')$ en

$$
b\in\operatorname{Hom}_A(L_n(N),M),
$$

et $\delta^n(\alpha)$ est la classe de $e_{M'}\circ c$ où $c\in\operatorname{Hom}_A(L_{n+1}(N),M')$ est tel que

$$
f\circ c=Db=(-1)^{n+1}b\circ d_{n+1}.
$$

On a donc un diagramme commutatif

$$
\begin{array}{ccccccccc}
L_{n+1}(N)&\xrightarrow{\,d_{n+1}\,}&L_n(N)& &\\
\downarrow\scriptstyle{(-1)^{n+1}c}&&\downarrow\scriptstyle{b}&\searrow\scriptstyle{a^n}&\\
0&\longrightarrow&M'&\xrightarrow{\,f\,}&M&\xrightarrow{\,g\,}&M''&\longrightarrow&0\\
&&\downarrow\scriptstyle{1_{M'}}&&\downarrow\scriptstyle{v^0}&&\downarrow\scriptstyle{v^1}\\
&&0&\longrightarrow&M'&\xrightarrow{\,e_{M'}\,}&I^0(M')&\xrightarrow{\,\delta^0\,}&I^1(M').
\end{array}
$$

Mais, dans Homgr_A (L(N), l(M')), on a

$$
D(v^0 \circ b) = \delta^0 \circ v^0 \circ b - (-1)^n v^0 \circ b \circ d_{n+1} = v^1 \circ a^n + e_{M'} \circ c .
$$

Les classes de $e_{M'} \circ c$ et $-v^1 \circ a$ dans $\mathrm{Ext}_A^{n+1}(N, M')$ sont égales, d'où $a$.

b) Considérons un diagramme commutatif

$$
\begin{array}{ccccccccc}
L_1(M'') & \xrightarrow{d_1} & L_0(M'') & \xrightarrow{p_{M''}} & M'' & \longrightarrow & 0 \\
\downarrow u_1 & & \downarrow u_0 & & \downarrow 1_{M''} \\
0 & \longrightarrow & M' & \xrightarrow{f} & M & \xrightarrow{g} & M'' & \longrightarrow & 0 .
\end{array}
$$

Par définition, $\theta$ est la classe de $-u_1 \in \mathrm{Homgr}_A^1(L(M''), M')$. Soit d'autre part $\alpha \in \mathrm{Ext}^n(M', N)$ représenté par un élément $a$ de $\mathrm{Homgr}_A^n(M', l(N))$. Par construction, $\delta^n(\alpha)$ s'obtient comme suit : on prolonge $a^n \in \mathrm{Hom}_A(M', I^n(N))$ en

$$
b \in \mathrm{Hom}_A(M, I^n(N))
$$

et $\delta^n(\alpha)$ est la classe de $c \circ p_{M''}$, où $c \in \mathrm{Hom}_A(M'', I^{n+1}(N))$ est tel que

$$
g \circ c = Db = \delta^{n+1} \circ b .
$$

On a donc un diagramme commutatif

$$
\begin{array}{ccccccccc}
L_1(M'') & \xrightarrow{d_1} & L_0(M'') & \xrightarrow{p_{M''}} & M'' & \longrightarrow & 0 \\
u_1 \downarrow & & u_0 \downarrow & & \downarrow 1_{M''} \\
0 & \longrightarrow & M' & \xrightarrow{f} & M & \xrightarrow{g} & M'' & \longrightarrow & 0 \\
& & & & b \downarrow & & c \downarrow \\
& & & & I^n(N) & \xrightarrow{\delta^n} & I^{n+1}(N) .
\end{array}
$$

Mais, dans Homgr_A (L(M''), l(N)), on a

$$
D(b \circ u_0) = \delta^n \circ b \circ u_0 - (-1)^n b \circ u_0 \circ c = c \circ p - (-1)^n a^n \circ u_1 .
$$

Les classes de $c \circ p$ et de $(-1)^{n+1} a^n \circ (-u_1)$ dans $\mathrm{Ext}_A^{n+1}(M'', N)$ sont donc égales, d'où $b$.

#### Corollaire 1 {#alg-x-s7-prop-5-cor-1 .statement}

a) *L’homomorphisme de liaison* $\mathrm{Hom}_A(M'', M'') \to \mathrm{Ext}_A^1(M'', M')$ *envoie* $1_{M''}$ *sur* $\theta$.
b) *L’homomorphisme de liaison* $\mathrm{Hom}_A(M', M') \to \mathrm{Ext}_A^1(M'', M')$ *envoie* $1_{M'}$ *sur* $-\theta$.

#### Corollaire 2 {#alg-x-s7-prop-5-cor-2 .statement}

*Considérons deux suites exactes de A-modules à gauche*

$$
\begin{align*}
0 &\to M' \to M \to M'' \to 0 \\
0 &\to N' \to N \to N'' \to 0 .
\end{align*}
$$

*Alors les homomorphismes composés d’homomorphismes de liaison*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M'',N'') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*et*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M',N') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*sont opposés.*

En effet si $\theta_1$, $\theta_2$ sont les classes associées aux suites exactes données, et si $\alpha\in\operatorname{Ext}_A^n(M',M'')$, les images de $\alpha$ sont respectivement

$$
\theta_2\circ\bigl((-1)^{n+1}\alpha\circ\theta_1\bigr)\quad\text{et}\quad
(\theta_2\circ\alpha)\circ\bigl((-1)^{n+2}\theta_1\bigr).
$$

Considérons une suite exacte de $A$-modules à gauche

$$
(\mathcal{S})\qquad 0\to N\to R_n\xrightarrow{f_n}R_{n-1}\xrightarrow{f_{n-1}}\cdots\to R_1\xrightarrow{f_1}M\to0
$$

et posons $K_0=M$, $K_i=\operatorname{Ker}f_i$, $i=1,\ldots,n-1$, $K_n=N$. On a donc des suites exactes

$$
(9)\qquad 0\to K_i\to R_i\to K_{i-1}\to0,\qquad 1\leq i\leq n,
$$

auxquelles sont associées pour tout $A$-module à gauche $P$, des homomorphismes de liaison

$$
\operatorname{Ext}_A^m(P,K_{i-1})\to\operatorname{Ext}_A^{m+1}(P,K_i),
$$

$$
\operatorname{Ext}_A^m(K_i,P)\to\operatorname{Ext}_A^{m+1}(K_{i-1},P),
$$

d’où par composition des *homomorphismes de liaison itérés*, associés à $(\mathcal{S})$

$$
\delta^m(P,\mathcal{S}):\operatorname{Ext}_A^m(P,M)\to\operatorname{Ext}_A^{m+n}(P,N)
$$

$$
\delta^m(\mathcal{S},P):\operatorname{Ext}_A^m(N,P)\to\operatorname{Ext}_A^{m+n}(M,P).
$$

#### Corollaire 3 {#alg-x-s7-prop-5-cor-3 .statement}

Si $\theta\in\operatorname{Ext}_A^n(M,N)$ est la classe de la suite exacte $(\mathcal{S})$, on a

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta\circ\alpha,\qquad
\delta^m(\mathcal{S},P)(\beta)=(-1)^{mn+n(n+1)/2}\beta\circ\theta.
$$

Si $\theta_i\in\operatorname{Ext}_A^1(K_{i-1},K_i)$ est la classe associée à la suite exacte (9), on a d’après la prop. 5

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta_n\circ\cdots\circ\theta_2\circ\theta_1\circ\alpha
$$

$$
\delta^m(\mathcal{S},P)(\beta)=(-1)^{(m+1)+\cdots+(m+n)}\beta\circ\theta_n\circ\cdots\circ\theta_1.
$$

Par ailleurs, d’après la prop. 3 (X, p. 118), on a $\theta=\theta_n\circ\cdots\circ\theta_1$. Le corollaire résulte immédiatement de là, et de la relation (E, III, p. 44)

$$
(m+1)+\cdots+(m+n)=mn+n(n+1)/2.
$$

#### Corollaire 4 {#alg-x-s7-prop-5-cor-4 .statement}

Si chaque module $R_i,\ i = 1, ..., n,$ est injectif (resp. projectif), l’application $\alpha \mapsto \theta \circ \alpha$ (resp. $\alpha \mapsto \alpha \circ \theta$) de $\mathrm{Ext}_A^m(P, M)$ dans $\mathrm{Ext}_A^{m+n}(P, N)$ (resp. de $\mathrm{Ext}_A^m(N, P)$ dans $\mathrm{Ext}_A^{m+n}(M, P)$) est bijective pour tout $A$-module $P$ et tout entier $m > 0$.

Cela résulte en effet du cor. 3 et des suites exactes

$$
\mathrm{Ext}_A^{m+i-1}(P, R_i) \to \mathrm{Ext}_A^{m+i-1}(P, K_{i-1}) \to \mathrm{Ext}_A^{m+i}(P, K_i) \to \mathrm{Ext}_A^{m+i}(P, R_i)
$$
(resp. $\mathrm{Ext}_A^{m+i-1}(R_i, P) \to \mathrm{Ext}_A^{m+i-1}(K_i, P) \to \mathrm{Ext}_A^{m+i}(K_{i-1}, P) \to \mathrm{Ext}_A^{m+i}(R_i, P)$),
dont les termes extrêmes sont nuls par hypothèse.

#### Remarque {#alg-x-s7-n6-rem-1 .statement}

Les définitions et propositions des n°s 3 à 6 s’appliquent aux $A$-modules à droite, considérés comme modules à gauche sur l’anneau $A^\circ$ opposé à $A$.

### 7. L’homomorphisme $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$

Soient $M$ un $A$-module à gauche, $P$ et $Q$ deux $A$-modules à droite. Considérons l’homomorphisme $\mathrm{Homgr}_A(L(P), L(Q)) \otimes_k (L(P) \otimes_A L(M)) \to L(Q) \otimes_A L(M)$ qui à $f \otimes (x \otimes y)$ associe $f(x) \otimes y$. D’après X, p. 99, c’est un morphisme de complexes. On en déduit une application $k$-linéaire graduée de degré 0

$$
H(\mathrm{Homgr}_A(L(P), L(Q))) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)
$$

donc par l’isomorphisme $\varphi(L(P), L(Q))$ du § 6 (X, p. 100, th. 1), une application $k$-linéaire graduée de degré 0

(10)
$$
\mathrm{Ext}_A(P, Q) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M),
$$
correspondant à des applications $k$-bilinéaires

(11)
$$
c_{P, Q; M}: \mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M);
$$
l’image du couple $(\alpha, \gamma)$ par $c_{P, Q; M}$ s’appelle produit de composition de $\alpha$ et $\gamma$ et se note $\alpha \circ \gamma$.

Par construction, $\alpha \circ \gamma$ s’obtient comme suit : on représente $\alpha$ par un morphisme de complexes $f : L(P) \to L(Q)(-n)$, $\gamma$ par un élément $z \in Z_m(L(P) \otimes_A L(M))$, et $\alpha \otimes \gamma$ est la classe de l’élément

$$
(f \otimes 1)(z) \in Z_m(L(Q)(-n) \otimes_A L(M)) = Z_{m-n}(L(Q) \otimes_A L(M)).
$$

Par exemple, si $\alpha \in \mathrm{Hom}_A(P, Q)$, alors $\alpha \circ \gamma = \mathrm{Tor}(\alpha, 1)(\gamma)$.

#### Remarque 1 {#alg-x-s7-n7-rem-1 .statement}

Si on utilise les isomorphismes $\psi$ de X, p. 69, on peut aussi définir le produit de composition par le diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P,Q;M}} & \mathrm{Tor}_{m-n}^A(Q, M) \\
\bar{a}_{P,Q} \times \psi_{P(M)} \downarrow & & \downarrow \psi_{Q(M)} \\
H^n(\mathrm{Homgr}_A(L(P), L(Q))) \times H_m(L(P) \otimes_A M) & \longrightarrow & H_{m-n}(L(Q) \otimes_A M);
\end{array}
$$

en d'autres termes, on représente $\alpha$ par un morphisme $f$ de $L(P)$ dans $L(Q) (-n)$, $\gamma$ par un cycle $x \in L_m(P) \otimes_A M$, et $\alpha \circ \gamma$ est la classe du cycle

$$
(f_m \otimes 1_M)(x) \in L_{m-n}(Q) \otimes_A M.
$$

#### Remarque 2 {#alg-x-s7-n7-rem-2 .statement}

On peut aussi utiliser les résolutions $l(P)$ et $l(Q)$.

De même, si $N$ est un deuxième $A$-module à gauche, on définit un produit de composition $(\mu, \gamma) \mapsto \mu \circ \gamma$ noté

$$
c_{P:M,N}: \mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-r}^A(P, N)
$$

par le diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P:M,N}} & \mathrm{Tor}_{m-r}^A(P, N) \\
1 \times \sigma_{P,M,r} \downarrow & & \downarrow \sigma_{P,N,m-r} \\
\mathrm{Ext}_A^r(M^\circ, N^\circ) \times \mathrm{Tor}_m^{A^\circ}(M^\circ, P^\circ) & \xrightarrow{c_{M^\circ,N^\circ,P^\circ}} & \mathrm{Tor}_{m-r}^{A^\circ}(N^\circ, P^\circ)
\end{array}
$$

où $\sigma$ désigne les isomorphismes de commutation (X, p. 71).

Si $\mu \in \mathrm{Ext}_A^r(M, N)$ est la classe du morphisme $g : L(M) \to L(N) (-r)$, et si $\gamma \in \mathrm{Tor}_m^A(P, M)$ est la classe du cycle $z = \sum z_{ij}$, où $z_{ij} \in L_i(P) \otimes_A L_j(M)$, $\mu \circ \gamma$ est donc la classe du cycle $\sum (-1)^{ir} (1 \otimes g)(z_{ij})$.

On peut aussi représenter $\gamma$ par un cycle $y \in P \otimes L_m(M)$, et $\mu \circ \gamma$ est la classe du cycle $(1 \otimes g)(y) \in P \otimes L_{m-r}(M)$.

#### Proposition 6 {#alg-x-s7-prop-6 .statement}

Soient $K, M, N$ des $A$-modules à gauche, $P, Q, R$ des $A$-modules à droite,
$\alpha \in \mathrm{Ext}_A^n(P, Q)$, $\beta \in \mathrm{Ext}_A^p(Q, R)$, $\lambda \in \mathrm{Ext}_A^r(K, M)$, $\mu \in \mathrm{Ext}_A^s(M, N)$, $\gamma \in \mathrm{Tor}_m^A(P, K)$.
Alors
(13) $$ (\beta \circ \alpha) \circ \gamma = \beta \circ (\alpha \circ \gamma) \quad \text{dans} \quad \mathrm{Tor}_{m-p-n}^A(R, K), $$
(14) $$ (\mu \circ \lambda) \circ \gamma = \mu \circ (\lambda \circ \gamma) \quad \text{dans} \quad \mathrm{Tor}_{n-r-s}^A(P, N), $$
(15) $$ \alpha \circ (\lambda \circ \gamma) = (-1)^{nr} \lambda \circ (\alpha \circ \gamma) \quad \text{dans} \quad \mathrm{Tor}_{m-p-r}^A(Q, M). $$

Les formules (13) et (14) résultent aussitôt des définitions. Démontrons (15).
Soient $z = \sum z_{ij}$, $z_{ij} \in L_i(P) \otimes L_j(K)$ un cycle représentant $\gamma$, $f : L(P) \to L(Q) (-n)$ et $g : L(K) \to L(M) (-r)$ des morphismes représentant $\alpha$ et $\lambda$. Alors $\lambda \circ (\alpha \circ \gamma)$ est la classe de $\sum (-1)^{(i-n)r} (f \otimes g)(z_{ij})$ et $\alpha \circ (\lambda \circ \gamma)$ est la classe de

$$
\sum (-1)^{ir} (f \otimes g)(z_{ij}), \quad \text{d'où (15)}.
$$

### 8. Produits de composition et homomorphismes de liaison des produits de torsion

#### Proposition 7 {#alg-x-s7-prop-7 .statement}

a) Soient

(ε)
$$
0 \to P' \xrightarrow{f} P \xrightarrow{g} P'' \to 0
$$
une suite exacte de $A$-modules à droite, $\theta \in \mathrm{Ext}_A^1(P'', P')$ la classe associée, $M$ un $A$-module à gauche. L’homomorphisme de liaison
$$
\delta_n(\mathcal{E}, M) : \mathrm{Tor}_n^A(P'', M) \to \mathrm{Tor}_{n-1}^A(P', M) \text{ est l’application } \gamma \mapsto \theta \circ \gamma .
$$

b) Soient

(ε₁)
$$
0 \to M' \to M \to M'' \to 0
$$
une suite exacte de $A$-modules à gauche, $\theta_1 \in \mathrm{Ext}_A^1(M'', M')$ la classe associée, $P$ un $A$-module à droite. L’homomorphisme de liaison
$$
\delta_n(P, \mathcal{E}_1) : \mathrm{Tor}_n^A(P, M'') \to \mathrm{Tor}_{n-1}^A(P, M') \text{ est l’application } \gamma \mapsto \theta_1 \circ \gamma .
$$
Soit $\gamma \in \mathrm{Tor}_n^A(P'', M)$ la classe d’un cycle $z'' \in \dot{Z}_n(L(P'') \otimes_A L(M))$, et soit
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & P' & \xrightarrow{f} & P & \xrightarrow{g} & P'' & \longrightarrow & 0 \\
& & \uparrow u_1 & & \uparrow u_0 & & \uparrow 1 & & \\
L_1(P'') & \xrightarrow{d_1} & L_0(P'') & \xrightarrow{p_0''} & P'' & \longrightarrow & 0
\end{array}
$$
un diagramme commutatif. On notera $p' : L(P') \to P'$ et $p'' : L(P'') \to P''$ les morphismes de complexes canoniques. Par définition, $\delta(\gamma) \in \mathrm{Tor}_{n-1}^A(P', M)$ s’obtient comme suit : on choisit $x \in P \otimes L_n(M)$ tel que $(g \otimes 1)(x) = (p'' \otimes 1)(z'')$ et $\delta(\gamma)$ est la classe des cycles $z' \in Z_{n-1}(L(P') \otimes L(M))$ tels que
$$
(f \otimes 1)(p' \otimes 1)(z') = (1 \otimes d_n)(x) .
$$
Pour $0 \leq i \leq n$, notons $z''_i$ la composante de $z''$ dans $L_i(P'') \otimes L_{n-i}(M)$; on a
$$
0 = Dz'' = \sum_i (d_i \otimes 1 + (-1)^i \otimes d_{n-i})(z''_i) ,
$$
donc $(d_i \otimes 1)(z''_i) = (-1)^i \otimes d_{n-i+1}(z''_{i-1})$ et en particulier
$$
(d_1 \otimes 1)(z''_1) = -1 \otimes d_n(z''_0) .
$$
Choisissons alors $x = (u_0 \otimes 1)(z''_0)$: on a bien
$$
(g \otimes 1)(x) = (p_0'' \otimes 1)(z''_0) = (p'' \otimes 1)(z'') .
$$
Comme
$$
(1 \otimes d_n)(x) = (u_0 \otimes 1)(1 \otimes d_n)(z''_0) = - (u_0 \otimes 1)(d_1 \otimes 1)(z''_1)
= - (f \otimes 1)(u_1 \otimes 1)(z''_1) ,
$$

il en résulte que $\delta(\gamma)$ est la classe des cycles $z' \in Z_{n-1}(L(P') \otimes_A L(M))$ tels que $(p' \otimes 1)(z') = - (u_1 \otimes 1)(z''_1)$. Mais, par définition, la classe $\theta$ correspond par l’isomorphisme $\mathrm{Ext}_A^1(P'', P') \to H^1(\mathrm{Homgr}_A(L(P''), P'))$ à la classe du morphisme $f : L(P'')(1) \to P'$ défini par $- u_1$, et le produit $\theta \circ \gamma$ est la classe des cycles

$$
\overline{z}' \in Z_{n-1}(L(P') \otimes_A L(M)) \quad \text{tels que} \quad (p \otimes 1)(\overline{z}') = f(z'') = - (u_1 \otimes 1)(z''_1),
$$

ce qui achève la démonstration de a). L’assertion b) se déduit de a) par les isomorphismes de commutation.

#### Corollaire 1 {#alg-x-s7-prop-7-cor-1 .statement}

*Soient* $0 \to P' \to P \to P'' \to 0$ *une suite exacte de* $A$-*modules à droite*, $0 \to M' \to M \to M'' \to 0$ *une suite exacte de* $A$-*modules à gauche*. *Alors les homomorphismes composés d’homomorphismes de liaison*

$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P'', M') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*et*
$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P', M'') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*sont opposés*.

En effet, si $\theta$ et $\theta_1$ sont les classes associées aux suites exactes données, et si $\gamma \in \mathrm{Tor}_n^A(P'', M'')$, les images de $\gamma$ sont respectivement $\theta \circ (\theta_1 \circ \gamma)$ et $\theta_1 \circ (\theta \circ \gamma)$, donc sont opposées d’après la prop. 6.

Reprenons les notations de X, p. 127 et considérons la suite $(\mathscr{S})$ de $A$-modules à gauche et les homomorphismes de liaison associés aux suites exactes (9)

$$
\mathrm{Tor}_m^A(P, K_{i-1}) \to \mathrm{Tor}_{m-1}^A(P, K_i);
$$

on en déduit par composition des *homomorphismes de liaison itérés*

$$
\hat{\partial}_m(P, \mathscr{S}) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(P, N).
$$

Alors d’après la prop. 7 et la prop. 3 de X, p. 118 :

#### Corollaire 2 {#alg-x-s7-prop-7-cor-2 .statement}

*Si* $\theta \in \mathrm{Ext}_A^n(M, N)$ *est la classe associée à la suite exacte* $(\mathscr{S})$, *on a* $\hat{\partial}_m(P, \mathscr{S})(\alpha) = \theta \circ \alpha$ *pour tout* $\alpha \in \mathrm{Tor}_m^A(P, M)$.

#### Corollaire 3 {#alg-x-s7-prop-7-cor-3 .statement}

*Si tous les modules* $R_i, i = 1, ..., n$, *sont plats, l’application* $\alpha \mapsto \theta \circ \alpha$ *de* $\mathrm{Tor}_{m+n}^A(P, M)$ *dans* $\mathrm{Tor}_m^A(P, N)$ *est bijective pour tout* $A$-*module à droite* $P$ *et tout entier* $m > 0$.

Cela résulte du cor. 2 et des suites exactes

$$
\mathrm{Tor}_{m+n-i+1}^A(P, R_i) \to \mathrm{Tor}_{m+n-i+1}^A(P, K_{i-1}) \xrightarrow{\hat{\partial}} \mathrm{Tor}_{m+n-i}^A(P, K_i) \to \mathrm{Tor}_{m+n-i}^A(P, R_i)
$$

où les termes extrêmes sont nuls par hypothèse.

De même, si

$$(\mathcal{S}_1)$$
$$0 \to Q \to S_n \to S_{n-1} \to \ldots \to S_1 \to P \to 0$$

est une suite exacte de $A$-modules à droite, et $M$ un $A$-module à gauche, on définit des *homomorphismes de liaison itérés*

$$\partial^m(\mathcal{S}_1, M) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M)$$

et on a :

#### Corollaire 4 {#alg-x-s7-prop-7-cor-4 .statement}

*Si $\theta_1 \in \mathrm{Ext}_A^n(P, Q)$ est la classe associée à la suite exacte $(\mathcal{S}_1)$, on a $\partial^m(\mathcal{S}_1, M)(\alpha) = \theta_1 \circ \alpha$ pour tout $\alpha \in \mathrm{Tor}_m^A(P, M)$.

### 9. Calcul des produits de composition par décalage de résolutions

Soient

(16)
$$0 \to M \xrightarrow{\iota} K_n \to K_{n-1} \to \ldots \to K_1 \xrightarrow{\rho} M' \to 0$$

une suite exacte de $A$-modules à gauche et $\theta \in \mathrm{Ext}_A^n(M', M)$ la classe associée.

Soit $a : (R, d) \to M$ une résolution gauche de $M$; on a donc une suite exacte

$$\to R_k \xrightarrow{d_k} R_{k-1} \to \ldots \xrightarrow{d_1} R_0 \xrightarrow{a_0} M \to 0.$$

et par translation de $n$ (X, p. 26) une suite exacte

(17)
$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n a_0} M \to 0.$$

On déduit de (16) et (17) une suite exacte

$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n f \circ a_0} K_n \to K_{n-1} \to \ldots \to K_1 \to M' \to 0$$

d'où une résolution $R'$ de $M'$; notons $\varphi : R' \to R(-n)$ le morphisme tel que $\varphi_k = 1_{R_{k-n}}$ pour $k \geq n$.

Si $N$ est un $A$-module à gauche et $P$ un $A$-module à droite, on a donc des homomorphismes

$$\mathrm{H}(1_P \otimes \varphi) : \mathrm{H}(P \otimes_A R') \to \mathrm{H}(P \otimes_A R)(-n)$$
$$\mathrm{H}(\mathrm{Homgr}_A(\varphi, 1_N)) : \mathrm{H}(\mathrm{Homgr}_A(R, N))(n) \to \mathrm{H}(\mathrm{Homgr}_A(R', N)).$$

Soit $k$ un entier.

#### Proposition 8 {#alg-x-s7-prop-8 .statement}

*a)* *Le diagramme suivant, où $h_\theta(\alpha) = \theta \circ \alpha$, est commutatif*

$$
\begin{array}{ccc}
\mathrm{Tor}_{k+n}^A(P, M') & \xrightarrow{h_\theta} & \mathrm{Tor}_k^A(P, M) \\
\psi_{k+n}(P, R') \downarrow & & \downarrow \psi_k(P, R) \\
\mathrm{H}_{k+n}(P \otimes_A R') & \xrightarrow{H_{k+n}(1 \otimes \varphi)} & \mathrm{H}_k(P \otimes_A R)
\end{array}
$$

b) Le diagramme suivant, où $\delta_\theta(\beta) = \beta \circ \theta$, est commutatif

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(R, N)) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(\varphi, 1))} & H^{k+n}(\mathrm{Homgr}_A(R', N)) \\
\varphi^k(R, N) \downarrow & & \varphi^{k+n}(R', N) \downarrow \\
\mathrm{Ext}_A^k(M, N) & \xrightarrow{\delta_\theta} & \mathrm{Ext}_A^{k+n}(M', N).
\end{array}
$$

Soit $\alpha : L(M) \to R$ un morphisme de complexes tel que $a \circ \alpha = p_M$ et soit

$$
\begin{array}{ccccccccc}
L_n(M') & \longrightarrow & L_{n-1}(M') & \longrightarrow & \ldots & \longrightarrow & L_0(M') & \longrightarrow & M' \longrightarrow 0 \\
u_n \downarrow & & u_{n-1} \downarrow & & & & u_0 \downarrow & & 1 \downarrow \\
0 & \longrightarrow & M & \xrightarrow{f} & K_n & \longrightarrow & \ldots & \longrightarrow & K_1 \longrightarrow M' \longrightarrow 0
\end{array}
$$

un diagramme commutatif ; choisissons un homomorphisme $v_n : L_n(M') \to L_0(M)$ tel que $p_M \circ v_n = (-1)^n u_n$; d’après X, p. 47, prop. 1, a), $v_n$ se prolonge en un morphisme de complexes $v : L(M') \to L(M) (-n)$, et $\theta$ est l’image par l’isomorphisme canonique $H^n(\mathrm{Homgr}_A(L(M'), L(M))) \to \mathrm{Ext}_A^n(M', M)$ de la classe de $v$ (X, p. 117, remarque 1). On définit un morphisme de complexes $\beta : L(M') \to R'$ par $\beta_p = u_p$ pour $p \leq n - 1$, $\beta_p = \alpha_{p-n} \circ v_p$ pour $p \geq n$, et on a

$$
\varphi \circ \beta = \alpha(-n) \circ v.
$$

D’autre part, par définition des applications $\varphi$ et $\psi$, on a

$$
\begin{aligned}
& \psi_k(P, R) = H_k(p_P \otimes \alpha), \quad \varphi^k(R, N) = H^k(\mathrm{Homgr}_A(\alpha, e_N)), \\
& \psi_{k+n}(P, R') = H_{k+n}(p_P \otimes \beta), \quad \varphi^{k+n}(R', \tilde{N}) = H^{k+n}(\mathrm{Homgr}_A(\beta, e_N)).
\end{aligned}
$$

Enfin, par définition du produit de composition, on a

$$
h_\theta = H(1_{L(P)} \otimes v), \quad \delta_\theta = H(\mathrm{Homgr}_A(v, 1_{L(N)})) .
$$

Par conséquent, on a les égalités

$$
\begin{aligned}
\psi_k(P, R) \circ h_\theta &= H_k(p_P \otimes \alpha) \circ H_k(1_{L(P)} \otimes v) = H_k(p_P \otimes (\alpha \circ v)) = H_{k+n}(p_P \otimes (\varphi \circ \beta)) \\
&= H_{k+n}(1 \otimes \varphi) \circ H_{k+n}(p_P \circ \beta) = H_{k+n}(1 \otimes \varphi) \circ \psi_{k+n}(P, R'),
\end{aligned}
$$

d’où a) ; la démonstration de b) est analogue.

#### Remarque {#alg-x-s7-n9-rem-1 .statement}

Par les isomorphismes de commutation, on déduit de a) un énoncé analogue dans le cas d’une suite exacte (16) de A-modules à droite.

Soit maintenant $b : M' \to E'$ une résolution droite de $M'$; on a donc une suite exacte

$$
0 \to M' \xrightarrow{b^0} {E'}^0 \xrightarrow{\delta^0} {E'}^1 \to \ldots \to {E'}^k \xrightarrow{\delta^k} {E'}^{k+1}
$$

d’où une suite exacte

$$
0 \to M \xrightarrow{f} K_n \to K_{n-1} \to \ldots \to K_1 \xrightarrow{(-1)^n b^0 \circ g} {E'}^0 \xrightarrow{(-1)^n \delta^0} {E'}^1 \to \ldots
$$

correspondant à une résolution droite $E$ de $M$; notons $\sigma : E'(n) \to E$ le morphisme tel que $\sigma^k = 1_{{E'}^{k-n}}$ pour $k \geq n$. On a donc des homomorphismes

$$
H(\mathrm{Homgr}_A(1_N, \sigma)) : H(\mathrm{Homgr}_A(N, E'))(n) \to H(\mathrm{Homgr}_A(N, E)) .
$$

#### Proposition 9 {#alg-x-s7-prop-9 .statement}

*Le diagramme suivant, où $\gamma_\theta(\alpha) = \theta \circ \alpha$, est commutatif* :

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(N, E')) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(1_N, \sigma))} & H^{k+n}(\mathrm{Homgr}_A(N, E)) \\
\downarrow \varphi^k(N, E') & & \downarrow \varphi^{k+n}(N, E) \\
\mathrm{Ext}_A^k(N, M') & \xrightarrow{\gamma_\theta} & \mathrm{Ext}_A^{k+n}(N, M)
\end{array}
$$

Cela se démontre de façon analogue à la prop. 8.

## EXERCICES {#alg-x-s7-exercises}

See the [exercises for § 7](exercises/s7/).
