---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 2
section_title: Espaces métriques ; espaces métrisables
lang: fr
source: top-v-x-fr
book_pages: TG IX.11-TG IX.23, TG IX.90-TG IX.98
pdf_pages: 0131-0143, 0210-0218
extraction: ocr
subsections:
    - "no": 1
      title: Distances et espaces métriques
      page: 11
      pdf_page: 131
    - "no": 2
      title: Structure d’espace métrique
      page: 12
      pdf_page: 132
    - "no": 3
      title: Oscillation d’une fonction
      page: 14
      pdf_page: 134
    - "no": 4
      title: Espaces uniformes métrisables
      page: 15
      pdf_page: 135
    - "no": 5
      title: Espaces topologiques métrisables
      page: 15
      pdf_page: 135
    - "no": 6
      title: Emploi des suites dénombrables
      page: 17
      pdf_page: 137
    - "no": 7
      title: Fonctions semi-continues sur un espace métrisable
      page: 18
      pdf_page: 138
    - "no": 8
      title: Espaces métrisables de type dénombrable
      page: 18
      pdf_page: 138
    - "no": 9
      title: Espaces métriques compacts; espaces métrisables compacts
      page: 20
      pdf_page: 140
    - "no": 10
      title: Espaces quotients des espaces métrisables
      page: 22
      pdf_page: 142
statements: 33
exercises: 9
content_sha256: 658f14178c1b033de38316d093be8112fa307402df703f83c48823dca01267d0
---

## § 2. ESPACES MÉTRIQUES; ESPACES MÉTRISABLES

### 1. Distances et espaces métriques

#### Définition 1 {#top-ix-s2-def-1 .statement}

On appelle distance sur un ensemble X un écart fini d sur X tel que la relation $d(x, y) = 0$ entraîne $x = y$. On appelle espace métrique un ensemble X muni de la structure définie par la donnée d’une distance sur X.

Un espace métrique X est toujours considéré comme muni de la structure uniforme et de la topologie définies par la distance donnée sur X.

#### Exemple 1 {#top-ix-s2-n1-exa-1 .statement}

La distance euclidienne $d(x, y)$ (VI, p. 7) est une distance sur l’espace numérique $\mathbf{R}^n$; il en est de même des fonctions $\sup_{1 \leq i \leq n} |x_i - y_i|$, et $\sum_{i=1}^n |x_i - y_i|$
Toutes ces distances sont équivalentes (IX, p. 2).

#### Exemple 2 {#top-ix-s2-n1-exa-2 .statement}

Sur un ensemble quelconque X, l’écart d défini par les relations $d(x, x) = 0$, $d(x, y) = 1$ pour $x \neq y$, est une distance ; la structure uniforme qu’elle définit sur X est la structure uniforme discrète.

On a une définition équivalente à la déf. 1 en disant qu’une distance est un écart fini tel que la structure uniforme définie par cet écart soit séparée ; un écart fini équivalent à une distance est donc une distance.

On peut rattacher aux espaces métriques les espaces uniformes définis par la donnée d’un seul écart (qu’on peut supposer fini) lorsque cet écart n’est pas une distance. Soit $f$ un tel écart sur un ensemble X, $\mathcal{U}$ la structure uniforme qu’il définit ; cette structure n’est pas séparée, et l’intersection des entourages de $\mathcal{U}$ est la partie de $X \times X$ définie par la relation d’équivalence $f(x, y) = 0$ ; nous désignerons cette relation par R. Si $x \equiv x'$ (mod. R), on a, d’après l’inégalité du triangle, $f(x, y) \leq f(x, x') + f(x', y) = f(x', y)$, et de même $f(x', y) \leq f(x, y)$ donc $f(x, y) = f(x', y)$ ; autrement dit, $f$ est une fonction compatible (en x et y) avec la relation d’équivalence R (E, II, p. 44). Soit $\tilde{f}$ la fonction obtenue par passage au quotient (pour x et y) à partir de $f$ ; elle est définie sur $(X/R) \times (X/R)$, et si $x$ et $y$ sont deux points de X, $\dot{x}$ et $\dot{y}$ les classes (mod. R) de x et de y respectivement, on a $\tilde{f}(\dot{x}, \dot{y}) = f(x, y)$. Il en résulte aussitôt que $\tilde{f}$ est une distance sur $X/R$, qu’on appelle distance associée à l’écart $f$; en outre, la structure uniforme qu’elle définit sur $X/R$ n’est autre que la structure uniforme séparée associée à $\mathcal{U}$, d’après la définition de cette structure (II, p. 25). En passant à un espace quotient convenable, la structure uniforme définie par un seul écart se ramène donc à une structure d’espace métrique.

La prop. 1 de IX, p. 5 détermine la structure du complété d’un espace métrique:

#### Proposition 1 {#top-ix-s2-prop-1 .statement}

*Soient $X$ un espace métrique, $d$ la distance sur $X$. Si $\hat{X}$ est le complété de $X$ (pour la structure uniforme définie par $d$), la fonction $d$ se prolonge par continuité à $\hat{X} \times \hat{X}$; la fonction prolongée $\bar{d}$ est une distance sur $\hat{X}$, et la structure uniforme de $\hat{X}$ est identique à la structure uniforme définie par la distance $\bar{d}$.

La prop. 1 de IX, p. 5, montre en effet que $\bar{d}$ est un écart fini sur $\hat{X}$, et y définit la structure uniforme obtenue par complétion; comme cette dernière est séparée, $\bar{d}$ est une *distance*.

Lorsqu’on considère le complété d’un espace métrique $X$ comme un espace métrique, on sous-entend toujours que la distance sur $\hat{X}$ est obtenue en prolongeant par continuité la distance sur $X$.

### 2. Structure d’espace métrique

Soient $X$ et $X'$ deux espaces métriques, $d$ la distance sur $X$, $d'$ la distance sur $X'$. Conformément aux définitions générales (E, IV, p. 6), une application bijective $f$ de $X$ sur $X'$ est un *isomorphisme* de la structure d’espace métrique de $X$ sur celle de $X'$, si, quels que soient $x \in X$ et $y \in X'$, on a

$$
d(x, y) = d'(f(x), f(y)).
$$

On remarquera que, si $f$ est une application de $X$ sur $X'$ satisfaisant à l’identité (1), elle est nécessairement *bijective*, et par suite est un isomorphisme de $X$ sur $X'$; un tel isomorphisme est encore appelé *isométrie* (ou application *isométrique*) de $X$ sur $X'$.

Une isométrie de $X$ sur $X'$ est bien entendu un isomorphisme de la structure uniforme (resp. topologie) de $X$ sur la structure uniforme (resp. topologie) de $X'$; les réciproques sont inexactes, comme le montre l’existence de distances équivalentes distinctes (IX, p. 3).

Soient $X$ un espace métrique, $d$ la distance qui le définit. Pour tout $a > 0$, on désignera par $V_a$ la partie de $X \times X$ formée des couples $(x, y)$ tels que $d(x, y) < a$, par $W_a$ la partie formée des couples $(x, y)$ tels que $d(x, y) \leq a$; lorsque $a$ parcourt l’ensemble des nombres $> 0$ (ou seulement une suite de nombres tendant vers 0), les ensembles $V_a$ (resp. $W_a$) constituent, d’après la continuité de $d$ (IX, p. 2), un système fondamental d’entourages *ouverts* (resp. *fermés*) de la structure uniforme de $X$; on a d’ailleurs $V_a \subset W_a$, mais ces deux ensembles ne sont pas nécessairement identiques.

Par analogie avec le cas de la distance euclidienne sur $\mathbf{R}^n$, l’ensemble $V_a(x)$ (resp. $W_a(x)$) est appelé boule ouverte (resp. boule fermée) de centre $x$ et de rayon $a$; c’est un ensemble ouvert (resp. fermé) dans $X$; de même, on appelle sphère de centre $x$ et de rayon $a$ l’ensemble des points $y$ tels que $d(x, y) = a$; c’est un ensemble fermé. D’après ce qui précède, les boules ouvertes (resp. fermées) de centre $x$ et de rayon $a$ forment un système fondamental de voisinages de $x$, lorsque $a$ parcourt l’ensemble des nombres $> 0$, ou une suite de nombres $> 0$ tendant vers $0$.

Il ne faut pas se laisser abuser par la terminologie précédente, et croire que, dans un espace métrique quelconque, les boules et sphères jouissent des mêmes propriétés que les boules et sphères euclidiennes étudiées dans VI, p. 9. C’est ainsi que l’adhérence d’une boule ouverte peut être distincte de la boule fermée de même centre et même rayon, que la frontière d’une boule fermée peut être distincte de la sphère de même centre et de même rayon, qu’une boule ouverte (ou fermée) peut ne pas être connexe, qu’une sphère peut être identique à l’ensemble vide (cf. IX, p. 91, exerc. 4).

Soient $A$ et $B$ deux parties non vides quelconques de l’espace métrique $X$. On appelle distance des ensembles $A$ et $B$ le nombre $d(A, B) = \inf_{x \in A,\ y \in B} d(x, y)$. En particulier, on note $d(x, A)$ la distance de l’ensemble $\{x\}$ réduit au point $x$, et de l’ensemble $A$; on l’appelle distance du point $x$ à l’ensemble $A$; on a donc
$$
d(x, A) = \inf_{y \in A} d(x, y),
$$
d’où
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
(IV, p. 21, prop. 9).

#### Remarque {#top-ix-s2-n2-rem-1 .statement}

Si $d(x, A) = a$, il se peut qu’il n’existe aucun point de $A$ dont la distance à $x$ soit égale à $a$. Toutefois, cette circonstance ne peut se présenter si $A$ est compact, car alors, en vertu du th. de Weierstrass (IV, p. 27, th. 1), il existe $y \in A$ tel que $d(x, A) = d(x, y)$.

#### Proposition 2 {#top-ix-s2-prop-2 .statement}

Les propriétés $d(x, A) = 0$ et $x \in \overline{A}$ sont équivalentes.

En effet, la propriété $d(x, A) = 0$ exprime que la boule $V_a(x)$ rencontre $A$ quel que soit $a > 0$, ce qui équivaut à $x \in \overline{A}$.

#### Proposition 3 {#top-ix-s2-prop-3 .statement}

La fonction $x \mapsto d(x, A)$ est uniformément continue dans $X$.

Soient en effet $x, y$ deux points quelconques de $X$; quel que soit $\varepsilon > 0$, il existe $z \in A$ tel que $d(y, z) \leq d(y, A) + \varepsilon$, d’où, en vertu de l’inégalité du triangle
$$
d(x, z) \leq d(x, y) + d(y, z) \leq d(x, y) + d(y, A) + \varepsilon.
$$
A fortiori $d(x, A) \leq d(x, y) + d(y, A) + \varepsilon$, et comme $\varepsilon$ est arbitraire, $d(x, A) \leq d(x, y) + d(y, A)$. De la même manière, on a
$$
d(y, A) \leq d(x, y) + d(x, A),
$$
c’est-à-dire
$$
|d(x, A) - d(y, A)| \leq d(x, y),
$$
d’où la proposition.

#### Remarque {#top-ix-s2-n2-rem-2 .statement}

On peut avoir $d(A, B) = 0$ pour deux parties $A, B$ de $X$ telles que $\overline{A} \cup \overline{B} = \varnothing$, lorsqu’aucune de ces deux parties n’est réduite à un point. Par exemple, sur la droite numérique $\mathbf{R}$, l’ensemble des entiers $> 0$, et l’ensemble des points de la suite $(n + 1/2n)_{n \geqslant 1}$ sont fermés, sans point commun, et ont une distance nulle.

Toutefois, si $A$ est compact et $B$ fermé, la relation $d(A, B) = 0$ entraîne $A \cap B \neq \varnothing$, car en vertu de la relation

$$
d(A, B) = \inf_{x \in A} d(x, B),
$$

de la prop. 3 et du th. de Weierstrass, il existe $x_0 \in A$ tel que $d(x_0, B) = d(A, B) = 0$, donc (IX, p. 13, prop. 2) $x_0 \in B$.

On appelle diamètre d’une partie non vide $A$ de $X$ le nombre (fini ou égal à $+\infty$) $\delta(A) = \sup_{x \in A, y \in A} d(x, y)$. La notion d’ensemble « petit d’ordre $W_a$ » (II, p. 12) est identique à celle d’ensemble de diamètre $\leq a$. Pour qu’un ensemble non vide $A$ soit réduit à un point, il faut et il suffit que $\delta(A) = 0$.

On dit qu’un ensemble $A \subset E$ est borné (pour la distance $d$) si son diamètre est fini. Il revient au même de dire que, pour tout point $x_0 \in E$, $A$ est contenu dans une boule de centre $x_0$. Toute partie d’un ensemble borné est un ensemble borné; la réunion d’une famille finie d’ensembles bornés est un ensemble borné.

On notera qu’une partie de $E$ peut être bornée pour la distance $d$, mais non bornée pour une distance équivalente à $d$ (cf. IX, p. 3).

### 3. Oscillation d’une fonction

A la notion de diamètre se rattache celle d’oscillation d’une fonction $f$ définie dans un ensemble quelconque $X$, et prenant ses valeurs dans un espace métrique $Y$; si $A$ est une partie non vide quelconque de $X$, on appelle oscillation de $f$ dans $A$ le diamètre $\delta(f(A))$.

Si en outre $X$ est une partie d’un espace topologique $Z$, on appelle oscillation de $f$ en un point $x \in \overline{X}$ le nombre $\omega(x; f) = \inf \delta(f(V \cap X))$, $V$ parcourant le filtre des voisinages de $x$ dans $Z$.

#### Proposition 4 {#top-ix-s2-prop-4 .statement}

L’oscillation $\omega(x; f)$ d’une fonction quelconque $f$ définie dans une partie $X$ d’un espace topologique $Z$, et prenant ses valeurs dans un espace métrique $Y'$, est une fonction semi-continue supérieurement dans $\overline{X}$.

Soit en effet $a$ un point quelconque de $\overline{X}$; pour tout $k > \omega(a; f)$, il existe un voisinage ouvert $V$ de $a$ tel que $\delta(f(V \cap X)) \leq k$; pour tout $x \in V \cap \overline{X}$, $V$ est un voisinage de $x$, donc

$$
\omega(x; f) \leq \delta(f(V \cap X)) \leq k,
$$

ce qui prouve que $\omega$ est semi-continue supérieurement au point $a$.

Pour qu’on ait $\omega(x; f) = 0$ en un point $x \in \overline{X}$, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un voisinage $V$ de $x$ tel que $f(V \cap X)$ soit contenu dans une boule de rayon $\varepsilon$; si $x \in X$, cette condition exprime que $f$ est continue au point $x$ (par rapport à $X$); si $x \in X \cap \mathcal{CX}$, elle exprime que l’image par $f$ de la trace sur $X$ du filtre des voisinages de $x$ dans $Z$ est une base de filtre de Cauchy sur $Y'$; en particulier:

#### Proposition 5 {#top-ix-s2-prop-5 .statement}

*Soit $f$ une fonction définie dans une partie $X$ d’un espace topologique $Z$, prenant ses valeurs dans un espace métrique complet $Y'$; pour qu’en un point $x \in \overline{X}$, $f$ ait une limite relativement à $X$, il faut et il suffit que l’osillation de $f$ au point $x$ soit nulle.*

### 4. Espaces uniformes métrisables

#### Définition 2 {#top-ix-s2-def-2 .statement}

*On dit qu’une distance sur un ensemble $X$ est compatible avec une structure uniforme $\mathcal{U}$ sur $X$ si la structure uniforme définie par cette distance est identique à $\mathcal{U}$.

On dit qu’une structure uniforme sur un ensemble $X$ est métrisable s’il existe une distance sur $X$ compatible avec cette structure. Un espace uniforme est dit métrisable si sa structure uniforme est métrisable.*

Des distances distinctes peuvent être compatibles avec une même structure uniforme; elles sont alors *équivalentes* (IX, p. 2, déf. 2). Rappelons que toute distance est équivalente à une distance *bornée* (IX, p. 3).

#### Théorème 1 {#top-ix-s2-thm-1 .statement}

*Pour qu’une structure uniforme soit métrisable, il faut et il suffit qu’elle soit séparée et que le filtre des entourages de cette structure ait une base dénombrable.*

La condition est *nécessaire*, car (avec la notation de IX, p. 12), les entourages $V_{1/n}(n \geqslant 1)$ forment une base du filtre des entourages de la structure uniforme d’un espace métrique.

La condition est *suffisante*, car si elle est remplie, la structure uniforme considérée est définie par un seul écart (qu’on peut supposer fini) d’après la prop. 2 de IX, p. 6, et comme elle est séparée, cet écart est une distance.

#### Corollaire 1 {#top-ix-s2-thm-1-cor-1 .statement}

*Une structure uniforme séparée définie par une famille dénombrable d’écart est métrisable.*

En effet, si $(f_n)$ est une suite d’écart définissant une telle structure, le filtre des entourages est engendré par la famille dénombrable des ensembles $-1^{f_n}([0, 1/m])$, où $m$ et $n$ parcourent l’ensemble des entiers $> 0$.

#### Corollaire 2 {#top-ix-s2-thm-1-cor-2 .statement}

*Tout produit dénombrable d’espaces uniformes métrisables est métrisable.*

En effet, un tel espace est séparé, et sa structure uniforme admet un système fondamental dénombrable d’entourages (d’après II, p. 8, prop. 4).

### 5. Espaces topologiques métrisables

#### Définition 3 {#top-ix-s2-def-3 .statement}

*On dit qu’une distance sur un ensemble $X$ est compatible avec une topologie $\mathcal{T}$ sur $X$ si la topologie définie par cette distance est identique à $\mathcal{T}$. On dit qu’un espace topologique $X$ est métrisable s’il existe une distance sur $X$ compatible avec la topologie de $X$.

Deux distances sur un ensemble $X$, compatibles avec une même topologie $\mathcal{T}$, peuvent être non équivalentes.

Un exemple de ce fait est fourni par le sous-espace $\mathbf{R}_+^*$ de $\mathbf{R}$ formé des nombres réels $> 0$; la structure uniforme induite par la structure uniforme additive de $\mathbf{R}$, et la structure uniforme induite par la structure uniforme multiplicative de $\mathbf{R}^*$, sont toutes deux métrisables et compatibles avec la topologie de $\mathbf{R}_+^*$, mais elles ne sont pas comparables.

On remarquera aussi qu’il peut exister des structures uniformes non métrisables compatibles avec la topologie d’un espace topologique métrisable (IX, p. 91, exerc. 7).

Nous nous contenterons ici de donner des conditions nécessaires pour qu’un espace topologique soit métrisable (pour une condition nécessaire et suffisante, cf. IX, p. 109, exerc. 32). En premier lieu, un espace ne peut être métrisable que s’il est complètement régulier (nous verrons même (IX, p. 43, prop. 2) qu’un espace métrisable est nécessairement « normal », ce qui est une condition plus forte). D’autre part, d’après le th. 1 (IX, p. 15):

#### Proposition 6 {#top-ix-s2-prop-6 .statement}

Tout point d’un espace métrisable possède un système fondamental dénombrable de voisinages.

Plus généralement:

#### Proposition 7 {#top-ix-s2-prop-7 .statement}

Dans un espace métrisable, tout ensemble fermé est intersection d’une famille dénombrable d’ensembles ouverts; tout ensemble ouvert est réunion d’une famille dénombrable d’ensembles fermés.

En effet, soit $d$ une distance compatible avec la topologie d’un espace métrisable $X$. Si $A$ est fermé dans $X$, il est l’intersection des ensembles ouverts $V_{1/n}(A)$ (ensemble des $x$ tels que $d(x, A) < 1/n$; cf. IX, p. 13, prop. 2). La seconde partie de la proposition résulte de la première par passage aux complémentaires.

#### Remarque 1 {#top-ix-s2-n5-rem-1 .statement}

Les conditions nécessaires qui précèdent ne sont pas suffisantes (cf. IX, p. 92, exerc. 12).
2) On peut donner des exemples d’espaces où tout point a un système fondamental dénombrable de voisinages, mais où il existe des ensembles fermés qui ne sont pas des intersections dénombrables d’ensembles ouverts (IX, p. 94, exerc. 14); de tels espaces ne sont pas métrisables).

Le cor. 2 de IX, p. 15, montre qu’un produit dénombrable d’espaces topologiques métrisables est métrisable. En outre un espace $X$ somme (I, p. 15) d’une famille quelconque $(Y_i)_{i \in I}$ d’espaces métrisables est métrisable: en effet, si pour chaque $i \in I$, $d_i$ est une distance compatible avec la topologie de $Y_i$, on peut supposer que $d_i$ est bornée et que le diamètre de $Y_i$ est $\leq 1$; on définit alors une distance $d$ compatible avec la topologie de $X$ en prenant $d(x, y) = d_i(x, y)$ si $x, y$ appartiennent à un même ensemble $Y_i$, et $d(x, y) = 1$ dans le cas contraire.

### 6. Emploi des suites dénombrables

La prop. 6 est à l’origine du rôle qu’on peut faire jouer aux suites dénombrables de points dans un espace métrisable; dans beaucoup de questions, leur emploi peut se substituer à celui des filtres. Cela tient à ce que les filtres des voisinages des points de l’espace (et par suite les filtres convergents) sont déterminés par la donnée des suites convergentes de points de cet espace: en effet, comme le filtre des voisinages d’un point possède une base dénombrable, il est l’intersection des filtres élémentaires plus fins que lui (I, p. 43, prop. 11), c’est-à-dire des filtres élémentaires associés aux suites qui convergent vers le point considéré.

La notion de suite convergente est par contre tout à fait inadaptée à l’étude des espaces topologiques où il existe des points dont le filtre des voisinages n’admet pas de base dénombrable. On peut former en particulier des espaces topologiques séparés et non discrets dans lesquels, en chaque point x, l’intersection d’une famille dénombrable de voisinages de x est encore un voisinage de x (I, p. 100, exerc. 6); dans un tel espace, il n’y a pas d’autres suites convergentes que celles dont tous les termes sont égaux à partir d’une certain rang.

A titre d’exemple d’emploi des suites dénombrables, indiquons les propositions suivantes:

#### Proposition 8 {#top-ix-s2-prop-8 .statement}

Dans un espace métrisable E, pour qu’un point x soit adhérent à une partie non vide A de E, il faut et il suffit qu’il existe une suite de points de A qui converge vers x.

Nous savons déjà que la condition est suffisante (I, p. 47, prop. 6). Pour voir qu’elle est nécessaire, considérons un système fondamental dénombrable (V_n) de voisinages de x tel que V_{n+1} \subset V_n pour tout n. Si x est adhérent à A, chacun des ensembles V_n \cap A est non vide; si x_n est un point de V_n \cap A, la suite (x_n) converge vers x.\footnote{La proposition peut encore être exacte dans certains espaces où un point au moins n’admet pas de système fondamental dénombrable de voisinages: par exemple, l’espace obtenu en rendant compact, par adjonction d’un point à l’infini (I, p. 67, th. 4), un espace discret non dénombrable.}

La prop. 8 entraîne ceci:

#### Proposition 9 {#top-ix-s2-prop-9 .statement}

Pour qu’un espace métrique X soit complet, il faut et il suffit que toute suite de Cauchy dans X soit convergente.

En effet, soit $\hat{X}$ le complété de X; s’il existe un point $x \in \hat{X}$ n’appartenant pas à X, il existe une suite $(x_n)$ de points de X qui converge vers x; c’est une suite de Cauchy non convergente dans X.

#### Proposition 10 {#top-ix-s2-prop-10 .statement}

Soient X un espace métrisable, f une application de X dans un espace topologique Y. Pour que f soit continue en un point $a \in X$, il faut et il suffit que pour toute suite $(x_n)$ de points de X qui converge vers a, la suite $(f(x_n))$ converge vers $f(a)$ dans Y.

On sait déjà que la condition est nécessaire (I, p. 50, cor. 1). Pour voir qu’elle est suffisante, considérons le filtre $\mathcal{B}$ des voisinages de $f(a)$ dans Y; l’hypothèse entraîne que $f^{-1}(\mathfrak{B})$ est moins fin que tout filtre élémentaire associé à une suite qui converge vers $a$, c’est-à-dire tout filtre élémentaire convergent vers $a$; mais l’intersection de ces derniers est le filtre des voisinages de $a$ (I, p. 43, prop. 11), d’où la proposition.

On notera que les prop. 8 et 10 sont encore valables dans un espace $X$ où l’on suppose que tout point admet un système fondamental dénombrable de voisinages.

### 7. Fonctions semi-continues sur un espace métrisable

#### Proposition 11 {#top-ix-s2-prop-11 .statement}

Soient $X$ un espace métrisable, $f$ une fonction $\geqslant 0$, semi-continue inférieurement dans $X$. Alors $f$ est l’enveloppe supérieure d’une suite croissante de fonctions continues et finies dans $X$.

Soit d’une distance définissant la topologie de $X$. Supposons d’abord que $f = \varphi_A$, où $A$ est une partie ouverte de $X$. La fonction $h_n$ définie par
$$
h_n(x) = \inf(n . d(x, X - A), 1)
$$
est alors continue, finie et $\geqslant 0$ dans $X$; en outre, $h_n(x) = f(x)$ pour $x \in X - A$ et pour $d(x, X - A) > 1/n$. On a donc bien $f = \sup_n h_n$. Dans le cas général, il résulte de IV, p. 31, prop. 3 que $f$ est l’enveloppe supérieure d’une suite $(g_n)$ de fonctions dont chacune est combinaison linéaire de fonctions caractéristiques d’ensembles ouverts. En vertu de ce qu’on vient de voir, $g_n$ est l’enveloppe supérieure d’une suite croissante $(h_{mn})_{m \geqslant 0}$ de fonctions continues finies et $\geqslant 0$ (IV, p. 30); d’où il résulte que $f = \sup_{m, n} h_{mn}$ (E, III, p. 11). En posant $f_n = \sup_{p \leqslant n, q \leqslant n} h_{pq}$, on voit que $f$ est l’enveloppe supérieure de la suite croissante des fonctions $f_n$, qui sont finies, $\geqslant 0$ et continues (IV, p. 30).

### 8. Espaces métrisables de type dénombrable

#### Définition 4 {#top-ix-s2-def-4 .statement}

On dit qu’un espace métrisable est de type dénombrable si sa topologie admet une base dénombrable.

Il est clair que tout sous-espace d’un espace métrisable de type dénombrable est de type dénombrable. La définition de la base de la topologie d’un espace produit (I, p. 24), et le cor. 2 (IX, p. 15), prouvent que tout produit d’une famille dénombrable d’espace métrisables de type dénombrable est un espace métrisable de type dénombrable. De même, tout espace somme d’une famille dénombrable d’espaces métrisables de type dénombrable est un espace métrisable de type dénombrable (IX, p. 16).

#### Proposition 12 {#top-ix-s2-prop-12 .statement}

Pour un espace topologique métrisable $X$, les propositions suivantes sont équivalentes :
a) $X$ est de type dénombrable ;

b) il existe un ensemble dénombrable dense dans $X$;
c) $X$ est homéomorphe à un sous-espace du cube $I^\mathbf{N}$, où $I$ est l’intervalle $(0, 1)$ dans $\mathbf{R}$.

D’après les remarques précédentes, il est clair que c) implique a); a) implique b), car si $(U_n)$ est une base dénombrable de la topologie de $X$ et $a_n$ un point de $U_n$, l’ensemble des $a_n$ est partout dense dans $X$. Montrons enfin que b) entraîne c). Soit $(a_n)$ une suite partout dense de points de $X$, et pour tout $x \in X$, soit $\varphi(x)$ le point $(d(x, a_n))_{n \in \mathbf{N}}$ de $I^\mathbf{N}$ ($d$ étant une distance compatible avec la topologie de $X$ et pour laquelle le diamètre de $X$ est $\leqslant 1$); nous allons voir que $\varphi$ est un homéomorphisme de $X$ sur un sous-espace de $I^\mathbf{N}$. En effet, $\varphi$ est continue puisque chacune des fonctions $x \mapsto d(x, a_n)$ l’est; en outre $\varphi$ est injective, car tout point de $X$ est limite d’une suite extraite de $(a_n)$ (IX, p. 17, prop. 8). Soit $B$ une boule de centre $x_0$ et de rayon $r$ dans $X$, et soit $n$ un entier tel que $d(x_0, a_n) < r/3$. L’image par $\varphi$ de l’ensemble $W$ des points $x \in X$ tels que

$$
|d(x_0, a_n) - d(x, a_n)| < r/3
$$

est par définition un voisinage de $\varphi(x_0)$ dans $\varphi(X)$. Mais pour tout $x \in W$, on a $d(x, a_n) < d(x_0, a_n) + r/3 < 2r/3$, d’où

$$
d(x, x_0) \leqslant d(x_0, a_n) + d(x, a_n) < r,
$$

ce qui montre que $W$ est un voisinage de $x_0$ contenu dans $B$; donc $\varphi$ est un homéomorphisme de $X$ sur $\varphi(X)$.

On notera que pour un espace topologique quelconque $X$, la propriété b) n’entraîne pas nécessairement l’existence d’une base dénombrable, même lorsque $X$ est compact et que tout point de $X$ admet un système fondamental dénombrable de voisinages (IX, p. 92, exerc. 12; cf. I, p. 90, exerc. 7).

#### Corollaire {#top-ix-s2-n8-cor-1 .statement}

(i) Tout sous-espace d’un espace métrisable de type dénombrable est métrisable de type dénombrable.
(ii) Toute somme (resp. tout produit) d’une famille dénombrable d’espaces métrisables de type dénombrable est métrisable de type dénombrable.

L’assertion (i) résulte de la définition; pour prouver l’assertion (ii) relative aux sommes, notons que toute somme d’espaces métrisables est métrisable (IX, p. 16); d’autre part, si $X$ est somme d’une suite $(X_n)$ d’espaces topologiques et si $D_n$ est une partie partout dense de $X_n$, $\bigcup_n D_n$ est dense dans $X$. Enfin, l’assertion (ii) relative aux produits résulte de la prop. 12 et de la relation $(I^\mathbf{N})^\mathbf{N} = I^{\mathbf{N} \times \mathbf{N}}$, et du fait que $\mathbf{N} \times \mathbf{N}$ est dénombrable.

#### Proposition 13 {#top-ix-s2-prop-13 .statement}

Soit $X$ un espace topologique admettant une base dénombrable $(U_n)$; pour tout recouvrement ouvert $(V_i)_{i \in I}$ de $X$ il existe une partie dénombrable $J$ de $I$ telle que $(V_i)_{i \in J}$ soit un recouvrement de $X$.

En effet, soit $H$ la partie de $\mathbf{N}$ formée des indices $n$ tels que $U_n$ soit contenu dans un au moins des $V_i$; la suite $(U_n)_{n \in H}$ est un recouvrement de $X$, car tout point $x \in X$ appartient à un $V_i$, et comme $V_i$ est ouvert, il existe un indice $n$ tel que $x \in U_n \subset V_i$. Cela étant, il existe une application $\psi$ de $H$ dans $I$ telle que $U_n \subset V_{\psi(n)}$ pour tout $n \in H$; en prenant $J = \psi(H)$, qui est dénombrable, on répond à la question.

### 9. Espaces métriques compacts; espaces métrisables compacts

Le critère de précompacité des espaces uniformes (II, p. 29, th. 4) donne, pour les espaces métriques, la proposition suivante:

#### Proposition 14 {#top-ix-s2-prop-14 .statement}

*Pour qu’un espace métrique $X$ soit précompact, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un recouvrement fini de $X$ dont tous les ensembles aient un diamètre $\leq \varepsilon$.*

Si on ajoute l’hypothèse que $X$ est *complet*, on obtient un critère de *compacité* des espaces métriques.

On déduit de la prop. 14 un critère *topologique* de compacité, applicable aux espaces métrisables:

#### Proposition 15 {#top-ix-s2-prop-15 .statement}

*Pour qu’un espace topologique métrisable $X$ soit compact, il faut et il suffit que toute suite infinie de points de $X$ ait une valeur d’adhérence dans $X$.*

D’après l’axiome (C) (I, p. 59), la condition est *nécessaire*. Pour voir qu’elle est *suffisante*, considérons une distance $d$ compatible avec la topologie de $X$. Montrons d’abord que l’espace métrique $X$ ainsi défini est *complet*: en effet, toute suite de Cauchy dans $X$ a alors une valeur d’adhérence, et par suite est convergente (II, p. 14, cor. 2 de la prop. 5); la prop. 9, IX, p. 17 montre donc que $X$ est complet. En second lieu, montrons que $X$ est *précompact*; dans le cas contraire, en vertu de la prop. 14, il existerait un nombre $\alpha > 0$ tel qu’il n’y ait aucun recouvrement fini de $X$ par des parties de $X$ de diamètre $< \alpha$. On pourrait alors définir par récurrence sur $n$ une suite infinie $(x_n)$ de points de $X$ par la condition $d(x_p, x_n) > \alpha/2$ pour tout $p < n$; or, une telle suite ne peut avoir de valeur d’adhérence, puisque toute boule de rayon $< \alpha/4$ contient au plus un point de la suite.

#### Corollaire {#top-ix-s2-n9-cor-1 .statement}

*Pour qu’une partie $A$ d’un espace topologique métrisable $X$ soit relativement compacte, il faut et il suffit que toute suite infinie de points de $A$ ait une valeur d’adhérence dans $X$.*

La condition est nécessaire d’après I, p. 62, prop. 7. Inversement, soit $d$ une distance compatible avec la topologie de $X$. Montrons que l’espace $\overline{A}$ est compact, en appliquant le critère de la prop. 15: soit $(x_n)$ une suite de points de $\overline{A}$; pour chaque indice $n$, il existe $y_n \in A$ tel que $d(x_n, y_n) < 1/n$; la suite $(y_n)$ admet par hypothèse une valeur d’adhérence $a \in X$, et $a$ est aussi valeur d’adhérence de la suite $(x_n)$, car si $y_m$ appartient à la boule de centre $a$ et de rayon $1/n$ pour un $m > n$, $x_m$ appartient à la boule de centre $a$ et de rayon $2/n$.

Il faut remarquer que la prop. 15 n’est pas une conséquence de l’existence, en tout point de X, d’un système fondamental dénombrable de voisinages; on peut donner des exemples d’espaces non métrisables et non compacts, dans lesquels tout point possède un système fondamental dénombrable de voisinages, et toute suite de points une valeur d’adhérence (IX, p. 94, exerc. 14).

#### Proposition 16 {#top-ix-s2-prop-16 .statement}

Pour qu’un espace compact X soit métrisable, il faut et il suffit que sa topologie admette une base dénombrable.

La condition est nécessaire. En effet, d’après la prop. 14 (IX, p. 20), pour tout entier $n \geqslant 1$, il existe une partie finie $A_n$ de X telle que la distance à $A_n$ de tout point de X soit $\leqslant 1/n$; l’ensemble dénombrable $A = \bigcup_n A_n$ est par suite dense dans X, d’où notre assertion (IX, p. 18, prop. 12).

La condition est suffisante. Soit en effet $(U_n)$ une base dénombrable de la topologie de X. Tout voisinage d’un point de la diagonale $\Delta$ de $X \times X$ contient alors un voisinage de la forme $U_n \times U_n$; il résulte de l’axiome de Borel-Lebesgue appliqué à l’ensemble compact $\Delta$ dans $X \times X$, que tout voisinage de $\Delta$ contient une réunion finie d’ensembles de la forme $U_n \times U_n$, qui est un voisinage de $\Delta$. Les voisinages de $\Delta$ qui sont réunions finies d’ensembles de la forme $U_n \times U_n$ forment par suite un système fondamental d’entourages de la structure uniforme de X (II, p. 27, th. 1); notre assertion résulte par suite du th. 1 (IX, p. 5).

#### Corollaire {#top-ix-s2-n9-cor-2 .statement}

Soient X un espace localement compact, $X'$ l’espace compact obtenu par adjonction à X d’un point à l’infini $\omega$ (I, p. 68). Les propositions suivantes sont équivalentes:

a) la topologie de X admet une base dénombrable;
b) $X'$ est métrisable;
c) X est métrisable et dénombrable à l’infini.

Montrons d’abord que a) entraîne b). Soit $(U_n)$ une base dénombrable de la topologie de X; tout voisinage d’un point x de X contient un voisinage compact de x, lequel contient à son tour un voisinage de x égal à l’un des $U_n$; ceux des $U_n$ qui sont relativement compacts forment donc aussi une base de la topologie de X, et on peut donc supposer tous les $U_n$ relativement compacts. L’espace X est donc réunion dénombrable des ensembles compacts $\overline{U}_n$, autrement dit est dénombrable à l’infini; cela entraîne que, dans $X'$, le point $\omega$ admet un système fondamental dénombrable $(V_n)$ de voisinages ouverts (I, p. 69, corollaire); il est clair alors que tout voisinage d’un point $y \in X'$ contient, soit l’un des $U_n$, soit l’un des $V_n$, qui est un voisinage de y; autrement dit les $U_n$ et les $V_n$ forment une base dénombrable de la topologie de E’, et notre assertion résulte de la prop. 16.

Il est immédiat que b) entraîne c), car b) implique que $\omega$ admet un système fondamental dénombrable de voisinages (I, p. 69, corollaire).

Prouvons enfin que c) entraîne a). Il existe par hypothèse une suite croissante $(V_n)$ d’ensembles ouverts relativement compacts, formant un recouvrement ouvert de X et tels que $V_n \subset V_{n+1}$ (I, p. 68, prop. 15). Le sous-espace $V_n$ étant compact et métrisable, admet une base dénombrable (IX, p. 21, prop. 16), et il en est donc de même de $V_n$; soit $(U_{mn})_{m \geq 1}$ une base de la topologie de $V_n$. Pour $x \in E$ et tout voisinage $W$ de $x$, il existe $n$ tel que $x \in V_n$, donc il existe $m$ tel que $x \in U_{mn} \subset V_n \cap W$; les ensembles $U_{mn}$ ($m \geq 1, n \geq 1$) forment par suite une base de la topologie de $X$.

### 10. Espaces quotients des espaces métrisables

Si $X$ est un espace métrisable, $R$ une relation d’équivalence dans $X$, l’espace quotient $X/R$ n’est pas nécessairement métrisable (même si en outre $X$ est localement compact *et $X/R$ normal*). Toutefois:

#### Proposition 17 {#top-ix-s2-prop-17 .statement}

*Tout espace quotient séparé d’un espace compact métrisable est un espace compact métrisable.*

Il revient au même de dire que si $f$ est une application continue d’un espace compact métrisable $X$ dans un espace séparé $Y$, $f(X)$ *est un sous-espace métrisable* de $Y$ (I, p. 63, cor. 3).

Soient $X$ un espace compact métrisable, $R$ une relation d’équivalence dans $X$ telle que $X/R$ soit séparé. On sait alors (I, p. 62, th. 2) que $X/R$ est compact; d’après la prop. 16 (IX, p. 21), tout revient à prouver que la topologie de $X/R$ admet une base dénombrable. Nous utiliserons pour cela le fait que $R$ est *fermée* (I, p. 63, cor. 2) et que les classes mod. $R$ sont compactes. Soit $\varphi$ l’application canonique de $X$ sur $X/R$, et soit $(U_n)$ une base dénombrable de la topologie de $X$.

Soient $z$ un point quelconque de $X/R$, $V$ un voisinage de $z$ dans $X/R$; $\varphi^{-1}(V)$ est donc un voisinage dans $X$ de l’ensemble compact $\varphi^{-1}(z)$. Comme pour tout $x \in \varphi^{-1}(z)$ il existe un $U_n$ contenant $x$ et contenu dans $\varphi^{-1}(V)$, l’axiome de Borel-Lebesgue montre qu’il existe un recouvrement ouvert fini $(U_{n_k})_{1 \leq k \leq r}$ de $\varphi^{-1}(z)$ tel que, si on pose $W = \bigcup_k U_{n_k}$, $W$ soit un voisinage de $\varphi^{-1}(z)$ contenu dans $\varphi^{-1}(V)$. Comme $R$ est fermée, $\varphi(W)$ est alors un voisinage de $z$ dans $X/R$, contenu dans $V$ (I, p. 35, *Remarque*). Désignons par $\mathfrak{B}$ l’ensemble des intérieurs des ensembles de la forme $\varphi(W)$, où $W$ parcourt l’ensemble $\mathfrak{F}$ des réunions finies d’ensembles de la forme $U_n$; ce qui précède prouve que $\mathfrak{B}$ est une base de la topologie de $X/R$, et comme $\mathfrak{F}$ est dénombrable, il en est de même de $\mathfrak{B}$.

#### Proposition 18 {#top-ix-s2-prop-18 .statement}

*Soient $X$ un espace métrique complet, $R$ une relation d’équivalence ouverte dans $X$, telle que $X/R$ soit séparé, $\varphi$ l’application canonique de $X$ sur $X/R$. Pour toute partie compacte $K$ de $X/R$, il existe une partie compacte $K'$ de $X$ telle que $\varphi(K') = K$.*

Soit $\mathfrak{B}_1$ l’ensemble des boules ouvertes de rayon $1/2$ dans $X$. Lorsque $B$ parcourt $\mathfrak{B}_1$, les ensembles $\varphi(B)$ forment un recouvrement ouvert de $K$, donc il existe un nombre fini de points $x_1, \ldots, x_m$ de $X$ tels que les images par $\varphi$ des boules ouvertes de rayon $1/2$ et de centre $x_i (1 \leq i \leq m)$ forment un recouvrement ouvert de K. Posons $H_1 = \{x_1, \ldots, x_m\}$, et supposons défini, pour $1 < i \leq n$, un ensemble fini $H_i$ tel que:

$1^\circ$ $H_i \subset H_{i+1}$ et tout point de $H_{i+1}$ est à une distance $< 1/2^i$ de $H_i$ pour $1 \leq i \leq n - 1$;
$2^\circ$ les images par $\varphi$ des boules ouvertes de rayon $1/2^i$, dont le centre parcourt $H_i$, forment un recouvrement ouvert de K, pour $1 \leq i \leq n$.

Soit alors $\mathfrak{B}_{n+1}$ l’ensemble des boules ouvertes de rayon $1/2^{n+1}$, dont le centre $x$ est tel que $d(x, H_n) < 1/2^n$; d’après les propriétés de $H_n$, les ensembles $\varphi(B)$, où B parcourt $\mathfrak{B}_{n+1}$, forment un recouvrement ouvert de K; donc il existe un ensemble fini $L_{n+1} \subset X$, tel que les images par $\varphi$ des boules ouvertes de rayon $1/2^{n+1}$, dont le centre parcourt $L_{n+1}$, forment un recouvrement ouvert de K; en prenant $H_{n+1} = H_n \cup L_{n+1}$, on voit qu’on peut définir par récurrence une suite infinie $(H_n)$ de parties de X ayant les propriétés $1^\circ$ et $2^\circ$ ci-dessus. Posons $H = \bigcup_n H_n$ et montrons que H est *précompact*: pour tout $p > 0$ et tout point $z_{n+p} \in H_{n+p}$, il existe une suite de points $z_{n+i} \in H_{n+i} (0 \leq i \leq p-1)$ tels que
$$
d(z_{n+i}, z_{n+i+1}) < 1/2^{n+i} \quad \text{pour} \quad 0 \leq i \leq p-1;
$$
on en conclut que $d(z_n, z_{n+p}) \leq \sum_{i=0}^{p-1} 1/2^{n+i} \leq 1/2^{n-1}$, et par suite
$$
d(y, H_n) \leq 1/2^{n-1}
$$
pour tout $y \in H$, ce qui prouve notre assertion. Comme X est complet, $H$ est compact, et par suite $\varphi(H)$ est compact. Montrons que $K \subset \varphi(H)$: si $z \in K$, on a par définition $d(H_n, \varphi^{-1}(z)) \leq 1/2^n$ pour tout $n$, d’où $d(H, \varphi^{-1}(z)) = 0$; comme $\varphi^{-1}(z)$ est fermé et $H$ compact, cela entraîne $H \cap \varphi^{-1}(z) \neq \varnothing$ (IX, p. 14, *Remarque*), d’où notre assertion. Si alors $K' = H \cap \varphi^{-1}(K)$, $K'$ est fermé dans $H$, donc compact, et on a $\varphi(K') = K$.

## EXERCICES {#top-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
