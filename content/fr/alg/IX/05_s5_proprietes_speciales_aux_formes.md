---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 5
section_title: Propriétés spéciales aux formes bilinéaires alternées
lang: fr
source: alg-ix-fr
pdf_pages: 0077-0087
extraction: ocr
subsections:
    - "no": 1
      title: Réduction des formes bilinéaires alternées.
      page: 0
      pdf_page: 77
    - "no": 2
      title: Pfaffien d'une matrice alternée.
      page: 0
      pdf_page: 80
    - "no": 3
      title: Groupe symplectique.
      page: 0
      pdf_page: 82
statements: 11
exercises: 0
content_sha256: 693e6fdc19755fda00825e8c7dc2e818b1c457da08c603a8d654e97e5a9f7eb2
---

## § 5. Propriétés spéciales aux formes bilinéaires alternées

### 1. Réduction des formes bilinéaires alternées.

#### Théorème 1 {#alg-ix-s5-thm-1 .statement}

Soient $A$ un anneau (commutatif) principal, $E$ un $A$-module libre de dimension finie $n$ et $\Phi$ une forme bilinéaire alternée sur $E$. Alors il existe une base $(e_i)_{1 \leq i \leq n}$ de $E$ et un entier pair $2r \leq n$, tels que

$1^o$ $\Phi(e_1, e_2) = \alpha_1, \Phi(e_3, e_4) = \alpha_2, \ldots, \Phi(e_{2r-1}, e_{2r}) = \alpha_r$

où les $\alpha_i$ sont des éléments $\neq 0$ de $A$, et où $\alpha_i$ divise $\alpha_{i+1}$ pour $i = 1, \ldots, r-1$.

$2^o$ Tous les autres éléments $\Phi(e_i, e_j)$ où $i \leq j$ sont nuls.

Les idéaux $A \alpha_i$ ($i = 1, \ldots, r$) sont uniquement déterminés par les conditions précédentes. Le sous-module $E^0$ de $E$ orthogonal à $E$ est engendré par $e_{2r+1}, \ldots, e_n$.

Nous procéderons par récurrence sur la dimension $n$ de $E$. Le théorème est évident pour $n = 0$. Si $\Phi = 0$, le théorème est évident aussi ; on peut donc supposer $\Phi \neq 0$. Notons $f$ l’application linéaire $d_\Phi$ de $E$ dans $E^*$ associée à droite à $\Phi$ ($\S 1$, no 1); alors $f(E)$ est un sous-module non réduit à 0 du module $E^*$, qui est un module libre de dimension $n$. Soit $A\alpha_1$ le plus grand facteur invariant de $f(E)$ par rapport à $E^*$ (chap. VII, $\S 4$, no 2, th. 1); on sait (*loc. cit.*) qu’il existe une base $(e'_1, a'_2, \ldots, a'_n)$ de $E^*$ et un élément $f(e_2) \in f(E)$ tels que $f(e_2) = \alpha_1 e'_1$. Soit $(e_1, a_2, \ldots, a_n)$ la base de $E$ (identifié au bidual $E^{**}$) duale de $(e'_1, a'_2, \ldots, a'_n)$; on a

$$
\Phi(e_1, e_2) = -\Phi(e_2, e_1) = \langle e_1, f(e_2) \rangle = \alpha_1.
$$

Soit $P$ le sous-module $Ae_1 + Ae_2$ de $E$. Nous allons voir que $E$ est *somme directe* de $Ae_1, Ae_2$ et du sous-module $P^0$ orthogonal de $P$. Il suffit pour cela de prouver que, pour tout $x \in E$, il existe des éléments $\xi_1, \xi_2$ de $A$, déterminés de façon unique et tels que $x - \xi_1 e_1 - \xi_2 e_2 \in P^0$, c’est-à-dire tels que

$$
\Phi(e_1, x - \xi_1 e_1 - \xi_2 e_2) = 0, \qquad \Phi(e_2, x - \xi_1 e_1 - \xi_2 e_2) = 0.
$$

D’après (1) ces conditions s’écrivent

$$
\langle e_1, f(x) \rangle = \xi_2 \alpha_1, \langle e_2, f(x) \rangle = -\xi_1 \alpha_1.
$$

Mais on sait (*loc. cit.*) que l’image de $f(E)$ par toute forme linéaire sur $E^*$ est contenue dans l’idéal $A\alpha_1$, autrement dit toutes les valeurs $\Phi(x, y) = \langle x, f(y) \rangle$ appartiennent à $A\alpha_1$; d’où l’existence et l’unicité de $\xi_1$ et $\xi_2$. Ainsi $P^0$ est un module libre de rang $n-2$; il existe donc, dans $P^0$, d’après l’hypothèse de récurrence, une base $(e_3, e_4, \ldots, e_n)$ satisfaisant aux conditions de l’énoncé. Pour montrer que la base $(e_1, \ldots, e_n)$ de $E$ ainsi obtenue satisfait aussi à ces conditions, il suffit de prouver que $\alpha_1$ divise $\alpha_2$; or cela résulte de ce que toutes les valeurs $\Phi(x, y)$ sont des multiples de $\alpha_1$. Il est alors clair que $e_{2r+1}, \ldots, e_n$ engendrent $E^0$. Enfin, si $(e'_i)$ est la base duale de $(e_i)$, on a $f(e_{2j-1}) = -\alpha_j e'_{2j}$ et $f(e_{2j}) = \alpha_j e'_{2j}$ pour $j = 1, \ldots, r$ et $f(e_k) = 0$ pour $k = 2r+1, \ldots, n$; les idéaux $A\alpha_1, A\alpha_1, A\alpha_2, A\alpha_2, \ldots, A\alpha_r, A\alpha_r$ sont donc les facteurs invariants de $f(E)$ par rapport à $E^*$, ce qui démontre leur unicité (chap. VII, $\S 4$, no 2, th. 1).

#### Corollaire 1 {#alg-ix-s5-thm-1-cor-1 .statement}

*Soient $A$ un corps commutatif, $E$ un espace vectoriel de dimension finie $n$ sur $A$, et $\Phi$ une forme bilinéaire alternée sur E. Il existe alors une base $(e_i)_{1 \leq i \leq n}$ de E et un entier pair $2r \leq n$ tels que

$$
\Phi\left( \sum_{i=1}^n \xi_i e_i, \sum_{i=1}^n \eta_i e_i \right) = \sum_{j=1}^r (\xi_{2j-1} \eta_{2j} - \xi_{2j} \eta_{2j-1}).
$$

En particulier $\Phi$ est de rang pair $2r$.

Une base vérifiant (2) est dite base symplectique pour $\Phi$.

#### Remarque {#alg-ix-s5-n1-rem-1 .statement}

On notera que ce corollaire est aussi une conséquence immédiate de la prop. 3 du § 4, n° 2 et de son cor. 1, car avec les notations de cette proposition, on a nécessairement $H = \{0\}$ puisque $\Phi$ est alternée.

#### Corollaire 2 {#alg-ix-s5-thm-1-cor-2 .statement}

Soient A un corps commutatif, E un espace vectoriel de dimension finie n sur A. Pour tout bivecteur $z \in \bigwedge^2 E$, il existe une base $(e_i)_{1 \leq i \leq n}$ de E telle que

$$
z = e_1 \wedge e_2 + e_3 \wedge e_4 + \cdots + e_{2r-1} \wedge e_{2r} \quad (2r \leq n).
$$

Il suffit en effet de remarquer que z s’identifie canoniquement à une forme bilinéaire alternée sur $E^*$ (chap. III, § 8, n° 2), et d’appliquer le cor. 1 à cette forme.

En traduisant le cor. 1 en langage matriciel, on obtient :

#### Corollaire 3 {#alg-ix-s5-thm-1-cor-3 .statement}

Soient A un corps commutatif, R une matrice carrée alternée sur A. Le rang de R est un nombre pair $2r$, et il existe une matrice inversible P sur A telle que

$$
{}^tP.R.P = \begin{pmatrix}
0 & I_r & 0 \\
-I_r & 0 & 0 \\
0 & 0 & 0
\end{pmatrix}.
$$

#### Remarque {#alg-ix-s5-n1-rem-2 .statement}

Si A est un anneau commutatif quelconque et R une matrice carrée alternée d’ordre impair n sur A, on a det $R = 0$. Ceci résulte du cor. 3 lorsque A est un corps. Une démonstration directe dans le cas où A est un corps de caractéristique $\neq 2$ est la suivante : comme ${}^tR = -R$, on a det $R = \det {}^tR = (-1)^n \det R$, d’où $2 \det {}^tR = 0$. Ceci étant, puisque le déterminant d’une matrice alternée $(\alpha_{ij})$ est un polynôme à coefficients entiers par rapport aux $\alpha_{ij}$ tels que $i < j$, le principe de prolongement des identités algébriques (chap. IV, § 2, no 5, Scholie) montre alors que notre assertion est vraie pour un anneau commutatif arbitraire A.

### 2. Pfaffien d'une matrice alternée.

Soient A un corps commutatif de caractéristique 0, et $R = (\alpha_{ij})$ une matrice alternée d'ordre pair $2m$ sur A. Désignons par E l'espace vectoriel $A^{2m}$, par $(e_i)$ ($i = 1, \ldots, 2m$) sa base canonique, et par e l'élément $e_1 \wedge e_2 \wedge \ldots \wedge e_{2m}$ de $\wedge^2 E$. La puissance extérieure $m$-ième du bivecteur $u = \sum_{i < j} \alpha_{ij} e_i \wedge e_j \in \wedge^2 E$ est de la forme $\alpha . e$, où $\alpha$ est un élément de A que nous allons calculer. L'élément $\wedge^m u$ est une somme de termes de la forme
$$
\alpha_{h_1 k_1} \alpha_{h_2 k_2} \cdots \alpha_{h_m k_m} e_{h_1} \wedge e_{k_1} \wedge e_{h_2} \wedge e_{k_2} \wedge \ldots \wedge e_{h_m} \wedge e_{k_m}
$$
avec $h_j < k_j$ pour $j = 1, \ldots, m$. Un tel terme est nul s'il y figure deux $e_j$ égaux, c'est-à-dire si l'ensemble $\{ h_1, k_1, \ldots, h_m, k_m \}$ n'est pas exactement $\{ 1, 2, \ldots, 2m \}$. En outre, si, dans (3), on échange simultanément $e_{h_r}$ et $e_{h_{r+1}}$ d'une part, $e_{k_r}$ et $e_{k_{r+1}}$ d'autre part, le produit ne change pas ; il ne change donc pas par toute permutation effectuée sur les couples $(h_1, k_1), \ldots, (h_m, k_m)$. Considérons alors les ensembles (et non les suites) $S = \{ (h_1, k_1), \ldots, (h_m, k_m) \}$ de couples $(h_j, k_j)$ tels que $1 \leq h_j < k_j \leq 2m$ pour $j = 1, 2, \ldots, m$; soit $\mathcal{S}$ l'ensemble de ces couples. Pour $S \in \mathcal{S}$, posons
1°) $\varepsilon(S) = 0$ si $\{ h_1, k_1, \ldots, h_m, k_m \} \neq \{ 1, 2, \ldots, 2m \}$;
2°) dans le cas contraire, $\varepsilon(S) = 1$ ou $\varepsilon(S) = -1$ suivant que la permutation qui applique $h_j$ sur $2j-1$ et $k_j$ sur $2j$ ($j = 1, \ldots, m$) est paire ou impaire.

Les remarques précédentes prouvent alors que $\wedge^m u$ est égal à
$$
m! \sum_{S \in \mathcal{S}} \varepsilon(S) (\prod_{(h, k) \in S} \alpha_{hk}) e.
$$

Introduisons alors $m(2m-1)$ indéterminées $X_{hk}$ indexées au moyen des couples $(h, k)$ tels que $1 \leq h < k \leq 2m$, et appelons P le polynôme sur $\mathbf{Z}$ par rapport aux $X_{hk}$, défini par
$$
P((X_{hk})) = \sum_{S \in \mathcal{S}} \varepsilon(S) (\prod_{(h, k) \in S} X_{hk}).
$$

On a donc

(6) $\bigwedge^m u = m! \mathrm{P}((\alpha_{hk})) . e.$

#### Définition 1 {#alg-ix-s5-def-1 .statement}

Etant donnée une matrice alternée $R = (\alpha_{ij})$ $(i, j = 1, \ldots, 2m)$ d’ordre pair $2m$ sur un anneau commutatif quelconque $A$, on appelle pfaffien de $R$, et on note $\mathrm{Pf}(R)$, l’élément $\mathrm{P}((\alpha_{hk}))$ de $A$, où $1 \leq h < k \leq 2m$.

#### Exemple {#alg-ix-s5-n2-exa-1 .statement}

Supposons :

$\alpha_{12} = -\alpha_{21} = \beta_1, \alpha_{34} = -\alpha_{43} = \beta_2, \ldots, \alpha_{2m-1, 2m} = -\alpha_{2m, 2m-1} = \beta_m,$

tous les autres $\alpha_{ij}$ étant nuls (cf. th. 1). Alors le pfaffien de $R = (\alpha_{ij})$ est $\beta_1 \beta_2 \ldots \beta_m$.

#### Proposition 1 {#alg-ix-s5-prop-1 .statement}

Soient $R$ une matrice alternée d’ordre pair $2m$ sur un anneau commutatif $A$, et $P$ une matrice carrée d’ordre $2m$ sur $A$. On a

(7) $\mathrm{Pf}({}^t P . R . P) = (\det P) \mathrm{Pf}(R).$

En effet, supposons d’abord que $A$ soit un corps de caractéristique 0 et posons $R = (\alpha_{ij}), P = (\beta_{st})$. Associons à $R$ le bivecteur

$$ u = \sum_{i < j} \alpha_{ij} e_i \wedge e_j = \frac{1}{2} \sum_{1 \leq i, j \leq 2m} \alpha_{ij} e_i \wedge e_j $$

de $\bigwedge^2 \mathbf{A}^{2m}$, où $(e_i)$ désigne la base canonique de $\mathbf{A}^{2m}$; considérons ${}^t P$ comme la matrice, par rapport à la base $(e_i)$, d’un endomorphisme $f$ de $\mathbf{A}^{2m}$. Alors le bivecteur $(\bigwedge f)(u)$ est associé à la matrice ${}^t P . R . P$ puisqu’il est égal à $\frac{1}{2} \sum_{i, j, s, t} \beta_{is} \alpha_{ij} \beta_{jt} e_s \wedge e_t$. Comme l’extension $\bigwedge f$ de $f$ à l’algèbre extérieure $\bigwedge \mathbf{A}^{2m}$ est un endomorphisme de cette algèbre (chap. III, § 5, no 9), on a $\bigwedge ((\bigwedge f)(u)) = (\bigwedge f)(\bigwedge u)$; comme $\bigwedge f$ est l’homothétie de rapport $\det f$, il résulte donc de (6) et de la déf. 1, que l’on a $m! \mathrm{Pf}({}^t P . R . P) = m! (\det P) \mathrm{Pf}(R)$, d’où (7) dans le cas envisagé. Le cas général s’en déduit en remarquant que les deux membres de (7) sont des polynômes à coefficients entiers par rapport aux éléments des matrices $R$ et $P$ (chap. IV, § 2, no 5, Scholie).

#### Proposition 2 {#alg-ix-s5-prop-2 .statement}

Pour toute matrice alternée $R$ d’ordre pair $2m$ sur un anneau commutatif $A$, on a
$$
\det R = (\mathrm{Pf}(R))^2.
$$
En effet, comme les deux membres de (8) sont des polynômes à coefficients entiers par rapport aux éléments de $R$, le principe de prolongement des identités algébriques (chap. IV, § 2, n° 5, Scholie) montre qu’il suffit de faire la démonstration dans le cas où $A$ est un corps de caractéristique 0 et où $\det R \neq 0$. Si $P$ est une matrice carrée inversible d’ordre $2m$ sur $A$, on a $\det (^tP . R . P) = (\det P)^2 (\det R)$ et $\mathrm{Pf} (^tP . R . P) = (\det P) \mathrm{Pf}(R)$ (prop. 1), de sorte qu’il suffit de prouver (8) pour $^tP . R . P$ au lieu de $R$. D’après le cor. 1 du th. 1, on peut, par un choix convenable de $P$, supposer que la matrice $^tP . R . P$ est de la forme $(\alpha_{ij})$ où
$$
\alpha_{12} = -\alpha_{21} = 1, \ldots, \alpha_{2m-1, 2m} = -\alpha_{2m, 2m-1} = 1,
$$
tous les autres $\alpha_{ij}$ étant nuls (cf. Exemple). Or le déterminant de cette matrice est égal à 1, et son pfaffien également ; ceci achève la démonstration.

### 3. Groupe symplectique.

Supposons l’anneau $A$ commutatif. Si $\Phi$ est une forme bilinéaire alternée sur $E$, les automorphismes du module $E$ laissant $\Phi$ invariante s’appellent les *automorphismes symplectiques* (ou *transformations symplectiques*) relatifs à $\Phi$, et ils forment un groupe que l’on appelle le *groupe symplectique* associé à $\Phi$; on le note quelquefois $\mathbf{Sp}(\Phi)$.

Considérons en particulier, sur le module $E = A^{2m}$, la forme bilinéaire alternée $\Phi_0$ dont la matrice par rapport à la base canonique $(e_i)$ de $E$ est
$$
R_m = \begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix}.
$$
Les automorphismes symplectiques et le groupe symplectique relatifs à $\Phi_0$ s’appellent simplement automorphismes symplectiques et groupe symplectique *à 2m variables* (sur $A$); ce groupe se note $\mathbf{Sp}(2m, A)$ ou $\mathbf{Sp}_{2m}(A)$. Toute matrice $A$ d’un automorphisme symplectique par rapport à la base canonique $(e)_i$ s’appelle une *matrice symplectique*. Une telle matrice est inversible, et, d’après la formule (48) du § 1, n° 10, satisfait à la relation

$$(9)$$
$$
{}^tA . R_m . A = R_m.
$$

Réciproquement si une matrice carrée $A$ d’ordre $2m$ sur $A$ satisfait à (9), elle est symplectique : il suffit en effet de prouver qu’elle est inversible ; or (9) entraîne $\mathrm{Pf}(R_m) = \mathrm{Pf}({}^tA . R_m . A) = (\det A) \mathrm{Pf}(R_m)$ d’après la prop. 1 du n° 2, donc $\det A = 1$. Nous avons en même temps prouvé la proposition suivante :

#### Proposition 3 {#alg-ix-s5-prop-3 .statement}

*Le déterminant d’une matrice symplectique est égal à 1.*

Si $A$ est un corps commutatif et $\Phi$ une forme bilinéaire alternée non dégénérée sur un espace vectoriel $E$ de dimension paire $2m$ sur $A$, le groupe symplectique associé à $\Phi$ est *isomorphe* à $\mathbf{Sp}(2m, A)$, d’après le cor. 1 du th. 1.

*Exercices.* — ¶ 1) Soient $A$ un anneau commutatif principal, $E$ un $A$-module libre de dimension finie $n$, $\Phi$ une forme bilinéaire alternée sur $E$ ; les idéaux $A \alpha_i$ ($1 \leq i \leq r$) définis dans le th. 1 du n° 1 sont appelés les *facteurs invariants* de $\Phi$.

$a)$ Soit $F$ un sous-module de $E$, et soit $\Phi_F$ la restriction de $\Phi$ à $F \times F$. Montrer que si $A \beta_i$ ($1 \leq i \leq s$) sont les facteurs invariants de $\Phi_F$ (où $\beta_i$ divise $\beta_{i+1}$), on a $s \leq r$ et $\beta_i$ est multiple de $\alpha_i$ pour $1 \leq i \leq s$. (Se ramener au cas où $r = s = n/2$, et utiliser les exerc. 9 b) et 9 c) du chap. VII, § 4).

$b)$ Soient $E_1$ un second $A$-module libre de dimension finie, $\Phi_1$ une forme bilinéaire alternée sur $E_1$, $A \gamma_1, \ldots, A \gamma_s$ ses facteurs invariants ($\gamma_i$ divisant $\gamma_{i+1}$). Pour que $\Phi_1$ soit l’image réciproque de $\Phi$ par une application linéaire de $E_1$ dans $E$, il faut et il suffit que $s \leq r$ et que $\gamma_i$ soit multiple de $\alpha_i$ pour $1 \leq i \leq s$. (Utiliser $a$) et la prop. 4 du chap. VII, § 4, n° 5).

$c)$ Soient $F, G$ deux sous-modules de $E$, tels que $F^0$ (resp. $G^0$) soit supplémentaire de $F$ (resp. $G$) dans $E$. Si les restrictions de $\Phi$ à $F$ et $G$ sont équivalentes, montrer qu’il en est de même des restrictions de $\Phi$ à $F^0$ et à $G^0$, et qu’il existe un automorphisme de $E$ laissant $\Phi$ invariante et transformant $F$ en $G$.

$d)$ Donner un exemple de deux sous-modules $F, G$ de $E$, de dimension 2, tels que $F$ et $G$ admettent des supplémentaires dans $E$ et que les restrictions $\Phi_F$ et $\Phi_G$ soient équivalentes, mais qu’il n’existe aucun automorphisme de $E$ laissant $\Phi$ invariante et transformant $F$ en $G$ (prendre $n = 4$).

2) Soit $\Phi$ une forme bilinéaire alternée sur un espace vectoriel $E$ de dimension finie. Montrer que pour tout sous-espace vectoriel $M$ de $E$, la différence dim M – dim (M ∩ M^0) est paire. (Considérer d’abord le cas où Φ est non dégénérée).

¶ 3) Soit E un espace vectoriel de dimension paire n = 2m sur un corps commutatif A ; soient Φ et Ψ deux formes bilinéaires alternées sur E ; on suppose Ψ non dégénérée. Soient u et v les applications linéaires de E dans E* associées à droite à Φ et Ψ respectivement ; v est un isomorphisme de E sur E* ; on pose ω = v^{-1} \circ u, de sorte que ω est un endomorphisme de E.

a) On pose M_0 = E, et par récurrence M_{k+1} = ω(M_k) pour k > 0. Montrer que si M'_k est le sous-espace orthogonal à M_k pour Φ, M_{k+1} est le sous-espace orthogonal à M'_k pour Ψ.

b) Soit n_0 la dimension de M'_0 ; on pose m_0 = 0, et pour k ≥ 1, on désigne par m_k la dimension de M_k ∩ M'_0. Montrer que pour k ≥ 1 la dimension de M_k est n − n_0 − (m_1 + ... + m_{k−1}) et celle de M'_k est n_0 + (m_1 + ... + m_k).

c) Montrer que, pour tout k ≥ 0, la dimension de M_k ∩ M'_k est m_k + m_{k+1} + ... + m_{2k}, et celle de M'_k ∩ M_{k+1} est m_{k+1} + m_{k+2} + ... + m_{2k+1} (appliquer l’exerc. 2 b) du § 3 pour calculer les dimensions de M_h ∩ M'_{2k−h} et de M'_h ∩ M_{2k+1−h} par récurrence sur h).

d) Déduire de c) que les nombres m_k sont pairs (utiliser l’exerc. 2).

e) Conclure de d) que le nombre des diviseurs élémentaires de l’endomorphisme ω, correspondant à la racine caractéristique λ = 0, et ayant un degré donné, est pair (cf. chap. VII, § 5, exerc. 20).

4) Soient E un espace vectoriel sur un corps commutatif A, admettant une base dénombrable (e_n)_{n≥1}, Φ une forme alternée non dégénérée sur E. Montrer qu’il existe dans E une base (a_n) telle que Φ(a_{2n−1}, a_{2n}) = 1 pour tout n ≥ 1, et Φ(a_i, a_j) = 0 pour tout autre couple d’indices tels que i < j (raisonner comme dans l’exerc. 13 du § 4).

5) Pour toute matrice alternée X = (x_{ij}) d’ordre pair n = 2m sur un anneau commutatif, et pour tout indice i, montrer que l’on a
$$
\mathrm{Pf}(X) = \sum_{j=1}^{n} (-1)^{i+j-1} \mathrm{Pf}(X_{ij}) x_{ij},
$$
où X_{ij} est la matrice d’ordre n − 2 obtenue en supprimant dans X les lignes et les colonnes d’indices i et j.

6) Soit M une matrice carrée d’ordre m sur un anneau commutatif. Montrer que si on pose
$$
R = \begin{pmatrix}
0 & M \\
-^t M & 0
\end{pmatrix}
$$
on a Pf(R) = det M (le démontrer d’abord lorsque M est inversible, en utilisant la formule (7)).

7) Soient A un corps commutatif, $\mathfrak{A}(A)$ l’ensemble des matrices alternées d’ordre 2m sur A ; soit I une application de $\mathfrak{A}(A)$ dans A telle que pour toute matrice R ∈ $\mathfrak{A}(A)$ et toute matrice P d’ordre 2m sur A, on ait I(^tPRP) = (det P)^h I(R), où h est un entier rationnel. Montrer que I(R) = c(PfR)^h, où c ∈ A (utiliser la formule (7) et le th. 1 du n° 1).

8) Soient P, Q deux matrices carrées alternées d’ordre pair 2m sur un anneau commutatif A. Soit φ(X) = Pf(P − XQ) ; montrer que, si Q est inversible, on a $\varphi(Q^{-1}P) = 0$. (Considérer d’abord le cas où A est un corps ; déduire alors de l’exerc. 3 que le polynôme minimal de la matrice $Q^{-1}P$ divise $\varphi(X)$, en passant à une extension algébriquement close de A, et en remarquant que $\varphi^2$ est le polynôme caractéristique de $Q^{-1}P$ à un facteur scalaire près).

§ 9) Soient E un espace vectoriel de dimension $n$ sur un corps commutatif A, $\Phi$ une forme bilinéaire alternée sur E, $\Psi$ une forme sesquilinéaire hermitienne (pour un automorphisme involutif de A) sur E, $P$ et $Q$ les matrices respectives de $\Phi$ et $\Psi$ par rapport à une même base de E.

a) On suppose $\Psi$ non dégénérée. Montrer que le nombre des diviseurs élémentaires de $Q^{-1}P$ correspondant à la racine caractéristique 0 et ayant un même degré pair, est un nombre pair (méthode de l’exerc. 3).

b) On suppose que $\Phi$ soit non dégénérée (ce qui implique que $n$ est pair). Montrer que le nombre des diviseurs élémentaires de $P^{-1}Q$ correspondant à la racine caractéristique 0, et ayant un même degré impair, est un nombre pair (même méthode).

10) Soit $\omega_{2m}(\mathbf{F}_q)$ l’ordre du groupe symplectique $\mathbf{Sp}(2m, \mathbf{F}_q)$ sur le corps fini $\mathbf{F}_q$. Montrer que si $h_{2m}$ est le nombre des couples de vecteurs $(x, y)$ de $\mathbf{F}_q^{2m}$ tels que $\Phi_0(x, y) = 1$ (notations du no 3), on a $\omega_{2m}(\mathbf{F}_q) = h_{2m}\omega_{2m-2}(\mathbf{F}_q)$; en déduire

$$
\omega_{2m}(\mathbf{F}_q) = (q^{2m} - 1)q^{2m-1}(q^{2m-2} - 1)q^{2m-3} \ldots (q^2 - 1)q.
$$

11) Soit A un corps commutatif. Montrer que toute transformation $u$ appartenant au groupe symplectique $\mathbf{Sp}(2m, A)$ est un produit de transvections appartenant à ce groupe (dites transvections symplectiques ; cf. § 4, exerc. 6). (Raisonner par récurrence sur $m$, en montrant que si $x, y$ sont deux vecteurs non orthogonaux de $E = A^{2m}$, il existe un produit $v$ de transvections symplectiques tel que $vu$ laisse invariants $x$ et $y$). En déduire une nouvelle démonstration de la prop. 3 du no 3.

*12) Soient A un corps commutatif, E un espace vectoriel de dimension paire $n = 2m$ sur A, $\Phi$ une forme bilinéaire alternée non dégénérée sur E. Montrer que, pour toute similitude $u$ pour la forme $\Phi$ ($\S 6$, no 5), de multiplicateur $\alpha$, on a $\det u = \alpha^m$ (utiliser la formule (7)).*

§ 13) On suppose que A est un corps commutatif de caractéristique 0, E un espace vectoriel de dimension $2m$ sur A, $\Phi$ une forme bilinéaire alternée non dégénérée sur E. On identifie la forme inverse $\widehat{\Phi}$ de $\Phi$ à un bivecteur $\Gamma \in \bigwedge^2 E$, de sorte que pour toute base symplectique $(e_i)_{1 \leq i \leq 2m}$ de E (pour $\Phi$), indexée de sorte que $\Phi(e_i, e_j) = \Phi(e_{m+i}, e_{m+j}) = 0$, $\Phi(e_i, e_{m+j}) = \delta_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq m$), on ait

$$
\Gamma = e_1 \wedge e_{m+1} + e_2 \wedge e_{m+2} + \cdots + e_m \wedge e_{2m}.
$$

On dit qu’un $p$-vecteur décomposable et non nul $z \in \bigwedge^p E$ est isotrope (resp. totalement isotrope) pour $\Phi$, si le sous-espace vectoriel $V_z$ correspondant à $z$ (chap. III, § 7, no 3) est isotrope (resp. totalement isotrope).

a) Si $z$ est un $p$-vecteur décomposable $\neq 0$, $2r$ la dimension d’un supplémentaire de $V_z \cap V_z^0$ par rapport à $V_z$, montrer que $m - p + r$ est le plus grand des entiers $h$ tels que l’on ait $z \wedge \Gamma^h \neq 0$, en désignant par $\Gamma^h$ la puissance $h$-ème de $\Gamma$ dans l’algèbre extérieure $\wedge E$ (utiliser la prop. 2 du § 4, n° 2).

b) Montrer que tout bivecteur $x \in \overset{2}{\wedge} E$ peut s’écrire sous la forme $\lambda \Gamma + x_1$, où $\lambda$ est un scalaire et $x_1$ une combinaison linéaire de bivec- teurs décomposables totalement isotropes. (Se ramener au cas où $x$ est décomposable, et remarquer que si $(e_i)$ est une base symplectique, $(e_1 + e_2) \wedge (e_{m+1} - e_{m+2})$ est totalement isotrope).

c) Si $p \leq m$, montrer que tout $p$-vecteur $z \in \overset{p}{\wedge} E$ peut s’écrire $z = x \wedge \Gamma + z_1$, où $x$ est un $(p-2)$-vecteur et $z_1$ une combinaison linéaire de $p$-vecteurs décomposables totalement isotropes. (Se ramener au cas où $z$ est décomposable, et raisonner par récurrence sur $p$. Se ramener ainsi au cas où, $(e_i)$ étant une base symplectique, on a $z = e_1 \wedge e_2 \wedge \ldots \wedge e_{p-1} \wedge e_{m+p-1}$, et considérer les bivec- teurs $(e_{p-1} + e_{p+i}) \wedge (e_{m+p-1} - e_{m+p+i})$ pour $0 \leq i \leq m-p$.

d) Pour $1 \leq p \leq m$, montrer que tout $(m+p)$-vecteur $z \in \overset{m+p}{\wedge} E$ peut s’écrire $z = y \wedge \Gamma^p$, où $y$ est un $(m-p)$-vecteur. (Se ramener au cas où $z$ est décomposable ; si $2r$ est la dimension d’un supplémentaire de $V_z \cap V_z^0$ par rapport à $V_z$, distinguer deux cas, suivant que $r = p$ ou $r > p$; dans le second cas, raisonner par récurrence sur $r$, de la même manière que dans c)). En déduire que l’application $y \to y \wedge \Gamma^p$ de $\overset{m+p}{\wedge} E$ dans $\overset{m+p}{\wedge} E$ est bijective (remarquer que les deux espaces ont même dimension). Si $y$ est un $(m-p)$-vecteur décomposable, montrer que $z = y \wedge \Gamma^p$ est décomposable et que $V_z = V_y^0$.

e) Déduire de d) que, pour $p \leq m$, le sous-espace $\overset{p}{\wedge} E$ est somme directe de la composante homogène de degré $p$ de l’idéal bilatère $c$ engendré par $\Gamma$ dans $\wedge E$, et du sous-espace $R_p$ des $p$-vecteurs $z_1$ tels que $z_1 \wedge \Gamma^{m-p+1} = 0$ (pour $z \in \overset{p}{\wedge} E$, appliquer d) au $(2m-p+2)$-vecteur $z \wedge \Gamma^{m-p+1}$). En utilisant c), prouver que $R_p$ est engendré par les $p$-vec- teurs décomposables totalement isotropes, et en utilisant d), montrer que l’application $x \to x \wedge \Gamma$ de $\overset{p-2}{\wedge} E$ dans $\overset{p}{\wedge} E$ est injective, et que $R_p$ est de dimension $\binom{2m}{p} - \binom{2m}{p-2}$.

f) Montrer que si $p \leq m$, une condition nécessaire et suffisante pour qu’un $p$-vecteur $z$ soit de la forme $x \wedge \Gamma$ est que, pour tout $m$-vecteur décomposable totalement isotrope $u$, on ait $z \wedge u = 0$. (Montrer que, si cette condition est satisfaite, et si $z \in R_p$, on a $z \wedge y = 0$ pour tout $(2m-p)$-vecteur $y$; mettre pour cela $y$ sous la forme $x \wedge \Gamma^{m-p}$, où $x$ est un $p$-vecteur, puis appliquer c) à $x$, et remarquer que, si $x_1$ est un $p$-vecteur décomposable totalement isotrope, $x_1 \wedge \Gamma^{m-p}$ est un $(2m-p)$-vecteur décomposable qui peut s'écrire $u_1 \wedge v_1$, où $u_1$ est un $m$-vecteur décomposable totalement isotrope).

Soit $\alpha$ l'annulateur de l'idéal $c$ dans $\wedge E$; $\alpha$ est somme directe des sous-espaces $R_m, R_{m-1} \wedge \Gamma, \ldots, R_1 \wedge \Gamma^{m-1}$ et $K \Gamma^m$. Montrer que l'annulateur de $\alpha$ dans $\wedge E$ est égal à $c$ (cf. § 2, exerc. 4 b)).

g) Pour tout automorphisme symplectique $u$ de $E$ (pour $\Phi$), soit $\bar{u}$ l'extension canonique de $u$ en un automorphisme de l'algèbre $\wedge E$ (chap. III, § 5, no 9). Montrer que les seuls éléments de $\wedge E$ invariants par tous les automorphismes $\bar{u}$ sont les combinaisons linéaires de $1, \Gamma, \Gamma^2, \ldots, \Gamma^m$ à coefficients dans $K$. (Si $(e_i)$ est une base symplectique, écrire qu'un élément de $\wedge E$ est invariant par les transvections symplectiques (exerc. 11) correspondant aux hyperplans orthogonaux aux $e_i$; puis considérer les transformations symplectiques $u_{ij}$ définies par $u_{ij}(e_i) = e_j, u_{ij}(e_j) = e_i, u_{ij}(e_{m+i}) = e_{m+j}, u_{ij}(e_{m+j}) = e_{m+i}, u_{ij}(e_k) = e_k$ pour tout autre indice $k$).

14) Soient $A$ un corps commutatif de caractéristique 2, $E$ l'espace vectoriel $A^{2m}$; on identifie le groupe symplectique $Sp(2m, A)$ au groupe des matrices symplectiques $U$, satisfaisant donc à la relation $^tU . R . U = R$, où $R = \begin{pmatrix} 0 & I_m \\ I_m & 0 \end{pmatrix}$. On pose $D = \begin{pmatrix} 0 & 0 \\ I_m & 0 \end{pmatrix}$; montrer que toute matrice symplectique $U$ telle que $I + U$ soit inversible peut s'écrire d'une seule manière sous la forme $(^tD + S)^{-1}(D + S)$, où $S$ est une matrice symétrique telle que $D + S$ soit inversible, et réciproquement (cf. § 4, exerc. 11).

15) Soient $A$ un corps commutatif, $E$ un espace vectoriel de dimension $2m$ sur $A$, $\Phi$ une forme bilinéaire alternée non dégénérée sur $E$.
a) Étendre aux endomorphismes $u$ de $E$ tels que $u^*u = uu^*$ ($u^*$ étant l'adjoint de $u$ pour $\Phi$) les résultats du § 4, exerc. 12 a) et b).

b) On suppose que $u^* = u$. Avec les notations de l'exerc. 12 du § 4, montrer que si $M$ est un élément minimal de l'ensemble $\mathfrak{M}$ des sous-espaces non isotropes contenus dans $G(p, p)$ et stables pour $u$, ou bien $M$ est un sous-module indécomposable de $E_u$, ou bien il est somme directe de deux tels sous-modules isomorphes (raisonner comme dans l'exerc. 12 c) du § 4). Montrer par des exemples (avec $p(X) = X - 1$) que les deux cas peuvent se présenter.

c) On suppose $u^* = -u$, $A$ n'étant pas de caractéristique 2. Avec les mêmes notations, soit $p^h$ le polynôme minimal de la restriction de $u$ à $M$, et soit $d$ le degré de $p$. Montrer que si $d(h-1)$ est impair, $M$ est un sous-module indécomposable de $E_u$; si au contraire $d(h-1)$ est pair, $M$ est, soit indécomposable, soit somme directe de deux sous-modules indécomposables isomorphes.

d) On suppose que $u^*u = 1$ (autrement dit que $u \in Sp(\Phi)$). Avec les notations de c), si $p(X)$ ne divise par $X^{d(h-1)} - 1$, ou si $p(X) = X - 1$ et $(-1)^h \neq -1$, $M$ est un sous-module indécomposable de $E_u$; sinon, $M$ est, soit indécomposable, soit somme directe de deux sous-modules indécomposables isomorphes.
