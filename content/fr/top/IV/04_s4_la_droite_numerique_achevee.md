---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 4
section_title: La droite numérique achevée
lang: fr
source: top-i-iv-fr
book_pages: TG IV.13-TG IV.17, TG IV.52-TG IV.53
pdf_pages: 0284-0288, 0323-0324
extraction: ocr
subsections:
    - "no": 1
      title: Homéomorphie des intervalles ouverts de $\mathbf{R}$
      page: 13
      pdf_page: 284
    - "no": 2
      title: La droite achevée
      page: 13
      pdf_page: 284
    - "no": 3
      title: L’addition et la multiplication dans $\overline{\mathbf{R}}$
      page: 15
      pdf_page: 286
statements: 11
exercises: 7
content_sha256: af63fd49662b26044df6b743e044f17da548890c091998233d4421ac7411fd07
---

## § 4. LA DROITE NUMÉRIQUE ACHEVÉE

### 1. Homéomorphie des intervalles ouverts de $\mathbf{R}$

#### Proposition 1 {#top-iv-s4-prop-1 .statement}

*Tous les intervalles ouverts non vides de $\mathbf{R}$ sont homéomorphes à la droite $\mathbf{R}$.*

Considérons d’abord un intervalle ouvert *borné* $I = ]a, b[ \quad (a < b)$. Posons, pour $x \in I, f(x) = -\left( \frac{1}{x-a} + \frac{1}{x-b} \right)$. Cette fonction est continue et strictement croissante dans $I$, car on a vu que $\frac{1}{x-b}$ est strictement décroissante dans $]-\infty, b[$ et $\frac{1}{x-a}$ strictement décroissante dans $]a, +\infty[$. Il en résulte que $f$ est un homéomorphisme de $I$ sur un intervalle $f(I)$ de $\mathbf{R}$ (IV, p. 9, th. 5); $f(I)$ n’est borné ni supérieurement, ni inférieurement, car si on avait par exemple $f(x) \leq c$ quel que soit $x \in I$, on en tirerait, puisque $b-x > 0, 1 - \frac{b-x}{x-a} \leq c(b-x)$, d’où contradiction dès que $x$ est suffisamment voisin de $b$ (en vertu de la continuité des deux membres, qui sont des fonctions rationnelles, au point $b$). Donc $f(I) = \mathbf{R}$, ce qui établit que tout intervalle ouvert borné est homéomorphe à $\mathbf{R}$. Soit $g$ l’application réciproque de $f$; elle applique tout intervalle ouvert illimité de $\mathbf{R}$ sur un intervalle $J$ contenu dans $I$ et ouvert par rapport à $I$. Puisque $I$ est ouvert dans $\mathbf{R}$, $J$ est lui-même ouvert dans $\mathbf{R}$; comme il est borné, il est homéomorphe à $\mathbf{R}$, ce qui démontre que tout intervalle ouvert illimité est homéomorphe à $\mathbf{R}$.

#### Remarque {#top-iv-s4-n1-rem-1 .statement}

Pour démontrer que tous les intervalles ouverts *bornés* sont homéomorphes entre eux, il suffirait de remarquer que, pour $a \neq b, a' \neq b'$, il existe un homéomorphisme de $\mathbf{R}$ sur lui-même, de la forme $x \mapsto \alpha x + \beta$ (et un seul) qui applique $a$ sur $a'$ et $b$ sur $b'$, donc tout intervalle ouvert (resp. fermé, semi-ouvert) d’extrémités $a, b$, sur un intervalle ouvert (resp. fermé, semi-ouvert) d’extrémités $a', b'$: ce que le lecteur vérifiera facilement en calculant $\alpha$ et $\beta$.

### 2. La droite achevée

On va maintenant définir, par *adjonction* de deux nouveaux éléments à $\mathbf{R}$, un espace topologique $\overline{\mathbf{R}}$ tel que tout homéomorphisme de $\mathbf{R}$ sur un intervalle ouvert borné $I$ de $\mathbf{R}$ puisse se prolonger en un homéomorphisme de $\overline{\mathbf{R}}$ sur l’intervalle fermé ayant mêmes extrémités que $I$.

Pour cela, soit $\overline{\mathbf{R}}$ l’ensemble obtenu par adjonction à $\mathbf{R}$ (E, II, p. 30) de deux éléments qu’on notera respectivement $-\infty, +\infty$. On prolonge à $\overline{\mathbf{R}}$ la structure d’ordre de $\mathbf{R}$, en posant $-\infty < a, a < +\infty$ pour tout $a \in \mathbf{R}$, et $-\infty < +\infty$; il est clair qu’on a ainsi un ensemble totalement ordonné, dont la structure d’ordre induit sur $\mathbf{R}$ la structure d’ordre de la droite numérique. En second lieu, considérons sur $\overline{\mathbf{R}}$ la topologie engendrée par l’ensemble des intervalles ouverts de $\overline{\mathbf{R}}$;

comme la trace sur $\mathbf{R}$ d’un intervalle ouvert de $\overline{\mathbf{R}}$ est un intervalle ouvert de $\mathbf{R}$, cette topologie induit sur $\mathbf{R}$ la topologie de la droite numérique.

#### Définition 1 {#top-iv-s4-def-1 .statement}

On appelle droite numérique achevée l’ensemble $\overline{\mathbf{R}}$ muni de la structure d’ordre et de la topologie ainsi définies.

Lorsqu’on raisonne sur la droite achevée $\overline{\mathbf{R}}$, il est souvent commode, par un abus de langage, d’appeler encore ses points nombres réels; les points de $\mathbf{R}$ (auxquels ce nom était réservé jusqu’ici) sont alors dits nombres réels finis. Nous adoptons cette convention dans ce paragraphe et dans les trois suivants; chaque fois que nous l’adopterons par la suite, nous signalerons expressément à quelle partie du texte elle s’étend.

Si $a$ est un nombre réel fini, les intervalles $]a, +\infty[$ et $]-\infty, a[$ (resp. $]a, +\infty[$ et $]-\infty, a[$) de $\overline{\mathbf{R}}$ sont contenus dans $\mathbf{R}$ et identiques aux intervalles de $\mathbf{R}$ désignés jusqu’ici par les notations $]a, \rightarrow[$ et $]\leftarrow, a[$ (resp. $]a, \rightarrow[$ et $]\leftarrow, a[$); ces nouvelles notations sont beaucoup plus fréquemment employées. De même $\mathbf{R}$ est identique à l’intervalle $]-\infty, +\infty[$ de $\overline{\mathbf{R}}$; on le désigne parfois par cette notation.

#### Proposition 2 {#top-iv-s4-prop-2 .statement}

Tout homéomorphisme $f$ de $\mathbf{R}$ sur un intervalle $]a, b[$ se prolonge en un homéomorphisme $\tilde{f}$ de $\overline{\mathbf{R}}$ sur $[a, b]$; si $f$ est une fonction croissante, $\tilde{f}$ est un isomorphisme de la structure d’ordre de $\overline{\mathbf{R}}$ sur celle de $[a, b]$.

En effet, soit d’abord $f$ un homéomorphisme croissant. Si on prolonge $f$ à $\overline{\mathbf{R}}$ en posant $\tilde{f}(-\infty) = a, \tilde{f}(+\infty) = b$, il est immédiat que $\tilde{f}$ est une application strictement croissante (donc bijective) de $\overline{\mathbf{R}}$ sur $[a, b]$. Elle applique donc tout intervalle ouvert de $\overline{\mathbf{R}}$ sur un intervalle ouvert par rapport à $[a, b]$, donc est un homéomorphisme de $\mathbf{R}$ sur $[a, b]$, en vertu de la déf. 1, et de la prop. 5 de IV, p. 5.

Si $f$ est décroissant, on appliquera ce qui précède à l’homéomorphisme croissant $x \mapsto -f(x)$ de $\mathbf{R}$ sur $]-b, -a[$.

Toutes les propriétés de l’intervalle $[a, b]$, obtenues au § 2, qui ne font intervenir que la structure d’ordre et la topologie de cet intervalle, se transportent donc à $\overline{\mathbf{R}}$, d’où les propositions suivantes:

#### Proposition 3 {#top-iv-s4-prop-3 .statement}

La droite numérique achevée est compacte.

Il existe donc (II, p. 27, th. 1) une structure uniforme et une seule compatible avec la topologie de $\overline{\mathbf{R}}$; cette structure est isomorphe à la structure uniforme induite sur $[a, b]$ par la structure uniforme additive de $\mathbf{R}$. Mais il faut remarquer que la structure uniforme *induite* sur $\mathbf{R}$ par celle de $\overline{\mathbf{R}}$ (structure qui est compatible avec la topologie de la droite numérique) *n’est pas la structure uniforme additive* de $\mathbf{R}$; car pour cette dernière $\mathbf{R}$ est un espace *complet*, alors que $\mathbf{R}$ n’est pas un sous-espace complet de $\overline{\mathbf{R}}$, puisque $\mathbf{R}$ n’est pas fermé dans $\overline{\mathbf{R}}$.

#### Proposition 4 {#top-iv-s4-prop-4 .statement}

Toute partie non vide de $\overline{\mathbf{R}}$ possède une borne supérieure et une borne inférieure.

La borne supérieure (resp. inférieure) d’une partie non vide $A$ de $\overline{\mathbf{R}}$ se note $\sup A$ (resp. $\inf A$). On a évidemment
(1)
$$
\inf A \leq \sup A.
$$

Si $A \subset B$, $\sup A \leq \sup B$ et $\inf A \geq \inf B$ (E, III, p. 10, prop. 4).

#### Proposition 5 {#top-iv-s4-prop-5 .statement}

*Pour qu’une partie A de $\overline{\mathbf{R}}$ soit connexe, il faut et il suffit que A soit un intervalle.*

#### Corollaire {#top-iv-s4-n2-cor-1 .statement}

*La droite numérique achevée est un espace connexe et localement connexe.*

#### Proposition 6 {#top-iv-s4-prop-6 .statement}

*Pour qu’une application f dans $\overline{\mathbf{R}}$ d’un intervalle I de $\overline{\mathbf{R}}$ soit un homéomorphisme de I sur $f(I)$, il faut et il suffit que f soit strictement monotone et continue dans I; $f(I)$ est alors un intervalle de $\overline{\mathbf{R}}$.*

Enfin, les fonctions $\sup(x, y)$ et $\inf(x, y)$ sont *continues* dans $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$.

### 3. L’addition et la multiplication dans $\overline{\mathbf{R}}$

Remarquons d’abord que la fonction $-x$ se prolonge par continuité à $\overline{\mathbf{R}}$, suivant les formules $-(+\infty) = -\infty$ et $-(-\infty) = +\infty$; la fonction ainsi prolongée est encore un homéomorphisme de $\overline{\mathbf{R}}$ sur lui-même.

En second lieu, considérons les fonctions $x + y$ et $xy$, définies dans $\mathbf{R} \times \mathbf{R}$, à valeurs dans $\mathbf{R}$; si on considère qu’elles prennent leurs valeurs *dans l’espace topologique* $\overline{\mathbf{R}}$, nous allons voir qu’on peut aussi les prolonger par continuité en certains points de $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$.

En ce qui concerne $x + y$, posons $A' = ]-\infty, +\infty]$, $A'' = [-\infty, +\infty[$; on a la proposition suivante:

#### Proposition 7 {#top-iv-s4-prop-7 .statement}

*La fonction $x + y$ peut être prolongée par continuité à chacun des ensembles $A' \times A'$, $A'' \times A''$, suivant les formules*

$$
(2)
\begin{cases}
x + (+\infty) = (+\infty) + x = +\infty & (x \neq -\infty) \\
x + (-\infty) = (-\infty) + x = -\infty & (x \neq +\infty).
\end{cases}
$$

Montrons par exemple que, lorsque $(x, y)$ tend vers le point $(a, +\infty)$ ($a \neq -\infty$), en restant dans $\mathbf{R} \times \mathbf{R}$, $x + y$ tend vers $+\infty$. En effet, il existe un nombre fini $b < a$, et l’intervalle $]b, +\infty]$ est un voisinage de $a$ dans $\overline{\mathbf{R}}$; quel que soit $c$ fini, les relations $x > b, y > c - b$ entraînent $x + y > c$, ce qui montre que $x + y$ est aussi voisin qu’on veut de $+\infty$ lorsque $(x, y)$ est assez voisin de $(a, +\infty)$. On raisonne de même dans les autres cas.

Par contre $x + y$ *n’a pas de limite* aux points $(- \infty, +\infty)$ et $(+\infty, -\infty)$ de $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$; en effet, si $x + y$ avait une limite $k$ (finie ou infinie) lorsque $(x, y)$ tend vers $(+\infty, -\infty)$ en restant dans $\mathbf{R} \times \mathbf{R}$, il en résulterait que, pour tout $a$ fini, la fonction $(x + a) - x$ tendrait vers $k$ lorsque $x$ tend vers $+\infty$ en restant dans $\mathbf{R}$, ce qui est absurde, puisque $(x + a) - x = a$, et que $a$ est arbitraire.

La fonction $x + y$ applique $A' \times A'$ (resp. $A'' \times A''$) dans $A'$ (resp. $A''$). C’est donc une *loi de composition* dans $A'$ (resp. $A''$) qui prolonge l’addition dans $\mathbf{R}$; en vertu du principe de prolongement des identités (I, p. 53, cor. 1), cette loi est commutative et associative; 0 est élément neutre pour cette loi; le seul élément de A' non simplifiable (A, I, p. 15) est $+\infty$, d’après les formules (2).

Si $x, y, z, t$ sont des points de $\overline{\mathbf{R}}$ tels que $x \leq y$ et $z \leq t$, on a $x + z \leq y + t$ lorsque les deux membres de cette inégalité sont définis.

On notera que, dans $\overline{\mathbf{R}}$, la relation $x < y$ n’entraîne $x + z < y + z$ que lorsque $z$ est fini, d’après les formules (2); on vérifie aisément que les relations $x < y$ et $z < t$ entraînent encore $x + z < y + t$ lorsque les deux membres de cette inégalité ont un sens.

On pose encore, dans $\overline{\mathbf{R}}$, $x^+ = \sup(x, 0)$, $x^- = \sup(-x, 0)$, $|x| = \sup(x, -x)$; on a donc $(+\infty)^+ = (-\infty)^- = +\infty$, $(+\infty)^- = (-\infty)^+ = 0$,

$$
|+\infty| = |-\infty| = +\infty.
$$

Les sommes $x^+ - x^-$ et $x^+ + x^-$ ont un sens quel que soit $x \in \overline{\mathbf{R}}$, et valent donc respectivement $x$ et $|x|$ d’après le principe de prolongement des identités. En outre, chaque fois que la somme $x + y$ est définie, on a $|x + y| \leq |x| + |y|$.

On notera par contre que les formules (6) et (7) de IV, p. 2, peuvent cesser d’avoir un sens pour certaines valeurs de $x$ et $y$ dans $\overline{\mathbf{R}}$; par exemple, pour $x = -\infty$, $y = 0$, on a $\sup(x, y) = 0$, mais la somme $x + (y - x)^+$ n’est pas définie, car $(y - x)^+ = +\infty$.

Désignons maintenant par $\overline{\mathbf{R}}^*$ le complémentaire de 0 dans $\overline{\mathbf{R}}$; l’analogue de la prop. 7 pour la multiplication est la suivante:

#### Proposition 8 {#top-iv-s4-prop-8 .statement}

*La fonction xy peut être prolongée par continuité à l’ensemble $\overline{\mathbf{R}}^* \times \overline{\mathbf{R}}^*$, suivant les formules*

$$
\begin{cases}
x.(+\infty) = (+\infty).x = \begin{cases} +\infty & \text{si } x > 0 \\ -\infty & \text{si } x < 0 \end{cases} \\
x.(-\infty) = (-\infty).x = \begin{cases} -\infty & \text{si } x > 0 \\ +\infty & \text{si } x < 0. \end{cases}
\end{cases}
$$

Nous laissons au lecteur la démonstration de cette proposition, qui est analogue à celle de la prop. 7.

On voit de même que $xy$ n’a pas de limite aux points $(0, +\infty)$, $(+\infty, 0)$, $(0, -\infty)$, $(- \infty, 0)$ de $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$.

La fonction $xy$ est une *loi de composition* dans $\overline{\mathbf{R}}^*$, prolongeant la multiplication dans $\mathbf{R}^*$; cette loi est *associative* et *commutative* (principe de prolongement des identités); elle admet 1 pour élément unité; les éléments non simplifiables dans $\overline{\mathbf{R}}^*$ sont $+\infty$ et $-\infty$.

Si $x \leq y$ et $z > 0$, on a $xz \leq yz$ lorsque les deux membres de cette inégalité sont définis; lorsque le produit $xy$ a un sens, il en est de même de $|x|.|y|$, et on a $|xy| = |x|.|y|$.

Enfin, la formule de distributivité

$$
x(y + z) = xy + xz
$$

est encore valable, en vertu du principe de prolongement des identités, lorsque toutes les opérations qui figurent aux deux membres sont définies.

On notera que le premier membre de (4) peut avoir un sens sans que le second soit défini ; il suffit de considérer par exemple le cas où $x = +\infty, y = 2, z = -1$. Il faut donc n’user qu’avec précaution de la formule de distributivité dans $\overline{\mathbf{R}}$.

Enfin, pour tout $\varepsilon > 0$, la relation $|x| \geq \varepsilon$ entraîne $|1/x| \leq \varepsilon$, donc la fonction $1/x$, définie dans $\mathbf{R}^*$, a pour limite 0 lorsque $x$ tend vers $+\infty$ ou $-\infty$; elle se prolonge donc par continuité à $\overline{\mathbf{R}}^*$.

## EXERCICES {#top-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
