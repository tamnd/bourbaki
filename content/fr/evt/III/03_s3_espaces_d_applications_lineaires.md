---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 3
section_title: Espaces d’applications linéaires continues
lang: fr
source: evt-i-v-fr
book_pages: EVT III.13-EVT III.24, EVT III.42-EVT III.44
pdf_pages: 0148-0159, 0177-0179
extraction: ocr
subsections:
    - "no": 1
      title: Les espaces $ \mathcal{L}_\mathfrak{S}(E; F) $
      page: 13
      pdf_page: 148
    - "no": 2
      title: Condition pour que $ \mathcal{L}_{\mathfrak{S}}(E; F) $ soit séparé
      page: 15
      pdf_page: 150
    - "no": 3
      title: Relations entre $ \mathcal{L}(E ; F) $ et $ \mathcal{L}(\hat{E} ; F) $
      page: 16
      pdf_page: 151
    - "no": 4
      title: Parties équicontinues de $ \mathcal{L}(E ; F) $
      page: 16
      pdf_page: 151
    - "no": 5
      title: Parties équicontinues de $ E' $
      page: 19
      pdf_page: 154
    - "no": 6
      title: Le complété d’un espace localement convexe
      page: 20
      pdf_page: 155
    - "no": 7
      title: $ \mathcal{S}$-bornologies sur $ \mathcal{L}(E ; F) $
      page: 22
      pdf_page: 157
    - "no": 8
      title: Parties complètes de $ \mathcal{L}_{\mathcal{S}}(E ; F) $
      page: 22
      pdf_page: 157
statements: 40
exercises: 13
content_sha256: 267b87ed593a4827b22d801ba8f77379a0ccb0929a65f3ed1ef65849c5a25afa
---

## § 3. ESPACES D’APPLICATIONS LINÉAIRES CONTINUES

### 1. Les espaces $ \mathcal{L}_\mathfrak{S}(E; F) $

Soient $ F $ un espace vectoriel topologique, $ E $ un ensemble quelconque et $ \mathfrak{S} $ une famille de parties de $ E $. Considérons l’espace vectoriel $ F^E $ muni de la structure uniforme de la $ \mathfrak{S} $-convergence (TG, X, p. 2). On sait que cette structure uniforme est compatible avec la structure de groupe commutatif de $ F^E $ (TG, X, p. 6, cor. 2). La topologie qu’on en déduit s’appelle la $ \mathfrak{S}\text{-topologie} $. Si $ X $ est une partie de $ F^E $ ou plus généralement un ensemble muni d’une application $ j : X \to F^E $, on appelle $ \mathfrak{S}\text{-topologie} $ sur $ X $ l’image réciproque par $ j $ de la $ \mathfrak{S}\text{-topologie} $ sur $ F^E $.

#### Remarque 1 {#evt-iii-s3-n1-rem-1 .statement}

La $ \mathfrak{S}\text{-topologie} $ est identique à la $ \mathfrak{S}'\text{-topologie} $, où $ \mathfrak{S}' $ désigne la bornologie engendrée par $ \mathfrak{S} $ (III, p. 1).
2) Soit $ M \in \mathfrak{S} $ et soit $ V $ un voisinage de 0 dans $ F $; notons $ T(M, V) $ l’ensemble des $ f \in F^E $ telles que $ f(x) \in V $ pour tout $ x \in M $. Si $ \mathfrak{S} $ est stable par réunion finie, les ensembles $ T(M, V) $ forment un système fondamental de voisinages de 0 pour la $ \mathfrak{S}\text{-topologie} $ de $ F^E $.

#### Proposition 1 {#evt-iii-s3-prop-1 .statement}

*Soient E un ensemble, $ \mathfrak{S} $ un ensemble de parties de E, F un espace vectoriel topologique, H un sous-espace vectoriel de $ F^E $. Pour que la $ \mathfrak{S}\text{-topologie} $ soit compatible avec la structure d’espace vectoriel de H, il faut et il suffit que, pour tout $ u \in H $ et tout $ M \in \mathfrak{S} $, $ u(M) $ soit borné dans F. Si, en outre, F est localement convexe, la $ \mathfrak{S}\text{-topologie} $ sur H est localement convexe.*

Compte tenu des remarques 1) et 2) ci-dessus, on voit qu’une condition nécessaire et suffisante pour que la $ \mathfrak{S}\text{-topologie} $ soit compatible avec la structure d’espace vectoriel de H est que les ensembles $ H \cap T(M, V) $ soient *absorbants* dans H (I, p. 7, prop. 4) ; or cela signifie que, pour tout $ u \in H $, toute partie $ M \in \mathfrak{S} $ et tout voisinage équilibré $ V $ de 0 dans $ F $, il existe $ \lambda \neq 0 $ tel que $ u(M) \subset \lambda V $, c’est-à-dire (III, p. 2) que $ u(M) $ soit bornée dans $ F $. Enfin la dernière assertion de la proposition résulte de ce que, si $ V $ est convexe, il en est de même de $ T(M, V) $.

#### Corollaire {#evt-iii-s3-n1-cor-1 .statement}

*Soient E et F deux espaces localement convexes, $ \mathfrak{S} $ un ensemble de parties bornées de E, $ \mathcal{L}(E; F) $ l’espace vectoriel des applications linéaires continues de E dans F. La $ \mathfrak{S}\text{-topologie} $ est compatible avec la structure d’espace vectoriel de $ \mathcal{L}(E; F) $; elle est localement convexe.*

Il suffit de remarquer que, si $ u $ est une application linéaire continue de E dans F et M une partie bornée de E, $ u(M) $ est bornée dans F (III, p. 4, cor. 1).

Étant donnés deux espaces vectoriels localement convexes E et F, et un ensemble $ \mathcal{S} $ de parties bornées de E, nous désignerons par $ \mathcal{L}_{\mathcal{S}}(E ; F) $ l’espace localement convexe obtenu en munissant $ \mathcal{L}(E ; F) $ de la $ \mathcal{S} $-topologie.

#### Exemple 1 {#evt-iii-s3-n1-exa-1 .statement}

$ \mathcal{S} $ est l’ensemble des parties finies de E ; la $ \mathcal{S} $-topologie est alors la topologie de la convergence simple et l’espace $ \mathcal{L}_{\mathcal{S}}(E ; F) $ est aussi noté $ \mathcal{L}_s(E ; F) $. Une partie bornée de $ \mathcal{L}_s(E ; F) $ est appelée une partie simplement bornée de $ \mathcal{L}(E ; F) $.

#### Exemple 2 {#evt-iii-s3-n1-exa-2 .statement}

$ \mathcal{S} $ est l’ensemble des parties compactes (resp. précompactes, convexes compactes). La $ \mathcal{S} $-topologie est alors appelée la topologie de la convergence compacte (resp. précompacte, convexe compacte) et l’espace $ \mathcal{L}_{\mathcal{S}}(E ; F) $ est aussi noté $ \mathcal{L}_c(E ; F) $ (resp. $ \mathcal{L}_{pc}(E ; F) $, $ \mathcal{L}_{cc}(E ; F) $). (Cf. IV, p. 48, exerc. 7.)

#### Exemple 3 {#evt-iii-s3-n1-exa-3 .statement}

Si $ \mathcal{S} $ est l’ensemble de toutes les parties bornées de E, on dit que la $ \mathcal{S} $-topologie est la topologie de la convergence bornée, et l’espace $ \mathcal{L}_{\mathcal{S}}(E ; F) $ est noté $ \mathcal{L}_b(E ; F) $.

#### Exemple 4 {#evt-iii-s3-n1-exa-4 .statement}

Lorsque $ F = K $, l’espace $ \mathcal{L}(E ; F) $ est le dual $ E' $ de E. On note alors $ E'_\mathcal{S} $, $ E'_s $, etc. l’espace $ \mathcal{L}_{\mathcal{S}}(E ; K) $, $ \mathcal{L}_s(E ; K) $, etc. L’espace $ E'_s $ (resp. $ E'_b $) est appelé le dual faible (resp. le dual fort) de E. Une partie bornée de $ E'_s $ (resp. $ E'_b $) est dite faiblement (resp. fortement) bornée. On notera que la topologie faible sur $ E' $ n’est autre que $ \sigma(E', E) $ (II, p. 45).

Lorsque $ E = F $, on note $ \mathcal{L}(E) $, $ \mathcal{L}_{\mathcal{S}}(E) $, etc. l’espace $ \mathcal{L}(E ; E) $, $ \mathcal{L}_{\mathcal{S}}(E ; E) $, etc.

Soient $ p $ une semi-norme continue sur F, et M une partie bornée de E. Posons

$$
p_M(u) = \sup_{x \in M} p(u(x)) .
$$

Il est immédiat que $ p_M $ est une semi-norme sur $ \mathcal{L}(E ; F) $ et que si $ \Gamma $ est un système fondamental de semi-normes sur F, la famille des semi-normes $ p_M $, où $ p $ parcourt $ \Gamma $ et M parcourt une base de la bornologie engendrée par $ \mathcal{S} $, est un système fondamental de semi-normes de $ \mathcal{L}_{\mathcal{S}}(E ; F) $.

En particulier, si E et F sont des espaces semi-normés, et si l’on note $ p $ (resp. $ q $) la semi-norme de E (resp. F), la topologie de la convergence bornée sur $ \mathcal{L}(E ; F) $ est définie par la semi-norme

$$
r(u) = \sup_{p(x) \leq 1} q(u(x))
$$

(cf. TG, X, p. 21 à 24). Lorsqu’on considère $ \mathcal{L}_b(E ; F) $ comme un espace semi-normé, c’est toujours de la semi-norme (2) qu’il est question sauf mention expresse du contraire. Si F est un espace normé, la semi-norme (2) est une norme.

#### Remarque 3 {#evt-iii-s3-n1-rem-3 .statement}

Soit A une partie dense de la boule unité de E. Vu la continuité de $ u $, on a aussi

$$
r(u) = \sup_{x \in A} q(u(x)) .
$$

Par exemple

$$
r(u) = \sup_{p(x) < 1} q(u(x)) .
$$

Comme on a $ u(tx) = tu(x) $ pour $ t \in \mathbf{R} $, on a aussi, dès que $ E \neq \{0\} $ :

$$
r(u) = \sup_{p(x)=1} q(u(x)) = \sup_{p(x) \neq 0} \frac{q(u(x))}{p(x)}.
$$

#### Remarque 4 {#evt-iii-s3-n1-rem-4 .statement}

La formule (2) montre que l’application $ u \mapsto r(u) $ est semi-continue inférieurement sur $ \mathcal{L}_s(E; F) $.

#### Proposition 2 {#evt-iii-s3-prop-2 .statement}

*Soient E et F deux espaces localement convexes, et soit $ \mathfrak{S} $ un ensemble de parties bornées de E.*

1) *Sur $ \mathcal{L}(E; F) $, la $ \mathfrak{S} $-topologie est identique à la $ \tilde{\mathfrak{S}} $-topologie, où $ \tilde{\mathfrak{S}} $ désigne la plus petite bornologie adaptée (III, p. 3) à E contenant $ \mathfrak{S} $.*

2) *Supposons que $ \{0\} $ ne soit pas dense dans F et soit $ \mathfrak{S}' $ un autre ensemble de parties bornées de E. Pour que la $ \mathfrak{S}' $-topologie soit moins fine que la $ \mathfrak{S} $-topologie, il faut et il suffit que l’on ait $ \mathfrak{S}' \subset \tilde{\mathfrak{S}} $.*

Soient $ u \in \mathcal{L}(E; F) $, $ M \in \mathfrak{S} $, et soit $ p $ une semi-norme continue sur F. Comme $ p \circ u $ est une semi-norme continue sur E, il est équivalent de dire que $ p \circ u $ est majorée par 1 dans M ou dans l’enveloppe fermée convexe équilibrée $ \tilde{M} $ de M ; autrement dit, on a $ p_M = p_{\tilde{M}} $. En outre, il est clair qu’on a $ p_{\lambda M} = \lambda p_M $ pour $ \lambda > 0 $ et $ p_{M \cup M'} = \sup(p_M, p_{M'}) $, d’où la première assertion puisque $ \tilde{\mathfrak{S}} $ admet pour base l’ensemble des homothétiques des enveloppes convexes équilibrées fermées de réunions finies d’ensembles de $ \mathfrak{S} $.

Démontrons la deuxième assertion : tout d’abord, si F est le corps de base, il résulte de la définition que la $ \tilde{\mathfrak{S}} $-topologie sur $ E' = \mathcal{L}(E; F) $ admet pour système fondamental de voisinages de 0 l’ensemble des polaires des ensembles de $ \tilde{\mathfrak{S}} $. Soit A une partie bornée de E, dont le polaire $ A^\circ $ est un voisinage de 0 pour la $ \tilde{\mathfrak{S}} $-topologie ; il existe donc $ B \in \tilde{\mathfrak{S}} $ fermé, convexe et équilibré tel que $ A^\circ \supset B^\circ $, d’où $ A \subset B^{\circ \circ} $; mais d’après le cor. 3 de II, p. 49, on a $ B^{\circ \circ} = B $, d’où $ A \subset B $, et $ A \in \tilde{\mathfrak{S}} $. Donc, si $ \mathfrak{S}' $ est un ensemble de parties bornées de E, la $ \mathfrak{S}' $-topologie est moins fine que la $ \mathfrak{S} $-topologie sur $ E' $ si et seulement si $ \mathfrak{S}' \subset \tilde{\mathfrak{S}} $. Le cas général en résulte aussitôt, car si $ y \in F $ n’est pas adhérent à 0, on vérifie immédiatement que l’application qui à $ f \in E' $ fait correspondre l’application $ x \mapsto f(x) y $ est un isomorphisme d’espaces localement convexes de $ E_{\mathfrak{S}'} $ sur son image dans $ \mathcal{L}_{\mathfrak{S}}(E; F) $.

### 2. Condition pour que $ \mathcal{L}_{\mathfrak{S}}(E; F) $ soit séparé

#### Proposition 3 {#evt-iii-s3-prop-3 .statement}

*Soient E et F deux espaces localement convexes, F étant supposé séparé, et soit $ \mathfrak{S} $ un ensemble de parties bornées de E. Si la réunion A des ensembles de $ \mathfrak{S} $ est totale dans E, l’espace $ \mathcal{L}_{\mathfrak{S}}(E; F) $ est séparé.*

Soit $ u_0 $ un élément non nul de $ \mathcal{L}(E; F) $; comme $ u_0 $ est continue et A totale dans E, il existe $ x_0 $ dans A tel que $ u_0(x_0) \neq 0 $. Comme F est séparé, il existe un voisinage V de 0 dans F tel que $ u_0(x_0) \notin V $. Soit $ M \in \mathfrak{S} $ tel que $ x_0 \in M $. Alors l’ensemble U des $ u \in \mathcal{L}(E; F) $ telles que $ u(M) \subset V $ est un voisinage de 0 dans $ \mathcal{L}(E; F) $ et l’on a $ u_0 \notin U $, donc $ \mathcal{L}(E; F) $ est séparé.

En particulier, sur $ \mathcal{L}(E ; F) $ les topologies suivantes sont séparées dès que F est séparé : la convergence simple, la convergence compacte, précompacte ou convexe compacte, et la convergence bornée.

### 3. Relations entre $ \mathcal{L}(E ; F) $ et $ \mathcal{L}(\hat{E} ; F) $

Soient E et F deux espaces localement convexes séparés, et supposons F complet ; soit $ \hat{E} $ le complété de E. Comme toute application linéaire continue $ u $ de E dans F se prolonge d’une seule manière en une application linéaire continue $ \bar{u} $ de $ \hat{E} $ dans F, on peut identifier par l’application $ u \mapsto \bar{u} $ les espaces $ \mathcal{L}(E ; F) $ et $ \mathcal{L}(\hat{E} ; F) $. Soit de plus $ \mathfrak{S} $ un ensemble de parties bornées de E ; la $ \mathfrak{S} $-topologie sur $ \mathcal{L}(E ; F) $ coïncide avec la $ \mathfrak{S} $-topologie sur $ \mathcal{L}(\hat{E} ; F) $, et aussi avec la $ \hat{\mathfrak{S}} $-topologie, où $ \hat{\mathfrak{S}} $ désigne l’ensemble des adhérences dans $ \hat{E} $ des ensembles de $ \mathfrak{S} $.

Par exemple, si E est normé, la topologie de la convergence bornée sur $ \mathcal{L}(E ; F) $ s’identifie à la topologie de la convergence bornée sur $ \mathcal{L}(\hat{E} ; F) $ : en effet, toute partie bornée de $ \hat{E} $ est contenue dans l’adhérence d’une partie bornée de E. Comme la boule unité de $ \hat{E} $ est l’adhérence de la boule unité de E, il résulte de la formule (3) (III, p. 14) que si F est un espace de Banach, l’application $ u \mapsto \bar{u} $ est une isométrie de $ \mathcal{L}(E ; F) $ sur $ \mathcal{L}(\hat{E} ; F) $.

On notera que si E n’est pas un espace normé, il peut arriver qu’il existe des parties bornées de $ \hat{E} $ qui ne sont contenues dans l’adhérence d’aucune partie bornée de E (c’est le cas par exemple si E est le dual faible d’un espace de Banach de dimension infinie) ; il en est cependant ainsi si E est métrisable, de type dénombrable (III, p. 41, exerc. 16).

### 4. Parties équicontinues de $ \mathcal{L}(E ; F) $

Soient E et F deux espaces localement convexes. Pour qu’une partie H de $ \mathcal{L}(E ; F) $ soit équicontinue, il faut et il suffit qu’elle soit équicontinue au point 0 de E (I, p. 9, prop. 6) ; cela signifie que pour tout voisinage V de 0 dans F, l’ensemble $ \bigcap_{u \in H} u^{-1}(V) $ est un voisinage de 0 dans E, ou encore que pour toute semi-norme continue $ p $ sur F, la fonction $ \sup_{u \in H} (p \circ u) $ est une semi-norme continue sur E. De plus (I, p. 5), H est uniformément équicontinue. Notons que l’enveloppe convexe équilibrée d’une partie équicontinue est équicontinue puisque, si $ p $ est une semi-norme continue sur F, et $ \tilde{H} $ l’enveloppe convexe équilibrée de H, on a, pour des $ u_i $ dans H, l’inégalité $ p \circ (\sum \lambda_i u_i) \leq \sum |\lambda_i| \cdot (p \circ u_i) $, donc $ \sup_{u \in H} (p \circ u) = \sup_{u \in \tilde{H}} (p \circ u) $.

Par suite, l’ensemble des parties équicontinues est une bornologie convexe sur $ \mathcal{L}(E ; F) $ (III, p. 2, déf. 2).

#### Proposition 4 {#evt-iii-s3-prop-4 .statement}

Soient E, F deux espaces localement convexes, F étant supposé séparé. Munissons l’espace $ F^E $ de toutes les applications de E dans F de la topologie de la convergence simple.

(i) L’ensemble des applications linéaires de E dans F est fermé dans $ F^E $.

(ii) Si H est une partie équicontinue de $ \mathcal{L}(E; F) $, l’adhérence $ \overline{H} $ de H dans $ F^E $ est contenue dans $ \mathcal{L}(E; F) $ et est équicontinue.

On sait que $ \overline{H} $ est équicontinue (TG, X, p. 15). Tout revient à prouver l’assertion (i). Soient x, y dans E et $ \lambda, \mu $ dans K, et soit $ A(x, y, \lambda, \mu) $ l’ensemble des $ u \in F^E $ telles que

$$
u(\lambda x + \mu y) - \lambda u(x) - \mu u(y) = 0 .
$$

Cet ensemble est fermé dans $ F^E $ puisque l’application $ u \mapsto u(x) $ de $ F^E $ dans F est continue pour tout $ x \in E $ et que F est séparé. Or l’ensemble des applications linéaires de E dans F est égal à

$$
\bigcap_{x, y, \lambda, \mu} A(x, y, \lambda, \mu) ,
$$

donc est fermé dans $ F^E $.

#### Corollaire 1 {#evt-iii-s3-prop-4-cor-1 .statement}

Pour qu’une partie équicontinue H de $ \mathcal{L}(E; F) $ soit relativement compacte dans $ \mathcal{L}_s(E; F) $, il faut et il suffit que, pour tout $ x \in E $, l’ensemble $ H(x) $ des $ u(x) $, où $ u $ parcourt H, soit relativement compact dans F.

En effet, cette condition est nécessaire et suffisante pour que $ \overline{H} $ soit compacte dans $ F^E $ (TG, I, p. 64).

#### Corollaire 2 {#evt-iii-s3-prop-4-cor-2 .statement}

Toute partie équicontinue du dual $ E' $ de E est relativement compacte pour la topologie faible $ \sigma(E', E) $ de $ E' $ (III, p. 14, Exemple 4).

En effet, si H est une partie équicontinue de $ E' $, $ \sup_{u \in H} |u| $ est une semi-norme continue sur E ; en particulier pour tout $ x \in E $, l’ensemble $ H(x) $ est borné, donc relativement compact dans le corps des scalaires.

#### Corollaire 3 {#evt-iii-s3-prop-4-cor-3 .statement}

Dans le dual fort $ E'_b $ d’un espace semi-normé E, toute boule fermée est compacte pour la topologie faible $ \sigma(E', E) $.

En effet, cette boule est aussi fermée pour $ \sigma(E', E) $.

#### Proposition 5 {#evt-iii-s3-prop-5 .statement}

Soient E et F deux espaces localement convexes et soit T une partie totale de E. Sur toute partie équicontinue H de $ \mathcal{L}(E; F) $, les structures uniformes suivantes coïncident :

1) la structure uniforme de la convergence simple dans T ;
2) la structure uniforme de la convergence simple dans E ;
3) la structure uniforme de la convergence dans les parties précompactes de E.

Rappelons (III, p. 15, prop. 2) que, dans $ \mathcal{L}(E; F) $, la $ \mathfrak{S} $-topologie coïncide avec la $ \tilde{\mathfrak{S}} $-topologie où $ \tilde{\mathfrak{S}} $ est la plus petite bornologie adaptée à E et contenant $ \mathfrak{S} $.

Dans l’énoncé de la prop. 5, on peut donc remplacer le mot « totale » par « partout dense ». La proposition résulte alors des propriétés générales des ensembles équicontinu (TG, X, p. 16, th. 1).

#### Exemple 1 {#evt-iii-s3-n4-exa-1 .statement}

Soit $ \mu $ la mesure de Lebesgue sur $ \mathbf{R} $ et soit $ E $ l’espace semi-normé $ \mathcal{L}^p(\mu) $ ($ 1 \leq p < \infty $) (INT, IV). Pour toute fonction numérique $ f $ et tout nombre réel $ h $, notons $ f_h $ la fonction $ x \mapsto f(x - h) $. Il est clair que l’application $ f \mapsto f_h $ définit une isométrie linéaire de $ E $ sur lui-même. Si $ f $ est continue à support compact, $ f_h $ converge vers $ f $, uniformément donc aussi en moyenne d’ordre $ p $, lorsque $ h $ tend vers $ 0 $. Comme l’ensemble $ \mathscr{K}(\mathbf{R}) $ des fonctions continues à support compact est dense dans $ E $, et comme l’ensemble des isométries linéaires de $ E $ est équicontinu, il résulte de la prop. 5 que pour toute $ f \in E $, $ f_h $ converge en moyenne d’ordre $ p $ vers $ f $ lorsque $ h $ tend vers $ 0 $.

Prenons $ p = 1 $, et considérons la transformation de Fourier qui à $ f \in \mathcal{L}^1(\mu) $ fait correspondre la fonction $ \hat{f} $ sur $ \mathbf{R} $ définie par

$$
\hat{f}(y) = \int e^{-2i\pi xy} f(x) \, d\mu(x) .
$$

Les formes linéaires $ f \mapsto \hat{f}(y) $ forment une partie équicontinue du dual de $ \mathcal{L}^1(\mu) $.

D’autre part, on sait que l’ensemble $ T $ des fonctions caractéristiques d’intervalles fermés bornés est une partie totale de $ \mathcal{L}^1(\mu) $, et on vérifie aisément que, pour $ f \in T $, la transformée de Fourier $ \hat{f} $ est une fonction continue tendant vers zéro à l’infini. On en déduit qu’il en est de même pour tout $ f \in L^1(\mu) $ (« th. de Riemann-Lebesgue »). En effet, la relation $ \sup_{y \in \mathbf{R}} |\hat{f}(y)| \leq \|f\|_1 $ montre que l’application $ f \mapsto \hat{f} $ est une application continue de $ \mathcal{L}^1(\mu) $ dans l’espace $ \mathscr{B}(\mathbf{R}) $ des fonctions bornées sur $ \mathbf{R} $ muni de la convergence uniforme. Comme $ \hat{f} $ est continue pour $ f \in T $, il en résulte que $ \hat{f} $ est continue quelle que soit $ f \in L^1(\mu) $. Le fait que $ \hat{f} $ tende vers zéro à l’infini résulte de ce que le sous-espace $ \mathscr{C}_0(\mathbf{R}) $ des fonctions continues tendant vers $ 0 $ à l’infini est fermé dans $ \mathscr{B}(\mathbf{R}) $.

#### Exemple 2 {#evt-iii-s3-n4-exa-2 .statement}

Soit $ E $ l’espace des fonctions numériques continues dans $ \mathbf{R} $, muni de la topologie de la convergence compacte. Soit $ K $ un compact de $ \mathbf{R} $ et soit $ (\mu_n) $ une suite de mesures sur $ \mathbf{R} $ à support dans $ K $. Supposons $ \|\mu_n\| \leq 1 $ pour tout $ n $. L’ensemble des $ \mu_n $ est alors une partie équicontinue de $ E' $. Alors, si pour toute fonction $ f \in E $, on a $ \lim_{n \to \infty} \mu_n(f) = 0 $, la suite des fonctions $ x \mapsto \int e^{itx} d\mu_n(t) $ converge vers $ 0 $, uniformément dans toute partie compacte de $ \mathbf{R} $ (car l’ensemble des fonctions $ t \mapsto e^{itx} $, où $ x $ parcourt un compact de $ \mathbf{R} $, est compact dans $ E $). \*

#### Corollaire {#evt-iii-s3-n4-cor-1 .statement}

Supposons $ F $ séparé. Soit $ H $ une partie équicontinue de $ \mathcal{L}(E; F) $. Si un filtre $ \Phi $ sur $ H $ converge simplement vers une application $ u_0 $ de $ E $ dans $ F $, $ u_0 $ est une application linéaire continue de $ E $ dans $ F $, et $ \Phi $ converge uniformément vers $ u_0 $ dans toute partie précompacte de $ E $.

La première assertion résulte de la prop. 4 (III, p. 16) et la seconde de la prop. 5 (III, p. 17).

#### Proposition 6 {#evt-iii-s3-prop-6 .statement}

Soit $ H $ une partie équicontinue de $ \mathcal{L}(E; F) $. Si $ F $ est métrisable et s’il existe un ensemble dénombrable total dans $ E $, la structure uniforme sur $ H $ de la convergence simple dans $ E $ est métrisable. Si en outre il existe un ensemble dénombrable total dans $ F $, il existe un ensemble dénombrable partout dense dans $ H $ (pour la topologie de la convergence uniforme dans les parties précompactes de $ E $).

Soit $ (a_n) $ une suite totale dans $ E $. L’application $ u \mapsto (u(a_n)) $ est alors un isomorphisme de $ \mathcal{L}(E; F) $, muni de la structure uniforme de la convergence simple dans l’ensemble des $ a_n $, sur un sous-espace uniforme de $ \mathbf{F}^\mathbf{N} $. Si $ F $ est métrisable (resp. métrisable de type dénombrable), il en est de même de $ \mathbf{F}^\mathbf{N} $ (TG, IX, p. 15, cor. 2, et p. 19, corollaire), et la proposition résulte de la prop. 5 (III, p. 17).

#### Corollaire 1 {#evt-iii-s3-prop-6-cor-1 .statement}

Soient E un espace localement convexe métrisable de type dénombrable et F un espace normé de type dénombrable. Alors $ \mathscr{L}(E; F) $ est réunion d’une famille dénombrable de parties équicontinues et il existe dans $ \mathscr{L}(E; F) $ un ensemble dénombrable dense pour la topologie de la convergence uniforme dans les parties précompactes de E.

Soient B la boule unité de F et $ (V_n) $ un système fondamental dénombrable de voisinages de 0 dans E. Pour tout entier n, l’ensemble $ H_n $ des $ u \in \mathscr{L}(E; F) $ telles que $ u(V_n) \subset B $ est équicontinu et $ \mathscr{L}(E; F) $ est la réunion des $ H_n $. Le corollaire résulte donc de la prop. 6.

#### Corollaire 2 {#evt-iii-s3-prop-6-cor-2 .statement}

Dans le dual $ E' $ d’un espace normé de type dénombrable, toute boule fermée est un espace compact métrisable pour la topologie faible $ \sigma(E', E) $ et il existe dans $ E' $ un ensemble dénombrable dense pour $ \sigma(E', E) $.

Cela résulte de la prop. 6 et de III, p. 17, cor. 3.

### 5. Parties équicontinues de $ E' $

Dans ce numéro, on désigne par E un espace localement convexe et par $ E' $ son dual. Lorsque nous parlerons du polaire $ M^\circ $ d’une partie M de E (resp. $ E' $), il s’agira toujours, sauf mention expresse du contraire, du polaire de M relativement à la dualité entre E et $ E' $. Rappelons que, si V est un voisinage convexe, équilibré et fermé de 0 dans E, on a $ V = V^{\circ\circ} $ (II, p. 49, cor. 3).

#### Proposition 7 {#evt-iii-s3-prop-7 .statement}

Soit M une partie de $ E' $. Les conditions suivantes sont équivalentes :
(i) M est équicontinue ;
(ii) M est contenue dans le polaire d’un voisinage de 0 dans E ;
(iii) le polaire de M est un voisinage de 0 dans E.

Si M est équicontinue, il existe un voisinage convexe équilibré V de 0 tel que $ |u(x)| \leq 1 $ pour $ x \in V $ et $ u \in M $; on a donc $ M \subset V^\circ $ et (i) entraîne (ii). Avec les mêmes notations, si $ M \subset V^\circ $, on a $ V \subset V^{\circ\circ} \subset M^\circ $ et (ii) entraîne (iii). Enfin, si $ M^\circ $ contient un voisinage convexe équilibré V de 0, on a $ M \subset M^{\circ\circ} \subset V^\circ $ et les relations $ x \in \varepsilon V $, $ u \in M $ entraînent $ |u(x)| \leq \varepsilon $, pour tout $ \varepsilon > 0 $, ce qui montre que (iii) entraîne (i).

Remarquons que tout $ x \in E $ définit une application $ j(x): u \mapsto u(x) $ de $ E' $ dans K. On peut donc parler de la $ \mathfrak{S} $-topologie sur E, lorsque $ \mathfrak{S} $ est un ensemble de parties de $ E' $; c’est l’image réciproque par j de la $ \mathfrak{S} $-topologie sur $ K^{E'} $. On vérifie aussitôt que si $ \mathfrak{S} $ est une bornologie convexe sur $ E' $, un système fondamental de voisinages de 0 pour la $ \mathfrak{S} $-topologie sur E est formé des polaires des ensembles de $ \mathfrak{S} $. Il en est en particulier ainsi lorsque $ \mathfrak{S} $ est l’ensemble des parties équicontinues de $ E' $ et la prop. 7 entraîne :

#### Corollaire 1 {#evt-iii-s3-prop-7-cor-1 .statement}

La topologie de E est identique à la topologie de la convergence uniforme dans les parties équicontinues de $ E' $.

Plus généralement, soit F un espace localement convexe ; toute $ u \in \mathscr{L}(E; F) $ définit une application $ j(u) : (x, f) \mapsto f(u(x)) $ de $ E \times F' $ dans $ K $ (c’est-à-dire dans $ \mathbf{R} $ ou $ \mathbf{C} $). Ceci permet de définir dans l’espace $ \mathcal{L}(E; F) $ la topologie de la convergence uniforme dans un ensemble de parties de $ E \times F' $. En particulier :

#### Corollaire 2 {#evt-iii-s3-prop-7-cor-2 .statement}

*Soit $ \mathfrak{S} $ un ensemble de parties bornées de E. La $ \mathfrak{S}$-topologie sur $ \mathcal{L}(E; F) $ est la topologie de la convergence uniforme dans les ensembles de la forme $ A \times B \subset E \times F' $, où $ A $ décrit $ \mathfrak{S} $ et $ B $ l’ensemble des parties équicontinues de $ F' $.

En effet, pour tout $ u \in \mathcal{L}(E; F) $, tout $ A \in \mathfrak{S} $ et tout voisinage $ V $ convexe, équilibré et fermé de $ 0 $ dans $ F $, la relation $ u(A) \subset V $ est équivalente à « $ j(u)(A \times V^\circ) $ est contenu dans la boule unité de $ K $ ».

#### Proposition 8 {#evt-iii-s3-prop-8 .statement}

*Soit $ H $ un ensemble d’applications linéaires de $ E $ dans un espace localement convexe $ F $. Pour que $ H $ soit équicontinu, il faut et il suffit que, pour toute partie équicontinue $ X $ du dual $ F' $ de $ F $, l’ensemble des formes linéaires $ f \circ u $ pour $ f \in X $ et $ u \in H $ soit équicontinu.

Il est évident que la condition est nécessaire. Supposons-la vérifiée et soit $ V $ un voisinage convexe, équilibré et fermé de $ 0 $ dans $ F $. Puisque $ V^\circ $ est équicontinu, il existe un voisinage $ W $ de $ 0 $ dans $ E $ tel que $ |f(u(x))| \leq 1 $ pour $ x \in W, u \in H $ et $ f \in V^\circ $; autrement dit, on a $ u(W) \subset V^{\circ \circ} = V $ pour tout $ u \in H $ et $ H $ est donc équicontinu.

### 6. Le complété d’un espace localement convexe

#### Théorème 1 (Grothendieck) {#evt-iii-s3-thm-1 .statement}

*Soit $ E $ un espace localement convexe, et soit $ \mathfrak{S} $ une bornologie adaptée et couvrante sur $ E $. Soit $ F \subset E^* $ l’espace des formes linéaires sur $ E $ dont la restriction à tout ensemble appartenant à $ \mathfrak{S} $ est continue. On munit $ F $ de la $ \mathfrak{S}$-topologie. L’injection canonique de $ E'_\mathfrak{S} $ dans $ F $ se prolonge en un isomorphisme du complété $ \hat{E}'_\mathfrak{S} $ de $ E'_\mathfrak{S} $ sur $ F $.

Comme toute limite simple de formes linéaires sur $ E $ est une forme linéaire (III, p. 16, prop. 4) et que la bornologie $ \mathfrak{S} $ est couvrante, il résulte de TG, X, p. 9, cor. 2 que l’espace $ F $, muni de la $ \mathfrak{S}$-topologie, est séparé et *complet*. Il est clair que $ E'_\mathfrak{S} $ est un sous-espace vectoriel topologique de $ F $; il suffit donc de prouver que $ E'_\mathfrak{S} $ est *partout dense* dans $ F $, ce qui résulte du lemme suivant :

#### Lemme 1 {#evt-iii-s3-lem-1 .statement}

*Soit $ A $ une partie convexe, équilibrée et fermée de $ E $, et soit $ u $ une forme linéaire sur $ E $ dont la restriction à $ A $ est continue. Pour tout $ \varepsilon > 0 $, il existe $ x' \in E' $ tel que*
$$
|u(x) - \langle x, x' \rangle| \leq \varepsilon \quad \text{pour tout } x \in A .
$$

Soit en effet $ \varepsilon > 0 $. Il existe un voisinage convexe, équilibré et fermé $ U $ de $ 0 $ dans $ E $ tel que $ |u(x)| \leq \varepsilon $ pour tout $ x \in U \cap A $. On sait que le polaire $ U^\circ $ de $ U $ dans $ E^* $ est contenu dans $ E' $ et est compact pour la topologie $ \sigma(E^*, E) $ (III, p. 17, cor. 2). Comme le polaire $ A^\circ $ de $ A $ dans $ E^* $ est fermé pour $ \sigma(E^*, E) $, il en résulte que $ A^\circ + U^\circ $ est une partie convexe *fermée* de $ E^* $ (TG, III, p. 28, cor. 1).

Soit $ C $ une partie convexe, équilibrée et fermée de $ E $. Alors, $ C $ est fermée pour σ(E, E') (II, p. 49, cor. 3), donc aussi pour σ(E, E*), et on a par suite C = C°° (pour la dualité entre E et E*). Par suite, on a

$$
A \cap U = A^{°°} \cap U^{°°} = (A° \cup U°)^° \supset (A° + U°)^°
$$

d’où

$$
(A \cap U)^° \subset (A° + U°)^{°°} = A° + U° .
$$

Comme la forme linéaire $ \varepsilon^{-1}u $ appartient à $(A \cap U)^°$, il existe donc $ v \in A° $ et $ w \in U° $ tels que $ u = \varepsilon(v + w) $. Alors $ x' = \varepsilon w $ appartient à $ E' $ et $ u - x' = \varepsilon v $ est majorée en valeur absolue par $ \varepsilon $ sur $ A $, d’où le lemme.

Soit maintenant $ E $ un espace localement convexe séparé, et soit $ \hat{E} $ son complété. Toute forme linéaire $ f $ continue sur $ E $ se prolonge par continuité à $ \hat{E} $; on a donc $(\hat{E})' = E'$ (III, p. 16) et tout élément de $ \hat{E} $ définit une forme linéaire sur $ E' $, c’est-à-dire un élément du dual algébrique $ E'^* $ de $ E' $. De plus, la dualité entre $ E $ (resp. $ \hat{E} $) et $ E' $ est séparante (II, p. 26, cor. 1). Par suite $ E $ et $ \hat{E} $ s’identifient à des sous-espaces vectoriels de $ E'^* $.

#### Théorème 2 {#evt-iii-s3-thm-2 .statement}

*Soit E un espace localement convexe séparé, et soit $ \hat{E} $ son complété ; on identifie E et $ \hat{E} $ à des sous-espaces vectoriels de $ E'^* $. Pour qu’un élément $ f \in E'^* $ appartienne à $ \hat{E} $, il faut et il suffit que la restriction de $ f $ à toute partie équicontinue de $ E' $ soit continue pour la topologie $ \sigma(E', E) $.*

L’espace $ E $ s’identifie au dual topologique de $ E' $ lorsqu’on munit $ E' $ de la topologie $ \sigma(E', E) $ (II, p. 46, prop. 3) ; d’autre part, si $ \mathcal{S} $ est l’ensemble des parties équicontinues de $ E' $, la topologie donnée sur $ E $ est la $ \mathcal{S} $-topologie (III, p. 19, cor. 1). Il résulte alors de III, p. 13, prop. 1, que les ensembles de $ \mathcal{S} $ sont bornés pour $ \sigma(E', E) $ (*cf.* plus loin, III, p. 22, prop. 9), autrement dit $ \mathcal{S} $ est une bornologie adaptée et couvrante pour la topologie $ \sigma(E', E) $. Le th. 2 est alors conséquence du th. 1, où l’on remplace $ E $ par $ E' $ et $ E'_\mathcal{S} $ par $ E $.

**Corollaire 1 (Banach).** — *Soit E un espace localement convexe séparé et complet. Pour qu’une forme linéaire sur $ E' $ soit continue pour la topologie faible $ \sigma(E', E) $ (c’est-à-dire provienne d’un élément de $ E $), il suffit que sa restriction à toute partie équicontinue de $ E' $ soit continue pour $ \sigma(E', E) $.*

#### Remarque {#evt-iii-s3-n6-rem-1 .statement}

Supposons de plus qu’il existe dans $ E $ un ensemble total dénombrable ; alors toute partie équicontinue de $ E' $ est métrisable pour la topologie $ \sigma(E', E) $ (III, p. 18, prop. 6) ; pour vérifier qu’une forme linéaire $ u $ sur $ E' $ est faiblement continue, il suffit donc de vérifier que, pour toute suite équicontinue $ (x'_n) $ dans $ E' $ qui converge vers 0 pour $ \sigma(E', E) $, on a $ \lim_{n \to \infty} u(x'_n) = 0 $.

#### Corollaire 2 {#evt-iii-s3-thm-2-cor-2 .statement}

*Soit $ (E_i)_{i \in I} $ une famille d’espaces localement convexes séparés et soit $ E $ leur somme directe topologique. L’application canonique de la somme directe des $ \hat{E}_i $ dans $ \hat{E} $ est un isomorphisme. En particulier, $ E $ est complet si et seulement si tous les $ E_i $ sont complets.*

On sait que le dual de E s’identifie au produit des duals des $ E_i $ (II, p. 33, formule (1)). Soit $ u \in \hat{E} $ et soit $ u_i \in E'_i* $ la restriction de $ u $ (considérée comme élément de $ E'(*) $) à $ E'_i \subset E' $. Il est immédiat qu’il suffit de démontrer que $ u_i = 0 $ sauf pour un nombre fini d’indices $ i \in I $. Supposons au contraire qu’il existe une suite $ (i_n)_{n \in \mathbf{N}} $ d’indices distincts telle que $ u_{i_n} \neq 0 $. Il existe alors $ x_{i_n} \in E'_{i_n} $ telle que $ u_{i_n}(x_{i_n}) = n $. L’ensemble $ H $ des $ x_{i_n} $ est équicontinu dans $ E' $ et la restriction de $ u $ à $ H $ n’est pas bornée, ce qui est impossible.

### 7. $ \mathcal{S}$-bornologies sur $ \mathcal{L}(E ; F) $

Soient $ E $ et $ F $ deux espaces localement convexes et $ \mathcal{S} $ un ensemble de parties bornées de $ E $. Dire qu’une partie $ H $ de $ \mathcal{L}(E ; F) $ est bornée pour la $ \mathcal{S}$-topologie signifie : pour tout $ M \in \mathcal{S} $, tout voisinage $ V $ de 0 dans $ F $ absorbe l’ensemble $ H(M) = \bigcup_{u \in H} u(M) $; cela revient à dire que *pour tout $ M \in \mathcal{S} $, l’ensemble $ H(M) $ est borné dans $ F $*. De façon équivalente, cela signifie que pour tout voisinage $ V $ de 0 dans $ F $, l’ensemble $ \bigcap_{u \in H} u^{-1}(V) $ *absorbe toute partie* $ M $ de $ \mathcal{S} $.

#### Proposition 9 {#evt-iii-s3-prop-9 .statement}

*Soient $ E $ et $ F $ deux espaces localement convexes et soit $ \mathcal{S} $ un ensemble de parties bornées de $ E $. Toute partie équicontinue de $ \mathcal{L}(E ; F) $ est bornée pour la $ \mathcal{S}$-topologie.*

En effet, si $ H $ est une partie équicontinue de $ \mathcal{L}(E ; F) $ et $ V $ un voisinage de 0 dans $ F $, l’ensemble $ \bigcap_{u \in H} u^{-1}(V) $ est un voisinage de 0 dans $ E $, donc absorbe toute partie bornée de $ E $.

Une partie de $ \mathcal{L}(E ; F) $ qui est bornée pour une $ \mathcal{S}$-topologie n’est pas nécessairement équicontinue, même si $ \mathcal{S} $ est couvrante et même si $ \mathcal{S} $ est la bornologie canonique de $ E $ (IV, p. 50, exerc. 17). Nous étudierons au paragraphe suivant sous le nom d’espaces *tonnelés* les espaces $ E $ tels que toute partie simplement bornée de $ \mathcal{L}(E ; F) $ soit équicontinue. Notons dès maintenant le résultat suivant :

#### Proposition 10 {#evt-iii-s3-prop-10 .statement}

*Soit $ E $ un espace bornologique* (en particulier, un espace localement convexe métrisable), *et soit $ F $ un espace localement convexe. Toute partie* $ H $ *de* $ \mathcal{L}(E ; F) $ *qui est bornée pour la topologie de la convergence bornée est équicontinue.*

En effet, pour tout voisinage convexe équilibré $ V $ de 0 dans $ F $, l’ensemble $ \bigcap_{u \in H} u^{-1}(V) $ absorbe toute partie bornée de $ E $, donc est un voisinage de 0 dans $ E $, ce qui prouve que $ H $ est équicontinue.

### 8. Parties complètes de $ \mathcal{L}_{\mathcal{S}}(E ; F) $

#### Proposition 11 {#evt-iii-s3-prop-11 .statement}

*Soient $ E $ et $ F $ deux espaces localement convexes, $ \mathcal{S} $ un recouvrement de $ E $ formé de parties bornées. Si $ F $ est séparé et quasi-complet* (III, p. 8), *toute partie équicontinue* $ H $ *de* $ \mathcal{L}(E ; F) $, *fermée pour la* $ \mathcal{S}$-*topologie, est un sous-espace uniforme complet de* $ \mathcal{L}_{\mathcal{S}}(E ; F) $.

Comme $ H $ est bornée dans $ \mathcal{L}_\mathfrak{S}(E; F) $ (III, p. 22, prop. 9) et fermée dans $ F^E $ pour la $ \mathfrak{S} $-topologie (III, p. 16, prop. 4), cela résulte du cor. 3 de TG, X, p. 7.

#### Remarque 1 {#evt-iii-s3-n8-rem-1 .statement}

Soit $ M $ un sous-espace uniforme complet de $ \mathcal{L}_\mathfrak{S}(E; F) $. Pour tout ensemble de parties bornées $ \mathfrak{S}' \supset \mathfrak{S} $ de $ E $, la $ \mathfrak{S}' $-topologie est plus fine que la $ \mathfrak{S} $-topologie sur $ \mathcal{L}(E; F) $; d’autre part, il existe un système fondamental de voisinages de 0 pour la $ \mathfrak{S}' $-topologie qui sont fermés pour la topologie de la convergence simple (III, p. 13, Remarque 2), et a fortiori pour la $ \mathfrak{S} $-topologie. On en conclut (TG, III, p. 26, cor. 1) que $ M $ est encore complet pour la $ \mathfrak{S}' $-topologie.

#### Corollaire {#evt-iii-s3-n8-cor-1 .statement}

*Soient* $ E $ et $ F $ *deux espaces localement convexes*, $ H $ *une partie équicontinue de* $ \mathcal{L}(E; F) $. *Si* $ F $ *est séparé et quasi-complet, et si un filtre* $ \Phi $ *sur* $ H $ *converge simplement en tous les points d’une partie totale* $ T $ *de* $ E $, *alors il existe une application linéaire continue* $ u $ *de* $ E $ *dans* $ F $ *telle que* $ \Phi $ *converge uniformément vers* $ u $ *dans toute partie précompacte de* $ E $.

En effet, en vertu de la prop. 5 (III, p. 17), $ \Phi $ est un filtre de Cauchy pour la structure uniforme de la convergence précompacte dans $ E $; d’après la prop. 11, l’adhérence $ \overline{H} $ de $ H $ dans $ \mathcal{L}_{pc}(E; F) $ est complète et $ \Phi $ converge donc uniformément sur toute partie précompacte de $ E $ vers une application $ u \in \overline{H} $.

#### Remarque 2 {#evt-iii-s3-n8-rem-2 .statement}

Soit $ (u_n) $ une suite d’applications linéaires continues d’un espace de Banach $ E $ dans un espace de Banach $ F $; il peut se faire que $ (u_n(x)) $ ait une limite en tout point d’un sous-espace vectoriel partout dense $ T $ de $ E $, sans que la suite $ (u_n) $ soit bornée dans l’espace normé $ \mathcal{L}(E; F) $. Prenons par exemple pour $ E $ l’espace des fonctions numériques continues dans $ \mathbf{R} $, tendant vers zéro à l’infini, avec la norme $ \|f\| = \sup_{x \in \mathbf{R}} |f(x)| $ et pour $ T $ le sous-espace des fonctions numériques continues à support compact. La suite des applications linéaires continues $ f \mapsto nf(n) $ de $ E $ dans $ \mathbf{R} $ converge vers 0 pour tout $ f \in T $, mais n’est pas bornée dans $ \mathcal{L}_b(E; \mathbf{R}) $. Le même exemple montre que dans l’espace $ \mathcal{L}(T; \mathbf{R}) $ une suite $ (v_n) $ peut être simplement convergente et non bornée pour la topologie de la convergence bornée.

D’autre part, la suite des applications linéaires continues $ f \mapsto \sum_{k=1}^n f(k) $ est une suite de Cauchy dans $ \mathcal{L}(T; \mathbf{R}) $ pour la topologie de la convergence simple, mais n’a pas de limite dans $ \mathcal{L}(T; \mathbf{R}) $ pour cette topologie.

#### Proposition 12 {#evt-iii-s3-prop-12 .statement}

*Soient* $ E $ *un espace localement convexe bornologique*, $ F $ *un espace localement convexe séparé et complet et* $ \mathfrak{S} $ *un ensemble de parties bornées de* $ E $, *contenant l’image de toute suite convergeant vers* 0. *Alors l’espace* $ \mathcal{L}_\mathfrak{S}(E; F) $ *est complet*.

Soit $ \Phi $ un filtre de Cauchy dans $ \mathcal{L}_\mathfrak{S}(E; F) $. Alors $ \Phi $ est un filtre de Cauchy pour la topologie de la convergence simple, donc converge dans $ F^E $; en outre, sa limite $ u $ est une application linéaire de $ E $ dans $ F $ et $ \Phi $ converge vers $ u $ uniformément dans tout ensemble de $ \mathfrak{S} $ (TG, X, p. 6, prop. 5). Il en résulte que l’image par $ u $ d’une suite convergeant vers zéro est une suite convergeant vers zéro, donc que $ u $ est *continue* puisque $ E $ est bornologique (III, p. 11, prop. 1, (iii)).

#### Corollaire 1 {#evt-iii-s3-prop-12-cor-1 .statement}

Le dual fort d’un espace bornologique est complet.

#### Corollaire 2 {#evt-iii-s3-prop-12-cor-2 .statement}

Soit E un espace semi-normé et soit F un espace de Banach (resp. de Fréchet). L’espace $ \mathcal{L}_b(E; F) $ est un espace de Banach (resp. de Fréchet). En particulier, le dual d’un espace semi-normé est un espace de Banach.

## EXERCICES {#evt-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
