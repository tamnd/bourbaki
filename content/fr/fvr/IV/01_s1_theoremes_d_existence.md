---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: ÉQUATIONS DIFFÉRENTIELLES
section: 1
section_title: Théorèmes d'existence
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0160-0175, 0196-0200
extraction: ocr
subsections:
    - "no": 1
      title: La notion d’équation différentielle
      page: 0
      pdf_page: 160
    - "no": 2
      title: Équations différentielles admettant pour solutions des primitives de fonctions réglées
      page: 2
      pdf_page: 161
    - "no": 3
      title: Existence de solutions approchées
      page: 4
      pdf_page: 163
    - "no": 4
      title: Comparaison des solutions approchées
      page: 7
      pdf_page: 166
    - "no": 5
      title: Existence et unicité des solutions des équations lipschitziennes et localement lipschitziennes
      page: 10
      pdf_page: 169
    - "no": 6
      title: Continuité des intégrales en fonction d’un paramètre
      page: 13
      pdf_page: 172
    - "no": 7
      title: Dépendance des conditions initiales
      page: 14
      pdf_page: 173
statements: 29
exercises: 18
content_sha256: 244c14cc6ceeac67c63e543e1fdfe21015957882d5b1eaf06db34f3ff10aa2bb
---

## § 1. THÉORÈMES D’EXISTENCE

### 1. La notion d’équation différentielle

Soient I un intervalle contenu dans $\mathbf{R}$ et non réduit à un point, E un espace vectoriel topologique sur $\mathbf{R}$, A et B deux parties ouvertes de E. Soit $(\mathbf{x}, \mathbf{y}, t) \mapsto g(\mathbf{x}, \mathbf{y}, t)$ une application de $A \times B \times I$ dans E; à toute application dérivable $u$ de I dans A, dont la dérivée prend ses valeurs dans B, faisons correspondre l’application $t \mapsto g(u(t), u'(t), t)$ de I dans E, que nous désignerons par $\tilde{g}(u)$; $\tilde{g}$ est donc définie dans l’ensemble $\mathcal{D}(A, B)$ des applications dérivables de I dans A, dont la dérivée prend ses valeurs dans B. Nous dirons que l’équation $\tilde{g}(u) = 0$ est une équation différentielle en $u$ (relativement à la variable réelle $t$); une solution de cette équation est encore appelée intégrale de l’équation différentielle (dans l’intervalle I); c’est donc une application dérivable de I dans A, dont la dérivée prend ses valeurs dans B, et qui est telle que $g(u(t), u'(t), t) = 0$ pour tout $t \in I$. Par abus de langage, nous écrirons l’équation différentielle $\tilde{g}(u) = 0$ sous la forme

$$
g(\mathbf{x}, \mathbf{x}', t) = 0,
$$

étant sous-entendu que $\mathbf{x}$ est un élément de l’ensemble $\mathcal{D}(A, B)$.

Par exemple, pour $I = E = \mathbf{R}$, les relations
$$
x' = 2t, \quad tx' - 2x = 0, \quad {x'}^2 - 4x = 0, \quad x - t^2 = 0
$$
sont des équations différentielles, qui admettent toutes quatre pour solution la fonction $x(t) = t^2$.

Dans ce chapitre, nous ne considérerons en principe que le cas où E est un espace normé complet sur $\mathbf{R}$, et où les équations différentielles sont de la forme particulière
(1)
$$
\mathbf{x}' = \mathbf{f}(t, \mathbf{x})
$$

(« équations résolues par rapport à x' »), f désignant une fonction à valeurs dans E, définie dans I × H, où H est une partie ouverte non vide de E. Nous élargirons d’autre part un peu la notion de solution (ou intégrale) d’une telle équation (dans l’intervalle I) : nous dirons qu’une fonction u définie et continue dans I, à valeurs dans H, est une solution (ou intégrale) de l’équation (1) s’il existe une partie dénombrable A de I telle qu’en tout point t du complémentaire de A par rapport à I, u admette une dérivée u'(t) telle que u'(t) = f(t, u(t)). Si u est dérivable et vérifie la relation précédente en tout point t ∈ I, nous dirons que c’est une solution stricte de l’équation (1) dans I.

Dans le cas particulier d’une équation différentielle de la forme x' = f(t), f étant une application de I dans E, les solutions au sens précédent sont les primitives de la fonction f (II, p. 1), et les solutions strictes sont les primitives strictes.

Lorsque E est un produit d’espaces normés complets E_i (1 ≤ i ≤ n), on peut écrire x = (x_i)_{1 ≤ i ≤ n} et f = (f_i)_{1 ≤ i ≤ n} où x_i est une application de I dans E_i, et f_i une application de I × H dans E_i; l’équation (1) est alors équivalente au système d’équations différentielles

$$
\text{x}'_i = f_i(t, x_1, x_2, \ldots, x_n) \quad (1 ≤ i ≤ n).
$$

Le cas le plus important est celui où tous les E_i sont égaux à \mathbf{R} ou à \mathbf{C}; on dit alors que (2) est un système d’équations différentielles scalaires.

À l’étude des systèmes (2) se ramène celle des relations de la forme

$$
\text{x}^{(n)} = f(t, \text{x}, \text{x}', \ldots, \text{x}^{(n-1)})
$$

où x est une fonction vectorielle n fois dérivable dans I: en posant en effet x_1 = x, x_p = x^{(p-1)} pour 2 ≤ p ≤ n, la relation (3) est équivalente au système

$$
\begin{cases}
\text{x}'_i = \text{x}_{i+1} & (1 ≤ i ≤ n-1) \\
\text{x}'_n = f(t, \text{x}_1, \text{x}_2, \ldots, \text{x}_n).
\end{cases}
$$

Une relation de la forme (3) est appelée équation différentielle d’ordre n (résolue par rapport à x^{(n)}); par opposition, les équations de la forme (1) sont dites équations différentielles du premier ordre.

On ramène de même à un système de la forme (2) tout « système d’équations différentielles » de la forme

$$
D^n \text{x}_i = f_i(t, \text{x}_1, D\text{x}_1, \ldots, D^{n-1}\text{x}_1, \ldots, \text{x}_p, D\text{x}_p, \ldots, D^{n-p}\text{x}_p)
$$
(1 ≤ i ≤ p), où x_i est une fonction n_i fois dérivable dans I (pour 1 ≤ i ≤ p).

### 2. Équations différentielles admettant pour solutions des primitives de fonctions réglées

Rappelons (II, p. 4, déf. 3) qu’une fonction vectorielle u définie dans un intervalle I ⊂ \mathbf{R} est dite réglée si, dans toute partie compacte de I, elle est limite uniforme de fonctions en escalier; une condition équivalente est qu’en tout point intérieur à I, u ait une limite à droite et une limite à gauche, ainsi qu’une limite à droite à l’origine de I et une limite à gauche à l’extrémité de I, lorsque ces points appartiennent à I (II, p. 5, th. 3). Nous allons dans ce chapitre nous restreindre aux équations différentielles (1) dont toute solution est une primitive d’une fonction réglée dans I. Cette condition est évidemment satisfaite si, pour toute application continue u de I dans H, la fonction f(t, u(t)) est réglée dans I; le lemme suivant donne une condition suffisante pour qu’il en soit ainsi:

#### Lemme 1 {#fvr-iv-s1-lem-1 .statement}

Soit f une application de I × H dans E telle que, en désignant par fx (pour tout x ∈ H) l’application t ↦ f(t, x) de I dans E, les conditions suivantes soient réalisées:
1° fx est réglée dans I pour tout x ∈ H; 2° l’application x ↦ fx de H dans l’ensemble F(I, E) des applications de I dans E est continue quand on munit F(I, E) de la topologie de la convergence compacte (TG, X, p. 04). Dans ces conditions:
1° Pour toute application continue u de I dans H, la fonction t ↦ f(t, u(t)) est réglée dans I; de façon précise, la limite à droite (resp. à gauche) de cette fonction en un point t₀ ∈ I est égale à la limite à droite (resp. à gauche) de la fonction t ↦ f(t, u(t₀)) au point t₀.
2° Si (uₙ) est une suite d’applications de I dans H, qui converge uniformément vers une application continue u de I dans H, dans toute partie compacte de I, la suite des fonctions f(t, uₙ(t)) converge uniformément vers f(t, u(t)) dans toute partie compacte de I.
1° Soit c la limite à droite de f(t, u(t₀)) au point t₀; pour tout ε > 0, il existe un voisinage compact V de t₀ dans I tel que l’on ait \|f(t, u(t₀)) − c\| ≤ ε pour t ∈ V et t > t₀. D’autre part, il existe δ > 0 tel que les relations
x ∈ H,\quad \|x − u(t₀)\| ≤ δ
entraînent \|f(s, x) − f(s, u(t₀))\| ≤ ε pour tout s ∈ V; si W ⊂ V est un voisinage de t₀ dans I tel que l’on ait \|u(t) − u(t₀)\| ≤ δ pour tout t ∈ W, on aura donc \|f(t, u(t)) − c\| ≤ 2ε pour t ∈ W et t > t₀, ce qui prouve que c est limite à droite de f(t, u(t)) au point t₀.
2° Soit K une partie compacte de I; comme u est continue dans I, u(K) est une partie compacte de H; pour tout ε > 0 et tout x ∈ u(K) il existe un nombre δₓ tel que, pour y ∈ H, \|y − x\| ≤ δₓ et pour tout t ∈ K, on ait \|f(t, y) − f(t, x)\| ≤ ε. Il existe un nombre fini de points xᵢ ∈ u(K) tels que les boules fermées de centre xᵢ et de rayon $\frac{1}{2} \delta_{x_i}$ forment un recouvrement de u(K); soit δ = Min (δₓᵢ). Par hypothèse, il existe un entier n₀ tel que pour n ≥ n₀, on ait \|uₙ(t) − u(t)\| ≤ $\frac{1}{2} \delta$ pour tout t ∈ K. Or, pour tout t ∈ K, il existe un indice i tel que
\|u(t) − xᵢ\| ≤ $\frac{1}{2} \delta_{x_i}$;
par suite, on a \|uₙ(t) − xᵢ\| ≤ δₓᵢ, d’où \|f(t, uₙ(t)) − f(t, u(t))\| ≤ 2ε pour tout t ∈ K et tout n ≥ n₀.

Dans toute la suite de ce paragraphe, I désignera un intervalle contenu dans $\mathbf{R}$ et non réduit à un point, H un ensemble ouvert non vide contenu dans l’espace normé E, f une application de $I \times H$ dans E satisfaisant aux conditions du lemme 1.

#### Proposition 1 {#fvr-iv-s1-prop-1 .statement}

Soient $t_0$ un point de I, $x_0$ un point de H ; pour qu’une fonction continue u soit une solution de l’équation (1) dans I et prenne la valeur $x_0$ au point $t_0$, il faut et il suffit qu’elle vérifie la relation

$$
u(t) = x_0 + \int_{t_0}^t f(s, u(s)) \, ds
$$

pour tout $t \in I$.

En effet, d’après le lemme 1, si u est solution de (1) dans I, $f(t, u(t))$ est réglée, donc le second membre de (6) est défini et égal à $u(t)$ pour tout $t \in I$. Réciproquement, si u est une fonction continue satisfaisant à (6), $f(t, u(t))$ est réglée d’après le lemme 1, donc u a pour dérivée $f(t, u(t))$ sauf aux points d’une partie dénombrable de I.

#### Corollaire {#fvr-iv-s1-n2-cor-1 .statement}

En tout point de I distinct de l’origine (resp. de l’extrémité) de cet intervalle, toute solution u de (1) dans I admet une dérivée à gauche (resp. à droite) égale à la limite à gauche (resp. à droite) de $f(t, u(t))$ en ce point.

#### Proposition 2 {#fvr-iv-s1-prop-2 .statement}

Si f est une application continue de $I \times H$ dans E, toute solution de l’équation (1) dans I est une solution stricte.

En effet, une telle solution u est primitive de la fonction continue $f(t, u(t))$ (II, p. 16, prop. 3).

On notera d’ailleurs qu’une fonction f continue dans $I \times H$ vérifie les conditions du lemme 1 (TG, X, p. 13, cor. 3).

Dans ce qui suit, nous allons nous donner arbitrairement $t_0 \in I$ et $x_0 \in H$, et chercher s’il existe dans I (ou dans un voisinage de $t_0$ par rapport à I) des solutions de (1) prenant la valeur $x_0$ au point $t_0$ (ou, ce qui revient au même, des solutions de (6)).

### 3. Existence de solutions approchées

Étant donné un nombre $\varepsilon > 0$, nous dirons qu’une application continue u de I dans H est une solution approchée à $\varepsilon$ près de l’équation différentielle

$$
x' = f(t, x)
$$

si, en tous les points du complémentaire par rapport à I d’un ensemble dénombrable, u admet une dérivée qui satisfait à la condition

$$
\|u'(t) - f(t, u(t))\| \leq \varepsilon.
$$

Soit $(t_0, x_0)$ un point de $I \times H$; $f$ satisfaisant par hypothèse aux conditions du lemme 1 (IV, p. 3), il existe un voisinage compact $J$ de $t_0$ dans $I$ tel que $f(t, x_0)$ soit bornée dans $J$, et une boule ouverte $S$ de centre $x_0$, contenue dans $H$, telle que $f(t, x) - f(t, x_0)$ soit bornée dans $J \times S$; il en résulte que $f(t, x)$ est bornée dans $J \times S$. Dans tout ce n°, $J$ désignera un intervalle compact, voisinage de $t_0$ dans $I$, $S$ une boule ouverte de centre $x_0$ et de rayon $r$, contenue dans $H$, $J$ et $S$ étant tels que $f$ soit bornée dans $J \times S$; $M$ désignera la borne supérieure de $\|f(t, x)\|$ dans $J \times S$.

#### Proposition 3 {#fvr-iv-s1-prop-3 .statement}

*Dans tout intervalle compact d’origine (ou d’extrémité) $t_0$, contenu dans $J$ et de longueur $< r/(M + \varepsilon)$, il existe une solution approchée à $\varepsilon$ près de l’équation (1), à valeurs dans $S$, et égale à $x_0$ au point $t_0$.*

Nous allons supposer que $t_0$ n’est pas l’extrémité de $J$, et démontrer la proposition pour les intervalles d’origine $t_0$. Soit $\mathfrak{M}$ l’ensemble des solutions approchées de (1) à $\varepsilon$ près, dont chacune prend ses valeurs dans $S$, est égale à $x_0$ au point $t_0$, et est définie dans un intervalle semi-ouvert $[t_0, b[$ contenu dans $J$ (intervalle dépendant de la solution approchée que l’on considère). Montrons d’abord que $\mathfrak{M}$ n’est pas vide. Soit $c$ la limite à droite de $f(t, x_0)$ au point $t_0$; d’après le lemme 1 (IV, p. 3), la fonction $f(t, x_0 + c(t - t_0))$ a une limite à droite égale à $c$ au point $t_0$, donc la restriction de la fonction $x_0 + c(t - t_0)$ à un intervalle semi-ouvert $[t_0, b[$ assez petit appartient à $\mathfrak{M}$.

Ordonnons l’ensemble $\mathfrak{M}$ par la relation «$u$ est une restriction de $v$», et montrons que $\mathfrak{M}$ est *inductif* (E, III, p. 20). Soit $(u_\alpha)$ une partie totalement ordonnée de $\mathfrak{M}$, et soit $[t_0, b_\alpha[$ l’intervalle où $u_\alpha$ est définie: pour $b_\alpha \leq b_\beta$, $u_\beta$ est donc un prolongement de $u_\alpha$. La réunion des intervalles $[t_0, b_\alpha[$ est un intervalle $[t_0, b[$ contenu dans $J$, et il existe une fonction et une seule $u$ définie dans $[t_0, b[$ et coïncidant avec $u_\alpha$ dans $[t_0, b_\alpha[$ pour tout $\alpha$; parmi les $b_\alpha$, il existe une suite croissante $(b_{\alpha_n})$ tendant vers $b$; comme $u$ coïncide avec $u_{\alpha_n}$ dans $[t_0, b_{\alpha_n}[$, $u$ admet, en tous les points du complémentaire par rapport à $[t_0, b[$ d’un ensemble *dénombrable*, une dérivée vérifiant la relation (7), et est donc la borne supérieure de l’ensemble $(u_\alpha)$ dans $\mathfrak{M}$.

D’après le th. de Zorn (E, III, p. 20, th. 2), $\mathfrak{M}$ admet un élément maximal $u_0$; nous allons montrer que si $[t_0, t_1[$ est l’intervalle où est définie $u_0$, ou bien $t_1$ est l’extrémité de $J$, ou bien $t_1 - t_0 \geq r/(M + \varepsilon)$. Raisonnons par l’absurde, en supposant qu’aucune de ces deux hypothèses ne soit vérifiée; montrons d’abord qu’on peut prolonger $u_0$ par continuité au point $t_1$: en effet, quels que soient $s$ et $t$ dans $[t_0, t_1[$, on a

$$
\|u_0(s) - u_0(t)\| \leq (M + \varepsilon)|s - t|
$$

d’après le th. des accroissements finis; le critère de Cauchy montre donc que $u_0$ admet une limite à gauche $x_1 \in S$ au point $t_1$. Soit alors $c_1$ la limite à droite au point $t_1$ de la fonction $f(t, x_1)$; on a $\|c_1\| \leq M$; le même raisonnement qu’au début de la démonstration montre qu’on peut prolonger $u_0$ dans un intervalle semi-ouvert d’origine $t_1$, par la fonction $x_1 + c_1(t - t_1)$, de sorte que la fonction prolongée appartienne encore à $\mathbf{R}$, ce qui est absurde. La proposition est donc démontrée.

Lorsque $f$ est uniformément continue dans $J \times S$, on peut démontrer la prop. 3 sans faire usage du th. de Zorn (IV, p. 37, exerc. 1 a)).

#### Proposition 4 {#fvr-iv-s1-prop-4 .statement}

L’ensemble des solutions approchées de (1) à $\varepsilon$ près définies dans un même intervalle $K \subset J$, et prenant leurs valeurs dans $S$, est uniformément équicontinu.

En effet, si $u$ est une fonction quelconque appartenant à cet ensemble, $s$ et $t$ deux points de $K$, on a, d’après le th. des accroissements finis,

$$
\|u(s) - u(t)\| \leq (M + \varepsilon)|s - t|.
$$

#### Corollaire (théorème de Peano) {#fvr-iv-s1-n3-cor-1 .statement}

Si $E$ est de dimension finie sur $\mathbf{R}$, dans tout intervalle compact $K$ d’origine (ou d’extrémité) $t_0$, contenu dans $J$ et de longueur $< r/M$, il existe une solution de (1) à valeurs dans $S$, égale à $x_0$ au point $t_0$.

En effet, d’après la prop. 3, dès que $n$ est assez grand, il existe une solution approchée $u_n$ de l’équation (1) à $1/n$ près, définie dans $K$, à valeurs dans $S$, et égale à $x_0$ au point $t_0$. En outre, à partir d’une certaine valeur de $n$, $u_n(K)$ est contenu dans une boule fermée de centre $x_0$ et de rayon $< r$, indépendant de $n$. L’ensemble des $u_n$ est équicontinu (prop. 4), et comme $E$ est de dimension finie, $S$ est relativement compacte dans $E$, donc pour tout $t \in K$, l’ensemble des $u_n(t)$ est relativement compact dans $E$. D’après le th. d’Ascoli (TG, X, p. 17, th. 2), l’ensemble des $u_n$ est relativement compact dans l’espace $\mathcal{F}(K; E)$ des applications de $K$ dans $E$, muni de la topologie de la convergence uniforme. Il existe donc une suite $(u_{n_k})$ extraite de $(u_n)$, qui converge uniformément dans $K$ vers une fonction continue $u$. On a $u(K) \subset S$ et par suite $t \mapsto f(t, u(t))$ est définie dans $K$; en vertu du lemme 1 (IV, p. 3), $f(t, u_{n_k}(t))$ converge uniformément vers $f(t, u(t))$ dans $K$; d’après (IV, p. 4, formule (7)), $u_{n_k}$ est primitive d’une fonction qui tend uniformément vers $f(t, u(t))$ dans $K$, donc (II, p. 2, th. 1) $u$ est solution de (1) dans $K$, égale à $x_0$ au point $t_0$.

#### Remarque 1 {#fvr-iv-s1-n3-rem-1 .statement}

Il peut exister une infinité d’intégrales d’une équation différentielle (1), prenant la même valeur en un point donné. Par exemple, l’équation différentielle scalaire $x' = 2 \sqrt{|x|}$ admet pour intégrales prenant la valeur 0 au point $t = 0$ toutes les fonctions définies par

$$
\begin{align*}
u(t) &= 0 & \text{pour } -\beta \leq t \leq \alpha \\
u(t) &= -(t + \beta)^2 & \text{pour } t \leq -\beta \\
u(t) &= (t - \alpha)^2 & \text{pour } t \geq \alpha
\end{align*}
$$

quels que soient les nombres positifs $\alpha$ et $\beta$.

#### Remarque 2 {#fvr-iv-s1-n3-rem-2 .statement}

Le th. de Peano n’est plus exact lorsque $E$ est un espace normé complet quelconque de dimension infinie (IV, p. 41, exerc. 18).

### 4. Comparaison des solutions approchées

Dans ce qui suit, I et H désignent, comme ci-dessus, un intervalle contenu dans $\mathbf{R}$ et un ensemble ouvert dans l’espace normé E, respectivement; $t_0$ est un point de I.

#### Définition 1 {#fvr-iv-s1-def-1 .statement}

Etant donnée une fonction numérique positive $t \mapsto k(t)$ définie dans I, on dit qu’une application $\mathbf{f}$ de $I \times H$ dans E est lipschitzienne pour la fonction $k(t)$ si, pour tout $x \in H$, la fonction $t \mapsto \mathbf{f}(t, x)$ est réglée dans I, et si, pour tout $t \in I$ et tout couple de points $x_1, x_2$ de H, on a (« condition de Lipschitz »)

$$
\| \mathbf{f}(t, x_1) - \mathbf{f}(t, x_2) \| \leq k(t) \| x_1 - x_2 \|.
$$

On dira que $\mathbf{f}$ est lipschitzienne (sans préciser) dans $I \times H$ si elle est lipschitzienne dans cet ensemble pour une certaine constante $k \geq 0$. Il est immédiat qu’une fonction lipschitzienne dans $I \times H$ satisfait aux conditions du lemme 1 de IV, p. 3 (la réciproque étant inexacte); lorsque $\mathbf{f}$ est lipschitzienne (dans $I \times H$), on dit que l’équation différentielle

$$
x' = \mathbf{f}(t, x)
$$

est lipschitzienne (dans $I \times H$).

#### Exemple {#fvr-iv-s1-n4-exa-1 .statement}

Lorsque $E = \mathbf{R}$, et que H est un intervalle dans $\mathbf{R}$, si en tout point $(t, x)$ de $I \times H$ la fonction $f(t, x)$ admet une dérivée partielle $f'_x$ (II, p. 24) telle que $|f'_x(t, x)| \leq k(t)$ dans $I \times H$, la condition (8) est vérifiée en vertu du th. des accroissements finis; nous verrons plus tard comment cet exemple se généralise au cas où E est un espace normé quelconque.

Si $\mathbf{f}$ est lipschitzienne dans $I \times H$, pour tout intervalle compact $J \subset I$ et toute boule ouverte $S \subset H$, $\mathbf{f}$ est bornée dans $J \times S$. La prop. 3 (IV, p. 5) est donc applicable, et démontre l’existence de solutions approchées de l’équation (1). Mais on a en outre la proposition suivante, qui permet de comparer deux solutions approchées:

#### Proposition 5 {#fvr-iv-s1-prop-5 .statement}

Soient $k(t)$ une fonction numérique réglée et $> 0$ dans I, $\mathbf{f}(t, x)$ une fonction définie et lipschitzienne pour la fonction $k(t)$ dans $I \times H$. Si $u$ et $v$ sont deux solutions approchées de l’équation (1) à $\varepsilon_1$ et $\varepsilon_2$ près respectivement, définies dans I et prenant leurs valeurs dans H, on a, pour tout $t \in I$ tel que $t \geq t_0$,

$$
\| u(t) - v(t) \| \leq \| u(t_0) - v(t_0) \| \Phi(t) + (\varepsilon_1 + \varepsilon_2) \Psi(t)
$$

où

$$
\begin{cases}
\Phi(t) = 1 + \int_{t_0}^t k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) ds \\
\Psi(t) = t - t_0 + \int_{t_0}^t (s - t_0) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) ds.
\end{cases}
$$

De la relation $\|u'(t) - f(t, u(t))\| \leq \varepsilon_1$, valable dans le complémentaire d’un ensemble dénombrable, on déduit, par application du th. des accroissements finis
$$
\|u(t) - u(t_0) - \int_{t_0}^t f(s, u(s))\ ds\| \leq \varepsilon_1 (t - t_0)
$$
et de même
$$
\|v(t) - v(t_0) - \int_{t_0}^t f(s, v(s))\ ds\| \leq \varepsilon_2 (t - t_0)
$$
d’où
$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\|
+ \left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\ ds \right\| + (\varepsilon_1 + \varepsilon_2)(t - t_0).
$$
D’après la condition de Lipschitz (8), on a
$$
\left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\ ds \right\| \leq \int_{t_0}^t \|f(s, u(s)) - f(s, v(s))\|\ ds
\leq \int_{t_0}^t k(s)\|u(s) - v(s)\|\ ds
$$
d’où, en posant $w(t) = \|u(t) - v(t)\|$,
$$
w(t) \leq w(t_0) + (\varepsilon_1 + \varepsilon_2)(t - t_0) + \int_{t_0}^t k(s)w(s)\ ds.
$$
La proposition est alors conséquence du lemme suivant:

#### Lemme 2 {#fvr-iv-s1-lem-2 .statement}

Si, dans l’intervalle $[t_0, t_1]$, $w$ est une fonction numérique continue satisfaisant à l’inégalité
$$
w(t) \leq \varphi(t) + \int_{t_0}^t k(s)w(s)\ ds
$$
où $\varphi$ est une fonction réglée $\geq 0$ dans $[t_0, t_1]$, on a, pour $t_0 \leq t \leq t_1$
$$
w(t) \leq \varphi(t) + \int_{t_0}^t \varphi(s)k(s) \exp \left( \int_s^t k(\tau)\ d\tau \right) ds.
$$
Posons en effet $y(t) = \int_{t_0}^t k(s)w(s)\ ds$; la relation (12) entraîne que, dans le complémentaire d’un ensemble dénombrable, on a
$$
y'(t) - k(t)y(t) \leq \varphi(t)k(t).
$$
En posant $z(t) = y(t)\exp(-\int_{t_0}^t k(s)\ ds)$, la relation (14) équivaut à
$$
z'(t) \leq \varphi(t)k(t) \exp \left( -\int_{t_0}^t k(s)\ ds \right).
$$

Appliquant le th. des accroissements finis (I, p. 23, th. 2) à cette inégalité, il vient, puisque $z(t_0) = 0$

$$
z(t) \leq \int_{t_0}^t \varphi(s)k(s) \exp \left( - \int_{t_0}^s k(\tau) \, d\tau \right) ds
$$

d’où

$$
y(t) \leq \int_{t_0}^t \varphi(s)k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) ds
$$

et comme $w(t) \leq \varphi(t) + y(t)$, on obtient ainsi (13).

#### Corollaire {#fvr-iv-s1-n4-cor-1 .statement}

*Soit $\mathbf{f}$ une fonction lipschitzienne pour la constante $k > 0$, définie dans $I \times H$. Si $\mathbf{u}$ et $\mathbf{v}$ sont deux solutions approchées de (1) à $\varepsilon_1$ et $\varepsilon_2$ près respectivement, définies dans $I$ et prenant leurs valeurs dans $H$, on a, pour tout $t \in I$,

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$

Cette inégalité est en effet une conséquence immédiate de (9) lorsque $t \geq t_0$; pour la démontrer lorsque $t \leq t_0$, il suffit de l’appliquer à l’équation

$$
\frac{d\mathbf{x}}{ds} = -\mathbf{f}(-s, \mathbf{x})
$$

déduite de (1) par le changement de variable $t = -s$.

#### Remarque 1 {#fvr-iv-s1-n4-rem-1 .statement}

Lorsque $k = 0$, l’inégalité (15) est remplacée par l’inégalité

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| + (\varepsilon_1 + \varepsilon_2) |t - t_0|
$$

dont la démonstration est immédiate.

#### Remarque 2 {#fvr-iv-s1-n4-rem-2 .statement}

Lorsque $E$ est de dimension *finie*, et que $\mathbf{f}$ est lipschitzienne dans $I \times H$, on peut démontrer l’existence de solutions approchées de l’équation (1) (IV, p. 5, prop. 3) sans utiliser l’axiome de choix (IV, p. 37, exerc. 1b)).

#### Proposition 6 {#fvr-iv-s1-prop-6 .statement}

*Soient $\mathbf{f}$ et $\mathbf{g}$ deux fonctions définies dans $I \times H$, satisfaisant aux conditions du lemme 1 de IV, p. 3, et telles que, dans $I \times H$,

$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leq \alpha.
$$

On suppose en outre que $\mathbf{g}$ soit lipschitzienne pour la constante $k > 0$ dans $I \times H$. Dans ces conditions, si $\mathbf{u}$ est une solution approchée de $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ à $\varepsilon_1$ près, définie dans $I$, à valeurs dans $H$, et $\mathbf{v}$ une solution approchée de $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ à $\varepsilon_2$ près, définie dans $I$, à valeurs dans $H$, on a, pour tout $t \in I$

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\alpha + \varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$

En effet, on a, pour tout t dans le complémentaire par rapport à I d’une partie dénombrable de I,
$$
\|u'(t) - g(t, u(t))\| \leq \alpha + \varepsilon_1
$$
autrement dit, $u$ est solution approchée de $x' = g(t, x)$ à $\alpha + \varepsilon_1$ près, d’où l’inégalité (17) par application de la prop. 5 de IV, p. 7.

### 5. Existence et unicité des solutions des équations lipschitziennes et localement lipschitziennes

#### Théorème 1 (Cauchy) {#fvr-iv-s1-thm-1 .statement}

Soient $f$ une fonction lipschitzienne dans $I \times H$, J un intervalle compact contenu dans I et non réduit à un point, $t_0$ un point de J, S une boule ouverte de centre $x_0$ et de rayon r, contenue dans H, M la borne supérieure de $\|f(t, x)\|$ dans $J \times S$. Dans ces conditions, pour tout intervalle compact K non réduit à un point, contenu dans l’intersection de J et de $]t_0 - r/M, t_0 + r/M[$ et contenant $t_0$, il existe une solution et une seule de l’équation différentielle $x' = f(t, x)$, définie dans K, à valeurs dans S et égale à $x_0$ au point $t_0$.

En effet, pour tout $\varepsilon > 0$ assez petit, l’ensemble $F_\varepsilon$ des solutions approchées de (1) à $\varepsilon$ près, définies dans K, à valeurs dans S et égales à $x_0$ au point $t_0$, n’est pas vide (IV, p. 5, prop. 3); en outre, si $u$ et $v$ appartiennent à $F_\varepsilon$, on a, d’après (15) (IV, p. 9)
$$
\|u(t) - v(t)\| \leq 2\varepsilon \frac{e^{k|t-t_0|} - 1}{k}
$$
pour tout $t \in K$, donc les ensembles $F_\varepsilon$ forment une base de filtre $\mathcal{G}$ qui converge uniformément dans K vers une fonction continue $w$, égale à $x_0$ au point $t_0$; $w$ prend ses valeurs dans S, parce que, dès que $\varepsilon$ est assez petit, les fonctions $u \in F_\varepsilon$ prennent leurs valeurs dans une boule fermée contenue dans S. Comme $f(t, u(t))$ tend uniformément dans K vers $f(t, w(t))$ suivant $\mathcal{G}$, $w$ satisfait à l’équation (6) de IV, p. 4, donc est solution de (1). L’unicité de la solution découle aussitôt de l’inégalité (15) de IV, p. 9, où on fait $\varepsilon_1 = \varepsilon_2 = 0$ et $u(t_0) = v(t_0)$.

Nous dirons qu’une fonction $f$ définie dans $I \times H$ est localement lipschitzienne dans cet ensemble si, pour tout point $(t, x)$ de $I \times H$, il existe un voisinage V de t (par rapport à I) et un voisinage S de x tels que $f$ soit lipschitzienne dans $V \times S$ (pour une constante k dépendant de V et de S). En vertu du th. de Borel-Lebesgue, pour tout intervalle compact $J \subset I$ et tout point $x_0 \in H$, il existe une boule ouverte S de centre $x_0$, contenue dans H, telle que $f$ soit lipschitzienne dans $J \times S$; $f$ satisfait donc aux conditions du lemme 1 de IV, p. 3. Lorsque $f$ est localement lipschitzienne dans $I \times H$, nous dirons que l’équation $x' = f(t, x)$ est localement lipschitzienne dans $I \times H$.

Nous allons généraliser et préciser le th. 1 de IV, p. 10 pour les équations localement lipschitziennes; nous nous bornerons au cas où $t_0$ est l’origine de l’intervalle I; on passe aisément de là au cas où $t_0$ est un point quelconque de I (cf. IV, IV, p. 9, corollaire).

#### Théorème 2 {#fvr-iv-s1-thm-2 .statement}

Soient $I \subset \mathbf{R}$ un intervalle (non réduit à un point) d’origine $t_0 \in I$, $H$ une partie ouverte non vide de $E$, $f$ une fonction localement lipschitzienne dans $I \times H$.

1° Pour tout $x_0 \in H$, il existe un plus grand intervalle $J \subset I$, d’origine $t_0 \in J$, dans lequel il existe une intégrale $u$ de l’équation $x' = f(t, x)$, prenant ses valeurs dans $H$ et égale à $x_0$ au point $t_0$; cette intégrale est unique.

2° Si $J \neq I$, $J$ est un intervalle semi-ouvert $(t_0, \beta[$ de longueur finie ; en outre, pour toute partie compacte $K \subset H$, $\overline{u}^1(K)$ est alors une partie compacte de $\mathbf{R}$.

3° Si $J$ est borné, et si $f(t, u(t))$ est bornée dans $J$, $u(t)$ a une limite à gauche $c$ à l’extrémité de $J$; en outre, si $J \neq I$, $c$ est un point frontière de $H$ dans $E$.

1° Soit $\mathfrak{M}$ l’ensemble des intervalles $L$ (non réduits à un point) d’origine $t_0 \in L$, contenus dans $I$ et tels que, dans $L$, il existe une solution de (1) (IV, p. 2) à valeurs dans $H$ et égale à $x_0$ au point $t_0$; d’après le th. 1 (IV, p. 10), l’ensemble $\mathfrak{M}$ n’est pas vide. Soient $L, L'$ deux intervalles appartenant à $\mathfrak{M}$, et supposons par exemple que $L \subset L'$; si $u$ et $v$ sont deux intégrales de (1), définies respectivement dans $L$ et $L'$, à valeurs dans $H$ et égales à $x_0$ au point $t_0$, nous allons voir que $v$ est un prolongement de $u$. En effet, soit $t_1$ la borne supérieure de l’ensemble des $t \in L$ tels que $u(s) = v(s)$ pour $t_0 \leq s \leq t$; nous allons prouver que $t_1$ est l’extrémité de $L$. Dans le cas contraire, on aurait $u(t_1) = v(t_1)$ par continuité, et $x_1 = u(t_1)$ appartiendrait à $H$; comme $f$ est localement lipschitzienne, le th. 1 prouve qu’il ne peut exister qu’une seule intégrale de (1) définie dans un voisinage de $t_1$, à valeurs dans $H$ et égale à $x_1$ au point $t_1$; il y a donc contradiction à supposer que $t_1$ ne soit pas l’extrémité de $L$. Nous voyons donc que, si $J$ est la réunion des intervalles $L \in \mathfrak{M}$, il existe une intégrale $u$ et une seule de (1), définie dans $J$, à valeurs dans $H$ et égale à $x_0$ au point $t_0$.

2° Supposons $J \neq I$, et soit $\beta$ l’extrémité de $J$; si $\beta$ est l’extrémité de $I$, on a $\beta \in I$ (donc $\beta$ est fini) et $J = (t_0, \beta[$ en vertu de l’hypothèse. Supposons donc que $\beta$ ne soit pas l’extrémité de $I$; si $\beta \in J$, $u(\beta) = c$ appartient à $H$; d’après le th. 1, il existe une intégrale de (1) à valeurs dans $H$, définie dans un intervalle

$$
[\beta, \beta_1[ \subset I
$$

et égale à $c$ au point $\beta$; $J$ ne serait donc pas le plus grand des intervalles de $\mathfrak{M}$, ce qui est absurde; on a donc bien $J = (t_0, \beta[$.

Si $K$ est une partie compacte de $H$, $\overline{u}^1(K)$ est fermé dans $J$; nous allons voir qu’il existe $\gamma \in J$ tel que $\overline{u}^1(K)$ soit contenu dans $(t_0, \gamma]$, ce qui prouvera que $\overline{u}^1(K)$ est compact. Dans le cas contraire, il existerait un point $c \in K$ tel que $(\beta, c)$ soit adhérent à l’ensemble des points $(t, u(t))$ tels que $t < \beta$ et $u(t) \in K$. Comme $\beta \in I$ et $c \in H$, il existerait un voisinage $V$ de $\beta$ dans $I$ et une boule ouverte $S$ de centre $c$ et de rayon $r$, contenue dans $H$, tels que $f$ soit lipschitzienne et bornée dans $V \times S$; soit $M$ la borne supérieure de $\|f(t, x)\|$ dans cet ensemble. Par hypothèse, il existe $t_1 \in J$ tel que $\beta - t_1 < r/2M, t_1 \in V$ et $\|u(t_1) - c\| \leq r/2$; le th. 1 montre qu’il existe une intégrale et une seule de (1), à valeurs dans $H$, définie dans un intervalle $(t_1, t_2)$ contenant $\beta$, et égale à $u(t_1)$ au point $t_1$; comme cette intégrale coïncide avec $u$ dans l’intervalle $(t_1, \beta]$, $J = (t_0, \beta[$ ne serait pas le plus grand des intervalles de $\mathfrak{M}$, ce qui est absurde.

3° Supposons que $J$ soit borné et que $\|\mathbf{f}(t, u(t))\| \leq M$ dans $J$; on a donc $\|u'(t)\| \leq M$ dans le complémentaire d’une partie dénombrable de $J$; par suite $\|u(s) - u(t)\| \leq M|s - t|$ quels que soient $s$ et $t$ dans $J$, en vertu du th. des accroissements finis; d’après le critère de Cauchy, $u$ a donc une limite à gauche $c$ à l’extrémité $\beta$ de $J$. Si $J \neq I$, $c$ ne peut appartenir à $H$, car en prolongeant $u$ par continuité au point $\beta$, $u$ serait une intégrale de (1) à valeurs dans $H$, définie dans l’intervalle $[t_0, \beta]$ et égale à $x_0$ au point $t_0$; on aurait donc $J = [t_0, \beta[$, contrairement à ce qu’on a vu au 2°.

#### Corollaire 1 {#fvr-iv-s1-thm-2-cor-1 .statement}

Si $H = E$ et $J \neq I$, $\mathbf{f}(t, u(t))$ n’est pas bornée dans $J$; si de plus $E$ est de dimension finie, $\|u(t)\|$ a pour limite à gauche $+\infty$ à l’extrémité de $J$.

La première partie est une conséquence immédiate de la troisième partie du th. 2. Si $E$ est de dimension finie, toute boule fermée $S \subset E$ est compacte, donc la seconde partie du th. 2 montre qu’il existe $\gamma \in J$ tel que $u(t) \notin S$ pour $t > \gamma$.

Si $E$ est de dimension infinie, il peut se faire que $J \neq I$, mais que $\|u(t)\|$ reste bornée lorsque $t$ tend vers l’extrémité de $J$ (IV, p. 37, exerc. 5).

#### Corollaire 2 {#fvr-iv-s1-thm-2-cor-2 .statement}

Si, dans $I \times H$, $\mathbf{f}$ est lipschitzienne pour une fonction réglée $k(t)$, et si l’extrémité $\beta$ de $J$ appartient à $I$, $u$ a une limite à gauche au point $\beta$; si $H = E$ et si $\mathbf{f}$ est lipschitzienne pour une fonction réglée $k(t)$ dans $I \times E$, on a $J = I$.

En effet, si $\beta \in I$, il existe un voisinage compact $V$ de $\beta$ dans $I$, tel que $\mathbf{f}(t, x_0)$ et $k(t)$ soient bornées dans $V$; on a donc $\|\mathbf{f}(t, x)\| \leq m\|x\| + h$ ($m$ et $h$ constantes) dans $V \times H$, d’où $\|u'(t)\| \leq m\|u(t)\| + h$ dans le complémentaire d’une partie dénombrable de $V \cap J$, et par suite $\|u(t)\| \leq m \int_{t_0}^t \|u(s)\| ds + q$ ($q$ constante) dans $V \cap J$; le lemme 2 (IV, p. 8) montre que $\|u(t)\| \leq c e^{mt} + d$ ($c$ et $d$ constantes) dans $V \cap J$, donc $\mathbf{f}(t, u(t))$ reste bornée dans $J$, et le corollaire résulte alors du th. 2 de IV, p. 11.

#### Exemple 1 {#fvr-iv-s1-n5-exa-1 .statement}

Pour une équation différentielle de la forme $x' = g(t)$, où $g$ est réglée dans $I$, toute intégrale $u$ est évidemment définie dans $I$ tout entier. On notera que $u$ peut être bornée dans $I$ sans que $g(t)$ le soit.

#### Exemple 2 {#fvr-iv-s1-n5-exa-2 .statement}

Pour l’équation scalaire $x' = \sqrt{1 - x^2}$, on a $I = \mathbf{R}$, $H = ]-1, 1[$. Si on prend $t_0 = x_0 = 0$, l’intégrale correspondante est $\sin t$ dans le plus grand intervalle contenant 0, où la dérivée de $\sin t$ soit positive, c’est-à-dire dans $]-\pi/2, +\pi/2[$; aux extrémités de cet intervalle, l’intégrale tend vers une extrémité de $H$.

#### Exemple 3 {#fvr-iv-s1-n5-exa-3 .statement}

Pour l’équation scalaire $x' = 1 + x^2$, on a $I = H = \mathbf{R}$; l’intégrale nulle pour $t = 0$ est $\operatorname{tg} t$, et le plus grand intervalle contenant 0, où cette fonction est continue, est $J = ]-\pi/2, +\pi/2[$; aux extrémités de $J$, $|\operatorname{tg} t|$ tend vers $+\infty$ (cf. IV, p. 12, cor. 1).

#### Exemple 4 {#fvr-iv-s1-n5-exa-4 .statement}

Pour l’équation scalaire $x' = \sin tx$, on a $I = H = \mathbf{R}$ et le second membre est borné dans $I \times H$, donc (IV, p. 12, cor. 1) toute intégrale est définie dans $\mathbf{R}$ tout entier.

### 6. Continuité des intégrales en fonction d’un paramètre

La prop. 6 (IV, p. 9) montre que lorsqu’une équation différentielle

$$
\mathbf{x}' = \mathbf{f}(t, \mathbf{x})
$$

est « voisine » d’une équation lipschitzienne $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ et qu’on suppose que les deux équations admettent chacune une solution approchée dans un même intervalle, ces deux solutions approchées sont « voisines »; nous allons préciser ce résultat en montrant que l’existence de solutions de l’équation lipschitzienne $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ dans un intervalle entraîne celle de solutions approchées de l’équation $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ dans le même intervalle pourvu que, dans ce dernier, les valeurs de la solution de $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ ne soient pas « trop voisines » de la frontière de H.

#### Proposition 7 {#fvr-iv-s1-prop-7 .statement}

Soient $\mathbf{f}$ et $\mathbf{g}$ deux fonctions définies dans $I \times H$, satisfaisant aux conditions du lemme 1 de IV, p. 3, et telles que, dans $I \times H$

$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leqslant \alpha.
$$

On suppose en outre que $\mathbf{g}$ soit lipschitzienne pour la constante $k > 0$ dans $I \times H$, et que $\mathbf{f}$ soit localement lipschitzienne dans $I \times H$, ou que $E$ soit de dimension finie. Soient $(t_0, \mathbf{x}_0)$ un point de $I \times H$, $\mu$ un nombre $> 0$, et

$$
\varphi(t) = \mu e^{k(t-t_0)} + \alpha \frac{e^{k(t-t_0)} - 1}{k}.
$$

Soit $\mathbf{u}$ une intégrale de l’équation $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$, définie dans un intervalle $K = [t_0, b[$ contenu dans $I$, égale à $\mathbf{x}_0$ au point $t_0$ et telle que, pour tout $t \in K$, la boule fermée de centre $\mathbf{u}(t)$ et de rayon $\varphi(t)$ soit contenue dans $H$. Dans ces conditions, pour tout $\mathbf{y} \in H$ tel que $\| \mathbf{y} - \mathbf{x}_0 \| \leqslant \mu$, il existe une intégrale $\mathbf{v}$ de $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$, définie dans $K$, à valeurs dans $H$, et égale à $\mathbf{y}$ au point $t_0$; en outre, on a $\| \mathbf{u}(t) - \mathbf{v}(t) \| \leqslant \varphi(t)$ dans $K$.

Soit $\mathfrak{M}$ l’ensemble des intégrales de $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$, dont chacune prend ses valeurs dans $H$, est égale à $\mathbf{y}$ au point $t_0$ et est définie dans un intervalle semi-ouvert $(t_0, t_1[$ contenu dans $I$ (dépendant de l’intégrale que l’on considère). D’après le th. 1 de IV, p. 10 (lorsque $\mathbf{f}$ est localement lipschitzienne) ou IV, p. 6, corollaire (lorsque $E$ est de dimension finie), $\mathfrak{M}$ n’est pas vide, et le même raisonnement que dans la prop. 3 de IV, p. 5, montre que $\mathfrak{M}$ est inductif quand on l’ordonne par la relation « $\mathbf{v}$ est une restriction de $\mathbf{w}$ ». Soit $\mathbf{v}_0$ un élément maximal de $\mathfrak{M}$, $[t_0, t_1[$ l’intervalle où est définie $\mathbf{v}_0$; d’après la prop. 6 de IV, p. 9, tout revient à prouver que $t_1 \geqslant b$. Dans le cas contraire, on aurait

$$
\| \mathbf{u}(t) - \mathbf{v}_0(t) \| \leqslant \varphi(t)
$$

dans l’intervalle $[t_0, t_1[$ (en vertu de la prop. 6; dans l’intervalle compact $[t_0, t_1]$, la fonction réglée $\mathbf{g}(t, \mathbf{u}(t))$ est bornée, donc, dans l’intervalle $[t_0, t_1[$, $\mathbf{g}(t, \mathbf{v}_0(t))$ est bornée, puisque l’on a $\| \mathbf{g}(t, \mathbf{v}_0(t)) \| \leqslant \| \mathbf{g}(t, \mathbf{u}(t)) \| + k \varphi(t)$ dans cet intervalle.

Comme $v_0$ est solution approchée de $x' = g(t, x)$ à $\alpha$ près dans $[t_0, t_1[$, il existe un nombre $M > 0$ tel que $\|v'_0(t)\| \leq M$ dans cet intervalle, sauf aux points d’un ensemble dénombrable; le th. des accroissements finis montre alors que $\|v_0(s) - v_0(t)\| \leq M|s - t|$ pour tout couple de points $s, t$ de $[t_0, t_1[$, donc (critère de Cauchy) $v_0(t)$ a une limite à gauche $c$ au point $t_1$, et, par continuité, on a $\|c - u(t_1)\| \leq \varphi(t_1)$, donc $c \in H$. On voit alors par IV, p. 10, th. 1 ou IV, p. 6, corollaire, qu’il existe une intégrale de $x' = f(t, x)$ définie dans un intervalle $[t_1, t_2[$ et égale à $c$ au point $t_1$, ce qui contredit la définition de $v_0$.

#### Théorème 3 {#fvr-iv-s1-thm-3 .statement}

Soient $F$ un espace topologique, $f$ une application de $I \times H \times F$ dans $E$ telle que, pour tout $\xi \in F$, $(t, x) \mapsto f(t, x, \xi)$ soit lipschitzienne dans $I \times H$, et que, lorsque $\xi$ tend vers $\xi_0$, $f(t, x, \xi)$ tende uniformément vers $f(t, x, \xi_0)$ dans $I \times H$. Soit $u_0(t)$ une intégrale de $x' = f(t, x, \xi_0)$, définie dans un intervalle $J = [t_0, b[$ contenu dans $I$, à valeurs dans $H$ et égale à $x_0$ au point $t_0$. Pour tout intervalle compact $(t_0, t_1]$ contenu dans $J$, il existe un voisinage $V$ de $\xi_0$ dans $F$ tel que, pour tout $\xi \in V$, l’équation $x' = f(t, x, \xi)$ ait une intégrale (et une seule) $u(t, \xi)$ définie dans $(t_0, t_1]$, à valeurs dans $H$ et égale à $x_0$ au point $t_0$; en outre, lorsque $\xi$ tend vers $\xi_0$, $u(t, \xi)$ tend uniformément vers $u_0(t)$ dans $(t_0, t_1]$.

En effet, soit $r > 0$ tel que, pour $t_0 \leq t \leq t_1$, la boule fermée de centre $u_0(t)$ et de rayon $r$ soit contenue dans $H$; si $f(t, x, \xi_0)$ est lipschitzienne pour la constante $k > 0$ dans $I \times H$, prenons $\alpha$ assez petit pour que $\frac{e^{k(t_1-t_0)} - 1}{k} < r$; en prenant $V$ tel que, pour tout $\xi \in V$, on ait $\|f(t, x, \xi) - f(t, x, \xi_0)\| \leq \alpha$ dans $I \times H$, on répondra à la question en vertu de la prop. 7 de IV, p. 13; en outre, on a
$$
\|u(t, \xi) - u_0(t)\| \leq \alpha \frac{e^{k(t_1-t_0)} - 1}{k}
$$
dans $(t_0, t_1]$, ce qui achève de démontrer le théorème.

#### Remarque {#fvr-iv-s1-n6-rem-1 .statement}

Lorsque $H = E$ et que la condition (16) de IV, p. 13, est vérifiée dans $I \times E$, la prop. 7 de IV, p. 13, s’applique à toute solution $u$ de $x' = g(t, x)$, dans un intervalle quelconque où cette solution est définie; on peut même supposer que $g(t, x)$ est lipschitzienne pour une fonction $k(t)$ réglée dans $K$, mais non nécessairement bornée dans cet intervalle.

### 7. Dépendance des conditions initiales

Soit $x' = f(t, x)$ une équation localement lipschitzienne dans $I \times H$; d’après le th. 2 (IV, p. 11), pour tout point $(t_0, x_0)$ de $I \times H$, il existe un plus grand intervalle $J(t_0, x_0) \subset I$, non réduit à un point, contenant $t_0$, et dans lequel il existe une intégrale (et une seule) de l’équation, égale à $x_0$ au point $t_0$; nous allons préciser la manière dont cette intégrale, et l’intervalle $J(t_0, x_0)$ où elle est définie, dépendent du point $(t_0, x_0)$.

#### Théorème 4 {#fvr-iv-s1-thm-4 .statement}

Soient $f$ une fonction localement lipschitzienne dans $I \times H$, $(a, b)$ un point quelconque de $I \times H$.

1° Il existe un intervalle $K \subset I$, voisinage de $a$ dans $I$, et un voisinage $V$ de $b$ dans $H$ tels que, pour tout point $(t_0, x_0)$ de $K \times V$, il existe une intégrale et une seule $u(t, t_0, x_0)$ définie dans $K$, à valeurs dans $H$ et égale à $x_0$ au point $t_0$ (autrement dit, on a $J(t_0, x_0) \supseteq K$ quel que soit $(t_0, x_0) \in K \times V$).

2° L’application $(t, t_0, x_0) \mapsto u(t, t_0, x_0)$ de $K \times K \times V$ dans $H$ est uniformément continue.

3° Il existe un voisinage $W \subset V$ de $b$ dans $H$ tel que, pour tout point
$$
(t, t_0, x_0) \in K \times K \times W,
$$
l’équation $x_0 = u(t_0, t, x)$ ait dans $V$ une solution unique $x$ égale à $u(t, t_0, x_0)$ (« résolution de l’intégrale par rapport à la constante d’intégration »).

1° Soient $S$ une boule de centre $b$ et de rayon $r$ contenue dans $H$, $J_0$ un intervalle contenu dans $I$ et voisinage de $a$ dans $I$, tels que $f$ soit bornée et lipschitzienne (pour une certaine constante $k$) dans $J_0 \times S$; nous désignerons par $M$ la borne supérieure de $\|f(t, x)\|$ dans $J_0 \times S$. Il existe alors (IV, p. 10, th. 1) un intervalle $J \subset J_0$, voisinage de $a$ dans $I$, et une intégrale $v$ de $x' = f(t, x)$ définie dans $J$, à valeurs dans $S$ et égale à $b$ au point $a$. Nous allons voir que la boule ouverte $V$ de centre $b$ et de rayon $r/2$, et l’intersection $K$ de $J$ et d’un intervalle $]a - l, a + l[$, où $l$ est assez petit, répondent à la question. En effet, la prop. 7 de IV, p. 13 (appliquée à l’ensemble $J_0 \times S$ et au cas où $\alpha = 0$) montre qu’il existe une intégrale de $x' = f(t, x)$ définie dans $K$, à valeurs dans $S$, et égale à $x_0$ en un point $t_0 \in K$, pourvu que l’on ait
$$
\|v(t) - b\| + \|v(t_0) - x_0\| e^{k|t - t_0|} < r
$$
pour tout $t \in K$. Or, d’après le th. des accroissements finis, on a
$$
\|v(t) - b\| \leq M|t - a| \leq Ml
$$
pour tout $t \in K$; comme $\|x_0 - b\| < r/2$, on voit qu’il suffit de prendre $l$ tel que
$$
Ml + (Ml + r/2) e^{2kl} < r
$$
pour que la relation (18) soit vérifiée pour tout point $(t, t_0, x_0)$ de $K \times K \times V$.

2° D’après le th. des accroissements finis, on a
$$
\|u(t_1, t_0, x_0) - u(t_2, t_0, x_0)\| \leq M|t_2 - t_1|
$$
quels que soient $t_0, t_1, t_2$ dans $K$ et $x_0$ dans $V$. La prop. 5 (IV, p. 7) montre que
$$
\|u(t, t_0, x_1) - u(t, t_0, x_2)\| \leq e^{2kl} \|x_2 - x_1\|
$$
quels que soient $t$ et $t_0$ dans $K$, $x_1$ et $x_2$ dans $V$. Enfin, si $t_1$ et $t_2$ sont deux points quelconques de $K$, on a
$$
\|u(t_1, t_2, x_0) - u(t_2, t_2, x_0)\| \leq M|t_2 - t_1|
$$

d’après le th. des accroissements finis, c’est-à-dire
$$
\|u(t_1, t_2, x_0) - x_0\| \leq M|t_2 - t_1|;
$$
comme $u(t, t_2, x_0)$ est identique à l’intégrale qui, au point $t_1$, prend la valeur $u(t_1, t_2, x_0)$, la prop. 5 (IV, p. 7) montre que l’on a
(22)
$$
\|u(t, t_1, x_0) - u(t, t_2, x_0)\| \leq M e^{2kl}|t_2 - t_1|
$$
quels que soient $t, t_1, t_2$ dans K et $x_0$ dans V. Les trois inégalités (20), (21) et (22) démontrent donc la continuité uniforme de l’application $(t, t_0, x_0) \mapsto u(t, t_0, x_0)$ dans $K \times K \times V$.

3° D’après (20), on a $\|u(t, t_0, x_0) - x_0\| \leq M|t - t_0| \leq 2Ml$ dans
$$
K \times K \times V.
$$
Si $l$ a été pris assez petit pour que $2Ml < r/4$, on voit donc que si $x_0$ est un point quelconque de la boule ouverte W de centre b et de rayon $r/4$, on a $u(t, t_0, x_0) \in V$ quels que soient $t$ et $t_0$ dans K. Si $x = u(t, t_0, x_0)$, la fonction $s \mapsto u(s, t, x)$ est donc définie dans K et égale à l’intégrale de (1) qui prend la valeur $x$ au point $t$, c’est-à-dire à $u(s, t_0, x_0)$; en particulier
$$
x_0 = u(t_0, t_0, x_0) = u(t_0, t, x).
$$
D’ailleurs, si $y \in V$ est tel que $x_0 = u(t_0, t, y)$, l’intégrale $s \mapsto u(s, t, y)$ prend la valeur $x_0$ au point $t_0$, donc est identique à $s \mapsto u(s, t_0, x_0)$, et par suite prend la valeur $x$ au point $t$, ce qui montre que $y = x$ et achève la démonstration.

## EXERCICES {#fvr-iv-s1-exercises}

Exercices

§ I

See the [exercises for § 1](exercises/s1/).
