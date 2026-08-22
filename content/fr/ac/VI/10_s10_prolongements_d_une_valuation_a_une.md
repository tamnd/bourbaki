---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 10
section_title: Prolongements d’une valuation à une extension transcendante
lang: fr
source: ac-v-vii-fr
pdf_pages: 0156-0163, 0193-0194
extraction: ocr
subsections:
    - "no": 1
      title: Cas d’une extension transcendante monogène.
      page: 0
      pdf_page: 156
    - "no": 2
      title: Rang rationnel d’un groupe commutatif.
      page: 0
      pdf_page: 159
    - "no": 3
      title: '*Cas d’une extension transcendante quelconque.*'
      page: 0
      pdf_page: 161
statements: 11
exercises: 2
content_sha256: 9bc2e5f67f32e7e644149dc3dc04355b9906b397d9a53ce225d606db702985e8
---

## § 10. Prolongements d’une valuation à une extension transcendante.

### 1. Cas d’une extension transcendante monogène.

#### Lemme 1 {#ac-vi-s10-lem-1 .statement}

Soient $ K $ un corps, $ \nu $ une valuation de $ K $, $ \Gamma $ son groupe des ordres, $ \Gamma' $ un groupe totalement ordonné contenant $ \Gamma $, et $ \xi $ un élément de $ \Gamma' $. Il existe une valuation $ \omega $ et une seule de $ K(X) $ telle que, pour $ P = \sum_j a_j X^j $ ($ a_j \in K $), on ait $ \omega(P) = \inf_j (\nu(a_j) + j\xi) $.

En vertu de la prop. 4 du § 3, no 2, il suffit de montrer que la formule

$$
\omega\left( \sum_j a_j X^j \right) = \inf_j (\nu(a_j) + j\xi)
$$

définit une valuation de l’anneau $ K[X] $. Comme

$$
\nu(a_j + b_j) + j\xi \geq \inf(\nu(a_j), \nu(b_j)) + j\xi = \inf(\nu(a_j) + j\xi, \nu(b_j) + j\xi),
$$

on a

$$
\omega(P + Q) \geq \inf(\omega(P), \omega(Q))
$$

pour $ P, Q $ dans $ K[X] $, l’égalité ayant lieu si $ \omega(P) \neq \omega(Q) $.

Démontrons que l’on a

$$
\omega(PQ) = \omega(P) + \omega(Q)
$$

pour $ P = \sum_j a_j X^j $ et $ Q = \sum_j b_j X^j $. Soit $ i $ (resp. $ k $) le plus petit des entiers $ j $ tels que $ \nu(a_j) + j\xi $ (resp. $ \nu(b_j) + j\xi $) prenne sa valeur minimum; notons $ \alpha $ (resp. $ \beta $) cette valeur minimum. Pour $ j, j' $ dans $ \mathbf{N} $, on a
$$
\omega(a_j b_{j'} X^{j+j'}) = \nu(a_j) + j\xi + \nu(b_{j'}) + j'\xi \geq \alpha + \beta,
$$
d’où $ \omega(PQ) \geq \alpha + \beta $ d’après (2). Considérons maintenant le terme $ cX^{i+k} $ de degré $ i + k $ de PQ; on a $ c = \sum_{n \in \mathbf{Z}} a_{i+n} b_{k-n} $; d’après le choix de $ i $ et $ k $, l’élément
$$
\omega(a_{i+n} b_{k-n} X^{i+k}) = \nu(a_{i+n}) + (i+n)\xi + \nu(b_{k-n}) + (k-n)\xi
$$
prend une fois et une seule, pour $ n = 0 $, sa valeur minimum $ \alpha + \beta $; on a donc $ \omega(cX^{i+k}) = \alpha + \beta $, d’où, d’après (1),
$$
\omega(PQ) = \alpha + \beta = \omega(P) + \omega(Q).
$$
C.Q.F.D.

PROPOSITION 1. — Soient K un corps, $ \nu $ une valuation de K, $ \Gamma $ son groupe des ordres, $ \Gamma' $ un groupe totalement ordonné contenant $ \Gamma $, et $ \xi $ un élément de $ \Gamma' $ tel que les relations $ n\xi \in \Gamma, n \in \mathbf{Z} $, entraînent $ n = 0 $. Il existe alors une valuation $ \omega $ et une seule de K(X) à valeurs dans $ \Gamma' $ et prolongeant $ \nu $, telle que $ \omega(X) = \xi $. Le corps résiduel de $ \omega $ est égal à celui de $ \nu $, et son groupe des ordres est le sous-groupe $ \Gamma + \mathbf{Z}\xi $ de $ \Gamma' $.

Démontrons d’abord l’unicité de $ \omega $. Soit $ P = \sum_j a_j X^j $ un élément de K[X]. On a $ \omega(a_j X^j) = \nu(a_j) + j\xi $, ce qui montre que les monômes $ a_j X^j $ tels que $ a_j \neq 0 $ ont des valeurs distinctes pour $ \omega $. Il s’ensuit que $ \omega(P) = \inf_j (\nu(a_j) + j\xi) $, ce qui montre à la fois l’unicité de $ \omega $ sur K[X] (donc aussi sur K(X)) et le fait que le groupe des ordres de $ \omega $ est $ \Gamma + \mathbf{Z}\xi $. On voit en outre que, si $ P \neq 0 $, on peut écrire $ P = aX^n(1+u) $ avec $ a \in K^*, n \in \mathbf{N}, u \in K(X) $ et $ \omega(u) > 0 $; tout élément $ R \neq 0 $ de K(X) peut donc s’écrire sous la forme $ R = bX^n(1+u') $, avec $ b \in K^*, n \in \mathbf{Z}, u' \in K(X) $ et $ \omega(u') > 0 $; on a $ \omega(R) = \nu(b) + n\xi $, donc $ \omega(R) = 0 $ si et seulement si $ \nu(b) = 0 $ et $ n = 0 $; ainsi, lorsque $ \omega(R) = 0 $, R et b sont congrus modulo l’idéal de $ \omega $, ce qui montre que le corps résiduel de $ \omega $ est égal à celui de $ \nu $.

Enfin l’existence de $ \omega $ résulte du lemme 1.

PROPOSITION 2. — Soient K un corps, $ \nu $ une valuation de K, $ \Gamma $ son groupe des ordres, et k son corps résiduel. Il existe une valuation $ \omega $ et une seule de K(X) prolongeant $ \nu $, telle que $ \omega(X) = 0 $ et que l’image t de X dans le corps résiduel k’ de ω soit transcendante sur k. Le groupe des ordres de ω est égal à celui de v, et son corps résiduel est k(t).

Pour montrer l’unicité de ω, il nous suffira de montrer que, si P = $ \sum_j a_j X^j $ est un élément non nul de K[X], on a
$$
\omega(P) = \inf_j (\nu(a_j)).
$$
Quitte à diviser P par un élément de K*, on peut supposer qu’on a $ \nu(a_j) \geq 0 $ pour tout j, et que l’un des $ \nu(a_j) $ est nul. Comme $ \omega(X) = 0 $, P appartient alors à l’anneau de ω ; notant $ \bar{a}_j $ l’image canonique de $ a_j $ dans k, l’image canonique de P dans le corps résiduel $ k' $ est $ \sum_j \bar{a}_j t^j $; comme t est transcendant sur k et que l’un des $ \bar{a}_j $ est non nul, cette image est non nulle, d’où
$$
\omega(P) = 0 = \inf_j (\nu(a_j)).
$$

Démontrons maintenant l’existence de ω. La formule $ \omega(P) = \inf_j (\nu(a_j)) $ (pour $ P = \sum_j a_j X^j $) définit une valuation ω de K(X) en vertu du lemme 1, et ω a évidemment même groupe des ordres que v. On a $ \omega(X) = 0 $. Montrons que l’image canonique t de X dans le corps résiduel $ k' $ de ω est transcendante sur k : en effet, si $ \sum_j \bar{a}_j t^j = 0 $ avec $ \bar{a}_j \in k $ pour tout j, on a, en désignant par $ a_j $ un représentant de $ \bar{a}_j $ dans l’anneau de v, $ \omega(\sum_j a_j X^j) > 0 $; d’où $ \nu(a_j) > 0 $ pour tout j, donc $ \bar{a}_j = 0 $ pour tout j. Montrons enfin qu’on a $ k' = k(t) $ : en effet, tout élément R de K(X) peut s’écrire $ R = c (\sum_j a_j X^j)/(\sum_j b_j X^j) $, avec $ c, a_j, b_j $ dans K, $ \nu(a_j) \geq 0 $ et $ \nu(b_j) \geq 0 $ pour tout j, l’un des $ \nu(a_j) $ et l’un des $ \nu(b_j) $ étant nul ; on a $ \omega(R) \geq 0 $ si et seulement si $ \nu(c) \geq 0 $ ; en notant f l’homomorphisme canonique de l’anneau de ω sur $ k' $, on a
$$
f(R) = f(c)(\sum_j f(a_j)t^j)/(\sum_j f(b_j)t^j),
$$
ce qui démontre notre assertion.

#### Remarque {#ac-vi-s10-n1-rem-1 .statement}

Il ne faudrait pas croire que les deux types de prolongements de v à K(X) que nous venons de rencontrer soient les seuls ; il peut exister un troisième type de prolongement, où $ \Gamma'/\Gamma $ est un groupe de torsion, et $ k' $ une extension algébrique

### 2. Rang rationnel d’un groupe commutatif.

#### Définition 1 {#ac-vi-s10-def-1 .statement}

On appelle rang rationnel d’un groupe commutatif $ G $ la dimension du $ \mathbf{Q} $-espace vectoriel $ G \otimes_{\mathbf{Z}} \mathbf{Q} $.

Cette dimension peut aussi être définie comme la borne supérieure (finie ou infinie) des cardinaux $ r $ tels qu’il existe $ r $ éléments de $ G $ linéairement indépendants sur $ \mathbf{Z} $ (Alg., chap. II, 3e éd., § 7, no 10, prop. 26). Le rang rationnel de $ G $ est *nul* si et seulement si $ G $ est un groupe de torsion. Pour un sous-groupe d’un groupe additif $ \mathbf{R}^n $, la notion de rang rationnel coïncide avec celle définie en Top. gén., chap. VII, § 1.

Dans la suite de ce paragraphe, nous noterons $ r(G) $ le rang rationnel du groupe commutatif $ G $. Si $ G' $ est un sous-groupe de $ G $, on a (puisque $ \mathbf{Q} $ est un $ \mathbf{Z} $-module plat) la formule d’additivité

$$
r(G) = r(G') + r(G/G').
$$

#### Proposition 3 {#ac-vi-s10-prop-3 .statement}

Soient $ G $ un groupe commutatif totalement ordonné, et $ H $ un sous-groupe de $ G $. Si l’on note $ h(G) $ et $ h(H) $ les hauteurs de $ G $ et $ H $ ($ \S 4 $, no 4), on a l’inégalité

$$
h(G) \leq h(H) + r(G/H).
$$

Soit, en effet, $ G_0 \subset G_1 \subset \cdots \subset G_n $ une suite strictement croissante de sous-groupes isolés de $ G $. On doit établir l’inégalité

$$
n \leq h(H) + r(G/H).
$$

Elle est évidente pour $ n = 0 $. Supposons $ n \geq 1 $, et raisonnons par récurrence sur $ n $. En appliquant l’hypothèse de récurrence au groupe $ G_{n-1} $ et à son sous-groupe $ H \cap G_{n-1} $; on obtient

$$
n - 1 \leq h(H \cap G_{n-1}) + r(G_{n-1}/(H \cap G_{n-1})).
$$

Distinguons alors deux cas :

a) On a $ H \cap G_{n-1} = H $, autrement dit $ H \subset G_{n-1} $. L’inégalité (7) s’écrit

$$
n \leq h(H) + r(G_{n-1}/H) + 1.
$$

Or $ G/G_{n-1} $ est un groupe totalement ordonné non réduit à 0; ce n’est donc pas un groupe de torsion, et l’on a $ r(G/G_{n-1}) \geq 1 $.

D’où, d’après (4), $ r(G/H) \geq r(G_{n-1}/H) + 1 $. En portant dans (8), on obtient bien l’inégalité (6) cherchée.

$ b) $ On a $ H \cap G_{n-1} \neq H $. Comme $ H \cap G_{n-1} $ est un sous-groupe isolé de $ H $, on en conclut que $ h(H) \geq h(H \cap G_{n-1}) + 1 $. D’autre part on a évidemment $ r(G/H) \geq r(G_{n-1}/(H \cap G_{n-1})) $. En portant dans (7), on obtient encore (6).

#### Corollaire {#ac-vi-s10-n2-cor-1 .statement}

*Pour tout groupe commutatif totalement ordonné* $ G $, *on a* $ h(G) \leq r(G) $.
On fait $ H = \{0\} $ dans la prop. 3.

#### Proposition 4 {#ac-vi-s10-prop-4 .statement}

*Soit* $ G $ *un groupe commutatif totalement ordonné*. *On suppose que* $ G $ *est de type fini, et qu’on a* $ h(G) = r(G) $. *Alors* $ G $ *est isomorphe à* $ \mathbf{Z}^{r(G)} $ *ordonné lexicographiquement*.

Posons $ r = r(G) = h(G) $. Si $ r = 0 $, on a $ G = \{0\} $. Si $ r = 1 $, la structure des groupes commutatifs de type fini montre qu’on a un isomorphisme $ j $ de $ G $ sur $ \mathbf{Z} $ (*Alg.*, chap. VII, § 4, no 6, th. 3). Or $ \mathbf{Z} $ ne possède que deux structures d’ordre total compatibles avec sa structure de groupe, à savoir la structure d’ordre usuelle et son opposée. Donc $ j $ ou — $ j $ est un isomorphisme du groupe ordonné $ G $ sur $ \mathbf{Z} $ muni de l’ordre usuel.

Supposons maintenant qu’on ait $ r \geq 2 $, et raisonnons par récurrence sur $ r $. Soit $ H $ un sous-groupe isolé de $ G $, de hauteur $ r - 1 $. On a $ r(H) + r(G/H) = r $ (formule (4)), $ r(H) \geq h(H) = r - 1 $ et $ r(G/H) \geq h(G/H) = 1 $ (cor. de la prop. 3), d’où $ r(H) = r - 1 $ et $ r(G/H) = 1 $. L’hypothèse de récurrence montre que $ H $ est isomorphe à $ \mathbf{Z}^{r-1} $ ordonné lexicographiquement, et le cas $ r = 1 $ montre que $ G/H $ est isomorphe à $ \mathbf{Z} $. Comme $ \mathbf{Z} $ est un $ \mathbf{Z} $-module libre, $ H $ est un *facteur direct* dans $ G $ (*Alg.*, chap. II, 3e éd., § 1, no 11, prop. 21). Le lemme suivant montre alors que $ G $ est isomorphe (non canoniquement) au produit lexicographique $ H \times (G/H) $, ce qui achève la démonstration.

#### Lemme 2 {#ac-vi-s10-lem-2 .statement}

*Soit* $ H $ *un sous-groupe isolé d’un groupe commutatif totalement ordonné* $ G $. *Si* $ H $ *est facteur direct dans* $ G $, *le groupe ordonné* $ G $ *est isomorphe au groupe* $ (G/H) \times H $ *ordonné lexicographiquement*.

Soit $ j $ un isomorphisme de groupes de $ (G/H) \times H $ sur $ G $ tel que $ j(0, x) = x $ pour tout $ x \in H $, et que $ j(y, x) $ admette $ y $ pour classe modulo $ H $. Comme $ (G/H) \times H $ est totalement ordonné, tout revient à montrer que $ j $ est *croissant* (*Ens.*, chap. III, 2e éd., § 1, no 12, prop. 11). Soit $(y, x)$ un élément $\geqslant 0$ de $(G/H) \times H$ ordonné lexicographiquement. Si $y > 0$, la classe de $j(y, x)$ modulo $H$ est un élément $> 0$, d’où $j(y, x) > 0$, car, sinon, on aurait $y \leqslant 0$ (\S 4, no 2, prop. 3). Si $y = 0$ et $x \geqslant 0$, on a $j(y, x) = x \geqslant 0$. Donc $j$ est bien croissant.

### 3. *Cas d’une extension transcendante quelconque.*

Dans ce no nous utiliserons les notations suivantes : K est un corps, $K'$ une extension de K, $\nu$ une valuation de K, $\nu'$ un prolongement de $\nu$ à $K'$, $\Gamma$ et $k$ (resp. $\Gamma'$ et $k'$) le groupe des ordres et le corps résiduel de $\nu$ (resp. $\nu'$). Nous poserons :

$$
d(K'/K) = \dim.\mathrm{al}_K K' = \text{degré de transcendance de } K' \text{ sur } K; \\
s(\nu'/\nu) = \dim.\mathrm{al}_k k' = \text{degré de transcendance de } k' \text{ sur } k; \\
r(\nu'/\nu) = r(\Gamma'/\Gamma) = \text{rang rationnel de } \Gamma'/\Gamma,
$$

si les membres de droite sont finis ; sinon, nous conviendrons de poser $d(K'/K) = +\infty$ (resp. $s(\nu'/\nu) = +\infty,\ r(\nu'/\nu) = +\infty$).

#### Théorème 1 {#ac-vi-s10-thm-1 .statement}

*Soient $x_1, \ldots, x_s$ des éléments de l’anneau de $\nu'$ dont les images canoniques $\overline{x}_i$ dans $k'$ soient algébriquement indépendantes sur $k$, et $y_1, \ldots, y_r$ des éléments de $K'$ tels que les images canoniques des $\nu'(y_j)$ dans $\Gamma'/\Gamma$ soient linéairement indépendantes sur $\mathbf{Z}$. Alors les $r+s$ éléments $x_1, \ldots, x_s, y_1, \ldots, y_r$ de $K'$ sont algébriquement indépendants sur $K$; la restriction de $\nu'$ à $K(x_1, \ldots, x_s, y_1, \ldots, y_r)$ admet $k(\overline{x}_1, \ldots, \overline{x}_s)$ pour corps résiduel, et $\Gamma + \mathbf{Z}\nu'(y_1) + \cdots + \mathbf{Z}\nu'(y_r)$ pour groupe des ordres.*

Notre assertion est évidente si $r+s=0$. Procédons par récurrence sur $r+s$. Si $r' \leqslant r,\ s' \leqslant s$ et $r'+s' < r+s$, l’hypothèse de récurrence montre que les hypothèses du th. 1 sont vérifiées si l’on remplace K par $K(x_1, \ldots, x_{s'}, y_1, \ldots, y_{r'})$ et les familles $(x_1, \ldots, x_s), (y_1, \ldots, y_r)$ par $(x_{s'+1}, \ldots, x_s), (y_{r'+1}, \ldots, y_r)$. Nous sommes donc ramenés à l’un des deux cas suivants :

a) On a un élément $x$ de l’anneau de $\nu'$ tel que $\overline{x}$ soit transcendant sur $k$; il s’agit de montrer que $x$ est transcendant sur $K$, et que la restriction de $\nu'$ à $K(x)$ admet $k(\overline{x})$ pour corps résiduel et $\Gamma$ pour groupe des ordres.

b) On a un élément $y$ de $K'$ tel que les relations $n\nu'(y) \in \Gamma$ et $n \in \mathbf{Z}$ entraînent $n=0$; il s’agit de montrer que $y$ est transcendant sur $ K $, et que la restriction de $ \nu' $ à $ K(y) $ admet $ k $ pour corps résiduel, et $ \Gamma + \mathbf{Z}\nu'(y) $ pour groupe des ordres.

Or la prop. 1 du § 8, no 1 montre que $ x $ (resp. $ y $) ne peut être algébrique sur $ K $. Les autres assertions de $ a) $ (resp. $ b$) ) s’en déduisent aussitôt en vertu de la prop. 2 (resp. prop. 1) du no 1.

#### Corollaire 1 {#ac-vi-s10-thm-1-cor-1 .statement}

*On a l’inégalité*

$$
s(\nu'/\nu) + r(\nu'/\nu) \leq d(K'/K).
$$

*De plus, si $ K' $ est une extension de type fini de $ K $, et s’il y a égalité dans (9), alors $ \Gamma'/\Gamma $ est un $ \mathbf{Z} $-module de type fini, et $ k' $ est une extension de type fini de $ k $.

Soient $ r $ et $ s $ des entiers naturels tels que $ r \leq r(\nu'/\nu) $ et $ s \leq s(\nu'/\nu) $; montrons, ce qui prouvera (9), qu’on a $ r + s \leq d(K'/K) $. Par hypothèse, il existe des éléments $ x_1, \ldots, x_s, y_1, \ldots, y_r $ de $ K' $ qui vérifient les hypothèses du th. 1. Il sont donc algébriquement indépendants sur $ K $, ce qui démontre l’inégalité $ r + s \leq d(K'/K) $.

Si $ K' $ est une extension de type fini de $ K $, $ d(K'/K) $ est fini, donc $ s(\nu'/\nu) $ et $ r(\nu'/\nu) $ sont aussi finis; notons-les $ s $ et $ r $. Il existe des éléments $ x_1, \ldots, x_s, y_1, \ldots, y_r $ de $ K' $ qui vérifient les hypothèses du th. 1. Si $ r + s = d(K'/K) $, ces éléments forment une base de transcendance de $ K' $ sur $ K $, et $ K' $ est donc une extension algébrique de degré fini de $ K'' = K(x_1, \ldots, y_r) $. Soient $ \Gamma'' $ et $ k'' $ le groupe des ordres et le corps résiduel de la restriction de $ \nu' $ à $ K'' $. D’après le th. 1, $ \Gamma''/\Gamma $ est un $ \mathbf{Z} $-module de type fini, et $ k'' $ est une extension pure de type fini de $ k $. D’autre part, comme $ K' $ est une extension algébrique de degré fini de $ K'' $, $ \Gamma'/\Gamma'' $ est un groupe fini, et $ k' $ est une extension algébrique de degré fini de $ k'' $ ($ § 8 $, no 1, lemme 2). Ceci démontre le corollaire 1.

#### Corollaire 2 {#ac-vi-s10-thm-1-cor-2 .statement}

*Soient $ h $ et $ h' $ les hauteurs de $ \nu $ et $ \nu' $. On a alors*

$$
s(\nu'/\nu) + h' \leq d(K'/K) + h.
$$

En effet, d’après la prop. 3, on a $ h' \leq r(\nu'/\nu) + h $.

#### Corollaire 3 {#ac-vi-s10-thm-1-cor-3 .statement}

*Supposons que $ K' $ soit une extension de type fini de $ K $, que $ \Gamma $ soit isomorphe à $ \mathbf{Z}^h $ (ordonné lexicographiquement), et qu’il y ait égalité dans la formule (10). Alors $ \Gamma' $ est isomorphe à $ \mathbf{Z}^{h'} $ (ordonné lexicographiquement), et $ k' $ est une extension de type fini de $ k $.*

S’il y a égalité dans (10), il y a égalité dans (9), d’où le fait que $ k' $ est une extension de type fini de $ k $, et que $ \Gamma' $ est un $ \mathbf{Z} $-module de type fini. De plus, en comparant (9) et (10), on voit que $ h' - h = r(\Gamma'/\Gamma) $, d’où $ h' = r(\Gamma') $, et la prop. 4 (n° 2) montre alors que $ \Gamma' $ est isomorphe à $ \mathbf{Z}^{h'} $ ordonné lexicographiquement.

COROLLAIRE 4. — Supposons que $ \varphi $ soit impropre (auquel cas $ k = K $). On a alors

(11) $$ h(\Gamma') + d(k'/K) \leq r(\Gamma') + d(k'/K) \leq d(K'/K). $$

Si, en particulier, $ \varphi' $ est de hauteur 1, on a

(12) $$ d(k'/K) \leq d(K'/K) - 1; $$

de plus, si $ K' $ est une extension de type fini de $ K $ et s’il y a égalité dans (12), alors $ \varphi' $ est une valuation discrète, et $ k' $ est une extension de type fini de $ K $.

C’est une série de cas particuliers des corollaires 1, 2, 3.

## EXERCICES {#ac-vi-s10-exercises}

See the [exercises for § 10](exercises/s10/).
