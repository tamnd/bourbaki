---
book: top
book_title: General Topology
chapter: V
chapter_title: GROUPES À UN PARAMÈTRE
section: 2
section_title: Mesure des grandeurs
lang: fr
source: top-v-x-fr
book_pages: TG V.5-TG V.9, TG V.16
pdf_pages: 0012-0016, 0023-0023
extraction: ocr
statements: 5
exercises: 2
content_sha256: bd7e65967af93f4f719b250f95e6f706ae85d916ffa49b125b4ce3f1fbc0df61
---

## § 2. MESURE DES GRANDEURS

On a vu (cf. Note historique du chap. IV) que le problème de la mesure des grandeurs est à l’origine de la notion de nombre réel; plus précisément, les diverses espèces de grandeurs dont l’étude s’imposa peu à peu, pour des raisons pratiques ou théoriques, furent d’abord considérées séparément; et la possibilité de les mesurer toutes par un même système de nombres apparut comme une constatation expérimentale bien avant que les mathématiciens grecs n’eussent conçu l’idée hardie d’en faire l’objet d’une démonstration rigoureuse. Dans la théorie axiomatique établie par ces derniers, l’idée de grandeur apparaît liée à une loi de composition (l’« addition » des grandeurs de même espèce) et à une relation d’ordre (la relation « A est plus petit que B », dite relation de comparaison des grandeurs). Nous allons, dans ce qui suit, examiner le même problème, c’est-à-dire rechercher les conditions auxquelles doivent satisfaire une loi de composition interne et une relation d’ordre sur un ensemble E pour que celui-ci soit isomorphe à une partie E’ de $\mathbf{R}$, munie de la structure induite par l’addition et la relation $\leqslant$ dans $\mathbf{R}$. Comme nous ne supposerons pas a priori que la loi de composition donnée sur E soit commutative, nous la noterons multiplicativement; à cela près, nous ne nous écarterons guère des raisonnements classiques sur la mesure des grandeurs.

Soit E un ensemble totalement ordonné par une relation d’ordre notée $x \leqslant y$, et possédant un plus petit élément $\omega$. Soit I une partie de E telle que $\omega \in I$, et que les relations $x \in I, y \leqslant x$ entraînent $y \in I$; supposons donnée dans E une loi de composition non partout définie $(x, y) \mapsto xy$, le composé $xy$ étant défini pour tout couple d’éléments de I ($xy$ appartient à E, mais non nécessairement à I; cf. A, I, p. 1). Faisons en outre les hypothèses suivantes:

(GR_I) $\omega$ est élément neutre ($\omega x = x \omega = x$ pour tout $x \in I$) et la loi de composition est associative (au sens suivant: chaque fois que $x \in I, y \in I, z \in I, xy \in I$ et $yz \in I$, on a $x(yz) = (xy)z$).

(GR_{II}) La relation $x < y$ entre éléments de I entraîne, pour tout $z \in I$, les relations $xz < yz$ et $zx < zy$.

(GR_{III}) L’ensemble des éléments > ω de I n’est pas vide et n’a pas de plus petit élément, et, quels que soient les éléments x, y de I tels que x < y, il existe z > ω tel que xz ≤ y.

La condition (GR_{II}) entraîne qu’on peut multiplier membre à membre les inégalités entre éléments de I : x < y et x' < y' entraînent xx' < yy' (car xx' < yx' et yx' < yy'). En particulier on a y < yx pour tout x > ω (x ∈ I, y ∈ I).

Étant donnée une suite finie (x_i)_{1 ≤ i ≤ p} d’éléments de I, on peut définir par récurrence sur p le composé $\prod_{i=1}^{p} x_i$ de cette suite comme égal à $\left( \prod_{i=1}^{p-1} x_i \right) x_p$, pourvu que le composé $\prod_{i=1}^{p-1} x_i$ soit défini et appartienne à I ; si $\prod_{i=1}^{p} x_i$ est défini, chacun des composés $\prod_{i=1}^{q} x_i$ est donc défini et appartient à I pour $2 ≤ q ≤ p - 1$. Lorsqu’on prend tous les x_i égaux à un même élément x ∈ I, on voit en particulier que si x^p est défini, x^q est défini et appartient à I pour $2 ≤ q ≤ p - 1$; par convention, on pose $x^0 = ω$ pour tout x ∈ I. D’après (GR_{II}), si x > ω, on a $ω < x^q < x^p$ pour $1 ≤ q ≤ p - 1$ si x^p est défini ; si x < y et si y^p est défini, on voit, par récurrence sur p, que x^p est défini et que $x^p < y^p$. D’autre part, la condition d’associativité (GR_I) entraîne, par récurrence sur n, que, si $x^{m+n}$ est défini, il en est de même de $x^m x^n$, et que $x^{m+n} = x^m x^n$. Inversement, en vertu de (GR_I) et (GR_{II}), si $x^m x^n$ est défini et appartient à I, $x^{m+n}$ est défini et $x^{m+n} = x^m x^n$ : on le voit encore par récurrence sur n, car on a $x^{n-1} ≤ x^n$, donc $x^m x^{n-1}$ est défini et appartient à I ; par hypothèse $x^m x^{n-1} = x^{m+n-1} ∈ I$, donc $(x^{m+n-1})x = x^{m+n}$ est défini et égal à $x^m x^n$ d’après le résultat précédent. De même, on voit par récurrence sur n que, si $x^{mn}$ est défini, $(x^m)^n$ est défini et $x^{mn} = (x^m)^n$ ; inversement, si $(x^m)^n$ est défini et appartient à I, $x^{mn}$ est défini et égal à $(x^m)^n$.

Enfin, l’axiome (GR_{III}) entraîne que, pour tout x ∈ I tel que x > ω, il existe y > ω tel que $y^2 ≤ x$. En effet, si x > ω, il existe z > ω tel que z < x, puis t > ω tel que zt ≤ x ; on prendra pour y le plus petit des éléments z, t. Par récurrence sur n, on en déduit qu’il existe u > ω tel que $u^{2^n} ≤ x$.

Introduisons maintenant l’hypothèse suivante :

(GR_{IV}) (« Axiome d’Archimède ») Quels que soient x ∈ I, y ∈ I, tels que x > ω, il existe un entier n > 0 tel que $x^n$ soit défini et que $x^n > y$.

Si on prend pour E un ensemble de nombres réels ≥ 0, contenant 0 et des nombres > 0 arbitrairement petits, pour I l’intersection de E et d’un intervalle de $\mathbf{R}$ d’origine 0 et non réduit à un point, pour loi de composition l’addition de deux nombres de I, et si on suppose que x + y ∈ E pour x ∈ I, y ∈ I, il est clair que les axiomes (GR_I), (GR_{II}), (GR_{III}) et (GR_{IV}) sont vérifiés.¹ Réciproquement :

¹ Dans les ensembles de « grandeurs » qui interviennent dans les sciences expérimentales, les axiomes (GR_I) et (GR_{II}) sont en général susceptibles de vérification expérimentale, au moins avec

#### Proposition 1 {#top-v-s2-prop-1 .statement}

Soit E un ensemble totalement ordonné, possédant un plus petit élément ω ; soit I une partie de E, telle que ω ∈ I, et que les relations x ∈ I, y ≤ x entraînent y ∈ I ; soit (x, y) ↦ xy une application de I × I dans E. Alors, si les axiomes (GR_I), (GR_{II}), (GR_{III}) et (GR_{IV}) sont satisfaits, il existe une application f strictement croissante de I dans l’ensemble R_+ des nombres réels ≥ 0, telle que l’on ait

$$
f(xy) = f(x) + f(y)
$$

chaque fois que x ∈ I, y ∈ I et xy ∈ I ; en outre, pour tout b ∈ I, l’intersection de f(I) et de l’intervalle [0, f(b)] de R est dense dans cet intervalle.

Étant donnés deux éléments quelconques x, y de I tels que y ≠ ω, notons (x : y) le plus grand des entiers n ≥ 0 tels que y^n soit défini et ≤ x¹ ; cet entier existe d’après (GR_{IV}) ; si (x : y) = p, y^{p+1} est défini et > x. Si x ∈ I, y ∈ I et xy ∈ I, on a

(1)

$$(x : z) + (y : z) \leq (xy : z) \leq (x : z) + (y : z) + 1.$$

En effet, soit (x : z) = p, (y : z) = q ; on a z^p ≤ x, z^q ≤ y ; comme xy ∈ I, z^p z^q est défini et appartient à I, donc z^{p+q} est défini et on a z^{p+q} = z^p z^q ≤ xy ; en outre, si z^{p+q+2} est défini, on a z^{p+q+2} > xy, puisque z^{p+1} > x et z^{p+1} > y.

Démontrons maintenant les inégalités

(2)

$$\begin{cases}
(x:y)(y:z) \leq (x:z) \\
((x:y) + 1)((y:z) + 1) \geq (x:z) + 1.
\end{cases}$$

Soit (x:y) = p et (y:z) = q ; on a y^p ≤ x et z^q ≤ y, donc (z^q)^p est défini et ≤ x ; il appartient donc à I et par suite z^{pq} est défini et on a z^{pq} = (z^q)^p ≤ x ; d’où la première inégalité. D’autre part, si z^{(p+1)(q+1)} est défini on a z^{(p+1)(q+1)} > x, puisque y^{p+1} > x et z^{q+1} > y ; d’où la seconde inégalité.

Désignons par 𝔅 le filtre des sections de l’ensemble ordonné des éléments > ω de I, filtrant pour la relation ≥ ; une base de 𝔅 est formée des intervalles ]ω, z], où z parcourt l’ensemble des éléments > ω. Étant donnés deux éléments a et x de I tels que a > ω, nous allons voir que le rapport (x : z)/(a : z), qui est défini pour z ≤ a et est un nombre rationnel > 0, est une fonction de z qui a une limite suivant 𝔅. C’est évident si x = ω, car alors (x : z) = 0 quel que soit z. Si x > ω, nous allons montrer que l’image 𝔅 de 𝔅 par l’application

$$z \mapsto (x : z)/(a : z)$$

(restreinte à l’ensemble des z > ω qui sont ≤ x et ≤ a) est une base de filtre de Cauchy pour la structure uniforme du groupe multiplicatif $\mathbf{R}_+^*$, et converge par

une certaine approximation. Par contre l’axiome (GR_{III}), qui postule l’existence de grandeurs « aussi petites qu’on veut », ne peut évidemment être fondé de la même manière ; il constitue une pure exigence a priori. Quant à l’axiome (GR_{IV}), il peut être considéré comme une « extrapolation » d’un fait vérifiable expérimentalement pour des grandeurs qui ne sont pas « trop petites ».

¹ Lorsque E = I est l’ensemble des entiers naturels, la loi de composition étant l’addition, (x : y) n’est autre que la partie entière de x/y, ou, comme on dit encore, le « quotient approché par défaut à une unité près » de x par y.

suite vers un nombre réel > 0. En effet, remarquons d’abord que, u > ω étant donné, (u:z) a pour limite +∞ suivant 𝔅; car il existe z > ω tel que z^{2^n} ≤ u, d’où (u:z) ≥ 2^n > n. Donnons-nous alors un nombre ε > 0 arbitraire; il existe t > ω tel que (x:t) ≥ 1/ε et (a:t) ≥ 1/ε; écrivons la double inégalité

$$
\frac{(x:t)}{(a:t) + 1} \cdot \frac{(t:z)}{(t:z) + 1} \leq \frac{(x:z)}{(a:z)} \leq \frac{(x:t) + 1}{(a:t)} \cdot \frac{(t:z) + 1}{(t:z)},
$$

qui résulte immédiatement des inégalités (2). Il existe z_0 > ω tel que z ≤ z_0 entraîne (t:z) ≥ 1/ε, donc

$$
\frac{1}{(1 + \varepsilon)^2} \frac{(x:t)}{(a:t)} \leq \frac{(x:z)}{(a:z)} \leq (1 + \varepsilon)^2 \frac{(x:t)}{(a:t)},
$$

ce qui prouve que 𝔅 est une base de filtre de Cauchy pour la structure uniforme multiplicative

Fixons désormais l’élément a > ω (« unité de mesure »), et posons, pour tout x ∈ I,

$$
f(x) = \lim_{\mathfrak{F}} \frac{(x:z)}{(a:z)}.
$$

D’après ce qui précède, on a f(ω) = 0, f(x) > 0 pour x > ω, et f(a) = 1. Si on divise les trois membres de (1) par (a:z), et qu’on passe à la limite suivant 𝔅, on voit que f(xy) = f(x) + f(y) pour x ∈ I, y ∈ I. De même, la relation x ≤ y entraîne (x:z) ≤ (y:z), d’où, en divisant par (a:z) et passant à la limite, f(x) ≤ f(y); f est croissante dans I. On en déduit que f est strictement croissante dans I; en effet, si x < y, il existe z > ω tel que xz ≤ y, d’où f(xz) ≤ f(y), et comme xz ∈ I, f(x) + f(z) = f(xz) ≤ f(y); comme f(z) > 0, il s’ensuit bien que f(x) < f(y).

Enfin, si b ∈ I, l’intersection de f(I) et de l’intervalle [0, f(b)] de ℝ est dense dans cet intervalle; pour tout entier n > 0, il existe en effet x > ω tel que f(x) ≤ 2^{-n}: il suffit de prendre x tel que x^{2^n} ≤ a; si p est le plus petit entier tel que x^{p+1} > b, on a (p + 1)f(x) > f(b) et qf(x) ≤ f(b) pour 1 ≤ q ≤ p; donc tout intervalle contenu dans [0, f(b)] et de longueur > 2^{-n} contient au moins un point de la forme qx = f(x^q) ∈ f(I). La proposition 1 est par suite entièrement démontrée.

#### Remarque 1 {#top-v-s2-rem-1 .statement}

Les relations x ∈ I, y ∈ I, xy ∈ I, yx ∈ I entraînent

$$
f(xy) = f(x) + f(y) = f(yx),
$$

donc yx = xy, puisque f est strictement croissante; autrement dit, la loi induite par la loi de composition de E sur un intervalle (ω, b) convenable (b étant pris par exemple tel que b^2 ≤ a) est commutative.

#### Remarque 2 {#top-v-s2-rem-2 .statement}

Toute application g de I dans ℝ_+, satisfaisant aux mêmes conditions que f, est de la forme x ↦ λf(x) où λ > 0. En effet, soit λ = g(a) > 0; les relations z^p ≤ x ≤ z^{p+1}, z^q ≤ a ≤ z^{q+1} entraînent, par hypothèse,

$$
p g(z) \leq g(x) \leq (p + 1)g(z), \quad q g(z) \leq g(a) \leq (q + 1)g(z),
$$
d’où
$$
\lambda \frac{(x:z)}{(a:z) + 1} \leq g(x) \leq \lambda \frac{(x:z) + 1}{(a:z)},
$$
et, en passant à la limite suivant $\mathcal{F}$, on a $g(x) = \lambda f(x)$.

Cherchons à quelles conditions $f(I)$ est un intervalle de $\mathbf{R}_+$. On a évidemment deux conditions nécessaires:

**(GR_{IIIa})** *L’ensemble des éléments > $\omega$ de I n’est pas vide et n’a pas de plus petit élément, et, quels que soient les éléments x, y de I tels que x < y, il existe z $\in$ I tel que xz = y* (« soustraction » des grandeurs).

**(GR_{IVa})** *Toute suite croissante d’éléments de I, majorée par un élément de I, admet une borne supérieure dans I*.

Nous allons montrer que ces conditions sont suffisantes, et qu’en outre elles dispensent de postuler l’axiome (GR_{IV}) (axiome d’Archimède). D’une façon précise, nous allons démontrer la proposition suivante:

#### Proposition 2 {#top-v-s2-prop-2 .statement}

*Si un ensemble totalement ordonné E et une partie I satisfont aux axiomes (GR_I), (GR_{II}), (GR_{IIIa}) et (GR_{IVa}), il existe une application strictement croissante f de I sur un intervalle de $\mathbf{R}$ d’origine 0, telle que l’on ait $f(\omega) = 0$ et $f(xy) = f(x) + f(y)$ chaque fois que x, y et xy appartiennent à I*.

Montrons d’abord que l’axiome (GR_{IV}) est vérifié. Raisonnons par l’absurde: soient $x \in I, y \in I$ tels qu’on ait $x > \omega$ et $x^n \leq y$ pour tout entier $n > 0$ tel que $x^n$ soit défini. On voit, par récurrence sur $n$, que $x^n$ est défini et appartient à I pour tout $n > 0$: en effet, si $x^n$ est défini, c’est un élément de I puisque $x^n \leq y$, donc $x^{n+1}$ est défini. Alors la suite croissante $(x^n)$ possède une borne supérieure $b \in I$ d’après (GR_{IVa}). Puisque $x < b$, il existe $c \in I$ tel que $xc = b$, d’après (GR_{IIIa}), et on a $c < b$ puisque $x > \omega$. Or, pour tout $n$, on a $x^{n+1} \leq b = xc$, d’où $x^n \leq c$ d’après (GR_{II}); la borne supérieure $b$ des $x^n$ est donc $\leq c$, ce qui est contradictoire.

Les conditions d’application de la prop. 1 (V, p. 7) sont donc remplies. Reste à montrer que, si $\gamma = f(c)$ ($c > \omega$) est un élément quelconque de $f(I)$, et $\beta$ un nombre réel tel que $0 < \beta < \gamma$, il existe $b \in I$ tel que $f(b) = \beta$ (IV, p. 7, prop. 1). Comme l’intersection de $f(I)$ et de $[0, \gamma]$ est dense dans cet intervalle, il existe une suite croissante $(x_n)$ d’éléments de I telle que $f(x_n)$ ait pour limite $\beta$. Soit $b$ la borne supérieure de la suite $(x_n)$ dans I; on a $f(b) \geq f(x_n)$ quel que soit $n$, donc $f(b) \geq \beta$; mais $f(b) > \beta$ est impossible, sinon il existerait $y \in I$ tel que $\beta < f(y) < f(b)$, et comme $\beta$ est la borne supérieure de la suite $(f(x_n))$, on aurait $f(x_n) < f(y) < f(b)$ quel que soit $n$, d’où $x_n < y < b$ quel que soit $n$, ce qui est absurde. Donc $f(b) = \beta$.

La proposition 2 est ainsi démontrée.

#### Remarque {#top-v-s2-n0-rem-3 .statement}

Lorsque $I = E$, l’image $f(I) = f(E)$ est $\mathbf{R}_+$ tout entier, car pour un $b > \omega$, $b^n$ est défini pour tout $n$, donc $n.f(b)$ appartient à $f(E)$ quel que soit $n$, ce qui entraîne que $f(E)$ n’est pas borné, puisque $f(b) > 0$.

## EXERCICES {#top-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
