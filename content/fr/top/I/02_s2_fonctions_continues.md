---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 2
section_title: Fonctions continues
lang: fr
source: top-i-iv-fr
book_pages: TG I.8-TG I.17
pdf_pages: 0020-0029, 0102-0105
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions continues
      page: 8
      pdf_page: 20
    - "no": 2
      title: Comparaison des topologies
      page: 11
      pdf_page: 23
    - "no": 3
      title: Topologies initiales
      page: 12
      pdf_page: 24
    - "no": 4
      title: Topologies finales
      page: 14
      pdf_page: 26
    - "no": 5
      title: Recollement d’espaces topologiques
      page: 16
      pdf_page: 28
statements: 30
exercises: 12
content_sha256: dbdc66bc8f9ab4254506e013eb58494246bd3d2613c30e0d530cd4c0872e1e3a
---

## § 2. FONCTIONS CONTINUES

### 1. Fonctions continues

#### Définition 1 {#top-i-s2-def-1 .statement}

*On dit qu’une application* $f$ *d’un espace topologique* $X$ *dans un espace topologique* $X'$ *est continue en un point* $x_0 \in X$ *si, quel que soit le voisinage* $V'$ *de* $f(x_0)$ *dans* $X'$, *il existe un voisinage* $V$ *de* $x_0$ *dans* $X$ *tel que la relation* $x \in V$ *entraîne* $f(x) \in V'$.

On peut énoncer la déf. 1 sous la forme plus imagée suivante: dire que $f$ est continue au point $x_0$ signifie que $f(x)$ *est aussi voisin qu’on veut de* $f(x_0)$ *dès que* $x$ *est assez voisin de* $x_0$.

La relation « pour tout $x \in V, f(x) \in V'$ » est équivalente à $f(V) \subset V'$ ou encore à $V \subset f^{-1}(V')$; tenant compte de l’axiome ($V_1$) des voisinages, la déf. 1 est équivalente à la suivante: *on dit que* $f : X \to X'$ *est continue au point* $x_0$ *si, pour tout voisinage* $V'$ *de* $f(x_0)$ *dans* $X'$, $f^{-1}(V')$ *est un voisinage de* $x_0$ *dans* $X$. Il suffit d’ailleurs que $f^{-1}(V')$ soit un voisinage de $x_0$ pour tout voisinage $V'$ appartenant à un *système fondamental de voisinages* de $f(x_0)$ dans $X'$ (I, p. 4).

#### Proposition 1 {#top-i-s2-prop-1 .statement}

*Soit* $f$ *une application d’un espace topologique* $X$ *dans un espace topologique* $X'$. *Si* $f$ *est continue au point* $x$, *et si* $x$ *est adhérent à une partie* $A$ *de* $X$, *alors* $f(x)$ *est adhérent à* $f(A)$.

Soit en effet $V'$ un voisinage de $f(x)$ dans $X'$; comme $f^{-1}(V')$ est un voisinage de $x$ dans $X$, il existe un point $y \in A \cap f^{-1}(V')$, donc on a $f(y) \in f(A) \cap V'$, ce qui prouve que $f(x)$ est adhérent à $f(A)$.

#### Proposition 2 {#top-i-s2-prop-2 .statement}

*Soient* $X, X', X''$ *trois espaces topologiques*, $f$ *une application de* $X$ *dans* $X'$ *continue au point* $x \in X$, $g$ *une application de* $X'$ *dans* $X''$ *continue au point* $f(x)$. *Alors l’application composée* $h = g \circ f$ *de* $X$ *dans* $X''$ *est continue au point* $x$.

En effet, soit $V''$ un voisinage de $h(x) = g(f(x))$ dans $X''$; comme $g$ est continue au point $f(x)$, $g(V'')$ est un voisinage de $f(x)$ dans $X'$; comme $f$ est continue au point $x$, $f^{-1}(g(V'')) = h^{-1}(V'')$ est un voisinage de $x$ dans $X$, d’où la proposition.

#### Définition 2 {#top-i-s2-def-2 .statement}

*On dit qu’une application d’un espace topologique* $X$ *dans un espace topologique* $X'$ *est continue dans* $X$ *(ou simplement qu’elle est continue)* *si elle est continue en tout point de* $X$.

#### Exemple 1 {#top-i-s2-n1-exa-1 .statement}

L’application identique d’un espace topologique $X$ sur lui-même est continue.

#### Exemple 2 {#top-i-s2-n1-exa-2 .statement}

Une application constante d’un espace topologique dans un espace topologique est continue.

#### Exemple 3 {#top-i-s2-n1-exa-3 .statement}

Toute application d’un espace discret dans un espace topologique est continue.

#### Théorème 1 {#top-i-s2-thm-1 .statement}

*Soit* $f$ *une application d’un espace topologique* $X$ *dans un espace topologique* $X'$; *les propriétés suivantes sont équivalentes*:
a) $f$ *est continue dans* $X$;
b) *pour tout partie* $A$ *de* $X$, $f(\overline{A}) \subset \overline{f(A)}$;
c) *l’image réciproque par* $f$ *de toute partie fermée de* $X'$ *est une partie fermée de* $X$;
d) *l’image réciproque par* $f$ *de toute partie ouverte de* $X'$ *est une partie ouverte de* $X$.

On a déjà vu que a) entraîne b) (prop. 1). Montrons que b) entraîne c): si $F'$ est une partie fermée de $X'$ et $F = f^{-1}(F')$, on a par hypothèse $f(\overline{F}) \subset \overline{f(F)} \subset \overline{F'} = F'$, donc $\overline{F} \subset f^{-1}(F') = F \subset \overline{F}$, autrement dit $F = \overline{F}$ et $F$ est fermé. En vertu de la relation $\complement f^{-1}(A') = f^{-1}(\complement A')$ pour toute partie $A'$ de $X'$, c) implique d). Enfin, si d) est vérifiée, pour tout $x \in X$ et tout voisinage $V'$ de $f(x)$ dans $X'$, il existe un ensemble $A'$ ouvert dans $X'$ tel que $f(x) \in A' \subset V'$; donc $x \in f^{-1}(A') \subset f^{-1}(V')$, et comme $f^{-1}(A')$ est ouvert, $f^{-1}(V')$ est un voisinage de $x$ dans $X$, ce qui prouve que d) entraîne a).

#### Remarque 1 {#top-i-s2-n1-rem-1 .statement}

Soit $\mathcal{B}$ une base (I, p. 5) de la topologie de $X'$; pour que $f : X \to X'$ soit continue, il faut et il suffit que $f^{-1}(U')$ soit un ensemble ouvert dans $X$ pour tout $U' \in \mathcal{B}$.

#### Exemple {#top-i-s2-n1-exa-4 .statement}

Soit $a$ un nombre rationnel quelconque; l’application $x \mapsto a + x$ de la droite rationnelle $\mathbf{Q}$ dans elle-même est continue dans $\mathbf{Q}$, car l’image réciproque par cette application d’un intervalle ouvert $]b, c[$ est l’intervalle ouvert $]b - a, c - a[$. De même, l’application $x \mapsto ax$ est continue dans $\mathbf{Q}$: c’est évident si $a = 0$, puisque alors $ax = 0$ pour tout $x$; si $a \neq 0$, l’image réciproque par cette application de l’intervalle ouvert $]b, c[$ est l’intervalle ouvert d’extrémités $b/a$ et $c/a$.

#### Remarque 2 {#top-i-s2-n1-rem-2 .statement}

L’image directe d’un ensemble ouvert (resp. fermé) de $X$ par une application continue $f : X \to X'$ n’est pas nécessairement un ensemble ouvert (resp. fermé) dans $X'$ (cf. I, p. 30).

#### Exemple {#top-i-s2-n1-exa-5 .statement}

*L’application $f : x \mapsto 1/(1 + x^2)$ de $\mathbf{R}$ dans lui-même est continue, mais $f(\mathbf{R})$ est l’intervalle semi-ouvert $]0, 1]$, qui n’est ni ouvert ni fermé dans $\mathbf{R}$.*

#### Théorème 2 {#top-i-s2-thm-2 .statement}

1° Si $f : X \to X'$ et $g : X' \to X''$ sont deux applications continues, alors $g \circ f : X \to X''$ est continue.

2° Pour qu’une bijection $f$ d’un espace topologique $X$ sur un espace topologique $X'$ soit un homéomorphisme, il faut et il suffit que $f$ et la bijection réciproque $g$ de $f$ soient continues (ou, comme on dit encore, que $f$ soit bicontinue).

La première assertion est une conséquence immédiate de la prop. 2; la seconde résulte du th. 1, d) et de la définition d’un homéomorphisme (I, p. 2).

#### Remarque 3 {#top-i-s2-n1-rem-3 .statement}

Il peut exister une bijection continue d’un espace topologique $X$ sur un espace topologique $X'$ qui ne soit pas bicontinue; on en a un exemple en prenant pour $X'$ la droite rationnelle $\mathbf{Q}$, pour $X$ l’ensemble $\mathbf{Q}$ muni de la topologie discrète; l’application identique $X \to X'$ est continue, mais non un homéomorphisme.

#### Remarque 4 {#top-i-s2-n1-rem-4 .statement}

Pour vérifier qu’une bijection continue $f : X \to X'$ est un homéomorphisme, il suffit de prouver que pour tout $x \in X$ et tout voisinage $V$ de $x, f(V)$ est un voisinage de $f(x)$ dans $X'$.

#### Remarque 5 {#top-i-s2-n1-rem-5 .statement}

Soient $X$ un espace topologique, et pour tout $x \in X$, soit $\mathfrak{V}(x)$ l’ensemble des voisinages de $x$. Soit $x_0$ un point de $X$; pour tout $x \in X$, définissons un ensemble $\mathfrak{V}_0(x)$ de parties de $X$ de la façon suivante: $\mathfrak{V}_0(x_0) = \mathfrak{V}(x_0)$, et pour $x \neq x_0, \mathfrak{V}_0(x)$ est l’ensemble de toutes les parties de $X$ contenant $x$. On vérifie aussitôt (I, p. 3, prop. 2) que les $\mathfrak{V}_0(x)$ sont les ensembles de voisinages des points de $X$ pour une topologie sur $X$; désignons par $X_0$ l’espace topologique ainsi obtenu, par $j$ l’application identique $X_0 \to X$, qui est continue mais non bicontinue en général. Pour qu’une application $f$ de $X$ dans un espace topologique $X'$ soit continue au point $x_0$, il faut et il suffit que l’application composée $X_0 \xrightarrow{j} X \xrightarrow{f} X'$ soit continue dans $X_0$, ainsi qu’il résulte aussitôt des définitions.

### 2. Comparaison des topologies

Le th. 2 de I, p. 10 montre que l’on peut prendre pour morphismes des structures topologiques les applications continues (E, IV, p. 11); nous supposerons toujours par la suite que l’on a fait ce choix de morphismes. Conformément aux définitions générales (E, IV, p. 13), cela permet de définir une relation d’ordre dans l’ensemble des topologies sur un même ensemble X:

#### Définition 3 {#top-i-s2-def-3 .statement}

Étant données deux topologies $\mathcal{T}_1, \mathcal{T}_2$ sur un même ensemble X, on dit que $\mathcal{T}_1$ est plus fine que $\mathcal{T}_2$ (et que $\mathcal{T}_2$ est moins fine que $\mathcal{T}_1$) si, en désignant par $X_i$ l’ensemble X muni de la topologie $\mathcal{T}_i$ ($i = 1, 2$), l’application identique $X_1 \to X_2$ est continue. Si de plus $\mathcal{T}_1 \neq \mathcal{T}_2$, on dit que $\mathcal{T}_1$ est strictement plus fine que $\mathcal{T}_2$ (et que $\mathcal{T}_2$ est strictement moins fine que $\mathcal{T}_1$).

Deux topologies dont l’une est plus fine que l’autre sont dites comparables.

Les critères de continuité d’une application (I, p. 8, déf. 1 et I, p. 9, th. 1) donnent aussitôt la proposition suivante:
Proposition 3. — Étant données deux topologies $\mathcal{T}_1, \mathcal{T}_2$ sur un ensemble X, les propositions suivantes sont équivalentes:
a) $\mathcal{T}_1$ est plus fine que $\mathcal{T}_2$.
b) Pour tout $x \in X$, tout voisinage de x pour $\mathcal{T}_2$ est un voisinage de x pour $\mathcal{T}_1$.
c) Pour toute partie A de X, l’adhérence de A pour $\mathcal{T}_1$ est contenue dans l’adhérence de A pour $\mathcal{T}_2$.
d) Toute partie de X fermée pour $\mathcal{T}_2$ est fermée pour $\mathcal{T}_1$.
e) Toute partie de X ouverte pour $\mathcal{T}_2$ est ouverte pour $\mathcal{T}_1$.

#### Exemple {#top-i-s2-n2-exa-1 .statement}

*Dans l’espace de Hilbert H des suites $x = (x_n)$ de nombres réels tels que $\|x\|^2 = \sum_{n=0}^\infty x_n^2 < +\infty$, les voisinages d’un point $x_0$ pour la topologie forte sur H sont les ensembles contenant une boule $\|x - x_0\| < \alpha$ de centre $x_0$; les voisinages de $x_0$ pour la topologie faible sur H sont les ensembles contenant un ensemble défini par une relation de la forme $\sup_{1 \leq i \leq n} |(x - x_0 | a_i)| \leq 1$ (où les $a_i$ sont des points de H et $(x | y) = \sum_{n=0}^\infty x_n y_n$ pour $x = (x_n)$ et $y = (y_n)$) (EVT, chap. V). Or, si $\beta = \sup_{1 \leq i \leq n} \|a_i\|$, la relation $\|x - x_0\| \leq 1/\beta$ entraîne $|(x - x_0 | a_i)| \leq \|x - x_0\| \cdot \|a_i\| \leq 1$ pour $1 \leq i \leq n$, ce qui prouve que la topologie forte sur H est plus fine que la topologie faible. D’autre part, pour toute famille finie $(a_i)_{1 \leq i \leq n}$ de points de H, il existe dans H des points x tels que $(x - x_0 | a_i) = 0$ pour $1 \leq i \leq n$, et que $\|x - x_0\|$ soit arbitrairement grand, ce qui prouve que la topologie forte est strictement plus fine que la topologie faible.*

#### Remarque 1 {#top-i-s2-n2-rem-1 .statement}

Dans l’ensemble ordonné des topologies sur un ensemble X, la topologie dont les seuls ensembles ouverts sont $\varnothing$ et X est la topologie la moins fine et la topologie discrète est la topologie la plus fine.

#### Remarque 2 {#top-i-s2-n2-rem-2 .statement}

D’une manière plus imagée, plus une topologie est fine, plus il y a d’ensembles ouverts, d’ensembles fermés, de voisinages; l’adhérence (resp. l’intérieur) d’un ensemble est d’autant plus petite (resp. d’autant plus grand) que la topologie est plus fine; plus une topologie est fine, moins il y a d’ensembles partout denses.

#### Remarque 3 {#top-i-s2-n2-rem-3 .statement}

Si $f : X \to X'$ est une application continue, elle reste continue lorsqu’on remplace la topologie de X par une topologie plus fine et la topologie de X’ par une topologie moins fine (I, p. 10, th. 2). Autrement dit, il y a d’autant plus d’applications continues de X dans X’ que la topologie de X est plus fine et celle de X’ moins fine.

### 3. Topologies initiales

#### Proposition 4 {#top-i-s2-prop-4 .statement}

Soient X un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces topologiques, et pour chaque $i \in I$, soit $f_i$ une application de X dans $Y_i$. Soit $\mathcal{S}$ l’ensemble des parties de X de la forme $f_i^{-1}(U_i)$ ($i \in I$, $U_i$ ouvert dans $Y_i$), et soit $\mathcal{B}$ l’ensemble des intersections finies d’ensembles de $\mathcal{S}$. Alors $\mathcal{B}$ est une base d’une topologie $\mathcal{T}$ sur X qui est la structure topologique initiale sur X pour la famille $(f_i)$ (E, IV, p. 14) et en particulier est la moins fine sur X rendant continues les applications $f_i$. De façon plus précise, soit g une application d’un espace topologique Z dans X. Pour que g soit continue en un point $z \in Z$ (lorsque X est muni de la topologie $\mathcal{T}$), il faut et il suffit que chacune des fonctions $f_i \circ g$ soit continue au point z.

Soit $\mathcal{O}$ l’ensemble de toutes les réunions d’ensembles appartenant à $\mathcal{B}$; il est immédiat que $\mathcal{O}$ satisfait à l’axiome (O_I) en vertu de l’associativité de la réunion, et à l’axiome (O_{II}) en vertu de la définition de $\mathcal{B}$ et de la distributivité de l’intersection finie par rapport à la réunion quelconque (E, II, p. 5, prop. 8). L’ensemble $\mathcal{O}$ est donc l’ensemble des parties ouvertes de X pour une topologie $\mathcal{T}$ dont $\mathcal{B}$ est une base. Prouvons la dernière assertion de l’énoncé, ce qui entraînera les autres en raison des propriétés générales des structures initiales (E, IV, p. 14, critère CST 9). En premier lieu, la définition de $\mathcal{S}$ montre que les $f_i$ sont continues dans X (I, p. 9, th. 1), donc, si g est continue au point z, il en est de même des $f_i \circ g$ (I, p. 10, prop. 2). Inversement, supposons toutes les $f_i \circ g$ continues au point z, et soit V un voisinage de $g(z)$ dans X; par définition, il existe une partie finie J de I et pour chaque $i \in J$ un ensemble ouvert $U_i$ dans $Y_i$ tel que V contienne l’ensemble $\bigcap_{i \in J} f_i^{-1}(U_i)$ et que $g(z)$ appartienne à ce dernier ensemble.

Or, on a $g(V) \supset \bigcap_{i \in J} g(f_i^{-1}(U_i))$, et l’hypothèse entraîne que chacun des ensembles $g(f_i^{-1}(U_i))$ est un voisinage de z dans Z, donc il en est de même de $g(V)$, ce qui achève la démonstration.

Soit $\mathcal{B}_i$ une base de la topologie de $Y_i$ ($i \in I$); désignons par $\mathcal{S}'$ l’ensemble des parties de X de la forme $f_i^{-1}(U_i)$ pour $i \in I$, $U_i \in \mathcal{B}_i$ pour tout $i \in I$; si $\mathcal{B}'$ est l’ensemble des intersections finies d’ensembles de $\mathcal{S}'$, il est immédiat que $\mathcal{S}'$ est encore une base de la topologie $\mathcal{T}$.

Les propriétés générales des structures initiales (E, IV, p. 14, critère CST 10) entraînent en particulier la propriété suivante de transitivité (dont la démonstration directe est d’ailleurs immédiate):

#### Proposition 5 {#top-i-s2-prop-5 .statement}

*Soient X un ensemble, $(Z_i)_{i \in I}$ une famille d’espaces topologiques, $(J_\lambda)_{\lambda \in L}$ une partition de I et $(Y_\lambda)_{\lambda \in L}$ une famille d’ensembles ayant L pour ensembles d’indices. Enfin, pour tout $\lambda \in L$, soit $h_\lambda$ une application de X dans $Y_\lambda$; pour tout $\lambda \in L$ et tout $i \in J_\lambda$, soit $g_{i\lambda}$ une application de $Y_\lambda$ dans $Z_i$; on pose alors $f_i = g_{i\lambda} \circ h_\lambda$. On munit chacun des $Y_\lambda$ de la topologie la moins fine rendant continues les $g_{i\lambda}$ ($i \in J_\lambda$); alors, sur X, la topologie la moins fine rendant continues les $f_i$ est identique à la topologie la moins fine rendant continues les $h_\lambda$.

#### Exemple {#top-i-s2-n3-exa-1 .statement}

I : *Image réciproque d’une topologie.* — Soient X un ensemble, Y un espace topologique, $f$ une application de X dans Y; la topologie la moins fine $\mathcal{T}$ sur X rendant continue $f$ est appelée l’*image réciproque* par $f$ de la topologie de Y. Il résulte de la prop. 4 (I, p. 12) et des formules donnant l’image réciproque d’une réunion et d’une intersection (E, II, p. 25, prop. 3 et 4) que les ensembles ouverts (resp. fermés) pour $\mathcal{T}$ sont les *images réciproques* par $f$ des ensembles ouverts (resp. fermés) de Y; par suite, pour tout $x \in X$, les ensembles $f^{-1}(W)$, où W parcourt un système fondamental de voisinages de $f(x)$ dans Y, forment un système fondamental de voisinages de $x$ pour $\mathcal{T}$. Nous étudierons au § 3, sous le nom de *topologie induite*, le cas particulier où X est une partie de Y et $f$ l’injection canonique $X \to Y$; X, muni de cette topologie, prend alors le nom de *sous-espace* de Y (cf. I, p. 17).

Pour qu’une application $f$ d’un espace topologique X dans un espace topologique $X'$ soit *continue*, il faut et il suffit que la topologie de X soit *plus fine* que l’image réciproque par $f$ de la topologie de $X'$.

II: *Borne supérieure d’un ensemble de topologies.* — Toute famille $(\mathcal{T}_i)_{i \in I}$ de topologies sur un ensemble X admet une *borne supérieure* $\mathcal{T}$ dans l’ensemble ordonné des topologies sur X, c’est-à-dire qu’il existe une topologie *la moins fine* parmi toutes les topologies sur X *plus fines* que toutes les $\mathcal{T}_i$. Il suffit en effet d’appliquer la prop. 4 (I, p. 12) en désignant par $Y_i$ l’ensemble X muni de la topologie $\mathcal{T}_i$ et par $f_i$ l’application identique $X \to Y_i$: $\mathcal{T}$ est la topologie la moins fine rendant continues les $f_i$.

Soit maintenant $\mathfrak{S}$ un ensemble *quelconque* de parties d’un ensemble X; parmi les topologies $\mathcal{T}$ sur X pour lesquelles les ensembles de $\mathfrak{S}$ sont *ouverts*, il en existe une $\mathcal{T}_0$ moins fine que toutes les autres, que l’on appelle la topologie *engendrée par* $\mathfrak{S}$: en effet, il suffit de considérer sur X, pour chaque ensemble $U \in \mathfrak{S}$, la topologie $\mathcal{T}_U$ dont les ensembles ouverts sont $\varnothing$, U et X (il est clair que cet ensemble de parties vérifie $(O_I)$ et $(O_{II})$); la topologie $\mathcal{T}_0$ n’est autre que la *borne supérieure des topologies* $\mathcal{T}_U$. En vertu de la prop. 4 (I, p. 12), si $\mathfrak{B}$ est l’ensemble des *intersections* finies des ensembles appartenant à $\mathcal{G}$, $\mathcal{B}$ est une base de la topologie $\mathcal{T}_0$. On dit que $\mathcal{G}$ est un système générateur de $\mathcal{T}_0$.

III: Topologie produit. — Soit $(X_i)_{i \in I}$ une famille d’espaces topologiques; sur l’ensemble produit $X = \prod_{i \in I} X_i$, la topologie la moins fine rendant continues les projections $\mathrm{pr}_i : X \to X_i$ est appelée la topologie produit de celles des $X_i$; nous l’étudierons plus en détail au § 4.

### 4. Topologies finales

#### Proposition 6 {#top-i-s2-prop-6 .statement}

Soient $X$ un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces topologiques, et pour chaque $i \in I$, soit $f_i$ une application de $Y_i$ dans $X$. Soit $\mathcal{O}$ l’ensemble des parties $U$ de $X$ telles que, pour tout $i \in I$, $f_i^{-1}(U)$ soit ouvert dans $Y_i$; $\mathcal{O}$ est l’ensemble des parties ouvertes de $X$ pour une topologie $\mathcal{T}$ sur $X$ qui est la structure finale sur $X$ pour la famille $(f_i)$ (E, IV, p. 19), et en particulier, la plus fine sur $X$ rendant continues les applications $f_i$. En d’autres termes, soit $g$ une application de $X$ dans un espace topologique $Z$; pour que $g$ soit continue (lorsque $X$ est muni de la topologie $\mathcal{T}$) il faut et il suffit que chacune des applications $g \circ f_i$ soit continue.

On vérifie immédiatement que $\mathcal{O}$ satisfait aux axiomes $(O_1)$ et $(O_{II})$ (E, II, p. 25, prop. 3 et 4); prouvons la dernière assertion de l’énoncé, qui entraînera la proposition en raison des propriétés générales des structures finales (E, IV, p. 19, critère CST 18). Il est clair que les $f_i$ sont continues pour $\mathcal{T}$ par définition de $\mathcal{O}$ (I, p. 9, th. 1), donc, si $g$ est continue, il en est de même des $g \circ f_i$ (I, p. 10, th. 2). Inversement, supposons toutes les $g \circ f_i$ continues, et soit $V$ un ensemble ouvert dans $Z$; par hypothèse, pour tout $i \in I$, $f_i^{-1}(g(V))$ est ouvert dans $Y_i$, donc $g^{-1}(V) \in \mathcal{O}$, ce qui achève la démonstration.

#### Corollaire {#top-i-s2-n4-cor-1 .statement}

Sous les hypothèses de la prop. 6, pour qu’une partie $F$ de $X$ soit fermée pour $\mathcal{T}$, il faut et il suffit que pour tout $i \in I$, $f_i^{-1}(F)$ soit fermé dans $Y_i$.

Cela résulte par passage aux complémentaires de la définition des ensembles ouverts pour $\mathcal{T}$.

Les propriétés générales des structures finales (E, IV, p. 20, critère CST 19) entraînent la propriété suivante de transitivité (dont la démonstration directe est immédiate):

#### Proposition 7 {#top-i-s2-prop-7 .statement}

Soient $X$ un ensemble, $(Z_i)_{i \in I}$ une famille d’espaces topologiques, $(J_\lambda)_{\lambda \in L}$ une partition de $I$ et $(Y_\lambda)_{\lambda \in L}$ une famille d’ensembles ayant $L$ pour ensemble d’indices. Enfin, pour tout $\lambda \in L$, soit $h_\lambda$ une application de $Y_\lambda$ dans $X$; pour tout $\lambda \in L$ et tout $i \in J_\lambda$, soit $g_{\lambda i}$ une application de $Z_i$ dans $Y_\lambda$; on pose alors $f_i = h_\lambda \circ g_{\lambda i}$. On munit chacun des $Y_\lambda$ de la topologie la plus fine rendant continues les $g_{\lambda i}$ ($i \in J_\lambda$); alors, sur $X$, la topologie la plus fine rendant continues les $f_i$ est identique à la topologie la plus fine rendant continues les $h_\lambda$.

#### Exemple {#top-i-s2-n4-exa-1 .statement}

I: Topologie quotient. — Soient $X$ un espace topologique, $R$ une relation d’équivalence sur $X$, $Y = X/R$ l’ensemble quotient de $X$ par cette relation, $\varphi : X \to Y$ l’application canonique. La topologie la plus fine sur $Y$ rendant continue $\varphi$ est appelée topologie quotient de celle de $X$ par la relation $R$; nous l’étudierons plus en détail au § 3.

II: Borne inférieure d’un ensemble de topologies. — Toute famille $(\mathcal{T}_i)_{i \in I}$ de topologies sur un ensemble $X$ admet une borne inférieure $\mathcal{T}$ dans l’ensemble des topologies sur $X$, autrement dit $\mathcal{T}$ est la plus fine des topologies qui sont moins fines que toutes les $\mathcal{T}_i$. Il suffit en effet d’appliquer la prop. 6 en prenant pour $Y_i$ l’ensemble $X$ muni de $\mathcal{T}_i$ et pour $f_i$ l’application identique $Y_i \to X$. Si $\mathcal{O}_i$ est l’ensemble des parties de $X$ ouvertes pour $\mathcal{T}_i$, l’ensemble $\bigcap_{i \in I} \mathcal{O}_i$ est l’ensemble des parties de $X$ ouvertes pour $\mathcal{T}$. On dit aussi que $\mathcal{T}$ est l’intersection des $\mathcal{T}_i$.

III: Somme d’espaces topologiques. — Soit $(X_i)_{i \in I}$ une famille d’espaces topologiques, $X$ l’ensemble somme des $X_i$ (E, II, p. 30, déf. 8); pour tout $i \in I$, soit $j_i$ l’application canonique (injective) de $X_i$ dans $X$. La topologie $\mathcal{T}$ sur $X$ la plus fine rendant continues les $j_i$ est appelée la topologie somme des topologies des $X_i$, et on dit que $X$, muni de cette topologie, est l’espace somme des espaces topologiques $X_i$. Identifions chacun des $X_i$ à une partie de $X$ au moyen de $j_i$; pour qu’un ensemble $A \subset X$ soit ouvert (resp. fermé) pour $\mathcal{T}$, il faut et il suffit que chacun des ensembles $A \cap X_i$ soit ouvert (resp. fermé) dans $X_i$. En particulier, chacun des $X_i$ est à la fois ouvert et fermé.

IV: La proposition suivante généralise la situation de l’exemple III:

#### Proposition 8 {#top-i-s2-prop-8 .statement}

Soient $X$ un ensemble, $(X_\lambda)_{\lambda \in L}$ une famille de parties de $X$. Supposons chaque $X_\lambda$ munie d’une topologie $\mathcal{T}_\lambda$ telle que, pour tout couple $(\lambda, \mu)$ d’indices:
1° $X_\lambda \cap X_\mu$ soit ouvert (resp. fermé) pour chacune des topologies $\mathcal{T}_\lambda, \mathcal{T}_\mu$.
2° Les topologies induites sur $X_\lambda \cap X_\mu$ par $\mathcal{T}_\lambda$ et $\mathcal{T}_\mu$ coïncident.
Soit $\mathcal{T}$ la topologie la plus fine sur $X$ rendant continues les injections $j_\lambda : X_\lambda \to X$. Alors, pour tout $\lambda \in L$, $X_\lambda$ est ouvert (resp. fermé) dans $X$ pour la topologie $\mathcal{T}$ et la topologie induite par $\mathcal{T}$ sur $X_\lambda$ est identique à $\mathcal{T}_\lambda$.

Compte tenu de la prop. 6 et de son corollaire (I, p. 14), tout revient à démontrer que pour tout $\lambda$ et toute partie $A_\lambda$ de $X_\lambda$, les propositions suivantes sont équivalentes:
(i) $A_\lambda$ est ouvert (resp. fermé) pour $\mathcal{T}_\lambda$;
(ii) pour tout $\mu \in L$, $A_\lambda \cap X_\mu$ est ouvert (resp. fermé) pour $\mathcal{T}_\mu$.
Or il est clair que (ii) entraîne (i) en prenant $\mu = \lambda$. Inversement si (i) est vérifiée, $A_\lambda \cap X_\mu$ est ouvert (resp. fermé) dans $X_\lambda \cap X_\mu$ pour la topologie $\mathcal{T}_{\lambda \mu}$ induite sur $X_\lambda \cap X_\mu$ par $\mathcal{T}_\lambda$; mais $\mathcal{T}_{\lambda \mu}$ est aussi la topologie induite sur $X_\lambda \cap X_\mu$ par $\mathcal{T}_\mu$, donc $A_\lambda \cap X_\mu$ est aussi l’intersection de $X_\lambda \cap X_\mu$ et d’une partie $B_\mu$ de $X_\mu$ ouverte (resp. fermée) pour $\mathcal{T}_\mu$; comme $X_\lambda \cap X_\mu$ est ouvert (resp. fermé) pour $\mathcal{T}_\mu$, il en est de même de $A_\lambda \cap X_\mu$, ce qui achève la démonstration.

On notera que si la réunion des $X_\lambda$ est distincte de $X$, la topologie induite par $\mathcal{T}$ sur $X - (\bigcup_{\lambda \in L} X_\lambda)$ est *discrète*. En effet, si $x \in X$ n’appartient à aucun des $X_\lambda$, $\{x\} \cap X_\lambda = \varnothing$ est ouvert pour $\mathcal{T}_\lambda$ quel que soit $\lambda$, donc $\{x\}$ est ouvert pour $\mathcal{T}$.

### 5. Recollement d’espaces topologiques

Soit $(X_\lambda)_{\lambda \in L}$ une famille d’ensembles, et soit $X$ l’ensemble *somme* des $X_\lambda$ (E, II, p. 30, déf. 8); nous identifierons chaque $X_\lambda$ à une partie de $X$ au moyen de l’injection canonique $j_\lambda : X_\lambda \to X$.

Considérons dans $X$ une relation d’équivalence $R$ telle que *chaque classe d’équivalence suivant R ait au plus un élément dans chaque $X_\lambda$*; pour tout couple $(\lambda, \mu)$ d’indices, soit $A_{\lambda \mu}$ la partie de $X_\lambda$ formée des éléments $x$ tels qu’il existe un élément $y \in X_\mu$ appartenant à la classe d’équivalence de $x$. Il est clair qu’à tout point $x \in A_{\lambda \mu}$ correspond un $y \in A_{\mu \lambda}$ et un seul congru à $x$ mod. $R$; les applications $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ ainsi définies vérifient alors les conditions suivantes:

(i) pour tout $\lambda \in L$, $h_{\lambda \lambda}$ est l’identité de $A_{\lambda \lambda} = X_\lambda$;
(ii) pour tout triplet d’indices $(\lambda, \mu, \nu)$ de $L$, et tout $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$, on a $h_{\mu \lambda}(x) \in A_{\mu \nu}$ et

$$
h_{\nu \lambda}(x) = h_{\nu \mu}(h_{\mu \lambda}(x)).
$$

*Inversement*, supposons donnés, pour tout couple $(\lambda, \mu)$ d’indices, une partie $A_{\lambda \mu}$ de $X_\lambda$ et une application $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ vérifiant les conditions (i) et (ii) précédentes. Il résulte d’abord de (ii) appliqué aux triplets $(\lambda, \mu, \lambda)$ et $(\mu, \lambda, \mu)$ que $h_{\lambda \mu} \circ h_{\mu \lambda}$ (resp. $h_{\mu \lambda} \circ h_{\lambda \mu}$) est la restriction de $h_{\lambda \lambda}$ (resp. $h_{\mu \mu}$) à $A_{\lambda \mu}$ (resp. $A_{\mu \lambda}$), d’où, en vertu de (i), on déduit que $h_{\lambda \mu}$ et $h_{\mu \lambda}$ sont des *bijections* réciproques l’une de l’autre. Soit alors $R \{x, y\}$ la relation « il existe $\lambda, \mu$ tels que $x \in A_{\lambda \mu}, y \in A_{\mu \lambda}$ et $y = h_{\mu \lambda}(x)$ ». Il résulte de (i) et de ce qui précède que $R$ est *réflexive* et *symétrique*; d’autre part, si on a $x \in A_{\lambda \mu}, y = h_{\mu \lambda}(x) \in A_{\mu \lambda} \cap A_{\mu \nu}$ et $z = h_{\nu \mu}(y)$, on a aussi $x = h_{\lambda \mu}(y)$, donc, d’après (ii), $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$; la relation (1) prouve donc que $R$ est *transitive*, autrement dit, $R$ est une relation d’équivalence dans $X$. Il résulte d’ailleurs de (i) et de la définition de $R$ que chaque classe d’équivalence suivant $R$ a *au plus un élément* dans chacun des $X_\lambda$, et que $A_{\lambda \mu}$ est l’ensemble des $x \in X_\lambda$ tels qu’il existe un $y \in X_\mu$ congru à $x$ mod. $R$. On dit que l’ensemble quotient $X/R$ est obtenu par *recollement des $X_\lambda$ le long des $A_{\lambda \mu}$ au moyen des bijections* $h_{\mu \lambda}$. Si $\varphi : X \to X/R$ est l’application canonique, la restriction de $\varphi$ à chaque $X_\lambda$ est une *bijection* de $X_\lambda$ sur $\varphi(X_\lambda)$.

Supposons maintenant que chaque $X_\lambda$ soit un *espace topologique*, et soit $\mathcal{T}_\lambda$ sa topologie. Munissons l’ensemble $X/R$ de la topologie $\mathcal{T}$ la plus fine rendant continues les applications $\varphi \circ j_\lambda:X_\lambda \to X/R$; il revient d’ailleurs au même de dire que l’on munit $X$ de la topologie somme des $\mathcal{T}_\lambda$ et $X/R$ du quotient par $R$ de cette topologie. On dit que l’espace topologique $X/R$ s’obtient par recollement des espaces topologiques $X_\lambda$ le long des $A_{\lambda\mu}$, au moyen des bijections $h_{\lambda\mu}$. Les ensembles ouverts (resp. fermés) de $X/R$ sont donc les images canoniques des parties $B$ de $X$, saturées pour $R$ et telles que $B \cap X_\lambda$ soit ouvert (resp. fermé) dans $X_\lambda$ pour tout $\lambda \in L$.

Comme la restriction de $\varphi$ à chaque $X_\lambda$ est une bijection sur la partie $X'_\lambda=\varphi(X_\lambda)$ de $X/R$, on peut transporter au moyen de cette bijection la topologie $\mathcal{T}_\lambda$, de sorte que $X'_\lambda$ est alors muni d’une topologie $\mathcal{T}'_\lambda$ et que la topologie $\mathcal{T}$ sur $X/R$ est la plus fine rendant continues les injections canoniques $X'_\lambda \to X/R$. En général, la topologie induite par $\mathcal{T}$ sur $X'_\lambda$ est moins fine que $\mathcal{T}'_\lambda$, mais non identique à cette dernière même lorsque les $h_{\lambda\mu}$ sont des homéomorphismes (I, p. 94, exerc. 15). Toutefois, il résulte de I, p. 15, prop. 8, que l’on a, avec les notations précédentes :

#### Proposition 9 {#top-i-s2-prop-9 .statement}

Supposons que les $h_{\lambda\mu}$ soient des homéomorphismes et que chaque $A_{\lambda\mu}$ soit ouvert (resp. fermé) dans $X_\lambda$; alors chaque $\varphi(X_\lambda)$ est ouvert (resp. fermé) dans $X/R$ et la restriction de $\varphi$ à $X_\lambda$ est un homéomorphisme de $X_\lambda$ sur le sous-espace $\varphi(X_\lambda)$ de $X/R$.

## EXERCICES {#top-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
