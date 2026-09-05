---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 6
section_title: FONCTIONS SYMÉTRIQUES
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0064-0089, 0099-0104
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes symétriques
      page: 57
      pdf_page: 64
    - "no": 2
      title: Fractions rationnelles symétriques
      page: 62
      pdf_page: 69
    - "no": 3
      title: Séries formelles symétriques
      page: 63
      pdf_page: 70
    - "no": 4
      title: Sommes de puissances
      page: 65
      pdf_page: 72
    - "no": 5
      title: Fonctions symétriques des racines d’un polynôme
      page: 67
      pdf_page: 74
    - "no": 6
      title: Résultant
      page: 71
      pdf_page: 78
    - "no": 7
      title: Discriminant
      page: 76
      pdf_page: 83
statements: 46
exercises: 7
content_sha256: 5159b1b30c3ac692aa8536a5f74fcbb2499ef16d5f320af8e43374358b2d23f7
---

## § 6. FONCTIONS SYMÉTRIQUES

### 1. Polynômes symétriques

Soit $n$ un entier positif. Pour toute permutation $\sigma \in \mathfrak{S}_n$, soit $\varphi_\sigma$ l’automorphisme de la $A$-algèbre $A[X_1, ..., X_n]$ qui envoie $X_i$ sur $X_{\sigma(i)}$ pour $1 \leq i \leq n$. Il est clair que $\sigma \mapsto \varphi_\sigma$ est un homomorphisme de $\mathfrak{S}_n$ dans le groupe des automorphismes de $A[X_1, ..., X_n]$. On pose $\sigma f = \varphi_\sigma(f)$ pour $\sigma \in \mathfrak{S}_n$ et $f \in A[X_1, ..., X_n]$. On dit que le polynôme $f$ est symétrique si l’on a $\sigma f = f$ pour tout $\sigma \in \mathfrak{S}_n$; les polynômes symétriques forment une sous-algèbre unifère graduée de $A[X_1, ..., X_n]$; on la notera $A[X_1, ..., X_n]^{\text{sym}}$ dans la suite de ce paragraphe.

Pour tout entier positif $k$, notons $\mathfrak{P}_k$ l’ensemble des parties à $k$ éléments de l’ensemble $\{1, 2, ..., n\}$, et posons
$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i .
$$
Lorsqu’il convient de préciser l’entier $n$, on écrit $s_{k,n}$ pour $s_k$. On a en particulier
$$
\begin{align*}
s_0 &= 1 \\
s_1 &= \sum_{1 \leq i \leq n} X_i \\
s_2 &= \sum_{1 \leq i < j \leq n} X_i X_j \\
&\cdots \\
s_n &= X_1 \ldots X_n
\end{align*}
$$
et $s_k = 0$ pour $k > n$. Il est clair que $s_k$ est un polynôme symétrique homogène de degré $k$; on l’appelle le polynôme symétrique élémentaire de degré $k$.

Dans l’anneau $A[X_1, ..., X_n, U, V]$, on a la relation

$$
(2) \quad \prod_{i=1}^n (U + V X_i) = \sum_{k=0}^n U^{n-k} V^k s_k ;
$$

par des substitutions convenables, on en déduit les relations

$$
(3) \quad \prod_{i=1}^n (1 + T X_i) = \sum_{k=0}^n s_k T^k ,
$$
$$
(4) \quad \prod_{i=1}^n (X - X_i) = \sum_{k=0}^n (-1)^{n-k} s_{n-k} X^k .
$$

#### Théorème 1 {#alg-iv-s6-thm-1 .statement}

*Posons* $E = A[X_1, ..., X_n]$ *et* $S = A[X_1, ..., X_n]^{\text{sym}}$.

a) *La* $A$-*algèbre* $S$ *des polynômes symétriques est engendrée par* $s_1, ..., s_n$.

b) *Les éléments* $s_1, ..., s_n$ *de* $E$ *sont algébriquement indépendants sur* $A$ *(IV, p. 4)*.

c) *La famille des monômes* $X^\nu = X_1^{\nu(1)} ... X_n^{\nu(n)}$ *tels que* $0 \leq \nu(i) < i$ *pour* $1 \leq i \leq n$ *est une base du* $S$*-module* $E$. *En particulier,* $E$ *est un* $S$*-module libre de rang* $n!$.

Nous démontrerons le théorème par récurrence sur $n$, le cas $n = 0$ étant trivial. Posons $B = A[X_n]$ et notons $s'_k$ le polynôme symétrique élémentaire de degré $k$ en $X_1, ..., X_{n-1}$; on a donc $B[X_1, ..., X_{n-1}] = A[X_1, ..., X_n]$. Si l’on remplace $n$ par $n-1$ et $A$ par $B$ dans l’énoncé du théorème 1, on peut formuler ainsi l’hypothèse de récurrence :

(A) *La* $B$*-algèbre* $S'$ *des polynômes* $f \in A[X_1, ..., X_n]$ *invariants par toutes les permutations de* $X_1, ..., X_{n-1}$ *est engendrée par* $s'_1, ..., s'_{n-1}$.

(B) *Les éléments* $s'_1, ..., s'_{n-1}$ *de* $E$ *sont algébriquement indépendants sur* $B$.

(C) *La famille des monômes* $X_1^{\nu(1)} ... X_{n-1}^{\nu(n-1)}$ *tels que* $0 \leq \nu(i) < i$ *pour* $1 \leq i \leq n-1$ *est une base du* $S'$*-module* $E$.

On a la relation évidente

$$
(5) \quad s_k = s'_k + s'_{k-1} X_n \quad (1 \leq k \leq n-1),
$$

d’où l’on déduit par récurrence sur $k$

$$
(6) \quad s'_k = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s'_i X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

On a $S \subset S'$ donc $s_1, ..., s_n$ appartiennent à $S'$; d’après (A) et la formule (6), la $B$*-algèbre* $S'$ *est donc engendrée par* $s_1, ..., s_{n-1}$.

D’après (B), il existe un endomorphisme $u$ de la $B$*-algèbre* $S'$ *tel que*

$$
(7) \quad u(s'_k) = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s'_i X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

D’après (5), on a $u(s_k) = u(s'_k) + u(s'_{k-1}) X_n$, d’où $u(s_k) = s'_k$ par un calcul facile.

Soit $P \in B[Y_1, ..., Y_{n-1}]$; de $P(s_1, ..., s_{n-1}) = 0$, on déduit alors

$$
0 = u(P(s_1, ..., s_{n-1})) = P(s'_1, ..., s'_{n-1}) ,
$$

d’où $P = 0$ d’après (B). Par suite, la B-algèbre $S'$ est engendrée par les éléments algébriquement indépendants $s_1, ..., s_{n-1}$. On peut reformuler cette propriété comme suit :

(D) *La A-algèbre S' est engendrée par les éléments algébriquement indépendants $s_1, ..., s_{n-1}, X_n$*.

On peut donc identifier $S'$ à l’anneau de polynômes $C[X_n]$, où $C$ est la sous-A-algèbre de E engendrée par $s_1, ..., s_{n-1}$.

*Prouvons a).* Soit $f \in S$ un polynôme symétrique homogène de degré $m$. On a $f \in S' = C[X_n]$ et il existe donc un élément $g = P(s_1, ..., s_{n-1})$ de $C$, homogène de degré $m$ en $X_1, ..., X_n$, tel que $f - g$ soit divisible par $X_n$. Comme $f - g$ est symétrique, chacun de ses termes est aussi divisible par $X_1, ..., X_{n-1}$, donc $f - g$ est divisible par $s_n = X_1 ... X_n$. Autrement dit, il existe $h \in S$ tel que $f = g + h s_n$, d’où $\deg h < m$. Par récurrence sur $m$, on en déduit que $f$ appartient à

$$
C[s_n]_E = A[s_1, ..., s_{n-1}, s_n]_E .
$$

On a ainsi prouvé que la A-algèbre S est engendrée par $s_1, ..., s_n$.

*Prouvons b).* Si l’on substitue $X_n$ à $X$ dans (4), on trouve

$$
(-1)^{n+1} s_n = X_n^n + \sum_{k=1}^{n-1} (-1)^{n-k} s_{n-k} X_n^k ;
$$

autrement dit, $(-1)^{n+1} s_n$ est un polynôme unitaire en $X_n$, de degré $n$, à coefficients dans $C$. D’après IV, p. 10, on a donc la propriété suivante :

(E) *L’homomorphisme $\varphi$ de C-algèbres de $C[T]$ dans $C[X_n] = S'$ qui transforme T en $s_n$ est injectif, et $S'$ est un module libre sur l’image de $\varphi$, de base $(1, X_n, ..., X_n^{n-1})$*.

Les éléments $s_1, ..., s_{n-1}$ de $C$ sont algébriquement indépendants sur $A$ d’après (D) ; l’injectivité de $\varphi$ signifie donc que $s_1, ..., s_{n-1}, s_n$ sont algébriquement indépendants sur $A$, d’où *b)*.

*Prouvons c).* L’image de $\varphi$ est égale à $C[s_n]_E = S$, donc d’après (E), $S'$ est un module libre sur $S$, de base $(1, X_n, ..., X_n^{n-1})$. L’assertion *c)* résulte alors de l’hypothèse de récurrence (C) et de la prop. 25 de II, p. 31.

C.Q.F.D.

Soit $f$ un polynôme symétrique en $X_1, ..., X_n$, homogène de degré $m$. D’après le th. 1 (IV, p. 58), il existe un polynôme $Q \in A[Y_1, ..., Y_n]$ tel que $f = Q(s_1, ..., s_n)$. La démonstration précédente fournit un *procédé de calcul explicite* pour $Q$, par double récurrence sur $n$ et $m$. En effet, on a vu qu’il existe un polynôme $P \in A[Y_1, ..., Y_{n-1}]$ et un polynôme $h$ symétrique en $X_1, ..., X_n$, homogène de degré $m - n$, tels que

(8)
$$
f = P(s_1, ..., s_{n-1}) + s_n h .
$$

Pour tout polynôme $u \in A[X_1, ..., X_n]$, posons

$$
u'(X_1, ..., X_{n-1}) = u(X_1, ..., X_{n-1}, 0) .
$$

Alors $s'_1, \ldots, s'_{n-1}$ sont les polynômes symétriques élémentaires en $X_1, \ldots, X_{n-1}$, et la formule (8) entraîne

$$
f' = P(s'_1, \ldots, s'_{n-1}) .
$$

La détermination de $P$ est donc ramenée à un calcul sur les polynômes symétriques à $n - 1$ indéterminées, et $h$ s’en déduit par (8).

Illustrons la méthode sur deux exemples.
Exemples. — 1) Soient $n = 3$ et

$$
f = X_1^2(X_2 + X_3) + X_2^2(X_3 + X_1) + X_3^2(X_1 + X_2) .
$$

On a

$$
f' = X_1^2X_2 + X_1X_2^2 = X_1X_2(X_1 + X_2) = s'_1s'_2 .
$$

Formons alors $g = f - s_1s_2$; on a

$$
g = f - (X_1 + X_2 + X_3)(X_1X_2 + X_1X_3 + X_2X_3) = -3X_1X_2X_3 ,
$$

d’où finalement

$$
f = s_1s_2 - 3s_3 .
$$

2) Soit encore $n = 3$; posons $p = X_1^3 + X_2^3 + X_3^3$.
On a $p(X_1, 0, 0) = X_1^3 = s_1(X_1, 0, 0)^3$. Posant $q = p - s_1^3$, on obtient aussitôt

$$
q = -3f - 6X_1X_2X_3 = -3s_1s_2 + 3s_3
$$

et finalement

$$
p = s_1^3 - 3s_1s_2 + 3s_3 .
$$

Soient $S_1, \ldots, S_n$ des indéterminées. Nous munirons l’algèbre de polynômes $A[S_1, \ldots, S_n]$ de la graduation de type $\mathbf{N}$ pour laquelle $S_k$ est de poids $k$ pour $1 \leq k \leq n$ (IV, p. 3); nous munirons $A[X_1, \ldots, X_n]$ de la graduation ordinaire. Pour $1 \leq k \leq n$, le polynôme symétrique élémentaire $s_{k,n}$ en $X_1, \ldots, X_n$ est homogène de degré $k$. D’après le th. 1 (IV, p. 58), l’application $g \mapsto g(s_{1,n}, \ldots, s_{n,n})$ est donc un isomorphisme d’algèbres graduées

$$
\varphi_n : A[S_1, \ldots, S_n] \to A[X_1, \ldots, X_n]^{\text{sym}} .
$$

Soit $m$ un entier tel que $0 \leq m \leq n$. Pour tout entier $k$ tel que $1 \leq k \leq m$, on a

$$
s_{k,m}(X_1, \ldots, X_m) = s_{k,n}(X_1, \ldots, X_m, 0, \ldots, 0)
$$

d’après la définition (1) (IV, p. 57), de $s_k$. Par suite, le diagramme suivant

$$
\begin{array}{ccc}
A[S_1, \ldots, S_m] & \xrightarrow{j} & A[S_1, \ldots, S_n] \\
\downarrow \varphi_m & & \downarrow \varphi_n \\
A[X_1, \ldots, X_m]^{\text{sym}} & \xleftarrow{p} & A[X_1, \ldots, X_n]^{\text{sym}}
\end{array}
$$

(ou $j$ désigne l’inclusion canonique, et $p$ l’homomorphisme

$$
g \mapsto g(X_1, \ldots, X_m, 0, \ldots, 0))
$$

est commutatif.

#### Proposition 1 {#alg-iv-s6-prop-1 .statement}

Pour tout couple d’entiers positifs k, n, soit S_k^{(n)} le A-module formé des polynômes symétriques en X_1, ..., X_n, homogènes de degré k. Si l’entier m satisfait à 0 ≤ k ≤ m ≤ n, l’application f ↦ f(X_1, ..., X_m, 0, ..., 0) est un isomorphisme de S_k^{(n)} sur S_k^{(m)}.

D’après la commutativité du diagramme (10), il suffit de prouver que tout polynôme isobare de poids k en S_1, ..., S_n ne dépend que de S_1, ..., S_m sous les hypothèses 0 ≤ k ≤ m ≤ n. Or le poids d’un monôme S_1^{\alpha(1)} ... S_n^{\alpha(n)} est égal à l’entier $\alpha(1) + 2\alpha(2) + \cdots + n\alpha(n)$; comme les entiers $\alpha(1), ..., \alpha(n)$ sont positifs, la relation
$$
\alpha(1) + 2\alpha(2) + \cdots + n\alpha(n) = k \leq n
$$
entraîne $\alpha(j) = 0$ pour $k < j \leq n$, d’où notre assertion.

#### Exemple 3 {#alg-iv-s6-n1-exa-3 .statement}

D’après l’exemple 2 de IV, p. 60, et la prop. 1 ci-dessus, on a donc
$$
\sum_{i=1}^n X_i^3 = s_{1,n}^3 - 3s_{1,n}s_{2,n} + 3s_{3,n}
$$
pour tout entier $n \geq 3$. La commutativité du diagramme (10) donne par ailleurs les formules
$$
X_1^3 + X_2^3 = s_{1,2}^3 - 3s_{1,2}s_{2,2},
$$
$$
X_1^3 = s_{1,1}^3.
$$

#### Remarque {#alg-iv-s6-n1-rem-1 .statement}

Soient n et k deux entiers positifs. On note $\Delta_{k,n}$ l’ensemble des éléments de longueur k dans $\mathbf{N}^n$; de plus, on munit $\Delta_{k,n}$ de la relation d’ordre, notée $\alpha \leq \beta$, induite par l’ordre lexicographique sur $\mathbf{N}^n$ (E, III, p. 23), et l’on définit une action du groupe $\mathfrak{S}_n$ sur $\mathbf{N}^n$ par $(\sigma \alpha)(i) = \alpha(\sigma^{-1}(i))$ pour $\sigma \in \mathfrak{S}_n, \alpha \in \mathbf{N}^n$ et $1 \leq i \leq n$. Par ailleurs, notons $D_k$ l’ensemble des éléments $\alpha = (\alpha(1), ..., \alpha(k))$ de $\mathbf{N}^k$ tels que
$$
\alpha(1) \geq \alpha(2) \geq \cdots \geq \alpha(k), \quad \alpha(1) + \cdots + \alpha(k) = k.
$$

Supposons qu’on ait $k \leq n$ et identifions $\mathbf{N}^k$ à une partie de $\mathbf{N}^n$ par l’application $(\alpha(1), ..., \alpha(k)) \mapsto (\alpha(1), ..., \alpha(k), 0, ..., 0)$. Alors, $D_k$ se compose des éléments $\alpha$ de $\Delta_{k,n}$ tels que $\sigma \alpha \leq \alpha$ pour tout $\sigma \in \mathfrak{S}_n$. Par suite, toute orbite du groupe $\mathfrak{S}_n$ dans $\Delta_{k,n}$ contient un unique élément de $D_k$. Pour tout $\alpha \in D_k$, soit $O(\alpha)$ l’orbite de $\alpha$ dans $\Delta_{k,n}$ pour l’opération de $\mathfrak{S}_n$; posons
$$
\text{M}(\alpha) = \sum_{\beta \in O(\alpha)} X^\beta.
$$
Il résulte du lemme 1 de IV, p. 44, que la famille $(\text{M}(\alpha))_{\alpha \in D_k}$ est une base du A-module $S_k^{(n)}$.

Pour tout $\alpha \in D_k$, posons
$$
S(\alpha) = \prod_{i=1}^k s_i^{\alpha(i) - \alpha(i+1)} \quad \text{(en convenant que } \alpha(k+1) = 0 \text{)} ;
$$

comme on a $\sum_{i=1}^{k} i \cdot (\alpha(i) - \alpha(i+1)) = \sum_{i=1}^{k} \alpha(i) = k$, le polynôme symétrique $S(\alpha)$ est homogène de degré $k$. Il résulte immédiatement du théorème 1 (IV, p. 58) que la famille $(S(\alpha))_{\alpha \in D_k}$ est une base du A-module $S_k^{(n)}$.

Soient $\alpha, \beta$ dans $D_k$. Soit $c_{\alpha \beta}$ le coefficient du monôme $X^\beta$ dans le polynôme $S(\alpha)$ défini par (12) dans le cas $A = \mathbf{Z}$ et $k = n$. C’est donc un entier positif, indépendant de l’anneau $A$ et de l’entier $n$. D’après la formule (9) (IV, p. 60), on a alors

$$
S(\alpha) = \sum_{\beta \in D_k} c_{\alpha \beta} \cdot M(\beta) \quad (\alpha \in D_k).
$$

On peut montrer (cf. IV, p. 94, exerc. 13) que la matrice $C = (c_{\alpha \beta})_{\alpha, \beta \in D_k}$ est telle que $c_{\alpha \alpha} = 1$ et $c_{\alpha \beta} = 0$ pour $\alpha < \beta$; généralisant la terminologie introduite dans II, p. 151, on peut dire que C appartient au groupe trigonal strict inférieur. Il en est donc de même de la matrice D inverse de C. On trouvera dans la Table (IV, p. 96-97) la valeur des matrices C et D lorsque $2 \leq k \leq 5$.

Supposons maintenant qu’on ait $n < k$ et identifions $\mathbf{N}^n$ à une partie de $\mathbf{N}^k$ par l’application $(\alpha(1), \ldots, \alpha(n)) \mapsto (\alpha(1), \ldots, \alpha(n), 0, \ldots, 0)$. Pour tout $\alpha$ dans $D_k \cap \mathbf{N}^n$, on note encore $0(\alpha)$ l’orbite de $\alpha$ dans $\Delta_{k,n}$ pour l’opération de $\mathfrak{S}_n$, et l’on définit $M(\alpha)$ par (11). On définit encore $S(\alpha)$ par la formule (12). Alors les familles $(M(\alpha))_{\alpha \in D_k \cap \mathbf{N}^n}$ et $(S(\alpha))_{\alpha \in D_k \cap \mathbf{N}^n}$ sont des bases du A-module $S_k^{(n)}$. D’après la formule (9) de IV, p. 60, on a une formule analogue à (13), où l’on remplace $D_k$ par $D_k \cap \mathbf{N}^n$, avec les mêmes entiers $c_{\alpha \beta}$.

#### Exemple 4 {#alg-iv-s6-n1-exa-4 .statement}

D’après l’exemple 3 de IV, p. 61, on a

$$
M(3, 0, 0) = S(3, 0, 0) - 3S(2, 1, 0) + 3S(1, 1, 1)
$$

pour tout entier $n \geq 3$, et donc

$$
M(3, 0) = S(3, 0) - 3S(2, 1)
$$

pour $n = 2$.

### 2. Fractions rationnelles symétriques

Soient $K$ un corps commutatif, $X_1, X_2, \ldots, X_n$ des indéterminées. Pour tout $\sigma \in \mathfrak{S}_n$, nous avons défini au no 1 (IV, p. 57) un automorphisme $\varphi_\sigma$ de $K[X_1, X_2, \ldots, X_n]$. Cet automorphisme se prolonge de manière unique en un automorphisme $\psi_\sigma$ du corps $K(X_1, \ldots, X_n)$, et $\sigma \mapsto \psi_\sigma$ est un homomorphisme injectif de $\mathfrak{S}_n$ dans le groupe des automorphismes de $K(X_1, \ldots, X_n)$. Pour tout $f \in K(X_1, \ldots, X_n)$, on a $(\psi_\sigma f)(X_1, \ldots, X_n) = f(X_{\sigma(1)}, \ldots, X_{\sigma(n)})$. Les fractions rationnelles $f$ telles que $\psi_\sigma(f) = f$ pour tout $\sigma \in \mathfrak{S}_n$ sont appelées fractions rationnelles symétriques. L’ensemble des fractions rationnelles symétriques en $X_1, \ldots, X_n$ est un sous-corps de $K(X_1, \ldots, X_n)$.

#### Proposition 2 {#alg-iv-s6-prop-2 .statement}

Le corps des fractions rationnelles symétriques en $X_1, \ldots, X_n$ est le corps des fractions de l’anneau des polynômes symétriques en $X_1, \ldots, X_n$.

Soit $f \in K(X_1, \ldots, X_n)$ une fraction rationnelle symétrique.

Soient $u_1, v_1$ deux éléments de $K[X_1, ..., X_n]$ tels que $f = \frac{u_1}{v_1}$. Posons $v = \prod_{\sigma \in S_n} \psi_\sigma(v_1) \in K[X_1, ..., X_n]$, et $u = vf \in K[X_1, ..., X_n]$. Alors $v$ est symétrique, donc $u$ est symétrique puisque $f$ l’est, et l’on a $f = \frac{u}{v}$, d’où la proposition.

#### Corollaire {#alg-iv-s6-n2-cor-1 .statement}

*Soient $s_1, s_2, ..., s_n$ les polynômes symétriques élémentaires en $X_1, ..., X_n$. Pour toute fraction rationnelle $g \in K(S_1, S_2, ..., S_n)$, la suite $(s_1, s_2, ..., s_n)$ est substituable dans $g$, et l’application $g \mapsto g(s_1, s_2, ..., s_n)$ est un isomorphisme de $K(S_1, S_2, ..., S_n)$ sur le corps des fractions rationnelles symétriques en $X_1, ..., X_n$.*
Cela résulte de la prop. 2 et du th. 1 de IV, p. 58.

### 3. Séries formelles symétriques

Soient I un ensemble, $X = (X_i)_{i \in I}$ une famille d’indéterminées et $A[[X]]$ l’algèbre de séries formelles en les $X_i$. Pour toute permutation $\sigma \in S_I$, il existe un unique automorphisme continu $\varphi_\sigma$ de l’algèbre $A[[X]]$ qui applique $X_i$ sur $X_{\sigma(i)}$ pour tout $i \in I$ (IV, p. 26, prop. 4) ; il est clair que $\sigma \mapsto \varphi_\sigma$ est un homomorphisme de $S_I$ dans le groupe des automorphismes continus de l’algèbre $A[[X]]$. Soit $f \in A[[X]]$ une série formelle ; on pose $\sigma f = \varphi_\sigma(f)$, et l’on dit que la série formelle $f$ est *symétrique* si l’on a $\sigma f = f$ pour tout $\sigma \in S_I$. Les séries formelles symétriques forment une sous-algèbre fermée de $A[[X]]$, qu’on note $A[[X]]^{\text{sym}}$ et qu’on munit de la topologie induite par celle de $A[[X]]$.

Soit T une indéterminée. Dans l’anneau de séries formelles $A[[X, T]]$, la famille $(X_i T)_{i \in I}$ est sommable, donc la famille $(1 + X_i T)_{i \in I}$ est multipliable (IV, p. 25, prop. 2) ; de plus, on a

$$
\prod_{i \in I} (1 + X_i T) = 1 + \sum_{k \geq 1} s_k T^k,
$$

où la série formelle $s_k \in A[[X]]$ est définie par

$$
s_k = \sum_{H \in \mathfrak{P}_k} (\prod_{i \in H} X_i) \quad (k \geq 1)
$$

(on note $\mathfrak{P}_k$ l’ensemble des parties finies à $k$ éléments de I). On a en particulier $s_1 = \sum_{i \in I} X_i$. Lorsque I est fini à $n$ éléments, on a $s_k = 0$ pour $k > n$ ; plus précisément, si $I = \{1, ..., n\}$, la série formelle $s_k$ n’est autre que le polynôme symétrique élémentaire de degré $k$ en $X_1, ..., X_n$.

Soit $S = (S_k)_{k \geq 1}$ une suite d’indéterminées. Comme la série formelle $s_k$ est d’ordre $\geq k$, et appartient à $A[[X]]^{\text{sym}}$, les conditions a) et b) de la prop. 4 de IV, p. 26, sont satisfaites avec $E = A[[X]]^{\text{sym}}$; il existe donc un unique homomorphisme continu de $A$-algèbres

$$
\varphi_I : A[[S]] \to A[[X]]^{\text{sym}}
$$

tel que $\varphi_I(S_k) = s_k$ pour tout entier $k \geq 1$.

**Théorème 2. — a)** *Si I est un ensemble fini à n éléments, $\varphi_1$ induit un isomorphisme bicontinu de $A[[S_1, ..., S_n]]$ sur $A[[X]]^{sym}$.*

*b)* *Si I est infini, $\varphi_1$ est un isomorphisme bicontinu de $A[[S]]$ sur $A[[X]]^{sym}$.*

Dans le cas a), on pose $B = A[[S_1, ..., S_n]]$ et on munit cette algèbre de la topologie induite par celle de $A[[S]]$; on note aussi $\psi_1$ la restriction de $\varphi_1$ à B. Dans le cas b), on pose $B = A[[S]]$ et $\psi_1 = \varphi_1$. On munit l’algèbre de polynômes $A[S]$ de la graduation de type $\mathbf{N}$ pour laquelle $S_k$ est de poids $k$ pour tout entier $k \geqslant 1$.

*Lemme 1. — Soient J une partie finie de I, r un entier tel que Card J $\geqslant r$, et f une série formelle symétrique homogène de degré r en les $X_i$ ($i \in I$). Soit $\overline{f}$ la série formelle obtenue en substituant 0 à $X_i$ pour tout i dans I — J. Si $\overline{f} = 0$, on a $f = 0$.

Posons $f = \sum_{|\alpha|=r} a_\alpha X^\alpha$ (où $|\alpha|$ est la longueur $\sum_{i \in I} \alpha_i$ du multiindice $\alpha = (\alpha_i)_{i \in I}$).
Soit $\alpha$ un multiindice de longueur $r$, et soit J’ le support de $\alpha$ (ensemble des $i \in I$ tels que $\alpha_i \neq 0$). On a Card J’ $\leqslant r$, donc il existe une permutation $\sigma \in \mathfrak{S}_I$ telle que $\sigma(J') \subset J$. Posons $\beta_i = \alpha_{\sigma^{-1}(i)}$ pour $i \in I$. Le monôme $X^\beta = \prod_{i \in I} X_{\sigma(i)}^{\alpha_i}$ ne dépend que des indéterminées $X_j$ ($j \in J$), d’où $a_\beta = 0$ d’après l’hypothèse $\overline{f} = 0$. Comme $f$ est symétrique, on a $a_\alpha = a_\beta$. Vu l’arbitraire de $\alpha$, on a donc $f = 0$.

*Lemme 2. — Soit f une série formelle symétrique homogène de degré r en les $X_i$ ($i \in I$). Il existe un unique polynôme $P \in B \cap A[S]$, isobare de poids r, tel que $f = \psi_1(P)$.

Le cas où I est fini résulte du th. 1 (IV, p. 58).

Supposons I infini et choisissons une partie finie J de I à r éléments. Reprenons les notations du lemme 1. Remarquons que tout polynôme isobare de poids r en les $S_n$ ($n \geqslant 1$) ne dépend que de $S_1, ..., S_r$, et que $\overline{s}_1, ..., \overline{s}_r$ sont les polynômes symétriques élémentaires en les r indéterminées $X_j$ ($j \in J$). Si P est un polynôme isobare de poids r en les $S_n$, et $h = f - \psi_1(P)$, on a $\overline{h} = \overline{f} - P(\overline{s}_1, ..., \overline{s}_r)$, et le lemme 1 montre que la relation $f = \psi_1(P)$ équivaut à $\overline{f} = P(\overline{s}_1, ..., \overline{s}_r)$. D’après le th. 1 (IV, p. 58), il existe un unique polynôme $P \in A[S]$ isobare de poids r tel que $\overline{f} = P(\overline{s}_1, ..., \overline{s}_r)$, d’où le lemme.

*Lemme 3. — Pour tout entier $m \geqslant 0$, soit $c_m$ l’idéal de l’algèbre $A[[X]]^{sym}$ formé des séries formelles symétriques d’ordre $\geqslant m$. La suite $(c_m)_{m \geqslant 0}$ est un système fondamental de voisinages de 0 dans $A[[X]]^{sym}$.

Le lemme est immédiat si I est fini. Supposons désormais I infini. Pour toute partie finie J de I, à m éléments, on note $\tilde{J}$ l’ensemble des éléments de $\mathbf{N}^{(I)}$ de longueur $< m$ et de support contenu dans J. On note aussi $\alpha'_j$ l’ensemble des séries formelles ne contenant aucun terme de la forme $aX^\alpha$ avec $\alpha \in \tilde{J}$. Comme $\tilde{J}$ est une partie finie de $\mathbf{N}^{(I)}$, et que toute partie finie de $\mathbf{N}^{(I)}$ est contenue dans un ensemble de la forme $\tilde{J}$, la famille $(\alpha'_j)$ est une base de voisinages de 0 dans $A[[X]]$ (IV, p. 24). Or le lemme 1 entraîne la relation $\alpha'_j \cap A[[X]]^{sym} = c_m$ pour toute partie J à m éléments. Ceci prouve le lemme 3.

Comme il n’y a qu’un nombre fini de monômes d’un poids donné en les $S_k$, toute série formelle $f \in B$ s’écrit de manière unique sous la forme $f = \sum_{r \geq 0} P_r$, où $P_r$ est un polynôme isobare de poids $r$ dans $B \cap A[S]$. Pour tout entier $m \geq 0$, soit $b_m$ l’idéal de $B$ formé des séries formelles du type précédent telles que $P_r = 0$ pour $0 \leq r < m$. La suite $(b_m)_{m \geq 0}$ est une base de voisinages de 0 dans $B$.

Avec les notations précédentes, $\psi_1(P_r)$ est une série formelle symétrique en les $X_i$, homogène de degré $r$, et c’est donc la composante homogène de degré $r$ de $\psi_1(f)$. Le lemme 2 montre que $\psi_1$ est un isomorphisme d’algèbres de $B$ sur $A[[X]]^{\text{sym}}$, transformant $b_m$ en $c_m$ pour tout entier $m \geq 0$; le lemme 3 montre alors que $\psi_1$ est bicontinu.

C.Q.F.D.

### 4. Sommes de puissances

On note encore $X = (X_i)_{i \in I}$ une famille d’indéterminées. Les séries formelles symétriques $s_k$ sont définies comme plus haut, par

$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i \quad (k \geq 1),
$$

où $\mathfrak{P}_k$ est l’ensemble des parties finies à $k$ éléments de $I$. On pose aussi

$$
p_k = \sum_{i \in I} X_i^k \quad (k \geq 1).
$$

C’est une série formelle symétrique homogène de degré $k$.

#### Lemme 4 (« Relations de Newton ») {#alg-iv-s6-lem-4 .statement}

Pour tout entier $d \geq 1$, on a

$$
p_d = \sum_{k=1}^{d-1} (-1)^{k-1} s_k p_{d-k} + (-1)^{d+1} ds_d.
$$

Définissons une dérivation continue $\Delta$ dans $A[[X]]$ par $\Delta(u) = \sum_{n \geq 0} n u_n$, où, pour tout $u$ dans $A[[X]]$, $u_n$ est la composante homogène de degré $n$ de $u$. D’après (16) et la prop. 2 de IV, p. 25, on a

$$
1 + \sum_{k \geq 1} s_k = \prod_{i \in I} (1 + X_i).
$$

D’après la prop. 9 de IV, p. 32, on a donc

$$
(\sum_{k \geq 1} k s_k) \cdot (1 + \sum_{k \geq 1} s_k)^{-1} = \sum_{i \in I} \Delta(X_i)/(1 + X_i).
$$

On a $\Delta(X_i) = X_i$ et $X_i/(1 + X_i) = \sum_{k \geq 1} (-1)^{k-1} X_i^k$. Le second membre de (20) est donc égal à $\sum_{k \geq 1} (-1)^{k-1} p_k$. D’après (20), on a alors

$$
\sum_{k \geq 1} k s_k = (1 + \sum_{k \geq 1} s_k) \cdot (\sum_{k \geq 1} (-1)^{k-1} p_k)
$$

et le lemme 4 en résulte par comparaison des composantes homogènes de degré $d$.

#### Remarque {#alg-iv-s6-n4-rem-1 .statement}

Avec les notations de la démonstration précédente, on a

$$
\Delta u = \sum_{i \in I} X_i \cdot D_i(u)
$$

(IV, p. 31, cor. 1). Autrement dit, la relation d’Euler (IV, p. 8, prop. 6) s’étend aux séries formelles : si $u \in \mathbf{A}[[\mathbf{X}]]$ est homogène de degré $n$, on a

(21)

$$
n \cdot u = \sum_{i \in I} X_i \cdot D_i(u) .
$$

Lorsque $I$ est fini, à $n$ éléments, on a $s_k = 0$ pour $k > n$. Les relations de Newton s’écrivent alors sous la forme

$$
\begin{align*}
p_1 &= s_1 \\
p_2 &= s_1 p_1 - 2s_2 \\
p_3 &= s_1 p_2 - s_2 p_1 + 3s_3 \\
&\cdots \\
p_{n-1} &= s_1 p_{n-2} - s_2 p_{n-3} + \cdots + (-1)^{n-1} s_{n-2} p_1 + (-1)^n (n-1) s_{n-1} \\
p_n &= s_1 p_{n-1} - s_2 p_{n-2} + \cdots + (-1)^n s_{n-1} p_1 + (-1)^{n+1} n s_n
\end{align*}
$$

et

(22) $p_k = s_1 p_{k-1} - s_2 p_{k-2} + \cdots + (-1)^{n+1} s_n p_{k-n}$ (pour $k > n$).

Les $n$ premières relations précédentes sont valables quel que soit $I$; on en déduit par exemple

$$
p_1 = s_1 , \quad p_2 = s_1^2 - 2s_2 , \quad p_3 = s_1^3 - 3s_1 s_2 + 3s_3 .
$$

Plus généralement, soit $S = (S_n)_{n \geq 1}$ une famille d’indéterminées. Définissons par récurrence les polynômes $P_d \in \mathbf{Z}[S_1, \ldots, S_d]$ par $P_1 = S_1$ et

$$
P_d = \sum_{k=1}^{d-1} (-1)^{k-1} S_k P_{d-k} + (-1)^{d+1} d S_d \quad (d \geq 2) .
$$

On a alors les « formules universelles » $p_d = P_d(s_1, \ldots, s_d)$ valables quels que soient l’anneau $\mathbf{A}$ et la famille d’indéterminées $\mathbf{X}$.

Soit $\mathbf{P} = (P_k)_{k \geq 1}$ une suite d’indéterminées. Comme $p_k$ est homogène de degré $k$ dans $\mathbf{A}[[\mathbf{X}]]$, il existe un homomorphisme continu de $\mathbf{A}$-algèbres (et un seul)

$$
\lambda_I : \mathbf{A}[[\mathbf{P}]] \to \mathbf{A}[[\mathbf{X}]]^{\text{sym}}
$$

tel que $\lambda_1(P_k) = p_k$ pour tout entier $k \geq 1$ (IV, p. 27). Si l’on munit $P_k$ du poids $k$, $\lambda_1$ transforme un polynôme isobare de poids $n$ en les $P_k$ en une série formelle homogène de degré $n$ en les $X_i$.

**Proposition 3. — a)** *Si I est un ensemble fini à n éléments et si $n!.1$ est inversible dans $A$, $\lambda_1$ induit un isomorphisme bicontinu de $A[[P_1, ..., P_n]]$ sur $A[[X]]^{sym}$.

b) *Si I est infini et si A est une Q-algèbre, $\lambda_1$ est un isomorphisme bicontinu de $A[[P]]$ sur $A[[X]]^{sym}$.

Nous traiterons seulement le cas a), le cas b) étant tout à fait analogue.

D’après le th. 2 (IV, p. 64), on peut identifier $A[[X]]^{sym}$ à l’algèbre de séries formelles $A[[S_1, ..., S_n]]$, $S_k$ correspondant à $s_k$. D’après le lemme 4 de IV, p. 65, il existe des séries formelles $g_1, ..., g_n$ d’ordre $\geq 2$ en les indéterminées $s_1, ..., s_n$ telles que
$$
p_k = (-1)^{k+1} k s_k + g_k(s_1, ..., s_n) \quad (1 \leq k \leq n) .
$$
Comme $k!.1$ est inversible dans $A$, le lemme 2 de IV, p. 33, prouve l’existence d’un automorphisme $T$ de la $A$-algèbre topologique $A[[X]]^{sym}$ qui transforme $s_k$ en $p_k$ pour $1 \leq k \leq n$. La prop. 3, a) résulte aussitôt de là.

**Corollaire. — Soient $\xi_1, ..., \xi_n, \eta_1, ..., \eta_n$ des éléments de $A$. On suppose que $A$ est intègre.

a) *Si l’on a $s_k(\xi_1, ..., \xi_n) = s_k(\eta_1, ..., \eta_n)$ pour $1 \leq k \leq n$, il existe une permutation $\sigma \in S_n$ telle que $\eta_i = \xi_{\sigma(i)}$ pour $1 \leq i \leq n$.

b) *Supposons que l’on ait $n!.1 \neq 0$ dans $A$ et
$$
\xi_1^k + \cdots + \xi_n^k = \eta_1^k + \cdots + \eta_n^k
$$
pour $1 \leq k \leq n$. Il existe une permutation $\sigma \in S_n$ telle que $\eta_i = \xi_{\sigma(i)}$ pour $1 \leq i \leq n$.

Sous les hypothèses de a), on a $\prod_{i=1}^n (X - \xi_i) = \prod_{i=1}^n (X - \eta_i)$. Substituant $\eta_n$ à $X$, on obtient $\prod_{i=1}^n (\eta_n - \xi_i) = 0$ et comme $A$ est intègre, il existe un entier $\sigma(n)$ tel que $1 \leq \sigma(n) \leq n$ et $\eta_n = \xi_{\sigma(n)}$. L’assertion a) résulte facilement par récurrence de là, car $A[X]$ est un anneau intègre.

Sous les hypothèses de b), il existe d’après la prop. 3 des polynômes $\Pi_1, ..., \Pi_n$ en $n$ indéterminées à coefficients dans le corps des fractions de $A$ tels que $s_k = \Pi_k(p_1, ..., p_n)$ pour $1 \leq k \leq n$. La relation (23) entraîne alors
$$
s_k(\xi_1, ..., \xi_n) = s_k(\eta_1, ..., \eta_n)
$$
pour $1 \leq k \leq n$, et b) résulte de a).

### 5. Fonctions symétriques des racines d’un polynôme

Considérons un polynôme unitaire de degré $n$, à coefficients dans $A$, soit
$$
f = X^n + a_1 X^{n-1} + \cdots + a_{n-1} X + a_n .
$$

Définissons la A-algèbre associative, commutative et unifère $E_f$ par les générateurs $x_1, \ldots, x_n$ et les relations

$$
(24) \quad \sum_{i_1 < \ldots < i_k} x_{i_1} \ldots x_{i_k} = (-1)^k a_k \quad (1 \leq k \leq n) .
$$

De manière plus précise, on a

$$
E_f = A[X_1, \ldots, X_n]/a
$$

où l’idéal $a$ est engendré par les polynômes $s_k + (-1)^{k+1} a_k$ pour $1 \leq k \leq n$, et $x_i$ est la classe de $X_i$ modulo $a$ pour $1 \leq i \leq n$. La relation (24) équivaut encore à $f(X) = \prod_{i=1}^n (X - x_i)$. Lorsqu’il y aura un risque d’ambiguïté, on écrira $x_{1,f}, \ldots, x_{n,f}$ pour $x_1, \ldots, x_n$ respectivement.

#### Proposition 4 {#alg-iv-s6-prop-4 .statement}

*Soient B un anneau commutatif, ρ un homomorphisme de A dans B, et $\xi_1, \ldots, \xi_n$ des éléments de B. On suppose que l’on a la relation $^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ dans B[X]. Il existe alors un homomorphisme d’anneaux $u : E_f \to B$ et un seul tel que $\rho(a) = u(a.1)$ pour tout $a \in A$ et $u(x_i) = \xi_i$ pour $1 \leq i \leq n$.

Considérons B comme une A-algèbre associative, commutative et unifère au moyen de $\rho$. La relation $^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ s’écrit aussi sous la forme*

$$
\sum_{i_1 < \ldots < i_k} \xi_{i_1} \ldots \xi_{i_k} = (-1)^k a_k \cdot 1 \quad (1 \leq k \leq n)
$$

dans B. Comme les relations (24) définissent une présentation de $E_f$, la prop. 4 s’ensuit.

La prop. 4 justifie le nom d’« algèbre de décomposition universelle de $f$ » pour $E_f$. La relation $f(X) = \prod_{i=1}^n (X - x_{i,f})$ s’appelle la « décomposition universelle de $f$ ». Soit $\sigma \in S_n$ une permutation ; comme on a $f(X) = \prod_{i=1}^n (X - x_{\sigma(i),f})$, il existe un automorphisme $t_\sigma$ de la A-algèbre $E_f$, caractérisé par $t_\sigma(x_{i,f}) = x_{\sigma(i),f}$ pour $1 \leq i \leq n$. On a $t_{\sigma \tau} = t_\sigma \circ t_\tau$ pour $\sigma, \tau$ dans $S_n$, d’où une action du groupe $S_n$ sur la A-algèbre $E_f$.

#### Proposition 5 {#alg-iv-s6-prop-5 .statement}

*Dans l’algèbre de décomposition universelle $E_f$, la famille des monômes $x_1^{v(1)} \ldots x_n^{v(n)}$, tels que $0 \leq v(i) < i$ pour $1 \leq i \leq n$, est une base du A-module $E_f$. En particulier, $E_f$ est un A-module libre de rang $n!$.

Posons $B = A[X_1, \ldots, X_n]$ et $C = A[X_1, \ldots, X_n]^{\text{sym}}$. D’après le th. 1 (IV, p. 58), on a $C = A[s_1, \ldots, s_n]$ et $s_1, \ldots, s_n$ sont algébriquement indépendants sur A. Les polynômes sans terme constant en $s_1, \ldots, s_n$ forment un idéal $C^+$ de C, supplémentaire de $A$, et engendré par $s_1, \ldots, s_n$. Soit $c$ l’idéal de $C$ engendré par $s_1 + a_1, s_2 - a_2, \ldots, s_n + (-1)^{n+1}a_n$. Il existe un automorphisme de la $A$-algèbre $C$ qui applique $s_k$ sur $s_k + (-1)^{k+1}a_k$ pour $1 \leq k \leq n$, donc $C^+$ sur $c$; par suite, on a $C = A \oplus c$. Par ailleurs, le th. 1, c) de IV, p. 58, montre que l’on a

$$
B = \bigoplus_{v \in S} CX^v
$$

où $S$ est l’ensemble des $v \in \mathbf{N}^n$ tels que $0 \leq v(i) < i$ pour $1 \leq i \leq n$. L’idéal $a$ de $B$ est engendré par $c$, d’où $a = Bc = \bigoplus_{v \in S} c.X^v$. Comme on a $C = A \oplus c$, on en déduit

$$
B = a \oplus \bigoplus_{v \in S} AX^v,
$$

d’où la prop. 5 puisque $E_f = B/a$.

#### Corollaire {#alg-iv-s6-n5-cor-1 .statement}

*L’homomorphisme canonique de $A$ dans l’algèbre de décomposition universelle du polynôme unitaire $f \in A[X]$ est injectif.*
En effet, l’élément unité de $E_f$ appartient à une base du $A$-module $E_f$.

#### Proposition 6 {#alg-iv-s6-prop-6 .statement}

*Soit $f \in A[X]$ un polynôme unitaire de degré $n$. Soit $P$ un polynôme symétrique en $X_1, \ldots, X_n$ à coefficients dans $A$. Il existe un élément $a$ de $A$, et un seul, possédant la propriété suivante :*
(FS) *Quels que soient l’homomorphisme d’anneaux $\rho : A \to B$ et la décomposition $\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ dans $B[X]$, on a $\rho(a) = P(\xi_1, \ldots, \xi_n)$.*

Posons $f = X^n + \sum_{k=1}^n a_k X^{n-k}$. D’après le th. 1 de IV, p. 58, il existe un polynôme $\Pi$ en $n$ indéterminées à coefficients dans $A$ tel que $P = \Pi(s_1, \ldots, s_n)$. Posons $a = \Pi(-a_1, a_2, \ldots, (-1)^n a_n)$. Sous les hypothèses de (FS), on a

$$
s_k(\xi_1, \ldots, \xi_n) = (-1)^k \rho(a_k)
$$

d’où

$$
\begin{align*}
\rho(a) &= \Pi(-\rho(a_1), \rho(a_2), \ldots, (-1)^n \rho(a_n)) \\
&= \Pi(s_1(\xi_1, \ldots, \xi_n), \ldots, s_n(\xi_1, \ldots, \xi_n)) \\
&= P(\xi_1, \ldots, \xi_n).
\end{align*}
$$

Ceci prouve l’existence d’un élément $a$ satisfaisant à (FS). L’unicité de $a$ résulte du cor. de la prop. 5, car on a $a.1 = P(x_{1,f}, \ldots, x_{n,f})$ dans l’algèbre de décomposition universelle $E_f$.

Avec les notations de la prop. 6, on posera parfois $a = P^*(f)$. Voici quelques exemples.

#### Exemple 1 {#alg-iv-s6-n5-exa-1 .statement}

Si $P = s_k$, on a $P^*(f) = (-1)^k a_k$.

#### Exemple 2 {#alg-iv-s6-n5-exa-2 .statement}

\* Soit $g$ un polynôme dans $\mathbf{A}[X]$; posons

$$
P(X_1, \ldots, X_n) = g(X_1) \ldots g(X_n)
$$

Alors $P^*(f)$ n’est autre que le résultant $\operatorname{res}(f, g)$ d’après le cor. 1 de IV, p. 75.

#### Exemple 3 {#alg-iv-s6-n5-exa-3 .statement}

Posons $\Delta(X_1, \ldots, X_n) = \prod_{i < j} (X_i - X_j)^2$. Alors $\Delta^*(f)$ n’est autre que le discriminant du polynôme unitaire $f$ (IV, p. 77, formule (46)).

#### Exemple 4 {#alg-iv-s6-n5-exa-4 .statement}

Posons $P(X_1, \ldots, X_n) = X_1^k + \cdots + X_n^k$; introduisons par ailleurs l’algèbre $E = \mathbf{A}[X]/(f)$ et notons $x$ l’image de $X$ dans $E$. Rappelons que le $\mathbf{A}$-module $E$ est libre, de base $(1, x, \ldots, x^{n-1})$ (IV, p. 10, corollaire). Montrons que l’on a

$$
\operatorname{Tr}_{E/\mathbf{A}}(x^k) = P^*(f)
$$

Posons $\pi_k = \operatorname{Tr}_{E/\mathbf{A}}(x^k)$ pour tout entier $k \geq 1$. Compte tenu des relations de Newton (IV, p. 65), il suffit d’établir les relations

$$
\begin{align*}
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + k a_k = 0 \quad \text{pour } 1 \leq k \leq n \\
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{n-1} \pi_{k-n+1} + a_n \pi_{k-n} = 0 \quad \text{pour } k > n
\end{align*}
$$

(que nous appellerons aussi « relations de Newton »). La relation (27) est immédiate, car le premier membre est la trace de

$$
x^{k-n}(x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n) = 0 .
$$

Supposons qu’on ait $1 \leq k \leq n$ et posons

$$
y = x^k + a_1 x^{k-1} + \cdots + a_{k-1} x + a_k . 1 ;
$$

soit $M = (m_{ij})$ la matrice de l’application linéaire $u \mapsto yu$ dans $E$, par rapport à la base $(x^i)_{0 \leq i < n}$. On prouve facilement les relations

$$
\begin{align*}
&m_{ii} = a_k \quad \text{pour } 0 \leq i < n - k \\
&m_{ii} = 0 \quad \text{pour } n - k \leq i < n ,
\end{align*}
$$

d’où

$$
\operatorname{Tr}_{E/\mathbf{A}}(y) = \sum_{i=0}^{n-1} m_{ii} = (n - k) a_k .
$$

On a par ailleurs

$$
\operatorname{Tr}_{E/\mathbf{A}}(y) = \pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + n a_k ,
$$

d’où la formule (26).

### 6. Résultant

Dans ce numéro, on se donne deux entiers positifs $p, q$ et deux polynômes $f, g$ dans $\mathbf{A}[X]$, de la forme

$$
f = t_p X^p + t_{p-1} X^{p-1} + \cdots + t_0
$$
$$
g = u_q X^q + u_{q-1} X^{q-1} + \cdots + u_0
$$

tels que $\deg f \leq p, \deg g \leq q$. Pour tout entier $n \geq 0$, on note $S_n$ le sous-$\mathbf{A}$-module de $\mathbf{A}[X]$ formé des polynômes de degré $< n$; il a pour base la famille $(X^i)_{0 \leq i < n}$, donc est de rang $n$.

On munit $S_q \times S_p$ de la base

$$
B_1 = ((X^{q-1}, 0), \ldots, (X, 0), (1, 0), (0, X^{p-1}), \ldots, (0, X), (0, 1))
$$

et $S_{p+q}$ de la base

$$
B_2 = (X^{p+q-1}, \ldots, X, 1)
$$

On définit une application linéaire $\varphi : S_q \times S_p \to S_{p+q}$ par

$$
\varphi(u, v) = uf + vg
$$

et l’on note $M(f, g, p, q)$ la matrice de $\varphi$ par rapport aux bases $B_1$ et $B_2$. C’est une matrice carrée d’ordre $p + q$, indexée par l’ensemble $\{0, 1, \ldots, p + q - 1\}$. Ses éléments $a_{ij}$ sont donnés par les règles :

a) on a $a_{ij} = t_{p-i+j}$ pour $0 \leq j \leq q - 1$,
b) on a $a_{ij} = u_{j-i}$ pour $q \leq j \leq p + q - 1$,

où l’on convient que $t_k$ est nul si $k \notin \{0, p\}$ et que $u_k$ est nul si $k \notin \{0, q\}$.

Par exemple, pour $p = 2$ et $q = 3$, on a la matrice

$$
\begin{pmatrix}
t_2 & 0 & 0 & u_3 & 0 \\
t_1 & t_2 & 0 & u_2 & u_3 \\
t_0 & t_1 & t_2 & u_1 & u_2 \\
0 & t_0 & t_1 & u_0 & u_1 \\
0 & 0 & t_0 & 0 & u_0
\end{pmatrix}.
$$

#### Définition 1 {#alg-iv-s6-def-1 .statement}

Avec les notations ci-dessus, le déterminant de la matrice $M(f, g, p, q)$ s’appelle le résultant du couple $(f, g)$ pour les degrés $p$ et $q$, ou simplement le résultant de $f$ et $g$ si $p = \deg f$ et $q = \deg g$.

Ce résultant se note $\operatorname{res}_{p,q}(f, g)$ ou simplement $\operatorname{res}(f, g)$ lorsque $p = \deg f, q = \deg g$.

#### Exemple 1 {#alg-iv-s6-n6-exa-1 .statement}

Soient $\lambda, \mu$ dans $\mathbf{A}$. On a les formules
$$
\begin{align*}
\operatorname{res}_{p,0}(f, \lambda) &= \lambda^p, & \operatorname{res}_{0,q}(\mu, g) &= \mu^q \\
\operatorname{res}_{p,1}(f, \lambda) &= \lambda^p t_p, & \operatorname{res}_{1,q}(\mu, g) &= (-1)^q \mu^q u_q,
\end{align*}
$$
de démonstration immédiate.

#### Exemple 2 {#alg-iv-s6-n6-exa-2 .statement}

Lorsque $p = q = 1$, on a
$$
\operatorname{res}_{1,1}(t_1 X + t_0, u_1 X + u_0) = t_1 u_0 - t_0 u_1 .
$$

#### Remarque 1 {#alg-iv-s6-n6-rem-1 .statement}

La matrice $M(g, f, q, p)$ se déduit de $M(f, g, p, q)$ par $pq$ transpositions de colonnes, d’où
$$
\operatorname{res}_{q,p}(g, f) = (-1)^{pq} \operatorname{res}_{p,q}(f, g) .
$$

#### Remarque 2 {#alg-iv-s6-n6-rem-2 .statement}

Soit $\rho : \mathbf{A} \to \mathbf{B}$ un homomorphisme d’anneaux. La définition 1 entraîne aussitôt la formule
$$
\operatorname{res}_{p,q}(\rho f, \rho g) = \rho(\operatorname{res}_{p,q}(f, g)) .
$$

#### Remarque 3 {#alg-iv-s6-n6-rem-3 .statement}

Soient $\lambda, \mu$ dans $\mathbf{A}$. On a
$$
\operatorname{res}_{p,q}(\lambda f, \mu g) = \lambda^q \mu^p \operatorname{res}_{p,q}(f, g) .
$$
(28)

#### Remarque 4 {#alg-iv-s6-n6-rem-4 .statement}

Supposons qu’on ait $p + q \geqslant 1$. D’après III, p. 99, formule (28), l’image de $\varphi$ contient le polynôme constant $\operatorname{res}_{p,q}(f, g)$. Il existe donc un couple de polynômes $(u, v)$, avec $u \in S_q,\ v \in S_p$, tel que
$$
\operatorname{res}_{p,q}(f, g) = uf + vg ,
$$
d’où
$$
\operatorname{res}_{p,q}(f, g) \in \mathbf{A} \cap (f, g) .
$$
Ce couple $(u, v)$ est unique lorsque $\operatorname{res}_{p,q}(f, g)$ est simplifiable dans $\mathbf{A}$ : en effet, $\varphi$ est alors injective (III, p. 91, prop. 3).

#### Remarque 5 {#alg-iv-s6-n6-rem-5 .statement}

Supposons $p \geqslant q$. Soit $h \in \mathbf{A}[X]$ un polynôme de degré $\leqslant p - q$. Montrons que l’on a
$$
\operatorname{res}_{p,q}(f, g) = \operatorname{res}_{p,q}(f + gh, g) .
$$
En effet, posons $\omega(u, v) = (u, uh + v)$ pour $(u, v) \in S_q \times S_p$. Alors $\omega$ est un automorphisme du $\mathbf{A}$-module $S_q \times S_p$ et l’on a
$$
\omega^{-1}(u, v) = (u, -uh + v) .
$$
La matrice de $\omega$ par rapport à la base $B_1$ est triangulaire inférieure, et ses éléments diagonaux sont égaux à 1. D’autre part, $\varphi \circ \omega$ applique $(u, v)$ sur $u(f + gh) + vg$. La formule (29) signifie que les matrices représentant $\varphi$ et $\varphi \circ \omega$ ont même déterminant, et ceci résulte de la relation $\det \omega = 1$.

Supposons $f$ unitaire de degré $p$; posons $E = A[X]/(f)$ et notons $x$ l’image canonique de $X$ dans $E$. On sait (IV, p. 10) que $E$ est un $A$-module libre, de base $(1, x, ..., x^{p-1})$. On peut donc définir la norme $N_{E/A}(u)$ de tout élément $u$ de $E$ (III, p. 110, déf. 2).

#### Proposition 7 {#alg-iv-s6-prop-7 .statement}

*Supposons $f$ unitaire de degré $p$. Avec les notations précédentes, on a*¹

$$
\operatorname{res}_{p,q}(f, g) = N_{E/A}(g(x)) .
$$

Définissons une application $A$-linéaire $\theta$ de $S_q \times S_p$ dans $S_{p+q}$ par $\theta(u, v) = uf + v$. Alors $\theta$ transforme la base $B_1$ de $S_q \times S_p$ en la suite

$$
(fX^{q-1}, ..., fX, f, X^{p-1}, ..., X, 1)
$$

d’éléments de $S_{p+q}$; la matrice $M_\theta$ de $\theta$ par rapport aux bases $B_1$ et $B_2$ est donc triangulaire inférieure et ses éléments diagonaux sont égaux à 1, d’où $\det M_\theta = 1$.

Par suite, $\theta$ est bijectif, et $\operatorname{res}_{p,q}(f, g)$ est égal au déterminant de l’endomorphisme $\varphi' = \varphi \circ \theta^{-1}$ de $S_{p+q}$. De manière explicite, on a

$$
\varphi'(uf + v) = uf + vg
$$

pour tout couple $(u, v)$ dans $S_q \times S_p$. Or, on a $A[X] = S_{p+q} + (f)$ et $fS_q = S_{p+q} \cap (f)$, donc l’injection canonique de $S_{p+q}$ dans $A[X]$ définit par passage aux quotients un isomorphisme $\gamma$ de $S_{p+q}/fS_q$ sur $E$. Soit $\psi$ la multiplication par $g(x)$ dans $E$. La formule (31) montre que $\varphi'$ induit l’identité sur $fS_q$ et $\gamma^{-1}\psi\gamma$ sur $S_{p+q}/fS_q$. On a donc $\det \varphi' = \det \psi$, d’où la formule (30) puisque $\det \varphi' = \operatorname{res}_{p,q}(f, g)$ et $\det \psi = N_{E/A}(g(x))$ par définition.

#### Corollaire 1 {#alg-iv-s6-prop-7-cor-1 .statement}

*Soit $f \in A[X]$ un polynôme unitaire. Pour tout polynôme $g \in A[X]$, les conditions suivantes sont équivalentes :*
(i) res$(f, g)$ *est inversible dans* $A$;
(ii) *il existe des polynômes* $u, v$ *de* $A[X]$ *tels que* $uf + vg = 1$;
(iii) *$g(x)$ est inversible dans l’algèbre* $A[X]/(f)$.

L’équivalence de (i) et (iii) résulte de la prop. 3 de III, p. 111, et de la prop. 7; celle de (ii) et (iii) est triviale.

#### Corollaire 2 {#alg-iv-s6-prop-7-cor-2 .statement}

*Supposons que* $A$ *soit un corps. Soient* $f, g$ *dans* $A[X]$. *Les conditions suivantes sont équivalentes lorsque* $f$ *et* $g$ *sont non nuls :*
(i) *on a* $\operatorname{res}(f, g) \neq 0$;
(ii) *les polynômes* $f$ *et* $g$ *sont étrangers dans* $A[X]$;
*(iii) quelle que soit l’extension* $L$ *de* $A$, *les polynômes* $f$ *et* $g$ *n’ont pas de racine commune dans* $L$. \*

¹ Le résultant $\operatorname{res}_{p,q}(f, g)$ est donc indépendant de $q$ lorsque $f$ est unitaire de degré $p$. On le note alors simplement $\operatorname{res}(f, g)$.

On se ramène aussitôt au cas où $f$ est unitaire (IV, p. 72, remarque 3).
L’équivalence de (i) et (ii) n’est qu’une traduction du cor. 1 d’après la déf. 1 de IV, p. 12 ; l’équivalence de (ii) et (iii) n’est autre que le cor. 7 de IV, p. 12.

#### Corollaire 3 {#alg-iv-s6-prop-7-cor-3 .statement}

Pour tout $\lambda \in \mathbf{A}$, on a

$$
\operatorname{res}_{p,1}(f, \lambda - X) = f(\lambda) , \quad \operatorname{res}_{1,q}(X - \lambda, g) = g(\lambda) .
$$

Lorsque $f(X) = X - \lambda$, l’algèbre E est égale à A, et l’on a $x = \lambda$ ; la deuxième formule (32) résulte donc de la prop. 7 (IV, p. 73). D’après les remarques 1 et 3 (IV, p. 72), on en déduit

$$
\operatorname{res}_{p,1}(f, \lambda - X) = (-1)^p \operatorname{res}_{1,p}(\lambda - X, f) = (-1)^{p+p} \operatorname{res}_{1,p}(X - \lambda, f) = f(\lambda) .
$$

Supposons maintenant $f$ et $g$ unitaires. On note F la A-algèbre $\mathbf{A}[X, Y]/(f(X), g(Y))$ et $x$ (resp. $y$) l’image canonique de X (resp. Y) dans F.

#### Proposition 8 {#alg-iv-s6-prop-8 .statement}

Supposons $f$ et $g$ unitaires de degrés respectifs $p$ et $q$. Avec les notations précédentes, le A-module F est libre de base $(x^i y^j)_{0 \leq i < p, 0 \leq j < q}$, et l’on a

$$
\operatorname{res}(f, g) = N_{F/A}(x - y) .
$$

Posons $E = \mathbf{A}[X]/(f)$ et $E' = \mathbf{A}[Y]/(g)$. D’après II, p. 60, cor. 1, l’homomorphisme $\sigma$ de $E \otimes E'$ dans F déduit de l’homomorphisme canonique $\mathbf{A}[X] \otimes \mathbf{A}[Y] \to \mathbf{A}[X, Y]$ est bijectif. Ceci prouve l’assertion sur la base de F. On identifiera E à son image dans F par $\sigma$. Alors, l’homomorphisme de E-algèbres de $E[Y]/(g(Y))$ dans F qui applique Y sur $y$ est un isomorphisme.

D’après la transitivité de la norme (III, p. 114), on a

$$
N_{F/A}(x - y) = N_{E/A}(N_{F/E}(x - y)) .
$$

D’après la prop. 7 (IV, p. 73), $N_{F/E}(x - y)$ est le résultant des polynômes $g(Y)$ et $x - Y$ de $E[Y]$, donc est égal à $g(x)$ (IV, p. 74, cor. 3). D’après la formule (34) et la prop. 7 (IV, p. 73), on a donc

$$
N_{F/A}(x - y) = N_{E/A}(g(x)) = \operatorname{res}(f, g) .
$$

#### Proposition 9 {#alg-iv-s6-prop-9 .statement}

Soient $p_1$ et $q_1$ des entiers positifs et $f_1, g_1$ des polynômes dans $\mathbf{A}[X]$ tels que $\deg f_1 \leq p_1$, $\deg g_1 \leq q_1$. On a

$$
\operatorname{res}_{p,q+q_1}(f, gg_1) = \operatorname{res}_{p,q}(f, g) . \operatorname{res}_{p,q_1}(f, g_1)
$$
$$
\operatorname{res}_{p+p_1,q}(ff_1, g) = \operatorname{res}_{p,q}(f, g) . \operatorname{res}_{p_1,q}(f_1, g) .
$$

On a $\operatorname{res}_{p,q}(f, g) = (-1)^{pq} \operatorname{res}_{q,p}(g, f)$ (IV, p. 72) ; il suffit donc de prouver la formule (35). De même, la remarque 3 (loc. cit.) montre que si la formule (35) est établie pour un polynôme $f$, elle l’est pour tous les polynômes de la forme $\lambda f$ avec $\lambda \in \mathbf{A}$. Enfin, lorsque $f$ est unitaire de degré $p$, la formule (35) résulte de la prop. 7 (IV, p. 73), en vertu de la formule $N_{E/A}(ab) = N_{E/A}(a) \cdot N_{E/A}(b)$. De tout ceci, on conclut que la formule (35) est vraie lorsque le coefficient $t_p$ de $X^p$ dans $f$ est *inversible*.

#### Lemme 5 {#alg-iv-s6-lem-5 .statement}

*Soit t un élément de A. Il existe un anneau commutatif C contenant A comme sous-anneau, un sous-anneau B de C contenant A, un élément $\tau$ de B, inversible dans C, et un homomorphisme d’anneaux $\rho : B \to A$ tel que $\rho(\tau) = t$ et que la restriction de $\rho$ à A soit égale à $\mathrm{Id}_A$.

Il suffit de prendre pour B l’algèbre $A^{(N)}$ du monoïde $\mathbf{N}$, c’est-à-dire l’algèbre de polynômes $A[\tau]$ en une indéterminée $\tau$, pour C l’algèbre $A^{(Z)}$ du groupe $\mathbf{Z}$ et pour $\rho$ l’homomorphisme $P \mapsto P(t)$ de $A[\tau]$ dans A.

Avec les notations du lemme 5, où l’on fait $t = t_p$, posons

$$
F = \tau X^p + t_{p-1} X^{p-1} + \cdots + t_1 X + t_0
$$

dans $B[X]$. Le coefficient de $X^p$ dans F est *inversible dans C* ; si l’on considère F, $g$, $g_1$ comme des polynômes de $C[X]$, on a donc

$$
\operatorname{res}_{p,q+q_1}(F, gg_1) = \operatorname{res}_{p,q}(F, g) \cdot \operatorname{res}_{p,q_1}(F, g_1)
$$

d’après ce qui précède. On ne change pas les résultants si l’on considère F, $g$ et $g_1$ comme des polynômes de $B[X]$. Comme on a $^\rho F = f, ^\rho g = g, ^\rho g_1 = g_1$, la formule (35) résulte de (38) et de la remarque 2 (IV, p. 72).

#### Corollaire 1 {#alg-iv-s6-lem-5-cor-1 .statement}

(i) *Soient $\lambda, \alpha_1, \ldots, \alpha_p$ des éléments de A et supposons que l’on ait $f(X) = \lambda(X - \alpha_1) \ldots (X - \alpha_p)$. On a*

$$
\operatorname{res}_{p,q}(f, g) = \lambda^q g(\alpha_1) \ldots g(\alpha_p) .
$$

(ii) *Soient $\mu, \beta_1, \ldots, \beta_q$ des éléments de A et supposons que l’on ait de plus $g(X) = \mu(X - \beta_1) \ldots (X - \beta_q)$. On a alors*

$$
\operatorname{res}_{p,q}(f, g) = \lambda^q \mu^p \prod_{\substack{1 \leq i \leq p \\ 1 \leq j \leq q}} (\alpha_i - \beta_j) .
$$

L’assertion (i) résulte aussitôt des formules (28), (32) et (36). L’assertion (ii) résulte aussitôt de (i).

#### Corollaire 2 {#alg-iv-s6-lem-5-cor-2 .statement}

*Pour tout entier $r \geq 0$, on a*

$$
\operatorname{res}_{p,q+r}(f, g) = t_p^r \cdot \operatorname{res}_{p,q}(f, g) .
$$

Compte tenu de l’exemple 1 (IV, p. 72), il suffit de faire $q_1 = r, g_1 = 1$ dans la formule (35).

Supposons $f$ unitaire. Soient $\rho : A \to B$ un homomorphisme d’anneaux et $\xi_1, \ldots, \xi_p$ des éléments de $B$ tels que l’on ait la décomposition

$$
\rho f(X) = (X - \xi_1) \ldots (X - \xi_p) .
$$

D’après la remarque 2 (IV, p. 72) et le cor. 1 ci-dessus, on a

$$
\rho(\operatorname{res}(f, g)) = g(\xi_1) \ldots g(\xi_p) .
$$

Cette remarque s’applique en particulier à la décomposition universelle de $f$ (IV, p. 68), et comme $\rho$ est alors injectif, cela fournit un moyen de calcul de $\operatorname{res}(f, g)$.

#### Exemple 3 {#alg-iv-s6-n6-exa-3 .statement}

Prouvons la formule

(42) $\operatorname{res}_{2,2}(aX^2 + bX + c, a'X^2 + b'X + c') = (ac' - ca')^2 + (bc' - cb')(ba' - ab') .$

En raisonnant comme dans la prop. 9 (IV, p. 74), on voit qu’il suffit de prouver cette formule lorsque $a$ est *inversible*. Il existe alors une décomposition de la forme

(43) $aX^2 + bX + c = a(X - x)(X - y)$

dans $B[X]$, où $B$ est un anneau commutatif convenable contenant $A$ comme sous-anneau. D’après le cor. 1 ci-dessus, le résultant cherché est égal à

(44) $R = a^2(a'x^2 + b'x + c')(a'y^2 + b'y + c') .$

Or on a

$$
ax + ay = -b , \quad axy = c
$$

d’après (43), d’où $(ax)^2 + (ay)^2 = b^2 - 2ac$.

D’après (44), on a

$$
R = {a'}^2(axy)^2 + a{b'}^2(axy) + a^2{c'}^2 + a'b'(axy)(ax + ay) + a'c'((ax)^2 + (ay)^2) + ab'c'(ax + ay)
$$
$$
= {a'}^2c^2 + a{b'}^2c + a^2{c'}^2 - a'b'cb + a'c'(b^2 - 2ac) - ab'c'b
$$
$$
= (ac' - ca')^2 + (ab' - a'b)(b'c - c'b) ,
$$

d’où le résultat annoncé.

### 7. Discriminant

#### Définition 2 {#alg-iv-s6-def-2 .statement}

*Soient $f$ un polynôme unitaire de $A[X]$ et $m$ son degré. Notons $E$ la $A$-algèbre $A[X]/(f)$ et $x$ l’image canonique de $X$ dans $E$. On appelle discriminant de $f$, et l’on note dis(f), le discriminant $D_{E/A}(1, x, ..., x^{m-1})$ de la base $(1, x, ..., x^{m-1})$ de la A-algèbre E.

Pour tout entier positif $k$, posons $p_k = \mathrm{Tr}_{E/A}(x^k)$. D’après III, p. 115, la définition 2 se traduit par la formule

$$
\text{dis}(f) = \det(p_{i+j})_{0 \leq i,j < m}.
$$

#### Exemple 1 {#alg-iv-s6-n7-exa-1 .statement}

Si $f$ est un polynôme unitaire de degré 0 ou 1, on a $\text{dis}(f) = 1$ d’après (45).

#### Exemple 2 {#alg-iv-s6-n7-exa-2 .statement}

Soit $f(X) = X^2 + \alpha X + \beta$ un polynôme unitaire de degré 2. Les relations de Newton s’écrivent sous la forme (IV, p. 70)

$$
\begin{align*}
p_0 &= 2 \\
p_1 + \alpha &= 0 \\
p_2 + \alpha p_1 + 2\beta &= 0,
\end{align*}
$$

d’où $p_1 = -\alpha, p_2 = \alpha^2 - 2\beta$. Par suite, on a

$$
\text{dis}(f) = \det \begin{pmatrix} 2 & -\alpha \\ -\alpha & \alpha^2 - 2\beta \end{pmatrix} = \alpha^2 - 4\beta.
$$

Soient B un anneau commutatif, $\rho$ un homomorphisme de A dans B et $\xi_1, ..., \xi_m$ des éléments de B tels que

$$
\rho f(X) = (X - \xi_1) ... (X - \xi_m).
$$

Notons $M$ la matrice $(\rho(p_{i+j}))_{0 \leq i,j < m}$ et $D$ la matrice de van der Monde $(\xi_{i+1}^j)_{0 \leq i,j < m}$. D’après l’exemple 4 de IV, p. 70, on a

$$
\rho(p_k) = \xi_1^k + \cdots + \xi_m^k,
$$

d’où $M = {}^tD.D$; on a $\det D = \prod_{i > j} (\xi_i - \xi_j)$ d’après III, p. 99, et $\det M = (\det D)^2$, c’est-à-dire

$$
\rho(\text{dis}(f)) = \prod_{i < j} (\xi_i - \xi_j)^2.
$$

(46)

De plus, on a $\left( \text{en notant } D \text{ la dérivation } \frac{d}{dX} \right)$

$$
D(\rho f)(\xi_i) = (\xi_i - \xi_1) ... (\xi_i - \xi_{i-1}) (\xi_i - \xi_{i+1}) ... (\xi_i - \xi_m)
$$

pour $1 \leq i \leq m$, d’où

$$
\rho(\text{dis}(f)) = (-1)^{m(m-1)/2} \prod_{i \neq j} (\xi_i - \xi_j) = (-1)^{m(m-1)/2} \prod_{i=1}^m D(\rho f)(\xi_i).
$$

D’après le cor. 1 de IV, p. 75, appliqué à la décomposition universelle de $f$, on a finalement
$$
\text{res}(f, Df) = \text{res}(Df, f) = (-1)^{m(m-1)/2} \text{dis}(f) .
$$

#### Proposition 10 {#alg-iv-s6-prop-10 .statement}

Soit $m \geqslant 1$. Il existe un unique polynôme $\Delta \in \mathbf{Z}[A_1, ..., A_m]$ avec la propriété suivante : quels que soient l’anneau commutatif $A$ et le polynôme unitaire $f = X^m + \sum_{i=1}^m a_i X^{m-i}$ dans $A[X]$, on a
$$
\text{dis}(f) = \Delta(a_1, ..., a_m) .
$$
De plus, $\Delta$ est de degré $\leqslant 2m - 2$; si l’on munit $A_i$ du poids $i$, alors $\Delta$ est isobare de poids $m(m-1)$.

a) Unicité de $\Delta$ : si $\Delta$ satisfait à (48), on a en particulier $\Delta = \text{dis}(F)$, où $F$ est le polynôme $X^m + \sum_{i=1}^m A_i X^{m-i}$ à coefficients dans $\mathbf{Z}[A_1, ..., A_m]$.

b) Existence de $\Delta$ : soient $s_1, ..., s_m$ les polynômes symétriques élémentaires en les indéterminées $X_1, ..., X_m$. Il existe un polynôme $\Delta \in \mathbf{Z}[A_1, ..., A_m]$ isobare de poids $m(m-1)$ tel que
$$
\Delta(-s_1, s_2, ..., (-1)^m s_m) = \prod_{i < j} (X_i - X_j)^2 ;
$$
en effet, le second membre de cette relation est un polynôme $P$ symétrique, homogène de degré $m(m-1)$, dans $\mathbf{Z}[X_1, ..., X_m]$ (IV, p. 58, th. 1). Or la formule (46) signifie que l’on a $\text{dis}(f) = P^*(f)$ avec les notations de IV, p. 69 ; la formule (48) résulte aussitôt de là.

c) Degré de $\Delta$ : la relation (47) et la définition du résultant (IV, p. 71) entraînent la formule
$$
(-1)^{m(m-1)/2} \Delta = \det(a_{ij})_{0 \leq i, j \leq 2m-2}
$$
avec les valeurs suivantes des $a_{ij}$
$$
\begin{align*}
a_{00} &= 1 , \quad a_{0,m-1} = m , & a_{0j} &= 0 \quad \text{si} \quad j \neq 0 , \quad j \neq m-1 \\
a_{ij} &= A_{i-j} & \text{pour} \quad 1 \leq i \leq 2m-2 , \quad 0 \leq j \leq m-2 \\
a_{ij} &= (j-i+1) A_{m+i-j-1} & \text{pour} \quad 1 \leq i \leq 2m-2 , \quad m-1 \leq j \leq 2m-2 .
\end{align*}
$$
Dans ces formules, on convient que $A_0 = 1$ et $A_i = 0$ pour $i < 0$ ou $i > m$. La formule (50) montre aussitôt que $\Delta$ est de degré $\leq 2m-2$.

La prop. 10 permet d’étendre la définition du discriminant aux polynômes non unitaires. Soit $m \geqslant 1$ un entier. Il existe un unique polynôme homogène de degré $2m-2$, soit $\tilde{\Delta}$, dans $\mathbf{Z}[A_0, A_1, ..., A_m]$, tel que
$$
\Delta(A_1, ..., A_m) = \tilde{\Delta}(1, A_1, ..., A_m) ;
$$

en effet, comme $\Delta$ est de degré $\leq 2m - 2$, la fraction rationnelle

$$
A_0^{2m-2} \Delta(A_1/A_0, \ldots, A_m/A_0)
$$

appartient au sous-anneau $\mathbf{Z}[A_0, A_1, \ldots, A_m]$ de $\mathbf{Q}(A_0, A_1, \ldots, A_m)$. Si $A_i$ est de poids $i$ pour $0 \leq i \leq m$, alors $\tilde{\Delta}$ est isobare de poids $m(m-1)$. Si $f$ est un polynôme de degré $\leq m$, soit

$$
f = a_0 X^m + a_1 X^{m-1} + \cdots + a_{m-1} X + a_m,
$$

on posera

(52)

$$
\operatorname{dis}_m(f) = \tilde{\Delta}(a_0, a_1, \ldots, a_m).
$$

Lorsque $m = \deg f$, on écrit simplement $\operatorname{dis}(f)$ pour $\operatorname{dis}_m(f)$; si $f$ est unitaire, $\operatorname{dis}(f)$ coïncide avec le discriminant défini dans la déf. 2, d’après les formules (48), (51) et (52).

#### Proposition 11 {#alg-iv-s6-prop-11 .statement}

*Soit $f$ dans $\mathbf{A}[X]$ de degré $\leq m$.*

(i) *Si $\rho : \mathbf{A} \to \mathbf{B}$ est un homomorphisme d’anneaux, on a* $\operatorname{dis}_m(\rho f) = \rho(\operatorname{dis}_m(f))$.

(ii) *Soient $\lambda, \alpha_1, \ldots, \alpha_m$ des éléments de $\mathbf{A}$. Si* $f = \lambda(X - \alpha_1) \ldots (X - \alpha_m)$, *on a*

(53)

$$
\operatorname{dis}_m(f) = \lambda^{2m-2} \prod_{i < j} (\alpha_i - \alpha_j)^2.
$$

(iii) *Soit $a_0$ le coefficient de $X^m$ dans $f$. On a*

(54)

$$
\operatorname{res}_{m,m-1}(f, Df) = \operatorname{res}_{m-1,m}(Df, f) = (-1)^{m(m-1)/2} a_0 \operatorname{dis}_m(f).
$$

L’assertion (i) est évidente.
Comme $\tilde{\Delta}$ est homogène de degré $2m - 2$, on a

(55)

$$
\operatorname{dis}_m(\lambda f) = \lambda^{2m-2} \operatorname{dis}_m(f)
$$

pour tout polynôme $f \in \mathbf{A}[X]$ de degré $\leq m$. L’assertion (ii) résulte des formules (46) et (55).
Lorsque $f$ est unitaire de degré $m$, on a $a_0 = 1$ et l’assertion (iii) se réduit à la formule (47). Compte tenu de (55) et de la relation

(56)

$$
\operatorname{res}_{m,n}(\lambda f, \mu g) = \lambda^n \mu^m \operatorname{res}_{m,n}(f, g),
$$

(IV, p. 72), on passe de là au cas où $a_0$ est inversible dans $\mathbf{A}$. Le cas général résulte alors de la prop. 11, (i) et du lemme 5 (IV, p. 75).

#### Corollaire 1 {#alg-iv-s6-prop-11-cor-1 .statement}

*Soit $g \in \mathbf{A}[X]$ et soit $n$ un entier positif tel que $\deg g \leq n$. On a*

(57)

$$
\operatorname{dis}_{m+n}(fg) = \operatorname{dis}_m(f) \cdot \operatorname{dis}_n(g) \cdot \operatorname{res}_{m,n}(f, g)^2.
$$

En raisonnant comme ci-dessus, on se ramène au cas où $f$ et $g$ sont unitaires de degrés respectifs $m$ et $n$. Posons $B = E_f \otimes E_g$, où $E_f$ (resp. $E_g$) est l’algèbre de décomposition universelle de $f$ (resp. $g$) (IV, p. 68). Alors $A$ est un sous-anneau de $B$, et dans $B[X]$, on a des décompositions

$$
f = \prod_{i=1}^m (X - \alpha_i), \quad g = \prod_{j=1}^n (X - \beta_j).
$$

On a par suite

$$
fg = \prod_{k=1}^{m+n} (X - \gamma_k),
$$

avec $\gamma_i = \alpha_i$ pour $1 \leq i \leq m$, et $\gamma_{m+j} = \beta_j$ pour $1 \leq j \leq n$. On a l’identité évidente

$$
\prod_{k<k'} (\gamma_k - \gamma_{k'}) = \prod_{i<i'} (\alpha_i - \alpha_{i'}) \cdot \prod_{j<j'} (\beta_j - \beta_{j'}) \cdot \prod_{i,j} (\alpha_i - \beta_j).
$$

En élevant cette relation au carré, on obtient (57) d’après (40) et (46).

#### Corollaire 2 {#alg-iv-s6-prop-11-cor-2 .statement}

*Si $a_0$ est le coefficient de $X^m$ dans $f$, on a*

$$
\operatorname{dis}_{m+1}(f) = a_0^2 \operatorname{dis}_m(f).
$$

Cela résulte du cor. 1, où l’on fait $n = 1, g = 1$, d’après la formule $\operatorname{res}_{m,1}(f, 1) = a_0$ (IV, p. 72, exemple 1).

#### Corollaire 3 {#alg-iv-s6-prop-11-cor-3 .statement}

*Supposons que $A$ soit un corps. Soit $f$ un polynôme non constant de $A[X]$. Pour que $f$ et $Df$ soient étrangers, il faut et il suffit que l’on ait $\operatorname{dis}(f) \neq 0$.*
Cela résulte de la prop. 11, (iii) et du cor. 2 de IV, p. 73.

#### Remarque {#alg-iv-s6-n7-rem-1 .statement}

Une double application du cor. 2 ci-dessus montre que l’on a $\operatorname{dis}_m(f) = 0$ pour tout polynôme $f$ de degré $\leq m - 2$.

#### Exemple 3 {#alg-iv-s6-n7-exa-3 .statement}

Soit $m = 2$. D’après l’exemple 2 (IV, p. 77), on a $\Delta(A_1, A_2) = A_1^2 - 4A_2$, d’où $\tilde{\Delta}(A_0, A_1, A_2) = A_1^2 - 4A_0A_2$. Autrement dit, on a

$$
\operatorname{dis}_2(a_0X^2 + a_1X + a_2) = a_1^2 - 4a_0a_2.
$$

#### Exemple 4 {#alg-iv-s6-n7-exa-4 .statement}

Considérons le polynôme

$$
F = A_0X^3 + 3A_1X^2 + 3A_2X + A_3
$$

à coefficients dans $\mathbf{Q}[A_0, A_1, A_2, A_3]$. On a

$$
DF = 3(A_0X^2 + 2A_1X + A_2),
$$
d’où
$$
F - \frac{1}{3}X \cdot DF = A_1X^2 + 2A_2X + A_3.
$$

D’après les formules (54) (IV, p. 79) et (29) (IV, p. 72), on a

$$
A_0 \cdot \mathrm{dis}_3(F) = - \mathrm{res}_{2,3}(DF, F) = - \mathrm{res}_{2,3}(DF, F - \frac{1}{3}X \cdot DF).
$$

Appliquant le cor. 2 de IV, p. 75, on trouve finalement

$$
\mathrm{dis}_3(F) = - 27 \mathrm{res}_{2,2}(A_0 X^2 + 2A_1 X + A_2, A_1 X^2 + 2A_2 X + A_3).
$$

D’après l’exemple 3 de IV, p. 76, on a donc

$$
\tilde{\Delta}(A_0, 3A_1, 3A_2, A_3) = - 27(A_0 A_3 - A_1 A_2)^2 - 108(A_1 A_3 - A_2^2)(A_1^2 - A_0 A_2).
$$

Après quelques calculs, on trouve que si $f = a_0 X^3 + a_1 X^2 + a_2 X + a_3$, on a

$$
\mathrm{dis}_3(f) = a_1^2 a_2^2 + 18a_0 a_1 a_2 a_3 - 4a_1^3 a_3 - 4a_0 a_2^3 - 27a_0^2 a_3^2.
$$

En particulier, on a

$$
\mathrm{dis}(X^3 + pX + q) = - (4p^3 + 27q^2).
$$

Exercises

## EXERCICES {#alg-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
