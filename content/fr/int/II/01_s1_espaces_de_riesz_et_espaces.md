---
book: int
book_title: Integration
chapter: II
chapter_title: Espaces de Riesz
section: 1
section_title: Espaces de Riesz et espaces complètement réticulés
lang: fr
source: int-i-iv-fr
pdf_pages: 0021-0029, 0036-0041
extraction: ocr
subsections:
    - "no": 1
      title: Définition des espaces de Riesz
      page: 0
      pdf_page: 21
    - "no": 2
      title: Génération d’un espace de Riesz par ses éléments positifs
      page: 0
      pdf_page: 24
    - "no": 3
      title: Espaces complètement réticulés
      page: 0
      pdf_page: 24
    - "no": 4
      title: Sous-espaces et espaces produits d’espaces complètement réticulés
      page: 0
      pdf_page: 26
    - "no": 5
      title: Bandes dans un espace complètement réticulé
      page: 0
      pdf_page: 27
statements: 16
exercises: 14
content_sha256: 65e80833bfdc362cbc20f4d473358f8b4560e8aade59dd55bc339cb34363a94c
---

## § 1. Espaces de Riesz et espaces complètement réticulés

### 1. Définition des espaces de Riesz

Rappelons que, sur un ensemble E, une structure d’espace vectoriel sur le corps $\mathbf{R}$ et une structure d’ordre sont dites compatibles si elles satisfont aux deux axiomes suivants:
(EO₁) La relation $x \leq y$ entraîne $x + z \leq y + z$ quel que soit $z \in E$.
(EO₂) La relation $x \geq 0$ entraîne $\lambda x \geq 0$ pour tout scalaire $\lambda > 0$.

L’espace E, muni de ces deux structures, est appelé espace vectoriel ordonné (*Esp. vect. top.*, chap. II, 2e éd., § 2, n° 5).

L’axiome (EO₁) signifie que la structure d’ordre et la structure de groupe additif sur E sont compatibles, autrement dit que E, muni de ces deux structures, est un groupe ordonné (*Alg.*, chap. VI, § 1, n° 1).

L’axiome (EO₁) entraîne que les relations $x \leq y$ et $x + z \leq y + z$ sont équivalentes. De même, il résulte de (EO₂) que, pour tout scalaire $\lambda > 0$, les relations $x \leq y$ et $\lambda x \leq \lambda y$ sont équivalentes, car on a $\lambda^{-1} > 0$ et par suite la relation $\lambda x \leq \lambda y$ entraîne $\lambda^{-1}(\lambda x) \leq \lambda^{-1}(\lambda y)$. On peut donc dire que, dans un espace vectoriel ordonné, les translations et les homothéties de rapport $> 0$ sont des automorphismes de la structure d’ordre ; on exprime encore ce fait en disant que l’ordre est *invariant* par toute translation et toute homothétie de rapport $> 0$. En outre, la symétrie $x \mapsto -x$ est un isomorphisme de la structure d’ordre de E sur la structure d’ordre *opposée*.

#### Définition 1 {#int-ii-s1-def-1 .statement}

*On dit qu’un espace vectoriel ordonné est un espace de Riesz si la structure d’ordre est une structure d’ensemble réticulé* (c’est-à-dire si deux éléments quelconques $x, y$ de E admettent une borne supérieure sup $(x, y)$ et une borne inférieure inf $(x, y)$).

#### Exemple {#int-ii-s1-n1-exa-1 .statement}

L’espace $\mathbf{R}^A$ de toutes les fonctions numériques (finies) définies dans un ensemble quelconque $A$ est un espace de Riesz (pour la relation d’ordre « quel que soit $t \in A, x(t) \leq y(t) »$); en effet, deux fonctions numériques quelconques $x, y$ définies dans $A$ admettent une borne supérieure (resp. inférieure) égale à l’application $t \mapsto \sup(x(t), y(t))$ (resp. à l’application $t \mapsto \inf(x(t), y(t))$).

On peut encore dire qu’un espace de Riesz est un espace vectoriel $E$ muni d’une structure d’ordre telle que, d’une part, cette structure et la structure de groupe additif de $E$ définissent sur $E$ une structure de *groupe réticulé* (*Alg.*, chap. VI, § 1, n° 9), et que d’autre part l’axiome (EO$_{\text{II}}$) soit vérifié.

Toutes les propriétés des groupes réticulés sont donc applicables aux espaces de Riesz; nous allons rappeler les principales (cf. *Alg.*, chap. VI, § 1, n°s 9 à 12) en indiquant aussi les conséquences qui découlent de l’axiome (EO$_{\text{II}}$).

Rappelons d’abord qu’on pose $x^+ = \sup(x, 0)$ (*partie positive* de $x$), $x^- = (-x)^+ = \sup(-x, 0)$ (*partie négative* de $x$), $|x| = \sup(x, -x)$ (*valeur absolue* de $x$); on a $x = x^+ - x^-$ et $|x| = x^+ + x^-$; ces deux relations équivalent ici à
$$
x^+ = \frac{1}{2}(|x| + x), \quad x^- = \frac{1}{2}(|x| - x).
$$
La relation $x \leq y$ équivaut à « $x^+ \leq y^+$ et $x^- \geq y^-$ ». Quels que soient $x$ et $y$, on a l’inégalité *du triangle*
$$(1)$$
$$
|x + y| \leq |x| + |y|.
$$

En raison de l’invariance de l’ordre par toute homothétie de rapport $> 0$, on a
$$(2)$$
$$
\sup(\lambda x, \lambda y) = \lambda \sup(x, y) \quad \text{pour tout } \lambda \geq 0.
$$
En particulier
$$(3)$$
$$
(\lambda x)^+ = \lambda x^+, \quad (\lambda x)^- = \lambda x^- \quad \text{pour tout } \lambda \geq 0.
$$
Au contraire, pour $\lambda < 0$, on a $(\lambda x)^+ = (-\lambda x)^- = |\lambda| x^-$ et $(\lambda x)^- = (-\lambda x)^+ = |\lambda| x^+$; on en conclut que, pour tout $\lambda \in \mathbf{R}$ et tout $x \in E$, on a
$$(4)$$
$$
|\lambda x| = |\lambda| \cdot |x|.
$$
L’invariance de l’ordre par translation montre que pour tout $z \in E$ (5) $\sup(x + z, y + z) = z + \sup(x, y)$
d’où en particulier
(6) $\sup(x, y) = x + (y - x)^+ = \frac{1}{2}(x + y + |x - y|)$.

On a les relations
(7) $\inf(x, y) = -\sup(-x, -y)$
(8) $\sup(x, y) + \inf(x, y) = x + y.$

Si $x, y, z$ sont $\geqslant 0$, on a (Alg., chap. VI, 2e éd., § 1, n° 12, prop. 11)
(9) $\inf(x + y, z) \leqslant \inf(x, z) + \inf(y, z).$

Si A et B sont deux parties de E ayant chacune une borne supérieure, A + B admet également une borne supérieure, et on a
(10) $\sup(A + B) = \sup A + \sup B.$

Deux éléments $x, y$ de E sont dits étrangers si $\inf(|x|, |y|) = 0$; d’après (8), cette relation équivaut à $\sup(|x|, |y|) = |x| + |y|$, et aussi, d’après (6), à $||x| - |y|| = |x| + |y|$; 0 est le seul élément étranger à lui-même; pour tout $x \in E$, $x^+$ et $x^-$ sont étrangers et peuvent être caractérisés comme les seuls éléments étrangers $y \geqslant 0, z \geqslant 0$ tels que $x = y - z$. Si $y$ est étranger à $x$, tout $z \in E$ tel que $|z| \leqslant |y|$ est étranger à $x$. Si $y$ et $z$ sont étrangers à $x$, il en est de même de $|y| + |z|$, en vertu de l’inégalité (9); en particulier, $n|y|$ est étranger à $x$ pour tout entier $n > 0$, d’où on déduit que $\lambda y$ est étranger à $x$ pour tout scalaire $\lambda$, puisqu’il existe un entier $n$ tel que $|\lambda| \leqslant n$, d’où $|\lambda y| \leqslant n|y|$. Si une partie A de E est formée d’éléments étrangers à $x$, et si A admet une borne supérieure, cette borne supérieure est encore étrangère à $x$ (Alg., chap. VI, § 1, n° 12, cor. de la prop. 13).

Enfin, on a le lemme de décomposition (Alg., chap. VI, § 1, n° 10, th. 1):
Si $(x_i)_{i \in I}, (y_j)_{j \in J}$ sont deux suites finies d’éléments $\geqslant 0$ de E, telles que $\sum_{i \in I} x_i = \sum_{j \in J} y_j$, il existe une suite finie $(z_{ij})_{(i,j) \in I \times J}$ d’éléments $\geqslant 0$ de E telle que $x_i = \sum_{j \in J} z_{ij}$ pour tout $i \in I$ et $y_j = \sum_{i \in I} z_{ij}$ pour tout $j \in J$.

### 2. Génération d’un espace de Riesz par ses éléments positifs

Soit E un espace vectoriel ordonné; l’ensemble P des éléments $\geqslant 0$ de E est un cône convexe de sommet 0, c’est-à-dire (Esp. vect. top., chap. II, 2e éd., § 2, n° 4) un ensemble tel que $P + P \subset P$ et $\lambda P \subset P$ pour tout $\lambda > 0$. Inversement, si, dans un espace vectoriel E sur $\mathbf{R}$, P est un cône convexe de sommet 0, tel que $P \cap (-P) = \{0\}$ (autrement dit, un cône convexe pointé et saillant), on sait (loc. cit.) que la relation $y - x \in P$ est une relation d’ordre (qu’on note $x \leqslant y$) compatible avec la structure d’espace vectoriel de E. Pour que la structure d’ordre ainsi définie sur E définisse une structure d’espace de Riesz, il faut et il suffit que:

1° P engendre E, c’est-à-dire que tout $z \in E$ soit de la forme $y - x$, où $x$ et $y$ appartiennent à P;
2° P vérifie l’une des deux conditions suivantes:
a) deux éléments quelconques de P admettent dans P une borne supérieure;
b) deux éléments quelconques de P admettent dans P une borne inférieure (Alg., chap. VI, § 1, n° 8, prop. 8).

### 3. Espaces complètement réticulés

#### Définition 2 {#int-ii-s1-def-2 .statement}

On dit qu’un espace de Riesz E est complètement réticulé si toute partie majorée non vide de E admet une borne supérieure dans E.

Il est immédiat que toute partie minorée non vide d’un espace complètement réticulé E admet une borne inférieure dans E.

#### Exemple 1 {#int-ii-s1-n3-exa-1 .statement}

Si A est un ensemble quelconque, l’espace $\mathbf{R}^A$ des fonctions numériques définies dans A est complètement réticulé, la borne supérieure dans $\mathbf{R}^A$ d’une famille majorée étant son enveloppe supérieure (Top. gén., chap. IV, § 5, n° 5).
2) Soit F un ensemble quelconque; l’espace $\mathcal{B}(F)$ des fonctions numériques bornées dans F, muni de la structure d’ordre induite par celle de $\mathbf{R}^F$, est complètement réticulé. Par contre, si F est un espace topologique, l’espace $\mathcal{C}(F)$ des fonctions numériques continues dans F (muni de la structure d’ordre induite par celle de $\mathbf{R}^F$) est un espace de Riesz qui en général n’est pas complètement réticulé (cf. exerc. 13). Considérons par exemple le cas où $F = \mathbf{R}$; soient I l’intervalle ]0, 1[, $\varphi_I$ la fonction caractéristique de I, et soit H l’ensemble des fonctions continues $x(t)$ telles que $x \leqslant \varphi_I$; il est clair que H est majoré dans $\mathcal{C}(F)$. La fonction $\varphi_I$ est l’enveloppe supérieure des $x \in H$, mais non leur borne supérieure dans $C(F)$, puisque $\varphi_1$ est semi-continue inférieurement et non continue. Montrons qu’en fait $H$ n’a pas de borne supérieure dans $C(F)$; il suffit de prouver que, si $u$ est une fonction continue telle que $u \geq \varphi_1$, il existe une fonction continue $v \neq u$ telle que $u \geq v \geq \varphi_1$. Or, on a $u(0) \geq 1$, donc il existe un nombre $\alpha > 0$ tel que $u(t) > 0$ pour $-\alpha \leq t \leq 0$; si $w$ est une fonction continue nulle hors de l’intervalle $]-\alpha, 0[$, et telle que $0 < w(t) < u(t)$ dans cet intervalle, la fonction $v = u - w$ répond à la question.

#### Proposition 1 {#int-ii-s1-prop-1 .statement}

*Pour qu’un espace vectoriel ordonné E soit complètement réticulé, il faut et il suffit que E soit un espace de Riesz, et vérifie l’une des deux conditions suivantes*:

a) tout ensemble non vide $A$, formé d’éléments $\geq 0$ de $E$, majoré et filtrant pour la relation $\leq$, admet une borne supérieure dans $E$;

b) tout ensemble non vide $A$, formé d’éléments $\geq 0$ de $E$ et filtrant pour la relation $\geq$, admet une borne inférieure dans $E$.

Les conditions sont évidemment nécessaires. Inversement, supposons que $E$ soit un espace de Riesz satisfaisant à la condition *a)*. Soit $B$ une partie majorée non vide de $E$; l’ensemble $C$ des bornes supérieures des parties finies de $E$ est filtrant pour la relation $\leq$; soit $a$ un de ses éléments, et $C_a$ l’ensemble des $x \in C$ qui sont $\geq a$; si nous prouvons que $C_a$ admet une borne supérieure, cette borne sera aussi la borne supérieure de $B$. Or, $C_a - a$ est un ensemble d’éléments $\geq 0$, majoré et filtrant pour la relation $\leq$; il a donc une borne supérieure $b$, et par suite $a + b$ est la borne supérieure de $C_a$.

D’autre part, la condition *b)* entraîne *a)*: en effet, si $F$ est un ensemble non vide d’éléments $\geq 0$ de $E$, majoré et filtrant pour $\leq$, et si $c$ est un majorant de $F$, $c - F$ est un ensemble d’éléments $\geq 0$, filtrant pour $\geq$; s’il admet une borne inférieure $m$, $c - m$ est la borne supérieure de $F$.

#### Proposition 2 {#int-ii-s1-prop-2 .statement}

*Soit E un espace de Riesz, muni d’une topologie séparée compatible avec sa structure d’espace vectoriel ordonné (Esp. vect. top., chap. II, 2e éd., § 2, n° 7). Si, pour tout ensemble $H \subset E$ majoré et filtrant pour la relation $\leq$, le filtre des sections de $H$ est convergent, E est complètement réticulé*.

En effet, on sait que la limite du filtre des sections de $H$ est la borne supérieure de $H$ dans $E$ (Esp. vect. top., chap. II, 2e éd., § 2, n° 7, prop. 18).

### 4. Sous-espaces et espaces produits d’espaces complètement réticulés

Soient E un espace complètement réticulé, H un sous-espace vectoriel de E. La structure d’ordre induite sur H par celle de E est compatible avec la structure d’espace vectoriel de H, mais l’espace vectoriel ordonné H ainsi défini n’est pas nécessairement un espace complètement réticulé.

De façon précise, il peut se faire que H ne soit pas un espace de Riesz (exerc. 2), ou que H soit un espace de Riesz non complètement réticulé : ce dernier cas est celui du sous-espace $\mathcal{C}(\mathbf{R})$ de l’espace $\mathcal{B}(\mathbf{R})$ (n° 3, exemple 2).

En outre, lorsque H est un espace de Riesz (complètement réticulé ou non) il se peut que la borne supérieure dans H de deux éléments de H soit distincte de leur borne supérieure dans E (exerc. 3 b)). Enfin, il est possible que H soit complètement réticulé, que les bornes supérieures de toute partie finie de H soient les mêmes dans E et dans H, mais qu’il existe des parties infinies de H, majorées dans H, et dont les bornes supérieures dans E et dans H soient distinctes (exerc. 13 f)).

Soit $(E_i)_{i \in I}$ une famille quelconque d’espaces vectoriels ordonnés. Rappelons que, dans l’espace produit $E = \prod_{i \in I} E_i$, la relation d’ordre produit des relations d’ordre des espaces facteurs est la relation « quel que soit $i \in I,\ x_i \leq y_i$ » (Ens., chap. III, § 1, n° 4). On vérifie aussitôt que cette relation est compatible avec la structure d’espace vectoriel de E ; E, muni de cette structure, est appelé l’espace produit des espaces ordonnés $E_i$.

#### Proposition 3 {#int-ii-s1-prop-3 .statement}

*Soit $(E_i)_{i \in I}$ une famille d’espaces vectoriels ordonnés. Pour que l’espace produit $E = \prod_{i \in I} E_i$ soit un espace de Riesz (resp. un espace complètement réticulé), il faut et il suffit que chacun des espaces $E_i$ soit un espace de Riesz (resp. un espace complètement réticulé).*

Bornons-nous à examiner le cas des espaces complètement réticulés. Supposons que tous les $E_i$ soient complètement réticulés ; soient A une partie majorée non vide de E, $a = (a_i)$ un majorant de A. Pour tout $i \in I$, $\mathrm{pr}_i A$ est majoré par $a_i$, et admet donc une borne supérieure $b_i$ dans $E_i$ ; il est clair que $b = (b_i)$ est la borne supérieure de A dans E.

Réciproquement, supposons E complètement réticulé. Soit $A_\kappa$ une partie majorée de $E_\kappa$, $A'_\kappa$ la partie de E formée des $x = (x_i)$ tels que $x_\kappa \in A_\kappa$ et $x_i = 0$ pour $i \neq \kappa$. Il est immédiat que $A'_\kappa$ est majorée dans E, donc admet une borne supérieure $b = (b_i)$; d’après la définition de la relation d’ordre produit, on a nécessairement $b_i = 0$ pour $i \neq \kappa$, et $b_\kappa$ est borne supérieure de $A_\kappa$, ce qui achève la démonstration.

#### Définition 3 {#int-ii-s1-def-3 .statement}

Soient E un espace vectoriel ordonné, V et W deux sous-espaces vectoriels supplémentaires de E. On dit que E est somme directe ordonnée de V et W si l’application canonique $(x, y) \mapsto x + y$ de l’espace vectoriel ordonné $V \times W$ sur l’espace vectoriel ordonné E est un isomorphisme.

#### Proposition 4 {#int-ii-s1-prop-4 .statement}

Pour qu’un espace vectoriel ordonné E soit somme directe ordonnée de deux sous-espaces vectoriels supplémentaires V, W, il faut et il suffit que les relations $x \in V,\ y \in W,\ x + y \geq 0$ entraînent $x \geq 0$ et $y \geq 0$.

En effet, comme $x \geq 0$ et $y \geq 0$ entraînent $x + y \geq 0$ dans E, la condition de l’énoncé exprime que $(x, y) \to x + y$ transforme l’ensemble des éléments $\geq 0$ de $V \times W$ en l’ensemble des éléments $\geq 0$ de E.

### 5. Bandes dans un espace complètement réticulé

#### Définition 4 {#int-ii-s1-def-4 .statement}

Dans un espace complètement réticulé E, on dit qu’un sous-espace vectoriel B de E est une bande s’il satisfait aux conditions suivantes : 1) les relations $x \in B,\ y \in E$ et $|y| \leq |x|$ entraînent $y \in B$; 2) pour toute partie non vide X de B, majorée dans E, la borne supérieure sup X de X dans E appartient à B.

#### Exemple {#int-ii-s1-n5-exa-1 .statement}

Dans l’espace $\mathbf{R}^A$ des fonctions numériques finies définies dans un ensemble A, l’ensemble des fonctions nulles en tous les points d’une partie M de A est une bande.

#### Remarque {#int-ii-s1-n5-rem-1 .statement}

Dans l’espace $\mathbf{R}^A$, le sous-espace $\mathcal{B}(A)$ des fonctions numériques bornées dans A satisfait à la condition 1) de la déf. 4; en outre, pour toute partie X de $\mathcal{B}(A)$ majorée dans $\mathcal{B}(A)$, l’enveloppe supérieure de X appartient à $\mathcal{B}(A)$. Mais, si A est infini, une partie de $\mathcal{B}(A)$ peut être majorée dans $\mathbf{R}^A$ sans être majorée dans $\mathcal{B}(A)$, et par suite $\mathcal{B}(A)$ n’est pas une bande dans $\mathbf{R}^A$.

Il résulte aussitôt de la déf. 4 que, si B est une bande dans E, pour toute partie non vide X de B, minorée dans E, inf X appartient à B. Toute bande B dans E, munie de la structure d’espace vectoriel ordonné induite par celle de E, est un espace complètement réticulé, et pour toute partie $X \subset B$, majorée dans B, la borne supérieure de X dans B est identique à sa borne supérieure dans E.

Toute intersection d’une famille de bandes dans un espace complètement réticulé E est encore une bande. Pour toute partie $M \subset E$, il existe une plus petite bande contenant M (puisque E est lui-même une bande); on dira que cette bande est la bande engendrée par M.

Les propriétés des bandes dans un espace complètement réticulé reposent sur la proposition suivante:

#### Proposition 5 {#int-ii-s1-prop-5 .statement}

Soient E un espace complètement réticulé, A une partie non vide de E formée d’éléments $\geqslant 0$, telle que : 1) $A + A \subset A$; 2) les relations $x \in A,\ 0 \leqslant y \leqslant x$ entraînent $y \in A$. Soit M l’ensemble des bornes supérieures dans E des parties de A majorées dans E. Dans ces conditions, tout élément $x \geqslant 0$ de E peut s’écrire sous la forme $y + z$, où $y \in M$ est la borne supérieure des éléments $v \in A$ tels que $v \leqslant x$, et où z est un élément $\geqslant 0$ étranger à tous les éléments de M.

En effet, on a $y \leqslant x$. Tout revient à montrer que $z = x - y$ est étranger à tout élément $t \in A$ (n° 1), ou encore que $u = \inf (z, t)$ est nul. Par hypothèse, on a $u \in A$ et $u \leqslant x - y$, donc $u + y \leqslant x$; pour tout $v \in A$ tel que $v \leqslant x$, on a par définition $v \leqslant y$, donc $u + v \leqslant u + y \leqslant x$; comme $u + v \in A$ par hypothèse, on a aussi $u + v \leqslant y$ par définition de y; enfin, comme $u + y$ est la borne supérieure dans E des éléments $u + v$ tels que $v \in A$ et $v \leqslant x$, on a $u + y \leqslant y$, d’où $u \leqslant 0$, ce qui achève la démonstration.

#### Théorème 1 (F. Riesz) {#int-ii-s1-thm-1 .statement}

Soit A une partie d’un espace complètement réticulé E. L’ensemble A' des éléments étrangers à tous les éléments de A est une bande; la bande A'' des éléments étrangers à tous les éléments de A' est identique à la bande engendrée par A, et E est somme directe ordonnée des bandes A' et A''.

Les propriétés des éléments étrangers, rappelées au n° 1, et la définition d’une bande, montrent aussitôt que A' est une bande, donc aussi A''. D’après la prop. 5 et la définition d’une bande, tout élément $x \geqslant 0$ de E peut s’écrire $x = y + z$, où $y \in A'$ et $z \in A''$, $y$ et $z$ étant $\geqslant 0$; comme tout élément de E est différence de deux éléments $\geqslant 0$, on a $E = A' + A''$; d’autre part, 0 étant le seul élément étranger à lui-même, on a $A' \cap A'' = \{0\}$, ce qui prouve que E est somme directe de A' et A''; enfin, comme les composants dans A' et A'' d’un élément $\geqslant 0$ de E sont $\geqslant 0$, E est somme directe ordonnée de A' et A'' (n° 4, prop. 4).

Reste à montrer que $A''$ est identique à la bande B engendrée par A. Or, E est somme directe de B et de la bande B' formée des éléments étrangers à tous les éléments de B ; comme $A \subset B$, on a $B' \subset A'$; mais d’autre part $B \subset A''$, et E est aussi somme directe de $A'$ et $A''$; on a donc nécessairement $B = A''$, $B' = A'$.

Le th. 1 et la prop. 5 permettent de donner une autre définition de la bande engendrée par un ensemble d’éléments de E :

#### Proposition 6 {#int-ii-s1-prop-6 .statement}

Soient E un espace complètement réticulé, M une partie de E, B la bande engendrée par M. Soit $M_1$ l’ensemble des éléments $\geqslant 0$ de E dont chacun est majoré par un élément de la forme $\sum_i |x_i|$, où $x_i \in M$; soit $M_2$ l’ensemble des bornes supérieures des parties majorées de $M_1$; l’ensemble $M_2$ est identique à l’ensemble des éléments $\geqslant 0$ de B.

On a évidemment $M_2 \subset B$ par définition d’une bande; d’autre part, si B’ est la bande des éléments étrangers à tous les éléments de $M_1$, le th. 1 montre que E est somme directe ordonnée de B et B’. Mais la prop. 5 prouve que tout élément $\geqslant 0$ de E est somme d’un élément de $M_2$ et d’un élément de B’, d’où la proposition.

#### Corollaire {#int-ii-s1-n5-cor-1 .statement}

Soit a un élément d’un espace complètement réticulé E. Soient $B_a$ la bande engendrée par a, $B'_a$ la bande des éléments étrangers à a. Pour tout élément $x \geqslant 0$ de E, le composant de x dans $B_a$ (pour la décomposition de E en somme directe ordonnée de $B_a$ et $B'_a$) est égal à $\sup_{n \in \mathbf{N}} (\inf (n|a|, x))$.

Cela résulte de la prop. 6 appliquée à $M = \{a\}$, et de la prop. 4.

On notera que les bandes engendrées par a et $|a|$ sont identiques. Si a et b sont deux éléments étrangers de E, A et B les bandes engendrées par a et b respectivement, tout élément de A est étranger à tout élément de B; en effet, b appartient à la bande A’ des éléments étrangers à a, d’où $B \subset A'$; et d’après le th. 1, tout élément de A est étranger à tout élément de A’.

## EXERCICES {#int-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
