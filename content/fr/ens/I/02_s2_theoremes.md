---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 2
section_title: Théorèmes
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0022-0026, 0048-0048
extraction: ocr
subsections:
    - "no": 1
      title: Axiomes
      page: 21
      pdf_page: 22
    - "no": 2
      title: Démonstrations
      page: 0
      pdf_page: 23
    - "no": 3
      title: Substitutions dans une théorie
      page: 23
      pdf_page: 24
    - "no": 4
      title: Comparaison des théories
      page: 24
      pdf_page: 25
statements: 1
exercises: 1
content_sha256: 91e884c72b2659211827e3a2490bb93ae696dee676d02353031a40d80e1462ad
---

## § 2. THÉORÈMES

Pour faciliter la lecture de ce qui suit, nous écrirons désormais, si $A$ est une relation, non$(A)$ au lieu de $\neg A$. Si $A$ et $B$ sont des relations, nous écrirons « $(A)$ ou $(B)$ » au lieu de $\vee AB$, et $(A) \Rightarrow (B)$ au lieu de $\Rightarrow AB$. Parfois, nous supprimerons les parenthèses. Le lecteur pourra déterminer sans peine, dans chaque cas, de quel assemblage il s’agit.

### 1. Axiomes

La donnée des signes spécifiques définit, nous l’avons vu, les termes et les relations d’une théorie $\mathcal{T}$. Pour achever de construire $\mathcal{T}$, on fait ce qui suit:

1° On écrit d’abord un certain nombre de relations de $\mathcal{T}$; on dit que ce sont les axiomes explicites de $\mathcal{T}$; les lettres qui figurent dans les axiomes explicites sont appelées les constantes de $\mathcal{T}$.

2° On se donne une ou plusieurs règles,\footnote{Ces règles seront exprimées en utilisant, pour abréger, les symboles dont nous avons parlé (et notamment les lettres italiques grasses) (I, p. 15); mais il serait facile de se passer complètement de l’emploi de ces symboles pour les formuler (voir I, p. 25, note 1).} qu’on appelle les schémas de $\mathcal{T}$, et qui doivent présenter les particularités suivantes: $a)$ l’application d’une telle règle $\mathcal{R}$

E I.22                                                                     DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                                                     § 2

fournit une relation de $\mathcal{T}$ ; b) si $T$ est un terme de $\mathcal{T}$, $x$ une lettre, $R$ une relation de $\mathcal{T}$ construite par application du schéma $\mathfrak{R}$, la relation $(T \mid x)R$ peut encore se construire par application de $\mathfrak{R}$.

Dans tous les cas que nous envisagerons, la vérification de ces conditions sera toujours facile.

Toute relation, formée par application d’un schéma de $\mathcal{T}$, est appelée axiome implicite de $\mathcal{T}$.

Intuitivement, les axiomes représentent, soit des assertions évidentes, soit des hypothèses dont on s’apprête à tirer des conséquences; les constantes représentent des objets bien déterminés, pour lesquels les propriétés exprimées par les axiomes explicites sont supposées vraies. Au contraire, si la lettre $x$ n’est pas une constante, elle représente un objet complètement indéterminé; si une propriété de l’objet $x$ est supposée vraie par un axiome, cet axiome est nécessairement implicite, de sorte que la propriété est encore vraie d’un objet $T$ quelconque.

### 2. Démonstrations

Un texte démonstratif d’une théorie $\mathcal{T}$ comporte:

1° Une construction formative auxiliaire de relations et de termes de $\mathcal{T}$.

2° Une démonstration de $\mathcal{T}$, c’est-à-dire une suite de relations de $\mathcal{T}$ figurant dans la construction formative auxiliaire, telles que, pour chaque relation $R$ de la suite, l’une au moins des conditions suivantes soit vérifiée:

$a_1)$ $R$ est un axiome explicite de $\mathcal{T}$;

$a_2)$ $R$ résulte de l’application d’un schéma de $\mathcal{T}$ à des termes ou relations figurant dans la construction formative auxiliaire;

$b)$ il y a dans la suite deux relations $S$, $T$ précédant $R$, telles que $T$ soit $S \Rightarrow R$.

Un théorème de $\mathcal{T}$ est une relation figurant dans une démonstration de $\mathcal{T}$.

Cette notion est donc essentiellement relative à l’état de la théorie considérée, au moment où on la décrit: une relation d’une théorie $\mathcal{T}$ devient un théorème de $\mathcal{T}$ lorsqu’on a réussi à l’insérer dans une démonstration de $\mathcal{T}$. Dire qu’une relation de $\mathcal{T}$ « n’est pas un théorème de $\mathcal{T}$ » ne peut avoir de sens en Mathématique si on ne précise pas le stade du développement de $\mathcal{T}$ auquel on se réfère.

Au lieu de « théorème de $\mathcal{T}$ », on dit aussi « relation vraie dans $\mathcal{T}$ » (ou « proposition », « lemme », « corollaire », etc.). Soit $R$ une relation de $\mathcal{T}$, $x$ une lettre, $T$ un terme de $\mathcal{T}$; si $(T \mid x)R$ est un théorème de $\mathcal{T}$, on dit que $T$ vérifie dans $\mathcal{T}$ la relation $R$ (ou est une solution de $R$), quand $R$ est considérée comme relation en $x$.

Dans les mathématiques courantes, on omet le plus souvent de préciser que les relations écrites constituent une démonstration.

Une relation est dite fausse dans $\mathcal{T}$ si sa négation est un théorème de $\mathcal{T}$. On dit qu’une théorie $\mathcal{T}$ est contradictoire quand on a écrit une relation qui est à la fois vraie et fausse dans $\mathcal{T}$.

Ici encore, il s’agit bien entendu d’une notion relative à un stade déterminé du développement d’une théorie. On se gardera de la confusion (malheureusement suggérée par le sens intuitif du mot « faux ») qui consisterait à croire que, lorsqu’on a prouvé qu’une relation $R$ est fausse dans $\mathcal{T}$, on a par là même établi que $R$ « n’est pas vraie » dans $\mathcal{T}$ (cette dernière phrase n’ayant à proprement parler aucun sens précis en Mathématique, comme on l’a vu plus haut).

Nous donnerons dans ce qui suit des critères métamathématiques dits critères déductifs, qui permettent d’abréger les démonstrations. Ces critères seront désignés par la lettre C suivie d’un numéro.

Cl (syllogisme). Soient $A$ et $B$ des relations d’une théorie $\mathcal{T}$. Si $A$ et $A \Rightarrow B$ sont des théorèmes de $\mathcal{T}$, $B$ est un théorème de $\mathcal{T}$.

En effet, soit $R_1, R_2, \ldots, R_n$ une démonstration de $\mathcal{T}$ où figure $A$, et $S_1, S_2, \ldots, S_p$ une démonstration de $\mathcal{T}$ où figure $A \Rightarrow B$. Il est évident que $R_1, R_2, \ldots, R_n, S_1, S_2, \ldots, S_p$ est une démonstration de $\mathcal{T}$ où figurent $A$ et $A \Rightarrow B$. Donc

$$
R_1, R_2, \ldots, R_n, S_1, S_2, \ldots, S_p, B
$$

est une démonstration de $\mathcal{T}$, ce qui prouve que $B$ est un théorème de $\mathcal{T}$.

### 3. Substitutions dans une théorie

Soient $\mathcal{T}$ une théorie, $A_1, A_2, \ldots, A_n$ ses axiomes explicites, $x$ une lettre, $T$ un terme de $\mathcal{T}$. Soit $(T \mid x)\mathcal{T}$ la théorie dont les signes et les schémas sont les mêmes que ceux de $\mathcal{T}$, et dont les axiomes explicites sont $(T \mid x)A_1, (T \mid x)A_2, \ldots, (T \mid x)A_n$.

C2. Soient $A$ un théorème d’une théorie $\mathcal{T}$, $T$ un terme de $\mathcal{T}$, $x$ une lettre. Alors $(T \mid x)A$ est un théorème de $(T \mid x)\mathcal{T}$.

En effet, soit $R_1, R_2, \ldots, R_n$ une démonstration de $\mathcal{T}$ où figure $A$. Considérons la suite $(T \mid x)R_1, (T \mid x)R_2, \ldots, (T \mid x)R_n$, qui est une suite de relations de $\mathcal{T}$ d’après CF8 (I, p. 20). On va voir que c’est une démonstration de $(T \mid x)\mathcal{T}$, ce qui établira le critère. Si $R_k$ est un axiome implicite de $\mathcal{T}$, $(T \mid x)R_k$ est encore un axiome implicite de $\mathcal{T}$ (I, p. 22), donc de $(T \mid x)\mathcal{T}$. Si $R_k$ est un axiome explicite de $\mathcal{T}$, $(T \mid x)R_k$ est un axiome explicite de $(T \mid x)\mathcal{T}$. Enfin, se $R_k$ est précédée des relations $R_i$ et $R_j$, $R_j$ étant $R_i \Rightarrow R_k$, $(T \mid x)R_k$ est précédée de $(T \mid x)R_i$ et de $(T \mid x)R_j$, et cette dernière relation est identique à $(T \mid x)R_i \Rightarrow (T \mid x)R_k$ (critère CS5).

C3. Soient $A$ un théorème d’une théorie $\mathcal{T}$, $T$ un terme de $\mathcal{T}$, et $x$ une lettre qui n’est pas une constante de $\mathcal{T}$. Alors $(T \mid x)A$ est un théorème de $\mathcal{T}$.

Cela résulte aussitôt de C2, puisque $x$ ne figure pas dans les axiomes explicites de $\mathcal{T}$.

Plus particulièrement, si $\mathcal{T}$ ne comporte pas d’axiomes explicites, ou si les axiomes expli ne contiennent pas de lettres, le critère C3 s’applique sans restriction sur la lettre x.

### 4. Comparaison des théories

Une théorie $\mathcal{T}'$ est dite plus forte qu’une théorie $\mathcal{T}$ si tous les signes de $\mathcal{T}$ sont des signes de $\mathcal{T}'$, si tous les axiomes expli de $\mathcal{T}$ sont des théorèmes de $\mathcal{T}'$, et si les schémas de $\mathcal{T}$ sont des schémas de $\mathcal{T}'$.

**C4.** — Si une théorie $\mathcal{T}'$ est plus forte qu’une théorie $\mathcal{T}$, tous les théorèmes de $\mathcal{T}$ sont des théorèmes de $\mathcal{T}'$.

Soit $R_1, R_2, \ldots, R_n$ une démonstration de $\mathcal{T}$. On va voir de proche en proche que chaque $R_i$ est un théorème de $\mathcal{T}'$, ce qui établira le critère. Supposons notre assertion établie pour les relations précédant $R_k$ et établissons-la pour $R_k$. Si $R_k$ est un axiome de $\mathcal{T}$, c’est un théorème de $\mathcal{T}'$ par hypothèse. Si $R_k$ est précédé par des relations $R_i$ et $R_i \Rightarrow R_k$, on sait déjà que $R_i$ et $R_i \Rightarrow R_k$ sont des théorèmes de $\mathcal{T}'$, donc $R_k$ est un théorème de $\mathcal{T}'$ d’après C1.

Si chacune des deux théories $\mathcal{T}$ et $\mathcal{T}'$ est plus forte que l’autre, on dit que $\mathcal{T}$ et $\mathcal{T}'$ sont équivalentes. Alors, tout théorème de $\mathcal{T}$ est un théorème de $\mathcal{T}'$ et vice-versa.

**C5.** — Soient $\mathcal{T}$ une théorie, $A_1, A_2, \ldots, A_n$ ses axiomes expli, $a_1, a_2, \ldots, a_n$ ses constantes, $T_1, T_2, \ldots, T_h$ des termes de $\mathcal{T}$. Supposons que
$$
(T_1|a_1)(T_2|a_2)\ldots(T_h|a_h)A_i
$$
(pour $i=1,2,\ldots,n$) soient des théorèmes d’une théorie $\mathcal{T}'$, que les signes de $\mathcal{T}$ soient des signes de $\mathcal{T}'$, et que les schémas de $\mathcal{T}$ soient des schémas de $\mathcal{T}'$. Alors, si $A$ est un théorème de $\mathcal{T}$, $(T_1|a_1)\ldots(T_h|a_h)A$ est un théorème de $\mathcal{T}'$.

En effet, $\mathcal{T}'$ est plus forte que la théorie $(T_1|a_1)\ldots(T_h|a_h)\mathcal{T}$, et il suffit d’appliquer C2 et C4.

Quand on déduit, par ce procédé, un théorème de $\mathcal{T}'$ d’un théorème de $\mathcal{T}$, on dit qu’on applique dans $\mathcal{T}'$ les résultats de $\mathcal{T}$. Intuitivement, les axiomes de $\mathcal{T}$ expriment des propriétés de $a_1,a_2,\ldots,a_n$, et $A$ exprime une propriété qui est une conséquence de ces axiomes. Si des objets $T_1,T_2,\ldots,T_h$ possèdent dans $\mathcal{T}$ les propriétés exprimées par les axiomes de $\mathcal{T}$, ils possèdent aussi la propriété $A$.

\* Par exemple, dans la théorie des groupes $\mathcal{T}$, les axiomes expli contiennent deux constantes $G$ et $\mu$ (le groupe et la loi de composition). Dans la théorie des ensembles $\mathcal{T}'$, on définit deux termes : la droite numérique et l’addition des nombres réels. Si on substitue ces termes respectivement à $G$ et $\mu$ dans les axiomes expli de $\mathcal{T}$, on obtient des théorèmes de $\mathcal{T}'$. D’autre part, les schémas et les signes de $\mathcal{T}$ et $\mathcal{T}'$ sont les mêmes. On peut donc « appliquer à l’addition des nombres réels les résultats de la théorie des groupes ». On dit qu’on a construit pour la théorie des groupes un modèle dans la théorie des ensembles. (On observera que, la théorie des groupes étant plus forte que la théorie des ensembles, on peut aussi appliquer à la théorie des groupes les résultats de la théorie des ensembles.)\*

#### Remarque {#ens-i-s2-n4-rem-1 .statement tag=03G7}

Sous les hypothèses de C5, si la théorie $\mathcal{T}$ s’avérait contradictoire, il en serait de même de $\mathcal{T}'$. En effet, si $A$ et « non $A$ » sont des théorèmes de $\mathcal{T}$,

§ 3, N° 1                                                                 THÉORIES LOGIQUES                                                                 E 1.25

$(T_1\mid a_1)\ldots(T_h\mid a_h)A$, et non $(T_1\mid a_1)\ldots(T_h\mid a_h)A$ sont des théorèmes de $\mathcal T$, \* Par exemple, si la théorie des groupes était contradictoire, la théorie des ensembles le serait aussi.\*

## EXERCICES {#ens-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
