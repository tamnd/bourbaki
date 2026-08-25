---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 5
section_title: Séparation des ensembles convexes
lang: fr
source: evt-i-v-fr
book_pages: EVT II.39-EVT II.43, EVT II.81-EVT II.86
pdf_pages: 0074-0078, 0116-0121
extraction: ocr
subsections:
    - "no": 1
      title: Le théorème de Hahn-Banach (forme géométrique)
      page: 39
      pdf_page: 74
    - "no": 2
      title: Séparation des ensembles convexes dans un espace vectoriel topologique
      page: 39
      pdf_page: 74
    - "no": 3
      title: Séparation des ensembles convexes dans un espace localement convexe
      page: 41
      pdf_page: 76
    - "no": 4
      title: Approximation des fonctions convexes
      page: 42
      pdf_page: 77
statements: 24
exercises: 30
content_sha256: 3cced2bb65f66fe5bc8603a35c5374d0dd15f5390e882e6a1e5fbfc228729e11
---

## § 5. SÉPARATION DES ENSEMBLES CONVEXES

### 1. Le théorème de Hahn-Banach (forme géométrique)

#### Théorème 1 (Hahn-Banach) {#evt-ii-s5-thm-1 .statement}

Soient E un espace vectoriel topologique, A un ensemble ouvert convexe non vide dans E, M une variété linéaire non vide ne rencontrant pas A. Il existe alors un hyperplan fermé H contenant M et ne rencontrant pas A.

Par translation on peut se ramener au cas où $0 \in A$, de sorte que A est absorbant. Soit $p$ la jauge de l’ensemble ouvert convexe absorbant A (II, p. 22), de sorte que A est l’ensemble des $x \in E$ tels que $p(x) < 1$. Soit d’autre part V le sous-espace vectoriel de E engendré par M ; M est donc un hyperplan dans V ne passant pas par 0, et il y a par suite une forme linéaire et une seule $f$ sur V telle que M soit l’ensemble des $y \in V$ tels que $f(y) = 1$. L’hypothèse $M \cap A = \varnothing$ entraîne donc que pour tout $y \in V$ tel que $f(y) = 1$, on a $p(y) \geqslant 1$; comme $f$ et $p$ sont positivement homogènes, on a donc $f(y) \leqslant p(y)$ pour tout $y \in V$ tel que $f(y) > 0$; comme de plus $p(y) \geqslant 0$ pour tout $y \in V$, on voit finalement que l’on a $f(y) \leqslant p(y)$ pour tout $y \in V$. En vertu de la forme analytique du th. de Hahn-Banach (II, p. 24, th. 1), il existe une forme linéaire $h$ sur E prolongeant $f$ et telle que, pour tout $x \in E$, on ait $h(x) \leqslant p(x)$. Soit alors H l’hyperplan dans E, d’équation $h(x) = 1$. Il est clair que $H \cap V = M$ et que $H \cap A = \varnothing$. D’autre part, le complémentaire de H dans E contient un ensemble ouvert non vide A, donc H est fermé dans E (I, p. 11, corollaire).

C.Q.F.D.

#### Remarque 1 {#evt-ii-s5-n1-rem-1 .statement}

Lorsque $0 \in M$, le th. 1 peut encore s’énoncer de la façon suivante : *il existe une forme linéaire g continue dans E, telle que $g(x) = 0$ dans M et $g(x) > 0$ dans A* (II, p. 9, prop. 4).

#### Remarque 2 {#evt-ii-s5-n1-rem-2 .statement}

Si l’on applique le th. 1 au cas où E est muni de la topologie localement convexe la plus fine (II, p. 27, Exemple 2), et si pour simplifier on suppose que $0 \in A$, on obtient le résultat suivant (où en apparence il n’intervient plus de topologie) : dans un espace vectoriel réel E, si A est un ensemble convexe *absorbant*, et M une variété linéaire non vide ne rencontrant pas A, alors il existe un hyperplan H contenant M et tel que A soit d’un même côté de H. Ce résultat n’est pas valable pour un ensemble convexe A quelconque (II, p. 69, exerc. 5).

### 2. Séparation des ensembles convexes dans un espace vectoriel topologique

#### Définition 1 {#evt-ii-s5-def-1 .statement}

*Deux parties non vides A, B d’un espace vectoriel topologique réel E sont dites séparées par un hyperplan fermé H, si A est contenu dans un des demi-espaces fermés déterminés par H, et B dans l’autre demi-espace fermé.*

#### Définition 2 {#evt-ii-s5-def-2 .statement}

*Deux parties non vides A, B d’un espace vectoriel topologique réel E sont dites strictement séparées par un hyperplan fermé H, si A est contenu dans un des demi-espaces ouverts déterminés par H, et B dans l’autre demi-espace ouvert.*

#### Proposition 1 {#evt-ii-s5-prop-1 .statement}

Dans un espace vectoriel topologique réel E, soient A un ensemble ouvert convexe non vide, et B un ensemble convexe non vide ne rencontrant pas A ; il existe alors un hyperplan fermé H séparant A et B.

En effet, l’ensemble C = A − B est ouvert, convexe (II, p. 10, prop. 7) et non vide, et l’on a 0 ∉ C. En vertu du th. 1 de II, p. 39, il existe donc une forme linéaire continue f ≠ 0 sur E, telle que f(z) > 0 dans C. Alors, pour tout x ∈ A et tout y ∈ B, on a f(x) > f(y). Posons α = inf_{x∈A} f(x) ; α est fini, et l’on a f(x) ≥ α pour tout x ∈ A et f(y) ≤ α pour tout y ∈ B ; l’hyperplan fermé H d’équation f(z) = α sépare donc A et B.

#### Remarque 1 {#evt-ii-s5-n2-rem-1 .statement}

L’hyperplan H ne rencontre pas A (II, p. 16, prop. 17) ; si A et B sont deux ensembles convexes ouverts non vides sans point commun, il existe donc un hyperplan fermé qui sépare strictement A et B.
2) Par contre, lorsque B n’est pas ouvert, il n’existe pas nécessairement d’hyperplan fermé séparant strictement A et B, même si E est de dimension finie, et si $\overline{A}$ et $\overline{B}$ ne se rencontrent pas (II, p. 83, exerc. 12).

#### Définition 3 {#evt-ii-s5-def-3 .statement}

Dans un espace vectoriel E, on appelle hyperplan d’appui d’une partie A de E, un hyperplan H contenant au moins un point de A et tel que tous les points de A soient d’un même côté de H.

Soit f une forme linéaire ≠ 0 sur E ; dire que l’hyperplan d’équation f(x) = α est un hyperplan d’appui de A signifie que α est le plus petit élément, ou le plus grand élément, de l’ensemble f(A) ⊂ R. Autrement dit, pour qu’il existe un hyperplan d’appui de A parallèle à l’hyperplan d’équation f(x) = 0, il faut et il suffit que l’une des bornes de l’ensemble f(A) soit finie et appartienne à f(A).

#### Proposition 2 {#evt-ii-s5-prop-2 .statement}

Soient E un espace vectoriel topologique, A un ensemble compact non vide dans E. Pour tout hyperplan fermé H dans E, il existe un hyperplan d’appui de A parallèle à H.

En effet, si f(x) = γ est une équation de H, où f est une forme linéaire continue dans E, la restriction de f à A est continue, donc est bornée et atteint ses bornes dans A (TG, IV, p. 27, th. 1).

Cette démonstration prouve qu’il existe un ou deux hyperplans d’appui de A parallèles à H, le premier cas ne pouvant se présenter que si A est contenu tout entier dans un hyperplan parallèle à H.

#### Proposition 3 {#evt-ii-s5-prop-3 .statement}

Dans un espace vectoriel topologique E, soit A un ensemble convexe fermé d’intérieur non vide. Tout hyperplan d’appui de A est fermé, et tout point frontière de A appartient à un hyperplan d’appui de A au moins.

Tout hyperplan d’appui de A est fermé, puisque tous les points de A sont d’un même côté d’un tel hyperplan (II, p. 16, prop. 17). D’autre part, si x_0 est point frontière de A, x_0 n’appartient pas à l’ensemble convexe ouvert non vide $\overset{\circ}{A}$ ; d’après le th. 1 de II, p. 39, il existe un hyperplan H passant par x_0 et ne rencontrant pas $\overset{\circ}{A}$. Comme A est l’adhérence de $\overset{\circ}{A}$ (II, p. 15, cor. 1 de la prop. 16), il résulte de la prop. 17 de II, p. 16 que H est un hyperplan d’appui de A.

### 3. Séparation des ensembles convexes dans un espace localement convexe

#### Proposition 4 {#evt-ii-s5-prop-4 .statement}

Soient E un espace localement convexe, A un ensemble convexe fermé non vide dans E, K un ensemble convexe compact non vide dans E, ne rencontrant pas A. Il existe alors un hyperplan fermé H qui sépare strictement A et K.

En effet, il existe un voisinage ouvert convexe V de 0 dans E tel que A + V et K + V ne se rencontrent pas (TG, II, p. 31, prop. 4). Comme A + V et K + V sont ouverts et convexes dans E, la prop. 1 de II, p. 40 montre qu’il existe un hyperplan fermé H séparant strictement A + V et K + V, et a fortiori A et K.

#### Remarque {#evt-ii-s5-n3-rem-1 .statement}

Si A et B sont deux ensembles convexes fermés non vides sans point commun dans un espace localement convexe séparé E, il existe un hyperplan fermé qui les sépare lorsque E est de dimension finie (II, p. 83, exerc. 13) ; mais cette conclusion n’est plus nécessairement exacte lorsque E est de dimension infinie (II, p. 83, exerc. 10 et 11).

#### Corollaire 1 {#evt-ii-s5-prop-4-cor-1 .statement}

Dans un espace localement convexe, tout ensemble convexe fermé A est l’intersection des demi-espaces fermés qui le contiennent.

En effet, pour tout point x $\notin$ A, il existe, d’après la prop. 4, un hyperplan fermé séparant strictement x et A.

#### Corollaire 2 {#evt-ii-s5-prop-4-cor-2 .statement}

Dans un espace localement convexe séparé, tout ensemble convexe compact A est l’intersection des demi-espaces fermés qui le contiennent et qui sont déterminés par les hyperplans d’appui de A.

En effet, soit $x_0 \notin A$; $\{x_0\}$ est fermé, donc il existe un hyperplan fermé H séparant strictement $x_0$ et A (prop. 4); soit $f(x) = \alpha$ une équation de H ($f$ forme linéaire continue), et supposons que $f(x) > \alpha$ pour tout $x \in A$. Si l’on pose $\gamma = \inf_{x \in A} f(x)$, le demi-espace défini par $f(x) \geq \gamma$ contient A, est déterminé par l’hyperplan d’appui d’équation $f(x) = \gamma$, et ne contient pas $x_0$; d’où le corollaire.

Dans un espace localement convexe, un ensemble convexe fermé, non compact et n’ayant pas de point intérieur, peut n’avoir aucun hyperplan d’appui fermé (II, p. 91, exerc. 18 ; cf. aussi V, p. 71, exerc. 11).

#### Corollaire 3 {#evt-ii-s5-prop-4-cor-3 .statement}

Dans un espace localement convexe, l’adhérence de toute variété linéaire M est l’intersection des hyperplans fermés qui contiennent M.

En effet, pour tout $x \notin \overline{M}$, soit H un hyperplan fermé séparant strictement x et $\overline{M}$; $\overline{M}$ est donc parallèle à H ; l’hyperplan fermé $H_1$ contenant $\overline{M}$ et parallèle à H ne contient pas x, d’où le corollaire.

#### Corollaire 4 {#evt-ii-s5-prop-4-cor-4 .statement}

Soit C un ensemble convexe fermé dans un espace localement convexe E. Pour qu’une partie A de E soit contenue dans C, il faut et il suffit que, pour toute fonction numérique affine continue u dans E telle que $u(x) \geq 0$ pour tout x dans C, on ait $u(y) \geq 0$ pour tout y dans A.

La condition est évidemment nécessaire. Montrons inversement qu’elle est suffisante ; si un point $x \in A$ n’est pas contenu dans $C$, il existe un hyperplan fermé d’équation $f(z) = \alpha$ séparant strictement $x$ et $C$; si l’on suppose par exemple que $f(x) < \alpha$, la fonction affine continue $u = f - \alpha$ contredit l’hypothèse.

#### Corollaire 5 {#evt-ii-s5-prop-4-cor-5 .statement}

Dans un espace localement convexe $E$, l’adhérence de tout cône convexe $C$ de sommet 0 est l’intersection de demi-espaces fermés contenant $C$ déterminés par des hyperplans fermés passant par 0.

En effet, $\overline{C}$ est un cône convexe de sommet 0 (II, p. 14, prop. 14). Pour tout $x \notin \overline{C}$, il existe un hyperplan fermé $H$ séparant strictement $x$ et $\overline{C}$ (prop. 4). Il suffit maintenant d’appliquer le lemme suivant :

#### Lemme 1 {#evt-ii-s5-lem-1 .statement}

Si un cône $A$ de sommet 0 est contenu dans un demi-espace ouvert déterminé par un hyperplan $H$, il est contenu dans un demi-espace fermé déterminé par l’hyperplan $H_0$ parallèle à $H$ et passant par 0.

En effet, soit $f(z) = \alpha$ avec $\alpha < 0$ une équation de $H$, de sorte que $f(z) = 0$ est l’équation de $H_0$. S’il existait un $z \in A$ tel que $f(z) < 0$, il existerait un $\lambda > 0$, tel que $f(\lambda z) = \alpha$, et comme $\lambda z \in A$, cela contredirait l’hypothèse.

### 4. Approximation des fonctions convexes

#### Proposition 5 {#evt-ii-s5-prop-5 .statement}

Soient $X$ un ensemble convexe fermé dans un espace localement convexe. Alors toute fonction convexe semi-continue inférieurement $f$ dans $X$ est l’enveloppe supérieure d’une famille de fonctions qui sont des restrictions à $X$ de fonctions linéaires affines continues dans $E$.

En effet, l’ensemble $A \subset E \times \mathbf{R}$ des points $(x, t)$ tels que $x \in X$ et $t \geqslant f(x)$ est convexe (II, p. 18, prop. 19) et fermé, puisque la fonction $(x, t) \mapsto f(x) - t$ est semi-continue inférieurement. Soit alors $x$ un point quelconque de $X$, et soit $a \in \mathbf{R}$ tel que $a < f(x)$. En vertu du cor. 1 de II, p. 41, il existe dans $E \times \mathbf{R}$ un hyperplan fermé $H$ contenant $(x, a)$ et ne rencontrant pas $A$. Toute forme linéaire continue sur $E \times \mathbf{R}$ étant de la forme

$$
(z, t) \mapsto u(z) + \lambda t ,
$$

où $\lambda \in \mathbf{R}$ et $u$ est une forme linéaire continue dans $E$, $H$ a une équation de la forme $u(z) + \lambda t = \alpha$, et comme $H$ passe par $(x, a)$, on a $\alpha = u(x) + \lambda a$. On ne peut avoir $\lambda = 0$, car $H$ aurait pour équation $u(z - x) = 0$, ce qui est absurde puisque le point $(x, f(x)) \in A$ n’appartient pas à $H$. En divisant au besoin par $-\lambda$, on peut donc supposer que $H$ a pour équation $t - a = u(z - x)$. Comme $f(x) - a > 0$, on a donc $f(z) > u(z - x) + a$ pour tout $z \in X$, ce qui prouve le corollaire.

#### Remarque 1 {#evt-ii-s5-n4-rem-1 .statement}

Il résulte de la prop. 5 que $f$ est l’enveloppe supérieure d’une famille filtrante croissante de fonctions qui sont des restrictions à $X$ de fonctions convexes continues dans $E$.

#### Remarque 2 {#evt-ii-s5-n4-rem-2 .statement}

Supposons de plus que $X$ soit un cône (convexe fermé) de sommet 0 et que $f$ soit positivement homogène. Alors $f$ est l’enveloppe supérieure d’une famille de fonctions qui sont des restrictions à X de formes linéaires continues dans E. En effet, soit $(u_\alpha)$ une famille de fonctions linéaires affines continues dans E dont les restrictions à X ont pour enveloppe supérieure $f$. Posons $u_\alpha = v_\alpha + \lambda_\alpha$, où $\lambda_\alpha \in \mathbf{R}$, et où $v_\alpha$ est une forme linéaire continue dans E. On a $\lambda_\alpha = u_\alpha(0) \leq f(0) = 0$. D’autre part, si $x \in X$, on a, pour tout $\mu > 0$,

$$
\mu^{-1}\lambda_\alpha + v_\alpha(x) = \mu^{-1}(\lambda_\alpha + v_\alpha(\mu x)) = \mu^{-1}u_\alpha(\mu x) \leq \mu^{-1}f(\mu x) = f(x)
$$

donc $u_\alpha \leq v_\alpha \leq f$ dans X, de sorte que $f$ est l’enveloppe supérieure des $v_\alpha$.

#### Remarque 3 {#evt-ii-s5-n4-rem-3 .statement}

La restriction à X d’une fonction affine continue dans E est une fonction affine (i.e. à la fois concave et convexe (II, p. 18)) dans X ; mais il peut exister des fonctions continues affines dans un ensemble compact convexe $X \subset E$, qui ne sont pas des restrictions à X de fonctions affines continues dans E (II, p. 83, exerc. 11, c)). Toutefois :

#### Proposition 6 {#evt-ii-s5-prop-6 .statement}

Soient E un espace localement convexe séparé, X un ensemble convexe compact dans E, $f$ une fonction affine semi-continue supérieurement dans X. Soit L l’ensemble des restrictions à X des fonctions affines continues dans E ; l’ensemble $L'$ des $h \in L$ telles que l’on ait $h(x) > f(x)$ pour tout $x \in X$ est alors filtrant décroissant, et son enveloppe inférieure est égale à $f$.

On peut se limiter au cas où X est non vide. Soient $u, v$ deux éléments de L tels que $u(x) > f(x)$ et $v(x) > f(x)$ pour tout $x \in X$, et soit $b$ une constante qui majore $u$ et $v$. Soit U (resp. V) l’ensemble convexe compact des points $(x, t)$ de $X \times \mathbf{R}$ tels que $u(x) \leq t \leq b$ (resp. $v(x) \leq t \leq b$), et soit F l’ensemble des $(x, t) \in X \times \mathbf{R}$ tels que $t \leq f(x)$ ; F est convexe et fermé dans $X \times \mathbf{R}$. L’enveloppe convexe K de $U \cup V$ ne rencontre pas F, car $U \cup V$ est contenu dans l’ensemble des $(x, t) \in X \times \mathbf{R}$ tels que $f(x) < t$, ensemble qui est convexe et ne rencontre pas F. Comme K est compact (II, p. 14, prop. 15), on peut séparer strictement F et K par un hyperplan fermé H de $E \times \mathbf{R}$. Pour tout $x \in X$, H sépare strictement les points $(x, f(x))$ et $(x, b)$, donc rencontre la droite $\{x\} \times \mathbf{R}$ en un seul point $w(x)$ ; par suite H est le graphe d’une fonction affine continue dont la restriction $w$ à X appartient à L, minore $u$ et $v$ et vérifie l’inégalité $w(x) > f(x)$ pour tout $x \in X$. Ceci prouve que l’ensemble $L'$ est filtrant décroissant. La prop. 5 de II, p. 42, appliquée à $-f$, prouve que $f$ est l’enveloppe inférieure de $L'$.

#### Corollaire {#evt-ii-s5-n4-cor-1 .statement}

Soit $f$ une fonction affine continue dans X ; il existe alors une suite $(h_n)$ d’éléments de L qui converge uniformément vers $f$ dans X.

En effet, la prop. 6 et le th. de Dini (TG, X, p. 34, th. 1) montrent que pour tout $n$ il existe $h_n \in L$ telle que $f \leq h_n \leq f + 1/n$.

## EXERCICES {#evt-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
