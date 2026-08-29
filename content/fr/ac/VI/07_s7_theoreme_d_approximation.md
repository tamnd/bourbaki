---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 7
section_title: Théorème d’approximation
lang: fr
source: ac-v-vii-fr
pdf_pages: 0128-0133, 0182-0183
extraction: ocr
subsections:
    - "no": 1
      title: Intersection d’un nombre fini d’anneaux de valuation
      page: 0
      pdf_page: 128
    - "no": 2
      title: Valuations indépendantes
      page: 0
      pdf_page: 130
    - "no": 3
      title: Cas des valeurs absolues
      page: 0
      pdf_page: 132
statements: 16
exercises: 3
content_sha256: cb90577db0ff77f03331b1d5585e9d0206d7ffc4505843b13154172f4befc9f4
---

## § 7. Théorème d’approximation.

### 1. Intersection d’un nombre fini d’anneaux de valuation

#### Proposition 1 {#ac-vi-s7-prop-1 .statement}

Soient $K$ un corps, $(\mathbf{A}_i)_{1 \leq i \leq n}$ une famille finie d’anneaux de valuation pour $K$, et $B = \bigcap_{i=1}^n \mathbf{A}_i$. Posons $\mathfrak{p}_i = B \cap m(\mathbf{A}_i)$. Alors $\mathbf{A}_i = B_{\mathfrak{p}_i}$ pour tout $i$, et le corps des fractions de $B$ est $K$.

Il est clair que $B_{p_i} \subset A_i$. Pour prouver l’inclusion opposée, nous aurons besoin du lemme suivant :

#### Lemme 1 {#ac-vi-s7-lem-1 .statement}

*Soient $v_i$ ($1 \leq i \leq n$) des valuations d’un corps $K$, et $x \in K^*$. Il existe alors un polynôme $f(X)$ de la forme*

$$
f(X) = 1 + n_1 X + \cdots + n_{k-1} X^{k-1} + X^k
$$
$$(k \geq 2,\ n_j \in \mathbf{Z}\ \text{pour}\ 1 \leq j \leq k-1)$$

*tel que $f(x) \neq 0$ et que l’élément $z = f(x)^{-1}$ jouisse des propriétés suivantes pour $1 \leq i \leq n$:*

$$
\begin{array}{ll}
v_i(z) = 0 & \text{si}\ v_i(x) \geq 0 \\
v_i(z) + v_i(x) > 0 & \text{si}\ v_i(x) < 0.
\end{array}
$$

Admettons pour un moment ce lemme, et montrons comment il entraîne que $A_1 \subset B_{p_1}$. Soit $x$ un élément non nul de $A_1$. Appliquons le lemme à $x$ et à des valuations $v_i$ associées aux $A_i$. On a $v_i(z) \geq 0$ et $v_i(zx) \geq 0$ pour tout $i$, donc $z \in B$ et $zx \in B$. Comme $v_1(x) \geq 0$, on a $v_1(z) = 0$, donc $z \notin p_1$. Donc $x = xz/z \in B_{p_1}$. Le corps des fractions de $B$ contient alors $A_1$, et est donc $K$.

Passons à la démonstration du lemme. Soit $I$ l’ensemble des indices $i$ tels que $v_i(x) \geq 0$. Pour $i \in I$, soit $A_i$ l’anneau de la valuation $v_i$, et notons $\bar{x}_i$ l’image canonique de $x$ dans $\kappa(A_i)$. Pour tout $i \in I$, construisons un polynôme $f_i$ de la façon suivante : s’il existe un polynôme $g(X)$ de la forme (1) tel que $g(\bar{x}_i) = 0$ dans $\kappa(A_i)$, nous prendrons pour $f_i$ un tel polynôme ; sinon nous prendrons $f_i = 1$. Posons alors $f(X) = 1 + X^2 \prod_{i \in I} f_i(X)$. C’est évidemment un polynôme de la forme (1). Si $i \in I$, on a $f(x) \in A_i$, et aussi $f(\bar{x}_i) \neq 0$ par construction ; donc $f(x) \notin m(A_i)$, $v_i(f(x)) = 0$ et $v_i(z) = 0$. Si $i \notin I$, on a $v_i(x) < 0$, d’où $v_i(f(x)) = kv_i(x)$ (§ 3, no 1, prop. 1), et $v_i(x) + v_i(z) = (1 - k)v_i(x) > 0$ (puisque $k \geq 2$). D’où le lemme.

#### Proposition 2 {#ac-vi-s7-prop-2 .statement}

*Les hypothèses étant celles de la prop. 1, supposons de plus que $A_i \not\subset A_j$ pour $i \neq j$. Alors les $p_i$ sont des idéaux maximaux de $B$ deux à deux distincts, et tout idéal maximal de $B$ est égal à un des $p_i$.

Si on avait $p_i \subset p_j$ pour $i \neq j$, on aurait $A_i = B_{p_i} \supset B_{p_j} = A_j$. Il suffit alors d’appliquer le Chap. II, § 3, no 5, cor. de la prop. 17.

#### Corollaire 1 {#ac-vi-s7-prop-2-cor-1 .statement}

*Supposons que $A_i \not\subset A_j$ pour $i \neq j$. Pour toute famille d’éléments $a_i \in A_i \ (1 \leq i \leq n)$, il existe $x \in B$ tel que $x \equiv a_i \ (\mathrm{mod.}\ m(A_i))$ pour $1 \leq i \leq n$.*

#### Corollaire 2 {#ac-vi-s7-prop-2-cor-2 .statement}

Supposons que $A_i \subsetneq A_j$ pour $i \neq j$. Il existe des éléments $x_i$ ($1 \leq i \leq n$) de $K$ tels que $v_i(x_i) = 0$ et $v_j(x_i) > 0$ pour $i \neq j$.
Pour chaque indice $i$, on applique le cor. 1 à la famille $(a_j)$ telle que $a_i = 1$ et $a_j = 0$ pour $j \neq i$.

#### Corollaire 3 {#ac-vi-s7-prop-2-cor-3 .statement}

Tout anneau de valuation pour $K$ contenant $B$ contient l’un des $A_i$.
On peut se borner au cas où $A_i \subsetneq A_j$ pour $i \neq j$. Soit $V$ un anneau de valuation pour $K$ contenant $B$. Posons
$$
\mathfrak{p} = m(V) \cap B.
$$
Il existe un idéal maximal $\mathfrak{p}_i$ de $B$ contenant $\mathfrak{p}$, d’où
$$
A_i = B_{\mathfrak{p}_i} \subset B_{\mathfrak{p}} \subset V.
$$

### 2. Valuations indépendantes

#### Définition 1 {#ac-vi-s7-def-1 .statement}

Soient $A$ et $A'$ deux anneaux de valuation pour un même corps $K$. On dit que $A$ et $A'$ sont indépendants si $K$ est l’anneau engendré par $A$ et $A'$. Deux valuations de $K$ sont dites indépendantes si leurs anneaux sont indépendants, dépendantes dans le cas contraire.

Une valuation impropre de $K$ est indépendante de toute valuation de $K$. Pour que deux valuations de hauteur 1 de $K$ soient indépendantes, il faut et il suffit qu’elles soient inéquivalentes ($§ 4, n° 5,$ prop. 6, c)).

#### Théorème 1 (Théorème d’approximation pour les valuations) {#ac-vi-s7-thm-1 .statement}

Soient $v_i$ ($1 \leq i \leq n$) des valuations deux à deux indépendantes d’un corps $K$, et $\Gamma_i$ le groupe des ordres de $v_i$. Soient $a_i \in K$ et $\alpha_i \in \Gamma_i$ ($1 \leq i \leq n$). Il existe alors $x \in K$ tel que $v_i(x - a_i) \geq \alpha_i$ pour tout $i$.
Si $v_i$ est impropre, on a $\alpha_i = 0$ et la relation $v_i(x - a_i) \geq \alpha_i$ est vraie pour tout $x \in K$. On peut donc supposer les $\nu_i$ non impropres.

Soient $A_i$ l’anneau de $\nu_i$, $B = \bigcap_{i=1}^n A_i$ et $\mathfrak{p}_i = m(A_i) \cap B$. D’après la prop. 1 du no 1, les $a_i$ peuvent s’écrire $a_i = b_i/s$ ($b_i \in B$, $s \in B - \{0\}$); si l’on pose $x = y/s$ et $\alpha'_i = \alpha_i + \nu_i(s)$, on devra avoir $\nu_i(y - b_i) \geq \alpha'_i$. Ceci montre qu’on peut supposer que $a_i \in B$ pour tout $i$; on peut aussi supposer que $\alpha_i > 0$ pour tout $i$. Soit $v_i$ l’ensemble des $z \in K$ tels que $\nu_i(z) \geq \alpha_i$; posons $q_i = v_i \cap B$. Pour $x \in B$, $\nu_i(x - a_i) \geq \alpha_i$ équivaut à $x \equiv a_i$ ($q_i$). Il s’agit donc de montrer que l’homomorphisme canonique $B \to \prod_{i=1}^n (B/q_i)$ est surjectif, c’est-à-dire qu’on a $q_i + q_j = B$ pour $i \neq j$ (Chap. II, § 1, no 2, prop. 5). Comme les idéaux maximaux de $B$ sont les $\mathfrak{p}_i$ (prop. 2), il suffira pour cela de montrer que l’on a $q_i \notin \mathfrak{p}_j$ pour $i \neq j$.

Supposons qu’il existe $i, j$ tels que l’on ait $q_i \subset \mathfrak{p}_j$ et $i \neq j$. Nous verrons dans un instant que la racine de $q_i$ est un idéal premier $\mathfrak{p}$ de $B$. On a alors $\mathfrak{p} \subset \mathfrak{p}_j$, et aussi $\mathfrak{p} \subset \mathfrak{p}_i$ puisque $\alpha_i > 0$, donc $q_i \subset \mathfrak{p}_i$. On a donc $A_j = B_{\mathfrak{p}_j} \subset B_{\mathfrak{p}}$ (no 1, prop. 1), et, de même, $A_i \subset B_{\mathfrak{p}}$. Or, comme $v_i \neq (0)$ et que $v_i = B_{\mathfrak{p}_i} q_i$ (chap. II, § 2, no 4, prop. 10), on a $q_i \neq (0)$, d’où $\mathfrak{p} \neq (0)$ et $B_{\mathfrak{p}} \neq K$. Ceci contredit l’hypothèse que $A_i$ et $A_j$ sont indépendants.

Reste à montrer que $\mathfrak{p}$ est premier. Or ceci résulte du lemme suivant :

#### Lemme 2 {#ac-vi-s7-lem-2 .statement}

Soient $A$ un anneau de valuation, et $\mathfrak{b}$ un idéal de $A$ distinct de $A$. Alors la racine $r$ de $\mathfrak{b}$ est un idéal premier.

Supposons qu’on ait $xy \in r$. Il existe alors $n \geq 1$ tel que $(xy)^n \in \mathfrak{b}$. Notons $\nu$ une valuation associée à $A$. Si, par exemple, on a $\nu(x) \geq \nu(y)$, on a $\nu(x^{2^n}) \geq \nu(x^n y^n)$, d’où $x^{2^n} \in \mathfrak{b}$ et $x \in r$.

#### Corollaire 1 {#ac-vi-s7-lem-2-cor-1 .statement}

Pour toute famille d’éléments $\gamma_i \in \Gamma_i (1 \leq i \leq n)$, il existe $x \in K$ tel que $\nu_i(x) = \gamma_i (1 \leq i \leq n)$.

On peut supposer $A_i \neq K$ pour tout $i$. Alors, il existe pour tout $i$ un $a_i \in K$ tel que $\nu_i(a_i) = \gamma_i$ et un $\alpha_i \in \Gamma_i$ tel que $\gamma_i < \alpha_i$. Appliquons le th. 1 à ces éléments $a_i$: il existe $x \in K$ tel que $\nu_i(x - a_i) > \nu_i(a_i)$; d’où, comme $x = a_i + (x - a_i)$, $\nu_i(x) = \nu_i(a_i) = \gamma_i$ ($§ 3$, no 1, prop. 1).

#### Corollaire 2 {#ac-vi-s7-lem-2-cor-2 .statement}

Soit $\mathcal{T}_i$ la topologie définie sur $K$ par $\nu_i$; munissons $K^n$ de la topologie produit des $\mathcal{T}_i$. Si les $\nu_i$ sont non impropres, la diagonale de $K^n$ est dense dans $K^n$.

#### Proposition 3 {#ac-vi-s7-prop-3 .statement}

Soient $\nu$ et $\nu'$ deux valuations non impropres d’un même corps K. Pour que $\nu$ et $\nu'$ définissent la même topologie sur K, il faut et il suffit qu’elles soient dépendantes.

Supposons les topologies $\mathcal{T}_\nu$ et $\mathcal{T}_{\nu'}$, définies par $\nu$ et $\nu'$, identiques. Puisque $\mathcal{T}_\nu$ est séparée, la diagonale de $K^2$ est fermée, donc $\nu$ et $\nu'$ sont dépendantes (cor. 2 du th. 1).

Inversement, supposons $\nu$ et $\nu'$ dépendantes. Alors leurs anneaux A et A' sont contenus dans un même anneau A'' distinct de K, et A'' est l’anneau d’une valuation $\nu''$ ($§ 4$, n° 1, prop. 1). Il suffit de montrer que la topologie $\mathcal{T}_{\nu''}$ est identique à $\mathcal{T}_\nu$. Soient $\Gamma$ et $\Gamma''$ les groupes des ordres de $\nu$ et $\nu''$. Il existe un homomorphisme croissant $\lambda$ de $\Gamma$ sur $\Gamma''$ tel que $\nu'' = \lambda \circ \nu$ ($§ 4$, n° 3). Si $\alpha'' \in \Gamma''$, soit $\alpha \in \lambda^{-1}(\alpha'')$; la condition $\nu(x) \geq \alpha$ entraîne $\nu''(x) \geq \alpha''$. Soient $\beta \in \Gamma$, et $\beta'' = \lambda(\beta)$; la condition $\nu(x) \leq \beta$ entraîne $\nu''(x) \leq \beta''$, donc la condition $\nu''(x) > \beta''$ entraîne $\nu(x) > \beta$. Comme $\nu$ et $\nu''$ sont non impropres, les inégalités envisagées définissent des systèmes fondamentaux de voisinages de 0 pour $\mathcal{T}_\nu$ et $\mathcal{T}_{\nu''}$. Donc $\mathcal{T}_\nu = \mathcal{T}_{\nu''}$, ce qui termine la démonstration.

#### Remarque 1 {#ac-vi-s7-n2-rem-1 .statement}

La prop. 3 montre que la relation « $\nu$ et $\nu'$ sont dépendantes » est une relation d’équivalence.

#### Remarque 2 {#ac-vi-s7-n2-rem-2 .statement}

Compte tenu des relations entre valuations de hauteur 1 et valeurs absolues ultramétriques ($§ 6$, n° 2), la prop. 3 résulte aussi, dans le cas des valuations de hauteur 1, de la caractérisation des valeurs absolues équivalentes (Top. gén., chap. IX, 2e éd., $§ 3$, n° 2, prop. 5).

#### Proposition 4 {#ac-vi-s7-prop-4 .statement}

Soient $\nu_1, \ldots, \nu_n (n \geq 2)$ des valuations deux à deux dépendantes d’un même corps K. Alors les anneaux $A_1, \ldots, A_n$ de $\nu_1, \ldots, \nu_n$ engendrent un sous-anneau de K distinct de K.

Pour $n = 2$, la prop. 4 résulte de la déf. 1. Supposons-la établie pour $n - 1$ valuations. Il existe alors un sous-anneau A de K distinct de K et contenant $A_1, \ldots, A_{n-1}$; il existe aussi un sous-anneau $B \neq K$ contenant $A_{n-1}$ et $A_n$. Comme A et B contiennent $A_{n-1}$, ils sont comparables pour l’inclusion ($§ 4$, n° 1, cor. de la prop. 1). Le plus grand des deux contient donc tous les $A_i$.

### 3. Cas des valeurs absolues

#### Théorème 2 (Théorème d’approximation pour les valeurs absolues) {#ac-vi-s7-thm-2 .statement}

Soient $f_i (1 \leq i \leq n)$ des valeurs absolues non impropres et deux à deux inéquivalentes sur un même corps K. Soient $a_i (1 \leq i \leq n)$ des éléments de K, et $\varepsilon$ un nombre réel $> 0$. Il existe alors $x \in K$ tel que $f_i(x - a_i) \leq \varepsilon$ pour tout $i$.

Notons $K_i$ le corps K muni de la topologie définie par $f_i$. Le résultat à démontrer équivaut au suivant : dans le produit $P = K_1 \times \cdots \times K_n$, l’adhérence $\overline{D}$ de la diagonale D est égale à P. Ceci est évident pour $n = 1$. Nous supposerons que ce point est établi dans le cas de $k$ valeurs absolues pour $k < n$.

Montrons d’abord qu’il existe, pour $2 \leq h \leq n$, un élément $x_h$ de K tel que $f_1(x_h) < 1$, $f_2(x_h) > 1$, et $f_i(x_h) \neq 1$ pour $3 \leq i \leq h$. Raisonnons par récurrence sur $h$. Si $h = 2$, ceci résulte du fait que $f_1$ et $f_2$ sont inéquivalentes. Supposons donc démontrée l’existence de $x_{h-1}$, et prouvons celle de $x_h$. Si $f_h(x_{h-1}) \neq 1$, on peut prendre $x_h = x_{h-1}$; si $f_h(x_{h-1}) = 1$, on choisit $z \in K^*$ tel que $f_h(z) \neq 1$, et $x_h = z(x_{h-1})^s$ répond à la question pour s assez grand. On a ainsi prouvé l’existence de $x_n$.

Quand l’entier $q$ tend vers l’infini, $f_1(x_n^q)$ tend vers 0, $f_2(x_n^q)$ tend vers $+\infty$, et $f_i(x_n^q)$ tend vers 0 ou $+\infty$ pour $i \geq 3$. Posant $y_q = x_n^q(1 + x_n^q)^{-1}$, on a $1 - y_q = (1 + x_n^q)^{-1}$; donc la suite $(y_q)$ tend vers 0 dans $K_1$, vers 1 dans $K_2$, et vers 0 ou 1 dans $K_i$ pour $i \geq 3$. En changeant la numérotation des $K_i$, on peut donc supposer qu’il existe un entier $r (1 \leq r < n)$ tel que $\overline{D}$ contienne le point $(e_1, \ldots, e_n)$ où $e_i = 1$ pour $1 \leq i \leq r$ et $e_i = 0$ pour $r + 1 \leq i \leq n$. Or, $\overline{D}$ est un sous-K-espace vectoriel de P. Donc $\overline{D}$ contient les diagonales $D'$ et $D''$ de $P' = K_1 \times \cdots \times K_r$ et $P'' = K_{r+1} \times \cdots \times K_n$. D’après l’hypothèse de récurrence, $P' = \overline{D}'$ et $P'' = \overline{D}''$. Donc $\overline{D} = P$. C.Q.F.D.

## EXERCICES {#ac-vi-s7-exercises}

See the [exercises for § 7](exercises/s7/).
