---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES ET INTÉGRALES
section: 1
section_title: Primitives et intégrales
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0053-0065, 0081-0085
extraction: ocr
subsections:
    - "no": 1
      title: Définition des primitives
      page: 0
      pdf_page: 53
    - "no": 2
      title: Existence des primitives
      page: 2
      pdf_page: 54
    - "no": 3
      title: Fonctions réglées
      page: 4
      pdf_page: 56
    - "no": 4
      title: Intégrales
      page: 7
      pdf_page: 59
    - "no": 5
      title: Propriétés des intégrales
      page: 9
      pdf_page: 61
    - "no": 6
      title: Forme intégrale du reste de la formule de Taylor; primitives d’ordre supérieur
      page: 12
      pdf_page: 64
statements: 22
exercises: 23
content_sha256: 5a27641b592dcf22dbdae6a37b4e3830b667c63fcc0afddc3d65bffc2a43fdb8
---

## § 1. PRIMITIVES ET INTÉGRALES

Sauf mention expresse du contraire, nous ne considérerons, dans ce chapitre, que des fonctions vectorielles d’une variable réelle, prenant leurs valeurs dans un espace normé complet sur $\mathbf{R}$. Lorsqu’il s’agit en particulier de fonctions numériques, il est donc toujours sous-entendu que ces fonctions sont finies si le contraire n’est pas spécifié.

### 1. Définition des primitives

Une fonction vectorielle $\mathbf{f}$, définie dans un intervalle $I \subset \mathbf{R}$, ne peut être en tout point de cet intervalle la dérivée d’une fonction vectorielle $\mathbf{g}$ (définie et continue dans $I$) que si elle satisfait à des conditions assez restrictives: par exemple, si $\mathbf{f}$ admet une limite à droite et une limite à gauche en un point $x_0$ intérieur à $I$, $\mathbf{f}$ doit être continue au point $x_0$, d’après la prop. 6 de I, p. 26; il en résulte que, si on prend pour $I$ l’intervalle $(-1, +1)$, pour $f$ la fonction numérique égale à $-1$ dans $(-1, 0[$, à $+1$ dans $]0, 1]$, $f$ n’est pas la dérivée d’une fonction continue dans $I$; toutefois, la fonction $|x|$ a pour dérivée $f(x)$ en tout point $\neq 0$; on est ainsi conduit à poser la définition suivante:

#### Définition 1 {#fvr-ii-s1-def-1 .statement}

Etant donnée une fonction vectorielle $\mathbf{f}$, définie dans un intervalle $I \subset \mathbf{R}$, on dit qu’une fonction $\mathbf{g}$ définie dans $I$ est une primitive de $\mathbf{f}$ si $\mathbf{g}$ est continue dans $I$ et admet une dérivée égale à $\mathbf{f}(x)$ en tout point $x$ du complémentaire (par rapport à $I$) d’une partie dénombrable de $I$.

Si en outre g admet en tout point x de I une dérivée égale à f(x), on dira que g est une primitive stricte de f.

Avec cette définition, on voit que la fonction numérique f considérée ci-dessus admet une primitive égale à |x|.

Il est clair que, si f admet une primitive dans I, toute primitive de f est aussi une primitive de toute fonction égale à f sauf aux points d’une partie dénombrable de I. Par abus de langage, on peut parler d’une primitive dans I d’une fonction f_0 définie seulement dans le complémentaire (par rapport à I) d’une partie dénombrable de I : il s’agira de la primitive de toute fonction f définie dans I, et égale à f_0 aux points où f_0 est définie.

#### Proposition 1 {#fvr-ii-s1-prop-1 .statement}

Soit f une fonction vectorielle définie dans I, à valeurs dans E ; si f admet une primitive g dans I, l’ensemble des primitives de f dans I est identique à l’ensemble des fonctions g + a, où a est une fonction constante, à valeurs dans E.

En effet, il est clair que g + a est une primitive de f quel que soit a ∈ E ; d’autre part, si g_1 est une primitive de f, g_1 − g admet une dérivée égale à 0 sauf aux points d’une partie dénombrable de I, donc est constante (I, p. 24, corollaire).

On dit que les primitives d’une fonction f (lorsqu’elles existent) sont définies « à une constante additive près ». Pour définir sans ambiguïté une primitive de f, il suffit de se donner (arbitrairement) sa valeur en un point x_0 ∈ I ; en particulier, il existe une primitive et une seule g de f telle que g(x_0) = 0 ; pour toute primitive h de f, on a g(x) = h(x) − h(x_0).

### 2. Existence des primitives

Soit f une fonction définie dans un intervalle quelconque I ⊂ ℝ ; pour qu’une fonction g définie dans I soit une primitive de f, il faut et il suffit que la restriction de g à tout intervalle compact J ⊂ I soit une primitive de la restriction de f à J.

#### Théorème 1 {#fvr-ii-s1-thm-1 .statement}

Soient A un ensemble filtré par un filtre 𝔞, (f_α)_{α ∈ A} une famille de fonctions vectorielles à valeurs dans un espace normé complet E sur ℝ, définies dans un intervalle I ⊂ ℝ ; pour tout α ∈ A, soit g_α une primitive de f_α. On suppose que :
1° suivant le filtre 𝔞, les fonctions f_α convergent uniformément dans tout partie compacte de I vers une fonction f ;
2° il existe un point a ∈ I tel que, suivant le filtre 𝔞, la famille (g_α(a)) a une limite dans E.

Dans ces conditions, les fonctions g_α convergent uniformément (suivant 𝔞) dans toute partie compacte de I, vers une primitive g de f.

D’après la remarque du début de ce n°, nous pouvons nous borner au cas où I est un intervalle compact.

Montrons d’abord que les $g_\alpha$ convergent uniformément dans $I$ vers une fonction continue $g$. Par hypothèse, pour tout $\varepsilon > 0$, il existe un ensemble $M \in \mathfrak{F}$ tel que, pour deux indices quelconques $\alpha, \beta$ appartenant à $M$, on ait $\| f_\alpha(x) - f_\beta(x) \| \leq \varepsilon$ pour tout $x \in I$; on a par suite (I, p. 23, th. 2)
$$
\| g_\alpha(x) - g_\beta(x) - (g_\alpha(a) - g_\beta(a)) \| \leq \varepsilon |x - a| \leq \varepsilon l
$$
en désignant par $l$ la longueur de $I$; comme par hypothèse $g_\alpha(a)$ tend vers une limite suivant $\mathfrak{F}$, il résulte du critère de Cauchy que les $g_\alpha$ convergent uniformément dans $I$. Reste à voir que la limite $g$ des $g_\alpha$ est une primitive de $f$.

Pour tout entier $n > 0$, soit $\alpha_n$ un indice tel que $\| f(x) - f_{\alpha_n}(x) \| \leq 1/n$ dans $I$; il est clair que la suite $(f_{\alpha_n})$ converge uniformément vers $f$ et que la suite $(g_{\alpha_n})$ converge uniformément vers $g$ dans $I$. Soit $H_n$ la partie dénombrable de $I$ où $f_{\alpha_n}$ n’est pas la dérivée de $g_{\alpha_n}$, et soit $H$ la réunion des $H_n$, qui est donc une partie dénombrable de $I$; nous allons voir qu’en tout point $x \in I$ n’appartenant pas à $H$, $g$ admet une dérivée égale à $f(x)$. En effet, on voit comme ci-dessus que pour tout $m \geq n$ et tout $y \in I$, on a
$$
\| g_{\alpha_m}(y) - g_{\alpha_n}(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|.
$$
En faisant croître $m$ indéfiniment, on a aussi
$$
\| g(y) - g(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|
$$
pour tout $y \in I$; or, il existe $h > 0$ tel que, pour $|y - x| \leq h$ et $y \in I$, on ait $\| g_{\alpha_n}(y) - g_{\alpha_n}(x) - f_{\alpha_n}(x) (y - x) \| \leq |y - x|/n$; comme d’autre part, on a $\| f(x) - f_{\alpha_n}(x) \| \leq 1/n$, on obtient finalement
$$
\| g(y) - g(x) - f(x) (y - x) \| \leq \frac{4}{n} |y - x|
$$
pour $y \in I$ et $|y - x| \leq h$, ce qui achève la démonstration.

#### Corollaire 1 {#fvr-ii-s1-thm-1-cor-1 .statement}

L’ensemble $\mathcal{H}$ des applications de $I$ dans $E$ qui admettent une primitive dans un intervalle $I$ est un sous-espace vectoriel fermé (donc complet) de l’espace vectoriel complet $\mathcal{F}_c(I; E)$ des applications de $I$ dans $E$, muni de la topologie de la convergence uniforme dans toute partie compacte de $I$ (TG, X, p. 4).

#### Corollaire 2 {#fvr-ii-s1-thm-1-cor-2 .statement}

Soit $x_0$ un point de $I$, et pour chaque fonction $f \in \mathcal{H}$, soit $P(f)$ la primitive de $f$ qui s’annule au point $x_0$; l’application $f \mapsto P(f)$ de $\mathcal{H}$ dans $\mathcal{F}_c(I; E)$ est une application linéaire continue.

Le cor. 1 du th. 1 permet d’établir l’existence de primitives de certaines catégories de fonctions par le procédé suivant : si on sait que les fonctions appartenant à une partie $\mathcal{A}$ de $\mathcal{F}_c(I; E)$ admettent une primitive, il en sera de même des fonctions appartenant à l’adhérence dans $\mathcal{F}_c(I; E)$ du sous-espace vectoriel engendre par $\mathscr{A}$. Nous allons appliquer cette méthode au n° suivant.

### 3. Fonctions réglées

#### Définition 2 {#fvr-ii-s1-def-2 .statement}

On dit qu’une application $f$ d’un intervalle $I \subset \mathbf{R}$ dans un ensemble $E$ est une fonction en escalier s’il existe une partition de $I$ en un nombre fini d’intervalles $J_k$ telle que $f$ soit constante dans chacun des $J_k$.

Soit $(a_i)_{0 \leq i \leq n}$ la suite strictement croissante formée des extrémités distinctes des $J_k$; comme les $J_k$ sont deux à deux sans point commun, chacun d’eux est, soit réduit à un point $a_i$, soit un intervalle ayant pour extrémités deux points consécutifs $a_i, a_{i+1}$; en outre, comme $I$ est réunion des $J_k$, $a_0$ est l’origine, et $a_n$ l’extrémité de $I$. Toute fonction en escalier dans $I$ peut donc être caractérisée comme une fonction constante dans chacun des intervalles ouverts $]a_i, a_{i+1}[$ ($0 \leq i \leq n - 1$), $(a_i)_{0 \leq i \leq n}$ étant une suite strictement croissante de points de $I$ telle que $a_0$ soit l’origine et $a_n$ l’extrémité de $I$.

#### Proposition 2 {#fvr-ii-s1-prop-2 .statement}

L’ensemble des fonctions en escalier définies dans $I$, à valeurs dans un espace vectoriel $E$ sur $\mathbf{R}$, est un sous-espace vectoriel $\mathscr{E}$ de l’espace vectoriel $\mathcal{F}(I; E)$ de toutes les applications de $I$ dans $E$.

En effet, soient $f$ et $g$ deux fonctions en escalier, $(A_i)$ et $(B_j)$ deux partitions de $I$ en un nombre fini d’intervalles telles que $f$ (resp. $g$) soit constante dans chacun des $A_i$ (resp. $B_j$); quels que soient les nombres réels $\lambda, \mu$, il est clair que $\lambda f + \mu g$ est constante dans chacun des intervalles non vides $A_i \cap B_j$, et ces intervalles forment une partition de $I$.

#### Corollaire {#fvr-ii-s1-n3-cor-1 .statement}

Le sous-espace vectoriel $\mathscr{E}$ est engendré par les fonctions caractéristiques d’intervalles.

Considérons maintenant le cas où $E$ est un espace normé sur $\mathbf{R}$; alors, il est immédiat que la fonction caractéristique d’un intervalle $J$ d’extrémités $a, b$ ($a < b$) admet une primitive, savoir la fonction égale à $a$ pour $x \leq a$, à $x$ pour $a \leq x \leq b$, et à $b$ pour $x > b$. Le cor. de la prop. 2 montre donc que toute fonction en escalier à valeurs dans $E$ admet une primitive.

Nous pouvons maintenant appliquer la méthode exposée au n° 2.

#### Définition 3 {#fvr-ii-s1-def-3 .statement}

On dit qu’une fonction vectorielle, définie dans un intervalle $I$, à valeurs dans un espace normé complet $E$ sur $\mathbf{R}$, est une fonction réglée si, dans toute partie compacte de $I$, elle est limite uniforme de fonctions en escalier.

En d’autres termes, les fonctions réglées sont les éléments de l’adhérence dans $\mathcal{F}_c(I; E)$ du sous-espace vectoriel $\mathscr{E}$, des fonctions en escalier ; $\overline{\mathscr{E}}$ est un sous-espace vectoriel de $\mathcal{F}_c(I; E)$ et comme $\mathcal{F}_c(I; E)$ est complet, il en est de même de $\mathcal{E}$; autrement dit, si une fonction est dans toute partie compacte de $I$ limite uniforme de fonctions réglées, elle est réglée dans $I$. Pour que $\mathbf{f}$ soit réglée dans un intervalle $I$, il faut et il suffit que sa restriction à tout intervalle compact contenu dans $I$ soit réglée.

Le cor. 1 de II, p. 3 montre que:

#### Théorème 2 {#fvr-ii-s1-thm-2 .statement}

*Toute fonction réglée dans un intervalle $I$ admet une primitive dans $I$.*

Nous allons transformer la déf. 3 de II, p. 4 en une autre équivalente:

#### Théorème 3 {#fvr-ii-s1-thm-3 .statement}

*Pour qu’une fonction vectorielle $\mathbf{f}$ définie dans un intervalle $I$, à valeurs dans un espace normé complet $E$ sur $\mathbf{R}$, soit réglée, il faut et il suffit qu’elle ait une limite à droite et une limite à gauche en tout point intérieur à $I$, une limite à droite à l’origine de $I$ et une limite à gauche à l’extrémité de $I$, lorsque ces points appartiennent à $I$. L’ensemble des points de discontinuité de $\mathbf{f}$ dans $I$ est alors dénombrable.*

Comme tout intervalle $I$ est réunion dénombrable d’intervalles compacts, on peut se borner à démontrer le th. 3 lorsque $I$ est *compact*, soit $I = [a, b]$.

1° La condition est *nécessaire*. Supposons en effet que $\mathbf{f}$ soit réglée, et soit $x$ un point de $I$ distinct de $b$. Par hypothèse, pour tout $\varepsilon > 0$, il existe une fonction en escalier $g$ telle que $\| \mathbf{f}(z) - g(z) \| \leq \varepsilon$ pour tout $z \in I$; comme $g$ admet une limite à droite au point $x$, il existe $y$ tel que $x < y \leq b$ et tel que, pour tout couple de points $z, z'$ de l’intervalle $]x, y]$, on ait $\| g(z) - g(z') \| \leq \varepsilon$ et par suite $\| \mathbf{f}(z) - f(z') \| \leq 3\varepsilon$; cela prouve (critère de Cauchy) que $\mathbf{f}$ a une limite à droite au point $x$. On montre de même que $\mathbf{f}$ a une limite à gauche en tout point de $I$ distinct de $a$.

2° La condition est *suffisante*. Supposons-la remplie; pour tout $x \in I$, il existe un intervalle ouvert $V_x = ]c_x, d_x[$ contenant $x$ et tel que dans l’intersection de $I$ et de chacun des intervalles ouverts $]c_x, x[$, $]x, d_x[$ (lorsque cette intersection n’est pas vide), l’oscillation de $\mathbf{f}$ soit $\leq \varepsilon$. Comme $I$ est compact, il existe un nombre fini de points $x_i$ de $I$ tels que les $V_{x_i}$ forment un recouvrement de $I$; soit $(a_k)_{0 \leq k \leq n}$ la suite obtenue en rangeant dans l’ordre croissant les points de l’ensemble fini formé de $a, b$ et des points $x_i, c_{x_i}$ et $d_{x_i}$ qui appartiennent à $I$; chacun des intervalles $]a_k, a_{k+1}[$ ($0 \leq k \leq n-1$) étant contenu dans un intervalle $]c_{x_i}, x_i[$ ou $]x_i, d_{x_i}[$, l’oscillation de $\mathbf{f}$ y est $\leq \varepsilon$; soit $c_k$ une des valeurs de $\mathbf{f}$ dans $]a_k, a_{k+1}[$; en posant $g(a_k) = \mathbf{f}(a_k)$ pour $0 \leq k \leq n$, et $g(x) = c_k$ pour tout $x \in ]a_k, a_{k+1}[$ ($0 \leq k \leq n-1$), on définit une fonction en escalier $g$ telle que $\| \mathbf{f}(z) - g(z) \| \leq \varepsilon$ dans $I$; donc $\mathbf{f}$ est réglée dans $I$.

Montrons enfin que si $\mathbf{f}$ est réglée dans $I$, l’ensemble de ses points de discontinuité est dénombrable. Pour tout $n > 0$, il existe une fonction en escalier $g_n$ telle que $\| \mathbf{f}(x) - g_n(x) \| \leq 1/n$ dans $I$; comme la suite $(g_n)$ converge uniformément vers $\mathbf{f}$ dans $I$, $\mathbf{f}$ est continue en tout point où les $g_n$ sont toutes continues

(TG, X, p. 8, cor. 1); mais comme $g_n$ est continue sauf aux points d’un ensemble fini $H_n$, $f$ est continue aux points du complémentaire de l’ensemble $H = \bigcup_n H_n$, qui est dénombrable.

#### Corollaire 1 {#fvr-ii-s1-thm-3-cor-1 .statement}

Soit $f$ une fonction réglée dans $I$; en tout point de $I$, sauf l’extrémité (resp. l’origine) de $I$, toute primitive de $f$ a une dérivée à droite égale à $f(x+)$ (resp. une dérivée à gauche égale à $f(x-)$); en particulier, en tout point $x$ où $f$ est continue, $f(x)$ est la dérivée d’une quelconque de ses primitives.

C’est une conséquence immédiate du th. 3 et de la prop. 6 de I, p. 22 de II, p. 5.

#### Corollaire 2 {#fvr-ii-s1-thm-3-cor-2 .statement}

Soient $f_i$ ($1 \leq i \leq n$) $n$ fonctions réglées dans un intervalle $I$, $f_i$ prenant ses valeurs dans un espace normé complet $E_i$ sur $\mathbf{R}$ ($1 \leq i \leq n$). Si $g$ est une application continue du sous-espace $\prod_{i=1}^n \overline{f_i(I)}$ de $\prod_{i=1}^n E_i$ dans un espace normé complet $F$ sur $\mathbf{R}$, la fonction composée $x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x))$ est réglée dans $I$.

En effet, elle satisfait de façon évidente aux conditions du th. 3 de II, p. 5.

On voit ainsi que si $f$ est une fonction vectorielle réglée dans $I$, la fonction numérique $x \mapsto \|f(x)\|$ est aussi réglée. De même, les fonctions numériques réglées dans $I$ forment un anneau; en outre, si $f$ et $g$ sont deux fonctions numériques réglées, $\sup(f, g)$ et $\inf(f, g)$ sont réglées.

Remarque — 1.) Si $f$ est une fonction numérique réglée dans $I$, $g$ une fonction vectorielle réglée dans un intervalle contenant $f(I)$, la fonction composée $g \circ f$ n’est pas nécessairement réglée (cf. II, p. 29, exerc. 4).

Deux cas particuliers du th. 3 de II, p. 5 sont spécialement importants:

#### Proposition 3 {#fvr-ii-s1-prop-3 .statement}

Toute fonction vectorielle continue dans un intervalle $I \subset \mathbf{R}$, prenant ses valeurs dans un espace normé complet $E$ sur $\mathbf{R}$, est réglée et admet dans $I$ une primitive, dont elle est la dérivée en tout point.

Remarques — 2.) Pour démontrer qu’une fonction continue admet une primitive, on peut utiliser le fait que tout polynôme (à coefficients dans $E$) d’une variable réelle admet une primitive; comme d’après le th. de Weierstrass (TG, X, p. 37, prop. 3) toute fonction continue est limite uniforme de polynômes dans tout intervalle compact, le th. 1 de II, p. 2 montre que toute fonction continue admet une primitive.

3) Le principe de la remarque précédente s’étend sans modification importante aux fonctions vectorielles d’une variable complexe, à valeurs dans un espace normé complet sur $\mathbf{C}$. Si $U$ est un ensemble ouvert dans $\mathbf{C}$, homéomorphe à $\mathbf{C}$, une primitive d’une telle fonction vectorielle $f$ définie dans $U$ est par définition une fonction continue dans $U$, ayant une dérivée égale à $f$ en tout point de $U$. Avec cette définition, le th. 1 de II, p. 2 s’étend sans modification (on démontre en effet, en tenant compte de ce que $U$ est connexe, que $(g_a)$ est uniformément convergente suivant $\mathfrak{g}$ dans un voisinage de tout point de $U$, d’où résulte que $(g_a)$ est uniformément convergente suivant $\mathfrak{g}$ dans toute partie compacte de $U$; la fin de la démonstration se fait en utilisant la prop. 4 de I, p. 26). Par suite, toute fonction qui est limite uniforme de polynômes dans toute partie compacte de U, admet une primitive dans U ; ces fonctions ne sont autres que les fonctions dites holomorphes dans U, que nous étudierons plus en détail dans un Livre ultérieur.

#### Proposition 4 {#fvr-ii-s1-prop-4 .statement}

Toute fonction numérique f monotone dans un intervalle I ⊂ ℝ est réglée, et toute primitive de f est convexe dans I.

En effet, f satisfait au critère du th. 3 de TG, IV, p. 19, prop 4; la seconde partie de la proposition résulte cor. 1 , de II, p. 6, et de la prop. 5 de I, p. 36.

Remarque — 4.) Il ne faudrait pas croire que les fonctions réglées dans un intervalle I soient les seules fonctions ayant une primitive dans I (cf. II, p. 29, exerc. 7 et 8).

### 4. Intégrales

Nous avons obtenu (II, p. 5, th. 2) une primitive d’une fonction réglée dans un intervalle I comme limite uniforme de primitives de fonctions en escalier. Ce procédé peut s’exprimer de façon légèrement différente: soient x₀, x deux points quelconques de I tels que x₀ < x; appelons subdivision de l’intervalle (x₀, x) toute suite d’intervalles (xᵢ, xᵢ₊₁) de réunion {x₀, x}, où (xᵢ)₀≤i≤n est une suite strictement croissante de points de {x₀, x} telle que xₙ = x. Nous appellerons somme de Riemann relative à une fonction vectorielle f définie dans I, et à la subdivision formée des (xᵢ, xᵢ₊₁) toute expression de la forme $\sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)$ où tᵢ appartient à (xᵢ, xᵢ₊₁) pour $0 \leq i \leq n-1$. On a alors la proposition suivante:

#### Proposition 5 {#fvr-ii-s1-prop-5 .statement}

Soient f une fonction réglée dans un intervalle I, g une primitive de f dans I, (x₀, x) un intervalle compact contenu dans I. Pour tout ε > 0, il existe un nombre ρ > 0 tel que, pour toute subdivision de (x₀, x) en intervalles de longueur ≤ ρ, on ait

$$
\|g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)\| \leq \varepsilon
$$

pour toute somme de Riemann relative à cette subdivision.

En effet, soit f une fonction en escalier telle que $\|f(y) - f_1(y)\| \leq \varepsilon$ pour tout $y \in (x_0, x)$; on a, en désignant par g₁ une primitive de f₁ dans I,

$$
\|g(x) - g(x_0) - (g_1(x) - g_1(x_0))\| \leq \varepsilon(x - x_0)
$$

d’après le th. des accroissements finis, et d’autre part

$$
\left\| \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) - \sum_{i=0}^{n-1} f_1(t_i)(x_{i+1} - x_i) \right\| \leq \varepsilon(x - x_0).
$$

Il suffit donc de démontrer la proposition lorsque f est une fonction en escalier. Soit $(y_k)_{1 \leq k \leq m}$ la suite finie strictement croissante des points de discontinuité de f dans $[x_0, x]$. Pour toute subdivision de $[x_0, x]$ en intervalles de longueur ≤ ρ, chacun des points $y_k$ appartient à deux intervalles au plus; il ne peut donc y avoir que $2m$ intervalles au plus dans lesquels $f$ ne soit pas constante; or, dans un tel intervalle $(x_i, x_{i+1})$, on a
$$
\|g(x_{i+1}) - g(x_i) - f(t_i)\ (x_{i+1} - x_i)\| \leq 2M\ (x_{i+1} - x_i)
$$
en désignant par $M$ la borne supérieure de $\|f\|$ dans $(x_0, x)$; au contraire, lorsque $f$ est constante dans $(x_i, x_{i+1})$, on a
$$
g(x_{i+1}) - g(x_i) - f(t_i)\ (x_{i+1} - x_i) = 0.
$$
On voit donc que la différence $\|g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)\ (x_{i+1} - x_i)\|$ ne peut excéder $4Mm\rho$; il suffit donc de prendre $\rho \leq \varepsilon/4Mm$ pour obtenir (1).

Remarque — 1.) Lorsque $f$ est continue, la prop. 5 se démontre plus simplement: comme $f$ est uniformément continue dans $(x_0, x)$, il existe $\rho > 0$ tel que dans tout intervalle de longueur $\leq \rho$ contenu dans $(x_0, x)$, l’oscillation de $f$ soit $\leq \frac{\varepsilon}{x - x_0}$; pour toute subdivision de $(x_0, x)$ en intervalles $(x_i, x_{i+1})$ de longueur $\leq \rho$, et tout choix de $t_i$ dans $(x_i, x_{i+1})$ pour $0 \leq i \leq n - 1$, la fonction en escalier $f_1$ égale à $f(t_i)$ dans $(x_i, x_{i+1})$ ($0 \leq i \leq n - 1$), à $f(x)$ au point $x$, est telle que $\|f(y) - f_1(y)\| \leq \frac{\varepsilon}{x - x_0}$ dans $(x_0, x)$; si $g_1$ est une primitive de $f_1$, on a $g_1(x) - g_1(x_0) = \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)$, donc la relation (1) résulte aussitôt de l’application du th. des accroissements finis.

Dans tout le reste de ce chapitre, nous allons nous borner à l’étude des primitives des fonctions réglées dans un intervalle I. Pour une telle fonction $f$, à valeurs dans E, une primitive $g$ de $f$, et deux points quelconques $x_0, x$ de I, l’élément $g(x) - g(x_0)$ de E (qui évidemment est le même, quelle que soit la primitive $g$ de $f$ que l’on considère) est appelé intégrale de la fonction $f$ de $x_0$ à $x$ (ou dans l’intervalle compact $[x_0, x]$) et noté $\int_{x_0}^x f(t)dt$ ou $\int_{x_0}^x f$. Ce nom et cette notation ont leur origine dans la prop. 5 de II, p. 7, qui montre qu’une intégrale peut être approchée arbitrairement par une somme de Riemann; plus particulièrement, on peut, en prenant des subdivisions de $(x_0, x)$ en intervalles égaux, écrire
$$
\frac{1}{x - x_0} \int_{x_0}^x f(t)\ dt = \lim_{n \to \infty} \frac{1}{n} \sum_{k=0}^{n-1} f\left(x_0 + k \frac{x - x_0}{n}\right).
$$
Autrement dit, l’élément $\frac{1}{x - x_0} \int_{x_0}^x f(t)dt$ est limite de la moyenne arithmétique des valeurs de $f$ aux origines des intervalles d’une subdivision de $(x_0, x)$ en intervalles égaux; aussi l’appelle-t-on encore la moyenne (ou valeur moyenne) de la fonction $f$ dans l’intervalle $[x_0, x]$.

Par définition, la fonction $x \mapsto \int_{x_0}^x f(t)\ dt$ n’est autre que la primitive de $f$ qui s’annule au point $x_0 \in I$; aussi la note-t-on encore $\int_{x_0}^x f(t)\ dt$ ou $\int_{x_0}^x f$.

#### Remarque 2 {#fvr-ii-s1-n4-rem-2 .statement}

Pour une fonction quelconque $h$ définie dans $I$, à valeurs dans $E$, l’élément $h(x) - h(x_0)$ s’écrit aussi $h(t)|_{x_0}^{x}$; avec cette notation, on voit que, si $g$ est une primitive quelconque de la fonction réglée $f$ dans $I$, on a

$$
\int_{x_0}^{x} f(t)\, dt = g(t)|_{x_0}^{x}.
$$

#### Remarque 3 {#fvr-ii-s1-n4-rem-3 .statement}

Les expressions $\int_{x_0}^{x} f(t)\, dt,\ g(t)|_{x_0}^{x}$ sont des « symboles abréviateurs » représentant des assemblages dans lesquels figurent les lettres $x,\ x_0,\ f,\ g$, mais non la lettre $t$ (cf. E, I, p. 14); on dit que dans ces symboles, $t$ est une « variable muette »; on peut donc y remplacer $t$ par tout autre argument distinct de $x,\ x_0,\ f$ et $g$ (et des arguments qui entrent éventuellement dans la démonstration où figurent de tels symboles) sans changer le sens du symbole obtenu (le lecteur comparera ces symboles à des symboles tels que $\sum_{i=1}^{n} x_i,\ \bigcup X_i$, où $i$ est de même une variable muette).

#### Remarque 4 {#fvr-ii-s1-n4-rem-4 .statement}

L’approximation d’une intégrale par des sommes de Riemann se rattache étroitement à l’une des origines historiques de la notion d’intégrale, le problème de la mesure des aires. Nous reviendrons sur ce point au Livre d’Intégration qui est consacré aux généralisations de la notion d’intégrale auxquelles a conduit ce problème; dans ces généralisations, les fonctions « intégrées » ne sont plus nécessairement définies dans une partie de $\mathbf{R}$; d’autre part, même lorsqu’il s’agit de fonctions numériques $f$ d’une variable réelle (non nécessairement réglées) pour lesquelles on peut définir une intégrale $\int_{x_0}^{x} f(t)\, dt$, la fonction $x \mapsto \int_{x_0}^{x} f(t)\, dt$ n’est pas toujours une primitive de $f$, et il existe des fonctions ayant une primitive, mais non « intégrables » au sens auquel nous faisons allusion.

### 5. Propriétés des intégrales

Les propriétés des intégrales des fonctions réglées ne sont autres que la traduction, dans la notation qui leur est propre, des propriétés des dérivées démontrées au chap. I.

En premier lieu, la formule (3) montre que, quels que soient les points $x,\ y,\ z$ de $I$, on a

$$
\int_{x}^{x} f(t)\, dt = 0
$$
$$
\int_{x}^{y} f(t)\, dt + \int_{y}^{x} f(t)\, dt = 0
$$
$$
\int_{x}^{y} f(t)\, dt + \int_{y}^{z} f(t)\, dt + \int_{z}^{x} f(t)\, dt = 0
$$

D’après la prop. 1 de II, p. 2, on a
$$
\int_{x_0}^{x} (f + g) = \int_{x_0}^{x} f + \int_{x_0}^{x} g
$$
et pour tout scalaire $k$
$$
\int_{x_0}^{x} kf = k \int_{x_0}^{x} f.
$$

Soient E, F deux espaces normés complets sur $\mathbf{R}$, $u$ une application linéaire continue de E dans F. Si $f$ est une fonction réglée dans I, à valeurs dans E, $u \circ f$ est une fonction réglée dans I, à valeurs dans F (II, p. 6, cor. 2), et on a (I, p. 13, prop. 2)

$$
\int_a^b u(f(t))\ dt = u \left( \int_a^b f(t)\ dt \right).
$$

Soient maintenant E, F, G trois espaces normés complets sur $\mathbf{R}$, $(x, y) \mapsto [x, y]$ une application bilinéaire continue de $E \times F$ dans G. Soient $f$ et $g$ deux fonctions vectorielles définies et continues dans I, prenant leurs valeurs dans E et F respectivement; supposons en outre que $f$ et $g$ soient toutes deux primitives de fonctions réglées, que nous désignerons par $f'$ et $g'$ par abus de langage (ces fonctions ne sont en effet égales respectivement aux dérivées de $f$ et $g$ qu’aux points du complémentaire d’un ensemble dénombrable). D’après la prop. 3 de I, p. 14, la fonction $h(x) = [f(x), g(x)]$ admet en tout point du complémentaire d’une partie dénombrable de I, une dérivée égale à $[f'(x), g'(x)] + [f'(x), g(x)]$. Or, d’après la continuité de $[x, y]$ et le cor. 2 de II, p. 7, chacune des fonctions $[f, g']$ et $[f', g]$ est une fonction réglée dans; I on a donc la formule

$$
\int_a^b [f'(t), g(t)]\ dt = [f(t), g(t)]|_a^b - \int_a^b [f(t), g'(t)]\ dt
$$

dite formule d’intégration par parties, qui permet de calculer de nombreuses primitives

Par exemple, la formule d’intégration par parties donne la formule suivante

$$
\int_{x_0}^\infty t f'(t)\ dt = t f(t)|_{x_0}^\infty - \int_{x_0}^\infty f(t)\ dt
$$

et ramène donc l’un à l’autre le calcul des primitives des deux fonctions $f(x)$ et $x f'(x)$.

De même, si $f$ et $g$ sont n fois dérivables dans un intervalle I, et si $f^{(n)}$ et $g^{(n)}$ sont des fonctions réglées dans I, la formule (5) de I, p. 29 équivaut à la suivante:

$$
\int_a^b [f^{(n)}(t), g(t)]\ dt \\
= \sum_{p=0}^{n-1} (-1)^p [f^{(n-p-1)}(t), g^{(p)}(t)]|_a^b + (-1)^n \int_a^b [f(t), g^{(n)}(t)]\ dt
$$

qu’on appelle formule d’intégration par parties d’ordre n.

Traduisons maintenant la formule de dérivation des fonctions composées (I, p. 17, prop. 5). Soit $f$ une fonction numérique définie et continue dans I, et qui soit primitive d’une fonction réglée dans I (que nous écrirons encore $f'$ par abus de langage); soit d’autre part $g$ une fonction vectorielle (à valeurs dans un espace normé complet) continue dans un intervalle ouvert J contenant $f(I)$; si $h$ désigne une primitive quelconque de g dans J, h admet en tout point de J une dérivée égale à g (II, p. 6, prop. 3); donc la fonction composée h ∘ f admet une dérivée égale à g(f(x))f'(x) en tous les points du complémentaire (par rapport à I) d’une partie dénombrable de I (I, p. 17, prop. 5); comme la fonction g(f(x))f'(x) est réglée (II, p. 7, cor 2), on peut écrire la formule

$$
\int_a^b g(f(t))f'(t)\,dt = \int_{f(a)}^{f(b)} g(u)\,du
$$

dite *formule du changement de variables*, qui facilite également le calcul des primitives.

Si on prend par exemple $f(x) = x^2$, on voit que la formule (13) ramène l’un à l’autre le calcul des primitives des fonctions g(x) et xg(x^2).

Pour traduire le th. des accroissements finis (I, p. 23, th. 1) pour les primitives de fonctions numériques réglées, remarquons d’abord qu’une fonction numérique réglée f dans un intervalle compact I est bornée dans I; soit J l’ensemble des points de I où f est *continue*, et posons $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$; on sait (II, p. 5, th. 3) que $I \cap \complement J$ est dénombrable; en outre, si B est le complémentaire, par rapport à I, d’une partie dénombrable quelconque de I, et $m' = \inf_{x \in B} f(x)$, $M' = \sup_{x \in B} f(x)$, on a $m' \leq m \leq M \leq M'$: en effet, en tout point $x \in J$, il existe des points y de B arbitrairement voisins de x, où on a donc $m' \leq f(y) \leq M'$; f étant continue au point x, on voit, en faisant tendre y vers x (y restant dans B) que $m' \leq f(x) \leq M'$, ce qui démontre notre assertion. Cela étant, la traduction du th. des accroissements finis donne la proposition suivante:

**Proposition 6** (théorème de la moyenne). — *Soit f une fonction numérique réglée dans un intervalle compact I = (a, b); si J est l’ensemble des points de I où f est continue, et $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$, on a*

$$
m < \frac{1}{b - a} \int_a^b f(t)\,dt < M
$$

sauf lorsque f est constante dans J, auquel cas les trois membres de (14) sont égaux.

En d’autres termes, la *moyenne* de la fonction réglée f dans I est comprise entre les bornes de f dans la partie de I où f est continue.

#### Corollaire 1 {#fvr-ii-s1-prop-5-cor-1 .statement}

*Si une fonction numérique f réglée dans I est telle que $f(x) \geq 0$ aux points où f est continue, on a* $\frac{1}{b - a} \int_a^b g(t)\,dt > 0$ *sauf si* $f(x) = 0$ *aux points ou f est continue.*

#### Corollaire 2 {#fvr-ii-s1-prop-5-cor-2 .statement}

Soient $f$ et $g$ deux fonctions numériques réglées dans $I$, telles que $g(x) \geqslant 0$ aux points où $g$ est continue ; si $m$ et $M$ sont les bornes inférieure et supérieure de $f$ dans l’ensemble des points de $I$ où $f$ est continue, on a

$$
\frac{m}{b-a} \int_a^b g(t)\ dt \leqslant \frac{1}{b-a} \int_a^b f(t)\ g(t)\ dt \leqslant \frac{M}{b-a} \int_a^b g(t)\ dt.
$$

Les deux premiers membres (resp. les deux derniers) ne sont égaux que si $g(x)(f(x)-m)=0$ (resp. $g(x)\ (f(x)-M)=0$) en tout point où $f$ et $g$ sont continues.

Pour les fonctions vectorielles, le th. des accroissements finis (I, p. 23, th. 2) donne de même la proposition suivante :

#### Proposition 7 {#fvr-ii-s1-prop-7 .statement}

Soit $\mathbf{f}$ une fonction vectorielle réglée dans un intervalle compact $I = [a,\ b]$, à valeurs dans un espace normé complet $E$, et soit $g$ une fonction numérique réglée dans $I$, telle que $g(x) \geqslant 0$ aux points où $g$ est continue ; dans ces conditions, on a

$$
\left\| \int_a^b \mathbf{f}(t)\ g(t)\ dt \right\| \leqslant \int_a^b \| \mathbf{f}(t) \| \ g(t)\ dt.
$$

En particulier, on a

$$
\left\| \int_a^b \mathbf{f}(t)\ dt \right\| \leqslant \int_a^b \| \mathbf{f}(t) \| \ dt.
$$

### 6. Forme intégrale du reste de la formule de Taylor; primitives d’ordre supérieur

La formule d’intégration par parties d’ordre $n$ (II, p. 10, formule (11)) permet d’exprimer sous forme d’une intégrale le reste $r_n(x)$ du développement de Taylor d’ordre $n$ d’une fonction $\mathbf{f}$ admettant une dérivée $(n+1)$-ème réglée dans un intervalle $I$ (I, p. 30) ; en effet, en remplaçant, dans (12), $\mathbf{f}$ par $\mathbf{f}'$, $b$ par $x$ et $g(t)$ par la fonction $(t-x)^n/n!$, il vient

$$
\mathbf{f}(x) = \mathbf{f}(a) + \mathbf{f}'(a) \frac{(x-a)}{1!} + \mathbf{f}''(a) \frac{(x-a)^2}{2!} + \ldots + \mathbf{f}^{(n)}(a) \frac{(x-a)^n}{n!} + \int_a^x \mathbf{f}^{(n+1)}(t) \frac{(x-t)^n}{n!}\ dt
$$

autrement dit

$$
r_n(x) = \int_a^x \mathbf{f}^{(n+1)}(t) \frac{(x-t)^n}{n!}\ dt
$$

formule qui permet souvent d’obtenir des majorations simples du reste.

Étant donnée une fonction $\mathbf{f}$ réglée dans un intervalle $I$, une primitive quelconque $g$ de $\mathbf{f}$, étant continue dans $I$, admet à son tour une primitive ; une quelconque des primitives d’une primitive quelconque de $\mathbf{f}$ est appelée primitive seconde de $\mathbf{f}$. Plus généralement, on appelle primitive d’ordre $n$ de $\mathbf{f}$ une primitive d’une primitive d’ordre $n - 1$ de $\mathbf{f}$. On voit aussitôt, par récurrence sur $n$, que la différence de deux primitives d’ordre $n$ de $\mathbf{f}$ est un polynôme de degré au plus égal à $n - 1$ (à coefficients dans $\mathbf{E}$). Une primitive d’ordre $n$ de $\mathbf{f}$ est entièrement déterminée si on se donne, en un point $a \in I$, sa valeur et celles de ses $n - 1$ premières dérivées.

On désignera en particulier par la notation $\int_a^{(n)} \mathbf{f}$ celle des primitives d’ordre $n$ de $\mathbf{f}$ qui est nulle au point $a$ ainsi que ses $n - 1$ premières dérivées. La formule de Taylor d’ordre $n - 1$, appliquée à cette primitive, montre que si $\mathbf{g} = \int_a^{(n)} \mathbf{f}$, on a

$$
\mathbf{g}(x) = \int_a^x \mathbf{f}(t) \frac{(x - t)^{n-1}}{(n-1)!} \, dt
$$

et ramène la détermination des primitives d’ordre $n$ au calcul d’une seule intégrale.

## EXERCICES {#fvr-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
