---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 2
section_title: Exemples d’algèbres
lang: fr
source: alg-i-iii-fr
book_pages: A III.12-A III.30
pdf_pages: 0399-0417, 0565-0570
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres d’endomorphismes
      page: 12
      pdf_page: 399
    - "no": 2
      title: Algèbres de matrices
      page: 12
      pdf_page: 399
    - "no": 3
      title: Algèbres quadratiques
      page: 12
      pdf_page: 399
    - "no": 4
      title: Algèbres cayleyennes
      page: 15
      pdf_page: 402
    - "no": 5
      title: Construction d’algèbres cayleyennes. Quaternions
      page: 16
      pdf_page: 403
    - "no": 6
      title: Algèbre d’un magma, d’un monoïde, d’un groupe
      page: 19
      pdf_page: 406
    - "no": 7
      title: Algèbres libres
      page: 21
      pdf_page: 408
    - "no": 8
      title: Définition d’une algèbre par générateurs et relations
      page: 22
      pdf_page: 409
    - "no": 9
      title: Algèbres de polynômes
      page: 25
      pdf_page: 412
    - "no": 10
      title: Algèbre large d’un monoïde
      page: 27
      pdf_page: 414
    - "no": 11
      title: Séries formelles sur un anneau commutatif
      page: 28
      pdf_page: 415
statements: 20
exercises: 4
content_sha256: 13eb8ae334e2c27bb261675f7ae2326e6c05f328bc68c6450bead53a15ffe82c
---

## § 2. EXEMPLES D’ALGÈBRES

Dans tout ce paragraphe, A désigne un anneau commutatif.

### 1. Algèbres d’endomorphismes

Soit B une A-algèbre associative ayant un élément unité noté 1, et soit M un B-module à droite. On sait que l’anneau $E = \mathrm{End}_B(M)$ est en outre muni d’une structure de module sur le centre de B. Or, l’image de l’homomorphisme $h : \alpha \mapsto \alpha . 1$ de A dans B est contenue dans le centre de B (III, p. 3); donc h munit E d’une structure de A-module. De plus, pour $\alpha \in A$, $f, g$ dans E, on a $\alpha(f \circ g) = f \circ (\alpha g) = (\alpha f) \circ g$; donc la multiplication dans E et la structure de A-module de E définissent sur E une structure de A-algèbre associative; l’application identique de M est élément unité de cette algèbre.

### 2. Algèbres de matrices

Soient B une A-algèbre associative unifère, et $\mathbf{M}_n(B)$ l’ensemble des matrices carrées d’ordre n sur B (II, p. 149). Alors $\mathbf{M}_n(B)$ est muni d’une structure de A-module définie par $\alpha . (b_{ij}) = (\alpha b_{ij})$ ($\alpha \in A$, $b_{ij} \in B$, $1 \leq i \leq n, 1 \leq j \leq n$); cette structure et la multiplication des matrices définissent sur $\mathbf{M}_n(B)$ une structure de A-algèbre associative unifère. La bijection canonique de $\mathbf{M}_n(B)$ sur $\mathrm{End}_B(B^n_d)$ (II, p. 150) est un isomorphisme de A-algèbres.

Lorsque B = A, la A-algèbre $\mathbf{M}_n(A)$ admet une base canonique $(E_{ij})$ formée des unités matricielles (II, p. 142); la table de multiplication correspondante est

$$
E_{ij} E_{hk} = \delta_{jh} E_{ik}.
$$

L’élément unité $I_n$ est égal à $\sum_{i=1}^n E_{ii}$.

### 3. Algèbres quadratiques

Soient $\alpha, \beta$ deux éléments de A, $(e_1, e_2)$ la base canonique du A-module $A^2$. On appelle algèbre quadratique de type $(\alpha, \beta)$ sur A le A-module $A^2$ muni de la structure d’algèbre définie par la table de multiplication (III, p. 10)

$$
e_1^2 = e_1, \quad e_1 e_2 = e_2 e_1 = e_2, \quad e_2^2 = \alpha e_1 + \beta e_2.
$$

Une A-algèbre E isomorphe à une algèbre quadratique est encore dite algèbre quadratique. Il revient au même de dire que E admet une base de deux éléments dont l’un est élément unité.

On peut montrer que toute A-algèbre unifère qui admet une base de deux éléments est une algèbre quadratique (III, p. 178, § 2, exerc. 1).

Si une base $(e_1, e_2)$ d’une A-algèbre a la table de multiplication (2), on dit que c’est une base de type $(\alpha, \beta)$. Par abus de langage, on dit qu’une algèbre quadratique est de type $(\alpha, \beta)$ lorsqu’elle possède une base de type $(\alpha, \beta)$.

#### Proposition 1 {#alg-iii-s2-prop-1 .statement}

*Une algèbre quadratique E est associative et commutative.*

La fait que E soit commutative résulte de l’égalité $e_1 e_2 = e_2 e_1$ dans (2) (III, p. 12); de même, pour vérifier l’associativité, il suffit de voir que $x(yz) = (xy)z$ lorsque $x, y, z$ sont chacun égaux à $e_1$ ou $e_2$. Or, cette relation est évidente si l’un au moins des éléments $x, y, z$ est égal à $e_1$: elle est encore vraie pour $x = y = z = e_2$ puisque E est commutative; d’où la proposition.

Notons $e$ l’élément unité dans une algèbre quadratique E, et soit $(e, i)$ une base de E de type $(\alpha, \beta)$; toute autre base de E contenant $e$ est donc de la forme $(e, j)$ avec $j = \gamma e + \delta i$ (II, p. 98, corollaire). En outre, pour que $(e, j)$ soit une base de E, il faut et il suffit que $\delta$ soit *inversible* dans A; la condition est évidemment suffisante; inversement, si $\bar{i}$ est l’image canonique de $i$ dans $E/Ae$, $\bar{i}$ et $\bar{j} = \delta \bar{i}$ doivent chacun former une base de $E/Ae$, d’où la nécessité de la condition. On a alors

$$
j^2 = (\gamma^2 + \alpha \delta^2)e + (2\gamma \delta + \beta \delta^2)i = (\alpha \delta^2 - \gamma^2 - \beta \gamma \delta)e + (2\gamma + \beta \delta)j;
$$

on voit donc que E est de type

$$(3)$$
$$(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)$$

pour tout $\delta \in A$ inversible et tout $\gamma \in A$. En particulier, si E est de type $(\alpha, 2\beta')$, elle est aussi de type $(\alpha + {\beta'}^2, 0)$ comme on le voit en prenant $\gamma = -\beta'$ et $\delta = 1$.

#### Proposition 2 {#alg-iii-s2-prop-2 .statement}

*Soient E une A-algèbre quadratique, e son élément unité. Pour tout $u \in E$, soit T(u) la trace de l’endomorphisme $m_u : x \mapsto ux$ du A-module libre E (II, p. 78). Alors l’application s définie par $s(u) = T(u).e - u$ est un automorphisme de l’algèbre E, et l’on a $s^2(u) = u$ pour tout $u \in E$.

En effet, soit $(e, i)$ une base de E de type $(\alpha, \beta)$; on a $T(e) = 2$, d’où $s(e) = e$, et $T(i) = \beta$, d’où $s(i) = \beta e - i$. Donc $(e, s(i))$ est une base de E, dont le type est donné par (3) avec $\gamma = \beta$ et $\delta = -1$, ce qui redonne $(\alpha, \beta)$; on en conclut que s est un automorphisme de l’algèbre E. Comme $m_{s(u)} = s m_u s^{-1}$, les endomorphismes $m_u$ et $m_{s(u)}$ du A-module E ont même trace (II, p. 78, prop. 3), d’où

$$
s^2(u) = T(u).e - s(u) = T(u).e - (T(u).e - u) = u
$$

pour tout $u \in E$.

On dit que l’automorphisme s est la conjugaison de la A-algèbre E, et s(u) est appelé le conjugué de u.

Si $u = \xi e + \eta i$, avec $\xi, \eta$ dans A, on a $s(u) = (\xi + \beta \eta)e - \eta i$, d’où
$$
T(u)e = u + s(u) = (2\xi + \beta \eta)e
$$
$$
u.s(u) = (\xi^2 + \beta \xi \eta - \alpha \eta^2)e = N(u)e
$$
où l’on a posé $N(u) = \xi^2 + \beta \xi \eta - \alpha \eta^2$. Les éléments T(u) et N(u) (ou, lorsqu’on identifie canoniquement A et Ae, les éléments T(u)e et N(u)e) s’appellent respectivement la trace et la norme de u.

Lorsque $\beta = 0$, les formules précédentes se simplifient en
$$
s(\xi e + \eta i) = \xi e - \eta i, \quad T(\xi e + \eta i) = 2\xi, \quad N(\xi e + \eta i) = \xi^2 - \alpha \eta^2.
$$
Il est clair que T est une forme linéaire sur E, *et N une forme quadratique sur E (IX, § 3, n° 4)*. Comme E est commutative et associative, il résulte de (5) que l’on a
$$
N(uv) = N(u)N(v).
$$
Pour que u soit inversible dans E, il faut et il suffit que N(u) soit inversible dans A. En effet comme $N(e) = 1$, la nécessité de la condition résulte de (7) où on fait $v = u^{-1}$. Inversement, si N(u) est inversible dans A, il résulte de (5) que u est inversible et que l’on a
$$
u^{-1} = (N(u))^{-1}s(u).
$$
\* On peut prouver que N(u) est le déterminant (III, p. 90) de l’endomorphisme $m_u$ (cf. III, p. 111, Exemple 1).*

La proposition suivante donne la structure des algèbres quadratiques sur un corps commutatif:

#### Proposition 3 {#alg-iii-s2-prop-3 .statement}

Soit E une A-algèbre quadratique de type $(\alpha, \beta)$.

(i) Si A est un corps et s’il ne contient aucun élément $\zeta$ tel que $\zeta^2 = \alpha + \beta \zeta$, E est un corps (commutatif) (cf. V, § 3).

(ii) Si l’anneau A contient un élément $\zeta$ tel que $\zeta^2 = \alpha + \beta \zeta$ et si $\beta - 2\zeta$ est inversible (resp. nul), E est isomorphe à $A \times A$ (resp. est de type $(0, 0)$).

Prouvons (i). Soient $\xi, \eta$ deux éléments de A et $u = \xi e + \eta i$. Si $\eta \neq 0$ et si l’on pose $\theta = -\xi \eta^{-1}$, on a $N(u) = \eta^2(\theta^2 - \beta \theta - \alpha)$ d’après (5), d’où $N(u) \neq 0$ en vertu de l’hypothèse sur A ; si $\eta = 0$, on a $N(u) = \xi^2$. En tous cas, si $u \neq 0$, on a $N(u) \neq 0$, donc N(u) est inversible dans A, et par suite u est inversible dans E.

Prouvons maintenant (ii). La base canonique $(e_1, e_2)$ de l’algèbre $A \times A$ est de type $(0, 1)$. On a vu (III, p. 13, formule (3)) que E est de type
$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$
pour tout $\gamma \in A$ et tout $\delta$ inversible dans A. Si $\beta - 2\zeta$ est inversible, prenons $\delta = (\beta - 2\zeta)^{-1}$ et $\gamma = -\zeta (\beta - 2\zeta)^{-1}$; alors $2\gamma + \beta \delta = 1$, et $\alpha \delta^2 - \gamma^2 - \beta \gamma \delta = \delta^2 (\alpha - \zeta^2 + \beta \zeta) = 0$; ainsi E est de type $(0, 1)$, donc isomorphe à $A \times A$. Si $\beta - 2\zeta = 0$, on a déjà remarqué que $E$ est de type $(\alpha + \zeta^2, 0)$, donc de type $(0, 0)$ puisque $\alpha + \zeta^2 = 2\zeta^2 - \beta\zeta = 0$.

Une $A$-algèbre quadratique de type $(0, 0)$ s’appelle aussi une algèbre de nombres duaux sur $A$.

### 4. Algèbres cayleyennes

#### Définition 1 {#alg-iii-s2-def-1 .statement}

On appelle algèbre cayleyenne sur $A$ un couple $(E, s)$, où $E$ est une algèbre sur $A$ ayant un élément unité $e$, et $s$ est un antiautomorphisme de $E$ tel que l’on ait
$$
u + s(u) \in Ae \quad \text{et} \quad u.s(u) \in Ae
$$
pour tout $u \in E$.

On dit que $s$ est la conjugaison de l’algèbre cayleyenne $(E, s)$ et que $s(u)$ est le conjugué de $u$. La condition $u + s(u) \in Ae$ entraîne que $u$ et $s(u)$ sont permutables. On pose
$$
\text{T}(u) = u + s(u)
$$
$$
\text{N}(u) = u.s(u) = s(u).u
$$
et on dit que ces éléments de la sous-algèbre $Ae$ sont respectivement la trace et la norme cayleyennes de $u$.

Le couple formé d’une algèbre quadratique $E$ et de sa conjugaison $s$ (qui est un antiautomorphisme, puisque $E$ est commutative) (III, p. 13) est une algèbre cayleyenne.

Soit $(E, s)$ une algèbre cayleyenne; comme $s(e) = e$, on a $s(u + s(u)) = u + s(u)$, autrement dit $s(u) + s^2(u) = u + s(u)$, ou encore
$$
s^2(u) = u
$$
de sorte que $s^2$ est l’application identique de $E$. On en déduit
$$
\text{T}(s(u)) = \text{T}(u), \qquad \text{N}(s(u)) = \text{N}(u).
$$
Enfin, la relation $(u - u)(u - s(u)) = 0$ donne
$$
u^2 - \text{T}(u).u + \text{N}(u) = 0
$$
pour tout $u \in E$.

#### Proposition 4 {#alg-iii-s2-prop-4 .statement}

Soient $E$ une $A$-algèbre, $s$ et $s'$ des antiautomorphismes de $E$ tels que $(E, s)$ et $(E, s')$ soient des algèbres cayleyennes. Si $E$ admet une base contenant l’élément unité $e$, on a $s' = s$.
Il est clair que $s'(u) = s(u) = u$ pour tout $u \in Ae$. Si $T, N$ (resp. $T', N'$) sont les fonctions trace et norme pour $(E, s)$ (resp. $(E, s')$), il résulte de (13) que l’on a
$$
(T(u) - T'(u)).u - (N(u) - N'(u)) = 0.
$$
Soient $B$ une base de $E$ contenant $e$, $u$ un élément de $B$ distinct de $e$; on a

T(u) − T'(u) = 0, d’où s(u) = s'(u). Comme s et s' coïncident dans B, ils sont égaux.

Dans ce qui suit, nous poserons $\bar{u} = s(u)$, de sorte que l’on a

$$
\left\{\begin{array}{lll}
u + \bar{u} = T(u), & u\bar{u} = \bar{u}u = N(u), & u = u, \\
u + v = \bar{u} + \bar{v}, & \alpha u = \alpha \bar{u}, & \bar{u}\bar{v} = \bar{v}.\bar{u}
\end{array}\right.
$$

pour $u, v$ dans E, $\alpha \in A$; en outre

$$
T(e) = 2e, \quad N(e) = e.
$$

De la formule $T(uv) = uv + \bar{u}\bar{v} = uv + \bar{v}.\bar{u} = uv + (T(v) - v)(T(u) - u)$, on déduit

$$
uv + vu = T(u)v + T(v)u + (T(uv) - T(u)T(v))
$$

d’où, par échange de $u$ et $v$,

$$
T(vu) = T(uv).
$$

D’autre part, on a $N(u + v) = (u + v)(\bar{u} + \bar{v}) = N(u) + N(v) + T(u\bar{v})$, d’où

$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v).
$$

Or, (16) appliquée en remplaçant $u$ par $\bar{u}$ donne

$$
T(\bar{u}v) = T(u)T(v) + \bar{u}v + v\bar{u} - T(u)v - T(v)\bar{u} = T(u)T(v) - uv - \bar{v}.\bar{u};
$$

d’où

$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v) = T(u)T(v) - T(uv).
$$

Enfin, il est clair que pour tout $\alpha \in A$, on a

$$
N(\alpha u) = \alpha^2 N(u);
$$

en particulier $N(2u) = 4N(u)$, de sorte que la formule (19) donne

$$
(T(u))^2 - T(u^2) = 2N(u).
$$

Il est clair que T est une forme linéaire sur le $(Ae)$-module E. Comme $(u, v) \mapsto T(v\bar{u})$ est une forme bilinéaire sur ce module, \* il résulte de (18) et (20) que N est une forme quadratique (cf. IX, § 3, n° 4).*

### 5. Construction d’algèbres cayleyennes. Quaternions

Soit $(E, s)$ une algèbre cayleyenne sur A, pour laquelle nous utiliserons les notations de III, p. 15, et soit $\gamma \in A$. Soit F l’algèbre sur A dont le module sous-jacent est $E \times E$ et dont la multiplication est définie par

$$
(x, y)(x', y') = (xx' + \gamma \bar{y}'y, y\bar{x}' + y'x);
$$

il est clair que $(e, 0)$ est élément unité de F, et que $E \times \{0\}$ est une sous-algèbre de F isomorphe à E; nous l’identifierons à E dans ce qui suit, de sorte que $x \in E$ est identifié à $(x, 0)$ et en particulier $e$ est identifié à l’élément unité de F.

Soit $t$ la permutation de F définie par
$$
t((x, y)) = (\bar{x}, -y) \quad (x \in E, y \in E).
$$

#### Proposition 5 {#alg-iii-s2-prop-5 .statement}

(i) *Le couple* $(F, t)$ *est une algèbre cayleyenne sur* A.
(ii) *Posons* $j = (0, e)$ *de sorte que* $(x, y) = xe + yj$ *pour* $x \in E, y \in E$. *La trace et la norme cayleyennes* $T_F$ *et* $N_F$ *de* F *sont données par les formules*
$$
T_F(xe + yj) = T(x), \qquad N_F(xe + yj) = N(x) - \gamma N(y).
$$
(iii) *Pour que* F *soit associative, il faut et il suffit que* E *soit associative et commutative.*
Pour $(x, y) \in F$, on a
$$
(x, y) + t((x, y)) = (x + \bar{x}, 0) = T(x)e,
$$
$$
(x, y)t((x, y)) = (x, y)(\bar{x}, -y) = (x\bar{x} - \gamma y\bar{y}, y\bar{x} - yx) = (N(x) - \gamma N(y), 0)
= (N(x) - \gamma N(y))e.
$$

Pour prouver à la fois (i) et (ii), il suffit donc de montrer que $t$ est un antiautomorphisme de F. Il est clair que $t$ est une bijection A-linéaire. D’autre part, on a
$$
t((x, y).(x', y')) = t((xx' + \gamma \bar{y}'y, y\bar{x}' + y'x)) = (\bar{x}'\bar{x} + \gamma \bar{y}\bar{y}', -y\bar{x}' - y'x)
= (\bar{x}', -y')(x, -y) = t((x', y'))t((x, y))
$$
donc $t$ est un antiautomorphisme.

Reste à prouver (iii). Comme E s’identifie à une sous-algèbre de F, on peut supposer E associative. Soient $u = (x, y), u' = (x', y'), u'' = (x'', y'')$ des éléments de F. On a
$$
\begin{cases}
(uu')u'' = ((xx' + \gamma \bar{y}'y)x'' + \gamma \bar{y}''(y\bar{x}' + y'x), (y\bar{x}' + y'x)\bar{x}'' + y''(xx' + \gamma \bar{y}'y)) \\
u(u'u'') = (x(x'x'' + \gamma \bar{y}''y') + \gamma (x''\bar{y}' + \bar{x}'\bar{y}'')y, y(\bar{x}''\bar{x}' + \gamma \bar{y}'y'') + (y'\bar{x}'' + y''x')x)
\end{cases}
$$

L’examen de ces formules montre que la commutativité de E entraîne l’associativité de F. Réciproquement, si F est associative, les formules (27) appliquées avec $y = y' = 0, x'' = 0$ et $y'' = e$ donnent $(0, x'x) = (0, xx')$ c’est-à-dire $x'x = xx'$ quels que soient $x, x'$ dans E; ainsi E est alors commutative.

C. Q. F. D.

Notons encore qu’avec les notations précédentes, on a, pour $x, y$ dans E,
$$
yj = j\bar{y}, \qquad x(yj) = (yx)j, \qquad (xj)y = (x\bar{y})j, \qquad (xj)(yj) = \bar{y}xe
$$
$$
j^2 = e.
$$

L’algèbre cayleyenne $(F, t)$ est appelée l’*extension cayleyenne de* $(E, s)$ *définie par* $\gamma$.
*Exemples.* — 1) Si l’on prend $E = A$ (donc $s = 1_A$), l’algèbre F est une *A-algèbre quadratique*, de base $(e, j)$ avec $j^2 = \gamma e$.

2) Prenons pour E une algèbre quadratique de type $(\alpha, \beta)$, de sorte que le module sous-jacent à E est $\mathbf{A}^2$, avec la table de multiplication (2) (III, p. 12) pour la base canonique. Prenons pour s la conjugaison dans E (III, p. 13, prop. 2). Alors, pour tout $\gamma \in \mathbf{A}$, l’extension cayleyenne F de $(E, s)$ définie par $\gamma$ est appelée l’algèbre de quaternions de type $(\alpha, \beta, \gamma)$, qui est associative en vertu de III, p. 13, prop. 1 et III, p. 17, prop. 5; son module sous-jacent est $\mathbf{A}^4$, et si l’on note $(e, i, j, k)$ la base canonique de $\mathbf{A}^4$, la table de multiplication correspondante est donnée par

$$
\left\{\begin{array}{lll}
i^2 = \alpha e + \beta i, & ij = k, & ik = \alpha j + \beta k \\
ji = \beta j - k, & j^2 = \gamma e, & jk = \beta \gamma e - \gamma i \\
ki = -\alpha j, & kj = \gamma i, & k^2 = -\alpha \gamma e
\end{array}\right.
$$

De plus, pour $u = \rho e + \xi i + \eta j + \zeta k$ (avec $\rho, \xi, \eta, \zeta$ dans $\mathbf{A}$), on a (en écrivant $\bar{u}$ au lieu de $t(u)$ et identifiant $\mathbf{A}$ à $Ae$):

$$
\begin{cases}
\bar{u} = (\rho + \beta \xi)e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho + \beta \xi \\
N_F(u) = \rho^2 + \beta \rho \xi - \alpha \xi^2 - \gamma (\eta^2 + \beta \eta \zeta - \alpha \zeta^2)
\end{cases}
$$

Les formules (30) résultent en effet de (28) et (29) (III, p. 17), et les formules (31) de (23) et (24) (III, p. 17), compte tenu des formules relatives à l’algèbre quadratique E.

On a, pour $u, v$ dans F

$$
N_F(uv) = N_F(u)N_F(v)
$$

car $N_F(uv) = uv.\overline{uv} = uv(\overline{v}.\overline{u}) = u(v\overline{v})\overline{u} = (u\overline{u})(v\overline{v})$ en vertu de l’associativité et du fait que $N_F(u)$ appartient au centre de F.

Une A-algèbre isomorphe à une algèbre de quaternions est encore dite algèbre de quaternions; si une base d’une telle algèbre a la table de multiplication (30), on dit que c’est une base de type $(\alpha, \beta, \gamma)$. Par abus de langage, on dit qu’une algèbre de quaternions est de type $(\alpha, \beta, \gamma)$ lorsqu’elle possède une base de type $(\alpha, \beta, \gamma)$.

Lorsque $\beta = 0$, les formules (30) et (31) se simplifient en

$$
\left\{\begin{array}{lll}
i^2 = \alpha e, & ij = k, & ik = \alpha j \\
ji = -k, & j^2 = \gamma e, & jk = -\gamma i \\
ki = -\alpha j; & kj = \gamma i; & k^2 = -\alpha \gamma e
\end{array}\right.
$$

et

$$
\begin{cases}
\bar{u} = \rho e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho \\
N_F(u) = \rho^2 - \alpha \xi^2 - \gamma \eta^2 + \alpha \gamma \zeta^2
\end{cases}
$$

On remplace alors partout $(\alpha, \beta, \gamma)$ par $(\alpha, \gamma)$ dans les locutions précédentes. Il est immédiat que les algèbres de quaternions de types $(\alpha, \gamma)$ et $(\gamma, \alpha)$ sont isomorphes.

On notera que les formules (32) montrent que F n’est pas commutative lorsque $-1 \neq 1$ dans A.

\* Si l’on prend pour A le corps $\mathbf{R}$ des nombres réels, et $\alpha = \gamma = -1, \beta = 0$, l’algèbre F correspondante s’appelle l’algèbre des quaternions de Hamilton, et est notée $\mathbf{H}$. Si $u = \rho e + \xi i + \eta j + \zeta k$ ($\rho, \xi, \eta, \zeta$ dans $\mathbf{R}$) est un élément $\neq 0$ de $\mathbf{H}$, la formule $u \bar{u} = \bar{u} u = \rho^2 + \xi^2 + \eta^2 + \zeta^2$ (III, p. 18, formule (34)) montre que $N(u) \neq 0$ dans $\mathbf{R}$, de sorte que $u$ admet un inverse $u^{-1} = N(u)^{-1} \bar{u}$ dans $\mathbf{H}$, et que $\mathbf{H}$ est donc un corps non commutatif.*

3) Si on prend pour E une algèbre de quaternions (cf. III, p. 18, Exemple 2), l’extension cayleyenne de E définie par un élément $\delta \in A$ est en général non associative (III, p. 17, prop. 5); on l’appelle algèbre d’octonions sur A (cf. III, p. 176).

### 6. Algèbre d’un magma, d’un monoïde, d’un groupe

Rappelons qu’un magma est un ensemble muni d’une loi de composition (I, p. 1). Soit S un magma, noté multiplicativement, et soit $E = A^{(S)}$ le A-module des combinaisons linéaires formelles des éléments de S (II, p. 25); on sait qu’on définit une application canonique $s \mapsto e_s$ de S dans $A^{(S)}$ telle que la famille $(e_s)_{s \in S}$ soit une base (dite canonique) de $A^{(S)}$, tout élément de $A^{(S)}$ s’écrivant donc d’une seule manière sous la forme $\sum_{s \in S} \alpha_s e_s$, où $(\alpha_s)$ est une famille d’éléments de A à support fini. Cela étant, on définit sur E une structure de A-algèbre en prenant comme table de multiplication de la base canonique

$$
e_s e_t = e_{st}.
$$

L’algèbre E ainsi définie s’appelle l’algèbre du magma S sur A. Si $x = \sum_{s \in S} \xi_s e_s$ et $y = \sum_{s \in S} \eta_s e_s$ sont deux éléments de E, on a

$$
xy = \sum_{s \in S} \left( \sum_{t u = s} \xi_t \eta_u \right) e_s.
$$

Lorsque S est un monoïde (resp. un groupe), on dit que E est l’algèbre du monoïde (resp. du groupe) S sur A; c’est alors une algèbre associative (III, p. 11); de même, lorsque S est un monoïde commutatif, son algèbre est associative et commutative. Enfin, si le magma S admet un élément neutre $u$, $e_u$ est élément unité de l’algèbre E; comme l’élément $e_u$ est libre, A s’identifie alors à la sous-algèbre $Ae_u$ de E.

Lorsque $A \neq \{0\}$, on identifie parfois S à son image par l’injection $s \mapsto e_s$, de sorte qu’on écrit $\sum_{s \in S} \alpha_s s$ un élément de E; mais cette identification n’est pas possible (sous peine de confusion) lorsque S est noté additivement. On écrit alors souvent aussi $e^s$ au lieu de $e_s$.

Soient B un second anneau commutatif, et $\rho : A \to B$ un homomorphisme d’anneaux; considérons les algèbres $E = A^{(S)}$ et $E' = B^{(S)}$ d’un même magma S sur A et sur B, et soient $(e_s)_{s \in S}$ et $(e'_s)_{s \in S}$ leurs bases canoniques respectives. L’algèbre $B^{(S)}$ s’identifie canoniquement, par l’application A-linéaire j telle que $j(e_s \otimes 1) = e'_s$ pour tout $s \in S$, à l’algèbre $A^{(S)} \otimes_A B$ obtenue à partir de $A^{(S)}$ par extension à B de l’anneau des scalaires (II, p. 25, cor. 3).

#### Proposition 6 {#alg-iii-s2-prop-6 .statement}

*Soient S un magma, F une A-algèbre et f un homomorphisme de S dans F munie de sa seule structure multiplicative. Alors il existe un homomorphisme de A-algèbres $\bar{f} : A^{(S)} \to F$ et un seul rendant commutatif le diagramme*

$$
\begin{array}{ccc}
S & \xrightarrow{f} & F \\
\downarrow & & \downarrow 1_F \\
A^{(S)} & \xrightarrow{\bar{f}} & F
\end{array}
$$

(où la flèche verticale de gauche est l’application canonique $s \mapsto e_s$).

En effet, soit $\bar{f} : A^{(S)} \to F$ l’unique homomorphisme de A-modules tel que $\bar{f}(e_s) = f(s)$ (II, p. 25, cor. 3); il suffit de vérifier que $\bar{f}$ est un homomorphisme d’algèbres, et pour cela il suffit de prouver que $\bar{f}(e_s e_t) = \bar{f}(e_s) \bar{f}(e_t)$, ce qui résulte aussitôt de la définition et de l’hypothèse $f(st) = f(s)f(t)$.

La prop. 6 exprime que le couple formé de $A^{(S)}$ et de l’application canonique $s \mapsto e_s$ est solution du problème d’application universelle (E, IV, p. 23), où $\Sigma$ est l’espèce de structure de A-algèbre et les $\alpha$-applications les homomorphismes de S dans une A-algèbre munie de sa seule loi multiplicative.

#### Corollaire {#alg-iii-s2-n6-cor-1 .statement}

*Soient S, S’ deux magmas, g : S $\to$ S’ un homomorphisme. Il existe alors un homomorphisme de A-algèbres u : $A^{(S)} \to A^{(S')}$ et un seul rendant commutatif le diagramme*

$$
\begin{array}{ccc}
S & \xrightarrow{g} & S' \\
\downarrow & & \downarrow \\
A^{(S)} & \xrightarrow{u} & A^{(S')}
\end{array}
$$

(où les flèches verticales sont les applications canoniques).

Il suffit d’appliquer la prop. 6 en prenant pour f l’application composée $S \xrightarrow{g} S' \longrightarrow A^{(S')}$.

En particulier, si T est une *partie stable* du magma S (I, p. 6), l’ensemble des éléments $\sum_{s \in T} \alpha_s e_s$ de $A^{(S)}$ est une *sous-algèbre* de $A^{(S)}$ canoniquement isomorphe à l’algèbre $A^{(T)}$, et qu’on identifie parfois à cette dernière.

#### Exemple {#alg-iii-s2-n6-exa-1 .statement}

Soient V un A-module, S un monoïde qui *opère à gauche* dans V; cela signifie (I, p. 49) qu’on se donne une application $(s, x) \mapsto s.x$ de S dans V telle que $s.(x + y) = s.x + s.y,\ s.(\alpha x) = \alpha(s.x)$ et $s.(t.x) = (st).x$ pour $s, t$ dans S, $x, y$ dans V et $\alpha \in A$ et que si e désigne l’élément neutre de S, $e.x = x$ pour $x \in V$.

Si l’on pose $f(s)(x) = s.x$, $f$ est un *homomorphisme* de $S$ dans l’algèbre $\mathrm{End}_A(V)$ (munie de sa seule loi multiplicative), transformant l’élément neutre $e$ en l’élément unité $1_V$. Appliquant la prop. 6 de III, p. 20, on en déduit un homomorphisme de A-algèbres $\tilde{f} : A^{(S)} \to \mathrm{End}_A(V)$, qui munit le groupe additif sous-jacent à $V$ d’une structure de *module à gauche* sur $A^{(S)}$.

Ceci permet de ramener l’étude des groupes commutatifs à opérateurs à celle des modules. Soit en effet $M$ un groupe commutatif à opérateurs, noté additivement, et dont toutes les lois d’action sont notées multiplicativement. Soit $\Omega$ l’ensemble somme (E, II, p. 30) des domaines d’opérateurs des diverses lois d’action de $M$, chacun de ces domaines étant identifié canoniquement à une partie de $\Omega$. Soit $\mathrm{Mo}(\Omega)$ le *monoïde libre* (I, p. 79) construit sur $\Omega$; on définit une loi d’action $(s, x) \mapsto s.x$ sur $M$, ayant $\mathrm{Mo}(\Omega)$ comme domaine d’opérateurs, par récurrence sur la longueur du *mot* $s$ dans $\mathrm{Mo}(\Omega)$; si $s$ est de longueur 0, c’est le mot vide $e$, et nous posons $e.x = x$ pour tout $x \in M$. Si $s$ est de longueur $n \geqslant 1$, on peut l’écrire d’une seule manière $s = tu$, où $u$ est de longueur $n - 1$ et $t$ de longueur 1, de sorte que $t \in \Omega$; on pose alors $s.x = t.(u.x)$. Pour deux mots quelconques $s, s'$ dans $\mathrm{Mo}(\Omega)$, on vérifie la relation $s.(s'.x) = (ss').x$ par récurrence sur la longueur de $s$.

Appliquant alors la méthode décrite ci-dessus, on obtient finalement sur $M$ une structure de $\mathbf{Z}^{(\mathrm{Mo}(\Omega))}$-module à gauche, et on vérifie sans peine que les notions usuelles de la théorie des groupes à opérateurs (sous-groupes stables, homomorphismes) sont les mêmes pour les groupes commutatifs à opérateurs et les modules qui leur sont ainsi associés.

### 7. Algèbres libres

#### Définition 2 {#alg-iii-s2-def-2 .statement}

*Soit I un ensemble ; désignons par* $M(I)$ (resp. $\mathrm{Mo}(I)$, resp. $\mathbf{N}^{(I)}$) *le magma libre* (I, p. 77) (resp. *le monoïde libre* (I, p. 79), resp. *le monoïde commutatif libre* (I, p. 88)) *construit sur I*. *L’algèbre de* $M(I)$ (resp. $\mathrm{Mo}(I)$, resp. $\mathbf{N}^{(I)}$) *sur* $A$ *s’appelle l’algèbre libre* (resp. *l’algèbre associative libre*, resp. *l’algèbre associative et commutative libre* (ou, par abus de langage, *l’algèbre commutative libre*)) *de l’ensemble* $I$ *sur l’anneau* $A$.

Nous noterons $\mathrm{Lib}_A(I)$ (resp. $\mathrm{Libas}_A(I)$, resp. $\mathrm{Libasc}_A(I)$) l’algèbre libre (resp. l’algèbre associative libre, resp. l’algèbre commutative libre) de $I$ sur $A$. Par composition de l’injection canonique de $I$ dans $M(I)$ (resp. $\mathrm{Mo}(I)$, resp. $\mathbf{N}^{(I)}$) et de l’application canonique de $M(I)$ (resp. $\mathrm{Mo}(I)$, resp. $\mathbf{N}^{(I)}$) dans $\mathrm{Lib}_A(I)$ (resp. $\mathrm{Libas}_A(I)$, resp. $\mathrm{Libasc}_A(I)$) on obtient une application canonique de $I$ dans $\mathrm{Lib}_A(I)$ (resp. $\mathrm{Libas}_A(I)$, resp. $\mathrm{Libasc}_A(I)$), qui est injective si $A \neq \{0\}$. Nous désignerons par $X_i$ l’image d’un élément $i \in I$ par cette application canonique, et nous dirons que $X_i$ est l’*indéterminée d’indice* $i$ de $\mathrm{Lib}_A(I)$ (resp. $\mathrm{Libas}_A(I)$, resp. $\mathrm{Libasc}_A(I)$).

Comme $\mathrm{Mo}(I)$ et $\mathbf{N}^{(I)}$ ont chacun un élément neutre, $\mathrm{Libas}_A(I)$ et $\mathrm{Libasc}_A(I)$ sont des algèbres associatives unifères, et en outre $\mathrm{Libasc}_A(I)$ est commutative. Si $e$ est l’élément unité de $\mathrm{Libas}_A(I)$ (resp. $\mathrm{Libasc}_A(I)$), l’application $\alpha \mapsto \alpha e$ est un isomorphisme de $A$ sur un sous-anneau du centre de $\mathrm{Libas}_A(I)$ (resp. $\mathrm{Libasc}_A(I)$), qu’on identifie à $A$ (III, p. 19).

#### Proposition 7 {#alg-iii-s2-prop-7 .statement}

*Soient I un ensemble, F une algèbre (resp. une algèbre associative unifère, resp. une algèbre associative et commutative unifère) sur A. Pour toute application f : I → F, il existe un homomorphisme (resp. un homomorphisme unifère) et un seul $\bar{f}$ de Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) dans F tel que $\bar{f}(X_i) = f(i)$ pour tout $i \in I$.

Soit $F_m$ le magma (resp. le monoïde) obtenu en munissant l’ensemble F de sa loi de composition multiplicative. Il y a un homomorphisme (resp. un homomorphisme unifère) et un seul g de M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) dans $F_m$ tel que $g(i) = f(i)$ pour tout $i \in I$ (I, p. 78, p. 79 et p. 88); la prop. 7 résulte donc de III, p. 20, prop. 6.

#### Remarque 1 {#alg-iii-s2-n7-rem-1 .statement}

Nous définirons plus loin un isomorphisme de Libas_A(I) sur l’algèbre tensorielle du module libre $A^{(I)}$ (III, p. 62) ainsi qu’un isomorphisme de Libasc_A(I) sur l’algèbre symétrique de $A^{(I)}$ (III, p. 75).

#### Remarque 2 {#alg-iii-s2-n7-rem-2 .statement}

Soit $\rho$ un homomorphisme unifère de A dans un anneau commutatif B. Comme on l’a vu dans III, p. 20, on déduit de $\rho$ un isomorphisme $\sigma$ de Lib_B(I) (resp. Libas_B(I), resp. Libasc_B(I)) sur l’algèbre $(\mathrm{Lib}_A(I))_{(B)}$ (resp. $(\mathrm{Libas}_A(I))_{(B)}$, resp. $(\mathrm{Libasc}_A(I))_{(B)}$) obtenue par extension des scalaires à B au moyen de $\rho$; si $X_i^A, X_i^B$ sont les indéterminées d’indice i correspondant respectivement à A et à B, on a $\sigma(X_i^B) = X_i^A \otimes 1$.

#### Remarque 3 {#alg-iii-s2-n7-rem-3 .statement}

Soit J une partie de I; on sait que M(J) s’identifie à une partie stable du magma $M(I)$, donc (III, p. 20) $\mathrm{Lib}_A(J)$ s’identifie canoniquement à une sous-algèbre de $\mathrm{Lib}_A(I)$, engendrée par les $X_i$ tels que $i \in J$; on dit qu’un élément de $\mathrm{Lib}_A(J)$ ne fait intervenir que les indéterminées d’indices appartenant à J. La définition donnée dans III, p. 19 de l’algèbre d’un magma montre que $\mathrm{Lib}_A(I)$ est la réunion de la famille filtrante des sous-algèbres $\mathrm{Lib}_A(J)$ lorsque J parcourt l’ensemble des parties *finies* de I. On a des résultats analogues pour Libas_A(I) et Libasc_A(I).

#### Remarque 4 {#alg-iii-s2-n7-rem-4 .statement}

À tout élément s de M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) est associé sa *longueur* $l(s)$, qui est un entier $\geqslant 1$ (resp. $\geqslant 0$) tel que $l(ss') = l(s) + l(s')$ (I, p. 77, p. 79 et p. 87). Si $e_s$ est l’élément de $\mathrm{Lib}_A(I)$ (resp. Libas_A(I), resp. Libasc_A(I)) correspondant à s, on appelle *degré total* (ou simplement *degré*) d’un élément $x = \sum_s \alpha_s e_s \neq 0$ de $\mathrm{Lib}_A(I)$ (resp. Libas_A(I), resp. Libasc_A(I)) le plus grand des nombres $l(s)$ lorsque s parcourt l’ensemble (non vide par hypothèse) des éléments tels que $\alpha_s \neq 0$. Par exemple, si $i, j, k$ sont trois éléments distincts de I, l’élément $(X_i(X_jX_k))X_i - (X_iX_j)(X_kX_i)$ est un élément $\neq 0$ de degré total 4 dans $\mathrm{Lib}_A(I)$.

### 8. Définition d’une algèbre par générateurs et relations

Soient F une algèbre sur A, $(x_i)_{i \in I}$ une famille d’éléments de F. En vertu de la prop. 7, il existe un unique homomorphisme $f : \mathrm{Lib}_A(I) \to F$ tel que $f(X_i) = x_i$ pour tout $i \in I$. Pour que $f$ soit surjectif, il faut et il suffit que $(x_i)_{i \in I}$ soit un système générateur de $F$.

Si $U \in \mathrm{Lib}_A(I)$, $f(U)$ s’appelle l’élément de $F$ déduit de $U$ par substitution des éléments $x_i$ aux indéterminées $X_i$, ou encore la valeur de $U$ pour les valeurs $x_i$ des indéterminées $X_i$; on le note le plus souvent $U((x_i)_{i \in I})$; on a en particulier $U((X_i)_{i \in I}) = U$. Si $\lambda$ est un homomorphisme de $F$ dans une algèbre $F'$ sur $A$, on a
$$
\lambda(U((x_i)_{i \in I})) = U((\lambda(x_i))_{i \in I}).
$$
Considérons en particulier le cas où $F = \mathrm{Lib}_A(J)$, où $J$ est un second ensemble; pour toute famille $(H_i)_{i \in I}$ d’éléments de $\mathrm{Lib}_A(J)$ et toute famille $(y'_j)_{j \in J}$ d’élément d’une $A$-algèbre $F'$, on a
$$
(\mathrm{U}((H_i)_{i \in I}))((y'_j)_{j \in J}) = \mathrm{U}((H_i((y'_j)_{j \in J}))_{i \in I}).
$$
Les notations étant comme ci-dessus, on appelle relateur de la famille $(x_i)_{i \in I}$ dans $F$ tout élément $U$ de $\mathrm{Lib}_A(I)$ tel que $U((x_i)_{i \in I}) = 0$, ou encore tel que $f(U) = 0$. L’idéal bilatère $\mathrm{Ker}(f)$ formé par ces éléments est appelé l’idéal des relateurs de $(x_i)$.

Soit $(R_j)_{j \in J}$ une famille d’éléments de $\mathrm{Lib}_A(I)$. On dit que $((x_i)_{i \in I}, (R_j)_{j \in J})$ est une présentation de l’algèbre $F$ si $(x_i)_{i \in I}$ est un système générateur de $F$, et si l’idéal bilatère de $\mathrm{Lib}_A(I)$ engendré par les $R_j$ est égal à l’idéal des relateurs de la famille $(x_i)_{i \in I}$; on dit que les $x_i$ sont les générateurs et les $R_j$ les relateurs de la présentation.

Considérons maintenant un ensemble quelconque $I$, et une famille $(R_j)_{j \in J}$ d’éléments de $\mathrm{Lib}_A(I)$. On appelle algèbre universelle définie par le système générateur $I$ lié par la famille de relateurs $(R_j)_{j \in J}$ l’algèbre $E$ quotient de $\mathrm{Lib}_A(I)$ par l’idéal bilatère engendré par la famille $(R_j)$. Il est clair que si l’on note $\overline{X}_i$ l’image de $X_i$ dans $E$, $((\overline{X}_i)_{i \in I}, (R_j)_{j \in I})$ est une présentation de $E$. En outre, si $(x_i)_{i \in I}$ est une famille d’éléments d’une algèbre $F$ et si l’on a $R_j((x_i)_{i \in I}) = 0$ pour tout $j \in J$, il existe un unique homomorphisme $g : E \to F$ tel que $g(\overline{X}_i) = x_i$ pour tout $i \in I$; pour que $((x_i)_{i \in I}, (R_j)_{j \in J})$ soit une présentation de $F$, il faut et il suffit que $g$ soit bijectif.

Ces remarques justifient les abus de langage suivants: au lieu de dire « $((x_i)_{i \in I}, (R_j)_{j \in J})$ est une présentation de $F$ », on dit aussi « $F$ est l’algèbre engendrée par les générateurs $x_i$ soumis aux relations $R_j((x_i)_{i \in I}) = 0$ ». Lorsque les $R_j$ sont de la forme $P_j - Q_j$, on dit aussi que « $F$ est l’algèbre engendrée par les $x_i$ soumis aux relations $P_j((x_i)) = Q_j((x_i))$ ».

Soit $H$ un ensemble; nous dirons qu’un élément $S$ de $\mathrm{Lib}_A(H)$ est un relateur universel pour une $A$-algèbre $F$ si l’on a $S((x_h)_{h \in H}) = 0$ pour toute famille $(x_h)_{h \in H}$ d’éléments de $F$ ayant $H$ pour ensemble d’indices.

#### Exemple 1 {#alg-iii-s2-n8-exa-1 .statement}

Prenons $H = \{1, 2, 3\}$; les algèbres qui admettent
$$
(X_1 X_2) X_3 - X_1 (X_2 X_3)
$$
comme relateur universel sont les algèbres associatives. Les algèbres qui admettent

X_1 X_2 - X_2 X_1 comme relateur universel sont les algèbres commutatives. \* Les algèbres qui admettent les relateurs universels X_1 X_1 et

$$(X_1 X_2) X_3 + (X_2 X_3) X_1 + (X_3 X_1) X_2$$

sont les algèbres de Lie.*

Soit I un ensemble; donnons-nous une famille $(S_k)_{k \in K}$ d’éléments de Lib_A(H), et considérons l’ensemble T des éléments de Lib_A(I) de la forme $S_k((U_h)_{h \in H})$, où $k$ parcourt K, et pour chaque $k$, $(U_h)_{h \in H}$ parcourt l’ensemble des familles d’éléments de Lib_A(I) ayant H pour ensemble d’indices; considérons une famille $(R_j)_{j \in J}$ ayant T pour ensemble d’éléments. Cela étant, soit F l’algèbre universelle définie par le système générateur I lié par la famille $(R_j)_{j \in J}$, et soit $u : \mathrm{Lib}_A(I) \to F$ l’homomorphisme canonique, de sorte que Ker(u) est engendré par les éléments $S_k((U_h)_{h \in H})$ pour tous les $k \in K$ et toutes les familles $(U_h)_{h \in H}$ d’éléments de Lib_A(I); il est clair que chacun des $S_k$ ($k \in K$) est un relateur universel pour F. Soit maintenant F’ une algèbre admettant un système générateur $(x_i)_{i \in I}$, pour laquelle chacun des $S_k$ soit un relateur universel, et soit $u' : \mathrm{Lib}_A(I) \to F'$ l’homomorphisme tel que $u'(X_i) = x_i$ pour tout $i \in I$; il est clair que Ker(u) $\subset$ Ker(u’), donc u’ s’écrit d’une seule manière sous la forme $u' = h \circ u$, où $h : F \to F'$ est un homomorphisme, tel que $h(\overline{X}_i) = x_i$ pour tout $i \in I$. On dit pour cette raison que F est l’algèbre universelle définie par le système générateur I, correspondant à la famille de relateurs universels $(S_k)_{k \in K}$. Par abus de langage, on dit parfois que F est l’algèbre universelle engendrée par I et soumise aux identités $S_k((u_h)) = 0$ pour toute famille $(u_h)_{h \in H}$ d’éléments de F.

#### Exemple 2 {#alg-iii-s2-n8-exa-2 .statement}

Soit L’ l’algèbre universelle engendrée par I et soumise aux identités $(uv)w - u(vw) = 0$ pour toute famille de trois éléments de L’, et soit L” l’algèbre obtenue par adjonction à L’ d’un élément unité; il existe alors un isomorphisme unifère unique g de L” sur Libas_A(I) tel que $g(\overline{X}_i) = X_i$ pour tout $i \in I$. En effet, il est clair que L” est associative et l’existence de l’homomorphisme g résulte de la définition de L’ et des remarques qui la précèdent; mais alors il est clair que L” vérifie la propriété universelle (III, p. 22, prop. 7) qui caractérise Libas_A(I), d’où la conclusion.

Des considérations analogues aux précédentes s’appliquent aux algèbres associatives (resp. associatives et commutatives), en tenant compte des remarques qui suivent. Quand le contexte indique suffisamment que les algèbres que l’on considère sont des algèbres unifères, on fait souvent l’abus de langage qui consiste à appeler système générateur d’une algèbre F une famille d’éléments $(x_i)_{i \in I}$ de F telle que la sous-algèbre engendrée par les $x_i$ ($i \in I$) et par l’élément unité soit égale à F. Cela étant, soient F une algèbre associative unifère sur A, et soit $(x_i)_{i \in I}$ une famille d’éléments de F; en vertu de III, p. 22, prop. 7, il existe un unique homomorphisme unifère $f : \mathrm{Libas}_A(I) \to F$ tel que $f(X_i) = x_i$ pour tout $i \in I$; si U $\in \mathrm{Libas}_A(I)$, on appelle encore $f(U)$ l’élément de F déduit de U par substitution des éléments $x_i$ aux indéterminées $X_i$, et on le note encore $U((x_i)_{i \in I})$. On transporte alors aussitôt aux algèbres associatives les notions de relateur, de présentation, et de relateur universel ; il suffit simplement de remplacer partout $\mathrm{Lib}_A(I)$ par $\mathrm{Libas}_A(I)$.

L’algèbre associative unifère universelle, définie par le système générateur $I$ lié par la famille de relateurs $(R_j)_{j \in J}$ est l’algèbre quotient de $\mathrm{Libas}_A(I)$ par l’idéal bilatère engendré par la famille $(R_j)$. On définit de même l’algèbre associative unifère universelle définie par le système générateur $I$, et correspondant à une famille de relateurs universels. Nous laissons au lecteur le soin d’énoncer les définitions analogues relatives aux algèbres associatives et commutatives, $\mathrm{Libasc}_A(I)$ se substituant à $\mathrm{Libas}_A(I)$.

#### Exemple 3 {#alg-iii-s2-n8-exa-3 .statement}

Soit $L'$ l’algèbre associative unifère universelle engendrée par $I$ et soumise aux identités $uv - vu = 0$ pour toute famille de deux éléments de $L'$. On voit comme dans III, p. 24, Exemple 2 que $L'$ est canoniquement isomorphe à $\mathrm{Libasc}_A(I)$.

### 9. Algèbres de polynômes

Soit $B$ une $A$-algèbre associative, commutative et unifère et soit $(x_i)_{i \in I}$ une famille d’éléments de $B$; on désigne par $A[(x_i)_{i \in I}]_B$, ou simplement $A[(x_i)_{i \in I}]$, la sous-algèbre de $B$ engendrée par les $x_i$ ($i \in I$) et par l’élément unité, lorsqu’aucune confusion n’en résulte. Pour tout ensemble $I$, l’algèbre $\mathrm{Libasc}_A(I)$ est donc égale à $A[(X_i)_{i \in I}]$ (qu’on note aussi $A[X_i]_{i \in I}$); cette dernière notation, qui a l’avantage d’indiquer la notation choisie pour noter les indéterminées, est celle que nous emploierons en général dans la suite de ce Traité. Les éléments de $A[(X_i)_{i \in I}]$ sont appelés polynômes par rapport aux indéterminées $X_i$ ($i \in I$) à coefficients dans $A$; il convient de noter que lorsqu’on dit « soit $A[(X_i)_{i \in I}]$ une algèbre de polynômes », on sous-entend toujours que les $X_i$ sont les indéterminées. Pour toute partie $J$ de $I$, l’usage de la notation précédente revient à identifier $\mathrm{Libasc}_A(J)$ à la sous-algèbre de $\mathrm{Libasc}_A(I)$ engendrée par les $X_i$ d’indice $i \in J$ et l’élément unité (cf. III, p. 22, Remarque 3). Pour $I = \{1, 2, \ldots, n\}$ on écrit $A[X_1, X_2, \ldots, X_n]$ au lieu de $A[(X_i)_{i \in I}]$.

Si $I$ et $I'$ sont deux ensembles équipotents, les algèbres $\mathrm{Libasc}_A(I)$ et $\mathrm{Libasc}_A(I')$ sont isomorphes. On note souvent $A[X]$ l’algèbre des polynômes correspondant à un ensemble d’indices $I$ non spécifié à un seul élément, $X$ étant l’unique indéterminée; de même, on notera $A[X, Y]$, $A[X, Y, Z]$, … les algèbres de polynômes correspondant à des ensembles d’indices non spécifiés à 2, 3, … éléments. On notera qu’en vertu des conventions faites plus haut, $A[X]$ et $A[Y]$ sont par exemple des sous-algèbres (distinctes) de $A[X, Y, Z]$ si $A \neq \{0\}$.

Les éléments

$$
X^\nu = \prod_{i \in I} X_i^{\nu(i)}
$$

où $\nu$ parcourt $\mathbf{N}^{(I)}$, forment une base de l’algèbre de polynômes $A[(X_i)_{i \in I}]$. Ces éléments s’appellent les monômes en les indéterminées $X_i$, et le nombre $|\nu| = \sum_{i \in I} \nu(i)$ est appelé le degré (ou degré total) du monôme $X^\nu$. L’unique monôme de degré 0 est l’élément unité de $A[(X_i)_{i \in I}]$; on l’identifie souvent à l’élément unité 1 de A. Tout polynôme $u$ de $A[(X_i)_{i \in I}]$ s’écrit d’une façon et d’une seule

$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$

avec $\alpha_\nu \in A$; les éléments $\alpha_\nu$, nuls sauf pour un nombre fini d’indices $\nu \in \mathbf{N}^{(I)}$, s’appellent les coefficients de $u$; les éléments $\alpha_\nu X^\nu$ s’appellent les termes de $u$ (l’élément $\alpha_\nu X^\nu$ étant souvent appelé « le terme en $X^\nu$ »); en particulier le terme $\alpha_0 X^0$ (identifié à $\alpha_0 \in A$) s’appelle le terme constant de $u$. Si $J$ est une partie de $I$, $u$ appartient à $A[(X_i)_{i \in J}]$ si et seulement si $\alpha_\nu = 0$ lorsque $\nu \notin \mathbf{N}^{(J)}$. Il en résulte que $A[(X_i)_{i \in I}]$ est la réunion des sous-algèbres $A[(X_i)_{i \in J}]$, où $J$ parcourt l’ensemble des parties finies de $I$. Si $\alpha_\nu = 0$ pour $|\nu| > n$, on dit que $u$ est un polynôme de degré $\leq n$. Lorsque $\alpha_\nu = 0$, on dit (par abus de langage) que $u$ ne contient pas de terme en $X^\nu$; en particulier, quand $\alpha_0 = 0$, on dit que $u$ est un polynôme sans terme constant.

Pour tout polynôme non nul $u = \sum \alpha_\nu X^\nu$, on appelle degré (ou degré total) de $u$ le plus grand des entiers $|\nu|$ pour les multiindices $\nu$ tels que $\alpha_\nu \neq 0$.

Soit F une A-algèbre associative unifère, et soit $(x_i)_{i \in I}$ une famille d’éléments de F, deux à deux permutables. La sous-algèbre F’ de F engendrée par les $x_i$ et l’élément unité est commutative (III, p. 111), ce qui permet de définir la substitution des $x_i$ aux $X_i$ dans un polynôme $u \in A[(X_i)_{i \in I}]$ (bien que F ne soit pas nécessairement commutative): $u((x_i)_{i \in I})$ est un élément de F’, donc de F, et $h: u \mapsto u((x_i)_{i \in I})$ est un homomorphisme de $A[(X_i)_{i \in I}]$ dans F. Les éléments du noyau de $h$ sont les relateurs de la famille $(x_i)$ dans $A[(X_i)_{i \in I}]$, qu’on appelle aussi relateurs polynomiaux (à coefficients dans A) entre les $x_i$. L’image de l’homomorphisme $h$ est la sous-algèbre F’, qu’on désigne encore par $A[(x_i)_{i \in I}]$ (même quand F n’est pas commutative); si $a$ est l’idéal des relateurs polynomiaux entre les $x_i$, on a une suite exacte de A-modules

$$
0 \longrightarrow a \longrightarrow A[(X_i)_{i \in I}] \xrightarrow{h} A[(x_i)_{i \in I}] \longrightarrow 0.
$$

#### Proposition 8 {#alg-iii-s2-prop-8 .statement}

*Soient $A[(X_i)_{i \in I}]$ une algèbre de polynômes, $J$ une partie de $I$, K le complémentaire de $J$ dans $I$. Si on pose $A' = A[(X_j)_{j \in J}]$ et si on note $X'_k$ ($k \in K$) les indéterminées dans l’algèbre de polynômes Libasc$_A'$(K) = $A'[(X'_k)_{k \in K}]$, il existe un isomorphisme unique d’anneaux de $A'[(X'_k)_{k \in K}]$ sur $A[(X_i)_{i \in I}]$ qui coïncide avec l’identité dans $A'$ et transforme $X'_k$ en $X_k$ pour tout $k \in K$.*

En effet, il est clair que $A[(X_i)_{i \in I}]$ est une $A'$-algèbre engendrée par les $X_k$ pour $k \in K$. D’autre part, comme un relateur polynomial entre les $X_k$ ($k \in K$) à coefficients dans $A'$ s’écrit d’une seule manière $\sum h_\nu((X_j)_{j \in J}) {X'}^\nu$ où $\nu$ parcourt une partie finie de $\mathbf{N}^{(\mathbf{K})}$ et où les $h_v$ sont des éléments de $A[(X_j)_{j \in J}]$, les $h_v$ doivent être des relateurs polynomiaux entre les $X_j$ à coefficients dans $A$, donc sont tous nuls, ce qui prouve la proposition.

On utilise souvent l’isomorphisme décrit dans la prop. 8 pour identifier les éléments de $A[(X_i)_{i \in I}]$ à des polynômes à coefficients dans $A' = A[(X_j)_{j \in J}]$. Si $u$ est un élément $\neq 0$ de $A[(X_i)_{i \in I}]$, son degré total quand on le considère comme élément de $A'[(X_k)_{k \in K}]$ est encore appelé son *degré par rapport aux* $X_i$ *d’indice* $i \in K$.

#### Remarque {#alg-iii-s2-n9-rem-1 .statement}

Soient $I$ et $J$ deux ensembles, $(P_j)_{j \in J}$ une famille d’éléments de $\mathbf{Z}[(X_i)_{i \in I}]$; si $Q$ est un élément de $\mathbf{Z}[(Y_j)_{j \in J}]$ tel que $Q((P_j)_{j \in J}) = 0$, alors, pour toute famille $(b_i)_{i \in I}$ d’éléments deux à deux permutables d’un anneau $B$, on a $Q((P_j((b_i)_{i \in I}))_{j \in J}) = 0$. On appelle parfois *identités polynomiales* les relations vraies de la forme $Q((P_j)_{j \in J}) = 0$. Par exemple

$$
(X_1 + X_2)^2 - X_1^2 - X_2^2 - 2X_1X_2 = 0
$$
avec
$$
Q = Y_1^2 - Y_2, \quad P_1 = X_1 + X_2, \quad P_2 = X_1^2 + X_2^2 + 2X_1X_2
$$
$$
X_1^n - X_2^n - (X_1 - X_2)(X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}) = 0
$$
avec
$$
Q = Y_1 - Y_2Y_3, \quad P_1 = X_1^n - X_2^n, \quad P_2 = X_1 - X_2,
$$
$$
P_3 = X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}
$$
sont des identités polynomiales.

### 10. Algèbre large d’un monoïde

L’algèbre d’un monoïde $S$ sur $A$ est (en tant que $A$-module) le sous-module du produit $A^S$ formé des familles $(\alpha_s)_{s \in S}$ de support fini; la multiplication dans cette algèbre est définie par les relations $(\alpha_s)(\beta_s) = (\gamma_s)$, où, pour tout $s \in S$,
$$
\gamma_s = \sum_{tu = s} \alpha_t \beta_u
$$
(cf. III, p. 19, formule (35)). La somme du second membre de (38) a un sens parce que $(\alpha_s)$ et $(\beta_s)$ sont des familles de supports finis, et qu’il en est donc de même de la famille double $(\alpha_t \beta_u)_{(t, u) \in S \times S}$. Mais le second membre de (38) a encore un sens pour des éléments *quelconques* $(\alpha_s), (\beta_s)$ de $A^S$ lorsque le monoïde $S$ vérifie la condition suivante:

(D) *Pour tout* $s \in S$, *il n’existe qu’un nombre fini de couples* $(t, u)$ *dans* $S \times S$ *tels que* $tu = s$.

Supposons donc que $S$ vérifie la condition (D); sur le $A$-module produit $A^S$, on peut alors définir une loi de multiplication par la formule (38). Il est immédiat que la multiplication ainsi définie sur $A^S$ est $A$-bilinéaire; en outre, elle est *associative*, car on a, pour $\alpha, \beta, \gamma$ dans $A^S$,
$$
\sum_{uvw = t} \alpha_u \beta_v \gamma_w = \sum_{rw = t} ((\sum_{uv = r} \alpha_u \beta_v) \gamma_w) = \sum_{us = t} (\alpha_u (\sum_{vw = s} \beta_v \gamma_w)).
$$
Cette multiplication et la structure de $A$-module de $A^S$ définissent donc sur

$A^S$ une structure d’algèbre associative unifère sur $A$; nous dirons que l’ensemble $A^S$, muni de cette structure, est l’algèbre large du monoïde $S$ sur $A$.

Il est immédiat que l’algèbre $A^{(S)}$ du monoïde $S$ sur $A$ (dite encore algèbre stricte de $S$ lorsqu’on veut éviter des confusions) est une sous-algèbre de l’algèbre large de $S$ sur $A$ (et est identique à cette dernière lorsque $S$ est fini). Par abus de langage, on note encore tout élément $(\xi_s)_{s \in S}$ de l’algèbre large de $S$ sur $A$ par la même notation $\sum_{s \in S} \xi_s e_s$ (ou même $\sum_{s \in S} \xi_s . s$) que les éléments de l’algèbre stricte de $S$; bien entendu le signe de sommation qui figure dans cette notation ne correspond à aucune opération algébrique puisqu’il porte en général sur une infinité de termes $\neq 0$. Avec cette notation, la multiplication dans l’algèbre large de $S$ est encore donnée par la formule (35) de III, p. 19.

Si $S$ est commutatif, il en est de même de son algèbre large $A^S$. Si $T$ est un sous-monoïde de $S$, l’algèbre large $A^T$ du monoïde s’identifie canoniquement à une sous-algèbre de l’algèbre large de $S$. Si $\rho : A \to B$ est un homomorphisme d’anneaux, l’extension canonique $\rho^S : A^S \to B^S$ est un $A$-homomorphisme de l’algèbre large de $S$ sur $A$ dans l’algèbre large de $S$ sur $B$, qui prolonge l’homomorphisme canonique $A^{(S)} \to B^{(S)}$.

### 11. Séries formelles sur un anneau commutatif

Pour tout ensemble $I$, le monoïde additif $\mathbf{N}^{(I)}$ vérifie la condition (D) de III, p. 27: en effet, si $s = (n_i)_{i \in I}$ avec $n_i = 0$ sauf pour les indices $i$ d’une partie finie $H$ de $I$, la relation $s = t + u$ avec $t = (p_i)_{i \in I}$ et $u = (q_i)_{i \in I}$ équivaut à $p_i + q_i = n_i$ pour tout $i$; mais cela entraîne $p_i = q_i = 0$ pour $i \notin H$ et $p_i \leq n_i$, $q_i \leq n_i$ pour $i \in H$; il y a donc $\prod_{i \in H} (n_i + 1)$ couples $(t, u)$ dans $\mathbf{N}^{(I)}$ tels que $t + u = s$.

On peut donc considérer l’algèbre large sur $A$ du monoïde $\mathbf{N}^{(I)}$, qui contient l’algèbre (stricte) $A[[X_i]]_{i \in I}$ de ce monoïde. C’est une algèbre associative, commutative et unifère, qu’on appelle algèbre des séries formelles par rapport aux indéterminées $X_i$ ($i \in I$) et à coefficients dans $A$ et qu’on note $A[[X_i]]_{i \in I}$; ses éléments portent le nom de séries formelles par rapport aux indéterminées $X_i$ ($i \in I$), à coefficients dans $A$. Un tel élément $(\alpha_v)_{v \in \mathbf{N}^{(I)}}$ se note encore, suivant la convention faite dans III, p. 28, $\sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$; les $\alpha_v$ sont les coefficients de la série formelle, les $\alpha_v X^v$ ses termes; un polynôme en les $X_i$ est donc une série formelle n’ayant qu’un nombre fini de termes $\neq 0$.

Il est clair que de toute bijection $\sigma : I_1 \to I_2$, on déduit canoniquement un isomorphisme d’algèbres $A[[X_i]]_{i \in I_1} \to A[[X_i]]_{i \in I_2}$ en faisant correspondre à la série formelle $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_i^{n_i}$ la série formelle $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_{\sigma(i)}^{n_i}$.

Soit $J$ une partie de $I$; l’algèbre $A[[X_i]]_{i \in J}$ peut être identifiée à la sous-algèbre de $A[[X_i]]_{i \in I}$ constituée par les séries formelles $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ où α_{(n_i)} = 0 pour tout élément (n_i) \in \mathbf{N}^{(I)} tel que n_i \neq 0 pour un indice i \in I - J au moins. En outre, si K = I - J, A[[X_i]]_{i \in I} s’identifie canoniquement à (A[[X_j]]_{j \in J})[[X_k]]_{k \in K}, en identifiant la série formelle $\sum_{(n_i)} \alpha_{(n_i)} \prod_{i \in I} X_i^{n_i}$ à la série formelle $\sum_{(m_k)} \beta_{(m_k)} \prod_{k \in K} X_k^{m_k}$, où
$$
\beta_{(m_k)} = \sum_{(p_j)} \gamma_{(p_j)} \prod_{j \in J} X_j^{p_j}
$$
avec $\gamma_{(p_j)} = \alpha_{(n_i)}$ pour la suite $(n_i)$ telle que $n_i = p_i$ pour $i \in J$ et $n_i = m_i$ pour $i \in K$.

Etant donnée une série formelle $u = \sum_v \alpha_v X^v$, on appelle termes de degré total $p$ dans $u$ les termes $\alpha_v X^v$ tels que $|v| = p$. La série formelle $u_p$ dont les termes de degré total $p$ sont ceux de $u$ et dont les autres termes sont nuls, est dite partie homogène de degré $p$ de $u$; lorsque I est fini, $u_p$ est un polynôme pour tout $p$; $u_0$ s’identifie à un élément de A (dit encore terme constant de $u$). Si $u$ et $v$ sont deux séries formelles et $w = uv$, on a
$$
w_p = \sum_{r=0}^p u_r v_{p-r},
$$
pour tout entier $p \geq 0$.

Pour toute série formelle $u \neq 0$, on appelle ordre total (ou simplement ordre) de $u$ le plus petit des entiers $p \geq 0$ tels que $u_p \neq 0$. Si on désigne cet ordre par $\omega(u)$, et si $u$ et $v$ sont deux séries formelles $\neq 0$, on a
$$
\omega(u + v) \geq \inf(\omega(u), \omega(v)) \quad \text{si } u + v \neq 0
$$
$$
\omega(uv) \geq \omega(u) + \omega(v) \quad \text{si } uv \neq 0.
$$
En outre, si $\omega(u) \neq \omega(v)$, on a nécessairement $u + v \neq 0$ et les deux membres de (40) sont égaux.

On notera que l’ordre de 0 n’est pas défini. Par abus de langage on convient toutefois de dire que « $f$ est une série formelle d’ordre $\geq p$ (resp. $> p$) » si la partie homogène de degré $n$ de $f$ est nulle pour tout $n < p$ (resp. $n \leq p$); 0 est donc une « série formelle d’ordre $> p$ » pour tout entier $p \geq 0$.

Soit J une partie de I, et identifions comme ci-dessus A[[X_i]]_{i \in I} à B[[X_k]]_{k \in K}, avec K = I - J et B = A[[X_j]]_{j \in J}; aux définitions ci-dessus appliquées à B[[X_k]]_{k \in K} correspondent donc de nouvelles définitions pour les séries formelles $u \in A[[X_i]]_{i \in I}$: un terme $\alpha_{(n_i)} \prod_{i \in I} X_i^{n_i}$ est dit de degré $p$ par rapport aux $X_i$ d’indice $i \in K$ si $\sum_{i \in K} n_i = p$, et la série formelle de B[[X_k]]_{k \in K} ayant même termes de degré $p$ que $u$ et les autres nuls est dite partie homogène de degré $p$ par rapport aux $X_i$ d’indice $i \in K$. Si $u \neq 0$, l’ordre $\omega_K(u)$ par rapport aux $X_i$ d’indice $i \in K$ est le plus petit des entiers $p \geqslant 0$ tels que la partie homogène de degré $p$ de $u$ par rapport aux $X_i$ d’indice $i \in K$ soit $\neq 0$. On a encore les inégalités (40) et (41) lorsqu’on y remplace $\omega$ par $\omega_K$.

## EXERCICES {#alg-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
