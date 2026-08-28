---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 1
section_title: Vecteurs de Witt
lang: fr
source: ac-viii-ix-fr
book_pages: AC IX.42-AC IX.68
pdf_pages: 0113-0129, 0154-0180
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes de Witt
      page: 0
      pdf_page: 113
    - "no": 2
      title: Les applications $f, v$ et $\Phi$
      page: 2
      pdf_page: 114
    - "no": 3
      title: Construction de polynômes
      page: 4
      pdf_page: 116
    - "no": 4
      title: L’anneau W(A) des vecteurs de Witt
      page: 6
      pdf_page: 118
    - "no": 5
      title: L’homomorphisme F et le décalage V
      page: 7
      pdf_page: 119
    - "no": 6
      title: Filtration et topologie de l’anneau W(A)
      page: 10
      pdf_page: 122
    - "no": 7
      title: Les anneaux $W_n(A)$ des vecteurs de Witt de longueur finie
      page: 12
      pdf_page: 124
    - "no": 8
      title: L’anneau des vecteurs de Witt à coefficients dans un anneau de caractéristique $p$
      page: 15
      pdf_page: 127
statements: 29
exercises: 58
content_sha256: 18354c626dd9c636314d443a2d42f81a66f14088339262d25bc4eedae5c9dfa6
---

## § 1. VECTEURS DE WITT

Dans tout ce paragraphe, $p$ désigne un nombre premier.

### 1. Polynômes de Witt

Pour tout entier $n \geqslant 0$, on appelle $n$-ième polynôme de Witt l’élément $\Phi_n$ de $\mathbf{Z}[X_0, ..., X_n]$ défini par

$$
\Phi_n(X_0, ..., X_n) = \sum_{i=0}^n p^i X_i^{p^{n-i}} = X_0^{p^n} + p X_1^{p^{n-1}} + \cdots + p^n X_n .
$$

On a évidemment $\Phi_0 = X_0$ et les relations de récurrence

$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = \Phi_n(X_0^p, ..., X_n^p) + p^{n+1} X_{n+1}
$$
$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = X_0^{p^{n+1}} + p \Phi_n(X_1, ..., X_{n+1}) .
$$

Lorsqu’on affecte $X_i$ du poids $p^i$, le polynôme $\Phi_n$ est isobare de poids $p^n$ (A, IV, p. 3).

#### Proposition 1 {#ac-ix-s1-prop-1 .statement}

Soient A un anneau filtré et $(\mathbf{J}_n)_{n \in \mathbf{Z}}$ sa filtration. On suppose que l’on a $\mathbf{J}_0 = \mathbf{A}$ et $p.1_A \in \mathbf{J}_1$. Soient m et n des entiers tels que $m \geqslant 1$ et $n \geqslant 0$, et $a_0, ..., a_n, b_0, ..., b_n$ des éléments de A.

a) Si l’on a $a_i \equiv b_i \mod \mathbf{J}_m$ pour $0 \leqslant i \leqslant n$, alors on a
$$
\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i} \quad \text{pour } 0 \leqslant i \leqslant n .
$$

b) Supposons que, pour tout entier $k \geqslant 1$, et tout $x \in \mathbf{A}$, la relation $p.x \in \mathbf{J}_{k+1}$ entraîne $x \in \mathbf{J}_k$. Si l’on a $\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i}$ pour $0 \leqslant i \leqslant n$, alors on a $a_i \equiv b_i \mod \mathbf{J}_m$ pour $0 \leqslant i \leqslant n$.

#### Lemme 1 {#ac-ix-s1-lem-1 .statement}

Si x et y sont deux éléments de A congrus modulo $\mathbf{J}_m$, on a
$$
x^{p^n} \equiv y^{p^n} \mod \mathbf{J}_{m+n} .
$$
Par récurrence sur n, on se ramène au cas où $n = 1$. Notons P le polynôme $\sum_{i=0}^{p-1} X^i Y^{p-1-i}$ de $\mathbf{Z}[X, Y]$. Vu l’hypothèse faite sur x et y, on a $P(x, y) \equiv P(x, x) \equiv p.x^{p-1} \mod \mathbf{J}_m$. Or on a $\mathbf{J}_m + p.\mathbf{A} \subset \mathbf{J}_1$, d’où $P(x, y) \in \mathbf{J}_1$. Finalement, $x^p - y^p = (x - y) P(x, y)$ appartient à $\mathbf{J}_m \mathbf{J}_1 \subset \mathbf{J}_{m+1}$.

Démontrons a) par récurrence sur n. Le cas $n = 0$ est immédiat. Supposons $n \geqslant 1$. Sous les hypothèses de a), on a
(4) $a_i^p \equiv b_i^p \mod \mathbf{J}_{m+1}$ pour $0 \leqslant i \leqslant n-1$ d’après le lemme 1 ,
(5) $\Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \equiv \Phi_{n-1}(b_0^p, ..., b_{n-1}^p) \mod \mathbf{J}_{m+n}$
d’après l’hypothèse de récurrence appliquée aux éléments $a_0^p, ..., a_{n-1}^p, b_0^p, ..., b_{n-1}^p$ de A, et
(6) $\Phi_n(a_0, ..., a_n) - p^n.a_n \equiv \Phi_n(b_0, ..., b_n) - p^n.b_n \mod \mathbf{J}_{m+n}$
d’après les formules (2) et (5). Comme $a_n - b_n$ appartient à $\mathbf{J}_m$, l’élément $p^n.a_n - p^n.b_n$ appartient à $\mathbf{J}_{m+n}$ et on déduit de (6) la congruence
$$
\Phi_n(a_0, ..., a_n) \equiv \Phi_n(b_0, ..., b_n) \mod \mathbf{J}_{m+n} ,
$$
d’où a).

Démontrons b) par récurrence sur n. Le cas $n = 0$ est immédiat. Supposons $n \geqslant 1$. Sous les hypothèses de b), on a $a_i \equiv b_i \mod \mathbf{J}_m$ pour $0 \leqslant i \leqslant n-1$ d’après l’hypothèse de récurrence, et on en déduit comme précédemment les congruences (4), (5) et (6). Mais par hypothèse $\Phi_n(a_0, ..., a_n)$ et $\Phi_n(b_0, ..., b_n)$ sont congrus mod. $\mathbf{J}_{m+n}$, et l’on a donc $p^n.(a_n - b_n) \in \mathbf{J}_{m+n}$. Comme la relation $p.x \in \mathbf{J}_{k+1}$ entraîne $x \in \mathbf{J}_k$ pour tout $x \in \mathbf{A}$ et tout $k \geqslant 1$, on a $a_n - b_n \in \mathbf{J}_m$, ce qui achève la démonstration.

### 2. Les applications $f, v$ et $\Phi$

Soit A un anneau. Munissons $\mathbf{A}^\mathbf{N}$ de la structure d’anneau produit. Notons $f_A$, ou simplement $f$, l’endomorphisme $(a_n)_{n \in \mathbf{N}} \mapsto (a_{n+1})_{n \in \mathbf{N}}$ de $\mathbf{A}^\mathbf{N}$. Notons $v_A$, ou simplement $v$, l’endomorphisme du groupe additif sous-jacent à $\mathbf{A}^{\mathbf{N}}$ qui à $(a_n)_{n \in \mathbf{N}}$ associe $(0, p \cdot a_0, p \cdot a_1, ...)$.

Pour tout entier $m \geqslant 0$, notons $\Phi_m$ l’application de $\mathbf{A}^{\mathbf{N}}$ dans $\mathbf{A}$ qui à $a = (a_n)_{n \in \mathbf{N}}$ associe $\Phi_m(a_0, ..., a_m)$. On note $\Phi_A$, ou simplement $\Phi$, l’application $a \mapsto (\Phi_n(a))_{n \in \mathbf{N}}$ de $\mathbf{A}^{\mathbf{N}}$ dans lui-même.

#### Lemme 2 {#ac-ix-s1-lem-2 .statement}

Soit $\mathbf{A}$ un anneau muni d’un endomorphisme $\sigma$ vérifiant $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ pour tout $a \in \mathbf{A}$. Soient $n \geqslant 1$ un entier et $a_0, ..., a_{n-1}$ des éléments de $\mathbf{A}$. Posons $u_i = \Phi_i(a_0, ..., a_i)$ pour $0 \leqslant i \leqslant n - 1$. Soit $u_n$ un élément de $\mathbf{A}$. Les conditions suivantes sont équivalentes :

a) Il existe $a_n \in \mathbf{A}$ tel que $u_n = \Phi_n(a_0, ..., a_n)$.

b) On a $\sigma(u_{n-1}) \equiv u_n \mod. p^n \cdot \mathbf{A}$.

Pour $0 \leqslant i \leqslant n - 1$, on a $\sigma(a_i) \equiv a_i^p \mod. p \cdot \mathbf{A}$. D’après la prop. 1 du no 1 appliquée au cas où $J_k = p^k \cdot \mathbf{A}$ (pour $k \in \mathbf{N}$) et où $m = 1$, on a la congruence

$$
\Phi_{n-1}(\sigma(a_0), ..., \sigma(a_{n-1})) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A},
$$

c’est-à-dire

$$
\sigma(u_{n-1}) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A}.
$$

Or, d’après la formule (2), la relation $u_n = \Phi_n(a_0, ..., a_n)$ équivaut à

$$
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n.
$$

Le lemme en résulte.

#### Proposition 2 {#ac-ix-s1-prop-2 .statement}

Soit $\mathbf{A}$ un anneau.

a) Si $p \cdot 1_A$ est non diviseur de 0 dans $\mathbf{A}$, l’application $\Phi_A$ est injective.

b) Si $p \cdot 1_A$ est inversible dans $\mathbf{A}$, l’application $\Phi_A$ est bijective.

c) Si $\sigma$ est un endomorphisme de l’anneau $\mathbf{A}$, vérifiant $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ pour tout $a \in \mathbf{A}$, l’image $\mathbf{A}'$ de $\Phi_A$ est un sous-anneau de $\mathbf{A}^{\mathbf{N}}$, stable par $f_A$ et $v_A$. C’est l’ensemble des éléments $(u_n)_{n \in \mathbf{N}}$ de $\mathbf{A}^{\mathbf{N}}$ tels que $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ pour tout $n \in \mathbf{N}$.

Si $a = (a_n)_{n \in \mathbf{N}}$ et $u = (u_n)_{n \in \mathbf{N}}$ sont des éléments de $\mathbf{A}^{\mathbf{N}}$, la relation $\Phi_A(a) = u$ est équivalente, d’après la formule (2), aux égalités

$$
\begin{cases}
u_0 = a_0, \\
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n & \text{pour tout } n \geqslant 1.
\end{cases}
$$

Soit $u = (u_n)_{n \in \mathbf{N}}$ dans $\mathbf{A}^{\mathbf{N}}$. Lorsque $p \cdot 1_A$ est non diviseur de 0 dans $\mathbf{A}$ (resp. lorsque $p \cdot 1_A$ est inversible dans $\mathbf{A}$), il existe au plus une suite $(a_n)_{n \in \mathbf{N}}$ dans $\mathbf{A}$ (resp. exactement une suite $(a_n)_{n \in \mathbf{N}}$ dans $\mathbf{A}$) satisfaisant aux égalités (10), d’où a) et b).

Démontrons c). D’après le lemme 2, l’image $\mathbf{A}'$ de $\mathbf{A}^{\mathbf{N}}$ par $\Phi_A$ est l’ensemble des $u = (u_n)_{n \in \mathbf{N}}$ dans $\mathbf{A}^{\mathbf{N}}$ tels que $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ pour tout $n \in \mathbf{N}$. Il en résulte aussitôt que $\mathbf{A}'$ est un sous-anneau de $\mathbf{A}^{\mathbf{N}}$, stable par $f_A$ et $v_A$.

#### Remarque {#ac-ix-s1-n2-rem-1 .statement}

Soient $a = (a_n)_{n \in \mathbf{N}}$ et $u = (u_n)_{n \in \mathbf{N}}$ des éléments de $A^\mathbf{N}$ tels que $u = \Phi_A(a)$, et $m$ un entier $\geqslant 0$. On déduit de (10) les assertions suivantes :

Si les $u_n$, pour $0 \leqslant n \leqslant m$, appartiennent à un sous-anneau $B$ de $A$ et si, pour tout $x \in A$, la relation $p.x \in B$ entraîne $x \in B$, alors les $a_n$, pour $0 \leqslant n \leqslant m$, appartiennent à $B$.

Si $A$ est muni d’une graduation de type $\mathbf{N}$, si $p.1_A$ est non diviseur de 0 dans $A$, si $d \in \mathbf{N}$ et si $u_n$ est homogène de degré $dp^n$ pour $0 \leqslant n \leqslant m$, alors $a_n$ est homogène de degré $dp^n$ pour $0 \leqslant n \leqslant m$.

### 3. Construction de polynômes

Soit $A$ l’anneau $\mathbf{Z}[X, Y]$ des polynômes à coefficients entiers en deux familles d’indéterminées $X = (X_n)_{n \in \mathbf{N}}$ et $Y = (Y_n)_{n \in \mathbf{N}}$. Soit $\theta$ l’endomorphisme de $A$ défini par $\theta(X_n) = X_n^p$ et $\theta(Y_n) = Y_n^p$ pour tout $n \in \mathbf{N}$. Alors $p$ n’est pas diviseur de 0 dans $A$ et l’ensemble des $a$ dans $A$ tels que $\theta(a) \equiv a^p \mod. p.A$ est un sous-anneau de $A$ contenant les $X_n$ et les $Y_n$, donc égal à $A$ tout entier.

D’après la prop. 2, a) et c) du no 2, il existe des éléments $S = (S_n)_{n \in \mathbf{N}}, P = (P_n)_{n \in \mathbf{N}}, I = (I_n)_{n \in \mathbf{N}}$ et $F = (F_n)_{n \in \mathbf{N}}$ de $A^\mathbf{N}$ caractérisés respectivement par les égalités

$$
\left\{
\begin{array}{l}
\Phi_A(S) = \Phi_A(X) + \Phi_A(Y) \\
\Phi_A(P) = \Phi_A(X) \Phi_A(Y) \\
\Phi_A(I) = - \Phi_A(X) \\
\Phi_A(F) = f_A(\Phi_A(X))
\end{array}
\right.
$$

Les éléments $S_n, P_n, I_n$ et $F_n$ de $A$ sont donc caractérisés par les formules suivantes (où $n$ parcourt $\mathbf{N}$) :

(12) $$ \Phi_n(S_0, ..., S_n) = \Phi_n(X_0, ..., X_n) + \Phi_n(Y_0, ..., Y_n), $$
(13) $$ \Phi_n(P_0, ..., P_n) = \Phi_n(X_0, ..., X_n) \Phi_n(Y_0, ..., Y_n), $$
(14) $$ \Phi_n(I_0, ..., I_n) = - \Phi_n(X_0, ..., X_n), $$
(15) $$ \Phi_n(F_0, ..., F_n) = \Phi_{n+1}(X_0, ..., X_{n+1}). $$

Affectons $X_n$ et $Y_n$ du poids $p^n$ pour tout $n \in \mathbf{N}$. On déduit de la remarque du no 2 les assertions suivantes :

a) On a $S_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ et $S_n$ est isobare de poids $p^n$.
b) On a $P_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ et $P_n$ est isobare de poids $p^n$ en chacune des familles $(X_0, ..., X_n)$ et $(Y_0, ..., Y_n)$.
c) On a $I_n \in \mathbf{Z}[X_0, ..., X_n]$ et $I_n$ est isobare de poids $p^n$.
d) On a $F_n \in \mathbf{Z}[X_0, ..., X_{n+1}]$ et $F_n$ est isobare de poids $p^{n+1}$.

La formule (2) permet dans la pratique de déterminer les polynômes $S_n, P_n, I_n$ et $F_n$ de proche en proche.

#### Exemple 1 {#ac-ix-s1-n3-exa-1 .statement}

On a

$$
S_0 = X_0 + Y_0
$$
$$
S_1 = X_1 + Y_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} X_0^i Y_0^{p-i}.
$$

De plus, $S_n - X_n - Y_n$ appartient à l’anneau $\mathbf{Z}[X_0, ..., X_{n-1}, Y_0, ..., Y_{n-1}]$.

#### Exemple 2 {#ac-ix-s1-n3-exa-2 .statement}

On a

$$
P_0 = X_0 Y_0
$$
$$
P_1 = p X_1 Y_1 + X_0^p Y_1 + X_1 Y_0^p.
$$

#### Exemple 3 {#ac-ix-s1-n3-exa-3 .statement}

Lorsque $p \neq 2$, on a $I_n = - X_n$. Pour $p = 2$, on a

$$
I_0 = - X_0
$$
$$
I_1 = - (X_0^2 + X_1)
$$
$$
I_2 = - X_0^4 - X_0^2 X_1 - X_1^2 - X_2.
$$

#### Exemple 4 {#ac-ix-s1-n3-exa-4 .statement}

On a

$$
F_0 = X_0^p + p X_1
$$
$$
F_1 = X_1^p + p X_2 - \sum_{i=0}^{p-1} \binom{p}{i} p^{p-i-1} X_0^{pi} X_1^{p-i}.
$$

Comme on a $\Phi_n(F_0, ..., F_n) \equiv \Phi_n(X_0^p, ..., X_n^p) \mod. p^{n+1}$. A pour tout $n \in \mathbf{N}$ (formules (2) et (15)), il résulte de la prop. 1, b) qu’on a $F_n \equiv X_n^p \mod. p$. A pour tout $n \in \mathbf{N}$.

#### Remarque {#ac-ix-s1-n3-rem-1 .statement}

Soit $J$ l’ensemble des entiers $j \geq 1$. Pour tout élément $j$ de $J$, définissons le polynôme $\varphi_j$ de $\mathbf{Z}[(X_j)_{j \in J}]$ par la formule

$$
\varphi_j = \sum_d d X_d^{j/d},
$$

où la somme porte sur les éléments de $J$ qui divisent $j$. Pour tout entier $n \geq 0$, on a

$$
\varphi_{p^n} = \Phi_n(X_{p^0}, ..., X_{p^n}).
$$

Pour tout anneau $A$ et tout élément $m$ de $J$, on note $\varphi_m$ l’application de $A^J$ dans $A$ qui à $(a_j)_{j \in J}$ associe $\varphi_m((a_j)_{j \in J})$; on note $\varphi_A$, ou simplement $\varphi$, l’application de $A^J$ dans lui-même qui à $a = (a_j)_{j \in J}$ associe $(\varphi_m(a))_{m \in J}$.

Soit $\mathcal{A} = \mathbf{Z}[(X_j)_{j \in J}, (Y_j)_{j \in J}]$ l’anneau des polynômes à coefficients entiers en les deux familles d’indéterminées $X = (X_j)_{j \in J}$ et $Y = (Y_j)_{j \in J}$. On peut montrer (p. 51, exerc. 34) qu’il existe dans $\mathcal{A}$ des éléments

$$
s = (s_j)_{j \in J}, \quad p = (p_j)_{j \in J} \quad \text{et} \quad i = (i_j)_{j \in J},
$$

caractérisés par les égalités suivantes :

$$
\varphi_{\mathcal{A}}(s) = \varphi_{\mathcal{A}}(\mathbf{X}) + \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(p) = \varphi_{\mathcal{A}}(\mathbf{X}) \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(i) = - \varphi_{\mathcal{A}}(\mathbf{X}) .
$$

### 4. L’anneau W(A) des vecteurs de Witt

Soit A un anneau. Si $a = (a_n)_{n \in \mathbf{N}}$ et $b = (b_n)_{n \in \mathbf{N}}$ sont des éléments de $A^\mathbf{N}$, nous noterons $S_A(a, b)$ (resp. $P_A(a, b)$, resp. $I_A(a)$) ou simplement $S(a, b)$ (resp. $P(a, b)$, resp. $I(a)$) la suite $(S_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$ (resp. $(P_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$, resp. $(I_n(a_0, ..., a_n))_{n \in \mathbf{N}}$). En substituant $a_n$ à $X_n$ et $b_n$ à $Y_n$, pour tout $n \in \mathbf{N}$, dans les formules (12), (13) et (14), on obtient les égalités

(16)
$$
\Phi_A(S_A(a, b)) = \Phi_A(a) + \Phi_A(b)
$$
(17)
$$
\Phi_A(P_A(a, b)) = \Phi_A(a) \Phi_A(b)
$$
(18)
$$
\Phi_A(I_A(a)) = - \Phi_A(a) .
$$

Nous noterons W(A) l’ensemble $A^\mathbf{N}$ muni des lois de composition $S_A$ et $P_A$.

Soit $\rho : B \to A$ un homomorphisme d’anneaux. Nous noterons $\rho^\mathbf{N}$ ou encore W($\rho$) l’application de $B^\mathbf{N}$ dans $A^\mathbf{N}$ qui à l’élément $b = (b_n)_{n \in \mathbf{N}}$ de $B^\mathbf{N}$ associe $(\rho(b_n))_{n \in \mathbf{N}}$. Il résulte aussitôt des définitions qu’on a

(19)
$$
W(\rho) \circ S_B = S_A \circ (W(\rho) \times W(\rho))
$$
(20)
$$
W(\rho) \circ P_B = P_A \circ (W(\rho) \times W(\rho))
$$
(21)
$$
W(\rho) \circ I_B = I_A \circ W(\rho)
$$
(22)
$$
\rho^\mathbf{N} \circ \Phi_B = \Phi_A \circ W(\rho) .
$$

#### Lemme 3 {#ac-ix-s1-lem-3 .statement}

Soit A un anneau. Il existe un homomorphisme surjectif d’anneaux $\rho : B \to A$, où B est un anneau satisfaisant aux conditions suivantes : p n’est pas diviseur de 0 dans B, et il existe un endomorphisme $\sigma$ de B tel que $\sigma(b) \equiv b^p \mod. p.B$ pour tout $b \in B$.

Il suffit en effet de poser $B = \mathbf{Z}[(X_a)_{a \in A}]$, de prendre pour $\sigma$ l’endomorphisme de B défini par $\sigma(X_a) = X_a^p$ pour tout $a \in A$, et pour $\rho$ l’homomorphisme de B dans A défini par $\rho(X_a) = a$ pour tout $a \in A$.

#### Théorème 1 {#ac-ix-s1-thm-1 .statement}

a) Soit A un anneau (commutatif). Muni de l’addition $S_A$ et de la multiplication $P_A$, W(A) est un anneau (commutatif). L’élément neutre pour l’addition est la suite $0_A$ dont tous les termes sont nuls ; l’élément neutre pour la multiplication est la suite $1_A$ dont tous les termes sont nuls sauf celui d’indice 0 qui vaut $1_A$. L’opposé d’un élément a de W(A) est $I_A(a)$.

b) Soit $\rho : B \to A$ un homomorphisme d’anneaux. Alors $W(\rho) : W(B) \to W(A)$ est un homomorphisme d’anneaux.

c) Soit $A$ un anneau. L’application $\Phi_A$ est un homomorphisme d’anneaux de $W(A)$ dans l’anneau produit $A^\mathbf{N}$. En particulier, pour tout $n \in \mathbf{N}$, l’application $\Phi_n : a \mapsto \Phi_n(a_0, ..., a_n)$ est un homomorphisme d’anneaux de $W(A)$ dans $A$.

Compte tenu des formules (16), (17), (19) et (20), il suffit de démontrer l’assertion $a$.

Soit $\rho : B \to A$ un homomorphisme d’anneaux satisfaisant aux conditions du lemme 3. Soit $B'$ le sous-anneau de $B^\mathbf{N}$ formé des éléments $(b_n)_{n \in \mathbf{N}}$ tels que $\sigma(b_n) \equiv b_{n+1} \mod. p^{n+1}$.B pour tout $n \in \mathbf{N}$. D’après la prop. 2 du no 2, $\Phi_B$ induit une bijection $\Phi'_B$ de $W(B)$ sur $B'$. Au vu des formules (16) à (18) et des relations $\Phi_n(0_B) = 0$ et $\Phi_n(1_B) = 1_B$ ($n \in \mathbf{N}$), on voit par transport de structure que $W(B)$ est un anneau, d’élément neutre $0_B$ pour l’addition, $1_B$ pour la multiplication, l’opposé de $b$ étant $I_B(b)$.

L’application $W(\rho) : W(B) \to W(A)$ est surjective. D’après les formules (19) et (20), la relation d’équivalence R sur $W(B)$ associée à l’application $W(\rho)$ est compatible avec la structure d’anneau de $W(B)$. Comme $W(\rho)$ induit une bijection $\Psi$ de l’anneau quotient $W(B)/R$ sur $W(A)$, compatible avec les lois d’addition et de multiplication, l’assertion $a$ se déduit de là par transport de structure.

#### Définition 1 {#ac-ix-s1-def-1 .statement}

Soit $A$ un anneau. L’anneau $W(A)$ est appelé l’anneau des vecteurs de Witt à coefficients dans $A$.

Pour $a$ dans $W(A)$ et $n$ dans $\mathbf{N}$, l’élément $\Phi_n(a) = \Phi_n(a_0, ..., a_n)$ est parfois appelé la composante fantôme d’indice $n$ de $a$.

#### Remarque {#ac-ix-s1-n4-rem-1 .statement}

Reprenons les notations de la remarque du no 3. Soit $A$ un anneau. Si $a$ et $b$ sont des éléments de $A^J$ et $r = (r_j)_{j \in J}$ un élément de $A^J$, on note $r_A(a, b)$ l’élément $(r_j(a, b))_{j \in J}$ de $A^J$. Notons $U(A)$ l’ensemble $A^J$ muni des lois de composition $s_A$ et $p_A$. On peut montrer (p. 52, exerc. 35) que, muni de l’addition $s_A$ et de la multiplication $p_A$, $U(A)$ est un anneau (commutatif); on l’appelle l’anneau de Witt universel de $A$. L’élément neutre pour l’addition est l’élément de $U(A)$ dont toutes les composantes sont nulles ; l’élément neutre pour la multiplication est l’élément de $U(A)$ dont toutes les composantes sont nulles sauf celle d’indice 1 qui vaut $1_A$; l’opposé d’un élément $a$ de $U(A)$ est $i_A(a)$. L’application $\varphi_A$ est un homomorphisme d’anneaux de $U(A)$ dans l’anneau produit $A^J$.

Soit $\rho : B \to A$ un homomorphisme d’anneaux ; on note $U(\rho)$ l’application de $B^J$ dans $A^J$ qui à l’élément $(b_j)_{j \in J}$ de $B^J$ associe l’élément $(\rho(b_j))_{j \in J}$ de $A^J$. On peut montrer (loc. cit.) que $U(\rho)$ est un homomorphisme d’anneaux de $U(B)$ dans $U(A)$.

### 5. L’homomorphisme F et le décalage V

Soit $A$ un anneau. Dans la suite de ce paragraphe, on note respectivement $+$ et $\times$ les lois d’addition et de multiplication dans $W(A)$. Nous écrirons aussi $0$ pour $0_A$ et $1$ pour $1_A$. On définit $^1$ deux applications $F_A$ et $V_A$ (notées aussi simplement $F$ et $V$) de $W(A)$ dans lui-même par les formules

$$
(23) \quad F_A(a) = (F_n(a_0, ..., a_{n+1}))_{n \in \mathbf{N}},
$$
$$
(24) \quad V_A(a) = (0, a_0, a_1, ...)
$$

(pour $a = (a_n)_{n \in \mathbf{N}}$ dans $W(A)$). L’application $V_A$ s’appelle le décalage.

La formule
$$
(25) \quad \Phi_n(F_0(a), ..., F_n(a)) = \Phi_{n+1}(a_0, ..., a_{n+1}) \quad (n \in \mathbf{N})
$$
résulte aussitôt de (15). On peut aussi l’écrire sous la forme
$$
(26) \quad \Phi_A \circ F_A = f_A \circ \Phi_A .
$$
La formule
$$
(27) \quad \Phi_A \circ V_A = v_A \circ \Phi_A
$$
résulte de la relation (3).

Soit $\rho : B \to A$ un homomorphisme d’anneaux. Les relations
$$
(28) \quad W(\rho) \circ F_B = F_A \circ W(\rho)
$$
$$
(29) \quad W(\rho) \circ V_B = V_A \circ W(\rho)
$$
résultent aussitôt des définitions.

#### Proposition 3 {#ac-ix-s1-prop-3 .statement}

*Soit A un anneau.*
  a) *L’application $F_A$ est un endomorphisme de l’anneau $W(A)$.*
  b) *L’application $V_A$ est un endomorphisme du groupe additif sous-jacent à l’anneau $W(A)$.*
  c) *Pour tout $a$ dans $W(A)$, on a $F_A(V_A(a)) = p.a$ (somme dans $W(A)$ de $p$ termes égaux à $a$).*
  d) *Quels que soient $a$ et $b$ dans $W(A)$, on a*
$$
(30) \quad V_A(a \times F_A(b)) = V_A(a) \times b
$$
$$
(31) \quad V_A(a) \times V_A(b) = p.V_A(a \times b)
$$
(somme dans $W(A)$ de $p$ termes égaux à $V_A(a \times b)$).
  e) *Posons $\mu = V_A(1) = (0, 1, 0, ...)$. Pour tout $b$ dans $W(A)$, on a*
$$
(32) \quad V_A(F_A(b)) = \mu \times b .
$$

$^1$ La lettre $F$ est l’initiale du nom de Frobenius, et la lettre $V$ celle du mot allemand *Verschiebung*.

f) Pour tout élément $a$ de $W(A)$ notons $a^{*p}$ le produit dans $W(A)$ de $p$ éléments égaux à $a$. Alors on a

$$
(33) \quad F_A(a) \equiv a^{*p} \mod. p.W(A) \quad (\text{idéal de } W(A) \text{ engendré par } p.\mathbf{1}) .
$$

Soit $\rho : B \to A$ un homomorphisme d’anneaux satisfaisant aux conditions du lemme 3 du n° 4. Alors $W(\rho) : W(B) \to W(A)$ est un homomorphisme surjectif d’anneaux, et $\Phi_B : W(B) \to B^N$ est un homomorphisme injectif d’anneaux. De plus, $f_B : B^N \to B^N$ est un homomorphisme d’anneaux. D’après les formules (26) et (28), on a

$$
\Phi_B \circ F_B = f_B \circ \Phi_B, \quad W(\rho) \circ F_B = F_A \circ W(\rho),
$$

d’où aussitôt l’assertion $a$. L’assertion $b$ résulte de manière analogue des formules (27) et (29) et du fait que $v_B$ est un endomorphisme du groupe additif sous-jacent à $B^N$.

Soit $a$ un élément de $W(A)$, et choisissons un élément $x$ de $W(B)$ que $W(\rho)$ applique sur $a$. Posons $\xi = \Phi_B(x)$. Il résulte aussitôt des définitions de $f_B$ et $v_B$ qu’on a $f_B(v_B(\xi)) = p.\xi$ (somme dans $B^N$ de $p$ termes égaux à $\xi$). D’après les formules (26) et (27) (où l’on remplace A par B), les éléments $F_B(V_B(x))$ et $p.x$ de $W(B)$ ont donc même image $p.\xi$ par l’application injective $\Phi_B$, et ainsi sont égaux. La formule $F_A(V_A(a)) = p.a$ résulte alors des relations (28) et (29). Ceci prouve $c$.

Raisonnant de manière analogue, on ramène la démonstration de la formule (30) à celle de la relation

$$
v_B(\xi f_B(\eta)) = v_B(\xi) \eta
$$

pour $\xi, \eta$ dans $B^N$. Or cela résulte des égalités

$$
\xi f_B(\eta) = (\xi_0 \eta_1, \xi_1 \eta_2, ...)
$$
$$
v_B(\xi) \eta = (0, p\xi_0 \eta_1, p\xi_1 \eta_2, ...)
$$

Compte tenu de $b$ et $c$, la formule (31) résulte de la formule (30), où l’on remplace $b$ par $V_A(b)$. La formule (32) est le cas particulier $a = 1$ de la formule (30).

De façon analogue, on ramène la démonstration de la formule (33) à celle de la relation

$$
f_B(\xi) \equiv \xi^p \mod. p.\Phi_B(B^N),
$$

où $\xi^p$ désigne le produit dans $B^N$ de $p$ éléments égaux à $\xi$. Par la prop. 2, c) du n° 2, ceci équivaut au fait que pour tout $n \geqslant 0$, on ait

$$
\sigma(\xi_{n+1} - \xi_n^p) \equiv \xi_{n+2} - \xi_{n+1}^p \mod. p^{n+2}B .
$$

Or, pour tout $n \geqslant 0$, on a, par loc. cit.,

$$
\sigma(\xi_n) \equiv \xi_{n+1} \mod. p^{n+1}B
$$

puisque $\xi = \Phi_B(x)$; on en déduit, grâce au lemme 1 du n° 1,

$$
\sigma(\xi_n)^p \equiv \xi_{n+1}^p \mod. p^{n+2}\mathbf{B}.
$$

Ceci prouve la relation voulue.

#### Remarque {#ac-ix-s1-n5-rem-1 .statement}

Pour la définition d’applications analogues aux applications F et V, dans le cas de l’anneau de Witt universel, voir les exerc. 36, 37 et 38, p. 52 et suivantes.

### 6. Filtration et topologie de l’anneau W(A)

#### Lemme 4 {#ac-ix-s1-lem-4 .statement}

Soient A un anneau et m $\geqslant 1$ un entier. On a

(34)
$$
a = (a_0, ..., a_{m-1}, 0, ...) + (\underbrace{0, ..., 0}_{m \text{ termes}}, a_m, a_{m+1}, ...)
$$
pour tout $a$ dans W(A).

Soit $\rho : B \to A$ un homomorphisme d’anneaux satisfaisant aux conditions du lemme 3 du n° 4. Alors $W(\rho) : W(B) \to W(A)$ est un homomorphisme surjectif d’anneaux, et $\Phi_B : W(B) \to B^N$ est un homomorphisme injectif. Il suffit donc de prouver que l’on a

(35)
$$
\Phi_n(b) = \Phi_n(b_0, ..., b_{m-1}, 0, ...) + \Phi_n(0, ..., 0, b_m, b_{m+1}, ...)
$$
quels que soient $b$ dans W(B) et les entiers $m \geqslant 1, n \geqslant 0$. Or on a

$$
\Phi_n(b_0, ..., b_{m-1}, ...) = \Phi_n(b_0, ..., b_n) \quad \text{si} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=0}^{m-1} p^i \cdot b_i^{p^{n-i}} \quad \text{si} \quad m \leqslant n
$$
$$
\Phi_n(0, ..., 0, b_m, b_{m+1}, ...) = 0 \quad \text{si} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=m}^n p^i \cdot b_i^{p^{n-i}} \quad \text{si} \quad m \leqslant n,
$$
d’où la formule (35).

Soit A un anneau. Pour tout entier $m \geqslant 0$, on note $V_m(A)$ l’ensemble des vecteurs de Witt $a = (a_n)_{n \in \mathbf{N}}$ tels que $a_n = 0$ pour $0 \leqslant n < m$. C’est l’image de la puissance m-ième $V^m$ de l’application $V_A$. Les formules

(36)
$$
V^m(a + b) = V^m(a) + V^m(b)
$$
(37)
$$
V^m(a) \times b = V^m(a \times F^m(b))
$$
résultent de la prop. 3 du n° 5 par récurrence sur $m$. Elles entraînent que $V_m(A)$ est un idéal de W(A).

Dans la suite, on munira $W(A)$ de la topologie $\mathcal{T}$ associée à la filtration $(V_m(A))_{m \in \mathbf{Z}}$. Comme $V_m(A)$ est un idéal de $W(A)$ pour tout $m \in \mathbf{Z}$, la topologie $\mathcal{T}$ est compatible avec la structure d’anneau de $W(A)$ (TG, III, p. 49, exemple 3). Soit $a \in W(A)$; les ensembles $a + V_m(A)$, où $m$ parcourt $\mathbf{N}$, forment un système fondamental de voisinages de $a$ pour $\mathcal{T}$. Or, il résulte du lemme 4 que $a + V_m(A)$ se compose des vecteurs de Witt $b$ tels que $a_i = b_i$ pour $0 \leq i < m$. Par suite, $\mathcal{T}$ n’est autre que la topologie produit sur $A^\mathbf{N}$ de la topologie discrète sur chacun des facteurs, et $W(A)$ est donc un anneau topologique séparé et complet (TG, II, p. 17, prop. 10 et TG, III, p. 22, prop. 4).

Notons $\tau_A$ (ou simplement $\tau$) l’application de $A$ dans $W(A)$ qui à un élément $a$ de $A$ associe $(a, 0, 0, ...)$. On a $\Phi_n(\tau(a)) = a^{p^n}$ pour tout $n \in \mathbf{N}$. Pour tout homomorphisme d’anneaux $\rho : B \to A$, on a $W(\rho) \circ \tau_B = \tau_A \circ \rho$.

#### Proposition 4 {#ac-ix-s1-prop-4 .statement}

*Soient $a$ et $b$ dans $A$ et $x = (x_n)_{n \in \mathbf{N}}$ un élément de $W(A)$.*

a) *On a les formules*

$$
\tau(ab) = \tau(a) \times \tau(b)
$$
$$
\tau(a) \times x = (a^{p^n} x_n)_{n \in \mathbf{N}}.
$$

b) *La série de terme général $V^n(\tau(x_n))$ est convergente dans $W(A)$, de somme $x$.*
Soit $n$ un entier positif. Le polynôme $P_n(X_0, ..., X_n; Y_0, ..., Y_n)$ introduit au no 3 est isobare de poids $p^n$ en la famille $(X_0, ..., X_n)$ lorsqu’on affecte $X_i$ du poids $p^i$. On a donc
$$
P_n(X_0, 0, ..., 0; Y_0, ..., Y_n) = X_0^{p^n} P_n(1, 0, ..., 0; Y_0, ..., Y_n).
$$
Comme $1 = (1, 0, 0, ...)$ est élément unité de l’anneau des vecteurs de Witt à coefficients dans $\mathbf{Z}[(X_n)_{n \in \mathbf{N}}, (Y_n)_{n \in \mathbf{N}}]$, on a
$$
P_n(1, 0, ..., 0; Y_0, ..., Y_n) = Y_n.
$$
Par substitution de $a$ à $X_0$ et de $x_i$ à $Y_i$, on déduit de (40) et (41) la relation :
$$
P_n(a, 0, ..., 0; x_0, ..., x_n) = a^{p^n} x_n.
$$
D’après la définition de la multiplication dans $W(A)$, on a prouvé (39) ; la formule (38) est un cas particulier de (39).

*Démontrons b).* Par définition, $V^n(\tau(x_n))$ est la suite dont toutes les composantes sont nulles, sauf celle d’indice $n$ qui est égale à $x_n$. Il résulte du lemme 4, par récurrence sur $m$, qu’on a
$$
\sum_{n=0}^m V^n(\tau(x_n)) = (x_0, ..., x_m, 0, 0, ...)
$$

pour tout entier $m \geq 0$; on en déduit b) par passage à la limite puisque la topologie $\mathcal{T}$ sur $W(A)$ est produit des topologies discrètes des facteurs $A$.

### 7. Les anneaux $W_n(A)$ des vecteurs de Witt de longueur finie

#### Définition 2 {#ac-ix-s1-def-2 .statement}

Soient $A$ un anneau et $n \geq 1$ un entier. On note $W_n(A)$ l’anneau quotient $W(A)/V_n(A)$.

Étant donnés des éléments $a_0, ..., a_{n-1}$ de $A$, on note $[a_0, ..., a_{n-1}]$ ou $[a_i]_{0 \leq i < n}$ la classe modulo $V_n(A)$ de l’élément $(a_0, ..., a_{n-1}, 0, 0, ...)$ de $W(A)$. D’après le lemme 4 du n° 6, l’application $(a_0, ..., a_{n-1}) \mapsto [a_0, ..., a_{n-1}]$ de $A^n$ dans $W_n(A)$ est une bijection. Pour cette raison, on dit que les éléments de $W_n(A)$ sont les vecteurs de Witt de longueur $n$; par analogie, on qualifie parfois de vecteurs de Witt de longueur infinie les éléments de $W(A)$.

On note $\pi_n$ l’homomorphisme canonique de $W(A)$ dans $W_n(A)$. D’après le lemme 4 du n° 6, on a
$$
\pi_n(a) = [a_0, ..., a_{n-1}]
$$
pour tout $a = (a_n)_{n \in \mathbf{N}}$ dans $W(A)$.

D’après la définition des opérations dans $W(A)$, on a la description suivante des opérations dans $W_n(A)$ :
$$
[a_0, ..., a_{n-1}] + [b_0, ..., b_{n-1}] = [S_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
[a_0, ..., a_{n-1}] \times [b_0, ..., b_{n-1}] = [P_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
- [a_0, ..., a_{n-1}] = [I_i(a_0, ..., a_i)]_{0 \leq i < n}.
$$

De plus, l’élément neutre de l’addition dans $W_n(A)$ est $[0, ..., 0]$ et celui de la multiplication est $[1, 0, ..., 0]$.

Soit $i$ un entier tel que $0 \leq i \leq n$. Par passage au quotient, l’homomorphisme $\Phi_i$ de $W(A)$ dans $A$ définit un homomorphisme $\Phi_i$ de $W_n(A)$ dans $A$. Celui-ci associe au vecteur de Witt $[a_0, ..., a_{n-1}]$ l’élément $\Phi_i(a_0, ..., a_i)$ de $A$ (appelé aussi composante fantôme d’indice $i$ de $[a_0, ..., a_{n-1}]$).

Soit $\rho : B \to A$ un homomorphisme d’anneaux. Par passage aux quotients, l’homomorphisme $W(\rho)$ de $W(B)$ dans $W(A)$ définit un homomorphisme $W_n(\rho)$ de $W_n(B)$ dans $W_n(A)$. Il se décrit par la formule
$$
W_n(\rho)[b_0, ..., b_{n-1}] = [\rho(b_0), ..., \rho(b_{n-1})]
$$
pour tout $[b_0, ..., b_{n-1}]$ dans $W_n(B)$.

Soient $m$ et $n$ deux entiers tels que $1 \leq n \leq m$. On a $V_n(A) \supset V_m(A)$, d’où un homomorphisme canonique de $W_m(A) = W(A)/V_m(A)$ sur $W_n(A) = W(A)/V_n(A)$; on notera $\pi_{n,m}$ cet homomorphisme. On a explicitement
$$
\pi_{n,m}[a_0, ..., a_{m-1}] = [a_0, ..., a_{n-1}]
$$

pour $[a_0, ..., a_{m-1}]$ dans $W_m(A)$. La famille $(W_n(A), \pi_{n,m})$ est un système projectif d’anneaux et l’application $\pi : a \mapsto (\pi_n(a))_{n \geq 1}$ est un homomorphisme d’anneaux de $W(A)$ dans $\lim_{\leftarrow} W_n(A)$, dit canonique. Comme $W(A)$ est séparé et complet pour la filtration $(V_n(A))_{n \in \mathbf{Z}}$ (*cf.* n° 6), l’homomorphisme canonique $\pi$ est un isomorphisme d’anneaux topologiques, lorsque l’on munit $W_n(A)$ de la topologie discrète pour tout entier $n \geq 1$ (III, § 2, n° 6).

Désormais, les homomorphismes $\pi_n$ et $\pi_{n,m}$ seront qualifiés d’*homomorphismes de projection* de $W(A)$ dans $W_n(A)$, et de $W_m(A)$ dans $W_n(A)$ respectivement.

#### Exemple 1 {#ac-ix-s1-n7-exa-1 .statement}

L’homomorphisme $\Phi_0 : W_1(A) \to A$ est un isomorphisme.

#### Exemple 2 {#ac-ix-s1-n7-exa-2 .statement}

Explicitons les opérations dans $W_2(A)$. On a

$$
[a_0, a_1] + [b_0, b_1] = \left[ a_0 + b_0, a_1 + b_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} a_0^i b_0^{p-i} \right]
$$

$$
[a_0, a_1] \times [b_0, b_1] = [a_0 b_0, a_0^p b_1 + a_1 b_0^p + p \cdot a_1 b_1]
$$

pour $[a_0, a_1]$ et $[b_0, b_1]$ dans $W_2(A)$. Les composantes fantômes de $[a_0, a_1]$ sont $a_0$ et $a_0^p + p \cdot a_1$.

#### Exemple 3 {#ac-ix-s1-n7-exa-3 .statement}

Soit $n \geq 1$ un entier. Si $a_0, ..., a_{n-1}, b_0, ..., b_{n-1}$ sont des entiers tels que $a_i \equiv b_i \bmod p$ pour $0 \leq i < n$, on a (n° 1, prop. 1)

$$
\Phi_{n-1}(a_0, ..., a_{n-1}) \equiv \Phi_{n-1}(b_0, ..., b_{n-1}) \bmod p^n.
$$

Par suite, $\Phi_{n-1}$ définit par passage aux quotients un homomorphisme d’anneaux $\varphi_n : W_n(\mathbf{Z}/p\mathbf{Z}) \to \mathbf{Z}/p^n\mathbf{Z}$. L’image de $\varphi_n$ est un sous-groupe de $\mathbf{Z}/p^n\mathbf{Z}$ contenant 1, donc $\varphi_n$ est surjectif. Comme les ensembles finis $W_n(\mathbf{Z}/p\mathbf{Z})$ et $\mathbf{Z}/p^n\mathbf{Z}$ ont même cardinal $p^n$, $\varphi_n$ est un isomorphisme.

Soient $m$ et $n$ des entiers tels que $1 \leq n \leq m$. Il existe un seul homomorphisme d’anneaux $\alpha_{n,m} : \mathbf{Z}/p^m\mathbf{Z} \to \mathbf{Z}/p^n\mathbf{Z}$; par suite le diagramme

$$
\begin{array}{ccc}
\mathbf{Z}/p^m\mathbf{Z} & \xrightarrow{\alpha_{n,m}} & \mathbf{Z}/p^n\mathbf{Z} \\
\varphi_m \uparrow & & \varphi_n \uparrow \\
W_m(\mathbf{Z}/p\mathbf{Z}) & \xrightarrow{\pi_{n,m}} & W_n(\mathbf{Z}/p\mathbf{Z})
\end{array}
$$

est commutatif. Il en résulte que $\varphi = \lim \varphi_n$ est un isomorphisme d’anneaux topologiques de $W(\mathbf{Z}/p\mathbf{Z}) = \lim_{\leftarrow} W_n(\mathbf{Z}/p\mathbf{Z})$ sur $\mathbf{Z}_p = \lim_{\leftarrow} \mathbf{Z}/p^n\mathbf{Z}$ (III, § 2, n° 12, exemple 3).

Soient $m$ et $n$ deux entiers $\geq 1$. Par construction, on a une suite exacte de groupes additifs

(E)
$$
0 \longrightarrow W(A) \xrightarrow{\nu^m} W(A) \xrightarrow{\pi_m} W_m(A) \longrightarrow 0.
$$

Par passage aux quotients, l’endomorphisme $V^n$ du groupe additif de $W(A)$ définit un homomorphisme $V^n_m$ du groupe additif de $W_m(A)$ dans celui de $W_{m+n}(A)$. Autrement dit, on a un diagramme commutatif

$$
\begin{array}{ccc}
W(A) & \xrightarrow{V^n} & W(A) \\
\pi_m \downarrow & & \pi_{n+m} \downarrow \\
W_m(A) & \xrightarrow{V^n_m} & W_{n+m}(A)
\end{array}
$$

Par passage aux quotients, on déduit de la suite exacte (E) une suite exacte

(E') $$ 0 \longrightarrow W_m(A) \xrightarrow{V^n_m} W_{n+m}(A) \xrightarrow{\pi_{n,n+m}} W_n(A) \longrightarrow 0 . $$

On a

(45) $$ V^n_m[a_0, ..., a_{m-1}] = [\underbrace{0, ..., 0}_{n \text{ fois}}, a_0, ..., a_{m-1}], $$

pour tout élément $[a_0, ..., a_{m-1}]$ de $W_m(A)$.

D’après la prop. 3, c) du n° 5, on a $FV^{m+1}(a) = p.V^m(a)$ pour tout $a$ dans $W(A)$ et on a par suite $F(V_{m+1}(A)) \subset V_m(A)$. Par récurrence sur $n$, on en déduit que $F^n$ applique $V_{n+m}(A)$ dans $V_m(A)$, et définit donc, par passage aux quotients, un homomorphisme d’anneaux $F^n_m : W_{n+m}(A) \to W_m(A)$. Par construction, on a un diagramme commutatif

$$
\begin{array}{ccc}
W(A) & \xrightarrow{F^n} & W(A) \\
\pi_{n+m} \downarrow & & \pi_m \downarrow \\
W_{n+m}(A) & \xrightarrow{F^n_m} & W_m(A)
\end{array}
$$

Rappelons (n° 3) que le polynôme $F_i$ appartient à $\mathbf{Z}[X_0, ..., X_{i+1}]$ pour tout entier $i \geqslant 0$; l’homomorphisme $F^1_m$ de $W_{m+1}(A)$ dans $W_m(A)$ s’explicite donc comme suit :

(46) $$ F^1_m[a_0, ..., a_m] = [F_i(a_0, ..., a_{i+1})]_{0 \leqslant i < m}. $$

Soient $a \in W_m(A)$, $a' \in W_m(A)$ et $b \in W_{m+1}(A)$. Les formules suivantes résultent par passages aux quotients de la prop. 3 du n° 5 :

(47) $$ F^1_m(V^1_m(a)) = p.a $$
(48) $$ V^1_m(a \times F^1_m(b)) = V^1_m(a) \times b $$
(49) $$ V^1_m(a) \times V^1_m(a') = p.V^1_m(a \times a') $$
(50) $$ V^1_m(F^1_m(b)) = \mu_{m+1} \times b $$

(avec $\mu_{m+1} = [0, 1, 0, ..., 0]$).

### 8. L’anneau des vecteurs de Witt à coefficients dans un anneau de caractéristique $p$

#### Proposition 5 {#ac-ix-s1-prop-5 .statement}

Soit $A$ un anneau de caractéristique $p$ (A, V, p. 2). Quels que soient les éléments $a$ et $b$ de $W(A)$, et les entiers positifs $m, n$, on $a$, si $a = (a_n)_{n \in \mathbf{N}}$,

$$
(51) \quad F(a) = (a_n^p)_{n \in \mathbf{N}}
$$
$$
(52) \quad p.a = VF(a) = FV(a) = (0, a_0^p, a_1^p, ...)
$$
$$
(53) \quad V^m(a) \times V^n(b) = V^{m+n}(F^n(a) \times F^m(b)) .
$$

La formule (51) résulte de l’exemple 4 du n° 3. On déduit aussitôt de là l’égalité

$$
VF(a) = FV(a) = (0, a_0^p, a_1^p, ...) ,
$$

et l’égalité $p.a = FV(a)$ a été prouvée (n° 5, prop. 3), d’où (52).

Prouvons (53). D’après la formule (37) (où l’on substitue $V^n(b)$ à $b$), on a

$$
(54) \quad V^m(a) \times V^n(b) = V^m(a \times F^m(V^n(b))) .
$$

De la formule (37), on déduit aussi

$$
(55) \quad V^n(F^m(b)) \times a = V^n(F^m(b) \times F^n(a)) .
$$

La formule (53) résulte alors de (54) et (55) et de la relation $F^m \circ V^n = V^n \circ F^m$, elle-même conséquence de (51).

#### Corollaire {#ac-ix-s1-n8-cor-1 .statement}

Si $m$ et $n$ sont deux entiers positifs, on a

$$
V_m(A) \times V_n(A) \subset V_{m+n}(A) .
$$

Cela résulte de la formule (53), car $V_m(A)$ est l’image de $V^m : W(A) \to W(A)$.

#### Proposition 6 {#ac-ix-s1-prop-6 .statement}

Soit $A$ un anneau.

a) Pour tout entier $k \geqslant 1$, on a $(V_1(A))^k = p^{k-1} \cdot V_1(A)$.

b) Supposons que $A$ soit un anneau de caractéristique $p$. Sur l’anneau $W(A)$, la topologie $V_1(A)$-adique et la topologie $p$-adique coïncident, et elles sont plus fines que la topologie produit $\mathcal{C}$ (cf. n° 6). L’anneau $W(A)$ est séparé et complet pour la topologie $p$-adique.

Prouvons a) par récurrence sur $k$. Le cas $k = 1$ est évident. Supposons $k \geqslant 2$. D’après l’hypothèse de récurrence, on a $V_1(A)^{k-1} = p^{k-2} \cdot V_1(A)$ et par suite $V_1(A)^k = p^{k-2} \cdot (V_1(A))^2$. Mais il résulte de la prop. 3, d), formule (31), du n° 5 qu’on a $(V_1(A))^2 = p \cdot V_1(A)$, d’où a).

Supposons maintenant que $A$ soit de caractéristique $p$. Comme on a

$$
p \cdot W(A) = VF(W(A)) \subset V_1(A) \quad (\text{formule (52)}) ,
$$

on déduit de a) les inclusions $p^k.W(A) \subset (V_1(A))^k \subset p^{k-1}.W(A)$, et du corollaire à la prop. 5 l’inclusion $(V_1(A))^k \subset V_k(A)$, pour tout entier $k \geqslant 1$. La première assertion de b) en résulte.

Soit $k$ un entier $\geqslant 1$. D’après la formule (52), l’idéal $p^k.W(A)$ de $W(A)$ est l’ensemble des éléments $a = (a_n)_{n \in \mathbf{N}}$ de $W(A)$ tels qu’on ait $a_n = 0$ pour $n < k$ et $a_n \in A^{p^k}$ pour $n \geqslant k$. Il est donc fermé pour la topologie $\mathcal{G}$. Comme $W(A)$ est séparé et complet pour la topologie $\mathcal{G}$ (no 6) et que les idéaux $p^k.W(A)$ de $W(A)$, pour $k \geqslant 1$, forment une base de voisinages de $0$ dans $W(A)$ pour la topologie $p$-adique, l’anneau $W(A)$ est séparé et complet pour la topologie $p$-adique (TG, III, p. 26, cor. 1 à la prop. 10).

#### Proposition 7 {#ac-ix-s1-prop-7 .statement}

*Soit A un anneau parfait de caractéristique p.*

a) *Pour tout élément $a = (a_n)_{n \in \mathbf{N}}$ de $W(A)$, la série de terme général $p^n \tau(a_n^{p^{-n}})$ est convergente dans $W(A)$, de somme $a$.*

b) *Sur $W(A)$, la topologie $V_1(A)$-adique, la topologie $p$-adique et la topologie $\mathcal{G}$ coïncident. Plus précisément, on a $V_n(A) = p^n.W(A) = (V_1(A))^n$ pour tout entier $n \geqslant 0$. En particulier $\Phi_0$ définit un isomorphisme de $W(A)/p.W(A)$ sur $A$.*

Par définition (A, V, p. 5), l’application $a \mapsto a^p$ est un automorphisme de l’anneau $A$. D’après la prop. 5, F est donc un automorphisme de l’anneau $W(A)$, et l’on a, pour tout $n \in \mathbf{N}$,

$$
p^n.W(A) = V^n F^n(W(A)) = V^n(W(A)) = V_n(A).
$$

En particulier, on a $(V_1(A))^n = (p.W(A))^n = p^n.W(A)$. L’assertion b) résulte de là.

D’après la prop. 5, on a

$$
p^n.\tau(a_n^{p^{-n}}) = V^n F^n \tau(a_n^{p^{-n}}) = V^n \tau(a_n),
$$

et l’assertion a) résulte de la prop. 4 du no 6.

#### Proposition 8 {#ac-ix-s1-prop-8 .statement}

*Soit A un corps de caractéristique p. L’anneau $W(A)$ est un anneau local intègre séparé et complet, d’idéal maximal $V_1(A)$ et de corps résiduel isomorphe à A. Si le corps A est parfait, l’anneau $W(A)$ est un anneau de valuation discrète, et son idéal maximal est $p.W(A)$.*

L’homomorphisme $\Phi_0$ définit un isomorphisme de $W(A)/V_1(A)$ sur $A$ (no 7, exemple 1). L’idéal $V_1(A)$ de $W(A)$ est donc maximal. Comme l’anneau $W(A)$ est séparé et complet pour la topologie $V_1(A)$-adique (prop. 6, $b$), c’est un anneau local, d’idéal maximal $V_1(A)$ (III, § 2, no 13, prop. 19).

Soient $a$ et $b$ deux éléments non nuls de $W(A)$. Il existe des entiers $m \geqslant 0$ et $n \geqslant 0$, et des éléments $a' = (a'_n)_{n \in \mathbf{N}}$ et $b' = (b'_n)_{n \in \mathbf{N}}$ de $W(A)$ tels que $a = V^m(a')$, $b = V^n(b')$ et que les éléments $a'_0$ et $b'_0$ de $A$ soient non nuls. Alors la composante d’indice $m + n$ de $a \times b$ est égale à la composante d’indice 0 de $F^n(a') \times F^m(b')$ (formule (53)), c’est-à-dire à ${a'_0}^{p^n} {b'_0}^{p^m}$ (formule (51) et no 3, exemple 2). Par suite $a \times b$ est non nul et $W(A)$ est intègre.

Si le corps $A$ est parfait, l’idéal maximal $V_1(A)$ de $W(A)$ est égal à $p.W(A)$ (prop. 7, b)) et par suite W(A) est un anneau de valuation discrète (VI, § 3, n° 6, prop. 9, c)).

#### Remarque 1 {#ac-ix-s1-n8-rem-1 .statement}

Soit A un corps de caractéristique p. On peut montrer que l’anneau W(A) est noethérien si et seulement si A est parfait (p. 43, exerc. 9).

#### Remarque 2 {#ac-ix-s1-n8-rem-2 .statement}

Soit A un anneau de caractéristique p. D’après la prop. 5, on a les formules

$$
F_m^n[a_0, ..., a_{n+m-1}] = [a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$
$$
p^n.[a_0, ..., a_{n+m-1}] = [\underbrace{0, ..., 0}_{n \text{ fois}}, a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$

pour tout vecteur de Witt $[a_0, ..., a_{n+m-1}]$ de longueur $n + m$.

En fait, l’application $F : W(A) \to W(A)$ permet, par passage aux quotients par $V_m(A)$, de définir une application $\overline{F}_m : W_m(A) \to W_m(A)$. On a la formule

$$
\overline{F}_m[a_0, ..., a_{m-1}] = [a_0^p, ..., a_{m-1}^p].
$$

Les applications $V_m^1 \circ \overline{F}_m$ et $\overline{F}_{m+1} \circ V_m^1$ de $W_m(A)$ dans $W_{m+1}(A)$ sont égales et sont déduites, par passage au quotient, de la multiplication par $p$ dans $W_{m+1}(A)$.

## EXERCICES {#ac-ix-s1-exercises}

Dans les exercices 1 à 27, $p$ est un nombre premier fixé. Si $A$ est un anneau, l’anneau des vecteurs de Witt $W(A)$ est celui attaché au nombre premier $p$.

See the [exercises for § 1](exercises/s1/).
