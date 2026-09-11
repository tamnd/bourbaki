---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: Systèmes de racines
section: 2
section_title: Groupe de Weyl affine
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0172-0180, 0226-0226
extraction: ocr
subsections:
    - "no": 1
      title: Groupe de Weyl affine.
      page: 0
      pdf_page: 172
    - "no": 2
      title: Poids et points spéciaux
      page: 0
      pdf_page: 173
    - "no": 3
      title: Le normalisateur de $W_a$
      page: 0
      pdf_page: 174
    - "no": 4
      title: 'Application : ordre du groupe de Weyl'
      page: 0
      pdf_page: 176
    - "no": 5
      title: Systèmes de racines et groupes engendrés par des réflexions
      page: 0
      pdf_page: 177
statements: 17
exercises: 5
content_sha256: 71513a38f654c602c8a0ba71826e62fad8fc82e47588e08d18d9d1d38bac9ee5
---

## § 2. Groupe de Weyl affine

Dans ce paragraphe (n° 5 excepté), on désigne par R un système de racines réduit dans un espace vectoriel réel V. On désigne par W le groupe de Weyl de R ; on l’identifie à un groupe d’automorphismes du dual V* de V (§ 1, n° 1), et l’on munit V* d’un produit scalaire invariant par W. Soit E l’espace affine sous-jacent à V* ; pour $v \in V^*$, on désigne par $t(v)$ la translation de E de vecteur v. Enfin, on désigne par P (resp. Q ) le groupe des translations $t(v)$ dont le vecteur v appartient au groupe des poids P(R$^\vee$) (resp. au groupe des poids radiciels Q (R$^\vee$)) du système de racines R$^\vee$ inverse de R.

### 1. Groupe de Weyl affine.

Pour $\alpha \in R$ et $k \in \mathbf{Z}$, soit $L_{\alpha, k}$ l’hyperplan de E défini par :

$$
L_{\alpha, k} = \{ x \in E | \langle \alpha, x \rangle = k \}
$$

et soit $s_{\alpha, k}$ la réflexion orthogonale par rapport à $L_{\alpha, k}$. On a :

$$
s_{\alpha, k}(x) = x - (\langle \alpha, x \rangle - k) \alpha^\vee = s_{\alpha, 0}(x) + k \alpha^\vee
$$

pour tout $x \in E$. Autrement dit, on a :

(1)
$$
s_{\alpha, k} = t(k \alpha^\vee) \circ s_\alpha,
$$

où $s_\alpha$ est la réflexion orthogonale par rapport à l’hyperplan $L_\alpha = L_{\alpha, 0}$, c’est-à-dire la réflexion associée à la racine $\alpha$.

La formule (1) montre que $s_{\alpha, k}$ ne dépend pas du produit scalaire choisi.

#### Définition 1 {#lie-vi-s2-def-1 .statement}

On appelle groupe de Weyl affine du système de racines R et on note $W_a(R)$ (ou simplement $W_a$) le groupe de transformations affines de E engendré par les réflexions $s_{\alpha, k}$ pour $\alpha \in R$ et $k \in \mathbf{Z}$.

#### Proposition 1 {#lie-vi-s2-prop-1 .statement}

Le groupe $W_a$ est produit semi-direct de W par Q .

Comme W est engendré par les réflexions $s_\alpha$, il est contenu dans $W_a$. D’autre part, on a $t(\alpha^\vee) = s_{\alpha, 1} \circ s_\alpha$ si $\alpha \in R$, ce qui montre que $Q \subset W_a$.

Comme W laisse stable $Q(R^\vee)$ (§ 1, no 9), le groupe de transformations affines G engendré par W et Q est le produit semi-direct de W par Q. On a $G \subset W_a$ d’après ce qui précède et $s_{\alpha, k} \in G$ quels que soient $\alpha \in \mathbf{R}$ et $k \in \mathbf{Z}$ d’après (1). On en conclut que $W_a = G$.

#### Proposition 2 {#lie-vi-s2-prop-2 .statement}

*Le groupe $W_a$, muni de la topologie discrète, opère proprement sur E et permutte entre eux les hyperplans $L_{\alpha, k}$ (pour $\alpha \in \mathbf{R}$ et $k \in \mathbf{Z}$).*

Comme $Q(R^\vee)$ est un sous-groupe discret de $V^*$, le groupe Q opère proprement sur E. Il en est donc de même de $W_a = W.Q$, puisque W est fini. De plus, on a, pour $\alpha, \beta \in \mathbf{R}$ et $k \in \mathbf{Z}$:

$$
s_\beta(L_{\alpha, k}) = L_{\gamma, k} \quad \text{avec} \quad \gamma = s_\beta(\alpha) \in \mathbf{R}
$$
$$
t(\beta^\vee)(L_{\alpha, k}) = L_{\alpha, k + n(\alpha, \beta)},
$$

où $n(\alpha, \beta) = \langle \beta^\vee, \alpha \rangle$ est un entier, d’où la deuxième assertion.

On peut donc appliquer à $W_a$ opérant sur E les résultats du chapitre V, § 3. Pour éviter toute confusion avec les chambres du groupe de Weyl W dans $V^*$, nous appellerons *alcôves* les chambres déterminées par le système des hyperplans $L_{\alpha, k}$ (pour $\alpha \in \mathbf{R}$ et $k \in \mathbf{Z}$) dans E. *Le groupe $W_a$ opère donc de façon simplement transitive sur l’ensemble des alcôves et l’adhérence d’une alcôve est un domaine fondamental pour $W_a$ opérant sur E* (chap. V, § 3, no 2, th. 1 et no 3, th. 2). Il est clair que le groupe de Weyl W s’identifie à l’image canonique $U(W_a)$ de $W_a$ dans le groupe orthogonal de $V^*$ (cf. chap. V, § 3, no 6). Il en résulte que $W_a$ est *essentiel* (chap. V, § 3, no 7) et que $W_a$ est *irréductible* si et seulement si le système de racines R l’est (§ 1, no 2, cor. de la prop. 5). Si R est irréductible, chaque alcôve est un simplexe ouvert (chap. V, § 3, no 9, prop. 8). Dans le cas général, la décomposition canonique de l’espace affine E en produit (chap. V, § 3, no 8) correspond à la décomposition de R en composants irréductibles. En particulier, les alcôves sont des produits de simplexés ouverts.

Notons encore que le cor. du th. 1 du chap. V, § 3, no 2 montre que les $s_{\alpha, k}$ sont les seules réflexions appartenant à $W_a$.

### 2. Poids et points spéciaux

#### Proposition 3 {#lie-vi-s2-prop-3 .statement}

*Les points spéciaux* (chap. V, § 3, no 10, déf. 1) *de $W_a$ sont les poids de $R^\vee$*.

Soit $x_0 \in E$ et soit $\alpha \in \mathbf{R}$. L’hyperplan L parallèle à Ker $\alpha$ et passant par $x_0$ a pour équation $\langle \alpha, x \rangle = \langle \alpha, x_0 \rangle$. Pour qu’il soit égal à $L_{\beta, k}$, il faut d’une part que $\alpha$ et $\beta$ soient proportionnelles, ou encore, puisque R est réduit, que $\beta = \pm \alpha$, et d’autre part que $\langle \alpha, x_0 \rangle$ soit entier. On en déduit aussitôt que $x_0$ est un point spécial de $W_a$ si et seulement si $\langle \alpha, x_0 \rangle \in \mathbf{Z}$ pour tout $\alpha \in \mathbf{R}$, c’est-à-dire si et seulement si $x_0 \in P(R^\vee)$ (§ 1, no 9).

#### Corollaire {#lie-vi-s2-n2-cor-1 .statement}

(i) *Si $\varpi \in P(R^\vee)$, il existe une alcôve C telle que $\varpi$ soit point extrémal de $\overline{C}$.*

(ii) Si $C$ est une alcôve, $\overline{C} \cap Q(R^\vee)$ se réduit à un point et ce point est point extrémal de $\overline{C}$.

Cela résulte de la prop. 3, compte tenu du cor. de la prop. 11 du chap. V, § 3, no 10 et de la prop. 12 du chap. V, § 3, no 10.

#### Proposition 4 {#lie-vi-s2-prop-4 .statement}

Soit $C'$ une chambre de $R^\vee$.
(i) Il existe une alcôve $C$ et une seule contenue dans $C'$ et telle que $0 \in \overline{C}$.
(ii) La réunion des $w(\overline{C})$ pour $w \in W$ est un voisinage de $0$ dans $E$.
(iii) Tout mur de $C'$ est un mur de $C$.

Cela résulte de la prop. 11 du chap. V, § 3, no 10.

Supposons maintenant $R$ irréductible. Soit $(\alpha_i)_{i \in I}$ une base de $R$ (§ 1, no 5, déf. 3), et soit $(\omega_i)_{i \in I}$ la base duale. Les $\omega_i$ sont les poids fondamentaux de $R^\vee$ pour la chambre $C'$ de $R^\vee$ correspondant à la base $(\alpha_i)$. Soit

$$
\tilde{\alpha} = \sum_{i \in I} n_i \alpha_i
$$

la plus grande racine de $R$ (§ 1, no 8), et soit $J$ l’ensemble des $i \in I$ tels que $n_i = 1$.

#### Proposition 5 {#lie-vi-s2-prop-5 .statement}

Soit $C$ l’alcôve contenue dans $C'$ à laquelle $0$ est adhérent (prop. 4).
(i) $C$ est l’ensemble des $x \in E$ tels que $\langle \alpha_i, x \rangle > 0$ pour tout $i \in I$ et que $\langle \tilde{\alpha}, x \rangle < 1$.
(ii) L’ensemble $\overline{C} \cap P(R^\vee)$ se compose de $0$ et des $\omega_i$ pour $i \in J$.

Soit $D$ l’ensemble des $x \in E$ tels que $\langle \tilde{\alpha}, x \rangle < 1$ et posons $C_1 = C' \cap D$. Comme $0 \in \overline{C}$, on a $C \subset D$, d’où $C \subset C_1$. Nous allons montrer que, pour tout $\alpha \in R$ et tout $k \in \mathbf{Z}$, les ensembles $C$ et $C_1$ sont du même côté de l’hyperplan $L_{\alpha, k}$. Ceci prouvera que $C_1 \subset C$ et établira l’assertion (i). Si $k = 0$, la chambre $C'$ est toute entière d’un même côté de $L_{\alpha, 0}$, ce qui établit notre assertion dans ce cas. Si $k \neq 0$, on peut, quitte à changer $\alpha$ en $-\alpha$, supposer que $k > 0$. On a alors $\langle \alpha, x \rangle < k$ sur $C$, puisque $0 \in \overline{C}$. D’autre part, $\tilde{\alpha} - \alpha$ est positive sur $C'$ (§ 1, no 8, prop. 25). Pour $y \in C_1$, on a donc $\langle \alpha, y \rangle \leq \langle \tilde{\alpha}, y \rangle < 1 \leq k$. Par suite, $C$ et $C_1$ sont bien du même côté de $L_{\alpha, k}$.

Soit maintenant $\omega \in P(R^\vee)$. On a $\omega = \sum_i p_i \omega_i$, avec $p_i \in \mathbf{Z}$ (§ 1, no 10). Pour que $\omega \in \overline{C}'$, il faut et il suffit que les entiers $p_i$ soient tous positifs. Si $\omega \in \overline{C}'$, pour que $\omega \in \overline{C}$ il faut et il suffit que $\langle \tilde{\alpha}, \omega \rangle = \sum_i n_i p_i$ soit $\leq 1$, d’où (ii).

#### Corollaire {#lie-vi-s2-n2-cor-2 .statement}

L’alcôve $C$ est un simplexe ouvert de sommets $0$ et les $\omega_i / n_i, i \in I$.
Cela résulte de (i).

### 3. Le normalisateur de $W_a$

Dans ce no, nous supposons le produit scalaire choisi sur $V$ invariant non seulement par $W$, mais par le groupe $A(R)$ tout entier. Nous identifierons $A(R)$ et $A(R^\vee)$.

Soit G le normalisateur de $W_a$ dans le groupe des déplacements de l’espace affine euclidien E. Si $g$ est un déplacement de E, et $s$ la réflexion orthogonale par rapport à un hyperplan L, le déplacement $g s g^{-1}$ est la réflexion orthogonale par rapport à l’hyperplan $g(L)$. Il en résulte que G est l’ensemble des déplacements de E qui permutent entre eux les hyperplans $L_{\alpha, k}$ (pour $\alpha \in \mathbf{R}$ et $k \in \mathbf{Z}$).

Or, le groupe des automorphismes de E est le produit semi-direct du groupe orthogonal U de V* et du groupe T des translations. Si $u \in U$ et $v \in V^*$, le transformé de l’hyperplan $L_{\alpha, k}$ par $g = u \circ t(v)$ est l’hyperplan défini par l’équation
$$
\langle t u^{-1}(\alpha), x \rangle = k + \langle \alpha, v \rangle.
$$
Par suite, on a $g \in G$ si et seulement si d’une part $t u$ permutte entre elles les racines, c’est-à-dire appartient à $A(\mathbf{R})$, d’autre part $\langle \alpha, v \rangle \in \mathbf{Z}$ pour tout $\alpha \in \mathbf{R}$, c’est-à-dire si $v \in P(R^\vee)$. Autrement dit, le groupe G est produit semi-direct de $A(\mathbf{R})$ par P. Comme $Q \subset P$ et $W \subset A(\mathbf{R})$, on voit que le groupe quotient $G/W_a$ est produit semi-direct de $A(\mathbf{R})/W$ par $P(R^\vee)/Q(R^\vee)$; l’action correspondante de $A(\mathbf{R})/W$ sur $P(R^\vee)/Q(R^\vee)$ est l’action canonique (§ 1, no 9), comme on le vérifie immédiatement.

Nous désignerons par $W'_a$ le sous-groupe de G produit semi-direct de W par P. C’est un sous-groupe distingué de G, et $G/W'_a$ est canoniquement isomorphe à $A(\mathbf{R})/W$; de plus, l’application canonique de $P(R^\vee)$ dans $W'_a/W_a$ donne par passage au quotient un isomorphisme de $P(R^\vee)/Q(R^\vee)$ sur $W'_a/W_a$.

Soit maintenant C une alcôve de E, et soit $G_C$ le sous-groupe formé des éléments $g \in G$ tels que $g(C) = C$. Comme $W_a$ est simplement transitif sur les alcôves, le groupe G est produit semi-direct de $G_C$ et de $W_a$. L’isomorphisme correspondant de $G/W_a$ sur $G_C$ fournit en particulier un isomorphisme canonique de $P(R^\vee)/Q(R^\vee)$ sur le groupe $\Gamma_C = G_C \cap W'_a$.

Supposons que R soit irréductible, et reprenons les notations de la prop. 5 du no 2. Posons $R_0 = R$, et soit $R_i$ ($i \in I$) le système de racines engendré par les $\alpha_j$, pour $j \neq i$. Pour $i = 0$ (resp. $i \in I$), soit $w_i$ l’unique élément de $W(R_i)$ (identifié à un sous-groupe de W) qui transforme les racines positives de $R_i$ relativement à la base $(\alpha_j)_{j \neq i}$ en racines négatives (§ 1, no 6, cor. 3 de la prop. 17).

#### Proposition 6 {#lie-vi-s2-prop-6 .statement}

Pour tout $i \in J$, l’élément $\gamma_i = t(\overline{\omega}_i) w_i w_0$ appartient à $\Gamma_C$ et l’application $i \mapsto \gamma_i$ est une bijection de J sur $\Gamma_C - \{1\}$.

Remarquons tout d’abord que la racine $w_i(\tilde{\alpha})$ est de la forme
$$
n_i \alpha + \sum_{j \neq i} b_{ij} \alpha_j,
$$
donc est positive.

Montrons que, si $i \in J$, on a $\gamma_i \in \Gamma_C$. Soient en effet $a \in C$ et $b = \gamma_i(a)$.

n° 2.4.

Pour $1 \leq j \leq l$ et $j \neq i$, on a :

(2)
$$
\langle b, \alpha_j \rangle = \langle \overline{\omega}_i + w_i w_0(a), \alpha_j \rangle \\
= \langle w_0(a), w_i(\alpha_j) \rangle > 0
$$
puisque $w_0(a) \in -\mathbf{C}'$ et que $w_i(\alpha_j)$ est négative. D’autre part, on a :
(3)
$$
\langle b, \alpha_i \rangle = 1 + \langle w_0(a), w_i(\alpha_i) \rangle \geq 1 + \langle w_0(a), \tilde{\alpha} \rangle > 0
$$
puisque $w_0(a) \in -\mathbf{C}'$, que $\tilde{\alpha} - w_i(\alpha_i)$ prend des valeurs négatives sur $-\mathbf{C}'$ et que $\langle w_0(a), \tilde{\alpha} \rangle > -1$. Enfin, on a :
(4)
$$
\langle b, \tilde{\alpha} \rangle = n_i + \langle w_0(a), w_i(\tilde{\alpha}) \rangle = 1 + \langle w_0(a), w_i(\tilde{\alpha}) \rangle < 1
$$
puisque $w_0(a) \in -\mathbf{C}'$ et que $w_i(\tilde{\alpha})$ est une racine positive. Les relations (2), (3) et (4) entraînent alors que $b \in \mathbf{C}$, d’où $\gamma_i \in \Gamma_C$. Il est clair que l’application $i \mapsto \gamma_i$ est injective, puisque $\gamma_i(0) = \overline{\omega}_i$. Enfin, soit $\gamma \in \Gamma_C$, avec $\gamma \neq 1$ et posons $\gamma = t w$, avec $t \in \mathbf{P}$ et $w \in W$. On a $t \neq 1$ puisque $\Gamma_C \cap W = \{1\}$. D’autre part, on a $t(0) = \gamma(0) \in \overline{\mathbf{C}} \cap \mathbf{P}(R^\vee)$ et la prop. 5 entraîne qu’il existe $i \in J$ tel que $t(0) = \overline{\omega}_i$. On a alors $\gamma_i^{-1} \gamma(0) = 0$, d’où $\gamma = \gamma_i$ puisque $\Gamma_C \cap W = \{1\}$. Ceci achève la démonstration.

#### Corollaire {#lie-vi-s2-n3-cor-1 .statement}

Les $(\overline{\omega}_i)_{i \in J}$ forment un système de représentants dans $\mathbf{P}(R^\vee)$ des éléments non nuls de $\mathbf{P}(R^\vee)/\mathbf{Q}(R^\vee)$.

En effet, si l’on identifie $\Gamma_C$ à $\mathbf{P}(R^\vee)/\mathbf{Q}(R^\vee)$, l’élément $\gamma_i$ est transformé en la classe de $\overline{\omega}_i$ mod. $\mathbf{Q}(R^\vee)$.

#### Remarque 1 {#lie-vi-s2-n3-rem-1 .statement}

L’application $\gamma \mapsto \gamma(0)$ est une bijection de $\Gamma_C$ sur $\overline{\mathbf{C}} \cap \mathbf{P}(R^\vee)$.

#### Remarque 2 {#lie-vi-s2-n3-rem-2 .statement}

Le groupe $G$ est aussi le normalisateur de $W_a$ dans le groupe des automorphismes de $E$ muni seulement de sa structure affine (cf. exerc. 3).

### 4. Application : ordre du groupe de Weyl

#### Lemme 1 {#lie-vi-s2-lem-1 .statement}

Soient $X$ un espace localement compact dénombrable à l’infini, $G$ un groupe discret opérant continûment et proprement dans $X$, $\mu$ une mesure $\geq 0$ sur $X$ invariante par $G$, $G'$ un sous-groupe de $G$, $U$ et $U'$ deux parties ouvertes de $X$ de mesures finies $\neq 0$. On suppose que les $sU$ pour $s \in G$ (resp. les $s'U'$ pour $s' \in G'$) sont deux à deux disjoints et que leur réunion est de complémentaire négligeable. Alors $G'$ est d’indice fini dans $G$ et l’on a $(G : G') = \mu(U')/\mu(U)$.

Soit $(s_\lambda)_{\lambda \in \Lambda}$ une famille de représentants des classes à droite de $G$ suivant $G'$. Soit $U_1$ la réunion des $s_\lambda U$. Alors les $s'U_1$, pour $s' \in G'$, sont deux à deux disjoints et de réunion $M = \bigcup_{s \in G} sU$. Soit $M' = \bigcup_{s' \in G'} s'U'$. La réunion de $U'$ (resp. $U_1$) et d’une partie convenable de $X - M'$ (resp. $X - M$) est un domaine fondamental, évidemment $\mu$-mesurable, pour $G'$. D’après Intégr., chap. VII, § 2, n° 10, cor. du th. 4, on a $\mu(U') = \mu(U_1)$. Ceci prouve que Card $\Lambda = (G : G')$ est fini, et que $\mu(U') = (\text{Card } \Lambda)\mu(U)$.

#### Proposition 7 {#lie-vi-s2-prop-7 .statement}

*Supposons R irréductible. Soient B = \{ \alpha_1, \ldots, \alpha_l \} une base de R, f l’indice de connexion de R (§ 1, n° 9) et $\tilde{\alpha} = n_1 \alpha_1 + \cdots + n_l \alpha_l$ la plus grande racine de R (pour l’ordre défini par B). Alors l’ordre de W est égal à*

$$
(l!) n_1 n_2 \ldots n_l f.
$$

Soit $(\overline{\omega}_1, \ldots, \overline{\omega}_l)$ la base de $P(R^\vee)$ duale de B. D’après le cor. de la prop. 5, le simplexe ouvert C de sommets 0, $n_1^{-1} \overline{\omega}_1, \ldots, n_l^{-1} \overline{\omega}_l$ est une alcôve de E. Choisissons une mesure de Haar $\mu$ sur le groupe additif V*. Soit A l’ensemble des éléments de V* de la forme $\xi_1 \overline{\omega}_1 + \cdots + \xi_l \overline{\omega}_l$, avec $0 < \xi_i < 1$ pour $i = 1, \ldots, l$. D’après le cor. 2 de la prop. 15 de Intégr., chap. VII, § 1, n° 10, on a:

(5)
$$
\mu(A)/\mu(C) = (l!) n_1 n_2 \ldots n_l.
$$

Soit d’autre part $A'$ l’ensemble des éléments de V* de la forme

$$
\xi_1 \alpha_1^\vee + \cdots + \xi_l \alpha_l^\vee,
$$

avec $0 < \xi_i < 1$ pour $i = 1, \ldots, l$. Comme $(\alpha_1^\vee, \ldots, \alpha_l^\vee)$ est une base du $\mathbf{Z}$-module $Q(R^\vee)$, on peut appliquer le lemme 1 avec $X = V^*$, $G = W_a$, $G' = Q$, $U = C$ et $U' = A'$. On obtient:

(6)
$$
\mu(A')/\mu(C) = (W_a : Q) = \text{Card } W.
$$

Enfin, on peut appliquer une autre fois le lemme 1, en prenant $X = V^*$, $G = P$, $G' = Q$, $U = A$ et $U' = A'$. On obtient:

(7)
$$
\mu(A')/\mu(A) = (P : Q) = (P(R^\vee) : Q(R^\vee)) = f.
$$

La proposition résulte alors de la comparaison des formules (5), (6) et (7).

### 5. Systèmes de racines et groupes engendrés par des réflexions

#### Proposition 8 {#lie-vi-s2-prop-8 .statement}

*Soit F un espace hilbertien réel de dimension finie l. Soient $\mathcal{H}$ un ensemble d’hyperplans affines de F et G le groupe engendré par les réflexions orthogonales $s_H$ par rapport aux hyperplans $H \in \mathcal{H}$. On suppose que les conditions du chap. V, § 3 sont vérifiées (i.e. que $g(H) \in \mathcal{H}$ pour tout $H \in \mathcal{H}$ et $g \in G$, et que G opère proprement dans F). On suppose de plus que 0 est point spécial pour G et que le groupe T des translations appartenant à G est de rang l. Il existe alors un système de racines réduit R et un seul dans $V = F^*$ tel que l’isomorphisme canonique de F sur $V^*$ transforme G en le groupe de Weyl affine $W_a$ de R.*

Remarquons tout d’abord que l’hypothèse faite sur T entraîne que G est essentiel : sinon, l’espace affine F se décomposerait en produit $F_0 \times F_1$, avec $\dim F_1 < l$, le groupe G s’identifiant à un groupe de déplacements opérant proprement dans $F_1$ (chap. V, § 3, no 8, prop. 6), et T ne serait pas de rang $l$.

Soit $\mathfrak{H}_0$ l’ensemble des $H \in \mathfrak{H}$ tels que $0 \in H$. Pour $H \in \mathfrak{H}_0$, soit $\mathfrak{H}_H$ l’ensemble des éléments de $\mathfrak{H}$ parallèles à H. Puisque 0 est point spécial, $\mathfrak{H}$ est la réunion des $\mathfrak{H}_H$ pour $H \in \mathfrak{H}_0$. Soit $H \in \mathfrak{H}_0$. Puisque T est de rang $l$, il existe un $v \in F$ tel que la translation de vecteur $v$ appartienne à T et que $v \notin H$. Les hyperplans $H + kv$ pour $k \in \mathbf{Z}$ sont deux à deux distincts et appartiennent à $\mathfrak{H}_H$. Soit alors $a$ un vecteur unitaire de F orthogonal à H : on a $H + (v|a)a \in \mathfrak{H}_H$ et comme $\mathfrak{H}$ est localement fini (chap. V, § 3, no 1, lemme 1), il existe un plus petit nombre réel $\lambda > 0$ tel que $H + \lambda a \in \mathfrak{H}_H$. Nous allons montrer que $\mathfrak{H}_H$ est l’ensemble des hyperplans $H + k\lambda a$ pour $k \in \mathbf{Z}$. En effet,

$$
H' = H + \lambda a \in \mathfrak{H}_H
$$

et l’élément $s_{H'} \circ s_H$ de G est la translation de vecteur $2\lambda a$ (chap. V, § 2, no 4, prop. 5). Par suite, $H + 2n\lambda a = (s_{H'} s_H)^n(H)$ et $H + (2n+1)\lambda a = (s_{H'} s_H)^n(H')$ appartiennent à $\mathfrak{H}_H$. D’autre part, si $L \in \mathfrak{H}_H$, il existe $\xi \in \mathbf{R}$ tel que $L = H + \xi \lambda a$ et il existe un entier $n$ tel que

ou bien $2n < \xi \leq 2n + 1$, ou bien $2n - 1 < \xi \leq 2n$.

Dans le premier cas, on a $(s_H s_{H'})^n(L) = H + (\xi - 2n)\lambda a$ avec

$$
0 < (\xi - 2n)\lambda \leq \lambda
$$

et la définition de $\lambda$ entraîne $\xi = 2n + 1$; dans le second cas, on a

$$
s_H (s_H s_{H'})^n(L) = H + (2n - \xi)\lambda a \quad \text{avec} \quad 0 \leq (2n - \xi)\lambda < \lambda
$$

et la définition de $\lambda$ entraîne que $\xi = 2n$.

Il en résulte que si $\alpha_H$ est la forme linéaire sur F telle que

$$
H' = \{ x \in F | \langle \alpha_H, x \rangle = 1 \},
$$

l’ensemble $\mathfrak{H}_H$ est l’ensemble des hyperplans $L_{\alpha_H, k} = \{ x \in F | \langle \alpha_H, x \rangle = k \}$ pour $k \in \mathbf{Z}$, et les formes linéaires $\alpha_H$ et $-\alpha_H$ sont les seules à posséder cette propriété.

Par suite, la proposition sera démontrée si nous montrons que l’ensemble R des éléments de V de la forme $\pm \alpha_H$ est un système de racines réduit dans V.

a) Démontrons la condition (SR₁) : il est clair que R est fini (puisque $\mathfrak{H}_0$ est fini) et ne contient pas 0. De plus, R engendre V. En effet, si $x \in F$ est orthogonal à R, on a $x \in H$ pour tout $H \in \mathfrak{H}_0$ et la translation de vecteur $x$ commute avec tout élément de G. Comme G est essentiel, ceci entraîne $x = 0$.

b) Démontrons (SR_{II}). Pour $v \in V$ et $r \in \mathbf{R}$, posons comme précédemment $L_{v,r} = \{ x \in F | \langle v, x \rangle = r \}$; si $\alpha \in \mathbf{R}$, posons $H_\alpha = L_{\alpha,0}$, et soit $s_\alpha$ le transposé de $s_{H_\alpha}$. Il existe un élément $\alpha^\vee \in F$ et un seul orthogonal à $H_\alpha$ et tel que $\langle \alpha^\vee, \alpha \rangle = 2$. On a alors $s_{H_\alpha} = s_{\alpha^\vee,\alpha}$ et $s_\alpha = s_{\alpha,\alpha^\vee}$. Pour $\beta \in \mathbf{R}$, on a
$$
L_{s_{\alpha(\beta)},1} = s_{H_\alpha}(L_{\beta,1}) \in \mathfrak{H}
$$
et il existe $\gamma \in \mathbf{R}$ et $n \in \mathbf{N}^*$ tels que $L_{s_{\alpha(\beta)},1} = L_{\gamma,n}$. On a alors
$$
s_{H_\alpha}(L_{\gamma,1}) = L_{\beta,1/n}
$$
et par suite $1/n \in \mathbf{Z}$. On a donc $n = 1$ et $s_\alpha(\beta) = \gamma \in \mathbf{R}$. Ceci démontre (SR_{II}).

c) Démontrons (SR_{III}). Soit $\alpha \in \mathbf{R}$ et posons $H'_\alpha = L_{\alpha,1}$. On a
$$
H'_\alpha = H_\alpha + (1/2)\alpha^\vee;
$$
comme la translation $t(\alpha^\vee)$ de vecteur $\alpha^\vee$ est le produit $s_{H'_\alpha}s_{H_\alpha}$ (chap. V, § 2, no 4, prop. 5), elle appartient à T et $\alpha^\vee = t(\alpha^\vee)(0)$ est un *point spécial* pour G. Par suite, pour tout $\beta \in \mathbf{R}$, il existe un hyperplan $L_{\beta,k}$ passant par $\alpha^\vee$, avec $k$ entier, ce qui démontre que $\langle \beta, \alpha^\vee \rangle \in \mathbf{Z}$, c’est-à-dire (SR_{III}).

d) Enfin, il est évident que R est *réduit*, car si $H, H' \in \mathfrak{H}_0, H \neq H'$, les formes linéaires $\alpha_H$ et $\alpha_{H'}$ ne sont pas proportionnelles.

Remarque 1). — L’hypothèse que T est de rang l est en particulier vérifiée lorsque G est *irréductible et infini*. En effet l’espace vectoriel engendré par les vecteurs des translations de T est invariant par l’image canonique de G dans le groupe linéaire de F. Il est différent de $\{0\}$ si G est infini et est donc égal à F tout entier si G est infini et irréductible.

Un groupe fini engendré par des réflexions n’est pas toujours le groupe de Weyl d’un système de racines. Plus précisément :

#### Proposition 9 {#lie-vi-s2-prop-9 .statement}

*Soit V un espace vectoriel réel de dimension finie l, et soit G un sous-groupe fini de $\mathbf{GL}(V)$, engendré par des réflexions et essentiel. Munissons V d’un produit scalaire invariant par G. Les conditions suivantes sont équivalentes :*

(i) *Il existe un sous-groupe discret de rang l de V stable par G.*
(ii) *Il existe une $\mathbf{Q}$-structure sur V* (Alg., chap. II, 3e éd., § 8, no 1, déf. 1) *invariante par G.*
(iii) *Il existe un système de racines dans V dont le groupe de Weyl est G.*
(iv) *Il existe un groupe discret G’ de déplacements de V, opérant proprement dans V, engendré par des réflexions, tel que G’ soit produit semi-direct de G et d’un groupe de translations de rang l.*

(ii) $\Longrightarrow$ (i) : soit $V' \subset V$ une $\mathbf{Q}$-structure sur V invariante par G. Soit A une partie finie de $V'$ engendrant le $\mathbf{Q}$-espace vectoriel $V'$. En remplaçant A par $\bigcup_{s \in G} s(A)$, on peut supposer A stable par G. Soit B le sous-groupe de V engendré par A. Alors B est stable par G, de type fini et sans torsion, donc admet une base sur $\mathbf{Z}$ qui est en même temps une base de $V'$ sur $\mathbf{Q}$, donc une base de $V$ sur $\mathbf{R}$.

(iii) $\Longrightarrow$ (ii) : ceci résulte par exemple de la prop. 1 du § 1, no 1.

(iv) $\Longrightarrow$ (iii) : soit $G'$ un groupe vérifiant la condition (iv). Le groupe des translations de $G'$ est de rang $l$, et 0 est point spécial pour $G'$ d’après la prop. 9 du chap. V, § 3, no 10. La prop. 8 montre qu’il existe un système de racines réduit $R_0$ dans $V^*$ tel que $G'$ s’identifie à $W_a(R_0)$; le groupe $G$ est alors le groupe de Weyl du système de racines inverse de $R_0$.

(i) $\Longrightarrow$ (iv) : supposons que $G$ laisse stable un sous-groupe discret $M$ de $V$, de rang $l$. Munissons $V$ d’un produit scalaire invariant par $G$. Pour toute réflexion $s \in G$, on a $s(x) — x \in M$ quel que soit $x \in M$, donc la droite $D_s$ orthogonale à $H_s$ rencontre $M$; soient $\alpha_s, — \alpha_s$ les générateurs du groupe cyclique $D_s \cap M$. L’ensemble $A$ des $\alpha_s$ et des $— \alpha_s$ est stable par $G$, donc engendre un sous-groupe $M'$ de $M$ stable par $G$; le groupe discret $M'$ est de rang $l$ parce que $G$ est essentiel. Soit $G'$ le groupe de transformations affines de $V$ produit semi-direct de $G$ et du groupe des translations dont les vecteurs appartiennent à $M'$. Soit $G'_1$ le sous-groupe de $G'$ engendré par les réflexions de $G'$. On va montrer que $G'_1 = G'$, ce qui achèvera la démonstration. D’abord, $G'_1 \supseteq G$ puisque $G$ est engendré par des réflexions. D’autre part, pour toute réflexion $s$ de $G$, soit $t_s$ la translation de vecteur $\alpha_s$. La transformation $s \circ t_s$ est une réflexion, et $s \circ t_s \in G'$; donc $t_s$ est un produit de deux réflexions de $G'$; ceci étant vrai pour toute réflexion $s$ de $G$, les translations dont le vecteur appartient à $M'$ sont toutes dans $G'_1$.

#### Définition 2 {#lie-vi-s2-def-2 .statement}

Un groupe $G$ vérifiant les conditions équivalentes de la prop. 9 est appelé un groupe cristallographique.

Remarque 2). — Soit $G$ un groupe fini engendré par des réflexions et essentiel. Pour que $G$ soit cristallographique, il faut et il suffit que tout élément de sa matrice de Coxeter soit l’un des entiers 1, 2, 3, 4, 6. En effet, cette condition est nécessaire d’après la Remarque 3) du § 1, no 5. Le fait qu’elle soit suffisante résultera de la classification des groupes de Coxeter finis donnée au § 4 (pour une démonstration directe, voir chap. V, § 4, exerc. 6).

## EXERCICES {#lie-vi-s2-exercises}

On désigne par R un système de racines réduit dans un espace vectoriel réel V.

See the [exercises for § 2](exercises/s2/).
