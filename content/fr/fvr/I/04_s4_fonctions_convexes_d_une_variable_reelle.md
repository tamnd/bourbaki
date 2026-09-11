---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DÉRIVÉES
section: 4
section_title: Fonctions convexes d'une variable réelle
lang: fr
source: fvr-i-vii-fr
book_pages: FVR I.51-FVR I.54
pdf_pages: 0030-0040, 0049-0052
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fonctions convexes
      page: 32
      pdf_page: 30
    - "no": 2
      title: Familles de fonctions convexes
      page: 35
      pdf_page: 33
    - "no": 3
      title: Continuité et dérivabilité des fonctions convexes
      page: 36
      pdf_page: 34
    - "no": 4
      title: Critères de convexité
      page: 38
      pdf_page: 36
statements: 23
exercises: 25
content_sha256: 75259f901626bf63f4807a794433c6bf4a7b1dabbf9d8c9eec785a348d52570e
---

## § 4. FONCTIONS CONVEXES D’UNE VARIABLE RÉELLE

Soient H une partie de $\mathbf{R}$, $f$ une fonction numérique finie définie dans H, G le graphe ou ensemble représentatif de la fonction $f$ dans $\mathbf{R} \times \mathbf{R} = \mathbf{R}^2$, ensemble des points $M_x = (x, f(x))$, où $x$ parcourt H. Nous conviendrons de dire qu’un point $(a, b)$ de $\mathbf{R}^2$ tel que $a \in H$ est au-dessus (resp. strictement au-dessus, au-dessous, strictement au-dessous) de G si on a $b \geq f(a)$ (resp. $b > f(a)$, $b < f(a)$, $b < f(a)$). Si $A = (a, a')$ et $B = (b, b')$ sont deux points de $\mathbf{R}^2$, nous désignerons par AB le segment fermé d’extrémités A et B; si $a < b$, AB est le graphe de la fonction linéaire $a' + \frac{b' - a'}{b - a} (x - a)$ définie dans $(a, b)$; nous désignerons par $p(AB)$ la pente $\frac{b' - a'}{b - a}$ de ce segment, et ferons usage du lemme suivant, dont la vérification est immédiate:

#### Lemme {#fvr-i-s4-n0-lem-1 .statement}

Soient $A = (a, a')$, $B = (b, b')$, $C = (c, c')$ trois points de $\mathbf{R}^2$ tels que $a < b < c$. Les propositions suivantes sont équivalentes:
a) B est au-dessous de AC;
b) C est au-dessus de la droite passant par A et B;

![Figure 1](fig1.png)

Fig. 1

c) A est au-dessus de la droite passant par B et C;
d) $p(AB) \leq p(AC)$;
e) $p(AC) \leq p(BC)$.

Le lemme est encore exact quand on y remplace « au-dessus » (resp. « au-dessous ») par « strictement au-dessus » (resp. « strictement au-dessous ») et le signe $\leq$ par $<$ (fig. 1).

### 1. Définition des fonctions convexes

#### Définition 1 {#fvr-i-s4-def-1 .statement}

On dit qu’une fonction numérique finie $f$, définie dans un intervalle $(I \subset \mathbf{R})$, est convexe dans I, si, quels que soient les points $x, x'$ de I ($x < x'$), tout point $M_x$ du graphe G de f tel que $x \leq z \leq x'$ est au-dessous du segment $M_xM_{x'}$ (ou, ce qui revient au même, si tout point de ce segment est au-dessus de G) (fig. 2).

![Graph showing points M_x, M_z, M_{x'}, and segment G between M_x and M_{x'}](https://i.imgur.com/3Q5z5QG.png)

Fig. 2

Tenant compte de la représentation paramétrique d’un segment (TG, VI, p. 5), la condition pour que f soit convexe dans I est que l’on ait l’inégalité
$$
f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')
$$
pour tout couple $(x, x')$ de points de I et tout $\lambda \in [0, 1]$.

La définition 1 est encore équivalente à la suivante : *l’ensemble des points de $\mathbf{R}^2$ situés au-dessus du graphe G de f est convexe*. En effet, cette condition est évidemment suffisante pour que f soit convexe dans I ; elle est aussi nécessaire, car si f est convexe dans I, et si $(x, y), (x', y')$ sont deux points situés au-dessus de G, on a $y \geq f(x), y' \geq f(x')$, d’où, pour $0 \leq \lambda \leq 1$,
$$
\lambda y + (1 - \lambda)y' \geq \lambda f(x) + (1 - \lambda)f(x') \geq f(\lambda x + (1 - \lambda)x')
$$
d’après (1), ce qui montre que tout point du segment d’extrémités $(x, y)$ et $(x', y')$ est au-dessus de G.

#### Remarque {#fvr-i-s4-n1-rem-1 .statement}

On voit de même que l’ensemble des points situés *strictement au-dessus* de G est convexe. Réciproquement, si cet ensemble est convexe, on a
$$
\lambda y + (1 - \lambda)y' > f(\lambda x + (1 - \lambda)x')
$$
pour $0 \leq \lambda \leq 1$ et $y > f(x), y' > f(x')$ ; en faisant tendre y vers $f(x)$ et $y'$ vers $f(x')$ dans cette formule, il en résulte que f est convexe.

#### Exemple 1 {#fvr-i-s4-n1-exa-1 .statement}

Toute fonction linéaire affine (numérique) $ax + b$ est convexe dans $\mathbf{R}$.

#### Exemple 2 {#fvr-i-s4-n1-exa-2 .statement}

La fonction $x^2$ est convexe dans $\mathbf{R}$, car on a
$$
\lambda x^2 + (1 - \lambda){x'}^2 - (\lambda x + (1 - \lambda)x')^2 = \lambda(1 - \lambda)(x - x')^2 \geq 0
$$
pour $0 \leq \lambda \leq 1$.

#### Exemple 3 {#fvr-i-s4-n1-exa-3 .statement}

La fonction $|x|$ est convexe dans $\mathbf{R}$, car on a
$$
|\lambda x + (1 - \lambda)x'| \leq \lambda |x| + (1 - \lambda)|x'|
$$
pour $0 \leq \lambda \leq 1$.

Il est clair que si f est convexe dans I, sa restriction à tout intervalle $J \subset I$ est convexe dans J.

Soient $f$ une fonction convexe dans $I$, $x, x'$ deux points de $I$ tels que $x < x'$; si $z \in I$ est extérieur à $\{x, x'\}$, $M_z$ est au-dessus de la droite D joignant $M_x$ et $M_{x'}$; c’est une conséquence immédiate du lemme.

On en déduit que, si $z$ est un point tel que $x < z < x'$, et tel que $M_z$ soit sur le segment $M_xM_{x'}$, alors, pour tout autre point $z'$ tel que $x < z' < x'$, $M_{z'}$ est aussi sur le segment $M_xM_{x'}$, car il résulte de ce qui précède que $M_{z'}$ doit être à la fois au-dessus et au-dessous de ce segment; en d’autres termes, $f$ est alors égale à une fonction linéaire affine dans $\{x, x'\}$.

#### Définition 2 {#fvr-i-s4-def-2 .statement}

On dit qu’une fonction numérique finie $f$, définie dans un intervalle $I \subset \mathbf{R}$, est strictement convexe dans $I$, si quels que soient les points $x, x'$ de $I$ ($x < x'$), tout point $M_z$ du graphe G de $f$ tel que $x < z < x'$ est strictement au-dessous du segment $M_xM_{x'}$ (ou, ce qui revient au même, si tout point de ce segment, distinct des extrémités, est strictement au-dessus de G).

En d’autres termes, on doit avoir l’inégalité
$$
f(\lambda x + (1 - \lambda)x') < \lambda f(x) + (1 - \lambda)f(x')
$$
pour tout couple $(x, x')$ de points distincts de $I$ et tout $\lambda$ tel que $0 < \lambda < 1$.

Les remarques précédant la déf. 2 montrent que, pour qu’une fonction $f$ convexe dans $I$ soit strictement convexe, il faut et il suffit qu’il n’existe aucun intervalle contenu dans $I$ (et non réduit à un point) tel que la restriction de $f$ à cet intervalle soit linéaire affine.

Des exemples donnés ci-dessus, le premier et le troisième ne sont pas des fonctions strictement convexes; par contre, on voit que $x^2$ est une fonction strictement convexe dans $\mathbf{R}$; un calcul analogue montre que $1/x$ est strictement convexe dans $]0, +\infty[$.

#### Proposition 1 {#fvr-i-s4-prop-1 .statement}

Soit $f$ une fonction numérique finie, convexe (resp. strictement convexe) dans un intervalle $I \subset \mathbf{R}$. Pour toute famille $(x_i)_{1 \leq i \leq p}$ de $p \geq 2$ points distincts de $I$, et toute famille $(\lambda_i)_{1 \leq i \leq p}$ de $p$ nombres réels tels que $0 < \lambda_i < 1$ et $\sum_{i=1}^p \lambda_i = 1$, on a
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i)
$$
(resp.
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i)).
$$

La proposition (pour les fonctions convexes) se réduisant à l’inégalité (1) pour $p = 2$, nous raisonnons par récurrence sur $p > 2$. Le nombre $\mu = \sum_{i=1}^{n-1} \lambda_i$ est $> 0$; il est immédiat que si $a$ et $b$ sont le plus petit et le plus grand des $x_i$, on a
$$
a \leq \frac{\sum_{i=1}^{p-1} \lambda_i x_i}{\sum_{i=1}^{p-1} \lambda_i} \leq b,
$$
autrement dit le point $x = \frac{1}{\mu} \sum_{i=1}^{p-1} \lambda_i x_i$ appartient à $I$, et l’hypothèse de récurrence entraîne $\mu f(x) \leq \sum_{i=1}^{p-1} \lambda_i f(x_i)$; d’autre part, on a, d’après (1)

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) = f(\mu x + (1-\mu)x_p) \leq \mu f(x) + (1-\mu)f(x_p) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

On raisonne de même pour les fonctions strictement convexes en partant de l’inégalité (2).

On dit qu’une fonction numérique finie $f$ est *concave* (resp. *strictement concave*) dans $I$ si — $f$ est convexe (resp. strictement convexe) dans $I$. Il revient au même de dire que, pour tout couple $(x, x')$ de points distincts de $I$ et tout $\lambda$ tel que $0 < \lambda < 1$, on a

$$
f(\lambda x + (1-\lambda)x') \geq \lambda f(x) + (1-\lambda)f(x')
$$
(resp. $f(\lambda x + (1-\lambda)x') > \lambda f(x) + (1-\lambda)f(x')$).

### 2. Familles de fonctions convexes

#### Proposition 2 {#fvr-i-s4-prop-2 .statement}

Soient $f_i$ ($1 \leq i \leq p$) $p$ fonctions convexes dans un intervalle $I \subset \mathbf{R}$, et $c_i$ ($1 \leq i \leq p$) $p$ nombres positifs quelconques ; la fonction $f = \sum_{i=1}^p c_i f_i$ est convexe dans $I$.
En outre, si pour un indice $j$ au moins, $f_j$ est strictement convexe dans $I$ et $c_j > 0$, $f$ est strictement convexe dans $I$.

Cela résulte aussitôt de l’inégalité (1) (resp. (2)) appliquée à chacune des $f_i$, en multipliant les deux membres de l’inégalité relative à $f_i$ par $c_i$, et ajoutant membre à membre.

#### Proposition 3 {#fvr-i-s4-prop-3 .statement}

Soit $(f_\alpha)$ une famille de fonctions convexes dans un intervalle $I \subset \mathbf{R}$; si l’enveloppe supérieure $g$ de cette famille est finie en tout point de $I$, $g$ est convexe dans $I$.

En effet, l’ensemble des points $(x, y) \in \mathbf{R}^2$ situés au-dessus du graphe de $g$ est l’intersection des ensembles convexes formés respectivement des points situés au-dessus du graphe de chacune des fonctions $f_\alpha$; il est donc convexe.

#### Proposition 4 {#fvr-i-s4-prop-4 .statement}

Soit $H$ un ensemble de fonctions convexes dans un intervalle $I \subset \mathbf{R}$; si $\mathfrak{F}$ est un filtre sur $H$ qui converge simplement dans $I$ vers une fonction numérique finie $f_0$, cette fonction est convexe dans $I$.

Il suffit pour le voir de passer à la limite suivant $\mathfrak{F}$ dans l’inégalité (1).

### 3. Continuité et dérivabilité des fonctions convexes

#### Proposition 5 {#fvr-i-s4-prop-5 .statement}

Pour qu’une fonction numérique finie f soit convexe (resp. strictement convexe) dans un intervalle I, il faut et il suffit que pour tout a ∈ I, la pente

$$
p(M_aM_x) = \frac{f(x) - f(a)}{x - a}
$$

soit une fonction croissante (resp. strictement croissante) de x dans I ∩ C{a}.

Cette proposition est une conséquence immédiate des déf. 1 et 2 et du lemme de I, p. 32.

#### Proposition 6 {#fvr-i-s4-prop-6 .statement}

Soit f une fonction numérique finie, convexe dans un intervalle I ⊂ ℝ. En tout point a intérieur à I, f est continue, admet une dérivée à droite et une dérivée à gauche finies, et on a $f'_g(a) \leq f'_d(a)$.

En effet, pour x ∈ I et x > a, la fonction $x \mapsto \frac{f(x) - f(a)}{x - a}$ est croissante (prop. 5) et bornée inférieurement, puisque si y < a et y ∈ I, on a

$$
\frac{f(y) - f(a)}{y - a} \leq \frac{f(x) - f(a)}{x - a}
$$

d’après la prop. 5; cette fonction admet donc une limite à droite finie au point a, autrement dit $f'_d(a)$ existe et est finie; en outre, en faisant tendre x vers a (x > a) dans (5), il vient

$$
\frac{f(y) - f(a)}{y - a} \leq f'_d(a)
$$

pour tout y < a appartenant à I. On démontre de même que $f'_g(a)$ existe, et que

$$
f'_g(a) \leq \frac{f(x) - f(a)}{x - a}
$$

pour x ∈ I et x > a. En faisant tendre x vers a (x > a) dans cette dernière inégalité, il vient $f'_g(a) \leq f'_d(a)$. L’existence des dérivées à droite et à gauche au point a entraîne évidemment la continuité de f en ce point.

#### Corollaire 1 {#fvr-i-s4-prop-6-cor-1 .statement}

Soit f une fonction convexe (resp. strictement convexe) dans I; si a et b sont deux points intérieurs à I tels que a < b, on a (fig. 3)

$$
f'_d(a) \leq \frac{f(b) - f(a)}{b - a} \leq f'_g(b)
$$

(resp.

$$
f'_d(a) < \frac{f(b) - f(a)}{b - a} < f'_g(b).
$$

La double inégalité (8) provient de (6) et (7) par simple changement de notation. D’autre part, si $f$ est strictement convexe et $c$ tel que $a < c < b$, on a, d’après (8) et la prop. 5
$$
f'_a(a) \leq \frac{f(c) - f(a)}{c - a} < \frac{f(b) - f(a)}{b - a} < \frac{f(b) - f(c)}{b - c} \leq f'_g(b)
$$
d’où (9).

#### Corollaire 2 {#fvr-i-s4-prop-6-cor-2 .statement}

*Si $f$ est convexe (resp. strictement convexe) dans $I$, $f'_a$ et $f'_g$ sont croissantes (resp. strictement croissantes) dans l’intérieur de $I$; l’ensemble des points de $I$ où $f$ n’est pas dérivable est dénombrable, et $f'_a$ et $f'_g$ sont continues en tout point où $f$ est dérivable.*

La première partie résulte aussitôt de (8) (resp. (9)) et de l’inégalité
$$
f'_g(a) \leq f'_a(a).
$$
Soient d’autre part $E$ l’ensemble des points $x$ intérieurs à $I$ où $f$ n’est pas dérivable (c’est-à-dire $f'_g(x) < f'_a(x)$). Pour tout $x \in E$, soit $J_x$ l’intervalle ouvert $]f'_g(x), f'_a(x)[$; il résulte de (8) que si $x$ et $y$ sont deux points de $E$ tels que $x < y$, on a $u < v$ pour tout $u \in J_x$ et tout $v \in J_y$; autrement dit, lorsque $x$ parcourt $E$, les intervalles ouverts non vides $J_x$ sont deux à deux sans point commun; l’ensemble de ces intervalles est donc dénombrable, et il en est par suite de même de $E$. Enfin, $f'_a$ (resp. $f'_g$) étant croissante, a en tout point $x$ intérieur à $I$ une limite à droite et une limite à gauche; la prop. 6 de I, p. 26 montre alors que la limite à droite de $f'_a$ (resp. $f'_g$) au point $x$ est égale à $f'_a(x)$, et sa limite à gauche à $f'_g(x)$; d’où la dernière partie du corollaire.

Soient $f$ une fonction convexe dans $I$, $a$ un point intérieur à $I$, $D$ une droite passant par le point $M_a$, d’équation $y - f(a) = \alpha(x - a)$. Il résulte des inégalités (8) que si $f'_g(a) \leq \alpha \leq f'_a(a)$, tout point du graphe $G$ de $f$ est *au-dessus* de $D$, et, si $f$ est strictement convexe, $M_a$ est le seul point commun à $D$ et $G$; on dit que $D$ est une *droite d’appui* de $G$ au point $M_a$. Inversement, si $G$ est au-dessus de $D$, on a $f(x) - f(a) \geq \alpha(x - a)$ pour tout $x \in I$, d’où $\frac{f(x) - f(a)}{x - a} \geq \alpha$ pour $x \geq a$, et $\frac{f(x) - f(a)}{x - a} \leq \alpha$ pour $x < a$; faisant tendre $x$ vers $a$ dans ces inégalités, il vient $f'_g(a) \leq \alpha \leq f'_a(a)$.

En particulier, si $f$ est dérivable au point $a$, il n’existe qu’une seule droite d’appui de $G$ au point $M_a$, la tangente à $G$ en $M_a$.

#### Remarque {#fvr-i-s4-n3-rem-1 .statement}

Si $f$ est une fonction strictement convexe dans un intervalle ouvert $I$, $f'_a$ est strictement croissante dans $I$, donc trois cas seulement sont possibles, d’après la prop. 2 de I, p. 21:
  1° $f$ est strictement décroissante dans $I$;
  2° $f$ est strictement croissante dans $I$;
  3° il existe $a \in I$ tel que, pour $x \leq a$, $f$ soit strictement décroissante, et, pour $x \geq a$, strictement croissante.

Lorsque $f$ est convexe dans $I$, mais non strictement convexe, $f$ peut être constante dans un intervalle contenu dans $I$; soit $J = ]a, b[$ le plus grand intervalle ouvert où $f$ est constante (c’est-à-dire l’intérieur de l’intervalle où $f'_a(x) = 0$); $f$ est alors strictement décroissante dans l’intervalle formé des points $x \in I$ tels que $x \leq a$ (s’il en existe), strictement croissante dans l’intervalle formé des points $x \in I$ tels que $x \geq b$ (s’il en existe).

Dans tous les cas, on voit que $f$ possède une limite à droite à l’origine de $I$ (dans $\overline{\mathbf{R}}$), une limite à gauche à l’extrémité de $I$; ces limites peuvent être finies ou infinies (cf. I, p. 51, exerc. 5, 6 et 7). Par abus de langage, on dit parfois que la fonction continue (à valeurs dans $\overline{\mathbf{R}}$) égale à $f$ dans l’intérieur de $I$, et prolongée par continuité aux extrémités de $I$, est convexe dans $\tilde{I}$.

### 4. Critères de convexité

#### Proposition 7 {#fvr-i-s4-prop-7 .statement}

Soit $f$ une fonction numérique finie, définie dans un intervalle $I \subset \mathbf{R}$. Pour que $f$ soit convexe dans $I$, il faut et il suffit que, pour tout couple de nombres $a, b$ de $I$ tels que $a < b$, et pour tout nombre réel $\mu$, la fonction $f(x) + \mu x$ atteigne sa borne supérieure dans $[a, b]$ en l’un des points $a, b$.

La condition est nécessaire; en effet, comme $\mu x$ est convexe dans $\mathbf{R}$, $f(x) + \mu x$ est convexe dans $I$; on peut donc se borner au cas où $\mu = 0$. Or, pour
$$
x = \lambda a + (1 - \lambda)b \quad (0 \leq \lambda \leq 1),
$$
on a
$$
f(x) \leq \lambda f(a) + (1 - \lambda)f(b) \leq \operatorname{Max}(f(a), f(b)).
$$

La condition est suffisante. Prenons en effet $\mu = - \frac{f(b) - f(a)}{b - a}$ et soit $g(x) = f(x) + \mu x$; on a $g(a) = g(b)$, donc $g(x) \leq g(a)$ pour tout $x \in [a, b]$, et on vérifie aussitôt que cette inégalité équivaut à l’inégalité (1) où on a remplacé $z$ par $a$ et $x'$ par $b$.

#### Proposition 8 {#fvr-i-s4-prop-8 .statement}

Pour qu’une fonction numérique finie $f$ soit convexe (resp. strictement convexe) dans un intervalle ouvert $I \subset \mathbf{R}$, il faut et il suffit qu’elle soit continue dans $I$, admette une dérivée en tout point du complémentaire $B$ par rapport à $I$ d’une partie dénombrable de cet intervalle, et que cette dérivée soit croissante (resp. strictement croissante) dans $B$.

La condition est nécessaire d’après la prop. 6 et son corollaire 2 (I, p. 36); montrons qu’elle est suffisante. Supposons donc $f'$ croissante dans $B$, et supposons que $f$ ne soit pas convexe; il existerait donc (I, p. 36, prop. 5) trois points $a, b, c$ de

I tels que $a < c < b$, et $\frac{f(c) - f(a)}{c - a} > \frac{f(b) - f(c)}{b - c}$; mais d’après le th. des accroissements finis (I, p. 23, th. 1), on a
$$
\frac{f(c) - f(a)}{c - a} \leq \sup_{x \in B, a < x < c} f'(x) \quad \text{et} \quad \frac{f(b) - f(c)}{b - c} \geq \inf_{x \in B, c < x < b} f'(x).
$$
On aurait donc $\sup_{x \in B, a < x < c} f'(x) > \inf_{x \in B, c < x < b} f'(x)$, contrairement à l’hypothèse que $f'$ est croissante dans $B$.

Si maintenant $f'$ est supposée strictement croissante dans $B$, $f$ est convexe et ne peut être égale à une fonction linéaire affine dans aucun intervalle ouvert contenu dans $I$, car dans cet intervalle $f'$ serait constante, contrairement à l’hypothèse.

#### Corollaire {#fvr-i-s4-n4-cor-1 .statement}

Soit $f$ une fonction numérique finie, continue et deux fois dérivable dans un intervalle $I \subset \mathbf{R}$; pour que $f$ soit convexe dans $I$, il faut et il suffit que $f''(x) \geq 0$ pour tout $x \in I$; pour que $f$ soit strictement convexe dans $I$, il faut et il suffit que la condition précédente soit vérifiée et en outre que l’ensemble des points $x \in I$ où $f''(x) > 0$ soit partout dense dans $I$.

Cela résulte aussitôt de la proposition précédente, et du corollaire de I, p. 22.

#### Exemple {#fvr-i-s4-n4-exa-1 .statement}

\* Dans l’intervalle ]0, +∞[, la fonction $x^r$ (r réel quelconque) a une dérivée seconde égale à $r(r-1)x^{r-2}$; donc, elle est strictement convexe si $r > 1$ ou $r < 0$, strictement concave si $0 < r < 1$*.

Pour énoncer un autre critère de convexité, nous poserons la définition suivante: étant donné le graphe $H$ d’une fonction numérique finie définie dans un intervalle $I \subset \mathbf{R}$, et un point $a$ intérieur à $I$, nous dirons qu’une droite $D$ passant par $M_a = (a, f(a))$ est localement au-dessus (resp. localement au-dessous) de $G$ en ce point s’il existe un voisinage $V \subset I$ de $a$ tel que tout point de $D$ contenu dans $V \times \mathbf{R}$ soit au-dessus (resp. au-dessous) de $G$; nous dirons que $D$ est localement sur $G$ au point $M_a$ s’il existe un voisinage $V \subset I$ de $a$ tel que l’intersection de $D$ et de $V \times \mathbf{R}$ soit identique à celle de $G$ et de $B \times \mathbf{R}$ (autrement dit, si $D$ est à la fois localement au-dessus et localement au-dessous de $G$).

#### Proposition 9 {#fvr-i-s4-prop-9 .statement}

Soit $f$ une fonction numérique finie, semi-continue supérieurement dans un intervalle ouvert $I \subset \mathbf{R}$. Pour que $f$ soit convexe dans $I$, il faut et il suffit que, pour tout point $M_x$ du graphe $G$ de $f$, toute droite localement au-dessus de $G$ en ce point soit localement sur $G$ (au point $M_x$).

La condition est nécessaire; en effet, si $f$ est convexe dans $I$, en tout point $M_a$ du graphe $G$ de $f$, il existe une droite d’appui $\Delta$ de $G$; $\Delta$ est au-dessous de $G$, et $a$ fortiori localement au-dessous de $G$ (I, p. 37); si une droite $D$ est localement au dessus de $G$ au point $M_a$, elle est localement au-dessus de $\Delta$, donc coïncide nécessairement avec $\Delta$, et par suite est localement sur $G$ au point $M_a$.

La condition est suffisante. En effet, supposons-la remplie, et supposons que $f$ ne soit pas convexe dans I ; il existerait alors deux points a, b de I (a < b) tels qu’il existe des points M_x de G strictement au-dessus du segment M_aM_b (fig. 4).

Autrement dit, la fonction g(x) = f(x) − f(a) − $\frac{f(b) - f(a)}{b - a}$ (x − a) prendrait des valeurs > 0 dans {a, b}; comme elle est finie et semi-continue supérieurement dans cet intervalle compact, sa borne supérieure k dans {a, b} est finie et > 0, et

![Figure 4](https://i.imgur.com/4z5z5z5.png)

Fig. 4

l’ensemble $^{-1}g(k)$ est fermé et non vide (TG, IV, p. 30, th. 3 et p. 29, prop. 1). Soit c la borne inférieure de $^{-1}g(k)$; on a a < c < b, et au point M_c la droite D d’équation y = f(c) + $\frac{f(b) - f(a)}{b - a}$ (x − c) est localement au-dessus de G; mais elle ne peut être localement sur G en ce point, puisque, pour a < x < c, on a g(x) < k, ce qui signifie que M_x est strictement au-dessous de D. Nous aboutissons donc à une contradiction, ce qui établit la proposition.

#### Corollaire 1 {#fvr-i-s4-prop-9-cor-1 .statement}

Pour qu’une fonction numérique finie f, définie dans un intervalle ouvert I ⊂ \mathbf{R}, et semi-continue supérieurement dans I, soit convexe dans I, il faut et il suffit que, pour tout x ∈ I, il existe ε > 0 tel que la relation |h| ≤ ε entraîne
$$
f(x) \leq \frac{1}{2} (f(x + h) + f(x - h)).
$$

![Figure 5](https://i.imgur.com/4z5z5z5.png)

Fig. 5

Nous avons seulement à démontrer que la condition est suffisante. En effet, si en un point $M_a$ du graphe $G$ de $f$, une droite $D$ est localement au-dessus de $G$, elle est localement sur $G$ en ce point; car, dans le cas contraire, par exemple, un point $M_{a+h}$ serait strictement au-dessous de $D$, le point $M_{a-h}$ étant au-dessous de $D$; le milieu du segment $M_{a-h}M_{a+h}$ serait alors strictement au-dessous de $D$ (fig. 5), et en vertu de l’hypothèse $M_a$ serait a fortiori strictement au-dessous de $D$, ce qui est absurde.

#### Corollaire 2 {#fvr-i-s4-prop-9-cor-2 .statement}

Soit $f$ une fonction numérique finie, définie dans un intervalle ouvert $I \subset \mathbf{R}$. Si, pour tout point $x \in I$, il existe un intervalle ouvert $J_x \subset I$ contenant $x$ et tel que la restriction de $f$ à $J_x$ soit convexe dans $J_x$, alors $f$ est convexe dans $I$.

Il est clair en effet que $f$ satisfait au critère de la prop. 8.

Exercices

## EXERCICES {#fvr-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
