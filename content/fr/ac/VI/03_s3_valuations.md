---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 3
section_title: Valuations
lang: fr
source: ac-v-vii-fr
pdf_pages: 0097-0106, 0169-0171
extraction: ocr
subsections:
    - "no": 1
      title: Valuations sur un anneau
      page: 0
      pdf_page: 97
    - "no": 2
      title: Valuations sur un corps
      page: 0
      pdf_page: 98
    - "no": 3
      title: Traductions
      page: 0
      pdf_page: 101
    - "no": 4
      title: Exemples de valuations
      page: 0
      pdf_page: 102
    - "no": 5
      title: Idéaux d’un anneau de valuation
      page: 0
      pdf_page: 104
    - "no": 6
      title: Valuations discrètes
      page: 0
      pdf_page: 104
statements: 21
exercises: 8
content_sha256: cb962a9e1de7dbc0919ab4b3a3677fc2dce3757ec3b25d14f45c1f9ee9bd6230
---

## § 3. Valuations.

### 1. Valuations sur un anneau

Soit $\Gamma$ un groupe commutatif totalement ordonné, noté additivement. Dans la suite de ce chapitre, nous aurons à considérer, pour un tel groupe, l’ensemble obtenu en adjoignant à $\Gamma$ un élément noté $+\infty$; nous noterons $\Gamma_\infty$ cet ensemble, et nous le munirons : 1° d’un ordre total pour lequel $+\infty$ est le plus grand élément, autrement dit tel que $\alpha < +\infty$ pour tout $\alpha \in \Gamma$; 2° d’une structure de monoïde commutatif dont la loi induit sur $\Gamma$ la loi de groupe donnée, et est définie par les conditions

$$
(+x) + (+\infty) = +x, \quad \alpha + (+\infty) = +\infty
$$

pour tout $\alpha \in \Gamma$; on vérifie aussitôt que cette loi est associative et commutative et que la relation $\alpha \leq \beta$ dans $\Gamma_\infty$ entraîne $\alpha + \gamma \leq \beta + \gamma$ pour tout $\gamma \in \Gamma_\infty$.

#### Définition 1 {#ac-vi-s3-def-1 .statement}

Soient $C$ un anneau (non nécessairement commutatif), $\Gamma$ un groupe commutatif totalement ordonné, noté additivement. On appelle valuation de $C$ à valeurs dans $\Gamma$ toute application $v : C \to \Gamma_\infty$ qui vérifie les conditions suivantes :

(VL₁) $v(xy) = v(x) + v(y)$ pour $x \in C, y \in C$.
(VL₂) $v(x + y) \geq \inf (v(x), v(y))$ pour $x \in C, y \in C$.
(VL₃) $v(1) = 0$ et $v(0) = +\infty$.

Si $C$ est $\neq 0$ et n’a pas de diviseur de zéro autre que 0, l’unique application $v_0$ de $C$ dans $\Gamma_\infty$ telle que $v_0(x) = 0$ pour $x \neq 0$ et $v_0(0) = +\infty$ est une valuation, dite valuation impropre de $C$. Si $z \in C$ est tel que $z^n = 1$ pour un entier $n \geq 1$, on a, d’après (VL₁), $nv(z) = v(z^n) = 0$, donc $v(z) = 0$ pour toute valuation $v$ de $C$, puisque $\Gamma$ est un groupe totalement ordonné. En particulier on a $v(-1) = 0$, d’où $v(-x) = v(x)$ pour tout $x \in C$. En outre, il résulte de (VL₁) que $v(xy) = v(yx)$ quels que soient $x, y$ dans $C$. Si $x$ est inversible dans $C$, on a $v(x^{-1}) = -v(x)$.

#### Proposition 1 {#ac-vi-s3-prop-1 .statement}

Soit $v$ une valuation d’un anneau $C$ (non nécessairement commutatif). Quels que soient les éléments $x_i \in C$ ($1 \leq i \leq n$), on a

$$
v\left( \sum_{i=1}^n x_i \right) \geq \inf_{1 \leq i \leq n} v(x_i)
$$

En outre, s’il existe un seul indice $k$ tel que $\nu(x_k) = \inf_{1 \leq i \leq n} \nu(x_i)$, les deux membres de (1) sont égaux. En particulier, si $\nu(x) \neq \nu(y)$, on a $\nu(x + y) = \inf (\nu(x), \nu(y))$.

La relation (1) se déduit de l’axiome (VL$_{\text{II}}$) par récurrence sur $n$. S’il existe un seul indice $k$ tel que $\nu(x_k) = \inf_{1 \leq i \leq n} \nu(x_i)$, on a, en posant $y = \sum_{i \neq k} x_i$ et $z = \sum_{i=1}^n x_i$, $\nu(y) > \nu(x_k)$ et $\nu(z) \geq \nu(x_k)$ d’après (1); si l’on avait $\nu(z) > \nu(x_k)$, la relation $x_k = z - y$ donnerait $\nu(x_k) \geq \inf (\nu(z), \nu(y)) > \nu(x_k)$, ce qui est absurde; d’où $\nu(z) = \nu(x_k)$, ce qui démontre la seconde assertion.

#### Corollaire {#ac-vi-s3-n1-cor-1 .statement}

Si une suite finie d’éléments $(x_i)_{1 \leq i \leq n}$ de $\mathbf{C}$ (pour $n \geq 2$) est telle que $\sum_{i=1}^n x_i = 0$, il existe au moins deux indices distincts $j, k$ tels que $\nu(x_j) = \nu(x_k) = \inf_{1 \leq i \leq n} \nu(x_i)$.

S’il n’y avait qu’un seul indice $k$ tel que $\nu(x_k) = \inf_{1 \leq i \leq n} \nu(x_i)$, la prop. 1 montrerait que $\nu(x_k) = \nu(0) = +\infty$, d’où $\nu(x_i) = +\infty$ pour tout $i$, contrairement à la relation $n \geq 2$ et à l’hypothèse faite sur $k$.

#### Remarque 1 {#ac-vi-s3-n1-rem-1 .statement}

Si $\nu : \mathbf{C} \to \Gamma_\infty$ est une valuation de $\mathbf{C}$ et $u : \mathbf{B} \to \mathbf{C}$ un homomorphisme d’un anneau $\mathbf{B}$ dans $\mathbf{C}$, il est immédiat que l’application composée $\mathbf{B} \xrightarrow{u} \mathbf{C} \xrightarrow{\nu} \Gamma_\infty$ est une valuation de $\mathbf{B}$ à valeurs dans $\Gamma$.

#### Remarque 2 {#ac-vi-s3-n1-rem-2 .statement}

Les conditions (VL$_{\text{I}}$) et (VL$_{\text{II}}$) montrent aussitôt que l’ensemble $\bar{\nu}^1(+\infty)$ est un idéal bilatère $\mathfrak{p}$ dans $\mathbf{C}$ distinct de $\mathbf{C}$ en vertu de (VL$_{\text{III}}$); en outre, si $x, y$ sont deux éléments de $\mathbf{C}$ tels que $\nu(xy) = +\infty$, il résulte de (VL$_{\text{I}}$) que l’on a nécessairement $\nu(x) = +\infty$ ou $\nu(y) = +\infty$; autrement dit, l’anneau quotient $\mathbf{C}/\mathfrak{p}$ n’a pas de diviseur de 0 autre que 0; on vérifie aussitôt que l’application $\bar{\nu} : \mathbf{C}/\mathfrak{p} \to \Gamma_\infty$ déduite de $\nu$ par passage au quotient est une valuation de $\mathbf{C}/\mathfrak{p}$, l’image réciproque de $+\infty$ par cette valuation se réduisant à 0.

### 2. Valuations sur un corps

#### Proposition 2 {#ac-vi-s3-prop-2 .statement}

Soient $K$ un corps (non nécessairement commutatif), $\nu$ une valuation de $K$, à valeurs dans $\Gamma$. Alors:

(i) Pour $x \neq 0$, on a $\nu(x) \neq +\infty$.

(ii) L’ensemble $A$ des $x \in K$ tels que $\nu(x) \geqslant 0$ est un sous-anneau de $K$.

(iii) Pour tout $\alpha \geqslant 0$ dans $\Gamma$, l’ensemble $V_{\alpha}$ (resp. $V'_{\alpha}$) des $x \in A$ tels que $\nu(x) > \alpha$ (resp. $\nu(x) \geqslant \alpha$) est un idéal bilatère de $A$, et tout idéal $\neq (0)$ de $A$ (à gauche ou à droite) contient un des $V'_{\alpha}$.

(iv) L’ensemble $m(A)$ des $x \in A$ tels que $\nu(x) > 0$ est le plus grand idéal $\neq A$ de $A$; $U(A) = A - m(A)$ est l’ensemble des éléments inversibles de $A$ et $\kappa(A) = A/m(A)$ est un corps (non nécessairement commutatif).

(v) Pour tout $x \in K - A$, on a $x^{-1} \in m(A)$.

L’assertion (i) résulte de ce que $\nu(-1)$ est un idéal de $K$ non égal à $K$. La vérification du fait que $A$ est un anneau et les $V_{\alpha}$ et $V'_{\alpha}$ des idéaux bilatères est triviale en vertu des axiomes (VL_I), (VL_II) et (VL_III). Si $a$ est un idéal (à gauche, par exemple) de $A$ et si $x \neq 0$ appartient à $A$, tout $y \in A$ tel que $\nu(y) \geqslant \nu(x)$ peut s’écrire $y = zx$ avec $z = yx^{-1}$, donc $\nu(z) = \nu(y) - \nu(x) \geqslant 0$, et par suite $z \in A$; autrement dit l’idéal à gauche $Ax$ contient les $V'_{\alpha}$ pour $x \geqslant \nu(x)$. L’ensemble $U(A) = A - m(A)$ est l’ensemble des $x \in K$ tels que $\nu(x) = 0$; si $x \in U(A)$ on a
$$
\nu(x^{-1}) = -\nu(x) = 0,
$$
d’où $x^{-1} \in U(A)$; réciproquement, si $y \in A$ est inversible dans $A$, on a $\nu(y) \geqslant 0$, $\nu(y^{-1}) \geqslant 0$ et $\nu(y) + \nu(y^{-1}) = 0$, d’où $\nu(y) = 0$ et $y \in U(A)$; ceci prouve (iv), et (v) découle aussitôt des définitions.

On dit que $A$ (resp. $m(A)$, $\kappa(A)$) est l’anneau (resp. l’idéal, le corps résiduel) de la valuation $\nu$ sur $K$.

Il est clair que $U(A)$ est le noyau de l’homomorphisme $\nu : K^* \to \Gamma$, et que l’image $\nu(K^*)$ par $\nu$ du groupe multiplicatif $K^*$ est un sous-groupe du groupe additif $\Gamma$, dit groupe des ordres ou groupe des valeurs de $\nu$, qui est donc isomorphe à $K^*/U(A)$; pour un $x \in K$, l’élément $\nu(x)$ de $\Gamma_\infty$ est parfois appelé la valuation ou l’ordre de $x$ pour $\nu$. On dit que deux valuations $\nu, \nu'$ de $K$ sont équivalentes si elles ont même anneau.

#### Proposition 3 {#ac-vi-s3-prop-3 .statement}

Pour que deux valuations $\nu, \nu'$ sur un corps (non nécessairement commutatif) $K$ soient équivalentes, il faut et il suffit qu’il existe un isomorphisme $\lambda$ du groupe ordonné $\nu(K^*)$ sur le groupe ordonné $\nu'(K^*)$ tel que $\nu' = \lambda \circ \nu$.

En effet, supposons $\nu$ et $\nu'$ équivalentes; par hypothèse, l’anneau $A$ de la valuation $\nu$ étant le même que celui de $\nu'$, $\nu$ et $\nu'$ (restreints à $K^*$) se factorisent en des homomorphismes $K^* \to K^*/U(A) \xrightarrow{\mu} \nu(K^*)$, $K^* \to K^*/U(A) \xrightarrow{\nu'} \nu'(K^*)$, où $\mu$ et $\nu$ sont des isomorphismes; en outre, l’ensemble des éléments positifs de $\nu(K^*)$ (resp. $\nu'(K^*)$) est l’image par $\mu$ (resp. $\nu$) de l’ensemble des classes mod. $U(A)$ des éléments $\neq 0$ de $m(A)$; on en conclut que $\lambda = \nu \circ \mu^{-1}$ répond à la question, la réciproque étant évidente.

Supposons maintenant que $K$ soit un corps *commutatif*; alors, pour toute valuation $\nu$ de $K$, l’anneau $A$ de la valuation $\nu$ est un *anneau de valuation pour* $K$ au sens du § 1, no 2, déf. 2 (ce qui justifie la terminologie); cela résulte aussitôt de la prop. 2, c) et du § 1, no 2, th. 1, c). *Inversement*, rappelons que pour tout anneau intègre $B$ dont $K$ est le corps des fractions, la relation de divisibilité $x|y$ (équivalente à $y \in Bx$) fait de $K^*$ un groupe préordonné, dont le *groupe ordonné associé* $\Gamma_B$ est le quotient $K^*/U(B)$ de $K^*$ par le groupe $U(B)$ des éléments inversibles de $B$, les éléments positifs de ce groupe étant ceux de $B^*/U(B)$ (où $B^* = B - \{0\}$); l’application $x \to Bx$ définit, par passage au quotient, un isomorphisme du groupe ordonné $K^*/U(B)$ sur le groupe (ordonné par la relation $\supseteq$) des idéaux fractionnaires principaux non nuls de $K$ (*Alg.*, chap. VI, § 1, no5). Les anneaux $A$ ayant pour corps des fractions $K$ et pour lesquels le groupe $\Gamma_A = K^*/U(A)$ est *totalement ordonné* sont précisément les *anneaux de valuation pour* $K$ (§ 1, no 2, th. 1, d)). Si l’on désigne par $\nu_A$ l’homomorphisme canonique de $K^*$ sur $\Gamma_A$, il est immédiat que $\nu_A$ (prolongé par $\nu_A(0) = +\infty$) est une *valuation* (dite *canonique*) de $K$ dont l’anneau est $A$; toute valuation équivalente à $\nu_A$ s’écrit $\nu = \sigma \circ \nu_A$, où $\sigma$ est un isomorphisme de $\Gamma_A$ sur un sous-groupe du groupe où $\nu$ prend ses valeurs (prop. 3); on dit que $\sigma \circ \nu_A$ est la *factorisation canonique de* $\nu$.

#### Proposition 4 {#ac-vi-s3-prop-4 .statement}

*Soient* $C$ *un anneau intègre, K son corps des fractions, $C^* = C - \{0\}$, et $\nu : C \to \Gamma_\infty$ *une valuation de* $C$ *telle que* $\nu(x) \neq +\infty$ *pour* $x \in C^*$. *Il existe alors une valuation* $\omega$ *et une seule de* $K$ *qui prolonge* $\nu$, *et* $\omega(K^*)$ *est le sous-groupe de* $\Gamma$ *engendré par* $\nu(C^*)$.

D’après le th. 2 d’*Alg.*, chap. I, § 2, no 7, il existe un homomorphisme $\omega$ et un seul de $K^*$ dans $\Gamma$ qui prolonge $\nu|C^*$, et $\omega(K^*)$ est engendré par $\nu(C^*)$. Il reste à prouver que $\omega$ vérifie l’axiome (VL$_\mathrm{II}$). Soient donc $x \in K^*$, $y \in K^*$ tels que $x + y \in K^*$; il

existe $a \in C^*$ tel que $ax \in C^*$ et $ay \in C^*$, d’où $a(x + y) \in C^*$. Puisque la restriction de $\omega$ à $C^*$ vérifie (VL$_{\text{II}}$) on a
$$
\omega(a(x + y)) \geq \inf (\omega(ax), \omega(ay)).
$$
Retranchant $\omega(a)$ des deux membres, on obtient bien
$$
\omega(x + y) \geq \inf (\omega(x), \omega(y)).
$$

### 3. Traductions

Soient $K$ un corps (commutatif), $f$ une place de $K$, $\nu$ une valuation de $K$, et $A$ un anneau de valuation pour $K$. Nous dirons que $A, f$ et $\nu$ sont *associés*, si $A$ est l’anneau de $f$ et l’anneau de $\nu$. En vertu du no 1 et du § 2, no 3, chacun des trois objets $A, f$ et $\nu$ détermine alors les deux autres (à une équivalence près en ce qui concerne les places et les valuations). On a en particulier les équivalences suivantes :

$$
\begin{array}{lll}
x \in A & \iff f(x) \neq \infty & \iff \nu(x) \geq 0 \\
x \in m(A) & \iff f(x) = 0 & \iff \nu(x) > 0 \\
x \in A - m(A) = U(A) & \iff f(x) \neq 0 \text{ et } f(x) \neq \infty & \iff \nu(x) = 0 \\
x \in K - A & \iff f(x) = \infty & \iff \nu(x) < 0.
\end{array}
$$

Tout résultat portant sur les anneaux de valuation, les places ou les valuations se traduit en un résultat portant sur les deux autres notions. Ainsi la prop. 4 du § 2, no 4, donne :

#### Proposition 5 {#ac-vi-s3-prop-5 .statement}

*Soient K un corps, $\nu$ une valuation de K et K' une extension de K. Il existe une valuation $\nu'$ de K' dont la restriction à K est équivalente à $\nu$.*

Soient $\Gamma_\nu$ et $\Gamma_{\nu'}$ les groupes des ordres de $\nu$ et $\nu'$. Puisque la restriction de $\nu'$ à K est équivalente à $\nu$, il existe un isomorphisme $\lambda$ de $\Gamma_\nu$ sur un sous-groupe de $\Gamma_{\nu'}$, tel que $\nu' = \lambda \circ \nu$ sur K. Si l’on identifie $\Gamma_\nu$ à $\lambda(\Gamma_\nu)$ au moyen de $\lambda$, on voit que $\nu'$ prolonge $\nu$.

On notera que $\Gamma_{\nu'}$ est en général *distinct de* $\lambda(\Gamma_\nu)$, et que la classe d’équivalence de $\nu'$ n’est pas nécessairement unique. Nous reviendrons là-dessus au § 8.

En traduisant le th. 3 du § 1, no 3 (ou la prop. 6 du § 2, no 5) on obtient :

#### Proposition 6 {#ac-vi-s3-prop-6 .statement}

*Soient K un corps, A un sous-anneau de K, et x un élément de K. Pour que x soit entier sur A, il faut et il suffit que toute valuation de K positive dans A soit positive en x.

A partir de maintenant, nous laisserons en général au lecteur le soin d’effectuer des traductions analogues aux précédentes.

### 4. Exemples de valuations

Les exemples d’anneaux de valuation donnés au § 1, no 4, nous fournissent les exemples 1 à 4 ci-dessous:

#### Exemple 1 {#ac-vi-s3-n4-exa-1 .statement}

Toute valuation d’un corps fini F est impropre, puisque tout élément de F* est une racine de l’unité.

#### Exemple 2 {#ac-vi-s3-n4-exa-2 .statement}

Si K est un sous-corps d’un corps K’, la restriction à K d’une valuation de K’ est une valuation de K.

#### Exemple 3 {#ac-vi-s3-n4-exa-3 .statement}

Soient k un corps, et K = k((T)). L’application υ qui, à toute série formelle non nulle, fait correspondre son ordre (Alg., chap. IV, § 5, no 7), est une valuation de K dont le groupe des ordres est Z, et l’anneau k[[T]]. La place associée est l’homomorphisme canonique f : k[[T]] → k, prolongé à k((T)) en posant f(u) = ∞ si u ∉ k[[T]].

#### Exemple 4 {#ac-vi-s3-n4-exa-4 .statement}

Soient A un anneau principal, K son corps des fractions, et p un élément extrémal de A. Pour x ∈ K*, notons υ_p(x) l’exposant de p dans la décomposition de x en éléments extrémaux (Alg., chap. VII, § 1, no 3, th. 2); on voit aussitôt que υ_p est une valuation, dont le groupe des ordres est Z et l’anneau A_{A_p}. D’après la prop. 3 du § 1, no 4, on obtient ainsi, à une équivalence près, toutes les valuations non impropres de K qui sont positives sur A. Prenant A = Z, on retrouve les valuations p-adiques de Q (Top. Gén., chap. IX, § 3, no 2); ces valuations sont, à une équivalence près, les seules valuations non impropres de Q (§ 1, no 4, cor. 1 de la prop. 3). Prenant A = k[X], où k est un corps, les valuations non impropres de k(X) dont la restriction à k est impropre sont (à une équivalence près): d’une part les valuations υ_P où P parcourt l’ensemble des polynômes unitaires irréductibles de k[X], d’autre part la valuation υ définie par υ(P/Q) = deg(Q) − deg(P) pour P ∈ k[X] et Q ∈ k[X] (§ 1, no 4, cor. 2 de la prop. 3); toutes ces valuations ont évidemment Z pour groupe des ordres, et leurs corps résiduels sont des extensions algébriques monogènes de k (Alg., chap. V, § 3, no 1).

La proposition 4 du no 2 permet de construire une valuation dont le groupe des ordres et le corps résiduel sont donnés :

#### Exemple 6 {#ac-vi-s3-n4-exa-6 .statement}

Soient $\Gamma$ un groupe totalement ordonné, et $k$ un corps. Soient $\Gamma_+$ le monoïde des éléments positifs de $\Gamma$, et $C$ l’algèbre de $\Gamma_+$ sur $k$. Par définition, $C$ possède une base $(x_\alpha)_{\alpha \in \Gamma_+}$ sur $k$ dont la table de multiplication est $x_\alpha x_\beta = x_{\alpha + \beta}$. Si $x = \sum_\alpha a_\alpha x_\alpha$ est un élément non nul de $C$, posons $\nu(x) = \inf_{a_\alpha \neq 0} (\alpha)$ et posons $\nu(0) = + \infty$; on vérifie immédiatement que l’application $\nu$ de $C$ dans $\Gamma_\infty$ satisfait aux conditions (VL_I) et (VL_{II}) du no 1, et que $C$ est intègre. Soient $K$ le corps des fractions de $C$, et $\omega$ la valuation de $K$ qui prolonge $\nu$ (prop. 4, no 2). Comme tout élément de $\Gamma$ est différence de deux éléments positifs, $\omega$ admet $\Gamma$ pour groupe des ordres. Soient $A$ l’anneau de $\omega$, et $m$ son idéal maximal; on va montrer que $A$ est somme directe de $m$ et de $k$ (identifié à $k.1$), ce qui prouvera que le corps résiduel de $\omega$ est isomorphe à $k$. Il est clair que $m \cap k = (0)$. D’autre part, en notant $p$ l’idéal de $C$ engendré par les $x_\alpha$ où $\alpha > 0$, tout élément $x$ de valuation 0 dans $K$ se met sous la forme $(a + y)/(b + z)$ avec $a \in k^*, b \in k^*, y \in p$ et $z \in p$; on a alors

$$
x = ab^{-1} + (by - az)\ b^{-1}(b + z)^{-1}
$$

d’où $\omega(x - ab^{-1}) > 0$ et $x \equiv ab^{-1}$ (mod. $m$); ceci démontre notre assertion.

Si $\Gamma = \mathbf{Z} \times \mathbf{Z}$, on a $K = k(X, Y)$, et la construction précédente fournit donc des valuations de $k(X, Y)$, impropres sur $k$, dont le groupe des ordres est $\mathbf{Z} \times \mathbf{Z}$ et le corps résiduel $k$. Ces valuations dépendent de la structure d’ordre choisie sur $\mathbf{Z} \times \mathbf{Z}$. On peut, par exemple, munir $\mathbf{Z} \times \mathbf{Z}$ de l’ordre lexicographique. Ou bien, $\alpha$ étant un nombre irrationnel, on peut identifier $\mathbf{Z} \times \mathbf{Z}$ à un sous-groupe de $\mathbf{R}$ par l’homomorphisme $(m, n) \to m + n\alpha$ (homomorphisme qui est injectif car $\alpha$ est irrationnel), et munir $\mathbf{Z} \times \mathbf{Z}$ de l’ordre induit par celui de $\mathbf{R}$.

### 5. Idéaux d’un anneau de valuation

#### Définition 2 {#ac-vi-s3-def-2 .statement}

Soit G un ensemble ordonné. Un sous-ensemble M de G est dit majeur si les relations $x \in M$ et $y \geq x$ entraînent $y \in M$.

Soient K un corps, $\varphi$ une valuation de K, A l’anneau de $\varphi$, et G le groupe des ordres de $\varphi$. Pour tout ensemble majeur $M \subset G$, soit $a(M)$ l’ensemble des $x \in K$ tels que $\varphi(x) \in M \cup \{ +\infty \}$. Il est clair que $a(M)$ est un sous-A-module de K.

#### Proposition 7 {#ac-vi-s3-prop-7 .statement}

L’application $M \to a(M)$ est une bijection croissante de l’ensemble des sous-ensembles majeurs de G sur l’ensemble des sous-A-modules de K.

Soit $b$ un sous-A-module de K. L’ensemble des $\varphi(x)$ pour $x \in b - (0)$ est un sous-ensemble majeur $M(b)$ de G. La prop. 7 sera démontrée si l’on prouve les formules :
(2) $M(a(N)) = N$ pour tout sous-ensemble majeur N de G;
(3) $a(M(b)) = b$ pour tout sous-A-module $b$ de K.

La formule (2) est facile, car, pour tout $m \in N$, il existe $x \in K$ tel que $\varphi(x) = m$. On a évidemment $b \subset a(M(b))$; inversement, soit $x \in a(M(b))$ et supposons $x \neq 0$; on a $\varphi(x) \in M(b)$, donc il existe $y \in b$ tel que $\varphi(x) = \varphi(y)$; d’où $x = uy$ avec $\varphi(u) = 0$, ce qui prouve qu’on a $x \in Ay \subset b$, et termine la démonstration.

Corollaire. Soit $G_+$ l’ensemble des éléments positifs de G. L’application $M \to a(M)$ est une bijection de l’ensemble des sous-ensembles majeurs de $G_+$ sur l’ensemble des idéaux de A.

En effet, comme $A = a(G_+)$, $a(M) \subset A$ équivaut à $M \subset G_+$.

Par exemple l’idéal maximal $m(A)$ est égal à $a(S)$, où S désigne l’ensemble des éléments strictement positifs de G.

### 6. Valuations discrètes

#### Définition 3 {#ac-vi-s3-def-3 .statement}

Soient K un corps (non nécessairement commutatif), $\varphi$ une valuation de K, et $\Gamma$ le groupe des ordres de $\varphi$. On dit que $\varphi$ est discrète s’il existe un isomorphisme (nécessairement unique) du groupe ordonné $\Gamma$ sur $\mathbf{Z}$. Soit $\gamma$ l’élément de $\Gamma$ correspondant à 1 par cet isomorphisme; tout élément u de K tel que $v(u) = \gamma$ s’appelle une uniformisante de $v$. Une valuation discrète est dite normée si son groupe des ordres est $\mathbf{Z}$.

Par exemple la valuation $\nu_p$ définie par un élément extrémal $p$ d’un anneau principal *ou factoriel*, est une valuation discrète normée qui admet $p$ pour uniformisante. En particulier, si $k$ est un corps, $k[[T]]$ est l’anneau d’une valuation discrète de $k((T))$, qui admet T pour uniformisante. *Soient S une variété analytique complexe connexe de dimension 1, K le corps des fonctions méromorphes sur S, et $z_0$ un point de S; l’ensemble des $f \in K$ qui sont holomorphes en $z_0$ est l’anneau d’une valuation discrète $\nu$; pour qu’une fonction $f \in K$ soit une uniformisante pour $\nu$, il faut et il suffit qu’elle soit holomorphe et nulle en $z_0$ et qu’il existe un voisinage V de $z_0$ dans S tel que la restriction de $f$ à V soit homéomorphisme de V sur un voisinage de l’origine dans $\mathbf{C}$. C’est cet exemple, et d’autres analogues, qui sont à l’origine du mot « uniformisante »*.

#### Proposition 8 {#ac-vi-s3-prop-8 .statement}

Soient K un corps (non nécessairement commutatif), $\nu$ une valuation discrète de K, A l’anneau de $\nu$, et u une uniformisante pour $\nu$. Les idéaux non nuls de A sont bilatères et de la forme $Au^n (n \geqslant 0)$.

On peut supposer $\nu$ normée, de sorte que $\nu(u) = 1$. Pour tout $x \in K^*$, il y a un entier $n \in \mathbf{Z}$ tel que $\nu(x) = n = \nu(u^n)$, donc on peut écrire $x = zu^n = u^n z'$, où $z, z'$ sont deux éléments inversibles de l’anneau A; d’où la proposition.

#### Proposition 9 {#ac-vi-s3-prop-9 .statement}

Soit A un anneau local intègre distinct de son corps des fractions. Les conditions suivantes sont équivalentes:

a) A est l’anneau d’une valuation discrète.
b) A est principal.
c) L’idéal $m(A)$ est principal, et on a $\bigcap_{n=1}^{\infty} m(A)^n = (0)$.
d) A est un anneau noethérien et $m(A)$ est principal.
e) A est un anneau de valuation noethérien.

La prop. 8 montre que a) entraîne b), d) et e). Si A est principal, on a $m(A) = Au$ et tout idéal non nul de A est de la forme $Au^n$ puisque A est local (Alg., chap. VII, § 1, no 3, th. 2); on a donc $\bigcap_{n=0}^{\infty} m(A)^n = 0$; ceci montre que b) implique c). D’autre part d) implique c) (chap. III, § 3, no 2, cor. de la prop. 5);

#### Lemme 1 {#ac-vi-s3-lem-1 .statement}

Soit $\mathbf{A}$ un anneau de valuation. Tout $\mathbf{A}$-module sans torsion de type fini est libre. Tout idéal de type fini de $\mathbf{A}$ est principal. Tout $\mathbf{A}$-module sans torsion est plat.

Soit E un $\mathbf{A}$-module sans torsion de type fini, et soient $x_1, \ldots, x_n$ des générateurs de E en nombre minimum; montrons qu’ils sont linéairement indépendants. Si $\sum_{i=1}^n a_i x_i = 0$ ($a_i \in \mathbf{A}$) est une relation non triviale entre les $x_i$, l’un des $a_i$, soit $a_1$, divise tous les autres puisque l’ensemble des idéaux principaux de $\mathbf{A}$ est totalement ordonné par inclusion ($§ 1$, n° 2, th. 1); on a $a_1 \neq 0$ puisque la relation est non triviale. Comme E est sans torsion, on peut diviser par $a_1$, ce qui revient à supposer qu’on a $a_1 = 1$. Mais alors $x_1$ est combinaison linéaire de $x_2, \ldots, x_n$, contrairement au caractère minimal de $n$. Donc E est libre.

En particulier tout idéal $a$ de type fini de $\mathbf{A}$ est principal, tous les éléments d’un système de générateurs de $a$ étant multiples de l’un d’eux. La prop. 3 du chap. I, § 2, n° 4 montre alors que tout $\mathbf{A}$-module sans torsion est plat.

## EXERCICES {#ac-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
