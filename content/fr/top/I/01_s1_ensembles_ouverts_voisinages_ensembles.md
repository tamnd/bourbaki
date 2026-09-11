---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 1
section_title: Ensembles ouverts; voisinages; ensembles fermés
lang: fr
source: top-i-iv-fr
pdf_pages: 0013-0020, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: Ensembles ouverts
      page: 0
      pdf_page: 13
    - "no": 2
      title: Voisinages
      page: 2
      pdf_page: 14
    - "no": 3
      title: Systèmes fondamentaux de voisinages; bases d’une topologie
      page: 4
      pdf_page: 16
    - "no": 4
      title: Ensembles fermés
      page: 5
      pdf_page: 17
    - "no": 5
      title: Familles localement finies
      page: 6
      pdf_page: 18
    - "no": 6
      title: Intérieur, adhérence, frontière d'un ensemble; ensembles partout denses
      page: 6
      pdf_page: 18
statements: 23
exercises: 10
content_sha256: 3a696a2ba7595e18e902bd98cff631fa00210213e3f21a762a7168d48f4ae59c
---

## § 1. ENSEMBLES OUVERTS; VOISINAGES; ENSEMBLES FERMÉS

### 1. Ensembles ouverts

#### Définition 1 {#top-i-s1-def-1 .statement}

On appelle structure topologique (ou plus brièvement topologie) sur un ensemble $X$ une structure constituée par la donnée d’un ensemble $\mathcal{O}$ de parties de $X$ possédant les propriétés suivantes (dites axiomes des structures topologiques):
$(O_I)$ Toute réunion d’ensembles de $\mathcal{O}$ est un ensemble de $\mathcal{O}$.
$(O_{II})$ Toute intersection finie d’ensembles de $\mathcal{O}$ est un ensemble de $\mathcal{O}$.
Les ensembles de $\mathcal{O}$ sont appelés ensembles ouverts de la structure topologique définie par $\mathcal{O}$ sur $X$.

#### Définition 2 {#top-i-s1-def-2 .statement}

On appelle espace topologique un ensemble muni d’une structure topologique.

Les éléments d’un espace topologique sont souvent appelés points. Lorsqu’on a défini une topologie sur un ensemble $X$, on dit que cet ensemble est sous-jacent à l’espace topologique $X$.

L’axiome $(O_I)$ implique en particulier que la réunion de la partie vide de $\mathcal{O}$, c’est-à-dire l’ensemble vide (E, II, p. 22) appartient à $\mathcal{O}$. L’axiome $(O_{II})$ implique que l’intersection de la partie vide de $\mathcal{O}$, c’est-à-dire l’ensemble $X$ (E, II, p. 23, déf. 3) appartient à $\mathcal{O}$.

Lorsqu’on veut montrer qu’un ensemble $\mathcal{O}$ de parties de $X$ satisfait à $(O_{II})$, il est souvent commode d’établir séparément qu’il satisfait aux deux axiomes suivants, dont la conjonction est équivalente à $(O_{II})$:
$(O_{IIa})$ L’intersection de deux ensembles de $\mathcal{O}$ appartient à $\mathcal{O}$.
$(O_{IIb})$ $X$ appartient à $\mathcal{O}$.

Exemples de topologies. — Sur un ensemble quelconque X, l’ensemble de parties de X formé de X et de $\varnothing$ satisfait aux axiomes $(O_I)$ et $(O_{II})$ et définit donc une topologie sur X. Il en est de même de l’ensemble $\mathcal{P}(X)$ de toutes les parties de X : la topologie qu’il définit est dite topologie discrète sur X, et l’ensemble X muni de cette topologie est appelé espace discret.

Un recouvrement $(U_i)_{i \in I}$ d’une partie A d’un espace topologique X (E, II, p. 27) est dit ouvert si tous les $U_i$ sont ouverts dans X.

#### Définition 3 {#top-i-s1-def-3 .statement}

On appelle homéomorphisme d’un espace topologique X sur un espace topologique $X'$ un isomorphisme de la structure topologique de X sur celle de $X'$; c’est-à-dire, conformément aux définitions générales (E, IV, p. 6) une bijection de X sur $X'$ qui transforme l’ensemble des parties ouvertes de X en l’ensemble des parties ouvertes de $X'$.

On dit que X et $X'$ sont homéomorphes lorsqu’il existe un homéomorphisme de X sur $X'$.

#### Exemple {#top-i-s1-n1-exa-1 .statement}

Si X et $X'$ sont deux espaces discrets, toute bijection de X sur $X'$ est un homéomorphisme.

La définition d’un homéomorphisme se transforme aussitôt en le critère suivant: pour qu’une bijection f d’un espace topologique X sur un espace topologique $X'$ soit un homéomorphisme, il faut et il suffit que l’image par f de tout ensemble ouvert dans X soit un ensemble ouvert dans $X'$, et que l’image réciproque par f de tout ensemble ouvert dans $X'$ soit un ensemble ouvert dans X.

### 2. Voisinages

#### Définition 4 {#top-i-s1-def-4 .statement}

Dans un espace topologique X, on appelle voisinage d’une partie A de X tout ensemble qui contient un ensemble ouvert contenant A. Les voisinages d’une partie $\{x\}$ réduite à un seul point s’appellent aussi voisinages du point x.

Il est clair que tout voisinage d’une partie A de X est aussi un voisinage de toute partie $B \subset A$; en particulier, c’est un voisinage de tout point de A. Réciproquement, soit A un voisinage de chacun des points d’un ensemble B, et soit U la réunion des ensembles ouverts contenus dans A; on a $U \subset A$, et comme tout point de B appartient à un ensemble ouvert contenu dans A, on a $B \subset U$; mais U est ouvert en vertu de $(O_I)$, donc A est un voisinage de B. En particulier:

#### Proposition 1 {#top-i-s1-prop-1 .statement}

Pour qu’un ensemble soit un voisinage de chacun de ses points, il faut et il suffit qu’il soit ouvert.

Le mot « voisinage » a, dans le langage courant, un sens tel que beaucoup de propriétés où intervient la notion mathématique que nous avons désignée sous ce nom, apparaissent comme l’expression mathématique de propriétés intuitives; le choix de ce terme a donc l’avantage de rendre le langage plus imagé. Dans le même but, on peut aussi utiliser les expressions « assez voisin » et « aussi voisin qu’on veut » dans certains énoncés. Par exemple, on peut énoncer la prop. 1 sous la forme suivante: pour qu’un ensemble A soit ouvert, il faut et il suffit que, pour tout $x \in A$, tous les points assez voisins de $x$ appartiennent à A. Plus généralement, on dira qu’une propriété a lieu pour tous les points assez voisins d’un point $x$, lorsqu’elle a lieu en tous les points d’un voisinage de $x$.

Désignons par $\mathfrak{V}(x)$ l’ensemble des voisinages de $x$. Les ensembles de parties $\mathfrak{V}(x)$ jouissent des propriétés suivantes:

(V_I) *Toute partie de X qui contient un ensemble de $\mathfrak{V}(x)$ appartient à $\mathfrak{V}(x)$*.

(V_{II}) *Toute intersection finie d’ensembles de $\mathfrak{V}(x)$ appartient à $\mathfrak{V}(x)$*.

(V_{III}) *L’élément $x$ appartient à tout ensemble de $\mathfrak{V}(x)$*.

Ces trois propriétés sont en effet des conséquences immédiates de la déf. 4 et de l’axiome (O_{II}).

(V_{IV}) *Si V appartient à $\mathfrak{V}(x)$, il existe un ensemble W appartenant à $\mathfrak{V}(x)$ et tel que, pour tout $y \in W$, V appartienne à $\mathfrak{V}(y)$*.

En effet, il suffit, en vertu de la prop. 1, de prendre pour W un ensemble ouvert contenant $x$ et contenu dans V.

On peut encore exprimer cette propriété en disant qu’un voisinage de $x$ est aussi un voisinage de tous les points assez voisins de $x$.

Ces quatre propriétés des ensembles $\mathfrak{V}(x)$ sont caractéristiques; de façon précise:

#### Proposition 2 {#top-i-s1-prop-2 .statement}

*Si, à chaque élément $x$ d’un ensemble X, on fait correspondre un ensemble $\mathfrak{V}(x)$ de parties de X de sorte que les propriétés (V_I), (V_{II}), (V_{III}) et (V_{IV}) soient vérifiées, il existe une structure topologique et une seule sur X, telle que, pour tout $x \in X$, $\mathfrak{V}(x)$ soit l’ensemble des voisinages de $x$ pour cette topologie.*

D’après la prop. 1, s’il existe une topologie répondant à la question, l’ensemble des ensembles ouverts pour cette topologie est nécessairement l’ensemble $\mathcal{O}$ des parties A de X telles que, *pour tout $x \in A$, on ait $A \in \mathfrak{V}(x)$*; d’où l’unicité de cette topologie si elle existe.
L’ensemble $\mathcal{O}$ satisfait bien aux axiomes (O_I) et (O_{II}): pour (O_I), cela résulte

![Diagram showing nested sets U, W, V, x, y, z](https://i.imgur.com/3Q5z5QG.png)

Figure 1 immédiatement de $(V_I)$, et pour $(O_{II})$, de $(V_{II})$. Reste à voir que, pour la topologie définie par $O$, $\mathfrak{V}(x)$ est l’ensemble des voisinages de $x$ pour tout $x \in X$. Il résulte de $(V_I)$ que tout voisinage de $x$ appartient à $\mathfrak{V}(x)$. Réciproquement, soit $V$ un ensemble de $\mathfrak{V}(x)$, et soit $U$ l’ensemble des points $y \in X$ tels que $V \in \mathfrak{V}(y)$; montrons que $x \in U$, $U \subset V$ et $U \in O$, ce qui achèvera la démonstration. On a $x \in U$ puisque $V \in \mathfrak{V}(x)$; on a $U \subset V$, car tout point $y \in U$ appartient à $V$ en vertu de $(V_{III})$ et de l’hypothèse $V \in \mathfrak{V}(y)$. Reste à montrer que $U \in O$, c’est-à-dire que $U \in \mathfrak{V}(y)$ pour tout $y \in U$; or (fig. 1) si $y \in U$, il existe, en vertu de $(V_{IV})$, un ensemble $W \in \mathfrak{V}(y)$ tel que, pour tout $z \in W$, on ait $V \in \mathfrak{V}(z)$; comme la relation $V \in \mathfrak{V}(z)$ signifie que $z \in U$, on a $W \subset U$, donc, en vertu de $(V_I)$, $U \in \mathfrak{V}(y)$.

C.Q.F.D.

La prop. 2 montre qu’on peut définir une topologie sur $X$ en se donnant les ensembles $\mathfrak{V}(x)$ des voisinages des points de $X$, soumis seulement aux axiomes $(V_I)$, $(V_{II})$, $(V_{III})$ et $(V_{IV})$.

*Exemple. — On définit une topologie sur l’ensemble $\mathbf{Q}$ des nombres rationnels en prenant pour ensembles ouverts de cette topologie les réunions d’intervalles ouverts bornés; en effet, l’ensemble de ces parties satisfait bien à $(O_I)$, et pour voir qu’il satisfait à $(O_{II})$, il suffit de remarquer que si l’intersection de deux intervalles ouverts ]$a, b[$ et ]$c, d[$ n’est pas vide, elle est identique à l’intervalle ouvert ]$a, \beta[$, où $\alpha = \sup(a, c)$ et $\beta = \inf(b, d)$. On obtient la même topologie en définissant pour chaque $x \in \mathbf{Q}$ l’ensemble $\mathfrak{V}(x)$ des voisinages de ce point comme l’ensemble des parties contenant un intervalle ouvert auquel appartient $x$. L’espace topologique obtenu en munissant $\mathbf{Q}$ de cette topologie est appelé droite rationnelle (cf. IV, p. 2). On remarquera que dans cet espace, tout intervalle ouvert est un ensemble ouvert. *On définit de la même manière une topologie sur l’ensemble $\mathbf{R}$ des nombres réels; $\mathbf{R}$, muni de cette topologie, est appelé droite numérique (cf. I. p. 91, exerc. 5 et IV, p. 3).*

### 3. Systèmes fondamentaux de voisinages; bases d’une topologie

#### Définition 5 {#top-i-s1-def-5 .statement}

Dans un espace topologique $X$, on appelle système fondamental de voisinages d’un point $x$ (resp. d’une partie $A$ de $X$) tout ensemble $\mathcal{G}$ de voisinages de $x$ (resp. $A$) tel que pour tout voisinage $V$ de $x$ (resp. $A$), il existe un voisinage $W \in \mathcal{G}$ tel que $W \subset V$.

Si $\mathcal{G}$ est un système fondamental de voisinages d’une partie $A$ de $X$, toute intersection finie d’ensembles de $\mathcal{G}$ contient donc un ensemble de $\mathcal{G}$.

*Exemples. — 1) Dans un espace discret (I, p. 2) l’ensemble $\{x\}$ constitue à lui seul un système fondamental de voisinages du point $x$.
2) Sur la droite rationnelle $\mathbf{Q}$ (I, p. 4), l’ensemble des intervalles ouverts contenant un point $x$ est un système fondamental de voisinages de ce point. Il en est de même de l’ensemble des intervalles ouverts $\left] x - \frac{1}{n}, x + \frac{1}{n} \right[$, et de l’ensemble des intervalles fermés $\left[ x - \frac{1}{n}, x + \frac{1}{n} \right]$, où $n$ prend toutes les valeurs entières $> 0$, ou seulement une suite infinie strictement croissante de valeurs entières $> 0$.
*On a des résultats analogues pour la droite numérique.*

#### Définition 6 {#top-i-s1-def-6 .statement}

On appelle base de la topologie d’un espace topologique X tout ensemble $\mathcal{B}$ de parties ouvertes de X tel que tout ensemble ouvert de X soit réunion d’ensembles appartenant à $\mathcal{B}$.

#### Proposition 3 {#top-i-s1-prop-3 .statement}

Dans un espace topologique, pour qu’un ensemble $\mathcal{B}$ de parties ouvertes de X soit une base de la topologie de X, il faut et il suffit que pour tout $x \in X$, l’ensemble des $V \in \mathcal{B}$ tels que $x \in V$ soit un système fondamental de voisinages de x.

La condition est évidemment nécessaire. Inversement, si elle est satisfaite, pour tout ensemble ouvert U, et tout $x \in U$, il existe un ensemble ouvert $V_x \in \mathcal{B}$ tel que $x \in V_x \subset U$. La réunion des $V_x$ pour $x \in U$ est donc égale à U, ce qui achève la démonstration.

#### Exemple 1 {#top-i-s1-n3-exa-1 .statement}

La topologie discrète a pour base l’ensemble des parties réduites à un seul élément.

#### Exemple 2 {#top-i-s1-n3-exa-2 .statement}

L’ensemble des intervalles ouverts bornés est par définition une base de la topologie de la droite rationnelle (I, p. 4). *L’ensemble des intervalles ouverts bornés est de même une base de la topologie de la droite numérique.*

### 4. Ensembles fermés

#### Définition 7 {#top-i-s1-def-7 .statement}

Dans un espace topologique X, on appelle ensembles fermés les complémentaires des ensembles ouverts de X.

Par passage aux complémentaires, les axiomes (O_I) et (O_{II}) se traduisent respectivement en les suivants:
(O'_I) Toute intersection d’ensembles fermés est un ensemble fermé.
(O'_{II}) Toute réunion finie d’ensembles fermés est un ensemble fermé.

L’ensemble vide et l’espace entier X sont fermés (et par suite, à la fois ouverts et fermés; cf. I, p. 80).

Dans la droite rationnelle, tout intervalle de la forme $[a, \to[$ est un ensemble fermé, car son complémentaire $]\leftarrow, a[$ est ouvert; de la même manière, on voit que tout intervalle de la forme $]\leftarrow, a$ est un ensemble fermé; il en est donc de même de tout intervalle fermé borné $[a, b]$, qui est l’intersection des intervalles $[a, \to[$ et $]\leftarrow, b]$.

L’ensemble $\mathbf{Z}$ des nombres entiers rationnels est fermé dans la droite rationnelle, car son complémentaire $\bigcup_{n \in \mathbf{Z}} ]n, n+1[$ est ouvert.

Un recouvrement $(F_i)_{i \in I}$ d’une partie A d’un espace topologique X est dit fermé si tous les $F_i$ sont fermés dans X.

Un homéomorphisme f d’un espace topologique X sur un espace topologique X’ (I, p. 2) peut encore être caractérisé comme une bijection de X sur X’ telle que l’image par f de tout ensemble fermé dans X soit un ensemble fermé dans X’ et que l’image réciproque par f de tout ensemble fermé dans X’ soit un ensemble fermé dans X.

### 5. Familles localement finies

#### Définition 8 {#top-i-s1-def-8 .statement}

On dit qu’une famille $(A_i)_{i \in I}$ de parties d’un espace topologique $X$ est localement finie si, pour tout $x \in X$, il existe un voisinage $V$ de $x$ tel que $V \cap A_i = \varnothing$ sauf pour un nombre fini d’indices $i \in I$. On dit qu’un ensemble $\mathcal{G}$ de parties de $X$ est localement fini si la famille de parties définie par l’application identique de $\mathcal{G}$ sur lui-même est localement finie.

Il est clair que si $(A_i)_{i \in I}$ est une famille de parties localement finie et si $B_i \subset A_i$ pour tout $i \in I$, la famille $(B_i)_{i \in I}$ est localement finie.

Toute famille *finie* de parties d’un espace topologique $X$ est évidemment localement finie, la réciproque étant inexacte.

Par exemple, dans $\mathbf{Q}$, le recouvrement ouvert formé de l’intervalle $]{\leftarrow}, 1[$ et des intervalles $]n, {\rightarrow}[$ pour tout entier $n \geq 0$ est localement fini; on observera que chaque intervalle $]n, {\rightarrow}[$ rencontre une infinité d'ensembles du recouvrement précédent.

#### Proposition 4 {#top-i-s1-prop-4 .statement}

La réunion d'une famille localement finie de parties fermées d'un espace topologique $X$ est fermée dans $X$.

En effet, soit $(F_i)_{i \in I}$ une famille localement finie de parties fermées de $X$, et supposons que $x \in X$ n'appartienne pas à $F = \bigcup_{i \in I} F_i$; il existe un voisinage $V$ de $x$ qui ne rencontre que les $F_i$ dont les indices appartiennent à une partie *finie* $J$ de $I$. D'autre part, pour tout $i \in J$, $U_i = \complement F_i$ est ouvert et contient $x$; on en conclut que $\complement F$ contient le voisinage $V \cap \bigcap_{i \in J} U_i$ de $x$; en vertu de I, p. 2, prop. 1, $\complement F$ est ouvert, donc $F$ est fermé.

On notera que la réunion d'une famille *quelconque* de parties fermées de $X$ n'est pas nécessairement fermée: par exemple, dans la droite rationnelle $\mathbf{Q}$, l'ensemble $]0, 1[$ est réunion des ensembles fermés $\left[\frac{1}{n}, 1 - \frac{1}{n}\right]$ pour $n > 0$, mais n'est pas fermé.

### 6. Intérieur, adhérence, frontière d'un ensemble; ensembles partout denses

#### Définition 9 {#top-i-s1-def-9 .statement}

Dans un espace topologique $X$, on dit qu'un point $x$ est intérieur à une partie $A$ de $X$ lorsque $A$ est un voisinage de $x$. L'ensemble des points intérieurs à $A$ s'appelle l'intérieur de $A$ et se note $\overset{\circ}{A}$.

D'après la déf. 9 et I, p. 2, déf. 4, un point $x$ est intérieur à $A$ s'il existe un ensemble ouvert contenu dans $A$ et contenant $x$; il en résulte que $\overset{\circ}{A}$ est la réunion des ensembles ouverts contenus dans $A$, et par suite est *le plus grand ensemble ouvert contenu dans* $A$: en d'autres termes, si $B$ est un ensemble *ouvert* contenu dans $A$, on a $B \subset \overset{\circ}{A}$. Par suite, si $A$ et $B$ sont deux parties de $X$ telles que $B \subset A$, on a $\overset{\circ}{B} \subset \overset{\circ}{A}$; pour que $A$ soit un voisinage de $B$, il faut et il suffit que $B \subset \overset{\circ}{A}$.

#### Remarque {#top-i-s1-n6-rem-1 .statement}

L'intérieur d'un ensemble non vide peut être vide; c'est le cas pour un ensemble réduit à un seul point lorsqu'il n'est pas ouvert, par exemple dans la droite rationnelle *(ou la droite numérique)*.

La prop. 1 de I, p. 2 peut encore s’énoncer de la façon suivante:
Pour qu’un ensemble soit ouvert, il faut et il suffit qu’il soit identique à son intérieur.

La propriété (V_{II}) de I, p. 3 entraîne que tout point intérieur à la fois à deux ensembles A et B est intérieur à $A \cap B$; par suite:

(1) $$
\overset{\circ}{A} \cap \overset{\circ}{B} = \overset{\circ}{A} \cap \overset{\circ}{B}.
$$

Tout point intérieur au complémentaire d’un ensemble A est dit extérieur à A, et l’ensemble de ces points s’appelle l’extérieur de A dans X; un point $x \in X$ extérieur à A est donc caractérisé par la propriété qu’il existe un voisinage de x ne rencontrant pas A.

#### Définition 10 {#top-i-s1-def-10 .statement}

Dans un espace topologique X, on dit qu’un point x est adhérent à un ensemble A lorsque tout voisinage de x rencontre A. L’ensemble des points adhérents à A s’appelle adhérence de A et se note $\overline{A}$.

On peut encore énoncer cette définition en disant qu’un point x est adhérent à un ensemble A s’il existe des points de A aussi voisins qu’on veut de x.

Tout point non adhérent à A est extérieur à A, et réciproquement; on a donc les formules (duales l’une de l’autre):

(2) $$
\overline{\overline{A}} = \overset{\circ}{\overline{A}}, \quad \overline{\overset{\circ}{A}} = \overline{A}.
$$

A toute proposition sur les intérieurs d’ensembles correspond donc par passage aux complémentaires (E, II, p. 26, prop. 5) une proposition sur les adhérances, et vice versa. En particulier, l’adhérence d’un ensemble A est le plus petit ensemble fermé contenant A: en d’autres termes, si B est un ensemble fermé tel que $A \subset B$, on a $\overline{A} \subset B$. Si A et B sont deux parties de X telles que $A \subset B$, on a $\overline{A} \subset \overline{B}$.

Pour qu’un ensemble soit fermé, il faut et il suffit qu’il soit identique à son adhérence.

A la formule (1) correspond par passage aux complémentaires la formule

(3) $$
\overline{A \cup B} = \overline{A} \cup \overline{B}.
$$

#### Proposition 5 {#top-i-s1-prop-5 .statement}

Soit A un ensemble ouvert dans X; pour toute partie B de X, on a

(4) $$
A \cap \overline{B} \subset \overline{A \cap B}.
$$

En effet, soit $x \in A$ un point adhérent à B; pour tout voisinage V de x, $V \cap A$ est encore un voisinage de x, puisque A est ouvert; donc $V \cap A \cap B$ n’est pas vide, ce qui montre que x est adhérent à $A \cap B$.

Si x est un point adhérent à A mais n’appartenant pas à A, tout voisinage de x contient un point de A différent de x; mais si $x \in A$, il peut se faire qu’il existe un voisinage de x ne contenant aucun point de A différent de x; on dit alors que x est un *point isolé de* $A$; en particulier, dire qu’un point $x$ est isolé dans l’espace $X$ tout entier signifie que $\{x\}$ est un ensemble ouvert.

Un ensemble fermé dont aucun point n’est isolé est appelé ensemble *parfait*.

#### Définition 11 {#top-i-s1-def-11 .statement}

*Dans un espace topologique* $X$, *un point* $x$ *est dit point frontière d’un ensemble* $A$, *s’il est à la fois adhérent à* $A$ *et à* $\overline{CA}$; *l’ensemble des points frontières de* $A$ *s’appelle frontière de* $A$.

La frontière de $A$ est donc l’ensemble $\overline{A} \cap \overline{CA}$, qui est *fermé*. Un point frontière $x$ de $A$ est caractérisé par la propriété que tout voisinage de $x$ contient au moins un point de $A$ et au moins un point de $CA$; il peut ou non appartenir à $A$. La frontière de $A$ est identique à celle de $CA$; si on considère l’intérieur de $A$, l’extérieur de $A$ et la frontière de $A$, ceux de ces trois ensembles qui ne sont pas vides constituent une *partition de* $X$.

#### Définition 12 {#top-i-s1-def-12 .statement}

*On dit qu’une partie* $A$ *d’un espace topologique* $X$ *est dense dans* $X$ *(ou encore est* *partout dense, lorsqu’il n’en résulte pas de confusion sur* $X$) *si* $\overline{A} = X$, *autrement dit si pour toute partie ouverte non vide* $U$ *de* $X$, $U \cap A$ *est non vide*.

#### Exemple {#top-i-s1-n6-exa-1 .statement}

*On verra dans IV, p. 3 que l’ensemble des nombres rationnels et son complémentaire sont partout denses dans la droite numérique.* \*
Dans un espace discret $X$, il n’existe pas d’ensemble partout dense distinct de $X$. Par contre, tout ensemble non vide est partout dense pour la topologie sur $X$ dont les seuls ensembles ouverts sont $\varnothing$ et $X$.

#### Proposition 6 {#top-i-s1-prop-6 .statement}

*Si* $\mathcal{B}$ *est une base de la topologie d’un espace topologique* $X$, *il existe dans* $X$ *un ensemble partout dense* $D$ *tel que* $\mathrm{Card}(D) \leqslant \mathrm{Card}(\mathcal{B})$.

En effet, on peut se limiter au cas où les ensembles de $\mathcal{B}$ sont non vides (les ensembles de $\mathcal{B}$ non vides formant déjà une base de la topologie de $X$); alors, pour tout $U \in \mathcal{B}$, soit $x_U$ un point de $U$; il résulte de I, p. 5, prop. 3 que l’ensemble $D$ des $x_U$ est dense dans $X$ et on a $\mathrm{Card}(D) \leqslant \mathrm{Card}(\mathcal{B})$ (E, III, p. 25, prop. 3).

## EXERCICES {#top-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
