---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 1
section_title: Structures et isomorphismes
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0204-0214, 0231-0231
extraction: ocr
subsections:
    - "no": 1
      title: Échelons
      page: 0
      pdf_page: 204
    - "no": 2
      title: Extensions canoniques d'applications
      page: 2
      pdf_page: 205
    - "no": 3
      title: Relations transportables
      page: 3
      pdf_page: 206
    - "no": 4
      title: Espèces de structure
      page: 4
      pdf_page: 207
    - "no": 5
      title: Isomorphismes et transport de structures
      page: 6
      pdf_page: 209
    - "no": 6
      title: Déduction de structures
      page: 7
      pdf_page: 210
    - "no": 7
      title: Espèces de structure équivalentes
      page: 9
      pdf_page: 212
statements: 13
exercises: 1
content_sha256: 77b678bb39afcc800fea9d978ec3de7dfb020b87bf54133f0928865219092200
---

## § 1. STRUCTURES ET ISOMORPHISMES

Le but de ce chapitre est de décrire une fois pour toutes un certain nombre de constructions formatives et de démonstrations (cf. I, p. 17 et p. 22) qui interviennent très fréquemment en mathématique.

### 1. Échelons

Un schéma de construction d’échelon est une suite $c_1, c_2, \ldots, c_m$ de couples d’entiers naturels$^1$ $c_i = (a_i, b_i)$ satisfaisant aux conditions suivantes:

a) Si $b_i = 0$, on a $1 \leq a_i \leq i - 1$.

b) Si $a_i \neq 0$ et $b_i \neq 0$, on a $1 \leq a_i \leq i - 1$ et $1 \leq b_i \leq i - 1$.

Ces conditions entraînent que $c_1 = (0, b_1)$ avec $b_1 > 0$. Si $n$ est le plus grand des entiers $b_i$ figurant dans les couples $(0, b_i)$, on dit que $c_1, c_2, \ldots, c_m$ est un schéma de construction d’échelon sur $n$ termes.

Étant donnés un schéma $S = (c_1, c_2, \ldots, c_m)$ de construction d’échelon sur $n$ termes, et $n$ termes $E_1, \ldots, E_n$ d’une théorie $\mathcal{T}$ plus forte que la théorie des ensembles, on appelle construction d’échelon, de schéma $S$, sur $E_1, \ldots, E_n$, une suite $A_1, A_2, \ldots, A_m$ de $m$ termes de $\mathcal{T}$ définis de proche en proche par les conditions suivantes:

a) Si $c_i = (0, b_i)$, $A_i$ est le terme $E_{b_i}$.

b) Si $c_i = (a_i, 0)$, $A_i$ est le terme $\mathfrak{B}(A_{a_i})$.

c) Si $c_i = (a_i, b_i)$ avec $a_i \neq 0$ et $b_i \neq 0$, $A_i$ est le terme $A_{a_i} \times A_{b_i}$.

1 Nous utilisons la notion d’« entier » de la même façon qu’au chap. I, c’est-à-dire au sens métamathématique de repères rangés dans un certain ordre; cet emploi n’a rien de commun avec la théorie mathématique des entiers, développée au chap. III.

Nous dirons que le dernier terme $A_m$ de la construction d'échelon de schéma S sur $E_1, \ldots, E_n$ est l'échelon de schéma S sur les ensembles de base $E_1, \ldots, E_n$, et nous le désignerons, dans les raisonnements généraux qui vont suivre, par la notation $S(E_1, \ldots, E_n)$.

#### Exemple {#ens-iv-s1-n1-exa-1 .statement tag=03V4}

Étant donnés deux ensembles E, F, l'ensemble $\mathfrak{P}(\mathfrak{P}(E)) \times \mathfrak{P}(F)$ est un échelon sur E, F, de schéma
$$
(0, 1), \quad (0, 2), \quad (1, 0), \quad (3, 0), \quad (2, 0), \quad (4, 5).
$$
C'est aussi l'échelon sur E, F, de schéma
$$
(0, 2), \quad (0, 1), \quad (1, 0), \quad (2, 0), \quad (4, 0), \quad (5, 3).
$$
Plusieurs schémas distincts peuvent donc donner le même échelon sur les mêmes termes.

### 2. Extensions canoniques d'applications

Soit $S = (c_1, c_2, \ldots, c_m)$ un schéma de construction d'échelon sur n termes. Soient $E_1, \ldots, E_n, E'_1, \ldots, E'_n$ des ensembles (termes de $\mathcal{T}$) et soient $f_1, \ldots, f_n$ des termes de $\mathcal{T}$ tels que les relations

« $f_i$ est une application de $E_i$ dans $E'_i$ »

soient des théorèmes de $\mathcal{T}$ pour $1 \leq i \leq n$. Soit $A_1, \ldots, A_m$ (resp. $A'_1, \ldots, A'_m$) la construction d'échelon de schéma S sur $E_1, \ldots, E_n$ (resp. $E'_1, \ldots, E'_n$). On définit de proche en proche une suite de m termes $g_1, \ldots, g_m$ telle que $g_i$ soit une application de $A_i$ dans $A'_i$ (pour $1 \leq i \leq m$), par les conditions suivantes:

a) Si $c_i = (0, b_i)$, de sorte que $A_i = E_{b_i}, A'_i = E'_{b_i}$, $g_i$ est l'application $f_{b_i}$.

b) Si $c_i = (a_i, 0)$, de sorte que $A_i = \mathfrak{P}(A_{a_i}), A'_i = \mathfrak{P}(A'_{a_i})$, $g_i$ est l'extension canonique $\hat{g}_{a_i}$ de $g_{a_i}$ aux ensembles de parties (II, p. 30).

c) Si $c_i = (a_i, b_i)$ avec $a_i \neq 0$ et $b_i \neq 0$, de sorte que $A_i = A_{a_i} \times A_{b_i}$ et $A'_i = A'_{a_i} \times A'_{b_i}$, $g_i$ est l'extension canonique $g_{a_i} \times g_{b_i}$ de $g_{a_i}$ et $g_{b_i}$ à $A_{a_i} \times A_{b_i}$ (II, p. 21).

Nous dirons que le dernier terme $g_m$ de cette suite est l'extension canonique, de schéma S, des applications $f_1, \ldots, f_n$, et nous le désignerons par la notation $\langle f_1, \ldots, f_n \rangle^S$.

On vérifie de proche en proche les critères suivants:

CST1. Si $f_i$ est une application de $E_i$ dans $E'_i$, $f'_i$ une application de $E'_i$ dans $E''_i$ ($1 \leq i \leq n$), on a, pour tout schéma de construction d'échelon S sur n termes
$$
\langle f'_1 \circ f_1, f'_2 \circ f_2, \ldots, f'_n \circ f_n \rangle^S = \langle f'_1, f'_2, \ldots, f'_n \rangle^S \circ \langle f_1, f_2, \ldots, f_n \rangle^S.
$$

CST2. Si $f_i$ est injective (resp. surjective) pour $1 \leq i \leq n$, $\langle f_1, \ldots, f_n \rangle^S$ est injective (resp. surjective).

Ce dernier critère résulte des propriétés correspondantes de l'extension $\hat{g}$ (II, p. 30, prop. 1) et de l'extension $g \times h$ (II, p. 21).

CST3. Si $f_i$ est une bijection de $E_i$ sur $E'_i$, et $f_i^{-1}$ la bijection réciproque,$^1$ alors $\langle f_1, \ldots, f_n \rangle^S$ est une bijection, et $\langle f_1^{-1}, \ldots, f_n^{-1} \rangle^S$ la bijection réciproque; autrement dit, on a
$$
(\langle f_1, \ldots, f_n \rangle^S)^{-1} = \langle f_1^{-1}, \ldots, f_n^{-1} \rangle^S.
$$
Cela résulte aussitôt de CST1 et CST2.

### 3. Relations transportables

Soient $\mathcal{T}$ une théorie plus forte que la théorie des ensembles, $x_1, \ldots, x_n, s_1, \ldots, s_p$ des lettres distinctes entre elles et distinctes des constantes de $\mathcal{T}$, $A_1, \ldots, A_m$ des termes de $\mathcal{T}$ où ne figurent aucune des lettres $x_i$ ($1 \leq i \leq n$) et $s_j$ ($1 \leq j \leq p$). Soient $S_1, \ldots, S_p$ des schémas de construction d’échelon sur $n + m$ termes: nous dirons que la relation $T \{ x_1, \ldots, x_n, s_1, \ldots, s_p \}$:
$$
\text{« } s_1 \in S_1(x_1, \ldots, x_n, A_1, \ldots, A_m) \text{ et } s_2 \in S_2(x_1, \ldots, x_n, A_1, \ldots, A_m)
$$
et ... et $s_p \in S_p(x_1, \ldots, x_n, A_1, \ldots, A_m) \text{ »}$
est une typification des lettres $s_1, \ldots, s_p$.

Soit $R \{ x_1, \ldots, x_n, s_1, \ldots, s_p \}$ une relation de $\mathcal{T}$, contenant certaines des lettres $x_i, s_j$ (et éventuellement d’autres lettres). Dire que $R$ est transportable (dans $\mathcal{T}$) pour la typification $T$, les $x_i$ ($1 \leq i \leq n$) étant considérés comme ensembles de base principaux et les $A_h$ ($1 \leq h \leq m$) comme ensembles de base auxiliaires, c’est dire que la condition suivante est satisfaite:

Soient $y_1, \ldots, y_n, f_1, \ldots, f_n$ des lettres distinctes entre elles, distinctes des $x_i$ ($1 \leq i \leq n$), des $s_j$ ($1 \leq j \leq p$), des constantes de $\mathcal{T}$ et de toutes les lettres figurant dans $R$ ou dans les $A_h$ ($1 \leq h \leq m$). Soit d’autre part $\mathrm{Id}_h$ ($1 \leq h \leq m$) l’application identique de $A_h$ sur lui-même. Alors, la relation
(1) « $T \{ x_1, \ldots, x_n, s_1, \ldots, s_p \}$ et ($f_1$ est une bijection de $x_1$ sur $y_1$)
et ... et ($f_n$ est une bijection de $x_n$ sur $y_n$) »
entraîne, dans $\mathcal{T}$, la relation
(2) $R \{ x_1, \ldots, x_n, s_1, \ldots, s_p \} \Leftrightarrow R \{ y_1, \ldots, y_n, s'_1, \ldots, s'_p \}$
où on a posé
(3) $s'_j = \langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{S_j}(s_j) \quad (1 \leq j \leq p)$.
On a une définition analogue, mais plus simple, lorsqu’il n’y a pas d’ensemble auxiliaire.

Par exemple, si $n = p = 2$, et si la typification $T$ est
$$
\text{« } s_1 \in x_1 \text{ et } s_2 \in x_1 \text{ »,}
$$
la relation $s_1 = s_2$ est transportable. Par contre, la relation $x_1 = x_2$ ne l’est pas. On reconnaît aisément, dans les cas usuels, si une relation est transportable (pour une certaine typification).

$^1$ Pour des raisons de commodité typographique, nous écrivons $f^{-1}$ au lieu de $f^{-1}$.

### 4. Espèces de structure

Soit $\mathcal{T}$ une théorie plus forte que la théorie des ensembles. Une espèce de structure dans $\mathcal{T}$ est un texte $\Sigma$ formé des assemblages suivants:

1° Un certain nombre de lettres $x_1, \ldots, x_n, s$, distinctes entre elles et distinctes des constantes de $\mathcal{T}$; $x_1, \ldots, x_n$ sont appelées les ensembles de base principaux de l’espèce de structure $\Sigma$.

2° Un certain nombre de termes $A_1, \ldots, A_m$ de $\mathcal{T}$, dans lesquels ne figurent aucune des lettres $x_i, s$, et qui sont appelés les ensembles de base auxiliaires de $\Sigma$; $\Sigma$ peut éventuellement ne comporter aucun ensemble de base auxiliaire (mais il doit toujours y avoir au moins un ensemble de base principal).

3° Une typification $T\{x_1, x_2, \ldots, x_n, s\}$:
$$
s \in S(x_1, \ldots, x_n, A_1, \ldots, A_m)
$$
où $S$ est un schéma de construction d’échelon sur $n + m$ termes (IV, p. 1). On dit que $T\{x_1, \ldots, x_n, s\}$ est la caractérisation typique de l’espèce de structure $\Sigma$.

4° Une relation $R\{x_1, \ldots, x_n, s\}$ qui est transportable (dans $\mathcal{T}$) pour la typification, les $x_i$ étant ensembles de base principaux et les $A_j$ ensembles de base auxiliaires (IV, p. 3). On dit que $R$ est l’axiome de l’espèce de structure $\Sigma$.

On appelle théorie de l’espèce de structure $\Sigma$ la théorie $\mathcal{T}_\Sigma$ ayant les mêmes schémas d’axiomes que $\mathcal{T}$ et dont les axiomes explicites sont ceux de $\mathcal{T}$ et l’axiome « T et R »; les constantes de $\mathcal{T}_\Sigma$ sont donc les constantes de $\mathcal{T}$ et les lettres figurant dans T ou dans R.

Soit maintenant $\mathcal{T}'$ une théorie plus forte que $\mathcal{T}$, et soient $E_1, \ldots, E_n, U$ des termes de $\mathcal{T}'$. On dit que (dans la théorie $\mathcal{T}'$) $U$ est une structure d’espèce $\Sigma$ sur les ensembles de base principaux $E_1, \ldots, E_n$, avec $A_1, \ldots, A_m$ pour ensembles de base auxiliaires si la relation
$$
\text{« } T\{E_1, \ldots, E_n, U\} \text{ et } R\{E_1, \ldots, E_n, U\} \text{ »}
$$
est un théorème de $\mathcal{T}'$. Lorsqu’il en est ainsi, pour tout théorème $B\{x_1, x_2, \ldots, x_n, s\}$ de la théorie $\mathcal{T}_\Sigma$, la relation $B\{E_1, \ldots, E_n, U\}$ est un théorème de $\mathcal{T}'$ (I, p. 23). Dans $\mathcal{T}_\Sigma$, la constante $s$ est appelée la structure générique d’espèce $\Sigma$.

On dit aussi que (dans la théorie $\mathcal{T}'$) les ensembles de base principaux $E_1, \ldots, E_n$ sont munis de la structure $U$. Il est clair que $U$ est un élément de l’ensemble $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$. L’ensemble des éléments $V$ de $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$ qui vérifient la relation $R\{E_1, \ldots, E_n, V\}$ est donc l’ensemble des structures d’espèce $\Sigma$ sur $E_1, \ldots, E_n$; il peut être vide.

#### Exemple 1 {#ens-iv-s1-n4-exa-1 .statement tag=03V5}

Prenons pour $\mathcal{T}$ la théorie des ensembles et considérons l’espèce de structure sans ensemble de base auxiliaire, comportant un ensemble de base principal $A$, la caractérisation typique $s \in \mathfrak{P}(A \times A)$ et l’axiome
$$
s \circ s = s \text{ et } s \cap s^{-1} = \Delta_A
$$
($\Delta_A$ diagonale de $A \times A$), qui est une relation transportable pour la typification $s \in \mathfrak{P}(A \times A)$, ainsi qu’on le vérifie aisément. Il est clair que la théorie de cette espèce de structure n’est autre que la théorie des ensembles ordonnés (III, p. 2 et p. 5); aussi dit-on que l’espèce de structure ainsi définie est l’espèce de structure d’ordre sur A. Nous avons rencontré au chap. III de nombreux exemples d’ensembles munis de structures de cette espèce.

#### Exemple 2 {#ens-iv-s1-n4-exa-2 .statement tag=03V6}

Prenons pour $\mathcal{T}$ la théorie des ensembles, et considérons l’espèce de structure sans ensemble de base auxiliaire, comportant un ensemble de base principal A, la caractérisation typique $F \in \mathfrak{P}((A \times A) \times A)$, et ayant pour axiome la relation transportable

« F est un graphe fonctionnel dont $A \times A$ est l’ensemble de définition ».

Les structures de cette espèce sont des cas particuliers de ce que l’on appelle les structures algébriques, et la fonction dont le graphe est F (application de $A \times A$ dans A) est dite loi de composition d’une telle structure (A, I, § 1, no 1).

#### Exemple 3 {#ens-iv-s1-n4-exa-3 .statement tag=03V7}

$\mathcal{T}$ étant toujours la théorie des ensembles, considérons l’espèce de structure sans ensemble de base auxiliaire, comportant un ensemble de base principal A, la caractérisation typique $V \in \mathfrak{P}(\mathfrak{P}(A))$, et ayant pour axiome la relation transportable

$$
(\forall V)((V' \subset V) \Rightarrow ((\bigcup_{X \in V'} X) \in V)) \text{ et } A \in V
$$

et $(\forall X)(\forall Y)((X \in V \text{ et } Y \in V) \Rightarrow ((X \cap Y) \in V))$.

Cette espèce de structure est appelée espèce de structure topologique. Une structure de cette espèce est aussi appelée topologie, et la relation $X \in V$ s’exprime en disant que X est ouvert pour la topologie V (TG, I, § 1).

#### Exemple 4 {#ens-iv-s1-n4-exa-4 .statement tag=03V8}

\* Prenons pour $\mathcal{T}$ la théorie de l’espèce de structure de corps, qui comporte entre autres une constante K comme unique ensemble de base (principal). L’espèce de structure d’espace vectoriel à gauche sur K comporte K comme ensemble de base auxiliaire, un ensemble de base principal E, et a pour caractérisation typique la relation

$$
V \in \mathfrak{P}((E \times E) \times E) \times \mathfrak{P}((K \times E) \times E)
$$

$pr_1 V$ étant le graphe de l’addition dans E et $pr_2 V$ celui de la multiplication par un scalaire (cf. A, II, § 1, no 1); nous n’énoncerons pas ici l’axiome de cette espèce de structure (cf. A, II, § 1, no 1).

#### Exemple 5 {#ens-iv-s1-n4-exa-5 .statement tag=03V9}

Prenons de nouveau pour $\mathcal{T}$ la théorie des ensembles; dans cette théorie, le corps $\mathbf{C}$ des nombres complexes est un terme, qui ne contient aucune lettre. L’espèce de structure de variété analytique complexe de dimension n comporte $\mathbf{C}$ comme ensemble de base auxiliaire, et un ensemble de base principal V; nous n’indiquerons pas ici la caractérisation typique ni l’axiome de cette espèce de structure.*

#### Remarque {#ens-iv-s1-n4-rem-1 .statement tag=03VA}

— 1) Il arrive souvent dans les applications (comme dans l’Exemple 4 ci-dessus) que l’échelon $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$ est un produit d’échelons

$$
S_1(E_1, \ldots, A_m) \times \cdots \times S_p(E_1, \ldots, A_m).
$$

On remplace souvent alors, dans la définition de $\Sigma$, la lettre s par un « multiplet » $(s_1, \ldots, s_p)$ (cf. II, p. 9).

D’autre part, l’axiome d’une espèce de structure $\Sigma$ s’écrit le plus souvent comme conjonction de plusieurs relations transportables (comme dans l’Exemple 3 ci-dessus); on dit que ces relations sont les axiomes de l’espèce $\Sigma$.

2) On donne un nom aux espèces de structures les plus fréquemment utilisées en Mathématique, et aux ensembles munis de structures de ces espèces: c’est ainsi qu’un ensemble ordonné (III, p. 5) est un ensemble muni d’une structure d’ordre (Exemple 1); *nous définirons, dans la suite de ce Traité, les notions de groupe, de corps, d’espace topologique, de variété différentielle, etc., qui toutes désignent des ensembles munis de certaines structures.*

3) Par abus de langage, dans la théorie des ensembles $\mathcal{T}$, la donnée de n lettres distinctes entre elles $x_1, \ldots, x_n$ (sans caractérisation typique ni axiome) est encore considérée comme une espèce de structure $\Sigma_0$, dite espèce de structure d’ensemble sur les n ensembles de base principaux $x_1, \ldots, x_n$.

### 5. Isomorphismes et transport de structures

Soit $\Sigma$ une espèce de structure dans une théorie $\mathcal{T}$, sur $n$ ensembles de base principaux $x_1, \ldots, x_n$, avec $m$ ensembles de base auxiliaires $A_1, \ldots, A_m$; soit S le schéma de construction d’échelon sur $n + m$ lettres qui figure dans la caractérisation typique de $\Sigma$, et soit R l’axiome de $\Sigma$. Dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, soit U une structure d’espèce $\Sigma$ sur des ensembles $E_1, \ldots, E_n$ (comme ensembles de base principaux) et soit $U'$ une structure de même espèce sur des ensembles $E'_1, \ldots, E'_n$. Soit enfin (dans $\mathcal{T}'$) $f_i$ une bijection de $E_i$ sur $E'_i$ ($1 \leq i \leq n$). On dit que $(f_1, \ldots, f_n)$ est un isomorphisme des ensembles $E_1, \ldots, E_n$, munis de la structure U, sur les ensembles $E'_1, \ldots, E'_n$ munis de la structure $U'$, si l’on a (dans $\mathcal{T}'$)

$$
\langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(U) = U',
$$

$\mathrm{Id}_h$ désignant l’application identique de $A_h$ sur lui-même.

Soit $f'_i$ la bijection réciproque de $f_i$ ($1 \leq i \leq n$). Il résulte aussitôt de (4) et du critère CST3 (IV, p. 3) que l’on a

$$
\langle f'_1, \ldots, f'_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(U') = U
$$

et par suite que $(f'_1, \ldots, f'_n)$ est un isomorphisme de $E'_1, \ldots, E'_n$, munis de $U'$, sur $E_1, \ldots, E_n$, munis de U; on dit que les isomorphismes $(f_1, \ldots, f_n)$ et $(f'_1, \ldots, f'_n)$ sont réciproques l’un de l’autre.

On dit que $E'_1, \ldots, E'_n$, munis de $U'$, sont isomorphes à $E_1, \ldots, E_n$, munis de U, s’il existe un isomorphisme de $E_1, \ldots, E_n$ sur $E'_1, \ldots, E'_n$; on dit encore dans ce cas que les structures U et $U'$ sont isomorphes.

Les définitions précédentes entraînent, compte tenu de CST1, le critère suivant:

CST4. Soient $U, U', U''$ trois structures de même espèce $\Sigma$ sur des ensembles de base principaux $E_1, \ldots, E_n, E'_1, \ldots, E'_n, E''_1, \ldots, E''_n$ respectivement. Soit $f_i$ une bijection de $E_i$ sur $E'_i$, $g_i$ une bijection de $E'_i$ sur $E''_i$ ($1 \leq i \leq n$). Si $(f_1, \ldots, f_n)$ et $(g_1, \ldots, g_n)$ sont des isomorphismes, il en est de même de $(g_1 \circ f_1, \ldots, g_n \circ f_n)$.

On dit qu’un isomorphisme de $E_1, \ldots, E_n$ sur $E_1, \ldots, E_n$ (pour la même structure) est un automorphisme de $E_1, \ldots, E_n$. Le composé de deux automorphismes de $E_1, \ldots, E_n$ est un automorphisme. Il en est de même de l’isomorphisme réciproque d’un automorphisme; *en d’autres termes, les automorphismes de $E_1, \ldots, E_n$ forment un groupe (A, I, § 4, n° 1).*

#### Remarque {#ens-iv-s1-n5-rem-1 .statement tag=03VD}

Par abus de langage, lorsque $f_i$ est une bijection quelconque de $E_i$ sur $E'_i$ ($1 \leq i \leq n$), on dit que $(f_1, \ldots, f_n)$ est un isomorphisme de $(E_1, \ldots, E_n)$ sur $(E'_1, \ldots, E'_n)$ pour l’espèce de structure d’ensemble (IV, p. 5, Remarque 3).

CST5. Dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, soit U une structure d’espèce $\Sigma$ sur $E_1, \ldots, E_n$, et soit $f_i$ une bijection de $E_i$ sur un ensemble $E'_i$ ($1 \leq i \leq n$). Il existe sur $E'_1, \ldots, E'_n$ une structure d’espèce $\Sigma$ et une seule telle que $(f_1, \ldots, f_n)$ soit un isomorphisme de $E_1, \ldots, E_n$ sur $E'_1, \ldots, E'_n$.

En effet, cette structure ne peut être autre que le terme U' défini par la relation (4); reste à vérifier que ce terme est effectivement une structure d'espèce Σ, c'est-à-dire que la relation R{E'_1, ..., E'_n, U'} est vraie dans $\mathcal{T}'$. Or, cela résulte de ce que R{x_1, ..., x_n, s} est transportable, car R{E'_1, ..., E'_n, U'} est équivalente, dans $\mathcal{T}'$, à la relation R{E_1, ..., E_n, U} (IV, p. 3), qui est vraie dans $\mathcal{T}'$ par hypothèse.

On dit que la structure U' est obtenue en transportant la structure U aux ensembles E'_1, ..., E'_n au moyen des applications bijectives f_1, ..., f_n. Il revient donc au même de dire que deux structures de même espèce sont isomorphes ou se déduisent l'une de l'autre par transport de structure.

Il peut se faire que deux structures quelconques d'espèce Σ soient nécessairement isomorphes; on dit alors que l'espèce de structure Σ est univalente.* Il en est ainsi de la structure de groupe monogène infini (isomorphe à $\mathbf{Z}$), de celle de corps premier de caractéristique 0 (isomorphe à $\mathbf{Q}$), de la structure de corps ordonné, archimédien et complet (isomorphe à $\mathbf{R}$), de la structure de corps connexe, localement compact, commutatif et algébriquement clos (isomorphe à $\mathbf{C}$), enfin de la structure de corps connexe, localement compact et non commutatif (isomorphe au corps des quaternions $\mathbf{H}$). Pour certaines de ces espèces de structure, comme celle de corps premier de caractéristique 0, ou celle de corps ordonné, archimédien et complet, il n'y a même aucun automorphisme autre que l'application identique; mais il y a de tels automorphismes pour les autres exemples donnés ci-dessus (par exemple la symétrie $x \mapsto -x$ dans $\mathbf{Z}$).*

On observera que les espèces de structure précédentes sont essentiellement celles qui sont à la base de la Mathématique classique. Par contre,* l'espèce de structure de groupe, l'espèce de structure d'ensemble ordonné, l'espèce de structure topologique, ne sont pas univalentes.*

### 6. Déduction de structures

Soit Σ une espèce de structure dans une théorie $\mathcal{T}$, sur n ensembles de base principaux $x_1, ..., x_n$, avec m ensembles de base auxiliaires $A_1, ..., A_m$; soit s la structure générique de Σ. Soit T un schéma de construction d'échelon sur $n + m$ termes. On dit qu'un terme $V{x_1, ..., x_n, s}$ qui ne contient aucune lettre autre que les constantes de $\mathcal{T}_\Sigma$, est intrinsèque pour s, de type $T(x_1, ..., x_n, A_1, ..., A_m)$ s'il satisfait aux conditions suivantes:

1° la relation

$$
V{x_1, ..., x_n, s} \in T(x_1, ..., x_n, A_1, ..., A_m)
$$

est un théorème de $\mathcal{T}_\Sigma$;

2° soit $\mathcal{T}'_\Sigma$ la théorie obtenue en adjoignant aux axiomes de $\mathcal{T}_\Sigma$ les axiomes « $f_i$ est une bijection de $x_i$ sur $y_i$ » ($1 \leq i \leq n$) (les lettres $y_i$ et $f_i$ étant distinctes des constantes de $\mathcal{T}_\Sigma$ et distinctes entre elles, pour $1 \leq i \leq n$); si $s'$ est la structure obtenue en transportant s par $(f_1, ..., f_n)$ (IV, p. 7), alors

$$
V{y_1, ..., y_n, s'} = \langle f_1, ..., f_n, \mathrm{Id}_1, ..., \mathrm{Id}_m \rangle^T(V{x_1, ..., x_n, s})
$$

est un théorème de $\mathcal{T}'_\Sigma$.

La plupart des termes que l’on est amené à définir dans la théorie d’une espèce de structure sont des termes intrinsèques.

Soit maintenant $\Theta$ une seconde espèce de structure dans la théorie $\mathcal{T}$, sur $r$ ensembles de base principaux $u_1, \ldots, u_r$, avec $p$ ensembles de base auxiliaires $B_1, \ldots, B_p$; soit
$$
t \in \Gamma(u_1, \ldots, u_r, B_1, \ldots, B_p)
$$
la caractérisation typique de $\Theta$ (IV, p. 4). On appelle procédé de déduction d’une structure d’espèce $\Theta$ à partir d’une structure d’espèce $\Sigma$, un système de $r + 1$ termes $P, U_1, \ldots, U_r$, intrinsèques pour $s$, et tels que $P$ soit une structure d’espèce $\Theta$ sur $U_1, \ldots, U_r$, dans la théorie $\mathcal{T}_\Sigma$. Par abus de langage, on dira souvent que le seul terme $P$ est le procédé de déduction.

Soit $\mathcal{T}'$ une théorie plus forte que $\mathcal{T}$. Si, dans $\mathcal{T}'$, $S$ est une structure d’espèce $\Sigma$ sur $E_1, \ldots, E_n$, alors $P\{E_1, \ldots, E_n, S\}$ est une structure d’espèce $\Theta$ sur les $r$ ensembles $F_j = U_j\{E_1, \ldots, E_n, S\}$ ($1 \leq j \leq r$), dite déduite de $S$ par le procédé $P$, ou subordonnée à $S$. L’hypothèse que les termes $P, U_1, \ldots, U_r$ sont intrinsèques pour $s$, entraîne en outre le critère suivant:
CST6. Soit $(g_1, \ldots, g_n)$ un isomorphisme de $E_1, \ldots, E_n$, munis d’une structure $S$ d’espèce $\Sigma$, sur $E'_1, \ldots, E'_n$, munis d’une structure $S'$ de même espèce. Si $U_j$ est de type $\mathfrak{P}(T_j)$, posons
$$
h_j = \langle g_1, \ldots, g_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{T_j} \quad (1 \leq j \leq r),
$$
et soit $F'_j = U_j\{E'_1, \ldots, E'_n, S'\}$ ($1 \leq j \leq r$); $(h_1, \ldots, h_r)$ est alors un isomorphisme de $F_1, \ldots, F_r$ sur $F'_1, \ldots, F'_r$ quand on munit respectivement ces systèmes d’ensembles des structures d’espèce $\Theta$ déduites de $S$ et $S'$ par le procédé $P$.

Il est clair que les termes $x_1, \ldots, x_n$ sont intrinsèques pour $s$; dans de nombreux cas, les termes $U_1, \ldots, U_r$ sont certaines des lettres $x_1, \ldots, x_n$; on dit alors que la structure d’espèce $\Theta$ déduite de $s$ par le procédé $P$ est sous-jacente à $s$.

#### Exemple 1 {#ens-iv-s1-n6-exa-1 .statement tag=03VE}

L’espèce de structure de groupe topologique comporte un seul ensemble de base principal $A$, ne comporte aucun ensemble de base auxiliaire, et la structure générique correspondante est un couple $(s_1, s_2)$ ($s_1$ étant le graphe de la loi de composition sur $A$, et $s_2$ l’ensemble des ensembles ouverts de la topologie de $A$; cf. TG, III, § 1). Chacun des termes $s_1, s_2$ est un procédé de déduction, fournissant respectivement la structure de groupe et la topologie sous-jacentes à la structure de groupe topologique $(s_1, s_2)$.

De même, d’une structure d’espace vectoriel on déduit une structure de groupe commutatif sous-jacente. D’une structure d’anneau on déduit une structure de groupe commutatif et une structure de monoïde (multiplicatif) sous-jacentes. D’une structure de variété différentielle on déduit une topologie sous-jacente, etc.

#### Exemple 2 {#ens-iv-s1-n6-exa-2 .statement tag=03VF}

L’espèce de structure d’espace vectoriel sur $\mathbf{C}$ (resp. sur $\mathbf{R}$) comporte un ensemble de base principal $E$, un ensemble de base auxiliaire égal à $\mathbf{C}$ (resp. $\mathbf{R}$) et a pour caractérisation typique
$$
s_1 \in \mathfrak{P}((E \times E) \times E) \text{ et } s_2 \in \mathfrak{P}((\mathbf{C} \times E) \times E)
$$
(resp.
$$
s_1 \in \mathfrak{P}((E \times E) \times E) \text{ et } s_2 \in \mathfrak{P}((\mathbf{R} \times E) \times E).
$$)

Le couple $(s_1, s_2 \cap ((\mathbf{R} \times E) \times E))$ est un procédé de déduction d'une structure d'espace vectoriel sur $\mathbf{R}$ à partir d'une structure d'espace vectoriel sur $\mathbf{C}$ (« restriction à $\mathbf{R}$ du corps des scalaires »; cf. A, II, § 1, no 13).*

#### Exemple 3 {#ens-iv-s1-n6-exa-3 .statement tag=03VG}

Supposons que $\Theta$ ait mêmes ensembles de base (principaux et auxiliaires) que $\Sigma$, et même caractérisation typique. Si en outre l'axiome de $\Sigma$ implique (dans $\mathcal{T}$) celui de $\Theta$, il est clair que le terme $s$ est un procédé de déduction d'une structure d'espèce $\Theta$ à partir d'une structure d'espèce $\Sigma$. On dit alors que $\Theta$ est moins riche que $\Sigma$, ou que $\Sigma$ est plus riche que $\Theta$. Toute structure d'espèce $\Sigma$, dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, est aussi alors une structure d'espèce $\Theta$. Par exemple, l'espèce de structure d'ensemble totalement ordonné (obtenu en prenant pour axiome la conjonction de l'axiome des structures d'ordre (IV, p. 4, Exemple 1) et de la relation $s \cup s^{-1} = A \times A$) est plus riche que l'espèce de structure d'ordre.* L'espèce de structure de groupe commutatif est plus riche que l'espèce de structure de groupe. L'espèce de structure d'espace compact est plus riche que l'espèce de structure topologique, etc.*

#### Exemple 4 {#ens-iv-s1-n6-exa-4 .statement}

\* Si $\Sigma$ et $\Theta$ sont toutes deux l'espèce de structure de groupe (resp. d'anneau), on définit en Algèbre (A, I, § 1, no 5) un procédé de déduction associant à toute structure de groupe (resp. d'anneau) la structure de groupe (resp. d'anneau) sur son centre. Si $\Sigma$ est l'espèce de structure d'espace vectoriel sur un corps commutatif K, $\Theta$ l'espèce de structure d'algèbre sur K, on définit en A, III, §§ 5 et 7, des procédés de déduction associant à tout espace vectoriel sur K son algèbre tensorielle ou son algèbre extérieure. On rencontrera de nombreux autres exemples par la suite.*

#### Remarque {#ens-iv-s1-n6-rem-1 .statement tag=03VH}

Lorsque P est un « multiplet » $(P_1, \ldots, P_q)$, on dit aussi que les termes $P_1, \ldots, P_q$ constituent un procédé de déduction d'une structure d'espèce $\Theta$ à partir d'une structure d'espèce $\Sigma$.

### 7. Espèces de structure équivalentes

Dans une même théorie $\mathcal{T}$, soient $\Sigma$ et $\Theta$ deux espèces de structure ayant les mêmes ensembles de base principaux $x_1, \ldots, x_n$. Soient $s, t$ les structures génériques d'espèce $\Sigma$ et $\Theta$. Supposons que les conditions suivantes soient remplies:

1° On a un procédé de déduction $P_{x_1, \ldots, x_n, s}$ d'une structure d'espèce $\Theta$ sur $x_1, \ldots, x_n$ à partir d'une structure d'espèce $\Sigma$ sur $x_1, \ldots, x_n$.

2° On a un procédé de déduction $Q_{x_1, \ldots, x_n, t}$ d'une structure d'espèce $\Sigma$ sur $x_1, \ldots, x_n$ à partir d'une structure d'espèce $\Theta$ sur $x_1, \ldots, x_n$.

3° La relation
$$
Q_{x_1, \ldots, x_n, P_{x_1, \ldots, x_n, s}} = s
$$
est un théorème de $\mathcal{T}_\Sigma$, et la relation
$$
P_{x_1, \ldots, x_n, Q_{x_1, \ldots, x_n, t}} = t
$$
est un théorème de $\mathcal{T}_\Theta$.

On dit alors que les espèces de structure $\Sigma$ et $\Theta$ sont équivalentes par l'intermédiaire des procédés de déduction P et Q. Dans ce cas, pour tout théorème $B_{x_1, \ldots, x_n, s}$ de la théorie $\mathcal{T}_\Sigma$, la relation $B_{x_1, \ldots, x_n, Q}$ est un théorème de la théorie $\mathcal{T}_\Theta$ (I, p. 24); et inversement, pour tout théorème $C_{x_1, \ldots, x_n, t}$ de la théorie $\mathcal{T}_\Theta$, la relation $C_{x_1, \ldots, x_n, P}$ est un théorème de $\mathcal{T}_\Sigma$.

Si U est une structure d'espèce $\Sigma$, on dit que la structure déduite de U par le procédé P est équivalente à U. Le critère CST6 entraîne le suivant:

CST7. Soient $\mathcal{S}, \mathcal{S}'$ deux structures d’espèce $\Sigma$ sur des ensembles de base principaux $(E_1, \ldots, E_n), (E'_1, \ldots, E'_n)$ respectivement. Soient $\mathcal{S}_0, \mathcal{S}'_0$ les structures d’espèce $\Theta$ équivalentes respectivement à $\mathcal{S}$ et $\mathcal{S}'$. Pour que $(g_1, \ldots, g_n)$ soit un isomorphisme pour les structures $\mathcal{S}_0$ et $\mathcal{S}'_0$, il faut et il suffit que $(g_1, \ldots, g_n)$ soit un isomorphisme pour les structures $\mathcal{S}$ et $\mathcal{S}'$.

Pratiquement, on ne fera pas de distinction entre les théories $\mathcal{T}_\Sigma$ et $\mathcal{T}_\Theta$ de deux espèces de structures équivalentes.

*Exemples. — 1)* *Soit $\Sigma$ l’espèce de structure de groupe commutatif (A, I, § 4, n° 2); elle comporte un seul ensemble de base (principal) $A$, et sa structure générique une seule lettre $F$; la caractérisation typique de $\Sigma$ est $F \in \mathfrak{B}((A \times A) \times A)$, et nous désignerons par $R \{ A, F \}$ l’axiome de $\Sigma$. Cet axiome implique en particulier que $F$ est un graphe fonctionnel (la « loi de composition » du groupe, cf. IV, p. 5, Exemple 2). On définit alors dans $\mathcal{T}_\Sigma$ (où $\mathcal{T}$ désigne la théorie des ensembles) un terme $M \{ A, F \}$, qui est un graphe fonctionnel dans $\mathfrak{B}((\mathbf{Z} \times A) \times A)$ et vérifie la relation suivant $B \{ M, A, F \}$:

$$
(\forall x)(\forall y)(\forall n)((x \in A \text{ et } y \in A \text{ et } n \in \mathbf{Z}) \Rightarrow (M(n, F(x, y)) = F(M(n, x), M(n, y))))
$$
et $(\forall x)(\forall m)(\forall n)((x \in A \text{ et } m \in \mathbf{Z} \text{ et } n \in \mathbf{Z}) \Rightarrow (M(m + n, x) = F(M(m, x), M(n, x))))$
et $(\forall x)(\forall m)(\forall n)((x \in A \text{ et } m \in \mathbf{Z} \text{ et } n \in \mathbf{Z}) \Rightarrow (M(m, M(n, x)) = M(mn, x)))$
et $(\forall x)((x \in A) \Rightarrow (M(1, x) = x))$.

(« multiplication d’un élément de $A$ par un entier »; cf. A, I, § 3, n° 1).

Considérons alors l’espèce de structure $\Theta$ de $\mathbf{Z}\text{-module}$ (A, II, § 1, n° 1), ayant un seul ensemble de base principal $A$, avec $\mathbf{Z}$ pour ensemble auxiliaire, et dont la structure générique comporte deux lettres, $G, L$, avec la caractérisation typique

$$
G \in \mathfrak{B}((A \times A) \times A) \text{ et } L \in \mathfrak{B}((\mathbf{Z} \times A) \times A)
$$

et l’axiome

« $R \{ A, G \}$ et $(L \text{ est un graphe fonctionnel})$ et $B \{ L, A, G \}$. »

On vérifie aussitôt que les termes $F, M$ constituent un procédé de déduction d’une structure d’espèce $\Theta$ à partir d’une structure d’espèce $\Sigma$, et le terme $G$ un procédé de déduction d’une structure d’espèce $\Sigma$ à partir d’une structure d’espèce $\Theta$; en outre, la condition 3° ci-dessus est trivialement vérifiée. On peut donc dire que l’espèce de structure de groupe commutatif et celle de $\mathbf{Z}\text{-module}$ sont équivalentes.

2) Soient $\Sigma$ l’espèce de structure topologique (IV, p. 5, Exemple 3), $A$ l’ensemble de base et $V$ la structure générique de $\Sigma$. Considérons la relation

$$
x \in A \text{ et } X \subset A \text{ et } (\forall U)((U \in V \text{ et } x \in U) \Rightarrow (X \cap U \neq \varnothing)).
$$

Elle admet un graphe $P \subset \mathfrak{B}(A) \times A$ par rapport au couple $(X, a)$; $P \{ A, V \}$ est un terme que l’on appelle « l’ensemble des couples $(X, a)$ tels que $x$ soit adhérent à $X$ pour la topologie $V$ ». On démontre (cf. TG, I, § 1) que les relations suivantes sont des théorèmes de $\mathcal{T}_\Sigma$:

$$
P(\varnothing) = \varnothing \\
(\forall Y)((Y \subset A) \Rightarrow (Y \subset P(Y))) \\
(\forall Y)((Y \subset A) \Rightarrow (P(P(Y)) = P(Y))) \\
(\forall Y)(\forall Z)((Y \subset A \text{ et } Z \subset A) \Rightarrow (P(Y \cup Z) = P(Y) \cup P(Z))).
$$

Considérons alors l’espèce de structure $\Theta$, ayant un seul ensemble de base (principal) $A$, dont la structure générique comporte une seule lettre $W$, qui a pour caractérisation typique $W \in \mathfrak{B}(\mathfrak{B}(A) \times A)$ et pour axiome

$$
W(\varnothing) = \varnothing \text{ et } (\forall Y)((Y \subset A) \Rightarrow (Y \subset W(Y))) \\
\text{et } (\forall Y)((Y \subset A) \Rightarrow (W(W(Y)) = W(Y))) \\
\text{et } (\forall Y)(\forall Z)((Y \subset A \text{ et } Z \subset A) \Rightarrow (W(Y \cup Z) = W(Y) \cup W(Z))).
$$

Considérons d'autre part la relation
$$
U \subset A \text{ et } (\forall x)((x \in U) \Rightarrow (x \notin W(A - U))).
$$
L'ensemble des $U \in \mathfrak{P}(A)$ vérifiant cette relation est une partie $Q\{A, W\}$ de $\mathfrak{P}(A)$. On démontre alors (TG, I, § 1, exerc. 9) que les relations suivantes sont des théorèmes de $\mathcal{T}_\Theta$:
$$
\Lambda \in Q \\
(\forall M)((M \subset Q) \Rightarrow ((\bigcup_{X \in M} X) \in Q)) \\
(\forall X)(\forall Y)((X \in Q \text{ et } Y \in Q) \Rightarrow ((X \cap Y) \in Q)).
$$
Cela prouve que les termes $P\{A, V\}$ et $Q\{A, W\}$ vérifient les conditions 1° et 2° ci-dessus; on voit aussi qu'ils satisfont à la condition 3°. Les espèces de structure $\Sigma$ et $\Theta$ sont donc équivalentes; aussi considère-t-on toute structure d'espèce $\Theta$ comme une topologie, savoir celle qui lui correspond par le procédé de déduction $Q\{A, W\}$*

## EXERCICES {#ens-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
