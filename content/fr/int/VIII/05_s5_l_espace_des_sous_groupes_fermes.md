---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 5
section_title: L’espace des sous-groupes fermés
lang: fr
source: int-vii-viii-fr
pdf_pages: 0173-0188, 0205-0206
extraction: ocr
subsections:
    - "no": 1
      title: L’espace des mesures de Haar des sous-groupes fermés de $G$.
      page: 0
      pdf_page: 173
    - "no": 2
      title: Semi-continuité du volume de l’espace homogène.
      page: 0
      pdf_page: 176
    - "no": 3
      title: L’espace des sous-groupes fermés de G.
      page: 0
      pdf_page: 179
    - "no": 4
      title: '*Cas des groupes sans sous-groupes finis arbitrairement petits.*'
      page: 0
      pdf_page: 182
    - "no": 5
      title: '*Cas des groupes commutatifs.*'
      page: 0
      pdf_page: 184
    - "no": 6
      title: Autre interprétation de la topologie de l’espace des sous-groupes fermés.
      page: 0
      pdf_page: 187
statements: 20
exercises: 6
content_sha256: 07508ef75d3b43c6dbeb1fbf97e0fba84cec2d656d0ac9357378c5c64dd9dfa2
---

## § 5. L’espace des sous-groupes fermés.

Dans ce paragraphe, $G$ désigne un groupe localement compact et $\mu$ une mesure de Haar à droite sur $G$.

### 1. L’espace des mesures de Haar des sous-groupes fermés de $G$.

#### Lemme 1 {#int-viii-s5-lem-1 .statement}

Soient $\alpha$ une mesure positive $\neq 0$ sur $G$, S son support ; les deux conditions suivantes sont équivalentes :
a) S est un sous-groupe fermé de $G$ et la mesure induite par $\alpha$ sur S est une mesure de Haar à droite sur S.
b) Pour tout $s \in S$, on a $\delta(s)\alpha = \alpha$.
En outre, lorsque ces conditions sont vérifiées, l’ensemble des $t \in G$ tels que $\delta(t)\alpha = \alpha$ est égal à S.
Il est clair que a) entraîne b) ; inversement, la relation b) entraîne $Sx = S$ pour tout $x \in S$ ; autrement dit les relations $x \in S$ et $y \in S$ entraînent que $y \in Sx$, ou encore $yx^{-1} \in S$, et comme S n’est pas vide, S est un sous-groupe fermé de $G$. L’ensemble des $t \in G$ tels que $St = S$ est alors S lui-même, d’où la dernière assertion.

Dans le reste de ce paragraphe, nous noterons $\Gamma$ l’ensemble des mesures positives $\neq 0$ sur $G$ vérifiant les conditions du lemme 1, et pour tout $\alpha \in \Gamma$, nous noterons $H_\alpha$ le sous-groupe fermé de $G$, support de $\alpha$.

#### Proposition 1 {#int-viii-s5-prop-1 .statement}

L’ensemble $\Gamma$ est fermé dans l’espace $\mathscr{M}_+(G) - \{0\}$, muni de la topologie vague.
Démontrons d’abord les lemmes suivants :

#### Lemme 2 {#int-viii-s5-lem-2 .statement}

Soient X un espace localement compact et pour toute mesure $\alpha \in \mathscr{M}_+(X) - \{0\}$, soit $S_\alpha$ le support de $\alpha$. Soit $\Phi$ un filtre sur $\mathscr{M}_+(X) - \{0\}$ qui converge vaguement vers une mesure $\alpha_0 \neq 0$. Alors, pour tout voisinage V d’un point s du support de $\alpha_0$, il existe un ensemble $M \in \Phi$ tel que, pour toute $\alpha \in M$, on ait $V \cap S_\alpha \neq \varnothing$.

En effet, si $\varphi \in \mathscr{K}_+(X)$ est une fonction de support contenu dans V et telle que $\int \varphi(x) d\alpha_0(x) > 0$, il existe par définition un ensemble $M \in \Phi$ tel que $\int \varphi(x) d\alpha(x) > 0$ pour toute $\alpha \in M$, ce qui entraîne $V \cap S_\alpha \neq \varnothing$.

#### Lemme 3 {#int-viii-s5-lem-3 .statement}

Soient E un ensemble filtré par un filtre $\Phi$, $\xi \to \alpha(\xi)$ une application de E dans $\Gamma$, qui converge vaguement suivant $\Phi$ vers une mesure $\alpha_0 \neq 0$. Soit d’autre part $\xi \to t_\xi$ une application de E dans G telle que, pour tout $\xi \in E$, on ait $t_\xi \in H_{\alpha(\xi)}$. Si s est une valeur d’adhérence de l’application $\xi \to t_\xi$ suivant $\Phi$, on a $\delta(s)\alpha_0 = \alpha_0$.

Remplaçant au besoin $\Phi$ par un filtre plus fin, on peut supposer que s est valeur limite de $\xi \to t_\xi$ suivant $\Phi$; en vertu du lemme 1, on a $\delta(t_\xi)\alpha(\xi) = \alpha(\xi)$ pour tout $\xi \in E$, et la conclusion résulte de la continuité de l’application $(u, \lambda) \to \delta(u)\lambda$ dans $G \times \mathscr{M}_+(G)$ (§ 3, no 3, prop. 13).

Pour prouver la prop. 1, il suffit, en vertu du lemme 1, de montrer que, si un filtre $\Psi$ sur $\Gamma$ converge vaguement vers une mesure $\alpha_0 \neq 0$ et si s appartient au support de $\alpha_0$, on a $\delta(s)\alpha_0 = \alpha_0$. Or, pour tout voisinage V de s dans G, il existe $M \in \Psi$ tel que, pour toute $\alpha \in M$, on ait $V \cap H_\alpha \neq \varnothing$, en vertu du lemme 2. Pour tout voisinage V de s et toute $\alpha \in \Gamma$, soit alors $t_{V,\alpha}$ un point de $V \cap H_\alpha$ si $V \cap H_\alpha \neq \varnothing$, un point quelconque de $H_\alpha$ dans le cas contraire ; si $\Theta$ est le filtre des sections du filtre des voisinages de s, $\Phi$ le filtre produit $\Theta \times \Psi$, s est valeur d’adhérence de $(V, \alpha) \to t_{V,\alpha}$ suivant $\Phi$ d’après ce qui précède. Comme d’autre part l’application $(V, \alpha) \to \alpha$ a pour valeur limite $\alpha_0$ suivant $\Phi$, la proposition résulte du lemme 3.

#### Proposition 2 {#int-viii-s5-prop-2 .statement}

Soit $\varphi$ une fonction de $\mathscr{K}_+(G)$ telle que $\varphi(e) > 0$. Alors l’ensemble $\Gamma_\varphi$ des mesures $\alpha \in \Gamma$ telles que $\int \varphi(x)d\alpha(x) = 1$ est compact pour la topologie vague.

L’ensemble $\Gamma_\varphi$ est l’intersection de $\Gamma$ et de l’hyperplan de $\mathscr{M}(G)$ formé des $\alpha$ telles que $\int \varphi(x)d\alpha(x) = 1$; comme cet hyperplan est vaguement fermé dans $\mathscr{M}(G)$ et ne contient pas 0, il résulte de la prop. 1 que $\Gamma_\varphi$ est vaguement fermé dans $\mathscr{M}(G)$. Il suffit donc de montrer que, pour toute partie compacte K de G, on a $\sup_{\alpha \in \Gamma_\varphi} \alpha(K) < +\infty$ (chap. III, § 2, n° 7, prop. 9).

Or, soit U le voisinage ouvert de e dans G défini par l’inégalité $\varphi(x) > \varphi(e)/2$; comme $1 = \int \varphi(x)d\alpha(x) \geq \int_U \varphi(x)d\alpha(x)$ pour $\alpha \in \Gamma_\varphi$, on voit que, si l’on pose $c = 2/\varphi(e)$, on a $\alpha(U) \leq c$ pour toute $\alpha \in \Gamma_\varphi$. Soit V un voisinage ouvert symétrique de e dans G tel que $V^2 \subset U$; montrons que l’on a $\alpha(Vx) \leq c$ pour tout $x \in G$ et toute $\alpha \in \Gamma_\varphi$. En effet, cette relation est triviale si $Vx$ ne rencontre pas le support $H_\alpha$ de $\alpha$; si par contre il existe un $h \in Vx \cap H_\alpha$, on a $h = vx$ pour un $v \in V$, d’où

$$
Vx = Vv^{-1}h \subset V^2h \subset Uh,
$$

et comme $\delta(h)\alpha = \alpha$, il vient $\alpha(Vx) \leq \alpha(Uh) = \alpha(U) \leq c$. Soit alors $(x_i)_{1 \leq i \leq n}$ une suite de points de K telle que les $Vx_i$ forment un recouvrement de K ; il résulte de ce qui précède que $\alpha(K) \leq \sum_{i=1}^n \alpha(Vx_i) \leq nc$ pour toute $\alpha \in \Gamma_\varphi$; C.Q.F.D.

#### Proposition 3 {#int-viii-s5-prop-3 .statement}

Sous les hypothèses de la prop. 2, l’application $\alpha \to \left( \langle \varphi, \alpha \rangle, \frac{\alpha}{\langle \varphi, \alpha \rangle} \right)$ est un homéomorphisme de $\Gamma$ sur l’espace produit $\mathbf{R}_+^* \times \Gamma_\varphi$.

Comme l’application $\alpha \to \langle \varphi, \alpha \rangle$ est vaguement continue, il suffit de remarquer que l’on a $\langle \varphi, \alpha \rangle \neq 0$ pour toute mesure $\alpha \in \Gamma$, puisque e appartient au support $H_\alpha$ de $\alpha$ et que $\varphi(e) > 0$.

### 2. Semi-continuité du volume de l’espace homogène.

Dans ce n°, pour toute mesure $\alpha \in \Gamma$, nous poserons

(1)
$$
Q_\alpha = G / H_\alpha,
$$
et nous désignerons par $\pi_\alpha$ l’application canonique $G \to Q_\alpha$.

Soit $\Gamma^0$ le sous-ensemble de $\Gamma$ formé des mesures $\alpha$ telles que le sous-groupe $H_\alpha$ de $G$ soit unimodulaire ; les éléments de $\Gamma^0$ sont caractérisés par le fait que l’on a $\alpha(f) = \alpha(\tilde{f})$ pour toute fonction $f \in \mathscr{K}(G)$ (toute fonction de $\mathscr{K}(H_\alpha)$ se prolongeant en une fonction de $\mathscr{K}(G)$ en vertu du th. d’Urysohn) ; on en conclut que $\Gamma^0$ est une partie fermée de $\Gamma$. Pour toute $\alpha \in \Gamma^0$, rappelons que sur $Q_\alpha$ la mesure quotient $\mu_\alpha = \mu / \alpha$ est définie et relativement invariante par $G$ (chap. VII, § 2, n° 6, th. 3) ; rappelons aussi que pour toute fonction $f \in \mathscr{K}(G)$, on a

(2)
$$
\int_G f(x) d\mu(x) = \int_{Q_\alpha} d\mu_\alpha(\dot{x}) \int_{H_\alpha} f(xs) d\alpha(s)
$$
où $\dot{x} = \pi_\alpha(x)$ est l’image canonique de $x \in G$ dans $Q_\alpha$.

#### Proposition 4 {#int-viii-s5-prop-4 .statement}

Soit $\Gamma^0$ l’ensemble des mesures $\alpha \in \Gamma$ telles que $H_\alpha$ soit unimodulaire, et pour toute $\alpha \in \Gamma^0$, posons $\mu_\alpha = \mu / \alpha$; alors l’application $\alpha \to \| \mu_\alpha \|$ de $\Gamma^0$ dans $\overline{\mathbf{R}}$ est semi-continue inférieurement pour la topologie vague.

Pour toute $\alpha \in \Gamma^0$ et toute fonction $f \in \mathscr{K}(G)$, posons

$$
f_\alpha(\dot{x}) = \int_{H_\alpha} f(xs) d\alpha(s) = (f * \alpha)(x)
$$
où le produit de convolution est pris relativement à la mesure de Haar à droite $\mu$ et où l’on utilise le fait que $\tilde{\alpha} = \alpha$ (§ 4, n° 4, formule (11)). On sait (chap. VII, § 2, n° 1, prop. 2), que l’application $f \to f_\alpha$ de $\mathscr{K}_+(G)$ dans $\mathscr{K}_+(Q_\alpha)$ est surjective ; on a donc, en vertu de (2),

$$
\| \mu_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu_\alpha(f_\alpha) / \| f_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu(f) / \| f_\alpha \|
$$

où l’on pose

(3) $\|f_\alpha\| = \sup_{\dot{x} \in Q_\alpha} |f_\alpha(\dot{x})| = \sup_{x \in G} |(f * \alpha)(x)|.$

Pour établir la proposition, il suffira de montrer que, pour $f \in \mathscr{H}_+(G)$ donnée, l’application $\alpha \to \|f_\alpha\|$ est vaguement continue. Or, soit K le support de $f$; la fonction $f * \alpha$ a son support contenu dans $KH_\alpha$ et est invariante à droite par $H_\alpha$; par suite

$$ \|f_\alpha\| = \sup_{x \in K} |(f * \alpha)(x)|. $$

La conclusion résulte donc de ce que l’application $\alpha \to f * \alpha$ de $\mathscr{M}_+(G)$ muni de la topologie vague, dans $\mathscr{C}(G)$, muni de la topologie de la convergence compacte, est continue (§ 4, n° 2, Remarque 1).

Rappelons que si, pour une mesure $\alpha \in \Gamma^0$, $\|\mu_\alpha\|$ est finie, G est nécessairement unimodulaire (chap. VII, § 2, n° 6, cor. 3 du th. 3).

#### Proposition 5 {#int-viii-s5-prop-5 .statement}

Soit $g$ une fonction numérique positive $\mu$-intégrable et soit $\Gamma^0(g)$ l’ensemble des mesures $\alpha \in \Gamma^0$ telles que l’on ait $\int^* g(xs)d\alpha(s) \geq 1$ pour tout $x \in G$. Alors l’application $\alpha \to \|\mu_\alpha\|$ de $\Gamma^0(g)$ dans $\overline{\mathbf{R}}$ est vaguement continue.

Pour toute mesure $\alpha \in \Gamma^0(g)$, rappelons (chap. VII, § 2, n° 3, prop. 5) que la fonction

$$ g_\alpha(\dot{x}) = \int_{H_\alpha} g(xs)d\alpha(s) $$

est définie $\mu_\alpha$-presque partout sur $Q_\alpha$, est $\mu_\alpha$-intégrable, et que l’on a

(4) $\int_G g(x)d\mu(x) = \int_{Q_\alpha} g_\alpha(\dot{x})d\mu_\alpha(\dot{x}).$

En vertu de la prop. 4, il suffit de démontrer que, dans $\Gamma^0(g)$, $\alpha \to \|\mu_\alpha\|$ est semi-continue supérieurement. Une mesure $\alpha \in \Gamma^0(g)$ étant fixée, soit K une partie compacte de G. Il existe sur $Q_\alpha$ une fonction continue à support compact, prenant ses valeurs dans $(0, 1)$, égale à 1 dans l’ensemble compact $\pi_\alpha(K)$; comme l’application $f \to f_\alpha$ de $\mathscr{K}_+(G)$ dans $\mathscr{K}_+(Q_\alpha)$ est surjective (chap. VII, § 2, no 1, prop. 2), on voit qu’il existe une fonction $f \in \mathscr{K}_+(G)$ telle que l’on ait

$$
(f * \alpha)(x) = \int_G f(xs)d\alpha(s)
$$
$$
\begin{cases}
\leq 1 \text{ pour tout } x \in G \\
= 1 \text{ pour tout } x \in K.
\end{cases}
$$

Comme $\beta \to f * \beta$ est une application continue de $\mathscr{M}_+(G)$, muni de la topologie vague, dans $\mathscr{C}(G)$ muni de la topologie de la convergence compacte ($§ 4$, no 2, Remarque 1), on voit que, pour tout $\varepsilon > 0$, l’ensemble $U_\varepsilon$ des $\beta \in \Gamma^0(g)$ telles que l’on ait

$$
f_\beta(\dot{x}) = \int_G f(xs)d\beta(s) > 1 - \varepsilon \text{ pour tout } x \in K
$$

est un voisinage ouvert de $\alpha$ dans $\Gamma^0(g)$; pour toute $\beta \in U_\varepsilon$, on a alors en vertu de la formule (2)

$$
(5) \quad \| \mu_\alpha \| \geq \int_G f(x)d\mu(x) = \int_{Q_\beta} f_\beta(\dot{x})d\mu_\beta(\dot{x}) \geq (1 - \varepsilon)\mu_\beta(\pi_\beta(K)).
$$

Le nombre $\varepsilon > 0$ étant donné, choisissons une fonction $h \in \mathscr{K}_+(G)$ telle que $\int_G |g(x) - h(x)|d\mu(x) \leq \varepsilon$, et prenons dans ce qui précède $K = \operatorname{Supp}(h)$. Pour tout $\beta \in \Gamma^0(g)$, on a par hypothèse $g_\beta(\dot{x}) \geq 1$ presque partout (pour $\mu_\beta$) dans $Q_\beta$, donc

$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{Q_\beta - \pi_\beta(K)} g_\beta(\dot{x})d\mu_\beta(\dot{x}) = \int_{G - KH_\beta} g(x)d\mu(x)
$$

en vertu de (4); comme $h$ est nulle en dehors de $K$, et $a$ fortiori en dehors de $KH_\beta$, il vient

$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{G - KH_\beta} |g(x) - h(x)|d\mu(x)
$$
$$
\leq \int_G |g(x) - h(x)|d\mu(x) \leq \varepsilon;
$$

en combinant ce résultat avec (5), on voit que l’on a

$$
\|\mu_\beta\| \leq \varepsilon + \|\mu_\alpha\|/(1 - \varepsilon)
$$

dès que $\beta \in U_\varepsilon$, ce qui termine la démonstration.

#### Corollaire 1 {#int-viii-s5-prop-5-cor-1 .statement}

*Soient K une partie compacte de G, V un voisinage compact symétrique de e dans G, c un nombre réel > 0. La restriction de l’application $\alpha \to \|\mu_\alpha\|$ à l’ensemble des $\alpha \in \Gamma^0$ telles que l’on ait $G = KH_\alpha$ et $\alpha(V) \geq c$ est vaguement continue.*

En effet, soit $g \in \mathscr{K}_+(G)$ une fonction telle que $g(x) \geq 1/c$ pour $x \in KV$. Pour tout $x \in K$, on a

$$
\int g(xs)d\alpha(s) \geq \int_V g(xs)d\alpha(s) \geq 1
$$

$\alpha$ vérifiant les conditions de l’énoncé ; comme en outre $\pi_\alpha(K) = Q_x$ on a $\alpha \in \Gamma^0(g)$, d’où le corollaire.

#### Corollaire 2 {#int-viii-s5-prop-5-cor-2 .statement}

*Soit A une partie $\mu$-intégrable de G. La restriction de l’application $\alpha \to \|\mu_\alpha\|$ à l’ensemble $N_A$ des mesures de Haar normalisées des sous-groupes discrets H de G tels que $G = AH$ est vaguement continue.*

En effet, pour $a \in A$ et $\alpha \in N_A$, on a

$$
\int \varphi_A(as)d\alpha(s) \geq \varphi_A(a) = 1,
$$

et comme $\pi_\alpha(A) = Q_\alpha$, on a $N_A \subset \Gamma^0(\varphi_A)$, et le corollaire résulte donc de la prop. 5.

### 3. L’espace des sous-groupes fermés de G.

Désignons par $\Sigma$ l’ensemble des sous-groupes fermés de G ; si l’on associe à chaque mesure $\alpha \in \Gamma$ le sous-groupe $H_\alpha$ support de $\alpha$, on obtient une application (dite canonique) de $\Gamma$ dans $\Sigma$, qui est évidemment surjective et permet d’identifier canoniquement $\Sigma$ à l’ensemble des orbites du groupe des homothéties de rapport $> 0$ dans $\Gamma$. L’ensemble $\Sigma$, muni de la topologie quotient de la topologie vague sur $\Gamma$, est appelé l’espace des sous-groupes fermés de $G$.

#### Théorème 1 {#int-viii-s5-thm-1 .statement}

Soit $G$ un groupe localement compact. L’espace $\Sigma$ des sous-groupes fermés de $G$ est compact. On a en outre les propriétés suivantes :

(i) L’ensemble $\Sigma^0$ des sous-groupes fermés unimodulaires de $G$ est fermé dans $\Sigma$ (donc compact).

(ii) Si $G$ est engendré par un voisinage compact de $e$, l’ensemble $\Sigma_c^0$ des sous-groupes fermés unimodulaires $H$ de $G$ tels que l’espace quotient $G/H$ soit compact, est ouvert dans $\Sigma^0$ (donc localement compact).

(iii) Pour tout voisinage ouvert relativement compact $U$ de $e$ dans $G$, l’ensemble $D_U$ des sous-groupes discrets $H$ de $G$ tels que $H \cap U = \{e\}$ est fermé dans $\Gamma^0$ (donc compact).

Il résulte de la prop. 3 du no 1 que $\Sigma$ est homéomorphe à $\Gamma_\varphi$, donc compact en vertu de la prop. 2 du no 1. On a noté en outre au début du no 2 que l’ensemble $\Gamma^0$ des mesures $\alpha \in \Gamma$ telles que $H_\alpha$ soit unimodulaire est fermé dans $\Gamma$; comme $\Gamma^0$ est stable par les homothéties de rapport $> 0$, l’image $\Sigma^0$ de $\Gamma^0$ dans $\Sigma$ est une partie fermée de $\Sigma$, ce qui prouve (i).

La propriété (ii) sera conséquence de la proposition suivante :

#### Proposition 6 {#int-viii-s5-prop-6 .statement}

Supposons que le groupe localement compact $G$ soit engendré par un voisinage compact de $e$. Alors l’ensemble $\Gamma_c^0$ des mesures $\alpha \in \Gamma^0$ telles que $G/H_\alpha$ soit compact est ouvert dans $\Gamma^0$, et la restriction à $\Gamma_c^0$ de l’application $\alpha \to \| \mu_\alpha \|$ est vaguement continue.

Avec les notations de la prop. 5 du no 2, on a, pour $g \in \mathscr{K}_+(G)$

$$
\Gamma^0(g) \subset \Gamma_c^0.
$$

En effet, si $K$ est le support de $g$, la relation $\int g(xs)d\alpha(s) \geqslant 1$ pour tout $x \in G$ entraîne $KH_\alpha = G$, l’intégrale étant évidemment nulle dans le complémentaire de $KH_\alpha$, donc $G/H_\alpha = \pi_\alpha(K)$ est compact. Etant donnée une mesure $\alpha \in \Gamma_c^0$, il suffira donc de définir une fonction $g \in \mathscr{K}_+(G)$ telle que $\Gamma^0(g)$ soit un voisinage de $\alpha$ dans $\Gamma^0$. Puisque $G/H_\alpha$ est compact et que l’application canonique $f \to f_\alpha$ de $\mathscr{K}_+(G)$ dans $\mathscr{K}_+(G/H_\alpha)$ est surjective (chap. VII, § 2, n° 2, Remarque), il existe une fonction $g \in \mathscr{K}_+(G)$ telle que $\int g(xs)d\alpha(s) = 2$ pour tout $x \in G$. Soient K le support (compact) de $g$, L un voisinage compact symétrique de e dans G engendrant G ; l’application $\beta \to g * \beta$ de $\mathscr{M}_+(G)$ dans $\mathscr{C}(G)$ étant vaguement continue ($§ 4$, n° 2, Remarque 1), il existe un voisinage W de $\alpha$ dans $\Gamma^0$ tel que l’on ait

$$
(g * \beta)(x) = \int g(xs)d\beta(s) \geqslant 1
$$

pour toute $\beta \in W$ et tout $x \in LK$. Le premier membre de (7) étant nul en dehors de $KH_\beta$, la relation $\beta \in W$ implique

$$
LK \subset KH_\beta,
$$

d’où l’on déduit, par récurrence sur $n$, $L^nK \subset KH_\beta$ pour tout entier $n > 0$; comme L engendre G, on a donc $G = KH_\beta$ pour toute mesure $\beta \in W$, ce qui prouve que $W \subset \Gamma_c^0$. D’autre part, le premier membre de (7) étant invariant à droite par $H_\beta$, l’inégalité (7) est aussi valable pour $x \in LKH_\beta = G$; donc $W \subset \Gamma^0(g)$, ce qui démontre la proposition.

Enfin, (iii) sera conséquence de la proposition suivante :

#### Proposition 7 {#int-viii-s5-prop-7 .statement}

*Soit N $\subset \Gamma^0$ le sous-espace des mesures de Haar normalisées des sous-groupes discrets de G, et pour tout voisinage ouvert relativement compact U de e dans G, soit $N_U$ la partie de N formée des $\alpha$ telles que $H_\alpha \cap U = \{e\}$. Alors :
a) $N_U$ est compact.
b) Les intérieurs des ensembles $N_U$ dans N forment un recouvrement de N, lorsque U parcourt l’ensemble des voisinages ouverts relativement compacts de e dans G.
c) Pour qu’une partie M de N soit relativement compacte dans N, il faut et il suffit qu’il existe un voisinage ouvert relativement compact U de e dans G tel que $M \subset N_U$.*

Comme $D_U$ est l’image de $N_U$ par l’application continue canonique $\Gamma \to \Sigma$, l’assertion (iii) du th. 1 résultera aussitôt de la prop. 7, $a$.

Pour démontrer la prop. 7, notons que $N_U$ peut être définie comme la partie de $\Gamma^0$ formée des $\alpha$ telles que l’on ait à la fois
$$
\alpha(\{e\}) \geqslant 1 \quad \text{et} \quad \alpha(U) \leqslant 1.
$$
Or, si $A$ est compact (resp. ouvert relativement compact) dans $G$, l’application $\alpha \to \alpha(A)$ de $\mathscr{M}_+(G)$ dans $\mathbf{R}$ est semi-continue supérieurement (resp. inférieurement) pour la topologie vague (chap. IV, § 1, no 1, prop. 4 et § 4, no 4, Remarque) ; on voit donc que $N_U$ est une partie fermée de $\Gamma^0$. De plus, soit $\varphi \in \mathscr{K}_+(G)$ une fonction telle que $\varphi(e) = 1$ et $\varphi(x) = 0$ dans $G - U$; il est clair que $\int \varphi(x) d\alpha(x) = 1$ pour toute $\alpha \in N_U$; la prop. 2 du no 1 montre donc que $N_U$ est un ensemble compact, ce qui démontre a). Soit d’autre part $V$ un voisinage ouvert relativement compact de $e$ dans $G$ tel que $\overline{V} \subset U$, et soit $\varphi \in \mathscr{K}_+(G)$, de support contenu dans $U$ et telle que $\varphi(x) = 1$ dans $V$. On a $\alpha(\varphi) = 1$ pour $\alpha \in N_U$, et il existe donc un voisinage $W$ de $\alpha$ dans $N$ tel que l’on ait $\beta(\varphi) < 2$ pour $\beta \in W$; il est clair alors que l’on a $W \subset N_V$, donc $N_V$ est un voisinage de $N_U$. Comme les $N_U$ recouvrent $N$, cela démontre b). Enfin, toute partie compacte $M$ de $N$ est contenue dans une réunion finie d’ensembles $N_{U_i}$ ($1 \leqslant i \leqslant n$) et comme $\bigcup_i N_{U_i} \subset N_U$, où $U = \bigcap_i U_i$, cela démontre c).

#### Corollaire {#int-viii-s5-n3-cor-1 .statement}

*Le sous-espace* $N$ *de* $\Gamma^0$ *est localement compact*.

### 4. *Cas des groupes sans sous-groupes finis arbitrairement petits.*

#### Théorème 2 {#int-viii-s5-thm-2 .statement}

*Soit* $G$ *un groupe localement compact vérifiant la condition suivante :*

(L) Il existe un voisinage de e dans G qui ne contient aucun sous-groupe fini de G non réduit à e.
Alors on a les propriétés suivantes :
(i) L’ensemble D des sous-groupes discrets de G est localement fermé dans Σ (ce qui équivaut à dire qu’il est localement compact).
(ii) Pour qu’une partie fermée A de D soit compacte, il faut et il suffit qu’il existe un voisinage U de e dans G tel que H ∩ U = {e} pour tout sous-groupe H ∈ A.
(iii) Si en outre G est engendré par un voisinage compact de e, l’ensemble D_c des sous-groupes discrets H de G tels que G/H soit compact est localement fermé dans Σ (donc localement compact).
On a D_c = D ∩ Σ_c^0, donc (iii) est conséquence de (i) et du th. 1, (ii) du n° 3.
Avec les notations du n° 3, prop. 7, il suffit, pour démontrer (i) et (ii), de prouver que :

#### Proposition 8 {#int-viii-s5-prop-8 .statement}

La bijection canonique de N sur D est un homéomorphisme.
Or, si Γ_d est l’ensemble des mesures de Haar sur les sous-groupes discrets de G, D est canoniquement homéomorphe à l’espace des orbites du groupe des homothéties de rapport > 0 dans Γ_d (Top. gén., chap. I, 3e éd., § 5, n° 2, prop. 4). Il suffira donc de prouver que l’application canonique α → (α({e}), α/α({e})) de Γ_d sur ℝ_+^* × N est un homéomorphisme, ce qui résultera du lemme suivant :

#### Lemme 4 {#int-viii-s5-lem-4 .statement}

Si le groupe G vérifie la condition (L), l’application α → α({e}) de Γ_d dans ℝ_+^* est vaguement continue.
Considérons une mesure α ∈ Γ_d ; soit V_0 un voisinage ouvert relativement compact de e dans G tel que H_α ∩ V_0 = {e} et qu’il n’existe aucun sous-groupe fini de G contenu dans V_0 et non réduit à e. Soit V un voisinage compact symétrique de e tel que V^3 ⊂ V_0, et soit U un voisinage symétrique de e tel que U^2 ⊂ V. Soit φ (resp. ψ) une fonction de 𝒦_+(G), à valeurs dans [0, 1], égale à 1 dans V^3 (resp. au point e) et de support contenu dans V_0 (resp. dans U). L’ensemble des mesures β ∈ Γ_d telles que l’on ait $|\beta(\varphi) - \alpha(\varphi)| \leq \varepsilon$ et $|\beta(\psi) - \alpha(\psi)| \leq \varepsilon$ est un voisinage W de $\alpha$. Nous nous proposons de montrer que, pourvu que $\varepsilon$ soit pris assez petit, *on a* $H_\beta \cap V = \{e\}$ *pour toute* $\beta \in W$; il en résultera que $\beta(\psi) = \beta(\{e\})$, donc que $|\beta(\{e\}) - \alpha(\{e\})| \leq \varepsilon$, ce qui prouvera le lemme.

Il nous suffira de montrer que l’on a, pour $\beta \in W$,

(8)
$$(V^2 - V) \cap H_\beta = \varnothing.$$

Supposons en effet ce point établi : alors, pour $x$ et $y$ dans $V \cap H_\beta$, on a $xy^{-1} \in V^2 \cap H_\beta$; mais, en vertu de (8), cela entraîne $xy^{-1} \in V \cap H_\beta$; autrement dit, $V \cap H_\beta$ est un *sous-groupe* de G, qui est évidemment discret et compact, donc fini ; mais en vertu du choix de $V_0$, cela entraîne bien $V \cap H_\beta = \{e\}$.

Raisonnons par l’absurde et supposons donc qu’il existe un point $z$ de $V^2 - V$ appartenant à $H_\beta$; en vertu du choix de U et V, on a $\psi(sz^{-1}) + \psi(s) \leq \varphi(s)$ dans G, la relation $z \notin U^2$ entraînant $Uz \cap U = \varnothing$. Comme
$$
\int \psi(sz^{-1}) d\beta(s) = \int \psi(s) d\beta(s),
$$
on en déduit $2\beta(\psi) \leq \beta(\varphi) \leq \alpha(\varphi) + \varepsilon$; mais on a aussi
$$
\beta(\psi) \geq \alpha(\psi) - \varepsilon,
$$
et par construction $\alpha(\varphi) = \alpha(\psi) = \alpha(\{e\})$. On arrive ainsi à une contradiction dès que $\varepsilon < \alpha(\{e\})/3$. C.Q.F.D.

En termes imagés, on dit qu’un groupe G vérifiant la condition (L) *n’a pas de sous-groupes finis arbitrairement petits.* *On peut montrer que tout groupe de Lie vérifie la condition (L)*; mais cette condition n’est pas caractéristique des groupes de Lie; par exemple le groupe multiplicatif des entiers $p$-adiques congrus à 1 mod. $p$ satisfait à (L).

### 5. *Cas des groupes commutatifs.*

Soient G un groupe localement compact, $N \subset \Gamma^0$ le sous-espace des mesures de Haar normalisées des sous-groupes discrets de G, et N_c la partie de N correspondant aux sous-groupes discrets H de G tels que G/H soit compact ; on a donc N_c = N ∩ Γ^0_c avec les notations du n° 3, prop. 6 ; et si le groupe G est engendré par un voisinage compact de e, il résulte du n° 3, prop. 6 que N_c est ouvert dans N (donc localement compact en vertu du n° 3, cor. de la prop. 7) et que la restriction à N_c de l’application α → ||μ_α|| est vaguement continue.

#### Proposition 9 {#int-viii-s5-prop-9 .statement}

Soit G un groupe localement compact commutatif, engendré par un voisinage compact de e. Pour qu’une partie A de N_c soit relativement compacte dans N_c, il faut et il suffit qu’elle vérifie les deux conditions suivantes :

(i) Il existe un voisinage ouvert U de e dans G tel que H_α ∩ U = {e} pour toute α ∈ A.

(ii) Il existe une constante k telle que μ_α(G/H_α) ≤ k pour toute α ∈ A.

Si A ⊂ N_c est relativement compacte dans N_c, elle l’est a fortiori dans N et la nécessité des conditions (i) et (ii) résulte donc du n° 3, prop. 6 et 7 (sans supposer G commutatif). Réciproquement, supposons que A ⊂ N_c vérifie ces conditions ; si A est l’adhérence de A dans N, Ā est compacte en vertu du n° 3, prop. 7 ; en outre, comme α → ||μ_α|| est semi-continue inférieurement dans Γ^0 pour la topologie vague (n° 2, prop. 4), la condition (ii) implique que l’on a aussi ||μ_α|| ≤ k pour toute α ∈ Ā. Or, puisque G est commutatif, μ_α = μ/α est une mesure de Haar sur le groupe G/H_α, et G/H_α est donc compact pour toute α ∈ Ā (chap. VII, § 1, n° 2, prop. 2). Cela signifie que Ā ⊂ N_c, donc A est relativement compacte dans N_c.

#### Corollaire {#int-viii-s5-n5-cor-1 .statement}

Soit G un groupe localement compact commutatif, engendré par un voisinage compact de e et satisfaisant à la condition (L) du n° 4. Soit D_c l’ensemble des sous-groupes discrets H de G tels que G/H soit compact, et, pour tout H ∈ D_c, soit v(H) la masse totale μ_α(G/H), où μ_α est la mesure quotient de μ par la mesure de Haar normalisée α de H. Pour qu’une partie A de l’espace D_c soit relativement compacte dans D_c, il faut et il suffit qu’elle vérifie les deux conditions suivantes :

(i) Il existe un voisinage ouvert U de e dans G tel que H ∩ U = {e} pour tout H ∈ A.

(ii) Il existe une constante k telle que v(H) ≤ k pour tout H ∈ A.

Compte tenu de la prop. 9, cela résulte aussitôt de ce que D_c est l’image de N_c par la bijection canonique de N sur D, et de ce que, moyennant les hypothèses faites, cette bijection est un homéomorphisme (n° 4, prop. 8).

#### Exemple {#int-viii-s5-n5-exa-1 .statement}

Prenons G = \mathbf{R}^n et pour μ la mesure de Lebesgue ; toutes les hypothèses du cor. de la prop. 9 sont vérifiées. Les sous-groupes discrets H de G tels que G/H soit compact ne sont autres que les sous-groupes discrets de rang n (Top. gén., chap. VII, § 1, n° 1, th. 1) ; un tel sous-groupe H est engendré par une base (a_i)_{1 \leq i \leq n} de \mathbf{R}^n, et on a

$$
v(H) = |\det(a_1, \ldots, a_n)|
$$

(le déterminant étant pris par rapport à la base canonique de \mathbf{R}^n) (chap. VII, § 2, n° 10, th. 4). L’espace D_c peut ici s’interpréter de la façon suivante : tout sous-groupe H ∈ D_c est le transformé g. \mathbf{Z}^n du sous-groupe \mathbf{Z}^n par un élément g ∈ \mathbf{GL}(n, \mathbf{R}) et le sous-groupe de \mathbf{GL}(n, \mathbf{R}) laissant stable \mathbf{Z}^n s’identifie à \mathbf{GL}(n, \mathbf{Z}). Par suite D_c s’identifie canoniquement, en tant qu’espace homogène (non topologique), à \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}). D’autre part, \mathbf{GL}(n, \mathbf{R}) opère continûment dans \mathbf{R}^n, donc aussi dans \mathscr{M}_+(\mathbf{R}^n) pour la topologie vague (§ 3, n° 3, prop. 13), et par suite dans le sous-espace N_c de \mathscr{M}_+(\mathbf{R}^n) ; en outre, l’homéomorphisme canonique (n° 4, prop. 8) de N_c sur D_c est compatible avec les lois d’opération de \mathbf{GL}(n, \mathbf{R}). Comme \mathbf{GL}(n, \mathbf{R}) est dénombrable à l’infini et que D_c est localement compact, la bijection de \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}) sur D_c définie plus haut est un homéomorphisme (chap. VII, App. I, lemme 2). Le cor. de la prop. 9 donne donc un critère de compacité dans l’espace homogène \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}).

### 6. Autre interprétation de la topologie de l’espace des sous-groupes fermés.

Soit $\mathfrak{F}$ l’ensemble des parties fermées de $G$; on définit sur $\mathfrak{F}$ une structure uniforme séparée de la façon suivante : pour toute partie compacte $K$ de $G$ et tout voisinage $V$ de $e$ dans $G$, soit $P(K, V)$ l’ensemble des couples $(X, Y)$ d’éléments de $\mathfrak{F}$ tels que l’on ait à la fois

$$
X \cap K \subset VY \quad \text{et} \quad Y \cap K \subset VX.
$$

Montrons que l’ensemble des $P(K, V)$ est un système fondamental d’entourages d’une structure uniforme séparée $\mathscr{U}$ sur $\mathfrak{F}$. Les axiomes $(U'_I)$ et $(U'_{II})$ de Top. gén., chap. II, 3e éd., § 1, no 1 sont évidemment satisfaits ; en outre les relations $K \subset K'$ et $V' \subset V$ entraînent $P(K', V') \subset P(K, V)$; pour vérifier $(U'_{III})$, on peut donc se borner au cas où $V$ est un voisinage compact symétrique de $e$, de sorte que $VK$ est compact. Supposons que l’on ait $(X, Y) \in P(VK, V)$ et $(Y, Z) \in P(VK, V)$; on a alors $X \cap K \subset X \cap VK \subset VY$, et si $y \in Y$ est tel que $vy \in K$ pour un $v \in V$, on a nécessairement $y \in VK$, donc

$$
X \cap K \subset V(Y \cap VK);
$$

d’autre part on a $Y \cap VK \subset VZ$, d’où $X \cap K \subset V^2Z$ et on montre de même que $Z \cap K \subset V^2X$, ce qui prouve $(U'_{III})$. Enfin, si $X, Y$ sont deux éléments distincts de $\mathfrak{F}$, il existe par exemple un point $a \in X$ tel que $a \notin Y$, donc un voisinage compact symétrique $V$ de $e$ tel que $Va \cap Y = \varnothing$, ou encore $a \notin VY$; $a$ fortiori on a $(X, Y) \notin P(Va, V)$, ce qui achève de prouver notre assertion.

Cela étant, considérons sur l’ensemble $\Sigma$ des sous-groupes fermés de $G$ la topologie $\mathscr{T}$ induite par la topologie de l’espace uniforme $\mathfrak{F}$ que nous venons de définir. Nous allons voir que cette topologie est identique à la topologie définie au no 3. Il suffira de prouver que l’application $\alpha \to H_\alpha$ de $\Gamma$ dans $\Sigma$, quand on munit $\Sigma$ de la topologie $\mathscr{T}$, est continue : en effet, il en sera de même de la restriction de cette application à $\Gamma_\varphi$ (avec les notations du no 1, prop. 2) qui est bijective ; mais comme $\Gamma_\varphi$ est compact et la topologie $\mathscr{T}$ séparée, l’application $\alpha \to H_\alpha$ de $\Gamma_\varphi$ dans $\Sigma$ sera alors un homéomorphisme.

Soient donc $\alpha_0$ un point de $\Gamma$ et $\Phi$ un filtre sur $\Gamma$ qui converge vers $\alpha_0$ ; il s’agit de montrer que, suivant $\Phi$, $H_\alpha$ tend vers $H_{\alpha_0}$ pour la topologie $\mathscr{T}$. Soient $K$ une partie compacte de $G$, $V$ un voisinage compact symétrique de $e$ dans $G$ ; pour tout $x \in H_{\alpha_0} \cap K$, il existe un ensemble $M(x) \in \Phi$ tel que pour toute $\alpha \in M(x)$, on ait $Vx \cap H_\alpha \neq \emptyset$ (no 1, lemme 2), d’où $Vx \subset V^2H_\alpha$ ; recouvrant $H_{\alpha_0} \cap K$ par un nombre fini d’ensembles $Vx_i$, on voit que si $M = \bigcap_i M(x_i)$, on a $H_{\alpha_0} \cap K \subset V^2H_\alpha$ pour toute $\alpha \in M$. Inversement, supposons qu’il y ait un voisinage ouvert $U$ de $e$ dans $G$, tel que pour tout ensemble $L \in \Phi$, il y ait au moins un $\alpha \in L$ pour lequel $H_\alpha \cap K \not\subset UH_{\alpha_0}$ ; si $\omega(L)$ est l’ensemble des $\alpha \in L$ ayant cette propriété, les $\omega(L)$ formeraient la base d’un filtre $\Phi'$ plus fin que $\Phi$ sur $\Gamma$ et, pour toute $\alpha$ appartenant à la réunion $E$ des $\omega(L)$ pour $L \in \Phi$, il existerait un $t_\alpha \in H_\alpha \cap K$ n’appartenant pas à $UH_{\alpha_0}$ ; pour $\alpha \notin E$, on prend pour $t_\alpha$ un point quelconque de $H_\alpha$. Comme $K \cap C(UH_{\alpha_0})$ est compact, il existerait une valeur d’adhérence $s$ de $\alpha \to t_\alpha$ suivant $\Phi'$, appartenant à $K \cap C(UH_{\alpha_0})$ ; mais comme $\Phi'$ converge vers $\alpha_0$ dans $\Gamma$, cela contredit le lemme 3 du no 1.

## EXERCICES {#int-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
