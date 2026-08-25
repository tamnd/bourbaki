---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 5
section_title: Calculs formels dans les groupes de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0182-0189, 0263-0264
extraction: ocr
subsections:
    - "no": 1
      title: Les coefficients $c_{\alpha \beta \gamma}$
      page: 0
      pdf_page: 183
    - "no": 2
      title: Crochet dans l’algèbre de Lie
      page: 0
      pdf_page: 184
    - "no": 3
      title: Puissances
      page: 0
      pdf_page: 185
    - "no": 4
      title: Exponentielle
      page: 0
      pdf_page: 188
statements: 8
exercises: 2
content_sha256: f3689cb510418d67f1099834733ee4dd94b1c5eeaa96784df78a9541b550365b
---

## § 5. Calculs formels dans les groupes de Lie

Soient $f, g$ deux séries formelles à coefficients dans K par rapport aux mêmes indéterminées; soit $f_i$ (resp. $g_i$) la composante homogène de degré $i$ de $f$ (resp. $g$). Nous écrirons

$$
f \equiv g \pmod{\deg p}
$$

si $f_i = g_i$ pour $i < p$.

Dans ce §, G désigne un groupuscule de Lie de dimension finie $n$; le corps de base K est supposé de caractéristique zéro. On identifie une fois pour toutes, à l’aide d’une carte, un voisinage ouvert de $e$ dans G à un voisinage ouvert U de 0 dans $K^n$, de façon que $e$ s’identifie à 0. Pour $x, y$ dans U et $n \in \mathbf{Z}$, on note $x.y$ le produit de $x$ et $y$, et $x^{[m]}$ la puissance $m$-ème de $x$ dans G (lorsqu’ils sont définis). Les coordonnées de $x \in U$ sont notées $x_1, x_2, \ldots, x_n$.

### 1. Les coefficients $c_{\alpha \beta \gamma}$

Soit $\Omega$ l’ensemble des $(x, y) \in \mathbf{U} \times \mathbf{U}$ tels que $x.y$ soit défini et appartienne à $\mathbf{U}$. Alors $\Omega$ est ouvert dans $\mathbf{U} \times \mathbf{U}$, et l’application $(x, y) \mapsto x.y$ de $\Omega$ dans $\mathbf{U}$ est analytique. Les coordonnées $z_1, \ldots, z_n$ de $z = x.y$ admettent donc des développements en série entière à l’origine suivant les puissances de $x_1, \ldots, x_n, y_1, \ldots, y_n$. Par suite, il existe des constantes $c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} \in \mathbf{K}$, bien déterminées, telles que

(1)
$$
z_1^{\gamma_1} \ldots z_n^{\gamma_n} = \sum_{\alpha_1, \ldots, \beta_n \in \mathbf{N}} c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} x_1^{\alpha_1} \ldots x_n^{\alpha_n} y_1^{\beta_1} \ldots y_n^{\beta_n}
$$
pour $\gamma_1, \ldots, \gamma_n$ dans $\mathbf{N}$. Adoptant les conventions de VAR, R, nous écrirons ces formules plus brièvement:

(2)
$$
(x.y)^{\gamma} = \sum_{\alpha, \beta \in \mathbf{N}^n} c_{\alpha, \beta, \gamma} x^{\alpha} y^{\beta} \quad (\gamma \in \mathbf{N}^n).
$$

Puisque $x.0 = 0.x = x$ pour $x \in \mathbf{U}$, on a

(3)
$$
c_{\alpha, 0, \gamma} = c_{0, \alpha, \gamma} = \delta_{\alpha \gamma}
$$
où $\delta_{\alpha \gamma}$ est l’indice de Kronecker. En particulier, écrivant désormais $k$ à la place de $\varepsilon_k$ pour $k = 1, \ldots, n$,

(4)
$$
(x.y)_k = x_k + y_k + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha, \beta, k} x^{\alpha} y^{\beta}.
$$

Posant $c_{\alpha \beta} = (c_{\alpha \beta 1}, c_{\alpha \beta 2}, \ldots, c_{\alpha \beta n}) \in \mathbf{K}^n$, on a donc

(5)
$$
x.y = x + y + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$

Au second membre de (5), considérons la composante homogène de degré 2:

$$
B(x, y) = \sum_{i, j = 1}^n c_{ij} x_i y_j
$$
de sorte que $(x, y) \mapsto B(x, y)$ est une application bilinéaire de $\mathbf{K}^n \times \mathbf{K}^n$ dans $\mathbf{K}^n$.

On a

(6)
$$
x.y \equiv x + y + B(x, y) \pmod{\deg 3}.
$$

La formule (4) entraîne d’autre part que

(7)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{si} \quad |\alpha| + |\beta| < |\gamma|
$$
et que les termes de degré total $|\gamma|$ dans le développement de $z^{\gamma}$ sont aussi ceux de $(x_1 + y_1)^{\gamma_1}(x_2 + y_2)^{\gamma_2} \ldots (x_n + y_n)^{\gamma_n} = \sum_{\alpha + \beta = \gamma} ((\alpha, \beta)) x^{\alpha} y^{\beta}$ (cf. VAR, R, Notations et conventions). Donc:

(8)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{si} \quad |\alpha| + |\beta| = |\gamma| \quad \text{mais} \quad \alpha + \beta \neq \gamma
$$

(9)
$$
c_{\alpha,\beta,\alpha+\beta} = ((\alpha, \beta)).
$$
L’associativité du produit implique la relation
$$
\sum_{\alpha,\xi} c_{\alpha\xi\eta} x^\alpha \left( \sum_{\beta,\gamma} c_{\beta\gamma\xi} y^\beta z^\gamma \right) = \sum_{\xi,\gamma} c_{\xi\gamma\eta} \left( \sum_{\alpha,\beta} c_{\alpha\beta\xi} x^\alpha y^\beta \right) z^\gamma
$$
quels que soient $x, y, z$ assez voisins de 0, d’où
(10)
$$
\sum_\xi c_{\alpha\xi\eta} c_{\beta\gamma\xi} = \sum_\xi c_{\xi\gamma\eta} c_{\alpha\beta\xi} \quad (\alpha, \beta, \gamma, \eta \text{ dans } \mathbf{N}^n).
$$
Le groupuscule G admet un sous-groupuscule ouvert commutatif si et seulement si $c_{\alpha\beta\gamma} = c_{\beta\alpha\gamma}$ quels que soient $\alpha, \beta, \gamma$ dans $\mathbf{N}^n$.

### 2. Crochet dans l’algèbre de Lie

Pour $\alpha \in \mathbf{N}^n$, soit $e_\alpha$ la distribution ponctuelle $\frac{1}{\alpha!} \frac{\partial^\alpha}{\partial x^\alpha}$ à l’origine. En particulier,
$$
e_k = e_{e_k} = \frac{\partial}{\partial x_k}.
$$
Les $e_\alpha$ forment une base de l’espace vectoriel $U(G)$. Si $f$ est une fonction analytique dans un voisinage ouvert de 0 dans G, et si $f(x) = \sum_\alpha \lambda_\alpha x^\alpha$ est son développement en série entière à l’origine, on a
$$
\langle e_\alpha, f \rangle = \lambda_\alpha.
$$
En particulier,
$$
\langle e_\alpha, x^\gamma \rangle = \delta_{\alpha\gamma}.
$$
Donc
$$
\langle e_\alpha * e_\beta, x^\gamma \rangle = \langle e_\alpha \otimes e_\beta, (x.y)^\gamma \rangle \\
= \langle e_\alpha \otimes e_\beta, \sum_{\alpha',\beta'} c_{\alpha'\beta'\gamma} x^{\alpha'} y^{\beta'} \rangle \\
= \sum_{\alpha',\beta'} c_{\alpha'\beta'\gamma} \langle e_\alpha, x^{\alpha'} \rangle \langle e_\beta, y^{\beta'} \rangle = c_{\alpha\beta\gamma},
$$
donc
(11)
$$
e_\alpha * e_\beta = \sum_\gamma c_{\alpha\beta\gamma} e_\gamma.
$$
(La formule (10) exprime alors l’associativité de $U(G)$.)
En particulier, puisque $L(G)$ est stable pour le crochet,
(12)
$$
[e_i, e_j] = \sum_k (c_{ijk} - c_{jik}) e_k,
$$
Les constantes de structure de $L(G)$ relativement à la base $(e_1, \ldots, e_n)$ sont donc les $c_{ijk} - c_{jik}$. Autrement dit, identifiant canoniquement $L(G)$ à $K^n$, on obtient:
(13)
$$
[x, y] = B(x, y) - B(y, x).
$$

**Proposition 1.**

(i) $x^{[-1]} \equiv -x + B(x, x)$ mod deg 3
(ii) $x.y.x^{[-1]} \equiv y + [x, y]$ mod deg 3
(iii) $y^{[-1]}.x.y \equiv x + [x, y]$ mod deg 3
(iv) $x^{[-1]}.y^{[-1]}.x.y \equiv [x, y]$ mod deg 3
(v) $x.y.x^{[-1]}.y^{[-1]} \equiv [x, y]$ mod deg 3.

(Dans (i), $x^{[-1]}$ représente bien entendu le développement en série entière à l’origine de l’application $x \mapsto x^{[-1]}$; les autres formules s’interprètent de manière analogue.)

Soient $g_1$ et $g_2$ les composantes homogènes de degrés 1 et 2 de $x^{[-1]}$. On a
$$
0 = x.x^{[-1]}
$$
$$
\equiv x + g_1(x) + B(x, g_1(x)) \quad \text{mod deg 2} \quad \text{(d’après (6))}
$$
$$
\equiv x + g_1(x) \quad \text{mod deg 2}
$$
donc $g_1(x) = -x$. Ensuite
$$
0 = x.x^{[-1]}
$$
$$
\equiv x + (-x + g_2(x)) + B(x, -x + g_2(x)) \quad \text{mod deg 3}
$$
$$
\equiv g_2(x) - B(x, x) \quad \text{mod deg 3}
$$
donc $g_2(x) = B(x, x)$. Cela prouve (i). En utilisant (i), on a
$$
x.y.x^{[-1]} \equiv (x + y + B(x, y)).(-x + B(x, x)) \quad \text{mod deg 3}
$$
$$
\equiv x + y + B(x, y) + (-x + B(x, x)) + B(x + y, -x) \quad \text{mod deg 3}
$$
$$
\equiv y + B(x, y) - B(y, x) \quad \text{mod deg 3}
$$
$$
\equiv y + [x, y] \quad \text{mod deg 3} \quad \text{(d’après (13))}
$$
d’où (ii). La démonstration de (iii) est analogue. En combinant (i) et (iii), on obtient
$$
x^{[-1]}.y^{[-1]}.x.y \equiv (-x + B(x, x)).(x + [x, y]) \quad \text{mod deg 3}
$$
$$
\equiv -x + B(x, x) + x + [x, y] + B(-x, x) \quad \text{mod deg 3}
$$
$$
\equiv [x, y] \quad \text{mod deg 3}
$$
d’où (iv). La démonstration de (v) est analogue.

### 3. Puissances

Considérons $j$ points de $G$:
$$
x(1) = (x(1)_1, x(1)_2, \ldots, x(1)_n)
$$
$$
x(2) = (x(2)_1, x(2)_2, \ldots, x(2)_n)
$$
$$
\cdots \cdots \cdots \cdots \cdots \cdots \cdots \cdots
$$
$$
x(j) = (x(j)_1, x(j)_2, \ldots, x(j)_n).
$$

L’application $(x(1), x(2), \ldots, x(j)) \mapsto x(1) . x(2) \ldots x(j)$ admet un développement en série entière à l’origine:

$$
(14) \quad x(1) . x(2) \ldots x(j) = \sum_{\alpha(1), \alpha(2), \ldots, \alpha(j) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(j)} x(1)^{\alpha(1)} \ldots x(j)^{\alpha(j)}
$$

où les $a_{\alpha(1), \ldots, \alpha(j)}$ sont des éléments de $\mathbf{K}^n$. Posons, pour $j = 0, 1, 2, \ldots$

$$
(15) \quad \psi_j(x) = \sum_{\alpha(1) \neq 0, \ldots, \alpha(j) \neq 0} a_{\alpha(1), \ldots, \alpha(j)} x^{\alpha(1) + \cdots + \alpha(j)}
$$

où le second membre est une série entière convergente par rapport à la variable $x \in \mathbf{K}^n$. On obtient cette série en supprimant dans (14) les termes dans lesquels l’une des variables $x(1), \ldots, x(j)$ n’intervient pas explicitement, puis en faisant $x(1) = x(2) = \cdots = x(j) = x$.

Si $t \in \mathbf{K}$, toutes les applications puissance $t$-ème de $G$ ont même développement en série entière à l’origine, puisque deux quelconques d’entre elles coïncident dans un voisinage de 0. Nous noterons $x^{[t]}$ ce développement en série entière.

#### Proposition 2 {#lie-iii-s5-prop-2 .statement}

(i) *On a* $\psi_j \equiv 0 \mod \deg j$.
(ii) *Si* $t \in \mathbf{K}$, *on a*

$$
(16) \quad x^{[t]} = \sum_{i=0}^{\infty} \binom{t}{i} \psi_i(x)
$$

*où la série formelle de droite a un sens grâce à* (i).

$
\left( \text{On pose } \binom{t}{i} = \frac{t(t-1)\ldots(t-i+1)}{i!} \text{ pour tout } t \in \mathbf{K}. \right)
$

L’assertion (i) est évidente sur la définition des $\psi_j$.
Prouvons (ii) pour $t$ entier $\geqslant 0$. D’après (14), on a

$$
(17) \quad x^{[t]} = \sum_{\alpha(1), \ldots, \alpha(t) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \cdots + \alpha(t)}
$$

Pour $\alpha = (\alpha(1), \ldots, \alpha(t)) \in (\mathbf{N}^n)^t$, notons $\sigma(\alpha)$ l’ensemble des $j \in \{1, 2, \ldots, t\}$ tels que $\alpha(j) \neq 0$. Si, dans la somme (17), on groupe les termes pour lesquels $\sigma(\alpha)$ est le même, il vient

$$
(18) \quad x^{[t]} = \sum_{\sigma \subset \{1, t\}} h_{t, \sigma}(x)
$$

avec

$$
(19) \quad h_{t, \sigma}(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \cdots + \alpha(t)}
$$

Posons $\sigma = \{j_1, j_2, \ldots, j_q\}$ avec $j_1 < j_2 < \cdots < j_q$. Dans (14) (où l’on remplace $j$ par t), substituons 0 à x(k) pour k ∉ σ ; comme 0 est élément neutre de G, on obtient le développement en série entière à l’origine de x(j₁) . x(j₂) . . . . . x(jₖ) :

$$
x(j₁) . x(j₂) . . . . . x(jₖ) = \sum_{σ(α) ⊂ σ} a_{α(1),...,α(t)} x(j₁)^{α(j₁)} x(j₂)^{α(j₂)} . . . x(jₖ)^{α(jₖ)}
$$

donc, compte tenu de la définition de $ψ_q$:

(20)
$$
ψ_q(x) = \sum_{σ(α) = σ} a_{α(1),...,α(t)} x^{α(j₁)+⋯+α(jₖ)}.
$$

D’après (19) et (20), on voit que $h_{t,σ}(x) = ψ_{card_σ}(x)$. Alors, (18) entraîne

$$
x^{[t]} = \sum_{i=0}^{t} \binom{t}{i} ψ_i(x) = \sum_{i=0}^∞ \binom{t}{i} ψ_i(x).
$$

Cela établi, posons $x^{[t]'} = \sum_{i=0}^∞ \binom{t}{i} ψ_i(x)$ pour tout $t ∈ K$. Dans les séries entières $x^{[t]}$ et $x^{[t]'}$, chaque coefficient est fonction polynomiale de $t$. En effet, cela est évident pour $x^{[t]'}$. En ce qui concerne $x^{[t]}$, il suffit de prouver que, pour tout $u ∈ U(G)$, l’image de $u$ par $x ↦ x^{[t]}$ est fonction polynomiale de $t$. Or, pour $u ∈ U^m(G)$, cette image est $t^m u$ (\S 4, n° 3, prop. 7 (iv)).

Comme $x^{[t]} = x^{[t]'}$ pour $t$ entier $≥ 0$, on conclut de là que $x^{[t]} = x^{[t]'}$ pour tout $t ∈ K$.

#### Remarque 1 {#lie-iii-s5-n3-rem-1 .statement}

Ecrivons la condition (ii) de la prop. 2 pour $t$ entier $≥ 0$:

$$
\begin{align*}
0 &= ψ_0(x) \\
x &= ψ_0(x) + ψ_1(x) \\
x^{[2]} &= ψ_0(x) + 2ψ_1(x) + ψ_2(x) \\
&\cdots \cdots \cdots \cdots \cdots \cdots \cdots
\end{align*}
$$

Ces formules suffisent à déterminer les $ψ_i$.

#### Remarque 2 {#lie-iii-s5-n3-rem-2 .statement}

On voit que $ψ_0(x) = 0$, $ψ_1(x) = x$, $ψ_2(x) = x^{[2]} - 2x$,

$$
x^{[-1]} = \sum_{i=1}^∞ (-1)^i ψ_i(x).
$$

#### Remarque 3 {#lie-iii-s5-n3-rem-3 .statement}

L’expression précédente de $ψ_2$ et la formule (6) prouvent que

(21)
$$
ψ_2(x) ≡ B(x, x) \mod \deg 3.
$$

Compte tenu de la prop. 2, (i) et (ii), on voit que

(22)
$$
x^{[t]} ≡ tx + \binom{t}{2} B(x, x) \mod \deg 3.
$$

#### Remarque 4 {#lie-iii-s5-n3-rem-4 .statement}

Notons $\psi_{p,m}(x)$ et $h_{t,m}(x)$ les composantes homogènes de degré $m$ de $\psi_p(x)$ et de $x^{[t]}$. On a $\psi_{p,m} = 0$ pour $m < p$. D’autre part, la prop. 2 (ii) donne

$$
h_{t,m}(x) = \sum_{p \leq m} \frac{t(t-1)\ldots(t-p+1)}{p!} \psi_{p,m}(x)
$$

c’est-à-dire

$$
h_{t,m}(x) = \sum_{1 \leq r \leq m} t^r \varphi_{r,m}(x)
$$

où les $\varphi_{r,m}$ sont des applications polynomiales homogènes de degré $m$ de $K^n$ dans $K^n$. On a en particulier, d’après (23),

$$
\varphi_{1,m}(x) = \sum_{p \leq m} \frac{(-1)^{p-1}}{p} \psi_{p,m}(x)
$$
$$
\varphi_{m,m}(x) = \frac{1}{m!} \psi_{m,m}(x).
$$

#### Remarque 5 {#lie-iii-s5-n3-rem-5 .statement}

Si $K$ est de caractéristique $> 0$, les résultats des n° 1 et 2 restent valables à condition de définir $e_\alpha$, au n° 2, par $\langle e_\alpha, \sum_\beta \lambda_\beta x^\beta \rangle = \lambda_\alpha$. Au n° 3, si on définit les $\psi_j$ comme ci-dessus, le raisonnement fait prouve encore que $x^{[t]} = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x)$ si $t \in \mathbf{N}$.

### 4. Exponentielle

Soit $E(x)$ le développement en série entière en 0 d’une application exponentielle de G. Soit $L(x)$ le développement en série entière en 0 de l’application réciproque d’une application exponentielle injective de G. Puisque l’application tangente en 0 à toute application exponentielle est l’identité de $L(G)$, on a $E(x) \equiv x \mod \deg 2$ et $L(x) \equiv x \mod \deg 2$. Puisque $E(L(x)) = L(E(x))$ pour $x$ assez voisin de 0, les séries formelles $E$ et $L$ sont telles que $E(L(X)) = L(E(X)) = X$. Un raisonnement analogue montre que $E(tX) = (E(X))^{[t]}$, $L(X^{[t]}) = tL(X)$ pour $t \in K$.

#### Proposition 3 {#lie-iii-s5-prop-3 .statement}

On a

$$
L = \sum_{p=1}^\infty \frac{(-1)^{p-1}}{p} \psi_p
$$
$$
E = \sum_{p=1}^\infty \frac{1}{p!} \psi_{p,p}
$$

(rappelons que $\psi_{p,p}$ est la composante homogène de degré $p$ de $\psi_p$).

On a

$$
E(tx) = (E(x))^{[t]}
$$

ou, d’après (24),

$$
E(tx) = \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^r \varphi_{r,m}(E(x)).
$$

Les deux membres sont des séries formelles en $t$ et $x$. Egalons les termes du premier degré en $t$. Il vient

(29)
$$
x = \sum_{m \geq 0} \varphi_{1,m}(E(x)).
$$

Or l’inversion d’un système de séries formelles, quand elle est possible, ne l’est que d’une seule manière (A, IV, § 6, cor. de la prop. 8). Alors

$$
\begin{align*}
L(x) &= \sum_{m \geq 0} \varphi_{1,m}(x) & \text{d'après (29)} \\
&= \sum_{p,m} \frac{(-1)^p}{p} \psi_{p,m}(x) & \text{d'après (25)} \\
&= \sum_p \frac{(-1)^p}{p} \psi_p(x),
\end{align*}
$$

d’où (i). De même, on a, pour $t \neq 0$,

$$
\begin{align*}
L(tx) &= tL((tx)^{[t^{-1}]}) \\
&= tL\left( \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^{m-r} \varphi_{r,m}(x) \right) & \text{d'après (24).}
\end{align*}
$$

Egalons les termes du premier degré en $t$. Il vient

$$
x = L\left( \sum_{m \geq 0} \varphi_{m,m}(x) \right)
$$

d’où

$$
\begin{align*}
E(x) &= \sum_{m \geq 0} \varphi_{m,m}(x) \\
&= \sum_{m \geq 0} \frac{1}{m!} \psi_{m,m}(x) & \text{d'après (26).}
\end{align*}
$$

#### Proposition 4 {#lie-iii-s5-prop-4 .statement}

*Pour que la carte utilisée de $G$ soit canonique, il faut et il suffit que $\psi_j = 0$ pour $j \geq 2$.*

C’est suffisant d’après la prop. 3. Supposons que la carte soit canonique, et que $\psi_i = 0$ pour $2 \leq i < n$. On a $nx = x^{[n]} = \sum_{i=0}^n \binom{n}{i} \psi_i(x) = nx + \psi_n(x)$, d’où $\psi_n = 0$. Donc $\psi_j = 0$ pour $j \geq 2$ par récurrence sur $j$.

## EXERCICES {#lie-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
