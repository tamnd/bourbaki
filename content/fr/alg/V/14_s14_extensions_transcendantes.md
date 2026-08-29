---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 14
section_title: EXTENSIONS TRANSCENDANTES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.161-A V.164
pdf_pages: 0205-0217, 0265-0268
extraction: ocr
subsections:
    - "no": 1
      title: Familles algébriquement libres. Extensions pures
      page: 101
      pdf_page: 205
    - "no": 2
      title: Bases de transcendance
      page: 103
      pdf_page: 207
    - "no": 3
      title: Degré de transcendance d’une extension
      page: 105
      pdf_page: 209
    - "no": 4
      title: Prolongement d’isomorphismes
      page: 106
      pdf_page: 210
    - "no": 5
      title: Extensions algébriquement disjointes
      page: 108
      pdf_page: 212
    - "no": 6
      title: Familles algébriquement libres d’extensions
      page: 110
      pdf_page: 214
    - "no": 7
      title: Extensions de type fini
      page: 112
      pdf_page: 216
statements: 51
exercises: 20
content_sha256: 8f8fcfbd50502d9991e793039c34c47efda5c3ea0d1d85dca2b46a7d78412a82
---

## § 14. EXTENSIONS TRANSCENDANTES

### 1. Familles algébriquement libres. Extensions pures

Rappelons (IV, p. 4) la définition suivante :

#### Définition 1 {#alg-v-s14-def-1 .statement}

Soit E une extension d’un corps K ; on dit qu’une famille x = (x_i)_{i∈I} d’éléments de E est algébriquement libre sur K si les monômes x^α = ∏_{i∈I} x_i^{α_i} par rapport aux x_i (pour α = (α_i)_{i∈I} dans N^{(I)}) sont linéairement indépendants sur K. On dit qu’elle est algébriquement liée sur K dans le cas contraire.

La définition 1 peut encore s’exprimer comme suit :

#### Proposition 1 {#alg-v-s14-prop-1 .statement}

Pour qu’une famille $(x_i)_{i \in I}$ d’éléments d’une extension $E$ d’un corps $K$ soit algébriquement libre sur $K$, il faut et il suffit que la relation $f((x_i)) = 0$, où $f$ est un polynôme de $K[X_i]_{i \in I}$, entraîne $f = 0$.

#### Définition 2 {#alg-v-s14-def-2 .statement}

Soit $E$ une extension d’un corps $K$. Une famille $(x_i)_{i \in I}$ d’éléments de $E$ est appelée une base pure de $E$ (sur $K$) si elle est algébriquement libre et si l’on a $E = K(x_i)_{i \in I}$. On dit que $E$ est une extension pure de $K$ si $E$ possède une base pure.

La famille vide est algébriquement libre, donc $K$ est une extension pure de lui-même. Avec les notations de la déf. 2, chaque élément $x_i$ est transcendant sur $K$; si $I$ n’est pas vide, $E$ est donc une extension transcendante de $K$.

#### Proposition 2 {#alg-v-s14-prop-2 .statement}

Soient $E$ et $E'$ deux corps et $u$ un isomorphisme d’un sous-corps $K$ de $E$ sur un sous-corps $K'$ de $E'$. Soit $x = (x_i)_{i \in I}$ (resp. $x' = (x'_i)_{i \in I}$) une famille d’éléments de $E$ (resp. $E'$) algébriquement libre sur $K$ (resp. $K'$). Il existe un isomorphisme $v$ de $L = K(x_i)_{i \in I}$ sur $L' = K'(x'_i)_{i \in I}$ et un seul qui induise $u$ sur $K$ et applique $x_i$ sur $x'_i$ pour tout $i \in I$.

L’unicité de $v$ est claire. Posons $A = K[x_i]_{i \in I}$ et $A' = K'[x'_i]_{i \in I}$. Par hypothèse, les monômes $x^\alpha = \prod_{i \in I} x_i^{\alpha_i}$ (pour $\alpha = (\alpha_i)_{i \in I}$ dans $\mathbf{N}^{(I)}$) forment une base du $K$-espace vectoriel $A$, et l’on a une propriété analogue pour $A'$. Il existe donc un isomorphisme d’anneaux $w : A \to A'$ transformant tout élément $\sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha x^\alpha$ en $\sum_{\alpha \in \mathbf{N}^{(I)}} u(c_\alpha) {x'}^\alpha$. Comme $L$ est le corps des fractions de $A$ et $L'$ celui de $A'$, l’isomorphisme $w$ se prolonge en un isomorphisme $v$ du corps $L$ sur le corps $L'$.

#### Corollaire {#alg-v-s14-n1-cor-1 .statement}

Pour qu’une extension $E$ d’un corps $K$ soit pure, il faut et il suffit que $E$ soit $K$-isomorphe à un corps de fractions rationnelles sur $K$. De manière précise, si la famille $(x_i)_{i \in I}$ est une base pure de $E$, il existe un unique $K$-isomorphisme de $K(X_i)_{i \in I}$ sur $E$ qui applique $X_i$ sur $x_i$ pour tout $i \in I$.

#### Remarque {#alg-v-s14-n1-rem-1 .statement}

Il est clair que, dans une extension $E$ de $K$, une famille algébriquement libre sur $K$ est formée d’éléments linéairement indépendants sur $K$ (donc deux à deux distincts); autrement dit, c’est une famille libre pour la structure d’espace vectoriel de $E$ (par rapport à $K$). Mais la réciproque est inexacte, car si $E$ est une extension algébrique de $K$, une famille non vide quelconque d’éléments de $E$ (et a fortiori une famille non vide d’éléments linéairement indépendants sur $K$) n’est jamais algébriquement libre sur $K$. Lorsqu’il y a risque de confusion, nous dirons qu’une partie d’une extension $E$ de $K$, qui est libre pour la structure d’espace vectoriel de $E$ par rapport à $K$ est linéairement libre sur $K$.

Soit $E$ une extension d’un corps $K$. On dit qu’une partie $S$ de $E$ est algébriquement libre (sur $K$) si la famille définie par l’application identique de $S$ sur elle-même est algébriquement libre. On dit aussi que les éléments d’une partie algébriquement libre de $E$ sont algébriquement indépendants. Si une partie de $E$ n’est pas algébriquement libre, on dit qu’elle est algébriquement liée et que ses éléments sont algébriquement dépendants. Pour qu’une famille $(x_i)_{i \in I}$ d’éléments de $E$ soit algébriquement libre, il faut et il suffit que $i \mapsto x_i$ soit une bijection de $1$ sur une partie de $E$ algébriquement libre sur $K$.

Toute partie d'une partie algébriquement libre est algébriquement libre. En outre :

#### Proposition 3 {#alg-v-s14-prop-3 .statement}

*Pour qu'une famille* $(x_i)_{i \in I}$ *d'éléments d'une extension* $E$ *d'un corps* $K$ *soit algébriquement libre sur* $K$, *il faut et il suffit que toute sous-famille finie de* $(x_i)_{i \in I}$ *soit algébriquement libre sur* $K$.

La proposition résulte immédiatement de la déf. 1.

### 2. Bases de transcendance

#### Proposition 4 {#alg-v-s14-prop-4 .statement}

*Soient* $E$ *une extension d'un corps* $K$, $S$ *et* $T$ *deux parties de* $E$. *Les propriétés suivantes sont équivalentes :*
a) $S \cup T$ *est algébriquement libre sur* $K$ *et* $S \cap T = \varnothing$.
b) $S$ *est algébriquement libre sur* $K$, *et* $T$ *est algébriquement libre sur* $K(S)$.
c) $T$ *est algébriquement libre sur* $K$, *et* $S$ *est algébriquement libre sur* $K(T)$.

Il suffit évidemment de prouver que a) et b) sont équivalentes.

$a) \Rightarrow b)$ : supposons a) vérifiée. Comme $S$ est contenue dans $S \cup T$, elle est algébriquement libre sur $K$. Si $T$ n'est pas algébriquement libre sur $K(S)$, il existe (prop. 3) une famille finie $(y_j)_{1 \leq j \leq n}$ d'éléments distincts de $T$, algébriquement liée sur $K(S)$. Par suite, il existe un polynôme non nul $f$ de l'anneau $K(S)[Y_1, ..., Y_n]$ tel que $f(y_1, ..., y_n) = 0$; quitte à multiplier $f$ par un élément non nul de $K[S]$, on peut supposer que tous les coefficients de $f$ appartiennent à $K[S]$. Les coefficients de $f$ sont des polynômes par rapport à un nombre fini d'éléments distincts $x_i$ ($1 \leq i \leq m$) de $S$, à coefficients dans $K$. Les éléments $x_1, ..., x_m, y_1, ..., y_n$ sont deux à deux distincts car $S \cap T = \varnothing$. La relation $f(y_1, ..., y_n) = 0$ s'écrit alors

$$
g(x_1, ..., x_m; y_1, ..., y_n) = 0,
$$

où $g$ est un polynôme non nul de $K[X_1, ..., X_m, Y_1, ..., Y_n]$, et une telle relation contredit l'hypothèse que $S \cup T$ est algébriquement libre.

$b) \Rightarrow a)$ : supposons b) vérifiée. Il est clair d'abord que $T \cap K(S) = \varnothing$, et *a fortiori* $S \cap T = \varnothing$. Il suffit de montrer que si $x_i$ ($1 \leq i \leq m$) sont des éléments distincts de $S$ en nombre fini, $y_j$ ($1 \leq j \leq n$) des éléments distincts de $T$ en nombre fini, l'ensemble des $x_i$ et des $y_j$ est algébriquement libre sur $K$ (prop. 3). Considérons un polynôme $f \in K[X_1, ..., X_m, Y_1, ..., Y_n]$ tel que $f(x_1, ..., x_m, y_1, ..., y_n) = 0$ et posons

$$
f = \sum_{\alpha_1, ..., \alpha_n} \varphi_\alpha Y_1^{\alpha_1} ... Y_n^{\alpha_n}
$$

avec $\varphi_\alpha \in K[X_1, ..., X_m]$ pour tout $\alpha = (\alpha_1, ..., \alpha_n) \in \mathbf{N}^n$.

Soit $g = f(x_1, ..., x_m, Y_1, ..., Y_n)$; alors $g$ est un polynôme de l'anneau $K[S][Y_1, ..., Y_n]$, et la relation $f(x_1, ..., x_m, y_1, ..., y_n) = 0$ s'écrit $g(y_1, ..., y_n) = 0$. Comme $T$ est algébriquement libre sur $K(S)$, chacun des coefficients $\varphi_\alpha(x_1, ..., x_m)$ de $g$ est nul ; puisque $S$ est algébriquement libre sur $K$, on a $\varphi_\alpha = 0$ pour tout $\alpha \in \mathbf{N}^n$, d'où $f = 0$.

#### Corollaire {#alg-v-s14-n2-cor-1 .statement}

*Soient* $E$ *une extension d'un corps* $K$ *et* $S$ *une partie de* $E$ *algébriquement libre sur K. Si $x \in E$ est transcendant sur $K(S)$, alors $S \cup \{ x \}$ est algébriquement libre sur $K$.

#### Proposition 5 {#alg-v-s14-prop-5 .statement}

*Soit E une extension d’un corps K. Pour qu’une partie S de E soit algébriquement libre sur K, il faut et il suffit que, pour tout $x \in S$, l’élément x soit transcendant sur le corps $K(S - \{ x \})$.*

La condition est nécessaire d’après la prop. 4.

Pour prouver la suffisance, il suffit (prop. 3) de montrer que toute suite finie $(x_1, ..., x_n)$ d’éléments distincts de S est algébriquement libre. Or, par hypothèse, $x_i$ est transcendant sur $K(x_1, ..., x_{i-1})$ pour $1 \leq i \leq n$, et notre assertion résulte donc par récurrence sur $n$ du cor. de la prop. 4.

#### Proposition 6 {#alg-v-s14-prop-6 .statement}

*Soient E une extension d’un corps K et X une partie de E algébriquement libre sur K. Si $K' \subset E$ est une extension algébrique de K, alors X est algébriquement libre sur $K'$.*

Raisonnons par l’absurde et supposons que X soit algébriquement liée sur $K'$. D’après la prop. 5, il existe un élément $x \in X$ algébrique sur le corps $K'(M)$, où $M = X - \{ x \}$. Comme on a $K'(M) = K(M)$ ($K'$) et que $K'$ est algébrique sur K, le cor. 2 de V, p. 18, montre que $K'(M)$ est algébrique sur $K(M)$; comme $x$ est algébrique sur $K'(M)$, il est donc algébrique sur $K(M) = K(X - \{ x \})$ d’après la prop. 3 de V, p. 18. La prop. 5 montre alors que X est algébriquement lié sur K, d’où une contradiction.

#### Définition 3 {#alg-v-s14-def-3 .statement}

*On dit qu’une partie B d’une extension E d’un corps K est une base de transcendance de E (sur K) si B est algébriquement libre sur K, et si E est algébrique sur $K(B)$.*

#### Exemple {#alg-v-s14-n2-exa-1 .statement}

Une base pure est une base de transcendance. En revanche, si E est une extension pure de K, une base de transcendance de E sur K n’est pas toujours une base pure de E. Par exemple, dans $K(X)$, $\{ X^2 \}$ est une base de transcendance mais n’engendre pas $K(X)$.

#### Proposition 7 {#alg-v-s14-prop-7 .statement}

*Soit E une extension d’un corps K. Toute base de transcendance de E est un élément maximal de l’ensemble (ordonné par inclusion) des parties de E algébriquement libres sur K. Inversement, si S est une partie de E telle que E soit algébrique sur $K(S)$, toute partie algébriquement libre maximale de S est une base de transcendance de E.*

Soient B une base de transcendance de E sur K, et $x \in E - B$. Alors $x$ est algébrique sur $K(B)$; d’après V, p. 103, prop. 4, la partie $B \cup \{ x \}$ de E n’est pas algébriquement libre sur K, d’où la première partie de la proposition. D’autre part, si E est algébrique sur $K(S)$, et B est une partie algébriquement libre maximale de S, il résulte du cor. de la prop. 4 que tout $x \in S$ est algébrique sur $K(B)$; donc (V, p. 18, cor. 1), $K(S)$ est algébrique sur $K(B)$, et par suite (V, p. 18, prop. 3), E est algébrique sur $K(B)$.

#### Théorème 1 (Steinitz) {#alg-v-s14-thm-1 .statement}

Toute extension E d’un corps K admet une base de transcendance sur K. En d’autres termes, toute extension d’un corps K est une extension algébrique d’une extension pure de K.

Par contre, une extension n’est pas toujours extension pure d’une extension algébrique (V, p. 161, exerc. 2).

Ce théorème est une conséquence du théorème plus précis suivant :

#### Théorème 2 {#alg-v-s14-thm-2 .statement}

Soient E une extension d’un corps K, S une partie de E telle que E soit algébrique sur K(S), et T une partie de S, algébriquement libre sur K ; il existe alors une base de transcendance B de E sur K telle que T ⊂ B ⊂ S.

En effet, l’ensemble des parties algébriquement libres de S, ordonné par inclusion, est un ensemble de caractère fini (E, III, p. 34) d’après la prop. 3. D’après le th. 1 de E, III, p. 35, il admet un élément maximal B contenant T, et B est une base de transcendance de E sur K, en vertu de la prop. 7.

#### Corollaire (« théorème d’échange ») {#alg-v-s14-n2-cor-2 .statement}

Soient E une extension de K, S une partie de E telle que E soit algébrique sur K(S), T une partie de E algébriquement libre sur K ; il existe une partie S’ de S telle que T ∪ S’ soit une base de transcendance de E sur K et que T ∩ S’ = ∅.

En effet, E est algébrique sur K(T ∪ S) et l’on a T ⊂ T ∪ S.

### 3. Degré de transcendance d’une extension

#### Théorème 3 {#alg-v-s14-thm-3 .statement}

Soit E une extension d’un corps K. Toutes les bases de transcendance de E sur K ont même cardinal.

Il suffit de prouver l’inégalité Card(B) ≥ Card(B’) lorsque B et B’ sont deux bases de transcendance de E sur K. On peut supposer B’ non vide. Supposons d’abord B fini et raisonnons par récurrence sur son cardinal n ; pour n = 0, E est algébrique sur K et B’ est vide. Supposons donc n ≥ 1. Étant donné x ∈ B’, le théorème d’échange fournit une partie C de B telle que x ∉ C et que {x} ∪ C soit une base de transcendance de E sur K ; on a C ≠ B d’après la prop. 7, d’où Card(C) < n. Posons K_1 = K(x) et C’ = B’ − {x} ; alors C et C’ sont algébriquement libres sur le corps K_1 (V, p. 103, prop. 4) et E est algébrique à la fois sur K_1(C) = K(C ∪ {x}) et K_1(C’) = K(B’). Autrement dit, C et C’ sont deux bases de transcendance de E sur K_1 ; comme on a Card(C) < n, l’hypothèse de récurrence entraîne l’inégalité Card(C’) ≤ Card(C) ≤ n − 1, d’où Card(B’) ≤ n = Card(B).

Supposons maintenant B infini. Tout x ∈ B est algébrique sur K(B’) et il existe donc une partie finie S(x) de B’ telle que x soit algébrique sur K(S(x)). Posons S = ⋃_{x∈B} S(x) d’où S ⊂ B’ ; comme B est infini, on a Card(S) ≤ Card(B) (E, III, p. 49, cor. 3). Mais tout élément de B étant algébrique sur K(S), et E étant algébrique sur K(B), on conclut que E est algébrique sur K(S) (V, p. 18, prop. 3). La prop. 7 entraîne alors S = B’, d’où l’inégalité cherchée Card(B’) ≤ Card(B).

#### Définition 4 {#alg-v-s14-def-4 .statement}

Soit E une extension d’un corps K. Le cardinal de toute base de transcendance de E sur K est appelé le degré de transcendance de E sur K, et noté deg. tr_K E.

Les th. 2 et 3 et la déf. 4 entraînent les corollaires suivants, où l’on désigne par E une extension d’un corps K, de degré de transcendance fini n.

#### Corollaire 1 {#alg-v-s14-def-4-cor-1 .statement}

Soit S une partie de E telle que E soit algébrique sur K(S). On a Card(S) $\geq n$; si le cardinal de S est égal à n, alors S est algébriquement libre sur K (donc est une base de transcendance de E sur K).

#### Corollaire 2 {#alg-v-s14-def-4-cor-2 .statement}

Supposons que l’on ait $E = K(x_1, ..., x_m)$. Alors, on a $m \geq n$; si de plus on a $m = n$, alors $(x_1, ..., x_m)$ est une base pure de E sur K, et E est alors une extension pure de K.

#### Corollaire 3 {#alg-v-s14-def-4-cor-3 .statement}

Toute partie de E algébriquement libre sur K a au plus n éléments, et si elle a exactement n éléments, c’est une base de transcendance de E sur K.

#### Théorème 4 {#alg-v-s14-thm-4 .statement}

Soient K, E et F trois corps tels que $K \subset E \subset F$. Si S est une base de transcendance de E sur K et T une base de transcendance de F sur E, alors $S \cap T$ est vide et $S \cup T$ est une base de transcendance de F sur K.

En effet, F est algébrique sur E(T); de plus E(T) est algébrique sur le corps $K(S \cup T) = K(S)(T)$, puisque E est algébrique sur K(S) (V, p. 18, cor. 2); par suite (V, p. 18, prop. 3), F est algébrique sur K(S \cup T). D’autre part, T étant algébriquement libre sur E, l’est a fortiori sur K(S), donc (V, p. 103, prop. 4) $S \cup T$ est algébriquement libre sur K et $S \cap T = \varnothing$.

#### Corollaire {#alg-v-s14-n3-cor-1 .statement}

Soient K, E et F trois corps tels que $K \subset E \subset F$. On a

$$
\text{deg. tr}_K F = \text{deg. tr}_K E + \text{deg. tr}_E F .
$$

### 4. Prolongement d’isomorphismes

#### Proposition 8 {#alg-v-s14-prop-8 .statement}

Soient $\Omega$ une extension algébriquement close d’un corps K, E et F deux sous-extensions de $\Omega$, et u un K-isomorphisme de E sur F. Pour qu’il existe un K-automorphisme v de $\Omega$ prolongeant u, il faut et il suffit que $\Omega$ ait même degré de transcendance sur E et F.

La condition est évidemment nécessaire.

Supposons donc que $\Omega$ ait même degré de transcendance par rapport à E et à F, et choisissons une base de transcendance B de $\Omega$ sur E et une base de transcendance C de $\Omega$ sur F. Comme B et C sont équipotentes, la prop. 2 (V, p. 102) montre que u se prolonge en un K-isomorphisme $u'$ de E(B) sur F(C). Comme $\Omega$ est une clôture algébrique de E(B) et de F(C), le cor. de V, p. 23, montre que $u'$ se prolonge en un automorphisme v de $\Omega$.

#### Corollaire 1 {#alg-v-s14-prop-8-cor-1 .statement}

Soient $\Omega$ une extension algébriquement close d’un corps $K$ et $E$ une sous-extension de $\Omega$. Tout $K$-automorphisme de $E$ se prolonge en un $K$-automorphisme de $\Omega$.

#### Corollaire 2 {#alg-v-s14-prop-8-cor-2 .statement}

Soient $\Omega$ une extension algébriquement close d’un corps $K$, $E$ et $F$ deux sous-extensions de $\Omega$ et $u$ un $K$-isomorphisme de $E$ sur $F$. Si le degré de transcendance de $E$ sur $K$ est fini (en particulier, si $E$ est algébrique sur $K$), il existe un $K$-automorphisme de $\Omega$ prolongeant $u$.

Notons respectivement $n$, $d(E)$ et $d(F)$ le degré de transcendance de $E$ sur $K$, de $\Omega$ sur $E$ et de $\Omega$ sur $F$. L’existence du $K$-isomorphisme $u$ montre que le degré de transcendance de $F$ sur $K$ est égal à $n$. D’après le cor. du th. 4, le degré de transcendance de $\Omega$ sur $K$ est égal à $d(E) + n$ et aussi à $d(F) + n$. Par suite (E, III, p. 28, prop. 8), on a $d(E) = d(F)$, et l’on peut appliquer la prop. 8.

#### Proposition 9 {#alg-v-s14-prop-9 .statement}

Soient $K$ un corps et $\Omega$ une extension algébriquement close de $K$. On suppose que $\Omega$ n’est pas algébrique sur $K$. Alors, l’ensemble des éléments de $\Omega$ transcendants sur $K$ est infini. De plus, si $x$ et $y$ sont deux éléments de $\Omega$ transcendants sur $K$, il existe un automorphisme $u$ de $\Omega$ sur $K$ tel que $u(x) = y$.

Comme $\Omega$ n’est pas algébrique sur $K$, il existe un élément $x$ de $\Omega$ transcendant sur $K$; alors les éléments $x^n$ (pour $n \in \mathbf{N}$) sont distincts et transcendants sur $K$. Supposons que $x$ et $y$ soient transcendants sur $K$; d’après la prop. 2 (V, p. 102), il existe un $K$-isomorphisme $\tilde{u}$ de $K(x)$ sur $K(y)$ tel que $\tilde{u}(x) = y$; comme $K(x)$ est de degré de transcendance 1 sur $K$, le cor. 2 de la prop. 8 montre que $\tilde{u}$ se prolonge en un $K$-automorphisme $u$ de $\Omega$.

#### Proposition 10 {#alg-v-s14-prop-10 .statement}

Soient $K$ un corps, $\Omega$ une extension algébriquement close de $K$ et $G$ le groupe des $K$-automorphismes de $\Omega$. Soit $x \in \Omega$.

a) Pour que $x$ soit algébrique sur $K$, il faut et il suffit que l’ensemble des éléments $u(x)$ pour $u$ parcourant $G$ soit fini.

b) Pour que $x$ soit radiciel sur $K$, il faut et il suffit que l’on ait $u(x) = x$ pour tout $u \in G$.

En particulier, si $K$ est parfait, l’ensemble des invariants du groupe $G$ est égal à $K$.

Supposons d’abord que $x$ soit transcendant. D’après la prop. 9, l’ensemble $T$ des éléments de $\Omega$ transcendants sur $K$ est infini, et pour tout $y \in T$, il existe $u \in G$ avec $u(x) = y$. Donc l’ensemble des éléments $u(x)$ pour $u$ parcourant $G$ est infini.

Supposons maintenant que $x$ soit algébrique sur $K$, et notons $f$ son polynôme minimal sur $K$; l’ensemble des racines de $f$ dans $\Omega$ est fini, et pour tout $u \in G$, on a $f(u(x)) = u(f(x)) = 0$. Donc l’ensemble des éléments $u(x)$ pour $u$ parcourant $G$ est fini. Ceci prouve a).

Soit $L$ l’ensemble des éléments $y$ de $\Omega$ tels que $u(y) = y$ pour tout $u \in G$, et soit $\overline{K}$ la fermeture algébrique de $K$ dans $\Omega$. D’après ce qui précède, $L$ est une sous-extension de $\overline{K}$ sur $K$. De plus (cor. 1 de la prop. 8), tout $K$-automorphisme de $\overline{K}$ est la restriction à $\overline{K}$ d’un élément de $G$. L’assertion b) de la prop. 10 résulte alors du cor. 3 de V, p. 51.

### 5. Extensions algébriquement disjointes

#### Définition 5 {#alg-v-s14-def-5 .statement}

Soient L une extension d’un corps K, E et F deux sous-extensions de L. On dit que E et F sont algébriquement disjointes (sur K) ou que E est algébriquement disjointe de F sur K si, pour toute partie A (resp. B) de E (resp. F) algébriquement libre sur K, A et B sont disjointes et $A \cup B$ est algébriquement libre sur K.

#### Remarque 1 {#alg-v-s14-n5-rem-1 .statement}

Si E est une sous-extension de L algébrique sur K, elle est algébriquement disjointe de toute sous-extension F de L. Pour qu’une extension de K soit algébrique, il faut et il suffit qu’elle soit algébriquement disjointe d’elle-même.

#### Remarque 2 {#alg-v-s14-n5-rem-2 .statement}

Il se peut que E soit algébriquement disjointe de F sur K, mais non sur un sous-corps $K_0$ de K. \* Par exemple, C est algébriquement disjointe d’elle-même sur R mais non sur Q. \*

#### Remarque 3 {#alg-v-s14-n5-rem-3 .statement}

Il est clair que si E est algébriquement disjointe de F sur K, quand on considère E et F comme des sous-extensions de L, il en est de même si on les considère comme des sous-extensions de $K(E \cup F)$, et réciproquement.

#### Proposition 11 {#alg-v-s14-prop-11 .statement}

Si E et F sont algébriquement disjointes sur K, alors $E \cap F$ est algébrique sur K.
Cela résulte de la déf. 5.

#### Proposition 12 {#alg-v-s14-prop-12 .statement}

Soient L une extension d’un corps K, E et F des sous-extensions de L. Les conditions suivantes sont équivalentes :
a) E et F sont algébriquement disjointes ;
b) il existe une base de transcendance de E sur K qui est algébriquement libre sur F ;
c) toute partie de E algébriquement libre sur K est algébriquement libre sur F.
Introduisons les conditions suivantes :
b’) il existe une base de transcendance de F sur K qui est algébriquement libre sur E ;
c’) toute partie de F algébriquement libre sur K est algébriquement libre sur E.
a) $\Rightarrow b’$ : Supposons E et F algébriquement disjointes. Soit B (resp. C) une base de transcendance de E (resp. F) sur K. Alors $B \cap C = \varnothing$ et $B \cup C$ est algébriquement libre sur K, donc C est algébriquement libre sur $K(B)$ (V, p. 103, prop. 4) ; comme E est algébrique sur $K(B)$, la prop. 6 de V, p. 104, montre que C est algébriquement libre sur E.
b’) $\Rightarrow c$ : Supposons qu’il existe une base de transcendance C de F sur K qui soit algébriquement libre sur E. Soit A une partie de E algébriquement libre sur K. Alors C est algébriquement libre sur $K(A)$, donc A est algébriquement libre sur $K(C)$ (V, p. 103, prop. 4) et par suite sur F (V, p. 104, prop. 6) puisque F est algébrique sur $K(C)$.
c’) $\Rightarrow a$ : cela résulte aussitôt de la prop. 4 (V, p. 103).
On démontre de même les implications $a) \Rightarrow b) \Rightarrow c’) \Rightarrow a)$.

#### Corollaire {#alg-v-s14-n5-cor-1 .statement}

Supposons que E et F soient algébriquement disjointes sur K. Soient E' la fermeture algébrique de E dans L et F' celle de F (V, p. 19). Alors E' et F' sont algébriquement disjointes sur K.

Soit B une base de transcendance de E sur K ; c'est aussi une base de transcendance de E' sur K. Comme E est algébriquement disjointe de F sur K, B est algébriquement libre sur F, donc sur F' (V, p. 104, prop. 6) ; on applique alors la prop. 12.

#### Proposition 13 {#alg-v-s14-prop-13 .statement}

Soient L une extension d'un corps K, et E, F deux sous-extensions de L.

a) On a deg. tr_F F(E) ≤ deg. tr_K E. Lorsque E et F sont algébriquement disjointes sur K, toute base de transcendance de E sur K est une base de transcendance de F(E) sur F, et l'on a deg. tr_F F(E) = deg. tr_K E. Réciproquement, cette égalité entraîne que E et F sont algébriquement disjointes sur K lorsque deg. tr_K E est fini.

b) On a deg. tr_K K(E ∪ F) ≤ deg. tr_K E + deg. tr_K F. Lorsque E et F sont algébriquement disjointes sur K, on a deg. tr_K K(E ∪ F) = deg. tr_K E + deg. tr_K F. Réciproquement, cette égalité entraîne que E et F sont algébriquement disjointes sur K lorsque E et F sont de degrés de transcendance finis sur K.

a) Soit B une base de transcendance de E sur K ; alors E est algébrique sur K(B), et le cor. 2 de V, p. 18, montre que F(E) est algébrique sur F(K(B)) = F(B). D'après le th. 2 (V, p. 105), B contient une base de transcendance de F(E) sur F ; lorsque E est algébriquement disjointe de F sur K, B est algébriquement libre sur F (prop. 12) et c'est donc une base de transcendance de F(E) sur F. Les trois premières assertions de a) résultent de là. Supposons maintenant E de degré de transcendance fini sur K, égal à celui de F(E) sur F ; comme F(E) est algébrique sur F(B) et que Card B = deg. tr_F F(E), le cor. 1 de V, p. 106, montre que B est algébriquement libre sur F et E est donc algébriquement disjointe de F sur K (prop. 12).

b) On a K(E ∪ F) = F(E) et le cor. de V, p. 106, entraîne donc l'égalité :

$$
\operatorname{deg.} \operatorname{tr}_K K(E \cup F) = \operatorname{deg.} \operatorname{tr}_F F(E) + \operatorname{deg.} \operatorname{tr}_K F .
$$

L'assertion b) résulte immédiatement de a) et de cette égalité.

#### Proposition 14 {#alg-v-s14-prop-14 .statement}

Soient L une extension d'un corps K, E et F deux sous-extensions de L et B une base de transcendance de E sur K. Pour que E et F soient algébriquement disjointes sur K, il faut et il suffit que les extensions K(B) et F soient linéairement disjointes sur K.

Pour que E et F soient algébriquement disjointes sur K, il faut et il suffit que B soit une partie algébriquement libre sur F (prop. 12), c'est-à-dire que les monômes par rapport aux éléments de B soient linéairement indépendants sur F. Comme ces monômes forment une base du K-espace vectoriel K[B], il revient au même de dire que K[B] et F sont linéairement disjointes sur K. Enfin, comme K(B) est le corps des fractions de K[B], la prop. 6 de V, p. 14, montre que K[B] et F sont linéairement disjointes si et seulement s'il en est ainsi de K(B) et F.

#### Corollaire 1 {#alg-v-s14-prop-14-cor-1 .statement}

Si E et F sont linéairement disjointes, alors E est algébriquement disjointe de F sur K. Réciproquement, si E est une extension pure de K et si elle est algébriquement disjointe de F sur K, alors E et F sont linéairement disjointes sur K.

#### Corollaire 2 {#alg-v-s14-prop-14-cor-2 .statement}

Toute extension pure de K est linéairement disjointe de toute extension algébrique de K ; en particulier, K est algébriquement fermé dans toute extension pure de K.

### 6. Familles algébriquement libres d’extensions

#### Définition 6 {#alg-v-s14-def-6 .statement}

Soient L une extension d’un corps K, et $(E_i)_{i \in I}$ une famille de sous-extensions de L. On dit que la famille $(E_i)_{i \in I}$ est algébriquement libre si la condition suivante est vérifiée :

(AL) Soit pour tout $i \in I$ une partie $A_i$ de $E_i$ algébriquement libre sur K. On a alors $A_i \cap A_j = \varnothing$ pour $i \neq j$, et $\bigcup_{i \in I} A_i$ est algébriquement libre sur K.

#### Remarque {#alg-v-s14-n6-rem-1 .statement}

D’après la prop. 3 (V, p. 103), il suffit de vérifier la condition (AL) pour des parties $A_i$ finies. On en déduit le résultat suivant : si $(E_i)_{i \in I}$ est une famille algébriquement libre, il en est de même de $(E'_i)_{i \in I}$ si $E'_i$ est une sous-extension de $E_i$ pour tout $i \in I$; réciproquement, si toute famille $(E'_i)_{i \in I}$, où $E'_i$ est une sous-extension de type fini de $E_i$ pour tout $i \in I$, est algébriquement libre, alors $(E_i)_{i \in I}$ est algébriquement libre. D’autre part, pour que $(E_i)_{i \in I}$ soit algébriquement libre, il faut et il suffit que, pour toute partie finie J de I, $(E_i)_{i \in J}$ soit algébriquement libre. D’une manière imagée, on peut dire que l’indépendance algébrique des extensions est une propriété « de caractère fini ».

#### Proposition 15 {#alg-v-s14-prop-15 .statement}

Soit $(E_i)_{i \in I}$ une famille de sous-extensions d’une même extension L d’un corps K. Les conditions suivantes sont équivalentes :
a) La famille $(E_i)_{i \in I}$ est algébriquement libre.
b) Pour tout $i \in I$, l’extension $E_i$ est algébriquement disjointe sur K de l’extension $F_i$ engendrée par les $E_j$ pour $j \neq i$.
c) Il existe une famille $(B_i)_{i \in I}$ de parties disjointes de L, telle que $B_i$ soit une base de transcendance de $E_i$ sur K pour tout $i \in I$, et que $B = \bigcup_{i \in I} B_i$ soit algébriquement libre sur K.

Il est clair que a) entraîne c).
Plaçons-nous dans les hypothèses de c) et choisissons i dans I ; posons $C_i = \bigcup_{j \neq i} B_j$.
Pour tout $j \neq i$, tout élément de $E_j$ est algébrique sur $K(B_j)$ et a fortiori sur $K(C_i)$. D’après le cor. 1 de V, p. 18, le corps $F_i$ est donc algébrique sur $K(C_i)$. Par ailleurs, on a $B_i \cap C_i = \varnothing$ et $B = B_i \cup C_i$ est algébriquement libre sur K ; par suite, $B_i$ est algébriquement libre sur $K(C_i)$ (V, p. 103, prop. 4), donc aussi sur $F_i$ (qui est algébrique sur $K(C_i)$) d’après la prop. 6 de V, p. 104. On a prouvé que $E_i$ est algébriquement disjointe de $F_i$ sur K (V, p. 108, prop. 12), donc c) entraîne b).

Plaçons-nous dans les hypothèses de b) et prouvons a). Il suffit de montrer que si $i_1, \ldots, i_n$ sont des éléments distincts de $I$, la famille d’extensions $(E_{i_1}, \ldots, E_{i_n})$ est algébriquement libre ; nous raisonnons par récurrence sur $n$, le cas $n = 1$ étant trivial. Supposons donc $n > 1$ et que la famille $(E_{i_1}, \ldots, E_{i_{n-1}})$ soit algébriquement libre ; pour $1 \leq k \leq n$, choisissons une partie $A_k$ de $E_{i_k}$ algébriquement libre sur $K$, et posons $B = A_1 \cup \ldots \cup A_{n-1}$. Par l’hypothèse de récurrence, les parties $A_1, \ldots, A_{n-1}$ sont deux à deux disjointes et $B$ est algébriquement libre sur $K$ ; d’après l’hypothèse b), $E_{i_n}$ est algébriquement disjointe de $F_{i_n}$, et comme $B$ est contenue dans $F_{i_n}$, on a $B \cap A_n = \varnothing$ et $B \cup A_n = A_1 \cup \ldots \cup A_n$ est algébriquement libre sur $K$. On a donc prouvé que la famille $(E_{i_1}, \ldots, E_{i_n})$ est algébriquement libre.

La proposition suivante généralise la partie b) de la prop. 13 (V, p. 109).

#### Proposition 16 {#alg-v-s14-prop-16 .statement}

*Soit $(E_i)_{i \in I}$ une famille de sous-extensions d’une extension d’un corps $K$. Soit $E$ le corps engendré par $\bigcup_{i \in I} E_i$.*

a) *On a $\deg.\operatorname{tr}_K E \leq \sum_{i \in I} \deg.\operatorname{tr}_K E_i$, et il y a égalité si la famille $(E_i)_{i \in I}$ est algébriquement libre sur $K$.*

b) *Réciproquement, supposons que l’on ait $\deg.\operatorname{tr}_K E = \sum_{i \in I} \deg.\operatorname{tr}_K E_i$ et que $\deg.\operatorname{tr}_K E$ soit fini. Alors la famille $(E_i)_{i \in I}$ est algébriquement libre sur $K$.*

Pour tout $i \in I$, soit $B_i$ une base de transcendance de $E_i$ sur $K$ ; on pose $B = \bigcup_{i \in I} B_i$.

Pour tout $i \in I$, tout élément de $E_i$ est algébrique sur $K(B_i)$, donc sur $K(B)$ ; le cor. 1 de V, p. 18, montre alors que $E$ est algébrique sur $K(B)$ ; d’après V, p. 105, th. 2, $B$ contient donc une base de transcendance de $E$ sur $K$ ; si de plus, la famille $(E_i)_{i \in I}$ est algébriquement libre sur $K$, alors les $B_i$ sont disjoints et l’ensemble $B$ est algébriquement libre sur $K$. Cela établit a) (E, III, p. 26, cor. de la prop. 4).

Sous les hypothèses de b), $E$ est algébrique sur $K(B)$ et de degré de transcendance fini sur $K$, et l’on a $\operatorname{Card}(B) \leq \deg.\operatorname{tr}_K E$. D’après le cor. 1 de V, p. 106, $B$ est algébriquement libre sur $K$ et les $B_i$ sont disjoints. La prop. 15 montre alors que la famille $(E_i)_{i \in I}$ est algébriquement libre sur $K$.

Avant d’énoncer le théorème suivant, remarquons qu’il existe des extensions algébriquement closes de $K$ de degré de transcendance arbitraire, par exemple une clôture algébrique d’un corps de fractions rationnelles convenable.

#### Théorème 5 {#alg-v-s14-thm-5 .statement}

*Soient $(E_i)_{i \in I}$ une famille d’extensions d’un corps $K$ et $\Omega$ une extension algébriquement close de $K$. On suppose vérifiée l’inégalité*

$$
\deg.\operatorname{tr}_K \Omega \geq \sum_{i \in I} \deg.\operatorname{tr}_K E_i .
$$

*Il existe alors une famille $(F_i)_{i \in I}$ algébriquement libre de sous-extensions de $\Omega$ telle que $F_i$ soit $K$-isomorphe à $E_i$ pour tout $i \in I$.*

Pour tout $i \in I$, soit $B_i$ une base de transcendance de $E_i$ sur $K$. Soit $B$ une base de transcendance de $\Omega$ sur $K$. D’après (2), on a $\operatorname{Card} B \geq \sum_{i \in I} \operatorname{Card} B_i$ ; il existe donc une famille $(B'_i)_{i\in I}$ de parties de $B$, deux à deux disjointes, et des bijections $u_i : B_i \to B'_i$ (pour $i \in I$). D’après la prop. 2 de V, p. 102, $u_i$ se prolonge en un $K$-isomorphisme $v_i$ de $K(B_i)$ sur $K(B'_i)$; comme $\Omega$ est algébriquement close et $E_i$ algébrique sur $K(B_i)$, le cor. (V, p. 23) montre que $v_i$ se prolonge en un $K$-isomorphisme de $E_i$ sur une sous-extension $F_i$ de $\Omega$. Par construction, $B'_i$ est une base de transcendance de $F_i$ sur $K$, et la prop. 15 (V, p. 110) montre que la famille $(F_i)_{i\in I}$ de sous-extensions de $\Omega$ est algébriquement libre sur $K$.

#### Corollaire 1 {#alg-v-s14-thm-5-cor-1 .statement}

*Soient $E$ et $\Omega$ deux extensions d’un corps $K$. On suppose que $\Omega$ est algébriquement close, de degré de transcendance au moins égal à celui de $E$. Alors $E$ est $K$-isomorphe à une sous-extension de $\Omega$*.

#### Corollaire 2 {#alg-v-s14-thm-5-cor-2 .statement}

*Soit $\Omega$ un corps algébriquement clos de degré de transcendance infini sur son sous-corps premier. Tout corps de même caractéristique que $\Omega$ est réunion filtrante croissante de corps isomorphes à des sous-corps de $\Omega$.
En effet, tout corps est réunion filtrante croissante de ses sous-corps de type fini sur le corps premier, et il suffit d’appliquer le cor. 1.

*Exemple. — Cela s’applique notamment en caractéristique 0 en prenant $\Omega = \mathbf{C}$ (« principe de Lefschetz »). \*

### 7. Extensions de type fini

#### Proposition 17 {#alg-v-s14-prop-17 .statement}

*Soient $E$ une extension d’un corps $K$ et $B$ une base de transcendance de $E$ sur $K$. Pour que $E$ soit de type fini (V, p. 11, déf. 2) sur $K$, il faut et il suffit que $B$ soit finie et que le degré $[E : K(B)]$ soit fini.*
Supposons $E$ de type fini sur $K$ et soit $S$ une partie finie de $E$ telle que $E = K(S)$. D’après le th. 2 (V, p. 105), $S$ contient une base de transcendance $B'$ de $E$ sur $K$, et celle-ci a même cardinal que $B$ (V, p. 105, th. 3). Par suite, $B$ est finie. Posons $K' = K(B)$; alors $E$ est algébrique sur $K'$ et l’on a $E = K'(S)$; comme $S$ est finie, le th. 2 de V, p. 17, montre que $[E : K']$ est fini.
Réciproquement, supposons $B$ finie et $[E : K(B)]$ fini. Si $C$ est une base (finie) de l’espace vectoriel $E$ sur le corps $K(B)$, on a $E = K(B)(C) = K(B \cup C)$ et $E$ est une extension de type fini de $K$.

#### Corollaire 1 {#alg-v-s14-prop-17-cor-1 .statement}

*Supposons que $E$ soit une extension de type fini de $K$, et notons $K'$ la fermeture algébrique de $K$ dans $E$ (V, p. 19). Alors $K'$ est de degré fini sur $K$.
Soit $B$ une base de transcendance de $E$ sur $K$. D’après le cor. 2 de V, p. 110, $K'$ est linéairement disjointe de $K(B)$ sur $K$, d’où $[K' : K] = [K'(B) : K(B)] \leq [E : K(B)]$, et la finitude de $[K' : K]$ résulte de celle de $[E : K(B)]$.*

#### Corollaire 2 {#alg-v-s14-prop-17-cor-2 .statement}

Un corps de type fini sur son sous-corps premier ne contient qu’un nombre fini de racines de l’unité.

D’après le cor. 1, on est ramené à démontrer qu’un corps L qui est une extension de degré fini de son sous-corps premier ne possède qu’un nombre fini de racines de l’unité. C’est clair si L est de caractéristique $\neq 0$, puisqu’il est alors fini. Si L est de caractéristique 0, et contient une infinité de racines de l’unité, il contient des racines primitives de l’unité d’ordre arbitrairement grand ; d’après V, p. 80, th. 2, il existe donc une infinité d’entiers $n > 0$ tels que $\varphi(n) \leq [L : Q]$, ce qui est absurde (V, p. 77, formules (2) et (3)).

#### Corollaire 3 {#alg-v-s14-prop-17-cor-3 .statement}

Si E est une extension de type fini d’un corps K, toute sous-extension E’ de E est de type fini.

Soit B’ une base de transcendance de E’ sur K. D’après V, p. 105, th. 2, B’ est contenue dans une base de transcendance B de E sur K, donc est finie par la prop. 17. Comme E’ est algébrique sur K(B’) et que E est une extension de type fini de K(B’), le cor. 1 montre que $[E' : K(B')]$ est fini. La prop. 17 montre alors que E’ est de type fini sur K.

On peut paraphraser la prop. 17 en disant qu’une extension de type fini de K est une extension algébrique de degré fini d’une extension transcendante pure $K(x_1, ..., x_n)$.

## EXERCICES {#alg-v-s14-exercises}

See the [exercises for § 14](exercises/s14/).
