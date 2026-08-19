---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 6
section_title: Équivalence de Morita des modules et des algèbres
lang: fr
source: alg-viii-fr
book_pages: A VIII.91-A VIII.113
pdf_pages: 0100-0122
extraction: native
subsections:
    - "no": 1
      title: Commutant et dualité
      page: 91
      pdf_page: 100
    - "no": 2
      title: Modules générateurs et modules projectifs de type fini
      page: 94
      pdf_page: 103
    - "no": 3
      title: Bimodules inversibles et équivalence de Morita
      page: 96
      pdf_page: 105
    - "no": 4
      title: Correspondance de Morita des modules
      page: 99
      pdf_page: 108
    - "no": 5
      title: Ensembles ordonnés de sous-modules
      page: 102
      pdf_page: 111
    - "no": 6
      title: Autres propriétés préservées par la correspondance de Morita
      page: 105
      pdf_page: 114
    - "no": 7
      title: Équivalence de Morita des algèbres
      page: 107
      pdf_page: 116
statements: 41
exercises: 8
content_sha256: 581628492e0f29739554405c17ff5c1e810c6f0e6a624af1ca847ee0773060fe
---

## § 6. ÉQUIVALENCE DE MORITA DES MODULES ET DES ALGÈBRES

Dans ce paragraphe, $k$ désigne un anneau commutatif.

### 1. Commutant et dualité

Soient A et B des $k$-algèbres. Rappelons (III, p. 38) qu’on appelle bimodule sur les algèbres A et B un $(A$, B)-bimodule P pour lequel les deux structures de $k$-module déduites des structures de module sur A et sur B coïncident. Pour éviter toute ambiguïté, nous dirons alors que P est un $(A,B)_k$-bimodule. Soit P un $(A,B)_k$-bimodule. On note $P^*$ le dual Hom$_A(P,A)$ du A-module à gauche sous-jacent à P. C’est un $(B,A)_k$-bimodule (II, p. 35) ; pour $a\in A,b\in B,x\in P,x^*\in P^*$, on a

$$
\langle x, bx^*a\rangle =\langle xb, x^*\rangle a \tag{1}
$$

On note également $_sA_d$ l’algèbre A considérée comme $(A,A)_k$-bimodule (loc. cit.) et $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ l’homomorphisme de $(A,A)_k$-bimodules caractérisé par

$$
\Lambda (x\otimes x^*) =\langle x, x^*\rangle \tag{2}
$$

pour $x\in P$ et $x^*\in P^*$. On note $\widetilde{P}$ le dual Hom$_B(P,B)$ du B-module à droite sous-jacent à P ; c’est un $(B,A)_k$-bimodule. On note $\widetilde{\Lambda} :\widetilde{P}\otimes_BP\rightarrow_sB_d$ l’homomorphisme de $(B,B)_k$-bimodules caractérisé par

$$
\widetilde{\Lambda}(\widetilde{x}\otimes x) =\langle \widetilde{x}, x\rangle \tag{3}
$$

pour $x\in P$ et $\widetilde{x}\in \widetilde{P}$.

Supposons maintenant que l’application $b\rightarrow b_P$ soit une bijection de B sur End$_A(P)$; c’est alors un isomorphisme de B sur l’algèbre opposée de End$_A(P)$. L’homomorphisme canonique de $\mathbf{Z}$-modules de $P^*\otimes_AP$ dans End$_A(P)$ (II, p. 77) définit alors un homomorphisme de $\mathbf{Z}$-modules $\Theta  : P^*\otimes_AP\rightarrow B$ caractérisé par

$$
x\Theta (x^*\otimes y) =\langle x, x^*\rangle y \tag{4}
$$

pour $x, y\in P$ et $x^*\in P^*$. Compte tenu de (1), cet homomorphisme est $(B$, B)-linéaire et l’on a

$$
\Theta (x^*\otimes y)y^*=x^*\langle y, y^*\rangle \tag{5}
$$

pour $y\in P$ et $x^*, y^*\in P^*$. On déduit de (4) et (5) les égalités dans le $(B,B)_k$-bimodule $P^*\otimes_AP$

$$
(y^*\otimes x)\Theta (x^*\otimes y) =y^*\otimes  \langle x, x^*\rangle y=y^*\langle x, x^*\rangle  \otimes y= \Theta (y^*\otimes x)(x^*\otimes y)
$$

pour $x, y\in P,x^*, y^*\in P^*$, d’où

$$
s\Theta (t) = \Theta (s)t \tag{6}
$$

pour $s, t\in P^*\otimes_AP$. De même, pour $x, y$ dans P et $x^*, y^*$ dans $P^*$, on déduit de (4) et (5) les égalités suivantes dans le $(A,A)_k$-bimodule $P\otimes_BP^*$

$$
(x\otimes x^*)\langle y, y^*\rangle =x\otimes \Theta (x^*\otimes y)y^*=x\Theta (x^*\otimes y)\otimes y^*=\langle x, x^*\rangle (y\otimes y^*)
$$

d’où

$$
u\Lambda (v) = \Lambda (u)v \tag{7}
$$

pour $u, v\in P\otimes_BP^*$.

Pour tout élément $x^*$ de $P^*$, notons $\sigma (x^*)$ l’application B-linéaire $x\rightarrow \Theta (x^*\otimes x)$ de P dans B. On définit ainsi une application $\sigma$ de $P^*$ dans $\widetilde{P}$ qui est $(B$, A)-linéaire et satisfait par définition à

$$
\Theta (x^*\otimes y) =\langle \sigma (x^*), y\rangle \tag{8}
$$

pour $x^*\in P^*$ et $y\in P$. Par définition de $\widetilde{\Lambda}$, on a donc

$$
\Theta  =\widetilde{\Lambda}\circ (\sigma \otimes 1_P) \tag{9}
$$

Supposons que l’application $a\rightarrow a_P$ de A dans End$_B(P)$soit bijective, c’est alors un isomorphisme d’algèbres. De manière analogue, on définit un homomorphisme de $(A,A)_k$-bimodules $\widetilde{\Theta} : P\otimes_B\widetilde{P}\rightarrow_sA_d$ caractérisé par la relation

$$
\widetilde{\Theta}(x\otimes \widetilde{y})y=x\langle \widetilde{y}, y\rangle \tag{10}
$$

pour $x, y\in P$ et $\widetilde{y}\in \widetilde{P}$. On définit aussi un homomorphisme de $(B,A)_k$-bimodules $\widetilde{\sigma}:\widetilde{P}\rightarrow P^*$ caractérisé par la formule

$$
\widetilde{\Theta}(x\otimes \widetilde{y}) =\langle x,\widetilde{\sigma}(\widetilde{y})\rangle \tag{11}
$$

pour $x\in P,\widetilde{y}\in \widetilde{P}$. On a

$$
\widetilde{\Theta} = \Lambda \circ (1_P\otimes \widetilde{\sigma}) \tag{12}
$$

#### Proposition 1 {#alg-viii-s6-prop-1 .statement tag=006R}

Supposons que les applications $b\rightarrow b_P$ de B dans End$_A(P)$et $a\rightarrow a_P$ de A dans End$_B(P)$soient bijectives. Alors $\sigma$ et $\widetilde{\sigma}$ sont des isomorphismes réciproques l’un de l’autre et l’on a les formules

$$
\Lambda  =\widetilde{\Theta}\circ (1_P\otimes \sigma ) \tag{13}
$$

$$
\widetilde{\Lambda} = \Theta \circ (\widetilde{\sigma}\otimes 1_P) \tag{14}
$$

Pour $x\in P,x^*\in P^*$ et $y\in P$, on a, d’après les formules (4), (8), (10) et (11), (15) $\langle x, x^*\rangle y=x\Theta (x^*\otimes y) =x\langle \sigma (x^*), y\rangle =\widetilde{\Theta}(x\otimes \sigma (x^*))y=\langle x,\widetilde{\sigma}(\sigma (x^*))\rangle y$.

De même, pour $x\in P,\widetilde{y}\in \widetilde{P}$ et $y\in P$, on a

$$
x\langle \widetilde{y}, y\rangle =\widetilde{\Theta}(x\otimes \widetilde{y})y=\langle x,\widetilde{\sigma}(\widetilde{y})\rangle y=x\Theta  (\widetilde{\sigma}(\widetilde{y})\otimes y) =x\langle \sigma (\widetilde{\sigma}(\widetilde{y})), y\rangle \tag{16}
$$

Vu les hypothèses faites, P est fidèle en tant que A-module et en tant que B-module. Des formules (15) et (16) respectivement, on déduit $\widetilde{\sigma}\circ \sigma = 1_{P^*}$ et $\sigma \circ \widetilde{\sigma}= 1_{\widetilde{P}}$. Les formules (13) et (14) découlent alors de (12) et (9) respectivement.

#### Remarque 1 {#alg-viii-s6-n1-rem-1 .statement tag=006S}

Supposons que l’application $b\rightarrow b_P$ de B dans End$_A(P)$ soit bijective. Alors

a) Le B-module P s’identifie au contremodule de P ; il est donc fidèle et équilibré ;

b) Pour que l’application $a\rightarrow a_P$ de A dans End$_B(P)$ soit bijective, il faut et il suffit que le A-module P soit fidèle et équilibré.

#### Remarque 2 {#alg-viii-s6-n1-rem-2 .statement tag=006T}

Sous les hypothèses de la prop. 1, le A-module P est équilibré ; comme les anneaux $A_P$ et $A'_P$ ont même centre (VIII, p. 73), il existe un isomorphisme $\varphi$ du centre Z(A) de l’anneau A sur le centre Z(B) de l’anneau B caractérisé par la relation $\varphi (z)_P=z_P$ pour $z\in Z(A)$. De plus, les endomorphismes du $(A,B)_k$-bimodule P sont les homothéties $z_P$ où $z$ parcourt Z(A) ; les automorphismes du $(A,B)_k$-bimodule P sont les homothéties $z_P$ où $z$ est inversible dans Z(A).

### 2. Modules générateurs et modules projectifs de type fini

#### Proposition 2 {#alg-viii-s6-prop-2 .statement tag=006U}

Soient A et B des algèbres sur $k$ et soit P un $(A,B)_k$-bimodule. On suppose que l’application $b\rightarrow b_P$ de B dans End$_A(P)$est bijective. Les assertions suivantes sont équivalentes :

(i) Le A-module P est projectif de type fini ;

(ii) L’application Θ (VIII, p. 92) est un isomorphisme de $(B,B)_k$-bimodules de $P^*\otimes_AP$sur $_sB_d$;

(iii) L’image de Θ contient l’élément unité de B.

Si de plus l’application $a\rightarrow a_P$ de A dans End$_B(P)$est bijective, les assertions précédentes équivalent à la condition suivante :

(iv) Il existe un $(B,A)_k$-bimodule Q et un homomorphisme surjectif de $(B,B)_k$-bimodules de $Q\otimes_AP$sur $_sB_d$.

Par le corollaire de II, p. 77, l’assertion (i) implique (ii). De plus, (iii) résulte de (ii). Soit $t\in E^*\otimes E$ tel que $\Theta (t) = 1$. Soit $n$ un entier et soient $(x_1, . . . , x_n)\in P^n$ et $(x^*_1, . . . , x^*_n)\in P^{*n}$ tels que $t=\sum^n_{i=1}x^*_i\otimes x_i$. Pour tout $x$ appartenant à P, la relation $x\Theta (t) =x$ s’écrit

$$
\sum_{i=1}^n< x, x^*_i> x_i=x
$$

Il en résulte que le A-module P est de type fini engendré par la famille $(x_i)_{1\leqslant i\leqslant n}$ et on conclut la preuve de l’implication (iii) $=\Rightarrow$ (i) par la prop. 12 de II, p. 46.

De plus, on a évidemment (ii) $=\Rightarrow$ (iv). Soient Q un $(B,A)_k$-bimodule et $\theta$ un homomorphisme surjectif de $(B,B)_k$-bimodules de $Q\otimes_AP$ sur $_sB_d$. Avec les notations du numéro précédent, il existe un homomorphisme de $(B,A)_k$-bimodules $\zeta : Q\rightarrow \widetilde{P}$ tel que $\theta (y\otimes x) =\langle \zeta (y), x\rangle$ pour $x\in P,y\in Q$, et l’on a $\theta =\widetilde{\Lambda}\circ (\zeta \otimes 1_P)$. Comme $\theta$ est surjectif, il en est de même de $\widetilde{\Lambda}$. Si l’application $a\rightarrow a_P$ de A dans End$_B(P)$ est bijective, Θ est surjective d’après la relation (14) de la prop. 1 de VIII, p. 93, d’où l’implication (iv) $=\Rightarrow$ (iii).

#### Proposition 3 {#alg-viii-s6-prop-3 .statement tag=006V}

Soient A et B des algèbres sur $k$ et P un $(A,B)_k$-bimodule. Les propriétés suivantes sont équivalentes :

(i) Le A-module P est générateur ;

(ii) L’image de l’application Λ de $P\otimes_BP^*$ dans $_sA_d$ (VIII, p. 91) contient l’élément unité ;

(iii) Il existe un $(B,A)_k$-bimodule Q et un homomorphisme surjectif de $(A,A)_k$-bimodules de $P\otimes_BQ$dans $_sA_d$. Si de plus l’application $b\rightarrow b_P$ de B dans End$_A(P)$est bijective, elles sont équivalentes à la condition suivante :

(iv) L’application Λ est un isomorphisme de $P\otimes_BP^*$ sur $_sA_d$.

(i) $\Leftarrow \Rightarrow$ (ii) : l’image de Λ est l’idéal trace $\tau (P)$ (VIII, p. 75). L’équivalence de (i) et (ii) résulte donc du théorème 1 de VIII, p. 76.

(ii) $=\Rightarrow$ (iii) : il suffit de poser $Q = P^*$.

(iii) $=\Rightarrow$ (ii) : soient Q un $(B,A)_k$-bimodule et $\psi$ un homomorphisme de $(A,A)_k$-bimodules de $P\otimes_BQ$ dans $_sA_d$. Il existe un homomorphisme de $(B,A)_k$-bimodules Ψ de Q dans $P^*$ tel que $\psi (x\otimes y) =\langle x,\Psi (y)\rangle$ pour $x\in P$ et $y\in Q$, et l’on a l’égalité $\psi = \Lambda \circ (1_P\otimes \Psi )$. Si $\psi$ est surjectif, il en est de même de Λ.

Il est clair que (iv) implique (ii). Inversement, supposons que la condition (ii) soit satisfaite et que l’application $b\rightarrow b_P$ de B dans End$_A(P)$ soit bijective. Soit $e$ un élément de $P\otimes_BP^*$ tel que $\Lambda (e) = 1$. D’après la formule (7) de VIII, p. 92, on a $u= \Lambda (u)e$ pour tout $u$ dans $P\otimes_BP^*$, d’où l’injectivité de Λ.

#### Proposition 4 {#alg-viii-s6-prop-4 .statement tag=006W}

Soient A et B des algèbres sur $k$ et P un $(A,B)_k$-bimodule. On suppose que l’application $b\rightarrow b_P$ de B dans End$_A(P)$est bijective.

a) Si le A-module P est générateur, le B-module à droite P est projectif de type fini.

b) Si le A-module P est projectif de type fini, le B-module à droite P est générateur.

Supposons le A-module P générateur. Il est alors fidèle et équilibré (VIII, p. 78, th. 2) et par suite l’application $a\rightarrow a_P$ de A dans End$_B(P)$ est bijective (VIII, p. 93, remarque 1). De plus, l’application $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ est bijective (VIII, p. 94, prop. 3). Considérons P comme un $(B^o,A^o)_k$-bimodule. L’application Λ induit une application bijective $P^*\otimes_{B^o}P\rightarrow A^o$; par la prop. 2 de VIII, p. 94, (iv) $=\Rightarrow$ (i), le B-module à droite P est projectif de type fini.

Supposons maintenant le A-module P projectif et de type fini. Alors l’application $\Theta  : P^*\otimes_AP\rightarrow_sB_d$ est bijective (loc. cit. (i) $=\Rightarrow$ (ii)). D’après l’implication (iii) $=\Rightarrow$ (i) de la prop. 3 ci-dessus appliquée au $(B^o,A^o)_k$-bimodule P, le B-module à droite P est générateur.

#### Corollaire 1 {#alg-viii-s6-prop-4-cor-1 .statement tag=006X}

Le contremodule d’un module générateur est projectif de type fini. Le contremodule d’un module projectif de type fini est générateur.

Soit A une $k$-algèbre et soit M un A-module. On note B la $k$-algèbre opposée de l’algèbre End$_A(M)$. Le corollaire résulte de la proposition 4 appliquée au $(A,B)_k$-bimodule M.

#### Corollaire 2 {#alg-viii-s6-prop-4-cor-2 .statement tag=006Y}

Soient A et B des $k$-algèbres et P un $(A,B)_k$-bimodule. Les propriétés suivantes sont équivalentes :

(i) Le A-module P est générateur et l’application $b\rightarrow b_P$ de B dans End$_A(P)$ est bijective.

(ii) Le B-module à droite P est projectif de type fini, fidèle et équilibré et l’application $a\rightarrow a_P$ de A dans End$_B(P)$est bijective.

L’implication (i) $=\Rightarrow$ (ii) résulte de la proposition 4 a) et de la remarque 1 (VIII, p. 93). Sous les hypothèses de (ii), le A-module P est générateur (prop. 4, b) appliquée au $(B^o,A^o)_k$-bimodule P). Comme le B-module P est fidèle et équilibré, la seconde assertion de (i) est aussi vérifiée (VIII, p. 93, remarque 1).

### 3. Bimodules inversibles et équivalence de Morita

#### Définition 1 {#alg-viii-s6-def-1 .statement tag=006Z}

Soient A et B des $k$-algèbres et P un $(A,B)_k$-bimodule. On dit que P est inversible s’il existe un $(B,A)_k$-bimodule Q tel que $P\otimes_BQ$soit isomorphe à $_sA_d$ et $Q\otimes_AP$à $_sB_d$. Un tel bimodule Q s’appelle un inverse de P.

Soient A et B des $k$-algèbres. Soit P un $(A,B)_k$-bimodule inversible. Soit C une $k$-algèbre et $P'$ un $(B,C)_k$-bimodule inversible. Soient Q et $Q'$ des bimodules inverses de P et $P'$ respectivement. D’après l’associativité du produit tensoriel (II, p. 64, prop. 8) et la prop. 4 de II, p. 55, le $(C,A)_k$-bimodule $Q'\otimes_BQ$ est un inverse du $(A,C)_k$-bimodule $P\otimes_BP'$, de sorte que $P\otimes_BP'$ est un $(A,C)_k$-bimodule inversible.

Ainsi la relation

« A et B sont des $k$-algèbres et il existe un $(A,B)_k$-bimodule inversible »

est une relation d’équivalence.

#### Définition 2 {#alg-viii-s6-def-2 .statement tag=0070}

On dit que des $k$-algèbres A et B sont équivalentes au sens de Morita s’il existe un $(A,B)_k$-bimodule inversible. On dit que des anneaux A et B sont équivalents au sens de Morita si les $\mathbf{Z}$-algèbres A et B sont équivalentes au sens de Morita.

Deux $k$-algèbres isomorphes sont équivalentes au sens de Morita. Si deux $k$-algèbres sont équivalentes au sens de Morita, leurs algèbres opposées sont équivalentes au sens de Morita.

Soient P un $(A,B)_k$-bimodule inversible et Q un inverse de P. Alors Q est un $(B,A)_k$-bimodule inversible et admet P comme inverse. De plus, vu comme $(B^o,A^o)_k$-bimodule, P est inversible et admet pour inverse le $(A^o,B^o)_k$-bimodule Q.

#### Lemme 1 {#alg-viii-s6-lem-1 .statement tag=0071}

Soient A et B des $k$-algèbres, P un $(A,B)_k$-bimodule inversible, M et N des B-modules et $u: M\rightarrow N$une application B-linéaire. Si l’application $1_P\otimes u:$ $P\otimes_BM\rightarrow P\otimes_BN$est nulle (resp. bijective), il en est de même de $u$.

Soient Q un bimodule inverse de P et $\theta : Q\otimes_AP\rightarrow_sB_d$ un isomorphisme de $(B,B)_k$-bimodules. Le lemme résulte de la commutativité du diagramme

$Q\otimes_AP\otimes_BM^{1_Q\otimes 1_P\otimes u}/$/ $Q\otimes_AP\otimes_BN$

$\theta \otimes 1_M\theta \otimes 1_M$

M $u$ // N.

#### Théorème 1 {#alg-viii-s6-thm-1 .statement tag=0072}

Soient A et B des $k$-algèbres et P un $(A,B)_k$-bimodule. Notons $P^*$ le $(B,A)_k$-bimodule Hom$_A(P,A_s)$. Les assertions suivantes sont équivalentes :

(i) Le $(A,B)_k$-bimodule P est inversible ;

(ii) Le A-module P est projectif, de type fini et générateur, et l’application $b\rightarrow b_P$ de B dans End$_A(P)^o$ est un isomorphisme de $k$-algèbres ;

(iii) Le B-module à droite P est projectif, de type fini et générateur et l’application $a\rightarrow a_P$ de A dans End$_B(P)$est un isomorphisme de $k$-algèbres.

Si ces conditions sont vérifiées, les homomorphismes

$\Theta  : P^*\otimes P\rightarrow_sB_d$ et $\Lambda  : P\otimes P^*\rightarrow_sA_d$

sont des isomorphismes de sorte que le $(B,A)_k$-bimodule $P^*$ est un inverse de P.

Si la condition (ii) est vérifiée, P est un $(A,B)_k$-bimodule inversible d’inverse $P^*$ (VIII, p. 94, prop. 2 et p. 94, prop. 3). Cela démontre que (ii) implique (i) et la dernière assertion.

Supposons le $(A,B)_k$-bimodule P inversible. Alors le A-module P est générateur (VIII, p. 94, prop. 3, (iii) $=\Rightarrow$ (i)). Il est donc fidèle et équilibré (VIII, p. 78, th. 2) et, par suite, l’application $a\rightarrow a_p$ de A dans End$_B(P)$ est bijective.

Prouvons ensuite que l’application $b\rightarrow b_P$ de B dans End$_A(P)$ est bijective. Soit Q un $(B,A)_k$-bimodule inverse de P. Soit $u\in$ End$_A(P)$; alors $1_Q\otimes u$ est un endomorphisme du B-module à gauche $Q\otimes_AP$. Comme le $(B,B)_k$-bimodule $Q\otimes_AP$ est isomorphe à $_sB_d$, il existe un unique élément $b$ de B tel que $1_Q\otimes u$ soit l’homothétie de rapport $b$ du B-module à droite $Q\otimes_AP$. Par suite, on a $1_Q\otimes (u-b_P) = 0$. D’où $u=b_P$ d’après le lemme 1 ; cela prouve que l’application $b\rightarrow b_P$ de B dans End$_A(P)$ est bijective.

D’après la prop. 2 de VIII, p. 94, le A-module P est alors projectif de type fini. On a donc prouvé l’équivalence de (i) et (ii).

En échangeant les rôles de A et B, on obtient l’équivalence de (i) et (iii), ce qui achève la preuve de la proposition.

#### Corollaire 1 {#alg-viii-s6-thm-1-cor-1 .statement tag=0073}

Soient A et B des $k$-algèbres équivalentes au sens de Morita et soit P un $(A,B)_k$-bimodule inversible. Il existe un isomorphisme $\varphi$ du centre Z(A) de A sur le centre de B caractérisé par la relation $\varphi (z)_P=z_P$ pour tout $z\in Z(A)$. Les automorphismes du $(A,B)_k$-bimodule P sont les homothéties $z_P$ où $z$ est un élément inversible de Z(A).

Compte tenu du th. 1, cela résulte de la remarque 2 de VIII, p. 93.

#### Corollaire 2 {#alg-viii-s6-thm-1-cor-2 .statement tag=0074}

Soient A et B des $k$-algèbres équivalentes au sens de Morita et soit P un $(A,B)_k$-bimodule inversible. Tout $(B,A)_k$-bimodule inverse de P est isomorphe au dual $P^*$ = Hom$_A(P,A)$de P. Plus précisément, soit Q un $(B,A)_k$-bimodule inverse de P et soit $\lambda : P\otimes_BQ\rightarrow_sA_d$ un isomorphisme de $(A,A)_k$-bimodules, il existe une unique application $\tau : Q\rightarrow P^*$ caractérisée par la relation $\langle p, \tau (q)\rangle =\lambda (p\otimes q)$pour $p\in P$et $q\in Q$, et $\tau$ est un isomorphisme de $(B,A)_k$-bimodules.

L’existence et l’unicité de l’application $\tau$ sont claires. C’est un homomorphisme de $(B,A)_k$-bimodules et l’on a$\lambda = \Lambda \circ (1_P\otimes \tau )$. Comme $\lambda$ et Λ sont des isomorphismes de $(A,A)_k$-bimodules (VIII, p. 97, th. 1), il en est de même de $1_P\otimes \tau$. D’après le lemme 1 (VIII, p. 97), l’application $\tau$ est bijective.

#### Remarque {#alg-viii-s6-n3-rem-1 .statement tag=0075}

Sous les hypothèses du corollaire, soit $q$ un élément de Q tel qu’on ait $\lambda (p\otimes q) = 0$ pour tout $p\in P$. On a alors $\tau (q) = 0$, c’est-à-dire $q= 0$. De même, si $p$ est un élément de P tel qu’on ait $\lambda (p\otimes q) = 0$ pour tout $q\in Q$, alors $p= 0$.

#### Exemple 1 {#alg-viii-s6-n3-exa-1 .statement tag=0076}

Soient B une $k$-algèbre, $n$ un entier $\geqslant 1$ et A la $k$-algèbre $\mathbf{M}_n(B)$. Le B-module à droite $P = B^n_d$ est projectif, de type fini et générateur, et A s’identifie à l’algèbre des endomorphismes de P (II, p. 150). D’après le théorème 1, le $(A,B)_k$-bimodule P est inversible. Les algèbres B et $\mathbf{M}_n(B)$ sont donc équivalentes au sens de Morita.

#### Exemple 2 {#alg-viii-s6-n3-exa-2 .statement tag=00SH}

Soient A une $k$-algèbre commutative et P un A-module. Considérons P

comme un $(A,A)_k$-bimodule dont les deux lois d’action sont égales. Si le $(A,A)_k$-bimodule P est inversible, le A-module P est de type fini (th. 1). Compte tenu du th. 3 de AC, II, p. 143, les propriétés suivantes sont équivalentes :

(i) Le $(A,A)_k$-bimodule P est inversible ;

(ii) Il existe un A-module Q tel que $P\otimes_AQ$ soit isomorphe à A ;

(iii) Le A-module P est projectif, de type fini et de rang $1.*$

### 4. Correspondance de Morita des modules

Dans ce numéro, les lettres A et B désignent des $k$-algèbres équivalentes au sens de Morita et P un $(A,B)_k$-bimodule inversible. Choisissons un $(B,A)_k$-bimodule Q inverse de P et des isomorphismes

$\lambda : P\otimes_BQ\rightarrow_sA_d$ et $\theta : Q\otimes_AP\rightarrow_sB_d$.

Pour tout B-module à gauche V, nous noterons $\theta_V$ l’isomorphisme de B-modules $\theta \otimes 1_V: Q\otimes_AP\otimes_BV\rightarrow V$. De même, pour tout A-module à gauche M, nous noterons $\lambda_M$ l’isomorphisme de A-modules $\lambda \otimes 1_M: P\otimes_BQ\otimes_AM\rightarrow M$.

#### Théorème 2 (Morita) {#alg-viii-s6-thm-2 .statement tag=00S2}

a) Soient V et W des B-modules à gauche. L’application $g\rightarrow 1_P\otimes g$ est une bijection de Hom$_B(V,W)$sur Hom$_A(P\otimes_BV,P\otimes_BW)$. La bijection réciproque associe à tout élément $h$ de Hom$_A(P\otimes_BV,P\otimes_BW)$l’élément $\theta_W\circ (1_Q\otimes h)\circ \theta^{-1}_V$ de Hom$_B(V,W)$.

b) Pour tout A-module à gauche M l’application $\lambda_M: P\otimes_BQ\otimes_AM\rightarrow M$est un isomorphisme. En particulier, tout A-module à gauche est isomorphe à un module de la forme $P\otimes_BV$, où V est un B-module à gauche.

Soient V et W des B-modules à gauche. D’après le lemme 1 de VIII, p. 97, l’application $\varphi :g\rightarrow 1_P\otimes g$ de Hom$_B(V,W)$ dans Hom$_A(P\otimes_BV,P\otimes_BW)$ est injective. En échangeant les rôles de P et Q (et de A et B), on voit que l’application $\psi :h\rightarrow 1_Q\otimes h$ de Hom$_A(P\otimes_BV,P\otimes_BW)$ dans Hom$_A(Q\otimes_AP\otimes_BV,Q\otimes_AP\otimes_BW)$ est aussi injective. Or le composé $\psi \circ \varphi$ est l’application $g\rightarrow \theta^{-1}_W\circ g\circ \theta_V$. Elle est bijective, donc il en de même de $\psi$. Par suite, $\varphi$ est bijective et son application réciproque est l’application $h\rightarrow \theta_W\circ (1_Q\otimes h)\circ \theta^{-1}_V$.

L’assertion b) a déjà été vue.

Soient V un B-module à gauche et W un sous-module de V. Puisque le B-module P est projectif (VIII, p. 97, th. 1), l’application canonique de $P\otimes_BW$ dans $P\otimes_BV$ est injective. Nous identifierons $P\otimes_BW$ à son image dans $P\otimes_BV$ par cette application. On adopte des conventions analogues lorsque P et B sont remplacés par Q et A.

#### Proposition 5 {#alg-viii-s6-prop-5 .statement tag=0077}

Soit V un B-module à gauche. L’application $W\rightarrow P\otimes_BW$est un isomorphisme de l’ensemble, ordonné par inclusion, des sous-B-modules de V sur l’ensemble, ordonné par inclusion, des sous-A-modules de $P\otimes_BV$. L’isomorphisme réciproque associe à un sous-A-module N de $P\otimes_BV$l’image par $\theta_V$ du sous-B-module $Q\otimes_AN$de $Q\otimes_AP\otimes_BV$.

Désignons par $D_B(V)$ l’ensemble des sous-B-modules de V, ordonné par inclusion, et définissons de même les ensembles $D_A(P\otimes_BV)$ et $D_B(Q\otimes_AP\otimes_BV)$. Notons $\varphi : D_B(V)\rightarrow D_A(P\otimes_BV)$ l’application $W\rightarrow P\otimes_BW$ et $\psi$ l’application de $D_A(P\otimes_BV)$ dans $D_B(Q\otimes_AP\otimes_BV)$ donnée par $N\rightarrow Q\otimes_AN$. Ces applications sont croissantes, et l’application composée $\psi \circ \varphi$ est l’application $W\rightarrow \theta_V^{-1}$(W), qui est bijective. Par suite $\varphi$ est injective et $\psi$ surjective. En remplaçant B par A et V par $P\otimes_BV$, on voit que $\psi$ est aussi injective. Donc $\varphi$ et $\psi$ sont bijectives et l’application réciproque de $\varphi$ est bien celle décrite dans l’énoncé.

#### Exemple 1 {#alg-viii-s6-n4-exa-1 .statement tag=0078}

Appliquons la proposition 5 de VIII, p. 99 au cas particulier $V = B_s$.

a) L’application $J\rightarrow$ PJ est un isomorphisme de l’ensemble ordonné $D(B_s)$ des idéaux à gauche de B sur l’ensemble ordonné D(P) des sous-A-modules de P. L’application réciproque associe à un sous-A-module M de P l’idéal à gauche J(M) de B formé des éléments $b$ de B tels que M contienne $Pb$.

b) L’application $K\rightarrow$ KP est un isomorphisme de l’ensemble ordonné $D(A_d)$ des idéaux à droite de A sur l’ensemble ordonné D(P) des sous-B-modules de P. L’application réciproque associe à un sous-B-module V de P l’idéal à gauche K(V) de A formé des éléments $a$ de A tels que V contienne $aP$.

En effet, le A-module $P\otimes_BB_s$ s’identifie canoniquement à P. Si J est un idéal à gauche de B, l’image canonique de $P\otimes_BJ$ dans $P\otimes_BB_s$ correspond à PJ par cette identification. Par suite l’application $J\rightarrow$ PJ est un isomorphisme d’ensembles ordonnés de $D(B_s)$ sur D(P). Soit $J\in D(B_s)$. Notons $J'$ l’ensemble des éléments $b$ de B tels que PJ contienne $Pb$. C’est un idéal à gauche de B qui contient J, et on a PJ$'\subset$ PJ. Comme l’application $J\rightarrow$ PJ est un isomorphisme d’ensembles ordonnés, on a forcément PJ$'=$ PJ et $J = J'$. Cela prouve a).

L’assertion b) résulte de l’assertion a) appliquée au $(B^o,A^o)_k$-bimodule inversible P.

Notons que l’anneau A est un corps si et seulement si le B-module P est simple.

#### Exemple 2 {#alg-viii-s6-n4-exa-2 .statement tag=0079}

Notons $\mathscr{B}_A,\mathscr{B}_B$ et $\mathscr{B}_P$ les ensembles ordonnés formés des idéaux bilatères de A, des idéaux bilatères de B, et des sous-(A$,B$)$_k$-bimodules de P respectivement.

a) L’application $\mathfrak{b}\rightarrow P\mathfrak{b}$ est un isomorphisme d’ensembles ordonnés de $\mathscr{B}_B$ sur $\mathscr{B}_P$; l’isomorphisme réciproque associe à un sous-(A$,B$)$_k$-bimodule $P'$ de P l’idéal bilatère de B formé des éléments $b$ tels que $Pb\subset P'$.

b) L’application $\mathfrak{a}\rightarrow \mathfrak{a}P$ est un isomorphisme d’ensembles ordonnés de $\mathscr{B}_A$ sur $\mathscr{B}_P$; l’isomorphisme réciproque associe à un sous-(A$,B$)$_k$-bimodule $P'$ de P l’idéal bilatère de A formé des éléments $a$ tels que $aP\subset P'$.

En effet, soient J un idéal à gauche de B et $P'=$ PJ. Alors $P'$ est un sous-A-module de P et, par l’exemple 1, J se compose des éléments $b$ de B tels que $Pb\subset P'$ De plus $P'$ est un sous-(A$,B$)$_k$-bimodule de P si et seulement si J est un idéal bilatère de B. Ainsi a) résulte de loc. cit.

L’assertion b) résulte de a) appliquée au $(B^o,A^o)_k$-bimodule inversible P.

#### Proposition 6 {#alg-viii-s6-prop-6 .statement tag=007A}

Notons $\mathscr{B}_A,\mathscr{B}_B$ les ensembles ordonnés formés des idéaux bilatères de A et des idéaux bilatères de B.

a) Il existe un isomorphisme d’ensembles ordonnés $f$ de $\mathscr{B}_A$ sur $\mathscr{B}_B$ caractérisé par la propriété suivante : si $\mathfrak{a}$ est un idéal bilatère de A et $\mathfrak{b}$ un idéal bilatère de B, la relation $f(\mathfrak{a}) =\mathfrak{b}$ équivaut à $\mathfrak{a}P = P\mathfrak{b}$.

b) Supposons l’anneau A commutatif, de sorte que A s’identifie au centre de B (VIII, p. 98, cor. 1). L’isomorphisme $f:\mathscr{B}_A\rightarrow \mathscr{B}_B$ associe à un idéal $\mathfrak{a}$ de A l’idéal bilatère $B\mathfrak{a}$ de B, et l’on a $\mathfrak{a}= A\cap B\mathfrak{a}$.

L’assertion a) résulte de l’exemple 2.

Supposons enfin A commutatif, et identifions A au centre de B. Soit $\mathfrak{a}$ un idéal de A. Alors $B\mathfrak{a}$ est un idéal bilatère de B ; on a PB$\mathfrak{a}=\mathfrak{a}P$, d’où $f(\mathfrak{a}) = B\mathfrak{a}$. Soit $\mathfrak{a}'$ l’idéal $A\cap B\mathfrak{a}$ de A ; il est contenu dans $B\mathfrak{a}$ et contient $\mathfrak{a}$, donc $B\mathfrak{a}'$ est égal à $B\mathfrak{a}$. Comme $f$ est bijectif, on en déduit $\mathfrak{a}'=\mathfrak{a}$.

#### Exemple 3 {#alg-viii-s6-n4-exa-3 .statement tag=007B}

Soit V un B-module à gauche. Alors la correspondance précédente envoie l’annulateur du B-module V sur l’annulateur du A-module $P\otimes_BV$. En effet, notons $\mathfrak{a}$ l’annulateur du A-module $P\otimes_BV$ et $\mathfrak{b}$ celui du B-module V. Soit W le $(A,B)_k$-sous-bimodule de P formé des éléments tels que $p\otimes v= 0$ pour tout $v$ de V. On a l’inclusion $P\mathfrak{b}\subset W$; inversement, pour tout $p\in W$ et $q\in Q$, on a que $\theta (q\otimes p)$ appartient à $\mathfrak{b}$. Donc l’élément $\mathfrak{b}$ de $D(B_s)$ correspond à l’élément W de D(P). De même, $\mathfrak{a}\in D(A_d)$ correspond à W.

#### Exemple 4 {#alg-viii-s6-n4-exa-4 .statement tag=007C}

Pour tout idéal bilatère $\mathfrak{a}$ de A, notons $\mathbf{M}_n(\mathfrak{a})$ le sous-ensemble de $\mathbf{M}_n(A)$ formé des matrices à éléments dans $\mathfrak{a}$. C’est un idéal bilatère de $\mathbf{M}_n(A)$. On a $\mathbf{M}_n(\mathfrak{a})A^n=\mathfrak{a}^n= A^n\mathfrak{a}$. Il résulte de la prop. 6 que tout idéal bilatère de $\mathbf{M}_n(A)$ est de la forme $\mathbf{M}_n(\mathfrak{a})$, où $\mathfrak{a}$ est un idéal bilatère de A.

#### Remarque {#alg-viii-s6-n4-rem-1 .statement tag=007D}

Conservons les hypothèses et notations précédentes et supposons que le $(B,A)_k$-bimodule Q soit le dual $P^*$ du A-module P et que les isomorphismes $\lambda$ et $\theta$ soient les applications canoniques $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ et $\Theta  : P^*\otimes_AP\rightarrow_sB_d$ (VIII, p. 97, th. 1). Comme le A-module P est projectif de type fini, on dispose, pour tout A-module M, d’un isomorphisme canonique $\vartheta_M: P^*\otimes_AM\rightarrow$ Hom$_A(P,M)$ (II, p. 77, cor.). Nous laissons au lecteur le soin de traduire les résultats du présent numéro en remplaçant la construction $M\rightarrow Q\otimes_AM$ par la construction $M\rightarrow$ Hom$_A(P,M)$.

### 5. Ensembles ordonnés de sous-modules

Dans ce numéro, on note A et B des $k$-algèbres, M un A-module à gauche, V un B-module à gauche. On note D(M) (resp. D(V)) l’ensemble ordonné par inclusion des sous-modules de M (resp. de V). On suppose donné un isomorphisme d’ensembles ordonnés $\varphi : D(V)\rightarrow D(M)$.

D’après le théorème de Morita (VIII, p. 99, th. 2), on obtient un tel isomorphisme dans la situation suivante : P est un $(A,B)_k$-bimodule inversible, M est le A-module $P\otimes_BV$ et pour tout sous-module W de $V,\varphi (W)$ est l’image canonique de $P\otimes_BW$ dans M.

Un certain nombre de propriétés du module M, ou de ses sous-modules, s’expriment en termes de l’ensemble ordonné D(M) : elles sont présentées dans les tables I et II.

### TABLE I

Sous-modules de $\mathbf{M}$ Ensemble ordonné D(M)

Sous-module nul Plus petit élément de D(M)

Sous-module M Plus grand élément de D(M)

$\bigcap_{i\in I}M_i$ Borne inférieure inf$_{i\in I}M_i$

$\sum_{i\in I}M_i$ Borne supérieure sup$_{i\in I}M_i$

Sous-modules supplémentaires inf(M$',M''$) $= 0$, sup(M$',M''$) $= M$

Sous-module simple de M Élément minimal de D(M) $-\{0\}$

Sous-module maximal de M Élément maximal de D(M)$-\{M\}$

Socle $\mathscr{S}(M)$ de M Borne supérieure dans D(M) de l’ensemble

des éléments minimaux de D(M) $-\{0\}$

$*$ Radical $\mathfrak{R}(M)$ de M (VIII, p. 147)$*$ Borne inférieure dans D(M) de l’ensemble

des éléments maximaux de D(M)$-\{M\}$

### TABLE II

Propriétés du module M Propriétés de $D_A(M)$

M est noethérien L’ensemble ordonné D(M) est noethérien (E, III,

p. 51)

M est artinien L’ensemble D(M), ordonné par $\supset$, est noethérien

M est indécomposable On a $M\not= 0$ et il n’existe pas deux éléments $M'$ et

$M''$ de D(M), distincts de 0, vérifiant

inf(M$',M''$) $= 0$, sup(M$',M''$) $= M$.

M est de type fini Pour toute famille $(M_i)_{i\in I}$ dans D(M) de borne

supérieure M, il existe une partie finie J de I telle

que M = sup$_{j\in I}M_j$

M est simple Card(D(M)) = 2

M est semi-simple M est la borne supérieure, dans D(M), de l’ensemble des éléments minimaux de D(M) $-\{0\}$

Le module M est somme directe d’une famille $(M_i)_{i\in I}$ de sous-modules si et seulement si l’on a $M =\sum_{i\in I}M_i$ et $M_i\cap \sum_{j\not=i}M_j= 0$ pour tout $i\in I$. Cette remarque et l’examen de la table I donnent le résultat suivant.

#### Proposition 7 {#alg-viii-s6-prop-7 .statement tag=007E}

a) On a $\varphi (0) = 0$et $\varphi (V) = M$.

b) Soit $(V_i)_{i\in I}$ une famille de sous-modules de V. On a

$$
\varphi (\sum_{i\in I}V_i)=\sum_{i\in I}\varphi (V_i),\varphi (\bigcap_{i\in I}V_i)=\bigcap_{i\in I}\varphi (V_i)
$$

c) Le B-module V est somme directe de la famille $(V_i)_{i\in I}$ de sous-modules si et seulement si M est somme directe de la famille $(\varphi (V_i))_{i\in I}$.

Soient $V'$ et $V''$ des sous-modules de V tels que $V'$ soit contenu dans $V''$; posons $M'=\varphi (V')$ et $M''=\varphi (V'')$, de sorte que $M''$ contient $M'$. Notons $[V',V'']$ l’intervalle de D(V) formé des sous-modules W de V tels que l’on ait $V'\subset W\subset V''$, et définissons de même l’intervalle $[M',M'']$ de D(M). L’application $W\rightarrow W/V'$ est un isomorphisme d’ensembles ordonnés de $[V',V'']$ sur $D(V''/V')$; on définit de même un isomorphisme d’ensembles ordonnés de $[M',M'']$ sur $D(M''/M')$. Comme $\varphi$ applique l’intervalle $[V',V'']$ sur $[M',M'']$, il définit un isomorphisme $\varphi$ d’ensembles ordonnés de $D(V''/V')$ sur $D(M''/M')$. On déduit de cela et des tables I et II la proposition suivante :

#### Proposition 8 {#alg-viii-s6-prop-8 .statement tag=007F}

a) Soient $V'$ et $V''$ des sous-modules de V tels que $V''$ contienne $V'$. Le B-module $V''/V'$ est simple si et seulement si le A-module $\varphi (V'')/\varphi (V')$est simple.

b) Si $V'$ est un sous-module simple (resp. maximal, resp. facteur direct) de V, alors $\varphi (V')$est un sous-module simple (resp. maximal, resp. facteur direct) de M.

c) $\varphi$ transforme le socle $\mathscr{S}(V)$de V en le socle $\mathscr{S}(M)$de $M*$et le radical (VIII,

p. 147, définition 1$)\mathfrak{R}(V)$de V en le radical $\mathfrak{R}(M)$de M$.*$

d) Soit $(V_i)_{0\leqslant i\leqslant n}$ une suite finie de sous-modules de V. C’est une suite de Jordan-Hölder de V si et seulement si $(\varphi (V_i)_{0\leqslant i\leqslant n})$est une suite de Jordan-Hölder de M.

#### Lemme 2 {#alg-viii-s6-lem-2 .statement tag=007G}

Soient H et $H'$ des sous-modules de V tels que $H\cap H'= 0$. Pour que les B-modules H et $H'$ soient isomorphes, il faut et il suffit que les A-modules $\varphi (H)$ et $\varphi (H')$soient isomorphes.

Identifions $H + H'$ au produit $H\times H'$. Le graphe d’un isomorphisme de H sur $H'$ est un sous-module $H''$ de V satisfaisant à

$$
H\cap H''= H'\cap H''= 0H + H'= H + H''= H'+ H'' \tag{17}
$$

inversement, tout sous-module possédant ces propriétés est le graphe d’un isomorphisme de H sur $H'$. D’après la proposition 7, la relation $H\cap H'= 0$ équivaut à $\varphi (H)\cap \varphi (H') = 0$ et les relations (17) aux relations

$$
\varphi (H)\cap \varphi (H'') =\varphi (H')\cap \varphi (H'') = 0, \varphi (H) +\varphi (H') =\varphi (H) +\varphi (H'') =\varphi (H') +\varphi (H'')
$$

le lemme en résulte.

#### Proposition 9 {#alg-viii-s6-prop-9 .statement tag=00R6}

Soient S un sous-module simple de V et T le sous-module simple $\varphi (S)$de M. Si $V_S$ désigne le composant isotypique de type S dans V et $M_T$ le composant isotypique de type T dans M, on a $\varphi (V_S) = M_T$.

Tout sous-module simple $S'$ de V, distinct de S, satisfait à $S'\cap S = 0$. Il est donc isomorphe à S si et seulement si $\varphi (S')$ est isomorphe à T (lemme 2). Or $V_S$ est somme des sous-modules simples de V isomorphes à S et $M_T$ est somme des sous-modules simples de M isomorphes à T. La prop. 9 résulte aussitôt des prop. 7 et 8.

#### Proposition 10 {#alg-viii-s6-prop-10 .statement tag=007H}

a) Pour que le B-module V soit artinien, ou noethérien, ou indécomposable, ou simple, ou de type fini, il faut et il suffit qu’il en soit ainsi de M.

b) Pour que le B-module V soit de longueur finie, il faut et il suffit que le A-module M soit de longueur finie, et l’on a alors long$_B(V) =$ long$_A(M)$.

c) Pour que le B-module V soit semi-simple (resp. isotypique), il faut et il suffit que le A-module M soit semi-simple (resp. isotypique). S’il en est ainsi, on a long$_B(V) =$ long$_A(M)$.

L’assertion a) résulte de l’inspection de la table II.

L’assertion b) résulte de la prop. 8, d) (VIII, p. 104).

Le module V est semi-simple si et seulement s’il est égal à son socle $\mathscr{S}(V)$; il est isotypique si et seulement s’il existe un sous-module simple S de V tel que $V = V_S$. L’assertion c) résulte donc des prop. 7 c), 8 c) et 9 (VIII, p. 103 et 104).

### 6. Autres propriétés préservées par la correspondance de Morita

Soient A et B des $k$-algèbres équivalentes au sens de Morita et P un $(A,B)_k$-bimodule inversible.

#### Proposition 11 {#alg-viii-s6-prop-11 .statement tag=007I}

Soit

$$
(\mathscr{E})V'-\rightarrow^fV-\rightarrow^gV''
$$

un diagramme de B-modules et d’applications B-linéaires, et soit

$$
(P\otimes \mathscr{E})P\otimes_BV'\longrightarrow^{1_P\otimes f}P\otimes_BV\longrightarrow^{1_P\otimes g}P\otimes_BV''
$$

le diagramme correspondant de A-modules. Pour que $(\mathscr{E})$soit une suite exacte, il faut et il suffit que $(P\otimes \mathscr{E})$le soit.

Supposons la suite $(\mathscr{E})$ exacte. Comme le B-module à droite P est projectif, la suite $(P\otimes \mathscr{E})$ est exacte (II, p. 58, prop. 5 et p. 63, cor. 6).

Réciproquement, supposons la suite $(P\otimes \mathscr{E})$ exacte. Soient Q un $(B,A)_k$-bimodule inverse de P, et $\theta : Q\otimes_AP\rightarrow_sB_d$ un isomorphisme. Considérons le diagramme commutatif

$Q\otimes_AP\otimes_B{V'}^{1_Q\otimes 1_P\otimes f}/$/ $Q\otimes_AP\otimes_BV^{1_Q\otimes 1_P\otimes g}/$/ $Q\otimes_AP\otimes_BV''$

$\theta \otimes 1_{V'}\theta \otimes 1_V\theta \otimes 1_{V''}$

Puisque Q est un A-module projectif et que la suite (P$V'f$ // V $g\otimes \mathscr{E}$) est exacte, la première// $V''$ ligne de ce diagramme est une suite exacte ; comme les flèches verticales sont des isomorphismes, la seconde ligne est également exacte.

#### Corollaire {#alg-viii-s6-n6-cor-1 .statement tag=007J}

Soit $f: V\rightarrow W$une application B-linéaire. Pour que $f$ soit injective (resp. surjective), il faut et il suffit que $1_P\otimes f$ le soit.

#### Proposition 12 {#alg-viii-s6-prop-12 .statement tag=007K}

Soit V un B-module à gauche. Pour que le B-module V soit projectif (resp. générateur, resp. fidèle, $*$resp. injectif, resp. de présentation finie$*$), il faut et il suffit que le A-module $P\otimes_BV$le soit.

a) Supposons V projectif. Il existe un ensemble I tel que V soit isomorphe à un sous-module facteur direct de $B^{(I)}_s$. Le A-module $P\otimes_BV$ est alors isomorphe à un sous-module facteur direct de $P^{(I)}$; comme P est un A-module projectif, il en est de même de $P\otimes_BV$.

b) Supposons que le B-module V soit générateur. Soit M un A-module. Il existe un B-module W tel que M soit isomorphe à $P\otimes_BW$. Par le th. 1 de VIII, p. 76, il existe un ensemble I et une surjection $\varphi : V^{(I)}\rightarrow W$. Par le corollaire, l’application $1_P\otimes \varphi$ de $P\otimes (V^{(I})$ dans $P\otimes_AW$ est surjective, ce qui fournit une surjection de $(P\otimes V)^{(I)}\rightarrow M$. Par le th. 1 de VIII, p. 76, $P\otimes V$ est un A-module générateur.

c) Le B-module V est fidèle si et seulement si son annulateur est réduit à 0. L’assertion c) résulte donc de l’exemple 3 de VIII, p. 101.

$*$d) Supposons V injectif. D’après la remarque de VIII, p. 101 le A-module $P\otimes_BV$ est isomorphe à Hom$_B(Q,V)$, où Q est un $(B,A)_k$-bimodule inverse de A. Comme le A-module Q est projectif, donc plat (X, p. 9, exemple 1), le A-module Hom$_B(Q,V)$ est injectif en vertu de X, p. 18, prop. 11.

e) Supposons que V admette une présentation finie $L_1\rightarrow L_0\rightarrow V\rightarrow 0$ (X, p. 10). Par produit tensoriel avec P on en déduit une suite exacte de A-modules $N'_1-\rightarrow^uN'_0\rightarrow P\otimes_BV\rightarrow 0$, où $N'_1$ et $N'_0$ sont projectifs de type fini (prop. 11 et a)). Soit $N''_0$ un A-module de type fini tel que le module $N_0= N'_0\oplus N''_0$ soit libre de type fini, et soit $u': N'_1\oplus N''_0\rightarrow N_0$ l’homomorphisme $(u,1_{N''_0})$; alors $P\otimes_BV$ s’identifie au conoyau de $u'$. Soit $N_1$ un A-module libre de type fini et $p: N_1\rightarrow N'_1\oplus N''_0$ un homomorphisme surjectif ; la suite $N_1\longrightarrow^{u'\circ p}N_0\rightarrow P\otimes_BV\rightarrow 0$ est une présentation finie du A-module $P\otimes_BV.*$

f) Supposons le A-module $P\otimes_BV$ projectif (resp. générateur, resp. fidèle, $*$resp.

injectif, resp. de présentation finie$*)$. En appliquant ce qui précède (en échangeant les rôles de A et B, P et Q), on voit que le B-module $Q\otimes_AP\otimes_BV$ possède aussi cette propriété. Il en est donc de même du B-module V, qui lui est isomorphe.

#### Corollaire {#alg-viii-s6-n6-cor-2 .statement tag=007L}

Pour que l’anneau A soit artinien à gauche (resp. noethérien à gauche) il faut et il suffit que l’anneau B le soit.

Compte tenu de l’isomorphisme entre l’ensemble ordonné des idéaux à gauche de B et l’ensemble des sous-A-modules de P, pour que l’anneau B soit artinien à gauche (resp. noethérien à gauche), il faut et il suffit que le A-module P soit artinien (resp. noethérien). Mais par le th. 1 de VIII, p. 97, le A-module P est générateur et de type fini ; en particulier, $A_s$ est isomorphe à un facteur direct de $P^n$, pour un entier $n\geqslant 1$. Par suite P est artinien (resp. noethérien) si et seulement si A est artinien à gauche (resp. noethérien à gauche).

### 7. Équivalence de Morita des algèbres

#### Proposition 13 {#alg-viii-s6-prop-13 .statement tag=007M}

a) Si deux $k$-algèbres sont équivalentes au sens de Morita, leurs centres sont des $k$-algèbres isomorphes.

b) Pour que deux $k$-algèbres commutatives soient équivalentes au sens de Morita, il faut et il suffit qu’elles soient isomorphes.

c) Pour que deux $k$-algèbres qui sont des corps soient équivalentes au sens de Morita, il faut et il suffit qu’elles soient isomorphes.

d) Pour $i= 1,2$, soient $A_i$ et $B_i$ des $k$-algèbres équivalentes au sens de Morita, et $P_i$ un $(A_i,B_i)_k$-bimodule inversible. Posons $A = A_1\otimes_kA_2, B = B_1\otimes_kB_2$ et $P = P_1\otimes_kP_2$. Les $k$-algèbres A et B sont équivalentes au sens de Morita et P est un $(A,B)_k$-bimodule inversible.

e) Si A et B sont des $k$-algèbres équivalentes au sens de Morita et si $k'$ est une $k$-algèbre commutative, alors les $k'$-algèbres $A_{(k')}$ et $B_{(k')}$ sont équivalentes au sens de Morita.

L’assertion a) résulte du cor. 1 de VIII, p. 98 et b) en découle.

Soient K et L des $k$-algèbres qui sont des corps et soit P un $(K,L)_k$-bimodule inversible. Le L-espace vectoriel à droite P est un module simple (VIII, p. 100), donc de dimension 1, de sorte que les $k$-algèbres End$_L(P)$ et L sont isomorphes. D’après VIII, p. 97, th. 1, l’application $a\rightarrow a_P$ de K dans End$_L(P)$ est un isomorphisme. Donc les corps K et L sont isomorphes au-dessus de $k$, d’où c).

Sous les hypothèses de d), soient $Q_i(i= 1,2)$ un $(B_i,A_i)_k$-bimodule inverse de $P_i$; notons Q le $(B,A)_k$-bimodule $Q_1\otimes_kQ_2$. Considérons l’isomorphisme $k$-linéaire canonique $(P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)\longrightarrow (P_1\otimes_kQ_1)\otimes_k(P_2\otimes_kQ_2)$; il définit par passage aux quotients un isomorphisme

$$
(P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)\longrightarrow (P_1\otimes_{B_1}Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)
$$

qui est $(A$, A)-linéaire. Comme le $(A_i,A_i$)-bimodule $P_i\otimes_{B_i}Q_i$ est isomorphe à $A_i$, on obtient un isomorphisme $(A$, A)-linéaire $P\otimes_BQ\rightarrow A$. On obtient de même un isomorphisme $(B$, B)-linéaire $Q\otimes_AP\rightarrow B$, ce qui achève de prouver d).

Sous les hypothèses de e), soit P un $(A,B)_k$-bimodule inversible, alors $P_{(k')}$ est un $(A_{(k')},B_{(k')})_{k'}$-bimodule inversible.

Soit A une $k$-algèbre et soit $e$ un idempotent de A. L’ensemble $eAe$, muni de l’addition, de la multiplication et de l’action de $k$ induites par celles de A, est une $k$-algèbre, d’élément unité $e$.

#### Proposition 14 {#alg-viii-s6-prop-14 .statement tag=007N}

Soient A et B des $k$-algèbres. Pour que A et B soient équivalentes au sens de Morita, il faut et il suffit qu’il existe un entier $n\geqslant 1$et une matrice carrée $e= (e_{ij})$dans $\mathbf{M}_n(B)$satisfaisant aux conditions suivantes :

(i) On a $e^2=e$;

(ii) L’idéal bilatère de B engendré par les éléments $e_{ij}$ est égal à B ;

(iii) La $k$-algèbre A est isomorphe à $e\mathbf{M}_n(B)e$.

Si les conditions (i) et (ii) sont satisfaites, le $(e\mathbf{M}_n(B)e,B)_k$-bimodule $eB^n_d$ est inversible.

Compte tenu du th. 1 (VIII, p. 97), la $k$-algèbre A est équivalente à B au sens de Morita si et seulement si elle est isomorphe à l’algèbre des endomorphismes d’un B-module à droite projectif, de type fini et générateur. La proposition résulte donc des deux lemmes suivants.

#### Lemme 3 {#alg-viii-s6-lem-3 .statement tag=007O}

Pour qu’un B-module à droite P soit projectif, de type fini et générateur, il faut et il suffit qu’il existe un entier $n\geqslant 0$et un idempotent $e= (e_{ij})$dans $\mathbf{M}_n(B)$satisfaisant aux propriétés suivantes :

(i) Le B-module P est isomorphe à $eB^n_d$;

(ii) L’idéal bilatère de B engendré par les éléments $e_{ij}$ est égal à B.

Soit P un B-module à droite. Pour que P soit projectif et de type fini, il faut et il suffit qu’il soit isomorphe à un sous-module facteur direct d’un B-module de la forme $B^n_d$ où $n$ est un entier $\geqslant 0$ (II, p. 40, cor. 1). Si l’on identifie les $k$-algèbres $\mathbf{M}_n(B)$ et End(B$^n_d$), cela signifie qu’il existe un idempotent $e$ de $\mathbf{M}_n(B)$ tel que P soit isomorphe à $eB^n_d$.

Le B-module P est générateur si et seulement si son idéal trace $\tau (P)$ est égal à B, c’est-à-dire $\tau (eB^n_d) = B$ (VIII, p. 76, th. 1). Soient $x_1, . . . , x_n$ les éléments de $B^n_d$ correspondant aux colonnes de la matrice $e$, et soit $x^*_i$ (pour $1\leqslant i\leqslant n$) la forme linéaire $(b_1, . . . , b_n)\rightarrow b_i$ sur $eB^n_d$. La famille $(x_1, . . . , x_n)$ engendre le B-module $eB^n_d$ et la famille $(x^*_1, . . . , x^*_n)$ engendre son dual. Or on a $\langle x^*_i, x_j\rangle =e_{ij}$, donc $\tau (eB^n_d)$ est l’idéal bilatère de B engendré par les $e_{ij}$. Cela prouve le lemme 3.

#### Lemme 4 {#alg-viii-s6-lem-4 .statement tag=007P}

Soient V un B-module et E la $k$-algèbre des endomorphismes de V. Soit $e$ un projecteur de V et P l’image de $e$. L’application qui à $v\in eEe$ associe l’endomorphisme $x\rightarrow v(x)$du B-module P est un isomorphisme de $k$-algèbres de $eEe$ sur End$_B(P)$.

Notons $\varphi :eEe\rightarrow$ End$_B(P)$ l’application décrite dans l’énoncé ; c’est un homomorphisme de $k$-algèbres. Soit $u\in$ End$_B(P)$. Notons $v$ l’endomorphisme de V défini par $v(x) =u(e(x))$ pour $x\in V$. On a $(eve)(x) =u(x)$ pour $x\in P$, c’est-à-dire $\varphi (eve) =u$. Par suite, $\varphi$ est surjective. Soit $w$ un élément du noyau de $\varphi$; les restrictions de $w$ au noyau et à l’image de $e$ sont nulles, donc $w$ est nul, ce qui prouve que $\varphi$ est injective.

#### Exemple 1 {#alg-viii-s6-n7-exa-1 .statement tag=007Q}

Soient A une $k$-algèbre et $e$ un idempotent de A tel que $AeA = A$. La $k$-algèbre $eAe$ s’identifie à la $k$-algèbre des endomorphismes du sous-module $eA_d$ de $A_d$ (lemme 4). Comme $AeA = A$, il résulte de la prop. 14 que $eA_d$ est un $(eAe,A)_k$-bimodule inversible, donc que les $k$-algèbres $eAe$ et A sont équivalentes au sens de Morita. De plus, le théorème de Morita (VIII, p. 99) entraîne les résultats suivants :

a) Soient M et N des A-modules à gauche. Toute application $eAe$-linéaire de $eM$ dans $eN$ se prolonge de manière unique en une application A-linéaire de M dans N.

b) Tout module à gauche sur la $k$-algèbre $eAe$ est isomorphe à un module de la forme $eM$, où M est un A-module à gauche.

#### Exemple 2 {#alg-viii-s6-n7-exa-2 .statement tag=007R}

Soit A une $k$-algèbre et $n\geqslant 1$ un entier. Identifions l’algèbre de matrices $\mathbf{M}_n(A)$ à l’algèbre des endomorphismes du A-module à droite $A^n_d$. On a vu que A et $\mathbf{M}_n(A)$ sont équivalentes au sens de Morita. Pour tout A-module à gauche M, identifions $A^n_d\otimes_AM$ à $M^n$. L’algèbre $\mathbf{M}_n(A)$ opère alors à gauche sur $M^n$, et l’on a

$$
(a\cdot m)_i=\sum_{j=1}^na_{ij}m_j
$$

pour $a= (a_{ij})$ dans $\mathbf{M}_n(A)$ et $m= (m_i)$ dans $M^n$. Le théorème de Morita entraîne les résultats suivants :

a) Tout module à gauche sur l’algèbre $\mathbf{M}_n(A)$ est isomorphe à un module de la forme $M^n$, où M est un A-module à gauche.

b) Soit M un A-module à gauche. L’application $N\rightarrow N^n$ est une bijection de l’ensemble des sous-A-modules de M sur l’ensemble des sous-$\mathbf{M}_n$(A)-modules de $M^n$.

c) Soient M et N des A-modules à gauche. Pour toute application A-linéaire $g: M\rightarrow N$, soit $g_n$ l’application $(m_i)\rightarrow (g(m_i))$ de $M^n$ dans $N^n$. Alors l’application $g\rightarrow g_n$ est une bijection de Hom$_A(M,N)$ sur Hom$_{\mathbf{M}_n(A)}(M^n,N^n)$.

d) Soit M un A-module à gauche. Pour que le module $M^n$ sur l’anneau $\mathbf{M}_n(A)$ soit indécomposable, ou semi-simple, ou simple, ou artinien, ou noethérien, ou de type fini, il faut et il suffit qu’il en soit ainsi du A-module M.

#### Exemple 3 {#alg-viii-s6-n7-exa-3 .statement tag=007S}

Soient A un anneau principal et L un A-module libre de type fini non nul. Soit B l’anneau des endomorphismes de L ; alors L est un $(A,B)_{\mathbf{Z}}$-bimodule inversible et les anneaux A et B sont équivalents au sens de Morita. D’après le théorème de Morita, la prop. 10, a) (VIII, p. 104) et le théorème de structure des A-modules de type fini (VII, p. 19, th. 2), tout B-module de type fini est isomorphe à $\oplus^m_{i=1}(L/\mathfrak{a}_iL)$, où $m$ est un entier positif et les $\mathfrak{a}_i$ des idéaux de A vérifiant $\mathfrak{a}_1\subset \mathfrak{a}_2\subset  \cdots  \subset \mathfrak{a}_m$ et $\mathfrak{a}_n\not= A$; l’entier $m$ et les idéaux $\mathfrak{a}_i$ sont déterminés de façon unique. D’après la proposition 6 de VIII, p. 101, tout idéal bilatère de B est de la forme $dB$ où $d$ est un élément de A.

## EXERCICES {#alg-viii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
