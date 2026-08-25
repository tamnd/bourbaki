---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 13
section_title: Algèbres absolument semi-simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.225-A VIII.245
pdf_pages: 0229-0249
extraction: native+ocr
subsections:
    - "no": 1
      title: Modules absolument semi-simples
      page: 225
      pdf_page: 229
    - "no": 2
      title: Algèbres sur un corps séparablement clos
      page: 226
      pdf_page: 230
    - "no": 3
      title: Algèbres absolument semi-simples
      page: 227
      pdf_page: 231
    - "no": 4
      title: Caractérisation des modules absolument semi-simples
      page: 231
      pdf_page: 235
    - "no": 5
      title: Dérivations des algèbres semi-simples
      page: 232
      pdf_page: 236
    - "no": 6
      title: Cohomologie des algèbres
      page: 234
      pdf_page: 238
    - "no": 7
      title: Cohomologie des algèbres absolument semi-simples
      page: 236
      pdf_page: 240
    - "no": 8
      title: Scindage des algèbres artiniennes
      page: 238
      pdf_page: 242
statements: 33
exercises: 12
content_sha256: 69ef354b36df371c66828c6697791beb8ef7b87a519d89572e110234691e3e5a
---

## § 13. ALGÈBRES ABSOLUMENT SEMI-SIMPLES

### 1. Modules absolument semi-simples

#### Définition 1 {#alg-viii-s13-def-1 .statement tag=00F9}

Soient K un corps commutatif et A une K-algèbre. On dit qu’un A-module M est absolument semi-simple si le $A_{(L)}$-module $M_{(L)}$ est semi-simple pour toute extension L de K.

Tout module absolument semi-simple est semi-simple. Réciproquement, si le corps K est parfait, tout A-module semi-simple qui est de dimension finie sur K est absolument semi-simple (VIII, p. 218, cor. 1 a)), car toute extension d’un corps parfait est séparable (V, p. 35, prop. 2).

#### Proposition 1 {#alg-viii-s13-prop-1 .statement tag=00FA}

Soit K un corps commutatif et soit A une K-algèbre.

a) Toute somme directe de A-modules absolument semi-simples est un A-module absolument semi-simple. Tout sous-module et tout module quotient d’un module absolument semi-simple est un module absolument semi-simple.

b) Soient M un A-module et L une extension du corps K. Pour que le A-module M soit absolument semi-simple, il faut et il suffit que le $A_{(L)}$-module $M_{(L)}$ soit absolument semi-simple.

L’assertion a) résulte de l’assertion analogue pour les modules semi-simples (VIII, p. 52, cor. 1 et 3).

Supposons que le A-module M soit absolument semi-simple et soit $L'$ une extension de L. En tant que $A_{(L')}$-module, $L'\otimes_LM_{(L)}$ est isomorphe à $M_{(L')}$ (II, p. 83, prop. 2) ; c’est donc un module semi-simple. Ceci prouve que $M_{(L)}$ est absolument semi-simple.

Réciproquement, supposons que $M_{(L)}$ soit absolument semi-simple. Soit $L'$ une extension de K. Il existe une extension composée $(\Omega , u, v)$ de L et $L'$ (V, p. 12, cor.) ; identifions L et $L'$ à des sous-extensions de Ω. Le $A_{(\Omega )}$-module $M_{(\Omega )}$ est isomorphe à $(M_{(L)})_{(\Omega )}$, donc il est semi-simple. Mais $M_{(\Omega )}$ est aussi isomorphe à $(M_{(L')})_{(\Omega )}$, et la prop. 8, a) de VIII, p. 217 entraîne que $M_{(L')}$ est semi-simple. Donc M est absolument semi-simple.

#### Proposition 2 {#alg-viii-s13-prop-2 .statement tag=00FB}

Soient K un corps commutatif, A une K-algèbre et M un A-module de dimension finie sur K. Les conditions suivantes sont équivalentes :

(i) Le A-module M est absolument semi-simple ;

(ii) Il existe une extension P de K, qui est un corps parfait, telle que le $A_{(P)}$-module $M_{(P)}$ soit semi-simple ;

(iii) Le A-module M est semi-simple et le centre de son commutant est une algèbre étale sur le corps K.

Il est clair que (i) entraîne (ii). Par ailleurs, sous les hypothèses de (ii), le $A_{(P)}$-module $M_{(P)}$ est absolument semi-simple d’après le cor. 1, a) de VIII, p. 218. D’après la prop. 1, b), M est alors absolument semi-simple. Donc (ii) entraîne (i).

Supposons M semi-simple. Soit Z le centre du commutant de M ; c’est une algèbre commutative de degré fini sur le corps K. Si L est une extension de K, il résulte de la prop. 8, b) de VIII, p. 217. que le $A_{(L)}$-module $M_{(L)}$ est semi-simple si et seulement si l’anneau $Z_{(L)}$ est réduit. L’équivalence de (i) et (iii) résulte donc du th. 4 de V, p. 34.

### 2. Algèbres sur un corps séparablement clos

#### Lemme 1 {#alg-viii-s13-lem-1 .statement tag=00FC}

Soit D un corps et soit Z son centre. Notons $p$ l’exposant caractéristique de Z. On suppose que pour tout élément $a$ de D, il existe un entier $m\geqslant 0$tel que $a^{p^m}$ appartienne à Z. Alors le corps D est commutatif.

Si $p= 1$, alors D = Z. Nous supposons donc $p >1$.

Raisonnons par l’absurde en supposant D non commutatif. Soient $a$ un élément de $D-Z$, et $q$ une puissance de $p$ telle que $a^q$ appartienne à Z. Notons I l’application identique de D et $\sigma$ l’automorphisme intérieur $x\rightarrow axa^{-1}$ de D dans D associé à $a$; on a $\sigma^q= I$, car $a^q$ appartient à Z. On a $\sigma -I\not= 0$ car $a$ n’appartient pas à Z, et $(\sigma -I)^q=\sigma^q-I = 0$ car Z est de caractéristique $p$. Soit $f$ le plus grand entier positif tel qu’on ait $(\sigma -I)^f\not= 0$; on a $f\geqslant 1$. Choisissons un élément $c$ de D tel que $(\sigma -I)^f(c)\not= 0$ et posons

$$
x= (\sigma -I)^{f-1}(c),y= (\sigma -I)(x) = (\sigma -I)^f(c)
$$

Par construction, on a $y\not= 0$ et $\sigma (y) =y$; si l’on pose $z=y^{-1}x$, on en déduit

$$
\sigma (z) =\sigma (y)^{-1}\sigma (x) =y^{-1}(y+x) = 1 +z
$$

d’où $\sigma (z^{p^j}) = 1 +z^{p^j}$ pour tout entier positif $j$. Choisissons un entier $m\geqslant 0$ tel que $z^{p^m}$ appartienne au centre Z de D ; on a

$$
z^{p^m}=az^{p^m}a^{-1}=\sigma (z^{p^m}) = 1 +z^{p^m}
$$

et cette contradiction établit le lemme 1.

#### Proposition 3 {#alg-viii-s13-prop-3 .statement tag=00FD}

Soit K un corps séparablement clos (V, p. 43, déf. 4) et soit D une algèbre de degré fini sur K qui est un corps. Alors D est commutative.

Notons $p$ l’exposant caractéristique de K. Soit $a$ un élément de D. L’anneau $K[a]$ est une extension algébrique de K (V, p. 16, cor. 1). Comme le corps K est séparablement clos, il résulte de V, p. 42, prop. 13 que l’algèbre $K[a]$ est une extension radicielle de K. Il existe donc un entier $m\geqslant 0$ tel que $a^{p^m}$ appartienne à K. Compte tenu du lemme 1, le corps D est commutatif.

#### Corollaire {#alg-viii-s13-n2-cor-1 .statement tag=00FE}

Soient K un corps séparablement clos et A une algèbre semi-simple de degré fini sur K. Il existe alors un entier $r\geqslant 0$, des entiers strictement positifs $n_1, . . . , n_r$ et des extensions $K_1, . . . ,K_r$ de degré fini de K, tels que A soit isomorphe à l’algèbre $\prod^r_{i=1}\mathbf{M}_{n_i}(K_i)$.

D’après le théorème de structure des algèbres semi-simples (VIII, p. 131, th. 1), A est isomorphe à une algèbre $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ où $r$ est un entier $\geqslant 0,n_1, . . . , n_r$ des entiers strictement positifs, $D_1, . . . ,D_r$ des K-algèbres de degré fini qui sont des corps. Comme le corps K est séparablement clos, chaque corps $D_i$ est commutatif d’après la prop. 3, d’où le corollaire.

### 3. Algèbres absolument semi-simples

#### Définition 2 {#alg-viii-s13-def-2 .statement tag=00FF}

Soit K un corps commutatif. On dit qu’une K-algèbre A est absolument semi-simple si l’anneau $A_{(L)}$ est semi-simple pour toute extension L de K.

Une algèbre absolument semi-simple est semi-simple. La K-algèbre A est absolument semi-simple si et seulement si le A-module $A_s$ est absolument semi-simple. Compte tenu de la prop. 1 de VIII, p. 225, on obtient donc le résultat suivant : si L est une extension de K, la L-algèbre $A_{(L)}$ est absolument semi-simple si et seulement si la K-algèbre A est absolument semi-simple.

#### Théorème 1 {#alg-viii-s13-thm-1 .statement tag=00FG}

Soient K un corps commutatif et A une K-algèbre. Les conditions suivantes sont équivalentes :

(i) La K-algèbre A est absolument semi-simple ;

(ii) L’algèbre A est de degré fini sur K et il existe une extension P de K qui est un corps parfait et telle que la P-algèbre $A_{(P)}$ soit semi-simple ;

(iii) La K-algèbre A est semi-simple, de degré fini sur K, et son centre est une K-algèbre étale ;

(iv) Il existe une famille finie $(n_i,D_i)_{i\in I}$, où $n_i$ est un entier strictement positif, et $D_i$ une K-algèbre de degré fini qui est un corps, telle que le centre $Z_i$ de $D_i$ soit une extension séparable de K, et que A soit isomorphe au produit des anneaux de matrices $\mathbf{M}_{n_i}(D_i)$;

(v) Il existe une extension L de K et une famille finie d’entiers $(n_i)_{i\in I}$ telle que la L-algèbre $A_{(L)}$ soit isomorphe à l’algèbre $\prod_{i\in I}\mathbf{M}_{n_i}(L)$;

(vi) Il existe une extension L de K, galoisienne et de degré fini et une famille finie d’entiers $(n_i)$telle que $A_{(L)}$ soit isomorphe au produit des algèbres de matrices $\mathbf{M}_{n_i}(L)$.

Nous prouverons d’abord les implications (v) $=\Rightarrow$ (iv) $=\Rightarrow$ (iii) $=\Rightarrow$ (ii) $=\Rightarrow$ (i). Notons Z le centre de A.

Si la propriété (v) est satisfaite, la L-algèbre $A_{(L)}$ est semi-simple, de degré fini sur L, et son centre (isomorphe à $Z_{(L)}$, III, p. 41, cor.) est isomorphe à $L^r$ pour un certain entier $r\geqslant 0$. D’après le cor. 2, a) de VIII, p. 218, l’algèbre A est semi-simple et de degré fini sur K. Elle est donc isomorphe à un produit fini d’anneaux $\prod_{i\in I}\mathbf{M}_{n_i}(D_i)$ avec $n_i\geqslant 1$ pour tout $i\in I$, le corps $D_i$ étant une algèbre de degré fini sur K. Le centre $Z_i$ de $D_i$ est un corps commutatif extension de K et Z est isomorphe à $\prod_{i\in I}Z_i$. Donc $Z_{(L)}$ est isomorphe d’une part à $\prod_{i\in I}(Z_i)_{(L)}$, d’autre part à $L^r$. Autrement dit, l’algèbre $\prod_{i\in I}Z_i$ est étale sur le corps K et chacune des extensions $Z_i$ est séparable sur K (V, p. 30, cor.). Donc (v) entraîne (iv).

Si la propriété (iv) est satisfaite, il est clair que A est une algèbre semi-simple et de degré fini sur K. Son centre Z est isomorphe au produit $\prod_{i\in I}Z_i$ d’extensions séparables de degré fini de K ; c’est donc une algèbre étale. Donc (iv) entraîne (iii).

Les implications (iii) $=\Rightarrow$ (ii) $=\Rightarrow$ (i) résultent de la prop. 2 de VIII, p. 226 appliquée au A-module $M = A_s$.

#### Lemme 2 {#alg-viii-s13-lem-2 .statement tag=00FH}

Soient L un corps algébriquement clos et D un corps contenant L dans son centre. Si D est distinct de L, il existe une extension $L'$ de L telle que l’anneau $D\otimes_LL'$ ne soit pas artinien à gauche.

Soit $x$ un élément de D - L ; comme L est algébriquement clos, l’extension $L'= L(x)$ de L n’est pas algébrique et $x$ est transcendant sur L. L’anneau $B = L'\otimes_LL'$ est alors intègre d’après la prop. 5 de V, p. 135.

L’élément $y=x\otimes 1-1\otimes x$ de B n’est pas nul ; mais si $\varphi$ est l’homomorphisme de B dans $L'$ qui transforme $\xi \otimes \eta$ en $\xi \eta$, on a $\varphi (y) = 0$, donc $y$ n’est pas inversible dans B. Considérons l’anneau $C = D\otimes_LL'$ comme module à droite sur son sous-anneau B ; c’est un module libre puisque D est un espace vectoriel à droite sur son sous-corps $L'$. Comme $y$ est un élément non nul et non inversible de l’anneau intègre B, la multiplication à droite par $y$ dans C est une application $R_y$ qui est injective, mais non bijective. Or $R_y$ est un endomorphisme du C-module à gauche $C_s$; par suite (VIII, p. 26, cor. 1), l’anneau C n’est pas artinien à gauche.

Prouvons maintenant que (i) entraîne (v). Cela résulte du lemme suivant :

#### Lemme 3 {#alg-viii-s13-lem-3 .statement tag=00FI}

Soient A une K-algèbre absolument semi-simple et L une extension algébriquement close de K. Alors l’algèbre $A_{(L)}$ est isomorphe à un produit d’un nombre fini d’algèbres de matrices sur L.

La L-algèbre $A_{(L)}$ est semi-simple ; elle est donc isomorphe au produit d’un nombre fini d’algèbres de la forme $\mathbf{M}_{n_i}(D_i)$, où $D_i$ est un corps contenant L dans son centre et $n_i$ un entier $\geqslant 1$ (VIII, p. 133, remarque 1).

Soit $L'$ une extension de L. Comme la K-algèbre A est absolument semi-simple, l’anneau $A_{(L')}$ est semi-simple, donc artinien à gauche. Or, l’anneau $A_{(L')}$ est isomorphe à $L'\otimes_LA_{(L)}$, donc à $\prod_{i\in I}\mathbf{M}_{n_i}(L'\otimes_LD_i)$; d’après la prop. 5 de VIII, p. 7, chacun des anneaux $\mathbf{M}_{n_i}(L'\otimes_LD_i)$ est donc artinien à gauche.

Soient $n\geqslant 1$ un entier et B un anneau ; soit $(\mathfrak{b}_r)_{r\geqslant 0}$ une suite décroissante d’idéaux à gauche de B ; notons $\mathfrak{c}_r$ l’ensemble des matrices carrées d’ordre $n$ à éléments dans $\mathfrak{b}_r$. Alors $(\mathfrak{c}_r)_{r\geqslant 0}$ est une suite décroissante d’idéaux à gauche de $\mathbf{M}_n(B)$. En particulier, si l’anneau $\mathbf{M}_n(B)$ est artinien à gauche, il en est de même de B.

D’après ce qui précède, pour tout $i\in I$, et toute extension $L'$ de L, l’anneau $D_i\otimes_LL'$ est artinien à gauche. D’après le lemme 2, on a $D_i= L$ pour tout $i\in I$, ce qui entraîne le lemme 3.

Pour démontrer l’implication (i)$\Rightarrow$(vi) nous utiliserons le lemme suivant :

#### Lemme 4 {#alg-viii-s13-lem-4 .statement tag=00FJ}

Soient A et B des algèbres sur le corps K, possédant des systèmes générateurs finis ; soit $K'$ une extension de K. Si les $K'$-algèbres $A_{(K')}$ et $B_{(K')}$ sont isomorphes, il existe une sous-extension L de $K'$, de type fini sur K, telle que les L-algèbres $A_{(L)}$ et $B_{(L)}$ soient isomorphes.

Soient $(e_i)_{i\in I}$ et $(f_j)_{j\in J}$ des systèmes générateurs finis des algèbres A et B respectivement. Soit $u$ un isomorphisme de $A_{(K')}$ sur $B_{(K')}$ et $v$ l’isomorphisme réciproque ; il existe une sous-extension L de $K'$, de type fini sur K, telle que l’on ait $u(1\otimes e_i)\in B_{(L)}$ pour tout $i\in I$ et $v(1\otimes f_j)\in A_{(L)}$ pour tout $j\in J$. Par suite $u$ applique $A_{(L)}$ dans $B_{(L)}$ et $v$ applique $B_{(L)}$ dans $A_{(L)}$. Les applications induites $u': A_{(L)}\rightarrow B_{(L)}$ et $v': B_{(L)}\rightarrow A_{(L)}$ sont des homomorphismes d’anneaux, et ce sont des bijections réciproques l’une de l’autre.

Terminons la démonstration de l’implication (i)$\Rightarrow$(vi) Notons $K'$ une clôture séparable de K (V, p. 44). Alors $A_{(K')}$ est une algèbre absolument semi-simple sur $K'$. Par l’implication (i)$\Rightarrow$(iv), la $K'$-algèbre $A_{(K')}$ est isomorphe à un produit $\mathbf{M}_{n_1}(D_1)\times$ $\cdots  \times \mathbf{M}_{n_r}(D_r)$, où $D_i$ est une $K'$-algèbre de degré fini qui est un corps et dont le centre $Z_i$ est une extension séparable de $K'$. Comme $K'$ est séparablement clos, on a $Z_i= K'$. D’après la prop. 3 de VIII, p. 227, le corps $D_i$ est commutatif. On a donc $D_i= K'$. Notons B la K-algèbre $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$. Les $K'$-algèbres $A_{(K')}$ et $B_{(K')}$ sont isomorphes d’après ce qui précède. Toute sous-extension de $K'$, de type fini sur K, est séparable et de degré fini sur K, donc contenue dans une sous-extension L de $K'$, galoisienne et de degré fini sur K (V, p. 55, prop. 2). L’implication résulte donc du lemme 4 de VIII, p. 229.

L’implication (vi)$\Rightarrow$(v) est immédiate.

#### Corollaire 1 {#alg-viii-s13-lem-4-cor-1 .statement tag=00FK}

Soient K un corps commutatif, $A_1$ et $A_2$ des K-algèbres. On suppose que $A_1$ est absolument semi-simple.

a) Si $A_2$ est semi-simple, il en est de même de $A_1\otimes_KA_2$.

b) Si $A_2$ est absolument semi-simple, il en est de même de $A_1\otimes_KA_2$.

Notons $Z_1$ le centre de $A_1$ et $Z_2$ celui de $A_2$. Le centre Z de $A_1\otimes_KA_2$ est égal à $Z_1\otimes_KZ_2$ d’après le corollaire de III, p. 41. Supposons $A_2$ semi-simple ; alors $Z_2$ est une algèbre réduite (VIII, p. 133, prop. 2 et 3). D’après le th. 1, $Z_1$ est une K-algèbre étale, donc séparable. D’après la prop. 5 de V, p. 115, l’anneau $Z = Z_1\otimes_KZ_2$ est réduit ; comme $A_1$ est de degré fini sur K (th. 1), il résulte de la prop. 7 de VIII, p. 217, que l’anneau $A_1\otimes_KA_2$ est semi-simple.

Supposons maintenant que $A_2$ soit absolument semi-simple. Soit L une extension de K. Alors l’algèbre $A_{1(L)}$ est absolument semi-simple et l’algèbre $A_{2(L)}$ est semi-simple. Donc, par a), l’algèbre $A_1\otimes_KA_{2(L)}$ est semi-simple.

#### Corollaire 2 {#alg-viii-s13-lem-4-cor-2 .statement tag=00FL}

Soit K un corps séparablement clos et soit A une K-algèbre absolument semi-simple. Il existe alors un entier $r\geqslant 0$et des entiers strictement positifs $n_1, . . . , n_r$ tels que l’algèbre A soit isomorphe à l’algèbre $\prod^r_{i=1}\mathbf{M}_{n_i}(K)$.

D’après le th. 1, A est isomorphe à une algèbre de la forme $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$, pour un entier $r\geqslant 0$, des entiers $n_1, . . . , n_r$ et des K-algèbres de degré fini $D_1, . . . ,D_r$ qui sont des corps et dont les centres sont des extensions séparables de K et donc égales à K. Par la prop. 3 de VIII, p. 227, on a $D_i= K$ pour $i\in [1, r]$.

#### Exemple {#alg-viii-s13-n3-exa-1 .statement tag=00FM}

Pour qu’une K-algèbre commutative soit absolument semi-simple, il faut et il suffit qu’elle soit étale (V, p. 28, déf. 1) : cela résulte de la définition et de l’équivalence des conditions (i) et (v) du th. 1.

### 4. Caractérisation des modules absolument semi-simples

#### Proposition 4 {#alg-viii-s13-prop-4 .statement tag=00FN}

Soient K un corps commutatif et A une K-algèbre.

a) Soit M un A-module semi-simple. Pour que le A-module M soit absolument semi-simple, il faut et il suffit que tout module simple appartenant au support de M le soit.

b) Soit S un A-module simple et soit D son commutant. Les conditions suivantes sont équivalentes :

(i) Le A-module S est absolument semi-simple ;

(ii) La K-algèbre D est absolument semi-simple ;

(iii) La K-algèbre D est un corps, de degré fini sur K et son centre est une

extension séparable de K.

L’assertion a) résulte de la prop. 1, a) de VIII, p. 225. Plaçons-nous sous les hypothèses de b) ; soit L une extension de K. Pour que le $A_{(L)}$-module $S_{(L)}$ soit semi-simple, il faut et il suffit que l’anneau $D_{(L)}$ soit semi-simple (VIII, p. 217, prop. 8, c)). Cela prouve l’équivalence de (i) et (ii), et celle de (ii) et (iii) résulte du théorème 1 puisque D est un corps.

#### Corollaire {#alg-viii-s13-n4-cor-1 .statement tag=00RF}

Soient K un corps commutatif, $A_1$ et $A_2$ des K-algèbres, $M_1$ un $A_1$-module absolument semi-simple, $M_2$ un $A_2$-module semi-simple. Alors $M_1\otimes_KM_2$ est un module semi-simple sur l’anneau $A_1\otimes_KA_2$.

Le module $M_1$ est somme directe de $A_1$-modules simples absolument semi-simples (prop. 4). Il suffit donc de démontrer la proposition dans le cas où les modules $M_1$ et $M_2$ sont simples. Notons $D_1$ et $D_2$ leurs commutants. La K-algèbre $D_1$ est absolument semi-simple (loc. cit.) ; d’après le cor. 1 de VIII, p. 230, la K-algèbre $D_1\otimes_KD_2$ est semi-simple. Il résulte alors du cor. 1 de VIII, p. 211, que le $(A_1\otimes_KA_2)$-module $M_1\otimes_KM_2$ est semi-simple.

### 5. Dérivations des algèbres semi-simples

Dans ce numéro et les suivants, on note K un anneau commutatif, A une K-algèbre, B la K-algèbre $A\otimes_KA^o$ et $\varepsilon$ l’application K-linéaire de B dans A telle que l’on ait $\varepsilon (x\otimes y) =xy$ pour $x, y$ dans A.

Rappelons (III, p. 39) que tout $(A$, A)-bimodule P peut être considéré comme un B-module à gauche, dont la loi d’action est caractérisée par $(a\otimes a')p=apa'$ pour $a, a'$ dans A et $p$ dans P ; réciproquement, tout B-module peut être considéré comme un $(A$, A)-bimodule. On munit A de sa structure canonique de $(A$, A)-bimodule et de la structure de B-module correspondante ; on munit B de la structure de $(A,A)$-bimodule correspondant au B-module $B_s$. On a donc

$$
a(x\otimes y)a'= (a\otimes a')(x\otimes y) =ax\otimes ya'
$$

pour $a, a', x, y$ dans A, le produit $ya'$ étant calculé dans l’algèbre A.

L’application K-linéaire $\varepsilon$ est un homomorphisme de $(A$, A)-bimodules.

#### Proposition 5 {#alg-viii-s13-prop-5 .statement tag=00FO}

Les propriétés suivantes sont équivalentes :

(i) Le B-module A est projectif ;

(ii) Il existe un élément $e$ du $(A,A)$-bimodule B satisfaisant aux deux conditions suivantes $:\varepsilon (e) = 1$et $ae=ea$ pour tout $a\in A$.

L’application $\varepsilon : B\rightarrow A$ est surjective car on a $\varepsilon (a\otimes 1) =a$ pour tout $a\in A$; c’est un homomorphisme de $(A$, A)-bimodules, donc une application B-linéaire. Si le B-module A est projectif, il existe une section $s$ de $\varepsilon$ (II, p. 39, prop. 4) ; c’est un homomorphisme de $(A$, A)-bimodules de A dans B. Si l’on pose $e=s$(1), on a $\varepsilon (e) =\varepsilon (s(1)) = 1$ et $ae=s(a) =ea$ pour tout $a\in A$. Donc (i) implique (ii).

Inversement, soit $e$ un élément de B satisfaisant aux conditions de (ii). Définissons une application $s$ de A dans B par la formule

$$
s(a) =ae=ea \tag{1}
$$

C’est un homomorphisme de $(A$, A)-bimodules et l’on a $\varepsilon \circ s= 1_A$; autrement dit, $s$ est une section B-linéaire de l’application surjective $\varepsilon$. Par suite le B-module A est isomorphe au sous-module facteur direct $s(A)$ de $B_s$ (II, p. 20, prop. 15), donc est projectif (II, p. 39, prop. 4). Cela prouve que (ii) entraîne (i).

#### Remarque 1 {#alg-viii-s13-n5-rem-1 .statement tag=00FP}

Soit $e=\sum^r_{i=1}a_i\otimes a'_i$ un élément de B. Les conditions (ii) de la prop. 5 se traduisent par les formules

$$
\sum_{i=1}^ra_ia'_i= 1 \tag{2}
$$

(3) $\sum_{i=1}^raa_i\otimes a'_i=\sum_{i=1}^ra_i\otimes a'_ia$ pour tout $a\in A$.

Lorsqu’elles sont satisfaites, $e$ est un élément idempotent de B. En effet, on a alors les relations :

$$
e^2=\sum_{i=1}^ra_iea'_i=\sum_{i=1}^rea_ia'_i=e
$$

#### Remarque 2 {#alg-viii-s13-n5-rem-2 .statement tag=00FQ}

Soit K un anneau commutatif, soit A une K-algèbre et soit M un A-module. Le groupe End$_K(M)$ est muni d’une structure de $(A$, A)-bimodule définie par

$$
aua'(x) =au(a'x)
$$

pour tous $a, a'\in A$, tout $u\in$ End$_K(M)$ et tout $x\in M$. Munissons-la de la structure de B-module associée. Soit $e=\sum^r_{i=1}a_i\otimes a'_i$ un élément de B satisfaisant aux conditions (ii) de la prop. 5, donc aussi aux relations (2) et (3). Si $p\in$ End$_K(M)$ est un projecteur dont l’image N est un sous-A-module de M, alors $ep$ est un projecteur A-linéaire de même image.

En effet l’image de $ep$ est contenu dans N. Si $x$ appartient à N, il en est de même de $a'_ix$, d’où $p(a'_ix) =a'_ix$, et

$$
ep(x) =\sum_{i=1}^ra_ia'_ix=x
$$

d’après la formule (2). De la formule (3), on déduit que $aep(x) =ep(ax)$ pour tout $a\in A$ et tout $x\in M$, ce qui démontre que $ep$ est A-linéaire.

#### Théorème 2 {#alg-viii-s13-thm-2 .statement tag=00RG}

Soient K un corps commutatif, A une K-algèbre. Les propriétés suivantes sont équivalentes :

(i) La K-algèbre A est absolument semi-simple ;

(ii) La K-algèbre $B = A\otimes_KA^o$ est semi-simple ;

(iii) Le B-module A est projectif ;

(iv) Il existe un élément $e$ du $(A,A)$-bimodule B satisfaisant à $\varepsilon (e) = 1$et $ae=ea$ pour tout $a\in A$.

Supposons l’algèbre A absolument semi-simple, donc semi-simple. Alors l’algèbre $A^o$ est semi-simple (VIII, p. 133, prop. 2) et il résulte du cor. 1 de VIII, p. 230 que $B = A\otimes_KA^o$ est une K-algèbre semi-simple. Donc (i) entraîne (ii).

Comme tout module sur un anneau semi-simple est projectif (VIII, p. 134, prop. 4), (ii) entraîne (iii).

L’équivalence de (iii) et (iv) résulte de la prop. 5. Pour achever la démonstration, prouvons que (iv) implique (i). Soit $e=\sum^r_{i=1}a_i\otimes a'_i$ un élément de B satisfaisant aux conditions (ii) de la prop. 5. Soit L une extension du corps K ; il s’agit de prouver que l’anneau $A_{(L)}$ est semi-simple ou encore que tout $A_{(L)}$-module est semi-simple (VIII, p. 134, prop. 4). Soit M un $A_{(L)}$-module et soit N un sous-module de M ; considérons M comme un $(A$, L)-bimodule à gauche et N comme un sousbimodule (III, p. 39). Comme L est un corps, il existe un projecteur L-linéaire $u$ dans M, d’image N. Comme les homothéties $a_M$ associées aux éléments $a$ de A sont L-linéaires, il existe un unique homomorphisme de groupes de $A\otimes_KA^o$ dans End$_L(M)$ qui associe à un élément $a\otimes a'$ l’application L-linéaire $x\rightarrow au(a'x)$. Notons $v$ l’image de $e$ par cet homomorphisme ; il résulte de la remarque 2 que $v$ est un projecteur $A_{(L)}$-linéaire d’image N. Le noyau de $v$ est un sous-A$_{(L)}$-module de M, supplémentaire de N. D’après le cor. 2 de VIII, p. 52, le $A_{(L)}$-module M est semi-simple.

#### Remarque 3 {#alg-viii-s13-n5-rem-3 .statement tag=00FR}

On sait (VIII, p. 230, cor. 1) que le produit tensoriel de deux algèbres absolument semi-simples sur un corps commutatif est absolument semi-simple. Par suite, si l’algèbre A est absolument semi-simple, il en est de même de l’algèbre $B = A\otimes_KA^o$.

### 6. Cohomologie des algèbres

Dans ce numéro, on note K un anneau commutatif, A une K-algèbre, B la K-algèbre $A\otimes_KA^o$ et $\varepsilon$ l’application K-linéaire de B dans A telle que l’on ait $\varepsilon (x\otimes y) =$ $xy$ pour $x, y$ dans A. Pour $n\in \mathbf{N}$, on note $B_n$ le produit tensoriel sur K de $(n+ 2)$ copies du K-module A. On le considère comme un $(A$, A)-bimodule (et aussi comme B-module) en le munissant de la structure de A-module à gauche déduite de la structure de A-module à gauche du premier facteur du produit tensoriel, et de la structure de A-module à droite déduite de la structure de A-module à droite du dernier facteur. En particulier, $B_0$ n’est autre que le $(A$, A)-bimodule B.

Pour tout entier $n\geqslant 1$, on définit des homomorphismes de bimodules $d_n^i$ pour $i\in [0, n]$ et $d_n$ de $B_n$ dans $B_{n-1}$, par les formules

$$
d_n^i(x_0\otimes  \cdots  \otimes x_{n+1}) =x_0\otimes  \cdots  \otimes x_ix_{i+1}\otimes  \cdots  \otimes x_{n+1} \tag{4}
$$

pour $i\in [0, n]$.

$$
d_n=\sum_{i=0}^n(-1)^id_n^i \tag{5}
$$

On note $d_0=d^0_0$ l’application $\varepsilon : B_0\rightarrow A$.

Soit $n$ un entier $\geqslant 1$. Pour $0 \leqslant i < j \leqslant n$, on a

$$
d_{n-1}^i \circ d_n^j = d_{n-1}^{j-1} \circ d_n^i
$$

et l’on en déduit

$$
\begin{align*}
d_{n-1} \circ d_n &= \sum_{0 \leqslant i < j \leqslant n} (-1)^{i+j} d_{n-1}^i \circ d_n^j + \sum_{0 \leqslant j \leqslant i \leqslant n-1} (-1)^{i+j} d_{n-1}^i \circ d_n^j \\
&= \sum_{0 \leqslant i < j \leqslant n} (-1)^{i+j} d_{n-1}^{j-1} \circ d_n^i + \sum_{0 \leqslant j \leqslant i \leqslant n-1} (-1)^{i+j} d_{n-1}^i \circ d_n^j,
\end{align*}
$$

d’où

$$
d_{n-1} \circ d_n = 0.
$$

Soit $P$ un $(A, A)$-bimodule. Pour tout entier $n \geqslant 0$, on note $C^n(A, P)$ le K-module des applications K-multilinéaires de $A^n$ dans $P$. L’application $\alpha^n : C^n(A, P) \to \operatorname{Hom}_B(B_n, P)$ qui à $f \in C^n(A, P)$ associe l’homomorphisme $\alpha^n(f)$ caractérisé par

$$
\alpha^n(f)(x_0 \otimes \cdots \otimes x_{n+1}) = x_0 f(x_1, \ldots, x_n)x_{n+1}
$$

est un isomorphisme de K-modules.

On note $\partial^n$ (pour $n \geqslant 0$) l’unique application K-linéaire de $C^n(A, P)$ dans $C^{n+1}(A, P)$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
C^n(A, P) & \xrightarrow{\partial^n} & C^{n+1}(A, P) \\
\downarrow \alpha^n & & \downarrow \alpha^{n+1} \\
\operatorname{Hom}_B(B_n, P) & \xrightarrow{\operatorname{Hom}(d_{n+1}, 1_P)} & \operatorname{Hom}_B(B_{n+1}, P);
\end{array}
$$

on a donc par définition

$$
(\alpha^{n+1} \circ \partial^n)(f) = \alpha^n(f) \circ d_{n+1}
$$

pour tout $f \in C^n(A, P)$. Autrement dit, on a

$$
\partial^n(f)(x_0, \ldots, x_n) = \alpha^n(f)(d_{n+1}(1 \otimes x_0 \otimes \cdots \otimes x_n \otimes 1))
$$

pour $x_0, \ldots, x_n$ dans $A$ et $f$ dans $C^n(A, P)$, c’est-à-dire

$$
\begin{align*}
\partial^n(f)(x_0, \ldots, x_n) = & x_0 f(x_1, \ldots, x_n) \\
& + \sum_{i=0}^{n-1} (-1)^{i+1} f(x_0, \ldots, x_{i-1}, x_i x_{i+1}, x_{i+2}, \ldots, x_n) \\
& + (-1)^{n+1} f(x_0, \ldots, x_{n-1}) x_n.
\end{align*}
$$

D’après (7) et (9), on a

(11) $\partial^{n+1}\circ \partial^n= 0$ pour tout $n\geqslant 0$.

On note $H^0(A,P)$ le K-module Ker $\partial^0$ et, pour $n\geqslant 1, H^n(A,P)$ le K-module Ker $\partial^n/$ Im $\partial^{n-1}$. Le K-module $C^0(A,P)$ s’identifie à P et on a $C^1(A,P) =$ Hom$_K(A,P)$. Les applications $\partial^n$ pour $n\leqslant 2$ sont données par les formules

(12) $\partial^0(p)(a) =ap-pa$ pour tout $p\in P$;

(13) $\partial^1(f)(a, a') =af(a')-f(aa') +f(a)a'$ pour $f\in C^1(A,P)$;

$$
\partial^2(f)(a, a', a'') =af(a', a'')-f(aa', a'') +f(a, a'a'')-f(a, a')a'' \tag{14}
$$

pour $f\in C^2(A,P)$.

Ainsi $H^0(A,P)$ est le sous-K-module de P formé des éléments $p$ tels que $ap=$ $pa$ pour tout $a\in A$, et $H^1(A,P)$ est le quotient du K-module Der$_K(A,P)$ des K-dérivations de A dans P (III, p. 118) par le sous-K-module formé des dérivations de la forme $a\rightarrow ap-pa$ avec $p\in P$ (appelées dérivations intérieures).

### 7. Cohomologie des algèbres absolument semi-simples

#### Proposition 6 {#alg-viii-s13-prop-6 .statement tag=00FS}

Soient K un anneau commutatif et A une K-algèbre. Soit $e=$ $\sum^r_{i=1}a_i\otimes a'_i$ un élément de $B = A\otimes_KA^o$ vérifiant les conditions (ii) de la prop. 5 de VIII, p. 232. Pour tout entier $n\geqslant 1$et tout élément $f$ de $C^n(A,P)$, notons $\gamma^n(f)$ l’élément de $C^{n-1}(A,P)$défini par la formule

$$
\gamma^n(f)(x_1, . . . , x_{n-1}) =\sum_{i=1}^ra_if(a'_i, x_1. . . , x_{n-1}) \tag{15}
$$

On a alors

$$
\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =f \tag{16}
$$

pour tout entier $n\geqslant 1$et tout $f\in C^n(A,P)$.

#### Remarque 1 {#alg-viii-s13-n7-rem-1 .statement tag=00SF}

$*$Les morphismes $\partial_n: C^n(A,P)\rightarrow C^{n+1}(A,P)$ définissent

un complexe $(C(A,P), \partial )$ de K-modules (X, p. 24). L’application $\gamma_n$ définit donc une homotopie reliant 0 à Id$_{C(A,P)}$ de ce complexe dans lui-même (X, p. 32, déf. $4$)$.*$

Reprenons les notations du n$^o6$. Définissons, pour tout entier $n\geqslant 0$, une application $h_n: B_n\rightarrow B_{n+1}$ par la formule

$$
h_n(x) =d^1_{n+2}(e\otimes x) =\sum_{i=1}^ra_i\otimes a'_ix
$$

C’est un homomorphisme de $(A$, A)-bimodules (formule (3)).

#### Lemme 5 {#alg-viii-s13-lem-5 .statement tag=00FT}

On a la relation

$$
d_{n+1}\circ h_n+h_{n-1}\circ d_n= 1_{B_n} \tag{17}
$$

pour tout $n\geqslant 1$.

Soit $x\in B_n$; on a

$$
(d_{n+1}\circ h_n)(x) = (d_{n+1}\circ d^1_{n+2})(e\otimes x)
$$

$$
= (d^0_{n+1}\circ d^1_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d_{n+1}^{i-1}\circ d^1_{n+2})(e\otimes x)
$$

d’où, par la formule (6),

$$
(d_{n+1}\circ h_n)(x) = (d^0_{n+1}\circ d^0_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d^1_{n+1}\circ d_{n+2}^i)(e\otimes x)
$$

Mais on a

$$
(d^0_{n+1}\circ d^0_{n+2})(e\otimes x) =\varepsilon (e)x=x
$$

par la condition (ii) de la prop. 5 de VIII, p. 232 et, pour $i\geqslant 2$,

$$
d^i_{n+2}(e\otimes x) =e\otimes d^{i-2}_n(x)
$$

ce qui donne

$$
(d_{n+1}\circ h_n)(x) =x-d^1_{n+1}(e\otimes d_n(x)) =x-h_{n-1}\circ d_n(x)
$$

d’où la formule (17).

Avec le lemme 5, nous pouvons terminer la preuve de la proposition 6. Soient $n$ un entier $\geqslant 1$ et $f$ un élément de $C^n(A,P)$. On a par construction

$$
\alpha^{n-1}(\gamma^n(f)) =\alpha^n(f)\circ h_{n-1} \tag{18}
$$

et par suite, d’après les formules (9) et (18)

$$
\alpha^n(\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =\alpha^{n-1}(\gamma^n(f))\circ d_n+\alpha^{n+1}(\partial^n(f))\circ h_n
$$

$$
=\alpha^n(f)\circ h_{n-1}\circ d_n+\alpha^n(f)\circ d_{n+1}\circ h_n
$$

$$
=\alpha^n(f)
$$

où la dernière égalité résulte de (17). Comme $\alpha^n$ est bijective, la proposition en résulte.

#### Théorème 3 {#alg-viii-s13-thm-3 .statement tag=00FU}

Soient K un anneau commutatif, A une K-algèbre et P un $(A,A)$-bimodule. On suppose que le $(A\otimes_KA^o)$-module A est projectif. On a alors $H^n(A,P) = 0$pour tout entier $n\geqslant 1$.

Il s’agit de prouver que pour tout entier $n\geqslant 1$, tout élément $f$ de $C^n(A,P)$ tel que $\partial^n(f) = 0$ est de la forme $\partial^{n-1}(g)$ pour un élément $g$ de $C^{n-1}(A,P)$. Compte tenu de la prop. 5 (VIII, p. 232), c’est une conséquence immédiate de la prop. 6 de VIII, p. 236.

#### Corollaire {#alg-viii-s13-n7-cor-1 .statement tag=00FV}

Toute K-dérivation de A dans P est intérieure.

C’est une traduction de l’égalité $H^1(A,P) = 0$.

#### Remarque 2 {#alg-viii-s13-n7-rem-2 .statement tag=00FW}

Les hypothèses du th. 3 sont notamment vérifiées lorsque K est un corps et A une K-algèbre absolument semi-simple (VIII, p. 233, th. 2).

#### Remarque 3 {#alg-viii-s13-n7-rem-3 .statement tag=00FX}

Supposons que le K-module A soit projectif. Le théorème 3 peut aussi se

démontrer de la façon suivante. Le complexe $(\bigoplus_{n\geqslant 0}B_n, d)$ et l’homomorphisme $\varepsilon : B_0\rightarrow A$ définissent une résolution projective du B-module A ; le K-module $H^n(A,P)$ est donc isomorphe à Ext$^n_B(A,P)$ pour tout $n\geqslant 0$ (X, p. 100, th. 1). Si le B-module A est projectif, les K-modules Ext$^n_B(A,P)$ sont nuls pour $n\geqslant 1$ (X, p. 88, cor. de la prop. 5), ce qui entraîne la nullité de $H^n(A,P)$. Inversement, si $H^1(A,P)$ est nul pour tout $(A$, A)-bimodule P, le B-module A est projectif (X, p. 93, prop. $10$)$.*$

### 8. Scindage des algèbres artiniennes

Dans ce numéro, K désigne un anneau commutatif et A une K-algèbre. Soit $\mathfrak{r}$ le radical de A. Notons $\overline{A}$ l’algèbre quotient $A/\mathfrak{r}$ et $\pi$ l’application canonique de A sur A. On s’intéresse ici aux sous-algèbres S de A telles que $A = S\oplus \mathfrak{r}$.

Notons Σ l’ensemble des sections K-linéaires $s$ de $\pi$ satisfaisant à $s(\alpha \beta ) =$ $s(\alpha )s(\beta )$ pour $\alpha , \beta$ dans A. Observons qu’une telle section satisfait nécessairement à $s(1) = 1$ (autrement dit, $s$ est un homomorphisme d’anneaux) : on a en effet $s(1)^2=s$(1), et $s(1)$ est inversible puisqu’il appartient à $1 +\mathfrak{r}$ (VIII, p. 151, th. 1). Si $s$ est un élément de Σ, l’image S de $s$ est une sous-algèbre de A et l’on a $A = S\oplus \mathfrak{r}$. Inversement, si S est une sous-algèbre de A telle que $A = S\oplus \mathfrak{r}$, la restriction de $\pi$ à S est bijective, et la bijection réciproque définit un élément de Σ d’image S.

D’après le théorème de Jacobson (loc. cit.), tout élément de $1 +\mathfrak{r}$ est inversible dans A ; on appelle automorphisme spécial de A tout automorphisme intérieur de la forme $a\rightarrow xax^{-1}$ avec $x\in 1 +\mathfrak{r}$.

#### Proposition 7 {#alg-viii-s13-prop-7 .statement tag=00FY}

Supposons que le $(A\otimes_K\overline{A^o})$-module A soit projectif.

a) Soient $S_1$ et $S_2$ des sous-algèbres de A satisfaisant à $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. Il existe un automorphisme spécial de A transformant $S_1$ en $S_2$.

b) Supposons que $\pi$ possède une section K-linéaire et que le radical $\mathfrak{r}$ de A soit nilpotent. Il existe alors une sous-algèbre S de A satisfaisant à $A = S\oplus \mathfrak{r}$.

Plaçons-nous sous les hypothèses de a) et notons $s_1$ et $s_2$ les éléments de l’ensemble Σ correspondant aux sous-algèbres $S_1$ et $S_2$. Soit $\varepsilon$ l’application K-linéaire de $A\otimes_KA$ dans A telle que $\varepsilon (a\otimes b) =ab$. D’après la prop. 5 de VIII, p. 232, et la remarque 1 de VIII, p. 232, il existe un élément $e=\sum^r_{i=1}\alpha_i\otimes \alpha '_i$ de $\overline{A}\otimes_K\overline{A}$ satisfaisant à $\sum^r_{i=1}\alpha_i\alpha '_i= 1$ et $\sum^r_{i=1}\alpha \alpha_i\otimes \alpha '_i=\sum^r_{i=1}\alpha_i\otimes \alpha '_i\alpha$ pour tout $\alpha \in A$. Posons $x=\sum^r_{i=1}s_1(\alpha_i)s_2(\alpha '_i)$. On a $\pi (x) =\sum^r_{i=1}\alpha_i\alpha '_i= 1$, d’où $x\in 1 +\mathfrak{r}$. Soit $\alpha$ un élément de A. On a

$$
s_1(\alpha )x=\sum_{i=1}^rs_1(\alpha \alpha_i)s_2(\alpha '_i) = (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha \alpha_i\otimes \alpha '_i)
$$

$$
= (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha_i\otimes \alpha '_i\alpha )=\sum_{i=1}^rs_1(\alpha_i)s_2(\alpha '_i\alpha ) =xs_2(\alpha )
$$

L’égalité $x^{-1}S_1x= S_2$ en résulte, d’où l’assertion a).

Prouvons l’assertion b) sous l’hypothèse $\mathfrak{r}^2= 0$. En ce cas, le $(A$, A)-bimodule $\mathfrak{r}$ est annulé par $\mathfrak{r}$ et on le considère donc comme un $(A$, A)-bimodule. Choisissons une section K-linéaire $\sigma$ de $\pi$. On a

(19) $\alpha x=\sigma (\alpha )x$ et $x\alpha =x\sigma (\alpha )$

pour $\alpha \in \overline{A}$ et $x\in \mathfrak{r}$. Posons

$$
\varphi (\alpha , \beta ) =\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ) \tag{20}
$$

pour $\alpha , \beta \in A$. On a la relation $\pi (\varphi (\alpha , \beta )) =\alpha \beta -\alpha \beta = 0$ pour $\alpha , \beta \in A$. Donc $\varphi$ défini un élément de $C^2(A,\mathfrak{r})$. Soient $\alpha , \beta , \gamma$ des éléments de $\overline{A}$; compte tenu de(19), on a

$$
\partial^2\varphi (\alpha , \beta , \gamma ) =\alpha \varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\gamma
$$

$$
=\sigma (\alpha )\varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\sigma (\gamma )
$$

$$
=\sigma (\alpha )(\sigma (\beta \gamma )-\sigma (\beta )\sigma (\gamma ))-\sigma (\alpha \beta \gamma ) +\sigma (\alpha \beta )\sigma (\gamma ) +\sigma (\alpha \beta \gamma )
$$

$$
-\sigma (\alpha )\sigma (\beta \gamma )-(\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ))\sigma (\gamma )
$$

$$
= 0
$$

D’après le th. 3 de VIII, p. 238, le K-module $H^2(A,\mathfrak{r})$ est réduit à zéro. Il existe donc un élément $\psi$ de $C^1(A,\mathfrak{r})$ tel que $\partial^1\psi =\varphi$, c’est-à-dire tel qu’on ait

(21) $\varphi (\alpha , \beta ) =\alpha \psi (\beta )-\psi (\alpha \beta ) +\psi (\alpha )\beta$ pour $\alpha , \beta$ dans A.

On a $\psi (\alpha )\psi (\beta ) = 0$ puisque $\mathfrak{r}^2$ est nul ; on tire alors de (19) et (20)

$$
(\sigma +\psi )(\alpha \beta ) = (\sigma +\psi )(\alpha )(\sigma +\psi )(\beta ) \tag{22}
$$

de sorte que la section K-linéaire $\sigma +\psi$ de $\pi$ appartient à Σ. Son image est une sous-algèbre S de A telle que $A = S +\mathfrak{r}$.

Démontrons enfin l’existence de S dans le cas général. Raisonnons par récurrence sur le plus petit entier $p\geqslant 1$ tel que $\mathfrak{r}^p= 0$, le cas $p= 1$ étant trivial. Supposons qu’on ait $p\geqslant 2$, et posons $A'= A/\mathfrak{r}^{p-1}$; le radical $\mathfrak{r}'$ de $A'$ est égal à $\mathfrak{r}/\mathfrak{r}^{p-1}$ (prop. 5 de VIII, p. 150), donc satisfait à ${\mathfrak{r}'}^{p-1}= 0$, et l’algèbre $A'/\mathfrak{r}'$ est isomorphe à $\overline{A}= A/\mathfrak{r}$, donc est absolument semi-simple. D’après l’hypothèse de récurrence, il existe une sous-algèbre $S'$ de $A'$ telle que $A'= S'\oplus \mathfrak{r}'$. Alors $S'$ est de la forme $A''/\mathfrak{r}^{p-1}$, où $A''$ est une sous-algèbre de A contenant $\mathfrak{r}^{p-1}$, et l’on a

$$
A = A''+\mathfrak{r},\mathfrak{r}^{p-1}= A''\cap \mathfrak{r} \tag{23}
$$

L’algèbre $A''/\mathfrak{r}^{p-1}$ est isomorphe à $A'/\mathfrak{r}'$; on a $(\mathfrak{r}^{p-1})^2= 0$ donc $\mathfrak{r}^{p-1}$ est le radical de $A''$. D’après le cas traité précédemment, il existe une sous-algèbre S de $A''$ telle que $A''= S\oplus \mathfrak{r}^{p-1}$; on déduit de (23) la relation $A = S\oplus \mathfrak{r}$.

#### Corollaire 1 (théorème de Wedderburn) {#alg-viii-s13-prop-7-cor-1 .statement tag=00S8}

Soient K un corps commutatif, A une K-algèbre, $\mathfrak{r}$ le radical de A. On suppose que la K-algèbre $A/\mathfrak{r}$ est absolument semi-simple.

a) Soient $S_1$ et $S_2$ des sous-algèbres de A satisfaisant à $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. Il existe un automorphisme spécial de A transformant $S_1$ en $S_2$.

b) Si $\mathfrak{r}$ est nilpotent, il existe une sous-algèbre S de A satisfaisant à $A = S\oplus \mathfrak{r}$.

Cela résulte de la prop. 7 et du th. 2 de VIII, p. 233.

#### Corollaire 2 {#alg-viii-s13-prop-7-cor-2 .statement tag=00FZ}

Soit A une algèbre commutative de degré fini sur un corps parfait K et soit $\mathfrak{r}$ son radical. Il existe une unique sous-algèbre S de A telle que $A = S\oplus \mathfrak{r}$. De plus, S est isomorphe au produit d’un nombre fini d’extensions de degré fini de K.

La K-algèbre $A/\mathfrak{r}$ est semi-simple (VIII, p. 169, prop. 1) et de degré fini ; le corps K étant parfait, elle est absolument semi-simple (VIII, p. 228, th. 1). Comme l’idéal $\mathfrak{r}$ est nilpotent, l’existence et l’unicité de S résultent alors du cor. 1. Comme S est semi-simple, commutative et de degré fini, la dernière assertion est une conséquence de la prop. 3 de VIII, p. 133.

#### Remarque 1 {#alg-viii-s13-n8-rem-1 .statement tag=00G0}

L’hypothèse que $A/\mathfrak{r}$ est absolument semi-simple est essentielle dans le cor. 1 (VIII, p. 242, exerc. 4).

#### Remarque 2 {#alg-viii-s13-n8-rem-2 .statement tag=00G1}

Supposons que A soit une algèbre artinienne sur le corps K. Si A est commutative, on peut montrer (VIII, p. 176, exerc. 9) que A est isomorphe à un produit d’algèbres $A_1\times  \cdots  \times A_n$ telles que $A_i/\mathfrak{R}(A_i)$ soit un corps pour tout $i$. Par contre, si A n’est pas commutative, il se peut que A ne soit pas isomorphe à un produit d’algèbres $A_1\times  \cdots  \times A_n$ telles que $A_i/\mathfrak{R}(A_i)$ soit un anneau simple pour tout $i$ (VIII, p. 243, exerc. 5).

## EXERCICES {#alg-viii-s13-exercises}

See the [exercises for § 13](exercises/s13/).
