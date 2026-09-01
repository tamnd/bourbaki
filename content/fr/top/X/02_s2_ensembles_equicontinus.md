---
book: top
book_title: General Topology
chapter: X
chapter_title: ESPACES FONCTIONNELS
section: 2
section_title: Ensembles équicontinus
lang: fr
source: top-v-x-fr
book_pages: TG X.10-TG X.19, TG X.43-TG X.47
pdf_pages: 0259-0268, 0292-0296
extraction: ocr
subsections:
    - "no": 1
      title: Définition et critères généraux
      page: 10
      pdf_page: 259
    - "no": 2
      title: Critères spéciaux d’équicontinuité
      page: 14
      pdf_page: 263
    - "no": 3
      title: Adhérence d’un ensemble équicontinu
      page: 15
      pdf_page: 264
    - "no": 4
      title: Convergence simple et convergence compacte sur les ensembles équicontinus
      page: 16
      pdf_page: 265
    - "no": 5
      title: Ensembles compacts d’applications continues
      page: 17
      pdf_page: 266
statements: 23
exercises: 21
content_sha256: fa7642815c5cf2fdae478943771af908c710a55da0864faeb5a48b1aaf54bda2
---

## § 2. ENSEMBLES ÉQUICONTINUS

### 1. Définition et critères généraux

#### Définition 1 {#top-x-s2-def-1 .statement}

Soient X un espace topologique, Y un espace uniforme. On dit qu’une partie H de $\mathcal{F}(X; Y)$ est équicontinue en un point $x_0 \in X$ si, pour tout entourage V de Y, il existe un voisinage U de $x_0$ dans X tel que, pour tout $x \in U$ et toute fonction $f \in H$, on ait $(f(x_0), f(x)) \in V$. On dit que H est équicontinue si H est équicontinue en tout point de X.

#### Définition 2 {#top-x-s2-def-2 .statement}

Soient X et Y deux espaces uniformes. On dit qu’une partie H de $\mathcal{F}(X; Y)$ est uniformément équicontinue si, pour tout entourage V de Y, il existe un entourage U de X tel que les relations $(x, x') \in U$ et $f \in H$ entraînent $(f(x), f(x')) \in V$.

On dit qu’une famille $(f_i)_{i \in I}$ d’applications de X dans Y est équicontinue en un point $x_0$ (resp. équicontinue, uniformément équicontinue) si l’ensemble des $f_i$ est équicontinu en $x_0$ (resp. équicontinu, uniformément équicontinu).

Il est clair que si $H \subset \mathcal{F}(X; Y)$ est équicontinu en $x_0$, alors toute fonction $f \in H$ est continue en $x_0$; si H est équicontinu, les $f \in H$ sont donc continues dans X, autrement dit $H \subset C(X; Y)$. De même, si H est uniformément équicontinu (X étant un espace uniforme), toute fonction $f \in H$ est uniformément continue dans X. Il est clair que si H est uniformément équicontinu, il est équicontinu, mais un ensemble d’applications uniformément continues peut être équicontinu, sans être uniformément équicontinu (voir X, p. 43, exerc. 1, X, p. 12, cor. 2 et X, p. 15, prop. 4).

#### Exemple 1 {#top-x-s2-n1-exa-1 .statement}

Soient X un espace topologique (resp. un espace uniforme), Y un espace uniforme. Tout ensemble fini d’applications continues (resp. uniformément continues) de X dans Y est équicontinu (resp. uniformément équicontinu).

#### Exemple 2 {#top-x-s2-n1-exa-2 .statement}

Soient X, Y deux espaces métriques, $d$ (resp. $d'$) la distance sur X (resp. Y), k et $\alpha$ deux nombres > 0. L’ensemble des applications $f$ de X dans Y telles que, pour tout couple $(x, x')$ de points de X, on ait
$$
d'(f(x), f(x')) \leq k(d(x, x'))^\alpha
$$
est uniformément équicontinu. Par exemple, l’ensemble des isométries (IX, p. 12) de X sur une partie de Y est uniformément équicontinu.

*Soit H un ensemble de fonctions numériques définies dans un intervalle $I \subset \mathbf{R}$, dérivables dans I et telles que $|f'(x)| \leq k$ dans I pour tout $x \in I$ et toute $f \in H$. Alors H est uniformément équicontinu, car pour tout couple de points $x_1, x_2$ de I, on a
$$
|f(x_1) - f(x_2)| \leq k|x_1 - x_2|
$$
pour toute $f \in H$, en vertu du th. des accroissements finis (FVR, I, § 2, n° 2, th. 1).*

#### Exemple 3 {#top-x-s2-n1-exa-3 .statement}

Soient G un groupe topologique, Y un espace uniforme, $f$ une application uniformément continue de G dans Y, quand G est muni de sa structure uniforme gauche (III, p. 19). Pour tout $s \in G$, soit $f_s$ l’application $x \mapsto f(sx)$ de G dans Y. L’ensemble des applications $f_s$ ($s \in G$) est uniformément équicontinu, puisque la relation $x^{-1}x' \in V$ équivaut à $(sx)^{-1}(sx') \in V$.

#### Proposition 1 {#top-x-s2-prop-1 .statement}

Soient T un ensemble, $S$ un ensemble de parties de T, Y un espace uniforme, X un espace topologique (resp. un espace uniforme), et $f$ une application de $T \times X$ dans Y. Pour tout $A \in S$, soit $H_A \subset \mathcal{F}(X; Y)$ l’ensemble des applications de la forme $x \mapsto f(t, x)$ pour $t \in A$. Pour que l’application $x \mapsto f(. , x)$ de X dans $\mathcal{F}_S(T; Y)$ soit continue en un point $x_0 \in X$ (resp. uniformément continue), il faut et il suffit que, pour tout $A \in S$, l’ensemble $H_A$ soit équicontinu en $x_0$ (resp. uniformément équicontinu).

Considérons d’abord le cas particulier où $S = \{T\}$, autrement dit
$$
\mathcal{F}_S(T; Y) = \mathcal{F}_u(T; Y).
$$

Pour tout entourage V de Y, la condition $(f(., x), f(., x')) \in W(V)$ signifie que, pour tout $t \in T$, $(f(t, x), f(t, x')) \in V$. Dire que $x \mapsto f(., x)$ est continue en $x_0$ (resp. uniformément continue) signifie donc que pour tout entourage V de Y, il existe un voisinage U de $x_0$ dans X (resp. un entourage M de X) tel que la relation $x \in U$ (resp. $(x, x') \in M$) entraîne $(f(t, x), f(t, x_0)) \in V$ (resp. $(f(t, x), f(t, x')) \in V$) pour tout $t \in T$; la proposition résulte alors des déf. 1 et 2 (X, p. 2). Dans le cas général, il faut exprimer que pour tout $A \in \mathfrak{S}$, l’application $x \mapsto f(., x) | A$ de X dans $\mathcal{F}_u(A; Y)$ est continue au point $x_0$ (resp. uniformément continue) en vertu de X, p. 2; d’après ce qui précède, cela équivaut à la condition que pour tout $A \in \mathfrak{S}$, $H_A$ est équicontinu en $x_0$ (resp. uniformément équicontinu).

La prop. 1 permet de donner des traductions parfois utiles des déf. 1 et 2 (X, p. 2), en l’appliquant au cas où $T = H$ et où $f$ est l’application $(h, x) \mapsto h(x)$ de $H \times X$ dans $Y$; comme $f(., x)$ est l’application $h \mapsto h(x)$ de H dans Y, on voit que:

#### Corollaire 1 {#top-x-s2-prop-1-cor-1 .statement}

Soient X un espace topologique (resp. un espace uniforme), Y un espace uniforme, H une partie de $\mathcal{F}(X; Y)$. Pour tout $x \in X$, désignons par $\tilde{x}$ l’application $h \mapsto h(x)$ de H dans Y. Pour que H soit équicontinu en un point $x_0$ (resp. uniformément équicontinu), il faut et il suffit que l’application $x \mapsto \tilde{x}$ de X dans l’espace uniforme $\mathcal{F}_u(H; Y)$ soit continue en $x_0$ (resp. uniformément continue).

En particulier, si X est compact, toute application continue de X dans $\mathcal{F}_u(H; Y)$ est uniformément continue (II, p. 29, th. 2), donc:

#### Corollaire 2 {#top-x-s2-prop-1-cor-2 .statement}

Soient X un espace compact, Y un espace uniforme. Toute partie équicontinue de $\mathcal{F}(X; Y)$ est uniformément équicontinue.

Considérons maintenant un ensemble T, un espace topologique X, un espace uniforme Y, et une application $f : T \times X \to Y$. Désignons par $\tilde{f}$ l’application $x \mapsto f(., x)$ de X dans $\mathcal{F}_u(T; Y)$, et considérons l’application canonique $\theta : (t, g) \mapsto g(t)$ de $T \times \mathcal{F}_u(T; Y)$ dans Y; il est clair que le diagramme

$$
\begin{array}{ccc}
T \times X & \xrightarrow{f} & Y \\
\downarrow_{\iota_T \times \tilde{f}} & & \uparrow_{\theta} \\
T \times \mathcal{F}_u(T; Y)
\end{array}
$$

(où $\iota_T$ est l’application identique) est commutatif. Supposons maintenant que T soit muni d’une topologie et que pour tout $x \in X$, l’application $f(., x) : t \mapsto f(t, x)$ soit continue; on peut alors, dans le diagramme précédent, remplacer $\mathcal{F}_u(T; Y)$ par $\mathcal{C}_u(T; Y)$. Mais on sait que $\theta$ est continue (X, p. 10, prop. 9); si donc l’application $\tilde{f}$ est continue, il en est de même de $f$. Comme la continuité de $\tilde{f}$ s’exprime à l’aide de la prop. 1 (X, p. 11), on a le résultat suivant:

#### Corollaire 3 {#top-x-s2-prop-1-cor-3 .statement}

Soient T et X des espaces topologiques, Y un espace uniforme, f une application de T × X dans Y. Pour que f soit continue, il suffit que les conditions suivantes soient remplies:

1° pour tout x ∈ X, l’application partielle t ↦ f(t, x) est continue;
2° lorsque t parcourt T, les applications partielles x ↦ f(t, x) forment une partie équicontinue de $\mathcal{F}(X; Y)$.

Prenons en particulier pour T une partie H de $\mathcal{F}(X; Y)$ et pour f l’application canonique $(h, x) \mapsto h(x)$ de H × X dans Y; la condition 1° du cor. 3 signifie que H est muni d’une topologie plus fine que celle de la convergence simple, et la condition 2° que H est équicontinue; donc:

#### Corollaire 4 {#top-x-s2-prop-1-cor-4 .statement}

Soient X un espace topologique, Y un espace uniforme, H un ensemble équicontinu d’applications de X dans Y. Si H est muni de la topologie de la convergence simple, l’application $(h, x) \mapsto h(x)$ de H × X dans Y est continue.

De façon imagée, cela exprime que si $h \in H$ converge simplement vers $h_0 \in H$ et si $x \in X$ converge vers $x_0$, alors $h(x)$ converge vers $h_0(x_0)$.

#### Corollaire 5 {#top-x-s2-prop-1-cor-5 .statement}

Soient X un espace topologique, Y, Z deux espaces uniformes, H un ensemble équicontinu d’applications de Y dans Z. Si on munit H, $C(X; Y)$ et $C(X; Z)$ de la topologie de la convergence simple, l’application $(u, v) \mapsto u \circ v$ de H × $C(X; Y)$ dans $C(X; Z)$ est continue.

En effet, il faut prouver que pour tout $x \in X$, l’application $(u, v) \mapsto u(v(x))$ de H × $C(X; Y)$ dans Z continue. Or, $v \mapsto v(x)$ est continue dans H (X, p. 14, Remarque 6), et il résulte du cor. 4 que $(u, y) \mapsto u(y)$ est une application continue de H × Y dans Z; comme $(u, v) \mapsto u(v(x))$ est composée de $(u, y) \mapsto u(y)$ et de $(u, v) \mapsto (u, v(x))$, la proposition est démontrée.

La proposition suivante et son corollaire sont les analogues des cor. 3 et 4 de la prop. 1 pour les applications uniformément continues:

#### Proposition 2 {#top-x-s2-prop-2 .statement}

Soient T, X, Y des espaces uniformes, f une application de T × X dans Y. Pour que f soit uniformément continue, il faut et il suffit que les deux conditions suivantes soient remplies:

1° les applications $x \mapsto f(t, x)$ forment (pour $t \in T$) une partie uniformément équicontinue de $F(X; Y)$;
2° les applications $t \mapsto f(t, x)$ forment (pour $x \in X$) une partie uniformément équicontinue de $F(T; Y)$.

Il est immédiat que les conditions sont nécessaires. Inversement, supposons-les vérifiées et soit W un entourage de Y; il existe alors un entourage U de T et un entourage V de X tels que:

1° $(t', t'') \in U$ entraîne que pour tout $x \in X$,
$$(f(t', x), f(t'', x)) \in W;$$

$2^\circ\ (x', x'') \in V$ entraîne que pour tout $t \in T$,
$$
(f(t, x'), f(t, x'')) \in W.
$$
Il est clair alors que la relation « $(t', t'') \in U$ et $(x', x'') \in V$ » entraîne
$$
(f(t', x'), f(t'', x'')) \in \overset{2}{W},
$$
d’où la proposition.

Prenons en particulier pour $T$ une partie de $\mathcal{F}(X; Y)$ muni de la structure uniforme de la convergence uniforme, et pour $f$ l’application canonique
$$
(h, x) \mapsto h(x);
$$
la condition $2^\circ$ de la prop. 2 est automatiquement remplie, car pour tout entourage $W$ de $Y$, l’ensemble des couples $(h', h'')$ tels que $(h'(x), h''(x)) \in W$ pour tout $x \in X$ est un entourage de la structure uniforme de $H$ par définition. Il suffit donc d’exprimer la condition $1^\circ$; autrement dit:

#### Corollaire {#top-x-s2-n1-cor-1 .statement}

*Soient* $X$, $Y$ *deux espaces uniformes*, $H$ *une partie de* $\mathcal{F}(X; Y)$. *Pour que* $H$ *soit uniformément équicontinue, il faut et il suffit que l’application* $(h, x) \mapsto h(x)$ *de* $H \times X$ *dans* $Y$ *soit uniformément continue, H étant muni de la structure uniforme de la convergence uniforme*.

### 2. Critères spéciaux d’équicontinuité

Il est clair que toute partie d’un ensemble équicontinu (resp. uniformément équicontinu) est équicontinue (resp. uniformément équicontinue). De même, si $X$ est un espace topologique (resp. uniforme) et $Y$ un espace uniforme, toute réunion *finie* de parties équicontinues (resp. uniformément équicontinues) de $\mathcal{F}(X; Y)$ est équicontinue (resp. uniformément équicontinue.)

Soient $X$, $X'$ deux espaces topologiques (resp. uniformes), $Y$, $Y'$ deux espaces uniformes, $f : X' \to X$ une application continue (resp. uniformément continue), $g : Y \to Y'$ une application uniformément continue. Il résulte aussitôt des définitions que l’application $u \mapsto g \circ u \circ f$ de $\mathcal{F}(X; Y)$ dans $\mathcal{F}(X'; Y')$ transforme les parties équicontinues (resp. uniformément équicontinues) en parties équicontinues (resp. uniformément équicontinues).

#### Proposition 3 {#top-x-s2-prop-3 .statement}

*Soient* $X$ *un espace topologique* (resp. *uniforme*), $(Y_i)_{i \in I}$ *une famille d’espaces uniformes*, $Y$ *un ensemble, et pour chaque* $i \in I$, *soit* $f_i$ *une application de* $Y$ *dans* $Y_i$. *On munit* $Y$ *de la structure uniforme la moins fine rendant uniformément continues les* $f_i$. *Pour qu’une partie* $H$ *de* $\mathcal{F}(X; Y)$ *soit équicontinue* (resp. *uniformément équicontinue*), *il faut et il suffit que pour tout* $i \in I$, *l’image de* $H$ *par l’application* $u \mapsto f_i \circ u$ *soit une partie équicontinue* (resp. *uniformément équicontinue*) *de* $\mathcal{F}(X; Y_i)$.

Cela résulte aussitôt des déf. 1 et 2 (X, p. 2) et de la définition des entourages de Y.

#### Proposition 4 {#top-x-s2-prop-4 .statement}

Soient X, Y deux espaces uniformes, H un ensemble d’applications uniformément continues de X dans Y. Soient $\hat{X}$ et $\hat{Y}$ les séparés complétés respectifs de X et Y, et désignons par $\tilde{H}$ l’ensemble des applications $\hat{u}: \hat{X} \to \hat{Y}$, où u parcourt H (II, p. 24, prop. 15). Pour que H soit uniformément équicontinu, il faut et il suffit que $\tilde{H}$ le soit.

Rappelons que l’on a le diagramme commutatif

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y \\
i \downarrow & & j \downarrow \\
\hat{X} & \xrightarrow{\hat{u}} & \hat{Y}
\end{array}
$$

où i et j sont les applications canoniques; en outre la structure uniforme de X (resp. Y) est l’image réciproque par i (resp. j) de celle de $\hat{X}$ (resp. $\hat{Y}$). Pour que H soit uniformément équicontinu, il faut et il suffit donc que son image par l’application $u \mapsto j \circ u$ le soit (prop. 3), et on peut déjà se limiter au cas où Y est séparé et complet; de plus, si $\tilde{H}$ est uniformément équicontinu, il en est de même de H, qui est son image par l’application $\hat{u} \mapsto \hat{u} \circ i$; tout revient donc à établir la réciproque lorsque $\hat{Y} = Y$. Soit alors V un entourage fermé de Y; il y a par hypothèse un entourage U de X tel que les relations $(x, x') \in U, u \in H$ entraînent $(u(x), u(x')) \in V$. Or, si U' est l’image de U par $i \times i$, l’adhérence $\overline{U'}$ de U' dans $\hat{X} \times \hat{X}$ est un entourage de $\hat{X}$ (II, p. 23, prop. 12); l’hypothèse entraîne que, pour $(z, z') \in U'$ et $u \in H$, on a $(\hat{u}(z), \hat{u}(z')) \in V$; comme V est fermé et $\hat{u}$ continue, on a donc aussi, pour tout couple $(t, t') \in \overline{U'}$ et tout $u \in H$, $(\hat{u}(t), \hat{u}(t')) \in V$, ce qui achève la démonstration.

#### Proposition 5 {#top-x-s2-prop-5 .statement}

Soient G, G' deux groupes topologiques, munis de leur structure uniforme gauche, et soit H un ensemble d’homomorphismes de G dans G'. Les conditions suivantes sont équivalentes:

a) H est équicontinu en l’élément neutre e de G;
b) H est équicontinu;
c) H est uniformément équicontinu.

Il suffit de prouver que a) entraîne c). Soit V' un voisinage de l’élément neutre $e'$ de G'; par hypothèse, il existe un voisinage V de e dans G tel que l’on ait $u(V) \subset V'$ pour tout $u \in H$; comme les éléments de H sont des homomorphismes, la relation $x^{-1}y \in V$ entraîne $(u(x))^{-1}u(y) = u(x^{-1}y) \in V'$. D’où la conclusion, compte tenu de la définition des entourages des structures uniformes gauches de G et G' (III, p. 20).

### 3. Adhérence d’un ensemble équicontinu

#### Proposition 6 {#top-x-s2-prop-6 .statement}

Soient X un espace topologique (resp. uniforme), Y un espace uniforme, H une partie de $\mathcal{F}(X; Y)$. Pour que H soit équicontinue en un point $x_0 \in X$ (resp.

uniformément équicontinue), il faut et il suffit que l’adhérence $\overline{H}$ de $H$ dans l’espace $\mathcal{F}_s(X; Y)$ soit équicontinue en $x_0$ (resp. uniformément équicontinue).

La condition est trivialement suffisante. Pour prouver qu’elle est nécessaire, considérons un entourage $V$ de $Y$, fermé dans $Y \times Y$; par hypothèse, il existe un voisinage $U$ de $x_0$ dans $X$ (resp. un entourage $M$ de $X$) tel que la relation $x \in U$ (resp. $(x', x'') \in M$) entraîne $(h(x_0), h(x)) \in V$ (resp. $(h(x'), h(x'')) \in V$) pour tout $h \in H$. Comme $V$ est fermé, les $h \in \mathcal{F}(X; Y)$ qui vérifient la relation
$$
(h(x_0), h(x)) \in V
$$
pour tout $x \in U$ (resp. la relation $(h(x'), h(x'')) \in V$ pour tout couple $(x', x'') \in M$) forment une partie fermée de $\mathcal{F}_s(X; Y)$ ($X$, p. 4, Remarque 6); comme cette partie fermée contient $H$, elle contient $\overline{H}$, d’où la proposition, puisque les entourages de $Y$ fermés dans $Y \times Y$ forment un système fondamental d’entourages (II, p. 5, cor. 2).

### 4. Convergence simple et convergence compacte sur les ensembles équicontinus

#### Théorème 1 {#top-x-s2-thm-1 .statement}

Soient $X$ un espace topologique (resp. uniforme), $Y$ un espace uniforme, $H$ une partie équicontinue (resp. uniformément équicontinue) de $\mathcal{C}(X; Y)$. Alors, sur $H$, les structures uniformes de la convergence compacte (resp. précompacte), de la convergence simple, et de la convergence simple dans une partie partout dense $D$ de $X$, sont identiques.

Il suffit de montrer que sur $H$ la dernière structure uniforme est plus fine que la première; autrement dit, il faut prouver qu’étant donnés un entourage $V$ de $Y$ et une partie compacte (resp. précompacte) $A$ de $X$, il existe un entourage $W$ de $Y$ et une partie finie $F$ de $D$ tels que la relation
$$
u \in H,\ v \in H\ \text{et}\ (u(x), v(x)) \in W\ \text{pour tout}\ x \in F
$$
implique
$$
(u(x), v(x)) \in V\ \text{pour tout}\ x \in A
$$

Supposons d’abord $A$ compact et $H$ équicontinu. Étant donné un entourage symétrique $W$ de $Y$, tout point $x \in X$ possède un voisinage $U(x)$ tel que la relation $x' \in U(x)$ entraîne $(u(x), u(x')) \in W$ pour tout $u \in H$. On peut donc recouvrir l’ensemble compact $A$ par un nombre fini d’ensembles ouverts $U_i$ tels que pour tout couple de points $x', x''$ appartenant à un même ensemble $U_i$, on ait
$$
(u(x'), u(x'')) \in \overset{2}{W}
$$
pour tout $u \in H$. Soit $a_i$ un point de $D \cap U_i$, et soit $F$ l’ensemble des $a_i$; supposons alors (2) vérifiée; pour tout $x \in A$ il existe un indice $i$ tel que $a_i$ et $x$ appartiennent au même ensemble $U_i$, donc on a $(u(x), u(a_i)) \in \overset{2}{W}$ et $(v(a_i), v(x)) \in \overset{2}{W}$, d’où résulte que (2) implique (3) pourvu que $W$ ait été pris de sorte que $\overset{5}{W} \subset V$.

Si $A$ est précompact et $H$ uniformément équicontinu, utilisons la prop. 4 ($X$, p. 15) : il suffit d’observer que $i(\overline{A})$ est compact dans $\hat{X}$, $i(D)$ dense dans $\hat{X}$, et que les entourages de $Y$ sont les images réciproques par $j \times j$ de ceux de $\hat{Y}$.

#### Corollaire {#top-x-s2-n4-cor-1 .statement}

*Sous les hypothèses du th. 1, l’adhérence $\overline{H}$ de $H$ dans l’espace $\mathcal{F}(X; Y)$ muni de la topologie de la convergence simple est identique à l’adhérence de $H$ dans $\mathcal{C}(X; Y)$ muni de la topologie de la convergence compacte* (resp. *précompacte*).

En effet, l’ensemble $\overline{H}$ est équicontinu (resp. uniformément équicontinu) en vertu de $X$, p. 15, prop. 6, donc contenu dans $\mathcal{C}(X; Y)$; le corollaire résulte aussitôt du fait que, sur $\overline{H}$, les deux topologies considérées coïncident en vertu du th. 1.

### 5. Ensembles compacts d’applications continues

**Théorème 2** (Ascoli). — *Soient $X$ un espace topologique (resp. uniforme), $\mathfrak{S}$ un recouvrement de $X$, $Y$ un espace uniforme, $H$ un ensemble d’applications de $X$ dans $Y$; on suppose que pour tout $A \in \mathfrak{S}$, la restriction à $A$ de toute application $u \in H$ soit continue (resp. uniformément continue). Pour que $H$ soit précompact pour la structure uniforme de la $\mathfrak{S}$-convergence, il est nécessaire dans tous les cas et suffisant lorsque les ensembles $A \in \mathfrak{S}$ sont compacts (resp. précompacts), que les conditions suivantes soient vérifiées :

a) *Pour tout $A \in \mathfrak{S}$, l’ensemble $H \mid A \subset \mathcal{F}(A; Y)$ des restrictions à $A$ des fonctions $u \in H$ est équicontinu* (resp. *uniformément équicontinu*).

b) *Pour tout $x \in X$, l’ensemble $H(x) \subset Y$ des $u(x)$ pour $u \in H$ est précompact.*

$1^\circ$ Montrons d’abord la nécessité des conditions *a)* et *b)*. On sait ($X$, p. 4, *Remarque 6*) que l’application $u \mapsto u(x)$ de $\mathcal{F}_{\mathfrak{S}}(X; Y)$ dans $Y$ est uniformément continue ; si $H$ est précompact, il en est donc de même de $H(x)$ (II, p. 30, prop. 2), ce qui démontre *b)*. Pour prouver *a)*, considérons un ensemble $A \in \mathfrak{S}$, un point $x_0 \in A$ et un entourage $V$ de $Y$; puisque $H$ est précompact, il peut être recouvert par un nombre fini d’ensembles petits d’ordre $W(A, V)$; autrement dit, il y a une suite finie $(u_i)$ d’éléments de $H$ tels que pour tout $u \in H$, il existe au moins un indice $i$ pour lequel on ait

$$
(u(x), u_i(x)) \in V \quad \text{pour tout } x \in A.
$$

Cela étant, comme chacune des $u_i \mid A$ est continue au point $x_0$ (resp. uniformément continue), il y a un voisinage $U_i$ de $x_0$ dans $A$ (resp. un entourage $M_i$ de $A$) tel que

$$
x \in U_i \quad \text{entraîne} \quad (u_i(x), u_i(x_0)) \in V
$$
(resp. que

$$
(x', x'') \in M_i \quad \text{entraîne} \quad (u_i(x'), u_i(x'')) \in V).
$$

Soit $U$ (resp. $M$) l’intersection des $U_i$ (resp. des $M_i$) qui est encore un voisinage de $x_0$ dans $A$ (resp. un entourage de $A$). Pour toute $u \in H$, il y a un indice $i$ tel que (4) ait lieu; écrivant la condition (4) pour $x_0$ et pour $x$ (resp. pour $x'$ et $x''$) et tenant compte de (5) (resp. (6)), on voit aussitôt que la relation $x \in U$ (resp. $(x', x'') \in M$) entraîne $(u(x), u(x_0)) \in \overline{V}^3$ (resp. $(u(x'), u(x'')) \in \overline{V}^3$) pour toute $u \in H$, ce qui établit la propriété $a$.

2° Montrons maintenant que les conditions a) et b) sont suffisantes lorsque les $A \in \mathfrak{S}$ sont compacts (resp. précompacts). En effet la condition b) entraîne que $H$ est précompact pour la structure uniforme de la convergence simple (II, p. 31, prop. 3). Mais il résulte de la condition a) et du th. 1 (X, p. 16) que sur $H \mid A$, la structure uniforme de la convergence simple dans $A$ coïncide avec la structure de la convergence uniforme dans $A$, donc $H \mid A$ est précompact dans $\mathcal{F}_u(A; Y)$, ce qui entraîne que $H$ est précompact pour la structure uniforme de la $\mathfrak{S}$-convergence (X, p. 3).

On notera que la condition b) du th. 2 est toujours vérifiée lorsque $Y$ est un espace précompact.

#### Corollaire 1 {#top-x-s2-thm-1-cor-1 .statement}

Soient $X$ un espace topologique (resp. uniforme), $Y$ un espace uniforme séparé, $H$ une partie équicontinue (resp. uniformément équicontinue) de $C(X; Y)$. Supposons $H(x)$ relativement compact dans $Y$ pour tout $x \in X$. Alors $H$ est relativement compact dans $C(X; Y)$ muni de la topologie de la convergence compacte (resp. précompacte).

Soit $\overline{H}$ l’adhérence $H$ dans $\mathcal{F}_s(X; Y)$, qui est encore un ensemble équicontinu (resp. uniformément équicontinu) (X, p. 15, prop. 6). En outre, on a $\overline{H}(x) \subset \overline{H(x)}$ (X, p. 3, Remarque 6), donc $\overline{H}(x)$ est encore relativement compact; le th. 2 (X, p. 17) montre donc que $\overline{H}$ est précompact pour la $\mathfrak{S}$-convergence, en désignant par $\mathfrak{S}$ l’ensemble des parties compactes (resp. précompactes) de $X$. En outre, comme $\overline{H(x)}$ est compact, donc complet, $\overline{H}$ est complet pour la structure uniforme de la convergence simple (II, p. 17, prop. 10 et II, p. 16, prop. 8), donc aussi pour la structure uniforme de la $\mathfrak{S}$-convergence (X, p. 7, cor. 2); $\overline{H}$ est donc compact, puisqu’il est précompact, complet et séparé (X, p. 3, prop. 1).

#### Corollaire 2 {#top-x-s2-thm-1-cor-2 .statement}

Soient $X$ un espace topologique (resp. uniforme), $Y$ un espace uniforme séparé et complet, $H$ une partie équicontinue (resp. uniformément équicontinue) de $C(X; Y)$. On suppose que $H(x)$ est relativement compact dans $Y$ pour tout point $x$ appartenant à une partie partout dense $D$ de $X$. Alors $H$ est relativement compact dans $C(X; Y)$ muni de la topologie de la convergence compacte (resp. précompacte).

Tout revient à prouver que pour tout $x \in X$, $H(x)$ est relativement compact, car alors on peut appliquer le cor. 1. Comme $Y$ est complet, il suffit de voir que $H(x)$ est précompact pour tout $x \in X$. Or, pour tout entourage symétrique $V$ de $Y$, il existe un voisinage $U$ de $x$ tel que, pour tout $x' \in U$ et tout $u \in H$, on ait $(u(x), u(x')) \in V$. Par hypothèse, il existe $x' \in U \cap D$, et comme $H(x')$ est relativement compact dans $Y$, il existe un nombre fini de points $y_k \in Y$ tels que $H(x')$ soit contenu dans la réunion des ensembles $V(y_k)$; alors $H(x)$ est contenu dans la réunion des ensembles $\overline{V}(y_k)$, ce qui achève la démonstration.

#### Corollaire 3 {#top-x-s2-thm-1-cor-3 .statement}

Soient $X$ un espace localement compact, $Y$ un espace uniforme séparé, $H$ une partie de $C(X; Y)$. Pour que $H$ soit relativement compact dans $C_c(X; Y)$, il faut et il suffit que $H$ soit équicontinu et que, pour tout $x \in X$, $H(x)$ soit relativement compact dans $Y$.

Compte tenu du cor. 1, il suffit de montrer que si $H$ est relativement compact dans $C_c(X; Y)$, alors $H$ est équicontinu; or tout point $x \in X$ admet un voisinage compact $A$, et il résulte du th. 2 (X, p. 17) que $H|A$ est équicontinu, ce qui entraîne que $H$ est équicontinu au point $x$; d’où la conclusion.

#### Remarque {#top-x-s2-n5-rem-1 .statement}

Soient $X$ un espace topologique, $Y$ un espace uniforme, $\mathcal{S}$ un ensemble de parties de $X$. Alors sur toute partie précompacte $H$ de $\mathcal{F}_{\mathcal{S}}(X; Y)$, la structure uniforme de la $\mathcal{S}$-convergence est la même que la structure uniforme de la convergence simple dans $B = \bigcup_{A \in \mathcal{S}} A$. On peut se ramener au cas où $B = X$ et où $Y$ est séparé et complet: en effet, si $j$ est l’injection canonique $B \to X$ et $i$ l’application canonique $Y \to \hat{Y}$, la structure uniforme de la $\mathcal{S}$-convergence sur $\mathcal{F}(X; Y)$ est l’image réciproque de la structure uniforme de la $\mathcal{S}$-convergence sur $\mathcal{F}(B; \hat{Y})$ par l’application $\theta : u \mapsto i \circ u \circ j$ (X, p. 5, prop. 4), et pour que $H$ soit précompact, il faut et il suffit que $\theta(H)$ le soit (II, p. 31, prop. 3). Cela étant, si $B = X$ et si $Y$ est séparé et complet, $\mathcal{F}_{\mathcal{S}}(X; Y)$ est séparé et complet (X, p. 3, prop. 1 et X, p. 7, th. 1), donc l’adhérence $\overline{H}$ de $H$ dans cet espace est compacte. Sur $\overline{H}$, la topologie de la convergence simple est séparée (X, p. 3, prop. 1) et moins fine que celle de la $\mathcal{S}$-convergence, donc les deux topologies sont identiques (I, p. 63, cor. 3), et il en est par suite de même des structures uniformes de la $\mathcal{S}$-convergence et de la convergence simple (II, p. 27, th. 1).

## EXERCICES {#top-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
