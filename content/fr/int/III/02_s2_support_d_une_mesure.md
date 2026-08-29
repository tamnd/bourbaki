---
book: int
book_title: Integration
chapter: III
chapter_title: Mesures sur les espaces localement compacts
section: 2
section_title: Support d'une mesure
lang: fr
source: int-i-iv-fr
pdf_pages: 0068-0078, 0105-0106
extraction: ocr
subsections:
    - "no": 1
      title: Restriction d’une mesure à un ensemble ouvert. Définition d’une mesure par des données locales
      page: 0
      pdf_page: 68
    - "no": 2
      title: Support d’une mesure
      page: 0
      pdf_page: 70
    - "no": 3
      title: Caractérisation du support d’une mesure
      page: 0
      pdf_page: 72
    - "no": 4
      title: Mesures ponctuelles. Mesures à support fini
      page: 0
      pdf_page: 74
    - "no": 5
      title: Mesures discrètes
      page: 0
      pdf_page: 77
statements: 29
exercises: 5
content_sha256: 80fd53862ef7813c763749b44d7cbf4452a8f26a1227bdf81c37b2810f0d9b8b
---

## § 2. Support d’une mesure

### 1. Restriction d’une mesure à un ensemble ouvert. Définition d’une mesure par des données locales

Soient X un espace localement compact, Y un ensemble ouvert dans X. Le sous-espace Y de X est localement compact, et toute fonction continue à valeurs dans un espace vectoriel topologique E, définie dans Y et à support compact, peut être prolongée par continuité à X tout entier, en lui donnant la valeur 0 dans $\mathbf{C}Y$; on peut donc de cette manière identifier l’espace $\mathcal{K}(Y; E)$ au sous-espace de $\mathcal{K}(X; E)$ formé des fonctions continues à support compact contenu dans Y. Si $\mu$ est une mesure sur X, il est clair que la restriction de $\mu$ à $\mathcal{K}(Y; \mathbf{C})$ est une mesure sur Y, qu’on appelle restriction de $\mu$ au sous-espace ouvert Y, ou encore mesure induite sur Y par $\mu$ et que l’on note $\mu|Y$. Les restrictions à Y de $|\mu|$, $\mathcal{R}\mu$ et $\mathcal{I}\mu$ sont respectivement $|\mu|Y$, $\mathcal{R}(\mu|Y)$ et $\mathcal{I}(\mu|Y)$ en vertu du § 1, n°s 5 et 6. Si $\mu$ est réelle, les restrictions de $\mu^+$ et $\mu^-$ à Y sont respectivement $(\mu|Y)^+$ et $(\mu|Y)^-$, en vertu de la formule (8) du § 1, n° 5.

On voit aussitôt que si Y et Z sont deux ensembles ouverts dans X tels que $Y \supseteq Z$, et si $\mu|Y$ et $\mu|Z$ sont les restrictions de $\mu$ à Y et à Z, $\mu|Z$ est aussi la restriction de $\mu|Y$ au sous-espace ouvert Z de l’espace localement compact Y.

Au chap. IV, § 5, n° 7, nous généraliserons cette définition au cas où Y est un sous-espace localement compact de X.

On notera qu’une mesure sur $Y$ *n’est pas nécessairement* la restriction d’une mesure sur $X$ (cf. chap. V, § 7, n° 2, prop. 6).

Par exemple, soit $Y$ l’intervalle ouvert $]0, 1[$ de $X = \mathbf{R}$; l’application
$$
f \mapsto \int_0^1 \frac{f(x)}{x} dx
$$
est une mesure sur $Y$, car toute fonction de $\mathcal{K}(Y; \mathbf{C})$ est nulle dans un voisinage de 0 dans $\mathbf{R}$. Mais cette mesure ne peut être prolongée en une mesure sur $\mathbf{R}$, car dans le cas contraire, sa restriction à l’ensemble des fonctions $f \in \mathcal{K}(Y; \mathbf{C})$ telles que $\|f\| \leq 1$ serait bornée ; or, cela est inexact.

On a toutefois la proposition suivante :

#### Proposition 1 {#int-iii-s2-prop-1 .statement}

*Soit* $(Y_\alpha)_{\alpha \in A}$ *un recouvrement ouvert de* $X$, *et supposons donnée, sur chaque sous-espace* $Y_\alpha$, *une mesure* $\mu_\alpha$, *de sorte que pour tout couple* $(\alpha, \beta)$, *les restrictions de* $\mu_\alpha$ *et de* $\mu_\beta$ *à* $Y_\alpha \cap Y_\beta$ *soient identiques. Dans ces conditions, il existe une mesure* $\mu$ *et une seule sur* $X$ *dont la restriction à* $Y_\alpha$ *soit égale à* $\mu_\alpha$ *pour tout indice* $\alpha$.

Montrons en premier lieu que toute fonction $f \in \mathcal{K}(X; \mathbf{C})$ peut s’écrire sous la forme d’une somme finie $f = \sum_i f_i$, où, pour chacune des fonctions $f_i \in \mathcal{K}(X; \mathbf{C})$, il existe un indice $\alpha_i$ tel que $\operatorname{Supp}(f_i) \subset Y_{\alpha_i}$. Si $K = \operatorname{Supp}(f)$, il existe un nombre fini d’indices $\alpha_i$ ($1 \leq i \leq n$) tels que les $Y_{\alpha_i}$ forment un recouvrement de $K$; soient $h_i$ ($1 \leq i \leq n$) des applications continues de $X$ dans $]0, 1[$ telles que le support de $h_i$ soit compact et contenu dans $Y_{\alpha_i}$ pour $1 \leq i \leq n$, et que l’on ait $\sum_{i=1}^n h_i(x) = 1$ dans $K$ ($§ 1$, n° 2, lemme 1); les fonctions $f_i = f h_i$ répondent à la question. Ceci montre en premier lieu que s’il existe une mesure $\mu$ répondant à la question, elle est *unique*, car pour toute somme finie $f = \sum_{i=1}^n f_i$, où $f_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$, on doit avoir $\mu(f) = \sum_{i=1}^n \mu_{\alpha_i}(f_i)$. On aura en outre montré l’existence d’une forme linéaire $\mu$ sur $\mathcal{K}(X; \mathbf{C})$ dont la restriction à chaque sous-espace $\mathcal{K}(Y_\alpha; \mathbf{C})$ est $\mu_\alpha$, pourvu qu’on démontre la propriété suivante : si $(g_i)_{1 \leq i \leq m}$ et $(h_j)_{1 \leq j \leq n}$ sont deux suites finies de fonctions de $\mathcal{K}(X; \mathbf{C})$ telles que $g_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$ pour $1 \leq i \leq m$, $h_j \in \mathcal{K}(Y_{\beta_j}; \mathbf{C})$ pour $1 \leq j \leq n$, et
$$
\sum_{i=1}^m g_i(x) = \sum_{j=1}^n h_j(x) = 1
$$

dans K, on a

$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{j=1}^{n} \mu_{\beta_j}(f h_j).
$$

Or, on a

$$
f g_i = \sum_{j=1}^{n} f g_i h_j,
$$

d’où

$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{i=1}^{m} \sum_{j=1}^{n} \mu_{\alpha_i}(f g_i h_j).
$$

De même

$$
\sum_{j=1}^{n} \mu_{\beta_j}(f h_j) = \sum_{j=1}^{n} \sum_{i=1}^{m} \mu_{\beta_j}(f g_i h_j).
$$

Mais comme le support de $f g_i h_j$ est contenu dans $Y_{\alpha_i} \cap Y_{\beta_j}$, on a $\mu_{\alpha_i}(f g_i h_j) = \mu_{\beta_j}(f g_i h_j)$, ce qui établit notre assertion.

Il reste à voir que $\mu$ est une mesure sur $X$; or, tout point de $X$ admet un voisinage compact contenu dans un des $Y_\alpha$; la conclusion résulte donc aussitôt de la définition de $\mu$ et de la prop. 6 du n° 3 du § 1.

#### Corollaire (principe de localisation) {#int-iii-s2-n1-cor-1 .statement}

Soient $\mu$ et $\nu$ deux mesures sur $X$, et soit $(Y_\alpha)$ une famille d’ensembles ouverts de $X$ telle que, pour tout $\alpha$, les restrictions à $Y_\alpha$ de $\mu$ et $\nu$ soient égales; alors les restrictions de $\mu$ et $\nu$ à $Y = \bigcup_\alpha Y_\alpha$ sont égales.

### 2. Support d’une mesure

Soit $\mu$ une mesure sur un espace localement compact $X$, et soit $\mathcal{G}$ l’ensemble des ensembles ouverts $U \subset X$ tels que la restriction de $\mu$ à $U$ soit nulle; il résulte aussitôt du principe de localisation (n° 1, cor. de la prop. 1) que, si $U_0$ est la réunion des ensembles $U \in \mathcal{G}$, $U_0$ appartient lui-même à $\mathcal{G}$, et est par suite le plus grand des ensembles de $\mathcal{G}$.

#### Définition 1 {#int-iii-s2-def-1 .statement}

On appelle support d’une mesure $\mu$ sur un espace localement compact $X$ et on note $\operatorname{Supp}(\mu)$ l’ensemble fermé complémentaire du plus grand des ensembles ouverts de $X$ dans lesquels la restriction de $\mu$ est nulle.

Dire qu’un point $x \in X$ n’appartient pas au support de $\mu$ signifie qu’il existe un voisinage ouvert $V$ de $x$ tel que la restriction de $\mu$ à V soit nulle ; dire que $x$ appartient au support de $\mu$ signifie donc que pour tout voisinage $V$ de $x$, il existe une fonction $f \in \mathcal{H}(X; \mathbf{C})$, dont le support est contenu dans $V$, et qui est telle que $\mu(f) \neq 0$.

#### Exemple 1 {#int-iii-s2-n2-exa-1 .statement}

Pour qu’une mesure sur $X$ soit *nulle*, il faut et il suffit que son support soit *vide*.

#### Exemple 2 {#int-iii-s2-n2-exa-2 .statement}

Le support de la mesure de Lebesgue sur $\mathbf{R}$ est la droite $\mathbf{R}$ tout entière ; en effet, il n’est pas vide et est invariant par toute translation.

#### Exemple 3 {#int-iii-s2-n2-exa-3 .statement}

Sur l’intervalle $X = \{0, 1\}$ de $\mathbf{R}$, considérons un ensemble dénombrable partout dense, rangé en une suite $(a_n)$, et soit $\mu$ la mesure définie par la masse $2^{-n}$ placée au point $a_n$ pour tout $n \geq 0$ (§ 1, n° 3, Exemple 1). Le support de $\mu$ est $X$ tout entier ; en effet, soient $x$ un point quelconque de $X$, $V$ un voisinage de $x$, $f$ une fonction numérique continue et $> 0$ dans $X$, égale à 1 au point $x$, et dont le support est contenu dans $V$ (§ 1, n° 2, lemme 1) ; l’ensemble des $y \in V$ tels que $f(y) > 0$ est ouvert dans $X$, donc contient un point $a_n$, et par suite $\mu(f) \geq f(a_n)2^{-n} > 0$.

#### Proposition 2 {#int-iii-s2-prop-2 .statement}

*Le support d’une mesure $\mu$ est identique au support de la mesure $|\mu|$ ; si $\mu$ est réelle, son support est réunion des supports des mesures $\mu^+$ et $\mu^-$*.

En effet, si la restriction de $\mu$ à un ouvert $U$ est nulle, il en est de même de la restriction de $|\mu|$ (resp. de $\mu^+$ et de $\mu^-$ lorsque $\mu$ est réelle), et réciproquement.

On notera que les supports de $\mu^+$ et $\mu^-$ peuvent être non vides et *identiques* (cf. chap. V, § 5, exerc. 6).

#### Proposition 3 {#int-iii-s2-prop-3 .statement}

*Si $\mu$ et $\nu$ sont deux mesures sur un espace localement compact $X$, telles que $|\mu| \leq |\nu|$, on a $\mathrm{Supp}(\mu) \subset \mathrm{Supp}(\nu)$*.

En effet, si la restriction de $\nu$ à un ensemble ouvert est nulle, il en est de même de celle de $\mu$.

#### Proposition 4 {#int-iii-s2-prop-4 .statement}

*Le support de la somme de deux mesures est contenu dans la réunion de leurs supports*.

En effet, si les restrictions de deux mesures à un ensemble ouvert sont nulles, il en est de même de la restriction de leur somme.

Si $\mu$ et $\nu$ sont deux mesures *positives*, le support de $\lambda = \mu + \nu$ est *égal* à la réunion des supports de $\mu$ et de $\nu$ : en effet, si $x_0$ est un point de cette réunion, $V$ un voisinage quelconque de $x_0$, il existe une fonction continue $f \geq 0$, de support contenu dans $V$, et telle que l’un des deux nombres $\mu(f)$, $\nu(f)$ soit $> 0$ ; *a fortiori*, on a

$$
\lambda(f) = \mu(f) + \nu(f) > 0.
$$

#### Proposition 5 {#int-iii-s2-prop-5 .statement}

Le support de la restriction d’une mesure $\mu$ à un ensemble ouvert $U$ est la trace sur $U$ du support de $\mu$.

La proposition est évidente à partir des définitions.

#### Proposition 6 {#int-iii-s2-prop-6 .statement}

L’ensemble des mesures sur un espace localement compact $X$, dont le support est contenu dans un ensemble fermé $F$, est un sous-espace vectoriel vaguement fermé de $\mathcal{M}(X; \mathbf{C})$.

En effet, c’est l’intersection des hyperplans vaguement fermés d’équation $\mu(f) = 0$, où $f$ parcourt l’ensemble des fonctions de $\mathcal{K}(X; \mathbf{C})$ dont le support ne rencontre pas $F$.

Supposons $X$ non compact : étant donné un filtre $\Phi$ sur l’espace $\mathcal{M}(X; \mathbf{C})$ des mesures sur $X$, nous dirons que le support d’une mesure $\mu$ s’éloigne indéfiniment suivant $\Phi$ si, pour toute partie compacte $K$ de $X$, il existe un ensemble $M \in \Phi$ tel que, pour toute mesure $\mu \in M$, on ait $\operatorname{Supp}(\mu) \cap K = \emptyset$.

#### Proposition 7 {#int-iii-s2-prop-7 .statement}

Si $\Phi$ est un filtre sur $\mathcal{M}(X; \mathbf{C})$ tel que le support de $\mu$ s’éloigne indéfiniment suivant $\Phi$, $\mu$ converge vaguement vers 0 suivant $\Phi$.

En effet, soit $f$ une fonction quelconque de $\mathcal{K}(X; \mathbf{C})$, et soit $K$ son support. Par hypothèse, il existe un ensemble $M \in \Phi$ tel que pour toute mesure $\mu \in M$, $\operatorname{Supp}(\mu) \cap K = \emptyset$; on a par suite $\mu(f) = 0$ pour toute $\mu \in M$, ce qui démontre la proposition.

### 3. Caractérisation du support d’une mesure

Par définition, si le support d’une fonction $f \in \mathcal{K}(X; \mathbf{C})$ ne rencontre pas le support d’une mesure $\mu$, on a $\mu(f) = 0$; mais on a la propriété plus précise suivante:

#### Proposition 8 {#int-iii-s2-prop-8 .statement}

Soit $\mu$ une mesure sur un espace localement compact $X$. Pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$ qui est nulle dans $\operatorname{Supp}(\mu)$, on a $\mu(f) = 0$.

Posons $K = \operatorname{Supp}(f)$, $S = \operatorname{Supp}(\mu)$. Etant donné un nombre $\varepsilon > 0$, soit $V$ l’ensemble des $x \in X$ tels que $|f(x)| < \varepsilon$; $V$ est un ensemble ouvert contenant $S$ par hypothèse ; donc $\mathbf{C} S$ est un voisinage de l’ensemble compact $\mathbf{C} V$. Il existe par suite une application continue $h$ de $X$ dans $[0, 1]$, égale à 1 dans $\mathbf{C} V$ et dont le support est contenu dans $\mathbf{C} S$ (§ 1, n° 2, lemme 1). Comme le support de $fh$ ne rencontre pas $S$, on a $\mu(fh) = 0$. D’autre part, on a $f = fh$ dans $K \cap \mathbf{C} V$, et $|fh| \leq |f|$ dans $X$, donc $|f - fh| \leq 2\varepsilon$ dans $X$, d’après le choix de $V$. Remarquons enfin qu’il existe un nombre $M_K$ tel que $|\mu(g)| \leq M_K \|g\|$ pour toute fonction $g \in \mathcal{K}(X; \mathbf{C})$ dont le support est contenu dans $K$; comme le support de $f - fh$ est contenu dans $K$, on a
$$
|\mu(f - fh)| \leq 2M_K \varepsilon,
$$
et par suite $|\mu(f)| = |\mu(f - fh)| \leq 2M_K \varepsilon$; comme $\varepsilon$ est arbitraire, on a $\mu(f) = 0$.

#### Corollaire 1 {#int-iii-s2-prop-8-cor-1 .statement}

*Si deux fonctions $f, g$ de $\mathcal{K}(X; \mathbf{C})$ sont égales dans $\mathrm{Supp}\ (\mu)$, on a $\mu(f) = \mu(g)$.*

#### Corollaire 2 {#int-iii-s2-prop-8-cor-2 .statement}

*Soit $\mu$ une mesure positive sur $X$; si
$$
f \in \mathcal{K}(X; \mathbf{C})
$$
est telle que $f(x) \geq 0$ dans $\mathrm{Supp}\ (\mu)$, on a $\mu(f) \geq 0$.
En effet, on a $f = |f|$ dans $S$, donc $\mu(f) = \mu(|f|) \geq 0$ par le cor. 1.*

#### Corollaire 3 {#int-iii-s2-prop-8-cor-3 .statement}

*Soit $\mu$ une mesure bornée sur $X$; si $f \in \mathcal{K}(X; \mathbf{C})$ est telle que $|f(x)| \leq a$ dans $\mathrm{Supp}\ (\mu)$, on a $|\mu(f)| \leq a \|\mu\|$.
En effet, on a $\mathrm{Supp}\ (|\mu|) = \mathrm{Supp}\ (\mu)$, et si $h$ est une application continue de $X$ dans $\{0, 1\}$ égale à 1 dans $\mathrm{Supp}\ (f)$ et à support compact, on a $|f(x)| \leq ah(x)$ dans $\mathrm{Supp}\ (\mu)$, donc
$$
|\mu|(|f|) \leq a|\mu|(h) \leq a\|\mu\|
$$
en vertu du cor. 2; la conclusion résulte alors de la formule (13) du n° 6.*

#### Proposition 9 {#int-iii-s2-prop-9 .statement}

*Soit $\mu$ une mesure positive sur $X$; si $f$ est une fonction de $\mathcal{K}_+(X)$ telle que $\mu(f) = 0$, $f$ est nulle dans $\mathrm{Supp}\ (\mu)$.
Soit $x$ un point de $X$ tel que $f(x) > 0$; montrons que $x$ n’appartient pas à $\mathrm{Supp}(\mu)$. En effet, il existe alors un voisinage compact $V$ de $x$ et un nombre $a > 0$ tels que $f(y) \geq a$ dans $V$. Soit alors $g$ une fonction continue $\geq 0$ à support dans $V$, et montrons que $\mu(g) = 0$; en effet, si l’on pose $b = \|g\|$, on a $g \leq bf/a$, d’où $\mu(g) \leq b\mu(f)/a = 0$.*

#### Proposition 10 {#int-iii-s2-prop-10 .statement}

*Soit $\mu$ une mesure sur un espace localement compact $X$; pour toute fonction $g \in \mathcal{C}(X; \mathbf{C})$, le support de la mesure $g.\mu$ est l’adhérence $T$ de l’ensemble des points $x \in \mathrm{Supp}\ (\mu)$ tels que $g(x) \neq 0$.*

En effet, posons $S = \operatorname{Supp}(\mu)$; soit $x_0$ un point n’appartenant pas à $T$; il existe un voisinage ouvert $V$ de $x_0$ tel qu’en tout point de $V \cap S$, $g$ soit nulle ; si $f \in \mathcal{K}(X; \mathbf{C})$ a son support dans $V$, $fg$ est nulle dans $S$, donc (prop. 8) $\mu(gf) = 0$; autrement dit, la restriction de $g.\mu$ à $V$ est nulle.

Inversement, supposons que la restriction de $g.\mu$ à un voisinage ouvert $W$ d’un point $x_0 \in X$ soit nulle, et montrons qu’il n’existe aucun point de $W \cap S$ où $g$ soit $\neq 0$. En effet, s’il existait un tel point $y$, il existerait un voisinage compact $U$ de $y$, contenu dans $W$, et en tout point $x$ duquel on aurait $g(x) \neq 0$; mais alors toute fonction $f \in \mathcal{K}(X; \mathbf{C})$, dont le support est contenu dans $U$, peut s’écrire $f = gh$, où $h \in \mathcal{K}(X; \mathbf{C})$ a son support dans $U \subset W$; on aurait par suite $\mu(f) = \mu(gh) = 0$, contrairement à l’hypothèse $y \in S$.

On notera que $T$ est contenu dans l’intersection du support $S$ de $\mu$ et du support de $g$, sans être nécessairement égal à cette intersection. Par exemple, si $X = \mathbf{R}$, si $\mu$ est la mesure de Dirac au point 0 et si $g(x) = x$, on a $g.\mu = 0$ bien que l’intersection des supports de $g$ et de $\mu$ soit réduite au point 0, donc non vide.

#### Corollaire {#int-iii-s2-n3-cor-1 .statement}

Pour que la mesure $g.\mu$ soit nulle, il faut et il suffit que $g$ soit nulle dans le support de $\mu$.

#### Proposition 11 {#int-iii-s2-prop-11 .statement}

Toute mesure à support compact est bornée.

En effet, $|\mu|$ est aussi une mesure à support compact, donc on peut se borner au cas où $\mu \geqslant 0$; si $h$ est une application continue de $X$ dans $\{0, 1\}$, à support compact, égale à 1 dans $\operatorname{Supp}(\mu)$, on a, pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$, $|f(x)| \leq \|f\| h(x)$ dans $\operatorname{Supp}(\mu)$, donc (cor. 2 de la prop. 8) $\mu(|f|) \leq \mu(h)\|f\|$, ce qui prouve la proposition (§ 1, n° 8).

### 4. Mesures ponctuelles. Mesures à support fini

#### Proposition 12 {#int-iii-s2-prop-12 .statement}

Soient $a_i$ ($1 \leq i \leq n$) des points distincts dans un espace localement compact $X$. Toute mesure sur $X$ dont le support est contenu dans l’ensemble des $a_i$ est une combinaison linéaire des mesures $\varepsilon_{a_i}$ ($1 \leq i \leq n$).

En effet, une telle mesure $\mu$ est nulle pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$ satisfaisant aux $n$ relations $f(a_i) = 0$ (n° 3, prop. 8); comme ces relations s’écrivent $\varepsilon_{a_i}(f) = 0$, $\mu$ est combinaison linéaire des $\varepsilon_{a_i}$ (Alg., chap. II, 3e éd., § 7, n° 5, cor. 1 du th. 7).

En particulier, toute mesure dont le support est vide ou réduit à un seul point x est de la forme $\alpha \varepsilon_x$, où $\alpha$ est un nombre complexe; on dit qu’une telle mesure est une mesure ponctuelle; toute mesure dont le support est fini est donc une somme de mesures ponctuelles.

#### Théorème 1 {#int-iii-s2-thm-1 .statement}

Toute mesure $\mu$ sur un espace localement compact $X$ est vaguement adhérente à l’espace vectoriel $V$ des mesures dont le support est fini et contenu dans $\mathrm{Supp}(\mu)$.

Il suffit de prouver que $\mu$ est orthogonale au sous-espace $V^o$ de $\mathcal{K}(X; \mathbf{C})$ orthogonal à $V$ (Esp. vect. top., chap. II, 2e éd., § 6, n° 3, cor. 2 du th. 1), c’est-à-dire que les relations $\langle f, \varepsilon_a \rangle = 0$, où $a$ parcourt le support de $\mu$, entraînent $\langle f, \mu \rangle = 0$; mais cela n’est autre que la prop. 8 du n° 3.

#### Corollaire 1 {#int-iii-s2-thm-1-cor-1 .statement}

Toute mesure bornée $\mu$ sur $X$ est vaguement adhérente à l’ensemble convexe $A$ des mesures dont le support est fini et contenu dans celui de $\mu$, et dont la norme est $\leq \| \mu \|$. En outre, si $v$ tend vaguement vers $\mu$ en restant dans $A$, $\| v \|$ tend vers $\| \mu \|$.

Pour prouver la première assertion, il suffit d’établir que la mesure $\mu$ appartient à l’ensemble polaire de l’ensemble $A^o$, polaire de $A$ dans $\mathcal{K}(X; \mathbf{C})$ (Esp. vect. top, chap. II, 2e éd., § 6, n° 3, th. 1); cela signifie que, pour $f \in \mathcal{K}(X; \mathbf{C})$, les relations $| \langle f, \varepsilon_a \rangle | \leq 1 / \| \mu \|$ pour tout $a \in \mathrm{Supp}(\mu)$, entraînent $| \langle f, \mu \rangle | \leq 1$; or, c’est là une conséquence du cor. 3 de la prop. 8 du n° 3.

Pour prouver la seconde assertion, notons que l’on a
$$
\liminf_{v \to \mu, v \in A} \| v \| \geq \| \mu \|
$$
puisque la fonction $v \mapsto \| v \|$ est semi-continue inférieurement pour la topologie vague (§ 1, n° 9, cor. 4 de la prop. 15), et la conclusion résulte de ce que $\| v \| \leq \| \mu \|$ pour $v \in A$ par définition.

#### Corollaire 2 {#int-iii-s2-thm-1-cor-2 .statement}

Toute mesure bornée $\mu$ sur $X$ est vaguement adhérente à l’ensemble des mesures dont le support est fini et contenu dans celui de $\mu$ et dont la norme est égale à $\| \mu \|$.

On peut supposer $\mu \neq 0$. Soit $V$ un voisinage ouvert de 0 pour la topologie vague; pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, il existe, en vertu du cor. 1, une mesure $v_0$ dont le support est fini et contenu dans $\mathrm{Supp}(\mu)$ et qui est telle que $v_0 - \mu \in V$, et que

$$
\|\mu\| \geq \|v_0\| \geq (1 - \varepsilon)\|\mu\|. \text{ Si l'on pose } v = (\|\mu\|/\|v_0\|)v_0, \text{ on a } \|v\| = \|\mu\|, \text{ et } \|v - v_0\| \leq \|\mu\|; \text{ dès que } \varepsilon \text{ est assez petit, on a donc } v - \mu \in V + V, \text{ d'où la conclusion.}
$$

#### Corollaire 3 {#int-iii-s2-thm-1-cor-3 .statement}

*Toute mesure bornée positive* $\mu$ *sur* $X$ *est vaguement adhérente à l’ensemble convexe des mesures positives dont le support est fini et contenu dans celui de* $\mu$, *et dont la norme est égale à* $\|\mu\|$.

Le même raisonnement que dans le cor. 2 montre qu’on peut se borner à prouver que $\mu$ est vaguement adhérente à l’ensemble convexe $B$ formé des mesures positives de support fini contenu dans $\mathrm{Supp}(\mu)$ et de norme $\leq \|\mu\|$. Il suffit encore d’établir que $\mu$ appartient à l’ensemble polaire de l’ensemble $B^0$, polaire de $B$ *dans* $\mathcal{K}(X; \mathbf{R})$ (*Esp. vect. top.*, chap. II, 2e éd., § 6, n° 3, th. 1); mais cela signifie que pour $f \in \mathcal{K}(X; \mathbf{R})$ les relations $\langle f, \varepsilon_a \rangle \leq 1/\|\mu\|$ pour tout $a \in \mathrm{Supp}(\mu)$ entraînent $\langle f, \mu \rangle \leq 1$, ce qui est une conséquence du n° 3, cor. 2 de la prop. 8.

#### Corollaire 4 {#int-iii-s2-thm-1-cor-4 .statement}

*Dans l’espace* $\mathcal{M}(X; \mathbf{C})$, *l’ensemble des mesures ponctuelles est total pour la topologie de la convergence strictement compacte* (§ 1, n° 10).

En effet, sur le cône $\mathcal{M}_+(X)$, la topologie de la convergence strictement compacte est identique à la topologie vague (§ 1, n° 10, prop. 18), et toute mesure sur $X$ s’écrit $\mu_1 - \mu_2 + i\mu_3 - i\mu_4$, où les $\mu_j$ ($1 \leq j \leq 4$) sont des mesures positives; la conclusion résulte donc du th. 1.

#### Proposition 13 {#int-iii-s2-prop-13 .statement}

*Soit* $\mu$ *une mesure sur un espace localement compact* $X$. *Pour qu’un point* $x_0$ *appartienne à* $\mathrm{Supp}(\mu)$, *il faut et il suffit que la mesure ponctuelle* $\varepsilon_{x_0}$ *soit vaguement adhérente à l’ensemble des mesures* $g.\mu$, *où* $g$ *parcourt l’ensemble des fonctions continues à support compact telles que* $\|g.\mu\| \leq 1$.

La condition est évidemment suffisante en vertu de la prop. 6 du n° 2. Pour voir qu’elle est nécessaire, supposons $x_0 \in \mathrm{Supp}(\mu)$; considérons un nombre fini de fonctions $f_k$ ($1 \leq k \leq n$) de $\mathcal{K}(X; \mathbf{C})$, et un nombre arbitraire $\delta > 0$; il s’agit de prouver qu’il existe une fonction $g \in \mathcal{K}(X; \mathbf{C})$ telle que $\|g.\mu\| \leq 1$ et que l’on ait

$$
|f_k(x_0) - \mu(gf_k)| \leq \delta
$$

pour $1 \leq k \leq n$. Soit U un voisinage ouvert relativement compact de $x_0$ tel que l’oscillation de chacune des $f_k$ ($1 \leq k \leq n$) dans U soit $\leq \delta/2$. Par hypothèse, comme $x_0 \in \mathrm{Supp}\ (\mu)$, il existe une fonction $g_0 \in \mathcal{K}(X; \mathbf{C})$ dont le support est contenu dans U et qui est telle que $\mu(g_0) \neq 0$; la mesure $\nu = g_0 \cdot \mu$ n’est pas nulle, car pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$ égale à 1 dans U, on a $\nu(f) = \mu(g_0) \neq 0$. En outre, $\nu$ est bornée (n° 3, prop. 11); en multipliant $g_0$ par un scalaire, on peut supposer que $\| \nu \| = 1$. Cela étant, en posant $\alpha_k = f_k(x_0)$, on peut écrire, pour $1 \leq k \leq n$ et pour toute fonction $h \in \mathcal{K}(X; \mathbf{C})$

$$
f_k(x_0) - \nu(f_k h) = \alpha_k (1 - \nu(h)) + \nu((\alpha_k - f_k) h).
$$

Comme $\nu$ a son support dans U, on peut l’identifier à sa restriction à U; l’hypothèse $\| \nu \| = 1$ entraîne alors qu’il existe une fonction $h \in \mathcal{K}(X; \mathbf{C})$, de support contenu dans U, telle que $\| h \| \leq 1$ et que l’on ait $|\alpha_k (1 - \nu(h))| \leq \delta/2$ pour $1 \leq k \leq n$. La définition de U montre par ailleurs que $|(\alpha_k - f_k(x)) h(x)| \leq \delta/2$ pour tout $x \in U$; comme $\| \nu \| = 1$ et que $\mathrm{Supp}(\nu) \subset U$, on a donc $|\nu((\alpha_k - f_k) h)| \leq \delta/2$, et par suite, en posant $g = g_0 h$,

$$
|f_k(x_0) - \mu(g f_k)| \leq \delta \quad \text{pour} \quad 1 \leq k \leq n.
$$

Cela démontre la proposition, puisque

$$
\| g \cdot \mu \| = \| (g_0 h) \cdot \mu \| \leq \| g_0 \cdot \mu \| = 1.
$$

#### Corollaire {#int-iii-s2-n4-cor-1 .statement}

Soit $\mu$ une mesure sur X. Pour qu’une mesure $\nu$ sur X soit vaguement adhérente à l’ensemble des mesures $g \cdot \mu$, où $g$ parcourt $\mathcal{K}(X; \mathbf{C})$, il faut et il suffit que $\mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu)$.

En effet, $\mathrm{Supp}(g \cdot \mu) \subset \mathrm{Supp}(\mu)$ en vertu du n° 3, prop. 10; le support de toute limite vague de mesures de la forme $g \cdot \mu$ est donc aussi contenu dans $\mathrm{Supp}(\mu)$ (n° 2, prop. 6). Inversement, si $\mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu)$, $\nu$ est limite vague de mesures de support fini contenu dans $\mathrm{Supp}(\mu)$ (th. 1), donc est vaguement adhérente à l’ensemble des mesures $g \cdot \mu$ d’après la prop. 13.

### 5. Mesures discrètes

#### Proposition 14 {#int-iii-s2-prop-14 .statement}

Pour qu’une mesure $\mu$ sur un espace localement compact X soit une mesure discrète (§ 1, n° 3, Exemple 1), il faut et il suffit que $\mathrm{Supp}(\mu)$ soit un sous-espace fermé discret de X.

Soit $\mu$ une mesure discrète sur X, définie par les masses $h(x) \neq 0$ placées aux points $x$ d’un sous-espace fermé discret N de X; montrons que $\mathrm{Supp}(\mu) = N$. En effet, pour tout $a \in \mathbf{N}$ et tout voisinage V de $a$, il existe une fonction $f \in \mathcal{K}(X; \mathbf{C})$ de support contenu dans V, égale à 1 au point $a$ et à 0 aux autres points de $N$; d’où $\mu(f) = h(a) \neq 0$. Au contraire, si $b \notin N$, il existe un voisinage W de $b$ ne rencontrant pas $N$; pour toute fonction $g \in \mathcal{K}(X; \mathbf{C})$ à support contenu dans $N$, on a donc $\mu(g) = 0$, ce qui prouve que $b \notin \mathrm{Supp}(\mu)$.

Inversement, soit $\mu$ une mesure telle que $\mathrm{Supp}(\mu)$ soit un sous-espace fermé discret $N$ de $X$. Pour tout $a \in N$, il existe un voisinage ouvert $V_a$ de $a$ ne contenant aucun point de $N$ distinct de $a$; la restriction de $\mu$ à $V_a$ est donc une mesure ponctuelle de support $\{a\}$ (n° 2, prop. 5), et par suite (n° 4, prop. 12) de la forme $h(a)\varepsilon_a$, où $h(a) \neq 0$. Si l’on pose $h(x) = 0$ aux points de $\mathbf{C}N$, et si l’on désigne par $\nu$ la mesure définie par les masses $h(x)$, le principe de localisation montre que $\nu = \mu$.

On voit ainsi que sur un espace discret $X$, toute mesure est discrète.

## EXERCICES {#int-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
