---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 9
section_title: Algèbres de Clifford
lang: fr
source: alg-ix-fr
pdf_pages: 0137-0158
extraction: ocr
subsections:
    - "no": 1
      title: Définition et propriété universelle de l’algèbre de Clifford.
      page: 0
      pdf_page: 137
    - "no": 2
      title: Quelques opérations dans l’algèbre tensorielle.
      page: 0
      pdf_page: 139
    - "no": 3
      title: Base de l’algèbre de Clifford.
      page: 0
      pdf_page: 141
    - "no": 4
      title: Structure de l’algèbre de Clifford.
      page: 0
      pdf_page: 144
    - "no": 5
      title: Groupe de Clifford.
      page: 0
      pdf_page: 148
statements: 24
exercises: 0
content_sha256: e2c4e69fdd13a741a502879f76e3145e94bb7fd20f1e9d2440ff7b50608cba33
---

## § 9. Algèbres de Clifford

Dans ce paragraphe, nous supposerons l’anneau $\mathbf{A}$ commutatif. Nous désignerons par $Q$ une forme quadratique sur le $\mathbf{A}$-module $E$, et par $\Phi$ la forme bilinéaire associée ($§\ 3$, no 4).

### 1. Définition et propriété universelle de l’algèbre de Clifford.

#### Définition 1 {#alg-ix-s9-def-1 .statement}

On appelle algèbre de Clifford de $Q$ et on note $C(Q)$ l’algèbre quotient de l’algèbre tensorielle $T(E)$ du module $E$ par l’idéal bilatère (noté $I(Q)$) engendré par les éléments de la forme $x \otimes x - Q(x)\cdot 1$ $(x \in E)$.

Nous noterons $\rho_Q$ (ou simplement $\rho$ quand aucune confusion n’est à craindre) l’application de $E$ dans $C(Q)$ composée de l’application canonique de $E$ dans $T(E)$ et de l’application canonique $\sigma$ de $T(E)$ sur $C(Q)$; l’application $\rho_Q$ est dite canonique. Remarquons que $C(Q)$ est engendrée par $\rho_Q(E)$, et que, pour $x \in E$, on a

$$
\rho(x)^2 = Q(x)\cdot 1;
$$

d’où, en remplaçant $x$ par $x + y$ ($x,\ y$ dans $E$)

$$
\rho(x)\rho(y) + \rho(y)\rho(x) = \Phi(x,\ y)\cdot 1
$$

#### Exemple {#alg-ix-s9-n1-exa-1 .statement}

Si $E$ admet une base composée d’un seul élément $e$, $T(E)$ est isomorphe à l’algèbre de polynômes $\mathbf{A}[X]$, et $C(Q)$ est une extension quadratique de $\mathbf{A}$, ayant pour base $(1,\ u)$, où $u$ est l’élément $u = \rho(e)$ et vérifie $u^2 = Q(e)$.

Notons $T^h$ la puissance tensorielle $h$-ème $\bigotimes^h E$ dans $T(E)$, et soit $T^+$ (resp. $T^-$) la somme des $T^h$ pour $h$ pair (resp. impair).

Comme $T(E)$ est somme directe de $T^+$ et $T^-$ et que $I(Q)$ est engendré par des éléments de $T^+$, $I(Q)$ est somme directe de $T^+ \cap I(Q)$ et $T^- \cap I(Q)$, et $C(Q)$ est somme directe des deux sous-modules $C^+(Q) = \sigma(T^+)$ et $C^-(Q) = \sigma(T^-)$ (que l’on note aussi $C^+$ et $C^-$). Les éléments de $C^+$ seront dits pairs (resp. impairs). On a les relations

(3) $C^+C^+ \subset C^+, \quad C^+C^- \subset C^-, \quad C^-C^+ \subset C^-, \quad C^-C^- \subset C^+$.

En particulier $C^+$ est une sous-algèbre de $C(Q)$.

#### Proposition 1 {#alg-ix-s9-prop-1 .statement}

*Soit f une application linéaire de E dans une algèbre D sur A telle que $f(x)^2 = Q(x).1$ pour tout $x \in E$. Il existe un homomorphisme $\bar{f}$ et un seul de $C(Q)$ dans D tel que $f = \bar{f} \circ \rho_Q$.

L’unicité de $\bar{f}$ résulte de ce que $C(Q)$ est engendrée par $\rho_Q(E)$. Soit $h$ l’unique homomorphisme de $T(E)$ dans D qui prolonge $f$ ($h$ est défini par $h(x_1 \otimes \cdots \otimes x_n) = f(x_1) \ldots f(x_n)$). On a

$$
h(x \otimes x - Q(x).1) = (f(x)^2 - Q(x)).1 = 0,
$$

et par suite $h$ s’annule sur $I(Q)$ et définit par passage au quotient l’homomorphisme $\bar{f}$ cherché.

La prop. 1 exprime que $C(Q)$ est solution d’un problème d’application universelle (*Ens.*, chap. IV, § 3, n° 1).

Prenons en particulier pour D l’algèbre opposée de $C(Q)$ et pour $f$ l’application $\rho$; la prop. 1 entraîne qu’il existe un anti-automorphisme $\beta$ et un seul de $C(Q)$ dont la restriction à $\rho(E)$ soit l’identité ; on l’appelle l’antiautomorphisme *principal* de $C(Q)$. Il est clair que $\beta^2 = 1$.

D’autre part soient $Q'$ une forme quadratique sur un A-module $E'$ et $f$ une application linéaire de $E$ dans $E'$ telle que $Q' \circ f = Q$. On a $\rho_Q(f(x))^2 = Q'(f(x)).1 = Q(x).1$, et par suite il existe un homomorphisme $C(f)$ et un seul de $C(Q)$ dans $C(Q')$ tel que $C(f) \circ \rho_Q = \rho_{Q'} \circ f$. Si $f$ est l’identité, $C(f)$ est l’identité ; si $Q''$ est une forme quadratique sur un A-module $E''$ et $g$ une application linéaire de $E'$ dans $E''$ telle que $Q'' \circ g = Q'$, on a $C(g \circ f) = C(g) \circ C(f)$. Lorsque $E'$ est un sous-module de $E$ et $f$ l’injection canonique de $E'$ dans $E$ (de sorte que $Q'$ est la restriction de $Q$ à $E'$), on dit que $C(f)$ est l’homomorphisme *canonique* de $C(Q')$ dans $C(Q)$.

Prenons en particulier Q' = Q et pour f l’application x → -x ; on voit qu’il existe un automorphisme α et un seul de C(Q) tel que $\alpha \circ \rho = -\rho$; on l’appelle l’automorphisme principal de C(Q). Il est clair que $\alpha^2 = 1$, et que la restriction de $\alpha$ à $C^+$ (resp. $C^-$) est l’identité (resp. l’application $u \to -u$).

#### Proposition 2 {#alg-ix-s9-prop-2 .statement}

Soient $A'$ un anneau commutatif, $\varphi$ un homomorphisme de A dans $A'$, Q’ la forme quadratique sur $E' = A' \otimes_A E$ déduite de Q par extension des scalaires ($§ 3$, no 4, prop. 3). Il existe un isomorphisme j et un seul de l’algèbre $A' \otimes_A C(Q)$ sur $C(Q')$ tel que $j (1 \otimes \rho_Q(x)) = \rho_{Q'}(1 \otimes x)$ pour tout $x \in E$.

Il suffit de démontrer que l’algèbre $C' = A' \otimes C(Q)$ et l’application $1 \otimes \rho_Q$ de $E'$ dans $C'$ forment une solution du même problème d’application universelle que $C(Q')$ et $\rho_{Q'}$. Or, soient D’ une algèbre sur $A'$ et $f'$ une application $A'$-linéaire de $E'$ dans D’ telle que $f'(x')^2 = Q'(x').1$ pour tout $x' \in E'$. L’application $g : x \to f' (1 \otimes x)$ de E dans D’ (considéré comme A-module grâce à l’homomorphisme $\varphi$) est A-linéaire et on a $g(x)^2 = Q' (1 \otimes x).1 = Q(x).1$ pour tout $x \in E$. Il existe donc un A-homomorphisme $\overline{g}$ et un seul de $C(Q)$ dans D’ tel que $\overline{g}(\rho_Q(x)) = f'(1 \otimes x)$. Par suite il existe un $A'$-homomorphisme $\overline{f}'$ et un seul de $C'$ dans D’ tel que $\overline{f}'(1 \otimes \rho_Q(x)) = f'(1 \otimes x)$ pour tout $x \in E$; par linéarité il en résulte que $\overline{f}'((1 \otimes \rho_Q)(x')) = f'(x')$ pour tout $x' \in E'$. CQFD.

### 2. Quelques opérations dans l’algèbre tensorielle.

Dans ce no nous désignerons par $e_x$ ($x \in E$) l’application linéaire $u \to x \otimes u$ de l’algèbre tensorielle T(E) dans elle-même.

#### Lemme 1 {#alg-ix-s9-lem-1 .statement}

Soit $f$ un élément du dual $E^*$ de E. Il existe une application linéaire $i_f$ et une seule de T(E) dans elle-même telle que
$$
i_f(1) = 0 \tag{4}
$$
$$
i_f \circ e_x + e_x \circ i_f = f(x).I \tag{5}
$$
pour tout $x \in E$
(où I désigne l’application identique). L’application $f \to i_f$ de $E^*$ dans $\mathcal{L}(T(E))$ est linéaire. On a $i_f(T^n) \subset T^{n-1}$, $(i_f)^2 = 0$, et $i_f \circ i_g + i_g \circ i_f = 0$ pour $f, g$ dans $E^*$. L’application $i_f$ est nulle sur la sous-algèbre de

T(E) engendrée par le noyau de f. L’idéal I(Q) est stable par $i_f$; par passage au quotient $i_f$ définit donc une application linéaire (notée encore $i_f$) de $C(Q)$ dans elle-même.

En effet la formule (5) s’écrit

$$
i_f(x \otimes u) = -x \otimes i_f(u) + f(x) \cdot u \quad (x \in E,\ u \in T(E)).
$$

Comme (4) détermine complètement $i_f$ sur $T^0$, et que (6) détermine $i_f$ sur $T^n$ si on connaît ses valeurs sur $T^{n-1}$, l’unicité de $i_f$ est démontrée. D’autre part, pour $x \in E$ et $u \in T^{n-1}$, le second membre de (6) est bilinéaire sur $E \times T^{n-1}$; ceci démontre l’existence de $i_f$ par récurrence sur $n$ (chap. III, § 1, no 2) et prouve aussi, par récurrence sur $n$, que $i_f(T^n) \subset T^{n-1}$. Si $f = ag + bh$ (a, b dans A, g, h dans E*) il est clair que $ai_g + bi_h$ vérifie (4) et (5), donc est égal à $i_f$. On a

$$
(i_f)^2 \circ e_x = -i_f \circ e_x \circ i_f + f(x)i_f = e_x \circ (i_f)^2
$$

et, comme $(i_f)^2(1) = 0$, on en déduit par récurrence sur $n$ que $(i_f)^2$ est nul sur $T^n$. En remplaçant $f$ par $f + g$, la relation $(i_f)^2 = 0$ donne $i_f \circ i_g + i_g \circ i_f = 0$. Un raisonnement par récurrence analogue aux précédents montre que $i_f$ est nulle sur la sous-algèbre engendrée par le noyau de $f$. Enfin (6) entraîne que l’ensemble des éléments $u$ de $I(Q)$ tels que $i_f(u) \in I(Q)$ est un idéal à gauche de $T(E)$; de plus, si $u = (x \otimes x - Q(x) \cdot 1) \otimes \nu$ ($x \in E,\ \nu \in T(E)$), on a

$$
\begin{align*}
i_f(u) &= f(x)x \otimes \nu - x \otimes i_f(x \otimes \nu) - Q(x)i_f(\nu) \\
&= f(x)x \otimes \nu - f(x)x \otimes \nu + x \otimes x \otimes i_f(\nu) - Q(x)i_f(\nu) \\
&= (x \otimes x - Q(x) \cdot 1) \otimes i_f(\nu);
\end{align*}
$$

donc $I(Q)$ est stable par $i_f$, et la dernière assertion s’ensuit. CQFD.

Soit F une forme bilinéaire sur E ; dans le reste de ce paragraphe nous désignerons par $i_x^F$ ($x \in E$) l’application $i_f$ correspondant à la forme linéaire $f : y \to F(x, y)$ sur E.

#### Lemme 2 {#alg-ix-s9-lem-2 .statement}

Il existe une application linéaire $\lambda_F$ et une seule de $T(E)$ dans elle-même telle que

$$
\begin{align*}
\lambda_F(1) &= 1 \\
\lambda_F \circ e_x &= (e_x + i_x^F) \circ \lambda_F \qquad (x \in E).
\end{align*}
$$

Quel que soit $f \in E^*$, on a

$$
\lambda_F \circ i_f = i_f \circ \lambda_F.
$$

En effet la formule (8) équivaut à

$$
\lambda_F(x \otimes u) = x \otimes \lambda_F(u) + i_x^F(\lambda_F(u)) \quad (x \in E, u \in T(E)).
$$

Comme (7) détermine entièrement $\lambda_F$ sur $T^0$, et que (10) détermine $\lambda_F$ sur $T^n$ si on connaît ses valeurs sur $T^{n-1}$, l’unicité de $\lambda_F$ est démontrée. D’autre part, pour $x \in E$ et $u \in T^{n-1}$, le second membre de (10) est bilinéaire sur $E \times T^{n-1}$; ceci démontre l’existence de $\lambda_F$ par récurrence sur $n$. Il reste à démontrer (9), ce que nous ferons par récurrence ; les deux membres de (9) sont nuls sur $T^0$ ; supposons (9) vraie sur $\sum_{h=0}^{n-1} T^h$; on a alors, pour $x \in E$ et $u \in T^{n-1}$ :

$$
\begin{align*}
(\lambda_F \circ i_f)(x \otimes u) &= (-\lambda_F \circ e_x \circ i_f + f(x)\lambda_F)(u) \\
&= -(e_x + i_x^F) \circ \lambda_F \circ i_f(u) + f(x)\lambda_F(u) \\
&= -(e_x + i_x^F) \circ i_f \circ \lambda_F(u) + f(x)\lambda_F(u) \\
&= (i_f \circ e_x \circ \lambda_F - f(x)\lambda_F + i_f \circ i_x^F \circ \lambda_F + f(x)\lambda_F)(u) \\
&= (i_f \circ (e_x + i_x^F) \circ \lambda_F)(u) = (i_f \circ \lambda_F)(x \otimes u),
\end{align*}
$$

d’où notre dernière assertion.

#### Lemme 3 {#alg-ix-s9-lem-3 .statement}

Soient F et G deux formes bilinéaires sur E. On a $\lambda_F \circ \lambda_G = \lambda_{F+G}$. Pour toute forme bilinéaire F sur E, $\lambda_F$ est une bijection de $T(E)$ sur elle-même.

En effet, $\lambda_F \circ \lambda_G$ possède les propriétés caractéristiques (7) et (8) de $\lambda_{F+G}$ : on a $(\lambda_F \circ \lambda_G)(1) = 1$, et

$$
\begin{align*}
\lambda_F \circ \lambda_G \circ e_x &= \lambda_F \circ (e_x + i_x^G) \circ \lambda_G = (e_x + i_x^G + i_x^F) \circ \lambda_F \circ \lambda_G \\
&= (e_x + i_x^{F+G}) \circ \lambda_F \circ \lambda_G.
\end{align*}
$$

D’autre part, si $F = 0$, on a $i_x^F = 0$ pour tout $x \in E$, et par suite $\lambda_F = I$, ce qui entraîne que, pour toute F, on a $\lambda_F \circ \lambda_{-F} = \lambda_{-F} \circ \lambda_F = I$.

### 3. Base de l’algèbre de Clifford.

#### Proposition 3 {#alg-ix-s9-prop-3 .statement}

Soient Q et Q' deux formes quadratiques et F une forme bilinéaire sur E telles que $Q'(x) = Q(x) + F(x, x)$ pour tout $x \in E$. L’application $\lambda_F$ applique l’idéal $I(Q')$ sur l’idéal $I(Q)$, et définit un isomorphisme (noté $\overline{\lambda_F}$) du A-module $C(Q')$ sur le A-module $C(Q)$.

Comme $\lambda_F$ est une bijection dont $\lambda_{-F}$ est la bijection réciproque (lemme 3), il suffit de démontrer l’inclusion $\lambda_F(I(Q')) \subset I(Q)$. Comme $I(Q)$ est un idéal à gauche stable par $i_x^F$ (lemme 1), (8) montre que l’ensemble des $u \in T(E)$ tels que $\lambda_F(u) \in I(Q)$ est un idéal à gauche. Il suffit donc de démontrer que, quels que soient $u \in T(E)$ et $x \in E$, on a $\lambda_F(x \otimes x \otimes u - Q'(x)u) \in I(Q)$. Or, d’après (8) et le lemme 1, on a
$$
\lambda_F \circ e_x^2 = (e_x + i_x^F)^2 \circ \lambda_F = (e_x^2 + F(x, x)) \circ \lambda_F,
$$
d’où
$$
\begin{align*}
\lambda_F(x \otimes x \otimes u - Q'(x)u) &= (e_x^2 + F(x, x) - Q'(x)) \circ \lambda_F(u) \\
&= (x \otimes x - Q(x)) \otimes \lambda_F(u) \in I(Q).
\end{align*}
$$

#### Lemme 4 {#alg-ix-s9-lem-4 .statement}

Si la forme quadratique $Q$ est nulle, $C(Q)$ n’est autre que l’algèbre extérieure de $E$.

En effet l’algèbre extérieure de $E$ n’est autre que le quotient de $T(E)$ par l’idéal bilatère $J$ engendré par les éléments de la forme $a \otimes \nu \otimes a$ ($a \in E, \nu \in T(E)$) (chap. III, § 5, no 5 et no 9). Il est clair que $I(Q) \subset J$. Il suffit donc de montrer que $a \otimes \nu \otimes a \in I(Q)$. C’est évident si $\nu \in T^0$. Supposons cette assertion démontrée pour $\nu \in \sum_{h=0}^{n-1} T^h$, et soient $x \in E$ et $u \in T^{n-1}$; on a
$$
a \otimes x \otimes u \otimes a = (a + x) \otimes (a + x) \otimes u \otimes a
- a \otimes a \otimes u \otimes a - x \otimes a \otimes u \otimes a - x \otimes x \otimes u \otimes a
$$
et les quatre termes du second membre appartiennent à $I(Q)$.

Supposons en particulier que le module $E$ admette une base $(x_i)_{i \in L}$, et ordonnons totalement l’ensemble d’indices $L$. On sait (chap. III, § 5, no 6) que l’algèbre extérieure de $E$ admet comme base la famille formée des éléments $x_H$, où $H$ parcourt l’ensemble des parties finies de $L$ et où $x_H$ est l’élément $x_{h_1} \wedge \ldots \wedge x_{h_q}$, $(h_1, \ldots, h_q)$ désignant la suite strictement croissante des éléments de $H$.

D’autre part, considérons la forme bilinéaire $F$ définie par $F(x_i, x_j) = -\Phi(x_i, x_j)$ si $i > j$, $F(x_i, x_j) = 0$ si $i < j$ et $F(x_i, x_i) = -Q(x_i)$. Il est clair que $Q(x) + F(x, x) = 0$; avec les notations de la prop. 3, il résulte de cette proposition et du lemme 4 que $\bar{\lambda}_F$ est un isomorphisme de $\wedge E$ sur $C(Q)$, qui est donc un $A$-module libre. Démontrons, par récurrence sur le nombre d’éléments de $H$, que l’on a

$$
\bar{\lambda}_F(x_H) = \rho(x_{h_1}) \ldots \rho(x_{h_q})
$$

(où $(h_1, \ldots, h_q)$ est la suite strictement croissante des éléments de $H$). C’est évident si $H$ a 0 ou 1 élément. Supposons (11) vérifiée pour les parties ayant au plus $q - 1$ éléments. Considérons une partie $H$ à $q$ éléments, notons $j$ son plus petit élément, et écrivons $H = \{ j \} \cup K$, où $K$ est une partie à $q - 1$ éléments. On a, d’après (8) et l’hypothèse de récurrence

$$
\bar{\lambda}_F(x_H) = \bar{\lambda}_F(x_j \wedge x_K) = \rho(x_j) \bar{\lambda}_F(x_K) + i^F_{x_j}(\bar{\lambda}_F(x_K)) = x'_H + i^F_{x_j}(x'_K),
$$

en posant, pour toute partie finie $J$ de $L$, $x'_J = \rho(x_{j_1}) \ldots \rho(x_{j_s})$, où $(j_1, \ldots, j_s)$ est la suite croissante des éléments de $J$. Or, pour $i \in K$, $x_i$ appartient au noyau de la forme linéaire $y \to F(x_j, y)$, donc $i^F_{x_j}(x'_K) = 0$ (lemme 1). Ceci démontre le résultat cherché.

Nous avons donc démontré le théorème suivant :

#### Théorème 1 {#alg-ix-s9-thm-1 .statement}

*Supposons que le $A$-module $E$ admette une base $(x_i)_{i \in L}$, l’ensemble d’indices $L$ étant muni d’une structure d’ordre total. Pour toute partie finie $H$ de $L$, posons $x_H = \rho(x_{h_1}) \rho(x_{h_2}) \ldots \rho(x_{h_q})$, où $(h_1, \ldots, h_q)$ est la suite strictement croissante des éléments de $H$. Alors les éléments $x_H$ forment une base du $A$-module $C(Q)$.*

#### Corollaire 1 {#alg-ix-s9-thm-1-cor-1 .statement}

*Si $E$ est un module libre de dimension $n$, $C(Q)$ est un module libre de dimension $2^n$; de plus, si $n > 0$, $C^+$ et $C^-$ sont des modules libres de dimension $2^{n-1}$.

Ceci résulte aussitôt des propriétés des coefficients binomiaux.*

#### Corollaire 2 {#alg-ix-s9-thm-1-cor-2 .statement}

*Si $E$ est un module libre, l’application canonique $\rho$ de $E$ dans $C(Q)$ et l’application $a \to a.1$ de $A$ dans $C(Q)$ sont injectives.*

#### Corollaire 3 {#alg-ix-s9-thm-1-cor-3 .statement}

*Supposons que $E$ soit somme directe de deux sous-modules libres $E_1$ et $E_2$. Soient $Q_i$ la restriction de $Q$ à $E_i$ et $p_i$ l’application canonique de $C(Q_i)$ dans $C(Q)$ ($i = 1, 2$). Alors l’application linéaire $p$ de $C(Q_1) \otimes C(Q_2)$ dans $C(Q)$ déduite de l’application bilinéaire $(a, b) \to p_1(a)p_2(b)$ de $C(Q_1) \times C(Q_2)$ dans $C(Q)$ est une bijection.

Il suffit en effet de considérer la base de $E$ obtenue en prenant la réunion d’une base de $E_1$ et d’une base de $E_2$.

#### Corollaire 4 {#alg-ix-s9-thm-1-cor-4 .statement}

Les hypothèses et notations étant celles du cor. 3, supposons de plus que $E_1$ et $E_2$ soient orthogonaux, et transportons à $C(Q_1) \otimes C(Q_2)$, au moyen de la bijection $p$, la structure d’algèbre de $C(Q)$. Si $a_i$ et $b_i$ sont des éléments pairs ou impairs de $C(Q_i)$ ($i = 1,\ 2$), on $a\ (a_1 \otimes a_2)(b_1 \otimes b_2) = \varepsilon(a_1b_1) \otimes (a_2b_2)$, avec $\varepsilon = 1$ sauf si $a_2$ et $b_1$ sont impairs, auquel cas $\varepsilon = -1$.

Il suffit en effet de démontrer que $p_2(a_2)p_1(b_1) = \varepsilon p_1(b_1)p_2(a_2)$, et on peut, pour cela, supposer que $p_2(a_2)$ (resp. $p_1(b_1)$) est un produit $x_1 \ldots x_h$ (resp. $y_1 \ldots y_k$) d’éléments de $\rho_Q(E_2)$ (resp. $\rho_Q(E_1)$). Comme $E_1$ et $E_2$ sont orthogonaux, on a

$$
x_iy_j + y_jx_i = \Phi(x_i, y_j) = 0,
$$

d’où

$$
x_1 \ldots x_h y_1 \ldots y_k = (-1)^{hk} y_1 \ldots y_k x_1 \ldots x_h.
$$

Les conclusions des cor. 3 et 4 restent vraies si on omet l’hypothèse que $E_1$ et $E_2$ sont des modules libres (cf. exerc. 1).

### 4. Structure de l’algèbre de Clifford.

Dans ce n°, nous supposerons que $A$ est un corps, que $E$ est un espace vectoriel de dimension finie $m$ sur $A$, et que la forme quadratique $Q$ est non dégénérée (ce qui, d’après le th. 1 du § 5, n° 1, exige que $m$ soit pair si $A$ est de caractéristique 2). Puisque $E$ est libre, l’application canonique $\rho$ est injective (n° 3, cor. 2 du th. 1). Nous identifierons désormais $E$ et son image dans $C(Q)$.

#### Théorème 2 {#alg-ix-s9-thm-2 .statement}

Supposons que la dimension de $E$ soit un nombre pair $m = 2r$ et que $Q$ soit neutre (§ 4, n° 2). Alors l’algèbre $C(Q)$ est séparable (chap. VIII, § 7, n° 5, déf. 1) et est isomorphe à l’algèbre des endomorphismes d’un espace vectoriel de dimension $2^r$ sur $A$. De plus si $m > 0$, $C^+(Q)$ est séparable et est composée directe de deux idéaux isomorphes à l’algèbre des endomorphismes d’un espace vectoriel de dimension $2^{r-1}$ sur $A$.

En effet, comme Q est neutre, on peut décomposer E en somme directe de deux sous-espaces N et P totalement singuliers de dimensions r (§ 4, no 2, cor. 1 de la prop. 2). La restriction de Q à N étant nulle, la sous-algèbre S de C(Q) engendrée par N s’identifie à l’algèbre extérieure de N (no 3, lemme 4). Pour $n \in \mathbf{N}$, nous noterons $e'_n$ l’application $t \to nt$ de S dans elle-même.

Soit $(n_1, \ldots, n_r)$ une base de N ; nous noterons $(p_1, \ldots, p_r)$ la base de P telle que $\Phi(n_i, p_j) = \delta_{ij}$ (§ 4, no 2, prop. 2). Pour $p \in P$, nous noterons $p'$ la forme linéaire $n \to \Phi(n, p)$ sur N, et $i_p$ l’endomorphisme de S déduit par passage au quotient de l’endomorphisme $i_{p'}$ de T(N) associé à $p'$ comme il a été dit au lemme 1 du no 2. On a, d’après (5),

$$
e'_n \circ i_p + i_p \circ e'_n = \Phi(n, p) \qquad (n \in \mathbf{N}, \ p \in \mathbf{P}).
$$

Posons, pour $x = n + p \in E$ (avec $n \in \mathbf{N}$ et $p \in \mathbf{P}$), $s(x) = e'_n + i_p$. Il est clair que s est une application linéaire de E dans $\mathcal{L}(S)$. Comme on a
$$
s(x)^2 = (e'_n + i_p)^2 = Q(n) + \Phi(n, p) = Q(x)
$$
en vertu de (12) et du lemme 1 (no 2), s se prolonge en un homomorphisme (que nous noterons encore s) de C(Q) dans $\mathcal{L}(S)$ (no 1, prop. 1). Nous allons montrer que cet homomorphisme est surjectif, ce qui, puisque C(Q) et $\mathcal{L}(S)$ sont toutes deux de dimension $2^{2r}$, entraînera que s est un isomorphisme et démontrera notre première assertion.

Notons en effet I l’intervalle $[1, r]$. Pour toute partie H de I, nous poserons $H' = I - H$ et nous désignerons par $n_H$ (resp. $p_H$) le produit des $n_i$ (resp. $p_i$) pour $i \in H$, rangés dans l’ordre croissant des indices. Rappelons que les $n_H$ forment une base de S (no 3, th. 1). Posons enfin, pour deux parties quelconques H, K de I, $x_{H, K} = n_H p_I n_K$. Nous allons montrer que les éléments $s(x_{H, K})$ de $s(C(Q))$ engendrent $\mathcal{L}(S)$. Or, si $j \notin H$, on a $s(p_j)(n_H) = i_{p_j}(n_H) = 0$ d’après le lemme 1, puisque les $n_i$ pour $i \in H$ appartiennent au noyau de la forme linéaire $n \to \Phi(n, p_j)$ sur N ; d’autre part on a
$$
s(p_j)(n_j n_H) = (i_{p_j} \circ e'_{n_j})(n_H) = \Phi(p_j, n_j)n_H - n_j \cdot s(p_j)(n_H) = n_H
$$
(d’après (12)). Comme s est un homomorphisme, on en déduit, pour deux parties quelconques H, K de I, que $s(p_K)(n_H) = 0$ si $K \not\subset H$, et que $s(p_K)(n_H) = \pm n_{H-K}$ si $K \subset H$. Comme, pour $M \subset I$ et $L \subset I$, on a par définition $s(n_M)(n_L) = n_M n_L$, et que $n_M n_L$ est nul si $M \cap L \neq \emptyset$ et est égal à $\pm n_{M \cup L}$ dans le cas contraire, on conclut de ce qui précède que, pour des parties quelconques $H, K, L$ de $I$, $s(x_{H,K})(n_L) = s(n_H)s(p_I)s(n_{K'}) (n_L)$ est nul si $K \neq L$ et est égal à $\pm n_H$ si $K = L$. Ceci montre que les $s(x_{H,K})$ engendrent $\mathcal{L}(S)$ et termine la démonstration de la première assertion.

Pour démontrer la seconde assertion, posons $S^+ = S \cap C^+$ et $S^- = S \cap C^-$; il est clair que $S^+$ (resp. $S^-$) est le sous-espace de $S$ engendré par les $n_H$ tels que $H$ ait un nombre pair (resp. impair) d’éléments, que $S$ est somme directe de $S^+$ et $S^-$, et que $s(C^+)$ laisse $S^+$ et $S^-$ stables. Par suite $s$ applique $C^+$ dans une sous-algèbre de $\mathcal{L}(S)$, isomorphe au produit $\mathcal{L}(S^+) \times \mathcal{L}(S^-)$; la restriction de $s$ à $C^+$ est un isomorphisme de $C^+$ sur cette sous-algèbre, puisque $s$ est injective et que $C^+$ et $\mathcal{L}(S^+) \times \mathcal{L}(S^-)$ sont toutes deux de dimension $2^{2r-1}$ (no 2, cor. 1 du th. 1). CQFD.

#### Corollaire {#alg-ix-s9-n4-cor-1 .statement}

*Si m est pair, mais Q d’indice quelconque, l’algèbre C(Q) est une algèbre centrale simple de dimension $2^m$. De plus, si $m > 0$, la sous-algèbre $C^+(Q)$ est séparable, et son centre Z est de dimension 2 sur A. Lorsque Z est un corps, Z est une extension quadratique séparable de A et $C^+(Q)$ est simple; sinon, Z est composé direct de deux corps isomorphes à A, et $C^+(Q)$ est alors composée directe de deux sous-algèbres simples de dimensions $2^{m-2}$.

En effet, soient $A'$ la clôture algébrique de A, et $Q'$ la forme quadratique sur $E' = A' \otimes_A E$ déduite de Q par extension des scalaires. On a vu que $C(Q')$ est isomorphe à $A' \otimes_A C(Q)$ (prop. 2), et il est clair que $C^+(Q')$ est isomorphe à $A' \otimes_A C^+(Q)$. Comme $Q'$ est neutre ($§ 4$, no 2, cor. 2 de la prop. 3), le corollaire est une conséquence immédiate du th. 2 et des théorèmes de permanence du chap. VIII, $§ 7$.

#### Remarque 1 {#alg-ix-s9-n4-rem-1 .statement}

Comme l’algèbre $C(Q)$ est simple, elle n’a qu’une seule classe de représentations irréductibles ; on les appelle les *représentations spinorielles* ; quand on fixe son attention sur une de ces représentations, soit $\tau$, les éléments de l’espace où s’effectue $\tau$ répondent au nom de *spineurs*. Si Q est neutre, la restriction de $\tau$ à $C^+(Q)$ est, comme celle de $s$, somme de deux représentations absolument irréductibles inéquivalentes; les éléments des sous-espaces où s’effectuent ces deux représentations sont appelés semi-spineurs. Dans le cas général, si $C^+(Q)$ n’est pas simple, la restriction de $\tau$ à $C^+(Q)$ doit, puisqu’elle est fidèle, contenir des sous-représentations appartenant à chacune des deux classes de représentations irréductibles de $C^+(Q)$, donc est somme de deux représentations absolument irréductibles inéquivalentes, puisqu’il en est ainsi après extension des scalaires à la clôture algébrique $A'$ de $A$. Par contre, si $C^+(Q)$ est simple, elle n’a qu’une seule classe de représentations irréductibles, et la restriction de $\tau$ à $C^+(Q)$ est donc irréductible, puisqu’elle se décompose par extension des scalaires à $A'$ en deux représentations non équivalentes.

#### Remarque 2 {#alg-ix-s9-n4-rem-2 .statement}

Supposons $A$ de caractéristique $\neq 2$, et soit $(x_1, \ldots, x_m)$ ($m = 2r$) une base orthogonale de $E$. Posons
$$
z = 2^r x_1 \ldots x_m \in C(Q);
$$
comme $x_i x_j + x_j x_i = 0$ pour $i \neq j$, on a $zx_j = -x_j z$, ce qui entraîne que $z$ appartient au centre $Z$ de $C^+(Q)$ sans appartenir à $A$. On a
$$
z^2 = 2^{2r}(-1)^r Q(x_1) \ldots Q(x_m) = (-1)^r D
$$
en désignant par $D$ le discriminant de $\Phi$ par rapport à la base $(x_j)$ (cf. exerc. 9).

#### Théorème 3 {#alg-ix-s9-thm-3 .statement}

*Supposons que la dimension de $E$ soit un nombre impair $m = 2r + 1$ (donc que $A$ soit de caractéristique $\neq 2$).*

a) *L’algèbre $C^+(Q)$ est centrale simple. Si $Q$ est d’indice maximum $r$, $C^+(Q)$ est isomorphe à l’algèbre des endomorphismes d’un espace vectoriel de dimension $2^r$ sur $A$.*

b) *L’algèbre $C(Q)$ est séparable. Son centre $Z$ est de dimension 2, et $C(Q)$ est isomorphe à $Z \otimes_A C^+(Q)$, donc est simple ou composée directe de deux sous-algèbres simples.*

Soient en effet $x_0$ un vecteur non isotrope de $E$, et $F$ l’orthogonal de $x_0$; notons $Q_1$ la forme quadratique $y \to -Q(x_0)Q(y)$ sur $F$; il est clair que $Q_1$ est non dégénérée. Comme $x_0 y = -y x_0$ (pour $y \in F$), on a $(x_0 y)^2 = -Q(x_0)Q(y) = Q_1(y)$, et par suite l’application $y \to x_0 y$ de $F$ dans $C^+(Q)$ se prolonge en un homomorphisme $h$ de $C(Q_1)$ dans $C^+(Q)$ (n° 1, prop. 1). Or $C(Q_1)$ est simple (th. 2) et a même dimension $2^{2r}$ que $C^+(Q)$; ceci entraîne, puisque $h(1) = 1$, que $h$ est un isomorphisme. De plus, si $Q$ est d’indice $r$, on peut choisir $x_0$ de telle sorte que $Q_1$ soit aussi d’indice $r$ (§ 4, n° 2, prop. 3), ce qui démontre $a$.

Soit maintenant $(x_1, \ldots, x_{2r})$ une base orthogonale de $F$; posons $z = x_0 x_1 \ldots x_{2r}$. On vérifie immédiatement que $z$ commute avec $x_j$ pour $j = 0, \ldots, 2r$, donc appartient au centre de $C(Q)$. Soit $Z$ le sous-espace de $C(Q)$ engendré par $1$ et $z$; c’est une sous-algèbre du centre de $C(Q)$ et une extension quadratique de $A$, car $z$ est impair et $z^2$ est égal au scalaire $(-1)^r Q(x_0) \ldots Q(x_{2r})$. Considérons l’homomorphisme $\theta$ de $Z \otimes_A C^+(Q)$ dans $C(Q)$ défini par $\theta(u \otimes v) = uv$. Comme $z \in C^-$ et est inversible, l’application $u \to zu$ est un isomorphisme du module $C^+$ sur $C^-$, ce qui entraîne que $\theta(Z \otimes C^+)$ contient $C^+$ et $C^-$, donc coïncide avec $C(Q)$. Comme $Z \otimes C^+$ et $C(Q)$ ont même dimension $2^{2r+1}$, $\theta$ est un isomorphisme ; ceci démontre $b$, compte tenu des résultats du chap. VIII, § 7.

#### Remarque {#alg-ix-s9-n4-rem-3 .statement}

Le discriminant $D$ de $\Phi$ par rapport à la base $(x_j)_{(j=0,\ldots,2r)}$ est égal à $2^{2r+1} Q(x_0) \ldots Q(x_{2r})$. Par suite $Z$ est engendré par $1$ et par l’élément impair $z' = 2^{r+1} z$ tel que ${z'}^2 = (-1)^r 2D$. L’algèbre $C(Q)$ est donc simple si et seulement si $2(-1)^r D$ n’est pas un carré dans $A$.

### 5. Groupe de Clifford.

On suppose, dans ce n°, que $A$ est un corps, que $E$ est de dimension finie $m$, et que $Q$ est non dégénérée. On identifie $E$ avec son image canonique dans $C(Q)$.

#### Définition 2 {#alg-ix-s9-def-2 .statement}

On appelle groupe de Clifford de $Q$ (resp. groupe de Clifford spécial de $Q$), le groupe multiplicatif des éléments inversibles $s$ de $C(Q)$ (resp. $C^+(Q)$) tels que $sEs^{-1} = E$.

Dans ce n° nous noterons $G$ et $G^+$ le groupe de Clifford et le groupe de Clifford spécial de $Q$. Il est clair que l’on a $G^+ = G \cap C^+(Q)$.

#### Théorème 4 {#alg-ix-s9-thm-4 .statement}

Posons, pour $s \in G$ et $x \in E$, $\varphi(s).x = sx s^{-1}$.

a) L’application $\varphi$ est un homomorphisme de $G$ dans le groupe orthogonal $O(Q)$ de $Q$ et son noyau est l’ensemble des éléments inversibles du centre $Z$ de $C(Q)$.

b) L’ensemble $E \cap G$ est l’ensemble des vecteurs non singuliers de $E$; pour $x \in E \cap G$, $-\varphi(x)$ est la symétrie par rapport à l’hyperplan orthogonal à $x$.

c) Si $\dim(E)$ est paire, on a $\varphi(G) = O(Q)$, $\varphi(G^+)$ est d’indice 2 dans $O(Q)$ si $E \neq \{0\}$, et est égal à $SO(Q)$ si $A$ est de caractéristique $\neq 2$.

d) Si $\dim(E)$ est impaire (ce qui entraîne que $A$ est de caractéristique $\neq 2$), on a $\varphi(G) = \varphi(G^+) = SO(Q)$.

On a en effet $Q(sxs^{-1}) = (sxs^{-1})^2 = sx^2 s^{-1} = Q(x)$ pour $s \in G$ et $x \in E$, ce qui montre que $\varphi(s) \in O(Q)$. Pour que $\varphi(s) = 1$, il faut et il suffit que $s$ commute avec les éléments de $E$, c’est-à-dire appartienne au centre $Z$ de $C(Q)$. Ceci démontre a).

Pour qu’un élément $x$ de $E$ appartienne à $G$, il faut qu’il soit inversible, c’est-à-dire que ce soit un vecteur non singulier (puisque $x^2 = Q(x)$). S’il en est ainsi, on a $x^{-1} = Q(x)^{-1} x$, d’où, pour tout $y \in E$,
$$ xy x^{-1} = Q(x)^{-1} xy x = Q(x)^{-1} x (\Phi(x, y) - xy) = - (y - \Phi(x, y) Q(x)^{-1} x); $$
ceci démontre b) (§ 6, no 4).

#### Lemme 5 {#alg-ix-s9-lem-5 .statement}

Tout élément $s$ de $G$ est de la forme $zs'$, où $z$ est un élément inversible de $Z$ et $s'$ appartient à $G \cap C^+(Q)$ ou à $G \cap C^-(Q)$; le sous-groupe $G^+$ est d’indice 2 dans $G$ lorsque $E \neq \{0\}$.

La seconde assertion résulte évidemment de la première, puisque les vecteurs non singuliers appartiennent à $G \cap C^-(Q)$. Supposons d’abord $\dim(E)$ paire, et soit $s = t' + t''$, avec $t' \in C^+(Q)$ et $t'' \in C^-(Q)$; on a par définition $sx = (\varphi(s).x)s$ pour tout $x \in E$; comme $t'x$ et $(\varphi(s).x)t'$ (resp. $t''x$ et $(\varphi(s).x)t''$) sont des éléments impairs (resp. pairs), on a $t'x = (\varphi(s).x)t'$, d’où $s^{-1} t' x = xs^{-1} t'$ pour tout $x \in E$. On en conclut que $s^{-1} t' \in Z$ et comme $\dim(E)$ est paire, $Z = A$ (no 4, cor. du th. 2), donc $t' = as$, où $a \in A$. Si $a \neq 0$, on a donc $s = a^{-1} t'$ et $t' \in G \cap C^+(Q)$; si $a = 0$, $s = t'' \in G \cap C^-(Q)$ et le lemme est démontré dans ce cas. Si $\dim(E)$ est impaire, $A$ est de caractéristique $\neq 2$, donc pour tout $s \in G$, $\varphi(s)$ est un produit de symétries par rapport à des vecteurs non singuliers $x_i (i = 1, 2, \ldots, h)$ (§ 6, n° 4, prop. 5); si on pose $s' = x_1 x_2 \ldots x_h$, on a $\varphi(s) = \varphi(s')$, donc $s = z s'$, où $z \in \mathbf{Z}$, et $s'$ appartient à $C^+(Q)$ ou à $C^-(Q)$ suivant que $h$ est pair ou impair.

Supposons dim(E) paire. Comme tout élément $u$ de $\mathbf{O}(Q)$ se prolonge d’une manière et d’une seule en un automorphisme $\bar{u}$ de $C(Q)$ (prop. 1), et comme $C(Q)$ est centrale simple (th. 2), $\bar{u}$ est un automorphisme intérieur (chap. VIII, § 10, n° 1, th. 1). Il existe donc un élément $s$ de $G$ tel que $\varphi(s) = u$. D’autre part le centre de $C(Q)$ est contenu dans $C^+$, ce qui entraîne que $\varphi(G)/\varphi(G^+)$ est isomorphe à $G/G^+$, donc que $\varphi(G^+)$ est d’indice 2 dans $\varphi(G) = \mathbf{O}(Q)$ si $E \not= \{0\}$. Ceci démontre les deux premières assertions de c).

Supposons enfin que $A$ soit de caractéristique $\not= 2$. Alors tout élément $u$ de $\mathbf{O}(Q)$ est un produit de symétries par rapport à des hyperplans orthogonaux à des vecteurs non singuliers $x_i (i = 1, \ldots, h)$ (§ 6, n° 4, prop. 5); on a par suite $u = (-1)^h \varphi(x_1 \ldots x_h)$ et $\det(u) = (-1)^h$. Pour que $u$ appartienne à $\mathbf{SO}(Q)$, il faut et il suffit que $h$ soit pair, ce qui montre que $\varphi(G^+) \supset \mathbf{SO}(Q)$. Comme $\mathbf{SO}(Q)$ est d’indice 2 dans $\mathbf{O}(Q)$ lorsque $E \not= \{0\}$, on a $\varphi(G^+) = \mathbf{SO}(Q)$ si $E$ est de dimension *paire*, ce qui termine la démonstration de c). Par contre, si la dimension de $E$ est *impaire*, $\varphi(G)$ ne contient pas la transformation orthogonale $x \to -x$; en effet celle-ci se prolonge en l’automorphisme principal $\alpha$ de $C(Q)$ (n° 1), et $\alpha$ n’est pas un automorphisme intérieur puisque le centre $Z$ de $C(Q)$ contient un élément non nul de $C^-(Q)$ (th. 3). On a donc $\varphi(G) \not= \mathbf{O}(Q)$, et, comme $\varphi(G) \supset \varphi(G^+) \supset \mathbf{SO}(Q)$ et que $\mathbf{SO}(Q)$ est d’indice 2 dans $\mathbf{O}(Q)$, on a $\varphi(G) = \varphi(G^+) = \mathbf{SO}(Q)$. Ceci démontre d). CQFD.

Le sous-groupe $\varphi(G^+)$ de $\mathbf{O}(Q)$, qui est d’indice 2 si $E \not= \{0\}$, s’appelle le *groupe des rotations* de $E$, et ses éléments prennent le nom de *rotations*; on le note $\mathbf{O}^+(Q)$. Remarquons que, si $A$ n’est pas de caractéristique 2, on a $\mathbf{O}^+(Q) = \mathbf{SO}(Q)$ (cf. exerc. 9).

#### Proposition 4 {#alg-ix-s9-prop-4 .statement}

*Soit $\beta$ l’antiautomorphisme principal de $C(Q)$ (n° 1). Pour tout $s \in G^+$, $\beta(s)s$ est un scalaire. L’application $N : s \to \beta(s)s$ est un homomorphisme de $G^+$ dans le groupe multiplicatif $A^*$ des éléments non nuls de $A$.*

En effet, pour $s \in G^+$, on a $sEs^{-1} = E$, d’où $\beta(s)^{-1}E\beta(s) = E$, ce qui montre que $\beta(s) \in G^+$. Comme $sx = (\varphi(s).x)s$ pour tout $x \in E$, on a $x\beta(s) = \beta(sx) = \beta(s)(\varphi(s).x)$, et par suite $\beta(s)sx = \beta(s)(\varphi(s).x)s = x\beta(s)s$, ce qui entraîne que $\beta(s)s$ appartient au centre de $C(Q)$. Comme, de plus, $\beta(s)s$ appartient à $C^+(Q)$, $\beta(s)s$ est un scalaire (th. 2 et 3). Enfin on a $\beta(st)st = \beta(t)\beta(s)st = \beta(s)s\beta(t)t$, c’est-à-dire $N(st) = N(s)N(t)$ pour $s, t$ dans $G^+$. CQFD.

Le scalaire $N(s) = \beta(s)s$ ($s \in G^+$) s’appelle la norme spinorielle de $s$. On désigne par $G_0^+$ et on appelle groupe de Clifford réduit le noyau de l’homomorphisme $N$. L’image $\varphi(G_0^+)$ est notée $O_0^+(Q)$ et s’appelle le groupe orthogonal réduit de $Q$. Comme le noyau de la restriction de $\varphi$ à $G^+$ est l’ensemble des éléments pairs et invér-sibles du centre de $C(Q)$ (th. 4) et s’identifie donc à $A^*$ (th. 2 et 3), $\varphi(G^+)/O_0^+(Q)$ est isomorphe à $G^+/A^*G_0^+$, donc aussi à $N(G^+)/N(A^*)$, et en particulier commutatif. Il est clair que $N(A^*)$ est le sous-groupe $(A^*)^2$ des carrés d’éléments de $A^*$. Si $Q$ est d’indice $> 0$, il existe, quel que soit $a \in A^*$, deux éléments $x$ et $y$ de $E$ tels que $Q(x) = a$ et $Q(y) = 1$ (§ 4, no 2, prop. 4) ; comme $xy \in G^+$ et que $N(xy) = Q(x)Q(y) = a$, ceci montre que $N(G^+) = A^*$, donc que $\varphi(G^+)/O_0^+(Q)$ est isomorphe à $A^*/(A^*)^2$.

Exercices. — ¶ 1) Démontrer les cor. 3 et 4 du th. 1 du no 3 lorsque $E_1$ et $E_2$ sont deux sous-modules supplémentaires quelconques dans $E$. (Établir d’abord le cor. 4 : montrer pour cela que le produit tensoriel $C(Q_1) \otimes C(Q_2)$ est muni d’une structure d’algèbre par la convention de signe faite dans l’énoncé du cor. 4, et que cette algèbre $S$ est solution du même problème d’application universelle que $C(Q)$; on considérera pour cela, pour toute application linéaire $f$ de $E$ dans une algèbre $D$ sur $A$ telle que $(f(x))^2 = Q(x).1$, l’homomorphisme $\bar{f}_i$ de $C(Q_i)$ dans $D$ tel que $\bar{f}_i(1) = 1$, $\bar{f}_i(\rho_{Q_i}(x_i)) = f(x_i)$ pour $x_i \in E_i$ ($i = 1, 2$) et on prouvera qu’il existe un homomorphisme $\bar{f}$ de l’algèbre $S$ dans $D$ tel que
$$
\bar{f}(z_1 \otimes z_2) = \bar{f}_1(z_1)\bar{f}_2(z_2)
$$
pour $z_i \in C(Q_i)$ ($i = 1, 2$). Pour démontrer ensuite le cor. 3, considérer la forme quadratique $Q'$ somme directe externe de $Q_1$ et $Q_2$ (§ 3, no 4), et remarquer que l’on a $Q'(x) = Q(x) + F(x, x)$, $F$ étant la forme bilinéaire définie par $F(x_1 + x_2, y_1 + y_2) = -\Phi(x_1, y_2)$ pour $x_i, y_i$ dans $E_i$ ($i = 1, 2$) ; utiliser alors la prop. 3.)

¶ 2) On suppose que $E$ soit somme directe de deux sous-modules orthogonaux $E_1, E_2$ et on désigne par $Q_i$ la restriction de $Q$ à $E_i$ ($i = 1, 2$);

on suppose en outre qu’il existe $u \in C^+(Q_2)$ tel que $u^2 = a . 1$, $a$ étant invér sible dans $A$, et que $u \rho_{Q_2}(x_2) = -\rho_{Q_2}(x_2)$ pour tout $x_2 \in E_2$. Montrer qu’il existe un isomorphisme $\varphi$ de $C(Q)$ sur le produit tensoriel $C(aQ_1) \otimes C(Q_2)$ (tel qu’il est défini dans le chap. III, § 3, n° 1), ayant la propriété que pour tout $x = x_1 + x_2$ ($x_i \in E_i, i = 1, 2$), on a
$$
\varphi(\rho_Q(x)) = \rho_{aQ_1}(x_1) \otimes u^{-1} + 1 \otimes \rho_{Q_2}(x_2).
$$
(Prouver l’existence de l’homomorphisme $\varphi$ comme conséquence de la propriété universelle de $C(Q)$. D’autre part, il y a un homomorphisme $g_1$ de $C(aQ_1)$ dans $C(Q)$ tel que $g_1(\rho_{aQ_1}(x_1)) = h_2(u)\rho_{Q_1}(x_1)$, en désignant par $h_2$ l’homomorphisme canonique de $C(Q_2)$ dans $C(Q)$; remarquer alors que $g_1(z_1)$ et $h_2(z_2)$ sont permutables pour $z_1 \in C(aQ_1)$ et $z_2 \in C(Q_2)$, et en déduire l’existence d’un homomorphisme réciproque de $\varphi$.)

Dans quel cas ce résultat s’applique-t-il lorsque $A$ est un corps de caractéristique $\neq 2$ (utiliser la Remarque 2 suivant le cor. du th. 2) ?

3) a) Avec les notations du n° 2, soient $x_i$ ($1 \leqslant i \leqslant n$) des éléments de $E$ tels que $f(x_i) = 0$; montrer que l’on a $i_f(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0$. En particulier, si $F$ est une forme bilinéaire sur $E$ telle que $F(x_i, x_j) = 0$ pour $i > j$, on a $i_F^E(x_2 \otimes x_3 \otimes \cdots \otimes x_n) = 0$.

b) Avec les notations de la prop. 3 du n° 3, soient $x_i$ ($1 \leqslant i \leqslant n$) des éléments de $E$ tels que $F(x_i, x_j) = 0$ pour $i > j$. Montrer que l’on a $\overline{\lambda}_F(\rho_{Q'}(x_1) \ldots \rho_{Q'}(x_n)) = \rho_Q(x_1) \ldots \rho_Q(x_n)$ (utiliser $a$) et la formule (10) du n° 2).

c) On suppose que $A$ est un corps de caractéristique $\neq 2$; pour toute forme quadratique $Q$ sur $E$, soit $\mu_Q$ l’application $\overline{\lambda}_F$ de $C(Q)$ sur $\wedge E$ correspondant à $F(x, y) = \frac{1}{2} \Phi(x, y)$. Montrer que si les vecteurs $x_i$ ($1 \leqslant i \leqslant n$) sont deux à deux orthogonaux, on a
$$
\mu_Q(x_1 x_2 \ldots x_n) = x_1 \wedge x_2 \wedge \ldots \wedge x_n.
$$
En déduire que si $y_i$ ($1 \leqslant i \leqslant n$) sont $n$ vecteurs quelconques, on a
$$
n! \; \mu_Q^{-1}(y_1 \wedge y_2 \wedge \ldots \wedge y_n) = \sum_{\sigma \in S_n} \varepsilon_\sigma y_{\sigma(1)} y_{\sigma(2)} \cdots y_{\sigma(n)}.
$$

4) Soit $C_h$ le sous-module de $C(Q)$ engendré par les produits de $k$ éléments de $\rho_Q(E)$ pour $0 \leqslant k \leqslant h$. Montrer que l’application
$$
(x_1, \ldots, x_h) \to \rho_Q(x_1) \ldots \rho_Q(x_h)
$$
définit par passage aux quotients une application multilinéaire alternée de $E^h$ dans $C_h/C_{h-1}$. On en déduit une application linéaire $\pi_h$ de $\wedge^h E$ dans $C_h/C_{h-1}$; montrer que $\pi_h$ est un isomorphisme lorsque $E$ est un module libre. Si $f$ est une transformation orthogonale, on a $C(f) \circ \pi_h = \pi_h \circ (\wedge^h f)$. Lorsque $A$ est un corps de caractéristique $\neq 2$, montrer que $\pi_h$ est la restriction de l’application $\mu_Q^{-1}$ définie dans l’exerc. 3 c).

5) Avec les notations du n° 2, on considère l’application $i_f$ de $\wedge E$ dans elle-même. Montrer que l’on a

$$
i_f(x_1 \wedge \ldots \wedge x_h) = \sum_{i=1}^{h} (-1)^{i-1} f(x_i) (x_1 \wedge \ldots \wedge x_{i-1} \wedge x_{i+1} \wedge \ldots \wedge x_h)
$$

et en déduire que $i_f$ n’est autre que le produit intérieur droit $z \to z \llcorner f$ (chap. III, § 8, n° 4, déf. 2).

6) Montrer que, si E admet une base orthogonale $(e_1, e_2)$ pour Q, et si on pose $\alpha_i = Q(e_i)$ ($i = 1, 2$), l’algèbre C(Q) est isomorphe à l’algèbre des quaternions sur A correspondant au couple $(\alpha_1, \alpha_2)$.

7) Soient A un corps ordonné maximal, E un espace vectoriel de dimension paire $2r$ sur A, Q une forme quadratique non dégénérée sur E, positive ou négative. Montrer que, si Q est positive, C(Q) est isomorphe à une algèbre de matrices sur A lorsque $r(r-1)/2$ est pair, à une algèbre de matrices sur le corps des quaternions sur A lorsque $r(r-1)/2$ est impair. Si Q est négative, C(Q) est isomorphe à une algèbre de matrices sur A lorsque $r(r+1)/2$ est pair, à une algèbre de matrices sur le corps des quaternions sur A lorsque $r(r+1)/2$ est impair (utiliser les exerc. 2 et 6). Quelle est la structure de $C^+(Q)$ dans ces différents cas ?

8) Soient A l’anneau $\mathbf{Z}/(4)$, E le A-module $\mathbf{Z}/(2)$; si on pose Q(0) = 0, Q(u) = 1 pour l’unique élément $u \neq 0$ de E, Q est une forme quadratique sur E. Montrer que les A-modules C(Q) et $\wedge E$ ne sont pas isomorphes (on prouvera que C(Q) est isomorphe à la somme directe de deux modules isomorphes à E).

¶ 9) On suppose que A est un corps de caractéristique 2, E un espace vectoriel de dimension finie paire $2r$, Q une forme quadratique non dégénérée sur E.

a) Soit $(e_i)$ une base symplectique ($§ 5,$ n° 1) de E pour la forme bilinéaire alternée $\Phi$ associée à Q. Montrer que l’élément

$$
z = e_1 e_2 + e_3 e_4 + \cdots + e_{2r-1} e_{2r}
$$

de $C^+(Q)$ forme, avec l’élément unité, une base du centre Z de $C^+(Q)$. Pour que Z soit somme directe de deux corps, il faut et il suffit que l’élément

$$
\Delta(Q) = Q(e_1) Q(e_2) + Q(e_3) Q(e_4) + \cdots + Q(e_{2r-1}) Q(e_{2r})
$$

(appelé *pseudo-discriminant* de Q par rapport à la base symplectique $(e_i)$) soit de la forme $\lambda^2 + \lambda$, avec $\lambda \in A$.

b) Soit $u$ une similitude pour $\Phi$ ($§ 6,$ n° 5) de multiplicateur $\mu(u)$, et soit $Q_1(x) = Q(u(x))$. On pose

$$
u(e_{2i-1}) = \sum_{j=1}^{r} a_{ij} e_{2j-1} + \sum_{j=1}^{r} b_{ij} e_{2j},
$$
$$
u(e_{2i}) = \sum_{j=1}^{r} c_{ij} e_{2j-1} + \sum_{j=1}^{r} d_{ij} e_{2j},
$$

et $Q(e_{2i-1}) = \alpha_i, Q(e_{2i}) = \beta_i$ ($1 \leq i \leq r$). Montrer que l’on a
$$
\Delta(Q_1) = (\mu(u))^2 \Delta(Q) + (\mathrm{D}(u))^2 + \mu(u)\mathrm{D}(u)
$$
où
$$
\mathrm{D}(u) = \sum_{i,j} (\alpha_j a_{ij} c_{ij} + \beta_j b_{ij} d_{ij} + b_{ij} c_{ij})
$$
(invariant de Dickson de $u$ par rapport à la base $(e_i)$). (Remarquer que l’élément
$$
(\mu(u))^{-1}(u(e_1)u(e_2) + u(e_3)u(e_4) + \cdots + u(e_{2r-1})u(e_{2r}))
$$
appartient à $\mathbf{Z}$.) Pour que $u$ soit une similitude pour $Q$ ($§ 4$, exerc. 9) de multiplicateur $\mu(u)$, il faut et il suffit que $\mathrm{D}(u) = 0$ ou $\mathrm{D}(u) = \mu(u)$; les similitudes pour $Q$ telles que $\mathrm{D}(u) = 0$ sont dites directes.

c) Montrer que, si $\varphi$ est une similitude pour $\Phi$, $u$ une similitude pour $Q$, on a
$$
\mathrm{D}(u\varphi) = \mu(\varphi)\mathrm{D}(u) + \mu(u)\mathrm{D}(\varphi)
$$
(considérer l’invariant de Dickson de $\varphi$ par rapport à la base symplectique formée des $u(e_{2i-1})$ et $(\mu(u))^{-1}u(e_{2i})$ pour $1 \leq i \leq r$). En déduire que les similitudes directes pour $Q$ forment un sous-groupe distingué d’indice 2 dans le groupe des similitudes pour $Q$.

d) Si $u$ est la symétrie par rapport à l’hyperplan orthogonal à un vecteur non singulier dans $E$, montrer que $\mathrm{D}(u) = 1$. En déduire que le groupe $\varphi(G^+)$ (notations du n° 5) est le groupe $\mathbf{SO}(Q)$ défini dans l’exerc. 28 c) du $§ 6$.

e) Soit $u \in \mathbf{O}(Q)$, et supposons $\Lambda$ algébriquement clos. Montrer que, pour que $u \in \mathbf{SO}(Q)$, il faut et il suffit que le nombre des diviseurs élémentaires du module $E_u$ soit pair. (Avec les notations de l’exerc. 15 du $§ 5$, remarquer d’abord que si $p, q$ sont deux facteurs irréductibles distincts du polynôme minimal de $u$, le nombre des sous-modules indécomposables dont $G(p, q)$ est somme directe est égal au nombre des sous-modules indécomposables dont $G(q, p)$ est somme directe. Remarquer d’autre part que $G(p, p) = \{0\}$ sauf pour $p = X - 1$. Prouver enfin qu’on peut se borner au cas où $E_u$ est égal à $G(p, p)$ (avec $p = X - 1$) et est indécomposable. Il y a alors une base symplectique $(e_i)$ de $E$ telle que $e_1, e_3, \ldots, e_{2k-1}$ forment une base de $(p(u))^{2r-k}(E)$ pour $1 \leq k \leq r$; montrer que $e_1, e_3, \ldots, e_{2r-3}$ sont des vecteurs singuliers, et conclure que $\mathrm{D}(u) = 1$.)

$§ 10$ On suppose que $A$ est un corps, $E$ un espace vectoriel de dimension finie, $Q$ une forme quadratique dégénérée sur $E$; soient $M$ un sous-espace supplémentaire de $E^0$ dans $E$, $B$ l’algèbre de Clifford (semi-simple) de la restriction de $Q$ à $M$.

a) On suppose d’abord $A$ de caractéristique $\neq 2$. Soient $L$ l’algèbre de Clifford de la restriction de $Q$ à $E^0$ (isomorphe à $\wedge E^0$), $\mathcal{R}_0$ son radical (idéal engendré dans $L$ par $E^0$, et de codimension 1 dans $L$); montrer que le radical $\mathcal{R}$ de $C(Q)$ s’obtient (à une isomorphie près) en définissant la structure d’algèbre sur $B \otimes_A \mathcal{R}_0$ comme dans le cor. 4 du th. 1, que $C(Q)/\mathcal{R}$ est isomorphe à $B$ et $C(Q)$ est somme directe de $B$ et de $\mathcal{R}$.

b) On suppose A de caractéristique 2. Soit F le sous-espace de E⁰ formé des vecteurs singuliers $x \in E^0$, et soit N un supplémentaire de F par rapport à E⁰. Si $(a_i)_{1 \leq i \leq d}$ est une base de N, et Q$(a_i) = \alpha_i$, les éléments $\alpha_i^{1/2}$, dans une clôture algébrique de A, sont linéairement indépendants sur A. Soit $(\alpha_i^{1/2})_{1 \leq i \leq e}$ une 2-base du corps $A_1 = A(\alpha_1^{1/2}, \ldots, \alpha_d^{1/2})$ sur A (chap. V, § 8, exerc. 1), et soit $h = \dim F$. Si B₁ est l’algèbre centrale simple $B \otimes_A A_1$, montrer que C(Q) est isomorphe à l’algèbre $B_1 \otimes_{A_1} L_1$, où $L_1$ est l’algèbre extérieure d’un espace vectoriel de dimension $h + d - e$ sur $A_1$. Si $R_1$ est le radical de $L_1$ (de codimension 1 (sur $A_1$) dans $L_1$), le radical $R$ de C(Q) est isomorphe à l’algèbre $B_1 \otimes_{A_1} R_1$, $C(Q)/R$ est isomorphe à $B_1$, et C(Q) est somme directe de $B_1$ et de $R$.

c) Les hypothèses étant celles de b), on suppose en outre que $h = 0$, $d = 1, e = 0$ (ce qui implique que dim M est pair). Si $Q_0$ est la restriction de Q à M, montrer que $C^+(Q)$ est isomorphe à $C(Q_0)$.

¶ 11) a) Avec les hypothèses et notations du n° 5, montrer que $N(G^+)$ est le sous-groupe de $A^*$ engendré par les produits $Q(x)Q(y)$, où $x$ et $y$ parcourent l’ensemble des vecteurs non isotropes de E. (Se ramener au cas $A \neq \mathbf{F}_2$; utiliser la prop. 5 et l’exerc. 28 c) du § 6, ainsi que l’exerc. 9 d) du § 9.) Cas où Q est d’indice $\geq 1$.

b) On suppose en outre que $A \neq \mathbf{F}_2$, que E est de dimension $n \geq 2$ et que Q est d’indice $> 0$. Montrer que $O_0^+(Q)$ est le groupe des commutateurs du groupe $O(Q)$. (Se ramener au cas $n = 2$, en utilisant les exerc. 17 c) et 28 e) du § 6.)

c) On conserve les hypothèses de b), et on suppose en outre que A est de caractéristique $\neq 2$ et que E est de dimension paire. Pour que l’automorphisme $x \to -x$ de E appartienne à $O_0^+(Q)$ il faut et il suffit que le discriminant de Q (par rapport à une base quelconque de E) soit un carré.

¶ 12) a) Soit $a$ un élément inversible de A ; montrer qu’il existe un isomorphisme et un seul $\theta_a$ de $C^+(Q)$ sur $C^+(aQ)$ tel que

$$
\theta_a(\rho(x)\rho(y)) = a^{-1}\rho_1(x)\rho_1(y)
$$

quels que soient $x, y$ dans E ($\rho$ et $\rho_1$ désignant les applications canoniques de E dans $C(Q)$ et $C(aQ)$ respectivement). En déduire que si A est un corps de caractéristique $\neq 2$, E un espace vectoriel de dimension impaire et Q une forme quadratique non dégénérée, $C(Q)$ et $C(aQ)$ sont isomorphes (cf. exerc. 7).

b) On suppose que A soit un corps, E un espace vectoriel de dimension paire $2r > 0$, Q une forme quadratique non dégénérée. Soit $u$ une similitude relative à Q ; montrer qu’il existe un A-automorphisme et un seul $\bar{u}$ de l’algèbre $C^+(Q)$ tel que pour $1 \leq h \leq r$ et $x_i \in E$ ($1 \leq i \leq 2h$), on ait

$$
\bar{u}(x_1x_2 \ldots x_{2h}) = \mu^{-h}u(x_1)u(x_2) \ldots u(x_{2h})
$$

où $\mu$ désigne le multiplicateur de $u$. Pour que $\bar{u}$ soit un automorphisme intérieur, il faut et il suffit que $u$ soit une similitude directe (§ 6, n° 5 et § 9, exerc. 9 b)). On suppose en outre $r \geq 2$; alors, pour que $\bar{u}$ soit l’identité, il faut et il suffit que $u$ soit une homothétie.

Montrer que l’automorphisme $\bar{u}$ de $C^+(Q)$ est la restriction à $C^+(Q)$ d’un automorphisme intérieur de $C(Q)$.

¶ 13) On suppose que $A$ soit un corps de caractéristique $\neq 2$, $E$ un espace vectoriel de dimension paire $2r > 0$, $Q$ une forme quadratique non dégénérée. On désigne par $E_h$ l’image réciproque de $\wedge^h E$ par l’isomorphisme $\mu_Q$ de l’exerc. 3 c), de sorte que $E_h$ est le sous-espace de $C(Q)$ engendré par les produits $x_1 x_2 \ldots x_h$, où les $x_i$ ($1 \leq i \leq h$) sont deux à deux orthogonaux.

a) Soient $\alpha$ un élément de $A$, $s$ un élément de $E_2$. Montrer que, si $(\alpha + s)^2 \in A$, ou bien $s = 0$, ou bien $\alpha = 0$ et $s = xy$, où $x$ et $y$ sont deux vecteurs orthogonaux. (Remarquer que si $t = \mu_Q(\alpha + s)$, $t \wedge t$ appartient nécessairement à $A + \wedge^2 E$, en exprimant $s$ à l’aide d’une base orthogonale de $E$; en déduire qu’on a nécessairement $t = \beta + x \wedge y$ avec $\beta \in A$, $x, y$ dans $E$, en utilisant le § 5, no 1, cor. 2 du th. 1).

b) Soient $(x, y), (u, v)$ deux couples de vecteurs orthogonaux non isotropes dans $E$, $P_{xy}$ et $P_{uv}$ les plans $Ax + Ay, Au + Av$ respectivement. Pour que l’on ait $(xy)(uv) = -(uv)(xy)$ dans $C(Q)$, il faut et il suffit que $P_{xy} + P_{uv}$ soit un sous-espace non isotrope de dimension 3, dans lequel $P_{xy}$ et $P_{uv}$ sont faiblement orthogonaux (§ 3, exerc. 11).

c) Soit $g$ un $A$-automorphisme de $C^+(Q)$ transformant $E_2$ en lui-même; montrer qu’il existe une similitude $u$ relative à $Q$ telle que $g = \bar{u}$ (exerc. 12 b)). (Soit $(e_i)_{1 \leq i \leq 2r}$ une base orthogonale de $E$; en utilisant $a$ et $b$), montrer qu’il existe une base orthogonale $(x_i)$ de $E$ telle que $g(e_1 e_i) = x_1 x_i$ pour $2 \leq i \leq 2r$.

14) On suppose que $A$ est un corps de caractéristique $\neq 2$, $E$ un espace vectoriel de dimension $n$ sur $A$, $Q$ et $Q_1$ deux formes quadratiques non dégénérées sur $E$; soit $\tilde{\Delta}$ (resp. $\tilde{\Delta}_1$) la classe du discriminant $\Delta$ de $Q$ (resp. du discriminant $\Delta_1$ de $Q_1$) par rapport à une base de $E$, dans le groupe $A^*/(A^*)^2$, classe qui ne dépend pas de la base choisie dans $E$. On suppose $n = 2$.

a) Montrer que si $\tilde{\Delta} = \tilde{\Delta}_1$ et si les algèbres de Clifford $C(Q)$ et $C(Q_1)$ sont isomorphes, $Q$ et $Q_1$ sont équivalentes (considérer sur $C(Q)$ la forme quadratique $z \mapsto z \bar{z}$, où $z \mapsto \bar{z}$ est l’unique antiautomorphisme involutif de $C(Q)$ dont l’ensemble des invariants soit le centre de $C(Q)$ (cf. exerc. 6 et chap. VIII, § 11, exerc. 5 e)); appliquer le th. de Witt).

b) Pour que $C(Q)$ soit isomorphe à l’algèbre de matrices $\mathbf{M}_2(A)$ il faut et il suffit que, pour un $x \neq 0$ au moins dans $E$, il existe $y, z$ dans $E$ tels que $Q(x) + Q(y)Q(z) = 0$; s’il en est ainsi, cette propriété est vraie pour tout $x \neq 0$ dans $E$.

¶ 15) On garde les notations et hypothèses générales de l’exerc. 14, mais on suppose $n = 3$.

a) Montrer que $C^+(Q)$ est isomorphe à une algèbre de quaternions sur $A$ et que $\beta$ est l’antiautomorphisme $z \mapsto \bar{z}$ de cette algèbre dont l’ensemble des invariants est le centre de $C^+(Q)$; si $P$ est le sous-espace de $C^+(Q)$ formé des quaternions purs (c’est-à-dire tels que $z = -\bar{z}$; chap. VIII, § 11, exerc. 6), la restriction à $P$ de la forme quadratique $z \mapsto z \bar{z}$ est équivalente à $\lambda Q$, où $\lambda \in A$. En déduire que, pour que $C^+(Q)$ soit un corps, il faut et il suffit que $Q$ soit d’indice 0.

b) Montrer que si $\tilde{\Delta} = \tilde{\Delta}_1$ et si les algèbres de Clifford $C(Q)$ et $C(Q_1)$ sont isomorphes, $Q$ et $Q_1$ sont équivalentes. (Considérer d’abord le cas où $-\Delta$ est un carré dans $K$, et montrer que dans ce cas $C^+(Q)$ et $C^+(Q_1)$ sont isomorphes ; raisonner ensuite comme dans l’exerc. 14 $a$), en utilisant a) et l’exerc. 6 du chap. VIII, § 11. Dans le cas général, utiliser l’exerc. 12 $a))$.

c) Montrer que le groupe de Clifford spécial $G^+$ (pour la forme $Q$) est identique au groupe des éléments inversibles de $C^+(Q)$. (Si $(e_1, e_2, e_3)$ est une base orthogonale de $E$, et si $j = e_1 e_2 e_3$ dans $C(Q)$, remarquer que $x \to xj$ est un isomorphisme d’espace vectoriel de $E$ sur $P$).

d) Déduire de a) et c) que si $Q$ est d’indice 1, le groupe des rotations $O^+(Q)$ est isomorphe au groupe projectif $\mathbf{PGL}_2(A)$ (chap. II, 2e éd., App. III, no 6).

¶ 16) On garde les hypothèses et notations générales de l’exerc. 14, mais on suppose $n = 4$.

a) Donner un exemple où $\tilde{\Delta} = \tilde{\Delta}_1$ et où $C(Q)$ et $C(Q_1)$ sont isomorphes, mais où $Q$ et $Q_1$ ne sont pas équivalentes (cf. exerc. 7).

b) Soient $(e_i)_{1 \leq i \leq 4}$ une base orthogonale de $E$ pour $Q$, $Q_0$ la restriction de $Q$ à l’hyperplan $H = Ae_1 + Ae_2 + Ae_3$. Montrer que, si $Z$ est le centre de $C^+(Q)$, l’algèbre $C^+(Q)$ est isomorphe au produit tensoriel $Z \otimes_A C^+(Q_0)$. Pour tout $z \in C^+(Q)$, on a $\beta(z)z \in Z$; pour que $z$ appartienne au groupe de Clifford spécial $G^+$, il faut et il suffit que $z$ soit inversible et que $\beta(z)z \in A.1$. En déduire que le groupe $O_0^+(Q)$ est isomorphe au quotient par $\{1, -1\}$ du groupe des éléments $z \in Z \otimes_A C^+(Q_0)$ tels que $\beta(z)z = 1$.

c) On suppose que $\Delta$ n’est pas un carré dans $A$ (ce qui implique, en vertu du th. de Witt, que l’indice de $Q$ est 0 ou 1). Si $Q_0'$ est la forme quadratique obtenue à partir de $Q_0$ par extension à $A' = A(\sqrt{\Delta})$ du corps des scalaires, déduire de b) que $O_0^+(Q)$ est isomorphe à $O_0^+(Q_0')$. En particulier, si $Q$ est d’indice 1, $O_0^+(Q)$ est le groupe des commutateurs de $O(Q)$ et est isomorphe à $\mathbf{PSL}_2(A')$ (cf. exerc. 15 $d$) et chap. III, § 7, exerc. 8).

d) On suppose que $\Delta$ est un carré dans $A$ (ce qui implique, en vertu du th. de Witt, que $Q$ est d’indice 0 ou 2) et que $Q(e_4) = 1$. Si on pose $j = e_1 e_2 e_3$, tout $x \in E$ peut s’écrire d’une seule manière $x = \alpha e_4 + jz$, où $\alpha \in A$ et $z$ est un quaternion pur (exerc. 15 $a$)) dans $L = C^+(Q_0)$; si on pose $\psi(x) = \alpha + z$, $\psi$ est un isomorphisme d’espace vectoriel de $E$ sur $L$. Soit $Z = Ac' + Ac''$, où $c'$ et $c''$ sont les deux idempotents orthogonaux dans $Z$; tout élément inversible $s \in C^+(Q)$ s’écrit d’une seule manière $s = uc' + vc''$, où $u$ et $v$ appartiennent à $L$; pour que $s$ appartienne au groupe de Clifford spécial $G^+$, il faut et il suffit que $u \bar{u} = v \bar{v}$, et on a alors $\psi(sxs^{-1}) = u \psi(x) v^{-1}$ pour tout $x \in E$. En déduire que le quotient de $O_0^+(Q)$ par son centre (qui est un groupe à 2 éléments, cf. exerc. 11 $c$)) est isomorphe au produit $O_0^+(Q_0) \times O_0^+(Q_0)$; en particulier, si $Q$ est d’indice 2, ce groupe quotient est isomorphe à $\mathbf{PSL}_2(A) \times \mathbf{PSL}_2(A)$.

17) Soient K un corps commutatif de caractéristique $\neq 2$, A le corps $K(X_n)_{n \in \mathbf{N}}$ des fractions rationnelles sur K, par rapport à une famille dénombrable d’indéterminées (chap. IV, § 3, n° 1). Soit E un espace vectoriel sur A, ayant une base dénombrable $(e_n)_{n \in \mathbf{N}}$, et soit $\Phi$ une forme bilinéaire symétrique sur E, pour laquelle $(e_n)$ est une base orthogonale et telle que $\Phi(e_n, e_n) = X_n$ pour tout $n \in \mathbf{N}$. Si on pose $Q(x) = \Phi(x, x)$, montrer que l’algèbre de Clifford C(Q) est un corps (cf. chap. VIII, § 12, exerc. 14).
