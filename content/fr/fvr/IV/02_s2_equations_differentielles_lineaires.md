---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: ÉQUATIONS DIFFÉRENTIELLES
section: 2
section_title: Équations différentielles linéaires
lang: fr
source: fvr-i-vii-fr
book_pages: FVR IV.16-FVR IV.36, FVR IV.41-FVR IV.43
pdf_pages: 0175-0195, 0200-0202
extraction: ocr
subsections:
    - "no": 1
      title: Existence des intégrales d’une équation différentielle linéaire
      page: 16
      pdf_page: 175
    - "no": 2
      title: Linéarité des intégrales d’une équation différentielle linéaire
      page: 18
      pdf_page: 177
    - "no": 3
      title: Intégration de l’équation linéaire non homogène
      page: 20
      pdf_page: 179
    - "no": 4
      title: Systèmes fondamentaux d’intégrales d’un système linéaire d’équations différentielles scalaires
      page: 21
      pdf_page: 180
    - "no": 5
      title: Équation adjointe
      page: 25
      pdf_page: 184
    - "no": 6
      title: Équations différentielles linéaires à coefficients constants
      page: 26
      pdf_page: 185
    - "no": 7
      title: Équations linéaires d’ordre $n$
      page: 30
      pdf_page: 189
    - "no": 8
      title: Equations linéaires d’ordre $n$ à coefficients constants
      page: 33
      pdf_page: 192
    - "no": 9
      title: Systèmes d'équations linéaires à coefficients constants
      page: 35
      pdf_page: 194
statements: 21
exercises: 10
content_sha256: 3cc2c19d687fdf68937ab5da650a65a2b8b4a4035eaea77aaf7953b28d5a81e8
---

## § 2. ÉQUATIONS DIFFÉRENTIELLES LINÉAIRES

### 1. Existence des intégrales d’une équation différentielle linéaire

Soient E un espace normé complet sur le corps $\mathbf{R}$, J un intervalle dans $\mathbf{R}$, non réduit à un point. On dit qu’une équation différentielle
$$
\frac{dx}{dt} = f(t, x)
$$
où $f$ est définie dans $J \times E$, est une équation linéaire si, pour tout $t \in J$, l’application $x \mapsto f(t, x)$ est une application linéaire affine continue¹ de E dans lui-même; si on pose $b(t) = f(t, 0)$, l’application $x \mapsto f(t, x) - f(t, 0) = f(t, x) - b(t)$ est donc une application linéaire continue de E dans lui-même; nous désignons désormais cette application par $A(t)$, et nous noterons $A(t).x$ (ou simplement $A(t)x$) sa valeur en un point $x \in E$; l’équation différentielle linéaire (1) s’écrit donc

¹ Rappelons que si E est de dimension finie, toute application linéaire affine de E dans lui-même est continue (TG, VI, p. 3 et 6).

(2)
$$
\frac{d\mathbf{x}}{dt} = A(t) \cdot \mathbf{x} + \mathbf{b}(t)
$$
où $\mathbf{b}$ est une application de $J$ dans $E$; lorsque $\mathbf{b} = 0$, on dit que l'équation différentielle linéaire (2) est *homogène*.

#### Exemple 1 {#fvr-iv-s2-n1-exa-1 .statement}

Lorsque $E$ est de dimension finie $n$ sur $\mathbf{R}$, on peut identifier l'endomorphisme $A(t)$ à sa *matrice* $(a_{ij}(t))$ *par rapport à une base* (quelconque) de $E$ (A, II, p. 144); lorsqu'on identifie un vecteur $\mathbf{x} \in E$ à la matrice à une colonne $(x_i)$ de ses composantes par rapport à la base de $E$ considérée, l'écriture $A(t) \cdot \mathbf{x}$ de la valeur de l'application linéaire homogène $A(t)$ au point $\mathbf{x}$ est bien conforme aux conventions générales d'Algèbre (A, II, p. 144, prop. 2). Dans ce cas, l'équation (2) est équivalente au système d'équations différentielles scalaires
$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \quad (1 \leq i \leq n).
$$
2) Soient $G$ une *algèbre normée complète* sur $\mathbf{R}$, $\mathbf{a}(t)$, $\mathbf{b}(t)$ et $\mathbf{c}(t)$, trois applications de $J$ dans $G$; l'équation
$$
\frac{d\mathbf{x}}{dt} = \mathbf{a}(t)\mathbf{x} + \mathbf{x}\mathbf{b}(t) + \mathbf{c}(t)
$$
est une équation différentielle linéaire; $A(t)$ est ici l'application linéaire $\mathbf{x} \mapsto \mathbf{a}(t)\mathbf{x} + \mathbf{x}\mathbf{b}(t)$ de $G$ dans elle-même.

Pour tout $t \in J$, $A(t)$ est un élément de l'ensemble $\mathcal{L}(E)$ des applications linéaires continues de $E$ dans lui-même (endomorphismes continus de $E$); on sait (TG, X, p. 24) que $\mathcal{L}(E)$, muni de la *norme* $\|U\| = \sup_{\|\mathbf{x}\|=1} \|U.\mathbf{x}\|$ est une *algèbre normée complète* sur le corps $\mathbf{R}$ et que l'on a $\|UV\| \leq \|U\| \cdot \|V\|$.

Dans tout ce paragraphe, nous supposerons que les conditions suivantes sont satisfaites:
a) *L'application* $t \mapsto A(t)$ *de J dans* $\mathcal{L}(E)$ *est réglée*.
b) *L'application* $t \mapsto \mathbf{b}(t)$ *de J dans* $E$ *est réglée*.

Lorsque $E$ est de dimension $n$, $\mathcal{L}(E)$ est isomorphe à $\mathbf{R}^{n^2}$ (en tant qu'espace vectoriel topologique) et la condition a) signifie que chacun des éléments $a_{ij}(t)$ de la matrice $A(t)$ est une fonction *réglée* dans $J$.

Comme on a $\|A(t')\mathbf{x} - A(t)\mathbf{x}\| \leq \|A(t') - A(t)\| \cdot \|\mathbf{x}\|$, l'application
$$
t \mapsto A(t) \cdot \mathbf{x} + \mathbf{b}(t)
$$
est *réglée* pour tout $\mathbf{x} \in E$; en outre, on a
$$
\|A(t)\mathbf{x}_1 - A(t)\mathbf{x}_2\| = \|A(t)(\mathbf{x}_1 - \mathbf{x}_2)\| \leq \|A(t)\| \cdot \|\mathbf{x}_1 - \mathbf{x}_2\|
$$
quels que soient $t \in J$, $\mathbf{x}_1$ et $\mathbf{x}_2$ dans $E$; en d'autres termes, le second membre de (2) satisfait aux conditions du lemme 1 de IV, p. 3, et est *lipschitzien* pour la fonction *réglée* $\|A(t)\|$ dans $J \times E$. Par suite (IV, p. 12, cor. 2):

#### Théorème 1 {#fvr-iv-s2-thm-1 .statement}

*Soient* $t \mapsto A(t)$ *une application réglée de J dans* $\mathcal{L}(E)$, $t \mapsto \mathbf{b}(t)$ *une application réglée de J dans* $E$. *Pour tout point* $(t_0, \mathbf{x}_0)$ *de* $J \times E$, *l'équation linéaire* (2) *admet une solution et une seule*, définie dans $J$ tout entier et égale à $\mathbf{x}_0$ *au point* $t_0$.

### 2. Linéarité des intégrales d’une équation différentielle linéaire

La résolution d’une équation différentielle linéaire (2) est un problème linéaire (A, II, p. 48); l’équation linéaire homogène

$$
\frac{d\mathbf{x}}{dt} = A(t) \cdot \mathbf{x}
$$

est dite associée à l’équation non homogène (2); on sait alors (A, II, p. 48, prop. 14) que si $\mathbf{u}_1$ est une intégrale de l’équation non homogène (2), toute intégrale de cette équation est de la forme $\mathbf{u} + \mathbf{u}_1$ où $\mathbf{u}$ est une intégrale de l’équation homogène associée (4), et réciproquement. Nous allons d’abord étudier dans ce n° les intégrales d’une équation homogène (4).

#### Proposition 1 {#fvr-iv-s2-prop-1 .statement}

L’ensemble $\mathcal{I}$ des intégrales de l’équation linéaire homogène (4), définies dans $J$, est un sous-espace vectoriel de l’espace $\mathcal{C}(J; E)$ des applications continues de $J$ dans $E$.

La démonstration est immédiate.

#### Théorème 2 {#fvr-iv-s2-thm-2 .statement}

Pour tout point $(t_0, \mathbf{x}_0)$ de $J \times E$, soit $\mathbf{u}(t, t_0, \mathbf{x}_0)$ l’intégrale de l’équation homogène (4), définie dans $J$ et égale à $\mathbf{x}_0$ au point $t_0$.

1° Pour tout point $t \in J$, l’application $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ est une application linéaire bijective et bicontinue $C(t, t_0)$ de $E$ sur lui-même.

2° L’application $t \mapsto C(t, t_0)$ de $J$ dans $\mathcal{L}(E)$ est identique à l’intégrale de l’équation différentielle linéaire homogène

$$
\frac{dU}{dt} = A(t)U
$$

qui prend la valeur $I$ (application identique de $E$ sur lui-même) au point $t_0$.

3° Quels que soient les points $s, t, u$ de $J$, on a

$$
C(s, u) = C(s, t)C(t, u), \qquad C(s, t) = (C(t, s))^{-1}.
$$

D’après la prop. 1, $\mathbf{u}(t, t_0, \mathbf{x}_1) + \mathbf{u}(t, t_0, \mathbf{x}_2)$ (resp. $\lambda \mathbf{u}(t, t_0, \mathbf{x}_0)$) est une intégrale de (4) et prend au point $t_0$ la valeur $\mathbf{x}_1 + \mathbf{x}_2$ (resp. $\lambda \mathbf{x}_0$), donc, en vertu du th. 1 de IV, p. 17 elle est identique à $\mathbf{u}(t, t_0, \mathbf{x}_1 + \mathbf{x}_2)$ (resp. $\mathbf{u}(t, t_0, \lambda \mathbf{x}_0)$); l’application $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ est donc une application linéaire $C(t, t_0)$ de $E$ dans lui-même, et on peut écrire $\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0) \cdot \mathbf{x}_0$.

Comme l’application $(X, Y) \mapsto XY$ de $\mathcal{L}(E) \times \mathcal{L}(E)$ dans $\mathcal{L}(E)$ est continue (TG, X, p. 23, prop. 8), l’application $t \mapsto A(t)U$ de $J$ dans $\mathcal{L}(E)$ est réglée pour tout $U \in \mathcal{L}(E)$; on a en outre (TG, X, p. 21)

$$
\|A(t)X - A(t)Y\| = \|A(t)(X - Y)\| \leq \|A(t)\|\cdot\|X - Y\|,
$$

donc on peut appliquer à l’équation linéaire homogène (5) le th. 1 de IV, p. 17; soit $V(t)$ l’intégrale de cette équation définie dans $J$ et égale à $I$ au point $t_0$. On a (I, p. 14, prop. 3)
$$
\frac{d}{dt} (V(t) \cdot \mathbf{x}_0) = \frac{dV(t)}{dt} \cdot \mathbf{x}_0 = A(t) \cdot (V(t) \cdot \mathbf{x}_0)
$$
et pour $t = t_0$, $V(t_0) \cdot \mathbf{x}_0 = I \cdot \mathbf{x}_0 = \mathbf{x}_0$; d’après le th. 1 de IV, p. 17), on a nécessairement $V(t) \cdot \mathbf{x}_0 = C(t, t_0) \cdot \mathbf{x}_0$ pour tout $\mathbf{x}_0 \in E$, c’est-à-dire $V(t) = C(t, t_0)$; ceci démontre que $C(t, t_0)$ appartient à $\mathcal{L}(E)$, autrement dit, que $\mathbf{x}_0 \mapsto C(t, t_0) \cdot \mathbf{x}_0$ est continue dans $E$, et que l’application $t \mapsto C(t, t_0)$ est l’intégrale de (5) égale à $I$ au point $t_0$.

Enfin, l’intégrale $s \mapsto C(s, u) \cdot \mathbf{x}_0$ de (4) est égale à $C(t, u) \cdot \mathbf{x}_0$ au point $t$, donc on a, par définition
$$
C(s, u) \cdot \mathbf{x}_0 = C(s, t) \cdot (C(t, u) \cdot \mathbf{x}_0) = (C(s, t)C(t, u)) \cdot \mathbf{x}_0
$$
quel que soit $\mathbf{x}_0 \in E$, d’où la première relation (6); comme $C(s, s) = I$, on a $C(s, t)C(t, s) = I$ quels que soient $s$ et $t$ dans $J$; ceci prouve (E, II, p. 18, corollaire) que $C(t, t_0)$ est une application bijective de $E$ sur lui-même, dont l’application réciproque est $C(t_0, t)$. Le théorème est ainsi complètement démontré.

On dit que $C(t, t_0)$ est la résolvante de l’équation (2) de IV, p. 17.

#### Corollaire 1 {#fvr-iv-s2-thm-2-cor-1 .statement}

L’application qui, à tout point $\mathbf{x}_0 \in E$, fait correspondre la fonction continue $t \mapsto C(t, t_0) \cdot \mathbf{x}_0$, définie dans $J$, est un isomorphisme de l’espace normé $E$ sur l’espace vectoriel $\mathscr{I}$ des intégrales de (4), muni de la topologie de la convergence compacte.

C’est en effet une application linéaire bijective de $E$ sur $\mathscr{I}$; dans un ensemble compact $K \subset J$, $C(t, t_0)$ est bornée, donc on a $\|C(t, t_0) \cdot \mathbf{x}_0\| \leq M \|\mathbf{x}_0\|$ quels que soient $t \in K$ et $\mathbf{x}_0 \in E$, ce qui prouve la continuité de l’application considérée; comme
$$
C(t_0, t_0) \cdot \mathbf{x}_0 = \mathbf{x}_0,
$$
il est évident que son application réciproque est aussi continue.

#### Corollaire 2 {#fvr-iv-s2-thm-2-cor-2 .statement}

L’application $(s, t) \mapsto C(s, t)$ de $J \times J$ dans $\mathcal{L}(E)$ est continue.

En effet, on a, d’après (6), $C(s, t) = C(s, t_0)(C(t, t_0))^{-1}$; or, l’application $(X, Y) \mapsto XY$ de $\mathcal{L}(E) \times \mathcal{L}(E)$ dans $\mathcal{L}(E)$ est continue, et il en est de même de l’application $X \mapsto X^{-1}$ du groupe (ouvert) des éléments inversibles de $\mathcal{L}(E)$ sur lui-même (TG, IX, p. 40, prop. 14).

On notera que l’application
$$
t \mapsto C(t_0, t) = (C(t, t_0))^{-1}
$$
admet (dans le complémentaire d’un ensemble dénombrable) une dérivée égale à $- (C(t, t_0))^{-1} \frac{dC(t, t_0)/dt}{(C(t, t_0))^{-1}}$ (I, p. 16, prop. 4), c’est-à-dire (d’après IV, p. 18, la formule (5)) à $- C(t_0, t)A(t)$.

#### Corollaire 3 {#fvr-iv-s2-thm-2-cor-3 .statement}

Soit $K$ un intervalle compact contenu dans $J$, et soit $k = \sup_{t \in K} \|A(t)\|$.
Quels que soient $t$ et $t_0$ dans $K$, on a
$$
\|C(t, t_0) - I\| \leq e^{k|t-t_0|} - 1.
$$

En effet, on a $\|A(t)x_0\| \leq k\|x_0\|$ pour tout $t \in K$; dans $K$, la fonction constante égale à $x_0$ est donc une intégrale approchée à $k\|x_0\|$ près de l’équation (4) de IV, p. 18; d’après la formule (15) de IV, p. 9, on a donc
$$
\|C(t, t_0)x_0 - x_0\| \leq \|x_0\|\ (e^{k|t-t_0|} - 1)
$$
quels que soient $t$ et $t_0$ dans $K$, et $x_0$ dans $E$, ce qui équivaut à l’inégalité (7) d’après la définition de la norme dans $\mathscr{L}(E)$.

#### Proposition 2 {#fvr-iv-s2-prop-2 .statement}

*Soit B un endomorphisme continu de E, indépendant de t, et permutable avec A(t) pour tout t \in J; alors B est permutable avec C(t, t_0) quels que soient t et t_0 dans J.*

En effet, on a, d’après (5)
$$
\frac{d}{dt}\,(BC) = BAC = ABC \quad \text{et} \quad \frac{d}{dt}\,(CB) = ACB,
$$
donc $\frac{d}{dt}\,(BC - CB) = A(BC - CB)$; mais $BC(t_0, t_0) - C(t_0, t_0)\,B = 0$, donc (IV, p. 17, th. 1) $BC(t, t_0) - C(t, t_0)\,B = 0$ pour tout $t \in J$.

Un cas particulier important de la prop. 2 est celui où $E$ est muni d’une structure d’espace vectoriel normé par rapport au *corps des nombres complexes* $\mathbf{C}$, et où, pour tout $t \in J$, $A(t)$ est un endomorphisme de $E$ pour cette structure d’espace vectoriel; cela signifie que $A(t)$ est permutable avec l’endomorphisme continu $x \mapsto ix$ de $E$ (pour la structure d’espace vectoriel *sur* $\mathbf{R}$); donc $C(t, t_0)$ est permutable avec cet endomorphisme, ce qui signifie que, quels que soient $t$ et $t_0$ dans $J$, $C(t, t_0)$ est un endomorphisme continu de la structure d’espace vectoriel normé de $E$ sur $\mathbf{C}$.

### 3. Intégration de l’équation linéaire non homogène

L’intégration de l’équation linéaire non homogène
$$
\frac{dx}{dt} = A(t)\cdot x + b(t)
$$
se ramène à l’intégration de l’équation homogène associée
$$
\frac{dx}{dt} = A(t)\cdot x
$$
et au calcul d’une primitive. Avec les notations du th. 2 de IV, p. 18, posons en effet $x = C(t, t_0)\cdot z$, d’où on tire, d’après la seconde formule (6) de IV, p. 18, $z = C(t_0, t)\cdot x$; si $x$ est une intégrale de (2), $z$ est une intégrale de l’équation
$$
\frac{d}{dt}\,(C(t, t_0)\cdot z) = A(t)C(t, t_0)\cdot z + b(t);
$$
comme l’application bilinéaire
$$
(U, y) \mapsto U.y
$$
de $\mathscr{L}(E) \times E$ dans $E$ est continue (TG, X, p. 23, prop. 6), $z$ admet une dérivée (sauf en un ensemble dénombrable de points de $J$) et on a, par la formule de dérivation d’une fonction bilinéaire (I, p. 5, prop. 3)

$$
\frac{d}{dt} (C(t, t_0) \cdot \mathbf{z}) = \frac{dC(t, t_0)}{dt} \cdot \mathbf{z} + C(t, t_0) \cdot \frac{d\mathbf{z}}{dt} = A(t)C(t, t_0) \cdot \mathbf{z} + C(t, t_0) \cdot \frac{d\mathbf{z}}{dt}
$$

(en remplaçant $dC(t, t_0)/dt$ par $A(t)C(t, t_0)$, en vertu de (5) (IV, p. 18)). L’équation en $\mathbf{z}$ se réduit donc à $C(t, t_0) \cdot d\mathbf{z}/dt = \mathbf{b}(t)$, ou encore à

$$
\frac{d\mathbf{z}}{dt} = C(t_0, t) \cdot \mathbf{b}(t)
$$

d’après la seconde formule (6) de IV, p. 18. Or, le second membre de l’équation (8) est une fonction réglée dans $J$, étant obtenue en substituant des fonctions réglées à $U$ et $y$ dans la fonction bilinéaire continue $U.y$ (cf. II, p. 6, cor. 2); l’équation (8) a donc une intégrale et une seule prenant la valeur $\mathbf{x}_0$ au point $t_0$, donnée par la formule

$$
\mathbf{z}(t) = \mathbf{x}_0 + \int_{t_0}^t C(t_0, s) \cdot \mathbf{b}(s) \, ds.
$$

Comme on a $C(t, t_0) \cdot \int_{t_0}^t C(t_0, s) \cdot \mathbf{b}(s) \, ds = \int_{t_0}^t C(t, t_0)C(t_0, s) \cdot \mathbf{b}(s) \, ds$ (II, p. 10, formule (9)), on obtient (en tenant compte de la première formule (6) de IV, p. 18) le résultat suivant:

#### Proposition 3 {#fvr-iv-s2-prop-3 .statement}

*Avec les notations du th. 2 (IV, p. 18), pour tout point $(t_0, \mathbf{x}_0)$ de $J \times E$, l’intégrale de l’équation linéaire (2) définie dans $J$ et égale à $\mathbf{x}_0$ au point $t_0$, est donnée par la formule*

$$
\mathbf{u}(t) = C(t, t_0) \cdot \mathbf{x}_0 + \int_{t_0}^t C(t, s) \cdot \mathbf{b}(s) \, ds.
$$

La méthode qui conduit à la formule (10), et qui consiste à prendre la fonction $\mathbf{z}$ comme nouvelle fonction inconnue, est souvent appelée « méthode de variation des constantes ».

### 4. Systèmes fondamentaux d’intégrales d’un système linéaire d’équations différentielles scalaires

Nous allons considérer dans ce n° et le suivant le cas où $E$ est un espace vectoriel de dimension finie $n$ par rapport au corps $C$ des nombres complexes (donc de dimension $2n$ par rapport à $\mathbf{R}$), et où pour tout $t \in J$, $A(t)$ est un endomorphisme de $E$ *pour la structure d’espace vectoriel sur $C$*. On peut alors identifier $A(t)$ à sa matrice $(a_{ij}(t))$ par rapport à une base de $E$ (sur le corps $C$), les $a_{ij}$ étant cette fois $n^2$ fonctions *complexes* définies et réglées dans $J$; $x_j$ $(1 \leq j \leq n)$ désignant les composantes (complexes) d’un vecteur $\mathbf{x} \in E$ par rapport à la base considérée, l’équation linéaire

$$
\frac{d\mathbf{x}}{dt} = A(t) \cdot \mathbf{x} + \mathbf{b}(t)
$$

est encore équivalente au système

(3) $$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \quad (1 \leq i \leq n).
$$

Les th. 1 (IV, p. 17) et 2 (IV, p. 18) et la prop. 2 (IV, p. 20) montrent alors que, pour tout $x_0 = (x_{k0})_{1 \leq k \leq n}$ dans E, il existe une intégrale et une seule $\mathbf{u} = (u_k)_{1 \leq k \leq n}$ de l’équation

(4) $$
\frac{d\mathbf{x}}{dt} = A(t) \cdot \mathbf{x}
$$

définie dans E et égale à $\mathbf{x}_0$ au point $t_0$; cette intégrale peut s’écrire

$$
\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0) \cdot \mathbf{x}_0,
$$

$C(t, t_0)$ étant une matrice carrée *inversible* ($c_{ij}(t, t_0)$) d’ordre n, dont les coefficients sont des fonctions complexes continues dans $J \times J$ et telles que $t \mapsto c_{ij}(t, t_0)$ soit une primitive de fonction réglée dans J.

Dans le cas particulier où $n = 1$, le système (3) se réduit à une seule équation scalaire

(11) $$
\frac{dx}{dt} = a(t)x + b(t)
$$

$(a(t)$ et $b(t)$ fonctions complexes réglées dans J); on vérifie aussitôt que la matrice (à un élément) $C(t, t_0)$ est égale à $\exp \left( \int_{t_0}^t a(s) \, ds \right)$; l’intégrale de (11) égale à $x_0$ au point $t_0$ est donc donnée explicitement par la formule

(12) $$
u(t) = x_0 \exp \left( \int_{t_0}^t a(s) \, ds \right) + \int_{t_0}^t b(s) \exp \left( \int_{t_0}^s a(\tau) \, d\tau \right) ds.
$$

Dans l’espace $\mathcal{C}(J; E)$ des applications continues de J dans E, muni de la topologie de la convergence compacte, l’ensemble $\mathscr{I}$ des intégrales de l’équation (4) est un sous-espace vectoriel (sur $\mathbf{C}$) *isomorphe* à E, donc à $\mathbf{C}^n$ (IV, p. 19, cor. 1, et IV, p. 20, prop. 2). On appelle *système fondamental* d’intégrales de (4) une *base* $(\mathbf{u}_i)_{1 \leq j \leq n}$ de cet espace (sur le corps $\mathbf{C}$).

#### Proposition 4 {#fvr-iv-s2-prop-4 .statement}

*Pour que n intégrales $\mathbf{u}_j$ ($1 \leq j \leq n$) de l’équation (4) forment un système fondamental, il faut et il suffit que leurs valeurs $\mathbf{u}_j(t_0)$ en un point $t_0 \in J$ soient des vecteurs linéairement indépendants dans E.*

En effet, l’application qui, à tout $\mathbf{x}_0 \in E$, fait correspondre l’intégrale $t \mapsto C(t, t_0) \cdot \mathbf{x}_0$, est un isomorphisme de E sur $\mathscr{I}$ (IV, p. 19, cor. 1 et IV, p. 20, prop. 2).

Si $(\mathbf{e}_j)_{1 \leq j \leq n}$ est une base quelconque de E sur $\mathbf{C}$, les n intégrales

$$
\mathbf{u}_j(t) = C(t, t_0) \cdot \mathbf{e}_j \quad (1 \leq j \leq n)
$$

forment donc un système fondamental; si on identifie $C(t, t_0)$ à sa matrice par rapport à la base $(\mathbf{e}_j)$, les intégrales $\mathbf{u}_j$ ne sont autres que les colonnes de la matrice $C(t, t_0)$. L’intégrale de (4) prenant au point $t_0$ la valeur $\mathbf{x}_0 = \sum_{j=1}^n \lambda_j \mathbf{e}_j$ est alors
$$
C(t, t_0) \cdot \mathbf{x}_0 = \sum_{k=1}^n \lambda_k \mathbf{u}_k(t).
$$

Étant données $n$ intégrales quelconques $\mathbf{u}_j$ ($1 \leq j \leq n$) de (4), on appelle déterminant de ces $n$ intégrales en un point $t \in J$, par rapport à une base $(\mathbf{e}_j)_{1 \leq j \leq n}$ de E, le déterminant
$$
\Delta(t) = (\mathbf{u}_1(t), \mathbf{u}_2(t), \ldots, \mathbf{u}_n(t))
$$
des $n$ vecteurs $\mathbf{u}_j(t)$ par rapport à la base $(\mathbf{e}_j)$ (A, III, p. 90). On a (A, III, p. 91, prop. 2)
$$
\Delta(t) = \Delta(t_0) \det (C(t, t_0)).
$$

D’après la prop. 4 de IV, p. 22, pour que $(\mathbf{u}_j)_{1 \leq j \leq n}$ soit un système fondamental d’intégrales de (4), il faut et il suffit que le déterminant $\Delta(t)$ des $\mathbf{u}_j$ soit $\neq 0$ en un point $t_0$ de $J$; la formule (14) montre alors de nouveau que $\Delta(t) \neq 0$ en tout point de $J$, autrement dit que les vecteurs $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) sont toujours linéairement indépendants.

#### Proposition 5 {#fvr-iv-s2-prop-5 .statement}

*Le déterminant de la matrice $C(t, t_0)$ est donné par la formule*
$$
\det (C(t, t_0)) = \exp \left( \int_{t_0}^t \operatorname{Tr}(A(s)) \, ds \right).
$$

En effet, si on pose $\delta(t) = \det (C(t, t_0))$, on a, d’après la formule donnant la dérivée d’un déterminant (I, p. 8, formule (3))
$$
\frac{d\delta}{dt} = \operatorname{Tr} \left( \frac{dC(t, t_0)}{dt} (C(t, t_0))^{-1} \right) \delta(t)
$$
c’est-à-dire, en vertu de l’équation différentielle (5) de IV, p. 18 à laquelle satisfait $C(t, t_0)$
$$
\frac{d\delta}{dt} = \operatorname{Tr}(A(t)) \, \delta(t).
$$

Comme $\delta(t_0) = 1$, la formule (15) se déduit de l’expression (12) (IV, p. 22) de l’intégrale d’une équation linéaire scalaire.

La donnée de $n$ intégrales linéairement indépendantes de (4) détermine toutes les intégrales de cette équation, comme nous venons de le voir. Nous allons maintenant montrer que pour, $1 \leq p \leq n$, la donnée de $p$ intégrales linéairement indépendantes $\mathbf{u}_j$ ($1 \leq j \leq p$) de l’équation (4) ramène l’intégration de cette équation à celle d’un système linéaire homogène de $n - p$ équations scalaires. Supposons que, dans un intervalle $K \subset J$, il existe $n - p$ applications
$$
\mathbf{u}_{p+k} \quad (1 \leq k \leq n-p)
$$
de $K$ dans $E$, primitives de fonctions réglées dans $K$, et telles que, pour tout $t \in K$, les $n$ vecteurs $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) forment une base de $E$.

Pour tout point $t_1 \in J$, il existe toujours un intervalle $K$, voisinage de $t_1$ dans $J$, dans lequel sont définies $n - p$ fonctions $\mathbf{u}_{p+k}$ ($1 \leq k \leq n-p$) ayant les propriétés précédentes. En effet, soit $(\mathbf{e}_i)_{1 \leq i \leq n}$ une base de $E$; il existe $n - p$ vecteurs de cette base qui forment avec les $\mathbf{u}_j(t_1)$ ($1 \leq j \leq p$) une base de $E$ (A, II, p. 95, th. 2); supposons par exemple que ce soient $\mathbf{e}_{p+1}, \ldots, \mathbf{e}_n$; comme le déterminant $\det(\mathbf{u}_1(t), \ldots, \mathbf{u}_p(t), \mathbf{e}_{p+1}, \ldots, \mathbf{e}_n)$ (par rapport à la base $(\mathbf{e}_i)$) est fonction continue de $t$ et n’est pas nul pour $t = t_1$, il existe un voisinage $K$ de $t_1$ dans lequel il n’est pas nul; on peut donc prendre $\mathbf{u}_{p+k}(t) = \mathbf{e}_{p+k}$ ($1 \leq k \leq n-p$) pour $t \in K$.

Il existe une matrice inversible $B(t)$ d’ordre $n$, dont les éléments sont des primitives de fonctions réglées dans $K$, telle que $B(t) \cdot \mathbf{e}_j = \mathbf{u}_j(t)$ pour $1 \leq j \leq n$. Posons $\mathbf{x} = B(t) \cdot \mathbf{y}$; $\mathbf{y}$ satisfait à l’équation
$$
\frac{dB}{dt} \cdot \mathbf{y} + B(t) \cdot \frac{d\mathbf{y}}{dt} = A(t)B(t) \cdot \mathbf{y},
$$
qui s’écrit aussi
$$
\frac{d\mathbf{y}}{dt} = (B(t))^{-1}\left(A(t)B(t) - \frac{dB}{dt}\right) \cdot \mathbf{y} = H(t) \cdot \mathbf{y},
$$
où $H(t) = (h_{jk}(t))$ est une matrice à coefficients réglés dans $K$. D’après la définition de $B(t)$, cette équation linéaire admet les $p$ vecteurs constants $\mathbf{e}_j$ ($1 \leq j \leq p$) comme intégrales; on en conclut aussitôt qu’on a nécessairement $h_{jk}(t) = 0$ pour $1 \leq k \leq p$; les composantes $y_k$ de $\mathbf{y}$ (par rapport à la base $(\mathbf{e}_i)$) d’indice $k \geq p + 1$ satisfont donc à un système linéaire homogène de $n - p$ équations; une fois déterminées les solutions de ce système, les $dy_j/dt$ d’indice $j \leq p$ sont fonctions linéaires des $y_k$ d’indice $k \geq p + 1$, donc sont connues, et les primitives de ces fonctions donneront les $y_j$ d’indice $j \leq p$.

En particulier, lorsqu’on connaît $n - 1$ intégrales linéairement indépendantes de l’équation (4) de IV, p. 22, l’intégration de cette équation est ramenée à celle d’une seule équation scalaire homogène, et par suite au calcul de $n$ primitives.

#### Remarque 1 {#fvr-iv-s2-n4-rem-1 .statement}

Tout ce qui précède s’applique encore au cas où $E$ est de dimension $n$ sur le corps $\mathbf{R}$ et $A(t)$ un endomorphisme de $E$ pour tout $t \in J$: il suffit de remplacer partout $\mathbf{C}$ par $\mathbf{R}$.
2) Soit $A(t) = (a_{ij}(t))$ une matrice carrée d’ordre $n$ dont les éléments sont des fonctions réglées réelles (resp. complexes) de $t$ dans $J$, et soit $C(t, t_0) = (c_{ij}(t, t_0))$ la matrice résolvante du système linéaire (3) (IV, p. 22) correspondant. Soit $F$ un espace normé complet quelconque sur $\mathbf{R}$ (resp. $\mathbf{C}$) et considérons le système d’équations différentielles linéaires
$$
\frac{dy_i}{dt} = \sum_{j=1}^n a_{ij}(t)y_j,
$$
où les fonctions inconnues $y_j$ prennent leurs valeurs dans $F$. Il est immédiat que la solution (u_j)_{1 \leq j \leq n} de ce système telle que $u_j(t_0) = d_j$ pour $1 \leq j \leq n$ ($d_j$ arbitraires dans $\mathbf{F}$) est donnée par les formules

$$
u_i(t) = \sum_{j=1}^n c_{ij}(t, t_0) d_j \quad (1 \leq i \leq n).
$$

Considérons en particulier le cas où $A(t)$ est un endomorphisme d'un espace vectoriel $E$ de dimension finie $n$ sur $\mathbf{C}$, tel qu'il existe une base de $E$ par rapport à laquelle la matrice de $A(t)$ ait ses éléments réels pour tout $t \in J$. Alors ce qui précède montre (en vertu du th. 1 de IV, p. 17) que la matrice résolvante $C(t, t_0)$ par rapport à la même base a aussi ses éléments réels : il suffit en effet de considérer l'espace vectoriel $E_0$ sur $\mathbf{R}$ engendré par la base de $E$ considérée, et de remarquer que la restriction de $A(t)$ à $E_0$ est un endomorphisme de cet espace vectoriel.

### 5. Équation adjointe

L'espace $E$ étant toujours supposé être de dimension *finie* $n$ sur le corps $\mathbf{C}$, soit $E^*$ son *dual* (A, II, p. 40), qui est un espace de dimension $n$ sur $\mathbf{C}$ (A, II, p. 102, th. 4) ; la forme bilinéaire canonique $\langle x, x^* \rangle$ définie dans $E \times E^*$ (A, II, p. 41) est *continue* dans ce produit (étant un polynôme par rapport aux composantes de $x \in E$ et de $x^* \in E^*$).

Étant donnée une équation linéaire homogène (4) (IV, p. 22), où $t \mapsto A(t)$ est une application réglée de $J$ dans $\mathcal{L}(E)$, cherchons s'il existe une application $t \mapsto v(t)$ de $J$ dans $E^*$, primitive d'une fonction réglée dans $J$, et telle que la fonction numérique $t \mapsto \langle u(t), v(t) \rangle$ soit *constante* dans $J$ lorsque $u$ est une solution quelconque de (4) ; il revient au même d'écrire que la dérivée de cette fonction doit être nulle en tout point où $u$ et $v$ sont dérivables, c'est-à-dire qu'on doit avoir en ces points

$$
\left\langle \frac{du}{dt}, v(t) \right\rangle + \left\langle u(t), \frac{dv}{dt} \right\rangle = 0.
$$

Or, d'après (4), on a $\left\langle \frac{du}{dt}, v(t) \right\rangle = \langle A(t) \cdot u(t), v(t) \rangle = -\langle u(t), B(t) \cdot v(t) \rangle$

où $-B(t)$ est la *transposée* de $A(t)$ (A, II, p. 42). La relation à laquelle doit satisfaire $v$ s'écrit donc

$$
\left\langle u(t), \frac{dv}{dt} - B(t) \cdot v(t) \right\rangle = 0
$$

en tous les points où $A(t)$ est continue et $v(t)$ dérivable. Or, pour un tel point $t$ et un point $x_0 \in E$ *arbitraire*, il existe d'après le th. 1 de IV, p. 17, une solution $u$ de (4) telle que $u(t) = x_0$; on doit donc avoir $\left\langle x_0, \frac{dv}{dt} - B(t) \cdot v(t) \right\rangle = 0$ pour *tout* $x_0 \in E$, ce qui signifie que $\frac{dv}{dt} - B(t) \cdot v(t) = 0$. Par suite:

#### Proposition 6 {#fvr-iv-s2-prop-6 .statement}

*Pour qu'une application* $t \mapsto v(t)$ *de* $J$ *dans* $E^*$, *primitive d'une fonction réglée dans* $J$, *soit telle que* $\langle u(t), v(t) \rangle$ *soit constante dans* $J$ *pour toute solution* $u$ *de* l’équation (4) de IV, p. 22, il faut et il suffit que $\mathbf{v}$ soit solution de l’équation linéaire homogène

$$
\frac{d\mathbf{x}}{dt} = B(t) . \mathbf{x}
$$

où $-B(t)$ est la transposée de $A(t)$.

L’équation (16) est dite adjointe de (4); il est clair qu’inversement (4) est adjointe de (16). Les éléments de la matrice $B(t)$ étant fonctions réglées de $t$ dans $J$, les résultats obtenus ci-dessus sur les équations linéaires sont applicables à l’équation (16). En particulier, l’intégrale de (16) prenant la valeur $x_0^*$ au point $t_0$ peut s’écrire $H(t, t_0) . x_0^*$, où $H(t, t_0)$ est une application linéaire bijective de $E^*$ sur lui-même, identique à l’intégrale de l’équation

$$
\frac{dV}{dt} = B(t)V
$$

qui prend la valeur $I$ au point $t_0$. Il en résulte qu’on a (avec les notations de IV, p. 18)

$$
\langle C(t, t_0) . x_0, H(t, t_0) . x_0^* \rangle = \langle x_0, x_0^* \rangle
$$

quels que soient $x_0 \in E$ et $x_0^* \in E^*$, ce qui montre que

$$
H(t, t_0) = \tilde{C}(t, t_0)
$$

(contragrédiente de $C(t, t_0)$). En particulier, si on connaît un système fondamental d’intégrales de l’équation adjointe (16), la matrice $H(t, t_0)$ est déterminée, donc aussi $C(t, t_0)$, et par suite toutes les intégrales de l’équation (4).

#### Remarque {#fvr-iv-s2-n5-rem-1 .statement}

Soient $E$ et $F$ deux espaces normés complets sur $\mathbf{R}$ (ou sur $\mathbf{C}$), $(\mathbf{x}, \mathbf{y}) \mapsto \langle \mathbf{x}, \mathbf{y} \rangle$ une forme bilinéaire continue dans $E \times F$, telle que la relation « $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ pour tout $\mathbf{y} \in F$ » (resp. « $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ pour tout $\mathbf{x} \in E$ ») entraîne $\mathbf{x} = 0$ (resp. $\mathbf{y} = 0$). Supposons en outre que, pour tout $t \in J$, il existe une application linéaire continue $B(t)$ de $F$ dans lui-même, telle que l’on ait $\langle A(t) . \mathbf{x}, \mathbf{y} \rangle + \langle \mathbf{x}, B(t) . \mathbf{y} \rangle = 0$ pour tout $(\mathbf{x}, \mathbf{y}) \in E \times F$. Dans ces conditions, on voit comme ci-dessus que, pour qu’une application $t \mapsto \mathbf{v}(t)$ de $J$ dans $F$, primitive d’une fonction réglée, soit telle que $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ soit constante pour toute intégrale $\mathbf{u}$ de (4), il faut et il suffit que $\mathbf{v}$ soit intégrale de l’équation (16), qu’on appelle encore l’adjointe de (4).

### 6. Équations différentielles linéaires à coefficients constants

Nous supposons de nouveau que $E$ est un espace normé complet quelconque sur $\mathbf{R}$; soit $A$ un endomorphisme continu de $E$, indépendant de $t$, et considérons l’équation linéaire homogène

$$
\frac{d\mathbf{x}}{dt} = A . \mathbf{x}.
$$

Lorsque $E$ est de dimension finie, l’équation (19) est équivalente à un système homogène (3) (IV, p. 22) d’équations différentielles scalaires, où les coefficients $a_{ij}$ sont des constantes.

D’après le th. 1 (IV, p. 17), toute intégrale de (19) est définie dans $\mathbf{R}$ tout entier; d’après le th. 2 (IV, p. 18), l’intégrale de (19) prenant la valeur $x_0$ en un point $t_0 \in \mathbf{R}$ peut s’écrire $C(t, t_0)x_0$, où $C(t, t_0)$ est une application linéaire bijective et bicontinue de $E$ sur lui-même, satisfaisant à l’équation

$$
\frac{dU}{dt} = AU
$$

et telle que $C(t_0, t_0) = I$. On a en outre ici l’identité

$$
C(t + \tau, t_0 + \tau) = C(t, t_0)
$$

quel que soit $\tau \in \mathbf{R}$: en effet, on a $dC(s, t_0 + \tau)/ds = AC(s, t_0 + \tau)$ d’après (20), et, comme $A$ est constant, il en résulte qu’on a aussi

$$
\frac{dC(t + \tau, t_0 + \tau)}{dt} = AC(t + \tau, t_0 + \tau);
$$

d’autre part

$$
C(t_0 + \tau, t_0 + \tau) = I = C(t_0, t_0),
$$

d’où l’identité (21), puisque l’intégrale de (20) égale à $I$ au point $t_0$ est unique.

Si on pose $C_0(t) = C(t, 0)$, on a donc $C(t, t_0) = C_0(t - t_0)$; d’autre part, pour tout $\lambda \in \mathbf{R}$, $C_0(\lambda t)$ est identique à l’intégrale de l’équation

$$
\frac{dU}{dt} = \lambda AU
$$

qui prend la valeur $I$ au point 0. Nous poserons la définition suivante:

#### Définition 1 {#fvr-iv-s2-def-1 .statement}

Étant donné un endomorphisme continu $A$ de $E$, on désigne par $e^A$ ou $\exp A$ l’automorphisme de $E$ égal à la valeur au point $t = 1$ de l’intégrale de l’équation (20) qui prend la valeur $I$ au point $t = 0$.

Avec cette notation, les remarques qui précèdent la déf. 1 montrent que

$$
C(t, t_0) = \exp (A(t - t_0)).
$$

La notation exponentielle ainsi introduite et justifiée par les propriétés suivantes, qui sont tout à fait analogues à celles de la fonction $\exp z$, pour $z$ réel ou complexe (cf. III, p. 8 et 16):

#### Proposition 7 {#fvr-iv-s2-prop-7 .statement}

1° L’application $X \mapsto e^X$ est une application continue de $\mathcal{L}(E)$ dans le groupe des automorphismes de $E$ (éléments inversibles de $\mathcal{L}(E)$).

2° L’application $t \mapsto e^{xt}$ de $\mathbf{R}$ dans $\mathcal{L}(E)$ est dérivable et on a

$$
\frac{d}{dt}\left(e^{xt}\right) = X\,e^{xt} = e^{xt}X.
$$

3° Quel que soit $X \in \mathcal{L}(\mathbf{E})$, on a
$$
e^X = \sum_{n=0}^\infty \frac{X^n}{n!}
$$
la série du second membre étant absolument et uniformément convergente dans toute partie bornée de $\mathcal{L}(\mathbf{E})$; en particulier, $e^{it} = e^t I$ pour $t \in \mathbf{R}$.

4° Si $X$ et $Y$ sont permutables, $Y$ et $e^X$ sont tous deux permutables avec $e^X$, et on a
$$
e^{X+Y} = e^X e^Y.
$$

La relation (24) résulte de l’expression (23) de $C(t, 0)$ et du fait que cette fonction est intégrale de (20); de (24) on déduit par récurrence sur $n$ que $t \mapsto e^{xt}$ est indéfiniment dérivable dans $\mathbf{R}$ et que l’on a
$$
\mathrm{D}^n(e^{xt}) = X^n e^{xt}.
$$

D’après la formule de Taylor, on peut donc écrire
$$
e^X = I + \frac{X}{1!} + \frac{X^2}{2!} + \cdots + \frac{X^n}{n!} + X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{xt} dt.
$$

D’autre part, le cor. 3 de IV, p. 19, montre que $\|e^{xt}\| \leq \exp (\|X\| \cdot |t|)$. Donc le reste $r_n(X) = X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{xt} dt$ de la formule (27) satisfait à l’inégalité
$$
\|r_n(X)\| \leq \frac{\|X\|^{n+1}}{(n+1)!} e^{\|X\|}
$$
d’où on déduit la formule (25), la série du second membre étant absolument et uniformément convergente dans toute partie bornée de $\mathcal{L}(\mathbf{E})$. Pour tout couple d’éléments $X, T$ de $\mathcal{L}(\mathbf{E})$, on a donc
$$
e^{X+T} - e^X = \sum_{n=1}^\infty \frac{1}{n!} ((X+T)^n - X^n).
$$

Or, on peut écrire $(X+T)^n - X^n = \sum_{(V_i)} V_1 V_2 \ldots V_n$, la somme étant étendue aux $2^n - 1$ suites $(V_i)$ d’éléments de $\mathcal{L}(\mathbf{E})$ telles que $V_i = X$ ou $V_i = T$ pour $1 \leq i \leq n$, un au moins des $V_i$ étant égal à $T$; on en conclut aussitôt l’inégalité
$$
\|(X+T)^n - X^n\| \leq (\|X\| + \|T\|)^n - \|X\|^n,
$$
d’où
$$
\| \exp (X+T) - \exp X \| \leq \exp (\|X\| + \|T\|) - \exp \|X\|
$$
ce qui établit la continuité de l’application $X \mapsto \exp X$.

Enfin, si $X$ et $Y$ sont permutables, $Y$ est permutable avec $e^{xt}$ (IV, p. 20, prop. 2), donc on a
$$
\frac{d}{dt} (e^{xt} e^{yt}) = X e^{xt} e^{yt} + e^{xt} (Ye^{yt}) = (X + Y) e^{xt} e^{yt}.
$$

Comme d’autre part $e^{Xt}e^{Yt}$ est égal à $I$ pour $t = 0$, on a $e^{Xt}e^{Yt} = e^{(X+Y)t}$, d’où la formule (26). De cette dernière, on déduit en particulier que, pour $s$ et $t$ réels quelconques, on a
$$
e^{X(s+t)} = e^{Xs}e^{Xt}
$$
et aussi que
$$
e^{-X} = (e^X)^{-1}.
$$

On notera par contre que la formule (26) n’est plus exacte lorsqu’on ne suppose pas $X$ et $Y$ permutables : elle entraînerait en effet que $\exp X$ et $\exp Y$ sont toujours permutables, ce qui n’est pas le cas, comme le montrent des exemples simples (IV, p. 41, exerc. 3).

Supposons maintenant que $E$ soit un espace vectoriel de dimension finie sur le corps $\mathbf{C}$, et $A$ un endomorphisme de $E$ (pour la structure d’espace vectoriel sur $\mathbf{C}$) qu’on peut identifier à sa matrice par rapport à une base de $E$; pour tout $t \in \mathbf{R}$, $e^{At}$ est alors un automorphisme de $E$ pour cette même structure (IV, p. 20, prop. 2). Soient $r_k$ ($1 \leq k \leq q$) les racines distinctes (dans $\mathbf{C}$) du polynôme caractéristique $\varphi(r) = \det(A - rI)$ de l’endomorphisme $A$ (« racines caractéristiques » de $A$); si $n_k$ est l’ordre de multiplicité de $r_k$, on a $\sum_{k=1}^q n_k = n$. On sait (A, VII, § 5, no 3) qu’à chaque racine $r_k$ correspond un sous-espace $E_k$ de $E$, de dimension $n_k$, tel que $E_k$ soit stable par $A$, et que $E$ soit somme directe des $E_k$: $E_k$ peut être défini comme le sous-espace des vecteurs $x$ tels que
$$
(A - r_kI)^{n_k}x = 0.
$$

Soit $a$ un vecteur quelconque de $E$; on peut écrire $a = \sum_{k=1}^q a_k$, où $a_k \in E_k$; l’intégrale de l’équation (19) de IV, p. 26, prenant la valeur $a$ au point $t = 0$ est donc donnée par
$$
u(t) = e^{At}.a = \sum_{k=1}^q e^{At}.a_k = \sum_{k=1}^q e^{r_k t} e^{(A - r_k I)t}.a_k.
$$

Mais comme $a_k \in E_k$, on a
$$
e^{(A - r_k I)t}.a_k = a_k + \frac{t}{1!}(A - r_k I).a_k + \frac{t^2}{2!}(A - r_k I)^2.a_k + \cdots + \frac{t^{n_k - 1}}{(n_k - 1)!}(A - r_k I)^{n_k - 1}.a_k.
$$

Toute intégrale de l’équation (19) de IV, p. 26, peut donc s’écrire
$$
u(t) = \sum_{k=1}^q e^{r_k t} p_k(t)
$$
où $p_k(t)$ est un polynôme par rapport à $t$, à coefficients dans l’espace vectoriel $E_k$, et de degré $\leq n_k - 1$. En particulier, si toutes les racines de l’équation caractéristique de $A$ sont simples, les espaces $E_k$ ($1 \leq k \leq n$) sont tous de dimension 1 sur le corps $\mathbf{C}$, et il existe donc $n$ vecteurs $c_k$ tels que les $n$ fonctions $e^{r_k t}c_k$ ($1 \leq k \leq n$) forment un système fondamental d’intégrales de l’équation (19) de IV, p. 26.

Les racines caractéristiques de l’endomorphisme $A$ sont encore appelées les racines caractéristiques de l’équation linéaire (19) de IV, p. 26. On observera qu’on obtient l’équation caractéristique de $A$ en exprimant que la fonction $ec^{rt}$ est intégrale de (19) pour un vecteur $c \neq 0$.

Lorsque l’on a déterminé explicitement les racines $r_k$ ($1 \leq k \leq q$), ainsi que l’ordre de multiplicité $n_k$ de $r_k$, on obtient en pratique les intégrales de (19) en écrivant que cette équation est vérifiée par l’expression (32) de IV, p. 29, où $p_k$ est un polynôme arbitraire de degré $\leq n_k - 1$, à coefficients dans $E$; en identifiant, dans les deux membres de l’équation obtenue, les coefficients de $e^{r_k t}$ (pour $1 \leq k \leq q$), on obtient des équations linéaires par rapport aux coefficients des polynômes $p_k$: on constate aisément que ces équations déterminent les coefficients des termes de degré $> 0$ de $p_k$ en fonction du terme constant, et que ce dernier est solution de l’équation $(A - r_k I)^{n_k} x = 0$, qui définit le sous-espace $E_k$ (« méthode des coefficients indéterminés »).

#### Remarque {#fvr-iv-s2-n6-rem-1 .statement}

Lorsqu’il existe une base de $E$ telle que la matrice de $A$ par rapport à cette base ait ses éléments réels (cf. IV, p. 24, Remarque 2), l’équation caractéristique de $A$ a ses coefficients réels. Pour tout vecteur $x = (\xi_k)_{1 \leq k \leq n}$ de $E$, rapporté à la base considérée, soit $\bar{x} = (\bar{\xi}_k)_{1 \leq k \leq n}$; l’application $x \mapsto \bar{x}$ est une involution antilinéaire de $E$. On sait (A, VII) que, si $r_k$ est une racine non réelle de l’équation caractéristique de $A$, $E_k$ le sous-espace stable correspondant, alors $\bar{r}_k$ est une racine caractéristique ayant même ordre de multiplicité $n_k$ que $r_k$, et l’image $E'_k$ de $E_k$ par l’application $x \mapsto \bar{x}$ est le sous-espace stable correspondant à $\bar{r}_k$. On en déduit que si $u_j$ ($1 \leq j \leq n_k$) sont $n_k$ intégrales linéairement indépendantes à valeurs dans $E_k$, les $2n_k$ intégrales $u_j + \bar{u}_j, i(u_j - \bar{u}_j)$ sont linéairement indépendantes et ont, par rapport à la base choisie dans $E$, des composantes qui sont des fonctions réelles de $E$. Si $r_k$ est une racine caractéristique réelle, la Remarque 2 de IV, p. 24, montre (avec les mêmes notations) qu’il existe $n_k$ intégrales linéairement indépendantes $v_j$ ($1 \leq j \leq n_k$) à valeurs dans $E_k$ et qui ont leurs composantes réelles. On obtient de la sorte un système fondamental d’intégrales de (19) dont les composantes sont toutes réelles.

### 7. Équations linéaires d’ordre $n$

On appelle équation différentielle linéaire d’ordre $n$ toute équation de la forme

$$
\mathrm{D}^n x - a_1(t) \mathrm{D}^{n-1} x - \cdots - a_{n-1}(t) \mathrm{D} x - a_n(t) x = b(t)
$$

où les $a_k$ ($1 \leq k \leq n$) et $b$ sont des fonctions scalaires (complexes) de la variable réelle $t$, définies dans un intervalle $J$ de $\mathbf{R}$. Le procédé général de IV, p. 2, montre que cette équation équivaut au système linéaire de $n$ équations du premier ordre

$$
\begin{cases}
\frac{dx_k}{dt} = x_{k+1} \\
\frac{dx_n}{dt} = a_1(t)x_n + a_2(t)x_{n-1} + \cdots + a_n(t)x_1 + b(t) & (1 \leq k \leq n-1)
\end{cases}
$$

c’est-à-dire à l’équation linéaire

(35) $$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

où on a posé $\mathbf{x} = (x_1, x_2, \ldots, x_n) \in \mathbf{C}^n$, $\mathbf{b}(t) = (0, 0, \ldots, 0, b(t))$, et où la matrice $A(t)$ est définie par

$$
A(t) = \begin{pmatrix}
0 & 1 & 0 & \ldots & 0 \\
0 & 0 & 1 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & \ldots & 1 \\
a_n(t) & a_{n-1}(t) & a_{n-2}(t) & \ldots & a_1(t)
\end{pmatrix}.
$$

L’étude de l’équation linéaire d’ordre $n$ consiste donc à appliquer à l’équation linéaire particulière (35) les résultats généraux qui précèdent. Pour tout intervalle $J$ où les fonctions $a_j$ ($1 \leq j \leq n$) et $b$ sont réglées, il existe une fonction et une seule $u$, définie dans $J$, admettant dans cet intervalle une dérivée $(n-1)$-ème continue et une dérivée $n$-ème réglée (sauf aux points d’un ensemble dénombrable), satisfaisant à l’équation (33) dans le complémentaire d’une partie dénombrable de $J$, et telle que

(36) $$
u(t_0) = x_0, \quad Du(t_0) = x'_0, \ldots, D^{n-1}u(t_0) = x_0^{(n-1)}
$$

où $t_0$ est un point quelconque de $J$, $x_0, x'_0, \ldots, x_0^{(n-1)}$, $n$ nombres complexes arbitraires.

Pour que $p$ intégrales $u_j$ ($1 \leq j \leq p$) de l’équation homogène

(37) $$
D^n x - a_1(t)D^{n-1}x - \cdots - a_{n-1}(t)Dx - a_n(t)x = 0
$$

associée à (33), soient linéairement indépendantes (dans l’espace $\mathscr{C}(J, \mathbf{C})$ des applications continues de $J$ dans $\mathbf{C}$, considéré comme espace vectoriel sur $\mathbf{C}$), il faut et il suffit que les $p$ intégrales correspondantes $\mathbf{u}_j = (u_j, Du_j, \ldots, D^{n-1}u_j)$ de l’équation homogène $dx/dt = A(t).\mathbf{x}$ soient linéairement indépendantes (dans l’espace $\mathscr{C}(J; \mathbf{C}^n)$ des applications continues de $J$ dans $\mathbf{C}^n$). Il est évident en effet que la condition est nécessaire. Inversement, s’il existe $n$ constantes complexes $\lambda_j$ non toutes nulles telles qu’on ait identiquement $\sum_{j=1}^n \lambda_j u_j(t) = 0$ dans $J$, on en déduit $\sum_{j=1}^n \lambda_j D^k u_j(t) = 0$ dans $J$ pour tout entier $k$ tel que $1 \leq k \leq n-1$, ce qui signifie que l’on a $\sum_{j=1}^n \lambda_j \mathbf{u}_j(t) = 0$ dans $J$.

Par suite (IV, p. 19, cor. 1):

#### Proposition 8 {#fvr-iv-s2-prop-8 .statement}

*L’ensemble des intégrales de l’équation linéaire homogène (37), définies dans $J$, est un espace vectoriel de dimension $n$ sur le corps $\mathbf{C}$.*

Étant données n intégrales quelconques $u_j$ ($1 \leq j \leq n$) de l’équation (37), on appelle wronskien de ce système d’intégrales le déterminant (par rapport à la base canonique de $\mathbf{C}^n$) du système des n intégrales correspondantes $\mathbf{u}_j$ de l’équation $d\mathbf{x}/dt = A(t) \cdot \mathbf{x}$, c’est-à-dire la fonction

$$
W(t) = \begin{vmatrix}
u_1(t) & u_2(t) & \ldots & u_n(t) \\
Du_1(t) & Du_2(t) & \ldots & Du_n(t) \\
\vdots & \vdots & \ddots & \vdots \\
D^{n-1}u_1(t) & D^{n-1}u_2(t) & \ldots & D^{n-1}u_n(t)
\end{vmatrix}.
$$

Pour que les n intégrales $u_j$ soient linéairement indépendantes, il faut et il suffit que $W(t) \neq 0$ dans J; d’ailleurs, il suffit pour cela que $W(t_0) \neq 0$ en un point $t_0$ de J (IV, p. 22, prop. 4); en outre, on a (IV, p. 23, prop. 5)

$$
W(t) = W(t_0) \exp \left( \int_{t_0}^t a_1(s) \, ds \right).
$$

Identifions la résolvante $C(t, t_0)$ de l’équation (35) à sa matrice par rapport à la base canonique de $\mathbf{C}^n$; les colonnes $\mathbf{v}_j(t, t_0)$ ($1 \leq j \leq n$) de cette matrice sont alors n intégrales linéairement indépendantes

$$
\mathbf{v}_j(t, t_0) = (v_j(t, t_0), Dv_j(t, t_0), \ldots, D^{n-1}v_j(t, t_0))
$$

de l’équation homogène $d\mathbf{x}/dt = A(t) \cdot \mathbf{x}$, qui correspondent aux n intégrales linéairement indépendantes $v_j(t, t_0)$ de l’équation (37), telles que

$$
D^{k-1}v_j(t_0, t_0) = \delta_{jk}
$$

(indice de Kronecker) pour $1 \leq j \leq n,\ 1 \leq k \leq n$ (en convenant de poser $D^0v_j = v_j$). Il en résulte en particulier que la méthode de variation des constantes (IV, p. 21) appliquée à l’équation (35) donne ici comme intégrale particulière de (33), égale à 0 ainsi que ses $n - 1$ premières dérivées au point $t_0$, la fonction

$$
w(t) = \int_{t_0}^t v_n(t, s) b(s) \, ds.
$$

Dans le cas particulier de l’équation $D^n x = b(t)$, la formule (39) redonne la formule exprimant la primitive n-ème de la fonction réglée $b(t)$ qui s’annule ainsi que ses $n - 1$ premières dérivées au point $t_0$

$$
w(t) = \int_{t_0}^t b(s) \frac{(t-s)^{n-1}}{(n-1)!} \, ds
$$

(II, p. 13, formule (19)): l’intégrale de $D^n x = 0$ qui est nulle ainsi que ses $n - 2$ premières dérivées au point $t_0$, et dont la dérivée $(n-1)$-ème est égale à 1 en ce point, est en effet le polynôme $(t-t_0)^{n-1}/(n-1)!$.

### 8. Equations linéaires d’ordre $n$ à coefficients constants

Si, dans l’équation (33), les coefficients $a_i$ sont *constants*, la matrice correspondante $A$ est constante; l’équation caractéristique correspondante s’obtient en écrivant que $e^{rt}$ est solution, ce qui donne
$$
r^n - a_1 r^{n-1} - \cdots - a_{n-1} r - a_n = 0.
$$
Soient $r_j$ ($1 \leq j \leq q$) les racines distinctes de cette équation, $n_j$ ($1 \leq j \leq q$) l’ordre de multiplicité de la racine $r_j$ ($\sum_{j=1}^q n_j = n$). D’après les résultats de IV, p. 26 à 32, à chaque racine $r_j$ correspond, pour l’équation homogène
$$
\mathrm{D}^n x - a_1 \mathrm{D}^{n-1} x - \cdots - a_{n-1} \mathrm{D} x - a_n x = 0
$$
un système de $n_j$ intégrales *linéairement indépendantes*
$$
u_{jk}(t) = e^{r_j t} p_{jk}(t),
$$
où $p_{jk}$ est un polynôme (à coefficients complexes) de degré $\leq n_j - 1$ ($1 \leq k \leq n_j$); en outre, les $n$ intégrales $u_{jk}$ ($1 \leq j \leq q, 1 \leq k \leq n_j$) ainsi obtenues sont *linéairement indépendantes*. Il en résulte que les $n_j$ polynômes $p_{jk}$ ($1 \leq k \leq n_j$) sont linéairement indépendants dans l’espace des polynômes en $t$ de degré $\leq n_j - 1$, donc forment une *base* (sur $\mathbf{C}$) de cet espace, puisque ce dernier est de dimension $n_j$. Autrement dit:

#### Proposition 9 {#fvr-iv-s2-prop-9 .statement}

*Soient $r_j$ ($1 \leq j \leq q$) les racines distinctes de l’équation caractéristique (40), et soit $n_j$ l’ordre de multiplicité de la racine $r_j$ ($1 \leq j \leq q$). Les $n$ fonctions $t^{k} e^{r_j t}$ ($1 \leq k \leq n_j, 1 \leq j \leq q$) sont des intégrales linéairement indépendantes de l’équation homogène (41).*

On peut démontrer ce résultat directement de la façon suivante. Il résulte de l’équation (41) que la dérivée $n$-ème de toute intégrale de cette équation est dérivable dans $\mathbf{R}$, d’où on déduit aussitôt, par récurrence sur l’entier $m > n$, que toute intégrale de (41) admet une dérivée d’ordre $m$, autrement dit, est *indéfiniment dérivable* dans $\mathbf{R}$. Soit $\mathcal{D}$ l’espace vectoriel sur $\mathbf{C}$ (non topologique) des fonctions complexes indéfiniment dérivables dans $\mathbf{R}$; l’application $x \mapsto \mathrm{D} x$ est un endomorphisme de cet espace, et l’équation (41) peut s’écrire
$$
f(\mathrm{D}) x = 0
$$
où $f(\mathrm{D}) = \mathrm{D}^n - a_1 \mathrm{D}^{n-1} - \cdots - a_{n-1} \mathrm{D} - a_n$ (A, IV, § 2, no 1).

#### Proposition 10 {#fvr-iv-s2-prop-10 .statement}

*Soient $g$ et $h$ deux polynômes premiers entre eux tels que $f = gh$. Le sous-espace des solutions de (42) est somme directe des sous-espaces des solutions des deux équations*
$$
g(\mathrm{D}) x = 0, \qquad h(\mathrm{D}) x = 0.
$$

En effet, en vertu de l’identité de Bezout (A, VII, § 1, n° 2, th. 1), il existe deux polynômes $p(D)$ et $q(D)$ tels que $p(D)g(D) + q(D)h(D) = 1$. Pour toute solution $x$ de (42), on peut donc écrire $x = y + z$, où $y = p(D)g(D)x$ et $z = q(D)h(D)x$, et on a $h(D)y = p(D)(f(D)x) = 0$, et $g(D)z = q(D)(f(D)x) = 0$. D’autre part, si on a à la fois $g(D)x = 0$ et $h(D)x = 0$, on en tire
$$
x = p(D)(g(D)x) + q(D)(h(D)x) = 0,
$$
ce qui achève la démonstration.

Avec les notations précédentes, on peut alors écrire
$$
f(D) = \prod_{j=1}^q (D - r_j)^{n_j}
$$
et la prop. 10, appliquée par récurrence sur $q$, montre que le sous-espace des solutions de (42) est somme directe des sous-espaces des solutions des $q$ équations
$$
(D - r_j)^{n_j}x = 0 \qquad (1 \leq j \leq q).
$$
Or, pour tout nombre complexe $r$, on a
$$
D(e^{rt}x) = e^{rt}(D + r)x
$$
et par suite l’équation (43) équivaut à
$$
D^{n_j}(e^{-r_jt}x) = 0
$$
et a donc pour solutions les fonctions $e^{r_jt}p_j(t)$, où $p_j$ parcourt l’ensemble des polynômes de degré $\leq n_j - 1$; on retrouve ainsi la prop. 9 de IV, p. 33.

L’équation homogène (41) étant supposée résolue (c’est-à-dire que les racines caractéristiques sont supposées déterminées), on sait que la méthode de variation des constantes permet de trouver les solutions de l’équation non homogène
$$
D^n x - a_1 D^{n-1} x - \ldots - a_{n-1} Dx - a_n x = b(t)
$$
où $b(t)$ est une fonction réglée quelconque (IV, p. 21); on notera que si $b(t)$ est indéfiniment dérivable dans un intervalle $J$, toutes les intégrales de (45) sont indéfiniment dérivables dans $J$. Dans le cas particulier $b(t) = e^{\alpha t} p(t)$, où $p$ est un polynôme (à coefficients complexes) et $\alpha$ un nombre complexe quelconque, on obtient plus simplement une intégrale de (45) de la façon suivante. Posons $x = e^{\alpha t} y$; l’équation
$$
f(D)x = e^{\alpha t} p(t)
$$
s’écrit d’après (44)
$$
f(\alpha + D)y = p(t)
$$
ou encore, en vertu de la formule de Taylor appliquée au polynôme $f(D)$,

(46) $$
\frac{f^{(n)}(\alpha)}{n!} D^n y + \frac{f^{(n-1)}(\alpha)}{(n-1)!} D^{n-1} y + \cdots + \frac{f'(\alpha)}{1!} Dy + f(\alpha)y = p(t).
$$

Soit $m$ le degré du polynôme $p(t) = \sum_{k=0}^m \lambda_k t^{m-k}$; si $f(\alpha) \neq 0$ (c'est-à-dire si $\alpha$ n'est pas racine caractéristique), il existe un polynôme et un seul $u(t) = \sum_{k=0}^m c_k t^{m-k}$ de degré $m$, solution de l'équation (46), car les coefficients $c_k$ sont déterminés par le système d'équations linéaires
$$
f(\alpha)c_k + \binom{m-k+1}{1} f'(\alpha)c_{k-1} + \binom{m-k+2}{2} f''(\alpha)c_{k-2} + \cdots
+ \binom{m}{k} f^{(k)}(\alpha)c_0 = \lambda_k \quad (0 \leq k \leq m)
$$
qui admet évidemment une solution et une seule. Si au contraire $\alpha$ est une racine caractéristique, et si $h$ est son ordre de multiplicité, le calcul précédent montre qu'il existe un polynôme et un seul $v(t)$ de degré $m$, tel que toute solution de $D^h y = v(t)$ soit une intégrale; autrement dit, tout polynôme solution de (46) est alors de degré $m + h$ (« résonance »).

### 9. Systèmes d'équations linéaires à coefficients constants

Avec les notations du no 8, considérons plus généralement un système de $m$ équations différentielles de la forme
$$
\sum_{k=1}^n p_{jk}(D)x_k = b_j(t) \qquad (1 \leq j \leq m)
$$
où les inconnues $x_k$ ($1 \leq k \leq n$) et les seconds membres $b_j$ ($1 \leq j \leq m$) sont des fonctions complexes de la variable réelle $t$, et où les $p_{jk}(D)$ sont des polynômes (de degré quelconque) à coefficients constants (complexes) par rapport à l'opérateur de dérivation $D$ ($1 \leq j \leq m, 1 \leq k \leq n$).

De tels systèmes ne sont pas du même type que ceux considérés dans IV, p. 2, (formule (5)), comme le montre l'exemple suivant:
$$
\begin{cases}
Dx_1 = a(t) \\
D^2x_1 + Dx_2 + x_3 = b(t).
\end{cases}
$$

Nous nous bornerons au cas où les $b_j(t)$ sont les fonctions indéfiniment dérivables dans un intervalle $J$, et nous chercherons seulement les solutions $(x_k)_{1 \leq k \leq n}$ indéfiniment dérivables dans $J$. En posant $\mathbf{b}(t) = (b_1(t), \ldots, b_m(t))$ (application de $J$ dans $\mathbf{C}^m$), et $\mathbf{x} = (x_1, x_2, \ldots, x_n)$, le système (47) peut s'écrire
$$
P(D)\mathbf{x} = \mathbf{b}(t)
$$
où $P(D)$ est la matrice $(p_{jk}(D))$ à $m$ lignes et $n$ colonnes, dont les coefficients

appartiennent à l’anneau $\mathbf{C}[D]$ des polynômes en D, à coefficients dans $\mathbf{C}$. Soient $f_j(D)$ ($1 \leq j \leq r \leq \min(m, n)$) les *invariants de similitude* non nuls de la matrice $P(D)$; on sait (A, VII, § 5, no 1) que ce sont des polynômes unitaires bien déterminés, tels que $f_j$ divise $f_{j+1}$ pour $1 \leq j \leq r - 1$ (*r* étant le *rang* de $P(D)$); en outre, il existe deux matrices carrées $U(D)$ et $V(D)$, d’ordres respectifs $m$ et $n$, *inversibles* (dans les anneaux de matrices carrées d’ordre $m$ et $n$ respectivement, *à coefficients dans l’anneau* $\mathbf{C}[D]$ *des polynômes en D à coefficients complexes*), et telles que la matrice $Q(D) = (q_{jk}(D)) = U(D)P(D)V(D)$ ait tous ses termes nuls, à l’exception des termes diagonaux $q_{jj}(D) = f_j(D)$ pour $1 \leq j \leq r$. Posons alors $y = V^{-1}(D)x$; l’équation (49) est équivalente à l’équation
$$
U(D)(P(D)(V(D)y)) = U(D)b,
$$
c’est-à-dire à
$$
Q(D)y = U(D)b
$$
puisque $U(D)$ est inversible. Or, si $y = (y_1, y_2, \ldots, y_n)$, et si
$$
U(D)b(t) = (c_1(t), \ldots, c_m(t)),
$$
l’équation (50) s’écrit
$$
f_j(D)y_j = c_j(t) \quad \text{pour } 1 \leq j \leq r
$$
$$
0 = c_j(t) \quad \text{pour } r + 1 \leq j \leq m.
$$

Le système n’admet donc de solutions indéfiniment dérivables que si les conditions (52) sont vérifiées; la détermination des $y_j$ d’indice $j \leq r$ se ramène alors à l’intégration de $r$ équations différentielles linéaires à coefficients constants (51); les $y_j$ d’indice $> r$ sont des fonctions indéfiniment dérivables arbitraires. Une fois les solutions $y$ de l’équation (50) ainsi déterminées, on en déduit les solutions de (47) par la formule $x = V(D)y$.

#### Remarque 1 {#fvr-iv-s2-n9-rem-1 .statement}

Certains des polynômes $f_j(D)$ peuvent se réduire à des constantes non nulles; les $y_j$ correspondants sont alors entièrement déterminés.
2) Lorsque les $b_j$ sont tous nuls, c’est-à-dire que le système (47) est *homogène*, les conditions (52) sont toujours vérifiées; si en outre $r = n$, on voit que l’ensemble des solutions de (47) est un espace vectoriel sur $\mathbf{C}$, de dimension égale à la *somme des degrés* des $f_j(D)$, c’est-à-dire au *degré* de $\det(P(D))$.
3) Les polynômes $p_{jk}(D)$ étant donnés, un système (47) qui admet des solutions lorsque les seconds membres sont indéfiniment dérivables (ou dérivables jusqu’à un certain ordre) peut ne pas en admettre lorsque les seconds membres sont des fonctions réglées quelconques: c’est ce que montre l’exemple (48), qui n’admet pas de solution lorsque $a(t)$ n’est pas une primitive. Nous n’entendrons pas ici de rechercher les conditions supplémentaires de possibilité qui s’introduisent ainsi lorsque les seconds membres sont des fonctions réglées quelconques.

## EXERCICES {#fvr-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
