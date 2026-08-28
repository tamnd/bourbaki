---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 0
section_title: Algèbres alternatives. Octonions
appendix: true
lang: fr
source: alg-i-iii-fr
book_pages: A III.203
pdf_pages: 0559-0565, 0590-0590
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres alternatives
      page: 172
      pdf_page: 559
    - "no": 2
      title: Algèbres cayleyennes alternatives
      page: 174
      pdf_page: 561
    - "no": 3
      title: Octonions
      page: 176
      pdf_page: 563
statements: 11
exercises: 3
content_sha256: 3a47a3d2be32bed91a1d03fa3ff7423d81ccf2e7b20b7bab881dbeb7405ff7a3
---

## APPENDICE

# ALGÈBRES ALTERNATIVES. OCTONIONS

### 1. Algèbres alternatives

Soient A un anneau commutatif, F une A-algèbre (non nécessairement associative). Pour trois éléments quelconques $x, y, z$ de F, on pose
(1)
$$
a(x, y, z) = x(yz) - (xy)z
$$

(associateur de $x, y, z$); $a$ est évidemment une application A-trilinéaire de $\mathbf{F} \times \mathbf{F} \times \mathbf{F}$ dans $\mathbf{F}$.

#### Lemme 1 {#alg-iii-a0-lem-1 .statement}

Quels que soient $p, q, r, s$ dans l’algèbre $\mathbf{F}$, on a
$$
a(pq, r, s) - a(p, qr, s) + a(p, q, rs) = a(p, q, r)s + pa(q, r, s).
$$
La vérification résulte aussitôt de la définition (1).

#### Proposition 1 {#alg-iii-a0-prop-1 .statement}

Pour une A-algèbre $\mathbf{F}$, les conditions suivantes sont équivalentes:
a) Pour tout couple d’éléments $x, y$ de $\mathbf{F}$, la sous-algèbre engendrée par $x$ et $y$ est associative.
b) L’application trilinéaire $(x, y, z) \mapsto a(x, y, z)$ est alternée (III, p. 80).
c) Pour tout couple d’éléments $x, y$ de $\mathbf{F}$, on a $x^2y = x(xy)$ et $yx^2 = (yx)x$.
Il est clair que a) implique c). Montrons que c) implique b): en effet, par définition (III, p. 80), pour prouver b), il suffit de vérifier que $a(x, x, y) = 0$ et $a(x, y, y) = 0$, ce qui n’est autre que c).

Pour établir l’implication $b) \Rightarrow a)$, nous prouverons les 4 lemmes suivants.

#### Lemme 2 {#alg-iii-a0-lem-2 .statement}

Soient $\mathbf{E}$ une A-algèbre telle que l’application trilinéaire $(x, y, z) \mapsto a(x, y, z)$ soit alternée, $S$ un système générateur de $\mathbf{E}$, $\mathbf{U}$ un sous-A-module de $\mathbf{E}$ contenant $S$ et tel que $s\mathbf{U} \subset \mathbf{U}$ et $\mathbf{Us} \subset \mathbf{U}$ pour tout $s \in S$. Alors on a $\mathbf{U} = \mathbf{E}$.
En effet, l’ensemble $\mathbf{U}'$ des $x \in \mathbf{E}$ tels que $x\mathbf{U} \subset \mathbf{U}$ et $\mathbf{U}x \subset \mathbf{U}$ est évidemment un sous-A-module de $\mathbf{E}$, qui contient $S$ par hypothèse. D’autre part, pour $x, y$ dans $\mathbf{U}'$ et $u \in \mathbf{U}$, on a par hypothèse
$$
(xy)u = x(yu) + a(x, y, u) = x(yu) - a(x, u, y) = x(yu) - (xu)y + x(uy) \in \mathbf{U};
$$
par passage à l’algèbre opposée, on a de même $u(xy) \in \mathbf{U}$. Donc $\mathbf{U}'$ est une sous-algèbre de $\mathbf{E}$, et puisqu’elle contient $S$, on a $\mathbf{U}' = \mathbf{E}$. On a donc $\mathbf{EU} \subset \mathbf{U}$, et $a$ fortiori $\mathbf{UU} \subset \mathbf{U}$, ce qui prouve que $\mathbf{U}$ est une sous-algèbre de $\mathbf{E}$; comme elle contient $S$, on a $\mathbf{U} = \mathbf{E}$, ce qui démontre le lemme.

Disons qu’une partie $\mathbf{H}$ de $\mathbf{F}$ est fortement associative si $a(u, v, w) = 0$ lorsque deux au moins des éléments $u, v, w$ appartiennent à $\mathbf{H}$.

#### Lemme 3 {#alg-iii-a0-lem-3 .statement}

Supposons l’application $a$ alternée. Si $\mathbf{H}$ est une partie fortement associative de $\mathbf{F}$, la sous-algèbre de $\mathbf{F}$ engendrée par $\mathbf{H}$ est fortement associative.
Comme l’ensemble des parties fortement associatives de $\mathbf{F}$ est inductif, il suffit de prouver que si $\mathbf{H}$ est une partie fortement associative maximale de $\mathbf{F}$, $\mathbf{H}$ est alors une sous-algèbre de $\mathbf{F}$. Comme $\mathbf{H}$ est évidemment un sous-A-module de $\mathbf{F}$, il suffit de voir que pour deux éléments quelconques $u, v$ de $\mathbf{H}$, $\mathbf{H} \cup \{uv\}$ est encore fortement associative, car en vertu de la définition de $\mathbf{H}$, cela entraînera $uv \in \mathbf{H}$. Or, pour tout $z \in \mathbf{H}$ et tout $t \in \mathbf{F}$, on a en vertu de (2)
$$
a(uv, t, z) - a(u, vt, z) + a(u, v, tz) = 0
$$
puisque $\mathbf{H}$ est fortement associative; comme $u, v, z$ sont dans $\mathbf{H}$, on a aussi a(u, vt, z) = a(u, v, tz) = 0, d’où $a(uv, t, z) = 0$. Compte tenu de ce que $a$ est alternée, cela montre que $a(p, q, r) = 0$ chaque fois que deux au moins des éléments $p, q, r$ appartiennent à $\mathrm{H} \cup \{uv\}$, d’où le lemme.

#### Lemme 4 {#alg-iii-a0-lem-4 .statement}

*Supposons l’application a alternée. Alors, pour tout $x \in \mathbf{F}$, la sous-algèbre de $\mathbf{F}$ engendrée par $x$ est fortement associative.*

En effet, on a $a(u, v, w) = 0$ chaque fois que deux des trois éléments $u, v, w$ sont égaux à $x$, et il suffit d’appliquer le lemme 3.

#### Lemme 5 {#alg-iii-a0-lem-5 .statement}

*Supposons l’application a alternée, et soient $X, Y$ deux sous-algèbres fortement associatives de $\mathbf{F}$. Alors la sous-algèbre $E$ engendrée par $X \cup Y$ est associative.*

En effet, soit $Z$ l’ensemble des $z \in E$ tels que $a(u, v, z) = 0$ quels que soient $u \in X$ et $v \in Y$; c’est évidemment un sous-A-module contenant $X$ et $Y$ puisque $X$ et $Y$ sont fortement associatives; en vertu du lemme 2, il suffira de voir que pour $u \in X$ et $v \in Y$, on a $uZ \subset Z, vZ \subset Z, Zu \subset Z$ et $Zv \subset Z$. Or, pour $u, u'$ dans $X, v \in Y$ et $z \in Z$, on a d’après (2) (III, p. 173)

$$
a(u'u, z, v) - a(u', uz, v) + a(u', u, zv) = a(u', u, z)v + u'a(u, z, v) = 0
$$

en vertu du fait que $X$ est fortement associative et de la définition de $Z$. Mais comme $X$ est fortement associative, $a(u', u, zv) = 0$ et puisque $u'u \in X$, $a(u'u, z, v) = 0$ par définition de $Z$. On a donc bien $a(u', uz, v) = 0$ ce qui montre que $uZ \subset Z$. En appliquant maintenant (2) avec $(p, q, r, s) = (v, z, u, u')$, on obtient de même $Zu \subset Z$. Echangeant les rôles de $X$ et $Y$ (en tenant compte de ce que $a$ est alternée), on obtient $vZ \subset Z$ et $Zv \subset Z$; d’où le lemme.

Il suffit maintenant, pour achever de montrer que b) implique a) dans la prop. 1, de prendre $X = \{x\}$ et $Y = \{y\}$, en utilisant le lemme 4.

#### Définition 1 {#alg-iii-a0-def-1 .statement}

*On dit qu’une A-algèbre $F$ est alternative si elle satisfait aux condition équivalentes de la prop. 1.*

Une algèbre associative est évidemment alternative. Nous donnerons dans III, p. 176 un exemple d’algèbre alternative qui n’est pas associative.

Si $F$ est une A-algèbre alternative, toute A-algèbre $F \otimes_A A'$ obtenue à partir de $F$ par extension des scalaires (III, p. 7) est une $A'$-algèbre alternative, comme il résulte de la condition b) de la prop. 1.

### 2. Algèbres cayleyennes alternatives

#### Proposition 2 {#alg-iii-a0-prop-2 .statement}

*Soient $A$ un anneau, $F$ une A-algèbre cayleyenne, e son élément unité, $s : x \mapsto \bar{x}$ sa conjugaison, $N : F \to A$ sa norme cayleyenne (III, p. 15).

(i) *Pour que $F$ soit alternative, il faut et il suffit que l’on ait, pour tout couple d’éléments $x, y$ de $F$, $x^2y = x(xy)$.*

(ii) *Si $F$ est alternative, on a $N(xy) = N(x)N(y)$ quels que soient $x, y$ dans $F$.*

(iii) Supposons F alternative. Pour qu’un élément x ∈ F soit inversible il faut et il suffit que N(x) soit inversible dans Ae; l’inverse de x est alors unique et égal à N(x)^{-1}\bar{x}; en le notant x^{-1}, on a

$$
x^{-1}(xy) = x(x^{-1}y) = y
$$

pour tout y ∈ F.

La condition x^2y = x(xy) est évidemment nécessaire pour que F soit alternative (III, p. 173, prop. 1). Inversement, si elle est vérifiée pour tout couple d’éléments de F, en l’appliquant à \bar{x} et \bar{y}, elle donne \bar{x}^2\bar{y} = \bar{x}(\bar{x}\bar{y}); appliquant à cette relation la conjugaison s, il vient yx^2 = (yx)x, de sorte que les conditions c) de la prop. 1 de III, p. 173 sont satisfaites.

On a évidemment a(e, x, y) = 0 quels que soient x, y dans F. Si F est alternative, on déduit donc de la prop. 1 (III, p. 173) que la sous-algèbre G de F engendrée par e, x et y est associative. Comme \bar{x} = -x + T(x) \in -x + Ae, on a \bar{x} \in G, et de même \bar{y} \in G. Ceci étant, on a N(xy) = (xy)(\bar{x}\bar{y}) = xy.\bar{y}.\bar{x} = N(y)x\bar{x} = N(y)N(x), compte tenu de ce que N(y) \in Ae. Ceci prouve b).

Démontrons enfin c). Si N(x) est inversible dans Ae, et si l’on pose x' = N(x)^{-1}\bar{x}, on a xx' = x'x = e, car N(x) = x\bar{x} = \bar{x}x. Réciproquement, si x admet un inverse à gauche x'', on a N(x'')N(x) = N(e) = e par b), et N(x) est inversible dans Ae; de plus, comme x' = N(x)^{-1}\bar{x} est dans la sous-algèbre engendrée par x et e, les éléments x, x' et x'' appartiennent à la sous-algèbre associative engendrée par x, x'' et e, donc on a x'' = x''(xx') = (x''x)x' = x', d’où l’assertion d’unicité. Les formules x^{-1}(xy) = x(x^{-1}y) = y résultent de ce que x^{-1}, x et y sont éléments de la sous-algèbre engendrée par x, y et e, qui est associative.

C. Q. F. D.

#### Proposition 3 {#alg-iii-a0-prop-3 .statement}

Soient E une A-algèbre cayleyenne, γ un élément de A et F l’extension cayleyenne de E définie par γ et la conjugaison de E (III, p. 17, prop. 5). Pour que F soit alternative, il faut et il suffit que E soit associative.

Soient u = (x, y), v = (x', y') deux éléments de F (x, y, x', y' étant dans E). On a (III, p. 17, formule (27))

$$
\begin{cases}
u^2v = ((x^2 + \gamma\bar{y}y)x' + \gamma\bar{y}'(y\bar{x} + yx), (y\bar{x} + yx)\bar{x}' + y'(x^2 + \gamma\bar{y}y)) \\
u(uv) = (x(xx' + \gamma\bar{y}'y) + \gamma(x'\bar{y} + \bar{x}.\bar{y}')y, y(\bar{x}'\bar{x} + \gamma\bar{y}y') + (y\bar{x}' + y'\bar{x})x).
\end{cases}
$$

En tenant compte de ce que \bar{y}y et \bar{x} + x sont dans Ae, l’examen de ces formules montre que l’associativité de E entraîne u^2v = u(uv), donc le fait que F est alternative (III, p. 174, prop. 2). Réciproquement, si F est alternative, l’égalité u^2v = u(uv) appliquée pour y' = 0 donne

$$(y\bar{x} + yx)\bar{x}' = y(\bar{x}'\bar{x}) + (y\bar{x}')x.$$

Or le premier membre est égal à (yT(x))\bar{x}' = y(\bar{x}'T(x)) = y(\bar{x}'x + \bar{x}'\bar{x}); comparant au second membre, il vient (y\bar{x}')x = y(\bar{x}'x), ce qui prouve l’associativité de E, puisque x, y et \bar{x}' sont arbitraires dans E.

C. Q. F. D.

### 3. Octonions

Soit E une algèbre de quaternions de type $(\alpha, \beta, \gamma)$ sur A (III, p. 18, Exemple 2), et soit $\delta \in A$. L’extension cayleyenne F de E définie par $\delta$ et la conjugaison de E s’appelle une algèbre d’octonions sur A, et on dit qu’elle est de type $(\alpha, \beta, \gamma, \delta)$. En vertu de la prop. 3 de III, p. 175, F est une algèbre alternative. Elle possède une base $(e_i)_{0 \leq i \leq 7}$ de 8 éléments, définis par

$$
\begin{align*}
e_0 &= (e, 0), & e_1 &= (i, 0), & e_2 &= (j, 0), & e_3 &= (k, 0) \\
e_4 &= (0, e), & e_5 &= (0, i), & e_6 &= (0, j), & e_7 &= (0, k)
\end{align*}
$$

où $(e, i, j, k)$ est la base de E définie loc. cit.; il est clair que $e_0$ (aussi noté $e$) est l’élément unité de F. Si $u = \sum_{i=0}^{7} \xi_i e_i$ est un élément de F (avec les $\xi_i \in A$), les formules (23), (24) de III, p. 17 et (31) de III, p. 18 donnent pour le conjugué, la trace et la norme de l’octonion $u$

$$
\left\{
\begin{aligned}
\overline{u} &= (\xi_0 + \beta \xi_1)e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 + \beta \xi_1 \\
N_F(u) &= \xi_0^2 + \beta \xi_0 \xi_1 - \alpha \xi_1^2 - \gamma (\xi_2^2 + \beta \xi_2 \xi_3 - \alpha \xi_3^2) \\
&\quad - \delta (\xi_4^2 + \beta \xi_4 \xi_5 - \alpha \xi_5^2) + \gamma \delta (\xi_6^2 + \beta \xi_6 \xi_7 - \alpha \xi_7^2)
\end{aligned}
\right.
$$

Soient maintenant $u = (x, y)$, $u' = (x', y')$ et $u'' = (x'', y'')$ trois octonions (les éléments $x, x', x'', y, y', y''$ appartenant à E). Les formules (24) et (27) de III, p. 17 donnent

$$
\begin{align*}
T_F((uu')u'') &= T(xx'x'') + \delta T(\overline{y}'y x'') + \delta T(\overline{y}''y \overline{x}') + \delta T(\overline{y}''y' x) \\
T_F(u(u'u'')) &= T(xx'x'') + \delta T(x''y'y) + \delta T(\overline{x}' \overline{y}''y) + \delta T(x \overline{y}''y')
\end{align*}
$$

(où T désigne la trace dans E et où l’on tient compte de ce que E est associative). Comme $T(xy) = T(yx)$ quels que soient les quaternions $x, y$ (III, p. 16, formule (17)), on en déduit

$$
T_F((uu')u'') = T_F(u(u'u''))
$$

Etudions en particulier les octonions de type $(-1, 0, -1, -1)$: les formules (4) se simplifient alors en

$$
\left\{
\begin{aligned}
\overline{u} &= \xi_0 e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 \\
N_F(u) &= \sum_{i=0}^{7} \xi_i^2.
\end{aligned}
\right.
$$

\* Si l’on prend pour A le corps $\mathbf{R}$ des nombres réels, les octonions de type $(-1, 0, -1, -1)$ sur $\mathbf{R}$ s’appellent les octonions (ou octaves) de Cayley. Il résulte de la prop. 2, (ii) de III, p. 174 que tout octonion de Cayley $\neq 0$ est inversible.*

#### Proposition 4 {#alg-iii-a0-prop-4 .statement}

Soit F une algèbre d’octonions de type (−1, 0, −1, −1) sur A. Il existe un espace vectoriel V de dimension 3 sur le corps à deux éléments $\mathbf{Z}/2\mathbf{Z}$ et une bijection $\lambda \mapsto e'_\lambda$ de V sur la base $(e_i)_{0 \leq i \leq 7}$ telle que

(7)
$$
e'_0 = e_0, \quad e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}
$$
quels que soient $\lambda, \mu$ dans V. Pour qu’on ait $e'_\lambda(e'_\mu e'_v) = (e'_\lambda e'_\mu)e'_v$, il suffit que, dans V, $\lambda, \mu, v$, soient linéairement dépendants sur $\mathbf{Z}/2\mathbf{Z}$; cette condition est nécessaire si $2 \neq 0$ dans A.

Gardons les notations du début de ce n°. Il résulte des formules (33) de III, p. 18, que l’ensemble S formé des éléments $\pm e_0, \pm e_1, \pm e_2, \pm e_3$ est stable pour la multiplication. En outre, pour $x, y, y'$ dans E, on a, en vertu de la formule (22) de III, p. 16,

(8)
$$
(x, 0)(0, y') = (0, y'x), \quad (0, y')(x, 0) = (0, y'\bar{x}), \quad (0, y)(0, y') = (-\bar{y}'y, 0)
$$
de sorte que l’ensemble T formé des éléments $\pm e_i$ ($0 \leq i \leq 7$) est stable pour la multiplication; en outre, sa table de multiplication est indépendante de l’anneau A.

En particulier, soient A'' le corps $\mathbf{Z}/2\mathbf{Z}$ à deux éléments, et soient E'' l’algèbre des quaternions de type (1, 0, 1) sur A'', F'' l’algèbre des octonions de type (1, 0, 1, 1) sur A''; soit $(e''_i)_{0 \leq i \leq 7}$ la base de F'' formée comme ci-dessus. Puisque $-e''_i = e''_i$, l’ensemble T'' des $e''_i$ a 8 éléments et est stable par la multiplication; en outre, il résulte aussitôt de ce qui précède que l’application $\theta : T \to T''$ telle que $\theta(e_i) = \theta(-e_i) = e''_i$ pour $0 \leq i \leq 7$ est un homomorphisme pour la multiplication. D’ailleurs l’algèbre des quaternions E'' est ici commutative, donc F'' est associative (III, p. 17, prop. 5); de plus, la conjugaison dans F'' est ici l’identité. Donc T'' est un groupe, et les formules (8) montrent qu’il est commutatif; ces formules et les formules (33) de III, p. 18 montrent que le carré de tout élément de T'' est l’unité. Si l’on désigne par V le groupe T'' écrit en notation additive, V peut être muni d’une seule manière d’une structure d’espace vectoriel sur $\mathbf{Z}/2\mathbf{Z}$, nécessairement de dimension 3 puisque Card(V) = 8 = $2^{\dim(V)}$.

Pour tout $\lambda \in V$, notons alors $e'_\lambda$ l’élément de $(e_i)_{0 \leq i \leq 7}$ tel que $\theta(e'_\lambda) = \lambda$; on a $e'_0 = e_0$; en outre, comme $\theta$ est un homomorphisme et que la relation $\theta(x) = \theta(y)$ équivaut à $x = \pm y$, on a $e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}$. Si $\lambda, \mu, v$ sont linéairement indépendants sur $\mathbf{Z}/2\mathbf{Z}$, ils forment une base de V, donc tous les éléments $e_i$ ($0 \leq i \leq 7$) appartiennent à la sous-algèbre engendrée par $e'_\lambda, e'_\mu$ et $e'_v$; lorsque $2 \neq 0$ dans A, on ne peut par suite avoir $e'_\lambda(e'_\mu e'_v) = (e'_\lambda e'_\mu)e'_v$, car F serait associative, donc E serait commutative (III, p. 17, prop. 5), ce qui contredit les relations (33) de III, p. 18. Au contraire, si $\lambda, \mu, v$ sont linéairement dépendants dans V, les trois éléments $e'_\lambda, e'_\mu, e'_v$ appartiennent à une sous-algèbre à 2 générateurs de F, qui est par suite associative (III, p. 173, prop. 1); d’où la conclusion.

#### Remarque {#alg-iii-a0-n3-rem-1 .statement}

Comme $\bar{e}'_\lambda = -e'_\lambda$ pour $\lambda \neq 0$, on a
$$
e'^2_\lambda = -e_0 \quad \text{pour } \lambda \neq 0,
$$
$$
e'_\mu e'_\lambda = -e'_\lambda e'_\mu \quad \text{pour } \lambda \neq 0, \mu \neq 0 \text{ et } \mu \neq \lambda.
$$

Exercises

## EXERCICES {#alg-iii-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
