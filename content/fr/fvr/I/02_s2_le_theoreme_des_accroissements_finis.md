---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DÉRIVÉES
section: 2
section_title: Le théorème des accroissements finis
lang: fr
source: fvr-i-vii-fr
book_pages: FVR I.20-FVR I.27, FVR I.43-FVR I.46
pdf_pages: 0018-0025, 0041-0044
extraction: ocr
subsections:
    - "no": 1
      title: Théorème de Rolle
      page: 20
      pdf_page: 18
    - "no": 2
      title: Le théorème des accroissements finis pour les fonctions numériques
      page: 21
      pdf_page: 19
    - "no": 3
      title: Le théorème des accroissements finis pour les fonctions vectorielles
      page: 23
      pdf_page: 21
    - "no": 4
      title: Continuité des dérivées
      page: 26
      pdf_page: 24
statements: 21
exercises: 14
content_sha256: 5f7fd3a934efbad19ca044626397a8b33e935d66181fbad2c1fcc07084b1bff4
---

## § 2. LE THÉORÈME DES ACCROISSEMENTS FINIS

Dans les propositions démontrées au § 1, hypothèses et conclusions ont un caractère local : elles ne font intervenir que des propriétés des fonctions considérées dans un voisinage arbitrairement petit d’un point fixe. Au contraire, les questions dont nous allons nous occuper dans ce paragraphe font intervenir les propriétés d’une fonction dans tout un intervalle.

### 1. Théorème de Rolle

**Proposition 1** (« théorème de Rolle »). — Soit $f$ une fonction numérique finie et continue dans un intervalle fermé $I = [a, b]$ (où $a < b$), admettant en tout point de $]a, b[$ une dérivée (finie ou non), et telle que $f(a) = f(b)$. Il existe alors un point $c$ (au moins) de $]a, b[$ tel que $f'(c) = 0$.

La proposition est évidente si $f$ est constante; sinon $f$ prend par exemple des valeurs $> f(a)$, et atteint donc sa borne supérieure en un point $c$ intérieur à $I$ (TG, IV, p. 27, th. 1). Comme en ce point $f$ admet un maximum relatif, on a $f'(c) = 0$ (I, p. 20, prop. 7).

#### Corollaire {#fvr-i-s2-n1-cor-1 .statement}

Soit $f$ une fonction numérique finie et continue dans $[a, b]$ (où $a < b$), admettant en tout point de $]a, b[$ une dérivée (finie ou non). Il existe alors un point $c$ (au moins) de $]a, b[$ tel que $f(b) - f(a) = f'(c)(b - a)$.

Il suffit d’appliquer la prop. 1 à $f(x) = \frac{f(b) - f(a)}{b - a}(x - a)$.

Ce corollaire signifie qu’il existe un point $M_c = (c, f(c))$ de la courbe représentative $C$ de $f$ tel que $a < c < b$ et qu’en ce point la tangente à $C$ soit parallèle à la droite joignant les points $M_a = (a, f(a))$ et $M_b = (b, f(b))$.

### 2. Le théorème des accroissements finis pour les fonctions numériques

Du corollaire de la prop. 1 résulte en particulier l’importante propriété suivante : si on a $m \leq f'(x) \leq M$ dans $]a, b[$, on a aussi $m \leq \frac{f(b) - f(a)}{b - a} \leq M$. Autrement dit, d’une majoration de la dérivée $f'$ dans tout un intervalle d’extrémités $a, b$ résulte la même majoration du rapport $\frac{f(b) - f(a)}{b - a}$ (rapport de l’« accroissement » de la fonction à l’« accroissement » de la variable dans l’intervalle). Nous allons dans ce qui suit préciser et généraliser ce résultat fondamental.

#### Proposition 2 {#fvr-i-s2-prop-2 .statement}

Soit $f$ une fonction numérique finie et continue dans un intervalle fermé borné $I = [a, b]$ (où $a < b$), et admettant une dérivée à droite (finie ou non) en tous les points du complémentaire par rapport à $[a, b[$ d’une partie dénombrable $A$ de cet intervalle. Si $f'_d(x) \geq 0$ en tout point $x$ de $[a, b[$ n’appartenant pas à $A$, on a $f(b) \geq f(a)$; si en outre $f'_d(x) > 0$ en un point au moins de $[a, b[$, on a $f(b) > f(a)$.

Soit $\varepsilon > 0$ un nombre arbitraire, et désignons par $(a_n)_{n \geq 1}$ une suite obtenue en rangeant dans un certain ordre les points de l’ensemble dénombrable $A$. Soit $J$ l’ensemble des points $y \in I$ tels que, pour tout $x$ tel que $a \leq x \leq y$, on ait

$$
f(x) - f(a) \geq - \varepsilon (x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

la somme du second membre étant étendue à l’ensemble des indices $n$ tels que $a_n < x$. Nous allons démontrer que si $f'_d(x) \geq 0$ en tout point de $[a, b[$ distinct des $a_n$, on a $J = I$.

Il est clair que $J$ n’est pas vide, puisque $a \in J$; d’autre part, la définition de cet ensemble montre que si $y \in J$, on a $x \in J$ pour $a \leq x \leq y$, donc $J$ est un intervalle d’origine $a$ (TG, IV, p. 7, prop. 1); soit $c$ son extrémité. On a $c \in J$; c’est évident si $c = a$; sinon, pour tout $x < c$, on a l’inégalité (1), et a fortiori

$$
f(x) - f(a) \geq - \varepsilon (c - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

d’où, en faisant tendre $x$ vers $c$ dans cette inégalité, résulte (en raison de la continuité de $f$) que $c$ satisfait à (1).

Cela étant, nous allons voir qu’on a nécessairement $c = b$. En effet, si on avait $c < b$, ou bien on aurait $c \notin A$; alors $f'_d(c)$ existerait, et comme $f'_d(c) \geq 0$ par hypothèse, il existerait un $y$ tel que $c < y \leq b$ et que pour $c \leq x \leq y$, l’on ait

$$
f(x) - f(c) \geq - \varepsilon (x - c)
$$

d’où, en tenant compte de (1), où x est remplacé par c
$$
f(x) - f(a) \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n} \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
ce qui signifie qu’on aurait y \in J, contrairement à la définition de c. Ou bien on aurait c = a_k pour un indice k; comme f est continue au point a_k, il existerait un y tel que c < y \leq b et que, pour c < x \leq y, on ait
$$
f(x) - f(c) \geq -\frac{\varepsilon}{2^k}
$$
d’où, en tenant compte de (1), où x est remplacé par c,
$$
f(x) - f(a) \geq -\varepsilon(c-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n} \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
ce qui entraîne de nouveau contradiction; on a donc bien c = b, et par suite
(2)
$$
f(b) - f(a) \geq -\varepsilon(b-a) - \varepsilon \sum_{a_n < b} \frac{1}{2^n} \geq -\varepsilon(b-a) - \varepsilon.
$$
Comme \varepsilon > 0 est arbitraire, on déduit de (2) qu’on a f(b) \geq f(a), ce qui démontre la première partie de la proposition.

Remarquons maintenant que ce résultat appliqué à un intervalle [x, y] où a \leq x < y \leq b, prouve que f est croissante dans I; si on avait f(b) = f(a), on en déduirait que f est constante dans I, et par suite que f'_a(x) = 0 en tout point de [a, b[; d’où la seconde partie de l’énoncé.

#### Corollaire {#fvr-i-s2-n2-cor-1 .statement}

Soit f une fonction numérique finie et continue dans [a, b] (où a < b) et admettant une dérivée à droite en tous les points du complémentaire par rapport à [a, b[ d’une partie dénombrable A de cet intervalle. Pour que f soit croissante dans I, il faut et il suffit que f'_a(x) \geq 0 en tout point de [a, b[ n’appartenant pas à A; pour que f soit strictement croissante, il faut et il suffit que la condition précédente soit vérifiée, et en outre que l’ensemble des points x où f'_a(x) > 0 soit partout dense dans [a, b].

#### Remarque 1 {#fvr-i-s2-n2-rem-1 .statement}

La prop. 2 reste valable quand on remplace dans son énoncé l’intervalle [a, b[ par ]a, b] et les mots « dérivée à droite » par « dérivée à gauche ».

#### Remarque 2 {#fvr-i-s2-n2-rem-2 .statement}

L’hypothèse de la continuité de f dans l’intervalle fermé I (et non seulement sa continuité à droite¹ en tout point de [a, b[) est essentielle pour la validité de la prop. 2 (cf. I, p. 43, exerc. 8).

#### Remarque 3 {#fvr-i-s2-n2-rem-3 .statement}

La conclusion de la prop. 2 devient inexacte si on suppose seulement que l’ensemble A des points « exceptionnels » est rare dans I, mais non dénombrable (cf. I, p. 44, exerc. 3).

La prop. 2 entraîne le théorème fondamental suivant (en apparence plus général):

¹ Une fonction définie dans un intervalle I \subset \mathbf{R} est dite continue à droite en un point x_0 \in I si sa restriction à l’intervalle I \cap (x_0, +\infty[ est continue au point x_0 par rapport à cet intervalle; il revient au même de dire que la limite à droite de la fonction au point x_0 existe et est égale à la valeur de la fonction en ce point.

#### Théorème 1 (théorème des accroissements finis) {#fvr-i-s2-thm-1 .statement}

Soient $f$ et $g$ deux fonctions numériques finies et continues dans un intervalle fermé borné $I = [a, b]$, et admettant une dérivée à droite (finie ou non) en tous les points du complémentaire par rapport à $[a, b[$ d’une partie dénombrable de cet intervalle. On suppose en outre que $f'_d(x)$ et $g'_d(x)$ ne peuvent devenir infinis simultanément qu’aux points d’une partie dénombrable de $I$ et qu’il existe deux nombres finis $m, M$ tels que

$$
m \cdot g'_d(x) \leq f'_d(x) \leq M \cdot g'_d(x)
$$

sauf aux points d’une partie dénombrable de $I$ (en remplaçant $M \cdot g'_d(x)$ (resp. $m \cdot g'_d(x)$) par 0 si $M = 0$ (resp. $m = 0$) et $g'_d(x) = \pm \infty$. Dans ces conditions, on a

$$
m(g(b) - g(a)) < f(b) - f(a) < M(g(b) - g(a))
$$

sauf lorsqu’on a $f(x) = M \cdot g(x) + k$, ou $f(x) = m \cdot g(x) + k$ ($k$ constante) pour tout $x \in I$.

Il suffit d’appliquer la prop. 2 aux fonctions $M \cdot g - f$ et $f - m \cdot g$, qui, en vertu des hypothèses faites, ont une dérivée à droite positive sauf aux points d’une partie dénombrable de $I$.

#### Remarque {#fvr-i-s2-n2-rem-4 .statement}

Le th. 1 est inexact si on suppose dans l’énoncé que $f'_d$ et $g'_d$ peuvent simultanément infinis aux points d’une partie non dénombrable de $I$ (cf. I, p. 44, exerc. 3).

#### Corollaire {#fvr-i-s2-n2-cor-2 .statement}

Soit $f$ une fonction numérique finie et continue dans $[a, b]$ (où $a < b$) et admettant une dérivée à droit (finie ou non) en tous les points du complémentaire $B$ par rapport à $[a, b[$ d’une partie dénombrable de cet intervalle. Si $m$ et $M$ sont les bornes inférieure et supérieure de $f'_d$ dans $B$, on a

$$
m(b - a) < f(b) - f(a) - M(b - a)
$$

si $f$ n’est pas une fonction linéaire affine ; si $f$ est linéaire affine, on a

$$
m = M = \frac{f(b) - f(a)}{b - a}.
$$

Les inégalités (5) sont des conséquences de (4) lorsque $m$ et $M$ sont finis; le cas où l’un ou l’autre de ces nombres est infini est trivial.

#### Remarque {#fvr-i-s2-n2-rem-5 .statement}

Les inégalités (5) prouvent qu’une fonction continue ne peut avoir une dérivée à droite égale à $+\infty$ en tout point d’un intervalle (cf. I, p. 43, exerc. 6).

### 3. Le théorème des accroissements finis pour les fonctions vectorielles

#### Théorème 2 {#fvr-i-s2-thm-2 .statement}

Soit $\mathbf{f}$ une fonction vectorielle définie et continue dans un intervalle fermé borné $I = [a, b]$ de $\mathbf{R}$ (où $a < b$) et prenant ses valeurs dans un espace normé $\mathbf{E}$ sur $\mathbf{R}$; soit $g$ une fonction numérique continue et croissante dans $I$. On suppose que $\mathbf{f}$ et $g$ admettent une dérivée à droite en tous les points du complémentaire par rapport à $[a, b[$ d’une partie dénombrable $A$ de cet intervalle $(g'_a(x))$ pouvant être infinie en certains des points $x \notin A$, et qu’en chacun de ces points on a
$$
\|f'_a(x)\| \leq g'_a(x).
$$
Dans ces conditions, on a
$$
\|f(b) - f(a)\| \leq g(b) - g(a).
$$
La démonstration suit une marche tout à fait analogue à celle de la prop. 2. Soient $\varepsilon > 0$ un nombre arbitraire, et $(a_n)$ la suite obtenue en rangeant dans un certain ordre les points de $A$. Soit $J$ l’ensemble des points $y \in I$ tels que, pour tout $x$ tel que $a \leq x \leq y$, on ait
$$
\|f(x) - f(a)\| \leq g(x) - g(a) + \varepsilon(x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n};
$$
nous allons montrer que $J = I$. On voit d’abord, comme dans la prop. 2, que $J$ est un intervalle d’origine $a$; si $c$ est son extrémité, on a $c \in J$; en effet, pour tout $x < c$, on a la relation (8), et a fortiori
$$
\|f(x) - f(a)\| \leq g(c) - g(a) + \varepsilon(c - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$
d’où, en faisant tendre $x$ vers $c$ dans cette inégalité, résulte, en raison de la continuité de $f$, que $c$ satisfait à (8).

Montrons qu’on a nécessairement $c = b$. En effet, supposons $c < b$, et d’abord que $c \notin A$; $f'_a(c)$ et $g'_a(c)$ existent donc et vérifient (6); supposons en premier lieu que $g'_a(c)$ (qui est nécessairement $\geq 0$) soit finie; alors on peut toujours écrire $f'_a(c) = u g'_a(c)$, avec $\|u\| \leq 1$; la fonction $f(x) - u g(x)$ ayant au point $c$ une dérivée à droite nulle, il existe un $y$ tel que $c < y \leq b$ et que, pour $c \leq x \leq y$, on ait
$$
\|f(x) - f(c) - u(g(x) - g(c))\| \leq \varepsilon(x - c)
$$
d’où
$$
\|f(x) - f(c)\| \leq g(x) - g(c) + \varepsilon(x - c)
$$
et, en tenant compte de (8), où $x$ est remplacé par $c$
$$
\|f(x) - f(a)\| \leq g(x) - g(a) + \varepsilon(x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
$$
\leq g(x) - g(a) + \varepsilon(x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}.
$$
On aurait donc $y \in J$, ce qui est contradictoire. Supposons ensuite qu’on ait $c \notin A$ et $g'_a(c) = +\infty$; il existe alors un $y$ tel que $c < y \leq b$ et que, pour $c \leq x \leq y$, on ait, d’une part
$$
\|f(x) - f(c)\| \leq (\|f'_a(c)\| + 1)(x - c)
$$

et d'autre part
$$
g(x) - g(c) \geq (\|f'_d(c)\| + 1)(x - c)
$$
d'où
$$
\|f(x) - f(c)\| \leq g(x) - g(c)
$$
et on conclut comme précédemment. Enfin, si on a $c = a_k$, il existe un $y$ tel que $c < y \leq b$ et que, pour $c < x \leq y$, on ait
$$
\|f(x) - f(c)\| \leq \frac{\varepsilon}{2^k}
$$
d'où en, tenant compte de (8), où $x$ est remplacé par $c$,
$$
\|f(x) - f(a)\| \leq g(c) - g(a) + \varepsilon(c - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
$$
\leq g(x) - g(a) + \varepsilon(x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
ce qui entraîne de nouveau contradiction. La démonstration se termine comme celle de la propr. 2.

C.Q.F.D.

#### Remarque 1 {#fvr-i-s2-n3-rem-1 .statement}

Ici encore, on peut remplacer dans l'énoncé du th. 2 l'intervalle $[a, b]$ par ]$a, b$$]$ et « dérivée à droite » par « dérivée à gauche ».

#### Remarque 2 {#fvr-i-s2-n3-rem-2 .statement}

Nous montrerons plus tard comment on peut préciser les cas d'égalité dans la relation (7), et aussi comment on peut généraliser le th. 2 au cas où $E$ est un espace localement convexe quelconque, à l'aide d'une autre méthode de démonstration qui permet de déduire le th. 2 du th. 1.

#### Corollaire {#fvr-i-s2-n3-cor-1 .statement}

Pour qu'une fonction vectorielle continue dans un intervalle $I \subset \mathbf{R}$, à valeurs dans un espace normé $E$ sur $\mathbf{R}$, soit constante dans $I$, il suffit qu'elle ait une dérivée à droite nulle en tous les points du complémentaire (par rapport à $I$) d'une partie dénombrable de $I$.

#### Remarque {#fvr-i-s2-n3-rem-3 .statement}

Les démonstrations des th. 1 et 2 font intervenir de façon essentielle les propriétés topologiques particulières au corps $\mathbf{R}$; on peut en effet donner des exemples de corps valués $K$ pour lesquels il existe des applications continues non constantes de $K$ dans lui-même qui ont en tout point une dérivée nulle (cf. I, p. 44, exerc. 2).

#### Proposition 3 {#fvr-i-s2-prop-3 .statement}

Soit $f$ une fonction vectorielle à valeurs dans un espace normé $E$ sur $\mathbf{R}$, définie et continue dans un intervalle $I \subset \mathbf{R}$, dérivable à droite dans le complémentaire $B$ (par rapport à $I$) d'une partie dénombrable de $I$; quels que soient les points $x_0 \in B,\ x \in I,\ y \in I$, on a (en supposant par exemple $x < y$)
$$
\|f(y) - f(x) - f'_d(x_0)(y - x)\| \leq (y - x) \sup_{z \in B,\ x < z < y} \|f'_d(z) - f'_d(x_0)\|.
$$

Il suffit en effet d’appliquer le th. 2 en remplaçant $\mathbf{f}$ par la fonction
$$
\mathbf{f}(z) - \mathbf{f}'_d(x_0)z,
$$
et $g$ par la fonction linéaire dont la dérivée est $\sup_{z \in B,\ x < z < y} \| \mathbf{f}'_d(z) - \mathbf{f}'_d(x_0) \|$.

Le th. 2 s’étend aux fonctions vectorielles d’une variable complexe :

#### Proposition 4 {#fvr-i-s2-prop-4 .statement}

*Soit $\mathbf{f}$ une fonction vectorielle d’une variable complexe définie, continue et dérivable dans une partie ouverte convexe $A$ du corps $\mathbf{C}$, à valeurs dans un espace normé $E$ sur le corps $\mathbf{C}$. Si on a $\| \mathbf{f}'(z) \| \leq m$ pour tout $z \in A$, on a $\| \mathbf{f}(b) - \mathbf{f}(a) \| \leq m | b - a |$ pour tout couple de points $a, b$ de $A$.*

Posons en effet $g(t) = \frac{1}{b - a} \mathbf{f}(a + t(b - a))$ pour $0 \leq t \leq 1$; comme $g'(t) = \mathbf{f}'(a + t(b - a))$, l’application du th. 2 à la fonction $g$ donne aussitôt la proposition.

#### Corollaire {#fvr-i-s2-n3-cor-2 .statement}

*Pour qu’une fonction vectorielle $\mathbf{f}$ d’une variable complexe, définie et continue dans un ensemble $A \subset \mathbf{C}$, à valeurs dans un espace normé sur $\mathbf{C}$, soit constante, il suffit qu’elle ait une dérivée nulle en tout point de $A$.*

En effet, soit $a$ un point quelconque de $A$; l’ensemble $B$ des points $z$ de $A$ où $\mathbf{f}(z) = \mathbf{f}(a)$ est fermé puisque $\mathbf{f}$ est continue; il est aussi ouvert par application de la prop. 4 (avec $m = 0$) à un voisinage ouvert convexe, contenu dans $A$, d’un point quelconque de $B$; donc il est identique à $A$.

#### Proposition 5 {#fvr-i-s2-prop-5 .statement}

*Soit $\mathbf{f}$ une fonction vectorielle d’une variable complexe, définie, continue et dérivable dans un ensemble ouvert convexe $A \subset \mathbf{C}$, à valeurs dans un espace normé sur le corps $\mathbf{C}$; quels que soient les points $x_0, x$ et $y$ dans $A$, on a*
$$
\| \mathbf{f}(y) - \mathbf{f}(x) - \mathbf{f}'(x_0) (y - x) \| \leq |y - x| \cdot \sup_{z \in A} \| \mathbf{f}'(z) - \mathbf{f}'(x_0) \|.
$$
Il suffit d’appliquer le th. 2 à la fonction
$$
g(t) = \mathbf{f}(x + t(y - x)) - \mathbf{f}'(x_0) (y - x)t
$$
dans l’intervalle $[0, 1]$.

### 4. Continuité des dérivées

#### Proposition 6 {#fvr-i-s2-prop-6 .statement}

*Soient $I$ un intervalle ouvert de $\mathbf{R}$, $x_0$ une des extrémités de $I$, $\mathbf{f}$ une fonction vectorielle définie et continue dans $I$, prenant ses valeurs dans un espace normé complet $E$ sur $\mathbf{R}$; on suppose que $\mathbf{f}$ admet une dérivée à droite aux points du complémentaire $B$, par rapport à $I$, d’une partie dénombrable de $I$. Pour que $\mathbf{f}'_d(x)$ ait une limite lorsque $x$ tend vers $x_0$ en restant dans $B$ et $\neq x_0$, il faut et il suffit que $\frac{\mathbf{f}(y) - \mathbf{f}(x)}{y - x}$ ait une limite $c$ lorsque $(x, y)$ tend vers $(x_0, x_0)$ de sorte que $x \in I, y \in I, x \neq x_0, y \neq x_0$ et $x \neq y$. Dans ces conditions, $\mathbf{f}$ se prolonge par continuité au point $x_0$, $\mathbf{f}'_d(x)$ tend vers $\mathbf{c}$ lorsque $x$ tend vers $x_0$ (en restant dans B) et la fonction $\mathbf{f}$ prolongée (définie dans $I \subset \{x_0\}$) admet au point $x_0$ une dérivée égale à $\mathbf{c}$.

Supposons par exemple que $x_0$ soit l’extrémité de $I$. Montrons d’abord que si $\mathbf{f}'_d(x)$ tend vers $\mathbf{c}$ lorsque $x$ tend vers $x_0$ en restant dans B et $\neq x_0$, $\frac{\mathbf{f}(y) - \mathbf{f}(x)}{y - x}$ tend vers $\mathbf{c}$; cela résulte aussitôt du th. 2 appliqué à la fonction $\mathbf{f}(z) - \mathbf{c}z$, qui donne
$$
\| \mathbf{f}(y) - \mathbf{f}(x) - \mathbf{c}(y - x) \| \leq (y - x) \sup_{z \in B, x < z < y} \| \mathbf{f}'_d(z) - \mathbf{c} \|
$$
pour $x < y < x_0$. Inversement, si $\frac{\mathbf{f}(y) - \mathbf{f}(x)}{y - x}$ tend vers $\mathbf{c}$, pour tout $\varepsilon > 0$, il existe $h > 0$ tel que les conditions $|x - x_0| < h, |y - x_0| < h$ ($x \neq x_0, y \neq x_0$) entraînent
$$
\| \mathbf{f}(y) - \mathbf{f}(x) - \mathbf{c}(y - x) \| \leq \varepsilon |y - x|.
$$
Mais pour tout $x \in B$ et $\neq x_0$, tel que $|x - x_0| < h$, il existe $k > 0$ (dépendant de $x$) tel que la relation $x < y < x + k$ entraîne
$$
\| \mathbf{f}(y) - \mathbf{f}(x) - \mathbf{f}'_d(x)(y - x) \| \leq \varepsilon |y - x|
$$
d’où, en tenant compte de (11):
$$
\| \mathbf{f}'_d(x) - \mathbf{c} \| \leq 2\varepsilon
$$
pour $|x - x_0| < h, x \in B$ et $x \neq x_0$, ce qui prouve que $\mathbf{f}'_d(x)$ tend vers $\mathbf{c}$. En outre, de la relation (11) on tire d’abord que
$$
\| \mathbf{f}(y) - \mathbf{f}(x) \| \leq (\|\mathbf{c}\| + \varepsilon) |y - x|,
$$
ce qui prouve (critère de Cauchy) que $\mathbf{f}$ a une limite $\mathbf{d}$ au point $x_0$, lorsque $x$ tend vers ce point en restant dans $I$ et $\neq x_0$; faisant alors tendre $x$ vers $x_0$ dans (11), il vient, pour $y \in I, y \neq x_0$ et $|y - x_0| \leq h$,
$$
\left\| \frac{\mathbf{f}(y) - \mathbf{d}}{y - x_0} - \mathbf{c} \right\| \leq \varepsilon
$$
ce qui prouve que $\mathbf{c}$ est la dérivée au point $x_0$ de la fonction $\mathbf{f}$ prolongée par continuité à $I \cap \{x_0\}$.

#### Remarque {#fvr-i-s2-n4-rem-1 .statement}

Un raisonnement analogue, basé sur le th. 1, montre que si $f$ est une fonction numérique telle que $f'_d(x)$ tende vers $+\infty$ au point $x_0$, le rapport
$$
(f(y) - f(x))/(y - x)
$$
tend aussi vers $+\infty$, et réciproquement; si en outre $f$ a une limite finie au point $x_0$ (ce qui ici n’est plus une conséquence de l’hypothèse), la fonction $f$ prolongée au point $x_0$ par continuité a une dérivée égale à $+\infty$ en ce point.

## EXERCICES {#fvr-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
