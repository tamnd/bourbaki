---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 3
section_title: FRACTIONS RATIONNELLES
lang: fr
source: alg-iv-vii-fr
book_pages: A IV.18-A IV.23, A IV.84-A IV.85
pdf_pages: 0025-0030, 0091-0092
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fractions rationnelles
      page: 18
      pdf_page: 25
    - "no": 2
      title: Degrés
      page: 18
      pdf_page: 25
statements: 6
exercises: 7
content_sha256: fd149733f01f17427044dbf3404b8eaf26287c34c678118725924b0cf66ffa82
---

## § 3. FRACTIONS RATIONNELLES

### 1. Définition des fractions rationnelles

#### Définition 1 {#alg-iv-s3-def-1 .statement}

Soient K un corps commutatif, I un ensemble. Le corps des fractions (I, p. 110) de l’anneau intègre $K[(X_i)_{i \in I}]$ se note $K((X_i)_{i \in I})$ ou $K(X_i)_{i \in I}$. Ses éléments s’appellent les fractions rationnelles à coefficients dans K par rapport aux indéterminées $X_i$.

Pour $I = \{1, 2, ..., n\}$, on écrit $K(X_1, X_2, ..., X_n)$ au lieu de $K((X_i)_{i \in I})$.

Soient A un anneau intègre, K son corps des fractions. L’anneau $A[(X_i)_{i \in I}]$ s’identifie à un sous-anneau de $K[(X_i)_{i \in I}]$, donc de $K((X_i)_{i \in I})$. Pour tout $f \in K[(X_i)_{i \in I}]$, il existe un élément non nul $\alpha$ de A tel que $\alpha f \in A[(X_i)_{i \in I}]$. Donc, tout élément de $K((X_i)_{i \in I})$ peut se mettre sous la forme $u/v$, où $u, v \in A[(X_i)_{i \in I}]$, $v \neq 0$. Donc $K((X_i)_{i \in I})$ s’identifie au corps des fractions de $A[(X_i)_{i \in I}]$.

Soient maintenant K un corps commutatif, I un ensemble et $J \subset I$. Posons $B = K[(X_i)_{i \in J}]$. Alors $K[(X_i)_{i \in I}] = B[(X_i)_{i \in I - J}]$. D’après ce qui précède, $K((X_i)_{i \in I})$ s’identifie à $K'((X_i)_{i \in I - J})$, où $K' = K((X_i)_{i \in J})$.

### 2. Degrés

Soit K un corps commutatif. Pour tout élément $r$ de $K((X_i)_{i \in I})$, il existe $u, v \in K[(X_i)_{i \in I}]$ tels que $v \neq 0$ et $r = \frac{u}{v}$. La relation $\frac{u}{v} = \frac{u_1}{v_1}$ où $v \neq 0, v_1 \neq 0$, équivaut à $uv_1 = vu_1$; si $r \neq 0$, on a $u \neq 0$ et $u_1 \neq 0$ et alors $\deg u + \deg v_1 = \deg v + \deg u_1$ (IV, p. 9), ou encore $\deg u - \deg v = \deg u_1 - \deg v_1$. L’entier rationnel $\deg u - \deg v$ ne dépend donc que de $r$; on dit que c’est le *degré*, ou le *degré total* de $r$. On le note $\deg r$. On convient que $\deg 0 = -\infty$. Si $J \subset I$, on définit de même le degré par rapport aux $X_j$ d’indices $j \in J$. Lorsque $r$ est un polynôme, ces notions coïncident avec celles qu’on a définies en IV, p. 3.

#### Proposition 1 {#alg-iv-s3-prop-1 .statement}

*Soient r, s deux fractions rationnelles.*
(i) *Si $\deg r \neq \deg s$, on a*
$$
r + s \neq 0 \quad \text{et} \quad \deg(r + s) = \sup(\deg r, \deg s) .
$$
*Si $\deg r = \deg s$, on a* $\deg(r + s) \leq \deg r$.
(ii) *On a* $\deg(rs) = \deg r + \deg s$.
On peut se limiter au cas où $r$ et $s$ sont non nuls.
Écrivons $r = \frac{u}{v}, s = \frac{w}{z}$, où $u, v, w, z$ sont des polynômes non nuls. On a $rs = \frac{uw}{vz}$, donc
$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z = \deg r + \deg s .
$$
D’autre part, on a $r + s = \frac{uz + vw}{vz}$. Supposons $\deg r \neq \deg s$; autrement dit, $\deg u + \deg z \neq \deg w + \deg v$. Alors $uz + wv \neq 0$, et
$$
\begin{align*}
\deg(r + s) &= \deg(uz + wv) - \deg(vz) \\
&= \sup(\deg(uz), \deg(wv)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s) .
\end{align*}
$$
Supposons $\deg r = \deg s$, c’est-à-dire $\deg u + \deg z = \deg w + \deg v$. Si $r + s \neq 0$, on a
$$
\begin{align*}
\deg(r + s) &= \deg(uz + wv) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r .
\end{align*}
$$
\* L’application $r \mapsto -\deg r$ est donc une valuation discrète sur le corps $K((X_i)_{i \in I})$. \*

3. **Substitutions**

Soient $K$ un corps commutatif, $E$ une $K$-algèbre associative unifère, $x = (x_i)_{i \in I}$ une famille d’éléments de $E$ deux à deux permutables. Soient $B = K[(X_i)_{i \in I}]$ et $S_x$ l’ensemble des $v \in B$ non nuls tels que $v(x)$ soit inversible dans $E$. Soient $u \in B, v \in S_x$, et $f = \frac{u}{v} \in K((X_i)_{i \in I})$. L’élément $u(x)\ v(x)^{-1} = v(x)^{-1}u(x)$ est défini dans E ; en outre, si $u_1$ et $v_1$ sont deux polynômes tels que $f = \frac{u_1}{v_1}$ et $v_1 \in S_x$, on a $uv_1 = u_1 v$, donc $u(x)\ v_1(x) = u_1(x)\ v(x)$, donc

$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

Soit $f \in K((X_i)_{i \in I})$. S’il existe au moins un couple $(u, v)$ tel que $f = \frac{u}{v}$ et $v \in S_x$, on dit que x est substituable dans $f$; l’élément $u(x)\ v(x)^{-1}$, qui ne dépend que de $f$ et x, se note alors $f(x)$ ou $f((x_i))$ ou $f((x_i)_{i \in I})$.

#### Proposition 2 {#alg-iv-s3-prop-2 .statement}

*Soient K un corps commutatif, E une K-algèbre associative unifère, x = $(x_i)_{i \in I}$ une famille d’éléments de E deux à deux permutables. L’ensemble $S_x^{-1}B$ des $f \in K((X_i)_{i \in I})$ telles que x soit substituable dans f est une sous-K-algèbre de $K((X_i)_{i \in I})$. L’application $f \mapsto f(x)$ est un homomorphisme unifère $\varphi$ de $S_x^{-1}B$ dans E. L’image $\varphi(S_x^{-1}B)$ est l’ensemble des $yz^{-1}$ où y parcourt la sous-algèbre unifère $K[x]_E$ de E engendrée par la famille x et où z parcourt l’ensemble des éléments inversibles de $K[x]_E$.*

Soient $f_1 = \frac{u_1}{v_1}$, $f_2 = \frac{u_2}{v_2}$ deux éléments de $K((X_i)_{i \in I})$ tels que $v_1,\ v_2 \in S_x$. On a
$$
f_1 + f_2 = \frac{u_1 v_2 + u_2 v_1}{v_1 v_2},\ f_1 f_2 = \frac{u_1 u_2}{v_1 v_2},\ \text{et}\ v_1 v_2 \in S_x.$$
Donc $S_x^{-1}B$ est une sous-K-algèbre de $K((X_i)_{i \in I})$. Le reste de la proposition est évident.

#### Corollaire {#alg-iv-s3-n2-cor-1 .statement}

*Soient L un corps commutatif, K un sous-corps de L, x = $(x_i)_{i \in I}$ une famille d’éléments de L, M l’ensemble des $x_i$, U l’ensemble des $f \in K((X_i)_{i \in I})$ telles que x soit substituable dans f, $\varphi$ l’homomorphisme $f \mapsto f(x)$ de U dans L. Alors $\varphi(U)$ est le sous-corps de L engendré par K $\cup$ M.*

Soit L’ le sous-corps de L engendré par K $\cup$ M. On a
$$
K \cup M \subset \varphi(U) \subset L'
$$
et $\varphi(U)$ est un sous-anneau de L. La prop. 2 entraîne que $\varphi(U)$ est un sous-corps de L, d’où $\varphi(U) = L'$.

Soit $f \in K((X_i)_{i \in I})$. Soit $(g_i)_{i \in I}$ une famille d’éléments de $K((Y_l)_{l \in L})$. Si $(g_i)$ est substituable dans $f$, $f((g_i))$ est un élément de $K((Y_l)_{l \in L})$. En particulier, $(X_i)_{i \in I}$ est substituable dans $f$, et $f = f((X_i)_{i \in I})$.

#### Proposition 3 {#alg-iv-s3-prop-3 .statement}

*Soit E une algèbre sur K, associative, commutative, unifère et non nulle. Soit $f \in K((X_i)_{i \in I})$. Pour tout $i \in I$, soit $g_i \in K((Y_l)_{l \in L})$. Soit $y = (y_l)_{l \in L}$ une famille d’éléments de E. On suppose que y est substituable dans chaque $g_i$, et que $(g_i(y))_{i \in I}$ est substituable dans $f$. Alors :*

(i) $(g_i)_{i\in I}$ est substituable dans $f$;
(ii) si l’on note $h$ l’élément $f((g_i))$ de $K((Y_i)_{i\in L})$, alors $y$ est substituable dans $h$, et $h(y) = f((g_i(y)))$.

On peut supposer $I$ fini. Par hypothèse, pour tout $i \in I$, $g_i$ peut se mettre sous la forme $p_i/q_i$, où $p_i, q_i \in K[(Y_i)_{i\in L}]$ et $q_i(y)$ est inversible dans $E$. De même, $f$ peut se mettre sous la forme $u/v$, où $u, v \in K[(X_i)_{i\in I}]$ et $v((g_i(y)))$ est inversible. Soit $m = \sup(\deg u, \deg v)$. Soient $w = \prod_{i\in I} q_i \in K[(Y_i)_{i\in L}]$, $u_1 = u((g_i)) w^m$, $v_1 = v((g_i)) w^m$.

Le polynôme $u$ est combinaison $K$-linéaire de monômes $\prod_{i\in I} X_i^{v_i}$ tels que $\sum_{i\in I} v_i \leq m$.

On a $w^m \prod_{i\in I} g_i^{v_i} = w^m (\prod_{i\in I} p_i^{v_i}) (\prod_{i\in I} q_i^{v_i})^{-1} \in K[(Y_i)_{i\in L}]$ d’après le choix de $m$. Donc $u_1 \in K[(Y_i)_{i\in L}]$ et de même $v_1 \in K[(Y_i)_{i\in L}]$. De plus, $v_1(y) = (w(y))^m v((g_i(y)))$ est inversible. Donc $v_1 \neq 0$ parce que $E \neq 0$, et par suite $v((g_i)) \neq 0$. La famille $(g_i)$ est donc substituable dans $f$. En outre on a $f((g_i)) = u_1/v_1$, donc $y$ est substituable dans $h = f((g_i))$, et $h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y)))$.

Soient $K$ un corps commutatif, $E$ une $K$-algèbre commutative, associative et unifière. Soit $f \in K((X_i)_{i\in I})$. Soit $T_f$ l’ensemble des $x = (x_i)_{i\in I} \in E^I$ qui sont substituables dans $f$. L’application $x \mapsto f(x)$ de $T_f$ dans $E$ s’appelle la fonction rationnelle associée à $f$ (et à $E$); on la note parfois $\tilde{f}$. Si $g \in K((X_i)_{i\in I})$, on a $T_f \cap T_g \subset T_{f+g}$, $T_f \cap T_g \subset T_{fg}$; la fonction rationnelle associée à $f + g$ (resp. $fg$) est donc définie sur $T_f \cap T_g$, et a même valeur dans cet ensemble que la fonction $\tilde{f} + \tilde{g}$ (resp. $\tilde{f}\tilde{g}$). Soit $T'_f$ l’ensemble des $x \in T_f$ tels que $f(x)$ soit inversible; si $x \in T'_f$, $x$ est substituable dans $1/f$, et la fonction rationnelle associée à $1/f$ prend en $x$ la valeur $f(x)^{-1}$.

Soient $K$ un corps commutatif infini, $f \in K((X_i)_{i\in I})$, $g \in K((X_i)_{i\in I})$ et $\tilde{f}, \tilde{g}$ les fonctions rationnelles associées à $f, g$ (et à $K$). Si l’on a $\tilde{f}(x) = \tilde{g}(x)$ pour tout $x \in T_f \cap T_g$, alors $f = g$. En effet, si $f = u/v$ et $g = u_1/v_1$, où $u, v, u_1, v_1$ sont des polynômes, on a $u(x) v_1(x) = u_1(x) v(x)$ pour tout $x$ tel que $v(x) v_1(x) \neq 0$, donc $uv_1 = u_1 v$ (IV, p. 17, th. 2). Par suite, l’application $f \mapsto \tilde{f}$ est injective, et l’on identifie souvent $f$ et $\tilde{f}$.

\* En utilisant la factorialité de $K[(X_i)_{i\in I}]$ (AC, VII, § 3, no 2 et cor. du th. 2), on montre facilement ceci : pour tout $f \in K((X_i)_{i\in I})$, il existe $u, v \in K[(X_i)_{i\in I}]$ tels que :
    1) $f = u/v$;
    2) pour que $x \in K^I$ soit substituable dans $f$, il faut et il suffit que $v(x) \neq 0$. \*

4. Différentielles et dérivations

Soit $K$ un corps commutatif. D’après III, p. 123, prop. 5, toute dérivation $D$ de $K[(X_i)_{i\in I}]$ se prolonge d’une seule manière en une dérivation $\overline{D}$ de $K((X_i)_{i\in I})$. Si $D, D'$ sont des dérivations permutables de $K[(X_i)_{i\in I}]$, le crochet $[D, D'] = DD' - D'D$ est nul, donc $[\overline{D}, \overline{D'}]$, qui est une dérivation de $K((X_i)_{i\in I})$ prolongeant $[D, D']$, est nul ; autrement dit $\overline{D}$ et $\overline{D}'$ sont permutables. En particulier, les dérivations $D_i$ (IV, p. 6) se prolongent en des dérivations de $K((X_i)_{i \in I})$ qu’on note encore $D_i$ et qui sont deux à deux permutables. Si $f \in K((X_i)_{i \in I})$, $D_i f$ se note aussi $D_{X_i} f$, ou $\frac{\partial f}{\partial X_i}$, ou $f'_{X_i}$. Lorsqu’il n’y a qu’une seule indéterminée $X$, on emploie les notations $Df, \frac{df}{dX}, f'$.

Soient $B = K[(X_i)_{i \in I}]$, $C = K((X_i)_{i \in I})$. D’après III, p. 138, prop. 23, l’application canonique
$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$
est un isomorphisme de $C$-espaces vectoriels. Compte tenu de III, p. 134, le $C$-espace vectoriel $\Omega_K(C)$ admet donc pour base la famille $(dX_i)_{i \in I}$ des différentielles des $X_i$. Soit $\partial_i$ la forme coordonnée d’indice $i$ sur $\Omega_K(C)$, relativement à cette base. Alors l’application $u \mapsto \langle \partial_i, du \rangle$ de $C$ dans $C$ est une dérivation de $C$ qui transforme $X_i$ en 1 et $X_j$ en 0 pour $j \neq i$, donc est égale à $D_i$; autrement dit, on a
$$
du = \sum_{i \in I} (D_i u) \, dX_i
$$
pour tout $u \in C$. Si $I$ est fini, $(D_i)_{i \in I}$ est une base du $C$-espace vectoriel des dérivations de $C$.

#### Proposition 4 {#alg-iv-s3-prop-4 .statement}

*Soient E une K-algèbre associative, commutative et unifère, $x = (x_i)_{i \in I}$ une famille d’éléments de E, et $f \in K((X_i)_{i \in I})$. On suppose que x est substituable dans f. Soit $y = f(x)$.*

(i) *Pour toute dérivation $\Delta$ de $K((X_i)_{i \in I})$ qui applique $K[(X_i)_{i \in I}]$ dans lui-même, x est substituable dans $\Delta f$.*

(ii) *Pour toute dérivation D de E dans un E-module, on a*
$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

Soit $f = \frac{u}{v}$ avec $u, v \in K[(X_i)_{i \in I}]$ et $v(x)$ inversible dans $E$. Soit $\Delta$ une dérivation de $K((X_i)_{i \in I})$ qui applique $K[(X_i)_{i \in I}]$ dans lui-même. On a
$$
\Delta f = \frac{(\Delta u) \, v - u(\Delta v)}{v^2}
$$
et $v^2(x)$ est inversible, donc $x$ est substituable dans $\Delta f$. D’autre part, posons $r = u(x)$, $s = v(x)$. On a $y = s^{-1} r$, donc, pour toute dérivation D de E dans un E-module, on a
$$
Dy = s^{-2} (s(Dr) - r(Ds))
= s^{-2} (s \sum_{i \in I} (D_i u)(x) \cdot Dx_i - r \sum_{i \in I} (D_i v)(x) \cdot Dx_i)
$$

d’après la prop. 4 de IV, p. 6. Ainsi, $D_y = \sum_{i \in I} w_i . D x_i$, avec

$$
w_i = v(x)^{-2}(v(x) (D_i u)(x) - u(x) (D_i v)(x)) = (D_i f)(x)
$$

## EXERCICES {#alg-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
