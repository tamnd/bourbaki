---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 3
section_title: Le théorème de Hahn-Banach (forme analytique)
lang: fr
source: evt-i-v-fr
book_pages: EVT II.22-EVT II.25, EVT II.76-EVT II.78
pdf_pages: 0057-0060, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement des formes linéaires positives
      page: 22
      pdf_page: 57
    - "no": 2
      title: Le théorème de Hahn-Banach (forme analytique)
      page: 24
      pdf_page: 59
statements: 5
exercises: 8
content_sha256: f26dc0978286c19efaead481d9a06fea1d7f362ba1de89237b58bab0bc46d8d8
---

## § 3. LE THÉORÈME DE HAHN-BANACH (FORME ANALYTIQUE)

### 1. Prolongement des formes linéaires positives

#### Proposition 1 {#evt-ii-s3-prop-1 .statement}

*Soient E un espace vectoriel préordonné, V un sous-espace vectoriel de E tel que tout élément de E soit majoré par un élément de V. Pour toute forme linéaire f sur V, positive pour la structure d’espace vectoriel préordonné de V (induite par celle de E), l’ensemble $ S_f $ des formes linéaires positives sur E qui prolongent f est non vide, et pour tout $ a \in E $, l’ensemble des valeurs $ h(a) $, où h parcourt $ S_f $, est l’intervalle $ [\alpha', \alpha''] $, où

$$
\alpha' = \sup_{z \in V, z \leq a} f(z), \quad \alpha'' = \inf_{y \in V, y \geq a} f(y).
$$

I) *Supposons d’abord* $ E = V + \mathbf{R}a $. La proposition étant triviale pour $ a \in V $, on peut se borner au cas $ a \notin V $. L’hypothèse faite sur V entraîne que l’ensemble

A'' des $ y \in V $ tels que $ a \leq y $ est non vide ; de même, l’ensemble $ A' $ des $ z \in V $ tels que $ -z \geq -a $ (autrement dit, $ z \leq a $) est non vide. En outre, pour $ v \in A'' $ et $ z \in A' $, on a $ z \leq a \leq v $, donc par hypothèse, $ f(z) \leq f(v) $. On en conclut que $ \alpha' $ et $ \alpha'' $ sont finis et que $ \alpha' \leq \alpha'' $. Toute forme linéaire $ f_1 $ sur $ E $ prolongeant $ f $ est entièrement déterminée par $ f_1(a) $, et pour tout $ \lambda \in \mathbf{R} $ et tout $ x \in V $, on a

$$
f_1(x + \lambda a) = f(x) + \lambda f_1(a) .
$$

Pour que $ f_1 $ soit positive, il faut et il suffit que les relations :

(2)
$$
x \in V , \quad \lambda \in \mathbf{R} , \quad x + \lambda a \geq 0
$$
entraînent :

(3)
$$
f(x) + \lambda f_1(a) \geq 0 .
$$

Comme $ f(\mu x) = \mu f(x) $ et que les relations $ x \geq 0 $ et $ \mu x \geq 0 $ sont équivalentes pour $ \mu > 0 $, il suffit d’exprimer que (2) entraîne (3) dans les cas particuliers $ \lambda = 0 $, $ \lambda = 1 $ et $ \lambda = -1 $. Pour $ \lambda = 0 $, le fait que (2) entraîne (3) résulte de l’hypothèse que $ f $ est positive. Pour $ \lambda = 1 $, dire que (2) entraîne (3) signifie que pour $ -x \in A' $, on a $ f_1(a) \geq f(-x) $, autrement dit que $ f_1(a) \geq \alpha' $; pour $ \lambda = -1 $, dire que (2) entraîne (3) signifie que, pour $ x \in A'' $, on a $ f(x) \geq f_1(a) $, autrement dit que $ f_1(a) \leq \alpha'' $. La proposition est donc démontrée dans ce cas.

II) *Cas général.* Soit $ \mathfrak{F} $ l’ensemble des couples $ (W, g) $, où $ W $ est un sous-espace vectoriel de $ E $ contenant $ V $ et $ g $ une forme linéaire positive sur $ W $ prolongeant $ f $. Ordonnons $ \mathfrak{F} $ en posant

$$
(W, g) \leq (W', g')
$$

si $ W \subset W' $ et si $ g' $ prolonge $ g $. Il est immédiat que $ \mathfrak{F} $ est inductif, et, en vertu du th. 2 de E, III, p. 20, il a donc un élément maximal $ (W_0, g_0) $. Supposons $ W_0 \neq E $. Il existe alors un vecteur $ b \notin W_0 $, et si $ W_1 = W_0 + \mathbf{R}b $, la première partie de la démonstration montre qu’il existe une forme linéaire positive sur $ W_1 $ qui prolonge $ g_0 $, ce qui contredit l’hypothèse que $ (W_0, g_0) $ est maximal ; on a donc $ W_0 = E $, ce qui prouve la première assertion de la proposition. Lorsque $ a \in V $, la seconde assertion est évidente, avec $ \alpha' = \alpha'' = f(a) $; si au contraire $ a \notin V $ et si l’on pose $ V_1 = V + \mathbf{R}a $, la seconde assertion résulte de la première partie de la démonstration.

#### Corollaire {#evt-ii-s3-n1-cor-1 .statement}

*Soient E un espace vectoriel topologique muni d’une structure de préordre compatible avec sa structure d’espace vectoriel, P l’ensemble des éléments $ \geq 0 $ de E. Soit V un sous-espace vectoriel de E contenant au moins un point intérieur $ x_0 $ de P. Alors toute forme linéaire positive sur V se prolonge en une forme linéaire positive sur E.*

Il suffit, en vertu de la prop. 1, de voir que, pour tout $ x \in E $, il existe $ x' \in V $ tel que $ x' - x \in P $. Or, soit U un voisinage de 0 dans E tel que $ x_0 + U \subset P $. On a donc $ x + x_0 + U \subset x + P $, et par suite, il existe $ \varepsilon $ tel que $ 0 < \varepsilon < 1 $ et que le point
$$
y = x_0 + (1 - \varepsilon)\, x
$$
appartienne à $ x + P $; par suite tout point de la forme $ x + \lambda(y - x) $ appartient à $ x + P $ pour $ \lambda > 0 $. Mais si l’on prend $ \lambda = 1/\varepsilon $, on a $ x + \lambda(y - x) = \lambda x_0 \in V $, d’où la conclusion.

La conclusion de ce corollaire ne subsiste pas nécessairement si l’on ne suppose pas que $ V $ contient un point intérieur de $ P $, même si $ E $ est de dimension finie et si $ P \cap V $ contient des points intérieurs *dans* $ V $ (II, p. 97, exerc. 25, *b*)).

### 2. Le théorème de Hahn-Banach (forme analytique)

**Théorème 1** (Hahn-Banach). — *Soient* $ E $ *un espace vectoriel*, $ p $ *une fonction sous-linéaire dans* $ E $. *Soit* $ V $ *un sous-espace vectoriel de* $ E $, *et soit* $ f $ *une forme linéaire sur* $ V $ *telle que, pour tout* $ y \in V $, *on ait* $ f(y) \leq p(y) $. *Alors il existe une forme linéaire* $ h $ *sur* $ E $ *prolongeant* $ f $ *et telle que, pour tout* $ x \in E $, *on ait* $ h(x) \leq p(x) $.

Dans l’espace vectoriel $ E_1 = E \times \mathbf{R} $, l’ensemble $ P $ des couples $ (x, a) $ tels que $ p(x) \leq a $ est un ensemble convexe (II, p. 18, prop. 19), et c’est évidemment un cône pointé. Soit $ V_1 $ le sous-espace $ V \times \mathbf{R} $ de $ E_1 $, et posons $ g(y, a) = -f(y) + a $ pour tout point $ (y, a) \in V_1 $. Alors $ g $ est une forme linéaire positive pour la structure de préordre sur $ V_1 $ définie par $ P \cap V_1 $; en effet, si $ (y, a) \in P \cap V_1 $, on a $ a \geq p(y) \geq f(y) $, donc $ g(y, a) \geq 0 $. D’autre part, soit $ (x, a) \in E_1 $; montrons que $ (x, a) $ est majoré par un point de $ V_1 $ pour le préordre défini par $ P $: en effet, dire qu’un point $ (x', a') \in V_1 $ est tel que $ (x, a) \leq (x', a') $ signifie que l’on a $ p(x' - x) \leq a' - a $, et prenant $ a' \geq p(-x) + a $, on voit que le point $ (0, a') $ de $ V_1 $ répond à la question. On peut donc appliquer la prop. 1 de II, p. 22, et il y a une forme linéaire $ u $ sur $ E_1 $ prolongeant $ g $ et positive pour le préordre défini par $ P $. On a donc $ u(0, 1) = g(0, 1) = 1 $ et par suite $ u $ est de la forme $ u(x, a) = -h(x) + a $, où $ h $ est une forme linéaire sur $ E $ prolongeant $ f $; en outre, pour tout $ x \in E $ et tout $ a \geq p(x) $, on a $ h(x) \leq a $, donc $ h(x) \leq p(x) $.

C.Q.F.D.

#### Corollaire 1 {#evt-ii-s3-prop-1-cor-1 .statement}

*Soient* $ p $ *une semi-norme sur un espace vectoriel* $ E $, $ V $ *un sous-espace vectoriel de* $ E $, $ f $ *une forme linéaire sur* $ V $ *telle que* $ |f(y)| \leq p(y) $ *pour tout* $ y \in V $. *Alors il existe une forme linéaire* $ h $ *sur* $ E $, *prolongeant* $ f $, *et telle que* $ |h(x)| \leq p(x) $ *pour tout* $ x \in E $.

Pour une semi-norme $ q $ et une forme linéaire $ g $ sur $ E $, les relations $ g \leq q $ et $ |g| \leq q $ sont équivalentes. Le corollaire résulte donc du th. 1.

#### Corollaire 2 {#evt-ii-s3-prop-1-cor-2 .statement}

*Soient* $ E $ *un espace vectoriel*, $ x_0 $ *un point de* $ E $, $ p $ *une semi-norme sur* $ E $; *il existe une forme linéaire* $ f $ *définie dans* $ E $, *telle que* $ f(x_0) = p(x_0) $ *et que* $ |f(x)| \leq p(x) $ *pour tout* $ x \in E $.

On applique le cor. 1 au sous-espace vectoriel $ V $ engendré par $ x_0 $ et à la forme linéaire $ \xi x_0 \mapsto \xi p(x_0) $ définie dans $ V $.

#### Corollaire 3 {#evt-ii-s3-prop-1-cor-3 .statement}

Soient E un espace normé, V un sous-espace vectoriel de E, f une forme linéaire continue dans V ; il existe une forme linéaire continue h définie dans E, prolongeant f, et de même norme (TG, X, p. 23).

On applique le cor. 1 en prenant $ p(x) = \|f\| \cdot \|x\| $, ce qui donne $ \|h\| \leq \|f\| $; d’autre part, on a évidemment $ \|h\| \geq \|f\| $, d’où le corollaire.

La conclusion du cor. 3 ne s’étend pas aux applications linéaires continues d’un espace normé dans un espace normé quelconque (IV, p. 55, exerc. 16, c) et V, p. 64, exerc. 22).

## EXERCICES {#evt-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
