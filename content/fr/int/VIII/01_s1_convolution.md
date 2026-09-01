---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 1
section_title: Convolution
lang: fr
source: int-vii-viii-fr
pdf_pages: 0119-0127
extraction: ocr
subsections:
    - "no": 1
      title: Définition et exemples.
      page: 0
      pdf_page: 119
    - "no": 2
      title: Associativité.
      page: 0
      pdf_page: 121
    - "no": 3
      title: Cas des mesures bornées.
      page: 0
      pdf_page: 124
    - "no": 4
      title: Propriétés concernant les supports.
      page: 0
      pdf_page: 125
    - "no": 5
      title: Expression vectorielle du produit de convolution.
      page: 0
      pdf_page: 126
statements: 15
exercises: 0
content_sha256: 2fda2cb240ee30046e4d7ca00b89fdab933693bce9e6decfa8ba3209e8ccf533
---

## § 1. Convolution.

### 1. Définition et exemples.

Rappelons (chap. V, § 6, nos 1 et 4 ; chap. VI, § 2, no 10) que, si X et Y sont des espaces localement compacts, $\mu$ une mesure sur X, et si $\varphi$ est une application de X dans Y, $\varphi$ est dite $\mu$-propre si : a) $\varphi$ est $\mu$-mesurable ; b) pour chaque partie compacte K de Y, $\pi^{-1}(K)$ est essentiellement $\mu$-intégrable. Alors la mesure image $\nu = \varphi(\mu)$ sur Y existe et possède la propriété suivante : pour qu'une fonction $f$ sur Y, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, soit essentiellement intégrable pour $\nu$, il faut et il suffit que $f \circ \varphi$ le soit pour $\mu$, et l'on a alors

$$
\int_Y f(y) d\nu(y) = \int_X f(\varphi(x)) d\mu(x).
$$

#### Définition 1 {#int-viii-s1-def-1 .statement}

Soient $X_1, \ldots, X_n$ des espaces localement compacts, $\mu_i$ une mesure sur $X_i$ ($1 \leq i \leq n$) ; soient X le produit des $X_i$, $\mu$ celui des $\mu_i$. Soit $\varphi$ une application de X dans un espace localement compact Y. On dit que la suite $(\mu_i)$ est $\varphi$-convolvable, ou que $\mu_1, \ldots, \mu_n$ sont $\varphi$-convolvables, si $\varphi$ est $\mu$-propre ; en ce cas, l'image $\nu = \varphi(\mu)$ de $\mu$ par $\varphi$ s'appelle le produit de convolution des $\mu_i$ pour $\varphi$, et se note $*_{\varphi}(\mu_i)_{1 \leq i \leq n}$, ou $\prod_{i=1}^n \mu_i$, ou $\mu_1 * \mu_2 * \ldots * \mu_n$.

Les deux dernières notations ne sont à employer, bien entendu, que lorsqu’il ne peut y avoir aucun doute sur φ.

Soit f une fonction sur Y, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Pour que f soit essentiellement intégrable pour $\mu_1 * \mu_2 * \ldots * \mu_n$, il faut et il suffit que la fonction

$$
(x_1, \ldots, x_n) \to f(\varphi(x_1, \ldots, x_n))
$$

soit essentiellement intégrable pour $\mu_1 \otimes \mu_2 \otimes \ldots \otimes \mu_n$, et l’on a alors

(1)
$$
\int f\, d(\mu_1 * \mu_2 * \ldots * \mu_n) = \int f(\varphi(x_1, \ldots, x_n)) d\mu_1(x_1) \ldots d\mu_n(x_n)
$$

formule qui peut être considérée comme définissant $\mu_1 * \ldots * \mu_n$ quand on y prend $f \in \mathcal{H}(Y)$.

Les définitions entraînent aussitôt que les $\mu_i$ sont convolables si et seulement si les $|\mu_i|$ le sont. On a alors

$$
|\varphi(\mu_1 \otimes \ldots \otimes \mu_n)| \leq \varphi(|\mu_1 \otimes \ldots \otimes \mu_n|) = \varphi(|\mu_1| \otimes \ldots \otimes |\mu_n|)
$$
(chap. VI, § 2, no 10), c’est-à-dire

(2)
$$
|\ast_i \mu_i| \leq \ast_i |\mu_i|.
$$

Si les $\mu_i$ sont convolables positives, et si $\nu_i$ est une mesure sur $X_i$; telle que $0 \leq \nu_i \leq \mu_i$, les $\nu_i$ sont convolables et

$$
\ast_i \nu_i \leq \ast_i \mu_i.
$$

Supposons $\mu_1, \mu_2, \ldots, \mu_n$ convolables, et $\mu'_1, \mu_2, \ldots, \mu_n$ convolables ($\mu'_1$ étant une mesure sur $X_1$). D’après le chap. V, § 6, no 3, prop. 6, $\mu_1 + \mu'_1, \mu_2, \ldots, \mu_n$ sont convolables et $(\mu_1 + \mu'_1) * \mu_2 * \ldots * \mu_n = \mu_1 * \mu_2 * \ldots * \mu_n + \mu'_1 * \mu_2 * \ldots * \mu_n$.

#### Exemple 1 {#int-viii-s1-n1-exa-1 .statement}

Pour $\varphi$ quelconque, les mesures $\varepsilon_{x_i}$, où $x_i \in X_i$ pour $1 \leq i \leq n$, sont toujours convolables et ont pour produit de convolution $\varepsilon_y$, avec $y = \varphi(x_1, x_2, \ldots, x_n)$. Par suite, si chacune des $\mu_i$ est à support fini, les $\mu_i$ sont convolables et $\mu_1 * \ldots * \mu_n$ est à support fini. En particulier, soit M un monoïde muni d’une topologie localement compacte ; si on prend pour $\varphi$ la loi de composition dans $M$, les mesures à support fini sur $M$ forment, pour la convolution, une algèbre qui n’est autre que l’algèbre du monoïde $M$ (sur $\mathbf{R}$, ou sur $\mathbf{C}$, suivant qu’on considère les mesures réelles ou complexes).

#### Exemple 2 {#int-viii-s1-n1-exa-2 .statement}

Soit $M$ un monoïde muni de la topologie discrète ; supposons que, pour tout $m \in M$, il n’y ait qu’un ensemble fini de couples $(m', m'') \in M \times M$ tels que $m'm'' = m$; cela revient à dire que la loi de composition dans $M$ est une application propre de $M \times M$ dans $M$; alors les mesures sur $M$ forment, pour la convolution, une algèbre qui n’est autre que l’algèbre large du monoïde $M$; signalons les deux cas suivants :

a) $M = \mathbf{N}$, la loi de composition étant l’addition. À toute mesure $\mu$ sur $\mathbf{N}$, associons la série formelle

$$
S(\mu) = \sum_{n=0}^{\infty} \mu(\{n\}) t^n
$$

en une indéterminée $t$. Alors $S(\mu * \mu') = S(\mu) S(\mu')$. Une remarque analogue s’applique aux séries formelles à un nombre quelconque d’indéterminées.

*b) $M = \mathbf{N}^*$, la loi de composition étant la multiplication. À toute mesure $\mu$ sur $\mathbf{N}^*$, associons la série de Dirichlet formelle

$$
D(\mu) = \sum_{n=1}^{\infty} \mu(\{n\}) n^{-s}.
$$

Alors $D(\mu * \mu') = D(\mu) D(\mu')$*

#### Exemple 3 {#int-viii-s1-n1-exa-3 .statement}

Soient $X, Y, Z$ des espaces localement compacts, $\varphi$ une application continue de $X \times Y$ dans $Z$. Si $x \in X$ et si $\mu$ est une mesure sur $Y$, dire que $\varepsilon_x$ et $\mu$ sont $\varphi$-convolables revient à dire que l’application $\varphi(x, .)$ de $Y$ dans $Z$ est $\mu$-propre. Et l’on a alors $\varepsilon_x * \mu = \varphi(x, .)(\mu)$.

### 2. Associativité.

Le lemme suivant complète la prop. 7 du chap. V, § 8, no 3 :

#### Lemme 1 {#int-viii-s1-lem-1 .statement}

Pour $1 \leq i \leq n$, soient $X_i, Y_i$ deux espaces localement compacts, $\mu_i$ une mesure sur $X_i$, $\varphi_i$ une application continue de $X_i$ dans $Y_i$. Soient $X = \prod_i X_i$, $Y = \prod_i Y_i$, $\mu = \bigotimes_i \mu_i$, et $\varphi$ l’application de $X$ dans $Y$, produit des $\varphi_i$. Si $\varphi$ est $\mu$-propre et si $\mu_i \neq 0$ pour tout $i$, les $\varphi_i$ sont $\mu_i$-propres et $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$.

On peut supposer les $\mu_i$ positives et $n = 2$. Soit $f_1 \in \mathcal{K}_+(Y_1)$. Puisque $\mu_2 \neq 0$, il existe $f_2 \in \mathcal{K}_+(Y_2)$ telle que $f_2 \circ \varphi_2$ ne soit pas $\mu_2$-négligeable. La fonction $(x_1, x_2) \to f_1(\varphi_1(x_1))f_2(\varphi_2(x_2))$ est essentiellement $\mu$-intégrable et continue, donc $\mu$-intégrable. Donc il existe $x_2 \in X_2$ tel que $f_2(\varphi_2(x_2)) \neq 0$ et que la fonction $x_1 \to f_1(\varphi_1(x_1))f_2(\varphi_2(x_2))$ soit $\mu_1$-intégrable. Donc $f_1 \circ \varphi_1$ est $\mu_1$-intégrable, ce qui prouve que $\varphi_1$ est $\mu_1$-propre. On raisonne de même pour $\varphi_2$. On a $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$ d’après la prop. 7 du chap. V, § 8, no 3.

Le lemme suivant complète la prop. 4 du chap. V, § 6, no 3.

#### Lemme 2 {#int-viii-s1-lem-2 .statement}

Soient $T, T', T''$ trois espaces localement compacts, $\mu$ une mesure sur $T$, $\pi$ une application $\mu$-mesurable de $T$ dans $T'$, $\pi'$ une application continue de $T'$ dans $T''$, et $\pi'' = \pi' \circ \pi$. Si $\pi''$ est $\mu$-propre, $\pi$ est $\mu$-propre, $\pi'$ est $\pi(\mu)$-propre, et $\pi''(\mu) = \pi'(\pi(\mu))$.

Soit $K'$ une partie compacte de $T'$. Alors $K'' = \pi'(K')$ est compact, donc ${\pi''}^{-1}(K'')$ est essentiellement $\mu$-intégrable, donc $\pi^{-1}(K') \subset {\pi''}^{-1}(K'')$ est essentiellement $\mu$-intégrable, de sorte que $\pi$ est $\mu$-propre. Alors $\pi'$ est $\pi(\mu)$-propre et $\pi''(\mu) = \pi'(\pi(\mu))$ d’après le chap. V, § 6, no 3, prop. 4.

#### Proposition 1 {#int-viii-s1-prop-1 .statement}

Soient $X_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq n_i$), $Y_i$ ($1 \leq i \leq m$), $Z$ des espaces localement compacts ; pour chaque $i$, soit $\varphi_i$ une application de $X_i = \prod_j X_{ij}$ dans $Y_i$ ; soit $\varphi$ l’application de $X = \prod_i X_i$ dans $Y = \prod_i Y_i$, produit des $\varphi_i$ ; soit $\psi$ une application de $Y$ dans $Z$.

(i) Soient $\mu_{ij}$ des mesures respectivement données sur les $X_{ij}$, telles que, pour chaque $i$, les $\mu_{ij}$ ($1 \leq j \leq n_i$) soient $\varphi_i$-convolables et que les mesures $*_{i} |\mu_{ij}|$ soient $\psi$-convolables ; alors les $\mu_{ij}$, pour $1 \leq i \leq m, 1 \leq j \leq n_i$, sont $(\psi \circ \varphi)$-convolables et l’on a

$$
*_{i,j} \mu_{ij} = *_{i} (*_{j} \mu_{ij}).
$$

(ii) Supposons $\psi$ et les $\varphi_i$ continues, et soient $\mu_{ij}$ des mesures toutes $\neq 0$, respectivement données sur les $X_{ij}$, et $(\psi \circ \varphi)$-convolables ; alors, pour chaque $i$, les $\mu_{ij}$ ($1 \leq j \leq n_i$) sont $\varphi_i$-convolables, les mesures $*_{i} |\mu_{ij}|$ sont $\psi$-convolables, et l’on a la formule (3).

Il suffit d’envisager le cas où toutes les mesures considérées sont $\geq 0$.

Plaçons-nous dans les hypothèses de (i). L’application $\varphi$ est propre pour $\bigotimes_{i,j} \mu_{ij}$ et $\varphi(\bigotimes_{i,j} \mu_{ij}) = \bigotimes_{i} \varphi_i(\bigotimes_{j} \mu_{ij}) = \bigotimes_{i} (*_{j} \mu_{ij})$ (chap. V, § 8, prop. 7). L’application $\psi \circ \varphi$ est propre pour $\bigotimes_{i,j} \mu_{ij}$ et $(\psi \circ \varphi)(\bigotimes_{i,j} \mu_{ij}) = \psi(\bigotimes_{i} (*_{j} \mu_{ij})) = *_{i} (*_{j} \mu_{ij})$ (chap. V, § 6, prop. 4). Donc les $\mu_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq n_i$) sont $(\psi \circ \varphi)$-convolables et l’on a la formule (3).

Plaçons-nous dans les hypothèses de (ii). Le lemme 2 prouve d’abord que $\varphi$ est propre pour $\bigotimes_{i,j} \mu_{ij}$. Le lemme 1 prouve alors que, pour tout $i$, $\varphi_i$ est propre pour $\bigotimes_{j} \mu_{ij}$ et que

$$
\varphi(\bigotimes_{i,j} \mu_{ij}) = \bigotimes_{i} (*_{j} \mu_{ij}).
$$

D’après le lemme 2, $\psi$ est propre pour $\bigotimes_{i} (*_{j} \mu_{ij})$. D’où la proposition.

#### Corollaire {#int-viii-s1-n2-cor-1 .statement}

Soient $X_i, X'_i$ ($1 \leq i \leq n$), Y, $Y'$ des espaces localement compacts ; soient $\varphi, \varphi'$ des applications continues de $X = \prod_i X_i$ dans $Y$ et de $X' = \prod_i X'_i$ dans $Y'$, respectivement ; soient $f_i$ des applications continues de $X_i$ dans $X'_i$ ($1 \leq i \leq n$) et $g$ une application continue de $Y$ dans $Y'$, telles que $\varphi' \circ f = g \circ \varphi$, $f$ étant l’application de $X$ dans $X'$ produit des $f_i$. Soient $\mu_i$ des mesures respectivement données sur les $X_i$ et toutes $\neq 0$. Alors les deux assertions suivantes sont équivalentes :

(i) $f_i$ est $\mu_i$-propre pour tout $i$, et les mesures $f_i(|\mu_i|)$ sont $\varphi'$-convolables ;

(ii) les $\mu_i$ sont $\varphi$-convolables, et $g$ est propre pour $*_{\varphi}(|\mu_i|)$.
De plus, lorsque ces assertions sont vérifiées, on a

(4)
$$
*_{\varphi'}(f_i(\mu_i)) = g(*_{\varphi}\mu_i) = *_{g \circ \varphi}(\mu_i).
$$

En effet, soit $h = \varphi' \circ f = g \circ \varphi$. D’après la prop. 1, les conditions (i) et (ii) sont chacune équivalentes à la condition suivante :
(iii) les $\mu_i$ sont $h$-convolables.
S’il en est ainsi, on a
$$
*_{\varphi'}(f_i(\mu_i)) = *_h \mu_i = g(*_{\varphi}\mu_i).
$$

### 3. Cas des mesures bornées.

#### Proposition 2 {#int-viii-s1-prop-2 .statement}

Soient $X_1, \ldots, X_n, Y$ des espaces localement compacts, $\mu_i$ une mesure bornée sur $X_i$ ($1 \leq i \leq n$), $\mu$ le produit des $\mu_i$, $\varphi$ une application $\mu$-mesurable de $\prod_i X_i$ dans $Y$.
Alors les $\mu_i$ sont $\varphi$-convolables et $\| *_{i=1}^n \mu_i \| \leq \prod_{i=1}^n \| \mu_i \|$. Si les $\mu_i$ sont en outre positives, on a $\| *_{i=1}^n \mu_i \| = \prod_{i=1}^n \| \mu_i \|$.

En effet, $\mu'_i = |\mu_i|$ est bornée et $\| \mu'_i \| = \| \mu_i \|$ (chap. VI, § 2, no 9, prop. 13). On a $|\mu_1 \otimes \ldots \otimes \mu_n| = \mu'_1 \otimes \ldots \otimes \mu'_n$ (chap. VI, § 2, no 10), donc $\mu_1 \otimes \ldots \otimes \mu_n$ est bornée et
$$
\| \mu_1 \otimes \ldots \otimes \mu_n \| = \| \mu_1 \| \ldots \| \mu_n \|
$$
(chap. V, § 8, no 2, cor. 6 de la prop. 5). Donc $\varphi$ est $\mu$-propre (chap. V, § 6, no 1, Remarque 1), c’est-à-dire que les $\mu_i$ sont $\varphi$-convolables. On a $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \otimes \ldots \otimes \mu'_n \|$ (chap. V, § 6, no 2, th. 1) et par suite $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \| \ldots \| \mu'_n \|$. Enfin,
$$
| *_{i} \mu_i | \leq *_{i} \mu'_i \text{ (no 1, formule (2))},
$$
donc

$$
\| * \mu_i \| \leq \| * \mu'_i \| = \prod_{i=1}^n \| \mu_i \|.
$$

#### Proposition 3 {#int-viii-s1-prop-3 .statement}

*Soient $X_1, \ldots, X_n, Y$ des espaces localement compacts, $\varphi$ une application continue de $\prod_{i=1}^n X_i$ dans $Y$. Alors l’application $(\mu_1, \ldots, \mu_n) \to *_{\varphi} \mu_i$ de $\prod_{i=1}^n \mathcal{M}^1(X_i)$ dans $\mathcal{M}^1(Y)$ est multilinéaire continue.*

Ceci résulte de la prop. 2 et de ce qu’on a dit au no 1.

### 4. Propriétés concernant les supports.

#### Proposition 4 {#int-viii-s1-prop-4 .statement}

*Soient $X_1, \ldots, X_n, Y$ des espaces localement compacts, $\mu_i$ une mesure sur $X_i$ ($1 \leq i \leq n$), $S_i$ son support, $\varphi$ une application continue de $\prod_i X_i$ dans $Y$ telle que la restriction de $\varphi$ à $\prod_i S_i$ soit propre. Alors les $\mu_i$ sont $\varphi$-convolables.*

En effet, soit $K$ une partie compacte de $Y$. Le support de $\mu = \mu_1 \otimes \ldots \otimes \mu_n$ est $S = \prod_i S_i$ (chap. III, § 5, no 2, prop. 2).

Donc $\varphi^{-1}(K) \cap \left( \prod_i X_i - S \right)$ est $\mu$-négligeable. D’autre part, $\varphi^{-1}(K) \cap S$ est compact. Donc $\varphi^{-1}(K)$ est $\mu$-intégrable.

#### Proposition 5 {#int-viii-s1-prop-5 .statement}

*Soient $X_1, \ldots, X_n, Y$ des espaces localement compacts, $\mu_i$ une mesure sur $X_i$ ($1 \leq i \leq n$), $\mu$ le produit des $\mu_i$, $\varphi$ une application $\mu$-propre de $\prod_i X_i$ dans $Y$, et $S_i$ le support de $\mu_i$.

a) *Le support de $* \mu_i$ est contenu dans l’adhérence de $\varphi \left( \prod_i S_i \right)$.*

b) *Si $\varphi$ est continue et si les $\mu_i$ sont positives, le support de $* \mu_i$ est l’adhérence de $\varphi \left( \prod_i S_i \right)$.*

Soit $S = \prod_i S_i$ le support de $\mu$. Le support de $* \mu_i$ est contenu dans $\overline{\varphi(S)}$ d’après le chap. V, § 6, no 2, cor. 3 de la prop. 2.

n° 1

Si $\varphi$ est continue et si les $\mu_i$ sont positives, le support de $*_{i} \mu_i$ est $\overline{\varphi(S)}$ (loc. cit., cor. 4 de la prop. 2).

#### Corollaire {#int-viii-s1-n4-cor-1 .statement}

Si $\varphi$ est continue, et si les $\mu_i$ sont à support compact, les $\mu_i$ sont convolables et $*_{i} \mu_i$ est à support compact.

### 5. Expression vectorielle du produit de convolution.

#### Proposition 6 {#int-viii-s1-prop-6 .statement}

Soient $X, Y, Z$ des espaces localement compacts, $\varphi$ une application continue de $X \times Y$ dans $Z$, et $\lambda, \mu$ des mesures sur $X, Y$. Pour que $\lambda$ et $\mu$ soient $\varphi$-convolables, il faut et il suffit que l’application $(x, y) \to \varepsilon_{\varphi(x, y)} = \varepsilon_x * \varepsilon_y$ de $X \times Y$ dans $\mathcal{M}(Z)$ soit scalairement $(\lambda \otimes \mu)$-intégrable pour la topologie $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, et l’on a alors

$$
\lambda * \mu = \int_{X \times Y} (\varepsilon_x * \varepsilon_y) d\lambda(x) d\mu(y).
$$

Dire que $\lambda$ et $\mu$ sont $\varphi$-convolables signifie que, pour toute $f \in \mathcal{K}(Z)$, $f \circ \varphi$ est $(\lambda \otimes \mu)$-intégrable, c’est-à-dire que, pour toute $f \in \mathcal{K}(Z)$, la fonction $(x, y) \to \langle f, \varepsilon_{\varphi(x, y)} \rangle$ est $(\lambda \otimes \mu)$-intégrable, c’est-à-dire encore que l’application $(x, y) \to \varepsilon_{\varphi(x, y)}$ de $X \times Y$ dans $\mathcal{M}(Z)$ est scalairement $(\lambda \otimes \mu)$-intégrable pour $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. S’il en est ainsi, on a

$$
\langle \lambda * \mu, f \rangle = \int f(\varphi(x, y)) d\lambda(x) d\mu(y) = \int_{X \times Y} \langle \varepsilon_{\varphi(x, y)}, f \rangle d\lambda(x) d\mu(y),
$$

d’où $\lambda * \mu = \int_{X \times Y} \varepsilon_{\varphi(x, y)} d\lambda(x) d\mu(y)$.

#### Proposition 7 {#int-viii-s1-prop-7 .statement}

Soient $X, Y, Z$ des espaces localement compacts, $\varphi$ une application continue de $X \times Y$ dans $Z$, et $\lambda, \mu$ des mesures sur $X, Y$. On suppose que, pour tout $x \in X$, $\varepsilon_x$ et $\mu$ sont $\varphi$-convolables. Pour que $\lambda$ et $\mu$ soient $\varphi$-convolables, il faut et il suffit que l’application $x \to \varepsilon_x * |\mu|$ de $X$ dans $\mathcal{M}(Z)$ soit scalairement $\lambda$-intégrable pour la topologie $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, et l’on a alors $\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$.

Supposons que $\lambda$ et $\mu$ soient $\varphi$-convolables. Pour toute $f \in \mathcal{K}(Z)$, $f \circ \varphi$ est $(|\lambda| \otimes |\mu|)$-intégrable, donc la fonction $x \to \int_Y f(\varphi(x,y))d|\mu|(y) = \langle f, \varepsilon_x * |\mu| \rangle$ (qui par hypothèse est définie pour tout $x \in X$) est $\lambda$-intégrable; donc $x \to \varepsilon_x * |\mu|$ est scalairement $\lambda$-intégrable pour $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, et l’on a

$$
\langle f, \lambda * \mu \rangle = \int_X d\lambda(x) \int_Y f(\varphi(x,y))d\mu(y) = \int_X \langle f, \varepsilon_x * \mu \rangle d\lambda(x),
$$

d’où $\lambda * \mu = \int_X (\varepsilon_x * \mu)d\lambda(x)$. Réciproquement, supposons que l’application $x \to \varepsilon_x * |\mu|$ de $X$ dans $\mathcal{M}(Z)$ soit scalairement $\lambda$-intégrable pour $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. Soit $f \in \mathcal{K}_+(Z)$. Alors la fonction $(x, y) \to f(\varphi(x, y))$ est continue et l’on a (chap. V, § 8, prop. 1)

$$
\iint^* f(\varphi(x, y))\ d|\lambda|(x)d|\mu|(y) = \int^* d|\lambda|(x) \int^* f(\varphi(x, y))d|\mu|(y)
$$
$$
= \int^* \langle f, \varepsilon_x * |\mu| \rangle d|\lambda|(x) < +\infty.
$$

Donc $f \circ \varphi$ est $(\lambda \otimes \mu)$-intégrable, de sorte que $\lambda$ et $\mu$ sont $\varphi$-convolables.
