---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: Localisation
section: 2
section_title: Anneaux et modules de fractions
lang: fr
source: ac-i-iv-fr
pdf_pages: 0072-0099, 0152-0164
extraction: ocr
subsections:
    - "no": 1
      title: Définition des anneaux de fractions.
      page: 0
      pdf_page: 72
    - "no": 2
      title: Modules de fractions.
      page: 0
      pdf_page: 78
    - "no": 3
      title: Changement de partie multiplicative.
      page: 0
      pdf_page: 83
    - "no": 4
      title: Propriétés des modules de fractions.
      page: 0
      pdf_page: 86
    - "no": 5
      title: Idéaux dans un anneau de fractions.
      page: 0
      pdf_page: 88
    - "no": 6
      title: Nilradical et idéaux premiers minimaux.
      page: 0
      pdf_page: 92
    - "no": 7
      title: Modules de fractions de produits tensoriels et de modules d’homomorphismes.
      page: 0
      pdf_page: 95
    - "no": 8
      title: Application aux algèbres.
      page: 0
      pdf_page: 97
    - "no": 9
      title: Modules de fractions de modules gradués.
      page: 0
      pdf_page: 98
statements: 66
exercises: 25
content_sha256: 365de78589b6c776be87c9f01881a80c664bda57a356a2baf8f8cef314a57ae9
---

## § 2. Anneaux et modules de fractions

### 1. Définition des anneaux de fractions.

#### Définition 1 {#ac-ii-s2-def-1 .statement}

Soit A un anneau. On dit qu’une partie S de A est multiplicative si tout produit fini d’éléments de S appartient à S.

Il revient au même de dire que $1 \in S$ et que le produit de deux éléments de S appartient à S.

#### Exemple 1 {#ac-ii-s2-n1-exa-1 .statement}

Pour tout $a \in A$, l’ensemble des $a^n$, pour $n \in \mathbf{N}$, est une partie multiplicative de A.

#### Exemple 2 {#ac-ii-s2-n1-exa-2 .statement}

Soit $p$ un idéal de A. Pour que $A - p$ soit une partie multiplicative de A, il faut et il suffit que $p$ soit premier.

#### Exemple 3 {#ac-ii-s2-n1-exa-3 .statement}

L’ensemble des éléments de A non diviseurs de zéro est une partie multiplicative de A.

#### Exemple 4 {#ac-ii-s2-n1-exa-4 .statement}

Si S et T sont deux parties multiplicatives de A, l’ensemble ST des produits $st$, où $s \in S$ et $t \in T$, est une partie multiplicative.

#### Exemple 5 {#ac-ii-s2-n1-exa-5 .statement}

Soit $\mathcal{S}$ un ensemble filtrant (pour la relation $\subset$) de parties multiplicatives de A. Alors $T = \bigcup_{S \in \mathcal{S}} S$ est une partie multiplicative de A, car deux éléments quelconques de T appartiennent à une même partie $S \in \mathcal{S}$, donc leur produit appartient à T.

#### Exemple 6 {#ac-ii-s2-n1-exa-6 .statement}

Toute intersection de parties multiplicatives de A est une partie multiplicative.

Pour toute partie S d’un anneau A, il existe des parties multiplicatives de A contenant S, par exemple A lui-même. L’intersection de toutes ces parties est la plus petite partie multiplicative de A contenant S ; on dit qu’elle est engendrée par S. Il est immédiat que c’est l’ensemble formé de tous les produits finis d’éléments de S.

#### Proposition 1 {#ac-ii-s2-prop-1 .statement}

Soient A un anneau, S une partie de A. Il existe un anneau A’ et un homomorphisme h de A dans A’ ayant les propriétés suivantes :

1° les éléments de h(S) sont inversibles dans A’ ;
2° pour tout homomorphisme u de A dans un anneau B, tel que les éléments de u(S) soient inversibles dans B, il existe un homomorphisme u’ et un seul de A’ dans B tel que u = u’ ∘ h.

En d’autres termes, (A’, h) est une solution du problème d’application universelle (Ens., chap. IV, § 3, no 1) relativement aux données suivantes : l’espèce de structure Σ considérée est celle d’anneau, les morphismes sont les homomorphismes d’anneaux, et les α-applications sont les homomorphismes de A dans un anneau tels que l’image de S par un tel homomorphisme se compose d’éléments inversibles. Rappelons (loc. cit.) que, si (A’, h) et (A_1’, h_1) sont deux solutions de ce problème, il existe un isomorphisme unique j : A’ → A_1’ tel que h_1 = j ∘ h.

Soit $\overline{S}$ la partie multiplicative de A engendrée par S. Il est clair que toute solution du problème d’application universelle précédent est aussi une solution du problème d’application universelle obtenu en remplaçant S par $\overline{S}$, et inversement.

Considérons, dans l’ensemble $A \times \overline{S}$, la relation suivante entre éléments $(a, s), (a', s')$ :

(1) « Il existe $t \in \overline{S}$ tel que $t(sa' - s'a) = 0$ ».

h(a) = a/1 pour tout $a \in A$. Nous allons voir qu’on peut munir $A'$ d’une structure d’anneau telle que le couple $(A', h)$ réponde à la question.

Soient $x = a/s$ et $y = b/t$ deux éléments de $A'$. Les éléments $(ta + sb)/st$ et $ab/st$ ne dépendent que de $x$ et de $y$; en effet, si $x = a'/s'$, il existe par hypothèse $r \in \overline{S}$ tel que $r(s'a - sa') = 0$, d’où $r(s't(ta + sb) - st(ta' + s'b)) = 0$ et $r(s'tab - sta'b) = 0$. On vérifie aussitôt que les lois de composition $(x, y) \to x + y = (ta + sb)/st$ et $(x, y) \to xy = ab/st$ définissent sur $A'$ une structure d’anneau commutatif, pour laquelle $0/1$ est élément neutre pour l’addition, et $1/1$ élément unité. En outre, il est immédiat que $h$ est un homomorphisme d’anneaux et que, pour tout $s \in S$, $s/1$ est inversible dans $A'$, son inverse étant $1/s$. Enfin soient $B$ un anneau, $u : A \to B$ un homomorphisme tel que les éléments de $u(S)$ soient inversibles dans $B$; il existe une application $u' : A' \to B$ et une seule telle que
$$
u'(a/s) = u(a)(u(s))^{-1} \qquad (a \in A,\ s \in \overline{S}).
$$
En effet, si $a/s = a'/s'$, il existe $t \in \overline{S}$ tel que $t(sa' - s'a) = 0$, d’où $u(t)(u(s)u(a') - u(s')u(a)) = 0$ et comme $u(t)$, $u(s)$ et $u(s')$ sont inversibles, on a bien $u(a)(u(s))^{-1} = u(a')(u(s'))^{-1}$. On vérifie aussitôt que $u'$ est un homomorphisme pour l’addition et la multiplication ; enfin, il est clair que $u' \circ h = u$ et que $u'$ est le seul homomorphisme vérifiant cette relation, car elle implique $u'(a/s) = u'((a/1)(1/s)) = u'(1/s)u'(a/1) = u'(1/s)u(a)$, et $1 = u'(1/1) = u'(s/1)u'(1/s) = u(s)u'(1/s)$, d’où la formule (2).

C. Q. F. D.

#### Définition 2 {#ac-ii-s2-def-2 .statement}

Soient $A$ un anneau, $S$ une partie de $A$, $\overline{S}$ la partie multiplicative engendrée par $S$. On appelle anneau de fractions de $A$ défini par $S$ et on désigne par $A[S^{-1}]$ l’ensemble quotient de $A \times \overline{S}$ par la relation d’équivalence (1), muni de la structure d’anneau définie par
$$
(a/s) + (b/t) = (ta + sb)/st, \qquad (a/s)(b/t) = (ab)/(st)
$$
pour $a, b$ dans $A$, $s, t$ dans $\overline{S}$. On appelle application canonique de $A$ dans $A[S^{-1}]$ l’homomorphisme $a \to a/1$, qui fait de $A[S^{-1}]$ une $A$-algèbre.

Dans ce chapitre, nous noterons le plus souvent $i_A^S$ cette application canonique ; la démonstration de la prop. 1 montre que le couple $(A[S^{-1}], i_A^S)$ vérifie les conditions de l’énoncé de cette proposition.

#### Remarque 1 {#ac-ii-s2-n1-rem-1 .statement}

Il est clair que l’on a $A[\overline{S}^{-1}] = A[S^{-1}]$.

#### Remarque 2 {#ac-ii-s2-n1-rem-2 .statement}

Deux éléments de $A[S^{-1}]$ peuvent toujours s’écrire sous la forme $a/s$ et $a'/s$ ($a, a'$ dans $A, s \in \overline{S}$) avec le même « dénominateur » $s$, car si $b/t$ et $b'/t'$ sont deux éléments de $A[S^{-1}]$, on a $b/t = bt'/tt'$ et $b'/t' = b't/tt'$.

#### Remarque 3 {#ac-ii-s2-n1-rem-3 .statement}

Le noyau de $i_A^S$ est l’ensemble des $a \in A$ tels qu’il existe $s \in \overline{S}$ vérifiant $sa = 0$; pour que $i_A^S$ soit injectif, il faut et il suffit que $S$ ne contienne aucun diviseur de zéro dans $A$.

#### Remarque 4 {#ac-ii-s2-n1-rem-4 .statement}

S’il existe dans $S$ un élément nilpotent, on a $0 \in \overline{S}$, et l’anneau $A[S^{-1}]$ est réduit à $0$; cela résulte aussitôt de la déf. 2.

#### Remarque 5 {#ac-ii-s2-n1-rem-5 .statement}

Pour que $i_A^S$ soit une application bijective, il faut et il suffit que tout élément $s \in S$ soit inversible dans $A$ : la condition est évidemment nécessaire, puisque $s/1$ est inversible dans $A[S^{-1}]$; elle est suffisante, car pour tout $t \in \overline{S}$, $t$ est alors inversible dans $A$ et on a $a/t = at^{-1}/1$ dans $A[S^{-1}]$; donc $i_A^S$ est surjective, et on a vu en outre dans la Remarque 3 qu’elle est injective. On identifie alors $A$ et $A[S^{-1}]$ au moyen de $i_A^S$.

Exemple 7). — Si $R$ est l’ensemble des éléments non diviseurs de $0$ dans $A$, l’anneau $A[R^{-1}]$ n’est autre que ce que nous avons appelé l’anneau des fractions de $A$ (Alg., chap. I, § 9, no 4); pour éviter toute confusion, nous l’appellerons souvent l’anneau total des fractions de $A$. En particulier, si $A$ est intègre, $A[R^{-1}]$ est le corps des fractions de $A$ (loc. cit.).

#### Proposition 2 {#ac-ii-s2-prop-2 .statement}

Soient $A, B$ deux anneaux, $S$ une partie de $A$, $T$ une partie de $B$, $f$ un homomorphisme de $A$ dans $B$ tel que $f(S) \subset T$. Il existe un homomorphisme $f'$ et un seul de $A[S^{-1}]$ dans $B[T^{-1}]$ tel que $f'(a/1) = f(a)/1$ pour tout $a \in A$.

Supposons de plus que $T$ soit contenu dans la partie multiplicative de $B$ engendrée par $f(S)$. Alors, si $f$ est surjectif (resp. injectif) il en est de même de $f'$.

La première assertion revient à dire qu’il existe un homomorphisme $f' : A[S^{-1}] \to B[T^{-1}]$ et un seul rendant commutatif le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
i_A^S \downarrow & & \downarrow i_B^T \\
A[S^{-1}] & \xrightarrow{f'} & B[T^{-1}]
\end{array}
$$

Or, la relation $f(S) \subset T$ entraîne que $i_B^r(f(s))$ est inversible dans $B[T^{-1}]$ pour tout $s \in S$, et il suffit d’appliquer la prop. 1 à $i_B^T \circ f$. Il résulte aussitôt de (2) que, pour $a \in A$ et $s \in \overline{S}$ (partie multiplicative de $A$ engendrée par $S$), on a

(3)
$$
f'(a/s) = f(a)/f(s).
$$

Supposons que $T$ soit contenue dans la partie multiplicative engendrée par $f(S)$, qui n’est autre que $f(\overline{S})$. Il résulte alors de (3) que, si $f$ est surjectif, il en est de même de $f'$. Supposons maintenant $f$ injectif. Soit $a/s$ un élément du noyau de $f'$. Comme la partie multiplicative engendrée par $T$ est $f(\overline{S})$, il y a un élément $s_1 \in \overline{S}$ tel que $f(s_1)f(a) = 0$, d’où $f(s_1a) = 0$ et, par suite, $s_1a = 0$ puisque $f$ est injectif ; on a donc $a/s = 0$, ce qui montre que $f'$ est injectif.

Remarque 6). — Si les éléments de $T$ sont inversibles dans $B$, $B[T^{-1}]$ s’identifie à $B$ au moyen de l’isomorphisme $i_B^T$, et $f'$ devient alors identique à l’unique homomorphisme $u'$ de $A[S^{-1}]$ dans $B$ tel que $u' \circ i_A^S = f$.

#### Corollaire 1 {#ac-ii-s2-prop-2-cor-1 .statement}

Soient $A$ un anneau, $S$ une partie de $A$, $u$ un homomorphisme injectif de $A$ dans un anneau $B$ tel que les éléments de $u(S)$ soient inversibles dans $B$. L’unique homomorphisme $u'$ de $A[S^{-1}]$ dans $B$ tel que $u' \circ i_A^S = u$ est alors injectif.

C’est une conséquence immédiate de la prop. 2 et de la Remarque 6.

#### Corollaire 2 {#ac-ii-s2-prop-2-cor-2 .statement}

Soient $A$ un anneau, $S$ et $T$ deux parties de $A$ telles que $S \subset T$. Il existe un homomorphisme $i_A^{T,S}$ et un seul de $A[S^{-1}]$ dans $A[T^{-1}]$ tel que $i_A^T = i_A^{T,S} \circ i_A^S$.

Pour tout $a \in A$, $i_{A}^{T,s}$ applique donc l’élément $a/s$ de $A[S^{-1}]$ sur l’élément $a/s$ de $A[T^{-1}]$.

Remarque 7). — On notera que si $i_{A}^{T}$ est injectif, il en est de même de $i_{A}^{T,s}$ (cor. 1). C’est ce qui se produit si T est l’ensemble R des éléments non diviseurs de 0 de A ; on peut alors identifier $A[S^{-1}]$ au sous-anneau de l’anneau total des fractions $A[R^{-1}]$ engendré par A et par les inverses dans $A[R^{-1}]$ des éléments de S.

#### Corollaire 3 {#ac-ii-s2-prop-2-cor-3 .statement}

Soient A, B, C trois anneaux, S (resp. T, U) une partie multiplicative de A (resp. B, C), $f : A \to B$, $g : B \to C$ deux homomorphismes, $h : A \to C$ l’homomorphisme composé $g \circ f$; on suppose que $f(S) \subset T$, $g(T) \subset U$. Soient $f' : A[S^{-1}] \to B[T^{-1}]$, $g' : B[T^{-1}] \to C[U^{-1}]$, $h' : A[S^{-1}] \to C[U^{-1}]$ les homomorphismes correspondant à $f$, $g$, $h$; alors $h' = g' \circ f'$.

Cela résulte aussitôt des définitions.

En particulier, si S, T, U sont trois parties multiplicatives de A telles que $S \subset T \subset U$, on a $i_{A}^{U,s} = i_{A}^{U,T} \circ i_{A}^{T,s}$.

#### Corollaire 4 {#ac-ii-s2-prop-2-cor-4 .statement}

Soient S une partie d’un anneau A, B un sous-anneau de $A[S^{-1}]$ contenant $i_{A}^{S}(A)$, S’ l’ensemble $i_{A}^{S}(S)$. Soit j l’injection canonique de B dans $A[S^{-1}]$; l’unique homomorphisme g de $B[{S'}^{-1}]$ dans $A[S^{-1}]$ tel que $g \circ i_{B}^{S'} = j$ est un isomorphisme.

L’application g est injective en vertu du cor. 1 ; l’anneau $g(B[{S'}^{-1}])$ contient $i_{A}^{S}(A)$ et les inverses des éléments de S’; il est donc égal à $A[S^{-1}]$.

Lorsque A est intègre et $0 \notin S$, la notation $A[S^{-1}]$ est conforme à celle d’Alg., chap. IV, § 2, no 1 ; en outre, si S est multiplicative, $A[S^{-1}]$ coïncide dans ce cas avec l’ensemble noté $S^{-1}A$ dans Alg., chap. I, § 1, no 1.

Par extension de notation, pour toute partie multiplicative S d’un anneau A, nous noterons désormais $S^{-1}A$ l’anneau de fractions $A[S^{-1}]$. Lorsque S est le complémentaire d’un idéal premier p de A, nous écrirons $A_{p}$ au lieu de $S^{-1}A$.

Si A est intègre et $0 \notin S$, $S^{-1}A$ est toujours identifié à un sous-anneau du corps des fractions de A, contenant A (Remarque 7).

### 2. Modules de fractions.

L’homomorphisme canonique $i_A^s : A \to A[S^{-1}]$ défini au no 1 permet de considérer tout $A[S^{-1}]$-module comme un $A$-module.

#### Proposition 3 {#ac-ii-s2-prop-3 .statement}

Soient $A$ un anneau, $S$ une partie de $A$, $M$ un $A$-module, $M'$ le $A$-module $M \otimes_A A[S^{-1}]$, $f$ le $A$-homomorphisme canonique $x \to x \otimes 1$ de $M$ dans $M'$. Alors :

1° Pour tout $s \in S$, l’homothétie $z \to sz$ de $M'$ est bijective.

2° Pour tout $A$-module $N$ tel que, pour tout $s \in S$, l’homothétie $y \to sy$ de $N$ soit bijective, et tout homomorphisme $u$ de $M$ dans $N$, il existe un homomorphisme et un seul $u'$ de $M'$ dans $N$ tel que $u = u' \circ f$.

En d’autres termes, $(M', f)$ est une solution du problème d’application universelle ($Ens.$, chap. IV, § 3, no 1) relativement aux données suivantes : l’espèce de structure $\Sigma$ est celle de $A$-module dans lequel les homothéties produites par les éléments de $S$ sont bijectives, les morphismes sont les homomorphismes de $A$-modules, et les $\alpha$-applications sont aussi les homomorphismes de $A$-modules.

Pour tout $A$-module $N$ et tout $a \in A$, désignons par $h_a$ l’homothétie $y \to ay$ dans $N$; $a \to h_a$ est donc un homomorphisme d’anneaux de $A$ dans $\mathrm{End}_A(N)$. Dire que $h_a$ est bijective signifie que $h_a$ est un élément inversible de $\mathrm{End}_A(N)$. Supposons que, pour tout $s \in S$, $h_s$ soit inversible dans $\mathrm{End}_A(N)$; les éléments $h_a$ pour $a \in A$ et les inverses des éléments $h_s$ pour $s \in S$ engendrent alors dans $\mathrm{End}_A(N)$ un sous-anneau commutatif $B$, et l’homomorphisme $a \to h_a$ de $A$ dans $B$ est tel que les images des éléments de $S$ soient inversibles. On en conclut (no 1, prop. 1) qu’il existe un homomorphisme unique $h'$ de $A[S^{-1}]$ dans $B$ tel que $h'(a/s) = h_a(h_s)^{-1}$; on sait ($Alg.$, chap. II, 3e éd., § 1, no 14) qu’un tel homomorphisme définit sur $N$ une structure de $A[S^{-1}]$-module telle que $(a/s).y = (h_s)^{-1}(a.y)$; la structure de $A$-module déduite de cette structure de $A[S^{-1}]$-module au moyen de l’homomorphisme $i_A^s$ n’est autre que la structure initialement donnée.

Inversement, si $N$ est un $A[S^{-1}]$-module, et si on le considère comme $A$-module au moyen de $i_A^s$, les homothéties $y \to sy$, pour s \in S, sont bijectives, car $y \to (1/s)y$ est l’application réciproque de $y \to sy$; et la structure de $A[S^{-1}]$-module sur $N$ déduite de sa structure de $A$-module par le procédé décrit ci-dessus est la structure de $A[S^{-1}]$-module initialement donnée. Il y a donc correspondance *biunivoque canonique* entre $A[S^{-1}]$-modules et $A$-modules dans lesquels les *homothéties produites par les éléments de $S$* sont *bijectives*; en outre, si $N, N'$ sont deux $A$-modules ayant cette propriété, tout homomorphisme $u : N \to N'$ de $A$-modules est aussi un homomorphisme pour les structures de $A[S^{-1}]$-modules de $N$ et $N'$, car pour tout $y \in N$ et tout $s \in S$, on peut écrire $u(y) = u(s.((1/s)y))) = s.u((1/s)y)$, d’où $u((1/s)y) = (1/s)u(y)$; la réciproque est évidente.

Cela étant, l’énoncé de la prop. 3 n’est autre que la caractérisation du module obtenu à partir de $M$ par *extension des scalaires à $A[S^{-1}]$*, compte tenu de l’interprétation précédente (*Alg.*, chap. II, 3e éd., § 5, no 1, *Remarque 1*).

#### Définition 3 {#ac-ii-s2-def-3 .statement}

*Soient $A$ un anneau, $S$ une partie de $A$, $\overline{S}$ la partie multiplicative de $A$ engendrée par $S$, $M$ un $A$-module. On appelle module des fractions de $M$ défini par $S$ et on note $M[S^{-1}]$ ou $\overline{S}^{-1}M$ le $A[S^{-1}]$-module $M \otimes_A A[S^{-1}]$.*

Dans ce chapitre, nous noterons le plus souvent $i_M^S$ l’application canonique $m \to m \otimes 1$ de $M$ dans $M[S^{-1}]$.

#### Remarque 1 {#ac-ii-s2-n2-rem-1 .statement}

Il est clair que l’on a $M[\overline{S}^{-1}] = M[S^{-1}]$.

#### Remarque 2 {#ac-ii-s2-n2-rem-2 .statement}

Pour $m \in M$ et $s \in \overline{S}$, on écrit encore $m/s$ l’élément $m \otimes (1/s)$ de $M[S^{-1}]$. Tout élément de $M[S^{-1}]$ est de cette forme, car un tel élément s’écrit $\sum_i m_i \otimes (a_i/s)$ avec $m_i \in M, a_i \in A, s \in S$ (no 1, *Remarque 2*) et on a $m_i \otimes (a_i/s) = (a_i m_i) \otimes (1/s)$, donc $\sum_i m_i \otimes (a_i/s) = m \otimes (1/s)$ avec $m = \sum_i a_i m_i$. On a
$$
(4)\quad (m/s) + (m'/s') = (s'm + sm')/(ss')
$$
$$
(5)\quad (a/s)(m/s') = (am)/(ss')
$$
pour $m, m'$ dans $M, a \in A, s, s'$ dans $S$.

#### Remarque 3 {#ac-ii-s2-n2-rem-3 .statement}

Lorsque S est le complémentaire d’un idéal premier p de A, on écrit M_p au lieu de S^{-1}M.

#### Remarque 4 {#ac-ii-s2-n2-rem-4 .statement}

Soit M un A[S^{-1}]-module ; lorsque M est considéré canoniquement comme un A-module, i_M^s est une application bijective, car le couple formé de M et de l’application identique 1_M est aussi trivialement solution du problème d’application universelle résolu par M[S^{-1}] et i_M^s. On identifie alors M et M[S^{-1}].

#### Proposition 4 {#ac-ii-s2-prop-4 .statement}

Soient S une partie multiplicative de A, M un A-module. Pour que m/s = 0 (m \in M, s \in S), il faut et il suffit qu’il existe s' \in S tel que s'm = 0.

Si s' \in S est tel que s'm = 0, il est clair que m/s = (s'm)/(s's) = 0. Inversement, supposons que m/s = 0. Comme 1/s est inversible dans S^{-1}A, on a m/1 = 0. Pour tout sous-A-module P de S^{-1}A contenant 1, notons \beta(P, m) l’image de (m, 1) par l’application canonique de M \times P dans M \otimes_A P ; on a donc \beta(S^{-1}A, m) = 0. On sait (Alg., chap. II, 3e éd., § 6, no 7, cor. 4 de la prop. 12) qu’il existe un sous-module P de type fini de S^{-1}A contenant 1 et tel que \beta(P, m) = 0. Pour tout t \in S, désignons par A_t l’ensemble des a/t pour a \in A ; comme P est de type fini, il existe un t \in S tel que P \subset A_t (no 1, Remarque 2), d’où \beta(A_t, m) = 0. L’application a \to a/t de A dans A_t est surjective ; soit B son noyau. Elle définit une application surjective h : M \otimes_A A \to M \otimes_A A_t, dont le noyau est BM (M étant identifié à M \otimes A) ; on a \beta(A_t, m) = h(tm) et par suite tm se met sous la forme \sum_{i=1}^r b_i m_i avec b_i \in B, m_i \in M (1 \leq i \leq r). Comme b_i/t = 0 pour 1 \leq i \leq r, il existe un t' \in S tel que t'b_i = 0 pour 1 \leq i \leq r, d’où t'tm = 0, ce qui démontre la prop. 4.

#### Corollaire 1 {#ac-ii-s2-prop-4-cor-1 .statement}

Pour que m/s = m'/s' dans S^{-1}M, il faut et il suffit qu’il existe t \in S tel que t(s'm - sm') = 0.

En effet (m/s) - (m'/s') = (s'm - sm')/ss'.

#### Corollaire 2 {#ac-ii-s2-prop-4-cor-2 .statement}

Soit M un A-module de type fini. Pour que S^{-1}M = 0, il faut et il suffit qu’il existe s \in S tel que sM = 0.

Sans hypothèse sur M, il est clair que la relation sM = 0 pour un s \in S entraîne S^{-1}M = 0. Réciproquement, supposons que

$S^{-1}M = 0$, et soit $(m_i)_{1 \leq i \leq n}$ un système de générateurs de $M$; les $m_i/1$ engendrent le $S^{-1}A$-module $S^{-1}M$, donc dire que $S^{-1}M = 0$ revient à dire que $m_i/1 = 0$ pour $1 \leq i \leq n$; en vertu de la prop. 4, il y a des $s_i \in S$ tels que $s_i m_i = 0$, et en prenant $s = s_1 s_2 \ldots s_n \in S$, on a $s m_i = 0$ pour tout $i$, donc $sM = 0$.

#### Corollaire 3 {#ac-ii-s2-prop-4-cor-3 .statement}

*Soit M un A-module de type fini. Pour qu’un idéal a de A soit tel que aM = M, il faut et il suffit qu’il existe a ∈ a tel que $(1 + a)M = 0$.*

Il est clair que la relation $(1 + a)M = 0$ entraîne $M = aM$. Pour démontrer la réciproque, nous utiliserons le lemme suivant :

*Lemme 1. — Pour tout idéal a de A, l’ensemble S des éléments $1 + a$ pour $a \in a$, est une partie multiplicative de A, et l’ensemble $a'$ des éléments de $S^{-1}A$ de la forme $a/s$, où $a \in a$ et $s \in S$, est un idéal contenu dans le radical de $S^{-1}A$.*

La première assertion est évidente, ainsi que le fait que $a'$ est un idéal de $S^{-1}A$. D’autre part, $(1/1) + (a/s) = (s + a)/s$ et on a $s + a \in S$ pour $s \in S$ et $a \in a$ par définition de S ; donc $(1/1) + (a/s)$ est inversible dans $S^{-1}A$ pour tout $a/s \in a'$, ce qui achève de prouver le lemme (*Alg.*, chap. VIII, § 6, no 3, th. 1).

Cela étant, si on pose $N = S^{-1}M$, il est clair que N est un $S^{-1}A$-module de type fini ; si $aM = M$, on a $a'N = N$ et on en conclut que $N = 0$ par le lemme de Nakayama (*Alg.*, chap. VIII, § 6, no 3, cor. de la prop. 6) ; le corollaire résulte alors du cor. 2.

#### Proposition 5 {#ac-ii-s2-prop-5 .statement}

*Soient A, B deux anneaux, S une partie multiplicative de A, T une partie multiplicative de B, et f un homomorphisme de A dans B tel que $f(S) \subset T$. Soient M un A-module, N un B-module, et u une application A-linéaire de M dans N. Il existe alors une application $S^{-1}A$-linéaire $u'$ et une seule de $S^{-1}M$ dans $T^{-1}N$ telle que $u'(m/1) = u(m)/1$ pour tout $m \in M$.

En effet, l’application $i_N^{T} \circ u$ de M dans $T^{-1}N$ est A-linéaire. En outre, si $s \in S$, on a $f(s) \in T$, donc l’homothétie produite par s dans $T^{-1}N$ est bijective. L’existence et l’unicité de $u'$ résultent alors de la prop. 3. On a, pour $m \in M$ et $s \in S$,

$$
u'(m/s) = u(m)/f(s).
$$

Avec les mêmes notations, soient C un troisième anneau, U une partie multiplicative de C, g un homomorphisme de B dans C tel que $g(T) \subset U$, P un C-module, $\varphi$ une application B-linéaire de N dans P, et $\varphi'$ l’application $T^{-1}B$-linéaire de $T^{-1}N$ dans $U^{-1}P$ associée à $\varphi$. On a alors

$$(\varphi \circ u)' = \varphi' \circ u'$$

où le premier membre est l’application A-linéaire $S^{-1}M \to U^{-1}P$ associée à $\varphi \circ u$. De même, si $u_1$ est une seconde application A-linéaire de M dans N, on a

$$(u + u_1)' = u' + u'_1$$

le premier membre étant l’application A-linéaire $S^{-1}M \to T^{-1}N$ associée à $u + u_1$.

Remarque 5). — Si, dans la prop. 5, on prend $B = A$, $T = S$ et $f = 1_A$, on voit aussitôt que $u'$ n’est autre que l’application $u \otimes 1 : M \otimes S^{-1}A \to N \otimes S^{-1}A$. Nous la noterons désormais $S^{-1}u$; lorsque S est le complémentaire d’un idéal premier p de A, nous écrirons $u_p$ au lieu de $S^{-1}u$.

#### Proposition 6 {#ac-ii-s2-prop-6 .statement}

Soient $f$ un homomorphisme d’un anneau A dans un anneau B, S une partie multiplicative de A. Il existe une application j et une seule de $(f(S))^{-1}B$ dans $S^{-1}B$ (où B est considéré comme A-module au moyen de f) telle que $j(b/f(s)) = b/s$ pour $b \in B$, $s \in S$. Si $f' : S^{-1}A \to (f(S))^{-1}B$ est l’homomorphisme d’anneaux associé à f (no 1, prop. 2), on a $j \circ f' = S^{-1}f$. L’application j est un isomorphisme de la structure de $S^{-1}A$-module de $(f(S))^{-1}B$, définie par $f'$, sur celle de $S^{-1}B$, et aussi de la structure de B-module de $(f(S))^{-1}B$ sur celle de $S^{-1}B$ (résultant de la définition $S^{-1}B = (S^{-1}A) \otimes_A B$).

Si $b, b'$ sont dans B, $s, s'$ dans S, les conditions $b/s = b'/s'$ et $b/f(s) = b'/f(s')$ sont équivalentes comme il résulte du cor. 1 de la prop. 4, ce qui établit l’existence de j et montre que j est bijective ; l’unicité de j est évidente. Il est clair que j est un isomorphisme de groupes additifs. Si $a \in A, b \in B, s \in S, t \in S$, on a $(a/s).(b/f(t)) = f'(a/s)(b/f(t)) = (f(a)/f(s))(b/f(t)) = (f(a)b)/f(st)$, d’où il résulte que j est $(S^{-1}A)$-linéaire. Il est clair que $j \circ f' = S^{-1}f$. Enfin, si $b \in B, b' \in B, s \in S$, on a $j(b.(b'/f(s))) = j(bb'/f(s)) = bb'/s = b.(b'/s)$, ce qui démontre la dernière assertion.

L’application $j$ de la prop. 6 s’appelle l’isomorphisme canonique de $(f(S))^{-1}B$ sur $S^{-1}B$. On identifie en général ces deux ensembles au moyen de $j$; on a alors $f' = S^{-1}f, i_B^s = i_B^{f(s)}$.

### 3. Changement de partie multiplicative.

Soient $A$ un anneau, $S$ une partie multiplicative de $A$, $M$ un $A$-module. Si $T$ est une partie multiplicative de $A$ contenant $S$, il résulte de la prop. 5 du no 2 qu’il existe une application $S^{-1}A$-linéaire et une seule $i_M^{T,s} : S^{-1}M \to T^{-1}M$, telle que $i_M^T = i_M^{T,s} \circ i_M^s$; l’application $i_M^{T,s}$ transforme l’élément $m/s$ de $S^{-1}M$ en l’élément $m/s$ de $T^{-1}M$. On vérifie aussitôt que l’on a $i_M^{T,s} = i_A^{T,s} \otimes 1_M$. Si $U$ est une troisième partie multiplicative de $A$ telle que $T \subset U$, on a donc $i_M^{U,s} = i_M^{U,T} \circ i_M^{T,s}$; en outre, si $u : M \to N$ est un homomorphisme de $A$-modules, le diagramme

$$
\begin{array}{ccc}
S^{-1}M & \xrightarrow{S^{-1}u} & S^{-1}N \\
i_M^{T,s} \downarrow & & \downarrow i_N^{T,s} \\
T^{-1}M & \xrightarrow{T^{-1}u} & T^{-1}N
\end{array}
$$

est commutatif.

#### Proposition 7 {#ac-ii-s2-prop-7 .statement}

Soient $A$ un anneau, $S, T$ deux parties multiplicatives de $A$. Posons $T' = i_A^s(T)$.

(i) Il existe un isomorphisme $j$ et un seul de l’anneau $(ST)^{-1}A$ sur l’anneau ${T'}^{-1}(S^{-1}A)$ tel que le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^s} & S^{-1}A \\
i_A^{ST} \downarrow & & \downarrow i_{S^{-1}A}^{T'}
\\
(ST)^{-1}A & \xrightarrow{j} & {T'}^{-1}(S^{-1}A)
\end{array}
$$

soit commutatif.

(ii) Soit $M$ un $A$-module. Il existe un $(ST)^{-1}A$-isomorphisme $k$ du $(ST)^{-1}A$-module $(ST)^{-1}M$ sur le ${T'}^{-1}(S^{-1}A)$-module ${T'}^{-1}(S^{-1}M)$ tel que le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{i_M^s} & S^{-1}M \\
i_M^{ST} \downarrow & & \downarrow i_{S^{-1}M}^{T'}
\\
(ST)^{-1}M & \xrightarrow{k} & {T'}^{-1}(S^{-1}M)
\end{array}
$$

soit commutatif.

(i) Utilisons la définition de (ST)^{-1}A comme solution d’un problème d’application universelle. Soient B un anneau et f un homomorphisme de A dans B tel que f(ST) se compose d’éléments inversibles. Comme f(S) se compose par suite d’éléments inversibles, il existe un homomorphisme et un seul f' : S^{-1}A → B tel que f = f' ∘ i_A^S (n° 1, prop. 1). Pour tout t ∈ T, f'(i_A^S(t)) = f(t) est inversible dans B par hypothèse, donc f'(T') se compose d’éléments inversibles ; il existe alors, en vertu du n° 1, prop. 1, un homomorphisme et un seul f'' de T'^{-1}(S^{-1}A) dans B tel que f' = f'' ∘ i_{S^{-1}A}^{T'}, d’où f = f'' ∘ u en posant u = i_{S^{-1}A}^{T'} ∘ i_A^S.

En outre, si f''_1 : T'^{-1}(S^{-1}A) → B est un second homomorphisme tel que f''_1 ∘ u = f, on a (f''_1 ∘ i_{S^{-1}A}^{T'}) ∘ i_A^S = (f'' ∘ i_{S^{-1}A}^{T'}) ∘ i_A^S, d’où f''_1 ∘ i_{S^{-1}A}^{T'} = f'' ∘ i_{S^{-1}A}^{T'} et par suite f''_1 = f''.

Comme les images par u des éléments de ST dans T'^{-1}(S^{-1}A) sont inversibles, le couple (T'^{-1}(S^{-1}A), u) est solution du problème d’application universelle (relatif à A et ST) considéré au n° 1. Ceci démontre l’existence et l’unicité de j.

(ii) La démonstration est tout à fait analogue à celle de (i), en utilisant cette fois le n° 2, prop. 3, et elle est laissée au lecteur.

#### Proposition 8 {#ac-ii-s2-prop-8 .statement}

Soient A un anneau, S, T deux parties multiplicatives de A telles que S ⊂ T. Les propriétés suivantes sont équivalentes :

a) L’homomorphisme i_A^{T,S} : S^{-1}A → T^{-1}A est bijectif.

b) Pour tout A-module M, l’homomorphisme i_M^{T,S} : S^{-1}M → T^{-1}M est bijectif.

c) Pour tout t ∈ T, il existe a ∈ A tel que at ∈ S (autrement dit, tout élément de T divise un élément de S).

d) Tout idéal premier qui rencontre T rencontre S.

On a vu ci-dessus que i_A^{T,S} = 1_M ⊗ i_A^{T,S}, ce qui prouve aussitôt l’équivalence de a) et b). Posons T' = i_A^S(T) ; alors (prop. 7) T^{-1}A s’identifie à T'^{-1}(S^{-1}A), et a) équivaut à dire que les éléments de T' sont inversibles dans S^{-1}A (n° 1, Remarque 5). Or, dire que (t/1)(a/s) = 1/1 (t ∈ T, a ∈ A, s ∈ S) signifie qu’il existe s' ∈ S tel que tas' = ss', ce qui montre l’équivalence de a) et c). Montrons que d) entraîne c). Soit t un élément de T et supposons que t/1 ne soit pas inversible dans S^{-1}A ; il existe alors un idéal maximal m' de

S^{-1}A contenant t/1 (Alg., chap. I, § 8, no 7, th. 2), et $p = (i_A^{S})^{-1}(m')$ est un idéal premier de A contenant t et ne rencontrant pas S (puisque l’image par $i_A^S$ d’un élément de S est inversible). Réciproquement, s’il existe un idéal premier p qui rencontre T sans rencontrer S, aucun élément de $p \cap T$ ne peut diviser un élément de S ; ceci prouve que c) entraîne d), et termine la démonstration.

On déduit de la prop. 8 que parmi les parties multiplicatives T de A, contenant S et vérifiant les conditions équivalentes de la prop. 8, il y en a une plus grande, formée de tous les éléments de A qui divisent un élément de S (cf. exerc. 1).

#### Proposition 9 {#ac-ii-s2-prop-9 .statement}

Soient I un ensemble préordonné filtrant croissant, $(S_\alpha)_{\alpha \in I}$ une famille croissante de parties multiplicatives d’un anneau A, $S = \bigcup_{\alpha \in I} S_\alpha$. Posons $\rho_{\beta \alpha} = i_A^{S_\beta, S_\alpha}$ pour $\alpha \leq \beta$, $\rho_\alpha = i_A^{S_\alpha, S_\alpha}$. Alors $(S_\alpha^{-1}A, \rho_{\beta \alpha})$ est un système inductif d’anneaux, et si, pour tout $\alpha \in I$, $\rho'_\alpha$ est l’application canonique de $S_\alpha^{-1}A$ dans $\lim \rightarrow S_\alpha^{-1}A$, il existe un isomorphisme j et un seul de $\lim \rightarrow S_\alpha^{-1}A$ sur $S^{-1}A$ tel que $j \circ \rho'_\alpha = \rho_\alpha$ pour tout $\alpha \in I$.

On a $\rho_{\gamma \alpha} = \rho_{\gamma \beta} \circ \rho_{\beta \alpha}$ pour $\alpha \leq \beta \leq \gamma$ (no 1, cor. 3 de la prop. 2), donc $(S_\alpha^{-1}A, \rho_{\beta \alpha})$ est un système inductif. Posons $A' = \lim \rightarrow S_\alpha^{-1}A$; comme $\rho_\alpha = \rho_\beta \circ \rho_{\beta \alpha}$ pour $\alpha \leq \beta$ (no 1, cor. 3 de la prop. 2), $(\rho_\alpha)$ est un système inductif d’homomorphismes, et $j = \lim \rightarrow \rho_\alpha$ est l’unique homomorphisme de $A'$ dans $S^{-1}A$ tel que $j \circ \rho'_\alpha = \rho_\alpha$ pour tout $\alpha \in I$. Les homomorphismes $\rho'_\alpha \circ i_A^{S_\alpha} : A \to A'$ sont tous égaux, car $\rho_{\beta \alpha} \circ i_A^{S_\alpha} = i_A^{S_\beta}$ pour $\alpha \leq \beta$; soit u leur valeur commune. Il est clair que les éléments de $u(S)$ sont inversibles dans $A'$, ce qui montre qu’il existe un homomorphisme $h : S^{-1}A \to A'$ tel que $h \circ i_A^S = u$ (no 1, prop. 1). On a
$$
j \circ h \circ i_A^S = j \circ u = j \circ \rho'_\alpha \circ i_A^{S_\alpha} = \rho_\alpha \circ i_A^{S_\alpha} = i_A^S
$$
pour tout $\alpha \in I$, et par suite $j \circ h$ est l’automorphisme identique de $S^{-1}A$. D’autre part, pour tout $\alpha \in I$, on a
$$
h \circ j \circ \rho'_\alpha \circ i_A^{S_\alpha} = h \circ \rho_\alpha \circ i_A^{S_\alpha} = h \circ i_A^S = u = \rho'_\alpha \circ i_A^{S_\alpha},
$$
d’où $h \circ j \circ \rho'_\alpha = \rho'_\alpha$ pour tout $\alpha \in I$; il en résulte que $h \circ j$ est l’automorphisme identique de $A'$, et par suite $j$ est un isomorphisme.

#### Corollaire {#ac-ii-s2-n3-cor-1 .statement}

Les hypothèses étant celles de la prop. 9, soit M un A-module. Posons $f_{\beta \alpha} = i_M^{s_{\beta}, s_{\alpha}}$ pour $\alpha \leq \beta$, $f_{\alpha} = i_M^{s_{\alpha}, s_{\alpha}}$ pour tout $\alpha \in I$, et soit $f'_\alpha$ l’application canonique de $S_\alpha^{-1}M$ dans $\lim \rightarrow S_\alpha^{-1}M$; il existe alors un $S^{-1}A$-isomorphisme g de $S^{-1}M$ sur $\lim \rightarrow S_\alpha^{-1}M$ tel que $g \circ f_\alpha = f'_\alpha$ pour tout $\alpha \in I$.

Le corollaire résulte aussitôt des définitions $S_\alpha^{-1}M = M \otimes_A S_\alpha^{-1}A$ et $S^{-1}M = M \otimes_A S^{-1}A$, et du fait que le passage à la limite inductive commute au produit tensoriel (Alg., chap. II, 3e éd., § 6, no 7, prop. 12).

### 4. Propriétés des modules de fractions.

Dans tout ce no, A désigne un anneau et S une partie multiplicative de A.

Soit $(M_\alpha, \varphi_{\beta \alpha})$ un système inductif de A-modules ; alors $(S^{-1}M_\alpha, S^{-1}\varphi_{\beta \alpha})$ est un système inductif de $S^{-1}A$-modules, et le fait que le passage à la limite inductive commute aux produits tensoriels (Alg., chap. II, 3e éd., § 6, no 7, prop. 12) permet de définir un isomorphisme canonique

$$
\lim \rightarrow (S^{-1}M_\alpha) \to S^{-1} \lim \rightarrow M_\alpha.
$$

De même, le fait que la formation des sommes directes commute aux produits tensoriels (Alg., chap. II, § 3, no 7, prop. 7) permet de définir, pour toute famille $(M_i)_{i \in I}$ de A-modules, un isomorphisme canonique

$$
\bigoplus_{i \in I} S^{-1}M_i \to S^{-1} \bigoplus_{i \in I} M_i.
$$

Notons enfin que, si un A-module M est somme d’une famille $(N_i)_{i \in I}$ de sous-modules, $S^{-1}M$ est somme de la famille des sous-$S^{-1}A$-modules engendrée par les $i_M^S(N_i)$. Il en résulte que si M est un A-module de type fini (resp. de présentation finie), $S^{-1}M = S^{-1}A \otimes_A M$ est un $S^{-1}A$-module de type fini (resp. de présentation finie).

#### Théorème 1 {#ac-ii-s2-thm-1 .statement}

L’anneau $S^{-1}A$ est un A-module plat (chap. I, § 2, no 3, déf. 2).

Si $u : M' \to M$ est un homomorphisme injectif de A-modules, il faut établir que $S^{-1}u : S^{-1}M' \to S^{-1}M$ est injectif. Or, si $m'/s$ ($m' \in M',\ s \in S$) est tel que $u(m')/s = 0$, cela entraîne l’existence d’un $s' \in S$ tel que $s'u(m') = 0$ (n° 2, prop. 4) ou encore $u(s'm') = 0$; comme $u$ est injectif, on en déduit $s'm' = 0$, d’où $m'/s = 0$.

Le fait que $S^{-1}A$ est un A-module plat permet de lui appliquer les résultats du chap. I, § 2. En particulier :

1° Si M est un A-module et N un sous-module de M, $S^{-1}N$ s’identifie canoniquement à un sous-module de $S^{-1}M$, engendré par $i_M^S(N)$ (chap. I, § 2, n° 3, Remarque 2) ; cette identification étant faite, $S^{-1}(M/N)$ s’identifie à $(S^{-1}M)/(S^{-1}N)$, et si P est un second sous-module de M, on a

$$
S^{-1}(N + P) = S^{-1}N + S^{-1}P,\qquad S^{-1}(N \cap P) = S^{-1}N \cap S^{-1}P
$$

(chap. I, § 2, n° 6, prop. 6).

2° Si M est un A-module de type fini, on a

$$
S^{-1}\operatorname{Ann}(M) = \operatorname{Ann}(S^{-1}M)
$$

(chap. I, § 2, n° 10, cor. 2 de la prop. 12).

#### Proposition 10 {#ac-ii-s2-prop-10 .statement}

Soit M un A-module. Pour tout sous-module N’ du $S^{-1}A$-module $S^{-1}M$, soit $\varphi(N')$ l’image réciproque de N’ par $i_M^S$. Alors :
(i) On a $S^{-1}\varphi(N') = N'$.
(ii) Pour tout sous-module N de M, le sous-module $\varphi(S^{-1}N)$ de M est formé des $m \in M$ pour lesquels il existe $s \in S$ tel que $sm \in N$.
(iii) $\varphi$ est un isomorphisme (pour les structures d’ordre définies par les relations d’inclusion) de l’ensemble des sous-$S^{-1}A$-modules de $S^{-1}M$ sur l’ensemble des sous-modules Q de M qui vérifient la condition suivante :
(MS) Si $sm \in Q,\ s \in S,\ m \in M$, alors $m \in Q$.
On a évidemment $S^{-1}\varphi(N') \subset N'$; inversement, si $n' = m/s \in N'$, on a $m/1 \in N'$, donc $m \in \varphi(N')$ et par suite $n' \in S^{-1}(\varphi(N'))$; d’où (i). Pour qu’un élément $m \in M$ soit tel que $m \in \varphi(S^{-1}N)$, il faut et il suffit que $m/1 \in S^{-1}N$, c’est-à-dire qu’il existe $s \in S$ et $n \in N$ tels que $m/1 = n/s$; cela signifie qu’il existe $s' \in S$ tel que $s'sm = s'n \in N$, d'où (ii). Enfin, la relation $sm \in \varphi(N')$ équivaut par définition à $sm/1 \in N'$ et comme $s/1$ est inversible dans $S^{-1}A$, cela entraîne $m/1 \in N'$, ou $m \in \varphi(N')$, donc $\varphi(N')$ vérifie la relation (MS) ; il résulte d'autre part de (ii) que, si $N$ vérifie (MS), on a $\varphi(S^{-1}N) = N$, ce qui achève de prouver (iii).

On dit que le sous-module $\varphi(S^{-1}N)$ est le saturé de $N$ dans $M$ pour $S$, et les sous-modules vérifiant la condition (MS) (donc égaux à leurs saturés) sont dits saturés pour $S$. Le sous-module $\varphi(S^{-1}N)$ est le noyau de l'homomorphisme composé

$$
M \xrightarrow{h} M/N \xrightarrow{i_{M/N}^S} S^{-1}M/S^{-1}N
$$

où $h$ est l'homomorphisme canonique, comme il résulte de la commutativité du diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{h} & M/N \\
i_M^S \downarrow & & \downarrow i_{M/N}^S \\
S^{-1}M & \to & S^{-1}M/S^{-1}N
\end{array}
$$

Lorsque $S$ est le complémentaire dans $A$ d'un idéal premier $p$, on dit encore que $\varphi(S^{-1}N)$ est le saturé de $N$ dans $M$ pour $p$.

#### Corollaire 1 {#ac-ii-s2-prop-10-cor-1 .statement}

Soient $N_1, N_2$ deux sous-modules d'un $A$-module $M$. Pour que $S^{-1}N_1 \subset S^{-1}N_2$, il faut et il suffit que le saturé de $N_1$ pour $S$ soit contenu dans celui de $N_2$.

#### Corollaire 2 {#ac-ii-s2-prop-10-cor-2 .statement}

Si $M$ est un $A$-module noethérien (resp. artinien), $S^{-1}M$ est un $S^{-1}A$-module noethérien (resp. artinien). En particulier, si l'anneau $A$ est noethérien (resp. artinien), il en est de même de l'anneau $S^{-1}A$.

### 5. Idéaux dans un anneau de fractions.

#### Proposition 11 {#ac-ii-s2-prop-11 .statement}

Soient $A$ un anneau, $S$ une partie multiplicative de $A$. Pour tout idéal $b'$ de $S^{-1}A$, soit $b = (i_A^S)^{-1}(b')$, de sorte que $b' = S^{-1}b$.

(i) Soit $f$ l'homomorphisme canonique $A \to A/b$. L'homomorphisme de $S^{-1}A$ dans $(f(S))^{-1}(A/b)$ canoniquement associé à $f$ (no 1, prop. 2) est surjectif et son noyau est $b'$, ce qui définit par passage aux quotients un isomorphisme canonique de $(S^{-1}A)/b'$ sur $(f(S))^{-1}(A/b)$. En outre, l’homomorphisme canonique de $A/b$ dans $(f(S))^{-1}(A/b)$ est injectif.

(ii) L’application $b' \to b = (i_A^S)^{-1}(b')$, restreinte à l’ensemble des idéaux maximaux (resp. premiers) de $S^{-1}A$, est un isomorphisme (pour la relation d’inclusion) de cet ensemble sur l’ensemble des idéaux de $A$ maximaux parmi ceux qui sont disjoints de $S$ (resp. sur l’ensemble des idéaux premiers de $A$ disjoints de $S$).

(iii) Si $q'$ est un idéal premier de $S^{-1}A$ et si $q = (i_A^S)^{-1}(q')$, il existe un isomorphisme de l’anneau de fractions $A_q$ sur l’anneau $(S^{-1}A)_{q'}$, qui transforme $a/b$ en $(a/1)/(b/1)$ pour $a \in A,\ b \in A - q$.

(i) On peut identifier $(f(S))^{-1}(A/b)$ à $S^{-1}(A/b)$ au moyen de l’isomorphisme canonique entre ces deux modules (no 2, prop. 6). La suite exacte $0 \to b \to A \to A/b \to 0$ fournit alors une suite exacte $0 \to S^{-1}b \to S^{-1}A \to S^{-1}(A/b) \to 0$ (no 4, th. 1) dont l’existence démontre la première assertion de (i), compte tenu de ce que $b' = S^{-1}b$. Puisque $b$ est saturé pour $S$, les conditions $a \in A,\ s \in S,\ as \in b$ entraînent $a \in b$; l’homothétie de rapport $s$ dans $A/b$ est donc injective, ce qui prouve la deuxième assertion de (i).

(ii) Remarquons d’abord que la relation $b' = S^{-1}A$ équivaut à la relation $b \cap S \neq \emptyset$, cette dernière exprimant que $b'$ contient des éléments inversibles de $S^{-1}A$. Il résulte du no 4, prop. 10 (iii) que $b' \to b = (i_A^S)^{-1}(b')$ est un isomorphisme (pour la relation d’inclusion) de l’ensemble des idéaux de $S^{-1}A$ distincts de $S^{-1}A$ sur l’ensemble $\mathfrak{F}$ des idéaux de $A$ disjoints de $S$ et vérifiant la condition (MS) de la prop. 10. Si $b'$ est maximal (resp. premier), il est clair que $b$ est maximal dans $\mathfrak{F}$ (resp. premier) et réciproquement (en vertu de (i)). D’autre part, si $r$ est un idéal de $A$ disjoint de $S$, son saturé $r_1$ pour $S$ est un idéal de $A$ contenant $r$ et qui est disjoint de $S$: aucun élément $a \in S$ ne peut en effet être tel que $sa \in r$, pour un $s \in S$, car on en déduirait $sa \in r \cap S$. On en conclut que, si $r$ est maximal parmi les idéaux de $A$ disjoints de $S$, il est maximal dans $\mathfrak{F}$. De même, si $r$ est un idéal premier disjoint de $S$, il vérifie la condition (MS) du no 4, prop. 10 par définition des idéaux premiers, donc appartient à $\mathfrak{F}$. Ceci achève de prouver (ii).

(iii) Supposons $q'$ premier, de sorte qu’il en est de même de $q$. L’ensemble $T = A - q$ est une partie multiplicative de $A$ qui contient S, d'où ST = T. Posons T' = i_A^S(T) ; il résulte du n° 3, prop. 7, (i), qu'il existe un isomorphisme j et un seul de T^{-1}A = A_q sur T'^{-1}(S^{-1}A) tel que j(a/b) = (a/1)/(b/1), pour a ∈ A et b ∈ T. Il est d'autre part évident que T' ne rencontre pas q' ; inversement, soit a/s ∈ S^{-1}A ; puisque 1/s est inversible dans S^{-1}A, la condition a/s ∉ q' équivaut à i_A^S(a) = a/1 ∉ q', donc à a ∉ q ; il en résulte que S^{-1}A - q' = S^{-1}T', et, en vertu de la prop. 8 du n° 3, on a donc T'^{-1}(S^{-1}A) = (S^{-1}A)_{q'}.

C. Q. F. D.

L'isomorphisme défini dans (iii) est dit canonique. Lorsque A est intègre, les isomorphismes canoniques de A_q et de (S^{-1}A)_{q'} sur des sous-anneaux du corps des fractions K de A ont même image.

#### Remarque {#ac-ii-s2-n5-rem-1 .statement}

Pour qu'un idéal a de A soit tel que S^{-1}a = S^{-1}A (ou, ce qui revient au même en vertu du n° 4, th. 1, que S^{-1}(A/a)=0), il faut et il suffit que a ∩ S ≠ Ø, comme il résulte aussitôt des définitions.

#### Corollaire 1 {#ac-ii-s2-prop-11-cor-1 .statement}

Soient A un anneau, S une partie multiplicative de A. Tout idéal p de A, maximal parmi ceux qui sont disjoints de S, est premier.

En effet, en vertu de la prop. 11, l'hypothèse sur p signifie que p = (i_A^S)^{-1}(m'), où m' est un idéal maximal de S^{-1}A ; comme m' est premier, il en est de même de p.

#### Corollaire 2 {#ac-ii-s2-prop-11-cor-2 .statement}

Soient A un anneau, S une partie multiplicative de A. Pour tout idéal a de A ne rencontrant pas S, il existe un idéal premier contenant a et ne rencontrant pas S.

En effet, on a S^{-1}a ≠ S^{-1}A (Remarque), donc il existe un idéal maximal de S^{-1}A contenant S^{-1}a (Alg., chap. I, § 8, n° 7, th. 2) et le corollaire résulte de la prop. 11, (ii).

#### Corollaire 3 {#ac-ii-s2-prop-11-cor-3 .statement}

Soient A, B deux anneaux, ρ un homomorphisme de A dans B, et p un idéal premier de A. Pour qu'il existe un idéal premier p' de B tel que ρ^{-1}(p') = p, il faut et il suffit que ρ^{-1}(B_ρ(p)) = p.

S'il existe un idéal p' de B tel que ρ^{-1}(p') = p, on a ρ(p) ⊂ p', d'où $B_\rho(p) \subset p'$ et $\rho^{-1}(B_\rho(p)) \subset \rho^{-1}(p') \subset p$; comme l'inclusion opposée est évidente, on a bien $\rho^{-1}(B_\rho(p)) = p$. Inversement, supposons que l'on ait $\rho^{-1}(B_\rho(p)) = p$, et considérons la partie multiplicative $S = \rho(A - p)$ de $B$; l'hypothèse montre que $S \cap B_\rho(p) = \emptyset$; en vertu du cor. 2, il existe un idéal premier $p'$ de $B$ contenant $B_\rho(p)$ et disjoint de $S$; alors $\rho^{-1}(p')$ contient $p$ et ne peut contenir aucun élément de $A - p$, donc est égal à $p$.

#### Corollaire 4 {#ac-ii-s2-prop-11-cor-4 .statement}

*Soient A et B deux anneaux, $\rho$ un homomorphisme de A dans B.*

(i) *Supposons qu'il existe un B-module E tel que $\rho_*(E)$ soit un A-module fidèlement plat. Alors, pour tout idéal premier $p$ de A, il existe un idéal premier $p'$ de B tel que $\rho^{-1}(p') = p$.*

(ii) *Inversement, supposons que B soit un A-module plat. Alors, si, pour tout idéal premier $p$ de A, il existe un idéal $p'$ de B tel que $\rho^{-1}(p') = p$, B est un A-module fidèlement plat.*

(i) L'hypothèse entraîne que, pour tout idéal $a$ de A, on a $\rho^{-1}(B_\rho(a)) = a$ (chap. I, § 3, no 5, prop. 8, (ii)), et il suffit d'appliquer le cor. 3.

(ii) Il suffit de montrer que pour tout idéal maximal $m$ de A, il existe un idéal maximal $m'$ de B tel que $\rho^{-1}(m') = m$ (chap. I, § 3, no 5, prop. 9, e)). Or il existe par hypothèse un idéal $q$ de B tel que $\rho^{-1}(q) = m$; comme $q \neq B$, il existe un idéal maximal $m'$ de B contenant $q$, et par suite $\rho^{-1}(m') \supset m$; mais comme $\rho^{-1}(m')$ ne peut contenir 1, on a $\rho^{-1}(m') = m$.

#### Corollaire 5 {#ac-ii-s2-prop-11-cor-5 .statement}

*Soient A un anneau, S une partie multiplicative de A, B un anneau tel que $i_A^S(A) \subset B \subset S^{-1}A$. Soit q un idéal premier de B tel que l'idéal premier $p = (i_A^S)^{-1}(q)$ de A ne rencontre pas S, et soit $p'$ l'idéal premier $S^{-1}p$ de $S^{-1}A$. On a alors $p' \cap B = q$.*

Soit $S' = i_A^S(S)$; on a défini un isomorphisme canonique de ${S'}^{-1}B$ sur $S^{-1}A$ (no 1, cor. 4 de la prop. 2); nous identifierons ces deux anneaux au moyen de cet isomorphisme. Comme $q \cap S' = \emptyset$, $q' = {S'}^{-1}q$ est l'unique idéal premier de $S^{-1}A = {S'}^{-1}B$ tel que $q' \cap B = (i_B^{S'})^{-1}(q') = q$ (prop. 11, (ii)), d'où $(i_A^S)^{-1}(q') = p$; par suite on a $q' = p'$ (prop. 11, (ii)).

Avec les notations du cor. 5, on a des isomorphismes canoniques de $A_p$ et de $B_q$ sur $(S^{-1}A)_{p'}$ (prop. 11, (iii)), d’où un isomorphisme canonique $A_p \to B_q$.

### 6. Nilradical et idéaux premiers minimaux.

Dans un anneau (commutatif) $A$, l’ensemble des éléments nilpotents est un idéal, car si $x, y$ sont des éléments de $A$ tels que $x^m = y^n = 0$, on a $(x + y)^{m+n} = 0$ en vertu de la formule du binôme.

#### Définition 4 {#ac-ii-s2-def-4 .statement}

On appelle nilradical d’un anneau (commutatif) $A$ l’idéal des éléments nilpotents de $A$. On appelle racine d’un idéal $a$ de $A$ l’image réciproque, par l’application canonique $A \to A/a$, du nilradical de $A/a$.

Nous noterons souvent $r(a)$ la racine d’un idéal $a$ de $A$.
Dire qu’un élément $x \in A$ appartient à la racine de $a$ signifie donc qu’il existe un entier $n > 0$ tel que $x^n \in a$. Si $f$ est un homomorphisme de $A$ dans un anneau $B$, $b$ un idéal de $B$, la racine de $f^{-1}(b)$ est l’image réciproque par $f$ de la racine de $b$, car dire que $x^n \in f^{-1}(b)$ signifie que $(f(x))^n \in b$.

Le nilradical d’un anneau $A$ est contenu dans son radical ($Alg.$, chap. VIII, § 6, no 3, cor. 3 du th. 1) mais peut en être distinct ; il lui est toutefois égal lorsque $A$ est artinien ($Alg.$, chap. VIII, § 6, no 4, th. 3).

Nous dirons qu’un idéal premier $p$ d’un anneau $A$ est un idéal premier minimal s’il est minimal dans l’ensemble des idéaux premiers de $A$, ordonné par inclusion.

#### Proposition 12 {#ac-ii-s2-prop-12 .statement}

Soient $p$ un idéal premier minimal d’un anneau $A$. Pour tout $x \in p$, il existe un $s \in A - p$ et un entier $k > 0$ tels que $sx^k = 0$.

En effet, l’ensemble $S$ des éléments de la forme $sx^k$ ($k$ entier $\geqslant 0$, $s \in A - p$) est une partie multiplicative de $A$. Si on avait $0 \in S$, il existerait un idéal premier $p'$ disjoint de $S$ (no 5, cor. 2 de la prop. 11). On aurait alors $p' \subset p$ et $p' \neq p$ puisque $x \notin p'$, contrairement à l’hypothèse que $p$ est minimal.

#### Proposition 13 {#ac-ii-s2-prop-13 .statement}

Le nilradical d’un anneau $A$ est l’intersection de tous les idéaux premiers de $A$, et c’est aussi l’intersection des idéaux premiers minimaux de $A$.

Il est clair que, si $x \in A$ est nilpotent, il est contenu dans tout idéal premier de $A$ (§ 1, n° 1, déf. 1). Inversement, soit $x$ un élément non nilpotent de $A$; l’ensemble $S$ des $x^k$ ($k$ entier $\geqslant 0$) est alors une partie multiplicative de $A$ ne contenant pas $0$, donc il existe un idéal premier $p$ de $A$ ne rencontrant pas $S$ (n° 5, cor. 2 de la prop. 11), et $a fortiori$ $x \notin p$; ceci établit la première assertion. Pour démontrer la seconde, il suffit de prouver le

#### Lemme 2 {#ac-ii-s2-lem-2 .statement}

Tout idéal premier $p$ d’un anneau $A$ contient un idéal premier minimal de $A$.

Il suffit, en vertu du th. de Zorn, de montrer que l’ensemble $P$ des idéaux premiers, ordonné par la relation $\supset$, est *inductif*. Or, si $G$ est une partie totalement ordonnée non vide de $P$, l’intersection $p_0$ des idéaux $p \in G$ est encore un idéal premier : en effet, si $x \notin p_0$ et $y \notin p_0$, il existe un idéal $p \in G$ tel que $x \notin p$ et $y \notin p$, d’où $xy \notin p$ et $a fortiori$ $xy \notin p_0$.

#### Remarque {#ac-ii-s2-n6-rem-1 .statement}

Au § 4, n° 3, cor. 3 de la prop. 14, nous montrerons que dans un anneau *noethérien* l’ensemble des idéaux premiers minimaux est *fini* ; nous verrons en outre plus tard que toute suite décroissante d’idéaux premiers dans un anneau noethérien est *stationnaire*.

#### Corollaire 1 {#ac-ii-s2-lem-2-cor-1 .statement}

La racine d’un idéal $a$ d’un anneau $A$ est l’intersection des idéaux premiers contenant $a$, et c’est aussi l’intersection des éléments minimaux de cet ensemble d’idéaux premiers.

#### Corollaire 2 {#ac-ii-s2-lem-2-cor-2 .statement}

Pour tout idéal $a$ d’un anneau $A$, notons $r(a)$ la racine de $a$. Alors, pour deux idéaux $a, b$ de $A$, on a
$$
r(a \cap b) = r(ab) = r(a) \cap r(b);
$$
en particulier, si $a \subset b$, on a $r(a) \subset r(b)$.

En effet, pour qu’un idéal premier contienne $a \cap b$ (ou $ab$), il faut et il suffit qu’il contienne l’un des idéaux $a, b$ ($§ 1$, no 1, prop. 1).

#### Proposition 14 {#ac-ii-s2-prop-14 .statement}

*Pour que deux idéaux $a, b$ d’un anneau $A$ soient étrangers, il faut et il suffit que leurs racines $r(a)$ et $r(b)$ le soient.*

La nécessité de la condition est évidente puisque $a \subset r(a)$ et $b \subset r(b)$; la condition est suffisante en vertu du $§ 1$, no 2, prop. 3.

#### Proposition 15 {#ac-ii-s2-prop-15 .statement}

*Dans un anneau $A$, soient $a$ un idéal et $b$ un idéal de type fini contenu dans la racine de $a$. Alors il existe un entier $k > 0$ tel que $b^k \subset a$.*

Soit $(b_i)_{1 \leq i \leq n}$ un système de générateurs de $b$. Par hypothèse, il existe un entier $h$ tel que $b_i^h \in a$ pour $1 \leq i \leq n$. Quand on développe un produit de $nh$ éléments dont chacun est combinaison linéaire des $b_i$ à coefficients dans $A$, chaque terme est multiple d’un produit de $nh$ facteurs dont chacun est égal à un $b_i$; parmi ces facteurs, $h$ au moins correspondent à un même indice $i$, donc le produit appartient à $a$, et le nombre $k = nh$ répond à la question.

#### Corollaire {#ac-ii-s2-n6-cor-1 .statement}

*Dans un anneau noethérien, le nilradical est un idéal nilpotent.*

#### Proposition 16 {#ac-ii-s2-prop-16 .statement}

*Soient $B$ un anneau, $A$ un sous-anneau de $B$. Pour tout idéal premier minimal $p$ de $A$, il existe un idéal premier minimal $q$ de $B$ tel que $q \cap A = p$.*

Posons $S = A - p$; l’anneau $A_p = S^{-1}A$ s’identifie alors à un sous-anneau de $S^{-1}B$ (no 1, prop. 2), et d’autre part $A_p$ ne possède qu’un seul idéal premier $p'$ puisque $p$ est minimal (no 5, prop. 11). Comme $S^{-1}B$ n’est pas réduit à 0 (puisque il contient $A_p$), il possède au moins un idéal premier $r'$, et on a alors nécessairement $r' \cap A_p = p'$; si $j = i_B^s$, et si on pose $r = j^{-1}(r')$, on a alors

$$
i_A^s(r \cap A) \subset r' \cap A_p = p'
$$

donc $r \cap A \subset p$, et comme $p$ est minimal, $r \cap A = p$; en outre $r$ est premier dans $B$; si $q$ est un idéal premier minimal de $B$ contenu dans r (lemme 1), on a a fortiori q ∩ A ⊂ p, donc q ∩ A = p puisque p est minimal.

#### Définition 5 {#ac-ii-s2-def-5 .statement}

On dit qu’un anneau A est réduit si son nilradical est réduit à 0, autrement dit si aucun élément ≠ 0 de A n’est nilpotent.

Si $\mathfrak{N}$ est le nilradical d’un anneau A, $A/\mathfrak{N}$ est réduit, car si la classe mod. $\mathfrak{N}$ d’un élément $x \in A$ est nilpotente dans $A/\mathfrak{N}$, cela signifie que $x^h \in \mathfrak{N}$ pour un entier h, donc $x^{hk} = 0$ pour un entier k, et $x \in \mathfrak{N}$.

#### Proposition 17 {#ac-ii-s2-prop-17 .statement}

Soient A un anneau, $\mathfrak{N}$ son nilradical. Pour toute partie multiplicative S de A, $S^{-1}\mathfrak{N}$ est le nilradical de $S^{-1}A$. En particulier, si A est réduit, $S^{-1}A$ est réduit.

En effet, si $x \in A$, $s \in S$ sont tels que $(x/s)^n = x^n/s^n = 0$, il existe $s' \in S$ tel que $s'x^n = 0$ (no 1, Remarque 3) et a fortiori $(s'x)^n = 0$, donc $s'x \in \mathfrak{N}$ et $x/s = s'x/s's' \in S^{-1}\mathfrak{N}$; la réciproque est immédiate.

### 7. Modules de fractions de produits tensoriels et de modules d’homomorphismes.

#### Proposition 18 {#ac-ii-s2-prop-18 .statement}

Soient A un anneau, S une partie multiplicative de A.

(i) Si M et N sont deux A-modules, les $S^{-1}A$-modules $(S^{-1}M) \otimes_A N$, $M \otimes_A (S^{-1}N)$, $(S^{-1}M) \otimes_{S^{-1}A} (S^{-1}N)$ et $S^{-1}(M \otimes_A N)$ sont canoniquement isomorphes.

(ii) Si $M'$ et $N'$ sont deux $S^{-1}A$-modules, l’homomorphisme canonique
$$
M' \otimes_A N' \to M' \otimes_{S^{-1}A} N'
$$
déduit de l’application A-bilinéaire $(x', y') \to x' \otimes y'$ de $M' \times N'$ dans $M' \otimes_{S^{-1}A} N'$ est bijectif.

L’assertion (i) est conséquence immédiate de la définition $S^{-1}M = M \otimes_A S^{-1}A$ et de l’associativité du produit tensoriel, qui donne à des isomorphismes canoniques près
$$
(S^{-1}M) \otimes_{S^{-1}A} (S^{-1}N) = (S^{-1}M) \otimes_{S^{-1}A} (S^{-1}A \otimes_A N) = (S^{-1}M) \otimes_A N
$$
$$
= (S^{-1}A) \otimes_A M \otimes_A N = S^{-1}(M \otimes_A N).
$$

Pour prouver (ii), notons d’abord que dans M’ et N’, considérés comme A-modules, les homothéties produites par les éléments s ∈ S sont bijectives, donc on a M’ = S^{-1}M’ et N’ = S^{-1}N’ (n° 2, Remarque 4) et de même S^{-1}(M’ \otimes_A N’) = M’ \otimes_A N’ ; (ii) est alors un cas particulier de (i).

#### Corollaire {#ac-ii-s2-n7-cor-1 .statement}

Soient M un A-module, a un idéal de A. Les sous-S^{-1}A-modules (S^{-1}a)(S^{-1}M), a(S^{-1}M), (S^{-1}a)j(M) (où j : M → S^{-1}M est l’application canonique) et S^{-1}(aM) de S^{-1}M sont identiques. En particulier, si a et b sont deux idéaux de A, on a (S^{-1}a)(S^{-1}b) = a(S^{-1}b) = (S^{-1}a)b = S^{-1}(ab).

#### Remarque {#ac-ii-s2-n7-rem-1 .statement}

Soient M, N, P trois A-modules, f : M × N → P une application A-bilinéaire, S^{-1}f : (S^{-1}M) × (S^{-1}N) → S^{-1}P l’application S^{-1}A-bilinéaire obtenue à partir de f par extension à S^{-1}A de l’anneau des scalaires (Alg., chap. IX, § 1, n° 4, prop. 1). Soient i : M → S^{-1}M, j : N → S^{-1}N les homomorphismes canoniques ; il est immédiat que, si Q est le sous-A-module de P engendré par f(M × N), S^{-1}Q est le sous-S^{-1}A-module de S^{-1}P engendré par (S^{-1}f)(i(M) × j(N)).

#### Proposition 19 {#ac-ii-s2-prop-19 .statement}

Soient A un anneau, S une partie multiplicative de A.

(i) Si M et N sont deux A-modules, et si M est de type fini (resp. de présentation finie), l’homomorphisme canonique (chap. I, § 2, n° 10, formule (10))

$$
S^{-1}\mathrm{Hom}_A(M, N) \to \mathrm{Hom}_{S^{-1}A}(S^{-1}M, S^{-1}N)
$$

est injectif (resp. bijectif).

(ii) Si M’, N’ sont deux S^{-1}A-modules, l’injection canonique

$$
\mathrm{Hom}_{S^{-1}A}(M', N') \to \mathrm{Hom}_A(M', N')
$$

est bijective.

Comme S^{-1}A est un A-module plat, (i) est un cas particulier du chap. I, § 2, n° 10, prop. 11. D’autre part, on a déjà remarqué que tout A-homomorphisme de S^{-1}A-modules est nécessairement un S^{-1}A-homomorphisme, au cours de la démonstration de la prop. 3 du n° 2 ; d’où (ii).

#### Proposition 20 {#ac-ii-s2-prop-20 .statement}

Soient $A, A'$ deux anneaux, $\rho : A \to A'$ un homomorphisme, $S$ une partie multiplicative de $A$, $S' = \rho(S)$, $\rho' : S^{-1}A \to {S'}^{-1}A'$ l’homomorphisme correspondant à $\rho$ (n° 1, prop. 2).

(i) Pour tout $A'$-module $M'$, il existe un $S^{-1}A$-isomorphisme et un seul
$$
j : S^{-1}\rho_*(M') \to \rho'_*({S'}^{-1}M')
$$
tel que $j(m'/s) = m'/\rho(s)$ pour $m' \in M', s \in S$.

(ii) Pour tout $A$-module $M$, il existe un isomorphisme et un seul
$$
j' : (S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') \to {S'}^{-1}(M \otimes_A A')
$$
de ${S'}^{-1}A'$-modules, tel que $j'((m/s) \otimes (a'/s')) = (m \otimes a')/(\rho(s)s')$.

(i) Si on considère ${S'}^{-1}M'$ comme $A$-module au moyen de l’homomorphisme composé $i_{M'}^{S'} \circ \rho$, les homothéties produites par les éléments de $S$ sont bijectives, donc il existe un homomorphisme $j$ et un seul possédant la propriété énoncée (n° 2, prop. 3). Comme $\rho(S) = S'$, $j$ est surjectif ; en outre, si $m' \in M', s \in S, m'/\rho(s) = 0$, il existe $t' \in S'$ tel que $t'm' = 0$; comme il existe $t \in S$ tel que $\rho(t) = t'$, on a $t.m' = 0$ dans $\rho_*(M')$, donc $m'/s = 0$ dans $S^{-1}\rho_*(M')$.

(ii) Comme $(S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') = (M \otimes_A S^{-1}A) \otimes_{S^{-1}A} ({S'}^{-1}A')$, et ${S'}^{-1}(M \otimes_A A') = (M \otimes_A A') \otimes_{A'} ({S'}^{-1}A')$, l’existence de $j'$ résulte de l’associativité du produit tensoriel.

### 8. Application aux algèbres.

Soient $A$ un anneau, $B$ une $A$-algèbre (non nécessairement associative ni commutative, et n’ayant pas nécessairement d’élément unité), $S$ une partie multiplicative de $A$. On sait que sur le $S^{-1}A$-module $S^{-1}B = B \otimes_A S^{-1}A$ on définit canoniquement une structure de $S^{-1}A$-algèbre, dite obtenue par extension à $S^{-1}A$ de l’anneau des scalaires ($Alg.$, chap. III, § 3) et pour laquelle le produit $(x/s)(y/t)$ est égal à $(xy)/st$. Si $e$ est élément unité de $B$, $e/1$ est élément unité de $S^{-1}B$, et si $B$ est associative (resp. commutative), il en est de même de $S^{-1}B$.

Soient $A$ un anneau, $M$ un $A$-module ; désignons par $T(M)$ (resp. $\wedge (M), S(M)$) l’algèbre tensorielle (resp. l’algèbre extérieure, l’algèbre symétrique) de $M$ ($Alg.$, chap. III, 3e éd.). On sait que, pour toute A-algèbre commutative C, il existe un isomorphisme et un seul $j$ de $T(M) \otimes_A C$ sur $T(M \otimes_A C)$ (resp. de $\wedge (M) \otimes_A C$ sur $\wedge (M \otimes_A C)$, de $S(M) \otimes_A C$ sur $S(M \otimes_A C)$) tel que $j(x \otimes 1) = x \otimes 1$ pour $x \in M$, $M$ étant canoniquement identifié à un sous-module de $T(M)$ (resp. $\wedge (M), S(M)$) (*loc. cit.*). On voit donc en particulier que, pour toute partie multiplicative R de A, on a des *isomorphismes canoniques*

$$
R^{-1}T(M) \to T(R^{-1}M), \quad R^{-1}\wedge(M) \to \wedge(R^{-1}M), \quad R^{-1}S(M) \to S(R^{-1}M)
$$

qui se réduisent à l’identité dans $R^{-1}M$.

### 9. Modules de fractions de modules gradués.

Soient A un anneau gradué, M un A-module gradué, $\Delta$ le monoïde des degrés ; nous supposerons dans ce n° que $\Delta$ est un *groupe*. Rappelons (*Alg.*, chap. II, 3e éd., § 11) que A et M sont respectivement sommes directes de groupes additifs

$$
A = \bigoplus_{i \in \Delta} A_i, \qquad M = \bigoplus_{i \in \Delta} M_i
$$

avec $A_i A_j \subset A_{i+j}$ et $A_i M_j \subset M_{i+j}$ quels que soient $i, j$ dans $\Delta$. Soit S une partie multiplicative de A *dont tous les éléments sont homogènes*. Pour tout $i \in \Delta$, nous poserons $S_i = S \cap A_i$, et nous noterons $(S^{-1}M)_i$ l’ensemble des éléments $m'$ de $S^{-1}M$ pour lesquels il existe des éléments $j, k$ de $\Delta$, un élément $m \in M_j$ et un élément $s \in S_k$ tels que $j - k = i$ et $m' = m/s$. Si $(m'_q)_{1 \leq q \leq r}$ est une famille finie d’éléments de $S^{-1}M$ telle que $m'_q \in (S^{-1}M)_{j(q)}$, il existe des éléments $j(q) \in \Delta$ et $k \in \Delta$, des éléments $m_q \in M_{j(q)}$ ($1 \leq q \leq r$) et $s \in S_k$ tels que $m'_q = m_q/s$ pour $1 \leq q \leq r$ (n° 1, *Remarque* 2).

#### Proposition 21 {#ac-ii-s2-prop-21 .statement}

*L’anneau* $S^{-1}A$ *muni de la famille* $((S^{-1}A)_i)$ *est un anneau gradué*, et $S^{-1}M$ *muni de la famille* $((S^{-1}M)_i)$ *est un module gradué sur l’anneau gradué* $S^{-1}A$. *Les applications canoniques* $i^S_A$ *et* $i^S_M$ *sont homogènes de degré* 0.

Soient $m \in M_j$, $s \in S_k$, $m' \in M_{j'}$, $s' \in S_{k'}$, et supposons que $j - k = j' - k' = i$; alors $(m/s) - (m'/s') = (s'm - sm')/ss'$ et on a $s'm - sm' \in M_{j+k'} = M_{j'+k}$ et $ss' \in S_{k+k'}$, donc $(m/s) - (m'/s') \in (S^{-1}M)_i$ par définition ; ceci montre que les $(S^{-1}M)_i$ sont des sous-groupes additifs de $S^{-1}M$. La somme de ces sous-groupes est $S^{-1}M$ tout entier : en effet, tout $x \in S^{-1}M$ s’écrit $m/s$ où $m \in M, s \in S$; $s$ est *homogène* par hypothèse, et $m$ somme d’éléments homogènes $m_j$; donc $x$ est somme des $m_j/s$, qui appartiennent chacun à un sous-groupe $(S^{-1}M)_i$. Enfin, la somme des $(S^{-1}M)_i$ est directe ; considérons en effet une famille finie d’éléments $x_q (1 \leq q \leq n)$ tels que $x_q \in (S^{-1}M)_{i(q)}$, où les indices $i(q)$ sont distincts, et supposons que $\sum_{q=1}^n x_q = 0$. Chaque $x_q$ s’écrit $x_q = m_q/s$ avec $s \in S_k$ et $m_q \in M_{i(q)+k}$; l’hypothèse entraîne qu’il existe $s' \in S$ tel que $s'\left( \sum_{q=1}^n m_q \right) = 0$; si les $s'm_q$ n’étaient pas tous nuls, on aurait une contradiction puisque, si $s' \in S_d$, on a $s'm_q \in M_{i(q)+d}$, et les $i(q) + d$ sont tous distincts. On en conclut que $x_q = 0$ pour tout indice $q$.

On vérifie immédiatement que, si $a \in (S^{-1}A)_i$ et $x \in (S^{-1}M)_j$, on a $ax \in (S^{-1}M)_{i+j}$. Appliquant ce résultat au cas où $M = A$, on voit d’abord que $S^{-1}A$ est un anneau gradué par les $(S^{-1}A)_i$; on voit ensuite que $S^{-1}M$ est un module gradué sur $S^{-1}A$. Enfin, comme $1 \in A_0$, $i_A^S$ et $i_M^S$ sont homogènes de degré 0.

#### Proposition 22 {#ac-ii-s2-prop-22 .statement}

*Soient A (resp. B) un anneau gradué de type Δ, M (resp. N) un module gradué sur l’anneau gradué A (resp. B), S (resp. T) une partie multiplicative de A (resp. B) dont tous les éléments sont homogènes, $f : A \to B$ un homomorphisme homogène de degré 0 tel que $f(S) \subset T$, $u : M \to N$ une application A-linéaire qui est homogène de degré k. Alors l’homomorphisme $f' : S^{-1}A \to T^{-1}B$ déduit de $f$ (no 1, prop. 2) est homogène et de degré 0, et l’application $(S^{-1}A)$-linéaire $u' : S^{-1}M \to T^{-1}N$ déduite de $f$ et $u$ (no 2, prop. 5) est homogène et de degré k.*

Ceci résulte aussitôt des formules $f'(a/s) = f(a)/f(s)$ et $u'(m/s) = u(m)/f(s)$.

Notons enfin que, si E est une A-algèbre graduée, S une partie multiplicative de A formée d’éléments homogènes, $S^{-1}E$ muni de sa structure de $(S^{-1}A)$-algèbre (no 8) et de la graduation $(S^{-1}E)_i$ est une $S^{-1}A$-algèbre graduée, comme il résulte aussitôt des définitions.

## EXERCICES {#ac-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
