---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 1
section_title: POLYNÔMES
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0008-0020, 0089-0090
extraction: ocr
subsections:
    - "no": 1
      title: Définition des polynômes
      page: 0
      pdf_page: 8
    - "no": 2
      title: Degrés
      page: 2
      pdf_page: 9
    - "no": 3
      title: Substitutions
      page: 4
      pdf_page: 11
    - "no": 4
      title: Différentielles et dérivations
      page: 6
      pdf_page: 13
    - "no": 5
      title: Diviseurs de zéro dans un anneau de polynômes
      page: 8
      pdf_page: 15
    - "no": 6
      title: Division euclidienne des polynômes à une indéterminée
      page: 10
      pdf_page: 17
    - "no": 7
      title: Divisibilité des polynômes à une indéterminée¹
      page: 0
      pdf_page: 18
    - "no": 8
      title: Polynômes irréductibles
      page: 13
      pdf_page: 20
statements: 30
exercises: 6
content_sha256: 3ce7b549cf06b07802cd50498dea7e2f4b7ead610ff4dd91377872cb26fa1b03
---

## § 1. POLYNÔMES

### 1. Définition des polynômes

Soit I un ensemble. Rappelons (III, p. 25) que l’algèbre commutative libre de I sur A se note $A[(X_i)_{i \in I}]$ ou $A[X_i]_{i \in I}$. Les éléments de cette algèbre sont appelés polynômes par rapport aux indéterminées $X_i$ (ou en les indéterminées $X_i$) à coefficients dans A. Rappelons que l’indéterminée $X_i$ est l’image canonique de $i$ dans l’algèbre commutative libre de I sur A ; il est parfois commode de désigner cette image par une autre notation, telle que $X'_i$, $Y_i$, $T_i$, etc. On annonce souvent cette convention par une phrase telle que : « Soit $Y = (Y_i)_{i \in I}$ une famille d’indéterminées » ; lorsqu’il en est ainsi, on note $A[Y]$ l’algèbre de polynômes considérée. Pour $I = \{1, 2, ..., n\}$, on écrit $A[X_1, X_2, ..., X_n]$ au lieu de $A[(X_i)_{i \in I}]$.

Pour $v \in \mathbf{N}^{(I)}$, posons

$$
X^v = \prod_{i \in I} X_i^{v_i}
$$

Alors $(X^v)_{v \in \mathbf{N}^{(I)}}$ est une base du A-module $A[(X_i)_{i \in I}]$. Les $X^v$ s’appellent les monômes en les indéterminées $X_i$. Pour $v = 0$, on obtient l’élément unité de $A[(X_i)_{i \in I}]$. Tout polynôme $u \in A[(X_i)_{i \in I}]$ s’écrit d’une façon et d’une seule sous la forme

$$
u = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v
$$

avec $\alpha_v \in A$ et les $\alpha_v$ nuls sauf pour un nombre fini d’indices ; les $\alpha_v$ s’appellent les coefficients de $u$ ; les $\alpha_v X^v$ s’appellent les termes de $u$ (l’élément $\alpha_v X^v$ étant souvent appelé le terme en $X^v$) ; en particulier le terme $\alpha_0 X^0$, identifié à $\alpha_0$, s’appelle le terme constant de $u$. Lorsque $\alpha_v = 0$, on dit, par abus de langage, que $u$ ne contient pas de terme en $X^v$ ; en particulier, quand $\alpha_0 = 0$, on dit que $u$ est un polynôme sans terme constant (III, p. 26). On appelle polynôme constant tout multiple scalaire de 1.

Soient B un anneau commutatif, et $\rho : A \to B$ un homomorphisme d’anneaux. Considérons $B[(X_i)_{i \in I}]$ comme une A-algèbre grâce à $\rho$. Alors l’application $\sigma$ de $A[(X_i)_{i \in I}]$ dans $B[(X_i)_{i \in I}]$ qui transforme $\sum \alpha_v X^v$ en $\sum \rho(\alpha_v) X^v$ est un homomorphisme de A-algèbres ; si $u \in A[(X_i)_{i \in I}]$, on note parfois $^\rho u$ l’image de $u$ par cet homomorphisme. L’homomorphisme de $B \otimes_A A[(X_i)_{i \in I}]$ dans $B[(X_i)_{i \in I}]$ défini canoniquement par $\sigma$ transforme, pour tout $i \in I$, $1 \otimes X_i$ en $X_i$; c’est un isomorphisme de B-algèbres (III, p. 22).

Soit M un A-module libre de base $(e_i)_{i \in I}$. Il existe un homomorphisme unifère $\varphi$ et un seul de l’algèbre symétrique $S(M)$ dans l’algèbre $A[(X_i)_{i \in I}]$ tel que $\varphi(e_i) = X_i$ pour tout $i \in I$, et cet homomorphisme est un isomorphisme (III, p. 75). Cet isomorphisme est dit canonique. Cela permet d’appliquer aux algèbres de polynômes certaines propriétés des algèbres symétriques. Par exemple, soit $(\lambda_\lambda)_{\lambda \in \Lambda}$ une partition de I. Soit $\varphi_\lambda$ l’homomorphisme de $P_\lambda = A[(X_i)_{i \in I_\lambda}]$ dans $P = A[(X_i)_{i \in I}]$ qui transforme $X_i$ (considéré comme élément de $P_\lambda$) en $X_i$ (considéré comme élément de P). Alors les $\varphi_\lambda$ définissent un homomorphisme de l’algèbre $\bigotimes_{\lambda \in \Lambda} P_\lambda$ dans l’algèbre P, et cet homomorphisme est un isomorphisme (III, p. 73, prop. 9).

Soit E un A-module. On pose $E \otimes_A A[(X_i)_{i \in I}] = E[(X_i)_{i \in I}]$. Les éléments du A-module $E[(X_i)_{i \in I}]$ s’appellent polynômes en les indéterminées $X_i$ à coefficients dans E. Un tel polynôme s’écrit d’une façon et d’une seule $\sum_{v \in \mathbf{N}^{(I)}} e_v \otimes X^v$, où $e_v \in E$ et où les $e_v$ sont nuls sauf pour un nombre fini d’indices ; le plus souvent, on écrira $e_v X^v$ pour $e_v \otimes X^v$.

### 2. Degrés

Soit $P = A[(X_i)_{i \in I}]$ une algèbre de polynômes. Pour tout entier $n \in \mathbf{N}$, soit $P_n$ le sous-module de P engendré par les monômes $X^v$ tels que $|v| = \sum_{i \in I} v_i$ soit égal à $n$. Alors $(P_n)_{n \in \mathbf{N}}$ est une graduation qui fait de $A[(X_i)_{i \in I}]$ une algèbre graduée de type $\mathbf{N}$ (III, p. 31). Les éléments homogènes de degré $n$ de $A[(X_i)_{i \in I}]$ sont parfois appelés formes de degré $n$ par rapport aux indéterminées $X_i$.

Lorsqu’il sera question de degré de polynômes non homogènes, nous conviendrons généralement d’adjoindre à l’ensemble $\mathbf{N}$ des entiers naturels un élément noté $-\infty$ et de prolonger à $\mathbf{N} \cup \{-\infty\}$ la relation d’ordre et l’addition de $\mathbf{N}$ par les conventions suivantes, où $n \in \mathbf{N}$,

$$
-\infty < n , \quad (-\infty) + n = n + (-\infty) = -\infty , \quad (-\infty) + (-\infty) = -\infty .
$$

Soit $u = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$ un polynôme. La composante homogène $u_n$ de degré $n$ de $u$ (pour la graduation de type $\mathbf{N}$ définie ci-dessus) est égale à $\sum_{|v|=n} \alpha_v X^v$, et l’on a évidemment $u = \sum_{n \in \mathbf{N}} u_n$. Lorsque $u \neq 0$, les $u_n$ ne sont pas tous nuls, et l’on appelle degré (ou degré total) de $u$, et l’on note $\deg u$, le plus grand des entiers $n$ tels que $u_n \neq 0$; autrement dit (III, p. 26), le degré de $u$ est le plus grand des entiers $|\nu|$ pour les multiindices $\nu$ tels que $\alpha_\nu \neq 0$. Lorsque $u = 0$, le degré de $u$ est égal par convention à $-\infty$. Pour tout entier $p \in \mathbf{N}$, la relation $\deg u \leq p$ équivaut donc à « $\alpha_\nu = 0$ pour tout multiindice $\nu$ tel que $|\nu| > p$ » ; l’ensemble des polynômes $u$ tels que $\deg u \leq p$ est donc un sous-A-module de $A[(X_i)_{i \in I}]$, égal à $P_0 + P_1 + \cdots + P_p$ avec les notations ci-dessus.

Soit E un A-module. La famille $(E \otimes P_n)_{n \in \mathbf{N}}$ est une graduation de type $\mathbf{N}$ du module $E[(X_i)_{i \in I}] = E \otimes_A A[(X_i)_{i \in I}]$ des polynômes à coefficients dans E. On étend à ce cas les conventions adoptées plus haut pour le degré des polynômes non homogènes.

#### Proposition 1 {#alg-iv-s1-prop-1 .statement}

*Soient u et v deux polynômes.*

(i) *Si $\deg u \neq \deg v$, on a*

$$
u + v \neq 0 \quad \text{et} \quad \deg(u + v) = \sup(\deg u, \deg v) .
$$

*Si $\deg u = \deg v$, on a* $\deg(u + v) \leq \deg u$.

(ii) *On a* $\deg(uv) \leq \deg u + \deg v$.

Les démonstrations sont immédiates.

Soient $J \subset I$ et $B = A[(X_i)_{i \in I - J}]$. Identifions $A[(X_i)_{i \in I}]$ à $B[(X_i)_{i \in J}]$ (III, p. 26). Le degré de $u \in A[(X_i)_{i \in I}]$, considéré comme élément de $B[(X_i)_{i \in J}]$, s’appelle le degré de $u$ par rapport aux $X_i$ d’indice $i \in J$ (III, p. 27).

Soit $u = \sum_{k=0}^n \alpha_k X_k \in A[X]$ un polynôme non nul en une indéterminée, de degré $n$. Le coefficient $\alpha_n$, qui est par hypothèse $\neq 0$, s’appelle le *coefficient dominant* de $u$. Un polynôme $u \neq 0$ dont le coefficient dominant est égal à 1 s’appelle un *polynôme unitaire*.

Dans $A[X_1, X_2, ..., X_q]$, le nombre de monômes de degré total $p$ est égal au nombre d’éléments $(n_k)_{1 \leq k \leq q}$ de $\mathbf{N}^q$ tels que $\sum_{k=1}^q n_k = p$, c’est-à-dire à $\binom{q+p-1}{p}$ (E, III, p. 44, prop. 15).

Plus généralement, soient $\Delta$ un monoïde commutatif et $(\delta_i)_{i \in I}$ une famille d’éléments de $\Delta$. Il existe une unique graduation de type $\Delta$ de l’algèbre $A[(X_i)_{i \in I}]$ telle que chaque monôme $X^\nu$ soit de degré $\sum_{i \in I} \nu_i \delta_i$ (III, p. 31, exemple 3). Le cas considéré ci-dessus est celui où $\Delta = \mathbf{N}$ et $\delta_i = 1$. Dans le cas général, pour éviter des confusions, nous utiliserons le mot « poids » au lieu de « degré », et le mot « isobare » au lieu de « homogène ». Par exemple, il existe une unique graduation de type $\mathbf{N}$ de l’algèbre $A[(X_i)_{i \geq 1}]$ telle que $X_i$ soit de poids $i$ pour tout entier $i \geq 1$. Les éléments isobares de poids $n$ sont les polynômes de la forme $\sum_\nu a_\nu X^\nu$ avec $a_\nu = 0$ lorsque $\sum_{i \geq 1} i \cdot \nu_i \neq n$.

### 3. Substitutions

Soient E une algèbre associative unifère sur A, $x = (x_i)_{i \in I}$ une famille d’éléments de E deux à deux permutables. Soit $X = (X_i)_{i \in I}$ une famille d’indéterminées. D’après III, p. 22, prop. 7, il existe un unique homomorphisme unifère $f$ de $A[X]$ dans E tel que $f(X_i) = x_i$ pour tout $i \in I$. L’image d’un élément $u$ de $A[X]$ par $f$ se note $u(x)$ et s’appelle l’élément de E déduit par substitution des $x_i$ aux $X_i$ dans $u$, ou la valeur de $u$ pour les valeurs $x_i$ des $X_i$, ou encore la valeur de $u$ pour $X_i = x_i$. En particulier, $u = u((X_i)_{i \in I})$. Si $I = \{1, ..., n\}$, on écrit $u(x_1, ..., x_n)$ au lieu de $u((x_i)_{i \in I})$. Plus généralement, si M est un A-module et si $v$ est un élément de

$$
M[(X_i)_{i \in I}] = M \otimes_A A[(X_i)_{i \in I}] ,
$$

on note $v(x)$ l’image de $v$ dans $M \otimes_A E = M_{(E)}$ par l’application $1_M \otimes f$.

Si l’homomorphisme $u \mapsto u(x)$ de $A[X]$ dans E est injectif, on dit que la famille x est algébriquement libre sur A, ou que les $x_i$ sont algébriquement indépendants sur A. Cela signifie aussi que les monômes $x^\nu$ ($\nu \in \mathbf{N}^{(I)}$) sont linéairement indépendants sur A.

Si $\lambda$ est un homomorphisme unifère de E dans une A-algèbre associative unifère $E'$, on a

(1)
$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i)_{i \in I})) ,
$$
car $\lambda \circ f$ est un homomorphisme de $A[X]$ dans $E'$ qui transforme $X_i$ en $\lambda(x_i)$.

Soit $u \in A[X]$. Si E est commutative, l’application $x \mapsto u(x)$ de $E^I$ dans E s’appelle la fonction polynomiale définie par $u$ (et l’algèbre E) ; on la note parfois $\tilde{u}$ (ou même simplement $u$).

Soit $Y = (Y_j)_{j \in J}$ une autre famille d’indéterminées. Prenons pour E l’algèbre de polynômes $A[Y]$. Soit $u \in A[X]$; pour $i \in I$, soit $g_i \in A[Y]$ et posons $g = (g_i)_{i \in I}$; soit $u(g) \in A[Y]$ le polynôme obtenu par substitution des polynômes $g_i$ aux $X_i$ dans le polynôme $u$. Soit $y = (y_j)_{j \in J}$ une famille d’éléments deux à deux permutables d’une A-algèbre associative unifère $E'$; appliquons (1) en prenant pour $\lambda$ l’homomorphisme $g \mapsto g(y)$ de E dans $E'$; on obtient :

(2)
$$
(u(g))(y) = u((g_i(y))) .
$$

Si $f = (f_i)_{i \in I} \in (A[(X_j)_{j \in J}])^J$ et $g = (g_j)_{j \in J} \in (A[(Y_k)_{k \in K}])^J$, on note $f \circ g$, ou $f(g)$, la famille de polynômes $(f_i(g))_{i \in I} \in (A[(Y_k)_{k \in K}])^I$. Si l’on désigne par $\tilde{f}$ l’application $x \mapsto (f_i(x))_{i \in I}$ de ${E'}^J$ dans ${E'}^I$ (où $E'$ est une A-algèbre unifère associative et commutative), la relation (2) entraîne

(3)
$$
(\tilde{f} \circ g) \sim = \tilde{f} \circ \tilde{g} .
$$

Si $h = (h_k)_{k \in K} \in (A[(Z_l)_{l \in L}])^K$, il résulte de (2) que :

(4)
$$
f \circ (g \circ h) = (f \circ g) \circ h .
$$

#### Proposition 2 {#alg-iv-s1-prop-2 .statement}

Soit $\mathbf{a} = (a_i)_{i \in I}$ une famille d’éléments de $\mathbf{A}$ et soit $u \in \mathbf{A}[X]$. Soit $v$ le polynôme obtenu par substitution de $X_i + a_i$ à $X_i$ pour tout $i \in I$. Le terme constant de $v$ est égal à $u(\mathbf{a})$.

Le terme constant de $v$ est obtenu par la substitution de 0 à $X_i$ dans $v$ pour tout $i \in I$. La proposition résulte donc de la formule (2).

#### Corollaire 1 {#alg-iv-s1-prop-2-cor-1 .statement}

Soit $m$ l’idéal des polynômes $u \in \mathbf{A}[X]$ tels que $u(\mathbf{a}) = 0$. Alors $m$ est engendré par les polynômes $X_i - a_i$ (pour $i \in I$).

Il est clair qu’on a $X_i - a_i \in m$ pour tout $i \in I$. Soit $u \in m$ et soit $v$ comme dans la proposition 2. Comme $v$ est sans terme constant, il existe une famille à support fini $(P_i)_{i \in I}$ de polynômes dans $\mathbf{A}[X]$ telle que
$$
v(X) = \sum_{i \in I} X_i \cdot P_i(X)
$$
Substituons $X_i - a_i$ à $X_i$ pour tout $i \in I$ dans l’égalité précédente ; on trouve alors une relation de la forme $u(X) = \sum_{i \in I} (X_i - a_i) \cdot P'_i(X)$, d’où le corollaire.

#### Corollaire 2 {#alg-iv-s1-prop-2-cor-2 .statement}

Soient $X = (X_i)_{i \in I}$ et $Y = (Y_i)_{i \in I}$ deux familles d’indéterminées. L’ensemble $D$ des polynômes $u \in \mathbf{A}[X, Y]$ tels que $u(X, X) = 0$ est l’idéal de $\mathbf{A}[X, Y]$ engendré par les polynômes $X_i - Y_i$ (pour $i \in I$).

Ce corollaire résulte immédiatement du cor. 1 où l’on remplace $\mathbf{A}$ par $\mathbf{A}[Y]$ et $a_i$ par $Y_i$, en interprétant $\mathbf{A}[X, Y]$ comme l’anneau des polynômes en les $X_i$ à coefficients dans $\mathbf{A}[Y]$.

#### Proposition 3 {#alg-iv-s1-prop-3 .statement}

Soient $u \in \mathbf{A}[X]$ et $X.Z$ la famille $(X_i Z)_{i \in I}$ d’éléments de l’anneau de polynômes $\mathbf{A}[X][Z]$. Le coefficient de $Z^k$ dans $u(X.Z)$ est la composante homogène de degré $k$ de $u$, pour tout entier positif $k$.

Il suffit de démontrer la prop. lorsque $u$ est un monôme, auquel cas c’est immédiat.

#### Corollaire {#alg-iv-s1-n3-cor-1 .statement}

Pour qu’un polynôme $u \in \mathbf{A}[X]$ soit homogène de degré $k$, il faut et il suffit que l’on ait :
$$
u(X.Z) = u(X).Z^k .
$$

#### Remarque {#alg-iv-s1-n3-rem-1 .statement}

Soit $x \in \mathbf{A}'$. Soit $f$ l’application $u \mapsto u(x)$ de $\mathbf{A}[X]$ dans $\mathbf{A}$. Soit $M$ un $\mathbf{A}$-module. Considérons l’homomorphisme $1 \otimes f$ de $M[X] = M \otimes_A \mathbf{A}[X]$ dans $M \otimes_A \mathbf{A} = M$. Pour tout $v \in M[X]$, on a $(1 \otimes f)(v) = v(x)$. Si $v = \sum_{v \in \mathbf{N}^{(I)}} e_v X^v$, on a $v(x) = \sum_{v \in \mathbf{N}^{(I)}} x^v e_v$.

### 4. Différentielles et dérivations

Soit $B = A[(X_i)_{i \in I}]$. D’après III, p. 134, il existe, pour tout $i \in I$, une A-dérivation $D_i$ de B et une seule telle que

$$
D_i X_i = 1 , \quad D_i X_j = 0 \quad \text{pour } j \neq i .
$$

Le polynôme $D_i P$ s’appelle la dérivée partielle de $P$ par rapport à $X_i$; on le note aussi $D_{X_i} P$, ou $\frac{\partial P}{\partial X_i}$, ou $P'_{X_i}$. D’après III, p. 123, formule (21), on a, si $v = (v_j) \in \mathbf{N}^{(I)}$,

$$
D_i (X^v) = \begin{cases}
v_i X_i^{v_i - 1} \prod_{j \in I - \{i\}} X_j^{v_j} & \text{si } v_i > 0 \\
0 & \text{si } v_i = 0 .
\end{cases}
$$

On déduit de (6) que $D_i D_j = D_j D_i$ quels que soient $i, j \in I$. Pour $v = (v_i)_{i \in I} \in \mathbf{N}^{(I)}$, on pose $D^v = \prod_{i \in I} D_i^{v_i}$ et $v! = \prod_{i \in I} (v_i!)$. Munissons $\mathbf{N}^{(I)}$ de l’ordre produit. On a

$$
D^v (X^\mu) = \begin{cases}
\frac{\mu!}{(\mu - v)!} X^{\mu - v} & \text{si } v \leq \mu , \\
0 & \text{sinon} .
\end{cases}
$$

Lorsque $P$ est un polynôme en une seule indéterminée $X$, l’unique dérivée partielle de $P$ se note $DP$ ou $\frac{dP}{dX}$ ou $P'$, et s’appelle simplement la dérivée de $P$.

Soit à nouveau $B = A[(X_i)_{i \in I}]$. D’après III, p. 134, le B-module $\Omega_A(B)$ des A-différentielles de B admet pour base la famille $(dX_i)_{i \in I}$ des différentielles des $X_i$. Soit $\partial_i$ la forme coordonnée d’indice $i$ relativement à cette base sur $\Omega_A(B)$. Alors l’application $u \mapsto \langle \partial_i, du \rangle$ de B dans B est une dérivation de B qui transforme $X_i$ en 1 et $X_j$ en 0 pour $j \neq i$, donc est $D_i$; autrement dit, on a

$$
du = \sum_{i \in I} (D_i u) \, dX_i
$$

pour tout $u \in B$. Si I est fini, $(D_i)_{i \in I}$ est une base du B-module des dérivations de B.

#### Proposition 4 {#alg-iv-s1-prop-4 .statement}

Soient E une A-algèbre associative, commutative et unifère, $x = (x_i)_{i \in I}$ une famille d’éléments de E, $u$ un élément de $A[(X_i)_{i \in I}]$, et $y = u(x)$. Pour toute dérivation D de E dans un E-module, on a

$$
D_y = \sum_{i \in I} (D_i u)(x) . D_{x_i} .
$$

Il suffit de prouver la proposition quand $u$ est un monôme, et elle résulte alors de (6) et de III, p. 123, prop. 6.

#### Corollaire {#alg-iv-s1-n4-cor-1 .statement}

Soient $f \in \mathbf{A}[X_1, ..., X_p]$ et $g_i \in \mathbf{A}[Y_1, ..., Y_q]$ pour $1 \leq i \leq p$. Posons $h = f(g_1, ..., g_p)$. Alors, pour $1 \leq j \leq q$, on a

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j}.
$$

C’est le cas particulier $E = \mathbf{A}[Y_1, ..., Y_q]$, $x_i = g_i$ et $D = \partial / \partial Y_j$ de la prop. 4.

Soient $\mathbf{X} = (X_i)_{i \in I}$, $\mathbf{Y} = (Y_i)_{i \in I}$ deux familles disjointes d’indéterminées. Notons $\mathbf{X} + \mathbf{Y}$ la famille $(X_i + Y_i)_{i \in I}$. Soit $u \in \mathbf{A}[\mathbf{X}]$. Considérons l’élément $u(\mathbf{X} + \mathbf{Y})$ de $\mathbf{A}[\mathbf{X}, \mathbf{Y}]$. Pour $v \in \mathbf{N}^{(I)}$, on note $\Delta^v u$ le coefficient de $\mathbf{Y}^v$ dans $u(\mathbf{X} + \mathbf{Y})$, considéré comme polynôme en les $Y_i$ à coefficients dans $\mathbf{A}[\mathbf{X}]$. On a par définition $\Delta^v u \in \mathbf{A}[\mathbf{X}]$ et

$$
u(\mathbf{X} + \mathbf{Y}) = \sum_v (\Delta^v u) (\mathbf{X}) \mathbf{Y}^v.
$$

(Ici et dans la suite de ce numéro, les sommations portent sur l’ensemble d’indices $\mathbf{N}^{(I)}$, sauf mention du contraire.)

Soit $a \in \mathbf{A}^I$. En substituant $a$ à $\mathbf{X}$ et $\mathbf{X} - a$ à $\mathbf{Y}$ dans (9), on obtient

$$
u(\mathbf{X}) = \sum_v (\Delta^v u) (a) (\mathbf{X} - a)^v.
$$

En particulier, on a

$$
u(\mathbf{X}) = \sum_v (\Delta^v u) (0) \mathbf{X}^v.
$$

Si $u, v \in \mathbf{A}[\mathbf{X}]$, on a

$$
(uv)(\mathbf{X} + \mathbf{Y}) = (\sum_v (\Delta^v u) (\mathbf{X}) \mathbf{Y}^v) (\sum_\rho (\Delta^\rho v) (\mathbf{X}) \mathbf{Y}^\rho)
= \sum_\sigma \left[ \sum_{v+\rho=\sigma} (\Delta^v u) (\mathbf{X}) (\Delta^\rho v) (\mathbf{X}) \right] \mathbf{Y}^\sigma
$$

donc

$$
\Delta^\sigma (uv) = \sum_{v+\rho=\sigma} (\Delta^v u) (\Delta^\rho v).
$$

Soit $\mathbf{Z} = (Z_i)_{i \in I}$ une autre famille d’indéterminées. On a :

$$
\sum_v (\Delta^v u) (\mathbf{X}) (\mathbf{Y} + \mathbf{Z})^v = u(\mathbf{X} + \mathbf{Y} + \mathbf{Z})
= \sum_\sigma (\Delta^\sigma u) (\mathbf{X} + \mathbf{Y}) \mathbf{Z}^\sigma
= \sum_{\rho, \sigma} (\Delta^\rho \Delta^\sigma u) (\mathbf{X}) \mathbf{Y}^\rho \mathbf{Z}^\sigma,
$$

donc, d’après I, p. 94, corollaire 2 :

$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \sigma!} \Delta^{\rho+\sigma} u.
$$

#### Proposition 5 {#alg-iv-s1-prop-5 .statement}

Quels que soient $u \in A[X]$ et $v \in \mathbf{N}^{(l)}$, on a

$$
D^v u = v! \Delta^v u .
$$

Supposons d’abord que $v$ soit de longueur 1 ; il existe alors un élément $i$ de $I$ tel que $v = \varepsilon_i$, c’est-à-dire $v_i = 1$ et $v_j = 0$ pour tout $j \neq i$ dans $I$. La formule (12) montre que $\Delta^{\varepsilon_i}$ est une dérivation de la $A$-algèbre $A[X]$, qui annule évidemment $X_j$ pour $j \neq i$ et prend la valeur 1 sur $X_i$. On a donc $\Delta^{\varepsilon_i} = D_i$ pour tout $i \in I$.

D’après la formule (13), on a

$$(14)$$
$$(\rho! \Delta^\rho).( \sigma! \Delta^\sigma ) = (\rho + \sigma)! \Delta^{\rho+\sigma}$$

dans l’algèbre des endomorphismes du $A$-module $A[X]$. On en déduit $v! \Delta^v = D^v$ par récurrence sur la longueur de $v$.

Si $A$ est une $\mathbf{Q}$-algèbre, les formules (9), (10), (11) peuvent donc s’écrire

$$(15)$$
$$u(X + Y) = \sum_v \frac{1}{v!} (D^v u)(X) Y^v$$

$$(16)$$
$$u(X) = \sum_v \frac{1}{v!} (D^v u)(a) (X - a)^v$$

$$(17)$$
$$u(X) = \sum_v \frac{1}{v!} (D^v u)(0) X^v .$$

Les formules (15), (16), (17) s’appellent toutes trois « formule de Taylor ».

#### Proposition 6 (« identité d’Euler ») {#alg-iv-s1-prop-6 .statement}

Soit $u \in A[X]$ un polynôme homogène de degré $r$. On a

$$\sum_{i \in I} X_i . D_i u = ru .$$

Soit $D$ l’application $A$-linéaire de $A[X]$ dans lui-même telle que $D(v) = sv$ quand $v$ est homogène de degré $s$. On sait (III, p. 119, exemple 6) que $D$ est une dérivation de $A[X]$. La prop. 6 est donc un corollaire de la prop. 4 (IV, p. 6).

### 5. Diviseurs de zéro dans un anneau de polynômes

#### Proposition 7 {#alg-iv-s1-prop-7 .statement}

Soient $f \in A[X]$ un polynôme non nul en une indéterminée, $\alpha$ son coefficient dominant. Si $\alpha$ est simplifiable dans $A$ (en particulier si $f$ est unitaire), on a, pour tout élément non nul $g$ de $A[X]$,

$$ fg \neq 0 \quad \text{et} \quad \deg(fg) = \deg f + \deg g .$$

Soient $g \in A[X]$ un polynôme non nul, $\beta$ son coefficient dominant, $n = \deg f$, $p = \deg g$. Alors le coefficient de $X^{n+p}$ dans $fg$ est $\alpha \beta$ donc est non nul, d’où la proposition.

#### Proposition 8 {#alg-iv-s1-prop-8 .statement}

Si $A$ est intègre, $A[(X_i)_{i \in I}]$ est intègre.

Soient $u, v$ deux éléments non nuls de $A[(X_i)_{i \in I}]$. Il s’agit de prouver la relation $uv \neq 0$. Or $u$ et $v$ appartiennent à un même anneau $A[(X_j)_{j \in J}]$ où $J$ est une partie finie de $I$. On peut donc se borner au cas où $I$ est fini et égal à $\{ 1, 2, ..., p \}$. D’autre part, l’anneau $A[X_1, ..., X_p]$ est isomorphe à l’anneau des polynômes en $X_p$ à coefficients dans $A[X_1, ..., X_{p-1}]$. Par récurrence sur $p$, on est donc ramené à démontrer la proposition pour $A[X]$, et il suffit alors d’appliquer la proposition 7.

#### Corollaire 1 {#alg-iv-s1-prop-8-cor-1 .statement}

Si $A$ est intègre, et si $u, v$ sont des éléments de $A[(X_i)_{i \in I}]$, on a $\deg(uv) = \deg u + \deg v$.

On peut se limiter au cas où $u$ et $v$ sont non nuls. Soient $m = \deg u, n = \deg v$. On a

$$
u = u_0 + u_1 + \cdots + u_m, \quad v = v_0 + v_1 + \cdots + v_n
$$

où $u_h$ (resp. $v_h$) est la composante homogène de degré $h$ de $u$ (resp. $v$). Comme $u_m \neq 0$ et $v_n \neq 0$, on a $u_m v_n \neq 0$ (prop. 8). Or $uv = u_m v_n + w$ avec $\deg w < m + n$, d’où le corollaire.

#### Corollaire 2 {#alg-iv-s1-prop-8-cor-2 .statement}

Si $A$ est intègre, les éléments inversibles de $A[(X_i)_{i \in I}]$ sont les éléments inversibles de $A$.

Cela résulte aussitôt du cor. 1.

#### Proposition 9 {#alg-iv-s1-prop-9 .statement}

Soit $u \in A[(X_i)_{i \in I}]$. Pour que $u$ soit nilpotent dans l’anneau $A[(X_i)_{i \in I}]$, il faut et il suffit que tous ses coefficients soient nilpotents dans l’anneau $A$.

Comme dans la démonstration de la prop. 8, on se ramène au cas des polynômes en une variable $X$. Si tous les coefficients de $u$ sont nilpotents, $u$ est nilpotent (I, p. 95, cor. 3). Supposons $u$ nilpotent non nul, et soit $n$ son degré. Nous raisonnons par récurrence sur $n$. Soit $\alpha$ le coefficient dominant de $u$. Il existe un entier $m > 0$ tel que $u^m = 0$. Le coefficient dominant de $u^m$ est $\alpha^m$, donc $\alpha^m = 0$. Alors $u - \alpha X^n$ est nilpotent (I, loc. cit.), et l’hypothèse de récurrence prouve que tous les coefficients de $u - \alpha X^n$ sont nilpotents. Ainsi, tous les coefficients de $u$ sont nilpotents.

#### Remarque {#alg-iv-s1-n5-rem-1 .statement}

Soient $u$ et $v$ des éléments de $A[(X_i)_{i \in I}]$. On suppose que $A$ est intègre, que $v$ est multiple non nul de $u$, et que $v$ est homogène. Alors $u$ est homogène. En effet, soit $u' \in A[(X_i)_{i \in I}]$ tel que $v = uu'$; on a $u \neq 0, u' \neq 0$; soient

$$
u = u_h + u_{h+1} + \cdots + u_k \\
u' = u_{h'} + u_{h'+1} + \cdots + u_{k'}
$$

les décompositions de $u$ et $u'$ en composantes homogènes, avec $u_h \neq 0, u_k \neq 0, u_{h'} \neq 0, u_{k'} \neq 0$. Alors $v = u_h u_{h'} + u_h u_{h'+1} + \cdots + u_k u_{k'}$ et $u_h u_{h'}$ est homogène non nul de degré $h + h'$, $u_k u_{k'}$ est homogène non nul de degré $k + k'$ (prop. 8). Comme $v$ est homogène, on a $h + h' = k + k'$, d’où $h = k, h' = k'$.

### 6. Division euclidienne des polynômes à une indéterminée

#### Proposition 10 {#alg-iv-s1-prop-10 .statement}

Soient $f$ et $g$ des éléments non nuls de $\mathbf{A}[X]$ de degrés respectifs $m$ et $n$. Soient $\alpha_0$ le coefficient dominant de $f$, et $\mu = \sup(n - m + 1, 0)$. Il existe $u, v \in \mathbf{A}[X]$ tels que

$$
\alpha_0^\mu g = uf + v , \quad \deg v < m .
$$

Si $\alpha_0$ est simplifiable dans $\mathbf{A}$, $u$ et $v$ sont déterminés de manière unique par ces propriétés.

L’existence de $u$ et $v$ est évidente quand $n < m$ puisqu’on peut alors prendre $u = 0$ et $v = g$. Pour $n \geq m$, démontrons-la par récurrence sur $n$. Soit $\beta$ le coefficient dominant de $g$. Si $f = \sum_{k=0}^m \alpha_k X^{m-k}$, on peut écrire $\alpha_0^\mu g = \alpha_0^{\mu-1} \beta X^{n-m} f + \alpha_0^{\mu-1} g_1$, où $g_1 \in \mathbf{A}[X]$ et $\deg g_1 < n$. D’après l’hypothèse de récurrence, il existe $u_1, v \in \mathbf{A}[X]$ tels que $\alpha_0^{\mu-1} g_1 = u_1 f + v$ et $\deg v < m$. Donc

$$
\alpha_0^\mu g = (\alpha_0^{\mu-1} \beta X^{n-m} + u_1) f + v
$$

et il suffit de poser $u = \alpha_0^{\mu-1} \beta X^{n-m} + u_1$.

Supposons que $\alpha_0$ soit simplifiable dans $\mathbf{A}$, et prouvons l’unicité de $u$ et $v$. Soient $u, v, u_1, v_1 \in \mathbf{A}[X]$ tels que

$$
\alpha_0^\mu g = uf + v = u_1 f + v_1 , \quad \deg v < m , \quad \deg v_1 < m .
$$

On a $(u - u_1) f = v_1 - v$ et $\deg(v_1 - v) < m$, donc $u - u_1 = 0$ (IV, p. 8, prop. 7) et par suite $v_1 - v = 0$.

#### Corollaire (« division euclidienne des polynômes ») {#alg-iv-s1-n6-cor-1 .statement}

Soient $f$ un élément non nul de $\mathbf{A}[X]$ dont le coefficient dominant est inversible, et $m = \deg f$.

(i) Pour tout $g \in \mathbf{A}[X]$, il existe $u, v \in \mathbf{A}[X]$ tels que

$$
g = uf + v , \quad \deg v < m .
$$

En outre, ces conditions déterminent $u$ et $v$ de manière unique.

(ii) Les sous-$\mathbf{A}$-modules $\mathbf{A} + \mathbf{A}X + \cdots + \mathbf{A}X^{m-1}$ et $f\mathbf{A}[X]$ de $\mathbf{A}[X]$ sont supplémentaires dans $\mathbf{A}[X]$.

(iii) Supposons $f$ non constant et considérons $\mathbf{A}[X]$ comme un $\mathbf{A}[T]$-module au moyen de l’homomorphisme $u(T) \mapsto u(f(X))$ de $\mathbf{A}[T]$ dans $\mathbf{A}[X]$. Alors $\mathbf{A}[X]$ est un $\mathbf{A}[T]$-module libre de base $(1, X, \ldots, X^{m-1})$.

Les assertions (i) et (ii) sont des conséquences immédiates de la prop. 10.

Prouvons (iii). Soit $\psi$ l’homomorphisme $v \mapsto v(f(X), X)$ de $\mathbf{A}[T, X]$ dans $\mathbf{A}[X]$. Considérons d’abord $\mathbf{A}[T, X]$ comme l’anneau des polynômes en $T$ à coefficients dans $\mathbf{A}[X]$; le cor. 1 de IV, p. 5, montre que le noyau $a$ de $\psi$ est l’idéal $(T - f(X))$ de $\mathbf{A}[T, X]$. Considérons maintenant $\mathbf{A}[T, X]$ comme l’anneau des polynômes en X à coefficients dans A[T] ; alors $\psi$ est une application A[T]-linéaire de A[T][X] dans A[X]. L’assertion (ii) ci-dessus (appliquée au polynôme $f(X) - T$ en X à coefficients dans A[T]) montre que (1, X, ..., $X^{m-1}$) est une base d’un A[T]-sous-module de A[T, X] supplémentaire de a. Comme on a $\psi(X^i) = X^i$ pour tout entier $i \geqslant 0$, on en déduit aussitôt (iii).

Avec les notations de (i), on dit que u est le quotient et v le reste de la division euclidienne de g par f ; pour que le reste soit nul, il faut et il suffit que f divise g.

### 7. Divisibilité des polynômes à une indéterminée¹

#### Proposition 11 {#alg-iv-s1-prop-11 .statement}

Soit K un corps commutatif.

(i) Pour tout idéal non nul a de K[X], il existe un polynôme unitaire f dans K[X], et un seul, tel que a = (f).

(ii) Soient $f_1$ et $f_2$ dans K[X]. Pour que $(f_1) = (f_2)$, il faut et il suffit qu’il existe un élément non nul $\lambda$ de K tel que $f_2 = \lambda f_1$.

Prouvons (ii), la suffisance de la condition énoncée étant claire. Le cas où $f_1$ et $f_2$ engendrent l’idéal nul est trivial. Supposons donc que les polynômes non nuls $f_1$ et $f_2$ engendrent le même idéal de K[X]. Il existe donc des polynômes $u_1$ et $u_2$ tels que $f_1 = u_1 f_2$ et $f_2 = u_2 f_1$; on en déduit $u_1 u_2 = 1$, d’où $\deg u_1 + \deg u_2 = 0$, et par suite $\deg u_2 = 0$. On a donc prouvé que $u_2$ est un élément non nul de K.

Prouvons (i). Soit dans a un polynôme unitaire f de degré le plus petit possible. Étant donné g dans a, soient u et v le quotient et le reste de la division euclidienne de g par f ; alors $v = g - u f$ appartient à a et l’on a $\deg v < \deg f$; si v était non nul, il existerait un élément non nul $\lambda$ de K tel que $\lambda v$ soit unitaire, et comme $\lambda v$ appartiendrait à a, ceci contredirait la définition de f. On a donc a = (f). L’unicité d’un polynôme unitaire f tel que a = (f) résulte de (ii).

#### Proposition 12 {#alg-iv-s1-prop-12 .statement}

Soient K un corps commutatif et f, g deux éléments de K[X]. Pour tout polynôme d dans K[X], les propriétés suivantes sont équivalentes :

(i) Le polynôme d divise f et g, et tout polynôme qui divise à la fois f et g divise d.

(ii) Le polynôme d divise f et g, et il existe deux polynômes u et v tels que $d = u f + v g$.

(iii) On a la relation $(d) = (f) + (g)$ entre idéaux de K[X].

Le polynôme d est déterminé par ces propriétés, à la multiplication près par un élément non nul de K. Si f et g ne sont pas tous deux nuls, on a $d \neq 0$ et le degré de d majore le degré de tout polynôme divisant à la fois f et g.

Lorsque f et g sont nuls, chacune des propriétés (i) à (iii) est satisfaite dans le seul cas où $d = 0$, donc elles sont équivalentes. Nous supposerons désormais que f et g ne sont pas tous deux nuls, et nous noterons a l’idéal $(f) + (g)$ de K[X].

¹ Le lecteur notera l’analogie entre les résultats de ce numéro et du suivant et les propriétés de divisibilité dans l’anneau Z des entiers (I, p. 106). Ils dépendent essentiellement du fait que, dans les anneaux Z et K[X], tout idéal est principal, comme nous le verrons au chapitre VII, § 1.

Remarquons que, quels que soient les polynômes $u$ et $v$ dans $\mathbf{K}[X]$, les propriétés $(u) \supset (v)$ et « $u$ divise $v$ » sont équivalentes. L’assertion (ii) équivaut donc à « $(d) \supset (f)$ et $(d) \supset (g)$ et $d \in (f) + (g)$ », c’est-à-dire à (iii). Il est clair que (ii) entraîne (i). Supposons enfin (i) satisfaite ; on a $(d) \supset (f)$ et $(d) \supset (g)$, d’où $(d) \supset a$ ; par ailleurs, d’après la prop. 11 (IV, p. 11), il existe un polynôme $d_1$ tel que $a = (d_1)$; comme le polynôme $d_1$ divise à la fois $f$ et $g$, il divise $d$ par hypothèse, d’où $(d) \subset a$ ; finalement, on a $(d) = a$, c’est-à-dire (iii).

Les autres assertions de la prop. 12 sont des conséquences immédiates de la prop. 11 appliquée à l’idéal $a = (f) + (g)$.

#### Définition 1 {#alg-iv-s1-def-1 .statement}

Avec les notations de la prop. 12, on dit que $d$ est un plus grand commun diviseur (en abrégé $pgcd$) de $f$ et $g$. On dit que $f$ et $g$ sont étrangers, ou premiers entre eux, ou que $f$ est étranger à $g$, ou premier à $g$, lorsque 1 est un $pgcd$ de $f$ et $g$.

Dire que $f$ et $g$ sont étrangers signifie donc qu’il existe des polynômes $u$ et $v$ dans $\mathbf{K}[X]$ tels que $uf + vg = 1$.

#### Corollaire 1 {#alg-iv-s1-def-1-cor-1 .statement}

Soient $d$ un $pgcd$ de $f$ et $g$, $\mathbf{K}'$ un corps commutatif contenant $\mathbf{K}$ comme sous-corps. Alors $d$ est un $pgcd$ de $f$ et $g$ considérés comme éléments de $\mathbf{K}'[X]$.

Cela résulte de la prop. 12, (iii).

#### Corollaire 2 {#alg-iv-s1-def-1-cor-2 .statement}

Soit $d$ un $pgcd$ de $f$ et $g$.
(i) Si $u \in \mathbf{K}[X]$, $du$ est un $pgcd$ de $fu$ et $gu$.
(ii) Si $v \in \mathbf{K}[X]$ est un diviseur non nul de $f$ et $g$, $d|v$ est un $pgcd$ de $f/v$ et $g/v$.

Cela résulte de la prop. 12, (ii).

#### Corollaire 3 {#alg-iv-s1-def-1-cor-3 .statement}

Soit $w$ un diviseur commun de $f$ et $g$. Pour que $w$ soit un $pgcd$ de $f$ et $g$, il faut et il suffit que $f/w$ et $g/w$ soient étrangers.

Cela résulte du cor. 2.

#### Corollaire 4 {#alg-iv-s1-def-1-cor-4 .statement}

Soient $f, g, h \in \mathbf{K}[X]$. Si $f$ divise $gh$ et est étranger à $g$, alors $f$ divise $h$.

En effet, $f$ divise $gh$ et $fh$; donc $f$ divise tout $pgcd$ de $gh$ et $fh$, en particulier $h$ (cor. 2, (i)).

#### Corollaire 5 {#alg-iv-s1-def-1-cor-5 .statement}

Soient $f, g \in \mathbf{K}[X]$. Pour que $f$ et $g$ soient étrangers, il faut et il suffit que l’image canonique de $g$ dans $\mathbf{K}[X]/(f)$ soit inversible.

En effet, cette condition signifie qu’il existe $u, v \in \mathbf{K}[X]$ tels que $uf + vg = 1$.

#### Corollaire 6 {#alg-iv-s1-def-1-cor-6 .statement}

Soient $f, g_1, g_2, \ldots, g_n \in \mathbf{K}[X]$. Si $f$ est étranger à $g_1, g_2, \ldots, g_n$, alors $f$ est étranger à $g_1 g_2 \cdots g_n$.

\* Corollaire 7. — Pour que $f$ et $g$ soient étrangers, il faut et il suffit qu’ils n’aient de racines communes dans aucune extension de $\mathbf{K}$.

En effet, si $d$ est un $pgcd$ de $f$ et $g$, les racines communes à $f$ et $g$ dans une extension $\mathbf{K}'$ de $\mathbf{K}$ sont les racines de $d$ dans $\mathbf{K}'$. Le corollaire résulte donc de V, p. 21, prop. 4. \*

### 8. Polynômes irréductibles

#### Définition 2 {#alg-iv-s1-def-2 .statement}

Soit $K$ un corps commutatif. On dit que $f \in K[X]$ est irréductible si $\deg f \geq 1$, et si $f$ n’est divisible par aucun polynôme $g$ tel que $0 < \deg g < \deg f$.

Il revient au même de dire que $\deg f \geq 1$ et que les seuls diviseurs de $f$ dans $K[X]$ sont les scalaires $\neq 0$ et les produits de $f$ par les scalaires $\neq 0$. Comme la relation $(f) \subset (g)$ signifie que $g$ divise $f$, on voit que les polynômes irréductibles de $K[X]$ peuvent encore être définis comme les polynômes $f$ tels que l’idéal $(f)$ soit maximal (I, p. 99).

Soient $f, g \in K[X]$. Si $f$ est irréductible, il est clair que ou bien $f$ et $g$ sont étrangers ou bien $f$ divise $g$. Si $f$ et $g$ sont irréductibles, ou bien $f$ et $g$ sont étrangers, ou bien chacun est le produit de l’autre par un scalaire $\neq 0$. En particulier, deux polynômes unitaires irréductibles distincts sont étrangers.

#### Proposition 13 {#alg-iv-s1-prop-13 .statement}

Soit $\mathcal{J}$ l’ensemble des polynômes unitaires irréductibles de $K[X]$. Soient $f$ un élément non nul de $K[X]$, $\alpha$ son coefficient dominant. Il existe une famille $(v_p)_{p \in \mathcal{J}}$ à support fini d’entiers positifs, et une seule, telle que l’on ait la décomposition

$$
f = \alpha \prod_{p \in \mathcal{J}} p^{v_p}.
$$

Il suffit de prouver la proposition lorsque $f$ est unitaire, c’est-à-dire lorsque $\alpha = 1$. Nous raisonnons par récurrence sur le degré $n$ de $f$, le cas $n = 0$ étant trivial. Supposons donc $n \geq 1$ et la proposition établie pour tous les polynômes de degré $< n$.

Soit $E$ l’ensemble des polynômes unitaires $\neq 1$ qui divisent $f$; on a $f \in E$, donc $E$ n’est pas vide, et il existe dans $E$ un polynôme $g$ de degré minimum. Il est clair que $g$ est irréductible et qu’il existe un polynôme unitaire $h$ de degré $< n$ tel que $f = gh$; d’après l’hypothèse de récurrence, $h$ est produit d’une famille finie de polynômes unitaires irréductibles, donc $f$ a la même propriété. Ceci prouve l’existence de la décomposition (18).

Prouvons maintenant l’unicité de la décomposition (18). Soit $(w_p)_{p \in \mathcal{J}}$ une famille à support fini d’entiers positifs, telle que $f = \prod_{p \in \mathcal{J}} p^{w_p}$. Comme $f$ est de degré $n \geq 1$, il existe $p$ dans $\mathcal{J}$ tel que $w_p > 0$; si l’on avait $v_p = 0$, alors $f$ serait produit d’une famille finie d’éléments de $\mathcal{J}$ distincts de $p$, donc serait étranger à $p$ (IV, p. 12, cor. 6) contrairement au fait que $p$ divise $f$. Par l’hypothèse de récurrence, le polynôme $f/p$ admet une unique décomposition du type (18); on en déduit aussitôt l’égalité $w_q = v_q$ pour tout $q \in \mathcal{J}$.

Soit $f$ un polynôme non nul dans $K[X]$. On dit que $f$ est sans facteur multiple si les exposants $v_p$ de la décomposition (18) sont tous $\leq 1$; il revient au même de dire que $f$ est le produit d’une suite finie de polynômes irréductibles deux à deux distincts, ou encore que $f$ n’est pas divisible par le carré d’un polynôme non constant de $K[X]$.

## EXERCICES {#alg-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
