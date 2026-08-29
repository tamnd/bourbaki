---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 8
section_title: NORMES ET TRACES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.45-A V.50, A V.146
pdf_pages: 0149-0154, 0250-0250
extraction: ocr
subsections:
    - "no": 1
      title: Rappels
      page: 45
      pdf_page: 149
    - "no": 2
      title: Normes et traces dans les algèbres étalées
      page: 46
      pdf_page: 150
    - "no": 3
      title: Normes et traces dans les extensions de degré fini
      page: 48
      pdf_page: 152
statements: 9
exercises: 2
content_sha256: d59ed32155d2c30fd69ac39c13a938a7e0c5ae6558f4ec8e8dea639176f48b42
---

## § 8. NORMES ET TRACES

Dans tout ce paragraphe, on note $K$ un corps.

### 1. Rappels

Soit $A$ une algèbre de degré fini $n$ sur $K$. Pour tout $x \in A$, notons $L_x$ l’application linéaire $a \mapsto xa$ de $A$ dans $A$. Rappelons (III, p. 110) que la trace de $L_x$ s’appelle la *trace* de $x$ relativement à $A$ et se note $\mathrm{Tr}_{A/K}(x)$; de même, le déterminant de $L_x$ s’appelle la *norme* de $x$ relativement à $A$ et se note $N_{A/K}(x)$. Le *discriminant* d’une suite $(x_1, \ldots, x_n)$ de $n$ éléments de $A$ est par définition le déterminant $D_{A/K}(x_1, \ldots, x_n)$ de la matrice $(\mathrm{Tr}_{A/K}(x_i x_j))_{1 \leq i, j \leq n}$ (III, p. 115).

Soit $K'$ une extension du corps $K$ et soit $A' = A_{(K')}$ la $K'$-algèbre déduite de $A$ par extension des scalaires. On a les formules

$$
\text{(1)} \qquad \mathrm{Tr}_{A'/K'}(1 \otimes x) = \mathrm{Tr}_{A/K}(x) \cdot 1 , \quad N_{A'/K'}(1 \otimes x) = N_{A/K}(x) \cdot 1
$$
pour tout $x \in A$ (III, p. 110). Pour toute suite $(x_1, \ldots, x_n)$ d’éléments de $A$, on a
$$
\text{(2)} \qquad D_{A'/K'}(1 \otimes x_1, \ldots, 1 \otimes x_n) = D_{A/K}(x_1, \ldots, x_n) \cdot 1 ,
$$
comme il résulte de la première formule (1).

### 2. Normes et traces dans les algèbres étalées

Soit $A$ une algèbre étale de degré (fini) $n$ sur $K$. Par définition, il existe donc une extension $L$ de $K$ et des homomorphismes distincts $u_1, \ldots, u_n$ de $A$ dans $L$ avec les propriétés suivantes :
*a*) tout homomorphisme de $A$ dans $L$ est égal à l’un des $u_i$ (V, p. 29, cor.);
*b*) il existe un isomorphisme de $L$-algèbres $u : A_{(L)} \to L^n$ tel que
$$
u(1 \otimes x) = (u_1(x), \ldots, u_n(x)) \text{ pour tout } x \in A .
$$
De plus, toute extension algébriquement close $L$ de $K$ a les propriétés précédentes (V, p. 29, prop. 2).

On fixe $L, u_1, \ldots, u_n$ dans la suite. Soit $x \in A$. On va prouver les formules
$$
\text{(3)} \qquad \mathrm{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) , \quad N_{A/K}(x) \cdot 1 = \prod_{i=1}^n u_i(x) .
$$
Soit $v$ la multiplication par $1 \otimes x$ dans $A_{(L)}$; par rapport à la base de $A_{(L)}$ image par $u^{-1}$ de la base canonique de $L^n$, la matrice de l’application linéaire $v$ est diagonale, d’éléments diagonaux $u_1(x), \ldots, u_n(x)$. On en déduit
$$
\mathrm{Tr}_{A_{(L)}/L}(1 \otimes x) \cdot 1 = \sum_{i=1}^n u_i(x) , \text{ d'où } \mathrm{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) \text{ d'après (1)} ;
$$
le cas des normes se traite de manière analogue.

Soit de plus $(x_1, \ldots, x_n)$ une suite d’éléments de $A$; soit $U$ la matrice
$$
(u_i(x_j))_{1 \leq i, j \leq n}
$$
et soit $(t_{ij}) = {}^t U . U$. D’après la première formule (3), on a
$$
\mathrm{Tr}_{A/K}(x_i x_j) \cdot 1 = \sum_{k=1}^n u_k(x_i x_j) = \sum_{k=1}^n u_k(x_i) u_k(x_j) = t_{ij} ;
$$
passant aux déterminants, on obtient
$$
\text{(4)} \qquad D_{A/K}(x_1, \ldots, x_n) \cdot 1 = [\det u_i(x_j)]^2 .
$$

#### Proposition 1 {#alg-v-s8-prop-1 .statement}

Soit $A$ une algèbre commutative de degré fini sur $K$. Les conditions suivantes sont équivalentes :

a) L’algèbre $A$ est étale.

b) Il existe une base de $A$ dont le discriminant est non nul.

c) Pour tout $x \neq 0$ dans $A$, il existe $y$ dans $A$ tel que $\mathrm{Tr}_{A/K}(xy) \neq 0$.

De plus, lorsque ces conditions sont remplies, le discriminant d’une base quelconque de $A$ est non nul.

Nous allons montrer que, $A$ étant supposée étale, le discriminant de $A$ par rapport à une base quelconque $(x_1, ..., x_n)$ de $A$ sur $K$ est non nul ; ceci établira en particulier l’implication $a) \Rightarrow b)$. D’après (4) et avec les notations précédentes, il suffit de montrer que la matrice $U$ est inversible, ou encore que le système d’équations linéaires

$$
\sum_{i=1}^n \lambda_i u_i(x_j) = 0 \quad (\text{pour } 1 \leq j \leq n)
$$

n’admet que la solution $\lambda_1 = \cdots = \lambda_n = 0$ dans $L$. Or la relation (5) entraîne

$$
\sum_{i=1}^n \lambda_i u_i(x) = 0 \text{ pour tout } x \in A,
$$
d’où $\lambda_i = 0$ pour $1 \leq i \leq n$ d’après le théorème d’indépendance linéaire des homomorphismes (V, p. 26, th. 1).

L’équivalence de b) et c) résulte du lemme général suivant :

#### Lemme 1 {#alg-v-s8-lem-1 .statement}

Soient $V$ un espace vectoriel de dimension finie sur $K$, et $B$ une forme bilinéaire sur $V \times V$. Soient $(v_1, ..., v_n)$ une base de $V$ sur $K$ et $\Delta = \det B(v_i, v_j)$. On a $\Delta \neq 0$ si et seulement si, pour tout $x \neq 0$ dans $V$, il existe $y$ dans $V$ avec $B(x, y) \neq 0$.

On a $\Delta \neq 0$ si et seulement si le système d’équations linéaires

$$
\sum_{i=1}^n \lambda_i B(v_i, v_j) = 0 \quad (1 \leq j \leq n)
$$

n’admet que la solution $\lambda_1 = \cdots = \lambda_n = 0$ dans $K$. Si l’on pose $x = \sum_{i=1}^n \lambda_i v_i$, le système précédent équivaut à $B(x, v_j) = 0$ pour $1 \leq j \leq n$, ou encore, comme $(v_1, ..., v_n)$ est une base de $V$ sur $K$, à $B(x, y) = 0$ pour tout $y \in V$, d’où le lemme.

Montrons que la condition c) entraîne que $A$ est réduite. Soit $x$ un élément nilpotent de $A$; pour tout $y \in A$, l’élément $xy$ de $A$ est nilpotent, et par suite l’endomorphisme $L_{xy}$ de l’espace vectoriel $A$ est nilpotent. Le lemme suivant entraîne alors $\mathrm{Tr}(xy) = 0$ pour tout $y \in A$, d’où $x = 0$ sous l’hypothèse c).

#### Lemme 2 {#alg-v-s8-lem-2 .statement}

Soient $V$ un espace vectoriel de dimension finie sur $K$ et $u$ un endomorphisme nilpotent de $V$. On a $\mathrm{Tr}(u) = 0$.

Pour tout entier $n \geq 0$, soit $V_n$ l’image de $u^n$. Comme $u$ est nilpotent, il existe un entier $r \geq 0$ tel que $V_0 = V, V_r = 0$ et $V_i \neq V_{i+1}$ pour $0 \leq i \leq r - 1$. Soit d_i la dimension de V_{i-1} (pour $1 \leq i \leq r$). Il existe une base $(x_1, ..., x_d)$ de V telle que les vecteurs $x_j$ avec $d - d_i < j \leq d$ forment une base de $V_{i-1}$ (pour $1 \leq i \leq r$). On a $u(V_{i-1}) \subset V_i$ et par suite les éléments diagonaux de la matrice de $u$ dans la base $(x_1, ..., x_d)$ sont nuls. On a alors $\operatorname{Tr}(u) = 0$, d’où le lemme.

Montrons enfin que b) entraîne a). Soit $(x_1, ..., x_n)$ une base de A sur K telle que $D_{A/K}(x_1, ..., x_n) \neq 0$. Soient K' une extension de K, A' la K'-algèbre déduite de A par extension des scalaires et $x'_i = 1 \otimes x_i$ pour $1 \leq i \leq n$. D’après la formule (2) (V, p. 46), on a $D_{A'/K'}(x'_1, ..., x'_n) \neq 0$. En appliquant le résultat précédent à A', on voit que A' est réduite. L’algèbre A est donc étale (V, p. 34, th. 4).

#### Corollaire {#alg-v-s8-n2-cor-1 .statement}

*Soit E une extension de degré fini de K. Pour que E soit séparable, il faut et il suffit qu’il existe a dans E tel que $\operatorname{Tr}_{E/K}(a) \neq 0$*.

La condition est nécessaire d’après la prop. 1. Inversement, supposons qu’il existe $a \in E$ tel que $\operatorname{Tr}_{E/K}(a) \neq 0$. Soit $x \neq 0$ dans E ; si l’on pose $y = ax^{-1}$, on a $\operatorname{Tr}_{E/K}(xy) \neq 0$. La prop. 1 montre alors que E est une algèbre étale sur K, donc une extension séparable de K.

### 3. Normes et traces dans les extensions de degré fini

Les formules de transitivité des normes et traces dans les algèbres (III, p. 114) entraînent la proposition suivante dans le cas des extensions de degré fini.

#### Proposition 2 {#alg-v-s8-prop-2 .statement}

*Soient F une extension de degré fini de K et E une sous-extension de F. Pour tout $x \in F$, on a*

$$
\operatorname{Tr}_{F/K}(x) = \operatorname{Tr}_{E/K}(\operatorname{Tr}_{F/E}(x))
$$
$$
N_{F/K}(x) = N_{E/K}(N_{F/E}(x)) .
$$

#### Corollaire {#alg-v-s8-n3-cor-1 .statement}

*Posons $m = [F : E]$. Pour tout $x \in E$, on a*

$$
\operatorname{Tr}_{F/K}(x) = m \cdot \operatorname{Tr}_{E/K}(x)
$$
$$
N_{F/K}(x) = N_{E/K}(x)^m .
$$

#### Proposition 3 {#alg-v-s8-prop-3 .statement}

*Soient E une extension de degré fini n de K et x un élément de E, de degré d sur K. Notons $f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ le polynôme minimal de x sur K. On a*

$$
\operatorname{Tr}_{E/K}(x) = - \frac{n}{d} a_1
$$
$$
N_{E/K}(x) = ((-1)^d a_d)^{n/d} = (-1)^n a_d^{n/d} .
$$

La prop. 3 résulte aussitôt du cor. de la prop. 2 et du lemme suivant :

#### Lemme 3 {#alg-v-s8-lem-3 .statement}

Soient $\mathbf{R}$ un anneau commutatif, $f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ un polynôme unitaire de $\mathbf{R}[X]$, $A$ la $\mathbf{R}$-algèbre $\mathbf{R}[X]/(f)$, et $x$ la classe de $X$ dans $A$. On a alors $\mathrm{Tr}_{A/\mathbf{R}}(x) = -a_1$ et $\mathrm{N}_{A/\mathbf{R}}(x) = (-1)^d a_d$.

D’après le cor. (IV, p. 10), la suite $(1, x, ..., x^{d-1})$ est une base de $A$; on a par ailleurs
$$
x.1 = x , \quad x.x = x^2 , \ldots , x.x^{d-2} = x^{d-1} , \quad x.x^{d-1} = -a_d.1 - a_{d-1}.x - \cdots - a_1.x^{d-1} .
$$
La matrice qui exprime la multiplication par $x$ par rapport à la base $(1, x, ..., x^{d-1})$ de $A$ est donc de la forme suivante (on a fait $d = 5$ pour fixer les idées) :

$$
\begin{pmatrix}
0 & 0 & 0 & 0 & -a_5 \\
1 & 0 & 0 & 0 & -a_4 \\
0 & 1 & 0 & 0 & -a_3 \\
0 & 0 & 1 & 0 & -a_2 \\
0 & 0 & 0 & 1 & -a_1
\end{pmatrix}.
$$

La trace de cette matrice est visiblement égale à $-a_1$; le déterminant se calcule en développant par rapport à la première ligne, et l’on trouve
$$
(-1)^{d-1}(-a_d) = (-1)^d a_d.
$$

Dans la suite de ce numéro, on note $E$ une extension de degré fini de $K$ et $x$ un élément de $E$. Nous allons indiquer comment calculer la norme et la trace de $x$ dans divers cas.

a) *Cas d’une extension séparable* : supposons $E$ séparable de degré $n$ sur $K$, notons $\Omega$ une clôture algébrique de $K$ et $\sigma_1, ..., \sigma_n$ les $n$ $K$-homomorphismes distincts de $E$ dans $\Omega$. D’après la formule (3) (V, p. 46), on a dans $\Omega$
$$
\mathrm{Tr}_{E/K}(x) = \sum_{i=1}^n \sigma_i(x) , \quad \mathrm{N}_{E/K}(x) = \prod_{i=1}^n \sigma_i(x) .
$$

b) *Cas d’une extension radicielle* : supposons $K$ de caractéristique $p > 0$ et l’extension $E$ radicielle ; il existe un entier $e \geqslant 0$ tel que $[E : K] = p^e$ (V, p. 25, prop. 4). Si $f$ est la hauteur de $x$ sur $K$, le polynôme minimal de $x$ sur $K$ est $X^{p^f} - x^{p^f}$ (V, p. 23, prop. 1). D’après la prop. 3, on a $\mathrm{N}_{E/K}(x) = (x^{p^f})^{p^e/p^f}$; d’où
$$
\mathrm{N}_{E/K}(x) = x^{p^e} = x^{[E : K]} .
$$
Pour la trace, on trouve $\mathrm{Tr}_{E/K}(x) = -p^{e-f} a$, où $a$ est le coefficient de $X^{p^f-1}$ dans le polynôme $X^{p^f} - x^{p^f}$; autrement dit, on a
$$
\mathrm{Tr}_{E/K}(x) = p^e.x = [E : K] x = \begin{cases} x & \text{si } [E : K] = 1 \\ 0 & \text{si } [E : K] > 1 \end{cases} .
$$

c) Cas général : on peut résumer le calcul de la norme et de la trace dans la proposition suivante :

#### Proposition 4 {#alg-v-s8-prop-4 .statement}

Soient $p$ l’exposant caractéristique de $K$ et $E$ une extension de degré fini de $K$. Soient $\sigma_1, ..., \sigma_n$ les $K$-homomorphismes distincts de $E$ dans une clôture algébrique $\Omega$ de $K$, et soit $p^e = [E : K]_i$. Pour tout $x \in E$, on a dans $\Omega$

$$
\text{Tr}_{E/K}(x) = p^e \cdot \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = (\prod_{i=1}^n \sigma_i(x))^{p^e}.
$$

Soit $E_s$ la fermeture séparable de $K$ dans $E$; alors $E_s$ est une extension séparable de degré $n$ de $K$, et $\sigma_1, ..., \sigma_n$ induisent des $K$-homomorphismes distincts de $E_s$ dans $\Omega$; de plus, $E$ est une extension radicielle de $E_s$, de degré $p^e$ (V, p. 42, prop. 13 et p. 45). La prop. 4 résulte alors des formules (6), (7), (13), (14) et (12).

## EXERCICES {#alg-v-s8-exercises}

See the [exercises for § 8](exercises/s8/).
