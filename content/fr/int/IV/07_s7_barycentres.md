---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 7
section_title: Barycentres
lang: fr
source: int-i-iv-fr
pdf_pages: 0219-0238, 0267-0275
extraction: ocr
subsections:
    - "no": 1
      title: Définition des barycentres
      page: 0
      pdf_page: 219
    - "no": 2
      title: Points extrémaux et barycentres
      page: 0
      pdf_page: 221
    - "no": 3
      title: 'Applications: I. Espaces vectoriels de fonctions continues réelles'
      page: 0
      pdf_page: 226
    - "no": 4
      title: Applications. II. Espaces vectoriels de fonctions continues complexes
      page: 0
      pdf_page: 230
    - "no": 5
      title: 'Applications: III. Algèbres de fonctions continues'
      page: 0
      pdf_page: 231
    - "no": 6
      title: Unicité des représentations intégrales
      page: 0
      pdf_page: 235
statements: 29
exercises: 1
content_sha256: e97fd0f41e7d621fb14994516f11d408708f0959271b4f7db32957daf87aea55
---

## § 7. Barycentres

### 1. Définition des barycentres

Soient $E$ un espace localement convexe séparé sur $\mathbf{R}$, $E'$ son dual, ${E'}^*$ le dual algébrique de $E'$, $E$ étant canoniquement identifié à un sous-espace vectoriel de $E'$. Soit $K$ une partie compacte de $E$; l’injection canonique de $K$ dans $E$ étant continue à support compact, pour toute mesure $\mu$ sur $K$, l’intégrale $\int x\ d\mu(x)$ est donc définie et est un élément de $E'$ (chap. III, § 3, n° 1). En outre, sur $K$, la topologie induite par la topologie faible $\sigma(E', E')$ est identique à la topologie initiale. Enfin, si $C$ est l’enveloppe convexe fermée de $K$ dans $E'$ muni de $\sigma(E', E')$, $C \cap E$ est l’enveloppe convexe fermée de $K$ dans $E$ pour la topologie initiale (ou la topologie affaiblie $\sigma(E, E')$).

#### Définition 1 {#int-iv-s7-def-1 .statement}

Soit $K$ une partie compacte d’un espace localement convexe séparé $E$. Pour toute mesure positive $\mu$ sur $K$, de masse totale égale à 1, on appelle barycentre de $\mu$ le vecteur $b_\mu = \int x\ d\mu(x)$ (appartenant à $E'$).

#### Exemple {#int-iv-s7-n1-exa-1 .statement}

Soit $\mu$ une mesure discrète sur $K$, positive et de masse totale 1 ; elle est donc de la forme $\mu = \sum_{i=1}^n \lambda_i \varepsilon_{x_i}$, où les $x_i \in K$, les $\lambda_i$ sont des nombres réels tels que $\lambda_i \geq 0$ pour tout $i$ et $\sum_{i=1}^n \lambda_i = 1$. Comme $\int x\ d\varepsilon_y(x) = y$ (chap. III, § 3, n° 1, Exemple 3), on a $b_\mu = \int x\ d\mu(x) = \sum_i \lambda_i x_i$. En particulier, pour tout $x \in K$, $x$ est barycentre de la mesure $\varepsilon_x$.

#### Proposition 1 {#int-iv-s7-prop-1 .statement}

Soient $E$ un espace localement convexe séparé, $K$ une partie compacte de $E$, $C$ l’enveloppe convexe fermée de $K$ dans $E$. L’ensemble $C$ est alors formé des points de $E$ qui sont barycentres d’au moins une mesure positive de masse 1 sur $K$.
Ce n’est autre que la prop. 5 du chap. III, § 3, n° 2, appliquée à l’injection canonique de $K$ dans $E$.

#### Corollaire {#int-iv-s7-n1-cor-1 .statement}

Si l’enveloppe convexe fermée $C$ de $K$ dans $E$ est compacte, le barycentre de toute mesure positive de masse totale 1 sur $K$ appartient à $E$.
En effet, $C$ est alors aussi l’enveloppe convexe fermée de $K$ dans $E'$ muni de la topologie faible $\sigma(E', E')$, et il suffit d’appliquer à l’injection canonique de $K$ dans $E$ le chap. III, § 3, n° 2, prop. 4.

#### Remarque {#int-iv-s7-n1-rem-1 .statement}

Le cor. de la prop. 1 s’applique en particulier lorsque K est convexe, ou lorsque E est quasi-complet.

#### Proposition 2 {#int-iv-s7-prop-2 .statement}

Soient K une partie convexe compacte d’un espace localement convexe séparé E, μ une mesure positive de masse 1 sur K, b_μ son barycentre. Pour toute fonction numérique convexe f ≥ 0, semi-continue inférieurement dans K, on a

$$
f(b_{\mu}) \leq \int^* f d\mu.
$$

On sait (Esp. vect. top., chap. II, 2e éd., § 5, n° 4, prop. 5) que f est l’enveloppe supérieure d’une famille de restrictions à K de fonctions linéaires affines continues $h_{\alpha}: x \mapsto c_{\alpha} + \langle x, z'_{\alpha} \rangle$. On a donc

$$
\int h_{\alpha}(x) d\mu(x) \leq \int^* f(x) d\mu(x)
$$

pour tout α ; or $\int h_{\alpha}(x) d\mu(x) = c_{\alpha} + \int \langle x, z'_{\alpha} \rangle d\mu(x)$ puisque μ est de masse totale 1 ; mais $\int \langle x, z'_{\alpha} \rangle d\mu(x) = \langle b_{\mu}, z'_{\alpha} \rangle$ par définition du barycentre. On a donc $\sup_{\alpha} \int h_{\alpha}(x) d\mu(x) = \sup_{\alpha} h_{\alpha}(b_{\mu}) = f(b_{\mu})$, d’où la conclusion.

Lorsque μ est une mesure discrète positive sur K, de masse totale 1, la prop. 2 redonne l’inégalité qui définit les fonctions convexes dans K.

#### Corollaire {#int-iv-s7-n1-cor-2 .statement}

Pour toute fonction numérique g convexe bornée et semi-continue inférieurement dans K, on a $g(b_{\mu}) \leq \int g d\mu$.

Il suffit de remarquer que $\inf_{x \in K} g(x) = a$ est fini et d’appliquer la prop. 2 à $g - a$.

### 2. Points extrémaux et barycentres

#### Proposition 3 {#int-iv-s7-prop-3 .statement}

Soient K une partie convexe compacte d’un espace localement convexe séparé E, x un point de K. Toute mesure μ sur K, positive, de masse totale 1, et admettant x pour barycentre, est vaguement adhérente à l’ensemble des mesures positives discrètes de masse totale 1, admettant x pour barycentre.

Soit U un voisinage de μ pour la topologie vague ; on peut supposer que U est formé des mesures ν sur K telles que

(1)

$$
|\mu(f_i) - \nu(f_i)| \leq \delta
$$

pour un nombre fini de fonctions $f_i \in \mathcal{C}(K; \mathbf{C})$ ($1 \leq i \leq p$) et un nombre $\delta > 0$. Pour tout point $a \in K$, il existe un voisinage convexe fermé $V_a$ de 0 dans E tel que l’on ait

$$
|f_i(y) - f_i(a)| \leq \delta/2
$$

pour $1 \leq i \leq p$ et pour tout $y \in W_a = K \cap (a + V_a)$. Comme K est compact, il y a un nombre fini de points $a_j$ ($1 \leq j \leq r$) de K tels que les $W_{a_j}$ forment un recouvrement de K ($1 \leq j \leq r$). Considérons une partition continue de l’unité $(g_j)_{1 \leq j \leq r}$ sur K, subordonnée au recouvrement $(W_{a_j})$, et posons $\alpha_j = \mu(g_j)$ pour tout $j$; si $\alpha_j \neq 0$, posons $\mu_j = \alpha_j^{-1} g_j \cdot \mu$, et si $\alpha_j = 0$, posons $\mu_j = \varepsilon_{a_j}$. Chacune des mesures $\mu_j$ est positive, de masse totale 1, et son support est contenu dans l’ensemble convexe compact $W_{a_j}$; en outre, on a par définition

$$
\mu = \sum_{j=1}^r \alpha_j \mu_j
$$

puisque $g_j \cdot \mu = 0$ si $\mu(g_j) = 0$; les $\alpha_j$ sont $\geq 0$ et l’on a

$$
\sum_{j=1}^r \alpha_j = \sum_{j=1}^r \mu(g_j) = \mu \left( \sum_{j=1}^r g_j \right) = \mu(1) = 1.
$$

Soit $x_j$ le barycentre de $\mu_j$, qui appartient à $W_{a_j}$ (n° 1, prop. 1), et considérons la mesure discrète $v = \sum_{j=1}^r \alpha_j \varepsilon_{x_j}$; elle est positive et de masse totale 1, et son barycentre est $\sum_{j=1}^r \alpha_j x_j$, qui est aussi le barycentre de $\mu$ en vertu de (3), donc égal à $x$. Par ailleurs, en vertu de (2), on a $|f_i(y) - f_i(a)| \leq \delta/2$ pour tout $y \in W_{a_j}$ et tout $i$, d’où, puisque $\operatorname{Supp}(\mu_j) \subset W_{a_j}$, $|\mu_j(f_i) - f_i(a_j)| \leq \delta/2$ pour $1 \leq i \leq p$. D’autre part, comme $x_j \in W_{a_j}$, on a aussi

$$
|\varepsilon_{x_j}(f_i) - f_i(a_j)| \leq \delta/2
$$

pour $1 \leq i \leq p$, d’où $|\mu_j(f_i) - \varepsilon_{x_j}(f_i)| \leq \delta$ quels que soient $i, j$. Comme les $\alpha_j$ sont $\geq 0$ et ont pour somme 1, on déduit de (3) et de la définition de $v$ que $v$ vérifie l’inégalité (1).

C.Q.F.D.

#### Corollaire {#int-iv-s7-n2-cor-1 .statement}

Soit $K'$ une partie compacte de K telle que K soit l’enveloppe convexe fermée de K. Pour que $x \in K'$ soit point extrémal de K, il faut et il suffit que $\varepsilon_x$ soit la seule mesure positive sur $K'$, de masse totale 1, ayant $x$ pour barycentre.

Supposons que $x$ soit point extrémal de $K$; pour prouver que $\varepsilon_x$ est la seule mesure positive sur $K'$, de masse totale 1, ayant $x$ pour barycentre, il suffit de voir, en vertu de la prop. 3, que l’ensemble des mesures discrètes $v$ sur $K'$, positives, de masse totale 1 et ayant $x$ pour barycentre, est réduit à $\varepsilon_x$. Mais une telle mesure $v$ est de la forme $\sum_{i=1}^r \lambda_i \varepsilon_{x_i}$ avec $\lambda_i > 0$ pour $1 \leq i \leq r$ et $\sum_{i=1}^r \lambda_i = 1$; et l’hypothèse que $x$ est barycentre de $v$ s’écrit $x = \sum_{i=1}^r \lambda_i x_i$. Comme $x$ est extrémal, cela entraîne $x_i = x$ pour tout $i$, d’où $v = \varepsilon_x$.

Inversement, supposons que $\varepsilon_x$ soit la seule mesure positive sur $K'$, de masse totale 1, ayant $x$ pour barycentre, et montrons que $x$ est extrémal. Dans le cas contraire, il y aurait deux points distincts $x', x''$ de $K$ et un nombre réel $\lambda$ tels que $0 < \lambda < 1$ et
$$
x = \lambda x' + (1 - \lambda)x''.
$$
D’après la prop. 1, $x'$ (resp. $x''$) est barycentre d’une mesure positive $\mu'$ (resp. $\mu''$) de masse totale 1 sur $K'$. Alors $x$ est barycentre de $\lambda \mu' + (1 - \lambda)\mu''$. Donc $\lambda \mu' + (1 - \lambda)\mu'' = \varepsilon_x$. Donc $\mu'$ et $\mu''$ sont proportionnelles à $\varepsilon_x$, d’où $x' = x'' = x$, ce qui est absurde.

**Théorème 1** (Choquet).—Soient $E$ un espace localement convexe séparé sur $\mathbf{R}$, $K$ une partie convexe compacte et métrisable de $E$, $M$ l’ensemble des points extrémaux de $K$. L’ensemble $M$ est intersection d’une famille dénombrable de parties ouvertes de $K$, et tout point de $K$ est barycentre d’une mesure $\mu$ sur $K$ telle que $\mu(K - M) = 0$.

Pour démontrer la première assertion, désignons par $I$ l’intervalle $[0, 1]$ de $\mathbf{R}$; puisque $K$ est compact et métrisable, il en est de même de $K \times K \times I$; le sous-ensemble $U$ de $K \times K \times I$ formé des triplets $(x, y, \lambda)$ tels que $x \neq y$ et $0 < \lambda < 1$ est ouvert dans $K \times K \times I$, et il y a donc une suite $(F_n)$ d’ensembles fermés dans $K \times K \times I$ dont $U$ est réunion (*Top. gén.*, chap. IX, 2e éd., § 2, n° 5, prop. 7). L’application $q : K \times K \times I \to K$ définie par $q(x, y, \lambda) = \lambda x + (1 - \lambda)y$ est continue, et par définition des points extrémaux, on a $K - M = q(U) = \bigcup_n q(F_n)$; mais $F_n$ est compact puisqu’il est fermé dans $K \times K \times I$, donc $q(F_n)$ est compact, et par suite fermé dans K ; l’ensemble $U_n = K - q(F_n)$ est donc ouvert dans K, et l’on a $M = \bigcap_n U_n$.

Dans la suite de la démonstration, on désignera par $u$ une fonction numérique continue et *convexe* dans K, par $G \subset E \times \mathbf{R}$ le graphe de $u$, par S l’*enveloppe convexe fermée* de G dans $E \times \mathbf{R}$.

#### Lemme 1 {#int-iv-s7-lem-1 .statement}

*Soit $\bar{u}$ l’enveloppe inférieure des fonctions linéaires affines continues dans E et $\geq u$ dans K. Alors S est l’ensemble des points $(\mathbf{a}, b) \in E \times \mathbf{R}$ tels que l’on ait*

$$
\mathbf{a} \in K \quad \text{et} \quad u(\mathbf{a}) \leq b \leq \bar{u}(\mathbf{a}).
$$

En vertu du th. de Hahn–Banach, pour que $(\mathbf{a}, b)$ appartienne à S, il faut et il suffit que $h(\mathbf{a}, b) \geq 0$ pour toute fonction linéaire affine continue $h$ sur $E \times \mathbf{R}$ telle que $h(x, u(x)) \geq 0$ pour $x \in K$. Posant $h(x, t) = f(x) - \lambda t$, où $f$ est une fonction linéaire affine continue dans E, on voit que la relation $(\mathbf{a}, b) \in S$ équivaut à la propriété suivante: la relation

(4)
$$
f(x) \geq \lambda u(x) \quad \text{pour tout } x \in K
$$
implique

(5)
$$
f(\mathbf{a}) \geq \lambda b.
$$

Faisons d’abord $\lambda = 0$; le fait que (4) implique (5) pour toute fonction linéaire affine continue $f$ sur E équivaut à la relation $\mathbf{a} \in K$ en vertu du th. de Hahn–Banach. En second lieu, faisons $\lambda = -1$ et remplaçons $f$ par $-f$; alors la relation $f(x) \leq u(x)$ dans K doit entraîner $f(\mathbf{a}) \leq b$. Mais comme $u$ est convexe et continue dans K, $u(\mathbf{a})$ est égal à la borne supérieure des $f(\mathbf{a})$ pour les fonctions linéaires affines continues $f$ sur E telles que $f(x) \leq u(x)$ dans K (*Esp. vect. top.*, chap. II, 2e éd., § 5, n° 3, cor. 6 de la prop. 4); on obtient donc la relation $b \geq u(\mathbf{a})$. Enfin, faisons $\lambda = 1$; dire que (4) entraîne (5) signifie alors, par définition, que $b \leq \bar{u}(\mathbf{a})$. Cela prouve le lemme, puisque la relation (4) (resp. (5)) est équivalente à celle qu’on obtient en multipliant les deux membres par un scalaire $> 0$.

#### Lemme 2 {#int-iv-s7-lem-2 .statement}

*Si u est strictement convexe dans K, on a $u(x) < \bar{u}(x)$ pour tout point non extrémal x de K.*

En effet, il existe alors deux points distincts y, z de K tels que $x = (y + z)/2$, d’où $u(x) < (u(y) + u(z))/2$ puisque $u$ est strictement convexe. Si $f$ est une fonction linéaire affine dans E, on a $f(x) = (f(y) + f(z))/2$; appliquant cette relation aux fonctions linéaires affines continues $f$ qui sont $\geq u$ dans $K$, il vient
$$
\bar{u}(x) \geq (\bar{u}(y) + \bar{u}(z))/2 \geq (u(y) + u(z))/2 > u(x).
$$
Ces lemmes étant établis, on a donc (lemme 1), pour tout $a \in K$, $(a, \bar{u}(a)) \in S$. Comme $G$ est compact, étant image de $K$ par l’application continue $x \mapsto (x, u(x))$, il existe, en vertu de la prop. 1 du n° 1, une mesure positive $\nu$ sur $G$, de masse totale 1, ayant $(a, \bar{u}(a))$ pour barycentre. Comme la restriction à $G$ de la projection $pr_1$ est un homéomorphisme de $G$ sur $K$, on peut transporter la mesure $\nu$ à l’aide de cet homéomorphisme, ce qui donne une mesure $\mu$ sur $K$ (positive et de masse totale 1) telle que l’on ait
$$
\text{(6)} \quad a = \int x \, d\mu(x) \quad \text{et} \quad \bar{u}(a) = \int u(x) \, d\mu(x).
$$
La première des relations (6) signifie que $a$ est le barycentre de $\mu$. La fonction $\bar{u}$ est semi-continue supérieurement et bornée dans $K$, donc $\mu$-intégrable ($§ 4$, n° 4, cor. 1 de la prop. 5); en outre, comme la fonction $-\bar{u}$ est convexe par définition, on a, en vertu du cor. de la prop. 2 du n° 1
$$
\text{(7)} \quad \bar{u}(a) \geq \int \bar{u}(x) \, d\mu(x)
$$
d’où, en comparant avec la seconde formule (6)
$$
\text{(8)} \quad \int u(x) \, d\mu(x) \geq \int \bar{u}(x) \, d\mu(x).
$$
Mais comme $u(x) \leq \bar{u}(x)$ dans $K$, la relation (8) implique que $u(x) = \bar{u}(x)$ presque partout pour $\mu$. Compte tenu du lemme 2, on voit que le théorème 1 sera démontré une fois établi le

#### Lemme 3 {#int-iv-s7-lem-3 .statement}

*Soient E un espace localement convexe séparé sur R, K un partie convexe compacte métrisable de E. Il existe une fonction numérique strictement convexe dans K.*

En effet, l’espace de Banach $\mathcal{C}(K; \mathbf{R})$ est de type dénombrable (*Top. gén.*, chap. X, 2e éd., § 3, n° 3, th. 1), et il en est donc de même du sous-espace $\mathcal{A}$ de $\mathcal{C}(K; \mathbf{R})$ formé des restrictions à $K$ des fonctions linéaires affines continues dans $E$. Soit donc $(h_n)$ une suite partout dense dans $\mathcal{A}$, et soit $\alpha_n > \sup_{x \in K} |h_n(x)|$. Alors, chacune des fonctions $h_n^2/n^2 \alpha_n^2$ est convexe dans $K$ (*Esp. vect. top.*, chap. II, 2e éd., § 2, n° 8, *Exemples*), et la série de terme général $h_n^2/n^2 \alpha_n^2$ est normalement convergente, donc sa somme $u$ est continue et convexe dans $K$. Il reste à voir que $u$ est strictement convexe, et pour cela, il suffit de prouver que pour deux points distincts $x, x'$ de $K$, il y a un entier $n$ tel que la restriction au segment d’extrémités x, x' de $h_n^2$ est strictement convexe; mais pour cela il suffit que $h_n(x) \neq h_n(x')$ (loc. cit.). Or, il y a une fonction $h \in \mathcal{A}$ telle que $h(x) \neq h(x')$ (Esp. vect. top., chap. II, 2e éd., § 4, n° 1, cor. 1 de la prop. 2) et comme la suite $(h_n)$ est dense dans $\mathcal{A}$, il existe un $n$ tel que $h_n(x) \neq h_n(x')$.

C.Q.F.D.

#### Corollaire {#int-iv-s7-n2-cor-2 .statement}

Soient E un espace localement convexe séparé sur $\mathbf{R}$, C un cône convexe saillant de sommet 0 dans E, complet et métrisable pour la structure uniforme induite par la structure uniforme affaiblie de E. Soit M la réunion des génératrices extrémales de C. Pour tout $x \in C$, il existe une partie compacte K de C et une mesure $\lambda \geq 0$ de masse 1 sur K, telles que $K - (M \cap K)$ soit $\lambda$-négligeable et que le barycentre de $\lambda$ soit égal à x.

En effet, x appartient à un chapeau de C (Esp. vect. top., chap. II, 2e éd., §7, n° 2, prop. 5), et $M \cap K$ contient l’ensemble des points extrémaux de K (loc. cit., cor. 1 de la prop. 4). Il suffit alors d’appliquer le th. 1.

### 3. Applications: I. Espaces vectoriels de fonctions continues réelles

Soient X un espace compact non vide, $\mathcal{H}$ un sous-espace vectoriel de l’espace de Banach $\mathcal{C}(X; \mathbf{R})$ qui contient les constantes et sépare les points de X (Top. gén., chap. X, 2e éd., § 4, n° 1, déf. 1). Nous munirons $\mathcal{H}$ de la topologie d’espace normé induite par celle de $\mathcal{C}(X; \mathbf{R})$, et désignerons par $\mathcal{H}'$ le dual de cet espace normé. Pour tout $x \in X$, l’application $f \mapsto f(x)$ est une forme linéaire continue sur $\mathcal{H}$ (restriction à $\mathcal{H}$ de la mesure de Dirac $\varepsilon_x$), donc un élément de $\mathcal{H}'$ que nous noterons $i_{\mathcal{H}}(x)$, de sorte que l’on a
$$
\langle f, i_{\mathcal{H}}(x) \rangle = f(x)
$$
pour toute fonction $f \in \mathcal{H}$ et tout $x \in X$.

L’application $i_{\mathcal{H}}$ de X dans $\mathcal{H}'$ est injective et continue lorsqu’on munit $\mathcal{H}'$ de la topologie faible $\sigma(\mathcal{H}', \mathcal{H})$; la seconde assertion résulte aussitôt des définitions et de (9); quant à la première, notons que si $x, x'$ sont deux points distincts de X, il existe par hypothèse une fonction $h \in \mathcal{H}$ telle que $h(x) \neq h(x')$, donc, en vertu de (9), $\langle h, i_{\mathcal{H}}(x) \rangle \neq \langle h, i_{\mathcal{H}}(x') \rangle$ et a fortiori $i_{\mathcal{H}}(x) \neq i_{\mathcal{H}}(x')$. L’image $i_{\mathcal{H}}(X)$ est donc une partie compacte de $\mathcal{H}'$ (pour la topologie faible), et $i_{\mathcal{H}}$ un homéomorphisme de X sur $i_{\mathcal{H}}(X)$.

#### Proposition 4 {#int-iv-s7-prop-4 .statement}

(i) L’enveloppe convexe fermée C de $i_{\mathcal{H}}(X)$ dans $\mathcal{H}'$ (pour la topologie faible $\sigma(\mathcal{H}', \mathcal{H})$) est compacte.

(ii) Pour qu’un point $i_{\mathcal{H}}(x)$ soit point extrémal de C, il faut et il suffit que la seule mesure positive $\lambda$ sur X, telle que
$$
h(x) = \int h \, d\lambda
$$
pour toute fonction $h \in \mathcal{H}$ (ce qui entraîne en particulier que $\lambda$ est de masse totale 1 puisque $1 \in \mathcal{H}$) soit la mesure de Dirac $\varepsilon_x$.

La fonction $z' \mapsto \langle h, z' \rangle$ sur C atteint sa borne supérieure en un point extrémal de C au moins (*Esp. vect. top.*, chap. II, 2e éd., § 7, n° 1, prop. 1), et ce point appartient à $i_{\mathcal{H}}(X)$ (*loc. cit.*, cor. de la prop. 2).

(i) D’après (9), on a $\| i_{\mathcal{H}}(x) \| \leq 1$ dans l’espace normé $\mathcal{H}'$, autrement dit, $i_{\mathcal{H}}(X)$ est borné, et l’assertion résulte de ce que $\mathcal{H}'$, muni de la topologie faible $\sigma(\mathcal{H}', \mathcal{H})$, est quasi-complet (*Esp. vect. top.*, chap. IV, § 2, n° 2, cor. 2 du th. 1).

(ii) Toute mesure positive $\mu$ de masse 1 sur $i_{\mathcal{H}}(X)$ provient, par transport de structure au moyen de l’homéomorphisme $i_{\mathcal{H}}$, d’une mesure positive $\lambda$ de masse 1 sur X, la mesure de Dirac $\varepsilon_{i_{\mathcal{H}}(x)}$ provenant de $\varepsilon_x$. Dire que $\mu$ admet $i_{\mathcal{H}}(x)$ pour barycentre signifie, par définition, que l’on a
$$
\int_X \langle h, i_{\mathcal{H}}(z) \rangle \, d\lambda(z) = \langle h, i_{\mathcal{H}}(x) \rangle
$$
pour toute fonction $h \in \mathcal{H}$. Compte tenu de (9), l’assertion (ii) n’est autre que la traduction du critère du n° 2, cor. de la prop. 3, pour que $i_{\mathcal{H}}(x)$ soit point extrémal de C.

Nous dirons qu’un point $x \in X$ vérifiant la condition (ii) de la prop. 4 est $\mathcal{H}$-extrémal ; nous désignerons par $\mathrm{Ch}_{\mathcal{H}}(X)$ (ou simplement $\mathrm{Ch}(X)$) l’ensemble de ces points, par $\check{S}_{\mathcal{H}}(X)$ (ou simplement $\check{S}(X)$) l’adhérence de $\mathrm{Ch}_{\mathcal{H}}(X)$ dans X.

#### Proposition 5 {#int-iv-s7-prop-5 .statement}

Toute fonction $h \in \mathcal{H}$ atteint sa borne supérieure en un point $\mathcal{H}$-extrémal au moins.

Soient $x$ un point de X, $h$ une fonction de $\mathcal{H}$. La relation $h(z) \leq h(x)$ pour tout $z \in X$ s’écrit $\langle h, i_{\mathcal{H}}(z) \rangle \leq \langle h, i_{\mathcal{H}}(x) \rangle$ pour tout $z \in X$, et signifie donc que l’hyperplan faiblement fermé de $\mathcal{H}'$, d’équation $\langle h, t' \rangle = \langle h, i_{\mathcal{H}}(x) \rangle$ est un hyperplan d’appui de $i_{\mathcal{H}}(X)$. On sait (*Esp. vect. top.*, chap. II, 2e éd., § 7, n° 1, cor. 1 de la prop. 1), qu’un tel hyperplan contient un point extrémal au moins de $i_{\mathcal{H}}(X)$, et un tel point $i_{\mathcal{H}}(y)$ est l’image d’un point $\mathcal{H}$-extrémal $y$ par définition ; $h(y)$ est donc égal à la borne supérieure de $h$ dans X.

#### Proposition 6 {#int-iv-s7-prop-6 .statement}

Pour tout point $x \in X$, les propriétés suivantes sont équivalentes :

a) $x$ est $\mathcal{H}$-extrémal.

b) Pour tout voisinage ouvert $U$ de $x$ dans $X$ et tout $\varepsilon > 0$, il existe une fonction $h \geq 0$ dans $\mathcal{H}$ telle que $h(x) \leq \varepsilon$ et $h(y) \geq 1$ pour tout $y \in X - U$.

Soient $x$ un point quelconque de $X$, $f$ une fonction de $\mathcal{C}(X; \mathbf{R})$; on sait (*Esp. vect. top.*, chap. II, 2e éd., § 3, n° 1, prop. 1) que la borne inférieure des nombres $\lambda(f)$, pour toutes les mesures positives sur $X$ telles que $\lambda(h) = h(x)$ pour toute fonction $h \in \mathcal{H}$, est égale à la borne supérieure des nombres $h(x)$, où $h$ parcourt l’ensemble des fonctions $h \in \mathcal{H}$ telles que $h \leq f$. Supposons que $x$ soit $\mathcal{H}$-extrémal; alors il résulte de la prop. 4, (ii), que, pour toute fonction $f \in \mathcal{C}(X; \mathbf{R})$, on a
$$
f(x) = \sup_{h \in \mathcal{H}, h \leq f} h(x).
$$
Pour montrer que a) entraîne b), prenons pour $f$ une application continue de $X$ dans $\{0, 1\}$, de support contenu dans $U$ et telle que $f(x) = 1$; il y a donc en vertu de (11) une fonction $h' \in \mathcal{H}$ telle que $h' \leq f$ et $h'(x) \geq 1 - \varepsilon$. Comme $1 \in \mathcal{H}$, la fonction $h = 1 - h'$ répond aux conditions de b).

Réciproquement, supposons vérifiée la condition b); cette condition entraîne que $1 - h \leq \varphi_U$; pour toute mesure positive $\lambda$ sur $X$ vérifiant la condition (7), on a donc
$$
\lambda(U) = \lambda(\varphi_U) \geq \lambda(1 - h) = 1 - h(x) \geq 1 - \varepsilon.
$$
Comme par hypothèse cette relation a lieu pour tout $\varepsilon > 0$ et tout voisinage ouvert $U$ de $x$, on en conclut
$$
\lambda(\{x\}) = \inf_U \lambda(U) \geq 1 - \varepsilon
$$
pour tout $\varepsilon > 0$, donc $\lambda(\{x\}) = 1$. Comme $\lambda$ est positive et de masse totale 1, on a nécessairement $\lambda = \varepsilon_x$, ce qui prouve que $x$ est $\mathcal{H}$-extrémal en vertu de la prop. 4, (ii).

#### Proposition 7 {#int-iv-s7-prop-7 .statement}

Soit $F$ une partie fermée de $X$. Les propriétés suivantes sont équivalentes :

a) $F$ contient $\check{S}_{\mathcal{H}}(X)$.

b) Pour toute fonction $h \in \mathcal{H}$, l’ensemble $F$ rencontre l’ensemble des points de $X$ où $h$ atteint sa borne supérieure.

c) Pour tout point $x \in X$, il existe une mesure positive $\mu$ de masse 1 sur $X$, telle que $\operatorname{Supp}(\mu) \subset F$ et que $h(x) = \int h \, d\mu$ pour toute fonction $h \in \mathcal{H}$.

Soit $G = i_{\mathcal{H}}(F)$. La condition *a*) signifie que $G$ contient l’ensemble des points extrémaux de $C$. La condition *b*) signifie que $G$ rencontre l’intersection de $i_{\mathcal{H}}(X)$ avec chacun des hyperplans d’appui fermés de $i_{\mathcal{H}}(X)$. Enfin la condition *c*) signifie que tout point de $i_{\mathcal{H}}(X)$ est barycentre d’une mesure de support contenu dans $G$; en vertu du n° 1, prop. 1, cela équivaut encore à dire que l’enveloppe convexe fermée de $i_{\mathcal{H}}(X)$ est égale à l’enveloppe convexe fermée de $G$. L’équivalence des conditions *a)*, *b)* et *c*) résulte donc d’*Esp. vect. top.*, chap. II, 2° éd., § 7, n° 1, cor. 2 de la prop. 2.

#### Proposition 8 {#int-iv-s7-prop-8 .statement}

Supposons $X$ métrisable. *Alors l’ensemble* $\mathrm{Ch}_{\mathcal{H}}(X)$ *des points* $\mathcal{H}$-*extrémaux de* $X$ *est intersection d’une famille dénombrable d’ensembles ouverts dans* $X$, *et pour tout* $x \in X$, *il existe une mesure positive* $\mu$ *de masse* 1 *sur* $X$ *telle que*
$$
\mu(X - \mathrm{Ch}_{\mathcal{H}}(X)) = 0 \quad \text{et} \quad \int h \, d\mu = h(x)
$$
*pour toute* $h \in \mathcal{H}$.

C’est la traduction du th. 1 du n° 2, par transport de structure au moyen de l’homéomorphisme $x \mapsto i_{\mathcal{H}}(x)$, comme dans la prop. 5.

Un certain nombre de résultats de ce n° s’étendent lorsqu’on remplace $\mathcal{H}$ par un ensemble $\mathcal{P}$ de fonctions définies dans $X$, à valeurs dans $\mathbf{R} \cup \{+\infty\}$, semi-continues inférieurement, $\mathcal{P}$ étant supposé contenir les constantes et être tel que $\mathcal{P} + \mathcal{P} \subset \mathcal{P}$ (exerc. 2).

#### Exemple {#int-iv-s7-n3-exa-1 .statement}

Prenons pour $X$ la boule unité $\|x\| \leq 1$ dans $\mathbf{R}^3$, et soit $\mathcal{H}$ un espace vectoriel de fonctions continues dans $X$, contenant les restrictions à $X$ des fonctions linéaires affines dans $\mathbf{R}^3$, et vérifiant le « principe du maximum », c’est-à-dire que pour toute fonction $h \in H$ non constante, l’ensemble des points de $X$ où $h$ atteint sa borne supérieure est contenu dans la sphère $S_2$. Il résulte alors aisément des prop. 5 et 7 que $\mathrm{Ch}_{\mathcal{H}}(X) = \tilde{S}_{\mathcal{H}}(X) = S_2$. Un exemple important d’espace vectoriel $\mathcal{H}$ vérifiant les conditions précédentes est l’ensemble des fonctions continues dans $X$ et *harmoniques* dans la boule ouverte $\|x\| < 1$. Pour ces fonctions, on démontre que la mesure positive $\mu$ de masse 1 telle que $\mathrm{Supp}(\mu) \subset S_2$ et que $h(x) = \int h \, d\mu$ pour toute $h \in \mathcal{H}$, est donnée, si $\|x\| < 1$, par la formule de Poisson
$$
d\mu(z) = \frac{1 - \|z\|^2}{\|z - x\|^3} d\sigma(z)
$$
où $\sigma$ est la mesure sur $S_2$ invariante par le groupe orthogonal et telle que $\sigma(S_2) = 1$ (chap. VII, § 3, exerc. 8).*

### 4. Applications. II. Espaces vectoriels de fonctions continues complexes

Soient X un espace compact non vide, $\mathcal{H}$ un sous-espace vectoriel de l’espace de Banach complexe $\mathcal{C}(X; \mathbf{C})$ qui contient les constantes et sépare les points de X. L’ensemble des parties réelles $\mathcal{R}(f)$ des fonctions $f \in \mathcal{H}$ est un sous-espace vectoriel $\mathcal{H}_r$ de l’espace vectoriel réel $\mathcal{C}(X; \mathbf{R})$; pour toute $f \in \mathcal{H}$, l’ensemble $\mathcal{H}_r$ contient aussi $\mathcal{J}(f) = \mathcal{R}(-if)$; il en résulte que $\mathcal{H}_r$ sépare les points de X puisque la relation $h(x) = h(y)$ pour toute $h \in \mathcal{H}_r$ entraîne $\mathcal{R}(f(x)) = \mathcal{R}(f(y))$ et $\mathcal{J}(f(x)) = \mathcal{J}(f(y))$, donc $f(x) = f(y)$ pour toute $f \in \mathcal{H}$. Les points $\mathcal{H}_r$-extrémaux dans X sont encore appelés $\mathcal{H}$-extrémaux, et on note leur ensemble $\mathrm{Ch}_{\mathcal{H}}(X)$, et l’adhérence de ce dernier $\check{S}_{\mathcal{H}}(X)$. Les analogues des prop. 5 et 7 sont les suivantes :

#### Proposition 9 {#int-iv-s7-prop-9 .statement}

Pour toute fonction $f \in \mathcal{H}$, $\mathrm{Ch}_{\mathcal{H}}(X)$ rencontre l’ensemble des points où $|f|$ atteint sa borne supérieure.

On peut se borner au cas où $f$ n’est pas la constante 0. Soit $a$ un point de X où $|f|$ atteint sa borne supérieure, et posons $g = f/f(a)$; on a $g(a) = 1$ et $|g(x)| \leq 1$ pour tout $x \in X$, d’où
$$
\mathcal{R}(g(a)) = 1 \quad \text{et} \quad \mathcal{R}(g(x)) \leq 1 \text{ pour tout } x \in X.
$$
En vertu de la prop. 5 du n° 3 appliquée à $\mathcal{H}_r$, il existe $b \in \mathrm{Ch}_{\mathcal{H}}(X)$ où $\mathcal{R}(g(x))$ atteint sa borne supérieure 1, d’où $|g(b)| = 1$ puisque $|g(b)| \leq 1$; on en conclut que $|f(b)| = |f(a)| \geq |f(x)|$ pour tout $x \in X$.

#### Proposition 10 {#int-iv-s7-prop-10 .statement}

Soit F une partie fermée de X. Les propriétés suivantes sont équivalentes :
a) F contient $\check{S}_{\mathcal{H}}(X)$.
b) Pour toute fonction $f \in \mathcal{H}$, F rencontre l’ensemble des points de X où $|f|$ atteint sa borne supérieure.
c) Pour tout point $x \in X$, il existe une mesure positive $\mu$ de masse totale 1 sur X telle que $\mathrm{Supp}(\mu) \subset F$ et que $f(x) = \int f \, d\mu$ pour toute fonction $f \in \mathcal{H}$.

Prouvons l’équivalence des conditions a) et c): soit $f = f_1 + if_2$ avec $f_1, f_2$ dans $\mathcal{H}_r$; la relation $f(x) = \int f \, d\mu$ équivaut aux deux relations $f_1(x) = \int f_1 \, d\mu$ et $f_2(x) = \int f_2 \, d\mu$; il suffit donc d’appliquer à $\mathcal{H}_r$ l’équivalence des conditions a) et c) de la prop. 7 du n° 3. Le fait que a) entraîne b) résulte de la prop. 9. Montrons que b) entraîne a); il s’agit de voir que si b) est vérifiée, alors, pour toute $h \in \mathcal{H}_r$, F rencontre l’ensemble des points où $h$ atteint sa borne inférieure dans X. La condition b) entraîne que F est non vide; comme F est compact, il existe $a \in F$ tel que $h(a) \leq h(y)$ pour tout $y \in F$. Soit $f \in \mathcal{H}$ telle que $h = \mathcal{R}(f)$; pour tout $\varepsilon > 0$, la fonction $g = f - h(a) + \varepsilon$ appartient à $\mathcal{H}$, et l’on a
$$
\mathcal{R}(g(y)) = h(y) - h(a) + \varepsilon \geq \varepsilon
$$
pour tout $y \in F$. Soit c la borne supérieure de $|g|$ dans X, et posons $b = c^2 / 2\varepsilon$; pour tout $y \in F$, on a
$$
|g(y) - b|^2 = |g(y)|^2 - 2b \mathcal{R}(g(y)) + b^2 \leq c^2 - 2b\varepsilon + b^2 = b^2,
$$
autrement dit, la borne supérieure dans F de la fonction $|g - b|$ est $\leq b$. Comme $g - b \in \mathcal{H}$, l’hypothèse faite sur F entraîne $|g - b| \leq b$, d’où
$$
b^2 \geq |g - b|^2 = |g|^2 - 2b \mathcal{R}(g) + b^2
$$
et par suite $\mathcal{R}(g) \geq |g|^2 / 2b \geq 0$; comme $\mathcal{R}(g) = h - h(a) + \varepsilon$, et que $\varepsilon > 0$ est arbitraire, on a $h \geq h(a)$, et $h(a)$ est la borne inférieure de $h$ dans X, ce qui achève la démonstration.

#### Remarque {#int-iv-s7-n4-rem-1 .statement}

Si $f$ est une fonction continue réelle, un point où $|f|$ atteint sa borne supérieure est un point où l’une des fonctions $f, -f$ atteint sa borne supérieure. Pour un espace vectoriel $\mathcal{H}$ de fonctions continues réelles vérifiant les hypothèses du n° 3, les prop. 9 et 10 sont donc des corollaires triviaux des prop. 5 et 7 respectivement.

### 5. Applications: III. Algèbres de fonctions continues

#### Lemme 4 {#int-iv-s7-lem-4 .statement}

Soient X un espace compact, $\mathcal{H}$ un sous-espace vectoriel fermé de l’espace de Banach $\mathcal{C}(X; \mathbf{C})$ (resp. $\mathcal{C}(X; \mathbf{R})$). Soit a un point de X admettant un système fondamental dénombrable de voisinages; on suppose que, quels que soient les nombres c et d tels que $0 < c < d < 1$, et le voisinage ouvert U de a, il existe $f \in \mathcal{H}$ telle que
(12) $|f| \leq 1,\quad |f(a)| \geq d,\quad |f(x)| \leq c$ pour tout $x \in X - U$.
Alors il existe une fonction $u \in \mathcal{H}$ telle que $|u(x)| < |u(a)|$ pour tout $x \neq a$.

Soit $(V_n)$ ($n \geq 1$) un système fondamental de voisinages de a, et soient $\lambda, \mu, \varepsilon$ des nombres tels que
$$
0 < \lambda < 1,\quad 1 < \mu < \mu + \varepsilon \leq 1 + \lambda.
$$
On a donc $0 < \lambda / \mu < 1 / \mu < 1$. Nous allons définir par récurrence sur $n$ ($n \geq 1$) une suite décroissante $(U_n)$ de voisinages ouverts de a tels que $U_n \subset V_n$ pour tout $n$, et une suite $(h_n)$ de fonctions de $\mathcal{H}$ vérifiant les relations

$$(13_n)$$ $|h_n(x)| \leq \mu$ pour tout $x \in X$
$$(14_n)$$ $h_n(a) = 1$
$$(15_n)$$ $|h_n(x)| \leq \lambda$ pour tout $x \in X - U_n$
$$(16_n)$$ $$\left| \sum_{j=1}^n \lambda^j h_j(y) \right| < \sum_{j=1}^{n+1} \lambda^j$$ pour tout $y \in X$.

Supposons les $h_m$ et $U_m$ définis pour $1 \leq m < n$ et vérifiant les quatre conditions précédentes (où $n$ est remplacé par $m$); posons d’autre part $U_0 = X$. La fonction $\sum_{j=1}^{n-1} \lambda^j h_j$ (égale à 0 si $n = 1$) est continue et prend la valeur $\sum_{j=1}^{n-1} \lambda^j$ au point $a$; il existe donc un voisinage ouvert $U_n$ de $a$, contenu dans $U_{n-1} \cap V_n$, tel que l’on ait
$$(17)$$ $$\left| \sum_{j=1}^{n-1} \lambda^j h_j(y) \right| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n$$ pour tout $y \in U_n$.

Par hypothèse il existe une fonction $f \in \mathcal{H}$ telle que
$$
\begin{align*}
|f(x)| &\leq 1 \text{ pour tout } x \in X, \quad |f(a)| \geq 1/\mu, \\
|f(x)| &\leq \lambda/\mu \quad \text{pour } x \in X - U_n.
\end{align*}
$$
Posons $h_n = f/f(a)$; on a donc les relations $(13_n)$, $(14_n)$ et $(15_n)$; posons
$$
g = \sum_{j=1}^n \lambda^j h_j = \sum_{j=1}^{n-1} \lambda^j h_j + \lambda^n h_n.
$$
En vertu de (17) et de $(13_n)$, on a, pour $y \in U_n$
$$
|g(y)| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n + \mu \lambda^n \leq \sum_{j=1}^{n+1} \lambda^j,
$$
puisque $\varepsilon + \mu \leq 1 + \lambda$; pour $x \in X - U_n$, on a $|h_p(x)| \leq \lambda$ pour $1 \leq p \leq n$, d’où encore
$$
|g(x)| \leq \sum_{j=2}^{n+1} \lambda^j < \sum_{j=1}^{n+1} \lambda^j
$$
ce qui achève de prouver $(16_n)$.

Cela étant, la série $\sum_{n=1}^\infty \lambda^n h_n$ est normalement convergente dans $X$ puisque $\lambda < 1$ et $|h_n(x)| \leq \mu$ pour tout $n$ et tout $x \in X$; soit $u$ sa somme, qui appartient à $\mathcal{H}$ puisque $\mathcal{H}$ est fermé. En vertu de la n° 5

relation (14_n), on a $u(a) = \sum_{n=1}^{\infty} \lambda^n$; d’autre part, si $x \neq a$, il existe un entier $n$ tel que $x \notin U_{n+1}$; on a donc $|h_{n+k}(x)| \leq \lambda$ pour tout $k \geq 1$ en vertu de la relation (15_n); on en déduit, en utilisant (16_n)

$$
|u(x)| \leq \left| \sum_{j=1}^{n} \lambda^j h_j(x) \right| + \left| \sum_{j=n+1}^{\infty} \lambda^j h_j(x) \right| < \sum_{j=1}^{n+1} \lambda^j + \lambda \sum_{j=n+1}^{\infty} \lambda^j
$$
$$
= \sum_{j=1}^{\infty} \lambda^j = |u(a)|.
$$

#### Théorème 2 (E. Bishop) {#int-iv-s7-thm-2 .statement}

Soient X un espace compact, $\mathcal{A}$ une sous-algèbre fermée de l’algèbre de Banach complexe $\mathcal{C}(X; \mathbf{C})$. On suppose que $\mathcal{A}$ contient les constantes et sépare les points de X. Soit a un point de X ; les conditions suivantes sont équivalentes :

a) Il existe une fonction $f \in \mathcal{A}$ telle que $|f(x)| < |f(a)|$ pour tout $x \neq a$.

b) Le point a est $\mathcal{A}$-extrémal et admet un système fondamental dénombrable de voisinages.

a) $\Rightarrow$ b) : Soit $f \in \mathcal{A}$ telle que $|f(a)| > |f(x)|$ pour $x \neq a$; en vertu de la prop. 9 du n° 4, a est un point $\mathcal{A}$-extrémal. D’autre part, si $U_n$ est l’ensemble des $x \in X$ tels que $|f(x)| > |f(a)| - 1/n$, $U_n$ est un voisinage ouvert de a, et l’intersection des $U_n$ est réduite à a ; comme X est compact, les $U_n$ forment un système fondamental de voisinages de a (Top. gén., chap. I, 3e éd., § 9, n° 1, th. 1).

b) $\Rightarrow$ a) : Il suffit de vérifier que b) implique les hypothèses du lemme 4. Avec les notations de ce lemme, posons $\varepsilon = \log d / \log c$; on a $0 < \varepsilon < 1$. Comme a est un point $\mathcal{A}_r$-extrémal, il existe une fonction $g \in \mathcal{A}$ telle que

$$
\mathcal{R}(g) \geq 0, \quad \mathcal{R}(g(a)) \leq \varepsilon, \quad \mathcal{R}(g(x)) \geq 1 \quad \text{pour } x \in X - U
$$
(n° 3, prop. 6, b)). Posons $f = c^g$; comme $f$ est somme de la série normalement convergente $\sum_{n=0}^{\infty} (\log c)^n g^n / n!$, on a $f \in \mathcal{A}$, et
$$
|f| \leq 1, \quad |f(a)| \geq c^{\varepsilon} = d, \quad |f(x)| \leq c \quad \text{pour } x \in X - U.
$$

C.Q.F.D.

#### Corollaire {#int-iv-s7-n5-cor-1 .statement}

Supposons de plus que X soit métrisable. Alors les propriétés suivantes sont équivalentes :

a) a est un point $\mathcal{A}$-extrémal de X.
b) Il existe $u \in \mathcal{A}$ tel que $|u(x)| < |u(a)|$ pour tout $x \neq a$.

c) Soit $\mathfrak{M}$ l’ensemble des parties $M$ de $X$ telles que pour toute fonction $f \in \mathcal{A}$, $|f|$ atteigne sa borne supérieure dans $X$ en un point au moins de $M$. Alors $a$ appartient à tous les ensembles $M \in \mathfrak{M}$.

d) Soit $\mathfrak{N}$ l’ensemble des parties $N$ de $X$ telles que, pour toute fonction $f \in \mathcal{A}$, $\Re(f)$ atteigne sa borne supérieure dans $X$ en un point au moins de $N$. Alors $a$ appartient à tous les ensembles $N \in \mathfrak{N}$.

En d’autres termes, on a

$$
\mathrm{Ch}_{\mathcal{A}}(X) = \bigcap_{M \in \mathfrak{M}} M = \bigcap_{N \in \mathfrak{N}} N.
$$

Comme, dans un espace métrisable, tout point admet un système fondamental dénombrable de voisinages, l’équivalence de a) et b) résulte du th. 2. Montrons que b) entraîne c): en effet $a$ est l’unique point où $|u|$ atteint sa borne supérieure; d’autre part, c) entraîne a), car $\mathrm{Ch}_{\mathcal{A}}(X)$ rencontre, pour tout $f \in \mathcal{A}$, l’ensemble des points où $|f|$ atteint sa borne supérieure (n° 4, prop. 9). Le même raisonnement utilisant la prop. 5 du n° 3 montre que d) entraîne a). Enfin, pour voir que b) entraîne d), on peut se borner au cas où $X$ n’est pas réduit au point $a$, donc $u(a) \neq 0$; la fonction $v = u/u(a)$ appartient alors à $\mathcal{A}$, et l’on a $v(a) = 1$ et $|v(x)| < 1$ pour $x \neq a$, d’où $\Re(v(a)) = 1$ et $\Re(v(x)) < 1$ pour $x \neq a$. La fonction $\Re(v)$ n’atteignant sa borne supérieure qu’au point $a$, on a bien $a \in N$ pour tout $N \in \mathfrak{N}$.

#### Exemple {#int-iv-s7-n5-exa-1 .statement}

Soit $X_1$ l’ensemble des points $(z_1, z_2) \in \mathbf{C}^2$ tels que $|z_1|^2 + |z_2|^2 \leq 1$ (boule unité dans $\mathbf{R}^4$), et soit $\mathcal{A}_1'$ l’ensemble des restrictions à $X_1$ des fonctions holomorphes, à valeurs dans $\mathbf{C}$, définies dans un voisinage de $X_1$ dans $\mathbf{C}^2$ (voisinage dépendant de la fonction considérée); soit $\mathcal{A}_1$ l’adhérence de $\mathcal{A}_1'$ dans $\mathcal{C}(X_1 ; \mathbf{C})$, qui est évidemment une sous-algèbre complexe fermée de $\mathcal{C}(X_1 ; \mathbf{C})$ et sépare les points de $X_1$. L’application du « principe du maximum » pour les fonctions holomorphes montre que $\mathrm{Ch}_{\mathcal{A}_1}(X_1)$ est la sphère $S_3$.

Dans la définition précédente, remplaçons $X_1$ par le « polydisque » $X_2$ défini par les relations $|z_1| \leq 1$ et $|z_2| \leq 1$, ce qui donne des sous-algèbres $\mathcal{A}_2'$ et $\mathcal{A}_2$ (adhérence de $\mathcal{A}_2'$) dans $\mathcal{C}(X_2 ; \mathbf{C})$. Ici le principe du maximum montre que $\mathrm{Ch}_{\mathcal{A}_2}(X_2)$ est le « tore » défini par les relations $|z_1| = 1$ et $|z_2| = 1$.

On déduit de ces résultats qu’il n’existe pas d’isomorphisme analytique d’un voisinage ouvert de $X_1$ sur un voisinage ouvert de $X_2$ qui transforme $X_1$ en $X_2$; en effet, si $v$ était la restriction à $X_1$ d’une telle application, on aurait $\mathcal{A}_2 = v_* \mathcal{A}_1 v^{-1}$, et par suite $v$ transformerait $S_3$ en un espace homéomorphe à $T^2$, ce qui est absurde, car $S_3$ est simplement connexe, mais non $T^2$.

On notera toutefois que les espaces $X_1$ et $X_2$ sont homéomorphes, étant tous deux des ensembles convexes bornés dans $\mathbf{R}^4$ d’intérieur non vide.*

### 6. Unicité des représentations intégrales

Soient E un espace localement convexe séparé faible, C un cône convexe pointé saillant dans E. On sait que C est l’ensemble des éléments $\geqslant 0$ de E pour une relation d’ordre compatible avec la structure vectorielle de E. Quand on dira que C est réticulé, il s’agira bien entendu de l’ordre induit sur C par celui de E.

#### Lemme 5 {#int-iv-s7-lem-5 .statement}

On suppose C faiblement complet. Soit $\mathcal{A}$ l’ensemble des restrictions à C des formes linéaires continues sur E. Soient $(f_\lambda)_{\lambda \in \Lambda}$ une famille finie d’éléments de $\mathcal{A}$, et $f = \sup (f_\lambda)$. Pour tout $x \in C$, on pose

$$
\bar{f}(x) = \sup (f(x_1) + f(x_2) + \ldots + f(x_n))
$$

la borne supérieure étant prise sur l’ensemble $S_x$ des suites $(x_1, x_2, \ldots, x_n)$ d’éléments de C telles que $x_1 + x_2 + \ldots + x_n = x$. Posons Card $\Lambda = p$. Alors il existe $(y_1, \ldots, y_p) \in S_x$ tels que $\bar{f}(x) = f(y_1) + \ldots + f(y_p)$.

Notons $f_1, f_2, \ldots, f_p$ les éléments de la famille $(f_\lambda)$. Pour $k = 1, 2, \ldots, p$, soit $C_k$ l’ensemble des $y \in C$ tels que $f_1(y) < f(y), f_2(y) < f(y), \ldots, f_{k-1}(y) < f(y), f_k(y) = f(y)$. Les $C_k$ sont des cônes convexes disjoints de réunion C. Soient $x_1, x_2, \ldots, x_n$ dans C tels que $x_1 + x_2 + \ldots + x_n = x$. Soit $y_k$ la somme des $x_i$ qui appartiennent à $C_k$. On a $y_1 + y_2 + \ldots + y_p = x$. Comme $f$ est affine sur $C_k$, $f(y_1) + \ldots + f(y_p) = f(x_1) + \ldots + f(x_n)$. Donc

$$
f(x) = \sup (f(y_1) + \ldots + f(y_p))
$$

où $(y_1, y_2, \ldots, y_p)$ parcourt l’ensemble des suites de p points de C telles que $y_1 + y_2 + \ldots + y_p = x$. Posons $D = C \cap (x - C)$. Comme D est compact (Esp. vect. top., chap. II, 2e éd., § 6, n° 8, cor. 2 de la prop. 11), il en est de même de l’ensemble des éléments $(y_1, \ldots, y_p)$ de $D^p$ tels que $y_1 + \ldots + y_p = x$, de sorte que la borne supérieure (19) est atteinte.

#### Lemme 6 {#int-iv-s7-lem-6 .statement}

On conserve les hypothèses et les notations du lemme 5, et on suppose les $f_\lambda$ positives. La fonction $\bar{f}$ est positivement homogène, concave et semi-continue supérieurement dans C. Elle est affine si C est réticulé.

Il est clair que $\bar{f}$ est positivement homogène. Soient $x, y$ dans $\mathbf{C}$. Si $x_1, \ldots, x_m, y_1, \ldots, y_n$ dans $\mathbf{C}$ sont tels que $x_1 + \ldots + x_m = x$, $y_1 + \ldots + y_n = y$, on a $x_1 + \ldots + x_m + y_1 + \ldots y_n = x + y$, donc

$$
f(x_1) + \ldots + f(x_m) + f(y_1) + \ldots + f(y_n) \leq \bar{f}(x + y);
$$

on en déduit que $\bar{f}(x) + \bar{f}(y) \leq \bar{f}(x + y)$, donc $\bar{f}$ est concave. Soit $L$ (resp. $L_\lambda$) l’ensemble des $(t, x) \in \mathbf{R} \times E$ tels que $x \in \mathbf{C}$ et $0 \leq t \leq \bar{f}(x)$ (resp. $0 \leq t \leq f_\lambda(x)$). Chacun des $L_\lambda$ est fermé dans le cône convexe saillant faiblement complet $\mathbf{R}_+ \times \mathbf{C}$, donc la somme $\sum_{\lambda \in \Lambda} L_\lambda$ est fermée (\emph{Esp. vect. top.}, chap. II, 2e éd., § 6, n° 8, cor. 2 de la prop. 11). D’après le lemme 5, cette somme est égale à $L$. Donc $L$ est fermé, ce qui prouve que $\bar{f}$ est semi-continue supérieurement. Enfin, supposons $\mathbf{C}$ réticulé, et prouvons que $\bar{f}$ est convexe. Soient $x, y$ dans $\mathbf{C}$ et $\varepsilon > 0$. Il existe $z_1, z_2, \ldots, z_n$ dans $\mathbf{C}$ tels que $f(z_1) + \ldots + f(z_n) \geq \bar{f}(x + y) - \varepsilon$ et $z_1 + \ldots + z_n = x + y$. L’espace vectoriel $\mathbf{C} - \mathbf{C}$ est réticulé pour l’ordre induit par celui de $E$ (\emph{Alg.}, chap. VI, 2e éd., § 1, n° 9, prop. 8). D’après le théorème de décomposition (\emph{loc. cit.}, n° 10, th. 1), il existe $x_1, \ldots, x_n, y_1, \ldots, y_n$ dans $\mathbf{C}$ tels que $x_1 + y_1 = z_1, \ldots, x_n + y_n = z_n, x_1 + \ldots + x_n = x, y_1 + \ldots + y_n = y$. Alors, comme $f$ est positivement homogène et convexe, on a

$$
\begin{align*}
\bar{f}(x + y) &\leq \varepsilon + f(z_1) + \ldots + f(z_n) \\
&\leq \varepsilon + f(x_1) + f(y_1) + \ldots + f(x_n) + f(y_n) \\
&\leq \varepsilon + \bar{f}(x) + \bar{f}(y).
\end{align*}
$$

Comme $\varepsilon$ est arbitraire $> 0$, on a bien prouvé que $\bar{f}$ est convexe.

**Théorème 3** (Choquet).—*Soient* $E$ *un espace localement convexe faible séparé*, $C$ *un cône convexe saillant faiblement complet de sommet* 0 *dans* $E$, $G$ *la réunion des génératrices extrémales de* $C$, $K$ *une partie compacte convexe de* $C$, $\lambda$ *et* $\lambda'$ *des mesures positives de masse* 1 *sur* $K$, *admettant le même barycentre*, *et telles que* $\lambda^*(K - (K \cap G)) = {\lambda'}^*(K - (K \cap G)) = 0$. *Supposons* $\mathbf{C}$ *réticulé*. *Alors, pour toute fonction* $f$ *convexe* $\geq 0$ *semi-continue inférieurement et positivement homogène sur* $C$, *on a* $\lambda^*(f|K) = {\lambda'}^*(f|K)$.

Soit $\mathcal{A}$ (resp. $\mathcal{A}'$) l’ensemble des restrictions à $C$ des formes linéaires (resp. des fonctions affines) continues sur $E$. On sait (\emph{Esp. vect. top.}, chap. II, 2e éd., § 5, n° 4, *Remarque* 2) que $f$ est l’enveloppe supérieure de l’ensemble des éléments de $\mathcal{A}$ majorés par $f$. L’ensemble des fonctions de la forme $\sup(f_1, \ldots, f_p)$ où $f_1, \ldots, f_p$ appartiennent à $\mathcal{A}$, $f_1 \geq 0, \ldots, f_p \geq 0$, est filtrant croissant et admet $f$ pour enveloppe supérieure. Compte tenu du § 1, n° 1, th. 1, il suffit de vérifier l’égalité $\lambda(f|K) = \lambda'(f|K)$ lorsque $f$ est de la forme précédente.

Définissons $\bar{f}$ comme dans le lemme 5. Il est clair que $\bar{f}(y) = f(y)$ si $y \in G$. Comme $\lambda^*(K - (K \cap G)) = 0$, on a $\lambda(f|K) = \lambda(\bar{f}|K)$. D’après le lemme 6, $\bar{f}$ est affine et semi-continue supérieurement. Donc $\bar{f}|K$ est enveloppe inférieure d’un ensemble filtrant décroissant de restrictions d’éléments de $\mathcal{A}'$ à K (Esp. vect. top., chap. II, 2e éd., § 5, n° 4, prop. 6). Soit $x \in K$ le barycentre de $\lambda$. Si $g \in \mathcal{A}$, on a $\lambda(g|K) = g(x)$. Donc $\lambda(\bar{f}|K) = \bar{f}(x)$ ($§ 4$, n° 4, cor. 2 de la prop. 5). Ainsi, $\lambda(f|K) = \bar{f}(x)$, et on voit de même que $\lambda'(f|K) = \bar{f}(x)$.

#### Corollaire {#int-iv-s7-n6-cor-1 .statement}

Soient E un espace localement convexe séparé, C un cône convexe saillant de sommet 0 dans E, admettant une semelle compacte M, et G la réunion des génératrices extrémales de C. Soit $x \in M$. Si C est réticulé, il existe au plus une mesure positive $\lambda$ de masse 1 sur M, telle que $\lambda^*(M - (G \cap M)) = 0$, et admettant x pour barycentre.

En remplaçant la topologie de E par la topologie affaiblie, (ce qui ne change pas la topologie de M), on peut supposer E faible. Soient $\lambda$ et $\lambda'$ deux mesures sur M possédant les propriétés de l’énoncé, h une forme linéaire continue sur E telle que M soit l’intersection de C et de l’hyperplan d’équation $h(x) = 1$. Soit $\mathscr{S}$ le sous-ensemble de $\mathscr{C}(M)$ constitué par les restrictions à M des fonctions convexes $\geq 0$ positivement homogènes et continues dans C. Le cône C est faiblement complet (Esp. vect. top., chap. II, 2e éd., § 7, n° 3). D’après le th. 3, on a $\lambda(f) = \lambda'(f)$ pour toute $f \in \mathscr{S}$.

Si $f_1, f_2, f_3, f_4$ appartiennent à $\mathscr{S}$, on a
$$
\sup(f_1 - f_2, f_3 - f_4) = \sup(f_1 + f_4, f_3 + f_2) - (f_2 + f_4) \in \mathscr{S} - \mathscr{S}
$$
$$
\inf(f_1 - f_2, f_3 - f_4) = -\sup(f_2 - f_1, f_4 - f_3) \in \mathscr{S} - \mathscr{S}.
$$
Puisque $h|M \in \mathscr{S}$, $\mathscr{S} - \mathscr{S}$ contient les fonctions constantes. Si x et y sont deux points distincts de M, il existe une forme linéaire continue sur E qui sépare x et y, et cette forme est différence de deux formes linéaires continues positives sur C (Esp. vect. top., chap. II, 2e éd., § 6, n° 8, lemme 1). Il résulte de ce qui précède que, pour $\alpha, \beta$ réels, il existe $f \in \mathscr{S} - \mathscr{S}$ tel que $f(x) = \alpha, f(y) = \beta$.

Alors $\mathcal{S} - \mathcal{S}$ est partout dense dans $\mathcal{C}(M)$ pour la topologie de la convergence uniforme (*Top. gén.*, chap. X, 2\textsuperscript{e} éd., § 4, n\textsuperscript{o} 1, cor. de la prop. 2). Comme $\lambda$ et $\lambda'$ coïncident sur $\mathcal{S} - \mathcal{S}$, on a $\lambda = \lambda'$.

EXERCICES

## EXERCICES {#int-iv-s7-exercises}

See the [exercises for § 7](exercises/s7/).
