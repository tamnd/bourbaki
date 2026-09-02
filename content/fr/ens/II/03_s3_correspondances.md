---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 3
section_title: Correspondances
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0061-0074, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: Graphes et correspondances
      page: 9
      pdf_page: 61
    - "no": 2
      title: Correspondance réciproque d'une correspondance
      page: 0
      pdf_page: 63
    - "no": 3
      title: Composée de deux correspondances
      page: 0
      pdf_page: 63
    - "no": 4
      title: Fonctions
      page: 13
      pdf_page: 65
    - "no": 5
      title: Restrictions et prolongements de fonctions
      page: 15
      pdf_page: 67
    - "no": 6
      title: Définition d'une fonction par un terme
      page: 15
      pdf_page: 67
    - "no": 7
      title: Composée de deux fonctions. Fonction réciproque
      page: 0
      pdf_page: 68
    - "no": 8
      title: Rétractions et sections
      page: 18
      pdf_page: 70
    - "no": 9
      title: Fonctions de deux arguments
      page: 21
      pdf_page: 73
statements: 28
exercises: 11
content_sha256: bd8aaf627e5764e2a01125a05bc3c33a176dce7b0527e00ae4291443449ae378
---

## § 3. CORRESPONDANCES

### 1. Graphes et correspondances

#### Définition 1 {#ens-ii-s3-def-1 .statement tag=03PG}

On dit que $G$ est un graphe si tout élément de $G$ est un couple, autrement dit si la relation

$$(\forall z)(z \in G \Rightarrow (z est un couple))$$

est vraie.

Si $G$ est un graphe, la relation $(x,y) \in G$ s’exprime encore en disant que «$y$ correspond à $x$ par $G$».

Soit $R\{x,y\}$ une relation, $x$ et $y$ étant des lettres distinctes. Soit $G$ une lettre distincte de $x$ et de $y$ et ne figurant pas dans $R$. Si la relation

$$(\exists G)(G est un graphe et (\forall x)(\forall y)(R \Leftrightarrow ((x,y) \in G)))$$

est vraie, on dit que $R$ admet un graphe (par rapport aux lettres $x$ et $y$). Le graphe $G$ est alors unique en vertu de l’axiome d’extensionnalité, et s’appelle le graphe de $R$ (ou l’ensemble représentatif de $R$) par rapport à $x$ et $y$.

Soit $Z$ une lettre distincte de $x$ et de $y$ et ne figurant pas dans $R$. Si la relation

$$(\exists Z)(\forall x)(\forall y)(R \Rightarrow ((x,y) \in Z))$$

est vraie, $R$ admet un graphe: il suffit en effet de prendre pour ce graphe l’ensemble des couples $z$ tels que $z \in R\{\operatorname{pr}_1 z,\operatorname{pr}_2 z\}$ ($z$ étant une lettre distincte de $x$, $y$, $Z$ et ne figurant pas dans $R$). Cette condition est remplie si on connaît un terme $T$, où ne figurent ni $x$ ni $y$, tel que $R \Rightarrow ((x,y) \in T)$ soit vraie.

#### Proposition 1 {#ens-ii-s3-prop-1 .statement tag=03HI}

Soit $G$ un graphe. Il existe un ensemble $A$ et un seul, et un ensemble $B$ et un seul, qui possèdent les propriétés suivantes : 1) la relation $(\exists y)((x,y) \in G)$ est équivalente à $x \in A$; 2) la relation $(\exists x)((x,y) \in G)$ est équivalente à $y \in B$.

Il suffit en effet de prendre pour $A$ (resp. $B$) l’ensemble des objets de la forme $\operatorname{pr}_1 z$ (resp. $\operatorname{pr}_2 z$) pour $z \in G$ (II, p. 6): de façon précise, on a

$$A=\{x\mid(\exists y)((x,y)\in G)\}\quad\text{et}\quad B=\{y\mid(\exists x)((x,y)\in G)\}.$$

Ces ensembles s’appellent respectivement la première et la seconde projection du graphe $G$, ou encore l’ensemble de définition et l’ensemble des valeurs de $G$; on les désigne par $\operatorname{pr}_1\langle G\rangle$ et $\operatorname{pr}_2\langle G\rangle$ (ou $\operatorname{pr}_1 G$ et $\operatorname{pr}_2 G$ lorsqu’aucune confusion n’en résulte). On vérifie aussitôt que $G \subset (\operatorname{pr}_1 G) \times (\operatorname{pr}_2 G)$ : tout ensemble de couples est donc une partie d’un produit, et réciproquement. Si l’un des deux ensembles $\operatorname{pr}_1 G$, $\operatorname{pr}_2 G$ est vide, on a donc $G = \varnothing$ (II, p. 8, prop. 2).

#### Remarque {#ens-ii-s3-n1-rem-3 .statement tag=03S1}

La relation $x = y$ n’admet pas de graphe; car la première projection de ce graphe, s’il existait, serait l’ensemble de tous les objets (cf. II, p. 6, Remarque).

#### Définition 2 {#ens-ii-s3-def-2 .statement tag=03HJ}

On appelle correspondance entre un ensemble $A$ et un ensemble $B$ un triplet (II, p. 9) $\Gamma = (G, A, B)$ où $G$ est un graphe tel que $\operatorname{pr}_1 G \subset A$ et $\operatorname{pr}_2 G \subset B$. On dit que $G$ est le graphe de $\Gamma$, $A$ l’ensemble de départ et $B$ l’ensemble d’arrivée de $\Gamma$.

Si $(x,y) \in G$, on dit encore que « $y$ correspond à $x$ par la correspondance $\Gamma$ ».

Pour tout $x \in \operatorname{pr}_1 G$, on dit que la correspondance $\Gamma$ est définie pour l’objet $x$, et $\operatorname{pr}_1 G$ est appelé l’ensemble de définition (ou domaine) de $\Gamma$; pour tout $y \in \operatorname{pr}_2 G$, on dit que $y$ est une valeur prise par $\Gamma$ et $\operatorname{pr}_2 G$ est appelé l’ensemble des valeurs (ou image) de $\Gamma$.

Si $R\{x,y\}$ est une relation admettant un graphe $G$ (par rapport aux lettres $x$ et $y$), et si $A$ et $B$ sont deux ensembles tels que $\operatorname{pr}_1 G \subset A$ et $\operatorname{pr}_2 G \subset B$, on dit que $R$ est une relation entre un élément de $A$ et un élément de $B$ (relativement aux lettres $x,y$). On dit que la correspondance $\Gamma = (G,A,B)$ est la correspondance entre $A$ et $B$ définie par la relation $R$ (par rapport à $x$ et $y$).

Soient $G$ un graphe et $X$ un ensemble. La relation « $x \in X$ et $(x,y) \in G$ » entraîne $(x,y) \in G$ et admet par suite un graphe $G'$. La seconde projection de $G'$ se compose évidemment de tous les objets qui correspondent par $G$ à des objets de $X$.

#### Définition 3 {#ens-ii-s3-def-3 .statement tag=03PI}

Soient $G$ un graphe et $X$ un ensemble. L’ensemble des objets qui correspondent par $G$ à des éléments de $X$ s’appelle l’image de $X$ par $G$ et se désigne par $G\langle X\rangle$ ou $G(X)$.

Soient $\Gamma = (G,A,B)$ une correspondance, et $X$ une partie de $A$. L’ensemble $G\langle X\rangle$ se note encore $\Gamma\langle X\rangle$ ou $\Gamma(X)$ et s’appelle l’image de $X$ par $\Gamma$.

#### Remarque 1 {#ens-ii-s3-n1-rem-1 .statement tag=03PH}

D’une manière précise, $G\langle X\rangle$ désigne l’ensemble
$$
\{y \mid (\exists x)(x \in X \text{ et } (x,y) \in G)\}.
$$
Nous ne ferons plus que rarement désormais la traduction des définitions en langage formel.

#### Remarque 2 {#ens-ii-s3-n1-rem-2 .statement tag=03S2}

Les notations $G(X)$ et $\Gamma(X)$ peuvent parfois conduire à des confusions avec des notations introduites ultérieurement (cf. II, p. 14, Remarque).

Soit $G$ un graphe. Comme la relation $(x,y) \in G$ entraîne $y \in \operatorname{pr}_2 G$, on a $G\langle X\rangle \subset \operatorname{pr}_2 G$ pour tout ensemble $X$; comme $(x,y) \in G$ entraîne $x \in \operatorname{pr}_1 G$, on a $G\langle\operatorname{pr}_1 G\rangle = \operatorname{pr}_2 G$. On a $G\langle\varnothing\rangle = \varnothing$, puisque $x \notin \varnothing$ est un théorème. Si $X \subset \operatorname{pr}_1 G$ et $X \neq \varnothing$, on a $G\langle X\rangle \neq \varnothing$.

#### Proposition 2 {#ens-ii-s3-prop-2 .statement tag=03PJ}

Soient $G$ un graphe, $X$ et $Y$ deux ensembles; la relation $X \subset Y$ entraîne $G\langle X\rangle \subset G\langle Y\rangle$.

La proposition est évidente à partir des définitions et de C50 (II, p. 4).

E II.11                                     THÉORIE DES ENSEMBLES                                     § 3

#### Corollaire {#ens-ii-s3-n1-cor-1 .statement tag=03PK}

Si $A \supset \operatorname{pr}_1 G$, on a $G\langle A\rangle = \operatorname{pr}_2 G$.

#### Définition 4 {#ens-ii-s3-def-4 .statement tag=03PL}

Soient $G$ un graphe et $x$ un objet. On appelle coupe de $G$ suivant $x$ l'ensemble $G\langle\{x\}\rangle$ (qu'on désigne aussi parfois par $G(x)$, par abus de notation).

Il résulte aussitôt de C43 (I, p. 39) que la relation $y \in G\langle\{x\}\rangle$ est équivalente à $(x,y)\in G$. Si $G$ et $G'$ sont deux graphes, la relation $G \subset G'$ est donc équivalente à $(\forall x)(G\langle\{x\}\rangle \subset G'\langle\{x\}\rangle)$.

Si $\Gamma=(G,A,B)$ est une correspondance entre $A$ et $B$, pour tout $x\in A$ la coupe de $\Gamma$ suivant $x$ s'appelle encore la coupe de $\Gamma$ suivant $x$ et se note également $\Gamma\langle\{x\}\rangle$ (ou $\Gamma(x)$).

### 2. Correspondance réciproque d'une correspondance

Soient $G$ un graphe, $A=\operatorname{pr}_1G$, $B=\operatorname{pr}_2G$ ses projections. La relation $(y,x)\in G$ entraîne $(x,y)\in B\times A$; cette relation admet donc un graphe qui se compose des couples $(x,y)$ tels que $(y,x)\in G$.

#### Définition 5 {#ens-ii-s3-def-5 .statement tag=03PM}

Soient $G$ un graphe. Le graphe dont les éléments sont les couples $(x,y)$ tels que $(y,x)\in G$ s'appelle le graphe réciproque de $G$ et se désigne par $\overline{G}^{-1}$ ou $G^{-1}$.

Pour tout ensemble $X$, $\overline{G}^{-1}\langle X\rangle$ s'appelle l'image réciproque de $X$ par $G$.

Il est évident que le graphe réciproque de $\overline{G}^{-1}$ est $G$, et que l'on a $\operatorname{pr}_1\overline{G}^{-1}=\operatorname{pr}_2G$, $\operatorname{pr}_2\overline{G}^{-1}=\operatorname{pr}_1G$. En particulier, si $X$ et $Y$ sont deux ensembles, on a $\overline{X\times Y}^{-1}=Y\times X$. On dit qu'un graphe $G$ est symétrique si $\overline{G}^{-1}=G$.

Soit $\Gamma=(G,A,B)$ une correspondance entre $A$ et $B$. Comme $\operatorname{pr}_1\overline{G}^{-1}\subset B$ et $\operatorname{pr}_2\overline{G}^{-1}\subset A$, le triplet $(\overline{G}^{-1},B,A)$ est une correspondance entre $B$ et $A$, qu'on appelle la correspondance réciproque de $\Gamma$ et qu'on note $\overline{\Gamma}$ ou $\Gamma^{-1}$. Pour toute partie $Y$ de $B$, l'image $\overline{\Gamma}\langle Y\rangle$ de $Y$ par $\overline{\Gamma}$ s'appelle encore l'image réciproque de $Y$ par $\Gamma$. Il est évident que la correspondance réciproque de $\overline{\Gamma}$ est $\Gamma$.

### 3. Composée de deux correspondances

Soient $G$ et $G'$ deux graphes. Désignons par $A$ l'ensemble $\operatorname{pr}_1G$ et par $C$ l'ensemble $\operatorname{pr}_2G'$. La relation $(\exists y)((x,y)\in G$ et $(y,z)\in G')$ entraîne $(x,z)\in A\times C$; elle admet donc un graphe par rapport à $x$ et $z$.

#### Définition 6 {#ens-ii-s3-def-6 .statement tag=03PN}

Soient $G$ et $G'$ des graphes. On appelle composé de $G'$ et de $G$, et on désigne par $G'\circ G$ (ou parfois par $G'G$), le graphe par rapport à $x$ et $z$ de la relation $(\exists y)((x,y)\in G$ et $(y,z)\in G')$.

#### Proposition 3 {#ens-ii-s3-prop-3 .statement tag=03HK}

Soient $G$ et $G'$ deux graphes. Le graphe réciproque de $G' \circ G$ est $G^{-1} \circ G'^{-1}$.

En effet, la relation « $(x,y) \in G$ et $(y,z) \in G'$ » est équivalente à « $(z,y) \in G'^{-1}$ et $(y,x) \in G^{-1}$ ».

#### Proposition 4 {#ens-ii-s3-prop-4 .statement tag=03HL}

Soient $G_1,G_2,G_3$ des graphes. On a alors $(G_3 \circ G_2)\circ G_1=G_3\circ(G_2\circ G_1)$.

En effet, la relation $(x,t)\in(G_3\circ G_2)\circ G_1$ est équivalente à la relation

$$(\exists y)((x,y)\in G_1\ \text{et}\ (\exists z)((y,z)\in G_2\ \text{et}\ (z,t)\in G_3))$$

donc (notamment d’après C33 (I, p. 35)) à la relation

$$(\exists y)(\exists z)((x,y)\in G_1\ \text{et}\ (y,z)\in G_2\ \text{et}\ (z,t)\in G_3). \tag{1}$$

On voit de même que la relation $(x,t)\in G_3\circ(G_2\circ G_1)$ est équivalente à

$$(\exists z)(\exists y)((x,y)\in G_1\ \text{et}\ (y,z)\in G_2\ \text{et}\ (z,t)\in G_3). \tag{2}$$

Or on sait que les relations (1) et (2) sont équivalentes, ce qui démontre la prop. 4.

Le graphe $G_3\circ(G_2\circ G_1)$ se désigne par $G_3\circ G_2\circ G_1$. De même, si $G_1,G_2,G_3,G_4$ sont des graphes, on pose

$$G_4\circ(G_3\circ G_2\circ G_1)=G_4\circ G_3\circ G_2\circ G_1,$$

etc.

#### Proposition 5 {#ens-ii-s3-prop-5 .statement tag=03HM}

Soient $G$ et $G'$ des graphes et $A$ un ensemble. On a

$$(G'\circ G)\langle A\rangle=G'\langle G\langle A\rangle\rangle.$$

En effet, en vertu de C33 (I, p. 35), la relation $z\in(G'\circ G)\langle A\rangle$ est équivalente à

$$(\exists y)((\exists x)(x\in A\ \text{et}\ (x,y)\in G)\ \text{et}\ (y,z)\in G')$$

donc à $(\exists y)(y\in G\langle A\rangle\ \text{et}\ (y,z)\in G')$, ce qui démontre la proposition.

Si $G$ et $G'$ sont deux graphes, on a $\operatorname{pr}_1(G'\circ G)=G^{-1}\langle\operatorname{pr}_1G'\rangle$, et

$\operatorname{pr}_2(G'\circ G)=G'\langle\operatorname{pr}_2G\rangle$. Pour démontrer par exemple la seconde de ces relations, il suffit de remarquer que la relation $z\in\operatorname{pr}_2(G'\circ G)$ équivaut à $(\exists x)((x,z)\in G'\circ G)$, donc à

$$(\exists y)((\exists x)((x,y)\in G)\ \text{et}\ (y,z)\in G');$$

mais cette dernière est équivalente à $z\in G'\langle\operatorname{pr}_2G\rangle$.

Si $G$ est un graphe, $X$ un ensemble tel que $X\subset\operatorname{pr}_1G$, on a $X\subset G^{-1}\langle G\langle X\rangle\rangle$.

En effet, la relation $x\in X$ entraîne par hypothèse $(\exists y)((x,y)\in G)$; mais $(x,y)\in G$ est équivalente à $(y,x)\in G^{-1}$, et d’autre part $(x,y)\in G$ entraîne

$$(\exists z)(z\in X\ \text{et}\ (z,y)\in G);$$

donc $x \in X$ entraîne $(\exists y)((\exists z)(z \in X \text{ et } (z, y) \in G) \text{ et } (y, x) \in \overline{G}^{-1})$, c'est-à-dire $x \in \overline{G}^{-1}\langle G\langle X\rangle\rangle$.

Il est clair que si $G_1, G_2, G'_1, G'_2$ sont des graphes, les relations $G_1 \subset G_2$ et $G'_1 \subset G'_2$ entraînent $G'_1 \circ G_1 \subset G'_2 \circ G_2$.

Soient maintenant $\Gamma = (G, A, B)$ et $\Gamma' = (G', B, C)$ deux correspondances telles que l’ensemble d’arrivée de $\Gamma$ soit identique à l’ensemble de départ de $\Gamma'$. D’après ce qui précède, on a $\mathrm{pr}_1 (G' \circ G) \subset \mathrm{pr}_1 G \subset A$ et
$$
\mathrm{pr}_2 (G' \circ G) \subset \mathrm{pr}_2 G' \subset C;
$$
on peut donc poser la définition suivante:

#### Définition 7 {#ens-ii-s3-def-7 .statement tag=03PO}

*Soient $\Gamma = (G, A, B)$ et $\Gamma' = (G', B, C)$ deux correspondances telles que l’ensemble d’arrivée de $\Gamma$ soit identique à l’ensemble de départ de $\Gamma'$. On appelle composée de $\Gamma'$ et de $\Gamma$, et on note $\Gamma' \circ \Gamma$ (ou parfois $\Gamma'\Gamma$), la correspondance $(G' \circ G, A, C)$.*

Il résulte aussitôt de la prop. 5 que, si $X$ est une partie de $A$, on a $(\Gamma' \circ \Gamma)\langle X \rangle = \Gamma'\langle \Gamma\langle X \rangle \rangle$. En outre, comme l’ensemble d’arrivée de $\overline{\Gamma}'$ est identique à l’ensemble de départ de $\overline{\Gamma}$, la correspondance réciproque de $\Gamma' \circ \Gamma$ est $\overline{\Gamma}' \circ \overline{\Gamma}^{-1}$, en vertu de la prop. 3.

#### Définition 8 {#ens-ii-s3-def-8 .statement tag=03PP}

*Si $A$ est un ensemble, l’ensemble $\Delta_A$ des objets de la forme $(x, x)$, pour $x \in A$, s’appelle la diagonale de $A \times A$.*

Il est clair que l’on a $\mathrm{pr}_1 \Delta_A = \mathrm{pr}_2 \Delta_A = A$. La correspondance $\mathrm{Id}_A = (\Delta_A, A, A)$ est appelée la *correspondance identique* de $A$; elle est sa propre réciproque.

Si $\Gamma$ est une correspondance entre $A$ et $B$, $\mathrm{Id}_A$ la correspondance identique de $A$, $\mathrm{Id}_B$ la correspondance identique de $B$, on a $\Gamma \circ \mathrm{Id}_A = \mathrm{Id}_B \circ \Gamma = \Gamma$.

### 4. Fonctions

#### Définition 9 {#ens-ii-s3-def-9 .statement tag=03HN}

*On dit qu’un graphe $F$ est un graphe fonctionnel si, pour tout $x$, il existe au plus un objet correspondant à $x$ par $F$ (I, p. 40). On dit qu’une correspondance $f = (F, A, B)$ est une fonction si son graphe $F$ est un graphe fonctionnel, et si son ensemble de départ $A$ est égal à son ensemble de définition $\mathrm{pr}_1 F$. Autrement dit, une correspondance $f = (F, A, B)$ est une fonction si, pour tout $x$ appartenant à l’ensemble de départ $A$ de $f$, la relation $(x, y) \in F$ est fonctionnelle en $y$ (I, p. 41); l’objet unique correspondant à $x$ par $f$ s’appelle la valeur de $f$ pour l’élément $x$ de $A$, et se désigne par $f(x)$ ou $f_x$ (ou $F_x$).

Si $f$ est une fonction, $F$ son graphe et $x$ un élément de l’ensemble de définition de $f$, la relation $y = f(x)$ est donc équivalente à $(x, y) \in F$ (I, p. 41, critère C46).

CORRESPONDANCES

E II.14

#### Remarque {#ens-ii-s3-n4-rem-1 .statement tag=03HO}

Il faut prendre garde aux confusions que risque d’entraîner l’emploi simultané de la notation $f(x)$ et de la notation $f(X)$ (synonyme de $f(\langle X\rangle)$) introduite dans la déf. 3 (cf. II, p. 50, exerc. 11).

Soient A et B deux ensembles; on appelle application de A dans B une fonction $f$ dont l’ensemble de départ (égal à l’ensemble de définition) est égal à A et dont l’ensemble d’arrivée est égal à B; on dit aussi qu’une telle fonction est définie dans A et prend ses valeurs dans B.

Au lieu de dire « soit $f$ une application de A dans B », on emploiera souvent les phrases suivantes: « soit une application $f : A \rightarrow B$ » ou même « soit $f : A \rightarrow B$. » Pour faciliter la lecture d’un raisonnement où interviennent plusieurs applications, on fera usage de diagrammes tels que

$$
\begin{array}{ccccc}
&&C&&\\
&\nearrow g&&\searrow i&\\
A&\xrightarrow{\ f\ }&B&&E\\
&\searrow h&&\nearrow j&\\
&&D&&
\end{array}
$$

où un groupe de signes tel que $A \rightarrow B$ doit s’interpréter comme signifiant que $f$ est une application de A dans B.

On dit encore qu’une fonction $f$ définie dans A transforme $x$ en $f(x)$ (pour tout $x \in A$), ou que $f(x)$ est le transformé de $x$ par $f$, ou (par abus de langage) l’image de $x$ par $f$.

Dans certains cas, un graphe fonctionnel s’appelle aussi une famille; l’ensemble de définition s’appelle alors l’ensemble des indices, et l’ensemble des valeurs s’appelle, par abus de langage, l’ensemble des éléments de la famille; c’est surtout dans ce cas qu’on utilise la notation indicielle $f_x$ pour désigner la valeur de $f$ pour l’élément $x$. Lorsque l’ensemble des indices est le produit de deux ensembles, on dit souvent qu’il s’agit d’une famille double.

De même, une fonction dont l’ensemble d’arrivée est E s’appelle parfois une famille d’éléments de E. Lorsque tout élément de E est une partie d’un ensemble F, on dit aussi qu’on a une famille de parties de F.

Nous emploierons souvent, dans la suite de ce Traité, le mot « fonction » à la place de « graphe fonctionnel ».

**Exemples de fonctions.** — 1) L’ensemble vide est un graphe fonctionnel; toute fonction dont le graphe est vide a pour ensemble de définition et pour ensemble des valeurs l’ensemble vide; celle de ces fonctions dont l’ensemble d’arrivée est vide (autrement dit la fonction $(\varnothing,\varnothing,\varnothing)$) est appelée la fonction vide.

2) Soit A un ensemble; la correspondance identique de A (II, p. 13) est une fonction qu’on appelle l’application identique de A.

A tout ensemble A est ainsi associée une famille, constituée par l’application identique de A, dont A est l’ensemble des indices et l’ensemble des éléments. Par abus de langage, on désigne parfois un ensemble sous le nom de « famille »; c’est alors de la famille ainsi associée à l’ensemble considéré qu’il est question.

On dit qu'une fonction $f$ est *constante* si, quels que soient $x$ et $x'$ dans l'ensemble de définition de $f$, on a $f(x) = f(x')$.

Soit $f$ une application de l'ensemble $E$ dans l'ensemble $E$. On dit qu'un élément $x$ de $E$ est *invariant par $f$* si $f(x) = x$.

### 5. Restrictions et prolongements de fonctions

On dit que deux fonctions $f$ et $g$ *coïncident dans un ensemble* $E$ si $E$ est contenu dans les ensembles de définition de $f$ et de $g$, et si $f(x) = g(x)$ pour tout $x \in E$. Deux fonctions ayant même graphe coïncident dans leur ensemble de définition. Dire que $f = g$ revient à dire que $f$ et $g$ ont même ensemble de définition $A$, même ensemble d'arrivée $B$, et coïncident dans $A$.

Soient $f = (F, A, B)$ et $g = (G, C, D)$ deux fonctions. Dire que $F \subset G$ revient à dire que l'ensemble de définition $A$ de $f$ est contenu dans l'ensemble de définition $C$ de $g$, et que $g$ coïncide avec $f$ dans $A$. Si en outre $B \subset D$, on dit que $g$ est un *prolongement* de $f$ (ou, de façon plus précise, un prolongement de $f$ à $C$), ou que $g$ prolonge $f$ (à $C$). Lorsque $g$ est appelée une famille d'éléments de $D$, on dit aussi que $f$ est une *sous-famille* de $g$.

Soient $f$ une fonction, $X$ une partie de l'ensemble de définition $A$ de $f$. Il est immédiat que la relation « $x \in X$ et $y = f(x)$ » admet un graphe $G$ par rapport à $x$ et $y$, que ce graphe est fonctionnel et que $X$ est son ensemble de définition ; on dit que la fonction de graphe $G$, qui a le même ensemble d'arrivée que $f$, est la *restriction de $f$ à $X$*, et on la note parfois $f|_X$. Une fonction est un prolongement d'une quelconque de ses restrictions. Si deux fonctions $f, g$ ont même ensemble d'arrivée et coïncident dans un ensemble $E$, leurs restrictions à $E$ sont égales.

*Avec les notations précédentes, si $f = (F, A, B)$, $f|_X$ est égal à $(F \cap (X \times B), X, B)$, (II, p. 26); on dit encore que $f|_X$ est *déduite de $f$ par passage au sous-ensemble* $X$ de $A$. Soit $Y$ une partie de $B$ contenant $f(X)$; on dit que la fonction

$$(F \cap (X \times B), X, Y)$$

est *déduite de $f$ par passage aux sous-ensembles* $X$ de $A$ et $Y$ de $B$.*

### 6. Définition d'une fonction par un terme

C54. *Soient $T$ et $A$ deux termes, $x$ et $y$ des lettres distinctes. On suppose que $x$ ne figure pas dans $A$, et que $y$ ne figure ni dans $T$ ni dans $A$. Soit $R$ la relation « $x \in A$ et $y = T$ ». La relation $R$ admet un graphe $F$ par rapport aux lettres $x$ et $y$. Ce graphe est fonctionnel ; sa première projection est $A$, sa deuxième projection est l'ensemble des objets de la forme $T$ pour $x \in A$* (II, p. 6). *Pour tout $x \in A$, on a $F(x) = T$.*

En effet, soit $B$ l'ensemble des objets de la forme $T$ pour $x \in A$. On a $R \Rightarrow ((x, y) \in A \times B)$; comme l'assemblage désigné par $A \times B$ ne contient ni $x$,

Nº 7                                                                     CORRESPONDANCES                                                                     E II.16

ni y, R admet un graphe F par rapport aux lettres x et y (II, p. 9). Il est clair que la relation « $(x, y) \in F$ et $(x, y') \in F$ » entraîne $y = y'$, donc F est un graphe fonctionnel. Le reste du critère est évident.

Si C est un ensemble contenant l'ensemble B des objets de la forme T pour $x \in A$ (y ne figurant pas dans C), la fonction $(F, A, C)$ se désigne aussi par la notation $x \mapsto T$ ($x \in A$, $T \in C$); l'assemblage correspondant de la mathématique formelle ne contient ni x ni y et ne dépend pas du choix de la lettre y vérifiant les conditions précédentes. Quand le contexte est suffisamment explicite, on se contente des notations $x \mapsto T$ ($x \in A$), $(T)_{x \in A}$, ou $x \mapsto T$, et parfois simplement $T$ ou $(T)$. \* Ainsi, on peut parler de « la fonction $x^3$ », si le contexte indique clairement qu'il s'agit de l'application $x \mapsto x^3$ de l'ensemble des nombres complexes dans lui-même.\*

## Exemples

1) Si f est une application de A dans B, la fonction f est égale à la fonction $x \mapsto f(x)$ ($x \in A$, $f(x) \in B$), qu'on écrit simplement $x \mapsto f(x)$, ou aussi $(f_x)_{x \in A}$ (c'est surtout quand on utilise la dernière notation qu'on parle de « famille d'éléments » au lieu de « fonction »).

2) Soit G un ensemble de couples. Les fonctions

$$
z \mapsto \operatorname{pr}_1 z \quad (z \in G, \operatorname{pr}_1 z \in \operatorname{pr}_1 G)
$$

et

$$
z \mapsto \operatorname{pr}_2 z \quad (z \in G, \operatorname{pr}_2 z \in \operatorname{pr}_2 G)
$$

s'appellent respectivement la première et la seconde fonction coordonnée sur G; on les désigne par $\operatorname{pr}_1$ et $\operatorname{pr}_2$ quand il n'en résulte pas de confusion.

### 7. Composée de deux fonctions. Fonction réciproque

#### Proposition 6 {#ens-ii-s3-prop-6 .statement tag=03HP}

Si f est une application de A dans B, et g une application de B dans C, $g \circ f$ est une application de A dans C.

Soient F et G les graphes de f et g; montrons que $G \circ F$ est un graphe fonctionnel. Soient x, z, z' des objets tels que $(x, z) \in G \circ F$, $(x, z') \in G \circ F$. Il existe des objets y, y' tels que $(x, y) \in F$, $(x, y') \in F$, $(y, z) \in G$, $(y', z') \in G$. Puisque F est un graphe fonctionnel, on a $y = y'$, donc $(y, z') \in G$. Puisque G est un graphe fonctionnel, on en déduit que $z = z'$, ce qui prouve notre assertion. D'autre part, l'ensemble de définition de $g \circ f$ est évidemment A, ce qui achève la démonstration.

La fonction $g \circ f$ s'écrit aussi $x \mapsto g(f(x))$ (II, p. 16), et parfois $gf$ lorsqu'il ne peut en résulter de confusion.

#### Définition 10 {#ens-ii-s3-def-10 .statement tag=03HQ}

Soit f une application de A dans B. On dit que f est une injection, ou que f est une application injective, si deux éléments distincts de A ont des images distinctes par f. On dit que f est une surjection, ou que f est une application surjective, si $f(A)=B$.

On dit que $f$ est une bijection, ou que $f$ est une application bijective, si $f$ est à la fois injective et surjective.

Au lieu de dire que $f$ est injective, on dit aussi que $f$ est biunivoque. Au lieu de dire que $f$ est surjective, on dit aussi que $f$ est une application de $A$ sur $B$, ou une représentation paramétrique de $B$ au moyen de $A$ (dans ce dernier cas, $A$ s'appelle l'ensemble des paramètres de cette représentation, et ses éléments prennent le nom de paramètres). Si $f$ est bijective, on dit aussi que $f$ met $A$ et $B$ en correspondance biunivoque. Une bijection de $A$ sur $A$ s'appelle aussi une permutation de $A$.

Exemples

1) Si $A \subset B$, l'application de $A$ dans $B$ dont le graphe est la diagonale de $A$ est injective et s'appelle l'application canonique ou l'injection canonique (ou simplement l'injection) de $A$ dans $B$.

2) Soit $A$ un ensemble. L'application $x \mapsto (x, x)$ de $A$ dans $A \times A$ est une application injective appelée application diagonale de $A$.

3) Soit $G$ un ensemble de couples. L'application $\mathrm{pr}_1$ (resp. $\mathrm{pr}_2$) de $G$ dans $\mathrm{pr}_1 G$ (resp. $\mathrm{pr}_2 G$) est surjective; pour que $\mathrm{pr}_1$ soit injective, il faut et il suffit que $G$ soit un graphe fonctionnel.

4) Soit $G$ un ensemble de couples. L'application $z \mapsto (\mathrm{pr}_2 z, \mathrm{pr}_1 z)$ de $G$ dans $\overline{G}^{-1}$ est une bijection (dite canonique).

5) Soient $A$ un ensemble, $b$ un objet. L'application $x \mapsto (x, b)$ de $A$ dans $A \times \{b\}$ est une bijection.

6) Si $f$ est une application de $A$ dans $B$, l'application déduite de $f$ par passage aux sous-ensembles $A$ et $f(A)$ est surjective.

#### Proposition 7 {#ens-ii-s3-prop-7 .statement tag=03PQ}

Soit $f$ une application de $A$ dans $B$. Pour que $\overline{f}^{-1}$ soit une fonction, il faut et il suffit que $f$ soit bijective.

En effet, si $\overline{f}^{-1}$ est une fonction, son ensemble de départ $B$ est égal à son ensemble de définition, c'est-à-dire à $f(A)$. D'autre part, soient $x$ et $y$ deux éléments de $A$ tels que $f(x) = f(y)$. Si $F$ désigne le graphe de $f$, on a $(f(x), x) \in \overline{F}^{-1}$ et $(f(y), y) \in \overline{F}^{-1}$, donc $(f(x), y) \in \overline{F}^{-1}$, donc $x = y$, de sorte que $f$ est injective, et par suite bijective. Réciproquement, si $f$ est bijective, il est immédiat que $\overline{F}^{-1}$ est fonctionnel, et que l'ensemble de définition de $\overline{f}^{-1}$ est égal à $B$.

Lorsque $f$ est bijective, $\overline{f}^{-1}$ est appelée l'application réciproque de $f$; $\overline{f}^{-1}$ est bijective, $f \circ \overline{f}^{-1}$ est l'application identique de $A$ et $\overline{f}^{-1} \circ f$ est l'application identique de $B$.

Si une permutation est identique à la permutation réciproque, elle est dite involutive.

#### Remarque {#ens-ii-s3-n7-rem-1 .statement tag=03HR}

Soit $f$ une application de $A$ dans $B$; pour toute partie $X$ de $A$, on a vu (II, p. 12) que l’on a $X\subset f^{-1}\langle f(X)\rangle$. En outre, pour toute partie $Y$ de $B$, on a $f\langle f^{-1}(Y)\rangle\subset Y$: en effet, la relation $y\in f\langle f^{-1}(Y)\rangle$ équivaut à

$$
(\exists x)((\exists z)(z\in Y\ \mathrm{et}\ z=f(x))\ \mathrm{et}\ y=f(x))
$$

et elle entraîne donc la relation $(\exists z)(z\in Y\ \mathrm{et}\ y=z)$, et par suite aussi la relation $y\in Y$.

Si $f$ est une surjection, on a $f\langle f^{-1}(Y)\rangle=Y$ pour toute partie $Y$ de $B$, car la relation $y\in Y\subset B$ entraîne par hypothèse la relation $(\exists x)(y=f(x))$, donc aussi $(\exists x)(y\in Y\ \mathrm{et}\ y=f(x))$; mais «$y\in Y$ et $y=f(x)$» entraîne $(\exists z)(z\in Y\ \mathrm{et}\ z=f(x))$, d’où notre assertion.

Si $f$ est une injection, pour toute partie $X$ de $A$, on a $f^{-1}\langle f(X)\rangle=X$. En effet, la relation $x\in f^{-1}\langle f(X)\rangle$ équivaut à $f(x)\in f(X)$, donc à $(\exists z)(z\in X\ \mathrm{et}\ f(z)=f(x))$; mais l’hypothèse signifie que $f(z)=f(x)$ entraîne $z=x$, donc $x\in f^{-1}\langle f(X)\rangle$ entraîne $x\in X$.

### 8. Rétractions et sections

#### Proposition 8 {#ens-ii-s3-prop-8 .statement tag=03HS}

Soit $f$ une application de $A$ dans $B$. S’il existe une application $r$ (resp. $s$) de $B$ dans $A$ telle que $r\circ f$ (resp. $f\circ s$) soit l’application identique de $A$ (resp. $B$), $f$ est injective (resp. surjective). Réciproquement, si $f$ est surjective, il existe une application $s$ de $B$ dans $A$ telle que $f\circ s$ soit l’application identique de $B$. Si $f$ est injective et si $A\ne\varnothing$, il existe une application $r$ de $B$ dans $A$ telle que $r\circ f$ soit l’application identique de $A$.

En effet, s’il existe une application $r$ de $B$ dans $A$ telle que $r\circ f$ soit l’application identique de $A$, l’égalité $f(x)=f(y)$, où $x\in A$ et $y\in A$, entraîne $x=r(f(x))=r(f(y))=y$, donc $f$ est injective. S’il existe une application $s$ de $B$ dans $A$ telle que $f\circ s$ soit l’application identique de $B$, on a $B=f(s(B))\subset f(A)\subset B$, donc $f$ est surjective. Si $f$ est surjective, désignons par $T$ le terme $T_y(y\in A\ \mathrm{et}\ f(y)=x)$; on a $f(T)=x$ pour $x\in B$; si on désigne par $s$ l’application $x\mapsto T$ ($x\in B,T\in A$), $f\circ s$ est l’application identique de $B$. Enfin, supposons $f$ injective et $A\ne\varnothing$; soit $a$ un élément de $A$; la relation

$$
\langle(y\in A\ \mathrm{et}\ x=f(y))\ \mathrm{ou}\ (y=a\ \mathrm{et}\ x\in B-f(A))\rangle
$$

entraîne $(x,y)\in B\times A$, donc admet un graphe $R$ par rapport aux lettres $x$ et $y$. Ce graphe est fonctionnel en raison de l’hypothèse faite sur $f$, et a pour ensemble de définition $B$; enfin on a $R(x)=a$ si $x\in B-f(A)$ et $f(R(x))=x$ si $x\in f(A)$. Donc la fonction $r=(R,B,A)$ est telle que $r\circ f$ soit l’application identique de $A$.

#### Corollaire {#ens-ii-s3-n8-cor-1 .statement tag=03HT}

Soient $A$ et $B$ des ensembles, $f$ une application de $A$ dans $B$, $g$ une application de $B$ dans $A$. Si $g\circ f$ est l’application identique de $A$ et $f\circ g$ l’application identique de $B$, $f$ et $g$ sont bijectives et on a $g=f^{-1}$.

#### Définition 11 {#ens-ii-s3-def-11 .statement tag=03HU}

Soit $f$ une application injective (resp. surjective) de $A$ dans $B$. Toute application $r$ (resp. $s$) de $B$ dans $A$ telle que $r\circ f$ (resp. $f\circ s$) soit l’application identique de $A$ (resp. $B$) est appelée une rétraction (resp. section) associée à $f$.

Au lieu de rétraction (resp. section), on dit parfois inverse à gauche (resp. à droite).

Si $f$ est injective (resp. surjective), et si $r$ (resp. $s$) est une rétraction (resp. section) associée à $f$, $f$ est une section (resp. rétraction) associée à $r$ (resp. $s$). Donc une rétraction est surjective, une section est injective.

Si $f$ est surjective, et si $s, s'$ sont deux sections associées à $f$, telles que $s(B) = s'(B)$, on a $s = s'$; en effet, si $x \in B$, il existe un $y \in B$ que $s(x) = s'(y)$, et on a $x = f(s(x)) = f(s'(y)) = y$, donc $s(x) = s'(x)$, de sorte que $s = s'$. Ainsi une section $s$ est déterminée de manière unique par l’ensemble $s(B)$, de sorte que, par abus de langage, l’ensemble $s(B)$ lui-même s’appelle parfois une section associée à $f$.

#### Théorème 1 {#ens-ii-s3-thm-1 .statement tag=03PR}

Soient $f$ une application de $A$ dans $B$, $f'$ une application de $B$ dans $C$, et $f'' = f' \circ f$. Alors:

a) Si $f$ et $f'$ sont des injections, $f''$ est une injection ; si $r, r'$ sont des rétractions associées à $f$ et $f'$, $r \circ r'$ est une rétraction associée à $f''$.

b) Si $f$ et $f'$ sont des surjections, $f''$ est une surjection ; si $s, s'$ sont des sections associées à $f$ et $f'$, $s \circ s'$ est une section associée à $f''$.

c) Si $f''$ est une injection, $f$ est une injection ; si $r''$ est une rétraction associée à $f''$, $r'' \circ f'$ est une rétraction associée à $f$.

d) Si $f''$ est une surjection, $f'$ est une surjection ; si $s''$ est une section associée à $f''$, $f \circ s''$ est une section associée à $f'$.

e) Si $f''$ est une surjection et $f'$ une injection, $f$ est une surjection ; si $s''$ est une section associée à $f''$, $s'' \circ f'$ est une section associée à $f$.

f) Si $f''$ est une injection et $f$ une surjection, $f'$ est une injection ; si $r''$ est une rétraction associée à $f''$, $f \circ r''$ est une rétraction associée à $f'$.

Pour tout ensemble $E$, désignons par $\mathrm{Id}_E$ l’application identique de $E$.

a) On a $r \circ f = \mathrm{Id}_A$ et $r' \circ f' = \mathrm{Id}_B$, donc

$$
(r \circ r') \circ (f' \circ f) = r \circ \mathrm{Id}_B \circ f = r \circ f = \mathrm{Id}_A.
$$

Si $f$ et $f'$ sont des injections, $f''$ est donc une injection, d’après la prop. 8 si $A \neq \varnothing$, et de façon évidente si $A = \varnothing$.

b) On a $f \circ s = \mathrm{Id}_B$ et $f' \circ s' = \mathrm{Id}_C$, donc

$$
(f' \circ f) \circ (s \circ s') = f' \circ \mathrm{Id}_B \circ s' = f' \circ s' = \mathrm{Id}_C.
$$

Si $f$ et $f'$ sont des surjections, $f''$ est donc une surjection d’après la prop. 8.

c) On a $r'' \circ f'' = \mathrm{Id}_A$, donc $(r'' \circ f') \circ f = r'' \circ f'' = \mathrm{Id}_A$. Si $f''$ est une injection, $f$ est donc une injection, d’après la prop. 8 si $A \neq \varnothing$, et de façon évidente si $A = \varnothing$.

d) On a $f'' \circ s'' = \mathrm{Id}_C$, donc $f' \circ (f \circ s'') = f'' \circ s'' = \mathrm{Id}_C$. Si $f''$ est une surjection, $f'$ est donc une surjection d’après la prop. 8.

N° 8                                                                                                     CORRESPONDANCES                                                                                                 E II.20

e) On a $f''\circ s''=\mathrm{Id}_C$, et $f'$ est une bijection d’après d). Donc

$$
f\circ(s''\circ f')=(\overline{f'}^{-1}\circ f')\circ f\circ(s''\circ f')=\overline{f'}^{-1}\circ(f''\circ s'')\circ f'
$$

$$
=\overline{f'}^{-1}\circ\mathrm{Id}_C\circ f'=\overline{f'}^{-1}\circ f'=\mathrm{Id}_B.
$$

Si $f''$ est une surjection et $f'$ une injection, $f$ est donc une surjection d’après la prop. 8.

f) On a $r''\circ f''=\mathrm{Id}_A$, et $f$ est une bijection d’après c). Donc

$$
(f\circ r'')\circ f'=(f\circ r'')\circ f'\circ(f\circ f'^{-1})=f\circ(r''\circ f'')\circ f'^{-1}=f\circ\mathrm{Id}_A\circ f'^{-1}=f\circ f'^{-1}=\mathrm{Id}_B.
$$

Si $f''$ est une injection et $f$ une surjection, $f'$ est donc une injection, d’après la prop. 8 si $A\ne\varnothing$, et de façon évidente si $A=\varnothing$ (car on a alors $B=f\langle A\rangle=\varnothing$).

#### Proposition 9 {#ens-ii-s3-prop-9 .statement tag=03PS}

a) Soient $E,F,G$ des ensembles, $g$ une application de $E$ sur $F$, $f$ une application de $E$ dans $G$. Pour qu’il existe une application $h$ de $F$ dans $G$ telle que $f=h\circ g$ (fig. 1), il faut et il suffit que la relation $g(x)=g(y)$ (où $x\in E$, $y\in E$) entraîne la relation $f(x)=f(y)$. L’application $h$ est uniquement déterminée; si $s$ est une section associée à $g$, on a $h=f\circ s$.

$$
\begin{array}{ccc}
& E & \\
{}^{g}\swarrow & & \searrow^{f}\\
F & \xrightarrow{\ h\ } & G
\end{array}
$$

Fig. 1

$$
\begin{array}{ccc}
& E & \\
{}^{f}\nearrow & \uparrow^{g}\\
G & \xrightarrow{\ h\ } & F
\end{array}
$$

Fig. 2

b) Soient $E,F,G$ des ensembles, $g$ une application injective de $F$ dans $E$, $f$ une application de $G$ dans $E$. Pour qu’il existe une application $h$ de $G$ dans $F$ telle que $f=g\circ h$ (fig. 2), il faut et il suffit que $f(G)\subset g(F)$. L’application $h$ est uniquement déterminée; si $r$ est une rétraction associée à $g$, on a $h=r\circ f$.

a) Si $f=h\circ g$, la relation $g(x)=g(y)$ (où $x\in E$, $y\in E$) entraîne évidemment $f(x)=f(y)$. Et l’on a, pour toute section $s$ associée à $g$, $h=h\circ(g\circ s)$, ce qui montre que $h$ est uniquement déterminée par $f$. Réciproquement, supposons que la relation $g(x)=g(y)$ entraîne $f(x)=f(y);$ soit $s$ une section associée à $g$, et posons $h=f\circ s$; pour tout $x\in E$, on a $g(s(g(x)))=g(x)$, donc $f(s(g(x)))=f(x)$, c’est-à-dire $h(g(x))=f(x)$; on a donc bien $f=h\circ g$.

b) Si $f=g\circ h$, on a évidemment $f(G)\subset g(F)$, et pour toute rétraction $r$ associée à $g$, $h=(r\circ g)\circ h=r\circ f$, ce qui montre que $h$ est uniquement déterminée par $f$. Réciproquement, supposons que $f(G)\subset g(F)$; soit $r$ une rétraction associée à $g$, et posons $h=r\circ f$; pour tout $x\in G$, il existe un $y\in F$ tel que $f(x)=$ g(y), donc on a $g(h(x)) = g(r(f(x))) = g(r(g(y))) = g(y) = f(x)$; on a donc bien $f = g \circ h$.

### 9. Fonctions de deux arguments

On appelle fonction de deux arguments une fonction dont l’ensemble de définition est un ensemble de couples (ou, ce qui revient au même, une partie d’un produit). Soit $f$ une telle fonction; si $(x, y)$ est un élément de l’ensemble de définition de $f$, la valeur $f((x, y))$ de $f$ au point $(x, y)$ se désigne en général par $f(x, y)$.

Soient $f$ une fonction de deux arguments, $D$ son ensemble de définition, $C$ son ensemble d’arrivée. Pour tout $y$, soit $A_y$ l’ensemble des $x$ tels que $(x, y) \in D$ (c’est-à-dire la coupe de $\overline{D}^1$ suivant $y$ (n° 1)). L’application $x \mapsto f(x, y)$ ($x \in A_y, f(x, y) \in C$) s’appelle l’application partielle déterminée par $f$, relative à la valeur $y$ du second argument, et on la désigne par $f(., y)$ ou $f( , y)$ (ou parfois $f_y$); on a $f(., y)(x) = f(x, y)$ pour $(x, y) \in D$. De même, pour tout $x$, soit $B_x$ l’ensemble des $y$ tels que $(x, y) \in D$. L’application $y \mapsto f(x, y)$ ($y \in B_x, f(x, y) \in C$) s’appelle l’application partielle déterminée par $f$, relative à la valeur $x$ du premier argument, et on la désigne par $f(x, .)$ ou $f(x, )$ (ou parfois $f_x$); on a $f(x, .)(y) = f(x, y)$ pour $(x, y) \in D$.

Si, pour tout $y$ (resp. $x$), l’application partielle $f(., y)$ (resp. $f(x, .)$) est une application constante, on dit que $f$ ne dépend pas de son premier (resp. second) argument; cela signifie donc que $f(x, y) = f(x', y)$ si $(x, y)$ et $(x', y)$ sont dans $D$ (resp. $f(x, y) = f(x, y')$ si $(x, y)$ et $(x, y')$ sont dans $D$). Pour tout $y$ appartenant à la seconde projection de $D$, désignons par $g(y)$ la valeur commune des $f(x, y)$ pour $x \in A_y$; l’application $y \mapsto g(y)$ est une application de $\mathrm{pr}_2 D$ dans $C$, telle que $g(y) = f(x, y)$ pour $(x, y) \in D$.

Réciproquement, soit $g$ une application d’un ensemble $B$ dans un ensemble $C$, et soit $A$ un ensemble quelconque. L’application $(x, y) \mapsto g(y)$ de $A \times B$ dans $C$ ne dépend pas de son premier argument.

Soient $u$ une application de $A$ dans $C$, $v$ une application de $B$ dans $D$. L’application $z \mapsto (u(\mathrm{pr}_1 z), v(\mathrm{pr}_2 z))$ de $A \times B$ dans $C \times D$ s’appelle l’extension canonique (ou simplement extension) de $u$ et $v$ aux ensembles produits, ou encore produit de $u$ et $v$ (si aucune confusion n’est à craindre) et se désigne parfois par la notation $u \times v$ ou $(u, v)$; l’ensemble de ses valeurs est $u\langle A \rangle \times v\langle B \rangle$. Si $u$ et $v$ sont des applications injectives (resp. surjectives), $u \times v$ est une application injective (resp. surjective). Si $u$ et $v$ sont bijectives, $u \times v$ est bijective et l’application réciproque de $u \times v$ est $-u^{-1} \times -v^{-1}$. Si $u'$ est une application de $C$ dans $E$, $v'$ une application de $D$ dans $F$, on a

$$
(u' \times v') \circ (u \times v) = (u' \circ u) \times (v' \circ v).
$$

Si $U$ et $V$ sont les graphes respectifs de $u$ et $v$, le graphe $W$ de $u \times v$ est l’ensemble des couples $((x, y), (z, t))$ de $(A \times B) \times (C \times D)$ tels que $(x, z) \in U$ et $(y, t) \in V$; on le met en correspondance biunivoque avec le produit $U \times V$ (partie de $(A \times C) \times (B \times D)$) par l’application $((x, y), (z, t)) \mapsto ((x, z), (y, t))$ (cf. II, p. 35).

N° 1                             RÉUNION ET INTERSECTION D’UNE FAMILLE D’ENSEMBLES                             E II.22

## EXERCICES {#ens-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
