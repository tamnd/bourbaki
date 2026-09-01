---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 4
section_title: Convolution des mesures et des fonctions
lang: fr
source: int-vii-viii-fr
pdf_pages: 0147-0173
extraction: ocr
subsections:
    - "no": 1
      title: Convolution d'une mesure et d'une fonction.
      page: 0
      pdf_page: 147
    - "no": 2
      title: Exemples de mesures et de fonctions convolables.
      page: 0
      pdf_page: 151
    - "no": 3
      title: '**Convolution et transposition.**'
      page: 0
      pdf_page: 158
    - "no": 4
      title: Convolution d'une mesure et d'une fonction sur un groupe
      page: 0
      pdf_page: 162
    - "no": 5
      title: '**Convolution des fonctions sur un groupe.**'
      page: 0
      pdf_page: 163
    - "no": 6
      title: Applications.
      page: 0
      pdf_page: 168
    - "no": 7
      title: Régularisation.
      page: 0
      pdf_page: 170
statements: 42
exercises: 0
content_sha256: e56f96411e4d7f56886ab6e944a3ea703e0922e4f1ba9d99a6018dfb797489f9
---

## § 4. Convolution des mesures et des fonctions.

### 1. Convolution d'une mesure et d'une fonction.

Soit $X$ un espace localement compact sur lequel un groupe localement compact $G$ opère à gauche continûment. Soit $\beta$ une mesure positive sur $X$, quasi-invariante par $G$. Soit $\chi$ une fonction $> 0$ sur $G \times X$, mesurable pour toute mesure sur $G \times X$, et telle que, pour tout $s \in G$, $\chi(s^{-1}, .)$ soit une densité de $\gamma(s)\beta$ par rapport à $\beta$:

(1)
$$
\gamma(s)\beta = \chi(s^{-1}, .)\cdot \beta,
$$
ce qu'on peut écrire, avec les conventions du chap. VII, § 1, n° 1 :

(1')
$$
d\beta(sx) = \chi(s, x)d\beta(x).
$$

Ces données resteront fixées dans les n°s 1, 2 et 3 (exception faite de la Remarque 2 du n° 2).

Rappelons (§ 2, n° 5) que, si $\chi$ est continue et si $\beta$ est de support $X$, $\chi$ est alors un multiplicateur.

Soit $f$ une fonction complexe localement $\beta$-intégrable sur $X$, et soit $\mu$ une mesure sur $G$. Pour tout $s \in G$, la mesure $\gamma(s)(f.\beta)$ est de base $\beta$ puisque $\beta$ est quasi-invariante. Donc, si $\mu$ et $f.\beta$ sont convolables, $\mu * (f.\beta)$ est de base $\beta$ (§ 3, n° 2, prop. 10).

#### Définition 1 {#int-viii-s4-def-1 .statement}

Si $\mu$ et $f.\beta$ sont convolables, on dit que $\mu$ et $f$ sont convolables relativement à $\beta$. Toute densité de $\mu * (f.\beta)$ par rapport à $\beta$ s'appelle un produit de convolution de $\mu$ et $f$ relativement à $\beta$ et se note $\mu *_{\beta} f$.

On omet $\beta$ quand aucune confusion n'est possible. On définit de manière analogue la convolution pour plusieurs mesures sur $G$ et une fonction sur $X$.

Les différents produits de convolution de $\mu$ et $f$ sont égaux localement $\beta$-presque partout. Si $\beta$ est de support $X$ et s'il existe un produit de convolution de $\mu$ et $\beta$ qui soit continu, ce dernier est déterminé de manière unique ; c'est lui qu'on appelle alors le produit de convolution de $\mu$ et $f$ relativement à $\beta$.

Soit $s \in G$ et soit $f$ une fonction complexe localement $\beta$-intégrable sur $X$. Alors $\varepsilon_s$ et $f$ sont convolables, et on a

$$
\varepsilon_s * (f.\beta) = \gamma(s)(f.\beta) = (\gamma(s)f) \cdot (\gamma(s)\beta) = (\gamma(s)f) \cdot \chi(s^{-1}, .) \cdot \beta
$$

donc

(2)
$$
(\varepsilon_s * f)(x) = \chi(s^{-1}, x)f(s^{-1}x) = (\gamma_x(s)f)(x)
$$

localement $\beta$-presque partout.

#### Lemme 1 {#int-viii-s4-lem-1 .statement}

Soit $\mu$ une mesure sur $G$. Alors $\chi$ est localement $(\mu \otimes \beta)$-intégrable, et l'image de $\mu \otimes \beta$ par l'homéomorphisme $(s, x) \to (s, s^{-1}x)$ de $G \times X$ sur $G \times X$ est $\chi \cdot (\mu \otimes \beta)$.

On peut supposer $\mu \geqslant 0$. Soit $F \in \mathcal{H}_+(G \times X)$. On a

$$
\int F(s, s^{-1}x)d\mu(s)d\beta(x) = \int d\mu(s) \int F(s, s^{-1}x)d\beta(x)
$$
$$
= \int d\mu(s) \int F(s, x)d(\gamma(s^{-1})\beta)(x) = \int d\mu(s) \int F(s, x)\chi(s, x)d\beta(x).
$$

Or, la fonction $(s, x) \to F(s, x)\chi(s, x)$ est à support compact et $(\mu \otimes \beta)$-mesurable. D’après le chap. V, § 8, n° 1, prop. 4, l’égalité précédente prouve que cette fonction est $(\mu \otimes \beta)$-intégrable et que

$$
\int F(s, s^{-1}x)d\mu(s)d\beta(x) = \int F(s, x)\chi(s, x)d\mu(s)d\beta(x).
$$

Ceci prouve à la fois les deux assertions du lemme 1.

#### Proposition 1 {#int-viii-s4-prop-1 .statement}

*Soient $\mu$ une mesure sur $G$, $f$ une fonction complexe localement $\beta$-intégrable sur $X$. Supposons que la fonction $s \to f(s^{-1}x)\chi(s^{-1}, x)$ soit essentiellement $\mu$-intégrable sauf pour un ensemble localement $\beta$-négligeable de valeurs de $x$, et que la fonction $x \to \int |f(s^{-1}x)|\chi(s^{-1}, x)d|\mu|(s)$, définie localement presque partout pour $\beta$, soit localement $\beta$-intégrable. Alors $\mu$ et $f$ sont convolables.*

On peut supposer $f \geqslant 0$ et $\mu \geqslant 0$. Soit $h \in \mathcal{K}_+(X)$. Il s’agit de prouver que la fonction $(s, x) \to h(sx)$ est essentiellement intégrable pour $\mu \otimes (f.\beta) = (1 \otimes f).(\mu \otimes \beta)$ (chap. V, § 8, n° 3, prop. 6), c’est-à-dire que $\int^* h(sx)f(x)d\mu(s)d\beta(x) < +\infty$ (chap. V, § 5, n° 3, prop. 2); il suffira évidemment de prouver qu’il existe $a > 0$ tel que pour toute partie compacte $K$ de $G$, on ait

$$
\int^* h(sx)f(x)\varphi_K(s)d\mu(s)d\beta(x) \leqslant a.
$$

D’après le lemme 1,

$$
\int^* h(sx)f(x)\varphi_K(s)d\mu(s)d\beta(x)
= \int^* h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x)d\mu(s)d\beta(x).
$$

Or la fonction $(s, x) \to h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x)$ est $(\mu \otimes \beta)$-mesurable (lemme 1) et à support compact. L’expression précédente est donc égale (chap. V, § 8, n° 1, prop. 4) à

$$
\int^* h(x) d\beta(x) \int^* f(s^{-1}x) \varphi_K(s) \chi(s^{-1}, x) d\mu(s)
$$
$$
\leq (\sup h) \int_S^* d\beta(x) \int^* f(s^{-1}x) \chi(s^{-1}, x) d\mu(s)
$$
en désignant par S le support de h. D'où la proposition.

#### Proposition 2 {#int-viii-s4-prop-2 .statement}

Soient $\mu$ une mesure sur G, $f$ une fonction complexe localement $\beta$-intégrable sur X. On suppose vérifiée l'une des conditions suivantes :
(i) $f$ et $\chi$ sont continues ;
(ii) G opère proprement dans X et $f$ est nulle dans le complémentaire d'une réunion dénombrable d'ensembles compacts ;
(iii) $\mu$ est portée par une réunion dénombrable d'ensembles compacts.

Si $\mu$ et $f$ sont convolables, la fonction $s \to f(s^{-1}x) \chi(s^{-1}, x)$ est essentiellement $\mu$-intégrable sauf pour un ensemble localement $\beta$-négligeable de valeurs de $x$, et l'on a localement $\beta$-presque partout

(3) $$(\mu *^\beta f)(x) = \int_G f(s^{-1}x) \chi(s^{-1}, x) d\mu(s) = \int_G (\gamma^\chi(s)f)(x) d\mu(s).$$

Soit $h \in \mathcal{H}(X)$. Puisque $\mu$ et $f$ sont convolables, la fonction $(s, x) \to h(sx)f(x)$ est essentiellement $(\mu \otimes \beta)$-intégrable. D'après le lemme 1, la fonction $(s, x) \to h(x)f(s^{-1}x) \chi(s^{-1}, x)$ est essentiellement $(\mu \otimes \beta)$-intégrable. Sous les hypothèses (i) ou (ii) de l'énoncé, on en déduit que cette fonction est $(\mu \otimes \beta)$-intégrable ; car, dans le premier cas, elle est continue et on applique la prop. 2 du chap. V, § 2, no 1, et dans le second cas, elle est nulle hors d'une réunion dénombrable d'ensembles compacts, et on applique la prop. 3, loc. cit. D'après le théorème de Lebesgue-Fubini,

$$
\int h(sx) d\mu(s) d(f.\beta)(x) = \int h(x) f(s^{-1}x) \chi(s^{-1}, x) d\mu(s) d\beta(x)
$$
$$
= \int h(x) d\beta(x) \int f(s^{-1}x) \chi(s^{-1}, x) d\mu(s),
$$

la fonction $x \to g(x) = \int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s)$ étant en outre localement $\beta$-intégrable. On voit donc que

$$
\langle h, \mu * (f.\beta) \rangle = \langle h, g.\beta \rangle
$$

d'où $g = \mu *^\beta f$.

Supposons maintenant $\mu$ portée par la réunion S d'une suite d'ensembles compacts. La fonction

$$
(s, x) \to h(x)f(s^{-1}x)\chi(s^{-1}, x)\varphi_S(s)
$$

est essentiellement $(\mu \otimes \beta)$-intégrable, et nulle hors d'une réunion dénombrable d'ensembles compacts, donc $(\mu \otimes \beta)$-intégrable. Comme $\mu = \varphi_S.\mu$, le raisonnement se termine comme précédemment.

#### Remarque {#int-viii-s4-n1-rem-1 .statement}

L'hypothèse (iii) de la prop. 2 est satisfaite notamment quand $\mu$ est bornée. En effet, pour tout $n > 0$, il existe alors une partie compacte $K_n$ de G telle que

$$
|\mu|(G - K_n) \leq \frac{1}{n}
$$

(chap. IV, § 4, no 7), et $\mu$ est portée par la réunion des $K_n$. Plus généralement, soit $\rho$ une fonction semi-continue inférieurement finie $> 0$ sur G telle que $\rho(st) \leq \rho(s)\rho(t)$; si $\mu \in \mathcal{M}^\circ$, l'hypothèse (iii) est satisfaite; car $\rho.\mu$ est bornée, et $\mu$ est portée par les mêmes sous-ensembles que $\rho.\mu$ puisque, sur toute partie compacte de G, $\rho$ est minorée par une constante $> 0$.

### 2. Exemples de mesures et de fonctions convolables.

Dans les prop. 3 et 4, $\mathcal{C}'(G)$ et $\mathcal{M}(G)$ sont munis de la topologie de la convergence compacte dans $\mathcal{C}(G)$ et $\mathcal{K}(G)$ respectivement.

#### Proposition 3 {#int-viii-s4-prop-3 .statement}

Supposons $\chi$ continue. Soient $\mu \in \mathcal{C}'(G)$ et $f \in \mathcal{C}(X)$. Alors :

(i) $\mu$ et $f$ sont convolables relativement à $\beta$.

(ii) La formule (3) du n° 1 définit pour tout $x \in X$ un produit de convolution $\mu *_{\beta} f$ qui est continu et n’est autre que l’élément $\gamma_x(\mu)f$ défini par la représentation continue $\gamma_x$ de $G$ dans $C(X)$; de plus, l’application $(\mu, f) \to \mu *_{\beta} f$ est hypocontinue relativement aux parties équicontinues de $C'(G)$ et aux parties compactes de $C(X)$.

(iii) Si de plus $f \in \mathcal{K}(X)$ le produit $\mu *_{\beta} f$ de (ii) appartient à $\mathcal{K}(X)$ et l’application $(\mu, f) \to \mu *_{\beta} f$ est hypocontinue relativement aux parties équicontinues de $C'(G)$ et aux parties compactes de $\mathcal{K}(X)$.

On sait que $\mu$ et $f$ sont convolables (§ 3, n° 2, prop. 8 (i)). D’autre part, avec les notations du § 2, on a

$$
\gamma_x(\mu)f = \int (\gamma_x(s)f)d\mu(s) \in C(X)
$$

puisque $C(X)$ est quasi-complet. En particulier, pour tout $x \in X$, on a

$$
(\gamma_x(\mu)f)(x) = \int (\gamma_x(s)f)(x)d\mu(s).
$$

Ceci, joint à la prop. 2, et au § 2, n° 6, prouve (ii). Enfin, si $f \in \mathcal{K}(X)$, $\mu * (f.\beta)$ est à support compact (§ 3, n° 2, prop. 9), donc $\mu *_{\beta} f \in \mathcal{K}(X)$. Considérons la représentation continue $U$ de $G$ dans le complété $\mathcal{K}(X)^{\hat{}}$ obtenue en prolongeant par continuité les opérateurs $\gamma_x(s)$ continus dans $\mathcal{K}(X)$ (§ 2, n° 1, Remarque 3). Soit $S$ le support de $\mu$. Les fonctions $\gamma_x(s)f$, pour $s \in S$, ont leur support contenu dans un ensemble compact fixe $K$. L’ensemble $\mathcal{K}(X, K)$ est un sous-espace vectoriel complet de $\mathcal{K}(X)$. Donc $U(\mu)f \in \mathcal{K}(X)$. On voit alors comme précédemment que $U(\mu)f = \mu *_{\beta} f$, et (iii) résulte encore du § 2, n° 6.

#### Proposition 4 {#int-viii-s4-prop-4 .statement}

Supposons que $G$ opère proprement dans $X$ et que $\chi$ soit continue. Soient $\mu \in \mathcal{M}(G)$ et $f \in \mathcal{K}(X)$.

(i) $\mu$ et $f$ sont convolables relativement à $\beta$.

(ii) La formule (3) du n° 1 définit pour tout $x \in X$ un produit de convolution $\mu *_{\beta} f$ qui est continu.

(iii) L’application $(\mu, f) \to \mu *_{\beta} f$ de $\mathcal{M}(G) \times \mathcal{K}(X)$ dans $
\mathcal{C}(X)$ est hypocontinue relativement aux parties bornées de $M(G)$ et aux parties compactes de $\mathcal{K}(X)$ qui sont contenues dans un sous-espace $\mathcal{K}(X, L)$ (où $L$ est une partie compacte variable de $X$).

On sait que $\mu$ et $f$ sont convolables ($§ 3$, no 2, prop. 8 (ii)), et il est clair, que les intégrales figurant dans (3) existent pour tout $x \in X$. Soient $K$ et $L$ deux parties compactes de $X$. Il existe une partie compacte $H$ de $G$ telle que les relations $x \in K$ et $s^{-1}x \in L$ entraînent $s \in H$; soit $\varphi \in \mathcal{K}_+(G)$, telle que $\varphi(s) = 1$ pour $s \in H$. On a, pour $f \in \mathcal{K}(X, L)$ et $x \in K$ :

$$
\int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s) = \int f(s^{-1}x)\chi(s^{-1}, x)\varphi(s)d\mu(s) = ((\varphi \cdot \mu) *^\beta f)(x)
$$

Par suite $\int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s)$ est fonction continue de $x$ et définit un produit de convolution $\mu *^\beta f \in \mathcal{C}(X)$. De plus, l’application $\mu \to \varphi \cdot \mu$ de $M(G)$ dans $\mathcal{C}'(G)$ est continue pour les topologies de la convergence compacte. La prop. 3 (iii) entraîne donc que l’application $(\mu, f) \to \mu *^\beta f$ de $M(G) \times \mathcal{K}(X, L)$ dans $\mathcal{C}(X)$ est, pour toute partie compacte $L$ de $X$, hypocontinue relativement aux parties compactes de $\mathcal{K}(X, L)$. En particulier, l’application $(\mu, f) \to \mu *^\beta f$ de $M(G) \times \mathcal{K}(X)$ dans $\mathcal{C}(X)$ est séparément continue. Comme $\mathcal{K}(X)$ est tonnelé, cette application est hypocontinue relativement aux parties bornées de $M(G)$ (*Esp. vect. top.*, chap. III, § 4, no 2, prop. 6).

#### Remarque 1 {#int-viii-s4-n2-rem-1 .statement}

Sous les hypothèses de la prop. 4, l’application $\mu \to \mu *^\beta f$ de $M_+(G)$ dans $\mathcal{C}(X)$ est continue lorsqu’on munit $M_+(G)$ de la topologie *vague*, pour toute $f \in \mathcal{K}(X)$. En effet, soient $K$ une partie compacte de $X$, $S$ le support (compact) de $f$; comme $G$ opère proprement dans $X$, l’ensemble des $s \in G$ pour lesquels il existe $x \in K$ tel que $s^{-1}x \in S$ est une partie compacte $L$ de $G$ (*Top. gén.*, chap. III, 3e éd., § 4, no 5, th. 1). Soient $\varepsilon$ un nombre $> 0$, $\varphi$ une fonction de $\mathcal{K}_+(G)$ égale à 1 dans l’ensemble compact $L$, $\mu_0$ un élément de $M_+(G)$; l’ensemble $W_0$ des mesures $\mu \in M_+(G)$ telles que

$$
\left| \int \varphi(s)d\mu(s) - \int \varphi(s)d\mu_0(s) \right| \leq \varepsilon
$$

est un voisinage de $\mu_0$ dans $\mathcal{M}_+(G)$. D'autre part, la fonction $(s, x) \to f(s^{-1}x)\chi(s^{-1}, x)$ est uniformément continue dans $L \times K$, donc il existe un nombre fini de points $x_i \in K$ ($1 \leq i \leq n$) tels que pour tout $x \in K$, il existe un $i$ pour lequel on ait
$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_i)\chi(s^{-1}, x_i)| \leq \varepsilon
$$
pour tout $s \in L$. Comme $\mu(L) \leq \int \varphi(s)d\mu_0(s) + \varepsilon$ pour toute $\mu \in W_0$, on a aussi
$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)d\mu(s) \right| \leq
$$
$$
\leq \varepsilon \left( \int \varphi(s)d\mu_0(s) + \varepsilon \right)
$$
pour tout $x$ vérifiant l'inégalité précédente et toute $\mu \in W_0$. Soit alors $W$ le voisinage de $\mu_0$ dans $\mathcal{M}_+(G)$ formé des mesures $\mu \in W_0$ telles que
$$
\left| \int f(s^{-1}x_i)\chi(s^{-1}, x_i)d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)d\mu_0(s) \right| \leq \varepsilon
$$
pour $1 \leq i \leq n$. Il est clair que pour toute mesure $\mu \in W$ et tout $x \in K$, on a
$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s) - \int f(s^{-1}x)\chi(s^{-1}, x)d\mu_0(s) \right| \leq
$$
$$
\leq \varepsilon \left( 2 \int \varphi(s)d\mu_0(s) + 2\varepsilon + 1 \right)
$$
et comme $\varepsilon$ est arbitraire, cela démontre notre assertion.

#### Proposition 5 {#int-viii-s4-prop-5 .statement}

*Supposons $\chi$ continue et chaque fonction $\chi(s, .)$ bornée.*
(i) *La fonction $s \to \rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$ sur $G$ est semi-continue inférieurement $> 0$ et vérifie $\rho(st) \leq \rho(s)\rho(t)$ quels que soient $s, t$ dans $G$.*
(ii) *Soient $\mu \in \mathcal{M}^\circ(G)$ et $f \in L^\infty(X, \beta)$. Alors $\mu$ et $f$ sont* convolables et $\mu *_{\beta} f$ est donné localement presque partout par la formule (3) du n° 1. On a $\mu *_{\beta} f \in L^{\infty}(X, \beta)$, et $\| \mu *_{\beta} f \|_{\infty} \leq \| \mu \|_{\rho} \| f \|_{\infty}$.

(iii) Si de plus $f \in \mathcal{C}^{\infty}(X)$ (resp. $\mathcal{K}(X)$), la formule (3) du n° 1 définit pour tout $x$ un produit de convolution $\mu *_{\beta} f$ qui appartient à $\mathcal{C}^{\infty}(X)$ (resp. $\mathcal{K}(X)$).

(iv) Si $f \in \mathcal{K}(X)$, alors le produit de convolution $\mu *_{\beta} f$ défini par (3) n’est autre que l’élément $\gamma_{x}(\mu)f$ défini par la représentation continue $\gamma_{x}$ de $G$ dans $\mathcal{K}(X)$.

L’identité $\chi(st, x) = \chi(s, tx)\chi(t, x)$ entraîne aussitôt que $\rho(st) \leq \rho(s)\rho(t)$. D’autre part, $\rho$ est semi-continue inférieurement comme enveloppe supérieure de fonctions continues.

Soit $\mu \in \mathcal{M}^{o}(G)$. D’après la prop. 1 du n° 1, $\mu$ et 1 sont convolables ; la prop. 2 montre que $(|\mu| *_{\beta} 1)(x) \leq \int_{G} \rho(s)d|\mu|(s)$ localement $\beta$-presque partout. Donc, si $f$ est $\beta$-mesurable et si $|f| \leq 1$, $\mu$ et $f$ sont convolables et $N_{\infty}(\mu *_{\beta} f) \leq \int \rho(s)d|\mu|(s)$.

De plus, $\mu *_{\beta} f$ est donné localement presque partout par la formule (3) du n° 1, car la condition (iii) de la prop. 2 du n° 1 est satisfaite. Ceci entraîne (ii).

Supposons $f$ continue et bornée par 1 en valeur absolue. Il est clair que les intégrales figurant dans (3) existent pour tout $x \in X$. Montrons qu’elles dépendent continûment de $x$. On peut supposer $\mu \geq 0$. Soient $x_{0} \in X$ et $\varepsilon > 0$. Soit $K$ une partie compacte de $G$ telle que $\int_{G-K} \rho(s)d\mu(s) \leq \varepsilon$. Il existe un voisinage $V$ de $x_{0}$ dans $X$ tel que $x \in V$ implique

$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_{0})\chi(s^{-1}, x_{0})| \leq \varepsilon / \mu(K)
$$

pour $s \in K$. Alors, pour $x \in V$, on a

$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x)d\mu(s) - \int f(s^{-1}x_{0})\chi(s^{-1}, x_{0})d\mu(s) \right|
$$
$$
\leq 2 \int_{G-K} \rho(s)d\mu(s) + \int_{K} \frac{\varepsilon}{\mu(K)} d\mu(s) \leq 3\varepsilon
$$

d'où notre assertion. Supposons de plus $f \in \mathcal{K}(X)$. Soit $H$ une partie compacte de $X$ telle que $|f(y)| \leq \varepsilon$ pour $y \notin H$. Soit $x \notin KH$. On a $s^{-1}x \notin H$ pour $s \in K$, donc

$$
\left| \int_G f(s^{-1}x)\chi(s^{-1}, x)d\mu(s) \right| \leq \int_{G-K} \rho(s)d\mu(s) + \int_K \varepsilon \rho(s)d\mu(s)
$$
$$
\leq \varepsilon \left( 1 + \int_G \rho(s)d\mu(s) \right)
$$

ce qui achève de prouver (iii).

Enfin, si $f \in \mathcal{K}(X)$, comme $\varepsilon_x \in \mathcal{M}^1(X)$ pour tout $x \in X$, on a
$$
(\gamma_x(\mu)f)(x) = \int (\gamma_x(s)f)(x)d\mu(x)
$$
donc $\gamma_x(\mu)f$ est le produit de convolution $\mu *^\beta f$ défini par (3).

#### Proposition 6 {#int-viii-s4-prop-6 .statement}

*Supposons $\chi$ continue et chaque fonction $\chi(s, .)$ bornée. Soit $\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$. Soient $p$ et $q$ deux exposants conjugués ($1 \leq p < +\infty$). Soient $\mu \in \mathcal{M}^{p^{1/q}}(G)$ et $f \in L^p(X, \beta)$. Alors :

(i) $\mu$ et $f$ sont convolables ;
(ii) le produit de convolution $\mu *^\beta f$ est donné localement $\beta$-presque partout par la formule (3), et est égal localement $\beta$-presque partout à une fonction $g \in L^p(X, \beta)$ telle que $\|g\|_p \leq \|\mu\|_{p^{1/q}} \|f\|_p$;
(iii) $g$ est égal à l'élément $\gamma_x(\mu)f$ défini par la représentation continue $\gamma_x$ de $G$ dans $L^p(X, \beta)$.

On a
$$
\int^* \|\gamma_x(s)f\|_p d|\mu|(s) \leq \left( \int^* \rho(s)^{1/q} d|\mu|(s) \right) \|f\|_p < +\infty
$$
d'après le § 2, n° 5, formule (5). D'autre part, l'application $s \to \gamma_x(s)f$ de $G$ dans $L^p(X, \beta)$ est continue ($\S$ 2, prop. 9). Donc cette application est $\mu$-intégrable. Soit
$$
g = \int_G (\gamma_x(s)f)d\mu(s) \in L^p(X, \beta).
$$

On a $\|g\|_p \leq \left( \int \rho^{1/q}(s) d|\mu|(s) \right) \|f\|_p$. Appliquant les remarques précédentes à $|f|$, on voit que l’application $s \to \varepsilon_s * |f|$ de G dans $L^p(X, \beta)$ est $\mu$-intégrable, donc que, pour toute $h \in \mathcal{H}(X)$, l’application $s \to \langle h, \varepsilon_s * (|f|.\beta) \rangle$ est $\mu$-intégrable. La prop. 7 du § 1, n° 5, prouve alors que $\mu$ et $f.\beta$ sont convolables. En outre,

$$
\int_X g(x)h(x)d\beta(x) = \int_G d\mu(s) \int_X (\gamma_x(s)f)(x)h(x)d\beta(x)
$$

$$
= \int_G \langle h, \varepsilon_s *(f.\beta) \rangle d\mu(s)
$$

et cette dernière intégrale est égale à $\langle h, \mu * (f.\beta) \rangle$ d’après la prop. 7 du § 1, n° 5. On voit donc que $g$ est un produit de convolution de $\mu$ et $f$. Ce produit de convolution est donné localement $\beta$-presque partout par (3) d’après la prop. 2 et la Remarque qui la suit.

Par abus de notation, c’est souvent l’une des fonctions $g$ de l’énoncé qu’on note $\mu *_{\beta} f$, ce qui permet d’écrire

$$
\| \mu *_{\beta} f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p.
$$

Si $X$ est dénombrable à l’infini, cette manière d’écrire est d’ailleurs entièrement justifiée.

#### Corollaire {#int-viii-s4-n2-cor-1 .statement}

Sous les hypothèses de la prop. 6, l’application $(\mu, f) \to \mu *_{\beta} f$ définit sur $L^p(X, \beta)$ une structure de module à gauche sur $\mathcal{M}^{\rho^{1/q}}(G)$ ($1 \leq p \leq +\infty$).

Ceci résulte des prop. 5 et 6 et de l’associativité du produit de convolution.

#### Remarque 2 {#int-viii-s4-n2-rem-2 .statement}

Soit $X$ un espace localement compact sur lequel un groupe localement compact $G$ opère à droite continûment par $(x,s) \to xs$. Soit $\beta$ une mesure positive sur $X$. Soit $\chi$ une fonction $> 0$ sur $G \times X$, mesurable pour toute mesure sur $G \times X$, et telle que, pour tout $s \in G$, on ait $\delta(s)\beta = \chi(s, .).\beta$. Soit $f$ une fonction localement $\beta$-intégrable sur $X$ et soit $\mu$ une mesure sur $G$. Si $f.\beta$ et $\mu$ sont convolables (pour l’application $(x, s) \to xs$ de $X \times G$ dans $X$), $(f.\beta) * \mu$ est de base $\beta$. On dit alors que $f$ et $\mu$ sont convolables relativement à $\beta$; toute densité de $(f.\beta) * \mu$ par rapport à $\beta$ s'appelle un produit de convolution de $f$ et $\mu$ relativement à $\beta$ et se note $f *_{\beta} \mu$ ou simplement $f * \mu$.

Soit $G^0$ le groupe opposé à $G$. Par $(s, x) \to xs$, $G^0$ opère à gauche continûment dans $X$. Dire que $f$ et $\mu$ sont convolables au sens précédent équivaut à dire que $\mu$ et $f$ sont convolables pour $G^0$ opérant à gauche dans $X$; et les produits de convolution $f *_{\beta} \mu$ ne sont autres que les produits de convolution $\mu *_{\beta} f$ pour $G^0$ opérant à gauche dans $X$. D'autre part, on a, pour $s \in G^0$, $\gamma(s)\beta = \chi(s^{-1}, .) \cdot \beta$. Les résultats des n°s 1 et 2 se traduisent alors immédiatement en résultats concernant les produits $f *_{\beta} \mu$. En particulier :

1) Si $s \in G$ et si $f$ est localement $\beta$-intégrable, $f$ et $\varepsilon_s$ sont convolables, et l'on a

$$
(f * \varepsilon_s)(x) = \chi(s^{-1}, x)f(xs^{-1})
$$

2) Si $f$ et $\mu$ sont convolables et si l'une des conditions (i), (ii), (iii) de la prop. 2 est remplie, alors $f *_{\beta} \mu$ est donnée localement $\beta$-presque partout par

$$
(f *_{\beta} \mu)(x) = \int_G f(xs^{-1})\chi(s^{-1}, x)d\mu(s).
$$

Nous laissons au lecteur le soin de traduire les autres énoncés. On notera que, si $\chi$ est continue, on a

$$
\chi(ts, x) = \chi(s, xt)\chi(t, x) \qquad (x \in X ; s, t \text{ dans } G).
$$

### 3. **Convolution et transposition.**

Revenons aux hypothèses et aux notations du début du n° 1, mais supposons de plus que $\beta$ soit *relativement invariante de multiplicateur* $\chi$; $\chi$ est donc une fonction continue sur $G$.

#### Proposition 7 {#int-viii-s4-prop-7 .statement}

*Soient $f$ une fonction localement $\beta$-intégrable sur $X$, $\nu$ une mesure sur $X$ et $\mu$ une mesure sur $G$. On suppose que :*

(i) $\mu$ et $f$ sont convolables et la formule (3) du n° 1 définit localement $\beta$-presque partout un produit de convolution $\mu *_{\beta} f$.

(ii) $\chi . \tilde{\mu}$ et $\nu$ sont convolables.

(iii) La fonction $g(s, x) = f(s^{-1}x)\chi(s^{-1})$ est $(\mu \otimes \nu)$-intégrable. Alors $f$ est essentiellement intégrable pour $(\chi . \tilde{\mu}) * \nu$, la fonction $\mu *_{\beta} f$ définie par (3) est $\nu$-intégrable et l’on a

$$
\nu(\mu *_{\beta} f) = ((\chi . \tilde{\mu}) * \nu)(f).
$$

Puisque $g(s, x)$ est intégrable pour $\mu \otimes \nu$, la fonction $f(sx)$ est essentiellement intégrable pour $(\chi . \tilde{\mu}) \otimes \nu$ et $f$ est essentiellement intégrable pour $(\chi . \tilde{\mu}) * \nu$. D’après le théorème de Lebesgue-Fubini, $\mu *_{\beta} f = \int g(s, x)d\mu(s)$ est $\nu$-intégrable et l’on a

$$
\begin{align*}
\nu(\mu *_{\beta} f) &= \iint f(s^{-1}x)\chi(s^{-1})d\mu(s)d\nu(x) \\
&= \iint f(sx)\chi(s)d\tilde{\mu}(s)d\nu(x) = ((\chi . \tilde{\mu}) * \nu)(f).
\end{align*}
$$

#### Exemple 1 {#int-viii-s4-n3-exa-1 .statement}

On peut prendre $f \in \mathcal{C}(X)$, $\nu \in \mathcal{C}'(X)$ et $\mu \in \mathcal{C}'(G)$ d’après la prop. 3, et le cor. de la prop. 5 du § 1, n° 4. La formule (7) signifie alors que l’endomorphisme $\nu \to (\chi . \tilde{\mu}) * \nu$ de $\mathcal{C}'(X)$ est le transposé de l’endomorphisme $f \to \mu * f$ de $\mathcal{C}(X)$.

#### Exemple 2 {#int-viii-s4-n3-exa-2 .statement}

On peut prendre $f \in \mathcal{K}(X)$, $\nu \in \mathcal{M}(X)$ et $\mu \in \mathcal{C}'(G)$ d’après la prop. 3, la prop. 8 du § 3, n° 2, et la remarque que le support de la fonction continue $g(s, x)$ rencontre le support de $\mu \otimes \nu$ suivant un ensemble compact. La formule (7) signifie alors que l’endomorphisme $\nu \to (\chi . \tilde{\mu}) * \nu$ de $\mathcal{M}(X)$ est le transposé de l’endomorphisme $f \to \mu * f$ de $\mathcal{K}(X)$.

#### Exemple 3 {#int-viii-s4-n3-exa-3 .statement}

Si G opère proprement dans X, on peut prendre $f \in \mathcal{K}(X)$, $\nu \in \mathcal{C}'(X)$ et $\mu \in \mathcal{M}(G)$ d’après la prop. 4, la prop. 8 du § 3, n° 2, et la même remarque que dans l’Exemple 2.

#### Proposition 8 {#int-viii-s4-prop-8 .statement}

Soient $f$ et $g$ deux fonctions localement $\beta$-intégrables sur $X$ et soit $\mu \in \mathcal{M}(G)$. On suppose que :

(i) $\mu$ et $f$ sont convolables et la formule (3) du n° 1 définit localement $\beta$-presque partout un produit de convolution $\mu *_{\beta} f$.

(ii) $\chi \cdot \tilde{\mu}$ et $g$ sont convolables et la formule (3) du no 1 (où on remplace $\mu$ par $\chi \cdot \tilde{\mu}$ et $f$ par $g$) définit localement $\beta$-presque partout un produit de convolution $(\chi \cdot \tilde{\mu}) *_{\beta} g$.

(iii) Il existe une fonction $\psi$ sur $G$, localement $\mu$-presque partout égale à 1, telle que la fonction $h(s, x) = g(x)f(s^{-1}x)\chi(s^{-1})\psi(s)$ soit $(\mu \otimes \beta)$-intégrable.

Alors les fonctions $g(x)((\mu *_{\beta} f)(x))$ et $f(x)(((\chi \cdot \tilde{\mu}) *_{\beta} g)(x))$ sont essentiellement $\beta$-intégrables, et l’on a

$$
\int f(x)(((\chi \cdot \tilde{\mu}) *_{\beta} g)(x))d\beta(x) = \int g(x)((\mu *_{\beta} f)(x))d\beta(x)
$$

En effet, d’après (iii) et le théorème de Lebesgue-Fubini, la fonction $x \to g(x) \int f(s^{-1}x)\chi(s^{-1})\psi(s)d\mu(s)$ est $\beta$-intégrable et on a

$$
\begin{align*}
I &= \iint f(s^{-1}x)g(x)\chi(s^{-1})\psi(s)d\mu(s)d\beta(x) \\
&= \int g(x)d\beta(x) \int f(s^{-1}x)\chi(s^{-1})\psi(s)d\mu(s)
\end{align*}
$$

Mais on a $\psi \cdot \mu = \mu$ et par suite

$$
\int f(s^{-1}x)\chi(s^{-1})\psi(s)d\mu(s) = (\mu *_{\beta} f)(x),
$$

localement $\beta$-presque partout. Ceci montre que la fonction $x \to g(x)((\mu *_{\beta} f)(x))$ est essentiellement $\beta$-intégrable et que

$$
I = \int g(x)((\mu *_{\beta} f)(x))d\beta(x).
$$

D’autre part, le lemme 1 montre que la fonction $(s, x) \to g(sx)f(x)\chi(s^{-1})\psi(s)$ est intégrable pour $(\chi \cdot \mu) \otimes \beta$. Donc la fonction $(s, x) \to g(s^{-1}x)f(x)\psi(s^{-1})$ est intégrable pour $\tilde{\mu} \otimes \beta$ et l’on a

$$
\begin{align*}
I &= \iint g(s^{-1}x)f(x)\psi(s^{-1})d\tilde{\mu}(s)d\beta(x) \\
&= \int f(x)d\beta(x) \int g(s^{-1}x)\psi(s^{-1})d\tilde{\mu}(s).
\end{align*}
$$

Mais $\tilde{\psi} \cdot \tilde{\mu} = \tilde{\mu}$ et par suite $\int g(s^{-1}x)\psi(s^{-1})d\tilde{\mu}(s) = ((\chi \cdot \tilde{\mu}) *_{\beta} g)(x)$ localement $\beta$-presque partout. Ceci montre que la fonction $x \to f(x)(((\chi \cdot \tilde{\mu}) *_{\beta} g)(x))$ est essentiellement $\beta$-intégrable et que

$$
I = \int f(x)(((\chi \cdot \tilde{\mu}) *_{\beta} g)(x))d\beta(x).
$$

Ceci démontre la proposition.

#### Exemple 4 {#int-viii-s4-n3-exa-4 .statement}

On peut prendre $f \in \mathcal{C}(X),\ g \in \mathcal{K}(X)$ et $\mu \in \mathcal{C}'(G)$ (avec $\psi = 1$).

#### Exemple 5 {#int-viii-s4-n3-exa-5 .statement}

Si G opère proprement sur X, on peut prendre $f \in \mathcal{K}(X),\ g \in \mathcal{K}(X)$ et $\mu \in \mathcal{M}(G)$ (avec $\psi = 1$).

#### Exemple 6 {#int-viii-s4-n3-exa-6 .statement}

On peut prendre $f \in L^p(X, \beta),\ g \in L^q(X, \beta)$ et $\mu \in \mathcal{M}^o(G)$ avec $1 \leq p < +\infty,\ \frac{1}{p} + \frac{1}{q} = 1,\ \rho = \chi^{-1/q}$. Les conditions (i) et (ii) sont satisfaites d'après les prop. 5 et 6. Démontrons (iii). On a vu que $\mu$ était portée par un ensemble S réunion dénombrable d'ensembles compacts. On prendra pour $\psi$ la fonction caractéristique de S. La fonction $h$ est $(\mu \otimes \beta)$-mesurable : en effet la fonction $(s, x) \to g(x)\chi(s^{-1})\psi(s)$ l'est, ainsi que la fonction $(s, x) \to f(s^{-1}x)$ d'après le lemme 1. De plus, $g$ étant nulle hors d'une réunion dénombrable d'ensembles $\beta$-intégrables, $h$ est nulle hors d'une réunion dénombrable d'ensembles $(\mu \otimes \beta)$-intégrables. On a alors (chap. V, § 8, no 1, prop. 4):

$$
\begin{align*}
J &= \iint^* |g(x)f(s^{-1}x)|\chi(s^{-1})\psi(s)d|\mu|(s)d\beta(x) \\
&= \int^* |g(x)|d\beta(x) \int^* |f(s^{-1}x)|\chi(s^{-1})\psi(s)d|\mu|(s).
\end{align*}
$$

Mais comme $g$ (resp. $\psi$) est nulle hors d'une réunion dénombrable d'ensembles intégrables, les intégrales supérieures du second membre de (9) sont égales aux intégrales supérieures essentielles (chap. V, § 2, no 1, prop. 3). Or (chap. V, § 5, no 3, prop. 2) on a

$$
\int^* |f(s^{-1}x)| \chi(s^{-1}) \psi(s) d|\mu|(s) = \int^* |f(s^{-1}x)| \chi(s^{-1}) d|\mu|(s)
$$
puisque $\mu = \psi \cdot \mu$. D'après la prop. 6, cette dernière intégrale est finie et égale à $(|\mu| *^\beta |f|)(x)$ localement $\beta$-presque partout. On a donc
$$
J = \int^* |g(x)| (|\mu| *^\beta |f|)(x) d\beta(x)
$$
et $J$ est finie puisque $g \in L^q$ et $|\mu| *^\beta |f| \in L^p$ (prop. 6). Donc $h$ est $(\mu \otimes \beta)$-intégrable.

La formule (8) signifie alors que l'endomorphisme
$$
g \to (\chi \cdot \tilde{\mu}) * g
$$
de $L^q(X, \beta)$ est, pour $\mu \in \mathcal{M}^p(G)$, le transposé de l'endomorphisme $f \to \mu * f$ de $L^p(X, \beta)$.

### 4. Convolution d'une mesure et d'une fonction sur un groupe

Soit $G$ un groupe localement compact. Fixons dans les nos 4 et 5 une mesure positive $\beta \neq 0$ sur $G$, relativement invariante ; soient $\chi$ et $\chi'$ ses multiplicateurs à gauche et à droite (rappelons que $\chi' = \chi \Delta_G$). Si $\mu$ est une mesure sur $G$ et $f$ une fonction localement $\beta$-intégrable sur $G$, la convolabilité de $\mu$ et $f$ et les produits $\mu * f$ (resp. la convolabilité de $f$ et $\mu$ et les produits $f * \mu$) se définissent en considérant $G$ comme opérant sur lui-même à gauche (resp. à droite) par translations. Explicitons dans cette situation quelques-uns des résultats précédents :

1) Soient $\mu$ une mesure sur $G$, $f$ une fonction complexe localement $\beta$-intégrable sur $X$. On suppose vérifiée l'une des conditions suivantes :
   (i) $f$ est continue ;
   (ii) $f$ est nulle dans le complémentaire d'une réunion dénombrable d'ensembles compacts ;
   (iii) $\mu$ est portée par une réunion dénombrable d'ensembles compacts.

Si $\mu$ et $f$ sont convolables, on a localement $\beta$-presque partout

$$
(\mu * f)(x) = \int_G f(s^{-1}x)\chi(s^{-1})d\mu(s).
$$

Si $f$ et $\mu$ sont convolables, on a localement $\beta$-presque partout

$$
(f * \mu)(x) = \int_G f(xs^{-1})\chi'(s^{-1})d\mu(s).
$$

2) Soient $p$ et $q$ deux exposants conjugués ($1 \leq p \leq +\infty$). Si $\mu \in \mathcal{M}^{\chi^{-1/q}}(G)$ et $f \in L^p(G, \beta)$, $\mu$ et $f$ sont convolables, et $\mu * f$ est égale localement $\beta$-presque partout à une fonction de $L^p(G, \beta)$; on a (avec un abus de notations déjà signalé)

$$
\| \mu * f \|_p \leq \| \mu \|_{\chi^{-1/q}} \| f \|_p.
$$

Si $\mu \in \mathcal{M}^{{\chi'}^{-1/q}}(G)$ et $f \in L^p(G, \beta)$, $f$ et $\mu$ sont convolables, et $f * \mu$ est égale localement $\beta$-presque partout à une fonction de $L^p(G, \beta)$; on a $\| f * \mu \|_p \leq \| \mu \|_{{\chi'}^{-1/q}} \| f \|_p$.

3) Les applications $(\mu, f) \to \mu * f, (f, \mu) \to f * \mu$ définissent sur $L^p(G, \beta)$ des structures de module à gauche sur $\mathcal{M}^{\chi^{-1/q}}(G)$ et de module à droite sur $\mathcal{M}^{{\chi'}^{-1/q}}(G)$. Les deux lois externes sur $L^p(G, \beta)$ sont permutables d’après l’associativité de la convolution.

4) Si $\mu * f$ est continue et donnée en tout point par (10), on a

$$
(\mu * f)(e) = \int f(s^{-1})\chi(s^{-1})d\mu(s).
$$

Si $f * \mu$ est continue et donnée en tout point par (11), on a

$$
(f * \mu)(e) = \int f(s^{-1})\chi'(s^{-1})d\mu(s).
$$

### 5. **Convolution des fonctions sur un groupe.**

On conserve les notations $G, \beta, \chi, \chi'$ du n° 4.

Rappelons que, si $f$ est une fonction complexe sur $G$, la propriété d’être localement $\beta$-intégrable est indépendante du choix de $\beta$. Soit $\mathcal{L}(G)$ l’ensemble des fonctions possédant cette propriété. Si $f \in \mathcal{L}(G)$, $g \in \mathcal{L}(G)$, la relation

« $f.\beta$ et $g.\beta$ sont convolables »

est indépendante du choix de $\beta$ ($§ 3$, n° 1, prop. 6). Nous dirons alors que $f$ et $g$ sont *convolables*. D’après le n° 1, $(f.\beta) * (g.\beta)$ est de la forme $h.\beta$ avec $h \in \mathcal{L}$, $h$ étant déterminée aux ensembles localement $\beta$-négligeables près. On posera $h = f *^\beta g$ et on dira que $h$ est un *produit de convolution* de $f$ et $g$ relativement à $\beta$. (On omet $\beta$ quand aucune confusion n’est possible). Si $\beta$ est remplacée par $\psi.\beta$, $\psi$ étant une représentation continue de $G$ dans $\mathbf{R}_+^*$, $h$ ne change pas ($§ 3$, n° 1, prop. 6) ; si $\beta$ est remplacée par $a\beta$ ($a \in \mathbf{R}_+^*$), $h$ est remplacée par $ah$. On définit de manière analogue le produit de convolution de plusieurs fonctions sur $G$.

Si l’une des convolées de $f$ et $g$ est continue, elle est déterminée de manière unique puisque le support de $\beta$ est $G$. On l’appelle alors *le produit de convolution de $f$ et $g$ relativement à $\beta$*.

Il est clair que

$$
f *^\beta g = (f.\beta) *^\beta g = f *^\beta (g.\beta).
$$

#### Proposition 9 {#int-viii-s4-prop-9 .statement}

*Soient $f, g$ dans $\mathcal{L}(G)$. Supposons que la fonction $s \to g(s^{-1}x)f(s)\chi(s^{-1})$ soit essentiellement $\beta$-intégrable sauf pour un ensemble localement $\beta$-négligeable de valeurs de $x$, et que la fonction $x \to \int |g(s^{-1}x)f(s)|\chi(s^{-1})d\beta(s)$, définie localement $\beta$-presque partout, soit localement $\beta$-intégrable. Alors $f$ et $g$ sont convolables.*

Ceci résulte de la prop. 1 du n° 1.

#### Proposition 10 {#int-viii-s4-prop-10 .statement}

*Soient $f, g$ dans $\mathcal{L}(G)$. On suppose que l’une de ces deux fonctions est continue ou nulle dans le complémentaire d’une réunion dénombrable d’ensembles compacts. Si $f$* et $g$ sont convolables, la fonction $f * g$ est donnée localement $\beta$-presque partout par

$$
(f * g)(x) = \int_G g(s^{-1}x)f(s)\chi(s^{-1})d\beta(s)
$$
$$
= \int_G f(xs^{-1})g(s)\chi'(s^{-1})d\beta(s)
$$

Ceci résulte de la prop. 2 du n° 1, et des remarques du n° 4.

En particulier, si $f * g$ est continue et donnée en tout point par (15), on a
$$
(f * g)(e) = \int g(s^{-1})f(s)\chi(s^{-1})d\beta(s) = \int f(s^{-1})g(s)\chi'(s^{-1})d\beta(s).
$$

Plus particulièrement encore, si $\beta$ est une mesure de Haar à gauche et à droite, si $f * g$ et $g * f$ sont continues et données en tout point par (15) et la formule analogue pour $g * f$, on a
$$
(f * g)(e) = (g * f)(e) = \int f(s)g(s^{-1})d\beta(s).
$$

#### Proposition 11 {#int-viii-s4-prop-11 .statement}

Soient $f, g$ dans $\mathcal{L}(G)$. On suppose que l'une des fonctions $f, g$ est continue et que l'une des fonctions $f, g$ est à support compact. Alors $f$ et $g$ sont convolables. La formule (15) définit pour tout $x \in G$ un produit $f * g$ qui est continu. Si $f \in \mathcal{H}(G)$ et $g \in \mathcal{H}(G)$, on a $f * g \in \mathcal{H}(G)$.

Ceci résulte des prop. 3 et 4 du n° 2.

#### Proposition 12 {#int-viii-s4-prop-12 .statement}

Soient $p$ et $q$ deux exposants conjugués ($1 \leq p \leq +\infty$). Si $f\chi^{-1/q} \in L^1(G, \beta)$ et $g \in L^p(G, \beta)$, $f$ et $g$ sont convolables, $f * g$ est égale localement $\beta$-presque partout à une fonction de $L^p(G, \beta)$, et on a
$$
\|f * g\|_p \leq \|f\chi^{-1/q}\|_1 \|g\|_p.
$$
Si $f \in L^p(G, \beta)$ et $g{\chi'}^{-1/q} \in L^1(G, \beta)$ $f$ et $g$ sont convolables, $f * g$ est égale localement $\beta$-presque partout à une fonction de $L^p(G, \beta)$, et on a
$$
\|f * g\|_p \leq \|f\|_p \|g{\chi'}^{-1/q}\|_1.
$$

Ceci résulte des prop. 5 et 6 du n° 2 et des remarques du n° 4.

#### Proposition 13 {#int-viii-s4-prop-13 .statement}

Si $f\chi^{-1} \in L^1(G, \beta)$ et $g \in \mathcal{K}(G)$, ou si $f \in \mathcal{K}(G)$ et $g{\chi'}^{-1} \in L^1(G, \beta)$, $f$ et $g$ sont convolables, et (15) définit pour tout $x \in G$ un produit $f * g$ qui appartient à $\mathcal{K}(G)$.

Cela résulte de la prop. 5 du n° 2 et des remarques du n° 4.

#### Proposition 14 {#int-viii-s4-prop-14 .statement}

Si $f\chi^{-1} \in L^1(G, \beta)$ et $g \in L^\infty(G, \beta)$, la formule (15) définit pour tout $x \in G$ un produit $f * g$ qui est borné et uniformément continu pour la structure uniforme droite de $G$.

On sait déjà que $f * g$ appartient à $L^\infty(G, \beta)$ (n° 2, prop. 5) ; en outre on a $(f * g)(x) = \int f(xs^{-1})g(s)d\nu(s)$, en posant $\nu = {\chi'}^{-1}.\beta$; $\nu$ est une mesure de Haar à droite. Donc

$$
|(f * g)(x) - (f * g)(x')| \leq \|g\|_\infty \int |f(xs^{-1}) - f(x's^{-1})|d\nu(s)
$$

$$
= \|g\|_\infty \int |f(s^{-1}) - f(x'x^{-1}s^{-1})|d\nu(s)
$$

et la dernière intégrale est arbitrairement petite pourvu que $x'x^{-1}$ soit dans un voisinage convenable de $e$ (§ 2, n° 5, prop. 8).

#### Proposition 15 {#int-viii-s4-prop-15 .statement}

Soient $p$ et $q$ deux exposants conjugués $(1 < p < +\infty)$. Supposons $\beta$ invariante à gauche. Soient $f \in L^p(G, \beta)$, $g \in L^q(G, \tilde{\beta})$. Alors $f$ et $g$ sont convolables. La formule (15) définit, pour tout $x \in G$, un produit $f * g$ qui appartient à $\mathcal{K}(G)$, et qui est tel que $\|f * g\|_\infty \leq \|f\|_p\|\tilde{g}\|_q$.

En effet, on a $\tilde{g} \in L^q(G, \beta)$, donc la fonction $s \to g(s^{-1}x)f(s)$ est $\beta$-intégrable pour tout $x \in G$. En outre,

$$
\int |g(s^{-1}x)f(s)|d\beta(s) \leq \left( \int |f(s)|^p d\beta(s) \right)^{1/p} \left( \int |g(s^{-1}x)|^q d\beta(s) \right)^{1/q}
$$

$$
= \|f\|_p \left( \int |\tilde{g}(x^{-1}s)|^q d\beta(s) \right)^{1/q} = \|f\|_p\|\tilde{g}\|_q
$$

donc $f$ et $g$ sont convolables (prop. 9). On voit en même temps que (15) définit pour tout $x$ un produit $f * g$ tel que

$$
|(f * g)(x)| \leq \|f\|_p\|\tilde{g}\|_q .
$$

Pour $f, g$ dans $\mathcal{K}(G)$, on a $f * g \in \mathcal{K}(G)$ (prop. 11) ; donc, pour $f \in L^p(G, \beta)$ et $g \in L^q(G, \bar{\beta})$, le produit $f * g$ fourni par (15) est limite uniforme de fonctions de $\mathcal{K}(G)$, donc appartient à $\overline{\mathcal{K}(G)}$.

#### Corollaire {#int-viii-s4-n5-cor-1 .statement}

*Soient $f \in L^2(G, \beta)$, $g \in L^2(G, \beta)$. Alors $f$ et $\overline{g}$ sont convolables. L'une des convolées $f * \overline{g}$ appartient à $\overline{\mathcal{K}(G)}$ et sa valeur en $e$ est $\int_G f(s) \overline{g(s)} d\beta(s)$.*

Il suffit de faire $p = q = 2$ dans la prop. 15 et d'appliquer (16).

On ne suppose plus $\beta$ invariante à gauche. Soit $\rho$ une fonction $> 0$ finie semi-continue inférieurement sur $G$ telle que $\rho(st) \leq \rho(s)\rho(t)$ quels que soient $s, t$ dans $G$. On note $L^\rho(G, \beta)$ l'ensemble des classes de fonctions complexes sur $G$ intégrables pour $\rho.\beta$. Par l'application $f \to f.\beta$, $L^\rho(G, \beta)$ s'identifie à l'ensemble des éléments de $\mathcal{M}^\rho(G)$ qui sont de base $\beta$ (ensemble qui est indépendant du choix de $\beta$). Si on pose

$$
\|f\|_\rho = \int_G |f(s)| \rho(s) d\beta(s)
$$

pour $f \in L^\rho(G, \beta)$, cette identification est compatible avec les normes, donc $L^\rho(G, \beta)$ apparaît comme une sous-algèbre normée complète de $\mathcal{M}^\rho(G)$. C'est même un idéal bilatère de $\mathcal{M}^\rho(G)$ d'après la prop. 10 du § 3, no 2. (Pour $\rho = 1$, on retrouve une des assertions du no 4). En particulier, $L^1(G, \beta)$ s'identifie à un idéal bilatère fermé de $\mathcal{M}^1(G)$.

#### Proposition 16 {#int-viii-s4-prop-16 .statement}

*Soit $U$ une représentation continue de $G$ dans un espace de Banach $E$. Posons $\rho(s) = \|U(s)\|$ pour tout $s \in G$. Pour toute $f \in L^\rho(G, \beta)$, posons $U(f) = U(f.\beta)$. Alors $f \to U(f)$ est une représentation linéaire de l'algèbre $L^\rho(G, \beta)$ dans $E$, telle que $\|U(f)\| \leq \|f\|_\rho$.*

Ceci résulte du § 2, no 6, et du § 3, no 3, prop. 11.

### 6. Applications.

#### Proposition 17 {#int-viii-s4-prop-17 .statement}

Soient G un groupe localement compact, A une partie de G, mesurable et non localement négligeable pour une mesure de Haar. Alors A.A^{-1} est un voisinage de e.

Soit $\beta$ une mesure de Haar à gauche. Il existe une partie compacte K de G telle que B = A $\cap$ K soit intégrable de mesure > 0 pour $\beta$. Appliquons le cor. de la prop. 15 avec $f = g = \varphi_B$. La fonction $F = \varphi_B * \tilde{\varphi}_B$ est continue et > 0 en e. Donc il existe un voisinage V de e tel que $F(x) > 0$ pour $x \in V$. Or

$$
F(x) = \int \varphi_B(s) \varphi_B(x^{-1}s) d\beta(s) = \beta(B \cap xB).
$$

Donc, pour $x \in V$, on a $B \cap xB \neq \emptyset$, d'où $x \in B.B^{-1}$. Donc $V \subset B.B^{-1} \subset A.A^{-1}$.

#### Corollaire 1 {#int-viii-s4-prop-17-cor-1 .statement}

Soit H un sous-groupe de G mesurable pour une mesure de Haar $\beta$. Alors H est, soit ouvert, soit localement $\beta$-négligeable.

Car $H = H.H^{-1}$, donc, si H n'est pas localement $\beta$-négligeable, H contient un voisinage de e (prop. 17) et est par suite ouvert (Top. Gén., chap. III, 3e éd., § 2, no 1, cor. de la prop. 4).

#### Corollaire 2 {#int-viii-s4-prop-17-cor-2 .statement}

Soit L une partie de G stable pour la multiplication et dont le complémentaire est localement négligeable pour une mesure de Haar $\beta$. Alors $L = G$.

En effet, $L^{-1}$ et $L \cap L^{-1}$ sont de complémentaires localement $\beta$-négligeables. Or $L \cap L^{-1}$ est un sous-groupe, donc est ouvert (cor. 1) et par suite fermé. Donc $G - (L \cap L^{-1})$, qui est ouvert et localement $\beta$-négligeable, est vide. Donc $G = L \cap L^{-1}$.

#### Proposition 18 {#int-viii-s4-prop-18 .statement}

Soient G un groupe localement compact, $\Gamma$ un ensemble muni d'une multiplication $(u, v) \to uv$ et d'une topologie séparée telles que :
1) la topologie de $\Gamma$ est invariante par les translations ;
2) la restriction de la multiplication à toute partie compacte de $\Gamma$ est continue.

Soit $f : G \to \Gamma$ une application de $G$ dans $\Gamma$ telle que $f(xy) = f(x)f(y)$ pour $x, y$ dans $G$, et mesurable pour une mesure de Haar $\beta$ de $G$. Alors $f$ est continue.

Posons $g(x) = f(x^{-1})$ pour $x \in G$. Comme $f$ et $g$ sont $\beta$-mesurables, il existe une partie compacte $K$ non $\beta$-négligeable de $G$ telle que les restrictions de $f$ et $g$ à $K$ soient continues. L’application $(x, y) \to f(xy^{-1}) = f(x)g(y)$ de $K \times K$ dans $\Gamma$ est continue parce que la multiplication de $\Gamma$ est continue sur $f(K) \times g(K)$; or cette application s’écrit $\varphi \circ \psi$, où $\psi$ est l’application $(x, y) \to xy^{-1}$ de $K \times K$ sur $K.K^{-1}$, et où $\varphi$ est la restriction de $f$ à $K.K^{-1}$. Soit $R$ la relation d’équivalence définie sur $K \times K$ par $\psi$. L’application $\psi'$ de $(K \times K)/R$ sur $K.K^{-1}$ déduite de $\psi$ par passage au quotient est continue, donc $(K \times K)/R$ est séparé et $\psi'$ est un homéomorphisme. Comme $\varphi \circ \psi$ est continue, on voit que la restriction de $f$ à $K.K^{-1}$ est continue. Or $K.K^{-1}$ est un voisinage de $e$ (prop. 17), donc $f$ est continue en $e$. Pour tout $x_0 \in G$, on a $f(x_0x) = f(x_0)f(x)$, donc $f$ est continue en $x_0$ parce que la topologie de $\Gamma$ est invariante par translations.

#### Corollaire 1 {#int-viii-s4-prop-18-cor-1 .statement}

Soient $G$ un groupe localement compact, $\beta$ une mesure de Haar de $G$, $E$ un espace localement convexe tonnelé séparé, $U$ une représentation linéaire de $G$ dans $E$, telle que $U(s) \in \mathcal{L}(E; E)$ pour tout $s \in G$, $\beta$-mesurable quand on munit $\mathcal{L}(E; E)$ de la topologie de la convergence simple. Alors $U$ est une représentation linéaire continue.

Soit $\Gamma$ le groupe des automorphismes de $E$, muni de la topologie de la convergence simple. Cette topologie est séparée et invariante par translations. Soit $K$ une partie compacte de $\Gamma$. Alors $K$ est bornée dans $\mathcal{L}(E; E)$ muni de la topologie de la convergence simple, donc équicontinue ($Esp.\ vect.\ top.$, chap. III, § 3, n° 6, th. 2); donc l’application $(u, v) \to v \circ u$ de $K \times K$ dans $\mathcal{L}(E; E)$ est continue ($loc.\ cit.$, § 4, cor. 1 de la prop. 9). Donc, pour tout $x \in E$, l’application $s \to U(s)x$ de $G$ dans $E$ est continue (prop. 18). Comme $E$ est tonnelé, $U$ est continue ($§\ 2,\ n°\ 1,\ prop.\ 1$).

#### Corollaire 2 {#int-viii-s4-prop-18-cor-2 .statement}

Soient G un groupe localement compact, $\beta$ une mesure de Haar sur G, E un espace de Banach de type dénombrable, U une représentation linéaire de G dans E, telle que $U(s) \in \mathcal{L}(E; E)$ pour tout $s \in G$. Soit $(a_m)$ une suite totale dans E, et soit $(a'_n)$ une suite partout dense dans la boule unité B' du dual E' de E, munie de la topologie faible. On suppose que les fonctions $s \to \langle U(s)a_m, a'_n \rangle$ sur G sont $\beta$-mesurables. Alors U est une représentation linéaire continue.

Montrons d’abord que pour tout $z' \in E'$, les fonctions numériques
$$
s \to \langle U(s)a_m, z' \rangle
$$
sont $\beta$-mesurables ; on peut se borner au cas où $\|z'\| \leq 1$, et comme B' est métrisable pour la topologie faible (*Esp. vect. top.*, chap. IV, § 5, n° 1, prop. 2), il existe une suite $(a'_{n_k})$ extraite de $(a'_n)$ et qui converge faiblement vers $z'$; la fonction
$$
s \to \langle U(s)a_m, z' \rangle
$$
est donc limite d’une suite de fonctions $\beta$-mesurables d’où notre assertion. On en conclut que l’application $s \to U(s)a_m$ de G dans E est $\beta$-mesurable pour tout m (chap. IV, § 5, n° 5, prop. 10). D’autre part, il existe une suite $(b_m)$ d’éléments de E, combinaisons linéaires des $a_i$, qui est partout dense dans la boule unité de E. Pour tout $s \in G$, on a $\|U(s)\| = \sup_m \|U(s)b_m\|$, donc $s \to \|U(s)\|$ est mesurable. Soit K une partie compacte de G et soit $\varepsilon > 0$. Il existe une partie compacte $K_0$ de K telle que $\beta(K - K_0) \leq \varepsilon$ et que les restrictions à $K_0$ des fonctions $s \to U(s)a_m$ et $s \to \|U(s)\|$ soient continues. Alors les $U(s)$ pour $s \in K_0$ sont équicontinus et la topologie de la convergence simple induit sur $U(K_0)$ la topologie de la convergence simple dans l’ensemble des $a_m$ (*Esp. vect. top.*, chap. III, § 3, n° 5, prop. 5). Par suite l’application $s \to U(s)$ de $K_0$ dans $\mathcal{L}_s(E; E)$ est continue. Il suffit alors d’appliquer le cor. 1.

### 7. Régularisation.

#### Proposition 19 {#int-viii-s4-prop-19 .statement}

Soient G un groupe localement compact, $\beta$ une mesure positive $\neq 0$ relativement invariante sur G, $\mathcal{B}$ une base du filtre des voisinages de e dans G, formée de voisinages compacts. Pour tout $V \in \mathcal{B}$, soit $f_V$ une fonction continue $\geqslant 0$ sur $G$, de support contenu dans $V$, et telle que $\int f_V d\beta = 1$.

Alors, si $\mu$ est une mesure sur $G$, on a, dans $\mathcal{M}(G)$ muni de la topologie de la convergence compacte sur $\mathscr{K}(G)$,

$$
\mu = \lim_V (\mu * f_V) \cdot \beta = \lim_V (f_V * \mu) \cdot \beta
$$

la limite étant prise suivant le filtre des sections de $\mathcal{B}$.

Pour la topologie de la convergence compacte sur $\mathscr{C}(G)$, $f_V \cdot \beta$ tend vers $\varepsilon_e$ suivant le filtre des sections de $\mathcal{B}$ ($§ 2$, no 7, cor. 1 du lemme 4). Donc $\mu = \lim_V \mu * (f_V \cdot \beta) = \lim_V (f_V \cdot \beta) * \mu$ dans $\mathcal{M}(G)$ muni de la topologie de la convergence compacte sur $\mathscr{K}(G)$ ($§ 3$, no 3, cor. de la prop. 12).

#### Remarque 1 {#int-viii-s4-n7-rem-1 .statement}

On voit donc que toute mesure sur $G$ est limite de mesures admettant une densité continue par rapport à toute mesure de Haar (pour la topologie indiquée dans la prop. 19 et $a fortiori$ pour la topologie vague).

#### Remarque 2 {#int-viii-s4-n7-rem-2 .statement}

Si $G$ est métrisable, on peut prendre pour $\mathcal{B}$ une suite $(V_n)$ de voisinages. Alors $\mu$ est limite de la suite des mesures $(\mu * f_{V_n}) \cdot \beta$ à densités continues. *Si $G$ est un groupe de Lie réel, on peut prendre les $f_{V_n}$ indéfiniment différentiables ; nous verrons plus tard qu’alors les densités $\mu * f_{V_n}$ sont indéfiniment différentiables.*

#### Proposition 20 {#int-viii-s4-prop-20 .statement}

On conserve les hypothèses et les notations de la prop. 19. Soient $p \in [1, +\infty]$, et $g \in L^p(G, \beta)$. On a

$$
g = \lim_V g *^\beta f_V = \lim_V f_V *^\beta g
$$

au sens de la norme $N_p$, la limite étant prise suivant le filtre des sections de $\mathcal{B}$.

Il suffit d’appliquer la prop. 6 (iii), et le $§ 2$, no 7, cor. 3 du lemme 4.

#### Remarque 3 {#int-viii-s4-n7-rem-3 .statement}

D’après la prop. 15, les fonctions $g * f_V$, $f_V * g$ appartiennent à $\overline{\mathscr{K}}(G)$.

#### Corollaire {#int-viii-s4-n7-cor-1 .statement}

Soit W un sous-espace vectoriel fermé de $L^1(G, \beta)$. Pour que W soit un idéal à gauche (resp. à droite) de $L^1(G, \beta)$, il faut et il suffit que W soit invariant par les translations à gauche (resp. à droite) de G.

Supposons que W soit un idéal à gauche. Soient $s \in G$ et $g \in W$. On a $\varepsilon_s * g = \lim_{\nu} f_\nu * (\varepsilon_s * g) = \lim_{\nu} (f_\nu * \varepsilon_s) * g$, et $(f_\nu * \varepsilon_s) * g \in W$, donc $\varepsilon_s * g \in W$, donc $\gamma(s)g \in W$. Réciproquement, si W est invariant par les translations à gauche, on a $\mu *^\beta g \in W$ pour $\mu \in \mathcal{M}^1(G)$ et $g \in W$, donc W est a fortiori un idéal à gauche de $L^1(G, \beta)$. On raisonne de même pour les idéaux à droite.

#### Exemple {#int-viii-s4-n7-exa-1 .statement}

On prend $G = \mathbf{R}$. Définissons une fonction $F_n \in \mathcal{K}(\mathbf{R})$ par
$$
F_n(x) = (1 - x^2)^n \quad \text{si } x \in [-1, 1]
$$
$$
F_n(x) = 0 \qquad \text{si } x \notin [-1, 1].
$$
Soient $A_n = \int_{-1}^{+1} F_n(x) dx$, et $G_n = A_n^{-1} F_n$. Il est immédiat que les mesures $G_n(x) dx$ satisfont aux conditions du § 2, no 7, cor. 1 du lemme 4. Soit $\mu$ une mesure sur $\mathbf{R}$ dont le support soit contenu dans $(-1/2, 1/2)$. On a
$$
(\mu * G_n)(x) = \int_{\mathbf{R}} G_n(x - y) d\mu(y)
$$
$$
= A_n^{-1} \int_{-1/2}^{1/2} F_n(x - y) d\mu(y)
$$
Si $-\frac{1}{2} \leq x \leq \frac{1}{2}$, on a alors
$$
(\mu * G_n)(x) = A_n^{-1} \int_{-1/2}^{1/2} [1 - (x - y)^2]^n d\mu(y)
$$
donc $\mu * G_n$ coïncide dans $(-1/2, 1/2)$ avec un polynôme. En particulier, si $f$ est une fonction continue à support contenu dans $(-1/2, 1/2)$, $f * G_n$ coïncide dans $(-1/2, 1/2)$ avec un polynôme ; par ailleurs, d’après la prop. 5 (iv), et le § 2, no 7, cor. 3 du lemme 4, $f * G_n$ converge uniformément vers $f$. *Si $f$ est de classe $C^r$, les dérivées $D^s(f * G_n)$ tendent uniformément vers $D^s f$ pour $0 \leq s \leq r.*$
