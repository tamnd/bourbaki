---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 2
section_title: Algèbres normées
lang: fr
source: ts-i-ii-fr
book_pages: TS I.15-TS I.29, TS I.155-TS I.165
pdf_pages: 0028-0042, 0168-0178
extraction: native
subsections:
    - "no": 1
      title: Généralités
      page: 15
      pdf_page: 28
    - "no": 2
      title: Exemples
      page: 17
      pdf_page: 30
    - "no": 3
      title: Rayon spectral
      page: 20
      pdf_page: 33
    - "no": 4
      title: Inverses
      page: 22
      pdf_page: 35
    - "no": 5
      title: Spectre d’un élément dans une algèbre normée
      page: 24
      pdf_page: 37
    - "no": 6
      title: Spectre relatif à une sous-algèbre
      page: 28
      pdf_page: 41
statements: 28
exercises: 37
content_sha256: 015c9053b44cbf4ed498e124264f53c7733518249f85e8b9f95aff2a1903796f
---

## § 2. ALGÈBRES NORMÉES

Dans cette section, K désigne l’un des corps $\mathbf{R}$ ou $\mathbf{C}$.

### 1. Généralités

Rappelons (cf. TG, IX, p. 37, déf. 9) que l’on appelle algèbre normée une algèbre A sur K munie d’une norme $x\mapsto  \|x\|$ telle que :

$$
\|xy\|\leqslant \|x\| \|y\| \tag{1}
$$

quels que soient $x,y\in A$. Si A est complète, on dit que A est une algèbre de Banach.

Soit A une algèbre normable complète sur K. La topologie de A peut être définie par une norme vérifiant (1) (cf. TG, IX, p. 38). Lorsque A est munie de la structure d’algèbre normée définie par une telle norme, on dira aussi que l’algèbre A est une algèbre de Banach.

Rappelons également les faits suivants (cf. TG, IX, p. 38–39) :

(1) Si A est une algèbre normée non nulle et possède un élément unité $e$, alors $\|e\|\geqslant 1$.

(2) Soit A une K-algèbre normée. L’algèbre opposée à A, munie de la même norme, est une algèbre normée. L’algèbre complétée de A, munie de la norme obtenue par prolongement par continuité de la norme de A, est une K-algèbre de Banach. Toute sous-algèbre de A, munie de la norme induite, est une algèbre normée. Si I est un idéal bilatère fermé de A, l’algèbre $A/I$, munie de la norme définie par $\|\dot{x}\|=$ inf$_{x\in\dot{x}}\|x\|$ pour tout $\dot{x}\in A/I$, est une algèbre normée.

(3) Soient $(A_i)_{\in I}$ une famille d’algèbres normées et B l’algèbre produit des algèbres $A_i$. La sous-algèbre des éléments $(x_i)_{i\in I}$ de B tels que $\|(x_i)\|=$ sup$_{i\in I}\|x_i\|<+\infty$, est une algèbre normée, dite algèbre normée produit des algèbres $(A_i)_{i\in I}$. Si $A_i$ est une algèbre de Banach pour tout $i$, alors A est une algèbre de Banach.

Soit A une algèbre normée. Soit $(y_i)_{i\in I}$ une famille d’éléments de A ; la plus petite sous-algèbre fermée B de A contenant les éléments $y_i$ s’appelle la sous-algèbre fermée de A engendrée par les $y_i$; si B = A, on dit que les $y_i$ engendrent topologiquement l’algèbre normée A, ou que la famille $(y_i)_{i\in I}$ est un système générateur topologique de l’algèbre normée A.

Similairement, si A est une algèbre normée unifère, la plus petite sous-algèbre unifère fermée contenant les éléments $y_i$ s’appelle la sous-algèbre unifère fermée de A engendrée par les $y_i$. Si elle est égale à A, on dit que les $y_i$ engendrent topologiquement l’algèbre normée unifère A.

Soit A une K-algèbre normée. Notons $\widetilde{A}$ l’algèbre obtenue à partir de A par adjonction d’un élément unité. Sur $\widetilde{A}$, on définit une norme en posant $\|(\lambda , x)\|=|\lambda |+\|x\|$ pour tout $\lambda \in K$ et tout $x\in A$. On a

$$
\|(\lambda , x)(\mu, y)\|=|\lambda \mu|+\|xy+\mu x+\lambda y\|
$$

$$
\leqslant |\lambda | |\mu|+\|x\| \|y\|+|\mu| \|x\|+|\lambda | \|y\|
$$

$$
=\|(\lambda , x)\| \|(\mu, y)\|
$$

Donc $\widetilde{A}$ devient une algèbre normée, appelée algèbre unifère normée déduite de A par adjonction d’un élément unité. L’algèbre A s’identifie à l’idéal bilatère fermé $\{0\} \times A$ de $\widetilde{A}$.

#### Définition 1 {#ts-i-s2-def-1 .statement tag=025W}

Soit A une algèbre normée. Pour $a\in A$, notons $\boldsymbol{\gamma }_a$ et $\boldsymbol{\delta }_a$ les applications $x\mapsto ax$, et $x\mapsto xa$ de A dans A. L’application $\boldsymbol{\gamma }:a\mapsto \boldsymbol{\gamma }_a$ est une représentation de A dans A, dite représentation régulière gauche de A. L’application $\boldsymbol{\delta }:a\mapsto \boldsymbol{\delta }_a$ est une représentation de l’algèbre opposée de A dans A, dite représentation régulière droite de A.

#### Lemme 1 {#ts-i-s2-lem-1 .statement tag=025X}

Soit A une algèbre normée. La représentation régulière gauche de A et la représentation régulière droite de A sont continues de norme $\leqslant 1$.

Si l’algèbre A est unifère, les applications $x\mapsto  \|\boldsymbol{\gamma }_x\|$ et $x\mapsto  \|\boldsymbol{\delta }_x\|$ sont des normes sur A, définissant la topologie de A. Elles vérifient l’inégalité (1).

Si l’algèbre normée unifère A est non nulle, c’est-à-dire si $e\not= 0$, on a aussi $\|\boldsymbol{\gamma }_e\|=\|\boldsymbol{\delta }_e\|= 1$.

Il est immédiat que $\|\boldsymbol{\gamma }_x\|\leqslant \|x\|$ et que $\|\boldsymbol{\delta }_x\|\leqslant \|x\|$.

Si A possède un élément unité $e$, alors on a $x=\boldsymbol{\gamma }_xe=\boldsymbol{\delta }_xe$, donc : (2) $\|x\|\leqslant \|\boldsymbol{\gamma }_x\| \cdot  \|e\|\|x\|\leqslant \|\boldsymbol{\delta }_x\| \cdot  \|e\|$.

Dans ce cas, $x\mapsto  \|\boldsymbol{\gamma }_x\|$ et $x\mapsto  \|\boldsymbol{\delta }_x\|$ sont donc des normes équivalentes à la norme de A. Elles vérifient (1) car $\boldsymbol{\gamma }$ et $\boldsymbol{\delta }$ sont des représentations.

La dernière assertion provient du fait que $\boldsymbol{\gamma }_e=\boldsymbol{\delta }_e=$ Id$_A$.

### 2. Exemples

1) Soit E un espace normé. Munissons E du produit défini par $ab= 0$ pour tous $a$ et $b$ dans E ; cela définit sur E une structure d’algèbre normée.

2) Soit X un ensemble. On note $\mathscr{B}(X; K)$ l’algèbre normée des fonctions bornées sur X à valeurs dans K, munie de la norme

$\|f\|=$ sup$|f(x)|$

$x\in X$

(TG, X, p. 22). C’est une algèbre de Banach unifère sur K (TG, X, p. 21, cor. 1). Elle est commutative. Soit $f$ un élément de $\mathscr{B}(X; K)$. Alors $f$ est inversible dans $\mathscr{B}(X; K)$ si et seulement si on a

$_x$inf$_{\in X}|f(x)|>0$.

Le spectre de $f$ est donc l’ensemble des $\lambda \in K$ tels que

$_x$inf$_{\in X}|f(x)-\lambda |= 0$,

c’est-à-dire l’adhérence dans K de l’ensemble $f(X)$ des valeurs de $f$.

3) Soit X un espace topologique. On note $\mathscr{C}_b(X; K)$ la sous-algèbre unifère de $\mathscr{B}(X; K)$ des fonctions continues et bornées sur X à valeurs dans K$,\mathscr{C}_0(X; K)$ la sous-algèbre de $\mathscr{C}_b(X; K)$ constituée des fonctions qui tendent vers 0 à l’infini (cf. INT, III, §1, n$^o2$ et TG, X, p. 40, cor. 2). On rappelle que $\mathscr{K}(X; K)$ désigne la sous-algèbre de $\mathscr{C}_b(X; K)$ des fonctions continues à support compact.

Les algèbres $\mathscr{C}_b(X; K)$ et $\mathscr{C}_0(X; K)$ sont des algèbres de Banach commutatives sur K; en effet, ce sont des sous-espaces fermés de $\mathscr{B}(X; K)$ (TG, X, p. 21, cor. 2 et INT, III, §1, n$^o2)$.

L’inverse d’une fonction continue partout non nulle étant continue, la sous-algèbre $\mathscr{C}_b(X; K)$ est une sous-algèbre pleine de $\mathscr{B}(X; K)$. En particulier, le spectre d’un élément $f$ de $\mathscr{C}_b(X; K)$ est égal à $\overline{f(X)}$.

Si X est discret, on a $\mathscr{C}_b(X; K) =\mathscr{B}(X; K)$.

Si X est compact, on $\mathscr{C}_b(X; K) =\mathscr{K}(X; K) =\mathscr{C}(X; K)$, l’algèbre unifère normée $\mathscr{C}(X; K)$ des fonctions continues sur X à valeurs dans K. Dans ce cas, un élément $f\in \mathscr{C}(X; K)$ est inversible si et seulement si $f$ ne prend pas la valeur 0, et le spectre de $f$ est égal à l’ensemble $f(X)$ des valeurs de $f$.

Supposons désormais que X n’est pas compact. L’algèbre $\mathscr{C}_0(X; K)$ n’est alors pas unifère ; l’algèbre qui s’en déduit par adjonction d’un élément unité s’identifie à la sous-algèbre $K\cdot 1\oplus \mathscr{C}_0(X; K)$ de $\mathscr{C}(X; K)$ formée des fonctions qui ont une limite à l’infini. Pour qu’un élément de cette sous-algèbre soit inversible, il faut et il suffit qu’elle ne s’annule pas et que sa limite à l’infini ne soit pas nulle. Il en résulte que pour tout $f\in \mathscr{C}_0(X; K)$, le spectre de $f$ est égal à $f(X)\cup  \{0\}$.

Le spectre de $f\in \mathscr{K}(X; K)$ est égal à $f(X)$ (en effet, si X n’est pas compact, 0 appartient à $f(X)$).

4) Soit $n\geqslant 0$ un entier. Soit $A_n$ l’algèbre des fonctions $f: [0,1]\rightarrow K$ admettant des dérivées continues dans $[0,1]$ jusqu’à l’ordre $n$, munie de la norme

$^n$ 1 $(_{k)}$

$\|f\|=\sum$ sup $|f(t)|$.

$k$! $_{0\leqslant t\leqslant 1}$

$k=0$

Si $f, g\in A_n$, on a

$n$ 1 $(k)n$ 1 $k(k)(s)(k-s)$

$\|f g\|=\sum$ sup$|(f g)(t)|=\sum$ sup $\sum f(t)g(t)$

$k$! $k$! $s$

$k=0k=0s=0$

$nk$ 1 $(s)(k-s)$

$\leqslant \sum\sum$ sup $|f(t)|$ sup $|g(t)|=\|f\| \|g\|$,

$s$!($k-s$)! $_{0\leqslant t\leqslant 1}0_{\leqslant t\leqslant 1}$

$k=0s=0$

d’après la formule de Leibniz (FVR, I, p. 28, prop. 2), donc $A_n$ est une algèbre de Banach unifère commutative.

5) Soit E un espace de Banach dont on note $p$ la norme. L’algèbre $\mathscr{L}(E)$ des endomorphismes continus de E, munie de la norme

$\|u\|=$ sup $p(u(x))$

$p(x)\leqslant 1$

est une algèbre de Banach unifère (EVT, III, p. 14 et p. 24, cor. 2 ; TG, X, p. 23, formule (3)).

6) Soit G un groupe localement compact. Notons $e$ son élément unité. Soit $\mathscr{M}^1(G)$ l’espace de Banach des mesures complexes bornées sur G (INT, III, p. 57). Le produit de convolution (INT, VIII, p. 120, déf. 1) munit $\mathscr{M}^1(G)$ d’une structure d’algèbre de Banach complexe (INT, VIII, §3, n$^o1$, prop. 2) admettant pour élément unité la mesure $\varepsilon_e$ définie par la masse unité placée au point $e$. Si G est commutatif, cette algèbre de Banach est commutative. L’espace $\mathscr{C}'(G)$ des mesures à support compact est une sous-algèbre de $\mathscr{M}^1(G)$ (loc. cit.).

7) Soit G un groupe localement compact muni d’une mesure de Haar $\mu$. Alors $L^1_K(G, \mu)$ est une algèbre de Banach pour le produit de convolution (INT, VIII, prop. 12, p. 166). Si $K =\mathbf{C}$, l’application définie par $f\mapsto f \mu$ permet d’identifier $L^1_{\mathbf{C}}(G, \mu)$ à une sous-algèbre de l’algèbre de Banach $\mathscr{M}^1(G)$.

Si G est commutatif, l’algèbre de Banach $L^1_K(G, \mu)$ est commutative.

8) Prenons $G =\mathbf{Z}$ et $K =\mathbf{C}$ dans l’exemple 7. Alors $L^1_{\mathbf{C}}(\mathbf{Z})$ est l’algèbre de Banach commutative complexe des suites $(x_n)_{n\in\mathbf{Z}}$ telles que $\sum_n|x_n|<+\infty$, le produit des éléments $(x_n)$ et $(y_n)$ étant $(z_n)$, où

$$
z_n=\sum_{k\in\mathbf{Z}}x_ky_{n-k}
$$

et la norme $\|(x_n)\|=\sum_n|x_n|$. Cette algèbre admet pour élément unité la suite $\varepsilon = (\varepsilon_n)$ telle que $\varepsilon_0= 1$ et $\varepsilon_n= 0$ pour $n\not= 0$.

Notons $\mathbf{U}$ le cercle unité dans $\mathbf{C}$. Si $x= (c_n)$ est un élément de A, soit $\varphi (x)$ la fonction continue sur $\mathbf{U}$ dont la valeur en $e^{it}$ est

$$
\varphi (x)(e^{it}) =\sum_{n\in\mathbf{Z}}c_ne^{int}
$$

On vérifie que $\varphi$ est un morphisme de $L^1_{\mathbf{C}}(\mathbf{Z})$ sur une algèbre A de fonctions continues sur $\mathbf{U}$, la multiplication dans A étant la multiplication usuelle. En intégrant terme à terme l’égalité

$$
(\sum_{m\in\mathbf{Z}}c_me^{imt}\cdot e^{-int}=\varphi (x)(e^{it})\cdot e^{-int}
$$

il vient

1 $\int 1it-int$

$$
c_n=\varphi (x)(e)edt
$$

$$
2\pi_0
$$

En particulier, il en découle que le morphisme $\varphi$ est injectif. L’algèbre A, munie de la norme déduite de celle de $L^1_{\mathbf{C}}(\mathbf{Z})$ par $\varphi$, s’appelle l’algèbre de Banach des séries de Fourier absolument convergentes. Elle admet pour élément unité la fonction $1 =\varphi (\varepsilon )$.

9) Soit Δ le disque des nombres complexes $z$ vérifiant $|z|\leqslant 1$. L’algèbre A des fonctions continues sur Δ analytiques dans l’intérieur de Δ (VAR, R1, p. 26, 3.2.1) est munie de la norme $\|f\|=$ sup$_{z\in\Delta}|f(z)|$. Alors A est une algèbre de Banach unifère commutative.

### 3. Rayon spectral

#### Lemme 2 (Lemme de Fekete) {#ts-i-s2-lem-2 .statement tag=025Y}

Soit $(a_n)_{n\geqslant 1}$ une suite de nombres réels. Supposons que

$$
a_{n+m}\leqslant a_n+a_m
$$

pour tout $n\geqslant 1$ et tout $m\geqslant 1$. Alors la suite $(a_n/n)_{n\geqslant 1}$ converge et vérifie

$$
a_na_n
$$

lim = inf.

$$
^{n\rightarrow+\infty}n_{n\geqslant 1}n
$$

Posons $a_0= 0$ ; l’inégalité $a_{n+m}\leqslant a_n+a_m$ reste valide pour tout $n\geqslant$ 0 et tout $m\geqslant 0$. Fixons un entier $m\geqslant$ 1. Pour tout entier $n\geqslant 1$, soient $q(n)$ et $r(n)$ les entiers tels que $n=q(n)m+r(n)$ et $0\leqslant r(n)< m$ (E, III, p. 39, th. 1). L’hypothèse implique alors

$$
a_na_{q(n)m}a_{r(n)}q(n)a_ma_{r(n)}q(n)m
$$

$\leqslant$ + $\leqslant$ + $\leqslant a_m+$.

$$
nnnnnnn
$$

Faisant tendre $n$ vers $+\infty$, on en déduit que lim sup$_n(a_n/n)\leqslant a_m/m$ puisque $q(n)/n\rightarrow 1/m$. Puisque cela vaut pour tout $m\geqslant 1$, on a donc

$$
a_na_ma_n
$$

lim sup $\leqslant$ inf $\leqslant$ lim inf.

$$
_{n\rightarrow+\infty}n_{m\geqslant 1}m_n^{\rightarrow}_+^{\infty}n
$$

Ces inégalités démontrent la convergence de la suite $(a_n/n)_{n\geqslant 1}$ ainsi que la formule lim $a_n/n=$ inf$_{n\geqslant 1}a_n/n$.

#### Proposition 1 {#ts-i-s2-prop-1 .statement tag=025Z}

Soit A une algèbre normée. Pour tout $x\in A$, la suite $(\|x^n\|^{1/n})_{n\geqslant 1}$ est convergente et sa limite $\varrho (x)$ est égale à inf$_{n\geqslant 1}\|x^n\|^{1/n}$. De plus, pour toute norme $x\mapsto  \|x\|_1$ définissant la topologie de A, on a également

$\varrho (x) =$ lim $\|x^n\|^{1/n}_1=$ inf $\|x^n\|^{1/n}_1$.

$n\rightarrow +\infty n\geqslant 1$

Si $x$ est nilpotent, on a $\|x^n\|^{1/n}_1= 0$ pour tout entier $n$ suffisamment grand et toute norme $x\mapsto  \|x\|_1$ définissant la topologie de A.

Supposons maintenant que $x$ n’est pas nilpotent, et posons $\alpha_n=$ $\|x^n\|$. On a $\alpha_n>0$ pour tout entier $n\geqslant 1$, et $\alpha_{n+m}\leqslant \alpha_n\alpha_m$ pour tous $n, m\in \mathbf{N}$ d’après (1). Le lemme 2, appliqué à la suite $a_n=$ log($\alpha_n$), montre l’existence de la limite $\varrho (x)$ et la formule $\varrho (x) =$ inf$_{n>0}\alpha_n^{1/n}$.

Soit $x\mapsto  \|x\|_1$ une norme définissant la topologie de A. Il existe des nombres réels $a >0$ et $b >0$ tels que

$$
a\|x\|\leqslant \|x\|_1\leqslant b\|x\|
$$

pour tout $x\in A$ (EVT, II, p. 7, cor. 2). Par conséquent,

$$
a^{1/n}\|x^n\|^{1/n}\leqslant \|x^n\|^{1/n}_1\leqslant b^{1/n}\|x^n\|^{1/n}
$$

pour tout $n\geqslant 1$, d’où en passant à la limite, ou en prenant la borne inférieure, l’égalité

$\varrho (x) =_{n\rightarrow}$lim$_{+\infty}\|x^n\|^{1/n}_1=$ inf$_{n>0}\|x^n\|^{1/n}_1$.

#### Définition 2 {#ts-i-s2-def-2 .statement tag=0260}

Pour tout élément $x$ d’une algèbre normée A, le nombre réel

$\varrho (x) =$ lim$_{n\rightarrow \infty}\|x^n\|^{1/n}=$ inf$_{n>0}\|x^n\|^{1/n}$

est appelé le rayon spectral de $x$.

Pour tout élément $x$ de A, on a

$$
\varrho (x)\leqslant \|x\| \tag{3}
$$

(4) $\varrho (x^n) =\varrho (x)^n$, pour tout entier $n\geqslant 1$.

#### Définition 3 {#ts-i-s2-def-3 .statement tag=0261}

Un élément $x$ de A est quasi-nilpotent si $\varrho (x) = 0$.

Ceci revient à dire que, quel que soit $\lambda \in K$, les nombres $\|(\lambda x)^n\|$ sont bornés pour $n\geqslant 1$ ; ou encore que, quel que soit $\lambda \in K$, la suite $(\lambda x)^n$ tend vers 0 quand $n\rightarrow +\infty$.

#### Remarque 1 {#ts-i-s2-n3-rem-1 .statement tag=0262}

Soit A une algèbre normée. Si un élément $x\in A$ vérifie $\varrho (x) =\|x\|$, on a $\|x^n\|=\|x\|^n$ pour tout $n\in \mathbf{N}$, d’après (3) et (4).

Inversement, supposons que $\|x^2\|=\|x\|^2$ pour tout $x\in A$. Alors on a, pour tout entier $n\geqslant 0$, l’égalité $\|x^{2^n}\|=\|x\|^{2^n}$, donc $\|x\|=$ $\|x^{2^n}\|^{2^{-n}}$; quand $n$ tend vers $+\infty$, on obtient $\|x\|=\varrho (x)$.

#### Remarque 2 {#ts-i-s2-n3-rem-2 .statement tag=0263}

La fonction $x\mapsto \varrho (x)$ sur A, étant l’enveloppe inférieure des fonctions continues $x\mapsto  \|x^n\|^{1/n}$ pour $n\geqslant 1$, est semi-continue supérieurement (TG, IV, p. 31, cor.), mais en général elle n’est pas continue. Il peut même arriver (cf. exerc. 12 de I, p. 157) qu’une suite d’éléments nilpotents de A tende vers un élément qui n’est pas quasi-nilpotent.

### 4. Inverses

Soit A une algèbre de Banach unifère, dont on note 1 l’élément unité. Rappelons (TG, IX, prop. 14, p. 40) que le groupe G des éléments inversibles de A est une partie ouverte de A, que la topologie induite sur G par celle de A est compatible avec la structure de groupe et que le groupe topologique G est complet.

#### Proposition 2 {#ts-i-s2-prop-2 .statement tag=0264}

Soient A une algèbre de Banach et $x$ un élément de A. La série $\sum_{n=1}^{\infty}\lambda^nx^n$, considérée comme série entière en $\lambda$, a pour rayon de convergence $\varrho (x)^{-1}$. Si A est unifère et si $\varrho (x)<1$, alors $1-x$ est inversible et a pour inverse $\sum_{n=0}^{\infty}x^n$.

La série $\sum^{\infty}_{n=1}\lambda^nx^n$ a pour rayon de convergence

(lim sup$\|x^n\|^{1/n})^{-1}=\varrho (x)^{-1}$

$n\rightarrow +\infty$

(cf. VAR, R1, p. 23, 3.1.4). Supposons que A admette un élément

unité. Si $\varrho (x)<1$, la série $\sum_{n=0}^{\infty}x^n$ est donc absolument convergente.

Comme

$(1-x)\sum_{n=0}^kx^n$ = $\sum_{n=0}^kx^n(1-x) = 1-x^{k+1}$

pour tout entier $k\geqslant 0$, l’élément $1-x$ est inversible et son inverse est

égal à $\sum_{n=0}^{\infty}x^n$.

#### Corollaire 1 {#ts-i-s2-prop-2-cor-1 .statement tag=0265}

Si A est une algèbre de Banach unifère, alors le groupe des éléments inversibles de A contient la boule ouverte de centre 1 et de rayon 1.

C’est immédiat puisque $\|x\|<1$ implique $\varrho (x)<1$.

#### Corollaire 2 {#ts-i-s2-prop-2-cor-2 .statement tag=0266}

Soient A une algèbre de Banach et I un idéal à gauche (resp. à droite) maximal régulier de A. Alors I est fermé.

Soit $(\widetilde{A}, e)$ l’algèbre de Banach unifère déduite de A par adjonction d’un élément unité. Il existe un idéal à gauche (resp. à droite) maximal J de $\widetilde{A}$ tel que $J\cap A = I$ (A, VIII, p. 428, prop. 4). Alors J est disjoint de la boule ouverte de centre $e$ et de rayon 1 (cor. 1), et donc $\overline{J}\not=\widetilde{A}$. Comme J est un idéal maximal, cela implique que J = J, et par suite que $I = J\cap A = J\cap A$ est fermé dans A.

#### Corollaire 3 {#ts-i-s2-prop-2-cor-3 .statement tag=0267}

Le radical d’une algèbre de Banach est fermé.

En effet le radical est l’intersection des idéaux à gauche maximaux réguliers (A, VIII, p. 430, déf. 3).

#### Proposition 3 {#ts-i-s2-prop-3 .statement tag=0268}

Soit A une algèbre de Banach unifère.

a) Si $x\in A$ admet un inverse à gauche (resp. à droite) $y$, tout élément $x'\in A$ tel que $\|x'-x\|<\|y\|^{-1}$ admet un inverse à gauche (resp. à droite).

b) L’ensemble des éléments de A qui sont inversibles (resp. à gauche, resp. à droite) est ouvert dans A.

c) Soit $(x_n)$ une suite d’éléments de A admettant des inverses à gauche (resp. à droite$)y_n$, et convergeant vers un élément $x\in A$. Si la suite $(y_n)$ est bornée, alors $x$ est inversible à gauche (resp. à droite).

Il suffit de traiter le cas des inverses à gauche ; celui des inverses à droite en découle en considérant l’algèbre opposée.

Soient $x, y, x'\in A$ tels que $yx= 1$ et $\|x'-x\|<\|y\|^{-1}$. On a

$$
\|1-yx'\|=\|yx-yx'\|\leqslant \|y\| \cdot  \|x-x'\|<1
$$

donc $yx'$ est inversible : il existe $z\in$ A tel que $z(yx') = 1$. Ainsi l’élément $x'$ est inversible à gauche d’inverse $zy$. Cela démontre l’assertion a) et l’assertion b) en résulte immédiatement.

Soit $(x_n)$ une suite d’éléments de A admettant des inverses à gauche $y_n$, qui converge vers un élément $x\in$ A, et telle que la suite $(y_n)$ est bornée. Si $M\geqslant 1$ est un nombre réel tel que $\|y_n\|\leqslant M$ pour tout $n\geqslant 1$, alors on a $\|x_n-x\|<M^{-1}\leqslant \|y_n\|^{-1}$ pour $n$ assez grand, et donc $x$ admet un inverse à gauche d’après a).

#### Définition 4 {#ts-i-s2-def-4 .statement tag=0269}

Soit A une algèbre normée, soit $x$ un élément de A. Notons $\boldsymbol{\gamma }_x$ et $\boldsymbol{\delta }_x$ les applications $y\mapsto xy$ et $y\mapsto yx$ de A dans A. On dit que $x$ est un diviseur de zéro topologique à gauche (resp. à droite) si $\boldsymbol{\gamma }_x($resp. $\boldsymbol{\delta }_x)$ n’est pas un homéomorphisme de A sur $\boldsymbol{\gamma }_x(A)$ (resp. sur $\boldsymbol{\delta }_x(A)$).

#### Remarque {#ts-i-s2-n4-rem-1 .statement tag=026A}

D’après TG, IX, p. 36, cor. $2,x$ est un diviseur de zéro topologique à gauche (resp. à droite) si et seulement si il existe une suite $(z_n)$ dans A telle que $\|z_n\|= 1$ et telle que $xz_n$ tende vers 0 (resp. que $z_nx$ tende vers 0) quand $n\rightarrow +\infty$.

Un diviseur de zéro à gauche (resp. à droite) est un diviseur de zéro topologique à gauche (resp. à droite). Supposons que A est non nulle et unifère. Un diviseur de zéro topologique à gauche (resp. à droite) $x$ n’est pas inversible à gauche (resp. à droite). En effet, si par exemple $yx= 1$ et si $xz_n$ tend vers 0, alors $z_n=y(xz_n)$ tend vers 0 et on ne peut avoir $\|z_n\|= 1$ pour tout $n$.

#### Proposition 4 {#ts-i-s2-prop-4 .statement tag=026B}

Soit A une algèbre de Banach unifère. Soit $x$ un élément de A qui n’est pas inversible à gauche. S’il existe une suite $(x_n)$ d’éléments inversibles à gauche de A qui converge vers $x$, alors $x$ est un diviseur de zéro topologique à droite.

Soit $y_n$ un inverse à gauche de $x_n$. D’après la prop. 3 (ii), $\|y_n\|$ tend vers $+\infty$. Soit $z_n=\|y_n\|^{-1}y_n$. On a $\|z_n\|= 1$, et $z_nx_n=\|y_n\|^{-1}$ tend vers 0, donc $z_nx=z_nx_n+z_n(x-x_n)$ tend vers 0. On conclut alors à l’aide de la remarque suivant la définition 4.

#### Proposition 5 {#ts-i-s2-prop-5 .statement tag=026C}

Soit A une algèbre de Banach unifère et soit B une sous-algèbre pleine de A. Alors B est une sous-algèbre pleine de A.

En effet, soient $x$ un élément de $\overline{B}$ inversible dans A, et $(x_n)$ une suite d’éléments de B tendant vers $x$. Alors, pour $n$ assez grand, $x_n$ est inversible dans A et $x^{-1}_n$ tend vers $x^{-1}$. Puisque la sous-algèbre B est pleine, on a $x^{-1}_n\in B$, d’où $x^{-1}\in B$.

Soit A est une algèbre de Banach unifère et soit $(y_i)_{i\in I}$ une famille d’éléments de A. Soit B la sous-algèbre pleine de A engendrée par les éléments $y_i$. Alors $\overline{B}$ est la plus petite sous-algèbre pleine fermée de A contenant les $y_i$. On l’appelle la sous-algèbre pleine fermée engendrée par les éléments $y_i$.

### 5. Spectre d’un élément dans une algèbre normée

Dans ce numéro, on suppose que $K =\mathbf{C}$.

#### Théorème 1 {#ts-i-s2-thm-1 .statement tag=026D}

Soient A une algèbre de Banach unifère et $x\in A$.

a) L’ensemble Sp$_A(x)$ est une partie compacte de $\mathbf{C}$;

b) Le rayon spectral $\varrho (x)$ est le rayon du plus petit disque fermé de centre 0 dans $\mathbf{C}$ qui contient Sp$_A(x)$ ;

c) La résolvante $\lambda \mapsto R(x, \lambda ) = (\lambda -x)^{-1}$ de $x$ est holomorphe dans $\mathbf{C}-$ Sp$_A(x)$ et nulle à l’infini. De plus, pour tout entier $k\geqslant 0$, on a la formule

$\partial kkk+1$

$R(x, \lambda ) = (-1)k$! $R(x, \lambda )$ ;

$$
\partial \lambda^k
$$

d) Pour tout nombre complexe $\lambda$ tel que $|\lambda |>1/\varrho (x)$, on a

$$
R(x, \lambda ) =\sum_{n=0}^{+\infty}\lambda^{-n-1}x^n
$$

Le complémentaire du spectre Sp$_A(x)$ est l’image réciproque du groupe G des éléments inversibles de A par l’application continue $\lambda \mapsto$ $x-\lambda$ de $\mathbf{C}$ dans A ; d’après la proposition 3, b) de I, p. 23, le spectre Sp$_A(x)$ est une partie fermée de $\mathbf{C}$. Par ailleurs, soit $\lambda \in \mathbf{C}$ tel que $|\lambda |> \varrho (x)$. On a $\lambda -x=\lambda (1-\lambda^{-1}x)$. Puisque $\varrho (\lambda^{-1}x) =|\lambda |^{-1}\varrho (x)<1$, l’élément $1-\lambda^{-1}x$, donc également l’élément $\lambda -x$, est inversible et

$$
R(x, \lambda ) = (\lambda -x)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n \tag{5}
$$

(I, p. 22, prop. 2). En particulier, $\lambda \notin$ Sp$_A(x)$. Cela démontre que Sp$_A(x)$ est contenu dans le disque de centre 0 et de rayon $\varrho (x)$. Par suite, Sp$_A(x)$ est compact. Cette formule (5) prouve aussi que la résolvante de $x$ est définie et holomorphe dans le complémentaire du disque fermé $\Delta_{\varrho(x)}$ de centre 0 et de rayon $\varrho (x)$, et tend vers 0 à l’infini.

Soit $\lambda_0\in \mathbf{C}-$ Sp$_A(x)$. Posons $y=\lambda_0-x$. Soit $\mu\in \mathbf{C}$ tel que $|\lambda_0-\mu|<\|y^{-1}\|^{-1}$. On a

$$
\mu-x=y-(\lambda_0-\mu) =y(1-(\lambda_0-\mu)y^{-1})
$$

donc $\mu-x$ est inversible et a pour inverse

$$
(\mu-x)^{-1}=y^{-1}\sum_{n=0}^{\infty}(\lambda_0-\mu)^ny^{-n} \tag{6}
$$

d’après la prop. 2 de I, p. 22. Donc la résolvante de $x$ est définie et holomorphe dans le disque ouvert de centre $\lambda_0$ et de rayon $\|y^{-1}\|^{-1}$. Par suite, la résolvante de $x$ est une application holomorphe de $\mathbf{C}-$ Sp$_A(x)$ dans A.

La formule (1) de I, p. 4 implique $\frac{\partial}{\partial \lambda}R(x, \lambda ) =-R(x, \lambda )^2$, d’où, par récurrence sur $k$,

$\partial kkk+1$

$R(x, \lambda ) = (-1)k$! $R(x, \lambda )$.

$$
\partial \lambda^k
$$

Soit $a >0$ un nombre réel tel que Sp$_A(x)$ soit contenu dans le disque fermé $\Delta_a$ de centre 0 et de rayon $a$. La fonction $\lambda \mapsto (\lambda^{-1}-x)^{-1}$ est alors définie et holomorphe pour $0<|\lambda |< a^{-1}$ et tend vers 0 quand $\lambda$ tend vers 0. L’unique fonction continue sur le disque ouvert de centre 0 et de rayon $a^{-1}$ qui prolonge cette fonction holomorphe est alors holomorphe (VAR, R1, 3.3.9), donc le rayon de convergence de la série (5) qui la définit est $\geqslant a^{-1}$ (VAR, R1, 3.2.9). D’après la prop. 2 de I, p. 22, on a donc $a\geqslant \varrho (x)$.

#### Remarque 1 {#ts-i-s2-n5-rem-1 .statement tag=026E}

Le spectre d’un élément dans une algèbre de Banach unifère peut être une partie compacte non vide F quelconque de $\mathbf{C}($cf. exemple 3 de I, p. 17 ; pour $A =\mathscr{C}(F;\mathbf{C})$ et $f\in A$ l’inclusion canonique de F dans $\mathbf{C}$, on a Sp$_A(f) = F$).

#### Remarque 2 {#ts-i-s2-n5-rem-2 .statement tag=026F}

Soit A une algèbre de Banach unifère et soit $x\in A$. D’après le théorème 1 de I, p. 24$,\mathbf{C}-$ Sp$_A(x)$ est une partie ouverte de $\mathbf{C}$, donc est localement connexe. Donc les composantes connexes de $\mathbf{C}-$ Sp$_A(x)$ sont ouvertes. D’après le th. 1, l’une de ces composantes connexes contient l’ensemble des $\lambda \in \mathbf{C}$ tels que $|\lambda |> \varrho (x)$ ; toutes les autres composantes connexes sont donc bornées.

#### Corollaire 1 {#ts-i-s2-thm-1-cor-1 .statement tag=026G}

Soit A une algèbre normée unifère non nulle. Pour tout $x\in A$, le spectre Sp$_A(x)$ est non vide.

Supposons d’abord A complète. Si l’on avait Sp($x$) $=\emptyset$, la résolvante de $x$ serait holomorphe dans $\mathbf{C}$ et nulle à l’infini, donc identiquement nulle (VAR, R., 3.3.6, p. 29). Comme $R(x, \lambda ) = (\lambda -x)^{-1}$ est inversible, il en résulterait que 1 = 0 et donc que $A =\{0\}$.

Dans le cas général, soit $\widehat{A}$ l’algèbre compétée de A ; la relation Sp$_A(x) =\emptyset$ entraînerait Sp$_{\widehat{A}}(x) =\emptyset$, d’où $\widehat{A} =\{0\}$ et $A =\{0\}$.

#### Corollaire 2 (Théorème de Gelfand-Mazur) {#ts-i-s2-thm-1-cor-2 .statement tag=026H}

Soit A une algèbre normée sur $\mathbf{C}$. Si A est un corps, alors $A =\mathbf{C}\cdot 1$.

Si $x\in A$, il existe $\lambda \in \mathbf{C}$ tel que $x-\lambda$ soit non inversible (cor. 1), d’où $x-\lambda = 0$ et $x\in \mathbf{C}\cdot 1$.

#### Corollaire 3 {#ts-i-s2-thm-1-cor-3 .statement tag=026I}

Soient A une algèbre de Banach unifère et $x$ un élément inversible de A tel que $\|x\|=\|x^{-1}\|= 1$. Alors Sp($x$)$\subset \mathbf{U}$.

Soit Δ le disque de centre 0 et de rayon 1 dans $\mathbf{C}$. D’après le th. 1 b) et le fait que $\varrho (x)\leqslant \|x\|$, on a Sp($x$)$\subset \Delta$. De même, Sp($x$)$^{-1}$ = Sp($x^{-1}$)$\subset \Delta$, d’où le corollaire (cf. I, p. 2, remarque 4).

#### Corollaire 4 {#ts-i-s2-thm-1-cor-4 .statement tag=026J}

Soient E un espace de Banach complexe, $\mathscr{L}(E)$ l’algèbre de Banach des endomorphismes continus de E et A une sous-algèbre non nulle de $\mathscr{L}(E)$ telle que E soit un A-pseudomodule (A, II, p. 176, Appendice) simple.

a) Soit $u$ un endomorphisme de E, non nécessairement continu, qui commute avec A. Alors $u$ est une homothétie ;

b) Soit $u$ un endomorphisme de E, non nécessairement continu. Pour tout entier $n\geqslant 1$ et pour tout $(\xi_1, . . . , \xi_n)\in E^n$, il existe $v\in A$ tel que

$$
(v(\xi_1), . . . , v(\xi_n)) = (u(\xi_1), . . . , u(\xi_n))
$$

Montrons a). Soit $\widetilde{A}$ l’algèbre obtenue à partie de A par adjonction d’un élément unité. Puisque E est un A-pseudomodule simple, c’est un $\widetilde{A}$-module simple.

Soit B le commutant de $\widetilde{A}$ dans l’anneau des endomorphismes du $\mathbf{C}$-espace vectoriel E. L’algèbre B contient 1 et est l’algèbre des endomorphismes du $\widetilde{A}$-module E. Comme E est un $\widetilde{A}$-module simple, le lemme de Schur (A, VIII, p. 43, corollaire), montre que B est un corps.

Soit $\xi_0\in E$ tel que $A\xi_0\not=\{0\}$. On a donc $A\xi_0= E$. Pour tout $u\in B$, soit $A_u$ l’ensemble des $v\in A$ tels que $v(\xi_0) =u(\xi_0)$. Cet ensemble est non vide, puisque $A\xi_0= E$. On pose alors

$\|u\|_B=$ inf$_{v\in A_u}\|v\|$.

L’application $u\mapsto  \|u\|_B$ est une seminorme sur B.

Montrons que cette application est une norme. Soit $u$ un élément non nul de B. Pour tout $v\in A_u$, on a $\|v\|\geqslant \|v(\xi_0)\|/\|\xi_0\|=\|u(\xi_0)\|/\|\xi_0\|$, de sorte que $\|u\|_B\geqslant \|u(\xi_0)\|/\|\xi_0\|$. Il suffit donc de démontrer que $u(\xi_0)\not= 0$. Soit $\xi_1\in E$ tel que $u(\xi_1)\not= 0$. Comme $A\xi_0= E$, il existe $w\in A$ tel que $\xi_1=w(\xi_0)$. Alors, $wu(\xi_0) =uw(\xi_0) =u(\xi_1)\not= 0$, donc $u(\xi_0)\not= 0$.

D’autre part, soient $u$ et $u'$ des éléments de B. Pour tout $\varepsilon  >0$, il existe $v, v'\in A$ tels que $v(\xi_0) =u(\xi_0),v'(\xi_0) =u'(\xi_0)$ et $\|v\|\leqslant \|u\|_B+\varepsilon$, $\|v'\|\leqslant \|u'\|_B+\varepsilon$. Alors on a $vv'(\xi_0) =vu'(\xi_0) =u'v(\xi_0) =u'u(\xi_0)$, d’où

$$
\|u'u\|_B\leqslant \|v'v\|\leqslant \|v\|\|v'\|\leqslant (\|u\|_B+\varepsilon )(\|u'\|_B+\varepsilon )
$$

et finalement $\|u'u\|_B\leqslant \|u\|_B\|u'\|_B$. Cela montre que B, muni de la norme $u\mapsto  \|u\|_B$, est une algèbre normée. Comme c’est un corps, le corollaire 2 implique que $B =\mathbf{C}\cdot 1$, ce qui est la conclusion désirée.

Démontrons b). D’après a), le commutant de A dans End$_{\mathbf{C}}(E)$ est réduit aux homothéties de E. Son bicommutant est donc End$_{\mathbf{C}}(E)$. L’assertion b) résulte donc du théorème de densité de Jacobson (théo-rème 1 de A, VIII, p. 434).

#### Corollaire 5 {#ts-i-s2-thm-1-cor-5 .statement tag=026K}

Soient A une algèbre de Banach et $x\in A$.

a) Sp$'(x)$ est une partie compacte de $\mathbf{C}$;

b) Le rayon spectral $\varrho (x)$ est le rayon du plus petit disque fermé de centre 0 de $\mathbf{C}$ qui contient Sp$'(x)$ ;

c) Pour que $x$ soit quasi-nilpotent, il faut et il suffit que l’on ait Sp$'(x) =\{0\}$.

Les assertions a) et b) résultent du th. 1 en considérant l’algèbre de Banach déduite de A par adjonction d’un élément unité. L’assertion c) résulte de b).

### 6. Spectre relatif à une sous-algèbre

Dans ce numéro, on suppose que $K =\mathbf{C}$.

#### Lemme 3 {#ts-i-s2-lem-3 .statement tag=026L}

Soient $X_1$ et $X_2$ des sous-ensembles compacts de $\mathbf{C}$. Si $X_2$ est contenu dans $X_1$ et si la frontière de $X_1$ dans $\mathbf{C}$ est contenue dans $X_2$, alors $X_1$ est la réunion de $X_2$ et de certaines composantes connexes bornées du complémentaire de $X_2$ dans $\mathbf{C}$.

Soit U une composante connexe de $\mathbf{C}-X_2$. Tout point frontière de $X_1\cap U$ dans l’ouvert U est aussi point frontière de $X_1$ dans $\mathbf{C}$, donc appartient à $X_2$ par hypothèse ; comme $U\cap X_2=\emptyset$, on voit que $X_1\cap U$ n’a aucun point frontière dans l’espace U. Comme U est connexe, l’intersection $X_1\cap U$ est soit vide, soit égale à U (TG, I, p. 82, cor.), et le lemme en résulte.

#### Proposition 6 {#ts-i-s2-prop-6 .statement tag=026M}

Soient A une algèbre de Banach unifère et B une sous-algèbre unifère fermée de A. Pour tout $x\in B$, on a Sp$_B(x)\supset$ Sp$_A(x)$, et la frontière de Sp$_A(x)$ dans $\mathbf{C}$ contient la frontière de Sp$_B(x)$ dans $\mathbf{C}$. En particulier, si Sp$_B(x)\subset \mathbf{R}$, alors on a Sp$_B(x) =$ Sp$_A(x)$.

On a Sp$_B(x)\supset$ Sp$_A(x)$ (remarque 6 de I, p. 3). Si $\lambda$ est un point de la frontière de Sp$_B(x)$ dans $\mathbf{C}$, il existe une suite $(\lambda_n)$ de points extérieurs à Sp$_B(x)$ tendant vers $\lambda$. Alors $x-\lambda_n$ est inversible dans B et tend vers $x-\lambda$, qui n’est pas inversible dans B; donc $x-\lambda$ est diviseur de zéro topologique à gauche ou à droite dans B (prop. 4 de I, p. 24), donc dans A. Ainsi, $\lambda \in$ Sp$_A(x)$. Mais puisque Sp$_A(x)\subset$ Sp$_B(x)$, le nombre complexe $\lambda \in$ Fr$_{\mathbf{C}}$(Sp$_B(x))$ ne peut être intérieur à Sp$_A(x)$, donc appartient à sa frontière.

#### Corollaire {#ts-i-s2-n6-cor-1 .statement tag=026N}

L’ensemble Sp$_B(x)$ est la réunion de Sp$_A(x)$ et de certaines composantes connexes bornées de $\mathbf{C}-$ Sp$_A(x)$.

Cela découle de la prop. 6 et du lemme 3.

Ce corollaire sera complété par les propositions 13 de I, p. 46 et 14 de I, p. 46.

## EXERCICES {#ts-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
