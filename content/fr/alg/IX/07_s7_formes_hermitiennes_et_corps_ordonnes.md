---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 7
section_title: Formes hermitiennes et corps ordonnés
lang: fr
source: alg-ix-fr
pdf_pages: 0112-0130
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes positives.
      page: 0
      pdf_page: 113
    - "no": 2
      title: La loi d’inertie.
      page: 0
      pdf_page: 115
    - "no": 3
      title: Réduction d’une forme par rapport à une forme hermitienne positive.
      page: 0
      pdf_page: 116
statements: 42
exercises: 0
content_sha256: 6446758097a7cf0a8decb14d1ea8cad0e94d908cfee02c9a6bd8c910baf27cac
---

## § 7. Formes hermitiennes et corps ordonnés

Dans tout ce paragraphe on désigne par K un corps ordonné maximal (donc commutatif et de caractéristique nulle ; cf. chap. VI, § 2), et on suppose que l’on est dans l’un des trois cas suivants :

1°) A = K, J est l’identité ;
2°) A est le corps K(i), obtenu par adjonction à K d’une racine carrée i de −1, et, pour tout λ ∈ A, $\overline{\lambda}$ est le conjugué de λ (chap. II, § 7, n° 7).
3°) A est le corps des quaternions sur K correspondant au couple (−1, −1) (ou, comme nous dirons pour abréger, le corps des quaternions sur K), et, pour tout λ ∈ A, $\overline{\lambda}$ est le conjugué de λ (cf. chap. II, § 7, n° 8 et chap. VIII, § 11, n° 2).

Si Φ est une forme hermitienne sur E, on a donc, dans tous les cas, $\Phi(x, x) \in K$ pour tout $x \in E$, puisque $\Phi(x, x) = \overline{\Phi(x, x)}$.

### 1. Formes hermitiennes positives.

#### Définition 1 {#alg-ix-s7-def-1 .statement}

Une forme hermitienne $\Phi$ sur $E$ est dite positive (resp. négative) si $\Phi(x, x) \geqslant 0$ (resp. $\Phi(x, x) \leqslant 0$) pour tout $x \in E$.

Lorsque $A = K$, on dit encore que la forme quadratique
$$
Q(x) = \frac{1}{2} \Phi(x, x)
$$
à laquelle est associée $\Phi$ est positive (resp. négative).

Supposons $E$ de dimension finie sur $A$, et soit $(e_i)$ ($i = 1, \ldots, n$) une base orthogonale de $E$ ($\S 6$, no 1, th. 1). Pour qu’une forme hermitienne $\Phi$ sur $E$ soit positive, il faut et il suffit que $\Phi(e_i, e_i) \geqslant 0$ pour $i = 1, \ldots, n$. Soit $\Phi$ une forme hermitienne positive non dégénérée sur $E$; puisque tout élément positif de $K$ est un carré, donc de la forme $\rho \overline{\rho}$ ($\rho \in A$), il existe dans $E$ des bases orthonormales pour $\Phi$ ($\S 6$, no 1, cor. 1 du th. 1).

#### Proposition 1 {#alg-ix-s7-prop-1 .statement}

Supposons $E$ de dimension finie, et $A = K$ ou $A = K(i)$. Si $\Phi$ est une forme hermitienne positive non dégénérée sur $E$, alors les extensions de $\Phi$ à $\bigotimes^p E$ et $\wedge^p E$ ($p > 0$), ainsi que la forme inverse de $\Phi$, sont des formes hermitiennes positives non dégénérées.

Ceci résulte aussitôt de l’existence d’une base orthonormale de $E$, et de la prop. 2, $\S 6$, no 1.

La prop. 1 reste vraie si on y remplace partout « positive non dégénérée » par « positive ».

#### Proposition 2 {#alg-ix-s7-prop-2 .statement}

Soit $\Phi$ une forme hermitienne positive sur $E$. Pour $x, y$ dans $E$, on a
$$
\Phi(x, y) \overline{\Phi(x, y)} \leqslant \Phi(x, x) \Phi(y, y).
$$

L’inégalité est en effet immédiate lorsque les vecteurs $x$ et $y$ sont proportionnels. Supposons donc $x$ et $y$ linéairement indépendants. Soient $A'$ le sous-corps (commutatif) $K(\Phi(x, y))$ de $A$, $F$ le plan vectoriel sur $A'$ engendré par $x$ et $y$, et $\Phi_F$ la restriction de $\Phi$ à $F$; celle-ci prend ses valeurs dans $A'$. D’après la prop. 1, le discriminant de $\Phi_F$ par rapport à la base $(x, y)$ est $\geqslant 0$. Or ce discriminant est $\Phi(x, x)\Phi(y, y) - \Phi(x, y)\overline{\Phi(x, y)}$. CQFD.

#### Corollaire {#alg-ix-s7-n1-cor-1 .statement}

*L’ensemble des vecteurs isotropes de E est le sous-espace $E^0$ orthogonal de E pour $\Phi$. Pour que $\Phi$ soit non dégénérée, il faut et il suffit que l’on ait $\Phi(x, x) > 0$ pour tout $x \neq 0$.

#### Proposition 3 {#alg-ix-s7-prop-3 .statement}

*Supposons E de dimension finie et A commutatif ($\mathbf{A} = \mathbf{K}$ ou $\mathbf{A} = \mathbf{K}(i)$). Soient $\Phi$ une forme hermitienne sur E, X sa matrice par rapport à une base $(x_j)$ ($j = 1, \ldots, n$) de E ; pour toute partie H de $\{1, n\}$, notons $X_{H, H}$ le mineur de X obtenu en supprimant les lignes et les colonnes d’indices $j \notin H$ (chap. III, § 6, no 3).

a) *Si $\Phi$ est positive non dégénérée, on a $X_{H, H} > 0$ pour toute partie H de $\{1, n\}$.

b) *Réciproquement, si, en posant $H_j = \{1, j\}$, on a $X_{H_j, H_j} > 0$ pour $j = 1, \ldots, n$, $\Phi$ est positive non dégénérée.

Supposons d’abord $\Phi$ positive non dégénérée. Les éléments $(x_j)$ ($j \in H$) forment une base d’un sous-espace F de E, et le mineur $X_{H, H}$ est le discriminant de la restriction $\Phi_F$ de $\Phi$ à F par rapport à cette base ; or, comme $\Phi_F(x, x) > 0$ pour tout $x \neq 0$ dans F, $\Phi_F$ est positive non dégénérée (cor. de la prop. 2) ; on a donc $X_{H, H} > 0$ (prop. 1). Pour démontrer b), remarquons que, avec les notations de la prop. 1, § 6, no 1, le mineur $X_{H_j, H_j}$ est égal à $D_{j+1, j+1}$ ; il existe donc (prop. 1, § 6, no 1) une base orthogonale $(e_j)$ ($j = 1, \ldots, n$) de E telle que $\Phi(e_j, e_j) > 0$ pour $j = 1, \ldots, n$ ; par conséquent $\Phi$ est positive non dégénérée.

#### Remarque {#alg-ix-s7-n1-rem-1 .statement}

Il résulte de l’existence de bases orthonormales que deux formes hermitiennes positives non dégénérées sur deux espaces vectoriels de même dimension finie sont *équivalentes* (§ 1, no 6). Soient alors L un espace hermitien de dimension finie sur A, dont la forme métrique est positive non dégénérée, et $V_1$ et $V_2$ deux variétés linéaires de *même dimension* dans L (§ 6, no 6) ; comme les restrictions de la forme métrique aux directions $T_1$ et $T_2$ de $V_1$ et $V_2$ d’une part, aux sous-espaces orthogonaux $T_1^0$ et $T_2^0$ d’autre part, sont équivalentes, il existe un automorphisme unitaire $u$ de l’espace $T$ des translations de $L$ tel que $u(T_1) = T_2$ et $u(T_1^0) = T_2^0$; il existe donc un déplacement $v$ de $L$ tel que $v(V_1) = V_2$. Soient $(a, b), (a', b')$ deux couples de points de $L$; pour qu’il existe un déplacement $v$ de $L$ tel que $v(a) = a'$ et $v(b) = b'$, il faut et il suffit donc (avec la notation du § 6, no 6) que l’on ait $e(a, b) = e(a', b')$; l’élément $\sqrt{e(a, b)}$ de $A$ (chap. VI, § 2, no 4) est appelé la distance de $a$ et $b$ dans l’espace hermitien $L$.

### 2. La loi d’inertie.

#### Théorème 1 (« loi d’inertie ») {#alg-ix-s7-thm-1 .statement}

Supposons que $A$ satisfasse aux hypothèses du début de ce paragraphe, et que $E$ soit de dimension finie $n$. Soit $\Phi$ une forme hermitienne sur $E$. Alors :

a) Il existe une décomposition de $E$ en somme directe du sous-espace $E^0$ orthogonal à $E$, et de deux sous-espaces $E^+$ et $E^-$ tels que la restriction de $\Phi$ à $E^+$ (resp. $E^-$) soit positive (resp. négative) et non dégénérée.

b) Il existe une base orthogonale $(e_i)_{1 \leq i \leq n}$ de $E$ telle que

$$
\Phi\left( \sum_{i=1}^n \xi_i e_i, \sum_{i=1}^n \eta_i e_i \right) = \sum_{i=1}^s \xi_i \overline{\eta_i} - \sum_{i=s+1}^{s+t} \xi_i \overline{\eta_i}.
$$

c) Les dimensions $s$ de $E^+$ et $t$ de $E^-$ sont les mêmes pour toutes les décompositions en somme directe satisfaisant aux conditions énoncées dans a) ; l’entier $s$ (resp. $t$) est le maximum des dimensions des sous-espaces $F$ de $E$ tels que la restriction de $\Phi$ à $F$ soit positive (resp. négative) et non dégénérée.

d) Le rang de $\Phi$ est $s + t$.

e) Si $\Phi$ est non dégénérée, son indice est égal à $\inf(s, t)$ (\S 4, no 2, déf. 2).

Soit, en effet, $(x_i)$ ($i = 1, \ldots, n$) une base orthogonale de $E$ (\S 6, no 1, th. 1); rappelons que l’on a $\Phi(x, x) \in K$ pour tout $x \in E$. On peut supposer que l’on a $\Phi(x_i, x_i) > 0$ pour $i = 1, \ldots, s$, $\Phi(x_i, x_i) < 0$ pour $i = s + 1, \ldots, s + t$ et $\Phi(x_i, x_i) = 0$ pour $i = s + t + 1, \ldots, n$. Ceci démontre a), car on prend pour $E^+$ (resp. $E^-$) le sous-espace engendré par $x_1, \ldots, x_s$ (resp. par $x_{s+1}, \ldots, x_{s+t}$), et $E^0$ est alors engendré par $x_{s+t+1}, \ldots, x_n$. On en déduit b) en remarquant que $\Phi(x_i, x_i)$ est de la forme $\rho \overline{\rho}$ (resp.

- $\rho \bar{\rho} )\ (\rho \in A^*)$ pour $i = 1, \ldots, s$ (resp. $i = s + 1, \ldots, s + t$). Pour démontrer c), considérons un sous-espace P de E tel que la restriction de $\Phi$ à P soit positive et non dégénérée; on a alors $P \cap (E^- + E^0) = \{0\}$, et la somme $P + E^- + E^0$ est donc directe; on en conclut que $\dim P \leq \dim E^+ = s$, et ceci démontre c). L’assertion d) résulte aussitôt de a).

Supposons enfin que $\Phi$ soit non dégénérée, posons $q = \inf (s, t)$, et montrons que q est l’indice de $\Phi$. Avec les notations de b), les vecteurs $e_i + e_{s+i}$ (resp. $e_i - e_{s+i}$) ($i = 1, \ldots, q$) engendrent un sous-espace totalement isotrope F (resp. $F'$). Comme K est de caractéristique 0, $F + F'$ est engendré par $e_1, \ldots, e_q, e_{s+1}, \ldots, e_{s+q}$ et est donc non isotrope. La restriction de $\Phi$ au sous-espace $H = (F + F')^0$ est alors positive (ou négative) et non dégénérée, et H ne contient donc aucun vecteur isotrope $\neq 0$. Comme $F^0$ contient F et H, et que $\dim(F + H) = \operatorname{codim} F' = \operatorname{codim} F$, on a $F^0 = F + H$. Ainsi un vecteur isotrope z orthogonal à F est nécessairement dans F, car, dans la somme directe $F + H$, la composante de z dans H est isotrope. Par conséquent F est un sous-espace totalement isotrope maximal, et ceci démontre e).

#### Définition 2 {#alg-ix-s7-def-2 .statement}

Avec les notations du th. 1, le couple $(s, t)$ s’appelle la signature de $\Phi$.

### 3. Réduction d’une forme par rapport à une forme hermitienne positive.

Dans ce no nous supposerons que E est de dimension finie $n$ sur $A$, et nous noterons $\Phi$ une forme hermitienne positive non dégénérée sur E.

Comme les applications linéaires de E dans $E^*$ associées à $\Phi$ sont bijectives, quels que soient les éléments $x, y, z$ de E avec $y \neq 0$, il existe un élément $t$ de E et un seul tel que $\Phi(x, z) = \overline{\Phi(t, y)}$. En particulier, si $A = K$ ou $A = K(i)$ et si $u$ est une application semi-linéaire pour J de E dans lui-même (chap. II, App. I, no 1), il existe, pour tout $x \in E$, un élément $u^*(x)$ et un seul tel que pour tout $y \in E$, $\Phi(x, u(y)) = \overline{\Phi(u^*(x), y)}$. On voit aussitôt que $u^*$ est une application semi-linéaire pour J de E dans lui-même ; on l’appelle l’adjoint de $u$.

#### Remarque 1 {#alg-ix-s7-n3-rem-1 .statement}

Lorsque J est l’identité, on retrouve la notion d’adjoint d’un homomorphisme définie au § 1, no 8.

#### Remarque 2 {#alg-ix-s7-n3-rem-2 .statement}

Supposons toujours $A = K$ ou $A = K(i)$. Soit $E^J$ le A-module à droite défini au § 1, no 2, déf. 5. La forme $\Phi$ est une forme bilinéaire sur $E \times E^J$, $\Phi^J$ est une forme bilinéaire sur $E^J \times E$, et $u$ est une application A-linéaire de E dans $E^J$. L’adjoint de cet homomorphisme, au sens du § 1, no 8, est une application A-linéaire de E dans $E^J$; on voit aussitôt que celle-ci coïncide avec l’application $u^*$ ci-dessus définie.

On dit qu’un endomorphisme $u$ de E est normal (pour $\Phi$) si l’on a $uu^* = u^*u$.

Exemples d’endomorphismes normaux :
1) les automorphismes unitaires pour $\Phi$ ($\S$ 6, no 2), qui sont caractérisés par la relation $u^{-1} = u^*$ ($\S$ 1, no 8, cor. de la prop. 8);
2) les endomorphismes $u$ tels que $u^* = u$; ceux-ci sont appelés endomorphismes hermitiens.

Pour tout endomorphisme hermitien $u$ de E, posons $\Phi_u(x, y) = \Phi(u(x), y)$; on a
$$
\Phi_u(y, x) = \Phi(u(y), x) = \Phi(y, u(x)) = \overline{\Phi(u(x), y)} = \overline{\Phi_u(x, y)}.
$$
ce qui montre que $\Phi_u$ est une forme hermitienne sur E. Réciproquement soit $\Psi$ une forme hermitienne sur E ; comme l’application $s_\Phi$ de E dans $E^*$ associée à $\Phi$ est bijective, il existe, pour tout $x \in E$, un élément $u(x)$ de E et un seul tel que $\Psi(x, y) = \Phi(u(x), y)$; on vérifie aisément que $u$ est un endomorphisme hermitien de E. Ainsi $u \to \Phi_u$ est une bijection, dite canonique, de l’ensemble des endomorphismes hermitiens de E sur l’ensemble des formes hermitiennes sur E.

Supposons que $A = K$ ou $A = K(i)$; étant donnée une forme bilinéaire $\Psi$ sur E, il existe, pour tout $x \in E$, un élément $u(x)$ de E et un seul tel que $\Psi(x, y) = \overline{\Phi(u(x), y)}$; on voit aussitôt que $u$ est une application semi-linéaire (pour J) de E dans lui-même. Comme $\Phi(u(x), y) = \Phi(y, u(x)) = \overline{\Phi(u^*(y), x)}$, on voit que, pour que $\Psi$ soit symétrique (resp. alternée), il faut et il suffit que l’on ait $u^* = u$ (resp. $u^* = -u$).

#### Théorème 2 {#alg-ix-s7-thm-2 .statement}

Soit S un ensemble d’endomorphismes de E (resp. d’applications semi-linéaires de E dans E lorsque A = K ou A = K(i)) stable pour l’application u → u*. Alors, si V est un sous-espace de E stable pour S, son orthogonal V⁰ est stable pour S. D’autre part E est somme directe de sous-espaces stables pour S, minimaux dans l’ensemble des sous-espaces ≠ {0} et stables pour S, et deux à deux orthogonaux.

Soit en effet V un sous-espace de E stable pour S ; quels que soient x ∈ V⁰, y ∈ V et u ∈ S, on a u*(y) ∈ V, d’où Φ(y, u(x)) = Φ(u*(y), x) = 0 (resp. Φ(y, u(x)) = \overline{\Phi(u^*(y), x)} = 0), et par conséquent u(x) ∈ V⁰ ; ainsi V⁰ est stable pour S, ce qui démontre notre première assertion. Pour la seconde nous procéderons par récurrence sur la dimension n de E, le cas n = 0 étant trivial. Pour n ≠ 0 il existe un sous-espace V ≠ {0} de E stable pour S et minimal, par exemple un sous-espace stable ≠ {0} de dimension minimale. Il suffit alors d’appliquer à V⁰ l’hypothèse de récurrence, puisque l’adjoint de la restriction de u à V⁰ (par rapport à la restriction de Φ) est identique à la restriction à V⁰ de l’adjoint de u.

#### Corollaire 1 {#alg-ix-s7-thm-2-cor-1 .statement}

On suppose que A = K ou que A = K(i). Soit B une sous-algèbre de $\mathcal{L}_A(E)$, stable pour l’application u → u*. Alors E est un B-module semi-simple, et est somme directe de sous-modules simples deux à deux orthogonaux. L’algèbre B est semi-simple.

En effet, comme tout sous-B-module V de E admet un supplémentaire, par exemple V⁰, le B-module V est semi-simple (chap. VIII, § 3, no 3, prop. 7). Comme tout sous-B-module ≠ {0} et minimal de E est simple, E est somme directe de sous-modules simples deux à deux orthogonaux. Enfin B est une algèbre semi-simple, puisqu’elle admet un module semi-simple et fidèle E dont le contremodule est de type fini (chap. VIII, § 5, no 1, prop. 3).

#### Corollaire 2 {#alg-ix-s7-thm-2-cor-2 .statement}

Les hypothèses et notations étant celles du cor. 1, on suppose de plus que l’algèbre B est commutative. Alors tous ses éléments sont des endomorphismes (normaux) semi-simples de E. Lorsque A = K (resp. A = K(i)), E est somme directe de sous-B-modules simples deux à deux orthogonaux, qui sont des espaces vectoriels de dimension 1 ou 2 (resp. 1) sur A.

La première assertion résulte du chap. VIII, § 9, no 1, prop. 2, puisque B est semi-simple. D’autre part tout B-module simple est isomorphe à un B-module de la forme B/m, où m est un idéal maximal de B, donc à un corps commutatif L de degré fini sur A ; lorsque A = K (resp. A = K(i)), le corps L est nécessairement isomorphe à K ou K(i) (resp. K(i)), puisque K(i) est algébriquement clos (chap. VI, § 2, no 6, th. 3).

#### Proposition 4 {#alg-ix-s7-prop-4 .statement}

Soit u un endomorphisme normal de E. Lorsque A est égal à K(i) ou au corps des quaternions sur K, il existe une base orthonormale (pour Φ) de E formée de vecteurs propres de u. Lorsque A = K, u est semi-simple et E est somme directe de sous-espaces stables pour u, deux à deux orthogonaux, et de dimension 1 ou 2.

Examinons d’abord le cas où A est commutatif (A = K ou A = K(i)). Alors la sous-algèbre B = A[u, u*] de $\mathcal{L}_A(E)$ est commutative puisque u est normal ; elle est stable par l’application $\varphi \to \varphi^*$ en vertu des formules (32) et (33) du § 1, no 8. L’assertion relative au cas A = K résulte alors aussitôt du cor. 2 du th. 2. Lorsque A = K(i), ce corollaire montre aussi que E est somme directe de sous-espaces vectoriels $Ax_i$ ($i = 1, \ldots, n$) de dimension 1, deux à deux orthogonaux et stables pour u ; si l’on pose $e_i = (\Phi(x_i, x_i))^{-1/2} x_i$, $(e_i)$ est la base orthonormale cherchée.

Lorsque A est le corps des quaternions sur K, il nous suffira de même de démontrer, en vertu du th. 2, que tout élément minimal de l’ensemble des sous-espaces $\neq \{0\}$ de E stables par u et $u^*$ est de dimension 1. Or un tel sous-espace V contient nécessairement un vecteur propre $x \neq 0$ de u (*), comme on le voit en remarquant que le corps de quaternions A contient K(i) comme sous-corps algébriquement clos, et en restreignant à K(i) le corps des

(*) Si E est un espace vectoriel à gauche sur un corps non commutatif A, et u un endomorphisme de E, on dit encore qu’un vecteur $x \neq 0$ de E est un vecteur propre pour u s’il existe $a \in A$ tel que $u(x) = ax$; le scalaire a est alors appelé valeur propre de u. On notera que, pour tout $b \neq 0$ dans A, le vecteur $bx$ est un vecteur propre pour u, et que la valeur propre correspondante est $bab^{-1}$.

scalaires de V. Il ne reste donc plus qu’à montrer que le vecteur propre x de u est aussi un vecteur propre de u*. Posons $u(x) = ax$ ($a \in A$); on a alors $\Phi(u(x), x) = a\Phi(x, x) = \Phi(x, x)a = \Phi(x, \overline{a}x)$ puisque $\Phi(x, x)$ appartient au centre de A, et d’autre part $\Phi(u(x), x) = \Phi(x, u^*(x))$; il en résulte que l’on a $\Phi(x, u^*(x) - \overline{a}x) = 0$, et on peut donc écrire $u^*(x) = \overline{a}x + z$, où z est un vecteur orthogonal à x. On a donc

$$
\Phi(u^*(x), u^*(x)) = \overline{a}a\Phi(x, x) + \Phi(z, z) = \Phi(u(x), u(x)) + \Phi(z, z).
$$

Or, comme u est normal, on a

$$
\begin{align*}
\Phi(u(x), u(x)) &= \Phi(x, u^*u(x)) = \Phi(x, uu^*(x)) \\
&= \Phi(uu^*(x), x) = \Phi(u^*(x), u^*(x)).
\end{align*}
$$

Par conséquent on a $\Phi(z, z) = 0$, ce qui, par hypothèse, entraîne $z = 0$ et $u^*(x) = \overline{a}x$. CQFD.

#### Remarque {#alg-ix-s7-n3-rem-28 .statement}

Il résulte du th. 2 que les sous-espaces propres relatifs à deux valeurs propres distinctes de u sont orthogonaux.

#### Proposition 5 {#alg-ix-s7-prop-5 .statement}

Soit u un endomorphisme hermitien de E. Les valeurs propres de u appartiennent à K, et il existe une base orthonormale de E formée de vecteurs propres de u.

Lorsque A est égal à K(i) ou au corps des quaternions sur K, il suffit, en vertu de la prop. 4, de démontrer la première assertion ; or, si x est un vecteur propre $\neq 0$ de u et a la valeur propre correspondante, on a, en vertu de l’hypothèse $u = u^*$,

$$
a\Phi(x, x) = \Phi(u(x), x) = \Phi(x, u(x)) = \Phi(x, x)\overline{a} ;
$$

comme $\Phi(x, x)$ est un élément non nul du centre de A, il en résulte que $a = \overline{a}$, donc $a \in K$. Par conséquent une matrice hermitienne a toutes ses valeurs propres dans K. Supposons maintenant que A soit égal à K. La matrice M de u par rapport à une base orthonormale de E est alors symétrique ; c’est donc une matrice hermitienne si on la considère comme une matrice sur K(i). La première partie de la démonstration montre alors que cette matrice a toutes ses valeurs propres dans K, et admet donc, si $E \neq \{0\}$, des vecteurs propres $\neq 0$ dans E. Il en résulte que tout sous-espace stable pour u et minimal est nécessairement de dimension 1, et la conclusion s’ensuit aussitôt, comme dans la prop. 4.

#### Proposition 6 {#alg-ix-s7-prop-6 .statement}

a) Soit $\Psi$ une forme hermitienne (resp. bilinéaire symétrique si $\mathbf{A} = \mathbf{K}$ ou $\mathbf{A} = \mathbf{K}(i)$) sur $E$. Il existe une base de $E$ qui est orthonormale pour $\Phi$ et orthogonale pour $\Psi$.

b) Supposons $\mathbf{A} = \mathbf{K}$ ou $\mathbf{A} = \mathbf{K}(i)$, et soit $\Psi$ une forme bilinéaire alternée sur $E$. Il existe une base de $E$ qui est orthonormale pour $\Phi$ et par rapport à laquelle la matrice de $\Psi$ est de la forme

$$
\begin{pmatrix}
0 & a_1 & 0 & 0 \ldots 0 \\
-a_1 & 0 & 0 & 0 \ldots 0 \\
0 & 0 & 0 & a_2 \ldots 0 \\
0 & 0 & -a_2 & 0 \ldots 0 \\
\cdots & \cdots & \cdots & \cdots
\end{pmatrix}.
$$

où les $a_i$ sont $\geqslant 0$ dans $K$.

Lorsque $\Psi$ est hermitienne, notre assertion résulte aussitôt de la prop. 5 et de la correspondance canonique entre formes hermitiennes sur $E$ et endomorphismes hermitiens pour $\Phi$. Dans les deux autres cas, soit $u$ l’application semi-linéaire de $E$ dans lui-même définie au début de ce n° par la formule $\Psi(x, y) = \overline{\Phi(u(x), y)}$. Alors $u^2$ est une application $\mathbf{A}$-linéaire ; lorsque $\Psi$ est symétrique (resp. alternée), on a $u = u^*$ (resp. $u = -u^*$), donc $u^2$ est hermitien ; d’où aussi

$$
\Phi(u^2(x), x) = \overline{\Phi(x, u^2(x))} = \Phi(u^*(x), u(x)) = \Phi(u(x), u(x))
$$
(resp. $-\Phi(u(x), u(x))$);

ceci montre que la forme hermitienne $(x, y) \to \Phi(u^2(x), y)$ est positive (resp. négative). Appliquons alors le th. 2, et soit $V$ un élément minimal de la famille des sous-espaces $\neq \{0\}$ de $E$ stables pour $u$ et pour $u^*$. Comme $u^2$ est un endomorphisme hermitien, $V$ contient un vecteur propre $x \neq 0$ de $u^2$; posons $u^2(x) = ax$, où $a \in \mathbf{K}$ (prop. 5).

Lorsque $\Psi$ est symétrique, l’inégalité $\Phi(u^2(x), x) \geqslant 0$ montre que l’on a $a \geqslant 0$. Posons $y = a^{1/2}x + u(x)$; on a $u(y) = a^{1/2}u(x) + ax = a^{1/2}y$, et $Ay$ est stable pour $u$ et $u^* = u$. Si $y = 0$, $Ax$ est stable pour $u$ et $u^*$; en tous cas, $V$ est un sous-espace de dimension 1, et notre conclusion résulte aussitôt du th. 2.

Lorsque $\Psi$ est alternée, on a $a \leqslant 0$; posons

$$
y = (-a)^{1/2}x + u(x), \quad z = (-a)^{1/2}x - u(x).
$$

On a $u(y) = -(-a)^{1/2}z, \ u(z) = (-a)^{1/2}y$ et
$$
\Phi(y, z) = -a\Phi(x, x) - \Phi(u(x), u(x)) = -\Phi(ax, x) + \Phi(u^2(x), x) = 0.
$$

Si $y = z = 0$, on a $a = 0$ et $u(x) = 0$, donc $Ax$ est stable pour $u$ et $u^*$, $V$ est de dimension 1, et la matrice de la restriction de $\Psi$ à $V$ est nulle puisque $\Psi$ est alternée. Sinon, $y$ et $z$ sont tous deux $\neq 0$, ils engendrent $V$, et comme ils sont orthogonaux, $V$ est de dimension 2 et la matrice de la restriction de $\Psi$ à $V$ est de la forme $\begin{pmatrix} 0 & b \\ -b & 0 \end{pmatrix}$. Enfin, en vertu de la formule $\Psi'(x', y') = \overline{\Phi(u(x'), y')}$, on a $\Psi'(x', y') = 0$ lorsque $x'$ et $y'$ appartiennent à deux sous-espaces stables par $u$ et orthogonaux pour $\Phi$. Ceci démontre l’existence d’une base orthonormale de $E$ (pour $\Phi$) par rapport à laquelle la matrice de $\Psi$ a la forme indiquée. CQFD.

Exercices. — 1) On suppose vérifiées les hypothèses du début du § 7 ; soit $\Phi$ une forme hermitienne positive sur $E$.

a) Pour que l’on ait $\Phi(x, x)\Phi(y, y) = \Phi(x, y)\overline{\Phi(x, y)}$, il faut et il suffit que $x$ et $y$ soient linéairement dépendants ou que le plan engendré par $x$ et $y$ soit isotrope.

b) On suppose que, pour tout $x \in E$, $\Phi(x, x)$ soit un carré dans $K$. Montrer que pour deux vecteurs quelconques $x, y$ de $E$, on a
$$
\sqrt{\Phi(x + y, x + y)} \leq \sqrt{\Phi(x, x)} + \sqrt{\Phi(y, y)}.
$$

Si $\Phi$ est non dégénérée, les deux membres de cette inégalité ne peuvent être égaux que si $\alpha x + \beta y = 0$, où $\alpha$ et $\beta$ sont deux éléments de $K$, non tous deux nuls et tels que $\alpha \beta \leq 0$.

2) On suppose $A = K$ ou $A = K(i)$. Soit $X$ une matrice carrée hermitienne d’ordre $n$ sur $A$, telle que pour toute partie non vide $H$ de $\{1, n\}$, on ait $X_{H, H} \geq 0$ (notations de la prop. 3 du no 1).

a) Soit $\lambda$ un élément $> 0$ de $K$; montrer que la matrice $X + \lambda I$ est positive non dégénérée (utiliser la prop. 3 du no 1, en raisonnant par récurrence sur $n$).

b) En déduire que la matrice hermitienne $X$ est positive.

#### Remarque 3 {#alg-ix-s7-n3-rem-3 .statement}

On suppose que $A = K$ ou $A = K(i)$ et que $E$ est de dimension finie. Soient $\Phi_1, \Phi_2$ deux formes hermitiennes positives sur $E$, et soient $V = (\alpha_{ij}), W = (\beta_{ij})$ les matrices de ces formes par rapport à une même base $(e_i)$ de $E$. Montrer que la forme hermitienne $\Phi$ dont la matrice $(\gamma_{ij})$ par rapport à $(e_i)$ est telle que $\gamma_{ij} = \alpha_{ij}\beta_{ij}$ pour tout couple d’indices, est positive ; en outre, si $\Phi_1$ et $\Phi_2$ sont non dégénérées, il en est de même de $\Phi$. (Dans le calcul de $\Phi(x, x)$, exprimer les $\alpha_{ij}$ à l’aide des valeurs $\Phi_1(c_i, c_i)$ pour une base orthogonale $(c_i)$ de $E$ relative à $\Phi_1$.)

#### Remarque 4 {#alg-ix-s7-n3-rem-4 .statement}

On suppose que $A = K$ ou $A = K(i)$. Soit $R$ une matrice hermitienne d’ordre $n$ sur $A$; on dit que $R$ a pour signature $(s, t)$ si la forme hermitienne sur $A^n$ ayant $R$ pour matrice par rapport à la base canonique, a pour signature $(s, t)$. On désigne par $\Delta_k$ le mineur principal de $R$ obtenu en supprimant dans $R$ les lignes et les colonnes d’indice $> k$; on suppose que $\Delta_{s+t} \neq 0$ et que, pour aucun indice $k < s + t$, $\Delta_k$ et $\Delta_{k+1}$ ne soient simultanément nuls (cf. § 6, exerc. 1 b)). Montrer que si $\Delta_k = 0$ pour un $k < s + t$, $\Delta_{k-1}$ et $\Delta_{k+1}$ ont des signes opposés (méthode de l’exerc. 1 a) du § 6) et que le nombre $s - t$ est égal à

$$
\operatorname{sgn} \Delta_1 + \operatorname{sgn} (\Delta_1 \Delta_2) + \cdots + \operatorname{sgn} (\Delta_{s+t-1} \Delta_{s+t})
$$

(utiliser l’exerc. 2 du § 6).

#### Remarque 5 {#alg-ix-s7-n3-rem-5 .statement}

On suppose que $A = K$ ou $A = K(i)$; soient $R, S$ deux matrices hermitiennes sur $A$, de signatures $(s, t)$ et $(s', t')$ respectivement (exerc. 4); montrer que la matrice $R \otimes S$ est une matrice hermitienne de signature $(ss' + tt', st' + s't)$.

#### Remarque 6 {#alg-ix-s7-n3-rem-6 .statement}

Soient $K$ un corps ordonné maximal, $L$ une algèbre simple de rang fini sur $K$. Si $(s, t)$ est la signature de la forme bilinéaire symétrique $(x, y) \to \operatorname{Tr}_{L/K}(xy)$ sur $L$, montrer que l’on a :
$s - t = m$ si $L$ est isomorphe à une algèbre de matrices d’ordre $m$ sur $K$;
$s - t = 0$ si $L$ est isomorphe à une algèbre de matrices sur le corps $K(i)$;
$s - t = -2m$ si $L$ est isomorphe à une algèbre de matrices d’ordre $m$ sur le corps des quaternions sur $K$.

#### Remarque 7 {#alg-ix-s7-n3-rem-7 .statement}

On suppose que $A$ satisfait aux conditions du début du § 7 et que $E$ est de dimension finie $n$. Soit $\Phi$ une forme hermitienne positive non dégénérée sur $E$.
a) Montrer que toute similitude pour $\Phi$ s’écrit d’une seule manière comme produit d’une homothétie de rapport $\geqslant 0$ dans $K$, et d’une transformation unitaire.
b) Pour toute base $(a_i)_{1 \leq i \leq n}$ de $E$, montrer qu’il existe une base orthonormale et une seule $(e_i)_{1 \leq i \leq n}$ de $E$ satisfaisant aux conditions suivantes : 1° pour tout $m$ tel que $1 \leq m \leq n$, le sous-espace engendré par $a_1, \ldots, a_m$ est identique au sous-espace engendré par $e_1, \ldots, e_m$; 2° on a $\Phi(a_i, e_i) \geq 0$ dans $K$, pour tout indice $i$ (cf. § 6, no 1, prop. 1).
c) Déduire de b) que pour toute matrice carrée inversible $M$ d’ordre $n$ sur $A$, il existe un couple de matrices $(L, U)$ d’ordre $n$ et un seul, tel que $U$ soit une matrice unitaire, que $L = (\lambda_{ij})$ n’ait que des zéros au-dessous de sa diagonale et des termes diagonaux $\lambda_{ii}$ appartenant à $K$ et $> 0$, et enfin que $M = LU$.

#### Remarque 8 {#alg-ix-s7-n3-rem-8 .statement}

On suppose $A = K$; soit $L$ un espace hermitien de dimension finie sur $A$, dont la forme métrique est positive non dégénérée. Soient $M, N$ deux parties de $L$, $u$ une bijection de $M$ sur $N$ telle que l’on ait $e(u(a), u(b)) = e(a, b)$ quels que soient les points $a, b$ de $M$. Montrer qu’il existe un déplacement dont la restriction à $M$ soit égale à $u$ (raisonner par récurrence sur la dimension de la variété linéaire affine engendrée par $M$, comme dans le procédé d’orthogonalisation de Gram-Schmidt). La proposition s’étend-elle au cas où A est égal à K(i) ou au corps des quaternions sur K ?

#### Remarque 9 {#alg-ix-s7-n3-rem-9 .statement}

On suppose remplies les conditions du n° 3, et en outre que A est le corps des quaternions sur K. Soit u un endomorphisme normal de E. Montrer que E est somme directe de sous-espaces F_k (1 \leq k \leq r), deux à deux orthogonaux, tels que dans chacun des F_k il existe une base orthonormale (e_{ik}) (1 \leq i \leq n_k) et que l’on ait u(e_{ik}) = \lambda_k e_{ik} pour 1 \leq i \leq n_k, deux \lambda_k d’indices distincts n’étant pas transformés l’un de l’autre par un automorphisme intérieur de A. En outre, si (F'_k) est une seconde décomposition de E ayant les mêmes propriétés, avec un système (\lambda'_k) de valeurs propres, on a F'_k = F_k (à une permutation près des indices) et \lambda'_k = \alpha_k \lambda_k \alpha_k^{-1}; l’ensemble des vecteurs propres de u pour la valeur propre \lambda_k est le sous-espace sur le commutant A_k de \lambda_k dans A, engendré par les e_{ik} (1 \leq i \leq n_k).

#### Remarque 10 {#alg-ix-s7-n3-rem-10 .statement}

On suppose remplies les conditions du n° 3, et en outre que A est égal à K(i) ou au corps des quaternions sur K. Soit u un endomorphisme normal de E.

a) Montrer que pour qu’un sous-espace vectoriel F de E soit tel que u(F) \subset F, il faut et il suffit que F soit engendré par des vecteurs propres de u ; on a alors u(F^0) \subset F^0 et u^*(F) \subset F.

b) Pour que u soit unitaire (resp. pour que u^* = u, u^* = -u), il faut et il suffit que pour toute valeur propre \lambda de u, on ait \lambda \overline{\lambda} = 1 (resp. \overline{\lambda} = \lambda, \overline{\lambda} = -\lambda).

c) On dit qu’un endomorphisme hermitien u de E est positif (resp. positif et non dégénéré) si la forme hermitienne (x, y) \to \Phi(u(x), y) qui lui correspond canoniquement est positive (resp. positive et non dégénérée) ; il faut et il suffit pour cela que toutes les valeurs propres de u soient \geq 0 (resp. > 0).

d) Montrer que pour tout entier m > 0, il existe un endomorphisme normal v de E tel que v^m = u. Si u est hermitien positif, il existe un seul endomorphisme hermitien positif v tel que v^m = u, et il existe un polynôme f \in K[X] tel que v = f(u) ; ce dernier résultat est aussi valable lorsque A = K.

#### Remarque 11 {#alg-ix-s7-n3-rem-11 .statement}

On suppose remplies les conditions du n° 3, et en outre que A = K. Soit u un endomorphisme normal de E.

a) Soit V un élément minimal de l’ensemble des sous-espaces de E non réduits à 0, stables pour u et u* ; montrer que si V est de dimension 2, la restriction de u à V est une similitude directe de multiplicateur > 0.

b) Montrer que tout sous-espace de E stable pour u est aussi stable pour u*. (Soit E_0 l’espace vectoriel obtenu à partir de E par extension à K(i) du corps des scalaires ; \Phi est la restriction à E d’une forme hermitienne positive non dégénérée sur E_0 et u la restriction à E d’un endomorphisme normal u_0 de E_0 (pour cette forme) ; en outre E est l’ensemble des x \in E_0 invariants par une bijection semi-linéaire involutive j de E_0, et on a u_0j = ju_0. Appliquer alors l’exerc. 10 a.).

#### Remarque 12 {#alg-ix-s7-n3-rem-12 .statement}

On suppose remplies les conditions du n° 3, et en outre que A est égal à K(i) ou au corps des quaternions sur K. Montrer que pour tout endomorphisme $u$ de $E$, il existe une base orthonormale de $E$ par rapport à laquelle la matrice de $u$ n’ait que des zéros au-dessous de la diagonale. (Procéder par récurrence sur la dimension de $E$, en considérant un vecteur propre de $u$.)

#### Remarque 13 {#alg-ix-s7-n3-rem-13 .statement}

Soient $A$ un corps vérifiant les conditions du début du § 7, $E, F$ deux espaces vectoriels de dimension finie sur $A$, $\Phi$ (resp. $\Psi$) une forme hermitienne positive non dégénérée sur $E$ (resp. $F$). Montrer que, pour toute application linéaire $u$ de $E$ dans $F$, l’adjoint $u^*$ de $u$ (pour $\Phi$ et $\Psi$; cf. § 1, no 8) est tel que $u^*u$ et $uu^*$ soient des endomorphismes hermitiens positifs (exerc. 10 c)) de $E$ et $F$ respectivement.

#### Remarque 14 {#alg-ix-s7-n3-rem-14 .statement}

On suppose remplies les conditions du no 3. Soient $u$ un endomorphisme de $E$, $h_1, h_2$ les deux endomorphismes hermitiens positifs de $E$, tels que l’on ait $h_1^2 = u^*u, h_2^2 = uu^*$ (exerc. 13 et 10 d)).

a) Montrer qu’il existe un endomorphisme unitaire $\nu$ tel que $u = \nu h_1 = h_2 \nu$ et en particulier que $h_1$ et $h_2$ sont semblables (remarquer que $u(0) = \overline{h_1}(0)$ et que si $V$ est le sous-espace orthogonal à $\overline{u}(0)$, on a $\Phi(u(x), u(x)) = \Phi(h_1(x), h_1(x))$ pour tout $x \in V$. Pour que $\nu$ soit déterminé de façon unique, il faut et il suffit que $u$ soit bijective. Pour qu’on puisse prendre $\nu$ permutable avec $h_1$, il faut et il suffit que $u$ soit normal.

b) Déduire de a) que toute matrice carrée $M$ d’ordre $n$ sur $A$ peut s’écrire $UDV$, où $U$ et $V$ sont des matrices unitaires et $D$ une matrice diagonale dont les éléments sont $\geqslant 0$, et ont pour carrés les valeurs propres de $MM^*$.

#### Remarque 15 {#alg-ix-s7-n3-rem-15 .statement}

On suppose remplies les conditions du no 3. Montrer que toute matrice hermitienne positive $H$ sur $A$ peut s’écrire sous la forme $LL^*$, où $L = (\lambda_{ij})$ n’a que des zéros au-dessous de sa diagonale et des termes diagonaux appartenant à $K$ et $\geqslant 0$; en outre $L$ est déterminée de manière unique par ces conditions lorsque $H$ est inversible (cf. exerc. 10 d) et 7 c)).

#### Remarque 16 {#alg-ix-s7-n3-rem-16 .statement}

On suppose remplies les conditions du no 3 et en outre que $A = K(i)$. Soit $u$ un endomorphisme de $E$.

a) L’ensemble des valeurs propres de $u$ est contenu dans l’ensemble $U$ des valeurs de $\Phi(x, u(x))$ lorsque $x$ parcourt l’ensemble des éléments de $E$ tels que $\Phi(x, x) = 1$.

b) On dit qu’une partie $C$ de $A = K(i)$ est convexe si, pour tout couple d’éléments $(\xi, \eta) \in C^2$ et tout $\tau \in K$ tel que $0 \leqslant \tau \leqslant 1$ on a $\tau \xi + (1-\tau)\eta \in C$. Montrer que l’ensemble $U$ est convexe. (Se ramener au cas où $n = 2$; en écrivant $u$ sous la forme $\nu + i\omega$, où $\nu$ et $\omega$ sont hermitiens, et en remplaçant au besoin $u$ par $\lambda u$, où $\lambda \in A$ et $\lambda \overline{\lambda} = 1$, montrer que tout revient à prouver la propriété suivante. Soient $f(\xi_1, \xi_2) = \xi_1 \overline{\xi}_1 + \xi_2 \overline{\xi}_2$, $g(\xi_1, \xi_2) = a \xi_1 \overline{\xi}_1 + b \xi_2 \overline{\xi}_2$ ($a \in K, b \in K$), $h(\xi_1, \xi_2) = \alpha \xi_1 \overline{\xi}_1 + \beta \xi_1 \overline{\xi}_2 + \beta \xi_2 \overline{\xi}_1 + \gamma \xi_2 \overline{\xi}_2$ ($\alpha \in K, \gamma \in K, \beta \in A$); soient $(\eta_1, \eta_2) \in A^2, (\zeta_1, \zeta_2) \in A^2$ tels que $f(\eta_1, \eta_2) = f(\zeta_1, \zeta_2) = 1$, $g(\eta_1, \eta_2) = g(\zeta_1, \zeta_2) = 1$, $h(\eta_1, \eta_2) > 0$, $h(\zeta_1, \zeta_2) < 0$; il existe alors $(\theta_1, \theta_2) \in A^2$ tel que $f(\theta_1, \theta_2) = 1$, $g(\theta_1, \theta_2) = 1$ et $h(\theta_1, \theta_2) = 0$. On commencera par remarquer que pour tout couple $(\xi_1, \xi_2)$, il existe $\mu \in A$ tel que $\mu \overline{\mu} = 1$ et $\beta \mu \xi_1 \overline{\xi}_2 + \beta \mu \xi_2 \overline{\xi}_1 = 0$, ce qui permettra de se ramener au cas où $\beta = 0$; utiliser la prop. 5 du chap. VI, § 2, no 5.)

c) Montrer que si $u$ est normal, U est le plus petit ensemble convexe contenant toutes les valeurs propres de $u$. Donner un exemple où $u$ n’est pas normal mais où U possède encore la propriété précédente. (Prendre pour valeurs propres de $u$ les éléments $\pm 1 \pm i$ comme valeurs propres simples, et 0 comme valeur propre double.)

#### Remarque 17 {#alg-ix-s7-n3-rem-17 .statement}

On suppose remplies les conditions du n° 3 ; pour tout $\xi \in A$, on désigne par $|\xi|$ l’élément $\rho \geqslant 0$ de K tel que $\rho^2 = \xi \overline{\xi}$ (valeur absolue de $\xi$). Pour toute matrice carrée $M = (\alpha_{ij})$ sur A, on pose $f(M) = \max_i |\alpha_{ii}|$, $g(M) = \max_{i,j} |\alpha_{ij}|$, et on désigne par $\varphi(M)$ la plus grande valeur absolue des valeurs propres de $M$ (on montrera que cette définition a un sens lorsque A est le corps des quaternions sur K).

a) Soient $A, B, D$ trois matrices carrées d’ordre $n$ sur A. Montrer que si $D$ est diagonale, on a

$$
g^2(ADB^*) \leq f^2(D)f(AA^*)f(BB^*)
$$
(utiliser l’inégalité (1) du n° 1). En déduire que
$$
g(ABB^*A^*) \leq f(AA^*)\varphi(BB^*)
$$
(appliquer la prop. 5 à la matrice hermitienne $BB^*$). En déduire que, pour $m$ matrices carrées arbitraires $A_i$ ($1 \leq i \leq m$) sur A, on a
$$
g^2(A_1A_2\ldots A_m) \leq f(A_1A_1^*)\varphi(A_2A_2^*)\ldots\varphi(A_{m-1}A_{m-1}^*)f(A_m^*A_m)
$$
$$
\varphi^2(A_1A_2\ldots A_m) \leq \varphi(A_1A_1^*)\varphi(A_2A_2^*)\ldots\varphi(A_mA_m^*)
$$
$$
g^2(A_1A_2\ldots A_m) \leq \varphi(A_1A_1^*)\ldots\varphi(A_mA_m^*).
$$
(Pour (3), raisonner par récurrence à partir de (2). Pour (4), utiliser l’exerc. 12 ; déduire enfin (5) de (3).)

Montrer que l’inégalité (3) ne subsiste plus nécessairement lorsque l’on y remplace $A_m^*A_m$ par $A_mA_m^*$ (observer que l’on peut avoir $f(A^*A) \neq f(AA^*)$), ou lorsqu’on remplace $\varphi(A_iA_i^*)$ par $f(A_iA_i^*)$ pour $2 \leq i \leq m-1$ (prendre tous les $A_i$ égaux à la matrice carrée dont tous les éléments sont 1).

b) Soit $u$ un endomorphisme normal de E ; si $\lambda$ est valeur propre de $u$ (élément de $K(i)$ lorsque $A = K$), $\overline{\lambda}$ est une valeur propre de $u^*u$. Pour toute matrice normale $M$ (matrice d’un endomorphisme normal de E par rapport à une base orthonormale), on a donc $\varphi^2(M) = \varphi(MM^*)$. En déduire que l’on a aussi $g(M) \leq \varphi(M)$, et plus généralement, si $M_1, \ldots, M_m$ sont normales,
$$
g(M_1\ldots M_m) \leq \varphi(M_1)\ldots\varphi(M_m)
$$
$$
\varphi(M_1\ldots M_m) \leq \varphi(M_1)\ldots\varphi(M_m)
$$
(utiliser (4) et (5)).

c) Montrer que si $H$ est une matrice hermitienne positive sur A, on a $f(H) = g(H) \leq \varphi(H)$ (utiliser (3) et b), en écrivant $H = AA^*$.

#### Remarque 18 {#alg-ix-s7-n3-rem-18 .statement}

On suppose remplies les conditions du n° 3.**

a) Pour tout endomorphisme $u$ de $E$, soit $(e_i)$ une base orthonormale de $E$ formée de vecteurs propres de $u^*u$, et soit $\rho_i$ la valeur propre de $u^*u$ correspondant au vecteur $e_i$; on pose $s(u) = (\sum_{i=1}^n \rho_i)^{1/2}$ (racine carrée de $\operatorname{Tr}(u^*u)$ lorsque $A$ est commutatif); on a $s(u^*) = s(u)$. Si $u, v$ sont deux endomorphismes de $E$, $U, V$ leurs matrices par rapport à une même base orthonormale de $E$, montrer que pour la matrice $UV^* + VU^*$, à éléments dans $K$, on a $(\operatorname{Tr}(UV^* + VU^*))^2 \leq 4s(u)s(v)$ (remarquer que $(u^* + \lambda v^*)(u + \lambda v)$ est hermitien positif pour tout $\lambda \in K$); en déduire que $s(u + v) \leq s(u) + s(v)$. Si en outre $A$ est commutatif, on a

$$
|\operatorname{Tr}(uv)|^2 \leq s(u)s(v) \quad \text{et} \quad |\operatorname{Tr}(u)| \leq \sqrt{n}s(u)
$$

(écrire $u$ comme un produit en utilisant l’exerc. 14 b)).

b) On suppose en outre $A$ commutatif (donc égal à $K$ ou $K(i)$). Si $H_1, H_2$ sont deux matrices carrées hermitiennes positives, montrer que l’on a $\operatorname{Tr}(H_1H_2) \geq 0$ (se ramener au cas où $H_2$ est une matrice diagonale). En déduire que l’on a (notations de l’exerc. 17)

$$
|\operatorname{Tr}(H_1H_2)| \leq \varphi(H_1)\operatorname{Tr}(H_2) \leq \operatorname{Tr}(H_1)\operatorname{Tr}(H_2).
$$

Conclure de ces inégalités que pour deux endomorphismes quelconques $u, v$ de $E$, on a alors $s(uv) \leq s(u)s(v)$.

c) Supposant toujours $A$ commutatif, soit $\prod_{i=1}^n (x - \lambda_i)$ la décomposition en facteurs linéaires du polynôme caractéristique d’un endomorphisme quelconque $u$ de $E$; montrer que l’on a $\sum_{i=1}^n |\lambda_i|^2 \leq (s(u))^2$ et que, pour que les deux membres de cette inégalité soient égaux, il faut et il suffit que $u$ soit normal (utiliser l’exerc. 12).

#### Remarque 19 {#alg-ix-s7-n3-rem-19 .statement}

On suppose remplies les conditions du n° 3. Soit $M$ une matrice carrée d’ordre $n$ sur $A$; montrer que pour toute sous-matrice carrée $N$ de $M$ (obtenue en supprimant dans $M$ un certain nombre de lignes et les colonnes de mêmes indices que ces lignes), on a (notations de l’exerc. 17) $\varphi^2(N) \leq \varphi(MM^*)$ (appliquer convenablement la formule (4) de l’exerc. 17). Si en particulier $M$ est une matrice normale, $\varphi(N) \leq \varphi(M)$ (cf. exerc. 17 b)).

#### Remarque 20 {#alg-ix-s7-n3-rem-20 .statement}

On suppose remplies les conditions du n° 3 et en outre que $A$ est égal à $K$ ou à $K(i)$. Appliquer les résultats des exerc. 17 à 19 à l’extension de $\Phi$ aux $p$-èmes puissances extérieures (\$ 1, n° 9) et aux puissances extérieures $p$-èmes des endomorphismes ou matrices considérés. En particulier, montrer que, si $\prod_{i=1}^n (X - \lambda_i)$ et $\prod_{i=1}^n (X - \rho_i^2)$ sont les décompositions en facteurs linéaires des polynômes caractéristiques d’un endomorphisme $u$ de $E$ et de l’endomorphisme $u^*u$, et si on suppose $|\lambda_i| \geqslant |\lambda_{i+1}|$ et $\rho_i \geqslant \rho_{i+1} \geqslant 0$ pour $1 \leqslant i \leqslant n-1$, on a
$$
|\lambda_1 \lambda_2 \ldots \lambda_h| \leqslant \rho_1 \rho_2 \ldots \rho_h
$$
pour $1 \leqslant h \leqslant n-1$ et $|\lambda_1 \lambda_2 \ldots \lambda_n| = \rho_1 \rho_2 \ldots \rho_n$.

#### Remarque 21 {#alg-ix-s7-n3-rem-21 .statement}

On suppose remplies les conditions du no 3. Soit $u$ un endomorphisme hermitien de $E$ et soit $\prod_{i=1}^n (X-\lambda_i)$ la décomposition en facteurs linéaires de son polynôme caractéristique ; on suppose $\lambda_i \geqslant \lambda_{i+1}$ pour $1 \leqslant i \leqslant n-1$.

a) Montrer que la plus grande (resp. la plus petite) des valeurs propres $\lambda_i$ dans $K$ est égale à la plus grande (resp. la plus petite) des valeurs de $\Phi(u(x), x)$ lorsque $x$ parcourt l’ensemble des $x \in E$ tels que $\Phi(x, x) = 1$. (Raisonner directement, ou appliquer l’exerc. 16 c) en se ramenant au cas où $A = K(i)$ ($\S 3$, exerc. 4).)

b) Soit $\Psi_v$ la restriction à un sous-espace vectoriel $V$ de $E$ de la forme hermitienne $\Psi'$ associée à $u$, et soit $u_v$ l’endomorphisme hermitien de $V$ associé à $\Psi_v$. Montrer que $\lambda_k$ est la plus petite des plus grandes valeurs propres des $u_v$, lorsque $V$ parcourt l’ensemble des sous-espaces vectoriels de $E$, de dimension $n-k+1$ (utiliser la prop. 5).

#### Remarque 22 {#alg-ix-s7-n3-rem-22 .statement}

On suppose remplies les conditions du no 3, et en outre que $A$ est égal à $K(i)$ ou au corps des quaternions sur $K$. Soient $u, v$ deux endomorphismes normaux de $E$; soit $(E_i)_{1 \leqslant i \leqslant r}$ (resp. $(F_j)_{1 \leqslant j \leqslant s}$) la décomposition de $E$ en somme directe de sous-espaces deux à deux orthogonaux, tels que dans $E_i$ (resp. $F_j$) il y ait une base orthonormale formée de vecteurs propres de $u$ (resp. $v$) pour une même valeur propre $\lambda_i$ (resp. $\mu_j$), et que $\lambda_h$ et $\lambda_i$ (resp. $\mu_j$ et $\mu_k$) ne soient pas transformés l’un de l’autre par un automorphisme intérieur de $A$ si $h \neq i$ (resp. $j \neq k$) (cf. prop. 4 et exerc. 9). Pour qu’un endomorphisme $w$ de $E$ soit tel que $uw = vw$, il faut et il suffit que pour tout $j$ ($1 \leqslant j \leqslant s$), $w(F_j)$ soit contenu dans un des $E_i$ et que l’image par $w$ de tout vecteur propre de $v$ relatif à la valeur propre $\mu_j$ soit un vecteur propre de $u$ relatif à la valeur propre $\mu_j$ (ce qui implique en particulier que $\mu_j$ et $\lambda_i$ sont transformés l’un de l’autre par un automorphisme intérieur de $A$). En déduire que s’il en est ainsi, on a alors $u^*w = wv^*$.

#### Remarque 23 {#alg-ix-s7-n3-rem-23 .statement}

On suppose remplies les conditions du no 3. Soient $u$ et $v$ deux endomorphismes de $E$.

a) On suppose $u$ et $uv$ normaux. Pour que $vu$ soit normal, il faut et il suffit que $v$ et $u^*u$ soient permutables. (Pour voir que la condition est nécessaire, utiliser la relation $u(vu) = (uv)u$ et l’exerc. 22 ; pour voir qu’elle est suffisante, utiliser les exerc. 14 a) et 10 d).)

b) On suppose $u, v$ et $uv$ normaux ; soit $\beta$ la plus grande valeur propre de $uu^*$, et soit $F$ le sous-espace de $E$ formé des vecteurs propres de $uu^*$ relatifs à la valeur propre $\beta$. Montrer que $v(F) \subset F$. (Remarquer que pour tout endomorphisme normal $u$ et tout $x \in E$, on a
$$
\Phi(u(x), u(x)) = \Phi(u^*(x), u^*(x)).
$$)

Se ramener au cas où A est égal à K(i) ou au corps des quaternions sur K ; F admet alors une base formée de vecteurs propres pour u (et u*) ; remarquer que pour un tel vecteur z, on a $\Phi(u^*u v(z), v(z)) = \beta \Phi(v(z), v(z))$. En déduire que $\nu u$ est normal (raisonner par récurrence sur le nombre des valeurs propres distinctes de $u^*u$). Si h (resp. $h'$) est l’endomorphisme hermitien positif tel que $h^2 = uu^*$ (resp. $h'^2 = \nu \nu^*$) et si on pose $u = hu_1, \nu = h'\nu_1$, où $u_1$ et $\nu_1$ sont unitaires, h permutable à $u_1$ et $h'$ à $\nu_1$ (exerc. 14 a)), montrer que les couples $(h, h'), (h, \nu_1)$ et $(h', u_1)$ sont permutables ; réciproque. En déduire que $u^m \nu^n, \nu^n u^m, u \nu^*$ et $\nu^* u$ sont alors normaux ($m$ et $n$ entiers $> 0$ arbitraires).

#### Remarque 24 {#alg-ix-s7-n3-rem-24 .statement}

On suppose remplies les conditions du n° 3. Soit $\Gamma$ un groupe d’automorphismes de E tel que tout $u \in \Gamma$ soit normal. Montrer qu’il existe une décomposition de E en somme directe de sous-espaces $E_k$ ($1 \leq k \leq r$) deux à deux orthogonaux, tels que la restriction à $E_k$ de tout $u \in \Gamma$ soit de la forme $\lambda_k \nu_k$, où $\lambda_k$ est un élément $> 0$ de K et où $\nu_k$ est un endomorphisme unitaire de $E_k$ (décomposer chaque $u \in \Gamma$ sous la forme $h \nu$, où $\nu$ est unitaire, $h$ hermitien positif et $h^2 = uu^*$ (exerc. 14 a)) ; utiliser l’exerc. 23 b) et appliquer le cor. 2 du th. 2 à l’algèbre engendrée par les endomorphismes hermitiens $h$ correspondant aux $u \in \Gamma$. En déduire que si $\Gamma$ est fini, les éléments $u \in \Gamma$ sont unitaires.

#### Remarque 25 {#alg-ix-s7-n3-rem-25 .statement}

On suppose que $A = K$ (corps ordonné maximal). Soit L un espace euclidien de dimension $n$ sur A, dont la forme métrique est positive non dégénérée.

Soit S une quadrique affine non dégénérée dans L (§ 6, exerc. 25). Si S admet un centre $a$ et si on prend $a$ pour origine dans L, montrer qu’il existe une base orthonormale $(e_i)$ pour L telle que, par rapport à cette base, S ait pour équation $\lambda_1 \xi_1^2 + \cdots + \lambda_n \xi_n^2 = 1$. En outre, si deux bases orthonormales ont cette propriété, les éléments $\lambda_i \in K$ qui leur correspondent sont les mêmes à l’ordre près.

Si S n’admet pas de centre, montrer qu’il existe un point $b$ de S et ($b$ étant pris pour origine) une base orthonormale pour L telle que, par rapport à cette base, S ait pour équation $\lambda_1 \xi_1^2 + \cdots + \lambda_{n-1} \xi_{n-1}^2 + \xi_n = 0$. (Si $\overline{S}$ est la quadrique projective telle que $S = L \cap \overline{S}$, c le pôle (à l’infini) par rapport à $\overline{S}$ de l’hyperplan à l’infini $H_0$, déterminer $b$ par la condition que la droite passant par $b$ et $c$ soit perpendiculaire à l’hyperplan tangent à S au point $b$).

#### Remarque 26 {#alg-ix-s7-n3-rem-26 .statement}

a) Soient K un corps commutatif, S une partie de K telle que K soit un corps S-ordonnable maximal (chap. VI, § 2, exerc. 8). Soient $f$ un polynôme de $K[X]$, L son corps des racines. Montrer que si, pour toute structure d’ordre (total) sur K compatible avec sa structure d’anneau, L admet une structure d’extension ordonnée de K, on a nécessairement $L = K$. (Raisonner par l’absurde : en procédant comme dans l’exerc. 8 e) du chap. VI, § 2, se ramener au cas où on aurait $[L : K] = 2$. Conclure en remarquant que si $b \in K$ n’est pas un carré, il existe une structure d’ordre total sur K, compatible avec sa structure d’anneau, et pour laquelle $b < 0$ (cf. chap. VI, § 2, n° 3, lemme du th. 1)).

b) Etendre les résultats du n° 3 (la prop. 6 exceptée) au cas où K est un corps S-ordonnable maximal (*). (Commencer par démontrer l’analogue de la prop. 5, en utilisant a). Etablir ensuite l’analogue du cor. 2 du th. 2 pour le cas où l’algèbre commutative B est formée d’endomorphismes hermitiens, en utilisant la prop. 10 du chap. VIII, § 9, n° 4. Passer au cas d’un endomorphisme normal u pour A = K(i) en remarquant qu’on peut alors écrire $u = v + i w$, où v et w sont hermitiens et permutables. Enfin, si A est le corps des quaternions sur K, E_0 l’espace E considéré comme espace vectoriel de dimension 2n sur K(i), et si on pose $\Phi(x, y) = \Phi_1(x, y) + \Phi_2(x, y)i$, où $\Phi_1$ et $\Phi_2$ prennent leurs valeurs dans K(i), remarquer que si u est normal pour $\Phi$, il est aussi normal pour $\Phi_1$.)

#### Remarque 27 {#alg-ix-s7-n3-rem-27 .statement}

Soient K un corps ordonné maximal, E un espace vectoriel de dimension n sur K, $\Phi$ une forme bilinéaire symétrique non dégénérée sur E, de signature (s, t) distincte de (n, 0) et de (0, n). Soit $(e_i)$ une base orthogonale pour $\Phi$, telle que $\Phi(e_i, e_i) = 1$ pour $1 \leq i \leq s$, $\Phi(e_i, e_i) = -1$ pour $s+1 \leq i \leq n$. Pour toute transformation orthogonale $u \in \mathbf{U}(\Phi)$, soit

$$
U = \begin{pmatrix} M & N \\ P & Q \end{pmatrix}
$$

la matrice de u par rapport à $(e_i)$, écrite sous forme d’un tableau carré de matrices correspondant à la partition de $(1, n)$ en $(1, s)$ et $(s+1, n)$.

a) Démontrer les relations

$$
\begin{align*}
{}^tM \cdot M - {}^tP \cdot P &= I_s \\
{}^tQ \cdot Q - {}^tN \cdot N &= I_t \\
{}^tM \cdot N - {}^tP \cdot Q &= 0.
\end{align*}
$$

b) Soit R une matrice sur K à t lignes et s colonnes, telle que $I_s - {}^tR \cdot R$ soit la matrice d’une forme hermitienne (sur $K^s$) positive et non dégénérée. Montrer que $\det(M + \lambda NR)$ ne change pas de signe pour $-1 \leq \lambda \leq 1$ dans K (montrer, en utilisant a), que ${}^t(M + \lambda NR)(M + \lambda NR)$ est la matrice d’une forme symétrique positive non dégénérée).

c) On pose $\sigma(u) = \sigma(U) = \operatorname{sgn}(\det M)$; montrer que, pour deux éléments quelconques $u, v$ du groupe orthogonal $\mathbf{U}(\Phi)$, on a $\sigma(uv) = \sigma(u)\sigma(v)$ (utiliser a) et b)). En déduire que le groupe des commutateurs du groupe spécial orthogonal $\mathbf{SU}(\Phi)$ est distinct de $\mathbf{SU}(\Phi)$ (cf. § 10, exerc. 9).
