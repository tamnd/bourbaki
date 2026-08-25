---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 7
section_title: Convergence de la série de Hausdorff (cas réel ou complexe)
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0058-0063, 0090-0090
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes-continus à valeurs dans $g$
      page: 0
      pdf_page: 58
    - "no": 2
      title: Groupuscule défini par une algèbre de Lie normée complète
      page: 0
      pdf_page: 59
    - "no": 3
      title: Exponentielle dans les algèbres associatives normées complètes
      page: 0
      pdf_page: 62
statements: 4
exercises: 1
content_sha256: f070f248cb487d9e5e0c1908035e44c2b46f7939b9896ff1e9bf73f440ad0bfe
---

## § 7. Convergence de la série de Hausdorff (cas réel ou complexe)

Dans ce paragraphe, on suppose que K est l’un des corps $\mathbf{R}$ ou $\mathbf{C}$ que l’on munit de sa valeur absolue usuelle. Rappelons qu’on appelle algèbre normable sur K une algèbre A (non nécessairement associative) sur K, munie d’une topologie $\mathcal{T}$ possédant les propriétés suivantes:
1) $\mathcal{T}$ peut être définie par une norme;
2) l’application $(x, y) \mapsto xy$ de $A \times A$ dans A est continue.

On appelle algèbre normée sur K une algèbre A sur K, munie d’une norme telle que $\|xy\| \leq \|x\|\|y\|$ quels que soient $x, y$ dans A.

On désigne par $g$ une algèbre de Lie normable complète sur K. On choisit une norme sur $g$ et un nombre $M > 0$ tels que

$$(1)$$ $\|[x, y]\| \leq M \|x\|\|y\| \quad \text{pour } x, y \text{ dans } g.$

### 1. Polynômes-continus à valeurs dans $g$

Soit I un ensemble fini et soit $P(g^I; g)$ (resp. $\hat{P}(g^I; g)$) l’espace vectoriel des polynômes-continus (resp. séries formelles à composantes continues) sur $g^I$ à valeurs dans $g$. Rappelons (VAR, R, App.) que $P(g^I; g)$ est muni d’une graduation de type $\mathbf{N}^I$ et que $\hat{P}(g^I; g)$ s’identifie au complété de l’espace vectoriel $P(g^I; g)$ pour la topologie définie par la filtration associée à la graduation de $P(g^I; g)$. De plus, $P(g^I; g)$ est une algèbre de Lie graduée pour le crochet défini par $[f, g](x) = [f(x), g(x)]$ pour $f, g$ dans $P(g^I; g)$, $x \in g^I$; cette structure d’algèbre de Lie se prolonge par continuité à $\hat{P}(g^I; g)$ et en fait une algèbre de Lie filtrée séparée et complète.

D’après la prop. 2 du § 6, n° 3, il existe un homomorphisme continu $\varphi_I : u \mapsto \tilde{u}$ d’algèbres de Lie et un seul de $\hat{L}(I)$ dans $\hat{P}(g^I; g)$ appliquant l’indéterminée d’indice $i$ sur $pr_i$ pour tout $i \in I$, puisque $pr_i \in P(g^I; g)$. Il en résulte que $\tilde{u} \in P(g^I; g)$ pour $u \in L(I)$; plus précisément, lorsque $u \in L(I)$, $\tilde{u}$ n’est autre que l’application polynomiale $(t_i) \mapsto u((t_i))$ du § 2, n° 4. Il est d’autre part clair que $\varphi_I$ est compatible avec les multigraduations de $L(I)$ et $P(g^I; g)$. Si $u = \sum_{v \in \mathbf{N}^I} u_v$, où $u_v \in L^v(I)$ pour $v \in \mathbf{N}^I$, on a
$$
\tilde{u} = \sum_{v \in \mathbf{N}^I} \tilde{u}_v,\quad \text{avec } \tilde{u}_v \in P_v(g^I; g).
$$
Soit $u = (u_j)_{j \in J}$ une famille *finie* d’éléments de $\hat{L}(I)$, soit $v \in \hat{L}(J)$ et soit $w = v \circ u$ (\S 6, n° 3). Posons $\tilde{u} = (\tilde{u}_j)_j \in \mathcal{J}$. On a
$$(2)\qquad \tilde{v} \circ \tilde{u} = (v \circ u)^{\sim}.$$
En effet, ceci résulte par prolongement par continuité de la formule (7) du § 6, n° 3, et de (VAR, R, App., n° 6).

### 2. Groupuscule défini par une algèbre de Lie normée complète

Soient $H = \sum_{r,s \geq 0} H_{r,s} \in \hat{L}(U, V)$ la série de Hausdorff (\S 6, n° 4, déf. 1). Nous allons montrer que la série formelle correspondante
$$(3)\qquad \tilde{H} = \sum_{r,s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)$$
est *convergente* (VAR, R, 3.1.1).
Introduisons la série formelle $\eta \in \mathbf{Q}[[U, V]]$ suivante
$$(4)\qquad \eta(U, V) = -\log(2 - \exp(U + V))$$
$$(5)\qquad = \sum_{m \geq 1} \frac{1}{m} (\exp(U + V) - 1)^m$$
$$(6)\qquad = \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1, \ldots, r_m \\ s_1, \ldots, s_m \\ r_i + s_i \geq 1}} \frac{U^{r_1} V^{s_1}}{r_1! s_1!} \frac{U^{r_2} V^{s_2}}{r_2! s_2!} \cdots \frac{U^{r_m} V^{s_m}}{r_m! s_m!}.$$
D’où
$$(7)\qquad \eta(U, V) = \sum_{r,s \geq 0} \eta_{r,s} U^r V^s,$$
avec
$$(8)\qquad \eta_{r,s} = \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_i + s_i \geq 1}} \frac{1}{r_1! \cdots r_m! s_1! \cdots s_m!}.$$
Soient maintenant $u$ et $v$ deux nombres réels positifs tels que $u + v < \log 2$; on a $0 \leq \exp(u + v) - 1 < 1$; les séries déduites de (5) et (6) par substitution de $u$ à $U$ et de $v$ à $V$ sont convergentes, et les calculs précédents entraînent
$$(9)\qquad \sum_{r,s \geq 0} \eta_{r,s} u^r v^s = -\log(2 - \exp(u + v)) < +\infty.$$
Soient $r, s \geq 0$, et soit $\|\tilde{H}_{r,s}\|$ la norme du polynôme-continu $\tilde{H}_{r,s}$ (VAR, R, App., n° 2).

#### Lemme 1 {#lie-ii-s7-lem-1 .statement}

On a

$$
\|\tilde{H}_{r,s}\| \leq M^{r+s-1} \eta_{r,s}
$$

Soient $r_i, s_i$ dans $\mathbf{N}$ pour $1 \leq i \leq m$, avec $s_m = 1$; posons $r = \sum_i r_i, s = \sum_i s_i$ et considérons l’élément suivant de $L(\{U, V\})$:

$$
Z = \left( \left( \prod_{i=1}^{m-1} (\mathrm{ad}U)^{r_i} (\mathrm{ad}V)^{s_i} \right) (\mathrm{ad}U)^{r_m} \right)(V).
$$

On a $\tilde{Z} = f \circ p$, où $f$ est l’application $(r + s)$-linéaire de $g^{r+s}$ dans $g$ suivante:

$$
(x_1, \ldots, x_r, y_1, \ldots, y_s) \mapsto \\
(\mathrm{ad}(x_1) \circ \cdots \circ \mathrm{ad}(x_{r_1}) \circ \mathrm{ad}(y_1) \circ \cdots \circ \mathrm{ad}(y_{s_1}) \circ \mathrm{ad}(x_{r_1+1}) \circ \cdots \circ \mathrm{ad}(x_r))(y_s)
$$

et où $p$ est l’application de $g^2$ dans $g^{r+s}$ suivante:

$$
(x, y) \mapsto (\underbrace{x, \ldots, x}_{r}, \underbrace{y, \ldots, y}_{s});
$$

on a donc $\|\tilde{Z}\| \leq \|f\| \leq M^{r+s-1}$ (VAR, R, App.). Appliquant cette majoration aux différents termes du second membre de la formule (9) du § 6, n° 4, on obtient:

$$
(10) \quad \|(\tilde{H}'_{r,s})^\sim\| \leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s-1 \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \cdots r_m! s_1! \cdots s_{m-1}!}.
$$

Un raisonnement analogue donne

$$
(11) \quad \|(\tilde{H}''_{r,s})^\sim\| \leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \cdots r_{m-1}! s_1! \cdots s_{m-1}!},
$$

d’où, d’après (8),

$$
\|\tilde{H}_{r,s}\| \leq \eta_{r,s} \frac{M^{r+s-1}}{r+s} \leq \eta_{r,s} M^{r+s-1},
$$

ce qui démontre le lemme.

#### Proposition 1 {#lie-ii-s7-prop-1 .statement}

La série formelle $\tilde{H}$ est une série convergente (VAR, R, 3.1.1); son domaine de convergence strict (VAR, R, 3.1.4) contient l’ouvert

$$
\Omega = \left\{ (x, y) \in g \times g \mid \|x\| + \|y\| < \frac{1}{M} \log 2 \right\}.
$$

En effet, soient $u, v$ deux nombres réels $> 0$ tels que $u + v < \frac{1}{M} \log 2$; on a (lemme 1)

$$
(12) \quad M \sum_{r,s \geq 0} \|\tilde{H}_{r,s}\| u^r v^s \leq \sum_{r,s \geq 0} \eta_{r,s} M^{r+s} u^r v^s = - \log (2 - \exp M(u + v)) < +\infty
$$

d’après (9).

Notons $h : \Omega \to g$ la fonction analytique (VAR, R, 3.2.9) définie par $\tilde{H}$, c’est-à-dire par la formule

$$
h(x, y) = \sum_{r,s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y) \quad \text{pour } (x, y) \in \Omega.
$$

Cette fonction s’appelle la fonction de Hausdorff de $g$ relativement à $M$ (ou simplement la fonction de Hausdorff de $g$ si aucune confusion n’est à craindre). Remarquons que $H_{r,s}(U, -U) = 0$ pour $r + s \geq 2$, donc

$$
h(x, -x) = 0 \qquad \text{pour } \|x\| < \frac{1}{2M} \log 2.
$$

De même

$$
h(0, x) = h(x, 0) = x \qquad \text{pour } \|x\| < \frac{1}{M} \log 2.
$$

#### Proposition 2 {#lie-ii-s7-prop-2 .statement}

*Soit*

$$
\Omega' = \left\{ (x, y, z) \in g \times g \times g \mid \|x\| + \|y\| + \|z\| < \frac{1}{M} \log \frac{3}{2} \right\}.
$$

*Si* $(x, y, z) \in \Omega'$, *on a*

$$(x, y) \in \Omega,\qquad (h(x, y), z) \in \Omega,\qquad (y, z) \in \Omega,\qquad (x, h(y, z)) \in \Omega$$

*et*

$$
h(h(x, y), z) = h(x, h(y, z)).
$$

Soit $(x, y, z) \in \Omega'$; il est clair que $(x, y) \in \Omega$ et que $(y, z) \in \Omega$. De plus, on a:

$$
\|h(x, y)\| \leq \sum_{r,s} \|\tilde{H}_{r,s}\| \|x\|^r \|y\|^s,
$$

donc d’après (13)

$$
\|h(x, y)\| \leq - \frac{1}{M} \log (2 - \exp M(\|x\| + \|y\|)).
$$

Or $M(\|x\| + \|y\|) < \log \frac{3}{2} - M\|z\|$; posons $u = \exp(M\|z\|)$; on a $1 \leq u \leq \frac{3}{2}$ et

$$
\begin{align*}
M(\|h(x, y)\| + \|z\|) &< -\log (2 - \exp(\log \frac{3}{2} - M\|z\|)) + M\|z\| \\
&= -\log \left(2 - \frac{3}{2u}\right) + \log u = \log \frac{2u^2}{4u - 3} \\
&= \log \left(2 + \frac{2(u-1)(u-3)}{4u-3}\right) \leq \log 2.
\end{align*}
$$

On voit de même que $(x, h(y, z)) \in \Omega$.

Démontrons maintenant (17). Dans l’algèbre de Lie $\hat{L}(\{U, V, W\})$, on a

$$
H(H(U, V), W) = H(U, H(V, W))
$$

d’après la prop. 4 du § 6, n° 5. D’après le n° 1, formule (2), on a donc dans $\hat{P}(g \times g \times g, g)$ la relation
$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H}).
$$
D’après VAR, R, 3.1.9, il existe un nombre $\varepsilon > 0$ tel que la formule (17) soit vraie lorsque $\|x\|, \|y\|$ et $\|z\|$ sont $\leq \varepsilon$. Mais les fonctions $(x, y, z) \mapsto h(h(x, y), z)$ et $(x, y, z) \mapsto h(x, h(y, z))$ sont des fonctions analytiques dans $\Omega'$ à valeurs dans $g$ (VAR, R, 3.2.7). Comme $\Omega'$ est connexe, et qu’elles coïncident au voisinage de 0, elles sont égales (VAR, R, 3.2.5).

Les résultats précédents entraînent:

Soit $\alpha$ un nombre réel tel que $0 < \alpha \leq \frac{1}{3M} \log \frac{3}{2}$. Soient $G = \{ x \in g \mid \|x\| < \alpha \}$,
$\Theta = \{ (x, y) \in G \times G \mid h(x, y) \in G \}$, et $m : \Theta \to G$ la restriction de $h$ à $\Theta$. Alors:
1) $\Theta$ est ouvert dans $G \times G$, et $m$ est analytique.
2) $x \in G$ implique $(0, x) \in \Theta$, $(x, 0) \in \Theta$ et $m(0, x) = m(x, 0) = x$.
3) $x \in G$ implique $-x \in G$, $(x, -x) \in \Theta$, $(-x, x) \in \Theta$ et $m(x, -x) = m(-x, x) = 0$.
4) Soient $x, y, z$ dans $G$ tels que $(x, y) \in \Theta$, $(m(x, y), z) \in \Theta$, $(y, z) \in \Theta$ et $(x, m(y, z)) \in \Theta$. Alors $m(m(x, y), z) = m(x, m(y, z))$.
*Autrement dit* (chap. III, § 1), *si on pose* $-x = \sigma(x)$, *le quadruplet* $(G, 0, \sigma, m)$ *est un groupuscule de Lie sur K.*

### 3. Exponentielle dans les algèbres associatives normées complètes

Dans ce n°, on désigne par $A$ une *algèbre associative unifière normée complète* (TG, IX, § 3, n° 7). On a donc $\|x.y\| \leq \|x\| \cdot \|y\|$ pour $x, y$ dans $A$.

Soit $I$ un ensemble *fini* et soit $\hat{P}(A^I; A)$ l’espace vectoriel des *séries formelles à composantes continues* sur $A^I$ à valeurs dans $A$ (VAR, R, App., n° 5), munie de la structure d’algèbre obtenue en posant
$$
f.g = m \circ (f, g) \quad \text{pour } f, g \text{ dans } \hat{P}(A^I; A),
$$
où $m : A \times A \to A$ désigne la multiplication de $A$. Raisonnant comme au n° 1 et utilisant la prop. 1 du § 5, n° 1, on définit un homomorphisme continu d’algèbres unifères $u \mapsto \tilde{u}$ de $\hat{A}(I)$ dans $\hat{P}(A^I; A)$ appliquant l’indéterminée d’indice $i$ sur $\mathrm{pr}_i$; cet homomorphisme prolonge l’homomorphisme d’algèbres de Lie de $\hat{L}(I)$ dans $\hat{P}(A^I; A)$ défini au n° 1. Si $u = \sum_v u_v$ avec $u_v \in A^v(I)$ pour $v \in \mathbf{N}^I$, alors $\tilde{u} = \sum_v \tilde{u}_v$, où $\tilde{u}_v$ est l’application polynomiale $(t_i)_{i \in I} \mapsto u_v((t_i))$.

Soit $u = (u_j)_{j \in J}$ une famille finie d’éléments de $\hat{A}(I)$, soit $v \in \hat{A}(J)$ et posons $w = v \circ u$ (§ 5, n° 1). On a
$$(18)$$
$$(v \circ u)^{\sim} = \tilde{v} \circ \tilde{u}.$$

Prenons en particulier $I = \{U\}$, identifions $A$ et $A^{(U)}$, et considérons les images $\tilde{e}$ et $\tilde{l}$ des séries $e(U) = \sum_{n \geq 1} U^n / n!$ et $l(U) = \sum_{n \geq 1} (-1)^{n-1} U^n / n$ dans $\hat{P}(A; A)$. On a $\| \widetilde{U^n} \| \leq 1$ car $\| x_1 \ldots x_n \| \leq \| x_1 \| \ldots \| x_n \|$ pour $x_1, \ldots, x_n$ dans $A$. Par suite, le *rayon de convergence strict de $\tilde{e}$* (resp. $l$) *est infini* (resp. $\geq 1$).

Nous désignerons par $e_A$ (resp. $l_A$) l’application analytique de $A$ dans $A$ (resp. de $B$ dans $A$, où $B$ est la boule unité ouverte de $A$) définie par la série convergente $\tilde{e}$ (resp. $\tilde{l}$) et nous poserons $\exp_A(x) = 1 + e_A(x)$ (pour $x \in A$) et $\log_A(x) = l_A(x - 1)$ (pour $x \in A, \| x - 1 \| < 1$). On a donc

$$
\exp_A x = \sum_{n \geq 0} \frac{x^n}{n!} \quad (x \in A)
$$

$$
\log_A x = \sum_{n \geq 1} (-1)^{n-1} \frac{(x - 1)^n}{n} \quad (x \in A, \| x - 1 \| < 1).
$$

Comme $(e \circ l)(U) = (l \circ e)(U) = U$ (cf. § 6, n° 1), on a d’après (18) $\tilde{e} \circ \tilde{l} = \tilde{l} \circ \tilde{e} = \mathrm{Id}_A$. Par suite (VAR, R, 3.1.9)

$$
\exp_A(\log_A(x)) = x \quad (x \in A, \| x - 1 \| < 1)
$$
$$
\log_A(\exp_A(x)) = x \quad (x \in A, \| x \| < \log 2)
$$

car $\| x \| < \log 2$ entraîne $\| \exp_A(x) - 1 \| \leq \exp \| x \| - 1 < 1$.

Enfin, considérons $A$ comme une algèbre de Lie normée complète. On a $\|[x, y]\| = \|xy - yx\| \leq 2\|x\|\cdot\|y\|$. La prop. 1 du n° 2 entraîne que le domaine de convergence strict de la série formelle $\tilde{H}$ contient l’ensemble

$$
\Omega = \{ (x, y) \in A \times A \mid \| x \| + \| y \| < \frac{1}{2} \log 2 \}.
$$

Donc $\tilde{H}$ définit une fonction analytique $h : \Omega \to A$. On a $h(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y)$ (cf. § 3, n° 1, *Remarque 4*).

#### Proposition 3 {#lie-ii-s7-prop-3 .statement}

*Pour $\| x \| + \| y \| < \frac{1}{2} \log 2$, on a*

$$
\exp_A x \cdot \exp_A y = \exp_A h(x, y).
$$

En effet, il résulte de (18) et de la relation $e^U e^V = e^{H(U, V)}$ que

$$
m \circ (1 + \tilde{e}, 1 + \tilde{e}) = (1 + \tilde{e}) \circ \tilde{H}
$$

dans $\hat{P}(A \times A; A)$. On déduit donc de VAR, R, 3.1.9, que (23) est vraie pour $(x, y)$ assez voisin de $(0, 0)$, d’où la proposition par prolongement analytique (VAR, R, 3.2.5).

## EXERCICES {#lie-ii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
