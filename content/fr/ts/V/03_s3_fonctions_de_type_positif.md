---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 3
section_title: Fonctions de type positif
lang: fr
source: ts-iii-v-fr
book_pages: TS V.431-TS V.456, TS V.492-TS V.504
pdf_pages: 0444-0469, 0505-0517
extraction: native
subsections:
    - "no": 1
      title: Noyaux universellement positifs
      page: 432
      pdf_page: 445
    - "no": 2
      title: Complément sur le calcul fonctionnel holomorphe
      page: 435
      pdf_page: 448
    - "no": 3
      title: Formes linéaires positives
      page: 436
      pdf_page: 449
    - "no": 4
      title: Représentations des algèbres stellaires
      page: 441
      pdf_page: 454
    - "no": 5
      title: Fonctions de type positif sur un groupe topologique
      page: 442
      pdf_page: 455
    - "no": 6
      title: Dual unitaire d’un groupe localement compact
      page: 446
      pdf_page: 459
    - "no": 7
      title: Existence de représentations irréductibles
      page: 450
      pdf_page: 463
    - "no": 8
      title: Fonctions de type positif sur un groupe localement compact commutatif
      page: 454
      pdf_page: 467
statements: 39
exercises: 23
content_sha256: 8f947608d99ac54e80cc4c5fd4f082600da39e3898f055783986ac1426b514c2
---

## § 3. FONCTIONS DE TYPE POSITIF

Dans ce paragraphe, tous les espaces vectoriels, ainsi que tous les espaces hilbertiens et les algèbres considérées, sont sur $\mathbf{C}$, sauf mention du contraire.

### 1. Noyaux universellement positifs

Dans ce numéro, X est un espace topologique séparé.

#### Théorème 1 {#ts-v-s3-thm-1 .statement tag=03BX}

Soit $f\in \mathscr{C}(X\times X)$. Les conditions suivantes sont équivalentes :

(i) Pour toute partie compacte Y de X et toute mesure positive $\mu$ sur Y, l’endomorphisme de $L^2(Y, \mu)$ défini par le noyau $f|(Y\times Y)$ (déf. 1 de III, p. 29) est positif, autrement dit, on a

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)\geqslant 0
$$

pour tout $h\in \mathscr{L}^2(Y, \mu)$;

(ii) Pour tout entier $n\in \mathbf{N}$, toute famille $(x_i)_{0\leqslant i\leqslant n}$ dans X et toute famille $(t_i)_{0\leqslant i\leqslant n}$ de nombres complexes, on a

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

(iii) Il existe un espace hilbertien complexe E et une application continue $g: X\rightarrow E$ d’image totale telle que $f(x, y) =\langle g(x)|g(y)\rangle$ pour tous $x$ et $y$ dans X ;

(iv) Il existe un espace hilbertien complexe E et une application continue $g: X\rightarrow E$ telle que $f(x, y) =\langle g(x)|g(y)\rangle$ pour tous $x$ et $y$ dans X.

Il est apparent que (iii) implique (iv) et on voit que (i) implique (ii) en considérant la mesure discrète $\mu$ qui est l’image de la mesure de comptage sur $\{0, . . . , n\}$ par l’application $i\mapsto x_i$ et la fonction $h$ telle que

$$
h(x) =\sum_{0\leqslant i\leqslant n}t_i
$$

$x_i=x$

Démontrons que (iv) implique (i). Supposons qu’il existe un espace hilbertien complexe E et une application continue $g: X\rightarrow E$ tels que $f(x, y) =\langle g(x)|g(y)\rangle$ pour tout $(x, y)\in X\times X$. Soient Y une partie compacte de $X,\mu$ une mesure positive sur Y et $h\in \mathscr{L}^2(Y, \mu)$. On a

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)
$$

$$
=\int_{Y\times Y}\overline{h(x)}h(y)\langle g(x)|g(y)\rangle d(\mu\otimes \mu)(x, y)
$$

$$
=\langle\int_Yh(x)g(x)d\mu(x)|\int_Yh(y)g(y)d\mu(y)\rangle\geqslant 0
$$

d’après INT, V, p. 97, § 8, n$^o4$, prop. 9.

Démontrons enfin que (ii) implique (iii). Soit $\widetilde{E}$ l’espace des mesures complexes à support fini sur X. Pour $\mu_1$ et $\mu_2$ dans $\widetilde{E}$, on pose

$$
\langle \mu_1|\mu_2\rangle =\int_{X\times X}f(x, y) (\overline{\mu}_1\otimes \mu_2)(x, y)
$$

La forme sesquilinéaire ainsi définie sur $\widetilde{E}$ est une forme hermitienne positive. En effet, soit $\mu\in \widetilde{E}$; il existe une famille finie $(x_i)_{0\leqslant i\leqslant n}$ dans X et des nombres complexes $(t_i)_{0\leqslant i\leqslant n}$ tels que $\mu=\sum^n_{i=0}t_i\varepsilon_{x_i}$. On a alors

$$
\langle \mu|\mu\rangle =\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

par hypothèse. On définit $\widetilde{g}: X\rightarrow \widetilde{E}$ par $\widetilde{g}(x) =\varepsilon_x$. L’image de l’application $\widetilde{g}$ engendre $\widetilde{E}$. De plus, pour tout $(x, y)\in X\times X$, on a d’une part $f(x, y) =\langle \widetilde{g}(x)|\widetilde{g}(y)\rangle$ et d’autre part

$$
\|\widetilde{g}(x)-\widetilde{g}(y)\|^2=f(x, x) +f(y, y)-f(x, y)-f(y, x)
$$

ce qui implique que $\widetilde{g}$ est continue puisque $f$ est continue.

Soient E l’espace hilbertien séparé-complété de $\widetilde{E}$ (EVT, V, p. 8, cor. de la prop. 4) et $g: X\rightarrow E$ la composition de $\widetilde{g}$ et de l’application canonique $\widetilde{E}\rightarrow E$. Alors l’application $g$ est continue, son image est totale dans E, et on a $f(x, y) =\langle g(x)|g(y)\rangle$ pour tout $(x, y)\in X\times X$.

La méthode employée pour démontrer que (ii) implique (iii) est appelée la construction de Gelfand–Naimark–Segal.

#### Définition 1 {#ts-v-s3-def-1 .statement tag=03BY}

On dit qu’une fonction $f\in \mathscr{C}(X\times X)$ est un noyau universellement positif sur X si elle vérifie les conditions équivalentes du théorème 1.

Si $f$ est un noyau universellement positif sur X, un couple $(E, g)$ vérifiant la condition (iv) de loc. cit. est appelé une réalisation hilbertienne de $f$; si la condition (iii) est satisfaite, on dit que c’est une réalisation hilbertienne cyclique.

On note Noy$_+(X)$ l’ensemble des noyaux universellement positifs sur X.

Soient $X'$ un espace topologique séparé et $h: X\rightarrow X'$ une application continue. L’application $f\mapsto f\circ (h, h)$ de $\mathscr{C}(X'\times X')$ dans $\mathscr{C}(X\times X)$ induit par passage aux sous-espaces une application Noy$_+(X')\rightarrow$ Noy$_+(X)$.

#### Proposition 1 {#ts-v-s3-prop-1 .statement tag=03BZ}

Soit $f$ un noyau universellement positif sur X. Soient $(E_1, g_1)$ et $(E_2, g_2)$ des réalisations hilbertiennes de $f$. On suppose que $(E_1, g_1)$ est une réalisation hilbertienne cyclique. Il existe alors une unique application linéaire continue $u: E_1\rightarrow E_2$ telle que $g_2=u\circ g_1$. Cette application est isométrique. Si $(E_2, g_2)$ est également cyclique, alors $u$ est un isomorphisme.

L’unicité de $u$ résulte du fait que l’image de $g_1$ est totale dans $E_1$. Soit $F =\mathbf{C}^{(X)}$ et soit $(e_x)_{x\in X}$ la base canonique de F. Pour $j= 1$ et $j= 2$, notons $u_j$ l’application linéaire de F dans $E_j$ déterminée par $u_j(e_x) =g_j(x)$, et notons $F_j$ son image ; l’espace $F_1$ est dense dans $E_1$.

Soit $t=\sum t_xe_x$ un élément de F. On a

$$
\|u_1(t)\|^2=\sum_{x,y}\overline{t}_xt_y\langle g_1(x)|g_1(y)\rangle =\sum_{x,y}\overline{t}_xt_yf(x, y)
$$

$$
=\sum_{x,y}\overline{t}_xt_y\langle g_2(x)|g_2(y)\rangle =\|u_2(t)\|^2
$$

Par conséquent, il existe une application linéaire isométrique $v$ de $F_1$ dans $F_2$ telle que $u_2=v\circ u_1$, et en particulier $g_2(x) =v(g_1(x))$ pour tout $x\in X$. Puisque l’image de $g_1$ est totale dans $E_1$, cette application se prolonge en une application linéaire isométrique $u$ de $E_1$ dans $E_2$ telle que $g_2=u\circ g_1$.

D’après le lemme 8 de I, p. 107, l’image de $u$ est fermée dans $E_2$. Si $(E_2, g_2)$ est une réalisation hilbertienne cyclique, l’image de $u$ est également dense dans $E_2$ et $u$ est donc un isomorphisme.

#### Proposition 2 {#ts-v-s3-prop-2 .statement tag=03C0}

L’ensemble Noy$_+(X)$ est un cône auto-adjoint dans l’espace $\mathscr{C}(X\times X)$; il est stable par produit et il est fermé lorsque l’on munit $\mathscr{C}(X\times X)$ de la topologie de la convergence simple.

nombre réelIl est élémentaire que si$t\geqslant 0$, et que $\frac{f}{f}\in \in$ NoyNoy$_{++}(X)$.(X), alors $tf\in$ Noy$_+(X)$ pour tout

Si $(E_1, g_1)$ et $(E_2, g_2)$ sont des réalisations hilbertiennes de noyaux universellement positifs $f_1$ et $f_2$ sur X, alors le couple $(E_1\oplus E_2, g_1+g_2)$ (resp. le couple $(E_1\widehat{\otimes}_2E_2, g_1\otimes g_2))$ est une réalisation hilbertienne de $f_1+f_2$ (resp. de $f_1f_2)$; ce sont donc des noyaux universellement positifs.

La caractérisation (ii) de Noy$_+(X)$ (th. 1) implique que cet ensemble est fermé dans $\mathscr{C}(X\times X)$ muni de la topologie de la convergence simple.

### 2. Complément sur le calcul fonctionnel holomorphe

Pour toute partie X de $\mathbf{C}$, on note $X^*$ l’image de X par la conjugaison complexe. Soient U une partie ouverte de $\mathbf{C}$ et $g: U\rightarrow \mathbf{C}$ une fonction holomorphe. La fonction $f^*:z\mapsto g(\overline{z})$ est alors définie et holomorphe sur $U^*$. L’application $f\mapsto f^*$ est une bijection continue de $\mathscr{O}(U)$ dans $\mathscr{O}(U^*)$ telle que $(f_1f_2)^*=f_1^*f_2^*$ et $(f_1+f_2)^*=f_1^*+f_2^*$ pour $f_1$ et $f_2$ dans $\mathscr{O}(U)$.

Soit C une partie compacte de $\mathbf{C}$. Les applications $f\mapsto f^*$ de $\mathscr{O}(U)$ dans $\mathscr{O}(U^*)$ pour U parcourant les parties ouvertes de $\mathbf{C}$ contenant C induisent une bijection continue de l’espace $\mathscr{O}(C)$ dans $\mathscr{O}(C^*)$(I, p. 49, n$^o1$), qui est également notée $f\mapsto f^*$ et qui vérifie $(f_1f_2)^*=f_1^*f_2^*$ et $(f_1+f_2)^*=f_1^*+f_2^*$ pour $f_1$ et $f_2$ dans $\mathscr{O}(C)$.

#### Proposition 3 {#ts-v-s3-prop-3 .statement tag=03C1}

Soit A une algèbre de Banach unifère involutive. Soit $a\in A$. Le spectre de $a^*$ est l’image Sp$_A(a)^*$ de Sp$_A(a)$ par la conjugaison complexe. Pour tout $f\in \mathscr{O}$(Sp$_A(a))$, on a $f(a)^*=f^*(a^*)$.

La première assertion résulte de I, p. 97. D’après ce qui précède, l’application $\varphi$ de $\mathscr{O}$(Sp$_A(a))$ dans A définie par $f\mapsto (f^*(a^*))^*$ est un morphisme unifère continu de $\mathscr{O}$(Sp$_A(a))$ dans A tel que l’image du germe au voisinage de Sp$_A(a)$ de la fonction identique de $\mathbf{C}$ est égal à $a$. Par conséquent, $\varphi$ est l’application $f\mapsto f(a)$ du calcul fonctionnel holomorphe (I, p. 74, th. 5).

#### Lemme 1 {#ts-v-s3-lem-1 .statement tag=03C2}

Soit D le disque unité ouvert dans $\mathbf{C}$. Il existe une unique fonction holomorphe $f$ définie sur D telle que $f(z)^2= 1-z$ pour tout $z\in D$ et $f(0) = 1$. On a $f^*=f$.

Le rayon de convergence de la série entière

$$
^{+\infty}(1/2)_n
$$

$$
\sum(-z)
$$

$$
n
$$

$n=0$

est à 1 et sa somme $f$ définit une fonction holomorphe sur D (VAR,

$$
\surd
$$

R1, p. 27, 3.2.9) prenant la valeur 1 en 0. Elle vérifie $f(x) =1-x$ pour tout $x\in D\cap \mathbf{R}$ (FVR, III, p. 19), donc $f(z)^2= 1-z$ pour $z\in D$ puisque la différence $f(z)^2-(1-z)$ est une fonction holomorphe dont toutes les dérivées successives s’annulent en 0 (VAR, R1, p. 27, 3.2.5). Par définition, on vérifie que $f^*=f$.

Soit $g$ une fonction holomorphe sur D telle que $g(z)^2= 1-z$ pour tout $z\in D$ et telle que $g(0) = 1$. La fonction $g$ ne s’annule pas et la fonction continue $f /g$ sur D est à valeurs dans $\{-1,1\}$; puisque D est connexe et que $f(0) =g$(0), on a $f=g$.

### 3. Formes linéaires positives

#### Définition 2 {#ts-v-s3-def-2 .statement tag=03C3}

Soit A une algèbre involutive. Une forme linéaire $\lambda$ sur A est dite positive si $\lambda (a^*a)\in \mathbf{R}_+$ pour tout $a\in A$.

Si A est une algèbre de Banach involutive, on note $A'_+$ l’ensemble des formes linéaires positives continues sur A.

Soit A une algèbre de Banach involutive. L’ensemble $A'_+$ est un cône convexe pointé dans l’espace vectoriel réel des formes $\mathbf{C}$-linéaires sur A.

#### Lemme 2 {#ts-v-s3-lem-2 .statement tag=03C4}

Soient A une algèbre de Banach involutive et $\lambda$ une forme linéaire positive sur A.

a) Pour tous $a$ et $b$ dans A, on a $\lambda (a^*b) =\overline{\lambda(b^*a)}$ et

$$
|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)
$$

b) Si A est unifère, alors la forme linéaire $\lambda$ est continue et sa norme est égale à $\lambda (1)$.

L’application $(a, b)\mapsto \lambda (a^*b)$ est une forme hermitienne positive sur A ; elle vérifie donc $\lambda (a^*b) =\lambda (b^*a)$ et $|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)$ pour tous $a$ et $b$ dans A (EVT, V, p. 2, remarque et p. 3, prop. 2).

Démontrons b). Soit $a\in A$ un élément hermitien de norme $<1$. Le rayon spectral de $a$ est inférieur à $\|a\|$, donc le spectre de $a$ est contenu dans le disque unité ouvert D de $\mathbf{C}$ (th. 1 de I, p. 24). Soit $f$ une fonction holomorphe sur D telle que $f(z)^2= 1-z$ pour tout $z\in D$ (lemme 1 de V, p. 435). Appliquons le calcul fonctionnel holomorphe à l’élément $a$ et à la fonction $f$. L’élément $b=f(a)$ vérifie $b^2= 1-a($I, p. 74, th. 5). D’après la prop. 3 de V, p. 435, on a de plus $f(a)^*=f^*(a^*) =f(a)$, donc $b$ est hermitien. Il vient alors $\lambda (1-a) =\lambda (b^*b)\geqslant 0$, d’où $\lambda (a)\leqslant \lambda (1)$.

Soit maintenant $b\in A$ de norme $<1$. L’élément $b^*b$ est hermitien et $\|b^*b\|<1$, donc en appliquant a) avec $a= 1$, on trouve

$$
|\lambda (b)|^2\leqslant \lambda (1)\lambda (b^*b)\leqslant \lambda (1)^2
$$

avec égalité si $b= 1$. La forme linéaire $\lambda$ est donc continue, et sa norme est égale à $\lambda (1)$. L’assertion b) est démontrée.

#### Exemple {#ts-v-s3-n3-exa-1 .statement tag=03C5}

Soit X un espace topologique compact et soit A l’algèbre stellaire $\mathscr{C}(X)$. Les formes linéaires positives sur A s’identifient aux mesures positives sur X (INT, III, p. 52, § 1, n$^o6$, th. 1).

#### Lemme 3 {#ts-v-s3-lem-3 .statement tag=03C6}

Soit A une algèbre de Banach unifère involutive admettant une unité approchée (I, p. 120, déf. 7). Soit $\lambda$ une forme linéaire positive continue sur A.

a) Pour tout $a$ dans A, on a $\lambda (a^*) =\overline{\lambda(a)}$ et $|\lambda (a)|^2\leqslant \|\lambda \|\lambda (a^*a)$;

b) Soit $\widetilde{A}$ l’algèbre involutive obtenue à partir de A par adjonction d’un élément unité et soit $e$ son élément unité. Il existe une forme linéaire positive continue $\widetilde{\lambda}$ sur $\widetilde{A}$ qui prolonge $\lambda$ et telle que $\widetilde{\lambda}(e) =\|\lambda \|$;

c) Pour tous $a$ et $b$ dans A, on a $|\lambda (b^*ab)|\leqslant \|a\|\lambda (b^*b)$.

Démontrons a). Soit $\mathfrak{F}$ une unité approchée de A. Soit $a\in A$. En utilisant le lemme 2, a) et la définition d’une unité approchée, on trouve

$\lambda (a^*) =$ lim$_{f,\mathfrak{F}}\lambda (f a^*) =$ lim$_{f,\mathfrak{F}}\lambda (af^*) =$ lim$_{f,\mathfrak{F}}\lambda ((f a^*)^*) =\overline{\lambda(a)}$,

d’où (loc. cit.)

$|\lambda (a)|^2=$ lim$_{f,\mathfrak{F}}|\lambda (f a)|^2\leqslant \lambda (a^*a)$ lim sup$_{f,\mathfrak{F}}\lambda (f f^*)\leqslant \|\lambda \|\lambda (a^*a)$,

puisque $\mathfrak{F}$ est un filtre sur la boule unité de A.

Pour démontrer b), on peut supposer que $\lambda$ n’est pas nulle, puis que $\|\lambda \|= 1$. Pour $a\in A$ et $z\in \mathbf{C}$, posons $\widetilde{\lambda}(a+z\cdot e) =\lambda (a) +z$. L’application $\widetilde{\lambda}$ est une forme linéaire continue sur $\widetilde{A}$ qui prolonge $\lambda$ et vérifie $\widetilde{\lambda}(e) = 1$. Elle est positive : pour tous $a\in A$ et $z\in \mathbf{C}$, d’après a), on calcule

$$
\widetilde{\lambda}((a+z\cdot e)^*(a+z\cdot e)) =\lambda (a^*a) +z\lambda (a) +z\lambda (a^*) +|z|^2
$$

$$
=|z+\lambda (a)|^2+\lambda (a^*a)- |\lambda (a)|^2\geqslant 0
$$

Finalement, soit $b$ un élément de A. L’application $a\mapsto \widetilde{\lambda}(b^*ab)$ est une forme linéaire positive sur l’algèbre de Banach involutive unifère $\widetilde{A}$. Elle est donc continue de norme égale à sa valeur en $e$ (lemme 2, b)), qui est égale à $\lambda (b^*b)$, d’où l’assertion c).

#### Proposition 4 {#ts-v-s3-prop-4 .statement tag=03C7}

Soit A une algèbre de Banach involutive.

a) Pour tout espace hilbertien E, tout morphisme d’algèbres involutives $\varphi : A\rightarrow \mathscr{L}(E)$ et tout vecteur $x\in E$, la forme linéaire définie sur A par $\lambda (a) =\langle x|\varphi (a)x\rangle$ est une forme linéaire positive continue ;

b) Soit $\lambda \in A'_+$. L’application $f$ de $A\times A$ dans $\mathbf{C}$ définie par $f(a, b) =$ $\lambda (a^*b)$ pour tout $(a, b)\in A\times A$ est un noyau universellement positif sur A.

Démontrons a). Pour tout $a\in A$, on a

$$
\lambda (a^*a) =\langle x|\varphi (a^*a)x\rangle =\|\varphi (a)x\|^2\geqslant 0
$$

donc $\lambda$ est une forme linéaire positive sur A ; elle est continue puisque $\varphi$ est continu (prop. 2 de I, p. 104).

Démontrons b). La fonction $f$ est continue. Pour tout $n\in \mathbf{N}$, toute famille $(a_i)_{0\leqslant i\leqslant n}$ dans A et toute famille $(t_i)_{0\leqslant i\leqslant n}$ de nombres complexes, on a

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(a_i, a_j) =\lambda ((\sum_{i=0}^nt_ia_i)^*(\sum_{j=0}^nt_ja_j))\geqslant 0
$$

d’où le résultat (déf. 1 de V, p. 433).

#### Définition 3 {#ts-v-s3-def-3 .statement tag=03C8}

Soit A une algèbre de Banach involutive. Soit $\lambda \in A'_+$ une forme linéaire positive continue sur A. On appelle réalisation hilbertienne de $\lambda$ un triplet $(E, x, \varphi )$ formé d’un espace hilbertien E, d’un élément $x$ de E et d’un morphisme d’algèbres involutives $\varphi$ de A dans $\mathscr{L}(E)$, tels que $\lambda (b^*a) =\langle \varphi (b)x|\varphi (a)x\rangle$ pour tout $(a, b)\in A^2$.

Si l’ensemble des éléments $\varphi (a)x$ pour $a\in A$ est total dans E, on dit que $(E, x, \varphi )$ est une réalisation hilbertienne cyclique de $\lambda$.

#### Proposition 5 {#ts-v-s3-prop-5 .statement tag=03C9}

Soit A une algèbre de Banach involutive admettant une unité approchée. Toute forme linéaire positive continue sur A admet une réalisation hilbertienne cyclique $(E, x, \varphi )$. Si A est unifère, alors il existe une telle réalisation où le morphisme $\varphi$ est unifère.

On peut supposer que A est une algèbre unifère (lemme 3, b)).

Soit $\lambda$ une forme linéaire positive continue sur A. Soit $(E, g)$ une réalisation hilbertienne cyclique du noyau universellement positif $f$ sur A défini par $f(a, b) =\lambda (a^*b)$ (prop. 4 et th. 1). L’application $g$ est continue, son image est totale dans E, et on a $\lambda (a^*b) =\langle g(a)|g(b)\rangle$ pour tout $(a, b)\in A^2$. Posons $x=g(1)\in E$.

L’application $g$ de A dans E est linéaire : en effet, pour $(a, b, c)\in A^3$ et $(s, t)\in \mathbf{C}^2$, il vient

$$
\langle g(c)|g(sa+tb)\rangle =\lambda (c^*(sa+tb))
$$

$$
=s\lambda (c^*a) +t\lambda (c^*b) =\langle g(c)|sg(a) +tg(b)\rangle
$$

d’où l’assertion puisque l’image de $g$ est totale dans E.

En particulier, l’image F de $g$ est un sous-espace vectoriel dense de E. Le noyau de $g$ est un idéal à gauche de A : si $g(b) = 0$, alors pour tous $a$ et $c$ dans A, il vient

$$
\langle g(ab)|g(c)\rangle =\lambda ((ab)^*c) =\lambda (b^*(a^*c)) =\langle g(b)|g(a^*c)\rangle = 0
$$

donc $g(ab) = 0$ puisque F est dense dans E.

Soit $a\in A$. Puisque le noyau de $g$ est un idéal à gauche de A, il existe une application linéaire $\widetilde{\varphi}(a) : F\rightarrow F$ telle que $\widetilde{\varphi}(a)(g(b)) =g(ab)$ pour tout $b\in A$. De plus, pour tout $b\in A$, il vient

$$
\|\widetilde{\varphi}(a)(g(b))\|^2=\|g(ab)\|^2=\lambda (b^*a^*ab)\leqslant \|a^*a\|\lambda (b^*b)\leqslant \|a\|^2\|g(b)\|^2
$$

(lemme 3, c)), donc $\widetilde{\varphi}(a)$ est continue et de norme $\leqslant \|a\|$. Par conséquent, il existe un unique endomorphisme $\varphi (a)\in \mathscr{L}(E)$ qui induit $\widetilde{\varphi}(a)$ par passage aux sous-espaces.

Soient $a$ et $b$ dans A. On a

$$
(\varphi (a)\circ \varphi (b))(g(c)) =g(abc) =\varphi (ab)(g(c))
$$

pour tout $c$ dans A, donc $\varphi (ab) =\varphi (a)\circ \varphi (b)$ puisque F est dense dans E.

L’application $\varphi$ de A dans $\mathscr{L}(E)$ est linéaire : en effet, pour tout $(a, b)\in A^2$ et tout $(s, t)\in \mathbf{C}^2$, on a

$$
\varphi (sa+tb)(g(c)) =g((sa+tb)c) = (s\varphi (a) +t\varphi (b))g(c)
$$

pour tout $c\in A$, d’où $\varphi (sa+tb) =s\varphi (a) +t\varphi (b)$ puisque F est dense dans E. Comme $\|\varphi (b)\|\leqslant \|b\|$ pour tout $b\in A$, l’application $\varphi$ est continue. On a également $\varphi (1) = 1_E$ puisque $\varphi (1)(g(a)) =g(a)$ pour tout $a\in A$ et que F est dense dans E.

Enfin, soient $a,b,c$ dans A. On a

$$
\langle g(c)|\varphi (a^*)(g(b))\rangle =\langle g(c)|g(a^*b)\rangle =\lambda (c^*a^*b)
$$

$$
=\langle g(ac)|g(b)\rangle =\langle \varphi (a)(g(c))|g(b)\rangle
$$

d’où $\varphi (a^*) =\varphi (a)^*$ puisque F est dense dans E.

En conclusion, l’application $\varphi$ est un morphisme continu d’algèbres involutives de A dans $\mathscr{L}(E)$ et $g(a) =\varphi (a)x$ pour tout $a\in A$; par conséquent, le triplet $(E, x, \varphi )$ est une réalisation hilbertienne cyclique de $\lambda$.

#### Proposition 6 {#ts-v-s3-prop-6 .statement tag=03CA}

Soit A une algèbre de Banach involutive et soit $\lambda$ une forme linéaire positive continue sur A. Soient $(E_1, x_1, \varphi_1)$ et $(E_2, x_2, \varphi_2)$ des réalisations hilbertiennes de $\lambda$. On suppose que $(E_1, x_1, \varphi_1)$ est une réalisation hilbertienne cyclique.

a) Il existe une unique application linéaire continue $u$ de $E_1$ dans $E_2$ qui est un morphisme de représentations de $\varphi_1$ dans $\varphi_2($I, p. 11) et qui vérifie $u(\varphi_1(a)x_1) =\varphi_2(a)x_2$ pour tout $a\in A$;

b) L’application linéaire $u$ est isométrique ;

c) Si $(E_2, x_2, \varphi_2)$ est cyclique, alors $u$ est un isomorphisme ;

d) Si $(E_2, x_2, \varphi_2)$ est cyclique et si A est unifère, alors $u(x_1) =x_2$.

Pour $j\in  \{1,2\}$, définissons $\gamma_j: A\rightarrow E_j$ par $\gamma_j(a) =\varphi_j(a)x_j$ pour tout $a\in A$. Par définition, les couples $(E_j, \gamma_j)$ sont des réalisations hilbertiennes du noyau universellement positif $f$ sur A défini par $(a, b)\mapsto \lambda (a^*b)$. La réalisation hilbertienne $(E_1, \gamma_1)$ est cyclique ; d’après la prop. 1 de V, p. 434, il existe donc une unique application linéaire continue $u: E_1\rightarrow E_2$ telle que $\gamma_2=u\circ \gamma_1$, et celle-ci est isométrique. De plus, si $(E_2, x_2, \varphi_2)$ est également cyclique, alors $u$ est un isomorphisme. Pour démontrer a), b) et c), il suffit de démontrer que $u$ est un morphisme de représentations de $\varphi_1$ dans $\varphi_2$.

Soit $a\in A$. Pour tout $b\in A$, on a

$$
(u\circ \varphi_1(a))(\gamma_1(b)) = (u\circ \varphi_1(ab))x_1= (u\circ \gamma_1)(ab)
$$

$$
=\gamma_2(ab) =\varphi_2(a)(\gamma_2(b)) =\varphi_2(a)(u(\gamma_1(b)))
$$

donc les applications linéaires continues $u\circ \varphi_1(a)$ et $\varphi_2(a)\circ u$ coïncident sur le sous-espace de $E_1$ engendré par l’image de $\gamma_1$; ce sous-espace est dense dans $E_1$ par hypothèse, d’où $u\circ \varphi_1(a) =\varphi_2(a)\circ u$.

Démontrons enfin d). Supposons donc que A est unifère et que $(E_2, x_2, \varphi_2)$ est cyclique. Il existe une réalisation hilbertienne cyclique $(E_3, x_3, \varphi_3)$ de $\lambda$ telle que $\varphi_3$ est un morphisme unifère (prop. 5). Soit $j\in  \{1,2\}$. En appliquant ce qui précède à $(E_j, x_j, \varphi_j)$ et $(E_3, x_3, \varphi_3)$, on voit qu’il existe un isomorphisme isométrique $\widetilde{u}_j$ de $E_j$ dans $E_3$ tel que $\widetilde{u}_j\circ \varphi_j(a) =\varphi_3(a)\circ \widetilde{u}_j$ pour tout $a\in A$. En prenant $a= 1_A$, on voit que $\varphi_j$ est unifère. On a alors $x_2=\varphi_2(1_A)x_2=u(\varphi_1(1_A)x_1) =u(x_1)$.

#### Remarque {#ts-v-s3-n3-rem-1 .statement tag=03CB}

Conservons les notations de la proposition. Il est possible que $u(x_1)$ soit différent de $x_2$ (exercice 3, b) de V, p. 493). Cependant, le triplet $(E_2, u(x_1), \varphi_2)$ est aussi une représentation hilbertienne de $\lambda$.

### 4. Représentations des algèbres stellaires

Soit A une algèbre stellaire. Notons $A_+$ le cône convexe fermé des éléments positifs de A (déf. 6 de I, p. 115). Une forme linéaire $\lambda$ sur A est positive si et seulement si $\lambda (A_+)\subset \mathbf{R}_+($I, p. 118, th. 2).

#### Proposition 7 {#ts-v-s3-prop-7 .statement tag=03CC}

Soit A une algèbre stellaire. Toute forme linéaire positive $\lambda$ sur A est continue.

Démontrons d’abord que $\lambda$ est bornée sur l’intersection de $A_+$ et de la boule unité de A. Supposons que ce ne soit pas le cas. Il existe alors une suite $(x_n)_{n\geqslant 1}$ dans $A_+$ telle que $\|x_n\|\leqslant 1$ et $\lambda (x_n)\geqslant n$ pour tout entier $n\geqslant 1$. La série de terme général $n^{-2}x_n$ converge vers un élément $x$ de A (cf. TG, IV, p. 33, exemple 3). Pour tout entier $N\geqslant 1$, comme

$+\infty$

$\sum\frac{1}{n^2}x_n\in A_+$,

$n=N+1$

(I, p. 116, prop. 14) il vient

N N $+\infty$

$\sum\frac{1}{n}\leqslant \sum\frac{1}{n^2}\lambda (x_n) =\lambda (x)-\lambda (\sum\frac{1}{n^2}x_n)\leqslant \lambda (x)$,

$n=1n=1n=N+1$

ce qui est absurde (TG, IV, p. 33, exemple 4).

Comme tout élément de la boule unité de A est combinaison linéaire avec des coefficients bornés par 1 d’au plus quatre éléments positifs de A de norme $\leqslant 1$(I, p. 96, lemme 2 et formule (4) de I, p. 117), on conclut que $\lambda$ est continue.

Il existe des algèbres de Banach involutives qui admettent des formes linéaires positives qui ne sont pas continues (exercice 3, a) de V, p. 493).

#### Proposition 8 {#ts-v-s3-prop-8 .statement tag=03CD}

Soient A une algèbre stellaire et $a$ un élément non nul de A. Il existe une forme linéaire positive $\lambda \in A'_+$ telle que $\lambda (a^*a)>0$.

Considérons l’espace de Banach réel $A_h$ des éléments hermitiens de A. L’ensemble $A_+$ est un cône convexe fermé pointé saillant dans $A_h$ (prop. 14 de I, p. 116). L’élément $a^*a$ est positif (th. 2 de I, p. 118) et non nul, donc l’élément hermitien $-a^*a$ n’est donc pas positif. D’après EVT, II, p. 42, cor. 5, il existe une forme linéaire réelle continue $\lambda \in A'_h$ telle que $\lambda (-a^*a)<0$ et $\lambda (A_+)\subset \mathbf{R}_+$. La forme linéaire $\lambda$ s’étend en une forme $\mathbf{C}$-linéaire hermitienne sur A (cf. I, p. 98), qui est positive et qui possède la propriété demandée.

#### Théorème 2 (Gelfand–Naimark) {#ts-v-s3-thm-2 .statement tag=03CE}

Soit A une algèbre stellaire. Il existe un espace hilbertien E et un morphisme isométrique d’algèbres involutives $\varphi$ de A dans $\mathscr{L}(E)$. Si A est unifère, il existe un tel morphisme unifère.

Pour tout $b\in A-\{0\}$, soit $\lambda_b$ une forme linéaire positive continue sur A telle que $\lambda_b(b^*b)>0$ (prop. 8). Puisque A admet une unité approchée (I, p. 121, prop. 18), il existe une réalisation hilbertienne $(E_b, x_b, \varphi_b)$ de $\lambda_b$ (prop. 5). Si A est unifère, on peut supposer que $\varphi_b$ est unifère (loc. cit.). On a $\|\varphi_b(b)\|^2=\lambda_b(b^*b)\not = 0$.

Soit E la somme hilbertienne externe des espaces $E_b$ pour $b$ appartenant à A $-\{0\}$. Pour tout $a\in A$, notons $\varphi (a)\in \mathscr{L}(E)$ l’unique application linéaire continue dont la restriction à $E_b$ coïncide avec $\varphi_b(a)$ pour tout $b\in A-\{0\}$. L’application $a\mapsto \varphi (a)$ est un morphisme d’algèbres involutives ; il est injectif, donc isométrique (prop. 9 de I, p. 112), et vérifie $\varphi (1) = 1_E$ si A est unifère. Cela conclut la preuve.

*La catégorie dont les objets sont les algèbres stellaires et les morphismes les morphismes d’algèbres involutives est donc équivalente à la catégorie dont les objets sont les sous-algèbres fermées involutives des algèbres d’endomorphismes des espaces hilbertiens, et les morphismes sont les morphismes d’algèbres involutives.*

### 5. Fonctions de type positif sur un groupe topologique

Dans ce numéro, G est un groupe topologique dont on note $e$ l’élément unité. Les espaces hilbertiens considérés sont complexes.

#### Définition 4 {#ts-v-s3-def-4 .statement tag=03CF}

Une fonction continue $\varphi \in \mathscr{C}(G)$ est dite de type positif sur G si la fonction $f$ définie par $f(g, h) =\varphi (g^{-1}h)$ sur $G\times G$ est un noyau universellement positif sur G.

On note Pos(G) l’ensemble des fonctions de type positif sur G et on note Pos$_1(G) ($resp. Pos$_{\leqslant 1}(G))$ le sous-ensemble des $\varphi \in$ Pos(G) telles que $\varphi (e) = 1 ($resp. telles que $\varphi (e)\leqslant 1)$.

#### Exemple {#ts-v-s3-n5-exa-1 .statement tag=03CG}

Soient $\varrho$ une représentation unitaire de G dans un espace hilbertien E et $x\in E$. Soit $\varphi$ le coefficient matriciel diagonal défini par $\varphi (g) =\langle x|\varrho (g)x\rangle$ pour tout $g\in G$; la fonction $\varphi$ est continue. Il vient

$$
\varphi (g^{-1}h) =\langle x|\varrho (g)^*\varrho (h)x\rangle =\langle \varrho (g)x|\varrho (h)x\rangle
$$

pour tout $(g, h)\in G\times G$. Par conséquent $\varphi \in$ Pos(G) (théorème 1 de V, p. 432, (iv)). On a $\varphi \in$ Pos$_1(G)$ si et seulement si $\|x\|= 1$.

#### Définition 5 {#ts-v-s3-def-5 .statement tag=03CH}

Soit $\varphi$ une fonction de type positif sur G. Une réalisation hilbertienne de $\varphi$ est un couple $(\varrho , x)$ où $\varrho$ est une représentation unitaire de G dans un espace hilbertien E et $x\in E$, tel que $\varphi (g) =\langle x|\varrho (g)x\rangle$ pour tout $g\in G$.

Si $x$ est un vecteur cyclique de $\varrho$, on dit que c’est une réalisation hilbertienne cyclique de $\varphi$.

#### Proposition 9 {#ts-v-s3-prop-9 .statement tag=03CI}

Soit $\varphi \in \mathscr{C}(G)$. Les conditions suivantes sont équivalentes :

(i) La fonction $\varphi$ est de type positif sur G ;

(ii) Il existe une réalisation hilbertienne cyclique de $\varphi$;

(iii) Il existe une réalisation hilbertienne de $\varphi$.

La condition (ii) implique la condition (iii), et la condition (iii) implique (i) d’après l’exemple ci-dessus.

Démontrons finalement que (i) implique (ii). Soit $(E, \gamma )$ une réa-lisation hilbertienne cyclique du noyau universellement positif défini par $f(g, h) =\varphi (g^{-1}h)$ pour $(g, h)\in G\times G$. Soit $k\in G$. La fonction continue $\gamma_k:g\mapsto \gamma (kg)$ sur G vérifie

$$
\langle \gamma_k(g)|\gamma_k(h)\rangle =\langle \gamma (kg)|\gamma (kh)\rangle =f(kg, kh) =\varphi ((kh)^{-1}kg) =f(g, h)
$$

pour tout $(g, h)\in G\times G$, donc $(E, \gamma_k)$ est une réalisation hilbertienne de $f$. D’après la prop. 1 de V, p. 434, il existe un unique élément unitaire $\varrho (k)$ dans $\mathscr{L}(E)$ tel que $\gamma_k=\varrho (k)\circ \gamma$. Pour tout $g\in G$, et tout $(k_1, k_2)\in G\times G$, il vient

$$
\varrho (k_1k_2)(\gamma (g)) =\gamma (k_1k_2g) =\varrho (k_1)(\varrho (k_2)(\gamma (g)))
$$

d’où $\varrho (k_1k_2) =\varrho (k_1)\varrho (k_2)$ puisque l’image de $\gamma$ est une partie totale de E.

Soit $k\in G$. Pour tout $g\in G$, on a $\varrho (g)(\gamma (k)) =\gamma (gk)$, et l’application de G dans E définie par $g\mapsto \varrho (g)(\gamma (k))$ est donc continue. Puisque l’endomorphisme $\varrho (g)$ est unitaire, on en déduit que $\varrho$ est une représentation unitaire de G dans E (lemme 4 de V, p. 380). Posons alors $x=\gamma (e)$. L’ensemble des vecteurs $\varrho (g)x=\varrho (g)(\gamma (e)) =\gamma (g)$ pour $g$ parcourant G est total dans E, donc $x$ est un vecteur cyclique de $\varrho$. Comme

$$
\langle x|\varrho (g)x\rangle =f(e, g) =\varphi (g)
$$

pour tout $g\in G$, le couple $(\varrho , x)$ est une réalisation hilbertienne cyclique de $\varphi$.

#### Proposition 10 {#ts-v-s3-prop-10 .statement tag=03CJ}

Soit $\varphi$ une fonction de type positif sur G et soient $(\varrho_1, x_1)$ et $(\varrho_2, x_2)$ des réalisations hilbertiennes de $\varphi$, la représentation hilbertienne $(\varrho_1, x_1)$ étant cyclique. Il existe un unique G-morphisme isométrique $u$ de $\varrho_1$ dans $\varrho_2$ tel que $u(x_1) =x_2$. Si $(\varrho_2, x_2)$ est aussi cyclique, alors $u$ est un isomorphisme.

Pour $1\leqslant j\leqslant 2$, notons $E_j$ l’espace de $\varrho_j$ et $\gamma_j$ la fonction sur G définie par $\gamma_j(g) =\varrho_j(g)x_j$ pour tout $g\in G$. Les couples $(E_1, \gamma_1)$ et $(E_2, \gamma_2)$ sont des réalisations hilbertiennes de la fonction de type positif $(g, h)\mapsto \varphi (g^{-1}h)$, et $(E_1, \gamma_1)$ est une réalisation hilbertienne cyclique. D’après la prop. 1 de V, p. 434, il existe une unique application linéaire isométrique $u: E_1\rightarrow E_2$ telle que $\gamma_2=u\circ \gamma_1$. En particulier, on a $x_2=\gamma_2(e) =u(\gamma_1(e)) =u(x_1)$. De plus, pour tous $g$ et $h$ dans G, on a

$$
\varrho_2(g)u(\gamma_1(h)) =\varrho_2(g)\gamma_2(h) =\gamma_2(gh) =u(\gamma_1(gh)) =u(\varrho_1(g)\gamma_1(h))
$$

et comme l’ensemble des éléments $\gamma_1(h)$ pour $h\in G$ est total dans $E_1$, cela signifie que $u$ est un G-morphisme. D’après loc. cit., c’est un isomorphisme isométrique si $(\varrho_2, x_2)$ est également cyclique.

#### Proposition 11 {#ts-v-s3-prop-11 .statement tag=03CK}

Soient $\varphi \in$ Pos$_1(G)$ et $(\varrho , x)$ une réalisation hilbertienne cyclique de $\varphi$. Alors $\varrho$ est une représentation irréductible de G si et seulement si $\varphi$ est un point extrémal (EVT, II, p. 57, déf. 1) de Pos$_1(G)$.

Soit E l’espace de $\varrho$. Supposons tout d’abord que $\varrho$ n’est pas irréductible. Soit F un sous-espace fermé de E stable par $\varrho$, non nul et différent de E. Écrivons $x=x_1+x_2$, où $x_1\in F$ et $x_2\in F^{\circ}$. On a alors $1 =\|x\|^2=\|x_1\|^2+\|x_2\|^2$. La sous-représentation de E engendrée par $x_1$ est contenue dans F, donc $x_1\not =x$ puisque $x$ est un vecteur cyclique de $\varrho$, d’où $x_2\not = 0$. De même on vérifie que $x_1\not = 0$.

Pour $j= 1$ et $j= 2$, notons $\varphi_j$ la fonction continue sur G telle que

$$
\varphi_j(g) =\frac{1}{\|x_j\|^2}\langle x_j|\varrho (g)x_j\rangle
$$

pour tout $g\in G$. On a $\varphi_j\in$ Pos$_1(G)$(V, p. 443, exemple). Comme $\varphi =\|x_1\|^2\varphi_1+\|x_2\|^2\varphi_2$, il suffit de vérifier que $\varphi_1\not =\varphi_2$ pour démontrer que $\varphi$ n’est pas un point extrémal de Pos$_1(G)$; il suffit pour cela de démontrer que $\varphi \not =\varphi_1$.

Raisonnons par l’absurde et supposons que $\varphi =\varphi_1$. Comme on a $\langle x_1|\varrho (g)x_2\rangle = 0$ pour tout $g\in G$, il viendrait

$$
\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x\rangle =\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x_1\rangle =\varphi_1(g) =\varphi (g) =\langle x|\varrho (g)x\rangle
$$

pour tout $g\in G$, d’où $\langle x_1|y\rangle =\langle \|x_1\|^2x|y\rangle$ pour tout élément $y$ du sous-espace vectoriel de E engendré par les éléments $\varrho (g)x$ pour $g\in G$, donc pour tout $y\in E$ puisque $x$ est un vecteur cyclique de $\varrho$. Cela impliquerait que $x_1=\|x_1\|^2x$ est aussi un vecteur cyclique de $\varrho$, ce qui est une contradiction, d’où l’assertion.

Supposons maintenant que $\varrho$ est irréductible et démontrons que $\varphi$ est un point extrémal de Pos$_1(G)$. Soient $\varphi_1\not =\varphi_2$ des éléments de Pos$_1(G)$ et $t_1,t_2\in [0,1]$ tels que $t_1+t_2= 1$ et $\varphi =t_1\varphi_1+t_2\varphi_2$. Pour $j\in  \{1,2\}$, notons $(\varrho_j, x_j)$ une réalisation hilbertienne cyclique de $\varphi_j$, et notons $E_j$ l’espace de $\varrho_j$. Soit $x_3=t^{1/2}_1x_1+t^{1/2}_2x_2$. Alors $(\varrho_1\oplus \varrho_2, x_3)$ est une réalisation hilbertienne de $\varphi$. Comme $(\varrho , x)$ est cyclique, il existe un G-morphisme isométrique $u: E\rightarrow E_1\oplus E_2$ tel que $u(x) =x_3$ (prop. 10).

Soit $j= 1$ ou $j= 2$. Puisque $\varrho$ est irréductible, il existe $\lambda_j\geqslant 0$ tel que le G-morphisme $u_j=$ pr$_j\circ u$ de E dans $E_j$ vérifie

$$
\langle u_j(y)|u_j(y')\rangle =\lambda_j\langle y|y'\rangle
$$

pour tous $y$ et $y'$ dans E (cor. 5 de V, p. 388, si $u_j\not = 0$, et on peut prendre $\lambda_j= 0$ sinon). Pour tout $g\in G$, il vient

$$
t_j\varphi_j(g) =\langle t^{1/2}_jx_j|\varrho_j(g)(t^{1/2}_jx_j)\rangle =\langle u_j(x)|\varrho_j(g)(u_j(x))\rangle
$$

$$
=\langle u_j(x)|u_j(\varrho (g)x)\rangle =\lambda_j\varphi (g)
$$

Comme $\varphi_j(e) =\varphi (e) = 1$, on en déduit que $\varphi_j=\varphi$ si $t_j\not = 0$. L’hypothèse $\varphi_1\not =\varphi_2$ implique donc que $t_1$ ou $t_2$ doit être nul, ce qui démontre que $\varphi$ est un point extrémal de Pos$_1(G)$.

#### Lemme 4 {#ts-v-s3-lem-4 .statement tag=03CL}

Soit $\varphi \in$ Pos(G). La fonction $\varphi$ est bornée sur G et on a $\|\varphi \|_{\infty}=\varphi (e)$. De plus, on a

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \surd\overline{2\varphi(e)(\varphi(e) -\mathscr{R}(\varphi(g)))} \tag{1}
$$

pour tout $(g, h)\in G\times G$.

Soit $(\varrho , x)$ une réalisation hilbertienne de $\varphi$. On a $\varphi (e) =\|x\|^2$. Pour tout $g\in G$, il vient donc $|\varphi (g)|=|\langle x|\varrho (g)x\rangle |\leqslant \varphi (e)$ d’après l’inégalité de Cauchy-Schwarz. Cela démontre la première assertion.

Pour tout $(g, h)\in G\times G$, on a

$$
\varphi (g^{-1}h)-\varphi (h) =\langle x|\varrho (g^{-1}h)x\rangle  - \langle x|\varrho (h)x\rangle =\langle \varrho (g)x-x|\varrho (h)x\rangle
$$

puisque $\varrho$ est unitaire, d’où

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \|\varrho (g)x-x\|\|\varrho (h)x\|\leqslant \varphi (e)^{1/2}\|\varrho (g)x-x\|
$$

On conclut en observant que

$$
\|\varrho (g)x-x\|^2= 2\|x\|^2-2\mathscr{R}(\langle x|\varrho (g)x\rangle ) = 2(\varphi (e)-\mathscr{R}(\varphi (g)))
$$

#### Remarque {#ts-v-s3-n5-rem-1 .statement tag=03CM}

Les ensembles Pos(G) (resp. Pos$_1(G)$ et Pos$_{\leqslant 1}(G))$ sont des parties convexes auto-adjointes de l’algèbre stellaire $\mathscr{C}_b(G)$. Ils sont fermés dans l’espace $\mathscr{C}_b(G)$ muni de la topologie de la convergence simple. L’ensemble Pos(G) est un cône convexe de sommet 0 dans l’espace de Banach réel $\mathscr{C}_b(G)$.

### 6. Dual unitaire d’un groupe localement compact

Soit G un groupe topologique localement compact. On munit G d’une mesure de Haar à gauche $\mu$. Pour $p\in [1,+\infty ]$, on note $\mathscr{L}^p(G)$ (resp. $L^p(G))$ l’espace $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (resp. l’espace $L^p_{\mathbf{C}}(G, \mu))$. On identifie l’espace $\mathscr{C}_b(G)$ à son image dans $L^{\infty}(G)$.

Notons Δ le module de G. Rappelons que $L^1(G)$ est une algèbre de Banach involutive dont l’involution est induite, par passage aux quotients, par l’application $f\mapsto f^*$ où $f^*(y) = \Delta^{-1}(y)f(y^{-1})$ pour tous $f\in \mathscr{L}^1(G)$ et $y\in G ($cf. I, p. 99, exemple 4). L’algèbre de Banach $L^1(G)$ admet une unité approchée d’après INT, VIII, p. 172, §4, n$^o7$, prop. 20.

Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. L’application $f\mapsto \varrho (f)$ est un morphisme continu d’algèbres involutives de $L^1(G)$ dans $\mathscr{L}(E)$ (lemme 1 de V, p. 401) ; c’est une représentation non dégénérée de $L^1(G)$ dans E (INT, VIII, p. 139, § 2, n$^o7$, prop. 10, (i)).

#### Proposition 12 {#ts-v-s3-prop-12 .statement tag=03CN}

Soient E un espace hilbertien complexe et $\widetilde{\pi}$ un morphisme d’algèbres involutives de $L^1(G)$ dans $\mathscr{L}(E)$. Si la représentation $\widetilde{\pi}$ est non dégénérée, alors il existe une unique représentation unitaire $\pi$ de G dans E telle que $\widetilde{\pi}(f) =\pi (f)$ pour tout $f\in L^1(G)$.

L’unicité résulte de INT, VIII, p. 139, § 2, n$^o7$, cor. 3 du lemme 4.

Démontrons l’existence de $\pi$. On a $\|\widetilde{\pi}\|\leqslant 1$ d’après la prop. 2 de I, p. 104. Soit F le sous-espace de E engendré par les vecteurs de la forme $\widetilde{\pi}(f)x$ pour $f$ dans $L^1(G)$ et $x$ dans E ; il est dense dans E puisque la représentation $\widetilde{\pi}$ est non dégénérée.

Pour tout voisinage compact V de $e$, soit $\varphi_V$ une fonction continue positive à support contenu dans V telle que $\int\varphi_V\mu= 1$. Soit $\mathfrak{B}$ une base du filtre des voisinages compacts de $e$.

Soient $g$ dans G et $f$ dans $L^1(G)$. On a $(\varphi_V*\varepsilon_g)*f\rightarrow \varepsilon_g*f$ dans $L^1(G)$ suivant le filtre des sections de $\mathfrak{B}$ (INT, VIII, p. 172, § 4, n$^o7$, prop. 20), donc $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ converge vers $\widetilde{\pi}(\varepsilon_g*f)$ dans $\mathscr{L}(E)$. Cela implique que $\widetilde{\pi}(\varphi_V*\varepsilon_g)$ converge simplement suivant le filtre des sections de $\mathfrak{B}$ vers une application linéaire $\pi (g)$ de F dans F ; celle-ci est continue d’après EVT, III, p. 26, cor. 3, puisque $\|\widetilde{\pi}(\varphi_V*\varepsilon_g)\|\leqslant 1$ pour tout voisinage compact V de $e$. Il existe donc un unique endomorphisme de E qui induit $\pi (g)$ par passage aux sous-espaces. On note encore $\pi (g)$ cet endomorphisme ; on a $\|\pi (g)\|\leqslant 1$.

Soit $f\in L^1(G)$. Puisque $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ converge vers $\widetilde{\pi}(\varepsilon_g*f)$, on a $\pi (g)\widetilde{\pi}(f) =\widetilde{\pi}(\varepsilon_g*f)$.

Pour $g=e$, cette relation montre que $\pi (e)$ est l’identité sur F, donc $\pi (e) = 1_E$. Soient $g_1$ et $g_2$ dans G. On a

$$
\pi (g_1)\pi (g_2)\widetilde{\pi}(f) =\pi (g_1)\widetilde{\pi}(\varepsilon_{g_2}*f) =\widetilde{\pi}(\varepsilon_{g_1g_2}*f) =\pi (g_1g_2)\widetilde{\pi}(f)
$$

d’où $\pi (g_1)\pi (g_2) =\pi (g_1g_2)$ sur F, et donc sur E. Cela démontre que l’application $g\mapsto \pi (g)$ est une représentation de G dans E. Comme $\|\pi (g)\|\leqslant$ 1 et $\|\pi (g)^{-1}\|$ = $\|\pi (g^{-1})\|\leqslant$ 1, les endomorphismes $\pi (g)$ de E sont isométriques, donc unitaires (EVT, V, p. 40, prop. 3).

Soient $f\in L^1(G)$ et $x\in E$. L’application $g\mapsto \varepsilon_g*f$ de G dans $L^1(G)$ est continue (INT, VIII, p. 136, § 2, n$^o5$ et p. 144, § 3, n$^o2$, formule (5)), et $\widetilde{\pi}$ est continue, donc l’application $g\mapsto \widetilde{\pi}(\varepsilon_g*f)x=\pi (g)\widetilde{\pi}(f)x$ est continue en $g=e$. Comme F est dense dans E, la représentation $\pi$ est unitaire (lemme 4 de V, p. 380).

Soient $f_1$ et $f_2$ dans $L^1(G)$. D’après INT, VIII, p. 127, §1, n$^o5$, prop. 7, on a la relation

$$
f_1*f_2=\int_Gf_1(g)(\varepsilon_g*f_2)d\mu(g)
$$

dans $L^1$(G), d’où

$$
\widetilde{\pi}(f_1)\widetilde{\pi}(f_2) =\widetilde{\pi}(f_1*f_2) =\int_Gf_1(g)\widetilde{\pi}(\varepsilon_g*f_2)d\mu(g)
$$

$$
=\int_Gf_1(g)\pi (g)\widetilde{\pi}(f_2)d\mu(g) =(\int_Gf_1(g)\pi (g)d\mu(g))\widetilde{\pi}(f_2)
$$

en utilisant INT, VI, p. 9, § 1, n$^o1$, prop. 1. Il en résulte que

$$
\widetilde{\pi}(f) =\int_Gf(g)\pi (g)d\mu(g) =\pi (f)
$$

pour tout $f\in L^1(G)$. La proposition est démontrée.

#### Proposition 13 {#ts-v-s3-prop-13 .statement tag=03CO}

Soit $\varphi \in L^{\infty}(G)$. Notons $\lambda_{\varphi}$ la forme linéaire continue $f\mapsto  \langle f, \varphi \rangle$ sur $L^1(G)$. Alors $\varphi$ est la classe d’une fonction de type positif sur G si et seulement si $\lambda_{\varphi}$ est une forme linéaire positive continue sur $L^1(G)$.

Supposons que $\lambda_{\varphi}$ est une forme linéaire positive continue sur $L^1(G)$. Soit $(E, x,\widetilde{\pi})$ une réalisation hilbertienne cyclique de $\lambda$ (prop. 5 de V, p. 438).

Soit $\pi$ une représentation unitaire de G dans E telle que $\pi (f) =\widetilde{\pi}(f)$ pour tout $f\in L^1(G)$ (prop. 12). On a alors $\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle$ pour tout $f\in L^1(G)$.

Comme

$$
\pi (f) =\int_Gf(g)\pi (g)d\mu(g)
$$

pour tout $f\in L^1$(G), il vient

$$
\int_Gf(g)\varphi (g)d\mu(g) =\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle =\int_Gf(g)\langle x|\pi (g)x\rangle d\mu(g)
$$

pour tout $f\in L^1(G)$ (INT, VI, p. 9, § 1, n$^o1$, prop. 1). Ainsi, $\varphi$ est la classe dans $L^{\infty}(G)$ de la fonction sur G définie par $g\mapsto  \langle x|\pi (g)x\rangle$, qui est une fonction de type positif sur G (prop. 9 de V, p. 443).

Réciproquement, soit $\varphi \in$ Pos(G). Soit $f\in \mathscr{K}(G)$. On a alors

$$
\lambda_{\varphi}(f^**f) =\int_G\varphi (y)\int_G\Delta (z)^{-1}f(z^{-1})f(z^{-1}y)d\mu(z)d\mu(y)
$$

$$
=\int_G\varphi (y)\int_Gf(z)f(zy)d\mu(z)d\mu(y)
$$

(INT, VII, p. 19, § 1, n$^o3$, formule (22)). La fonction continue sur $G\times G$ définie par $(z, y)\mapsto \varphi (y)f(z)f(zy)$ est bornée et

$$
\int_G^*|\varphi(y)|\left(\int_G^*|\overline{f(z)}f(zy)|d\mu(z)\right)d\mu(y)
$$

$$
\leqslant\varphi(e)\int_G^*\int_G^*|f(z)||f(zy)|d\mu(z)d\mu(y)
$$

$$
=\varphi(e)\left(\int_G^*|f(z)|d\mu(z)\right)^2
$$

d’après INT, V, p. 94, § 8, n$^o3$, prop. 8. On déduit donc du théorème de Lebesgue–Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1) que

$$
\lambda_{\varphi}(f^**f) =\int_Gf(z)\int_G\varphi (y)f(zy)d\mu(y)d\mu(z)
$$

$$
=\int_{G\times G}f(z)f(y)\varphi (z^{-1}y)d(\mu\otimes \mu)(z, y)
$$

Cela implique que $\lambda_{\varphi}(f^**f)\geqslant 0$ d’après le théorème 1, (i) de V, p. 432 appliqué à la mesure induite par $\mu$ sur le support de $f$ (INT, IV, p. 186, § 5, n$^o7$, déf. 4). On en déduit par continuité que $\lambda_{\varphi}(f^**f)\geqslant 0$ pour tout $f\in L^1(G)$.

Les espaces $L^{\infty}(G)$ et $\mathscr{C}_b(G)$ sont munis de leurs topologies d’espaces de Banach, dont on note $f\mapsto  \|f\|_{\infty}$ la norme. On appellera ici topologie faible sur $L^{\infty}$(G), $\mathscr{C}_b(G)$ ou Pos(G) la topologie induite par la topologie faible $\sigma (L^{\infty}(G),L^1(G))$.

Comme $L^{\infty}(G)$ s’identifie au dual de $L^1(G)$ (INT, V, p. 61, §5, n$^o8$, th. 4), toute boule fermée de $L^{\infty}(G)$ est compacte pour la topologie faible (EVT, III, p. 17, cor. 3).

#### Corollaire {#ts-v-s3-n6-cor-1 .statement tag=03CP}

Dans $L^{\infty}(G)$ muni de la topologie faible, l’ensemble Pos(G) est fermé et l’ensemble Pos$_{\leqslant 1}(G)$ est compact.

La première assertion résulte de la proposition, et la seconde découle alors de EVT, III, loc. cit.

En général, Pos$_1(G)$ n’est pas compact pour la topologie faible, comme le montre l’exemple du groupe $\mathbf{R}$ (exercice 10 de V, p. 497).

#### Proposition 14 {#ts-v-s3-prop-14 .statement tag=03CQ}

L’ensemble des points extrémaux de Pos$_{\leqslant 1}(G)$ est égal à la réunion de l’ensemble des points extrémaux de Pos$_1(G)$ et de la fonction nulle. De plus, l’enveloppe fermée convexe de l’ensemble des points extrémaux de Pos$_1(G)$ contient Pos$_1(G)$.

D’après le cor. de la prop. 13, l’ensemble Pos$_{\leqslant 1}(G)$ est un chapeau du cône convexe pointé Pos(G), qui est défini par la jauge $\varphi \mapsto \varphi (e)$ (EVT, II, p. 61, déf. 3 et prop. 4). Ses points extrémaux sont donc la fonction nulle et les éléments $\varphi$ de Pos$_1(G)$ appartenant aux génératrices extrémales de Pos(G) (EVT, II, p. 62, cor. 1). Ceux-ci sont les points extrémaux de Pos$_1(G)$ (EVT, II, p. 61, prop. 3). La première assertion en résulte.

Démontrons la seconde assertion. Soit $\varphi \in$ Pos$_1(G)$. Comme l’ensemble Pos$_{\leqslant 1}(G)$ est compact pour la topologie faible (cor. de la prop. 13), il existe un filtre $\mathfrak{F}$ sur l’enveloppe convexe des points extrémaux de Pos$_{\leqslant 1}(G)$ qui converge vers $\varphi$ (EVT, II, p. 59, th. 1). Comme les boules fermées de l’espace de Banach $L^{\infty}(G)$ sont fermées pour la topologie faible et que $\|\varphi \|_{\infty}= 1$, on a lim$_{\psi ,\mathfrak{F}}\|\psi \|_{\infty}= 1$ (en effet, dans le cas contraire, il existerait un nombre réel $c <1$ et un filtre $\mathfrak{G}$ sur la boule fermée de rayon $c$ dans $L^{\infty}(G)$ qui serait plus fin que $\mathfrak{F}$, ce qui impliquerait que $\varphi$ appartient à cette boule fermée).

D’après la description des points extrémaux de Pos$_{\leqslant 1}$(G), tout élément $\psi$ de l’enveloppe convexe des points extrémaux de Pos$_{\leqslant 1}(G)$ est une fonction de type positif sur G de la forme

$$
\psi =\sum_{i\in I}t_i\psi_i
$$

où I est un ensemble fini, $\psi_i$ est un point extrémal de Pos$_1(G)$ pour tout $i\in I$, et $t_i\in [0,1]$. On a $\sum_it_i=\psi (e) =\|\psi \|_{\infty}\leqslant 1$ (lemme 4 de V, p. 446). Si $\psi \not = 0$, la fonction

$$
\frac{\psi}{\|\psi\|_{\infty}}=\sum_{i\in I}\frac{t_i}{\psi(e)}\psi^i
$$

appartient donc à l’enveloppe convexe des points extrémaux de Pos$_1(G)$. Comme lim$_{\psi ,\mathfrak{F}}\|\psi \|^{-1}_{\infty}\psi =\varphi$, on conclut que $\varphi$ appartient à l’enveloppe fermée convexe des points extrémaux de Pos$_1(G)$. L’assertion en résulte.

### 7. Existence de représentations irréductibles

On conserve les notations du numéro précédent.

#### Théorème 3 (Raikov) {#ts-v-s3-thm-3 .statement tag=03CR}

La topologie faible sur Pos$_1(G)$ coïncide avec la topologie de la convergence compacte.

Nous démontrerons d’abord quelques lemmes.

#### Lemme 5 {#ts-v-s3-lem-5 .statement tag=03CS}

Soient X un espace topologique localement compact et $\nu$ une mesure positive sur X. Sur toute partie bornée de $\mathscr{C}_b(X)$, la topologie induite par la topologie faible $\sigma (L^{\infty}(X),L^1(X))$ est moins fine que la topologie de la convergence compacte.

Soit B une partie bornée de $\mathscr{C}_b(X)$ et soit $M\in \mathbf{R}_+$ tel que $\|\varphi \|_{\infty}\leqslant M$ pour tout $\varphi \in B$. Soient $\psi \in L^1(X, \nu )$ et $\varepsilon  >0$. Fixons une partie compacte K de X telle que

$$
\int_{X-K}|\psi |d\nu  < \varepsilon
$$

Pour tous $\varphi_1$ et $\varphi_2$ dans B, on a alors

$$
\langle \varphi_1-\varphi_2, \psi \rangle =\int_X\psi (\varphi_1-\varphi_2)d\nu
$$

$$
=\int_K\psi (\varphi_1-\varphi_2)d\nu +\int_{X-K}\psi (\varphi_1-\varphi_2)d\nu
$$

d’où

$|\langle \varphi_1-\varphi_2, \psi \rangle |\leqslant$ sup$_{x\in K}|\varphi_1(x)-\varphi_2(x)| \|\psi \|_1+ 2M\varepsilon$,

et le lemme en résulte.

#### Lemme 6 {#ts-v-s3-lem-6 .statement tag=03CT}

Soit $\psi \in L^1(G)$. Soit B une partie bornée de l’espace de Banach $L^{\infty}(G)$. L’application $\varphi \mapsto \psi *\varphi$ de B dans $\mathscr{C}_b(G)$ est continue lorsque B est muni de la topologie faible et $\mathscr{C}_b(G)$ de la topologie de la convergence compacte.

Soient $\varphi \in L^{\infty}(G)$ et $\eta \in L^1(G)$. La fonction $\Delta^{-1}\check{\eta}$ appartient à $L^1(G)$ et $\langle \eta ,\check{\psi}\rangle =\langle \Delta^{-1}\check{\eta , \psi}\rangle ($cf. INT, VII, p. 19, § 1, n$^o3$, formule (22)). L’application $\varphi \mapsto \check{\varphi}$ est donc un automorphisme de l’espace $L^{\infty}(G)$ muni de la topologie faible.

Soit $\varphi \in L^{\infty}(G)$. D’après INT, VIII, p. 167, § 4, n$^o5$, prop. 14, la fonction $\psi *\varphi$ appartient à $\mathscr{C}_b(G)$ et vérifie

$$
(\psi *\varphi )(g) =\int_G\psi (h)\varphi (h^{-1}g)d\mu(h)
$$

$=\int_G\psi (gy)\check{\varphi}(y)d\mu(y) =\langle \check{\varphi ,}\boldsymbol{\gamma }$[^1]$_G(g^{-1})\psi \rangle$ pour tout $g\in G$. Il en résulte que l’application linéaire $u:\varphi \mapsto \psi *\varphi$ est une application continue de l’espace $L^{\infty}(G)$ muni de la topologie faible dans $\mathscr{C}_b(G)$ muni de la topologie de la convergence simple.

Soient $\varphi \in B$ et $(g, h)\in G\times G$. D’après la formule ci-dessus, on a

$|u(\varphi )(g)-u(\varphi )(h)|\leqslant \|\check{\varphi}\|_{\infty}\|(\boldsymbol{\gamma }$[^1]$_G(g^{-1})-\boldsymbol{\gamma }$[^1]$_G(h^{-1}))\psi \|_1$.

Comme B est bornée et que la représentation régulière gauche de G dans $L^1(G)$ est continue (n$^o4$ de V, p. 405), cela implique que $u(B)$ est une partie équicontinue de $\mathscr{C}_b(G)$. L’assertion résulte alors de ce qui précède et de TG, X, p. 16, th. 1.

#### Lemme 7 {#ts-v-s3-lem-7 .statement tag=03CU}

Soit $\psi \in L^1(G)$ telle que $\psi \geqslant 0$ et $\int\psi = 1$. Notons $p$ la semi-norme sur $\mathscr{C}_b(G)$ définie par $p(\varphi ) =|\langle \varphi , \psi \rangle |$ pour tout $\varphi \in \mathscr{C}_b(G)$. Pour tout $\varphi \in$ Pos$_1(G)$, on a

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \surd\overline{2p(1 -\varphi)}
$$

Soient $\varphi \in$ Pos$_1(G)$ et $x\in G$. D’après INT, VIII, p. 167, § 4, n$^o5$, prop. 14, on obtient

$$
|\psi *\varphi (x)-\varphi (x)|=|\int_G(\varphi (y^{-1}x)-\varphi (x))\psi (y)d\mu(y)|
$$

$$
\leqslant \int_G|\varphi (y^{-1}x)-\varphi (x)|\psi (y)d\mu(y)
$$

$$
\leqslant \int_G\surd\overline{2(1 -\mathscr{R}\varphi(y))}\psi (y)d\mu(y)
$$

en appliquant la majoration (1) de V, p. 446. L’inégalité de CauchySchwarz implique alors

$\surd \int 1/2\int 1/2$

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \overline{2}(_G(1-\mathscr{R}(\varphi ))\psi  d\mu)(_G\psi  d\mu)
$$

$$
\surd \surd
$$

$\leqslant$ 2 $p(1-\varphi )$,

d’où le résultat.

#### Lemme 8 {#ts-v-s3-lem-8 .statement tag=03CV}

Soit K un corps topologique et soient E et F des espaces vectoriels topologiques sur K. Soient $f$ une application de E dans F et X une partie de E. Soit $x\in X$. L’application $f|X$ est continue en $x$ si, pour tout voisinage W de 0 dans F, il existe un voisinage U de $x$ dans E et une application continue $g$ de X dans F tels que $(f-g)(U\cap X)\subset W$.

Soit $W_0$ un voisinage de 0 dans F et soit $V_0$ un voisinage symétrique de 0 dans F tel que $V_0+V_0+V_0\subset W_0$. Soit $U_0$ un voisinage de $x$ dans E et $g$ une application continue de X dans F telle que $(f-g)(U_0\cap X)\subset V_0$. Il existe un voisinage $U_1$ de $x$ dans E tel que $g(U_1\cap X)\subset g(x) + V_0$. Pour tout $y\in U_0\cap U_1\cap X$, on a

$$
f(y)-f(x) = (f(y)-g(y)) + (g(y)-g(x))+
$$

$$
(g(x)-f(x))\in V_0+ V_0+ V_0\subset W_0
$$

donc $f(y)\in f(x) + W_0$, d’où le résultat.

Démontrons maintenant le théorème 3. Notons Pos$_1(G)_f$ (resp. Pos$_1(G)_c)$ l’ensemble Pos$_1(G)$ muni de la topologie faible (resp. de la topologie de la convergence compacte) ; de même, notons $\mathscr{C}_b(G)_f$ (resp. $\mathscr{C}_b(G)_c)$ l’espace $\mathscr{C}_b(G)$ muni de la topologie faible (resp. de la topologie de la convergence compacte).

L’application identité de Pos$_1(G)_c$ dans Pos$_1(G)_f$ est continue (lemme 5). Réciproquement, notons $\iota$ l’inclusion de Pos$_1(G)_f$ dans $\mathscr{C}_b(G)_c$. Démontrons que $\iota$ est continue pour conclure la démonstration.

Soit $\varphi_1\in$ Pos$_1(G)$. Pour vérifier que $\iota$ est continue en $\varphi_1$, nous appliquons le lemme 8. Soit W un voisinage de 0 dans $\mathscr{C}_b(G)_c$. Il suffit de trouver une application linéaire $u$ de $\mathscr{C}_b(G)$ dans $\mathscr{C}_b(G)$ qui induit par passage aux sous-espaces une application continue de Pos$_1(G)_f$ dans $\mathscr{C}_b(G)_c$, ainsi qu’un voisinage U de 0 dans Pos$_1(G)_f$, de sorte que l’on ait $(\iota -u)(U\cap$ Pos$_1(G))\subset W$.

Il existe $\varepsilon  >0$ tel que W contient l’ensemble des $\varphi \in \mathscr{C}_b(G)$ qui vérifient $\|\varphi \|_{\infty}\leqslant \varepsilon$. Comme $\varphi_1(e) = 1$, il existe un voisinage compact V de $e$ dans G tel que

sup$_{x\in V}|1-\varphi_1(x)|\leqslant \frac{\varepsilon^2}{4}$.

Soit $\varphi_V$ la fonction caractéristique de V, et posons $\psi_V=\mu(V)^{-1}\varphi_V$. L’application linéaire $u:\varphi \mapsto \psi_V*\varphi$ de Pos$_1(G)_f$ dans $\mathscr{C}_b(G)_c$ est continue (lemme 6).

Notons $q_V$ la semi-norme $\varphi \mapsto  |\langle \varphi , \psi_V\rangle |$ sur $\mathscr{C}_b(G)$; elle est continue pour la topologie faible. Puisque $\psi_V$ est nulle en dehors de V, il vient $q_V(1-\varphi_1)\leqslant \varepsilon^2/4$; il existe donc un voisinage U de $\varphi_1$ dans $\mathscr{C}_b(G)_f$ tel que $q_V(1-\varphi )\leqslant \varepsilon^2/2$ pour tout $\varphi \in U$.

Soit $\varphi \in U\cap$ Pos$_1(G)$. D’après le lemme 7, on a

$$
\|(\iota -u)(\varphi )\|_{\infty}\leqslant \surd\overline{2q_V(1 -\varphi)}\leqslant \varepsilon
$$

donc $(\iota -u)(U)\subset W$. Le théorème est démontré.

En général, la topologie faible sur Pos$_{\leqslant 1}(G)$ ne coïncide pas avec la topologie de la convergence compacte, comme le montre l’exemple du groupe $\mathbf{R}$.

On rappelle qu’on note $\widehat{G}$ l’ensemble des classes de représentations unitaires irréductibles de G (V, p. 393, déf. 8).

#### Théorème 4 (Gelfand–Raikov) {#ts-v-s3-thm-4 .statement tag=03CW}

Pour tout $x\not =e$ dans G, il existe une représentation unitaire irréductible $\pi$ de G telle que $\pi (x)$ n’est pas l’endomorphisme identique de l’espace de $\pi$.

Soit $x\in G$ tel que $\pi (x)$ est l’identité pour tout $\pi \in \widehat{G}$. Il en résulte que $\varphi (x) =\varphi (e) = 1$ pour tout point extrémal $\varphi$ de Pos$_1(G)$ (prop. 11 de V, p. 444), donc pour tout $\varphi \in$ Pos$_1(G)$ d’après la prop. 14 puisque la forme linéaire $\varphi \mapsto \varphi (e)$ est continue sur Pos$_1(G)$ muni de la topologie faible (th. 3). Mais si $x\not =e$, il existe $f\in L^2(G)$ de norme 1 tel que $\langle f|\boldsymbol{\gamma }_G(x)f\rangle = 0$(V, p. 406, lemme 3). Comme le membre de gauche de cette égalité est de la forme $\varphi (x)$, où $\varphi \in$ Pos$_1$(G), c’est une contradiction.

Si G n’est pas localement compact, il n’est pas toujours vrai que les représentations unitaires irréductibles de G séparent les points de G.

#### Corollaire {#ts-v-s3-n7-cor-1 .statement tag=03CX}

Pour tous éléments $g\not =h$ dans G, il existe une représentation irréductible $\pi \in \widehat{G}$ et un coefficient matriciel $f$ de $\pi$ tel que $f(g)\not =f(h)$. En particulier, la sous-algèbre Υ(G) de $\mathscr{C}_b(G)$ sépare les points de G.

Soient $g\not =h$ dans G. Il existe une représentation irréductible $\pi \in \widehat{G}$ telle que $\pi (g)\not =\pi (h)$ (th. 4), donc il existe $x$ et $y$ dans l’espace de $\pi$ tels que $\langle x|\pi (g)y\rangle  \not =\langle x|\pi (h)y\rangle$.

### 8. Fonctions de type positif sur un groupe localement compact commutatif

Dans ce numéro, G est un groupe localement compact commutatif et $\mu$ désigne une mesure de Haar sur G. On note $\widehat{G}$ le groupe dual de G et $\widehat{\mu}$ la mesure de Haar duale de $\mu$ (déf. 4 de II, p. 214). On note $\mathscr{F}$ la transformation de Fourier sur l’espace de Banach $\mathscr{M}^1(G)$ des mesures bornées sur G.

Puisque $\mathscr{C}_0(G)$ est l’adhérence de $\mathscr{K}(G)$ dans $\mathscr{C}_b$(G), l’espace de Banach $\mathscr{M}^1(G)$ dual de $\mathscr{K}(G)$ muni de la topologie de $\mathscr{C}_b(G)$ s’identifie au dual de $\mathscr{C}_0(G) ($cf. INT, III, p. 56, § 1, n$^o8)$. On munit $\mathscr{M}^1(G)$ de la topologie faible associée à cette dualité.

#### Lemme 9 {#ts-v-s3-lem-9 .statement tag=03CY}

La transformation de Fourier est une application continue de $\mathscr{M}^1(G)$ muni de la topologie faible dans $\mathscr{C}_b(\widehat{G})$ muni de la topologie induite par la topologie faible $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$.

Soit $\mathfrak{F}$ un filtre sur $\mathscr{M}^1(G)$ convergeant faiblement vers une mesure bornée $\nu$ sur G. Pour tout $\varphi \in L^1(\widehat{G})$, on a $\mathscr{F}(\varphi )\in \mathscr{C}_0(G)$ (prop. 4 de II, p. 209), donc

$$
\int_{\widehat{G}}\varphi \mathscr{F}(\nu )d\widehat{\mu}=\int_G\mathscr{F}(\varphi )d\nu
$$

= lim$_{\eta ,\mathfrak{F}}\int_G\mathscr{F}(\varphi )d\eta =$ lim$_{\eta ,\mathfrak{F}}\int_{\widehat{G}}\varphi \mathscr{F}(\eta )d\widehat{\mu}$,

d’après la propriété de transposition de la transformation de Fourier (prop. 13 de II, p. 221). Le lemme en découle.

#### Théorème 5 (Bochner) {#ts-v-s3-thm-5 .statement tag=03CZ}

Une fonction continue $\varphi$ sur $\widehat{G}$ appartient à Pos($\widehat{G}$) si et seulement s’il existe une mesure positive bornée $\nu$ sur G telle que $\varphi =\mathscr{F}(\nu )$.

Soit $\nu \in \mathscr{M}^1(G)$ une mesure positive. Sa transformée de Fourier est continue. Pour toute famille finie $(x_i)_{i\in I}$ dans $\widehat{G}$ et toute famille finie $(t_i)_{i\in I}$ de nombres complexes, il vient

$$
\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\mathscr{F}(\nu )(x^{-1}_ix_j) =\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\int_Gx_i\overline{x}_jd\nu
$$

$$
=\int_G|\sum_{i\in I}\overline{t}_ix_i|^2d\nu \geqslant 0
$$

puisque $\nu$ est une mesure positive. La transformée de Fourier de $\nu$ est donc une fonction de type positif sur $\widehat{G}$ (th. 1 de V, p. 432, (ii)).

Démontrons la réciproque. Munissons l’ensemble Pos$_{\leqslant 1}(\widehat{G})$ de la topologie faible, induite comme précédemment par la topologie faible $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$. L’ensemble Pos$_{\leqslant 1}(\widehat{G})$ est compact et convexe (cor. de la prop. 13 de V, p. 448). D’après la prop. 14 de V, p. 450, la prop. 11 de V, p. 444 et le cor. 7 de V, p. 390, les points extrémaux de Pos$_{\leqslant 1}(\widehat{G})$ sont la fonction nulle et les éléments de $\widehat{G}$.

Soit $\mathscr{N}$ l’ensemble des mesures positives bornées de masse $\leqslant 1$ sur G ; il est compact dans $\mathscr{M}^1(G)$ muni de la topologie faible (EVT, III, p. 17, cor. 3). D’après le lemme 9 et la première partie de la preuve, la transformation de Fourier sur G définit par passage aux sous-espaces une application continue de $\mathscr{N}$ dans Pos$_{\leqslant 1}(\widehat{G})$; par homogénéité, il suffit de démontrer que cette application est surjective. L’image $\mathscr{F}(\mathscr{N})$ de $\mathscr{N}$ par la transformation de Fourier est convexe et compacte ; elle contient la fonction nulle et les éléments de $\widehat{G}$ (en effet, ceux-ci sont de la forme ev$_x:\chi \mapsto \chi (x)$ pour un élément $x$ de G d’après le th. 2 de II, p. 220, et on a ev$_x=\mathscr{F}(\varepsilon_{x^{-1}}))$. L’ensemble $\mathscr{F}(\mathscr{N})$ contient donc les points extrémaux de Pos$_{\leqslant 1}$(G), d’où $\mathscr{F}(\mathscr{N}) =$ Pos$_{\leqslant 1}(G)$ d’après le théorème de Krein–Milman (EVT, II, p. 59, th. 1). Cela conclut la démonstration.

Lorsque $G =\mathbf{R}^k$ pour un entier $k\in \mathbf{N}$, ce théorème correspond à la prop. 11 de INT, IX, p. 94, § 6, n$^o12$.

## EXERCICES {#ts-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
