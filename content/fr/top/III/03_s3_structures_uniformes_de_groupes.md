---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 3
section_title: Structures uniformes de groupes
lang: fr
source: top-i-iv-fr
book_pages: TG III.19-TG III.27, TG III.72-TG III.74
pdf_pages: 0202-0210, 0255-0257
extraction: ocr
subsections:
    - "no": 1
      title: Structures uniformes droite et gauche sur un groupe topologique
      page: 19
      pdf_page: 202
    - "no": 2
      title: Structures uniformes des sous-groupes, groupes quotients et groupes produits
      page: 21
      pdf_page: 204
    - "no": 3
      title: Groupes complets
      page: 22
      pdf_page: 205
    - "no": 4
      title: Complétion d’un groupe topologique
      page: 23
      pdf_page: 206
    - "no": 5
      title: Structure uniforme et complétion d’un groupe commutatif
      page: 25
      pdf_page: 208
statements: 19
exercises: 12
content_sha256: b5d803ce4aeed8102e51e5356d16ec750a2ff3e58b462fa6ba5877831112f0cb
---

## § 3. STRUCTURES UNIFORMES DE GROUPES

### 1. Structures uniformes droite et gauche sur un groupe topologique

Dans un groupe topologique $C$, on aperçoit la possibilité de définir une notion de « points assez voisins », et par suite une structure uniforme, en opérant de la manière suivante: $x$ et $y$ étant deux points quelconques de $G$, on effectue sur ces deux points *la même translation* amenant l’un d’eux, par exemple $x$, sur l’élément neutre $e$; la « proximité » de $x$ et $y$ est alors évaluée, en quelque sorte, par le voisinage $V$ de $e$ dans lequel se trouve ramené $y$. Cette translation, qui revient à composer $x^{-1}$ avec $x$ et $y$ respectivement, peut d’ailleurs se faire *à droite* ou *à gauche*; nous allons voir que, dans chacun des deux cas, on obtient effectivement une structure uniforme sur $G$ *compatible* avec la topologie de $G$. Prenons le cas où la translation se fait *à droite*; à tout voisinage $V$ de $e$, on fait correspondre l’ensemble $V_d$ des couples $(x, y) \in G \times G$ tels que $yx^{-1} \in V$. Soit $\mathcal{G}_d$ la famille des ensembles $V_d$, lorsque $V$ parcourt le filtre $\mathfrak{V}$ des voisinages de $e$; $\mathcal{G}_d$ est un système fondamental d’entourages (II, p. 2). En effet, comme $e \in V$, la diagonale $\Delta$ de $G \times G$ est contenue dans $V_d$ quel que soit $V \in \mathfrak{V}$, donc $\mathcal{G}_d$ est une base de filtre et satisfait à $(\mathbf{U}_1')$ (II, p. 2); comme les relations $yx^{-1} \in V$ et $xy^{-1} \in V^{-1}$ sont équivalentes, on a $\overline{V}_d^1 = (V^{-1})_d$, donc, d’après $(\mathrm{GV}_{\mathrm{II}})$, $\overline{V}_d^1 \in \mathcal{G}_d$, d’où $(\mathbf{U}_{\mathrm{II}}')$ (II, p. 2); enfin, les relations $zx^{-1} \in V$ et $yz^{-1} \in V$ entraînent $yx^{-1} \in V.V$, donc $V_d \circ V_d \subset (V.V)_d$, et $(\mathrm{GV}_1)$ montre que $\mathcal{G}_d$ satisfait à $(\mathbf{U}_{\mathrm{III}}')$ (II, p. 2).

La structure uniforme définie par $\mathcal{G}_d$ est compatible avec la topologie de $G$, car les relations $y \in V_d(x)$ et $y \in V.x$ sont équivalentes par définition, autrement dit $V_d(x) = V.x$.

On raisonne de manière analogue lorsque la translation se fait à gauche, et on peut poser la définition suivante:

#### Définition 1 {#top-iii-s3-def-1 .statement}

On appelle structure uniforme droite (resp. gauche) sur un groupe topologique $G$, la structure uniforme dont un système fondamental d’entourages est obtenu en faisant correspondre à tout voisinage $V$ de l’élément neutre $e$, l’ensemble $V_d$ (resp. $V_s$) des couples $(x, y)$ tels que $yx^{-1} \in V$ (resp. $x^{-1}y \in V$).

Lorsque $V$ parcourt un système fondamental de voisinages de $e$, les ensembles $V_d$ (resp. $V_s$) forment un système fondamental d’entourages de la structure uniforme droite (resp. gauche).

A toute proposition sur la topologie d’un espace uniforme correspond une proposition sur la topologie d’un groupe, la traduction se faisant à l’aide de la déf. 1 et des formules $V_d(x) = V.x, V_d(A) = V.A, V_s(x) = x.V, V_s(A) = A.V$ qui en découlent immédiatement. Par exemple, on a, pour toute partie non vide $A$ de $G$ (II, p. 5, cor. 1),

$$
\overline{A} = \bigcap_{V \in \mathfrak{V}} V.A = \bigcap_{V \in \mathfrak{V}} A.V.
$$

De même (II, p. 5, cor. 3), tout groupe séparé est régulier.

La structure uniforme droite et la structure uniforme gauche sur un groupe topologique sont en général distinctes (voir III, p. 73, exerc. 4). Elles sont évidemment confondues si le groupe est commutatif, car alors $V_d = V_s$; elles sont aussi confondues si le groupe est compact (II, p. 27, th. 1).

En général, on désignera par $G_s$ (resp. $G_d$) l’espace uniforme obtenu en munissant l’ensemble $G$ de sa structure uniforme gauche (resp. droite).

#### Proposition 1 {#top-iii-s3-prop-1 .statement}

Les translations à droite et à gauche sont des isomorphismes de la structure uniforme droite sur elle-même.

Pour les translations à droite, c’est immédiat, car la relation $yx^{-1} \in V$ est équivalente à $(ya)(xa)^{-1} \in V$ (en d’autres termes, l’application $(x, y) \mapsto (xa, ya)$ laisse $V_d$ invariant). Pour les translations à gauche, cela résulte de $(\mathrm{GV}_{\mathrm{III}})$; en effet, la relation $yx^{-1} \in V$ est équivalente à $(ay)(ax)^{-1} \in aV_a^{-1}$, donc $x \mapsto ax$ est uniformément continue dans $G_d$.

On voit de même que les translations à droite et à gauche sont des isomorphismes de la structure uniforme gauche sur elle-même.

Tout automorphisme intérieur $x \mapsto axa^{-1}$ de G est donc à la fois un automorphisme de la structure de groupe, de la topologie, et de chacune des deux structures uniformes de G.

#### Proposition 2 {#top-iii-s3-prop-2 .statement}

*La symétrie* $x \mapsto x^{-1}$ *est un isomorphisme de la structure uniforme droite sur la structure uniforme gauche*.

C’est une conséquence immédiate de la déf. 1 (III, p. 19).

Il faut se garder de croire que l’application $(x, y) \mapsto xy$ de l’espace uniforme $G_d \times G_d$ dans l’espace uniforme $G_d$ soit en général uniformément continue. De même, la symétrie $x \mapsto x^{-1}$, considérée comme application de $G_d$ sur $G_d$, n’est pas en général uniformément continue (voir III, p. 73, exerc. 3 et 4).

#### Proposition 3 {#top-iii-s3-prop-3 .statement}

*Tout homomorphisme continu f d’un groupe topologique G dans un groupe topologique G' est uniformément continu lorsqu’on le considère comme une application de G_d dans G'_d* (ou de G_s dans G'_s).

En effet, si V' est un voisinage de l’élément neutre dans G', et $V = f^{-1}(V')$, la relation $yx^{-1} \in V$ entraîne $f(y)(f(x))^{-1} = f(yx^{-1}) \in V'$.

### 2. Structures uniformes des sous-groupes, groupes quotients et groupes produits

Si H est un sous-groupe d’un groupe topologique G, la structure uniforme induite sur H par la structure uniforme droite de G, n’est autre que la structure uniforme droite du groupe topologique H.

Si H est un sous-groupe distingué de G, et $\varphi$ l’application canonique de G sur $G/H$, on obtient un système fondamental d’entourages de la structure uniforme droite du groupe quotient $G/H$ en associant à tout voisinage V de l’élément neutre dans G, l’ensemble des couples $(\dot{x}, \dot{y})$ de points de $G/H$ tels que $\dot{y}\dot{x}^{-1} \in \varphi(V)$ (III, p. 13, prop. 17); cette condition signifie qu’il existe au moins un point $x \in \dot{x}$, et au moins un point $y \in \dot{y}$, tels que $yx^{-1} \in V$ (ce qui s’écrit aussi $(x, y) \in V_d$). En particulier, si N est l’adhérence de l’élément neutre dans G, la structure uniforme droite sur $G/N$ est isomorphe à la structure uniforme séparée *associée* à la structure uniforme droite sur G (cf. II, p. 24).

Enfin, sur un produit d’une famille $(G_t)$ de groupes topologiques, la structure uniforme droite est la structure *produit* des structures uniformes droites des $G_t$ (cf. II, p. 10).

On a des énoncés analogues pour la structure uniforme gauche.

Pour que les structures uniformes droite et gauche sur le groupe produit $\prod_t G_t$ soient identiques, il faut et il suffit que les structures uniformes droite et gauche de chacun des groupes facteurs $G_t$ soient identiques. Il en est toujours ainsi lorsque certains des $G_t$ sont commutatifs, et les autres compacts.

### 3. Groupes complets

#### Définition 2 {#top-iii-s3-def-2 .statement}

On dit qu’un groupe topologique est complet si sa structure uniforme droite et sa structure uniforme gauche sont des structures d’espace complet.

D’après la prop. 2 de III, p. 21, il suffit, pour qu’un groupe soit complet, que l’une de ses deux structures uniformes soit une structure d’espace complet. Pour que G soit complet, il faut et il suffit que le groupe séparé G/N associé à G (III, p. 13) le soit (II, p. 25).

Tout sous-groupe fermé d’un groupe complet est complet (II, p. 16, prop. 8). Tout produit de groupes complets est complet (II, p. 17, prop. 10).

Par contre, si G est un groupe complet et H un sous-groupe distingué fermé de G, le groupe quotient G/H n’est pas nécessairement complet (voir cependant IX, § 3, prop. 4).

#### Proposition 4 {#top-iii-s3-prop-4 .statement}

Si, dans un groupe topologique G, il existe un voisinage V de e qui est complet pour la structure uniforme droite ou la structure uniforme gauche, G est complet.

Supposons par exemple V complet pour la structure uniforme droite et soit F un filtre de Cauchy sur G_d ; F contient un ensemble M petit d’ordre V_d, et si x_1 ∈ M, on a donc M ⊂ Vx_1 ; la trace de F sur le sous-space complet Vx_1 de G_d est donc un filtre de Cauchy qui converge vers un point x_0 ; comme x_0 est adhérent à F, il est point limite de F (II, p. 14, cor. 2 de la prop. 5).

#### Corollaire 1 {#top-iii-s3-prop-4-cor-1 .statement}

Un groupe localement compact est complet.

En effet, tout espace compact est complet pour son unique structure uniforme (II, p. 27, th. 1).

#### Corollaire 2 {#top-iii-s3-prop-4-cor-2 .statement}

Tout sous-groupe localement compact d’un groupe topologique séparé G est fermé dans G.

En effet, tout sous-espace complet d’un espace uniforme séparé est fermé (II, p. 16, prop. 8).

#### Proposition 5 {#top-iii-s3-prop-5 .statement}

Soient G_1 un groupe topologique, G_2 un groupe topologique séparé et complet, H_1 (resp. H_2) un sous-groupe partout dense de G_1 (resp. G_2). Tout homomorphisme continu u de H_1 dans H_2 se prolonge d’une seule manière en un homomorphisme continu ū de G_1 dans G_2. En outre, si G_1 est séparé et complet, et si u est un isomorphisme de H_1 sur H_2, ū est un isomorphisme de G_1 sur G_2.

En effet, u est uniformément continu pour les structures uniformes droites de H_1 et H_2 (III, p. 21, prop. 3), donc se prolonge d’une seule manière en une application ū de G_1 dans G_2, uniformément continue pour les structures uniformes droites de ces groupes (II, p. 20, th. 2). En outre, en vertu du principe de prolongement des identités (I, p. 53, cor. 1), ū est un homomorphisme de G_1 dans G_2, d’où la première assertion. Pour démontrer la seconde, il suffit de considérer l’isomorphisme v de H_2 sur H_1 réciproque de u, et son prolongement ū en un homomorphisme continu de G_2 dans G_1 ; en vertu de l’unicité du prolongement, $\bar{v} \circ \bar{u}$ et $\bar{u} \circ \bar{v}$ sont respectivement l’identité dans $G_1$ et dans $G_2$, donc (E, II, p. 18) $\bar{u}$ est bijective.

#### Remarque {#top-iii-s3-n3-rem-1 .statement}

Lorsque l’homomorphisme continu $u$ est bijectif, il n’en résulte pas en général que $\bar{u}$ soit injectif ni surjectif (cf. III, p. 73, exerc. 12); voir toutefois III, p. 26, prop. 10.

### 4. Complétion d’un groupe topologique

Soit G un groupe topologique séparé. L’espace uniforme $G_d$ peut être considéré comme sous-espace partout dense de son complété $\hat{G}_d$. Nous allons chercher si on peut considérer G comme sous-groupe partout dense d’un groupe séparé et complet $G'$. S’il en est ainsi, l’espace uniforme $G'_d$ est nécessairement isomorphe à $\hat{G}_d$ (II, p. 20, corollaire); on doit donc pouvoir définir sur $\hat{G}_d$ une structure de groupe topologique qui induise sur G la structure de groupe topologique donnée. Il nous faut par suite examiner : 1° si on peut prolonger par continuité les fonctions $xy$ et $x^{-1}$ à $\hat{G}_d \times \hat{G}_d$ et à $\hat{G}_d$ respectivement; 2° si les fonctions ainsi prolongées définissent bien sur $\hat{G}_d$ une structure de groupe (elles définiront alors nécessairement une structure de groupe topologique induisant sur G la structure donnée). Nous devrons ensuite établir que : 3° lorsque les opérations précédentes sont possibles, le groupe topologique qu’elles définissent est complet. Enfin, nous verrons que : 4° s’il existe un groupe complet répondant à la question, il est unique à une isomorphe près.

1) Prolongement par continuité de $xy$ et $x^{-1}$. — Les fonctions $xy$ et $x^{-1}$ n’étant pas uniformément continues en général, on ne peut appliquer le théorème de prolongement des fonctions uniformément continues (II, p. 20, th. 2). Néanmoins, on peut prolonger $xy$, grâce à la prop. 11 de II, p. 20 et à la proposition suivante:

#### Proposition 6 {#top-iii-s3-prop-6 .statement}

Soient $\mathcal{F}$ et $\mathcal{G}$ deux filtres-de Cauchy sur $G_d$; l’image, par l’application $(x, y) \mapsto xy$, du filtre $\mathcal{F} \times \mathcal{G}$, est une base de filtre de Cauchy sur $G_d$.

Évaluons la « proximité » de $xy$ et $x'y'$ dans $G_d$, autrement dit, formons le produit $(x'y')(xy)^{-1} = x'y'y^{-1}x^{-1}$; pour tout $a \in G$, on peut encore écrire $(x'y')(xy)^{-1} = (x'a^{-1})(ay'y^{-1}a^{-1})(ax^{-1})$; nous allons voir qu’en choisissant convenablement $a$, chacun des trois facteurs de ce produit est très petit dès que les couples $(x, y)$ et $(x', y')$ appartiennent tous deux à un même ensemble assez petit de $\mathcal{F} \times \mathcal{G}$. En effet, voit V un voisinage quelconque de $e$ dans G; il existe un ensemble $A \in \mathcal{F}$, petit d’ordre $V_d$; prenons pour $a$ un point de A; si $x$ et $x'$ sont deux points quelconques de A, on a $x'a^{-1} \in V$ et $ax^{-1} \in V$. D’autre part, la relation $ay'y^{-1}a^{-1} \in V$ équivaut à $y'y^{-1} \in a^{-1}Va = W$; comme W est un voisinage de $e$, il existe un ensemble $B \in \mathcal{G}$, petit d’ordre $W_d$; donc, quels que soient $(x, y)$ et $(x', y')$ dans $A \times B$, on a $(x'y')(xy)^{-1} \in V^3$, ce qui démontre la proposition.

Pour qu’on puisse prolonger $x^{-1}$ par continuité à $\hat{G}_d$, il faut et il suffit que l’image, par la symétrie $x \mapsto x^{-1}$, d’un filtre de Cauchy sur $G_d$ soit un filtre de Cauchy sur

G_d (II, p. 20, prop. 11). On peut donner des exemples de groupes topologiques G pour lesquels cette condition n’est pas vérifiée (cf. X, § 3, exerc. 16); nous supposerons qu’elle est vérifiée dans la suite de ce raisonnement.

2) Les fonctions xy et x^{-1} prolongées, définissent une structure de groupe sur $\hat{G}_d$. — En effet, si on applique le principe de prolongement des identités (I, p. 53, cor. 1) aux fonctions x(yz) et (xy)z définies dans $\hat{G}_d \times \hat{G}_d \times \hat{G}_d$, et égales dans le sous-espace partout dense $G_d \times G_d \times G_d$, on voit que la loi de composition $(x, y) \mapsto xy$ est associative dans $\hat{G}_d$. Pour la même raison, les fonctions $x, ex, xe$ sont identiques dans $\hat{G}_d$, et les fonctions $e, xx^{-1}, x^{-1}x$ sont identiques dans $\hat{G}_d$.

3) Le groupe topologique $\hat{G}_d$ est complet. — En effet, soit $\mathcal{U}_d$ sa structure uniforme droite, et soit $\mathcal{U}$ la structure uniforme obtenue sur $\hat{G}_d$ par complétion de la structure uniforme droite de G. Les structures $\mathcal{U}$ et $\mathcal{U}_d$ induisent la même structure uniforme sur G; toute base de filtre de Cauchy $\mathfrak{B}$ sur G pour la structure $\mathcal{U}_d$ est donc une base de filtre de Cauchy pour la structure $\mathcal{U}$. Or, $\mathfrak{B}$ converge dans $\hat{G}_d$, puisque $\mathcal{U}$ est une structure d’espace complet; comme les topologies sur $\hat{G}_d$ déduites de $\mathcal{U}$ et $\mathcal{U}_d$ sont identiques (la topologie déduite de $\mathcal{U}$ étant compatible avec la structure de groupe de $\hat{G}_d$ en vertu de 2)), on voit (II, p. 17, prop. 9) que $\mathcal{U}_d$ est une structure d’espace complet. Cette conclusion montre d’ailleurs que $\mathcal{U}$ et $\mathcal{U}_d$ sont identiques (II, p. 20, corollaire).

4) Unicité. — Elle résulte de la prop. 5 de III, p. 22.

En résumé, nous avons démontré le théorème suivant:
Théorème 1. — Pour qu’un groupe topologique séparé G soit isomorphe à un sous-groupe partout dense d’un groupe complet $\hat{G}$, il faut et il suffit que l’image, par la symétrie $x \mapsto x^{-1}$, d’un filtre de Cauchy pour la structure uniforme droite de G soit encore un filtre de Cauchy pour cette structure. Le groupe complet $\hat{G}$ (qu’on appelle le groupe complété de G) est alors unique (à un isomorphisme près).

#### Proposition 7 {#top-iii-s3-prop-7 .statement}

Soit G un groupe topologique séparé admettant un groupe complété $\hat{G}$. Les adhérences, dans $\hat{G}$, des voisinages de l’élément neutre dans G, forment un système fondamental de voisinages de l’élément neutre dans $\hat{G}$.

En effet, $\hat{G}$ étant régulier, tout voisinage de l’élément neutre dans $\hat{G}$ contient l’adhérence V d’un voisinage ouvert U de $e$ dans $\hat{G}$ et V est aussi l’adhérence de la trace de U sur G.

Soit G un groupe non nécessairement séparé; soient N = $\overline{\{e\}}$, G' = G/N le groupe séparé associé à G (III, p. 13). Si G' admet un groupe complété $\hat{G}'$, on dit que ce dernier est le groupe séparé complété de G et on le note $\hat{G}$; $\hat{G}'_d$ (resp. $\hat{G}'_s$) est alors l’espace uniforme séparé complété (II, p. 23) de $G_d$ (resp. $G_s$).

#### Proposition 8 {#top-iii-s3-prop-8 .statement}

*Soient G un groupe admettant un groupe séparé complété $\hat{G}'$. Tout homomorphisme continu u de G dans un groupe séparé complet H se factorise d’une seule manière en $u = v \circ \varphi$, où v est un homomorphisme continu de $\hat{G} = \hat{G}'$ dans H et $\varphi$ l’application canonique de G dans $\hat{G}$ (composée de l’injection canonique de $G'$ dans $\hat{G}$ et de l’homomorphisme canonique $\psi$ de G sur $G/N = G'$).*

Comme le noyau de u est fermé et contient e, il contient N, donc u s’écrit $u = w \circ \psi$, où w est un homomorphisme continu de $G'$ dans H; il suffit alors d’appliquer à w la prop. 5 de III, p. 22.

#### Corollaire {#top-iii-s3-n4-cor-1 .statement}

*Soient $G_1, G_2$ deux groupes topologiques admettant des groupes séparés complétés $\hat{G}_1, \hat{G}_2$ respectivement. Pour tout homomorphisme continu $f : G_1 \to G_2$, il existe un homomorphisme continu $\hat{f} : \hat{G}_1 \to \hat{G}_2$ et un seul rendant commutatif le diagramme*

$$
\begin{array}{ccc}
G_1 & \xrightarrow{f} & G_2 \\
\varphi_1 \downarrow & & \varphi_2 \downarrow \\
\hat{G}_1 & \xrightarrow{\hat{f}} & \hat{G}_2
\end{array}
$$

*où $\varphi_1$ et $\varphi_2$ sont les homomorphismes canoniques.*

Il suffit d’appliquer la prop. 8 à l’homomorphisme $\varphi_2 \circ f : G_1 \to \hat{G}_2$.

#### Proposition 9 {#top-iii-s3-prop-9 .statement}

*Soit G un groupe topologique séparé. S’il existe un voisinage $V_0$ de l’élément neutre tel que l’application $x \mapsto x^{-1}$ de $V_0$ dans G soit uniformément continue pour la structure uniforme droite, alors G admet un groupe complété.*

Montrons que le critère du th. 1 est vérifié. Soit donc $\mathcal{F}$ un filtre de Cauchy pour la structure uniforme droite de G; il existe par suite un ensemble $A \in \mathcal{F}$ petit d’ordre $(V_0)_d$ pour cette structure; autrement dit, si $a \in A$, on a $xa^{-1} \in V_0$ pour tout $x \in A$, ou encore $A \subset V_0a$. Montrons que pour tout voisinage W de e, il existe un ensemble $B \subset A$ appartenant à $\mathcal{F}$ et tel que $B^{-1}$ soit petit d’ordre $W_d$: cela signifie que, pour $x, y$ dans B, on doit avoir $y^{-1}x \in W$. Or, on peut écrire $x = sa$ et $y = ta$, avec $s, t$ dans $V_0$, et on a alors $yx^{-1} = ts^{-1}$ et $y^{-1}x = a^{-1}t^{-1}sa$. Par hypothèse, il existe un voisinage $W'$ de e tel que les relations $s \in V_0, t \in V_0$ et $ts^{-1} \in W'$ entraînent $t^{-1}s \in aWa^{-1}$; si $B \subset A$ est un ensemble de $\mathcal{F}$ petit d’ordre $W'_d$, on aura donc bien $y^{-1}x \in W$ quels que soient $x, y$ dans B, ce qui prouve la proposition.

### 5. Structure uniforme et complétion d’un groupe commutatif

Nous avons déjà remarqué que, dans un groupe topologique commutatif G, les structures uniformes droite et gauche sont identiques; lorsqu’on parle de la structure uniforme de G, c’est toujours de cette unique structure qu’il est question.

#### Théorème 2 {#top-iii-s3-thm-2 .statement}

Soit G un groupe topologique commutatif; les fonctions $x^{-1}$ et $xy$ sont uniformément continues dans G et $G \times G$ respectivement; en outre G admet un groupe séparé complété $\hat{G}$, qui est commutatif.

La continuité uniforme de $x^{-1}$ résulte de la prop. 2 de III, p. 21 ; celle de $xy$, de la prop. 3 de III, p. 21, puisque $(x, y) \mapsto xy$ est un homomorphisme continu de $G \times G$ dans G. Si G est séparé, il satisfait à la condition du th. 1 de III, p. 24 (comme tout groupe séparé dont les structures uniformes droite et gauche sont identiques); en outre, les fonctions $xy$ et $yx$ sont égales dans $\hat{G} \times \hat{G}$, d’après le principe de prolongement des identités. D’où la seconde assertion, en considérant dans le cas général le groupe séparé associé à G.

On déduit en particulier de ce théorème que, si $f$ et $g$ sont deux applications uniformément continues d’un espace uniforme E dans un groupe commutatif G, noté additivement, les fonctions $-f$ et $f + g$ sont uniformément continues.

#### Proposition 10 {#top-iii-s3-prop-10 .statement}

Soient G un groupe commutatif, $\mathcal{T}_1, \mathcal{T}_2$ deux topologies séparées compatibles avec la structure de groupe de G; on suppose que $\mathcal{T}_1$ est plus fine que $\mathcal{T}_2$ et qu’il existe un système fondamental de voisinages de 0 pour $\mathcal{T}_1$ qui soient fermés pour $\mathcal{T}_2$. Soient $G_1, G_2$ les groupes complétés de G pour $\mathcal{T}_1$ et $\mathcal{T}_2$ respectivement, et soit $f : G_1 \to G_2$ l’homomorphisme continu qui prolonge l’application identique de G (III, p. 22, prop. 5); alors $f$ est injectif.

Supposons G noté additivement. Soit $\mathcal{U}_1$ la structure uniforme sur G correspondant (III, p. 20) à la topologie $\mathcal{T}_1$; il suffira de montrer que si $\mathcal{F}$ et $\mathcal{F}'$ sont deux filtres de Cauchy minimaux (II, p. 14) pour $\mathcal{U}_1$, qui convergent dans $G_2$ vers le même point a, alors $\mathcal{F} = \mathcal{F}'$ (II, p. 21). Pour cela, il suffit de montrer que $\mathcal{F} \cap \mathcal{F}'$ est un filtre de Cauchy pour $\mathcal{U}_1$. Soit V un voisinage de 0 dans G pour $\mathcal{T}_1$, fermé pour $\mathcal{T}_2$; soit W un voisinage symétrique de 0 dans G pour $\mathcal{T}_1$, tel que $W + W \subset V$. Par hypothèse, il existe dans $\mathcal{F}$ (resp. $\mathcal{F}'$) un ensemble M (resp. $M'$) petit d’ordre $W_d$; pour $x \in M, y \in M$, on a donc $y - x \in W$, ou encore $y \in x + W$; si $\overline{W}$ et $\overline{V}$ sont les adhérences de W et V dans $G_2$, on déduit de ce qui précède que $y \in x + \overline{W}$, donc, puisque a est adhérent à M, $a \in x + \overline{W}$ pour tout $x \in M$. De même, on a $a \in x' + \overline{W}$ pour tout $x' \in M'$, d’où l’on tire $x - x' \in \overline{W} + \overline{W}$; mais comme $(x, y) \mapsto x + y$ est une application continue de $G_2 \times G_2$ dans $G_2$, on a $\overline{W} + \overline{W} \subset \overline{W} + \overline{W} \subset \overline{V}$. On en conclut que pour $x \in M, x' \in M'$, on a $x - x' \in \overline{V} \cap G = V$, puisque V est fermé pour $\mathcal{T}_2$; ceci achève donc la démonstration.

#### Corollaire 1 {#top-iii-s3-prop-10-cor-1 .statement}

Sous les hypothèses de la prop. 10, si A est une partie de G qui est un sous-espace complet pour la structure uniforme $\mathcal{U}_2$ correspondant à $\mathcal{T}_2$, A est aussi un sous-espace complet pour la structure uniforme $\mathcal{U}_1$ correspondant à $\mathcal{T}_1$.

En effet, si $A_1$ est l’adhérence de $A$ dans $G_1$, $f(A_1)$ est contenu dans l’adhérence de $A$ dans $G_2$, égale à $A$ par hypothèse. Comme $f(A) = A$ par définition et que $f$ est injective, on a $A_1 = A$.

#### Corollaire 2 {#top-iii-s3-prop-10-cor-2 .statement}

Soient $G$ un groupe commutatif, $\mathcal{T}_1, \mathcal{T}_2$ deux topologies séparées compatibles avec la structure de groupe de $G$. On suppose que $\mathcal{T}_1$ est plus fine que $\mathcal{T}_2$ et qu’il existe un système fondamental $\mathfrak{V}$ de voisinages de $0$ pour $\mathcal{T}_1$ qui soient complets pour la structure uniforme $\mathcal{U}_2$ correspondant à $\mathcal{T}_2$. Alors $G$ est complet pour la structure uniforme $\mathcal{U}_1$ correspondant à $\mathcal{T}_1$.

En effet, les ensembles de $\mathfrak{V}$ sont fermés pour $\mathcal{T}_2$, donc complets pour $\mathcal{U}_1$ en vertu du cor. 1 ; la proposition résulte alors de la prop. 4 de III, p. 22.

## EXERCICES {#top-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
