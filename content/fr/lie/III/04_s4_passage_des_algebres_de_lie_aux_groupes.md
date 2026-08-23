---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 4
section_title: Passage des algèbres de Lie aux groupes de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0164-0182, 0259-0263
extraction: ocr
subsections:
    - "no": 1
      title: Passage des morphismes d’algèbres de Lie aux morphismes de groupes de Lie
      page: 0
      pdf_page: 164
    - "no": 2
      title: Passage des algèbres de Lie aux groupes de Lie
      page: 0
      pdf_page: 166
    - "no": 3
      title: Applications exponentielles
      page: 0
      pdf_page: 169
    - "no": 4
      title: Fonctorialité des applications exponentielles
      page: 0
      pdf_page: 173
    - "no": 5
      title: Structure induite sur un sous-groupe
      page: 0
      pdf_page: 174
    - "no": 6
      title: Primitives des formes différentielles à valeurs dans une algèbre de Lie
      page: 0
      pdf_page: 176
    - "no": 7
      title: Passage des lois d’opérations infinitésimales aux lois d’opérations
      page: 0
      pdf_page: 180
statements: 41
exercises: 13
content_sha256: 2ce4dc5be28a4010bf77c731683a7b5cdfdc56fcc146df60792b5c36ad197a8c
---

## § 4. Passage des algèbres de Lie aux groupes de Lie

Rappelons que, jusqu’à la fin du chapitre, K est supposé de caractéristique 0.

### 1. Passage des morphismes d’algèbres de Lie aux morphismes de groupes de Lie

#### Lemme 1 {#lie-iii-s4-lem-1 .statement}

Soient G un groupuscule de Lie, $ \mathfrak{h} $ une sous-algèbre de Lie de $ L(G) $ admettant un supplémentaire topologique. La réunion des $ g\mathfrak{h} $ (resp. $ \mathfrak{h}g $) pour $ g \in G $ est un sous-fibré vectoriel intégrable de $ T(G) $.

Le feuilletage intégral (VAR, R, 9.3.2) de la réunion des $ g\mathfrak{h} $ (resp. $ \mathfrak{h}g $) s’appelle le feuilletage gauche (resp. droit) de G associé à $ \mathfrak{h} $.

#### Théorème 1 {#lie-iii-s4-thm-1 .statement}

Soient G et H des groupuscules de Lie, f un morphisme continu de L(G) dans L(H).

(i) Il existe un sous-groupuscule de Lie ouvert $ G' $ de G et un morphisme $ \varphi $ de $ G' $ dans H tels que $ f = L(\varphi) $.

(ii) Soient $ G_1, G_2 $ des sous-groupuscules de Lie ouverts de G, et $ \varphi_i $ un morphisme de $ G_i $ dans H tel que $ f = L(\varphi_i) $ pour $ i = 1, 2 $. Alors $ \varphi_1 $ et $ \varphi_2 $ coïncident dans un voisinage de e.

Soient $ p_1 : G \times H \to G $, $ p_2 : G \times H \to H $ les projections canoniques. Pour tout $ (g, h) \in G \times H $, soit $ f_{g,h} $ l’application $ ga \mapsto hf(a) $ de $ T_g(G) = gL(G) $ dans $ T_h(H) = hL(H) $. En considérant les trivialisations gauches de T(G) et T(H), on voit aussitôt que les $ f_{g,h} $ définissent un morphisme de $ p_1^*T(G) $ dans $ p_2^*T(H) $. Soit a le graphe de f; c’est une sous-algèbre de Lie fermée de $ L(G) \times L(H) $ qui admet $ \{0\} \times L(H) $ comme supplémentaire topologique. Pour tout $ (g, h) \in G \times H $, le graphe de $ f_{g,h} $ est $ (g, h) . a $. La réunion de ces graphes est un sous-fibré vectoriel intégrable de $ T(G \times H) $ (lemme 1). Il existe alors (VAR, R, 9.3.7) un voisinage ouvert U de $ e_G $ dans G et une application analytique $ \varphi $ de U dans H telle que $ \varphi(e_G) = e_H $ et $ T_g(\varphi) = f_{g,\varphi(g)} $ pour tout $ g \in U $. En particulier, $ T_{e_G}(\varphi) = f $.

Soit V un voisinage ouvert de $ e_G $ dans G tel que, pour $ (s, t) \in V \times V $, les produits st et $ \varphi(s)\varphi(t) $ soient définis, et $ st \in U $. Considérons les applications $ \alpha_1, \alpha_2 $ de $ V \times V $ dans H définies par

$$
\alpha_1(s, t) = \varphi(ts), \qquad \alpha_2(s, t) = \varphi(t)\varphi(s).
$$

On a $ \alpha_1(t, e) = \varphi(t) = \alpha_2(t, e) $. D’autre part, fixons t dans V, et soit $ \beta_i $ l’application $ s \mapsto \alpha_i(s, t) $ de V dans H. On a, pour tout $ s \in V $ et tout $ a \in L(G) $,

$$
\begin{align*}
T_s(\beta_1)(sa) &= T_{ts}(\varphi)(tsa) = f_{ts, \varphi(ts)}(tsa) \\
&= \varphi(ts)f(a) = f_{s, \beta_1(s)}(sa) \\
T_s(\beta_2)(sa) &= \varphi(t)T_s(\varphi)(sa) = \varphi(t)f_{s, \varphi(s)}(sa) \\
&= \varphi(t)\varphi(s)f(a) = f_{s, \beta_2(s)}(sa).
\end{align*}
$$

Donc (VAR, R, 9.3.7) $ \alpha_1 $ et $ \alpha_2 $ coïncident dans un voisinage de $ (e_G, e_G) $. La restriction de $ \varphi $ à un voisinage ouvert symétrique assez petit de $ e_G $ est donc un morphisme de groupuscules de Lie, d’où (i).

Soient $ G_1, G_2, \varphi_1, \varphi_2 $ comme dans (ii), et prouvons que $ \varphi_1, \varphi_2 $ coïncident dans un voisinage de $ e_G $. Il existe un voisinage ouvert $ W $ de $ e_G $ tel que $ \varphi_1(ts) = \varphi_1(t)\varphi_1(s) $, $ \varphi_2(ts) = \varphi_2(t)\varphi_2(s) $ quels que soient $ s, t $ dans $ W $. Alors, si $ s \in W $ et $ a \in L(G) $, on a
$$
T_s(\varphi_i)(sa) = \varphi_i(s)T_e(\varphi_i)(a) = \varphi_i(s)f(a) = f_{s,\varphi_i(s)}(sa)
$$
pour $ i = 1, 2 $. Comme $ \varphi_1(e_G) = e_H = \varphi_2(e_G) $, on conclut de VAR, R, 9.3.7, que $ \varphi_1 $ et $ \varphi_2 $ coïncident dans un voisinage de $ e_G $.

#### Corollaire 1 {#lie-iii-s4-thm-1-cor-1 .statement}

*Soient G et H deux groupuscules de Lie. Si L(G) et L(H) sont isomorphes, G et H sont localement isomorphes.*
Cela résulte du th. 1, et du § 1, n° 10, prop. 21.

#### Corollaire 2 {#lie-iii-s4-thm-1-cor-2 .statement}

*Soit G un groupuscule de Lie. Si L(G) est commutative, G est localement isomorphe au groupe de Lie additif L(G).*
En effet, l’algèbre de Lie du groupe additif $ L(G) $ est isomorphe à $ L(G) $. Il suffit donc d’appliquer le cor. 1.

#### Corollaire 3 {#lie-iii-s4-thm-1-cor-3 .statement}

*Soit G un groupe de Lie. Si L(G) est commutative, G contient un sous-groupe ouvert commutatif.*
Il existe un sous-groupuscule de Lie ouvert U de G qui est commutatif (cor. 2). Soit V un voisinage de $ e $ tel que $ V^2 \subset U $. On a $ xy = yx $ quels que soient $ x, y $ dans V. Donc le sous-groupe de G engendré par V est commutatif; il est évidemment ouvert.

### 2. Passage des algèbres de Lie aux groupes de Lie

Nous noterons $ H(X, Y) $ la série de Hausdorff (chap. II, § 6, n° 4, déf. 1).

#### Lemme 2 {#lie-iii-s4-lem-2 .statement}

*Soit L une algèbre de Lie normée complète sur $ \mathbf{R} $ ou $ \mathbf{C} $. Soit G l’ensemble des $ x \in L $ tels que $ \|x\| < \frac{1}{3} \log \frac{3}{2} $. Soit $ \theta $ l’application $ x \mapsto -x $ de G dans G. Soit H la restriction à $ G \times G $ de la fonction de Hausdorff de L* (chap. II, § 7, n° 2).
(i) $ (G, 0, \theta; H) $ est un groupuscule de Lie.
(ii) *Soit $ \varphi $ l’application identique de G dans L. La différentielle de $ \varphi $ en 0 est un isomorphisme de l’algèbre de Lie normable $ L(G) $ sur L.*
(i) résulte du chap. II, § 7, n° 2.
Comme $ \varphi $ est une carte de G, la différentielle $ \psi $ de $ \varphi $ en 0 est un isomorphisme d’espaces normables. D’autre part, le développement en série entière $ H = \sum_{i,j \geq 0} H_{ij} $ de l’application H est tel que $ H_{11}(x, y) = \frac{1}{2}[x, y] $. D’après le § 3, prop. 24, on a, quels que soient $ a, b $ dans $ L(G) $,
$$
\psi([a, b]) = H_{11}(\psi(a), \psi(b)) - H_{11}(\psi(b), \psi(a)) = [\psi(a), \psi(b)]
$$
ce qui prouve (ii).

On dit que G est le groupuscule de Lie défini par L.

Supposons K ultramétrique. Soit p la caractéristique du corps résiduel de K. Si $ p \neq 0 $, posons $ \lambda = |p|^{1/(p-1)} $; si $ p = 0 $, posons $ \lambda = 1 $.

#### Lemme 3 {#lie-iii-s4-lem-3 .statement}

Soit L une algèbre de Lie normée complète sur K. Soit G l’ensemble des $ x \in L $ tels que $ \|x\| < \lambda $. Soit $ H : G \times G \to G $ la fonction de Hausdorff de L (chap. II, § 8, n° 3).

(i) Muni de la loi de composition H, G est un groupe de Lie dans lequel O est élément neutre, et $ -x $ inverse de x pour tout $ x \in G $.

(ii) Soit $ \varphi $ l’application identique de G dans L. La différentielle de $ \varphi $ en O est un isomorphisme de l’algèbre de Lie normable $ L(G) $ sur L.

(iii) Pour tout $ \mu \in \mathbf{R}_+^* $, soit $ G_\mu $ l’ensemble des $ x \in L $ tels que $ \|x\| < \mu $. Alors les $ G_\mu $, pour $ \mu < \lambda $, forment un système fondamental de voisinages ouverts et fermés de O, et sont des sous-groupes de G.

Les assertions (i) et (iii) résultent du chap. II, § 8, n° 3, prop. 3, et (ii) se démontre comme dans le lemme 2.

On dit que G est le groupe de Lie défini par L.

#### Théorème 2 {#lie-iii-s4-thm-2 .statement}

Soit L une algèbre de Lie normable complète. Il existe un groupuscule de Lie G tel que $ L(G) $ soit isomorphe à L. Deux tels groupuscules de Lie sont localement isomorphes.

La première assertion résulte des lemmes 2 et 3. La deuxième assertion résulte du cor. 1 du th. 1, n° 1.

#### Corollaire 1 {#lie-iii-s4-thm-2-cor-1 .statement}

Soit G un groupe de Lie. Il existe un voisinage de e qui ne contient aucun sous-groupe fini distinct de $ \{e\} $. Si K = $ \mathbf{R} $ ou $ \mathbf{C} $, il existe un voisinage de e qui ne contient aucun sous-groupe distinct de $ \{e\} $.

Posons $ L(G) = L $. Choisissons une norme sur L définissant la topologie de L et telle que $ \| [x, y] \| \leq \|x\| \|y\| $ quels que soient $ x, y $ dans L.

Supposons K = $ \mathbf{R} $ ou $ \mathbf{C} $. Soit G' le groupuscule de Lie défini par L. Il existe une boule ouverte U' de centre 0 dans G', et un isomorphisme $ \varphi $ du groupuscule de Lie U' sur un voisinage ouvert U de e dans G. Soient $ V' = \frac{1}{2}U' $, $ V = \varphi(V') $, H un sous-groupe de G contenu dans V, et $ h \in H $. Posons $ x = \varphi^{-1}(h) \in V' $. Si $ x \neq 0 $, il existe un entier $ n > 0 $ tel que $ x, 2x, \ldots, nx $ sont dans $ V' $, $ (n+1)x \in U' $, $ (n+1)x \notin V' $. Alors $ h, h^2, \ldots, h^n $ sont dans V, $ h^{n+1} \in U $, $ h^{n+1} \notin V $, ce qui est absurde. Donc $ H = \{e\} $.

Supposons K ultramétrique. Il suffit de prouver le corollaire quand G est le groupe de Lie associé à L. Si $ g \in G $, les puissances de g calculées dans G sont les éléments de $ \mathbf{Z}g $ calculés dans L. Ceux-ci sont deux à deux distincts si $ g \neq e $. Donc G ne contient aucun sous-groupe fini distinct de $ \{e\} $.

#### Corollaire 2 {#lie-iii-s4-thm-2-cor-2 .statement}

Soient k un sous-corps fermé non discret de K, G un groupe de Lie sur k, et L = L(G). Supposons donnée sur L une structure L' de K-algèbre de Lie normable, compatible avec la structure de k-algèbre de Lie normable, et invariante par la représentation adjointe de G. Il existe alors sur G une structure de K-groupe de Lie et une seule compatible avec la structure de k-groupe de Lie et pour laquelle l’algèbre de Lie est L'.

Il existe un groupuscule de Lie G₁ sur K tel que L(G₁) = L' (th. 2). D’après le cor. 1 du th. 1, n° 1, G et G₁, considérés comme k-groupuscules de Lie, sont localement isomorphes. Donc il existe un voisinage ouvert G' de e dans G et une structure de K-groupuscule de Lie sur G', d’algèbre de Lie L, compatible avec la structure de groupuscule de Lie sur k. Soit V un voisinage ouvert symétrique de e dans G tel que V² ⊂ G'. Soit g ∈ G. Alors φ = Int g est un k-isomorphisme d’un sous-groupuscule de Lie ouvert assez petit de G' sur un sous-groupuscule de Lie ouvert de G'; et Tₑ(φ) est K-linéaire, donc Tₓ(φ) est K-linéaire pour x assez voisin de e; par suite la restriction de Int g à un voisinage ouvert assez petit de e dans V est K-analytique (VAR, R, 5.14.6). D’après le § 1, n° 9, prop. 18, il existe sur G une structure de K-variété analytique pour laquelle G est un K-groupe de Lie et V une sous-K-variété ouverte de G. Par translation, on voit que la structure de k-variété sous-jacente de G est la structure donnée. L’algèbre de Lie du K-groupe de Lie G est la même que celle du K-sous-groupuscule de Lie ouvert V, donc est L'. Enfin, l’unicité annoncée dans le corollaire résulte du § 3, n° 8, prop. 32.

#### Théorème 3 {#lie-iii-s4-thm-3 .statement}

Soient G un groupuscule de Lie, h une sous-algèbre de Lie de L(G) admettant un supplémentaire topologique. Il existe un sous-groupuscule de Lie H de G tel que L(H) = h. Si H₁ et H₂ sont des sous-groupuscules de Lie de G tels que

$$
L(H_1) = L(H_2) = h,
$$

alors H₁ ∩ H₂ est ouvert dans H₁ et H₂.

Il existe un groupuscule de Lie H' d’algèbre de Lie isomorphe à h (th. 2). Diminuant au besoin H', on peut supposer qu’il existe un morphisme φ de H' dans G tel que L(φ) soit un isomorphisme de L(H') sur h (n° 1, th. 1). Comme h admet un supplémentaire topologique, φ est une immersion en e. Donc, en diminuant encore H', on peut supposer que φ est un isomorphisme de la variété H' sur une sous-variété de G. Ceci prouve l’existence de H. La deuxième assertion résulte de la proposition suivante:

#### Proposition 1 {#lie-iii-s4-prop-1 .statement}

Soient G un groupuscule de Lie, H et H' deux sous-groupuscules de Lie. Pour que L(H) ⊃ L(H'), il faut et il suffit que H ∩ H' soit ouvert dans H'.

Si H ∩ H' est ouvert dans H', on a L(H') = L(H ∩ H') ⊂ L(H). Supposons L(H) ⊃ L(H'). Soient i, i' les injections canoniques de H, H' dans G. En diminuant au besoin H', on peut supposer qu’il existe un morphisme ψ de H' dans H tel que L(ψ) soit l’injection canonique de L(H') dans L(H) (n° 1, th. 1).

Alors $ L(i \circ \psi) = L(i') $, donc il existe un voisinage $ V $ de $ e_{H'} $ dans $ H' $ tel que $ i \circ \psi $ et $ i' $ coïncident dans $ V $ (th. 1). Par suite, $ V \subset H $, donc $ V \subset H \cap H' $, et $ H \cap H' $ est ouvert dans $ H' $ (\S 1, no 10).

#### Proposition 2 {#lie-iii-s4-prop-2 .statement}

*Soient G un groupe de Lie sur K, k un sous-corps fermé non discret de K, H un sous-groupe de Lie du k-groupe de Lie G. On suppose que L(H) est un sous-K-espace vectoriel de L(G) admettant un supplémentaire topologique. Alors H est un sous-groupe de Lie du K-groupe de Lie G.*

Il existe un sous-groupuscule de Lie $ H' $ du K-groupe de Lie G tel que $ L(H') = L(H) $ (th. 3). Considérons G, H, H' comme des k-groupuscules de Lie ; le th. 3 prouve alors que $ H \cap H' $ est ouvert dans H et $ H' $. Donc il existe un voisinage ouvert U de $ e $ dans G tel que $ U \cap H $ soit une sous-variété de G sur K. Par suite, H est un sous-groupe de Lie du K-groupe de Lie G (\S 1, no 3, prop. 6).

### 3. Applications exponentielles

#### Théorème 4 {#lie-iii-s4-thm-4 .statement}

*Soient G un groupuscule de Lie, L son algèbre de Lie, V un voisinage ouvert de 0 dans L, $ \varphi $ une application analytique de V dans G telle que $ \varphi(0) = 0 $ et $ T_0(\varphi) = \mathrm{Id}_L $. Les conditions suivantes sont équivalentes :

(i) Quel que soit $ b \in L $, on a $ \varphi((\lambda + \lambda')b) = \varphi(\lambda b)\varphi(\lambda'b) $ pour $ |\lambda| $ et $ |\lambda'| $ assez petits.

(ii) Quel que soit $ b \in L $ et l’entier $ n > 0 $, $ \varphi_*(b^n) $ est homogène de degré $ n $ dans $ U(G) $ (on identifie $ T_0^{(\infty)}(L) $ à $ TS(L) $, et $ b^n $ est calculé dans $ TS(L) $).

(iii) L’application $ \varphi_* $ de $ TS(L) $ dans $ U(G) $ est compatible avec les graduations de $ TS(L) $ et $ U(G) $.

(iv) L’application $ \varphi_* $ de $ TS(L) $ dans $ U(G) $ est l’application canonique de $ TS(L) $ dans l’algèbre enveloppante de $ L $.

(v) Il existe une norme sur $ L $ définissant la topologie de $ L $ et telle que

$$
\|[x, y]\| \leq \|x\|\|y\|
$$

quels que soient $ x, y $ dans $ L $, et un sous-groupuscule ouvert $ W \subset V $ du groupuscule de Lie défini par $ L $ (no 2), tels que $ \varphi | W $ soit un isomorphisme de $ W $ sur un sous-groupuscule de Lie ouvert de $ G $.

(v) $ \Rightarrow $ (i) : évident, car on a $ (\lambda b)(\lambda'b) = (\lambda + \lambda')b $ dans $ W $ pour $ |\lambda| $ et $ |\lambda'| $ assez petits.

(i) $ \Rightarrow $ (ii) : supposons vérifiée la condition (i). Soit $ b \in L $. Soit $ \psi $ la restriction de $ \varphi $ à $ V \cap Kb $. Par hypothèse, il existe un voisinage symétrique $ T $ de 0 dans le groupe de Lie additif $ Kb $ tel que $ \psi|T $ soit un morphisme du groupuscule de Lie $ T $ dans $ G $. Donc $ \varphi_*(b^n) = (\psi|T)_*(b^n) = ((\psi|T)_*(b))^n = (\varphi_*(b))^n $, de sorte que $ \varphi_*(b^n) $ est homogène de degré $ n $ dans $ U(G) $.

(iii) ⇒ (iv): l’application canonique de TS(L) dans l’algèbre enveloppante de L est l’unique morphisme de cogèbres graduées transformant 1 en 1 et prolongeant Id_L (chap. II, § 1, n° 5, Remarque 3). Or φ_* est un morphisme de cogèbres, et φ_*|L = Id_L par hypothèse. Si la condition (iii) est vérifiée, on voit que la condition (iv) l’est aussi.

(iv) ⇒ (v): supposons vérifiée la condition (iv). Choisissons une norme sur L définissant la topologie de L et telle que \| [x, y] \| ≤ \| x \| \| y \| quels que soient x, y dans L. Soit H le groupuscule de Lie défini par l’algèbre de Lie normée L. D’après le th. 1, il existe un sous-groupuscule ouvert S ⊂ V de H et un isomorphisme φ’ de S sur un sous-groupuscule ouvert de G. Comme on sait déjà que (v) ⇒ (iv), l’application φ’_* de TS(L) dans U(G) est l’application canonique de TS(L) dans l’algèbre enveloppante de L. Ainsi, φ_*(t) = φ’_*(t) pour tout t ∈ T_0^{(∞)}(L). Comme φ et φ’ sont analytiques, φ et φ’ coïncident dans un voisinage de 0.

#### Définition 1 {#lie-iii-s4-def-1 .statement}

Soient G un groupuscule de Lie, L son algèbre de Lie. On appelle application exponentielle de G toute application analytique φ, définie dans un voisinage ouvert de 0 dans L, à valeurs dans G, et vérifiant les conditions du th. 4.

Le th. 4 entraîne aussitôt que, pour tout groupuscule de Lie G, il existe une application exponentielle de G, et que deux applications exponentielles de G coïncident dans un voisinage de 0.

#### Exemple 1 {#lie-iii-s4-n3-exa-1 .statement}

Prenons pour G le groupe additif d’un espace normable complet E. L’isomorphisme canonique de L(G) sur E vérifie la condition (i) du th. 4, donc est une application exponentielle de G.

#### Exemple 2 {#lie-iii-s4-n3-exa-2 .statement}

Soit A une algèbre associative unifière normée complète. Soit A* le groupe de Lie formé par les éléments inversibles de A. Identifions L(A*) à A (§ 3, n° 9, cor. de la prop. 33). Si K = R ou C, on sait que l’application exp de A dans A* définie au chap. II, § 7, n° 3, vérifie la condition (i) du th. 4, donc est une application exponentielle. Soit maintenant K ultramétrique. Soit p la caractéristique du corps résiduel de K. Si p ≠ 0, posons λ = |p|^{1/(p-1)}; si p = 0, posons λ = 1. Soit U l’ensemble des x ∈ A tels que \| x \| < λ. On sait (chap. II, § 8, n° 4) que l’application exp de U dans A* vérifie la condition (i) du th. 4, donc est une application exponentielle. Remarquons que U est un sous-groupe additif de A.

Cet exemple explique la terminologie adoptée dans la déf. 1.

Soient G un groupuscule de Lie, φ une application exponentielle de G. Alors φ est étale en 0, donc il existe un voisinage ouvert U de 0 dans L(G) tel que φ(U) soit ouvert dans G et que φ|U soit un isomorphisme de la variété analytique U sur la variété analytique φ(U).

On appelle carte canonique (de première espèce) de G une carte ψ de la variété analytique G dont l’application réciproque est une application exponentielle. Si de plus G est de dimension finie et si on choisit une base de L(G), le système de coordonnées défini par ψ et par cette base dans le domaine de ψ s’appelle un système de coordonnées canoniques (de première espèce).

#### Proposition 3 {#lie-iii-s4-prop-3 .statement}

Soient G un groupuscule de Lie, L son algèbre de Lie, et φ une application exponentielle de G. Soient L₁, ..., Lₙ des sous-espaces vectoriels de L tels que L soit somme directe topologique de L₁, ..., Lₙ. L’application

$$(b₁, b₂, ..., bₙ) \mapsto θ(b₁, b₂, ..., bₙ) = φ(b₁)φ(b₂)...φ(bₙ),$$

définie dans une partie ouverte de L₁ × L₂ × ... × Lₙ, est analytique. L’application tangente en (0, 0, ..., 0) à θ est l’application canonique de L₁ × ... × Lₙ dans L.

Soit kᵢ l’injection canonique de Lᵢ dans L₁ × L₂ × ... × Lₙ. On a, pour tout b ∈ Lᵢ, $ (T_{(0,...,0)}θ)((T₀kᵢ)(b)) = (T₀φ)(b) = b $, donc $ (T_{(0,...,0)}θ)|Lᵢ $ est l’injection canonique de Lᵢ dans L.

En particulier, θ est étale en (0, 0, ..., 0). Sa restriction à un voisinage ouvert assez petit U de (0, 0, ..., 0) a une image ouverte dans G, et est un isomorphisme de la variété U sur la variété θ(U). L’application réciproque η de θ(U) sur U s’appelle une carte canonique de deuxième espèce de G, associée à la décomposition donnée de L en somme directe. Si de plus G est de dimension finie et si chaque Lᵢ est engendré par un vecteur non nul eᵢ, le système de coordonnées dans θ(U) défini par η et les eᵢ s’appelle un système de coordonnées canoniques de deuxième espèce.

#### Proposition 4 {#lie-iii-s4-prop-4 .statement}

Soient G un groupuscule de Lie, φ une application exponentielle injective de G. Quels que soient x, y dans L(G), on a

(1)
$$x + y = \lim_{λ ∈ K^*, λ → 0} λ^{-1}φ^{-1}(φ(λx)φ(λy))$$

(2)
$$[x, y] = \lim_{λ ∈ K^*, λ → 0} λ^{-2}φ^{-1}(φ(λx)φ(λy)φ(-λx)φ(-λy))$$

(on notera que $ φ^{-1}(φ(λx)φ(λy)) $ et $ φ^{-1}(φ(λx)φ(λy)φ(-λx)φ(-λy)) $ sont définis pour $ |λ| $ assez petit).

Munissions L = L(G) d’une norme définissant la topologie de L et telle que $ \| [x, y] \| ≤ \|x\| \|y\| $ quels que soient x, y dans L. Compte tenu des th. 2 et 4, on peut supposer que G est le groupuscule de Lie défini par L et que $ φ = \mathrm{Id}_G $. Notons $ (x, y) \mapsto x.y $ le produit dans le groupe G. Les formules à démontrer s’écrivent alors

(3)
$$x + y = \lim_{λ ∈ K^*, λ → 0} λ^{-1}((λx).(λy))$$

(4)
$$[x, y] = \lim_{λ ∈ K^*, λ → 0} λ^{-2}((λx).(λy).(-λx).(-λy)).$$

Il existe un voisinage ouvert V de 0 dans K tel que la fonction
$$
\lambda \mapsto f(\lambda) = (\lambda x) . (\lambda y)
$$
soit définie et analytique dans V. D’après le chap. II, § 6, n° 4, Remarque 2, le développement en série entière à l’origine de f est
$$
\lambda(x + y) + \frac{1}{2}\lambda^2[x, y] + \cdots
$$
et cela prouve (3). D’autre part, pour u, v dans G et \|u\|, \|v\| assez petits, u . v est une fonction analytique de (u, v) et les termes de degrés 1 et 2 dans le développement en série entière à l’origine de cette fonction sont $ u + v + \frac{1}{2}[u, v] $. D’après VAR, R, 3.2.7 et 4.2.3, les termes de degrés 1 et 2 dans le développement en série entière à l’origine de la fonction $ f(\lambda) . f(-\lambda) $ sont les termes de degrés 1 et 2 dans
$$
f(\lambda) + f(-\lambda) + \frac{1}{2}[f(\lambda), f(-\lambda)]
$$
ou encore dans
$$
\lambda(x + y) + \frac{1}{2}\lambda^2[x, y] - \lambda(x + y) + \frac{1}{2}\lambda^2[x, y] \\
+ \frac{1}{2}[\lambda(x + y), -\lambda(x + y)] = \lambda^2[x, y]
$$
et cela prouve (4).

#### Proposition 5 {#lie-iii-s4-prop-5 .statement}

*Soient G un groupe de Lie, k un sous-corps fermé non discret de K, G' le groupe G considéré comme groupe de Lie sur k, φ (resp. φ') une application exponentielle de G (resp. G'). Alors φ et φ' coïncident dans un voisinage de 0.*

En effet, φ vérifie l’hypothèse (i) du th. 4 relativement à G', donc est une application exponentielle de G'.

#### Proposition 6 {#lie-iii-s4-prop-6 .statement}

*Soient G un groupuscule de Lie, L son algèbre de Lie, φ : V → G une application exponentielle de G. Pour tout x ∈ V, identifions T_x(L) à L, de telle sorte que la différentielle droite ω(x) de φ en x soit une application linéaire de L dans L. Pour x assez voisin de 0, on a*
$$
\omega(x) = \sum_{n \geq 0} \frac{1}{(n + 1)!} (\operatorname{ad} x)^n.
$$

Munissons L d’une norme compatible avec sa topologie et telle que $ \| [x, y] \| \leq \| x \| \| y \| $ quels que soient $ x, y \in L $. Il suffit d’envisager le cas où G est le groupuscule de Lie défini par L, et où $ \varphi = \operatorname{Id}_G $. Par définition, $ \omega(x) $ est alors l’application tangente en x à l’application $ y \mapsto y . x^{-1} $ de G dans G. Si on note H(X, Y) la série de Hausdorff, $ \omega(x) $ est donc, pour $ \| x \| $ assez petit, l’application tangente en 0 à l’application $ y \mapsto H(x + y, -x) $ de G dans G. Dans H(X + Y, −X), la somme des termes du premier degré en Y est
$$
\sum_{m \geq 0} \frac{1}{(m + 1)!} (\operatorname{ad} X)^m Y
$$
(chap. II, § 6, n° 5, prop. 5). La proposition résulte alors de VAR, R, 3.2.4 et 4.2.3.

Soient G un groupuscule de Lie, et $ t \in K $. On appelle *application puissance t-ème de* G toute application, définie et analytique dans un voisinage ouvert de $ e $, à valeurs dans G, et coïncidant dans un voisinage de $ e $ avec une application

$$
g \mapsto \varphi(t \varphi^{-1}(g))
$$

où $ \varphi $ est une application exponentielle injective de G.

#### Proposition 7 {#lie-iii-s4-prop-7 .statement}

(i) *Si* $ t \in \mathbf{Z} $, *une application puissance t-ème coïncide dans un voisinage de* $ e $ *avec l’application* $ g \mapsto g^t $.

(ii) *L’application tangente en* $ e $ *à une application puissance t-ème est l’homothétie de rapport* $ t $.

(iii) *Si* $ h $ *est une application puissance t-ème et* $ h' $ *une application puissance t'-ème de* G, $ h \circ h' $ *est une application puissance* $ (tt') $-ème, *et* $ g \mapsto h(g)h'(g) $ *est une application puissance* $ (t + t') $-ème.

(iv) *Si* $ h $ *est une application puissance t-ème, et si* $ u \in U^n(G) $, *on a* $ h_*(u) = t^n u $.

Il suffit de prouver la proposition quand G est le groupuscule de Lie défini par une algèbre de Lie normée complète, et quand les applications puissance t-ème considérées sont construites à l’aide de l’application exponentielle $ \varphi = \mathrm{Id}_G $. Mais alors tout est évident.

### 4. Fonctorialité des applications exponentielles

#### Proposition 8 {#lie-iii-s4-prop-8 .statement}

*Soient* G *et* H *des groupuscules de Lie, h un morphisme de* G *dans* H, $ \varphi_G $ *et* $ \varphi_H $ *des applications exponentielles relativement à* G *et* H. *Il existe un voisinage* V *de* 0 *dans* L(G) *tel que* $ h \circ \varphi_G $ *et* $ \varphi_H \circ L(h) $ *coïncident dans* V.

Munissons L(G) et L(H) de normes définissant leurs topologies et telles que $ \| [x, y] \| \leq \| x \| \| y \| $ quels que soient $ x $ et $ y $. On peut supposer que G (resp. H) est le groupuscule de Lie défini par L(G) (resp. L(H)), de sorte que $ \varphi_G $ (resp. $ \varphi_H $) coïncide avec $ \mathrm{Id}_G $ (resp. $ \mathrm{Id}_H $) au voisinage de 0. D’autre part, il existe un voisinage ouvert symétrique W de 0 dans L(G) tel que L(h) soit un morphisme du groupuscule de Lie W dans H. D’après le th. 1, L(h) coïncide avec $ h $ dans un voisinage de 0, d’où la proposition.

En termes imagés, si l’on identifie G et H au voisinage de l’élément neutre à L(G) et L(H) grâce à des applications exponentielles, tout morphisme de G dans H est *linéaire* au voisinage de 0.

#### Corollaire 1 {#lie-iii-s4-prop-8-cor-1 .statement}

*Soient* G *un groupuscule de Lie, G' un sous-groupuscule de Lie de* G, $ \varphi $ *une application exponentielle de* G.

(i) *Il existe un voisinage ouvert* V *de* 0 *dans* L(G') *tel que* $ \varphi|V $ *soit un isomorphisme de la variété* V *sur un voisinage ouvert de* e *dans* G'.

(ii) Soit $ x \in L(G) $. Les conditions suivantes sont équivalentes : a) $ x \in L(G') $; b) $ \varphi(\lambda x) \in G' $ pour $ |\lambda| $ assez petit.
(i) s’obtient en appliquant la prop. 8 à l’injection canonique de $ G' $ dans $ G $, et (ii) résulte de (i).

#### Corollaire 2 {#lie-iii-s4-prop-8-cor-2 .statement}

Soient $ G $ un groupe de Lie, $ \rho $ une représentation linéaire analytique de $ G $, $ \varphi $ une application exponentielle de $ G $. Il existe un voisinage $ V $ de $ 0 $ dans $ L(G) $ tel que
$$
\rho(\varphi(x)) = \exp(L(\rho)x)
$$
pour tout $ x \in V $.
Cela résulte de la prop. 8 et de l’Exemple 2 du n° 3.

#### Corollaire 3 {#lie-iii-s4-prop-8-cor-3 .statement}

Soient $ G $ un groupe de Lie, $ \varphi $ une application exponentielle de $ G $.
(i) Il existe un voisinage $ V $ de $ 0 $ dans $ L(G) $ tel que
$$
\mathrm{Ad}(\varphi(x)) = \exp \mathrm{ad}\, x
$$
pour tout $ x \in V $.
(ii) Si $ g \in G $, il existe un voisinage $ W $ de $ 0 $ dans $ L(G) $ tel que
$$
g \varphi(x) g^{-1} = \varphi(\mathrm{Ad}\, g.x)
$$
pour tout $ x \in W $.
(i) résulte du cor. 2, et du § 3, n° 12, prop. 44.
(ii) résulte de la prop. 8 appliquée à Int $ g $.

### 5. Structure induite sur un sous-groupe

#### Lemme 4 {#lie-iii-s4-lem-4 .statement}

Soient $ G $ un groupe de Lie de dimension finie, $ \Omega $ un voisinage ouvert symétrique de $ e $ dans $ G $, $ H $ un sous-ensemble de $ \Omega $ contenant $ e $, tel que les conditions $ x \in H, y \in H, xy^{-1} \in \Omega $ entraînent $ xy^{-1} \in H $. Soit $ r \in \mathbf{N}_K $. Pour tout $ x \in H $, soit $ h_x $ l’ensemble des $ a \in T_x(G) $ possédant la propriété suivante : il existe un voisinage ouvert $ I $ de $ 0 $ dans $ K $, et une application de classe $ C^r $ de $ I $ dans $ G $, tels que $ f(0) = x, f(I) \subset H, (T_0f)(1) = a $.
(i) Posons $ h_e = h $. Alors $ h $ est une sous-algèbre de Lie de $ L(G) $, invariant par $ \mathrm{Ad}_{L(G)}(H) $.
(ii) On a $ h_x = xh = hx $ pour tout $ x \in H $ ($ xh $ et $ hx $ étant calculés dans $ T(G) $).
(iii) Soient $ V $ une variété de classe $ C^r $, $ v_0 $ un point de $ V $, $ f $ une application de classe $ C^r $ de $ V $ dans $ G $ telle que $ f(v_0) = e $ et $ f(V) \subset H $. Quel que soit le sous-groupuscule de Lie $ H' $ de $ G $ d’algèbre de Lie $ h $, on $ af(v) \in H' $ pour $ v $ assez voisin de $ v_0 $.
(iv) Quel que soit le sous-groupuscule de Lie $ H' $ de $ G $ d’algèbre de Lie $ h $, $ H' \cap H $ est un voisinage de $ e $ dans $ H' $.
(v) Pour tout $ x \in H $ et tout $ a \in h_x $, il existe un voisinage ouvert $ I $ de $ 0 $ dans $ K $, et une application de classe $ C^o $ de $ I $ dans $ G $ telle que $ f(0) = x, f(I) \subset H, (T_0f)(1) = a $.
Il est clair que $ Kh = h $, et que $ xh_{yz} = h_{xyz} $ pour $ x, y, xy, xyz $ dans $ H $. Cela entraîne (ii) et le fait que $ h $ est invariant par $ \mathrm{Ad}_{L(G)}(H) $.

Soient $ V, v_0, f $ comme dans (iii). Soit $ Y $ le feuilletage gauche de $ G $ associé à $ \mathfrak{h} $ (n° 1). Pour tout $ y \in H' $, on a $ T_y(H') = y \mathfrak{h} $. D’autre part, pour tout $ v \in V $, l’image de $ T_v(V) $ par $ T_v(f) $ est contenue dans $ \mathfrak{h}_{f(v)} = f(v) \mathfrak{h} $ (par définition de $ \mathfrak{h}_{f(v)} $). D’après VAR, R, 9.3.2, $ f $ est un morphisme de $ V $ dans $ Y $. Comme $ H' $ est une feuille de $ Y $ (VAR, R, 9.2.8), on a $ f(v) \in H' $ pour $ v $ assez voisin de $ v_0 $.

Soit $ (a_1, \ldots, a_s) $ une base de $ \mathfrak{h} $. Il existe un voisinage ouvert $ I $ de $ 0 $ dans $ K $, et des applications $ f_1, \ldots, f_s $ de classe $ C^r $ de $ I $ dans $ G $, telles que $ f_j(0) = e, f_j(I) \subset H, (Tf_j)1 = a_j $ pour tout $ j $. D’après (iii), on a $ f_j(\lambda) \in H' $ pour $ |\lambda| $ assez petit. Donc les $ f_1(\lambda_1) f_2(\lambda_2) \ldots f_s(\lambda_s) $ constituent, pour $ |\lambda_1|, \ldots, |\lambda_s| $ assez petits, un voisinage de $ e $ dans $ H' $; et ce voisinage est contenu dans $ H $. D’où (iv).

Si $ a \in \mathfrak{h} $, il existe un voisinage ouvert $ I $ de $ 0 $ dans $ K $ et une application de classe $ C^\omega $ de $ I $ dans $ G $ tels que $ f(0) = e, f(I) \subset H', (T_0 f)1 = a $. Cela, avec (iv), entraîne (v).

#### Définition 2 {#lie-iii-s4-def-2 .statement}

On dit que $ \mathfrak{h} $ est la sous-algèbre tangente à $ H $ en $ e $.

#### Proposition 9 {#lie-iii-s4-prop-9 .statement}

Soient $ G $ un groupe de Lie de dimension finie, $ H $ un sous-groupe de $ G $.

(i) Il existe sur $ H $ une structure de variété analytique et une seule ayant la propriété suivante: pour tout $ r $ compris entre $ 1 $ et $ \omega $, pour toute variété $ V $ de classe $ C^r $, et pour toute application $ f $ de $ V $ dans $ H $, $ f $ est de classe $ C^r $ comme application de $ V $ dans $ H $ si et seulement si $ f $ est de classe $ C^r $ comme application de $ V $ dans $ G $.

(ii) Pour cette structure, $ H $ est un groupe de Lie, l’injection canonique $ i $ de $ H $ dans $ G $ est une immersion, et $ L(i)(L(H)) $ est la sous-algèbre de Lie tangente en $ e $ à $ H $.

Dans (i), l’unicité est évidente. Prouvons l’existence. Soit $ \mathfrak{h} $ l’algèbre de Lie tangente en $ e $ à $ H $. Soit $ H' $ un sous-groupuscule de Lie de $ G $ d’algèbre de Lie $ \mathfrak{h} $. En remplaçant $ H' $ par un sous-groupuscule ouvert de $ H' $, on peut supposer $ H' \subset H $ (lemme 4 (iv)). Pour tout $ x \in H $, $ x H' x^{-1} $ est un sous-groupuscule de Lie de $ G $ d’algèbre de Lie $ x h x^{-1} = h $. Donc $ H' \cap (x H' x^{-1}) $ est ouvert dans $ H' $ (n° 2, th. 3), et l’application $ y \mapsto xy x^{-1} $ est un isomorphisme de $ H' \cap x^{-1} H' x $ sur $ x H' x^{-1} \cap H' $. Compte tenu de la prop. 18 du § 1, n° 9, il existe un sous-groupuscule de Lie ouvert W de H', et une structure de groupe de Lie sur H, possédant les propriétés suivantes : W est ouvert dans H, et les structures de variétés de H et H' induisent la même structure sur W. Il résulte de là que l’injection canonique i de H dans G est une immersion, et que L(i)(L(H)) = L(H') = 𝔤. En outre, soient V et f comme dans (i). Si f : V → H est de classe C^r, i ∘ f : V → G est de classe C^r. Supposons que i ∘ f : V → G soit de classe C^r, et prouvons que f : V → H est de classe C^r. Par translation, il suffit d’envisager le cas où il existe un v_0 ∈ V tel que f(v_0) = e, et de prouver que f : V → H est de classe C^r dans un voisinage ouvert de v_0. Or, d’après le lemme 4 (iii), on a f(v) ∈ H' pour v assez voisin de v_0, d’où notre assertion. On a ainsi prouvé (i), et (ii) a été obtenu en cours de route.

#### Définition 3 {#lie-iii-s4-def-3 .statement}

La structure de groupe de Lie sur H définie dans la prop. 9 s’appelle la structure induite sur H par la structure de groupe de Lie de G.

Si H est un sous-groupe de Lie de G, sa structure de groupe de Lie est induite par celle de G (VAR, R, 5.8.5).

Si G = R et H = Q, on a 𝔤 = {0}, donc la structure induite sur H est la structure de groupe de Lie discret. De même si G = C (considéré comme groupe de Lie complexe) et H = R.

### 6. Primitives des formes différentielles à valeurs dans une algèbre de Lie

#### Lemme 5 {#lie-iii-s4-lem-5 .statement}

Soient X une variété de classe C^r, F et F' des fibrés vectoriels de classe C^r et de base X, φ un morphisme de F dans F'. Pour tout x ∈ X, soit S_x l’ensemble des
$$(a, φ(a)) ∈ F_x ⊕ F'_x$$
pour $a ∈ F_x$. Alors la réunion S des S_x est un sous-fibré vectoriel de F ⊕ F'.

Soient θ et θ' les applications de F ⊕ F' dans lui-même définies de la manière suivante : si $(u, v) ∈ F_x ⊕ F'_x$, on a
$$\theta(u, v) = (u, v + φ(u)), \quad \theta'(u, v) = (u, v - φ(u)).$$
D’après VAR, R, 7.7.1, θ et θ' sont des morphismes du fibré vectoriel F ⊕ F' dans lui-même. Il est clair que $θ ∘ θ' = θ' ∘ θ = \mathrm{Id}_{F ⊕ F'}$. Donc θ et θ' sont des automorphismes de F ⊕ F'. Par suite, S = θ(F ⊕ {0}) est un sous-fibré vectoriel de F ⊕ F'.

#### Lemme 6 {#lie-iii-s4-lem-6 .statement}

Soient G un groupuscule de Lie, ω la forme différentielle gauche canonique de G (\S 3, n° 18.9), M une variété de classe C^r (r ≥ 2), α une forme différentielle de classe C^{r-1} et de degré 1 sur M, à valeurs dans L(G).

(i) Les éléments de $ T(M \times G) $ en lesquels s’annule la forme différentielle
$$
\theta = \mathrm{pr}_1^* \alpha - \mathrm{pr}_2^* \omega
$$
constituent un sous-fibré vectoriel $ S $ de classe $ C^{r-1} $ de $ T(M \times G) $.

(ii) Pour tout $ (x, g) \in M \times G $, $ T(\mathrm{pr}_1)|_{S_{(x,g)}} $ est un isomorphisme de $ S_{(x,g)} $ sur $ T_x(M) $.

(iii) Si $ d\alpha + [\alpha]^2 = 0 $ (cf. § 3, n° 14) le sous-fibré vectoriel $ S $ est intégrable.
Si $ (x, g) \in M \times G $ et $ (u, v) \in T_x(M) \times T_g(G) $, on a
$$
\theta_{(x,g)}(u, v) = \alpha(u) - g^{-1}v.
$$
Donc le noyau de $ \theta_{(x,g)} $ est l’ensemble $ S_{(x,g)} $ des $ (u, g\alpha(u)) $ pour $ u \in T_x(M) $, d’où (ii). Considérons $ T(M \times G) $ comme la somme directe de deux fibrés vectoriels $ F $ et $ F' $ avec $ F_{(x,g)} = T_x(M) \times \{0\} $ et $ F'_{(x,g)} = \{0\} \times T_g(G) $ pour tout
$$
(x, g) \in M \times G.
$$
Pour $ u \in T_x(M) \times \{0\} $, posons $ \varphi(u) = (0, g\alpha(u)) $. En utilisant la trivialisation gauche de $ T(G) $, on voit que $ \varphi $ est un morphisme de $ F $ dans $ F' $, d’où (i) (lemme 5).
Enfin, si $ d\alpha + [\alpha]^2 = 0 $, on a
$$
\begin{align*}
d\theta &= \mathrm{pr}_1^*(d\alpha) - \mathrm{pr}_2^*(d\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha \wedge \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega \wedge \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega) \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}\theta \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega)
\end{align*}
$$
donc $ S $ est intégrable (VAR, R, 9.3.6).

#### Théorème 5 {#lie-iii-s4-thm-5 .statement}

Soient $ G $ un groupuscule de Lie, $ M $ une variété de classe $ C^r $ ($ r \geq 2 $), $ \alpha $ une forme différentielle de classe $ C^{r-1} $ et de degré 1 sur $ M $ à valeurs dans $ L(G) $, telle que $ d\alpha + [\alpha]^2 = 0 $. Pour tout $ x \in M $ et tout $ g \in G $, il existe une application $ f $, définie et de classe $ C^{r-1} $ dans un voisinage ouvert de $ x $, à valeurs dans $ G $, telle que $ f(x) = g $ et $ f^{-1}.df = \alpha $. Deux applications qui vérifient ces conditions coïncident dans un voisinage de $ x $.

Soient $ x \in M $ et $ g \in G $. D’après le lemme 6 (dont nous adoptons les notations) et VAR, R, 9.3.7, il existe un voisinage ouvert $ U $ de $ x $ dans $ M $ et une application $ m \mapsto \varphi(m) = (m, f(m)) $ de classe $ C^{r-1} $ de $ U $ dans $ M \times G $ telle que $ f(x) = g $ et que $ \varphi^*(\theta) = 0 $. Alors
$$
\begin{align*}
f^{-1}.df &= f^*(\omega) & (\text{§ 3, n° 18.9}) \\
&= (\mathrm{pr}_2 \circ \varphi)^*(\omega) & (\text{car } f = \mathrm{pr}_2 \circ \varphi) \\
&= \varphi^*(\mathrm{pr}_1^*\alpha - \theta) & (\text{lemme 6}) \\
&= \varphi^*(\mathrm{pr}_1^*\alpha) & (\text{car } \varphi^*(\theta) = 0) \\
&= \alpha & (\text{car } \mathrm{pr}_1 \circ \varphi = \mathrm{Id}_U).
\end{align*}
$$

#### Proposition 10 {#lie-iii-s4-prop-10 .statement}

*Soient $ M $ une variété analytique, $ g $ une algèbre de Lie normable complète, $ \alpha $ une forme différentielle de degré 1 analytique sur $ M $, à valeurs dans $ g $, possédant les propriétés suivantes*:
    *a)* pour tout $ m \in M $, $ \alpha_m $ est un isomorphisme de $ T_m(M) $ sur $ g $;
    *b)* $ d\alpha + [\alpha]^2 = 0 $.
*Alors, pour tout $ m_0 \in M $, il existe un voisinage ouvert $ M' $ de $ m_0 $ dans $ M $, et une structure de groupuscule de Lie sur $ M' $, compatible avec la structure de variété de $ M' $, d’élément neutre $ m_0 $, ayant les propriétés suivantes*:
    *(i)* $ \alpha_{m_0} $ est un isomorphisme de $ L(M') $ sur $ g $;
    *(ii)* *la forme différentielle* $ m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m $ *est la forme différentielle canonique gauche de* $ M' $.
*Si $ M'_1 $ et $ M'_2 $ sont deux tels groupuscules, $ M'_1 $ et $ M'_2 $ possèdent un sous-groupuscule ouvert commun*.

Il existe un groupuscule de Lie $ G $ tel que $ L(G) = g $. Soit $ m_0 \in M $. D’après le th. 5, il existe un voisinage ouvert $ M' $ de $ m_0 $ dans $ M $ et une application analytique $ f $ de $ M' $ dans $ G $ telle que $ f(m_0) = e $ et $ f^{-1}.df = \alpha $. Alors $ T_{m_0}(f) = \alpha_{m_0} $ est un isomorphisme de $ T_{m_0}(M) $ sur $ g $; donc, en diminuant $ M' $ et $ G $, on peut supposer que $ f $ est un isomorphisme de la variété $ M' $ sur la variété $ G $. Transportons à $ M' $ la structure de groupuscule de Lie de $ G $ grâce à $ f^{-1} $. Alors $ T_{m_0}(f) $ devient un isomorphisme de $ L(M') $ sur $ L(G) = g $, d’où (i). D’autre part, en notant $ \omega $ la forme différentielle canonique gauche de $ G $, on a
$$
\alpha_{m_0}^{-1} \circ \alpha_m = (T_{m_0}f)^{-1} \circ (f^{-1}.df)(m)
= (T_{m_0}f)^{-1} \circ \omega(f(m)) \circ T_m f
$$
donc $ m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m $ est la forme différentielle canonique gauche de $ M' $.

Soit $ M'' $ un voisinage ouvert de $ m_0 $, muni d’une structure de groupuscule de Lie, d’élément neutre $ m_0 $, avec les propriétés analogues aux propriétés (i) et (ii). Alors $ \alpha_{m_0} $ est un isomorphisme de $ L(M') $ sur $ g $, et aussi de $ L(M'') $ sur $ g $, donc $ L(M') = L(M'') $. Par suite, en diminuant $ M' $ et $ M'' $, on peut supposer qu’il existe un isomorphisme $ \varphi $ du groupuscule $ M' $ sur le groupuscule $ M'' $ (n° 1, cor. 1 du th. 1). Alors $ \varphi^{-1}.d\varphi $ est la différentielle gauche canonique de $ M' $. D’autre part, soit $ \psi $ l’injection canonique de la variété $ M' \cap M'' $ dans le groupuscule de Lie $ M'' $; il est clair que $ \psi^{-1}.d\psi $ est une restriction de la différentielle gauche canonique de $ M'' $. Donc $ (\psi^{-1}.d\psi)(m) = \alpha_{m_0}^{-1} \circ \alpha_m = (\varphi^{-1}.d\varphi)(m) $ pour tout $ m \in M' \cap M'' $. Par suite $ \varphi $ et $ \psi $ coïncident dans un voisinage de $ m_0 $ (§ 3, 18.9). Cela prouve la dernière assertion de la proposition.

#### Corollaire {#lie-iii-s4-n6-cor-1 .statement}

Soit $ M $ une variété analytique de dimension finie $ n $. Soient $ \omega_1, \ldots, \omega_n $ des formes différentielles analytiques de degré 1 sur $ M $, à valeurs scalaires, linéairement indépendantes en tout point de $ M $, et telles que, pour tout $ k = 1, \ldots, n $, $ d\omega_k $ soit combinaison linéaire à coefficients constants des $ \omega_i \wedge \omega_j $. Alors, pour tout $ m_0 \in M $, il existe un voisinage ouvert $ M' $ de $ m_0 $ dans $ M $, et une structure de groupuscule de Lie sur $ M' $, compatible avec la structure de variété de $ M' $, d’élément neutre $ m_0 $, et telle que $ \omega_1|_{M'}, \ldots, \omega_n|_{M'} $ forment une base de l’espace des formes différentielles de degré 1 à valeurs scalaires invariantes à gauche sur $ M' $.

Si $ M'_1 $ et $ M'_2 $ sont deux tels groupuscules, $ M'_1 $ et $ M'_2 $ possèdent un sous-groupuscule ouvert commun.

Soient $ X_1, \ldots, X_n $ les champs de vecteurs sur $ M $ tels que, en chaque point $ m $ de $ M $, les $ (X_i)_m $ constituent la base de $ T_m(M) $ duale de $ ((\omega_1)_m, \ldots, (\omega_n)_m) $. Ces champs sont analytiques. Par hypothèse, il existe des $ c_{ijk} \in K $ ($ 1 \leq i, j, k \leq n $) tels que $ c_{ijk} = -c_{jik} $ et que $ d\omega_k = \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j $. D’après VAR, R, 8.5.7, formule (11), on en déduit

$$
\langle [X_i, X_j], \omega_k \rangle = - (d\omega_k)(X_i, X_j) = - \left( \sum_{r < s} c_{rsk} \omega_r \wedge \omega_s \right)(X_i, X_j) = - c_{ijk}
$$

donc $[X_i, X_j] = - \sum_k c_{ijk} X_k$. Il résulte de là que les $ -c_{ijk} $ sont les constantes de structure d’une algèbre de Lie $ g $ relativement à une base $ (e_1, \ldots, e_n) $. Pour tout $ m \in M $, soit $ \alpha_m $ l’application linéaire de $ T_m(M) $ dans $ g $ qui transforme $ (X_1)_m $ en $ e_1, \ldots, (X_n)_m $ en $ e_n $. Alors $ \alpha $ est une forme différentielle de degré 1 analytique sur $ M $ à valeurs dans $ g $, et $ \alpha_m $ est un isomorphisme de $ T_m(M) $ sur $ g $. D’autre part, $ \alpha = \sum_{k=1}^n \omega_k e_k $, donc

$$
d\alpha = \sum_{k=1}^n (d\omega_k) e_k = \sum_{k=1}^n \left( \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j \right) e_k
$$

et

$$
\begin{align*}
(\alpha)^2 &= \sum_{k=1}^n [\omega_k e_k]^2 + \sum_{i < j} (\omega_i e_i) \wedge (\omega_j e_j) \quad (\S 3, \text{formule (30)}) \\
&= \sum_{i < j} (\omega_i \wedge \omega_j)[e_i, e_j] \\
&= - \sum_{k=1}^n \sum_{i < j} (c_{ijk} \omega_i \wedge \omega_j) e_k \\
&= - d\alpha.
\end{align*}
$$

Il suffit alors d’appliquer la prop. 10.

### 7. Passage des lois d’opérations infinitésimales aux lois d’opérations

#### Proposition 11 {#lie-iii-s4-prop-11 .statement}

Soient $ G_1 $ et $ G_2 $ des groupuscules de Lie, $ X_1 $ et $ X_2 $ des variétés de classe $ C^r $ ($ r \geqslant 2 $). Pour $ i = 1, 2 $, soient $ \psi_i $ un morceau de loi d’opération à gauche de classe $ C^r $ de $ G_i $ dans $ X_i $, $ D_i $ la loi d’opération infinitésimale associée. Soient $ \mu : G_1 \to G_2 $ un morphisme, $ \varphi : X_1 \to X_2 $ une application de classe $ C^r $. On suppose que, pour tout $ a \in L(G) $, les champs de vecteurs $ (D_1)_a $ et $ (D_2)_{L(\mu)a} $ soient $ \varphi $-liés (VAR, R, 8.2.6). Alors, il existe un voisinage $ \Omega $ de $ \{e\} \times X_1 $ dans $ G_1 \times X_1 $ tel que $ \varphi(\psi_1(g, x)) = \psi_2(\mu(g), \varphi(x)) $ pour tout $ (g, x) \in \Omega $.

Soient $ p_1 : G_1 \times X_2 \to G_1 $, $ p_2 : G_1 \times X_2 \to X_2 $ les projections canoniques. Pour tout $ (g_1, x_2) \in G_1 \times X_2 $, soit $ f_{g_1, x_2} $ l’application $ g_1 a \mapsto (D_2)_{L(\mu)a}(x_2) $ de $ T_{g_1}(G_1) = g_1 L(G_1) $ dans $ T_{x_2}(X_2) $. Les $ f_{g_1, x_2} $ définissent un morphisme de $ p_1^*T(G_1) $ dans $ p_2^*T(X_2) $.

Soit $ x_0 \in X_1 $. Il existe un voisinage ouvert $ G $ de $ e $ dans $ G_1 $ et un voisinage ouvert $ X $ de $ x_0 $ dans $ X_1 $ tels que $ \psi_1(g, x) $ et $ \psi_2(\mu(g), \varphi(x)) $ soient définis pour $ (g, x) \in G \times X $. Posons, pour $ (g, x) \in G \times X $,
$$
\alpha(g, x) = \varphi(\psi_1(g, x)) \in X_2, \qquad \beta(g, x) = \psi_2(\mu(g), \varphi(x)) \in X_2.
$$
Si $ G $ et $ X $ sont assez petits, on a, pour tout $ (a, g, x) \in L(G_1) \times G \times X $,
$$
(T\alpha)(ag, 0_x) = (T\varphi)((D_1)_a(\psi_1(g, x)))
= (D_2)_{L(\mu)a}(\varphi(\psi_1(g, x)))
= (D_2)_{L(\mu)a}\alpha(g, x),
$$
$$
(T\beta)(ag, 0_x) = (T\psi_2)(L(\mu)a.\mu(g), \varphi(x))
= (D_2)_{L(\mu)a}(\psi_2(\mu(g), \varphi(x)))
= (D_2)_{L(\mu)a}\beta(g, x).
$$
Donc pour $ x \in X $, les morphismes $ g \mapsto \alpha(g, x) $ et $ g \mapsto \beta(g, x) $ sont des intégrales de $ f $; comme
$$
\beta(e, x) = \varphi(x) = \alpha(e, x)
$$
pour tout $ x \in X $, on conclut de VAR, R, 9.3.7, que $ \alpha $ et $ \beta $ coïncident dans un voisinage de $ (e, x_0) $. D’où la proposition.

#### Corollaire {#lie-iii-s4-n7-cor-1 .statement}

Soient $ G $ un groupuscule de Lie, $ X $ une variété de classe $ C^r $. Considérons deux morceaux de lois d’opérations à gauche de classe $ C^r $ de $ G $ dans $ X $. On suppose que, pour tout $ a \in L(G) $, le champ de vecteurs correspondant $ D_a $ sur $ X $ soit le même pour les deux morceaux de lois. Alors ces dans deux morceaux de lois coïncident dans un voisinage de $ \{e\} \times X $.

#### Théorème 6 {#lie-iii-s4-thm-6 .statement}

Soient $ G $ un groupuscule de Lie, $ X $ une variété de classe $ C^r $ ($ r \geqslant 2 $), et $ x_0 $ un point de $ X $. Soit $ a \mapsto D_a $ une loi d’opération infinitésimale à gauche de classe $ C^{r-1} $ de $ L(G) $ dans $ X $.

(i) Il existe un voisinage ouvert $ X' $ de $ x_0 $ dans $ X $, et un morceau de loi d’opération à gauche de classe $ C^{r-1} $ de $ G $ dans $ X' $ tels que la loi d’opération infinitésimale associée soit $ a \mapsto D_a|_{X'} $.

(ii) Soient deux morceaux de lois d’opérations à gauche de classe $ C^{r-1} $ de $ G $ dans un voisinage ouvert $ X'' $ de $ x_0 $; s’ils admettent $ a \mapsto D_a|X'' $ comme loi d’opération infinitésimale associée, ils coïncident dans un voisinage de $ (e, x_0) $.

L’assertion (ii) résulte du cor. de la prop. 11. Prouvons (i). Pour tout $ (g, x) \in G \times X $ et tout $ a \in L(G) $, posons

$$
Q_a(g, x) = (ag, D_a(x)) \in T_g(G) \times T_x(X).
$$

Soit $ S_{(g, x)} $ l’ensemble des $ Q_a(g, x) $ pour $ a \in L(G) $. D’après le lemme 5 du n° 6, les $ S_{(g, x)} $ sont les fibres d’un sous-fibré vectoriel $ S $ de $ T(G) \times T(X) $. Soient $ a, b $ dans $ L(G) $; on a

$$
\begin{align*}
[Q_a, Q_b](g, x) &= ([R_a, R_b](g), [D_a, D_b](x)) \\
&= (-R_{[a, b]}(g), -D_{[a, b]}(x)) \tag{\S 3, 18.6} \\
&= Q_{-[a, b]}(g, x)
\end{align*}
$$

donc $ S $ est intégrable (VAR, R, 9.3.3 (iv)).

D’après VAR, R, 9.3.7, il existe un voisinage ouvert $ G_1 $ de $ e $ dans $ G $, un voisinage ouvert $ X_1 $ de $ x_0 $ dans $ X $, et une application $ (g, x) \mapsto gx $ de classe $ C^{r-1} $ de $ G_1 \times X_1 $ dans $ X $, tels que $ ex = x $ pour tout $ x \in X_1 $, et

$$(6)$$
$$(ag)x = D_a(gx) \quad \text{pour } a \in L(G), g \in G_1, x \in X_1.$$

En particulier

$$(7)$$
$$ax = D_a(x).$$

Soient $ G_2 $ un voisinage ouvert de $ e $ dans $ G_1 $ et $ X_2 $ un voisinage ouvert de $ x_0 $ dans $ X_1 $ tels que $ gg' $ soit défini et appartienne à $ G_1 $ pour $ g, g' $ dans $ G_2 $, et que $ gx $ soit défini et appartienne à $ X_1 $ pour $ (g, x) \in G_2 \times X_2 $. Considérons les applications $ \alpha_1, \alpha_2 $ de $ G_2 \times (G_2 \times X_2) $ dans $ X $ définies par

$$\alpha_1(g, (h, x)) = g(hx), \qquad \alpha_2(g, (h, x)) = (gh)x.$$

Elles sont de classe $ C^{r-1} $. On a

$$\alpha_1(e, (h, x)) = hx = \alpha_2(e, (h, x)).$$

D’autre part

$$
\begin{align*}
T(\alpha_1)(ag, 0_{(h, x)}) &= (ag)(hx) \\
&= D_a(g(hx)) \qquad \text{d’après (6)} \\
&= D_a(\alpha_1(g, (h, x))), \\
T(\alpha_2)(ag, 0_{(h, x)}) &= (agh)x \\
&= D_a((gh)x) \qquad \text{d’après (6)} \\
&= D_a(\alpha_2(g, (h, x))).
\end{align*}
$$

D’après VAR, R, 9.3.7, $ \alpha_1 $ et $ \alpha_2 $ coïncident dans un voisinage de $ (e, (e, x_0)) $. Ceci posé, (i) résulte de (7) et de la prop. 23 du § 1, n° 11.

#### Corollaire 1 {#lie-iii-s4-thm-6-cor-1 .statement}

Soient G un groupuscule de Lie, X une variété paracompacte de classe $ C^r $ ($ r \geq 2 $). Soit $ a \mapsto D_a $ une loi d’opération infinitésimale à gauche de classe $ C^{r-1} $ de $ L(G) $ dans X.

(i) Il existe un morceau de loi d’opération à gauche de classe $ C^{r-1} $ de G dans X tel que la loi d’opération infinitésimale associée soit $ a \mapsto D_a $.

(ii) Deux lois d’opérations à gauche de classe $ C^{r-1} $ de G dans X, qui admettent $ a \mapsto D_a $ comme loi d’opération infinitésimale associée, coïncident dans un voisinage de $ \{e\} \times X $.

L’assertion (ii) résulte du cor. de la prop. 11. D’après le th. 6 (i), il existe un recouvrement ouvert $ (X_i)_{i \in I} $ de X, et, pour tout $ i \in I $, un morceau de loi d’opération à gauche $ \psi_i $ de classe $ C^{r-1} $ de G dans $ X_i $, tels que la loi d’opération infinitésimale associée soit $ a \mapsto D_a | X_i $. Comme X est paracompacte, on peut supposer le recouvrement $ (X_i)_{i \in I} $ localement fini. Pour tout $ (i, j) \in I \times I $ et tout $ x \in X_i \cap X_j $, $ \psi_i $ et $ \psi_j $ coïncident dans un voisinage de $ (e, x) $ (cor. de la prop. 11). Comme X est normale, on peut appliquer la prop. 24 du § 1, n° 11, ce qui prouve (i).

#### Corollaire 2 {#lie-iii-s4-thm-6-cor-2 .statement}

Soient X une variété paracompacte de classe $ C^r $ ($ r \geq 2 $), et $ \xi $ un champ de vecteurs de classe $ C^{r-1} $ sur X. Il existe un morceau de loi d’opération $ \psi $ de classe $ C^{r-1} $ de K dans X tel que, pour tout $ x \in X $, $ \xi(x) $ soit l’image par $ t \mapsto \psi(t, x) $ du vecteur tangent 1 à K en 0. Deux morceaux de lois d’opérations possédant la propriété précédente coïncident dans un voisinage de $ \{0\} \times X $.

C’est un cas particulier du cor. 1.

#### Remarque {#lie-iii-s4-n7-rem-1 .statement}

On peut bien entendu remplacer partout, dans ce n°, les lois d’opérations à gauche par les lois d’opérations à droite.

## EXERCICES {#lie-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
