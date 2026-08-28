---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 7
section_title: Monoïdes libres, groupes libres
lang: fr
source: alg-i-iii-fr
book_pages: A I.77-A I.91, A I.143-A I.151
pdf_pages: 0087-0101, 0153-0161
extraction: ocr
subsections:
    - "no": 1
      title: Magmas libres
      page: 77
      pdf_page: 87
    - "no": 2
      title: Monoïdes libres
      page: 78
      pdf_page: 88
    - "no": 3
      title: Somme amalgamée de monoïdes
      page: 80
      pdf_page: 90
    - "no": 4
      title: Application aux monoïdes libres
      page: 84
      pdf_page: 94
    - "no": 5
      title: Groupes libres
      page: 84
      pdf_page: 94
    - "no": 6
      title: Présentations d’un groupe
      page: 86
      pdf_page: 96
    - "no": 7
      title: Groupes et monoïdes commutatifs libres
      page: 87
      pdf_page: 97
    - "no": 8
      title: Notation exponentielle
      page: 89
      pdf_page: 99
    - "no": 9
      title: Relations entre les divers objets libres
      page: 0
      pdf_page: 100
statements: 18
exercises: 40
content_sha256: 12c52784939bf2fc3c72d9893f11993286f4b2130d14cb070da05f31f5af57bc
---

## § 7. MONOÏDES LIBRES, GROUPES LIBRES

Dans tout ce paragraphe, on note X un ensemble. Sauf mention expresse du contraire, l’élément neutre d’un monoïde se note e.

### 1. Magmas libres

On définit par récurrence sur l’entier $n \geqslant 1$ une suite d’ensembles $M_n(X)$ comme suit : on pose $M_1(X) = X$; pour $n \geqslant 2$, $M_n(X)$ est l’ensemble somme des ensembles $M_p(X) \times M_{n-p}(X)$ pour $1 \leqslant p \leqslant n-1$. L’ensemble somme de la famille $(M_n(X))_{n \geqslant 1}$ est noté $M(X)$; on identifie chacun des ensembles $M_n(X)$ à son image canonique dans $M(X)$. Pour tout élément $w$ de $M(X)$, il existe un unique entier $n$ tel que $w \in M_n(X)$; on l’appelle la longueur de $w$ et on le note $l(w)$. L’ensemble X se compose des éléments de longueur 1 dans $M(X)$.

Soient $w$ et $w'$ dans $M(X)$; posons $p = l(w)$ et $q = l(w')$. L’image de $(w, w')$ par l’injection canonique de $M_p(X) \times M_q(X)$ dans l’ensemble somme $M_{p+q}(X)$ s’appelle le composé de $w$ et $w'$ et se note $ww'$ ou $w.w'$. On a donc $l(w.w') = l(w) + l(w')$ et tout élément de $M(X)$ de longueur $\geqslant 2$ s’écrit de manière unique sous la forme $w'w''$ avec $w', w''$ dans $M(X)$.

On appelle magma libre construit sur X l’ensemble $M(X)$ muni de la loi de composition $(w, w') \mapsto w.w'$ (I, p. 1, déf. 1).

#### Proposition 1 {#alg-i-s7-prop-1 .statement}

Soit $M$ un magma. Toute application $f$ de $X$ dans $M$ se prolonge de manière unique en un morphisme de $M(X)$ dans $M$.

Par récurrence sur $n \geqslant 1$, on définit des applications $f_n : M_n(X) \to M$ comme suit: on pose $f_1 = f$; pour $n \geqslant 2$, l’application $f_n$ est définie par $f_n(w.w') = f_p(w).f_{n-p}(w')$ pour $p = 1, 2, \ldots, n-1$ et $(w, w')$ dans $M_p(X) \times M_{n-p}(X)$. Soit $g$ l’application de $M(X)$ dans $M$ dont la restriction à $M_n(X)$ est $f_n$ pour tout entier $n \geqslant 1$. Il est clair que $g$ est l’unique morphisme de $M(X)$ dans $M$ qui prolonge $f$.

Soit $u$ une application de $X$ dans un ensemble $Y$. D’après la prop. 1, il existe un homomorphisme et un seul de $M(X)$ dans $M(Y)$ qui coïncide avec $u$ sur $X$. On le notera $M(u)$. Si $v$ est une application de $Y$ dans un ensemble $Z$, l’homomorphisme $M(v) \circ M(u)$ de $M(X)$ dans $M(Z)$ coïncide avec $v \circ u$ sur $X$, d’où
$$
M(v) \circ M(u) = M(v \circ u).
$$

#### Proposition 2 {#alg-i-s7-prop-2 .statement}

Soit $u : X \to Y$ une application. Si $u$ est injective (resp. surjective, bijective), il en est de même de $M(u)$.

Supposons $u$ injective. Lorsque $X$ est vide, $M(X)$ est vide, donc $M(u)$ est injective. Si $X$ est non vide, il existe une application $v$ de $Y$ dans $X$ telle que $v \circ u$ soit l’application identique de $X$ (E, II, p. 18, prop. 8); l’application $M(v) \circ M(u) = M(v \circ u)$ est l’application identique de $M(X)$, donc $M(u)$ est injective.

Lorsque $u$ est surjective, il existe une application $w$ de $Y$ dans $X$ telle que $u \circ w$ soit l’application identique de $Y$ (E, II, p. 18, prop. 8). Alors $M(u) \circ M(w) = M(u \circ w)$ est l’application identique de $M(Y)$, donc $M(u)$ est surjective.

Enfin, si $u$ est bijective, elle est injective et surjective, donc $M(u)$ a les mêmes propriétés.

Soit $S$ une partie de $X$. D’après la prop. 2, l’injection de $S$ dans $X$ se prolonge en un isomorphisme de $M(S)$ sur un sous-magma $M'(S)$ de $M(X)$. On identifiera les magmas $M(S)$ et $M'(S)$ au moyen de cet isomorphisme. Alors $M(S)$ est le sous-magma de $M(X)$ engendré par $S$.

Soient $X$ un ensemble, et $(u_\alpha, v_\alpha)_{\alpha \in I}$ une famille de couples d’éléments de $M(X)$. Soit $R$ la relation d’équivalence sur $M(X)$ compatible avec la loi de $M(X)$ et engendrée par les $(u_\alpha, v_\alpha)$ (I, p. 12). Le magma $M(X)/R$ s’appelle le magma défini par $X$ et les relateurs $(u_\alpha, v_\alpha)_{\alpha \in I}$. Soit $h$ le morphisme canonique de $M(X)$ sur $M(X)/R$. Alors $M(X)/R$ est engendré par $h(X)$.

Soient $N$ un magma, et $(n_x)_{x \in X}$ une famille d’éléments de $N$. Soit $k$ le morphisme de $M(X)$ dans $N$ tel que $k(x) = n_x$ pour tout $x \in X$ (prop. 1). Si $k(u_\alpha) = k(v_\alpha)$ pour tout $\alpha \in I$, il existe un morphisme $f : M(X)/R \to N$ et un seul tel que $f(h(x)) = n_x$ pour tout $x \in X$ (I, p. 12, prop. 9).

### 2. Monoïdes libres

On appelle mot construit sur $X$ toute suite finie $w = (x_i)_{1 \leq i \leq n}$ d’éléments de $X$ indexée par un intervalle $\{1, n\}$ de $\mathbf{N}$ (éventuellement vide). L’entier $n$ s’appelle la longueur du mot $w$ est se note $l(w)$. Il y a un unique mot de longueur 0, à savoir la suite vide $e$. On identifiera $X$ à l’ensemble des mots de longueur 1.

Soient $w = (x_i)_{1 \leq i \leq m}$ et $w' = (x'_j)_{1 \leq j \leq n}$ deux mots. On appelle composé de $w$ et $w'$ le mot $u = (y_k)_{1 \leq k \leq m+n}$ défini par

$$
(1) \quad y_k = \begin{cases}
x_k & \text{pour } 1 \leq k \leq m \\
x'_{k-m} & \text{pour } m+1 \leq k \leq m+n.
\end{cases}
$$

Autrement dit, la suite $w''$ s’obtient en écrivant d’abord les éléments de la suite $w$ et ensuite ceux de $w'$. Le composé de $w$ et $w'$ se note en général $ww'$ ou $w.w'$; on dit parfois qu’il s’obtient par juxtaposition de $w$ et $w'$. On a par construction $l(w.w') = l(w) + l(w')$.

On établit immédiatement la relation $we = ew = w$ pour tout mot $w$. Soient $w = (x_i)_{1 \leq i \leq m}$, $w' = (x'_j)_{1 \leq j \leq n}$ et $w'' = (x''_k)_{1 \leq k \leq p}$ trois mots; il est clair que les mots $w(w'w'')$ et $(ww')w''$ sont tous deux égaux au mot $(y_l)_{1 \leq l \leq m+n+p}$ défini par

$$
(2) \quad y_l = \begin{cases}
x_l & \text{si } 1 \leq l \leq m \\
x'_{l-m} & \text{si } m+1 \leq l \leq m+n \\
x''_{l-m-n} & \text{si } m+n+1 \leq l \leq m+n+p.
\end{cases}
$$

Ce qui précède montre que l’ensemble des mots construits sur $X$, muni de la loi de composition $(w, w') \mapsto w.w'$, est un monoïde d’élément neutre $e$. On le note $Mo(X)$ et on l’appelle le monoïde libre construit sur $X$. Il résulte immédiatement de la définition du produit de mots que tout mot $w = (x_i)_{1 \leq i \leq n}$ est égal au produit $\prod_{i=1}^n x_i$. On peut donc écrire un mot sous la forme $x_1 \ldots x_n$.

#### Proposition 3 {#alg-i-s7-prop-3 .statement}

*Soit $M$ un monoïde. Toute application $f$ de $X$ dans $M$ se prolonge de manière unique en un homomorphisme de $Mo(X)$ dans $M$.*

Soit $g$ un homomorphisme de $Mo(X)$ dans $M$ prolongeant $f$. Si $w = (x_i)_{1 \leq i \leq n}$ est un mot, on a $w = \prod_{i=1}^n x_i$ dans le monoïde $Mo(X)$, d’où

$$
g(w) = \prod_{i=1}^n g(x_i) = \prod_{i=1}^n f(x_i)
$$

dans le monoïde $M$ (I, p. 4, formule (2)). Ceci prouve l’unicité de $g$.

Posons $h(w) = \prod_{i=1}^n f(x_i)$ pour tout mot $w = (x_i)_{1 \leq i \leq n}$. Le théorème d’associativité (I, p. 4, th. 1) et la définition du produit dans $Mo(X)$ entraînent $h(ww') = h(w)h(w')$. Par convention, le produit vide $h(e)$ est l’élément neutre de $M$ et l’on a $h(x) = f(x)$ pour $x \in X$. Donc $h$ est un homomorphisme de $Mo(X)$ dans $M$ prolongeant $f$.

Soit $u : X \to Y$ une application. D’après la prop. 3, il existe un homomorphisme et un seul de $Mo(X)$ dans $Mo(Y)$ qui coïncide avec $u$ sur $X$; on le note $Mo(u)$. Il transforme un mot $(x_i)_{1 \leq i \leq n}$ en le mot $(u(x_i))_{1 \leq i \leq n}$. Comme dans le cas des magmas (I, p. 78), on établit la formule $Mo(v \circ u) = Mo(v) \circ Mo(u)$ pour toute application $v : Y \to Z$, et l’on montre que $Mo(u)$ est injective (resp. surjective, bijective) s’il en est ainsi de $u$. Pour toute partie $S$ de $X$, on identifiera $Mo(S)$ au sous-monoïde de $Mo(X)$ engendré par $S$.

Soient $X$ un ensemble, et $(u_\alpha, v_\alpha)_{\alpha \in I}$ une famille de couples d’éléments de $Mo(X)$. Soit $R$ la relation d’équivalence sur $Mo(X)$ compatible avec la loi de $Mo(X)$ et engendrée par les $(u_\alpha, v_\alpha)$ (I, p. 12). Le monoïde $Mo(X)/R$ s’appelle le monoïde défini par $X$ et par les relateurs $(u_\alpha, v_\alpha)_{\alpha \in I}$. Soit $h$ le morphisme canonique de $Mo(X)$ sur $Mo(X)/R$. Alors $Mo(X)/R$ est engendré par $h(X)$.

Soient $N$ un monoïde, et $(n_x)_{x \in X}$ une famille d’éléments de $N$. Soit $k$ le morphisme de $Mo(X)$ dans $N$ tel que $k(x) = n_x$ pour tout $x \in X$ (I, p. 79, prop. 3). Si $k(u_\alpha) = k(v_\alpha)$ pour tout $\alpha \in I$, il existe un morphisme de magmas $f : Mo(X)/R \to N$ et un seul tel que $f(h(x)) = n_x$ pour tout $x \in X$ (I, p. 12, prop. 9); comme $k$ est unifière, $f$ est un morphisme de monoïdes.

### 3. Somme amalgamée de monoïdes

On note $(M_i)_{i \in I}$ une famille de monoïdes et $e_i$ l’élément neutre de $M_i$. On se donne un monoïde $A$ et une famille d’homomorphismes $h_i : A \to M_i$ (pour $i \in I$).

L’ensemble $S$ somme de la famille $(M_i)_{i \in I}$ a pour éléments les couples $(i, x)$ avec $i \in I$ et $x \in M_i$. Pour tout triplet $\alpha = (i, x, x')$ avec $i \in I$, $x, x'$ dans $M_i$, on pose $u_\alpha = (i, xx')$ et $v_\alpha = (i, x).(i, x')$; pour tout triplet $\lambda = (i, j, a)$ dans $I \times I \times A$, on pose $p_\lambda = (i, h_i(a))$ et $q_\lambda = (j, h_j(a))$; pour tout $i \in I$, on pose $\varepsilon_i = (i, e_i)$. Le monoïde $M$ défini par $S$ et les relateurs $(u_\alpha, v_\alpha), (p_\lambda, q_\lambda)$ et $(\varepsilon_i, e)$ est appelé la somme de la famille $(M_i)_{i \in I}$ amalgamée par $A$. On note $\varphi$ l’homomorphisme canonique de $Mo(S)$ sur $M$ et l’on pose $\varphi_i(x) = \varphi(i, x)$ pour $(i, x) \in S$. On dit que $\varphi_i$ est l’application canonique de $M_i$ dans $M$. Pour tout $a \in A$, l’élément $\varphi(i, h_i(a))$ est indépendant de $i$ et se note $h(a)$.\footnote{Lorsque $I$ est vide, on a $M = \{e\}$ et $h(a) = e$ pour tout $a \in A$.}

La propriété universelle des monoïdes définis par générateurs et relateurs (I, p. 80) entraîne le résultat suivant:

#### Proposition 4 {#alg-i-s7-prop-4 .statement}

a) Pour tout $i \in I$, l’application $\varphi_i$ est un homomorphisme de $M_i$ dans $M$ et l’on a $\varphi_i \circ h_i = h$ pour tout $i \in I$. De plus, $M$ est engendré par $\bigcup_{i \in I} \varphi_i(M_i)$.

b) Soient $M'$ un monoïde, et $f_i : M_i \to M'$ (pour $i \in I$) des homomorphismes tels que $f_i \circ h_i$ soit indépendant de $i \in I$. Il existe un homomorphisme $f : M \to M'$ et un seul tel que $f_i = f \circ \varphi_i$ pour tout $i \in I$.

Dans la suite, nous ferons l’hypothèse suivante:

(A) Pour tout $i \in I$, il existe une partie $P_i$ de $M_i$ contenant $e_i$, telle que l’application $(a, p) \mapsto h_i(a).p$ de $A \times P_i$ dans $M_i$ soit bijective.

Elle entraîne que les homomorphismes $h_i$ sont injectifs. Soit $x \in M$; on appelle décomposition de $x$ toute suite finie $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ avec $a \in A$, $i_\alpha \in I$ et $p_\alpha \in P_{i_\alpha}$ pour $1 \leq \alpha \leq n$, satisfaisant à

$$
x = h(a) \cdot \prod_{\alpha=1}^n \varphi_{i_\alpha}(p_\alpha).
$$

L’entier $n \geq 0$ s’appelle la longueur de la décomposition $\sigma$ et se note $l(\sigma)$; la suite $(e)$ est une décomposition de longueur 0 de l’élément neutre de $M$. On dit que la décomposition $\sigma$ est réduite si l’on a $i_\alpha \neq i_{\alpha+1}$ pour $1 \leq \alpha < n$ et $p_\alpha \neq e_{i_\alpha}$ pour $1 \leq \alpha \leq n$.

#### Proposition 5 {#alg-i-s7-prop-5 .statement}

Sous l’hypothèse (A), tout élément $x$ de $M$ admet une décomposition réduite unique $\sigma$. Toute décomposition $\sigma' \neq \sigma$ de $x$ satisfait à $l(\sigma') > l(\sigma)$.

A) Unicité d’une décomposition réduite :

Notons $\Sigma$ l’ensemble des suites $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ avec $n \geq 0$, $a \in A$, $i_\alpha \in I$ et $p_\alpha \in P_{i_\alpha} - \{e_{i_\alpha}\}$ pour $1 \leq \alpha \leq n$, telles que $i_\alpha \neq i_{\alpha+1}$ pour $1 \leq \alpha < n$. On note $\Phi$ l’application de $\Sigma$ dans $M$ définie par

$$
\Phi(a; i_1, \ldots, i_n; p_1, \ldots, p_n) = h(a) \cdot \prod_{\alpha=1}^n \varphi_{i_\alpha}(p_\alpha).
$$

Une décomposition réduite de $x \in M$ est un élément $\sigma$ de $\Sigma$ tel que $\Phi(\sigma) = x$.

Pour tout $i \in I$, soit $\Sigma_i$ le sous-ensemble de $\Sigma$ formé des suites $(e; i_1, \ldots, i_n; p_1, \ldots, p_n)$ avec $i \neq i_1$ lorsque $n > 0$. Soient

$$
\sigma = (e; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$

dans $\Sigma_i$ et $\xi$ dans $M_i$; posons $\xi = h_i(a) \cdot p$ avec $a \in A$ et $p \in P_i$, et

$$
\Psi_i(\xi, \sigma) = \begin{cases}
(a; i_1, \ldots, i_n; p_1, \ldots, p_n) & \text{si } p = e_i \\
(a; i, i_1, \ldots, i_n; p, p_1, \ldots, p_n) & \text{si } p \neq e_i.
\end{cases}
$$

Il est immédiat que $\Psi_i$ est une bijection de $M_i \times \Sigma_i$ sur $\Sigma$.

Soient $i \in I$ et $x \in M_i$; comme $\Psi_i$ est bijective, on définit une application $f_{i, x}$ de $\Sigma$ dans lui-même par

$$
f_{i, x}(\Psi_i(\xi, \sigma)) = \Psi_i(x\xi, \sigma) \quad (\xi \in M_i, \sigma \in \Sigma_i).
$$

De plus, pour $a \in A$, on note $f_a$ l’application de $\Sigma$ dans lui-même définie par

$$
f_a(a'; i_1, \ldots, i_n; p_1, \ldots, p_n) = (aa'; i_1, \ldots, i_n; p_1, \ldots, p_n).
$$

Il est clair que $f_{i, e_i}$ est l’application identique de $\Sigma$ et que l’on a $f_{i, xx'} = f_{i, x} \circ f_{i, x'}$ pour $x, x'$ dans $M_i$ et $f_{i, h_i(a)} = f_a$ pour $a \in A$ et $i \in I$.

On peut alors appliquer la prop. 4 (I, p. 80) au cas où $M'$ est le monoïde des applications de $\Sigma$ dans lui-même, avec la loi de composition $(f, f') \mapsto f \circ f'$, et où $f_i$ est l’homomorphisme $x \mapsto f_{i,x}$ de $M_i$ dans $M'$; il existe donc un homomorphisme $f$ de $M$ dans $M'$ tel que $f_{i,x} = f(\varphi_i(x))$ pour $i \in I$ et $x \in M_i$. Soit
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
dans $\Sigma$. Les formules (5) à (7) entraînent par récurrence sur $n$ la relation
$$
\begin{align*}
\sigma &= (f_a \circ f_{i_1, p_1} \circ \cdots \circ f_{i_n, p_n})(e) \\
&= f(h(a)\varphi_{i_1}(p_1) \cdots \varphi_{i_n}(p_n))(e),
\end{align*}
$$
c’est-à-dire $\sigma = f(\Phi(\sigma))(e)$. Ceci prouve que $\Phi$ est injective.

B) *Existence d’une décomposition*:
Soit D l’ensemble des éléments de M admettant une décomposition. On a $e \in D$ et $M$ est engendré par $\bigcup_{i \in I} \varphi_i(M_i)$, donc par $h(A) \cup \bigcup_{i \in I} \varphi_i(P_i)$. On a $D . \varphi_i(P_i) \subset D$ pour tout $i \in I$; pour prouver que l’on a $D = M$, il suffit donc de prouver la relation $D . h(A) \subset D$. Ceci résulte du lemme plus précis suivant :

#### Lemme 1 {#alg-i-s7-lem-1 .statement}

*Soient $i_1, \ldots, i_n$ dans $I$ et $p_\alpha$ dans $P_{i_\alpha}$ pour $1 \leq \alpha \leq n$. Pour tout $a \in A$, il existe $a' \in A$ et une suite $(p'_\alpha)_{1 \leq \alpha \leq n}$ avec $p'_\alpha \in P_{i_\alpha}$ telle que*
$$
\varphi_{i_1}(p_1) \cdots \varphi_{i_n}(p_n)h(a) = h(a')\varphi_{i_1}(p'_1) \cdots \varphi_{i_n}(p'_n).
$$
On a $h(a) = \varphi_{i_n}(h_{i_n}(a))$ et il existe $a_n \in A$ et $p'_n \in P_{i_n}$ tels que $p_n . h_{i_n}(a) = h_{i_n}(a_n) . p'_n$. On en déduit $\varphi_{i_n}(p_n)h(a) = h(a_n)\varphi_{i_n}(p'_n)$, d’où
$$
\varphi_{i_1}(p_1) \cdots \varphi_{i_{n-1}}(p_{n-1})\varphi_{i_n}(p_n)h(a) = \varphi_{i_1}(p_1) \cdots \varphi_{i_{n-1}}(p_{n-1})h(a_n)\varphi_{i_n}(p'_n);
$$
le lemme résulte de là par récurrence sur $n$.

C) *Fin de la démonstration*:
Soit $x \in M$ et soit $n$ le minimum des longueurs des décompositions de $x$. Nous allons prouver que toute décomposition $\sigma$ de $x$ de longueur $n$ est réduite. Ceci établira l’existence d’une décomposition réduite de $x$; l’unicité de la décomposition réduite entraîne alors $l(\sigma') > l(\sigma)$ pour toute décomposition $\sigma' \neq \sigma$ de $x$.

Le cas $n = 0$ étant trivial, supposons $n > 0$. Soit $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ une décomposition de $x$ de longueur $n$. S’il existait un entier $\alpha$ avec $1 \leq \alpha \leq n$ et $p_\alpha = e_{i_\alpha}$, la suite $(a; i_1, \ldots, i_{\alpha-1}, i_{\alpha+1}, \ldots, i_n; p_1, \ldots, p_{\alpha-1}, p_{\alpha+1}, \ldots, p_n)$ serait une décomposition de $x$ de longueur $n - 1$, ce qui est exclus. Supposons qu’il existe un entier $\alpha$ avec $1 \leq \alpha < n$ et $i_\alpha = i_{\alpha+1}$, et posons $p_\alpha p_{\alpha+1} = h_{i_\alpha}(a') . p'_\alpha$ avec $a' \in A$ et $p'_\alpha \in P_{i_\alpha}$; d’après le lemme 1, il existe des éléments $a'' \in A$, $p'_1 \in P_{i_1}, \ldots, p'_{\alpha-1} \in P_{i_{\alpha-1}}$ tels que
$$
\varphi_{i_1}(p_1) \cdots \varphi_{i_{\alpha-1}}(p_{\alpha-1})h(a') = h(a'')\varphi_{i_1}(p'_1) \cdots \varphi_{i_{\alpha-1}}(p'_{\alpha-1})
$$
et la suite
$$
(aa''; i_1, \ldots, i_{\alpha-1}, i_\alpha, i_{\alpha+2}, \ldots, i_n; p'_1, \ldots, p'_{\alpha-1}, p'_\alpha, p_{\alpha+2}, \ldots, p_n)
$$

est une décomposition de $x$ de longueur $n - 1$, ce qui est contradictoire.

On a bien prouvé que $\sigma$ est réduite. C. Q. F. D.

#### Corollaire {#alg-i-s7-n3-cor-1 .statement}

Sous l’hypothèse (A), les homomorphismes $\varphi_i$ et $h$ sont injectifs. Pour $i \neq j$ dans $I$, on a $\varphi_i(M_i) \cap \varphi_j(M_j) = h(A)$.

Tout d’abord $h$ est injectif: si $h(a) = h(a')$, alors $(a)$ et $(a')$ sont deux décompositions réduites d’un même élément de $M$, d’où $a = a'$. Soit $i \in I$; on a $h(A) = \varphi_i(h_i(A)) \subset \varphi_i(M_i)$; l’unicité des décompositions réduites entraîne

$$
h(A) \cap \varphi_i(M_i - h_i(A)) = \varnothing
$$

d’où $\varphi_i(M_i - h_i(A)) = \varphi_i(M_i) - h(A)$.

L’injectivité des homomorphismes $\varphi_i$ et la relation $\varphi_i(M_i) \cap \varphi_j(M_j) \subset h(A)$ pour $i \neq j$ sont alors conséquences du fait suivant: pour $i, j$ dans $I$, $x$ dans $M_i - h_i(A)$ et $y$ dans $M_j - h_j(A)$, la relation $\varphi_i(x) = \varphi_j(y)$ entraîne $i = j$ et $x = y$. En effet, posons $x = h_i(a) . p$ et $y = h_j(b) . q$ avec $a, b$ dans $A$, $p$ dans $P_i - \{ e_i \}$ et $y$ dans $P_j - \{ e_j \}$. On a $\varphi_i(x) = h(a) \varphi_i(p)$ et $\varphi_j(y) = h(b) \varphi_j(q)$, donc $(a; i; p)$ et $(b; j; q)$ sont deux décompositions réduites d’un même élément de $M$. On en déduit $i = j$, $a = b$ et $p = q$, d’où $x = h_i(a)p = h_j(b)q = y$.

C. Q. F. D.

Lorsque l’hypothèse (A) est remplie, nous identifierons chaque monoïde $M_i$ à un sous-monoïde de $M$ au moyen de $\varphi_i$; de même, nous identifierons $A$ à un sous-monoïde de $M$ par $h$. Alors $M$ est engendré par $\bigcup_{i \in I} M_i$ et l’on a $M_i \cap M_j = A$ pour $i \neq j$. Tout élément de $M$ s’écrit de manière unique sous la forme $a . \prod_{\alpha=1}^n p_\alpha$ avec $a \in A$, $p_1 \in P_{i_1} - \{ e \}$, $\ldots$, $p_n \in P_{i_n} - \{ e \}$ et $i_\alpha \neq i_{\alpha+1}$ pour $1 \leq \alpha < n$. Enfin, si $M'$ est un monoïde et $(f_i : M_i \to M')$ (pour $i \in I$) une famille d’homomorphismes dont les restrictions à $A$ sont toutes un même homomorphisme de $A$ dans $M'$, il existe un’homomorphisme $f : M \to M'$ et un seul dont la restriction à $M_i$ est $f_i$ pour tout $i \in I$.

L’hypothèse (A) est vérifiée dans deux cas importants:

a) On a $A = \{ e \}$. Dans ce cas, on a une famille $(M_i)_{i \in I}$ de monoïdes et $M$ s’appelle la somme monoïdale de cette famille. Chaque $M_i$ est identifié à un sous-monoïde de $M$, et $M$ est engendré par $\bigcup_{i \in I} M_i$; de plus, on a $M_i \cap M_j = \{ e \}$ pour $i \neq j$. Tout élément de $M$ s’écrit de manière unique sous la forme $x_1 \ldots x_n$ avec $x_1 \in M_{i_1} - \{ e \}$, $\ldots$, $x_n \in M_{i_n} - \{ e \}$ et $i_\alpha \neq i_{\alpha+1}$ pour $1 \leq \alpha < n$. Enfin, pour toute famille d’homomorphismes $(f_i : M_i \to M')$, il existe un homomorphisme unique $f : M \to M'$ dont la restriction à $M_i$ est $f_i$ pour tout $i \in I$.

b) On a une famille de groupes $(G_i)_{i \in I}$ contenant comme sous-groupe un même groupe $A$ et $h_i$ est l’injection de $A$ dans $G_i$. La somme de la famille $(G_i)_{i \in I}$ amalgamée par $A$ est alors un groupe $G$: en effet, le monoïde $G$ est engendré par $\bigcup_{i \in I} \varphi_i(G_i)$ et tout élément de $\bigcup_{i \in I} \varphi_i(G_i)$ admet un inverse dans $G$ (cf. I, p. 16, cor. 1); on le note $*_A G_i$ ou $G_1 *_A G_2$ lorsque $I = \{1, 2\}$. Lorsque $A$ est réduit à l’élément neutre, on dit aussi que $G$ est le produit libre de la famille $(G_i)_{i \in I}$ de groupes, et on le note $* G_i$ (ou $G_1 * G_2$ lorsque $I = \{1, 2\}$).¹

### 4. Application aux monoïdes libres

#### Lemme 2 {#alg-i-s7-lem-2 .statement}

Soit $M$ la somme monoïdale de la famille $(M_x)_{x \in X}$ définie par $M_x = \mathbf{N}$ pour tout $x \in X$; on note $\varphi_x$ l’homomorphisme canonique de $M_x$ dans $M$. L’application $x \mapsto \varphi_x(1)$ de $X$ dans $M$ se prolonge en un isomorphisme $h$ de $Mo(X)$ sur $M$.

Soit $h$ l’homomorphisme de $Mo(X)$ dans $M$ caractérisé par $h(x) = \varphi_x(1)$. Pour tout entier $n \geq 0$, on a $\varphi_x(n) = \varphi_x(1)^n = h(x)^n$ et comme $M$ est engendré par $\bigcup_{x \in X} \varphi_x(\mathbf{N})$, il est aussi engendré par $h(X)$. Donc $h$ est surjectif. Par ailleurs, pour tout $x$ dans $X$, l’application $n \mapsto x^n$ est un homomorphisme de $\mathbf{N} = M_x$ dans $Mo(X)$; il existe donc (I, p. 80, prop. 4) un homomorphisme $h'$ de $M$ dans $Mo(X)$ tel que $h'(\varphi_x(n)) = x^n$ pour $x \in X$ et $n \in \mathbf{N}$; en particulier, on a $h'(h(x)) = x$ pour $x \in X$, donc $h' \circ h$ est l’homomorphisme identique de $Mo(X)$. Par suite, $h$ est injectif. On a donc prouvé que $h$ est bijectif.

#### Proposition 6 {#alg-i-s7-prop-6 .statement}

Soit $w$ un élément de $Mo(X)$.

a) Il existe un entier $n \geq 0$, des éléments $x_\alpha$ de $X$ et des entiers $m(\alpha) > 0$ (pour $1 \leq \alpha \leq n$) tels que $x_\alpha \neq x_{\alpha+1}$ pour $1 \leq \alpha < n$ et $w = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$. La suite $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ est déterminée de manière unique par ces conditions.

b) Soient $p$ un entier positif, $x'_\beta$ dans $X$ et $m'(\beta)$ dans $\mathbf{N}$ pour $1 \leq \beta \leq p$, tels que $w = \prod_{\beta=1}^p x'_\beta^{m'(\beta)}$. On a $p \geq n$. Si $p = n$, on a $x'_\beta = x_\beta$ et $m'(\beta) = m(\beta)$ pour $1 \leq \beta \leq p$.

Avec les notations du lemme 2, on a $h^{-1}(\varphi_x(n)) = x^n$ pour $x \in X$ et $n \in \mathbf{N}$. La prop. 6 résulte alors de I, p. 81, prop. 5.

### 5. Groupes libres

Posons $G_x = \mathbf{Z}$ pour tout $x \in X$. Le produit libre de la famille $(G_x)_{x \in X}$ s’appelle le groupe libre construit sur $X$ et se note $F(X)$. Notons $\varphi_x$ l’homomorphisme canonique de $G_x = \mathbf{Z}$ dans $F(X)$. D’après I, p. 83, corollaire, l’application $x \mapsto \varphi_x(1)$ de $X$ dans $F(X)$ est injective; nous identifierons $X$ à son image dans $F(X)$ par cette application. Alors $X$ engendre $F(X)$ et l’on a $e \notin X$.

Par application de I, p. 81, prop. 5, on obtient le résultat suivant:

#### Proposition 7 {#alg-i-s7-prop-7 .statement}

Soit $g$ un élément du groupe libre $F(X)$. Il existe un entier $n \geq 0$, et une suite $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$, déterminés de manière unique par les relations $x_\alpha \in X$, $x_\alpha \neq x_{\alpha+1}$ pour $1 \leq \alpha < n$, $m(\alpha) \in \mathbf{Z}$, $m(\alpha) \neq 0$ pour $1 \leq \alpha \leq n$ et $g = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$.

¹ On notera que $G_1 * G_2$ n’est pas « produit » de $G_1$ et $G_2$ au sens de E, IV, p. 16 (ni au sens de la « théorie des catégories »; dans le cadre de cette théorie, $G_1 * G_2$ est la « somme » de $G_1$ et $G_2$).

Le groupe libre F(X) jouit de la propriété universelle suivante:

#### Proposition 8 {#alg-i-s7-prop-8 .statement}

Soient G un groupe et f une application de X dans G. Il existe un homomorphisme $\tilde{f}$ de F(X) dans G qui prolonge f, et un seul.

L’unicité de $\tilde{f}$ résulte du fait que le groupe F(X) est engendré par X. Pour tout x dans X, soit $f_x$ l’homomorphisme $n \mapsto f(x)^n$ de $\mathbf{Z}$ dans G. D’après I, p. 80, prop. 4, il existe un homomorphisme $\tilde{f}$ de F(X) dans G tel que $\tilde{f}(x^n) = f_x(n)$ pour $x \in X$ et $n \in \mathbf{Z}$; en particulier, on a $\tilde{f}(x) = f_x(1) = f(x)$ pour tout $x \in X$, donc $\tilde{f}$ prolonge f.

Soit $u : X \to Y$ une application. D’après la prop. 8, il existe un homomorphisme et un seul de F(X) dans F(Y) qui coïncide avec u sur X; on le note F(u). Comme dans le cas des magmas (I, p. 78) on établit la formule $F(v \circ u) = F(v) \circ F(u)$ pour toute application $v : Y \to Z$, et l’on montre que F(u) est injectif (resp. surjectif, bijectif) s’il en est ainsi de u. Pour toute partie S de X, on identifiera F(S) au sous-groupe de F(X) engendré par S.

Soit I un ensemble. Dans certains cas, on a intérêt à ne pas identifier un élément i de I à son image canonique $\varphi_i(1)$ dans le groupe libre F(I); cette dernière pourra être notée $T_i$ (ou $T'_i$, $X_i$, ... selon les cas) et s’appelle l’indéterminée d’indice i. Le groupe libre F(I) se note alors $F((T_i)_{i \in I})$ ou $F(T_1, \ldots, T_n)$ si $I = \{1, 2, \ldots, n\}$.

Soient G un groupe et $t = (t_i)_{i \in I}$ une famille d’éléments de G. D’après la prop. 8, il existe un homomorphisme $f_t$ de $F((T_i)_{i \in I})$ dans G caractérisé par $f_t(T_i) = t_i$ pour tout $i \in I$. L’image d’un élément $w$ de $F((T_i)_{i \in I})$ par $f_t$ sera notée $w(t)$ ou $w(t_1, \ldots, t_n)$ si $I = \{1, 2, \ldots, n\}$; on dit que $w(t)$ résulte de la substitution $T_i \mapsto t_i$ dans $w$. En particulier, si l’on prend $G = F((T_i)_{i \in I})$ et $(t_i) = (T_i) = T$, $f_T$ est l’homomorphisme identique de G, d’où $w(T) = w$; pour $I = \{1, 2, \ldots, n\}$, on a donc $w(T_1, \ldots, T_n) = w$.

Soient G et G’ deux groupes, u un homomorphisme de G dans G’ et $t = (t_1, \ldots, t_n)$ une suite finie d’éléments de G. Posons $t' = (u(t_1), \ldots, u(t_n))$; l’homomorphisme $u \circ f_t$ de $F(T_1, \ldots, T_n)$ dans G’ transforme $T_i$ en $u(t_i)$ pour $1 \leq i \leq n$, donc est égal à $f_{t'}$; pour $w$ dans $F(T_1, \ldots, T_n)$, on a donc

$$
u(w(t_1, \ldots, t_n)) = w(u(t_1), \ldots, u(t_n)).
$$

Soient donnés $w$ dans $F(T_1, \ldots, T_n)$ et des éléments $v_1, \ldots, v_n$ du groupe libre $F(T'_1, \ldots, T'_m)$. La substitution $T_i \mapsto v_i$ définit un élément $w' = w(v_1, \ldots, v_n)$ de $F(T'_1, \ldots, T'_m)$. Soient G un groupe, $t_1, \ldots, t_m$ des éléments de G et u l’homomorphisme de $F(T'_1, \ldots, T'_m)$ dans G caractérisé par $u(T'_j) = t_j$ pour $1 \leq j \leq m$. On a $u(v_i) = v_i(t_1, \ldots, t_m)$ et $u(w') = w'(t_1, \ldots, t_m)$; la formule (8) entraîne donc

$$
w'(t_1, \ldots, t_m) = w(v_1(t_1, \ldots, t_m), \ldots, v_n(t_1, \ldots, t_m)).
$$

Ceci justifie la « notation fonctionnelle » $w(t_1, \ldots, t_n)$. On laisse au lecteur le soin d’étendre les formules (8) et (9) au cas d’ensembles d’indices arbitraires.

### 6. Présentations d’un groupe

Soient G un groupe et $\mathbf{t} = (t_i)_{i \in I}$ une famille d’éléments de G. Soit $f_t$ l’unique homomorphisme du groupe libre F(I) dans G qui applique i sur $t_i$. L’image de $f_t$ est le sous-groupe engendré par les éléments $t_i$ de G. Les éléments du noyau de $f_t$ s’appellent les *relateurs* de la famille $\mathbf{t}$. On dit que $\mathbf{t}$ est *génératrice* (resp. *libre*, *basique*) si $f_t$ est surjectif (resp. injectif, bijectif).

Soit G un groupe. Une *présentation* de G est un couple $(\mathbf{t}, \mathbf{r})$ formé d’une famille génératrice $\mathbf{t} = (t_i)_{i \in I}$ et d’une famille $\mathbf{r} = (r_j)_{j \in J}$ de relateurs telles que le noyau $N_t$ de $f_t$ soit engendré par les éléments $gr_j g^{-1}$ pour $g \in F(I)$ et $j \in J$. Il revient au même de dire que $N_t$ est le sous-groupe distingué de F(I) engendré par les $r_j$ pour $j \in J$ (autrement dit le plus petit sous-groupe distingué de F(I) contenant les éléments $r_j$ ($j \in J$); cf. I, p. 36). Par abus de langage, on dit que les générateurs $t_i$ et les relations $r_j(\mathbf{t}) = e$ constituent une présentation du groupe G.

Soient I un ensemble et $\mathbf{r} = (r_j)_{j \in J}$ une famille d’éléments du groupe libre F(I). Soit $N(\mathbf{r})$ le sous-groupe distingué de F(I) engendré par les $r_j$ pour $j \in J$. On pose $F(I, \mathbf{r}) = F(I)/N(\mathbf{r})$ et l’on note $\tau_i$ la classe de i modulo $N(\mathbf{r})$. Le couple $(\tau, \mathbf{r})$ avec $\tau = (\tau_i)_{i \in I}$ est une présentation du groupe $F(I, \mathbf{r})$; si G est un groupe et $(\mathbf{t}, \mathbf{r})$ est une présentation de G avec $\mathbf{t} = (t_i)_{i \in I}$, il existe un isomorphisme unique u de $F(I, \mathbf{r})$ sur G tel que $u(\tau_i) = t_i$ pour tout $i \in I$. On dit que le groupe $F(I, \mathbf{r})$ est défini par les générateurs $\tau_i$ et les relateurs $r_j$, ou par abus de langage qu’il est *défini par les générateurs $\tau_i$ et les relations $r_j(\tau) = e$*. Lorsque $I = \{1, n\}$ et $J = \{1, m\}$, on dit que $F(I, \mathbf{r})$ est défini par la présentation $\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle$. Si $r_j = u_j^{-1} v_j$ avec $u_j$ et $v_j$ dans F(I), cette présentation se note également par le symbole

$$
\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle.
$$

#### Exemple 1 {#alg-i-s7-n6-exa-1 .statement}

Le groupe défini par la présentation $\langle \tau; \tau^q = e \rangle$ est cyclique d’ordre q.

#### Exemple 2 {#alg-i-s7-n6-exa-2 .statement}

Le groupe défini par la présentation $\langle x, y; xy = yx \rangle$ est isomorphe à $\mathbf{Z} \times \mathbf{Z}$.

#### Proposition 9 {#alg-i-s7-prop-9 .statement}

*Soient G un groupe, $\mathbf{t} = (t_i)_{i \in I}$ une famille génératrice de G et $\mathbf{r} = (r_j)_{j \in J}$ une famille de relateurs de $\mathbf{t}$. Les conditions suivantes sont équivalentes*:

a) *Le couple $(\mathbf{t}, \mathbf{r})$ est une présentation de G*.

b) *Soient G’ un groupe et $\mathbf{t}' = (t'_i)_{i \in I}$ une famille d’éléments de G’. Si l’on a $r_j(\mathbf{t}') = e$ pour tout $j \in J$, il existe un homomorphisme u de G dans G’ tel que $u(t_i) = t'_i$ pour tout $i \in I$*.

c) *Soient $\overline{G}$ un groupe et $\overline{\mathbf{t}} = (\overline{t}_i)_{i \in I}$ une famille génératrice de $\overline{G}$ telle que $r_j(\overline{\mathbf{t}}) = e$* pour tout $j \in J$. Tout homomorphisme de $\overline{G}$ dans $G$ qui applique $\bar{t}_i$ sur $t_i$ pour tout $i \in I$ est un isomorphisme.

On note $f$ l’homomorphisme de $F(I)$ dans $G$ qui applique $i$ sur $t_i$ pour tout $i \in I$, et $N$ le noyau de $f$.

a) $\Rightarrow$ b) : Supposons que $(\mathbf{t}, \mathbf{r})$ soit une présentation de $G$, et soit $\mathbf{t}' = (t'_i)_{i \in I}$ une famille d’éléments d’un groupe $G'$ avec $r_j(\mathbf{t}') = e$ pour tout $j \in J$. Soit $f'$ l’homomorphisme de $F(I)$ dans $G'$ caractérisé par $f'(i) = t'_i$ pour tout $i \in I$. Par hypothèse $f'(r_j) = e$ pour tout $j \in J$, et comme $N$ est engendré par les éléments $gr_jg^{-1}$ pour $j \in J$ et $g \in F(I)$, on a $f'(N) = \{e\}$. Comme l’homomorphisme $f : F(I) \to G$ est surjectif de noyau $N$, il existe un homomorphisme $u : G \to G'$ tel que $f' = u \circ f$. On a $u(t_i) = u(f(i)) = f'(i) = t'_i$.

b) $\Rightarrow$ c) : Supposons la condition b) vérifiée. Soit $\mathbf{t} = (t_i)_{i \in I}$ une famille génératrice d’un groupe $G$, telle que $r_j(\mathbf{t}) = e$ pour tout $j \in J$, et soit $v$ un homomorphisme de $\overline{G}$ dans $G$ tel que $v(\bar{t}_i) = t_i$ pour tout $i \in I$. Comme la famille $(t_i)_{i \in I}$ engendre $G$, l’homomorphisme $v$ est surjectif. D’après la propriété b), il existe un homomorphisme $u : G \to \overline{G}$ tel que $u(t_i) = \bar{t}_i$ pour tout $i \in I$. On a $u(v(\bar{t}_i)) = \bar{t}_i$ pour tout $i \in I$, donc $u \circ v$ est l’identité sur $\overline{G}$, ce qui prouve que $v$ est injectif. Donc $v$ est un isomorphisme, et la condition c) est vérifiée.

c) $\Rightarrow$ a) : Supposons la condition c) vérifiée. Soit $t'_i$ l’image canonique de $i$ dans $F(I, \mathbf{r})$ et $\mathbf{t}' = (t'_i)_{i \in I}$; on a donc $r_j(\mathbf{t}') = e$ pour tout $j \in J$. Comme on a $r_j(\mathbf{t}) = e$ pour tout $j \in J$, il existe un homomorphisme $v$ et un seul de $F(I, \mathbf{r})$ dans $G$ tel que $v(\bar{t}_i) = t_i$ pour tout $i \in I$. D’après c), $v$ est un isomorphisme de $F(I, \mathbf{r})$ sur $G$ qui transforme la présentation $(\mathbf{t}', \mathbf{r})$ de $F(I, \mathbf{r})$ en une présentation $(\mathbf{t}, \mathbf{r})$ de $G$.

### 7. Groupes et monoïdes commutatifs libres

L’ensemble $\mathbf{Z}^X$ de toutes les applications de $X$ dans $\mathbf{Z}$ est un groupe commutatif pour la loi définie par $(\alpha + \beta)(x) = \alpha(x) + \beta(x)$ ($\alpha, \beta$ dans $\mathbf{Z}^X, x \in X$); les éléments de $\mathbf{Z}^X$ sont parfois appelés multiindices. L’élément neutre, noté $0$, est l’application constante de valeur $0$. Pour $\alpha \in \mathbf{Z}^X$ on appelle support de $\alpha$ l’ensemble $S_\alpha$ des $x \in X$ tels que $\alpha(x) \neq 0$; on a $S_0 = \varnothing$ et $S_{\alpha + \beta} \subset S_\alpha \cup S_\beta$ pour $\alpha, \beta$ dans $\mathbf{Z}^X$. Par suite, l’ensemble $\mathbf{Z}^{(X)}$ des applications $\alpha : X \to \mathbf{Z}$ de support fini est un sous-groupe de $\mathbf{Z}^X$ qu’on appelle groupe commutatif libre construit sur $X$.

Pour tout $x \in X$, on note $\delta_x$ l’élément de $\mathbf{Z}^{(X)}$ défini par

$$
\delta_x(y) = \begin{cases}
1 & \text{si } y = x \\
0 & \text{si } y \neq x.
\end{cases}
$$

Par ailleurs, pour $\alpha \in \mathbf{Z}^{(X)}$, on définit l’entier $|\alpha|$, longueur de $\alpha$, par la formule

$$
|\alpha| = \sum_{x \in X} \alpha(x).
$$

On établit immédiatement les relations

(12) $$
\alpha = \sum_{x \in X} \alpha(x) \cdot \delta_x
$$
(13) $$
|\delta_x| = 1, \quad |0| = 0
$$
(14) $$
|\alpha + \beta| = |\alpha| + |\beta|
$$
pour $\alpha, \beta$ dans $\mathbf{Z}^{(X)}$ et $x$ dans $X$.

La relation d’ordre $\alpha \leq \beta$ est définie dans $\mathbf{Z}^{(X)}$ par $\alpha(x) \leq \beta(x)$ pour tout $x \in X$. Les relations $\alpha \leq \beta$ et $\alpha' \leq \beta'$ entraînent $\alpha + \alpha' \leq \beta + \beta'$, $|\alpha| \leq |\beta|$ et $-\alpha \geq -\beta$; de plus, la relation $\alpha \leq \beta$ équivaut à $\beta - \alpha \geq 0$. L’ensemble des éléments $\alpha \geq 0$ de $\mathbf{Z}^{(X)}$ se note $\mathbf{N}^{(X)}$; c’est l’ensemble des applications de $X$ dans $\mathbf{N}$ de support fini, et c’est un sous-monoïde de $\mathbf{Z}^{(X)}$ qu’on appelle le monoïde commutatif libre construit sur $X$. Les éléments de longueur 1 sont les éléments minimaux dans $\mathbf{N}^{(X)} - \{0\}$ et constituent l’ensemble des $\delta_x$ ($x \in X$).

Le monoïde $\mathbf{N}^{(X)}$ et le groupe $\mathbf{Z}^{(X)}$ jouissent de la propriété universelle suivante.

#### Proposition 10 {#alg-i-s7-prop-10 .statement}

*Soient M un monoïde (resp. un groupe) commutatif et f une application de X dans M. Il existe un homomorphisme g de $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$) dans M, et un seul, tel que $g(\delta_x) = f(x)$ pour tout $x \in X$. Si M est noté additivement, on a $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$ pour tout $\alpha$ dans $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$).*

Soit $g$ un homomorphisme de $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$) dans $M$ tel que $g(\delta_x) = f(x)$ pour tout $x \in X$. Pour tout $\alpha$ dans $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$), on déduit de (12) la formule
$$
g(\alpha) = \sum_{x \in X} \alpha(x) \cdot g(\delta_x) = \sum_{x \in X} \alpha(x) \cdot f(x),
$$
d’où l’unicité de $g$.

Pour tout $\alpha$ dans $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$), posons $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$. On a évidemment $g(0) = 0$; pour $\alpha, \beta$ dans $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$), on a
$$
g(\alpha + \beta) = \sum_{x \in X} (\alpha(x) + \beta(x)) \cdot f(x)
$$
$$
= \sum_{x \in X} (\alpha(x) \cdot f(x) + \beta(x) \cdot f(x))
$$
$$
= \sum_{x \in X} \alpha(x) \cdot f(x) + \sum_{x \in X} \beta(x) \cdot f(x)
$$
$$
= g(\alpha) + g(\beta)
$$
donc $g$ est un homomorphisme de $\mathbf{N}^{(X)}$ (resp. $\mathbf{Z}^{(X)}$) dans $M$. Par ailleurs, pour $y$ dans $X$, on a
$$
g(\delta_y) = \sum_{x \in X} \delta_y(x) \cdot f(x);
$$
on a $\delta_y(x) \cdot f(x) = 0$ pour $x \neq y$ et $\delta_y(y) \cdot f(y) = f(y)$ d’où $g(\delta_y) = f(y)$.

Soit $u : X \to Y$ une application. D’après la prop. 10, il existe un homomorphisme et un seul de $\mathbf{Z}^{(X)}$ dans $\mathbf{Z}^{(Y)}$ qui applique $\delta_x$ sur $\delta_{u(x)}$ pour tout $x \in X$. On le note $\mathbf{Z}^{(u)}$; on voit immédiatement qu’il transforme $\alpha \in \mathbf{Z}^{(X)}$ en l’élément $\beta \in \mathbf{Z}^{(Y)}$ défini par

$$
\beta(y) = \sum_{x \in u^{-1}(y)} \alpha(x).
$$

Comme dans le cas des magmas (I, p. 78), on établit la formule $\mathbf{Z}^{(v \circ u)} = \mathbf{Z}^{(v)} \circ \mathbf{Z}^{(w)}$ pour toute application $v : Y \to Z$; on montre aussi que $\mathbf{Z}^{(u)}$ est injective (resp. surjective, bijective) s’il en est ainsi de $u$.

Soit S une partie de X ; si $i$ est l’injection de S dans X, l’application $f = \mathbf{Z}^{(i)}$ est un isomorphisme de $\mathbf{Z}^{(S)}$ sur le sous-groupe H de $\mathbf{Z}^{(X)}$ engendré par les éléments $\delta_s$ pour $s \in S$. D’après (15), on a

$$
(f(\alpha))(x) = \begin{cases}
\alpha(x) & \text{si } x \in S \\
0 & \text{si } x \in X - S
\end{cases}
$$

et par suite H est l’ensemble des éléments de $\mathbf{Z}^{(X)}$ de support contenu dans S. On identifiera désormais $\mathbf{Z}^{(S)}$ à H au moyen de $f$.

La formule (15) montre que la restriction de $\mathbf{Z}^{(u)}$ à $\mathbf{N}^{(X)}$ est un homomorphisme $\mathbf{N}^{(u)}$ de $\mathbf{N}^{(X)}$ dans $\mathbf{N}^{(Y)}$. On a $\mathbf{N}^{(v \circ u)} = \mathbf{N}^{(v)} \circ \mathbf{N}^{(u)}$ pour toute application $v : Y \to Z$; de plus, $\mathbf{N}^{(u)}$ est injectif (resp. surjectif, bijectif) s’il en est ainsi de $u$. Si S est une partie de X, on a $\mathbf{N}^{(S)} = \mathbf{Z}^{(S)} \cap \mathbf{N}^{(X)}$.

#### Remarque {#alg-i-s7-n7-rem-1 .statement}

Soit M le monoïde multiplicatif des entiers strictement positifs, et soit $\mathfrak{P}$ l’ensemble des nombres premiers (I, p. 48, déf. 16). D’après la prop. 10 (I, p. 88), il existe un homomorphisme $u$ de $\mathbf{N}^{(\mathfrak{P})}$ dans M caractérisé par $u(\delta_p) = p$ pour tout nombre premier $p$. On a $u(\alpha) = \prod_{p \in \mathfrak{P}} p^{\alpha(p)}$ pour $\alpha$ dans $\mathbf{N}^{(\mathfrak{P})}$ et le th. 7 de I, p. 49 montre que $u$ est un isomorphisme de $\mathbf{N}^{(\mathfrak{P})}$ sur M.

### 8. Notation exponentielle

Soient M un monoïde, noté multiplicativement, et $\mathbf{u} = (u_x)_{x \in X}$ une famille d’éléments de M, commutant deux à deux. Soit $\alpha$ dans $\mathbf{N}^{(X)}$; les éléments $u_x^{\alpha(x)}$ et $u_y^{\alpha(y)}$ de M commutent pour $x, y$ dans X, et il existe une partie finie S de X telle que $u_x^{\alpha(x)} = 1$ pour $x$ dans $X - S$. On peut par suite poser:

$$
\mathbf{u}^{\alpha} = \prod_{x \in X} u_x^{\alpha(x)}.
$$

Soit $M'$ le sous-monoïde de M engendré par la famille $(u_x)_{x \in X}$; il est commutatif (I, p. 8, cor. 2). Il existe donc (I, p. 88, prop. 10) un unique homomorphisme $f$ de $\mathbf{N}^{(X)}$ dans $M'$ tel que $f(\delta_x) = u_x$ pour tout $x \in X$, et l’on a $f(\alpha) = \mathbf{u}^{\alpha}$ pour tout $\alpha$ dans $\mathbf{N}^{(X)}$. On en déduit les formules

$$
\mathbf{u}^{\alpha + \beta} = \mathbf{u}^{\alpha} \cdot \mathbf{u}^{\beta}
$$
$$
\mathbf{u}^{0} = 1
$$

(19) $$
\mathbf{u}^{\delta_x} = u_x
$$
pour $\alpha, \beta$ dans $\mathbf{N}^{(X)}$ et $x$ dans $X$.

Soit $\mathbf{v} = (v_x)_{x \in X}$ une autre famille d’éléments de $M$; on suppose que l’on a $v_x v_y = v_y v_x$ et $u_x v_y = v_y u_x$ pour $x, y$ dans $X$. Il existe alors (I, p. 8, cor. 2) un sous-monoïde commutatif $L$ de $M$ tel que $u_x \in L$ et $v_x \in L$ pour tout $x \in X$. L’application $\alpha \mapsto \mathbf{u}^\alpha \cdot \mathbf{v}^\alpha$ de $\mathbf{N}^{(X)}$ dans $L$ est alors un homomorphisme (I, p. 10, prop. 5) appliquant $\delta_x$ sur $u_x \cdot v_x$. On a donc a formule
(20) $$
\mathbf{u}^\alpha \cdot \mathbf{v}^\alpha = (\mathbf{u} \cdot \mathbf{v})^\alpha
$$
où $\mathbf{u} \cdot \mathbf{v}$ est la famille $(u_x \cdot v_x)_{x \in X}$.

Lorsque $M$ est commutatif, on peut définir $\mathbf{u}^\alpha$ pour toute famille $\mathbf{u}$ d’éléments de $M$ et les formules (15) à (20) sont valables sans restriction.

### 9. Relations entre les divers objets libres

Comme le monoïde libre $Mo(X)$ est un magma, la prop. 1 de I, p. 78, démontre l’existence d’un homomorphisme $\lambda : M(X) \to Mo(X)$ dont la restriction à $X$ est l’identité. De même, comme le groupe libre $F(X)$ est un monoïde, l’application identique de $X$ se prolonge en un homomorphisme $\mu : Mo(X) \to F(X)$ (I, p. 78, prop. 3). D’après I, p. 84, prop. 6 et prop. 7, $\mu$ est injectif. De même la prop. 10 de I, p. 88, et la prop. 8 de I, p. 85, démontrent l’existence d’homomorphismes $\nu : Mo(X) \to \mathbf{N}^{(X)}$ et $\pi : F(X) \to \mathbf{Z}^{(X)}$ caractérisés par $\nu(x) = \delta_x$ et $\pi(x) = \delta_x$ pour tout $x \in X$. Si $\iota$ est l’injection de $\mathbf{N}^{(X)}$ dans $\mathbf{Z}^{(X)}$, les deux homomorphismes $\iota \circ \nu$ et $\pi \circ \mu$ de $Mo(X)$ dans $\mathbf{Z}^{(X)}$ coïncident sur $X$, d’où $\iota \circ \nu = \pi \circ \mu$. On peut résumer la situation dans le diagramme commutatif suivant:

$$
\begin{array}{ccccc}
M(X) & \xrightarrow{\lambda} & Mo(X) & \xrightarrow{\nu} & \mathbf{N}^{(X)} \\
& & \downarrow \mu & & \downarrow \iota \\
& & F(X) & \xrightarrow{\pi} & \mathbf{Z}^{(X)}.
\end{array}
$$

Les homomorphismes $\lambda, \mu, \nu$ et $\pi$ seront qualifiés de canoniques.

Soit $w$ dans $M(X)$; on démontre immédiatement par récurrence sur $l(w)$ que la longueur du mot $\lambda(w)$ est égale à celle de $w$. Par ailleurs, on a
(21) $$
\nu(x_1 \ldots x_n) = \sum_{i=1}^n \delta_{x_i}
$$
pour $x_1, \ldots, x_n$ dans $X$, d’où $|\nu(x_1 \ldots x_n)| = n$ d’après (13) et (14) (I, p. 88). Autrement dit, on a
(22) $$
|\nu(u)| = l(u) \qquad (u \in Mo(X)).
$$

#### Proposition 11 {#alg-i-s7-prop-11 .statement}

*L’homomorphisme canonique* $\nu$ de $Mo(X)$ dans $\mathbf{N}^{(X)}$ est surjectif. Soient $w = x_1 \ldots x_n$ et $w' = x'_1 \ldots x'_m$ deux éléments de $Mo(X)$; pour qu’on ait $\nu(w) =$ ν(w'), il faut et il suffit que l’on ait m = n et qu’il existe une permutation σ ∈ S_n telle que x'_i = x_{σ(i)} pour 1 ≤ i ≤ n.

L’image de ν est un sous-monoïde I de N^{(X)} contenant les éléments δ_x (pour x ∈ X). La formule (12) (I, p. 88) montre que N^{(X)} est engendré par la famille (δ_x)_{x ∈ X}, d’où I = N^{(X)}. Par suite ν est surjectif.

Si m = n et si x'_i = x_{σ(i)} pour 1 ≤ i ≤ n, on a

$$
ν(w') = \sum_{i=1}^n δ_{x'_i} = \sum_{i=1}^n δ_{x_{σ(i)}} = \sum_{i=1}^n δ_{x_i} = ν(w)
$$

d’après la formule (21) (I, p. 90) et le théorème de commutativité (I, p. 8, th. 2).

Inversement, supposons que ν(w) et ν(w') soient égaux à un même élément α de N^{(X)}; d’après la formule (22) (I, p. 90), on a n = |α| = m. Pour tout x ∈ X, soit I_x (resp. I'_x) l’ensemble des entiers i tels que 1 ≤ i ≤ n et x_i = x (resp. x'_i = x). Donc (I_x)_{x ∈ X} et (I'_x)_{x ∈ X} sont des partitions de l’intervalle {1, n} de N; de plus, la formule $α = \sum_{i=1}^n δ_{x_i}$ montre que α(x) est le cardinal de I_x; de même la formule $α = \sum_{i=1}^n δ_{x'_i}$ montre que α(x) est le cardinal de I'_x. Il existe donc une permutation σ de {1, n} telle que σ(I'_x) = I_x pour tout x ∈ X, c’est-à-dire x'_i = x_{σ(i)} pour i = 1, ..., n.

#### Remarque {#alg-i-s7-n9-rem-1 .statement}

Soit S une partie de X. Rappelons que nous avons identifié M(S) à un sous-magma de M(X), Mo(S) à un sous-monoïde de Mo(X) et N^{(S)} à un sous-monoïde de N^{(X)}. On a

(23)

$$
M(S) = λ^{-1}(Mo(S)).
$$

En effet, il est clair que λ(M(S)) ⊂ Mo(S). Soit w ∈ λ^{-1}(Mo(S)); montrons, par récurrence sur l(w), que w ∈ M(S). C’est évident si l(w) = 1. Si l(w) > 1, on peut écrire w = w_1w_2 avec w_1, w_2 dans M(X), l(w_1) < l(w), l(w_2) < l(w). Alors λ(w_1)λ(w_2) ∈ Mo(S), donc λ(w_1) ∈ Mo(S) et λ(w_2) ∈ Mo(S), d’où w_1 ∈ M(S) et w_2 ∈ M(S) d’après l’hypothèse de récurrence, et finalement w ∈ M(S).

On a aussi

(24)

$$
Mo(S) = ν^{-1}(N^{(S)}).
$$

Cela résulte aussitôt de la formule (21) de I, p. 90.

De plus, N^{(S)} est l’ensemble des éléments de N^{(X)} dont le support est contenu dans S; si (S_i)_{i ∈ I} est une famille de parties de X, d’intersection S, on a donc N^{(S)} = ∩_{i ∈ I} N^{(S_i)} et les formules (23) et (24) entraînent

(25)

$$
M(S) = ∩_{i ∈ I} M(S_i), \quad Mo(S) = ∩_{i ∈ I} Mo(S_i).
$$

## EXERCICES {#alg-i-s7-exercises}

See the [exercises for § 7](exercises/s7/).
