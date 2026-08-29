---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 2
section_title: Places
lang: fr
source: ac-v-vii-fr
pdf_pages: 0091-0096, 0167-0169
extraction: ocr
subsections:
    - "no": 1
      title: Notion de morphisme pour les lois de composition non partout définies
      page: 0
      pdf_page: 91
    - "no": 2
      title: Places
      page: 0
      pdf_page: 92
    - "no": 3
      title: Places et anneaux de valuation
      page: 0
      pdf_page: 93
    - "no": 4
      title: Extension des places
      page: 0
      pdf_page: 95
    - "no": 5
      title: Caractérisation des éléments entiers au moyen des places
      page: 0
      pdf_page: 96
statements: 9
exercises: 6
content_sha256: 0e3cd49ce9b1c7f45994bc7e960e7402591e6b5e1c55dd2dff578eda3ad5b1c1
---

## § 2. Places

### 1. Notion de morphisme pour les lois de composition non partout définies

#### Définition 1 {#ac-vi-s2-def-1 .statement}

Soient $E$ et $E'$ deux ensembles munis chacun d’une loi de composition interne notée $(x, y) \to x * y$, non nécessairement partout définie. On dit qu’une application $f : E \to E'$ est un morphisme si, quels que soient $x, y$ dans $E$ tels que $f(x) * f(y)$ soit défini, le composé $x * y$ est aussi défini et l’on a:

$$
f(x * y) = f(x) * f(y).
$$

Plus brièvement, on peut dire que la formule (1) doit être vérifiée chaque fois que le membre de droite a un sens.

La notion de morphisme est distincte de celle de représentation (Alg., chap. I, § 1, no 1), où l’on exige que la formule (1) soit vérifiée chaque fois que le membre de gauche a un sens. Bien entendu, les deux notions coïncident pour les lois de composition partout définies.

#### Définition 2 {#ac-vi-s2-def-2 .statement}

Soient $E$ et $E'$ deux ensembles, munis chacun d’une famille de lois de composition internes $(x, y) \to x *_{\alpha} y$, $\alpha \in I$. On dit qu’une application $f : E \to E'$ est un morphisme si c’est un morphisme pour chacune des lois de composition $(x, y) \to x *_{\alpha} y$.

### 2. Places

Si $K$ est un corps, rappelons que l’on note $\widetilde{K}$ l’ensemble somme de $K$ et d’un élément noté $\infty$ (Alg., chap. II, 3e éd., § 9, n° 9); les lois de composition de $K$ se prolongent à $\widetilde{K}$ en posant (loc. cit.)

$$
\begin{align*}
(2)\quad a + \infty &= \infty & \text{pour} &\quad a \in K, a \neq \infty, \\
(3)\quad \infty . a = a . \infty &= \infty & \text{pour} &\quad a \in \widetilde{K}, a \neq 0.
\end{align*}
$$

Les seuls composés non définis sont donc les composés $\infty + \infty, \infty . 0$ et $0 . \infty$. D’autre part, les applications $x \to -x$ et $x \to x^{-1}$ se prolongent de même à $\widetilde{K}$ en posant $-\infty = \infty, 0^{-1} = \infty, \infty^{-1} = 0$. Nous écrirons aussi $x + (-y) = x - y$.

L’ensemble $\widetilde{K}$, dit corps projectif associé à $K$, peut être identifié à la droite projective $P_1(K)$ (loc. cit.).

#### Définition 3 {#ac-vi-s2-def-3 .statement}

Soient $K$ et $L$ deux corps. On appelle place de $K$ à valeurs dans $L$ tout morphisme $f$ de $\widetilde{K}$ dans $\widetilde{L}$ (pour l’addition et la multiplication) tel que $f(1) = 1$.

Autrement dit, si $x$ et $y$ sont des éléments de $\widetilde{K}$, et si $f(x) + f(y)$ (resp. $f(x)f(y)$) est défini, alors $x + y$ (resp. $xy$) est défini, et l’on a

$$
\begin{align*}
(4)\quad f(x + y) &= f(x) + f(y) \\
(5)\quad f(xy) &= f(x)f(y).
\end{align*}
$$

Comme $\infty + \infty$ n’est pas défini, il en est de même de $f(\infty) + f(\infty)$, ce qui montre que

$$
(6)\quad f(\infty) = \infty.
$$

De même, puisque $0 . \infty$ n’est pas défini, il en est de même de $f(0)f(\infty)$, ce qui, en vertu de (6), entraîne

$$
(7)\quad f(0) = 0.
$$

On a d’autre part

$$
(8)\quad f(a^{-1}) = f(a)^{-1} \quad \text{pour tout } a \in \widetilde{K}.
$$

En effet, si $f(a)f(a^{-1})$ est défini, $aa^{-1}$ est défini, donc égal à 1; on a alors $f(a)f(a^{-1}) = f(1) = 1$, ce qui prouve (8) dans ce cas. Si $f(a)f(a)^{-1}$ n’est pas défini, on a, soit $f(a) = 0$ et $f(a^{-1}) = \infty$, soit $f(a) = \infty$ et $f(a^{-1}) = 0$, et (8) est encore vérifiée.

On démontre de même la formule

$$
f(-a) = -f(a) \quad \text{pour tout } a \in \widetilde{K}.
$$

Des formules (8) et (9), il résulte que $f$ est aussi un morphisme pour les lois de composition $(x, y) \to x - y$ et $(x, y) \to xy^{-1}$.

Pour $x \in \widetilde{K}$, on dit que $f$ est finie en $x$ si $f(x) \neq \infty$; ceci implique $x \in K$, en vertu de (6).

Si $f : \widetilde{K} \to \widetilde{L}$ est une place, $f(\widetilde{K})$ est un sous-ensemble de $\widetilde{L}$ qui est stable pour les lois de composition $(x, y) \to x + y$, $(x, y) \to x - y$, $(x, y) \to xy$ et $(x, y) \to xy^{-1}$, et qui contient 1.

Si E est l’ensemble des éléments finis de $f(\widetilde{K})$, E est un sous-corps de L et l’on a $f(\widetilde{K}) = \overline{E}$. Par abus de langage, on dit que E est le corps des valeurs de $f$.

L’application composée de deux places est une place.

Soit $f$ un isomorphisme d’un corps K sur un sous-corps d’un corps L; prolongeons $f$ à $\widetilde{K}$ en posant $f(\infty) = \infty$. On obtient ainsi une place de K à valeurs dans L, qui est dite triviale, et qu’on identifie souvent à l’isomorphisme $f$.

### 3. Places et anneaux de valuation

#### Proposition 1 {#ac-vi-s2-prop-1 .statement}

Soient K un corps, A un anneau de valuation pour K, et $\kappa(A)$ le corps résiduel de A. Prolongeons l’application canonique de A sur $\kappa(A)$ en une application $h_A : \widetilde{K} \to (\kappa(A)) \sim$ par la formule $h_A(x) = \infty$ si $x \notin A$. L’application $h_A$ ainsi définie est une place de K dont le corps des valeurs est $\kappa(A)$.

Il est clair qu’on a $h_A(1) = 1$.

Montrons que $h_A$ est un morphisme pour l’addition. Soient $x, y$ deux éléments de $\widetilde{K}$ tels que $h_A(x) + h_A(y)$ soit défini. L’un des deux éléments $x, y$ appartient alors à A, donc $x + y$ est défini. Si $x \in A$ et $y \in A$, il est clair que

$$
h_A(x) + h_A(y) = h_A(x + y)
$$

est vérifiée. Si $x \in A$ et $y \notin A$, on a $x + y \notin A$, et les deux membres de la formule ci-dessus valent $\infty$.

Montrons enfin que $h_A$ est un morphisme pour la multiplication. Soient $x \in \overline{K}$, $y \in \overline{K}$ tels que $h_A(x)h_A(y)$ soit défini. Si $x \in A$ et $y \in A$, il est clair que $xy$ est défini, et qu’on a $h_A(x)h_A(y) = h_A(xy)$. Supposons maintenant que l’un des éléments $x, y$, par exemple $y$, n’appartienne pas à $A$; comme $h_A(y) = \infty$, on a $h_A(x) \neq 0$, c’est-à-dire $x \notin m(A)$, d’où $x^{-1} \in A$; il s’ensuit que $xy$ est défini et que $xy \notin A$, d’où $h_A(xy) = \infty = h_A(x)h_A(y)$. Ceci démontre la prop. 1.

Si $j$ est un isomorphisme de $\kappa(A)$ sur un sous-corps d’un corps $L$, $j \circ h_A : \overline{K} \to \overline{L}$ est une place de $K$ à valeurs dans $L$. Ce procédé fournit en fait toutes les places de $K$. De façon plus précise :

#### Proposition 2 {#ac-vi-s2-prop-2 .statement}

*Soient $K$ et $L$ deux corps, et $f$ une place de $K$ à valeurs dans $L$. Il existe alors un anneau de valuation $A$ pour $K$ et un isomorphisme $j$ de $\kappa(A)$ sur un sous-corps de $L$ tels que $f = j \circ h_A$; ces conditions déterminent $A$ et $j$ de manière unique. L’anneau $A$ est l’ensemble des $x \in K$ tels que $f(x) \neq \infty$, et $m(A)$ est l’ensemble des $x \in K$ tels que $f(x) = 0$.

Si l’on a $f = j \circ h_A$, la condition $f(x) \neq \infty$ (resp. $f(x) = 0$) équivaut à la condition $h_A(x) \neq \infty$ (resp. $h_A(x) = 0$), donc à la condition $x \in A$ (resp. $x \in m(A)$). Donc $A$ est déterminé de manière unique, et, comme $h_A$ est surjectif, $j$ est aussi unique.

Soit maintenant $f$ une place quelconque de $K$ à valeurs dans $L$; notons $A$ l’ensemble des $x \in K$ tels que $f(x) \neq \infty$. Si $x \in A$ et $y \in A$, les composés $f(x) - f(y)$ et $f(x)f(y)$ sont définis et $\neq \infty$, ce qui montre que $x - y \in A$ et $xy \in A$; donc $A$ est un sous-anneau de $K$. Si $x \notin A$, on a $f(x) = \infty$, donc $f(x^{-1}) = 0$ et $x^{-1}$ appartient au noyau $m$ de l’homomorphisme $f'$ obtenu en restreignant $f$ à $A$. Inversement, si $y \in m$, on a $y^{-1} \notin A$. Ceci montre que $A$ est un anneau de valuation pour $K$, et que $m$ est son idéal maximal. Soit $j$ l’homomorphisme injectif de $\kappa(A)$ dans $L$ déduit de $f'$ par passage au quotient. On a $f(x) = j(h_A(x))$ pour tout $x \in A$, et cette égalité reste vraie pour $x \notin A$, les deux membres étant alors égaux à $\infty$.

C.Q.F.D.

La décomposition $f = j \circ h_A$ est appelée la *décomposition canonique* de la place $f$. On dit que $A$ est *l’anneau de $f$*, que $m(A)$ est *l’idéal de $f$*, et que $\kappa(A)$ est le *corps résiduel* de $f$. Pour que deux places $f : \overline{K} \to \overline{L}$ et $f' : \overline{K} \to \overline{L}'$ aient même anneau, il faut et il suffit qu’il existe un isomorphisme $s$ du corps des valeurs de $f$ sur celui de $f'$ tel que $f' = s \circ f$; on dit alors que $f$ et $f'$ sont équivalentes. On voit qu’on peut traduire tout résultat sur les anneaux de valuation en un résultat sur les places, et inversement; c’est ce que nous ferons dans les numéros suivants.

Exemples de places. — 1) Soit K un corps. L’application identique de K est une place triviale, d’anneau K et d’idéal (0).

2) Soit $k$ un corps. Pour tout $u \in k((T))^\sim$, posons $f(u) = \infty$ si $u \notin k[[T]]$ et définissons $f(u)$ comme étant le terme constant de $u$ si $u \in k[[T]]$. Alors $f$ est une place de $k((T))$, de corps résiduel $k$, d’anneau $k[[T]]$. En effet, $k[[T]]$ est un anneau de valuation pour $k((T))$ (§ 1, no 4, Exemple 3), et la restriction de $f$ à $k[[T]]$ s’identifie à l’homomorphisme canonique de $k[[T]]$ sur son corps résiduel.

3) Soient $k$ un corps, $a$ un élément de $k$, et A l’ensemble des $u \in k(X)$ tels que $a$ soit substituable dans $u$ (Alg., chap. IV, § 3, no 2). Si $\mathfrak{p}$ désigne l’idéal premier $(X - a)$ de $k[X]$, on a $A = k[X]_{\mathfrak{p}}$, de sorte que A est un anneau de valuation pour $k(X)$ (§ 1, no 4, prop. 2). Pour tout $u \in k(X)^\sim$, posons $f(u) = \infty$ si $u \notin A$, et $f(u) = u(a)$ si $u \in A$. Alors $f$ est une place de $k(X)$, de corps résiduel $k$ et d’anneau A; en effet la restriction de $f$ à A est un homomorphisme de A sur $k$ (Alg., chap. IV, § 3, prop. 2), de noyau $\mathfrak{p}A = m(A)$. On dit que l’élément $f(u) \in \overline{k}$ s’obtient en faisant $X = a$ dans $u$.

*4) Soient S une variété analytique complexe connexe de dimension 1, et K le corps des fonctions méromorphes sur S. Pour tout $z_0 \in S$, l’application $f \mapsto f(z_0)$ de K dans $\overline{\mathbf{C}}$ est une place de K, dont l’anneau est l’ensemble des $f \in K$ qui sont holomorphes en $z_0$, et dont l’idéal est l’ensemble des $f \in K$ qui sont nulles en $z_0$. C’est cet exemple, et d’autres analogues, qui sont à l’origine de la terminologie de « place ».*

### 4. Extension des places

#### Proposition 3 {#ac-vi-s2-prop-3 .statement}

Soient K un corps, S un sous-anneau de K, et $f$ un homomorphisme de S dans un corps algébriquement clos L. Il existe alors une place de K à valeurs dans L qui prolonge $f$.

#### Proposition 4 {#ac-vi-s2-prop-4 .statement}

Soient K un corps, f une place de K à valeurs dans un corps L, et K' une extension de K. Il existe alors une extension L' de L et une place f' de K' à valeurs dans L' qui prolonge f. Si x_1, ..., x_n sont des éléments de K' algébriquement indépendants sur K, et a_1, ..., a_n des éléments quelconques de L, on peut choisir f' de manière que f'(x_i) = a_i pour 1 \leq i \leq n.

Soient V l’anneau de f, g la restriction de f à V, et g' le prolongement de g à V[x_1, ..., x_n] tel que g'(x_i) = a_i pour 1 \leq i \leq n. Il suffit de prendre pour L' une clôture algébrique de L, et d’appliquer la prop. 3 à g' et L': on obtient une place f': \bar{K}' \to \bar{L}' qui prolonge g'; si x \in \bar{K} - V, on a x^{-1} \in m(V), d’où f'(x^{-1}) = g(x^{-1}) = 0, et f'(x) = \infty = f(x); donc f' prolonge f.

### 5. Caractérisation des éléments entiers au moyen des places

#### Proposition 5 {#ac-vi-s2-prop-5 .statement}

Soient K un corps, S un sous-anneau de K, h un homomorphisme de S dans un corps, et p le noyau de h. Pour qu’un élément x de K soit entier sur l’anneau local S_p, il faut et il suffit que toute place de K prolongeant h soit finie en x.

Si f est une place de K prolongeant h, f est finie sur S_p et nulle sur pS_p, donc l’anneau de la place f domine S_p. Réciproquement, si V est un anneau de valuation pour K qui domine S_p, V est l’anneau d’une place f dont la restriction à S est un homomorphisme ayant même noyau que h; remplaçant f par une place équivalente, on voit que V est l’anneau d’une place de K qui prolonge h. Dire que toute place de K prolongeant h est finie en x équivaut à dire que x appartient à tous les anneaux de valuation pour K qui dominent S_p. La proposition résulte alors du th. 3 du § 1, n° 3.

#### Proposition 6 {#ac-vi-s2-prop-6 .statement}

Soient K un corps, S un sous-anneau de K. Pour qu’un élément x de K soit entier sur S, il faut et il suffit que toute place de K finie sur S soit finie en x.

C’est aussi une conséquence du th. 3 du § 1, n° 3.

## EXERCICES {#ac-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
