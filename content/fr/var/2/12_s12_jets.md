---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 12
section_title: Jets
lang: fr
source: var-fr
pdf_pages: 0143-0151
extraction: ocr
subsections:
    - "no": 1
      title: Jets d’applications
      page: 0
      pdf_page: 143
    - "no": 2
      title: Jets d’applications d’espaces de Banach
      page: 0
      pdf_page: 144
    - "no": 3
      title: Variétés de jets
      page: 0
      pdf_page: 144
    - "no": 4
      title: Repères et fibrations principales
      page: 0
      pdf_page: 146
    - "no": 5
      title: Jets de sections
      page: 0
      pdf_page: 147
    - "no": 6
      title: Jets de sections d’un fibré vectoriel
      page: 0
      pdf_page: 148
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 150
statements: 1
exercises: 0
content_sha256: 3cef1d15729f7411300863edad308e8143c54cc5db300a69be7628ab5c76eb0f
---

## § 12. Jets

Dans ce paragraphe, on note $X$ et $Y$ deux variétés de classe $C^r$, où $r \in \mathbf{N}_k$, et $k$ un entier tel que $0 \leq k \leq r$.

A partir du no 12.3, on suppose:

— soit que $K$ est de caractéristique zéro;

— soit que les variétés, espaces de Banach et fibrés vectoriels considérés sont localement de dimension finie.

### 12.1. Jets d’applications

### 12.1.1. Soit $x \in X$ et soient $f, g$ deux applications continues définies au voisinage de $x$ et à valeurs dans $Y$. On dit que $f$ et $g$ ont un contact d’ordre $\geq k$ en $x$ si l’on a $f(x)=g(x)$ et s’il existe des cartes $(U,\varphi,E)$ de $X$ en $x$ et $(V,\psi,F)$ de $Y$ en $f(x)$ telles que les applications $\psi \circ f \circ \varphi^{-1}$ et $\psi \circ g \circ \varphi^{-1}$, définies au voisinage de $\varphi(x)$ dans $E$ et à valeurs dans $F$, aient un contact d’ordre $\geq k$ en $\varphi(x)$ (1.1.2). Cette propriété est alors vérifiée par toutes les cartes de $X$ en $x$ et de $Y$ en $f(x)$.

### 12.1.2. Soient $x \in X$, $y \in Y$. Dans l’ensemble des applications de classe $C^r$ définies au voisinage de $x$, à valeurs dans $Y$, et appliquant $x$ sur $y$, la relation « $f$ et $g$ ont un contact d’ordre $\geq k$ » est une relation d’équivalence; la classe de $f$ pour cette relation se note $j^k_x(f)$ et s’appelle le jet d’ordre $k$ de $f$ de source $x$ et de but $y$. La source d’un jet est notée $s(j)$ et son but $b(j)$.

L’ensemble des jets d’ordre $k$ de $X$ dans $Y$ (resp. de source $x$, resp. de but $y$) est noté $J^k(X,Y)$ (resp. $J^k_x(X,Y)$, resp. $J^k(X,Y)_y$) et l’on pose

$$
J^k(X,Y)_y^x = J^k_x(X,Y) \cap J^k(X,Y)_y.
$$

### 12.1.3. Si $U$ et $V$ sont des ouverts de $X$ et $Y$ respectivement, on identifie de façon évidente $J^k(U,V)$ à l’image réciproque de $U \times V$ par l’application

$$
(s,b): J^k(X,Y) \longrightarrow X \times Y.
$$

### 12.1.4. Soit $Z$ une variété de classe $C^r$, et soit $(x,y,z) \in X \times Y \times Z$. Soit $j \in J^k(X,Y)_y$ et soit $j' \in J^k(Y,Z)_z$. Les applications $f' \circ f$, avec $f \in j$ et $f' \in j'$, ont même jet d’ordre $k$ en $x$; ce jet s’appelle le composé de $j$ et $j'$ et se note $j' \circ j$; on a $s(j' \circ j)=s(j)$ et $b(j' \circ j)=b(j')$. Si $T$ est une variété de classe $C^r$ et si $j'' \in J^k_z(Z,T)$, on a

$$
j'' \circ (j' \circ j)=(j'' \circ j')\circ j.
$$

12.1.5. Soit $j \in J_x^k(X, Y)$, avec $x \in X$, et soit $k'$ un entier tel que $0 \leq k' \leq k$. Les jets $j_x^{k'}(f)$, pour $f \in j$, sont égaux; le jet ainsi défini est noté $r^{k', k}(j)$; l’application $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ est surjective.

12.1.6. Supposons $r$ égal à $\infty$ ou à $\omega$. Soient $f$ et $g$ deux applications de classe $C^r$ définies au voisinage d’un point $x \in X$, et à valeurs dans $Y$. Si $j_x^m(f) = j_x^m(g)$ pour tout entier $m \geq 0$, on dit que $f$ et $g$ ont un contact d’ordre infini en $x$. On obtient ainsi une relation d’équivalence dont les classes s’appellent les jets d’ordre infini en $x$; le jet d’ordre infini de $f$ se note $j_x^\infty(f)$ ou $j_x^\omega(f)$. Les définitions et résultats qui précèdent s’étendent sans modification aux jets d’ordre infini.

### 12.2. Jets d’applications d’espaces de Banach

Dans ce n°, E et F désignent deux espaces de Banach. Si $m$ est un entier $\geq 0$, on note $P_m(E; F)$ l’espace de Banach des polynômes-continus homogènes de degré $m$ sur E à valeurs dans F (1ère partie, Appendice, A.2).

12.2.1. Soit U un ouvert de E, soit $f : U \to F$ une application de classe $C^r$, et soit $a \in U$. Il existe un polynôme-continu
$$
\tilde{f} = f_0 + \cdots + f_k \quad (\text{avec } f_m \in P_m(E; F))
$$
et un seul, qui soit de degré $\leq k$, et qui ait même jet d’ordre $k$ à l’origine que $x \mapsto f(x - a)$. Si $0 \leq m \leq k$, la $m$-ième composante $f_m$ de $\tilde{f}$ est notée $\Delta^m f(a)$ ou $\Delta_a^m(f)$. Lorsque $r = \omega$, cette notation coïncide avec celle de 3.2.1 et 4.2.1; lorsque $r \leq \infty$, on a
$$
m! \Delta^m f(a)(h) = D^m f(a)(h, \ldots, h) = D^m f(a) . h^m.
$$
L’application $f \mapsto \tilde{f}$ définit par passage au quotient une bijection de $J_a^k(E, F)$ sur $\prod_{0 \leq m \leq k} P_m(E; F)$ au moyen de laquelle on identifie ces deux espaces; en particulier, $J_a^k(E, F)$ est muni d’une structure d’espace de Banach sur K. Si $j \in J_a^k(E, F)$, on note $\Delta_a^m(j)$ la $m$-ième composante de $j$; on a
$$
\Delta_a^m(j) \in P_m(E; F) \quad \text{pour} \quad 0 \leq m \leq k, \quad \text{et} \quad \Delta_a^0(j) = b(j) \in F.
$$

12.2.2. Soit U (resp. V) un ouvert de E (resp. F). Notons $Q^k(E, F)$ l’espace de Banach produit des $P_m(E; F)$ pour $1 \leq m \leq k$. L’application
$$
j \mapsto (s(j), b(j), \Delta_{s(j)}^1(j), \ldots, \Delta_{s(j)}^k(j))
$$
est une bijection de $J^k(U, V)$ sur $U \times V \times Q^k(E, F)$, au moyen de laquelle on identifie ces deux ensembles. En particulier, $J_0^k(E, F)_0$ s’identifie à $Q^k(E, F)$.

### 12.3. Variétés de jets

12.3.1. Soient $c = (U, \varphi, E)$ et $c' = (V, \psi, F)$ des cartes de X et Y respectivement. Les applications $\varphi$ et $\psi$ définissent, par transport de structure, une bijection $\pi$ de $J^k(U, V)$ sur
$$
J^k(\varphi(U), \psi(V)) = \varphi(U) \times \psi(V) \times Q^k(E, F),
$$
cf. 12.2.2. Si l’on pose $W = J^k(U, V)$ et $G = E \times F \times Q^k(E, F)$, le triplet $(W, \pi, G)$ est une carte de $J^k(X, Y)$. Les cartes ainsi obtenues forment un $C^{r-k}$-atlas et celui-ci munit $J^k(X, Y)$ d’une *structure de K-variété de classe $C^{r-k}$*[^1]

Si $(x, y) \in X \times Y$, les ensembles $J_x^k(X, Y), J^k(X, Y)_y$ et $J_x^k(X, Y)_y$ sont des sous-variétés fermées de $J^k(X, Y)$.

12.3.2. Si $X$ et $Y$ sont pures (resp. de dimension finie, resp. séparées, resp. connexes), il en est de même de $J^k(X, Y)$.

Si $U$ (resp. $V$) est ouvert dans $X$ (resp. dans $Y$), $J^k(U, V)$ est une sous-variété ouverte de $J^k(X, Y)$, cf. 12.1.3.

12.3.3. Les applications $s : J^k(X, Y) \to X, b : J^k(X, Y) \to Y$ et $(s, b) : J^k(X, Y) \to X \times Y$ sont des fibrations (6.1.1) de classe $C^{r-k}$. Lorsque $k = 0$, $(s, b)$ est un isomorphisme.

12.3.4. Notons $T_X$ et $T_Y$ les fibrés vectoriels $pr_1^* T(X)$ et $pr_2^* T(Y)$ sur $X \times Y$, et soit $\mathscr{L}(T_X; T_Y)$ le fibré des homomorphismes de $T_X$ dans $T_Y$ (7.7.3); si $(x, y) \in X \times Y$, on a
$$
\mathscr{L}(T_X; T_Y)_{(x, y)} = \mathscr{L}(T_x(X); T_y(Y)).
$$
Soit $j \in J^k(X, Y), k \geqslant 1$, et soit $f \in j$. L’application tangente à $f$ en $x = s(j)$ ne dépend que de $j$; on la note $T(j)$; c’est un élément de $\mathscr{L}(T_x(X); T_y(Y))$, où $y = b(j)$. Lorsque $k = 1$ l’application
$$
T : J^1(X, Y) \to \mathscr{L}(T_X; T_Y)
$$
ainsi définie est un isomorphisme de variétés de classe $C^{r-1}$.

Pour $X = K$, cet isomorphisme identifie $J_0^1(K, Y)$ à $T(Y)$; pour $Y = K$, il identifie $J^1(X, K)_0$ au dual $T'(X)$ de $T(X)$.

12.3.5. Soit $k'$ un entier tel que $0 \leqslant k' \leqslant k$. L’application
$$
\rho^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)
$$
est une fibration de classe $C^{r-k}$.

12.3.6. Soit $Z$ une variété de classe $C^r$, et soit $T$ l’ensemble des couples
$$
(j, j') \in J^k(X, Y) \times J^k(Y, Z)
$$
tels que $b(j) = s(j')$. Alors $T$ est une sous-variété de $J^k(X, Y) \times J^k(Y, Z)$ et l’application $(j, j') \mapsto j' \circ j$ est un morphisme de classe $C^{r-k}$ de $T$ dans $J^k(X, Z)$.

12.3.7. Si $f : X \to Y$ est un morphisme de classe $C^r$, l’application $x \mapsto j_x^k(f)$ est un morphisme $j^k(f)$ de classe $C^{r-k}$ de $X$ dans $J^k(X, Y)$.

12.3.8. Soient $k'$ et $k''$ des entiers positifs de somme $k$. Soit $x \in X$, soit $U$ un voisinage ouvert de $x$, et soit $f : U \to Y$ un morphisme de classe $C^r$. L’application
$$
x \mapsto j_x^{k'}(f) : U \to J^{k'}(X, Y)
$$
est de classe $C^{r-k'}$ et son jet d’ordre $k''$ en $x$ ne dépend que de $j_x^k(f)$. On obtient ainsi une application canonique
$$
\alpha : J^k(X, Y) \to J^{k''}(X, J^{k'}(X, Y))
$$
qui est de classe $C^{r-k}$; si $K$ est de caractéristique zéro, c’est un plongement.

12.3.9. Soient $X', Y'$ des variétés de classe $C^r$, soient $f : X \to X'$ et $g : Y' \to Y$ des morphismes, et soient $(x, y') \in X \times Y'$, $x' = f(x)$, $y = g(y')$. Si $u \in J_{x'}^k(X', Y')_{y'}$, posons
$$
J_{x'}^k(f, g)_y(u) = j_y^k(g) \circ u \circ j_x^k(f).
$$
On obtient ainsi une application
$$
J^k(f, g) : J^k(X', Y') \times_{X'} X \to J^k(X, Y)
$$
qui est de classe $C^{r-k}$.

12.3.10. Soit $A$ une partie compacte de $X$. Soit $\mathscr{C}^k(X; Y)$ l’ensemble des applications de classe $C^k$ de $X$ dans $Y$. Pour tout $f \in \mathscr{C}^k(X; Y)$, l’application $j^k(f)|A$ appartient à l’ensemble $\mathscr{C}(A; J^k(X, Y))$ des applications continues de $A$ dans $J^k(X, Y)$. On a ainsi défini une application $\lambda$ de $\mathscr{C}^k(X; Y)$ dans $\mathscr{C}(A; J^k(X, Y))$. L’image réciproque par $\lambda$ de la topologie de la convergence compacte sur $\mathscr{C}(A; J^k(X, Y))$ (TG, X, § 3, déf. 1) est une topologie sur $\mathscr{C}^k(X; Y)$; on l’appelle la *topologie de la $C^k$-convergence uniforme sur $A$*.

### 12.4. Repères et fibrations principales

12.4.1. Soit $j \in J^k(X, Y)$ et soient $x = s(j)$, $y = b(j)$. On dit que $j$ est *inversible* s’il existe $j' \in J_y^k(Y, X)_x$ tel que $j' \circ j = j_x^k(\mathrm{Id}_X)$ et $j \circ j' = j_y^k(\mathrm{Id}_Y)$; le jet $j'$ est alors déterminé de manière unique; on le note $j^{-1}$. Si $k = 0$, tout jet est inversible. Si $k \geqslant 1$, les conditions suivantes sont équivalentes:
a) $j$ est inversible;
b) l’application $T(j) : T_x(X) \to T_y(Y)$ (cf. 12.3.4) est un isomorphisme;
c) il existe un isomorphisme $g$ de classe $C^r$ d’un voisinage ouvert de $x$ sur un voisinage ouvert de $y$, tel que $j_x^k(g) = j$.

12.4.2. Soit $E$ un espace de Banach. On note $\mathbf{GL}^k(E)$ l’ensemble des jets d’ordre $k$ de $E$ dans $E$ qui sont inversibles et ont $0$ pour source et pour but; c’est un ouvert de $J_0^k(E, E)_0$. Muni de la loi de composition des jets, et de la structure de variété induite par celle de l’espace de Banach $J_0^k(E, E)_0 = Q^k(E, E)$, c’est une variété de groupe de classe $C^\omega$.

On a $\mathbf{GL}^0(E) = \{ e \}$. Le groupe $\mathbf{GL}^1(E)$ s’identifie, au moyen de $T$, au groupe $\mathbf{GL}(E)$ des automorphismes de $E$.

Si $k' \leqslant k$, l’application $r^{k, k'} : \mathbf{GL}^k(E) \to \mathbf{GL}^{k'}(E)$ est un homomorphisme de classe $C^\omega$ et c’est une submersion surjective. L’application $f \mapsto \mathrm{Id}_E + f$ est un isomorphisme de variétés de groupes de $P_k(E, E)$ sur le noyau de $r^{k, k-1}$.

12.4.3. Soit E un espace de Banach. Pour tout $x \in X$, on appelle E-repère d’ordre k de X en x tout élément inversible de $J_0^k(E, X)_x$. L’ensemble des E-repères d’ordre k de X est une sous-variété ouverte $R^k(E, X)$ de $J_0^k(E, X)$; l’application b a pour restriction un morphisme, encore noté b, de $R^k(E, X)$ dans X; de même, si $k' \leq k$, on note encore $r^{k, k'}$ le morphisme de $R^k(E, X)$ dans $R^{k'}(E, X)$, restriction de l’application $r^{k, k'}$ de 12.1.5.

12.4.4. On suppose que X est pure de type E (5.1.7). Le groupe $GL^k(E)$ opère à droite sur $R^k(E, X)$ par la loi $(\rho, u) \mapsto \rho \circ u$ et le quadruplet $\lambda_X = (R^k(E, X), GL^k(E), X, b)$ est une fibration principale (6.2.1) de groupe structural $GL^k(E)$, de base X et de classe $C^{r-k}$.

Si $k' \leq k$, soit H le noyau de $r^{k, k'} : GL^k(E) \to GL^{k'}(E)$; le quadruplet $(R^k(E, X), H, R^{k'}(E, X), r^{k, k'})$ est une fibration principale de classe $C^{r-k}$.

La variété $J^k(X, Y)$ est munie d’une structure d’espace fibré associé à $\lambda_X$ (6.5.1): la fibre type est $J_0^k(E, Y)$ sur laquelle $GL^k(E)$ opère à gauche par la loi $(u, j) \mapsto j \circ u^{-1}$; l’application repère $R^k(E, X) \times J_0^k(E, Y) \to J^k(X, Y)$ transforme $(\rho, j)$ en $j \circ \rho^{-1}$. La projection $J^k(X, Y) \to X$ correspondant à cette structure d’espace fibré est s.

12.4.5. Soit F un espace de Banach, et supposons Y pure de type F. Alors $J^k(X, Y)$ est munie d’une structure d’espace fibré associé à $\lambda_Y$: la fibre type est $J^k(X, F)_0$ sur laquelle $GL^k(F)$ opère à gauche par la loi $(v, j) \mapsto v \circ j$; l’application repère est $(\sigma, j) \mapsto \sigma \circ j$; la projection $J^k(X, Y) \to Y$ est b.

12.4.6. Les hypothèses étant celles de 12.4.4 et 12.4.5, soit $\mu$ la fibration principale
$$
(R^k(E, X) \times R^k(F, Y), GL^k(E) \times GL^k(F), X \times Y, b \times b),
$$
produit de $\lambda_X$ et $\lambda_Y$. Alors $J^k(X, Y)$ est munie d’une structure d’espace fibré associé à $\mu$: la fibre type est $J_0^k(E, F)_0$ sur laquelle $GL^k(E) \times GL^k(F)$ opère à gauche par la loi $((u, v), j) \mapsto v \circ j \circ u^{-1}$; l’application repère est $((\rho, \sigma), j) \mapsto \sigma \circ j \circ \rho^{-1}$; la projection $J^k(X, Y) \to X \times Y$ est $(s, b)$.

### 12.5. Jets de sections

12.5.1. Soit $\pi : Y \to X$ une submersion, soit $x \in X$, et soit $s \in J_x^k(X, Y)$. On dit que s est un jet de section (d’ordre k) de $\pi$ si s est de la forme $j_x^k(f)$, où f est une section de classe $C^r$ de $\pi$ au-dessus d’un voisinage ouvert de x; cette condition équivaut à
$$
j_{b(s)}^k(\pi) \circ s = j_x^k(\mathrm{Id}_X).
$$
On note $P_x^k(\pi)$ (resp. $P^k(\pi)$) l’ensemble des jets $s \in J_x^k(X, Y)$ (resp. $J^k(X, Y)$) qui sont des jets de section de $\pi$; c’est une sous-variété de classe $C^{r-k}$ de $J^k(X, Y)$. Les applications
$$
s : P^k(\pi) \to X \quad \text{et} \quad b : P^k(\pi) \to Y
$$
sont des submersions; si $\pi$ est une fibration, ce sont des fibrations. Pour $k = 0$, b est un isomorphisme, par lequel on identifie $P^0(\pi)$ à Y.

Si $k' \leq k$, l’application $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ applique $P^k(\pi)$ dans $P^{k'}(\pi)$; l’application de $P^k(\pi)$ dans $P^{k'}(\pi)$ déduite de $r^{k, k'}$ est une fibration de classe $C^{r-k}$.

12.5.2. Soit $Z$ une variété de classe $C^r$; supposons que $Y = X \times Z$ et soit $\pi = \mathrm{pr}_1 : Y \to X$. La restriction de $J^k(\mathrm{Id}_X, \mathrm{pr}_2)$ (cf. 12.3.9) à $P^k(\pi)$ est un isomorphisme de $P^k(\pi)$ sur $J^k(X, Z)$, par lequel on identifie ces deux variétés.

12.5.3. Soit $Y'$ une variété de classe $C^r$, soient $\pi : Y \to X$ et $\pi' : Y' \to X$ des submersions et soit $g : Y \to Y'$ un morphisme tel que $\pi' \circ g = \pi$. L’application $J^k(\mathrm{Id}_X, g)$ a pour restriction une application

$$
P^k(g) : P^k(\pi) \to P^k(\pi')
$$

qui est de classe $C^{r-k}$.

Soit $X'$ une variété de classe $C^r$, et soit $f : X' \to X$ un morphisme; posons $(Y', \pi') = f^*(Y, \pi)$, cf. 5.11.5. L’application $J^k(f, \mathrm{Id}_Y)$ (cf. 12.3.9) définit une application de classe $C^{r-k}$ de $f^*P^k(\pi)$ dans $P^k(\pi')$.

### 12.6. Jets de sections d’un fibré vectoriel

12.6.1. Soit $E$ un fibré vectoriel de classe $C^r$ de base $X$, et soit $\pi$ sa projection. Soient $c_0 = (U, \varphi, F_0)$ une carte vectorielle de $E$ et $c_1 = (U, \psi, F_1)$ une carte de la variété $X$, de même domaine $U$. Ces cartes définissent une bijection $\theta$ de $P^k(\pi)|U$ sur $J^k(\psi(U), F_0) = \psi(U) \times F_0 \times Q^k(F_1, F_0)$, cf. 12.2.2 et 12.3.1, d’où une carte vectorielle

$$
d = (U, \theta, G), \quad \text{avec} \quad G = F_0 \times Q^k(F_1, F_0) = \prod_{m=0}^k P_m(F_1; F_0)
$$

de $P^k(\pi)$. Les cartes ainsi obtenues forment un $C^{r-k}$-atlas vectoriel, qui munit $P^k(\pi)$ d’une structure de fibré vectoriel de classe $C^{r-k}$, de base $X$. Ce fibré vectoriel est noté $P^k(E)$; la structure de variété sous-jacente est celle définie en 12.5.1.

Soit $U$ un ouvert de $X$, et soit $f \in \mathscr{S}_E^r(U)$ une section de classe $C^r$ de $E$ au-dessus de $U$. L’application $j^k(f) : x \mapsto j_x^k(f)$ est une section de classe $C^{r-k}$ de $P^k(E)$ au-dessus de $U$. L’application $j^k : \mathscr{S}_E^r(U) \to \mathscr{S}_{P^k(E)}^{r-k}(U)$ est $K$-linéaire.

12.6.2. Si $F$ est un espace de Banach, l’identification (12.5.2) de $P^k(F_X)$ avec $J^k(X, F)$ munit cette dernière variété d’une structure de fibré vectoriel de classe $C^{r-k}$, de base $X$. Lorsque $F = K$, on écrit $P^k(X)$ au lieu de $P^k(K_X)$.

#### Exemple {#var-2-s12-n6-exa-1 .statement}

Prenons $X = K^n$, et notons $u_1, \ldots, u_n$ les fonctions coordonnées sur $K^n$; alors la fibre $P^k_0(X)$ de $P^k(X)$ en 0 admet pour base la famille des jets d’ordre $k$ des monômes $u_1^{m_1} \ldots u_n^{m_n}$, avec $m_i \geqslant 0, \sum_{i=0}^n m_i \leqslant k$.

12.6.3. Soient $d$ un entier $\geqslant 0$, $E_1, \ldots, E_d, F$ des fibrés vectoriels de classe $C^r$ de base $X$, et soit $u : E_1 \times_X \cdots \times_X E_d \to F$ un morphisme multilinéaire (7.3.1) de classe $C^r$. Il existe alors un morphisme multilinéaire

$$
P^k(u) : P^k(E_1) \times_X \cdots \times_X P^k(E_d) \to P^k(F)
$$

et un seul tel que

$$
P^k(u)(j^k(s_1), \ldots, j^k(s_d)) = j^k(u(s_1, \ldots, s_d))
$$

pour tout ouvert U de X et toute suite de sections $s_i \in \mathscr{S}_{E_i}'(U)$ pour $1 \leq i \leq d$.

Si A est un fibré en algèbres (7.3.2) de base X, le morphisme de $P^k(A) \times_X P^k(A)$ dans $P^k(A)$ déduit de la multiplication $A \times_X A \to A$ fait de $P^k(A)$ un fibré en algèbres; si A est un fibré en algèbres associatives, $P^k(A)$ est un fibré en algèbres associatives; si en outre M est un fibré en A-modules (7.3.3), $P^k(M)$ est un fibré en $P^k(A)$-modules. En particulier, $P^k(X)$ est un *fibré en algèbres* associatives, commutatives et unifères; si E est un fibré vectoriel, $P^k(E)$ est un *fibré en $P^k(X)$*-modules. Si $u : E \to F$ est un morphisme de fibrés vectoriels, alors $P^k(u) : P^k(E) \to P^k(F)$ est un $P^k(X)$-homomorphisme.

12.6.4. Si $E \xrightarrow{u} F \xrightarrow{v} G$ est une suite exacte localement directe de fibrés vectoriels de base X, il en est de même de la suite

$$
P^k(E) \to P^k(F) \to P^k(G)
$$

où les homomorphismes considérés sont $P^k(u)$ et $P^k(v)$.

12.6.5. Soient $k'$ et $k''$ deux entiers positifs de somme $k$, et soit E un fibré vectoriel de classe $C^r$ et de base X. Le morphisme

$$
\alpha : J^k(X, E) \to J^{k''}(X, J^{k'}(X, E)) \quad (\text{cf. } 12.3.8)
$$

induit un morphisme de fibrés vectoriels

$$
\beta : P^k(E) \to P^{k''}(P^{k'}(E))
$$

qui est de classe $C^{r-k}$. Si U est un ouvert de X et $f \in \mathscr{S}_E'(U)$, on a

$$
\beta(j^{k}(f)) = j^{k''}(j^{k'}(f)).
$$

Lorsque K est de caractéristique zéro, $\beta$ est un isomorphisme de $P^k(E)$ sur un sous-fibré vectoriel de $P^{k''}(P^{k'}(E))$.

12.6.6. Soit $k'$ un entier tel que $0 \leq k' \leq k$, et soit E un fibré vectoriel de classe $C^r$ et de base X. L’application

$$
r^{k, k'} : P^k(E) \to P^{k'}(E)
$$

est un morphisme surjectif localement direct de classe $C^{r-k}$. Son noyau $N^{k, k'}(E)$ est formé des jets de section de E ayant un contact d’ordre $\geq k'$ avec la section nulle.

12.6.7 (*Le foncteur vectoriel $P_m$*). Les notations étant celles de 7.6, 7.7, 7.8, posons $I_+ = \{0\}, I_- = \{1\}$ et soit m un entier $\geq 0$. Si $\mathscr{V} = (V_0, V_1)$ est un couple d’espaces de Banach, notons $\tau_m(\mathscr{V})$ l’espace de Banach $P_m(V_1; V_0)$ des *polynômes-continus* homogènes de degré m sur $V_1$ à valeurs dans $V_0$ (A.2). De même, si $f = (f_0, f_1)$. où $f_0 : V_0 \to V'_0$ et $f_1 : V'_1 \to V_1$ sont des morphismes d’espaces de Banach, notons $\tau_m(f)$ le morphisme $p \mapsto f_0 \circ p \circ f_1$ de $P_m(V_1; V_0)$ dans $P_m(V'_1; V'_0)$. On obtient ainsi un *foncteur* vectoriel $\tau_m$ de classe $C^\omega$. Si $E_0$ et $E_1$ sont deux fibrés vectoriels de base $X$, on note $P_m(E_1; E_0)$ le fibré vectoriel déduit de $(E_0, E_1)$ par $\tau_m$ (7.6.2).

12.6.8. Reprenons les notations et hypothèses de 12.6.1. Il existe un morphisme de fibrés vectoriels

$$
\iota : P_k(T(X); E) \to P^k(E) \quad (\text{cf. } 12.6.6),
$$

et un seul tel que, quelles que soient la carte vectorielle $c_0 = (U, \varphi, F_0)$ de $E$ et la carte $c_1 = (U, \psi, F_1)$ de $X$, le diagramme suivant soit commutatif:

$$
\begin{array}{ccc}
P_k(T(X), E)|U & \xrightarrow{\iota|U} & P^k(E)|U \\
\downarrow \eta & & \downarrow \theta \\
U \times P_k(F_1; F_0) & \xrightarrow{i} & U \times \prod_{m=0}^k P_m(F_1; F_0)
\end{array}
$$

où: 1) $\iota|U$ est la restriction de $\iota$ à $P_k(T(X), E)|U$;
   2) $\theta$ est la bijection définie en 12.6.1;
   3) $i$ est l’application $(u, p) \mapsto (u, 0, \ldots, 0, p)$;
   4) $\eta$ est déduite, au moyen du foncteur vectoriel $\tau_k$, de la carte vectorielle $c'_1$ de $T(X)$ (cf. 8.1.1) et de la carte vectorielle $c_0$ de $E$.

Le morphisme $\iota$ est un isomorphisme de $P_k(T(X); E)$ sur le sous-fibré vectoriel $N^{k, k-1}(E)$ de $P^k(E)$ (cf. 12.6.6); la suite

$$
0 \to P_k(T(X); E) \xrightarrow{\iota} P^k(E) \xrightarrow{\tau^{k, k-1}} P^{k-1}(E) \to 0
$$

est une suite exacte localement directe de fibrés vectoriels.

Plus généralement, posons $N_0 = P^k(E)$, $N_m = N^{k, m-1}(E)$ pour $m \geq 1$, de sorte que les $N_m$ forment une suite décroissante de sous-fibrés vectoriels de $P^k(E)$:

$$
P^k(E) = N_0 \supset N_1 \supset \cdots \supset N_k \supset N_{k+1} = 0.
$$

Pour $0 \leq m \leq k$, la projection $r^{k, m} : P^k(E) \to P^m(E)$ définit un isomorphisme de $N_m/N_{m+1}$ sur $N^{m, m-1}(E)$; vu ce qui précède, on obtient ainsi des isomorphismes

$$
\iota_m : N_m/N_{m+1} \to P_m(T(X); E) \quad (0 \leq m \leq k).
$$

On a en particulier $N_0/N_1 \simeq E$ et $N_1/N_2 \simeq \mathscr{L}(T(X); E)$. Pour $k = 1$, cela donne une suite exacte:

$$
0 \to \mathscr{L}(T(X); E) \to P^1(E) \to E \to 0.
$$

### 12.7. Affaiblissement de structure

On suppose $K = \mathbf{R}$. Soit $r' \in N_k$ avec $k \leq r' \leq r$ et soient $X'$ et $Y'$ les variétés de classe $C^{r'}$ obtenues à partir de $X$ et $Y$ par affaiblissement de structure (5.13.1). Soient $x \in X$ et $j \in J_x^k(X, Y)$; soient $U$ une partie ouverte de $X$ contenant $x$ et $f$ une application de classe $C^k$ de $U$ dans $Y$, telles que $j_x^k(f) = j$. Considérons $f$ comme un germe de morphisme de X' dans Y'; son jet $j' \in J_x^k(X', Y')$ ne dépend que de $j$. L’application $j \mapsto j'$ est un isomorphisme de classe $C^{r'-k}$ de $J^k(X, Y)$ sur $J^k(X', Y')$; elle permet d’identifier $J^k(X', Y')$ à la variété de classe $C^{r'-k}$ déduite de la variété $J^k(X, Y)$ de classe $C^{r-k}$ par affaiblissement de structure. Un résultat analogue s’applique aux variétés $P^k(\pi)$ et $P^k(E)$ des n° 12.5 et 12.6.

[^1]: Lorsque $k = r$ (ce qui n’est possible que si $K = \mathbf{R}$), $J^k(X, Y)$ est munie d’une structure de *variété topologique* (cf. *Conventions et Notations*) et les morphismes et fibrations considérées ci-après doivent être pris dans un sens purement topologique (cf. note de bas de page du §6).
