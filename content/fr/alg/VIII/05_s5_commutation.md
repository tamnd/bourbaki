---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 5
section_title: Commutation
lang: fr
source: alg-viii-fr
book_pages: A VIII.73-A VIII.89
pdf_pages: 0083-0099
extraction: native
subsections:
    - "no": 1
      title: Commutant et bicommutant d’un module
      page: 73
      pdf_page: 83
    - "no": 2
      title: Modules générateurs
      page: 75
      pdf_page: 85
    - "no": 3
      title: Bicommutant d’un module générateur
      page: 78
      pdf_page: 88
    - "no": 4
      title: Contremodule d’un module semi-simple
      page: 80
      pdf_page: 90
    - "no": 5
      title: Théorème de densité
      page: 83
      pdf_page: 93
    - "no": 6
      title: Application à la théorie des corps
      page: 84
      pdf_page: 94
statements: 37
exercises: 19
content_sha256: c9e9120986305700fdf16b43f31ae23f7e2dcc7b5022b4c947c5783a982b30d4
---

## § 5. COMMUTATION

### 1. Commutant et bicommutant d’un module

Soient E un anneau et B une partie de E. On appelle commutant de B dans E le sous-anneau $B'$ de E formé des éléments qui commutent à tout élément de B. Le commutant $B''$ de $B'$ est appelé le bicommutant de B. On a $B\subset B''$ et $B'$ coïncide avec son bicommutant (III, p. 3). Le centre d’un sous-anneau B de E est $B\cap B'$, le centre commun de $B'$ et $B''$ est $B'\cap B''$. Si B est un sous-anneau commutatif de E, on a $B\subset B'$ et $B''$ est le centre de $B'$ (III, p. 4).

Soient A un anneau et M un A-module à gauche (resp. à droite). Appliquons ces définitions au cas où E est l’anneau des endomorphismes du groupe additif de M et B l’anneau $A_M$ des homothéties de M. Le commutant $A'_M$ de $A_M$ dans E s’appelle le commutant de M ; c’est l’anneau des endomorphismes du A-module M. Le bicommutant $A''_M$ de $A_M$ dans E s’appelle le bicommutant de M ; c’est l’anneau des endomorphismes du contremodule de M (VIII, p. 8, déf. 3). On a $A_M\subset A''_M$, l’anneau $A_M\cap A'_M$ est le centre de $A_M$ et $A'_M\cap A''_M$ est le centre commun de $A'_M$ et $A''_M$.

#### Définition 1 {#alg-viii-s5-def-1 .statement tag=005E}

On dit que le A-module M est équilibré si l’on a $A_M= A''_M$.

Si le A-module M est équilibré, les anneaux $A_M$ et $A'_M$ ont le même centre $A_M\cap A'_M$. Pour que M soit un A-module équilibré, il faut et il suffit qu’il soit un $A_M$-module équilibré. Pour tout A-module M, le contremodule de M est fidèle et équilibré.

Lorsque l’anneau A est commutatif, le bicommutant $A''_M$ de M est le centre de $A'_M=$ End$_A(M)$; dire que M est équilibré signifie que le centre de End$_A(M)$ est réduit aux homothéties.

Pour tout élément $a$ de A, notons $\boldsymbol{\delta }_a$ l’homothétie à droite $x\rightarrow xa$ de A dans A et $\boldsymbol{\gamma }_a$ l’homothétie à gauche $x\rightarrow ax$ (I, p. 92). L’application $a\rightarrow \boldsymbol{\delta }_a$ est un isomorphisme d’anneaux de $A^o$ sur le commutant du A-module $A_s$ (II, p. 150). L’application $a\rightarrow \boldsymbol{\gamma }_a$ est un isomorphisme d’anneaux de A sur le commutant du A-module à droite $A_d($loc. cit.). Si l’on identifie A au commutant de $A_d$ par cette application, le contremodule de $A_d$ s’identifie à $A_s$ et par suite le A-module $A_d$ est équilibré. De même le A-module $A_s$ est équilibré.

Soit $n$ un entier $\geqslant 1$. Considérons $A^n$ comme un $\mathbf{M}_n$(A)-module à gauche (loc. cit.). L’application qui à $m\in \mathbf{M}_n(A)$ associe l’endomorphisme $x\rightarrow mx$ du A-module $A^n_d$ est un isomorphisme d’anneaux de $\mathbf{M}_n(A)$ sur le commutant du A-module à droite $A^n_d($loc. cit.).

#### Proposition 1 {#alg-viii-s5-prop-1 .statement tag=005F}

Soit $(A_i)_{i\in I}$ une famille d’anneaux et, pour tout $i\in I$, soit $M_i$ un $A_i$-module. Posons $A =\prod A_i, M =\prod M_i$ et $N =\bigoplus M_i$. Munissons M de la structure de A-module dont la loi d’action est $((a_i),(x_i))\rightarrow (a_ix_i)$. L’ensemble N est un sous-A-module de M.

a) L’application $(u_i)\rightarrow \prod u_i$ de $\prod$ End$_{\mathbf{Z}}(M_i)$dans End$_{\mathbf{Z}}(M)$ (II, p. 10) définit par passage aux sous-ensembles des isomorphismes d’anneaux de $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$ et $\prod(A_i)''_{M_i}$ sur $A_M, A'_M$ et $A''_M$ respectivement.

b) L’application $(u_i)\rightarrow \bigoplus u_i$ de $\prod$ End$_{\mathbf{Z}}(M_i)$dans End$_{\mathbf{Z}}(N)$ (II, p. 13) définit par passage aux sous-ensembles des isomorphismes d’anneaux de $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$ et $\prod(A_i)''_{M_i}$ sur $A_N, A'_N$ et $A''_N$ respectivement.

L’application $\varphi : (u_i)\rightarrow \prod u_i$ de $\prod$ End$_{\mathbf{Z}}(M_i)$ dans End$_{\mathbf{Z}}(M)$ est un homomorphisme injectif d’anneaux. Par définition de la structure de A-module de M, on a $\varphi (\prod(A_i)_{M_i}) = A_M$. Soit $u\in A'_M$. Pour tout $i\in I$, notons $h_i$ l’élément de A dont toutes les composantes sont égales à 1 sauf celle d’indice $i$ qui est égale à 0 . Si $x$ est un élément de M dont la composante d’indice $i$ est nulle, on a $x=h_ix$, d’où pr$_i(u(x)) =$ pr$_i(u(h_ix)) =$ pr$_i(h_iu(x)) = 0$. Il existe par suite un unique homomorphisme de groupes $u_i: M_i\rightarrow M_i$ telle que pr$_i(u(y)) =u_i$(pr$_i(y))$ pour tout $y\in M$. On a $u=\prod u_i$. Comme l’application $u$ est A-linéaire, l’application $u_i$ est $A_i$-linéaire pour tout $i\in I$. Cela prouve que $A'_M$ est contenu dans l’image de $\prod(A_i)'_{M_i}$ par $\varphi$; l’inclusion opposée est évidente. En appliquant cela au contremodule de M, on en déduit que $\varphi$ induit un isomorphisme de $A''_M$ sur $\prod_i(A_i)''_{M_i}$. Cela prouve l’assertion a).

La démonstration de b) est la même que celle de a) mutatis mutandis.

Les isomorphismes d’anneaux définis dans la prop. 1 sont dits canoniques. On identifie souvent $\prod(A_i)_{M_i}$ à $A_M,\prod(A_i)'_{M_i}$ à $A'_M$, etc. au moyen de ces isomorphismes.

#### Proposition 2 {#alg-viii-s5-prop-2 .statement tag=005G}

Soit A un anneau et soit M un A-module. Soit I un ensemble. Alors le bicommutant du A-module $M^{(I)}$ coïncide avec l’anneau des homothéties du $A''_M$-module $M^{(I)}$.

Pour tout $i\in I$, on note $\pi_i: (x_j)_{j\in I}\rightarrow x_i$ l’homomorphisme de projection de $M^{(I)}$ dans M et $\iota_i: M\rightarrow M^{(I)}$ l’injection canonique correspondante (A, I, p. 45).

Soit $u$ un élément de End$_A(M^{(I)})$. Pour tous $i, j\in I$, l’application composée $u_{i,j}=\pi_j\circ u\circ \iota_i$ appartient au commutant $A'_M$ de M. Pour tout élément $b$ de $A''_M$ et tout $(x_i)\in M^{(I)}$ on a les relations

$$
bu((x_i)_{i\in I}) =b(\sum_{i\in I}u_{i,j}(x_i))_{j\in I}=(\sum_{i\in I}u_{i,j}(bx_i))_{j\in I}=u(b(x_i)_{i\in I})
$$

L’homothétie $b_{M^{(I)}}$ appartient donc au bicommutant du A-module $M^{(I)}$.

Inversement soit $b$ un élément du bicommutant de $M^{(I)}$. Pour tous $i, j\in I$, notons $b_{i,j}=\pi_j\circ b\circ \iota_i$. Soient $i, j\in I$ avec $i\not=j$. Comme $\iota_j\circ \pi_j$ appartient au commutant du A-module $M^{(I)}$, on a

$$
b_{i,j}=\pi_j\circ \iota_j\circ \pi_j\circ b\circ \iota_i=\pi_j\circ b\circ \iota_j\circ \pi_j\circ \iota_i= 0
$$

De même, on a

$$
b_{j,j}=\pi_j\circ b\circ \iota_j=\pi_i\circ \iota_i\circ \pi_j\circ b\circ \iota_j=\pi_i\circ b\circ \iota_i\circ \pi_j\circ \iota_j=b_{i,i}
$$

En outre, $b_{i,i}$ appartient à $A''_M$. Il en résulte que $b$ coïncide avec une homothétie du $A''_M$-module $M^{(I)}$.

### 2. Modules générateurs

Soit A un anneau.

#### Définition 2 {#alg-viii-s5-def-2 .statement tag=005H}

On dit qu’un A-module M est générateur si tout A-module N est engendré par les images des applications A-linéaires de M dans N.

Soit M un A-module à gauche. On note $M^*$ le dual de M et

$$
(x, x^*)\rightarrow  \langle x, x^*\rangle =x^*(x)
$$

la forme bilinéaire canonique sur $M\times M^*$ (II. p. 41). On note $\tau (M)$ l’ensemble des éléments de A de la forme $\sum^n_{i=1}\langle x_i, x^*_i\rangle$, où $x_1, . . . , x_n$ sont des éléments de M, et $x^*_1, . . . , x^*_n$ des éléments de $M^*$. C’est un idéal bilatère de A, qu’on appelle l’idéal trace de M. L’idéal trace du A-module $A_s$ est A. L’idéal trace du module somme directe d’une famille $(M_i)_{i\in I}$ de A-modules est l’idéal $\sum_{i\in I}\tau (M_i)$. Si M est un A-module projectif, il résulte de la prop. 12 de II, p. 46 que l’on a $M =\tau (M)M$.

#### Théorème 1 {#alg-viii-s5-thm-1 .statement tag=005I}

Soit M un A-module à gauche. Les conditions suivantes sont équivalentes :

(i) Le A-module M est générateur ;

(ii) Pour tout A-module N, il existe un ensemble I et une application A-linéaire surjective de $M^{(I)}$ dans N ;

(iii) Il existe un entier $n\geqslant 0$et une application A-linéaire surjective de $M^n$ dans $A_s$;

(iv) Il existe un entier $n\geqslant 0$tel que $A_s$ soit isomorphe à un sous-module facteur direct de $M^n$;

(v) L’idéal trace $\tau (M)$est égal à A ;

(vi) Il existe un entier $n\geqslant 0$, des éléments $x_1, . . . , x_n$ de M et des éléments $x^*_1, . . . , x^*_n$ de $M^*$ satisfaisant à $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$.

(i) $=\Rightarrow$ (ii) : Supposons que M soit générateur et soit N un A-module à gauche. Il existe une famille $(u_i)_{i\in I}$ d’applications A-linéaires de M dans N telle que l’on ait $N =\sum_{i\in I}u_i(M)$. L’application $(x_i)\rightarrow \sum_{i\in I}u_i(x_i)$ de $M^{(I)}$ dans N est A-linéaire et surjective.

(ii) $=\Rightarrow$ (iii) : Appliquons l’hypothèse (ii) au module $N = A_s$. Soit I un ensemble et soit $u: M^{(I)}\rightarrow A_s$ une application linéaire surjective. Comme $A_s$ est engendré par l’élément 1, il existe une partie finie J de I telle que $u(M^{(J)}) = A_s$, d’où (iii).

(iii) $=\Rightarrow$ (iv) : Cela résulte de la prop. 21 de II, p. 27.

(iv) $=\Rightarrow$ (v) : Soit $n\geqslant 1$ un entier tel que $A_s$ soit isomorphe à un sous-module facteur direct de M. On a $A =\tau (A_s)\subset \tau (M^n) =\tau$(M), d’où $\tau (M) = A$.

(v) $=\Rightarrow$ (vi) : C’est clair.

(vi) $=\Rightarrow$ (i) : Soient $n$ un entier $\geqslant 0,x_1, . . . , x_n$ des éléments de M et $x^*_1, . . . , x^*_n$ des éléments de $M^*$ satisfaisant à $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Soit N un A-module à gauche et $y$ un élément de N. Les applications $u_i:x\rightarrow  \langle x, x^*_i\rangle y$ de M dans N sont A-linéaires, et l’on a $y=\sum^n_{i=1}u_i(x_i)$. Cela démontre que M est un A-module générateur.

#### Corollaire {#alg-viii-s5-n2-cor-1 .statement tag=00R1}

Un A-module générateur est fidèle.

Soit $a\in A$ tel que $aM = 0$. En utilisant l’implication (i) $=\Rightarrow$ (iv) du th. 1, on obtient $aA_s= 0$, d’où $a= 0$. Le corollaire en résulte (II, p. 28).

#### Exemple 1 {#alg-viii-s5-n2-exa-1 .statement tag=005J}

Le A-module $A_s$ est générateur.

#### Exemple 2 {#alg-viii-s5-n2-exa-2 .statement tag=005K}

Tout A-module libre non nul est générateur. Plus généralement, tout module dont un quotient est générateur est lui-même générateur.

#### Exemple 3 {#alg-viii-s5-n2-exa-3 .statement tag=005L}

Soit M un A-module semi-simple, dont le contremodule est de type fini. Alors M est un $A_M$-module générateur. En effet, d’après le lemme 4 de VIII, p. 8, il existe un entier naturel $m$ tel que $(A_M)_s$ soit isomorphe à un sous-module de $M^m$. Comme $M^m$ est un $A_M$-module semi-simple, $(A_M)_s$ est isomorphe à un sous-module facteur direct de $M^m$ et M est un $A_M$-module générateur (VIII, p. 76, th. 1).

#### Exemple 4 {#alg-viii-s5-n2-exa-4 .statement tag=005M}

Soit A un anneau principal et soit P un A-module de type fini. Il existe un entier $n\geqslant 1$ et une suite croissante d’idéaux $(\mathfrak{a}_i)_{1\leqslant i\leqslant n}$ de A telle que P soit isomorphe à la somme directe des $A/\mathfrak{a}_i$ (VII, p. 19, th. 2) ; l’annulateur $\mathfrak{a}$ de P est égal à $\mathfrak{a}_1$. Alors P est un module générateur sur l’anneau $A/\mathfrak{a}$. Si P n’est pas un module de torsion, on a $\mathfrak{a}= 0$ et P est un A-module générateur.

#### Lemme 1 {#alg-viii-s5-lem-1 .statement tag=005N}

Soient A un anneau commutatif, M un A-module de type fini et Ann(M) son annulateur. Soit $\mathfrak{a}$ un idéal de A. Les conditions suivantes sont équivalentes :

(i) $\mathfrak{a}M = M$;

(ii) Ann(M) $+\mathfrak{a}= A$;

(iii) Il existe un élément $a$ de $\mathfrak{a}$ tel que $am=m$ pour tout $m\in M$.

(i) $=\Rightarrow$ (ii) : Soit $(x_1, . . . , x_n)$ une famille génératrice du A-module M. Si $\mathfrak{a}M = M$, chacun des $x_i$ peut s’écrire sous la forme $\sum^n_{j=1}c_{ij}x_j$, où les $c_{ij}$ appartiennent à $\mathfrak{a}$. Notons C la matrice $(c_{ij})$ et X la matrice colonne de composantes $x_1, . . . , x_n$. On a ($I_n-C$)X = 0. Soient $d$ le déterminant et V la matrice des cofacteurs de la matrice $I_n-C$. D’après la formule (26) de III, p. 99, on a $dX =^tV$($I_n-C$)X = 0, d’où $d\in$ Ann(M). D’autre part comme les $c_{ij}$ appartiennent à $\mathfrak{a}$ on a $d\equiv$ 1(mod $\mathfrak{a})$ (III, p. 96, (18)), d’où $1\in$ Ann(M) $+\mathfrak{a}$.

(ii) $=\Rightarrow$ (iii) : Sous l’hypothèse (ii), il existe $a\in \mathfrak{a}$ et $b\in$ Ann(M) tels que $a+b= 1$. On a alors $am=m$ pour tout $m\in M$.

(iii) $=\Rightarrow$ (i) : C’est clair.

#### Proposition 3 {#alg-viii-s5-prop-3 .statement tag=00R2}

Soit A un anneau commutatif. Tout A-module projectif de type fini et fidèle est générateur. Plus généralement, un A-module projectif P de type fini est un $A_P$-module générateur.

Soit P un A-module projectif de type fini. On a $\tau (P)P = P$ (VIII, p. 75). Si le A-module P est fidèle, l’idéal $\tau (P)$ est égal à A (lemme 1) et le A-module P est générateur (th. 1), d’où la première assertion. La seconde s’en déduit par le lemme suivant :

#### Lemme 2 {#alg-viii-s5-lem-2 .statement tag=005O}

Soient A un anneau et M un A-module projectif. Le $A_M$-module M est projectif.

Soit $(x_i)_{i\in I}$ une famille génératrice du A-module M. Il existe une famille $(x^*_i)_{i\in I}$ de formes linéaires sur le A-module M telles que, pour tout $x\in M$, la famille $(\langle x, x^*_i\rangle )_{i\in I}$ ait un support fini et que l’on ait $x=\sum_{i\in I}\langle x, x^*_i\rangle x_i$ (II, p. 46, prop. 12). Pour tout $i\in I$, l’application $x\rightarrow  \langle x, x^*_i\rangle_M$ est une forme linéaire sur le $A_M$-module M, et l’on a $x=\sum_{i\in I}\langle x, x^*_i\rangle_Mx_i$ pour tout $x\in M$. D’après loc. cit., M est un $A_M$-module projectif.

### 3. Bicommutant d’un module générateur

#### Théorème 2 {#alg-viii-s5-thm-2 .statement tag=005P}

Un module générateur est équilibré.

Soit A un anneau et soit M un A-module générateur ; par définition, il existe un entier $n\geqslant 0$, des éléments $x_1, . . . , x_n$ de M et des éléments $x^*_1, . . . , x^*_n$ du dual $M^*$ de M satisfaisant à $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Rappelons (II, p. 77) que l’on définit un homomorphisme de groupes $\theta : M^*\otimes_AM\rightarrow$ End$_A(M)$ par la formule $\theta (x^*\otimes y)(x) =$ $\langle x, x^*\rangle y$. Si $u$ est un élément du bicommutant de M, il commute avec End$_A(M)$; on a donc pour tout $y\in M$

$$
u(y) =u(\sum_{i=1}^n\langle x_i, x^*_i\rangle y)=\sum_{i=1}^nu(\theta (x^*_i\otimes y)(x_i))
$$

$$
=\sum_{i=1}^n\theta (x^*_i\otimes y)(u(x_i)) =(\sum_{i=1}^n\langle u(x_i), x^*_i\rangle )y
$$

Par suite $u$ appartient à $A_M$, et M est équilibré.

#### Corollaire 1 {#alg-viii-s5-thm-2-cor-1 .statement tag=005Q}

Un module libre est équilibré.

C’est clair si le module est nul, et un module libre non nul est générateur (VIII, p. 76, exemple 2).

#### Corollaire 2 {#alg-viii-s5-thm-2-cor-2 .statement tag=00R3}

Soit A un anneau et soit $n$ un entier $\geqslant 0$. Le centre de $\mathbf{M}_n(A)$ est formé des matrices scalaires à éléments dans le centre de A. Considérons $A^n$ comme un $\mathbf{M}_n(A)$-module à gauche (II, p. 150). Les endomorphismes de ce module sont les applications $x\rightarrow xa$, où $a$ parcourt A.

Soit M le A-module à droite $A^n_d$. Il est équilibré par le corollaire 1. Par suite, les centres de $A_M, A'_M$ et $A''_M$ coïncident. Le corollaire 2 résulte alors de ce que $A_M$ s’identifie à A et $A'_M$ à $\mathbf{M}_n(A)$.

#### Remarque {#alg-viii-s5-n3-rem-1 .statement tag=005R}

Soit M un A-module. Si le $A_M$-module M est générateur, on a $A_M=$ $A''_M$ d’après le th. 2 appliqué au $A_M$-module M, de sorte que M est un A-module équilibré.

#### Corollaire 3 {#alg-viii-s5-thm-2-cor-3 .statement tag=005S}

Tout module projectif de type fini sur un anneau commutatif est équilibré.

En effet, un module projectif de type fini M est un $A_M$-module générateur par la prop. 3 de VIII, p. 77. Le corollaire résulte donc de la remarque ci-dessus.

#### Corollaire 4 {#alg-viii-s5-thm-2-cor-4 .statement tag=005T}

Tout module de type fini sur un anneau principal est équilibré.

En effet, un module de type fini M sur un anneau principal A est un $A_M$-module générateur (VIII, p. 77, exemple 4).

#### Corollaire 5 {#alg-viii-s5-thm-2-cor-5 .statement tag=005U}

Soient K un corps commutatif, V un espace vectoriel de dimension finie sur K$,u$ et $v$ des endomorphismes de V. Les conditions suivantes sont équivalentes :

(i) Il existe un polynôme P dans K[X] tel que $v= P(u)$;

(ii) L’endomorphisme $v$ commute à tout endomorphisme de V qui commute à $u$.

Prenons pour A l’anneau K[X] et pour M le K[X]-module déduit de V et de $u$ (VII, p. 28). L’assertion (i) signifie que $v\in K[X]_M$ et (ii) que $v\in K[X]''_M$. Le corollaire 5 est donc un cas particulier du corollaire 4.

#### Proposition 4 {#alg-viii-s5-prop-4 .statement tag=005V}

Un module semi-simple dont le contremodule est de type fini est équilibré.

Cela résulte de l’exemple 3 de VIII, p. 77 et de la remarque.

#### Corollaire 1 {#alg-viii-s5-prop-4-cor-1 .statement tag=005W}

Soit $(S_i)_{i\in I}$ une famille finie de A-modules simples deux à deux non isomorphes. Pour $i\in I$, notons $D_i$ l’anneau opposé du corps des endomorphismes de $S_i$. Supposons que, pour tout $i\in I$, le $D_i$-espace vectoriel $S_i$ soit de dimension finie. Alors l’application $a\rightarrow (a_{S_i})_{i\in I}$ de A dans $\prod_{i\in I}$ End$_{D_i}(S_i)$est surjective.

Considérons le A-module $M =\prod_{i\in I}S_i$. Comme I est fini, on a aussi $M =\bigoplus_{i\in I}S_i$ et l’image de $S_i$ dans M est le composant isotypique de type $S_i$ de M. Par suite, les endomorphismes du A-module M sont les applications $(s_i)\rightarrow (s_id_i)$, où $(d_i)_{i\in I}$ parcourt $\prod_{i\in I}D_i$ (VIII, p. 62, prop. 5). Comme I est fini et que, pour tout $i\in I$, le $D_i$-espace vectoriel à droite $S_i$ est de dimension finie, le contremodule de M est de type fini. D’après la prop. 4, le A-module M est équilibré. Or le bicommutant du A-module M se compose des éléments de End$_{\mathbf{Z}}(M)$ de la forme $\prod_{i\in I}u_i$, où $(u_i)\in \prod_{i\in I}$ End$_{D_i}(S_i)$ (VIII, p. 74, prop. 1) puisque End$_{D_i}(S_i)$ est le bicommutant de $S_i$. Le corollaire résulte de là.

Ce corollaire s’applique en particulier lorsque A est une algèbre sur un corps commutatif K et que chacun des $S_i$ est un A-module simple, de dimension finie comme K-espace vectoriel : en effet, $D_i$ contient alors les homothéties $\alpha_{S_i}$, où $\alpha$ parcourt K, et $S_i$ est de dimension finie sur $D_i$ puisqu’il l’est sur K.

#### Corollaire 2 {#alg-viii-s5-prop-4-cor-2 .statement tag=00S0}

Soit A une algèbre sur un corps commutatif algébriquement clos K, et soit S un A-module simple, de dimension finie comme espace vectoriel sur K. Alors l’application $a\rightarrow a_S$ de A dans End$_K(S)$est surjective.

En effet, le corps des endomorphismes du A-module S se compose des homothéties $\alpha_S$, avec $\alpha \in K$ (VIII, p. 43, th. 1). On applique alors le corollaire 1 au A-module simple S.

### 4. Contremodule d’un module semi-simple

Soit A un anneau. On note $\mathscr{S}$ l’ensemble des classes de A-modules simples. Pour tout $\lambda \in \mathscr{S}$, on choisit un A-module simple $S_{\lambda}$ de classe $\lambda$ et on note $D_{\lambda}$ l’anneau opposé du corps des endomorphismes de $S_{\lambda}$. On considère $S_{\lambda}$ comme un $(A,D_{\lambda}$)-bimodule.

Soit M un A-module semi-simple et soit B l’anneau des endomorphismes de M. On note C le bicommutant de M. Pour tout $\lambda \in \mathscr{S}$, on note $V_{\lambda}$ le $(D_{\lambda}$, B)-bimodule à gauche Hom$_A(S_{\lambda},M)$. Enfin, on note $\mathscr{S}_M$ le support du A-module M (VIII, p. 62) ; c’est aussi l’ensemble des éléments $\lambda$ de $\mathscr{S}$ tels que $V_{\lambda}$ soit non nul.

#### Remarque 1 {#alg-viii-s5-n4-rem-1 .statement tag=00R4}

La description canonique $\alpha_M$ du A-module M est un isomorphisme de $(A$, B)-bimodules à gauche. D’après VIII, p. 67, cor. de la prop. 9, l’application $f\rightarrow ($Hom(1$_{S_{\lambda}}, f))_{\lambda\in\mathscr{S}_M}$ de B dans $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(V_{\lambda})$ est un isomorphisme d’anneaux.

#### Proposition 5 {#alg-viii-s5-prop-5 .statement tag=005X}

a) Le contre-module de M est semi-simple.

b) Pour tout $\lambda \in \mathscr{S}_M$, le B-module $V_{\lambda}$ est simple et son commutant est égal à $(D_{\lambda})_{V_{\lambda}}$.

c) L’application $\lambda \rightarrow$ cl(V$_{\lambda})$est une bijection du support du A-module M sur le support de son contremodule.

d) Pour tout $\lambda \in \mathscr{S}_M$, le sous-B-module $M_{\lambda}$ est le composant isotypique de type $V_{\lambda}$ du B-module M et la multiplicité de $V_{\lambda}$ dans M est égale à dim$_{D_{\lambda}}(S_{\lambda})$.

e) Pour $s\in S$, notons $\widetilde{s}$ l’application $\varphi \rightarrow \varphi (s)$de $V_{\lambda}=$ Hom$_A(S_{\lambda},M)$dans M. Elle est B-linéaire. L’application $s\rightarrow \widetilde{s}$ de $S_{\lambda}$ dans Hom$_B(V_{\lambda},M)$ainsi définie est un isomorphisme de $(A,D_{\lambda})$-bimodules.

Soit $\lambda \in \mathscr{S}_M$. Notons $E_{\lambda}$ l’anneau End$_{D_{\lambda}}(V_{\lambda})$; comme $V_{\lambda}$ est un $D_{\lambda}$-espace vectoriel non nul, c’est un $E_{\lambda}$-module simple (VIII, p. 41, exemple 3) et son commutant est égal à $(D_{\lambda})_{V_{\lambda}}$ (VIII, p. 78, cor. 1 du th. 2). Comme $E_{\lambda}$ est l’anneau des homothéties du B-module $V_{\lambda}$ (VIII, p. 67, cor. de la prop. 9), cela prouve b).

La description canonique $\alpha_M$ de M définit un isomorphisme $\alpha_{\lambda}$ de $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ sur $M_{\lambda}$. Comme $V_{\lambda}$ est un B-module simple, le B-module $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ est isotypique de type $V_{\lambda}$ (VIII, p. 57, prop. 1) ; il en est donc de même du B-module $M_{\lambda}$, ce qui prouve a).

D’après la remarque 1 ci-dessus, il existe des éléments $e_{\lambda}$ de B, pour $\lambda$ parcourant $\mathscr{S}_M$, tels que $(e_{\lambda})_{V_{\lambda}}= 1_{V_{\lambda}}$ et $(e_{\lambda})_{V_{\mu}}= 0$ pour $\mu \in \mathscr{S}_M,\mu \not=\lambda$. Les B-modules simples $V_{\lambda}$ sont donc deux à deux non isomorphes, ce qui prouve c) et la première assertion de d). Le B-module $M_{\lambda}$ est isomorphe à $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$, donc dim$_{D_{\lambda}}(S_{\lambda})$ est la multiplicité de $V_{\lambda}$ dans M (II, p. 62, cor. 1).

L’application $\sum_{\lambda\in\mathscr{S}_M}\alpha_{\lambda}$ de $\bigoplus_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ dans M fournit une description (VIII, p. 65, définition 5) du B-module semi-simple M. D’après VIII, p. 66, prop. 8 b), pour tout $\lambda \in \mathscr{S}_M$, l’application de $S_{\lambda}$ dans Hom$_B(V_{\lambda},M)$ décrite en e) est bijective et $D_{\lambda}$-linéaire. Comme elle est manifestement A-linéaire, cela prouve e).

#### Remarque 2 {#alg-viii-s5-n4-rem-2 .statement tag=00R5}

Il résulte de la démonstration que l’application induite

$$
\sum_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}\rightarrow M
$$

par la description canonique de M est une description du contre-module de M.

#### Proposition 6 {#alg-viii-s5-prop-6 .statement tag=005Y}

a) Considéré comme $(A,B^o)$-bimodule, M est semi-simple.

b) Pour tout $\lambda \in \mathscr{S}_M, M_{\lambda}$ est un sous-$(A,B^o)$-bimodule simple de M.

c) Pour tout sous-$(A,B^o)$-bimodule N de M, il existe une unique partie Λ de $\mathscr{S}_M$ tel que N soit égal à $\oplus_{\lambda\in\Lambda}M_{\lambda}$.

Soit $\lambda$ dans $\mathscr{S}_M$. Le A-module à gauche $S_{\lambda}$ et le B-module à droite $V_{\lambda}$ sont simples et $D_{\lambda}$ est l’anneau opposé du corps des endomorphismes de $S_{\lambda}$. D’après le cor. 2 de VIII, p. 59, le $(A,B^o$)-bimodule $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ est simple et il en est de même de $M_{\lambda}$, qui lui est isomorphe. Cela démontre b) et a) en résulte.

Si $\lambda$ et $\mu$ sont distincts dans $\mathscr{S}_M, M_{\lambda}$ et $M_{\mu}$ ne sont pas isomorphes en tant que A-modules, ni a fortiori en tant que $(A,B^o$)-bimodules. L’assertion c) en résulte d’après le cor. 2 de VIII, p. 63.

#### Proposition 7 {#alg-viii-s5-prop-7 .statement tag=005Z}

a) Pour tout élément $c$ du bicommutant C de M et pour tout $\lambda \in \mathscr{S}_M$, il existe un unique élément $c_{\lambda}$ de End$_{D_{\lambda}}(S_{\lambda})$tel que, pour tout $\varphi \in$ Hom$_A(S_{\lambda},M)$et tout $s\in S_{\lambda}$, on ait $c\varphi (s) =\varphi (c_{\lambda}s)$.

b) Munissons les $S_{\lambda}$, pour $\lambda$ parcourant $\mathscr{S}_M$, de la structure de C-module définie par a). Alors l’application canonique $\alpha_M$ de $\bigoplus_{\lambda\in\mathscr{S}_M}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ dans M est un isomorphisme de $(C,B^o)$-bimodules.

c) L’application $c\rightarrow (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ est un isomorphisme de C sur $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(S_{\lambda})$.

Les assertions a) et c) résultent de VIII, p. 66, prop. 9, puisque l’application canonique $\alpha_M$ de $\oplus_{\lambda\in\mathscr{S}_M}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$ dans M fournit une description du B-module M (remarque 2). En outre $\alpha_M$ est $(C,B^o$)-linéaire, ce qui prouve b).

#### Remarque 3 {#alg-viii-s5-n4-rem-3 .statement tag=0060}

Munissons $S_{\lambda}$, pour $\lambda \in \mathscr{S}_M$, de la structure de C-module donnée par la proposition 7, a). Si l’on remplace A par B et B par C dans la proposition 5 (VIII, p. 80), on voit que, pour tout $\lambda \in \mathscr{S}_M$, le C-module à gauche $S_{\lambda}$ est simple, de commutant $D_{\lambda}$, que le composant isotypique de type $S_{\lambda}$ du C-module M est égal à $M_{\lambda}$ et que l’application $\lambda \rightarrow$ cl$_C(S_{\lambda})$ est une bijection du support du A-module M sur le support du C-module M. Notons enfin qu’il y a identité entre applications A-linéaires et applications C-linéaires de $S_{\lambda}$ dans M, entre sous-A-modules et sousC-modules de M, et que les anneaux End$_A(M)$ et End$_C(M)$ sont égaux.

Soit M un module semi-simple. Notons Z le centre du bicommutant C du A-module M ; c’est aussi le centre du commutant B de M. On munit M et les $S_{\lambda}$ pour $\lambda \in \mathscr{S}_M$ des structures de Z-modules déduites par restriction des scalaires de celles de C-modules. Pour tout $\lambda \in \mathscr{S}_M$, on note $Z_{\lambda}$ le centre du corps $D_{\lambda}$.

#### Proposition 8 {#alg-viii-s5-prop-8 .statement tag=0061}

a) L’application $z\rightarrow (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ est un isomorphisme de Z sur le produit des corps $Z_{\lambda}$.

b) Pour que le A-module M soit isotypique et non nul, il faut et il suffit que Z soit un corps.

c) Soit Λ une partie de $\mathscr{S}_M$. Notons $e_{\Lambda}$ l’unique élément de Z tel que $(e_{\Lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ pour $\lambda \in \Lambda$et $(e_{\Lambda})_{S_{\lambda}}= 0$pour $\lambda \in \mathscr{S}_M-\Lambda$. On a $(e_{\Lambda})_{M_{\lambda}}= 1_{M_{\lambda}}$ pour $\lambda \in \Lambda$et $(e_{\Lambda})_{M_{\lambda}}= 0$pour $\lambda \in \mathscr{S}_M-\Lambda$.

d) Si le support $\mathscr{S}_M$ de M est fini, l’application $\Lambda \rightarrow e_{\Lambda}Z$est une bijection de l’ensemble des parties de $\mathscr{S}_M$ sur l’ensemble des idéaux de Z et l’application $\mathfrak{a}\rightarrow \mathfrak{a}M$ est une bijection de l’ensemble des idéaux de Z sur l’ensemble des sous-$(A,B^o)$-bimodules de M. Ces bijections sont des isomorphismes d’ensembles ordonnés. La bijection réciproque associe à un sous $(A,B^o)$-bimodule N de M l’idéal formé des éléments $z$ de Z qui appliquent N dans M.

Pour $\lambda \in \mathscr{S}_M, Z_{\lambda}$ est le centre commun du commutant $D_{\lambda}$ et du bicommutant $C_{\lambda}$ du A-module $S_{\lambda}$. D’après la prop. 7 c) ci-dessus, l’application $c\rightarrow (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ est un isomorphisme de C sur $\prod_{\lambda\in\mathscr{S}}C_{\lambda}$. Par restriction aux centres, on obtient l’isomorphisme $z\rightarrow (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ de Z sur$^{^M}\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$, d’où a).

Pour que l’anneau $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$ soit un corps, il faut et il suffit que l’ensemble $\mathscr{S}_M$ ait un seul élément, d’où b).

L’assertion c) résulte de la prop. 7 a). Supposons $\mathscr{S}_M$ fini. On déduit de a) et de la prop. 8 de I, p. 104, que l’application $\Lambda \rightarrow e_{\Lambda}Z$ est un isomorphisme d’ensembles ordonnés de $\mathfrak{P}(\mathscr{S}_M)$ sur l’ensemble des idéaux de Z. Soit Λ une partie de $\mathscr{S}_M$. D’après c), on a la relation $e_{\Lambda}$ZM $=e_{\Lambda}M =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$; Compte tenu de la prop. 6, c) de VIII, p. 81, il ne reste plus qu’à décrire la bijection réciproque. Mais pour que $z\in Z$ applique M dans $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$, il faut et il suffit que l’on ait $z=e_{\Lambda}z$, c’est-à-dire $z\in e_{\Lambda}Z$.

#### Corollaire {#alg-viii-s5-n4-cor-1 .statement tag=0062}

Supposons que A soit une algèbre sur un corps commutatif algébriquement clos K et que M soit un A-module semi-simple de dimension finie comme espace vectoriel sur K. Pour tout $\lambda$ dans $\mathscr{S}_M$, notons $e_{\lambda}$ le projecteur dans M d’image $M_{\lambda}$ et de noyau $\oplus_{\lambda\not=\mu}M_{\mu}$. Alors $(e_{\lambda})_{\lambda\in\mathscr{S}_M}$ est une base de l’espace vectoriel Z sur K.

Comme M est un espace vectoriel de dimension finie sur K, somme directe de la famille de sous-modules non nuls $(M_{\lambda})_{\lambda\in\mathscr{S}_M}$, l’ensemble $\mathscr{S}_M$ est fini et chacun des espaces $S_{\lambda}$ pour $\lambda \in \mathscr{S}_M$ est de dimension finie sur K. Le corps K étant algébriquement clos, on a $D_{\lambda}= Z_{\lambda}= K$ (VIII, p. 43, th. 1) et l’application $z\rightarrow (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ est un isomorphisme de Z sur $K^{\mathscr{S}_M}$ (prop. 8, a)). Le corollaire résulte alors de la partie c) de la prop. 8.

### 5. Théorème de densité

#### Théorème 3 {#alg-viii-s5-thm-3 .statement tag=00S1}

Soit M un A-module semi-simple et soit $c$ un endomorphisme du groupe additif de M. Pour que $c$ appartienne au bicommutant $A''_M$ de M, il faut et il suffit qu’il satisfasse à la condition suivante :

(D) Pour toute partie finie F de M, il existe un élément $a$ de A tel que $c$ coïncide avec $a_M$ sur F.

Supposons d’abord que $c$ satisfasse à la condition (D). Soit $u$ un élément de $A'_M$. Soit $x$ un élément de M et appliquons la condition (D) à la partie $F =\{x, u(x)\}$. Il existe un élément $a$ de A tel que $c(x) =ax$ et $c(u(x)) =au(x)$, d’où $u(c(x)) =$ $u(ax) =au(x) =c(u(x))$. Comme $x$ est arbitraire, on a $cu=uc$; ceci valant pour tout $u$, on a $c\in A''_M$.

Pour la réciproque, nous allons utiliser le lemme suivant.

#### Lemme 3 {#alg-viii-s5-lem-3 .statement tag=0063}

Soit M un A-module semi-simple. Soit B le bicommutant du A-module M. Alors tout sous-A-module de M est un sous-B-module de M.

Soit N un sous-A-module de M. Par le cor. 2 de VIII, p. 52 il existe un projecteur $p$ du A-module M d’image N. Comme on a la relation $pb=bp$ pour tout $b\in B$, on obtient que N est un sous-B-module de M.

Terminons la preuve du théorème 3. Supposons que $c$ appartienne à $A''_M$ et soit $F =\{x_1, . . . , x_n\}$ une partie finie de M. Notons $x$ l’élément $(x_1, . . . , x_n)$ de $M^n$. Le A-module $M^n$ est semi-simple et, par la prop. 2 de VIII, p. 75, son bicommutant coïncide avec les homothéties du $A''_M$-module $M^n$. Par le lemme 3, le sous-A-module $Ax$ de $M^n$ est un sous-A$''_M$-module de $M^n$. Soit $a\in A$ tel que $(cx_1, . . . , cx_n)$ soit égal à $ax$. Alors $c$ coïncide avec $a_M$ sur $\{x_1, . . . , x_n\}$, ce qui entraîne la condition (D).

#### Remarque {#alg-viii-s5-n5-rem-1 .statement tag=0064}

Notons E l’anneau des endomorphismes du groupe additif de M. Munissons M de la topologie discrète ; l’anneau E se compose d’applications de M dans M et on peut le munir de la topologie induite par la topologie produit de $M^M$ (« topologie de la convergence simple dans M », TG, I, p. 14). La topologie de E est séparée et compatible avec la structure de groupe additif de E. Pour tout $f$ dans E, les applications $g\rightarrow f\circ g$ et $g\rightarrow g\circ f$ de E dans E sont continues. Par suite, le commutant de toute partie de E est fermé dans E. Le théorème 3 entraîne donc que $A''_M$ est l’adhérence de $A_M$ dans E.

### 6. Application à la théorie des corps

#### Proposition 9 {#alg-viii-s5-prop-9 .statement tag=0065}

Soient L un corps et E un sous-anneau de End$_{\mathbf{Z}}(L)$qui contient l’application $\boldsymbol{\gamma }_a:x\rightarrow ax$ pour tout $a\in L$. Notons K l’ensemble des éléments $a$ de L tels que $u(xa) =u(x)a$ pour tout $x$ dans L et tout $u$ dans E ; c’est un sous-corps de L.

Soit V un sous-espace vectoriel de dimension finie du K-espace vectoriel à droite L, et soit $h$ une application K-linéaire de V dans L. Il existe un élément de E qui coïncide avec $h$ sur V.

Considérons L comme un E-module à gauche. Comme E contient les multiplications à gauche $\boldsymbol{\gamma }_a$, tout sous-E-module de L est un idéal à gauche du corps L ; le E-module L est donc simple. Tout endomorphisme du groupe additif de L qui commute aux $\boldsymbol{\gamma }_a$ est de la forme $\boldsymbol{\delta }_b:x\rightarrow xb$ avec $b$ dans L. Par suite, $b\rightarrow \boldsymbol{\delta }_b$ est un isomorphisme de K sur l’anneau opposé de End$_E$(L), qui est un corps.

Le bicommutant $E''$ du E-module L se compose donc des endomorphismes du K-espace vectoriel à droite L. Soit $v$ un endomorphisme du K-espace vectoriel L dont la restriction à V coïncide avec $h$; c’est un élément de $E''$. Soit $(x_i)_{i\in I}$ une base de V sur K ; d’après le th. 3 (VIII, p. 83), il existe un élément $u$ de E tel que $u(x_i) =v(x_i) =h(x_i)$ pour $i\in I$. Par linéarité, on en déduit $u(x) =h(x)$ pour tout $x$ dans V.

#### Corollaire {#alg-viii-s5-n6-cor-1 .statement tag=0066}

Soit L un corps. Soit Γ un sous-groupe du groupe des automorphismes du corps L et soit K le corps des invariants de Γ. Soit V un sous-K-espace vectoriel à droite de L, de dimension finie $n$ sur K. Il existe alors des éléments $\sigma_1, . . . , \sigma_n$ de Γ possédant la propriété suivante : pour toute application K-linéaire $u$ de V dans L, il existe des éléments $a_1, . . . , a_n$ de L tels qu’on ait $u(x) =\sum^n_{i=1}a_i\sigma_i(x)$ pour tout $x$ dans V.

Notons E l’ensemble des applications de L dans L de la forme $x\rightarrow \Sigma_{\sigma\in\Gamma}a_{\sigma}\sigma (x)$, où $(a_{\sigma})_{\sigma\in\Gamma}$ est une famille à support fini d’éléments de L. On a $\boldsymbol{\gamma }_a\in E$ pour tout $a$ dans L et E est un sous-anneau de l’anneau des endomorphismes du groupe additif de L. De plus, le corps K se compose des éléments $a$ de L tels que $u(xa) =u(x)a$ pour tout $x$ dans L et tout $u$ dans E.

Soit H le L-espace vectoriel à gauche Hom$_K(V,L)$; il est de dimension $n$. D’après la prop. 9, il est engendré par les restrictions à V des éléments de Γ. Il existe $n$ éléments $\sigma_1, . . . , \sigma_n$ de Γ dont les restrictions à V forment une base de H sur L. Le corollaire résulte de là.

#### Remarque {#alg-viii-s5-n6-rem-1 .statement tag=0067}

Lorsque le corps L est commutatif, ce corollaire se réduit au théorème d’Artin (V, p. 63).

## EXERCICES {#alg-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
