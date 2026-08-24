---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 8
section_title: Espaces localement convexes complexes
lang: fr
source: evt-i-v-fr
book_pages: EVT II.100
pdf_pages: 0099-0104, 0135-0135
extraction: ocr
subsections:
    - "no": 1
      title: Espaces vectoriels topologiques sur C
      page: 64
      pdf_page: 99
    - "no": 2
      title: Espaces localement convexes complexes
      page: 65
      pdf_page: 100
    - "no": 3
      title: Le théorème de Hahn-Banach et ses applications
      page: 67
      pdf_page: 102
    - "no": 4
      title: Topologies faibles sur les espaces vectoriels complexes
      page: 68
      pdf_page: 103
statements: 10
exercises: 3
content_sha256: d88b2b79394fd0cd193c5fcc8ec6b3ced35986fe395778391e22ec61a5fa6baa
---

## § 8. ESPACES LOCALEMENT CONVEXES COMPLEXES

### 1. Espaces vectoriels topologiques sur C

Soit E un espace vectoriel topologique sur le corps C des nombres complexes ; la topologie de E est aussi compatible avec la structure d’espace vectoriel sur $ \mathbf{R} $ obtenue en restreignant à $ \mathbf{R} $ le corps des scalaires. Nous désignerons par $ E_0 $ l’espace vectoriel topologique sur $ \mathbf{R} $ *sous-jacent* à E (I, p. 2). On notera que, dans $ E_0 $, l’application $ x \mapsto ix $ (qui n’est pas une homothétie) est un *automorphisme* u de la structure d’espace vectoriel topologique de $ E_0 $ tel que $ u^2(x) = -x $.

Inversement, soit F un espace vectoriel topologique sur $ \mathbf{R} $, et supposons qu’il existe un automorphisme u de F tel que $ u^2 = -1_F $ ($ 1_F $ automorphisme identique de F). On sait (A, IX, § 3, no 2) qu’on peut alors définir sur F une structure d’espace vectoriel par rapport à C, en posant, pour tout $ \lambda = \alpha + i\beta \in C $ et tout $ x \in F $, $ \lambda x = \alpha x + \beta u(x) $. En outre, l’application $ (\alpha, \beta, x) \mapsto \alpha x + \beta u(x) $ de $ \mathbf{R}^2 \times F $ dans F étant continue, la topologie de F est compatible avec la structure d’espace vectoriel par rapport à C ainsi définie ; si E désigne l’espace vectoriel topologique sur C défini de cette manière, F est l’espace vectoriel topologique sur $ \mathbf{R} $ sous-jacent à E.

#### Remarque {#evt-ii-s8-n1-rem-1 .statement}

Étant donné un espace vectoriel topologique F sur $ \mathbf{R} $, il n’existe pas toujours d’automorphisme u de F de carré $ -1_F $ : par exemple, on ne peut pas définir de structure d’espace vectoriel par rapport à C sur un espace vectoriel de dimension finie *impaire* par rapport à $ \mathbf{R} $.

Soient E un espace vectoriel topologique sur C, $ E_0 $ l’espace vectoriel topologique sur $ \mathbf{R} $ sous-jacent à E. Toute variété linéaire M dans E est aussi une variété linéaire dans $ E_0 $, la réciproque étant inexacte. Pour éviter toute confusion, on dira qu’une variété linéaire pour une structure d’espace vectoriel par rapport à $ \mathbf{C} $ (resp. par rapport à $ \mathbf{R} $) est une variété linéaire *complexe* (resp. *réelle*). Une variété linéaire complexe de dimension finie $ n $ (resp. de codimension finie $ n $) est une variété linéaire réelle de dimension $ 2n $ (resp. de codimension $ 2n $). Pour qu’un sous-espace vectoriel réel $ M $ de $ E $ soit aussi un sous-espace vectoriel complexe, il faut et il suffit que $ iM \subset M $.

Rappelons que, si $ E $ et $ F $ sont deux espaces vectoriels topologiques sur $ \mathbf{C} $, une application de $ E $ dans $ F $ est dite $ \mathbf{C}$-linéaire (resp. $ \mathbf{R}$-linéaire) si elle est une application linéaire pour les structures d’espace vectoriel de $ E $ et de $ F $ par rapport à $ \mathbf{C} $ (resp. $ \mathbf{R} $) ; toute application $ \mathbf{C}$-linéaire est évidemment $ \mathbf{R}$-linéaire, la réciproque étant inexacte. Par abus de langage, une forme $ \mathbf{C}$-linéaire sur $ E $ sera dite forme linéaire *complexe*, et une forme $ \mathbf{R}$-linéaire sur $ E $ (c’est-à-dire une forme linéaire sur $ E_0 $) sera dite forme linéaire *réelle*. Si $ f $ est une forme linéaire complexe sur $ E $, il est clair que la partie réelle $ g = \Re f $ et la partie imaginaire $ h = \Im f $ de $ f $ sont des formes linéaires réelles ; en outre, la relation $ f(ix) = if(x) $ entraîne l’identité $ h(x) = -g(ix) $; autrement dit, on a

$$
f(x) = (\Re f)(x) - i(\Re f)(ix).
$$

Inversement, si $ g $ est une forme linéaire réelle sur $ E $, $ f(x) = g(x) - ig(ix) $ est l’unique forme linéaire complexe sur $ E $ telle que $ \Re f = g $; pour que $ f $ soit continue dans $ E $, il faut et il suffit évidemment que $ g $ le soit.

Soit maintenant $ H $ un *hyperplan complexe* dans $ E $, d’équation $ f(x) = \alpha + i\beta $, $ f $ étant une forme linéaire complexe sur $ E $; en posant $ g = \Re f $, on voit que $ H $ est l’intersection des deux *hyperplans réels* $ H_1 $, $ H_2 $ d’équations respectives $ g(x) = \alpha $ et $ g(ix) = -\beta $; si $ H $ est *fermé*, il en est de même de $ H_1 $ et $ H_2 $ (I, p. 13, th. 1). Inversement, soit $ H_0 $ un hyperplan *réel* homogène, d’équation $ g(x) = 0 $ (*g* forme linéaire réelle sur $ E $) ; l’intersection $ H $ de $ H_0 $ et de $ iH_0 $ est un hyperplan *complexe* homogène, et si $ f $ est la forme linéaire complexe telle que $ \Re f = g $, $ f(x) = 0 $ est une équation de $ H $; si $ H_0 $ est fermé, il en est de même de $ H $.

Soit $ G $ un espace vectoriel topologique sur $ \mathbf{R} $, et soit $ G_{(C)} $ l’espace vectoriel sur $ \mathbf{C} $ déduit de $ G $ par extension à $ \mathbf{C} $ du corps des scalaires (A, II, p. 82). Identifions $ G $ à un sous-ensemble de $ G_{(C)} $ par l’application $ x \mapsto 1 \otimes x $. L’application $ \mathbf{R}$-linéaire $ (x, y) \mapsto x + i.y $ est alors une bijection de $ G \times G $ sur $ G_{(C)} $, par laquelle on transporte à $ G_{(C)} $ la topologie produit de $ G \times G $. Muni de cette topologie, $ G_{(C)} $ est alors un espace vectoriel topologique sur $ \mathbf{C} $. On dira que $ G_{(C)} $ est l’*espace vectoriel topologique complexifié de* $ G $.

### 2. Espaces localement convexes complexes

Dans un espace vectoriel complexe $ E $, dire qu’une partie $ A $ de $ E $ est *équilibrée* signifie que, pour tout $ x \in A $, on a $ \rho x \in A $ pour $ 0 \leq \rho \leq 1 $, et $ e^{i\vartheta}x \in A $ pour tout $ \vartheta $ réel.

On dit qu’une partie A de E est *convexe* si elle est convexe dans l’espace vectoriel réel $ E_0 $ sous-jacent à E. Pour qu’une partie convexe $ A \neq \varnothing $ de E soit équilibrée, il suffit que l’on ait $ e^{i\theta}A \subset A $ pour tout $ \theta $ réel ; en effet, cela entraîne d’abord $ -A = A $; comme A est symétrique, 0 appartient à A, et par suite $ \rho A \subset A $ pour $ 0 \leq \rho \leq 1 $.

Soit E un espace vectoriel topologique complexe. Le plus petit ensemble convexe équilibré (resp. fermé, convexe et équilibré) contenant une partie A de E est appelé l'*enveloppe convexe équilibrée* (resp. l'*enveloppe fermée convexe équilibrée*) de A ; l’enveloppe fermée, convexe et équilibrée de A est l’adhérence de l’enveloppe convexe équilibrée de A. Cette dernière est l’enveloppe convexe de la réunion des ensembles $ e^{i\theta}A $ ; on peut donc la définir comme l’ensemble des combinaisons linéaires $ \sum_i \lambda_i x_i $, où $ (x_i) $ est une famille finie quelconque de points de A, et $ (\lambda_i) $ une famille de nombres complexes telle que $ \sum_i |\lambda_i| \leq 1 $. Si A est précompact, il en est de même de son enveloppe équilibrée (I, p. 6, prop. 3).

On dit qu’un espace vectoriel topologique complexe E est *localement convexe* si l’espace vectoriel topologique réel sous-jacent $ E_0 $ est localement convexe, c’est-à-dire si tout voisinage de 0 dans E contient un voisinage convexe de 0 ; une topologie $ \mathcal{T} $ sur E est dite *localement convexe* si elle est compatible avec la structure d’espace vectoriel de E (par rapport à $ \mathbf{C} $) et si E, muni de $ \mathcal{T} $, est localement convexe. Comme tout voisinage fermé convexe V de 0 contient alors un voisinage équilibré W de 0 (I, p. 7, prop. 4), il contient aussi son enveloppe fermée, convexe et équilibrée U ; autrement dit, les voisinages de 0 *fermés*, *convexes* et *équilibrés* forment un système fondamental de voisinages de 0 dans E, invariant par toute homothétie de rapport $ \neq 0 $.

Réciproquement, soit E un espace vectoriel complexe, et soit $ \mathfrak{S} $ une base de filtre sur E formée de parties *convexes*, *équilibrées* et *absorbantes*. On sait alors (II, p. 25, prop. 1) que l’ensemble $ \mathfrak{B} $ des transformés des ensembles de $ \mathfrak{S} $ par les homothéties de rapport $ > 0 $ est un système fondamental de voisinages de 0 pour une topologie localement convexe $ \mathcal{T} $ sur l’espace vectoriel réel $ E_0 $ sous-jacent à E. En outre, comme les ensembles de $ \mathfrak{B} $ sont équilibrés, ils sont invariants par toute homothétie $ x \mapsto e^{i\theta}x $, ce qui prouve que $ \mathcal{T} $ est compatible avec la structure d’espace vectoriel de E (sur $ \mathbf{C} $) (I, p. 7, prop. 4).

Toute topologie localement convexe sur un espace vectoriel complexe E peut être définie par un ensemble de semi-normes, car la jauge d’un voisinage ouvert, convexe et équilibré de 0 est une semi-norme sur E.

Les notions et résultats relatifs aux espaces localement convexes réels exposés dans II, p. 27 à p. 38, s’étendent aux espaces localement convexes *complexes*, sans autre modification que le remplacement des ensembles convexes symétriques par les ensembles convexes *équilibrés*.

On dit qu’un espace localement convexe complexe est un *espace de Fréchet* lorsqu’il est métrisable et complet.

### 3. Le théorème de Hahn-Banach et ses applications

#### Théorème 1 (Hahn-Banach) {#evt-ii-s8-thm-1 .statement}

Soient $ p $ une semi-norme sur un espace vectoriel complexe $ E $, $ V $ un sous-espace vectoriel de $ E $, $ f $ une forme linéaire (complexe) sur $ V $ telle que $ |f(y)| \leq p(y) $ pour tout $ y \in V $. Alors il existe une forme linéaire $ f_1 $ sur $ E $ prolongeant $ f $ et telle que $ |f_1(x)| \leq p(x) $ pour tout $ x \in E $.

En effet, $ g = \Re f $ est une forme linéaire réelle définie dans $ V $ et satisfaisant à $ |g(y)| \leq p(y) $ en tout point de $ V $; il existe donc une forme linéaire réelle $ g_1 $ définie dans $ E $, prolongeant $ g $ et telle que $ |g_1(x)| \leq p(x) $ pour tout $ x \in E $ (II, p. 24, cor. 1). Soit $ f_1(x) = g_1(x) - ig_1(ix) $ la forme linéaire complexe sur $ E $ dont $ g_1 $ est la partie réelle (II, p. 65). Pour tout $ \vartheta $ réel, on a

$$
|\Re(e^{i\vartheta}f_1(x))| = |\Re(f_1(e^{i\vartheta}x))| = |g_1(e^{i\vartheta}x)| \leq p(e^{i\vartheta}x) = p(x)
$$

puisque $ p $ est une semi-norme sur l’espace complexe $ E $; ceci entraîne la relation $ |f_1(x)| \leq p(x) $, ce qui démontre le théorème.

#### Corollaire 1 {#evt-ii-s8-thm-1-cor-1 .statement}

Soient $ E $ un espace vectoriel topologique complexe, $ x_0 $ un point de $ E $, $ p $ une semi-norme continue dans $ E $; il existe une forme linéaire continue (complexe) $ f $ définie dans $ E $, telle que $ f(x_0) = p(x_0) $ et que $ |f(x)| \leq p(x) $ pour tout $ x \in E $.

#### Corollaire 2 {#evt-ii-s8-thm-1-cor-2 .statement}

Soient $ E $ un espace localement convexe complexe, $ V $ un sous-espace vectoriel de $ E $, $ f $ une forme linéaire (complexe) définie et continue dans $ V $; il existe alors une forme linéaire continue $ f_1 $ définie dans $ E $ et prolongeant $ f $. Si $ E $ est normé, il existe une telle forme $ f_1 $ telle que $ \|f_1\| = \|f\| $.

#### Corollaire 3 {#evt-ii-s8-thm-1-cor-3 .statement}

Soient $ E $ un espace localement convexe complexe séparé, $ M $ un sous-espace vectoriel de $ E $ de dimension finie. Il existe alors un sous-espace vectoriel fermé $ N $ de $ E $, supplémentaire topologique de $ M $ dans $ E $.

Les démonstrations à partir du th. 1 sont les mêmes que celles de II, p. 24, cor. 2, p. 25, cor. 3, p. 26, prop. 2 et p. 27, cor. 2.

#### Proposition 1 {#evt-ii-s8-prop-1 .statement}

Soient $ E $ un espace vectoriel topologique complexe, $ A $ un ensemble ouvert convexe non vide dans $ E $, $ M $ une variété linéaire (complexe) non vide ne rencontrant pas $ A $. Il existe alors un hyperplan complexe fermé $ H $ contenant $ M $ et ne rencontrant pas $ A $.

On peut se borner au cas où $ 0 \in M $. Alors il existe un hyperplan réel fermé $ H_0 $ contenant $ M $ et ne rencontrant pas $ A $ (II, p. 39, th. 1). Comme $ M = iM $, l’hyperplan complexe fermé $ H = H_0 \cap (iH_0) $ répond à la question.

#### Corollaire {#evt-ii-s8-n3-cor-1 .statement}

Dans un espace localement convexe complexe $ E $, toute variété linéaire complexe fermée $ M $ est l’intersection des hyperplans complexes fermés qui la contiennent.

En effet, pour tout $ x \notin M $, il existe un voisinage ouvert convexe $ V $ de $ x $ ne rencontrant pas M, donc un hyperplan complexe fermé H contenant M et ne rencontrant pas V ; a fortiori H ne contient pas x.

#### Proposition 2 {#evt-ii-s8-prop-2 .statement}

Soient E un espace vectoriel topologique complexe, A un ensemble ouvert convexe équilibré non vide, B un ensemble convexe non vide ne rencontrant pas A. Il existe alors une forme linéaire complexe continue f sur E et un nombre α > 0 tels que l’on ait |f(x)| < α dans A et |f(y)| ≥ α dans B.

En effet, il existe une forme linéaire continue réelle g sur E et un nombre réel α tels que g(x) < α dans A et g(y) ≥ α dans B (II, p. 40, prop. 1). Comme 0 ∈ A, on a α > 0. Montrons que la forme linéaire complexe continue f(x) = g(x) − ig(ix) et le nombre α répondent à la question. En effet, comme $ \Re f = g $, on a $ |f(y)| \geq \alpha $ dans B. D’autre part, pour tout $ x \in A $ et tout θ réel, $ e^{i\theta}x $ appartient à A, puisque A est équilibré, et l’on a $ f(x) = e^{-i\theta}f(e^{i\theta}x) $; il existe alors un nombre θ tel que $ |f(x)| = \Re(e^{i\theta}f(x)) = g(e^{i\theta}x) < \alpha $, d’où la proposition.

#### Proposition 3 {#evt-ii-s8-prop-3 .statement}

Soient E un espace localement convexe complexe, A un ensemble fermé convexe équilibré dans E, K un ensemble convexe compact non vide dans E, ne rencontrant pas A. Il existe alors une forme linéaire complexe continue f sur E et un nombre α > 0 tels que l’on ait |f(x)| < α dans A et |f(y)| > α dans K.

La proposition se déduit de II, p. 41, prop. 4 comme la prop. 2 se déduisait de II, p. 40, prop. 1.

### 4. Topologies faibles sur les espaces vectoriels complexes

Les définitions et résultats du § 6, n°s 1 et 2 (II, p. 43 à 47), s’appliquent sans changement aux espaces vectoriels complexes. Si F et G sont deux espaces vectoriels complexes en dualité par une forme bilinéaire B, les espaces réels sous-jacents $ F_0, G_0 $ sont en dualité par $ \Re B $, et il résulte de II, p. 65, formule (1) que les topologies faibles $ \sigma(F, G) $ et $ \sigma(F_0, G_0) $ sont identiques.

#### Définition 1 {#evt-ii-s8-def-1 .statement}

Soient F et G deux espaces vectoriels complexes en dualité. Pour toute partie M de F, on appelle polaire de M dans G et on note $ M^\circ $ l’ensemble des $ y \in G $ tels que l’on ait $ \Re(\langle x, y \rangle) \geq -1 $ pour tout $ x \in M $.

Si l’on note $ M^\circ $ le polaire de $ M \subset F $ dans G, on a encore $ (\lambda M)^\circ = \lambda^{-1}M^\circ $ pour tout $ \lambda \in \mathbf{C}^* $.

Si M est un sous-espace vectoriel (complexe) de E, $ M^\circ $ est un sous-espace vectoriel fermé (pour $ \sigma(G, F) $), la relation $ \Re(\lambda \langle x, y \rangle) \geq -1 $ pour tout scalaire $ \lambda \in \mathbf{C} $ entraînant $ \langle x, y \rangle = 0 $; on dit encore que $ M^\circ $ est le sous-espace de G orthogonal à M.

Si M est une partie équilibrée de F, $ M^\circ $ est une partie équilibrée de G ; c’est dans ce cas l’ensemble des $ y \in G $ tels que $ |\langle x, y \rangle| \leq 1 $ pour tout $ x \in M $; en effet, cette relation équivaut à $ \Re(\langle \zeta x, y \rangle) \leq 1 $ pour tout $ x \in M $ et tout $ \zeta \in \mathbf{C} $ tel que $ |\zeta| = 1 $.

Les résultats de II, p. 47 à p. 55 sont alors valables sans restriction pour les espaces vectoriels complexes.

Exercises

## EXERCICES {#evt-ii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
