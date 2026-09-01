---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 3
section_title: Convolution des mesures sur les groupes
lang: fr
source: int-vii-viii-fr
pdf_pages: 0139-0147, 0191-0205
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres de mesures.
      page: 0
      pdf_page: 139
    - "no": 2
      title: Cas d’un groupe opérant dans un espace.
      page: 0
      pdf_page: 143
    - "no": 3
      title: Convolution et représentations linéaires.
      page: 0
      pdf_page: 144
statements: 17
exercises: 28
content_sha256: ffd68731804fc84a7304dfbcffafa38d713f3e4132092ee65ad0d122f18fe0d9
---

## § 3. Convolution des mesures sur les groupes.

### 1. Algèbres de mesures.

Soit $G$ un groupe localement compact. Il sera entendu une fois pour toutes que des mesures $\mu_1, \ldots, \mu_n$ sur $G$ sont dites convolables si elles le sont pour l’application

$$
(x_1, x_2, \ldots, x_n) \to x_1 x_2 \ldots x_n ;
$$

et c’est au moyen de cette application qu’on prendra toujours le produit de convolution $*_{i} \mu_i$. Si $s \in G, t \in G$, on a

(1)
$$
\varepsilon_s * \varepsilon_t = \varepsilon_{st}.
$$
Si $s \in G$ et $\mu \in \mathcal{M}(G)$, on a
(2)
$$
\varepsilon_s * \mu = \gamma(s) \mu
$$
(3)
$$
\mu * \varepsilon_s = \delta(s^{-1}) \mu
$$
d’après le § 1, n° 1, exemple 3. Si $G$ est commutatif, dire que $\mu_1$ et $\mu_2$ sont convolables équivaut à dire que $\mu_2$ et $\mu_1$ sont convolables, et l’on a alors $\mu_1 * \mu_2 = \mu_2 * \mu_1$. Si $G$ n’est pas commutatif, il peut arriver que $\mu_1$ et $\mu_2$ soient convolables, sans que $\mu_2$ et $\mu_1$ le soient (exerc. 12).

#### Proposition 1 {#int-viii-s3-prop-1 .statement}

Soient $G$ un groupe localement compact, $\lambda, \mu, \nu$ des mesures $\neq 0$ sur $G$.
(i) Si $\lambda, \mu, \nu$ sont convolables, il en est de même de $\lambda$ et $\mu$, de $|\lambda| * |\mu|$ et $\nu$, de $\mu$ et $\nu$, de $\lambda$ et $|\mu| * |\nu|$, et l’on a
$$
\lambda * \mu * \nu = (\lambda * \mu) * \nu = \lambda * (\mu * \nu).
$$

(ii) Si $\lambda$ et $\mu$ sont convolables, ainsi que $|\lambda| * |\mu|$ et $\nu$, alors $\lambda, \mu, \nu$ sont convolables. De même si $\mu$ et $\nu$ sont convolables ainsi que $\lambda$ et $|\mu| * |\nu|$.

Ceci résulte de la prop. 1 du § 1, n° 2.

Il peut exister des mesures $\lambda, \mu, \nu$ sur $G$ telles que les produits de convolution $\lambda * \mu, (\lambda * \mu) * \nu, \mu * \nu, \lambda * (\mu * \nu)$ soient tous définis, et que cependant $(\lambda * \mu) * \nu \neq \lambda * (\mu * \nu)$ (cf. exerc. 4).

Soit $\rho$ une fonction $> 0$ finie semi-continue inférieurement sur $G$ telle que $\rho(st) \leq \rho(s)\rho(t)$ quels que soient $s, t$ dans $G$. On notera $\mathcal{M}^\rho(G)$ l'espace vectoriel des mesures $\lambda$ sur $G$ telles que $\rho$ soit $\lambda$-intégrable, et $||\lambda||_\rho$ (ou simplement $||\lambda||$) la norme $\int_G \rho(s)d|\lambda|(s)$ sur cet espace. Pour $\rho = 1$, on retrouve l'ensemble $\mathcal{M}^1(G)$ des mesures bornées sur $G$.

#### Proposition 2 {#int-viii-s3-prop-2 .statement}

(i) Deux éléments quelconques de $\mathcal{M}^\rho(G)$ sont convolables.

(ii) Pour la convolution, et pour la norme $||\lambda||$, $\mathcal{M}^\rho(G)$ est une algèbre normée complète admettant l'élément unité $\varepsilon_e$.

(iii) $C'(G)$ est une sous-algèbre de $\mathcal{M}^\rho(G)$.

Soient $\lambda, \mu$ dans $\mathcal{M}^\rho(G)$, et montrons que $\lambda$ et $\mu$ sont convolables. Soit $f \in \mathcal{K}_+(G)$. Comme $\rho$ est $> 0$ et semi-continue inférieurement, il existe une constante $k > 0$ telle que $f \leq k\rho$. On a alors

$$
\int^* f(st)d|\lambda|(s)d|\mu|(t) \leq k \int^* \rho(st)d|\lambda|(s)d|\mu|(t)
$$
$$
\leq k \int^* \rho(s)\rho(t)d|\lambda|(s)d|\mu|(t)
$$
$$
= k \left( \int^* \rho(s)d|\lambda|(s) \right) \left( \int^* \rho(t)d|\mu|(t) \right)
$$

(chap. V, § 8, n° 2, prop. 5). Donc $f$ est $(\lambda \otimes \mu)$-intégrable, de sorte que $\lambda$ et $\mu$ sont convolables. D'autre part, en utilisant le chap. V (§ 2, prop. 2, § 6, prop. 2, § 8, prop. 5) et le fait que $(s, t) \to \rho(s)\rho(t)$ est semi-continue inférieurement dans $G \times G$, on a
$$
\int_G^* \rho(s)d|\lambda * \mu|(s) = \int_G^-* \rho(s)d|\lambda * \mu|(s)
$$
$$
\leq \int_{G \times G}^-* \rho(st)d|\lambda|(s)d|\mu|(t) \leq \int_{G \times G}^-* \rho(s)\rho(t)d|\lambda|(s)d|\mu|(t)
$$
$$
= \int_{G \times G}^* \rho(s)\rho(t)d|\lambda|(s)d|\mu|(t) = ||\lambda||.||\mu||.
$$
On voit que $\lambda * \mu \in \mathcal{M}^o(G)$ et que $||\lambda * \mu|| \leq ||\lambda||.||\mu||$. Compte tenu de la prop. 1, $\mathcal{M}^o(G)$ est une algèbre. L’application $\lambda \to \rho.\lambda$ est une application linéaire isométrique $\theta$ de $\mathcal{M}^o(G)$ dans $\mathcal{M}^1(G)$; si $\mu \in \mathcal{M}^1(G)$, $1/\rho$, qui est localement bornée et semi-continue supérieurement, est localement $\mu$-intégrable, et $\rho$ est $(1/\rho)$.$\mu$-intégrable, donc $(1/\rho).\mu \in \mathcal{M}^o(G)$; ceci prouve que $\theta$ est surjective; donc $\mathcal{M}^o(G)$ est une algèbre normée complète. Enfin, il est clair que $\varepsilon_e$ est élément unité de $\mathcal{M}^o(G)$ et que $\mathcal{C}'(G)$ est une sous-algèbre de $\mathcal{M}^o(G)$ (§ 1, no 4, cor. de la prop. 5).

Si $\rho = 1$, la prop. 2, (i) et (ii), résulte aussi du § 1, prop. 2.

#### Proposition 3 {#int-viii-s3-prop-3 .statement}

*Soient $\mu_1, \ldots, \mu_n$ des mesures sur $G$. Si toutes les $\mu_i$, sauf une au plus, sont à support compact, alors les $\mu_i$ sont convolables.*

En effet, soit $S_i$ le support de $\mu_i$, et supposons $S_i$ compact pour $i \neq i_0$. Soit $K$ une partie compacte de $G$. L’ensemble des $(x_1, \ldots, x_n) \in \prod_i S_i$ tels que $x_1 x_2 \ldots x_n \in K$ est compact, car les conditions $x_i \in S_i$ pour tout $i$, $x_1 x_2 \ldots x_n \in K$ impliquent
$$
x_{i_0} \in S_{i_0-1}^{-1} \ldots S_1^{-1} K S_n^{-1} \ldots S_{i_0+1}^{-1}.
$$
Donc les $\mu_i$ sont convolables (§ 1, no 4, prop. 4).

#### Proposition 4 {#int-viii-s3-prop-4 .statement}

*L’application $(\lambda, \mu) \to \lambda * \mu$ (resp. $(\lambda, \mu) \to \mu * \lambda$) où $\lambda \in \mathcal{C}'(G)$, $\mu \in \mathcal{M}(G)$, définit sur $\mathcal{M}(G)$ une structure de module à gauche (resp. à droite) sur l’algèbre $\mathcal{C}'(G)$*.

Ceci résulte des prop. 1 et 3.

#### Proposition 5 {#int-viii-s3-prop-5 .statement}

Soient $\lambda$ une mesure de Haar à gauche (resp. à droite) sur $G$, et $\mu \in \mathcal{M}^1(G)$. Alors $\mu$ et $\lambda$ (resp. $\lambda$ et $\mu$) sont convolables, et $\mu * \lambda = \| \mu \| \lambda$ (resp. $\lambda * \mu = \| \mu \| \lambda$).

On peut supposer $\mu \geqslant 0$. Soit $f \in \mathcal{K}_+(G)$. Lorsque $\lambda$ est une mesure de Haar à gauche, on a

$$
\int^* d\mu(x) \int^* f(xy) d\lambda(y) = \int^* d\mu(x) \int f(y) d\lambda(y) = \lambda(f) \| \mu \|
$$

donc la fonction $(x, y) \to f(xy)$ est $(\mu \otimes \lambda)$-intégrable, et son intégrale pour $\mu \otimes \lambda$ est $\lambda(f) \| \mu \|$. On raisonne de même quand $\lambda$ est une mesure de Haar à droite.

#### Proposition 6 {#int-viii-s3-prop-6 .statement}

Soient $\mu$ et $\nu$ deux mesures convolables sur $G$. Soit $\chi$ une représentation continue de $G$ dans $\mathbf{C}^*$. Alors $\chi . \mu$ et $\chi . \nu$ sont convolables et $(\chi . \mu) * (\chi . \nu) = \chi . (\mu * \nu)$.

Soit $f \in \mathcal{K}(G)$. Alors $f \chi \in \mathcal{K}(G)$, donc la fonction

$$
(x, y) \to f(xy) \chi(xy) = f(xy) \chi(x) \chi(y)
$$

sur $G \times G$ est intégrable pour $\mu \otimes \nu$; donc la fonction $(x, y) \to f(xy)$ est intégrable pour $(\chi . \mu) \otimes (\chi . \nu)$; donc $\chi . \mu$ et $\chi . \nu$ sont convolables. En outre,

$$
\langle \chi . \mu * \chi . \nu, f \rangle = \int f(xy) \chi(x) \chi(y) d\mu(x) d\nu(y)
$$
$$
= \int (f \chi)(xy) d\mu(x) d\nu(y) = \langle \mu * \nu, \chi f \rangle
$$

d'où $(\chi . \mu) * (\chi . \nu) = \chi . (\mu * \nu)$.

#### Proposition 7 {#int-viii-s3-prop-7 .statement}

Soient $G$ et $G'$ deux groupes localement compacts, $u$ une représentation continue de $G$ dans $G'$, $\mu_1, \ldots, \mu_n$ des mesures sur $G$, toutes $\neq 0$. Alors les assertions suivantes sont équivalentes :

(i) $u$ est $\mu_i$-propre pour tout $i$, et les mesures $u(|\mu_i|)$ sont convolables ;
(ii) les $\mu_i$ sont convolables et $u$ est propre pour $*_{i}(|\mu_i|)$.

Lorsque ces conditions sont vérifiées, on a

$$
*_{i} u(\mu_i) = u(*_{i} \mu_i).
$$

#### Corollaire {#int-viii-s3-n1-cor-1 .statement}

Soient G un groupe localement compact, $\mu_1, \ldots, \mu_n$ des mesures sur G. Pour que la suite $(\mu_i)_{1 \leq i \leq n}$ soit convolvable, il faut et il suffit que la suite $(\check{\mu}_{n-i})_{0 \leq i \leq n-1}$ le soit, et l’on a alors $(\mu_1 * \ldots * \mu_n)^{\vee} = \check{\mu}_n * \ldots * \check{\mu}_1$.

Ceci résulte de la prop. 7 en considérant l’isomorphisme $x \to x^{-1}$ de G sur le groupe opposé.

### 2. Cas d’un groupe opérant dans un espace.

Soit X un espace localement compact sur lequel un groupe localement compact G opère à gauche continûment par
$$
(s, x) \to s.x.
$$
Si $\mu_1, \ldots, \mu_n$ sont des mesures sur G et $\nu$ une mesure sur X, celles-ci seront dites convolvables si elles le sont pour l’application $(s_1, \ldots, s_n, x) \to s_1 \ldots s_n x$ de $G^n \times X$ dans X, et leur produit de convolution devra s’entendre au sens de cette application.

Si $s \in G$ et $x \in X$, on a
$$
\varepsilon_s * \varepsilon_x = \varepsilon_{sx}.
$$
Si $s \in G$ et $\mu \in \mathcal{M}(X)$, on a
$$
\varepsilon_s * \mu = \gamma(s)\mu
$$
d’après le § 1, no 1, exemple 3.

#### Proposition 8 {#int-viii-s3-prop-8 .statement}

Soient $\mu$ une mesure sur G, $\nu$ une mesure sur X.
(i) Si $\mu$ est à support compact, $\mu$ et $\nu$ sont convolvables.
(ii) Si $\nu$ est à support compact, et si G opère proprement dans X, $\mu$ et $\nu$ sont convolvables.
Ceci résulte de la prop. 4 du § 1, no 4.

#### Proposition 9 {#int-viii-s3-prop-9 .statement}

Pour la convolution, $\mathcal{M}^1(X)$ est un module à gauche sur $\mathcal{M}^1(G)$, $\mathcal{M}(X)$ et $\mathcal{C}'(X)$ sont des modules à gauche sur $\mathcal{C}'(G)$.

Ceci résulte de la prop. 8, et du § 1, prop. 1, 3, et cor. de la prop. 5.

#### Proposition 10 {#int-viii-s3-prop-10 .statement}

Soient $\mu$ une mesure sur G, $\nu$ une mesure sur X, $\mu$ et $\nu$ étant convolables. Supposons de plus qu’il existe une mesure positive $\beta$ sur X telle que $\gamma(s)\nu$ soit de base $\beta$ quel que soit $s \in G$. Alors $\mu * \nu$ est de base $\beta$.

Soit K une partie compacte $\beta$-négligeable de X. Alors K est $\gamma(s)|\nu|$-négligeable pour tout $s \in G$. Or

$$
|\mu| * |\nu| = \int_G (\varepsilon_s * |\nu|) d|\mu|(s)
$$

(§ 1, n° 5, prop. 7), et l’application $s \to \varepsilon_s * |\nu|$ est vaguement continue (§ 2, prop. 6). Donc K est $|\mu| * |\nu|$-négligeable d’après le chap. V, § 3, n° 4, th. 1. Donc $|\mu| * |\nu|$ est de base $\beta$ (chap. V, § 5, n° 5, Remarque).

### 3. Convolution et représentations linéaires.

#### Proposition 11 {#int-viii-s3-prop-11 .statement}

Soient G un groupe localement compact, E un espace localement convexe quasi-complet, U une représentation continue de G dans E.

(i) Si $\lambda \in \mathcal{C}'(G)$, $\mu \in \mathcal{C}'(G)$, on a $U(\lambda * \mu) = U(\lambda)U(\mu)$.

(ii) Supposons que E soit un espace de Banach, et soit $\rho(s) = \|U(s)\|$ pour $s \in G$. Si $\lambda \in \mathcal{M}^\circ(G)$, $\mu \in \mathcal{M}^\circ(G)$, on a $U(\lambda * \mu) = U(\lambda)U(\mu)$.

Soient $\lambda, \mu$ dans $\mathcal{C}'(G)$. Quel que soit $x \in E$, on a, en appliquant notamment les prop. 1 et 4 du chap. VI, § 1, n° 1

$$
U(\lambda * \mu)x = \int_G U(s)x\ d(\lambda * \mu)(s)
$$
$$
= \int_{G \times G} U(st)x\ d\lambda(s)d\mu(t) = \int_{G \times G} U(s)U(t)x\ d\lambda(s)d\mu(t)
$$
$$
= \int_G U(\lambda)U(t)x\ d\mu(t) = U(\lambda) \int_G U(t)x\ d\mu(t) = U(\lambda)U(\mu)x
$$

d’où (i). Un raisonnement analogue s’applique dans le cas (ii).

Soit toujours G un groupe localement compact, et supposons que G opère continûment à gauche dans un espace localement compact X. Ceci définit (§ 2, n° 4) une représentation linéaire continue $\gamma$ de G dans $\mathcal{M}(X)$ (muni de la topologie de la convergence compacte dans $\mathcal{K}(X)$).

#### Proposition 12 {#int-viii-s3-prop-12 .statement}

Si $\lambda \in \mathcal{C}'(G)$ et $\mu \in \mathcal{M}(X)$, on a

$$
\gamma(\lambda)\mu = \lambda * \mu.
$$

D’après la prop. 7 du § 1, n° 5, on a

$$
\lambda * \mu = \int_G (\varepsilon_s * \mu) d\lambda(s).
$$

Or $\varepsilon_s * \mu = \gamma(s)\mu$ (n° 2, formule (5)), et

$$
\int_G (\gamma(s)\mu) d\lambda(s) = \gamma(\lambda)\mu
$$

par définition de $\gamma(\lambda)$.

#### Corollaire {#int-viii-s3-n3-cor-1 .statement}

L’application $(\lambda, \mu) \to \lambda * \mu$ de $\mathcal{C}'(G) \times \mathcal{M}(X)$ dans $\mathcal{M}(X)$ est hypocontinue relativement aux parties équicontinues de $\mathcal{C}'(G)$ et aux parties compactes de $\mathcal{M}(X)$ ($\mathcal{C}'(G)$ et $\mathcal{M}(X)$ étant respectivement munis de la topologie de la convergence compacte dans $\mathcal{C}(G)$ et $\mathcal{K}(X)$).

En effet, $\mathcal{M}(X)$, muni de la topologie de la convergence compacte dans $\mathcal{K}(X)$, est quasi-complet. Donc l’application $(\lambda, \mu) \to \gamma(\lambda)\mu$ de $\mathcal{C}'(G) \times \mathcal{M}(X)$ dans $\mathcal{M}(X)$ est hypocontinue relativement aux parties équicontinues de $\mathcal{C}'(G)$ et aux parties compactes de $\mathcal{M}(X)$ (§ 2, n° 6). Il suffit alors d’appliquer la prop. 12.

#### Remarque 1 {#int-viii-s3-n3-rem-1 .statement}

Soit $\lambda_0 \in \mathcal{C}'(G)$. L’application $\mu \to \lambda_0 * \mu$ de $\mathcal{M}(X)$ dans $\mathcal{M}(X)$ est vaguement continue. En effet, soit $f \in \mathcal{K}(X)$. On a $\langle \lambda_0 * \mu, f \rangle = \int f(sx)d\lambda_0(s)d\mu(x) = \langle \mu, g \rangle$ en posant $g(x) = \int f(sx)d\lambda_0(s)$. Or $g$ est continue (chap. VII, § 1, no 1, lemme 1). D’autre part, soient S le support de $\lambda_0$ et K celui de $f$. Les conditions $sx \in K$ et $s \in S$ entraînent $x \in S^{-1}K$; donc le support de $g$ est contenu dans $S^{-1}K$, de sorte que $g \in \mathcal{K}(X)$. Alors $\langle \lambda_0 * \mu, f \rangle = \langle \mu, g \rangle$ est fonction vaguement continue de $\mu$, ce qui prouve notre assertion.

#### Remarque 2 {#int-viii-s3-n3-rem-2 .statement}

Soit $\mu_0 \in \mathcal{M}(X)$. L’application $\lambda \to \lambda * \mu_0$ de $\mathcal{C}'(G)$ dans $\mathcal{M}(X)$ est continue pour les topologies $\sigma(\mathcal{C}'(G), \mathcal{C}(G))$ et $\sigma(\mathcal{M}(X), \mathcal{K}(X))$. En effet, soit $f \in \mathcal{K}(X)$. On a $\langle f, \lambda * \mu_0 \rangle = \langle h, \lambda \rangle$, en posant $h(s) = \int f(sx)d\mu_0(x)$, et l’on a $h \in \mathcal{C}(G)$ (chap. VII, § 1, no 1, lemme 1).

#### Proposition 13 {#int-viii-s3-prop-13 .statement}

L’application $(s, \mu) \to \gamma(s)\mu$ de $G \times \mathcal{M}_+(X)$ dans $\mathcal{M}_+(X)$ est continue lorsque l’ensemble $\mathcal{M}_+(X)$ des mesures positives sur $X$ est muni de la topologie vague.

Comme $\gamma(s)\mu = \gamma(ss_0^{-1})\gamma(s_0)\mu$, il résulte de la Remarque 1 qu’il suffit de prouver la continuité de l’application considérée en un point de la forme $(e, \mu_0)$ avec $\mu_0 \in \mathcal{M}_+(X)$. Etant donnés une fonction $f \in \mathcal{K}(X)$ et un nombre $\varepsilon > 0$, il s’agit donc de montrer qu’il existe un voisinage U de $e$ dans $G$ et un voisinage W de $\mu_0$ dans $\mathcal{M}_+(X)$ tels que les relations $s \in U, \mu \in W$ entraînent

$$
\left| \int f(sx)d\mu(x) - \int f(x)d\mu_0(x) \right| \leq \varepsilon.
$$

Soit V un voisinage compact du support K de $f$ dans X, et soit $\varphi \in \mathcal{K}_+(X)$ telle que $\varphi(x) = 1$ dans V ; il existe un voisinage $W_0$ de $\mu_0$ dans $\mathcal{M}_+(X)$ tel que $a = \sup_{\mu \in W_0} \mu(V)$ soit fini : il suffit de prendre pour $W_0$ l’ensemble des $\mu \in \mathcal{M}_+(X)$ telles que $|\langle \varphi, \mu - \mu_0 \rangle| \leq 1$. Comme l’application $(s, x) \to sx$ est continue, il y a d'autre part un voisinage compact $U_0$ de $e$ dans $G$ tel que $sK \subset V$ pour tout $s \in U_0$; la fonction $(s, x) \to f(sx)$ est alors uniformément continue dans $U_0 \times V$ et il y a donc un voisinage $U \subset U_0$ de $e$ tel que $|f(sx) - f(x)| \leq \varepsilon/2a$ pour tout $s \in U$ et tout $x \in V$. Pour $s \in U$ et $\mu \in W_0$, on a donc

$$
\left| \int f(sx)d\mu(x) - \int f(x)d\mu(x) \right| \leq \varepsilon/2;
$$

si $W \subset W_0$ est le voisinage de $\mu_0$ dans $\mathcal{M}_+(X)$ formé des mesures $\mu \in W_0$ telles que $\left| \int f(x)d\mu(x) - \int f(x)d\mu_0(x) \right| \leq \varepsilon/2$, $U$ et $W$ répondent à la question.

## EXERCICES {#int-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
