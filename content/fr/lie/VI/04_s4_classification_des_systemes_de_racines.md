---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: Systèmes de racines
section: 4
section_title: Classification des systèmes de racines
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0187-0222, 0227-0232
extraction: ocr
subsections:
    - "no": 1
      title: Groupes de Coxeter finis
      page: 0
      pdf_page: 187
    - "no": 2
      title: Graphes de Dynkin
      page: 0
      pdf_page: 194
    - "no": 3
      title: Groupe de Weyl affine et graphe de Dynkin complété
      page: 0
      pdf_page: 197
    - "no": 4
      title: Préliminaires à la construction des systèmes de racines
      page: 0
      pdf_page: 199
    - "no": 5
      title: Systèmes de type $B_l$ ($l \geqslant 2$)
      page: 0
      pdf_page: 201
    - "no": 6
      title: Systèmes de type $C_l$ ($l \geq 2$).
      page: 0
      pdf_page: 203
    - "no": 7
      title: Systèmes de type $A_l$ ($l \geq 1$).
      page: 0
      pdf_page: 204
    - "no": 8
      title: Systèmes de type $D_l$ ($l \geq 3$).
      page: 0
      pdf_page: 207
    - "no": 9
      title: Système de type $F_4$
      page: 0
      pdf_page: 210
    - "no": 10
      title: Système de type $E_8$
      page: 0
      pdf_page: 212
    - "no": 11
      title: Système de type $E_7$
      page: 0
      pdf_page: 215
    - "no": 12
      title: Système de type $E_6$
      page: 0
      pdf_page: 217
    - "no": 13
      title: Système de type $G_2$
      page: 0
      pdf_page: 219
    - "no": 14
      title: Systèmes de racines irréductibles non réduits
      page: 0
      pdf_page: 221
statements: 19
exercises: 10
content_sha256: 87e924732fb81e26f6841a677253e89e0878f90f47e9bc3c9ae0ca23ca054890
---

## § 4. Classification des systèmes de racines

### 1. Groupes de Coxeter finis

Nous nous proposons dans ce paragraphe de déterminer, à isomorphisme près, tous les systèmes de racines, et par conséquent tous les groupes cristallographiques (§ 2, no 5). Plus généralement, nous allons commencer par déterminer tous les groupes finis engendrés par des réflexions dans des espaces vectoriels réels de dimension finie : il revient au même (chap. V, § 4, no 8) de déterminer tous les groupes de Coxeter finis, ou encore (chap. V, § 4, no 8, th. 2) toutes les matrices de Coxeter d’ordre fini telles que la forme bilinéaire associée soit positive non dégénérée.

Soit $M = (m_{ij})_{i,j \in I}$ une matrice de Coxeter d’ordre $l$ fini. Posons

$$
q_{ij} = - \cos (\pi / m_{ij}).
$$

Rappelons que $q_{ii} = 1$ et que $q_{ij} = q_{ji}$ est nul ou $\leq -1/2$ pour $i \neq j$. Posons $E = \mathbf{R}^I$ et soit $(e_i)_{i \in I}$ la base canonique de $E$. Nous noterons $(x|y)$ la forme bilinéaire sur $E$ associée à $M$ (chap. V, § 4, no 1) et $q$ la forme quadratique $x \mapsto (x|x)$ sur $E$. Pour $x = \sum_{i \in I} \xi_i e_i \in E$, on a

$$
||x||^2 = q(x) = \sum_{i,j \in I} q_{ij} \xi_i \xi_j.
$$

Nous désignerons par $(\mathbf{X}, f)$ le graphe de Coxeter de $M$ (chap. IV, § 1, no 9). Si $a$ est une arête de $\mathbf{X}$, nous dirons que $f(a)$ est l’ordre de $a$.

Dans toute la suite de ce numéro, nous supposerons que le groupe de Coxeter $W(M)$ défini par $M$ (chap. V, § 4, no 3) est fini, de sorte que $q$ est positive non dégénérée et que $\mathbf{X}$ est une forêt (chap. V, § 4, no 8, prop. 8). Nous supposerons de plus que $\mathbf{X}$ est connexe (autrement dit que le groupe de Coxeter $W(M)$ est irréductible), de sorte que $\mathbf{X}$ est un arbre.

En exprimant que $q$ est positive non dégénérée, nous obtiendrons des conditions sur les $m_{ij}$ qui permettront de dresser la liste des possibilités pour les graphes de Coxeter correspondants; il restera ensuite à voir que ces possibilités sont effectivement réalisées, c’est-à-dire que les groupes $W(M)$ correspondants sont finis.

#### Lemme 1 {#lie-vi-s4-lem-1 .statement}

*Pour tout $i$, on a* $\sum_{j \neq i} q_{ij}^2 < 1$.

Soit $J$ l’ensemble des $j \in I$ distincts de $i$ tels que $q_{ij} \neq 0$, c’est-à-dire tels que $\{i, j\}$ soit une arête de $\mathbf{X}$. Si $j, j' \in J$ et $j \neq j'$, $\{j, j'\}$ n’est pas une arête (sinon $i, j, j'$ formeraient un circuit), donc $(e_j|e_{j'}) = 0$. Soit $F = \sum_{j \in J} \mathbf{R} e_j$. Alors $(e_j)_{j \in J}$ est une base orthonormale de $F$. La distance $d$ de $e_i$ à $F$ est donnée par $d^2 = 1 - \sum_{j \in J} (e_i|e_j)^2 = 1 - \sum_{j \in J} q_{ij}^2 = 1 - \sum_{j \neq i} q_{ij}^2$, d’où le lemme.

#### Lemme 2 {#lie-vi-s4-lem-2 .statement}

*Un sommet de $\mathbf{X}$ ne peut appartenir qu’à 3 arêtes au plus.*

En effet, si $i$ est lié à $h$ autres sommets, les relations $q_{ij}^2 \geq \frac{1}{4}$ pour ces autres sommets entraînent $\frac{h}{4} < 1$ d’après le lemme 1, donc $h \leq 3$.

#### Lemme 3 {#lie-vi-s4-lem-3 .statement}

*Si $i$ appartient à 3 arêtes, ces arêtes sont d’ordre 3.*

Dans le cas contraire, on aurait, compte tenu de la relation $\cos \frac{\pi}{4} = \frac{\sqrt{2}}{2}$,

$$
\sum_{j \neq i} q_{ij}^2 \geq \frac{1}{4} + \frac{1}{4} + (\frac{\sqrt{2}}{2})^2 = 1
$$

ce qui est impossible (lemme 1).

#### Lemme 4 {#lie-vi-s4-lem-4 .statement}

*S’il existe une arête d’ordre $\geq 6$, on a $l = 2$.*

Soit en effet $\{i, j\}$ cette arête. Si on avait $l > 2$, un des sommets $i, j$ (par exemple $i$) serait lié à un troisième sommet $j'$, puisque $\mathbf{X}$ est connexe. Compte tenu de la relation $\cos \frac{\pi}{6} = \frac{\sqrt{3}}{2}$ on aurait

$$
\sum_{k \neq i} q_{ik}^2 \geq \frac{1}{4} + (\frac{\sqrt{3}}{2})^2 = 1
$$

ce qui est impossible (lemme 1).

#### Lemme 5 {#lie-vi-s4-lem-5 .statement}

Un sommet ne peut appartenir à deux arêtes distinctes d’ordre $\geqslant 4$.

Soit $i$ un tel sommet. On aurait $\sum_{j \neq i} q_{ij}^2 \geq (\frac{\sqrt{2}}{2})^2 + (\frac{\sqrt{2}}{2})^2 = 1$, ce qui est impossible (lemme 1).

Soit $\{i, j\}$ une arête de $X$. Nous allons définir un nouveau graphe de Coxeter, qui sera dit déduit du graphe de $M$ par identification de $i$ et $j$. L’ensemble $I'$ des sommets est l’ensemble quotient de $I$ obtenu en identifiant $i$ et $j$. Posons $p = \{i, j\}$, qui est un élément de $I'$, et identifions les éléments de $I$ distincts de $i$ et $j$ à leurs images canoniques dans $I'$. Soient $k, k'$ deux éléments distincts de $I'$. Alors $\{k, k'\}$ est une arête du nouveau graphe dans les cas suivants :

1) $k$ et $k'$ sont distincts de $p$, et $\{k, k'\}$ est une arête de $X$; dans ce cas, on définit l’ordre de cette arête comme égal à $m_{kk'}$;

2) $k = p$, et l’un des ensembles $\{i, k'\}, \{j, k'\}$ est une arête de $X$; on définit l’ordre de $\{p, k'\}$ comme égal à $m_{ik'}$ si $\{i, k'\}$ est une arête de $X$, à $m_{jk'}$ si $\{j, k'\}$ est une arête de $X$ (les deux éventualités ne peuvent se produire simultanément puisque $X$ est un arbre).

Soit $M' = (m'_{ij})_{i,j \in I'}$ la nouvelle matrice de Coxeter ainsi définie, et posons $q'_{ij} = -\cos \frac{\pi}{m'_{ij}}$. On a, pour $k \neq p$, $q'_{pk} = q_{ik} + q_{jk}$. Donc, si $(\xi_i) \in \mathbf{R}^{I'}$,

$$
\sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k, k' \in I - \{i, j\}} q_{kk'} \xi_k \xi_{k'} + 2 \sum_{k \in I - \{i, j\}} (q_{ik} + q_{jk}) \xi_k \xi_p + \xi_p^2.
$$

Posons $\xi_i = \xi_j = \xi_p$; on obtient

(1)
$$
\sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} + \xi_p^2 - \xi_i^2 - \xi_j^2 - 2q_{ij} \xi_i \xi_j \\
= \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} - (1 + 2q_{ij}) \xi_p^2.
$$

#### Lemme 6 {#lie-vi-s4-lem-6 .statement}

Si $\{i, j\}$ est d’ordre 3, $W(M')$ est un groupe de Coxeter fini.

En effet, on a $q_{ij} = -\frac{1}{2}$, donc (1) devient

(2)
$$
\sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'}
$$
donc $(\xi_k)_{k \in I'} \mapsto \sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'}$ est une forme quadratique positive non dégénérée. Il suffit alors d’appliquer le th. 2 du chap. V, § 4, no 8.

#### Lemme 7 {#lie-vi-s4-lem-7 .statement}

On a l’alternative suivante :
a) $X$ possède un point de ramification (chap. IV, Annexe, no 1) et un seul, et toutes les arêtes de $X$ sont d’ordre 3.
b) $X$ est une chaîne, et possède au plus une arête d’ordre $\geqslant 4$.
Raisonnons par récurrence sur $l$.
a) Supposons que $X$ possède un point de ramification $i$. Alors $i$ appartient à 3 arêtes d’ordre 3, $\{i, k_1\}, \{i, k_2\}, \{i, k_3\}$ (lemmes 2 et 3). Si $l = 4$, le lemme est démontré. Sinon, $k_1$ par exemple appartient à une arête distincte des précédentes puisque $X$ est connexe. Identifions $i$ et $k_1$ dans le graphe de Coxeter de $M$. On obtient un nouveau graphe auquel on peut appliquer l’hypothèse de récurrence grâce au lemme 6. Or l’image $p$ de $i$ est point de ramification du nouveau graphe $X'$. Donc $X'$ n’a aucun autre point de ramification et a toutes ses arêtes d’ordre 3. Donc $X$ a toutes ses arêtes d’ordre 3, et n’a aucun point de ramification distinct de $i$ et $k_1$. Si $k_1$ était point de ramification dans $X$, $p$ appartiendrait à au moins 4 arêtes dans $X'$, contrairement au lemme 2.

b) Supposons que $X$ ne possède aucun point de ramification. Alors $X$ est une chaîne (chap. IV, Annexe, n° 3, prop. 3). Soit $\{i, j\}$ une arête d’ordre $\geqslant 4$. Si $l = 2$, le lemme est trivial. Sinon, $i$ par exemple appartient à une arête $\{i, k\}$ avec $k \neq j$ (puisque $X$ est connexe). Cette arête est d’ordre 3 (lemme 5). Identifions $i$ et $k$ dans le graphe de Coxeter de $M$. Grâce au lemme 6, on peut appliquer l’hypothèse de récurrence. Soit $p$ l’image de $i$ dans le nouveau graphe $X'$. Dans $X'$, $\{p, j\}$ est une arête d’ordre $\geqslant 4$, donc $X'$ n’a aucune autre arête d’ordre $\geqslant 4$, donc $\{i, j\}$ est la seule arête d’ordre $\geqslant 4$ dans $X$.

#### Lemme 8 {#lie-vi-s4-lem-8 .statement}

Soient $i_1, i_2, \ldots, i_p$ des sommets de $X$ tels que $\{i_1, i_2\}, \{i_2, i_3\}, \ldots, \{i_{p-1}, i_p\}$ soient des arêtes d’ordre 3. Alors $q \left( \sum_{r=1}^p r e_{i_r} \right) = \frac{1}{2} p(p+1)$.

On a $(e_{i_r}|e_{i_r}) = 1,\ (e_{i_r}|e_{i_{r+1}}) = -\frac{1}{2},\ (e_{i_r}|e_{i_s}) = 0$ si $s > r + 1$. Donc

$$
q \left( \sum_{r=1}^p r e_{i_r} \right) = \sum_{r=1}^p r^2 - 2 \sum_{r=1}^{p-1} \frac{1}{2} r(r+1) = p^2 - \sum_{r=1}^{p-1} r.
$$

D’après Ens., chap. III, § 5, n° 8, cor. de la prop. 14, ceci vaut

$$
p^2 - \frac{1}{2} p(p-1) = \frac{1}{2} p(p+1).
$$

#### Lemme 9 {#lie-vi-s4-lem-9 .statement}

Supposons que $X$ soit une chaîne ayant pour sommets $1, 2, \ldots, l$ et pour arêtes $\{1, 2\}, \{2, 3\}, \ldots, \{l-1, l\}$.

(i) Si l’une des arêtes $\{2, 3\}, \{3, 4\}, \ldots, \{l-2, l-1\}$ est d’ordre $\geqslant 4$, cette arête est d’ordre 4, et le graphe est le suivant :

$$
\begin{array}{cccc}
\circ & \circ & \circ & \\
\hline
& 4 &
\end{array}
$$

(ii) Si l’arête $\{1, 2\}$ est d’ordre 5, le graphe est l’un des suivants :

$$
\begin{array}{cccc}
\circ & 5 & \circ & \\
\circ & 5 & \circ & \\
\circ & 5 & \circ & \\
\end{array}
$$

On peut supposer $l > 2$ (lemme 4). Supposons que $\{i, i+1\}$ soit d’ordre $\geqslant 4$, avec $1 \leqslant i \leqslant l-1$. Posons

$$
x = e_1 + 2e_2 + \cdots + ie_i,\quad y = e_l + 2e_{l-1} + \cdots + (l-i)e_{i+1},\quad \text{et}\quad j = l-i.
$$

D’après le lemme 8, on a $\|x\|^2 = \frac{1}{2} i(i+1)$, $\|y\|^2 = \frac{1}{2} j(j+1)$. D’autre part, $(x|y) = ij(e_i|e_{i+1}) = -ij \cos \frac{\pi}{m}$ avec $m = 4$ ou $5$ (lemme 4). On a

$$
(x|y)^2 < \|x\|^2 \|y\|^2,
$$

c’est-à-dire

$$
\frac{1}{4} ij(i+1)(j+1) > i^2 j^2 \cos^2 \frac{\pi}{m}
$$

d’où

(3)
$$
(i+1)(j+1) > 4ij \cos^2 \frac{\pi}{m} \geq 2ij.
$$

Ceci donne d’abord $ij - i - j - 1 < 0$, ou $(i-1)(j-1) < 2$. Si

$$
1 < i < l-1,
$$

on a $1 < j < l-1$, donc $i = j = 2$, et en outre

$$
9 > 16 \cos^2 \frac{\pi}{m}, \text{ donc } \cos^2 \frac{\pi}{m} < \cos^2 \frac{\pi}{5} (*),
$$

donc $m = 4$. Ceci prouve (i). Si $i = 1$ et $m = 5$, on a $2j + 2 > 4j \frac{3+\sqrt{5}}{8}$, ou $j \frac{\sqrt{5}-1}{2} < 2, j < \sqrt{5} + 1 < 4$, donc $l = j + 1 \leq 4$. Ceci prouve (ii).

#### Lemme 10 {#lie-vi-s4-lem-10 .statement}

*Si X admet un point de ramification i, le sous-graphe plein X—{i} est réunion de trois chaînes, et si p—1, q—1, r—1 sont les longueurs de ces chaînes, le triplet (p, q, r) est égal, à une permutation près, à l’un des triplets (1, 2, 2), (1, 2, 3, ), (1, 2, 4), (1, 1, m) (m quelconque $\geq 1$).

Le sommet i appartient à 3 arêtes (lemme 2), et il n’existe aucun autre point de ramification (lemme 7), donc le sous-graphe plein X—{i} est somme de 3 chaînes X₁, X₂, X₃ dont chacune a un sommet terminal lié à i dans X. Soient {i₁, i₂}, {i₂, i₃}, ..., {iₚ₋₁, iₚ} les arêtes de X₁, {j₁, j₂}, ..., {jₖ₋₁, jₖ} celles de X₂, {k₁, k₂}, ..., {kᵣ₋₁, kᵣ} celles de X₃, avec i, j₁, k₁ liés à i dans X. On peut supposer $p \geq q \geq r \geq 1$. Posons

$$
\begin{align*}
x &= e_{i_p} + 2e_{i_{p-1}} + \cdots + pe_{i_1} \\
y &= e_{j_q} + 2e_{j_{q-1}} + \cdots + qe_{j_1} \\
z &= e_{k_r} + 2e_{k_{r-1}} + \cdots + re_{k_1}.
\end{align*}
$$

(*) Les racines 5-èmes de 1 distinctes de 1 sont solutions de $z^4 + z^3 + z^2 + z + 1 = 0$. Posant $x = \frac{1}{2} (z + \frac{1}{z})$, cette équation devient $(2x)^2 - 2 + 2x + 1 = 0$, ou $4x^2 + 2x - 1 = 0$, ou

$$
x = \frac{-1 \pm \sqrt{5}}{4}.
$$

D’où

$$
2 \cos^2 \frac{\pi}{5} - 1 = \cos \frac{2\pi}{5} = \frac{\sqrt{5}-1}{4}, \quad \cos^2 \frac{\pi}{5} = \frac{3+\sqrt{5}}{8} > \frac{5}{8} > \frac{9}{16}, \quad \cos \frac{\pi}{5} = \frac{1+\sqrt{5}}{4}.
$$

Comme toutes les arêtes de X sont d’ordre 3 (lemme 7), le lemme 8 donne $\|x\|^2 = \frac{1}{2} p(p+1)$, $\|y\|^2 = \frac{1}{2} q(q+1)$, $\|z\|^2 = \frac{1}{2} r(r+1)$. D’autre part, $e_i$ est orthogonal à $e_{i_1}, e_{i_2}, \ldots, e_{i_p}$, d’où $(e_i|x) = p(e_i|e_{i_1}) = -\frac{1}{2} p$; de même, $(e_i|y) = -\frac{1}{2} q$, $(e_i|z) = -\frac{1}{2} r$. Les vecteurs $\|x\|^{-1} x, \|y\|^{-1} y, \|z\|^{-1} z$ sont unitaires et deux à deux orthogonaux, et $e_i$ n’appartient pas au sous-espace F qu’ils engendrent; le carré de la distance de $e_i$ à F est

$$
1 - (e_i \Big| \frac{x}{\|x\|})^2 - (e_i \Big| \frac{y}{\|y\|})^2 - (e_i \Big| \frac{z}{\|z\|})^2
$$
$$
= 1 - \frac{1}{2} \frac{p}{p+1} - \frac{1}{2} \frac{q}{q+1} - \frac{1}{2} \frac{r}{r+1}
$$
$$
= 1 - \frac{1}{2} + \frac{1}{2} \frac{1}{p+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{q+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{r+1}.
$$

Exprimant que cette quantité est > 0, il vient

(4)
$$(p+1)^{-1} + (q+1)^{-1} + (r+1)^{-1} > 1.$$

Donc $3(r+1)^{-1} > 1$, d’où $r < 2$ et finalement $r = 1$. Alors (4) donne

(5)
$$(p+1)^{-1} + (q+1)^{-1} > \frac{1}{2}$$

donc $2(q+1)^{-1} > \frac{1}{2}$, d’où $q \leqslant 2$. Enfin, si $q = 2$, (5) donne

$$(p+1)^{-1} > \frac{1}{6}, \quad \text{d’où } p \leqslant 4.$$

#### Théorème 1 {#lie-vi-s4-thm-1 .statement}

Si (W, S) est un système de Coxeter fini irréductible, son graphe de Coxeter est isomorphe à l’un des suivants :

A_l \hspace{1cm} (l \geqslant 1 \text{ sommets})
B_l \hspace{1cm} (l \geqslant 2 \text{ sommets})
D_l \hspace{1cm} (l \geqslant 4 \text{ sommets})
E_6
E_7
E_8

F₄   o———o———o
G₂   o———o———o
H₃   o———o———o
H₄   o———o———o
I₂(p)   o———p———o (p = 5 ou p ≥ 7).

Ces graphes de Coxeter sont deux à deux non isomorphes.

En effet, soit $M = (m_{ij})$ la matrice de Coxeter de (W, S), et soit $l = \mathrm{Card}(S)$. Si l’un des $m_{ij}$ est $\geqslant 6$, on a $l = 2$ (lemme 4) et le graphe de Coxeter de (W, S) est de type G₂ ou I₂(p) avec $p \geqslant 7$. Supposons maintenant tous les $m_{ij} \leqslant 5$.

a) Si les $m_{ij}$ ne sont pas tous égaux à 3, le graphe X de (W, S) est une chaîne et un seul des $m_{ij}$ est égal à 4 ou 5 (lemme 7). Si l’un des $m_{ij}$ est égal à 5, le lemme 9 montre que l’on a l’un des types H₃, H₄ ou I₂(5). Si l’un des $m_{ij}$ est égal à 4, le lemme 9 montre que l’on a l’un des types Bₗ, F₄.

b) Supposons tous les $m_{ij}$ égaux à 3. Si X est une chaîne, le graphe de Coxeter est de type Aₗ. Sinon, le lemme 10 montre qu’il est de type E₆, E₇, E₈ ou Dₗ.

Le fait que les graphes de Coxeter énumérés soient deux à deux non isomorphes est évident.

Réciproquement :

#### Théorème 2 {#lie-vi-s4-thm-2 .statement}

Les groupes de Coxeter définis par les graphes de Coxeter Aₗ, Bₗ, ..., I₂(p) du th. 1 sont finis.

C’est clair pour I₂(p), le groupe correspondant étant le groupe diédral d’ordre $2p$ (chap. IV, § 1, no 9).

Pour H₄ la forme quadratique correspondante est

$$
\xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - 2 (\cos \frac{\pi}{5}) \xi_3 \xi_4
$$

$$
= \xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - \frac{1 + \sqrt{5}}{2} \xi_3 \xi_4
$$

$$
= (\xi_2 - \frac{\xi_1 + \xi_3}{2})^2 + (\xi_4 - \frac{1 + \sqrt{5}}{4} \xi_3)^2 + \frac{3}{4} (\xi_1 - \frac{1}{3} \xi_3)^2 + \frac{7 - 3 \sqrt{5}}{24} \xi_3^2.
$$

Comme $7 - 3 \sqrt{5}$ est $> 0$, cette forme est positive non dégénérée, et le groupe de Coxeter correspondant est fini. Il en est de même de celui correspondant à H₃, puisqu’il est isomorphe à un sous-groupe du précédent (chap. IV, § 1, no 8).

Pour les types Aₗ, Bₗ, ..., G₂, nous construirons, dans les nos 5 à 13, des systèmes de racines ayant les groupes correspondants comme groupes de Weyl. On verra ainsi que ces groupes sont, non seulement finis, mais cristallographiques (§ 2, no 5).

### 2. Graphes de Dynkin

Par abus de langage, nous appellerons graphe normé un couple $(\Gamma, f)$ ayant les propriétés suivantes :

1) $\Gamma$ est un graphe (dit sous-jacent à $(\Gamma, f)$).

2) Si $E$ désigne l’ensemble des couples $(i, j)$ tels que $\{i, j\}$ soit une arête de $\Gamma$, $f$ est une application de $E$ dans $\mathbf{R}$ telle que $f(i, j)f(j, i) = 1$ quel que soit $(i, j) \in E$.

On a une notion évidente d’isomorphisme de graphes normés.

Soit $R$ un système de racines réduit dans un espace vectoriel réel $V$. Nous allons lui associer un graphe normé $(X, f)$, appelé graphe de Dynkin de $R$. Les sommets de $X$ seront les éléments de l’ensemble $I$ des orbites de $W(R)$ dans la réunion des ensembles $\{B\} \times B$ (pour $B$ décrivant l’ensemble des bases de $R$). Si $N = (n_{ij})_{i,j \in I}$ (resp. $M = (m_{ij})_{i,j \in I}$) est la matrice de Cartan (resp. la matrice de Coxeter) canonique de $R$ ($§ 1$, no 5, Remarque 7), deux sommets $i$ et $j$ de $X$ seront liés si et seulement si $n_{ij} \neq 0$ et on pose alors :

$$
f(i, j) = \frac{n_{ij}}{n_{ji}}
$$

Comme $n_{ij} = 0$ entraîne $n_{ji} = 0$, on a bien défini ainsi un graphe normé $(X, f)$.

Soient $(x|y)$ un produit scalaire sur $V$, invariant par $W(R)$, et $B = (\alpha_i)_{i \in I}$ une base de $R$, indexée canoniquement. Les formules (7) et (9) du § 1, no 1 montrent que les sommets $i$ et $j$ du graphe $X$ sont liés si et seulement si

$$
(\alpha_i|\alpha_j) \neq 0
$$

et on a alors :

$$
f'(i, j) = \frac{(\alpha_i|\alpha_i)}{(\alpha_j|\alpha_j)}
$$

Compte tenu des résultats du § 1, no 3 et 5, les seules possibilités sont les suivantes, à l’échange près de $i$ et $j$ :

1) $i$ et $j$ ne sont pas liés; $n_{ij} = n_{ji} = 0$; $m_{ij} = 2$;
2) $f(i, j) = f(j, i) = 1$; $n_{ij} = n_{ji} = -1$; $m_{ij} = 3$;
3) $f(i, j) = 2$, $f(j, i) = 1/2$; $n_{ij} = -2$; $n_{ji} = -1$; $m_{ij} = 4$;
4) $f(i, j) = 3$, $f(j, i) = 1/3$; $n_{ij} = -3$; $n_{ji} = -1$; $m_{ij} = 6$.

On voit donc que la connaissance du graphe de Dynkin de $R$ détermine la matrice de Cartan et la matrice de Coxeter de R et par suite détermine R à isomorphisme près. Plus précisément, le cor. de la prop. 15 du § 1, n° 5 entraîne le résultat suivant :

#### Proposition 1 {#lie-vi-s4-prop-1 .statement}

*Soient $R_1$ et $R_2$ deux systèmes de racines réduits dans des espaces vectoriels réels $V_1$ et $V_2$. Soient $B_1 = (\alpha_i)_{i \in I_1}$ et $B_2 = (\alpha_i)_{i \in I_1}$ des bases de $R_1$ et $R_2$, indexées canoniquement. Soit $\lambda$ un isomorphisme du graphe de Dynkin de $R_1$ sur le graphe de Dynkin de $R_2$. Il existe alors un unique isomorphisme de $V_1$ sur $V_2$ transformant $R_1$ en $R_2$ et transformant $\alpha_i$ en $\alpha_{\lambda(i)}$ pour tout $i \in I_1$.

Il est clair qu’un automorphisme de R définit un automorphisme du graphe de Dynkin de R, d’où un homomorphisme $\varphi$ du groupe $A(R)$ dans le groupe des automorphismes du graphe de Dynkin de R.

#### Corollaire {#lie-vi-s4-n2-cor-1 .statement}

*L’homomorphisme $\varphi$ défini par passage au quotient un isomorphisme du groupe $A(R)/W(R)$ sur le groupe des automorphismes du graphe de Dynkin de R.*

On a évidemment $\varphi(g) = \mathrm{Id}$ pour tout $g \in W(R)$. D’autre part, la prop. 1 montre qu’il existe un isomorphisme $\psi$ du groupe des automorphismes du graphe de Dynkin de R sur le sous-groupe E des éléments de $A(R)$ laissant fixe une base donnée B de R, tel que $\varphi \circ \psi = \mathrm{Id}$. Comme $A(R)$ est le produit semi-direct de E et de $W(R)$ (§ 1, n° 5, prop. 16), le corollaire en résulte.

Dans la pratique, on représente le graphe de Dynkin $(X, f)$ par un dessin composé de points et de traits de la manière suivante. Les points correspondent aux sommets de X ; deux points correspondant à deux sommets distincts i et j sont liés par 0, 1, 2 ou 3 traits suivants que l’on est dans le cas 1), 2), 3) ou 4) ci-dessus (à l’échange près de i et j). De plus, dans les cas 3) et 4), c’est-à-dire lorsque $f(i, j) > 1$ ou encore lorsque les racines $\alpha_i$ et $\alpha_j$ ne sont pas orthogonales et ne sont pas de même longueur, on place sur les deux ou trois traits joignant les points correspondant à i et j un signe d’inégalité $>$ orienté vers le point correspondant à j (c’est-à-dire à la racine de plus petite longueur) :

$$
\begin{array}{cc}
\circ \Longrightarrow \circ & \text{(pour } f(i, j) = 2 \text{)}, \\
\circ \Rrightarrow \circ & \text{(pour } f(i, j) = 3 \text{)}.
\end{array}
$$

Il est clair que la donnée de ce dessin permet de reconstituer le graphe de Dynkin $(X, f)$.

On remarquera que la figure associée au graphe de Coxeter de $W(R)$ s’obtient à partir de la figure ainsi associée au graphe de Dynkin de R en conservant les points et les traits simples et en remplaçant les doubles traits (resp. triples traits) par un trait surmonté du nombre 4 (resp. 6). Inversement, si l’on connaît le graphe de Coxeter de $W(R)$, l’opération inverse permet de reconstituer la figure associée au graphe de Dynkin de R, à l’exception des signes d’inégalité surmontant les doubles et triples traits. On déduit alors immédiatement du th. 1 la liste des graphes de Dynkin possibles. Plus précisément :

#### Théorème 3 {#lie-vi-s4-thm-3 .statement}

Si R est un système de racines réduit et irréductible, son graphe de Dynkin est isomorphe à l’un des graphes représentés par les figures suivantes :

A_l   o———o———o……o———o   (l \geqslant 1 sommets)
B_l   o———o———o……o———o———o   (l \geqslant 2 sommets)
C_l   o———o———o……o———o———o   (l \geqslant 3 sommets)
D_l   o———o———o……o———o———o———o   (l \geqslant 4 sommets)
E_6   o———o———o———o
E_7   o———o———o———o———o
E_8   o———o———o———o———o———o———o
F_4   o———o———o———o
G_2   o———o———o

Ces graphes de Dynkin sont deux à deux non isomorphes et, pour chacun d’eux, il existe un système de racines irréductible et réduit l’admettant (à un isomorphisme près) comme graphe de Dynkin.

La première assertion résulte aussitôt du th. 1, compte tenu des remarques qui précèdent, du fait que les groupes de Coxeter de graphe H_3, H_4 et I_2(p) (pour p = 5 ou p \geqslant 7) ne sont pas cristallographiques, et de ce que les deux inégalités possibles pour le double (resp. triple) trait du graphe de Dynkin associé au graphe de Coxeter F_4 (resp. G_2) donnent des graphes de Dynkin isomorphes. La deuxième assertion est évidente et la troisième résultera de la construction explicite d’un système de racines réduit et irréductible pour chacun des types, construction qui va être effectuée dans les n°s 5 à 13.

#### Remarque 1 {#lie-vi-s4-n2-rem-1 .statement}

Le graphe A_1 est réduit à un seul sommet; on le note aussi B_1 ou C_1. Le graphe B_2———o est aussi noté C_2. Le graphe A_3———o———o est aussi noté D_3. Enfin, on note D_2 le graphe composé de deux sommets non liés. (Ces conventions proviennent des propriétés des systèmes de racines correspondants, cf. n°s 5 à 8.)

#### Remarque 2 {#lie-vi-s4-n2-rem-2 .statement}

Si (X, f) est le graphe de Dynkin d’un système de racines réduit R, le graphe de Dynkin du système inverse s’identifie à (X, f^{-1}). Autrement dit, la figure associée au graphe de Dynkin de R^\vee s’obtient à partir de celle associée au graphe de Dynkin de R en renversant les signes d’inégalité. Si R est irréductible, on voit que R est isomorphe à R^\vee, sauf si R est de type B_l ou C_l, auquel cas R^\vee est de type C_l ou B_l.

### 3. Groupe de Weyl affine et graphe de Dynkin complété

Soit R un système de racines réduit et irréductible et soit $(X, f)$ son graphe de Dynkin. Nous allons définir un autre graphe normé $(\tilde{X}, \tilde{f})$ que nous appellerons le *graphe de Dynkin complété* de R. L’ensemble $\tilde{I}$ des sommets de $\tilde{X}$ se compose de l’ensemble I des sommets de X et d’un sommet noté 0, n’appartenant pas à I. Pour définir $\tilde{f}$, choisissons une base $B = (\alpha_i)_{i \in I}$ de R et un produit scalaire $(x|y)$ invariant par $W(R)$. Soit $\alpha_0$ l’*opposée de la plus grande racine* pour l’ordre défini par B. Deux sommets distincts, $i, j \in \tilde{I}$ sont liés si et seulement si $(\alpha_i|\alpha_j) \neq 0$ et on pose alors

$$
\tilde{f}(i, j) = \frac{(\alpha_i|\alpha_i)}{(\alpha_j|\alpha_j)}.
$$

On vérifie aussitôt que le graphe $\tilde{X}$ et l’application $\tilde{f}$ ainsi définis ne dépendent pas du choix de B ni du produit scalaire.

Si le rang $l$ de R est égal à 1, on a $I = \{i\}$ et $\alpha_0 = -\alpha_i$; d’où $\tilde{f}(0, i) = 1$. Si $l \geq 2$, $\alpha_0$ n’est proportionnelle à aucune des $\alpha_i$ et $(\alpha_0|\alpha_i)$ est $\leq 0$ (\S 1, no 8, prop. 25). Pour tout couple $(i, j)$ d’éléments distincts de $\tilde{I}$, les seules possibilités sont celles notées 1), 2), 3), 4) au numéro précédent (en posant par exemple $n_{0i} = n(\alpha_0, \alpha_i)$ et $m_{0i} =$ ordre de $s_{\alpha_0}s_{\alpha_i}$ pour tout $i \in I$).

Dans le cas $l \geq 2$, on représente le graphe de Dynkin complété par une figure avec les mêmes conventions qu’au numéro précédent, on indique parfois en pointillé les traits joignent le sommet 0 aux autres sommets. Remarquons que le signe d’inégalité $>$ placé sur un tel trait, s’il existe, est toujours dirigé vers le sommet distinct de 0, puisque $\alpha_0$ est une racine de la plus grande longueur possible (\S 1, no 8, prop. 25). On identifie $(X, f)$ au sous-graphe de $(\tilde{X}, \tilde{f})$ obtenu en supprimant le sommet 0.

L’action de $A(R)$ sur $(X, f)$ se prolonge en une action sur $(\tilde{X}, \tilde{f})$, laissant 0 fixe, et $W(R)$ opère trivialement sur $(\tilde{X}, \tilde{f})$.

Reprenons les notations du \S 2. La prop. 5 du \S 2, no 2, jointe au th. 1 du chap. V, \S 3, no 2, montre que le graphe de Coxeter $\Sigma$ du groupe de Weyl affine $W_a(R)$ se déduit de $(\tilde{X}, \tilde{f})$ par les mêmes règles que celles permettant de passer de $(X, f)$ au graphe de Coxeter de $W(R)$. D’autre part, soit G le normalisateur de $W_a(R)$ (\S 2, no 3). À tout $g \in G$ correspond un automorphisme $\varphi(g)$ de $\Sigma$ et on a $\varphi(g) = \mathrm{Id}$ si $g \in W_a(R)$. Inversement, à tout automorphisme $\lambda$ de $\Sigma$ correspond, d’après la prop. 11 du chap. V, \S 4, no 9, un élément $g = \psi(\lambda)$ et un seul, conservant une alcôve C donnée et tel que $\varphi(g) = \lambda$. Comme G est produit semi-direct du sous-groupe $G_C$ des éléments conservant C et de $W_a(R)$ (\S 2, no 3), on en déduit que $\varphi$ fournit par passage au quotient un *isomorphisme de* $G/W_a$ (ou de $G_C$) *sur* $\mathrm{Aut}(\Sigma)$. On vérifie aussitôt que le composé de cet isomorphisme avec l’application canonique de $A(R)/W(R)$ dans $G/W_a$ coïncide avec l’homomorphisme de $A(R)/W(R)$ dans $\mathrm{Aut}(\Sigma)$ déduit de l’homomorphisme de $A(R)/W(R)$ dans $\mathrm{Aut}(\tilde{X}, \tilde{f})$ défini plus haut. D’après le § 2, n° 3, le groupe $\mathrm{Aut}(\Sigma)$ est isomorphe au produit semi-direct de $A(R)/W(R)$ par $P(R^\vee)/Q(R^\vee)$, et $P(R^\vee)/Q(R^\vee)$ est isomorphe au groupe $\Gamma_C = G_C \cap W'_a$ (avec les notations du § 2, n° 3); l’élément de $\mathrm{Aut}(\Sigma)$ correspondant à l’élément $\gamma_i$ de $\Gamma_C$ transforme le sommet 0 en le sommet $i$ de $\Sigma$.

#### Remarque {#lie-vi-s4-n3-rem-1 .statement}

On peut montrer que l’application canonique
$$
\mathrm{Aut}(\tilde{X}, \tilde{f}) \to \mathrm{Aut}(\Sigma)
$$
est un isomorphisme.

#### Théorème 4 {#lie-vi-s4-thm-4 .statement}

Soit $(W, S)$ un système de Coxeter irréductible, avec $S$ fini. Pour que la forme quadratique associée (chap. V, § 4, n° 1) soit positive et dégénérée, il faut et il suffit que le graphe de Coxeter de $(W, S)$ soit isomorphe à l’un des suivants :

$$
\begin{array}{ll}
\tilde{A}_1 & \\
\tilde{A}_l \quad (l \geq 2) & \text{(circuit à } l + 1 \text{ sommets)} \\
\tilde{B}_2 & \\
\tilde{B}_l \quad (l \geq 3) & (l + 1 \text{ sommets}) \\
\tilde{C}_l \quad (l \geq 3) & (l + 1 \text{ sommets}) \\
\tilde{D}_l \quad (l \geq 4) & (l + 1 \text{ sommets}) \\
\tilde{E}_6 & \\
\tilde{E}_7 & \\
\tilde{E}_8 & \\
\tilde{F}_4 & \\
\tilde{G}_2 &
\end{array}
$$

Ces graphes de Coxeter sont deux à deux non isomorphes.

D’après le chap. V, § 4, n° 9 et la prop. 8 du § 2, n° 5, les systèmes de Coxeter dont la forme quadratique est positive et dégénérée sont ceux qui correspondent aux groupes de Weyl affines des systèmes de racines réduits et irréductibles. Le théorème résulte alors de la détermination des graphes de Dynkin complétés faite dans les n°s 5 à 13 ci-après.

### 4. Préliminaires à la construction des systèmes de racines

Soient V un espace vectoriel réel de dimension $l \geqslant 1$ muni d’un produit scalaire $(x|y)$, L un sous-groupe discret de V, $\Lambda$ un ensemble fini de nombres $> 0$, et R l’ensemble des $\alpha \in L$ tels que $(\alpha|\alpha) \in \Lambda$. Supposons que R engendre V et que, pour tout couple $(\alpha, \beta)$ de points de R, le nombre $2 \frac{(\alpha|\beta)}{(\alpha|\alpha)}$ soit entier. Alors, R est un système de racines dans V. En effet, R vérifie évidemment (SR_I). Soit $\alpha \in R$; soit $s_\alpha$ la réflexion orthogonale $x \longmapsto x - 2 \frac{(x|\alpha)}{(\alpha|\alpha)} \alpha$; alors, si $\beta \in R$, on a $2 \frac{(\beta|\alpha)}{(\alpha|\alpha)} \in \mathbf{Z}$, donc $s_\alpha(\beta) \in L$, et par ailleurs $\|s_\alpha(\beta)\| = \|\beta\|$, donc $s_\alpha(\beta) \in R$; donc R vérifie (SR_{II}) et (SR_{III}), et est réduit si $\Lambda$ ne contient pas deux nombres de la forme $\lambda$ et $4\lambda$.

Nous prendrons pour V un sous-espace de $E = \mathbf{R}^n$. Soit $(\varepsilon_1, \ldots, \varepsilon_n)$ la base canonique de E; on munit E du produit scalaire $(x|y)$ pour lequel cette base est orthonormale et on identifie $E^*$ à E (resp. $V^*$ à V) au moyen de ce produit scalaire. Définissons dans E les sous-groupes $L_0, L_1, L_2, L_3$ comme suit :

1) $L_0$ est le $\mathbf{Z}$-module de base $(\varepsilon_i)$. On a $(\alpha|\beta) \in \mathbf{Z}$ pour $\alpha, \beta \in L_0$. Les vecteurs $\alpha \in L_0$ pour lesquels $(\alpha|\alpha) = 1$ sont les $\pm \varepsilon_i$ ($1 \leq i \leq n$); ceux pour lesquels $(\alpha|\alpha) = 2$ sont les $\pm \varepsilon_i \pm \varepsilon_j$ pour $i < j$ (les deux signes $\pm$, dans $\pm \varepsilon_i \pm \varepsilon_j$, sont choisis indépendamment l’un de l’autre; on adopte une convention analogue dans toute la fin de ce paragraphe).

2) $L_1$ est le sous-$\mathbf{Z}$-module de $L_0$ formé des $x = \sum_{i=1}^n \xi_i \varepsilon_i \in L_0$ tels que $\sum_{i=1}^n \xi_i$ soit pair; comme $\xi_i$ et $\xi_i^2$ ont même parité, il revient au même de dire que $(x|x)$ est pair. Soit $L_1'$ le sous-module de $L_1$ engendré par les $\varepsilon_i \pm \varepsilon_j$; on a $\sum_{i=1}^n \xi_i \varepsilon_i \equiv (\sum_{i=1}^n \xi_i) \varepsilon_n$ (mod. $L_1'$), et comme $2\varepsilon_n = (\varepsilon_1 + \varepsilon_n) - (\varepsilon_1 - \varepsilon_n) \in L_1'$, on voit que $L_1' = L_1$. Comme $L_0$ est engendré par $L_1$ et $\varepsilon_1$, $L_0/L_1$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$.

3) $L_2 = L_0 + \mathbf{Z}(\frac{1}{2} \sum_{i=1}^n \varepsilon_i)$. Il est clair qu’un élément $x = \sum_{i=1}^n \xi_i \varepsilon_i$ de V est dans $L_2$ si et seulement si

$$
2\xi_i \in \mathbf{Z}, \quad \xi_i - \xi_j \in \mathbf{Z} \quad \text{quels que soient } i \text{ et } j.
$$

Comme $(\varepsilon_k \left| \frac{1}{2} \sum_{i=1}^n \varepsilon_i \right|) = \frac{1}{2}$ pour tout $k$, et que $\left| \frac{1}{2} \sum_{i=1}^n \varepsilon_i \right|^2 = \frac{n}{4}$, on a $(\alpha|\beta) \in \frac{1}{2}\mathbf{Z}$ pour $\alpha, \beta \in L_2$ si $n$ est pair. Le groupe $L_2/L_0$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$.

4) $L_3 = L_1 + \mathbf{Z}(\frac{1}{2}\sum_{i=1}^n \varepsilon_i)$. Si $n$ est un multiple de 4, $L_3$ est l’ensemble des $\sum_{i=1}^n \xi_i \varepsilon_i$ qui vérifient (6) et en outre la condition $\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$; dans ce cas, on a $(\alpha|\beta) \in \mathbf{Z}$ quels que soient $\alpha, \beta \in L_3$.

Il est immédiat que le sous-groupe de E associé à $L_0$ (resp. $L_1, L_2$) est $L_0$ (resp. $L_2, L_1$). Le sous-groupe de E associé à $L_3$ est l’ensemble des

$$
x = \sum_{i=1}^n \xi_i \varepsilon_i \in L_2
$$

tels que $(x|\frac{1}{2}\sum_{i=1}^n \varepsilon_i) \in \mathbf{Z}$, c’est-à-dire tels que $\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$; si $n \equiv 0 \pmod{4}$, ce sous-groupe associé est donc $L_3$.

Le groupe commutatif $L_2/L_1$ est d’ordre 4, donc isomorphe à $\mathbf{Z}/4\mathbf{Z}$ ou à $(\mathbf{Z}/2\mathbf{Z}) \times (\mathbf{Z}/2\mathbf{Z})$ (Alg., chap. VII, § 4, n° 6, th. 3). Si $n$ est impair, on a

$$
p(\frac{1}{2}\sum_{i=1}^n \varepsilon_i) \in L_1 \iff p \equiv 0 \pmod{4}
$$

donc $L_2/L_1$ est cyclique d’ordre 4. Si $n$ est pair, on a

$$
p(\frac{1}{2}\sum_{i=1}^n \varepsilon_i) \in L_1 \iff p \equiv 0 \pmod{2}
$$

donc $L_2/L_1$, qui contient deux éléments distincts d’ordre 2, est isomorphe à $(\mathbf{Z}/2\mathbf{Z}) \times (\mathbf{Z}/2\mathbf{Z})$.

Nous utiliserons ces notations dans les neuf n°s suivants et dans les planches. Pour chaque type de graphe de Dynkin du th. 3, nous expliciterons :

(I) Un système de racines R et le nombre de racines.
(II) Une base B de $\dot{R}$, et les racines positives correspondantes.
La base B sera indexée par les entiers $1, \ldots, l$.
(III) Le nombre de Coxeter $h$ (§ 1, n° 11).
(IV) La plus grande racine $\tilde{\alpha}$ (pour l’ordre défini par B) et le graphe de Dynkin complété (n° 3). Nous indiquerons à côté de chaque sommet la racine correspondante de B.
(V) Le système inverse $R^\vee$, la forme bilinéaire canonique et la constante $\gamma(R)$ (§ 1, n° 12).
(VI) Les poids fondamentaux relativement à B (§ 1, n° 10).
(VII) La somme des racines positives.
(VIII) Les groupes P(R), Q(R), P(R)/Q(R) et l’indice de connexion (§ 1, n° 9).

(IX) Les exposants de $W(R)$ (chap. V, § 6, n° 2, déf. 2). Dans les cas $A_l, B_l, C_l$ et $D_l$ nous déterminerons les invariants symétriques.
(X) L’ordre de $W(R)$ (et éventuellement sa structure).
(XI) le groupe $A(R)/W(R)$, son action sur le graphe de Dynkin, et l’élément $w_0$ de $W(R)$ qui transforme $B$ en $-B$.
(XII) L’action de $P(R^\vee)/Q(R^\vee)$ sur le graphe de Dynkin complété et l’action de $A(R)/W(R)$ sur $P(R^\vee)/Q(R^\vee)$.
Pour chaque graphe de Dynkin du th. 3, ces données seront rassemblées dans les planches I à IX, en les ordonnant de façon uniforme comme ci-dessus. On y ajoute :
(XIII) La matrice de Cartan, qui se déduit du graphe de Dynkin comme on l’a expliqué au n° 2.

### 5. Systèmes de type $B_l$ ($l \geqslant 2$)

(I) Considérons dans $V = \mathbf{R}^l$ le groupe $L_0$ (n° 4). Soit $R$ l’ensemble des $\alpha \in L_0$ tels que $(\alpha|\alpha) = 1$ ou $(\alpha|\alpha) = 2$, c’est-à-dire l’ensemble des vecteurs $\pm \varepsilon_i$ ($1 \leqslant i \leqslant l$) et $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leqslant i < j \leqslant l$). Il est clair que $R$ engendre $V$ et que $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$ quels que soient $\alpha, \beta \in R$. Donc $R$ est un système de racines réduit dans $V$ (n° 4). Le nombre de racines est $n = 2l + 4 \frac{l(l-1)}{2} = 2l^2$.

(II) Posons

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \quad \alpha_2 = \varepsilon_2 - \varepsilon_3, \ldots, \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \quad \alpha_l = \varepsilon_l.
$$

On a alors

$$
\begin{align*}
\varepsilon_i &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_l & (1 \leqslant i \leqslant l) \\
\varepsilon_i + \varepsilon_j &= (\alpha_i + \alpha_{i+1} + \cdots + \alpha_l) + (\alpha_j + \alpha_{j+1} + \cdots + \alpha_l) & (1 \leqslant i < j \leqslant l). \\
\varepsilon_i - \varepsilon_j &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} & (1 \leqslant i < j \leqslant l).
\end{align*}
$$

Donc $(\alpha_1, \alpha_2, \ldots, \alpha_l)$ est une base de $R$ ($\S 1$, n° 7, cor. 3 de la prop. 20). En outre, on a $\|\alpha_i\|^2 = 2$ pour $i < l$, $\|\alpha_l\|^2 = 1$, $(\alpha_i|\alpha_{i+1}) = -1$ pour $1 \leqslant i \leqslant l-1$, $(\alpha_i|\alpha_j) = 0$ pour $j > i + 1$; le graphe de Dynkin de $R$ est donc de type $B_l$, ce qui montre que $R$ est irréductible. Les racines positives sont les $\varepsilon_i$ et les $\varepsilon_i \pm \varepsilon_j$ ($i < j$).

(III) D’après le th. 1 (ii) du chap. V, § 6, n° 2, on a

$$
h = n/l = 2l.
$$

(IV) Soit $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + 2\alpha_3 + \cdots + 2\alpha_l$, qui est une racine. La somme de ses coordonnées relativement à la base $(\alpha_i)$ est $2l - 1 = h - 1$. Compte tenu de la prop. 31 du § 1, n° 11, $\tilde{\alpha}$ est la plus grande racine de $R$. On a $(\tilde{\alpha}|\alpha_i) = 0$ pour $i \neq 2$ et $(\tilde{\alpha}|\alpha_2) = 1$. Comme $\alpha_2$ est de longueur 1 (resp. $\sqrt{2}$) quand $l = 2$ (resp. $l \geqslant 3$), on en déduit le graphe de Dynkin complété de $R$:

pour $l = 2$

pour $l \geqslant 3$

(V) La formule $\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)}$ donne pour $R^\vee$ l’ensemble des vecteurs $\pm 2\varepsilon_i$ ($1 \leqslant i \leqslant l$), $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leqslant i < j \leqslant l$). Le graphe de Dynkin de $R^\vee$ se déduit de celui de $R$ par le procédé expliqué au no 2, et l’on voit que $R^\vee$ est du type $C_l$.

Les racines non orthogonales à $\beta = \varepsilon_1$ sont $\pm \varepsilon_1$ et $\pm \varepsilon_1 \pm \varepsilon_j$ pour $2 \leqslant j \leqslant l$, donc sont au nombre de $4l - 2$; pour chacune de ces racines $\alpha$, on a $n(\alpha, \beta) = \pm 2$. La formule (17) du § 1, no 12 montre que, pour $\Phi_R$, le carré de la longueur de $\beta$ est $(4l - 2)^{-1}$; donc $\Phi_R(x, y) = (x|y)/(4l - 2)$. Appliquons la formule (18) du § 1, no 12 avec $x = y = \beta$. Il vient

$$
2 + \frac{1}{4}(4l - 4) = \gamma(R) \frac{1}{4l - 2}
$$

d’où $\gamma(R) = (l + 1)(4l - 2)$.

(VI) On calcule aisément les poids fondamentaux $\varpi_i$ ($1 \leqslant i \leqslant l$) tels que $(\varpi_i|\alpha_j^\vee) = \delta_{ij}$, et l’on trouve

$$
\begin{align*}
\varpi_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i - 1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_l) \quad (i < l) \\
\varpi_l &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l) = \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + l\alpha_l).
\end{align*}
$$

(VII) La somme des racines positives est

$$
\begin{align*}
2\rho &= (2l - 1)\varepsilon_1 + (2l - 3)\varepsilon_2 + \cdots + 3\varepsilon_{l-1} + \varepsilon_l \\
&= (2l - 1)\alpha_1 + 2(2l - 2)\alpha_2 + \cdots + i(2l - i)\alpha_i + \cdots + l^2\alpha_l.
\end{align*}
$$

(VIII) On a $Q(R) = L_0$ (no 4), et $P(R)$ est engendré par $Q(R)$ et $\varpi_l$, donc est égal à $L_2$ (no 4). Donc $P(R)/Q(R)$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$, et l’indice de connexion est égal à 2.

(IX) et (X) Dans $R^l$, la réflexion orthogonale $s_{\varepsilon_i - \varepsilon_j}$ ($i \neq j$) échange $\varepsilon_i$ et $\varepsilon_j$ et laisse invariants les $\varepsilon_k$ d’indice $k$ distinct de $i$ et $j$. Les $s_{\varepsilon_i - \varepsilon_j}$ engendrent un groupe $G_1$ isomorphe au groupe symétrique $S_l$. La réflexion orthogonale $s_{\varepsilon_i}$ transforme $\varepsilon_i$ en $-\varepsilon_i$ et laisse invariants les $\varepsilon_k$ d’indice $k$ distinct de $i$. Les $s_{\varepsilon_i}$ engendrent un groupe $G_2$ isomorphe à $(\mathbf{Z}/2\mathbf{Z})^l$. Le groupe de Weyl $W(R)$ est engendré par $G_1$ et $G_2$, et $G_2$ est distingué dans $W(R)$, donc $W(R)$ est isomorphe à un produit semi-direct de $\mathfrak{S}_l$ par $(\mathbf{Z}/2\mathbf{Z})^l$. Son ordre est par suite $2^l.l!$

L’algèbre symétrique $S(\mathbf{R}^l)$ s’identifie canoniquement à l’algèbre des fonctions polynômes $P(\xi_1, \ldots, \xi_l)$ sur $\mathbf{R}^l$. Pour qu’un tel polynôme soit invariant par $W(\mathbf{R})$, il faut d’abord que

$$
P(\xi_1, \xi_2, \ldots, \xi_l) = P(\pm \xi_1, \pm \xi_2, \ldots, \pm \xi_l)
$$

quels que soient les $l$ signes du second membre, c’est-à-dire que

$$
P(\xi_1, \ldots, \xi_l) = Q(\xi_1^2, \ldots, \xi_l^2)
$$

où $Q$ est un polynôme; il faut ensuite que $Q$ soit une fonction polynôme symétrique; et ces conditions sont suffisantes. Par suite (*Alg.*, chap. V, App. I), $S(\mathbf{R}^l)^{W(\mathbf{R})}$ est l’algèbre engendrée par les $l$ fonctions polynômes

$$
t_i = \sum_{\tau \in \mathfrak{S}_l} \xi_{\tau(1)}^2 \xi_{\tau(2)}^2 \ldots \xi_{\tau(l)}^2 \quad (1 \leq i \leq l).
$$

Par ailleurs, le degré de transcendance sur $\mathbf{R}$ du corps des fractions de $S(\mathbf{R}^l)^{W(\mathbf{R})}$ est $l$, donc les $t_i$ sont algébriquement indépendants. Comme les $t_i$ sont de degré 2, 4, \ldots, $2l$, on en conclut que les exposants de $W(\mathbf{R})$ sont (chap. V, § 6, no 2, prop. 3):

$$
1, 3, 5, \ldots, 2l - 1.
$$

(XI) Le seul automorphisme du graphe de Dynkin est l’identité. On a donc $A(\mathbf{R}) = W(\mathbf{R})$ et $-1 \in W(\mathbf{R})$. Comme $-1$ transforme B en $-B$, on en déduit que $w_0 = -1$.

(XII) Le groupe $P(\mathbf{R}^\vee)/Q(\mathbf{R}^\vee)$ est dual de $P(\mathbf{R})/Q(\mathbf{R})$, donc isomorphe à $\mathbf{Z}/2\mathbf{Z}$. Son élément non trivial permutte les sommets correspondants à $\alpha_0$ et $\alpha_1$ et laisse fixés les autres.

### 6. Systèmes de type $C_l$ ($l \geq 2$).

(I) L’existence de systèmes de racines de type $C_l$ a été démontrée au no 5, puisqu’on a vu que le système inverse d’un système de type $B_l$ est de type $C_l$. Un système de racines $R$ de type $C_l$ est donc obtenu en prenant dans $\mathbf{R}^l$ les vecteurs $\pm 2\varepsilon_i$ ($1 \leq i \leq l$), et $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Le nombre de racines est $2l^2$.

(II) On obtient une base de $R$ en prenant l’image, par l’application $\alpha \mapsto \frac{2\alpha}{(\alpha|\alpha)}$, de la base du système considéré au no 5. On obtient:

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \ \alpha_2 = \varepsilon_2 - \varepsilon_3, \ \ldots, \ \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \ \alpha_l = 2\varepsilon_l.
$$

Les racines positives sont les $2\varepsilon_i$ et les $\varepsilon_i \pm \varepsilon_j$ ($i < j$).

(III) Le nombre de Coxeter est le même que pour le système inverse : $h = 2l$.

(IV) Soit $\tilde{\alpha} = 2\varepsilon_1 = 2\alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-1} + \alpha_l$, qui est une racine. La somme de ses coordonnées relativement à $(\alpha_i)$ est $2l - 1 = h - 1$. Donc $\tilde{\alpha}$ est la plus grande racine. On a $(\tilde{\alpha}|\alpha_i) = 0$ pour $i \neq 1$, $(\tilde{\alpha}|\alpha_1) = 2$.

D’où le graphe de Dynkin complété :

(V) On a déjà déterminé $R^\vee$, qui est de type $B_l$. D’après la formule (19) du § 1, no 12, et d’après le no 5 (V), le carré de la longueur de $2\varepsilon_i$ pour $\Phi_R$ est

$$
((l + 1)(4l - 2))^{-1}((4l - 2)^{-1})^{-1} = (l + 1)^{-1};
$$

donc $\Phi_R(x, y) = (x|y)/4(l + 1)$.

On a $\gamma(R) = \gamma(R^\vee) = (l + 1)(4l - 2)$.

(VI) On trouve facilement les poids fondamentaux :

$$
\begin{align*}
\varpi_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i - 1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \frac{1}{2}\alpha_l) \quad (i \leq l).
\end{align*}
$$

(VII) La somme des racines positives est

$$
\begin{align*}
2\rho &= 2l\varepsilon_1 + (2l - 2)\varepsilon_2 + \cdots + 4\varepsilon_{l-1} + 2\varepsilon_l \\
&= 2l\alpha_1 + 2(2l - 1)\alpha_2 + \cdots + i(2l - i + 1)\alpha_i + \cdots \\
&+ (l - 1)(l + 2)\alpha_{l-1} + \frac{1}{2}l(l + 1)\alpha_l.
\end{align*}
$$

(VIII) D’après le no 4, et le no 5 (VIII), on a $Q(R) = L_1, P(R) = L_0; P(R)/Q(R)$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$, et l’indice de connexion est 2.

(IX) et (X) Ces questions ne concernent que $W(R)$, et les résultats sont donc les mêmes que pour le type $B_l$.

(XI) Le même raisonnement qu’au no 6 montre que $A(R) = W(R)$ et $w_0 = -1$.

(XII) Le seul élément non neutre de $P(R^\vee)/Q(R^\vee)$ définit l’unique automorphisme non trivial du graphe de Dynkin complété : il échange les sommets correspondant à $\alpha_j$ et $\alpha_{l-j}$ pour $0 \leq j \leq l$.

### 7. Systèmes de type $A_l$ ($l \geq 1$).

(I) et (II) Dans $E = \mathbf{R}^{l+1}$, soit $V$ l’hyperplan d’équation $\sum_{i=1}^{l+1} \xi_i = 0$. En remplaçant $l$ par $l + 1$ dans le no 5, on obtient un système $R'$ de type $B_{l+1}$ dans $E$, admettant la base

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \ \alpha_2 = \varepsilon_2 - \varepsilon_3, \ \ldots, \ \alpha_l = \varepsilon_l - \varepsilon_{l+1}, \ \alpha_{l+1} = \varepsilon_{l+1}.
$$

Comme $\alpha_1, \ldots, \alpha_l$ engendrent $V$, $R = R' \cap V$ est un système de racines dans

V, de base $(\alpha_1, \ldots, \alpha_l)$ (\S 1, n° 7, cor. 4 de la prop. 20). D’après les calculs de produits scalaires du n° 5, il est immédiat que R est de type $A_l$. Les éléments de R sont les $\varepsilon_i - \varepsilon_j$ ($i \neq j, 1 \leq i \leq l + 1, 1 \leq j \leq l + 1$). Leur nombre est $n = l(l + 1)$. Les racines positives sont les $\varepsilon_i - \varepsilon_j$ où $i < j$.

(III) On a $h = \frac{n}{l} = l + 1$.

(IV) Soit $\tilde{\alpha} = \varepsilon_1 - \varepsilon_{l+1} = \alpha_1 + \alpha_2 + \cdots + \alpha_l$, qui est une racine. La somme de ses coordonnées relativements à $(\alpha_i)$ est $l = h - 1$. Donc $\tilde{\alpha}$ est la plus grande racine.
Pour $l = 1$, on a $\tilde{\alpha} = \alpha_1$, d’où $(\tilde{\alpha}|\alpha_1) = 2$; le graphe de Coxeter du groupe $W_a(R)$ est

$$
\begin{array}{c}
\circ \xrightarrow{\infty} \circ \\
\alpha_1
\end{array}
$$

Pour $l \geq 2$, on a $(\tilde{\alpha}|\alpha_i) = 0$ pour $0 < i < l$ et $(\tilde{\alpha}|\alpha_1) = (\tilde{\alpha}|\alpha_l) = 1$. D’où le graphe de Dynkin complété:

$$
\begin{array}{cccccc}
\circ & \cdots & \circ & \cdots & \circ \\
\alpha_1 & \alpha_2 & \cdots & \alpha_{l-1} & \alpha_l
\end{array}
$$

(V) Identifiant V à son dual grâce au produit scalaire, on a $\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)} = \alpha$ pour tout $\alpha \in R$, donc $R^\vee = R$.
Pour la forme $\Phi_R$, la longueur des racines est $h^{-1/2} = (l + 1)^{-1/2}$ (\S 1, n° 12); donc $\Phi_R(x, y) = (x|y)/2(l + 1)$.
On a $\gamma(R) = (l + 1)^2$ (\S 1, n° 12, formule (20)).
(VI) Soit $(\varpi_i)_{1 \leq i \leq l}$ la famille des poids fondamentaux. Posons

$$
\varpi_i = \sum_{j=1}^{l+1} \xi_{ij} \varepsilon_j, \quad \text{avec } \xi_{ij} \in \mathbf{R}.
$$

Exprimant que $(\varpi_i|\alpha_j^\vee) = \delta_{ij}$, et $\varpi_i \in V$, on a

$$
\xi_{ii} - \xi_{i, i+1} = 1, \quad \xi_{ij} - \xi_{i, j+1} = 0 \quad \text{pour } j \neq i, \quad \sum_{j=1}^{l+1} \xi_{ij} = 0,
$$

ce qui donne aisément

$$
\varpi_i = \varepsilon_1 + \cdots + \varepsilon_i - \frac{i}{l+1} (\varepsilon_1 + \cdots + \varepsilon_{l+1})
$$
$$
= \frac{1}{l+1} ((l-i+1)(\alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1})
$$
$$
\phantom{=} + i((l-i+1)\alpha_i + (l-i)\alpha_{i+1} + \cdots + \alpha_l)).
$$

(VII) La somme des racines positives est

$$
2\rho = l\varepsilon_1 + (l-2)\varepsilon_2 + (l-4)\varepsilon_3 + \cdots - (l-2)\varepsilon_l - l\varepsilon_{l+1}
$$
$$
= l\alpha_1 + 2(l-1)\alpha_2 + \cdots + i(l-i+1)\alpha_i + \cdots + l\alpha_l.
$$

(VIII) Introduisons dans $E = \mathbf{R}^{l+1}$ le sous-groupe $L_0$ du no 4. Soit $p$ le projecteur orthogonal de $E$ sur $V$. D’après le § 1, no 10, prop. 28, on a
$$
Q(R) = Q(R') \cap V = L_0 \cap V, \text{ et } P(R) = p(P(R'));
$$
tenant compte du fait que le dernier poids fondamental de $R'$ est orthogonal à $V$, on a $P(R) = p(Q(R')) = p(L_0)$. Ainsi, $P(R)$ est le groupe engendré par les $\varepsilon_i - \varepsilon_j$ et par $p(\varepsilon_1) = \varepsilon_1 - (l + 1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i$, donc
$$
P(R) = Q(R) + \mathbf{Z}(\varepsilon_1 - (l + 1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i).
$$
Or $l+1$ est le plus petit entier $m > 0$ tel que $mp(\varepsilon_1) \in Q(R)$. Donc $P(R)/Q(R)$ est isomorphe à $\mathbf{Z}/(l + 1)\mathbf{Z}$ et l’indice de connexion est $l + 1$.

(IX) et (X) Pour tout automorphisme $g$ de $V$, soit $\varphi(g)$ l’automorphisme de $E$ qui prolonge $g$ et laisse invariant $\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l$. Si on prend pour $g$ la réflexion orthogonale $s_{\varepsilon_i - \varepsilon_j}|V$, $\varphi(g)$ est égal à $s_{\varepsilon_i - \varepsilon_j}$, donc échange $\varepsilon_i$ et $\varepsilon_j$ et laisse fixes les $\varepsilon_k$ d’indice $k$ distinct de $i$ et $j$. Soit
$$
X = \{\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_{l+1}\}.
$$
Alors $g \mapsto \varphi(g)|X$ est un isomorphisme de $W(R)$ sur le groupe symétrique de $X$. Ainsi, $W(R)$ est isomorphe au groupe symétrique $S_{l+1}$, donc est d’ordre $(l + 1)!$.

L’algèbre symétrique $S(E)$ s’identifie canoniquement à l’algèbre des fonctions polynômes $P(\xi_1, \xi_2, \ldots, \xi_{l+1})$ sur $E$. Soit $G = \varphi(W(R))$. D’après ce qui précède, l’ensemble $S(E)^G$ des éléments de $S(E)$ invariants par $G$ est l’ensemble des polynômes symétriques (\emph{Alg.}, chap. V, App. I), et par suite (\emph{ibid.}) $S(E)^G$ est l’algèbre engendrée par les fonctions
$$
s'_i = \sum_{\tau \in S_{l+1}} \xi_{\tau(1)} \xi_{\tau(2)} \cdots \xi_{\tau(i)} \quad (1 \leq i \leq l + 1).
$$
L’algèbre $S(V)$ s’identifie à l’algèbre des restrictions à $V$ des fonctions polynômes sur $E$. Si $P \in S(E)^G$, la restriction de $P$ à $V$ est évidemment invariante par $W(R)$. Réciproquement, si $Q \in S(V)^{W(R)}$, il existe $P \in S(E)$ prolongeant $Q$; remplaçant $P$ par $((l + 1)!)^{-1} \sum_{g \in G} g(P)$, qui a même restriction que $P$ à $V$, on voit qu’on peut supposer $P \in S(E)^G$. Ainsi, $S(V)^{W(R)}$ est engendré par les $s_i = s'_i|V$. Or $s_1 = 0$. Par ailleurs, le degré de transcendance sur $\mathbf{R}$ du corps des fractions de $S(V)^{W(R)}$ est $l$, donc les $s_i$ ($2 \leq i \leq l + 1$) sont algébriquement indépendants. Comme les $s_i$ sont de degrés $2, 3, \ldots, l + 1$, les exposants de $W(R)$ sont :
$$
1, 2, 3, \ldots, l.
$$

(XI) Pour $l = 1$, on a $A(R) = W(R) = \mathbf{Z}/2\mathbf{Z}$ et $w_0 = -1$.

Pour $l \geq 2$, soit $\varepsilon \in A(R)$ l’automorphisme qui transforme $\alpha_i$ en $\alpha_{l+1-i}$. Il est clair que l’automorphisme du graphe de Dynkin induit par $\varepsilon$ est l’unique automorphisme non trivial de ce graphe. Le groupe $A(R)/W(R)$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$. Comme $-1$ est un élément de $A(R)$ qui n’appartient pas à $W(R)$ d’après (IX) et (X), on voit que $A(R)$ est isomorphe à $W(R) \times \mathbf{Z}/2\mathbf{Z}$. On a $w_0 = -\varepsilon$.

(XII) Le groupe $P(R^\vee)/Q(R^\vee)$ étant cyclique d’ordre $l + 1$, il opère sur le graphe de Dynkin complété par permutations circulaires. Si $l \geq 2$, l’unique élément non neutre de $A(R)/W(R)$ opère sur $P(R^\vee)/Q(R^\vee)$ par l’automorphisme $x \mapsto -x$.

### 8. Systèmes de type $D_l$ ($l \geq 3$).

(I) Considérons dans $V = \mathbf{R}^l$ le groupe $L_0$ (n° 4). L’ensemble $R$ des $\alpha \in L_0$ tels que $(\alpha|\alpha) = 2$ est formé des vecteurs $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Il est clair que $R$ engendre $V$ et que $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$ quels que soient $\alpha, \beta \in R$. Donc $R$ est un système de racines réduit dans $V$ (n° 4). Le nombre de racines est $n = 2l(l-1)$.

(II) Posons

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \quad \alpha_2 = \varepsilon_2 - \varepsilon_3, \quad \ldots, \quad \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \quad \alpha_l = \varepsilon_{l-1} + \varepsilon_l.
$$

On a aussitôt les formules

$$
\begin{align*}
\varepsilon_i - \varepsilon_j &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} \quad (i < j) \\
\varepsilon_i + \varepsilon_j &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} + 2\alpha_j + 2\alpha_{j+1} + \cdots \\
&\phantom{=} + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l \quad (i < j \leq l-2) \\
\varepsilon_i + \varepsilon_{l-1} &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_l \quad (i < l-1) \\
\varepsilon_i + \varepsilon_l &= \alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2} + \alpha_l \quad (i < l-1) \\
\varepsilon_{l-1} + \varepsilon_l &= \alpha_l,
\end{align*}
$$

donc $(\alpha_1, \ldots, \alpha_l)$ est une base de $R$ ($\S 1$, n° 7, cor. 3 de la prop. 20). En outre, on a $\| \alpha_i \|^2 = 2$ pour tout $i$, $(\alpha_i|\alpha_j) = 0$ pour $i + 1 < j$ sauf pour $i = l-2$, $j = l$ qui donne $(\alpha_{l-2}|\alpha_l) = -1$, $(\alpha_i|\alpha_{i+1}) = -1$ pour $i \leq l-2$, et enfin $(\alpha_{l-1}|\alpha_l) = 0$; le graphe de Dynkin de $R$ est donc de type $D_l$. Les racines positives sont les $\varepsilon_i \pm \varepsilon_j$ pour $i < j$.

(III) On a $h = \frac{n}{l} = 2(l-1)$.

(IV) Soit $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l$, qui est une racine. La somme de ses coordonnées relativement à $(\alpha_i)$ est

$$
2l-3 = h-1.
$$

Donc $\tilde{\alpha}$ est la plus grande racine.

Si $l = 3$, on a
$$
(\tilde{\alpha}|\alpha_1) = 0, \quad (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = 1.
$$
Si $l \geq 4$, on a $(\tilde{\alpha}|\alpha_i) = 0$ pour $i \neq 2$ et $(\tilde{\alpha}|\alpha_2) = 1$. D'où le graphe de Dynkin complété:

![Graphe de Dynkin](../images/dynkin_graph.png)

(V) Comme $(\alpha|\alpha) = 2$ pour tout $\alpha \in \mathbf{R}$, on a $\mathbf{R}^\vee = \mathbf{R}$.
La longueur des racines pour $\Phi_\mathbf{R}$ est $h^{-1/2} = (2l - 2)^{-1/2}$. D'où
$$
\Phi_\mathbf{R}(x, y) = (x|y)/(4l - 4) \quad \text{et} \quad \gamma(\mathbf{R}) = 4(l - 1)^2.
$$
(VI) Un calcul analogue à celui du n° 7 donne les poids fondamentaux :
$$
\begin{align*}
\overline{\omega}_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i - 1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2}) \\
&\hspace{10cm} + \frac{1}{2} i(\alpha_{l-1} + \alpha_l)
\end{align*}
$$
pour $i < l - 1$,
$$
\begin{align*}
\overline{\omega}_{l-1} &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} - \varepsilon_l) \\
&= \frac{1}{2} (\alpha_1 + 2\alpha_2 + \cdots + (l - 2)\alpha_{l-2} + \frac{1}{2} l\alpha_{l-1} + \frac{1}{2} (l - 2)\alpha_l).
\end{align*}
$$
$$
\begin{align*}
\overline{\omega}_l &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} + \varepsilon_l) \\
&= \frac{1}{2} (\alpha_1 + 2\alpha_2 + \cdots + (l - 2)\alpha_{l-2} + \frac{1}{2} (l - 2)\alpha_{l-1} + \frac{1}{2} l\alpha_l).
\end{align*}
$$
(VII) La somme des racines positives est
$$
\begin{align*}
2\rho &= 2(l - 1)\varepsilon_1 + 2(l - 2)\varepsilon_2 + \cdots + 2\varepsilon_{l-1} \\
&= \sum_{i=1}^{l-2} 2\left(il - \frac{i(i+1)}{2}\right) \alpha_i + \frac{l(l-1)}{2} (\alpha_{l-1} + \alpha_l).
\end{align*}
$$
(VIII) Les $\pm \varepsilon_i \pm \varepsilon_j$ engendrent $L_1$ (n° 4), donc $Q(\mathbf{R}) = L_1$. Donc $Q(\mathbf{R}^\vee) = L_1$ et par suite $P(\mathbf{R}) = L_2$ (n° 4). D'après le n° 4, $P(\mathbf{R})/Q(\mathbf{R})$ est isomorphe à $\mathbf{Z}/4\mathbf{Z}$ pour $l$ impair, à $(\mathbf{Z}/2\mathbf{Z}) \times (\mathbf{Z}/2\mathbf{Z})$ pour $l$ pair. Dans le premier cas, $P(\mathbf{R})/Q(\mathbf{R})$ est engendré par l'image canonique de $\overline{\omega}_l$ (et aussi par celle de $\overline{\omega}_{l-1}$). Dans le second cas, $P(\mathbf{R})/Q(\mathbf{R})$ est engendré par les images canoniques de $\overline{\omega}_{l-1}$ et $\overline{\omega}_l$. Dans les deux cas, l'indice de connexion est 4.
(IX) et (X) Dans $\mathbf{R}^l$, la réflexion orthogonale $s_{\varepsilon_i-\varepsilon_j}$ ($i \neq j$) échange $\varepsilon_i$ et $\varepsilon_j$, et laisse invariante les $\varepsilon_k$ d'indice $k$ distinct de $i$ et $j$. Les $s_{\varepsilon_i-\varepsilon_j}$ engendrent un groupe $G_1$ isomorphe au groupe symétrique $\mathfrak{S}_l$. D'autre part, $s_{ij} = s_{\varepsilon_i - \varepsilon_j} s_{\varepsilon_i + \varepsilon_j}$ transforme $\varepsilon_i$ en $-\varepsilon_i$, $\varepsilon_j$ en $-\varepsilon_j$ et laisse invariants les $\varepsilon_k$ d'indice $k$ distinct de $i$ et $j$. Les $s_{ij}$ engendrent un groupe $G_2$, ensemble des automorphismes $u$ de l'espace vectoriel $\mathbf{R}^l$ tels que $u(\varepsilon_i) = (-1)^{\nu_i} \varepsilon_i$ avec $\prod_{i=1}^l (-1)^{\nu_i} = 1$. Le groupe $G_2$ est isomorphe à $(\mathbf{Z}/2\mathbf{Z})^{l-1}$, et $G_2$ est distingué dans $W(\mathbf{R})$, donc $W(\mathbf{R})$ est isomorphe à un produit semi-direct de $\mathfrak{S}_l$ par $(\mathbf{Z}/2\mathbf{Z})^{l-1}$. Son ordre est par suite $2^{l-1} \cdot l!$

Les fonctions polynômes $t_i$ du n° 5 sont invariantes par $W(\mathbf{R})$, et il en est de même de $t = \xi_1 \xi_2 \ldots \xi_l$; on a d'ailleurs $t_l = t^2$. Soit alors $P(\xi_1, \ldots, \xi_l)$ une fonction polynôme invariante par $W(\mathbf{R})$. Soit $\xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$ un monôme figurant dans $P$ tel que $\nu_i$ soit impair; alors $\nu_j$ est impair pour tout $j$, car dans $s_{ij}(P)$ figure le monôme $(-1)^{\nu_i + \nu_j} \xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$, d'où $\nu_i + \nu_j \equiv 0$ (mod. 2) et $\nu_j \equiv 1$ (mod. 2). Donc $P = P_1 + tP_2$, où tous les monômes figurant dans $P_1$ et $P_2$ possèdent uniquement des exposants pairs. Comme $P$ est invariant par les permutations des $\xi_i$, $P_1$ et $P_2$ possèdent la même propriété, donc s'écrivent comme des polynômes par rapport à $t_1, t_2, \ldots, t_l$. Ceci prouve que l'algèbre $S(\mathbf{R}^l)^{W(\mathbf{R})}$ est engendrée par $t_1, t_2, \ldots, t_{l-1}, t$. Par ailleurs, le degré de transcendance du corps des fractions de $S(\mathbf{R}^l)^{W(\mathbf{R})}$ est $l$, donc $t_1, t_2, \ldots, t_{l-1}, t$ sont algébriquement indépendants. On en conclut que la suite des exposants, convenablement ordonnée, est :

$$
1,\ 3,\ 5,\ \ldots,\ 2l-5,\ 2l-3,\ l-1.
$$

On notera que $l-1$ apparaît deux fois si $l$ est pair, une seule fois si $l$ est impair.

(XI) Les automorphismes du graphe de Dynkin sont ceux du graphe sous-jacent. Donc :
1) Si $l = 3$, $A(\mathbf{R})/W(\mathbf{R})$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$.
2) Si $l = 4$, toute permutation des sommets terminaux définit un automorphisme du graphe, donc $A(\mathbf{R})/W(\mathbf{R})$ est isomorphe à $\mathfrak{S}_3$.
3) Si $l \geqslant 5$, les chaînes issues du point de ramification $\alpha_{l-2}$ ont pour longueur 1,1 et $l-3 \geqslant 2$. Le seul automorphisme du graphe distinct de l'identité correspond donc à l'automorphisme $\varepsilon \in A(\mathbf{R})$ qui permute $\alpha_{l-1}$ et $\alpha_l$ et laisse fixes les $\alpha_i$ pour $1 \leqslant i \leqslant l-2$. Donc $A(\mathbf{R})/W(\mathbf{R})$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$; de plus $A(\mathbf{R})$ est produit semi-direct du groupe $G_1 \simeq \mathfrak{S}_l$ défini dans (IX) par le groupe $G_3$ formé des automorphismes $u$ de $\mathbf{R}^l$ tels que $u(\varepsilon_i) = \pm \varepsilon_i$ pour tout $i$.

Si $l$ est pair, on a $-1 \in W(\mathbf{R})$, d'où $w_0 = -1$. Si $l$ est impair, on a $-1 \notin W(\mathbf{R})$, d'où $A(\mathbf{R}) = W(\mathbf{R}) \times \{1, -1\}$ et $w_0 = -\varepsilon$.

(XII) Pour $l$ pair, $P(R^\vee)/Q(R^\vee)$ a trois éléments d'ordre 2, $\omega_1, \omega_{l-1}$ et $\omega_l$. Comme $\omega_l$ (resp. $\omega_{l-1}$) échange les sommets correspondant à $\alpha_0$ et $\alpha_l$ (resp. $\alpha_{l-1}$), il échange ceux correspondant à $\alpha_1$ et $\alpha_{l-1}$ (resp. $\alpha_l$) et aussi ceux correspondant à $\alpha_j$ et $\alpha_{l-j}$ pour
$$
2 \leq j \leq l - 2.
$$
On a $\omega_1 = \omega_l \omega_{l-1}$.

Pour $l$ impair, $P(R^\vee)/Q(R^\vee)$ a deux éléments d'ordre 4 qui sont $\omega_{l-1}$ et $\omega_l$, et un élément d'ordre 2, égal à $\omega_1$. En effet $\omega_1$ échange les sommets correspondant à $\alpha_0$ et $\alpha_1$, donc il laisse fixes les sommets correspondant aux $\alpha_j$ pour $2 \leq j \leq l - 2$ et est nécessairement d'ordre 2. Par suite $\omega_l$ est d'ordre 4 et transforme le sommet correspondant à $\alpha_0$ (resp. $\alpha_l$, resp. $\alpha_1$, resp. $\alpha_{l-1}$) en celui correspondant à $\alpha_l$ (resp. $\alpha_1$, resp. $\alpha_{l-1}$, resp. $\alpha_0$), et échange les sommets correspondant à $\alpha_j$ et $\alpha_{l-j}$ pour $2 \leq j \leq l - 2$. On a $\omega_1 = \omega_l^2$ et $\omega_{l-1} = \omega_l^3$.

Pour $l \neq 4$, l'élément non neutre de $A(R)/W(R)$ échange les sommets correspondant à $\alpha_{l-1}$ et $\alpha_l$, et par suite échange les éléments $\omega_{l-1}$ et $\omega_l$ de $P(R^\vee)/Q(R^\vee)$. Pour $l$ impair, l'automorphisme ainsi obtenu de $P(R^\vee)/Q(R^\vee)$ est l'application $x \mapsto -x$.

Pour $l = 4$, $A(R)/W(R)$ s'identifie au groupe des permutations de $\{1, 3, 4\}$ et opère par permutation des indices sur $\{\omega_1, \omega_3, \omega_4\}$.

### 9. Système de type $F_4$

(I) Considérons dans $\mathbf{R}^4$ le groupe $L_2$ (n° 4). Soit $R$ l'ensemble des $\alpha \in L_2$ tels que $(\alpha|\alpha) = 1$ ou $(\alpha|\alpha) = 2$; il contient les vecteurs
$$
\pm \varepsilon_i, \quad \pm \varepsilon_i \pm \varepsilon_j \ (i < j), \quad \frac{1}{2} (\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
Réciproquement, si $\alpha \in R$, les coordonnées de $\alpha$ ne prennent que les valeurs 0, $\pm \frac{1}{2}$, $\pm 1$ (car $(\frac{3}{2})^2 > 2$); ces coordonnées sont, ou bien toutes entières, ce qui donne les vecteurs $\pm \varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j$, ou bien toutes égales à $\pm \frac{1}{2}$, ce qui donne les vecteurs $\frac{1}{2} (\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$.

Soient $\alpha, \beta \in R$ et montrons que $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$. Si $\alpha = \pm \varepsilon_i$, ou si $\alpha = \frac{1}{2} (\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$, on a $(\alpha|\alpha) = 1$, et on a vu au n° 4 que $(\alpha|\beta) \in \frac{1}{2} \mathbf{Z}$ puisque $\alpha, \beta \in L_2$. Si $\alpha = \pm \varepsilon_i \pm \varepsilon_j$, on a $(\alpha|\alpha) = 2$, et on a vu au n° 4 que $(\alpha|\beta) \in \mathbf{Z}$ puisque $\alpha \in L_1$ et $\beta \in L_2$. Donc $R$ est un système de racines réduit dans $\mathbf{R}^4$ (n° 4). Le nombre de racines est $n = 8 + \binom{4}{2} 4 + 2^4 = 48$.

(II) Munissons $\mathbf{R}^4$ de l'ordre lexicographique défini par la base $(\varepsilon_1, \varepsilon_2, \varepsilon_3, \varepsilon_4)$ (§ 1, n° 7). On a donc en particulier $\varepsilon_1 > \varepsilon_2 > \varepsilon_3 > \varepsilon_4$. Les racines positives sont

$$
\varepsilon_i,\quad \varepsilon_i \pm \varepsilon_j\ (i < j),\quad \frac{1}{2}\ (\varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$

La plus petite est $\alpha_3 = \varepsilon_4$. Parmi les racines positives appartenant à $\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$ mais non à $\mathbf{R}\varepsilon_4$, la plus petite est $\alpha_2 = \varepsilon_3 - \varepsilon_4$. Parmi les racines positives appartenant à $\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$ mais non à $\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$, la plus petite est $\alpha_1 = \varepsilon_2 - \varepsilon_3$. Parmi les racines positives n’appartenant pas à $\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$, la plus petite est $\alpha_4 = \frac{1}{2}\ (\varepsilon_1 - \varepsilon_2 - \varepsilon_3 - \varepsilon_4)$. Aucune $\alpha_i$ n’est somme de 2 racines positives. Donc $(\alpha_1, \alpha_2, \alpha_3, \alpha_4)$ est une base de $\mathbf{R}$ (\S 1, n° 6, cor. 1 de la prop. 19). On a $\| \alpha_1 \|^2 = \| \alpha_2 \|^2 = 2, \| \alpha_3 \|^2 = \| \alpha_4 \|^2 = 1,$
$(\alpha_1|\alpha_2) = (\alpha_2|\alpha_3) = -1, (\alpha_3|\alpha_4) = -\frac{1}{2}, (\alpha_1|\alpha_3) = (\alpha_1|\alpha_4) = (\alpha_2|\alpha_4) = 0$.

On voit que $\mathbf{R}$ a un graphe de Dynkin de type $F_4$, donc est irréductible.

(III) On a $h = \frac{n}{l} = 12$.

(IV) Soit $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4$. La somme des coordonnées de $\tilde{\alpha}$ par rapport à $(\alpha_i)$ est $11 = h - 1$, donc $\tilde{\alpha}$ est la plus grande racine. On a $(\tilde{\alpha}|\alpha_1) = 1, (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = (\tilde{\alpha}|\alpha_4) = 0$.

Le graphe de Dynkin complété est:

![Graphe de Dynkin complet](https://i.imgur.com/3Q5z5QG.png)

(V) La formule $\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)}$ donne pour $R^\vee$ l’ensemble des vecteurs $\pm 2\varepsilon_i$
$\pm \varepsilon_i \pm \varepsilon_j, \pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4$. Le graphe de Dynkin de $R^\vee$ se déduit de celui de $\mathbf{R}$ par le procédé expliqué au n° 2, et l’on voit que $R^\vee$ est de type $F_4$.

Les racines non orthogonales à $\beta = \varepsilon_1$ sont $\pm \varepsilon_1, \pm \varepsilon_1 \pm \varepsilon_j\ (j \geq 2)$,
et $\frac{1}{2}\ (\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$; le nombre $n(\alpha, \beta) = 2(\alpha|\beta)$ est égal à $\pm 2$ pour les 14 premières de ces racines et à $\pm 1$ pour les 16 dernières; donc, pour $\Phi_R$, le carré de la longueur de $\beta$ est $4(14.4 + 16.1)^{-1} = \frac{1}{18}$; donc

$$
\Phi_R(x, y) = (x|y)/18.
$$

Appliquons alors la formule (18) du § 1, n° 12, avec $x = y = \beta$; il vient

$$
2 + 12.\frac{1}{4} + 16\frac{1/4}{1} = \gamma(\mathbf{R}) \cdot \frac{1}{18}
$$

d’où

$$
\gamma(\mathbf{R}) = 2.3^4.
$$

(VI) Le calcul des poids fondamentaux donne ici
$$
\overline{\omega}_1 = \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4 = \tilde{\alpha}
$$
$$
\overline{\omega}_2 = 2\varepsilon_1 + \varepsilon_2 + \varepsilon_3 = 3\alpha_1 + 6\alpha_2 + 8\alpha_3 + 4\alpha_4
$$
$$
\overline{\omega}_3 = \frac{1}{2} (3\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4) = 2\alpha_1 + 4\alpha_2 + 6\alpha_3 + 3\alpha_4
$$
$$
\overline{\omega}_4 = \varepsilon_1 = \alpha_1 + 2\alpha_2 + 3\alpha_3 + 2\alpha_4.
$$

(VII) La somme des racines positives est
$$
2\rho = 11\varepsilon_1 + 5\varepsilon_2 + 3\varepsilon_3 + \varepsilon_4 = 16\alpha_1 + 30\alpha_2 + 42\alpha_3 + 22\alpha_4.
$$

(VIII) On a $Q(R) = L_2$ (no 4), et $P(R) = Q(R)$ d’après (VI). L’indice de connexion est donc 1.

(IX) La famille des exposants a 4 termes, et puisque $h = 12$, les entiers 1, 5, 7, 11, étrangers à 12, doivent figurer dans cette famille (\$ 1, no 11, prop. 30); ce sont par suite tous les exposants de $W(R)$.

(X) et (XI) Le seul automorphisme du graphe de Dynkin est l’identité, donc $A(R) = W(R)$ et $w_0 = -1$. Soit $R'$ l’ensemble des éléments de $R$ de plus grande longueur, c’est-à-dire les $\pm \varepsilon_i \pm \varepsilon_j : R'$ est le système de racines de type $D_4$ construit au no 8. Tout élément de $A(R)$ est évidemment un élément de $A(R')$. Réciproquement, un élément de $A(R')$ laisse stable $L_1$ (qui est engendré par $R'$), donc son associé $L_2$, donc $R$. D’où $W(R) = A(R) = A(R')$. D’après le no 8, $W(R)$ est donc produit semi-direct de $S_3$ et de $W(R')$, $W(R')$ étant lui-même produit semi-direct de $S_4$ et de $(\mathbf{Z}/2\mathbf{Z})^3$. L’ordre de $W(R)$ est $3!4!2^3 = 2^7.3^2$.

### 10. Système de type $E_8$

(I) Considérons dans $\mathbf{R}^8$ le groupe $L_3$ (no 4). Soit $R$ l’ensemble des $\alpha \in L_3$ tels que $(\alpha|\alpha) = 2$; il contient les vecteurs
$$
\pm \varepsilon_i \pm \varepsilon_j \ (i < j), \quad \frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i \quad (\sum_{i=1}^8 \nu(i) \text{ pair}).
$$
Réciproquement, si un élément $\alpha \in L_3$ est tel que $(\alpha|\alpha) = 2$, ses coordonnées ne peuvent prendre que les valeurs 0, $\pm \frac{1}{2}$, $\pm 1$; d’après le no 4, ces coordonnées sont, ou bien toutes entières, ce qui donne les vecteurs $\pm \varepsilon_i \pm \varepsilon_j$, ou toutes égales à $\pm \frac{1}{2}$ et de somme paire, ce qui donne les vecteurs
$$
\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i
$$
avec $\sum_{i=1}^8 \nu(i)$ pair.

On a vu (n° 4) que $(\alpha|\beta) \in \mathbf{Z}$ quels que soient $\alpha, \beta \in L_3$. Donc $R$ est un système de racines réduit. Le nombre de racines est $n = \binom{8}{2} . 4 + 2^7 = 240$.

(II) Soit $\rho$ le vecteur $(0, 1, 2, 3, 4, 5, 6, 23)$ de $L_3$. Aucun élément de $R$ n’est orthogonal à $\rho$ (c’est clair pour les $\pm \varepsilon_i \pm \varepsilon_j$; si $\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i$ était orthogonal à $\rho$, on aurait $\sum_{i=1}^6 i(-1)^{\nu(i+1)} + 23(-1)^{\nu(8)} = 0$, ce qui est impossible puisque $\sum_{i=1}^6 i < 23$). Donc (\S 1, n° 7, cor. 2 de la prop. 20) les $\alpha \in R$ telles que $(\alpha|\rho) > 0$ sont les racines positives relativement à une certaine chambre. Ces racines sont les $\pm \varepsilon_i + \varepsilon_j (i < j)$, et les

$$
\frac{1}{2} (\varepsilon_8 + \sum_{i=1}^7 (-1)^{\nu(i)} \varepsilon_i)
$$

avec $\sum_{i=1}^7 \nu(i)$ pair. On a $(\alpha|\rho) \in \mathbf{Z}$ pour tout $\alpha \in R$ (n° 4), et $(\alpha|\rho)$ est égal à 1 pour les racines suivantes :

$$
\begin{align*}
\alpha_1 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7) \\
\alpha_2 &= \varepsilon_1 + \varepsilon_2, \quad \alpha_3 = \varepsilon_2 - \varepsilon_1, \quad \alpha_4 = \varepsilon_3 - \varepsilon_2, \quad \alpha_5 = \varepsilon_4 - \varepsilon_3, \\
\alpha_6 &= \varepsilon_5 - \varepsilon_4, \quad \alpha_7 = \varepsilon_6 - \varepsilon_5, \quad \alpha_8 = \varepsilon_7 - \varepsilon_6
\end{align*}
$$

et ces huit vecteurs forment une base de $R^8$. D’après le \S 1, n° 6, cor. 1 de la prop. 19, $(\alpha_1, \alpha_2, \ldots, \alpha_8)$ est la base de $R$ pour laquelle les racines positives sont celles qui ont été définies plus haut. On a

$$(\alpha_4|\alpha_5) = (\alpha_5|\alpha_6) = (\alpha_6|\alpha_7) = (\alpha_7|\alpha_8) = (\alpha_4|\alpha_2) = (\alpha_4|\alpha_3) = (\alpha_3|\alpha_1) = -1,$$

et $(\alpha_i|\alpha_j) = 0$ pour les autres couples d’indices. Le graphe de Dynkin de $R$ est donc de type $E_8$, et $R$ est irréductible.

(III) On a $h = \frac{n}{8} = 30$.
(IV) Soit

$$\tilde{\alpha} = \varepsilon_7 + \varepsilon_8 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8,$$

qui est une racine. La somme de ses coordonnées par rapport à $(\alpha_i)$ est $29 = h - 1$, donc $\tilde{\alpha}$ est la plus grande racine. Elle est orthogonale à tous les $\alpha_i$ sauf $\alpha_8$, et $(\tilde{\alpha}|\alpha_8) = 1$. D’où le schéma de Dynkin complété :

$$
\begin{array}{cccccccccc}
\circ & \circ & \circ & \circ & \circ & \circ & \circ & \circ & \circ \\
\alpha_1 & \alpha_3 & \alpha_4 & \alpha_5 & \alpha_6 & \alpha_7 & \alpha_8 \\
\downarrow & & & & & & & & \\
\alpha_2
\end{array}
$$

(V) Comme $(\alpha|\alpha) = 2$ pour tout $\alpha \in R$, on a $R^\vee = R$.

Pour $\Phi_R$, le carré de la longueur des racines est $\frac{1}{30}$ (\S 1, no 12). Donc $\Phi_R(x, y) = (x|y)/60$, et $\gamma(R) = 900$ (\S 1, no 12, formule (20)).

(VI) Le calcul des poids fondamentaux donne

$$
\begin{align*}
\overline{\omega}_1 &= 2\varepsilon_8 = 4\alpha_1 + 5\alpha_2 + 7\alpha_3 + 10\alpha_4 + 8\alpha_5 + 6\alpha_6 + 4\alpha_7 + 2\alpha_8 \\
\overline{\omega}_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8) \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\overline{\omega}_3 &= \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 7\varepsilon_8) \\
&= 7\alpha_1 + 10\alpha_2 + 14\alpha_3 + 20\alpha_4 + 16\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\overline{\omega}_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8 \\
&= 10\alpha_1 + 15\alpha_2 + 20\alpha_3 + 30\alpha_4 + 24\alpha_5 + 18\alpha_6 + 12\alpha_7 + 6\alpha_8 \\
\overline{\omega}_5 &= \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 4\varepsilon_8 \\
&= 8\alpha_1 + 12\alpha_2 + 16\alpha_3 + 24\alpha_4 + 20\alpha_5 + 15\alpha_6 + 10\alpha_7 + 5\alpha_8 \\
\overline{\omega}_6 &= \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 3\varepsilon_8 \\
&= 6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\overline{\omega}_7 &= \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8 \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 8\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\overline{\omega}_8 &= \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8 = \tilde{\alpha}.
\end{align*}
$$

(VII) La demi-somme des racines positives est la somme des poids fondamentaux (\S 1, no 10, prop. 29) et vaut donc

$$
\rho = \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 5\varepsilon_6 + 6\varepsilon_7 + 23\varepsilon_8 \\
= 46\alpha_1 + 68\alpha_2 + 91\alpha_3 + 135\alpha_4 + 110\alpha_5 + 84\alpha_6 + 57\alpha_7 + 29\alpha_8.
$$

(VIII) Le groupe $Q(R)$ est engendré par les $\varepsilon_i \pm \varepsilon_j$ et $\frac{1}{2} \sum_{i=1}^8 \varepsilon_i$, et est égal à $L_3$ (no 4). Donc $P(R)$, qui est l’associé de $Q(R^\vee) = Q(R) = L_3$, est $L_3$ (no 4). L’indice de connexion est égal à 1.

(IX) La famille des exposants a 8 termes, et puisque $h = 30$, les entiers 1, 7, 11, 13, 17, 19, 23, 29, étrangers à 30, doivent figurer dans cette famille; ce sont par suite tous les exposants de $W(R)$.

(X) On déduit de (IX) et du chap. V, § 6, no 2, cor. 1 de la prop. 3, que l’ordre de $W(R)$ est

$$
2.8.12.14.18.20.24.30 = 2^{14}.3^5.5^2.7.
$$

(XI) Le seul automorphisme du graphe de Dynkin est l’identité puisque les trois chaînes issues du point de ramification sont de longueurs distinctes. Donc $A(R) = W(R)$ et $w_0 = -1$.

### 11. Système de type $E_7$

(I) et (II) Soit $E = \mathbf{R}^8$, et soit $R_8$ le système de racines de $E$ construit au no 10. Soit $V$ l’hyperplan de $E$ engendré par les racines $\alpha_1, \ldots, \alpha_7$ de $R_8$; il est orthogonal au huitième poids fondamental $\omega = \varepsilon_7 + \varepsilon_8$ de $R_8$.

Soit $R = R_8 \cap V$. Alors $R$ est un système de racines réduit de base $(\alpha_1, \ldots, \alpha_7)$, cf. § 1, no 7, cor. 4 de la prop. 20; ce système est donc de type $E_7$. Ses éléments sont:

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 6), \qquad \pm (\varepsilon_7 - \varepsilon_8),
$$
$$
\pm \frac{1}{2} (\varepsilon_7 - \varepsilon_8 + \sum_{i=1}^6 (-1)^{\nu(i)} \varepsilon_i) \qquad \text{avec } \sum_{i=1}^6 \nu(i) \text{ impair.}
$$

Le nombre de racines est $n = 2 + \binom{6}{2} . 4 + 2^6 = 126$. Les racines positives sont

$$
\pm \varepsilon_i + \varepsilon_j \quad (1 \leq i < j \leq 6), \qquad -\varepsilon_7 + \varepsilon_8,
$$
$$
\frac{1}{2} (-\varepsilon_7 + \varepsilon_8 + \sum_{i=1}^6 (-1)^{\nu(i)} \varepsilon_i) \qquad \text{avec } \sum_{i=1}^6 \nu(i) \text{ impair.}
$$

(III) On a $h = \frac{n}{l} = 18$.

(IV) Soit $\tilde{\alpha} = \varepsilon_8 - \varepsilon_7 = 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7$, qui est une racine. La somme de ses coordonnées par rapport à $(\alpha_i)$ est $17 = h - 1$. C’est donc la plus grande racine. Elle est orthogonale à $\alpha_i$ pour $2 \leq i \leq 7$, et $(\tilde{\alpha}|\alpha_1) = 1$. Le graphe de Dynkin complété est

![Graphe de Dynkin completé](https://i.imgur.com/3Q5z5QG.png)

(V) Comme $(\alpha|\alpha) = 2$ pour tout $\alpha \in R$, on a $R^\vee = R$.

Pour $\Phi_R$, le carré de la longueur des racines est $\frac{1}{18}$, donc

$$
\Phi_R(x, y) = (x|y)/36, \qquad \text{et} \qquad \gamma(R) = 2^2 . 3^4
$$
(§ 1, no 12, formule (20)).

(VI) Le calcul des poids fondamentaux donne

$$
\overline{\omega}_1 = \varepsilon_8 - \varepsilon_7 = 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7 = \tilde{\alpha}
$$
$$
\overline{\omega}_2 = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 2\varepsilon_7 + 2\varepsilon_8)
$$
$$
= \frac{1}{2} (4\alpha_1 + 7\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 8\alpha_6 + 3\alpha_7)
$$

$$
\overline{\omega}_3 = \frac{1}{2} (-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 3\varepsilon_7 + 3\varepsilon_8)
= 3\alpha_1 + 4\alpha_2 + 6\alpha_3 + 8\alpha_4 + 6\alpha_5 + 4\alpha_6 + 2\alpha_7
$$
$$
\overline{\omega}_4 = \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + 2(\varepsilon_8 - \varepsilon_7)
= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 6\alpha_6 + 3\alpha_7
$$
$$
\overline{\omega}_5 = \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \frac{3}{2} (\varepsilon_8 - \varepsilon_7)
= \frac{1}{2} (6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 10\alpha_6 + 5\alpha_7)
$$
$$
\overline{\omega}_6 = \varepsilon_5 + \varepsilon_6 - \varepsilon_7 + \varepsilon_8
= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 2\alpha_7
$$
$$
\overline{\omega}_7 = \varepsilon_6 + \frac{1}{2} (\varepsilon_8 - \varepsilon_7)
= \frac{1}{2} (2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7).
$$

(VII) La somme $2\rho$ des racines positives est $2 \sum_{i=1}^{7} \overline{\omega}_i$ (\S 1, n° 10, prop. 29), d'où
$$
2\rho = 2\varepsilon_2 + 4\varepsilon_3 + 6\varepsilon_4 + 8\varepsilon_5 + 10\varepsilon_6 - 17\varepsilon_7 + 17\varepsilon_8
= 34\alpha_1 + 49\alpha_2 + 66\alpha_3 + 96\alpha_4 + 75\alpha_5 + 52\alpha_6 + 27\alpha_7.
$$

(VIII) D'après le n° 10 (VIII) et le \S 1, n° 10, prop. 28, on a
$$
\mathbf{Q}(R) = \mathbf{Q}(R_8) \cap V = L_3 \cap V \quad \text{et} \quad P(R) = p(P(R_8)) = p(L_3),
$$
où $p$ désigne la projection orthogonale de $E$ sur $V$. Le groupe $\mathbf{Q}(R)$ a pour base $(\alpha_1, \ldots, \alpha_7)$; le groupe $P(R)$ est engendré par $\mathbf{Q}(R)$ et
$$
p(\alpha_8) = \alpha_8 - \frac{1}{2} \omega.
$$
On a $\omega \in P(R_8), \frac{1}{2} \omega \notin P(R_8)$, donc $2p(\alpha_8) \in \mathbf{Q}(R)$ et $p(\alpha_8) \notin \mathbf{Q}(R)$.

On voit ainsi que $P(R)/\mathbf{Q}(R)$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$ et engendré, par exemple, par l'image de $\overline{\omega}_7$.

L'indice de connexion est 2.

(IX) La suite des exposants de $W(R)$ a 7 termes. Les nombres 1, 5, 7, 11, 13, 17, étrangers à $h = 18$, figurent dans cette suite. Le dernier exposant $m$ doit donc être que tel $m + m = 18$ (chap. V, \S 6, n° 2, formule (2)). Donc la suite des exposants est
$$
1, 5, 7, 9, 11, 13, 17.
$$

(X) On déduit de (IX) et du chap. V, \S 6, n° 2, cor. 1 de la prop. 3, que l'ordre de $W(R)$ est
$$
2.6.8.10.12.14.18 = 2^{10}.3^4.5.7.
$$

(XI) Le seul automorphisme du graphe de Dynkin est l’identité, donc $A(R) = W(R)$ et $w_0 = -1$.

(XII) $P(R^\vee)/Q(R^\vee)$ a un seul élément non neutre. Il échange les sommets correspondant à $\alpha_0$ et $\alpha_7$, $\alpha_1$ et $\alpha_6$, $\alpha_3$ et $\alpha_5$ et laisse fixes $\alpha_2$ et $\alpha_4$.

### 12. Système de type $E_6$

(I) et (II) Soit $E = R^8$, et soit $R_8$ le système de racines de $E$ construit au n° 10. Soit $V$ le sous-espace vectoriel de $E$ engendré par les racines $\alpha_1, \ldots, \alpha_6$ de $R_8$; c’est l’orthogonal du plan engendré par les deux derniers poids fondamentaux $\omega = \varepsilon_7 + \varepsilon_8$ et $\pi = \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8$ de $R_8$.

Soit $R = R_8 \cap V$. C’est un système de racines réduit de base $(\alpha_1, \ldots, \alpha_6)$, donc de type $E_6$. Ses éléments sont :

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 5)
$$
$$
\pm \frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec } \sum_{i=1}^5 \nu(i) \text{ pair.}
$$

Le nombre de racines est $n = \binom{5}{2} \cdot 4 + 2^5 = 72$. Les racines positives sont

$$
\pm \varepsilon_i + \varepsilon_j \quad (1 \leq i < j \leq 5)
$$
$$
\frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec } \sum_{i=1}^5 \nu(i) \text{ pair.}
$$

(III) On a $h = \frac{n}{6} = 12$.

(IV) Soit $\tilde{\alpha} = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8)$
$$
= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6,
$$
qui est une racine. La somme de ses coordonnées par rapport à $(\alpha_i)$ est $11 = h - 1$, donc $\tilde{\alpha}$ est la plus grande racine. Elle est orthogonale à $\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6$, et $(\tilde{\alpha}|\alpha_2) = 1$. Le graphe de Dynkin complété est

![Graphe de Dynkin complet pour E6](https://i.imgur.com/3Q5z5QG.png)

(V) Comme $(\alpha|\alpha) = 2$ pour tout $\alpha \in R$, on a $R^\vee = R$.

Pour $\Phi_R$, le carré de la longueur des racines est $\frac{1}{12}$, donc
$$
\Phi_R(x, y) = (x|y)/24, \quad \text{et} \quad \gamma(R) = 144.
$$

(VI) Le calcul des poids fondamentaux donne:

$$
\overline{\omega}_1 = \frac{2}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) = \frac{1}{3} (4\alpha_1 + 3\alpha_2 + 5\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6)
$$
$$
\overline{\omega}_2 = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8)
$$
$$
= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6 = \tilde{\alpha}
$$
$$
\overline{\omega}_3 = \frac{5}{6} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \frac{1}{2} (-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5)
$$
$$
= \frac{1}{3} (5\alpha_1 + 6\alpha_2 + 10\alpha_3 + 12\alpha_4 + 8\alpha_5 + 4\alpha_6)
$$
$$
\overline{\omega}_4 = \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8
$$
$$
= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6
$$
$$
\overline{\omega}_5 = \frac{2}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_4 + \varepsilon_5
$$
$$
= \frac{1}{3} (4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 5\alpha_6)
$$
$$
\overline{\omega}_6 = \frac{1}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_5
$$
$$
= \frac{1}{3} (2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6).
$$

(VII) La demi-somme $\rho$ des racines positives est $\sum_{i=1}^{6} \overline{\omega}_i$, d'où
$$
\rho = \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 4(\varepsilon_8 - \varepsilon_7 - \varepsilon_6)
$$
$$
= 8\alpha_1 + 11\alpha_2 + 15\alpha_3 + 21\alpha_4 + 15\alpha_5 + 8\alpha_6.
$$

(VIII) D'après le no 10 (VIII) et le § 1, no 10, prop. 28, on a
$$
Q(R) = Q(R_8) \cap V = L_3 \cap V \quad \text{et} \quad P(R) = p(P(R_8)) = p(L_3),
$$
où $p$ désigne la projection orthogonale de $E$ sur $V$. On a
$$
p(\alpha_7) = \alpha_7 - \frac{2}{3}\pi + \omega, \qquad p(\alpha_8) = \alpha_8 + \pi - 2\omega.
$$
Le groupe $Q(R)$ a pour base $(\alpha_1, \ldots, \alpha_6)$. Le groupe $P(R)$ est engendré par $Q(R)$ et $p(\alpha_7)$, car $p(\alpha_8) \in P(R_8) \cap V = Q(R_8) \cap V = Q(R)$. On a $3p(\alpha_7) \in Q(R)$ et $p(\alpha_7) \notin Q(R)$. Le groupe $P(R)/Q(R)$ est donc isomorphe à $\mathbf{Z}/3\mathbf{Z}$; il est engendré, par exemple, par l'image de $\overline{\omega}_6$.

L'indice de connexion est 3.

(IX) et (X) D'après le § 2, no 4, prop. 7, l'ordre du groupe de Weyl est $6!1.2.2.3.2.1.3 = 2^7.3^4.5$. La suite des exposants a 6 termes compris entre 1 et 11, et comporte les entiers 1, 5, 7, 11 qui sont étrangers à 12. Les autres exposants $m, m'$ sont des entiers tels que

$$
m + m' = 12
$$
$$
(m + 1)(m' + 1)(1 + 1)(5 + 1)(7 + 1)(11 + 1) = 2^7 \cdot 3^4 \cdot 5
$$

en vertu du chap. V, § 6, no 2, formule (2) et cor. 1 de la prop. 3. La seconde relation donne $(m + 1)(m' + 1) = 45$, et comme $m + m' + 2 = 14$, on obtient $m = 4, m' = 8$. La suite des exposants est donc

$$
1, \quad 4, \quad 5, \quad 7, \quad 8, \quad 11.
$$

(XI) et (XII) Comme les racines ont toutes même longueur, les automorphismes du graphe de Dynkin sont ceux du graphe sous-jacent. A part l’identité, il n’y a que l’automorphisme $\varepsilon$ qui transforme $\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6, \alpha_2$ respectivement en $\alpha_6, \alpha_5, \alpha_4, \alpha_3, \alpha_1, \alpha_2$. Donc $A(R)/W(R)$ est isomorphe à $\mathbf{Z}/2\mathbf{Z}$; comme — $1 \notin W(R)$ (chap. V, § 6, no 2, cor. 3 de la prop. 3), $A(R)$ est isomorphe à $W(R) \times \{1, -1\}$ et $w_0$ s’identifie à $-\varepsilon$. Il en résulte que l’élément non neutre de $A(R)/W(R)$ définit l’automorphisme $x \mapsto -x$ de $P(R^\vee)/Q(R^\vee)$.

De plus, $P(R^\vee)/Q(R^\vee)$ a deux éléments non neutres qui sont d’ordre 3. Ils définissent les deux seuls automorphismes d’ordre 3 du graphe de Dynkin complété.

### 13. Système de type $G_2$

(I) Dans $E = \mathbf{R}^3$, soit $V$ l’hyperplan d’équation

$$
\xi_1 + \xi_2 + \xi_3 = 0.
$$

Soit $R$ l’ensemble des $\alpha \in L_0 \cap V$ tels que $(\alpha|\alpha) = 2$ ou $(\alpha|\alpha) = 6$. Les éléments de $R$ sont

$$
\pm (\varepsilon_1 - \varepsilon_2), \quad \pm (\varepsilon_1 - \varepsilon_3), \quad \pm (\varepsilon_2 - \varepsilon_3), \quad \pm (2\varepsilon_1 - \varepsilon_2 - \varepsilon_3),
$$
$$
\pm (2\varepsilon_2 - \varepsilon_1 - \varepsilon_3), \quad \pm (2\varepsilon_3 - \varepsilon_1 - \varepsilon_2).
$$

Alors $R$ engendre $V$, et $\frac{2(\alpha|\beta)}{(\beta|\beta)} \in \mathbf{Z}$ quels que soient $\alpha, \beta \in R$ : c’est évident si $\beta = \pm (\varepsilon_i - \varepsilon_j)$ avec $i \neq j$; si $\beta = 2\varepsilon_1 - \varepsilon_2 - \varepsilon_3$ par exemple, on a $(\alpha|\beta) \in 3\mathbf{Z}$ pour tout $\alpha \in R$, d’où encore notre assertion. Donc $R$ est un système de racines réduit dans $V$. Le nombre de racines est $n = 12$.

(II) Posons $\alpha_1 = \varepsilon_1 - \varepsilon_2, \alpha_2 = -2\varepsilon_1 + \varepsilon_2 + \varepsilon_3$. Les racines sont alors

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \alpha_2,
$$
$$
\pm (3\alpha_1 + \alpha_2), \quad \pm (3\alpha_1 + 2\alpha_2).
$$

Donc $(\alpha_1, \alpha_2)$ est une base de $R$. On a $\|\alpha_1\|^2 = 2, \|\alpha_2\|^2 = 6, (\alpha_1|\alpha_2) = -3,$ donc $R$ est un système de type $G_2$. Les racines positives sont $\alpha_1, \alpha_1 + \alpha_2, 2\alpha_1 + \alpha_2, \alpha_2, 3\alpha_1 + \alpha_2, 3\alpha_1 + 2\alpha_2$.

(III) On a $h = \frac{n}{2} = 6$.

(IV) La plus grande racine est $\tilde{\alpha} = 3\alpha_1 + 2\alpha_2 = -\varepsilon_1 - \varepsilon_2 + 2\varepsilon_3$.
On a $(\tilde{\alpha}|\alpha_1) = 0,\ (\tilde{\alpha}|\alpha_2) = 3$. Le graphe de Dynkin complété est

$$
\begin{array}{c}
\alpha_1 \\
\longrightarrow \\
\alpha_2
\end{array}
$$

(V) Le système inverse $R^\vee$ est l’ensemble des vecteurs suivants :

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \frac{1}{3} \alpha_2,
$$
$$
\pm \frac{1}{3} (3\alpha_1 + \alpha_2), \quad \pm \frac{1}{3} (3\alpha_1 + 2\alpha_2).
$$

Il existe 10 racines non orthogonales à $\alpha_1$; on a $n(\beta, \alpha_1) = \pm 1$ pour 4 de ces racines, $n(\beta, \alpha_1) = \pm 3$ pour 4 autres, et $n(\beta, \alpha_1) = \pm 2$ pour $\beta = \pm \alpha_1$.
Donc le carré de la longueur de $\alpha_1$ pour $\Phi_R$ est $4(4.1 + 4.9 + 2.4)^{-1} = \frac{1}{12}$.
Donc $\Phi_R(x, y) = (x|y)/24$. Appliquons alors la formule (18) du § 1, n° 12, avec $x = y = \alpha_1$; il vient :
$$
2 + 4 \cdot \frac{1}{4} + 4 \cdot \frac{1}{4} = \gamma(R) \cdot \frac{1}{12}
$$
d’où $\gamma(R) = 48$.

(VI) et (VII) La demi-somme des racines positives est
$$
\rho = 5\alpha_1 + 3\alpha_2.
$$
Les poids fondamentaux $\varpi_1$ et $\varpi_2$ sont orthogonaux à $\alpha_2$ et $\alpha_1$, donc proportionnels à $2\alpha_1 + \alpha_2$ et $3\alpha_1 + 2\alpha_2$. On a
$$
\varpi_1 + \varpi_2 = \rho = 5\alpha_1 + 3\alpha_2 = (2\alpha_1 + \alpha_2) + (3\alpha_1 + 2\alpha_2).
$$
Donc
$$
\varpi_1 = 2\alpha_1 + \alpha_2, \quad \varpi_2 = 3\alpha_1 + 2\alpha_2 = \tilde{\alpha}.
$$

(VIII) $Q(R)$ est engendré par exemple par $\varepsilon_1 - \varepsilon_2$ et $\varepsilon_1 - \varepsilon_3$. D’après (VI) et (VII), $P(R) = Q(R)$. L’indice de connexion est 1.

(IX) La famille des exposants a 2 termes; comme 1 et $h - 1 = 5$ sont des exposants, ce sont les seuls.

(X) On a $(\overline{\alpha_1, \alpha_2}) = \frac{5\pi}{6}$, donc $W(R)$ est isomorphe au groupe diédral d’ordre 12.

(XI) Le seul automorphisme du graphe de Dynkin est l’identité, donc $A(R) = W(R)$ et $w_0 = -1$.

### 14. Systèmes de racines irréductibles non réduits

Les systèmes de racines irréductibles non réduits se déduisent des systèmes irréductibles réduits grâce aux prop. 13 et 14 du § 1, n° 4. Pour chaque entier $l \geqslant 1$, il existe, à un isomorphisme près, un seul système de racines non réduit irréductible de rang $l$: soient R un système de racines de type $B_l$, A l’ensemble des racines de plus petite longueur de R; on prend la réunion de R et de 2A. Avec les notations du n° 5, on obtient les vecteurs

$$
\pm \varepsilon_i,\ \pm 2\varepsilon_i,\ \pm \varepsilon_i \pm \varepsilon_j\quad (i < j)
$$

au nombre de $2l(l+1)$.

Exercises

## EXERCICES {#lie-vi-s4-exercises}

Si R est un système de racines, on note W^+(R) l’ensemble des éléments de W(R) de déterminant 1.

See the [exercises for § 4](exercises/s4/).
