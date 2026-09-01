---
book: top
book_title: General Topology
chapter: X
chapter_title: ESPACES FONCTIONNELS
section: 4
section_title: Approximation des fonctions continues numériques
lang: fr
source: top-v-x-fr
book_pages: TG X.54-TG X.61
pdf_pages: 0282-0290, 0303-0310
extraction: ocr
subsections:
    - "no": 1
      title: Approximation des fonctions continues par les fonctions d’un ensemble réticulé
      page: 0
      pdf_page: 282
    - "no": 2
      title: Approximation des fonctions continues par les polynômes
      page: 35
      pdf_page: 284
    - "no": 3
      title: 'Application: approximation des fonctions numériques continues définies dans un produit d’espaces compacts'
      page: 38
      pdf_page: 287
    - "no": 4
      title: Approximation des applications continues d’un espace compact dans un espace normé
      page: 38
      pdf_page: 287
statements: 18
exercises: 22
content_sha256: e2361ec9ebef01f71cc30be5e5c017b8eda732082bbb548b479fdc56ca49f1a2
---

## § 4. APPROXIMATION DES FONCTIONS CONTINUES NUMÉRIQUES

### 1. Approximation des fonctions continues par les fonctions d’un ensemble réticulé

Nous allons étudier, dans ce paragraphe, l’ensemble $\mathcal{C} = \mathcal{C}(X; \mathbf{R})$ des fonctions continues numériques¹ définies dans un espace compact X ; nous considérons toujours sur cet ensemble la topologie de la convergence uniforme ; on sait (X, p. 21) que cette topologie est définie par la norme $\|f\| = \sup_{x \in X} |f(x)|$, et que cette norme est compatible avec la structure d’algèbre de $\mathcal{C}$ sur le corps $\mathbf{R}$; muni de cette structure d’algèbre et de cette norme, $\mathcal{C}$ est une algèbre normée complète sur le corps $\mathbf{R}$ (X, p. 9, cor. 1).

Étant donné un ensemble $H \subset \mathcal{C}$, nous dirons qu’une fonction numérique f continue dans X peut être approchée uniformément par des fonctions de H si f est adhérente à H dans l’espace $\mathcal{C}$, c’est-à-dire si, pour tout $\varepsilon > 0$, il existe une fonction $g \in H$ telle que $|f(x) - g(x)| \leq \varepsilon$ pour tout $x \in X$. Dire que toute fonction numérique continue dans X peut être approchée uniformément par des fonctions de H signifie donc que H est partout dense dans $\mathcal{C}$.

Sur l’ensemble $\mathcal{C}$, on sait que la relation $f \leq g$ (équivalente à « quel que soit $x \in X, f(x) \leq g(x)$ ») est une relation d’ordre, pour laquelle $\mathcal{C}$ est un ensemble réticulé. On a évidemment $\|u| - |v|\| \leq \|u - v\|$, donc $u \mapsto |u|$ est une application uniformément continue de $\mathcal{C}$ dans lui-même ; on en déduit que

$$
(u, v) \mapsto \sup(u, v) = \frac{1}{2}(u + v + |u - v|)
$$

et

$$
(u, v) \mapsto \inf(u, v) = \frac{1}{2}(u + v - |u - v|)
$$

sont uniformément continues dans $\mathcal{C} \times \mathcal{C}$.

#### Proposition 1 {#top-x-s4-prop-1 .statement}

Soient X un espace compact, H un ensemble de fonctions continues numériques définies dans X. Soit f une fonction numérique continue dans X, et telle que,

¹ Les fonctions numériques dont il sera question dans ce paragraphe seront toujours supposées finies.

pour tout $x \in X$, il existe une fonction $u_x \in H$ telle que $u_x(x) > f(x)$ (resp. $u_x(x) < f(x)$). Alors il existe un nombre fini de fonctions $u_{x_i} = f_i \in H$ ($1 \leq i \leq n$) telles que, si on pose $v = \sup(f_1, f_2, \ldots, f_n)$ (resp. $w = \inf(f_1, f_2, \ldots, f_n)$) on ait $v(x) > f(x)$ (resp. $w(x) < f(x)$) pour tout $x \in X$.

En effet, pour tout $x \in X$, soit $G_x$ l’ensemble ouvert des $z \in X$ tels que $u_x(z) > f(z)$ (resp. $u_x(z) < f(z)$); comme $x \in G_x$ par hypothèse, $X$ est réunion des $G_x$ lorsque $x$ parcourt $X$. Comme $X$ est compact, il existe un nombre fini de points $x_i$ ($1 \leq i \leq n$) tels que les $G_{x_i}$ forment un recouvrement de $X$; il est clair que les fonctions $f_i = u_{x_i}$ répondent à la question.

#### Théorème 1 (Dini) {#top-x-s4-thm-1 .statement}

Soient $X$ un espace compact, $H$ un ensemble filtrant pour la relation $\leq$ (resp. $\geq$) de fonctions numériques continues dans $X$. Si l’enveloppe supérieure (resp. inférieure) $f$ de $H$ est finie et continue dans $X$, $f$ peut être approchée uniformément par des fonctions de $H$ (ou, ce qui revient au même, le filtre des sections de $H$ converge uniformément vers $f$ dans $X$).

En effet, étant donné $\varepsilon > 0$ arbitraire, pour tout $x \in X$ il existe une fonction $u_x \in H$ telle que $u_x(x) > f(x) - \varepsilon$. D’après la prop. 1 et comme $H$ est filtrant pour la relation $\leq$, il existe $g \in H$ telle que $g(x) > f(x) - \varepsilon$ pour tout $x \in X$; comme, d’autre part, on a $g(x) \leq f(x)$ par définition, le théorème est démontré.

#### Corollaire {#top-x-s4-n1-cor-1 .statement}

Soit $(u_n)$ une suite croissante (resp. décroissante) de fonctions numériques continues dans $X$. Si l’enveloppe supérieure (resp. inférieure) $f$ de la suite $(u_n)$ est finie et continue dans $X$, la suite $(u_n)$ converge uniformément vers $f$ dans $X$.

Il est immédiat que la conclusion du th. 1 n’est plus nécessairement exacte si on ne suppose plus $X$ compact, comme le montre l’exemple de la suite décroissante des fonctions $x/(n + x)$ dans $\mathbf{R}_+$.

#### Proposition 2 {#top-x-s4-prop-2 .statement}

Soient $X$ un espace compact, $H$ un ensemble de fonctions continues numériques définies dans $X$, tel que, pour deux fonctions quelconques $u \in H, v \in H$, les fonctions $\sup(u, v)$ et $\inf(u, v)$ appartiennent à $H$. Pour qu’une fonction numérique $f$ continue dans $X$ puisse être approchée uniformément par des fonctions de $H$, il faut et il suffit que, pour tout $\varepsilon > 0$, et tout couple $(x, y)$ de points de $X$, il existe une fonction $u_{x,y} \in H$ telle que $|f(x) - u_{x,y}(x)| < \varepsilon$ et $|f(y) - u_{x,y}(y)| < \varepsilon$.

La condition est évidemment nécessaire; montrons qu’elle est suffisante. Pour tout $\varepsilon > 0$, nous allons montrer qu’il existe une fonction $g \in H$ telle que $|f(z) - g(z)| < \varepsilon$ pour tout $z \in X$. Soit $x$ un point quelconque de $X$, et $H_x$ l’ensemble des fonctions $u \in H$ telles que $u(x) < f(x) + \varepsilon$. Par hypothèse, pour tout $y \in X$, la fonction $u_{x,y}$ appartient à $H_x$ et on a $u_{x,y}(y) > f(y) - \varepsilon$; d’après la prop. 1 (X, p. 33), il existe donc un nombre fini de fonctions de $H_x$ dont l’enveloppe supérieure $v_x$ est telle que $v_x(z) > f(z) - \varepsilon$ pour tout $z \in X$; d’autre part, on a, par définition de $H_x$, $v_x(x) < f(x) + \varepsilon$; enfin, $v_x$ appartient à $H$ d’après l’hypothèse. La prop. 1 montre donc qu’il existe un nombre fini de fonctions $v_{x_i}$ dont l’enveloppe inférieure $g$ est telle que $g(z) < f(z) + \varepsilon$ pour tout $z \in X$; d’autre part, comme on a $v_{x_i}(z) > f(z) - \varepsilon$ pour tout $z \in X$ et pour chaque indice $i$, on a aussi $g(z) > f(z) - \varepsilon$ pour tout $z \in X$; comme $g \in H$ d’après l’hypothèse, la proposition est démontrée.

#### Remarque {#top-x-s4-n1-rem-1 .statement}

Lorsque l’ensemble $H$ satisfait aux conditions de l’énoncé, il est réticulé pour la relation d’ordre $f \leq g$. Mais on notera qu’un sous-ensemble $H$ de $C$ peut être réticulé pour cette relation d’ordre sans que la borne supérieure (resp. inférieure) dans $H$ de deux fonctions $u, v$ de $H$ coïncide avec leur borne supérieure (resp. inférieure) dans $C$, c’est-à-dire avec la fonction
$$
x \mapsto \sup(u(x), v(x)) \quad (\text{resp. } x \mapsto \inf(u(x), v(x))).
$$
\* Un exemple en est fourni par les applications convexes d’un intervalle compact de $\mathbf{R}$ dans $\mathbf{R}$ (cf. FVR, I, § 4, exerc. 20).*

#### Corollaire {#top-x-s4-n1-cor-2 .statement}

*On suppose que $H$ soit tel que, pour deux fonctions quelconques $u \in H$, $v \in H$, les fonctions $\sup(u, v)$ et $\inf(u, v)$ appartiennent à $H$, et en outre que, pour tout couple de points distincts $x, y$ de $X$ et tout couple de nombres réels $\alpha, \beta$, il existe une fonction $g \in H$ telle que $g(x) = \alpha$ et $g(y) = \beta$. Alors toute fonction numérique continue dans $X$ peut être approchée uniformément par des fonctions de $H$.*

#### Théorème 2 (Stone) {#top-x-s4-thm-2 .statement}

*Soient $X$ un espace compact, $H$ un sous-espace vectoriel de $C(X, \mathbf{R})$ tel que: 1° les fonctions constantes appartiennent à $H$; 2° la relation $u \in H$ entraîne $|u| \in H$; 3° $H$ sépare les points de $X$ (IX, p. 9, déf. 5). Dans ces conditions, toute fonction numérique continue dans $X$ peut être approchée uniformément par des fonctions de $H$.*

Il suffit de montrer que $H$ satisfait aux conditions du cor. de la prop. 2. D’après l’hypothèse, si $u \in H$ et $v \in H$,
$$
\sup(u, v) = \frac{1}{2}(u + v + |u - v|) \quad \text{et} \quad \inf(u, v) = \frac{1}{2}(u + v - |u - v|)
$$
appartiennent à $H$. D’autre part, soient $x, y$ deux points distincts quelconques de $X$, $\alpha$ et $\beta$ deux nombres réels quelconques; par hypothèse, il existe une fonction $h \in H$ telle que $h(x) \neq h(y)$; posons $h(x) = \gamma, h(y) = \delta$; comme les constantes appartiennent à $H$, la fonction $g(z) = \alpha + (\beta - \alpha) \frac{h(z) - \gamma}{\delta - \gamma}$ appartient à $H$, et est telle que $g(x) = \alpha$ et $g(y) = \beta$.

### 2. Approximation des fonctions continues par les polynômes

Étant donné un ensemble $H$ de fonctions numériques définies dans un ensemble $X$, nous dirons qu’une fonction numérique définie dans $X$ est un *polynôme* (resp. un *polynôme sans terme constant*) à *coefficients réels par rapport aux fonctions de $H$* si elle est de la forme
$$
x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x))
$$

où $g$ est un polynôme (resp. un polynôme sans terme constant) à coefficients réels par rapport à $n$ indéterminées ($n$ quelconque) et où les $f_i$ ($1 \leq i \leq n$) appartiennent à $\mathbf{H}$.

#### Théorème 3 (Weierstrass-Stone) {#top-x-s4-thm-3 .statement}

Soient $X$ un espace compact, $\mathbf{H}$ un ensemble de fonctions numériques continues dans $X$, séparant les points de $X$. Alors toute fonction numérique continue dans $X$ peut être approchée uniformément par des polynômes (à coefficients réels) par rapport aux fonctions de $\mathbf{H}$.

Il revient au même de dire qu’une sous-algèbre de $\mathcal{C}(X; \mathbf{R})$ qui contient les fonctions constantes et sépare les points de $X$ est dense dans $\mathcal{C}(X; \mathbf{R})$.

Soit $\mathbf{H}_0$ l’ensemble des polynômes par rapport aux fonctions de $\mathbf{H}$ et $\overline{\mathbf{H}}_0$ son adhérence dans $\mathcal{C}$; pour tout polynôme $g$ à $n$ variables, à coefficients réels, $(u_1, u_2, \ldots, u_n) \mapsto g(u_1, u_2, \ldots, u_n)$ est une application continue de $\mathcal{C}^n$ dans $\mathcal{C}$, qui applique $\mathbf{H}_0^n$ dans $\mathbf{H}_0$; elle applique donc $\overline{\mathbf{H}}_0^n$ dans $\overline{\mathbf{H}}_0$ (I, p. 9, th. 1). En particulier, $\overline{\mathbf{H}}_0$ est un sous-espace vectoriel de $\mathcal{C}$, et satisfait évidemment à la première et à la troisième condition du th. 2 (X, p. 35); nous allons voir qu’il satisfait aussi à la seconde, d’où résultera que $\overline{\mathbf{H}}_0 = \mathcal{C}$. Comme toute fonction $u \in \overline{\mathbf{H}}_0$ est bornée dans $X$, il suffira de démontrer le lemme suivant:

#### Lemme 1 {#top-x-s4-lem-1 .statement}

Pour tout nombre $\varepsilon > 0$ et tout intervalle compact $I \subset \mathbf{R}$, il existe un polynôme $p(t)$ sans terme constant tel que $|p(t) - |t|| \leq \varepsilon$ dans $I$.

Il suffit d’établir le lemme dans un intervalle de la forme $I = (-a, +a)$, et par suite, en remplaçant $t$ par $at$, dans l’intervalle $(-1, +1)$. Comme on peut écrire $|t| = \sqrt{t^2}$, le lemme 1 sera donc la conséquence du résultat suivant:

#### Lemme 2 {#top-x-s4-lem-2 .statement}

Soit $(p_n)$ la suite des polynômes sans terme constant définie par récurrence sur $n$ par les conditions $p_0(t) = 0$, et
$$
p_{n+1}(t) = p_n(t) + \frac{1}{2}(t - (p_n(t))^2)
$$
pour $n \geq 0$; dans l’intervalle $(0, 1)$, la suite $(p_n)$ est croissante et converge uniformément vers $\sqrt{t}$.

Il suffit de prouver que, pour tout $t \in (0, 1)$, on a
$$
0 \leq \sqrt{t} - p_n(t) \leq \frac{2\sqrt{t}}{2 + n\sqrt{t}}
$$
car (2) entraîne $0 \leq \sqrt{t} - p_n(t) \leq 2/n$.

L’inégalité (2) est vraie pour $n = 0$; démontrons-la par récurrence; il résulte de l’hypothèse de récurrence (2) que l’on a $0 \leq \sqrt{t} - p_n(t) \leq \sqrt{t}$, donc $0 \leq p_n(t) \leq \sqrt{t}$. On déduit alors de (1) que
$$
\sqrt{t} - p_{n+1}(t) = (\sqrt{t} - p_n(t))(1 - \frac{1}{2}(\sqrt{t} + p_n(t)))
$$

d’où $\sqrt{t} - p_{n+1}(t) \geqslant 0$, et, en vertu de (2)

$$
\begin{align*}
\sqrt{t} - p_{n+1}(t) &\leqslant \frac{2\sqrt{t}}{2 + n\sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2} \right) \\
&\leqslant \frac{2\sqrt{t}}{2 + n\sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2 + (n+1)\sqrt{t}} \right) = \frac{2\sqrt{t}}{2 + (n+1)\sqrt{t}}
\end{align*}
$$

C.Q.F.D.

Lorsqu’on ne suppose plus X compact, la conclusion du th. 3 n’est plus nécessairement exacte. Par exemple, une fonction numérique continue, bornée et non constante dans $\mathbf{R}$, ne peut être approchée uniformément dans $\mathbf{R}$ par des polynômes (cf. X, p. 55, exerc. 6).

#### Proposition 3 {#top-x-s4-prop-3 .statement}

*Soient* $(\mathbf{K}_i)_{i \in I}$ *une famille d’intervalles compacts de* $\mathbf{R}$, $\mathbf{K} = \prod_{i \in I} \mathbf{K}_i$ *l’espace produit de ces intervalles, X un sous-espace compact de K. Toute fonction numérique continue dans X peut être uniformément par des polynômes par rapport aux coordonnées* $x_i = \mathrm{pr}_i x$.

En effet, si $x = (x_i)$ et $y = (y_i)$ sont deux points distincts de X, il existe un indice $i$ tel que $x_i \neq y_i$, ce qui montre que la famille des fonctions continues pr_i satisfait aux conditions du th. 3.

#### Proposition 4 {#top-x-s4-prop-4 .statement}

*Soient* X *un espace compact, A une partie fermée de X, H un ensemble de fonctions numériques continues dans X, séparant les points de* $\mathbf{C} A$, *et tel que A soit l’intersection des ensembles* $u^{-1}(0)$, *où u parcourt* H. *Dans ces conditions, toute fonction numérique continue dans X et nulle dans A peut être approchée uniformément par des polynômes sans terme constant par rapport aux fonctions de H*.

Considérons d’abord le cas particulier où A est réduit à un point $x_0$. L’hypothèse entraîne alors que H sépare les points de X, car si $x \neq x_0$, il existe par hypothèse une fonction $u \in H$ telle que $u(x) \neq 0 = u(x_0)$; pour tout $\varepsilon > 0$ et toute fonction numérique $f$ continue dans X et telle que $f(x_0) = 0$, il existe donc (X, p. 36, th. 3) un polynôme $g$ par rapport aux fonctions de H, tel que $|f(x) - g(x)| \leqslant \varepsilon$ pour tout $x \in X$; on en déduit en particulier $|g(x_0)| \leqslant \varepsilon$, d’où $|f(x) - (g(x) - g(x_0))| \leqslant 2\varepsilon$ pour tout $x \in X$, et comme $g(x) - g(x_0)$ est un polynôme sans terme constant par rapport aux fonctions de H, la proposition est démontrée dans ce cas.

Dans le cas général, considérons dans X la relation d’équivalence R dont les classes sont formées de l’ensemble A et des ensembles $\{x\}$, où $x$ parcourt $\mathbf{C} A$; l’espace quotient $X' = X/R$ est séparé (I, p. 58, prop. 15), et par suite compact. Soit $\varphi$ l’application canonique de X sur X/R; toute fonction numérique continue sur X et s’annulant dans A peut s’écrire $f = f_1 \circ \varphi$, où $f_1$ est une fonction numérique définie et continue dans $X'$, et s’annulant au point $x'_0 = \varphi(A)$; en appliquant la proposition à l’espace $X'$ et au point $x'_0$, on obtient le résultat final.

### 3. Application: approximation des fonctions numériques continues définies dans un produit d’espaces compacts

#### Théorème 4 {#top-x-s4-thm-4 .statement}

Soient $(X_i)_{i \in I}$ une famille d’espaces compacts, $X = \prod_{i \in I} X_i$ leur produit. Toute fonction numérique continue dans $X$ peut être approchée uniformément par des sommes d’un nombre fini de fonctions de la forme $(x_i) \mapsto \prod_{\alpha \in J} u_\alpha(x_\alpha)$, où $J$ est une partie finie (quelconque) de $I$ et où, pour chaque $\alpha \in J$, $u_\alpha$ est une fonction numérique continue dans $X_\alpha$.

En effet, considérons l’ensemble $H$ des « fonctions d’une variable » $(x_i) \mapsto u_\alpha(x_\alpha)$ ($\alpha$ quelconque dans $I$) continues dans $X$; cet ensemble sépare les points de $X$, car si $x = (x_i)$ et $y = (y_i)$ sont deux points distincts de $X$, il existe $\alpha \in I$ tel que $x_\alpha \neq y_\alpha$, et une fonction numérique $h_\alpha$ continue dans $X_\alpha$ telle que $h_\alpha(x_\alpha) \neq h_\alpha(y_\alpha)$; la fonction $x \mapsto h_\alpha(\mathrm{pr}_\alpha x)$ appartient à $H$ et prend des valeurs distinctes aux points $x$ et $y$. Comme tout polynôme par rapport aux fonctions de $H$ est de la forme décrite dans l’énoncé, le théorème résulte du th. 3 (X, p. 36).

Lorsqu’on ne suppose plus tous les espaces $X_i$ compacts, la conclusion du th. 4 n’est plus nécessairement exacte (cf. X, p. 56, exerc. 9).

### 4. Approximation des applications continues d’un espace compact dans un espace normé

Soient $X$ un espace compact, $Y$ un espace vectoriel normé sur le corps $\mathbf{R}$ (IX, p. 32); l’espace $C(X; Y)$ sera toujours supposé muni de la topologie de la convergence uniforme, définie par la norme $\|u\| = \sup_{x \in X} \|u(x)\|$ (X, p. 21).

Étant donné un ensemble $H$ de fonctions numériques continues, définies dans $X$, une famille finie $(u_i)_{1 \leq i \leq n}$ de fonctions appartenant à $H$, et une famille finie $(a_i)_{1 \leq i \leq n}$ de points de $Y$, l’application $x \mapsto \sum_{i=1}^n a_i u_i(x)$ de $X$ dans $Y$ est continue; nous la désignerons par $\sum_{i=1}^n a_i u_i$, et nous dirons que c’est une combinaison linéaire de fonctions de $H$, à coefficients dans $Y$. Nous dirons encore qu’une application continue $f$ de $X$ dans $Y$ peut être approchée uniformément par des combinaisons linéaires (à coefficients dans $Y$) de fonctions de $H$, si $f$ est adhérente au sous-espace vectoriel de $C(X; Y)$ formé par l’ensemble de ces combinaisons.

#### Proposition 5 {#top-x-s4-prop-5 .statement}

Soient $X$ un espace compact, $Y$ un espace normé sur $\mathbf{R}$, $H$ une partie de $C(X; \mathbf{R})$. Si toute fonction numérique continue dans $X$ peut être approchée uniformément par des fonctions de $\mathbf{H}$, toute application continue $\mathbf{f}$ de $X$ dans $Y$ peut être approchée uniformément par des combinaisons linéaires (à coefficients dans $Y$) de fonctions de $\mathbf{H}$.

Étant donné arbitrairement $\varepsilon > 0$, pour tout $x \in X$, il existe un voisinage ouvert de $x$ dans lequel l’oscillation de $\mathbf{f}$ est $\leq \varepsilon$. Il existe donc un recouvrement ouvert fini $(A_i)_{1 \leq i \leq n}$ de $X$ tel que l’oscillation de $\mathbf{f}$ dans chacun des $A_i$ soit $\leq \varepsilon$. Soit $\mathbf{a}_i$ une valeur de $\mathbf{f}$ dans $A_i$ ($1 \leq i \leq n$), et soit $(u_i)_{1 \leq i \leq n}$ une partition continue de l’unité subordonnée au recouvrement $(A_i)$ (IX, p. 47, th. 3). Soit $x$ un point quelconque de $X$; pour tout indice $i$ tel que $x \notin A_i$, on a $u_i(x) = 0$, et pour tout indice $i$ tel que $x \in A_i$, on a $\| \mathbf{f}(x) - \mathbf{a}_i \| \leq \varepsilon$; on en déduit que

$$
\| \mathbf{f}(x) - \sum_{i=1}^n \mathbf{a}_i u_i(x) \| = \| \sum_{i=1}^n (\mathbf{f}(x) - \mathbf{a}_i) u_i(x) \| \leq \varepsilon \sum_{i=1}^n u_i(x) = \varepsilon.
$$

D’autre part, il existe par hypothèse une fonction $v_i \in \mathbf{H}$ telle que

$$
|u_i(x) - v_i(x)| \leq \varepsilon / (\sum_{j=1}^n \| \mathbf{a}_j \|)
$$

pour tout $x \in X$ ($1 \leq i \leq n$); on a donc $\| \mathbf{f}(x) - \sum_{i=1}^n \mathbf{a}_i v_i(x) \| \leq 2\varepsilon$ pour tout $x \in X$, ce qui démontre la proposition.

A chacune des propositions démontrées ci-dessus, où on établit qu’une certaine partie $\mathbf{H}$ de $\mathcal{C}(X; \mathbf{R})$ est partout dense, correspond donc, par la prop. 5, une proposition analogue pour les applications continues de $X$ dans un espace normé quelconque $Y$. Nous nous bornerons à expliciter la proposition qui correspond ainsi au th. 3 (X, p. 36). Étant donné un ensemble $\mathbf{H}$ de fonctions numériques définies dans $X$, appelons polynôme par rapport aux fonctions de $\mathbf{H}$, à coefficients dans $Y$, toute combinaison linéaire, à coefficients dans $Y$, de produits d’une famille finie (éventuellement vide) de fonctions de $\mathbf{H}$. Alors:

#### Proposition 6 {#top-x-s4-prop-6 .statement}

*Soient $X$ un espace compact, $\mathbf{H}$ un ensemble de fonctions numériques continues dans $X$, séparant les points de $X$. Dans ces conditions, toute application continue de $X$ dans un espace normé $Y$ sur $\mathbf{R}$ peut être approchée uniformément par des polynômes par rapport aux fonctions de $\mathbf{H}$, à coefficients dans $Y$.*

la prop. 6 à l’ensemble formé des parties réelles et des parties imaginaires de fonctions $f \in \mathbf{H}$, en remarquant que
$$
\Re f = \frac{1}{2} (f + \bar{f}) \quad \text{et} \quad \Im f = \frac{1}{2i} (f - \bar{f}).
$$

#### Corollaire 1 {#top-x-s4-prop-6-cor-1 .statement}

*Si $X$ est une partie compacte de l’espace $\mathbf{C}^n$, toute application continue $(z_1, z_2, \ldots, z_n) \mapsto f(z_1, z_2, \ldots, z_n)$ de $X$ dans un espace normé $Y$ sur le corps $\mathbf{C}$ peut être approchée uniformément par des polynômes à coefficients dans $Y$ par rapport aux $z_k$ et aux $\overline{z}_k$.*

Nous verrons plus tard qu’en général il n’est pas possible d’approcher uniformément $f$ par des polynômes (à coefficients dans $Y$) *par rapport aux seules variables* $z_k$ même si $Y = \mathbf{C}$.

#### Corollaire 2 {#top-x-s4-prop-6-cor-2 .statement}

*Soient $X$ un espace localement compact, $\mathcal{C}_0(X)$ l’algèbre normée sur $\mathbf{C}$ des applications continues de $X$ dans $\mathbf{C}$, tendant vers $0$ à l’infini. Soit $A$ une sous-algèbre de $\mathcal{C}_0(X)$, séparant les points de $X$, telle que pour tout $x \in X$, il existe $f \in A$ pour laquelle $f(x) \neq 0$, et telle que la relation $f \in A$ entraîne $\bar{f} \in A$. Alors $A$ est dense dans $\mathcal{C}_0(X)$.*

Si $X'$ est l’espace compact obtenu par adjonction à $X$ d’un point à l’infini $\omega$, $\mathcal{C}_0(X)$ s’identifie au sous-espace de $\mathcal{C}(X'; \mathbf{C})$ formé des applications continues nulles au point $\omega$, la norme sur $\mathcal{C}_0(X)$ étant définie par
$$
\|f\| = \sup_{x \in X} |f(x)| = \sup_{x \in X'} |f(x)|.
$$
En vertu de la prop. 7 (X, p. 39), toute fonction $f \in \mathcal{C}_0(X)$ peut être approchée uniformément par des polynômes à coefficients complexes, par rapport à des fonctions appartenant à $A$; en outre, comme $f(\omega) = 0$, le raisonnement de X, p. 37, prop. 4 montre qu’on peut supposer ces polynômes sans terme constant et alors ils appartiennent à $A$.

Comme autre exemple d’application de la prop. 7, citons le résultat suivant:

#### Proposition 8 {#top-x-s4-prop-8 .statement}

*Soit $P$ l’ensemble des applications continues périodiques de $\mathbf{R}^m$ dans $\mathbf{C}$ dont le groupe des périodes contient $\mathbf{Z}^m$. Toute fonction appartenant à $P$ peut être approchée uniformément, dans $\mathbf{R}^m$, par des combinaisons linéaires à coefficients complexes des fonctions de la forme*
$$
(x_1, x_2, \ldots, x_m) \mapsto \mathbf{e}(h_1 x_1 + h_2 x_2 + \cdots + h_m x_m)
$$
*où les $h_i$ sont des entiers* (ces combinaisons sont appelées *polynômes trigonométriques à m variables*).

Il suffit de remarquer que $P$ (muni de la topologie de la convergence uniforme) est canoniquement isomorphe à l’espace des applications continues de l’espace compact $T^m$ dans $\mathbf{C}$ (VII, p. 11), et d’appliquer la prop. 7 à l’ensemble des applications de $T^m$ dans $\mathbf{C}$ qui correspondent aux $m$ applications
$$
(x_1, x_2, \ldots, x_m) \mapsto \mathbf{e}(x_i) \quad (1 \leq i \leq m)
$$
de $\mathbf{R}^m$ dans $\mathbf{C}$.

Exercises

## EXERCICES {#top-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
