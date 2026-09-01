---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: LA FONCTION GAMMA
section: 1
section_title: La fonction gamma dans le domaine réel
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0292-0301, 0310-0311
extraction: ocr
subsections:
    - "no": 1
      title: Définition de la fonction gamma
      page: 0
      pdf_page: 292
    - "no": 2
      title: Propriétés de la fonction gamma
      page: 3
      pdf_page: 294
    - "no": 3
      title: Les intégrales eulériennes
      page: 6
      pdf_page: 297
statements: 8
exercises: 6
content_sha256: 9446e53caabad4339b556318759f3afe3a1e9b177c0eaddd0ed9e70ee4b0f494
---

## § 1. LA FONCTION GAMMA DANS LE DOMAINE RÉEL

### 1. Définition de la fonction gamma

Nous avons défini (E, III, p. 41) la fonction $n!$ pour tout entier $n \geqslant 0$, comme égale au produit $\prod_{0 \leq k < n} (n - k)$; on a donc $0! = 1,\ (n + 1)! = (n + 1).n!$ pour $n \geqslant 0$. Nous poserons $\Gamma(n) = (n - 1)!$ pour tout entier $n \geqslant 1$; nous nous proposons de définir, dans l’ensemble des nombres réels $x > 0$, une fonction continue $\Gamma(x)$, prolongeant la fonction $\Gamma$ définie sur l’ensemble des entiers $\geqslant 1$.

Il est clair qu’il existe une infinité de telles fonctions; comme on a la relation $\Gamma(n + 1) = n\Gamma(n)$ pour tout entier $n \geqslant 1$, nous nous bornerons à considérer, parmi les fonctions continues qui prolongent $\Gamma$, celles qui pour tout $x > 0$ satisfont à l’équation
$$
f(x + 1) = x f(x).
$$
Pour qu’une solution de cette équation soit un prolongement de $\Gamma(n)$, il faut et il suffit qu’on ait en outre $f(1) = 1$.

Si $f$ satisfait à (1), pour tout $n$ entier $> 1$, on a, par récurrence sur $n$
$$
f(x + n) = x(x + 1)(x + 2)\ldots(x + n - 1)f(x)
$$
pour tout $x > 0$. Cette relation montre en particulier que les valeurs de $f$ dans un intervalle $]n, n + 1]$ ($n$ entier $\geqslant 1$) sont déterminées par ses valeurs dans l’intervalle $]0, 1]$. Inversement, soit $\varphi$ une fonction continue dans $]0, 1]$, satisfaisant aux seules conditions $\varphi(1) = 1,\ \lim_{x \to 0} x \varphi(x) = 1$; pour tout entier $n \geqslant 1$, définissons $f$ par la relation
$$
f(x) = (x - 1)(x - 2)\ldots(x - n)\varphi(x - n)
$$

dans l’intervalle ]n, n + 1); il est clair que f est continue dans ]0, +∞[, satisfait à l’équation (1), et prolonge Γ(n).

Si f est une solution continue de (1) et prend des valeurs > 0 dans ]0, 1[, elle prend des valeurs > 0 dans ]0, +∞[ d’après (2); la fonction g(x) = log f(x) est donc définie et continue dans ]0, +∞[ et satisfait dans cet intervalle à l’équation
(3)
$$
g(x + 1) - g(x) = \log x.
$$
Si g_1 est une seconde solution continue de (3) dans ]0, +∞[, et si h = g_1 - g, on a h(x + 1) - h(x) = 0 pour tout x > 0; autrement dit, h est une fonction continue périodique de période 1, définie dans ]0, +∞[; inversement, pour toute fonction h de cette nature, g + h est une solution continue de (3).

#### Proposition 1 {#fvr-vii-s1-prop-1 .statement}

*Il existe une fonction convexe et une seule g, définie dans ]0, +∞[, satisfaisant à l’équation (3) et prenant la valeur 0 pour x = 1.*

Montrons d’abord que s’il existe une fonction g satisfaisant aux conditions de l’énoncé, elle est bien déterminée dans l’intervalle ]0, 1[, et par suite dans tout l’intervalle ]0, +∞[. En effet, pour tout entier n > 1, la pente de la droite joignant le point (n, g(n)) au point (x, g(x)) est fonction croissante de x, puisque g est convexe (I, p. 36, prop. 5); on doit donc avoir, pour 0 < x ≤ 1
$$
\frac{g(n - 1) - g(n)}{(n - 1) - n} \leq \frac{g(n + x) - g(n)}{(n + x) - n} \leq \frac{g(n + 1) - g(n)}{(n + 1) - n}
$$
c’est-à-dire, d’après (3)
(4)
$$
x \log (n - 1) \leq g(x + n) - g(n) \leq x \log n.
$$
Or, d’après (3), on a
$$
g(x + n) - g(n) = g(x) + \log x + \sum_{k=1}^{n-1} (\log (x + k) - \log k).
$$
D’autre part, on peut écrire $\log n = \sum_{k=2}^{n} \log \frac{k}{k - 1}$, donc l’inégalité (4) s’écrit
$$
x \sum_{k=2}^{n-1} \log \frac{k}{k - 1} \leq g(x) + \log x
$$
$$
+ \sum_{k=2}^{n} (\log (x + k - 1) - \log (k - 1)) \leq x \sum_{k=2}^{n} \log \frac{k}{k - 1}.
$$
Posons, pour tout $n \geq 2$
(5)
$$
u_n(x) = x \log \frac{n}{n - 1} - \log (x + n - 1) + \log (n - 1)
$$
et
$$
g_n(x) = -\log x + \sum_{k=2}^{n} u_k(x).
$$

Pour $0 < x \leq 1$, on a donc

$$
g_n(x) - x \log \frac{n}{n-1} \leq g(x) \leq g_n(x).
$$

Comme $\log \frac{n}{n-1}$ tend vers 0 lorsque $n$ tend vers $+\infty$, on déduit de (6) que si la solution $g$ existe, elle est nécessairement égale, dans ]$0, 1]$, à la limite de $g_n(x)$.

Or, on tire aussitôt de la relation (5) que, pour tout $x$ fixe et $> 0$, on a

$$
u_n(x) = -x \log \left(1 - \frac{1}{n}\right) - \log \left(1 + \frac{x-1}{n}\right) + \log \left(1 - \frac{1}{n}\right) \sim \frac{x(x-1)}{2n^2}
$$

lorsque $n$ tend vers $+\infty$, ce qui prouve que la série de terme général $u_n(x)$ converge tout $x > 0$. Chacune des fonctions $u_n(x)$ étant convexe dans ]$0, +\infty[$, ainsi que $-\log x$, la fonction $g(x) = -\log x + \sum_{n=2}^\infty u_n(x)$ est convexe dans cet intervalle (I, p. 35; prop. 2 et prop. 4); enfin, on a $u_n(1) = 0$, d’où $g(1) = 0$, et

$$
u_n(x+1) = u_{n+1}(x) + x \left( \log \frac{n}{n-1} - \log \frac{n+1}{n} \right)
$$

d’où

$$
g(x+1) = -\log (x+1) + x \log 2 + \sum_{n=3}^\infty u_n(x) = \log x + g(x);
$$

autrement dit, $g$ satisfait à l’équation (3) de VII, p. 2.

#### Définition 1 {#fvr-vii-s1-def-1 .statement}

On désigne par $\Gamma(x)$ la fonction $> 0$ définie dans l’intervalle ]$0, +\infty[$, satisfaisant à l’équation

$$
\Gamma(x+1) = x \Gamma(x),
$$

telle que $\Gamma(1) = 1$ et que $\log \Gamma(x)$ soit convexe dans ]$0, +\infty[$.

### 2. Propriétés de la fonction gamma

#### Proposition 2 {#fvr-vii-s1-prop-2 .statement}

Pour tout $x > 0$, on a

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x \cdot n!}{x(x+1)\ldots(x+n)}
$$

(formule de Gauss), et

$$
\Gamma(x) = e^{-\gamma x} \frac{1}{x} \prod_{n=1}^\infty \frac{e^{x/n}}{1 + \frac{x}{n}}
$$

où $\gamma$ désigne la constante d’Euler, et le produit infini du second membre de (9) est absolument et uniformément convergent dans tout intervalle compact de $\mathbf{R}$ ne contenant aucun entier $< 0$ (formule de Weierstrass).

La fonction $\Gamma(x)$ est indéfiniment dérivable dans $]0, +\infty[$, et on a

$$
\frac{\Gamma'(x)}{\Gamma(x)} = -\gamma - \frac{1}{x} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{x+n} \right)
$$

et

$$
\mathrm{D}^k(\log \Gamma(x)) = \sum_{n=0}^{\infty} \frac{(-1)^k(k-1)!}{(x+n)^k} \quad \text{pour } k \geq 2,
$$

les séries qui figurent aux seconds membres de (10) et (11) étant absolument et uniformément convergentes dans tout intervalle compact ne contenant aucun entier $\leq 0$.

En effet, la démonstration de la prop. 1 de VII, p. 2, montre que

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x(n-1)!}{x(x+1)\ldots(x+n-1)}
$$

d’où la formule de Gauss, puisque $\frac{n}{x+n}$ tend vers 1 lorsque $n$ tend vers $+\infty$. On peut aussi écrire

$$
\log \frac{n}{n-1} = \frac{1}{n-1} + \left( \log \frac{n}{n-1} - \frac{1}{n-1} \right),
$$

donc (avec les notations de la prop. 1)

$$
\exp(u_n(x)) = e^{x(\log \frac{n}{n-1} - \frac{1}{n-1})} \frac{e^{x/n-1}}{1 + \frac{x}{n-1}}
$$

et la série de terme général $\log \frac{n}{n-1} - \frac{1}{n-1}$ est absolument convergente et a pour somme $-\gamma$, où $\gamma$ désigne la constante d’Euler (V, p. 32), d’où la formule de Weierstrass.

Pour $|x| \leq a$, on a $|1/(x+n)^k| \leq 1/(n-a)^k$ dès que $n > a$, donc la série du second membre de (11) est absolument et uniformément convergente dans tout intervalle compact de $\mathbf{R}$ ne contenant aucun entier $\leq 0$, quel que soit l’entier $k \geq 2$; le même raisonnement s’applique à la série du second membre de (10), puisque $\left| \frac{1}{n} - \frac{1}{x+n} \right| \leq \frac{a}{n(n-a)}$ pour $|x| \leq a$ et $n > a$. Comme ces séries s’obtiennent en dérivant terme à terme la série

$$
\log \Gamma(x) = -\gamma x - \log x + \sum_{n=1}^{\infty} \left( \frac{x}{n} - \log \left( 1 + \frac{x}{n} \right) \right)
$$

qui converge pour tout $x > 0$, la série de terme général $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ est absolument et uniformément convergente dans tout intervalle compact contenu dans $(0, +\infty)$, et on a bien les relations (10) et (11) de VII, p. 4, pour tout $x > 0$ (II, p. 2, th. 1). D’ailleurs, pour tout $x \in \mathbf{R}$, $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ est défini dès que $n$ est assez grand, donc le th. 1 de II, p. 2, montre encore que le produit infini du second membre de (9) (VII, p. 3) est absolument et uniformément convergent dans tout intervalle compact ne contenant aucun entier $\leq 0$.

La fonction $\Gamma(x)$, définie pour $x > 0$, peut se prolonger à tout l’ensemble des points $x$ distincts des entiers $\leq 0$ de façon à satisfaire à l’équation (7) de VII, p. 3, dans cet ensemble : il suffit, pour $-(n+1) < x < -n$, de poser
$$
\Gamma(x) = \frac{1}{x(x+1)\ldots(x+n)} \Gamma(x+n+1).
$$
D’après la prop. 2 de VII, p. 3, les formules (8), (9), (10) et (11) de VII, p. 3 et 4 sont encore valables dans cet ensemble. La formule (9) (VII, p. 3) montre que $\Gamma(x) \sim 1/x$ lorsque $x$ tend vers 0, d’où, d’après (7) de VII, p. 3,
$$
\Gamma(x) \sim \frac{(-1)^n}{n!(x+n)}
$$
lorsque $x$ tend vers $-n$ ($n$ entier $\geq 0$). La fonction $1/\Gamma(x)$ peut donc être prolongée par continuité à $\mathbf{R}$ tout entier, en lui donnant la valeur 0 aux entiers $\leq 0$; on a alors, pour tout $x \in \mathbf{R}$
$$
\frac{1}{\Gamma(x)} = \lim_{n \to \infty} \frac{x(x+1)\ldots(x+n)}{n^x \cdot n!}
$$
et
$$
\frac{1}{\Gamma(x)} = e^{x\gamma x} \cdot x \prod_{n=1}^{\infty} \left( 1 + \frac{x}{n} \right) e^{-x/n}
$$
et on montre comme dans la prop. 2 de VII, p. 3 que le produit infini du second membre de (13) est absolument et uniformément convergent dans tout intervalle compact de $\mathbf{R}$.

Comme $\Gamma(x) > 0$ pour $x > 0$, l’équation (7) de VII, p. 3, montre que l’on a $\Gamma(x) < 0$ pour $-(2n-1) < x < -(2n-2)$ et $\Gamma(x) > 0$ pour
$$
-2n < x < -(2n-1)
$$
$(n$ entier $\geq 1 )$; $\Gamma(x)$ a pour limite à droite $+\infty$ aux points $-2n, -\infty$ aux points $-(2n+1)$, pour limite à gauche $-\infty$ aux points $-2n, +\infty$ aux points $-(2n+1)$ (pour tout $n \in \mathbf{N}$). La formule (11) de VII, p. 4, montre que, pour $k = 2$, le second membre est toujours $\geq 0$ lorsqu’il est défini, donc
$$
\Gamma''(x) \Gamma(x) - (\Gamma'(x))^2 \geq 0,
$$

et par suite $\Gamma''(x)$ a le signe de $\Gamma(x)$; $\Gamma$ est donc *convexe* pour $x > 0$ et pour $-(2n+2) < x < -(2n+1)$, *concave* pour $-(2n+1) < x < -2n$ ($n \in \mathbf{N}$); on en déduit que, dans les intervalles où $\Gamma$ est convexe, $\Gamma'(x)$ croît de $-\infty$ à $+\infty$, et dans les intervalles où $\Gamma$ est concave, $\Gamma'(x)$ décroît de $+\infty$ à $-\infty$. D’où la courbe représentative de $\Gamma$ (fig. 1).

### 3. Les intégrales eulériennes

Nous dirons pour abréger qu’une fonction $f$ définie dans un intervalle $I \subset \mathbf{R}$ et $> 0$ dans cet intervalle, est *logarithmiquement convexe* dans $I$ si $\log f$ est convexe dans $I$. La définition de $\Gamma(x)$ montre donc que cette fonction est logarithmiquement convexe dans $]0, +\infty[$.

Il est clair que le *produit* de deux fonctions logarithmiquement convexes dans $I$ est logarithmiquement convexe dans $I$. En outre:

#### Lemme 1 {#fvr-vii-s1-lem-1 .statement}

*Soient* $f$ et $g$ *deux fonctions* $> 0$ *et deux fois dérivables dans un intervalle ouvert* $I$. *Si* $f$ *et* $g$ *sont logarithmiquement convexes dans* $I$, $f + g$ *est logarithmiquement convexe dans* $I$.

En effet, la relation $D^2(\log f(x)) \geq 0$ s’écrit $f(x)f''(x) - (f'(x))^2 \geq 0$. Nous sommes ramenés à montrer que les relations $a \geq 0,\ a' \geq 0,\ ac - b^2 \geq 0,\ a'c' - {b'}^2 \geq 0$ entraînent $(a + a')(c + c') - (b + b')^2 \geq 0$; or, les relations $a \geq 0,\ ac - b^2 \geq 0$ équivalent au fait que la forme quadratique $ax^2 + 2bxy + cy^2$ est $\geq 0$ dans $\mathbf{R}^2$, et il est clair que si
$$
ax^2 + 2bxy + cy^2 \geq 0 \quad \text{et} \quad a'x^2 + 2b'xy + c'y^2 \geq 0
$$
dans $\mathbf{R}^2$, on a aussi $(a + a')x^2 + 2(b + b')xy + (c + c')y^2 \geq 0$ dans $\mathbf{R}^2$.

#### Lemme 2 {#fvr-vii-s1-lem-2 .statement}

Soit une fonction numérique finie et $> 0$, définie et continue dans le produit $I \times J$ de deux intervalles ouverts dans $\mathbf{R}$ et telle que, pour tout $t \in J$, la fonction $x \mapsto f(x, t)$ soit logarithmiquement convexe et deux fois dérivable dans $I$. Dans ces conditions, si pour tout $x \in I$, l’intégrale $g(x) = \int_J f(x, t)\ dt$ est convergente, $g$ est logarithmiquement convexe dans $I$.

Montrons d’abord que, pour tout intervalle compact $K \subset J$, la fonction $g_K(x) = \int_K f(x, t)dt$ est logarithmiquement convexe. En effet, si $K = [a, b]$, la suite des fonctions
$$
g_n(x) = \frac{b - a}{n} \sum_{k=0}^{n-1} f\left(x, a + k \frac{b - a}{n}\right)
$$
converge simplement vers $g_K(x)$ dans $I$ (II, p. 7, prop. 5), donc $\log g_n$ converge simplement vers $\log g_K$; d’après le lemme 1 de VII, p. 6, $\log g_n$ est convexe dans $I$, donc (I, p. 35, prop. 4) il en est de même de $\log g_K$.

D’autre part, $g$ est limite simple des $g_K$ suivant l’ordonné filtrant des intervalles compacts contenus dans $I$ (II, p. 15), donc $\log g$ est limite simple des $\log g_K$; ces dernières fonctions étant convexes dans $I$, il en est de même de $\log g$ (I, p. 35, prop. 4).

On montre facilement que les lemmes 1 et 2 sont encore valables lorsque l’on n’y suppose plus les fonctions deux fois dérivables (VII, p. 20, exerc. 5).

#### Lemme 3 {#fvr-vii-s1-lem-3 .statement}

Soit $\varphi$ une fonction continue et $> 0$ dans un intervalle ouvert $J$ contenu dans $]0, +\infty[$. Si $I$ est un intervalle ouvert tel que l’intégrale $g(x) = \int_J t^{x-1}\varphi(t)dt$ soit convergente pour tout $x \in I$, $g$ est logarithmiquement convexe dans $I$.

En effet, $\log t^{x-1} = (x - 1) \log t$ est une fonction de $x$ qui est convexe et deux fois dérivable pour tout $t > 0$, donc le lemme 2 est applicable.

#### Proposition 3 {#fvr-vii-s1-prop-3 .statement}

Pour tout $x > 0$, on a
$$
\Gamma(x) = \int_0^\infty e^{-t} t^{x-1}\ dt
$$
(seconde intégrale eulérienne).

En effet, la fonction $g(x) = \int_0^\infty e^{-t} t^{x-1} dt$ est définie pour tout $x > 0$ (V, p. 19); le lemme 3 de VII, p. 7, montre donc qu’elle est logarithmiquement convexe dans ]0, +∞[. D’autre part, en intégrant par parties, on a
$$
g(x+1) = \int_0^\infty e^{-t} t^x dt = -e^{-t} t^x \Big|_0^\infty + x \int_0^\infty e^{-t} t^{x-1} dt = xg(x).
$$
Autrement dit, $g$ est une solution de l’équation (1) de VII, p. 1; enfin,
$$
g(1) = \int_0^\infty e^{-t} dt = 1;
$$
la proposition résulte donc de la prop. 1 de VII, p. 2.

Par le changement de variable $e^{-t} = u$, on déduit de (14) (VII, p. 7) la formule
$$
\Gamma(x) = \int_0^1 \left( \log \frac{1}{t} \right)^{x-1} dt.
$$
De même, par le changement de variable $u = t^x$, il vient
$$
x \Gamma(x) = \int_0^\infty e^{-t/x} dt
$$
ou encore, en tenant compte de (7) (VII, p. 1)
$$
\Gamma\left(1 + \frac{1}{x}\right) = \int_0^\infty e^{-t^x} dt
$$
et en particulier, pour $x = 2$
$$
\Gamma\left(\frac{3}{2}\right) = \frac{1}{2} \Gamma\left(\frac{1}{2}\right) = \int_0^\infty e^{-t^2} dt.
$$

#### Proposition 4 {#fvr-vii-s1-prop-4 .statement}

Pour $x > 0$ et $y > 0$, l’intégrale
$$
B(x, y) = \int_0^1 t^{x-1}(1-t)^{y-1} dt
$$
(première intégrale eulérienne) a pour valeur
$$
B(x, y) = \frac{\Gamma(x)\Gamma(y)}{\Gamma(x+y)}.
$$
En effet, l’intégrale est convergente pour $x > 0$ et $y > 0$ (V, p. 19). D’après le lemme 3 de VII, p. 7, la fonction $x \mapsto B(x, y)$ est logarithmiquement convexe pour $x > 0$. D’autre part, on a
$$
B(x+1, y) = \int_0^1 (1-t)^{x+y-1} \left( \frac{t}{1-t} \right)^x dt
$$
d’où, en intégrant par parties
$$
B(x+1, y) = -\frac{(1-t)^{x+y}}{x+y} \left( \frac{t}{1-t} \right)^x \Big|_0^1 \\
+ \frac{x}{x+y} \int_0^1 (1-t)^{x+y} \left( \frac{t}{1-t} \right)^{x-1} \frac{dt}{(1-t)^2} = \frac{x}{x+y} B(x, y).
$$

Il en résulte que $f(x) = B(x, y) \Gamma(x + y)$ satisfait à l’identité (1) de VII, p. 1. D’autre part cette fonction est logarithmiquement convexe, comme produit de deux fonctions logarithmiquement convexes. Enfin, on a $f(1) = B(1, y) \Gamma(y + 1)$, et $B(1, y) = \int_0^1 (1 - t)^{y-1} dt = 1/y$, d’où $f(1) = \frac{1}{y} \Gamma(y + 1) = \Gamma(y)$. La fonction $f(x)/\Gamma(y)$ est donc égale à $\Gamma'(x)$ d’après la prop. 1 de VII, p. 2, ce qui démontre (18).

Par le changement de variable $t = \frac{u}{u + 1}$, la formule (18) devient

$$
\int_0^\infty \frac{t^{x-1}}{(1 + t)^{x+y}} dt = \frac{\Gamma(x)\Gamma(y)}{\Gamma(x + y)}
$$

et par le changement de variable $t = \sin^2 \varphi$,

$$
\int_0^{\pi/2} \sin^{2x-1}\varphi \cos^{2y-1}\varphi d\varphi = \frac{1}{2} \frac{\Gamma(x)\Gamma(y)}{\Gamma(x + y)}.
$$

Si, dans cette dernière formule, on fait $x = y = \frac{1}{2}$, il vient

$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$

d’où, en vertu de (17)

$$
\int_0^\infty e^{-t^2} dt = \frac{1}{2} \sqrt{\pi}.
$$

D’après la relation (7) de VII, p. 3, on a pour $\Gamma(x)$, au voisinage de 0, le développement asymptotique

$$
\Gamma(x) = \frac{1}{x} \Gamma(x + 1)
$$
$$
= \frac{1}{x} + \Gamma'(1) + \frac{1}{2!} \Gamma''(1)x + \cdots + \frac{1}{n!} \Gamma^{(n)}(1)x^{n-1} + O(x^n).
$$

De même, pour tout $y$ fixe et $> 0$, on peut écrire

$$
\frac{1}{\Gamma(x + y)}
$$
$$
= \frac{1}{\Gamma(y)} + D\left( \frac{1}{\Gamma(y)} \right)x + \frac{1}{2!} D^2\left( \frac{1}{\Gamma(y)} \right)x^2 + \cdots + \frac{1}{n!} D^n\left( \frac{1}{\Gamma(y)} \right)x^n + O_1(x^{n+1})
$$

et la formule (18) donne donc, pour $y$ fixe, le développement asymptotique au voisinage de $x = 0$

$$
B(x, y) = \frac{1}{x} + \left( \Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} \right)
$$
$$
+ \left( \frac{\Gamma''(1)}{2} - \Gamma'(1) \frac{\Gamma'(y)}{\Gamma(y)} + \frac{2{\Gamma'}^2(y) - \Gamma(y)\Gamma''(y)}{2\Gamma^2(y)} \right)x + O(x^2).
$$

D’autre part, pour $x > 0$ et $y > 0$, on a
$$
\text{B}(x, y) = \int_0^1 \left( t^{x-1} + t^x \frac{(1-t)^{y-1} - 1}{t} \right) dt
$$
$$
= \frac{1}{x} + \int_0^1 t^x \frac{(1-t)^{y-1} - 1}{t} dt.
$$
La fonction $\varphi(t) = \frac{(1-t)^{y-1} - 1}{t}$ est continue dans l’intervalle compact $[0, 1]$; comme
$$
t^x = e^{x \log t} = 1 + x \log t + \frac{x^2}{2!} (\log t)^2 + \cdots + \frac{x^n}{n!} (\log t)^n + r_n(x, t)
$$
avec $|r_n(x, t)| \leq \frac{x^{n+1}}{(n+1)!} |\log t|^{n+1}$ (puisque $\log t \leq 0$ et $x > 0$), la formule (25) donne pour $\text{B}(x, y)$ le développement asymptotique au voisinage de $x = 0$
$$
\text{B}(x, y) = \frac{1}{x} + \int_0^1 \varphi(t) \, dt + x \int_0^1 \varphi(t) \log t \, dt + \cdots
$$
$$
+ \frac{x^n}{n!} \int_0^1 \varphi(t) (\log t)^n \, dt + O_2(x^{n+1}).
$$
Pour $n = 1$, l’identification de ce développement à (24) donne en particulier
$$
\Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} = \int_0^1 \frac{(1-t)^{y-1} - 1}{t} \, dt.
$$
D’ailleurs la formule (10) donne $\Gamma'(1) = \Gamma'(1)/\Gamma(1) = -\gamma$, donc (intégrale de Gauss)
$$
\frac{\Gamma'(x)}{\Gamma(x)} + \gamma = \int_0^1 \frac{1 - (1-t)^{x-1}}{t} \, dt.
$$

## EXERCICES {#fvr-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
