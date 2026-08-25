---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: Groupes de Coxeter et systèmes de Tits
section: 0
section_title: Graphes
appendix: true
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0032-0036
extraction: ocr
subsections:
    - "no": 1
      title: Définitions
      page: 0
      pdf_page: 32
    - "no": 2
      title: Composantes connexes d’un graphe
      page: 0
      pdf_page: 32
    - "no": 3
      title: Forêts et arbres
      page: 0
      pdf_page: 34
statements: 6
exercises: 0
content_sha256: 836ab5146f658366b31603e9aef198d23f7acf8cae07f776d8afc69bc3888484
---

## ANNEXE

# GRAPHES

### 1. Définitions

#### Définition 1 {#lie-iv-a0-def-1 .statement}

On appelle graphe combinatoire (ou simplement graphe, lorsqu’aucune confusion n’en résulte) un couple $\Gamma = (A, S)$, où $S$ est un ensemble, et $A$ une partie de $\mathfrak{P}(S)$ formée d’ensembles à deux éléments.

Soit $\Gamma = (A, S)$ un graphe. Les éléments de $A$ s’appellent les arêtes et ceux de $S$ les sommets de $\Gamma$; on dit que deux sommets $x, y$ sont liés si $\{x, y\}$ est une arête. Un sommet est dit terminal s’il est lié à un sommet au plus, et point de ramification s’il est lié à trois sommets au moins.

Conformément aux définitions générales (Ens. R, § 8), un isomorphisme du graphe $\Gamma$ sur un graphe $\Gamma' = (A', S')$ est une bijection $f$ de $S$ sur $S'$ qui transforme $A$ en $A'$. Un graphe $\Gamma' = (A', S')$ est appelé un sous-graphe de $\Gamma$ si l’on a $S' \subset S$ et $A' \subset A$; on dit que $\Gamma'$ est un sous-graphe plein de $\Gamma$ si l’on a $S' \subset S$ et $A' = A \cap \mathfrak{P}(S')$; il est clair que toute partie de $S$ est l’ensemble des sommets d’un sous-graphe plein de $\Gamma$ et d’un seul.

Pour faciliter la lecture des raisonnements, on représentera un graphe par un dessin composé de points correspondants aux sommets, deux points étant joints par un trait si et seulement si les sommets qu’ils représentent sont liés dans le graphe. Par exemple, la figure

![Un graphe avec quatre sommets a, b, c, d et e, et deux arêtes {a, b}, {b, c}, {c, d}, {c, e}.](https://i.imgur.com/3Q5z5QG.png)

représente un graphe dont les sommets sont $a, b, c, d, e$ et les arêtes $\{a, b\}, \{b, c\}, \{c, d\}$ et $\{c, e\}$.

### 2. Composantes connexes d’un graphe

Soit $\Gamma = (A, S)$ un graphe. Si $a$ et $b$ sont deux sommets, on appelle chemin joignant $a$ à $b$ toute suite $(x_0, \ldots, x_n)$ de sommets de $\Gamma$, avec $x_0 = a, x_n = b$, les sommets $x_i$ et $x_{i+1}$ étant liés pour $0 \leq i < n$; l’entier $n \geq 0$ est la longueur du chemin considéré. On dit que le chemin $(x_0, \ldots, x_n)$ est injectif si l’on a $x_i \neq x_j$ pour $i \neq j$; si un chemin $(x_0, \ldots, x_n)$ joignant $a$ à $b$ est de longueur minimale dans l’ensemble de ces chemins, il est nécessairement injectif : sinon, il existerait $i$ et $j$ avec $0 \leq i < j \leq n$ et $x_i = x_j$ et la suite

$$
(x_0, \ldots, x_i, x_{j+1}, \ldots, x_n)
$$

serait un chemin de longueur $< n$ joignant $a$ à $b$.

La relation « il existe un chemin joignant $a$ à $b$ » entre deux sommets $a$ et $b$ de $\Gamma$ est une relation d’équivalence $R$ dans l’ensemble $S$ des sommets. Les classes d’équivalence pour $R$ s’appellent les composantes connexes de $\Gamma$; on dit que $\Gamma$ est connexe s’il existe dans $S$ au plus une composante connexe, c’est-à-dire si deux sommets quelconques de $\Gamma$ peuvent être joints par au moins un chemin.

#### Proposition 1 {#lie-iv-a0-prop-1 .statement}

*Soient $\Gamma = (A, S)$ un graphe et $(S_\alpha)_{\alpha \in L}$ la famille de ses composantes connexes. On note $\Gamma_\alpha$ le sous-graphe plein de $\Gamma$ ayant $S_\alpha$ pour ensemble de sommets.*

(i) *Pour tout $\alpha$ dans $L$, le graphe $\Gamma_\alpha$ est connexe.*

(ii) *Si $\Gamma' = (A', S')$ est un sous-graphe connexe de $\Gamma$, il existe $\alpha$ dans $L$ tel que $S' \subset S_\alpha$.*

(iii) *Pour $\alpha \neq \beta$, aucun élément de $S_\alpha$ n’est lié dans $\Gamma$ à un élément de $S_\beta$ (autrement dit, toute arête de $\Gamma$ est une arête de l’un des $\Gamma_\alpha$).*

(iv) *Soit $(S'_\lambda)_{\lambda \in M}$ une partition de $S$ telle que pour $\lambda \neq \mu$ aucun élément de $S'_\lambda$ ne soit lié dans $\Gamma$ à un élément de $S'_\mu$; alors chacun des ensembles $S'_\lambda$ est réunion de composantes connexes de $\Gamma$.*

(i) Soient $\alpha$ dans $L$, et $a, b$ dans $S_\alpha$. Il existe donc un chemin $c = (x_0, \ldots, x_n)$ joignant $a$ à $b$ dans $\Gamma$; pour tout $i$ tel que $0 \leq i \leq n$, le chemin $(x_0, \ldots, x_i)$ joint $a$ à $x_i$ dans $\Gamma$, d’où $x_i \in S_\alpha$; finalement, $c$ est un chemin *dans* $\Gamma_\alpha$ joignant $a$ à $b$. Par suite, $\Gamma_\alpha$ est connexe.

(ii) Soient $\Gamma' = (A', S')$ un sous-graphe connexe non vide de $\Gamma$, $a$ un élément de $S'$, $S_\alpha$ la composante connexe de $\Gamma$ contenant $a$. Pour tout $b$ dans $S'$, il existe un chemin $c$ joignant $a$ à $b$ *dans* $\Gamma'$, et *a fortiori* *dans* $\Gamma$. Par suite, on a $S' \subset S_\alpha$.

(iii) Étant donnés $\alpha$ et $\beta$ distincts dans $L$, et des sommets $a \in S_\alpha$ et $b \in S_\beta$, il n’existe aucun chemin joignant $a$ à $b$, et en particulier aucune arête ne joint $a$ à $b$.

(iv) Soient $a$ dans $S'_\lambda$, et $S_\alpha$ la composante connexe de $\Gamma$ contenant $a$; pour tout $b$ dans $S_\alpha$, il existe un chemin $(x_0, \ldots, x_n)$ joignant $a$ à $b$ dans $\Gamma$. Si $i$ est un entier tel que $0 \leq i < n$ et $x_i \in S'_\lambda$, on a $x_{i+1} \in S'_\lambda$ puisque $x_i$ est lié à $x_{i+1}$; par récurrence, on a donc $x_i \in S'_\lambda$ pour $0 \leq i \leq n$ et en particulier $b = x_n$ est dans $S'_\lambda$. On a donc $S_\alpha \subset S'_\lambda$.

#### Corollaire 1 {#lie-iv-a0-prop-1-cor-1 .statement}

*Pour que le graphe $\Gamma = (A, S)$ soit connexe, il faut et il suffit qu’il n’existe aucune partition $(S', S'')$ de $S$ en deux ensembles non vides telle qu’aucun élément de $S'$ ne soit lié dans $\Gamma$ à un élément de $S''$.*

Supposons $\Gamma$ non connexe et soit $S'$ une de ses composantes connexes; l’ensemble $S'' = S - S'$ est non vide d’après la prop. 1, (i) et aucun élément de $S'$ n’est lié dans $\Gamma$ à un élément de $S''$ d’après la prop. 1, (iii).

Supposons $\Gamma$ connexe et soit $(S', S'')$ une partition ayant la propriété de l’énoncé. D’après la prop. 1, (iv), l’ensemble $S'$ contient au moins une composante connexe, d’où $S' = S$ et $S'' = \varnothing$, ce qui est contradictoire.

#### Corollaire 2 {#lie-iv-a0-prop-1-cor-2 .statement}

Pour qu’une partie $S'$ de $S$ soit réunion de composantes connexes, il faut et il suffit qu’aucun sommet appartenant à $S'$ ne soit lié à un sommet appartenant à $S - S'$.

La condition est suffisante d’après la prop. 1, (iv). Elle est nécessaire d’après la prop. 1, (iii).

### 3. Forêts et arbres

Soit $\Gamma = (A, S)$ un graphe. On appelle circuit dans $\Gamma$ toute suite
$$
(x_1, \ldots, x_n)
$$
de sommets distincts de $\Gamma$, avec $n \geq 3$, $x_i$ lié à $x_{i+1}$ pour $1 \leq i < n$ et $x_n$ lié à $x_1$. On dit que $\Gamma$ est une forêt s’il n’existe aucun circuit dans $\Gamma$; tout sous-graphe de $\Gamma$ est alors une forêt. Une forêt connexe s’appelle un arbre; les composantes connexes d’une forêt sont donc des arbres.

#### Proposition 2 {#lie-iv-a0-prop-2 .statement}

Soit $\Gamma = (A, S)$ une forêt n’ayant qu’un nombre fini de sommets.
(i) Si $\Gamma$ possède au moins un sommet, il admet un sommet terminal.
(ii) Si $\Gamma$ possède au moins deux sommets, il existe une partition $(S', S'')$ de l’ensemble des sommets en deux parties non vides telle que deux sommets distincts appartenant tous deux à $S'$ ou tous deux à $S''$ ne soient jamais liés.

Supposons qu’il existe au moins un sommet dans $\Gamma$, et soit $(x_0, \ldots, x_n)$ un chemin injectif de longueur maximale dans $\Gamma$. Le sommet $x_0$ ne peut être lié à un sommet $y$ distinct de $x_0, x_1, \ldots, x_n$ sinon il existerait dans $\Gamma$ un chemin injectif de longueur $n + 1$, à savoir $(y, x_0, \ldots, x_n)$. Le sommet $x_0$ n’est lié à aucun sommet $x_i$ avec $2 \leq i \leq n$, sinon $(x_0, x_1, \ldots, x_i)$ serait un circuit dans la forêt $\Gamma$. Donc $x_0$ est terminal.

On démontrera (ii) par récurrence sur le nombre $m$ de sommets de $\Gamma$, le cas $m = 2$ étant trivial. Supposons donc $m \geq 3$ et l’assertion (ii) prouvée pour les graphes à $m - 1$ sommets. Soit $a$ un sommet terminal de $\Gamma$ (cf. (i)). Appliquons l’hypothèse de récurrence au sous-graphe plein de $\Gamma$ ayant pour sommets les sommets $x \neq a$ de $\Gamma$; il existe donc deux parties non vides et disjointes $S'_1$ et $S''_1$ de $S$ avec $S'_1 \cup S''_1 = S - \{a\}$, telles que deux sommets distincts de $S'_1$ (resp. $S''_1$) ne soient jamais liés. Comme $a$ est lié à un sommet au plus de $\Gamma$, on peut supposer par exemple qu’il n’est lié à aucun sommet de $S''_1$; la partition $(S'_1, S''_1 \cup \{a\})$ de $S$ répond alors à la question. C.Q.F.D.

Pour tout entier $n \geq 1$, on note $A_n$ le graphe dont les sommets sont les entiers $1, 2, \ldots, n$ et les arêtes les parties $\{i, j\}$ avec $i - j = \pm 1$:

$$
\begin{array}{cccccc}
1 & 2 & 3 & \cdots & n-1 & n \\
\circ -- \circ -- \circ -- \cdots -- \circ -- \circ
\end{array}
$$

On dit qu’un graphe $\Gamma$ est une chaîne de longueur $m \geqslant 0$ s’il est isomorphe à $A_{m+1}$; ceci équivaut à l’existence dans $\Gamma$ d’un chemin injectif $(x_0, \ldots, x_m)$ contenant tous les sommets, les sommets $x_i$ et $x_j$ n’étant pas liés lorsque $|j - i| > 1$.

#### Proposition 3 {#lie-iv-a0-prop-3 .statement}

Pour qu’un graphe soit une chaîne, il faut et il suffit que le nombre de ses sommets soit fini et non nul, et qu’il soit un arbre sans point de ramification.

Supposons que le graphe $\Gamma$ soit une chaîne $(x_0, \ldots, x_m)$ avec les propriétés énumérées avant l’énoncé de la prop. 3. Il est clair qu’un sommet de $\Gamma$ est lié à deux sommets au plus. Pour $i < j$, le chemin $(x_i, \ldots, x_j)$ extrait du chemin $(x_0, \ldots, x_m)$ joint $x_i$ à $x_j$; donc $\Gamma$ est connexe. Enfin, soit $(x_{p_1}, \ldots, x_{p_n})$ un circuit dans $\Gamma$; soit $p_k$ le plus petit parmi les entiers distincts $p_1, \ldots, p_n$. Il existe $i$ et $j$ distincts tels que $x_{p_k}$ soit lié à $x_{p_i}$ et $x_{p_j}$: cela résulte de la définition d’un circuit. Comme on a $p_k < p_i$ et $p_k < p_j$, on a nécessairement $p_i = p_j = p_k + 1$, ce qui est contradictoire puisque $p_1, \ldots, p_n$ sont distincts. Il n’y a donc aucun circuit dans $\Gamma$.

Réciproquement, soit $\Gamma$ un arbre sans point de ramification, à un nombre fini non nul de sommets, et soit $(x_0, \ldots, x_m)$ un chemin injectif de longueur maximale dans $\Gamma$. Notons $T$ l’ensemble des sommets autres que $x_0, \ldots, x_m$. Un sommet $b \in T$ ne peut être lié à un sommet $x_i$; il y a en effet trois possibilités :

a) $i = 0$, mais alors $(b, x_0, \ldots, x_m)$ serait un chemin injectif de longueur $m + 1$ dans $\Gamma$;
b) $i = m$, mais alors $(x_0, \ldots, x_m, b)$ serait un chemin injectif de longueur $m + 1$ dans $\Gamma$;
c) $0 < i < m$, mais alors $x_i$ serait lié aux trois sommets distincts $x_{i-1}, x_{i+1}$ et $b$.

Comme $\Gamma$ est connexe, $T$ est vide d’après le cor. 1 de la prop. 1. Par ailleurs, s’il existait $i, j$ tels que $j - i > 1$ et que $x_i, x_j$ soient liés, on aurait un circuit $(x_i, x_{i+1}, \ldots, x_j)$ dans $\Gamma$. Donc $\Gamma$ est une chaîne.

Exercises
