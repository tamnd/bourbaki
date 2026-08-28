---
book: top
book_title: General Topology
chapter: II
chapter_title: STRUCTURES UNIFORMES
section: 4
section_title: Relations entre espaces uniformes et espaces compacts
lang: fr
source: top-i-iv-fr
book_pages: TG II.36-TG II.41
pdf_pages: 0166-0173, 0175-0180
extraction: ocr
subsections:
    - "no": 1
      title: Uniformité des espaces compacts
      page: 0
      pdf_page: 166
    - "no": 2
      title: Compacité des espaces uniformes
      page: 29
      pdf_page: 168
    - "no": 3
      title: Ensembles compacts dans un espace uniforme
      page: 31
      pdf_page: 170
    - "no": 4
      title: Ensembles connexes dans un espace compact
      page: 31
      pdf_page: 170
statements: 24
exercises: 26
content_sha256: 24a2100c7cc0d3ea1bced67c85c6191269d314297435893540570ef24dc000ed
---

## § 4. RELATIONS ENTRE ESPACES UNIFORMES ET ESPACES COMPACTS

### 1. Uniformité des espaces compacts

#### Définition 1 {#top-ii-s4-def-1 .statement}

On dit qu’une structure uniforme sur un espace topologique $X$ est compatible avec la structure de $X$ si cette dernière est identique à la topologie déduite de la structure uniforme considérée.

On dit qu’un espace topologique est uniformisable et que sa topologie est uniformisable s’il existe une structure uniforme compatible avec sa topologie.

Il existe des espaces topologiques non uniformisables, par exemple (en vertu de II, p. 5, cor. 3) les espaces ne vérifiant par l’axiome $(O_{III})$; le problème se pose donc de déterminer à quelle condition un espace topologique $X$ est uniformisable.

Ce n’est que dans IX, § 1, que nous donnerons une réponse complète à cette question. Dans ce paragraphe, nous n’examinerons qu’un cas particulier important, celui où $X$ est compact. On a alors le théorème suivant:

#### Théorème 1 {#top-ii-s4-thm-1 .statement}

Sur un espace compact $X$, il existe une structure uniforme et une seule compatible avec la topologie de $X$; l’ensemble des entourages de cette structure est identique à l’ensemble des voisinages de la diagonale $\Delta$ dans $X \times X$; en outre, $X$, muni de cette structure uniforme, est un espace uniforme complet.

La dernière partie du théorème est immédiate : tout filtre de Cauchy sur $X$ a en effet un point adhérent (axiome (C)), donc est convergent (II, p. 14, cor. 2 de la prop. 5).

Montrons en second lieu que, s’il existe une structure uniforme compatible avec la topologie de $X$, l’ensemble $\mathcal{U}$ des entourages de cette structure est identique à l’ensemble des voisinages de $\Delta$. On sait déjà que tout entourage est un voisinage de $\Delta$ (II, p. 4, prop. 2); il suffit d’établir inversement que tout voisinage de $\Delta$ appartient à $\mathcal{U}$. Supposons qu’il existe un voisinage $U$ de $\Delta$ n’appartenant pas à $\mathcal{U}$; alors les ensembles $V \cap \mathcal{G}U$, où $V$ parcourt $\mathcal{U}$, formeraient une base d’un filtre $\mathcal{G}$ sur l’espace compact $X \times X$; $\mathcal{G}$ aurait par suite un point adhérent $(a, b)$ n’appartenant pas à $\Delta$; comme $\mathcal{U}$ serait alors un filtre moins fin que $\mathcal{G}$, $(a, b)$ serait aussi adhérent à $\mathcal{U}$. Or, la structure uniforme définie par $\mathcal{U}$ est séparée par hypothèse, donc l’intersection des adhérences des ensembles de $\mathcal{U}$ est $\Delta$ (II, p. 5, cor. 2 et prop. 3); on aboutit ainsi à une contradiction.

Il reste à montrer que l’ensemble $\mathcal{V}$ des voisinages de $\Delta$ dans $X \times X$ est l’ensemble des entourages d’une structure uniforme compatible avec la topologie de $X$. Il suffira pour cela de voir que $\mathcal{V}$ est l’ensemble des entourages d’une structure uniforme séparée sur $X$; car s’il en est ainsi, la topologie déduite de cette structure sera une topologie moins fine que la topologie de $X$ (I, p. 11, prop. 3), donc nécessairement identique à cette dernière (I, p. 63, cor. 3).

Il est clair que $\mathcal{V}$ vérifie les axiomes $(F_I)$ et $(F_{II})$; montrons que les axiomes

(U_{II}) et (U_{III}) sont aussi vérifiés et que Δ est l’intersection des ensembles de $\mathfrak{V}$. Ce dernier point est immédiat, car tout ensemble réduit à un point $(x, y)$ de $X \times X$ est fermé, puisque $X$ est séparé; donc, si $x \neq y$ dans $X$, le complémentaire de $(x, y)$ dans $X \times X$ est un voisinage de $Δ$. Comme la symétrie $(x, y) \mapsto (y, x)$ est un homéomorphisme de $X \times X$ sur lui-même, pour tout $V \in \mathfrak{V}$, on a aussi $\overline{V}^1 \in \mathfrak{V}$, d’où $(U_{II})$. Supposons enfin que $\mathfrak{V}$ ne vérifie pas $(U_{III})$; il existerait alors un ensemble $V \in \mathfrak{V}$ tel que, pour tout $W \in \mathfrak{V}$, l’ensemble $\overline{W}^2 \cap \mathcal{C}V$ soit non vide; les ensembles $\overline{W}^2 \cap \mathcal{C}V$ (où $W$ parcourt $\mathfrak{V}$) formeraient donc une base de filtre sur $X \times X$, et cette dernière aurait par suite un point adhérent $(x, y)$ n’appartenant pas à $Δ$. Or, comme $X$ est régulier (I, p. 61, corollaire, il existerait un voisinage ouvert $U_1$ de $x$ et un voisinage ouvert $U_2$ de $y$ sans point commun, puis des voisinages fermés $V_1 \subset U_1, V_2 \subset U_2$ de $x$ et $y$ respectivement. Posons $U_3 = \mathcal{C}(V_1 \cup V_2)$, et considérons dans $X \times X$ le voisinage

$$
W = \bigcup_{i=1,2,3} (U_i \times U_i)
$$

de $Δ$. Il résulte aussitôt de ces définitions que si $(u, v) \in W$ et $u \in V_1$ (resp. $u \in U_1$), on a nécessairement $v \in U_1$ (resp. $v \in U_1 \cup U_3 = \mathcal{C}V_2$); par suite, le voisinage $V_1 \times V_2$ de $(x, y)$ dans $X \times X$ ne rencontre pas $\overline{W}$; nous avons ainsi obtenu une contradiction, ce qui achève la démonstration.

#### Remarque 1 {#top-ii-s4-n1-rem-1 .statement}

Pour tout recouvrement ouvert fini $\mathfrak{R} = (U_i)_{1 \leq i \leq n}$ de $X$, $V_{\mathfrak{R}} = \bigcup_{i=1}^n (U_i \times U_i)$ est un voisinage de $Δ$ dans $X \times X$; ces ensembles forment un système fondamental de voisinages de $Δ$ (et par suite un système fondamental d’entourages de l’unique structure uniforme de $X$): en effet, soit $W$ un voisinage quelconque de $Δ$ dans $X \times X$; pour tout $x \in X$ il y a un voisinage ouvert $U_x$ de $x$ dans $X$ tel que $U_x \times U_x \subset W$. Comme les $U_x$ ($x \in X$) forment un recouvrement ouvert de $X$, il existe un nombre fini de points $x_i$ ($1 \leq i \leq n$) tels que les $U_{x_i}$ ($1 \leq i \leq n$) forment un recouvrement $\mathfrak{R}$ de $X$; on a alors $V_{\mathfrak{R}} \subset W$, d’où notre assertion.

En raison de ce résultat, on dit souvent que l’unique structure uniforme de $X$ est la structure uniforme des recouvrements ouverts finis (cf. IX, § 4, exerc. 23).

#### Corollaire 1 {#top-ii-s4-thm-1-cor-1 .statement}

Tout sous-espace d’un espace compact est uniformisable.

#### Corollaire 2 {#top-ii-s4-thm-1-cor-2 .statement}

Tout espace localement compact est uniformisable.

Il suffit de remarquer qu’en vertu du th. d’Alexandroff (I, p. 67, th. 4), un espace localement compact est homéomorphe à un sous-espace d’un espace compact.

#### Remarque 2 {#top-ii-s4-n1-rem-2 .statement}

On notera qu’il peut exister plusieurs structures uniformes distinctes compatibles avec la topologie d’un espace localement compact.

Par exemple, nous avons vu que sur un espace discret infini, il y a plusieurs structures uniformes distinctes compatibles avec la topologie discrète (II, p. 7, Remarque 1).

Il ne faudrait pas croire cependant que l’unicité de la structure uniforme compatible avec la topologie d’un espace uniformisable soit une propriété caractérisant les espaces compacts; il y a des espaces localement compacts non compacts qui la possèdent également (II, p. 37, exerc. 4).

#### Théorème 2 {#top-ii-s4-thm-2 .statement}

Toute application continue $f$ d’un espace compact $X$ dans un espace uniforme $X'$ est uniformément continue.

En effet, soit $g = f \times f$, qui est continue dans $X \times X$ (I, p. 25, cor. 1); pour tout entourage ouvert $V'$ de $X'$, $g(V')$ est donc un ensemble ouvert dans $X \times X$, qui contient évidemment la diagonale; le théorème résulte donc du th. 1 (II, p. 27), puisque les entourages ouverts de $X'$ forment un système fondamental d’entourages (II, p. 5, cor. 2).

Sous les hypothèses du th. 2, la restriction de $f$ à tout sous-espace $A$ de $X$ est uniformément continue; donc (II, p. 20, th. 2):

#### Corollaire {#top-ii-s4-n1-cor-1 .statement}

Soient $A$ un sous-espace partout dense d’un espace compact $X$, $f$ une application de $A$ dans un espace uniforme séparé et complet $X'$; pour que $f$ puisse être prolongée par continuité à $X$ tout entier, il faut et il suffit que $f$ soit uniformément continue.

### 2. Compacité des espaces uniformes

#### Définition 2 {#top-ii-s4-def-2 .statement}

On dit qu’un espace uniforme $X$ est précompact si son séparé complété $\hat{X}$ est compact. On dit qu’une partie $A$ d’un espace uniforme $X$ est un ensemble précompact si le sous-espace uniforme $A$ de $X$ est précompact.

Pour qu’une partie $A$ d’un espace uniforme $X$ soit précompacte, il faut et il suffit donc que, si $i : X \to \hat{X}$ est l’application canonique, l’adhérence dans $\hat{X}$ de $i(A)$ soit un ensemble compact (II, p. 26, cor. 1).

#### Exemple {#top-ii-s4-n2-exa-1 .statement}

Dans tout espace uniforme $X$, l’ensemble des points d’une suite de Cauchy $(x_n)$ est précompact: en effet, comme les images des $x_n$ dans $\hat{X}$ forment encore une suite de Cauchy, on peut se borner au cas où $X$ est séparé. L’adhérence dans $\hat{X}$ de l’ensemble des $x_n$ est alors formée des $x_n$ et de $\lim_{n \to \infty} x_n$, donc est compacte (I, p. 61, Exemple 2).

#### Théorème 3 {#top-ii-s4-thm-3 .statement}

Pour qu’un espace uniforme $X$ soit précompact, il faut et il suffit que, pour tout entourage $V$ de $X$, il existe un recouvrement fini de $X$ dont tous les ensembles sont petits d’ordre $V$.

D’une manière plus imagée, on peut exprimer cette condition en disant qu’il existe des recouvrements finis de $X$ dont les ensembles sont aussi petits qu’on veut.

Soit $i$ l’application canonique de $X$ dans $\hat{X}$; les entourages de $X$ sont les images réciproques par $i \times i$ des entourages de $\hat{X}$ (II, p. 23, prop. 12). Pour montrer que la condition de l’énoncé est nécessaire, considérons un entourage arbitraire $U$ de $\hat{X}$, et un entourage symétrique $U'$ de $\hat{X}$ tel que $\overline{U'} \subset U$; comme $\hat{X}$ est compact, il existe un nombre fini de points $x_j \in \hat{X}$ tels que les $U'(x_j)$ (qui sont petits d’ordre $U$) forment un recouvrement de $\hat{X}$; si $V$ est l’image réciproque de $U$ par $i \times i$, les ensembles $\overline{i(U'(x_j))}$ forment donc un recouvrement de $X$ par des ensembles petits d’ordre $V$. Pour voir que la condition est suffisante, il suffit d’établir qu’elle entraîne que tout ultrafiltre $\mathcal{F}$ sur $\hat{X}$ est convergent; comme $\hat{X}$ est complet, il suffit de vérifier que $\mathcal{F}$ est un filtre de Cauchy, ou encore, que pour tout entourage fermé $U$ de $\hat{X}$, il existe dans $\mathcal{F}$ un ensemble petit d’ordre $U$ (II, p. 5, cor. 2). Soit $V$ l’image réciproque de $U$ par $i \times i$, et soit $(B_j)$ un recouvrement fini de $X$ par des ensembles petits d’ordre $V$; les ensembles $C_j = i(B_j)$ forment un recouvrement de $i(X)$ par des ensembles petits d’ordre $U$, donc on a $\hat{X} = \bigcup_j \overline{C_j}$; d’autre part, comme $C_j \times C_j \subset U$ et que $U$ est fermé dans $\hat{X} \times \hat{X}$, on a aussi $\overline{C_j} \times \overline{C_j} \subset U$, autrement dit les $\overline{C_j}$ sont aussi petits d’ordre $U$. Puisque $\mathcal{F}$ est un ultrafiltre, un des $\overline{C_j}$ appartient à $\mathcal{F}$ (I, p. 39, corollaire).

C.Q.F.D.

#### Corollaire {#top-ii-s4-n2-cor-1 .statement}

Pour qu’un espace uniforme $X$ soit compact, il faut et il suffit qu’il soit séparé et complet, et que pour tout entourage $V$ de $X$, il existe un recouvrement fini de $X$ par des ensembles petits d’ordre $V$.

Cela résulte du th. 3 de II, p. 27, th. 1.

#### Remarque 1 {#top-ii-s4-n2-rem-1 .statement}

Un espace quasi-compact non séparé n’est pas nécessairement uniformisable, puisqu’il ne vérifie pas nécessairement l’axiome $(\mathrm{O}_{\mathrm{III}})$ (cf. I, p. 61); par exemple la plupart des espaces quasi-compacts non séparés qui interviennent en Géométrie algébrique ne satisfont pas à $(\mathrm{O}_{\mathrm{III}})$ (cf. II, p. 36, exerc. 2 du § 4).

#### Proposition 1 {#top-ii-s4-prop-1 .statement}

Dans un espace uniforme, toute partie d’un ensemble précompact, toute réunion finie d’ensembles précompacts, toute adhérence d’ensemble précompact, est un ensemble précompact.

Les deux premières assertions découlent aussitôt du th. 3. D’autre part, soient $X$ un espace uniforme, $A$ un ensemble précompact dans $X$, $i$ l’application canonique de $X$ dans son séparé complété $\hat{X}$; $i(\overline{A})$ est contenu dans l’adhérence de $i(A)$ dans $\hat{X}$ (I, p. 9, th. 1), donc l’adhérence de $i(\overline{A})$ dans $\hat{X}$ est contenue par hypothèse dans un ensemble compact, et par suite est compacte.

#### Remarque 2 {#top-ii-s4-n2-rem-2 .statement}

Dans un espace uniforme $X$, un ensemble relativement compact $A$ est précompact, puisque $A$ est contenu dans un ensemble compact. Par contre, même si $X$ est séparé, un ensemble précompact n’est pas nécessairement relativement compact dans $X$, comme le montre le cas où $X$ lui-même est précompact, mais non compact.

#### Proposition 2 {#top-ii-s4-prop-2 .statement}

Soit $f : X \to Y$ une application uniformément continue. Pour toute partie précompacte $A$ de $X$, $f(A)$ est une partie précompacte de $Y$.

En effet, si $i : X \to \hat{X}, j : Y \to \hat{Y}$ sont les applications canoniques, on a $j(f(A)) = \hat{f}(i(A))$ (II, p. 24, prop. 15), donc $j(f(A))$ est relativement compact dans $\hat{Y}$ (I, p. 63, cor. 1).

#### Proposition 3 {#top-ii-s4-prop-3 .statement}

*Soient $X$ un ensemble, $(Y_\lambda)_{\lambda \in L}$ une famille d’espaces uniformes, et pour chaque $\lambda \in L$, soit $f_\lambda$ une application de $X$ dans $Y_\lambda$; on munit $X$ de la structure uniforme la moins fine rendant uniformément continues les $f_\lambda$. Pour qu’une partie $A$ de $X$ soit précompacte, il faut et il suffit que, pour tout $\lambda \in L$, $f_\lambda(A)$ soit une partie précompacte de $Y_\lambda$.*

La condition est nécessaire en vertu de la prop. 2; vu la caractérisation du séparé complété de $X$ (II, p. 26, prop. 18) elle est suffisante en vertu du th. de Tychonoff (I, p. 64, corollaire).

### 3. Ensembles compacts dans un espace uniforme

La proposition suivante précise, dans un espace uniforme quelconque, la prop. 3 de I, p. 61 relative aux espaces compacts.

#### Proposition 4 {#top-ii-s4-prop-4 .statement}

*Dans un espace uniforme $X$, soient $A$ un ensemble compact, $B$ un ensemble fermé tels que $A \cap B = \varnothing$. Il existe alors un entourage $V$ de $X$ tel que $V(A) \cap V(B) = \varnothing$.*

S’il n’en était pas ainsi, aucun des ensembles $A \cap \overline{V}(B)$, où $V$ parcourt l’ensemble des entourages symétriques de $X$, ne serait vide; ces ensembles formeraient donc une base de filtre sur $A$, qui aurait un point adhérent $x_0 \in A$. Pour tout entourage symétrique $V$ de $X$, $\overline{V}(x_0)$ rencontrerait donc $B$, et par suite, comme $B$ est fermé, on aurait $x_0 \in B$, contrairement à l’hypothèse.

#### Corollaire {#top-ii-s4-n3-cor-1 .statement}

*Soit $A$ un ensemble compact dans un espace uniforme $X$; lorsque $V$ parcourt l’ensemble des entourages de $X$, les ensembles $V(A)$ forment un système fondamental de voisinages de $A$.*

En effet, soit $U$ un voisinage ouvert quelconque de $A$; l’ensemble $B = \complement U$ est fermé et ne rencontre pas $A$; d’après la prop. 4, il existe un entourage $V$ tel que $V(A) \cap V(B) = \varnothing$; *a fortiori*, on a $V(A) \subset U$, ce qui démontre le corollaire.

### 4. Ensembles connexes dans un espace compact

#### Définition 3 {#top-ii-s4-def-3 .statement}

*Dans un espace uniforme $X$, soit $V$ un entourage symétrique; on dit qu’une suite finie $(x_i)_{0 \leq i \leq n}$ de points de $X$ est une $V$-chaîne si, pour tout indice $i$ tel que $0 \leq i < n$, $x_i$ et $x_{i+1}$ sont voisins d’ordre $V$; les points $x_0$ et $x_n$ sont appelés les extrémités de la $V$-chaîne, et on dit qu’ils sont joints par la $V$-chaîne.*

Étant donné un entourage symétrique $V$, la relation « il existe une $V$-chaîne joignant $x$ et $y$ » est une relation d’équivalence entre $x$ et $y$ dans $X$, comme on le vérifie aussitôt; soit $A_{x,V}$ la classe d’équivalence de $x$ suivant cette relation, c’est-à-dire l’ensemble des points $y \in X$ pouvant être joints à $x$ par une $V$-chaîne. Il est immédiat que si $y \in A_{x,v}$ on a $V(y) \subset A_{x,v}$, donc $A_{x,v}$ est ouvert; mais son complémentaire, qui est réunion de classes d’équivalence, est aussi ouvert. Donc:

#### Proposition 5 {#top-ii-s4-prop-5 .statement}

*Dans un espace uniforme $X$, l’ensemble $A_{x,v}$ des points qui peuvent être joints à un point donné $x$ par une $V$-chaîne, est à la fois ouvert et fermé.*

Pour tout $x \in X$, désignons par $A_x$ l’intersection des ensembles $A_{x,v}$ lorsque $V$ parcourt l’ensemble des entourages symétriques de $X$; c’est la classe d’équivalence de $x$ suivant la relation d’équivalence: « quel que soit l’entourage symétrique $V$, il existe une $V$-chaîne joignant $x$ et $y$ ».

#### Proposition 6 {#top-ii-s4-prop-6 .statement}

*Dans un espace compact $X$, la composante connexe d’un point $x$, l’ensemble $A_x$ et l’intersection des voisinages de $x$ à la fois ouverts et fermés sont identiques.*

Il suffit de montrer que $A_x$ est *connexe*; en effet, dans tout espace uniforme $X$, la composante connexe de $x$ est contenue dans l’intersection des voisinages à la fois ouverts et fermés de $X$, et cette intersection est elle-même contenue dans $A_x$ en vertu de la prop. 5.

Supposons que $A_x$ ne soit pas connexe; comme c’est un ensemble *fermé*, il existerait deux ensembles *fermés* non vides et sans point commun, $B$ et $C$, tels que $B \cup C = A_x$. D’après la prop. 4 (II, p. 31) il existerait alors un entourage $U$ de $X$ tel que $U(B) \cap U(C) = \varnothing$; soit $W$ un entourage *ouvert* tel que $W^2 \subset U$, et désignons par $H$ l’ensemble *fermé* complémentaire dans $X$ de l’ensemble $W(B) \cup W(C)$. Supposons par exemple que $x \in B$, et considérons un point $y \in C$; pour tout entourage symétrique $V \subset W$, on voit aussitôt, par récurrence sur $i$, que toute $V$-chaîne $(x_i)_{0 \leq i \leq n}$ joignant $x$ et $y$ dans $X$ a nécessairement un point dans $H$, en vertu du choix de $W$. Comme par hypothèse $x$ et $y$ peuvent être joints par une $V$-chaîne pour tout entourage symétrique $V$, on voit que, pour $V \subset W$, l’ensemble $H \cap A_{x,v}$ n’est pas vide. D’autre part, si $V' \subset V$, on a évidemment $A_{x,v'} \subset A_{x,v}$; il en résulte que lorsque $V$ parcourt l’ensemble des entourages symétriques de $X$, les ensembles $H \cap A_{x,v}$ formeraient une base de filtre composée d’ensembles *fermés* dans l’espace compact $H$. Il existerait donc un point commun à tous ces ensembles, autrement dit un point commun à $H$ et $A_x$; comme cela est contraire à la définition de $H$, la proposition est démontrée.

#### Corollaire {#top-ii-s4-n4-cor-1 .statement}

*Soient $X$ un espace localement compact, $K$ une composante connexe compacte de $X$. Alors les voisinages à la fois ouverts et fermés de $K$ forment un système fondamental de voisinages de $K$*.

En effet, soit $V$ un voisinage ouvert relativement compact de $K$ dans $X$ (I, p. 65, prop. 10), et soit $F$ sa frontière. Soit $U \subset \overline{V}$ un ensemble à la fois ouvert et fermé *par rapport à $\overline{V}$*; alors $U$ est fermé dans $X$, et si en outre $U$ ne rencontre pas $F$, $U$ est ouvert dans $X$, car cela entraîne $U \subset V$ et $U$ est ouvert par rapport à $V$. Tout revient donc à montrer qu’il existe dans $\overline{V}$ un ensemble contenant $K$, à la fois ouvert et fermé par rapport à $\overline{V}$, et qui ne rencontre pas $F$.

Raisonnons par l’absurde: les intersections avec $F$ des ensembles contenant

K et à la fois ouverts et fermés par rapport à $\overline{V}$ formeraient une base de filtre composée d’ensembles fermés dans F; comme F est compact, ces ensembles auraient un point commun $y \in F$; mais cela est absurde, car $\overline{V}$ est un espace compact, K est une composante connexe de cet espace, et en vertu de la prop. 6, l’intersection des ensembles contenant K et à la fois ouverts et fermés dans $\overline{V}$ se réduit à K. Le corollaire est donc démontré.

#### Proposition 7 {#top-ii-s4-prop-7 .statement}

Soient X un espace compact, R la relation d’équivalence dans X dont les classes sont les composantes connexes de X. L’espace quotient X/R est compact et totalement discontinu.

On sait déjà (I, p. 84, prop. 9) que X/R est totalement discontinu; tout revient à voir que X/R est séparé (I, p. 78, prop. 8). Soient A et B deux composantes connexes distinctes de X; en vertu de la prop. 6 (II, p. 32), il existe un entourage symétrique U de X tel qu’un point quelconque de A et un point quelconque de B ne puissent être joints par une U-chaîne. Or, l’ensemble V (resp. W) des points de X qui peuvent être joints à un point $x \in A$ (resp. $y \in B$) par une U-chaîne est à la fois ouvert et fermé dans X (II, p. 32, prop. 5) et contient A (resp. B); ces ensembles sont donc des voisinages ouverts de A et B respectivement, saturés pour R et ne se rencontrant pas, ce qui démontre la proposition.

Exercises

## EXERCICES {#top-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
