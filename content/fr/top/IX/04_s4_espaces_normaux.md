---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 4
section_title: Espaces normaux
lang: fr
source: top-v-x-fr
book_pages: TG IX.41-TG IX.52, TG IX.101-TG IX.111
pdf_pages: 0161-0172, 0221-0231
extraction: ocr
subsections:
    - "no": 1
      title: Définition des espaces normaux
      page: 41
      pdf_page: 161
    - "no": 2
      title: Prolongement d’une fonction numérique continue
      page: 44
      pdf_page: 164
    - "no": 3
      title: Recouvrements ouverts localement finis d’un ensemble fermé et partitions continues de l’unité dans un espace normal
      page: 46
      pdf_page: 166
    - "no": 4
      title: Normalité des espaces paracompacts
      page: 49
      pdf_page: 169
    - "no": 5
      title: Paracompacité des espaces métrisables
      page: 51
      pdf_page: 171
statements: 25
exercises: 36
content_sha256: 4aac5a26df47505d14ddc0cffc9d8b8e878874159eae5fa4f5dc37e07518736b
---

## § 4. ESPACES NORMAUX

### 1. Définition des espaces normaux

L’axiome ($O_{IV}$) des espaces uniformisables (IX, p. 7) peut s’énoncer de la façon suivante: *quels que soient l’ensemble fermé A, et le point $x \in CA$, il existe une application continue de X dans $[0, 1]$, égale à 0 au point $x$, et à 1 en tout point de A;* on exprime encore cette propriété en disant que, dans un espace uniformisable, on peut séparer un point et un ensemble fermé (ne contenant pas le point) *par une fonction continue numérique*.

Nous allons maintenant étudier les espaces dans lesquels on peut de la même manière séparer deux ensembles fermés sans point commun *par une fonction continue numérique*; de façon précise:

#### Définition 1 {#top-ix-s4-def-1 .statement}

*On dit qu’un espace topologique X est normal s’il est séparé et s’il vérifie l’axiome suivant:*

$(O_V)$ *Quels que soient les ensembles fermés sans point commun A et B dans X, il existe une application continue de X dans $[0, 1]$, égale à 0 en tout point de A et à 1 en tout point de B.*

Il est clair que tout espace normal est complètement régulier; mais il existe des espaces complètement réguliers et non normaux (voir exerc. 12, 13 (IX, p. 103) 16 (IX, p. 104), 14, 15 (IX, p. 113) et 5 (IX, p. 125).

L’énoncé de l’axiome ($O_V$), comme celui de l’axiome ($O_{IV}$), fait intervenir la droite numérique $\mathbf{R}$ comme ensemble auxiliaire. Mais on peut donner un énoncé équivalent à $(O_v)$, dans lequel n’intervient plus aucun ensemble auxiliaire:

**Théorème 1 (Urysohn).** — *L’axiome* $(O_v)$ *est équivalent au suivant*:
$(O'_v)$ *Quels que soient les ensembles fermés sans point commun A et B dans X, il existe deux ensembles ouverts sans point commun U et V tels que A $\subset$ U et B $\subset$ V.

Il est immédiat que $(O_v)$ entraîne $(O'_v)$, car si $f$ est une application continue de X dans $[0, 1]$, égal à 0 dans A, à 1 dans B, les ensembles ouverts $\overline{f}([0, \frac{1}{2}[)$ et $\overline{f([\frac{1}{2}, 1[)}$ contiennent respectivement A et B et n’ont aucun point commun.

Pour démontrer la réciproque, remarquons d’abord que $(O'_v)$ est équivalent à l’axiome suivant:

$(O''_v)$ *Quel que soit l’ensemble fermé A, et le voisinage ouvert V de A, il existe un voisinage ouvert W de A tel que $\overline{W} \subset V$.

S’il existe une application continue $f$ de X dans $(-1, +1)$, égale à $-1$ dans A, à 1 dans B, et si, pour tout $t \in [0, 1]$, on pose $U(t) = \overline{f}([-1, t[)$, on définit une famille d’ensembles ouverts dans X, ayant $[0, 1]$ pour ensemble d’indices, telle que $A \subset U(0)$, $B \subset \complement U(1)$, et, pour tout couple de nombres réels $t, t'$ tels que $0 \leq t \leq t' \leq 1$

$$(1)$$
$$
U(t) \subset U(t')
$$

puisque $U(t)$ est contenu dans l’ensemble fermé $\overline{f}([-1, t])$. Inversement, supposons qu’on ait défini une famille $U(t)$ d’ensembles ouverts $(0 \leq t \leq 1)$ ayant ces trois propriétés; pour tout $x \in X$, posons $g(x) = 1$ si $x \in \complement U(1)$, et sinon prenons pour $g(x)$ la borne inférieure des $t$ tels que $x \in U(t)$. On a évidemment $0 \leq g(x) \leq 1$ pour tout $x \in X$, $g(x) = 0$ dans A, $g(x) = 1$ dans B; enfin $g$ est *continue* dans X: en effet, si on pose $g(x) = a$, on a $|g(y) - g(x)| < \varepsilon$ pour tout $y$ appartenant à l’ensemble $U(a + \varepsilon) \cap \complement U(a - \varepsilon)$, qui est un voisinage de $x$ d’après (1) (en convenant de prendre $U(a + \varepsilon) = X$ si $a + \varepsilon > 1$, et $U(a - \varepsilon) = \varnothing$ si $a - \varepsilon < 0$).

Tout revient donc à définir une famille d’ensembles ouverts $U(t)$ du type précédent, en s’appuyant sur l’axiome $(O'_v)$. Prenons $U(1) = \complement B$; comme $A \subset U(1)$, il existe d’après $(O''_v)$ un ensemble ouvert $U(0)$ tel que $A \subset U(0)$ et $U(0) \subset U(1)$. Supposons ensuite que, pour chaque nombre *dyadique* $k/2^n$ ($k = 0, 1, \ldots, 2^n$), on ait défini un ensemble ouvert $U(k/2^n)$, ces ensembles étant tels que $U\left(\frac{k}{2^n}\right) \subset U\left(\frac{k+1}{2^n}\right)$ pour $0 \leq k \leq 2^n - 1$. Pour chaque nombre dyadique $\frac{2k+1}{2^{n+1}}$ ($0 \leq k \leq 2^n - 1$), il existe, d’après $(O''_v)$, un ensemble ouvert $U\left(\frac{2k+1}{2^{n+1}}\right)$ tel que

$$
U\left(\frac{k}{2^n}\right) \subset U\left(\frac{2k+1}{2^{n+1}}\right), \quad \text{et} \quad U\left(\frac{2k+1}{2^{n+1}}\right) \subset U\left(\frac{k+1}{2^n}\right).
$$

Pour tout nombre dyadique $r$ tel que $0 \leq r \leq 1$, on peut donc définir un ensemble ouvert $U(r)$, de sorte qu’on ait $A \subset U(0)$, $B \subset \complement U(1)$, et

(2)
$$
\overline{U}(r) \subset U(r')
$$
pour tout couple de nombres dyadiques $r, r'$ tels que $0 \leq r \leq r' \leq 1$.

Posons maintenant, pour tout nombre réel $t \in (0, 1)$,
$$
U(t) = \bigcup_{r \leq t} U(r) \quad (r \text{ dyadique});
$$
d’après (2), cette définition coïncide avec la précédente pour $t$ dyadique; d’autre part, si $0 \leq t < t' \leq 1$, il existe deux nombres dyadiques $r, r'$ tels que $t \leq r < r' \leq t'$; d’après (2), on a
$$
U(t) \subset \overline{U}(r) \subset U(r') \subset U(t'),
$$
ce qui établit la relation (1) et achève la démonstration.

Le th. 1 va nous permettre de démontrer que deux catégories importantes d’espaces topologiques sont des espaces normaux. En premier lieu:

#### Proposition 1 {#top-ix-s4-prop-1 .statement}

*Un espace compact est normal.*
En effet, un tel espace vérifie l’axiome $(\mathrm{O}'_V)$, d’après la prop. 3 de I, p. 61.

En ce qui concerne les espaces *localement compacts*, tout point d’un tel espace possède un voisinage compact, qui est un sous-espace normal; mais on peut donner des exemples d’espaces localement compacts *non normaux* (cf. exerc. 12 (IX, p. 103), exerc. 8 (IX, p. 85), exerc. 14 (IX, p. 113). Nous verrons plus loin (IX, p. 49, prop. 4) que tout espace *paracompact* est normal.

#### Proposition 2 {#top-ix-s4-prop-2 .statement}

*Un espace métrisable est normal.*
Soient $X$ un espace métrisable, $d$ une distance compatible avec la topologie de $X$, $A$ et $B$ deux ensembles fermés sans point commun dans $X$; comme les fonctions $d(x, A)$ et $d(x, B)$ sont continues, l’ensemble $U$ (resp. $V$) des points $x$ tels que $d(x, A) < d(x, B)$ (resp. $d(x, B) < d(x, A)$) est ouvert; il est clair que $A \subset U, B \subset V$ et que $U$ et $V$ ne se rencontrent pas, donc l’axiome $(\mathrm{O}'_V)$ est vérifié.

#### Remarque 1 {#top-ix-s4-n1-rem-1 .statement}

La prop. 2 donne une nouvelle condition *nécessaire* pour qu’un espace topologique soit métrisable; mais cette condition, même jointe à toutes les conditions nécessaires données au § 2, ne donne pas un système de conditions suffisantes pour qu’un espace topologique soit métrisable (cf. IX, p. 113, exerc. 15).

#### Remarque 2 {#top-ix-s4-n1-rem-2 .statement}

On peut donner des exemples d’espaces normaux qui ne sont ni métrisables ni localement compacts (voir IX, p. 113, exerc. 15).

D’après $(\mathrm{O}'_V)$, tout ensemble *fermé* dans un espace normal est un *sous-espace normal*; mais cette propriété n’est pas toujours exacte pour une partie *quelconque* d’un espace normal.

Par exemple, un espace complètement régulier et non normal est homéomorphe à un sous-espace d’un espace compact (IX, p. 8, prop. 3), et ce dernier est normal.

Signalons enfin que le produit de deux espaces normaux n’est pas nécessairement normal (voir IX, p. 103, exerc. 12 et IX, p. 113, exerc. 15).

### 2. Prolongement d’une fonction numérique continue

Soient X et Y deux espaces topologiques, A une partie fermée de X (distincte de X); si f est une application continue de A dans Y, il n’est pas toujours possible de prolonger f en une application continue de X tout entier dans Y. Lorsque Y = \mathbf{R}, la condition de possibilité d’un tel prolongement est donnée par le théorème suivant:

#### Théorème 2 (Urysohn) {#top-ix-s4-thm-2 .statement}

L’axiome (O_V) est équivalent à la propriété suivante:
(O''_V) Quels que soient l’ensemble A fermé dans X, et la fonction numérique (finie ou non) f, définie et continue dans A, il existe un prolongement g de f à l’espace tout entier X, qui est une application continue de X dans \mathbf{R}.

Il est immédiat que (O''_V) entraîne (O_V); car, si B et C sont deux ensembles fermés sans point commun dans X, la fonction égale à 0 dans B, à 1 dans C, est définie et continue dans l’ensemble fermé B \cup C. Si f est un prolongement continu de cette fonction dans X, et si on pose g = \inf(f^+, 1), g est continue dans X, prend ses valeurs dans [0, 1], et est égale à 0 dans B, à 1 dans C.

Montrons inversement que (O_V) entraîne (O''_V); comme \mathbf{R} et l’intervalle (−1, +1) sont homéomorphes, on peut se borner au cas où l’application continue f de A dans \mathbf{R} prend ses valeurs dans (−1, +1). Nous définirons le prolongement g de f en formant une suite (g_n) de fonctions continues dans X, telle que la suite (g_n(x)) soit convergente en tout point vers un nombre de l’intervalle (−1, +1); cette limite sera par définition la valeur de g(x), et il résultera du choix des g_n que la fonction g remplira les conditions voulues.

La définition des g_n repose sur le lemme suivant:

#### Lemme 1 {#top-ix-s4-lem-1 .statement}

Soit u une application continue de A dans (−1, +1); il existe une application continue v de X dans (−\frac{1}{3}, +\frac{1}{3}), telle que |u(x) − v(x)| ≤ \frac{2}{3} pour tout x ∈ A.

En effet, soient H l’ensemble des x ∈ A tels que −1 ≤ u(x) ≤ −\frac{1}{3}, K l’ensemble des x ∈ A tels que \frac{1}{3} ≤ u(x) ≤ 1; H et K sont fermés dans A, donc dans X, et ne se rencontrent pas; d’après (O_V), il existe une application continue v de X dans (−\frac{1}{3}, +\frac{1}{3}), égale à −\frac{1}{3} dans H, à \frac{1}{3} dans K; elle satisfait aux conditions du lemme.

Ce lemme étant démontré, définissons les g_n par récurrence. Appliquant le lemme pour u = f, on définit g_0 comme une application continue de X dans (−\frac{1}{3}, +\frac{1}{3}) telle que |f(x) − g_0(x)| ≤ \frac{2}{3} dans A. Supposons ensuite définie l’application continue g_n de X dans l’intervalle (−1 + (\frac{2}{3})^{n+1}, 1 − (\frac{2}{3})^{n+1}), telle que $|f(x) - g_n(x)| \leq (\frac{2}{3})^{n+1}$ dans A. Appliquant le lemme à la fonction $u(x) = (\frac{3}{2})^{n+1} (f(x) - g_n(x))$, on voit qu’il existe une application continue $h_{n+1}$ de X dans l’intervalle $(-\frac{2^{n+1}}{3^{n+2}}, \frac{2^{n+1}}{3^{n+2}})$ telle que
$$
|f(x) - g_n(x) - h_{n+1}(x)| \leq (\frac{2}{3})^{n+2}
$$
dans A; la récurrence se poursuit en prenant $g_{n+1} = g_n + h_{n+1}$, cette fonction satisfaisant bien à l’inégalité $|g_{n+1}(x)| \leq 1 - (\frac{2}{3})^{n+2}$ dans X, en vertu de la définition de $h_{n+1}$.

De cette définition, on conclut que pour $m \geq p, n \geq p$, on a
$$
|g_m(x) - g_n(x)| \leq \frac{2^{p+1}}{3^{p+2}} \sum_{k=0}^{\infty} \left( \frac{2}{3} \right)^k = \left( \frac{2}{3} \right)^{p+1}
$$
en tout point $x \in X$; on en déduit d’abord que la suite $(g_n(x))$ est une suite de Cauchy, donc converge vers un point $g(x)$ de l’intervalle $(-1, +1)$; comme $f(x) - g_n(x)$ tend vers 0 en tout point de A lorsque $n$ croît indéfiniment, $g$ est bien un prolongement de $f$ à X. Reste à voir que $g$ est continue dans X.

Soit donc $x$ un point quelconque de X; quel que soit $\varepsilon > 0$, il existe $n_0$ tel que, pour $m \geq n_0$ et $n \geq n_0$, on ait $|g_m(y) - g_n(y)| \leq \varepsilon$ pour tout $y \in X$, donc aussi, en faisant tendre $m$ vers $+\infty$, $|g(y) - g_n(y)| \leq \varepsilon$; soit V un voisinage de $x$ tel que $|g_n(y) - g_n(x)| \leq \varepsilon$ pour tout $y \in V$; on aura aussi, pour tout $y \in V$
$$
|g(y) - g(x)| \leq |g(y) - g_n(y)| + |g_n(y) - g_n(x)| + |g(x) - g_n(x)| \leq 3\varepsilon
$$
ce qui montre la continuité de $g$ au point $x$, et achève la démonstration (cette dernière partie du raisonnement utilise, dans un cas particulier, la notion de convergence uniforme, que nous définirons de manière générale dans X, p. 2).

#### Corollaire {#top-ix-s4-n2-cor-1 .statement}

Si $f$ est une fonction numérique finie, définie et continue dans A, il existe une fonction numérique finie $g$, définie et continue dans X, qui prolonge $f$.

Démontrons-le d’abord lorsque $f(x) \geq 0$ dans A; il existe alors un prolongement continu $g_1$ de $f$ à X, prenant ses valeurs dans $[0, +\infty)$. Si on pose $B = g_1^{-1}(+\infty)$, $\overline{B}$ est fermé et ne rencontre pas A par hypothèse; la fonction $h$, égale à $f$ dans A, à 0 dans B, est donc continue dans l’ensemble fermé $A \cup B$. Soit $g_2$ un prolongement continu de $h$ à X, prenant encore ses valeurs dans $[0, +\infty)$; la fonction $g = \inf(g_1, g_2)$ est un prolongement continu de $f$ à X, à valeurs $\geq 0$ et finies en tout point de X.

Pour passer de là au cas général, il suffit de remarquer que, si $f$ est finie et continue dans A, il en est de même de $f^+$ et $f^-$; en prolongeant $f^+$ et $f^-$ à X par des fonctions continues et finies $g_1, g_2$ respectivement, la fonction $g_1 - g_2$ est finie et continue dans X et prolonge $f$.

#### Remarque {#top-ix-s4-n2-rem-1 .statement}

Si X est un espace normal, A une partie fermée de X, il existe aussi un prolongement, continu dans X, de toute application continue $f$ de A dans un cube

I^L (IX, p. 8); en effet, on a alors $f = (f_\lambda)_{\lambda \in L}$, $f_\lambda$ étant une application continue de $A$ dans l’intervalle compact $I$ de $\mathbf{R}$; comme il existe une application continue $g_\lambda$ de $X$ dans $I$ qui prolonge $f_\lambda$, l’application $g = (g_\lambda)$ est un prolongement continu de $f$ à $X$.

### 3. Recouvrements ouverts localement finis d’un ensemble fermé et partitions continues de l’unité dans un espace normal

#### Définition 2 {#top-ix-s4-def-2 .statement}

Soient $X$ un espace topologique, $f$ une fonction numérique définie dans $X$. On appelle support de $f$ et on note $\operatorname{Supp}(f)$ le plus petit ensemble fermé $S$ dans $X$, tel que $f(x) = 0$ dans $C S$.

En d’autre termes, $\operatorname{Supp}(f)$ est l’adhérence dans $X$ de l’ensemble des $x \in X$ tels que $f(x) \neq 0$; on peut encore dire que c’est l’ensemble des $x \in X$ tels que dans tout voisinage de $x$ il existe un point $y$ où $f(y) \neq 0$.

Soit $(f_i)_{i \in I}$ une famille de fonctions numériques finies définies dans $X$, dont les supports forment une famille localement finie (I, p. 6); alors la somme $\sum_{i \in I} f_i(x)$ est définie pour tout $x \in X$ (puisque elle ne comporte qu’un nombre fini de termes $\neq 0$); on note $\sum_{i \in I} f_i$ et on appelle somme de la famille $(f_i)$ la fonction numérique finie $x \mapsto \sum_{i \in I} f_i(x)$. Si chacune des $f_i$ est continue, il en est de même de $f = \sum_{i \in I} f_i$; en effet, pour tout $x \in X$, il y a un voisinage $V$ de $x$ ne rencontrant qu’un nombre fini de supports des $f_i$, et par suite il y a une partie finie $H$ de $I$ telle que $f(y) = \sum_{i \in H} f_i(y)$ pour tout $y \in V$.

#### Définition 3 {#top-ix-s4-def-3 .statement}

Etant donnée une famille $(A_i)_{i \in I}$ de parties d’un espace topologique $X$, on dit qu’une famille $(f_i)_{i \in I}$ de fonctions numériques définies dans $X$ est subordonnée (resp. faiblement subordonnée) à la famille $(A_i)_{i \in I}$ si, pour tout $i \in I$, on a $\operatorname{Supp}(f_i) \subset A_i$ (resp. $f_i(x) = 0$ pour $x \notin A_i$).

Il est clair que si $(f_i)_{i \in I}$ est subordonnée à $(A_i)_{i \in I}$, elle lui est aussi faiblement subordonnée; la réciproque n’est pas nécessairement exacte; si $(f_i)_{i \in I}$ est faiblement subordonnée à $(A_i)_{i \in I}$, on en déduit seulement que $\operatorname{Supp}(f_i) \subset \overline{A}_i$ pour tout $i \in I$ (on notera d’ailleurs que cette relation n’entraîne pas nécessairement $f_i(x) = 0$ pour $x \notin A_i$).

#### Définition 4 {#top-ix-s4-def-4 .statement}

On appelle partition continue de l’unité sur un espace topologique $X$ toute famille $(f_i)_{i \in I}$ de fonctions numériques $\geqslant 0$, continues dans $X$, telle que, pour tout $x \in X$, la famille $(f_i(x))_{i \in I}$ soit sommable dans $\mathbf{R}$ et telle que $\sum_{i \in I} f_i(x) = 1$. On dit qu’une partition de l’unité $(f_i)_{i \in I}$ est localement finie si la famille des supports des $f_i$ est localement finie.

#### Proposition 3 {#top-ix-s4-prop-3 .statement}

Soient $X$ un espace topologique, $(U_i)_{i \in I}$ un recouvrement ouvert de $X$, $(f_i)_{i \in I}$ une partition continue de l’unité sur $X$ faiblement subordonnée à $(U_i)_{i \in I}$. Alors il existe sur $X$ une partition continue localement finie de l’unité, subordonnée à $(U_i)_{i \in I}$.

#### Lemme 2 {#top-ix-s4-lem-2 .statement}

Pour tout $x \in X$ et tout nombre $a > 0$, il existe un voisinage $V$ de $x$ et une partie finie $J$ de $I$ tels que, pour tout $y \in V$ et tout $i \in I - J$, on ait $f_i(y) < a$.

Comme $\sum_{i \in I} f_i(x) = 1$, il existe une partie finie $J$ de $I$ telle que
$$
\sum_{i \in J} f_i(x) > 1 - a/2.
$$
Les $f_i$ étant continues, il existe un voisinage $V$ de $x$ tel que, pour tout $y \in V$, on ait $\sum_{i \in J} f_i(y) > 1 - a$; d’où le lemme.

#### Lemme 3 {#top-ix-s4-lem-3 .statement}

La fonction $\sup_{i \in I} f_i$ est continue dans $X$.

Soit $x$ un point de $X$; il existe $\kappa \in I$ tel que $f_\kappa(x) \neq 0$. Posons $f_\kappa(x) = 4a > 0$, et soit $W$ un voisinage de $x$ dans $X$ tel que $f_\kappa(y) \geq 2a$ pour $y \in W$. En vertu du lemme 2, il existe un voisinage $V$ de $x$ et une partie finie $J$ de $I$ tels que $f_i(y) < a$ pour $y \in V$ et $i \in I - J$. Alors, si $y \in V \cap W$, on a $\sup_{i \in I} f_i(y) \geq 2a$, donc $\sup_{i \in I} f_i(y) = \sup_{i \in J} f_i(y)$, ce qui prouve que $\sup_{i \in I} f_i$ est continue au point $x$.

Posons alors, pour tout $\lambda \in I$,
$$
g_\lambda = \sup(0, f_\lambda - \frac{1}{2} \sup_{i \in I} f_i).
$$
Chacune des fonctions $g_\lambda$ est continue en vertu du lemme 3; en outre la famille $(g_\lambda)_{\lambda \in I}$ est subordonnée à $(U_\lambda)_{\lambda \in I}$ et la famille des supports des $g_\lambda$ est localement finie. En effet, avec les notations du lemme 3, pour $y \in V \cap W$ et $\lambda \in I - J$, on a $f_\lambda(y) < a \leq \frac{1}{2} \sup_{i \in I} f_i(y)$, donc $g_\lambda(y) = 0$ dans $V \cap W$, et par suite
$$
\operatorname{Supp}(g_\lambda) \cap (V \cap W) = \varnothing.
$$
D’autre part, comme $\sum_{i \in I} f_i(z) = 1$ pour tout $z \in X$, on a $\sup_{i \in I} f_i(z) > 0$ pour tout $z \in X$. Si $z$ est un point de $\bigcup U_\lambda$, on a $f_\lambda(z) = 0$ et par continuité il existe un voisinage $T$ de $z$ dans $X$ tel que $f_\lambda(t) - \frac{1}{2} \sup_{i \in I} f_i(t) < 0$ pour $t \in T$, autrement dit $g_\lambda(t) = 0$ pour $t \in T$; cela prouve que $\operatorname{Supp}(g_\lambda) \subset U_\lambda$.

Notons enfin qu’avec les mêmes notations, il existe un indice $\lambda \in J$ tel que $\sup_{i \in I} f_i(x) = f_\lambda(x) > 0$, et l’on a $g_\lambda(x) = \frac{1}{2} f_\lambda(x) > 0$; la fonction $h = \sum_{i \in I} g_i$ est donc continue et $> 0$ en tout point de $X$. On en conclut que si l’on pose $h_i = g_i/h$, la famille $(h_i)_{i \in I}$ est une partition de l’unité répondant aux conditions de l’énoncé.

#### Théorème 3 {#top-ix-s4-thm-3 .statement}

Soit $X$ un espace normal. Pour tout recouvrement ouvert localement fini $(A_i)_{i \in I}$ de $X$, il existe sur $X$ une partition continue de l’unité $(f_i)_{i \in I}$ subordonnée au recouvrement $(A_i)_{i \in I}$ (donc localement finie).

Munissons I d’une structure d’ensemble bien ordonné (E, III, p. 20, th. 1); nous allons définir par récurrence transfinie une famille $(g_i)_{i \in I}$ d’applications continues de $X$ dans $[0, 1]$, telle que: $1^\circ$ Supp$(g_i) \subset A_i$ pour tout $i \in I$; $2^\circ$ si $B_i$ est l’ensemble ouvert des $x \in X$ tels que $g_i(x) > 0$, alors, pour tout $i \in I$, la famille formée des $B_\lambda$ tels que $\lambda \leq i$, et des $A_\lambda$ tels que $\lambda > i$, soit un recouvrement ouvert de $X$. Supposons en effet les $g_i$ définis pour $i < \gamma$, de sorte que les deux propriétés précédentes soient vérifiées pour tout $i < \gamma$, et montrons qu’on peut définir $g_\gamma$ de sorte qu’elles soient aussi vérifiées pour $i = \gamma$. Montrons d’abord que les $B_i$ tels que $i < \gamma$ et les $A_i$ tels que $i \geq \gamma$ forment un recouvrement de $X$. Par hypothèse, pour tout $x \in X$, il n’y a qu’un nombre fini d’indices $\lambda \in I$ tels que $x \in A_\lambda$, soient $\lambda_1 < \lambda_2 < \cdots < \lambda_n$; soit $\lambda_n$ le plus grand des $\lambda_i$ tels que $\lambda_i < \gamma$; si $h < n$, on a $x \in A_{\lambda_n}$ et $\lambda_n \geq \gamma$; si $h = n$, l’hypothèse de récurrence montre que $x$ appartient à un $B_\lambda$ tel que $\lambda \leq \lambda_n < \gamma$, d’où notre assertion. Posons alors $C = (\bigcup_{i < \gamma} B_i) \cup (\bigcup_{i > \gamma} A_i)$; $C$ est ouvert et on a d’après ce qui précède $C \cap A_\gamma \subset C$; en vertu de l’axiome $(O_v)$ des espaces normaux, il existe donc une application continue $g_\gamma$ de $X$ dans $[0, 1]$, telle que $g_\gamma(x) = 0$ dans $C \cap A_\gamma$, et $g_\gamma(x) = 1$ dans $C$. On a par suite Supp$(g_\gamma) \subset A_\gamma$, et d’autre part, l’ensemble $B_\gamma$ des $x$ tels que $g_\gamma(x) > 0$ contient $C$, en d’autres termes, $B_\gamma \cup C = X$. Les $B_i$ tels que $i \leq \gamma$ et les $A_i$ tels que $i > \gamma$ forment donc bien un recouvrement de $X$, ce qui montre que l’on peut poursuivre la récurrence. Cela étant, il est clair que la famille $(B_i)_{i \in I}$ ainsi définie est un recouvrement de $X$ puisque pour tout $x \in X$, il existe un indice $\gamma$ tel que $x \notin A_i$ pour $i > \gamma$. Ce recouvrement étant localement fini, on peut former la fonction continue $g = \sum_{i \in I} g_i$, et par définition des $B_i$, on a $g(x) > 0$ pour tout $x \in X$. Si on pose $f_i(x) = g_i(x)/g(x)$ pour tout $i \in I$ et tout $x \in X$, les $f_i$ forment une partition continue de l’unité subordonnée au recouvrement $(A_i)$.

#### Corollaire 1 {#top-ix-s4-thm-3-cor-1 .statement}

Sous les hypothèses du th. 3, il existe un recouvrement ouvert $(B_i)_{i \in I}$ de $X$ tel que $B_i \subset A_i$ pour tout $i \in I$.

En effet, les $B_i$ construits dans la preuve du th. 3 répondent à la question puisque $B_i = \operatorname{Supp}(g_i)$.

#### Corollaire 2 {#top-ix-s4-thm-3-cor-2 .statement}

Quel que soit le recouvrement ouvert localement fini $(A_i)_{i \in I}$ d’un ensemble fermé $F$ dans un espace normal $X$, il existe une famille $(f_i)_{i \in I}$ de fonctions numériques $\geq 0$, définies et continues dans $X$, qui est subordonnée au recouvrement $(A_i)_{i \in I}$, telle que $\sum_{i \in I} f_i(x) = 1$ pour tout $x \in F$ et que $\sum_{i \in I} f_i(x) \leq 1$ pour tout $x \in X$.

En effet, la famille d’ensembles formées des $A_i$ et de $C F$ est un recouvrement ouvert localement fini de $X$. Il existe donc une partition continue de l’unité subordonnée à ce recouvrement, formée d’une famille $(f_i)_{i \in I}$ telle que $\operatorname{Supp}(f_i) \subset A_i$ pour tout $i \in I$, et d’une fonction $g$ de support contenu dans $C F$; il est clair que la famille $(f_i)$ répond à la question.

### 4. Normalité des espaces paracompacts

Rappelons (I, p. 69) qu’un espace topologique X est dit paracompact s’il est séparé et si pour tout recouvrement ouvert de X il existe un recouvrement ouvert plus fin et localement fini.

#### Proposition 4 {#top-ix-s4-prop-4 .statement}

Tout espace paracompact est normal.

La proposition résultera du lemme suivant:

#### Lemme 4 {#top-ix-s4-lem-4 .statement}

Soient A, B deux parties fermées sans point commun d’un espace paracompact X. Si, pour tout x ∈ A, il existe un voisinage ouvert V_x de x et un voisinage W_x de B sans point commun, alors il existe un voisinage ouvert T de A et un voisinage ouvert U de B sans point commun.

Supposons en effet ce lemme démontré; on peut l’appliquer au cas où B est réduit à un point, puisque X est séparé, et il montre alors que X est régulier. On peut alors appliquer de nouveau le lemme 2 à deux parties fermées quelconques sans point commun dans X, et cela montre que l’axiome (O'_V) est vérifié.

Pour démontrer le lemme, considérons le recouvrement ouvert de X formé de C A et des V_x, où x parcourt A, et soit (T_i)_{i∈I} un recouvrement ouvert plus fin et localement fini; par définition, si A ∩ T_i ≠ ∅, il existe x_i ∈ A tel que T_i ⊂ V_{x_i}. Soit T l’ensemble ouvert réunion des T_i tels que A ∩ T_i ≠ ∅ ; montrons qu’il existe un voisinage ouvert U de B ne rencontrant pas T. En effet, pour tout y ∈ B, il existe un voisinage ouvert S_y de y ne rencontrant qu’un nombre fini d’ensembles T_i ; soit J la partie finie de I formée des indices tels que T_i rencontre à la fois S_y et A; si on pose U_y = S_y ∩ ⋂_{i∈J} W_{x_i}, U_y est un voisinage ouvert de y ne rencontrant aucun des T_i, et par suite U_y ∩ T = ∅. Il suffit alors de prendre U = ⋃_{y∈B} U_y pour répondre à la question.

On peut donner des exemples d’espaces normaux qui ne sont pas paracompacts (IX, p. 107, exerc. 26).

#### Corollaire 1 {#top-ix-s4-lem-4-cor-1 .statement}

Pour tout recouvrement ouvert (A_i)_{i∈I} d’un espace paracompact X, il existe une partition continue de l’unité (f_i)_{i∈I} sur X, subordonnée au recouvrement (A_i).

En effet, soit (U_λ)_{λ∈L} un recouvrement ouvert localement fini plus fin que (A_i)_{i∈I}; il existe donc une application φ de L dans I telle que U_λ ⊂ A_{φ(λ)} pour tout λ ∈ L. D’après le th. 3 (IX, p. 47) et la prop. 4, il existe une partition continue de l’unité (g_λ)_{λ∈L} subordonnée à (U_λ); pour tout i ∈ I, posons f_i = ∑_{φ(λ)=i} g_λ somme qui est définie et continue puisque les supports des g_λ forment une famille localement finie; en outre, la réunion B_i des supports des g_λ tels que φ(λ) = i est fermée (I, p. 6) et contenue dans A_i; comme on a f_i(x) = 0 pour x ∈ C B_i, le support de f_i est contenu dans B_i, donc dans A_i. D’autre part, la famille (B_i) est localement finie, car pour tout x ∈ X, il y a un voisinage V de x et une partie finie

H de L telle que $V \cap U_\lambda = \varnothing$ pour $\lambda \notin H$; on en conclut que $V \cap B_i = \varnothing$ pour $i \notin \varphi(H)$. Enfin, on a, pour tout $x \in X$,

$$
1 = \sum_{\lambda \in L} g_\lambda(x) = \sum_{i \in I} \left( \sum_{\varphi(\lambda) = i} g_\lambda(x) \right) = \sum_{i \in I} f_i(x),
$$

ce qui achève de démontrer le corollaire.

#### Corollaire 2 {#top-ix-s4-lem-4-cor-2 .statement}

*Si F est une partie fermée d’un espace paracompact X, tout voisinage de F dans X contient un voisinage fermé (donc paracompact) de F.*
Cela résulte de I, p. 69, prop. 16, de IX, p. 49, prop. 4 et de l’axiome $(O''_V)$.

#### Proposition 5 {#top-ix-s4-prop-5 .statement}

*Soient X un espace localement compact, R une relation d’équivalence ouverte dans X, telle que l’espace quotient $X/R$ soit paracompact (cf. III, p. 35, prop. 13); soit $\pi$ l’application canonique de X sur $X/R$. Il existe une fonction $F \geq 0$ finie et continue dans X telle que :*

a) F n’est identiquement nulle dans aucune classe suivant R;
b) *pour toute partie compacte K de $X/R$, l’intersection de $\pi^{-1}(K)$ avec $\operatorname{Supp}(F)$ est compacte.*

Pour tout $z \in X/R$, soit $f_z : X \to [0, 1]$ une fonction continue dont le support est compact et qui n’est pas identiquement nulle dans $\pi^{-1}(z)$ (IX, p. 44, th. 2); soit $S_z$ l’ensemble ouvert des points $x \in X$ tels que $f_z(x) > 0$; on a donc $z \in \pi(S_z)$. Comme $\pi$ est une application ouverte, les $\pi(S_z)$ forment un recouvrement ouvert de $X/R$. Il existe donc un recouvrement ouvert $(U_i)_{i \in I}$ de $X/R$ localement fini, plus fin que le recouvrement formé des $\pi(S_z)$, puis (IX, p. 49, cor. 1) une partition continue de l’unité $(g_i)_{i \in I}$ sur $X/R$, subordonnée au recouvrement $(U_i)_{i \in I}$. Pour tout $i \in I$, soit $z_i \in X/R$ tel que $U_i \subset \pi(S_{z_i})$. La fonction $F_i = (g_i \circ \pi) \cdot f_{z_i}$ est continue, a son support contenu dans $\operatorname{Supp}(f_{z_i})$, donc compact; en outre, ce support est aussi contenu dans $\pi^{-1}(U_i)$. Les ensembles $\operatorname{Supp}(F_i)$ forment donc une famille localement finie, de sorte (IX, p. 46) qu’on définit une fonction finie et continue $F \geq 0$ dans X en posant $F = \sum_{i \in I} F_i$. Pour tout $z \in X/R$, il existe $i \in I$ tel que $g_i(z) > 0$, donc $z \in U_i$; puis il existe $x \in S_{z_i}$ tel que $\pi(x) = z$; alors $f_{z_i}(x) > 0$ et $g_i(\pi(x)) > 0$, donc $F_i(x) > 0$ et *a fortiori* $F(x) > 0$; ceci prouve que F possède la propriété a). Enfin, soit K une partie compacte de $X/R$. Il existe une partie finie J de I telle que, pour tout $i \in I - J$, on ait $U_i \cap K = \varnothing$, donc $\pi^{-1}(K) \cap \operatorname{Supp}(F_i) = \varnothing$. Alors

$$
\pi^{-1}(K) \cap \operatorname{Supp}(F) = \pi^{-1}(K) \cap (\bigcup_{i \in I} \operatorname{Supp}(F_i)) = \pi^{-1}(K) \cap (\bigcup_{i \in J} \operatorname{Supp}(F_i))
$$

est compact.

### 5. Paracompacité des espaces métrisables

Le théorème suivant précise la prop. 2 de IX, p. 43.

#### Théorème 4 {#top-ix-s4-thm-4 .statement}

Tout espace métrisable est paracompact.

En effet, si X est un espace métrisable, il est séparé. Il suffit de prouver la proposition suivante:

#### Proposition 6 {#top-ix-s4-prop-6 .statement}

Soient X un espace métrisable, $(U_i)_{i \in I}$ un recouvrement ouvert de X. Il existe une partition continue de l’unité faiblement subordonnée à $(U_i)_{i \in I}$.

En effet, la prop. 3 (IX, p. 46) montre alors qu’il existe aussi une partition continue localement finie de l’unité $(g_i)_{i \in I}$ subordonnée à $(U_i)_{i \in I}$. Les ouverts $V_i = g_i([0, +\infty[)$ formeront un recouvrement ouvert de X, plus fin que $(U_i)_{i \in I}$ et localement fini.

Pour prouver la prop. 6, prenons sur X une distance $d \leq 1$ compatible avec la topologie de X (IX, p. 3 et 15). Pour tout $i \in I$, posons

$$
f_i(x) = d(x, \mathbf{C} U_i).
$$

On a donc $f_i(x) = 0$ si $x \notin U_i$, et

$$
|f_i(x) - f_i(y)| \leq d(x, y)
$$

quels que soient $x, y$ dans X (IX, p. 13, formule (2)), ce qui prouve la continuité de $f_i$. Munissons I d’une structure d’ensemble bien ordonné (E, III, p. 20, th. 1), dont nous noterons $\alpha$ le plus petit élément. Pour tout $i \in I$, posons

$$
g_i(x) = \sup_{\gamma \leq i} f_\lambda(x), \quad h_i(x) = \sup_{\gamma < i} f_\lambda(x)
$$

(en convenant de prendre $h_\alpha(x) = 0$; on notera que si l’ensemble des $\lambda < i$ a un plus grand élément $\kappa$, on a $g_\kappa = h_i$);

$$
h(x) = \sup_{i \in I} f_i(x) = \sup_{i \in I} g_i(x).
$$

En vertu de (3), on a $f_i(x) \leq f_i(y) + d(x, y)$ pour tout $i$, donc

$$
g_i(x) = \sup_{\lambda \leq i} f_\lambda(x) \leq d(x, y) + \sup_{\lambda \leq i} f_\lambda(y) = d(x, y) + g_i(y);
$$

et en échangeant les rôles de $x$ et $y$, on voit que

$$
|g_i(x) - g_i(y)| \leq d(x, y)
$$

et de la même manière

$$
|h_i(x) - h_i(y)| \leq d(x, y), \quad |h(x) - h(y)| \leq d(x, y)
$$

ce qui prouve que les fonctions $g_i, h_i$ et $h$ sont continues dans X. En outre, on a $g_i(x) = \sup(f_i(x), h_i(x)) \geq 0$, et $g_i(x) = h_i(x)$ si $x \notin U_i$.

Posons $u_i(x) = g_i(x) - h_i(x)$, et prouvons que, pour tout $x \in X$, la famille $(u_i(x))$ est sommable dans $\mathbf{R}$ et a pour somme $\sum_{i \in I} u_i(x) = h(x)$. Il suffit évidemment de prouver, par récurrence transfinie, que l’on a

(4)
$$
\sum_{\lambda \leq i} u_\lambda(x) = g_i(x) \quad \text{pour tout } i \in I.
$$

Supposons en effet la relation (4) vérifiée pour $i < \gamma$; alors la famille $(u_\lambda(x))_{\lambda \leq \gamma}$ est sommable dans $\mathbf{R}$ et l’on a
$$
\left( \sum_{\lambda \leq \gamma} u_\lambda(x) \right) - u_\gamma(x) = \sum_{\lambda < \gamma} u_\lambda(x) = \sup_{\lambda < \gamma} \left( \sum_{\mu \leq \lambda} u_\mu(x) \right) = \sup_{\lambda < \gamma} g_\lambda(x) = \sup_{\lambda < \gamma} f_\lambda(x) = h_\gamma(x)
$$
d’où $\sum_{\lambda \leq \gamma} u_\lambda(x) = g_\gamma(x)$.

Alors, la fonction continue $h$ est $> 0$ en tout point, et la famille $(u_i/h)_{i \in I}$ est une partition continue de l’unité faiblement subordonnée à $(U_i)_{i \in I}$. C.Q.F.D.

## EXERCICES {#top-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
