---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 1
section_title: Hyperplans, chambres et facettes
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0056-0064
extraction: ocr
subsections:
    - "no": 1
      title: Notations
      page: 0
      pdf_page: 56
    - "no": 2
      title: Facettes
      page: 0
      pdf_page: 57
    - "no": 3
      title: Chambres
      page: 0
      pdf_page: 59
    - "no": 4
      title: Murs et faces
      page: 0
      pdf_page: 60
    - "no": 5
      title: Dièdres
      page: 0
      pdf_page: 62
    - "no": 6
      title: 'Exemples : cônes simpliciaux et simplexès'
      page: 0
      pdf_page: 63
statements: 18
exercises: 0
content_sha256: 41c8f874715f48eb74778f8a2f507ebc2a4097a079ab5ab5ab53f484259caed9
---

## § 1. Hyperplans, chambres et facettes

Dans ce paragraphe, on note E un espace affine réel de dimension finie d et T l’espace des translations de E (cf. Alg., chap. II, 3e éd., § 9 et Esp. vect. top., chap. II, § 2). Pour deux points a, b de E, on notera [ab] (resp. ]ab[, resp. ]ab]) le segment fermé (resp. ouvert, resp. ouvert en a et fermé en b), d’extrémités a, b. On munit T de son unique topologie d’espace vectoriel topologique séparé, cf. Esp. vect. top., chap. I, § 2, no 3; il est isomorphe à $ \mathbf{R}^d $. On munit E de l’unique topologie telle que, pour tout $ e \in E $, l’application : $ t \mapsto e + t $ de T sur E soit un homéomorphisme.

On note $ \mathfrak{H} $ un ensemble localement fini d’hyperplans de E (Top. gén., chap. I, § 1, no 5).

### 1. Notations

Soit H un hyperplan de E. Rappelons que E — H a deux composantes connexes, que l’on appelle les demi-espaces ouverts limités par H. Leurs adhérences s’appellent les demi-espaces fermés limités par H. Soient $ x, y \in E $. On dit que $ x $ et $ y $ sont strictement du même côté de H s’ils sont contenus dans le même sous-espace ouvert limité par H, ou, ce qui revient au même, si le segment fermé d’extrémités $ x $ et $ y $ ne rencontre pas H. On dit que $ x $ et $ y $ sont de part et d’autre de H si $ x $ appartient à l’un des demi-espaces ouverts limités par H, et $ y $ à l’autre. Si $ x \in E $ et $ t \in T $, on dit que $ x $ et $ t $ sont strictement du même côté de H s’il en est ainsi pour $ x $ et $ h + t $, quel que soit $ h \in H $.

Soit A une partie connexe non vide de E. Pour tout hyperplan H de E ne rencontrant pas A, on note $ D_H(A) $ l’unique demi-espace ouvert limité par H qui contient A. Si $ \mathfrak{M} $ est un ensemble d’hyperplans de E dont aucun ne rencontre A, on pose

$$
D_{\mathfrak{M}}(A) = \bigcap_{H \in \mathfrak{M}} D_H(A).
$$

Si A est réduit à un point $ a $, on écrit $ D_H(a) $ et $ D_{\mathfrak{M}}(a) $ au lieu de $ D_H(\{a\}) $ et $ D_{\mathfrak{M}}(\{a\}) $.

### 2. Facettes

L’ensemble des points de E qui n’appartiennent à aucun hyperplan H de l’ensemble $ \mathfrak{S} $ est ouvert dans E puisque $ \mathfrak{S} $ est localement fini. De manière plus précise, on a le résultat suivant:

#### Proposition 1 {#lie-v-s1-prop-1 .statement}

Soit a un point de E. Il existe un voisinage ouvert convexe de a qui ne rencontre aucun hyperplan H appartenant à $ \mathfrak{S} $ et ne passant pas par a. De plus, il n’existe qu’un nombre fini d’hyperplans appartenant à $ \mathfrak{S} $ et passant par a.

L’ensemble $ \mathfrak{N} $ des hyperplans H tels que $ H \in \mathfrak{S} $ et $ a \notin H $ est localement fini puisqu’il est contenu dans $ \mathfrak{S} $; par suite, l’ensemble U des points de E n’appartenant à aucun des hyperplans de l’ensemble $ \mathfrak{N} $ est ouvert; comme on a $ a \in U $, il existe un voisinage ouvert convexe de a contenu dans U. Le reste de la proposition est évident.

Étant donnés deux points x et y de E, on notera R $ \{x, y\} $ la relation
« Pour tout hyperplan H $ \in \mathfrak{S} $, ou bien $ x \in H $ et $ y \in H $, ou bien x et y sont strictement du même côté de H. »

Il est clair que R est une relation d’équivalence dans E.

#### Définition 1 {#lie-v-s1-def-1 .statement}

On appelle facette de E relativement à $ \mathfrak{S} $ toute classe selon la relation d’équivalence R définie ci-dessus.

#### Proposition 2 {#lie-v-s1-prop-2 .statement}

L’ensemble des facettes est localement fini.

C’est évident, puisque $ \mathfrak{S} $ est localement fini.

Soient F une facette et a un point de F. Pour qu’un hyperplan H $ \in \mathfrak{S} $ contienne F, il faut et il suffit que l’on ait $ a \in H $; l’ensemble $ \mathfrak{S} $ de ces hyperplans est donc fini; il a pour intersection un sous-espace affine L de E, que l’on appellera le support affine de F; la dimension de L s’appellera la dimension de F.

Si $ \mathfrak{N} $ est l’ensemble des hyperplans $ H \in \mathfrak{S} $ ne contenant pas F, on a

(2)
$$
F = L \cap \bigcap_{H \in \mathfrak{N}} D_H(a).
$$

Nous allons montrer que l’adhérence de F est donnée par la formule

(3)
$$
\overline{F} = L \cap \bigcap_{H \in \mathfrak{N}} \overline{D_H(a)}.
$$

Il est clair que le membre de droite contient le membre de gauche. Inversement, soit $ x \in L \cap \bigcap_{H \in \mathfrak{N}} \overline{D_H(a)} $. Le segment ouvert d’extrémités a et x est contenu dans L et dans chacun des $ D_H(a) $ pour $ H \in \mathfrak{N} $, donc dans F. Il en résulte que x est adhérent à F, d’où la formule.

#### Proposition 3 {#lie-v-s1-prop-3 .statement}

Soient F une facette et L son support affine.
(i) L’ensemble F est une partie ouverte et convexe du sous-espace affine L de E.

(ii) L’adhérence de F est réunion de F et de facettes de dimension strictement inférieure à celle de F.

(iii) Dans l’espace topologique L, l’ensemble F est l’intérieur de son adhérence.

Comme tout demi-espace ouvert et tout hyperplan sont des parties convexes de E, la formule (2) montre que F est intersection d’une famille de parties convexes, donc est convexe. Par ailleurs, soit a dans F, et soit U un voisinage ouvert convexe de a dans E ne rencontrant aucun des hyperplans appartenant à l’ensemble $ \mathfrak{N} $ des $ H \in \mathfrak{S} $ tels que $ a \in H $. Pour tout $ H \in \mathfrak{N} $, on a alors $ U \subset D_H(a) $, d’où $ L \cap U \subset F $, donc F est ouvert dans l’espace topologique L.

Soient b un point de $ \overline{F} - F $, appartenant à la facette F’, et $ \mathfrak{N}' $ l’ensemble des hyperplans $ H \in \mathfrak{N} $ passant par b ; on pose $ \mathfrak{N}'' = \mathfrak{N} - \mathfrak{N}' $. Pour tout H dans $ \mathfrak{N}'' $, on a $ b \notin H $ et $ b \in \overline{D_H(a)} $, d’où $ b \in D_H(a) $ et donc $ D_H(b) = D_H(a) $; par définition d’une facette, on a donc :

$$
F' = L \cap \bigcap_{H \in \mathfrak{N}'} H \cap \bigcap_{H \in \mathfrak{N}''} D_H(a)
$$

alors que (3) entraîne :

$$
\overline{F} = L \cap \bigcap_{H \in \mathfrak{N}'} \overline{D_H(a)} \cap \bigcap_{H \in \mathfrak{N}''} \overline{D_H(a)}
$$

d’où $ F' \subset \overline{F} $. On ne peut avoir $ \mathfrak{N}' = \varnothing $, car cela entraînerait $ F = F' $ d’après (2) et (4), contrairement à l’hypothèse $ b \notin F $ et $ b \in F' $. Le support de F’ est l’ensemble $ L' = L \cap \bigcap_{H \in \mathfrak{N}'} H $; on a $ a \in L $, mais $ a \notin H $ pour H dans $ \mathfrak{N}' $, d’où $ L' \neq L $ et finalement $ \dim L' < \dim L $, c’est-à-dire $ \dim F' < \dim F $. Ceci prouve (ii).

Soient H dans $ \mathfrak{N}' $ et D le demi-espace ouvert limité par H et distinct de $ D_H(a) $; on a $ b \in H \cap L $, et il est immédiat que $ D \cap L $ est un demi-espace de L limité par l’hyperplan $ H \cap L $ de L ; par suite, tout voisinage de b dans L rencontre $ D \cap L $, et comme $ D \cap L $ est disjoint de $ \overline{F} $ d’après (3), on voit que le point b de $ \overline{F} - F $ ne peut être intérieur à $ \overline{F} $ dans l’espace topologique L. Comme F est ouvert dans L, on a (iii).

C.Q.F.D.

#### Corollaire {#lie-v-s1-n2-cor-1 .statement}

Soient F et F’ deux facettes. Si l’on a $ \overline{F} = \overline{F}' $, les facettes F et F’ sont égales.

Cela résulte de (iii).

#### Proposition 4 {#lie-v-s1-prop-4 .statement}

Soient F une facette, et L un sous-espace affine de E, intersection d’hyperplans appartenant à $ \mathfrak{S} $; on note $ \mathfrak{N} $ l’ensemble des hyperplans $ H \in \mathfrak{S} $ qui ne contiennent pas L. Les conditions suivantes sont équivalentes :

(i) Il existe une facette F’ de support L rencontrant $ \overline{F} $.
(ii) Il existe une facette F’ de support L contenue dans $ \overline{F} $.
(iii) Il existe un point x dans $ L \cap \overline{F} $ qui n’appartient à aucun des hyperplans de $ \mathfrak{N} $.
Si ces conditions sont remplies, $ L \cap D_{\mathfrak{N}}(F) $ est l’unique facette de support L contenue dans $ \overline{F} $.

(i) $ \Longrightarrow $ (ii) : Comme $ \overline{F} $ est réunion de facettes (prop. 3, (ii)), toute facette qui rencontre $ \overline{F} $ rencontre une facette contenue dans $ \overline{F} $, et lui est donc égale.

(ii) $ \Longrightarrow $ (iii) : Tout point $ x $ de $ F' $ vérifie (iii) car tout hyperplan de $ \mathfrak{S} $ contenant $ x $ contient $ F' $, donc $ L $.

(iii) $ \Longrightarrow $ (i) : Soit $ x $ un point vérifiant (iii) et soit $ F' $ la facette contenant $ x $; il est clair que $ F' $ rencontre $ \overline{F} $. Soit $ H \in \mathfrak{S} $; on a $ x \notin H $ si $ H \in \mathfrak{N} $ et évidemment $ x \in H $ si $ H \notin \mathfrak{N} $; par suite, le support de $ F' $ est l’intersection des hyperplans de $ \mathfrak{S} - \mathfrak{N} $, et il est égal à $ L $.

Enfin, soit $ F' $ une facette de support $ L $, contenue dans $ \overline{F} $, et soit $ x $ un point de $ F' $; comme aucun hyperplan de $ \mathfrak{N} \subset \mathfrak{S} $ ne passe par $ x $, la prop. 1 montre qu’il existe un voisinage ouvert convexe $ U $ de $ x $ ne rencontrant aucun hyperplan de $ \mathfrak{N} $. Comme $ x $ est adhérent à $ F $, on a $ U \cap F \neq \emptyset $; or $ \mathfrak{N} $ est l’ensemble des hyperplans $ H \in \mathfrak{S} $ qui ne contiennent pas $ F' $, et pour tout $ H $ dans $ \mathfrak{N} $, on a $ D_H(x) = D_H(U) = D_H(U \cap F) = D_H(F) $ et la formule (2) entraîne

$$
F' = L \cap D_{\mathfrak{N}}(F).
$$

C.Q.F.D.

### 3. Chambres

#### Définition 2 {#lie-v-s1-def-2 .statement}

On appelle chambre de $ E $ relativement à $ \mathfrak{S} $ (ou simplement chambre s’il n’y a pas d’ambiguïté sur $ \mathfrak{S} $) toute facette de $ E $ relativement à $ \mathfrak{S} $ qui n’est contenue dans aucun hyperplan appartenant à $ \mathfrak{S} $.

Soit $ U $ l’ensemble ouvert dans $ E $ formé des points qui n’appartiennent à aucun hyperplan de $ \mathfrak{S} $; comme un hyperplan appartenant à $ \mathfrak{S} $ ne peut rencontrer une facette sans la contenir, les chambres sont donc les facettes contenues dans $ U $; toute chambre est une partie ouverte et convexe (donc connexe) de $ E $ d’après la prop. 3, (i); comme les chambres forment une partition de $ U $, ce ne sont autres que les composantes connexes de $ U $. Toute partie convexe $ A $ de $ U $ est connexe, donc contenue dans une chambre qui est bien déterminée si $ A $ est non vide. Il est clair que les chambres sont les facettes de support $ E $, et la prop. 3, (iii) montre que toute chambre est l’intérieur de son adhérence. Enfin, soient $ C $ une chambre et $ A $ une partie non vide de $ C $; des formules (2) et (3), on déduit :

$$
C = \bigcap_{H \in \mathfrak{S}} D_H(A) = D_{\mathfrak{S}}(A), \quad \overline{C} = \bigcap_{H \in \mathfrak{S}} \overline{D_H(A)}
$$

puisque l’on a $ D_H(A) = D_H(a) $ pour tout $ a \in A $.

#### Proposition 5 {#lie-v-s1-prop-5 .statement}

Soit $ C $ une partie non vide de $ E $. On suppose qu’il existe une partie $ \mathfrak{S}' $ de $ \mathfrak{S} $ ayant les deux propriétés suivantes :
a) On peut associer à tout $ H $ dans $ \mathfrak{S}' $ un demi-espace ouvert $ D_H $ limité par $ H $ de sorte que $ C = \bigcap_{H \in \mathfrak{S}'} D_H $.
b) L’ensemble $ C $ ne rencontre aucun hyperplan qui appartient à $ \mathfrak{S} - \mathfrak{S}' $.

Dans ces conditions, C est une chambre définie par $ \mathfrak{H} $ dans E, et l’on a $ D_H = D_H(C) $ pour tout $ H \in \mathfrak{H} $.

Les propriétés a) et b) montrent que C est une partie convexe de U; il existe donc une chambre $ C' $ avec $ C \subset C' $. Comme on a $ C \subset D_H $, on a $ D_H = D_H(C) $ pour tout H dans $ \mathfrak{H}' $, d’où $ C = D_{\mathfrak{H}'}(C) \supset D_{\mathfrak{H}}(C) $ puisque $ \mathfrak{H}' \subset \mathfrak{H} $; on a $ D_{\mathfrak{H}}(C) = C' $ d’après (6), d’où $ C \supset C' $. Finalement, on a $ C = C' $.

#### Proposition 6 {#lie-v-s1-prop-6 .statement}

Tout point de E est adhérent à une chambre au moins.

Si E est réduit à un point, c’est évident. Sinon, soit $ a \in E $, et soient $ H_1, \ldots, H_m $ les hyperplans de $ \mathfrak{H} $ contenant a. Puisque $ \mathfrak{H} $ est localement fini, il existe un voisinage V de a ne rencontrant aucun hyperplan de $ \mathfrak{H} $ distinct de $ H_1, \ldots, H_m $. Soit D une droite passant par a et qui n’est contenue dans aucun des $ H_i $; si $ x \in D, x \neq a $, et x est assez voisin de a, le segment ouvert $ ]ax[ $ est contenu dans V et ne rencontre aucun des $ H_i $. On a alors $ ]ax[ \subset U $; comme $ ]ax[ $ est connexe, il est contenu dans une chambre C, d’où $ a \in \overline{C} $.

#### Proposition 7 {#lie-v-s1-prop-7 .statement}

Soient L un sous-espace affine de E et $ \Omega $ une partie ouverte non vide de L.

(i) Il existe un point a de $ \Omega $ n’appartenant à aucun des hyperplans de $ \mathfrak{H} $ qui ne contiennent pas L.

(ii) Si L est un hyperplan et si $ L \notin \mathfrak{H} $, il existe une chambre rencontrant $ \Omega $.

(iii) Si L est un hyperplan et si $ L \in \mathfrak{H} $, il existe un point a de $ \Omega $ n’appartenant à aucun hyperplan $ H \neq L $ de $ \mathfrak{H} $.

On notera $ \mathfrak{N} $ l’ensemble des hyperplans H avec $ H \in \mathfrak{H} $ et $ L \not\subset H $, et $ \mathfrak{L} $ l’ensemble des hyperplans de l’espace affine L de la forme $ L \cap H $ avec $ H \in \mathfrak{N} $. Il est clair que $ \mathfrak{L} $ est un ensemble localement fini d’hyperplans dans L, et la prop. 6 montre que $ \Omega $ rencontre une chambre $ \Gamma $ définie par $ \mathfrak{L} $ dans L. Si a est un point de $ \Gamma \cap \Omega $, on aura $ a \notin H $ pour tout $ H \in \mathfrak{N} $, d’où (i).

Supposons que L soit un hyperplan; tout hyperplan contenant L lui est égal, et par suite, on peut distinguer deux cas:

a) $ L \notin \mathfrak{H} $: alors $ \mathfrak{N} = \mathfrak{H} $, et l’on a $ a \notin H $ pour tout $ H \in \mathfrak{H} $; donc a appartient à une chambre définie par $ \mathfrak{H} $ dans E, d’où (ii).

b) $ L \in \mathfrak{H} $: on a alors $ \mathfrak{N} = \mathfrak{H} - \{L\} $, d’où (iii).

### 4. Murs et faces

#### Définition 3 {#lie-v-s1-def-3 .statement}

Soit C une chambre de E. On appelle face de C toute facette contenue dans l’adhérence de C et dont le support est un hyperplan. On appelle mur de C tout hyperplan qui est le support d’une face de C.

Tout mur de C appartient à $ \mathfrak{H} $. La prop. 4 montre qu’un hyperplan $ L \in \mathfrak{H} $ est un mur de C si et seulement si l’on a $ C \neq D_{\mathfrak{H} - \{L\}}(C) $. De plus, tout mur de C est le support d’une seule face de C.

#### Proposition 8 {#lie-v-s1-prop-8 .statement}

Tout hyperplan H appartenant à $ \mathfrak{H} $ est le mur d’au moins une chambre.

D’après la prop. 7, (iii), il existe un point $ a $ de $ H $ n’appartenant à aucun hyperplan $ H' \neq H $ de $ \mathfrak{S} $; d’après la prop. 6, il existe une chambre $ C $ telle que $ a \in \overline{C} $; la prop. 4 montre alors que $ H $ est un mur de $ C $.

#### Proposition 9 {#lie-v-s1-prop-9 .statement}

*Soient $ C $ une chambre et $ \mathfrak{M} $ l’ensemble des murs de $ C $. On a $ C = D_{\mathfrak{M}}(C) $ et toute partie $ \mathfrak{L} $ de $ \mathfrak{S} $ telle que $ C = D_{\mathfrak{L}}(C) $ contient $ \mathfrak{M} $. Pour qu’une partie $ F $ de $ \overline{C} $ soit une facette, il faut et il suffit que ce soit une facette de $ E $ relativement à la famille $ \mathfrak{M} $.*

$ a) $ Soit $ \mathfrak{L} $ une partie de $ \mathfrak{S} $ telle que $ C = D_{\mathfrak{L}}(C) $. Considérons un hyperplan $ L $ appartenant à $ \mathfrak{S} $ mais non à $ \mathfrak{L} $; soit $ \mathfrak{N} $ l’ensemble des hyperplans $ H \neq L $ appartenant à $ \mathfrak{S} $. On a $ \mathfrak{L} \subset \mathfrak{N} $, d’où $ C = D_{\mathfrak{N}}(C) $, et $ L $ ne rencontre pas $ D_{\mathfrak{N}}(C) $. D’après la prop. 4 (implication (i) $ \Longrightarrow $ (iii)), l’hyperplan $ L $ n’est pas un mur de $ C $. Par conséquent, tout mur de $ C $ appartient à $ \mathfrak{L} $.

$ b) $ On suppose toujours $ C = D_{\mathfrak{L}}(C) $. Soit $ H $ un hyperplan appartenant à $ \mathfrak{L} $, qui ne soit pas un mur de $ C $, et posons $ \mathfrak{L}' = \mathfrak{L} - \{H\} $. D’après la prop. 4 (implication (iii) $ \Longrightarrow $ (i)), l’ensemble convexe $ D_{\mathfrak{L}'}(C) $ ne rencontre pas $ H $, d’où $ D_{\mathfrak{L}'}(C) \subset D_H(C) $ et $ C = D_{\mathfrak{L}'}(C) $. Par récurrence sur le cardinal de $ \mathfrak{S} $, on en conclut que, si $ \mathfrak{F} $ est une partie finie de $ \mathfrak{L} $ ne contenant aucun mur de $ C $, on a $ C = D_{\mathfrak{L}-\mathfrak{F}}(C) $.

$ c) $ Soit $ a $ un point de $ C $; on a évidemment $ C \subset D_{\mathfrak{M}}(a) $. Soit $ a' $ un point de $ D_{\mathfrak{M}}(a) $; comme le segment fermé $ [aa'] $ est compact, l’ensemble $ \mathfrak{S} $ des hyperplans $ H \in \mathfrak{S} $ qui rencontrent $ [aa'] $ est fini. Comme $ a $ et $ a' $ sont strictement du même côté de tout mur de $ C $, aucun mur de $ C $ n’appartient à $ \mathfrak{S} $; d’après $ b) $, on a donc $ C = D_{\mathfrak{S}-\mathfrak{S}}(C) $. Comme $ a' \in D_{\mathfrak{S}-\mathfrak{S}}(a) $, on a $ a' \in C $. On a donc prouvé que $ D_{\mathfrak{M}}(a) \subset C $, ce qui démontre la première partie de la proposition.

$ d) $ Pour prouver la dernière assertion de la proposition, il suffit évidemment de montrer qu’une partie $ F $ de $ \overline{C} $ qui est une facette de $ E $ relativement à $ \mathfrak{M} $, est une facette de $ E $ relativement à $ \mathfrak{S} $, ou encore que tout hyperplan $ H \in \mathfrak{S} $ qui rencontre $ F $ contient $ F $. Soit donc $ H $ un hyperplan rencontrant $ F $ et ne le contenant pas. Comme $ F $ est ouvert dans son support affine, il n’est pas tout entier d’un même côté de $ H $. Il en résulte que $ \overline{C} $ n’est pas tout entier d’un même côté de $ H $ et par suite l’hyperplan $ H $ ne peut pas appartenir à $ \mathfrak{S} $, ce qui achève la démonstration.

#### Remarque 1 {#lie-v-s1-n4-rem-1 .statement}

Il résulte de la formule (6) et de la prop. 9 que l’adhérence d’une chambre $ C $ est l’intersection des demi-espaces fermés limités par un mur de $ C $ et qui contiennent $ C $.

#### Remarque 2 {#lie-v-s1-n4-rem-2 .statement}

Soit $ F $ une facette dont le support est un hyperplan $ L $; on va montrer qu’il existe deux chambres dont $ F $ soit une face. Soit $ \mathfrak{N} $ l’ensemble des hyperplans $ H \neq L $ appartenant à $ \mathfrak{S} $; posons $ A = D_{\mathfrak{N}}(F) $ et notons $ D^+ $ et $ D^- $ les demi-espaces ouverts limités par $ L $. L’ensemble $ A $ est ouvert et contient $ F \subset L $, et comme tout point de $ L $ est adhérent à $ D^+ $ et à $ D^- $, les ensembles $ C^+ = A \cap D^+ $ et $ C^- = A \cap D^- $ sont non vides; ce sont des chambres. De plus, l’hyperplan L rencontre $ D_{\mathfrak{H}}(F) = D_{\mathfrak{H}}(C^+) $; la prop. 4 montre que L est un mur de $ C^+ $ et F, qui rencontre $ L \cap D_{\mathfrak{H}}(F) $, est une face de $ C^+ $; de même, F est une face de $ C^- $. Enfin, soit C une chambre dont F soit une face, et supposons par exemple $ D^+ = D_L(C) $; d’après la prop. 4, l’ensemble $ D_{\mathfrak{H}}(C) $ rencontre F, donc est égal à $ D_{\mathfrak{H}}(F) $ et l’on a

$$
C = D_S(C) = D_L(C) \cap D_{\mathfrak{H}}(C) = D^+ \cap D_{\mathfrak{H}}(F) = C^+.
$$

### 5. Dièdres

Rappelons (Alg., chap. II, 3e éd., § 9, no 3) que deux sous-espaces affines P et P' de E sont dits parallèles s’il existe un vecteur t dans T tel que $ P' = t + P $. Il est clair que la relation « P et P' sont parallèles » est une relation d’équivalence dans l’ensemble des sous-espaces affines de E.

#### Lemme 1 {#lie-v-s1-lem-1 .statement}

Deux hyperplans non parallèles ont une intersection non vide.

Soient H et H' deux hyperplans non parallèles, $ a \in H $ et $ a' \in H' $; il existe deux hyperplans M et M' dans l’espace vectoriel T tels que $ H = M + a $ et $ H' = M' + a' $; comme H et H' ne sont pas parallèles, on a $ M \neq M' $, d’où $ T = M + M' $; il existe alors $ u \in M $ et $ u' \in M' $ tels que $ a' - a = u - u' $, et le point $ u + a = u' + a' $ appartient à $ H \cap H' $.

#### Lemme 2 {#lie-v-s1-lem-2 .statement}

Soient H et H' deux hyperplans distincts dans E, et f, f' deux fonctions affines sur E telles que H (resp. H') se compose des points a de E tels que $ f(a) = 0 $ (resp. $ f'(a) = 0 $). Enfin soit L un hyperplan dans E. On suppose l’une des hypothèses suivantes remplies :

a) Les hyperplans H, H' et L sont parallèles.

b) Les hyperplans H et H' ne sont pas parallèles, et $ H \cap H' \subset L $.

Il existe alors des nombres réels $ \lambda, \lambda' $ non tous deux nuls tels que L se compose des $ a \in E $ qui annulent la fonction affine $ g = \lambda . f + \lambda' . f' $.

Le lemme étant trivial lorsque $ L = H $, nous pouvons supposer qu’il existe un point a de L avec $ a \notin H $. Posons $ \lambda = f'(a), \lambda' = -f(a) $ et

$$
g = \lambda . f + \lambda' . f';
$$

on a $ \lambda' \neq 0 $ puisque $ a \notin H $; de plus, comme $ H \neq H' $, il existe $ b \in H $ tel que $ b \notin H' $, d’où $ f(b) = 0, f'(b) \neq 0 $, et donc $ g(b) = -f(a) . f'(b) $ est non nul. L’ensemble $ L_1 $ des points où s’annule la fonction affine $ g \neq 0 $ est alors un hyperplan dans E; on a $ g(a) = 0 $, d’où $ a \in L_1 $.

a) Supposons H et H' parallèles : tout point de $ L_1 \cap H $ annule g et f, donc aussi $ f' $ puisque $ \lambda' \neq 0 $, et appartient donc à H'; mais comme H et H' sont parallèles et distincts, ils sont disjoints, d’où $ L_1 \cap H = \varnothing $, et le lemme 1 montre que $ L_1 $ est parallèle à H. Comme on a $ a \in L $ et $ a \in L_1 $, on a donc $ L = L_1 $.

b) Supposons H et H' non parallèles : d’après le lemme 1, il existe un point c dans $ H \cap H' $; nous munirons E de la structure d’espace vectoriel obtenue en prenant c comme origine. Alors $ H \cap H' $ est un sous-espace vectoriel de codimension 2 dans E, et comme on a $ a \notin H $, le sous-espace vectoriel M de E engendré par $ H \cap H' $ et a est un hyperplan; comme on a $ H \cap H' \subset L \cap L_1 $ et $ a \in L \cap L_1 $, on a $ M \subset L \cap L_1 $, d’où $ M = L = L_1 $.

C.Q.F.D.

#### Proposition 10 {#lie-v-s1-prop-10 .statement}

Soit C une chambre, soient H et H' deux murs de C, et soit L un hyperplan rencontrant $ D_H(C) \cap D_{H'}(C) $. On suppose que H est distinct de H' et que l’une des conditions suivantes est satisfaite :

a) Les hyperplans H, H' et L sont parallèles.

b) Les hyperplans H et H' ne sont pas parallèles, et $ H \cap H' \subset L $.
Alors L rencontre C.

Soit b (resp. $ b' $) un point de la face de C de support H (resp. H'); il est immédiat que tout point du segment $[bb']$ distinct de b et $ b' $ appartient à C.

Introduisons une fonction affine $ f $ nulle en tout point de H et telle que $ f(x) > 0 $ pour x dans $ D_H(C) $; introduisons de même une fonction affine $ f' $ ayant la propriété analogue par rapport à H'. Appliquant le lemme 2, on peut trouver des nombres $ \lambda $ et $ \lambda' $ et une fonction affine g ayant les propriétés indiquées. On a $ (\lambda, \lambda') \neq (0, 0) $ et pour tout point x de $ L \cap D_H(C) \cap D_{H'}(C) $, on a $ f(x) > 0, f'(x) > 0 $ et $ \lambda \cdot f(x) + \lambda' \cdot f'(x) = 0 $, d’où $ \lambda \lambda' < 0 $. Par ailleurs, on a $ g(b) = \lambda' \cdot f'(b) $ et $ g(b') = \lambda \cdot f(b') $, et comme $ f(b') > 0, f'(b) > 0 $, on a $ g(b) \cdot g(b') < 0 $. Les points b et $ b' $ sont strictement de part et d’autre de l’hyperplan L, et il existe un point c de L appartenant à $[bb']$ et distinct de b et $ b' $, donc appartenant à C.

### 6. Exemples : cônes simpliciaux et simplexès

a) Soient a un point de E, et $ (e_1, \ldots, e_d) $ une base de T; tout point de E s’écrit alors d’une manière et d’une seule sous la forme

$$
x = a + \xi_1 \cdot e_1 + \cdots + \xi_d \cdot e_d
$$

avec $ \xi_1, \ldots, \xi_d $ réels. On notera $ e'_i $ la fonction affine sur E qui, pour tout $ x \in E $ écrit sous la forme (7), prend la valeur $ \xi_i $. On notera $ H_i $ l’hyperplan formé des x tels que $ e'_i(x) = 0 $, et $ \mathfrak{S} $ l’ensemble des hyperplans $ H_1, \ldots, H_d $. Pour toute partie J de l’ensemble $ I = \{1, 2, \ldots, d\} $, on posera $ H_J = \bigcap_{i \in J} H_i $; pour toute suite $ (\varepsilon_1, \ldots, \varepsilon_d) $ de nombres tous égaux à 0, 1 ou — 1, on notera $ F(\varepsilon_1, \ldots, \varepsilon_d) $ l’ensemble des $ x \in E $ tels que $ e'_i(x) $ soit de signe (Top. gén., chap. IV, § 3, no 2) $ \varepsilon_i $ pour tout i dans I. Il est immédiat que les facettes définies par $ \mathfrak{S} $ dans E sont les ensembles $ F(\varepsilon_1, \ldots, \varepsilon_d) $ et que ces ensembles sont deux à deux distincts; le support de $ F(\varepsilon_1, \ldots, \varepsilon_d) $ est égal à $ H_J $ si J est l’ensemble des $ i \in I $ tels que $ \varepsilon_i = 0 $; en particulier, les chambres sont les ensembles de la forme $ F(\varepsilon_1, \ldots, \varepsilon_d) $ où chacun des nombres $ \varepsilon_i $ est égal à 1 ou — 1.

L’ensemble $ C = F(1, \ldots, 1) $ formé des $ x $ avec $ e_i'(x) > 0 $ pour tout $ i \in I $ est une chambre, qu’on appellera le cône simplicial ouvert de sommet $ a $ défini par la base $ (e_1, \ldots, e_d) $. Son adhérence se compose des points $ x $ tels que $ e_i'(x) \geqslant 0 $ pour tout $ i \in I $ lorsque $ d \geqslant 1 $; sinon, cette adhérence est vide. Pour toute partie $ J $ de $ I $, soit $ C_J $ l’ensemble des points $ x $ de $ E $ tels que $ e_i'(x) = 0 $ pour $ i \in J $ et $ e_i'(x) > 0 $ pour $ i \in I - J $. Alors $ C_J $ est une facette de support $ H_J $, et c’est un cône simplicial ouvert de sommet $ a $ dans l’espace affine $ H_J $; de plus, on a $ \overline{C} = \bigcup_{J \subset I} C_J $. En particulier, les murs de $ C $ sont les hyperplans $ H_i $ pour $ i \in I $, et la face de $ C $ contenue dans $ H_i $ est égale à $ C_{\{i\}} $.

On ne change aucun des ensembles $ H_i, H_J, C, C_J $ et $ F(\varepsilon_1, \ldots, \varepsilon_d) $ si l’on remplace la base $ (e_1, \ldots, e_d) $ par une base $ (\lambda_1 e_1, \ldots, \lambda_d e_d) $ avec $ \lambda_i > 0 $ pour tout $ i $.

$ b) $ Supposons maintenant donné un système affinement libre de points de $ E $, soit $ (a_0, a_1, \ldots, a_d) $. On sait que tout point de $ E $ s’écrit d’une manière et d’une seule sous la forme $ x = \xi_0 \cdot a_0 + \cdots + \xi_d \cdot a_d $ avec $ \xi_0, \ldots, \xi_d $ réels et $ \xi_0 + \cdots + \xi_d = 1 $ (*Alg.*, chap. II, 3e éd., § 9, no 3). On définit des fonctions affines $ f_0, \ldots, f_d $, la fonction $ f_i $ faisant correspondre à tout point $ x $ mis sous la forme précédente le nombre $ \xi_i $. Nous noterons $ H_i $ l’hyperplan de $ E $ défini par $ f_i(x) = 0 $ et $ \mathfrak{S} $ l’ensemble des hyperplans $ H_0, H_1, \ldots, H_d $; enfin, nous poserons $ I = \{0, 1, \ldots, d\} $. On appelle simplexe ouvert de sommets $ a_0, \ldots, a_d $ l’ensemble $ C $ des points $ x $ de $ E $ tels que $ f_i(x) > 0 $ pour tout $ i \in I $; c’est une des chambres définies par $ \mathfrak{S} $ dans $ E $. L’adhérence de $ C $ est l’ensemble $ \overline{C} $ des points $ x $ de $ E $ tels que $ f_i(x) \geqslant 0 $ pour tout $ i \in I $; c’est l’enveloppe convexe de l’ensemble fini $ \{a_0, \ldots, a_d\} $ et l’on voit facilement que les points extrémaux de $ \overline{C} $ sont $ a_0, \ldots, a_d $.

Pour toute partie $ J $ de $ I $, distincte de $ I $, posons $ H_J = \bigcap_{i \in J} H_i $ et soit $ C_J $ l’ensemble des points $ x $ de $ E $ tels que $ f_i(x) = 0 $ pour $ i \in J $ et $ f_i(x) > 0 $ pour $ i \in I - J $. L’ensemble $ C_J $ est un simplexe ouvert dans l’espace affine $ H_J $ ayant pour sommets les points $ a_i $ pour $ i \in I - J $; on a $ C_\varnothing = C, \overline{C} = \bigcup_{J \neq I} C_J $ et $ C_J \neq C_{J'} $ pour $ J \neq J' $; de plus $ C_J $ est une facette de support $ H_J $. En particulier, les murs de $ C $ sont $ H_0, \ldots, H_d $ et $ C_{\{i\}} $ est la face contenue dans $ H_i $.

Pour toute partie non vide $ K $ de $ I $, soit $ B_K $ l’ensemble des points $ x $ de $ E $ tels que $ f_i(x) > 0 $ pour $ i \in K $ et $ f_i(x) < 0 $ pour $ i \in I - K $. Les ensembles $ B_K $ sont les chambres définies par $ \mathfrak{S} $ dans $ E $ et l’on a $ B_I = C $. On voit facilement que $ \overline{C} $ est compact; par contre, si $ K $ est une partie de $ I $ distincte de $ I $, de cardinal $ p $, la chambre $ B_K $ contient la suite des points $ x_n $ définis pour $ n \geqslant 2 $ par

$$
f_i(x_n) = \begin{cases}
n & \text{pour } i \in K \\
(1 - pn)/(d + 1 - p) & \text{pour } i \in I - K
\end{cases}
$$

et ceci prouve que $ B_K $ n’est pas relativement compacte.
