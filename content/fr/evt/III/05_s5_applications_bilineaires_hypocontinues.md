---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 5
section_title: Applications bilinéaires hypocontinues
lang: fr
source: evt-i-v-fr
book_pages: EVT III.28-EVT III.34, EVT III.48-EVT III.50
pdf_pages: 0163-0169, 0183-0185
extraction: ocr
subsections:
    - "no": 1
      title: Applications bilinéaires séparément continues
      page: 28
      pdf_page: 163
    - "no": 2
      title: Applications bilinéaires séparément continues sur un produit d’espaces de Fréchet
      page: 30
      pdf_page: 165
    - "no": 3
      title: Applications bilinéaires hypocontinues
      page: 31
      pdf_page: 166
    - "no": 4
      title: Prolongement d’une application bilinéaire hypocontinue
      page: 32
      pdf_page: 167
    - "no": 5
      title: Hypocontinuité de l’application $(u, v) \mapsto v \circ u$
      page: 33
      pdf_page: 168
statements: 16
exercises: 15
content_sha256: 3e6f9eaa3d21c28690fd64490285cbb09a94c4fb07a288022a743515dba1e898
---

## § 5. APPLICATIONS BILINÉAIRES HYPOCONTINUES

### 1. Applications bilinéaires séparément continues

Soient E, F, G trois espaces localement convexes. Pour toute application bilinéaire $ u $ de $ E \times F $ dans G, et pour tout $ x \in E $ (resp. $ y \in F $), on désignera par $ u(x, .) $ (resp. $ u(., y) $) l’application $ y \mapsto u(x, y) $ (resp. $ x \mapsto u(x, y) $) de F dans G (resp. de E dans G).

#### Définition 1 {#evt-iii-s5-def-1 .statement}

On dit qu’une application bilinéaire $ u $ de $ E \times F $ dans G est séparément continue si, pour tout $ x \in E $, l’application linéaire $ u(x, .) $ de F dans G est continue et, pour tout $ y \in F $, l’application linéaire $ u(., y) $ de E dans G est continue.

La proposition suivante résulte aussitôt de la définition.

#### Proposition 1 {#evt-iii-s5-prop-1 .statement}

Pour qu’une application bilinéaire $ u $ de $ E \times F $ dans G soit séparément continue, il faut et il suffit que, pour tout $ y \in F $, l’application linéaire $ u(., y) $ de E dans G soit continue, et que l’application linéaire $ y \mapsto u(., y) $ de F dans $ \mathcal{L}_s(E ; G) $ soit continue.

On peut encore dire que si, à toute application linéaire $ v \in \mathcal{L}(F ; \mathcal{L}_s(E ; G)) $ on fait correspondre l’application bilinéaire $ (x, y) \mapsto v(y)(x) $, on définit une bijection linéaire de $ \mathcal{L}(F ; \mathcal{L}_s(E ; G)) $ sur l’espace vectoriel des applications bilinéaires séparément continues de $ E \times F $ dans $ G $.

Une application bilinéaire séparément continue de $ E \times F $ dans $ G $ n’est pas nécessairement continue dans $ E \times F $ (III, p. 48, exerc. 2 ; cf. toutefois III, p. 30, et IV, p. 26, th. 2).

La notion de forme bilinéaire séparément continue sur un produit $ E_1 \times E_2 $ de deux espaces localement convexes se rattache étroitement à celle d’application linéaire continue lorsque $ E_1 $ et $ E_2 $ sont munies de topologies faibles (II, p. 45). Supposons en effet que $ (E_1, F_1) $ et $ (E_2, F_2) $ soient deux couples d’espaces vectoriels réels (resp. complexes) en dualité séparante (*loc. cit.*); munissons $ E_i $ (resp. $ F_i $) de la topologie faible $ \sigma(E_i, F_i) $ (resp. $ \sigma(F_i, E_i) $) pour $ i = 1, 2 $; notons par ailleurs $ B(E_1, E_2) $ l’espace vectoriel des formes bilinéaires séparément continues sur $ E_1 \times E_2 $. Appliquant la prop. 1 au cas où $ G = K $, on voit que, pour toute forme bilinéaire $ \Phi \in B(E_1, E_2) $ et tout $ x_2 \in E_2 $, l’application $ x_1 \mapsto \Phi(x_1, x_2) $ est une forme linéaire *continue* sur $ E_1 $, donc (II, p. 46, prop. 3) il existe un élément et un seul $ ^d\Phi(x_2) \in F_1 $ tel que

$$
\Phi(x_1, x_2) = \langle x_1, {}^d\Phi(x_2) \rangle
$$

quels que soient $ x_1 \in E_1 $ et $ x_2 \in E_2 $; en outre l’application $ {}^d\Phi : E_2 \to F_1 $ est linéaire et *continue* pour les topologies (faibles) de $ E_2 $ et de $ F_1 $.

Inversement, pour toute application linéaire continue $ u : E_2 \to F_1 $, l’application $ (x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle $ est une forme bilinéaire séparément continue sur $ E_1 \times E_2 $, et on a $ u = {}^d\Phi $. On a ainsi défini un isomorphisme $ d : \Phi \mapsto {}^d\Phi $ de $ B(E_1, E_2) $ sur $ \mathcal{L}(E_2 ; F_1) $, dit *canonique*. La formule

$$
\Phi(x_1, x_2) = \langle {}^s\Phi(x_1), x_2 \rangle
$$

définit de même un isomorphisme *canonique* $ s : \Phi \mapsto {}^s\Phi $ de $ B(E_1, E_2) $ sur $ \mathcal{L}(E_1, F_2) $; on a évidemment le diagramme commutatif

(3)

$$
\begin{array}{ccc}
B(E_1, E_2) & & \\
\downarrow s & & \downarrow d^{-1} \\
\mathcal{L}(E_1 ; F_2) & \longleftrightarrow & \mathcal{L}(E_2 ; F_1)
\end{array}
$$

où $ t $ est l’isomorphisme de transposition (II, p. 49, prop. 5 et corollaire). Vu la définition des topologies faibles sur $ F_1 $ et $ F_2 $, il est immédiat en outre que lorsqu’on munit $ B(E_1, E_2) $, $ \mathcal{L}(E_1 ; F_2) $ et $ \mathcal{L}(E_2 ; F_1) $ de la *topologie de la convergence simple*, les *isomorphismes du diagramme* (3) *sont des isomorphismes d’espaces vectoriels topologiques*.

### 2. Applications bilinéaires séparément continues sur un produit d’espaces de Fréchet

#### Proposition 2 {#evt-iii-s5-prop-2 .statement}

Soient E, F et G trois espaces localement convexes. On suppose E et F métrisables, et E tonnelé. Soit H un ensemble d’applications bilinéaires séparément continues de E × F dans G. On suppose que pour tout x ∈ E, l’ensemble des applications u(x, .) de F dans G, où u parcourt H, est équicontinu. Alors H est équicontinu.

Soit (U_n) (resp. (V_n)) une suite fondamentale de voisinages de 0 dans E (resp. F). Si H n’est pas équicontinu, il existe un voisinage convexe équilibré fermé W de 0 dans G tel que, pour tout n, H(U_n × V_n) ne soit pas contenu dans W. Il existe donc une suite de couples (x_n, y_n) ∈ U_n × V_n, et une suite (u_n) d’éléments de H, telles que u_n(x_n, y_n) ∉ W. Soit p la jauge de W. Pour tout y ∈ F, et tout u ∈ H, l’application u(., y) de E dans G est continue, donc p ◦ u(., y) est une semi-norme continue sur E. D’autre part, pour tout x ∈ E, l’ensemble des applications u(x, .) pour u ∈ H est équicontinu ; comme la suite (y_n) tend vers 0, elle est bornée, et l’ensemble des u(x, y_n), pour n ≥ 0 et u ∈ H, est borné (III, p. 22, prop. 9). Il résulte de ceci que la fonction $ p'(x) = \sup_{\substack{u \in H \\ n \geqslant 0}} p(u(x, y_n)) $ est une semi-norme (finie) sur E, semi-continue inférieurement. Comme E est tonnelé, p’ est continue (III, p. 24, corollaire). Comme (x_n) tend vers 0 dans E, p’(x_n) tend vers 0, de sorte qu’on a p’(x_n) ≤ 1 si n est assez grand ; mais dès lors, on a $ p(u_n(x_n, y_n)) \leq p'(x_n) \leq 1 $, donc $ u_n(x_n, y_n) \in W $ ce qui contredit l’hypothèse sur $ u_n, x_n, y_n $.

#### Corollaire 1 {#evt-iii-s5-prop-2-cor-1 .statement}

Soient E et F deux espaces de Fréchet, et G un espace localement convexe. Toute application bilinéaire séparément continue de E × F dans G est continue.

En effet, tout espace de Fréchet est tonnelé (III, p. 25, corollaire).

Soient E et F deux espaces localement convexes. On note $ \mathscr{B}(E, F) $ l’espace des formes bilinéaires continues sur E × F, muni de la topologie de la convergence uniforme sur les ensembles de la forme A × B où A (resp. B) est borné dans E (resp. F). La formule

$$
u(x, y) = \langle y, \varphi(u)(x) \rangle
$$

(pour $ x \in E, y \in F $ et $ u \in \mathscr{B}(E, F) $) définit une application linéaire continue et injective $ \varphi $ de $ \mathscr{B}(E, F) $ dans $ \mathscr{L}_b(E; F'_b) $.

#### Corollaire 2 {#evt-iii-s5-prop-2-cor-2 .statement}

Supposons que E et F soient métrisables et que E soit tonnelé. Alors $ \varphi $ est un isomorphisme d’espaces vectoriels topologiques de $ \mathscr{B}(E, F) $ sur $ \mathscr{L}_b(E; F'_b) $.

Soit $ f \in \mathscr{L}_b(E; F'_b) $. Posons $ u(x, y) = \langle y, f(x) \rangle $ pour $ x \in E $ et $ y \in F $. La forme bilinéaire u sur E × F est séparément continue ; d’après la prop. 2, elle appartient donc à $ \mathscr{B}(E, F) $, et l’on a $ f = \varphi(u) $. Donc $ \varphi $ est une bijection linéaire de $ \mathscr{B}(E, F) $ sur $ \mathscr{L}_b(E; F'_b) $. Il est immédiat que $ \varphi $ est bicontinue, d’où le cor. 2.

### 3. Applications bilinéaires hypocontinues

Nous allons dans ce qui suit définir une notion intermédiaire entre celle d’application bilinéaire continue et celle d’application bilinéaire séparément continue.

#### Proposition 3 {#evt-iii-s5-prop-3 .statement}

Soient E, F, G trois espaces localement convexes, $ \mathcal{S} $ un ensemble de parties bornées de E. Soit u une application bilinéaire séparément continue de $ E \times F $ dans G. Les propriétés suivantes sont équivalentes :

a) Pour tout voisinage W de 0 dans G et tout ensemble $ M \in \mathcal{S} $, il existe un voisinage V de 0 dans F tel que $ u(M \times V) \subset W $.

b) Pour tout ensemble $ M \in \mathcal{S} $, l’image de M par l’application $ x \mapsto u(x, .) $ est une partie équicontinue de $ \mathcal{L}(F; G) $.

c) L’application $ y \mapsto u(., y) $ de F dans $ \mathcal{L}_{\mathcal{S}}(E; G) $ est continue.

En effet, a) exprime que $ y \mapsto u(., y) $ est continue au point 0, compte tenu de la définition des voisinages de 0 dans $ \mathcal{L}_{\mathcal{S}}(E; G) $ (III, p. 13); de même a) exprime que l’image de M par l’application $ x \mapsto u(x, .) $ est équicontinue au point 0 (III, p. 16).

#### Définition 2 {#evt-iii-s5-def-2 .statement}

Soit u une application bilinéaire de $ E \times F $ dans G. On dit que u est $ \mathcal{S}$-hypocontinue si u est séparément continue et si elle vérifie l’une des conditions équivalentes a), b), c) de la prop. 3.

La condition c) de la prop. 3 montre que la notion d’application bilinéaire $ \mathcal{S}$-hypocontinue ne dépend de $ \mathcal{S} $ que par l’intermédiaire de la $ \mathcal{S} $-topologie sur $ \mathcal{L}(E; G) $.

Pour tout ensemble $ \mathcal{I} $ de parties bornées de F, on définit de la même manière la notion d’application $ \mathcal{I}$-hypocontinue, en échangeant dans la prop. 3 les rôles de E et F. On dit qu’une application bilinéaire séparément continue u est ($ \mathcal{S}, \mathcal{I} $)-hypocontinue si elle est à la fois $ \mathcal{S}$-hypocontinue et $ \mathcal{I}$-hypocontinue.

Toute application bilinéaire continue de $ E \times F $ dans G est ($ \mathcal{S}, \mathcal{I} $)-hypocontinue pour tout couple ($ \mathcal{S}, \mathcal{I} $) d’ensembles de parties bornées : en effet, pour tout voisinage W de 0 dans G, il existe un voisinage U de 0 dans E et un voisinage V de 0 dans F tel que $ u(U \times V) \subset W $; comme tout ensemble $ M \in \mathcal{S} $ est borné, il existe $ \lambda > 0 $ tel que $ \lambda M \subset U $, d’où

$$
u(M \times \lambda V) = u(\lambda M \times V) \subset u(U \times V) \subset W .
$$

La réciproque est inexacte en général (III, p. 48, exerc. 3).

#### Proposition 4 {#evt-iii-s5-prop-4 .statement}

Soit u une application bilinéaire $ \mathcal{S}$-hypocontinue de $ E \times F $ dans G. Pour tout ensemble $ M \in \mathcal{S} $, la restriction de u à $ M \times F $ est continue, et $ u(M \times Q) $ est bornée dans G pour toute partie bornée Q de F.

La première assertion résulte du cor. 3 de TG, X, p. 13. Soit W un voisinage de 0 dans G ; il existe par hypothèse un voisinage V de 0 dans F tel que $ u(M \times V) \subset W $. Comme il existe $ \lambda \neq 0 $ tel que $ \lambda Q \subset V $, on a $ \lambda u(M \times Q) = u(M \times \lambda Q) \subset W $, ce qui prouve la seconde partie de la proposition.

#### Proposition 5 {#evt-iii-s5-prop-5 .statement}

Soit u une application bilinéaire ($ \mathcal{S}, \mathcal{T} $)-hypocontinue de $ E \times F $ dans $ G $. Pour tout couple d’ensembles $ M \in \mathcal{S}, N \in \mathcal{T} $, $ u $ est uniformément continue dans $ M \times N $.

La proposition résulte aussitôt de la prop. 2 de TG, X, p. 13 et de la prop. 5 de TG, X, p. 15.

#### Proposition 6 {#evt-iii-s5-prop-6 .statement}

Si $ F $ est un espace tonnelé, toute application bilinéaire séparément continue $ u $ de $ E \times F $ dans un espace localement convexe $ G $ est $ \mathcal{S} $-hypocontinue pour tout ensemble $ \mathcal{S} $ de parties bornées de $ E $.

Autrement dit, l’application linéaire $ y \mapsto u(., y) $ de $ F $ dans $ \mathcal{L}_b(E ; G) $ est continue.

Il suffit en effet (III, p. 31, prop. 3) de prouver que l’image par $ x \mapsto u(x, .) $ de toute partie bornée $ M $ de $ E $ est équicontinue dans $ \mathcal{L}(F ; G) $. Or, en vertu de la prop. 1 (III, p. 28), cette image est une partie simplement bornée de $ \mathcal{L}(F ; G) $, et comme $ F $ est tonnelé, toute partie simplement bornée de $ \mathcal{L}(F ; G) $ est équicontinue (III, p. 25, th. 1).

#### Remarque {#evt-iii-s5-n3-rem-1 .statement}

Supposons que la topologie de $ F $ soit la plus fine des topologies localement convexes sur $ F $ rendant continues des applications linéaires $ h_\alpha : F_\alpha \to F $ (II, p. 29). Alors, la condition c) de la prop. 3 (III, p. 31) montre que, si $ E $ et $ G $ sont localement convexes, pour que l’application bilinéaire $ u : E \times F \to G $ soit $ \mathcal{S} $-hypocontinue, il faut et il suffit que chacune des applications bilinéaires

$$
(x, y_\alpha) \mapsto u(x, h_\alpha(y_\alpha))
$$

de $ E \times F_\alpha $ dans $ G $ soit $ \mathcal{S} $-hypocontinue.

Supposons maintenant que $ E $ soit un espace localement convexe, limite inductive stricte d’une suite croissante $ (E_n) $ de sous-espaces vectoriels fermés dans $ E $ (II, p. 36) ; alors tout ensemble $ M \in \mathcal{S} $ est contenu dans l’un des $ E_n $ et borné dans ce sous-espace (III, p. 5, prop. 6). Notons $ \mathcal{S}_n $ l’ensemble des parties appartenant à $ \mathcal{S} $ et contenues dans $ E_n $. La condition a) de la prop. 3 (III, p. 31) montre que pour qu’une application bilinéaire $ u : E \times F \to G $ soit $ \mathcal{S} $-hypocontinue, il faut et il suffit que chacune des restrictions $ u_n : E_n \times F \to G $ de $ u $ soit $ \mathcal{S}_n $-hypocontinue.

### 4. Prolongement d’une application bilinéaire hypocontinue

#### Proposition 7 {#evt-iii-s5-prop-7 .statement}

Soient $ E, F, G $ trois espaces localement convexes, $ G $ étant supposé séparé ; soit $ E_0 $ (resp. $ F_0 $) un sous-espace vectoriel dense de $ E $ (resp. $ F $). Soit $ u $ une application bilinéaire séparément continue de $ E \times F $ dans $ G $.

1) Si $ u(E_0 \times F_0) = \{0\} $, on a $ u = 0 $.

2) Soit $ \mathcal{S}_0 $ un ensemble de parties bornées de $ E_0 $ ; si la restriction de $ u $ à $ E_0 \times F_0 $ est $ \mathcal{S}_0 $-hypocontinue, il en est de même de $ u $.

1) Par hypothèse, pour tout $ x \in E_0 $, l’application linéaire continue $ u(x, .) $ est nulle dans $ F_0 $, donc dans $ F $ : alors, pour tout $ y \in F $, l’application linéaire continue $ u(., y) $ est nulle dans $ E_0 $, donc dans $ E $, ce qui prouve que l’on a $ u = 0 $.

2) Pour tout voisinage fermé $ W $ de $ 0 $ dans $ G $ et pour tout ensemble $ M \in \mathcal{S}_0 $, il existe par hypothèse un voisinage V de 0 dans F_0 tel que u(M × V) ⊂ W. Or \overline{V} est un voisinage de 0 dans F ; pour tout x ∈ M, de la relation u({x} × V) ⊂ W, on déduit u({x} × \overline{V}) ⊂ W, puisque u(x, .) est continue et W fermé ; on a donc la relation u(M × \overline{V}) ⊂ W, ce qui montre que u est $ \mathcal{S}_0 $-hypocontinue.

#### Proposition 8 {#evt-iii-s5-prop-8 .statement}

*Soient E, F, G trois espaces localement convexes, G étant supposé séparé et quasi-complet. Soit E_0 (resp. F_0) un sous-espace vectoriel dense de E (resp. F), $ \mathcal{S}_0 $ (resp. $ \mathcal{T}_0 $) un ensemble de parties bornées de E_0 (resp. F_0) tel que tout point de E (resp. F) soit adhérent à un ensemble de $ \mathcal{S}_0 $ (resp. $ \mathcal{T}_0 $). Alors toute application bilinéaire ($ \mathcal{S}_0, \mathcal{T}_0 $)-hypocontinue u de E_0 × F_0 dans G se prolonge d’une seule manière en une application bilinéaire séparément continue $ \overline{u} $ de E × F dans G, et $ \overline{u} $ est ($ \mathcal{S}_0, \mathcal{T}_0 $)-hypocontinue.*

L’unicité et l’hypocontinuité de $ \overline{u} $ résultent de la prop. 7 ; tout revient à établir l’existence de $ \overline{u} $. Pour tout $ y' \in F_0 $, l’application linéaire continue $ x' \mapsto u(x', y') $ de E_0 dans G se prolonge d’une seule manière en une application linéaire continue $ x \mapsto u_1(x, y') $ de E dans G (III, p. 8, prop. 10). Il est immédiat que, pour tout $ x \in E $, l’application $ y' \mapsto u_1(x, y') $ de F_0 dans G est linéaire ; montrons qu’elle est continue. Par hypothèse, il existe $ M \in \mathcal{S}_0 $ tel que $ x \in \overline{M} $. Pour tout voisinage fermé W de 0 dans G, il existe par hypothèse un voisinage V de 0 dans F_0 tel que $ u(M \times V) \subset W $; comme $ x \mapsto u_1(x, y') $ est continue, on en déduit $ u_1(\overline{M} \times V) \subset W $, et en particulier $ u_1(x, y') \in W $ pour tout $ y' \in V $, ce qui établit notre assertion. En vertu de la prop. 7, l’application bilinéaire $ u_1 $ de E × F_0 dans G est ($ \mathcal{S}_0, \mathcal{T}_0 $)-hypocontinue. On achève la démonstration en échangeant les rôles de E et F dans la première partie de la démonstration, appliquée à $ u_1 $.

### 5. Hypocontinuité de l’application $(u, v) \mapsto v \circ u$

#### Proposition 9 {#evt-iii-s5-prop-9 .statement}

*Soient R, S, T trois espaces localement convexes séparés. On suppose les espaces $ \mathcal{L}(R; S) $, $ \mathcal{L}(S; T) $, $ \mathcal{L}(R; T) $ munis tous trois de la topologie de la convergence simple (resp. compacte, bornée). Alors l’application bilinéaire $(u, v) \mapsto v \circ u$ de $ \mathcal{L}(R; S) \times \mathcal{L}(S; T) $ dans $ \mathcal{L}(R; T) $ est ($ \mathcal{S}, \mathcal{T} $)-hypocontinue, lorsque $ \mathcal{T} $ est l’ensemble des parties équicontinues de $ \mathcal{L}(S; T) $, et $ \mathcal{S} $ l’ensemble des parties finies (resp. des parties compactes, des parties bornées) de $ \mathcal{L}(R; S) $.

Prouvons d’abord que $(u, v) \mapsto v \circ u$ est $ \mathcal{T} $-hypocontinue. Soient H un ensemble équicontinu dans $ \mathcal{L}(S; T) $, W un voisinage de 0 dans T, M une partie finie (resp. compacte, bornée) de R. Il faut voir qu’il existe un voisinage V de 0 dans S tel que, si $ u(M) \subset V $ et $ v \in H $, on ait $ v(u(M)) \subset W $. Mais il suffit pour cela que l’on ait $ v(V) \subset W $ pour tout $ v \in H $, et l’existence d’un tel voisinage V résulte de l’équicontinuité de H.

Pour voir que $(u, v) \mapsto v \circ u$ est $ \mathcal{S} $-hypocontinue, nous allons établir que, pour tout voisinage W de 0 dans T, toute partie finie (resp. compacte, bornée) M de R et toute partie finie (resp. compacte, bornée) L de $ \mathcal{L}(R; S) $, il existe une partie finie (resp. compacte, bornée) N de S telle que les relations $ v(N) \subset W $ et $ u \in L $ entraînent $ v(u(M)) \subset W $. Il suffit évidemment de montrer qu’on peut prendre $ N = \bigcup_{u \in L} u(M) $, c’est-à-dire que cet ensemble N est fini (resp. compact, borné) avec L et M. C’est immédiat si L et M sont finis, ou si M est borné dans R et L borné dans $ \mathcal{L}(R; S) $ (pour la topologie de la convergence bornée, cf. III, p. 22). Reste donc à établir que si M est compact dans R, et L compact dans $ \mathcal{L}(R; S) $ pour la topologie de la convergence compacte, N est compact dans S. Mais, si $ u_M $ est la restriction à M de tout $ u \in L $, l’application $ u \mapsto u_M $ de L dans l’espace $ \mathcal{C}(M; S) $ des applications continues de M dans S, muni de la topologie de la convergence uniforme, est continue ; l’image de L par cette application est donc compacte, et notre assertion résulte alors de la continuité de l’application $ (w, x) \mapsto w(x) $ de $ \mathcal{C}(M; S) \times M $ dans S (TG, X, p. 10, prop. 9).

Dans les deux corollaires qui suivent, on suppose comme dans la prop. 9 que les espaces $ \mathcal{L}(R; S) $, $ \mathcal{L}(S; T) $, $ \mathcal{L}(R; T) $ sont tous trois munis de la topologie de la convergence simple, ou tous trois de la topologie de la convergence compacte, ou tous trois de la topologie de la convergence bornée.

#### Corollaire 1 {#evt-iii-s5-prop-9-cor-1 .statement}

Pour toute partie équicontinue H de $ \mathcal{L}(S; T) $, l’application $ (u, v) \mapsto v \circ u $ de $ \mathcal{L}(R; S) \times H $ dans $ \mathcal{L}(R; T) $ est continue.
Cela résulte aussitôt des prop. 9 (III, p. 33) et 4 (III, p. 31).

#### Corollaire 2 {#evt-iii-s5-prop-9-cor-2 .statement}

On suppose S tonnelé. Si la suite $ (u_n) $ tend vers u dans $ \mathcal{L}(R; S) $ et la suite $ (v_n) $ vers v dans $ \mathcal{L}(S; T) $, la suite $ (v_n \circ u_n) $ tend vers $ v \circ u $ dans $ \mathcal{L}(R; T) $.
En effet, la suite $ (v_n) $ étant simplement bornée dans $ \mathcal{L}(S; T) $, est équicontinue puisque S est tonnelé (III, p. 25, th. 1) ; le corollaire est alors conséquence du cor. 1.

## EXERCICES {#evt-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
