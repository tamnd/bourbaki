---
book: int
book_title: Integration
chapter: III
chapter_title: Mesures sur les espaces localement compacts
section: 4
section_title: Produits de mesures
lang: fr
source: int-i-iv-fr
pdf_pages: 0086-0100, 0107-0109
extraction: ocr
subsections:
    - "no": 1
      title: Produit de deux mesures
      page: 0
      pdf_page: 86
    - "no": 2
      title: Propriétés des mesures produits
      page: 0
      pdf_page: 90
    - "no": 3
      title: Continuité des mesures produits
      page: 0
      pdf_page: 92
    - "no": 4
      title: Produit d’un nombre fini de mesures
      page: 0
      pdf_page: 94
    - "no": 5
      title: Limites projectives de mesures
      page: 0
      pdf_page: 96
    - "no": 6
      title: Produits infinis de mesures
      page: 0
      pdf_page: 99
statements: 21
exercises: 2
content_sha256: 82b3ee69957ad213d05a343d2ce1e28aefa3a09c0af8ea93d09e6a38261ee993
---

## § 4. Produits de mesures

### 1. Produit de deux mesures

#### Théorème 1 {#int-iii-s4-thm-1 .statement}

*Soient X, Y deux espaces localement compacts, $\lambda$ une mesure sur X, $\mu$ une mesure sur Y; il existe sur $X \times Y$ une mesure $\nu$ et une seule telle que, pour toute fonction $g \in \mathscr{H}(X; \mathbf{C})$ et toute fonction $h \in \mathscr{H}(Y; \mathbf{C})$, on ait*
$$
\int g(x)h(y)\, d\nu(x, y) = \left( \int g(x)\, d\lambda(x) \right) \left( \int h(y)\, d\mu(y) \right).
$$

#### Lemme 1 {#int-iii-s4-lem-1 .statement}

*Soient X, Y deux espaces localement compacts, K (resp. L) une partie compacte de X (resp. Y).
(i) La restriction à $\mathscr{H}(X \times Y, K \times L; \mathbf{C})$ de la bijection canonique $\omega : \mathscr{F}(X \times Y; \mathbf{C}) \to \mathscr{F}(X; \mathscr{F}(Y; \mathbf{C}))$ (*Ens. R, § 4, n° 14)* est une isométrie de l’espace de Banach $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ sur l’espace de Banach $\mathcal{K}(X, K ; \mathcal{K}(Y, L ; \mathbf{C}))$.

(ii) *L’espace vectoriel* $\mathcal{K}(X, K ; \mathbf{C}) \otimes_c \mathcal{K}(Y, L ; \mathbf{C})$, *identifié canoniquement à un sous-espace de* $\mathcal{K}(X \times Y, K \times L ; \mathbf{C})$, (*Alg.*, chap. II, 3e éd., § 7, no 7, commentaires suivant le cor. de la prop. 15) *est dense dans cet espace de Banach*.

Il est immédiat que l’image par $\omega$ de $\mathcal{K}(X \times Y, K \times L ; \mathbf{C})$ est contenue dans $\mathcal{K}(X, K ; \mathcal{K}(Y, L ; \mathbf{C}))$. Inversement, si $u$ est une application continue de $X$ dans $\mathcal{K}(Y, L ; \mathbf{C})$, de support contenu dans $K$, l’application $(x, y) \mapsto u(x)(y)$ de $X \times Y$ dans $\mathbf{C}$ est continue et a son support contenu dans $K \times L$, donc la restriction de $\omega$ à $\mathcal{K}(X \times Y, K \times L ; \mathbf{C})$ est une bijection de cet espace sur $\mathcal{K}(X, K ; \mathcal{K}(Y, L ; \mathbf{C}))$; le fait que cette restriction est une isométrie d’espaces de Banach résulte de la relation
$$
\sup_{(x, y) \in K \times L} |f(x, y)| = \sup_{x \in K} (\sup_{y \in L} |f(x, y)|).
$$
Ceci prouve (i); d’autre part, l’image par $\omega$ de
$$
\mathcal{K}(X, K ; \mathbf{C}) \otimes_c \mathcal{K}(Y, L ; \mathbf{C})
$$
identifié à un sous-espace de $\mathcal{K}(X \times Y, K \times L ; \mathbf{C})$, est l’espace $\mathcal{K}(X, K ; \mathbf{C}) \otimes_c \mathcal{K}(Y, L ; \mathbf{C})$ identifié canoniquement cette fois à un espace d’applications de $X$ dans $\mathcal{K}(Y, L ; \mathbf{C})$ (*Alg.*, chap. II, 3e éd., § 7, no 7, cor. de la prop. 15); mais on sait que ce sous-espace de $\mathcal{K}(X, K ; \mathcal{K}(Y, L ; \mathbf{C}))$ est *dense* dans ce dernier (§ 1, no 2, prop. 5), donc la conclusion de (ii) résulte de ce que la restriction de $\omega$ est un isomorphisme topologique.

Ce lemme étant démontré, notons maintenant que toute partie compacte de $X \times Y$ est contenue dans un produit $K \times L$, où $K$ (resp. $L$) est une partie compacte de $X$ (resp. $Y$). Il résulte donc du lemme 1, (ii) que le sous-espace $\mathcal{K}(X ; \mathbf{C}) \otimes_c \mathcal{K}(Y ; \mathbf{C})$ est *dense* dans $\mathcal{K}(X \times Y ; \mathbf{C})$; comme la relation (1) s’écrit aussi $\nu(g \otimes h) = \lambda(g)\mu(h)$ pour $g \in \mathcal{K}(X ; \mathbf{C}), h \in \mathcal{K}(Y ; \mathbf{C})$, on en déduit aussitôt l’unicité de $\nu$. Pour prouver l’existence de $\nu$, nous utiliserons le lemme suivant:

#### Lemme 2 {#int-iii-s4-lem-2 .statement}

*Les notations étant celles du lemme 1, pour toute fonction* $f \in \mathcal{K}(X \times Y, K \times L ; \mathbf{C})$, *la fonction*
$$
y \mapsto h(y) = \int f(x, y) \, d\lambda(x)
$$
*appartient à* $\mathcal{K}(Y, L ; \mathbf{C})$.

En effet, pour toute fonction $u \in \mathcal{K}(X; \mathcal{K}(Y, L; \mathbf{C}))$, l’intégrale $\int u(x) \, d\lambda(x)$ appartient à $\mathcal{K}(Y, L; \mathbf{C})$, puisque ce dernier est un espace de Banach ($§ 3$, n° 3, cor. 1 de la prop. 7); mais pour $u = \omega(f)$ et pour tout $y \in Y$, on a
$$
\left\langle \int u(x) \, d\lambda(x), \varepsilon_y \right\rangle = \int u(x)(y) \, d\lambda(x) = \int f(x, y) \, d\lambda(x)
$$
d’où le lemme.

Considérons alors, pour toute fonction $f \in \mathcal{K}(X \times Y; \mathbf{C})$, le nombre $v(f) = \mu(\int f(x, y) \, d\lambda(x))$ (que nous noterons encore $\int d\mu(y) \int f(x, y) \, d\lambda(x)$ par abus de notation); si K (resp. L) est une partie compacte de X (resp. Y), il existe un nombre $a_K$ (resp. $b_L$) tel que, pour toute fonction $g \in \mathcal{K}(X, K; \mathbf{C})$ (resp. $h \in \mathcal{K}(Y, L; \mathbf{C})$), on ait $|\lambda(g)| \leq a_K \|g\|$ (resp. $|\mu(h)| \leq b_L \|h\|$). Il en résulte que pour toute fonction $f \in \mathcal{K}(X \times Y, K \times L; \mathbf{C})$, on a
$$
|\int f(x, y) \, d\lambda(x)| \leq a_K \|f\|
$$
pour tout $y \in Y$, puis $|v(f)| \leq a_K b_L \|f\|$. La forme linéaire $v$ sur $\mathcal{K}(X \times Y; \mathbf{C})$ est donc une mesure sur $X \times Y$ et vérifie (1) de façon évidente, ce qui achève la démonstration du th. 1.

#### Définition 1 {#int-iii-s4-def-1 .statement}

Etant données deux mesures $\lambda, \mu$ définies respectivement sur deux espaces localement compacts $X, Y$, on appelle mesure produit de $\lambda$ par $\mu$ l’unique mesure $v$ sur $X \times Y$ satisfaisant à la relation (1) pour toute fonction $g \in \mathcal{K}(X; \mathbf{C})$ et toute fonction $h \in \mathcal{K}(Y; \mathbf{C})$.

Dans la démonstration du th. 1, on peut intervertir les rôles des espaces $X$ et $Y$; identifiant canoniquement $Y \times X$ et $X \times Y$, on définit ainsi sur $X \times Y$ la mesure
$$
f \mapsto \int d\lambda(x) \int f(x, y) \, d\mu(y),
$$
qui satisfait encore à la condition (1). On a donc démontré le théorème suivant:

#### Théorème 2 {#int-iii-s4-thm-2 .statement}

Soient $\lambda, \mu$ deux mesures définies respectivement sur deux espaces localement compacts $X, Y$. Pour toute fonction $f$ de $\mathcal{K}(X \times Y; \mathbf{C})$, l’intégrale de $f$ par rapport à la mesure produit $v$ de $\lambda$ par $\mu$ a pour valeur
$$
\int f(x, y) \, dv(x, y) = \int d\lambda(x) \int f(x, y) \, d\mu(y)
$$
$$
= \int d\mu(y) \int f(x, y) \, d\lambda(x).
$$

En raison de cette dernière formule, l’intégrale de $f$ par rapport à la mesure produit $\nu$ se note le plus souvent $\int \int \int d\lambda\, d\mu$, ou $\int \int f\, d\mu\, d\lambda$, ou $\int \int f\lambda\mu$, ou $\int \int f\mu\lambda$, ou $\int \int f(x, y)\, d\lambda(x)\, d\mu(y)$, ou $\int \int f(x, y)\, d\mu(y)\, d\lambda(x)$, ou $\int \int f(x, y)\lambda(x)\mu(y)$, ou $\int \int f(x, y)\mu(y)\lambda(x)$; on dit que c’est l’intégrale *double* de $f$ par rapport à $\lambda$ et à $\mu$. Avec cette notation, la formule (3) s’écrit

(4)
$$
\int \int \int f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\lambda(x) \int f(x, y)\, d\mu(y)
$$
$$
= \int d\mu(y) \int f(x, y)\, d\lambda(x).
$$

La formule (3) montre que si $\lambda$ et $\mu$ sont des mesures réelles (resp. positives), la mesure produit $\nu$ est réelle (resp. positive).

#### Exemple 1 {#int-iii-s4-n1-exa-1 .statement}

La mesure produit des mesures de Dirac $\varepsilon_x$ ($x \in X$) et $\varepsilon_y$ ($y \in Y$) est la mesure de Dirac $\varepsilon_{(x, y)}$.

#### Exemple 2 {#int-iii-s4-n1-exa-2 .statement}

Prenons $X = Y = \mathbf{R}$, et pour $\lambda$ et $\mu$ la *mesure de Lebesgue* (§ 1, n° 3) sur $\mathbf{R}$; leur produit est appelé la *mesure de Lebesgue* sur $\mathbf{R}^2$; l’intégrale d’une fonction $f \in \mathcal{H}(\mathbf{R}^2; \mathbf{C})$ par rapport à cette mesure se note $\int \int f(x, y)\, dx\, dy$ ou $\int \int f(x, y)\, dy\, dx$; la formule (4), pour une fonction nulle hors d’un pavé compact $[a, b] \times [c, d]$, entraîne la formule
$$
\int_c^d dy \int_a^b f(x, y)\, dx = \int_a^b dx \int_c^d f(x, y)\, dy
$$
démontrée dans *Fonct. var. réelle*, chap. II, § 3, n° 6.

Comme la mesure de Lebesgue sur $\mathbf{R}$ est invariante par toute translation (§ 1, n° 3), il en résulte aussitôt que la mesure de Lebesgue sur $\mathbf{R}^2$ est *invariante par toute translation de $\mathbf{R}^2$*.

#### Remarque {#int-iii-s4-n1-rem-1 .statement}

Soit $E$ un espace localement convexe séparé, et soit $f$ une application de $\mathcal{H}(X \times Y; E)$ telle que $f(X \times Y)$ soit contenu dans une partie *convexe complète* $C$ de $E$. Pour tout $y \in Y$, l’intégrale $h(y) = \int f(x, y)\, d\lambda(x)$ appartient alors à $E$ (§ 3, n° 3, prop. 7); en outre, la fonction $h$ appartient à $\mathcal{H}(Y; E)$: en effet, pour tout $z' \in E'$, on a
$$
\langle h(y), z' \rangle = \int \langle f(x, y), z' \rangle\, d\lambda(x),
$$
donc $y \mapsto \langle h(y), z' \rangle$ appartient à $\mathcal{H}(Y; \mathbf{C})$ en vertu du lemme 2. L’intégrale $\int h\, d\mu$ est donc définie (et *a priori* appartient à ${E'}^*$); montrons que l’on a
(5)
$$
\int \int f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\mu(y) \int f(x, y)\, d\lambda(x)
$$
$$
= \int d\lambda(x) \int f(x, y)\, d\mu(y)
$$

généralisant ainsi la formule (4). En effet, pour tout $z' \in E'$, on a
$$
\left\langle \int \int f d\lambda d\mu, z' \right\rangle = \int \int \left\langle f, z' \right\rangle d\lambda d\mu = \int d\mu \int \left\langle f, z' \right\rangle d\lambda
$$
$$
= \int \left\langle \int f d\lambda, z' \right\rangle d\mu = \left\langle \int d\mu \int f d\lambda, z' \right\rangle
$$
en vertu de (4), d’où (5).

### 2. Propriétés des mesures produits

Si $\lambda$ (resp. $\mu$) est une mesure sur $X$ (resp. $Y$) et $\nu$ la mesure produit de $\lambda$ par $\mu$, la restriction de $\nu$ à $\mathcal{K}(X; \mathbf{C}) \otimes_{c} \mathcal{K}(Y; \mathbf{C})$ n’est autre que le produit tensoriel $\lambda \otimes \mu$ des deux formes linéaires $\lambda$ et $\mu$ (*Alg.*, chap. II, 3e éd., § 3, n° 2), car la relation (1) du n° 1 s’écrit $\langle g \otimes h, \nu \rangle = \langle g, \lambda \rangle \langle h, \mu \rangle = \langle g \otimes h, \lambda \otimes \mu \rangle$ quels que soient $g \in \mathcal{K}(X; \mathbf{C})$ et $h \in \mathcal{K}(Y; \mathbf{C})$. Par abus de langage, nous noterons encore $\lambda \otimes \mu$ la mesure produit $\nu$ (et non seulement sa restriction au sous-espace partout dense $\mathcal{K}(X; \mathbf{C}) \otimes_{c} \mathcal{K}(Y; \mathbf{C})$ de $\mathcal{K}(X \otimes Y; \mathbf{C})$).

L’application $(\lambda, \mu) \mapsto \lambda \otimes \mu$ de $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ dans $\mathcal{M}(X \times Y; \mathbf{C})$ est évidemment bilinéaire, en vertu de la formule (3) du n° 1.

#### Proposition 1 {#int-iii-s4-prop-1 .statement}

*Soient $\lambda$ une mesure sur $X$, $\mu$ une mesure $Y$; si $g \in \mathcal{C}(X; \mathbf{C}), h \in \mathcal{C}(Y; \mathbf{C}),$ on a*
$$(6)$$
$$(g.\lambda) \otimes (h.\mu) = (g \otimes h).(\lambda \otimes \mu).$$

En effet, pour toute fonction $f \in \mathcal{K}(X \times Y; \mathbf{C})$, on a, en vertu de la formule (3) du n° 1,
$$
\langle f, (g \otimes h).(\lambda \otimes \mu) \rangle = \int d\lambda(x) \int f(x, y) g(x) h(y) d\mu(y)
$$
$$
= \int g(x) d\lambda(x) \int f(x, y) h(y) d\mu(y)
$$
ce qui prouve la formule (6).

#### Proposition 2 {#int-iii-s4-prop-2 .statement}

*Le support du produit $\lambda \otimes \mu$ est égal au produit du support de $\lambda$ et du support de $\mu$.*

Remarquons en premier lieu que la relation $\lambda \otimes \mu = 0$ entraîne que l’une des mesures $\lambda, \mu$ est nulle (*Alg.*, chap. II, 3e éd., § 7, n° 7, prop. 16, (ii)). D’autre part, si $U$ (resp. $V$) est un ensemble ouvert dans $X$ (resp. $Y$), la restriction de $\lambda \otimes \mu$ au produit $U \times V$ est le produit des restrictions de $\lambda$ à $U$ et de $\mu$ à $V$, comme il résulte du th. 1 du n° 1 et de la définition de la restriction d’une mesure à un ensemble ouvert (§ 2, n° 1). Pour que la restriction de $\lambda \otimes \mu$ à $U \times V$ soit nulle, il faut et il suffit par conséquent que la restriction de $\lambda$ à $U$ ou la restriction de $\mu$ à $V$ soit nulle, ce qui démontre la proposition, compte tenu de la définition du support d’une mesure (§ 2, n° 2).

#### Proposition 3 {#int-iii-s4-prop-3 .statement}

*Soient* $\lambda \in \mathcal{M}(X; \mathbf{C})$, $\mu \in \mathcal{M}(Y; \mathbf{C})$. *On a*
$$
|\lambda \otimes \mu| = |\lambda| \otimes |\mu|.
$$
(7)

Soient $f \in \mathcal{K}_+(X \times Y)$, $g \in \mathcal{K}(X \times Y; \mathbf{C})$ telles que $|g| \leq f$; on a (§ 1, n° 6, formule (13))

$$
|\langle g, \lambda \otimes \mu \rangle| = \left| \int d\lambda(x) \int g(x, y) \, d\mu(y) \right| \leq \int d|\lambda|(x) \int |g(x, y)| \, d|\mu|(y)
$$
$$
= \langle |g|, |\lambda| \otimes |\mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle.
$$

On en conclut que $\langle f, |\lambda \otimes \mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle$, et finalement
$$
|\lambda \otimes \mu| \leq |\lambda| \otimes |\mu|.
$$
(8)

D’autre part, soient $u \in \mathcal{K}_+(X)$, $v \in \mathcal{K}_+(Y)$. Pour tout $\varepsilon > 0$, il existe $u_1 \in \mathcal{K}(X; \mathbf{C})$, $v_1 \in \mathcal{K}(Y; \mathbf{C})$ telles que $|u_1| \leq u$, $|v_1| \leq v$ et
$$
|\langle u_1, \lambda \rangle| \geq \langle u, |\lambda| \rangle - \varepsilon, \quad |\langle v_1, \mu \rangle| \geq \langle v, |\mu| \rangle - \varepsilon
$$
(§ 1, n° 6). On en déduit que $|u_1 \otimes v_1| \leq u \otimes v$, et
$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle \geq |\langle u_1 \otimes v_1, \lambda \otimes \mu \rangle| = |\langle u_1, \lambda \rangle \langle v_1, \mu \rangle|
$$
$$
\geq (\langle u, |\lambda| \rangle - \varepsilon)(\langle v, |\mu| \rangle - \varepsilon).
$$

Comme $\varepsilon$ est arbitraire, on en conclut que
$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle \geq \langle u, |\lambda| \rangle \langle v, |\mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Compte tenu de (8), on voit que
$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Toute fonction de $\mathcal{K}(X; \mathbf{C})$ (resp. $\mathcal{K}(Y; \mathbf{C})$) étant combinaison linéaire de fonctions de $\mathcal{K}_+(X)$ (resp. $\mathcal{K}_+(Y)$), la formule précédente est encore vraie pour $u \in \mathcal{K}(X; \mathbf{C})$ et $v \in \mathcal{K}(Y; \mathbf{C})$; la proposition résulte donc de ce que $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ est dense dans $\mathcal{K}(X \times Y; \mathbf{C})$.

#### Corollaire {#int-iii-s4-n2-cor-1 .statement}

Soient $\lambda \in \mathcal{M}(X; \mathbf{R}), \mu \in \mathcal{M}(Y; \mathbf{R})$. Alors on a
$$
\begin{cases}
(\lambda \otimes \mu)^+ = \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- \\
(\lambda \otimes \mu)^- = \lambda^+ \otimes \mu^- + \lambda^- \otimes \mu^+
\end{cases}
$$
En effet, on a, en vertu de la prop. 3,
$$
(\lambda \otimes \mu)^+ = \frac{1}{2}(\lambda \otimes \mu + |\lambda| \otimes |\mu|)
= \frac{1}{2}((\lambda^+ - \lambda^-) \otimes (\mu^+ - \mu^-) + (\lambda^+ + \lambda^-) \otimes (\mu^+ + \mu^-))
= \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^-.
$$
On raisonne de même pour $(\lambda \otimes \mu)^-$.

#### Proposition 4 {#int-iii-s4-prop-4 .statement}

Soient $\lambda \in \mathcal{M}(X; \mathbf{C}), \mu \in \mathcal{M}(Y; \mathbf{C})$. On a
$$
\|\lambda \otimes \mu\| = \|\lambda\| \cdot \|\mu\|,
$$
en convenant de remplacer le second membre par 0 lorsque l’un des facteurs est 0 et l’autre $+\infty$. En particulier, si $\lambda$ et $\mu$ sont bornées, $\lambda \otimes \mu$ est bornée.

En vertu de la prop. 3 ci-dessus, et du § 1, n° 8, cor. de le prop. 10, on peut se ramener au cas où $\lambda$ et $\mu$ sont des mesures positives. Si $\lambda = 0$ ou $\mu = 0$, le résultat est trivial ; supposons donc $\lambda \neq 0$ et $\mu \neq 0$. Prouvons d’abord que $\|\lambda \otimes \mu\| \leq \|\lambda\| \cdot \|\mu\|$. On peut supposer $\lambda$ et $\mu$ bornées. Pour toute $f \in \mathcal{K}_+(X \times Y)$, on a
$$
\langle f, \lambda \otimes \mu \rangle = \int d\lambda(x) \int f(x, y) d\mu(y)
$$
et
$$
\int f(x, y) d\mu(y) \leq \|f\| \cdot \|\mu\|
$$
pour tout $x \in X$, donc
$$
\langle f, \lambda \otimes \mu \rangle \leq \|f\| \cdot \|\lambda\| \cdot \|\mu\|,
$$
ce qui démontre notre assertion. D’autre part, soient
$$
\alpha < \|\lambda\|, \beta < \|\mu\|
$$
deux nombres réels $\geq 0$. Il existe $g \in \mathcal{K}_+(X), h \in \mathcal{K}_+(Y)$ telles que $\|g\| \leq 1, \|h\| \leq 1, \lambda(g) \geq \alpha, \mu(h) \geq \beta$. Alors on a $g \otimes h \in \mathcal{K}_+(X \times Y)$, $\|g \otimes h\| \leq 1$ et $\langle g \otimes h, \lambda \otimes \mu \rangle \geq \alpha \beta$; donc $\|\lambda \otimes \mu\| \geq \alpha \beta$ et finalement $\|\lambda \otimes \mu\| \geq \|\lambda\| \cdot \|\mu\|$, ce qui achève la démonstration.

### 3. Continuité des mesures produits

#### Proposition 5 {#int-iii-s4-prop-5 .statement}

Pour toute mesure $\lambda_0 \in \mathcal{M}(X; \mathbf{C})$, l’application $\mu \mapsto \lambda_0 \otimes \mu$ de $\mathcal{M}(Y; \mathbf{C})$ dans $\mathcal{M}(X \times Y; \mathbf{C})$ est vaguement continue.

En effet, pour toute fonction $f \in \mathcal{K}(X \times Y; \mathbf{C})$, on sait que la fonction $h(y) = \int f(x, y) d\lambda_0(x)$ appartient à $\mathcal{K}(Y; \mathbf{C})$ (n° 1, lemme 2), et l’on a $\langle f, \lambda_0 \otimes \mu \rangle = \langle h, \mu \rangle$, d’où la proposition.

#### Proposition 6 {#int-iii-s4-prop-6 .statement}

Lorsqu’on munit $\mathcal{M}(X; \mathbf{C}), \mathcal{M}(Y; \mathbf{C})$ et $\mathcal{M}(X \times Y; \mathbf{C})$ de la topologie de la convergence strictement compacte (§ 1, n° 10), l’application bilinéaire $(\lambda, \mu) \mapsto \lambda \otimes \mu$ de $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ dans $\mathcal{M}(X \times Y; \mathbf{C})$ est hypocontinue pour les ensembles de parties vaguement bornées de $\mathcal{M}(X; \mathbf{C})$ et $\mathcal{M}(Y; \mathbf{C})$ (Esp. vect. top., chap. III, § 4, n° 2).

Soient $K \subset X, L \subset Y$ deux ensembles compacts, $A$ une partie compacte de $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$, $B$ une partie vaguement bornée et fermée de $\mathcal{M}(X; \mathbf{C})$; on sait que $B$ est vaguement compacte (§ 1, n° 9, prop. 15), donc aussi compacte pour la topologie de la convergence strictement compacte (§ 1, n° 10, prop. 17). D’autre part, l’espace de Banach $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ est isométrique à $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ (n° 1, lemme 1); l’application $\varphi$ de $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C})) \times \mathcal{M}(X; \mathbf{C})$ dans $\mathcal{K}(Y, L; \mathbf{C})$ telle que $\varphi(g, \lambda)$ soit la fonction $h$ définie par $h(y) = \int g(x, y) d\lambda(x)$, est séparément continue en vertu du § 3, n° 4, prop. 8 et 9. Comme $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ est tonnelé, on en conclut que l’application $\varphi$ est hypocontinue relativement aux parties vaguement bornées de $\mathcal{M}(X; \mathbf{C})$ (Esp. vect. top., chap. III, § 4, n° 2, prop. 6); la restriction de cette application à $A \times B$ est donc continue (loc. cit., prop. 4). L’image $C$ de $A \times B$ par cette application est par suite une partie compacte de l’espace de Banach $\mathcal{K}(Y, L; \mathbf{C})$. Or, $C$ n’est autre que l’ensemble des fonctions $h(y) = \int f(x, y) d\lambda(x)$ lorsque $f$ parcourt $A$ et $\lambda$ parcourt $B$; en vertu de la formule (3) du n° 1, les conditions $\lambda \in B$ et $\mu \in C^\circ$ entraînent donc $\lambda \otimes \mu \in A^\circ$. En vertu de la définition de la topologie de la convergence strictement compacte, cela prouve la proposition (Esp. vect. top., chap. III, § 4, n° 2, déf. 2).

La conclusion de la prop. 6 n’est plus valable lorsqu’on remplace la topologie de la convergence strictement compacte par la topologie vague (exerc. 2c)). Toutefois, si $B$ (resp. $C$) est une partie vaguement bornée de $\mathcal{M}(X, \mathbf{C})$ (resp. $\mathcal{M}(Y; \mathbf{C})$), l’image de $B \times C$ par l’application $(\lambda, \mu) \mapsto \lambda \otimes \mu$ est vaguement bornée dans $\mathcal{M}(X \times Y; \mathbf{C})$ en vertu de la prop. 6, donc la restriction de cette application à $B \times C$ est vaguement continue en vertu de la prop. 4 et du § 1, n° 10, prop. 17 (cf. exerc. 3).

### 4. Produit d’un nombre fini de mesures

Soient $X_i$ ($1 \leq i \leq n$) $n$ espaces localement compacts, $X = \prod_{i=1}^n X_i$ leur produit. L’ensemble des combinaisons linéaires des fonctions complexes de la forme

$$
(x_1, x_2, \ldots, x_n) \mapsto f_1(x_1)f_2(x_2)\ldots f_n(x_n)
$$

s’identifie canoniquement au produit tensoriel $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$, et il résulte du lemme 1 du n° 1, par récurrence sur $n$, que ce produit tensoriel est dense dans $\mathcal{K}(X; \mathbf{C})$.

Soit alors $\mu_i$ une mesure sur $X_i$ ($1 \leq i \leq n$); il existe sur $X$ une mesure $\nu$ et une seule telle que, pour $f_i \in \mathcal{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$), on ait

$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \nu \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$

En effet, si cette mesure existe, elle est unique d’après ce qui précède. D’autre part, soit $\nu = \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$ la mesure sur $X$ définie par la relation de récurrence sur $n$

$$
\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n = (\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_{n-1}) \otimes \mu_n.
$$

Il résulte du n° 1, formule (1) et de cette définition (par récurrence sur $n$) que $\nu$ vérifie (11); on dit que c’est la mesure produit des mesures $\mu_i$ ($1 \leq i \leq n$), et on la note encore $\bigotimes_{i=1}^n \mu_i$.

La relation (11) s’écrit aussi

$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$

**Proposition 7** (« associativité du produit de mesures »). —
Soit $(I_k)_{1 \leq k \leq r}$ une partition de l’intervalle $[1, n]$ dans $\mathbf{N}$; on a

$$
\bigotimes_{k=1}^r \left( \bigotimes_{i \in I_k} \mu_i \right) = \bigotimes_{i=1}^n \mu_i.
$$

En effet, ces deux mesures coïncident, d’après (12), pour toute fonction de $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$.

L’intégrale d’une fonction $f \in \mathcal{K}(X; \mathbf{C})$ par rapport à la mesure produit se note

$$
\int f d\mu_1 d\mu_2 \ldots d\mu_n,
$$

ou

$$
\iint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n
$$

ou

$$
\int f(\mu_1 \otimes \cdots \otimes \mu_n)
$$

ou encore

$$
\iint \ldots \int f(x_1, x_2, \ldots, x_n) d\mu_1(x_1) d\mu_2(x_2) \ldots d\mu_n(x_n)
$$

ou

$$
\iint \ldots \int f(x_1, x_2, \ldots, x_n) \mu_1(x_1) \mu_2(x_2) \ldots \mu_n(x_n)
$$

avec $n$ signes $\int$; on dit que c’est une intégrale multiple d’ordre $n$ ou intégrale $n$-uple. En vertu de l’associativité du produit de mesures et du théorème d’interversion des intégrations (n° 1, th. 2), on a, pour toute permutation $\sigma$ de $\{1, n\}$,

(14)

$$
\iint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n = \int d\mu_{\sigma(1)} \int d\mu_{\sigma(2)} \ldots \int f d\mu_{\sigma(n)}.
$$

La notation de l’intégrale et la formule (14) s’étendent de façon évidente aux fonctions $\mathbf{f} \in \mathcal{K}(X; E)$ à valeurs dans un espace localement convexe séparé $E$, telles que $\mathbf{f}(X)$ soit contenu dans une partie convexe complète de $E$. Nous laissons au lecteur le soin de généraliser au produit d’un nombre fini quelconque de mesures les résultats des n°s 2 et 3 concernant le produit de deux mesures.

En particulier, on appelle mesure de Lebesgue sur $\mathbf{R}^n$ le produit de $n$ mesures identiques à la mesure de Lebesgue sur $\mathbf{R}$; l’intégrale d’une fonction $\mathbf{f} \in \mathcal{K}(\mathbf{R}^n; E)$, satisfaisant à la condition précédente, se note

$$
\iint \ldots \int \mathbf{f}(x_1, x_2, \ldots, x_n) dx_1 dx_2 \ldots dx_n
$$

et est égale à

$$
\int_{-\infty}^{+\infty} dx_1 \int_{-\infty}^{+\infty} dx_2 \ldots \int_{-\infty}^{+\infty} \mathbf{f}(x_1, x_2 \ldots, x_n) dx_n.
$$

La mesure de Lebesgue sur $\mathbf{R}^n$ est invariante par toute translation.

### 5. Limites projectives de mesures

Soient X, Y deux espaces compacts, $p : X \to Y$ une application continue; alors $f \mapsto f \circ p$ est une application linéaire continue de $\mathcal{C}(Y ; \mathbf{C})$ dans $\mathcal{C}(X ; \mathbf{C})$, puisque l’on a $\|f \circ p\| \leq \|f\|$ pour toute fonction $f \in \mathcal{C}(Y ; \mathbf{C})$; nous noterons $p'$ cette application. Sa transposée ${}^t p' : \mathcal{M}(X ; \mathbf{C}) \to \mathcal{M}(Y ; \mathbf{C})$ est donc telle que, pour toute mesure $\mu$ sur X, ${}^t p'(\mu)$ soit la mesure sur Y telle que
$$
\langle {}^t p'(\mu), f \rangle = \langle \mu, f \circ p \rangle
$$
pour toute fonction $f \in \mathcal{C}(Y ; \mathbf{C})$. On observera que pour tout $x \in X$, on a ${}^t p'(\varepsilon_x) = \varepsilon_{p(x)}$; pour cette raison, on notera $p_*(\mu)$ la mesure ${}^t p'(\mu)$, qui prolonge donc $p$ lorsqu’on plonge canoniquement X (resp. Y) dans $\mathcal{M}(X ; \mathbf{C})$ (resp. $\mathcal{M}(Y ; \mathbf{C})$) (§ 1, n° 9, prop 13); pour toute mesure $\mu$ sur X, $p_*(\mu)$ est un cas particulier de la notion générale d’image d’une mesure, que nous étudierons au chap. V, § 6. Comme on a vu ci-dessus que l’on a $\|p'\| \leq 1$, on a aussi $\|{}^t p'\| \leq 1$, et par suite
$$
\|p_*(\mu)\| \leq \|\mu\|
$$
pour toute mesure $\mu \in \mathcal{M}(X ; \mathbf{C})$.

Considérons maintenant un ensemble préordonné filtrant I, un système projectif $(X_\alpha, p_{\alpha\beta})$ d’espaces compacts $X_\alpha$ (Top. gén., chap. I, 3e éd., § 4, n° 4) ayant I pour ensemble d’indices; on sait que l’espace limite projective $X = \lim_{\leftarrow} X_\alpha$ est compact (Top. gén., chap. I, 3e éd., § 9, n° 6, prop. 8); nous désignerons par $p_\alpha$ l’application canonique de X dans $X_\alpha$.

Il est clair que $(\mathcal{M}(X_\alpha ; \mathbf{C}), (p_{\alpha\beta})_* )$ est un système projectif d’espaces vectoriels, et que $((p_\alpha)_*)$ est un système projectif d’applications linéaires, ce qui justifie la définition suivante:

#### Définition 2 {#int-iii-s4-def-2 .statement}

On dit qu’une famille $(\mu_\alpha)_{\alpha \in I}$, où, pour tout $\alpha \in I$, $\mu_\alpha$ est une mesure sur $X_\alpha$, est un système projectif de mesures si, pour $\alpha \leq \beta$, on a $\mu_\alpha = (p_{\alpha\beta})_*(\mu_\beta)$. On dit qu’une mesure $\mu$ sur $X = \lim_{\leftarrow} X_\alpha$ est limite projective du système projectif $(\mu_\alpha)$ si, pour tout $\alpha \in I$, on a $\mu_\alpha = (p_\alpha)_*(\mu)$.

#### Proposition 8 {#int-iii-s4-prop-8 .statement}

(i) Si un système projectif $(\mu_\alpha)$ de mesures sur les $X_\alpha$ admet une limite projective, celle-ci est unique.

(ii) Si un système projectif $(\mu_\alpha)$ admet une limite projective, la famille des normes $(\|\mu_\alpha\|)$ est bornée.

(iii) Si les $p_{\alpha\beta}$ sont surjectives et la famille ($\| \mu_\alpha \|$) bornée; le système projectif de mesures ($\mu_\alpha$) admet une limite projective.

(iv) Si les $p_{\alpha\beta}$ sont surjectives, tout système projectif ($\mu_\alpha$) de mesures positives admet une limite projective $\mu$, qui est une mesure positive sur $X$, et l’on a $\| \mu \| = \| \mu_\alpha \|$ pour tout $\alpha$.

(i) Nous prouverons d’abord le lemme suivant:

#### Lemme 3 {#int-iii-s4-lem-3 .statement}

Soit $F$ l’ensemble des fonctions $f \in \mathcal{C}(X ; \mathbf{C})$ ayant la propriété suivante: il existe un $\alpha \in I$ et une fonction $f_\alpha \in \mathcal{C}(X_\alpha ; \mathbf{C})$ tels que $f = f_\alpha \circ p_\alpha$. Alors $F$ est un sous-espace vectoriel partout dense de $\mathcal{C}(X ; \mathbf{C})$.

Notons d’abord que si $g = g_\beta \circ p_\beta$ et $h = h_\gamma \circ p_\gamma$, où $g_\beta \in \mathcal{C}(X_\beta ; \mathbf{C})$ et $h_\gamma \in \mathcal{C}(X_\gamma ; \mathbf{C})$, il existe $\alpha \in I$ tel que $\alpha \geq \beta$ et $\alpha \geq \gamma$, et l’on a donc $p_\beta = p_{\beta \alpha} \circ p_\alpha$, $p_\gamma = p_{\gamma \alpha} \circ p_\alpha$, ce qui montre que
$$
g + h = (g_\beta \circ p_{\beta \alpha} + h_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha
$$
appartient à $F$; on voit de même que $gh \in F$; $F$ est donc une sous-$\mathbf{C}$-algèbre de $\mathcal{C}(X ; \mathbf{C})$, qui contient les constantes et est telle que la relation $f \in F$ entraîne $\bar{f} \in F$. Enfin, si $x \neq y$ sont deux points de $X$, il existe $\alpha \in I$ tel que $p_\alpha(x) \neq p_\alpha(y)$, donc il y a une fonction $f_\alpha \in \mathcal{C}(X_\alpha ; \mathbf{C})$ telle que $f_\alpha(p_\alpha(x)) \neq f_\alpha(p_\alpha(y))$. La conclusion résulte par suite du th. de Weierstrass–Stone (Top. gén., chap. X, 2e éd., § 4, n° 4, prop. 7).

Ce lemme étant établi, soient $\mu, \mu'$ deux mesures sur $X$ telles que $(p_\alpha)_*(\mu) = (p_\alpha)_*(\mu')$ pour tout $\alpha \in I$; cela signifie que, pour tout $\alpha \in I$ et toute fonction $f_\alpha \in \mathcal{C}(X_\alpha ; \mathbf{C})$, on a
$$
\langle f_\alpha, (p_\alpha)_*(\mu) \rangle = \langle f_\alpha, (p_\alpha)_*(\mu') \rangle,
$$
ou encore $\langle f_\alpha \circ p_\alpha, \mu \rangle = \langle f_\alpha \circ p_\alpha, \mu' \rangle$; autrement dit, $\mu$ et $\mu'$ coïncident dans le sous-espace $F$ de $\mathcal{C}(X ; \mathbf{C})$, qui est partout dense en vertu du lemme 3, donc $\mu = \mu'$, ce qui démontre (i).

(ii) La relation (15) appliquée à $p_\alpha$ montre que si $\mu$ est limite projective du système projectif $(\mu_\alpha)$, on a nécessairement
$$
\| \mu \| \geq \| \mu_\alpha \|
$$
pour tout $\alpha \in I$.

(iii) Supposons les $p_{\alpha\beta}$ surjectives; on sait qu’il en est alors de même des $p_\alpha$ (Top. gén., chap. I, 3e éd., § 9, n° 6, prop. 8). Considérons un système projectif de mesures $(\mu_\alpha)$, et montrons d’abord qu’il existe sur $F$ (avec les notations du lemme 3) une forme linéaire $\lambda$ telle que pour tout $\alpha \in I$ et toute $f_\alpha \in \mathcal{C}(X_\alpha ; \mathbf{C})$, on ait λ(f_α \circ p_α) = μ_α(f_α). En effet, soient β, γ deux indices dans I, f_β ∈ C(X_β ; C), f_γ ∈ C(X_γ ; C) deux fonctions telles que f_β \circ p_β = f_γ \circ p_γ ; il existe alors un indice α ∈ I tel que α ≥ β et α ≥ γ, donc p_β = p_{βα} \circ p_α, p_γ = p_{γα} \circ p_α, et (f_β \circ p_{βα}) \circ p_α = (f_γ \circ p_{γα}) \circ p_α ; comme p_α est surjective, cela entraîne f_β \circ p_{βα} = f_γ \circ p_{γα}, donc

$$
\mu_\alpha(f_\beta \circ p_{\beta\alpha}) = \mu_\alpha(f_\gamma \circ p_{\gamma\alpha});
$$

mais par définition cette dernière relation s’écrit aussi $\mu_\beta(f_\beta) = \mu_\gamma(f_\gamma)$, d’où notre assertion.

Cela étant, supposons qu’il existe un nombre fini $a > 0$ tel que $\|\mu_\alpha\| \leq a$ pour tout $\alpha ∈ I$; alors, on a, pour toute fonction $f_\alpha ∈ C(X_\alpha ; C)$

$$
|\lambda(f_\alpha \circ p_\alpha)| = |\mu_\alpha(f_\alpha)| \leq a \|f_\alpha\| = a \|f_\alpha \circ p_\alpha\|
$$

puisque $p_\alpha$ est surjective. Ceci montre que la forme linéaire $\lambda$ est continue dans F, et il résulte du lemme 3 que $\lambda$ se prolonge en une mesure $\mu$ sur X telle que $(p_\alpha)_*(\mu) = \mu_\alpha$ pour tout $\alpha ∈ I$, ce qui prouve (iii).

(iv) Pour prouver l’existence de $\mu$, il suffit, en vertu de (iii), de vérifier que la famille des normes ($\|\mu_\alpha\|$) est bornée. Mais on a $\|\mu_\alpha\| = \mu_\alpha(1)$, et pour $\alpha ≤ \beta$, la relation $\mu_\alpha = (p_{\alpha\beta})_*(\mu_\beta)$ entraîne que $\mu_\alpha(1) = \mu_\beta(1)$; comme I est filtrant, les masses totales de toutes les mesures $\mu_\alpha$ sont donc égales, d’où notre assertion. En outre, le sous-espace F vérifie de façon évidente la propriété (P) du § 1, n° 7, prop. 9, donc la mesure $\mu$, limite projective de $(\mu_\alpha)$, est positive. Enfin la relation $\mu_\alpha = (p_\alpha)_*(\mu)$ montre comme ci-dessus que $\mu(1) = \mu_\alpha(1)$.

#### Exemple {#int-iii-s4-n5-exa-1 .statement}

Soit $(X_\lambda)_{\lambda ∈ L}$ une famille d’espaces compacts; posons $X = \prod_{\lambda ∈ L} X_\lambda$, et pour toute partie finie J de L, posons $X_J = \prod_{\lambda ∈ J} X_\lambda$; désignons par $\mathrm{pr}_J : X → X_J$, et $\mathrm{pr}_{J,K} : X_K → X_J$ (pour $J ⊂ K$) les projections canoniques. On sait que $(X_J, \mathrm{pr}_{JK})$ est un système projectif d’espaces compacts, et que la limite projective du système d’applications continues $(\mathrm{pr}_J)$ est un homéomorphisme de X sur l’espace limite projective $\lim_{←} X_J$, permettant d’identifier ces deux espaces (Top. gén., chap. I, 3e éd., § 4, n° 4 et Ens. chap. III, 2e éd., § 7, n° 2, Remarque 3). Comme les projections $\mathrm{pr}_{J,K}$ sont surjectives, il résulte de la prop. 8 que l’ensemble $\mathcal{M}(X ; C)$ (resp. $\mathcal{M}_+(X)$) s’identifie à l’ensemble des systèmes projectifs $(\mu_J)$ tels que la famille des normes ($\|\mu_J\|$) soit bornée (resp. tels que les $\mu_J$ soient toutes positives, et nécessairement de même masse totale).

Considérons en particulier le cas où, pour chaque $\lambda \in L$, on prend une mesure $\mu_\lambda$ sur $X_\lambda$, et où on pose $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$. Si $J \subset K$ sont deux parties finies de $I$, on a alors, pour toute fonction $f_J \in \mathcal{C}(X_J; \mathbf{C})$, en vertu de la formule (14) du n° 4,

$$
\mu_K(f_J \circ \mathrm{pr}_{J,K}) = \mu_J(f_J) \cdot \prod_{\lambda \in K - J} \mu_\lambda(1).
$$

Pour que $(\mu_J)$ soit un système projectif de mesures, il faut et il suffit donc que l’on ait, soit $\mu_\lambda = 0$ pour tout $\lambda \in L$, soit $\mu_\lambda(1) = 1$ pour tout $\lambda \in L$.

### 6. Produits infinis de mesures

Soit $(X_\lambda)_{\lambda \in L}$ une famille d’espaces compacts, et pour tout $\lambda \in L$, soit $\mu_\lambda$ une mesure sur $X_\lambda$. Gardons les notations de l’Exemple du n° 5, de sorte qu’en particulier on a $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$ pour toute partie finie $J$ de $L$.

#### Proposition 9 {#int-iii-s4-prop-9 .statement}

*Supposons que toutes les mesures $\mu_\lambda$ soient positives et que la famille $(\mu_\lambda(1))_{\lambda \in L}$ soit multipliable dans $\mathbf{R}_+$ (le produit pouvant avoir la valeur 0). Alors il existe sur $X$ une mesure $\mu$ et une seule telle que, pour toute partie finie $J$ de $L$ et toute fonction $f_J \in \mathcal{C}(X_J; \mathbf{C})$, on ait*

$$
\mu(f_J \circ \mathrm{pr}_J) = \mu_J(f_J) \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

*En outre, la mesure $\mu$ est positive et sa masse totale est donnée par*

$$
\mu(1) = \prod_{\lambda \in L} \mu_\lambda(1).
$$

Soit $F$ l’espace vectoriel formé des fonctions sur $X$ de la forme $f_J \circ \mathrm{pr}_J$, où $J$ parcourt l’ensemble filtrant des parties finies de $L$, et $f_J \in \mathcal{C}(X_J; \mathbf{C})$; on dit encore que $F$ est l’espace des fonctions continues dans $X$ *ne dépendant que d’un nombre fini de variables*. Le lemme 3 du n° 5 montre que $F$ est dense dans $\mathcal{C}(X; \mathbf{C})$, ce qui prouve l’assertion d’unicité. Si, pour un $\lambda \in L$, on a $\mu_\lambda = 0$, la mesure $\mu = 0$ répond à la question, puisque dans le second membre de (18), on a $\mu_J(f_J) = 0$ si $\lambda \in J$, et $\prod_{\lambda \in L - J} \mu_\lambda(1) = 0$ si $\lambda \notin J$. On peut donc supposer $\mu_\lambda \neq 0$ pour tout $\lambda \in L$, et comme les mesures $\mu_\lambda$ sont positives, cela entraîne $\mu_\lambda(1) \neq 0$ pour tout $\lambda \in L$. Posons alors $\mu'_\lambda = \mu_\lambda / \mu_\lambda(1)$ pour tout $\lambda \in L$, de sorte que $\mu'_\lambda$ est une mesure positive sur $X_\lambda$ telle que $\mu'_\lambda(1) = 1$. Il résulte alors de la prop. 8 du n° 5 qu’il existe sur X une mesure positive $\mu'$ de masse totale 1, telle que l’on ait $\mu'(f_J \circ \mathrm{pr}_J) = \mu'_J(f_J)$ pour toute partie finie J de L et toute fonction $f_J \in \mathcal{C}(X_J ; \mathbf{C})$. La mesure positive
$$
\mu = \left( \prod_{\lambda \in L} \mu_\lambda(1) \right) \mu
$$
répond alors à la question, puisque l’on a
$$
\mu_J(f_J) = \mu'_J(f_J) \cdot \prod_{\lambda \in J} \mu_\lambda(1),
$$
$$
\prod_{\lambda \in L} \mu_\lambda(1) = \prod_{\lambda \in J} \mu_\lambda(1) \cdot \prod_{\lambda \in L - J} \mu_\lambda(1).
$$
On dit que la mesure $\mu$ définie dans la prop. 9 est la mesure produit de la famille de mesures positives $(\mu_\lambda)_{\lambda \in L}$, et on la note $\bigotimes_{\lambda \in L} \mu_\lambda$.

#### Corollaire {#int-iii-s4-n6-cor-1 .statement}

Supposons vérifiées les conditions de la prop. 9, et soit $(L_\rho)_{\rho \in R}$ une partition de L. Alors chacune des familles de mesures $(\mu_\lambda)_{\lambda \in L_\rho}$ admet une mesure produit, la famille des mesures produits $\left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right)_{\rho \in R}$ admet une mesure produit, et l’on a
$$
\bigotimes_{\rho \in R} \left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right) = \bigotimes_{\lambda \in L} \mu_\lambda.
$$
Cela résulte aussitôt des formules (18) et (19) et de l’associativité du produit pour les familles multipliables dans $\mathbf{R}_+$ (Top. gén., chap. IV, 3e éd., § 7, n° 5, Remarque).

EXERCICES

## EXERCICES {#int-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
