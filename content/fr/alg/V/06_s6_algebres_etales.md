---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 6
section_title: ALGÈBRES ÉTALES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.144
pdf_pages: 0130-0139, 0248-0248
extraction: ocr
subsections:
    - "no": 1
      title: Indépendance linéaire des homomorphismes
      page: 0
      pdf_page: 130
    - "no": 2
      title: Indépendance algébrique des homomorphismes
      page: 27
      pdf_page: 131
    - "no": 3
      title: Algèbres diagonalisables et algèbres étales
      page: 28
      pdf_page: 132
    - "no": 4
      title: Sous-algèbres d’une algèbre étale
      page: 29
      pdf_page: 133
    - "no": 5
      title: Degré séparable d’une algèbre commutative
      page: 30
      pdf_page: 134
    - "no": 6
      title: Caractérisation différentielle des algèbres étales
      page: 32
      pdf_page: 136
    - "no": 7
      title: Algèbres réduites et algèbres étalées
      page: 33
      pdf_page: 137
statements: 20
exercises: 2
content_sha256: 8181457df575d1d33da33311edde292d95015c19f2ec41a221890f0ec1d9c27a
---

## § 6. ALGÈBRES ÉTALES

Dans tout ce paragraphe, on note K un corps.

### 1. Indépendance linéaire des homomorphismes

Soient L une extension de K et V un espace vectoriel sur K. Dans ce paragraphe, on note Hom_K(V, L) l’ensemble des applications K-linéaires de V dans L muni de la structure d’espace vectoriel sur L telle que :

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

pour $x \in V, \alpha \in L$ et $f, g$ dans Hom_K(V, L). Soient $V_{(L)} = L \otimes_K V$ l’espace vectoriel sur L déduit de V par extension des scalaires et $(V_{(L)})^*$ son dual. D’après II, p. 82, on a un isomorphisme canonique $u \mapsto \tilde{u}$ de L-espaces vectoriels de $(V_{(L)})^*$ sur Hom_K(V, L) tel que $\tilde{u}(x) = u(1 \otimes x)$ pour $x \in V$ et $u$ dans $(V_{(L)})^*$. Si V est de dimension finie n sur K, l’espace vectoriel $V_{(L)}$ sur L est de dimension n, ainsi que son dual $(V_{(L)})^* = V_{(L)}^*$, d’où la formule

(2) $$ [\mathrm{Hom}_K(V, L) : L ] = [V : K] . $$

#### Théorème 1 {#alg-v-s6-thm-1 .statement}

Soient L une extension d’un corps K et A une algèbre sur K ; soit $\mathcal{H}$ l’ensemble des homomorphismes de K-algèbres de A dans L. Alors $\mathcal{H}$ est une partie libre de l’espace vectoriel $\mathrm{Hom}_K(A, L)$ sur L.

Montrons, par récurrence sur l’entier $n \geqslant 0$, que toute suite $(u_1, \ldots, u_n)$ d’éléments distincts de $\mathcal{H}$ est libre. Le cas $n = 0$ étant trivial, supposons désormais $n \geqslant 1$; soient $\alpha_1, \ldots, \alpha_n$ des éléments de L tels que l’on ait $\sum_{i=1}^n \alpha_i u_i = 0$. Pour $x, y$ dans A, on a

$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0 ,
$$

d’où $\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0$. D’après l’hypothèse de récurrence, les éléments $u_1, \ldots, u_{n-1}$ de $\mathcal{H}$ sont linéairement indépendants, d’où $\alpha_i [u_i(x) - u_n(x)] = 0$ pour $1 \leqslant i \leqslant n-1$ et pour tout $x$ dans A. Les $u_i$ étant distincts, cela implique $\alpha_i = 0$ pour $i \neq n$, donc $\alpha_n u_n = 0$, d’où $\alpha_n = \alpha_n u_n(1) = 0$ (en notant 1 l’élément unité de A). On a donc prouvé que $\alpha_1, \ldots, \alpha_{n-1}, \alpha_n$ sont nuls, d’où le théorème.

#### Corollaire 1 {#alg-v-s6-thm-1-cor-1 .statement}

Soient $\Gamma$ un monoïde, L un corps et X l’ensemble des homomorphismes de $\Gamma$ dans le monoïde multiplicatif de L. Alors X est une partie libre du L-espace vectoriel $L^\Gamma$ des applications de $\Gamma$ dans L.

Soient A l’algèbre du monoïde $\Gamma$ à coefficients dans L et $(e_\gamma)_{\gamma \in \Gamma}$ la base canonique de A sur L (III, p. 19). Pour toute application L-linéaire $u$ de A dans L, posons $\tilde{u}(\gamma) = u(e_\gamma)$ (pour $\gamma \in \Gamma$) ; alors, l’application $u \mapsto \tilde{u}$ est un isomorphisme de L-espaces vectoriels de $\mathrm{Hom}_L(A; L)$ sur $L^\Gamma$, qui applique sur X l’ensemble des homomorphismes de L-algèbres de A dans L. Il suffit alors d’appliquer le th. 1 avec $K = L$.

#### Corollaire 2 (Théorème de Dedekind) {#alg-v-s6-thm-1-cor-2 .statement}

*Soient E et L deux extensions de K. L’ensemble des K-homomorphismes de E dans L est libre sur L. Si E est de degré fini sur K, le nombre des K-homomorphismes de E dans L est au plus égal à [E : K].*
La dernière assertion se déduit de la première en tenant compte de la formule (2).

### 2. Indépendance algébrique des homomorphismes

#### Théorème 2 {#alg-v-s6-thm-2 .statement}

*Soient K un corps infini, L une extension de K et A une algèbre sur K. Soient $u_1, ..., u_n$ des K-homomorphismes d’algèbres distincts de A dans L et f un polynôme de $L[X_1, ..., X_n]$. Si l’on a $f(u_1(x), ..., u_n(x)) = 0$ pour tout $x \in A$, on a $f = 0$.
Soit B l’ensemble des éléments de $L^n$ de la forme $(u_1(x), ..., u_n(x))$ avec $x \in A$. D’après le théorème 1, il n’existe pas de suite $(\alpha_1, ..., \alpha_n)$ d’éléments non tous nuls de L telle que $\sum_{i=1}^n \alpha_i u_i(x) = 0$ pour tout $x \in A$; par suite (II, p. 104, th. 7), B engendre l’espace vectoriel $L^n$ sur L. Il existe donc des éléments $a_1, ..., a_n$ de A tels que la matrice $(u_i(a_j))_{1 \leq i,j \leq n}$ soit inversible.
Définissons le polynôme $g \in L[Y_1, ..., Y_n]$ par
$$
g(Y_1, ..., Y_n) = f(\sum_{j=1}^n u_1(a_j) Y_j, ..., \sum_{j=1}^n u_n(a_j) Y_j).
$$
Soient $y_1, ..., y_n$ dans K ; si l’on pose $x = \sum_{i=1}^n y_i a_i$, on a
$$
g(y_1, ..., y_n) = f(u_1(x), ..., u_n(x)), \text{ d’où } g(y_1, ..., y_n) = 0
$$
d’après l’hypothèse faite sur $f$. Comme le corps K est infini, on a $g = 0$ (IV, p. 17, corollaire 2) ; or, la matrice $(u_i(a_j))$ a une inverse $(b_{ij})$, et l’on a
$$
f(X_1, ..., X_n) = g(\sum_{j=1}^n b_{1j} X_j, ..., \sum_{j=1}^n b_{nj} X_j),
$$
d’où $f = 0$.

Le théorème 2 n’a pas d’analogue pour les corps finis. Soient en effet K un corps fini à q éléments, $A = L = K$ et $f(X) = X^q - X$. On a $x^q = x$ pour tout $x \in K$ (V, p. 89, prop. 2) ; par suite, si $u$ est l’automorphisme identique de K, on a $f(u(x)) = 0$ pour tout $x \in K$ bien que $f$ ne soit pas nul.

### 3. Algèbres diagonalisables et algèbres étales

#### Définition 1 {#alg-v-s6-def-1 .statement}

Soit $A$ une algèbre sur $K$. On dit que $A$ est diagonalisable s’il existe un entier $n \geqslant 0$ tel que $A$ soit isomorphe à l’algèbre produit $K^n$. On dit que $A$ est diagonalisée par une extension $L$ de $K$ si l’algèbre $A_{(L)}$ sur $L$ déduite de $A$ par extension des scalaires est diagonalisable. On dit que $A$ est étale s’il existe une extension de $K$ qui diagonalise $A$.

Rappelons que l’algèbre produit $K^n$ est l’espace vectoriel $K^n$ muni du produit défini par

$$
(x_1, \ldots, x_n).(y_1, \ldots, y_n) = (x_1y_1, \ldots, x_ny_n) .
$$

Si $\varepsilon_1, \ldots, \varepsilon_n$ est la base canonique de $K^n$, on a

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{si} \quad i \neq j
$$

et $1 = \varepsilon_1 + \cdots + \varepsilon_n$.

Toute algèbre étale sur $K$ est commutative et de degré fini sur $K$.

#### Proposition 1 {#alg-v-s6-prop-1 .statement}

Soit $A$ une algèbre de degré fini $n$ sur le corps $K$. Les conditions suivantes sont équivalentes :

a) L’algèbre $A$ est diagonalisable.
b) Il existe une base $(e_1, \ldots, e_n)$ de $A$ telle que $e_i^2 = e_i$ et $e_i e_j = 0$ pour $i \neq j$.
c) Les homomorphismes de $K$-algèbres de $A$ dans $K$ engendrent le dual du $K$-espace vectoriel $A$.
d) Tout $A$-module est somme directe de sous-modules qui sont de dimension 1 sur $K$.

L’équivalence de a) et b) résulte de la formule (6) ; d’autre part, les $n$ projections $K^n \to K$ sont des homomorphismes d’algèbres, donc a) implique c). Si c) est satisfait, les homomorphismes d’algèbres de $A$ dans $K$ forment une base du dual de $A$ (V, p. 26, th. 1) ; notons-les $u_1, \ldots, u_n$ ; alors $a \mapsto (u_i(a))$ est un isomorphisme de $A$ sur l’algèbre $K^n$, d’où a). On a donc démontré l’équivalence des conditions $a), b)$ et c).

Supposons b) vérifiée, et soit $M$ un $A$-module ; alors les homothéties $(e_i)_M$ de rapport $e_i$ sont des projecteurs de $M$, et $M$ est somme directe des $e_i M$, qui en sont des sous-A-modules. On peut donc supposer qu’il existe un indice $i$ tel que $(e_j)_M = 0$ pour $j \neq i$. Alors tout sous-espace vectoriel de $M$ en est un sous-A-module, d’où d).

Inversement, supposons d) vérifiée et considérons le $A$-module $A_s$. Il existe alors une base $(f_i)$ du $K$-espace vectoriel $A$ tel que $Af_i = Kf_i$ pour $i = 1, \ldots, n$. Quitte à remplacer chaque $f_i$ par un multiple scalaire convenable, on peut supposer que $1 = f_1 + \cdots + f_n$. Si $i \neq j$, $f_i f_j$ appartient à $Af_i \cap Af_j = Kf_i \cap Kf_j$, donc est nul. Alors $f_i = f_i f_1 + \cdots + f_i f_n = f_i^2$, d’où b).

#### Corollaire {#alg-v-s6-n3-cor-1 .statement}

Soient L une extension de K et $\mathcal{H}$ l’ensemble des homomorphismes d’algèbres de A dans L. On a Card $\mathcal{H} \leq [A : K]$, avec égalité si et seulement si A est diagonalisée par L. Si A est diagonalisée par L, alors $\mathcal{H}$ est une base du L-espace vectoriel $\mathrm{Hom}_K(A, L)$.

L’espace vectoriel $\mathrm{Hom}_K(A, L)$ sur L est de dimension $[A : K]$ d’après la formule (2) et $\mathcal{H}$ est une partie libre de $\mathrm{Hom}_K(A, L)$ d’après le th. 1 (V, p. 26). On a donc Card $\mathcal{H} \leq [A : K]$ avec égalité si et seulement si $\mathcal{H}$ est une base de $\mathrm{Hom}_K(A, L)$. Il existe un isomorphisme de L-espaces vectoriels, soit $\pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^*$, caractérisé par $u(x) = (\pi u)(1 \otimes x)$ pour $x \in A$, et $\pi$ applique $\mathcal{H}$ sur l’ensemble $\mathcal{H}_L$ des homomorphismes de L-algèbres de $A_{(L)}$ dans L. Enfin, l’équivalence de a) et c) dans la prop. 1 montre que l’algèbre $A_{(L)}$ sur L est diagonalisable si et seulement si $\mathcal{H}_L$ engendre l’espace vectoriel $A_{(L)}^*$ sur L. Ceci prouve le corollaire.

#### Proposition 2 {#alg-v-s6-prop-2 .statement}

Soient A une algèbre sur K et $\Omega$ une extension algébriquement close de K. Les assertions suivantes sont équivalentes :
a) L’algèbre A est étale.
b) Il existe une extension de degré fini de K qui diagonalise A.
c) L’extension $\Omega$ de K diagonalise A.

Supposons que A soit étale. Soit n le degré de A sur K, soit L une extension de K qui diagonalise A, et soit $\mathcal{H}$ l’ensemble des homomorphismes d’algèbres de A dans L. On a Card $\mathcal{H} = n$ d’après le cor. de la prop. 1. D’autre part, pour tout $u \in \mathcal{H}$, on a $[u(A) : K] \leq n$. D’après V, p. 17, th. 2, la sous-extension L’ de L engendrée par les images des éléments de $\mathcal{H}$ est de degré fini sur K. Comme il existe n homomorphismes distincts de A dans L’, l’extension L’ diagonalise A d’après le cor. de la prop. 1. Ceci montre que a) entraîne b).

Comme toute extension de degré fini de K est isomorphe à une sous-extension de $\Omega$ (V, p. 20, th. 1), b) entraîne c). Enfin, c) entraîne évidemment a).

### 4. Sous-algèbres d’une algèbre étale

#### Proposition 3 {#alg-v-s6-prop-3 .statement}

Soit A une algèbre étale sur K. Il n’existe qu’un nombre fini de sous-algèbres et d’idéaux de A. De plus, toute extension de K qui diagonalise A diagonalise toute sous-algèbre et toute algèbre quotient de A, et en particulier ces algèbres sont étales.

Il suffit de montrer qu’une algèbre $K^n$ n’a qu’un nombre fini de sous-algèbres et d’idéaux, et que les sous-algèbres et les algèbres quotients de $K^n$ sont diagonalisables. On notera $(\varepsilon_1, ..., \varepsilon_n)$ la base canonique de $K^n$.

Soit A une sous-algèbre de $K^n$, et soient $v_1, ..., v_n$ les restrictions à A des n projections $K^n \to K$. Comme l’intersection des noyaux des $v_i$ est évidemment réduite à 0, les $v_i$ engendrent le K-espace vectoriel dual de A (II, p. 104, cor. 1); la K-algèbre A est donc diagonalisable (V, p. 28, prop. 1).

Pour toute partie I de {1, 2, ..., n}, posons $\varepsilon_I = \sum_{i \in I} \varepsilon_i$. Il est immédiat que les éléments $\varepsilon_I$ sont les idempotents de $K^n$; on a $\varepsilon_I = 0$ si et seulement si I est vide et $\varepsilon_I \varepsilon_J = \varepsilon_{I \cap J}$. D’après ce qui précède, toute sous-algèbre A de $K^n$ est diagonalisable ; d’après la condition b) de la prop. 1, toute sous-algèbre A de $K^n$ admet donc une base $(\varepsilon_{I_1}, ..., \varepsilon_{I_p})$ où $(I_1, ..., I_p)$ est une partition de {1, 2, ..., n}, et il n’y a finalement qu’un nombre fini de telles sous-algèbres.

Pour toute partie I de {1, 2, ..., n}, soit $a_I$ le sous-espace vectoriel de $K^n$ ayant pour base les idempotents $\varepsilon_i$ pour $i \in I$. Il est immédiat que $a_I$ est un idéal de $K^n$; de plus, si $J = \{1, 2, ..., n\} - I$, les classes $\overline{\varepsilon_j}$ de $\varepsilon_j$ modulo $a_I$ pour $j \in J$ forment une base de $K^n / a_I$. On a $\overline{\varepsilon_j^2} = \overline{\varepsilon_j}$ et $\overline{\varepsilon_j} \overline{\varepsilon_k} = 0$ si $j \neq k$, donc l’algèbre $K^n / a_I$ est diagonalisable d’après la prop. 1 de V, p. 28.

Il reste à prouver que tout idéal $a$ de $K^n$ est de la forme $a_I$. Soit I l’ensemble des entiers $i$ tels que $1 \leq i \leq n$ et $\varepsilon_i \in a$; on a $a_I \subset a$. Soit $x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n$ un élément de $a$ (avec $x_1, ..., x_n$ dans $K$) et soit $i$ dans $\{1, 2, ..., n\} - I$. On a $x_i \varepsilon_i = x \varepsilon_i \in a$ et $\varepsilon_i \notin a$, d’où $x_i = 0$. On a donc $x = \sum_{i \in I} x_i \varepsilon_i$, d’où $x \in a_I$. On a prouvé l’inclusion $a \subset a_I$, d’où finalement $a = a_I$.

#### Corollaire {#alg-v-s6-n4-cor-1 .statement}

*Soient $A_1, ..., A_m$ des algèbres sur $K$, et $A = A_1 \times \cdots \times A_m$. Pour que $A$ soit étale, il faut et il suffit que $A_1, ..., A_m$ soient étales.*

Supposons A étale ; chacune des algèbres $A_1, ..., A_m$ est isomorphe à un quotient de A, donc est étale d’après la prop. 3. Réciproquement, toute extension de K qui diagonalise $A_1, ..., A_m$ diagonalise évidemment A.

### 5. Degré séparable d’une algèbre commutative

Soit A une algèbre commutative de degré fini $n$ sur K. Pour toute extension L de K, le nombre $h(L)$ des homomorphismes d’algèbres de A dans L est fini et majoré par $n$ (V, p. 29, cor.).

#### Lemme 1 {#alg-v-s6-lem-1 .statement}

*Soit $\Omega$ une clôture algébrique de K. On a $h(L) \leq h(\Omega)$ pour toute extension L de K, avec égalité si L est algébriquement clos.*

Soit L’ la fermeture algébrique de K dans L. Pour tout homomorphisme $u$ de A dans L, on a $[u(A) : K] \leq n$, donc $u(A) \subset L'$ d’après V, p. 17, prop. 2 ; on a donc $h(L') = h(L)$. Comme l’extension L’ de K est isomorphe à une sous-extension de $\Omega$ (V, p. 20, th. 1), on a $h(L') \leq h(\Omega)$. Si L est algébriquement clos, alors L’ est une clôture algébrique de K ; les extensions L’ et $\Omega$ de K sont alors isomorphes (V, p. 22, th. 2) et par suite $h(L') = h(\Omega)$. Le lemme résulte aussitôt de là.

D’après le lemme 1, le nombre $h(L)$ a la même valeur pour toutes les extensions algébriquement closes L de K ; ce nombre sera noté $[A : K]_s$ et appelé le *degré séparable* de A.

Soient $A$ et $B$ deux algèbres commutatives de degré fini sur $K$. Nous allons établir la formule

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

Soit $L$ une extension algébriquement close de $K$; notons $\mathcal{H}(A)$ l’ensemble des homomorphismes d’algèbres de $A$ dans $L$, et définissons de manière analogue $\mathcal{H}(B)$ et $\mathcal{H}(A \otimes_K B)$. Par définition, on a Card $\mathcal{H}(A) = [A : K]_s$ et des formules analogues pour $[B : K]_s$ et $[A \otimes_K B : K]_s$. De plus (III, p. 38, formule (6)), la formule $(u * v) (a \otimes b) = u(a) v(b)$ définit une bijection $(u, v) \mapsto u * v$ de $\mathcal{H}(A) \times \mathcal{H}(B)$ sur $\mathcal{H}(A \otimes_K B)$, d’où la formule (7).

Soit $K'$ une extension de $K$; prouvons la formule

$$
[A_{(K')} : K']_s = [A : K]_s .
$$

En effet, prenons pour $L$ une clôture algébrique de $K'$. La formule $\tilde{u}(x) = u(1 \otimes x)$ (pour $x \in A$) définit une bijection $u \mapsto \tilde{u}$ de l’ensemble des $K'$-homomorphismes de $A_{(K')}$ dans $L$ sur l’ensemble des $K$-homomorphismes de $A$ dans $L$, d’où (8).

Enfin, supposons que $K'$ soit une extension de degré fini de $K$; si $A'$ est une $K'$-algèbre commutative de degré fini, c’est aussi une $K$-algèbre commutative de degré fini et l’on a $[A' : K] = [A' : K'][K' : K]$ (V, p. 9, th. 1). Nous allons prouver la formule

$$
[A' : K]_s = [A' : K']_s \cdot [K' : K]_s .
$$

En effet, soit $S$ (resp. $T$) l’ensemble des $K$-homomorphismes de $K'$ (resp. $A'$) dans une clôture algébrique $L$ de $K$; pour tout $\sigma \in S$, notons $T_\sigma$ l’ensemble des éléments $f$ de $T$ tels que $f(\alpha . 1) = \sigma(\alpha)$ pour tout $\alpha \in K'$. Alors la famille $(T_\sigma)_{\sigma \in S}$ est une partition de $T$, et l’on a Card $S = [K' : K]_s$; or, pour tout $\sigma \in S$, l’ensemble $T_\sigma$ se compose des $K'$-homomorphismes de $A'$ dans l’extension algébriquement close $(L, \sigma)$ de $K'$, d’où Card $T_\sigma = [A' : K']_s$. On a ainsi prouvé (9).

#### Proposition 4 {#alg-v-s6-prop-4 .statement}

*Soit $A$ une algèbre commutative de degré fini sur $K$. On a* $[A : K]_s \leq [A : K]$, *avec égalité si et seulement si* $A$ *est étale*.

Soient $\Omega$ une clôture algébrique de $K$ et $\mathcal{H}$ l’ensemble des homomorphismes d’algèbres de $A$ dans $\Omega$. On a Card $\mathcal{H} = [A : K]_s$, et $A$ est étale si et seulement si $A$ est diagonalisée par l’extension $\Omega$ de $K$ (V, p. 29, prop. 2). La prop. 4 résulte alors du cor. de V, p. 29.

#### Corollaire 1 {#alg-v-s6-prop-4-cor-1 .statement}

*Soient $A$ et $B$ deux algèbres commutatives sur $K$, de degrés finis non nuls. Pour que l’algèbre $C = A \otimes_K B$ soit étale, il faut et il suffit que* $A$ *et* $B$ *soient étales*.

On a $[C : K] = [A : K] \cdot [B : K]$ et la formule analogue (7) pour les degrés séparables. De plus, on a $[A : K]_s \leq [A : K]$ et des formules analogues pour $B$ et $C$. Il en résulte qu’on a $[C : K] = [C : K]_s$ si et seulement si l’on a à la fois $[A : K] = [A : K]_s$ et $[B : K] = [B : K]_s$; il suffit alors d’appliquer la prop. 4.

#### Corollaire 2 {#alg-v-s6-prop-4-cor-2 .statement}

*Soit $K'$ une extension de $K$.*
    *a)* *Pour qu’une $K$-algèbre $A$ soit étale, il faut et il suffit que la $K'$-algèbre $A_{(K')}$ soit étale.*
    *b)* *Soit $A'$ une algèbre sur $K'$, non réduite à 0. Pour que $A'$ soit étale sur $K$, il faut et il suffit que $A'$ soit étale sur $K'$ et que $K'$ soit étale sur $K$.*
    On raisonne comme dans le cor. 1, en appliquant cette fois les formules (8) pour *a)* et (9) pour *b)*.

### 6. Caractérisation différentielle des algèbres étales

#### Théorème 3 {#alg-v-s6-thm-3 .statement}

*Soit $A$ une algèbre commutative de degré fini sur $K$. Pour que $A$ soit étale, il faut et il suffit que le module $\Omega_K(A)$ des $K$-différentielles de $A$ soit réduit à 0.*
    *A)* Soit $L$ une clôture algébrique de $K$ (V, p. 22, th. 2). Pour que $A$ soit étale, il faut et il suffit que l’algèbre $A_{(L)}$ sur $L$ soit diagonalisable (V, p. 29, prop. 2). De plus, le $A$-module $\Omega_L(A_{(L)})$ est isomorphe à $\Omega_K(A) \otimes_A A_{(L)}$ (III, p. 136, prop. 20), donc à $\Omega_K(A) \otimes_K L$ d’après l’associativité du produit tensoriel ; par suite, $\Omega_K(A) = 0$ équivaut à $\Omega_L(A_{(L)}) = 0$. Pour prouver le th. 3, il suffit donc de considérer le cas où $K$ est algébriquement clos et de montrer que l’algèbre $A$ est diagonalisable si et seulement si l’on a $\Omega_K(A) = 0$.
    *B)* Supposons $A$ diagonalisable ; alors (V, p. 28, prop. 1), l’espace vectoriel $A$ est engendré par les idempotents de $A$. L’assertion $\Omega_K(A) = 0$ résulte alors du lemme suivant :
    *Lemme 2.* — *Soient $A$ une algèbre commutative sur $K$ et $e$ un idempotent de $A$. On a $de = 0$ dans $\Omega_K(A)$.*
    De la relation $e = e^2$, on déduit $de = 2e.de$; par multiplication par $e$, on en déduit $e.de = 2e^2.de = 2e.de$, d’où $e.de = 0$. Finalement, on a $de = 2e.de = 0$.
    *C)* Nous démontrerons d’abord deux lemmes :
    *Lemme 3.* — *Soit $A$ une algèbre commutative de degré fini sur le corps algébriquement clos $K$, telle que $\Omega_K(A) = 0$. On a $m = m^2$ pour tout idéal maximal $m$ de $A$.*
    L’algèbre $A/m$ est une extension de degré fini du corps algébriquement clos $K$, d’où $[A/m : K] = 1$. Pour tout $a \in A$, il existe donc un unique scalaire $\lambda$ tel que $a - \lambda.1$ appartienne à $m$; notons $D(a)$ la classe de $a - \lambda.1$ modulo $m^2$. Il est immédiat que $D$ est une $K$-dérivation de $A$ dans le $A$-module $m/m^2$. La propriété universelle de $\Omega_K(A)$ (III, p. 134) et l’hypothèse $\Omega_K(A) = 0$ entraînent $D = 0$, d’où $m/m^2 = 0$ et finalement $m = m^2$.
    *Lemme 4.* — *Soit $A$ un anneau commutatif et soit $a$ un idéal de type fini de $A$ tel que $a = a^2$. Il existe un idempotent $e$ de $A$ tel que $a = Ae$.*

Soit $(a_1, \ldots, a_r)$ un système générateur de l’idéal $a$; comme on $a a = a^2$, il existe des éléments $x_{ij}$ de $a$ tels que $a_i = \sum_{j=1}^r x_{ij} a_j$ pour $1 \leq i \leq r$. Notons $M$ la matrice carrée d’ordre $r$ dont les éléments sont $\delta_{ij} - x_{ij}$ et soit $D$ son déterminant. Il existe (III, p. 99, formule (26)) une matrice carrée $N$ d’ordre $r$ à éléments dans $A$ telle que $N.M = D.I_r$, d’où immédiatement $Da_j = 0$ pour $1 \leq j \leq r$ et finalement $Da = 0$. Or la matrice $M$ est congrue à $I_r$ modulo $a$, d’où $D \equiv 1$ mod. $a$. Posons $e = 1 - D$; on a $e \in a$ et $ex = x$ pour tout $x \in a$. On en déduit que $e$ est un idempotent et que $a$ est égal à $Ae$.

Ces lemmes étant prouvés, montrons par récurrence sur le degré de $A$ que $A$ est diagonalisable si $K$ est algébriquement clos et si $\Omega_K(A) = 0$. Soit $m$ un idéal maximal de $A$ (I, p. 99). D’après les lemmes 3 et 4, il existe un idempotent $e$ tel que $m = Ae$; on a vu que $A/m$ est de degré 1 sur $K$. Alors $A$ est somme directe des idéaux $a = (1 - e)A$ et $m$, et l’on a $[a : K] = 1$, donc $A$ est isomorphe à $K \times A/a$. Comme $\Omega_K(A/a)$ est isomorphe à un quotient de $\Omega_K(A)$ (III, p. 137, prop. 22), il est nul et l’hypothèse de récurrence montre que $A/a$ est diagonalisable. Ceci prouve que $A$ est diagonalisable.

### 7. Algèbres réduites et algèbres étalées

#### Définition 2 {#alg-v-s6-def-2 .statement}

Soit $A$ un anneau commutatif. On dit que $A$ est réduit si tout élément nilpotent (I, p. 93) de $A$ est nul.

Si $A$ est un corps, ou un anneau intègre, ou un produit d’anneaux réduits, c’est un anneau réduit. Pour qu’un anneau commutatif $A$ soit réduit, il faut et il suffit que l’on ait $a^2 \neq 0$ pour tout $a \neq 0$ dans $A$ : en effet, on déduit de là, par récurrence sur $n$, $a^{2^n} \neq 0$ d’où $a^n \neq 0$ pour tout $a \neq 0$ dans $A$.

On dit qu’une algèbre commutative est réduite si l’anneau sous-jacent est réduit.

#### Proposition 5 {#alg-v-s6-prop-5 .statement}

Soit $A$ une algèbre commutative de degré fini sur $K$. Pour que $A$ soit réduite, il faut et il suffit qu’il existe des extensions $L_1, \ldots, L_n$ de degré fini de $K$ telles que $A$ soit $K$-isomorphe à $L_1 \times \cdots \times L_n$.

La condition énoncée est évidemment suffisante.

Réciproquement, supposons $A$ réduite ; en raisonnant par récurrence sur le degré de $A$, on voit qu’il suffit de prouver que, si $A$ n’est pas un corps, il existe deux algèbres $A_1$ et $A_2$ non nulles telles que $A$ soit isomorphe à $A_1 \times A_2$, ou encore qu’il existe dans $A$ un idempotent différent de 0 et 1.

Supposons désormais que $A$ soit réduite et ne soit pas un corps. Parmi les idéaux de $A$ différents de 0 et de $A$, soit $a$ un idéal dont la dimension comme $K$-espace vectoriel soit minimale. Pour tout $x \neq 0$ dans $a$, on a $x^2 \neq 0$, car $A$ est réduite, d’où $a^2 \neq \{0\}$. On a $a^2 \subset a$ et le caractère minimal de $a$ entraîne $a^2 = a$. D’après le lemme 4, il existe un idempotent $e$ tel que $a = Ae$, et l’on a $e \neq 0, e \neq 1$ car $a$ est distinct de 0 et $A$.

#### Théorème 4 {#alg-v-s6-thm-4 .statement}

Soit $A$ une algèbre commutative de degré fini $A$ sur $K$. Les assertions suivantes sont équivalentes :

a) L’algèbre $A$ est étale.
b) Pour toute extension $L$ de $K$, l’anneau $L \otimes_K A$ est réduit.
c) Il existe un surcorps parfait $P$ de $K$ tel que l’anneau $P \otimes_K A$ soit réduit.
*d) Il existe des extensions algébriques séparables $L_1, ..., L_n$ de $K$ telles que $A$ soit isomorphe à $L_1 \times \cdots \times L_n$.
En particulier, toute algèbre étale est réduite.

A) Démontrons d’abord l’équivalence de a), b) et c).
Supposons $A$ étale et soit $L$ une extension de $K$. Soit $\Omega$ un surcorps algébriquement clos de $L$ (V, p. 22, th. 2). Alors, $L \otimes_K A$ est isomorphe à un sous-anneau de $\Omega \otimes_K A$ et ce dernier est isomorphe à un anneau $\Omega^n$ d’après la prop. 2 (V, p. 29). Par suite, l’anneau $L \otimes_K A$ est réduit.
On a donc prouvé que a) entraîne b), et c) est un cas particulier de b). Plaçons-nous dans les hypothèses de c). Pour que la $K$-algèbre $A$ soit étale, il faut et il suffit que la $P$-algèbre $A_{(P)}$ soit étale (V, p. 32, cor. 2). L’algèbre $A$ est donc étale d’après le lemme suivant :

#### Lemme 5 {#alg-v-s6-lem-5 .statement}

Soit $B$ une algèbre réduite, de degré fini sur le corps parfait $P$. Alors $B$ est étale.
D’après la prop. 5, il existe des extensions $L_1, ..., L_n$ de $P$ telles que $B$ soit isomorphe à l’algèbre $L_1 \times \cdots \times L_n$. Comme un produit fini d’algèbres étales est étale (V, p. 30, cor.), il suffit d’examiner le cas où $B$ est une extension de $P$. D’après le th. 3 (V, p. 32), il suffit de prouver que l’on a $dx = 0$ dans $\Omega_P(B)$ pour tout $x \in B$.
Soit $x \in B$; comme $B$ est de degré fini sur $K$, $x$ est algébrique sur $K$ (V, p. 17, prop. 2). Soit $f$ le polynôme minimal de $x$ et soit $f'$ la dérivée de $f$. Le polynôme $f$ est non constant. Supposons qu’on ait $f' = 0$; d’après V, p. 8, cor., le corps $P$ est de caractéristique $p \neq 0$, et l’on a $f \in P[X^p]$; comme $P$ est parfait, on a $P[X^p] = P[X]^p$, mais le polynôme irréductible $f$ ne peut appartenir à $P[X]^p$.
On a donc $f' \neq 0$ et comme le degré de $f'$ est strictement plus petit que celui de $f$, on a $f'(x) \neq 0$. Or, de $f(x) = 0$, on déduit $f'(x).dx = 0$ dans $\Omega_P(B)$, d’où $dx = 0$, ce qu’il fallait démontrer.

*B*) Supposons que $A$ soit étale ; d’après l’équivalence de a) et b), l’algèbre $A$ est réduite, et il existe donc des extensions $L_1, ..., L_n$ de $K$ telles que $A$ soit isomorphe à l’algèbre $L_1 \times \cdots \times L_n$ (prop. 5). Comme $A$ est étale, chacune des extensions $L_i$ est une algèbre étale (V, p. 30, cor.), donc est par définition une extension algébrique séparable de $K$.
L’implication $d) \Rightarrow a)$ résulte de V, p. 30, cor. \*

#### Corollaire {#alg-v-s6-n7-cor-1 .statement}

Supposons $K$ de caractéristique $p \neq 0$. Pour que $A$ soit étale, il faut et il suffit que l’on ait $A = K[A^p]$. Pour toute base $(a_i)_{i \in I}$ de $A$ sur $K$, la famille $(a_i^p)_{i \in I}$ est alors une base de $A$ sur $K$.

Choisissons une clôture algébrique $\Omega$ de $K$. Soient $u$ et $v$ deux $K$-homomorphismes de $A$ dans $\Omega$; si $u$ et $v$ ont même restriction à $K[A^p]$, on a
$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p, \text{ d'où } u(x) = v(x)
$$
pour tout $x \in A$. On a donc l’inégalité $[A : K]_s \leq [K[A^p] : K]_s$; si $A$ est étale, on a alors
$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$
d’où $A = K[A^p]$.

Réciproquement, supposons que l’on ait $A = K[A^p]$; soit $(a_i)_{i \in I}$ une base de $A$ sur $K$. D’après V, p. 4, prop. 2, $b$, la famille $(a_i^p)_{i \in I}$ engendre le $K$-espace vectoriel $K[A^p]$, et comme $A = K[A^p]$ est de dimension finie égale au cardinal de $I$, la famille $(a_i^p)_{i \in I}$ est une base de $A$ sur $K$. Soit $u$ un élément de $\Omega \otimes_K A$ tel que $u^2 = 0$, d’où $u^p = 0$; comme $(a_i)_{i \in I}$ est une base de $A$ sur $K$, il existe une famille $(\lambda_i)_{i \in I}$ d’éléments de $\Omega$ telle que $u = \sum_{i \in I} \lambda_i \otimes a_i$, d’où $u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p$; comme $(a_i^p)_{i \in I}$ est une base de $A$ sur $K$ et $u^p = 0$, on a donc $\lambda_i^p = 0$, d’où $\lambda_i = 0$ pour tout $i \in I$, et finalement $u = 0$. On a montré que l’anneau $\Omega \otimes_K A$ est réduit ; comme le corps $\Omega$ est parfait, l’algèbre $A$ sur $K$ est étale d’après le th. 4.

Pour une autre caractérisation des algèbres étales, voir V, p. 47, prop. 1.

## EXERCICES {#alg-v-s6-exercises}

See the [exercises for § 6](exercises/s6/).
