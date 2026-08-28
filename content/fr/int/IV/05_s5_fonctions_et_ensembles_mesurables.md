---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 5
section_title: Fonctions et ensembles mesurables
lang: fr
source: int-i-iv-fr
pdf_pages: 0173-0207, 0249-0258
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fonctions et ensembles mesurables
      page: 0
      pdf_page: 173
    - "no": 2
      title: Principe de localisation. Ensembles localement négligeables
      page: 0
      pdf_page: 175
    - "no": 3
      title: Propriétés élémentaires des fonctions mesurables
      page: 0
      pdf_page: 178
    - "no": 4
      title: Limites de fonctions mesurables
      page: 0
      pdf_page: 179
    - "no": 5
      title: Critères de mesurabilité
      page: 0
      pdf_page: 181
    - "no": 6
      title: Critères d’intégrabilité
      page: 0
      pdf_page: 188
    - "no": 7
      title: Mesure induite sur un sous-espace localement compact
      page: 0
      pdf_page: 190
    - "no": 8
      title: Familles $\mu$-denses d’ensembles compacts.
      page: 0
      pdf_page: 192
    - "no": 9
      title: Partitions localement dénombrables
      page: 0
      pdf_page: 194
    - "no": 10
      title: Fonctions mesurables définies dans une partie mesurable
      page: 0
      pdf_page: 195
    - "no": 11
      title: Convergence en mesure
      page: 0
      pdf_page: 198
    - "no": 12
      title: Une propriété de la convergence vague
      page: 0
      pdf_page: 204
statements: 76
exercises: 30
content_sha256: e0490ea743776a194803b2ddeaff4d8770f05d7bc1a191c652da232c512b3310
---

## § 5. Fonctions et ensembles mesurables

### 1. Définition des fonctions et ensembles mesurables

#### Définition 1 {#int-iv-s5-def-1 .statement}

Soient X un espace localement compact, $\mu$ une mesure sur X. On dit qu’une application f de X dans un espace topologique F est mesurable pour la mesure $\mu$ (ou encore $\mu$-mesurable) si, pour toute partie compacte K de X, il existe un ensemble $\mu$-négligeable N $\subset K$ et une partition de $K - N$ formée d’une suite (finie ou infinie) $(K_n)$ d’ensembles compacts, tels que la restriction de f à chacun des $K_n$ soit continue.

Il est clair que toute application continue de X dans F est mesurable.

On notera que si $\mu$ et $\nu$ sont deux mesures sur X telles que tout ensemble $\mu$-négligeable soit $\nu$-négligeable, alors toute fonction $\mu$-mesurable est aussi $\nu$-mesurable (cf. chap. V, § 5).

La déf. 1 se transforme en le critère suivant:

#### Proposition 1 {#int-iv-s5-prop-1 .statement}

Pour qu’une application f de X dans F soit mesurable, il faut et il suffit que, pour tout ensemble compact K $\subset X$ et tout nombre $\varepsilon > 0$, il existe un ensemble compact $K_1 \subset K$, tel que $|\mu|(K - K_1) \leq \varepsilon$, et que la restriction de f à $K_1$ soit continue.

En effet, si cette condition est remplie, on peut définir par récurrence une suite d’ensembles compacts $K_n \subset K$, deux à deux sans point commun, tels que $|\mu|\left(K - \left( \bigcup_{i=1}^n K_i \right)\right) \leq 1/n$, et que la restriction de f à chacun des $K_n$ soit continue; le complémentaire par rapport à K de la réunion des $K_n$ est alors négligeable (§ 4, n° 5, cor. de la prop. 7), donc f est mesurable. Inversement, supposons qu’il existe un ensemble négligeable N $\subset K$ et une partition $(K_n)$ de $K - N$ formée d’ensembles compacts tels que la restriction de f à chacun des $K_n$ soit continue; pour tout $\varepsilon > 0$, il existe un entier $n$ tel que, si $H = \bigcup_{i=1}^n K_i$, on ait $|\mu|(K - H) \leq \varepsilon$ (§ 4, n° 5, cor. de la prop. 7); l’ensemble $H$ est compact, les $K_i$ ($1 \leq i \leq n$) forment une partition finie de $H$ en ensembles compacts et la restriction de $f$ à chacun des $K_i$ est continue; donc la restriction de $f$ à $H$ est continue.

#### Proposition 2 {#int-iv-s5-prop-2 .statement}

*Soit* $(F_n)$ *une suite d’espaces topologiques, et pour chaque* $n$, *soit* $f_n$ *une application mesurable de* $X$ *dans* $F_n$. *Pour tout ensemble compact* $K \subset X$ *et tout* $\varepsilon > 0$, *il existe un ensemble compact* $K_0 \subset K$ *tel que* $|\mu|(K - K_0) \leq \varepsilon$, *et que la restriction à* $K_0$ *de chacune des fonctions* $f_n$ *soit continue*.

En effet, il existe pour chaque entier $n \geq 1$ un ensemble compact $K_n \subset K$ tel que $|\mu|(K - K_n) \leq \varepsilon/2^n$, et que la restriction de $f_n$ à $K_n$ soit continue. L’ensemble $K_0 = \bigcap_{n=1}^\infty K_n$ est compact, les restrictions à $K_0$ de toutes les fonctions $f_n$ sont continues, et comme $K - K_0$ est contenu dans la réunion des $K - K_n$, on a

$$
|\mu|(K - K_0) \leq \sum_{n=1}^\infty \frac{\varepsilon}{2^n} = \varepsilon.
$$

#### Définition 2 {#int-iv-s5-def-2 .statement}

*On dit qu’une partie* $A$ *de* $X$ *est mesurable si sa fonction caractéristique* $\varphi_A$ *est mesurable*.

En vertu de la déf. 1, il revient au même de dire qu’un ensemble mesurable $A$ est un ensemble tel que, pour tout ensemble compact $K$, il existe un ensemble négligeable $N \subset K$ et une partition $(K_n)$ de $K - N$ formée d’une suite d’ensembles compacts, dont chacun est contenu dans $K \cap A$ ou dans $K \cap \complement A$.

Cette définition donne aussitôt le critère suivant:

#### Proposition 3 {#int-iv-s5-prop-3 .statement}

*Pour qu’un ensemble* $A$ *soit mesurable, il faut et il suffit que, pour tout ensemble compact* $K$, $A \cap K$ *soit intégrable*.

La condition est nécessaire parce que la réunion d’une suite d’ensembles intégrables $A_n$ est intégrable lorsque $\sum_n |\mu|(A_n)$ est finie (§ 4, n° 5, cor. de la prop. 8). La condition est suffisante parce que, pour tout ensemble intégrable $B$, il existe un ensemble négligeable $N \subset B$ et une partition de $B - N$ en une suite d’ensembles compacts ($§ 4$, n° 6, cor. 2 du th. 4).

#### Corollaire 1 {#int-iv-s5-prop-3-cor-1 .statement}

Les ensembles ouverts et les ensembles fermés sont mesurables.

En particulier l’espace $X$ tout entier est mesurable.

#### Corollaire 2 {#int-iv-s5-prop-3-cor-2 .statement}

Si $X$ est métrisable, tout sous-ensemble souslinien $A$ de $X$ (Top. gén., chap. IX, 2e éd., § 6, n° 2) est $\mu$-mesurable pour toute mesure $\mu$ sur $X$.

En vertu de la prop. 3, il suffit de vérifier que tout ensemble souslinien relativement compact $A$ est $\mu$-intégrable. Or, $A$ est alors capacitable pour $|\mu|^*$ (Top. gén., chap. IX, 2e éd., § 6, n° 9, th. 5). Donc, pour tout $\varepsilon > 0$, il existe une partie compacte $K$ de $A$ telle que $|\mu|^*(A) \leq |\mu|^*(K) + \varepsilon = |\mu|(K) + \varepsilon$. Soit $U$ une partie ouverte relativement compacte de $X$ contenant $A$ et telle que

$$
|\mu|(U) = |\mu|^*(U) \leq |\mu|^*(A) + \varepsilon.
$$

Alors $|\mu|^*(U - K) = |\mu|(U) - |\mu|(K) \leq 2\varepsilon$, donc $|\mu|^*(A - K) \leq 2\varepsilon$, ce qui prouve que $A$ est $\mu$-intégrable ($§ 4$, n° 6, cor. 1 du th. 4).

### 2. Principe de localisation. Ensembles localement négligeables

#### Proposition 4 (principe de localisation) {#int-iv-s5-prop-4 .statement}

Soit $f$ une application de $X$ dans un espace topologique $F$. On suppose que pour tout $x \in X$, il existe un voisinage intégrable $V_x$ de $x$, et une application mesurable $g_x$ de $X$ dans $F$ telle que $f(y) = g_x(y)$ presque partout dans $V_x$. Alors $f$ est mesurable.

En effet, soit $K$ un ensemble compact ; il existe un nombre fini de points $x_i \in K$ tels que les $V_{x_i}$ forment un recouvrement de $K$. On en conclut aussitôt ($§ 4$, n° 9, lemme 1) qu’il existe un ensemble négligeable $N \subset K$ et une partition finie de $K - N$ formée d’ensembles intégrables $M_j$, tels que chacun des ensembles $K \cap V_{x_i}$ soit réunion d’une partie de $N$ et d’un certain nombre des $M_j$, et que, dans chacun des $M_j$, $f$ soit égale à une des fonctions $g_{x_i}$. Or, pour chaque $M_j$, il existe un ensemble négligeable $N_j \subset M_j$ et une partition de $M_j - N_j$ formée d’une suite d’ensembles compacts $K_{nj}$ ($n \in \mathbf{N}$) ; d’autre part, pour chaque $K_{nj}$, il existe un ensemble négligeable $P_{nj} \subset K_{nj}$, et une partition de $K_{nj} - P_{nj}$ formée d’une suite d’ensembles compacts $K_{mnj}$ ($m \in \mathbf{N}$) telle que la restriction de $f$ à chacun des $K_{mnj}$ soit continue. Comme la réunion de $N$, des $N_j$ et des $P_{nj}$ est négligeable, $f$ est mesurable.

La notion de fonction mesurable est donc une notion de caractère local.

#### Définition 3 {#int-iv-s5-def-3 .statement}

On dit qu’un ensemble $A \subset X$ est localement négligeable (pour la mesure $\mu$) si, pour tout $x \in X$, il existe un voisinage $V$ de $x$ tel que $V \cap A$ soit négligeable.

En vertu du principe de localisation, tout ensemble localement négligeable est mesurable. Les propriétés des ensembles négligeables (§ 2) montrent que toute partie d'un ensemble localement négligeable est localement négligeable, et que toute réunion dénombrable d'ensembles localement négligeables est localement négligeable.

#### Proposition 5 {#int-iv-s5-prop-5 .statement}

Pour qu'un ensemble $A$ soit localement négligeable, il faut et il suffit que, pour tout ensemble compact $K$, $A \cap K$ soit négligeable.

La condition est évidemment suffisante puisque tout point de $X$ a un voisinage compact. Elle est nécessaire, car si, pour tout $x \in K$, il existe un voisinage $V_x$ de $x$ tel que $A \cap V_x$ soit négligeable, alors il existe un nombre fini de points $x_i \in K$ tels que les $V_{x_i}$ forment un recouvrement de $K$, et $A \cap K$ est contenu dans la réunion des ensembles négligeables $A \cap V_{x_i}$.

#### Corollaire 1 {#int-iv-s5-prop-5-cor-1 .statement}

Pour qu'un ensemble $A$ soit négligeable, il faut et il suffit qu'il soit localement négligeable et de mesure extérieure finie.

La condition est évidemment nécessaire. Inversement, si elle est vérifiée, $A$ est contenu dans un ensemble ouvert intégrable $G$, réunion d'un ensemble négligeable $N$ et d'une suite $(K_n)$ d'ensembles compacts (§ 4, n° 6, cor. 2 du th. 4); comme $A \cap N$ et les ensembles $A \cap K_n$ sont négligeables, il en est de même de leur réunion $A$.

#### Corollaire 2 {#int-iv-s5-prop-5-cor-2 .statement}

Tout ensemble ouvert localement négligeable est négligeable (et par suite contenu dans le complémentaire du support de $\mu$).

En effet, la mesure extérieure d’un ensemble ouvert G est la borne supérieure des mesures $|\mu|(K)$ des ensembles compacts $K \subset G$ (§ 4, n° 6, cor. 4 du th. 4); si G est localement négligeable, on a $|\mu|(K) = 0$ pour tout ensemble compact K contenu dans G, donc $|\mu|^*(G) = 0$.

#### Corollaire 3 {#int-iv-s5-prop-5-cor-3 .statement}

Dans un espace localement compact X dénombrable à l’infini, tout ensemble localement négligeable est négligeable.

En effet, X étant réunion d’une suite $(K_n)$ d’ensembles compacts, tout ensemble localement négligeable A est réunion des ensembles négligeables $A \cap K_n$, donc est négligeable.

On peut donner des exemples d’espaces localement compacts non dénombrables à l’infini, et de mesures sur un tel espace X, tels qu’il existe dans X des ensembles localement négligeables et non négligeables (§ 1, exerc. 5).

#### Corollaire 4 {#int-iv-s5-prop-5-cor-4 .statement}

Soit f une application de X dans un espace topologique F. Si l’ensemble N des points de discontinuité de f est localement négligeable, f est mesurable.

En effet, pour tout ensemble compact $K \subset X$, $K \cap N$ est négligeable (prop. 5), donc, pour tout $\varepsilon > 0$, il existe un ensemble compact $K_1 \subset K - (K \cap N)$ tel que $|\mu|(K - K_1) \leq \varepsilon$ (§ 4, n° 6, th. 4), et par hypothèse la restriction de f à $K_1$ est continue, d’où la conclusion.

Si $P\{x\}$ est une propriété, la propriété « $P\{x\}$ localement presque partout (par rapport à $\mu$) » est par définition équivalente à la propriété « l’ensemble des x tels que $(x \in X$ et non $P\{x\})$ est localement négligeable (pour la mesure $\mu$) ». Si F est un ensemble quelconque, la relation « $f(x) = g(x)$ localement presque partout » est une relation d’équivalence dans l’ensemble des applications de X dans F. En particulier, si F est un espace vectoriel, une application $f$ de X dans F telle que $f(x) = 0$ localement presque partout est dite localement négligeable. Nous-laissons au lecteur le soin d’établir pour ces notions la plupart des propriétés correspondant à celles qui ont été énumérées au § 2, n°s 4, 5 et 6 pour les fonctions égales presque partout. Nous nous bornerons à remarquer que si deux applications continues $f, g$ de X dans un espace topologique séparé F sont égales localement presque partout, elles sont égales presque partout en vertu du cor. 2 de la prop. 5 (et par suite égales en tout point du support de $\mu$ ($§ 2, n^o\ 4,$ prop. 9)); d’autre part, nous expliciterons la proposition suivante, conséquence immédiate du principe de localisation:

#### Proposition 6 {#int-iv-s5-prop-6 .statement}

*Soit f une application mesurable de X dans un espace topologique F. Toute application de X dans F, égale à f localement presque partout, est mesurable.*

### 3. Propriétés élémentaires des fonctions mesurables

#### Théorème 1 {#int-iv-s5-thm-1 .statement}

*Soient X un espace localement compact, $\mu$ une mesure sur X, $(F_n)$ une suite d’espaces topologiques, $F = \prod_n F_n$ leur produit. Pour chaque indice n, soit $f_n$ une application mesurable de X dans $F_n$, et soit $f(x) = (f_n(x)) \in F$; pour toute application continue u de $f(X)$ dans un espace topologique G, la fonction $x \to u(f(x))$ est mesurable.

En effet, pour toute partie compacte K de X et tout nombre $\varepsilon > 0$, il existe un ensemble compact $K_1 \subset K$ tel que
$$
|\mu|(K - K_1) \leq \varepsilon,
$$
et que les restrictions à $K_1$ de toutes les fonctions $f_n$ soient continues (n° 1, prop. 2); il est clair que $u \circ f$ est continue dans $K_1$, d’où le théorème.

#### Remarque 1 {#int-iv-s5-n3-rem-1 .statement}

Le théorème ne s’étend pas à un produit quelconque d’espaces topologiques (exerc. 1).
2) Si f est une application continue de X dans lui-même, g une application mesurable de X dans F, $g \circ f$ n’est pas nécessairement mesurable (exerc. 2).

#### Corollaire 1 {#int-iv-s5-thm-1-cor-1 .statement}

*L’enveloppe supérieure et l’enveloppe inférieure d’un nombre fini de fonctions numériques mesurables (finies ou non) est mesurable.

En effet, $\sup(u, v)$ et $\inf(u, v)$ sont continues dans $\bar{\mathbf{R}} \times \bar{\mathbf{R}}$.

#### Corollaire 2 {#int-iv-s5-thm-1-cor-2 .statement}

*Pour qu’une fonction numérique (finie ou non) soit mesurable, il faut et il suffit que $f^+$ et $f^-$ le soient.

La condition est nécessaire d’après le cor. 1; elle est suffisante parce que l’image A de X par l’application $x \mapsto (f^+(x), f^-(x))$ dans $\bar{\mathbf{R}} \times \bar{\mathbf{R}}$ ne contient pas les points $(+\infty, +\infty)$ et $(-\infty, -\infty)$; par suite, l’application $(u, v) \mapsto u - v$ est continue dans A.*

#### Corollaire 3 {#int-iv-s5-thm-1-cor-3 .statement}

Si $f$ et $g$ sont deux applications mesurables de $X$ dans un espace vectoriel topologique $F$, $f + g$ et $\alpha f$ sont mesurables ($\alpha$ scalaire quelconque).

L’ensemble des applications mesurables de $X$ dans un espace vectoriel topologique $F$ est donc un espace vectoriel.

#### Corollaire 4 {#int-iv-s5-thm-1-cor-4 .statement}

Soit $F$ un espace vectoriel de dimension $n$ sur $\mathbf{R}$, et soit $(e_k)_{1 \leq k \leq n}$ une base de $F$. Pour qu’une fonction $f = \sum_{k=1}^n e_k f_k$ soit mesurable, il faut et il suffit que chacune des fonctions numériques $f_k$ soit mesurable.

#### Corollaire 5 {#int-iv-s5-thm-1-cor-5 .statement}

Soient $F$, $G$, $H$ trois espaces vectoriels topologiques et soit $(u, v) \mapsto [u . v]$ une application bilinéaire continue de $F \times G$ dans $H$. Si $f$ est une application mesurable de $X$ dans $F$, $g$ une application mesurable de $X$ dans $G$, $[f . g]$ est une application mesurable de $X$ dans $H$.

En particulier, si $f$ est une application mesurable de $X$ dans un espace normé $F$ réel (resp. complexe) et $g$ une application mesurable de $X$ dans $\mathbf{R}$ (resp. $\mathbf{C}$), $gf$ est mesurable. Si $F$ est une algèbre normée, $f$ et $g$ deux applications mesurables de $X$ dans $F$, $fg$ est mesurable.

#### Corollaire 6 {#int-iv-s5-thm-1-cor-6 .statement}

Si $f$ est une application mesurable de $X$ dans un espace normé $F$, la fonction numérique $|f|$ est mesurable.

### 4. Limites de fonctions mesurables

#### Théorème 2 (Egoroff) {#int-iv-s5-thm-2 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$, $A$ un ensemble dénombrable, $\mathfrak{F}$ un filtre sur $A$ ayant une base dénombrable, $(f_\alpha)_{\alpha \in A}$ une famille d’applications mesurables de $X$ dans un espace métrisable $F$. On suppose que $\lim_{\mathfrak{F}} f_\alpha(x) = f(x)$ existe dans le complémentaire d’une partie localement négligeable $N$ de $X$. Dans ces conditions :
1° la fonction $f$ (prolongée de façon arbitraire dans $N$) est mesurable ;
2° pour toute partie compacte $K$ de $X$ et tout $\varepsilon > 0$, il existe un ensemble compact $K_1 \subset K$ tel que $|\mu|(K - K_1) \leq \varepsilon$, et tel que les restrictions des $f_\alpha$ à $K_1$ soient continues et convergent uniformément vers $f$ dans $K_1$.

La première assertion résulte évidemment de la seconde, que nous allons démontrer. Il existe un ensemble compact $K_0 \subset K$ tel que $|\mu|(K - K_0) \leq \varepsilon/2$, et que les restrictions à $K_0$ de toutes les fonctions $f_\alpha$ soient continues (n° 1, prop. 2). Soit $(A_n)$ une base dénombrable décroissante du filtre $\mathcal{F}$; soit $d$ une distance sur $F$ compatible avec la topologie. Pour tout couple d’entiers $n > 0$, $r > 0$, soit $B_{n,r}$ l’ensemble des points $x \in K_0$ tels que, pour au moins un couple d’indices $\alpha, \beta$ appartenant à $A_n$, on ait $d(f_\alpha(x), f_\beta(x)) \geq 1/r$; pour $\alpha$ et $\beta$ fixés, l’ensemble des $x \in K_0$ tels que $d(f_\alpha(x), f_\beta(x)) \geq 1/r$ est fermé dans $K_0$, donc compact; par suite, $B_{n,r}$ est réunion dénombrable d’ensembles compacts contenus dans $K_0$, donc est intégrable ($§ 4$, n° 5, prop. 6 et 8). Si l’on fixe $r$, l’intersection de la suite décroissante des ensembles $B_{n,r}$ ($n = 1, 2, \ldots$) est de mesure nulle, puisque $f_\alpha(x)$ tend presque partout vers $f(x)$ dans $K_0$ suivant le filtre $\mathcal{F}$; on a donc $\lim_{n \to \infty} |\mu|(B_{n,r}) = 0$ ($§ 4$, n° 5, cor. de la prop. 7), et il existe par suite un entier $n_r$ tel que $|\mu|(B_{n_r,r}) \leq \varepsilon/2^{r+2}$. Soit $B$ la réunion (pour $r = 1, 2, \ldots$) des ensembles $B_{n_r,r}$; $B$ est intégrable, et on a
$$
|\mu|(B) \leq \sum_{r=1}^\infty |\mu|(B_{n_r,r}) \leq \varepsilon/4
$$
($§ 4$, n° 5, cor. de la prop. 8). Soit $C$ le complémentaire de $B$ dans $K_0$; par construction, $f_\alpha(x)$ converge uniformément vers $f(x)$ dans $C$ suivant le filtre $\mathcal{F}$, et comme les restrictions des $f_\alpha$ à $C$ sont continues, il en est de même de la restriction de $f$ à $C$. Il suffit alors de prendre un ensemble compact $K_1 \subset C$ tel que $|\mu|(C - K_1) \leq \varepsilon/4$ pour satisfaire aux conditions de l’énoncé, puisque $|\mu|(K - K_1) = |\mu|(K - K_0) + |\mu|(B) + |\mu|(C - K_1) \leq \varepsilon$.

Les conclusions du th. 2 ne subsistent plus nécessairement si $F$ n’est pas métrisable (exerc. 1). Si $F$ est métrisable et si l’ensemble $A$ n’est pas dénombrable, mais si le filtre $\mathcal{F}$ possède une base dénombrable, la première conclusion du th. 2 est encore valable; en effet, si $(A_n)$ est une base dénombrable de $\mathcal{F}$, et $\alpha_n$ un élément de $A_n$, $f$ est limite localement presque partout de la suite $(f_{\alpha_n})$, donc est mesurable; mais la seconde conclusion du th. 2 n’est plus nécessairement valable (cf. exerc. 4).

#### Corollaire 1 {#int-iv-s5-thm-2-cor-1 .statement}

Soit $(f_n)$ une suite de fonctions numériques (finies ou non). Si les $f_n$ sont mesurables, les fonctions $\sup_n f_n$, $\inf_n f_n$, $\limsup_n f_n$, $\liminf_n f_n$, sont mesurables.

En effet, la droite achevée $\bar{\mathbf{R}}$, homéomorphe à un intervalle compact de $\mathbf{R}$, est métrisable. La fonction $\sup f_n$ est limite simple de la suite croissante des fonctions $g_n = \sup^n (f_1, f_2, \ldots, f_n)$, qui sont mesurables (n° 3, cor. 1 du th. 1); de même, $\lim_{n \to \infty} \sup f_n$ est limite simple de la suite décroissante des fonctions $h_n = \sup_{p \geq 0} f_{n+p}$, dont chacune est mesurable d’après ce qui précède. Enfin, comme $\inf f_n = -\sup(-f_n)$ et $\liminf f_n = -\limsup(-f_n)$, ces fonctions sont mesurables.

#### Corollaire 2 {#int-iv-s5-thm-2-cor-2 .statement}

Les ensembles mesurables dans X forment une tribu (Top. gén., chap. IX, 2e éd., § 6, n° 3).
En effet, si M et N sont mesurables,

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N
$$

et $\varphi_{M \cap N} = \varphi_M - \varphi_M \varphi_N$ sont mesurables en vertu du n° 3, th. 1. Si $(M_n)$ est une suite d’ensembles mesurables et M leur réunion, $\varphi_M = \sup_n \varphi_{M_n}$ est mesurable en vertu du cor. 1 du th. 2. D’où le corollaire.

En particulier, comme les ensembles ouverts sont mesurables :

#### Corollaire 3 {#int-iv-s5-thm-2-cor-3 .statement}

Les ensembles boréliens dans X (Top. gén., chap. IX, 2e éd., § 6, n° 3, déf. 4) sont $\mu$-mesurables pour toute mesure $\mu$ sur X.

### 5. Critères de mesurabilité

Lorsque F est un espace vectoriel topologique, toute fonction étagée sur les ensembles mesurables ($§ 4$, n° 9, déf. 4), à valeurs dans F, est évidemment mesurable (n° 3, cor. 3 du th. 1); une telle fonction $f$ ne prend qu’un nombre fini de valeurs, et pour tout $y \in F$, $\overline{f^{-1}}(y)$ est mesurable. Plus généralement, soient F un espace topologique quelconque, $f$ une application de X dans F ne prenant qu’un nombre fini de valeurs distinctes $a_i$ ($1 \leq i \leq m$); si les ensembles $A_i = \overline{f^{-1}}(a_i)$ sont mesurables, la fonction $f$ est mesurable. En effet, pour tout ensemble compact K, et pour chacun des ensembles $A_i \cap K$, il existe un ensemble négligeable $N_i \subset A_i \cap K$ et une partition de $A_i \cap K \cap \mathbf{C} N_i$ formée d’une suite $(K_{in})$ d’ensembles compacts ; comme K est la réunion des ensembles $A_i \cap K$, et que la restriction de $f$ à chacun des $K_{in}$ est constante, donc continue, $f$ est mesurable. Par abus de langage, nous dirons qu’une application $f$ de $X$ dans $F$ est une fonction étagée mesurable si elle ne prend qu’un nombre fini de valeurs et si, pour tout $y \in F$, $f^{-1}(y)$ est mesurable.

#### Théorème 3 {#int-iv-s5-thm-3 .statement}

*Pour qu’une application $f$ de $X$ dans un espace métrisable $F$ soit mesurable, il faut et il suffit que, pour tout ensemble compact $K \subset X$, il existe une suite $(g_n)$ de fonctions étagées mesurables, à valeurs dans $F$, telle que $g_n(x)$ tende vers $f(x)$ pour presque tout $x \in K$.*

La condition est suffisante, en raison du th. d’Egoroff et du principe de localisation. Montrons qu’elle est nécessaire : par hypothèse, il existe un ensemble négligeable $N \subset K$ et une partition $(K_m)$ de $K - N$ formée d’ensembles compacts tels que la restriction de $f$ à chacun des $K_m$ soit continue. Pour définir la suite $(g_n)$, il suffit de procéder de la façon suivante : soit $d$ une distance compatible avec la topologie de $F$; pour chaque $K_i$ d’indice $i \leq n$, il existe une partition finie de $K_i$ en ensembles intégrables assez petits $A_{ij}$ ($1 \leq j \leq q_i$) tels que l’oscillation de $f$ dans chacun des $A_{ij}$ soit $\leq 1/n$ (§ 4, n° 9, lemme 1); on prendra $g_n$ constante dans chacun des $A_{ij}$ et égale à une des valeurs de $f$ dans cet ensemble (pour $1 \leq i \leq n, 1 \leq j \leq q_i$), et égale à un élément fixe $a \in F$ pour tout point de $X$ n’appartenant à aucun des $A_{ij}$. Il est clair que la suite $(g_n(x))$ converge vers $f(x)$ en tout point de $K$ n’appartenant pas à $N$.

#### Corollaire 1 {#int-iv-s5-thm-3-cor-1 .statement}

*Soit $f$ une application mesurable de $X$ dans un espace de Banach $F$; pour tout ensemble compact $K \subset X$, il existe une suite $(g_n)$ de fonctions étagées mesurables, de support contenu dans $K$, telles que $|g_n(x)| \leq |f(x)|$ pour tout $x \in X$ et que $g_n(x)$ tende vers $f(x)$ pour presque tout $x \in K$.*

Avec les notations de la démonstration du th. 3, et en désignant par $a_{ij}$ une des valeurs de $f$ dans $A_{ij}$, il suffira de prendre pour valeur de $g_n$ dans $A_{ij}$, le point 0 si $|a_{ij}| \leq 1/n$, et le point $a_{ij}(1 - 1/(n|a_{ij}|))$ dans le cas contraire; enfin, on prendra $g_n(x) = 0$ dans le complémentaire de la réunion des $A_{ij} (1 \leq i \leq n, 1 \leq j \leq q_i)$.

#### Corollaire 2 {#int-iv-s5-thm-3-cor-2 .statement}

Soit X un espace localement compact dénombrable à l’infini. Si f est une application mesurable de X dans un espace métrisable F, il existe une suite $(g_n)$ de fonctions étagées mesurables, à valeurs dans F, telle que $g_n(x)$ tende vers $f(x)$ pour presque tout $x \in X$.

En effet, si X est réunion d’une suite croissante $(A_n)$ d’ensembles compacts, les ensembles $A_n - A_{n-1}$ non vides forment une partition de X en ensembles intégrables ; il existe par suite un ensemble négligeable $N \subset X$ et une partition de $\mathbf{C}N$ formée d’une suite $(K_n)$ d’ensembles compacts, tels que la restriction de $f$ à chacun des $K_n$ soit continue ; la démonstration du th. 3 peut alors se terminer sans modification.

#### Proposition 7 {#int-iv-s5-prop-7 .statement}

Soit f une application mesurable de X dans un espace topologique F ; l’image réciproque par f de tout ensemble fermé (resp. ouvert) dans F est mesurable.

Il suffit de faire la démonstration pour l’image réciproque $\bar{f}^{-1}(A)$ d’un ensemble A fermé dans F. Soit K une partie compacte de X ; il existe un ensemble négligeable $N \subset K$ et une partition $(K_n)$ de $K - N$ formée d’ensembles compacts tels que la restriction de $f$ à chacun des $K_n$ soit continue. L’intersection $K_n \cap \bar{f}^{-1}(A)$ est donc l’image réciproque de l’ensemble fermé A par la restriction de $f$ à $K_n$ ; c’est par suite un ensemble fermé dans $K_n$, donc compact. L’ensemble $K \cap \bar{f}^{-1}(A)$ est donc réunion de l’ensemble négligeable $N \cap \bar{f}^{-1}(A)$ et des ensembles compacts $K_n \cap \bar{f}^{-1}(A)$, ce qui prouve que $\bar{f}^{-1}(A)$ est mesurable.

#### Théorème 4 {#int-iv-s5-thm-4 .statement}

Soit F un espace métrisable, et soit d une distance sur F compatible avec la topologie. Pour qu’une application f de X dans F soit mesurable, il faut et il suffit qu’elle vérifie les deux conditions suivantes :

a) l’image réciproque par f de toute boule fermée de F est mesurable ;

b) pour tout ensemble compact $K \subset X$, il existe une partie dénombrable H de F, telle que $f(x) \in \bar{H}$ pour presque tout $x \in K$.

La condition a) est nécessaire en vertu de la prop. 7 ; d’autre part, avec les notations du th. 3, on satisfait à la condition b) en prenant pour H l’ensemble dénombrable formé des valeurs de toutes les fonctions $g_n$.

Montrons maintenant que les conditions a) et b) sont suffisantes. Soit K une partie compacte quelconque de X; il existe une partie négligeable N de K telle que $f(K - N)$ soit contenu dans l’adhérence d’un ensemble dénombrable de points de F, que nous rangerons en une suite $(a_n)$. Soit $A_{n,p}$ l’ensemble des $x \in K - N$ tels que $d(f(x), a_n) \leq 1/p$. Il résulte de la condition a) que $A_{n,p}$ est mesurable. Pour $p$ fixé, définissons par récurrence une suite d’ensembles $B_{n,p} \subset K - N$ en posant $B_{1,p} = A_{1,p}$ et $B_{n+1,p} = A_{n+1,p} \cap \bigcap_{k \leq n} C(\bigcup_k A_{k,p})$; les $B_{n,p}$ sont mesurables et ceux qui ne sont pas vides forment une partition de $K - N$. Soit $g_{m,p}$ la fonction égale à $a_i$ dans l’ensemble $B_{i,p}$ pour $1 \leq i \leq m$, et égale à une constante $b \in F$ dans le complémentaire de la réunion de ces ensembles ; $g_{m,p}$ est une fonction étagée mesurable ; lorsque $m$ croît indéfiniment, $g_{m,p}$ converge simplement vers la fonction $f_p$ égale à $a_n$ dans $B_{n,p}$ ($n \geq 1$) et à $b$ dans $N \cup C K$, donc (th. 2) $f_p$ est mesurable. Lorsque $p$ croît indéfiniment, $f_p(x)$ tend vers $f(x)$ pour tout $x \in K - N$, et vers $b$ pour $x \in N \cup C K$; la limite des $f_p$ est donc mesurable, et le principe de localisation prouve que $f$ elle-même est mesurable.

#### Remarque 1 {#int-iv-s5-n5-rem-1 .statement}

La condition a) seule ne suffit pas pour que $f$ soit mesurable (exerc. 7).
2) Si la topologie de F admet une base dénombrable, la condition b) du th. 4 est automatiquement remplie pour toute application de X dans F. La démonstration prouve en outre qu’il suffit de supposer que les images réciproques par $f$ des boules fermées de rayon rationnel, dont le centre appartient à un ensemble dénombrable partout dense dans F, sont des ensembles mesurables.
3) On peut remplacer l’hypothèse a) par la condition que l’image réciproque par $f$ de toute boule ouverte de F est mesurable.

Le cas des fonctions numériques (finies ou non) mérite une mention particulière :

#### Proposition 8 {#int-iv-s5-prop-8 .statement}

Soit D un ensemble dénombrable partout dense dans $\mathbf{R}$. Pour qu’une fonction numérique (finie ou non) $f$ soit mesurable, il suffit (et il faut) que pour tout $a \in D$, l’ensemble des $x \in X$ tels que $f(x) \geq a$ soit mesurable.

En effet, s’il en est ainsi, pour tout $b \in \bar{\mathbf{R}}$, l’ensemble des $x$ tels que $f(x) \geq b$ est mesurable, comme intersection des ensembles (formant une famille dénombrable) des $x$ tels que $f(x) \geq a$, lorsque $a$ parcourt l’ensemble des points de D qui sont $\leq b$. L’ensemble des $x$ tels que $f(x) < b$ est mesurable, comme complémentaire d’un ensemble mesurable. Enfin, si $b$ est fini, l’ensemble des $x$ tels que $f(x) \leq b$ est mesurable, comme intersection des ensembles des $x$ tels que $f(x) < b + 1/n$; et $f^{-1}(-\infty)$ est mesurable comme intersection des ensembles des $x$ tels que $f(x) < n$, où $n$ parcourt $\mathbf{Z}$. Finalement, l’image réciproque par $f$ de tout intervalle fermé de $\bar{\mathbf{R}}$ est mesurable, comme intersection de deux ensembles mesurables, et le th. 4 s’applique.

On montrerait de même qu’il suffit que pour tout $a \in D$, l’ensemble des $x$ tels que $f(x) > a$ soit mesurable.

#### Corollaire {#int-iv-s5-n5-cor-1 .statement}

*Toute fonction semi-continue inférieurement* (resp. *supérieurement*) *est mesurable*.

En effet, si $f$ est semi-continue inférieurement, l’ensemble des $x \in X^-$ tels que $f(\bar{x}) \leq a$ est fermé pour tout $a \in \bar{\mathbf{R}}$.

La prop. 7 permet de préciser comme suit le th. 3 lorsque F est métrisable et *compact* :

#### Proposition 9 {#int-iv-s5-prop-9 .statement}

*Si F est un espace métrisable et compact, toute application mesurable f de X dans F est limite uniforme (dans X tout entier) d’une suite de fonctions étagées mesurables*.

Soit $d$ une distance compatible avec la topologie de F. Pour tout entier $n$, il existe un nombre *fini* de points $a_k \in F$ tels que les boules fermées $B_k$ de centre $a_k$ et de rayon $1/n$ forment un recouvrement de F ; les ensembles $A_k = f^{-1}(B_k)$ sont donc mesurables (prop. 7), et forment un recouvrement de X. Il existe par suite (§ 4, n° 9, lemme 1) une partition $(C_i)$ de X en un nombre fini d’ensembles mesurables telle que chacun des $A_h$ soit réunion d’un nombre fini des $C_i$. Soient $c_i$ un point de $C_i$, et $g_n$ la fonction étagée mesurable égale à $f(c_i)$ dans $C_i$ (pour chaque indice i). Il est clair que $d(f(x), g_n(x)) \leq 2/n$ pour tout $x \in X$.

#### Proposition 10 {#int-iv-s5-prop-10 .statement}

*Soient F un espace de Banach de type dénombrable, F' son dual, $(\mathbf{a}'_n)$ une suite faiblement dense dans la boule unité de F' (Esp.-vect.-top., chap.-IV,-§ 5; n° 1, prop.-2). Pour qu’une application f de X dans F soit mesurable, il faut et il suffit que pour tout n la fonction scalaire $x \mapsto \langle \mathbf{f}(x), \mathbf{a}'_n \rangle$ soit mesurable*.

La condition étant évidemment nécessaire (n° 3, th. 1), prouvons qu’elle est suffisante ; il suffit de vérifier la condition a) du th. 4, et pour cela, en vertu du principe de localisation, il suffit de prouver que pour toute partie compacte K de X et toute boule fermée B $\subset F$, de centre $a$ et de rayon $r$, l’ensemble $A = K \cap f^{-1}(B)$ est mesurable; or, pour tout $z \in F$, on a
$$
|z| = \sup_n |\langle z, a'_n \rangle| / |a'_n|;
$$
A est donc l’intersection de $K$ et des ensembles définis par
$$
|\langle f(x), a'_n \rangle - \langle a, a'_n \rangle| \leq r |a'_n|;
$$
comme ces ensembles sont mesurables par hypothèse, A est mesurable.

#### Corollaire 1 {#int-iv-s5-prop-10-cor-1 .statement}

Soit F un espace de Banach. Pour qu’une application $f$ de X dans F soit mesurable, il faut et il suffit qu’elle vérifie les deux conditions suivantes:
a) pour tout $a' \in F'$, la fonction scalaire $x \mapsto \langle f(x), a' \rangle$ est mesurable;
b) pour tout ensemble compact $K \subset X$, il existe une partie dénombrable $H$ de F telle que $f(x) \in \overline{H}$ pour presque tout $x \in K$.

La nécessité des conditions résulte du n° 3, th. 1 et du th. 4. Pour prouver que les conditions sont suffisantes, il suffit encore de vérifier la condition a) du th. 4. Avec les mêmes notations que dans la démonstration de la prop. 10, on peut (en vertu de b)) supposer, en modifiant au besoin $f$ dans un ensemble négligeable, que l’on a $f(K) \subset \overline{H}$, où $H$ est une partie dénombrable de F. Si V est le sous-espace vectoriel fermé de F engendré par l’ensemble $H \cup \{a\}$, V est un espace de Banach de type dénombrable et toute forme linéaire continue dans V est la restriction d’une forme $a' \in F'$; le même raisonnement que dans la prop. 10 montre alors que $K \cap f^{-1}(B)$ est mesurable.

#### Corollaire 2 {#int-iv-s5-prop-10-cor-2 .statement}

Soient F un espace localement convexe métrisable de type dénombrable, $F'$ son dual. Pour qu’une application $f$ de X dans F soit mesurable, il faut et il suffit que pour tout $a' \in F'$, la fonction scalaire $x \mapsto \langle f(x), a' \rangle$ soit mesurable.

En effet, F peut être considéré comme un sous-espace d’un produit dénombrable $\prod_n E_n$ d’espaces de Banach (Esp. vect. top., chap. II, 2e éd., § 4, n° 3), et l’on peut supposer que $\mathrm{pr}_n(F)$ est dense dans $E_n$, qui est donc de type dénombrable. Pour tout $n$, l’application $\mathrm{pr}_n \circ f$ est alors mesurable en vertu de la prop. 10, donc $f$ est mesurable en vertu du n° 3, th. 1.

#### Proposition 11 {#int-iv-s5-prop-11 .statement}

Soit F un espace localement convexe, limite inductive d’une suite d’espaces localement convexes métrisables $F_n$ de type dénombrable, F étant réunion des $F_n$. Soit $F'$ le dual de F muni de la topologie faible $\sigma(F', F)$. Pour qu’une application $f$ de X dans $F'$ soit mesurable, il faut et il suffit que, pour tout $a \in F$, la fonction scalaire $x \mapsto \langle a, f(x) \rangle$ soit mesurable.

La condition est nécessaire en vertu du n° 3, th. 1 ; prouvons qu’elle est suffisante. Supposons d’abord que F soit métrisable et de type dénombrable, et soit D un ensemble dénombrable dense dans F. Soit $(V_n)$ une suite fondamentale décroissante de voisinages ouverts convexes équilibrés de 0 dans F ; les ensembles polaires $V_n^o$ sont équicontinu et leur réunion est $F'$ tout entier. Soit $X_n = f^{-1}(V_n^o)$; la suite $(X_n)$ est croissante et $X = \bigcup_n X_n$; montrons que chacun des $X_n$ est $\mu$-mesurable. En effet, $D \cap V_n$ est dense dans $V_n$; pour tout $y \in D \cap V_n$, soit $S_y$ l’ensemble des $x \in X$ tels que $|\langle y, f(x) \rangle| \leq 1$; l’hypothèse entraîne que chacun des $S_y$ est mesurable, et $X_n$ est l’intersection de la famille dénombrable des $S_y$ pour $y \in D \cap V_n$. Cela étant, pour toute partie compacte K de X et tout $\varepsilon > 0$, il existe un entier $n$ tel que $|\mu|(K - (K \cap X_n)) \leq \varepsilon/4$, puis une partie compacte $K_1$ de $K \cap X_n$ telle que $|\mu|((K \cap X_n) - K_1) \leq \varepsilon/4$; enfin, il existe une partie compacte $K_2$ de $K_1$ telle que $|\mu|(K_1 - K_2) \leq \varepsilon/2$ et que les restrictions à $K_2$ de toutes les fonctions $\langle y, f \rangle$, où $y \in D$, soient continues (n° 1, prop. 2). Comme l’ensemble $f(K_2) \subset f(X_n) \subset V_n^o$ est équicontinu, la topologie induite par $\sigma(F', F)$ sur $f(K_2)$ est identique à la topologie de la convergence simple dans D (Top. gén., chap. X, 2e éd., § 2, n° 4, th. 1); par suite, la restriction de f à $K_2$ est continue, d’où notre assertion dans ce premier cas.

Passons au cas général. Si $z'$ est une forme linéaire continue sur F, sa restriction $z'_n$ à $F_n$ est continue; comme $F = \bigcup_n F_n$, le dual $F'$ de F peut être identifié (algébriquement) à un sous-espace vectoriel du produit $\prod_n F'_n$, et l’on a $\mathrm{pr}_n(z') = z'_n$. En outre, toute partie finie de F étant contenue dans l’un des $F_n$, la topologie $\sigma(F', F)$ n’est autre que la topologie induite par la topologie produit des topologies $\sigma(F'_n, F_n)$. Cela étant, si $\langle a, f \rangle$ est mesurable pour tout $a \in F$, il en est de même de $\langle a_n, \mathrm{pr}_n \circ f \rangle$ pour tout $n$ et tout $a_n \in F_n$, puisque $\langle a_n, \mathrm{pr}_n \circ f \rangle = \langle a_n, f \rangle$; la première partie de la démonstration montre donc que $\mathrm{pr}_n \circ f$ est mesurable pour tout $n$, et il en est donc de même de $f$ (n° 3, th. 1).

### 6. Critères d’intégrabilité

#### Théorème 5 {#int-iv-s5-thm-5 .statement}

Pour qu’une application $f$ de $X$ dans un espace de Banach $F$ soit de puissance $p$-ième intégrable ($1 \leq p < +\infty$), il faut et il suffit que $f$ soit mesurable et que $N_p(f)$ soit finie.

La condition est nécessaire : en effet, si $f \in \mathcal{L}_F^p$, il existe une suite $(g_n)$ de fonctions continues à support compact qui converge presque partout vers $f$ ($§ 3$, n° 4, cor. 2 du th. 3); en vertu du th. 2 du n° 4, $f$ est mesurable.

Pour prouver que les conditions sont suffisantes, nous établirons d’abord un lemme :

#### Lemme 1 {#int-iv-s5-lem-1 .statement}

Soit $g$ une fonction à valeurs dans $F$, telle que $N_p(g) < +\infty$ (autrement dit, une fonction de $\mathcal{F}_F^p$). L’ensemble $A$ de points $x \in X$ tels que $g(x) \neq 0$ est contenu dans la réunion d’un ensemble négligeable et d’une suite d’ensembles compacts.

En effet, soit $A_n$ l’ensemble des points $x \in X$ tels que $|g(x)| \geq 1/n$; $A$ est réunion des $A_n$, et on a $\varphi_{A_n} \leq n|g|$, d’où $|\mu|^*(A_n) \leq (nN_p(g))^p$; $A_n$ est donc contenu dans la réunion d’un ensemble négligeable et d’une suite d’ensembles compacts ($§ 4$, n° 6, cor. 3 du th. 4); par suite, il en est de même de $A$.

Ce lemme étant démontré, considérons d’abord le cas où $f$ a un support compact $K$. D’après le cor. 1 du th. 3 du n° 4, il existe une suite $(g_n)$ de fonctions étagées mesurables telles que

$$
|g_n(x)| \leq |f(x)|
$$

en tout point $x \in X$, et que $g_n(x)$ tende presque partout vers $f(x)$. Or, $g_n$ est combinaison linéaire de fonctions caractéristiques d’ensembles mesurables contenus dans $K$; ces ensembles étant intégrables en vertu de la prop. 3 du n° 1, $g_n$ appartient à $\mathcal{L}_F^p$. Comme $N_p(f) < +\infty$, le th. de Lebesgue ($§ 3$, n° 7, th. 6) montre que $f$ appartient à $\mathcal{L}_F^p$.

Dans le cas général, il résulte du lemme 1 qu’il existe une suite croissante $(K_n)$ d’ensembles compacts telle que $f(x)$ soit nulle presque partout dans le complémentaire de la réunion des $K_n$. Soit $f_n$ la fonction égale à $f(x)$ dans $K_n$, et à 0 ailleurs ; $f_n$ est mesurable en vertu du n° 3, cor. 5 du th. 1; comme $|f_n| \leq |f|$, $f_n$ appartient à $\mathcal{L}_F^p$ en vertu de la première partie du raisonnement. Comme $f(x)$ est presque partout égale à la limite de la suite des $f_n(x)$, le th. de Lebesgue prouve encore que $f \in \mathcal{L}_F^p$, ce qui achève la démonstration.

On aura soin de noter qu’une fonction localement négligeable mais non négligeable n’est pas intégrable; une fonction égale localement presque partout à une fonction intégrable n’est donc pas nécessairement intégrable.

#### Corollaire 1 {#int-iv-s5-lem-1-cor-1 .statement}

Pour qu’un ensemble soit intégrable, il faut et il suffit qu’il soit mesurable et de mesure extérieure finie.

#### Corollaire 2 {#int-iv-s5-lem-1-cor-2 .statement}

Soit $(\mathbf{F}_n)$ une suite d’espaces topologiques; pour chaque indice $n$, soit $f_n$ une application mesurable de $X$ dans $\mathbf{F}_n$, et soit $f(x) = (f_n(x)) \in F = \prod_n \mathbf{F}_n$; soit enfin $\mathbf{u}$ une application continue de $f(X)$ dans un espace de Banach $G$. Pour que la fonction $g(x) = \mathbf{u}(f(x))$ soit intégrable, il faut et il suffit que $N_1(g) < +\infty$.

En effet, $g$ est mesurable (n° 3, th. 1).

#### Corollaire 3 {#int-iv-s5-lem-1-cor-3 .statement}

Pour toute fonction intégrable $f$ et tout ensemble mesurable $A$, la fonction $f \varphi_A$ est intégrable.

En effet, il résulte du th. 5 et du n° 3, cor. 5 du th. 1 que $f \varphi_A$ est mesurable, et on a $N_1(f \varphi_A) \leq N_1(f)$.

On pose $\int_A f d\mu = \int f \varphi_A d\mu$ (ou $\int_A f \mu$) pour toute fonction intégrable $f$ et tout ensemble mesurable $A$. On écrit aussi $\int_A^* f d|\mu|$ (ou $\int_A^* f |\mu|$) au lieu de $\int_A^* f \varphi_A d|\mu|$ pour toute fonction numérique (finie ou non) $f \geq 0$ (en posant $f(x) \varphi_A(x) = 0$ si $f(x) = +\infty$ et $\varphi_A(x) = 0$).

#### Corollaire 4 {#int-iv-s5-lem-1-cor-4 .statement}

Pour toute suite $(f_n)$ de fonctions mesurables $\geq 0$ sur $X$, on a

(1)
$$
\int^* \left( \sum_n f_n \right) d|\mu| = \sum_n \int^* f_n d|\mu|.
$$

Compte tenu du § 1, n° 3, th. 3, on est ramené à prouver que pour deux fonctions mesurables $f \geq 0$, $g \geq 0$ sur $X$, on a

(2)
$$
\int^* (f + g) d|\mu| = \int^* f d|\mu| + \int^* g d|\mu|.
$$

Ce n’est autre que l’additivité de l’intégrale lorsque $f$ et $g$ sont intégrables. Dans le cas contraire, si par exemple $f$ est non intégrable, on a $\int^* f d|\mu| = +\infty$ en vertu du th. 5; $a$ fortiori, on a $\int^* (f + g) d|\mu| = +\infty$.

#### Corollaire 5 {#int-iv-s5-lem-1-cor-5 .statement}

Pour toute suite $(A_n)$ d’ensembles mesurables deux à deux disjoints, on a
$$
|\mu|^*(\bigcup_n A_n) = \sum_n |\mu|^*(A_n).
$$
Cela résulte du cor. 4 appliqué aux $\varphi_{A_n}$.

### 7. Mesure induite sur un sous-espace localement compact

Soient X un espace localement compact, $\mu$ une mesure sur X, Y un sous-espace localement compact de X. Comme Y est l’intersection d’un ensemble ouvert et d’un ensemble fermé dans X (Top. gén., chap. I, 3e éd., §9, n° 7, prop. 12), il est $\mu$-mesurable (n° 1, cor. de la prop. 3). Pour toute fonction $g \in \mathcal{K}(Y; \mathbf{C})$, soit $g'$ la fonction définie dans X, égale à g dans Y et à 0 dans X − Y ; montrons que $g'$ est $\mu$-intégrable. On peut se borner au cas où g est réelle et $\geqslant 0$ (en écrivant g comme combinaison linéaire de telles fonctions); comme $g'$ est bornée et à support compact, il suffit de montrer que $g'$ est $\mu$-mesurable (n° 6, th. 5); mais cela résulte de ce que $g'$ est semi-continue supérieurement dans X (n° 5, cor. de la prop. 8). On peut donc poser la définition suivante :

#### Définition 4 {#int-iv-s5-def-4 .statement}

Etant donné un sous-espace localement compact Y d’un espace localement compact X, on appelle mesure induite sur Y par une mesure $\mu$ sur X, et l’on note $\mu_Y$ ou $\mu|Y$, la mesure définie par la formule
$$
\int g\, d\mu_Y = \int g'\, d\mu
$$
pour toute fonction $g \in \mathcal{K}(Y; \mathbf{C})$, $g'$ désignant la fonction égale à g dans Y et à 0 dans X − Y.

#### Exemple {#int-iv-s5-n7-exa-1 .statement}

Soient $\mu$ la mesure de Lebesgue sur $\mathbf{R}$, I un intervalle quelconque dans $\mathbf{R}$; I est un sous-espace localement compact de $\mathbf{R}$ et la mesure induite par $\mu$ sur I est la forme linéaire
$$
g \mapsto \int_a^b g(x)\, dx
$$
sur $\mathcal{K}(I; \mathbf{C})$, en désignant par $a$ et $b$ l’origine et l’extrémité (finies ou non) de I (cf. §4, n° 4, Exemple), autrement dit ce que nous avons appelé la mesure de Lebesgue sur I.

Lorsque Y est un sous-espace ouvert de X, la déf. 1 coïncide avec la définition de la mesure induite par $\mu$ sur Y (ou restriction de $\mu$ à Y) donnée au chap. III, § 2, n° 1 : en effet, pour toute fonction $g \in \mathcal{K}(Y; \mathbf{C})$, la fonction $g'$ est alors continue dans X.

Nous étudierons en détail au chap. V, § 5 l’intégration par rapport à une mesure induite, et n’aurons besoin jusque-là que des résultats suivants :

#### Lemme 2 {#int-iv-s5-lem-2 .statement}

Soient $\mu$ une mesure positive sur X, K une partie compacte de X.

(i) Pour toute partie compacte (resp. ouverte) H de K, on a $\mu_K(H) = \mu(H)$.

(ii) Pour qu’une partie N de K soit $\mu_K$-négligeable, il faut et il suffit qu’elle soit $\mu$-négligeable.

(iii) Si S est le support de $\mu_K$, on a $\mathrm{Supp}(\mu_S) = S$.

(i) On peut se borner au cas où H est compact. Désignons par $f$ la fonction caractéristique de H dans l’espace K ; $f$ est semi-continue supérieurement, et est donc enveloppe inférieure d’une famille filtrante décroissante $(g_\alpha)$ de fonctions de $\mathcal{K}_+(K)$; on a $\mu_K(H) = \inf \int g_\alpha d\mu_K$ ($§ 4$, n° 4, cor. 2 de la prop. 5). Si $g'_\alpha$ est la fonction égale à $g_\alpha$ dans K, à 0 dans $X - K$, $g'_\alpha$ est semi-continue supérieurement, et l’enveloppe inférieure de la famille filtrante décroissante $(g'_\alpha)$ est la fonction caractéristique $\varphi_H$ de H dans l’espace X ; on a donc
$$
\mu(H) = \inf_\alpha \int g'_\alpha d\mu = \inf_\alpha \int g_\alpha d\mu_K = \mu_K(H)
$$
en vertu de (1).

(ii) Si N est $\mu$-négligeable, pour tout $\varepsilon > 0$ il existe un voisinage ouvert relativement compact U de N dans X tel que $\mu(U) \leq \varepsilon$; comme $K - (U \cap K)$ est compact, il résulte de (i) que $\mu_K(U \cap K) \leq \mu(U) \leq \varepsilon$, donc N est $\mu_K$-négligeable. Réciproquement, si N est $\mu_K$-négligeable, il existe un voisinage ouvert V de N dans X tel que $\mu_K(V \cap K) \leq \varepsilon$; en vertu de (i), on a
$$
\mu(V \cap K) = \mu_K(V \cap K),
$$
donc $\mu(N) = 0$ puisque $\varepsilon$ est arbitraire.

(iii) Pour toute partie ouverte U de K rencontrant S, on a par hypothèse $\mu_K(U \cap S) \neq 0$, donc $\mu(U \cap S) \neq 0$ par (i), et comme $U \cap S$ est ouvert dans S, $\mu_S(U \cap S) \neq 0$ par (i); comme tout ensemble ouvert non vide dans S est de la forme $U \cap S$, où U est ouvert dans K, cela prouve que $\mathrm{Supp}(\mu_S) = S$.

#### Lemme 3 {#int-iv-s5-lem-3 .statement}

Soit Y un sous-espace localement compact de X ; pour toute mesure $\mu$ sur X, on a $|\mu_Y| = |\mu|_Y$.

Soient $f$ une fonction de $\mathcal{K}_+(Y)$, $\varepsilon$ un nombre $> 0$ arbitraire ; par définition, il existe une fonction $g \in \mathcal{K}(Y; \mathbf{C})$ telle que $|g| \leq f$ et $|\mu_Y|(f) \leq |\mu_Y(g)| + \varepsilon$. Si l’on désigne par $f'$ et $g'$ les fonctions obtenues respectivement en prolongeant $f$ et $g$ par 0 dans $X - Y$, on a $\mu_Y(g) = \mu(g')$, et comme $|g'| \leq f'$,

$$
|\mu(g')| \leq |\mu|(|g'|) \leq |\mu|(f') = |\mu|_Y(f)
$$

d’où $|\mu_Y|(f) \leq |\mu|_Y(f) + \varepsilon$, et comme $\varepsilon$ est arbitraire,

$$
|\mu_Y|(f) \leq |\mu|_Y(f).
$$

D’autre part, soient $K$ le support de $f$, $U$ un voisinage compact de $K$ dans $X$ tel que $|\mu|(U - K) \leq \varepsilon$; en vertu du th. d’Urysohn, il existe une fonction $f_1 \in \mathcal{K}_+(X)$, prolongeant $f$, de support contenu dans $U$ et telle que $\|f_1\| = \|f\|$. Il existe une fonction $h_1 \in \mathcal{K}(X; \mathbf{C})$ telle que $|h_1| \leq f_1$ et que $|\mu|(f_1) \leq |\mu(h_1)| + \varepsilon$. Si $h$ est la restriction de $h_1$ à $Y$, on a $h \in \mathcal{K}(Y; \mathbf{C}), |h| \leq f$, et $\mu(h_1) - \mu_Y(h) = \mu(h_1 \varphi_{U-K})$, donc $|\mu(h_1) - \mu_Y(h)| \leq \|f\| \cdot |\mu|(U - K) \leq \varepsilon \|f\|$; par ailleurs, on a de même

$$
|\mu|(f_1) - |\mu|_Y(f) = |\mu|(f_1 \varphi_{U-K}) \quad \text{et} \quad ||\mu|(f_1) - |\mu|_Y(f)|| \leq \varepsilon \|f\|.
$$

On en tire que

$$
|\mu|_Y(f) \leq |\mu_Y(h)| + \varepsilon(1 + 2\|f\|) \leq |\mu_Y|(f) + \varepsilon(1 + 2\|f\|)
$$

et comme $\varepsilon$ est arbitraire, $|\mu|_Y(f) \leq |\mu_Y|(f)$, ce qui achève la démonstration.

### 8. Familles $\mu$-denses d’ensembles compacts.

#### Proposition 12 {#int-iv-s5-prop-12 .statement}

Soient $\mu$ une mesure sur un espace localement compact $X$, $A$ une partie $\mu$-mesurable de $X$, $\mathfrak{R}$ un ensemble de parties compactes de $A$, satisfaisant aux conditions suivantes :

(PL_I) Toute partie fermée (donc compacte) d’un ensemble de $\mathfrak{R}$ appartient à $\mathfrak{R}$.

(PL_{II}) Toute réunion finie d’ensembles de $\mathfrak{R}$ appartient à $\mathfrak{R}$.
Les quatre propriétés suivantes sont alors équivalentes :
a) Pour qu’une partie $B$ de $A$ soit localement $\mu$-négligeable, il faut et il suffit que $|\mu|^*(B \cap K) = 0$ pour tout $K \in \mathfrak{R}$.
b) Pour tout partie compacte $K_0$ de $A$ et tout $\varepsilon > 0$, il existe une partie $K \in \mathfrak{R}$, contenue dans $K_0$ et telle que $|\mu|(K_0 - K) \leq \varepsilon$.
c) Pour toute partie compacte $B$ de $A$, il existe une partition de $B$ formée d’un ensemble $\mu$-négligeable $N$ et d’une suite $(H_n)$ d’ensembles compacts appartenant à $\mathfrak{R}$.

d) Pour toute partie compacte B de A. il existe une suite croissante $(K_n)$ d’ensembles compacts de $A$, contenus dans B et tels que l’ensemble $N = B - \bigcup_n K_n$ soit $\mu$-négligeable.

Il est immédiat (n° 2, prop. 5) que d) entraîne a); c) entraîne d) en prenant pour $K_n$ la réunion des $H_p$ tels que $p \leq n$, et en utilisant (PL_{II}). Pour démontrer que b) entraîne c), on définit par récurrence une suite $(H_p)$ d’ensembles de $A$ de sorte que $H_{n+1} \subset B - \bigcup_{p \leq n} H_p$ et que l’on ait $|\mu| \left( B - \bigcup_{p \leq n} H_p \right) \leq 1/n$ (§ 4, n° 6, th. 4). Reste enfin à prouver que a) entraîne b). Raisonnons par l'absurde, et supposons que la borne supérieure $\alpha$ des nombres $|\mu|(K)$, où K parcourt l'ensemble des parties de $K_0$ appartenant à $A$, soit $< |\mu|(K_0)$. En vertu de (PL_{II}), il existe une suite croissante $(L_n)$ de parties compactes de $K_0$, appartenant à $A$ et telle que $\sup_n |\mu|(L_n) = \alpha$.

Posons $B = \bigcup_n L_n$; B est intégrable et l'on a $|\mu|(B) = \alpha$, donc $|\mu|(K_0 - B) = |\mu|(K_0) - \alpha > 0$. Mais nous allons voir d'autre part que, pour toute partie $K \in A$, on a $|\mu|(K \cap (K_0 - B)) = 0$, ce qui, en vertu de a), entraînera contradiction. En effet, s'il existait une partie $K \in A$ telle que $|\mu|(K \cap (K_0 - B)) > 0$, il existerait une partie compacte H de $K \cap (K_0 - B)$ telle que $|\mu|(H) > 0$. D'après (PL_I), on aurait $H \in A$ et, pour $n$ assez grand,

$$
|\mu|(L_n \cup H) = |\mu|(L_n) + |\mu|(H) > \alpha.
$$

Mais $L_n \cup H$ appartient à $A$ en vertu de (PL_{II}), et cela contredit la définition de $\alpha$.

#### Définition 6 {#int-iv-s5-def-6 .statement}

Soit A une partie $\mu$-mesurable de X. On dit qu’un ensemble $A$ de parties compactes de A est $\mu$-dense dans A s’il vérifie les conditions (PL_I), (PL_{II}), a), b), c), d) de la prop. 12.

L’ensemble de toutes les parties compactes de A est $\mu$-dense dans A.

Lorsque $A = X$, on dira simplement « ensemble $\mu$-dense » au lieu de « ensemble $\mu$-dense dans X ». Si $X - A$ est localement $\mu$-négligeable, tout ensemble de parties compactes de A, $\mu$-dense dans A, est $\mu$-dense dans X.

#### Remarque {#int-iv-s5-n8-rem-1 .statement}

Supposons que A soit réunion d’une suite $(L_n)$ d’ensembles compacts et d’un ensemble $\mu$-négligeable (resp. localement $\mu$-négligeable), et soit $A$ un ensemble de parties compactes, μ-dense dans A. Appliquant à chaque $L_n$ la propriété c) de l’énoncé de la prop. 12, on voit que A est réunion d’une suite d’ensembles compacts appartenant à $\mathfrak{R}$ et d’un ensemble $\mu$-négligeable (resp. localement $\mu$-négligeable).

Si K est une partie compacte de X, il revient au même de dire qu’un ensemble de parties compactes de K est $\mu$-dense dans K ou $\mu_K$-dense dans K ; cela résulte des lemmes 2 et 3 du n° 7 et de la condition b) de la prop. 12.

#### Proposition 13 {#int-iv-s5-prop-13 .statement}

Soient A une partie $\mu$-mesurable de X, $\mathfrak{R}$ un ensemble de parties compactes, $\mu$-dense dans A. Soit $\mathfrak{H}$ un ensemble de parties compactes de A satisfaissant à (PL_I) et (PL_{II}) et tel que, pour tout $K \in \mathfrak{R}$, l’ensemble des $H \in \mathfrak{H}$ tels que $H \subset K$ soit $\mu_K$-dense (ou, ce qui revient au même, $\mu$-dense) dans K. Alors $\mathfrak{H}$ est $\mu$-dense dans A.

En effet, soit L une partie compacte de A. Pour tout $\varepsilon > 0$, il existe $K \in \mathfrak{R}$ tel que $K \subset L$ et $|\mu|(L - K) \leq \varepsilon/2$, puis $H \in \mathfrak{H}$ tel que $H \subset K$ et $|\mu|(K - H) \leq \varepsilon/2$; on en déduit $|\mu|(L - H) \leq \varepsilon$, d’où la proposition.

### 9. Partitions localement dénombrables

#### Définition 7 {#int-iv-s5-def-7 .statement}

On dit qu’un ensemble de parties $\mathfrak{U}$ d’un espace topologique T est localement dénombrable si, pour tout $t \in T$, il existe un voisinage V de t tel que l’ensemble des $A \in \mathfrak{U}$ rencontrant V soit dénombrable.

Si l’ensemble $\mathfrak{U}$ de parties de T est localement dénombrable, alors, pour toute partie compacte K de T, l’ensemble des $A \in \mathfrak{U}$ rencontrant K est dénombrable, puisqu’on peut recouvrir K par un nombre fini de voisinages ouverts de points de K, dont chacun ne rencontre qu’un sous-ensemble dénombrable de parties appartenant à $\mathfrak{U}$.

La déf. 7 montre que la réunion d’une ensemble localement dénombrable de parties $\mu$-mesurables (resp. localement $\mu$-négligeables) d’un espace localement compact est $\mu$-mesurable (resp. localement $\mu$-négligeable) (n° 1, prop. 3 et n° 2, prop. 5).

#### Proposition 14 {#int-iv-s5-prop-14 .statement}

Soient X un espace localement compact, $\mu$ une mesure sur X, A une partie $\mu$-mesurable de X, $\mathfrak{R}$ un ensemble de parties compactes de A, $\mu$-dense dans A. Il existe un ensemble $\mathfrak{H} \subset \mathfrak{R}$ localement dénombrable, formé de parties deux à deux disjointes, tel que $A - \bigcup_{K \in \mathcal{H}} K$ soit localement $\mu$-négligeable et que, pour tout $K \in \mathcal{H}$, le support de $\mu_K$ soit $K$ tout entier.

Considérons les ensembles $\Omega \subset \mathfrak{R}$ formés d’ensembles deux à deux disjoints tels que, pour tout $L \in \Omega$, on ait $\mathrm{Supp}(\mu_L) = L$. Ces ensembles $\Omega$ forment une partie $\mathcal{H}$ de $\mathfrak{P}(\mathfrak{R})$, qui est non vide (car elle contient l’élément $\emptyset$) et que nous ordonnerons par la relation d’inclusion dans $\mathfrak{P}(\mathfrak{R})$. Il est immédiat que $\mathcal{H}$ est *inductif* ; soit $\mathcal{H}$ un élément maximal de $\mathcal{H}$ (*Ens. R*, § 6, no 10). Montrons tout d’abord que $\mathcal{H}$ est *localement dénombrable*. En effet, pour tout $x \in X$, soit $V$ un voisinage ouvert relativement compact de $x$; si $(K_i)_{1 \leq i \leq n}$ est une famille finie d’ensembles distincts de $\mathcal{H}$ rencontrant $V$, on a $\sum_{i=1}^n |\mu|(K_i \cap V) = |\mu|\left(V \cap \left( \bigcup_{i=1}^n K_i \right)\right)$ puisque les $K_i$ sont deux à deux disjoints, d’où $\sum_{i=1}^n |\mu|(K_i \cap V) \leq |\mu|(V)$. Si $\mathcal{H}_V$ est l’ensemble des $K \in \mathcal{H}$ rencontrant $V$, on a donc
$$
\sum_{K \in \mathcal{H}_V} |\mu|(K \cap V) < +\infty,
$$
et comme $|\mu|(K \cap V) > 0$ pour tout $K \in \mathcal{H}_V$, $\mathcal{H}_V$ est nécessairement dénombrable. Prouvons ensuite que $N = A - \bigcup_{K \in \mathcal{H}} K$ est localement $\mu$-négligeable. On a vu plus haut que $N$ est $\mu$-mesurable. Si $N$ n’était pas localement négligeable, il contiendrait un ensemble compact non négligeable $L_0$, et par suite (no 8, prop. 12) un ensemble compact non négligeable $L \subset L_0$ appartenant à $\mathfrak{R}$. Comme $|\mu_L|(L) = |\mu|(L) > 0$ (no 7, lemmes 2 et 3), la mesure induite $\mu_L$ sur $L$ par $\mu$ n’est pas nulle; son support $S$ est donc une partie compacte non vide appartenant à $\mathfrak{R}$ en vertu de (PL₁), et l’on a $\mathrm{Supp}(\mu_S) = S$ (no 7, lemme 2, (iii)). On en conclut que l’ensemble $\mathcal{H} \cup \{S\}$ appartiendrait à $\mathcal{H}$, ce qui contredit la définition de $\mathcal{H}$; l’ensemble $N$ est donc localement négligeable, ce qui achève la démonstration.

### 10. Fonctions mesurables définies dans une partie mesurable

#### Proposition 15 {#int-iv-s5-prop-15 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$, $A$ une partie $\mu$-mesurable de $X$, $f$ une application de $A$ dans un espace topologique $F$. Les conditions suivantes sont équivalentes :

a) L’ensemble $\mathfrak{H}$ des parties compactes $K$ de $A$ telles que la restriction de $f$ à $K$ soit continue, est $\mu$-dense dans $A$.

b) Il existe un ensemble $\mathfrak{R}$ de parties compactes de $A$, $\mu$-dense dans $A$, et tel que la restriction de $f$ à tout $K \in \mathfrak{R}$ soit $\mu_K$-mesurable.

c) Il existe un homéomorphisme $j$ de $F$ sur un sous-espace d’un espace topologique $G$ et une application $\mu$-mesurable $g$ de $X$ dans $G$, tels que $g|A = j \circ f$.

d) Tout prolongement de $f$ en une application de $X$ dans $F$, constante dans $X - A$, est $\mu$-mesurable.

Il est clair que a) implique b) et que d) implique c). Le fait que c) implique a) résulte de la condition c) de la prop. 12 du n° 8. D’autre part, b) implique a): en effet, la déf. 1 montre que l’ensemble des parties $H \in \mathfrak{R}$ contenues dans un $K \in \mathfrak{R}$ quelconque est $\mu_K$-dense dans $K$ (n° 8, prop. 12, c)), et la prop. 13 du n° 8 montre que $\mathfrak{R}$ est $\mu$-dense dans $A$. Reste à voir que a) implique d). Soit $g$ un prolongement de $f$ à $X$, constant dans $X - A$. Pour toute partie compacte $L$ de $X$, $L \cap A$ et $L \cap (X - A)$ sont $\mu$-intégrables; donc, pour tout $\varepsilon > 0$, il existe une partie compacte $P \subset L \cap A$ et une partie compacte
$$
Q \subset L \cap (X - A)
$$
telles que $|\mu|(L \cap A) - P) \leq \varepsilon/4$ et $|\mu|(L \cap (X - A)) - Q) \leq \varepsilon/4$. Il existe d’autre part une partie $H \in \mathfrak{H}$ contenue dans $P$ et telle que $|\mu|(P - H) \leq \varepsilon/2$; la restriction de $g$ à l’ensemble compact $K = H \cup Q$ est alors continue ($g$ étant constante dans $Q$) et l’on a $|\mu|(L - K) \leq \varepsilon$, ce qui achève la démonstration.

#### Définition 8 {#int-iv-s5-def-8 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$, $A$ une partie $\mu$-mesurable de $X$. On dit qu’une application $f$ de $A$ dans un espace topologique $F$ est $\mu$-mesurable si elle vérifie les conditions équivalentes de la prop. 15.

Si $A$ est localement $\mu$-négligeable, toute application de $A$ dans $F$ est donc $\mu$-mesurable.

#### Corollaire 1 {#int-iv-s5-def-8-cor-1 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$, $A$ une partie $\mu$-mesurable de $X$, $f$ une application $\mu$-mesurable de $A$ dans un espace topologique $F$. Soit $\mathfrak{R}$ un ensemble de parties compactes de $X$, $\mu$-dense dans $X$. Il existe alors une partition de $A$ formée d’un ensemble localement négligeable $N$ et d’une famille localement dénombrable $(K_\lambda)_{\lambda \in L}$ d’ensembles $K_\lambda \in \mathfrak{R}$, telle que $f|K_\lambda$ soit continue pour tout $\lambda \in L$.

Compte tenu du n° 9, prop. 14, il suffit de montrer que l’ensemble $\mathfrak{H} \subset \mathfrak{K}$ des parties $K \in \mathfrak{K}$ telles que $K \subset A$ et que $f|K$ soit continue, est $\mu$-dense dans $A$. Or, il résulte aussitôt de la prop. 1 du n° 1 et de la condition d) de la prop. 15 que, pour toute partie compacte $K_0$ de $A$ et tout $\varepsilon > 0$, il existe une partie $K \subset K_0$ appartenant à $\mathfrak{K}$, telle que $|\mu|(K_0 - K) \leq \varepsilon$ et que $f|K$ soit continue; la conclusion résulte donc de la prop. 12 du n° 8.

#### Corollaire 2 {#int-iv-s5-def-8-cor-2 .statement}

Soit $K$ un sous-espace compact de $X$; pour qu’une application $f$ de $K$ dans un espace topologique $F$ soit $\mu$-mesurable, il faut et il suffit qu’elle soit $\mu_K$-mesurable.

Compte tenu du lemme 2 du n° 7, cela résulte aussitôt de la prop. 1 du n° 1, et de la condition a) de la prop. 15.

#### Proposition 16 {#int-iv-s5-prop-16 .statement}

Soit $\mathfrak{U}$ un ensemble localement dénombrable de parties $\mu$-mesurables de $X$, et soit $B = \bigcup_{A \in \mathfrak{U}} A$. Pour qu’une application $f$ de $B$ dans un espace topologique $F$ soit $\mu$-mesurable, il faut et il suffit que la restriction de $f$ à tout $A \in \mathfrak{U}$ soit $\mu$-mesurable.

On a déjà remarqué (n° 9) que $B$ est $\mu$-mesurable. La condition étant évidemment nécessaire, prouvons qu’elle est suffisante. Soit donc $K$ une partie compacte de $B$. Par hypothèse, il existe une suite $(A_n)$ d’ensembles appartenant à $\mathfrak{U}$ et telle que les $K \cap A_n$ forment un recouvrement de $K$. Posons $C_0 = K \cap A_0$,

$$
C_n = K \cap A_n \cap \complement \left( \bigcup_{i < n} C_i \right)
$$

pour $n > 0$, de sorte que les $C_n$ non vides forment une partition de $K$ en ensembles $\mu$-intégrables. La restriction de $f$ à $C_n$ étant $\mu$-mesurable, il existe une partition de $C_n$ formée d’un ensemble $\mu$-négligeable $N_n$ et d’une suite $(L_{mn})_{m \geq 0}$ d’ensembles compacts tels que $f|L_{mn}$ soit continue. Comme $N = \bigcup_n N_n$ est $\mu$-négligeable, on voit que la condition a) de la prop. 15 est satisfaite, d’où la proposition.

La propriété d) de la prop. 15 permet aussitôt de généraliser aux fonctions mesurables définies dans une partie mesurable $A$ de $X$ les propriétés des fonctions mesurables définies dans $X$ tout entier vues aux n°s 2 à 5; nous laissons ces généralisations au lecteur. Signalons seulement que le principe de localisation (n° 2, prop. 4) est encore valable lorsqu’on suppose que chacune des fonctions $g_x$ n’est définie que dans $V_x$ (ou presque partout dans $V_x$) et est mesurable.

### 11. Convergence en mesure

Soient X un espace localement compact, $\mu$ une mesure sur X, A une partie $\mu$-mesurable de X, F un espace uniforme; nous désignerons par $\mathcal{S}(A, \mu ; F)$, ou $\mathcal{S}_F(A, \mu)$ (ou simplement $\mathcal{S}_F(\mu)$, ou même $\mathcal{S}_F$, lorsque $A = X$) l’ensemble des applications $\mu$-mesurables de A dans F (n° 10, déf. 8). Pour tout entourage V de la structure uniforme de F, tout ensemble $\mu$-intégrable $B \subset A$ et tout nombre $\delta > 0$, nous désignerons par $W(V, B, \delta)$ l’ensemble des couples $(f, g)$ de fonctions de $\mathcal{S}(A, \mu ; F)$ ayant la propriété suivante: l’ensemble M des $x \in B$ pour lesquels $(f(x), g(x)) \notin V$ est tel que $|\mu|^*(M) \leq \delta$. Montrons que les ensembles $W(V, B, \delta)$ forment un système fondamental d’entourages d’une structure uniforme sur $\mathcal{S}(A, \mu ; F)$: il est clair que $W(V, B, \delta)$ est symétrique si V l’est, et que si $V' \subset V, B' \supset B$ et $\delta' \leq \delta$, on a
$$
W(V', B', \delta') \subset W(V, B, \delta);
$$
il suffit donc de vérifier l’axiome (U_{III}) (Top. gén., chap. II, 3e éd., § 1, n° 1). Or, si $V'$ est un entourage tel que ${V'}^2 \subset V$, on a
$$
W(V', B, \delta/2) \circ W(V', B, \delta/2) \subset W(V, B, \delta).
$$
On notera que lorsque K parcourt un ensemble $\mu$-dense $\mathfrak{K}$ de parties compactes de A, les ensembles $W(V, K, \delta)$ forment aussi un système fondamental d’entourages de la structure uniforme précédente: en effet, pour tout ensemble intégrable $B \subset A$, il existe une partie compacte $K \in \mathfrak{K}$ contenue dans B et telle que $|\mu|(B - K) \leq \delta$, et par suite $W(V, K, \delta) \subset W(V, B, 2\delta)$.

#### Définition 9 {#int-iv-s5-def-9 .statement}

On dit que la structure uniforme sur $\mathcal{S}(A, \mu ; F)$ dont les $W(V, B, \delta)$ forment un système fondamental d’entourages est la structure uniforme de la convergence en mesure dans A.

La topologie correspondante est dite topologie de la convergence en mesure dans A, et on dit qu’un filtre (resp. une suite) qui converge pour cette topologie est convergent (resp. convergente) en mesure dans A; on supprime souvent la mention de A lorsque $A = X$.

Supposons F séparé; alors, pour tout ensemble $\mu$-intégrable $B \subset A$, l’intersection des entourages $W(V, B, \delta)$, où V parcourt un système fondamental d’entourages de F et $\delta$ parcourt l’ensemble des nombres > 0, est l’ensemble des couples $(f, g)$ tels que $f(x) = g(x)$ presque partout (pour $\mu$) dans B. En effet, l’ensemble M des $x \in B$ tels que $f(x) \neq g(x)$ est $\mu$-intégrable, puisque c’est l’image réciproque par l’application $\mu$-mesurable $x \mapsto (f(x), g(x))$ du complémentaire de la diagonale dans $F \times F$, qui est ouvert (n° 5, prop. 7); si $|\mu|(M) = \alpha > 0$, il existe une partie compacte $K \subset M$ telle que $|\mu|(M - K) < \alpha/2$ et que les restrictions de $f$ et $g$ à $K$ soient continues; il y a donc un entourage $V_0$ de $F$ tel que $(f(x), g(x)) \notin V_0$ pour tout $x \in K$, et par suite, on a $(f, g) \notin W(V_0, B, \alpha/2)$.

On en conclut que, lorsque $F$ est séparé, l’intersection de tous les entourages de $\mathscr{S}(A, \mu; F)$ est l’ensemble des couples $(f, g)$ tels que $f(x) = g(x)$ localement presque partout dans $A$. L’espace uniforme séparé associé à $\mathscr{S}(A, \mu; F)$, que nous noterons $S(A, \mu; F)$ ou $S_F(A, \mu)$ (ou même $S_F(\mu)$ ou $S_F$ lorsque $A = X$) est donc formé des classes d’équivalence pour la relation «$f(x) = g(x)$ localement presque partout dans $A$ » dans l’ensemble $\mathscr{S}(A, \mu; F)$.

#### Proposition 17 {#int-iv-s5-prop-17 .statement}

Soit $(A_\lambda)_{\lambda \in L}$ une famille localement dénombrable de parties $\mu$-mesurables de $A$, deux à deux disjointes et telles que $A - \bigcup_{\lambda \in L} A_\lambda$ soit localement $\mu$-négligeable. Alors, si, pour toute classe $f \in S(A, \mu; F)$, et tout $\lambda \in L$, $f_\lambda$ désigne la classe de la restriction à $A_\lambda$ de l’une quelconque des fonctions de la classe $f$, l’application $\psi : f \mapsto (f_\lambda)_{\lambda \in L}$ est un isomorphisme de l’espace uniforme $S(A, \mu; F)$ sur l’espace uniforme produit $\prod_{\lambda \in L} S(A_\lambda, \mu; F)$.

Il résulte du n° 10, prop. 16 que $\psi$ est bijective. Considérons un entourage $T$ de $S(A, \mu; F)$, image canonique d’un $W(V, B, \delta)$, où $B$ est une partie compacte de $A$; on sait que l’ensemble $J$ des $\lambda \in L$ tels que $B \cap A_\lambda \neq \varnothing$ est dénombrable (n° 9), et l’on a $|\mu|(B) = \sum_{\lambda \in J} |\mu|(B \cap A_\lambda)$; il y a donc une partie finie $H$ de $J$ telle que l’on ait
$$
\sum_{\lambda \in J - H} |\mu|(B \cap A_\lambda) \leq \frac{\delta}{2}.
$$
Ceci posé, l’image de $T$ par $\psi \times \psi$ est contenue dans l’image canonique du produit $\prod_{\lambda \in H} W(V, B \cap A_\lambda, \delta)$. D’autre part, si $m$ est le nombre des éléments de $H$, l’image de $T$ par $\psi \times \psi$ contient l’image canonique de l’entourage $\prod_{\lambda \in H} W(V, A_\lambda, \delta/2m)$, ce qui prouve la proposition.

#### Proposition 18 {#int-iv-s5-prop-18 .statement}

Si F est métrisable, et si A est réunion d’un ensemble localement μ-négligeable et d’une suite (A_n) d’ensembles μ-intégrables, l’espace S(A, μ; F) est métrisable.

Comme chaque A_n est réunion d’un ensemble négligeable et d’une suite d’ensembles compacts, on peut déjà supposer que les A_n sont compacts et deux à deux disjoints. La prop. 17 permet ensuite de supposer que A est compact. Si (V_n) est un système fondamental dénombrable d’entourages de F, il est clair que les W(V_n, K, 1/n) forment un système fondamental d’entourages de $\mathcal{S}(A, \mu; F)$ lorsque n parcourt $\mathbf{N}$, d’où la proposition.

#### Lemme 4 {#int-iv-s5-lem-4 .statement}

Soit F un espace uniforme métrisable, et soit B ⊂ A une réunion dénombrable d’ensembles μ-intégrables. Alors, pour toute suite de Cauchy (f_n) dans $\mathcal{S}(A, \mu; F)$, il existe une suite (f_{n_k}) extraite de (f_n), telle que (f_{n_k}(x)) soit une suite de Cauchy dans F pour presque tout x ∈ B.

Supposons d’abord B intégrable, et désignons par d une distance compatible avec la structure uniforme de F. Nous allons définir par récurrence une suite double (f_{mn}) de fonctions de $\mathcal{S}(A, \mu; F)$ telle que f_{0n} = f_n pour tout n, que (f_{mn})_{n ≥ 0} soit extraite de (f_{m-1,n})_{n ≥ 0} pour tout m > 0, et enfin que, pour m > 0, l’ensemble M_{mn} des x ∈ B pour lesquels d(f_{mn}(x), f_{m,n+1}(x)) > 1/2^{m+n+1} ait une mesure |μ|(M_{mn}) ≤ 1/2^{m+n+1}; la possibilité de cette définition résulte de ce que (f_n) est une suite de Cauchy dans $\mathcal{S}(A, \mu; F)$. Posons $M_m = \bigcup_{n ≥ 0} M_{mn}$; on a

$$
|\mu|(M_m) \leq \sum_{n=0}^{\infty} |\mu|(M_{mn}) \leq 1/2^m
$$

et pour tout x ∈ B − M_m, on a $d(f_{mn}(x), f_{m,n+p}(x)) \leq 1/2^{m+n+1}$ pour tout n ≥ 0 et tout p > 0; donc, la suite (f_{mn}(x))_{n ≥ 0} est une suite de Cauchy dans F. Soit alors $N = \bigcap_{m=0}^{\infty} M_m$; N est négligeable.

Posons $\varepsilon_n = f_{nn}$ pour tout n ≥ 0; pour tout m, la suite (g_n)_{n ≥ m} est extraite de la suite (f_{mn})_{n ≥ 0}; si x ∈ B − N, il y a un indice m tel que x ∉ M_n, ce qui prouve que la suite (g_n(x)) est une suite de Cauchy dans F.

Si maintenant B est réunion d’une suite (B_m) d’ensembles intégrables, on peut définir par récurrence une suite double (g_{mn}) telle que g_{0n} = f_n, que (g_{mn})_{n ≥ 0} soit une suite extraite de (g_{m-1,n})_{n ≥ 0} pour tout $m > 0$, et que la suite $(g_{mn}(x))_{n \geq 0}$ soit une suite de Cauchy dans $B_m - P_m$, où $P_m$ est négligeable. Posons $h_n = g_{nn}$ pour tout $n \geq 0$, de sorte que, pour tout $m$, la suite $(h_n)_{n \geq m}$ soit extraite de $(g_{mn})_{n \geq 0}$; la suite $(h_n(x))_{n \geq 0}$ est alors une suite de Cauchy dans $F$ pour tout $x \in B - P$, où $P = \bigcup_{m=0}^{\infty} P_m$ est négligeable.

#### Proposition 19 {#int-iv-s5-prop-19 .statement}

*Si l’espace uniforme $F$ est métrisable et complet, l’espace uniforme $S(A, \mu; F)$ est complet.*

Il existe une famille $(K_\lambda)_{\lambda \in L}$ de parties compactes de $A$, localement dénombrable, telle que les $K_\lambda$ soient deux à deux disjointes et que $A - \bigcup_\lambda K_\lambda$ soit localement négligeable (n° 9, prop. 14). En vertu de la prop. 17, $S(A, \mu; F)$ est isomorphe au produit $\prod_{\lambda \in L} S(K_\lambda, \mu; F)$; on est donc ramené à démontrer la proposition lorsque $A$ est *intégrable*; alors (prop. 18), $S(A, \mu; F)$ est métrisable, et en vertu du lemme 4, pour toute suite de Cauchy $(f_n)$ dans $\mathcal{S}(A, \mu; F)$, il y a une suite extraite $(f_{n_k})$ qui est convergente dans $A - N$, où $N$ est négligeable; la limite $f$ de $(f_{n_k})$ (prolongée de façon arbitraire à $A$ tout entier) est alors $\mu$-mesurable, et il résulte de l’extension du th. d’Egoroff mentionnée au n° 10 que la suite $(f_{n_k})$ converge *en mesure* vers $f$ dans $A$. Cela entraîne que $f$ est une valeur d’adhérence de la suite $(f_n)$ dans $\mathcal{S}(A, \mu; F)$, et comme la suite $(f_n)$ est par hypothèse une suite de Cauchy, elle converge vers $f$.

C.Q.F.D.

#### Corollaire {#int-iv-s5-n11-cor-1 .statement}

*Soit $F$ un espace uniforme métrisable.*
(i) *Toute suite* $(f_n)$ *d’éléments de* $\mathcal{S}(A, \mu; F)$ *qui converge localement presque partout vers une application* $f$ *(nécessairement $\mu$-mesurable)* *de* $A$ *dans* $F$, *converge en mesure vers* $f$ *dans* $A$.
(ii) *Soit* $(f_n)$ *une suite d’éléments de* $\mathcal{S}(A, \mu; F)$, *qui converge en mesure vers une application* $f$ *de* $A$ *dans* $F$. *Pour tout ensemble* $B \subset A$ *réunion dénombrable d’ensembles intégrables*, *il existe une suite* $(f_{n_k})$ *extraite de* $(f_n)$ *telle que la suite* $(f_{n_k}(x))$ *converge dans* $F$ *vers* $f(x)$ *pour presque tout* $x \in B$.

(i) L’assertion résulte aussitôt de l’extension du th. d’Egoroff mentionnée au n° 10.
(ii) En vertu du lemme 4, il existe une suite $(f_{n_k})$ extraite de $(f_n)$ telle que $(f_{n_k}(x))$ soit une suite de Cauchy dans $F$ pour tout x ∈ B − N, où N est négligeable ; soit f′(x) ∈ $\hat{F}$ la limite de cette suite pour x ∈ B − N. Il est clair que f′ est une application μ-mesurable de B − N dans $\hat{F}$, et la suite (f_n) converge en mesure vers f′ dans B − N, en vertu de (i); f′ est par suite égale à f presque partout dans B.

#### Proposition 20 {#int-iv-s5-prop-20 .statement}

Soit F un espace de Banach, muni de la structure uniforme définie par sa norme.

(i) Pour toute partie μ-mesurable A de X, la topologie de la convergence en mesure est compatible avec la structure d’espace vectoriel de $\mathcal{S}(A, \mu; F)$.

(ii) L’espace $\mathcal{K}(X; F)$ est partout dense dans $\mathcal{S}(X, \mu; F)$.

(iii) Pour tout nombre réel fini p ≥ 1, la topologie induite par la topologie de la convergence en mesure sur l’espace $\mathcal{L}_F^p(X, \mu)$ est moins fine que la topologie de la convergence en moyenne d’ordre p.

(i) Pour toute partie μ-intégrable B de A et tout δ > 0, désignons par $T(B, \delta)$ l’ensemble des $f \in \mathcal{S}(A, \mu; F)$ tels que l’ensemble C des $x \in B$ tels que $|f(x)| \geq \delta$ vérifie la relation $|\mu|(C) \leq \delta$; il est clair que si $V_\delta$ est l’entourage de F formé des couples (y, z) tels que $|y - z| \leq \delta$, l’entourage $W(V_\delta, B, \delta)$ est l’ensemble des couples (f, g) d’applications mesurables de A dans F telles que $f - g \in T(B, \delta)$. Il est clair que les ensembles $T(B, \delta)$ sont symétriques, et que l’on a $T(B, \delta) + T(B, \delta) \subset T(B, 2\delta)$ et $T(B, \alpha \delta) \subset \alpha T(B, \delta)$ pour tout scalaire $\alpha$ tel que $|\alpha| \leq 1$; il suffit donc de vérifier que les ensembles $T(B, \delta)$ sont absorbants (Esp. vect. top., 2e éd., chap. I, § 1, n° 5, prop. 4). Or, si f est une application μ-mesurable de A dans F, la fonction numérique $|f|$ est aussi μ-mesurable (n° 3, cor. 6 du th. 1). Soit $C_n$ l’ensemble des $x \in B$ tels que $|f(x)| \geq n$; les $C_n$ forment une suite décroissante d’ensembles intégrables dont l’intersection est vide; donc il existe un entier n tel que $|\mu|(C_n) \leq \delta$ (§ 4, n° 5, cor. de la prop. 7); on peut en outre supposer n pris assez grand pour que $1/n \leq \delta$; alors on a $f/n^2 \in T(B, \delta)$, ce qui achève de prouver l’assertion (i).

(iii) La relation $\int |f|^p d|\mu| \leq \delta^{p+1}$ entraîne que si C est l’ensemble des $x \in X$ tels que $|f(x)| \geq \delta$, on a

$$
\delta^p |\mu|^*(C) \leq \int |f|^p d|\mu| \leq \delta^{p+1}
$$

d’où $|\mu|^*(C) \leq \delta$, ce qui démontre (iii).

(ii) En vertu de (iii), il suffit de montrer par exemple que $\mathcal{L}_F^1$ est partout dense dans $\mathcal{S}_F$, puisque par définition $\mathcal{K}(X; F)$ est dense dans $\mathcal{L}_F^1$ pour la topologie de la convergence en moyenne. Or, soient $f$ un élément quelconque de $\mathcal{S}_F$, et $T(B, \delta)$ un voisinage de 0 dans cet espace ; on voit comme dans (i) qu’il existe une partie intégrable $C$ de $B$ telle que $|\mu|(C) \leq \delta$ et que $f$ soit *bornée* dans $B - C$; désignant alors par $g$ la fonction égale à $f$ dans $B - C$, à 0 dans $X - (B - C)$, il résulte du n° 6, th. 5 que $g$ est intégrable, et l’on a évidemment $f - g \in T(B, \delta)$.

*Remarques.* 1) L’espace vectoriel topologique $\mathcal{S}(X, \mu; F)$ n’est pas nécessairement localement convexe (exerc. 24).
2) La topologie induite par la topologie de la convergence en mesure sur l’ensemble des $f$ telles que $N_p(f) \leq 1$ peut être strictement moins fine que la topologie induite sur cet ensemble par la topologie de la convergence en moyenne d’ordre $p$ (exerc. 22). Voir toutefois la prop. 21 ci-dessous.

#### Définition 10 {#int-iv-s5-def-10 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$, $F$ un espace de Banach, et $p \in [1, +\infty[$. Une partie $H$ de $\mathcal{L}_F^p(X, \mu)$ est dite équiintégrable d’ordre $p$ (pour $\mu$) si elle satisfait aux conditions suivantes :
(i) Pour tout $\varepsilon > 0$, il existe $\delta > 0$ tel que, pour tout ensemble intégrable $A$ de mesure $|\mu|(A) \leq \delta$ et pour toute $f \in H$, on ait
$$
\int |f|^p \varphi_A d|\mu| \leq \varepsilon.
$$
(ii) Pour tout $\varepsilon > 0$, il existe une partie compacte $K$ de $X$ telle que, pour toute $f \in H$, on ait $\int |f|^p \varphi_{X-K} d|\mu| \leq \varepsilon$.

Si $p = 1$, on dit « équiintégrable » au lieu de « équiintégrable d’ordre $p$ ».

#### Remarque {#int-iv-s5-n11-rem-1 .statement}

Supposons $\mu$ bornée. Pour tout $a > 0$, l’ensemble des applications mesurables de $X$ dans $F$ telles que $|f(x)| \leq a$ presque partout est équiintégrable d’ordre $p$, et ceci quel que soit $p \in [1, +\infty[$.

#### Proposition 21 {#int-iv-s5-prop-21 .statement}

Soit $H$ une partie de $\mathcal{L}_F^p(X, \mu)$ équiintégrable d’ordre $p$. Sur $H$, la structure uniforme de la convergence en mesure est égale à la structure uniforme induite par celle de $\mathcal{L}_F^p(X, \mu)$.

Soit $\varepsilon > 0$. Il existe $\delta$ et $K$ avec les propriétés (i) et (ii) de la déf. 10. Soient $f, g$ dans $H$ telles que

$$
|f(x) - g(x)| \leq \left( \frac{\varepsilon}{|\mu|(K)} \right)^{1/p}
$$

pour $x \in K$, sauf sur un ensemble $M$ de mesure $\leq \delta$. On a

$$
\left( \int_{X-K} |f-g|^p d|\mu| \right)^{1/p} \leq \left( \int_{X-K} |f|^p d|\mu| \right)^{1/p} + \left( \int_{X-K} |g|^p d|\mu| \right)^{1/p}
$$
$$
\leq 2\varepsilon^{1/p}
$$

et de même

$$
\left( \int_M |f-g|^p d|\mu| \right)^{1/p} \leq 2\varepsilon^{1/p}
$$

donc

$$
\int |f-g|^p d|\mu| = \int_{X-K} |f-g|^p d|\mu| + \int_M |f-g|^p d|\mu|
$$
$$
+ \int_{K-M} |f-g|^p d|\mu|
$$
$$
\leq 2^p \varepsilon + 2^p \varepsilon + \frac{\varepsilon}{|\mu|(K)} |\mu|(K-M) \leq (2^{p+1} + 1)\varepsilon.
$$

Donc la structure uniforme de la convergence en mesure sur $H$ est plus fine que la structure uniforme induite par celle de $\mathcal{L}_F^p(X, \mu)$. Il suffit alors d’appliquer la prop. 20.

### 12. Une propriété de la convergence vague

#### Lemme 5 {#int-iv-s5-lem-5 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure positive bornée sur $X$, $F$ un espace de Banach, $f$ une fonction bornée sur $X$ à valeurs dans $F$. Les conditions suivantes sont équivalentes:

(i) L’ensemble des points de discontinuité de $f$ est $\mu$-négligeable.

(ii) Pour tout $\varepsilon > 0$, il existe des éléments $a_1, \ldots, a_n$ de $F$, des fonctions $g_1, \ldots, g_n$ appartenant à $\mathscr{H}(X)$, et une fonction $h \geq 0$ continue bornée sur $X$, tels que $|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|$ partout sur $X$, et $\int h \, d\mu \leq \varepsilon$.

Nous noterons N l’ensemble des points de discontinuité de f, et nous poserons M = sup |f|.

(i) ⇒ (ii). Supposons la condition (i) satisfaite. Soit ε > 0. La fonction f est μ-intégrable (n° 2, cor. 4 de la prop. 5 et n° 6, th. 5), donc il existe a_1, ..., a_n dans F, g_1, ..., g_n dans $\mathscr{K}(X)$ tels que, posant $k = |f - g_1 a_1 - ... - g_n a_n|$, on ait $\int k\ d\mu \leq \varepsilon/2$ (§ 3, n° 5, prop. 10). En multipliant g_1, ..., g_n par un même élément convenable de $\mathscr{K}(X)$, on peut en outre supposer que
$$
|g_1 a_1 + ... + g_n a_n| \leq |f|
$$
sur X, d’où $k \leq 2M$. L’ensemble N’ des points de discontinuité de k est contenu dans N, donc est négligeable. Pour tout $x \in X$, posons $l(x) = \limsup_{y \to x} k(y)$. On a $2M \geq l \geq k$ sur X, et $l = k$ sur $X - N'$, c’est-à-dire presque partout pour $\mu$, donc $\int l\ d\mu \leq \varepsilon/2$. D’autre part, l est bornée et semi-continue supérieurement, donc enveloppe inférieure de l’ensemble des fonctions continues bornées majorant l. Il existe donc une fonction continue bornée h $\geq l$ sur X telle que $h \leq 2M$ et $\int h\ d\mu \leq \int l\ d\mu + \varepsilon/2$ (§ 4, n° 4, cor. 2 de la prop. 5). On a alors $\int h\ d\mu \leq \varepsilon$, et $|f - g_1 a_1 - ... - g_n a_n| \leq h$.

(ii) ⇒ (i). Supposons la condition (ii) satisfaite. Pour tout $x \in X$, soit $\omega(x)$ l’oscillation de f en x. Soit $\varepsilon > 0$. Il existe a_1, ..., a_n, g_1, ..., g_n, h avec les propriétés de (ii). Pour tout $x \in X$, $\omega(x)$ est l’oscillation de $f - g_1 a_1 - ... - g_n a_n$ en x, donc $\omega(x) \leq 2h(x)$. Donc $\int \omega\ d\mu \leq 2\varepsilon$. Par suite, l’ensemble $A_\varepsilon$ des $x \in X$ tels que $\omega(x) \geq \sqrt{\varepsilon}$ est tel que $\mu(A_\varepsilon) \leq 2\sqrt{\varepsilon}$. Ceci prouve que $\mu(N) \leq 2\sqrt{\varepsilon}$, d’où $\mu(N) = 0$.

#### Proposition 22 {#int-iv-s5-prop-22 .statement}

Soient F un espace de Banach, X un espace localement compact, $\mathscr{E}$ l’ensemble des mesures positives bornées sur X, $\mu$ un élément de $\mathscr{E}$, $\mathcal{B}$ une base de filtre sur $\mathscr{E}$. On suppose que $\mathcal{B}$ converge vaguement vers $\mu$ et que $\|v\|$ tend vers $\|\mu\|$ suivant $\mathcal{B}$. Soit f une application de X dans F vérifiant les conditions suivantes:
(i) f est bornée, intégrable pour $\mu$ et pour toute mesure appartenant à un élément de $\mathcal{B}$;
(ii) l’ensemble des points de discontinuité de f est $\mu$-négligeable.

Alors $\int f\ dv$ tend vers $\int f\ d\mu$ suivant $\mathcal{B}$.

Soit $\varepsilon > 0$. Il existe des éléments a_1, ..., a_n de F, des fonctions g_1, ..., g_n de $\mathscr{K}(X)$, et une fonction h $\geq 0$ continue bornée sur X, tels que $|f - g_1 a_1 - ... - g_n a_n| \leq h \leq 2 \sup |f|$ sur X et $\int h\ d\mu \leq \varepsilon$ (lemme 5). Soit M = sup|f|. Il existe une partie compacte K de X telle que $\mu^*(X - K) \leq \varepsilon$ (§ 4, n° 7, prop. 12, et n° 6, th. 4), un voisinage compact K' de K dans X, et une application continue h' de X dans [0, 2M] tels que h' = h sur K, h' = 2M sur X - K'; en remplaçant h par sup(h, h'), on peut supposer en outre que h' majore h. On a $\int (h' - h) d\mu \leq 2M \mu^*(X - K) \leq 2M \varepsilon$. D’autre part, $h' = h_1 + 2M$, où $h_1 \in \mathcal{K}(X)$. Compte tenu du § 4, n° 7, prop. 12, le nombre $\int h' dv = \int h_1 dv + 2M \|v\|$ tend suivant $\mathcal{B}$ vers

$$
\int h_1 d\mu + 2M \|\mu\| = \int h' d\mu.
$$

Il existe alors un $A \in \mathcal{B}$ tel que, pour toute $v \in A$, on ait

$$
\left| \int (g_1 a_1 + \ldots + g_n a_n) dv - \int (g_1 a_1 + \ldots + g_n a_n) d\mu \right| \leq \varepsilon,
$$
$$
\int h dv \leq \int h' dv \leq \int h' d\mu + \varepsilon \leq \int h d\mu + 2M \varepsilon + \varepsilon \leq 2(M + 1)\varepsilon.
$$

Ces inégalités entraînent

$$
\left| \int f dv - \int f d\mu \right| \leq
$$
$$
\int h dv + \left| \int (g_1 a_1 + \ldots + g_n a_n) dv - \int (g_1 a_1 + \ldots + g_n a_n) d\mu \right|
$$
$$
+ \int h d\mu \leq 2(M + 2)\varepsilon,
$$

ce qui démontre la proposition.

#### Remarque {#int-iv-s5-n12-rem-1 .statement}

Les conditions (i) et (ii) de la proposition 22 sont satisfaites si f est continue et bornée.

#### Exemple {#int-iv-s5-n12-exa-1 .statement}

Prenons pour X l’espace compact U des nombres complexes de valeur absolue 1. En posant, pour toute $f \in \mathcal{K}(U)$,
$$
\mu(f) = \int_0^1 f(e^{2i\pi t}) dt,
$$
on définit une mesure positive de masse 1 sur X. D’autre part, soit $\theta$ un nombre réel ; pour tout entier $n \geq 0$, soient $v_n$ la masse unité placée au point $e^{2i\pi n \theta}$ de U, et
$$
\mu_n = \frac{1}{n+1} (v_0 + \ldots + v_n),
$$
de sorte que $\mu_n$ est une mesure positive de masse 1 sur U. Alors, si $\theta$ est irrationnel, $\mu_n$ tend vaguement vers $\mu$. En effet, comme les combinaisons linéaires des fonctions $z \mapsto z^k$ ($k \in \mathbf{Z}$) sont partout denses dans $\mathcal{K}(U)$ (Top. gén., chap. X, 2e éd., § 4, n° 4, prop. 8), il suffit de prouver que $\mu_n(z^k)$ tend vers $\mu(z^k)$ pour $k \in \mathbf{Z}$. Or, pour $k = 0$, on a $\mu_n(z^k) = \mu(z^k) = 1$; pour $k \neq 0$, on a
$$
\mu_n(z^k) = \frac{1}{n+1}(1 + e^{2i\pi k\theta} + e^{4i\pi k\theta} + \ldots + e^{2i\pi kn\theta}).
$$
Comme $e^{2i\pi k\theta} \neq 1$ (puisque $\theta$ est irrationnel), on en déduit
$$
|\mu_n(z^k)| = \left| \frac{1}{n+1} \frac{e^{2i\pi k(n+1)\theta} - 1}{e^{2i\pi k\theta} - 1} \right| \leq \frac{1}{n+1} \frac{2}{|e^{2i\pi k\theta} - 1|},
$$
donc $\mu_n(z^k)$ tend vers $0 = \mu(z^k)$. Dans ces conditions, on peut appliquer la proposition 22, et on voit en particulier que, si $A$ est une partie de $U$ de frontière négligeable pour $\mu$, $\mu_n(A)$ tend vers $\mu(A)$. Autrement dit, si $p_n$ désigne le nombre d’entiers $k \in \{0, n\}$ tels que $e^{2i\pi k\theta} \in A$, $n^{-1} p_n$ tend vers $\mu(A)$ quand $n$ tend vers $+\infty$.

## EXERCICES {#int-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
