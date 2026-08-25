---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 6
section_title: La série de Hausdorff
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0049-0058, 0088-0090
extraction: ocr
subsections:
    - "no": 1
      title: Exponentielle et logarithme dans les algèbres filtrées
      page: 0
      pdf_page: 49
    - "no": 2
      title: Groupe de Hausdorff
      page: 0
      pdf_page: 50
    - "no": 3
      title: Séries formelles de Lie
      page: 0
      pdf_page: 52
    - "no": 4
      title: La série de Hausdorff
      page: 0
      pdf_page: 53
    - "no": 5
      title: Substitutions dans la série de Hausdorff
      page: 0
      pdf_page: 55
statements: 20
exercises: 6
content_sha256: cc4c4c91056ceff910084b079cbdb9376ec061cce2e20fe4d3319ece23785316
---

## § 6. La série de Hausdorff

*On suppose dans ce paragraphe que $K$ est un corps de caractéristique 0.*

### 1. Exponentielle et logarithme dans les algèbres filtrées

Soit $A$ une algèbre associative unifière, séparée et complète pour une filtration réelle $(A_\alpha)$. On pose $m = A_0^+ = \bigcup_{\alpha > 0} A_\alpha$.

Pour $x \in m$, la famille $(x^n/n!)_{n \in \mathbf{N}}$ est sommable. On pose

$$
e^x = \exp x = \sum_{n \geq 0} x^n/n!.
$$

On a $\exp(x) \in 1 + m$, et l’application $\exp : m \to 1 + m$ est dite *application exponentielle* de $A$.

Pour tout $y \in 1 + m$, la famille $((-1)^{n-1}(y-1)^n/n)_{n \geq 1}$ est sommable. On pose

$$
\log y = \sum_{n \geq 1} (-1)^{n-1}(y-1)^n/n.
$$

On a $\log y \in m$, et l’application $\log : 1 + m \to m$ est dite *application logarithme* de $A$.

#### Proposition 1 {#lie-ii-s6-prop-1 .statement}

*L’application exponentielle est un homéomorphisme de $m$ sur $1 + m$ et l’application logarithme en est l’homéomorphisme réciproque*.

Pour $x \in A_\alpha$, on a $\frac{x^n}{n!} \in A_{n\alpha}$. Il en résulte que la série définissant l’exponentielle converge uniformément dans chacun des ensembles $A_\alpha$ pour $\alpha > 0$; comme $A_\alpha$ est ouvert dans $m$ et que $m = \bigcup_{\alpha > 0} A_\alpha$, l’application exponentielle est continue. On montre de même que l’application logarithme est continue.

Soient $e$ et $l$ les séries formelles sans terme constant

$$
e(\mathbf{X}) = \sum_{n \geq 1} \frac{\mathbf{X}^n}{n!} \qquad l(\mathbf{X}) = \sum_{n \geq 1} (-1)^{n-1} \mathbf{X}^n/n.
$$

$$
\exp x = e(x) + 1, \quad \log(1 + x) = l(x)
$$

on en déduit immédiatement

$$
\log \exp x = x, \quad \exp \log(1 + x) = 1 + x
$$

pour $x$ dans $m$, d’où la proposition.

#### Remarque 1 {#lie-ii-s6-n1-rem-1 .statement}

Si $x \in m, y \in m$ et si $x$ et $y$ commutent, on a $\exp(x + y) = \exp(x) \exp(y)$, la famille $\left( \frac{x^i}{i!} \cdot \frac{y^j}{j!} \right)_{i,j \in \mathbf{N}}$ étant sommable (cf. A, IV, § 6, n° 9, prop. 11).

#### Remarque 2 {#lie-ii-s6-n1-rem-2 .statement}

Comme les séries $e$ et $l$ sont sans terme constant et que $A_\alpha$ est un idéal fermé de $A$, on a $\exp A_\alpha \subset 1 + A_\alpha$ et $\log(1 + A_\alpha) \subset A_\alpha$ d’où $\exp A_\alpha = 1 + A_\alpha$ et $\log (1 + A_\alpha) = A_\alpha$ pour $\alpha > 0$.

#### Remarque 3 {#lie-ii-s6-n1-rem-3 .statement}

Soient $B$ une algèbre associative unifière filtrée, séparée et complète, et $n = \bigcup_{\alpha > 0} B_\alpha$. Soit $f$ un homomorphisme unifière continu de $A$ dans $B$ tel que $f(m) \subset n$. On a $f(\exp x) = \exp f(x)$ pour $x \in m$ et $f(\log y) = \log f(y)$ pour $y \in 1 + m$; démontrons par exemple la première de ces formules:

$$
f(\exp x) = \sum_{n \geq 0} f(x^n)/n! = \sum_{n \geq 0} f(x)^n/n! = \exp f(x).
$$

#### Remarque 4 {#lie-ii-s6-n1-rem-4 .statement}

Soit $E$ une algèbre associative unifière. Si $a$ est un élément nilpotent de $E$, la famille $\left( \frac{a^n}{n!} \right)_{n \in \mathbf{N}}$ est à support fini et on pose $\exp a = \sum_{n \geq 0} a^n/n!$. On dit qu’un élément $b$ est unipotent si $b - 1$ est nilpotent; on pose alors $\log b = \sum_{n \geq 1} (-1)^{n-1}(b - 1)^n/n$. On déduit des relations $e(l(X)) = l(e(X)) = X$ que l’application $a \mapsto \exp a$ est une bijection de l’ensemble des éléments nilpotents de $E$ sur l’ensemble des éléments unipotents de $E$, et que $b \mapsto \log b$ en est l’application réciproque.

### 2. Groupe de Hausdorff

Soit $X$ un ensemble. Reprenons les notations du § 5, n°s 1 et 2. On identifie l’algèbre de Lie libre $L(X)$ à son image canonique dans $A(X)$ (\S 3, n° 1, th. 1). On notera $\hat{L}(X)$ l’adhérence de $L(X)$ dans $\hat{A}(X)$, c’est-à-dire l’ensemble des éléments de $\hat{A}(X)$ de la forme $a = \sum_{n \geq 1} a_n$ tels que $a_n \in L^n(X)$ pour tout $n \geq 0$; c’est une sous-algèbre de Lie filtrée de $\hat{A}(X)$.

#### Théorème 1 {#lie-ii-s6-thm-1 .statement}

La restriction de l’application exponentielle de $\hat{A}(X)$ à $\hat{L}(X)$ est une bijection de $\hat{L}(X)$ sur un sous-groupe fermé du groupe de Magnus $\Gamma(X)$.

Posons $A(X) = A, \quad A^n(X) = A^n, \quad \hat{A}(X) = \hat{A}, \quad L^n(X) = L^n, \quad \hat{L}(X) = \hat{L}, \quad \Gamma(X) = \Gamma$. Soit B l’algèbre $A \otimes A$ munie de la graduation de type $\mathbf{N}$ définie par $B^n = \sum_{i+j=n} A^i \otimes A^j$. Soit $\hat{B} = \prod_{n \geq 0} B^n$ l’algèbre filtrée complète associée (AC, III, § 2, no 12, Exemple 1). Le coproduit $c : A \to A \otimes A$ défini au § 3, no 1, cor. 1 du th. 1, est gradué de degré 0, donc se prolonge par continuité en un homomorphisme $\hat{c} : \hat{A} \to \hat{B}$ donné par
$$
\hat{c}\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} c(a_n) \quad \text{pour } a_n \in A^n.
$$
On définit aussi les homomorphismes continus $\delta'$ et $\delta''$ de $\hat{A}$ dans $\hat{B}$ par
$$
\delta'\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (a_n \otimes 1), \qquad \delta''\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (1 \otimes a_n) \quad \text{pour } a_n \in A^n.
$$
D’après le cor. 2 du th. 1 du § 3, no 1, $L^n$ est l’ensemble des $a_n \in A^n$ tels que $c(a_n) = a_n \otimes 1 + 1 \otimes a_n$. Il en résulte que $\hat{L}$ est l’ensemble des $a \in \hat{A}$ tels que
$$
\hat{c}(a) = \delta'(a) + \delta''(a).
$$
Soit $\Delta$ l’ensemble des $b \in \hat{A}$ de terme constant égal à 1 et satisfaisant à la relation
$$
\hat{c}(b) = \delta'(b) \cdot \delta''(b),
$$
autrement dit, l’ensemble des $b = \sum_{n \geq 0} b_n$ tels que $b_n \in A^n$ pour tout $n \geq 0$, $b_0 = 1$ et $c(b_n) = \sum_{i+j=n} b_i \otimes b_j$ pour $n \geq 0$. Cette dernière caractérisation montre que $\Delta$ est une partie fermée de $\Gamma$; comme $\hat{c}, \delta'$ et $\delta''$ sont des homomorphismes d’anneaux, et que tout élément de $\delta'(\hat{A})$ commute à tout élément de $\delta''(\hat{A})$, les restrictions à $\Gamma$ des applications $\hat{c}$ et $\delta'\delta''$ sont des homomorphismes de groupes et $\Delta$ est un sous-groupe de $\Gamma$.

D’après la prop. 1 du no 1, l’application exponentielle de $\hat{A}$ est une bijection de l’ensemble $\hat{A}^+$ des éléments de $\hat{A}$ sans terme constant sur $\Gamma$. Soient $a \in \hat{A}^+$ et $b = \exp a$. Comme $\hat{c}$ est un homomorphisme continu d’anneaux, on a
$$
\hat{c}(b) = \hat{c}\left( \sum_{n \geq 0} a^n/n! \right) = \sum_{n \geq 0} \hat{c}(a)^n/n! = \exp \hat{c}(a).
$$
On prouve de même les relations
$$
\delta'(b) = \exp \delta'(a), \qquad \delta''(b) = \exp \delta''(a),
$$
et comme $\delta'(a)$ commute à $\delta''(a)$, on a (no 1, Remarque 1)
$$
\delta'(b)\delta''(b) = \exp (\delta'(a) + \delta''(a)).
$$
Par suite, $a$ satisfait à (3) si et seulement si $b$ satisfait à (4), ce qui démontre le théorème.

#### Remarque {#lie-ii-s6-n2-rem-1 .statement}

La démonstration précédente montre que exp(\hat{L}) est le sous-groupe $\Delta$ de $\Gamma$ formé des $b$ satisfaisant à (4).

On peut donc transporter par l’application exponentielle la loi de groupe de $\Delta$ à $\hat{L}$. Autrement dit, $\hat{L}$ est un groupe topologique complet pour la loi de composition $(a, b) \mapsto a \circledast b$ donnée par
$$
a \circledast b = \log(\exp a \cdot \exp b).
$$
Le groupe topologique ainsi obtenu s’appelle le groupe de Hausdorff (déduit de X relativement à K).

Soit $g$ l’homomorphisme du groupe libre $F = F(X)$ dans $\Gamma$ tel que $g(x) = \exp x$ pour $x \in X$. Comme $\exp x - 1 - x = \sum_{n \geq 2} x^n / n!$ est d’ordre $\geq 2$, $g$ est injectif d’après le th. 1 du § 5, no 3. Par suite, l’application $\log \circ g$ est un homomorphisme injectif de $F$ dans le groupe de Hausdorff qui prolonge l’injection canonique $X \to \hat{L}$.

Pour tout entier $m \geq 1$, on note $\hat{L}_m$ l’ensemble des éléments d’ordre $\geq m$ de $\hat{L}$ et $\Gamma_m$ l’ensemble des $u \in \Gamma$ tels que $u - 1$ soit d’ordre $\geq m$. On a $\hat{L}_m = \exp^{-1}(\Gamma_m)$ d’après la Remarque 2 du no 1 ; comme $(\Gamma_m)_{m \geq 1}$ est une filtration centrale entière sur $\Gamma$ (§ 4, no 5, prop. 2), $(\hat{L}_m)_{m \geq 1}$ est une filtration centrale entière sur le groupe $\hat{L}$.

### 3. Séries formelles de Lie

#### Lemme 1 {#lie-ii-s6-lem-1 .statement}

Soient $g$ une algèbre de Lie filtrée (§ 4, no 1), $(g_\alpha)_{\alpha \in \mathbf{R}}$ sa filtration, et soit $\alpha \in \mathbf{R}$. Soit P un polynôme de Lie homogène de degré $n$ en les indéterminées $(T_i)_{i \in I}$ (§ 2, no 4). On a $P((a_i)) \in g_{n\alpha}$ pour toute famille $(a_i)_{i \in I}$ d’éléments de $g_\alpha$.

Tout polynôme de Lie de degré $n \geq 2$ est somme finie de termes de la forme $[Q, R]$ où $Q$ et $R$ sont de degré $< n$ et dont la somme des degrés est égale à $n$ (§ 2, no 7, prop. 7). Le lemme en résulte par récurrence sur $n$.

On appelle série formelle de Lie$^1$ (à coefficients dans $K$) en les indéterminées $(T_i)_{i \in I}$ tout élément de l’algèbre de Lie $\hat{L}((T_i)_{i \in I}) = \hat{L}(I)$. Un tel élément $u$ s’écrit de manière unique comme somme d’une famille sommable $(u_v)_{v \in \mathbf{N}^{(I)}}$ où $u_v \in L^v(I)$.

Supposons I fini. Soit $g$ une algèbre de Lie filtrée séparée et complète, telle que $g = \bigcup_{\alpha > 0} g_\alpha$; soit $t = (t_i)_{i \in I}$ une famille d’éléments de $g$.

#### Proposition 2 {#lie-ii-s6-prop-2 .statement}

L’homomorphisme $f_t : L(I) \to g$ tel que $f_t(T_i) = t_i$ (§ 2, no 4) se prolonge par continuité en un homomorphisme continu, et un seul, $f_t$ de $\hat{L}(I)$ dans $g$.

En effet, il existe $\alpha > 0$ tel que $t_i \in g_\alpha$ pour tout $i \in I$; on a donc $f_t(L^v(I)) \subset g_{|v|\alpha}$ pour tout $v$ (lemme 1), ce qui entraîne la continuité de $f_t$.

C.Q.F.D.

1 Une série formelle de Lie n’est pas en général une série formelle au sens de A, IV, § 6.

Si $u \in \hat{\mathbf{L}}(\mathbf{I})$, on pose $u((t_i)) = \hat{f}_t(u)$. En particulier, prenant $g = \hat{\mathbf{L}}(\mathbf{I})$, on a $u = u((T_i))$; dans le cas général, on dit que $u((t_i))$ est le résultat de la substitution des $t_i$ aux $T_i$ dans la série formelle de Lie $u((T_i))$. Si $u = \sum_{v \in \mathbf{N}^{(I)}} u_v$, avec $u_v \in \mathbf{L}^v(X)$, la famille $(u_v((t_i)))_{v \in \mathbf{N}^{(I)}}$ est sommable et

$$
u((t_i)) = \sum_{v \in \mathbf{N}^I} u_v((t_i)).
$$

Soit $\sigma$ un homomorphisme continu de $g$ dans une algèbre de Lie filtrée séparée et complète $g'$, telle que $g' = \bigcup_{\alpha > 0} g'_\alpha$. Pour toute famille finie $t = (t_i)_{i \in I}$ d’éléments de $g$ et tout $u \in \hat{\mathbf{L}}(\mathbf{I})$, on a

$$
\sigma(u((t_i))) = u((\sigma(t_i))),
$$

car l’homomorphisme $\sigma \circ \hat{f}_t$ est continu et applique $T_i$ sur $\sigma(t_i)$, pour $i \in I$.

Soit $u = (u_j)_{j \in J}$ une famille finie d’éléments de $\hat{\mathbf{L}}(\mathbf{I})$ et soit $v \in \hat{\mathbf{L}}(\mathbf{J})$; par substitution des $u_j$ aux $T_j$ dans $v$, on obtient un élément $w = v((u_j)_{j \in J})$ de $\hat{\mathbf{L}}(\mathbf{I})$ noté $v \circ u$. On a

$$
w((t_i)_{i \in I}) = v((u_j((t_i)_{i \in I}))_{j \in J}),
$$

pour toute famille finie $t = (t_i)_{i \in I}$ d’éléments de $g$, comme on le voit en transformant par l’homomorphisme continu $\hat{f}_t$ l’égalité $w = v((u_j)_{j \in J})$.

Soit $u = \sum_{v \in \mathbf{N}^I} u_v \in \hat{\mathbf{L}}(\mathbf{I})$, avec $u_v \in \mathbf{L}^v(\mathbf{I})$. L’application $\tilde{u}: (t_i) \mapsto u((t_i))$ de $g^I$ dans $g$ est continue: en effet, dans chacun des ouverts $g_\alpha$ pour $\alpha > 0$, la famille des $\tilde{u}_v$ est uniformément sommable et il suffit de prouver que chaque $\tilde{u}_v$ est continue, ce qui est immédiat par récurrence sur $|v|$.

### 4. La série de Hausdorff

Soit $\{U, V\}$ un ensemble à deux éléments.

#### Définition 1 {#lie-ii-s6-def-1 .statement}

L’élément $H = U \mathbin{\&} V = \log(\exp U . \exp V)$ (n° 2) de l’algèbre de Lie $\hat{\mathbf{L}}_q(\{U, V\})$ s’appelle la série de Hausdorff en les indéterminées $U$ et $V$.

On désigne par $H_n$ (resp. $H_{r,s}$) la composante homogène de degré total $n$ (resp. de multidegré $(r, s)$) de $H$. On a

$$
H = \sum_{n \geq 0} H_n = \sum_{r,s \geq 0} H_{r,s} \qquad H_n = \sum_{\substack{r+s=n \\ r,s \geq 0}} H_{r,s}.
$$

#### Théorème 2 {#lie-ii-s6-thm-2 .statement}

Si r et s sont deux entiers positifs, tels que $r + s \geqslant 1$, on a $\mathbf{H}_{r,s} = \mathbf{H}'_{r,s} + \mathbf{H}''_{r,s}$ avec

(9) $$ (r + s) \mathbf{H}'_{r,s} = \sum_{m \geqslant 1} \frac{(-1)^{m-1}}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s - 1 \\ r_1 + s_1 \geqslant 1, \ldots, r_{m-1} + s_{m-1} \geqslant 1}} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m}}{r_m!} (\mathrm{V}) $$

(10) $$ (r + s) \mathbf{H}''_{r,s} = \sum_{m \geqslant 1} \frac{(-1)^{m-1}}{m} \sum_{\substack{r_1 + \cdots + r_{m-1} = r - 1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geqslant 1, \ldots, r_{m-1} + s_{m-1} \geqslant 1}} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) (\mathrm{U}). $$

Dans $\hat{A}_q(\{\mathrm{U}, \mathrm{V}\})$, on a $\exp \mathrm{U} . \exp \mathrm{V} = 1 + \mathrm{W}$ avec $\mathrm{W} = \sum_{r+s \geqslant 1} \frac{\mathrm{U}^r}{r!} \frac{\mathrm{V}^s}{s!}$, d’où $\mathbf{H} = \sum_{m \geqslant 1} (-1)^{m-1} \mathrm{W}^m / m$ (n° 2), c’est-à-dire:

(11) $$ \mathbf{H}_{r,s} = \sum_{m \geqslant 1} \frac{(-1)^{m-1}}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geqslant 1, \ldots, r_m + s_m \geqslant 1}} \prod_{i=1}^m \frac{\mathrm{U}^{r_i}}{r_i!} \frac{\mathrm{V}^{s_i}}{s_i!}. $$

L’application linéaire $P_n$, définie par $P_n(x_1, \ldots, x_n) = \frac{1}{n} \left( \prod_{i=1}^{n-1} (\mathrm{ad}\ x_i) \right)(x_n)$ pour $n \geqslant 1$ et $x_1, \ldots, x_n$ dans $\{\mathrm{U}, \mathrm{V}\}$, est un projecteur de $A_q^n(\{\mathrm{U}, \mathrm{V}\})$ sur $L_q^n(\{\mathrm{U}, \mathrm{V}\})$ (§ 3, n° 2, cor. de la prop. 1); comme $\mathbf{H}_{r,s}$ appartient à $L_q^{r+s}(\{\mathrm{U}, \mathrm{V}\})$, on a $\mathbf{H}_{r,s} = P_{r+s}(\mathbf{H}_{r,s})$. Or, on a

(12) $$
P_{r+s} \left( \prod_{i=1}^m \frac{\mathrm{U}^{r_i}}{r_i!} \frac{\mathrm{V}^{s_i}}{s_i!} \right)
= \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m}}{r_m!} \frac{(\mathrm{ad}\ V)^{s_m-1}}{s_m!} \right) (\mathrm{V})
$$
lorsque $s_m \geqslant 1$, et
(13) $$
P_{r+s} \left( \prod_{i=1}^m \frac{\mathrm{U}^{r_i}}{r_i!} \frac{\mathrm{V}^{s_i}}{s_i!} \right)
= \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m-1}}{r_m!} \right) (\mathrm{U})
$$
lorsque $r_m \geqslant 1$ et $s_m = 0$. De plus, on a évidemment $(\mathrm{ad}\ t)^{p-1} . t = 0$ si $p \geqslant 2$ et $(\mathrm{ad}\ t)^0 . t = t$. Il en résulte que les deux membres de (12) sont nuls lorsque $s_m \geqslant 2$ et que ceux de (13) le sont lorsque $r_m \geqslant 2$. Le théorème résulte de là, $\mathbf{H}'_{r,s}$ étant la somme des termes du type (12) et $\mathbf{H}''_{r,s}$ celle des termes du type (13).

C.Q.F.D.

#### Remarque 1 {#lie-ii-s6-n4-rem-1 .statement}

On a défini (\S 3, n° 2, Remarque) un projecteur Q de A(X) sur L(X) tel que Q(a^m) = 0 pour $a \in L(X)$ et $m \geq 2$, et Q(1) = 0. On a alors $H = Q(\exp H) = Q(\exp U \cdot \exp V)$, d’où immédiatement

$$
H_{r,s} = Q \left( \frac{U^r}{r!} \frac{V^s}{s!} \right) \quad \text{pour } r + s \geq 1.
$$

#### Remarque 2 {#lie-ii-s6-n4-rem-2 .statement}

On a

$$
H(U, V) \equiv U + V + \frac{1}{2}[U, V] + \frac{1}{12}[U, [U, V]] \\
+ \frac{1}{12}[V, [V, U]] - \frac{1}{24}[U, [V, [U, V]]]
$$
modulo $\sum_{n \geq 5} L^n(\{U, V\})$.

#### Remarque 3 {#lie-ii-s6-n4-rem-3 .statement}

On a $H_{0,n} = H_{n,0} = 0$ pour tout entier $n \neq 1$, d’où

$$
H(U, 0) = H(0, U) = U.
$$

D’autre part, comme $[U, -U] = 0$, on a

$$
H(U, -U) = 0.
$$

### 5. Substitutions dans la série de Hausdorff

Comme K est un corps contenant $\mathbf{Q}$, la série de Hausdorff peut être considérée comme une série formelle de Lie à coefficients dans K. Par suite, si $g$ est une algèbre de Lie filtrée, séparée et complète avec $g = \bigcup_{\alpha > 0} g_\alpha$, on peut, pour $a, b$ dans $g$, substituer $a$ et $b$ à U et V dans H (cf. n° 3 et \S 2, n° 5, Remarque).

En particulier, soit A une algèbre associative unifière, filtrée, séparée et complète. Posons $m = \bigcup_{\alpha > 0} A_\alpha$ et $m_\alpha = A_\alpha \cap m$ pour $\alpha \in \mathbf{R}$; on a donc $m_\alpha = A_\alpha$ pour $\alpha > 0$ et $m_\alpha = m$ pour $\alpha \leq 0$. Pour le crochet $[a, b] = ab - ba$, m est une algèbre de Lie filtrée, séparée et complète, à laquelle on peut appliquer ce qui précède. Avec ces notations, on a le résultat suivant, qui complète la prop. 1 du n° 1.

#### Proposition 3 {#lie-ii-s6-prop-3 .statement}

Si $a \in m, b \in m$, on a $\exp H(a, b) = \exp a \cdot \exp b$.

Soient $a, b$ dans $m$; il existe $\alpha > 0$ tel que $a \in A_\alpha$ et $b \in A_\alpha$. Par suite, il existe un homomorphisme continu $\theta$ de l’algèbre de Magnus $\hat{A}(\{U, V\})$ dans A appliquant U sur $a$ et V sur $b$ (\S 5, n° 1, prop. 1).

La restriction de $\theta$ à $\hat{L}(\{U, V\})$ est un homomorphisme continu d’algèbres de Lie de $\hat{L}(\{U, V\})$ dans m qui applique U (resp. V) sur $a$ (resp. $b$). D’après la formule (6) du n° 3, on a donc $\theta(H) = H(a, b)$. Il suffit alors d’appliquer l’homomorphisme continu $\theta$ aux deux membres de la relation $\exp H(U, V) = \exp U \cdot \exp V$ en tenant compte de la Remarque 3 du n° 1.

#### Remarque 1 {#lie-ii-s6-n5-rem-1 .statement}

Si $a$ et $b$ commutent, on a $H_{r,s}(a,b) = 0$ pour $r + s \geq 2$, car tout polynôme de Lie homogène de degré $\geq 2$ est nul en $(a,b)$. On a donc $H(a,b) = a + b$, et la prop. 3 redonne la formule $\exp(a + b) = \exp a . \exp b$.

#### Proposition 4 {#lie-ii-s6-prop-4 .statement}

Soit $g$ une algèbre de Lie filtrée, séparée et complète, telle que $g = \bigcup_{\alpha > 0} g_\alpha$.

L’application $(a, b) \mapsto H(a, b)$ est une loi de groupe sur $g$, compatible avec la topologie de $g$, pour laquelle $0$ est élément neutre et $-a$ est inverse de $a$, pour tout $a \in g$.

L’application $(a, b) \mapsto H(a, b)$ de $g \times g$ dans $g$ est continue (n° 3); comme l’application $a \mapsto -a$ est évidemment continue, il suffit de prouver les relations

$$
\text{(18)} \qquad H(H(a, b), c) = H(a, H(b, c))
$$
$$
\text{(19)} \qquad H(a, -a) = 0
$$
$$
\text{(20)} \qquad H(a, 0) = H(0, a) = a
$$

pour $a, b, c$ dans $g$. D’après la formule (7) du n° 3, il suffit de démontrer ces formules lorsque $a, b, c$ sont trois indéterminées et que $g = \hat{L}(\{a, b, c\})$. Or la restriction de l’application exponentielle à $\hat{L}(\{a, b, c\})$ est une injection dans l’algèbre de Magnus $\hat{A}(\{a, b, c\})$ et l’on a d’après la prop. 3:

$$
\begin{align*}
\exp H(H(a, b), c) &= \exp H(a, b) . \exp c = \exp a . \exp b . \exp c \\
\exp H(a, H(b, c)) &= \exp a . \exp H(b, c) = \exp a . \exp b . \exp c \\
\exp H(a, -a) &= \exp a . \exp(-a) = \exp(a - a) = \exp 0 \\
\exp H(a, 0) &= \exp a . \exp 0 = \exp a \\
\exp H(0, a) &= \exp 0 . \exp a = \exp a.
\end{align*}
$$

Ceci établit les relations (18) à (20).

#### Remarque 2 {#lie-ii-s6-n5-rem-2 .statement}

Prenons pour $g$ l’algèbre de Lie $\hat{L}(X)$. La loi de groupe introduite dans la proposition précédente coïncide avec la loi définie au n° 2. En d’autres termes, on a

$$
\text{(21)} \qquad a \circledast b = H(a, b) \qquad \text{pour } a, b \text{ dans } \hat{L}(X);
$$

la loi du groupe de Hausdorff est donc donnée par la série de Hausdorff.

#### Remarque 3 {#lie-ii-s6-n5-rem-3 .statement}

Soit $g$ une algèbre de Lie munie de la filtration entière $(\mathcal{C}^n g)$ définie par la suite centrale descendante. Supposons qu’il existe un $m \geq 1$ tel que $\mathcal{C}^m g = \{0\}$. Pour la topologie déduite de la filtration $(\mathcal{C}^n g)_{n \geq 1}$, l’algèbre de Lie $g$ est séparée, complète, et même discrète. On a $P(a_1, \ldots, a_r) = 0$ pour $a_1, \ldots, a_r$ dans $g$ et pour tout polynôme de Lie $P$ homogène de degré $\geq m$; en particulier, on a $H_{r,s}(a, b) = 0$ pour $r + s \geq m$, et la série $H(a, b) = \sum_{r,s} H_{r,s}(a, b)$ n’a qu’un nombre fini de termes non nuls. La loi de groupe $(a, b) \mapsto H(a, b)$ sur $g$ est alors une application polynomiale (\S 2, n° 4).

§ 5
LA SÉRIE DE HAUSDORFF

#### Proposition 5 {#lie-ii-s6-prop-5 .statement}

Soit $K_{r,s}$ la composante de multidegré $(r, s)$ de $H(U + V, -U)$. On a

$$
K_{n,1}(U, V) = \frac{1}{(n+1)!} (\operatorname{ad} U)^n(V) \quad \text{pour } n \geq 0.
$$

En effet, posons $K(U, V) = H(U + V, -U)$, $K_1(U, V) = \sum_{n \geq 0} K_{n,1}(U, V)$. Notons $L$ (resp. $R$) la multiplication à gauche (resp. à droite) par $U$ dans $\hat{A}(\{U, V\})$.

On peut écrire

$$
e^{UV} e^{-U} = \sum_{p, q} \frac{U^p}{p!} V \frac{(-U)^q}{q!}
$$
$$
= \sum_{n \geq 0} \frac{1}{n!} \left( \sum_{p+q=n} \frac{n!}{p!q!} (L^p(-R)^q) . V \right)
$$
$$
= \sum_{n \geq 0} \frac{1}{n!} (L - R)^n . V
$$

et par suite

$$
e^{UV} e^{-U} = \sum_{n \geq 0} \frac{1}{n!} (\operatorname{ad} U)^n V.
$$

Calculons maintenant modulo l’idéal $\sum_{m \geq 0} \sum_{n \geq 2} A^{m,n}(\{U, V\})$ de $A(\{U, V\})$. Pour tout $n \geq 1$, on a

$$
(U + V)^n \equiv U^n + \sum_{i=1}^{n-1} U^i V U^{n-1-i}
$$

d’où

$$
(\operatorname{ad} U)(U + V)^n \equiv ((L - R) \sum_{i=1}^{n-1} L^i R^{n-i}) . V
$$
$$
\equiv (L^n - R^n) . V
$$
$$
\equiv U^n V - V U^n.
$$

Par suite, on a

$$
(\operatorname{ad} U) . e^{U+V} \equiv e^{UV} - V e^U
$$

par sommation sur $n$.

Par ailleurs, $K_1(U, V) \equiv K(U, V)$ et $e^{K_1(U,V)} \equiv 1 + K_1(U, V)$, donc

$$
K_1 \equiv e^K - 1 \equiv e^{U+V} e^{-U} - 1
$$

d’après la prop. 3. On en déduit

$$
(\mathrm{ad}\ U)\mathbf{K}_1 \equiv U e^{U+V} e^{-U} - e^{U+V} e^{-U} U \equiv (U e^{U+V} - e^{U+V} U) e^{-U}
$$
$$
\equiv (e^{UV} - V e^U) e^{-U} \tag{d’après (23)}
$$
$$
\equiv e^{UV} e^{-U} - V
$$
$$
\equiv \sum_{n \geq 1} \frac{1}{n!} (\mathrm{ad}\ U)^n V \tag{d’après (22)}
$$
$$
\equiv (\mathrm{ad}\ U) \left( \sum_{n \geq 0} \frac{(\mathrm{ad}\ U)^n}{(n+1)!} V \right).
$$

Il suffit alors d’appliquer la Remarque du § 2, n° 11.

## EXERCICES {#lie-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
