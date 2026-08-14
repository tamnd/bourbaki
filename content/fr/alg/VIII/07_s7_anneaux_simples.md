---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 7
section_title: Anneaux simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.115-A VIII.129
pdf_pages: 0123-0137
extraction: native
subsections:
    - "no": 1
      title: Anneaux simples
      page: 115
      pdf_page: 123
    - "no": 2
      title: Modules sur un anneau simple
      page: 118
      pdf_page: 126
    - "no": 3
      title: Degrés
      page: 120
      pdf_page: 128
    - "no": 4
      title: Idéaux des anneaux simples
      page: 122
      pdf_page: 130
statements: 24
exercises: 16
content_sha256: b72c918f126c4b4d2cd5d6b619af8ff04f06dc17e2232d98a8287e35038e3263
---

## § 7. ANNEAUX SIMPLES

### 1. Anneaux simples

#### Proposition 1 {#alg-viii-s7-prop-1 .statement tag=0081}

Soit A un anneau non nul. Les conditions suivantes sont équivalentes :

(i) Le A-module $A_s$ est isotypique ;

(ii) L’anneau A est artinien à gauche et tout idéal bilatère de A est égal à 0 ou à A ;

(iii) L’anneau A est artinien à gauche et il existe un A-module à gauche S qui est simple et fidèle.

Si ces conditions sont satisfaites, le A-module $A_s$ est de longueur finie et isotypique de type S, et tout A-module simple est isomorphe à S.

Démontrons que (i) entraîne (ii). Sous les hypothèses de (i), le A-module de type fini $A_s$ est semi-simple, donc de longueur finie et artinien (VIII, p. 67, prop. 10) ; par suite, l’anneau A est artinien à gauche. Les endomorphismes du A-module à gauche $A_s$ sont les multiplications à droite par les éléments de A. Comme le A-module à gauche $A_s$ est isotypique, il résulte de la prop. 6, b) de VIII, p. 81, que le $(A,A)$-bimodule $_sA_d$ est simple. Les sous-bimodules de $_sA_d$ sont les idéaux bilatères de A, donc (i) implique (ii).

Démontrons que (ii) entraîne (iii). L’anneau A n’est pas réduit à 0 ; par suite, il existe un A-module simple S. L’annulateur de S est un idéal bilatère de A, distinct de A. Sous les hypothèses de (ii), il est égal à 0. Le A-module S est alors fidèle et (ii) entraîne (iii).

Démontrons que (iii) entraîne (i). Sous les hypothèses de (iii), il existe un entier $m\geqslant 1$ tel que $A_s$ soit isomorphe à un sous-module de $S^m$ (VIII, p. 46, prop. 5, a)). Puisque $S^m$ est un A-module isotypique de type S, il en est de même de $A_s$ (VIII, p. 57, prop. 2) ; donc (iii) implique (i).

Supposons les conditions (i) à (iii) satisfaites. Nous avons vu au cours de la démonstration que le A-module $A_s$ est de longueur finie et isotypique de type S. Tout A-module à gauche simple est isomorphe à un quotient de $A_s$, donc à S.

#### Définition 1 {#alg-viii-s7-def-1 .statement tag=0082}

On dit que l’anneau A est simple s’il satisfait aux conditions équivalentes (i), (ii) et (iii) de la proposition 1. Soit K un corps commutatif ; une K-algèbre est dite simple si son anneau sous-jacent est simple.

#### Remarque 1 {#alg-viii-s7-n1-rem-1 .statement tag=0083}

Rappelons que d’après le th. 1 de I, p. 109, les conditions suivantes sont équivalentes :

(i) Le A-module $A_s$ est simple ;

(ii) L’anneau A n’est pas réduit à 0, et il n’existe aucun idéal à gauche de A distinct de 0 et de A ;

(iii) L’anneau A est un corps.

Par conséquent, compte tenu de la condition (ii) de la prop. 1, les anneaux simples commutatifs ne sont autres que les corps commutatifs.

#### Remarque 2 {#alg-viii-s7-n1-rem-2 .statement tag=0084}

☡ On dit parfois qu’un anneau A est quasi-simple s’il n’est pas réduit à 0 et si ses seuls idéaux bilatères sont 0 et A. On dit que A est primitif s’il possède un module simple et fidèle. D’après la prop. 1, tout anneau simple est quasi-simple. Comme tout anneau non réduit à 0 possède un module simple et que l’annulateur d’un module simple est un idéal bilatère, on voit que tout anneau quasi-simple est primitif. Cependant, il existe des anneaux quasi-simples qui ne sont pas simples, et des anneaux primitifs qui ne sont pas quasi-simples (VIII, p. 124, exerc. 2) ; de tels anneaux ne sont pas artiniens à gauche.

#### Théorème 1 (Wedderburn) {#alg-viii-s7-thm-1 .statement tag=00S3}

Pour qu’un anneau soit simple, il faut et il suffit qu’il soit isomorphe à un anneau de matrices $\mathbf{M}_r(D)$, où $r\geqslant 1$est un entier et D un corps.

#### Lemme 1 {#alg-viii-s7-lem-1 .statement tag=0085}

Soient A un anneau simple, S un A-module à gauche simple et D l’anneau opposé du corps End$_A(S)$. Alors S est un $(A,D)$-bimodule inversible. C’est aussi un espace vectoriel à droite de dimension finie sur D et l’application $a\rightarrow a_S$ est un isomorphisme d’anneaux de A sur End$_D(S)$.

D’après la prop. 1 de VIII, p. 115, le A-module $A_s$ est de longueur finie, et isotypique de type S. Il existe donc un entier $m\geqslant 1$ tel que les A-modules $A_s$ et $S^m$ soient isomorphes. Alors le A-module S est projectif et de type fini. Il est générateur (VIII, p. 76, th. 1) et le lemme 1 résulte du th. 1 de VIII, p. 97, (ii)$\Rightarrow$(i) et (ii)$\Rightarrow$(iii) appliqué au $(A,D)_{\mathbf{Z}}$-bimodule S.

#### Lemme 2 {#alg-viii-s7-lem-2 .statement tag=00R7}

Soient D un corps et V un espace vectoriel à droite de dimension finie $r\geqslant 1$sur le corps D. Alors V est un module simple sur l’anneau E = End$_D(V)$et son commutant est égal à $D_V$. L’anneau E est simple et sa longueur à gauche est égale à $r$.

On sait que V est un E-module simple (VIII, p. 41, exemple 3) et que son commutant est égal à $D_V$ (VIII, p. 78, cor. 1). Soit $(x_i)_{1\leqslant i\leqslant r}$ une base de V sur le corps D. L’application $u\rightarrow (u(x_i))_{1\leqslant i\leqslant r}$ est un isomorphisme du E-module $E_s$ sur le E-module $V^r$; par suite, le E-module $E_s$ est isotypique de longueur $r$, donc l’anneau E est simple.

Démontrons maintenant le théorème 1. Rappelons (II, p. 150) que l’anneau $\mathbf{M}_r(D)$ s’identifie à l’anneau des endomorphismes du D-espace vectoriel à droite $D^r_d$; de plus, tout espace vectoriel à droite de dimension finie $r$ sur un corps D est isomorphe à $D^r_d$ (II, p. 97). Le théorème 1 résulte donc des lemmes 1 et 2.

#### Remarque 3 {#alg-viii-s7-n1-rem-3 .statement tag=0086}

Soit A un anneau simple, soient S un A-module simple et D l’anneau opposé du corps End$_A(S)$. Alors le A-module $A_s$ est de longueur finie et dim$_D(S)$ est égal à long(A). En effet, par le lemme 1, l’anneau A est isomorphe à End$_D(S)$ et on applique le lemme 2.

#### Corollaire 1 {#alg-viii-s7-lem-2-cor-1 .statement tag=0087}

a) Le centre d’un anneau simple est un corps.

b) L’anneau opposé d’un anneau simple est simple.

c) La longueur à gauche d’un anneau simple est égale à sa longueur à droite.

Soient D un corps, Z son centre et V un espace vectoriel à droite sur le corps D, de dimension finie $r\geqslant 1$. On note E l’anneau des endomorphismes de V.

L’application $z\rightarrow z_V$ est un isomorphisme de Z sur le centre de E d’après le corollaire 2 de VIII, p. 78. L’assertion a) résulte de là. Le dual $V^*$ de V est un espace vectoriel à droite sur le corps $D^o$ opposé de D et sa dimension est égale à $r$. L’application $u\rightarrow^tu$ est un isomorphisme de l’anneau $E^o$ opposé de E sur l’anneau End$_{D^o}(V^*)$. Par suite, l’anneau $E^o$ est simple et les anneaux E et $E^o$ ont la même longueur à gauche, égale à $r$ (lemme 2).

#### Corollaire 2 {#alg-viii-s7-lem-2-cor-2 .statement tag=0088}

Soient $r$ et $r'$ des entiers strictement positifs et soient D et $D'$ des corps. Pour que les anneaux $\mathbf{M}_r(D)$et $\mathbf{M}_{r'}(D')$soient isomorphes, il faut et il suffit que l’on ait $r=r'$ et que les corps D et $D'$ soient isomorphes.

La condition est évidemment suffisante.

Réciproquement, supposons que les anneaux $B = \mathbf{M}_r(D)$ et $B'= \mathbf{M}_{r'}(D')$ soient isomorphes. Comme $r$ est la longueur de $B_s$ et $r'$ celle de $B'_s$ (lemme 2), on a $r=r'$. De plus, B est équivalent à D au sens de Morita et $B'$ à $D'$ (VIII, p. 98, exemple 1). Par suite, les corps D et $D'$ sont équivalents au sens de Morita, donc isomorphes (VIII, p. 107, prop. 13, c)).

#### Corollaire 3 {#alg-viii-s7-lem-2-cor-3 .statement tag=0089}

Soit K un corps commutatif et soit A une K-algèbre de degré fini dont l’anneau sous-jacent est simple. Il existe un entier $r$ et une K-algèbre D de degré fini sur K qui est un corps tels que A soit isomorphe à $M_r(D)$. En particulier, si K est algébriquement clos, A est isomorphe à une algèbre de matrices sur K.

Soit S un A-module à gauche simple ; c’est un K-espace vectoriel de dimension finie sur K. Son commutant est donc une algèbre de degré fini sur K. La première assertion résulte alors du lemme 1. Si K est algébriquement clos, alors D = K par le th. 1 de VIII, p. 43.

#### Remarque 4 {#alg-viii-s7-n1-rem-4 .statement tag=008A}

Soit K un corps commutatif algébriquement clos et soit A une algèbre de degré fini sur K. L’algèbre A est simple si et seulement s’il existe un entier $n\geqslant 1$ tel que A soit isomorphe à $M_n(K)$. Son centre est alors isomorphe à K.

### 2. Modules sur un anneau simple

#### Lemme 3 {#alg-viii-s7-lem-3 .statement tag=008B}

Soit A un anneau simple et soit S un A-module simple. Notons D le corps opposé du commutant de S. Tout A-module est isomorphe à un A-module de la forme $S\otimes_DV$, où V est un espace vectoriel à gauche sur le corps D.

Cela résulte du lemme 1 de VIII, p. 116 et du théorème de Morita (VIII, p. 99).

#### Proposition 2 {#alg-viii-s7-prop-2 .statement tag=008C}

Soient A un anneau simple et S un A-module simple.

a) Tout A-module est projectif et isotypique de type S, donc semi-simple. Si $\mathfrak{a}$ est sa longueur, il est isomorphe à $S^{(\mathfrak{a})}$.

b) Tout A-module non nul est générateur.

c) Deux A-modules sont isomorphes si et seulement s’ils ont même longueur.

Notons D le corps opposé du commutant de S. D’après le lemme 1 de VIII, p. 116, S est un $(A$, D)-bimodule inversible. Soit M un A-module ; d’après le lemme 3, il est isomorphe à un module de la forme $S\otimes_DV$, où V est un espace vectoriel à gauche sur le corps D.

Le D-module V est projectif et isotypique de type $D_s$; il est générateur si et seulement s’il n’est pas réduit à 0. Enfin, la longueur de $S\otimes_DV$ est égale à la dimension du D-espace vectoriel V, et deux espaces vectoriels sont isomorphes si et seulement s’ils ont même dimension. La prop. 2 résulte de là, compte tenu de la prop. 10 de VIII, p. 104 et de la prop. 12 de VIII, p. 106.

Soit $r\geqslant 1$ un entier. Nous dirons qu’un cardinal $\mathfrak{a}$ est divisible par $r$ s’il existe un cardinal $\mathfrak{b}$ tel que $\mathfrak{a}=r\mathfrak{b}$. Il en est ainsi si $\mathfrak{a}$ est infini, puisqu’on a $r\mathfrak{a}=\mathfrak{a}$ (E, III, p. 49, cor. 3) ; il résulte de cette remarque que si le cardinal $\mathfrak{a}$ est divisible par $r$, il existe un unique cardinal $\mathfrak{b}$ tel que $\mathfrak{a}=r\mathfrak{b}$.

#### Corollaire {#alg-viii-s7-n2-cor-1 .statement tag=008D}

Soit $k$ un corps commutatif et soit A une $k$-algèbre simple de degré fini sur $k$. Tout A-module simple est de dimension finie sur $k$;pour que deux A-modules soient isomorphes, il faut et il suffit que leur dimension sur $k$ soient égales.

Tout A-module simple sur A est isomorphe à un quotient de $A_s$, donc de dimension finie sur $k$. Le corollaire résulte alors de la prop. 2, c) de VIII, p. 118.

#### Proposition 3 {#alg-viii-s7-prop-3 .statement tag=008E}

Soit A un anneau simple. Pour qu’un A-module M soit libre, il faut et il suffit que sa longueur soit divisible par la longueur de A. S’il en est ainsi, toutes les bases de M ont le même cardinal, noté dim$_A(M)$ (II, p. 98, remarque 2), et caractérisé par la relation

(1) long$_A(M) =$ long(A)$\cdot$ dim$_A(M)$.

Supposons que M soit libre et soit $(e_i)_{i\in I}$ une base de M. Le A-module M est somme directe des A-modules $Ae_i$, eux-mêmes isomorphes à $A_s$. Posons $r=$ long$_A(A_s)$; c’est un entier supérieur ou égal à 1 (VIII, p. 115, prop. 1). On a long$_A(M) =r$ Card(I) d’après la formule (13) de VIII, p. 68.

Réciproquement, supposons que le cardinal long$_A(M)$ soit divisible par $r$. Soit $\mathfrak{a}$ le cardinal tel que long$_A(M) =r\mathfrak{a}$. Alors le A-module M a même longueur que $A^{(\mathfrak{a})}_s$, donc lui est isomorphe d’après la prop. 2. Ceci prouve que M est libre.

#### Proposition 4 {#alg-viii-s7-prop-4 .statement tag=008F}

Soient A un anneau simple et M un A-module non nul. Notons B l’anneau des endomorphismes du A-module M, et considérons M comme un B-module à gauche.

a) L’application $a\rightarrow a_M$ est un isomorphisme de A sur l’anneau des endomorphismes du B-module M.

b) Supposons que M soit de longueur finie comme A-module. Alors l’anneau B est simple et l’on a

(2) long$_A(M) =$ long(B) et long$_B(M) =$ long(A).

Le A-module M est générateur d’après la prop. 2 de VIII, p. 118 ; on a par définition $B = A'_M$ et l’assertion a) résulte donc du th. 2 de VIII, p. 78.

Supposons que M soit un A-module de longueur finie. Choisissons un A-module simple S et notons D le corps opposé de l’anneau des endomorphismes de S. D’après le lemme 3 le A-module M est isomorphe à un module de la forme $S\otimes_DV$ où V est un espace vectoriel à gauche sur le corps D. L’espace vectoriel V est de dimension finie. D’après le th. 3 de VIII, p. 60, l’anneau B est isomorphe à End$_D(V)$; d’après le lemme 2 (VIII, p. 117) l’anneau B est donc simple et, compte tenu de la remarque 1 de VIII, p. 59, on obtient les égalités

long(B) = dim$_D(V) =$ long$_A(M)$.

Par la remarque 1 de VIII, p. 59 et la remarque 3 de VIII, p. 117, on a les relations

long$_B(M) =$ long$_{End_D(V)}(S\otimes_DV) =$ dim$_D(S) =$ long(A)

ce qui démontre la dernière formule.

### 3. Degrés

Considérons un anneau B et un sous-anneau A de B. On munit B de la structure de $(A$, A)-bimodule déduite par restriction des scalaires de la structure de $(B,B)$-bimodule de $_sB_d$.

#### Proposition 5 {#alg-viii-s7-prop-5 .statement tag=008G}

Soit B un anneau, soit A un sous-anneau simple de B et soit S un A-module à gauche simple. Alors B est un A-module à gauche libre de dimension long$_A(B\otimes_AS)$.

Soit $r$ la longueur de A ; le A-module $A_s$ est isomorphe à $S^r$. Or le A-module à gauche B est isomorphe à $B\otimes_AA_s$ (II, p. 56), donc à $(B\otimes_AS)^r$ (II, p. 61, prop. 7). On a donc long$_A(B) =r$ long$_A(B\otimes_AS)$, et la prop. 5 résulte de la prop. 3 de VIII, p. 119.

#### Définition 2 {#alg-viii-s7-def-2 .statement tag=008H}

Soient B un anneau, A un sous-anneau simple de B. On appelle degré (à gauche) de B sur A, et l’on note [^1] $[B : A]_s$, la dimension du A-module à gauche libre B.

En remplaçant A et B par les anneaux opposés, on déduit de ce qui précède que B est un A-module à droite libre ; on notera $[B : A]_d$ sa dimension, et on l’appellera le degré à droite de B sur A.

☡ On peut donner un exemple d’un corps B et d’un sous-corps A tels que les degrés $[B : A]_s$ et $[B : A]_d$ soient distincts[^2].

Soit B un anneau, soit A un sous-anneau simple de B et soit S un A-module à gauche simple. Soient M un A-module à gauche et $\mathfrak{a}$ sa longueur. Les A-modules M et $S^{(\mathfrak{a})}$ sont isomorphes (VIII, p. 118, prop. 2), donc les B-modules $B\otimes_AM$ et $(B\otimes_AS)^{(\mathfrak{a})}$ sont isomorphes. De la prop. 5 et de la définition 2, on déduit la relation

(3) long$_A(B\otimes_AM) = [B : A]_s$ long$_A(M)$.

#### Proposition 6 {#alg-viii-s7-prop-6 .statement tag=008I}

Soient C un anneau, B un sous-anneau simple de C, et A un sous-anneau simple de B. On a alors $[C : A]_s= [C : B]_s[B : A]_s$.

Introduisons une base $(e_i)_{i\in I}$ de C considéré comme B-module à gauche, et une base $(f_j)_{j\in J}$ de B considéré comme A-module à gauche. Alors la famille $(f_je_i)_{j\in J,i\in I}$ est une base de C considéré comme A-module à gauche (II, p. 31, prop. 25), d’où la prop. 6.

#### Remarque 1 {#alg-viii-s7-n3-rem-1 .statement tag=008J}

Supposons que A soit un sous-anneau simple d’un anneau simple B et que le degré à droite $[B : A]_d$ soit fini. Soit C l’anneau des endomorphismes de B considéré comme A-module à droite ; c’est un anneau simple d’après la prop. 4, b) de VIII, p. 119. Pour tout $b$ dans B, soit $\gamma (b)$ l’application $x\rightarrow bx$ de B dans B ; alors $\gamma :b\rightarrow \gamma (b)$ est un isomorphisme de B sur un sous-anneau de C. De plus, si $(x_1, . . . , x_m)$ est une base du A-module à droite B, le morphisme qui applique $c$ sur $(c(x_1), . . . , c(x_m))$ est un isomorphisme de B-modules à gauche de C sur $B^m_s$, d’où la relation

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

Compte tenu de la formule (2) de VIII, p. 119 appliquée au A-module à droite B, on a

(5) long(C) $= [B : A]_d$ long(A).

#### Remarque 2 {#alg-viii-s7-n3-rem-2 .statement tag=008K}

Soit K un corps commutatif. Si A est une sous-algèbre simple d’une algèbre B, de degré fini sur K, le degré à gauche de B sur A satisfait à la relation $[B : A]_s[A : K] =$ [B : K] d’après la prop. 6 de VIII, p. 121. On a de même $[B : A]_d[A : K] = [B : K]$, d’où l’égalité $[B : A]_s= [B : A]_d$.

### 4. Idéaux des anneaux simples

Soient D un corps et V un espace vectoriel à droite sur le corps D, de dimension finie $n\geqslant 1$. On considère l’anneau simple A = End$_D(V)$. Pour tout sous-espace vectoriel W de V, on note $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W))$ l’ensemble des éléments $a$ de A satisfaisant $aW = 0$ (resp. $aV\subset W)$.

#### Proposition 7 {#alg-viii-s7-prop-7 .statement tag=008L}

a) L’application $W\rightarrow \mathfrak{a}(W)$est une bijection de l’ensemble des sous-espaces vectoriels de V sur l’ensemble des idéaux à gauche de A.

b) L’application $W\rightarrow \mathfrak{b}(W)$est une bijection de l’ensemble des sous-espaces vectoriels de V sur l’ensemble des idéaux à droite de A.

c) Soient $W_1$ et $W_2$ des sous-espaces vectoriels de V. Les relations $W_1\subset W_2$, $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$et $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$sont équivalentes.

L’assertion b) résulte de l’exemple 1, b) de VIII, p. 100 appliquée au $(D^o,A^o)$-bimodule inversible V, de même que l’équivalence des relations $W_1\subset W_2$ et $\mathfrak{b}(W_1)\subset$ $\mathfrak{b}(W_2)$.

Soit $V^*$ le dual de V, considéré comme espace vectoriel à droite sur le corps $D^o$ opposé de D. Pour tout sous-espace W de V, notons $W'$ l’orthogonal de W dans $V^*$. L’application $W\rightarrow W'$ est une bijection de l’ensemble des sous-espaces de V sur l’ensemble des sous-espaces de $V^*$. Si $W_1$ et $W_2$ sont deux sous-espaces de V, les relations $W_1\subset W_2$ et $W_1'\supset W'_2$ sont équivalentes. Or, l’application $u\rightarrow^tu$ est un isomorphisme de A sur l’anneau opposé de End$_{D^o}(V^*)$; elle transforme idéaux à gauche de A en idéaux à droite de End$_{D^o}(V^*)$, et $\mathfrak{a}(W)$ en l’ensemble $\mathfrak{b}(W')$ des endomorphismes $h$ de $V^*$ tels que $h(V^*)\subset W'$. L’assertion a), ainsi que l’équivalence des relations $W_1\subset W_2$ et $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, résultent alors de l’assertion analogue à b) pour le dual $V^*$ de V.

#### Corollaire {#alg-viii-s7-n4-cor-1 .statement tag=008M}

a) Les idéaux à gauche minimaux de A sont les idéaux $\mathfrak{a}(H)$, où H est un hyperplan de V ; les idéaux à gauche maximaux de A sont les idéaux $\mathfrak{a}(L)$, où L est une droite de V ;

b) Les idéaux à droite minimaux de A sont les idéaux $\mathfrak{b}(L)$, où L est une droite de V ; les idéaux à droite maximaux de A sont les idéaux $\mathfrak{b}(H)$, où H est un hyperplan de V.

Soit $(L_i)_{i\in I}$ une famille de droites dont V soit somme directe. Soit $(\varepsilon_i)_{i\in I}$ la famille de projecteurs associée à la décomposition $V =\oplus_{i\in I}L_i$. Les $\varepsilon_i$ sont des idempotents dans A, on a $\varepsilon_i\varepsilon_j= 0$ pour $i\not=j$ et $\sum_{i\in I}\varepsilon_i= 1$. Notons $H_i$ l’hyperplan $\sum_{j\not=i}L_j$; c’est le noyau de $\varepsilon_i$. On a alors

$$
\mathfrak{a}(H_i) = A\varepsilon_i,\mathfrak{b}(L_i) =\varepsilon_iA
$$

Le A-module $A_s$ est somme directe de la famille $(\mathfrak{a}(H_i))_{i\in I}$ d’idéaux à gauche minimaux, et $A_d$ est somme directe de la famille $(\mathfrak{b}(L_i))_{i\in I}$ d’idéaux à droite minimaux.

Considérons le cas particulier $V = (D_d)^n$ et identifions A à l’anneau de matrices $\mathbf{M}_n(D)$. Notons I l’intervalle $[1, n]$ de $\mathbf{N}$et $(v_i)_{i\in I}$ la base canonique de V ; posons $L_i=v_iD$, et notons $E_{ij}$ les unités matricielles (II, p. 142). On a alors $\varepsilon_i= E_{ii}$. L’idéal à gauche AE$_{ii}$ est égal à DE$_{1i}+\cdots +$ DE$_{ni}$ et se compose des matrices dont toutes les colonnes à l’exception de la $i$-ème sont nulles. L’idéal à droite $E_{ii}A$ est égal à DE$_{i1}+\cdots +$ DE$_{in}$ et se compose des matrices dont toutes les lignes à l’exception de la $i$-ème sont nulles. On a aussi la relation

$$
E_{ii}A E_{jj}= E_{ii}A\cap A E_{jj}= D E_{ij}
$$

pour $i$ et $j$ compris entre 1 et $n$.

## EXERCICES {#alg-viii-s7-exercises}

See the [exercises for § 7](exercises/s7/).

[^1]: Si A et B sont des corps commutatifs, on prendra soin de ne pas confondre le degré qui est égal à [B : A] avec le degré séparable de l’extension B de A, défini en V, p. 30, et noté aussi $[B : A]_s$.
[^2]: cf. A. H. Schofield, Artin’s problem for skew field extensions, Math. Proc. Cambridge Philos. Soc. **97** (1985), p. 1–6.
