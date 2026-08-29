---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 13
section_title: EXTENSIONS RADICIELLES DE HAUTEUR $\leqslant 1$
lang: fr
source: alg-iv-vii-fr
book_pages: A V.93-A V.101, A V.160-A V.161
pdf_pages: 0197-0205, 0264-0265
extraction: ocr
subsections:
    - "no": 1
      title: Parties $p$-libres et $p$-bases
      page: 93
      pdf_page: 197
    - "no": 2
      title: Différentielles et $p$-bases
      page: 96
      pdf_page: 200
    - "no": 3
      title: Correspondance entre sous-corps et algèbres de Lie de dérivations
      page: 99
      pdf_page: 203
statements: 22
exercises: 6
content_sha256: 6316f010144f544cbd464dc697739758c97518d59738e53e3a3e3a059078ac56
---

## § 13. EXTENSIONS RADICIELLES DE HAUTEUR $\leqslant 1$

Dans tout ce paragraphe, on note $p$ un nombre premier. Tous les corps considérés sont de caractéristique $p$.

### 1. Parties $p$-libres et $p$-bases

#### Définition 1 {#alg-v-s13-def-1 .statement}

*Soient K un corps et L une extension radicielle de hauteur $\leqslant 1$ de K. On dit qu’une famille $(x_i)_{i \in I}$ d’éléments de L est $p$-libre sur K (resp. est une $p$-base de L sur K) si l’on a $x_i \notin K$ pour tout $i \in I$ et si l’homomorphisme de $\bigotimes_{i \in I} K(x_i)$ dans L, déduit des injections canoniques $u_i : K(x_i) \to L$, est injectif (resp. bijectif).*

Si $a$ est un élément de $L - K$, il est radiciel de hauteur 1, et son polynôme minimal sur $K$ est donc $X^p - a^p$ (V, p. 23, prop. 1); par suite $\{ 1, a, \ldots, a^{p-1} \}$ est une base de $K(a)$ sur $K$. Soient $(x_i)_{i \in I}$ une famille d’éléments de $L - K$ et $\Lambda$ la partie de $\mathbf{N}^{(I)}$ formée des familles à support fini $\alpha = (\alpha_i)_{i \in I}$ telles que $\alpha_i < p$ pour tout $i \in I$; la prop. 9 (III, p. 43) montre que les éléments $\bigotimes_{i \in I} x_i^{\alpha_i}$ pour $\alpha$ parcourant $\Lambda$ forment une base de l’espace vectoriel $\bigotimes_{i \in I} K(x_i)$ sur $K$. De plus, l’homomorphisme canonique de $\bigotimes_{i \in I} K(x_i)$ dans $L$ a pour image $K(x_i)_{i \in I}$ (V, p. 18, cor. 1). On a donc la proposition suivante :

#### Proposition 1 {#alg-v-s13-prop-1 .statement}

*Soient $K$ un corps, $L$ une extension radicielle de hauteur $\leq 1$ de $K$ et $x = (x_i)_{i \in I}$ une famille d’éléments de $L$. Alors l’espace vectoriel $K(x_i)_{i \in I}$ sur $K$ est engendré par les produits $x^\alpha = \prod_{i \in I} x_i^{\alpha_i}$ pour $\alpha$ dans $\Lambda$. Pour que $(x_i)_{i \in I}$ soit $p$-libre (resp. une $p$-base), il faut et il suffit que la famille $(x^\alpha)_{\alpha \in \Lambda}$ soit libre sur $K$ (resp. soit une base de $L$ sur $K$).*

#### Corollaire {#alg-v-s13-n1-cor-1 .statement}

*Soit $L'$ une extension d’un corps $K$ engendrée par deux sous-extensions linéairement disjointes $K'$ et $L$. Supposons $L$ radicielle de hauteur $\leq 1$ sur $K$; alors $L'$ est radicielle de hauteur $\leq 1$ sur $K'$. De plus, pour qu’une famille d’éléments de $L$ soit $p$-libre sur $K$ (resp. soit une $p$-base de $L$ sur $K$), il faut et il suffit qu’elle soit $p$-libre sur $K'$ (resp. soit une $p$-base de $L'$ sur $K'$).

On a $L^p \subset K \subset K'$ et $L' = K'(L)$, d’où ${L'}^p = {K'}^p(L^p) \subset K'$. Autrement dit, $L'$ est une extension radicielle de hauteur $\leq 1$ de $K'$. Les autres assertions du corollaire résultent aussitôt de la prop. 1 et de V, p. 13, prop. 5.

#### Remarque {#alg-v-s13-n1-rem-1 .statement}

Soient $K$ un corps, $L$ une extension radicielle de hauteur $\leq 1$ de $K$ et $(x_i)_{i \in I}$ une famille d’éléments de $L$. Soient $A$ l’algèbre de polynômes $K[(X_i)_{i \in I}]$, $a$ l’idéal de $A$ engendré par les polynômes $X_i^p - x_i^p$ et $\varphi : A \to L$ l’homomorphisme de $K$-algèbres tel que $\varphi(X_i) = x_i$ pour tout $i \in I$. La famille $(x_i)_{i \in I}$ est $p$-libre si et seulement si le noyau de $\varphi$ est égal à $a$. En effet, $K[(X_i)]/a$ s’identifie à l’algèbre $\bigotimes_{i \in I} K[X_i]/(X_i^p - x_i^p)$.

Soit $L$ une extension radicielle de hauteur $\leq 1$ d’un corps $K$. On dit qu’une partie $S$ de $L$ est $p$-libre (resp. une $p$-base) si la famille définie par l’application identique de $S$ sur elle-même est $p$-libre (resp. une $p$-base). Pour qu’une famille $(x_i)_{i \in I}$ d’éléments de $L$ soit $p$-libre (resp. une $p$-base), il faut et il suffit que l’application $i \mapsto x_i$ soit une bijection de $I$ sur une partie $p$-libre (resp. une $p$-base) de $L$. D’après la prop. 1, toute partie d’une partie $p$-libre est $p$-libre ; réciproquement si $S$ est une partie de $L$ telle que toute partie finie de $S$ soit $p$-libre, alors $S$ est $p$-libre. Enfin, une $p$-base de $L$ sur $K$ est une partie $p$-libre $B$ telle que $L = K(B)$.

#### Proposition 2 {#alg-v-s13-prop-2 .statement}

Soient K un corps, L une extension radicielle de hauteur $\leq 1$ de K et S une partie de L. Pour que S soit p-libre, il faut et il suffit que l’on ait K(T) $\neq$ K(S) pour toute partie T $\neq$ S de S.

Supposons d’abord que S soit p-libre et soit T $\neq$ S une partie de S. Notons $\Lambda$ l’ensemble des familles à support fini $\alpha = (\alpha_s)_{s \in S}$ d’entiers compris entre 0 et $p - 1$; soit $\Lambda'$ la partie de $\Lambda$ formée des familles $\alpha = (\alpha_s)_{s \in S}$ telles que $\alpha_s = 0$ pour tout s dans T – S. Posons aussi $u_\alpha = \prod_{s \in S} s^{\alpha_s}$ pour $\alpha \in \Lambda$. Alors (V, p. 94, prop. 1), la famille $(u_\alpha)_{\alpha \in \Lambda}$ est une base de K(S) sur K, et la sous-famille $(u_\alpha)_{\alpha \in \Lambda'}$ est une base de K(T) sur K. Comme on a $\Lambda' \neq \Lambda$, on a K(T) $\neq$ K(S).

Supposons maintenant que S né soit pas p-libre. Il existe alors un entier $n \geq 1$ et une suite d’éléments $x_1, ..., x_n$ de S telle que $(x_1, ..., x_{n-1})$ soit p-libre, mais non $(x_1, ..., x_n)$. On a $[K(x_1, ..., x_{n-1}):K] = p^{n-1}$ et $[K(x_1, ..., x_n):K] < p^n$. Comme $[K(x_1, ..., x_n):K]$ est un multiple de $[K(x_1, ..., x_{n-1}):K]$, on a donc

$$
[K(x_1, ..., x_n):K] = [K(x_1, ..., x_{n-1}):K],
$$

d’où $x_n \in K(x_1, ..., x_{n-1})$. Ceci entraîne $K(S - \{x_n\}) = K(S)$.

#### Proposition 3 {#alg-v-s13-prop-3 .statement}

Soient K un corps, L une extension radicielle de hauteur $\leq 1$ de K, et S, T deux parties de L. Les conditions suivantes sont équivalentes :

a) La partie S est p-libre sur K, et T est p-libre sur K(S).
b) On a $S \cap T = \varnothing$ et $S \cup T$ est p-libre sur K.

Si T est p-libre sur K(S), on a $T \cap K(S) = \varnothing$ et a fortiori $S \cap T = \varnothing$. Nous pouvons donc supposer S et T disjointes. Soit $\Lambda$ la partie de $N^{(S \cup T)}$ formée des familles $\alpha = (\alpha_x)_{x \in S \cup T}$ avec $\alpha_x < p$ pour tout x dans S $\cup$ T. Définissons de manière analogue les parties $\Lambda'$ de $N^{(S)}$ et $\Lambda''$ de $N^{(T)}$. On peut identifier de manière naturelle $N^{(S \cup T)}$ à $N^{(S)} \times N^{(T)}$, et $\Lambda$ s’identifie à $\Lambda' \times \Lambda''$. Pour $\alpha \in \Lambda$, posons $u_\alpha = \prod_{x \in S \cup T} x^{\alpha_x}$; définissons de même $u'_\beta$ et $u''_\gamma$ pour $\beta \in \Lambda'$ et $\gamma \in \Lambda''$. On a $u_\alpha = u'_\beta u''_\gamma$ pour $\alpha = (\beta, \gamma)$ dans $\Lambda = \Lambda' \times \Lambda''$. De plus, $(u'_\beta)_{\beta \in \Lambda'}$ engendre le K-espace vectoriel K(S) (V, p. 94, prop. 1). Pour que S $\cup$ T soit p-libre sur K, il faut et il suffit que la famille $(u'_\beta u''_\gamma)_{\beta \in \Lambda', \gamma \in \Lambda''}$ soit libre sur K (V, p. 94, prop. 1); il revient au même (II, p. 31) de supposer que la famille $(u'_\beta)_{\beta \in \Lambda'}$ est libre sur K et la famille $(u''_\gamma)_{\gamma \in \Lambda''}$ libre sur K(S). L’équivalence de a) et b) résulte alors de la prop. 1 (V, p. 94).

#### Corollaire {#alg-v-s13-n1-cor-2 .statement}

Soient L une extension radicielle de hauteur $\leq 1$ de K et M une sous-extension de L. Alors L est radicielle de hauteur $\leq 1$ sur M et M est radicielle de hauteur $\leq 1$ sur K. De plus, si B est une p-base de M sur K et C une p-base de L sur M, on a $B \cap C = \varnothing$ et $B \cup C$ est une p-base de L sur K.

Soit K un corps. On dit qu’une famille $(x_i)_{i \in I}$ est une p-base (absolue) de K si c’est une p-base de K sur $K^p$. Pour tout entier $n \geq 1$, notons $\Lambda(n)$ la partie de $N^{(I)}$ formée des $\alpha = (\alpha_i)_{i \in I}$ tels que $\alpha_i < p^n$ pour tout $i \in I$.

#### Proposition 4 {#alg-v-s13-prop-4 .statement}

Soit $x = (x_i)_{i \in I}$ une $p$-base de $K$. Pour tout entier $n \geq 1$, la famille $(x^\alpha)_{\alpha \in \Lambda(n)}$ est une base de $K$ sur $K^{p^n}$.

Pour $n = 1$, l’assertion se réduit à la prop. 1 (V, p. 94). L’ensemble $\Lambda(n)$ se compose des éléments de $\mathbf{N}^{(1)}$ de la forme $\alpha = \beta + p^{n-1}\gamma$ avec $\beta \in \Lambda(n-1)$ et $\gamma \in \Lambda(1)$. Une telle décomposition est unique, et l’on a $x^\alpha = x^\beta (x^\gamma)^{p^{n-1}}$. De plus, la famille $(x_i^{p^{n-1}})_{i \in I}$ est évidemment une $p$-base de $K^{p^{n-1}}$ sur $K^{p^n}$, donc la famille $(x^\gamma)^{p^{n-1}}$ est une base de $K^{p^{n-1}}$ sur $K^{p^n}$. On conclut alors par récurrence, grâce à II, p. 31, prop. 25.

### 2. Différentielles et $p$-bases

Soient $K$ un corps (de caractéristique $p$) et $V$ un espace vectoriel sur $K$. Rappe-lons (III, p. 119) qu’une dérivation de $K$ dans $V$ est une application $D$ de $K$ dans $V$ satisfaisant aux relations

(1)
$$
D(x + y) = D(x) + D(y)
$$
(2)
$$
D(xy) = xD(y) + yD(x)
$$
pour $x, y \in K$. On en déduit $D(1) = 0$ et $D(x^n) = nx^{n-1}D(x)$ pour tout $x \neq 0$ et tout entier $n \in \mathbf{Z}$ (III, p. 123 et 124). Comme $K$ est de caractéristique $p$, on a donc pour tout $x$ dans $K$

(3)
$$
D(x^p) = 0 .
$$
Par ailleurs (III, p. 123), on a pour $x, y \in K, y \neq 0$,

(4)
$$
D(x/y) = (yD(x) - xD(y))/y^2 .
$$

D’après les formules précédentes, le noyau de $D$ est donc un sous-corps $E$ de $K$ contenant $K^p$. Soit $M$ un sous-corps de $K$; on dit que $D$ est une $M$-dérivation si elle est $M$-linéaire ; d’après (2), il revient au même de supposer que la restriction de $D$ à $M$ est nulle.

On a défini (III, p. 134) le module $\Omega_M(K)$ des $M$-différentielles de $K$ et la $M$-dérivation canonique $d = d_{K/M}$ de $K$ dans $\Omega_M(K)$. L’image de $d_{K/M}$ engendre le $K$-espace vectoriel $\Omega_M(K)$. Pour qu’une application $D$ de $K$ dans $V$ soit une $M$-dérivation, il faut et il suffit qu’il existe une application $K$-linéaire $u : \Omega_M(K) \to V$ telle que $D = u \circ d_{K/M}$; cette application $u$ est déterminée de manière unique.

#### Proposition 5 {#alg-v-s13-prop-5 .statement}

Soient $K$ un corps et $L$ une extension de $K$ engendrée par un élément $x$ tel que $x \notin K, x^p \in K$. Soient $V$ un espace vectoriel sur $L$ et $\Delta$ une dérivation de $K$ dans $V$, telle que $\Delta(x^p) = 0$. Il existe alors une unique dérivation $D$ de $L$ dans $V$ prolongeant $\Delta$ et telle que $D(x) = 0$.

D’après V, p. 23, prop. 1, $\{1, x, \ldots, x^{p-1}\}$ est une base de $L$ sur $K$. Pour tout élément $u = a_0 + a_1 x + \cdots + a_{p-1} x^{p-1}$ de $L$ (avec $a_0, \ldots, a_{p-1}$ dans $K$), on posera $D(u) = \Delta(a_0) + x \Delta(a_1) + \cdots + x^{p-1} \Delta(a_{p-1})$. Il est clair que $D$ prolonge $\Delta$, et satisfait à (1); il suffit donc d’établir la relation
$$
D(uv) = u.D(v) + v.D(u)
$$
lorsque $u$ est de la forme $ax^i$ et $v$ de la forme $bx^j$ avec $a, b$ dans $K$, $0 \leq i < p$ et $0 \leq j < p$.

Lorsque $i + j < p$, on a $uv = x^{i+j}.ab$, d’où $D(uv) = x^{i+j}\Delta(ab)$. Dans le cas contraire, on a $0 \leq i + j - p < p$ et donc $uv = x^{i+j-p}(abx^p)$ avec $abx^p \in K$, mais comme $\Delta(x^p) = 0$, on a $\Delta(abx^p) = x^p \Delta(ab)$, d’où encore $D(uv) = x^{i+j}\Delta(ab)$. On a donc dans tous les cas
$$
\begin{align*}
D(uv) &= x^{i+j}\Delta(ab) = x^i x^j (a.\Delta(b) + b.\Delta(a)) \\
&= (ax^i) x^j.\Delta(b) + (bx^j) x^i.\Delta(a) = u.D(v) + v.D(u) .
\end{align*}
$$

#### Corollaire 1 {#alg-v-s13-prop-5-cor-1 .statement}

*Soient $K$ un corps, $L$ une extension radicielle de hauteur $\leq 1$ de $K$ et $V$ un espace vectoriel sur $L$. Toute dérivation $\Delta$ de $K$ dans $V$ nulle sur $L^p$ se prolonge en une dérivation de $L$ dans $V$.

D’après le th. de Zorn (E, III, p. 20), il existe un prolongement maximal de $\Delta$ en une dérivation $D_0 : L_0 \to V$, où $L_0$ est un sous-corps de $L$ contenant $K$. Soit $x \in L$; on a $x^p \in L_0$ et $\Delta(x^p) = 0$, d’où $D_0(x^p) = 0$. D’après la prop. 5, $D_0$ se prolonge en une dérivation définie dans $L_0(x)$; d’après le caractère maximal de $D_0$, on a donc $L_0(x) = L_0$, d’où $x \in L_0$. Vu l’arbitraire de $x$, on a $L_0 = L$.

#### Corollaire 2 {#alg-v-s13-prop-5-cor-2 .statement}

*Soient $L$ une extension radicielle de hauteur $\leq 1$ d’un corps $K$ et $E$ une sous-extension de $L$. Soit $U$ le sous-espace de $\Omega_K(L)$ engendré par les différentielles des éléments de $E$. Alors $E$ se compose des éléments de $L$ dont la différentielle appartient à $U$. En particulier, on a $d_{L/K} x \neq 0$ pour tout $x \in L - K$.

Soit $x$ un élément de $L$ n’appartenant pas à $E$. Alors $\{ 1, x, ..., x^{p-1} \}$ est une base de $E(x)$ sur $E$. Soit $\Delta$ l’application $E$-linéaire de $E(x)$ dans $L$ telle que $\Delta(x^i) = ix^i$ pour $0 \leq i < p$. On vérifie aussitôt que $\Delta$ est une $E$-dérivation de $E(x)$ dans $L$, et en particulier une $K$-dérivation. D’après le corollaire 1 à la prop. 5, il existe une $K$-dérivation $D$ de $L$ dans $L$ prolongeant $\Delta$. D’après la propriété universelle de $\Omega_K(L)$, il existe une forme linéaire $u$ sur ce $L$-espace vectoriel telle que $D = u \circ d_{L/K}$. On a $D(x) = x$ et $D|E = 0$; par suite, on a $u(d_{L/K} x) \neq 0$ et $u|U = 0$, d’où $d_{L/K} x \notin U$.

La dernière assertion est le cas particulier $E = K$; on a alors $U = 0$.

#### Théorème 1 {#alg-v-s13-thm-1 .statement}

*Soient $L$ une extension radicielle de hauteur $\leq 1$ d’un corps $K$ et $(x_i)_{i \in I}$ une famille d’éléments de $L$.

a) *Pour que $(x_i)_{i \in I}$ soit $p$-libre sur $K$, il faut et il suffit que la famille $(dx_i)_{i \in I}$ soit libre dans le $L$-espace vectoriel $\Omega_K(L)$.

b) *Pour que $(x_i)_{i \in I}$ engendre $L$ sur $K$, il faut et il suffit que la famille $(dx_i)_{i \in I}$ engendre le $L$-espace vectoriel $\Omega_K(L)$.

c) *Pour que $(x_i)_{i \in I}$ soit une $p$-base de $L$ sur $K$, il faut et il suffit que la famille $(dx_i)_{i \in I}$ soit une base du $L$-espace vectoriel $\Omega_K(L)$.

Remarquons d’abord que la différentielle $dx$ d’un élément du corps $K((x_i)_{i \in I})$ est une combinaison linéaire à coefficients dans $L$ des différentielles $dx_i, i \in I$. Pour que la famille $(x_i)_{i \in I}$ soit $p$-libre, il faut et il suffit que l’on ait $x_i \notin K(x_j)_{j \in I - \{i\}}$ pour tout $i \in I$ (V, p. 95, prop. 2). D’après le cor. 2 de la prop. 5, ceci signifie que $dx_i$ n’est pas combinaison linéaire des $dx_j$ pour $j \neq i$ dans $I$. L’assertion a) résulte de là. L’assertion b) résulte aussitôt du cor. 2 de la prop. 5, et c) résulte de a) et b).

Le corollaire suivant précise le cor. 1 de la prop. 5 :

#### Corollaire {#alg-v-s13-n2-cor-1 .statement}

*Soit* $(x_i)_{i \in I}$ *une p-base de* $L$ *sur* $K$. *Soient* $V$ *un espace vectoriel sur* $L$, $\Delta$ *une dérivation de* $K$ *dans* $V$ *nulle sur* $L^p$ *et* $(u_i)_{i \in I}$ *une famille d’éléments de* $V$. *Il existe une dérivation* $D$ *de* $L$ *dans* $V$, *et une seule, qui prolonge* $\Delta$ *et applique* $x_i$ *sur* $u_i$ *pour tout* $i \in I$.

D’après le cor. 1 de la prop. 5, il existe une dérivation $D_0$ de $L$ dans $V$ prolongeant $\Delta$. Les dérivations de $L$ dans $V$ prolongeant $\Delta$ sont exactement les applications de la forme $D = D_0 + u \circ d_{L/K}$, où $u$ est une application $L$-linéaire de $\Omega_K(L)$ dans $V$. On a $D(x_i) = u_i$ si et seulement si l’application linéaire $u$ satisfait aux conditions $u(dx_i) = u_i - D_0(x_i)$. Puisque la famille $(dx_i)$ est une base de $\Omega_K(L)$, cela détermine $u$ de manière unique, d’où le corollaire.

Soient $L$ une extension radicielle de hauteur $\leq 1$ de $K$ et $(x_i)_{i \in I}$ une $p$-base de $L$ sur $K$. D’après le cor. du th. 1, il existe pour tout $i \in I$ une $K$-dérivation $D_i$ de $L$ dans $L$ caractérisée par $D_i(x_j) = \delta_{ij}$ (symbole de Kronecker); on dira parfois que $D_i$ est la *dérivation partielle par rapport à* $x_i$. Lorsque $I$ est *fini*, la famille $(D_i)_{i \in I}$ est une base de l’espace vectoriel sur $L$ formé des $K$-dérivations de $L$ dans $L$.

Le th. 1 permet de ramener l’étude des $p$-bases à celle des bases d’un espace vectoriel. On a par exemple les résultats suivants :

#### Théorème 2 {#alg-v-s13-thm-2 .statement}

*Soit* $L$ *une extension radicielle de hauteur* $\leq 1$ *d’un corps* $K$.

*a)* *Il existe des p-bases de* $L$ *sur* $K$. *Plus précisément, si* $S$ *est une partie p-libre de* $L$ *sur* $K$ *et* $T$ *une partie de* $L$ *telle que* $S \subset T$ *et* $L = K(T)$, *il existe une p-base* $B$ *de* $L$ *sur* $K$ *telle que* $S \subset B \subset T$.

*b)* *Deux p-bases de* $L$ *sur* $K$ *ont même cardinal*.

*c)* *Pour que* $[L : K]$ *soit fini, il faut et il suffit que l’espace vectoriel* $\Omega_K(L)$ *sur* $L$ *soit de dimension finie sur* $L$ *et l’on a alors*

(5)
$$
[L : K] = p^{[\Omega_K(L) : L]}.
$$

Les assertions a) et b) sont immédiates (II, p. 95 et 96). Si $[L : K]$ est fini, il existe d’après a) une $p$-base finie $(x_1, ..., x_n)$ de $L$ sur $K$; alors les monômes $x_1^{\alpha_1} ... x_n^{\alpha_n}$ avec $0 \leq \alpha_i < p$ pour $1 \leq i \leq n$ forment une base de $L$ sur $K$ et les différentielles $dx_1, ..., dx_n$ forment une base de $\Omega_K(L)$ sur $L$. On a donc $[L : K] = p^n$ et $[\Omega_K(L) : L] = n$. Réciproquement, si $\Omega_K(L)$ est de dimension finie sur $L$, il existe une $p$-base finie de $L$ sur $K$ (V, p. 97, th. 1) et $[L : K]$ est fini.

#### Corollaire {#alg-v-s13-n2-cor-2 .statement}

*Pour tout* $x \in L - K$, *il existe une p-base de* $L$ *sur* $K$ *contenant* $x$.
En effet, $\{x\}$ est une partie $p$-libre de $L$ sur $K$, et il suffit d’appliquer le th. 2, *a)*.

Soient $K$ un corps et $L$ une extension de $K$. Si $D$ est une $K$-dérivation de $L$ à valeurs dans un $L$-espace vectoriel, on a $D(x^p) = 0$ pour tout $x \in L$, et par suite $D$ est une $K(L^p)$-dérivation. On en déduit $\Omega_K(L) = \Omega_{K(L^p)}(L)$. Comme $L$ est une extension radicielle de hauteur $\leq 1$ de $K(L^p)$, on peut appliquer les résultats précédents. Par exemple, du th. 1, *c)* on déduit ceci : soit $(x_i)_{i \in I}$ une famille d’éléments de $L$; pour que $(dx_i)_{i \in I}$ soit une base du $L$-espace vectoriel $\Omega_K(L)$, il faut et il suffit que $(x_i)_{i \in I}$ soit une $p$-base de $L$ sur $K(L^p)$. De manière analogue, le cor. 2 de la prop. 5 entraîne :

#### Proposition 6 {#alg-v-s13-prop-6 .statement}

*Soient* $K$ *un corps (de caractéristique p)* *et* $L$ *une extension de* $K$.
  a) *Soit* $x \in L$. *La différentielle* $d_{L/K} x$ *est nulle si et seulement si* $x$ *appartient à* $K(L^p)$.
  b) *On a* $\Omega_K(L) = 0$ *si et seulement si* $L = K(L^p)$.
  c) *Supposons* $L$ *radicielle de hauteur finie sur* $K$. *On a alors* $\Omega_K(L) = 0$ *si et seulement si* $L = K$.

### 3. Correspondance entre sous-corps et algèbres de Lie de dérivations

On note $E$ un corps et $g$ l’ensemble des dérivations de $E$ dans $E$. Rappelons que $g$ est un espace vectoriel sur $E$, dont les opérations sont définies par

$$
(D + D')(x) = D(x) + D'(x), \quad (aD)(x) = a.D(x)
$$

pour $D, D'$ dans $g$ et $a, x$ dans $E$. De plus, si $D$ et $D'$ sont deux dérivations de $E$ dans $E$, il en est de même de $[D, D'] = DD' - D'D$ (III, p. 120). Enfin la formule de Leibniz (III, p. 122) donne

$$
D^p(xy) = x.D^p(y) + \sum_{j=1}^{p-1} \binom{p}{j} D^j(x) D^{p-j}(y) + D^p(x).y
$$

$(x, y \text{ dans } E)$; comme les coefficients binomiaux $\binom{p}{j}$ pour $1 \leq j \leq p-1$ sont divisibles par $p$ (V, p. 4, lemme 1), on voit que $D^p$ est une dérivation de $E$ dans $E$. On établit immédiatement la relation (pour $a, a' \in E$)

$$
[aD, a'D'] = aa'.[D, D'] + (aD(a')).D' - (a'D'(a)).D .
$$

En particulier, l’application $(D, D') \mapsto [D, D']$ de $g \times g$ dans $g$ est $E^p$-linéaire.

On note $\mathcal{C}$ l’ensemble des sous-corps $K$ de $E$ tels que $E^p \subset K$ et que $[E : K]$ soit fini ; pour tout $K \in \mathcal{C}$, on note $g(K)$ l’ensemble des $K$-dérivations de $E$. Par ailleurs, on note $\mathcal{L}$ l’ensemble des sous-espaces vectoriels $h$ de $g$, de dimension finie sur $E$, et tels que l’on ait $[D, D'] \in h$ et $D^p \in h$ quels que soient $D$ et $D'$ dans $h$; pour tout $h \in \mathcal{L}$, on note $I(h)$ l’ensemble des $x \in E$ tels que $D(x) = 0$ pour tout $D \in h$.

#### Théorème 3 (Jacobson) {#alg-v-s13-thm-3 .statement}

Les applications $K \mapsto g(K)$ et $h \mapsto I(h)$ sont des bijections de $\mathcal{C}$ sur $\mathcal{L}$ et $\mathcal{L}$ sur $\mathcal{C}$ respectivement, réciproques l’une de l’autre. Si $K \in \mathcal{C}$ et $h \in \mathcal{L}$ se correspondent, on a $[E : K] = p^{[h : E]}$.

La démonstration utilise plusieurs lemmes préliminaires.

#### Lemme 1 {#alg-v-s13-lem-1 .statement}

Soient $L$ un corps, $V$ un espace vectoriel sur $L$ et $u$ un endomorphisme de $V$ tel que $u^p = u$. Pour tout $i \in \mathbf{F}_p$, soit $V_i$ le noyau de $u - i$. On a alors
$$
V = \bigoplus_{i \in \mathbf{F}_p} V_i.
$$
Pour tout $i \in \mathbf{F}_p$, notons $P_i(X)$ le polynôme $- \prod_{j \neq i} (X - j)$. On a
$$
(X - i) P_i(X) = X - X^p
$$
d’après la formule (2) (V, p. 90). Dérivant la formule (2) citée, on trouve
$$
\sum_{i \in \mathbf{F}_p} P_i(X) = 1.
$$
Les formules (8) et (9) montrent que l’endomorphisme $P_i(u)$ de $V$ applique $V$ dans $V_i$ et qu’on a $\sum_{i \in \mathbf{F}_p} P_i(u) = 1$, d’où $V = \sum_{i \in \mathbf{F}_p} V_i$. Il reste à démontrer que la somme est directe. Pour tout $i \in \mathbf{F}_p$, soit $v_i \in V_i$; il est immédiat que $P_i(u)$ annule $v_j$ pour tout $j \neq i$ et l’on a $P_i(u) v_i = a v_i$ avec $a = - \prod_{n \in \mathbf{F}_p^*} n \neq 0$. La relation $\sum_{i \in \mathbf{F}_p} v_i = 0$ entraîne donc $v_i = 0$ pour tout $i \in \mathbf{F}_p$ et la somme est directe.

#### Lemme 2 {#alg-v-s13-lem-2 .statement}

Soit $D$ une dérivation de $E$ telle que $D^p = D$ et soit $K$ le noyau de $D$. On suppose qu’il existe $x$ non nul dans $E$ tel que $D(x) = x$. Alors $K$ est un sous-corps de $E$ contenant $E^p$ et l’on a $[E : K] = p$.

Il est clair que $K$ est un sous-corps de $E$ contenant $E^p$. Notons $K_i$ le noyau de $D - i$ pour $i \in \mathbf{F}_p$. On a $K_0 = K$ et le lemme 1 entraîne $E = \bigoplus_{i \in \mathbf{F}_p} K_i$. Soit $i \in \mathbf{F}_p$ et soit $u$ dans $K_i$; on a
$$
D(xu) = D(x).u + x.D(u) = xu + x(iu) = (i + 1)xu
$$
d’où $xu \in K_{i+1}$. Comme $x$ est non nul, la multiplication par $x$ est un automorphisme du $K$-espace vectoriel $E$, qui envoie $K_i$ sur $K_{i+1}$ pour tout $i \in \mathbf{F}_p$. Comme on a $[K_0 : K] = 1$, on a $[K_i : K] = 1$ pour tout $i \in \mathbf{F}_p$, d’où $[E : K] = p$.

#### Lemme 3 {#alg-v-s13-lem-3 .statement}

Soit $h \in \mathcal{L}$, de dimension $s$ sur $E$. Alors $I(h)$ appartient à $\mathcal{C}$ et l’on a $[E : I(h)] = p^s$.

Il est clair que $I(h)$ est un sous-corps de $E$ contenant $E^p$. Pour tout $x \in E$, soit $f_x$ la forme $E$-linéaire $D \mapsto D(x)$ sur $h$. Comme l’intersection des noyaux de ces formes linéaires est réduite à 0, elles engendrent l’espace vectoriel dual de $h$ (II, p. 104, th. 7); par suite, il existe $x_1, \ldots, x_s$ dans $E$ tels que les formes linéaires $f_{x_1}, \ldots, f_{x_s}$ forment une base de ce dual. Soit $(\Delta_1, \ldots, \Delta_s)$ la base de $h$ caractérisée par

Δ_i(x_j) = f_{x_j}(Δ_i) = δ_{ij}. Posons D_i = x_iΔ_i. Alors (D_1, ..., D_s) est une base de h sur E, et l’on a D_i(x_j) = x_iδ_{ij}. Les dérivations D_i^p - D_i et [D_i, D_j] pour i, j = 1, ..., s appartiennent à h et annulent x_1, ..., x_s ; on a donc

(10) $D_i^p = D_i , \quad [D_i, D_j] = 0 .$

Pour i compris entre 0 et s, notons K_i l’intersection des noyaux des dérivations D_j pour 1 ≤ j ≤ i. Alors K_i est un sous-corps de E et l’on a

$$ E = K_0 \supset K_1 \supset ... \supset K_{s-1} \supset K_s = I(h) . $$

Soit i compris entre 0 et s − 1 ; alors K_i est stable par D_{i+1} car D_{i+1} commute à D_1, ..., D_i. De plus, on a D_{i+1}^p = D_{i+1}, D_{i+1}(x_{i+1}) = x_{i+1} ≠ 0 et x_{i+1} ∈ K_i. Le lemme 2 entraîne alors [K_i : K_{i+1}] = p, d’où finalement [E : K] = [K_0 : K_s] = p^s.

Passons à la démonstration du théorème. Soit h ∈ 𝔖, de dimension s sur E ; posons K = I(h) ; alors [E : K] = p^s d’après le lemme 3, d’où [Ω_K(E) : E] = s d’après le th. 2, c) (V, p. 98). D’après la propriété universelle du module des différentielles, l’application u ↦ u ∘ d_{E/K} est un isomorphisme du dual de Ω_K(E) sur g(K), donc [g(K) : E] = s. Or on a [h : E] = s et h ⊂ g(K), d’où h = g(K), c’est-à-dire h = g(I(h)).

Inversement, pour tout corps K ∈ 𝔖, il est immédiat que g(K) appartient à 𝔖 (V, p. 98, th. 2, c)). Si x appartient à I(g(K)), on a u(d_{E/K}x) = 0 pour toute forme linéaire u sur Ω_K(E), d’où d_{E/K}x = 0 et finalement x ∈ K par le cor. 2 de la prop. 5 (V, p. 97). On a donc K = I(g(K)).

#### Remarque 1 {#alg-v-s13-n3-rem-1 .statement}

Les bijections réciproques K ↦ g(K) et h ↦ I(h) sont décroissantes ; par suite, h ↦ I(h) est un isomorphisme de l’ensemble ordonné 𝔖 sur l’ensemble ordonné opposé à 𝔖. On en déduit la relation I(h ∩ h') = E^p(I(h), I(h')) pour h, h' dans 𝔖, car h ∩ h' est le plus grand élément de 𝔖 contenu à la fois dans h et h'.

#### Remarque 2 {#alg-v-s13-n3-rem-2 .statement}

On peut montrer que tout sous-espace de dimension finie de g, qui est stable par D ↦ D^p, est aussi stable par le crochet.

## EXERCICES {#alg-v-s13-exercises}

See the [exercises for § 13](exercises/s13/).
