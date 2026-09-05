---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 6
section_title: Filtres
lang: fr
source: top-i-iv-fr
book_pages: TG I.36-TG I.46
pdf_pages: 0048-0058, 0109-0111
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un filtre
      page: 36
      pdf_page: 48
    - "no": 2
      title: Comparaison des filtres
      page: 36
      pdf_page: 48
    - "no": 3
      title: Bases d’un filtre
      page: 38
      pdf_page: 50
    - "no": 4
      title: Ultrafiltres
      page: 39
      pdf_page: 51
    - "no": 5
      title: Filtre induit
      page: 40
      pdf_page: 52
    - "no": 6
      title: Image directe et image réciproque d’une base de filtre
      page: 40
      pdf_page: 52
    - "no": 7
      title: Produit de filtres
      page: 41
      pdf_page: 53
    - "no": 8
      title: Filtres élémentaires
      page: 42
      pdf_page: 54
    - "no": 9
      title: Germes suivant un filtre
      page: 43
      pdf_page: 55
    - "no": 10
      title: Germes en un point
      page: 45
      pdf_page: 57
statements: 29
exercises: 20
content_sha256: b042b015a8c18f06cd3667b0ba26e507005e3526693c0fd684a68f2ea4d54e7a
---

## § 6. FILTRES

### 1. Définition d’un filtre

#### Définition 1 {#top-i-s6-def-1 .statement}

On appelle filtre sur un ensemble X un ensemble $\mathcal{F}$ de parties de X qui possède les propriétés suivantes:

$(\mathrm{F}_I)$ Toute partie de X contenant un ensemble de $\mathcal{F}$ appartient à $\mathcal{F}$.

$(\mathrm{F}_{II})$ Toute intersection finie d’ensembles de $\mathcal{F}$ appartient à $\mathcal{F}$.

$(\mathrm{F}_{III})$ La partie vide de X n’appartient pas à $\mathcal{F}$.

Des deux dernières de ces propriétés on déduit que toute intersection finie d’ensembles de $\mathcal{F}$ est non vide.

Un filtre $\mathcal{F}$ sur X définit sur X une structure dont les axiomes sont ($\mathrm{F}_I$), ($\mathrm{F}_{II}$) et ($\mathrm{F}_{III}$); cette structure est dite structure d’ensemble filtré, et l’ensemble X, muni de cette structure, est appelé ensemble filtré par le filtre $\mathcal{F}$.

L’axiome ($\mathrm{F}_{II}$) est équivalent à la conjonction des deux axiomes suivants:

$(\mathrm{F}_{IIa})$ L’intersection de deux ensembles de $\mathcal{F}$ appartient à $\mathcal{F}$.

$(\mathrm{F}_{IIb})$ X appartient à $\mathcal{F}$.

Les axiomes ($\mathrm{F}_{IIb}$) et ($\mathrm{F}_{III}$) montrent qu’il n’y a pas de filtre sur l’ensemble vide.

Pour qu’un ensemble de parties satisfaisant à ($\mathrm{F}_I$) vérifie aussi ($\mathrm{F}_{IIb}$), il faut et il suffit qu’il soit non vide. Pour qu’un ensemble de parties satisfaisant à ($\mathrm{F}_I$) vérifie aussi ($\mathrm{F}_{III}$), il faut et il suffit que cet ensemble soit différent de $\mathfrak{P}(X)$.

Exemples de filtres. — 1) Si $X \neq \varnothing$, l’ensemble de parties réduit au seul élément X est un filtre sur X. Plus généralement, l’ensemble des parties de X qui contiennent une partie non vide A de X est un filtre sur X.

2) Sur un espace topologique X, l’ensemble des voisinages d’une partie non vide quelconque de X (et en particulier d’un point de X) est un filtre.

3) Si X est un ensemble infini, les complémentaires des parties finies de X sont les éléments d’un filtre. Le filtre des complémentaires des parties finies de l’ensemble $\mathbf{N}$ des entiers $\geqslant 0$ est appelé le filtre de Fréchet.

### 2. Comparaison des filtres

#### Définition 2 {#top-i-s6-def-2 .statement}

Étant donnés deux filtres $\mathcal{F}, \mathcal{F}'$ sur un même ensemble X, on dit que $\mathcal{F}'$ est plus fin que $\mathcal{F}$, ou que $\mathcal{F}$ est moins fin que $\mathcal{F}'$, si $\mathcal{F} \subset \mathcal{F}'$. Si de plus $\mathcal{F} \neq \mathcal{F}'$, on dit que $\mathcal{F}'$ est strictement plus fin que $\mathcal{F}$, ou que $\mathcal{F}$ est strictement moins fin que $\mathcal{F}'$.

Deux filtres dont l’un est plus fin que l’autre sont dits comparables. L’ensemble de tous les filtres sur X est ordonné par la relation « $\mathcal{F}$ est moins fin que $\mathcal{F}'$ », qui n’est autre que la relation induite par la relation d’inclusion dans $\mathfrak{P}(\mathfrak{P}(X))$.

Soit $(\mathcal{F}_i)_{i \in I}$ une famille non vide quelconque de filtres sur un ensemble X (nécessairement non vide); l’ensemble $\mathcal{F} = \bigcap_{i \in I} \mathcal{F}_i$ vérifie les axiomes ($\mathrm{F}_I$), ($\mathrm{F}_{II}$) et $(\mathbf{F}_{\text{III}})$, donc est un filtre, appelé *filtre intersection* de la famille $(\mathcal{F}_i)_{i \in I}$, et qui est évidemment la *borne inférieure* de l’ensemble des $\mathcal{F}_i$ dans l’ensemble ordonné des filtres sur $X$.

Le filtre formé de l’unique ensemble $X$ est *le plus petit élément* de l’ensemble ordonné des filtres sur $X$; lorsque $X$ a plus d’un élément, nous verrons dans I, p. 39 qu’il n’y a pas de plus grand élément dans l’ensemble ordonné des filtres sur $X$.

Étant donné un ensemble $\mathcal{G}$ de parties d’un ensemble $X$, cherchons s’il existe des filtres sur $X$ *contenant* $\mathcal{G}$. Si un tel filtre existe, il contient aussi, d’après $(\mathbf{F}_{\text{II}})$, l’ensemble $\mathcal{G}'$ des *intersections finies* d’ensembles de $\mathcal{G}$ (y compris $X$, intersection de la partie vide de $\mathcal{G}$); une condition *nécessaire* pour que le problème soit possible est donc que la partie vide de $X$ n’appartienne pas à $\mathcal{G}'$. Montrons que cette condition est *suffisante*: en effet, tout filtre contenant $\mathcal{G}'$ contient aussi, d’après $(\mathbf{F}_{\text{I}})$, l’ensemble $\mathcal{G}''$ des parties de $X$ qui contiennent un ensemble de $\mathcal{G}'$. Or, $\mathcal{G}''$ satisfait évidemment à $(\mathbf{F}_{\text{I}})$; il satisfait à $(\mathbf{F}_{\text{II}})$ d’après la définition de $\mathcal{G}'$, et enfin il satisfait à $(\mathbf{F}_{\text{III}})$ puisque la partie vide de $X$ n’appartient pas à $\mathcal{G}'$. L’ensemble $\mathcal{G}''$ est donc *le moins fin des filtres contenant* $\mathcal{G}$. Nous avons donc prouvé:

#### Proposition 1 {#top-i-s6-prop-1 .statement}

*Pour qu’il existe un filtre sur $X$ contenant un ensemble $\mathcal{G}$ de parties de $X$, il faut et il suffit qu’aucune des intersections finies d’ensembles de $\mathcal{G}$ ne soit vide.*

On dit que le filtre $\mathcal{G}''$ défini ci-dessus est *engendré* par $\mathcal{G}$, et que $\mathcal{G}$ est un *système générateur* de $\mathcal{G}''$.

#### Exemple {#top-i-s6-n2-exa-1 .statement}

Soit $\mathcal{G}$ un ensemble quelconque de parties d’un ensemble $X$, et considérons la topologie $\mathcal{T}$ sur $X$ *engendrée* par $\mathcal{G}$ (I, p. 13, *Exemple II*). Comme l’ensemble des intersections finies d’ensembles de $\mathcal{G}$ est une base de $\mathcal{T}$, il résulte de la démonstration de la prop. 1 ci-dessus, ainsi que la prop. 3 de I, p. 5, que pour tout $x \in X$, le *filtre des voisinages* de $x$ pour $\mathcal{T}$ est *engendré* par l’ensemble $\mathcal{G}(x)$ des ensembles de $\mathcal{G}$ auxquels appartient $x$.

#### Corollaire 1 {#top-i-s6-prop-1-cor-1 .statement}

*Soient $\mathcal{F}$ un filtre sur un ensemble $X$, $A$ une partie de $X$. Pour qu’il existe un filtre $\mathcal{F}'$ plus fin que $\mathcal{F}$ et tel que $A \in \mathcal{F}'$ il faut et il suffit que $A$ rencontre tous les ensembles de $\mathcal{F}$.*

#### Corollaire 2 {#top-i-s6-prop-1-cor-2 .statement}

*Pour qu’un ensemble $\Phi$ de filtres sur un ensemble non vide $X$ admette une borne supérieure dans l’ensemble de tous les filtres sur $X$, il faut et il suffit que pour toute suite finie $(\mathcal{F}_i)_{1 \leq i \leq n}$ d’éléments de $\Phi$ et tout $A_i \in \mathcal{F}_i$ ($1 \leq i \leq n$), l’intersection $A_1 \cap \cdots \cap A_n$ soit non vide.*

Cela exprime en effet que la réunion $\mathcal{G}$ des filtres $\mathcal{F} \in \Phi$ vérifie la condition de la prop. 1.

#### Corollaire 3 {#top-i-s6-prop-1-cor-3 .statement}

*L’ensemble ordonné des filtres sur un ensemble non vide $X$ est inductif.*

En effet, tout *ensemble totalement ordonné* $\Phi$ de filtres sur $X$ vérifie la condition du cor. 2, car les ensembles $A_i$ appartiennent tous à l’un des $\mathcal{F}_j$ par hypothèse, et il suffit d’appliquer $(\mathbf{F}_{\text{II}})$.

### 3. Bases d’un filtre

Si $\mathcal{G}$ est un système générateur d’un filtre $\mathcal{F}$ sur $X$ (I, p. 37), $\mathcal{F}$ n’est pas en général l’ensemble des parties de $X$ contenant un ensemble de $\mathcal{G}$: pour que $\mathcal{G}$ ait cette propriété, il faut et il suffit que toute intersection finie d’ensembles de $\mathcal{G}$ contienne un ensemble de $\mathcal{G}$. On a donc la proposition suivante:

#### Proposition 2 {#top-i-s6-prop-2 .statement}

Étant donné un ensemble de parties $\mathcal{B}$ d’un ensemble $X$, pour que l’ensemble des parties de $X$ contenant un ensemble de $\mathcal{B}$ soit un filtre, il faut et il suffit que $\mathcal{B}$ possède les deux propriétés suivantes:

$(\mathrm{B}_I)$ L’intersection de deux ensembles de $\mathcal{B}$ contient un ensemble de $\mathcal{B}$.

$(\mathrm{B}_{II})$ $\mathcal{B}$ n’est pas vide, et la partie vide de $X$ n’appartient pas à $\mathcal{B}$.

#### Définition 3 {#top-i-s6-def-3 .statement}

On dit qu’un ensemble de parties $\mathcal{B}$ d’un ensemble $X$ qui satisfait aux axiomes $(\mathrm{B}_I)$ et $(\mathrm{B}_{II})$ est une base du filtre qu’il engendre. On dit que deux bases de filtre sont équivalentes lorsqu’elles engendrent le même filtre.

Si $\mathcal{G}$ est un système générateur d’un filtre $\mathcal{F}$, l’ensemble $\mathcal{G}'$ des intersections finies d’ensembles de $\mathcal{G}$ est une base de $\mathcal{F}$ (I, p. 37).

#### Proposition 3 {#top-i-s6-prop-3 .statement}

Pour qu’une partie $\mathcal{B}$ d’un filtre $\mathcal{F}$ sur $X$ soit une base de $\mathcal{F}$, il faut et il suffit que tout ensemble de $\mathcal{F}$ contienne un ensemble de $\mathcal{B}$.

La condition est évidemment nécessaire; elle est suffisante, car si elle est remplie, l’ensemble des parties de $X$ contenant un ensemble de $\mathcal{B}$ est identique à $\mathcal{F}$ en vertu de $(\mathrm{F}_I)$.

#### Proposition 4 {#top-i-s6-prop-4 .statement}

Sur un ensemble $X$, pour qu’un filtre $\mathcal{F}'$ de base $\mathcal{B}'$ soit plus fin qu’un filtre $\mathcal{F}$ de base $\mathcal{B}$, il faut et il suffit que tout ensemble de $\mathcal{B}$ contienne un ensemble de $\mathcal{B}'$.

La proposition résulte aussitôt des déf. 2 (I, p. 36) et 3 (I, p. 38).

#### Corollaire {#top-i-s6-n3-cor-1 .statement}

Pour que deux bases de filtre $\mathcal{B}$, $\mathcal{B}'$ sur un ensemble $X$ soient équivalentes, il faut et il suffit que tout ensemble de $\mathcal{B}$ contienne un ensemble de $\mathcal{B}'$ et que tout ensemble de $\mathcal{B}'$ contienne un ensemble de $\mathcal{B}$.

*Exemples de bases de filtre.* — 1) Soit $X$ un espace topologique; les bases du filtre des voisinages d’un point $x \in X$ ne sont autres, en vertu de la prop. 3, que les *systèmes fondamentaux de voisinages* de $x$ (I, p. 4, déf. 5).

2) Soit $X$ un ensemble non vide, préordonné *filtrant* pour une relation $(\sigma)$ (E, III, p. 12); pour tout élément $a \in X$, on appellera *section* de $X$ relative à l’élément $a$ l’ensemble $S(a)$ des $x \in X$ tels que $a(\sigma)x$. L’ensemble $\mathcal{G}$ des sections de $X$ est une *base de filtre*: il satisfait en effet à $(B_{II})$ de manière évidente; d’autre part, si $a, b$ sont deux éléments quelconques de $X$, il existe par hypothèse un élément $c \in X$ tel que $a(\sigma)c$ et $b(\sigma)c$, d’où $S(c) \subset S(a) \cap S(b)$, ce qui démontre $(B_I)$. Le filtre engendré par $\mathcal{G}$ est appelé le *filtre des sections* de l’ensemble filtrant $X$.

Par exemple, le *filtre de Fréchet* (I, p. 36) est le filtre des sections sur l’ensemble ordonné $\mathbf{N}$, considéré comme ensemble filtrant pour la relation $\leqslant$.

Soit maintenant $\mathcal{F}$ un filtre sur un ensemble $Z$; comme $\mathcal{F}$ est un ensemble filtrant pour la relation $\supset$ (en vertu de l’axiome $(\mathrm{F}_{\Pi})$), on peut définir sur $\mathcal{F}$ un *filtre des sections*, une section relative à un ensemble $A \in \mathcal{F}$ étant ici l’ensemble $S(A)$ des ensembles $M \in \mathcal{F}$ tels que $M \subset A$. Ce filtre est appelé le *filtre des sections du filtre* $\mathcal{F}$.

### 4. Ultrafiltres

#### Définition 4 {#top-i-s6-def-4 .statement}

*On appelle ultrafiltre sur un ensemble $X$ un filtre tel qu’il n’existe aucun filtre strictement plus fin que lui* (en d’autres termes, un élément *maximal* de l’ensemble ordonné des filtres sur $X$).

Comme l’ensemble ordonné des filtres sur $X$ est inductif (I, p. 37, cor. 3), le th. de Zorn (E, III, p. 20, th. 2) entraîne le théorème suivant:
**Théorème 1.** — *Pour tout filtre $\mathcal{F}$ sur un ensemble $X$, il existe un ultrafiltre plus fin que $\mathcal{F}$*.

#### Proposition 5 {#top-i-s6-prop-5 .statement}

*Soit $\mathcal{F}$ un ultrafiltre sur un ensemble $X$. Si $A$ et $B$ sont deux parties de $X$ telles que $A \cup B \in \mathcal{F}$, on a $A \in \mathcal{F}$ ou $B \in \mathcal{F}$*.

Raisonnons par l’absurde, et supposons que $A \notin \mathcal{F}$, $B \notin \mathcal{F}$ et $A \cup B \in \mathcal{F}$. Soit $\mathcal{G}$ l’ensemble des parties $M$ de $X$ telles que $A \cup M \in \mathcal{F}$. On vérifie immédiatement que $\mathcal{G}$ est un filtre sur $X$. Or $\mathcal{G}$ est strictement plus fin que $\mathcal{F}$, puisque $B \in \mathcal{G}$; mais ceci est en contradiction avec l’hypothèse que $\mathcal{F}$ est un ultrafiltre.

#### Corollaire {#top-i-s6-n4-cor-1 .statement}

*Si la réunion d’une suite finie $(A_i)_{1 \leq i \leq n}$ de parties de $X$ appartient à un ultrafiltre $\mathcal{F}$, l’un au moins des $A_i$ appartient à $\mathcal{F}$*.

Il suffit de raisonner par récurrence sur $n$.

En particulier, si $(A_i)_{1 \leq i \leq n}$ est un *recouvrement de $X$*, un au moins des $A_i$ appartient à $\mathcal{F}$.

La prop. 5 *caractérise* les ultrafiltres; plus généralement:

#### Proposition 6 {#top-i-s6-prop-6 .statement}

*Soit $\mathcal{G}$ un système générateur d’un filtre sur un ensemble $X$; si, pour toute partie $Y$ de $X$, on a $Y \in \mathcal{G}$ ou $\complement Y \in \mathcal{G}$, $\mathcal{G}$ est un ultrafiltre sur $X$*.

Soit en effet $\mathcal{F}$ un filtre contenant $\mathcal{G}$ (il en existe par hypothèse); $\mathcal{F}$ est identique à $\mathcal{G}$, car si $Y \in \mathcal{F}$, on a $\complement Y \notin \mathcal{F}$, donc $\complement Y \notin \mathcal{G}$, ce qui entraîne $Y \in \mathcal{G}$.

*Exemple d’ultrafiltre.* — L’ensemble des parties d’un ensemble non vide $X$ qui contiennent un élément $a \in X$ est un ultrafiltre; en effet, c’est un filtre et si $Y$ est une partie quelconque de $X$, on a $a \in Y$ ou $a \in \complement Y$. Ces ultrafiltres sont dits *triviaux*.

Le lecteur pourra observer qu’en dehors de cet exemple, nous ne démontrerons jamais l’existence d’un ultrafiltre (même sur un ensemble infini dénombrable) autrement que par le th. 1 (donc en utilisant l’axiome de choix).

#### Remarque {#top-i-s6-n4-rem-1 .statement}

Si $X$ est un ensemble contenant au moins deux éléments, il y a au moins deux ultrafiltres distincts sur $X$, donc l’ensemble ordonné des filtres sur $X$ n’a pas de plus grand élément.

#### Proposition 7 {#top-i-s6-prop-7 .statement}

*Tout filtre $\mathcal{F}$ sur un ensemble $X$ est l’intersection des ultrafiltres plus fins qui lui.*

Il est clair que cette intersection contient $\mathcal{F}$. D’autre part, soit $A$ un ensemble n’appartenant pas à $\mathcal{F}$, et posons $A' = \complement A$; comme $A$ ne contient aucun ensemble de $\mathcal{F}$, on a $M \cap A' \neq \varnothing$ pour tout $M \in \mathcal{F}$, et par suite (I, p. 37, cor. 1), il existe un filtre $\mathcal{F}'$ plus fin que $\mathcal{F}$ et contenant $A'$. Si $\mathcal{U}$ est un ultrafiltre plus fin que $\mathcal{F}'$ (I, p. 39, th. 1), on a donc $A \notin \mathcal{U}$, ce qui achève la démonstration.

### 5. Filtre induit

#### Proposition 8 {#top-i-s6-prop-8 .statement}

Soient $\mathcal{F}$ un filtre sur un ensemble $X$, $A$ une partie de $X$. Pour que la trace $\mathcal{F}_A$ de $\mathcal{F}$ sur $A$ soit un filtre sur $A$, il faut et il suffit que tout ensemble de $\mathcal{F}$ rencontre $A$.

En effet, la relation $(M \cap N) \cap A = (M \cap A) \cap (N \cap A)$ montre que $\mathcal{F}_A$ vérifie $(\mathrm{F}_{\mathrm{II}})$; de même, si $M \cap A \subset P \subset A$, on a $P = (M \cup P) \cap A$, donc $\mathcal{F}_A$ vérifie $(\mathrm{F}_1)$. Pour que $\mathcal{F}_A$ satisfasse à $(\mathrm{F}_{\mathrm{III}})$, il faut et il suffit que tout ensemble de $\mathcal{F}$ rencontre $A$, d’où la proposition.

En particulier, si $A \in \mathcal{F}$, $\mathcal{F}_A$ est un filtre sur $A$, d’après $(\mathrm{F}_{\mathrm{II}})$ et $(\mathrm{F}_{\mathrm{III}})$.

#### Définition 5 {#top-i-s6-def-5 .statement}

Si la trace, sur une partie $A$ d’un ensemble $X$, d’un filtre $\mathcal{F}$ sur $X$, est un filtre sur $A$, on dit que ce filtre est induit par $\mathcal{F}$ sur $A$.

Si un filtre $\mathcal{F}$ sur $X$ induit un filtre sur $A \subset X$, la trace sur $A$ d’une base de $\mathcal{F}$ est une base de $\mathcal{F}_A$ en vertu de la prop. 3 de I, p. 37.

#### Exemple {#top-i-s6-n5-exa-1 .statement}

Soient $X$ un espace topologique, $A$ une partie de $X$, $x$ un point de $X$; pour que la trace sur $A$ du filtre des voisinages de $x$ soit un filtre sur $A$, il faut et il suffit que tout voisinage de $x$ rencontre $A$, autrement dit (I, p. 7, déf. 10) que $x$ soit adhérent à $A$.

Ce qui fait l’intérêt de cet exemple de filtre induit, c’est d’une part qu’il joue un rôle important dans la théorie des limites (I, p. 50), et d’autre part que tout filtre peut être défini de cette manière. En effet, soit $\mathcal{F}$ un filtre sur un ensemble $X$; soit $X'$ l’ensemble obtenu en adjoignant à $X$ un nouvel élément $\omega$, $X$ étant identifié au complémentaire de $\{\omega\}$ dans $X'$ (E, II, p. 30); soit $\mathcal{F}'$ le filtre sur $X'$ formé des ensembles $M \cup \{\omega\}$, où $M$ parcourt $\mathcal{F}$. Pour tout point $x \neq \omega$ de $X'$, soit $\mathcal{V}(x)$ l’ensemble des parties de $X'$ contenant $x$; posons d’autre part $\mathcal{V}(\omega) = \mathcal{F}'$; les $\mathcal{V}(x)$, pour $x \in X'$, satisfont visiblement aux axiomes $(\mathrm{V}_1)$, $(\mathrm{V}_\mathrm{II})$, $(\mathrm{V}_\mathrm{III})$, et $(\mathrm{V}_\mathrm{IV})$, donc définissent sur $X'$ une topologie dont ils sont les filtres de voisinages; enfin $\omega$ est adhérent à $X$ pour cette topologie et $\mathcal{F}$ est induit par $\mathcal{F}' = \mathcal{V}(\omega)$ sur $X$. La topologie ainsi définie sur $X'$ (resp. l’ensemble $X'$ muni de cette topologie) s’appelle topologie associée (resp. espace topologique associé) à $\mathcal{F}$.

#### Proposition 9 {#top-i-s6-prop-9 .statement}

Pour qu’un ultrafiltre $\mathcal{U}$ sur un ensemble $X$ induise un filtre sur une partie $A$ de $X$, il faut et il suffit que $A \in \mathcal{U}$; si cette condition est remplie, $\mathcal{U}_A$ est un ultrafiltre sur $A$.

C’est une conséquence immédiate des prop. 5 et 6 (I, p. 39).

### 6. Image directe et image réciproque d’une base de filtre

Soit $\mathcal{B}$ une base de filtre sur un ensemble $X$, et soit $f$ une application de $X$ dans un ensemble $X'$; $f(\mathcal{B})$ est une base de filtre sur $X'$, car la relation $M \neq \varnothing$ entraîne f(M) \neq \varnothing, et on a $f(M \cap N) \subset f(M) \cap f(N)$. Si $\mathfrak{B}_1$ est une base d’un filtre *plus fin* que le filtre de base $\mathfrak{B}$, $f(\mathfrak{B}_1)$ est une base d’un filtre *plus fin* que le filtre de base $f(\mathfrak{B})$ (I, p. 38, prop. 4).

#### Proposition 10 {#top-i-s6-prop-10 .statement}

*Si $\mathfrak{B}$ est une base d’ultrafiltre sur un ensemble $X$, $f$ une application de $X$ dans $X'$, $f(\mathfrak{B})$ est une base d’ultrafiltre sur $X'$.*

Soit en effet $M'$ une partie de $X'$; si $f^{-1}(M')$ contient un ensemble $M$ de $\mathfrak{B}$, $M'$ contient $f(M)$; sinon, $\complement f^{-1}(M') = f^{-1}(\complement M')$ contient un ensemble $N$ de $\mathfrak{B}$ (I, p. 39, prop. 5), donc $\complement M'$ contient $f(N)$. La proposition résulte par suite de la prop. 6 de I, p. 39.

Considérons en particulier le cas où $f$ est l’injection canonique $A \to X$ d’une partie $A$ d’un ensemble $X$. Si $\mathfrak{B}$ est une base de filtre sur $A$, $f(\mathfrak{B})$ est une base de filtre sur $X$. On dit que le filtre $\mathfrak{F}$ sur $X$ engendré par $f(\mathfrak{B})$ est le *filtre engendré par $\mathfrak{B}$, lorsqu’on considère $\mathfrak{B}$ comme base de filtre sur $X$*. Si $\mathfrak{B}$ est une *base d’ultrafiltre sur $A$*, c’est aussi une *base d’ultrafiltre sur $X$*, en vertu de la prop. 10.

Examinons maintenant si l’*image réciproque* d’une base de filtre est une base de filtre. Soit $\mathfrak{B}'$ une base de filtre sur un ensemble $X'$, et soit $f$ une application de $X$ dans $X'$; pour que $f^{-1}(\mathfrak{B}')$ soit une base de filtre sur $X$, *il faut et il suffit que* $f^{-1}(M') \neq \varnothing$ *pour tout* $M' \in \mathfrak{B}'$, comme il résulte aussitôt de la relation

$$
f^{-1}(M' \cap N') = f^{-1}(M') \cap f^{-1}(N')
$$

et de la déf. 3 de I, p. 38. Cette condition peut aussi s’exprimer en disant que *tout ensemble de $\mathfrak{B}'$ rencontre $f(X)$* (ou encore que la trace de $\mathfrak{B}'$ sur $f(X)$ est une base de filtre). On notera que si elle est remplie, $f(f^{-1}(\mathfrak{B}'))$ est une base d’un filtre *plus fin* que le filtre de base $\mathfrak{B}'$.

Si $\mathfrak{B}$ est une base de filtre sur $X$, il est clair que la condition précédente est remplie par $\mathfrak{B}' = f(\mathfrak{B}); f^{-1}(f(\mathfrak{B}))$ est alors une base d’un filtre *moins fin* que le filtre de base $\mathfrak{B}$.

Soient $A$ une partie d’un ensemble $X$, $\varphi$ l’injection canonique $A \to X$; si $\mathfrak{B}$ est une base de filtre sur $X$, $\varphi^{-1}(\mathfrak{B})$ n’est autre que $\mathfrak{B}_A$; en exprimant, à l’aide de la condition précédente, que c’est une base de filtre sur $A$, on retrouve une partie de la prop. 8 de I, p. 40.

### 7. Produit de filtres

Soit $(X_i)_{i \in I}$ une famille d’ensembles, et pour chaque indice $i \in I$, soit $\mathfrak{B}_i$ une *base de filtre* sur $X_i$. Soit $\mathfrak{B}$ l’ensemble des parties de l’ensemble produit $X = \prod_{i \in I} X_i$, qui sont de la forme $\prod_{i \in I} M_i$, où $M_i = X_i$ sauf pour un nombre fini d’indices et où $M_i \in \mathcal{B}_i$ pour tout $i$ tel que $M_i \neq X_i$. En vertu de la formule
$$
(\prod_{i \in I} M_i) \cap (\prod_{i \in I} N_i) = \prod_{i \in I} (M_i \cap N_i),
$$
il est immédiat que $\mathcal{B}$ est une base de filtre sur $X$. On notera que le filtre de base $\mathcal{B}$ est aussi engendré par les ensembles $\operatorname{pr}_k^{-1}(M_k)$, où $M_k \in \mathcal{B}_k$ et où $k$ parcourt $I$, puisque $\operatorname{pr}_k^{-1}(M_k) = M_k \times \prod_{i \neq k} X_i$.

#### Définition 6 {#top-i-s6-def-6 .statement}

Étant donné un filtre $\mathcal{F}_i$ sur chacun des ensembles $X_i$ d’une famille $(X_i)_{i \in I}$ on appelle produit des filtres $\mathcal{F}_i$ et on note $\prod_{i \in I} \mathcal{F}_i$ (si aucune confusion n’en résulte) le filtre sur $X = \prod_{i \in I} X_i$ ayant pour base l’ensemble des parties de la forme $\prod_{i \in I} M_i$, où $M_i \in \mathcal{F}_i$ pour tout $i \in I$ et $M_i = X_i$ sauf pour un nombre fini d’indices.

Le lecteur vérifiera aisément que le filtre produit des $\mathcal{F}_i$ peut encore être défini comme le moins fin des filtres $\mathcal{G}$ sur $X$ tels que $\operatorname{pr}_i(\mathcal{G}) = \mathcal{F}_i$ pour tout $i \in I$.

Les remarques précédentes montrent que si, pour tout $i \in I$, $\mathcal{B}_i$ est une base de $\mathcal{F}_i$, $\mathcal{B}$ est une base du filtre produit $\prod_{i \in I} \mathcal{F}_i$ (I, p. 38, prop. 3).

Sur un produit $X = \prod_{i \in I} X_i$ d’espaces topologiques, le filtre des voisinages d’un point quelconque $x = (x_i)$ est le produit des filtres des voisinages des points $x_i$ (I, p. 24).

La construction d’un filtre produit $\mathcal{F} = \prod_{i \in I} \mathcal{F}_i$ se simplifie lorsque l’ensemble d’indices $I$ est fini : une base de $\mathcal{F}$ est alors formée de tous les produits $\prod_{i \in I} M_i$, où $M_i \in \mathcal{F}_i$ pour tout $i \in I$. Si $I = \{1, 2, \ldots, n\}$ on écrit $\mathcal{F}_1 \times \mathcal{F}_2 \times \cdots \times \mathcal{F}_n$ au lieu de $\prod_{i \in I} \mathcal{F}_i$.

### 8. Filtres élémentaires

#### Définition 7 {#top-i-s6-def-7 .statement}

Soit $(x_n)_{n \in \mathbf{N}}$ une suite infinie d’éléments d’un ensemble $X$; on appelle filtre élémentaire associé à la suite $(x_n)$ le filtre engendré par l’image du filtre de Fréchet (I, p. 36) par l’application $n \mapsto x_n$ de $\mathbf{N}$ dans $X$.

Il revient au même de dire que le filtre élémentaire associé à $(x_n)$ est l’ensemble des parties $M$ de $X$ telles que l’on ait $x_n \in M$ sauf pour un nombre fini de valeurs de $n$. Si $S_n$ désigne l’ensemble des $x_p$ tels que $p \geq n$, les ensembles $S_n$ forment une base du filtre élémentaire associé à la suite $(x_n)$.

Le filtre élémentaire associé à une suite infinie extraite d’une suite $(x_n)$ est plus fin que le filtre élémentaire associé à $(x_n)$ (cf. I, p. 98, exerc. 15).

Tout filtre élémentaire possède par définition une base dénombrable. Inversement:

#### Proposition 11 {#top-i-s6-prop-11 .statement}

Si un filtre $\mathcal{F}$ possède une base dénombrable, il est le filtre intersection des filtres élémentaires plus fins que $\mathcal{F}$.

En effet, rangeons la base dénombrable de $\mathcal{F}$ en une suite $(A_n)_{n \in \mathbf{N}}$; si on pose $B_n = \bigcap_{p=0}^n A_p$, les $B_n$ forment encore une base de $\mathcal{F}$ (I, p. 38, prop. 3) et on a $B_{n+1} \subset B_n$ pour tout $n$. Soit $a_n$ un élément quelconque de $B_n$; il est clair que $\mathcal{F}$ est moins fin que le filtre associé à $(a_n)$. Le filtre intersection $\mathfrak{J}$ des filtres élémentaires plus fins que $\mathcal{F}$ existe donc et est évidemment plus fin que $\mathcal{F}$; s’il était strictement plus fin, il existerait un ensemble $M \in \mathfrak{J}$ tel que $B_n \cap \complement M \neq \varnothing$ pour tout $n$; si $b_n$ est un élément de $B_n \cap \complement M$, le filtre associé à la suite $(b_n)$ serait plus fin que $\mathcal{F}$ et $M$ n’appartiendrait pas à ce filtre, contrairement à la définition de $\mathfrak{J}$.

#### Remarque {#top-i-s6-n8-rem-1 .statement}

Un filtre moins fin qu’un filtre à base dénombrable peut fort bien ne pas posséder de base dénombrable; par exemple, si $X$ est un ensemble infini non dénombrable, le filtre des complémentaires des parties finies de $X$ n’a pas de base dénombrable (sans quoi l’ensemble des parties finies de $X$ serait dénombrable, ce qui est contraire à l’hypothèse); toutefois ce filtre est moins fin que tout filtre élémentaire associé à une suite infinie dont les termes sont distincts.

### 9. Germes suivant un filtre

Soit $\mathcal{F}$ un filtre sur un ensemble $X$. Dans l’ensemble $\mathfrak{P}(X)$ des parties de $X$, la relation

« il existe $V \in \mathcal{F}$ tel que $M \cap V = N \cap V$ »

entre $M$ et $N$ est une relation d’équivalence $R$, car elle est évidemment réflexive et symétrique, et si $M, N, P$ sont trois parties de $X$ telles que $M \cap V = N \cap V$ et $N \cap W = P \cap W$ pour deux ensembles $V, W$ de $\mathcal{F}$, on en conclut que $M \cap (V \cap W) = N \cap (V \cap W) = P \cap (V \cap W)$ et l’on a $V \cap W \in \mathcal{F}$, d’où la transitivité de $R$. On dit que la classe mod. $R$ d’une partie $M$ de $X$ est le germe de $M$ suivant $\mathcal{F}$; l’ensemble quotient $\mathfrak{P}(X)/R$ est appelé l’ensemble des germes de parties de $X$ (suivant $\mathcal{F}$).

Les applications $(M, N) \mapsto M \cap N$ et $(M, N) \mapsto M \cup N$ de $\mathfrak{P}(X) \times \mathfrak{P}(X)$ dans $\mathfrak{P}(X)$ sont compatibles avec les relations d’équivalence $R \times R$ et $R$ (E, II, p. 44). En effet, si $M \equiv M'$ (mod. $R$) et $N \equiv N'$ (mod. $R$), il existe $V$ et $W$ dans $\mathcal{F}$ tels que $M \cap V = M' \cap V$ et $N \cap W = N' \cap W$, d’où

$$
(M \cap N) \cap (V \cap W) = (M' \cap N') \cap (V \cap W)
$$

et

$$
(M \cup N) \cap (V \cap W) = (M \cap (V \cap W)) \cup (N \cap (V \cap W)) \\
= (M' \cap (V \cap W)) \cup (N' \cap (V \cap W)) = (M' \cup N') \cap (V \cap W).
$$

Par passage aux quotients, on déduit de ces applications deux applications notées (par abus de langage) $(\xi, \eta) \mapsto \xi \cap \eta$ et $(\xi, \eta) \mapsto \xi \cup \eta$ de $(\mathfrak{P}(X)/R) \times (\mathfrak{P}(X)/R)$ dans $\mathfrak{P}(X)/R$. On vérifie immédiatement que pour ces lois de composition tout élément est idempotent, et que ces lois sont commutatives, associatives et distributives l’une par rapport à l’autre. En outre, les relations $\xi = \xi \cap \eta$ et $\eta = \xi \cup \eta$ sont équivalentes; si on les écrit (par abus de langage) $\xi \subset \eta$, on vérifie aisément que cette relation est une relation d’ordre sur $\mathfrak{P}(X)/R$, pour laquelle cet ensemble est réticulé, admet le germe de $\varnothing$ pour plus petit élément et le germe de $X$ pour plus grand élément; on notera d’ailleurs que la relation $\xi \subset \eta$ signifie qu’il existe $M \in \xi, N \in \eta$ et $V \in \mathfrak{F}$ tels que $M \cap V \subset N \cap V$.

Soit maintenant $X'$ un second ensemble, et désignons par $\Phi$ l’ensemble des applications dont l’ensemble de départ est une partie de $X$ appartenant à $\mathfrak{F}$ et dont $X'$ est l’ensemble d’arrivée. Dans $\Phi$, la relation

« il existe $V \in \mathfrak{F}$ tel que $f$ et $g$ soient définies et coïncident dans $V$ »

entre $f$ et $g$ est une *relation d’équivalence* $S$, car elle est évidemment réflexive et symétrique; de plus, elle est transitive, car si $f$ et $g$ sont définies et coïncident dans $V \in \mathfrak{F}$, et si $g$ et $h$ sont définies et coïncident dans $W \in \mathfrak{F}$, alors $f$ et $h$ sont définies et coïncident dans $V \cap W \in \mathfrak{F}$. On dit que la classe mod. $S$ d’une application $f$ d’un ensemble $V \in \mathfrak{F}$ dans $X'$ est le *germe de $f$ (suivant $\mathfrak{F}$)* , et l’ensemble quotient $\tilde{\Phi} = \Phi/S$ est appelé l’*ensemble des germes d’applications de $X$ dans $X'$ (suivant $\mathfrak{F}$)*.

#### Remarque 1 {#top-i-s6-n9-rem-1 .statement}

Toute application $f$ d’une partie $M \in \mathfrak{F}$ de $X$ dans $X'$ est équivalente mod. $S$ à une application $f_1$ de $X$ dans $X'$ (ce qui justifie la terminologie précédente): il suffit en effet de prolonger $f$ à $X$ en lui donnant par exemple une valeur constante dans $X - M$.

#### Remarque 2 {#top-i-s6-n9-rem-2 .statement}

Pour que les *fonctions caractéristiques* $\varphi_M$ et $\varphi_N$ de deux parties $M, N$ de $X$ aient même germe suivant $\mathfrak{F}$, il faut et il suffit que les parties $M$ et $N$ aient même germe suivant $\mathfrak{F}$.

Soient $X''$ un troisième ensemble, $\varphi$ une application de $X'$ dans $X''$, $\Phi'$ l’ensemble des applications dont l’ensemble de départ est une partie de $X$ appartenant à $\mathfrak{F}$ et dont $X''$ est l’ensemble d’arrivée. Pour toute application $f \in \Phi$, $\varphi \circ f$ appartient à $\Phi'$; en outre, il est immédiat que si $g \in \Phi$ a même germe que $f$ suivant $\mathfrak{F}$, $\varphi \circ f$ et $\varphi \circ g$ ont même germe suivant $\mathfrak{F}$; ce germe ne dépend donc que du germe $\tilde{f}$ de $f$ suivant $\mathfrak{F}$ et se note $\varphi(\tilde{f})$. On définit ainsi une application (encore notée $\varphi$ par abus de langage) de l’ensemble $\tilde{\Phi}$ des germes d’applications de $X$ dans $X'$, dans l’ensemble $\tilde{\Phi}'$ des germes d’applications de $X$ dans $X''$.

Soient maintenant $X'_i$ ($1 \leq i \leq n$) des ensembles, $Y = \prod_{i=1}^n X'_i$ leur produit; désignons par $\Phi_i$ (resp. $\Phi$) l’ensemble des applications dont l’ensemble de départ est une partie appartenant à $\mathfrak{F}$ et dont $X'_i$ (resp. $Y$) est l’ensemble d’arrivée. Si $f_i \in \Phi_i$ pour $1 \leq i \leq n$ et si $M_i \in \mathfrak{F}$ est l’ensemble de départ de $f_i$, l’application t \mapsto (f_1(t), \ldots, f_n(t)) est définie dans \bigcap_{i=1}^n M_i et appartient donc à $\Phi$; nous la désignerons (par abus de langage) par $(f_1, \ldots, f_n)$. En outre, si $f_i$ et $g_i$ appartiennent à $\Phi_i$ et ont même germe suivant $\mathcal{F}$ (pour $1 \leq i \leq n$), il est immédiat que $(f_1, \ldots, f_n)$ et $(g_1, \ldots, g_n)$ ont même germe suivant $\mathcal{F}$; ce germe ne dépend donc que des germes $\tilde{f}_i$ des $f_i$. Si on le désigne par $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$, il est immédiat que $\Gamma$ est une bijection de l’ensemble produit $\prod_{i=1}^n \tilde{\Phi}_i$ sur l’ensemble $\tilde{\Phi}$, en désignant par $\tilde{\Phi}_i$ (resp. $\tilde{\Phi}$) l’ensemble des germes suivant $\mathcal{F}$ des applications de X dans $X'_i$ (resp. dans Y); aussi, par abus de langage, écrit-on d’ordinaire $(\tilde{f}_1, \ldots, \tilde{f}_n)$ au lieu de $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ s’il n’en résulte pas de confusion.

D’après ce qui précède, toute application $\psi$ de Y dans un ensemble $X''$ définit donc une application $(\tilde{f}_1, \ldots, \tilde{f}_n) \mapsto \psi(\tilde{f}_1, \ldots, \tilde{f}_n)$ de $\prod_{i=1}^n \tilde{\Phi}_i$ dans l’ensemble $\tilde{\Phi}'$ des germes des applications de X dans $X''$.

En particulier, si $I = \{1, 2\}$ et si $X'_1, X'_2$ et $X''$ sont tous égaux à un même ensemble $X'$ (de sorte que $\psi$ est une loi de composition sur $X'$) on déduit de $\psi$ une loi de composition sur l’ensemble $\tilde{\Phi}$ des germes d’applications de X dans $X'$. On vérifie aussitôt que si la loi donnée sur $X'$ est associative (resp. commutative), il en est de même de la loi correspondante sur $\tilde{\Phi}$; si la loi $\psi$ sur $X'$ admet un élément neutre $e'$, le germe suivant $\mathcal{F}$ de l’application constante $x \mapsto e'$ est élément neutre pour la loi correspondante sur $\tilde{\Phi}$. Enfin, lorsque $X'$ admet un élément neutre $e'$, pour que le germe $\tilde{f}$ d’un élément $f \in \Phi$ soit inversible dans $\tilde{\Phi}$, il faut et il suffit qu’il existe $V \in \mathcal{F}$, contenu dans l’ensemble de départ de $f$, et tel que $f(t)$ soit inversible dans $X'$ pour tout $t \in V$; si, pour tout $t \in V$, on note $g(t)$ l’inverse de $f(t)$, le germe $\tilde{g}$ de $g$ est alors l’inverse de $\tilde{f}$ dans $\tilde{\Phi}$. En particulier, si $X'$ est un groupe pour la loi $\psi$, $\tilde{\Phi}$ est un groupe pour la loi correspondante; on prouve de même que si $X'$ est un anneau (resp. une algèbre sur un anneau A), $\tilde{\Phi}$ est un anneau (resp. une algèbre sur A) pour les lois de composition correspondantes.

### 10. Germes en un point

Un des cas les plus fréquents où s’appliquent les définitions et résultats du n° 9 est celui où $\mathcal{F}$ est le filtre des voisinages d’un point $a$ d’un espace topologique X; on parle alors de « germes au point $a$ » au lieu de « germes suivant $\mathcal{F}$ ». On notera qu’il n’existe alors qu’un seul germe de voisinages du point $a$, celui de l’espace X tout entier. Les germes d’ensembles fermés sont identiques aux germes d’ensembles localement fermés au point $a$, car si L est localement fermé au point $a$, les germes de L et de $\overline{L}$ au point $a$ sont égaux (I, p. 18, prop. 1). On en conclut que si $\xi, \eta$ sont deux germes d’ensembles localement fermés au point $a$, $\xi \cup \eta$ et $\xi \cap \eta$ sont aussi de tels germes.

Comme $a$ appartient à tout ensemble $V \in \mathcal{F}, f(a)$ est défini pour toute application $f$ dont l’ensemble de départ appartient à $\mathcal{F}$; en outre, si $f$ et $g$ ont même germe au point $a$, on a nécessairement $f(a) = g(a)$, donc $f(a)$ ne dépend que du germe $\tilde{f}$ de $f$ au point $a$; on dit que c’est la valeur de $\tilde{f}$ au point $a$ et on la note $\tilde{f}(a)$. On notera que la relation $\tilde{f}(a) = \tilde{g}(a)$ n’entraîne nullement $\tilde{f} = \tilde{g}$ en général.

Soient $X', X''$ deux espaces topologiques, $b$ un point de $X'$, $g, g'$ deux applications de $X'$ dans $X''$ ayant même germe au point $b$. Si $f, f'$ sont deux applications de $X$ dans $X'$, continues au point $a$, ayant même germe en ce point et telles que $f(a) = b, g \circ f$ et $g' \circ f'$ ont même germe au point $a$: en effet, si $V'$ est un voisinage de $b$ tel que $g(x') = g'(x')$ dans $V'$, il existe un voisinage $V$ de $a$ tel que $f(V) \subset V'$, $f'(V) \subset V'$ et $f(x) = f'(x)$ dans $V$, d’où notre assertion. Le germe de $g \circ f$ au point $a$ est alors appelé le composé des germes $\tilde{g}$ et $\tilde{f}$ de $g$ et de $f$ et se note $\tilde{g} \circ \tilde{f}$.

## EXERCICES {#top-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
