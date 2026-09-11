---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 11
section_title: Formule de Stokes
lang: fr
source: var-fr
pdf_pages: 0136-0142
extraction: ocr
subsections:
    - "no": 1
      title: Pièces
      page: 0
      pdf_page: 136
    - "no": 2
      title: Formule de Stokes pour les pièces
      page: 0
      pdf_page: 137
    - "no": 3
      title: Formule de Stokes pour les ensembles localement polyédraux[^1]
      page: 0
      pdf_page: 138
    - "no": 4
      title: Formule de Stokes relative (intégration sur les fibres)
      page: 0
      pdf_page: 139
statements: 1
exercises: 0
content_sha256: f1165c8a6f12721343d74c911068a2aca50a9171ac61b24075e228a251000002
---

## § 11. Formule de Stokes

Dans ce paragraphe, on suppose $\mathbf{K}=\mathbf{R}$.

### 11.1. Pièces

### 11.1.1. Soit E un espace de Banach. Une partie S de E est appelée un demi-espace fermé s'il existe une forme linéaire continue $h\neq 0$ et un nombre réel $k$ tel que $S=\{x|h(x)\leq k\}$ (cf. EVT, II, § 2, no 6); la frontière de S est alors l'hyperplan fermé $\{x|h(x)=k\}$; on l'appelle également le bord de S, et on le note $\partial S$.

### 11.1.2. Soient X une variété de classe $C^r$ et A une partie de X. On dit que A est une pièce de X si, pour tout $a\in A$, il existe une carte $c=(U,\varphi,E)$ de X en a telle que $\varphi(A\cap U)$ soit un ouvert d'un demi-espace fermé de E. On pose $\partial A=A-\mathring{A}$ (ensemble des points non intérieurs de A). C'est une sous-variété de A, que l'on appelle le bord de A.[^1] Si $a\in\partial A$, il existe une carte $c=(U,\varphi,E)$ de X centrée en a et un hyperplan fermé H de E tels que $\varphi(A\cap U)$ soit un voisinage ouvert de 0 dans un des demi-espaces fermés $S_c$ de E définis par H (EVT, II, § 2, no 6), et que $\varphi(\partial A\cap U)=H\cap\varphi(A\cap U)$. Une telle carte est dite adaptée à A en a. Le demi-espace fermé $S_c$ est alors l'unique demi-espace fermé de E dont $\varphi(A\cap U)$ soit un ouvert.

Pour qu'une partie fermée A de X soit une pièce de X, il faut et il suffit que $\mathring{A}$ soit dense dans A et que $A-\mathring{A}$ soit une sous-variété de X de codimension 1 en chacun de ses points.

### 11.1.3. Exemples

a) Dans $\mathbf{R}^n$, une boule fermée de rayon $>0$ est une pièce; son bord est la sphère correspondante.

b) Si A est une pièce de la variété X et si B est une partie fermée de $\partial A$, alors $A-B$ est une pièce de X.

c) Soit $\varphi:X\rightarrow X'$ un morphisme de variétés de classe $C^r$, et soit $A'$ une pièce de $X'$. Si $\varphi$ est transversale à $\partial A'$ (5.11.6), $\varphi^{-1}(A')$ est une pièce de X dont le bord est $\varphi^{-1}(\partial A')$.

En particulier, soit $h : X \to \mathbf{R}$ une fonction de classe $C^r$, et soit $a \in \mathbf{R}$; supposons qu’il n’existe aucun $x \in X$ tel que $h(x) = a$ et $d_x h = 0$. L’ensemble $\{ x | h(x) \leq a \}$ est une pièce fermée de $X$ de bord $h^{-1}(a)$.

d) Si $r = \infty$ et si $X$ est localement compacte, tout compact de $X$ admet un système fondamental de voisinages formé de pièces compactes.

11.1.4. Soient $X$ une variété de classe $C^r$ et $A$ une pièce de $X$. Soient $a \in \partial A$ et $v \in T_a(X)$. Soit $c = (U, \varphi, E)$ une carte de $X$ adaptée à $A$ en $a$ (11.1.2) et soit $h = \theta_c^{-1}(v)$ l’élément de $E$ correspondant à $v$ (5.5.1). Soit $S_c$ le demi-espace fermé de $E$ dont $\varphi(A \cap U)$ est un ouvert (11.1.2). On dit que $v$ est un *vecteur rentrant* (resp. *strictement rentrant*, resp. *sortant*, resp. *strictement sortant*) pour $A$ en $a$ si $h$ appartient à $S_c$ (resp. $\dot{S}_c, -S_c, -\dot{S}_c$), condition qui est indépendante du choix de la carte adaptée $c$. On note $T_a^+(A)$ (resp. $T_a^-(A)$) l’ensemble des vecteurs sortants (resp. rentrants) de $T_a(X)$ pour $A$. Ce sont des demi-espaces fermés de $T_a(X)$, dont le bord contient 0. On a
$$
T_a(\partial A) = T_a^+(A) \cap T_a^-(A).
$$

**11.2. Formule de Stokes pour les pièces**

Dans ce n°, on désigne par $X$ une variété de classe $C^r$ ($r \geq 2$) pure de dimension finie $n$ et séparée. On désigne par $A$ une pièce de $X$ et par $i$ l’injection canonique de $\partial A$ dans $X$. On désigne par $E$ un espace de Banach.

### 11.2. Formule de Stokes pour les pièces

11.2.1. Soit $x \in \partial A$ et soit $\xi$ une orientation de $T_x(\partial A)$; on note $\tilde{i}_x(\xi)$ l’orientation de $T_x(X)$ contenant les éléments $v \wedge u$, où $v$ est un vecteur strictement sortant pour $A$ en $x$ (11.1.4) et où $u$ est un élément non nul de $\wedge^{n-1} T_x(\partial A)$ appartenant à l’orientation $\xi$. L’application $\tilde{i}_x$ est une bijection de $\mathrm{Or}(T_x(\partial A))$ sur $\mathrm{Or}(T_x(X))$. Les applications $\tilde{i}_x$ pour $x \in \partial A$, définissent un morphisme $\tilde{i} : \tilde{\partial A} \to \tilde{X}$ qui est une *orientation* de $i$ (10.2.5). Si $\xi$ est une orientation de $X$, l’orientation de $\partial A$ associée à $\xi$ par $\tilde{i}$ (10.2.5) est dite *définie par* $\xi$.

#### Exemple {#var-2-s11-n2-exa-1 .statement}

Lorsque $X = \mathbf{R}^n$, que $\xi$ est l’orientation usuelle de $\mathbf{R}^n$ et que $A$ est une boule fermée de rayon $> 0$, l’orientation de la sphère $\partial A$ définie par $\xi$ est l’orientation canonique (10.2.8, b)).

11.2.2. Soit $\omega$ une forme différentielle tordue de degré $p$ sur $X$ à valeurs dans $E$ (10.4.1); l’image réciproque $i^*(\omega)$ de $\omega$ par le morphisme orienté $i : \partial A \to X$ se note $\omega|_{\partial A}$ et s’appelle la *forme induite par* $\omega$ *sur* $\partial A$ (cf. 10.4.3).

11.2.3. Faisons l’une des deux hypothèses suivantes:

(i) $\omega$ est une forme différentielle tordue de degré $n-1$ sur $X$, à valeurs dans $E$;
(ii) $X$ est orientée, $\partial A$ est munie de l’orientation correspondante (11.2.1) et $\omega$ est une forme différentielle de degré $n-1$ sur $X$ à valeurs dans $E$.

Supposons de plus que $\omega$ soit *de classe* $C^1$ et que l’intersection de $A$ et du support de $\omega$ soit compacte. La différentielle extérieure $d\omega$ de $\omega$ est continue (8.3.5 et 10.3.4).

La fonction caractéristique de $A$ est essentiellement intégrable pour la mesure vectorielle définie par $d\omega$ sur $X$ et la forme différentielle $\omega|_{\partial A}$ de degré $n - 1$ sur $\partial A$ est intégrable (10.4.3 et 10.4.4). On a
$$
\int_A d\omega = \int_{\partial A} \omega \quad \text{(« formule de Stokes »)}.
$$
11.2.4. Soit $\alpha$ une forme différentielle tordue de degré $n$ sur $X$ à valeurs dans $E$, à support compact, et de classe $C^1$. Pour qu’il existe une forme différentielle tordue $\omega$ de degré $n - 1$ sur $X$, à valeurs dans $E$, à support compact et de classe $C^1$, telle que $\alpha = d\omega$, il est nécessaire que $\int_X \alpha = 0$; si $X$ est connexe, cette condition est suffisante; si de plus $\alpha$ est de classe $C^k$ ($k \leq r - 1, k \neq \omega$), on peut choisir $\omega$ de classe $C^k$.

11.2.5. Supposons que $X$ soit la variété réelle sous-jacente à $\mathbf{C}$, que $E$ soit un espace de Banach complexe et que $A$ soit une pièce *compacte* de $X$. Munissons $X$ de l’orientation définie par sa structure complexe (10.2.7). Soit $f$ une application *continue* de $A$ dans $E$ dont la restriction à l’intérieur $\mathring{A}$ de $A$ est holomorphe. Notons $dz$ la différentielle de l’injection $z : \partial A \to \mathbf{C}$. La forme $f.dz$, produit de $f$ et de $dz$, est une forme différentielle de degré 1 sur $\partial A$, à valeurs dans $E$, de classe $C^0$, et l’on a:
$$
\int_{\partial A} f.dz = 0 \quad \text{(« formule de Cauchy »)}.
$$
Lorsque $f$ se prolonge en une application holomorphe, notée encore $f$, d’un voisinage ouvert $U$ de $A$, à valeurs dans $E$, la forme différentielle $f.dz$ (où $z$ désigne cette fois l’injection canonique de $U$ dans $\mathbf{C}$) est de classe $C^\infty$ sur $U$ et sa différentielle extérieure est nulle.

11.2.6 (*Dérivée d’une intégrale*). Supposons $X$ orientée. Soit $Y$ une variété de classe $C^r$, et soit $\alpha$ une forme différentielle de degré $n$ sur $Y$, à valeurs dans $E$, de classe $C^1$, et à support compact. Soit $I$ un ouvert de $\mathbf{R}$ contenant 0 et soit $g : I \times X \to Y$ un morphisme de classe $C^r$; pour $t \in I$, notons $g_t$ l’application $x \mapsto g(t, x)$ de $X$ dans $Y$. Notons $\psi$ le morphisme de $X$ dans $T(Y)$ défini par $\psi(x) = T_{(0, x)}(g)(1, 0)$; c’est un *relèvement* de $g_0$ (8.6.5). Supposons que la restriction de $\mathrm{pr}_1 : I \times A \to I$ à l’intersection de $I \times A$ et du support de $g^*(\alpha)$ soit *propre* (TG, I, § 10). Pour tout $t \in I$, l’intersection de $A$ et du support de $g_t^*(\alpha)$ est alors compacte; l’application $t \mapsto \int_A g_t^*(\alpha)$ est de classe $C^1$ sur $I$ et sa dérivée à l’origine est donnée par la formule
$$
\frac{d}{dt} \left( \int_A g_t^*(\alpha) \right)_{t=0} = \int_A \theta_\psi \cdot \alpha = \int_A i(\psi) \, d\alpha + \int_{\partial A} i(\psi) \, \alpha,
$$
cf. n° 8.6.

### 11.3. Formule de Stokes pour les ensembles localement polyédraux[^2]

Dans ce n°, $X$ désigne une variété réelle pure de dimension finie $n$ de classe $C^r$ ($r \geq 2$); on suppose $X$ séparée.

11.3.1. Soit $A$ une partie d’un espace vectoriel réel de dimension finie. On dit que $A$ est polyédrale si elle est réunion finie d’intersections finies de demi-espaces fermés. Une partie $A$ de $X$ est dite localement polyédrale si, pour tout $x\in X$, il existe une carte $c=(U,\varphi,E)$ de $X$ en $x$ et une partie polyédrale $A_c$ de $E$ telles que $\varphi(A\cap U)=\varphi(U)\cap A_c$. Une pièce de $X$ est une partie localement polyédrale.

11.3.2. Soit $A$ une partie fermée de $X$, et soit $\operatorname{Fr}(A)=A-\mathring{A}$ sa frontière. Un point $x\in\operatorname{Fr}(A)$ est dit régulier s’il existe un voisinage ouvert $U$ de $x$ tel que $A\cap U$ soit une pièce de la variété $U$ (auquel cas $x$ appartient au bord de $A\cap U$). On note $\partial A$ l’ensemble des points réguliers de $\operatorname{Fr}(A)$ et on l’appelle le bord régulier (ou simplement le bord) de $A$. L’ensemble $A'=\mathring{A}\cup\partial A$ est une pièce de $X$, de bord $\partial A$.

11.3.3. *\** **Exemple.** — Soit $\mathscr{H}$ un ensemble localement fini d’hyperplans d’un espace affine réel $E$ de dimension finie $n$, et soit $C$ une chambre de $E$ relativement à $\mathscr{H}$ (LIE, V, § 1, no 3). L’adhérence $\overline{C}$ de $C$ est une partie localement polyédrale de la variété $E$ ; le bord régulier de $\overline{C}$ est la réunion des faces de $C$ (loc. cit., no 4). En particulier, si $C$ est un simplexe ouvert (loc. cit., no 6) de sommets $a_0,\ldots,a_n$, le bord de $\overline{C}$ est la réunion des $C_{(i)}$ ($0\leq i\leq n$), où $C_{(i)}$ est le simplexe ouvert de sommets $a_0,\ldots,a_{i-1},a_{i+1},\ldots,a_n$ dans l’espace affine engendré par ces sommets.*\*

11.3.4. Soit $A$ une partie localement polyédrale de $X$, et soit $\omega$ une forme différentielle tordue de degré $n-1$ sur $X$ à valeurs dans un espace de Banach $E$ ; on suppose que $\omega$ est de classe $C^1$ et que l’intersection de son support avec $A$ est compacte. Alors, la fonction caractéristique de $A$ (resp. $A'$, $\hat{A}$) est essentiellement intégrable pour la mesure vectorielle définie par $d\omega$ sur $X$ et l’on a

$$
\int_A d\omega=\int_{A'}d\omega=\int_{\hat{A}}d\omega.
$$

La forme différentielle $\omega|\partial A$ (pour l’orientation canonique de l’injection canonique de $\partial A$, considérée comme le bord de la pièce $A'$, dans $X$) est intégrable dans $\partial A$ et l’on a

$$
\int_A d\omega=\int_{\partial A}\omega
\qquad\text{(« formule de Stokes »).}
$$

Lorsque $X$ est munie d’une orientation, et que l’on munit $\partial A$ de l’orientation correspondante (11.2.1), cette formule est encore valable si $\omega$ est une forme différentielle usuelle de degré $n-1$ à valeurs dans $E$, de classe $C^1$ et telle que $A\cap\operatorname{Supp}\omega$ soit compact.

### 11.4. Formule de Stokes relative (intégration sur les fibres)

Dans ce numéro, on désigne par $X$ et $S$ deux variétés (réelles) de classe $C^r$ et par $\pi:X\to S$ une submersion. On désigne par $n$ un entier et on suppose que, pour tout $s\in S$, la fibre $X_s=\pi^{-1}(s)$ de $\pi$ en $s$ (qui est une sous-variété de $X$ (5.10.5)) est pure de dimension $n$.

4—B.

11.4.1. Soient E et H deux espaces vectoriels et soit F un sous-espace vectoriel de dimension finie n de H. Soient p un entier $\geqslant 0$, u une application $(n + p)$-linéaire alternée de $H^{n+p}$ dans E et $t_1, \ldots, t_p$ des éléments de H/F; soient $t'_1, \ldots, t'_p$ des représentants de $t_1, \ldots, t_p$ dans H. L’application

$$
(x_1, \ldots, x_n) \mapsto u(t'_1, \ldots, t'_p, x_1, \ldots, x_n)
$$

est une application $n$-linéaire alternée de $F^n$ dans E, qui ne dépend que de u et des $t_i$; on la note $u \perp (t_1, \ldots, t_p)$ (cf. A, III, p. 158 pour le cas particulier $E = K$). L’application

$$
(t_1, \ldots, t_p) \mapsto u \perp (t_1, \ldots, t_p)
$$

est $p$-linéaire alternée.

11.4.2 (« $\pi$-torsion »). Considérons le fibré vectoriel T(X/S) sur X (8.1.3); il est de rang fini n en chaque point de X. On pose $\tilde{R}_\pi = \tilde{R}_{T(X/S)}$ (10.3.1) et $\tilde{X}_\pi = \mathrm{Or}_{T(X/S)}$ (10.2.2). Soit $s \in S$; compte tenu de l’identification naturelle de $T(X/S)|_{X_s}$ avec $T(X_s)$ (8.1.3), la fibre en s de l’application $\tilde{\pi}: \tilde{X}_\pi \to S$ composée de $\pi$ et de l’application canonique $\tilde{X}_\pi \to X$, est $\tilde{X}_s$ (10.2.4). On appelle forme différentielle $\pi$-tordue sur X une forme différentielle $T(X/S)$-tordue (10.3.3).

11.4.3 (« S-orientation d’un S-morphisme »). Soit $X'$ une variété munie d’une submersion $\pi': X' \to S$ dont les fibres $X_s$ sont pures de dimension finie $n'$, et soit $\varphi: X' \to X$ un morphisme tel que $\pi' = \pi \circ \varphi$. On appelle S-orientation de $\varphi$ un morphisme $\tilde{\varphi}: \tilde{X}'_\pi \to \tilde{X}_\pi$, commutant à l’action du groupe $\{ \pm 1 \}$ et tel que le diagramme

$$
\begin{array}{ccc}
\tilde{X}'_\pi & \xrightarrow{\tilde{\varphi}} & \tilde{X}_\pi \\
| & & | \\
X' & \xrightarrow{\varphi} & X
\end{array}
$$

soit commutatif. La donnée d’une S-orientation de $\varphi$ permet, comme en 10.4.2, d’identifier les fibrés $\tilde{R}_{\pi'}$ et $\varphi^*(\tilde{R}_\pi)$ et de définir l’image réciproque d’une forme différentielle $\pi$-tordue par le morphisme S-orienté $\varphi$: c’est une forme différentielle $\pi'$-tordue sur $X'$.

11.4.4. Soit A une pièce de X telle que la restriction de $\pi$ à $\partial A$ soit une submersion. Pour tout $s \in S$, la fibre $X_s = \pi^{-1}(s)$ est une sous-variété de X transversale à $\partial A$ et $A \cap X_s$ est une pièce de $X_s$, notée $A_s$, de bord $\partial A \cap X_s$.

Soit i l’injection canonique de $\partial A$ dans X. Il existe une S-orientation $\tilde{i}$ et une seule de i telle que, pour tout $s \in S$, la restriction de $\tilde{i}$ à $(\partial A_s)^*$ (identifié à la fibre en s de la submersion $\partial \tilde{A}_{\pi|\partial A} \to S$) soit l’orientation définie en 11.2.1 de l’injection canonique de $\partial A_s$ dans $X_s$. Si $\omega$ est une forme différentielle $\pi$-tordue sur X, l’image réciproque de $\omega$ par le morphisme i ainsi orienté est notée $\omega|\partial A$ (cf. 11.2.2).

11.4.5 (« Produit intérieur »). Soit $p$ un entier $\geqslant 0$ et soit $\omega$ une forme différentielle $n$-tordue de degré $n + p$ sur $X$, à valeurs dans un fibré vectoriel $E$ de base $X$. Soient $s \in S$ et $x \in X_s$; on a $\omega(x) = \xi \otimes u$, où $\xi$ est une orientation de $T_x(X_s) = T(X/S)_x$, identifiée à un élément de $(\tilde{R}_{X_s})_x = (\tilde{R}_\pi)_x$ (10.3.2), et où $u$ est une application $(n + p)$-linéaire alternée de $T_x(X)$ dans $E_x$. Soient $t_1, \ldots, t_p$ des vecteurs tangents à $S$ en $s$. Posons

$$
\theta(x) = \xi \otimes (u \wedge (t_1, \ldots, t_p)) \in (\tilde{R}_{X_s})_x \otimes (\mathrm{Alt}^n(T(X); E))_x
$$

(cf. 11.4.1). On définit ainsi une forme différentielle tordue $\theta : x \mapsto \theta(x)$ de degré $n$ sur $X_s$, à valeurs dans $E|X_s$. On la note $\omega \wedge (t_1, \ldots, t_p)$.

En particulier, soit $M$ un fibré vectoriel de classe $C^{r-1}$ de base $S$ et prenons $E = \pi^*(M)$. Le fibré $E|X_s$ s’identifie naturellement au fibré trivial de base $X_s$ défini par l’espace de Banach $M_s$ et la forme $\omega \wedge (t_1, \ldots, t_p)$ s’identifie à une forme différentielle tordue sur $X_s$, à valeurs dans $M_s$.

11.4.6. Conservons les notations précédentes (en particulier $E = \pi(*M)$) et supposons de plus que $X$ soit séparée et $\omega$ continue. Soit $A$ une pièce de $X$ telle que la restriction de $\pi$ à $\partial A$ soit une submersion et que la restriction de $\pi$ à l’intersection de $A$ et du support de $\omega$ soit propre. Pour $s \in S$ et $t_1, \ldots, t_p$ dans $T_s(S)$, la forme $\omega \wedge (t_1, \ldots, t_p)$ (11.4.5) est une forme différentielle tordue de degré $n$ sur $X_s$, continue, à valeurs dans l’espace de Banach $M_s$, et son support rencontre $A_s$ suivant un compact. Il existe une forme différentielle $\alpha$ et une seule de degré $p$ sur $S$, à valeurs dans le fibré vectoriel $M$, et telle que

$$
\alpha(s)(t_1, \ldots, t_p) = \int_{A_s} \omega \wedge (t_1, \ldots, t_p)
$$

quels que soient $s \in S$ et $t_1, \ldots, t_p$ dans $T_s(S)$. La forme $\alpha$ se note $\int_{\pi|A} \omega$ (ou simplement $\int_\pi \omega$ lorsque $A = X$); on dit qu’elle s’obtient en intégrant $\omega$ sur $A$ le long des fibres de $\pi$. Si $\omega$ est de classe $C^k$ ($0 \leq k \leq r - 1, k \leq \infty$), il en est de même de $\int_{\pi|A} \omega$.

Lorsque $\omega$ est une forme de degré $< n$, on convient que $\int_{\pi|A} \omega = 0$.

11.4.7. Conservons les hypothèses et notations précédentes.

a) Pour toute forme différentielle scalaire continue $\beta$ sur $S$, on a

$$
\int_{\pi|A} (\pi^*\beta) \wedge \omega = \beta \wedge \int_{\pi|A} \omega.
$$

b) Soient $\eta$ un champ de vecteurs continu sur $X$ et $\zeta$ un champ de vecteurs continu sur $S$, tels que $\eta$ soit $\pi$-lié à $\zeta$ (8.2.6). On a

$$
i(\zeta) \int_{\pi|A} \omega = \int_{\pi|A} i(\eta)\omega.
$$

c) Supposons de plus que $\eta, \zeta$ et $\omega$ soient de classe $C^1$, que l’on ait $\eta(x) \in T_x(\partial A)$ pour tout $x \in \partial A$ et que $M$ soit le fibré trivial défini par un espace de Banach $E$. On a

$$
\theta_\zeta \cdot \int_{\pi|A} \omega = \int_{\pi|A} \theta_\eta \cdot \omega,
$$

(cf. 8.4.2 et 10.3.4).

d) Si $\omega$ est de degré $n + p$ et de classe $C^1$, on a
$$
d \left( \int_{\pi|A} \omega \right) = \int_{\pi|A} d\omega + (-1)^p \int_{\pi|\partial A} \omega|_{\partial A}.
$$
e) Supposons que S soit réduite à un point. Les formes $\pi$-tordues sur X sont alors les formes tordues ordinaires (10.4.1). Si $\omega$ est de degré $n$, la forme $\int_{\pi|A} \omega$ de degré 0 sur S est la constante $\int_A \omega$ (10.4.3).

11.4.8. Soit $\pi': S \to S'$ une submersion telle que les fibres de $\pi'$ soient des sous-variétés pures de dimension finie constante $n'$. Posons $\pi'' = \pi' \circ \pi$; c'est une submersion de X sur S' dont les fibres sont des sous-variétés pures de dimension $m = n + n'$.

Soit $x \in X$. La suite
$$
0 \longrightarrow T(X/S)_x \xrightarrow{\mathrm{Id}} T(X/S')_x \xrightarrow{T_x(\pi)} T(S/S')_{\pi(x)} \longrightarrow 0
$$
est exacte. Il existe un isomorphisme $j$ et un seul du fibré vectoriel $\tilde{R}_{\pi} \otimes \pi^*(\tilde{R}_{\pi'})$ sur $\tilde{R}_{\pi''}$ tel que, si $\xi$ (resp. $\eta$) est une orientation de $T(X/S)_x$ (resp. de $(\pi^*T(S/S'))_x$) identifié à $T(S/S')_{\pi(x)}$, on ait $j(\xi \otimes \eta) = \eta \xi$ (le produit étant défini par la suite exacte précédente (10.2.1)).

Soit $M'$ un fibré vectoriel de base $S'$; posons $M = {\pi'}^*(M')$, et $E = \pi^*(M) = {\pi''}^*(M')$. Si $\omega$ est une forme différentielle $\pi''$-tordue sur X à valeurs dans E, l'isomorphisme $j$ permet de l'identifier à une forme $\pi$-tordue à valeurs dans $\pi^*(\tilde{R}_{\pi'}) \otimes E$, ou encore à valeurs dans $\pi^*(\tilde{R}_{\pi'} \otimes M)$.

Soit de plus A une pièce de X telle que $\pi|\partial A : \partial A \to S$ soit une submersion ; il en est alors de même de $\pi''|\partial A : \partial A \to S'$. Supposons en outre que $\omega$ soit continue et que la restriction de $\pi''$ à $A \cap \operatorname{Supp} \omega$ soit propre; il en est alors de même de la restriction de $\pi$ à $A \cap \operatorname{Supp} \omega$. On peut considérer d'une part la forme différentielle $\int_{\pi''|A} \omega$ sur $S'$, qui est une forme à valeurs dans $M'$, d'autre part la forme différentielle $\int_{\pi|A} \omega$ sur S, qui est une forme à valeurs dans $\tilde{R}_{\pi'} \otimes M$, ou encore une forme $\pi'-$tordue à valeurs dans $M = {\pi'}^*(M')$. De plus, $\pi(A)$ est une sous-variété ouverte de S et la restriction de $\pi'$ à $\pi(A) \cap \operatorname{Supp} \int_{\pi|A} \omega$ est propre. La forme différentielle $\int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega$ est définie; c'est une forme différentielle sur $S'$, à valeurs dans $M'$. On a
$$
\int_{\pi' \circ \pi|A} \omega = \int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega.
$$
Si $A = X$, on a
$$
\int_{\pi' \circ \pi} \omega = \int_{\pi'} \int_{\pi} \omega.
$$

[^1]: Cette terminologie provient de ce que A est naturellement muni d'une structure de «variété à bord», de bord $\partial A$. Pour la définition de cette catégorie, ainsi que pour celle, plus générale, de la catégorie des «variétés à bord anguleux», le lecteur pourra se reporter à H. CARTAN, Séminaire 1961/62, Topologie Différentielle, exposés 1-2-3 (par A. DOUADY), Benjamin, New York, 1969. Signalons qu'on peut montrer que toute «variété à bord» dont le bord est paracompact est isomorphe à une pièce fermée d'une variété.
[^2]: Le lecteur qui s’intéresse à des cas plus généraux pourra consulter H. WHITNEY, Geometric Integration Theory, Chap. III, § 18 (Princeton Univ. Press, 1957).
