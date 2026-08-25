---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE)
section: 2
section_title: Familles orthogonales dans un espace hilbertien
lang: fr
source: evt-i-v-fr
book_pages: EVT V.17-EVT V.25, EVT V.69-EVT V.72
pdf_pages: 0279-0287, 0331-0334
extraction: ocr
subsections:
    - "no": 1
      title: Somme hilbertienne externe d’espaces hilbertiens
      page: 17
      pdf_page: 279
    - "no": 2
      title: Somme hilbertienne de sous-espaces orthogonaux d’un espace hilbertien
      page: 18
      pdf_page: 280
    - "no": 3
      title: Familles orthonormales
      page: 21
      pdf_page: 283
    - "no": 4
      title: Orthonormalisation
      page: 23
      pdf_page: 285
statements: 23
exercises: 16
content_sha256: e5de09b0e9d0f2ad6f54ba921d0a8d90ad0f508b2222c1702d1d6d2f1979035e
---

## § 2. FAMILLES ORTHOGONALES DANS UN ESPACE HILBERTIEN

### 1. Somme hilbertienne externe d’espaces hilbertiens

#### Proposition 1 {#evt-v-s2-prop-1 .statement}

*Soient $(E_i)_{i \in I}$ une famille d’espaces hilbertiens, P l’espace vectoriel produit $\prod_{i \in I} E_i$, et E la partie de P formée des familles $x = (x_i)_{i \in I}$ telles que $\sum_{i \in I} \|x_i\|^2$ soit fini.

a) *E est un sous-espace vectoriel de P.*

b) *Quels que soient $x = (x_i)_{i \in I}$ et $y = (y_i)_{i \in I}$ dans E, la famille $(\langle x_i|y_i \rangle)_{i \in I}$ est sommable. Si l’on pose $\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$, on définit une forme hermitienne positive séparante sur E.*

c) *Pour le produit scalaire ainsi défini, E est un espace hilbertien ; la somme directe S des $E_i$ est dense dans E.*

Pour $x = (x_i)_{i \in I}$ et $y = (y_i)_{i \in I}$ dans E, on a
$$
\|x_i + y_i\|^2 \leq 2(\|x_i\|^2 + \|y_i\|^2),
$$
donc $x + y = (x_i + y_i)_{i \in I}$ appartient à E. Ceci prouve a).

D’après l’inégalité de Cauchy-Schwarz, on a
$$
|\langle x_i|y_i \rangle| \leq \|x_i\| \cdot \|y_i\| \leq \frac{1}{2}(\|x_i\|^2 + \|y_i\|^2)
$$
d’où $\sum_{i \in I} |\langle x_i|y_i \rangle| < +\infty$. On a $\langle x|x \rangle = \sum_{i \in I} \|x_i\|^2 > 0$ si $x \neq 0$, d’où aussitôt l’assertion b).

On rappelle que S est le sous-espace de P formé des familles $x = (x_i)_{i \in I}$ telles que l’ensemble des $i \in I$ pour lesquels $x_i \neq 0$ soit fini. Il est immédiat que S est dense dans E ; il reste donc à prouver que E est complet pour la topologie $\mathcal{T}_1$ déduite de la norme $\|x\| = \langle x|x \rangle^{1/2}$. Soit $\mathcal{T}_2$ la topologie induite sur E par la topologie produit sur $\prod_{i \in I} E_i$. Pour tout $r > 0$, soit $B_r$ l’ensemble des $x \in E$ tels que $\|x\| \leq r$. Cette relation signifie que l’on a $\sum_{i \in J} \|x_i\|^2 \leq r^2$ pour toute partie finie J de I, et par suite $B_r$ est une partie fermée, donc complète, de $\prod_{i \in I} E_i$. Le fait que E soit complet pour $\mathcal{T}_1$ résulte alors de TG, III, p. 27.

#### Définition 1 {#evt-v-s2-def-1 .statement}

Soit $(E_i)_{i \in I}$ une famille d’espaces hilbertiens. L’espace hilbertien E défini dans la prop. 1 s’appelle la somme hilbertienne externe de la famille $(E_i)_{i \in I}$ et se note $\bigoplus_{i \in I} E_i$ ou $\bigoplus_{i \in I} E_i$.

Soit $f_i$ l’application de $E_i$ dans E qui transforme $z \in E_i$ en l’élément $(x_k) \in E$ tel que $x_k = 0$ pour $k \neq i$ et $x_i = z$; il est clair que $f_i$ est un isomorphisme de l’espace hilbertien $E_i$ sur un sous-espace vectoriel fermé de E. On dit que $f_i$ est l’application canonique de $E_i$ dans E et on identifie le plus souvent $E_i$ et son image dans E par cet isomorphisme. Avec cette convention, $E_i$ et $E_k$ sont orthogonaux dans E pour $i \neq k$, et E est le sous-espace vectoriel fermé engendré par la réunion des sous-espaces $E_i$.

Lorsque I est fini, E est la somme directe des $E_i$; comme le projecteur canonique de E sur $E_i$ est continu pour tout $i \in I$, E est aussi alors somme directe topologique des $E_i$ (TG, III, p. 46, prop. 2). Si $I = \{1, n\}$, on écrit aussi $E_1 \oplus E_2 \oplus \ldots \oplus E_n$ au lieu de $\bigoplus_{i=1}^n E_i$.

#### Exemple {#evt-v-s2-n1-exa-1 .statement}

Soient E un espace hilbertien et I un ensemble d’indices. On désigne par $\ell^2_E(I)$ la somme hilbertienne externe de la famille $(E_i)_{i \in I}$ où $E_i = E$ pour tout $i \in I$. Autrement dit, $\ell^2_E(I)$ est l’espace des familles $x = (x_i)_{i \in I}$ d’éléments de E telles que $\sum_{i \in I} \|x_i\|^2 < +\infty$, muni du produit scalaire $\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$ (espace des familles de carré sommable d’éléments de E indexées par I). On pose $\ell^2(I) = \ell^2_K(I)$.

### 2. Somme hilbertienne de sous-espaces orthogonaux d’un espace hilbertien

#### Définition 2 {#evt-v-s2-def-2 .statement}

On dit qu’un espace hilbertien E est somme hilbertienne d’une famille $(E_i)_{i \in I}$ de sous-espaces vectoriels fermés de E, lorsque :
1) pour deux indices distincts $i, k$ dans I, les sous-espaces $E_i$ et $E_k$ sont orthogonaux dans E ;
2) le sous-espace vectoriel fermé engendré par la réunion des $E_i$ est E.

¹ On prendra garde de ne pas confondre cette notation avec celle de la somme directe « algébrique » des espaces $E_i$ (A, II, p. 12).

#### Théorème 1 {#evt-v-s2-thm-1 .statement}

Soit E un espace hilbertien somme hilbertienne d'une famille $(E_i)_{i\in I}$ de sous-espaces vectoriels fermés de E. Il existe un isomorphisme $f$ et un seul de E sur la somme hilbertienne externe $\bigoplus_{i\in I} E_i = F$ de la famille $(E_i)$ tel que, pour tout $i \in I$, la restriction de $f$ à $E_i$ soit l'application canonique $f_i$ de $E_i$ dans $F$.

Soit $S \subset F$ la somme directe « algébrique » des $E_i$, et soit $g$ l'application linéaire $(x_i)_{i\in I} \mapsto \sum_{i\in I} x_i$ de S dans E. Montrons que $g$ est un isomorphisme de l'espace préhilbertien S sur le sous-espace (préhilbertien) $g(S)$ de E, engendré par la réunion des $E_i$ : en effet, pour deux éléments $x = (x_i)_{i\in I}$, $y = (y_i)_{i\in I}$ de S, on a

$$
\langle g(x)|g(y) \rangle = \langle \sum_{i\in I} x_i | \sum_{i\in I} y_i \rangle = \sum_{(i,k)\in I \times I} \langle x_i|y_k \rangle .
$$

Mais si $i \neq k$, on a $\langle x_i|y_k \rangle = 0$ par hypothèse, d'où

$$
\langle g(x)|g(y) \rangle = \sum_{i\in I} \langle x_i|y_i \rangle = \langle x|y \rangle ;
$$

ceci démontre notre assertion. Comme S est dense dans F et $g(S)$ dense dans E, l'isomorphisme $g$ se prolonge en un isomorphisme $\bar{g}$ de F sur E (V, p. 8, cor.). Il est clair que l'isomorphisme réciproque $f$ de $\bar{g}$ répond à la question ; son unicité résulte de ce que le sous-espace fermé de E engendré par la réunion des $E_i$ est E lui-même.

Lorsque E est somme hilbertienne d'une famille $(E_i)_{i\in I}$ de sous-espaces, on identifie le plus souvent E à la somme hilbertienne externe F des $E_i$ au moyen de l'isomorphisme $f$. Si l'ensemble I est fini, dire que E est somme hilbertienne de la famille $(E_i)_{i\in I}$ signifie donc que les $E_i$ sont deux à deux orthogonaux et que l'espace vectoriel E est somme directe de la famille $(E_i)_{i\in I}$ de sous-espaces.

#### Corollaire 1 {#evt-v-s2-thm-1-cor-1 .statement}

Soit E un espace hilbertien, somme hilbertienne d'une famille $(E_i)_{i\in I}$ de sous-espaces vectoriels fermés de E ; pour tout $i \in I$, soit $p_{E_i}$ l'orthoprojecteur (V, p. 13) de E sur $E_i$.

a) Pour tout $x \in E$, la famille $(\|p_{E_i}(x)\|^2)_{i\in I}$ est sommable dans $\mathbf{R}$, la famille $(p_{E_i}(x))_{i\in I}$ est sommable dans E, et l'on a

$$
\|x\|^2 = \sum_{i\in I} \|p_{E_i}(x)\|^2 , \quad x = \sum_{i\in I} p_{E_i}(x) .
$$

b) Réciproquement, si $(x_i)_{i\in I}$ est une famille d'éléments de E tels que $x_i \in E_i$ pour tout $i \in I$ et que $\sum_{i\in I} \|x_i\|^2 < +\infty$, cette famille est sommable, et sa somme $x$ est le seul point de E tel que $p_{E_i}(x) = x_i$ pour tout $i \in I$.

c) Pour tout couple de points $x, y$ de E, on a

$$
\langle x|y \rangle = \sum_{i\in I} \langle p_{E_i}(x)|p_{E_i}(y) \rangle .
$$

Ces propriétés sont en effet évidentes dans la somme hilbertienne externe des $E_i$, et se transportent à E par isomorphisme.

#### Corollaire 2 {#evt-v-s2-thm-1-cor-2 .statement}

Soient E un espace préhilbertien séparé, $(E_i)_{i \in I}$ une famille de sous-espaces vectoriels complets de E tels que, pour tout couple d’indices distincts $i, k$ dans I, les sous-espaces $E_i$ et $E_k$ soient orthogonaux. Soit V le sous-espace vectoriel fermé de E engendré par la réunion des $E_i$. Pour tout $i \in I$, soit $p_{E_i}$ l’orthoprojecteur de E sur $E_i$. Soit $x \in E$.

1) On a $\sum_{i \in I} \|p_{E_i}(x)\|^2 \leq \|x\|^2$.

2) Les conditions suivantes sont équivalentes : a) $x \in V$; b) $\sum_{i \in I} \|p_{E_i}(x)\|^2 = \|x\|^2$;

c) la famille $(p_{E_i}(x))_{i \in I}$ est sommable dans E, et l’on a $x = \sum_{i \in I} p_{E_i}(x)$.

3) Supposons V complet. Alors la famille $(p_{E_i}(x))_{i \in I}$ est sommable dans E, et l’on a

$$
p_V(x) = \sum_{i \in I} p_{E_i}(x), \quad \|p_V(x)\|^2 = \sum_{i \in I} \|p_{E_i}(x)\|^2,
$$

en désignant par $p_V$ l’orthoprojecteur de E sur V.

En effet, soit $\hat{E}$ l’espace hilbertien complété de E ; on identifie E à un sous-espace dense de $\hat{E}$ ; les $E_i$, étant complets, sont des sous-espaces fermés de $\hat{E}$. L’adhérence $\overline{V}$ de V dans $\hat{E}$ est le sous-espace vectoriel fermé de $\hat{E}$ engendré par la réunion des $E_i$, et l’on a $V = \overline{V} \cap E$. L’espace $\hat{E}$ est somme hilbertienne des $E_i$ et du sous-espace W supplémentaire orthogonal de $\overline{V}$ dans $\hat{E}$ ; posons $x_0 = p_W(x)$ et $x_i = p_{E_i}(x)$ pour tout $i \in I$. D’après le cor. 1, on a $\|x^2\| = \|x_0\|^2 + \sum_{i \in I} \|x_i\|^2$, et $x = x_0 + \sum_{i \in I} x_i$ dans $\hat{E}$.

Ceci entraîne aussitôt l’assertion 1), et le fait que les conditions b) et c) de 2) sont équivalentes à la condition $x_0 = 0$, donc à la condition $x \in V$. Enfin, si V est complet, et si on pose $x' = p_V(x)$, on a $x' - x_i = (x - x_i) - (x - p_V(x))$, donc $x' - x_i$ est orthogonal à $E_i$, et par suite $x_i = p_{E_i}(x')$ pour tout $i \in I$ ; il suffit alors d’appliquer la propriété 2) au vecteur $x'$.

#### Remarque {#evt-v-s2-n2-rem-1 .statement}

Soient E un espace préhilbertien séparé, $(V_i)_{i \in I}$ une famille de sous-espaces vectoriels de E tels que, pour tout couple d’indices distincts $i, k$, les sous-espaces $V_i$ et $V_k$ soient orthogonaux. Alors, pour tout $k \in I$, l’intersection de $V_k$ et du sous-espace vectoriel fermé $W_k$ engendré par la réunion des $V_i$ d’indice $i \neq k$, est réduite à 0 : en effet, si $x$ appartient à la fois à $V_k$ et $W_k$, il est orthogonal à tous les $V_i$ d’indice $i \neq k$, donc à $W_k$. En particulier, il est orthogonal à lui-même, donc nul.

#### Proposition 2 {#evt-v-s2-prop-2 .statement}

Soient E un espace hilbertien et $(V_\lambda)_{\lambda \in L}$ une famille de sous-espaces vectoriels fermés de E ; pour chaque $\lambda \in L$, soit $(W_{\lambda \mu})_{\mu \in M_\lambda}$ une famille de sous-espaces vectoriels fermés de $V_\lambda$ tels que $V_\lambda$ soit le sous-espace vectoriel fermé engendré par la réunion de cette famille. Pour que E soit somme hilbertienne de la famille $(W_{\lambda \mu})_{\lambda \in L, \mu \in M_\lambda}$, il faut et il suffit que E soit somme hilbertienne de la famille $(V_\lambda)_{\lambda \in L}$ et que, pour chaque $\lambda \in L$, $V_\lambda$ soit somme hilbertienne de la famille $(W_{\lambda \mu})_{\mu \in M_\lambda}$ (« associativité de la somme hilbertienne »).

Pour montrer que la condition est nécessaire, il suffit de voir que $V_\alpha$ et $V_\beta$ sont orthogonaux si $\alpha \neq \beta$. Or, tout élément de $W_{\alpha \mu}$ ($\mu \in M_\alpha$) est orthogonal à tous les $W_{\beta v}$ ($v \in M_\beta$), donc au sous-espace vectoriel fermé $V_\beta$ qu’ils engendrent ; le même raisonnement montre ensuite que tout élément de $V_\beta$, étant orthogonal à tous les $W_{\alpha \mu}$ ($\mu \in M_\alpha$), est orthogonal à $V_\alpha$.

Pour montrer que la condition est suffisante, il suffit de vérifier que, si elle est remplie, E est égal au sous-espace vectoriel fermé F engendré par la réunion des $W_{\lambda,\mu}$ ($\lambda \in L, \mu \in M_\lambda$) ; or, pour chaque $\lambda \in L$, F contient le sous-espace vectoriel fermé engendré par la réunion des $W_{\lambda,\mu}$ tels que $\mu \in M_\lambda$, c'est-à-dire $V_\lambda$ ; donc F est le sous-espace vectoriel fermé engendré par la réunion des $V_\lambda$, c'est-à-dire E par hypothèse.

### 3. Familles orthonormales

#### Définition 3 {#evt-v-s2-def-3 .statement}

Dans un espace préhilbertien E, on dit qu'une famille $(e_i)_{i \in I}$ de vecteurs est orthogonale si $e_i$ et $e_k$ sont orthogonaux pour $i \neq k$ et orthonormale si l'on a de plus $\|e_i\| = 1$ pour tout $i \in I$.

On appelle ensemble orthonormal toute partie S de E telle que la famille définie par l'application identique de S sur elle-même soit orthonormale. Si $(e_i)_{i \in I}$ est une famille orthonormale, l'application $i \mapsto e_i$ est injective ; on peut donc parler indifféremment de famille orthonormale ou d'ensemble orthonormal.

Si $(e_i)_{i \in I}$ est une famille orthonormale, les sous-espaces vectoriels complets $D_i = K e_i$, de dimension 1, sont deux à deux orthogonaux. Pour tout $x \in E$, la projection orthogonale de $x$ sur $D_i$ est $\lambda_i e_i$, avec $\langle e_i | x - \lambda_i e_i \rangle = 0$, ce qui donne $\langle e_i | x \rangle = \lambda_i \langle e_i | e_i \rangle = \lambda_i$. Les résultats du no 2, appliqués aux sous-espaces $D_i$, donnent les énoncés suivants :

#### Proposition 3 {#evt-v-s2-prop-3 .statement}

Dans un espace préhilbertien séparé E, toute famille orthonormale est topologiquement libre.

On notera que cette propriété résulte aussi de la caractérisation des familles topologiquement libres (II, p. 5, cor. 2 et IV, p. 46, Remarque 1), compte tenu de l'identification du dual de E avec le complété de E ou de l'espace conjugué de E selon que K est égal à $\mathbf{R}$ ou $\mathbf{C}$ (V, p. 17, Remarque).

#### Proposition 4 {#evt-v-s2-prop-4 .statement}

Soient E un espace préhilbertien séparé, $(e_i)_{i \in I}$ une famille orthonormale dans E, V le sous-espace vectoriel fermé de E engendré par les $e_i$.

1) Pour tout $x \in E$, on a
$$
\sum_{i \in I} |\langle e_i | x \rangle|^2 \leq \|x\|^2
$$
(inégalité de Bessel), de sorte que l'ensemble des $i \in I$ tels que $\langle e_i | x \rangle \neq 0$ est dénombrable. En outre, les conditions suivantes sont équivalentes : a) $x \in V$; b) $\|x\|^2 = \sum_{i \in I} |\langle e_i | x \rangle|^2$; c) la famille des $\langle e_i | x \rangle . e_i$ est sommable dans E, et l'on a $x = \sum_{i \in I} \langle e_i | x \rangle . e_i$.

2) Si V est complet, la famille des $\langle e_i | x \rangle . e_i$ est sommable dans E pour tout $x \in E$, et l'on a $\sum_{i \in I} \langle e_i | x \rangle . e_i = p_V(x)$, $\sum_{i \in I} |\langle e_i | x \rangle|^2 = \|p_V(x)\|^2$.

3) Supposons V complet. Pour toute famille $(\lambda_i)_{i \in I}$ de scalaires telle que $\sum |\lambda_i|^2 < +\infty$, il existe un point $x \in V$ et un seul tel que $\langle e_i | x \rangle = \lambda_i$ pour tout $i \in I$.

$i \in I$. Si $(\mu_i)_{i \in I}$ est une seconde famille de scalaires telle que $\sum_{i \in I} |\mu_i|^2 < + \infty$, et si $y \in V$ est tel que $\langle e_i | y \rangle = \mu_i$ pour tout $i \in I$, on a $\langle x | y \rangle = \sum_{i \in I} \overline{\lambda_i} \mu_i$.

#### Proposition 5 {#evt-v-s2-prop-5 .statement}

Soit $(e_i)_{i \in I}$ une famille orthonormale dans un espace préhilbertien séparé E. Les propriétés suivantes sont équivalentes :
a) la famille $(e_i)$ est totale ;
b) pour tout $x \in E$, la famille $\langle e_i | x \rangle . e_i$ est sommable dans E, et l’on a $x = \sum_{i \in I} \langle e_i | x \rangle . e_i$ ;
c) pour tout $x \in E$, on a
(2)
$$
\|x\|^2 = \sum_{i \in I} |\langle e_i | x \rangle|^2
$$
(relation de Parseval).

Lorsque E est hilbertien ces conditions sont encore équivalentes à la suivante :
d) les relations $\langle e_i | x \rangle = 0$ pour tout $i \in I$ entraînent $x = 0$.

L’équivalence des conditions a), b), c) résulte aussitôt de la prop. 4. L’équivalence des conditions a) et d) lorsque E est hilbertien résulte du cor. 1 de V, p.16.

#### Définition 4 {#evt-v-s2-def-4 .statement}

On appelle base orthonormale d’un espace préhilbertien séparé E une famille orthonormale et totale dans E.

Une base orthonormale d’un espace préhilbertien séparé E est aussi une base orthonormale du complété de E.

Soit $(e_i)_{i \in I}$ une base orthonormale de E ; pour tout $x \in E$, les nombres $\langle e_i | x \rangle$ s’appellent, par abus de langage, les coordonnées de x par rapport à la base $(e_i)$. On a
(3)
$$
\langle x | y \rangle = \sum_{i \in I} \overline{\langle e_i | x \rangle} \langle e_i | y \rangle
$$
quels que soient $x$ et $y$ dans E.

Une base orthonormale de E n’est pas, en général, une base de E sur le corps K au sens défini en A, II, p. 25 ; pour éviter des confusions, nous dirons toujours qu’une base d’un espace préhilbertien E, au sens de loc. cit., est une base algébrique de E sur K.

Soient E et F deux espaces préhilbertiens séparés, et u une application linéaire continue de E dans F. Soit $(e_i)_{i \in I}$ (resp. $(f_j)_{j \in J}$) une base orthonormale de E (resp. F). Posons
$$
u_{ji} = \langle f_j | u(e_i) \rangle
$$
pour $i \in I$, $j \in J$. La famille $(u_{ji})_{(i,j) \in I \times J}$ est appelée la matrice de u par rapport aux bases orthonormales $(e_i)$ et $(f_j)$. Soient $x \in E$ et $y = u(x)$ ; si l’on note $\xi_i = \langle e_i | x \rangle$ et $\eta_j = \langle f_j | y \rangle$ les coordonnées de x et y respectivement, on a $\eta_j = \sum_{i \in I} u_{ji} \xi_i$ pour tout $j \in J$. Lorsque $(e_i)$ est une base algébrique de E et $(f_j)$ une base algébrique de F, notre définition est en accord avec celle de A, II, p. 144.

#### Exemple {#evt-v-s2-n3-exa-1 .statement}

Soit E l’espace des fonctions continues sur $\mathbf{R}$, à valeurs complexes, telles que $f(x + n) = f(x)$ pour $x \in \mathbf{R}$ et $n \in \mathbf{Z}$. On munit E du produit scalaire défini par
$$
\langle f | g \rangle = \int_0^1 \overline{f(t)}\, g(t)\, dt .
$$
Alors E est un espace préhilbertien séparé, mais non complet. Pour tout entier $n \in \mathbf{Z}$, posons $e_n(x) = e(nx)$. Il est immédiat que la famille $(e_n)_{n \in \mathbf{Z}}$ est orthonormale dans E. De plus, la topologie de la convergence uniforme sur E est plus fine que la topologie déduite de la norme $\|f\|_2 = \langle f | f \rangle^{1/2}$. La famille $(e_n)_{n \in \mathbf{Z}}$ est totale dans E pour la convergence uniforme (TG, X, p. 40), et a fortiori dans l’espace préhilbertien E. Donc $(e_n)_{n \in \mathbf{Z}}$ est une base orthonormale de E.

### 4. Orthonormalisation

#### Théorème 2 {#evt-v-s2-thm-2 .statement}

Pour tout ensemble orthonormal L dans un espace hilbertien E, il existe une base orthonormale B de E contenant L.

En effet, soit $\mathfrak{D}$ l’ensemble des parties orthonormales de E, ordonné par inclusion ; il est immédiat que cet ensemble est de caractère fini (E, III, p. 34). Il existe donc dans $\mathfrak{D}$ un ensemble maximal B contenant L, en vertu du th. 1 de E, III, p. 35. Tout revient à prouver que B est un ensemble total. Dans le cas contraire, il existerait un vecteur $y \neq 0$ orthogonal à tous les vecteurs de B (V, p. 22, prop. 5), et en multipliant $y$ par un scalaire convenable, on pourrait supposer que $\|y\| = 1$; alors, $B \cup \{y\}$ serait un ensemble orthonormal distinct de B et contenant B, ce qui contredit la définition de B ; d’où le théorème.

#### Corollaire 1 {#evt-v-s2-thm-2-cor-1 .statement}

Dans tout espace hilbertien, il existe une base orthonormale.

Il suffit d’appliquer le th. 2 au cas où $L = \varnothing$.

#### Corollaire 2 {#evt-v-s2-thm-2-cor-2 .statement}

Tout espace hilbertien est isomorphe à un espace $\ell^2(I)$.

De manière plus précise, soit $(e_i)_{i \in I}$ une base orthonormale d’un espace hilbertien E. D’après les prop. 4 (V, p. 21) et 5 (V, p. 22), l’application $\varphi$ définie par
$$
\varphi(x) = (\langle e_i | x \rangle)_{i \in I}
$$
est un isomorphisme d’espaces hilbertiens de E sur $\ell^2(I)$. L’isomorphisme réciproque $\psi$ est défini par
$$
\psi((\lambda_i)_{i \in I}) = \sum_{i \in I} \lambda_i e_i .
$$

#### Proposition 6 {#evt-v-s2-prop-6 .statement}

Soit E un espace préhilbertien séparé, et soit $(a_n)_{n \in I}$ (I intervalle de $\mathbf{N}$ d’origine 1) une famille libre dénombrable (finie ou non) de vecteurs de E. Il existe une famille orthonormale $(e_n)_{n \in I}$ et une seule dans E, possédant les propriétés suivantes :
1) pour tout entier $p \in I$, le sous-espace vectoriel de E engendré par $e_1, e_2, \ldots, e_p$ est identique au sous-espace vectoriel de E engendré par $a_1, a_2, \ldots, a_p$;
2) pour tout entier $p \in I$ le nombre $\langle a_p | e_p \rangle$ est réel et $> 0$.

En effet, soit $V_n$ le sous-espace (de dimension $n$) engendré par $a_1, a_2, \ldots, a_n$. Si $n + 1 \in I$ et $b_{n+1} = a_{n+1} - p_{V_n}(a_{n+1})$ ($p_{V_n}$ désignant l’orthoprojecteur sur le sous-espace complet $V_n$), la droite $Kb_{n+1}$ est l’orthogonal de $V_n$ dans $V_{n+1}$. Si les $e_n$ satisfont à la condition 1) de l’énoncé, on doit avoir $e_{n+1} = \lambda b_{n+1}$; la condition $\|e_{n+1}\| = 1$ donne ensuite $|\lambda|^2 \|b_{n+1}\|^2 = 1$, et la condition $\langle a_{n+1}|e_{n+1} \rangle > 0$ donne $\lambda \langle a_{n+1}|b_{n+1} \rangle > 0$; cela détermine complètement $\lambda$, et prouve par suite qu’on peut déterminer par récurrence une famille orthonormale $(e_n)_{n \in I}$ et une seule de façon à satisfaire aux conditions 1) et 2) de l’énoncé.

On dit que la suite $(e_n)_{n \in I}$ est obtenue par *orthonormalisation* de la famille libre $(a_n)_{n \in I}$. Il est clair que le sous-espace vectoriel engendré par la famille $(e_n)$ est identique au sous-espace vectoriel engendré par la famille $(a_n)$. En particulier, si $(a_n)$ est une suite totale, il en est de même de $(e_n)$, qui est donc une base orthonormale de $E$; d’où :

#### Corollaire {#evt-v-s2-n4-cor-1 .statement}

*Dans tout espace préhilbertien séparé $E$ de type dénombrable, il existe une base orthonormale dénombrable.*

En effet, dire que $E$ est de type dénombrable signifie qu’il existe dans $E$ une suite totale, et on peut toujours extraire d’une telle suite une famille libre totale (A, II, p. 95, th. 2).

On peut donner des exemples d’espaces préhilbertiens séparés ne possédant aucune base orthonormale (V, p. 69, exerc. 2).
*Exemple.* — Soient $I$ l’intervalle $[-1, 1]$ de $\mathbf{R}$ et $E$ l’espace vectoriel des fonctions continues sur $I$ à valeurs réelles. On note $x$ l’injection canonique de $I$ dans $\mathbf{R}$, considérée comme élément de $E$. D’après le th. de Stone-Weierstrass, la suite $(x^n)_{n \in \mathbf{N}}$ est totale dans $E$ pour la topologie de la convergence uniforme (TG, X, p. 37).

Considérons $E$ comme un espace préhilbertien réel séparé dans lequel le produit scalaire est donné par
$$
\langle f | g \rangle = \int_{-1}^{1} f(t) \, g(t) \, dt .
$$
La suite $(x^n)_{n \in \mathbf{N}}$ est alors totale dans l’espace préhilbertien $E$. Soit $(\Pi_n)_{n \in \mathbf{N}}$ la suite obtenue par orthonormalisation de la suite $(x^n)_{n \in \mathbf{N}}$. On peut montrer que l’on a $\Pi_n = (n + \frac{1}{2})^{1/2} P_n$, où le *polynôme de Legendre* $P_n$ est défini par
$$
P_n(x) = \frac{1}{2^n n!} \left( \frac{d}{dx} \right)^n (x^2 - 1)^n .
$$

#### Proposition 7 {#evt-v-s2-prop-7 .statement}

*Dans un espace hilbertien $E$, deux bases orthonormales sont équipotentes.*

Soient $B$ et $C$ deux bases orthonormales de $E$. Le cas où l’un des deux ensembles $B, C$ est fini est trivial, puisqu’une base orthonormale finie est une base algébrique de l’espace. Supposons donc $B$ et $C$ infinies. Pour tout $x \in B$, soit $C_x$ la partie de $C$ formée des $y \in C$ tels que $\langle x | y \rangle \neq 0$. L’ensemble $C_x$ est dénombrable (V, p. 21, prop. 4). Pour tout $y \in C$, il existe $x \in B$ tel que $y \in C_x$, puisque $B$ est une base orthonormale et que $y \neq 0$; autrement dit, $C$ est la réunion des ensembles dénombrables $C_x$ lorsque $x$ parcourt $B$. Le cardinal de $C$ est donc inférieur à celui de $\mathbf{N} \times B$, donc à celui de B (E, III, p. 49, cor. 4); de même, le cardinal de B est inférieur à celui de C, ce qui achève la démonstration.

Le cardinal d'une base orthonormale quelconque d'un espace hilbertien E est appelé la dimension hilbertienne de E.

#### Corollaire 1 {#evt-v-s2-prop-7-cor-1 .statement}

Étant données deux bases orthonormales dans un espace hilbertien E, il existe un automorphisme de E transformant la première base en la seconde.

#### Corollaire 2 {#evt-v-s2-prop-7-cor-2 .statement}

Pour que les espaces hilbertiens $\ell^2(I)$ et $\ell^2(J)$ soient isomorphes, il faut et il suffit que I et J soient équipotents.

## EXERCICES {#evt-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
