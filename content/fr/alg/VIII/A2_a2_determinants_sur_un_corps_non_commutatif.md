---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 2
section_title: Déterminants sur un corps non commutatif
appendix: true
lang: fr
source: alg-viii-fr
book_pages: A VIII.437-A VIII.449
pdf_pages: 0439-0451
extraction: native
subsections:
    - "no": 1
      title: Une généralisation des formes multilinéaires alternées
      page: 437
      pdf_page: 439
    - "no": 2
      title: Un théorème d’unicité
      page: 438
      pdf_page: 440
    - "no": 3
      title: Déterminant d’un automorphisme
      page: 441
      pdf_page: 443
    - "no": 4
      title: Déterminant d’une matrice carrée
      page: 442
      pdf_page: 444
    - "no": 5
      title: Le groupe unimodulaire
      page: 445
      pdf_page: 447
statements: 18
exercises: 4
content_sha256: 7c5b5108718dd1876d11c57f837b6d263675472290159fad6f7007f100a07326
---

### APPENDICE 2 DÉTERMINANTS SUR UN CORPS NON COMMUTATIF

Dans cet appendice, la lettre D désigne un corps et $D^*_{ab}$ le quotient du groupe multiplicatif $D^*$ de D par son sous-groupe dérivé (I, p. 67). Le groupe $D^*_{ab}$ est commutatif et $D^*_{ab}$ s’identifie à $D^*$ si le corps D est commutatif. On note $\pi$ l’homomorphisme canonique de $D^*$ sur $D^*_{ab}$.

### 1. Une généralisation des formes multilinéaires alternées

Soit V un espace vectoriel à droite sur le corps D, de dimension finie $n\geqslant 0$. On note B(V) l’ensemble des bases de V et Ω(V) l’ensemble des applications $\omega$ de B(V) dans $D^*_{ab}$ qui satisfont aux deux conditions suivantes :

a) Si $\lambda_1, . . . , \lambda_n$ sont des éléments de $D^*$, on a

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\pi (\lambda_1. . . \lambda_n)\omega (v_1, . . . , v_n) \tag{1}
$$

pour toute base $(v_1, . . . , v_n)$de V.

b) Si $i$ et $j$ sont deux entiers distincts de l’intervalle $[1, n]$, on a

$$
\omega (v_1, . . . , v_{i-1}, v_i+v_j, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_n) \tag{2}
$$

pour toute base $(v_1, . . . , v_n)$de V.

Soit $\omega$ un élément de Ω(V). Soient $(v_1, . . . , v_n)$ une base de V et $i$ un entier de l’intervalle $[1, n-1]$; d’après la propriété b), on a

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}, . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}-(v_i+v_{i+1}), . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1},-v_i, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i+v_{i+1})-v_i,-v_i, . . . , v_n)
$$

d’où finalement

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\pi (-1)\omega (v_1, . . . , v_{i+1}, v_i, . . . , v_n) \tag{3}
$$

Comme le groupe symétrique $\mathfrak{S}_n$ est engendré par les transpositions de deux éléments consécutifs de l’intervalle $[1, n]$ (I, p. 61, prop. 9), la formule (3) se généralise en

$$
\omega (v_{\sigma(1)}, . . . , v_{\sigma(n)}) =\pi (\varepsilon (\sigma ))\omega (v_1, . . . , v_n) \tag{4}
$$

où $\sigma$ appartient à $\mathfrak{S}_n$ et $\varepsilon (\sigma )$ désigne sa signature (I, p. 62).

La formule (2) se généralise comme suit. Tout d’abord, pour tout $\lambda$ dans $D^*$, on a

$$
\omega (v_1, . . . , v_n) =\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}, . . . , v_n)
$$

$$
=\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}+v_j, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i\lambda^{-1}+v_j)\lambda , . . . , v_n)
$$

c’est-à-dire

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+v_j\lambda , . . . , v_n) \tag{5}
$$

Par une récurrence immédiate, on en déduit

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+w, . . . , v_n) \tag{6}
$$

pour toute combinaison linéaire $w=\sum_{j\not=i}v_j\lambda_j$ des vecteurs $v_j$ pour $j$ distinct de $i$ dans l’intervalle $[1, n]$.

### 2. Un théorème d’unicité

Dans ce numéro, pour tout entier strictement positif $m$, tout entier $i$ de l’intervalle $[1, m]$ et toute suite $(v_1, . . . , v_m)$ de $V^m$, on notera $(v_1, . . . ,\widehat{v}_i, . . . , v_m)$ la suite $(v_1, . . . , v_{i-1}, v_{i+1}, . . . , v_m)$ de $V^{m-1}$.

#### Proposition 1 {#alg-viii-a2-prop-1 .statement tag=00Q1}

Soient W un hyperplan de V et $e$ un vecteur de V W. Soit $\varphi$ un élément de Ω(W). Il existe un élément $\omega$ de Ω(V), et un seul, tel que l’on ait (7) $\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1})$

pour toute base de $(w_1, . . . , w_{n-1})$de W.

A) Unicité de $\omega :$ Soit $\omega$ un élément de Ω(V). Soit $(v_1, . . . , v_n)$ une base de V, et soient $\mu_1, . . . , \mu_n$ les coordonnées de $e$ dans cette base. Désignons par I l’ensemble des entiers compris entre 1 et $n$ tels que $\mu_i\not= 0$; il n’est pas vide. Soit $i$ un élément de I ; la suite $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ est une base de V et, comme $e-v_i\mu_i$ est combinaison linéaire de la suite $(v_1, . . . ,\widehat{v}_i, . . . , v_n)$, la formule (6) entraîne

$$
\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, v_i\mu_i) =\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, e) \tag{8}
$$

Il résulte des formules (1) et (3) que le premier membre de cet égalité est égal à $\pi (-1)^{n-i}\pi (\mu_i)\omega (v_1, . . . , v_n)$. Notons $p$ le projecteur de V d’image W et de noyau $eD$. Les vecteurs $v_j-p(v_j)$ sont proportionnels à $e$, et une application répétée de la formule (6) montre que le second membre de la formule (8) est égal à $\omega (p(v_1), . . . ,p(\widehat{v}_i), . . . , p(v_n), e)$.

De tout ceci il résulte que si $\omega$ satisfait à la relation (7), on a

$$
\omega (v_1, . . . , v_n) =\pi (-1)_{n-i}\pi (\mu_i)_{-1}\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . , p(v_n)) \tag{9}
$$

pour tout $i$ dans I ce qui prouve l’unicité de $\omega$.

B) Construction de $\omega :$ Soit $(v_1, . . . , v_n)$ une base de V ; on définit $\mu_1, . . . , \mu_n$ et I comme ci-dessus. Pour tout $i$ dans I, l’hypothèse $\mu_i\not= 0$ entraîne que la suite $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ engendre l’espace V, donc la suite $(p(v_1), . . . ,p(\widehat{v}_i), . . . , p(v_n))$ engendre l’espace $W =p(V)$. Autrement dit, cette dernière suite est une base de W, et l’on peut définir l’élément

$$
t_i=\pi (-1)_n^-_i\pi (\mu_i)^-_1\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . , p(v_n)) \tag{10}
$$

de $D^*_{ab}$.

Soient $i$ et $j$ deux éléments de I tels que $i < j$; démontrons l’égalité $t_i=t_j$. Par définition, le vecteur $v_i\mu_i+v_j\mu_j-e$ est combinaison linéaire des vecteurs $p(v_k)$ pour $k$ distinct de $i$ et $j$; par suite $p(v_i)\mu_i+p(v_j)\mu_j$ est combinaison linéaire des vecteurs $p(v_k)$ pour $k$ distinct de $i$ et $j$. D’après la formule (6), on a donc

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n), p(v_i)\mu_i)
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . ,p(\widehat{v}_j), . . . , p(v_n),-p(v_j)\mu_j)
$$

Par application des formules (1) et (3), on en déduit

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))\pi (\mu_i)\pi (-1)_{n-i-1}
$$

$$
=\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . , p(v_n))\pi (-\mu_j)\pi (-1)_{n-j}
$$

d’où $t_i=t_j$.

Ceci étant prouvé, on définit $\omega (v_1, . . . , v_n)$ comme la valeur commune des $t_i$ pour $i$ parcourant I. On a ainsi construit une application $\omega$ de B(V) dans $D^*_{ab}$ qui satisfait à la relation (9). Soit $(w_1, . . . , w_{n-1})$ une base de W ; si l’on pose $v_i=w_i$ pour $1\leqslant i\leqslant n-1$ et $v_n=e$, on a $I =\{n\}$ et $\mu_n= 1$; on a par ailleurs $p(v_i) =w_i$ pour $1\leqslant i\leqslant n-1$ et la formule $\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1})$ est un cas particulier de (9).

Il s’agit maintenant de prouver que $\omega$ appartient à Ω(V).

C) Preuve de la formule (1) : Soient $\lambda_1, . . . , \lambda_n$ des éléments de $D^*$ et $(v_1, . . . , v_n)$ une base de V. On définit $\mu_1, . . . , \mu_n$ et I comme ci-dessus ; choisissons $i$ dans I. Comme on a $e=\sum^n_{j=1}(v_j\lambda_j)(\lambda^-_j^1\mu_j)$, la formule (9) entraîne

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\pi (-1)_{n-i}\pi (\lambda_{-i1}\mu_i)_{-1}\varphi (p(v_1)\lambda_1, . . . ,p(v_i)\widehat{\lambda}_i, . . . , p(v_n)\lambda_n) \tag{11}
$$

Mais on a $\pi (\lambda^-_i^1\mu_i)^{-1}=\pi (\mu_i)^{-1}\pi (\lambda_i)$ et

$$
\varphi (p(v_1)\lambda_1, . . . ,p(v_i)\widehat{\lambda}_i, . . . , p(v_n)\lambda_n)
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))\pi (\lambda_1. . .\widehat{\lambda}_i. . . \lambda_n)
$$

la comparaison des formules (9) et (11) établit la relation cherchée

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\omega (v_1, . . . , v_n)\pi (\lambda_1. . . \lambda_n)
$$

D) Preuve de la formule (2) : Soient $(v_1, . . . , v_n)$ une base de V et $i, j$ deux entiers distincts dans l’intervalle $[1, n]$; définissons$\mu_1, . . . , \mu_n$ comme précédemment. Considérons la base $(v_1', . . . , v'_n)$ de V définie par $v_i'=v_i+v_j$ et $v'_k=v_k$ pour $k\not=i$, et introduisons les coordonnées $\mu '_1, . . . , \mu '_n$ de $e$ par rapport à cette base ; elles satisfont à $\mu '_j=\mu_j-\mu_i$ et $\mu '_k=\mu_k$ pour $k\not=j$. On pose $t=\omega (v_1, . . . , v_n)$ et $t'=\omega (v'_1, . . . , v_n')$. Il s’agit de prouver l’égalité de $t$ et $t'$.

Remarquons d’abord que, par définition de $\omega$, on a

$$
t=\pi (-1)_{n-k}\pi (\mu_k)_{-1}\varphi (p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n)) \tag{12}
$$

$$
t_'=\pi (-1)_{n-k}\pi (\mu_{'k})_{-1}\varphi (p(v_{1'}), . . . ,p(\widehat{v}_{'k}), . . . , p(v_{'n})) \tag{13}
$$

pour tout $k$ tel que $\mu_k$ et $\mu '_k$ soient non nuls.

a) Si $\mu_i\not=0$, les suites $(p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n))$ et $(p(v_{'1}), . . . ,p(\widehat{v}_{'k}), . . . , p(v_{'n}))$

sont égales et l’on a $\mu_i=\mu '_i$, d’où $t=t'$.

b) S’il existe un indice $k$, distinct de $i$ et de $j$, tel que $\mu_k\not= 0$, on a $p(v_l') =p(v_l)$ pour $l\not=i$ et $p(v_i') =p(v_i) +p(v_j)$; les éléments $p(v_i)$ et $p(v_j)$ appartiennent tous les deux à la suite $(p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n))$. Comme $\varphi$ appartient à Ω(W) la formule (2) de VIII, p. 437 s’applique et donne

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n)) =\varphi (p(v_1'), . . . ,p(\widehat{v}_{'k}), . . . , p(v'_n))
$$

Mais on a aussi $\mu_k=\mu '_k$, d’où $t=t'$.

c) Il reste à examiner le cas où le seul indice $k$ tel que $\mu_k\not= 0$ est $j$. On a alors $\mu '_j=\mu_j,e=v_j\mu_j$ et $p(v_j) = 0$. Faisons $k=j$ dans les formules (12) et (13). Comme les suites $(p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))$ et $(p(v_{'1}), . . . ,p(\widehat{v}_{j'}), . . . , p(v_{n'}))$ sont égales, on

a $t=t'$.

#### Corollaire 1 {#alg-viii-a2-prop-1-cor-1 .statement tag=00Q2}

Soient $(e_1, . . . , e_n)$une base de V et $t$ un élément de $D^*_{ab}$. Il existe un élément $\omega$ de Ω(V), et un seul, tel que $\omega (e_1, . . . , e_n) =t$.

Démontrons le corollaire par récurrence sur $n$. Si $n= 0, V$ admet pour seule base la base vide, de sorte que l’assertion est vérifiée. Supposons donc $n\geqslant 1$; notons W le sous-espace de V engendré par $e_1, . . . , e_{n-1}$. D’après la prop. 1, il existe une bijection Λ de Ω(V) sur Ω(W) satisfaisant à

$$
(\Lambda (\omega ))(w_1, . . . , w_{n-1}) =\omega (w_1, . . . , w_{n-1}, e_n)
$$

pour toute base $(w_1, . . . , w_{n-1})$ de W et tout $\omega$ dans Ω(V). Par hypothèse de récurrence, il existe un unique élément $\varphi$ de Ω(W) tel que $\varphi (e_1, . . . , e_{n-1}) =t$. La relation $\omega (e_1, . . . , e_n) =t$, pour $\omega$ dans Ω(V) équivaut à $\Lambda (\omega ) =\varphi$, d’où le corollaire 1.

#### Corollaire 2 {#alg-viii-a2-prop-1-cor-2 .statement tag=00Q3}

Soient $\omega$ et $\omega '$ deux éléments de Ω(V). il existe un unique élément $t$ de $D^*_{ab}$ tel que $\omega '=t\omega$.

#### Remarque {#alg-viii-a2-n2-rem-1 .statement tag=00Q4}

Supposons le corps D commutatif. Par définition, B(V) est une partie de $V^n$. Il est clair que la restriction à B(V) d’une forme $n$-linéaire alternée non nulle $f: V^n\rightarrow D$ appartient à Ω(V). Par ailleurs, si $(e_1, . . . , e_n)$ est une base de V et $t$ un élément non nul de D, il existe une unique forme $n$-linéaire alternée $f$ telle que $f(e_1, . . . , e_n) =t$ (III, p. 80 et p. 87). D’après le cor. 1, Ω(V) se compose des restrictions à B(V) des formes $n$-linéaires alternées non nulles.

### 3. Déterminant d’un automorphisme

Supposons d’abord le corps D commutatif. Compte tenu de la remarque ci-dessus, le déterminant d’un automorphisme $u$ de V est l’unique élément det $u$ de $D^*$ tel que l’on ait

(14) $\omega (u(v_1), . . . , u(v_n)) =$ (det $u)\omega (v_1, . . . , v_n)$ pour toute base $(v_1, . . . , v_n)$ de V et tout élément $\omega$ de Ω(V).

Revenons au cas où D n’est plus supposé commutatif.

#### Proposition 2 {#alg-viii-a2-prop-2 .statement tag=00Q5}

a) Soit $u$ un automorphisme de V. Il existe un unique élément de $D^*_{ab}$ noté det $u$ et appelé le déterminant de $u$, tel que l’on ait

(15) $\omega (u(v_1), . . . , u(v_n)) =$ (det $u)\omega (v_1, . . . , v_n)$

pour toute base $(v_1, . . . , v_n)$de V et tout $\omega$ dans Ω(V).

b) L’application $u\rightarrow$ det $u$ de $\mathbf{G}\mathbf{L}(V)$dans $D^*_{ab}$ est un homomorphisme de groupes.

Soit $\omega_0$ un élément de Ω(V). L’application $(v_1, . . . , v_n)\rightarrow \omega_0(u(v_1), . . . , u(v_n))$ de B(V) dans $D^*_{ab}$ appartient à Ω(V) ; d’après le cor. 2 de VIII, p. 441, il existe un unique élément $t$ de $D^*_{ab}$ tel que l’on ait

$$
\omega_0(u(v_1), . . . , u(v_n)) =t\omega_0(v_1, . . . , v_n)
$$

pour $(v_1, . . . , v_n)$ dans B(V). Si $\omega$ est un autre élément de Ω(V), il existe un élément $s$ de $D^*_{ab}$ tel que

$$
\omega (v_1, . . . , v_n) =s\omega_0(v_1, . . . , v_n)
$$

pour toute base $(v_1, . . . , v_n)$ de V (loc. cit.). On en déduit aussitôt la relation

$$
\omega (u(v_1), . . . , u(v_n)) =t\omega (v_1, . . . , v_n)
$$

Ceci prouve a) ; l’assertion b) est une conséquence immédiate de a).

### 4. Déterminant d’une matrice carrée

Soit $n$ un entier positif. Appliquons ce qui précède à l’espace vectoriel à droite $D^n_d$ sur le corps D ; les éléments de $D^n_d$ sont interprétés comme des matrices à $n$ lignes et une colonne. Soit $(\varepsilon_1, . . . , \varepsilon_n)$ la base canonique de $D^n_d$. D’après le cor. 2 de VIII, p. 441, il existe un unique élément $\omega_0$ de $\Omega (D^n_d)$ tel que $\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$. Si A est un élément de $\mathbf{G}\mathbf{L}_n$(D), ses colonnes $a_1, . . . , a_n$ forment une base de $D^n_d$; l’élément $\omega_0(a_1, . . . , a_n)$ de $D^*_{ab}$ d’appelle le déterminant de A et se note det(A). Comme on a $a_i= A\varepsilon_i$ pour $1\leqslant i\leqslant n$, le déterminant de A n’est autre que le déterminant de l’automorphisme $x\rightarrow Ax$ de $D^n_d$. En particulier, si le corps D est commutatif, le déterminant de A coïncide avec celui qu’on a défini en III, p. 92.

Soit V un espace vectoriel à droite, de dimension finie $n$ sur le corps D, et soit $(e_1, . . . , e_n)$ une base de V. Si $u$ est un automorphisme de V et A la matrice de $u$ par rapport à la base $(e_1, . . . , e_n)$, on a det($u$) $=$ det(A).

On note ($E_{ij}$) la famille des unités matricielles de $\mathbf{M}_n(D)$ (II. p. 142). Pour tout élément $\lambda$ de D et tout couple $(i, j)$ d’entiers distincts dans $[1, n]$, on pose (II, p. 161)

$$
B_{ij}(\lambda ) = I_n+\lambda E_{ij}
$$

c’est un élément de $\mathbf{G}\mathbf{L}_n(D)$. Si $\lambda_1, . . . , \lambda_n$ sont des éléments de $D^*$, la matrice diagonale diag($\lambda_1, . . . , \lambda_n$) appartient aussi à $\mathbf{G}\mathbf{L}_n(D)$.

#### Proposition 3 {#alg-viii-a2-prop-3 .statement tag=00Q6}

L’application det est l’unique homomorphisme de $\mathbf{G}\mathbf{L}_n(D)$ dans $D^*_{ab}$ qui satisfait aux relations

(16) det($B_{ij}(1)$) $= 1$

pour $i\not=j$ et

(17) det(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1. . . \lambda_n)$,

pour $\lambda_1, . . . , \lambda_n\in D^*$

Soient A un élément de $\mathbf{G}\mathbf{L}_n(D)$ et $a_1, . . . , a_n$ ses colonnes. On a

det(A$) =\omega_0(a_1, . . . , a_n)$.

Or les colonnes de la matrice A diag($\lambda_1, . . . , \lambda_n$) sont $a_1\lambda_1, . . . , a_n\lambda_n$ et celles de la matrice AB$_{ij}(1)$ dont $a_1, . . . , a_j+a_i, a_{j+1}, . . . , a_n$. Comme $\omega_0$ est l’unique élément de $\Omega (D^n_d)$ tel que $\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$, on voit que le déterminant est l’unique application $\varphi : \mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$ qui satisfait aux relations

(18) $\varphi ($A diag($\lambda_1, . . . , \lambda_n$)) $=\varphi ($A$)\pi (\lambda_1. . . \lambda_n)$

(19) $\varphi ($AB$_{ij}(1)) =\varphi ($A) pour $i\not=j$

$$
\varphi (I_n) = 1 \tag{20}
$$

Cela prouve tout d’abord que que l’application déterminant satisfait aux relations (16) et (17). Nous savons déjà que cette application est un homomorphisme de $\mathbf{G}\mathbf{L}_n(D)$ dans $D^*_{ab}$. Inversement, si $\varphi$ est un homomorphisme de $\mathbf{G}\mathbf{L}_n(D)$ dans $D^*_{ab}$ tel que $\varphi (B_{ij}(1)) = 1$ pour $i\not=j$ et $\varphi$(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1. . . \lambda_n)$, alors $\varphi$ satisfait aux relations (18) à (20) et est donc égal à det.

#### Exemple 1 {#alg-viii-a2-n4-exa-1 .statement tag=00Q7}

Les colonnes de la matrice $B_{ij}(\lambda )$ sont $\varepsilon_1, . . . , \varepsilon_j+\varepsilon_i\lambda , \varepsilon_{i+1}, . . . , \varepsilon_n$. Compte tenu de la formule (5) de VIII, p. 438, on a

(21) det($B_{ij}(\lambda )$) $= 1$.

#### Exemple 2 {#alg-viii-a2-n4-exa-2 .statement tag=00Q8}

Soit $\sigma$ une permutation de l’intervalle $[1, n]$ de $\mathbf{N}$, de signature $\varepsilon (\sigma )$. Soit M $(\sigma )$ la matrice de la permutation $\sigma$ (II, p. 151). Les colonnes de la matrice M $(\sigma )$ sont $\varepsilon_{\sigma(1)}, . . . , \varepsilon_{\sigma(n)}$. Par application de la formule (4) de VIII, p. 438, on a donc (22) det(M $(\sigma )) =\pi (\varepsilon (\sigma ))$.

#### Exemple 3 {#alg-viii-a2-n4-exa-3 .statement tag=00Q9}

Supposons $n\geqslant 1$. Pour toute matrice diagonale inversible de la forme Δ = diag($d_1, . . . , d_n$), on a Δ$B_{ij}(\lambda )\Delta^{-1}= B_{ij}(d_i\lambda d^-_j^1)$. Soit A un élément de $\mathbf{G}\mathbf{L}_n(D)$. D’après le cor. 1 de II, p. 162 et la formule précédente, il existe des matrices P et Δ dans $\mathbf{G}\mathbf{L}_n(D)$ telles que A = PΔ, que P soit produit de matrices de la forme $B_{ij}(\lambda )$ et que Δ soit une matrice diagonale de la forme diag(1$, . . . ,1, d)$. On a det(P) = 1 d’après l’exemple 1, donc det(A) = det(Δ) $=\pi (d)$ par la prop. 3.

#### Exemple 4 {#alg-viii-a2-n4-exa-4 .statement tag=00QA}

Soit $D'$ un corps et soit $u$ un homomorphisme de D dans $D'$. Par passage aux quotients, $u$ définit un homomorphisme de groupes $u_{ab}$ de $D^*_{ab}$ dans $D^{'*}_{ab}$. Soit $u_n$ l’homomorphisme de $\mathbf{G}\mathbf{L}_n(D)$ dans $\mathbf{G}\mathbf{L}_n(D')$ qui transforme une matrice A $= (a_{ij})$ en la matrice $(u(a_{ij}))$. La formule

(23) det($u_n($A$)) =u_{ab}$(det(A))

pour $A\in \mathbf{G}\mathbf{L}_n$(D), résulte aussitôt de l’exemple 3.

#### Exemple 5 {#alg-viii-a2-n4-exa-5 .statement tag=00QB}

On a $\mathbf{G}\mathbf{L}_1(D) = D^*$ et la prop. 3 montre que l’on a det($a$) $=\pi (a)$ pour $a$ dans $\mathbf{G}\mathbf{L}_1(D)$.

#### Exemple 6 {#alg-viii-a2-n4-exa-6 .statement tag=00QC}

Supposons que l’on ait $n= 2$. Soit A $= (^{a b}_{c d})$ un élément de $\mathbf{G}\mathbf{L}_2(D)$. Les éléments $a$ et $c$ de D ne sont pas tous deux nuls. Nous allons expliciter le déterminant de A.

a) Si $a$ n’est pas nul, on a

1 0 $a$ 0 1 $a^{-1}b$

(24) A = $ca^{-1}$ 1 0 $d-ca^{-1}b$ 0 1.

D’où $ad-aca^{-1}b\not= 0$ et

(25) det(A$) =\pi (ad-aca^{-1}b)$.

b) Si $a$ est nul, on a $c\not= 0$ et

0 $b$ 0 1 $c d$

(26) A = =,

$c d$ 1 0 0 $b$

d’où d’après a) et l’exemple 2$,cb\not= 0$ et

(27) det(A$) =\pi (-cb)$.

#### Exemple 7 {#alg-viii-a2-n4-exa-7 .statement tag=00QD}

Soit $D^o$ le corps opposé de D. L’application $A\rightarrow^tA$de $\mathbf{M}_n(D)$ dans $\mathbf{M}_n(D^o)$ satisfait à $^t($AB$) =^tB^tA$. Pour toute matrice A dans $\mathbf{G}\mathbf{L}_n$(D), la matrice transposée $^tA$est donc inversible dans $\mathbf{M}_n(D^o)$, mais elle n’est pas nécessairement inversible dans $\mathbf{M}_n(D)$. Il résulte de l’exemple 3 que si A appartient à $\mathbf{G}\mathbf{L}_n$(D), les éléments A de $\mathbf{G}\mathbf{L}_n(D)$ et $^tA$de $\mathbf{G}\mathbf{L}_n(D^o)$ ont même déterminant. Par contre, même si la matrice $^tA$appartient à $\mathbf{G}\mathbf{L}_n(D)$ son déterminant deans GL$_n(D)$ n’est pas nécessairement égal à celui de A (cf. exemple 6).

#### Remarque 1 {#alg-viii-a2-n4-rem-1 .statement tag=00QE}

Soit V un espace vectoriel à droite sur le corps D, de dimension finie $n$. Considérons l’espace dual $V^*=$ Hom$_D(V,D)$ comme un espace vectoriel à droite sur le corps $D^o$ opposé de D. Soit $u$ un automorphisme de V et soit $^tu$ l’automorphisme de $V^*$ transposé de $u$. Si $u$ est représenté par une matrice A de $\mathbf{M}_n(D)$ par rapport à une base $(e_1, . . . , e_n)$ de V, l’automorphisme $^tu$ est représenté par la matrice $^tA$de $\mathbf{M}_n(D^o)$ par rapport à la base $(e^*_1, . . . , e^*_n)$ de $V^*$ duale de $(e_1, . . . , e_n)$ (II, p. 145, prop. 3). D’après l’exemple 7, le déterminant de $^tu$ est égal à celui de $u$.

#### Remarque 2 {#alg-viii-a2-n4-rem-2 .statement tag=00QF}

Les résultats des numéros 1 à 4 se généralisent au cas où D est un anneau local (VIII, p. 448, exerc. 2).

### 5. Le groupe unimodulaire

Soit $n$ un entier positif. On note $\mathbf{S}\mathbf{L}_n(D)$ le noyau de l’homomorphisme de groupes det$: \mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$, et on l’appelle le groupe unimodulaire (cf. III, p. 104 pour le cas où le corps D est commutatif).

#### Théorème 1 {#alg-viii-a2-thm-1 .statement tag=00QG}

Supposons $n\geqslant 2$.

a) Le sous-groupe $\mathbf{S}\mathbf{L}_n(D)$de $\mathbf{G}\mathbf{L}_n(D)$est engendré par les matrices $B_{ij}(\lambda )$où $i$ et $j$ sont des entiers distincts de l’intervalle $[1, n]$ et $\lambda$ parcourt D.

b) Supposons $n\geqslant 3$ou Card(D) $\geqslant 3$. Le groupe dérivé de $\mathbf{G}\mathbf{L}_n(D)$est égal à $\mathbf{S}\mathbf{L}_n(D)$.

c) Supposons $n\geqslant 3$ou Card(D) $\geqslant 4$. Le groupe dérivé de $\mathbf{S}\mathbf{L}_n(D)$est égal à $\mathbf{S}\mathbf{L}_n(D)$.

A) Notons T le sous-groupe de $\mathbf{G}\mathbf{L}_n(D)$ engendré par les matrices $B_{ij}(\lambda )$. D’après l’exemple 1 de VIII, p. 443, on a det($B_{ij}(\lambda )$) $= 1$, d’où $T\subset \mathbf{S}\mathbf{L}_n(D)$. Pour prouver que ces deux groupes sont égaux, il suffit alors, d’après l’exemple 3 de loc. cit., de prouver que toute matrice de la forme diag(1$, . . . ,1, d)$avec $\pi (d) = 1$appartient à $($ T. La matrice diag(1$), . . . ,1, d)$ appartient à l’image de l’homomorphisme $U\rightarrow^{I_n}_{0^{-2}U}^0$ de $\mathbf{G}\mathbf{L}_2(D)$ dans $\mathbf{G}\mathbf{L}_n(D)$; il suffit donc de considérer le cas $n= 2$. Comme le noyau de $\pi$ est le groupe dérivé de $D^*$, on peut supposer $d=uvu^{-1}v^{-1}$ avec $u, v$ dans $D^*$. Notre assertion résulte alors des égalités

1 0 $u^{-1}$ 0 $v^{-1}$ 0 $vu$ 0

(28) = $-_-$

0 $d$ 0 $u$ 0 $v$ 0 $u^1v^1$

et

(29) $s$ 0 = 1 $s$ 1 0 1 $-1$ 1 0

0 $s^{-1}$ 0 1 $1-s^{-1}$ 1 0 1 $1-s$ 1

pour $s\in D^*$.

B) Par construction, $\mathbf{S}\mathbf{L}_n(D)$ est le noyau d’un homomorphisme de $\mathbf{G}\mathbf{L}_n(D)$ dans un groupe commutatif, donc il contient le groupe dérivé $(\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))$ de $\mathbf{G}\mathbf{L}_n(D)$. Vu ce qui précède, on a

$$
\mathbf{S}\mathbf{L}_n(D)\supset (\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))\supset (\mathbf{S}\mathbf{L}_n(D),\mathbf{S}\mathbf{L}_n(D))
$$

Pour prouver c), il suffit de démontrer que les matrices $B_{ij}(\lambda )$ sont des commutateurs dans $\mathbf{S}\mathbf{L}_n(D)$.

Supposons $n\geqslant 3$. Si $i,j,k$ sont des entiers distincts dans l’intervalle $[1, n]$ et $\mu , \nu$ des éléments de D, on a

$$
B_{ij}(\mu \nu ) = B_{ik}(\mu )^{-1}B_{kj}(\nu )^{-1}B_{ik}(\mu )B_{kj}(\nu ) \tag{30}
$$

En prenant $\mu = 1$ et $\nu =\lambda$, on voit que la matrice $B_{ij}(\lambda )$ est un commutateur d’éléments de $\mathbf{S}\mathbf{L}_n(D)$.

Supposons maintenant $n= 2$. Soient $u$ et $v$ des éléments de D avec $u\not= 0$. On a les relations

1 $v-uvuu$ 0 1 $-vu^{-1}$ 0 1 $v$

(31) = $-_1$

0 1 0 $u$ 0 1 0 $u$ 0 1

et

1 0 $u^{-1}$ 0 1 0 $u$ 0 1 0

(32) $v-uvu$ 1 = 0 $u-v$ 1 0 $u^{-1}v$ 1

On a det$(^u_{0u}^{0_{-1}})= 1$; donc les matrices $B_{12}(v-uvu)$ et $B_{21}(v-uvu)$ sont des commutateurs d’éléments de $\mathbf{S}\mathbf{L}_n(D)$.

Supposons que le corps D ait au moins 4 éléments. Soit $\lambda$ un élément de D. Si $\lambda$ est égal à 0, 1 ou $-1$, choisissons un élément $u$ arbitraire dans $D- \{0,1,-1\}$; sinon posons $u=\lambda$. Dans les deux cas, $u$ est un élément non nul de D, il commute à $\lambda$, et l’on a $u^2\not= 1$. Posons $v=\lambda (1-u^2)^{-1}$. On a $uv=vu$ d’où $v-uvu=v(1-u^2) =\lambda$. Il résulte alors des relations (31) et (32) que les matrices $B_{12}(\lambda )$ et $B_{21}(\lambda )$ sont des commutateurs dans $\mathbf{S}\mathbf{L}_n(D)$ d’où c).

C) Il reste à prouver que $\mathbf{S}\mathbf{L}_2(D)$ est le groupe dérivé de $\mathbf{G}\mathbf{L}_2(D)$ lorsque D a 3 éléments. D’après A), le groupe $\mathbf{S}\mathbf{L}_2(D)$ est engendré par les matrices $B_{12}(1) = (^{1 1}_{0 1})$ et $B_{21}(1) = (^{1 0}_{1 1})$, et ces matrices sont des commutateurs d’éléments de $\mathbf{G}\mathbf{L}_2(D)$ puisque l’on a $B_{21}(1) =^tB_{12}(1)$ et

1 1 $-1 0$ 1 1 $-1 0^{-1}$ 1 1 $^{-1}$

(33) =.

0 1 0 1 0 1 0 1 0 1

#### Remarque {#alg-viii-a2-n5-rem-1 .statement tag=00QH}

Si D est un corps à 2 éléments, alors $\mathbf{G}\mathbf{L}_2(D)$ est égal à $\mathbf{S}\mathbf{L}_2(D)$ et c’est un groupe d’ordre 6 dont le groupe dérivé est d’ordre 3. Si D est un corps à 3 éléments, le groupe $\mathbf{S}\mathbf{L}_2(D)$ est d’ordre 24 et son groupe dérivé est d’ordre 8. Supposons $n\geqslant 2$; sauf dans les deux cas précédents, tout sous-groupe distingué de $\mathbf{S}\mathbf{L}_n(D)$ distinct de $\mathbf{S}\mathbf{L}_n(D)$ est contenu dans le centre $Z((\mathbf{S}\mathbf{L}_n(D))$ de $)\mathbf{S}\mathbf{L}_n(D)$ (II. p. 207, exerc. 13 et p. 208 exerc. 14). Le groupe $\mathbf{S}\mathbf{L}_n(D)/Z\mathbf{S}\mathbf{L}_n(D)$ est alors simple.

Soit V un espace vectoriel à droite sur le corps D, de dimension finie $n$. On note $\mathbf{S}\mathbf{L}(V)$ et on appelle groupe unimodulaire de V, le noyau de l’homomorphisme det$: \mathbf{G}\mathbf{L}(V)\rightarrow D^*_{ab}$. Le choix d’une base de V permet d’identifier ce groupe à $\mathbf{S}\mathbf{L}_n(D)$.

On dit qu’un automorphisme $u$ de V est une transvection s’il existe un vecteur $v$ de V et une forme linéaire $\varphi$ sur V tels que $\varphi (v) = 0$ et $u(x) =x+v\varphi (x)$ pour tout $x$ de V. Lorsque $n\geqslant 2,u$ est une transvection si et seulement s’il existe une base de V dans laquelle la matrice de $u$ soit de la forme $B_{ij}(\lambda )$. Le th. 1 entraîne le corollaire suivant :

#### Corollaire {#alg-viii-a2-n5-cor-1 .statement tag=00RU}

Soit V un espace vectoriel à droite sur le corps D, de dimension finie $n\geqslant 2$.

a) Le sous-groupe $\mathbf{S}\mathbf{L}(V)$de $\mathbf{G}\mathbf{L}(V)$est engendré par les transvections.

b) Le sous-groupe $\mathbf{S}\mathbf{L}(V)$est le groupe dérivé de $\mathbf{G}\mathbf{L}(V)$sauf lorsque l’on a $n= 2$et que D possède 2 éléments.

c) Le groupe $\mathbf{S}\mathbf{L}(V)$est égal à son groupe dérivé sauf lorsqu’on a $n= 2$et que D possède 2 ou 3 éléments.

## EXERCICES {#alg-viii-a2-exercises}

See the [exercises for Appendix 2](exercises/a2/).
