---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 4
section_title: Le théorème de Banach-Steinhaus
lang: fr
source: evt-i-v-fr
book_pages: EVT III.24-EVT III.28, EVT III.44-EVT III.48
pdf_pages: 0159-0163, 0179-0183
extraction: ocr
subsections:
    - "no": 1
      title: Tonneaux et espaces tonnelés
      page: 24
      pdf_page: 159
    - "no": 2
      title: Le théorème de Banach-Steinhaus
      page: 25
      pdf_page: 160
    - "no": 3
      title: Parties bornées de $ \mathcal{L}(E ; F) $ (cas quasi-complet)
      page: 27
      pdf_page: 162
statements: 23
exercises: 22
content_sha256: af8195ba612f0792738a2a9d2c92a04335bd97100bc4ffc880dcd00a20a80a3f
---

## § 4. LE THÉORÈME DE BANACH-STEINHAUS

Dans ce paragraphe, on désigne par E un espace localement convexe et par E’ son dual. Lorsqu’on parle de topologie faible sur E’, il s’agit de $ \sigma(E', E) $.

### 1. Tonneaux et espaces tonnelés

#### Proposition 1 {#evt-iii-s4-prop-1 .statement}

Soit T une partie de E. Les conditions suivantes sont équivalentes :
(i) T est convexe, équilibré, fermé et absorbant.
(ii) T est le polaire d’un ensemble M convexe, équilibré et faiblement borné dans E’.
(iii) Il existe une semi-norme p sur E, semi-continue inférieurement, telle que T soit l’ensemble des $ x \in E $ satisfaisant à $ p(x) \leq 1 $.

(i) $ \Rightarrow $ (ii) : sous les hypothèses de (i), posons $ M = T^\circ $; alors M est convexe et équilibré dans E’. Pour tout $ x \in E $, il existe un nombre réel $ r > 0 $ tel que $ r.x \in T $, d’où $ |u(x)| \leq \frac{1}{r} $ pour tout $ u \in M $; autrement dit, M est faiblement borné. D’après le cor. 3 de II, p. 49, on a $ T = M^\circ $, donc T satisfait à (ii).

(ii) $ \Rightarrow $ (iii) : sous les hypothèses de (ii), posons $ p(x) = \sup_{u \in M} |u(x)| $ pour tout $ x \in E $.

Il est immédiat que $ T = M^\circ $ se compose des $ x \in E $ tels que $ p(x) \leq 1 $. La semi-norme p sur E’ est semi-continue inférieurement, comme enveloppe supérieure d’une famille de fonctions continues (TG, IV, p. 31, corollaire).

(iii) $ \Rightarrow $ (i) : c’est clair.

#### Corollaire {#evt-iii-s4-n1-cor-1 .statement}

Les conditions suivantes sont équivalentes :
(i) toute partie faiblement bornée de E’ est équicontinue ;
(ii) tout ensemble convexe, équilibré, fermé et absorbant dans E est un voisinage de 0 ;
(iii) toute semi-norme semi-continue inférieurement dans E est continue.

#### Définition 1 {#evt-iii-s4-def-1 .statement}

On appelle tonneau dans E tout ensemble T satisfaisant aux conditions équivalentes de la prop. 1.

#### Définition 2 {#evt-iii-s4-def-2 .statement}

On dit que l’espace E est tonnelé s’il satisfait aux conditions équivalentes du corollaire de la prop. 1.

On sait (III, p. 22, prop. 9) que toute partie équicontinue du dual E’ de E est fortement et faiblement bornée. On peut donc traduire la définition des espaces tonnelés de la manière suivante :

#### Scholie {#evt-iii-s4-n1-sch-1 .statement}

Dans le dual d’un espace tonnelé, il y a identité entre ensembles équicontinus, ensembles fortement bornés, ensembles faiblement bornés et ensembles relativement compacts pour la topologie faible. Si E est tonnelé et séparé et si $ E'_b $ est son dual fort, les polaires des voisinages de 0 dans l’un de ces espaces forment une base de la bornologie canonique de l’autre, et les polaires des parties bornées de l’un de ces espaces forment une base du filtre des voisinages de 0 de l’autre.

#### Proposition 2 {#evt-iii-s4-prop-2 .statement}

Tout espace localement convexe E qui est un espace de Baire (TG, IX, p. 54) est tonnelé.

En effet, soit T un tonneau dans E ; comme T est absorbant, E est réunion des ensembles fermés $ nT $ ($ n $ entier $ > 0 $) ; puisque E est un espace de Baire, un au moins de ces ensembles admet un point intérieur, donc T lui-même admet un point intérieur x. Si $ x \neq 0 $, comme on a $ -x \in T $ et que 0 est un point du segment ouvert d’extrémités x et $ -x $, 0 est un point intérieur de l’ensemble convexe T (II, p. 15, prop. 16). Donc T est un voisinage de 0.

#### Corollaire {#evt-iii-s4-n1-cor-2 .statement}

Tout espace de Fréchet (et en particulier tout espace de Banach) est tonnelé.

Cela résulte du th. de Baire (TG, IX, p. 55, th. 1).

#### Proposition 3 {#evt-iii-s4-prop-3 .statement}

Soit $ (F_i)_{i \in I} $ une famille d’espaces tonnelés, et pour chaque $ i \in I $, soit $ f_i $ une application linéaire de $ F_i $ dans un espace vectoriel E. L’espace E, muni de la topologie localement convexe la plus fine rendant continues les $ f_i $ (II, p. 29, prop. 5), est un espace tonnelé.

En effet, soit T un tonneau dans E. Comme $ f_i $ est continue, $ f_i^{-1}(T) $ est un ensemble convexe, fermé, équilibré et absorbant dans $ F_i $, autrement dit un tonneau dans $ F_i $; comme $ F_i $ est tonnelé, $ f_i^{-1}(T) $ est un voisinage de 0 dans $ F_i $, pour tout $ i \in I $, ce qui entraîne que T est un voisinage de 0 dans E (II, p. 29, prop. 5).

#### Corollaire 1 {#evt-iii-s4-prop-3-cor-1 .statement}

Tout espace quotient d’un espace tonnelé est tonnelé.

#### Corollaire 2 {#evt-iii-s4-prop-3-cor-2 .statement}

Soit $ (E_i)_{i \in I} $ une famille d’espaces localement convexes, et soit E la somme directe topologique de cette famille. Pour que E soit tonnelé, il faut et il suffit que chacun des $ E_i $ le soit.

La condition est évidemment suffisante en vertu de la prop. 3 ; elle est nécessaire d’après le cor. 1, puisque chacun des $ E_i $ est isomorphe à un espace quotient de E (II, p. 33, prop. 8).

#### Corollaire 3 {#evt-iii-s4-prop-3-cor-3 .statement}

Toute limite inductive d’espaces tonnelés est un espace tonnelé.

On prouvera plus loin (IV, p. 14, corollaire) que tout produit d’espaces tonnelés est tonnelé.

### 2. Le théorème de Banach-Steinhaus

#### Théorème 1 {#evt-iii-s4-thm-1 .statement}

Soient E un espace tonnelé, F un espace localement convexe. Toute partie simplement bornée H de $ \mathscr{L}(E; F) $ est équicontinue.

En effet, soit $ p $ une semi-norme continue sur $ F $; posons $ q = \sup_{u \in H} (p \circ u) $. Puisque $ H $ est simplement bornée, on a $ q(x) < +\infty $ pour tout $ x \in E $ et $ q $ est une semi-norme semi-continue inférieurement, comme enveloppe supérieure finie de semi-normes continues. Comme $ E $ est tonnelé, $ q $ est une semi-norme continue et $ H $ est donc équicontinue.

#### Corollaire 1 {#evt-iii-s4-thm-1-cor-1 .statement}

*Soient* $ E $ et $ F $ *des espaces de Banach*, $ H $ *un ensemble d’applications linéaires continues de* $ E $ *dans* $ F $; *si, pour tout* $ x \in E $, *on a* $ \sup_{u \in H} \|u(x)\| < +\infty $, *on a aussi* $ \sup_{u \in H} \|u\| < +\infty $.

En effet, l’hypothèse signifie que $ H $ est simplement bornée et la conclusion qu’elle est équicontinue. De plus, tout espace de Banach est tonnelé (III, p. 25).

#### Corollaire 2 (théorème de Banach-Steinhaus) {#evt-iii-s4-thm-1-cor-2 .statement}

*Soient* $ E $ *un espace tonnelé*, $ F $ *un espace localement convexe séparé et* $ (u_n) $ *une suite d’applications linéaires continues de* $ E $ *dans* $ F $, *convergeant simplement vers une application* $ u $ *de* $ E $ *dans* $ F $. *Alors on a* $ u \in \mathcal{L}(E; F) $, *et* $ (u_n) $ *converge vers* $ u $ *uniformément sur toute partie précompacte de* $ E $.

La suite $ (u_n) $ est en effet simplement bornée, donc équicontinue et le corollaire résulte du cor. à la prop. 5 de III, p. 18.

#### Remarque 1 {#evt-iii-s4-n2-rem-1 .statement}

La propriété exprimée par le cor. 2 n’entraîne pas que $ E $ soit tonnelé : nous verrons plus loin que le dual fort d’un espace de Fréchet la possède, bien que n’étant pas nécessairement tonnelé (IV, p. 22, corollaire et p. 58, exerc. 5).
2) Soient $ E $ et $ F $ deux espaces de Banach et soit $ (u_n) $ une suite d’applications linéaires continues de $ E $ dans $ F $ telle que $ \sup \|u_n\| = +\infty $. L’ensemble $ X $ des $ x \in E $ tels que $ \sup \|u_n(x)\| = +\infty $ est alors *dense* dans $ E $ et est l’intersection d’une suite d’ouverts de $ E $. En effet, notons $ X_k $ l’ensemble des $ x \in E $ tels que $ \sup \|u_n(x)\| > k $ (pour $ k $ entier $ > 0 $). Chaque $ X_k $ est ouvert et $ X $ est l’intersection des $ X_k $. Comme $ E $ est un espace de Baire, il suffit de montrer que chaque $ X_k $ est dense dans $ E $. Or si le complémentaire de $ X_k $ contenait un ouvert non vide $ U $, on aurait $ \|u_n(x)\| \leq 2k $ pour $ x \in U - U $ et, comme $ U - U $ est un voisinage de $ 0 $, on aurait $ \sup \|u_n\| < +\infty $.

#### Corollaire 3 {#evt-iii-s4-thm-1-cor-3 .statement}

*Soient* $ E $ *un espace tonnelé*, $ F $ *un espace localement convexe séparé*, $ \Phi $ *un filtre sur* $ \mathcal{L}(E; F) $ *qui converge simplement dans* $ E $ *vers une application* $ u $ *de* $ E $ *dans* $ F $. *Si* $ \Phi $ *contient une partie simplement bornée de* $ \mathcal{L}(E; F) $ *ou si* $ \Phi $ *admet une base dénombrable*, $ u $ *est une application linéaire continue de* $ E $ *dans* $ F $, *et* $ \Phi $ *converge uniformément vers* $ u $ *dans toute partie précompacte de* $ E $.

Supposons d’abord que $ \Phi $ contienne un ensemble simplement borné $ H $; comme $ H $ est équicontinu (th. 1), le corollaire résulte du cor. de la prop. 5 (III, p. 18). Si $ \Phi $ admet une base dénombrable, tout filtre élémentaire $ \Psi $ associé à une suite $ (u_n) $ (TG, I, p. 42) plus fin que $ \Phi $ est alors simplement convergent dans $ E $ vers $ u $ et il résulte du cor. 2 que $ u $ est une application linéaire continue de $ E $ dans $ F $, et que $ \Psi $ converge vers $ u $ pour la topologie de la convergence uniforme dans les parties précompactes de $ E $. Par suite, il en est de même de $ \Phi $, puisque ce dernier est l’intersection des filtres élémentaires plus fins que lui (TG, I, p. 43).

On notera qu’un filtre sur $ \mathcal{L}(E; F) $, qui converge simplement et admet une base dénombrable, ne contient pas nécessairement un ensemble simplement borné : c’est ce que montre l’exemple du filtre des voisinages de 0 dans $ F = \mathcal{L}(K ; F) $ lorsque la topologie de $ F $ est métrisable mais ne peut être définie par une seule norme.

#### Exemple {#evt-iii-s4-n2-exa-1 .statement}

Soit $ E $ l’espace de Banach (sur $ \mathbf{C} $) formé des fonctions complexes continues et de période 1 dans $ \mathbf{R} $, avec la norme $ \|f\| = \sup_x |f(x)| $.

Pour tout entier $ n \in \mathbf{Z} $ et toute fonction $ f \in E $, posons $ c_n(f) = \int_0^1 f(x)\ e^{-2i\pi nx} dx $ ($ n $-ième coefficient de Fourier de $ f $) ; chacune des applications $ f \mapsto c_n(f) $ est une forme linéaire continue sur $ E $. Soit $ (\alpha_n) $ une suite de nombres complexes telle que, pour toute fonction $ f \in E $, la série de terme général $ \alpha_n c_n(f) + \alpha_{-n} c_{-n}(f) $ soit convergente. Dans ces conditions, l’application $ u : f \mapsto \alpha_0 c_0(f) + \sum_{n \geq 1} [\alpha_0 c_n(f) + \alpha_{-n} c_{-n}(f)] $ est une forme linéaire continue sur $ E $ ; \* autrement dit, il existe une mesure $ \mu $ sur $[0, 1]$ telle que $ u(f) = \int f(x)\ d\mu(x) $ pour toute fonction $ f \in E $, ou encore que $ \alpha_{-n} $ soit le $ n $-ième coefficient de Fourier de $ \mu $. \* En effet, pour tout entier $ m > 0 $, l’application $ f \mapsto \sum_{k = -m}^m \alpha_k c_k(f) $ est une forme linéaire continue $ u_m $ sur $ E $, et pour toute $ f \in E $, la suite $ (u_m(f)) $ converge vers $ u(f) $ par hypothèse. L’assertion résulte donc du th. de Banach-Steinhaus, puisque $ E $ est tonnelé.

#### Corollaire 4 {#evt-iii-s4-thm-1-cor-4 .statement}

*Soient $ E $ et $ F $ deux espaces localement convexes, $ \mathfrak{S} $ un recouvrement de $ E $ formé de parties bornées. Si $ E $ est tonnelé et si $ F $ est séparé et quasi-complet, l’espace $ \mathcal{L}_{\mathfrak{S}}(E ; F) $ est séparé et quasi-complet.*

En effet, toute partie bornée et fermée de $ \mathcal{L}_{\mathfrak{S}}(E ; F) $ est simplement bornée (puisque $ \mathfrak{S} $ est un recouvrement de $ E $), donc équicontinue (III, p. 25, th. 1) et par suite est un sous-espace complet de $ \mathcal{L}_{\mathfrak{S}}(E ; F) $ en vertu de la prop. 11 (III, p. 22).

#### Corollaire 5 {#evt-iii-s4-thm-1-cor-5 .statement}

*Le dual fort et le dual faible d’un espace tonnelé sont quasi-complets.*

### 3. Parties bornées de $ \mathcal{L}(E ; F) $ (cas quasi-complet)

#### Théorème 2 {#evt-iii-s4-thm-2 .statement}

*Soient $ E $ un espace localement convexe séparé, $ F $ un espace localement convexe, $ \mathfrak{S} $ l’ensemble des parties de $ E $ convexes, équilibrées, bornées, fermées et semi-complètes (III, p. 7). Toute partie simplement bornée $ H $ de $ \mathcal{L}(E ; F) $ est bornée pour la $ \mathfrak{S} $-topologie.*

Soit $ A \in \mathfrak{S} $. L’espace $ E_A $ est alors un espace de Banach (III, p. 8, corollaire), donc tonnelé. D’autre part, l’image canonique de $ H $ dans $ \mathcal{L}(E_A ; F) $ est simplement bornée, donc équicontinue (III, p. 25, th. 1). Par suite, l’ensemble des $ u(x) $ pour $ u \in H $ et $ x \in A $ est borné dans $ F $, ce qui montre que $ H $ est bornée pour la $ \mathfrak{S} $-topologie.

#### Corollaire 1 {#evt-iii-s4-thm-2-cor-1 .statement}

*Soient $ E $ un espace localement convexe séparé, $ F $ un espace localement convexe, et $ \mathfrak{S} $ un ensemble de parties bornées de $ E $. Si $ E $ est semi-complet, toute partie simplement bornée de $ \mathcal{L}(E ; F) $ est bornée pour la $ \mathfrak{S} $-topologie.*

Il suffit d’appliquer le th. 2, quitte à remplacer les ensembles de $ \mathcal{S} $ par leurs enveloppes convexes fermées, équilibrées, ce qui ne change pas la $ \mathcal{S} $-topologie.

Lorsque E est semi-complet (par exemple quasi-complet), on peut donc parler de parties bornées de $ \mathcal{L}(E ; F) $ sans préciser pour quelle $ \mathcal{S} $-topologie, puisque celles-ci sont les mêmes pour toutes les $ \mathcal{S} $-topologies dès que $ \mathcal{S} $ est un recouvrement de E.

#### Corollaire 2 {#evt-iii-s4-thm-2-cor-2 .statement}

Tout espace bornologique semi-complet est tonnelé.

Toute partie simplement bornée de son dual est fortement bornée (cor. 1), donc équicontinue (III, p. 22, prop. 10).

#### Corollaire 3 {#evt-iii-s4-thm-2-cor-3 .statement}

Soit E un espace localement convexe. Toute partie de E bornée pour $ \sigma(E, E') $ est bornée.

Soit A une partie de E. Dire que A est bornée pour $ \sigma(E, E') $ signifie que toute forme linéaire continue sur E est bornée sur A ; dire que A est bornée signifie que toute semi-norme continue sur E est bornée sur A. Soit N l’adhérence de 0 dans E et soit $ \pi $ l’application canonique de E sur E/N. Les formes linéaires continues sur E sont les applications de la forme $ f \circ \pi $ avec $ f \in (E/N)' $ et l’on a une caractérisation analogue des semi-normes continues sur E. Quitte à remplacer E par E/N et A par $ \pi(A) $, on peut donc se limiter au cas où E est séparé.

Soit $ \mathcal{S} $ l’ensemble des parties équicontinues de E’ ; lorsque E’ est muni de $ \sigma(E', E) $, E s’identifie à $ (E')_{\mathcal{S}} $ (III, p. 19, cor. 1). Toute partie équicontinue fermée de E’ est compacte pour $ \sigma(E', E) $ (III, p. 17, cor. 2), donc complète pour $ \sigma(E', E) $. Il suffit donc d’appliquer le th. 2.

## EXERCICES {#evt-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
