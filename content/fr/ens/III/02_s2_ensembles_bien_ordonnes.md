---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 2
section_title: Ensembles bien ordonnés
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.15-E III.23, E III.75-E III.79
pdf_pages: 0119-0127, 0179-0183
extraction: ocr
subsections:
    - "no": 1
      title: Segments d’un ensemble bien ordonné
      page: 15
      pdf_page: 119
    - "no": 2
      title: Le principe de récurrence transfinie
      page: 17
      pdf_page: 121
    - "no": 3
      title: Le théorème de Zermelo
      page: 19
      pdf_page: 123
    - "no": 4
      title: Ensembles inductifs
      page: 20
      pdf_page: 124
    - "no": 5
      title: Isomorphismes d’ensembles bien ordonnés
      page: 21
      pdf_page: 125
    - "no": 6
      title: Produits lexicographiques
      page: 22
      pdf_page: 126
statements: 27
exercises: 20
content_sha256: 2bcb4b4feea0003a48f4107927aea90e166d60f5048e35a80eaa3a7a48884c8b
---

## § 2. ENSEMBLES BIEN ORDONNÉS

### 1. Segments d’un ensemble bien ordonné

On dit qu’une relation $R \{x, y\}$ est une *relation de bon ordre entre $x$ et $y$* si $R$ est une relation d’ordre entre $x$ et $y$ et si, pour tout ensemble non vide $E$ sur lequel $R \{x, y\}$ induit une relation d’ordre (c’est-à-dire tel que $x \in E$ entraîne $R \{x, x\}$; cf. III, p. 2), $E$, ordonné par cette relation, admet un *plus petit élément*.

On dit qu’un ensemble $E$ ordonné par un ordre $\Gamma$ est *bien ordonné* si la relation $y \in \Gamma \langle x \rangle$ est une relation de bon ordre entre $x$ et $y$; on dit alors que $\Gamma$ est un *bon ordre* sur $E$. Il revient au même de poser la définition suivante:

#### Définition 1 {#ens-iii-s2-def-1 .statement tag=03JY}

*On dit qu’un ensemble $E$ est bien ordonné s’il est ordonné et si toute partie non vide de $E$ admet un plus petit élément.*

Un ensemble bien ordonné $E$ *est totalement ordonné*, puisque toute partie $\{x, y\}$ de $E$ possède un plus petit élément. Toute partie $A$ de $E$, majorée dans $E$, admet une borne supérieure dans $E$.

#### Exemple 1 {#ens-iii-s2-n1-exa-1 .statement tag=03SX}

Soit $E = \{\alpha, \beta\}$ un ensemble dont les éléments sont distincts. On vérifie aussitôt que la partie $\{(\alpha, \alpha), (\beta, \beta), (\alpha, \beta)\}$ de $E \times E$ est le graphe d’un bon ordre sur $E$.

#### Exemple 2 {#ens-iii-s2-n1-exa-2 .statement tag=03SY}

Toute partie d’un ensemble bien ordonné (en particulier la partie vide) est bien ordonnée par l’ordre induit.

#### Exemple 3 {#ens-iii-s2-n1-exa-3 .statement tag=03SZ}

*L’existence d’ensembles totalement ordonnés et non bien ordonnés est équivalente à l’axiome de l’infini* (III, p. 34, cor. 1 et p. 80, exerc. 3).

#### Exemple 4 {#ens-iii-s2-n1-exa-4 .statement tag=03T0}

*Si $\Gamma$ est un bon ordre sur $E$, l’ordre opposé à $\Gamma$ n’est un bon ordre sur $E$ que si $E$ est fini* (III, p. 80, exerc. 3).*

#### Exemple 5 {#ens-iii-s2-n1-exa-5 .statement tag=03T1}

Soit E un ensemble bien ordonné; l’ensemble $E_1$ obtenu en adjoignant à E un plus grand élément $b$ (III, p. 9) est bien ordonné, car pour toute partie H de $E_1$ non vide et non réduite à $b$, le plus petit élément de $H \cap E$ est aussi le plus petit élément de H.

#### Remarque {#ens-iii-s2-n1-rem-1 .statement tag=03JZ}

\* L’axiome de l’infini (III, p. 45) permet de montrer qu’il existe des ensembles bien ordonnés qui n’ont pas de plus grand élément, par exemple l’ensemble $\mathbf{N}$ des entiers naturels.*

#### Définition 2 {#ens-iii-s2-def-2 .statement tag=03QN}

Dans un ensemble ordonné E, on appelle segment de E toute partie S de E telle que les relations $x \in S, y \in E$ et $y \leq x$ entraînent $y \in S$.

Il est évident que toute intersection ou toute réunion de segments de E est un segment de E; si S est un segment de E, tout segment de S est aussi un segment de E. L’ensemble E lui-même et l’ensemble vide sont des segments de E.

#### Proposition 1 {#ens-iii-s2-prop-1 .statement tag=03QO}

Dans un ensemble bien ordonné E, tout segment de E distinct de E est un intervalle $]\leftarrow, a[$, où $a \in E$.

En effet, soit S un segment de E distinct de E. Comme E — S n’est pas vide, il a un plus petit élément $a$; en vertu de la déf. 2, la relation $x \geq a$ entraîne $x \notin S$, sinon l’on aurait $a \in S$, ce qui est absurde. Donc E — S est l’intervalle $[a, \rightarrow[$, et S l’intervalle $]\leftarrow, a[$.

Pour tout élément $x$ d’un ensemble totalement ordonné E, nous noterons $S_x$ le segment $]\leftarrow, x[$, et nous dirons que c’est le segment d’extrémité $x$.

On notera que, si E est bien ordonné et n’est pas vide, il a un plus petit élément $\alpha$, et que par suite $S_x$ est aussi l’intervalle semi-ouvert $[\alpha, x[$.

Soit E un ensemble totalement ordonné. La réunion A des $S_x$ lorsque $x$ parcourt E est E si E n’a pas de plus grand élément; si E possède un plus grand élément $b$, on a $A = E - \{b\}$.

#### Proposition 2 {#ens-iii-s2-prop-2 .statement tag=03QP}

L’ensemble $E^*$ des segments d’un ensemble bien ordonné E est bien ordonné par inclusion; l’application $x \mapsto S_x$ est un isomorphisme de l’ensemble bien ordonné E sur l’ensemble des segments de E distincts de E.

Il est clair que, si $x \in E$ et $y \in E$, la relation $x \leq y$ entraîne $S_x \subset S_y$ et que $x < y$ entraîne $S_x \neq S_y$; l’application $x \mapsto S_x$ est donc un isomorphisme de E sur l’ensemble S(E) des segments de E distincts de E (III, p. 14, prop. 11), et par suite S(E) est bien ordonné. En outre, $E^*$ est isomorphe à l’ensemble bien ordonné déduit de S(E) par adjonction d’un plus grand élément.

#### Proposition 3 {#ens-iii-s2-prop-3 .statement tag=03QQ}

Soit $(X_i)_{i \in I}$ une famille d’ensembles bien ordonnés telle que, pour tout couple d’indices $(i, k)$ l’un des ensembles $X_i, X_k$ soit un segment de l’autre. Alors, sur l’ensemble $E = \bigcup_{i \in I} X_i$, il existe un ordre et un seul qui induise sur chacun des $X_i$ l’ordre donné; muni de cet ordre, E est un ensemble bien ordonné. Tout segment de $X_i$ est un segment de E; pour tout $x \in X_i$, le segment d’extrémité $x$ dans $X_i$ est égal au segment d’extrémité $x$ dans E; tout segment de E est E ou un segment de l’un des $X_i$.

La première assertion résulte du lemme général suivant:

#### Lemme 1 {#ens-iii-s2-lem-1 .statement tag=03QR}

Soit $(X_\alpha)_{\alpha \in A}$ une famille d’ensembles ordonnés, filtrante pour la relation $\subset$ (autrement dit, telle que pour tout couple d’indices $\alpha, \beta$ il existe un indice $\gamma$ tel que $X_\alpha \subset X_\gamma$ et $X_\beta \subset X_\gamma$). On suppose que, pour tout couple d’indices $(\alpha, \beta)$ tel que $X_\alpha \subset X_\beta$, l’ordre induit sur $X_\alpha$ par celui de $X_\beta$ est identique à l’ordre donné sur $X_\alpha$. Dans ces conditions, sur l’ensemble $E = \bigcup_{\alpha \in A} X_\alpha$, il existe un ordre et un seul qui induise sur chacun des $X_\alpha$ l’ordre donné.

En effet, soit $G_\alpha$ le graphe de l’ordre donné sur $X_\alpha$. Si $G$ est le graphe d’un ordre sur $E$ induisant sur chacun des $X_\alpha$ l’ordre de graphe $G_\alpha$, on a nécessairement $G_\alpha \subset G$ pour tout $\alpha \in A$, donc $G$ contient la réunion $\bigcup_{\alpha \in A} G_\alpha$. D’autre part, pour tout couple $(x, y)$ d’éléments de $E$, il existe par hypothèse un indice $\alpha \in A$ tel que $x \in X_\alpha$ et $y \in X_\alpha$; si $(x, y) \in G$, on a nécessairement $(x, y) \in G_\alpha$, d’où $G \subset \bigcup_{\alpha \in A} G_\alpha$. Si l’ordre cherché existe sur $E$, son graphe est donc nécessairement $G = \bigcup_{\alpha \in A} G_\alpha$. Reste à montrer que cet ensemble répond à la question. Comme $G_\beta \cap (X_\alpha \times X_\alpha) = G_\alpha$ lorsque $X_\alpha \subset X_\beta$, on a $G \cap (X_\alpha \times X_\alpha) = G_\alpha$ pour tout $\alpha \in A$; d’autre part, il résulte de l’hypothèse que trois éléments quelconques $x, y, z$ de $E$ appartiennent à un même $X_\alpha$; on en conclut aussitôt que $(x, y) \in G$ est une relation d’ordre sur $E$, qui répond à la question.

Ce lemme étant établi, montrons que, sous les hypothèses de la prop. 3, chaque $X_t$ est un segment de $E$. En effet, si $x \in X_t, y \in E$ et $y \leq x$, il existe un indice $\kappa$ tel que $X_t \subset X_\kappa$ et $y \in X_\kappa$; comme par hypothèse $X_t$ est un segment de $X_\kappa$, on a $y \in X_t$, d’où notre assertion. Le même raisonnement prouve que, pour tout $x \in X_t$, le segment d’extrémité $x$ dans $X_t$ est identique à l’intervalle $]\leftarrow, x[$ dans $E$. Prouvons ensuite que $E$ est bien ordonné: en effet, si $H$ est une partie non vide de $E$, il y a un indice $t \in I$ tel que $H \cap X_t \neq \varnothing$; si $a$ est le plus petit élément de $H \cap X_t$ dans $X_t$, $a$ est aussi le plus petit élément de $H$ dans $E$; en effet, pour tout $x \in H$, il existe $\kappa \in I$ tel que $X_t \subset X_\kappa$ et $x \in X_\kappa$; on ne peut avoir $x < a$, puisque l’intervalle $]\leftarrow, a]$ est contenu dans $X_t$, et par suite on a $x \geq a$, $X_\kappa$ étant totalement ordonné.

Reste enfin à montrer qu’un segment de $E$ distinct de $E$ est un segment de l’un des $X_t$; cela résulte aussitôt de ce qui précède, puisqu’un tel segment est de la forme $]\leftarrow, x[$ (III, p. 16, prop. 1) et que $x$ appartient à un $X_t$.

### 2. Le principe de récurrence transfinie

#### Lemme 2 {#ens-iii-s2-lem-2 .statement tag=03K0}

Soient $E$ un ensemble bien ordonné, $\mathcal{S}$ un ensemble de segments de $E$ possédant les propriétés suivantes: 1° toute réunion de segments appartenant à $\mathcal{S}$ appartient à $\mathcal{S}$; 2° si $S_x \in \mathcal{S}$, on a $S_x \cup \{x\} \in \mathcal{S}$. Alors, tout segment de $E$ appartient à $\mathcal{S}$.

En effet, supposons qu’il y ait des segments de $E$ n’appartenant pas à $\mathcal{S}$, et soit $S$ le plus petit d’entre eux (III, p. 16, prop. 2). Si $S$ n’a pas de plus grand élément, S est réunion de segments de S distincts de S, et ces segments appartiennent à $\mathcal{S}$ d’après la définition de S, donc $S \in \mathcal{S}$, ce qui est absurde. Si au contraire S a un plus grand élément a, on a $S = S_a \cup \{a\}$, et comme $S_a$ est un segment de S distinct de S, on a $S_a \in \mathcal{S}$; mais on a alors aussi $S \in \mathcal{S}$, ce qui est absurde.

Pour plus de commodité, nous nous placerons dans une théorie $\mathcal{T}$ où E est un ensemble bien ordonné par une relation notée $x \leq y$. On a alors les critères suivants:

C59 (Principe de récurrence transfinie). *Soit $R^{x}$ une relation de $\mathcal{T}$ (x n’étant pas une constante de $\mathcal{T}$), telle que la relation*

$$
(x \in E \text{ et } (\forall y)((y \in E \text{ et } y < x) \Rightarrow R^{y})) \Rightarrow R^{x}
$$

*soit un théorème de $\mathcal{T}$. Dans ces conditions, la relation $(x \in E) \Rightarrow R^{x}$ est un théorème de $\mathcal{T}$*.

En effet, soit $\mathcal{S}$ l’ensemble des segments S de E tels que $(y \in S) \Rightarrow R^{y}$. Il est clair que toute réunion de segments appartenant à $\mathcal{S}$ appartient à $\mathcal{S}$. D’autre part, si $S_x \in \mathcal{S}$, on a $R^{x}$ d’après l’hypothèse du critère, donc $(y \in S_x \cup \{x\}) \Rightarrow R^{y}$ d’après la méthode de disjonction des cas. Alors (lemme 2), $E \in \mathcal{S}$, ce qui prouve le critère.

Dans les utilisations de C59, la relation

$$
x \in E \text{ et } (\forall y)((y \in E \text{ et } y < x) \Rightarrow R^{y})
$$

s’appelle généralement « l’hypothèse de récurrence ».

Pour toute application g d’un segment S de E dans un ensemble F, et pour tout $x \in S$, nous désignerons, dans ce qui suit, par $g^{(x)}$ l’application du segment $S_x = ]\leftarrow, x[$ de E sur $g(S_x)$ qui coïncide avec g dans $S_x$. Avec cette notation:

C60 (définition d’une application par récurrence transfinie). *Soient u une lettre, T^{u} un terme de la théorie $\mathcal{T}$. Il existe un ensemble U et une application f de E sur U tels que, pour tout $x \in E$, on ait $f(x) = T^{f^{(x)}}$. En outre, l’ensemble U et l’application f sont déterminés de façon unique par ces conditions.*

Prouvons d’abord la propriété d’unicité. Supposons que $f'$ et $U'$ satisfont aussi aux conditions du critère. Soit $\mathcal{S}$ l’ensemble des segments S de E tels que $f$ et $f'$ coïncident dans S. Il est clair que toute réunion de segments appartenant à $\mathcal{S}$ appartient à $\mathcal{S}$. D’autre part, si $S_x \in \mathcal{S}$, $f$ et $f'$ coïncident dans $S_x$, donc $f^{(x)} = f'^{(x)}$ et par suite $f(x) = T^{f^{(x)}} = T^{f'^{(x)}} = f'(x)$, ce qui montre que $S_x \cup \{x\} \in \mathcal{S}$. Il en résulte que $E \in \mathcal{S}$ (lemme 2) et par suite $f = f'$ et $U' = f'(E) = f(E) = U$.

Désignons maintenant par $\mathcal{S}_1$ l’ensemble des segments S de E pour lesquels il existe un ensemble $U_S$ et une application $f_S$ de S sur $U_S$ tels que, pour tout $x \in S$, on ait $f_S(x) = T^{f_S^{(x)}}$. Pour tout $S \in \mathcal{S}_1$, $f_S$ et $U_S$ sont déterminés de façon unique en vertu de la première partie du raisonnement; en particulier, si $S'$ et $S''$ sont deux segments appartenant à $\mathcal{S}_1$ et tels que $S' \subset S''$, $f_{S'}$ est l’application de $S'$ sur $f_{S''}(S')$ qui coïncide avec $f_{S''}$ dans $S'$. Il suit de cette remarque que toute réunion de segments appartenant à $\mathfrak{S}_1$ appartient à $\mathfrak{S}_1$ (II, p. 28, prop. 7). D’autre part, si $S_x \in \mathfrak{S}_1$, on définit sur $S = S_x \cup \{x\}$ une fonction $f_S$ prolongeant $f_{S_x}$ en posant $f_S(x) = T\{f_{S_x}\}$ (II, p. 29, prop. 8), et comme $f_S^{(x)} = f_{S_x}$, il est immédiat que $S_x \cup \{x\} \in \mathfrak{S}_1$. Donc (lemme 2), on a $E \in \mathfrak{S}_1$, ce qui achève la démonstration.

Le plus souvent, on appliquera le critère précédent au cas où il existe un ensemble $F$ tel que, *pour toute application h d’un segment de E sur une partie de F, on ait* $T\{h\} \in F$. Alors l’ensemble $U$ obtenu par application de C60 est une *partie de F*. En effet, avec les notations précédentes, soit $\mathfrak{S}_2$ la partie de $\mathfrak{S}_1$ formée des segments $S$ de $E$ tels que $U_S \subset F$. On voit aussitôt que toute réunion de segments appartenant à $\mathfrak{S}_2$ appartient à $\mathfrak{S}_2$; d’autre part, l’hypothèse sur $F$ entraîne que, si $S_x \in \mathfrak{S}_2$, on a $S_x \cup \{x\} \in \mathfrak{S}_2$; on conclut encore à l’aide du lemme 2.

### 3. Le théorème de Zermelo

#### Lemme 3 {#ens-iii-s2-lem-3 .statement tag=03K1}

*Soient E un ensemble, $\mathfrak{S}$ une partie de $\mathcal{P}(E)$ et p une application de $\mathfrak{S}$ dans E telle que $p(X) \notin X$ pour tout $X \in \mathfrak{S}$. Il existe alors une partie M de E et un bon ordre $\Gamma$ sur M tels que* (en désignant par $x \leq y$ la relation $y \in \Gamma\langle x \rangle$ dans M et par $S_x$ le segment $]\leftarrow, x[$):

1° *pour tout* $x \in M$, *on a* $S_x \in \mathfrak{S}$ *et* $p(S_x) = x$;
2° $M \notin \mathfrak{S}$.

Soit $\mathfrak{M}$ l’ensemble des parties G de $E \times E$ satisfaisant aux conditions suivantes:
a) G est le graphe d’un bon ordre sur $\mathrm{pr}_1 G = U$;
b) si on note $x \leq y$ la relation $(x, y) \in G$ dans U, pour tout $x \in U$ le segment $S_x$ est tel que $S_x \in \mathfrak{S}$ et $p(S_x) = x$.

Montrons que, si G, G’ sont deux éléments de $\mathfrak{M}$, et si U et U’ désignent les premières projections de G et G’, l’un des deux ensembles U, U’ est contenu dans l’autre, et que si, par exemple, $U \subset U'$, on a $G = G' \cap (U \times U)$ (en d’autres termes, la relation d’ordre sur U est induite par la relation d’ordre sur U’) et U est un *segment* de U’.

Pour cela, considérons l’ensemble V des $x \in U \cap U'$ tels que les segments d’extrémité x soient les mêmes dans U et U’, et que les ordres induits sur ce segment par ceux de U et U’ soient identiques. Il est clair que V est un *segment* dans U et dans U’, et que les ordres induits sur V sont les mêmes; notre assertion sera prouvée si nous montrons que $V = U$ ou $V = U'$. Raisonnons par l’absurde en supposant $V \neq U$ et $V \neq U'$. Soit x le plus petit élément de $U - V$ dans U et $x'$ le plus petit élément de $U' - V$ dans U’; on a $V = S_x$ dans U, $V = S_{x'}$ dans U’. Mais par hypothèse, on a $V \in \mathfrak{S}$ et $x = p(S_x), x' = p(S_{x'})$, d’où $x = x'$; on aurait alors par définition $x \in V$, ce qui est absurde.

On peut alors appliquer à l’ensemble des $U = \mathrm{pr}_1 G$ (pour $G \in \mathfrak{M}$) la prop. 3 de III, p. 16, et on obtient ainsi un ensemble bien ordonné $M = \bigcup_{G \in \mathfrak{M}} \mathrm{pr}_1 G$; en outre l’on voit aisément que le graphe de l’ordre sur M appartient à $\mathfrak{M}$. Si on avait $M \in \mathcal{S}$, en posant $a = p(M)$, on aurait $a \notin M$; on pourrait alors adjoindre à M l’élément a comme le plus grand élément, et l’ensemble $M' = M \cup \{a\}$ serait bien ordonné. Comme $M = S_a$ dans $M'$, on aurait $S_a \in \mathcal{S}$ et $p(S_a) = a$; le graphe de l’ordre sur $M'$ appartiendrait donc à $\mathfrak{M}$, ce qui est absurde.

On notera que si $\varnothing \notin \mathcal{S}$ (et en particulier si $\mathcal{S}$ est vide), l’ensemble M dont l’existence est affirmée par le lemme 3 est l’ensemble vide, comme le montre la condition 1° de l’énoncé.

**Théorème 1 (Zermelo).** — *Sur tout ensemble E il existe un bon ordre.*

Soit $\mathcal{S} = \mathfrak{P}(E) - \{E\}$ l’ensemble des parties de E distinctes de E; pour tout $X \in \mathcal{S}$, posons $p(X) = \tau_x(x \in E - X)$; comme la relation $X \in \mathcal{S}$ entraîne $(\exists x)(x \in E - X)$, elle entraîne par définition $p(X) \in E - X$ (I, p. 32), donc $p(X) \notin X$. On peut alors appliquer le lemme 3; il existe par suite un bon ordre sur une partie M de E telle que $M \notin \mathcal{S}$; mais la seule partie de E n’appartenant pas à $\mathcal{S}$ est E, d’où le théorème.

### 4. Ensembles inductifs

#### Définition 3 {#ens-iii-s2-def-3 .statement tag=03K2}

*On dit qu’un ensemble ordonné E est inductif si toute partie totalement ordonnée de E possède un majorant dans E.*

#### Exemple 1 {#ens-iii-s2-n4-exa-1 .statement tag=03T2}

Soit $\mathfrak{F}$ un ensemble de parties d’un ensemble A, ordonné par inclusion et tel que, pour tout sous-ensemble totalement ordonné $\mathcal{G}$ de $\mathfrak{F}$, la réunion des ensembles de $\mathcal{G}$ appartienne à $\mathfrak{F}$; alors $\mathfrak{F}$ est inductif pour la relation $\subset$, puisque la réunion des ensembles de $\mathcal{G}$ est la borne supérieure de $\mathcal{G}$ dans $\mathfrak{P}(A)$.

#### Exemple 2 {#ens-iii-s2-n4-exa-2 .statement tag=03T3}

Un exemple important d’ensemble de parties inductif pour la relation $\subset$ est l’ensemble $\mathfrak{F}$ des graphes d’applications de parties d’un ensemble A dans un ensemble B; en effet, $\mathfrak{F}$ est une partie de $\mathfrak{P}(A \times B)$ et dire qu’une partie $\mathcal{G}$ de $\mathfrak{F}$ est totalement ordonnée par inclusion signifie que les éléments de $\mathcal{G}$ sont des graphes d’applications telles que, de deux quelconques de ces applications, l’une prolonge l’autre. Il s’ensuit aussitôt que la réunion des ensembles de $\mathcal{G}$ est un élément de $\mathfrak{F}$ (II, p. 28, prop. 7). On peut donc dire encore que l’ensemble $\Phi(A, B)$ des applications de parties de A dans B est inductif pour la relation d’ordre « v prolonge u » entre u et v.

#### Exemple 3 {#ens-iii-s2-n4-exa-3 .statement tag=03T4}

\* Il résulte de l’axiome de l’infini (III, p. 45) que l’ensemble bien ordonné des entiers naturels n’est pas inductif pour la relation $\leqslant$.*.

#### Théorème 2 {#ens-iii-s2-thm-2 .statement tag=03QT}

*Tout ensemble ordonné inductif possède un élément maximal.*

Ce théorème est un cas particulier du résultat suivant:

#### Proposition 4 {#ens-iii-s2-prop-4 .statement tag=03K3}

*Soit E un ensemble ordonné dont toute partie bien ordonné soit majorée; alors E admet un élément maximal.*

Disons qu’un élément $v \in E$ est un *majorant strict* d’une partie X de E si $v$ est un majorant de X et si $v \notin X$. Soit $\mathcal{S}$ l’ensemble des parties de E admettant un majorant strict, et pour tout $S \in \mathcal{S}$, posons $p(S) = \tau_v(v \text{ est un majorant strict de } S)$; alors $p(S)$ est un majorant strict de S. Appliquant à $\mathcal{S}$ et à $p$ le lemme 3 (III, p. 19), on voit qu’il existe une partie M de E et un bon ordre $\Gamma$ sur $M$ satisfaisant aux conditions de ce lemme; en particulier, $M$ n’admet pas de majorant strict dans $E$. En outre, l’ordre $\Gamma$ est identique à l’ordre induit sur $M$ par celui de $E$. En effet, dans $M$, la relation « $y \in \Gamma\langle x \rangle$ et $x \neq y$ » équivaut à $x \in S_y$, et comme $p(S_y) = y$ est un majorant de $S_y$ (pour l’ordre de $E$), elle entraîne $x < y$ dans $E$. Mais cela signifie que l’injection de $M$ dans $E$ est une application strictement croissante (lorsque $M$ est muni de $\Gamma$) et comme $M$ est totalement ordonné, on en conclut que, dans $M$, les relations $y \in \Gamma\langle x \rangle$ et $x \leq y$ sont équivalentes (III, p. 14, prop. 11). Cela étant, il existe par hypothèse un majorant $m$ de $M$ dans $E$; mais comme $M$ n’admet pas de majorant strict, $m$ est nécessairement élément maximal dans $E$.

#### Corollaire 1 {#ens-iii-s2-prop-4-cor-1 .statement tag=03K4}

*Soient $E$ un ensemble ordonné inductif, et $a$ un élément de $E$; il existe un élément maximal $m$ de $E$ tel que $m \geq a$.*

En effet, il résulte de la déf. 3 que l’ensemble $F$ des éléments $x \geq a$ de $E$ est inductif, et un élément maximal de $F$ est aussi élément maximal de $E$.

#### Corollaire 2 {#ens-iii-s2-prop-4-cor-2 .statement tag=03K5}

*Soit $\mathfrak{F}$ un ensemble de parties d’un ensemble $E$ tel que, pour tout sous-ensemble $\mathfrak{G}$ de $\mathfrak{F}$, totalement ordonné par inclusion, la réunion (resp. l’intersection) des ensembles de $\mathfrak{G}$ appartienne à $\mathfrak{F}$; alors $\mathfrak{F}$ possède un élément maximal (resp. minimal).*

### 5. Isomorphismes d’ensembles bien ordonnés

#### Théorème 3 {#ens-iii-s2-thm-3 .statement tag=03K6}

*Soient $E$ et $F$ deux ensembles bien ordonnés; l’une au moins des deux propositions suivantes est vraie:
1) il existe un isomorphisme et un seul de $E$ sur un segment de $F$;
2) il existe un isomorphisme et un seul de $F$ sur un segment de $E$.*

Soit $\mathfrak{F}$ l’ensemble des applications de parties de $E$ dans $F$ dont chacune est définie dans un segment de $E$ et est un isomorphisme de ce segment sur un segment de $F$. L’ensemble $\mathfrak{F}$, ordonné par la relation « $v$ prolonge $u$ » entre $u$ et $v$, est *inductif*. En effet, soit $\mathfrak{G}$ une partie totalement ordonnée de $\mathfrak{F}$; la réunion $S$ des ensembles de définition des $u \in \mathfrak{G}$ est une réunion de segments de $E$, donc un segment de $E$; si $v$ est la borne supérieure de $\mathfrak{G}$ dans $\Phi(E, F)$ (III, p. 10, *Exemple 2*), $v(S)$ est réunion des ensembles de valeurs des $u \in \mathfrak{G}$, donc est un segment de $F$; enfin, pour tout couple d’éléments $x, y$ de $S$, tel que $x < y$, il existe un $u \in \mathfrak{G}$ dont l’ensemble de définition contient $x$ et $y$ (puisque $\mathfrak{G}$ est totalement ordonnée), et comme $v(x) = u(x) < u(y) = v(y)$, $v$ est un isomorphisme de $S$ sur $v(S)$, ce qui démontre notre assertion. Soit alors $u_0$ un élément maximal de $\mathfrak{F}$ (III, p. 20, th. 2), et soit $S_0$ le segment de $E$ qui est l’ensemble de définition de $u_0$. Si nous prouvons que l’on a, soit $S_0 = E$, soit $u_0(S_0) = F$, l’existence de l’un des isomorphismes considérés dans l’énoncé sera démontrée. Raisonnons par l’absurde, en supposant $S_0 \neq E$ et $u_0(S_0) \neq F$; il existerait alors un élément $a \in E$ et un élément $b \in F$ tels que $S_0 = ]\leftarrow, a[$ et $u_0(S_0) = ]\leftarrow, b[$ (III, p. 16, prop. 1); prolongeons $u_0$ en une application $u_1$ du segment }←, a{ dans F, en posant $u_1(a) = b$; comme $u_1$ est un isomorphisme de }←, a} sur le segment }←, b), cela contredit l’hypothèse que $u_0$ est maximal dans $\mathfrak{F}$.

Les assertions d’unicité du th. 3 sont conséquences du lemme suivant:

#### Lemme 4 {#ens-iii-s2-lem-4 .statement tag=03K7}

*Soient E, F deux ensembles bien ordonnés, f, g deux applications croissantes de E dans F telles que f(E) soit un segment de F et que g soit strictement croissante; on a alors $f(x) \leqslant g(x)$ pour tout $x \in E$.*

Raisonnons par l’absurde, en supposant que l’ensemble des $y \in E$ tels que $f(y) > g(y)$ ne soit pas vide; cet ensemble aurait alors un plus petit élément a. Pour $x < a$, on a, par définition de a, $f(x) \leqslant g(x) < g(a) < f(a)$, g étant strictement croissante. Comme $f(E)$ est un segment de F, il existe $z \in E$ tel que $g(a) = f(z)$; f étant croissante, la relation $f(z) < f(a)$ entraîne $z < a$, d’où

$$
f(z) \leqslant g(z) < g(a) = f(z),
$$

ce qui est absurde.

#### Corollaire 1 {#ens-iii-s2-lem-4-cor-1 .statement tag=03K8}

*Le seul isomorphisme d’un ensemble bien ordonné E sur un segment de E est l’application identique de E sur lui-même.*

Il suffit en effet de faire $F = E$ dans le th. 3.

#### Corollaire 2 {#ens-iii-s2-lem-4-cor-2 .statement tag=03K9}

*Soient E et F deux ensembles bien ordonnés; s’il existe un isomorphisme f de E sur un segment T de F et un isomorphisme g de F sur un segment S de E, on a nécessairement $S = E, T = F$ et f et g sont réciproques l’un de l’autre.*

En effet, $g \circ f$ est un isomorphisme de E sur le segment $g(T) \subset S$ de E; en vertu du cor. 1, on a nécessairement $g(T) = S = E$ et $g \circ f$ est l’application identique de E; on voit de même que $f \circ g$ est l’application identique de F, d’où le corollaire.

#### Corollaire 3 {#ens-iii-s2-lem-4-cor-3 .statement tag=03KA}

*Tout sous-ensemble A d’un ensemble bien ordonné E est isomorphe à un segment de E.*

En vertu du th. 3, il suffit de prouver qu’il n’existe pas d’isomorphisme g de E sur un segment de A de la forme $S_a$; mais g serait alors une application strictement croissante de E dans E, telle que $g(a) \in S_a$, autrement dit $g(a) < a$; or, cette inégalité contredit le lemme 4 (où on prend pour f l’application identique).

### 6. Produits lexicographiques

Soit $(E_t)_{t \in I}$ une famille d’ensembles ordonnés, dont l’ensemble d’indices I soit bien ordonné. Considérons l’ensemble produit $E = \prod_{t \in I} E_t$, et la relation

« $x \in E$ et $y \in E$ et pour le plus petit indice $t \in I$ tel que $\mathrm{pr}_t x \neq \mathrm{pr}_t y$, on a $\mathrm{pr}_t x < \mathrm{pr}_t y$ » que nous noterons $R\{x, y\}$. Il est immédiat que $R\{x, x\}$ est équivalente à $x \in E$, que $R\{x, y\}$ implique ($R\{x, x\}$ et $R\{y, y\}$) et que ($R\{x, y\}$ et $R\{y, x\}$) implique $x = y$. On vérifie en outre que ($R\{x, y\}$ et $R\{y, z\}$) implique $R\{x, z\}$ (il suffit de considérer le plus petit indice $i \in I$ pour lequel deux des trois éléments $\mathrm{pr}_i x, \mathrm{pr}_i y, \mathrm{pr}_i z$ soient inégaux); la relation $R\{x, y\}$ est donc une *relation d’ordre sur l’ensemble produit* $E$. On dit que cette relation, et l’ordre qu’elle définit, sont la *relation d’ordre lexicographique* et l’*ordre lexicographique* sur $E$ (déduits des ordres donnés sur $I$ et sur les $E_i$); l’ensemble $E$, ordonné par cette relation, est appelé le *produit lexicographique* de la famille d’ensembles ordonnés $(E_i)_{i \in I}$. Lorsque les $E_i$ sont *totalement ordonnés*, leur produit lexicographique est *totalement ordonné*.

## EXERCICES {#ens-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
