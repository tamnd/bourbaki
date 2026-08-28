---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 3
section_title: Algèbre enveloppante de l'algèbre de Lie libre
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0030-0036, 0077-0077
extraction: ocr
subsections:
    - "no": 1
      title: Algèbre enveloppante de $L(X)$
      page: 0
      pdf_page: 30
    - "no": 2
      title: Projecteur de $A^+(X)$ sur $L(X)$
      page: 0
      pdf_page: 32
    - "no": 3
      title: Dimension des composantes homogènes de $L(X)$
      page: 0
      pdf_page: 33
statements: 10
exercises: 4
content_sha256: 8e67284651045a700a67dbcb545887f81a8fbe0cbd98b7244242686345694ce3
---

## § 3. Algèbre enveloppante de l’algèbre de Lie libre

Dans ce paragraphe, on note $A(X) = A_K(X)$ l’algèbre associative libre Libas(X) de l’ensemble $X$ sur l’anneau $K$ (A, III, p. 21, déf. 2). On identifie $X$ à son image canonique dans $A(X)$; rappelons que le $K$-module $A(X)$ admet pour base le monoïde libre $Mo(X)$ déduit de $X$; on note $A^+(X)$ le sous-module de $A(X)$ engendré par les mots non vides.

### 1. Algèbre enveloppante de $L(X)$

#### Théorème 1 {#lie-ii-s3-thm-1 .statement}

Soit $\alpha : L(X) \to A(X)$ l’unique homomorphisme d’algèbres de Lie prolongeant l’injection canonique de $X$ dans $A(X)$ (§ 2, n° 2, prop. 1). Soit $\sigma : L(X) \to U(L(X))$ l’application canonique de $L(X)$ dans son algèbre enveloppante et soit $\beta : U(L(X)) \to A(X)$ l’unique homomorphisme d’algèbres unifères tel que $\beta \circ \sigma = \alpha$ (chap. I, § 2, n° 1, prop. 1). Alors:
a) $\alpha$ est injectif, et $\alpha(L(X))$ est un sous-module facteur direct de $A(X)$.
b) $\beta$ est bijectif.

Soient $B$ une $K$-algèbre unifière et $\varphi$ une application de $X$ dans $B$; d’après la prop. 1 du § 2, n° 2, il existe un homomorphisme d’algèbres de Lie $\psi : L(X) \to B$ tel que $\psi | X = \varphi$; d’après la prop. 1 du chap. I, § 2, n° 1, il existe un homomorphisme d’algèbres unifères $\theta : U(L(X)) \to B$ tel que $\theta \circ \sigma = \psi$, donc tel que $(\theta \circ \sigma) | X = \varphi$. Comme $\sigma(X)$ engendre l’algèbre unifière $U(L(X))$, l’homomorphisme $\theta$ est l’unique homomorphisme d’algèbres unifères satisfaisant à cette dernière condition. Ceci montre que le couple $(U(L(X)), \sigma | X)$ est une solution du même problème universel que $A(X)$; prenant pour $\varphi$ l’injection canonique de $X$ dans $A(X)$, on en déduit que $\beta$ est un isomorphisme, ce qui démontre $b$.

Enfin, comme $L(X)$ est un $K$-module libre (§ 2, n° 11, cor. du th. 1), $\sigma$ est injectif et $\sigma(L(X))$ est un sous-module facteur direct de $U(L(X))$ (chap. I, § 2, n° 7, cor. 3 du th. 1). D’après $b$, cela démontre $a$.

#### Corollaire 1 {#lie-ii-s3-thm-1-cor-1 .statement}

Il existe sur l’algèbre $A(X)$ un unique coproduit faisant de $A(X)$ une bigèbre et tel que les éléments de $X$ soient primitifs. De plus, $\beta$ est un isomorphisme de la bigèbre $U(L(X))$ sur $A(X)$ munie de cette structure de bigèbre.

Cela résulte de l’assertion b) du théorème et du fait que $X$ engendre l’algèbre unifère $A(X)$.

Dorénavant, on munit $A(X)$ de cette structure de bigèbre et *on identifie* $L(X)$ à son image par $\alpha$, c’est-à-dire *à la sous-algèbre de Lie de $A(X)$ engendrée par $X$*.

#### Corollaire 2 {#lie-ii-s3-thm-1-cor-2 .statement}

*Si $K$ est un corps de caractéristique 0, $L(X)$ est l’algèbre de Lie des éléments primitifs de $A(X)$.*
    Cela résulte du cor. 1 et du cor. de la prop. 9 du § 1, n° 5.

#### Remarque 1 {#lie-ii-s3-n1-rem-1 .statement}

Soit $K'$ un anneau commutatif contenant $K$. Si on identifie $A(X), L(X)$ et $L_{K'}(X)$ à des parties de $A_{K'}(X)$, il résulte de la partie *a)* du th. 1 la relation
$$
L(X) = L_{K'}(X) \cap A(X).
$$
2) Le cor. 2 du th. 1 reste valable si on suppose seulement que le groupe additif de l’anneau $K$ est sans torsion. En effet, supposons d’abord $K = \mathbf{Z}$; tout élément primitif de $A(X)$ est un élément primitif de $A_{\mathbf{Q}}(X)$, donc est dans $L_{\mathbf{Q}}(X) \cap A(X) = L(X)$ (cor. 2 et formule (1)). Dans le cas général, $K$ est plat sur $\mathbf{Z}$ et on applique la *Remarque* 2 du § 1, n° 2 et la prop. 3 du § 2, n° 5.
3) Soient $\Delta$ un monoïde commutatif, $\varphi_0$ une application de $X$ dans $\Delta$, $\varphi : Mo(X) \to \Delta$ l’homomorphisme de monoïde associé; si on munit $A(X)$ de la graduation $(A^\delta(X))_{\delta \in \Delta}$ définie en A, III, p. 31, *Exemple* 3 et $L(X)$ de la graduation $(L^\delta(X))_{\delta \in \Delta}$ définie au § 2, n° 6, on a aussitôt, pour $\delta \in \Delta$, $L^\delta(X) \subset L(X) \cap A^\delta(X)$. Comme $L$ est la somme des $L^\delta(X)$ pour $\delta \in \Delta$, et que la somme des $L(X) \cap A^\delta(X)$ pour $\delta \in \Delta$ est directe, cela entraîne
$$
L^\delta(X) = L(X) \cap A^\delta(X).
$$
4) Soit $A$ une algèbre associative unifère, et soit $t = (t_i)_{i \in I}$ une famille d’éléments de $A$. On a un diagramme

$$
\begin{array}{ccc}
L(I) & \xrightarrow{f_t} & A \\
\downarrow i & & \uparrow g_t \\
A(I)
\end{array}
$$

où $i$ est l’injection canonique, $f_t$ est l’homomorphisme d’algèbre de Lie défini par $t$ et $g_t$ l’homomorphisme d’algèbre unifère tel que $g_t(i) = t_i$ pour $i \in I$. Le diagramme est commutatif car $g_t \circ i$ et $f_t$ coïncident dans $I$. Il en résulte que, si $P \in L(I)$, l’élément $P((t_i)_{i \in I})$ défini au § 2, n° 4, coïncide avec l’élément $P((t_i)_{i \in I})$ défini en A, III, p. 24, *Exemple* 2.

### 2. Projecteur de $A^+(X)$ sur $L(X)$

Soit $\pi$ l’application linéaire de $A^+(X)$ dans $L(X)$ définie par
$$
\pi(x_1 \ldots x_n) = (\mathrm{ad}(x_1) \circ \cdots \circ \mathrm{ad}(x_{n-1}))(x_n)
$$
pour $n > 0, x_1, \ldots, x_n$ dans $X$.

#### Proposition 1 {#lie-ii-s3-prop-1 .statement}

*a)* *La restriction $\pi_0$ de $\pi$ à $L(X)$ est une dérivation de $L(X)$.*
*b)* *Pour tout entier $n \geqslant 1$ et tout $u$ dans $L^n(X)$, on a $\pi(u) = n.u$.*

*a)* Soient $E$ l’algèbre des endomorphismes du module $L(X)$ et $\theta$ l’homomorphisme de $A(X)$ dans $E$ tel que $\theta(x) = \mathrm{ad}\, x$ pour tout $x \in X$. La restriction de $\theta$ à $L(X)$ est un homomorphisme d’algèbres de Lie de $L(X)$ dans $E$, qui coïncide sur $X$ avec la représentation adjointe de $L(X)$, d’où
$$
\theta(u).v = [u, v] \quad \text{pour } u, v \text{ dans } L(X).
$$
Soient $a$ dans $A(X)$ et $b$ dans $A^+(X)$; on a
$$
\pi(a.b) = \theta(a).\pi(b).
$$
Il suffit en effet de considérer le cas $a = x_1 \ldots x_p,\ b = x_{p+1} \ldots x_{p+q}$ avec $p \geqslant 0,\ q \geqslant 1$ et $x_1, \ldots, x_{p+q}$ dans $X$; mais alors (5) résulte immédiatement de (3) puisque l’on a $\theta(x) = \mathrm{ad}\, x$ pour $x \in X$.

Soient $u$ et $v$ dans $L(X)$; d’après (4) et (5), on a
$$
\begin{align*}
\pi_0([u, v]) &= \pi(uv - vu) = \theta(u).\pi(v) - \theta(v).\pi(u) \\
&= [u, \pi(v)] - [v, \pi(u)] = [u, \pi_0(v)] + [\pi_0(u), v],
\end{align*}
$$
donc $\pi_0$ est une dérivation de $L(X)$.

*b)* Soit $\pi_1$ l’endomorphisme du module $L(X)$ qui coïncide dans $L^n(X)$ avec la multiplication par l’entier $n \geqslant 1$. La formule $[L^n(X), L^m(X)] \subset L^{n+m}(X)$ montre que $\pi_1$ est une dérivation (A, III, p. 119, *Exemple 6*). La dérivation $\pi_1 - \pi_0$ de $L(X)$ s’annule dans $X$, et comme $X$ engendre $L(X)$, on a $\pi_0 = \pi_1$, d’où *b)*.

#### Corollaire {#lie-ii-s3-n2-cor-1 .statement}

*Supposons que $K$ soit une $\mathbf{Q}$-algèbre. Soit $P$ l’application linéaire de $A^+(X)$ dans lui-même telle que*
$$
P(x_1 \ldots x_n) = \frac{1}{n} (\mathrm{ad}\, x_1 \circ \cdots \circ \mathrm{ad}\, x_{n-1})(x_n)
$$
*pour $n \geqslant 1$, et $x_1, \ldots, x_n$ dans $X$. Alors $P$ est un projecteur de $A^+(X)$ sur $L(X)$.*

L’image de $P$ est contenue dans $L(X)$. De plus, pour tout $n \geqslant 1$ et tout $u$ dans $L^n(X)$, on a $P(u) = \frac{1}{n} \pi(u)$, d’où $P(u) = u$ d’après la prop. 1. Comme $L(X) = \sum_{n \geqslant 1} L^n(X)$, on voit que la restriction de $P$ à $L(X)$ est l’identité.

(On notera que, si Card(X) $\geqslant 2$, les projecteurs P et Q *ne coïncident pas* dans $A^+(X)$. En effet, soient $x, y$ dans X, tels que $x \neq y$, et posons

$$
z = x[x, y] + [x, y]x = x^2y - yx^2.
$$

On a $Q(z) = 0$ et $P(z) = \frac{1}{3}[x, [x, y]] \neq 0$, cf. § 2, n° 10, *Exemple* et n° 11, th. 1.)

### 3. Dimension des composantes homogènes de $L(X)$

Soient X un ensemble, $\alpha$ un élément de $\mathbf{N}^{(X)}$, et d un entier $> 0$. On écrit $d|\alpha$ s’il existe un $\beta \in \mathbf{N}^{(X)}$ tel que $\alpha = d\beta$. L’élément $\beta$, qui est unique, se note alors $\alpha/d$.

#### Lemme 1 {#lie-ii-s3-lem-1 .statement}

*Soient n un entier $> 0$, $T_1, \ldots, T_n$ des indéterminées, et $u_1, \ldots, u_n$ dans $\mathbf{Z}$. Soit $(c(\alpha))_{\alpha \in \mathbf{N}^n - \{0\}}$ une famille d’éléments de $\mathbf{Z}$ telle que*

$$
1 - \sum_{i=1}^n u_i T_i = \prod_{\alpha \neq 0} (1 - T^\alpha)^{c(\alpha)}. \tag{7}
$$

*Pour tout $\alpha \in \mathbf{N}^n - \{0\}$, on a*

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!} u^{\alpha/d} \tag{8}
$$

*où $\mu$ est la fonction de Möbius* (App.).

La formule (7) est équivalente, en prenant le logarithme des deux membres (A, IV, § 6, n° 9, n° 11e édition) à:

$$
\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{\alpha \neq 0} c(\alpha) \log(1 - T^\alpha). \tag{9}
$$

Or

$$
-\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{j \geqslant 1} \frac{1}{j} \left( \sum_{i=1}^n u_i T_i \right)^j \\
= \sum_{j \geqslant 1} \frac{1}{j} \sum_{|\beta|=j} \frac{|\beta|!}{\beta!} u^\beta T^\beta \\
= \sum_{|\beta|>0} \frac{1}{|\beta|} \frac{|\beta|!}{\beta!} u^\beta T^\beta. \tag{10}
$$

D’autre part

$$(11)$$
$$
-\sum_{\alpha \neq 0} c(\alpha) \log(1 - T^\alpha) = \sum_{|\alpha| > 0, k \geq 1} \frac{1}{k} c(\alpha) T^{k\alpha}
= \sum_{|\beta| > 0, k|\beta} \frac{1}{k} c\left(\frac{\beta}{k}\right) T^\beta.
$$

Donc (7) équivaut à

$$(12)$$
$$
\sum_{k|\beta} \left| \frac{\beta}{k} \right| c\left( \frac{\beta}{k} \right) = \frac{|\beta|!}{\beta!} u^\beta \quad \text{pour tout } \beta \in \mathbf{N}^n - \{0\}.
$$

Soit $\Lambda$ l’ensemble des $(\lambda_1, \lambda_2, \ldots, \lambda_n) \in \mathbf{N}^n - \{0\}$ tels que le p.g.c.d. de $\lambda_1, \lambda_2, \ldots, \lambda_n$ soit égal à 1. Tout élément de $\mathbf{N}^n - \{0\}$ s’écrit de manière unique sous la forme $m\lambda$, où $m$ est un entier $\geq 1$ et où $\lambda \in \Lambda$. La condition (12) équivaut à

$$(13)$$
$$
\sum_{k|m} \left| \frac{m\lambda}{k} \right| c\left( \frac{m\lambda}{k} \right) = \frac{(m|\lambda|)!}{(m\lambda)!} u^{m\lambda} \quad \text{pour tout } \lambda \in \Lambda \text{ et tout } m \geq 1.
$$

D’après la formule d’inversion de Möbius (App. ), la condition (13) équivaut à

$$(14)$$
$$
|m\lambda| c(m\lambda) = \sum_{d|m} \mu(d) \frac{\left| \frac{m\lambda}{d} \right|!}{\left( \frac{m\lambda}{d} \right)!} u^{\frac{m\lambda}{d}}
$$

pour tout $\lambda \in \Lambda$ et tout $m \geq 1$.

C.Q.F.D.

#### Théorème 2 {#lie-ii-s3-thm-2 .statement}

*Soient X un ensemble fini et n = Card(X).*
    *a)* *Pour tout entier r $\geq 1$, le K-module L^r(X) est libre de rang*

$$(15)$$
$$
c(r) = \frac{1}{r} \sum_{d|r} \mu(d) n^{r/d},
$$

*où $\mu$ est la fonction de Möbius.*
    *b)* *Pour tout $\alpha \in \mathbf{N}^X - \{0\}$, le K-module L^\alpha(X) (\S 2, n° 6) est libre de rang*

$$(16)$$
$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!}.
$$

Nous savons déjà que les modules L^r(X) pour $r \in \mathbf{N}$, et L^\alpha(X) pour $\alpha \in \mathbf{N}^X$, sont libres (\S 2, n° 11, cor. du th. 1). Considérons la multigraduation $(A^\alpha(X))_{\alpha \in \mathbf{N}^X}$ de A(X) définie par l’homomorphisme canonique $\varphi$ de Mo(X) dans $\mathbf{N}^X$ (A, III, p. 31, *Exemple 3*) ; on a $A^\alpha(X) \cap L(X) = L^\alpha(X)$ d’après la *Remarque 3* du n° 1. Pour $\alpha \in \mathbf{N}^X$, le K-module A^\alpha(X) admet pour base l’ensemble des mots dans lesquels chaque lettre x de X apparaît $\alpha(x)$ fois. Soit $d(\alpha)$ le nombre de ces mots, c’est-à-dire le rang de $A^\alpha(X)$; nous allons calculer de deux manières différentes la série formelle $P((T_x)_{x \in X}) \in \mathbf{Z}[[(T_x)_{x \in X}]]$ définie par

$$
P(T) = \sum_{\alpha \in \mathbf{N}^X} d(\alpha) T^\alpha.
$$

1) On a

$$
P(T) = \sum_{m \in Mo(X)} T^{\varphi(m)} = \sum_{r=0}^\infty \sum_{x_1, \ldots, x_r} T_{x_1} \ldots T_{x_r} = \sum_{r=0}^\infty \left( \sum_{x \in X} T_x \right)^r
$$

d’où

$$
P(T) = \left( 1 - \sum_{x \in X} T_x \right)^{-1}.
$$

2) Pour tout $\alpha \in \mathbf{N}^X - \{0\}$, soit $(\ell_{\alpha,j})_{1 \leq j \leq c(\alpha)}$ une base de $L^\alpha(X)$ et munissons l’ensemble $I$ des couples $(\alpha, j)$ tels que $\alpha \in \mathbf{N}^X - \{0\}$ et $1 \leq j \leq c(\alpha)$ d’une relation d’ordre total. D’après le th. 1 du n° 1 et le th. de Poincaré–Birkhoff–Witt (chap. I, § 2, n° 7, cor. 3 du th. 1), les éléments

$$
y_m = \prod_{(\alpha, j) \in I} (\ell_{\alpha,j})^{m(\alpha,j)},
$$

l’indice $m$ parcourant $\mathbf{N}^{(I)}$, forment une base de $A(X)$. Chaque $y_m$ est de multidegré $\sum_{(\alpha, j) \in I} m(\alpha, j) \alpha$. Notons $u(m)$ ce multidegré. Il en résulte que

$$
P(T) = \sum_{m \in \mathbf{N}^{(I)}} T^{u(m)} = \sum_{m \in \mathbf{N}^{(I)}} \prod_{(\alpha, j) \in I} T^{m(\alpha,j)\alpha}
$$
$$
= \prod_{(\alpha, j) \in I} \sum_{r=0}^\infty T^{r\alpha} = \prod_{(\alpha, j) \in I} (1 - T^\alpha)^{-1},
$$

d’où enfin

$$
P(T) = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{-c(\alpha)}.
$$

En comparant (18) et (19), on obtient

$$
1 - \sum_{x \in X} T_x = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{c(\alpha)}.
$$

Le lemme 1 donne alors b).

Substituant maintenant une même indéterminée $U$ aux $T_x$ pour $x \in X$, dans la formule (20), on obtient

$$
1 - nU = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - U^{|c(\alpha)|})^{c(\alpha)} = \prod_{r > 0} (1 - U^r)^{c(r)}.
$$

En appliquant de nouveau le lemme 1, on en déduit a).

#### Exemple {#lie-ii-s3-n3-exa-1 .statement}

On a:

$$
c(1) = n, \quad c(2) = \frac{1}{2}(n^2 - n), \quad c(3) = \frac{1}{3}(n^3 - n),
c(4) = \frac{1}{4}(n^4 - n^2), \quad c(5) = \frac{1}{5}(n^5 - n), \quad c(6) = \frac{1}{6}(n^6 - n^3 - n^2 + n).
$$

#### Remarque {#lie-ii-s3-n3-rem-1 .statement}

Soit X un ensemble et soit $\alpha \in \mathbf{N}^{(X)}$; le rang du K-module libre $L^\alpha(X)$ est encore donné par la formule (16). Cela résulte aussitôt du th. 2b) et de la prop. 4 du § 2, no 6.

## EXERCICES {#lie-ii-s3-exercises}

La lettre X désigne un ensemble.

See the [exercises for § 3](exercises/s3/).
