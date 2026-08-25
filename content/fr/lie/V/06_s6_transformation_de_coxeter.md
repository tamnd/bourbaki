---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 6
section_title: Transformation de Coxeter
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0115-0122, 0138-0140
extraction: ocr
subsections:
    - "no": 1
      title: Définition des transformations de Coxeter
      page: 0
      pdf_page: 115
    - "no": 2
      title: Valeurs propres d’une transformation de Coxeter. Exposants
      page: 0
      pdf_page: 116
statements: 14
exercises: 4
content_sha256: aef30dc7ca559392b46ef6dd97b0bfe4a41ce470e3a631f7c76c02fd30963b86
---

## § 6. Transformation de Coxeter

Dans ce paragraphe, $V$ désigne un espace vectoriel réel de dimension finie $l$ et $W$ désigne un sous-groupe fini de $\mathbf{GL}(V)$, engendré par des réflexions, et essentiel (\S 3, n° 7). On munit $V$ d’un produit scalaire $(x|y)$ invariant par $W$
On note $\mathfrak{H}$ l’ensemble des hyperplans $H$ de $V$ tels que la réflexion orthogonale $s_H$ correspondante appartienne à $W$.

### 1. Définition des transformations de Coxeter

Nous appellerons chambre ordonnée relative à $W$ le couple formé d’une chambre $C$ déterminée par $\mathfrak{H}$ et d’une bijection $i \mapsto H_i$ de $\{1, 2, \ldots, l\}$ sur l’ensemble des murs de $C$ (cf. \S 3, n° 9, prop. 7).

#### Définition 1 {#lie-v-s6-def-1 .statement}

On appelle transformation de Coxeter définie par une chambre ordonnée $(C, (H_i)_{1 \leq i \leq l})$ l’élément $c = s_{H_1} s_{H_2} \cdots s_{H_l}$ de $W$.

#### Proposition 1 {#lie-v-s6-prop-1 .statement}

Toutes les transformations de Coxeter de $W$ sont conjuguées dans $W$.

Comme $W$ permutte transitivement les chambres déterminées par $\mathfrak{H}$ (\S 3, n° 2, th. 1), tout revient à prouver ceci : soient $(C, (H_i)_{1 \leq i \leq l})$ une chambre ordonnée, et $\pi \in \mathfrak{S}_l$; alors $s_{H_1} s_{H_2} \cdots s_{H_l}$ et $s_{H_{\pi(1)}} s_{H_{\pi(2)}} \cdots s_{H_{\pi(l)}}$ sont conjugués dans W. Compte tenu du § 4, n° 8, prop. 8, ceci résultera aussitôt du lemme suivant:

#### Lemme 1 {#lie-v-s6-lem-1 .statement}

Soient X une forêt finie, x ↦ g_x une application de X dans un groupe Γ, telle que g_x et g_y commutent toutes les fois que x et y ne sont pas liés dans X. Soit T l’ensemble des ordres totaux sur X. Pour tout ξ ∈ T, soit p_ξ le produit dans Γ de la séquence (g_x)_{x ∈ X} définie par ξ. Les éléments p_ξ sont alors conjugués dans Γ.

1) Raisonnons par récurrence sur n = Card X. Le cas où n = 1 est immédiat, supposons n ≥ 2. Il existe dans X un sommet terminal a (chap. IV, Annexe, n° 3, prop. 2). Soit b ∈ X − {a} un sommet lié à a s’il en existe; si a n’est lié à aucun sommet de X − {a}, on prend b quelconque dans X − {a}. Dans tous les cas, g_a commute à g_x pour x ≠ b. Soit η ∈ T tel que a soit le plus grand élément de X et b le plus grand élément de X − {a}; soit ξ ∈ T, et prouvons que p_ξ, p_η sont conjugués.

2) Supposons d’abord que, pour ξ, a soit le plus grand élément de X et b le plus grand élément de X − {a}. Soit X’ le sous-graphe plein X − {a}, qui est une forêt. Définissons une application x ↦ g'_x de X’ dans Γ en posant g'_x = g_x si x ≠ b, g'_b = g_bg_a. Soient ξ’, η’ les restrictions de ξ, η à X’. L’hypothèse de récurrence est applicable, donc p_ξ’ et p_η’ sont conjugués. Mais il est clair que p_ξ’ = p_ξ, p_η’ = p_η, d’où le lemme dans ce cas.

3) Supposons que a soit le plus grand élément de X pour ξ. Soit X_1 (resp. X_2) l’ensemble des éléments de X − {a} strictement majorés (resp. minorés) par b; soit ξ_i la restriction de ξ à X_i. On a

$$
p_ξ = p_{ξ_1} g_b p_{ξ_2} g_a = p_{ξ_1} g_b g_a p_{ξ_2},
$$

et cet élément est conjugué de p_{ξ_1} p_{ξ_2} g_b g_a. On est donc ramené au cas 2).

4) Dans le cas général, soit X_3 (resp. X_4) l’ensemble des éléments de X strictement majorés (resp. minorés) par a; soit ξ_i la restriction de ξ à X_i. On a p_ξ = p_{ξ_3} g_a p_{ξ_4}, et cet élément est conjugué de p_{ξ_4} p_{ξ_3} g_a. On est donc ramené au cas 3).

Il résulte de la prop. 1 que toutes les transformations de Coxeter ont le même ordre h = h(W). Ce nombre s’appelle le nombre de Coxeter de W.

#### Remarque {#lie-v-s6-n1-rem-1 .statement}

Soient W_1, ..., W_m des groupes finis essentiels dans des espaces V_1, ..., V_m, engendrés par des réflexions. Soit C_f une chambre relative à W_f. Soit W le groupe W_1 × ... × W_m opérant dans V_1 × ... × V_m. Alors C_1 × ... × C_m est une chambre relative à W. Les transformations de Coxeter de W définies par C sont les produits c_1 c_2 ... c_m, où c_j est une transformation de Coxeter de W_f définie par C_f.

### 2. Valeurs propres d’une transformation de Coxeter. Exposants

Comme toutes les transformations de Coxeter sont conjuguées (n° 1, prop. 1), elles ont même polynôme caractéristique P(T). Soit h le nombre de Coxeter de W. On a

$$
P(T) = \prod_{j=1}^{l} \left( T - \exp \frac{2i\pi m_j}{h} \right)
$$

où $m_1, m_2, \ldots, m_l$ sont des entiers tels que

$$
0 \leq m_1 \leq m_2 \leq \cdots \leq m_l < h.
$$

#### Définition 2 {#lie-v-s6-def-2 .statement}

Les entiers $m_1, m_2, \ldots, m_l$ s’appellent les exposants de W.

Soient C une chambre déterminée par $\mathfrak{g}$, $H_1, \ldots, H_l$ ses murs, et posons $s_i = s_{H_i}$. Notons $e_i$ le vecteur unitaire orthogonal à $H_i$ et situé du même côté de $H_i$ que C. D’après la prop. 2 de l’Annexe du chap. IV, on peut supposer les $H_i$ numérotés de telle manière que $e_1, e_2, \ldots, e_r$ soient deux à deux orthogonaux, et que $e_{r+1}, e_{r+2}, \ldots, e_l$ soient deux à deux orthogonaux. Alors $s' = s_1 s_2 \ldots s_r$ est la symétrie orthogonale par rapport au sous-espace

$$
V' = H_1 \cap H_2 \cap \cdots \cap H_r,
$$

$s'' = s_{r+1} s_{r+2} \ldots s_l$ est la symétrie orthogonale par rapport au sous-espace

$$
V'' = H_{r+1} \cap H_{r+2} \cap \cdots \cap H_l,
$$

et $c = s' s''$ est une transformation de Coxeter. Comme $(e_1, \ldots, e_l)$ est une base de V, V est somme directe de $V'$ et $V''$.

On en déduit d’abord que l' $n'est pas valeur propre de c$. Car si $x \in V$ est tel que $c(x) = x$, on a $s'(x) = s''(x)$, donc $x - s'(x) = x - s''(x)$ est orthogonal à $V'$ et $V''$, donc nul, d’où $x = s'(x) = s''(x) \in V' \cap V'' = \{0\}$.

On a par suite

(1)

$$
0 < m_1 \leq m_2 \leq \cdots \leq m_l < h.
$$

Le polynôme caractéristique de $c$ est à coefficients réels. Donc, pour tout $j$, l’exposant de $T - \exp \frac{2i\pi m_j}{h}$ dans $P(T)$ est égal à celui de $T - \exp \frac{2i\pi (h - m_j)}{h}$. D’où

(2)

$$
m_j + m_{l+1-j} = h \quad (1 \leq j \leq l).
$$

Ajoutant membre à membre les égalités (2), on obtient :

(3)

$$
m_1 + m_2 + \cdots + m_l = \frac{1}{2} lh.
$$

#### Lemme 2 {#lie-v-s6-lem-2 .statement}

Supposons W irréductible. Avec les notations précédentes, il existe deux vecteurs linéairement indépendants $z', z''$ tels que :
(i) le plan P engendré par $z', z''$ est stable par $s'$ et $s''$;
(ii) $s'|P$ et $s''|P$ sont les réflexions orthogonales par rapport à $Rz'$ et $Rz''$;

(iii) $z', z'' \in \overline{C}$, et $P \cap C$ est l’ensemble des combinaisons linéaires de $z'$, $z''$ à coefficients $> 0$.

Soit $(e^1, \ldots, e^l)$ la base de $V$ telle que $(e^i|e_j) = \delta_{ij}$. Alors $C$ est le cône simplicial ouvert déterminé par les $e^i$ (\S 3, no 9, prop. 7). Il est clair que $V'$ est engendré par $e^{r+1}, \ldots, e^l$ et $V''$ par $e^1, \ldots, e^r$. Soit $q$ l’endomorphisme de $V$ tel que $q(e^1) = e_1, \ldots, q(e^l) = e_l$. Sa matrice par rapport à $(e^1, \ldots, e^l)$ est $Q = ((e_i|e_j))$. On a $(e_i|e_j) \leq 0$ pour $i \neq j$ (\S 3, no 4, prop. 3). Puisque $W$ est irréductible, il n’existe pas de partition $\{1, 2, \ldots, l\} = I_1 \cup I_2$ telle que $(e_i|e_j) = 0$ pour $i \in I_1$ et $j \in I_2$. Donc (\S 3, no 5, lemme 4) $Q$ admet un vecteur propre $(a_1, \ldots, a_l)$ à coordonnées toutes $> 0$; soit $a$ la valeur propre correspondante. Posons

$$
z = a_1 e^1 + \cdots + a_l e^l,
z'' = a_1 e^1 + \cdots + a_r e^r \in V'' \cap \overline{C},
z' = a_{r+1} e^{r+1} + \cdots + a_l e^l \in V' \cap \overline{C},
$$

et soit $P$ le plan engendré par $z'$ et $z''$. Alors $P \cap C$ est l’ensemble des combinaisons linéaires de $z'$ et $z''$ à coefficients $> 0$. La relation $q(z) = az$ donne

$$
\sum_{j=1}^l a_j e_j = \sum_{j=1}^l a a_j e^j;
$$
en multipliant scalairement par $e_k$ (où $k \leq r$), il vient
$$
a_k + \sum_{j=r+1}^l a_j (e_j|e_k) = a a_k; \text{ donc}
$$
$$
(a - 1)z'' = \sum_{k=1}^r \left( \sum_{j=r+1}^l a_j (e_j|e_k) \right) e^k
= \sum_{j=r+1}^l a_j \left( \sum_{k=1}^r (e_j|e_k) e^k \right)
= \sum_{j=r+1}^l a_j (-e^j + \sum_{k=1}^l (e_j|e_k) e^k)
= - \sum_{j=r+1}^l a_j e^j + \sum_{j=r+1}^l a_j e_j
= -z' + \sum_{j=r+1}^l a_j e_j.
$$

Ainsi, $(a - 1)z'' + z'$ est orthogonal à $e^1, \ldots, e^r$, c’est-à-dire à $V''$. Donc $s''$ laisse stable le plan engendré par $z''$ et $(a - 1)z'' + z'$, c’est-à-dire $P$. De même, $s'$ laisse stable $P$. Comme $z' \in P \cap V'$ et $z'' \in P \cap V''$, $s'|P$ et $s''|P$ sont les réflexions par rapport à $Rz'$ et $Rz''$.

#### Théorème 1 {#lie-v-s6-thm-1 .statement}

On suppose $W$ irréductible. Alors :

(i) $m_1 = 1,\ m_l = h - 1$.
(ii) Card ($\xi$) = $\frac{1}{2} lh$.

Conservons les notations précédentes. La restriction de $c = s's''$ à P est la rotation d’angle $2(\overline{z''}, z')$ (\S 2, n° 5, cor. de la prop. 6). Comme $c$ est d’ordre $h$, les $h$ éléments $1, c, \ldots, c^{h-1}$ de W sont deux à deux distincts; les éléments $s'$, $s'c, \ldots, s'c^{h-1}$ sont donc deux à deux distincts, et sont distincts des précédents car $c^i|P$ est une rotation et $s'c^j|P$ est une réflexion. L’ensemble

$$
\{1, c, \ldots, c^{h-1}, s', s'c, \ldots, s'c^{h-1}\}
$$

est le sous-groupe $W'$ de W engendré par $s'$ et $s''$, et induit dans P le groupe $W''$ engendré par les réflexions orthogonales par rapport à $Rz', Rz''$. Le transformé de C par un élément de $W'$ est disjoint de — C ou égal à — C. Donc le transformé de $P \cap C$ par un élément de $W''$ est disjoint de — (P $\cap$ C) ou égal à — (P $\cap$ C). Donc, pour une orientation convenable de P, il existe un entier $m > 0$ tel que $(\overline{z''}, z') = \frac{\pi}{m}$ (\S 2, n° 5, cor. de la prop. 7). Par ailleurs, les ensembles $g'(C)$, pour $g' \in W'$, sont deux à deux disjoints; les ensembles $g''(P \cap C)$, pour $g'' \in W''$, sont donc deux à deux disjoints; ainsi, $W''$ est d’ordre $2h$. D’où $m = h$. En définitive, $c|P$ est une rotation d’angle $\frac{2\pi}{h}$, et admet par suite les valeurs propres $\exp \frac{2i\pi}{h}$, $\exp \frac{2i\pi(h-1)}{h}$. Ceci prouve que $m_1 = 1$, $m_l = h - 1$.

Les transformées de $Rz'$ et $Rz''$ par $W'$ sont $h$ droites $D_1, \ldots, D_h$ de P, et les points de $P - (D_1 \cup \cdots \cup D_h)$ sont transformés par des éléments de $W'$ de points de $P \cap C$. Donc un hyperplan de $\mathfrak{g}$ coupe nécessairement P suivant l’une des droites $D_i$, et par suite est transformé, par une opération de $W'$, d’un hyperplan de $\mathfrak{g}$ contenant $Rz'$ ou $Rz''$.

Or, tout $H \in \mathfrak{g}$ qui contient $Rz'$ est l’un des hyperplans $H_1, \ldots, H_r$. En effet, soit $e_H$ le vecteur unitaire orthogonal à H et situé du même côté de H que C. On a $e_H = \lambda_1 e_1 + \cdots + \lambda_l e_l$ avec des $\lambda_i$ tous $\geq 0$ (\S 3, n° 5, lemme 6, (i)). Or $0 = (e_H|z') = \lambda_{r+1} a_{r+1} + \cdots + \lambda_l a_l$, donc

$$
\lambda_{r+1} = \cdots = \lambda_l = 0, \quad \text{et} \quad e_H = \lambda_1 e_1 + \cdots + \lambda_r e_r.
$$

Supposons que deux des $\lambda_i$ soient non nuls, par exemple $\lambda_1$ et $\lambda_2$; comme $e_1, \ldots, e_r$ sont deux à deux orthogonaux, on aurait

$$
s_1(e_H) = -\lambda_1 e_1 + \lambda_2 e_2 + \cdots + \lambda_r e_r
$$

et les coordonnées de $s_1(e_H)$ ne seraient pas toutes de même signe, ce qui est absurde (*loc. cit.*). Donc $e_H$ est proportionnel à l’un des vecteurs $e_1, \ldots, e_r$, ce qui prouve notre assertion. De même, tout $H \in \mathfrak{g}$ qui contient $Rz''$ est l’un des hyperplans $H_{r+1}, \ldots, H_l$.

Le nombre d’éléments de $\mathfrak{g}$ contenant $Rz'$ ou $Rz''$ est donc $l$. Si $h$ est pair, Card($\mathfrak{g}$) est donc égal à $\frac{h}{2} l$. Si $h$ est impair, Card($\mathfrak{g}$) est égal à n° 6.2.

$$
\frac{h-1}{2} l + r, \text{ et aussi à } \frac{h-1}{2} l + (l-r); \text{ d'où } r = l - r, \text{ de sorte que }
r = \frac{l}{2}, \text{ et Card}(\mathfrak{S}) = \frac{h-1}{2} l + \frac{l}{2} = \frac{h}{2} l.
$$

#### Remarque {#lie-v-s6-n2-rem-1 .statement}

Conservons les notations de la démonstration précédente. Soient $c'$ l’extension $\mathbf{C}$-linéaire de $c$ à $V \otimes_{\mathbf{R}} \mathbf{C}$, et $c''$ la restriction de $c'$ à $P \otimes_{\mathbf{R}} \mathbf{C}$. D’après l’étude de $c|P$, $c''$ admet un vecteur propre $x$ correspondant à la valeur propre $\exp \frac{2i\pi}{h}$, et ce vecteur propre n’appartient à aucun ensemble $D \cap \mathbf{C}$, où $D$ désigne une droite de $P$ (puisque $D$ n’est pas stable par $c$). Or, pour tout $H \in \mathfrak{S}$, on a vu que $H \cap P$ est une droite; donc $x \in H \otimes_{\mathbf{R}} \mathbf{C}$.

#### Corollaire {#lie-v-s6-n2-cor-1 .statement}

*Soit $R_0$ l’ensemble des vecteurs unitaires de $V$ orthogonaux à un élément de $\mathfrak{S}$. Si $W$ est irréductible, on a, pour tout $x \in V$,*

$$
\sum_{u \in R_0} (x|u)^2 = h(x|x).
$$

Posons $f(x) = \sum_{u \in R_0} (x|u)^2$. Il est clair que $f$ est une forme quadratique positive invariante par $W$, non dégénérée puisque les $e_i$ forment une base de $V$. Comme $W$ est irréductible, il existe une constante $\beta$ telle que $f(x) = \beta (x|x)$ (\S 2, n° 1, prop. 1). Si $(x_i)_{1 \leq i \leq l}$ est une base orthonormale de $V$ pour le produit scalaire $(x|y)$, on a

$$
\begin{align*}
\beta l &= \sum_{i=1}^l \beta (x_i|x_i) = \sum_{i=1}^l f(x_i) = \sum_{i=1}^l \sum_{u \in R_0} (x_i|u)^2 \\
&= \sum_{u \in R_0} 1 = \operatorname{Card}(R_0) = 2 \operatorname{Card}(\mathfrak{S}) = hl.
\end{align*}
$$

D’où $\beta = h$, ce qui prouve (4).

#### Proposition 2 {#lie-v-s6-prop-2 .statement}

*Si $h$ est pair, l’unique élément de $W$ qui transforme $\mathbf{C}$ en $-\mathbf{C}$ est $c^{h/2}$.

Adoptons les notations de la démonstration du th. 1. Puisque $c|P$ est une rotation d’angle $\frac{2\pi}{h}$, $c^{h/2}$ transforme $z'$ en $-z'$, $z''$ en $-z''$, donc $z' + z'' = z$ en $-z$. Or $z \in \mathbf{C}$, donc la chambre $c^{h/2}(\mathbf{C})$ est nécessairement $-\mathbf{C}$.*

#### Proposition 3 {#lie-v-s6-prop-3 .statement}

*Supposons $W$ irréductible. Soient $u_1, \ldots, u_l$ des éléments homogènes de l’algèbre symétrique $S = S(V)$, algébriquement indépendants sur $\mathbf{R}$ et engendrant l’algèbre des éléments de $S$ invariants par $W$ (\S 5, n° 3, th. 3). Si $p_j$ est le degré de $u_j$, les exposants de $W$ sont $p_1 - 1, \ldots, p_l - 1$.

Posons $V' = V \otimes_{\mathbf{R}} \mathbf{C}$, $S' = S(V') = S \otimes_{\mathbf{R}} \mathbf{C}$, et prolongeons le produit scalaire de $V$ en une forme hermitienne sur $V'$. Si $c$ est une transformation de Coxeter de W, il existe une base orthonormale $(\mathbf{X}_i)_{1 \leq i \leq l}$ de $V'$ formée de vecteurs propres de $c \otimes 1$ (*Alg.*, chap. IX, § 7, n° 3, prop. 4); on peut supposer en outre que, pour $1 \leq j \leq l$, $\mathbf{X}_j$ correspond à la valeur propre $\exp \frac{2i\pi m_j}{h}$ de $c \otimes 1$. Il est clair que $S'$ s’identifie à l’algèbre $\mathbf{C}[\mathbf{X}_1, \ldots, \mathbf{X}_l]$, et l’on peut écrire $u_j \otimes 1 = f_j(\mathbf{X}_1, \ldots, \mathbf{X}_l)$, où $f_j$ est un polynôme homogène de degré $p_j$ dans $\mathbf{C}[\mathbf{X}_1, \ldots, \mathbf{X}_l]$. Posons $D_j = \frac{\partial}{\partial \mathbf{X}_j}$, et $J(\mathbf{X}_1, \ldots, \mathbf{X}_l) = \det(D_k f_j)$. Rappelons (\S 5, n° 4, prop. 5) que $J(\mathbf{X}_1, \ldots, \mathbf{X}_l)$ est proportionnel au produit dans $S'$ de $\mathrm{Card}(\mathfrak{S})$ vecteurs $y_k$ de $V$ donc chacun est orthogonal à un hyperplan de $\mathfrak{S}$. Comme on peut supposer que $\mathbf{X}_1 \notin H \otimes \mathbf{C}$ pour tout $H \in \mathfrak{S}$ (*Remarque*), les composantes sur $\mathbf{X}_1$ de chacun des vecteurs $y_k$ sont $\neq 0$, donc $J(1, 0, 0, \ldots, 0) \neq 0$. La règle de développement d’un déterminant prouve alors l’existence d’une permutation $\sigma$ de $\{1, 2, \ldots, l\}$ telle que $(D_{\sigma(j)} f_j)(1, 0, 0, \ldots, 0) \neq 0$ pour tout $j$. Comme $D_{\sigma(j)} f_j$ est homogène de degré $p_j - 1$, le coefficient de $X_1^{p_j-1} X_{\sigma(j)}$ dans $f_j(\mathbf{X}_1, \ldots, \mathbf{X}_l)$ est non nul. Or $f_j(\mathbf{X}_1, \ldots, \mathbf{X}_l)$ est invariant par $c \otimes 1$, et

$$(c \otimes 1)(X_1^{p_j-1} X_{\sigma(j)}) = (\exp \frac{2i\pi}{h} (p_j - 1 + m_{\sigma(j)}))(X_1^{p_j-1} X_{\sigma(j)}).$$

Ceci prouve que $p_j - 1 + m_{\sigma(j)} \equiv 0$ (mod. $h$). Or $h - m_{\sigma(j)}$ est un exposant (formule (2)). En permutant les $u_j$, on peut donc supposer que $p_j - 1 \equiv m_j$ (mod. $h$) pour tout $j$. Comme $p_j - 1 \geq 0$ et $m_j < h$, on a $p_j - 1 = m_j + \mu_j h$ avec $\mu_j$ entier $\geq 0$. D’après le \S 5, prop. 3, on voit que

$$\mathrm{Card}(\mathfrak{S}) = \sum_{j=1}^l (p_j - 1) = \sum_{j=1}^l m_j + h \sum_{j=1}^l \mu_j.$$

Compte tenu de la formule (3) et du th. 1 (ii), on obtient $h \sum_{j=1}^l \mu_j = 0$, donc $\mu_j = 0$, pour tout $j$ et finalement $p_j - 1 = m_j$ pour tout $j$.

#### Corollaire 1 {#lie-v-s6-prop-3-cor-1 .statement}

*Si* $(m_i)_{1 \leq i \leq l}$ *est la suite croissante des exposants de* $W$, *l’ordre de* $W$ *est égal à* $(m_1 + 1)(m_2 + 1) \ldots (m_l + 1)$.
Ceci résulte des relations $m_j + 1 = p_j$ et du \S 5, n° 3, cor. du th. 3.

#### Corollaire 2 {#lie-v-s6-prop-3-cor-2 .statement}

*Si* $c$ *est une transformation de Coxeter de* $W$,

$$\exp \left( \frac{2i\pi}{h} \right) \text{ et } \exp \left( -\frac{2i\pi}{h} \right)$$

*sont des valeurs propres de multiplicité* 1 *de* $c$.

Dans le cas contraire, il existerait deux invariants homogènes de degré 2 non proportionnels dans $S$, d’où deux formes quadratiques non proportionnelles sur $V^*$ invariantes par $W$, contrairement au \S 2, n° 1, prop. 1.

#### Corollaire 3 {#lie-v-s6-prop-3-cor-3 .statement}

Pour que l’homothétie de rapport — 1 dans V appartienne à W, il faut et il suffit que tous les exposants de W soient impairs. Lorsqu’il en est ainsi, h est pair et l’on a $c^{h/2} = -1$ pour toute transformation de Coxeter c de W.

La première assertion résulte du § 5, n° 3, prop. 4. Supposons les exposants de W impairs. Alors h est pair d’après la formule (2), et

$$
\left( \exp \frac{2i \pi m_j}{h} \right)^{h/2} = \exp (i \pi m_j) = -1;
$$

donc $c^{h/2} = -1$ puisque c est un automorphisme semi-simple de V (Alg., chap. IX, § 7, n° 3, prop. 4).

## EXERCICES {#lie-v-s6-exercises}

Dans les exercices ci-dessous (exerc. 3 excepté), les hypothèses et notations sont celles du § 6.

See the [exercises for § 6](exercises/s6/).
