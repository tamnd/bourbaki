---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 12
section_title: Produit tensoriel de modules semi-simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.207-A VIII.224
pdf_pages: 0211-0228
extraction: native
subsections:
    - "no": 1
      title: Modules semi-simples sur un produit tensoriel d’algèbres
      page: 207
      pdf_page: 211
    - "no": 2
      title: Produit tensoriel de modules simples
      page: 209
      pdf_page: 213
    - "no": 3
      title: Produit tensoriel d’algèbres commutatives semi-simples
      page: 211
      pdf_page: 215
    - "no": 4
      title: Radical d’un produit tensoriel d’algèbres
      page: 213
      pdf_page: 217
    - "no": 5
      title: Produit tensoriel de modules semi-simples
      page: 214
      pdf_page: 218
    - "no": 6
      title: Produit tensoriel d’algèbres semi-simples
      page: 217
      pdf_page: 221
    - "no": 7
      title: Extension des scalaires dans les modules semi-simples
      page: 217
      pdf_page: 221
statements: 26
exercises: 17
content_sha256: 9e42892d72dc2ab26c82028829284468e5686373270b4f69406c6225b1a5cc75
---

## § 12. PRODUIT TENSORIEL DE MODULES SEMI-SIMPLES

Dans ce paragraphe, la lettre K désigne un corps commutatif. Si E et F sont des espaces vectoriels sur K, on note $E\otimes F$le produit tensoriel $E\otimes_KF$.

### 1. Modules semi-simples sur un produit tensoriel d’algèbres

Dans ce numéro, on considère des K-algèbres $A_1$ et $A_2$; on note A l’algèbre $A_1\otimes A_2$.

#### Proposition 1 {#alg-viii-s12-prop-1 .statement tag=00E6}

Soient $M_1$ un $A_1$-module et $M_2$ un $A_2$-module, tous deux non réduits à 0. Si le module $M = M_1\otimes M_2$ sur l’anneau $A = A_1\otimes A_2$ est simple (resp. isotypique, resp. semi-simple), le $A_1$-module $M_1$ et le $A_2$-module $M_2$ sont simples (resp. isotypiques, resp. semi-simples).

Supposons que M soit un A-module semi-simple. Soit $N_1$ un sous-A$_1$-module de $M_1$. Notons N l’image canonique de $N_1\otimes M_2$ dans le A-module M. D’après le cor. 2 de VIII, p. 52, il existe un projecteur A-linéaire $p$ dans M, d’image N. On a par hypothèse $M_2\not= 0$; on peut donc choisir un élément $m$ de $M_2$ et une forme linéaire $\varphi$ sur le K-espace vectoriel $M_2$, tels que $\varphi (m) = 1$ (II, p. 105, cor. 2). Soit $u$ l’application de $M_1$ dans M définie par $u(m_1) =m_1\otimes m$ et soit $v$ l’application K-linéaire de M dans $M_1$ caractérisée par $v(m_1\otimes m_2) =\varphi (m_2)m_1$. Posons $q=v\circ p\circ u$. L’application $q: M_1\rightarrow M_1$ est $A_1$-linéaire, son image est contenue dans $N_1$ et on a $q(n) =n$ pour tout $n\in N_1$. Par suite $q$ est un projecteur dans $M_1$ d’image $N_1$. On a prouvé que $M_1$ est un $A_1$-module semi-simple (VIII, p. 52, cor. 2).

Supposons que M soit simple et que $M_1$ soit somme directe de deux sous-A$_1$-modules $M'_1$ et $M''_1$. Posons $M'= M'_1\otimes M_2$ et $M''= M''_1\otimes M_2$; alors M est somme directe des sous-A-modules $M'$ et $M''$. Comme M est simple, $M'$ ou $M''$ est réduit à 0 ; comme on a $M_2\not= 0$ par hypothèse, on a $M'_1= 0$ ou $M''_1= 0$ (II, p. 62, cor. 2). Cela prouve que $M_1$ est un $A_1$-module simple.

Supposons maintenant que M soit un A-module isotypique. Soient S et T des sous-A$_1$-modules simples de $M_1$. Les A-modules $S\otimes M_2$ et $T\otimes M_2$ s’identifient à des sous-modules non nuls de M. Ils sont donc isotypiques de même type que M. D’après la remarque de VIII, p. 57, il existe une application A-linéaire non nulle $f: S\otimes M_2\rightarrow T\otimes M_2$. L’application $f$ est en particulier $A_1$-linéaire. Comme les $A_1$-modules $S\otimes M_2$ et $T\otimes M_2$ sont non nuls et isotypiques de type S et T respectivement, S et T sont isomorphes. Cela prouve que $M_1$ est un $A_1$-module isotypique.

#### Proposition 2 {#alg-viii-s12-prop-2 .statement tag=00E7}

Soit S un module simple sur l’anneau $A = A_1\otimes A_2$ et de dimension finie sur K. Pour $i\in  \{1,2\}$, il existe un $A_i$-module simple $S_i$ tel que le $A_i$-module S soit isotypique de type $S_i$. Le A-module S est isomorphe à un quotient du A-module $S_1\otimes S_2$.

Comme S est un $A_1$-module de dimension finie non nulle sur K, il est de longueur finie sur $A_1$ et il existe un $A_1$-module à gauche simple $S_1$ et une application $A_1$-linéaire non nulle de $S_1$ dans S. Munissons $M_2=$ Hom$_{A_1}(S_1,S)$ de la structure de $A_2$-module à gauche définie par la loi d’action $(a_2, u)\rightarrow (a_2)_S\circ u$. On a $M_2\not= 0$ par construction et $M_2$ est de dimension finie sur K. On peut donc trouver un $A_2$-module à gauche simple $S_2$ et une application $A_2$-linéaire non nulle $\varphi : S_2\rightarrow M_2$. On définit une application A-linéaire non nulle $\psi$ de $S_1\otimes S_2$ dans S telle que l’on ait

$$
\psi (s_1\otimes s_2) =\varphi (s_2)(s_1)
$$

pour tout $s_1\in S_1$ et tout $s_2\in S_2$. Comme S est un A-module simple et que $\psi$ n’est pas nulle, $\psi$ est surjective et S est isomorphe à un quotient de $S_1\otimes S_2$. Pour $i\in  \{1,2\}$, le $A_i$-module $S_1\otimes S_2$ est isotypique de type $S_i$, et il en est donc de même du $A_i$-module S (VIII, p. 57, prop. 2).

Pour toute K-algèbre B, on note $\mathscr{S}_K(B)$ l’ensemble des classes de B-modules à gauche simples (VIII, p. 47) qui sont de dimension finie sur K.

#### Théorème 1 {#alg-viii-s12-thm-1 .statement tag=00E8}

Supposons le corps K algébriquement clos.

a) Soit $M_1$ un $A_1$-module et $M_2$ un $A_2$-module tous deux simples (resp. semi-simples) et de dimension finie sur K. Alors $M_1\otimes M_2$ est un module simple (resp. semi-simple) sur l’anneau $A_1\otimes A_2$ et de dimension finie sur K.

b) L’application de $\mathscr{S}_K(A_1)\times \mathscr{S}_K(A_2)$sur $\mathscr{S}_K(A_1\otimes A_2)$qui applique (cl(S$_1)$, cl(S$_2))$sur cl(S$_1\otimes S_2)$lorsque $S_1$ (resp. $S_2)$est un $A_1$-module (resp. $A_2$-module) simple de dimension finie sur K est bijective.

Pour démontrer a), il suffit de considérer le cas où $M_1$ et $M_2$ sont simples. Soit $M'$ un sous-A-module de $M = M_1\otimes M_2$, c’est un sous-A$_1$-module de $M_1\otimes M_2$, stable par l’ensemble des endomorphismes de la forme $1_{M_1}\otimes u$, où $u$ parcourt l’ensemble des homothéties du $A_2$-module $M_2$. Comme le corps K est algébriquement clos, le lemme de Schur (VIII, p. 43, th. 1) entraîne que le commutant End$_A(M_1)$ de $M_1$ est égal à K. D’après le cor. 2 de VIII, p. 59, le sous-A-module $M'$ de $M^{^1}_1\otimes M_2$ est de la forme $M_1\otimes M'_2$, où $M'_2$ est un sous-A$_2$-module de $M_2$. On a supposé que $M_2$ est simple ; on a donc $M'_2= 0$ ou $M'_2= M_2$, c’est-à-dire $M'= 0$ ou $M'= M$. Donc M est simple.

Si S est un module simple sur $A_1\otimes A_2$, de dimension finie sur K, il résulte de la prop. 2 et de a) que S est isomorphe à un module de la forme $S_1\otimes S_2$, où $S_1$ (resp. $S_2)$ est un $A_1$-module (resp. $A_2$-module) simple. De plus, en tant que $A_i$-module, S est isotypique de type $S_i$, donc la classe de $S_i$ ne dépend que de celle de S. Cela prouve b).

#### Remarque 1 {#alg-viii-s12-n1-rem-1 .statement tag=00E9}

L’assertion a) du th. 1 n’est plus vraie lorsque le corps K n’est pas supposé algébriquement clos. On peut donner des exemples (VIII, p. 221, exerc. 4) où $M_i$ est un $A_i$-module simple, de dimension finie sur K pour $i\in  \{1,2\}$ et où le A-module $M_1\otimes M_2$ n’est pas semi-simple, ou est semi-simple mais non simple.

#### Remarque 2 {#alg-viii-s12-n1-rem-2 .statement tag=00EA}

Il existe un homomorphisme $\varphi$ de $R_K(A_1)\otimes_{\mathbf{Z}}R_K(A_2)$ dans $R_K(A)$ caractérisé par la relation $\varphi ([M_1]\otimes [M_2]) = [M_1\otimes M_2]$. Cela se démontre comme la prop. 9 de VIII, p. 192. Si le corps K est algébriquement clos, $\varphi$ est un isomorphisme de $R_K(A_1)\otimes_ZR_K(A_2)$ sur $R_K(A)$ d’après le th. 1, b), puisque pour toute K-algèbre B, le $\mathbf{Z}$-module $R_K(B)$ est libre de base la famille $([S])_{S\in\mathscr{S}_K(B)}$ (VIII, p. 191).

### 2. Produit tensoriel de modules simples

Soient $A_1$ et $A_2$ des algèbres sur le corps commutatif K. On note A la K-algèbre $A_1\otimes A_2$.

#### Lemme 1 {#alg-viii-s12-lem-1 .statement tag=00RB}

Soient $M_1$ et $N_1$ des $A_1$-modules et soient $M_2$ et $N_2$ des $A_2$-modules. On fait les hypothèses suivantes :

(i) Le $A_1$-module $M_1$ est de type fini ;

(ii) Le $A_2$-module $M_2$ est de type fini ou $N_1$ est de dimension finie sur K. Posons $M = M_1\otimes M_2$ et $N = N_1\otimes N_2$, et considérons-les comme modules sur l’anneau $A = A_1\otimes A_2$. L’homomorphisme canonique (II, p.57)

$\lambda :$ Hom$_K(M_1,N_1)\otimes$ Hom$_K(M_2,N_2)\longrightarrow$ Hom$_K(M,N)$

induit alors un isomorphisme de K-espaces vectoriels

$\varphi :$ Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)\longrightarrow$ Hom$_A(M,N)$.

L’application $\lambda$ est injective (II, p. 110, prop. 16) et applique le sous-espace vectoriel Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ dans Hom$_A(M,N)$. Il suffit donc de prouver que toute application A-linéaire de M dans N appartient à l’image de Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ par $\lambda$. Soit $u: M\rightarrow N$ une application A-linéaire. Soit $x\in M_1$. Notons $u_x$ l’application $A_2$-linéaire $y\rightarrow u(x\otimes y)$ de $M_2$ dans $N_1\otimes N_2$. Posons P = Hom$_{A_2}(M_2,N_2)$. Notons $\nu$ l’homomorphisme canonique de $N_1\otimes P$ dans Hom$_{A_2}(M_2,N_1\otimes N_2)$ (II, p. 75). Cette application est injective, (II, p. 75, prop. 2, (i) appliquée au K-espace vectoriel $N_1)$. D’après l’hypothèse (ii), il existe un sous-espace vectoriel $V_x$ de $N_1$, de dimension finie sur K, tel que $u_x$ prenne ses valeurs dans $V_x\otimes N_2$. Il en résulte que $u_x$ est l’image par $\nu$ d’un unique élément $v_x$ de $N_1\otimes P$. L’application $\widetilde{u}:x\rightarrow v_x$ de $M_1$ dans $N_1\otimes P$ est $A_1$-linéaire. D’après l’hypothèse (i), le $A_1$-module $M_1$ est de type fini et un raisonnement analogue au précédent montre que $\widetilde{u}$ appartient à l’image de Hom$_{A_1}(M_1,N_1)\otimes P$ dans Hom$_{A_1}(M_1,N_1\otimes P)$, d’où le lemme 1.

#### Théorème 2 {#alg-viii-s12-thm-2 .statement tag=00EB}

Soient $A_1$ et $A_2$ des algèbres sur le corps commutatif K ; soit $S_1$ un $A_1$-module simple et soit $S_2$ un $A_2$-module simple. Soient $D_1$ et $D_2$ les commutants respectifs de $S_1$ et $S_2$. Posons $M = S_1\otimes S_2, A = A_1\otimes A_2$ et $D = D_1\otimes D_2$. On considère M comme un $(A,D)$-bimodule à gauche.

a) Le commutant du A-module M est égal à $D_M$.

b) L’application $\mathfrak{a}\rightarrow \mathfrak{a}M$est un isomorphisme de l’ensemble des idéaux à droite de D, ordonné par inclusion, sur l’ensemble des sous-A-modules de M, ordonné par inclusion ; l’application réciproque associe à un sous-module N de M l’idéal de D formé des éléments $d$ tels que $dM\subset N$

L’assertion a) résulte du lemme 1 puisqu’un module simple est monogène.

Soit T le $(A_1,D_2$)-bimodule $S_1\otimes (D_2)_d$. On identifie $M = S_1\otimes S_2$ à $T\otimes_{D_2}S_2$ (II, p. 64) ; cette identification est compatible avec les structures de modules à gauche sur l’anneau $A = A_1\otimes A_2$.

Soit N un sous-A-module de M ; c’est un sous-A$_2$-module de $T\otimes_{D_2}S_2$, stable par les endomorphismes de la forme $(a_1)_T\otimes 1_{S_2}$ pour $a_1$ parcourant $A_1$. Il résulte du cor. 2 de VIII, p. 59, qu’il existe un unique sous-(A$_1,D_2$)-bimodule V de T, tel que $N = V\otimes_{D_2}S_2$.

L’isomorphisme $u$ de $T = S_1\otimes (D_2)_d$ dans $((D_1)_d\otimes (D_2)_d)\otimes_{D_1}S_1$ caractérisé par $u(s\otimes d) = 1\otimes d\otimes s$ est $(A_1,D_2$)-linéaire. Identifions ces $(A_1,D_2$)-bimodules. Un raisonnement analogue à celui qui précède démontre l’existence et l’unicité d’un sous-(D$_1\otimes D_2$)-module à droite $\mathfrak{a}$ de $D_1\otimes D_2$ tel que $V =\mathfrak{a}\otimes_{D_1}S_1$. Compte tenu des identifications faites, $\mathfrak{a}$ est l’unique idéal à droite de $D = D_1\otimes D_2$ tel que $N =\mathfrak{a}M$.

On vient de prouver que l’application$\mathfrak{a}\rightarrow \mathfrak{a}M$ est bijective ; la dernière assertion en résulte.

#### Corollaire 1 {#alg-viii-s12-thm-2-cor-1 .statement tag=00EC}

Le module $S_1\otimes S_2$ sur l’anneau $A_1\otimes A_2$ est semi-simple (resp. isotypique, resp. simple) si et seulement si l’anneau $D = D_1\otimes D_2$ est semi-simple (resp. simple, resp. un corps). En particulier, $S_1\otimes S_2$ est simple si le commutant de $S_1$ ou de $S_2$ est égal à K.

Compte tenu du théorème 2, pour que le module $S_1\otimes S_2$ sur l’anneau $D_1\otimes D_2$ soit semi-simple (resp. isotypique, resp. simple), il faut et il suffit que le D-module à droite $(D_1\otimes D_2)_d$ le soit (VIII, p. 104, prop. 10). Or le D-module à droite $D_d$ est simple si et seulement si D est un corps ; il est isotypique (resp. semi-simple) si et seulement si l’anneau D est simple (resp. semi-simple) (VIII, p. 116, déf 1, VIII, p. 117, cor. 1 et VIII, p. 133, prop. 2).

#### Corollaire 2 {#alg-viii-s12-thm-2-cor-2 .statement tag=00ED}

On a $\mathfrak{R}_A(M) =\mathfrak{R}(D)M$. Pour que le A-module M soit sans radical, il faut et il suffit que l’anneau D soit sans radical.

Cela résulte de la prop. 8 de VIII, p. 104 et du th. 2, b).

### 3. Produit tensoriel d’algèbres commutatives semi-simples

#### Théorème 3 {#alg-viii-s12-thm-3 .statement tag=00EE}

Soient $Z_1$ et $Z_2$ des algèbres commutatives semi-simples sur K. Le radical de l’anneau $Z_1\otimes Z_2$ est égal à l’ensemble des éléments nilpotents de cet anneau.

Traitons d’abord le cas où $Z_1$ et $Z_2$ sont des extensions $L_1$ et $L_2$ du corps K. Quitte à échanger $L_1$ et $L_2$, on se ramène au cas où le degré de transcendance de $L_1$ sur K est majoré par celui de $L_2$ sur K. Choisissons une clôture algébrique Ω de $L_2$; d’après le cor. 1 du th. 5 de V, p. 112, on peut supposer que $L_1$ est une sous-extension de Ω.

A) Prouvons d’abord que le radical de $L_1\otimes L_2$ est contenu dans celui de $L_1\otimes \Omega$. Posons $\mathfrak{a}=\mathfrak{R}(L_1\otimes L_2)(L_1\otimes \Omega )$; c’est un idéal de l’anneau commutatif $L_1\otimes \Omega$ et l’on doit prouver que $\mathfrak{a}$ est contenu dans le radical de $L_1\otimes \Omega$. Autrement dit (VIII, p. 151, th. 1), il s’agit de prouver que, pour $x\in \mathfrak{a}$, l’élément $1 +x$ est inversible dans $L_1\otimes \Omega$. Or, comme Ω est une extension algébrique de $L_2$, il existe une extension $L_3$ de $L_2$, de degré fini, telle que $x$ appartienne à $\mathfrak{R}(L_1\otimes L_2)(L_1\otimes L_3)$. Il suffit évidemment de prouver que $1 +x$ est inversible dans $L_1\otimes L_3$. Or $C = L_1\otimes L_3$ est un module de type fini sur l’anneau $B = L_1\otimes L_2$; d’après le cor. de VIII, p. 171, on a $\mathfrak{R}(B)C\subset \mathfrak{R}$(C), donc $x$ appartient au radical de C et $1 +x$ est inversible dans C.

B) Prouvons que le radical de $L_1\otimes \Omega$se compose d’éléments nilpotents. Notons $p$ l’exposant caractéristique de K et P la fermeture radicielle de K dans Ω (V, p. 24) ; c’est un corps parfait. Comme P est une extension algébrique de K, on a $L_1(P) =$ $L_1[P]$ (V, p.18, cor. 1). Soit $\mathfrak{b}$ le noyau de l’homomorphisme canonique de $L_1\otimes P$ sur le corps $P_1= L_1[P]$. Soit $x\in \mathfrak{b}$; il existe des éléments $y_1, . . . , y_n$ de $L_1$, et des éléments $z_1, . . . , z_n$ de P tels que $x=\sum^n_{i=1}y_i\otimes z_i$ et $\sum^n_{i=1}y_iz_i= 0$. Comme P est radiciel sur K, il existe une puissance $q$ de $p$ telle que $z^q_1, . . . , z_n^q$ appartiennent à K. On a alors $\sum_n\sum_n(\sum_n)_q$

$$
x^q=y^q_i\otimes z^q_i=y_i^qz_i^q\otimes 1 =y_iz_i\otimes 1 = 0
$$

$i=1i=1i=1$

Donc $\mathfrak{b}$ se compose d’éléments nilpotents.

Posons $\mathfrak{c}$ = $\mathfrak{b}\otimes_P\Omega$; c’est le noyau de l’homomorphisme canonique de $(L_1\otimes P)\otimes_P\Omega$ sur $P_1\otimes_P\Omega$, et il se compose d’éléments nilpotents d’après ce qui précède. Or Ω est une extension algébriquement close de P, et $P_1$ est une sous-extension de Ω. Comme le corps P est parfait, $P_1$ est une extension séparable de P (V, p. 119, th. 3) ; d’après le th. 4 de V, p. 120, l’intersection des idéaux maximaux de l’anneau commutatif $P_1\otimes_P\Omega$ est réduite à 0. Autrement dit, l’anneau $P_1\otimes_P\Omega$, qui est isomorphe à $((L_1\otimes P)\otimes_P\Omega )/\mathfrak{c}$, est sans radical. Ceci prouve (VIII, p. 150, prop. 5) que $\mathfrak{c}$ contient le radical de l’anneau $(L_1\otimes P)\otimes_P\Omega$; or cet anneau est isomorphe à $L_1\otimes \Omega$, et $\mathfrak{c}$ se compose d’éléments nilpotents. Donc le radical de $L_1\otimes \Omega$ se compose d’éléments nilpotents.

C) Fin de la démonstration du cas particulier. D’après A) et B), le radical $\mathfrak{r}$ de $L_1\otimes L_2$ est contenu dans l’ensemble $\mathfrak{n}$ des éléments nilpotents de cet anneau commutatif ; on sait par ailleurs que $\mathfrak{n}$ est contenu dans $\mathfrak{r}$ (VIII, p. 153, remarque 2).

Passons au cas général. Comme une K-algèbre commutative semi-simple est le produit d’un nombre fini d’extensions du corps K (VIII, p. 133, prop. 3) et que le radical d’un produit d’anneaux est le produit des radicaux (VIII, p. 152, cor. 3), le radical de $Z_1\otimes Z_2$ est l’ensemble des éléments nilpotents de cet anneau.

### 4. Radical d’un produit tensoriel d’algèbres

Soient $A_1$ et $A_2$ des K-algèbres.

#### Proposition 3 {#alg-viii-s12-prop-3 .statement tag=00EF}

On suppose que les algèbres $A_1$ et $A_2$ sont semi-simples, de centres respectifs $Z_1$ et $Z_2$. Posons $Z = Z_1\otimes Z_2$.

a) L’application $\mathfrak{a}\rightarrow \mathfrak{a}A$est un isomorphisme de l’ensemble des idéaux de Z, ordonné par inclusion, sur l’ensemble des idéaux bilatères de A, ordonné par inclusion.

b) Le radical de A est égal à l’intersection des idéaux bilatères maximaux de A et est égal à $\mathfrak{R}(Z)A$.

c) Si l’une des K-algèbres $Z_1$ ou $Z_2$ est séparable, en particulier si le corps K est parfait, les radicaux des anneaux Z et A sont réduits à 0.

Chacune des algèbres $A_i$ est produit d’un nombre fini d’algèbres simples. Or le centre d’un produit d’anneaux est le produit des centres, et l’on a des assertions analogues pour les radicaux (VIII, p. 152, cor. 3) et pour les idéaux bilatères (I, p. 104, prop. 8). Il suffit donc de prouver la proposition 3 sous l’hypothèse que $A_1$ et $A_2$ sont des algèbres simples.

Pour $i\in  \{1,2\}$, posons $B_i= A_i\otimes A^o_i$ et considérons $A_i$ comme un $B_i$-module, les homothéties étant caractérisées par la formule

$$
(x\otimes y)z=xzy
$$

pour $x, y$ et $z$ dans $A_i$. Le commutant du $B_i$-module $A_i$ est $(Z_i)_{A_i}$, l’ensemble des homothéties par les éléments de $Z_i$, que l’on identifie à $Z_i$. De plus, les sous-B$_i$-modules de $A_i$ sont les idéaux bilatères de $A_i$, et comme l’anneau $A_i$ est simple, il n’a pas d’autre idéal bilatère que 0 et $A_i$. Donc $A_i$ est un $B_i$-module simple. Par ailleurs, les sous-(B$_1\otimes B_2$)-modules de $A_1\otimes A_2$ sont les idéaux bilatères de l’anneau $A_1\otimes A_2$.

L’assertion a) résulte donc de VIII, p. 210, th. 2, b) appliqué au $B_1$-module simple $A_1$, de commutant $Z_1$ et au $B_2$-module simple $A_2$ de commutant $Z_2$.

Démontrons l’assertion b). L’intersection des idéaux bilatères maximaux de A est le radical du $(B_1\otimes B_2$)-module $A_1\otimes A_2$; d’après le cor. 2 de VIII, p. 211, cette intersection coïncide avec $\mathfrak{R}(Z)A$. Les algèbres $Z_1$ et $Z_2$ sont commutatives et semi-simples. Le radical de l’anneau Z est donc formé d’éléments nilpotents (VIII, p. 211, th. 3) et l’idéal bilatère $\mathfrak{R}(Z)A$ de l’anneau A est contenu dans le radical $\mathfrak{R}(A)$ (VIII, p. 153, remarque 1). Mais l’intersection des idéaux bilatères maximaux de A contient $\mathfrak{R}(A)$ (VIII, p. 150, prop. 5, d)). Cela prouve l’assertion b).

Le produit tensoriel d’une algèbre commutative séparable et d’une algèbre commutative réduite est un anneau réduit (V, p. 115, prop. 5) ; les algèbres $Z_1$ et $Z_2$ sont commutatives et semi-simples, donc réduites. Si l’une des algèbres $Z_1$ ou $Z_2$ est séparable, l’algèbre Z est réduite ; elle est donc sans radical d’après le th. 3 de VIII, p. 211 et l’on a $\mathfrak{R}(A) =\mathfrak{R}(Z)A = 0$. Ceci a lieu en particulier si le corps K est parfait, car toute algèbre commutative et réduite sur un corps parfait est séparable (V, p. 119, th. 3).

#### Corollaire {#alg-viii-s12-n4-cor-1 .statement tag=00EG}

Supposons que les algèbres $A_1$ et $A_2$ soient simples et que le centre $Z_1$ de $A_1$ soit réduit à K. Alors l’anneau $A_1\otimes A_2$ n’a pas d’idéal bilatère distinct de 0 et de lui-même.

Par hypothèse, on a $Z_1= K$, et comme $A_2$ est simple, son centre $Z_2$ est un corps (VIII, p. 117, cor. 1, a)). L’anneau $Z = Z_1\otimes Z_2$ est donc un corps, et le corollaire résulte de la prop. 3, a).

### 5. Produit tensoriel de modules semi-simples

#### Proposition 4 {#alg-viii-s12-prop-4 .statement tag=00EH}

Pour $i\in  \{1,2\}$, soient $A_i$ une K-algèbre, $M_i$ un $A_i$-module semi-simple et $Z_i$ le centre du commutant de $M_i$. Posons $A = A_1\otimes A_2, M = M_1\otimes M_2$ et $Z = Z_1\otimes Z_2$. On a $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$. Si l’une des algèbres $Z_1$ ou $Z_2$ est séparable sur K, en particulier si le corps K est parfait, alors le A-module M est sans radical.

Pour $i\in  \{1,2\}$, soit $S_i$ un $A_i$-module simple, $D_i$ son commutant et $I(i)$ un ensemble. Commençons par traiter le cas où $M_i$ est le $A_i$-module $S^{(I(i))}_i$. Le centre $Z_i$ de son commutant s’identifie au centre de $D_i$. Posons $D = D_1\otimes D_2$. On a $\mathfrak{R}(D) =$ $\mathfrak{R}(Z)D$ (prop. 3 de VIII, p. 213), et $\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(D)(S_1\otimes S_2)$ (VIII, p. 211, cor. 2), d’où $\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(Z)(S_1\otimes S_2)$. Le A-module M est somme directe d’une famille de A-modules isomorphes à $S_1\otimes S_2$ et le radical de la somme directe d’une famille de modules est la somme directe des radicaux (VIII, p. 148, cor. 2). On a donc $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$.

Passons au cas général. Pour $i\in  \{1,2\}$, notons $\mathscr{S}_{M_i}$ le support du $A_i$-module $M_i$. Pour $\lambda \in \mathscr{S}_{M_i}$, notons $M_{i;\lambda}$ le composant isotypique de type $\lambda$ de $M_i$, et $Z_{i;\lambda}$ le centre de son commutant. L’anneau $Z_i$ s’identifie au produit des anneaux $Z_{i;\lambda}$, pour $\lambda \in \mathscr{S}_{M_i}$. Soient $\lambda \in \mathscr{S}_{M_1}$ et $\mu \in \mathscr{S}_{M_2}$. Notons $i_{\lambda}: Z_{1;\lambda}\rightarrow Z_1$ l’unique application K-linéaire telle que pr$_{\lambda}\circ i_{\lambda}$ soit l’application identique de $Z_{1;\lambda}$ et pr$_{\lambda'}\circ i_{\lambda}$ soit l’application nulle pour $\lambda '\in \mathscr{S}_{M_1}-\{\lambda \}$. Définissons de même $i_{\mu}: Z_{2;\mu}\rightarrow Z_2$. Posons $Z_{\lambda ,\mu}= Z_{1;\lambda}\otimes Z_{2;\mu},i_{\lambda ,\mu}=i_{\lambda}\otimes i_{\mu}$ et notons $\pi_{\lambda ,\mu}$ l’application pr$_{\lambda}\otimes$ pr$_{\mu}$ de Z dans $Z_{\lambda ,\mu}$. L’application $\pi_{\lambda ,\mu}$ est un homomorphisme surjectif d’anneaux ; on a donc $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))\subset \mathfrak{R}(Z_{\lambda ,\mu})$ (VIII, p. 150, prop. 5 b)). Démontrons l’inclusion opposée. Soit $z$ un élément de $\mathfrak{R}(Z_{\lambda ,\mu})$; comme $Z_{1;\lambda}$ et $Z_{2;\mu}$ sont des corps, $z$ est nilpotent (th. 3 de VIII, p. 211). On a $i_{\lambda ,\mu}(xy) =i_{\lambda ,\mu}(x)\cdot i_{\lambda ,\mu}(y)$ pour $x, y$ dans $Z_{\lambda ,\mu}$, par conséquent $i_{\lambda ,\mu}(z)$ est nilpotent donc appartient à $\mathfrak{R}(Z)$. Comme $\pi_{\lambda ,\mu}\circ i_{\lambda ,\mu}$ est l’application identique de $Z_{\lambda ,\mu}$, l’élément $z$ appartient à $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))$. Nous avons ainsi prouvé l’égalité $\pi_{\lambda ,\mu}(\mathfrak{R}(Z)) =\mathfrak{R}(Z_{\lambda ,\mu})$.

Posons $M_{\lambda ,\mu}= M_{1;\lambda}\otimes M_{2;\mu}$; c’est un sous-module de M, stable par Z ; pour $z\in Z$ et $m\in M_{\lambda ,\mu}$, on a $zm=\pi_{\lambda ,\mu}(z)m$. Par suite $\mathfrak{R}(Z)M_{\lambda ,\mu}$ est égal à $\mathfrak{R}(Z_{\lambda ,\mu})M_{\lambda ,\mu}$, et donc à $\mathfrak{R}_A(M_{\lambda ,\mu})$ d’après le cas isotypique. Comme le radical d’une somme directe est la somme directe des radicaux (VIII, p. 148, cor. 2) et que M est somme directe des sous-modules $M_{\lambda ,\mu}$, pour $(\lambda , \mu )\in \mathscr{S}_{M_1}\times \mathscr{S}_{M_2}$, l’égalité $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$ est démontrée. La dernière assertion résulte alors de la prop. 3 de VIII, p. 213.

#### Lemme 2 {#alg-viii-s12-lem-2 .statement tag=00EI}

Soient $A_1$ et $A_2$ des algèbres sur le corps commutatif K. Soient $M_1$ un $A_1$-module de dimension finie sur K et $M_2$ un $A_2$-module de longueur finie. Le $A_1\otimes A_2$-module $M_1\otimes M_2$ est de longueur finie.

Posons $M = M_1\otimes M_2$. Soit $(e_1, . . . , e_n)$ une base de $M_1$ sur le corps K. L’application $(x_1, . . . , x_n)\rightarrow \sum^n_{i=1}e_i\otimes x_i$ est un isomorphisme du $A_2$-module $M^n_2$ sur le $A_2$-module M. Comme $M_2$ est un $A_2$-module de longueur finie, il en est de même de M. De plus, tout sous-A-module de M est un sous-A$_2$-module ; par suite, M est un A-module de longueur finie.

#### Proposition 5 {#alg-viii-s12-prop-5 .statement tag=00RC}

Soient $A_1$ et $A_2$ des algèbres sur le corps commutatif K. Soient $M_1$ un $A_1$-module semi-simple, de dimension finie sur K, et $M_2$ un $A_2$-module semi-simple. Pour $i= 1,2$, notons $D_i$ le commutant du $A_i$-module $M_i$ et $Z_i$ le centre de $D_i$. Posons $A = A_1\otimes A_2, M = M_1\otimes M_2, D = D_1\otimes D_2$ et $Z = Z_1\otimes Z_2$.

a) Le commutant du A-module M s’identifie à D et son centre est Z. Si le $A_2$-module $M_2$ est de longueur finie, le A-module M est de longueur finie, l’anneau D est artinien à droite et à gauche et l’anneau Z est artinien.

b) Les conditions suivantes sont équivalentes :

(i) Le A-module M est semi-simple ;

(ii) L’anneau Z est isomorphe au produit d’une famille de corps commutatifs ;

(iii) L’anneau Z est réduit.

c) Les conditions suivantes sont équivalentes :

(i) Le A-module M est isotypique et non réduit à 0 ;

(ii) L’anneau Z est un corps ;

(iii) L’anneau Z est intègre.

Par hypothèse $M_1$ est de dimension finie sur K. Le commutant de M s’identifie alors à D (VIII, p. 209, lemme 1) et son centre est Z (III, p. 41, cor.). Supposons le $A_2$-module $M_2$ de longueur finie. Le A-module M est de longueur finie d’après le lemme 2. Comme $M_2$ est semi-simple et de type fini, l’anneau $D_2$ est semi-simple (VIII, p. 135, prop. 6) et son centre $Z_2$ est le produit d’une famille finie de corps commutatifs. Par suite, le $D_2$-module $(D_2)_s$ et le $Z_2$-module $(Z_2)_s$ sont de longueur finie. D’autre part, comme $M_1$ est de dimension finie sur K, il en est de même de $D_1$ et $Z_1$. D’après le lemme 2, le module $(D_1\otimes D_2)_s$ est de longueur finie, donc l’anneau $D_1\otimes D_2$ est artinien à gauche. On prouve de même que l’anneau $D_1\otimes D_2$ est artinien à droite et que l’anneau $Z_1\otimes Z_2$ est artinien, d’où a).

Démontrons b). Le centre du commutant d’un module semi-simple est isomorphe au produit d’une famille de corps commutatifs (VIII, p. 82, prop. 8, a)) ; cela prouve que (i) entraîne (ii). L’implication (ii) $=\Rightarrow$ (iii) est claire.

Supposons l’anneau Z réduit. On a alors $\mathfrak{R}(Z) = 0$ (VIII, p. 211, th. 3) et, par la prop. 4 de VIII, p. 214$,\mathfrak{R}_A(M) = 0$. Comme le $A_2$-module $M_2$ est semi-simple, il existe une famille $(S_i)_{i\in I}$ de $A_2$-modules simples et un isomorphisme de $M_2$ sur $\bigoplus S_i$. Par conséquent, le A-module M est isomorphe à $\bigoplus M_1\otimes S_i$. Pour tout $i\in I$, le A-module $M_1\otimes S_i$ est donc sans radical ; par a) il est de longueur finie et donc semi-simple (VIII, p. 149, prop. 3, b)). Le A-module M est alors somme directe d’une famille de modules semi-simples, donc est semi-simple. Cela prouve que (iii) implique (i), et termine la démonstration de b).

Pour qu’un A-module soit isotypique et non nul, il faut et il suffit qu’il soit semi-simple et que le centre de son commutant soit un corps (VIII, p. 82, prop. 8, b)). Ainsi c) résulte de b).

#### Corollaire {#alg-viii-s12-n5-cor-1 .statement tag=00EJ}

Si $Z_1$ ou $Z_2$ est une algèbre séparable sur le corps K (ce qui a lieu par exemple si K est parfait), le A-module $M_1\otimes M_2$ est semi-simple.

Les anneaux $Z_1$ et $Z_2$ sont isomorphes à des produits de corps, donc sont des anneaux réduits. En particulier, si K est parfait, ce sont des algèbres séparables sur K (V, p. 119, th. 3). D’après la prop. 5 de V, p. 115, le produit tensoriel d’une algèbre séparable et d’une algèbre réduite est réduit. Donc Z est un anneau réduit, et le corollaire résulte de la prop. 5, b)

### 6. Produit tensoriel d’algèbres semi-simples

#### Proposition 6 {#alg-viii-s12-prop-6 .statement tag=00EK}

Soient $A_1$ et $A_2$ des K-algèbres non nulles. Si l’anneau $A_1\otimes A_2$ est simple (resp. semi-simple), alors les anneaux $A_1$ et $A_2$ sont simples (resp. semi-simples).

Pour qu’un anneau B soit semi-simple (resp. simple), il faut et il suffit que le B-module $B_s$ soit semi-simple (resp. isotypique et non nul). La proposition résulte alors de la prop. 1 (VIII, p. 207).

#### Proposition 7 {#alg-viii-s12-prop-7 .statement tag=00EL}

Soient $A_1$ et $A_2$ des K-algèbres semi-simples, de centres respectifs $Z_1$ et $Z_2$. On suppose que $A_1$ est de degré fini sur K. Alors l’anneau $A_1\otimes A_2$ est artinien à gauche, ainsi que son centre $Z_1\otimes Z_2$. Pour que l’anneau $A_1\otimes A_2$ soit simple (resp. semi-simple), il faut et il suffit que l’anneau $Z_1\otimes Z_2$ soit un corps (resp. un anneau réduit).

C’est le cas particulier $M_1= (A_1)_s, M_2= (A_2)_s$ de la prop. 5 de VIII, p. 215.

#### Corollaire 1 {#alg-viii-s12-prop-7-cor-1 .statement tag=00EM}

Soient $A_1$ et $A_2$ des K-algèbres semi-simples ; on suppose que $A_1$ est de dimension finie sur K. Supposons que le centre de $A_1$ ou celui de $A_2$ soit une algèbre séparable sur K, ce qui a lieu, par exemple, si K est parfait, alors $A_1\otimes A_2$ est semi-simple.

C’est le cas particulier $M_1= (A_1)_s, M_2= (A_2)_s$ du corollaire de VIII, p. 216.

#### Corollaire 2 {#alg-viii-s12-prop-7-cor-2 .statement tag=00RD}

Soient $A_1$ et $A_2$ des K-algèbres simples ; on suppose que $A_1$ est de dimension finie sur K. Si le centre de $A_1$ ou celui de $A_2$ est égal à K, alors l’algèbre $A_1\otimes A_2$ est simple. C’est en particulier le cas si K est algébriquement clos.

Les centres $Z_1$ et $Z_2$ de $A_1$ et $A_2$ respectivement sont des corps ; si l’un des anneaux $Z_1$ ou $Z_2$ est égal à K, l’anneau $Z_1\otimes Z_2$ est un corps. Il suffit donc d’appliquer la prop. 7.

Si le corps K est algébriquement clos, le centre de $A_1$ est égal à K.

### 7. Extension des scalaires dans les modules semi-simples

#### Proposition 8 {#alg-viii-s12-prop-8 .statement tag=00EN}

Soient A une K-algèbre, M un A-module et L une extension du corps K. Notons D le commutant de M et Z le centre de D.

a) Supposons que le $A_{(L)}$-module $M_{(L)}$ soit simple (resp. isotypique, resp. semi-simple). Alors le A-module M est simple (resp. isotypique, resp. semi-simple).

b) Supposons que le A-module M soit semi-simple et que M ou L soit de dimension finie sur K. Pour que le $A_{(L)}$-module $M_{(L)}$ soit semi-simple, il faut et il suffit que l’anneau $Z_{(L)}$ soit réduit. Pour que le $A_{(L)}$-module $M_{(L)}$ soit isotypique et non nul, il faut et il suffit que l’anneau $Z_{(L)}$ soit intègre.

c) Supposons que le A-module M soit simple. Pour que le $A_{(L)}$-module $M_{(L)}$ soit semi-simple (resp. isotypique, resp. simple), il faut et il suffit que l’anneau $D_{(L)}$ soit semi-simple (resp. simple, resp. un corps).

L’assertion a) est un cas particulier de la prop. 1 (VIII, p. 207), l’assertion b) un cas particulier de la prop. 5 (VIII, p. 215), et l’assertion c) un cas particulier du cor. 1 de VIII, p. 211.

#### Corollaire 1 {#alg-viii-s12-prop-8-cor-1 .statement tag=00EO}

a) Supposons que le A-module M soit semi-simple, que l’extension L de K soit séparable et que M ou L soit de dimension finie sur K. Alors le $A_{(L)}$-module $M_{(L)}$ est semi-simple.

b) Supposons que le A-module M soit simple et que son commutant soit égal à K. Alors le $A_{(L)}$-module $M_{(L)}$ est simple.

L’assertion a) résulte du cor., VIII, p. 216. L’assertion b) est un cas particulier de la prop. 8, c).

#### Corollaire 2 {#alg-viii-s12-prop-8-cor-2 .statement tag=00RE}

Soit L une extension du corps K. Notons Z le centre de la K-algèbre A.

a) Si la L-algèbre $A_{(L)}$ est semi-simple, la K-algèbre A est semi-simple.

b) Supposons que la K-algèbre A soit semi-simple et que L ou A soit de dimension finie sur K. Pour que la L-algèbre $A_{(L)}$ soit semi-simple, il faut et il suffit que l’anneau $Z_{(L)}$ soit réduit ; c’est le cas en particulier si L est une extension séparable de K. Pour que $A_{(L)}$ soit une L-algèbre simple, il faut et il suffit que l’anneau $Z_{(L)}$ soit intègre ; c’est en particulier le cas si le centre de A est égal à K.

Les assertions a) et b) résultent de la prop. 8, a) et b) appliquée au A-module $A_s$.

#### Proposition 9 {#alg-viii-s12-prop-9 .statement tag=00EP}

Soient A une K-algèbre et L une extension séparable de K.

a) Si M est un A-module sans radical, le $A_{(L)}$-module $M_{(L)}$ est sans radical.

b) Si la K-algèbre A est sans radical, la L-algèbre $A_{(L)}$ est sans radical.

Démontrons l’assertion a). Soit M un A-module sans radical. On identifie M à son image canonique dans $M_{(L)}$. Soit N un sous-module maximal de M. Comme le A-module $M/N$ est simple, il résulte de la prop. 4 de VIII, p. 214 que le $A_{(L)}$-module $(M/N)_{(L)}= M_{(L)}/N_{(L)}$ est sans radical, d’où $\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset N_{(L)}$ d’après le cor. 1, c) de VIII, p. 148. Or il résulte du cor. de la prop. 14 de II, p. 109 que l’intersection des $N_{(L)}$, où N parcourt l’ensemble des sous-modules maximaux de M, est réduite à 0. Par conséquent, le $A_{(L)}$-module $M_{(L)}$ est sans radical.

L’assertion b) découle de l’assertion a) appliquée au A-module $A_s$.

#### Proposition 10 {#alg-viii-s12-prop-10 .statement tag=00EQ}

Soient A une K-algèbre et L une extension de K. Soit M un A-module.

a) On fait une des deux hypothèses suivantes :

(i) Le A-module M est de type fini et L est algébrique sur K ;

(ii) L’anneau A est artinien à gauche.

Alors on a l’inclusion

$$
\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})
$$

b) Si L est une extension séparable de K, alors on a l’inclusion

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

Démontrons tout d’abord l’assertion a). Plaçons-nous dans le cas (i). Supposons d’abord L de degré fini sur K. Alors le A-module $M_{(L)}$ est de type fini. Notons $f$ l’homomorphisme canonique de A dans $A_{(L)}$; l’anneau $A_{(L)}$ est engendré par la réunion de son centre et de $f(A)$. On peut donc appliquer la prop. 3 de VIII, p. 170 au $A_{(L)}$-module $M_{(L)}$. On en déduit l’inclusion $\mathfrak{R}_A(M_{(L)})\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$, et a fortiori $\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ (VIII, p. 148, cor. 1).

Traitons le cas général. Soient $x_1, . . . , x_n$ des éléments engendrant le A-module M et $x$ un élément de $\mathfrak{R}_A(M)$. Soient $a_1, . . . , a_n$ des éléments de $A_{(L)}$; comme L est algébrique sur K, il existe une extension finie $L'$ de K, contenue dans L, telle que les $a_i$ appartiennent à $A_{(L')}$. D’après ce qui précède, $x$ appartient au radical du $A_{(L')}$-module $M_{(L')}$; il résulte du cor. de VIII, p. 149, que les éléments $x_i+a_ix$ $(1\leqslant i\leqslant n)$ engendrent le $A_{(L')}$-module $M_{(L')}$, donc le $A_{(L)}$-module $M_{(L)}$. D’après ce même corollaire, $x$ appartient au radical du $A_{(L)}$-module $M_{(L)}$.

Plaçons-nous dans le cas (ii). Soit $\mathfrak{r}$ le radical de A, de sorte que le radical du A-module M est égal à $\mathfrak{r}M$ (VIII, p. 170, cor.). Le radical $\mathfrak{r}$ de A est un idéal bilatère nilpotent de A (VIII, p. 169, prop. 1), donc $\mathfrak{r}_{(L)}$ est un idéal bilatère nilpotent de $A_{(L)}$. On en déduit $\mathfrak{r}_{(L)}\subset \mathfrak{R}(A_{(L)})$ (VIII, p. 151, th. 1) et la prop. 6 de VIII, p. 154 entraîne $\mathfrak{R}(A_{(L)})M_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$. On a donc $\mathfrak{R}_A(M) =\mathfrak{r}M\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$, ce qui achève la démonstration de l’assertion a).

Le A-module $M/\mathfrak{R}_A(M)$ est sans radical. Si L est une extension séparable de K, il résulte de la prop. 9 de VIII, p. 218 que le $A_{(L)}$-module $(M/\mathfrak{R}_A(M))_{(L)}$ est sans radical. Par conséquent on a l’inclusion

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

#### Corollaire {#alg-viii-s12-n7-cor-1 .statement tag=00ER}

Soit L une extension séparable de K. On a $\mathfrak{R}(A_{(L)}) =\mathfrak{R}(A)_{(L)}$ si L est algébrique sur K ou si l’anneau A est artinien à gauche.

C’est le cas particulier $M = A_s$ de la prop. 10.

## EXERCICES {#alg-viii-s12-exercises}

See the [exercises for § 12](exercises/s12/).
