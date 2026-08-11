---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 14
section_title: Algèbres centrales et simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.247-A VIII.272
pdf_pages: 0250-0275
extraction: native
subsections:
    - "no": 1
      title: Algèbres centrales et simples
      page: 247
      pdf_page: 250
    - "no": 2
      title: Deux lemmes sur les bimodules
      page: 250
      pdf_page: 253
    - "no": 3
      title: Théorèmes de conjugaison
      page: 252
      pdf_page: 255
    - "no": 4
      title: Automorphismes des algèbres semi-simples
      page: 254
      pdf_page: 257
    - "no": 5
      title: Sous-algèbres simples des algèbres simples
      page: 255
      pdf_page: 258
    - "no": 6
      title: Sous-algèbres commutatives maximales
      page: 257
      pdf_page: 260
    - "no": 7
      title: Sous-algèbres étales maximales
      page: 260
      pdf_page: 263
    - "no": 8
      title: Sous-algèbres diagonalisables des algèbres simples
      page: 262
      pdf_page: 265
statements: 36
exercises: 19
content_sha256: 0332dfb05214d16c01e52f87c187495097e27bfacb03a6b3412d923cf6b7dc24
---

## § 14. ALGÈBRES CENTRALES ET SIMPLES

Dans ce paragraphe, K désigne un corps commutatif.

### 1. Algèbres centrales et simples

#### Définition 1 {#alg-viii-s14-def-1 .statement tag=00GE}

On dit qu’une algèbre A sur le corps K est centrale si l’application $\lambda \rightarrow \lambda 1$est une bijection de K sur le centre de A.

Une algèbre centrale n’est pas réduite à 0. Pour tout entier $n\geqslant 1$, la K-algèbre de matrices $\mathbf{M}_n(K)$ est centrale (VIII, p. 78, cor. 2) et simple (VIII, p. 116, th. 1). Plus généralement, soit D une K-algèbre centrale de degré fini, alors $\mathbf{M}_n(D)$ est également centrale. Soit A un anneau simple ; son centre Z est un corps (VIII, p. 117, cor. 1), et A est donc une algèbre centrale et simple sur Z. Si le corps K est algébriquement clos, une algèbre simple de degré fini sur K est centrale (VIII, p. 118, cor. 3). L’algèbre opposée d’une algèbre centrale et simple est centrale et simple.

#### Remarque 1 {#alg-viii-s14-n1-rem-1 .statement tag=00GF}

Soient A et B des K-algèbres. Si l’algèbre $A\otimes_KB$ est centrale et simple, il en est de même de A et B (III, p. 41, cor. de la prop. 6 et VIII, p. 217, prop. 6). Réciproquement, si les algèbres A et B sont centrales et simples et si l’une d’elles est de degré fini sur K, alors l’algèbre $A\otimes_KB$ est centrale et simple (III, p. 41, cor. de la prop. 6 et VIII, p. 217, cor. 2).

#### Remarque 2 {#alg-viii-s14-n1-rem-2 .statement tag=00GG}

Soit A une K-algèbre et soit L une extension du corps K. Si la L-algèbre $A_{(L)}$ est centrale et simple, alors la K-algèbre A est centrale et simple. Réciproquement, si l’un des degrés [A : K] ou [L : K] est fini et si la K-algèbre A est centrale et simple, la L-algèbre $A_{(L)}$ est centrale et simple. Cela résulte du cor. 2 de VIII, p. 218.

#### Remarque 3 {#alg-viii-s14-n1-rem-3 .statement tag=00GH}

Soient A et B des K-algèbres équivalentes au sens de Morita. L’algèbre A est centrale simple si et seulement s’il en est de même de B (VIII, p. 101, prop. 6, p. 106, cor. et p. 98, cor. 1).

#### Remarque 4 {#alg-viii-s14-n1-rem-4 .statement tag=00GI}

En particulier, si A est une K-algèbre centrale et simple et si $n\geqslant 1$, alors $\mathbf{M}_n(A)$ est une K-algèbre centrale et simple (VIII, p. 98, exemple 1).

#### Théorème 1 {#alg-viii-s14-thm-1 .statement tag=00GJ}

Soit A une K-algèbre de degré fini. Les propriétés suivantes sont équivalentes :

(i) L’algèbre A est centrale et simple ;

(ii) L’algèbre A est centrale et sans radical ;

(iii) L’homomorphisme canonique de la K-algèbre $A\otimes_KA^o$ dans la K-algèbre End$_K(A)$qui transforme $a\otimes a'$ en l’application K-linéaire $x\rightarrow axa'$ de A dans A est bijectif ;

(iv) Il existe une extension L du corps K et un entier $n\geqslant 1$tels que les L-algèbres $A_{(L)}$ et $\mathbf{M}_n(L)$soient isomorphes ;

(v) Pour toute clôture séparable $K'$ de K, il existe un entier $n\geqslant 1$tel que les $K'$-algèbres $A_{(K')}$ et $\mathbf{M}_n(K')$soient isomorphes ;

(vi) Il existe une extension L du corps K, galoisienne et de degré fini, et un entier $n\geqslant 1$tels que les L-algèbres $A_{(L)}$ et $\mathbf{M}_n(L)$soient isomorphes ;

(vii) Il existe une K-algèbre de degré fini D qui est un corps de centre K et un entier $n\geqslant 1$tel que l’algèbre A soit isomorphe à l’algèbre $\mathbf{M}_n(D)$.

Pour qu’un anneau soit simple, il faut et il suffit qu’il soit semi-simple et que son centre soit un corps (VIII, p. 138, cor. de la prop. 10). Comme A est une algèbre de degré fini sur le corps K, c’est un anneau artinien à gauche ; il est donc semi-simple si et seulement s’il est sans radical (VIII, p. 150, prop. 4). L’équivalence de (i) et (ii) résulte de là.

Posons $E = A\otimes_KA^o$ et F = End$_K(A)$; notons $\varphi$ l’homomorphisme canonique de E dans F défini par la relation $\varphi (a\otimes a')(x) =axa'$ pour $x, a, a'$ dans A. Si l’algèbre A est centrale et simple, il en est de même de $A^o$ et donc de E (remarque 1), et $\varphi$ est donc injectif. Or on a $[E : K] = [A : K]^2= [F : K]$, donc $\varphi$ est bijectif. Réciproquement, supposons $\varphi$ bijectif ; comme l’algèbre F est centrale et simple (car elle est isomorphe à une algèbre de matrices $\mathbf{M}_m$(K)), il en est de même de E, donc aussi de A (remarque 1). On a donc prouvé l’équivalence de (i) et (iii).

Par la remarque 4, l’assertion (vii) entraîne l’assertion (i). L’implication réciproque résulte du cor. 3 de VIII, p. 118 et du cor. 2 de VIII, p. 78.

Il est clair que (vi) entraîne (iv), et (iv) entraîne (i) d’après la remarque 2.

Il reste à prouver les implications (i)$\Rightarrow$(v)$\Rightarrow$(vi). Supposons que A soit centrale et simple et notons $K'$ une clôture séparable de K (V, p. 44). Alors $A_{(K')}$ est une algèbre centrale, simple et de degré fini sur $K'$ (VIII, p. 247, remarque 2). D’après le corollaire de VIII, p. 227, il existe donc un entier $n\geqslant 1$ et un isomorphisme de $K'$-algèbres de $A_{(K')}$ sur $\mathbf{M}_n(K')$; remarquons que les $K'$-algèbres $\mathbf{M}_n(K')$ et $\mathbf{M}_n(K)_{(K')}$ sont isomorphes. D’après le lemme 4 de VIII, p. 229, il existe une sous-extension L de $K'$, de type fini K telle que les L-algèbres $A_{(L)}$ et $\mathbf{M}_n(K)_{(L)}$ soient isomorphes. Alors L est séparable et de degré fini sur K, donc contenue dans une sous-extension $L'$ de $K'$, galoisienne et de degré fini sur K (V, p. 55, prop. 2). Les $L'$-algèbres $A_{(L')}$ et $\mathbf{M}_n(L')$ sont alors isomorphes.

#### Corollaire 1 {#alg-viii-s14-thm-1-cor-1 .statement tag=00GK}

Soit A une algèbre centrale, simple et de degré fini sur un corps séparablement clos K. Il existe un entier $n\geqslant 1$tel que A soit isomorphe à l’algèbre de matrices $\mathbf{M}_n(K)$.

En effet, toute extension galoisienne de K est égale à K ; il suffit d’appliquer l’équivalence des propriétés (i) et (v) du th. 1.

#### Corollaire 2 {#alg-viii-s14-thm-1-cor-2 .statement tag=00GL}

Soit A une algèbre centrale, simple, et de degré fini sur K (par exemple, un corps de centre K et de degré fini sur K). Il existe un entier $n\geqslant 1$tel que $[A : K] =n^2$.

Soient L une extension de K et $n$ un entier strictement positif tels que les L-algèbres $A_{(L)}$ et $\mathbf{M}_n(L)$ soient isomorphes. On a

$$
[A : K] = [A_{(L)}: L] = [\mathbf{M}_n(L) : L] =n^2
$$

Avec les notations du corollaire 2, l’entier $n$ s’appelle le degré réduit de A.

#### Remarque 5 {#alg-viii-s14-n1-rem-5 .statement tag=00GM}

Soit A une algèbre centrale, simple et de degré fini sur K, dont le degré réduit est un nombre premier $\ell$. Alors A est un corps ou A est isomorphe à $\mathbf{M}_{\ell}(K)$. En effet, A est isomorphe à une algèbre de la forme $\mathbf{M}_n$(D), où D est un corps de centre K et l’on a

$$
\ell^2= [A : K] =n^2[D : K]
$$

si A n’est pas un corps, alors $n\not= 1$, donc $n=\ell$ et D = K.

### 2. Deux lemmes sur les bimodules

Soient A et B des anneaux. Pour tout homomorphisme $f$ de B dans A, on note $A^f$ le $(B$, A)-bimodule dont le A-module à droite sous-jacent est $A_d$ et dont la loi d’action de B-module à gauche est donnée par $(b, a)\rightarrow f(b)a$.

#### Lemme 1 {#alg-viii-s14-lem-1 .statement tag=00GN}

Soient $f$ et $g$ des homomorphismes de B dans A. Les conditions suivantes sont équivalentes :

(i) Les $(B,A)$-bimodules $A^f$ et $A^g$ sont isomorphes ;

(ii) Il existe un automorphisme intérieur (I, p. 97, exemple $2)\theta$ de A tel que $g=\theta \circ f$.

Les automorphismes du A-module à droite $A_d$ sont les applications $x\rightarrow ax$, où $a$ est un élément inversible de A. Pour qu’un tel automorphisme soit une application B-linéaire de $A^f$ dans $A^g$, il faut et il suffit que l’on ait

$$
g(b)ax=af(b)x
$$

pour tout $x$ dans A et tout $b$ dans B. Cette relation équivaut à $g(b) =af(b)a^{-1}$ pour tout $b$ dans B, c’est-à-dire à $g=\theta \circ f$, où $\theta$ est l’automorphisme intérieur $x\rightarrow axa^{-1}$ de A.

#### Lemme 2 {#alg-viii-s14-lem-2 .statement tag=00GO}

Supposons que B soit un anneau semi-simple et un module de type fini sur son centre Z. Soient M et N des $(B,A)$-bimodules. Supposons-les de longueur finie (ce qui a lieu en particulier si ce sont des A-modules à droite de longueur finie). Si M et N sont isomorphes comme $(Z,A)$-bimodules, ils sont isomorphes comme $(B,A)$-bimodules.

A) Considérons d’abord le cas où B est l’anneau des endomorphismes d’un espace vectoriel S de dimension finie $d$ sur un corps commutatif L. On a alors Z = L ; on considère S comme un $(B$, Z)-bimodule. L’anneau B est simple, S est un B-module simple et Z est le commutant de S ; tout B-module est isotypique de type S (VIII, p. 118, prop. 2 a)). Soit $(V, \alpha )$ (resp. $(W, \beta ))$ une description du B-module M (resp. N). L’ensemble V (resp. W) est muni d’une structure de $(Z,A)$-bimodule de sorte que $\alpha$ (resp. $\beta )$ soit un isomorphisme de $(B$, A)-bimodules (VIII, p. 60, remarque 2). Comme $(Z$, A)-bimodule, M est isomorphe à $V^d$ et N à $W^d$, et il existe un isomorphisme de l’ensemble des sous-(Z, A)-bimodules de V, ordonné par inclusion, sur celui des sous-(B, A)-bimodules de M (loc. cit.). Donc V est un $(Z$, A)-bimodule de longueur finie et il en est de même de W. Comme les $(Z,A)$-bimodules $V^d$ et $W^d$ sont isomorphes, les $(Z$, A)-bimodules V et W sont isomorphes d’après le th. 2, d) de VIII, p. 34 appliqué à l’anneau $Z\otimes_{\mathbf{Z}}A^o$. Finalement, les $(B$, A)-bimodules M et N sont isomorphes.

B) Considérons maintenant le cas où B est un anneau simple, de type fini en tant que Z-module. Alors Z est un corps et B est une algèbre centrale, simple, et de degré fini sur le corps Z. D’après le th. 1 de VIII, p. 248 il existe une extension $Z'$ de Z, de degré fini sur Z, telle que la $Z'$-algèbre $B'= B_{(Z')}$ soit isomorphe à l’algèbre des endomorphismes d’un espace vectoriel de dimension finie sur $Z'$. Posons $M'= M_{(Z')}$ et $N'= N_{(Z')}$. Alors $M'$ et $N'$ sont des $(B'$, A)-bimodules de longueur finie ; considérés comme $(Z'$, A)-bimodules, $M'$ et $N'$ sont isomorphes. D’après le cas traité en $A), M'$ et $N'$ sont isomorphes comme $(B'$, A)-bimodules et a fortiori comme $(B$, A)-bimodules. Posons $r= [Z': Z]$; le $(B$, A)-bimodule $M'= Z'\otimes_ZM$ est isomorphe à $M^r$ et, de même, le $(B$, A)-bimodule $N'$ est isomorphe à $N^r$; comme M et N sont des $(B$, A)-bimodules de longueur finie, il résulte du th. 2, d) de VIII, p. 34 que les $(B$, A)-bimodules M et N sont isomorphes.

C) Considérons enfin le cas général, où B est un anneau semi-simple, de type fini en tant que Z-module. Soit $\mathscr{S}$ l’ensemble des classes de B-modules simples ; il est fini (VIII, p. 132, prop. 1). Pour tout $\lambda \in \mathscr{S}$, notons $M_{\lambda}$ (resp. $N_{\lambda})$ le composant isotypique de type $\lambda$ du B-module M (resp. N) ; c’est un sous-(B, A)-bimodule de M (resp. N) (remarque, VIII, p. 63). Pour $\lambda \in \mathscr{S}$, notons $\mathfrak{b}_{\lambda}$ l’annulateur du B-module $\lambda$ et posons $B_{\lambda}= B/\mathfrak{b}_{\lambda}$; soit $Z_{\lambda}$ le centre de $B_{\lambda}$. Pour $\lambda \in \mathscr{S}$, les $(B_{\lambda},A)$-bimodules $M_{\lambda}$ et $N_{\lambda}$ sont de longueur finie. On peut alors identifier B au produit des anneaux simples $B_{\lambda}$, et Z au produit des $Z_{\lambda}$ (VIII, p. 137, prop. 8). De plus, on peut identifier M à $\prod_{\lambda\in\mathscr{S}}M_{\lambda}$ et N à $\prod_{\lambda\in\mathscr{S}}N_{\lambda}$,. Par hypothèse, M et N sont isomorphes comme $(Z$, A)-bimodules ; il en résulte que pour $\lambda \in \mathscr{S}, M_{\lambda}$ et $N_{\lambda}$ sont des $(Z_{\lambda}$, A)-bimodules isomorphes. D’après le cas traité en B), les $(B_{\lambda}$, A)-bimodules $M_{\lambda}$ et $N_{\lambda}$ sont isomorphes, donc les $(B$, A)-bimodules M et N sont isomorphes.

#### Remarque {#alg-viii-s14-n2-rem-1 .statement tag=00GP}

Il résulte de la démonstration du lemme 2 que M et N sont des $(Z,A)$-bimodules de longueur finie. Par conséquent, si B et A sont deux anneaux semi-simples qui sont des modules de type fini sur leurs centres respectifs Z(B) et Z(A), deux $(B$, A)-bimodules de longueur finie qui sont isomorphes comme (Z(B),Z(A))bimodules sont isomorphes.

### 3. Théorèmes de conjugaison

#### Théorème 2 {#alg-viii-s14-thm-2 .statement tag=00GQ}

Soient B un anneau semi-simple et Z son centre ; on suppose que B est un Z-module de type fini. Soit A un anneau artinien à droite et soient $f$ et $g$ des homomorphismes d’anneaux de B dans A ; notons $f_Z$ et $g_Z$ les restrictions de $f$ et $g$ à Z. Les propriétés suivantes sont équivalentes :

(i) Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$;

(ii) Il existe un automorphisme intérieur $\theta$ de A tel que $g_Z=\theta \circ f_Z$.

Comme l’anneau A est artinien à droite, $A_d$ est un A-module à droite de longueur finie (VIII, p. 5, th. 1). Ainsi $A^f$ et $A^g$ sont des $(B$, A)-bimodules de longueur finie. D’après le lemme 1 (VIII, p. 250), l’assertion (i) signifie que $A^f$ et $A^g$ sont des $(B$, A)-bimodules isomorphes et l’assertion (ii) que ce sont des $(Z$, A)-bimodules isomorphes. L’équivalence de (i) et (ii) résulte donc du lemme 2 (VIII, p. 250).

#### Corollaire {#alg-viii-s14-n3-cor-1 .statement tag=00GR}

Soient A et B des algèbres sur le corps K. On suppose que B est centrale, simple et de degré fini et que A est artinienne à droite. Soient $f$ et $g$ des homomorphismes de K-algèbres de B dans A. Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$.

Avec les notations du théorème 2, on a en effet Z = K, d’où $f_Z=g_Z$.

#### Théorème 3 {#alg-viii-s14-thm-3 .statement tag=00S9}

Soient A et B des K-algèbres simples, Z(A) et Z(B) leurs centres. On suppose que l’algèbre B est de degré fini sur K, et que l’algèbre $Z(A)\otimes_KZ(B)$est un corps (ce qui a lieu en particulier si A ou B est centrale). Soient $f$ et $g$ des homomorphismes de K-algèbres de B dans A. Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$.

D’après le lemme 1 de VIII, p. 250 il suffit de prouver que les $(B$, A)-bimodules $A^f$ et $A^g$ sont isomorphes. Or, on peut considérer $A^f$ et $A^g$ comme des modules à gauche sur l’algèbre $C = B\otimes_KA^o$, et cette dernière est simple d’après la prop. 7 de VIII, p. 217. Comme A-modules à droite, $A^f$ et $A^g$ sont isomorphes à $A_d$, donc de longueur finie puisque l’anneau A est simple (VIII, p. 117, cor. 1). A fortiori$, A^f$ et $A^g$ sont des C-modules de longueur finie. Soit S un C-module simple ; il existe des entiers strictement positifs $m$ et $n$ tels que $A^f$ soit isomorphe à $S^m$ et $A^g$ à $S^n$. Le A-module à droite S est donc de longueur finie non nulle. Comme les A-modules à droite sous-jacents à $A^f$ et $A^g$ sont isomorphes, ils ont même longueur ; on a donc $m=n$, de sorte que les C-modules $A^f$ et $A^g$ sont isomorphes.

#### Corollaire 1 {#alg-viii-s14-thm-3-cor-1 .statement tag=00GS}

Soit A une algèbre centrale et simple sur K, et soit L une extension de degré fini de K. Si $f$ et $g$ sont des homomorphismes de K-algèbres de L dans A, il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$.

#### Corollaire 2 {#alg-viii-s14-thm-3-cor-2 .statement tag=00GT}

Soit A une algèbre centrale et simple sur K et soit L une sous-algèbre de A qui est un corps. Tout homomorphisme de K-algèbre de L dans A se prolonge en un automorphisme intérieur de A.

#### Corollaire 3 {#alg-viii-s14-thm-3-cor-3 .statement tag=00GU}

Soit D un corps, de centre K, et de degré fini sur K. Tout élément de D est algébrique sur K. Soient $x$ et $y$ des éléments de D ; pour qu’il existe un élément $a$ de $D^*$ tel que $y=axa^{-1}$, il faut et il suffit que $x$ et $y$ aient même polynôme minimal sur K.

La première assertion résulte du cor. 1 de V, p. 16.

Supposons qu’il existe un élément $a$ de $D^*$ tel que $y=axa^{-1}$; pour tout polynôme P de K[X], on a $P(y) =aP(x)a^{-1}$, et en particulier on a $P(x) = 0$ si et seulement si $P(y) = 0$. Par suite $x$ et $y$ ont le même polynôme minimal sur K (V, p. 15, th. 1).

Réciproquement, supposons que $x$ et $y$ aient le même polynôme minimal. D’après loc. cit., il existe un K-isomorphisme $u$ de $K[x]$ sur $K[y]$ tel que $u(x) =y$, et $K[x]$ est un corps. D’après le cor. 2$,u$ se prolonge en un automorphisme intérieur $\theta :z\rightarrow aza^{-1}$ de D, et l’on a donc $y=\theta (x) =axa^{-1}$.

#### Proposition 1 {#alg-viii-s14-prop-1 .statement tag=00GV}

Soit A une algèbre centrale, simple et de degré fini sur K. Soit B une K-algèbre, soient $f$ et $g$ des homomorphismes d’algèbres de B dans A. Les conditions suivantes sont équivalentes :

(i) Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$;

(ii) En tant que B-modules à gauche, $A^f$ et $A^g$ sont isomorphes.

D’après le lemme 1 (VIII, p. 250), la propriété (i) équivaut au fait que $A^f$ et $A^g$ sont isomorphes comme $(B$, A)-bimodules. Comme A est de dimension finie sur K, $A^f$ et $A^g$ sont des B-modules de longueur finie. Comme le centre de A est égal à K , l’équivalence de (i) et (ii) résulte du lemme 2 de VIII, p. 250, appliqué au $(A^o,B^o$)-bimodules $A^f$ et $A^g$.

### 4. Automorphismes des algèbres semi-simples

#### Théorème 4 {#alg-viii-s14-thm-4 .statement tag=00GW}

Soient A un anneau semi-simple, Z son centre et $u$ un automorphisme de A. On suppose que A est un Z-module de type fini et que l’on a $u(z) =z$ pour tout $z$ dans Z. Alors $u$ est un automorphisme intérieur.

Cela résulte du th. 2 de VIII, p. 252 appliquée avec $f=$ Id$_A$ et $g=u$.

#### Exemple {#alg-viii-s14-n4-exa-1 .statement tag=00RH}

Le th. 4 s’applique dans les deux cas particuliers suivants :

a) Soient D un corps et Z son centre. Si D est de degré fini sur Z, tout auto$\dbend$ morphisme de D qui laisse fixes les éléments de Z est intérieur. L’hypothèse que D est de degré fini sur Z est essentielle (VIII, p. 265, exerc. 4).

b) Soit V un espace vectoriel de dimension finie sur le corps K. Tout automorphisme de la K-algèbre End$_K(V)$ est intérieur ; ce résultat s’étend au cas où l’espace V n’est pas de dimension finie sur K (VIII, p. 268, exerc. 13).

En particulier, tout automorphisme d’une algèbre de matrices $\mathbf{M}_n(K)$ (avec $n\geqslant 1)$ est intérieur. Ce résultat admet la généralisation suivante :

#### Proposition 2 {#alg-viii-s14-prop-2 .statement tag=00GX}

Soient L un anneau commutatif et V un L-module libre de dimension finie $m$. On suppose que tout L-module M tel que $M^m$ soit isomorphe à $L^m$ est isomorphe à L. Alors tout automorphisme de la L-algèbre End$_L(V)$est intérieur.

Posons B = End$_L(V)$. Soit $u$ un automorphisme de la L-algèbre B. Considérons V comme un B-module à gauche ; soit $u_*(V)$ le B-module à gauche associé à $u$, dont la loi d’action est $(b, v)\rightarrow u(b)(v)$ (II, p. 30). Soit $(e_1, . . . , e_m)$ une base du L-module V ; étant donnés des éléments $v_1, . . . , v_m$ de V, il existe un unique élément $b$ de B tel que l’on ait $b(e_i) =v_i$ pour $1\leqslant i\leqslant m$. Autrement dit, l’élément $e= (e_1, . . . , e_m)$ de $V^m$ fournit une base du B-module $V^m$. Comme $u$ est un automorphisme, $e$ donne aussi une base du B-module $u_*(V^m) =u_*(V)^m$, qui est donc isomorphe à $V^m$. Le $(B$, L)-bimodule V est inversible (VIII, p. 98, exemple 1) D’après le th. 2, b) de VIII, p. 99, il existe donc un L-module M tel que le B-module $u_*(V)$ soit isomorphe à $V\otimes_LM$. Les B-modules $V\otimes_LL^m$ et $V\otimes_LM^m$, respectivement isomorphes à $V^m$ et à $u_*(V)^m$ sont donc isomorphes. D’après loc. cit., les L-modules $L^m$ et $M^m$ sont isomorphes. Vu l’hypothèse faite, M est isomorphe à L ; par suite le B-module $u_*$(V), qui est isomorphe à $V\otimes_LM$, est isomorphe à V. Soit $h$ un isomorphisme de B-modules de V sur $u_*(V)$; c’est en particulier un automorphisme du L-module V, c’est-à-dire un élément inversible de B. Pour $b$ dans B et $v$ dans V, on a $h(b(v)) =u(b)(h(v))$, d’où $u(b) =hbh^{-1}$.

Les hypothèses de la prop. 2 sont satisfaites notamment lorsque l’anneau commutatif L est principal (VII, p. 14, cor. 3), ou artinien (VIII, p. 34, th. 2 d)), ou local (VIII, p. 33, cor. 6).

### 5. Sous-algèbres simples des algèbres simples

#### Théorème 5 {#alg-viii-s14-thm-5 .statement tag=00GY}

Soit A une K-algèbre centrale et simple et soit B une sous-algèbre de A, semi-simple et de degré fini sur K.

a) Le commutant $B'$ de B dans A est une sous-algèbre semi-simple et B est le commutant de $B'$ dans A. De plus l’algèbre $B\cap B'$ est une algèbre commutative semi-simple de degré fini sur K et c’est le centre commun de B et de $B'$.

b) Supposons que B soit simple. Alors $B'$ est simple et l’on a les égalités

$$
[A : B']_s= [B : K],[A : B]_s= [B': K],[A : K] = [B : K][B': K]
$$

(voir VIII, p. 120, déf. 2 pour la définition du degré $[A : B]_s)$.

La K-algèbre $A^o$ est centrale et simple et la K-algèbre B est semi-simple et de degré fini. D’après le cor. 1 de VIII, p. 217, l’algèbre $C = B\otimes_KA^o$ est semi-simple. Soit M le C-module ayant même groupe additif que A, avec la loi d’action caractérisée par la formule $(b\otimes a)a'=ba'a$, pour $a, a'$ dans A et $b$ dans B. Soit $u$ un élément de End$_{\mathbf{Z}}(A)$. Alors $u$ appartient au commutant $C'_M$ du C-module M si et seulement si $u$ est A-linéaire à droite et B-linéaire à gauche, ce qui revient à dire que $u$ apprtient au commutant de $B_M$ dans l’anneau des homothéties du A-module $A_s$. On définit donc un isomorphisme $\gamma$ de $B'$ sur $C'_M$ par la relation $\gamma (b')(x) =b'x$ pour $b'$ dans $B'$ et $x$ dans M. Or l’anneau C est semi-simple et le C-module M est engendré par l’élément 1 de A. D’après la prop. 6 de VIII, p. 135 l’anneau $C'_M$ est semi-simple, donc l’algèbre $B'$ est semi-simple.

Soit $\varphi$ l’homomorphisme de K-algèbres de $A\otimes_KA^o$ dans End$_K(M)$ qui associe à $a\otimes a'$ l’application K-linéaire $x\rightarrow axa'$ de M dans M. Comme les K-algèbres A et $A^o$ sont centrales et simples, les seuls idéaux bilatères de $A\otimes_KA^o$ sont 0 et $A\otimes_KA^o$ (VIII, p. 214, cor.). On a $C_M=\varphi (B\otimes A^o)$ et $C'_M=\varphi (B'\otimes K)$. L’homomorphisme $\varphi$ n’est pas nul ; il est donc injectif. L’anneau C étant semi-simple, on a $C''_M= C_M$ d’après la prop 5 de VIII, p. 135. Il en résulte que la sous-algèbre $B\otimes_KA^o$ de $A\otimes_KA^o$ est le commutant de la sous-algèbre $B'\otimes_KK$. Le commutant de $B'\otimes_KK$ dans $A\otimes_KK$ est donc égal à $(B\otimes_KA^o)\cap (A\otimes_KK)$, c’est-à-dire à $B\otimes K$ d’après la prop. 19 de II, p. 113. Donc le commutant de $B'$ dans A est égal à B. L’algèbre $L = B\cap B'$ est le centre de B. Comme B est une algèbre semi-simple de degré fini sur K, l’algèbre L est commutative, semi-simple et de degré fini sur K. Comme B est le commutant de $B'$ dans A, le centre de $B'$ est aussi égal à $L = B\cap B'$ (VIII, p. 73). On a prouvé a).

Supposons maintenant que l’algèbre B soit simple. D’après le cor. 2 de VIII, p. 217, l’anneau C est simple. D’après la prop. 4 de VIII, p. 119 appliquée au C-module M, dont le commutant est isomorphe à $B'$, l’anneau $B'$ est simple et M est un $B'$-module de longueur finie. Autrement dit, $B'$ est un sous-anneau simple de l’anneau simple A et le degré à gauche $[A : B']_s$ est un entier $m\geqslant 1$. Considéré comme $B'$-module à gauche, A possède une base finie $(a_1, . . . , a_m)$. De plus (loc. cit.$),\varphi$ induit par restriction un isomorphisme de C sur $C''_M=$ End$_{B'}$(A), et l’application $c\rightarrow (ca_1, . . . , ca_m)$ de C sur $A^m$ est donc bijective. Par suite, C est un A-module à droite libre de dimension $m$. Or on a $C = B\otimes A^o$, donc C est un A-module à droite libre de dimension [B : K], d’où $[A : B']_s=m= [B : K]$. De la prop. 6 de VIII, p. 121, on déduit

$$
[A : K] = [A : B']_s[B': K] = [B : K][B': K]
$$

comme on a aussi

$$
[A : K] = [A : B]_s[B : K]
$$

et que [B : K] est fini et non nul, on conclut à l’égalité $[A : B]_s= [B': K]$ (E, III, p. 49). On a prouvé b).

$\dbend$ Soit A une K-algèbre simple, centrale, de degré fini. Il peut exister des sous-algèbres commutatives semi-simples B de A satisfaisant à $[A : K]\not=$ $[B : K][B': K]$ (exerc. 1 de VIII, p. 265).

#### Théorème 6 {#alg-viii-s14-thm-6 .statement tag=00GZ}

Soient A une K-algèbre centrale et simple, B une sous-algèbre de degré fini de A et $B'$ son commutant dans A.

a) Supposons que B soit centrale et simple. Alors $B'$ est centrale et simple et l’homomorphisme de K-algèbres $\theta : B\otimes_KB'\rightarrow A$qui transforme $b\otimes b'$ en $bb'$ est un isomorphisme.

b) Supposons que B soit semi-simple et soit $L = B\cap B'$. Alors $B'$ est une algèbre semi-simple. Le commutant $L'$ de L dans A est un anneau semi-simple de centre L, et l’homomorphisme d’anneaux $\psi : B\otimes_LB'\rightarrow L'$ qui transforme $b\otimes b'$ en $bb'$ est un isomorphisme.

Prouvons a). Si B est centrale et simple, $B'$ est centrale et simple d’après le th. 5 de VIII, p. 255. Alors la K-algèbre $B\otimes_KB'$ est simple (VIII, p. 217, cor. 2) et l’homomorphisme $\theta : B\otimes_KB'\rightarrow A$ est injectif. Or, d’après l’égalité de $[A : B']_s$ et [B : K] (VIII, p. 255, th. 5), les $B'$-modules à gauche $B\otimes_KB'$ et A sont libres de même dimension finie ; ce sont donc des $B'$-modules ayant la même longueur finie. D’après le corollaire 2 de II, p. $22,\theta$ est bijectif.

Prouvons b). D’après le th. 5 de VIII, p. 255, l’algèbre L est commutative, de degré fini sur K et semi-simple. D’après loc. cit. appliqué à L, son commutant $L'$ dans A est une algèbre semi-simple et L est le commutant de $L'$ dans A, donc L est le centre de $L'$. Comme L est le centre des anneaux semi-simples $L', B$ et $B'$, on peut identifier $L'$ à un produit fini d’anneaux simples $L'_i(i\in I)$, de sorte que l’on ait

$$
L =\prod_{i\in I}L_i,B =\prod_{i\in I}B_i,B'=\prod_{i\in I}B'_i
$$

où $L_i$ est le centre de $L'_i$, et où $B_i$ et $B'_i$ sont des sous-algèbres de $L'_i$, de centre $L_i$, commutante l’une de l’autre dans $L'_i$. Considérons $L'_i$ comme une algèbre centrale et simple sur le corps commutatif $L_i$, et $B_i$ comme une $L_i$-algèbre centrale, simple et de degré fini. D’après l’assertion a), l’application canonique $\psi_i: B_i\otimes_{L_i}B'_i\rightarrow L'_i$ qui transforme $b_i\otimes b'_i$ en $b_ib'_i$ est un isomorphisme d’anneaux. Or on peut identifier $B\otimes_LB'$ à $\prod_{i\in I}(B_i\otimes_{L_i}B'_i)$ de sorte que $\psi$ soit le produit de la famille d’applications $(\psi_i)_{i\in I}$. Donc $\psi$ est un isomorphisme d’anneaux.

#### Corollaire {#alg-viii-s14-n5-cor-1 .statement tag=00H0}

Supposons que le corps K soit algébriquement clos et que A soit une algèbre simple et de degré fini sur K. Soit B une sous-algèbre simple de A et soit $B'$ le commutant de B dans A. Alors $B'$ est une K-algèbre simple, B est le commutant de $B'$, on a $[A : K] = [B : K][B': K]$et l’homomorphisme canonique de $B\otimes_KB'$ dans A est un isomorphisme de K-algèbres.

Comme toute algèbre simple de degré fini sur K est centrale, le corollaire résulte des théorèmes 5 et 6.

### 6. Sous-algèbres commutatives maximales

On dit qu’une sous-algèbre d’une K-algèbre A est une sous-algèbre commutative maximale de A si c’est un élément maximal de l’ensemble des sous-algèbres commutatives de A.

#### Lemme 3 {#alg-viii-s14-lem-3 .statement tag=00H1}

Soient A une K-algèbre et L une sous-algèbre de A.

a) Pour que L soit une sous-algèbre commutative maximale de A, il faut et il suffit que L soit égale à son commutant $L'$ dans A.

b) Soit $K'$ une K-algèbre commutative non nulle. Pour que L soit une sous-algèbre commutative maximale de A, il faut et il suffit que $L_{(K')}$ soit une sous-algèbre commutative maximale de $A_{(K')}$.

Prouvons a). Supposons d’abord que L soit égale à $L'$. Alors L est commutative ; si M est une sous-algèbre commutative de A contenant L, on a $xy=yx$ pour $x$ dans L et $y$ dans M, d’où $M\subset L'$ et donc M = L. Par suite, L est une sous-algèbre commutative maximale de A.

Réciproquement, supposons que L soit une sous-algèbre commutative maximale de A et soit $x$ un élément de $L'$. La sous-algèbre M de A engendrée par $L\cup  \{x\}$ est alors commutative et contient L. Vu le caractère maximal de L, on a M = L, d’où $x\in L$ et finalement $L = L'$, d’où a).

D’après la prop. 6 de III, p. 40, le commutant de $L_{(K')}$ dans $A_{(K')}$ est $L'_{(K')}$. Comme les égalités $L = L'$ et $L_{(K')}= L'_{(K')}$ sont équivalentes (II, p. 113, prop. 19), l’assertion b) résulte de a).

#### Proposition 3 {#alg-viii-s14-prop-3 .statement tag=00H2}

Soit A une K-algèbre centrale, simple et de degré fini et soit L une sous-algèbre commutative semi-simple de A. Les conditions suivantes sont équivalentes :

(i) L’algèbre L est une sous-algèbre commutative maximale de A ;

(ii) Le L-module à gauche A est libre, de dimension égale à [L : K] ;

(iii) On a $[A : K] = [L : K]^2$.

Supposons de plus que A soit l’algèbre End$_K(V)$, où V est un espace vectoriel de dimension finie non nulle sur K. Alors les conditions précédentes équivalent aussi à la suivante :

(iv) V est un L-module libre de dimension 1.

A) Supposons que A soit de la forme End$_K$(V), où V est un espace vectoriel de dimension finie non nulle sur le corps K. Nous établirons l’équivalence des conditions (i) à (iv) selon le schéma logique

(i) $=\Rightarrow$ (iv) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii) $=\Rightarrow$ (i) .

Comme L est une algèbre commutative, semi-simple, de degré fini sur K, on peut l’identifier à un produit fini $\prod_{i\in I}L_i$ d’extensions de degré fini de K (VIII, p. 133, prop. 3). Pour tout $i\in I$, soit $V_i$ le composant isotypique de type $L_i$ du L-module V, c’est un espace vectoriel de dimension finie non nulle sur $L_i$ car V est un L-module fidèle (VIII, p. 140, cor.). On peut alors identifier V à $\prod_{i\in I}V_i$. Dans ces conditions, le commutant $L'$ de L dans A, qui n’est autre que l’algèbre End$_L$(V), s’identifie au produit $\prod_{i\in I}$ End$_{L_i}(V_i)$.

Supposons que L soit une sous-algèbre commutative maximale de End$_K(V)$. D’après le lemme 3 a), on a $L = L'$, donc $L'$ est commutative et l’on a dim$_{L_i}(V_i) = 1$ pour tout $i\in I$. Ainsi (i) entraîne (iv).

Supposons que le L-module V soit libre de dimension 1. Soit $(e_1, . . . , e_r)$ une base de V sur K. L’application $a\rightarrow (ae_1, . . . , ae_r)$ est un isomorphisme de A-modules à gauche de A sur $V^r$ et donc de L-modules. Par suite, A est un L-module à gauche libre de dimension $r$, et l’on a $r=$ dim$_K(V) = [L : K]$. Donc (iv) entraîne (ii).

Il est clair que (ii) entraîne (iii).

Supposons enfin qu’on ait $[A : K] = [L : K]^2$, autrement dit dim$_K(V) = [L : K]$. On a donc $\sum_i$ dim$_{L_i}(V_i)[L_i: K] =\sum_i[L_i: K]$, de sorte que pour tout $i, V_i$ est de dimension 1 sur $L_i$. On a alors End$_{L_i}(V_i) = L_i$ pour tout $i$, d’où $L'= L$. D’après le lemme 3 a), L est une sous-algèbre commutative maximale de A. Donc (iii) entraîne (i).

B) Passons au cas général. D’après le th. 1 de VIII, p. 248, il existe une extension $K'$ de K, séparable et de degré fini, telle que la $K'$-algèbre $A_{(K')}$ soit isomorphe à une algèbre End$_{K'}(V')$, où $V'$ est un espace vectoriel de dimension finie non nulle sur $K'$. Alors la $K'$-algèbre $L_{(K')}$ est commutative et semi-simple (VIII, p. 218, cor. 2). D’après la première partie de la démonstration, les conditions suivantes sont équivalentes :

(i$')$ L’algèbre $L_{(K')}$ est une sous-algèbre commutative maximale de $A_{(K')}$;

(ii$')$ Le $L_{(K')}$-module à gauche $A_{(K')}$ est libre, de dimension $[L_{(K')}: K']$;

(iii$')$ On a $[A_{(K')}: K'] = [L_{(K')}: K']^2$.

D’après le lemme 3 b), les conditions (i) et (i’) sont équivalentes.

Posons $n= [L : K]$, d’où $n= [L_{(K')}: K']$; la condition (ii) signifie que les L-modules à gauche A et $L^n$ sont isomorphes ; d’après le th. 3 de VIII, p. 34, ceci équivaut à l’isomorphisme des $L_{(K')}$-modules $A_{(K')}$ et $(L_{(K')})^n$, d’où l’équivalence de (ii) et (ii$')$.

Enfin, on a $[A : K] = [A_{(K')}: K']$ et $[L : K] = [L_{(K')}: K']$, d’où l’équivalence des conditions (iii) et (iii$')$.

On a ainsi prouvé l’équivalence des conditions (i), (ii) et (iii).

#### Corollaire {#alg-viii-s14-n6-cor-1 .statement tag=00H3}

Soit A une algèbre centrale, simple et de degré fini sur K et soit L une K-algèbre commutative semi-simple telle que [A : K] soit égal à $[L : K]^2$;soient $f$ et $g$ des homomorphismes injectifs de L dans A. Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$.

Posons $n= [L : K]$. Considéré comme un module à gauche sur le sous-anneau $f$(L), A est libre de dimension $n:$ cela résulte de l’équivalence des conditions (ii) et (iii) de la prop. 3. Comme $f$ est un isomorphisme de L sur $f$(L), le L-module à gauche $A^f$ (dont la loi d’action est donnée par $(x, a)\rightarrow f(x)a)$ est libre de dimension $n$. Il en est de même de $A^g$, qui est donc isomorphe à $A^f$. On conclut en utilisant l’équivalence des conditions (i) et (ii) de la prop. 1 (VIII, p. 253).

$\dbend$ Supposons que A soit une algèbre centrale, simple et de degré fini sur K. Il peut exister des sous-algèbres commutatives maximales L de A, non semi-simples, telles que $[A : K]\not= [L : K]^2$ (VIII, p. 266, exerc. 5).

### 7. Sous-algèbres étales maximales

#### Lemme 4 {#alg-viii-s14-lem-4 .statement tag=00H4}

Soit A une algèbre centrale, simple et de degré fini sur K, distincte de K. Il existe une sous-algèbre étale (V, p. 28, déf. 1) de A, distincte de K.

D’après le théorème de Wedderburn (VIII, p. 116, th. 1), on peut supposer que A est de la forme $\mathbf{M}_n$(D), où $n$ est un entier strictement positif et D un corps de centre K.

Supposons $n >1$. L’algèbre des matrices diagonales à éléments dans K est une sous-algèbre étale de A distincte de K.

Supposons $n= 1$. Soit $p$ l’exposant caractéristique de D. Par le lemme 1 de VIII, p. 226, il existe un élément $a$ de D tel que $a^{p^m}$ n’appartienne à K pour aucun entier positif $m$. Pour $m$ assez grand, l’élément $x=a^{p^m}$ est séparable sur K (V, p. 42, prop. 13), mais n’appartient pas à K ; la sous-algèbre $K(x)$ de A est une extension séparable de degré fini du corps K, donc une sous-algèbre étale sur K ; elle est distincte de K.

#### Proposition 4 {#alg-viii-s14-prop-4 .statement tag=00H5}

Soit A une algèbre centrale, simple et de degré fini sur K. Soit L une sous-algèbre de A et soit $L'$ le commutant de L dans A.

a) Si L est maximale parmi les sous-algèbres commutatives semi-simples de A, on a $L = L'$ et L est une sous-algèbre commutative maximale de A.

b) Si L est maximale parmi les sous-algèbres étales de A, on a $L = L'$, et L est une sous-algèbre commutative maximale de A.

On sait que la relation $L = L'$ signifie que L est une sous-algèbre commutative maximale de A (VIII, p. 257, lemme 3 a)). Supposons que L soit semi-simple, commutative et distincte de $L'$. D’après le th. 5 de VIII, p. 255, $L'$ est semi-simple, et L est le commutant de $L'$, donc le centre de $L'$; par suite, $L'$ n’est pas commutative. Il nous suffit de prouver qu’il existe une sous-algèbre semi-simple commutative M de A, distincte de L et contenant L, et qui est étale si L est étale.

D’après le théorème de structure des anneaux semi-simples (VIII, p. 131, th. 1), il existe des anneaux simples $B_1, . . . ,B_r$ et un isomorphisme $\varphi$ de $L'$ sur $B_1\times  \cdots  \times B_r$. Pour 1 $\leqslant i\leqslant r$, notons $E_i$ le centre de $B_i$; on a donc $\varphi (L) = E_1\times  \cdots  \times E_r$. Comme $L'$ n’est pas commutative, on peut supposer que $B_1$, par exemple, n’est pas commutative ; on a donc $B_1\not= E_1$, et d’après le lemme 4, il existe une sous-algèbre $M_1$ de $B_1$, commutative, distincte de $E_1$, et étale sur $E_1$. Posons $M =\varphi^{-1}(M_1\times E_2\times  \cdots  \times E_r)$; c’est une sous-algèbre commutative semi-simple de A, contenant L et distincte de L. Supposons que L soit étale sur K et démontrons que M est étale. Les extensions $E_i$ de K sont séparables (V, p. 29, prop. 3). De plus, comme la $E_1$-algèbre $M_1$ et la K-algèbre $E_1$ sont étales, la K-algèbre $M_1$ est étale (V, p. 32, cor. 2). Ainsi la K-algèbre $M_1\times E_2\times  \cdots  \times E_r$ est étale, donc M a la même propriété.

Soit A une algèbre simple centrale et de degré fini sur K. Une sous-algèbre de A maximale parmi les sous-algèbres commutatives semi-simples de A est appelée une sous-algèbre semi-simple commutative maximale de A. D’après la prop. 4, le qualificatif « maximal » se rapporte donc au choix à la propriété d’être commutative, ou semi-simple et commutative. Une sous-algèbre de A maximale parmi les sous-algèbres étales de A est appelée une sous-algèbre semi-simple étale maximale de A.

#### Corollaire 1 {#alg-viii-s14-prop-4-cor-1 .statement tag=00H6}

Soit A une K-algèbre centrale, simple et de degré fini. Toute sous-algèbre semi-simple (resp. étale) commutative de A est contenue dans une sous-algèbre commutative maximale de A qui est semi-simple (resp. étale).

#### Corollaire 2 {#alg-viii-s14-prop-4-cor-2 .statement tag=00H7}

Soit D un corps de centre K et de degré fini sur K.

a) Les sous-corps commutatifs maximaux de D sont les sous-algèbres commutatives maximales de D et aussi les sous-algèbres semi-simples commutatives maximales de D. Tout sous-corps commutatif L de D est contenu dans un sous-corps commutatif maximal.

b) Soit L un sous-corps commutatif de D qui est une extension séparable de K, alors il est contenu dans un sous-corps commutatif maximal de D qui est une extension séparable de K.

c) Soit L un sous-corps commutatif de D. Pour que L soit un sous-corps commutatif maximal de D, il faut et il suffit qu’on ait $[D : K] = [L : K]^2$.

Une sous-algèbre de D est un corps (V, p. 10, prop. 1) et donc semi-simple. De plus, un sous-corps commutatif maximal de D contient K. Les assertions a) et b) résultent alors du cor. 1 et l’assertion c) de la prop. 3 (VIII, p. 258).

#### Proposition 5 {#alg-viii-s14-prop-5 .statement tag=00H8}

Soit A une algèbre centrale, simple et de degré fini sur K. Soit B une sous-algèbre semi-simple de A et soit $B'$ le commutant de B.

a) Pour que B contienne une sous-algèbre semi-simple commutative maximale de A, il faut et il suffit que B contienne $B'$.

b) Supposons que B contienne $B'$ et soit $g$ un homomorphisme de K-algèbres de B dans A. Il existe un automorphisme intérieur $\theta$ de A qui coïncide avec $g$ sur B.

Soit L une sous-algèbre commutative maximale de A ; d’après le lemme 3 de VIII, p. 257, L est égale à son commutant $L'$ dans A. Si B contient L, son commutant $B'$ est contenu dans $L'$ et donc dans B.

Réciproquement, supposons que $B'$ soit contenu dans B. Alors $B'$ est le centre de B et c’est une algèbre semi-simple commutative (VIII, p. 133, prop. 2). D’après le corollaire 1 ci-dessus, il existe une sous-algèbre semi-simple commutative maximale L de A, contenant $B'$. Le commutant de L est L (VIII, p. 257, lemme 3 a)) et celui de $B'$ est égal à B (VIII, p. 255, th. 5). La relation $L\supset B'$ entraîne donc $L\subset B$. On a prouvé a).

Prouvons b). Supposons que B contienne $B'$ et choisissons, d’après a), une sous-algèbre semi-simple commutative maximale L de A, contenue dans B. Soit $g$ un homomorphisme de B dans A. D’après la prop. 3 de VIII, p. 258 on a l’égalité $[A : K] = [L : K]^2$; d’après le cor. de VIII, p. 259, il existe un automorphisme intérieur $\theta_1$ de A, qui coïncide avec $g$ sur L. Si $f$ est l’injection canonique de B dans A, les homomorphismes $g$ et $\theta_1\circ f$ ont même restriction au centre $B'$ de B car $B'$ est contenu dans L. D’après le th. 2 de VIII, p. 252, il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$; autrement dit, $\theta$ prolonge $g$.

### 8. Sous-algèbres diagonalisables des algèbres simples

Soit D une K-algèbre qui est un corps et soit V un espace vectoriel à droite de dimension finie sur D. Soit L une sous-K-algèbre de End$_D(V)$ qui est une K-algèbre diagonalisable (V, p. 28). Par définition, L est de degré fini sur K, et il existe une base $(\varepsilon_i)_{i\in I}$ de L sur K, avec les propriétés suivantes :

$\varepsilon^2_i=\varepsilon_i, \varepsilon_i\varepsilon_j= 0$ si $i\not=j,\sum_{i\in I}\varepsilon_i= 1$.

Posons $V_i=\varepsilon_i(V)$ pour tout $i$ dans I ; alors $(V_i)_{i\in I}$ est une famille de sous-espaces vectoriels de V non nuls, dont V est la somme directe (II, p. 18, prop. 12). Soit $u$ un endomorphisme de V ; pour que $u$ appartienne à L, il faut et il suffit que, pour tout $i\in I$, il existe un élément $\lambda_i$ de K tel que $u(x) =\lambda_ix$ pour tout $x\in V_i$.

Réciproquement, supposons que V soit somme directe d’une famille $(V_i)_{i\in I}$ de sous-espaces vectoriels non réduits à 0. Pour tout élément $\boldsymbol{\lambda }= (\lambda_i)_{i\in I}$ de $K^I$, notons $u_{\boldsymbol{\lambda }}$ l’endomorphisme du D-espace vectoriel V tel que $u_{\boldsymbol{\lambda }}(x) =\lambda_ix$ pour $x\in V_i$. L’ensemble L des endomorphismes $u_{\boldsymbol{\lambda }}$, pour $\boldsymbol{\lambda }\in K^I$, est une sous-algèbre diagonalisable de End$_D$(V), admettant pour base la famille $(\varepsilon_i)_{i\in I}$, où $\varepsilon_i$ est le projecteur d’image $V_i$, de noyau $\sum_{j\not=i}V_j$. On dit que L est la sous-algèbre diagonalisable de End$_D(V)$ associée à la décomposition en somme directe $V =\oplus_{i\in I}V_i$. On a [L : K] = Card(I) $\leqslant$ dim$_D(V)$.

#### Proposition 6 {#alg-viii-s14-prop-6 .statement tag=00H9}

Soit L la sous-algèbre diagonalisable de End$_D(V)$associée à une décomposition en somme directe $V =\oplus_{i\in I}V_i$.

a) Pour que L soit maximale parmi les sous-algèbres diagonalisables de la K-algèbre End$_D(V)$, il faut et il suffit que chacun des $V_i$ soit de dimension 1 sur D.

b) Pour que L soit une sous-algèbre commutative maximale de End$_D(V)$, il faut et il suffit que l’on ait D = K et que chaque $V_i$ soit de dimension 1 sur K.

Si chacun des espaces vectoriels $V_i$ est de dimension 1 sur D, on a

[L : K] = Card(I) = dim$_D(V)$,

donc L est maximal parmi les sous-algèbres diagonalisables de End$_D(V)$. Dans le cas contraire, il existe un indice $j\in I$ tel que dim$_D(V_j)\geqslant 2$. Choisissons deux sous-espaces vectoriels non nuls $V'_j$ et $V_j''$ de $V_j$ dont $V_j$ soit somme directe. La sous-algèbre diagonalisable de End$_D(V)$ associée à la décomposition en somme directe $V = (\oplus_{i\in I\{j\}}V_i)\oplus V'_j\oplus V_j''$ contient L et n’est pas égale à L, d’où a).

Le commutant $L'$ de L dans End$_D(V)$ se compose des endomorphismes de la forme $(x_i)\rightarrow (u_i(x_i))$, avec $(u_i)\in \prod_{i\in I}$ End$_D(V_i)$. Pour que L soit une sous-algèbre commutative maximale de End$_D$(V), il faut et il suffit que l’on ait $L = L'$ (VIII, p. 257, lemme 3 a)). Cette relation équivaut donc à « End$_D(V_i) = K$ pour tout $i\in I$ », d’où l’assertion b).

#### Proposition 7 {#alg-viii-s14-prop-7 .statement tag=00HA}

Soit L une algèbre commutative de degré fini sur K. Les assertions suivantes sont équivalentes :

(i) L’algèbre L est étale ;

(ii) Il existe une extension séparable de degré fini de K qui diagonalise K.

L’implication (ii)$\Rightarrow$(i) résulte de V, p. 29, prop. 2.

Démontrons l’implication (i)$\Rightarrow$(ii). Soit Ω une clôture séparable de K. D’après le th. 4 de V, p. 34, il existe des extensions de degré fini $L_1, . . . ,L_n$ de K, contenues dans Ω telles que L soit isomorphe au produit $L_1\times  \cdots  \times L_n$. Soit N une extension galoisienne de K qui contient les $L_i$ (V, p. 56) et démontrons que $A_{(N)}$ est diagonalisable. Par le théorème de l’élément primitif, (V, p. 39, th. 1), pour tout $i\in [1, n]$, il existe un polynôme séparable irréductible $P_i\in K[X]$ tel que $L_i$ soit isomorphe à $K[X]/(P_i)$. Comme N est une extension normale de K, dans laquelle $P_i$ admet une racine, le polynôme $P_i$ est scindé à racines simples dans N. Par conséquent, la N-algèbre $L_{i(N)}$, qui est isomorphe à $N[X]/(P_i)$ est isomorphe à $N^{[L_i:K]}$. Par suite, $A_{(N)}$ est diagonalisable.

#### Théorème 7 {#alg-viii-s14-thm-7 .statement tag=00HB}

Soient A une K-algèbre centrale, simple et de degré fini, et L une sous-algèbre de A. Les conditions suivantes sont équivalentes :

(i) L’algèbre L est une sous-algèbre étale maximale de A ;

(ii) Il existe une extension $K'$ de K, un entier $n\geqslant 1$et un isomorphisme $\theta$ de $A_{(K')}$ sur $\mathbf{M}_n(K')$qui transforme $L_{(K')}$ en l’ensemble des matrices diagonales ;

(iii) Il existe $K',n$ et $\theta$ comme dans (ii), l’extension $K'$ étant de plus supposée galoisienne et de degré fini.

Il est clair que (iii) entraîne (ii).

Si la condition (ii) est satisfaite, $L_{(K')}$ est une sous-algèbre commutative maximale de $A_{(K')}$ (prop. 6) et elle est diagonalisable. La K-algèbre L est alors étale (V, p. 28, déf. 1) et c’est une sous-algèbre commutative maximale de A (VIII, p. 257, lemme 3 b)). On a prouvé que (ii) entraîne (i).

Supposons la condition (i) satisfaite. Comme L est étale sur K, d’après la prop. 7 il existe une extension $K_1$ de K, galoisienne et de degré fini telle que la $K_1$-algèbre $L_{(K_1)}$ soit diagonalisable. L’algèbre A est centrale et simple ; d’après (VIII, p. 248, th. 1), il existe une extension galoisienne $K_2$, un espace vectoriel V de dimension finie $n$ sur $K_2$ et un isomorphisme $\theta$ de $A_{(K_2)}$ sur End$_{K_2}(V)$. Par la prop. 1 de V, p. 55, on peut supposer que $K_1= K_2$. D’après la prop. 4, b) de VIII, p. 260 et le lemme 3, b) (VIII, p. 257), $L_{(K')}$ est une sous-algèbre commutative maximale de $A_{(K')}$, donc $\theta (L_{(K')})$ en est une de End$_{K'}(V')$. Appliquons la prop. 6 à l’algèbre diagonalisable $\theta (L_{(K')}) :$ il existe une base $(e_1, . . . , e_n)$ de $V'$ sur $K'$ telle que $\theta (L_{(K')})$ se compose des endomorphismes de $V'$ dont la matrice par rapport à cette base soit diagonale. Donc (i) entraîne (iii).

## EXERCICES {#alg-viii-s14-exercises}

See the [exercises for § 14](exercises/s14/).
