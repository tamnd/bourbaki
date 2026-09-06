---
book: top
book_title: General Topology
chapter: II
chapter_title: STRUCTURES UNIFORMES
section: 1
section_title: Espaces uniformes
lang: fr
source: top-i-iv-fr
pdf_pages: 0140-0145, 0173-0174
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une structure uniforme
      page: 0
      pdf_page: 140
    - "no": 2
      title: Topologie d’un espace uniforme
      page: 3
      pdf_page: 142
statements: 14
exercises: 5
content_sha256: 6288b483aef86cdb0dac40f4076086ed2473b9ef34afd6ac94d9e5de7de025f4
---

## § 1. ESPACES UNIFORMES

### 1. Définition d’une structure uniforme

#### Définition 1 {#top-ii-s1-def-1 .statement}

On appelle structure uniforme sur un ensemble $X$ une structure constituée par la donnée d’un ensemble $\mathcal{U}$ de parties de $X \times X$ qui satisfait aux axiomes $(F_I)$ et $(F_{II})$ de I, p. 36, et aux axiomes suivants :

$(U_I)$ Tout ensemble de $\mathcal{U}$ contient la diagonale $\Delta$ (fig. 1).

$(U_{II})$ La relation $V \in \mathcal{U}$ entraîne $\overline{V} \in \mathcal{U}$.

$(U_{III})$ Quel que soit $V \in \mathcal{U}$, il existe $W \in \mathcal{U}$ tel que $W \circ W \subset V$.

![Figure 1](../images/figure_1.png)

On dit que les ensembles de $\mathcal{U}$ sont les entourages de la structure uniforme définie sur $X$ par $\mathcal{U}$.

On appelle espace uniforme un ensemble muni d’une structure uniforme.

Si V est un entourage d’une structure uniforme sur X, on exprimera la relation $(x, x') \in V$ en disant que « x et $x'$ sont voisins d’ordre V ».

#### Remarque 1 {#top-ii-s1-n1-rem-1 .statement}

Pour rendre le langage plus imagé, on pourra employer les expressions « x et y sont assez voisins » et « x et y sont aussi voisins qu’on veut » dans certains énoncés. Par exemple, on dira qu’une relation R $\{x, y\}$ est vérifiée si x et y sont assez voisins, lorsqu’il existe un entourage V tel que la relation $(x, y) \in V$ entraîne R $\{x, y\}$.

#### Remarque 2 {#top-ii-s1-n1-rem-2 .statement}

La conjonction des axiomes (U_{II}) et (U_{III}) est (compte tenu des autres axiomes des structures uniformes) équivalente à l’axiome:

(U_a) Quel que soit $V \in \mathcal{U}$, il existe $W \in \mathcal{U}$ tel que $W \circ \overline{W}^1 \subset V$.\footnote{Rappelons (E, II, p. 11) que si V et W sont deux parties de $X \times X$, l’ensemble noté $V \circ W$ ou VW est l’ensemble des couples $(x, y) \in X \times X$ ayant la propriété qu’il existe $z \in X$ tel que l’on ait $(x, z) \in W$ et $(z, y) \in V$; l’ensemble $\overline{V}^1$ est l’ensemble des couples $(x, y) \in X \times X$ tels que $(y, x) \in V$.}

Il est clair en effet que (U_{II}) et (U_{III}) entraînent (U_a). Inversement, si (U_a) est vérifiée, on a $\overline{W}^1 = \Delta \circ \overline{W}^1 \subset V$ d’après (U_I); donc $W \subset \overline{V}^1$, ce qui montre (compte tenu de (F_I)) que $\overline{V} \in \mathcal{U}$; d’autre part, si l’on pose $W' = W \cap \overline{W}^1$, on a $W' \in \mathcal{U}$ d’après ce qui précède et (F_{II}) et on a $W' \circ W' \subset W \circ \overline{W}^1 \subset V$.

Dans toute la suite de ce chapitre, on écrira $\overline{V}^2$ au lieu de $V \circ V$, et on posera, en général, $V^n = V \circ V = V \circ V^{n-1}$ pour tout entier $n > 1$ et toute partie V de $X \times X$.

#### Remarque 3 {#top-ii-s1-n1-rem-3 .statement}

Si X est non vide, l’axiome (U_I) entraîne qu’aucun ensemble de $\mathcal{U}$ n’est vide, donc que $\mathcal{U}$ est un filtre sur $X \times X$. Sur l’ensemble vide, il n’y a qu’une seule structure uniforme, ayant pour ensemble d’entourages $\mathcal{U} = \{ \varnothing \}$.

#### Définition 2 {#top-ii-s1-def-2 .statement}

On appelle système fondamental d’entourages d’une structure uniforme tout ensemble $\mathcal{B}$ d’entourages tel que tout entourage contienne un ensemble appartenant à $\mathcal{B}$.

L’axiome (U_{III}) montre que, si $n$ est un entier quelconque $> 0$, les ensembles $V^n$, où V parcourt un système fondamental d’entourages, forment encore un système fondamental d’entourages.

Appelons entourages symétriques les entourages V d’une structure uniforme tels que $V = \overline{V}^1$; pour tout entourage V, $V \cap \overline{V}^1$ et $V \cup \overline{V}^1$ sont des entourages symétriques; les axiomes (F_{II}) et (U_{II}) montrent que les entourages symétriques forment un système fondamental d’entourages.

Pour qu’un ensemble $\mathcal{B}$ de parties de $X \times X$ soit un système fondamental d’entourages d’une structure uniforme sur X, il faut et il suffit qu’il satisfasse à l’axiome (B_I) de I, p. 38, et aux axiomes suivants:

(U'_I) Tout ensemble de $\mathcal{B}$ contient la diagonale $\Delta$.

(U'_{II}) Quel que soit $V \in \mathcal{B}$, il existe $V' \in \mathcal{B}$ tel que $V' \subset \overline{V}^1$.

(U'_{III}) Quel que soit $V \in \mathcal{B}$, il existe $W \in \mathcal{B}$ tel que $\overline{W}^2 \subset V$.

Si X est non vide, un système fondamental d’entourages d’une structure uniforme sur X est une base du filtre des entourages de cette structure (I, p. 38, prop. 3).

Exemples de structures uniformes. —*1) Sur l’ensemble des nombres réels R, on définit de la manière suivante une structure uniforme, dite structure uniforme additive: pour chaque $\alpha > 0$, on considère, dans $\mathbf{R} \times \mathbf{R}$, l’ensemble $V_\alpha$ des couples $(x, y)$ de nombres réels tels que $|x - y| < \alpha$; lorsque $\alpha$ parcourt l’ensemble des nombres réels $> 0$, les $V_\alpha$ constituent un système fondamental d’entourages de la structure uniforme additive sur $\mathbf{R}$. On définit de la même manière une structure uniforme (dite encore structure additive) sur l’ensemble $\mathbf{Q}$ des nombres rationnels; on étudiera aux chap. III et IV ces structures, et les structures uniformes que l’on peut définir de façon analogue sur les groupes.*

2) Soient X un ensemble, R une relation d’équivalence dans X, C son graphe dans $X \times X$. On sait (E, II, p. 41) que l’on a $\Delta \subset C$ et $\overline{C} = \overline{\overline{C}} = C$; l’ensemble de parties de $X \times X$ réduit au seul ensemble C est donc un système fondamental d’entourages d’une structure uniforme sur X. En particulier, si on prend pour R la relation d’égalité, on a $C = \Delta$, et les entourages de la structure uniforme correspondante sont alors toutes les parties de $X \times X$ contenant $\Delta$; on dit que cette structure uniforme est la structure uniforme discrète sur X et l’ensemble X, muni de cette structure uniforme, est appelé espace uniforme discret.

3) Sur l’ensemble $\mathbf{Z}$ des entiers rationnels, on définit de la manière suivante une structure uniforme importante en Théorie des Nombres: étant donné un nombre premier $p$, on considère, pour chaque entier $n > 0$, l’ensemble $W_n$ des couples $(x, y) \in \mathbf{Z} \times \mathbf{Z}$ tels que $x \equiv y \pmod{p^n}$. On vérifie aisément que ces ensembles constituent un système fondamental d’entourages d’une structure uniforme sur $\mathbf{Z}$, dite structure $p$-adique (III, p. 82, exerc. 23 et suiv., et IX, §3, n°2).

Conformément aux définitions générales (E, IV, p. 6), si X et X’ sont deux ensembles munis de structures uniformes dont les ensembles d’entourages sont respectivement $\mathcal{U}$ et $\mathcal{U}'$, une bijection f de X sur X’ est un isomorphisme de la structure uniforme de X sur celle de X’ si, en posant $g = f \times f$, on a $g(\mathcal{U}) = \mathcal{U}'$.

Par exemple, si X et X’ sont deux ensembles équipotents, toute bijection de X sur X’ est un isomorphisme de la structure uniforme discrète de X sur la structure uniforme discrète de X’.

### 2. Topologie d’un espace uniforme

#### Proposition 1 {#top-ii-s1-prop-1 .statement}

Soit X un ensemble muni d’une structure uniforme $\mathcal{U}$. Pour tout $x \in X$, soit $\mathfrak{V}(x)$ l’ensemble des parties $V(x)$ de X, où V parcourt l’ensemble des entourages de $\mathcal{U}$; il existe sur X une topologie et une seule telle que pour tout $x \in X$, $\mathfrak{V}(x)$ soit le filtre des voisinages de x pour cette topologie.

Il faut montrer que les $\mathfrak{V}(x)$ vérifient les conditions (V_I), (V_{II}), (V_{III}) et (V_{IV}) de I, p. 3. Pour les trois premières, cela résulte aussitôt de ce que l’ensemble des entourages de $\mathcal{U}$ vérifie (F_I), (F_{II}) et (U_I). D’autre part, si V est un entourage de $\mathcal{U}$, W un entourage de $\mathcal{U}$ tel que $\overset{2}{W} \subset V$, $V(x)$ appartient à $\mathfrak{V}(y)$ pour tout $y \in W(x)$; en effet, si $(x, y) \in W$ et $(y, z) \in W$, on a $(x, z) \in \overset{2}{W} \subset V$, donc $W(y) \subset V(x)$ pour tout $y \in W(x)$, ce qui achève la démonstration.

#### Définition 3 {#top-ii-s1-def-3 .statement}

On dit que la topologie définie dans la prop. 1 est la topologie déduite de la structure uniforme $\mathcal{U}$.

#### Exemple 1 {#top-ii-s1-n2-exa-1 .statement}

La topologie déduite de la structure uniforme additive sur l’ensemble des nombres réels est la topologie de la droite numérique (I, p. 4); de même, la topologie déduite de la structure additive sur l’ensemble des nombres rationnels est la topologie de la droite rationnelle.*

#### Exemple 2 {#top-ii-s1-n2-exa-2 .statement}

Sur un ensemble quelconque X, la topologie déduite de la structure uniforme discrète (II, p. 3, Exemple 2) est la topologie discrète.

Quand nous parlerons, par la suite, de la topologie d’un espace uniforme X, il faudra toujours entendre, sauf mention expresse du contraire, la topologie déduite de la structure uniforme de cet espace; l’espace topologique obtenu en munissant l’ensemble X de cette topologie sera parfois appelé l’espace topologique sous-jacent à l’espace uniforme considéré. Par exemple, quand nous dirons qu’un espace uniforme est séparé, ou compact, ou localement compact, etc., cela signifiera que l’espace sous-jacent a cette propriété.

Étant donnés deux espaces uniformes X, X’, tout isomorphisme $f$ de la structure uniforme de X sur celle de X’ est aussi un homéomorphisme de X sur X’; on dit que $f$ est un isomorphisme de l’espace uniforme X sur l’espace uniforme X’. On notera qu’un homéomorphisme de X sur X’ n’est pas nécessairement un isomorphisme de la structure uniforme de X sur celle de X’.

En d’autres termes, les topologies déduites de deux structures uniformes distinctes sur un même ensemble X peuvent être identiques. *Par exemple, sur ]0, +∞[, la même topologie est déduite de la structure uniforme additive et de la structure uniforme multiplicative, qui sont distinctes (III, p. 80, exerc. 17).*
Pour un autre exemple, voir II, p. 7, Remarque 1.

#### Proposition 2 {#top-ii-s1-prop-2 .statement}

Soit X un espace uniforme. Pour tout entourage symétrique V de X et toute partie M de $X \times X$, VMV est un voisinage de M dans l’espace topologique produit $X \times X$, et l’adhérence de M dans cet espace est donnée par la formule

$$
\overline{M} = \bigcap_{V \in \mathfrak{S}} VMV,
$$

$\mathfrak{S}$ désignant l’ensemble des entourages symétriques de X.

En effet, si V est un entourage symétrique de X, la relation $(x, y) \in VMV$ signifie qu’il existe $(p, q) \in M$ tel que $(x, p) \in V$ et $(q, y) \in V$, autrement dit (V étant symétrique), $x \in V(p)$ et $y \in V(q)$, ou encore $(x, y) \in V(p) \times V(q)$. Comme $V(p) \times V(q)$ est un voisinage de $(p, q)$ dans $X \times X$, cela démontre la première assertion. En outre, les relations $(x, p) \in V, (y, q) \in V$ s’écrivent aussi $p \in V(x)$, $q \in V(y)$, ou encore $(p, q) \in V(x) \times V(y)$. Or, lorsque V parcourt $\mathfrak{S}$, les ensembles $V(x) \times V(y)$ constituent un système fondamental de voisinages de $(x, y)$ dans $X \times X$: en effet, si U, U’ sont deux entourages quelconques, il y a toujours un entourage symétrique $V \subset U \cap U'$, donc

$$
V(x) \times V(y) \subset U(x) \times U'(y).
$$

Dire que $V(x) \times V(y)$ rencontre $M$ pour tout $V \in \mathcal{S}$ signifie donc que $(x, y) \in \overline{M}$, d’où la formule (1).

#### Corollaire 1 {#top-ii-s1-prop-2-cor-1 .statement}

*Pour toute partie A de X et tout entourage symétrique V de X, V(A) est un voisinage de A dans X, et l’on a*

$$
\overline{A} = \bigcap_{V \in \mathcal{S}} V(A) = \bigcap_{V \in \mathfrak{U}} V(A)
$$

(* désignant l’ensemble des entourages de X).

En effet, si on pose $M = A \times A$, on a $VMV = V(A) \times V(A)$ pour $V \in \mathcal{S}$, car la relation « il existe $p \in A$ tel que $(x, p) \in V$ » équivaut à $x \in V(A)$ par définition. On en conclut le corollaire, en vertu de I, p. 26, prop. 5 et I, p. 27, prop. 7.

On dit que $V(A)$ est le *voisinage d’ordre* $V$ de $A$.

Si $V$ est un entourage de $X$ *ouvert* dans $X \times X$, $V(x)$ est ouvert dans $X$ pour tout $x \in X$ (I, p. 26, cor. de la prop. 2), donc $V(A)$, réunion des $V(x)$ pour $x \in A$, est *ouvert* dans $X$. Par contre, si $V$ est un entourage fermé dans $X \times X$, $V(A)$ n’est pas nécessairement fermé dans $X$ pour toute partie $A$ de $X$ (II, p. 34, exerc. 3).

D’autre part, il convient de remarquer que, lorsque $V$ parcourt l’ensemble des entourages de $X$, les ensembles $V(A)$ ne forment pas nécessairement un système fondamental de voisinages de $A$ dans $X$ (II, p. 34, exerc. 2).

#### Corollaire 2 {#top-ii-s1-prop-2-cor-2 .statement}

*Les intérieurs (resp. les adhérences) dans $X \times X$ des entourages de X forment un système fondamental d’entourages de X*.

En effet, si $V$ est un entourage quelconque de $X$, il existe un entourage symétrique $W$ tel que $\overset{3}{W} \subset V$; comme $\overset{3}{W}$ est un voisinage de $W$ (prop. 2), l’intérieur de $V$ dans $X \times X$ contient $W$ et est donc un entourage de $X$. En outre (prop. 2), on a $W \subset \overline{W} \subset \overset{3}{W} \subset V$, donc $V$ contient l’adhérence d’un entourage de $X$.

#### Corollaire 3 {#top-ii-s1-prop-2-cor-3 .statement}

*Tout espace uniforme vérifie l’axiome* ($O_{III}$).

En effet, pour tout $x \in X$, si $V$ parcourt l’ensemble des entourages de $X$ fermés dans $X \times X$, les $V(x)$ forment un système fondamental de voisinages de $x$ dans $X$ en vertu du cor. 2, et les $V(x)$ sont fermés dans $X$ (I, p. 26, cor. de la prop. 4).

#### Proposition 3 {#top-ii-s1-prop-3 .statement}

*Pour qu’un espace uniforme X soit séparé, il faut et il suffit que l’intersection des entourages de sa structure uniforme soit la diagonale $\Delta$ de $X \times X$. Tout espace uniforme séparé est régulier*.

La dernière assertion résulte aussitôt du cor. 3 de la prop. 2. On a vu que les entourages fermés forment un système fondamental d’entourages de $X$ (cor. 2 de la prop. 2); si leur intersection est égale à $\Delta$, $\Delta$ est fermé dans $X \times X$, donc $X$ est séparé (I, p. 52, prop. 1). Inversement, si $X$ est séparé, pour tout point $(x, y)$ n’appartenant pas à $\Delta$, il existe un entourage $V$ de $X$ tel que $y \notin V(x)$, ce qu’équivaut à $(x, y) \notin V$; donc $\Delta$ est l’intersection des entourages de $X$.

Lorsqu’un espace uniforme X est séparé, on dit que sa structure uniforme est séparée. Soit $\mathfrak{B}$ un système fondamental d’entourages de cette structure; pour que X soit séparé, il faut et il suffit que l’intersection des ensembles de $\mathfrak{B}$ soit $\Delta$.

## EXERCICES {#top-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
