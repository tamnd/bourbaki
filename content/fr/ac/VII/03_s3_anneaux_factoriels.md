---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: Diviseurs
section: 3
section_title: Anneaux factoriels
lang: fr
source: ac-v-vii-fr
pdf_pages: 0226-0237, 0291-0298
extraction: ocr
subsections:
    - "no": 1
      title: Définition des anneaux factoriels
      page: 0
      pdf_page: 226
    - "no": 2
      title: Caractérisations des anneaux factoriels
      page: 0
      pdf_page: 226
    - "no": 3
      title: Décomposition en éléments extrémaux
      page: 0
      pdf_page: 228
    - "no": 4
      title: Anneaux de fractions d’un anneau factoriel
      page: 0
      pdf_page: 229
    - "no": 5
      title: Anneaux de polynômes sur un anneau factoriel
      page: 0
      pdf_page: 229
    - "no": 6
      title: Anneaux factoriels et anneaux de Zariski
      page: 0
      pdf_page: 231
    - "no": 7
      title: Préliminaires sur les automorphismes des anneaux de séries formelles
      page: 0
      pdf_page: 231
    - "no": 8
      title: Le théorème de préparation
      page: 0
      pdf_page: 232
    - "no": 9
      title: '*Factorialité des anneaux de séries formelles*'
      page: 0
      pdf_page: 236
statements: 23
exercises: 27
content_sha256: c86210c1d1ba178a2e2323abf3be27dbcd1653b5a9ae5496bb9e9db4c5ef234b
---

## § 3. Anneaux factoriels

### 1. Définition des anneaux factoriels

#### Définition 1 {#ac-vii-s3-def-1 .statement}

On appelle anneau factoriel un anneau de Krull dont tous les idéaux divisoriels sont principaux.

En d’autres termes, le groupe des classes de diviseurs ($§ 1$, n° 2) est réduit à 0.

#### Exemple 1 {#ac-vii-s3-n1-exa-1 .statement}

Tout anneau principal est factoriel (et, rappelons-le, est un anneau de Dedekind). Réciproquement tout anneau de Dedekind factoriel est principal en vertu du § 2, n° 2, th. 1, c).

#### Exemple 2 {#ac-vii-s3-n1-exa-2 .statement}

En particulier, si $K$ est un corps, les anneaux $K[X]$ et $K[[X]]$ sont factoriels (voir th. 2 et prop. 8 ci-dessous pour des généralisations).

#### Exemple 3 {#ac-vii-s3-n1-exa-3 .statement}

\* L’anneau local d’un point simple d’une variété algébrique est factoriel. L’anneau des germes de fonctions analytiques à l’origine de $\mathbf{C}^n$ est factoriel. \*

### 2. Caractérisations des anneaux factoriels

Etant donné un anneau $A$, nous aurons à considérer la condition suivante:

(M) Toute famille non vide d’idéaux principaux entiers de $A$ possède un élément maximal.

#### Théorème 1 {#ac-vii-s3-thm-1 .statement}

Soit $A$ un anneau intègre. Les conditions suivantes sont équivalentes:
a) $A$ est factoriel;

b) le groupe ordonné des idéaux principaux fractionnaires non nuls de $A$ est somme directe de groupes isomorphes à $\mathbf{Z}$ (ordonnée par l’ordre produit);
c) la condition (M) est satisfaite, et l’intersection de deux idéaux principaux de $A$ est un idéal principal;
d) la condition (M) est satisfaite, et, pour tout élément extrémal $p$ de $A$, l’idéal $Ap$ est premier;
e) $A$ est un anneau de Krull, et tout idéal premier de hauteur 1 est principal.

Nous noterons $K$ le corps des fractions de $A$, et $\mathcal{P}^*$ (ou $\mathcal{P}^*(A)$) le groupe ordonné des idéaux principaux fractionnaires non nuls de $A$. Nous ferons la démonstration suivant le schéma logique:

$$
\begin{array}{ccc}
a & \rightarrow & d \\
| & & | \\
e & \leftrightarrow & b \\
| & & | \\
& \rightarrow & c
\end{array}
$$

Montrons que a) implique b): en effet, si $A$ est factoriel, $\mathcal{P}^*$ est isomorphe au groupe des diviseurs de $A$, donc à une somme directe de groupes $\mathbf{Z}$ ($§ 1$, no 3, th. 2).

Notons maintenant que la relation « l’intersection de deux idéaux principaux entiers de $A$ est un idéal principal » veut dire que tout couple d’éléments de $A$ admet un p.p.c.m., c’est-à-dire que $\mathcal{P}^*$ est un groupe réticulé (*Alg.*, chap. VI, $§ 1$, no 9, prop. 8). Le fait que b) implique c) (et lui est même équivalent) résulte donc d’*Alg.*, chap. VI, $§ 1$, no 13, th. 2. Le fait que c) implique d) résulte d’*Alg.*, chap. VI, $§ 1$, no 13, prop. 14, (DIV).

Le fait que d) implique b) résulte d’*Alg.*, chap. VI, $§ 1$, no 13, th. 2 appliqué au groupe $\mathcal{P}^*$.

Montrons que b) implique e). Si b) est vérifiée, on a un isomorphisme de $\mathcal{P}^*$ sur $\mathbf{Z}^{(l)}$; notons $(v_i(x))_{i \in I}$ l’élément de $\mathbf{Z}^{(l)}$ correspondant à l’idéal $Ax$ ($x \in K^*$). On voit aussitôt que chaque $v_i$ est une valuation discrète de $K$, que $A$ est l’intersection des anneaux des $v_i$, et que, pour $x \in K^*$, on a $v_i(x) = 0$ sauf pour un nombre fini d’indices $i$; donc $A$ est un anneau de Krull. D’autre part, soit $q$ un idéal premier de hauteur 1 de $A$; il contient un élément non nul $a$, nécessairement non inversible, donc aussi (par définition d’un idéal premier) l’un des éléments extrémaux $p$ de $A$; comme $Ap$ est premier non nul, on a $q = Ap$, ce qui montre bien que $q$ est principal.

Montrons enfin que e) implique a). Soit $a$ un idéal divisoriel de A. Il existe des idéaux premiers $p_i$ de hauteur 1 de A tels que $\operatorname{div}\alpha = \sum_i n_i \operatorname{div} p_i$ avec $n_i \in \mathbf{Z}$. Si e) est satisfaite, $p_i$ est de la forme $Ap_i$, d’où $\operatorname{div}\alpha = \operatorname{div}\left( \prod_i Ap_i^{n_i} \right)$, donc $\alpha = \prod_i Ap_i^{n_i}$ puisque $\alpha$ est divisoriel.

C.Q.F.D.

#### Proposition 1 {#ac-vii-s3-prop-1 .statement}

Soit A un anneau de Krull. Si tout idéal divisoriel de A est inversible, alors, pour tout idéal maximal m de A, $A_m$ est factoriel. La réciproque est vraie si on suppose en outre que tout idéal divisoriel de A est de type fini (en particulier si A est noethérien).

Supposons que tout idéal divisoriel de A soit inversible; comme $A_m$ est un anneau de Krull (§ 1, n° 4, prop. 6), tout idéal divisoriel $\alpha$ de $A_m$ est intersection de deux idéaux fractionnaires principaux (§ 1, n° 5, cor. 2 de la prop. 9); donc $\alpha = bA_m$, où b est un idéal divisoriel de A (chap. II, § 2, n° 4); comme b est inversible par hypothèse, on déduit du chap. II, § 5, n° 6, th. 4 que $\alpha$ est principal, donc $A_m$ est un anneau factoriel (n° .1, déf. 1). Inversement, si tous les $A_m$ sont factoriels, et si c est un idéal divisoriel de type fini de A, $cA_m$ est un idéal divisoriel de $A_m$, comme il résulte du § 1, n° 5, cor. 2 de la prop. 9 et du chap. II, § 2, n° 4; par hypothèse $cA_m$ est principal, donc il résulte du chap. II, § 5, n° 6, th. 4 que c est inversible.

### 3. Décomposition en éléments extrémaux

Soient A un anneau intègre, K son corps des fractions, et U le groupe multiplicatif des éléments inversibles de A. Rappelons (Alg., chap. VI, § 1, n° 5) qu’on a un isomorphisme canonique de $K^*/U$ sur le groupe $\mathcal{P}^*$ des idéaux principaux fractionnaires non nuls de A. La condition b) du th. 1 se traduit alors de la manière suivante:

#### Proposition 2 {#ac-vii-s3-prop-2 .statement}

Soit A un anneau intègre. Pour que A soit factoriel, il faut et il suffit qu’il existe une partie P de A telle que tout $a \in A - \{0\}$ s’écrive de manière unique sous la forme $a = u \prod_{p \in P} p^{n(p)}$, où $u \in U$, et où les $n(p)$ sont des entiers positifs, nuls sauf un nombre fini d’entre eux.

Si P vérifie cette condition, il est clair que tous ses éléments sont extrémaux, et que tout élément extrémal de A est associé à

Supposons toujours A factoriel. On a vu (n° 2, th. 1) que le groupe $\mathcal{P}^*$ est réticulé. On peut donc appliquer les résultats d’Alg., chap. VI, § 1, n°s 9 à 13. En particulier, tout élément de K* s’écrit, d’une façon et essentiellement d’une seule, sous forme de fraction irréductible. Deux éléments quelconques $a, b$ de K* ont un p.g.c.d. et un p.p.c.m.; si $a = u \prod_{p \in P} p^{n(p)}$ et $b = u' \prod_{p \in P} p^{m(p)}$ sont des décompositions de $a$ et $b$ en produits d’éléments extrémaux, on a:

(1) $\text{p.g.c.d. } (a, b) = w \prod_{p \in P} p^{\inf(m(p), n(p))}$

(2) $\text{p.p.c.m. } (a, b) = w' \prod_{p \in P} p^{\sup(m(p), n(p))}$

avec $w, w'$ dans U. On retrouve, en particulier, les résultats d’Alg., chap. VII, § 1, n° 3.

Pour tout $p \in P$, l’application $a \to n(p)$ est une valuation discrète $v_p$ de K, dont l’anneau est évidemment $A_{A_p}$. Il résulte du th. 1, e) que les $v_p$ ne sont autres que les valuations essentielles de A, et que les idéaux $Ap$ ($p \in P$) ne sont autres que les idéaux premiers de hauteur 1 de A.

### 4. Anneaux de fractions d’un anneau factoriel

#### Proposition 3 {#ac-vii-s3-prop-3 .statement}

Soient A un anneau de Krull, S une partie multiplicative de A ne contenant pas 0.
(i) Si A est factoriel, $S^{-1}A$ est factoriel.
(ii) Si S est engendrée par une famille d’éléments $p_i$ telle que les idéaux principaux $Ap_i$ soient premiers, et si $S^{-1}A$ est factoriel, alors A est factoriel.

Cela résulte aussitôt de la déf. 1 du n° 1 et du § 1, n° 10, prop. 17.

### 5. Anneaux de polynômes sur un anneau factoriel

Soient A un anneau factoriel, K son corps des fractions, et $f$ un élément non nul de $K[X]$; un élément c de $K^*$ sera appelé un contenu de $f$ si c’est un p.g.c.d. des coefficients de $f$. Soient $v$ une valuation de K essentielle pour A, et $\bar{v}$ son prolongement canonique

#### Lemme 1 (Gauss) {#ac-vii-s3-lem-1 .statement}

Soient $f, f'$ des éléments non nuls de K[X], $c, c'$ des contenus de $f, f'$. Alors $cc'$ est un contenu de $ff'$.
Soit $d$ un contenu de $ff'$. Pour toute valuation $v$ de K essentielle pour A, notons $\bar{v}$ son prolongement canonique à K[X]. On a $v(d) = \bar{v}(ff') = \bar{v}(f) + \bar{v}(f') = v(c) + v(c') = v(cc')$. Donc $cc'd^{-1}$ est un élément inversible de A.

#### Théorème 2 {#ac-vii-s3-thm-2 .statement}

Soient A un anneau factoriel, K son corps des fractions, ($p_\lambda$) un système représentatif d’éléments extrémaux de A, et ($P_\lambda$) un système représentatif de polynômes irréductibles de K[X], chaque $P_\lambda$ ayant pour contenu 1. Alors :
(i) A[X] est un anneau factoriel ;
(ii) l’ensemble des $p_\lambda$ et des $P_\lambda$ est un système représentatif d’éléments extrémaux de A[X].
Soit $f$ un élément non nul de A[X]. Dans l’anneau K[X], on peut décomposer $f$ de manière unique sous la forme :
$$
f = a \prod_\lambda P_\lambda^{n(\lambda)} \quad (a \in K^*,\ n(\lambda) \geqslant 0).
$$
La lemme 1 prouve que $a$ est un contenu de $f$. Donc $a \in A$. Comme A est factoriel, on peut décomposer $a$ de manière unique sous la forme :
$$
a = u \prod_\iota p_\iota^{m(\iota)} \quad (u \text{ inversible dans } A,\ m(\iota) \geqslant 0).
$$
D’où l’existence et l’unicité de la décomposition :
$$
f = u \prod_\iota p_\iota^{m(\iota)} \prod_\lambda P_\lambda^{n(\lambda)}.
$$
On notera que cette proposition prouve que tout élément de A admet la même décomposition en éléments extrémaux dans A et dans A[X]. Le p.g.c.d. d’une famille d’éléments de A est donc le même dans A et dans A[X].

On peut aussi utiliser la prop. 18 du § 1, n° 10, pour montrer que A[X] est un anneau factoriel si et seulement si A est factoriel.

#### Corollaire {#ac-vii-s3-n5-cor-1 .statement}

Si A est un anneau factoriel, l’anneau $A[X_1, \ldots, X_n]$ est factoriel.
On raisonne par récurrence sur $n$.

Ce corollaire s’étend au cas d’une famille infinie d’indéterminées (cf. exerc. 2).

### 6. Anneaux factoriels et anneaux de Zariski

#### Proposition 4 {#ac-vii-s3-prop-4 .statement}

Soient $\mathbf{A}$ un anneau de Zariski, $\hat{\mathbf{A}}$ son complété. Si $\hat{\mathbf{A}}$ est factoriel, $\mathbf{A}$ est factoriel.
Cela résulte du n° 1, déf. 1, et du § 1, n° 10, prop. 16.

COROLLAIRE . — Si le complété d’un anneau local noethérien $\mathbf{A}$ est factoriel, $\mathbf{A}$ est factoriel.

### 7. Préliminaires sur les automorphismes des anneaux de séries formelles

#### Lemme 2 {#ac-vii-s3-lem-2 .statement}

Soit $f(X_1, X_2, \ldots, X_n)$ une série formelle $\neq 0$ à coefficients dans un anneau $E$. Il existe des entiers $u(i) \geqslant 1$ ($1 \leqslant i \leqslant n - 1$) tels que $f(T^{u(1)}, \ldots, T^{u(n-1)}, T) \neq 0$.
Supposons déterminés des entiers $u(i) \geqslant 1$ ($1 \leqslant i \leqslant k - 1$) tels que $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X_n) \neq 0$. Nous allons déterminer un entier $u(k) \geqslant 1$ tel que
$$
f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_n^{u(k)}, X_{k+1}, \ldots, X_n) \neq 0.
$$
Le lemme sera alors démontré par récurrence.
Observons que la série $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X_n)$ peut être considérée comme une série en $X_k$ et $X_n$ à coefficients dans $E[[X_{k+1}, \ldots, X_{n-1}]]$. On voit ainsi qu’il suffit d’établir le lemme pour $n = 2$.
Soit donc
$$
f = \sum_{i,j} e_{ij} X^i Y^j \in E[[X, Y]]
$$
avec $f \neq 0$. Soit $G \subset \mathbf{N} \times \mathbf{N}$ l’ensemble non vide des couples $(i, j)$ tels que $e_{ij} \neq 0$. Munissons $\mathbf{N} \times \mathbf{N}$ de l’ordre lexicographique. Soit $(c, d)$ le plus petit élément de $G$. Choisissons un entier $p > d$.
Dans le développement de $f(T^p, T) = \sum_{(i,j) \in G} e_{ij} T^{ip+j}$, cherchons quels sont les termes de degré $cp + d$. Si $ip + j = cp + d$, on ne peut avoir $i \geqslant c + 1$, car ceci donnerait
$$
ip + j \geqslant (c + 1)p + j \geqslant (c + 1)p > cp + d;
$$
on ne peut pas non plus avoir $i < c$, car $(c, d)$ est le plus petit élément de $G$; on a donc $i = c$, et alors $j = d$. Le terme de degré cp + d de $f(T^p, T)$ est donc $e_{cd} T^{cp+d}$. Puisque $e_{cd} \neq 0$, on a $f(T^p, T) \neq 0$. D’où le lemme.

Dans l’anneau $E[[X_1, \ldots, X_n]]$, soit $\alpha$ l’idéal des séries formelles sans terme constant. Si $w_1, \ldots, w_n$ sont des éléments de $\alpha$, rappelons que l’application $f(X_1, \ldots, X_n) \to f(w_1, \ldots, w_n)$ est l’unique endomorphisme $s$ de l’anneau $E[[X_1, \ldots, X_n]]$ tel que $s(X_i) = w_i$ pour $1 \leq i \leq n$ (chap. III, § 4, no 5, prop. 6).

Prenons $w_1 = X_1 + X_n^{u(1)}, \ldots, w_{n-1} = X_{n-1} + X_n^{u(n-1)}, w_n = X_n$, où les $u(i)$ sont des entiers $\geq 1$. Soit $s'$ l’endomorphisme de $E[[X_1, \ldots, X_n]]$ qui transforme $X_1$ en $X_1 - X_n^{u(1)}, \ldots, X_{n-1}$ en $X_{n-1} - X_n^{u(n-1)}$, et $X_n$ en $X_n$. On a $s'(s(X_i)) = X_i$ pour $1 \leq i \leq n$, donc $s' \circ s$ est l’automorphisme identique; de même $s \circ s'$. Donc $s$ est un automorphisme.

#### Lemme 3 {#ac-vii-s3-lem-3 .statement}

Soit $f$ un élément non nul de $E' = E[[X_1, ..., X_n]]$. Il existe des entiers $u(i) \geq 1$ ($1 \leq i \leq n-1$) tels que l’automorphisme $s$ de $E'$ défini par $s(X_i) = X_i + X_n^{u(i)}$ ($1 \leq i \leq n-1$) et $s(X_n) = X_n$ transforme $f$ en un élément $g$ tel que $g(0, ..., 0, X_n) \neq 0$.

En effet, on a $g(0, ..., 0, X_n) = f(X_n^{u(1)}, ..., X_n^{u(n-1)}, X_n)$. Le lemme 3 est donc une conséquence du lemme 2.

### 8. Le théorème de préparation

Dans ce no, on désigne par $A$ un anneau local, par $m$ son idéal maximal, par $k = A/m$ son corps résiduel. On suppose que $A$ est séparé et complet pour la topologie $m$-adique. Soit $B = A[[X]]$; c’est un anneau local dont l’idéal maximal $\mathfrak{N}$ est engendré par $m$ et $X$; pour la topologie $\mathfrak{N}$-adique, $B$ est séparé et complet (chap. III, § 2, no 6, prop. 6).

Pour toute série formelle
$$
f = \sum_{i=0}^{\infty} a_i X^i \in B,
$$
posons
$$
\bar{f} = \sum_{i=0}^{\infty} \bar{a}_i X^i \in k[[X]],
$$
où $\bar{a}_i$ désigne l’image canonique de $a_i$ dans $k$. La série $\bar{f}$ sera appelée la série réduite de $f$; si $\bar{f} \neq 0$, l’ordre de $\bar{f}$ (c’est-à-dire le plus petit entier $s$ tel que $a_s \notin m$) sera appelé l’ordre réduit de $f$.

#### Proposition 5 {#ac-vii-s3-prop-5 .statement}

Soit $f \in B$ une série dont la série réduite n’est pas nulle. Notons $s$ son ordre réduit, et $M$ le sous-A-module de $B$ ayant $\{1, X, ..., X^{s-1}\}$ pour base. Alors $B$ est somme directe de $M$ et de $fB$ et $f$ n’est pas diviseur de zéro dans $B$.

a) Montrons que $fB \cap M = (0)$. Supposons que l’on ait une relation :

(3) $\left( \sum_{i=0}^{\infty} b_i X^i \right) f = r_0 + r_1 X + \cdots + r_{s-1} X^{s-1} \quad (b_i \in A, r_j \in A)$.

Montrons que les $b_i$ (donc les $r_j$) sont tous nuls, ce qui prouvera en particulier que $f$ n’est pas diviseur de zéro dans B. Puisque A est séparé, il suffit de montrer que $b_i \in m^n$ pour tout $i \geq 0$ et tout $n \geq 0$. C’est évident pour $n = 0$. Nous raisonnons par double récurrence : nous supposerons qu’on a $b_i \in m^{n-1}$ pour tout $i$ et $b_i \in m^n$ pour $i < k$, et nous démontrerons que ceci implique $b_k \in m^n$. Pour cela, posons $f = \sum_{i=1}^{\infty} a_i X^i$, et comparons les coefficients de $X^{s+k}$ dans (3); il vient :

(4)
$$
(b_0 a_{s+k} + \cdots + b_{k-1} a_{s+1}) + b_k a_s + (b_{k+1} a_{s-1} + \cdots + b_{k+s} a_0) = 0.
$$
Les termes de la première parenthèse appartiennent à $m^n$ puisque $b_i \in m^n$ pour $i < k$; il en est de même de ceux de la seconde, puisque $b_i \in m^{n-1}$ pour tout $i$ et que $a_i \in m$ pour $i \leq s - 1$. Donc $b_k a_s \in m^n$, et, comme $a_s$ est un élément inversible de A, on a bien $b_k \in m^n$.

b) Montrons que $fB + M = B$. Posons
$$
g = a_s + a_{s+1} X + a_{s+2} X^2 + \cdots;
$$
c’est un élément inversible de B. On a
$$
f - X^s g = a_0 + a_1 X + \cdots + a_{s-1} X^{s-1};
$$
si donc on pose $fg^{-1} - X^s = (f - X^s g) g^{-1} = -h$, les coefficients de $h$ appartiennent à $m$. Ceci posé, soit $r$ un élément de B. Par récurrence sur $n$, définissons une suite $(q^{(n)})$ d’éléments de B : on prend pour $q^{(0)}$ l’unique série vérifiant :
(5)
$$
r \equiv X^s q^{(0)} \pmod{M};
$$
posant $h = \sum_{i=0}^{\infty} h_i X^i$ et $q^{(n)} = \sum_{i=0}^{\infty} q_i^{(n)} X^i$, les $q_i^{(n)}$ sont définis par :
(6)
$$
q_i^{(n)} = \sum_{j=0}^{i+s} h_j q_{i+s-j}^{(n-1)}
$$
Il résulte aussitôt de (6) qu’on a :
(7)
$$
X^s q^{(n)} \equiv h q^{(n-1)} \pmod{M}.
$$
Comme on a $h_j \in m$ pour tout $j$, il résulte aussi de (6), par récurrence sur $n$, qu’on a $q_i^{(n)} \in m^n$ pour tout $i$ et pour tout $n$. Comme $A$ est complet, il s’ensuit que la série $q^{(0)} + q^{(1)} + \cdots + q^{(n)} + \cdots$ converge vers un élément $q$ de $B$. D’après (5) et (7), on a :

(8)
$$
X^s(q^{(0)} + q^{(1)} + \cdots + q^{(n)}) \equiv r + h(q^{(0)} + \cdots + q^{(n-1)}) \pmod{M}.
$$
Comme $M$ est fermé, (8) donne à la limite $r \equiv (X^s - h)q \pmod{M}$, c’est-à-dire $r \in f g^{-1}q + M \subset fB + M$.

C.Q.F.D.

On peut aussi utiliser les résultats du chap. III, § 2, pour démontrer la relation $B = fB + M$ (cf. exerc. 12): La méthode suivie ici a l’avantage de s’appliquer aux séries convergentes.

#### Corollaire {#ac-vii-s3-n8-cor-1 .statement}

Les hypothèses et notations étant celles de la prop. 5, on suppose que $s \geqslant 1$, de sorte que $f \in Bm + BX$. Alors le $A$-homomorphisme $h$ de $B' = A[[T]]$ dans $B = A[[X]]$ tel que $h(T) = f$ (chap. III, § 2, n° 9, prop. 11, a) définit sur $B$ une structure de $B'$-module libre admettant $\{1, X, \ldots, X^{s-1}\}$ pour base. En particulier $h$ est injectif.

Munissons en effet le $B'$-module $B$ de la filtration (T)-adique, qui est formée des $f^n B$ pour $n \geqslant 0$ (chap. III, § 2, n° 1). Alors $B/fB$ est un module libre sur l’anneau $A = B'/TB'$, et les images des $X^i$ ($0 \leqslant i \leqslant s-1$) dans cet $A$-module en forment une base (prop. 5); comme en outre $f$ n’est pas diviseur de zéro dans $B$ (prop. 5), $Bf^n/Bf^{n+1}$ est aussi un $(B'/TB')$-module libre de rang $s$, de sorte que la condition (GR) du chap. III, § 2, n° 8 est satisfaite (en y remplaçant $A$ par $B'$ et $M$ par $B$). D’autre part, puisque $B'$ est séparé et complet pour la filtration (T)-adique, et que $\mathrm{gr}(B)$ est un $\mathrm{gr}(B')$-module de type fini en vertu de ce qui précède, on voit d’abord (chap. III, § 2, n° 9, cor. 1 de la prop. 12) que $B$ est un $B'$-module de type fini. La première assertion du corollaire résulte alors du chap. III, § 2, n° 9, prop. 13. La seconde s’en déduit aussitôt.

#### Définition 2 {#ac-vii-s3-def-2 .statement}

On dit qu’un polynôme $F = A[X]$ est distingué s’il est de la forme $F = X^s + a_{s-1} X^{s-1} + \cdots + a_0$, avec $a_i \in m$ pour $0 \leqslant i \leqslant s-1$.

Notons que le produit de deux polynômes distingués est un polynôme distingué.

#### Proposition 6 (Théorème de préparation) {#ac-vii-s3-prop-6 .statement}

Soient $f \in \mathbf{B}$ une série dont la série réduite n’est pas nulle, et s son ordre réduit. Il existe alors un couple $(u, F)$ et un seul tel que $u$ soit un élément inversible de $\mathbf{B}$, $F$ un polynôme distingué de degré $s$, et $f = uF$.

Posons $F = X^s + G$, avec $G = g_0 + \cdots + g_{s-1}X^{s-1}$ ($g_i \in \mathbf{A}$). La relation $f = uF$ équivaut à $F = u^{-1}f$, c’est-à-dire à $X^s = u^{-1}f - G$. Donc la prop. 5 montre l’unicité de $G$ et de $u^{-1}$, et par suite de $F$ et de $u$. Elle montre aussi qu’il existe $v \in \mathbf{B}$, et un polynôme $G = g_0 + \cdots + g_{s-1}X^{s-1}$ ($g_i \in \mathbf{A}$) tels que $X^s = vf - G$; il reste à démontrer que $v$ est inversible dans $\mathbf{B}$, et qu’on a $g_i \in m$ pour tout $i$. Or, en notant $\bar{g}_i$ l’image canonique de $g_i$ dans $k$, et $\bar{f}, \bar{v}$ les séries réduites de $f, g$, on a:

$$
X^s + \bar{g}_0 + \bar{g}_1X + \cdots + \bar{g}_{s-1}X^{s-1} = \bar{f}\bar{v};
$$

puisque $\bar{f}$ est d’ordre $s$, on a $\bar{g}_i = 0$ pour tout $i$, et $\bar{v}$ est d’ordre 0, donc $v$ est inversible.

C.Q.F.D.

#### Proposition 7 {#ac-vii-s3-prop-7 .statement}

Soient $F$ un polynôme distingué, et $g, h$ deux séries formelles de $\mathbf{B}$ telles que $F = gh$. Il existe alors un élément inversible $u$ de $\mathbf{B}$ tel que $ug$ et $u^{-1}h$ soient des polynômes distingués, et l’on a $F = (ug)(u^{-1}h)$.

En effet, les séries réduites de $g$ et $h$ sont $\neq 0$; donc, d’après la prop. 6, il existe des éléments inversibles $u, v$ de $\mathbf{B}$ tels que $ug$ et $vh$ soient des polynômes distingués. Alors $uvF = (ug)(vh)$ est un polynôme distingué, et $uv$ est inversible. Par passage aux séries réduites, on voit aussitôt que $F$ et $uvF$ ont même ordre réduit, c’est-à-dire même degré. L’assertion d’unicité dans la prop. 6 montre donc qu’on a $F = uvF$, d’où $uv = 1$.

#### Corollaire {#ac-vii-s3-n8-cor-2 .statement}

Supposons en outre que $\mathbf{A}$ soit intègre, et soit $F$ un polynôme distingué de degré $s$. Pour que $F$ soit extrémal dans $\mathbf{A}[X]$, il faut et il suffit qu’il soit extrémal dans $\mathbf{B} = \mathbf{A}[[X]]$.

Supposons que $F$ ne soit pas extrémal dans $\mathbf{A}[X]$, de sorte que l’on a $F = f_1f_2$, où $f_1$ et $f_2$ sont des éléments non inversibles de $\mathbf{A}[X]$; le produit des coefficients dominants de $f_1$ et $f_2$ étant égal à 1, ces coefficients sont inversibles dans $\mathbf{A}$, et l’hypothèse entraîne que $f_1$ et $f_2$ sont de degrés $> 0$ et $< s$; comme les polynômes réduits $\bar{f}_1, \bar{f}_2$ sont tels que $\bar{f}_1\bar{f}_2 = X^s$, ni $\bar{f}_1$ ni $\bar{f}_2$ ne peut être inversible dans $k[[X]]$, car si $\bar{f}_1$ était inversible, $\bar{f}_2$ serait d’ordre $s$, ce qui est absurde. *A fortiori*, ni $f_1$ ni $f_2$ n’est inversible dans B, et F est non extrémal dans B.

Réciproquement, si F n’est pas extrémal dans $A[[X]]$, on a $F = gh$, où ni g ni h n’est inversible dans B ; leurs ordres réduits sont donc $\geqslant 1$; alors les polynômes distingués $ug$ et $u^{-1}h$ de la prop. 7 ne sont pas constants, ce qui montre que F n’est pas extrémal dans $A[X]$.

### 9. *Factorialité des anneaux de séries formelles*

#### Proposition 8 {#ac-vii-s3-prop-8 .statement}

*Soit C un anneau qui est, soit un corps, soit un anneau de valuation discrète. Alors l’anneau de séries formelles $C[[X_1, \ldots, X_n]]$ est factoriel.*

Soient $\mathfrak{p}$ l’idéal maximal de C, et $\pi$ un générateur de $\mathfrak{p}$ (si C est un corps, on a $\pi = 0$). Munissons C de la topologie $\mathfrak{p}$-adique, qui est séparée. Comme C est un anneau local noethérien, $B = C[[X_1, \ldots, X_n]]$ est un anneau local noethérien, et son complété est $\hat{C}[[X_1, \ldots, X_n]]$ (chap. III, § 2, n° 6, prop. 6). D’après le cor. de la prop. 4 (n° 6), il suffit de prouver que $\hat{C}[[X_1, \ldots, X_n]]$ est factoriel. Or, si C est un corps, on a $\hat{C} = C$; si C est un anneau de valuation discrète, il en est de même de $\hat{C}$ (chap. VI, § 5, n° 3, prop. 5). Nous supposerons donc, dans la suite de la démonstration, que C est *complet*.

Raisonnant par récurrence à partir du cas trivial $n = 0$, nous supposerons démontré que $A = C[[X_1, \ldots, X_{n-1}]]$ est factoriel. Nous identifierons B à $A[[X_n]]$, et nous noterons m l’idéal maximal de A (engendré par $\pi, X_1, \ldots, X_{n-1}$). Nous démontrerons que tout élément non nul g de B est, de façon essentiellement unique, produit d’éléments extrémaux.

Soit K le corps $C/C\pi$; comme $B/B\pi$ s’identifie à $K[[X_1, \ldots, X_n]]$, l’idéal $B\pi$ est premier, et $\pi$ est extrémal. Si $\pi \neq 0$, $B_{B\pi}$ est donc l’anneau d’une valuation discrète normée w (chap. VI, § 3, n° 6, prop. 9); tout élément non nul g de B s’écrit donc $g = \pi^{w(g)}f$, avec $f \in B$ et $f$ non multiple de $\pi$. Il suffira donc de démontrer que $f$ est, de façon essentiellement unique, produit d’éléments extrémaux. Or l’image canonique de $f$ dans $K[[X_1, \ldots, X_n]]$ n’est pas nulle; le lemme 3 (n° 7) montre donc qu’il existe un automorphisme de B qui transforme $f$ en un élément $f'$ tel que les coefficients de $f'(0, \ldots, 0, X_n)$ ne soient pas tous dans $C\pi$; ceci veut dire que les coefficients de la série $f'$, considérée comme série formelle en

X_n, ne sont pas tous dans m. Il suffira de démontrer notre assertion pour $f'$.

Dans la suite, tous les éléments de B seront considérés comme des séries formelles en $X_n$ à coefficients dans A. D’après la prop. 6 du n° 8 (applicable puisque C, et donc A, sont séparés et complets, et que la série réduite de $f'$ est $\neq 0$), $f'$ est associée, dans B, à un polynôme distingué et à un seul F. D’après la prop. 7 du n° 8, toute série qui divise $f'$ (ou, ce qui revient au même, qui divise F) est associée à un polynôme distingué qui divise F, et toute décomposition de $f'$ est, à des facteurs inversibles près, de la forme $f' = u F_1 \ldots F_q$, où $u$ est inversible et où les $F_i$ sont des polynômes distingués extrémaux (dans B) tels que $F = F_1 \ldots F_q$. D’après le cor. de la prop. 7 du n° 8, les $F_i$ sont aussi extrémaux dans $A[X_n]$. Or, comme A est factoriel d’après l’hypothèse de récurrence, il en est de même de $A[X_n]$ (th. 2, n° 5); donc, puisqu’ils sont unitaires, les $F_i$ sont déterminés de façon unique par F (à une permutation près). Ceci montre l’unicité de la décomposition $f' = u F_1 \ldots F_q$; son existence résulte du fait que B est noethérien ce qui termine la démonstration.

#### Remarque 1 {#ac-vii-s3-n9-rem-1 .statement}

Il existe des anneaux factoriels A tels que l’anneau $A[[X]]$ ne soit pas factoriel (exerc. 8). Cependant, si A est principal, $A[[X_1, \ldots, X_n]]$ est factoriel (exerc. 9).

#### Remarque 2 {#ac-vii-s3-n9-rem-2 .statement}

\* Nous verrons plus tard, par des méthodes homologiques, que tout anneau local régulier est factoriel (cf. § 4, n° 7, cor. 3 de la prop. 16). Cela donnera une autre démonstration, conceptuellement plus simple, de la prop. 8.*

## EXERCICES {#ac-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
