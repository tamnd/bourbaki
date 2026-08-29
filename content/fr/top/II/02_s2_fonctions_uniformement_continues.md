---
book: top
book_title: General Topology
chapter: II
chapter_title: STRUCTURES UNIFORMES
section: 2
section_title: Fonctions uniformément continues
lang: fr
source: top-i-iv-fr
book_pages: TG II.6-TG II.12, TG II.35
pdf_pages: 0145-0151, 0174-0174
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions uniformément continues
      page: 6
      pdf_page: 145
    - "no": 2
      title: Comparaison des structures uniformes
      page: 6
      pdf_page: 145
    - "no": 3
      title: Structures uniformes initiales
      page: 8
      pdf_page: 147
    - "no": 4
      title: Image réciproque d’une structure uniforme. Sous-espaces uniformes
      page: 9
      pdf_page: 148
    - "no": 5
      title: Borne supérieure d’un ensemble de structures uniformes
      page: 10
      pdf_page: 149
    - "no": 6
      title: Produit d’espaces uniformes
      page: 10
      pdf_page: 149
    - "no": 7
      title: Limites projectives d’espaces uniformes
      page: 12
      pdf_page: 151
statements: 24
exercises: 6
content_sha256: bfb04ecdf1f9360e7000738526e7648065d67c1912d1d3570bfd26485e9fc429
---

## § 2. FONCTIONS UNIFORMÉMENT CONTINUES

### 1. Fonctions uniformément continues

#### Définition 1 {#top-ii-s2-def-1 .statement}

On dit qu’une application $f$ d’un espace uniforme X dans un espace uniforme $X'$ est uniformément continue si, pour tout entourage $V'$ de $X'$, il existe un entourage $V$ de X tel que la relation $(x, y) \in V$ entraîne $(f(x), f(y)) \in V'$.

D’une manière plus imagée, on peut dire que $f$ est uniformément continue si $f(x)$ et $f(y)$ sont aussi voisins qu’on veut dès que $x$ et $y$ sont assez voisins.

Si on pose $g = f \times f$, la déf. 1 signifie encore que pour tout entourage $V'$ de $X'$, $g^{-1}(V')$ est un entourage de X.

#### Exemple 1 {#top-ii-s2-n1-exa-1 .statement}

L’application identique d’un espace uniforme sur lui-même est uniformément continue.
2) Une application constante d’un espace uniforme dans un espace uniforme est uniformément continue.
3) Toute application d’un espace uniforme discret dans un espace uniforme est uniformément continue.

#### Proposition 1 {#top-ii-s2-prop-1 .statement}

Toute application uniformément continue est continue.

C’est une conséquence immédiate des définitions.

Par contre, une application continue d’un espace uniforme X dans un espace uniforme $X'$ n’est pas nécessairement uniformément continue, *comme le montre l’exemple $x \mapsto x^3$, homéomorphisme de $\mathbf{R}$ sur lui-même, qui n’est pas uniformément continue pour la structure uniforme additive.* (Voir II, p. 29, th. 2.)

#### Proposition 2 {#top-ii-s2-prop-2 .statement}

1° Si $f : X \to X'$ et $g : X' \to X''$ sont deux applications uniformément continues, alors $g \circ f : X \to X''$ est uniformément continue.
2° Pour qu’une bijection $f$ d’un espace uniforme X sur un espace uniforme $X'$ soit un isomorphisme, il faut et il suffit que $f$ et la bijection réciproque $g$ de $f$ soient uniformément continues.

Cela résulte immédiatement de l’interprétation de la déf. 1 en termes de l’application produit $f \times f$.

### 2. Comparaison des structures uniformes

La prop. 2 montre que l’on peut prendre pour morphismes des structures uniformes les applications uniformément continues (E, IV, p. 11); nous supposerons toujours par la suite que l’on a fait ce choix de morphismes. Conformément aux définitions générales (E, IV, p. 13), cela permet de définir une relation d’ordre dans l’ensemble des structures uniformes sur un même ensemble X:

#### Définition 2 {#top-ii-s2-def-2 .statement}

Étant données deux structures uniformes $\mathcal{U}_1, \mathcal{U}_2$ sur un même ensemble X, on dit que $\mathcal{U}_1$ est plus fine que $\mathcal{U}_2$ (et que $\mathcal{U}_2$ est moins fine que $\mathcal{U}_1$) si, en désignant par $X_i$ l’ensemble X muni de la structure uniforme $\mathcal{U}_i$ ($i = 1, 2$) l’application identique $X_1 \to X_2$ est uniformément continue.

Si $\mathcal{U}_1$ est plus fine que $\mathcal{U}_2$ et distincte de $\mathcal{U}_2$, on dit que $\mathcal{U}_1$ est strictement plus fine que $\mathcal{U}_2$ (et que $\mathcal{U}_2$ est strictement moins fine que $\mathcal{U}_1$).

Deux structures uniformes dont l’une est plus fine que l’autre sont dites comparables.

#### Exemple {#top-ii-s2-n2-exa-1 .statement}

Dans l’ensemble ordonné des structures uniformes sur un ensemble X, la structure uniforme discrète est la structure uniforme la plus fine, et la structure uniforme la moins fine est celle dont l’ensemble des entourages est formé du seul élément $X \times X$.

La déf. 1 de II, p. 6 entraîne aussitôt la proposition suivante:
Proposition 3. — Étant données deux structures uniformes $\mathcal{U}_1, \mathcal{U}_2$ sur un ensemble X, pour que $\mathcal{U}_1$ soit plus fine que $\mathcal{U}_2$, il faut et il suffit que tout entourage de $\mathcal{U}_2$ soit un entourage de $\mathcal{U}_1$.

#### Corollaire {#top-ii-s2-n2-cor-1 .statement}

Sur un ensemble X, soit $\mathcal{U}_1$ une structure uniforme plus fine qu’une structure uniforme $\mathcal{U}_2$; alors la topologie déduite de $\mathcal{U}_1$ est plus fine que la topologie déduite de $\mathcal{U}_2$.

Cela résulte aussitôt de la comparaison des topologies à l’aide des voisinages (I, p. 11, prop. 3).

#### Remarque 1 {#top-ii-s2-n2-rem-1 .statement}

Il peut se faire qu’une structure uniforme $\mathcal{U}_1$ soit strictement plus fine qu’une structure uniforme $\mathcal{U}_2$, mais que les topologies déduites de ces deux structures uniformes soient identiques. C’est ce que montre l’exemple suivant:
Soit X un ensemble non vide; pour toute partition finie $\varpi = (A_i)_{1 \leq i \leq n}$ de X, posons $V_{\varpi} = \bigcup_i (A_i \times A_i)$; les ensembles $V_{\varpi}$ constituent un système fondamental d’entourages d’une structure uniforme $\mathcal{U}$ sur X; en effet pour toute partition finie $\varpi$, on a $\Delta \subset V_{\varpi}$ et $V_{\varpi} \circ V_{\varpi} = \overline{V}_{\varpi} = V_{\varpi}$ (II, p. 3, Exemple 2); d’autre part, si $\varpi' = (B_j)$ et $\varpi'' = (C_k)$ sont deux partitions finies de X, ceux des ensembles $B_j \cap C_k$ qui sont non vides forment une partition $\varpi$ de X, et l’on a $V_{\varpi} \subset V_{\varpi'} \cap V_{\varpi''}$. On dit que $\mathcal{U}$ est la structure uniforme des partitions finies sur X. La topologie déduite de $\mathcal{U}$ est la topologie discrète, car pour tout $x \in X$ les ensembles $\{x\}$ et $\mathcal{C}\{x\}$ forment une partition finie de X. Cependant, si X est infini, il est clair que $\mathcal{U}$ est strictement moins fine que la structure uniforme discrète.

#### Remarque 2 {#top-ii-s2-n2-rem-2 .statement}

Si $f : X \to X'$ est une application uniformément continue, elle reste uniformément continue lorsqu’on remplace la structure uniforme de X par une structure uniforme plus fine et celle de $X'$ par une structure uniforme moins fine (II, p. 6, prop. 2). Autrement dit, il y a d’autant plus d’applications uniformément continues de X dans X' que la structure uniforme de X est plus fine et celle de X' moins fine.

### 3. Structures uniformes initiales

#### Proposition 4 {#top-ii-s2-prop-4 .statement}

Soient X un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces uniformes, et pour chaque $i \in I$, soit $f_i$ une application de X dans $Y_i$; pour tout $i \in I$, on pose $g_i = f_i \times f_i$.

Soit $G$ l’ensemble des parties de $X \times X$ de la forme $g_i^{-1}(V_i)$ ($i \in I$, $V_i$ entourage de $Y_i$), et soit $B$ l’ensemble des intersections finies

$$
U(V_{i_1}, \ldots, V_{i_n}) = g_{i_1}^{-1}(V_{i_1}) \cap \cdots \cap g_{i_n}^{-1}(V_{i_n})
$$

d’ensembles de $G$. Alors $B$ est un système fondamental d’entourages d’une structure uniforme $U$ sur X qui est la structure uniforme initiale sur X pour la famille $(f_i)$ (E, IV, p. 14) et en particulier est la moins fine sur X rendant uniformément continues les applications $f_i$. En d’autres termes, soit h une application d’un espace uniforme Z dans X. Pour que h soit uniformément continue (lorsque X est muni de la structure uniforme U), il faut et il suffit que chacune des fonctions $f_i \circ h$ soit uniformément continue.

Il est immédiat que B vérifie les axiomes (B_I) et (U'_I); si $W_i = g_i^{-1}(V_i)$, on a $W_i^{-1} = g_i^{-1}(V_i)$ et $W_i^2 \subset g_i^{-1}(V_i)^2$, donc B vérifie aussi (U''_II) et (U'''_III) et est par suite un système fondamental d’entourages d’une structure uniforme U sur X. En outre, il résulte aussitôt de la définition de U et de la déf. 1 de II, p. 6 que $f_i$ est uniformément continue pour tout $i \in I$; donc (II, p. 6, prop. 2) $f_i \circ h$ est uniformément continue pour tout $i \in I$ si h l’est. Inversement, supposons que pour tout $i \in I$, $f_i \circ h$ soit uniformément continue et considérons un ensemble $U(V_{i_1}, \ldots, V_{i_n})$; par hypothèse, pour $1 \leq k \leq n$, il existe un entourage $W_k$ de Z tel que la relation $(z, z') \in W_k$ entraîne $(f_{i_k}(h(z)), f_{i_k}(h(z')))) \in V_k$; si $W = \bigcap_k W_k$, les n relations précédentes sont simultanément vérifiées lorsque z et $z'$ sont voisins d’ordre W, ce qui prouve qu’on a alors

$$(h(z), h(z')) \in U(V_{i_1}, \ldots, V_{i_n}),$$

et achève la démonstration.

#### Corollaire {#top-ii-s2-n3-cor-1 .statement}

La topologie sur X déduite de la structure uniforme la moins fine rendant uniformément continues les $f_i$ est la topologie la moins fine rendant continues les $f_i$.

Cela résulte aussitôt de la définition des voisinages d’un point pour cette dernière topologie (I, p. 12, prop. 4).

Les propriétés générales des structures initiales (E, IV, p. 14, critère CST 10) entraînent en particulier la propriété suivante de transitivité:

#### Proposition 5 {#top-ii-s2-prop-5 .statement}

Soient X un ensemble, $(Z_i)_{i \in I}$ une famille d’espaces uniformes, $(J_\lambda)_{\lambda \in L}$ une partition de I et $(Y_\lambda)_{\lambda \in L}$ une famille d’ensembles ayant L pour ensemble d’indices. Enfin, pour tout $\lambda \in L$, soit $h_\lambda$ une application de $X$ dans $Y_\lambda$; pour tout $\lambda \in L$ et tout $i \in J_\lambda$, soit $g_{i\lambda}$ une application de $Y_\lambda$ dans $Z_i$; on pose alors $f_i = g_{i\lambda} \circ h_\lambda$. On munit chacun des $Y_\lambda$ da la structure uniforme la moins fine rendant uniformément continues les $g_{i\lambda}$ ($i \in J_\lambda$); alors, sur $X$, la structure uniforme la moins fine rendant uniformément continues les $f_i$ est identique à la structure uniforme la moins fine rendant uniformément continues les $h_\lambda$.

### 4. Image réciproque d’une structure uniforme. Sous-espaces uniformes

Soient $X$ un ensemble, $Y$ un espace uniforme, $f$ une application de $X$ dans $Y$; la structure uniforme la moins fine $\mathcal{U}$ sur $X$ rendant uniformément continue $f$ est appelée l’image réciproque par $f$ de la structure uniforme de $Y$. Il résulte de la prop. 4 de II, p. 8 et des formules donnant l’image réciproque d’une intersection que les images réciproques par $g = f \times f$ des entourages de $Y$ forment déjà un système fondamental d’entourages pour $\mathcal{U}$. La topologie déduite de $\mathcal{U}$ est alors l’image réciproque par $f$ de la topologie de $Y$ (II, p. 8, corollaire).

#### Remarque {#top-ii-s2-n4-rem-1 .statement}

Si $f : X \to Y$ est surjective, les entourages de $Y$ sont alors les images directes par $g$ des entourages de $X$.

Pour qu’une application $f$ d’un espace uniforme $X$ dans un espace uniforme $X'$ soit uniformément continue, il faut et il suffit que l’image réciproque par $f$ de la structure uniforme de $X'$ soit moins fine que la structure uniforme de $X$.

Soit $A$ une partie d’un espace uniforme $X$; la structure uniforme induite sur $A$ par la structure uniforme de $X$ est l’image réciproque de cette dernière par l’injection canonique $A \to X$; il revient au même (II, p. 8, prop. 4) de poser la définition suivante:

#### Définition 3 {#top-ii-s2-def-3 .statement}

Soit $A$ une partie d’un espace uniforme $X$. On appelle structure uniforme induite sur $A$ par la structure uniforme de $X$ la structure uniforme dont l’ensemble des entourages est la trace sur $A \times A$ de l’ensemble des entourages de $X$.

La topologie déduite de la structure uniforme induite sur $A$ est la topologie induite sur $A$ par celle de $X$; $A$, muni de la structure uniforme et de la topologie induites par celles de $X$, est appelé sous-espace uniforme de $X$.

Si $A$ est une partie d’un espace uniforme $X$, $f : X \to X'$ une application uniformément continue, la restriction $f|A$ est une application uniformément continue de $A$ dans $X'$. Si $A' \subset X'$ est tel que $f(X) \subset A'$, l’application de $X$ dans le sous-espace uniforme $A'$ de $X'$ ayant même graphe que $f$, est encore uniformément continue (II, p. 8, prop. 4).

Si $B \subset A \subset X$, le sous-espace uniforme $B$ de $X$ est identique au sous-espace uniforme $B$ du sous-espace uniforme $A$ de $X$ (transitivité des structures uniformes induites; II, p. 8, prop. 5).

#### Proposition 6 {#top-ii-s2-prop-6 .statement}

Soit $A$ une partie partout dense d’un espace uniforme $X$; les adhérences, dans $X \times X$, des entourages du sous-espace uniforme $A$, forment un système fondamental d’entourages de $X$.

En effet, $A \times A$ est dense dans $X \times X$ (I, p. 27, prop. 7). Soit $V$ un entourage ouvert de $A$, trace sur $A \times A$ d’un entourage ouvert $U$ de $X$; on a $U \subset \overline{V}$ (I, p. 7, prop. 5), relation qui, jointe à $\overline{V} \subset \overline{U}$, établit la proposition, compte tenu de II, p. 5, cor. 2.

### 5. Borne supérieure d’un ensemble de structures uniformes

Toute famille $(\mathcal{U}_i)_{i \in I}$ de structures uniformes sur un ensemble $X$ admet une borne supérieure $\mathcal{U}$ dans l’ensemble ordonné des structures uniformes sur $X$: il suffit en effet d’appliquer la prop. 4 de II, p. 8 en désignant par $Y_i$ l’ensemble $X$ muni de la structure uniforme $\mathcal{U}_i$, et par $f_i$ l’application identique $X \to Y_i$; la topologie déduite de $\mathcal{U}$ n’est autre alors que la borne supérieure des topologies déduites des $\mathcal{U}_i$. Il résulte en outre de la prop. 4 de II, p. 8 que si $X \neq \varnothing$ et si $\mathcal{U}_i$ est le filtre des entourages de $\mathcal{U}_i$, le filtre des entourages de $\mathcal{U}$ est la borne supérieure des filtres $\mathcal{U}_i$ (I, p. 37).

#### Exemple {#top-ii-s2-n5-exa-1 .statement}

Pour toute partition finie $\varpi = (A_i)_{1 \leq i \leq n}$ d’un ensemble non vide $X$, l’ensemble $V_\varpi = \bigcup_i (A_i \times A_i)$ constitue à lui seul un système fondamental d’entourages d’une structure uniforme $\mathcal{U}_\varpi$ sur $X$ (II, p. 3, Exemple 2); la structure uniforme des partitions finies sur $X$ (II, p. 7, Remarque 1) est la borne supérieure des structures uniformes $\mathcal{U}_\varpi$.

#### Remarque {#top-ii-s2-n5-rem-1 .statement}

Une famille $(\mathcal{U}_i)$ de structures uniformes sur $X$ admet aussi une borne inférieure dans l’ensemble de toutes les structures uniformes sur $X$, savoir la borne supérieure des structures uniformes moins fines que toutes les $\mathcal{U}_i$ (il y en a, puisque l’ensemble de toutes les structures uniformes sur $X$ a un plus petit élément). Mais (en supposant $X \neq \varnothing$) le filtre des entourages de cette structure uniforme n’est pas nécessairement le filtre intersection des filtres d’entourages des $\mathcal{U}_i$, car ce dernier ne vérifie pas nécessairement l’axiome $(\mathbf{U}_{III})$ (II, p. 35, exerc. 4).

### 6. Produit d’espaces uniformes

#### Définition 4 {#top-ii-s2-def-4 .statement}

Étant donnée une famille $(X_i)_{i \in I}$ d’espaces uniformes, on appelle espace uniforme produit de cette famille l’ensemble produit $X = \prod_{i \in I} X_i$ muni de la structure uniforme la moins fine rendant uniformément continues les projections $\mathrm{pr}_i : X \to X_i$. Cette structure est appelée produit des structures uniformes des $X_i$, et on dit que les espaces uniformes $X_i$ sont les espaces facteurs de $X$.

La topologie déduite de la structure uniforme produit sur $X$ est identique à la topologie produit des topologies des $X_i$ (II, p. 8, corollaire).

#### Proposition 7 {#top-ii-s2-prop-7 .statement}

Soit $f = (f_i)$ une application d’un espace uniforme $Y$ dans un espace uniforme produit $X = \prod_{i \in I} X_i$. Pour que $f$ soit uniformément continue, il faut et il suffit que, pour tout $i \in I$, $f_i$ soit uniformément continue.

Comme $f_i = \mathrm{pr}_i \circ f$, c’est un cas particulier de la prop. 4 de II, p. 8.

#### Corollaire {#top-ii-s2-n6-cor-1 .statement}

Soient $(X_i)_{i \in I}$, $(Y_i)_{i \in I}$ deux familles d’espaces uniformes ayant même ensemble d’indices. Pour tout $i \in I$, soit $f_i$ une application de $X_i$ dans $Y_i$. Si chacune des $f_i$ est uniformément continue, l’application produit $f : (x_i) \mapsto (f_i(x_i))$ est uniformément continue. Réciproquement, si les $X_i$ sont non vides et si $f$ est uniformément continue, chacune des $f_i$ est uniformément continue.

En effet, $f$ s’écrit $x \mapsto (f_i(\mathrm{pr}_i x))$, et la première assertion résulte de la prop. 7. La seconde se démontre en considérant un point $a = (a_i)$ de $\prod_{i \in I} X_i$ et en reprenant le raisonnement de I, p. 25, cor. 1, où on remplace « continue au point $a$ (resp. $a_k$) » par « uniformément continue ».

Le critère général de transitivité des structures uniformes initiales (II, p. 8, prop. 5) montre, comme pour le produit d’espaces topologiques (I, p. 25) que le produit d’espaces uniformes est *associatif*, et que l’on a la propriété suivante:

#### Proposition 8 {#top-ii-s2-prop-8 .statement}

Soient $X$ un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces uniformes, et pour chaque $i \in I$, soit $f_i$ une application de $X$ dans $Y_i$. Soit $f$ l’application $x \mapsto (f_i(x))$ de $X$ dans $Y = \prod_{i \in I} Y_i$, et soit $\mathcal{U}$ la structure uniforme la moins fine sur $X$ rendant uniformément continues les $f_i$. Alors $\mathcal{U}$ est l’image réciproque par $f$ de la structure uniforme induite sur $f(X)$ par la structure uniforme produit sur $Y$.

#### Corollaire {#top-ii-s2-n6-cor-2 .statement}

Pour tout $i \in I$, soit $A_i$ un sous-espace de $Y_i$. La structure uniforme induite sur $A = \prod_{i \in I} A_i$ par la structure uniforme produit sur $\prod_{i \in I} Y_i$ est la structure uniforme produit des structures uniformes des sous-espaces $A_i$.

En outre, on voit aussitôt que si $X_1, X_2$ sont deux espaces uniformes et $a_1$ un point quelconque de $X_1$, l’application $x_2 \mapsto (a_1, x_2)$ est un isomorphisme de $X_2$ sur le sous-espace $\{a_1\} \times X_2$ de $X_1 \times X_2$; par suite:

#### Proposition 9 {#top-ii-s2-prop-9 .statement}

Soit $f$ une application uniformément continue d’un espace uniforme produit $X_1 \times X_2$ dans un espace uniforme $Y$; toute application partielle $x_2 \mapsto f(x_1, x_2)$ de $X_2$ dans $Y$ est alors uniformément continue.

On exprime encore cette proposition en disant qu’une fonction uniformément continue de deux arguments est uniformément continue par rapport à chacun d’eux.

*L’exemple donné dans I, p. 27, Remarque 2, montre que la réciproque de cette proposition est inexacte.*

### 7. Limites projectives d’espaces uniformes

Soient I un ensemble préordonné, la relation de préordre dans I étant notée $\alpha \leq \beta$. Pour tout $\alpha \in I$, soit $X_\alpha$ un espace uniforme, et pour $\alpha \leq \beta$, soit $f_{\alpha \beta}$ une application de $X_\beta$ dans $X_\alpha$. Nous dirons que $(X_\alpha, f_{\alpha \beta})$ est un système projectif d’espaces uniformes si: 1° $(X_\alpha, f_{\alpha \beta})$ est un système projectif d’ensembles (cf. E, III, p. 52); 2° pour $\alpha \leq \beta$, $f_{\alpha \beta}$ est une application uniformément continue. Sur $X = \lim_{\leftarrow} X_\alpha$, la structure uniforme la moins fine rendant uniformément continues les applications canoniques $f_\alpha : X \to X_\alpha$ est appelée la limite projective (pour les $f_{\alpha \beta}$) des structures uniformes des $X_\alpha$, et l’ensemble $X$, muni de cette structure uniforme, est appelé la limite projective du système projectif d’espaces uniformes $(X_\alpha, f_{\alpha \beta})$. Toutes les propriétés des limites projectives d’espaces topologiques établies dans I, pp. 28–29 (à l’exception de la prop. 9) restent valables en remplaçant « topologie » par « structure uniforme » et « application continue » par « application uniformément continue »; en outre:

#### Proposition 10 {#top-ii-s2-prop-10 .statement}

Soient I un ensemble préordonné filtrant, $(X_\alpha, f_{\alpha \beta})$ un système projectif d’espaces uniformes ayant I pour ensemble d’indices, J une partie cofinale de I. Pour tout $\alpha \in I$, soit $f_\alpha$ l’application canonique de $X = \lim_{\leftarrow} X_\alpha$ dans $X_\alpha$, et soit $g_\alpha = f_\alpha \times f_\alpha$. La famille des ensembles $\overline{g_\alpha^1}(V_\alpha)$, où $\alpha$ parcourt J, et où, pour chaque $\alpha \in J$, $V_\alpha$ parcourt un système fondamental d’entourages de $X_\alpha$, est un système fondamental d’entourages de $X$.

Nous laissons au lecteur la démonstration, qui est une adaptation immédiate de celle de la prop. 9 de I, p. 29.

Enfin, la topologie sur $X = \lim_{\leftarrow} X_\alpha$ déduite de la structure uniforme limite projective des structures uniformes des $X_\alpha$ est la limite projective des topologies des $X_\alpha$.

## EXERCICES {#top-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
