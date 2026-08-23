---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 3
section_title: Intégration de mesures positives
lang: fr
source: int-v-fr
pdf_pages: 0021-0039, 0109-0112
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions à valeurs dans un espace de mesures
      page: 0
      pdf_page: 21
    - "no": 2
      title: Intégrales superposées de fonctions positives
      page: 0
      pdf_page: 26
    - "no": 3
      title: Intégrales superposées de fonctions à valeurs dans un espace de Banach
      page: 0
      pdf_page: 30
    - "no": 4
      title: Fonctions universellement mesurables
      page: 0
      pdf_page: 33
    - "no": 5
      title: Diffusions
      page: 0
      pdf_page: 34
    - "no": 6
      title: Composition des diffusions bornées
      page: 0
      pdf_page: 37
statements: 30
exercises: 11
content_sha256: 202326f90fffa51b23c7d93972a9123ba43a5505721e85820845781a1c997c55
---

## § 3. Intégration de mesures positives

### 1. Fonctions à valeurs dans un espace de mesures

Soient $X$ un espace localement compact, $\mathcal{M}_+(X)$ le cône convexe des mesures positives sur $X$. Dans toute la suite de ce chapitre, $\mathcal{M}_+(X)$ sera muni de la topologie induite par la topologie vague sur $\mathcal{M}(X)$ (chap. III, 2e éd., § 1, n° 9); dire qu’une application $\Lambda : t \mapsto \lambda_t$ de l’espace localement compact $T$ dans $\mathcal{M}_+(X)$ est continue signifie donc que, pour toute fonction $f \in \mathcal{K}(X)$, la

Soit $ \Lambda : t \mapsto \lambda_t $ une application de T dans $ \mathcal{M}_+(X) $; nous dirons que $ \Lambda $ est *scalairement essentiellement intégrable* pour la mesure $ \mu $ si, pour toute fonction $ f \in \mathscr{K}(X) $, la fonction $ t \mapsto \lambda_t(f) $ est essentiellement $ \mu $-intégrable. Si l’on pose $ v(f) = \int \lambda_t(f)\ d\mu(t) $, il est clair que $ v $ est une forme linéaire positive sur $ \mathscr{K}(X) $, et par suite (chap. III, 2e éd., § 1, n° 6, th. 1) une mesure sur X. Nous dirons que $ v $ est l’intégrale de la fonction $ \Lambda $ à valeurs dans $ \mathcal{M}_+(X) $, et nous écrirons $ v = \int \lambda_t\ d\mu(t) $.

La définition précédente est un cas particulier de la notion d’intégrale faible, qui sera traitée de façon générale au chap. VI.

Si $ f $ désigne un élément de $ \mathscr{K}(X) $, l’intégrale $ \int \lambda_t(f)\ d\mu(t) $ sera aussi notée, par abus de notation, $ \int d\mu(t) \int f(x)\ d\lambda_t(x) $; la définition de l’intégrale $ v = \int \lambda_t\ d\mu(t) $ s’écrit alors :

(1)
$$
\int f(x)\ dv(x) = \int d\mu(t) \int f(x)\ d\lambda_t(x).
$$

Nous ferons des abus de notation analogues dans la suite, pour les intégrales supérieures, les intégrales supérieures essentielles, les intégrales de fonctions à valeurs dans un espace de Banach.

#### Exemple 1 {#int-v-s3-n1-exa-1 .statement}

Supposons que T soit un espace discret, et que $ \mu $ soit la mesure sur T définie par la masse +1 placée en chaque point de T (chap. III, 2e éd., § 1, n° 3). Soit $ h $ une fonction $ \geqslant 0 $ définie dans T : la fonction $ h $ étant semi-continue inférieurement (et même continue) dans T, on a $ \mu^*(h) = \mu^*(h) = \sum_{t \in T} h(t) $ (chap. IV, § 1, n° 1, *Exemple*). Pour la mesure $ \mu $, les notions de fonction intégrable et de fonction essentiellement intégrable sont donc identiques. Cela étant, dire qu’une application $ t \mapsto \lambda_t $ de T dans $ \mathcal{M}_+(X) $ est scalairement essentiellement $ \mu $-intégrable revient à dire que la famille $ (\lambda_t)_{t \in T} $ est sommable (§ 2, n° 1), et on a alors $ \int \lambda_t\ d\mu(t) = \sum_{t \in T} \lambda_t $. On notera que l’application $ t \mapsto \lambda_t $ est vaguement continue.

#### Exemple 2 {#int-v-s3-n1-exa-2 .statement}

L’application $ t \mapsto \varepsilon_t $ de T dans $ \mathcal{M}_+(T) $ est vaguement continue, scalairement essentiellement $ \mu $-intégrable pour toute mesure positive $ \mu $ sur T, et on a $ \int \varepsilon_t\ d\mu(t) = \mu $.

#### Proposition 1 {#int-v-s3-prop-1 .statement}

Supposons que $ \mu $ soit la borne supérieure d’une famille filtrante croissante $ (\mu_i)_{i \in I} $ de mesures positives sur $ T $; pour que $ \Lambda : t \mapsto \lambda_t $ soit scalairement essentiellement $ \mu $-intégrable, il faut et il suffit que $ \Lambda $ soit scalairement essentiellement $ \mu_i $-intégrable pour tout $ i \in I $, et que la famille $ (\int \lambda_t \, d\mu_i(t))_{i \in I} $ soit majorée dans $ \mathcal{M}(X) $. On a dans ce cas
$$
\int \lambda_t \, d\mu(t) = \sup_{i \in I} \int \lambda_t \, d\mu_i(t).
$$
En effet, vérifier que $ \Lambda $ est scalairement essentiellement intégrable pour une mesure positive $ \eta $ sur $ T $ revient à vérifier que $ t \mapsto \lambda_t(g) $ est $ \eta $-mesurable et admet une intégrable supérieure essentielle finie par rapport à $ \eta $, quelle que soit la fonction $ g \in \mathscr{K}_+(X) $. La proposition résulte donc aussitôt de la prop. 11 du § 1, n° 4 et de son corollaire 2.

#### Corollaire {#int-v-s3-n1-cor-1 .statement}

Supposons que $ \mu $ soit la somme d’une famille sommable $ (\mu_\alpha)_{\alpha \in A} $ de mesures positives sur $ T $; pour que $ \Lambda : t \mapsto \lambda_t $ soit scalairement essentiellement $ \mu $-intégrable, il faut et il suffit que $ \Lambda $ soit scalairement essentiellement $ \mu_\alpha $-intégrable pour $ \alpha \in A $, et que la famille des mesures $ \int \lambda_t \, d\mu_\alpha(t) $ soit sommable. On a alors
$$
\int \lambda_t \, d\mu(t) = \sum_{\alpha \in A} \int \lambda_t \, d\mu_\alpha(t).
$$
Il en résulte immédiatement que toute application scalairement essentiellement $ \mu $-intégrable est aussi scalairement essentiellement $ \mu' $-intégrable pour toute mesure $ \mu' \leq \mu $.

Nous nous bornerons dans ce paragraphe à l’étude des applications scalairement essentiellement intégrables de $ T $ dans $ \mathcal{M}_+(X) $ qui possèdent la propriété envisagée dans la définition suivante.

#### Définition 1 {#int-v-s3-def-1 .statement}

Soient $ X $ un espace localement compact, $ \Lambda : t \mapsto \lambda_t $ une application scalairement essentiellement $ \mu $-intégrable de $ T $ dans $ \mathcal{M}_+(X) $, et $ v $ l’intégrale de $ \Lambda $.
On dit que $ \Lambda $ est $ \mu $-pré-adéquate si, pour toute fonction semi-continue inférieurement $ f \geq 0 $ définie dans $ X $, la fonction $ t \mapsto \int^\cdot f \, d\lambda_t $ est $ \mu $-mesurable dans $ T $, et si l’on a
$$
\int^\cdot f(x) \, dv(x) = \int^\cdot d\mu(t) \int^\cdot f(x) \, d\lambda_t(x).
$$

On dit que $ \Lambda $ est $ \mu $-adéquate* si $ \Lambda $ est $ \mu' $-pré-adéquate pour toute mesure positive $ \mu' \leq \mu $.

On peut montrer que si $ \Lambda $ est $ \mu $-pré-adéquate, et si la mesure $ \nu $ est modérée — en particulier si $ X $ est dénombrable à l’infini — alors $ \Lambda $ est $ \mu $-adéquate (exerc. 7); mais on ignore si ces notions sont équivalentes en général. Dans les énoncés des n°s 2 et 3 ci-dessous, les assertions précédées d’un a) ou d’un b) s’étendent aussitôt aux applications pré-adéquates, tandis que celles qui sont précédées d’un c) valent seulement pour les applications adéquates.

La proposition suivante permet souvent de vérifier qu’une application donnée est $ \mu $-adéquate.

#### Proposition 2 {#int-v-s3-prop-2 .statement}

Soit $ \Lambda : t \mapsto \lambda_t $ une application scalairement essentiellement intégrable de $ T $ dans $ \mathcal{M}_+(X) $, et soit $ \nu = \int \lambda_t \, d\mu(t) $.

a) Si $ \Lambda $ est vaguement continue, l’application $ t \mapsto \lambda_t^\bullet(f) $ est semi-continue inférieurement pour toute fonction semi-continue inférieurement $ f \geq 0 $ définie dans $ X $, $ \Lambda $ est $ \mu $-adéquate, et on a la relation
$$
\int^* f(x) \, d\nu(x) = \int^* d\mu(x) \int^* f(x) \, d\lambda_t(x).
$$
(5)

b) Si $ \Lambda $ est vaguement $ \mu $-mesurable, $ \Lambda $ est $ \mu $-adéquate.

c) Si la topologie de $ X $ admet une base dénombrable, $ \Lambda $ est vaguement mesurable (et donc aussi $ \mu $-adéquate).

Soit $ f $ une fonction semi-continue inférieurement $ \geq 0 $ définie dans $ X $. Soit $ F $ l’ensemble, filtrant pour la relation $ \leq $, des fonctions $ g \in \mathscr{H}(X) $ telles que $ 0 \leq g \leq f $. Pour $ g \in F $, notons $ h_g $ la fonction définie dans $ T $ par $ h_g(t) = \lambda_t(g) $. Posons de même
$$
h_f(t) = \lambda_t^*(f) = \lambda_t^\bullet(f) = \sup_{g \in F} h_g(t)
$$
(\S 1, n° 1, prop. 4). Faisons l’hypothèse suivante, plus faible que celle de a): supposons seulement que la restriction de $ \Lambda $ à $ S $ soit vaguement continue, $ S $ étant un fermé de $ T $ contenant le support de $ \mu $. Pour $ g \in F $, notons $ \bar{h}_g $ la fonction numérique qui coïncide avec $ h_g $ dans $ S $ et qui vaut $ +\infty $ dans $ \mathbf{C}S $. Posons $ \bar{h}_f = \sup_{g \in F} \bar{h}_g $; on a $ \bar{h}_f = h_f $ dans $ S $. Pour toute $ g \in F $ la fonction $ \bar{h}_g $ est semi-continue inférieurement; $ \bar{h}_f $ est donc semi-continue inférieurement

\* Dans la 1re édition, on appelait applications $ \mu $-adéquates les applications scalairement $ \mu $-intégrables et vaguement $ \mu $-mesurables. La définition qui est donnée ici est plus générale (prop. 2).

et on a, la famille $(\bar{h}_g)_{g \in F}$ étant filtrante

$$
\mu^*(\bar{h}_f) = \sup_{g \in F} \mu^*(\bar{h}_g) = \sup_{g \in F} \mu^*(h_g) = \sup_{g \in F} v(g) = v^*(f)
$$

(chap. IV, § 1, n° 1, th. 1 et § 2, n° 3, prop. 6). Comme $h_f = \bar{h}_f$ dans S, donc presque partout, ceci s’écrit aussi $\mu^*(h_f) = v^*(f)$, égalité identique à (5). De même, $f$ et $\bar{h}_f$ étant semi-continues inférieurement, les relations précédentes donnent l’égalité $\mu^*(\bar{h}_f) = v^*(f)$ (§ 1, n° 1, prop. 4); comme $\bar{h}_f = h_f$ sur S, il vient $\mu^*(h_f) = v^*(f)$ (§ 1, n° 1, prop. 1), égalité identique à (4). L’application $\Lambda$ est donc $\mu$-pré-adéquate; mais on aurait pu remplacer partout dans ce raisonnement $\mu$ par $\mu' \leq \mu$, $v$ par $v' = \int \lambda_t d\mu'(t)$, car $\Lambda$ est aussi scalairement essentiellement $\mu'$-intégrable, et S contient le support de $\mu'$. Il en résulte que $\Lambda$ est $\mu$-adéquate.

Supposons $\Lambda$ vaguement continue; on peut prendre $S = T$; alors $h_f = \bar{h}_f$ est semi-continue inférieurement, ce qui achève de prouver la partie a) de l’énoncé.

Supposons $\Lambda$ vaguement $\mu$-mesurable, et démontrons b). L’ensemble $\mathcal{K}$ des compacts K de T tels que la restriction de $\Lambda$ à K soit continue étant $\mu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15), il existe une famille sommable $(\mu_\alpha)_{\alpha \in A}$ de mesures sur T, telle qu’on ait $\mu = \sum_{\alpha \in A} \mu_\alpha$ et que le support $S_\alpha$ de chacune des mesures $\mu_\alpha$ appartienne à $\mathcal{K}$ (§ 2, n° 3, prop. 4). Pour tout $\alpha \in A$, l’application $\Lambda$ est scalairement essentiellement $\mu_\alpha$-intégrable, et nous poserons $v_\alpha = \int \lambda_t d\mu_\alpha(t)$; la famille $(v_\alpha)$ est sommable, et sa somme est égale à $v$ (cor. de la prop. 1). Si $f$ est une fonction semi-continue inférieurement positive définie sur X, la première partie de la démonstration appliquée aux mesures $\mu_\alpha$ et aux fermés $S_\alpha$ montre:

1° que $h_f$ est $\mu_\alpha$-mesurable pour tout $\alpha \in A$, donc $\mu$-mesurable (§ 2, n° 2, prop. 2);
2° que l’on a:

$$
\int f(x) dv_\alpha(x) = \int d\mu_\alpha(t) \int f(x) d\lambda_t(x).
$$

La formule (4) s’en déduit en sommant sur $\alpha$ (§ 2, n° 2, prop. 1). En appliquant le raisonnement précédent à une mesure $\mu'$ quelconque majorée par $\mu$ (ce qui est légitime, car $\Lambda$ est scalairement essentiellement $\mu'$-intégrable et vaguement $\mu'$-mesurable, cf. § 2, n° 2, prop. 2), on constate que $\Lambda$ est $\mu$-adéquate, et b) est démontrée.

Enfin, supposons que la topologie de X admette une base dénombrable, et montrons que toute application scalairement essentiellement $ \mu $-intégrable $ \Lambda : t \mapsto \lambda_t $ de $ T $ dans $ \mathcal{M}_+(X) $ est vaguement $ \mu $-mesurable. Cela résultera du lemme suivant:

#### Lemme 1 {#int-v-s3-lem-1 .statement}

*Soit X un espace localement compact ayant une base dénombrable. Il existe alors dans $ \mathscr{K}(X) $ une partie dénombrable S possédant la propriété suivante: pour toute fonction $ f \in \mathscr{K}(X) $, il existe une suite $ (f_n) $ d’éléments de S, une fonction positive $ \varphi \in S $, telles que, quel que soit le nombre $ \varepsilon > 0 $, l’on ait $ |f_n - f| \leq \varepsilon \varphi $ dès que n est suffisamment grand.*

Soit $ X' $ le compactifié d’Alexandroff de X, qui est un compact métrisable (*Top. gén.*, chap. IX, n° 9, prop. 16 et cor.); nous identifierons $ \mathscr{K}(X) $ à une partie de $ \mathscr{C}(X') $. Soit $ S' $ une partie dénombrable dense de l’espace de Banach $ \mathscr{C}(X') $ (*Top. gén.*, chap. X, 2e éd., § 3, th. 1); on peut supposer que $ S' $ contient la fonction constante $ n $ pour tout $ n \in \mathbf{N} $. Soit $ (U_n) $ une suite d’ouverts relativement compacts de X, de réunion X; tels que $ \overline{U}_n \subset U_{n+1} $ pour tout $ n $ (*Top. gén.*, chap. I, 4e éd., § 9, prop. 15), et soit $ \varphi_n $ une fonction de $ \mathscr{K}_+(X) $ égale à 1 sur $ \overline{U}_n $. Nous désignerons par S l’ensemble dénombrable des éléments de $ \mathscr{K}(X) $ de la forme $ \varphi_n g $ ($ n \in \mathbf{N} $, $ g \in S' $). Si $ f \in \mathscr{K}(X) $, soit $ (g_n) $ une suite d’éléments de S’ qui converge uniformément vers $ f $, et soit $ k $ un entier tel que le support de $ f $ soit contenu dans $ U_k $. Soit enfin $ m $ un entier qui majore les normes des fonctions $ g_n $. Les fonctions $ f_n = \varphi_k g_n $ appartiennent à S, et satisfont à l’énoncé, avec $ \varphi = m \varphi_k $.

Ce lemme étant établi, et l’application $ t \mapsto \lambda_t(g) $ étant scalairement essentiellement intégrable pour tout $ g \in S $, l’application $ t \mapsto (\lambda_t(g))_{g \in S} $ de T dans $ \mathbf{R}^S $ est $ \mu $-mesurable (chap. IV, § 5, n° 3, th. 1). L’ensemble $ \mathfrak{R} $ des compacts K de T tels que la restriction de cette application à K soit continue est donc $ \mu $-dense, et il nous suffira de montrer que la restriction de $ \Lambda $ à tout $ K \in \mathfrak{R} $ est continue. Or soient $ f $ un élément quelconque de $ \mathscr{K}(X) $, $ f_n $ et $ \varphi $ des éléments de S satisfaisant à l’énoncé du lemme 1; la fonction $ t \mapsto \lambda_t(f) $ est alors limite uniforme dans K des fonctions continues $ t \mapsto \lambda_t(f_n) $; elle est donc continue dans K, et la proposition est démontrée.

### 2. Intégrales superposées de fonctions positives

Dans toute la suite de ce paragraphe, sauf mention expresse du contraire, nous désignons par X un espace localement compact, par $ \Lambda : t \mapsto \lambda_t $ une application $ \mu $-adéquate de T dans $ \mathcal{M}_+(X) $, et par $ v $ l’intégrale de $ \Lambda $.

#### Proposition 3 {#int-v-s3-prop-3 .statement}

Soit $ f $ une fonction numérique $ \geqslant 0 $ définie dans $ X $.

a) *On a l’inégalité*

(6) $ \int^* f(x)\ dv(x) \geqslant \int^\cdot d\mu(t) \int^* f(x)\ d\lambda_t(x) \geqslant \int^\cdot d\mu(t) \int^\cdot f(x)\ d\lambda_t(x). $

b) *Si $ \Lambda $ est vaguement continue, on a*

(7) $ \int^* f(x)\ dv(x) \geqslant \int^* d\mu(t) \int^* f(x)\ d\lambda_t(x). $

c) *Si l’on a $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout, on a*

(8)
$$
\int^\cdot f(x)\ dv(x) \geqslant \int^\cdot d\mu(t) \int^* f(x)\ d\lambda_t(x)
$$
$$
= \int^\cdot d\mu(t) \int^\cdot f(x)\ d\lambda_t(x).
$$

Soit $ g $ une fonction semi-continue inférieurement dans $ X $ telle que $ f \leqslant g $. Pour tout $ t \in T $, on a
$$
\int^* f(x)\ d\lambda_t(x) \leqslant \int^* g(x)\ d\lambda_t(x),
$$
donc, d’après (4) et la prop. 4 du § 1,
$$
\int^\cdot d\mu(t) \int^* f(x)\ d\lambda_t(x) \leqslant \int^\cdot d\mu(t) \int^* g(x)\ d\lambda_t(x) = \int^* g(x)\ dv(x).
$$

La première des inégalités (6) résulte alors de la définition de $ \int^* f(x)\ dv(x) $ (chap. IV, § 1, n° 3, déf. 3), et la seconde en résulte aussitôt. L’inégalité (7) se démontre de manière analogue si $ \Lambda $ est vaguement continue, en utilisant (5) au lieu de (4).

Passons à la démonstration de (8). L’application $ t \mapsto \lambda_t^*(1) $ est mesurable, finie localement $ \mu $-presque partout. L’ensemble $ \mathfrak{K} $ des compacts $ K $ de $ T $ tels que la restriction de $ t \mapsto \lambda_t^*(1) $ à $ K $ soit finie et continue est donc $ \mu $-dense, et la prop. 4 du § 2, n° 3 entraîne l’existence d’une famille sommable $ (\mu_\alpha)_{\alpha \in A} $ de mesures positives, dont les supports appartiennent à $ \mathfrak{K} $, telle que $ \mu = \sum_{\alpha \in A} \mu_\alpha $. L’application $ \Lambda $ est $ \mu_\alpha $-adéquate pour tout $ \alpha \in A $; posons $ v_\alpha = \int \lambda_t\ d\mu_\alpha(t) $. La prop. 1 montre que $ v = \sum_{\alpha \in A} v_\alpha $, et la relation (4), appliquée à la mesure $ \mu_\alpha $ et à la fonction 1, montre que $ v_\alpha $ est une mesure bornée (car $ \lambda_t^*(1) $ est borné sur $ \operatorname{Supp}(\mu_\alpha) $). Ecrivons alors la formule

$$
\int^* f(x) \, dv_\alpha(x) \geq \int^* d\mu_\alpha(t) \int^* f(x) \, d\lambda_t(x) = \int^* d\mu_\alpha(t) \int^* f(x) \, d\lambda_t(x)
$$

(la dernière égalité provient de ce que $ \lambda_t $ est bornée localement presque partout, et de la prop. 7 du § 1). L’inégalité (7) s’obtient en sommant sur $ \alpha $ (\$ 2, n° 2, prop. 1).

Si l’on ne fait aucune hypothèse analogue à celle de c), l’inégalité (8) peut être mise en défaut (exerc. 2).

#### Corollaire 1 {#int-v-s3-prop-3-cor-1 .statement}

Soit $ f $ une fonction $ \geq 0 $ définie dans $ X $, et soit $ H $ l’ensemble des $ t \in T $ tels que $ f $ ne soit pas $ \lambda_t $-négligeable.
a) Si $ f $ est $ v $-négligeable, $ H $ est localement $ \mu $-négligeable.
b) Si $ f $ est $ v $-négligeable, et si $ \Lambda $ est vaguement continue, $ H $ est $ \mu $-négligeable.
c) Si $ f $ est localement $ v $-négligeable, et si $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout, $ H $ est localement $ \mu $-négligeable.

#### Corollaire 2 {#int-v-s3-prop-3-cor-2 .statement}

Soit $ f $ une fonction $ \geq 0 $ définie dans $ X $ et $ v $-modérée. L’ensemble des $ t \in T $ tels que $ f $ ne soit pas $ \lambda_t $-modérée est alors localement $ \mu $-négligeable (et même $ \mu $-négligeable si $ \Lambda $ est vaguement continue).
En effet, $ f $ est la somme d’une suite de fonctions $ f_n \geq 0 $, telle que $ f_n $ soit nulle hors d’un compact $ K_n $ pour $ n \geq 1 $, et que $ f_0 $ soit $ v $-négligeable (\$ 1, n° 2, prop. 6); $ f_0 $ est alors $ \lambda_t $-négligeable, sauf pour des $ t $ qui forment un ensemble localement $ \mu $-négligeable (et même $ \mu $-négligeable si $ \Lambda $ est vaguement continue) d’après le cor. 1, et l’énoncé en résulte aussitôt.

#### Proposition 4 {#int-v-s3-prop-4 .statement}

Soit $ f $ une fonction $ v $-mesurable définie dans $ X $, à valeurs dans un espace topologique $ G $, et soit $ M $ l’ensemble des $ t \in T $ tels que $ f $ ne soit pas $ \lambda_t $-mesurable.
a) Supposons que $ f $ soit constante dans le complémentaire d’une partie $ v $-modérée de $ X $; $ M $ est alors localement $ \mu $-négligeable.
b) Supposons que $ f $ soit constante dans le complémentaire d’une partie $ v $-modérée de $ X $, et que $ \Lambda $ soit vaguement continue; $ M $ est alors $ \mu $-négligeable.

c) Supposons qu’on ait $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout ; M est alors localement $ \mu $-négligeable.

Démontrons d’abord a) (resp. b)). Tout ensemble $ v $-intégrable étant contenu dans un ouvert $ v $-intégrable, la fonction $ f $ est constante dans le complémentaire B d’une réunion dénombrable d’ouverts $ v $-intégrables. Il existe une partition de $ X - B $ formée d’un ensemble $ v $-négligeable N, et d’une suite $ (K_n) $ d’ensembles compacts tels que la restriction de $ f $ à chacun des $ K_n $ soit continue. Soit S l’ensemble des $ t \in T $ tels que N ne soit pas $ \lambda_t $-négligeable : S est localement $ \mu $-négligeable (resp. $ \mu $-négligeable) d’après le cor. 1 de la prop. 3. Les ensembles $ K_n $, B, N sont mesurables pour toute mesure sur T, et la restriction de $ f $ à chacun d’eux est $ \lambda_t $-mesurable pour tout $ t \notin S $. La fonction $ f $ est donc $ \lambda_t $-mesurable pour tout $ t \notin S $ (chap. IV, 2e éd., § 5, n° 10, prop. 6).

Pour établir c), reprenons les notations de la démonstration de la prop. 3 ; $ f $ étant $ v $-mesurable, est mesurable pour chacune des mesures $ \nu_\alpha \leq \nu $. Or ces mesures sont bornées, donc modérées, et il résulte de a) que M est localement $ \mu_\alpha $-négligeable pour tout $ \alpha \in A $. Cela entraîne que M est localement $ \mu $-négligeable ($ \S 2 $, n° 2, cor. 2 de la prop. 1).

#### Proposition 5 {#int-v-s3-prop-5 .statement}

Soit $ f $ une fonction numérique positive $ v $-mesurable définie dans X, et soit N l’ensemble des $ t \in T $ tels que $ f $ ne soit pas $ \lambda_t $-mesurable et $ \lambda_t $-modérée.

a) Supposons que $ f $ soit $ v $-modérée. L’ensemble N est alors localement $ \mu $-négligeable, la fonction $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ est $ \mu $-mesurable, et on a

$$
\int^* f(x) \, dv(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

b) Supposons que $ f $ soit $ v $-modérée, et que $ \Lambda $ soit vaguement continue. L’ensemble N est alors $ \mu $-négligeable, la fonction $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ est $ \mu $-mesurable et $ \mu $-modérée, et on a

$$
\int^* f(x) \, dv(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

c) Supposons qu’on ait $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout. L’ensemble N est alors localement $ \mu $-négligeable, la fonction $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ est $ \mu $-mesurable, et on a (9).

Démontrons d’abord a) (resp. b)) en supposant que $ f $ soit $ v $-modérée. Les assertions concernant l’ensemble N ont déjà été établies (prop. 4, et cor. 2 de la prop. 3). D’après la prop. 6 du § 1, nous pouvons nous borner à prouver a) (resp. b)) dans chacun des cas particuliers suivants:
    1) La fonction $ f $ est $ \nu $-négligeable.
    2) Il existe un compact $ K $ tel que $ f $ soit nulle hors de $ K $, et que la restriction de $ f $ à $ K $ soit continue.
    Le cas particulier 1) a déjà été traité (cor. 1 de la prop. 3). Pour traiter le second, désignons par $ G $ un ouvert $ \nu $-intégrable contenant $ K $, par $ M $ une constante qui majore $ f $, par $ h $ la fonction semi-continue inférieurement $ M \varphi_G $, et par $ g $ la fonction $ h - f $. La fonction $ f $ étant semi-continue supérieurement dans $ X $, $ g $ est semi-continue inférieurement et positive. En outre, $ f $, $ g $, $ h $ sont $ \nu $-intégrables.
    Appliquons alors la formule (4) (resp. (5)) aux fonctions semi-continues inférieurement $ h $ et $ g $. Il apparaît par différence que la fonction $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ (resp. $ \int^* f(x) \, d\lambda_t(x) $) est $ \mu $-mesurable, et qu’on a la formule (9) (resp. (10)). Enfin, sous l’hypothèse b), la fonction $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ a une intégrale supérieure finie : elle est donc bien $ \mu $-modérée.
    Pour démontrer c), reprenons les mesures $ \mu_\alpha $ et $ \nu_\alpha $ de la démonstration de la prop. 3 ; $ f $ étant $ \nu_\alpha $-mesurable et $ \nu_\alpha $-modérée, l’assertion a) entraîne que $ t \mapsto \int^* f(x) \, d\lambda_t(x) $ est $ \mu_\alpha $-mesurable, et que
    $$
    \int^* f(x) \, d\nu_\alpha(x) = \int^* d\mu_\alpha(t) \int^* f(x) \, d\lambda_t(x).
    $$
Il ne reste plus qu’à sommer sur $ \alpha $, en appliquant les prop. 1 et 2 du § 2, n° 2.

Si $ f $ n’est pas supposée $ \nu $-modérée, et si l’on ne fait pas l’hypothèse de c), la relation (9) peut être inexacte (exerc. 3).

#### Corollaire {#int-v-s3-n2-cor-1 .statement}

Soit $ \mathbf{f} $ une fonction définie dans $ X $, à valeurs dans un espace de Banach $ F $ ou dans $ \bar{\mathbf{R}} $, $ \nu $-mesurable et $ \nu $-modérée. Pour que $ \mathbf{f} $ soit $ \nu $-intégrable, il faut et il suffit que
$$
\int^* d\mu(t) \int^* |\mathbf{f}(x)| \, d\lambda_t(x) < +\infty.
$$
Cela résulte aussitôt de la prop. 5 et du critère d’intégrabilité (chap. IV, § 5, n° 6, th. 5).

### 3. Intégrales superposées de fonctions à valeurs dans un espace de Banach

#### Théorème 1 {#int-v-s3-thm-1 .statement}

Soit $ \mathbf{f} $ une fonction à valeurs dans un espace de Banach $ F $ ou dans $ \bar{\mathbf{R}} $, et soit $ H $ l’ensemble des $ t \in T $ pour lesquels $ \mathbf{f} $ n’est pas $ \lambda_t $-intégrable.

a) Si $ f $ est $ v $-intégrable, $ H $ est localement $ \mu $-négligeable, la fonction $ t \mapsto \int f(x)\ d\lambda_t(x) $ (définie pour $ t \notin H $) est essentiellement $ \mu $-intégrable, et on a

(11)
$$
\int f(x)\ dv(x) = \int d\mu(t) \int f(x)\ d\lambda_t(x).
$$

b) Si $ f $ est $ v $-intégrable, et si $ \Lambda $ est vaguement continue, $ H $ est de plus $ \mu $-négligeable, et la fonction $ t \mapsto \int f(x)\ d\lambda_t(x) $ (définie pour $ t \notin H $) est $ \mu $-intégrable.

c) Si l’on a $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout, les conclusions de a) restent vraies pour une fonction $ f $ essentiellement $ v $-intégrable.

Nous allons établir d’abord a) (resp. b)). Cet énoncé est vrai lorsque $ f $ est une fonction numérique positive (prop. 5); si $ f $ est une fonction intégrable à valeurs dans $ \bar{\mathbf{R}} $, ce résultat s’applique aux fonctions positives $ f^+ $ et $ f^- $, et s’étend donc à $ f $ par différence. Reste à traiter le cas des fonctions à valeurs dans $ F $. Soit $ \mathcal{H} $ le sous-espace de $ \mathcal{L}_F^1(v) $ constitué par les combinaisons linéaires, à coefficients dans $ F $, de fonctions de $ \mathcal{K}(X) $: le résultat relatif aux fonctions réelles entraîne aussitôt la validité de l’énoncé pour les éléments de $ \mathcal{H} $. Or $ \mathcal{H} $ est dense dans $ \mathcal{L}_F^1(v) $; pour tout $ f \in \mathcal{L}_F^1(v) $, il existe donc une suite $ (f_n) $ d’éléments de $ \mathcal{H} $, qui possède les propriétés suivantes:

1) la suite $ (f_n) $ converge vers $ f $ en moyenne dans $ \mathcal{L}_F^1(v) $, et $ v $-presque partout;
2) la fonction $ g = |f_0| + \sum_{n \in \mathbf{N}} |f_{n+1} - f_n| $ est telle que $ v^*(g) < +\infty $ (chap. IV, § 3, n° 4, th. 3).

Soit $ N_1 $ l’ensemble des $ t \in T $ tels que $ \lambda_t^*(g) = +\infty $: $ N_1 $ est localement $ \mu $-négligeable (resp. $ \mu $-négligeable) d’après la formule (6) (resp. (7)). Pour $ t \notin N_1 $, les $ f_n $ appartiennent à $ \mathcal{L}_F^1(\lambda_t) $, la suite $ (f_n) $ converge $ \lambda_t $-presque partout, ainsi que pour la topologie de la convergence en moyenne dans $ \mathcal{L}_F^1(\lambda_t) $ (chap. IV, § 3, n° 3, prop. 6). Soit $ M $ l’ensemble des $ x \in X $ tels que $ f_n(x) $ ne converge pas vers $ f(x) $: $ M $ étant $ v $-négligeable, l’ensemble $ N_2 $ des $ t \in T $ tels que $ M $ ne soit pas $ \lambda_t $-négligeable est localement $ \mu $-négligeable (resp. $ \mu $-négligeable) d’après le cor. 1 de la prop. 3.

Supposons que $ t $ n’appartienne pas à $ N_1 \cup N_2 $; la suite $ (f_n) $ converge en moyenne dans $ \mathcal{L}_F^1(\lambda_t) $, et converge $ \lambda_t $-presque partout vers $ f $. On a donc $ f \in \mathcal{L}_F^1(\lambda_t) $, et $ \int f\ d\lambda_t = \lim_{n \to \infty} \int f_n\ d\lambda_t $ (chap. IV, § 4, n° 1). L’ensemble $ H $ de l’énoncé est donc contenu dans $ N_1 \cup N_2 $;

il est par suite localement $ \mu $-négligeable (resp. $ \mu $-négligeable). D’autre part, la fonction $ t \mapsto \int f\, d\lambda_t $ est égale localement $ \mu $-presque partout à la limite d’une suite de fonctions $ \mu $-mesurables ; elle est donc $ \mu $-mesurable. Enfin, on a pour tout $ t \notin N_1 \cup N_2 $ et tout $ n $,

$$
\left| \int f_n(x)\, d\lambda_t(x) \right| \leq \int^* g(x)\, d\lambda_t(x)
$$

en vertu de l’inégalité $ |f_n| \leq g $, et de la prop. 2 du chap. IV, § 4, n° 2. Or la fonction $ t \mapsto \int^* g(x)\, d\lambda_t(x) $ est essentiellement $ \mu $-intégrable (resp. $ \mu $-intégrable) d’après la prop. 5. On peut donc appliquer le théorème de Lebesgue, et il vient :

$$
\int d\mu(t) \int f(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int d\mu(t) \int f_n(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int f_n(x)\, dv(x).
$$

Comme $ \int f_n(x)\, dv(x) $ tend vers $ \int f(x)\, dv(x) $ lorsque $ n $ tend vers $ +\infty $, d’après les hypothèses faites sur la suite $ (f_n) $, la relation (11) en résulte, et on a prouvé a) (resp. b)).

Supposons maintenant que $ \lambda_t^*(1) < +\infty $ localement $ \mu $-presque partout, et que $ g $ soit une fonction essentiellement $ v $-intégrable. Soit $ f $ une fonction $ v $-intégrable telle que $ g = f $ localement $ v $-presque partout ($ \S 1, n° 3 $). On a alors $ g = f $ presque partout pour $ \lambda_t $, sauf pour des $ t $ qui forment un ensemble localement $ \mu $-négligeable $ P $ (cor. 1 c) de la prop. 3). On a $ \int g\, d\lambda_t = \int f\, d\lambda_t $ pour $ t \notin P \cup H $, et cela achève la démonstration.

#### Remarque {#int-v-s3-n3-rem-1 .statement}

Soit $ \Lambda : t \mapsto \lambda_t $ une application $ \mu $-adéquate de $ T $ dans $ \mathcal{M}_+(X) $. Si une application $ \Lambda' : t \mapsto \lambda'_t $ de $ T $ dans $ \mathcal{M}_+(X) $ est égale à $ \Lambda $ localement $ \mu $-presque partout, il résulte aussitôt des définitions que $ \Lambda' $ est aussi $ \mu $-adéquate, et que $ \Lambda $ et $ \Lambda' $ ont même intégrale. Si maintenant $ H : t \mapsto \eta_t $ est une fonction à valeurs dans $ \mathcal{M}_+(X) $, définie localement $ \mu $-presque partout, nous dirons encore que $ H $ est $ \mu $-adéquate si elle est égale localement $ \mu $-presque partout à une application $ \Lambda : t \mapsto \lambda_t $, partout définie et $ \mu $-adéquate. On pose alors $ \int \eta_t\, d\mu(t) = \int \lambda_t\, d\mu(t) $, définition qui ne dépend pas de la fonction $ \Lambda $ utilisée. Nous laisserons au lecteur le soin de vérifier que les propositions démontrées dans les numéros précédents s’étendent aux fonctions $ \mu $-adéquates définies localement $ \mu $-presque partout.

### 4. Fonctions universellement mesurables

#### Définition 2 {#int-v-s3-def-2 .statement}

On dit qu’une application $ f $ de $ T $ dans un espace topologique $ F $ est universellement mesurable si elle est $ \mu $-mesurable pour toute mesure positive $ \mu $ sur $ T $.

Les sous-ensembles de $ T $ dont la fonction caractéristique est universellement mesurable sont appelés ensembles universellement mesurables. Ils forment une tribu sur $ T $ (chap. IV, 2e éd., § 5, n° 4, cor. 2 du th. 2) qui contient les ensembles boréliens (même réf., cor. 3), et les ensembles sousliniens si $ T $ est métrisable (chap. IV, 2e éd., § 5, n° 1, cor. 2 de la prop. 3). Pour qu’une application $ f $ de $ T $ dans un espace topologique $ F $, métrisable de type dénombrable, soit universellement mesurable, il faut et il suffit que l’image réciproque par $ f $ de toute boule fermée de $ F $ soit une partie universellement mesurable de $ T $ (chap. IV, § 5, n° 5, th. 4).

#### Proposition 6 {#int-v-s3-prop-6 .statement}

Pour qu’une application $ f $ de $ T $ dans un espace topologique $ F $ soit universellement mesurable, il faut et il suffit que $ f $ soit mesurable pour toute mesure positive sur $ T $ à support compact.

Cette condition est évidemment nécessaire; elle est d’autre part suffisante, car toute mesure positive $ \mu $ est somme d’une famille de mesures à support compact ($ § 2, n° 3, $ prop. 4): l’énoncé résulte alors de la prop. 2 du $ § 2, n° 2 $.

#### Proposition 7 {#int-v-s3-prop-7 .statement}

Soit $ \mu $ une mesure positive sur $ T $, et soit $ f $ une application $ \mu $-mesurable de $ T $ dans un espace topologique $ F $. Il existe alors une application universellement mesurable $ f' $ de $ T $ dans $ F $, telle que $ f = f' $ localement $ \mu $-presque partout.

Soit $ \mathfrak{K} $ l’ensemble des compacts de $ T $ tels que la restriction de $ f $ à $ K $ soit continue; $ \mathfrak{K} $ étant $ \mu $-dense (chap. IV, 2e éd., § 5, n° 10, prop. 13), il existe une famille $ (K_i)_{i \in I} $ d’éléments de $ \mathfrak{K} $ deux à deux disjoints, localement dénombrable, telle que l’ensemble $ N = T - \bigcup_{i \in I} K_i $ soit localement $ \mu $-négligeable (chap. IV, 2e éd., § 5, n° 9, prop. 14). Soit $ x $ un élément de $ F $; posons

$$
f'(t) = f(t) \text{ si } t \in \bigcup_{i \in I} K_i,
$$
$$
f'(t) = x \text{ si } t \in N.
$$

Les fonctions $ f $ et $ f' $ sont égales localement $ \mu $-presque partout.

### 5. Diffusions

#### Définition 3 {#int-v-s3-def-3 .statement}

Soit $ X $ un espace localement compact, et soit $ \Lambda : t \mapsto \lambda_t $ une application de $ T $ dans $ \mathcal{M}_+(X) $. On dit que $ \Lambda $ est une diffusion de $ T $ dans $ X $ si $ \Lambda $ est adéquate pour toute mesure positive sur $ T $ à support compact. On dit que la diffusion $ \Lambda $ est bornée si toutes les mesures $ \lambda_t $ sont bornées et si on a $ \sup_{t \in T} \| \lambda_t \| < +\infty $; cette quantité est alors appelée la norme de $ \Lambda $, et notée $ \| \Lambda \| $.

La proposition suivante ne fait que traduire la définition :

#### Proposition 8 {#int-v-s3-prop-8 .statement}

Pour qu’une application $ \Lambda : t \mapsto \lambda_t $ de $ T $ dans $ \mathcal{M}_+(X) $ soit une diffusion, il faut et il suffit que les conditions suivantes soient satisfaites :
1) Pour toute fonction semi-continue inférieurement $ f \geqslant 0 $ définie dans $ X $, la fonction $ t \mapsto \lambda_t^*(f) $ est universellement mesurable dans $ T $.
2) Pour toute fonction $ g \in \mathscr{K}_+(X) $, la fonction $ t \mapsto \lambda_t(g) $ est localement bornée dans $ T $.
3) Pour toute fonction semi-continue inférieurement $ f \geqslant 0 $ définie dans $ X $, et toute mesure positive $ \mu $ à support compact dans $ T $, on a la relation suivante, où $ v $ désigne $ \int \lambda_t \, d\mu(t) $:

$$
\int f(x) \, dv(x) = \int d\mu(t) \int f(x) \, d\lambda_t(x).
$$

Supposons que $ \Lambda $ soit une diffusion. La condition 1) est alors satisfaite d’après la définition des applications adéquates (n° 1, déf. 1), et la prop. 6 ; la condition 3) est satisfaite d’après la formule (4), puisque $ \Lambda $ est $ \mu $-adéquate. Soit $ g \in \mathscr{K}_+(X) $, et soit $ u $ la fonction $ t \mapsto \lambda_t(g) $ (universellement mesurable d’après 1)); supposons que $ u $ ne soit pas localement bornée. Il existe alors un compact $ K $ tel que $ u $ ne soit pas bornée sur $ K $, et il existe donc une suite $ (t_n) $ d’éléments de $ K $ telle que $ u(x_n) \geqslant n^2 $ pour tout $ n \geqslant 1 $; $ u $ n’est donc pas intégrable pour la mesure à support compact $ \mu = \sum_{n \geqslant 1} \frac{1}{n^2} \varepsilon_{t_n} $, en contradiction avec l’hypothèse faite sur $ \Lambda $, qui entraîne que $ t \mapsto \lambda_t(g) $ est intégrable pour toute mesure positive à support compact. Les trois conditions ci-dessus sont donc nécessaires. Inversement, les conditions 1) et 2) entraînent que $ \Lambda $ est scalairement essentiellement $ \mu $-intégrable pour toute mesure $ \mu $ à support compact. Comme toute mesure $ \mu' \geq 0 $ majorée par une mesure $ \mu $ à support compact a aussi un support compact, les conditions 1) et 3) expriment que $ \Lambda $ est $ \mu $-adéquate pour toute mesure positive à support compact, ce qui est bien le résultat cherché.

#### Proposition 9 {#int-v-s3-prop-9 .statement}

*Soit $ \Lambda : t \mapsto \lambda_t $ une application de $ T $ dans $ \mathcal{M}_+(X) $, telle que la fonction $ t \mapsto \lambda_t(g) $ soit universellement mesurable et localement bornée dans $ T $ pour tout $ g \in \mathcal{K}_+(X) $. On peut affirmer que $ \Lambda $ est une diffusion dans chacun des cas suivants :
a) la topologie de $ X $ admet une base dénombrable ;
b) $ \Lambda $ est universellement mesurable pour la topologie vague.*
En effet, soit $ \mu $ une mesure positive à support compact dans $ T $; l’application $ \Lambda $ est scalairement essentiellement $ \mu $-intégrable, donc $ \mu $-adéquate si a) ou b) est satisfaite (prop. 2).

Dans toute la fin de ce paragraphe, nous adopterons les notations suivantes : nous désignerons par $ \langle \eta, h \rangle $ l’intégrale supérieure essentielle, pour une mesure positive $ \eta $, d’une fonction positive $ \eta $-mesurable $ h $. L’application $ \Lambda : t \mapsto \lambda_t $ sera une diffusion de $ T $ dans $ X $. Si $ f $ est une fonction universellement mesurable positive définie dans $ X $, nous noterons $ \Lambda f $ l’application $ t \mapsto \lambda_t^*(f) $. Si $ \mu $ est une mesure positive sur $ T $ telle que $ \Lambda $ soit scalairement essentiellement $ \mu $-intégrable, nous noterons $ \mu \Lambda $ la mesure $ \int \lambda_t \, d\mu(t) $. La définition de l’intégrale prend alors la forme
$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle \quad \text{pour } f \in \mathcal{K}_+(X).
$$
Nous dirons qu’une mesure positive $ \mu $ sur $ T $ appartient au domaine de $ \Lambda $ si $ \Lambda $ est $ \mu $-adéquate : cela revient à dire (compte tenu de la prop. 8) que $ \Lambda $ est scalairement essentiellement $ \mu $-intégrable et qu’on a $ \langle \mu' \Lambda, f \rangle = \langle \mu', \Lambda f \rangle $ pour toute mesure positive $ \mu' \leq \mu $ et pour toute fonction $ f $ positive semi-continue inférieurement.

#### Proposition 10 {#int-v-s3-prop-10 .statement}

*Soient $ f, g $ deux fonctions universellement mesurables positives sur $ X $, $ a $ un nombre $ \geq 0 $, $ \mu $ et $ \nu $ deux mesures positives sur $ T $.*

a) On a $ \Lambda(f + g) = \Lambda f + \Lambda g, \Lambda(af) = a \Lambda f $.

b) Si $ \mu $ et $ \nu $ appartiennent au domaine de $ \Lambda $, il en est de même de $ \mu + \nu $ et de $ a \mu $, et on a $ (\mu + \nu)\Lambda = \mu \Lambda + \nu \Lambda, (a \mu) \Lambda = a(\mu \Lambda) $.

Le seul point non évident est l’appartenance de $ (\mu + \nu) $ au domaine de $ \Lambda $, qui se traite en remarquant que toute mesure positive majorée par $ \mu + \nu $ est de la forme $ \mu' + \nu' $, où $ \mu' \leq \mu, \nu' \leq \nu $ (« lemme de décomposition », chap. II, § 1, n° 1). Voir aussi la prop. 11 ci après.

#### Proposition 11 {#int-v-s3-prop-11 .statement}

Pour qu’une mesure positive $ \mu $ sur $ T $ appartienne au domaine de $ \Lambda $, il faut et il suffit que $ \Lambda $ soit scalairement essentiellement $ \mu $-intégrable.

Cette condition est évidemment nécessaire. Inversement, supposons-la satisfaite, et soit $ f $ une fonction positive semi-continue inférieurement définie dans $ X $. La fonction $ \Lambda f $ est universellement mesurable, donc $ \mu $-mesurable. Nous allons prouver qu’on a $ \langle \mu, \Lambda f \rangle = \langle \mu \Lambda, f \rangle $; comme cette égalité vaudra aussi pour toute mesure positive $ \mu' \leq \mu $, puisque $ \Lambda $ est aussi scalairement essentiellement $ \mu' $-intégrable, il en résultera que $ \Lambda $ est $ \mu $-adéquate.

Soit $ (\mu_i)_{i \in I} $ une famille sommable de mesures positives à support compact, telle que $ \mu = \sum_{i \in I} \mu_i $ (§ 2, n° 3, prop. 4); la famille des mesures $ \mu_i \Lambda $ est alors sommable, et $ \mu \Lambda = \sum_{i \in I} \mu_i \Lambda $ (n° 1, cor. de la prop. 1). On a par conséquent $ \langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle $ (§ 2, n° 1, prop. 1); mais $ \Lambda $ est $ \mu_i $-adéquate, de sorte qu’on a

$$
\langle \mu_i \Lambda, f \rangle = \langle \mu_i, \Lambda f \rangle.
$$

En appliquant de nouveau la prop. 1 du § 2, on obtient l’égalité cherchée:

$$
\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i, \Lambda f \rangle = \langle \mu, \Lambda f \rangle.
$$

#### Corollaire 1 {#int-v-s3-prop-11-cor-1 .statement}

Si $ \Lambda $ est une diffusion bornée, toute mesure positive bornée $ \mu $ appartient au domaine de $ \Lambda $, et on a

$$
\| \mu \Lambda \| \leq \| \mu \| \| \Lambda \|.
$$

#### Corollaire 2 {#int-v-s3-prop-11-cor-2 .statement}

Supposons que $ \mu $ soit somme d’une famille sommable $ (\mu_\alpha)_{\alpha \in A} $ de mesures positives appartenant au domaine de $ \Lambda $. Pour que $ \mu $ appartienne au domaine de $ \Lambda $, il faut et il suffit que la famille des mesures $ \mu_\alpha \Lambda $ soit sommable, et on a dans ce cas
$$
\mu \Lambda = \sum_{\alpha \in \mathbf{A}} \mu_\alpha \Lambda.
$$
Il suffit d’appliquer le cor. de la prop. 1 du n° 1.

La proposition 5, exprimée dans le langage des diffusions, prend la forme suivante :

#### Proposition 12 {#int-v-s3-prop-12 .statement}

Soit $ \mu $ une mesure positive sur $ T $ qui appartient au domaine de $ \Lambda $, et soit $ f $ une fonction universellement mesurable $ \geqslant 0 $ définie dans $ X $. Si $ f $ est modérée pour la mesure $ \mu \Lambda $, ou si les mesures $ \lambda_t $ sont bornées, la fonction $ \Lambda f $ est $ \mu $-mesurable et on a
$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle.
$$

#### Corollaire {#int-v-s3-n5-cor-1 .statement}

Si $ X $ est dénombrable à l’infini, ou si les mesures $ \lambda_t $ sont bornées, la fonction $ \Lambda f $ est universellement mesurable dans $ T $ pour toute fonction universellement mesurable $ f \geqslant 0 $ définie dans $ X $, et on a (13).

### 6. Composition des diffusions bornées

#### Proposition 13 {#int-v-s3-prop-13 .statement}

Soient $ T, X, Y $ trois espaces localement compacts, $ \Lambda : t \mapsto \lambda_t $ une diffusion bornée de $ T $ dans $ X $, $ H : x \mapsto \eta_x $ une diffusion bornée de $ X $ dans $ Y $. L’application $ t \mapsto \lambda_t H $ est alors une diffusion bornée de $ T $ dans $ Y $, que l’on désigne par $ \Lambda H $, et on a
$$
\| \Lambda H \| \leqslant \| \Lambda \| \| H \|.
$$
Soient $ f $ une fonction universellement mesurable $ \geqslant 0 $ définie dans $ Y $, $ \mu $ une mesure sur $ T $. Supposons que $ \mu $ appartienne au domaine de $ \Lambda $, et que $ \mu \Lambda $ appartienne au domaine de $ H $; alors $ \mu $ appartient au domaine de $ \Lambda H $ et on a :
$$
\begin{align}
\langle \mu(\Lambda H), f \rangle &= \langle \mu \Lambda, H f \rangle = \langle \mu, \Lambda H f \rangle; \\
(\mu \Lambda) H &= \mu(\Lambda H); \quad \Lambda(H f) = (\Lambda H) f.
\end{align}
$$
Posons $ \gamma_t = \lambda_t H $; nous désignerons par $ \Gamma $ l’application $ \Lambda H $ de $ T $ dans $ \mathcal{M}_+(Y) $, et par $ \Gamma f $ la fonction $ t \mapsto \langle \gamma_t, f \rangle $ (par abus de notation, car nous ignorons encore si $ \Gamma $ est une diffusion). On a $ \langle \gamma_t, f \rangle = \langle \lambda_t H, f \rangle = \langle \lambda_t, H f \rangle $ d’après (13); la fonction $ H f $ étant positive et universellement mesurable dans $ X $ (cor. de la prop. 12), il en résulte d’abord que $ \Gamma f = \Lambda(Hf) $, et ensuite que $ \Gamma f $ est universellement mesurable dans $ T $ (même référence). Il est clair que toutes les mesures $ \gamma_t $ ont une masse totale au plus égale à $ \| \Lambda \| \| H \| $. Par conséquent, $ \Gamma g $ est universellement mesurable et bornée pour toute fonction $ g \in \mathcal{K}_+(Y) $; $ \Gamma $ est donc scalairement essentiellement intégrable pour toute mesure bornée sur $ T $, et en particulier pour toute mesure à support compact. Plus généralement, si $ \mu $ est une mesure du domaine de $ \Lambda $, telle que $ \mu \Lambda $ appartenne au domaine de $ H $, on a, pour $ g \in \mathcal{K}_+(Y) $,

$$
\langle \mu, \Gamma g \rangle = \langle \mu, \Lambda(Hg) \rangle = \langle \mu \Lambda, Hg \rangle = \langle (\mu \Lambda)H, g \rangle.
$$

Cette dernière quantité étant finie, on voit que $ \Gamma $ est scalairement essentiellement $ \mu $-intégrable. Désignons par $ \mu \Gamma $ l’intégrale $ \int \gamma_t \, d\mu(t) $ (par abus de notation, car nous ignorons encore si $ \Gamma $ est une diffusion). Les relations précédentes s’écrivent alors

$$
\langle \mu \Gamma, g \rangle = \langle (\mu \Lambda)H, g \rangle,
$$

ou encore $ \mu \Gamma = (\mu \Lambda)H $, car $ g $ est arbitraire dans $ \mathcal{K}_+(Y) $.

Considérons à nouveau la fonction universellement mesurable $ f \geqslant 0 $. Nous avons

$$
\langle \mu \Gamma, f \rangle = \langle (\mu \Lambda)H, f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda(Hf) \rangle = \langle \mu, \Gamma f \rangle.
$$

Lorsque $ f $ est semi-continue inférieurement, et lorsque $ \mu $ parcourt l’ensemble des mesures positives à support compact, ces relations expriment que $ \Gamma $ est une diffusion de $ T $ dans $ Y $. L’énoncé ne fait alors qu’expliciter les relations obtenues au cours de la démonstration ci-dessus.

#### Définition 4 {#int-v-s3-def-4 .statement}

*Les notations étant celles de la proposition 13, la diffusion $ \Lambda H $ est appelée la diffusion composée des diffusions bornées $ H $ et $ \Lambda $.*

Soient $ X_1, X_2, X_3, X_4 $ quatre espaces localement compacts, $ \Lambda_1, \Lambda_2, \Lambda_3 $ trois diffusions bornées de $ X_1 $ dans $ X_2, X_2 $ dans $ X_3, X_3 $ dans $ X_4 $ respectivement. Il résulte aussitôt de la prop. 13 qu’on a

$$
(\Lambda_1 \Lambda_2) \Lambda_3 = \Lambda_1 (\Lambda_2 \Lambda_3).
$$

On utilisera donc des notations sans parenthèses pour la composition des diffusions.

#### Exemple {#int-v-s3-n6-exa-1 .statement}

Soient $ u $ une application universellement mesurable de $ T $ dans $ X $, $ v $ une application universellement mesurable de $ X $ dans $ Y $; d’après la prop. 2b), on définit des diffusions $ \Lambda $ et $ H $ par les formules :

$$
\lambda_t = \varepsilon_{u(t)}, \quad \eta_x = \varepsilon_{v(x)} ;
$$

la diffusion $ \Gamma = \Lambda H $ est alors définie par

$$
\gamma_t = \varepsilon_{(v \circ u)(t)}
$$

On prendra donc garde que l’ordre de composition des diffusions est l’opposé de l’ordre habituel de composition des fonctions.

## EXERCICES {#int-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
