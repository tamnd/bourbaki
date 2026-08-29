---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 15
section_title: EXTENSIONS SÉPARABLES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.165-A V.166
pdf_pages: 0217-0225, 0269-0270
extraction: ocr
subsections:
    - "no": 1
      title: Caractérisation des éléments nilpotents d’un anneau
      page: 0
      pdf_page: 217
    - "no": 2
      title: Algèbres séparables
      page: 114
      pdf_page: 218
    - "no": 3
      title: Extensions séparables
      page: 116
      pdf_page: 220
    - "no": 4
      title: Critère de séparabilité de MacLane
      page: 0
      pdf_page: 221
    - "no": 5
      title: Extensions d’un corps parfait
      page: 0
      pdf_page: 223
    - "no": 6
      title: Caractérisation de la séparabilité par les automorphismes
      page: 120
      pdf_page: 224
statements: 24
exercises: 12
content_sha256: b215ae22ba213fd12c6db1406b74f563872be7ba482443fb12ad1f2ce85292ad
---

## § 15. EXTENSIONS SÉPARABLES

### 1. Caractérisation des éléments nilpotents d’un anneau

#### Proposition 1 {#alg-v-s15-prop-1 .statement}

Soient A un anneau commutatif et x un élément de A. Pour que x soit nilpotent, il faut et il suffit que le polynôme $1 - xT$ soit inversible dans l’anneau A[T].

Notons que A[T] est un sous-anneau de l’anneau de séries formelles A[[T]], et que $1 - xT$ admet dans A[[T]] l’inverse $\sum_{n=0}^{\infty} x^n T^n$ (IV, p. 28, prop. 5). Pour que $1 - xT$ soit inversible dans A[T], il faut et il suffit que $\sum_{n=0}^{\infty} x^n T^n$ soit un polynôme, c’est-à-dire que x soit nilpotent.

#### Proposition 2 {#alg-v-s15-prop-2 .statement}

Soit A un anneau commutatif. L’ensemble des éléments nilpotents de A est un idéal de A égal à l’intersection de l’ensemble des idéaux premiers de A.

Soient x un élément nilpotent de A et p un idéal premier de A. La classe de x modulo p est un élément nilpotent de l’anneau intègre A/p, donc est nulle ; on a donc $x \in p$.

Soit x un élément non nilpotent de A. D’après la prop. 1, l’idéal principal $(1 - xT)$ de A[T] est distinct de A[T]. D’après le th. de Krull (I, p. 99), il existe un idéal maximal m de A[T] contenant $1 - xT$. Alors m est un idéal premier de A[T], donc $p = A \cap m$ est un idéal premier de A. On a $1 \notin m$ et $1 - xT \in m$, d’où $xT \notin m$ et $a \text{ fortiori } x \notin p$.

On a donc prouvé que l’ensemble $n$ des éléments nilpotents de $A$ est l’intersection de l’ensemble des idéaux premiers de $A$; comme toute intersection d’idéaux est un idéal, $n$ est un idéal.

#### Corollaire {#alg-v-s15-n1-cor-1 .statement}

*Pour qu’un anneau commutatif soit réduit* (V, p. 33, déf. 2), *il faut et il suffit qu’il soit isomorphe à un sous-anneau d’un produit de corps*.

La condition est évidemment suffisante.

Soit $A$ un anneau réduit. D’après la prop. 2, l’intersection $n$ de l’ensemble des idéaux premiers de $A$ est réduite à 0. Pour tout idéal premier $p$ de $A$, soient $k(p)$ le corps des fractions de $A/p$ et $\varphi_p$ l’homomorphisme canonique de $A$ dans $k(p)$. Soit $\varphi$ l’homomorphisme de $A$ dans $\prod_p k(p)$ dont la composante d’indice $p$ est $\varphi_p$. Le noyau de $\varphi_p$ est $p$, donc celui de $\varphi$ est $n = 0$; par suite $\varphi$ est un isomorphisme de $A$ sur un sous-anneau de $\prod_p k(p)$.

### 2. Algèbres séparables

#### Définition 1 {#alg-v-s15-def-1 .statement}

*Soit $A$ une algèbre commutative sur un corps $K$. On dit que $A$ est séparable sur $K$, ou que c’est une $K$-algèbre séparable, si l’anneau $L \otimes_K A$ est réduit pour toute extension $L$ de $K$*.

Toute algèbre séparable est évidemment réduite. Pour une réciproque partielle, cf. th. 3 (V, p. 119).

#### Exemple 1 {#alg-v-s15-n2-exa-1 .statement}

Soit $A$ une algèbre de polynômes $K[X_i]_{i \in I}$. Pour toute extension $L$ de $K$, l’anneau $L \otimes_K A$ est isomorphe à $L[X_i]_{i \in I}$ (III, p. 22, remarque 2), donc est intègre (IV, p. 9, prop. 8). Autrement dit, toute algèbre de polynômes sur un corps $K$ est une $K$-algèbre séparable.

#### Exemple 2 {#alg-v-s15-n2-exa-2 .statement}

Soit $A$ une algèbre commutative de degré fini sur un corps $K$. Pour que $A$ soit séparable, il faut et il suffit qu’elle soit étale (V, p. 34, th. 4).

#### Exemple 3 {#alg-v-s15-n2-exa-3 .statement}

Soit $E$ une extension algébrique d’un corps $K$. Si $L$ est une extension de $K$, l’anneau $L \otimes_K E$ est réunion des sous-anneaux $L \otimes_K F$ où $F$ parcourt l’ensemble des sous-extensions de degré fini de $E$; par suite, l’anneau $L \otimes_K E$ est réduit si et seulement s’il en est ainsi de $L \otimes_K F$ pour toute sous-extension $F$ de $E$, de degré fini sur $K$. Compte tenu de l’exemple 2, on voit que $E$ est une algèbre séparable au sens de la déf. 1 ci-dessus, si et seulement si c’est une extension algébrique séparable au sens de la déf. 1 de V, p. 35.

#### Proposition 3 {#alg-v-s15-prop-3 .statement}

*Soit $K$ un corps*.

a) *Toute sous-algèbre d’une $K$-algèbre séparable est séparable*.

b) *Toute limite inductive de $K$-algèbres séparables est séparable*.

c) *Tout produit de $K$-algèbres séparables est séparable*.

d) *Soit $A$ une $K$-algèbre et soit $K'$ une extension de $K$. Pour que $A$ soit séparable, il faut et il suffit que la $K'$-algèbre $A_{(K')}$ déduite de $A$ par extension des scalaires soit séparable*.

Soit L une extension de K. Soient A une algèbre séparable sur K et B une sous-algèbre de A ; alors l’anneau $L \otimes_K A$ est réduit, et $L \otimes_K B$ est isomorphe à un sous-anneau de $L \otimes_K A$, donc est réduit. Donc B est séparable. Ceci prouve a). On démontre de même b) en utilisant l’isomorphisme canonique de $L \otimes_K \lim_{\longrightarrow} A_i$ avec $\lim_{\longrightarrow} L \otimes_K A_i$ (II, p. 93, prop. 7), et l’on prouve c) en remarquant que $L \otimes_K (\prod_{i \in I} A_i)$ est isomorphe à un sous-anneau de $\prod_{i \in I} (L \otimes_K A_i)$ (II, p. 109, prop. 15).

Utilisons les notations de d). Pour toute extension $L'$ de $K'$, les anneaux $L' \otimes_{K'} A_{(K')}$ et $L' \otimes_K A$ sont isomorphes (II, p. 83, prop. 2). On en déduit que, si A est une K-algèbre séparable, alors $A_{(K')}$ est une $K'$-algèbre séparable. Réciproquement, supposons que $A_{(K')}$ soit une $K'$-algèbre séparable. La remarque précédente montre que l’anneau $L' \otimes_K A$ est réduit pour toute extension $L'$ de K contenant $K'$ comme sous-extension. Soit L une extension de K ; d’après le scholie (V, p. 13), il existe une extension $L'$ de K contenant $K'$ comme sous-extension et un K-homomorphisme de L dans $L'$ ; l’anneau $L \otimes_K A$ est alors isomorphe à un sous-anneau de $L' \otimes_K A$, donc est réduit. Ceci prouve que A est une K-algèbre séparable.

#### Proposition 4 {#alg-v-s15-prop-4 .statement}

*Soit A une algèbre séparable sur un corps K et soit B l’anneau total des fractions de A. Alors la K-algèbre B est séparable.*

Soit S l’ensemble des éléments simplifiables de A. On a identifié (I, p. 108) A à un sous-anneau de B ; de plus, tout élément de S est inversible dans B et tout élément de B est de la forme $as^{-1}$ avec $a \in A$ et $s \in S$. Soient L une extension de K et x un élément nilpotent de $L \otimes_K B$. On peut écrire x sous la forme $x = \sum_{i=1}^n y_i \otimes a_i s_i^{-1}$ avec $y_i \in L, a_i \in A, s_i \in S$ pour $1 \leq i \leq n$. Si l’on pose $s = s_1 \ldots s_n$ alors $x(1 \otimes s)$ appartient au sous-anneau $L \otimes_K A$ de $L \otimes_K B$ ; comme $x(1 \otimes s)$ est nilpotent et A séparable sur K, on a $x(1 \otimes s) = 0$ et comme s est inversible dans B, on a finalement $x = 0$. Ceci prouve que l’anneau $L \otimes_K B$ est réduit, d’où la proposition.

#### Proposition 5 {#alg-v-s15-prop-5 .statement}

*Soient K un corps, A et B deux K-algèbres commutatives. Si A est réduite et B séparable, alors $A \otimes_K B$ est réduite,

D’après le cor. de la prop. 2 (V, p. 114), A est isomorphe à une sous-algèbre d’un produit $\prod_{i \in I} L_i$, où $L_i$ est une extension de K pour tout $i \in I$. Par suite, $A \otimes_K B$ est isomorphe à un sous-anneau de $(\prod_{i \in I} L_i) \otimes_K B$, et ce dernier anneau est isomorphe à un sous-anneau de $\prod_{i \in I} (L_i \otimes_K B)$ (II, p. 109, prop. 15). Comme B est séparable, chacun des anneaux $L_i \otimes_K B$ est réduit, et il en est donc de même de $\prod_{i \in I} (L_i \otimes_K B)$ et *a fortiori* de $A \otimes_K B$.

#### Corollaire 1 {#alg-v-s15-prop-5-cor-1 .statement}

*Soient K un corps, L une extension séparable de K et f un polynôme de K[X]. Si f est sans facteur multiple dans K[X], il est aussi sans facteur multiple dans L[X].*

Si f est sans facteur multiple dans K[X], l’anneau quotient K[X]/(f) est réduit ;

en effet, $f$ est produit de polynômes irréductibles $f_i$ deux à deux étrangers, donc $K[X]/(f)$ est isomorphe d’après I, p. 104, prop. 9, au produit des corps $K[X]/(f_i)$. D’après la prop. 5, l’anneau $L[X]/(f)$ est réduit, puisqu’isomorphe à $L \otimes_K K[X]/(f)$; si $g$ est un polynôme non constant de $L[X]$ tel que $g^2$ divise $f$, alors la classe de $fg^{-1}$ dans $L[X]/(f)$ en est un élément nilpotent non nul ; donc $f$ est sans facteur multiple dans $L[X]$.

#### Corollaire 2 {#alg-v-s15-prop-5-cor-2 .statement}

*Soient A et B deux K-algèbres commutatives. Si A et B sont séparables, il en est de même de A $\otimes_K$ B.*

Soit L une extension de K. L’anneau $L \otimes_K A$ est réduit car A est séparable ; la prop. 5 montre alors que $(L \otimes_K A) \otimes_K B$ (isomorphe à $L \otimes_K (A \otimes_K B)$) est un anneau réduit, d’où le corollaire.

### 3. Extensions séparables

Soit K un corps. Comme une extension de K est une K-algèbre, la notion de séparabilité introduite dans la déf. 1 (V, p. 114) s’applique en particulier au cas des extensions de K. D’après l’exemple 3 (V, p. 114), cette définition de séparabilité coïncide dans le cas des extensions algébriques avec celle du § 7 (V, p. 35, déf. 1).

#### Proposition 6 {#alg-v-s15-prop-6 .statement}

*Toute extension pure d’un corps K est séparable.*

Cela résulte aussitôt de l’exemple 1 (V, p. 114) et de la prop. 4 (V, p. 115).

#### Proposition 7 {#alg-v-s15-prop-7 .statement}

*Soient E un corps, G un groupe d’automorphismes de E et K le sous-corps de E formé des invariants de G. Alors E est une extension séparable de K.*

Soit L une extension de K ; il existe une extension algébriquement close $\Omega$ de L dont le degré de transcendance sur K soit au moins égal à celui de E sur K. D’après le cor. 1 (V, p. 112), il existe un K-homomorphisme $u$ de E dans $\Omega$. Notons $v$ l’homomorphisme de $\Omega$-algèbres de $A = \Omega \otimes_K E$ dans $\Omega$ qui transforme $\lambda \otimes x$ en $\lambda .u(x)$ pour $\lambda \in \Omega$ et $x \in E$ ; notons aussi $a$ le noyau de $v$.

Pour tout $s \in G$, soit $h_s$ l’automorphisme $\mathrm{Id}_\Omega \otimes s$ de la $\Omega$-algèbre A ; le noyau de l’homomorphisme $v \circ h_s$ de A dans $\Omega$ est l’idéal premier $a_s = h_s^{-1}(a)$ de A. Il est clair que l’idéal $b = \bigcap_{s \in G} a_s$ de A est stable par les automorphismes $h_s$. Par suite (V, p. 60, cor.), l’idéal b de A est de la forme $c \otimes_K E$, où c est un idéal de $\Omega$. Or on a $b \subset a \neq A$, d’où $c \neq \Omega$, et comme $\Omega$ est un corps, on a donc $c = 0$, d’où $b = 0$.

La famille $(a_s)_{s \in G}$ d’idéaux premiers de A a donc une intersection nulle. D’après la prop. 2 (V, p. 113), l’anneau A est donc réduit, et il en est *a fortiori* de même du sous-anneau $L \otimes_K E$ de A. Vu l’arbitraire de l’extension L de K, ceci prouve que E est séparable sur K.

#### Proposition 8 {#alg-v-s15-prop-8 .statement}

*Soit L une extension d’un corps K. Si L est séparable sur K, toute sous-extension de L est séparable sur K. Réciproquement, si toute sous-extension de type fini de L est séparable sur K, alors L est séparable sur K.*

Cela résulte aussitôt de la prop. 3, *a*) et *b*) (V, p. 114).

On peut donc dire que la séparabilité est une propriété « de caractère fini ».

#### Proposition 9 {#alg-v-s15-prop-9 .statement}

Soient L une extension d’un corps K et M une L-algèbre commutative (par exemple, une extension de L). Si M est séparable sur L, et L séparable sur K, alors M est séparable sur K.

Soit K’ une extension de K. Comme L est extension séparable de K, l’anneau K’ $\otimes_K$ L est réduit ; comme M est une L-algèbre séparable, la prop. 5 (V, p. 115) montre que l’anneau $(K' \otimes_K L) \otimes_L M$ est réduit. Or l’anneau $K' \otimes_K M$ est isomorphe à $(K' \otimes_K L) \otimes_L M$ (II, p. 83, prop. 2), donc est réduit. Ceci prouve que M est séparable sur K.

Si l’extension M est séparable sur K, elle n’est pas nécessairement séparable sur L (cf. cependant V, p. 119, cor. 3). Par exemple, si p est un nombre premier, le corps $F_p(X)$ des fractions rationnelles en une indéterminée X sur $F_p$ est séparable sur $F_p$ (V, p. 116, prop. 6), mais c’est une extension algébrique radicielle de $F_p(X^p)$; en particulier $F_p(X)$ n’est pas séparable sur $F_p(X^p)$.

Nous étudierons plus loin (V, p. 131, prop. 5) la séparabilité des extensions composées.

### 4. Critère de séparabilité de MacLane

#### Théorème 1 {#alg-v-s15-thm-1 .statement}

Soit K un corps de caractéristique 0. Toute K-algèbre réduite, et en particulier toute extension de K, est séparable sur K.

Montrons d’abord que toute extension L de K est séparable. Soit B une base de transcendance de L sur K (V, p. 105, th. 1) et soit $L_1 = K(B)$. Alors $L_1$ est séparable sur K (V, p. 116, prop. 6). De plus, L est une extension algébrique de $L_1$ et le corps $L_1$ est de caractéristique 0 ; par suite, L est séparable sur $L_1$ (V, p. 36, cor.). D’après la prop. 9, L est donc séparable sur K.

Soit alors A une algèbre réduite sur le corps K. D’après le cor. de la prop. 2 (V, p. 114), il existe une famille $(L_i)_{i \in I}$ d’extensions de K telle que A soit isomorphe à une sous-algèbre de $\prod_{i \in I} L_i$. Chacune des algèbres $L_i$ est séparable sur K par ce qui précède, et A a donc la même propriété d’après la prop. 3, a) et c) (V, p. 114).

#### Théorème 2 {#alg-v-s15-thm-2 .statement}

Soient K un corps de caractéristique $p \neq 0$, $K^{p^{-\infty}}$ une clôture parfaite de K et A une K-algèbre commutative. Les propriétés suivantes sont équivalentes :

a) A est séparable.
b) Il existe une extension K’ de K telle que le corps K’ soit parfait et l’anneau $K' \otimes_K A$ réduit.
c) L’anneau $K^{p^{-\infty}} \otimes_K A$ est réduit.
d) L’anneau $K' \otimes_K A$ est réduit pour toute extension K’ de K, de degré fini et radicielle de hauteur $\leq 1$.
e) Pour toute famille $(a_i)_{i \in I}$ d’éléments de A linéairement libre sur K, la famille $(a_i^p)_{i \in I}$ est linéairement libre sur K.
f) Il existe une base $(a_i)_{i \in I}$ du K-espace vectoriel A telle que la famille $(a_i^p)_{i \in I}$ soit linéairement libre sur K.

Si une extension K’ de K est un corps parfait, elle contient une sous-extension K-isomorphe à $K^{p^{-\infty}}$ (V, p. 6, prop. 3); de plus, toute extension radicielle de K est isomorphe à une sous-extension de $K^{p^{-\infty}}$ (V, p. 25, prop. 3). Ces remarques démontrent les implications $a) \Rightarrow b) \Rightarrow c) \Rightarrow d)$.

Montrons que d) entraîne e). Soit $(a_i)_{i \in I}$ une famille linéairement libre dans $A$ et soit $(\lambda_i)_{i \in I}$ une famille à support fini dans $K$ telle que $\sum_{i \in I} \lambda_i a_i^p = 0$. Soit $K'$ la sous-extension de $K^{p^{-\infty}}$ engendrée par les éléments $\lambda_i^{p^{-1}}$; elle est de degré fini et de hauteur $\leq 1$. Posons $x = \sum_{i \in I} \lambda_i^{p^{-1}} \otimes a_i$ dans $K' \otimes_K A$; on a
$$
x^p = \sum_{i \in I} \lambda_i \otimes a_i^p = 1 \otimes \sum_{i \in I} \lambda_i a_i^p = 0 .
$$
Sous l’hypothèse d), on a $x = 0$, d’où $\lambda_i = 0$ pour tout $i \in I$.

Il est clair que e) entraîne f) et il reste à prouver que f) entraîne a). Soit donc $(a_i)_{i \in I}$ une base de $A$ sur $K$, telle que la famille $(a_i^p)_{i \in I}$ soit linéairement libre sur $K$. Soit $L$ une extension de $K$ et soit $x$ un élément de $L \otimes_K A$ tel que $x^p = 0$. Posons $x = \sum_{i \in I} \lambda_i \otimes a_i$ avec $\lambda_i \in L$ pour tout $i \in I$. On a $x^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p = 0$ et comme la famille $(a_i^p)_{i \in I}$ est linéairement libre sur $K$, on a $\lambda_i^p = 0$, d’où $\lambda_i = 0$ pour tout $i \in I$; finalement, on a $x = 0$. On a prouvé que la relation $x^p = 0$ entraîne $x = 0$ dans $L \otimes_K A$, d’où il résulte immédiatement que $L \otimes_K A$ est réduit.

#### Corollaire 1 (MacLane) {#alg-v-s15-thm-2-cor-1 .statement}

*Soient* $K$ *un corps d’exposant caractéristique* $p$, $\Omega$ *une extension parfaite de* $K$ *et* $L$ *une sous-extension de* $\Omega$. *Les conditions suivantes sont équivalentes* :
  *a)* $L$ *est séparable sur* $K$.
  *b)* $L$ *est linéairement disjointe de* $K^{p^{-\infty}}$ *sur* $K$.
  *c)* $L$ *est linéairement disjointe sur* $K$ *de toute extension radicielle de* $K$ *contenue dans* $\Omega$, *de degré fini et de hauteur* $\leq 1$.

Le cas où $K$ est de caractéristique 0 est trivial puisque $L$ est alors séparable sur $K$ (th. 1), et $K^{p^{-\infty}} = K$ par convention. Supposons donc $p \neq 1$. Montrons d’abord que a) entraîne b). Supposons $L$ séparable sur $K$ et soit $(a_i)_{i \in I}$ une base de $L$ sur $K$. Soit $(\lambda_i)_{i \in I}$ une famille à support fini d’éléments de $K^{p^{-\infty}}$ telle que $\sum_{i \in I} \lambda_i a_i = 0$; il existe un entier $f \geq 0$ et des éléments $\mu_i$ de $K$ tels que $\lambda_i = \mu_i^{p^{-f}}$. On a
$$
\sum_{i \in I} \mu_i a_i^{p^f} = (\sum_{i \in I} \lambda_i a_i)^{p^f} = 0
$$
et le th. 2 entraîne par récurrence sur $f$ que la famille $(a_i^{p^f})_{i \in I}$ est linéairement libre sur $K$. On a donc $\mu_i = 0$, d’où $\lambda_i = 0$ pour tout $i \in I$. Finalement $L$ est linéairement disjointe de $K^{p^{-\infty}}$ sur $K$.

Il est clair que b) entraîne c). Enfin, supposons c) vérifiée et soit $K'$ une extension de $K$, de degré fini et radicielle de hauteur $\leq 1$. L’anneau $K' \otimes_K L$ est isomorphe à un sous-anneau de $\Omega$, donc est réduit. On en déduit par le th. 2 que $L$ est séparable sur $K$.

#### Corollaire 2 {#alg-v-s15-thm-2-cor-2 .statement}

*Soient* $K$ *un corps d’exposant caractéristique* $p$, $K^{p^{-\infty}}$ *une clôture parfaite de* $K$ *et* $L$ *une extension séparable de* $K$. *Alors l’anneau* $L \otimes_K K^{p^{-\infty}}$ *est un corps*. *Si* $L$ *est de plus algébrique sur* $K$, *alors* $L \otimes_K K^{p^{-\infty}}$ *est une clôture parfaite de* $L$.

Le cas $p = 1$ est trivial ; supposons donc $p \neq 1$. Soit $\Omega$ une clôture parfaite de $L$. D’après le cor. 1, il existe un isomorphisme de $K$-algèbres de $L \otimes_K K^{p^{-\infty}}$ sur $L[K^{p^{-\infty}}]$ qui transforme $x \otimes y$ en $xy$ pour $x \in L$ et $y \in K^{p^{-\infty}}$. Comme $K^{p^{-\infty}}$ est algébrique sur $K$, l’anneau $L[K^{p^{-\infty}}]$ est un sous-corps de $\Omega$ (V, p. 18, cor. 1). Supposons de plus $L$ algébrique sur $K$. Alors $L[K^{p^{-\infty}}]$ est une extension algébrique du corps parfait $K^{p^{-\infty}}$, donc c’est un corps parfait (V, p. 42, cor. 1) ; enfin, comme le corps $L[K^{p^{-\infty}}]$ est une extension radicielle de $L$ (V, p. 24, cor.), c’est une clôture parfaite de $L$.

#### Corollaire 3 {#alg-v-s15-thm-2-cor-3 .statement}

*Soient* $L$ *une extension algébrique de* $K$ *et* $M$ *une* $L$*-algèbre commutative* (par exemple une extension de $L$). *Si* $M$ *est séparable sur* $K$, *elle est séparable sur* $L$.

L’algèbre $L$ est $K$-isomorphe à une sous-algèbre de $M$, donc $L$ est extension séparable de $K$. Par suite (cor. 2), il existe un $L$-isomorphisme de $L^{p^{-\infty}}$ sur $K^{p^{-\infty}} \otimes_K L$. L’anneau $L^{p^{-\infty}} \otimes_L M$ est donc isomorphe à $(K^{p^{-\infty}} \otimes_K L) \otimes_L M$, donc à $K^{p^{-\infty}} \otimes_K M$ (II, p. 83, prop. 2) et ce dernier anneau est réduit car $M$ est séparable sur $K$. L’anneau $L^{p^{-\infty}} \otimes_L M$ est donc réduit, ce qui prouve que $M$ est séparable sur $L$ (V, p. 117, th. 2).

#### Remarque {#alg-v-s15-n4-rem-1 .statement}

On peut formuler le critère de MacLane sans faire intervenir d’extension de $K$ autre que $L$. En effet, d’après la condition *c)* du cor. 1, $L$ est séparable sur $K$ si et seulement si $L$ et $K^{p^{-1}}$ sont linéairement disjointes sur $K$. Comme l’application $x \mapsto x^p$ est un isomorphisme de $L$ sur le sous-corps $L^p$, on obtient le critère suivant (cf. V, p. 166, exerc. 11 pour un critère analogue concernant les algèbres) :

*L est séparable sur* $K$ *si et seulement si les sous-corps* $L^p$ *et* $K$ *de* $L$ *sont linéairement disjoints sur* $K^p$.

### 5. Extensions d’un corps parfait

Pour la commodité des références, nous résumons les principales propriétés des extensions des corps parfaits :

#### Théorème 3 {#alg-v-s15-thm-3 .statement}

*Soit* $K$ *un corps parfait*.
a) *Toute extension algébrique de* $K$ *est un corps parfait*.
b) *Toute extension de* $K$ *est séparable*.
c) *Pour qu’une* $K$*-algèbre soit séparable, il faut et il suffit qu’elle soit réduite*.
d) *Soient* $A$ *et* $B$ *deux* $K$*-algèbres réduites*. *Alors* $A \otimes_K B$ *est réduite*.
e) *Si* $E$ *et* $F$ *sont deux extensions de* $K$, *l’anneau* $E \otimes_K F$ *est réduit*.

L’assertion *a)* n’est autre que le cor. 1 de la prop. 11 (V, p. 42).
L’assertion *b)* résulte du th. 1 (V, p. 117) lorsque $K$ est de caractéristique 0, et du cor. 1 (V, p. 118) lorsque $K$ est de caractéristique $p \neq 0$.
Prouvons *c)*. Le cas où $K$ est de caractéristique 0 résulte du th. 1 (V, p. 117). Il suffit donc de montrer que si $K$ est parfait de caractéristique $p \neq 0$ et $A$ est une $K$-algèbre réduite, alors $A$ est séparable sur $K$. Or cela résulte de l’équivalence des conditions *a)* et *b)* du th. 2 (V, p. 117 ; faire $K' = K$ dans *b)*).

Enfin, l’assertion d) résulte de c) et de la prop. 5 (V, p. 115) et e) est un cas particulier de d).

### 6. Caractérisation de la séparabilité par les automorphismes

#### Théorème 4 {#alg-v-s15-thm-4 .statement}

Soient $\Omega$ une extension algébriquement close d’un corps $K$ et $L$ une sous-extension de $\Omega$. Les conditions suivantes sont équivalentes :

a) $L$ est séparable sur $K$.

b) L’intersection des noyaux des homomorphismes de $\Omega$-algèbres de $\Omega \otimes_K L$ dans $\Omega$ est réduite à 0.

c) Quels que soient les éléments $a_1, ..., a_n$ de $L$ linéairement indépendants sur $K$, il existe des $K$-automorphismes $\sigma_1, ..., \sigma_n$ de $\Omega$ tels que $\det(\sigma_i(a_j)) \neq 0$.

d) Soit $V$ un sous-$K$-espace vectoriel de $L$, de dimension finie. Toute application $K$-linéaire de $V$ dans $\Omega$ est combinaison linéaire (à coefficients dans $\Omega$) de restrictions à $V$ de $K$-automorphismes de $\Omega$.

$d) \Rightarrow c)$ : Soient $a_1, ..., a_n$ des éléments de $L$ linéairement indépendants sur $K$ et $V$ le sous-$K$-espace vectoriel de $L$ engendré par $a_1, ..., a_n$. L’application $f \mapsto (f(a_1), ..., f(a_n))$ est une bijection $\Omega$-linéaire de $\mathrm{Hom}_K(V, \Omega)$ sur $\Omega^n$. Supposons d) satisfaite. Il existe alors des $K$-automorphismes $\sigma_1, ..., \sigma_n$ de $\Omega$ tels que les éléments $(\sigma_i(a_1), ..., \sigma_i(a_n))$ de $\Omega^n$ (pour $1 \leq i \leq n$) forment une base de $\Omega^n$. On a $\det(\sigma_i(a_j)) \neq 0$, donc d) entraîne c).

$c) \Rightarrow b)$ : Supposons c) satisfaite et soit $x$ dans $\Omega \otimes_K L$. Écrivons $x$ sous la forme $\sum_{j=1}^n x_j \otimes a_j$ avec $x_1, ..., x_n$ dans $\Omega$ et des éléments $a_1, ..., a_n$ de $L$ linéairement indépendants sur $K$. Choisissons des $K$-automorphismes $\sigma_1, ..., \sigma_n$ de $\Omega$ tels que $\det \sigma_i(a_j) \neq 0$; soient $\chi_1, ..., \chi_n$ les $\Omega$-homomorphismes de $\Omega \otimes_K L$ dans $\Omega$ tels que $\chi_i(a \otimes b) = a \cdot \sigma_i(b)$ pour $a \in \Omega$ et $b \in L$. Supposons que l’on ait $\chi_i(x) = 0$ pour $1 \leq i \leq n$, autrement dit, que l’on ait $\sum_{j=1}^n x_j \cdot \sigma_i(a_j) = 0$ pour $1 \leq i \leq n$.

Comme on a supposé que la matrice $(\sigma_i(a_j))$ a un déterminant non nul, on a par conséquent $x_i = 0$ pour $1 \leq i \leq n$, et finalement $x = 0$.

$b) \Rightarrow a)$ : Comme toute extension d’un corps de caractéristique 0 est séparable (V, p. 117, th. 1), il suffit d’examiner le cas où $K$ est de caractéristique $p \neq 0$. Soient $X$ l’ensemble des homomorphismes de $\Omega$-algèbres de $\Omega \otimes_K L$ dans $\Omega$ et $f$ l’homomorphisme de $\Omega \otimes_K L$ dans $\Omega^X$ défini par $f(u) = (\chi(u))_{\chi \in X}$ pour $u \in \Omega \otimes_K L$. La condition b) signifie que $f$ est injectif et entraîne donc que l’anneau $\Omega \otimes_K L$ est réduit. La condition b) du th. 2 (V, p. 117) est alors satisfaite avec $K' = \Omega$, donc $L$ est séparable sur $K$.

$a) \Rightarrow d)$ : Supposons $L$ séparable sur $K$. Soient $V$ un sous-$K$-espace vectoriel de dimension finie de $L$, $V_{(\Omega)} = \Omega \otimes_K V$ le $\Omega$-espace vectoriel déduit de $V$ par extension des scalaires, et $f_0$ la forme linéaire sur $V_{(\Omega)}$ telle que $f_0(x \otimes y) = xy$ pour $x \in \Omega$ et $y \in V$. Notons $G$ le groupe des $K$-automorphismes de $\Omega$; pour $\sigma \in G$, on pose $\sigma_V = \sigma \otimes \mathrm{Id}_V$ et $g_\sigma = \sigma \circ f_0 \circ \sigma_V^{-1}$.

Pour tout $\sigma \in G$, l’application $g_\sigma$ de $V_{(\Omega)}$ dans $\Omega$ est $\Omega$-linéaire et transforme $x \otimes y$ en $x.\sigma(y)$ pour $x \in \Omega$ et $y \in V$. Le noyau $N_\sigma$ de $g_\sigma$ est donc un sous-espace vectoriel de $V_{(\Omega)}$, et il en est donc de même de $N = \bigcap_{\sigma \in G} N_\sigma$. Si $p$ est l’exposant caractéristique de $K$, le corps des invariants de $G$ dans $\Omega$ est égal à $K^{p^{-}}$ (V, p. 107, prop. 10). On a évidemment $\sigma_V(N) = N$ pour tout $\sigma \in G$; par suite (V, p. 60, cor.), le $\Omega$-espace vectoriel $N$ est engendré par $N_0 = N \cap (K^{p^{-}} \otimes V)$. Comme $L$ est séparable sur $K$, les corps $K^{p^{-}}$ et $L$ sont linéairement disjoints sur $K$ (V, p. 118, cor. 1); on a $K^{p^{-}} \otimes_K V \subset K^{p^{-}} \otimes_K L$ et $f_0(x \otimes y) = xy$ pour $x \in \Omega$ et $y \in V$. Par suite, la restriction de $f_0$ à $K^{p^{-}} \otimes_K V$ est injective. Or $f_0 = g_1$ est nulle sur $N$ et $a fortiori$ sur $N_0 \subset K^{p^{-}} \otimes_K V$. On a donc $N_0 = 0$, d’où $N = 0$. Comme $V$ est de dimension finie sur $K$, $V_{(\Omega)}$ est de dimension finie sur $\Omega$; l’intersection des noyaux des formes linéaires $g_\sigma$ est nulle, donc (II, p. 104, th. 7) la famille $(g_\sigma)_{\sigma \in G}$ engendre le dual de $V_{(\Omega)}$. Soit alors $u$ une application $K$-linéaire de $V$ dans $\Omega$; soit $\tilde{u}$ la forme linéaire sur $V_{(\Omega)}$ qui applique $x \otimes y$ sur $xu(y)$ pour $x \in \Omega$ et $y \in V$. D’après ce qui précède, il existe des éléments $\sigma_1, ..., \sigma_n$ de $G$ et $\lambda_1, ..., \lambda_n$ de $\Omega$ tels que
$$
\tilde{u} = \sum_{i=1}^n \lambda_i g_{\sigma_i}, \text{d’où } u(y) = \sum_{i=1}^n \lambda_i \sigma_i(y) \text{ pour tout } y \in V. \text{ On a prouvé que } a) \text{ entraîne } d).
$$

## EXERCICES {#alg-v-s15-exercises}

See the [exercises for § 15](exercises/s15/).
