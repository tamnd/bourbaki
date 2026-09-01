---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 2
section_title: Représentations linéaires des groupes
lang: fr
source: int-vii-viii-fr
pdf_pages: 0127-0139
extraction: ocr
subsections:
    - "no": 1
      title: Représentations linéaires continues.
      page: 0
      pdf_page: 127
    - "no": 2
      title: Représentation contragrédiente.
      page: 0
      pdf_page: 130
    - "no": 3
      title: 'Exemple : représentations linéaires dans des espaces de fonctions continues.'
      page: 0
      pdf_page: 131
    - "no": 4
      title: 'Exemple : représentations linéaires dans des espaces de mesures.'
      page: 0
      pdf_page: 133
    - "no": 5
      title: 'Exemple : représentations linéaires dans les espaces $L^p$.'
      page: 0
      pdf_page: 133
    - "no": 6
      title: Prolongement d’une représentation linéaire de $G$ aux mesures sur $G$.
      page: 0
      pdf_page: 135
    - "no": 7
      title: Relations entre les endomorphismes $U(\mu)$ et les endomorphismes $U(s)$.
      page: 0
      pdf_page: 136
statements: 22
exercises: 0
content_sha256: 44a57de0c4a6a533f84f5b948fbf1f0d490f84c3155cf450b525e49bf5166e03
---

## § 2. Représentations linéaires des groupes.

### 1. Représentations linéaires continues.

Soient $G$ un groupe topologique, $E$ un espace localement convexe, $U$ une représentation linéaire de $G$ dans $E$.

#### Définition 1 {#int-viii-s2-def-1 .statement}

(i) On dit que $U$ est séparément continue si, pour tout $s \in G$, $U(s)$ est un endomorphisme continu de $E$, et si, pour tout $x \in E$, l’application $s \to U(s)x$ de $G$ dans $E$ est continue.

(ii) On dit que $U$ est continue si $(s, x) \to U(s)x$ est une application continue de $G \times E$ dans $E$.

(iii) On dit que U est équicontinue si elle est continue et si l’ensemble des endomorphismes U(s), où s parcourt G, est équicontinu.

#### Remarque 1 {#int-viii-s2-n1-rem-1 .statement}

Dire que U est séparément continue signifie que s → U(s) est une application continue de G dans l’espace $\mathcal{L}(E; E)$ des endomorphismes continus de E, muni de la topologie de la convergence simple.

#### Remarque 2 {#int-viii-s2-n1-rem-2 .statement}

Dire que U est continue équivaut à l’ensemble des trois conditions suivantes :

a) pour tout s ∈ G, U(s) est continu ; b) il existe un voisinage V de e tel que U(V) soit équicontinu ; c) il existe un ensemble total D dans E tel que, pour tout x ∈ D, l’application s → U(s)x soit continue.

Ces conditions sont évidemment nécessaires. Réciproquement, supposons les conditions a), b), c) satisfaites. Sur U(V), la topologie de la convergence simple est identique à la topologie de la convergence simple dans D (Esp. vect. top., chap. III, § 3, no 5, prop. 5). Donc l’application (s, x) → U(s)x de V × E dans E est continue (Top. gén., chap. X, 2e éd., § 2, no 1, cor. 3 de la prop. 1). Comme $U(s_0 s)x = U(s_0)(U(s)x)$ quels que soient $s_0 \in G, s \in G, x \in E$, on voit que U est continue.

Lorsque G est localement compact, les conditions a) et b) sont équivalentes à la condition :

a’) pour toute partie compacte K de G, U(K) est équicontinu.

#### Remarque 3 {#int-viii-s2-n1-rem-3 .statement}

Supposons que U soit une représentation linéaire continue G dans E. Pour tout s ∈ G, soit $\widehat{U}(s)$ le prolongement continu de U(s) au complété $\widehat{E}$ de E. Alors $\widehat{U}$ est une représentation linéaire de G dans $\widehat{E}$, satisfaisant aux conditions a) et c) de la Remarque 2, et aussi à la condition b) d’après Top. gén., chap. X, 2e éd., § 2, no 2, prop. 4. Donc $\widehat{U}$ est une représentation linéaire continue de G dans $\widehat{E}$.

#### Remarque 4 {#int-viii-s2-n1-rem-4 .statement}

Si E est un espace normé, on dit que U est isométrique lorsque $\|U(s)\| = 1$ pour tout $s \in G$. Il suffit pour cela que $\|U(s)\| \leq 1$ pour tout $s \in G$, car on a alors

$$
1 = \|1\| \leq \|U(s)\| \cdot \|U(s^{-1})\|,
$$
d'où $\|U(s)\| = \|U(s^{-1})\| = 1$ pour tout $s \in G$.

#### Proposition 1 {#int-viii-s2-prop-1 .statement}

*Si G est localement compact et si E est tonnelé, toute représentation linéaire U séparément continue de G dans E est continue.*

En effet, pour toute partie compacte K de G, $U(K)$ est compact pour la topologie de la convergence simple (*Remarque 1*), donc est équicontinu (*Esp. vect. top.*, Chap. III, § 3, no 6, th. 2); on applique alors la *Remarque 2*.

#### Lemme 1 {#int-viii-s2-lem-1 .statement}

*Soient G un groupe localement compact, $\rho$ une fonction finie semi-continue inférieurement $\geq 0$ sur G telle que $\rho(st) \leq \rho(s)\rho(t)$ quels que soient s, t dans G. Alors $\rho$ est majorée dans toute partie compacte de G.*

Il existe une partie ouverte non vide U de G telle que $\rho$ soit majorée dans U (*Top. gén.*, chap. IX, 2e éd., § 5, no 4, th. 2). Soit K une partie compacte de G. Alors K est recouvert par un nombre fini d'ensembles $s_1 U, \ldots, s_n U$. Pour tout $x \in U$, on a $\rho(s_i x) \leq \rho(s_i) \rho(x)$, donc $\rho$ est majorée dans $s_i U$, donc dans K.

#### Lemme 2 {#int-viii-s2-lem-2 .statement}

*Soient G un groupe topologique, U une représentation linéaire de G dans un espace normé E, A une partie partout dense de E. On suppose que, pour tout $s \in G$, $U(s)$ est continu et que, pour tout $x \in A$, $s \to U(s)x$ est une application continue de G dans E. Alors la fonction $s \to g(s) = \|U(s)\|$ sur G est semi-continue inférieurement et vérifie $g(st) \leq g(s)g(t)$.

Soit B la boule unité de E. On a $g(s) = \sup_{x \in B \cap A} \|U(s)x\|$, et chaque fonction $s \to \|U(s)x\|$ est continue sur G, donc $g$ est semi-continue inférieurement. D'autre part,

$$
g(st) = \|U(s)U(t)\| \leq \|U(s)\| \cdot \|U(t)\| = g(s)g(t).
$$

#### Proposition 2 {#int-viii-s2-prop-2 .statement}

*Soient G un groupe localement compact, U une représentation linéaire de G dans un espace normé E. Soit A une partie partout dense de E. On suppose que, pour tout s ∈ G, U(s) est continu et que, pour tout x ∈ A, s → U(s)x est une application continue de G dans E. Alors U est continue.
En effet, \|U(s)\| est majoré sur toute partie compacte de G d’après les lemmes 1 et 2, et l’on applique alors la Remarque 2.

### 2. Représentation contragrédiente.

Soit U une représentation linéaire séparément continue de G dans E. Soit E’ le dual de E. L’application s → $^tU(s)$ est une représentation linéaire dans E’ du groupe $G^0$ opposé à G ; nous dirons que cette représentation est la transposée de U. L’application $s \to ^tU(s^{-1}) = ^tU(s)^{-1}$ est une représentation linéaire de G dans E’, appelée contragrédiente de U.

#### Lemme 3 {#int-viii-s2-lem-3 .statement}

Soient X un espace localement compact, Y et Z des espaces topologiques, φ une application continue de $X \times Y$ dans Z, $\varphi_x$ l’application $y \to \varphi(x, y)$ de Y dans Z. Les espaces $\mathcal{C}(Y)$, $\mathcal{C}(Z)$ étant munis de la topologie de la convergence compacte, l’application $(x, f) \to f \circ \varphi_x$ de $X \times \mathcal{C}(Z)$ dans $\mathcal{C}(Y)$ est continue.

Il suffit évidemment de considérer le cas où X est compact. Soient $(x_0, f_0) \in X \times \mathcal{C}(Z)$, K une partie compacte de Y, et $\varepsilon > 0$. Soit $K' = \varphi(X \times K)$. Comme $f_0 \circ \varphi$ est uniformément continue dans $X \times K$, il existe un voisinage W de $x_0$ tel que $|f_0(\varphi(x, y)) - f_0(\varphi(x_0, y))| \leq \varepsilon$ pour $x \in W$ et $y \in K$. D’autre part, si l’on prend $f \in \mathcal{C}(Z)$ telle que $|f(z) - f_0(z)| \leq \varepsilon$ pour tout $z \in K'$, on aura $|f(\varphi(x, y)) - f_0(\varphi(x, y))| \leq \varepsilon$ pour $x \in X$, $y \in K$, et par suite $|f(\varphi(x, y)) - f_0(\varphi(x_0, y))| \leq 2\varepsilon$ pour $x \in W$ et $y \in K$. D’où le lemme.

Revenons alors aux notations antérieures.

#### Proposition 3 {#int-viii-s2-prop-3 .statement}

(i) Si U est séparément continue, $^tU$ est séparément continue lorsqu’on munit E’ de la topologie faible $\sigma(E', E)$.

(ii) Si G est localement compact et si U est continue, $^tU$ est continue lorsqu’on munit E’ de la topologie de la convergence compacte.

L’assertion (i) est immédiate. L’assertion (ii) résulte du lemme 3 où l’on fait $X = G,\ Y = Z = E,\ \varphi(s, x) = U(s)x$.

### 3. Exemple : représentations linéaires dans des espaces de fonctions continues.

Soit $G$ un groupe discret opérant à gauche sur un ensemble $X$. Une fonction complexe $\chi$ sur $G \times X$ est appelée un multiplicateur si l’on a

(1) $\chi(e, x) = 1$ quel que soit $x \in X$;

(2) $\chi(st, x) = \chi(s, tx)\chi(t, x)$ quels que soient $s, t$ dans $G,\ x \in X$.

On en déduit

(3) $\chi(t^{-1}, tx)\chi(t, x) = 1$ quels que soient $t \in G,\ x \in X$,

et en particulier $\chi(t, x) \neq 0$ quels que soient $t \in G,\ x \in X$.

Pour toute fonction complexe $f$ définie sur $X$ et tout $s \in G$, soit $\gamma_\chi(s)f$ la fonction complexe sur $X$ définie par

(4) $(\gamma_\chi(s)f)(x) = \chi(s^{-1}, x)f(s^{-1}x)$.

On a $\gamma_\chi(e)f = f$, et

$$
(\gamma_\chi(s)\gamma_\chi(s')f)(x) = \chi(s^{-1}, x)(\gamma_\chi(s')f)(s^{-1}x)
$$
$$
= \chi(s^{-1}, x)\chi({s'}^{-1}, s^{-1}x)f({s'}^{-1}s^{-1}x)
$$
$$
= \chi((ss')^{-1}, x)f((ss')^{-1}x) = (\gamma_\chi(ss')f)(x),
$$

donc $\gamma_\chi$ est une représentation linéaire de $G$. Pour $\chi = 1$, on retrouve les endomorphismes $\gamma(s)$ (chap. VII, § 1, no 1, formule (3)).

Supposons maintenant $G$ et $X$ localement compacts, $G$ opérant continûment sur $X$, et $\chi$ continue sur $G \times X$. Alors $\mathcal{C}(X)$ et $\mathcal{K}(X)$ sont stables pour les $\gamma_\chi(s)$, d’où des représentations linéaires de $G$ dans $\mathcal{C}(X)$ et $\mathcal{K}(X)$ que nous noterons encore $\gamma_\chi$.

#### Proposition 4 {#int-viii-s2-prop-4 .statement}

Les représentations linéaires $\gamma_\chi$ de $G$ dans $\mathcal{C}(X)$ et $\mathcal{K}(X)$ sont continues.

L’application $(s, f) \to (s, \gamma(s)f)$ de $G \times \mathcal{C}(X)$ dans $G \times \mathcal{C}(X)$ est continue (n° 2, lemme 3). D’autre part, l’application $(s, f) \to \chi(s, .)f$ de $G \times \mathcal{C}(X)$ dans $\mathcal{C}(X)$ est continue ; car, si $s$ tend vers $s_0$ dans $G$, $\chi(s, .)$ tend vers $\chi(s_0, .)$ uniformément dans toute partie compacte de $X$ ; si en outre $f$ tend vers $f_0$ dans $\mathcal{C}(X)$, $\chi(s, .)f$ tend vers $\chi(s_0, .)f_0$ uniformément dans toute partie compacte de $X$, d’où notre assertion. Donc la représentation $\gamma_\chi$ de $G$ dans $\mathcal{C}(X)$ est continue.

Montrons que la représentation $\gamma_\chi$ de $G$ dans $\mathscr{K}(X)$ est continue. Comme $\mathscr{K}(X)$ est limite inductive d’espaces de Banach, il est tonnelé ($Esp.\ vect.\ top.$, chap. III, § 1, n° 2, cor. 2 de la prop. 2), donc il suffit de prouver que $\gamma_\chi$ est séparément continue (n° 1, prop. 1). Or, soient $H$ une partie compacte de $X$ et $s_0 \in G$. Soient $V$ un voisinage compact de $s_0$ dans $G$, et $L = VH$, qui est compact dans $X$. Pour toute $f \in \mathscr{K}(X, H)$, le support de $\gamma_\chi(s_0)f$ est contenu dans $L$, et l’on a

$$
\sup_{x \in X} |(\gamma_\chi(s_0)f)(x)| \leq \sup_{x \in L} |\chi(s_0^{-1}, x)| \cdot \sup_{x \in X} |f(x)|,
$$

donc $f \to \gamma_\chi(s_0)f$ est une application linéaire continue de $\mathscr{K}(X, H)$ dans $\mathscr{K}(X, L)$ ; il en résulte que $f \to \gamma_\chi(s_0)f$ est une application linéaire continue de $\mathscr{K}(X)$ dans lui-même ($Esp.\ vect.\ top.$, chap. II, § 2, n° 2, cor. de la prop. 1). D’autre part, la topologie de $\mathscr{K}(X, L)$ est induite par celle de $\mathcal{C}(X)$. D’après ce qui a déjà été démontré, l’application $s \to \gamma_\chi(s)f$ de $V$ dans $\mathscr{K}(X, L)$ est continue. Ceci achève de prouver que $\gamma_\chi$ est séparément continue.

#### Proposition 5 {#int-viii-s2-prop-5 .statement}

*Supposons que chaque fonction $\chi(s, .)$ soit bornée. Alors $\gamma_\chi$ laisse stable $\mathscr{K}(X)$, et la représentation linéaire $\gamma_\chi$ de $G$ dans $\mathscr{K}(X)$ est continue.*

Il est clair que $\gamma_\chi$ laisse stable $\mathscr{K}(X)$ et que chacun des $\gamma_\chi(s)$ est *continu* dans $\mathscr{K}(X)$. D’autre part, pour toute $f \in \mathscr{K}(X)$, $s \to \gamma_\chi(s)f$ est *une* application continue de $G$ dans $\mathscr{K}(X)$ et *a fortiori* dans $\mathscr{K}(X)$. Donc la représentation $\gamma_\chi$ dans $\mathscr{K}(X)$ est continue (n° 1, prop. 2).

### 4. Exemple : représentations linéaires dans des espaces de mesures.

Soient toujours G un groupe localement compact, opérant continûment à gauche dans un espace localement compact X, et $\chi$ un multiplicateur continu sur $G \times X$. La représentation linéaire $\gamma_\chi$ de G dans $\mathcal{H}(X)$ admet une représentation contragrédiente dans $\mathcal{M}(X)$, que nous noterons encore $\gamma_\chi$, et qui est définie par la formule suivante (où $\mu \in \mathcal{M}(X)$, $f \in \mathcal{H}(X)$) :

$$
\langle \gamma_\chi(s)\mu, f \rangle = \langle \mu, \gamma_\chi(s^{-1})f \rangle = \langle \chi(s, .) \cdot \mu, \gamma(s^{-1})f \rangle = \langle \gamma(s)(\chi(s, .) \cdot \mu), f \rangle
$$

d'où

$$
\gamma_\chi(s)\mu = \gamma(s)(\chi(s, .) \cdot \mu) = (\gamma(s)\chi(s, .)) \cdot (\gamma(s)\mu).
$$

Remarquons que

$$
(\gamma(s)\chi(s, .))(x) = \chi(s, s^{-1}x).
$$

La représentation linéaire $\gamma_\chi$ de G dans $\mathcal{C}(X)$ admet une représentation contragrédiente dans l’espace $\mathcal{C}'(X)$ des mesures sur X à support compact, représentation que nous noterons encore $\gamma_\chi$; les endomorphismes $\gamma_\chi(s)$ de $\mathcal{C}'(X)$ sont les restrictions des endomorphismes $\gamma_\chi(s)$ de $\mathcal{M}(X)$.

#### Proposition 6 {#int-viii-s2-prop-6 .statement}

Si l’on munit $\mathcal{M}(X)$ (resp. $\mathcal{C}'(X)$) de la topologie de la convergence uniforme dans les parties compactes de $\mathcal{H}(X)$ (resp. $\mathcal{C}(X)$), la représentation linéaire $\gamma_\chi$ de G dans $\mathcal{M}(X)$ (resp. $\mathcal{C}'(X)$) est continue.

#### Proposition 7 {#int-viii-s2-prop-7 .statement}

Supposons que chaque fonction $\chi(s, .)$ soit bornée. Alors $\gamma_\chi$ laisse stable $\mathcal{M}^1(X)$ et, si l’on munit $\mathcal{M}^1(X)$ de la topologie de la convergence uniforme dans les parties compactes de $\overline{\mathcal{H}(X)}$, la représentation linéaire $\gamma_\chi$ de G dans $\mathcal{M}^1(X)$ est continue.

Ces propositions résultent des prop. 3, 4, 5.

### 5. Exemple : représentations linéaires dans les espaces $L^p$.

Soit toujours G un groupe localement compact, opérant continûment à gauche dans un espace localement compact X.

Soit $\beta$ une mesure positive sur $X$ de support $X$. Supposons qu’il existe une fonction continue $\chi > 0$ sur $G \times X$ telle qu’on ait, pour tout $s \in G$,

$$
\gamma(s)\beta = \chi(s^{-1}, .) \cdot \beta
$$

(ce qui implique en particulier que $\beta$ est quasi-invariante par $G$). *Alors, $\chi$ est un multiplicateur.* En effet, soient $s, t$ dans $G$; on a

$$
\gamma(s)\gamma(t)\beta = \gamma(s)(\chi(t^{-1}, .) \cdot \beta) = (\gamma(s)\chi(t^{-1}, .)) \cdot (\gamma(s)\beta)
$$
$$
= (\gamma(s)\chi(t^{-1}, .)) \cdot \chi(s^{-1}, .) \cdot \beta
$$
$$
\gamma(st)\beta = \chi(t^{-1}s^{-1}, .) \cdot \beta
$$

donc

$$
\chi(t^{-1}, s^{-1}x)\chi(s^{-1}, x) = \chi(t^{-1}s^{-1}, x)
$$

localement $\beta$-presque partout, et en conséquence partout puisque $\chi$ est continue et $\beta$ de support $X$.

Soit $p \in [1, +\infty[$. Pour toute $f \in \mathcal{L}_c^n(X, \beta)$ et tout $s \in G$, soit $\gamma_{\chi,p}(s)f$ la fonction sur $X$ définie par

$$
(\gamma_{\chi,p}(s)f)(x) = \chi(s^{-1}, x)^{1/p}f(s^{-1}x).
$$

On a

$$
\int^* |\chi(s^{-1}, x)^{1/p}f(s^{-1}x)|^p d\beta(x) = \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \int |f(x)|^p d\beta(x)
$$

donc $\gamma_{\chi,p}(s)f \in \mathcal{L}_c^n(X, \beta)$. On voit que $\gamma_{\chi,p}(s)$ est un endomorphisme *isométrique* de $\mathcal{L}_c^n(X, \beta)$ et définit par passage au quotient un endomorphisme isométrique de $L_c^n(X, \beta)$, noté encore $\gamma_{\chi,p}(s)$. D’autre part, $\chi^{1/p}$ est évidemment un multiplicateur, donc $\gamma_{\chi,p}$ est une représentation linéaire de $G$ dans $L_c^n(X, \beta)$ d’après ce qu’on a vu au no 3.

#### Proposition 8 {#int-viii-s2-prop-8 .statement}

*La représentation linéaire $\gamma_{\chi,p}$ de $G$ dans $L_c^n(X, \beta)$ est continue et isométrique.*

Soit $f \in \mathcal{H}(X)$. Quand $s$ tend vers $s_0$ dans $G$, $\gamma_{\chi,p}(s)f$ tend vers $\gamma_{\chi,p}(s_0)f$ dans $\mathcal{K}(X)$, donc dans $L_c^p(X, \beta)$. Comme les $\gamma_{\chi,p}(s)$ sont isométriques, la prop. 8 s’obtient en appliquant la Remarque 2 du n° 1.

Pour le cas où $\chi$ n’est pas supposée continue, cf. § 4, exerc. 13.

#### Proposition 9 {#int-viii-s2-prop-9 .statement}

Supposons que chaque fonction $\chi(s, .)$ soit bornée. Alors $\gamma_\chi$ laisse stable $L_c^p(X, \beta)$, et la représentation linéaire $\gamma_\chi$ de $G$ dans $L_c^p(X, \beta)$ est continue.

Soit $f \in \mathcal{L}_c^p(X, \beta)$. On a

$$
\int^* |\chi(s^{-1}, x)f(s^{-1}x)|^p d\beta(x) \leq \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$

$$
= \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int |f(x)|^p d\beta(x)
$$

donc $\gamma_\chi(s)f \in \mathcal{L}_c^p(X, \beta)$, et

(5)

$$
\|\gamma_\chi(s)\| \leq \sup_{x \in X} \chi(s^{-1}, x)^{1/q}
$$

en notant $q$ l’exposant conjugué de $p$. Si $f \in \mathcal{K}(X)$, $\gamma_\chi(s)f$ tend vers $\gamma_\chi(s_0)f$ dans $\mathcal{K}(X)$, donc dans $\mathcal{L}_c^p(X, \beta)$, quand $s$ tend vers $s_0$. Donc la représentation $\gamma_\chi$ de $G$ dans $L_c^p(X, \beta)$ est continue (n° 1, prop. 2).

On a des propriétés analogues à celles des n°s 3, 4, 5 si $G$ opère à droite dans $X$.

En particulier, si l’on considère $G$ comme opérant sur lui-même par translations à gauche ou à droite, et si l’on fait $\chi = 1$, on obtient les représentations régulières gauche et droite de $G$ dans $\mathcal{C}(G)$, $\mathcal{K}(G)$, $\overline{\mathcal{K}(G)}$, $\mathcal{C}'(G)$, $\mathcal{M}(G)$, $\mathcal{M}^1(G)$. Si l’on prend pour $\beta$ une mesure de Haar à gauche (resp. à droite) de $G$, et si l’on fait $\chi = 1$, on obtient la représentation régulière gauche (resp. droite) de $G$ dans $L_c^p(G, \beta)$.

### 6. Prolongement d’une représentation linéaire de $G$ aux mesures sur $G$.

Soient $G$ un groupe localement compact, $E$ un espace localement convexe, $U$ une représentation linéaire de $G$ dans $E$.

Supposons $U$ continue et $E$ quasi-complet. Alors pour toute mesure $\mu \in \mathcal{C}'(G)$, on a $\int_G U(s)d\mu(s) \in \mathcal{L}(E; E)$ (chap. VI, § 1, no 7).

Nous poserons $U(\mu) = \int_G U(s)d\mu(s)$. Munissons $\mathcal{C}'(G)$ de la topologie de la convergence compacte dans $\mathcal{C}(G)$. L’application $(\mu, x) \to U(\mu)x$ de $\mathcal{C}'(G) \times E$ dans $E$ est hypocontinue relativement aux parties équicontinues de $\mathcal{C}'(G)$ et aux parties compactes de $E$; en particulier, l’application $\mu \to U(\mu)$ de $\mathcal{C}'(G)$ dans $\mathcal{L}(E; E)$ (muni de la topologie de la convergence compacte) est continue (*loc. cit.*, prop. 16).

Pour pouvoir appliquer plus loin ces résultats, notons que, si $X$ est un espace localement compact, $\mathcal{C}(X)$, muni de la topologie de la convergence compacte, est complet (*Top. gén.*, chap. X, 2e éd., § 1, no 6, cor. 3 du th. 2). D’autre part, $\mathcal{K}(X)$ est tonnelé, donc son dual $\mathcal{M}(X)$, muni de la topologie de la convergence compacte sur $\mathcal{K}(X)$, est quasi-complet (*Esp. vect. top.*, chap. III, § 3, no 7, cor. 2 du th. 4). Bien entendu, $\overline{\mathcal{K}(X)}$ est complet pour la topologie déduite de sa norme, donc son dual $\mathcal{M}^1(X)$ est quasi-complet pour la topologie de la convergence compacte sur $\overline{\mathcal{K}(X)}$ (*loc. cit.*).

Supposons maintenant que $U$ soit une représentation linéaire continue du groupe localement compact $G$ dans un *espace de Banach* $E$. Posons $g(s) = \|U(s)\|$ pour tout $s \in G$. Alors, si $\mu$ est une mesure sur $G$ telle que $g$ soit $\mu$-intégrable, on a
$$
\int_G U(s)d\mu(s) \in \mathcal{L}(E; E) \quad \text{et} \quad \| \int_G U(s)d\mu(s) \| \leq \int g(s)d|\mu|(s)
$$
(Chap. VI, § 1, no 7, *Remarque* 1). Nous poserons encore
$$
U(\mu) = \int_G U(s)d\mu(s).
$$

### 7. Relations entre les endomorphismes $U(\mu)$ et les endomorphismes $U(s)$.

#### Lemme 4 {#int-viii-s2-lem-4 .statement}

*Soient T un espace localement compact, a un point de T, M une partie de $\mathcal{M}(T)$, $\mathfrak{F}$ un filtre sur M. On suppose que :*

(i) pour toute partie compacte K de T, les nombres $|\mu|(K)$, pour $\mu \in M$, sont majorés ;
(ii) $\lim_{\mu, \mathfrak{F}} |\mu|(K) = 0$ pour toute partie compacte K de $T - \{a\}$;
(iii) il existe un voisinage compact V de a dans T tel que $\lim_{\mu, \mathfrak{F}} \mu(V) = 1$.

Alors le filtre $\mathfrak{F}$ converge vers $\varepsilon_a$ dans $\mathcal{M}(T)$ muni de la topologie de la convergence compacte dans $\mathcal{K}(T)$.

D’après l’hypothèse (i), M est une partie équicontinue de $\mathcal{M}(T)$ puisqu’elle est vaguement bornée et que $\mathcal{K}(T)$ est tonnelé (*Esp. vect. top.*, chap. III, § 3, no 6, th. 2). Il suffit donc (*Top. gén.*, chap. X, 2e éd., § 2, no 4, th. 1) de prouver que, si $f \in \mathcal{K}(T)$, on a $\lim_{\mu, \mathfrak{F}} \mu(f) = f(a)$. Soit K la réunion de V et du support de $f$; si K’ est l’adhérence de $K - V$, on a
$$
|\mu(K) - \mu(V)| = |\mu(K - V)| \leq |\mu|(K');
$$
comme K’ est compact et ne contient pas a, on en conclut que $\lim_{\mu, \mathfrak{F}} \mu(K) = 1$. Soit $\varepsilon > 0$, et soit W un voisinage ouvert de a dans K tel que $|f(t) - f(a)| \leq \varepsilon$ pour $t \in W$; on peut écrire
$$
\mu(f) - f(a) = f(a)(\mu(K) - 1) + \int_K (f(t) - f(a)) d\mu(t);
$$
l’intégrale sur K peut s’écrire comme somme des intégrales analogues sur W et sur $K - W$; si C = sup $|f|$, on aura donc
$$
|\mu(f) - f(a)| \leq C|\mu(K) - 1| + \varepsilon . |\mu|(K) + 2C . |\mu|(K - W).
$$
Comme le premier et le troisième terme du second membre tendent vers 0 suivant $\mathfrak{F}$, on voit bien que $\lim_{\mu, \mathfrak{F}} \mu(f) = f(a)$.

#### Corollaire 1 {#int-viii-s2-lem-4-cor-1 .statement}

Les hypothèses étant celles du lemme 4, supposons de plus qu’il existe une partie compacte $K_0$ de T contenant les supports de toutes les mesures $\mu \in M$. Alors $\mathfrak{F}$ converge aussi vers $\varepsilon_a$ dans $\mathcal{C}'(T)$ muni de la topologie de la convergence compacte dans $\mathcal{C}(T)$.

En effet, l’application de restriction de $\mathcal{C}(T)$ dans $\mathcal{C}(K_0)$ est continue ; donc, si H est une partie compacte de $\mathcal{C}(T)$, les restrictions à $K_0$ des fonctions de H forment une partie compacte de $\mathcal{C}(K_0)$. Il suffit alors d’appliquer le lemme 4 en remplaçant T par $K_0$.

#### Corollaire 2 {#int-viii-s2-lem-4-cor-2 .statement}

Les hypothèses étant celles du cor. 1, soit $f$ une application continue de T dans un espace localement convexe quasi-complet E. On a
$$
\lim_{\mu,\mathfrak{F}} \int f(t)d\mu(t) = f(a).
$$
Ceci résulte du cor. 1 et de la prop. 14 du chap. VI, § 1, no 6.

#### Corollaire 3 {#int-viii-s2-lem-4-cor-3 .statement}

Soient G un groupe localement compact, E un espace localement convexe quasi-complet, U une représentation linéaire continue de G dans E. Soient $\beta$ une mesure positive sur G, a un élément de G, $\mathcal{B}$ une base du filtre des voisinages de a, formée de voisinages compacts. Pour tout $V \in \mathcal{B}$, soit $f_V$ une fonction continue $\geqslant 0$ sur G, de support contenu dans V, et telle que $\int f_V d\beta = 1$. Alors, pour tout $x \in E$, on a
$$
U(a)x = \lim_V U(f_V \cdot \beta)x
$$
la limite étant prise suivant le filtre des sections de $\mathcal{B}$.

L’application $s \to U(s)x$ de G dans E est continue. D’après le cor. 2, on a $U(a)x = \lim_V \int (U(s)x) \cdot f_V(s)d\beta(s)$ suivant le filtre des sections de $\mathcal{B}$, c’est-à-dire $U(a)x = \lim_V U(f_V \cdot \beta)x$.

#### Proposition 10 {#int-viii-s2-prop-10 .statement}

Soient G un groupe localement compact, E un espace localement convexe quasi-complet, U une représentation linéaire continue de G dans E, $\beta$ une mesure positive sur G de support G.

(i) Les vecteurs $U(f \cdot \beta)x$, où $f$ parcourt $\mathcal{K}(G)$ et où $x$ parcourt E, sont partout denses dans E.

(ii) Soit F un sous-espace vectoriel fermé de E. Si F est stable pour U, on a $U(\mu)(F) \subset F$ pour toute $\mu \in \mathcal{C}'(G)$. Réciproquement, si $U(f \cdot \beta)(F) \subset F$ pour toute $f \in \mathcal{K}(G)$, F est stable pour U.

La première partie de (ii) est immédiate puisque les restrictions des $U(s)$ à $F$ ($s \in G$) définissent une représentation linéaire continue de $G$ dans l’espace localement convexe quasi-complet $F$. La deuxième partie de (ii), et (i), résultent du cor. 3 du lemme 4.
