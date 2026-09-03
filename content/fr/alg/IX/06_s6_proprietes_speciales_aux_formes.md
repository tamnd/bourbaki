---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 6
section_title: Propriétés spéciales aux formes hermitiennes
lang: fr
source: alg-ix-fr
pdf_pages: 0088-0112
extraction: ocr
subsections:
    - "no": 1
      title: Bases orthogonales.
      page: 0
      pdf_page: 88
    - "no": 2
      title: Groupe unitaire et groupe orthogonal.
      page: 0
      pdf_page: 91
    - "no": 3
      title: Projecteurs orthogonaux et involutions.
      page: 0
      pdf_page: 93
    - "no": 4
      title: Symétries dans le groupe orthogonal.
      page: 0
      pdf_page: 95
    - "no": 5
      title: Groupe des similitudes.
      page: 0
      pdf_page: 96
    - "no": 6
      title: Géométrie hermitienne.
      page: 0
      pdf_page: 98
statements: 17
exercises: 0
content_sha256: 783f2b68bfc70c755e7a59da78ba4ea7f91f435a5f45796c2931ea0e513f2e14
---

## § 6. Propriétés spéciales aux formes hermitiennes

### 1. Bases orthogonales.

#### Définition 1 {#alg-ix-s6-def-1 .statement}

Soit $\Phi$ une forme hermitienne sur $E$. Une base $(e_i)$ de $E$ est dite orthogonale pour $\Phi$ si deux éléments quelconques de cette base sont orthogonaux pour $\Phi$.

Si de plus $\Phi(e_i, e_i) = 1$ pour tout $i$, la base $(e_i)$ est dite orthonormale.

Soit $(e_i)$ une base orthogonale ; si on pose $\Phi(e_i, e_i) = \alpha_i$, on a
$$
\Phi(\sum_i \xi_i e_i, \sum_i \eta_i e_i) = \sum_i \xi_i \alpha_i \overline{\eta_i}.
$$

#### Lemme 1 {#alg-ix-s6-lem-1 .statement}

On suppose que $A$ est un corps et $\Phi$ une forme hermitienne $\neq 0$ sur $E$. Si tous les vecteurs de $E$ sont isotropes, $A$ est un corps commutatif de caractéristique 2, l’antiautomorphisme $J$ est l’identité et $\Phi$ est alternée.

En effet, si l’on développe $\Phi(x + y, x + y) = 0$, il vient, en tenant compte des hypothèses $\Phi(x, x) = \Phi(y, y) = 0$, la relation $\Phi(x, y) = -\overline{\Phi(x, y)}$ quels que soient $x, y$ dans $E$. Comme $\Phi$ est $\neq 0$, il existe $x, y$ dans $E$ tels que $\Phi(x, y) = 1$. Écrivant que $\Phi(\lambda x, y) = -\Phi(\lambda x, y)$, il vient $\overline{\lambda} = -\lambda$ pour tout $\lambda \in A$. En prenant d’abord $\lambda = 1$, on voit que $A$ est de caractéristique 2 ; la relation $\overline{\lambda} = -\lambda$ montre alors que $J$ est l’identité, donc $A$ est commutatif et $\Phi$ est alternée.

#### Théorème 1 {#alg-ix-s6-thm-1 .statement}

Supposons que $A$ soit un corps et $E$ un espace vectoriel de dimension finie $n$ sur $A$. Alors, pour toute forme hermitienne $\Phi$ sur $E$, $E$ admet une base orthogonale, sauf si les conditions suivantes sont simultanément réalisées :

(C) $A$ est commutatif de caractéristique 2, l’antiautomorphisme $J$ est l’identité, $\Phi$ est alternée et non nulle.

Raisonnons par récurrence sur $n$, le résultat étant évident pour $n = 0$. On peut supposer $\Phi \neq 0$. Si (C) n’est pas vérifiée, le lemme 1 montre qu’il existe un élément $x \in E$ tel que $\Phi(x, x) \neq 0$. Soit $H$ le sous-espace de $E$ orthogonal à $x$; il est de dimension $\geq n - 1$, et, comme $x \in \mathbf{H}$, $\mathbf{H}$ est exactement de dimension $n - 1$. Si la restriction $\Psi$ de $\Phi$ à $\mathbf{H}$ ne vérifie pas (C), il existe, d’après l’hypothèse de récurrence, une base $(e_2, \ldots, e_n)$ de $\mathbf{H}$ qui est orthogonale pour $\Psi$; en posant $e_1 = x$, on obtient une base orthogonale $(e_1, e_2, \ldots, e_n)$ de $\mathbf{E}$. Il reste à examiner le cas où $\mathbf{A}$ est un corps commutatif de caractéristique 2, où $\mathbf{J}$ est l’identité, et où $\Psi$ est alternée et $\neq 0$. Il existe alors $y, z$ dans $\mathbf{H}$ tels que $\Psi(y, z) \neq 0$; posons $e_1 = x + y$; pour que $x + \lambda z (\lambda \in \mathbf{A})$ soit orthogonal à $e_1$, il faut et il suffit quel’on ait $0 = \Phi(x + y, x + \lambda z) = \Phi(x, x) + \lambda \Psi(y, z)$, condition qui détermine $\lambda$ de façon unique; le scalaire $\lambda$ étant ainsi choisi, on a $\Phi(x + \lambda z, x + \lambda z) = \Phi(x, x) \neq 0$, donc la restriction $\Psi'$ de $\Phi$ au sous-espace $\mathbf{H}'$ de $\mathbf{E}$ orthogonal de $e_1$ n’est pas alternée; on peut par suite appliquer l’hypothèse de récurrence à $\mathbf{H}'$, ce qui démontre le théorème.

Lorsque (C) est vérifiée, il n’existe évidemment pas de base orthogonale pour $\Phi$.

#### Corollaire 1 {#alg-ix-s6-thm-1-cor-1 .statement}

*Les notations étant celles du th. 1, on suppose de plus que (C) n’est pas vérifiée, que $\Phi$ est non dégénérée et que, pour tout $x \in \mathbf{E}$, il existe $\rho \in \mathbf{A}$ tel que $\Phi(x, x) = \rho \bar{\rho}$. Alors $\mathbf{E}$ admet une base orthonormale pour $\Phi$*.

Soit en effet $(e_i)$ ($i = 1, \ldots, n$) une base orthogonale de $\mathbf{E}$. Posons $\Phi(e_i, e_i) = \alpha_i$. On a $\alpha_i \neq 0$ pour $i = 1, \ldots, n$ puisque $\Phi$ est non dégénérée. Il existe, par hypothèse, des éléments $\beta_i$ de $\mathbf{A}$ tels que $\alpha_i = \beta_i \overline{\beta_i}$ pour $i = 1, \ldots, n$; on a $\beta_i \neq 0$. En posant $f_i = \beta_i^{-1} e_i$, on a $\Phi(f_i, f_i) = \beta_i^{-1} \alpha_i \overline{\beta_i^{-1}} = 1$ pour tout $i$, et $\Phi(f_i, f_j) = 0$ pour $i \neq j$. Donc $(f_i)$ est une base orthonormale.

#### Remarque {#alg-ix-s6-n1-rem-1 .statement}

La dernière hypothèse du corollaire est vérifiée lorsque $\mathbf{J}$ est l’identité, et que tout élément de $\mathbf{A}$ est le carré d’un élément de $\mathbf{A}$ (par exemple lorsque $\mathbf{A}$ est algébriquement clos).

#### Corollaire 2 {#alg-ix-s6-thm-1-cor-2 .statement}

*Soient $\mathbf{A}$ un corps et $R$ une matrice hermitienne d’ordre $n$ et de rang $r$ sur $\mathbf{A}$. Alors, sauf si la condition suivante est vérifiée :

(C') $\mathbf{A}$ est commutatif de caractéristique 2, $\mathbf{J}$ est l’identité, $R$ est alternée et non nulle,* il existe une matrice inversible $P$ d’ordre $n$ sur $A$ telle que

$$
tP . R . \overline{P} = \begin{pmatrix}
\alpha_1 & 0 \ldots 0 \ldots 0 \\
0 & \alpha_2 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots \alpha_r \ldots 0 \\
0 & 0 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots 0 \ldots 0
\end{pmatrix}
$$

où $\overline{\alpha}_i = \alpha_i \neq 0$ pour $i = 1, \ldots, r$.

#### Proposition 1 {#alg-ix-s6-prop-1 .statement}

*On suppose que $A$ est un corps commutatif. Soient $\Phi$ une forme hermitienne sur $E$, et $(x_n)$ ($n = 1, 2, \ldots$) une suite (finie ou infinie) de vecteurs linéairement indépendants de $E$ telle que, pour tout $n$, le sous-espace $E_n = Ax_1 + \cdots + Ax_n$ soit non isotrope. Soit $D_{jn}$ ($j \leq n$) le cofacteur de $\Phi(x_j, x_n)$ dans la matrice $(\Phi(x_s, x_t))_{(s,t=1,\ldots,n)}$. On a alors $D_{nn} \neq 0$ pour tout $n$. Posons*

$$
e_n = \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j.
$$

Alors, pour tout $n$, $(e_1, \ldots, e_n)$ est une base orthogonale de $E_n$ et l’on a

$$
\Phi(e_n, e_n) = D_{nn}^{-1} D_{n+1, n+1}.
$$

En effet, comme la restriction de $\Phi$ à $E_{n-1}$ est non dégénérée, on a $D_{nn} \neq 0$ (§ 2, prop. 3) ; notons que l’on a $D_{11} = 1$ puisque le déterminant de la matrice vide est égal à 1. Les formules (2) impliquent d’abord que l’on a $e_n \equiv x_n$ (mod. $E_{n-1}$) pour tout $n$, donc que les $e_n$ sont linéairement indépendants, et que $(e_1, \ldots, e_n)$ est une base de $E_n$. Pour tout $j < n$, on a

$$
\Phi(e_n, x_j) = D_{nn}^{-1} \sum_{k=1}^n D_{kn} \Phi(x_k, x_j) = 0
$$

(chap. III, § 6, n° 1, formule (12)) ; donc $e_n$ est orthogonal à $E_{n-1}$, et en particulier à $e_j$ pour $j < n$. D’autre part on a

$$
\Phi(e_n, e_n) = \Phi(e_n, \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j) = \Phi(e_n, x_n) = \Phi(\sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j, x_n)
$$
$$
= D_{nn}^{-1} \sum_{j=1}^n D_{jn} \Phi(x_j, x_n) = D_{nn}^{-1} D_{n+1, n+1}
$$

(chap. III, § 6, n° 1, formule (10)). Ceci démontre nos assertions.

Avec les notations de la prop. 1, on dit que la suite $(e_n)$ est obtenue à partir de la suite $(x_n)$ par le procédé d’orthogonalisation de Gram-Schmidt.

#### Proposition 2 {#alg-ix-s6-prop-2 .statement}

Soient $\Phi$ une forme hermitienne sur $E$, et $(e_i)$ $(i = 1, \ldots, n)$ une base orthogonale (resp. orthonormale) de $E$ pour $\Phi$. Alors, pour tout $p \geqslant 0$, la base de $\bigotimes^p E$ formée des $e_{i_1} \otimes \cdots \otimes e_{i_p}$ et la base $(e_H)$ de $\wedge^p E$ (où $H$ parcourt l’ensemble des parties à $p$ éléments de $\{1, n\}$; cf. chap. III, § 5, n° 6) sont orthogonales (resp. orthonormales) pour les extensions de $\Phi$ à $\bigotimes^p E$ et $\wedge^p E$ respectivement ($§ 1$, n° 9). Si, de plus, les applications associées à $\Phi$ sont bijectives, la base $(e'_i)$ de $E^*$ duale de $(e_i)$ est orthogonale (resp. orthonormale) pour la forme inverse $\widehat{\Phi}$ de $\Phi$ ($§ 1$, n° 7).

Les assertions relatives à $\bigotimes^p E$ et $\wedge^p E$ résultent aussitôt des formules (35) et (37) du $§ 1$, n° 9. Celle relative à la forme inverse résulte de ce que la matrice de $\widehat{\Phi}$ par rapport à $(e'_i)$ est l’inverse de la matrice de $\Phi$ par rapport à $(e_i)$ ($§ 1$, n° 10).

### 2. Groupe unitaire et groupe orthogonal.

Soit $\Phi$ une forme hermitienne sur $E$; les automorphismes du A-module $E$ qui laissent $\Phi$ invariante s’appellent automorphismes unitaires (ou transformations unitaires) relatifs à $\Phi$, et leur groupe s’appelle le groupe unitaire associé à $\Phi$; on le note $\mathbf{U}(\Phi)$. Étant donnée une forme quadratique $Q \neq 0$ sur $E$, les automorphismes du A-module $E$ qui laissent $Q$ invariante s’appellent automorphismes orthogonaux (ou transformations orthogonales) relatifs à $Q$; leur groupe s’appelle le groupe orthogonal associé à $Q$; on le note $\mathbf{O}(Q)$.

Toute transformation orthogonale pour une forme quadratique $Q$ est unitaire pour la forme bilinéaire associée à $Q$. La réciproque est vraie lorsque le scalaire 2 n’est pas égal à 0 ou diviseur de zéro dans $A$ ($§ 3$, n° 4, (13)), par exemple si $A$ est un corps de caractéristique $\neq 2$.

Considérons, en particulier, sur le module $E = A^n$, la forme hermitienne $\Phi_0$ dont la matrice par rapport à la base canonique (e_i) de E est la matrice unité $I_n$. Les automorphismes unitaires associés à $\Phi_0$ s’appellent tout simplement *automorphismes* (ou *transformations*) *unitaires à n variables* ; leur groupe est appelé *groupe unitaire à n variables* et se note parfois $\mathbf{U}(n, A)$ ou $\mathbf{U}_n(A)$. La matrice $U$ d’un automorphisme unitaire par rapport à $(e_i)$ s’appelle une *matrice unitaire*. Une telle matrice est inversible, et satisfait, d’après la formule (48) du § 1, n° 10, à la relation

$$(4)$$
$$
{}^t U \cdot \overline{U} = I_n;
$$

réciproquement, si A est un anneau commutatif ou est un corps, une matrice $U$ qui satisfait à (4) est inversible, et est alors unitaire.

Lorsque J est l’identité et que 2 n’est pas égal à 0 ni diviseur de 0 dans A, on emploie les termes de *groupe orthogonal à n variables*, d'*automorphisme orthogonal* (ou *transformation orthogonale*) à *n variables* et de *matrice orthogonale* au lieu des termes précédents, et on écrit $\mathbf{O}(n, A)$ (resp. $\mathbf{O}_n(A)$) au lieu de $\mathbf{U}(n, A)$ (resp. $\mathbf{U}_n(A)$). La relation (4) s’écrit alors

$$(5)$$
$$
{}^t U \cdot U = I_n
$$

et, comme A est commutatif, elle est une condition nécessaire et suffisante pour que $U$ soit une matrice orthogonale.

#### Proposition 3 {#alg-ix-s6-prop-3 .statement}

*Supposons que A soit un corps commutatif et que E soit de dimension finie $> 0$. Soit $\Phi$ une forme hermitienne non dégénérée sur E. L’application $u \to \det u$ est un homomorphisme du groupe unitaire $\mathbf{U}(\Phi)$ associé à $\Phi$ sur le sous-groupe multiplicatif H de A formé des éléments $\rho$ tels que $\rho \overline{\rho} = 1$ (sous-groupe réduit à $\{1, -1\}$ lorsque J est l’identité).

Soient en effet $u$ un élément de $\mathbf{U}(\Phi)$, $U$ sa matrice par rapport à une base de E, et $R$ la matrice de $\Phi$ par rapport à cette base. La relation $R = {}^t U \cdot R \cdot \overline{U}$ ($§ 1$, n° 10, formule (48)) montre que l’on a $(\det U)(\det \overline{U}) = 1$ puisque $R$ est inversible ; d’où $(\det u)(\det u) = 1$. L’homomorphisme $u \to \det u$ applique $\mathbf{U}(\Phi)$ sur H. En effet, lorsque A est de caractéristique 2 et J l’identité, H est réduit à l’élément 1. Sinon il existe une base orthogonale $(e_i)$ ($i = 1, \ldots, n$) de E (th. 1); pour tout $\rho \in A$ tel que $\rho \overline{\rho} = 1$, soit $u$ l’automorphisme de E défini par $u(e_1) = \rho e_1$ et $u(e_i) = e_i$ pour $i = 2, \ldots, n$; alors $u$ est unitaire et $\det u = \rho$, d’où la proposition.

Dans les conditions de la prop. 3, le noyau de l’homomorphisme $u \to \det u$ est un sous-groupe distingué de $\mathbf{U}(\Phi)$, qu’on appelle le groupe spécial unitaire associé à $\Phi$; on le note parfois $\mathbf{SU}(\Phi)$.

Lorsque $J$ est l’identité et que $A$ n’est pas de caractéristique 2, ce groupe est encore appelé le groupe spécial orthogonal associé à $\Phi$ (ou à la forme quadratique $Q(x) = \Phi(x, x)$) et se note parfois $\mathbf{SO}(Q)$.

Si $E = A^n$ et si $\Phi$ est la forme dont la matrice par rapport à la base canonique de $E$ est la matrice unité, on emploie les notations $\mathbf{SU}(n, A)$ ou $\mathbf{SU}_n(A)$ et $\mathbf{SO}(n, A)$ ou $\mathbf{SO}_n(A)$.

### 3. Projecteurs orthogonaux et involutions.

Dans tout ce n°, on suppose que le scalaire 2 est inversible dans $A$ (par exemple que $A$ est un corps de caractéristique $\neq 2$), et que $\Phi$ est une forme hermitienne non dégénérée sur $E$. On note $\frac{1}{2}$ l’inverse de 2.

#### Lemme 2 {#alg-ix-s6-lem-2 .statement}

Pour qu’un endomorphisme $u$ de $E$ soit tel que $u^2 = 1$, il faut et il suffit que $\frac{1}{2}(1 - u)$ soit un projecteur dans $E$; alors $u$ est la différence des deux projecteurs $\frac{1}{2}(1 + u)$ et $\frac{1}{2}(1 - u)$.

En effet, dans l’anneau $\mathcal{L}(E)$, la relation $\left( \frac{1}{2}(1 - u) \right)^2 = \frac{1}{2}(1 - u)$ équivaut à $u^2 = 1$. Le reste est trivial.

Un endomorphisme $u$ de $E$ tel que $u^2 = 1$ (qui est alors nécessairement un automorphisme de $E$ égal à son inverse) est appelé une involution. Posons $\varphi = \frac{1}{2}(1 - u)$, $U^- = \varphi(E)$, $U^+ = \varphi^{-1}(0)$ ($= \omega(E)$ en posant $\omega = \frac{1}{2}(1 + u)$); on sait que $E$ est somme directe de $U^+$ et de $U^-$ (chap. VIII, § 1, n° 1), et on a $u(x) = x$ dans $U^+$, $u(x) = -x$ dans $U^-$. Lorsque $A$ est un corps et $E$ de dimension finie, il en résulte, puisque $A$ est de caractéristique $\neq 2$, que les seuls vecteurs propres $\neq 0$ de $u$ sont les éléments ≠ 0 dans U^+ ou dans U^- ; ils correspondent respectivement aux valeurs propres + 1 et -1.

#### Proposition 4 {#alg-ix-s6-prop-4 .statement}

Soit u ∈ GL(E) une involution. Les propriétés suivantes sont équivalentes :
a) u appartient au groupe unitaire associé à Φ ;
b) les sous-modules U^+ = $\frac{1}{2}(1 + u)(E)$ et U^- = $\frac{1}{2}(1 - u)(E)$
sont orthogonaux (et par suite non isotropes).
En outre, si A est un corps et E de dimension finie, les propriétés a) et b) sont équivalentes à :
c) u = u*.
En effet, pour x ∈ U^+ et y ∈ U^-, la relation $\Phi(u(x), u(y)) = \Phi(x, y)$
donne $2\Phi(x, y) = 0$, donc a) entraîne b). Réciproquement on a évidemment $\Phi(u(x), u(y)) = \Phi(x, y)$ lorsque x et y sont tous deux dans U^+ ou tous deux dans U^-, et, vu b), cette relation est encore vraie lorsque l’un d’eux est dans U^+ et l’autre dans U^- ; comme E est somme directe de U^+ et U^-, on voit que b) entraîne a). Enfin, lorsque E est un espace vectoriel de dimension finie, l’adjoint u* est défini puisque Φ est non dégénérée ; la relation a) équivaut à $uu^* = 1$ (§ 1, n° 8, cor. de la prop. 8) ; comme $u^2 = 1$ par hypothèse, a) et c) sont équivalentes.

#### Corollaire 1 {#alg-ix-s6-prop-4-cor-1 .statement}

On suppose que A est un corps et que E est de dimension finie. L’application $u \to \frac{1}{2}(1 + u)(E)$ est une bijection de l’ensemble des involutions u appartenant au groupe unitaire associé à Φ sur l’ensemble des sous-espaces non isotropes de E ; le sous-espace U^+ correspondant à u est l’ensemble des éléments de E invariants par u.

D’après la prop. 4, il suffit de montrer que tout sous-espace non isotrope M de E est l’ensemble des vecteurs invariants par une involution $u \in \mathbf{U}(\Phi)$, et que celle-ci est unique. Or E est somme directe de M et de M^0 (§ 4, n° 1, cor. de la prop. 1), et on a nécessairement $u(x) = x$ pour $x \in M$ et $u(x) = -x$ pour $x \in M^0$ en vertu de la prop. 4 ; ces relations déterminent u de façon unique, et l’endomorphisme u ainsi déterminé répond évidemment à la question (prop. 4).

On dit que l’involution $u$ ainsi déterminée est la symétrie par rapport au sous-espace non isotrope M.

#### Corollaire 2 {#alg-ix-s6-prop-4-cor-2 .statement}

On suppose que $\mathbf{A}$ est un corps et que $\mathbf{E}$ est de dimension finie. Pour qu’un projecteur $\nu$ dans $\mathbf{E}$ soit tel que $\nu(\mathbf{E})$ et $\nu(0)$ soient orthogonaux (et par suite non isotropes), il faut et il suffit que $\nu = \nu^*$.

Il suffit d’appliquer la prop. 4 à l’involution $u = 1 - 2\nu$.

Un projecteur satisfaisant à la condition du corollaire 2 est appelé un projecteur orthogonal pour $\Phi$.

### 4. Symétries dans le groupe orthogonal.

Sauf mention expresse du contraire, on suppose, dans ce no, que $\mathbf{A}$ est un corps commutatif de caractéristique $\neq 2$, et que $\Phi$ est la forme bilinéaire symétrique associée à une forme quadratique Q non dégénérée sur $\mathbf{E}$. Rappelons que l’on a $\Phi(x, x) = 2Q(x)$ pour $x \in \mathbf{E}$ (§ 3, no 4).

Soient H un hyperplan non isotrope dans $\mathbf{E}$, et $u$ la symétrie par rapport à H (no 3). Soit $a \neq 0$ un vecteur orthogonal à H ; on a par hypothèse $u(a) = -a$. Tout vecteur $x \in \mathbf{E}$ s’écrit d’une manière et d’une seule sous la forme $x = \lambda a + y$ avec $\lambda \in \mathbf{A}$ et $y \in \mathbf{H}$; comme $a$ et $y$ sont orthogonaux, on a $\Phi(x, a) = \lambda \Phi(a, a)$, d’où, puisque $a$ est non isotrope (§ 4, no 1, cor. de la prop. 1), $\lambda = \Phi(x, a)\Phi(a, a)^{-1}$. Ceci étant, on a

$$
u(x) = \lambda u(a) + u(y) = -\lambda a + y = x - 2\lambda a,
$$

d’où

$$
u(x) = x - 2\Phi(x, a)\Phi(a, a)^{-1}.a = x - \Phi(x, a)Q(a)^{-1}.a.
$$

On notera que le dernier membre de (6) garde un sens lorsque $\mathbf{A}$ est un corps de caractéristique 2, et $a$ un vecteur non singulier de $\mathbf{E}$; on vérifie aussitôt que l’on a encore alors $Q(u(x)) = Q(x)$ pour tout $x \in \mathbf{E}$, autrement dit $u \in \mathbf{O}(Q)$. On dit encore que l’involution $u$ ainsi définie est la symétrie par rapport à l’hyperplan orthogonal à $a$ (cf. exerc. 28).

#### Proposition 5 {#alg-ix-s6-prop-5 .statement}

On suppose l’espace vectoriel $\mathbf{E}$ de dimension finie n. Le groupe orthogonal $\mathbf{O}(Q)$ associé à $Q$ est alors engendré par les symétries par rapport aux hyperplans non isotropes de $\mathbf{E}$.

La proposition étant évidente pour $n = 0$, nous raisonnons par récurrence sur $n$. Soit $u$ une transformation orthogonale de $E$, et soit $x$ un vecteur non isotrope de $E$ (lemme 1); distinguons trois cas:

a) Supposons d’abord que $u(x) = x$. Alors l’hyperplan $H$ orthogonal à $x$ est non isotrope, et on a $u(H) = H$. La restriction $u'$ de $u$ à $H$ appartient donc au groupe orthogonal $O(Q')$ associé à la restriction $Q'$ de $Q$ à $H$. L’hypothèse de récurrence entraîne, puisque $Q'$ est non dégénérée, que l’on a $u' = v_1' \ldots v_m'$, où $v_i'$ est une symétrie par rapport à un hyperplan $L_i$ de $H$. L’endomorphisme $v_i$ de $E$ qui prolonge $v_i'$ et est tel que $v_i(x) = x$ est alors la symétrie par rapport à l’hyperplan $Ax + L_i$ de $E$. On a évidemment $u = v_1 v_2 \ldots v_m$.

b) Supposons en second lieu que $u(x) = -x$. Si l’on note $s$ la symétrie par rapport à l’hyperplan $H$ orthogonal à $x$, et si l’on pose $v = su$, on a $v(x) = x$, et on est ramené au cas a).

c) Passons enfin au cas général, et posons $y = u(x)$, de sorte que $Q(y) = Q(x)$. Dans ces conditions, les vecteurs $x - y$ et $x + y$ ne peuvent être tous deux isotropes, car, des relations $Q(x - y) = 0$ et $Q(x + y) = 0$, on tirerait, en ajoutant membre à membre, $2(Q(x) + Q(y)) = 0$ ($§ 3$, no 4, déf. 2), d’où $4Q(x) = 0$ contrairement à l’hypothèse. Supposons, par exemple, que $a = x - y$ ne soit pas isotrope ; on a alors

$$
\Phi(y, a) = Q(y + a) - Q(y) - Q(a) = Q(x) - Q(y) - Q(a) = -Q(a);
$$

par suite, si l’on note $s$ la symétrie par rapport à l’hyperplan orthogonal à $a$, la formule (6) prouve que $s(y) = y + a = x$; en posant $v = su$, on a $v(x) = x$, et on est ramené au cas a). Si $a = x - y$ est isotrope et $b = x + y$ non isotrope, on voit de même qu’on est ramené au cas b).

### 5. Groupe des similitudes.

Soit $\Phi$ une forme hermitienne sur $E$. Un automorphisme $u$ du $A$-module $E$ s’appelle une similitude (relativement à $\Phi$) s’il existe un élément inversible $\alpha$ de $A$ tel que l’on ait

$$
\Phi(u(x), u(y)) = \alpha \Phi(x, y)
$$

quels que soient $x, y$ dans $E$. Les similitudes forment un groupe $\Gamma$.

Lorsque $\Phi$ prend des valeurs qui sont des éléments réguliers de $A$ (par exemple lorsque $A$ est un corps et que $\Phi \neq 0$), l’élément $\alpha$ de $A$ vérifiant (7) est déterminé de façon unique par $u$; on l’appelle le *multiplicateur* de la similitude $u$. Changeant $x$ en $\lambda x$ dans (7), on voit alors que $\alpha$ appartient au *centre* de $A$; échangeant $x$ et $y$ dans (7), on voit en outre que $\overline{\alpha} = \alpha$. Si, pour $u \in \Gamma$, on note $\alpha(u)$ le multiplicateur de $u$, l’application $u \to \alpha(u)$ est un homomorphisme de $\Gamma$ dans le groupe multiplicatif des éléments inversibles du centre de $A$. Le noyau de cet homomorphisme est le groupe unitaire associé à $\Phi$, qui est donc un sous-groupe distingué de $\Gamma$. Soient $\beta$ un élément inversible du centre de $A$, $\nu$ l’homothétie de rapport $\beta$, et $\omega$ un automorphisme unitaire de $E$; alors $\nu \omega = \omega \nu$ est une similitude de $E$, et son multiplicateur est $\beta \overline{\beta}$. Réciproquement, soit $u$ une similitude dont le multiplicateur est de la forme $\beta \overline{\beta}$ ($\beta$ désignant un élément inversible du centre de $A$); alors $u \nu^{-1}$ est un automorphisme unitaire $\omega$, donc $u$ est de la forme $\nu \omega$.

Supposons maintenant que $A$ soit un corps, $E$ un espace vectoriel de dimension finie, et que $\Phi$ soit non dégénérée. Pour toute similitude $u$ de multiplicateur $\alpha$ on a
$$
\Phi(x, \alpha y) = \alpha \Phi(x, y) = \Phi(u(x), u(y)) = \Phi(x, u^*(u(y))),
$$
donc $u^* u$ est l’homothétie de rapport $\alpha$. Si $A$ est commutatif, et si $n$ désigne la dimension de $E$, on déduit de là et de la formule (50) du § 1, no 10 que l’on a
$$
(\det u)(\overline{\det u}) = \alpha^n.
$$

Distinguons alors deux cas :
1°) L’entier $n$ est *impair*, soit $n = 2q + 1$. Alors, en posant $\rho = \alpha^{-q} (\det u)$, on a $\alpha = (\det u) (\det u)^{-2q} = \rho \overline{\rho}$. Donc $u$ est le produit de l’homothétie de rapport $\rho$ et d’un automorphisme unitaire.
2°) L’entier $n$ est *pair*, soit $n = 2q$. Alors, en posant $\rho = \alpha^{-q} (\det u)$, on a $\rho \overline{\rho} = 1$. En particulier, lorsque $J$ est l’identité, on a $(\det u)^2 = \alpha(u)^{2q}$; les similitudes $u$ telles que $\det u = \alpha(u)^q$ (resp. $\det u = -\alpha(u)^q$) sont dites *directes* (resp. *inverses*); les similitudes directes forment un sous-groupe distingué d’indice 2 de $\Gamma$;

les homothéties de rapport $\neq 0$ sont des similitudes directes ; il en est de même des transformations orthogonales de déterminant 1 (no 2) ; les transformations orthogonales de déterminant -1 sont des similitudes inverses.

Les définitions et résultats précédents sont encore valables pour les formes $\varepsilon$-hermitiennes ($§ 3$, no 1), et en particulier pour les formes alternées.

Soient A un corps commutatif et Q une forme quadratique $\neq 0$ sur E. On appelle similitude (relativement à Q) tout automorphisme $u$ de E tel qu’il existe un élément non nul $\alpha$ de A (appelé multiplicateur de $u$) pour lequel $Q(u(x)) = \alpha Q(x)$ quel que soit $x \in E$. Il est clair que $u$ est alors une similitude de multiplicateur $\alpha$ relativement à la forme bilinéaire associée à Q ; la réciproque est vraie lorsque la caractéristique de A est $\neq 2$.

### 6. Géométrie hermitienne.

#### Définition 2 {#alg-ix-s6-def-2 .statement}

Soient A un corps, L un espace affine sur A et T l’espace des translations de L (chap. II, 2e éd., App. II). Si T est muni d’une forme hermitienne $\Phi$ non dégénérée, on dit que L est un espace hermitien sur A, et que $\Phi$ est la forme métrique de L.

Si J est l’identité (ce qui implique que A est commutatif), on dit plutôt que L est un espace euclidien.

Si $a$ et $b$ sont deux points de L, posons $e(a, b) = \Phi(b - a, b - a)$. Soit c un troisième point de L. Pour que $b - a$ et $c - a$ soient orthogonaux, il faut, d’après la formule (17) du $§ 1$, no 5, que l’on ait $e(b, c) = e(a, b) + e(a, c)$, et cette condition est suffisante lorsque $J = 1$ et que A n’est pas de caractéristique 2 (« théorème de Pythagore »).

Deux variétés linéaires de L sont dites orthogonales si leurs directions (chap. II, 2e éd., App. II, no 3) sont orthogonales. Une variété linéaire de L est dite isotrope (resp. totalement isotrope) si sa direction est isotrope (resp. totalement isotrope). Un vecteur de T est dit orthogonal à une variété linéaire de L s’il est orthogonal à la direction de cette variété.

Soient V une variété linéaire en L, et $x$ un point de L. L’ensemble des points $y$ de L tels que $y - x$ soit orthogonal à V est une variété linéaire W passant par $x$ ; on dit que W est la variété totalement orthogonale (ou, plus simplement, orthogonale) à V passant par x. Si L est de dimension finie, la dimension de W est égale à la codimension de V. En outre, si V est non isotrope, les directions de V et de W sont supplémentaires (§ 4, no 1, cor. de la prop. 1); alors W rencontre V en un seul point $x_1$; en prenant une origine dans V, on voit aussitôt que, pour V fixé, l’application $x \to x_1$ est une application linéaire affine idempotente ; on l’appelle la projection orthogonale de L sur V ; l’application linéaire qui lui est associée (chap. II, 2e éd., App. II, no 4) est le projecteur orthogonal de T sur la direction de V (no 3).

#### Définition 3 {#alg-ix-s6-def-3 .statement}

Soient L un espace hermitien sur un corps A, T l’espace des translations de L. On appelle déplacement (resp. similitude) de L toute bijection affine u de L sur L telle que l’application linéaire $\varphi$ associée à u dans T (chap. II, 2e éd., App. II, no 4) soit unitaire (resp. soit une similitude).

Le groupe des translations est un sous-groupe distingué du groupe affine ; c’est donc un sous-groupe distingué du groupe des similitudes et du groupe des déplacements. Pour tout $a \in L$, soit $G_a$ le groupe des similitudes (resp. déplacements) laissant a fixe ; si on identifie L à T en prenant a pour origine, $G_a$ est le groupe des similitudes (resp. le groupe unitaire) de T. Toute similitude (resp. déplacement) u se met, d’une façon et d’une seule, sous la forme $u = u_1 t_1$ où $u_1 \in G_a$ et $t_1 \in T$, et aussi sous la forme $u = t_2 u_2$ où $u_2 \in G_a$ et $t_2 \in T$; on a d’ailleurs $u_2 = u_1$ et $t_2 = u_1 t_1 u_1^{-1}$ (chap. II, 2e éd., App. II, no 4).

Soient $u$ une similitude dans L, $\varphi$ la similitude associée dans T. Le multiplicateur de $\varphi$ s’appelle aussi le multiplicateur de $u$ (no 5). Si l’on note $\alpha(u)$ ce multiplicateur, l’application $u \to \alpha(u)$ est un homomorphisme du groupe des similitudes de L dans le groupe multiplicatif des éléments inversibles du centre de A ; son noyau est le groupe des déplacements, qui est donc un sous-groupe distingué du groupe des similitudes. Lorsque A est commutatif et L de dimension finie, il y a, entre le déterminant det $u$ (égal par définition à det $\varphi$) et $\alpha(u)$, les mêmes relations qu’au no 5. Les déplacements $u$ tels que det $u = 1$ forment un sousgroupe distingué du groupe des déplacements ; ce sous-groupe est d’indice 2 si A est un corps commutatif de caractéristique $\neq 2$ et J l’identité.

#### Proposition 6 {#alg-ix-s6-prop-6 .statement}

*Soit L un espace hermitien de dimension finie sur A, dont la forme métrique soit d’indice 0. Toute similitude u de L, de multiplicateur $\mu \neq 1$, admet alors un point fixe et un seul.*

En effet, soit $a$ un point de L. Il existe une similitude $\varphi$ de L laissant $a$ fixe et une translation $t$ de L telles que $u = t \varphi$. Dire que $b$ est un point fixe de $u$ revient à dire que $\varphi(b) - b = t$. Pour montrer que cette équation admet une solution $b$ et une seule, identifions L à son espace des translations T en prenant $a$ pour origine. Il suffit alors de prouver que l’endomorphisme $\varphi - 1$ de T est inversible, autrement dit que la relation $\varphi(x) - x = 0$ ($x \in T$) entraîne $x = 0$. Or, si $\varphi(x) - x = 0$, on a $\Phi(x, x) = \Phi(\varphi(x), \varphi(x)) = \mu \Phi(x, x)$, donc $\Phi(x, x) = 0$ puisque $\mu \neq 1$; ceci entraîne $x = 0$ puisque $\Phi$ est d’indice 0. CQFD.

Supposons que A soit un corps de caractéristique $\neq 2$. Tout déplacement $u$ de L tel que $u^2 = 1$ admet au moins un point fixe, par exemple le milieu $\frac{1}{2}(x + u(x))$ de deux points homologues ; en prenant ce point pour origine, on voit que l’automorphisme unitaire de T associé à $u$ est une symétrie (n° 3). Soit V une variété linéaire non isotrope dans L ; on dit qu’un déplacement $u$ est la *symétrie par rapport à V* si, en prenant une origine dans V, $u$ est identifié à la symétrie par rapport à V de T. Il revient au même de dire que $u(x)$ s’obtient de la façon suivante : en notant $x_1$ la projection orthogonale de $x$ sur V, on a $u(x) - x = 2(x_1 - x)$.

*Exercices.* — 1) On suppose que A est un corps commutatif. Étant donnée une matrice hermitienne $R$ d’ordre $n$ sur A, on appelle *mineurs principaux* d’ordre $r$ de $R$ les mineurs obtenus en supprimant dans $R$ $n - r$ lignes et les $n - r$ colonnes de *mêmes indices*.

a) Si un mineur principal d’ordre $r$ de $R$ n’est pas nul, mais si tous les mineurs principaux d’ordres $r + 1$ et $r + 2$ qui contiennent ce mineur d’ordre $r$ sont nuls, montrer que $R$ est de rang $r$ (cf. chap. III, § 7, exerc. 1 et § 8, exerc. 11 et chap. IV, § 2, exerc. 10). En déduire que, pour que $R$ soit de rang $r$, il faut et il suffit qu’il existe un mineur principal d’ordre $r$ qui soit $\neq 0$, et que tous les mineurs principaux d’ordres $r + 1$ et $r + 2$ soient nuls.

b) Déduire de a) que si $R$ est de rang $r$, il existe une permutation $\sigma \in \mathfrak{S}_n$ telle que, si on effectue sur les lignes et les colonnes de $R$ la même permutation $\sigma$, et si on désigne par $S$ la matrice obtenue, par $\Delta_k$ le mineur principal d’ordre $k$ de $S$ obtenu en supprimant dans $S$ les lignes et les colonnes d’indice $> k$, on ait les deux propriétés suivantes : $1^\circ \Delta_r \neq 0$; $2^\circ$ il n’existe pas d’indice $k < r$ tel que $\Delta_k = \Delta_{k+1} = 0$.

2) On suppose que $A$ est un corps commutatif, et que $E$ est de dimension finie $n$. Soient $\Phi$ une forme sesquilinéaire hermitienne sur $E$, vérifiant la condition (T) du § 4, no 2, $R = (\alpha_{ij})$ la matrice de $\Phi$ par rapport à une base $(e_i)$ de $E$.

a) Si $\Phi$ est de rang $r$, et si le mineur principal (exerc. 1) obtenu en supprimant dans $R$ les lignes et les colonnes d’indices $> r$ n’est pas nul, montrer qu’il existe une nouvelle base $(f_i)$ de $E$ telle que $e_i = f_i$ pour $1 \leq i \leq r$ et que la matrice de $\Phi$ par rapport à $(f_i)$ s’obtienne en remplaçant par 0 dans $R$ tous les $\alpha_{ij}$ tels que $i > r$ ou $j > r$ (considérer le sous-espace $E^0$ orthogonal à $E$).

b) Déduire de a) que si $\Phi$ est de rang $n$, et si le cofacteur $\Delta_{n-1}$ de $\alpha_{nn}$ dans le déterminant $\Delta = \det R$ n’est pas nul, il existe une nouvelle base $(f_i)$ de $E$ telle que $f_i = e_i$ pour $1 \leq i \leq n-1$, et que l’on ait

$$
\Phi(x, y) = \Phi\left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-1} \sum_{j=1}^{n-1} \alpha_{ij} \xi_i \overline{\eta_j} + \frac{\Delta}{\Delta_{n-1}} \xi_n \overline{\eta_n}
$$

(considérer la forme hermitienne dont la matrice par rapport à $(e_i)$ s’obtient en remplaçant $\alpha_{nn}$ par $\alpha_{nn} - \frac{\Delta}{\Delta_{n-1}}$ dans $R$).

c) On suppose que $\Phi$ est de rang $n$, que $\Delta_{n-1} = 0$, mais que le mineur principal $\Delta_{n-2}$ de $R$ obtenu en supprimant les lignes et les colonnes d’indices $n-1$ et $n$ dans $R$ n’est pas nul. Montrer qu’il existe une nouvelle base $(f_i)$ de $E$ telle que $f_i = e_i$ pour $1 \leq i \leq n-2$, et que l’on ait

$$
\Phi(x, y) = \left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-2} \sum_{j=1}^{n-2} \alpha_{ij} \xi_i \overline{\eta_j} + \xi_{n-1} \overline{\eta_n} + \xi_n \overline{\eta_{n-1}}.
$$

(Si $H$ est l’hyperplan engendré par $e_1, \ldots, e_{n-1}$, qui est isotrope, remarquer que la droite orthogonale à $H$ n’est pas dans le sous-espace engendré par $e_1, \ldots, e_{n-2}$, et utiliser la prop. 2 du § 4, no 2).

3) Soient $A$ un corps fini, $E$ un espace vectoriel de dimension finie sur $A$, $\Phi$ une forme sesquilinéaire hermitienne non dégénérée sur $E$, relative à un automorphisme $J \neq 1$ de $A$. Montrer que $E$ admet une base orthonormale pour $\Phi$ (cf. chap. V, § 11, no 5, cor. du th. 3).

4) Soient $A$ un corps fini de caractéristique $\neq 2$, $E$ un espace vectoriel de dimension finie $n$ sur $A$.

a) Montrer que pour toute forme bilinéaire symétrique $\Phi$ non dégénérée sur $E$, il existe une base orthogonale $(e_i)$ de $E$ telle que $\Phi(e_i, e_i) = 1$ pour $1 \leq i \leq n-1$, $\Phi(e_n, e_n) = \Delta$ (discriminant de $\Phi$ par rapport à $(e_i)$). (Remarquer que si $\alpha \beta \neq 0$, l’équation $\alpha \xi^2 + \beta \eta^2 = \gamma$ admet toujours des solutions $(\xi, \eta)$ dans $A$ si $\gamma \neq 0$ (chap. V, § 11, exerc. 4)).

b) Pour que deux formes bilinéaires symétriques non dégénérées sur E soient équivalentes, il faut et il suffit que le rapport de leurs discriminants (par rapport à une même base de E) soit un carré dans A. En déduire que, si n est impair, pour toute forme bilinéaire symétrique $\Phi$ non dégénérée sur E, il existe une base orthogonale par rapport à laquelle la matrice de $\Phi$ est de la forme $\lambda I_n \ (\lambda \in A)$; l’indice de $\Phi$ est alors $(n-1)/2$.

c) Si $n = 2m$ est pair, montrer que l’indice d’une forme bilinéaire symétrique non dégénérée $\Phi$ sur E est m si $(-1)^m \Delta$ est un carré dans A, $m-1$ dans le cas contraire.

5) Soit A un corps commutatif de caractéristique $\neq 2$. Soit I un polynôme à coefficients dans A, par rapport à $n(n+1)/2$ indéterminées $X_{ij} \ (1 \leq i \leq j \leq n)$; pour toute matrice symétrique $R = (\alpha_{ij})$ sur un surcorps commutatif $A'$ de A, on désigne par $I(R)$ l’élément de $A'$ obtenu en substituant $\alpha_{ij}$ à l’indéterminée $X_{ij} \ (i \leq j)$ dans I.

On suppose que I est tel que, pour la matrice $U = (u_{ij})$ avec $u_{ij} = X_{ij}$ pour $i \leq j$, $u_{ij} = X_{ji}$ pour $i > j$ et la matrice carrée $P = (Y_{ij})$ d’ordre n (où les $Y_{ij}$ sont $n^2$ autres indéterminées), on ait

$$
I(PUP) = (\det P)^h I(U)
$$

où h est un entier $> 0$. Montrer que h est pair et que $I(U) = \gamma (\det U)^k$, où $h = 2k$ et $\gamma \in A$. (En utilisant le th. 1, montrer que pour toute matrice symétrique $R$ sur la clôture algébrique $\Omega$ de A, on a $(I(R))^2 = \lambda (\det R)^h$, où $\lambda \in \Omega$, et utiliser le fait que le polynôme $\det U$ par rapport aux $X_{ij}$ n’est pas un carré, en considérant les termes de ce polynôme contenant un $X_{ii}$.

*6) Soient A un corps valué complet non discret, commutatif et de caractéristique $\neq 2$ (Top. gén., chap. IX, § 3, no 2), $\Phi$ une forme hermitienne non dégénérée sur un espace vectoriel E de dimension finie n sur A, $R = (\alpha_{ij})$ la matrice de $\Phi$ par rapport à une base $(e_i)$ de E. Montrer qu’il existe $\varepsilon > 0$ tel que, pour toute matrice hermitienne $R' = (\chi'_{ij})$ vérifiant les conditions $|\alpha'_{ij} - \alpha_{ij}| \leq \varepsilon$ pour tout couple $(i, j)$, la forme $\Phi'$ ayant $R'$ comme matrice par rapport à la base $(e_i)$ soit équivalente à $\Phi$. (Se ramener au cas où $R$ est diagonale ; utiliser l’exerc. 2 b) en s’appuyant sur le lemme suivant : il existe un nombre $a > 0$ tel que pour $|\eta| \leq a$, il existe dans A un élément $\xi$ tel que $\xi^2 = 1 - \eta$. Pour démontrer ce lemme, on utilisera la série du binôme pour $(1-x)^{1/2}$.*

¶ 7) Soient A un corps commutatif non ordonnable (chap. VI, § 2, exerc. 8) de caractéristique $\neq 2$, E un espace vectoriel de dimension finie $n > 0$ sur A, Q une forme quadratique non dégénérée sur E, $(e_i)$ une base orthogonale pour Q, de sorte que $Q \left( \sum_{i=1}^n \xi_i e_i \right) = \sum_{i=1}^n \alpha_i \xi_i^2$. Pour $1 \leq r \leq n$, on pose $Q_r(\xi_1, \ldots, \xi_r) = \sum_{i=1}^r \alpha_i \xi_i^2$, et on désigne par $M_r$ l’ensemble des valeurs de Q_r lorsque les $\xi_i \ (1 \leq i \leq r)$ parcourent A.

a) Montrer que si, pour un indice r, on a $M_r = M_{r+1}$, il en résulte que $M_r = A$ (remarquer que tout élément de A est somme de carrés (chap. VI, § 2, exerc. 7)).

b) On suppose que le sous-groupe S du groupe multiplicatif $A^*$, formé des carrés d’éléments de A, est d’indice fini s dans $A^*$. Déduire de a) que si $n > s$, toute forme quadratique non dégénérée sur E est d’indice $> 0$ (remarquer que tout ensemble $M_r$ est réunion de 0 et de classes mod. S). *Application au cas où A est un corps $p$-adique $\mathbf{Q}_p$ (Top. gén., chap. III, § 5, exerc. 35).*

8) Soient A un corps commutatif de caractéristique $\neq 2$, E un espace vectoriel de dimension finie n sur A, Q une forme quadratique non dégénérée d’indice 0 sur E. Soient $A'$ une extension algébrique de A, de degré fini et impair, $E'$ l’espace vectoriel sur $A'$ obtenu par extension à $A'$ du corps des scalaires de E. Montrer que l’extension $Q'$ de Q à $E'$ ($§ 3$, no 4, prop. 3) est encore d’indice 0. (Se ramener au cas ou $A' = A[X]/(f)$, f étant un polynôme irréductible de degré impair m sur A. Soient $(e_i)$ une base orthogonale de E pour Q, et $\rho_i = Q(e_i)$; montrer que, dans $A[X]$, une relation de la forme $\sum_i \rho_i(g_i(X))^2 = f(X)h(X)$, où les $g_i$ sont des polynômes non tous nuls, de degré $\leq m - 1$, est impossible ; observer pour cela que h serait nécessairement de degré impair, et considérer un facteur irréductible de h, de degré impair).

9) Soient A un corps, E un espace vectoriel sur A admettant une base dénombrable $(e_n)_{n \geq 1}$, $\Phi$ une forme sesquilinéaire hermitienne non dégénérée sur E, satisfaisant à la condition (T) ($§ 4$, no 2).

a) Montrer que si les conditions (C) du th. 1 ne sont pas simultanément vérifiées, il existe dans E une base orthogonale pour $\Phi$ (raisonner comme dans l’exerc. 4 du $§ 5$).

b) On suppose en outre A commutatif, et qu’il existe un entier s tel que sur tout espace vectoriel de dimension finie et $> s$ par rapport à A, toute forme sesquilinéaire hermitienne non dégénérée soit d’indice $> 0$ (cf. exerc. 7). Montrer qu’il existe alors dans E une base orthonormale pour $\Phi$. (Raisonner comme dans a), en observant que pour tout élément de A de la forme $\alpha = \lambda + \overline{\lambda}$, et toute forme hermitienne non dégénérée $\Psi$ sur un espace F de dimension finie $> s$, il existe $z \in F$ tel que $\Psi(z, z) = \alpha$ (cf. $§ 4$, no 2, prop. 4).)

¶ 10) a) Soit A un anneau principal dans lequel il n’y a qu’un seul idéal maximal $A\pi$, tel que 2 ne soit pas divisible par $\pi$ (chap. VII, § 1, exerc. 4). Soit E un module libre sur A, de dimension n. Montrer que toute forme bilinéaire symétrique $\Phi$ sur E admet une base orthogonale. (Soit r le plus grand exposant tel que $\pi^r$ divise tous les éléments $\Phi(x, y)$; montrer qu’il existe $a \in E$ tel que $\Phi(a, a) = \alpha \pi^r$, où $\alpha$ est inversible dans A ; en déduire que E est somme directe de $F = Aa$ et du sous-module $F^0$ orthogonal à F.)

b) Donner un exemple (pour $n = 2$) où $\Phi$ est non dégénérée et où il existe un sous-module F non isotrope de E, de rang 1, admettant un supplémentaire dans E mais tel que $F^0$ ne soit pas supplémentaire de F.

c) Soient $(e_i)$ une base orthogonale pour $\Phi$, et $\alpha_i = \Phi(e_i, e_i)$. Montrer que les idéaux $A\alpha_i$ sont, à l’ordre près, indépendants de la base orthogonale considérée (cf. $§ 5$, th. 1).

On dit que ces idéaux sont les facteurs invariants de la forme $\Phi$. Donner un exemple de deux formes ayant mêmes facteurs invariants et non équivalentes (prendre deux formes dont le quotient des discriminants n’est pas un carré).

d) Soient $F$ un sous-module de $E$, $\Phi_F$ la restriction de $\Phi$ à $F \times F$, $A\alpha_i$ ($1 \leq i \leq r$) les facteurs invariants non nuls de $\Phi$, rangés de sorte que $\alpha_i$ divise $\alpha_{i+1}$, $A\beta_i$ ($1 \leq i \leq s$) les facteurs invariants non nuls de $\Phi_F$, rangés de sorte que $\beta_i$ divise $\beta_{i+1}$. Montrer que l’on a $s \leq r$ et que $\beta_i$ est multiple de $\alpha_i$ pour $1 \leq i \leq s$ (même méthode que dans l’exerc. 1 a) du § 5).

e) On suppose $\Phi$ non dégénérée ; soient $F$, $G$ deux sous-modules non isotropes de $E$ tels que $F^0$ (resp. $G^0$) soit supplémentaire de $F$ (resp. $G$). On suppose que les restrictions de $\Phi$ à $F$ et à $G$ soient équivalentes ; montrer qu’il existe alors un automorphisme $u$ de $E$, laissant invariante $\Phi$, et tel que $u(F) = G$. (En utilisant $a$), se ramener au cas où $F = Aa, G = Ab, \Phi(a, a) = \Phi(b, b)$. Soit $(c_j)$ une base de $G^0$, et soient $b', c'_j$ ($1 \leq j \leq n-1$) les composantes de $b$ et $c_j$ respectivement dans $F^0$; montrer qu’il existe des scalaires $\mu_j$ ($1 \leq j \leq n-1$) tels que les éléments $d_j = c'_j + \mu_j b'$ satisfassent aux relations $\Phi(d_j, d_k) = \Phi(c_j, c_k)$ pour tout couple d’indices ; on remarquera pour cela que pour tout $\lambda \in A$, l’un des éléments $1 \pm \lambda$ est inversible dans $A$.

11) Soit $A$ un anneau principal de caractéristique 0, dans lequel il n’y a qu’un seul idéal principal $\pi$, tel que 2 soit divisible par $\pi$. Si $(e_1, e_2)$ est la base canonique de $E = A^2$, $\Phi$ la forme bilinéaire symétrique sur $E$ définie par $\Phi(\xi_1 e_1 + \xi_2 e_2, \eta_1 e_1 + \eta_2 e_2) = \xi_1 \eta_2 + \xi_2 \eta_1$, montrer qu’il n’existe pas de base orthogonale de $E$ pour $\Phi$.

12) Soient $A$ le corps fini $\mathbf{F}_{q^2}$, $J$ l’automorphisme involutif $\xi \to \xi^q$ de $A$, dont $\mathbf{F}_q$ est le corps des invariants. Si $E$ est un espace vectoriel de dimension $n$ sur $A$, $\Phi$ une forme sesquilinéaire hermitienne (pour $J$) non dégénérée sur $E$, montrer que l’ordre du groupe unitaire $\mathbf{U}(\Phi)$ est égal à
$$
(q^n - (-1)^n) q^{n-1}(q^{n-1} - (-1)^{n-1}) q^{n-2} \ldots (q^2 - 1) q(q + 1)
$$
(méthode analogue à celle de l’exerc. 10 du § 5, en utilisant l’exerc. 3).

13) Soient $A$ le corps fini $\mathbf{F}_q$ ($q$ non multiple de 2), $E$ un espace vectoriel de dimension $n$ sur $A$, $Q$ une forme quadratique non dégénérée sur $E$. Montrer que :
a) Si $n$ est impair, l’ordre du groupe $\mathbf{SO}(Q)$ est
$$
(q^{n-1} - 1) q^{n-2}(q^{n-3} - 1) q^{n-4} \ldots (q^2 - 1) q.
$$
b) Si $n = 2m$ est pair, l’ordre du groupe $\mathbf{SO}(Q)$ est égal à
$$
(q^{2m-1} - \varepsilon q^{m-1}) (q^{2m-2} - 1) q^{2m-3} \ldots (q^2 - 1) q
$$
où $\varepsilon = 1$ si $(-1)^m \Delta$ est un carré dans $A$, $\varepsilon = -1$ dans le cas contraire, $\Delta$ désignant le discriminant de $Q$ par rapport à une base quelconque de $E$. (Méthode analogue à celle de l’exerc. 12, en utilisant l’exerc. 3 du § 6 et l’exerc. 5 du chap. V, § 11.)

14) On suppose que $A$ est un corps commutatif, $E$ un espace vectoriel de dimension finie $n \geqslant 2$ sur $A$, $\Phi$ une forme sesquilinéaire hermitienne non dégénérée sur $E$, satisfaisant à la condition (T) ($§ 4$, no 2). Montrer que les seuls endomorphismes $\omega$ de $E$ permutant avec tous les automorphismes $u$ appartenant au groupe spécial unitaire $\mathbf{SU}(\Phi)$ sont les homothéties, sauf lorsque l’on a simultanément $n = 2$, $J = 1$, $A$ étant de caractéristique $\neq 2$. (Si $n \geqslant 3$, écrire que $\omega$ permute avec les involutions $u \in \mathbf{SU}(\Phi)$, et utiliser l’exerc. 3 du $§ 4$; si $n = 2$ et $J \neq 1$, écrire que $\omega$ permute avec les éléments de $\mathbf{SU}(\Phi)$ dont la matrice est de la forme $\begin{pmatrix} \lambda & 0 \\ 0 & \lambda^{-1} \end{pmatrix}$ par rapport à une base orthogonale de $E$.)

$§ 15$) Soient $A$ un corps commutatif de caractéristique $\neq 2$, $E$ un espace vectoriel de dimension $n \geqslant 1$ sur $A$, $Q$ une forme quadratique non dégénérée sur $E$. Pour tout automorphisme $u \in \mathbf{O}(Q)$, soit $\omega = u - 1$, et soient $r$ le rang de $\omega$, et $W = \overline{\omega}(0)$.

a) Montrer que $\omega(E)$ est le sous-espace $W^0$ orthogonal à $W$.

b) Montrer que si $n = 2, r = 2$, $u$ est produit de deux symétries par rapport à des droites de $E$. (Etablir que si $\omega(x)$ est isotrope pour tout vecteur non isotrope $x \in E$, $\omega(x)$ est isotrope pour tout $x \in E$; on considérera séparément le cas où $A$ a au moins 5 éléments et le cas $A = \mathbf{F}_3$.)

c) On suppose $n$ et $r$ quelconques. Montrer que si $\omega(E)$ n’est pas totalement isotrope, $u$ est produit de $r$ symétries par rapport à des hyperplans de $E$, et ne peut être produit d’un nombre moindre de symétries. (Se ramener au cas où $W$ est totalement isotrope, et procéder par récurrence sur $n$ et $r$. Si $W \neq \{0\}$, montrer qu’il existe un vecteur $a \in W^0$ tel que $\omega(a)$ ne soit pas isotrope, en raisonnant par l’absurde et utilisant le fait qu’un plan dont toutes les droites sauf une au plus sont isotropes est nécessairement totalement isotrope ; prendre alors la symétrie $s$ par rapport à l’hyperplan orthogonal à $\omega(a)$, et considérer l’automorphisme $su$. Si $W = \{0\}$, prendre $a \in E$ tel que $\omega(a)$ ne soit pas isotrope, et, avec la même signification pour $s$, considérer encore l’automorphisme $su$, et utiliser b).)

d) On suppose que $\omega(E)$ soit totalement isotrope. Si $s$ est une symétrie par rapport à un hyperplan non isotrope $H$, montrer que le sous-espace des vecteurs invariants par $su$ est $H \cap W$, donc est de dimension $n - r - 1$, et en déduire que $su$ ne peut être produit de moins de $r + 1$ symétries par rapport à des hyperplans. Déduire alors de c) que $u$ est produit de $r + 2$ symétries par rapport à des hyperplans, mais ne peut être produit d’un nombre moindre de symétries.

e) Déduire de c) et d) que tout automorphisme orthogonal est produit de $n$ symétries au plus par rapport à des hyperplans.

f) Montrer que si $n$ est impair (resp. pair), pour tout automorphisme $u \in \mathbf{O}(Q)$ de déterminant 1 (resp. – 1), il existe un vecteur $x \neq 0$ invariant par $u$ (utiliser e)).

16) Les hypothèses étant les mêmes que dans l’exerc. 15, montrer que, si $n \geqslant 3$, le groupe $\mathbf{SO}(Q)$ est engendré par les symétries par rapport aux sous-espaces non isotropes de $E$ de dimension $n - 2$ (raisonner comme dans la prop. 5 du n° 4).

**¶ 17) Les hypothèses sont les mêmes que dans l’exerc. 15.**

a) Montrer que, pour $n \geqslant 2$, le groupe des commutateurs $\Omega(Q)$ du groupe orthogonal $O(Q)$ est engendré par les éléments $(st)^2$, où $s$ et $t$ parcourent l’ensemble des symétries par rapport à des hyperplans (utiliser la prop. 5 du no 4, et remarquer que pour tout groupe $\Gamma$, le sous-groupe engendré par les carrés des éléments de $\Gamma$ contient le groupe des commutateurs de $\Gamma$).

b) Montrer que si $n \geqslant 3$, le groupe des commutateurs de $SO(Q)$ est engendré par les carrés des éléments de $SO(Q)$ (utiliser l’exerc. 16) ; en déduire que ce groupe est identique à $\Omega(Q)$, et que le groupe quotient $SO(Q)/\Omega(Q)$ est un groupe commutatif dont tous les éléments sont d’ordre 2.

c) On dit qu’un plan $P \subset E$ est *hyperbolique* s’il est non isotrope et s’il contient des droites isotropes (nécessairement au nombre de 2). On dit qu’un automorphisme $u \in O(Q)$ est *hyperbolique* s’il existe un plan hyperbolique $P$ tel que $u(x) = x$ pour tout $x \in P^0$; on dit alors que $u$ est une transformation hyperbolique associée à $P$. Montrer que si $Q$ est d’indice $\geqslant 1$, tout $u \in O(Q)$ est produit de transformations hyperboliques (utiliser la prop. 5 du no 4 et l’exerc. 4 a) du § 4). En déduire que si $P$ est un plan hyperbolique, tout $u \in O(Q)$ peut s’écrire $u = t \varphi$, où $t$ est une transformation hyperbolique associée à $P$ et $\varphi \in \Omega(Q)$.

**¶ 18) Soient A un corps commutatif, E un espace vectoriel de dimension $n$ sur A, $\Phi$ une forme sesquilinéaire hermitienne non dégénérée sur E, satisfaisant à la condition (T) ($§ 4$, no 2). Soient V un sous-espace vectoriel de E, $H_v$ le sous-groupe du groupe unitaire $U(\Phi)$ formé des automorphismes unitaires $u$ tels que $u(V) = V$.

a) Montrer que, lorsque V n’est pas un sous-espace totalement isotrope de dimension $n/2$, l’image de $H_v$ par l’application $u \to \det u$ est le sous-groupe de $A^*$ formé des $\rho \in A$ tels que $\rho \overline{\rho} = 1$.

b) Si $n$ est pair et si V est un sous-espace totalement isotrope de dimension $n/2$, montrer que l’image de $H_v$ par l’application $u \to \det u$ est le sous-groupe de $A^*$ formé des éléments de la forme $\bar{\lambda}/\lambda$ (utiliser la prop. 2 du $§ 4$, no 2).

c) Soient V, W deux sous-espaces vectoriels de E tels que les restrictions de $\Phi$ à V et W soient équivalentes. Montrer qu’il existe $u \in SU(\Phi)$ tel que $u(V) = W$ dans les cas suivants :
  1° J est distinct de l’identité (utiliser le th. 3 du chap. V, § 11, no 5).
  2° $J = 1$, A est de caractéristique $\neq 2$, V et W ne sont pas des sous-espaces totalement isotropes de dimension $n/2$.

d) On suppose que $J = 1$, que A est de caractéristique $\neq 2$, que $n = 2m$ est pair, et que $\Phi$ est une forme bilinéaire symétrique non dégénérée d’indice $m$. Soient V, W deux sous-espaces totalement isotropes de dimension $m$ dans E ; montrer que si $\dim(V \cap W) = q$, pour tout automorphisme orthogonal $u$ tel que $u(V) = W$, on a $\det u = (-1)^{m-q}$ (utiliser b) et la prop. 2 du $§ 4$, no 2). En déduire que l’ensemble des sous-espaces totalement isotropes de dimension $m$ est réunion de deux classes d’intransitivité $N_1, N_2$ pour le groupe $SU(\Phi)$; si V et W sont dans la même classe (resp. dans des classes différentes), la dimension de V ∩ W a même parité que m (resp. n’a pas même parité que m). Pour qu’une similitude u (pour Φ) soit directe, il faut et il suffit que u(N₁) = N₁ (utiliser l’exerc. 4 c) du § 4.

19) Soient A un corps, E un espace vectoriel de dimension finie et > 0 sur A, Φ une forme sesquilinéaire ε-hermitienne sur E, non dégénérée et non alternée. Soit u un automorphisme de E tel que l’on ait

$$
\Phi(u(x), u(x)) = \alpha \Phi(x, x)
$$

pour tout $x \in E$, avec $\alpha \in A$. Montrer que u est une similitude de multiplicateur $\alpha$ sauf lorsque les conditions suivantes sont simultanément vérifiées : A est commutatif et de caractéristique 2, J est l’identité (utiliser l’exerc. 8 du § 1).

20) Soient A un corps, L un espace hermitien de dimension finie sur A ; on suppose que la forme métrique Φ de L satisfasse à la condition (T) (§ 4, no 2). Montrer que si l’indice de Φ est > 0, il peut y avoir des similitudes de L, de multiplicateur $\neq 1$, et qui n’admettent aucun point fixe (utiliser le raisonnement de la prop. 6 du no 6, et la prop. 2 du § 4, no 2).

21) Soient A un corps commutatif de caractéristique $\neq 2$, L un espace euclidien de dimension finie sur A, Φ la forme métrique de L.

a) Montrer que toute bijection u de L sur lui-même, telle que

$$
\Phi(u(x) - u(y), u(x) - u(y)) = \Phi(x - y, x - y)
$$

quels que soient x, y dans L, est un déplacement (utiliser l’exerc. 7 du § 1).

b) Montrer que le groupe des déplacements est engendré par les symétries par rapport aux hyperplans non isotropes de l’espace affine L (en utilisant la prop. 5 du no 4, se ramener à prouver que toute translation non isotrope est produit de deux telles symétries).

22) Dans un espace hermitien L, on dit que deux variétés linéaires sont perpendiculaires si leurs directions sont des sous-espaces faiblement orthogonaux (§ 3, exerc. 11). On suppose L de dimension finie ; soient V₁, V₂ deux variétés linéaires, W₁, W₂ leurs directions respectives. On suppose que $p = \dim(W₁ + W₂) < n$; montrer que si $W₁ + W₂$ n’est pas isotrope, il existe au moins une variété linéaire U de dimension $n - p$, perpendiculaire à V₁ et à V₂, et rencontrant chacune des variétés V₁, V₂ en un seul point ; en outre, si $q = \dim(W₁ \cap W₂)$, la réunion de toutes les variétés linéaires U ayant les propriétés précédentes est une variété linéaire de dimension $n - p + q$.

23) Soient A un corps commutatif de caractéristique $\neq 2$, E un espace vectoriel de dimension finie $n + 1 \geq 2$ sur A, Q une forme quadratique sur E, Φ la forme bilinéaire symétrique associée à Q. L’ensemble C des $x \in E$ tels que $Q(x) = 0$ est appelé le cône isotrope de sommet 0 et d’équation $Q(x) = 0$. S’il n’est pas réduit à 0, l’image S de C – {0} dans l’espace projectif $\mathbf{P}(E)$, par l’application canonique $\pi$ de $E - \{0\}$ sur $\mathbf{P}(E)$ (chap. II, 2e éd., App. III), est appelée *quadrique projective* (resp. *conique projective* si $n = 2$) d’équation homogène $Q(x) = 0$. On dit que S est *dégénérée* si Q est dégénérée. On dit que deux variétés linéaires projectives $V_1, V_2$ de $\mathbf{P}(E)$ sont *conjuguées* par rapport à S si $\overline{\pi}(V_1)$ et $\overline{\pi}(V_2)$ sont orthogonaux (pour $\Phi$). La *polaire* $V^0$ d’une variété linéaire projective $V \subset \mathbf{P}(E)$ par rapport à S est la variété telle que $\overline{\pi}(V^0) \cup \{0\}$ soit le sous-espace totalement orthogonal (pour $\Phi$) à $\overline{\pi}(V) \cup \{0\}$; si V est un hyperplan et si S est non dégénérée, $V^0$ est réduite à un point, appelé *pôle* de V. Une variété linéaire projective V est dite *tangente* à S si $\overline{\pi}(V) \cup \{0\}$ est un sous-espace isotrope (pour $\Phi$).

On suppose dans ce qui suit que S est non vide et non dégénérée.

a) Montrer que l’intersection de S et d’une variété linéaire projective V est vide ou est une quadrique *dans* V ; pour que cette quadrique soit dégénérée, il faut et il suffit que V soit tangente à S.

b) Montrer que l’hyperplan tangent à S en un point $z \in S$ est la réunion des droites passant par z et tangentes à S.

c) On suppose $z \notin S$. Pour toute droite D passant par z et rencontrant S en deux points $a, b$ (distincts ou non), soit $z'$ le *conjugué harmonique* de z par rapport à $a$ et $b$, c’est-à-dire le point de D tel que $\begin{bmatrix} a & b \\ z' & z \end{bmatrix} = -1$ (chap. II, 2e éd., App. III, exerc. 4) ; montrer que $z'$ appartient à l’hyperplan polaire de z par rapport à S, et qu’il existe n de ces points formant une famille projectivement libre dans $\mathbf{P}(E)$ et appartenant à S (cf. § 4, exerc. 4 a)).

d) On suppose que $n = 3$ et que $\Phi$ est d’indice maximum $v = 2$. L’ensemble des droites contenues dans S est alors réunion de deux ensembles $N_1, N_2$ tels que toute droite de $N_1$ rencontre toute droite de $N_2$, mais que deux droites distinctes de $N_1$ (resp. $N_2$) ne se rencontrent pas (exerc. 18 d)). Soient D, D’ deux droites distinctes appartenant à $N_1$; pour tout $z \in D$ il existe une droite $\Delta \in N_2$ et une seule passant par z ; si $u(z)$ est le point où $\Delta$ rencontre D’, montrer que $u$ est une application linéaire projective de D sur D’.

e) Supposant toujours $n = 3$, soient D, D’, D’’ trois droites de $\mathbf{P}(E)$ dont deux quelconques ne se rencontrent pas. Montrer que la réunion des droites rencontrant D, D’ et D’’ est une quadrique non dégénérée.

24) Les hypothèses et notations sont celles de l’exerc. 23, la quadrique S étant supposée non vide et non dégénérée.

a) Montrer que le sous-groupe $\Gamma$ du groupe projectif $\mathbf{PGL}(E)$ formé des bijections linéaires projectives transformant S en elle-même, est l’image canonique du groupe des similitudes relativement à Q. (Utiliser l’exerc. 23 c) ci-dessus, l’exerc. 2 a) du § 4 et l’exerc. 8 du § 1.)

b) Soit $a$ un point de $\mathbf{P}(E)$ n’appartenant pas à S, et soit $\Phi_1$ la restriction de $\Phi$ à l’hyperplan orthogonal à $\overline{\pi}(a)$ dans E. Montrer que le sousgroupe de $\Gamma$ laissant $a$ invariant est isomorphe au quotient du groupe orthogonal $\mathbf{U}(\Phi_1)$ par son centre.

c) Soient $b$ un point de $S$, $F$ l’hyperplan (isotrope) orthogonal à $\overline{\pi}(b)$ dans $E$, $M$ un supplémentaire (non isotrope) de $\overline{\pi}(b)$ par rapport à $F$, et $\Phi_2$ la restriction de $\Phi$ à $M$. Montrer que le sous-groupe de $\Gamma$ laissant $b$ invariant est isomorphe au groupe des similitudes d’un espace euclidien $L$ de dimension $n - 1$, ayant comme forme métrique la forme inverse ($§ 1$, no 7) de $\Phi_2$. (Remarquer que si une similitude pour $\Phi$ transforme la droite $\overline{\pi}(b)$ en elle-même, elle transforme $F$ en lui-même, et est entièrement déterminée par sa restriction à $F$).

25) Soient $A$ un corps commutatif de caractéristique $\neq 2$, $L$ un espace affine de dimension finie $n \geqslant 2$ sur $A$. On identifie $L$ au complémentaire d’un hyperplan projectif $H_0$ (« hyperplan à l’infini ») d’un espace projectif $\mathbf{P}(E)$ de dimension $n$ (chap. II, 2e éd., App. III, no 4). On dit qu’un ensemble non vide $S \subset L$ est une quadrique affine (resp. conique affine si $n = 2$) si $S$ est l’intersection de $L$ et d’une quadrique (resp. conique) projective dans $\mathbf{P}(E)$ (exerc. 23).

a) Montrer que s’il existe une quadrique projective non dégénérée $\overline{S} \subset \mathbf{P}(E)$ telle que $S = L \cap \overline{S}$, cette quadrique est la seule ayant ces propriétés, sauf lorsque $n = 2$, $A = \mathbf{F}_3$ et que $S$ est réduit à 2 éléments (remarquer qu’en dehors de ce cas exceptionnel, pour tout point $z \in H_0$ n’appartenant pas à $\overline{S}$, il existe une droite passant par $z$ et rencontrant $S$ en deux points distincts). On dit alors que $S$ est une quadrique affine non dégénérée. On dit que deux variétés linéaires affines $V_1, V_2$ contenues dans $L$ sont conjuguées par rapport à $S$ si les variétés linéaires projectives $\overline{V}_1, \overline{V}_2$ telles que $V_i = L \cap \overline{V}_i \ (i = 1, 2)$ sont conjuguées par rapport à $\overline{S}$; on définit de même la polaire (lorsqu’elle n’est pas contenue dans $H_0$) où le pôle d’une variété linéaire affine par rapport à $S$, et les variétés linéaires affines tangentes à $S$.

b) On suppose que $S$ est non dégénérée ; montrer qu’on peut prendre une origine $a$ dans $L$ telle qu’en identifiant $L$ de cette façon à un espace vectoriel, il y ait une base $(e_i)$ de $L$ telle que $S$ soit l’ensemble des $x = \sum_{i=1}^n \xi_i e_i$ satisfaisant à une équation de l’une des deux formes

$$
\alpha_1 \xi_1^2 + \cdots + \alpha_n \xi_n^2 = 1 \\
\alpha_1 \xi_1^2 + \cdots + \alpha_{n-1} \xi_{n-1}^2 + \xi_n = 0.
$$

Dans le premier cas, le point $a$ est bien déterminé et est le pôle par rapport à $\overline{S}$ de l’hyperplan à l’infini $H_0$ (appelé centre de $S$). (Distinguer deux cas suivant que $H_0$ est ou non tangent à $\overline{S}$; utiliser le th. 1 du § 6, no 1 et la prop. 2 du § 4, no 2.)

26) Soient $A$ un corps commutatif algébriquement clos de caractéristique $\neq 2$, $E$ un espace vectoriel de dimension finie sur $A$, $Q$ une forme quadratique non dégénérée sur $E$. Soit $u \in \mathbf{O}(Q)$; avec les notations de l’exerc. 12 du § 4, on a $G(p, p) = \{0\}$ sauf pour $p(X) = X - 1$ et $p(X) = X + 1$. Soit $M$ un élément minimal de l’ensemble des sous-espaces non isotropes contenus dans $G(p, p)$ et stables pour $u$, et soit $p^h$ le polynôme minimal de la restriction de $u$ à $M$. Montrer que si $h$ est impair, $M$ est un sous-module indécomposable de $E_u$, et que si $h$ est pair, $M$ est somme directe de deux sous-modules indécomposables isomorphes de $E_u$. (Pour voir que si $h = 2k$ est pair, $M$ ne peut être indécomposable, montrer que $N = p^k(u)(M)$ serait alors totalement isotrope ; si $(e_i)_{1 \leq i \leq 2k}$ est une base de $M$ telle que $u(e_i) = \varepsilon e_i + e_{i+1}$ pour $i \leq 2k - 1$, $u(e_{2k}) = \varepsilon e_{2k}$ (avec $\varepsilon = \pm 1$), montrer que $e_k$ ne peut être orthogonal à $e_{k+1}$, et en déduire que la relation $Q(u(e_k)) = Q(e_k)$ conduit à une contradiction).

27) Soient $A$ un corps commutatif de caractéristique 2, $E$ un espace vectoriel sur $A$, de dimension finie $n$, $Q$ une forme quadratique sur $E$, $\Phi$ la forme bilinéaire associée, qui est alternée, donc de rang pair $2m$ ($§ 5$, no 1, cor. 1 du th. 1).

a) Montrer que si $E^0$ est le sous-espace de $E$ (de dimension $n - 2m$) orthogonal à $E$ pour $\Phi$, on a $Q(\lambda x + \mu y) = \lambda^2 Q(x) + \mu^2 Q(y)$ quels que soient $x, y$ dans $E^0$; autrement dit, la restriction $Q_0$ de $Q$ à $E^0$ est une application semi-linéaire de $E^0$ (considéré comme espace vectoriel sur $A$) dans $A$ (considéré comme espace vectoriel sur le sous-corps $A^2$), relatif à l’isomorphisme $\xi \to \xi^2$ de $A$ sur $A^2$. Soit $q$ la dimension (sur $A$) du noyau $E^0 \cap \overline{Q}(0)$ de $Q$, et soit $E_1$ un supplémentaire de $E^0 \cap \overline{Q}(0)$ par rapport à $E^0$; on a $n - 2m - q \leq [A : A^2]$.

b) Déduire de a) qu’il existe une base $(e_i)_{1 \leq i \leq n}$ de $E$, dont les $2m$ premiers vecteurs forment une base d’un supplémentaire $E_2$ de $E^0$ dans $E$, les $n - 2m - q$ suivants une base de $E_1$, telle que l’on ait, pour $x = \sum_{i=1}^n \xi_i e_i$

$$
Q(x) = \sum_{i=1}^m (\alpha_i \xi_i^2 + \xi_i \xi_{m+i} + \beta_i \xi_{m+i}^2) + \sum_{i=2m+1}^{n-q} \gamma_i \xi_i^2
$$

les $\gamma_i$ ($2m + 1 \leq i \leq n - q$) étant des éléments de $A$ linéairement indépendants par rapport à $A^2$.

c) On appelle indice de $Q$ la dimension maxima des sous-espaces totalement singuliers $V$ de $E$ tels que $V \cap E^0 = \{0\}$. Montrer que si $v$ est l’indice de $Q$, on peut prendre la base $(e_i)$ de $E$ ayant les propriétés énoncées dans b) de sorte que $\alpha_i = \beta_i = 0$ pour $1 \leq i \leq v$ et que la restriction de $Q$ au sous-espace de $E_2$ engendré par $e_{v+1}, \ldots, e_m, e_{m+v+1}, \ldots, e_{2m}$ soit une forme quadratique (non dégénérée) d’indice 0.

d) On suppose $q = 0$; soit $O(Q)$ le groupe des automorphismes de $E$ laissant invariante $Q$. Si $u \in O(Q)$, montrer que $u(x) = x$ pour tout $x \in E^0$. Pour tout $x \in E_2$, soit $u(x) = u_0(x) + u_2(x)$, où $u_0(x) \in E^0$ et $u_2(x) \in E_2$; montrer que $u_2$ appartient au groupe symplectique $Sp(\Phi_2)$ (où $\Phi_2$ est la restriction de $\Phi$ à $E_2$) et que l’on a $Q(u_2(x)) + Q(x) \in Q(E^0)$. Réciproquement, pour tout automorphisme $u_2 \in Sp(\Phi_2)$ tel que $Q(u_2(x)) + Q(x) \in Q(E^0)$ pour tout $x \in E_2$, montrer qu’il existe une application linéaire $u_0$ de $E_2$ dans $E^0$ et une seule telle que l’application linéaire égale à $u_0 + u_2$ dans $E_2$, à l’identité dans $E^0$, appartienne à $\mathbf{O}(Q)$.

e) On suppose que $A$ soit un corps *parfait* ($A^2 = A$) et que $q = 0$. Déduire de b) que tout sous-espace vectoriel de $E$, de dimension $\geqslant 3$, contient au moins un vecteur $x$ tel que $Q(x) = 0$. Si $n$ est *impair*, on a nécessairement $m = \nu$ et $n = 2m + 1$, de sorte qu’il existe une base $(e_i)$ de $E$ par rapport à laquelle on a

$$
Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_m \xi_{2m} + \xi_{2m+1}^2,
$$

et (avec les notations de d)) $\mathbf{O}(Q)$ est isomorphe à $\mathbf{Sp}(\Phi_2)$; toutes les formes quadratiques telles que $q = 0$ sont alors équivalentes. Si $n$ est *pair*, on a nécessairement $n = 2m, \nu = m$ ou $\nu = m - 1$, et il existe une base $(e_i)$ de $E$ par rapport à laquelle on a

$$
(1) \quad Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_{m-1} \xi_{2m-1} + \xi_m \xi_{2m} + \lambda(\xi_m^2 + \xi_{2m}^2)
$$

où $\lambda \in A$. Soit $A_1$ le corps obtenu en adjoignant à $A$ les racines du polynôme $\lambda X^2 + X + \lambda$; montrer que ce corps est indépendant de la base $(e_i)$ par rapport à laquelle $Q$ peut s’écrire sous la forme (1), et que pour que deux formes quadratiques (telles que $q = 0$) soient équivalentes, il faut et il suffit que les extensions quadratiques de $A$ qui leur correspondent de cette façon soient identiques (utiliser le th. de Witt). Cas où $A$ est un corps fini de caractéristique 2.

**¶ 28**) Soient $A$ un corps commutatif de caractéristique 2, distinct de $\mathbf{F}_2$, $E$ un espace vectoriel de dimension $n = 2m$ sur $A$, $Q$ une forme quadratique non dégénérée sur $E$.

a) Montrer que le groupe orthogonal $\mathbf{O}(Q)$ est engendré par les symétries (qui ne sont autres ici que les transvections appartenant à $\mathbf{O}(Q)$ ($§ 4$, exerc. 6)) (raisonner comme dans l’exerc. 11 du $§ 5$). En déduire que le groupe des commutateurs de $\mathbf{O}(Q)$ est engendré par les carrés des éléments de $\mathbf{O}(Q)$ (cf. exerc. 17).

b) On suppose que $Q$ soit d’indice maximum ; soient $V, W$ deux sous-espaces totalement singuliers de $E$ ($§ 4$, no 1) de dimension $m$. Soit $u$ une symétrie $x \to x + \frac{\Phi(x, a)}{Q(a)} a$ ($§ 4$, exerc. 6) ; soit $k$ la dimension de $V \cap W$. Montrer que la dimension de $V \cap u(W)$ est $k + 1$ si $a$ est orthogonal à $V \cap W, k - 1$ dans le cas contraire (dans le premier cas remarquer que $a = x + y$, ou $x \in V, y \in W$, et montrer que $u(y) = x$; dans le second, remarquer que $u$ ne peut laisser invariant aucun vecteur singulier non orthogonal à $a$).

c) On suppose de nouveau que l’indice de $Q$ soit quelconque. Montrer que le sous-groupe $\mathbf{SO}(Q)$ de $\mathbf{O}(Q)$, formé des automorphismes de $E$ qui sont produits d’un nombre *pair* de symétries, est un sous-groupe distingué d’indice 2 de $\mathbf{O}(Q)$. (Montrer que le produit d’un nombre impair de symétries ne peut être l’identité, en considérant l’extension de $Q$ à l’es-

Bourbaki XXIV.

pace vectoriel E' obtenu par extension du corps des scalaires de E à sa clôture algébrique ; utiliser alors b).) (Cf. § 9, exerc. 9.)

d) Si V₁, V₂ sont deux sous-espaces totalement singuliers de E, de même dimension < m, montrer qu’il existe un automorphisme u ∈ SO(Q) tel que u(V₁) = V₂. Au contraire, si V₁ et V₂ sont deux sous-espaces totalement singuliers de dimension m, pour qu’il existe un automorphisme u ∈ SO(Q) tel que u(V₁) = V₂, il faut et il suffit que la dimension de V₁ ∩ V₂ ait même parité que m (raisonner comme dans l’exerc. 18, en utilisant b)).

e) On dit qu’un plan P ⊂ E est hyperbolique s’il est non isotrope et contient des droites singulières (nécessairement au nombre de 2). On dit qu’une transformation u ∈ O(Q) est hyperbolique s’il existe un plan hyperbolique P tel que u(x) = x pour tout x ∈ P⁰ ; on dit alors que u est une transformation hyperbolique associée à P. Montrer que si Q est d’indice > 0, tout u ∈ O(Q) est produit de transformations hyperboliques (utiliser a)). En déduire que si P est un plan hyperbolique, toute transformation u ∈ O(Q) peut s’écrire u = sv, où s est une transformation hyperbolique associée à P et v appartient au groupe des commutateurs de O(Q).

29) Les hypothèses étant celles de l’exerc. 28, on suppose de plus que Q est d’indice maximum m ; soit (eᵢ) une base symplectique de E (pour la forme alternée Φ associée à Q) formée de vecteurs singuliers (§ 4, n° 2, prop. 2), de sorte que la matrice de Φ par rapport à cette base soit la matrice notée R dans l’exerc. 14 du § 5. Avec les notations de ce dernier exercice, montrer que, pour qu’une matrice symplectique (tD + S)⁻¹(D + S) soit la matrice d’un automorphisme u ∈ O(Q), il faut et il suffit que S soit alternée (écrire que tout vecteur u(eᵢ) est singulier, en remarquant que l’on a (tD + S).u(eᵢ) = (D + S).eᵢ).
