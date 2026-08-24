---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 5
section_title: Invariants dans l’algèbre symétrique
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0101-0115, 0134-0138
extraction: ocr
subsections:
    - "no": 1
      title: Série de Poincaré des algèbres graduées
      page: 0
      pdf_page: 101
    - "no": 2
      title: 'Invariants d’un groupe linéaire fini : propriétés de module'
      page: 0
      pdf_page: 104
    - "no": 3
      title: 'Invariants d’un groupe linéaire fini : propriétés d’anneau'
      page: 0
      pdf_page: 106
    - "no": 4
      title: Éléments anti-invariants
      page: 0
      pdf_page: 111
    - "no": 5
      title: Compléments (*)
      page: 0
      pdf_page: 113
statements: 23
exercises: 9
content_sha256: f520106d6dad9ccf5e1823170909e9f7735d0ab0bad2ac11aae118378739b749
---

## § 5. Invariants dans l’algèbre symétrique

### 1. Série de Poincaré des algèbres graduées

Soit K un anneau commutatif à élément unité, non réduit à 0. Soient M un K-module gradué de type $ \mathbf{Z} $, $ M_n $ l’ensemble des éléments de M homogènes de degré n. Supposons que chaque $ M_n $ soit *libre de type fini*. Alors le rang $ \mathrm{rg}_K(M_n) $ est défini pour tout $ n $ (*Alg. comm.*, chap. II, § 5, no 3).

#### Définition 1 {#lie-v-s5-def-1 .statement}

S’il existe $ n_0 \in \mathbf{Z} $ tel que $ M_n = 0 $ pour $ n \leq n_0 $, la série formelle $ \sum_{n \geq n_0} \mathrm{rg}_K(M_n) T^n $, qui est un élément de $ \mathbf{Q}((T)) $, s’appelle la série de Poincaré de $ M $ et se note $ P_M(T) $.

Soient $ M' $ un autre $ K $-module gradué de type $ \mathbf{Z} $, $ (M'_n)_{n \in \mathbf{Z}} $ sa graduation. Supposons que $ M'_n $ soit nul pour $ n $ majoré par un certain nombre. Alors on a

(1)
$$
P_{M \oplus M'}(T) = P_M(T) + P_{M'}(T)
$$
et, si l’on munit $ M \otimes_K M' $ de la graduation totale (*Alg.*, chap. II, 3e éd., § 11, n° 5)

(2)
$$
P_{M \otimes M'}(T) = P_M(T) P_{M'}(T).
$$

#### Proposition 1 {#lie-v-s5-prop-1 .statement}

Soit $ S = \bigoplus_{n \geq 0} S_n $ une $ K $-algèbre graduée commutative admettant un système générateur $ (x_1, x_2, \ldots, x_m) $ formé d’éléments homogènes et algébriquement indépendants. Soit $ d_i $ le degré de $ x_i $, et supposons $ d_i > 0 $ pour tout $ i $. Alors les $ S_n $ sont libres de rang fini sur $ K $, et l’on a

(3)
$$
P_S(T) = \prod_{i=1}^m (1 - T^{d_i})^{-1}.
$$

En effet, $ S $ s’identifie au produit tensoriel $ K[x_1] \otimes K[x_2] \otimes \cdots \otimes K[x_m] $, muni de la graduation totale. La série de Poincaré de $ K[x_i] $ est
$$
\sum_{n \geq 0} T^{nd_i} = (1 - T^{d_i})^{-1},
$$
et il suffit d’appliquer (2).

Sous les hypothèses de la prop. 1, nous dirons que $ S $ est une $ K $-algèbre graduée de *polynômes*.

#### Corollaire {#lie-v-s5-n1-cor-1 .statement}

Les degrés $ d_i $ sont déterminés à l’ordre près par $ S $.

En effet, l’inverse de $ P_S(T) $ est le polynôme $ N(T) = \prod_{i=1}^m (1 - T^{d_i}) $, qui est donc déterminé de manière unique. Si $ q $ est un entier $ \geq 1 $ et si $ \zeta \in \mathbf{C} $ est une racine primitive $ q $-ème de l’unité, la multiplicité de la racine $ \zeta $ de $ N(T) $ est égale au nombre des $ d_i $ qui sont multiples de $ q $. Ce nombre est nul pour $ q $ suffisamment grand. Le nombre des $ d_i $ égaux à $ q $ est ainsi déterminé de manière unique par récurrence descendante.

On dit que les entiers $ d_i $ sont les *degrés caractéristiques* de $ S $. Leur nombre est égal au degré de transcendance de $ S $ sur $ K $ lorsque $ K $ est un corps ; nous l’appellerons encore le degré de transcendance de $ S $ sur $ K $ dans le cas général. C’est la multiplicité de la racine 1 du polynôme $ N(T) $.

Soient $ S = \bigoplus_{n \geq 0} S_n $ une K-algèbre graduée commutative, $ R = \bigoplus_{n \geq 0} R_n $ une sous-algèbre graduée de S. *On suppose que chaque $ R_n $ est libre de type fini*, et que le *R-module S admet une base finie formée d’éléments homogènes* $ z_1, z_2, \ldots, z_N $ de degrés $ f_1, f_2, \ldots, f_N $. Alors, si l’on note M le K-module gradué $ \sum_{j=1}^N Kz_j $, le K-module gradué S est isomorphe à $ R \otimes_K M $, donc chaque $ S_n $ est libre de type fini et l’on a

$$
P_S(T) = P_M(T)P_R(T) = (\sum_{j=1}^N T^{f_j})P_R(T).
$$

#### Proposition 2 {#lie-v-s5-prop-2 .statement}

*Conservons les notations précédentes, et supposons que S et R soient des K-algèbres graduées de polynômes.*

(i) R et S ont même degré de transcendance r sur K.

(ii) *Soient $ p_1, \ldots, p_r $ (resp. $ q_1, \ldots, q_r $) les degrés caractéristiques de S (resp. R)*. On a

$$
\prod_{i=1}^r (1 - T^{q_i}) = (\sum_{j=1}^N T^{f_j}) \prod_{i=1}^r (1 - T^{p_i}).
$$

(iii) $ N p_1 p_2 \cdots p_r = q_1 q_2 \cdots q_r $.

La formule (4) prouve d’abord que la multiplicité de la racine 1 est la même dans les polynômes $ P_S(T)^{-1} $ et $ P_R(T)^{-1} $ et, compte tenu de (3), prouve (i) puis (ii).

On déduit de (ii) que

$$
\prod_{i=1}^r (1 + T + T^2 + \cdots + T^{q_i-1}) = (\sum_{j=1}^N T^{f_j}) \prod_{i=1}^r (1 + T + T^2 + \cdots + T^{p_i-1}).
$$

Faisant $ T = 1 $ dans cette relation, on obtient (iii).

#### Remarque {#lie-v-s5-n1-rem-1 .statement}

Soient $ S = K[X_1, \ldots, X_n] $ une K-algèbre graduée de polynômes, $ d_i $ le degré de $ X_i $ et $ F(X_1, \ldots, X_n) $ un élément homogène de degré m de S. Alors on a

$$
\sum_{i=1}^n d_i X_i \frac{\partial F}{\partial X_i} = mF.
$$

En effet, il est immédiat que l’application K-linéaire D de S dans S qui transforme tout élément z homogène de degré p en $ pz $ est une dérivation de S. Donc :

$$
mF(X_1, \ldots, X_n) = D(F(X_1, \ldots, X_n)) = \sum_{i=1}^n D(X_i) \frac{\partial F}{\partial X_i} = \sum_{i=1}^n d_i X_i \frac{\partial F}{\partial X_i}.
$$

### 2. Invariants d’un groupe linéaire fini : propriétés de module

Soient $ K $ un anneau commutatif ayant un élément unité, $ V $ un $ K $-module, $ G $ un groupe opérant dans $ V $. On sait que tout automorphisme de $ V $ se prolonge de façon unique en un automorphisme de l’algèbre symétrique $ S = S(V) $, et $ G $ opère donc dans cette algèbre. Si $ x \in S $ et $ g \in G $, nous noterons $ g_S . x $ le transformé de $ x $ par $ g $. Soit $ R $ la sous-algèbre $ S^G $ de $ S $ formée des éléments invariants par $ G $.

Supposons $ G $ fini, $ V $ de type fini, et $ K $ nœthérien. Alors $ S $ est un $ R $-module de type fini, et $ R $ est une $ K $-algèbre de type fini ($ Alg. comm. $, chap. V, § 1, no 9, th. 2). Supposons $ S $ intègre et soit $ N $ son corps des fractions. Le corps des fractions $ L $ de $ R $ est l’ensemble des éléments de $ N $ invariants par $ G $ (*loc. cit.*, cor. de la prop. 23), donc $ N $ est une extension galoisienne de $ L $. Tout élément de $ N $ s’écrit $ z/t $ avec $ z \in S $ et $ t \in R $ (*loc. cit.*, prop. 23). D’après $ Alg. $, chap. II, 3e éd., § 7, no 10, cor. 3 de la prop. 26, le rang du $ R $-module $ S $ est $[N : L]$. Supposons que $ G $ opère fidèlement dans $ V $. Le groupe de Galois de $ N $ sur $ L $ s’identifie alors à $ G $, donc $[N : L] = \mathrm{Card}\,(G)$; ainsi :

$$
\mathrm{rg}_R(S) = [N : L] = \mathrm{Card}\,(G).
$$

Pour toute algèbre graduée $ A = A_0 \oplus A_1 \oplus \ldots \oplus A_n \oplus \ldots $, nous noterons $ A_+ $ l’idéal $ \bigoplus_{n > 0} A_n $.

#### Théorème 1 {#lie-v-s5-thm-1 .statement}

*Soient $ K $ un corps commutatif, $ V $ un espace vectoriel de dimension finie sur $ K $, $ S = S(V) $ l’algèbre symétrique de $ V $, $ G $ un groupe fini d’automorphismes de $ V $, et $ R $ la sous-algèbre graduée de $ S $ formée des éléments invariants par $ G $. On suppose que $ G $ est engendré par des pseudo-réflexions ($ § 2, $ no 1 ), et que $ q = \mathrm{Card}(G) $ est étranger à l’exposant caractéristique de $ K $. Alors le $ R $-module $ S $ admet une base formée de $ q $ éléments homogènes.*

$ a) $ Comme chaque sous-module de $ S/(R_+ S) $ est libre sur $ R_0 = K $, il suffit de montrer (en vertu d’*Alg.*, chap. II, 3e éd., § 11, no 4, prop. 7) que l’homomorphisme canonique de $ R_+ \otimes_R S $ dans $ S $ est injectif. Pour tout $ R $-module $ E $, notons $ T(E) $ le $ R $-module $ \mathrm{Ker}(R_+ \otimes_R E \to E) $ (*autrement dit $ T(E) = \mathrm{Tor}_1^R(R/R_+, E)_* $). Si $ E, E' $ sont deux $ R $-modules et si $ u $ est un homomorphisme de $ E $ dans $ E' $, l’homomorphisme $ 1 \otimes u $ de $ R_+ \otimes E $ dans $ R_+ \otimes E' $ définit par restriction à $ T(E) $ un homomorphisme de $ T(E) $ dans $ T(E') $ que nous noterons $ T(u) $. Si $ u' $ est un homomorphisme de $ E' $ dans un $ R $-module $ E'' $, on a $ T(u' \circ u) = T(u') \circ T(u) $. Donc, si $ G $ opère sur $ E $ de façon $ R $-linéaire, $ G $ opère dans $ T(E) $.

$ b) $ Le groupe $ G $ opère dans $ S $ de façon $ R $-linéaire, donc aussi dans $ T(S) $. Par ailleurs, $ T(S) $ est muni de manière naturelle d’une structure de $ S $-module gradué. Montrons d’abord que, si $ g \in G $, $ g $ transforme tout élément $ x $ de $ T(S) $ est un élément congru à $ x $ modulo $ S_1 T(S) $. Il suffit de le faire quand $ g $ est une pseudo-réflexion. Il existe alors un vecteur non nul $ v $ de $ V $ tel que $ g(x) - x \in K v $ pour tout $ x \in V $. Comme $ V $ engendre $ S $, on en déduit que $ g_S $ opère trivialement sur $ S/Sv $. Donc, pour tout $ y \in S $, il existe un élément $ h(y) $ de $ S $ tel que

$$
g_S(y) - y = h(y)v.
$$

Comme $ S $ est intègre et que $ v $ est non nul, cet élément est déterminé de manière unique par $ y $; il est immédiat que $ h $ est un endomorphisme de degré — 1 du $ R $-module $ S $. Ainsi, $ g_S - 1_S = m_v \circ h $ en notant $ m_v $ l’homothétie de rapport $ v $ dans $ S $. Donc

$$
T(g_S) - 1_{T(S)} = T(g_S - 1_S) = T(m_v) \circ T(h)
$$

dont l’image est contenue dans $ vT(S) $, ce qui prouve notre assertion.

$ c) $ Montrons maintenant que tout élément de $ T(S) $ invariant par $ G $ est nul. En effet, soit $ Q $ l’endomorphisme du $ R $-module $ S $ défini par

$$
Q(y) = q^{-1} \sum_{g \in G} g_S(y)
$$

pour tout $ y \in S $. On a $ Q(S) = R $. On peut donc écrire $ Q = i \circ Q' $ où $ Q' $ est un homomorphisme du $ R $-module $ S $ sur le $ R $-module $ R $ et où $ i $ désigne l’injection canonique de $ R $ dans $ S $. Donc $ T(Q) = T(i) \circ T(Q') $, et $ T(Q') = 0 $ puisque $ T(R) = \mathrm{Ker}\,(R_+ \otimes R \to R) = 0 $. Donc

$$
0 = T(Q) = q^{-1} \sum_{g \in G} T(g_S).
$$

Or $ q^{-1} \sum_{g \in G} T(g_S) $ laisse fixes les éléments de $ T(S) $ invariants par $ G $. Ceux-ci sont donc nuls.

$ d) $ Supposons $ T(S) \neq 0 $. Il existe dans $ T(S) $ un élément homogène $ u \neq 0 $ de degré minimum. D’après $ b) $, $ u $ est invariant par $ G $. D’après $ c) $, $ u = 0 $. On a ainsi une contradiction, d’où $ T(S) = 0 $. C.Q.F.D.

#### Remarque 1 {#lie-v-s5-n2-rem-1 .statement}

Il résulte d’Alg., chap. II, 3e éd., § 11, no 4, prop. 7 que, si $ (z_1, z_2, \ldots, z_q) $ est une famille d’éléments homogènes de $ S $ dont les images canoniques dans $ S/(R_+S) $ forment une base de $ S/(R_+S) $ sur $ K $, alors $ (z_1, z_2, \ldots, z_q) $ est une base de $ S $ sur $ R $.

#### Remarque 2 {#lie-v-s5-n2-rem-2 .statement}

Soit $ g $ une pseudo-réflexion de $ V $, d’ordre fini $ n \geq 2 $, premier à l’exposant caractéristique de $ K $. D’après le théorème de Maschke (Annexe, prop. 2), on peut décomposer $ V $ en $ D \oplus H $, où $ H $ est l’hyperplan formé des éléments de $ V $ invariants par $ g $, et où $ D $ est une droite sur laquelle $ g $ opère par multiplication par une racine primitive $ n $-ème de l’unité. Lorsque $ K = \mathbf{R} $, ceci n’est possible que si $ n = 2 $, et $ g $ est alors une réflexion; dans ce cas, les groupes auxquels s’appliquent le th. 1 sont donc les groupes de Coxeter finis. (Pour $ K = C $, par contre, le th. 1 s’applique à certains groupes qui ne sont pas de Coxeter) (*).

#### Théorème 2 {#lie-v-s5-thm-2 .statement}

Les hypothèses et notations sont celles du théorème 1.

(i) Il existe un sous-espace vectoriel gradué de $ S $, supplémentaire de $ R_+ S $ dans $ S $, stable par $ G $.

(ii) Soit $ U $ un tel supplémentaire. L’homomorphisme canonique de $ U \otimes_K R $ dans $ S $ est un isomorphisme de $ G $-modules, et la représentation de $ G $ dans $ U $ (resp. $ S $) est isomorphe à la représentation régulière de $ G $ sur $ K $ (resp. $ R $).

En effet, pour tout entier $ n \geq 0 $, les $ K $-espaces vectoriels $ S_n $ et $ (R_+ S) \cap S_n $ sont stables par $ G $, et il résulte du th. de Maschke (Annexe, prop. 2) qu’il existe un supplémentaire $ U_n $ de $ (R_+ S) \cap S_n $ dans $ S_n $ stable par $ G $. Alors $ \sum_{n \geq 0} U_n $ est un supplémentaire de $ R_+ S $ dans $ S $ stable par $ G $, d’où (i).

Soit $ U $ un sous-espace vectoriel gradué de $ S $, supplémentaire de $ R_+ S $ dans $ S $, stable par $ G $. D’après la remarque 1, toute base du $ K $-espace vectoriel $ U $ est aussi une base du $ R $-module $ S $, et par suite une base du corps des fractions $ N $ de $ S $ sur le corps des fractions $ L $ de $ R $. Ainsi, le $ L $-espace vectoriel $ N $ s’identifie à $ U \otimes_K L $. Comme $ U $ est stable par $ G $, cette identification est compatible avec les opérations de $ G $. L’algèbre $ L[G] $ du groupe $ G $ sur $ L $ s’identifie à l’algèbre $ K[G] \otimes_K L $. L’extension galoisienne $ N $ de $ L $ admet une base normale ($ Alg. $, chap. V, § 10, th. 5 et $ Alg. $, chap. VII, § 5, no 7), ce qui peut s’interpréter en disant que $ N $, considéré comme $ L[G] $-module, est isomorphe au module de la représentation régulière de $ G $ sur $ L $. Comme $ U $ est de dimension finie sur $ K $, il résulte alors de l’Annexe, prop. 1, que le $ K[G] $-module $ U $ est isomorphe au module de la représentation régulière de $ G $ sur $ K $. Nos assertions en résultent aussitôt.

### 3. Invariants d’un groupe linéaire fini : propriétés d’anneau

#### Théorème 3 {#lie-v-s5-thm-3 .statement}

Les hypothèses et notations sont celles du th. 1. Dans l’ensemble des systèmes générateurs de l’idéal $ R_+ $ de $ R $ formés d’éléments homogènes, choisissons un élément minimal $ (\alpha_1, \ldots, \alpha_l) $. Soit $ k_i $ le degré de $ \alpha_i $. On suppose que les $ k_i $ sont étrangers à l’exposant caractéristique de $ K $. Alors $ l = \dim V $, les $ \alpha_i $ engendrent la $ K $-algèbre $ R $, et sont algébriquement indépendants sur $ K $. En particulier, $ R $ est une $ K $-algèbre graduée de polynômes de degré de transcendance $ l $ sur $ K $.

L’hypothèse faite sur les $ k_i $ est superflue, mais n’est pas gênante pour les applications aux groupes de Coxeter finis, puisqu’on a alors $ K = R $. Cf. le no 5, où l’on donnera d’ailleurs une autre démonstration du th. 3.

(*) On trouvera une classification de ces groupes dans G. C. Shephard et J. A. Todd, Finite unitary reflection groups, Canad. J. of Maths., t. VI (1954), p. 274-304.

Le th. 3 résultera de la prop. 2 (i), du th. 1, et du lemme suivant:

#### Lemme 1 {#lie-v-s5-lem-1 .statement}

Soient $ K $ un corps commutatif, $ S $ une $ K $-algèbre graduée de polynômes, et $ R $ une sous-algèbre graduée de type fini de $ S $ telle que le $ R $-module $ S $ admette une base $ (z_\lambda)_{\lambda \in \Lambda} $ formée d’éléments homogènes. Dans l’ensemble des systèmes générateurs de l’idéal $ R_+ $ de $ R $ formés d’éléments homogènes, choisissons un élément minimal $ (\alpha_1, \ldots, \alpha_s) $. On suppose que, pour tout $ i $, le degré $ k_i $ de $ \alpha_i $ est étranger à l’exposant caractéristique $ p $ de $ K $. Alors les $ \alpha_i $ engendrent la $ K $-algèbre $ R $ et sont algébriquement indépendants sur $ K $.

D’après Alg., chap. II, § 11, no 4, prop. 7, l’hypothèse faite sur les $ \alpha_i $ équivaut à dire qu’ils sont homogènes et que leurs images dans le $ K $-espace vectoriel $ R_+/((R_+)^2 $ forment une base de cet espace. Cette condition est invariante par extension du corps de base; on peut donc se ramener au cas où celui-ci est parfait.

La famille $ (\alpha_1, \ldots, \alpha_s) $ engendre l’algèbre $ R $ d’après Alg. comm., chap. III, § 1, no 2, prop. 1. Raisonnons par l’absurde et supposons que cette famille soit algébriquement liée sur $ K $.

1) Nous allons d’abord montrer qu’il existe des familles

$$
(\beta_i)_{1 \leq i \leq s}, \quad (\gamma_k)_{1 \leq k \leq r}, \quad (d_{ik})_{1 \leq i \leq s, 1 \leq k \leq r}
$$

d’éléments homogènes de $ S $, avec les propriétés suivantes:

(7) $ \beta_i \in R $ pour tout $ i $, et les $ \beta_i $ sont non tous nuls;

(8) $ \deg \gamma_k > 0 $ pour tout $ k $;

(9) $ \alpha_i = \sum_{k=1}^r d_{ik} \gamma_k $ pour tout $ i $;

(10) $ \sum_{i=1}^s \beta_i d_{ik} = 0 $ pour tout $ k $.

Soient $ X_1, \ldots, X_s $ des indéterminées et munissons $ K[X_1, \ldots, X_s] $ de la structure d’algèbre graduée pour laquelle $ X_i $ est de degré $ k_i $. Il existe des éléments homogènes non nuls $ H(X_1, \ldots, X_s) $ de $ K[X_1, \ldots, X_s] $ tels que $ H(\alpha_1, \ldots, \alpha_s) = 0 $; choisissons $ H $ de manière que son degré soit minimum. Si $ \partial H / \partial X_i \neq 0 $, le polynôme $ \frac{\partial H}{\partial X_i} (\alpha_1, \ldots, \alpha_s) $ est donc un élément homogène non nul de $ R $; si $ p \neq 1 $, $ H $ n’est pas de la forme $ H_1^p $ avec $ H_1 \in K[X_1, \ldots, X_s] $. Prenons alors

$$
\beta_i = k_i \frac{\partial H}{\partial X_i} (\alpha_1, \ldots, \alpha_s).
$$

Comme $ K $ est parfait, les polynômes $ \partial H / \partial X_i \in K[X_1, \ldots, X_s] $ ne sont pas tous nuls (Alg., chap. V, § 1, no 3, prop. 4); vu l’hypothèse faite sur les $ k_i $, il en est de même des $ \beta_i $.

D’autre part, S s’identifie à une algèbre graduée de polynômes

$$
K[x_1, \ldots, x_r]
$$

en notant $x_1, \ldots, x_r$ des indéterminées affectées de degrés $m_i > 0$ convenables. Soit $D_k$ la dérivation partielle par rapport à $x_k$ dans S. Nous prendrons $d_{ik} = k_i^{-1} D_k(\alpha_i)$. Alors l’égalité (10) est vraie car son premier membre est $D_k(H(\alpha_1, \ldots, \alpha_s))$. D’autre part, si on pose $y_1 = m_1 x_1, \ldots, y_r = m_r x_r$, l’égalité (9) résulte de l’égalité (5) du no 1.

2) Soit $h$ l’idéal de R engendré par les $\beta_i$; il existe une partie J de

$$
I = \{1, 2, \ldots, s\}
$$

telle que $(\beta_i)_{i \in J}$ soit un système générateur minimal de $h$. On a $J \neq \emptyset$ car $h \neq 0$. Nous allons déduire de (9) et (10) que, si $i \in J$, $\alpha_i$ est combinaison R-linéaire des $\alpha_j$ pour $j \neq i$, ce qui contredira la minimalité de $(\alpha_1, \ldots, \alpha_s)$ et achèvera la démonstration.

Il existe des éléments homogènes $\gamma_{ji}$ de R ($i \in J, j \in I - J$) tels que

$$
\beta_j = \sum_{i \in J} \gamma_{ji} \beta_i \quad (j \in I - J).
$$

En tenant compte de (11), la formule (10) donne

$$
\sum_{i \in J} \beta_i (d_{ik} + \sum_{j \in I - J} \gamma_{ji} d_{jk}) = 0.
$$

Posons

$$
u_{ik} = d_{ik} + \sum_{j \in I - J} \gamma_{ji} d_{jk}.
$$

On a donc

$$
\sum_{i \in J} \beta_i u_{ik} = 0.
$$

Écrivons $u_{ik} = \sum_{\lambda \in \Lambda} \delta_{ik\lambda} z_\lambda$, où les $\delta_{ik\lambda}$ appartiennent à R. La relation (14) entraîne $\sum_{i \in J} \beta_i \delta_{ik\lambda} = 0$ quels que soient $k$ et $\lambda$. Si l’un des $\delta_{ik\lambda}$ avait une composante homogène de degré 0 non nulle, l’égalité précédente entraînerait que l’un des $\beta_i (i \in J)$ est combinaison R-linéaire des autres, contrairement à la minimalité de $(\beta_i)_{i \in J}$. Donc $\delta_{ik\lambda} \in \mathbf{R}_+$ et par suite $u_{ik} \in \mathbf{R}_+ S$ quels que soient $i$ et $k$. Il existe donc des $u_{ikh} \in S$ tels que $u_{ik} = \sum_{h=1}^s u_{ikh} \alpha_h$, autrement dit, d’après (13),

$$
d_{ik} + \sum_{j \in I - J} \gamma_{ji} d_{jk} = \sum_{h=1}^s u_{ikh} \alpha_h.
$$

Multiplions les deux membres de (15)$_{ik}$ par $y_k$, et additionnons pour $i$ fixé dans $ J $ et $ k = 1, 2, \ldots, r $; en vertu de (9), on trouve

$$
\alpha_i + \sum_{j \in I - J} \gamma_{ji} \alpha_j = \sum_{h=1}^s \sum_{k=1}^r u_{ikh} y_k \alpha_h.
$$

Prenons les composantes homogènes de degré $ k_i $ des deux membres. Comme $ \deg y_k > 0 $, on voit que $ \alpha_i $ est combinaison S-linéaire des $ \alpha_j $ avec $ j \neq i $. Comme S est libre sur $ \mathbf{R} $ et que $ \alpha_1, \ldots, \alpha_s \in \mathbf{R} $, on en déduit que $ \alpha_i $ est combinaison R-linéaire des $ \alpha_j $ avec $ j \neq i $ (*Alg. comm.*, chap. I, § 3, no 5, prop. 9 d)).

#### Corollaire {#lie-v-s5-n3-cor-1 .statement}

*Les hypothèses et notations étant celles du th. 3, le produit des degrés caractéristiques de R est Card (G)*.

En effet, on a $ \mathrm{rg}_R(S) = \mathrm{Card}(G) $ (formule (6), no 2). Les degrés caractéristiques de S sont égaux à 1. Alors le corollaire résulte du no 1, prop. 2 (iii).

#### Lemme 2 {#lie-v-s5-lem-2 .statement}

*Soient K un corps commutatif, V un espace vectoriel de dimension finie sur K, $ S = \bigoplus_{n \geq 0} S_n $ l’algèbre symétrique de V, s un endomorphisme de V, et $ s^{(n)} $ le prolongement canonique de s à $ S_n $. Alors, T désignant une indéterminée, on a dans $ K[[T]] $

$$
\sum_{n=0}^\infty \mathrm{Tr}(s^{(n)}) T^n = (\det (1 - sT))^{-1}.
$$

Quitte à étendre le corps de base, on peut supposer K algébriquement clos. Soit $ (e_1, \ldots, e_r) $ une base de V par rapport à laquelle la matrice de s est triangulaire inférieure, et soient $ \lambda_1, \ldots, \lambda_r $ les éléments diagonaux de cette matrice. Par rapport à la base $ (e_1^{i(1)} \ldots e_r^{i(r)})_{i(1)+\ldots+i(r)=n} $ de $ S_n $, ordonnée lexicographiquement, la matrice de $ s^{(n)} $ est triangulaire inférieure, et ses éléments diagonaux sont les produits $ \lambda_1^{i(1)} \ldots \lambda_r^{i(r)} $. Donc

$$
\mathrm{Tr}(s^{(n)}) = \sum_{i(1)+\cdots+i(r)=n} \lambda_1^{i(1)} \ldots \lambda_r^{i(r)},
$$

et par suite

$$
\sum_{n=0}^\infty \mathrm{Tr}(s^{(n)}) T^n = (\sum_{n=0}^\infty \lambda_1^n T^n)(\sum_{n=0}^\infty \lambda_2^n T^n) \ldots (\sum_{n=0}^\infty \lambda_r^n T^n)
= (1 - \lambda_1 T)^{-1}(1 - \lambda_2 T)^{-1} \ldots (1 - \lambda_r T)^{-1}
= (\det (1 - sT))^{-1}.
$$

#### Lemme 3 {#lie-v-s5-lem-3 .statement}

*Soient K, V et S comme dans le lemme 2, G un groupe fini d’automorphismes de V, q l’ordre de G, R la sous-algèbre graduée de S formée des éléments invariants par G. On suppose K de caractéristique 0. La série de Poincaré de R est alors*

$$
q^{-1} \sum_{g \in G} (\det(1 - gT))^{-1}.
$$

En effet, l’endomorphisme $ f = q^{-1} \sum_{g \in G} g^{(n)} $ est un projecteur de $ S_n $ sur $ R_n $, donc $ \operatorname{Tr}(f) = \dim_K S^G $. La série de Poincaré de $ R $ est alors

$$
q^{-1} \sum_{g \in G} (\sum_{n=0}^\infty (\operatorname{Tr} g^{(n)}) T^n),
$$

et il suffit d’appliquer le lemme 2.

#### Proposition 3 {#lie-v-s5-prop-3 .statement}

*Les hypothèses et notations étant celles du th. 3, soit $ H $ l’ensemble des pseudo-réflexions appartenant à $ G $ et distinctes de 1. On suppose $ K $ de caractéristique 0. Alors* $ \operatorname{Card}(H) = \sum_{i=1}^l (k_i - 1) $.

D’après la prop. 3 de l’Annexe, on peut supposer $ K $ algébriquement clos. Pour tout $ g \in G $, soient $ \lambda_1(g), \ldots, \lambda_l(g) $ ses valeurs propres. Comme tout $ g \in G $ est diagonalisable (Annexe, prop. 2), on a $ g = 1 $ si et seulement si tous les $ \lambda_i(g) $ sont égaux à 1, et $ g \in H $ si et seulement si le nombre des $ \lambda_i(g) $ égaux à 1 est $ l - 1 $ (nous noterons alors $ \lambda(g) $ la valeur propre distincte de 1). La prop. 1 du no 1 et le lemme 3 prouvent que

$$
q \prod_{i=1}^l (1 - T^{k_i})^{-1} = \sum_{g \in G} (\det(1 - gT))^{-1}
$$

dans $ K[[T]] $, donc dans $ K(T) $. Par suite, on a dans $ K(T) $ :

$$
q \frac{(1 - T)^{l-1}}{\prod_{i=1}^l (1 - T^{k_i})} = \frac{1}{1 - T} + \sum_{g \in H} \frac{1}{1 - \lambda(g)T} + \sum_{g \neq 1, g \in H} \frac{(1 - T)^{l-1}}{\det(1 - gT)},
$$

ce qui s’écrit

$$
\frac{q - \prod_{i=1}^l (1 + T + \cdots + T^{k_i-1})}{(1 - T) \prod_{i=1}^l (1 + T + \cdots + T^{k_i-1})}
$$

$$
= \sum_{g \in H} \frac{1}{1 - \lambda(g)T} + \sum_{g \neq 1, g \in H} \frac{(1 - T)^{l-1}}{\det(1 - gT)}.
$$

On voit que $ q - \prod_{i=1}^l (1 + T + \cdots + T^{k_i-1}) $ doit s’annuler pour $ T = 1 $, d’où $ q = k_1 k_2 \ldots k_l $, ce que nous savions déjà par le cor. du th. 3. Cela étant dit, soit $ Q(T) $ le polynôme $ (1 - T)^{-1}(q - \prod_{i=1}^l (1 + T + \cdots + T^{k_i-1})) $. En dérivant l’égalité $ (1 - T)Q(T) = q - \prod_{i=1}^l (1 + T + \cdots + T^{k_i-1}) $ et en faisant $ T = 1 $, on voit que $ - Q(1) $ est la valeur pour $ T = 1 $ de
$$
-\frac{d}{dt} (\prod_{i=1}^l (1 + T + \cdots + T^{k_i-1}))
$$
$$
= - \sum_{i=1}^l (1 + 2T + \cdots + (k_i-1)T^{k_i-2}) \prod_{j \neq i} (1 + T + \cdots + T^{k_j-1})
$$
d’où
$$
Q(1) = \sum_{i=1}^l \frac{(k_i-1)k_i}{2} \prod_{j \neq i} k_j = (\prod_{j=1}^l k_j) \left( \sum_{i=1}^l \frac{k_i-1}{2} \right).
$$
Revenant à (17), on a par ailleurs
$$
Q(1) = (\prod_{j=1}^l k_j) \left( \sum_{g \in H} \frac{1}{1-\lambda(g)} \right)
$$
Donc
$$
\sum_{i=1}^l \frac{k_i-1}{2} = \sum_{g \in H} \frac{1}{1-\lambda(g)}.
$$
Or les éléments de $ G $ qui laissent fixes les points d’un hyperplan donné laissent stable une droite supplémentaire de l’hyperplan (Annexe, prop. 2), donc forment un sous-groupe cyclique $ G' $ de $ G $ d’après *Alg.*, chap. V, § 11, n° 1, th. 1. Soit $ t $ l’ordre de $ G' $; les valeurs de $ \lambda(g) $ pour $ g \in G' $ sont $ \theta, \theta^2, \ldots, \theta^{t-1} $ avec $ \theta $ racine primitive $ t $-ème de l’unité. On a $ \frac{1}{1-\theta^i} + \frac{1}{1-\theta^{t-i}} = 1 $, donc
$$
\sum_{g \in G', g \neq 1} \frac{1}{1-\lambda(g)} = \frac{1}{2} (t-1) = \frac{1}{2} \operatorname{Card}(H \cap G').
$$
L’égalité (18) prouve alors la proposition.

#### Remarque {#lie-v-s5-n3-rem-1 .statement}

Lorsque $ K = \mathbf{R} $, $ G $ est un groupe de Coxeter et $ H $ est l’ensemble des réflexions appartenant à $ G $, on sait (§ 3) que les éléments de $ H $ sont en correspondance binnivoque avec les *murs* de $ V $.

#### Proposition 4 {#lie-v-s5-prop-4 .statement}

Les hypothèses et notations étant celles du th. 3, on suppose $ K $ de caractéristique $ \neq 2 $. Pour qu’on ait $ -1 \in G $, il faut et il suffit que les degrés caractéristiques $ k_1, \ldots, k_l $ de $ \mathbf{R} $ soient tous pairs.

Soit $ f $ l’automorphisme de l’algèbre $ S $ qui prolonge l’automorphisme $ -1 $ de $ V $. On a $ f(z) = (-1)^{\deg z} z $ pour tout $ z $ homogène de $ S $. Donc, si $ -1 \in G $, tout élément homogène de degré impair de $ \mathbf{R} $ est nul, et les $ k_i $ sont pairs. Réciproquement, si les $ k_i $ sont pairs, tout élément de $ \mathbf{R} $ est invariant par $ f $, et la théorie de Galois montre que $ -1 \in G $.

### 4. Éléments anti-invariants

On conserve les hypothèses et les notations du th. 3, et on suppose $ K $ de caractéristique 0. Un élément $ z $ de $ S $ est dit *anti-invariant* par $ G $ si
$$
g(z) = (\det g)^{-1} z
$$
quel que soit $ g \in G $.

Soit $ H $ l’ensemble des pseudo-réflexions appartenant à $ G $ et distinctes de 1. Pour tout $ g \in H $, il existe $ e_g \in V $ et $ f_g \in V^* $ tels que
$$
g(x) = x + f_g(x)e_g, \quad \text{quel que soit } x \in V.
$$

#### Proposition 5 {#lie-v-s5-prop-5 .statement}

(i) *Soit D l’élément $ \prod_{g \in H} e_g $ de S. Les éléments de S anti-invariants par G sont les éléments de RD.*

(ii) *Supposons S identifiée à l’algèbre des polynômes $ K[X_1, \ldots, X_l] $ par le choix d’une base $ (X_1, \ldots, X_l) $ de $ V $, et soient $ (P_1, \ldots, P_l) $ des éléments homogènes algébriquement indépendants de S engendrant l’algèbre R (th. 3). Alors le jacobien*
$$
J = \det \left( \frac{\partial P_i}{\partial X_j} \right)
$$
*est de la forme $ \lambda D $, où $ \lambda \in K^* $.*

a) Avec les notations de (ii), on a
$$
dP_1 \wedge dP_2 \wedge \ldots \wedge dP_l = J dX_1 \wedge dX_2 \wedge \ldots \wedge dX_l,
$$
d’où, pour tout $ g \in G $,
$$
g(J)(\det g)dX_1 \wedge \ldots \wedge dX_l = g(J)d(gX_1) \wedge \ldots \wedge d(gX_l)
= g(dP_1 \wedge \ldots \wedge dP_l) = dP_1 \wedge \ldots \wedge dP_l = J dX_1 \wedge \ldots \wedge dX_l
$$
donc $ J $ est anti-invariant par $ G $. En outre, le corps des fractions $ N $ de $ S $ est extension galoisienne du corps des fractions $ E $ de $ R $ (n° 2); si $ \Delta $ est une dérivation de $ E $ à valeurs dans un surcorps $ \Omega $ de $ N $, $ \Delta $ se prolonge en une dérivation de $ N $ dans $ \Omega $ (*Alg.*, chap. V, § 9, prop. 5); comme les $ P_i $ sont algébriquement indépendants, on en déduit que $ dP_1 \wedge \ldots \wedge dP_l \neq 0 $, donc $ J \neq 0 $.

$ b) $ Soit $ z $ un élément de $ S $ anti-invariant par $ G $. Montrons que $ z $ est divisible par $ D $ dans $ S $. Soit $ a $ un vecteur non nul de $ V $. Les éléments de $ G $ qui laissent stable $ Ka $ laissent stable un hyperplan supplémentaire $ L $ (Annexe, prop. 2); pour qu’un élément de $ G $ laissant stable $ Ka $ soit 1 ou une pseudo-réflexion de vecteur $ a $, il faut et il suffit qu’il induise 1 dans $ L $; les pseudo-réflexions de vecteur $ a $ qui appartiennent à $ G $ constituent donc avec 1 un sous-groupe cyclique $ G' $ de $ G $; soit $ t $ son ordre. Il existe une base $ (X_1, \ldots, X_l) $ de $ V $ telle que $ a = X_1, X_2 \in L, \ldots, X_l \in L $, et on peut identifier $ z $ à un polynôme $ P(X_1, \ldots, X_l) $ à coefficients dans $ K $. Exprimant que $ g(z) = (\det g)^{-1}z $ pour $ g \in G' $, on voit que $ X_1 $ n’intervient dans $ P(X_1, \ldots, X_l) $ qu’avec des exposants congrus à — 1 modulo $ t $. Donc $ P(X_1, \ldots, X_l) $ est divisible par $ X_1^{t-1} = a^{t-1} $. Or $ D $ est, à un facteur scalaire près, le produit des $ a^{t-1} $ pour les $ a \in V $ tels que $ t > 1 $, et ces éléments de $ S $ sont étrangers deux à deux. Comme $ S $ est factoriel, $ z $ est divisible par $ D $.

$ c) $ D’après $ a) $ et $ b) $, $ J $ est divisible par $ D $ dans $ S $. Or
$$
\deg J = \sum_{i=1}^l (k_i - 1) = \mathrm{Card}\,(H)
$$

(prop. 3), donc $ \deg J = \deg D $, donc $ J = \lambda D $ avec $ \lambda \in K $. Comme $ J \neq 0 $, on a $ \lambda \in K^* $. On a ainsi prouvé (ii).

$ d) $ Les parties $ a) $ et $ c) $ de la démonstration prouvent que $ D $ est anti-invariant par $ G $. Alors, si $ y \in R $, il est clair que $ yD $ est anti-invariant par $ G $. Enfin, si $ z \in S $ est anti-invariant par $ G $, on a vu en $ b) $ qu’il existe $ y \in S $ tel que $ z = yD $. Comme $ S $ est intègre, on a $ y \in R $. Ceci achève de prouver (i).

### \*5. Compléments (*)

#### Lemme 4 {#lie-v-s5-lem-4 .statement}

Soient $ K $ un corps commutatif, $ V $ un espace vectoriel de dimension finie sur $ K $, $ G $ un groupe fini d’automorphismes de $ V $ d’ordre $ q $ inversible dans $ K $, $ S $ l’algèbre symétrique de $ V $, $ R $ la sous-algèbre de $ S $ formée des éléments invariants par $ G $. Pour qu’un idéal premier $ \mathfrak{P} $ de hauteur 1 de $ S $ soit ramifié sur $ \mathfrak{p} = \mathfrak{P} \cap R $ (Alg. comm.), il faut et il suffit qu’il existe un élément non nul $ a $ de $ V $ et un élément non nul $ f $ de $ V^* $ tels que $ \mathfrak{P} = Sa $ et que la pseudo-réflexion $ s_{a,f} $ appartienne à $ G $. Le groupe de décomposition $ G^z(\mathfrak{P}) $ est alors le sous-groupe des éléments de $ G $ laissant $ Ka $ stable, et le groupe d’inertie $ G^T(\mathfrak{P}) $ est le sous-groupe cyclique $ H_a $ de $ G $ formé des pseudo-réflexions de $ G $ de vecteur $ a $. Le corps résiduel $ S(\mathfrak{P}) $ de $ S $ en $ \mathfrak{P} $ est séparable sur le corps résiduel $ R(\mathfrak{p}) $ de $ R $ en $ \mathfrak{p} $, et l’indice de ramification $ e(\mathfrak{P}/\mathfrak{p}) $, égal au coefficient de $ \mathfrak{P} $, augmenté de 1, dans le diviseur $ \operatorname{div}(\mathcal{D}_{S/R}) $ de la différente, est égal à $ \operatorname{Card}(H_a) $.

Dire que $ \mathfrak{P} $ est ramifié sur $ R $ signifie que son groupe d’inertie $ G^T(\mathfrak{P}) $ n’est pas réduit à l’identité, autrement dit qu’il existe $ g \neq 1 $ dans $ G $ tel que $ g(z) \equiv z \pmod{\mathfrak{P}} $ pour tout $ z \in S $. Comme $ S $ est un anneau factoriel, $ \mathfrak{P} $ est un idéal principal $ Sa $, et $ a $ doit diviser tous les éléments $ g(z) - z $ ($ z \in S $); or, pour $ z \in V $, ceux-ci sont homogènes de degré 1 et non tous nuls (car $ g \neq 1 $); donc $ a $ doit être homogène de degré 1, autrement dit $ a \in V $. Il existe alors une forme linéaire $ f $ sur $ V $ telle que $ g = s_{a,f} $. Inversement, si $ g $ est une pseudo-réflexion $ s_{a,f} $ distincte de 1, on a $ g(z) \equiv z \pmod{Sa} $ pour tout $ z \in S $, donc $ g $ appartient au groupe d’inertie de l’idéal premier $ \mathfrak{P} = Sa $. Ceci prouve la première assertion du lemme et les caractérisations de $ G^z(\mathfrak{P}) $ et $ G^T(\mathfrak{P}) $. On sait que le degré résiduel $ [S(\mathfrak{P}) : R(\mathfrak{p})] $ divise $ \operatorname{Card}(G) = q $ (Alg. comm., chap. V, § 2, no 2); comme $ q $ est étranger à l’exposant caractéristique $ p $ de $ K $ (qui est celui aussi de $ S(\mathfrak{P}) $), l’extension $ S(\mathfrak{P}) $ de $ R(\mathfrak{p}) $ est séparable. L’égalité $ e(\mathfrak{P}/\mathfrak{p}) = \operatorname{Card}(H_a) $ en résulte (Alg. comm.). Comme $ e(\mathfrak{P}/\mathfrak{p}) $ est étranger à $ p $, le coefficient de $ \mathfrak{P} $ dans $ \operatorname{div}(\mathcal{D}_{S/R}) $ est $ e(\mathfrak{P}/\mathfrak{p}) - 1 $ (Alg. comm.). Ceci achève la démonstration du lemme.

#### Lemme 5 {#lie-v-s5-lem-5 .statement}

Soient $ K $ un corps commutatif, $ S $ une $ K $-algèbre graduée de polynômes et $ R $ une sous-algèbre graduée de $ S $. Pour que $ S $ soit un $ R $-module libre gradué (Alg.,

(*) Dans ce numéro, nous utilisons des résultats figurant dans des chapitres en préparation du livre d’Algèbre commutative. Nous y renvoyons par le sigle « Alg. comm. ».

chap. II, 3e éd. § 11, no 2), il faut et il suffit que les deux conditions suivantes soient vérifiées:

a) R est une K-algèbre graduée de polynômes;
b) si (\alpha_1, \ldots, \alpha_s) est un système générateur de la K-algèbre R formée d’éléments homogènes et algébriquement indépendants, ce système est une suite S-régulière (*).
Lorsque S est un R-module de type fini, b) est conséquence de a).
Pour la démonstration, voir Alg. comm.

#### Théorème 4 {#lie-v-s5-thm-4 .statement}

Soient K un corps commutatif, V un espace vectoriel de dimension finie sur K, S l’algèbre symétrique de V, G un groupe fini d’automorphismes de V, et R la sous-algèbre de S formée des éléments invariants par G. On suppose que q = Card G est inversible dans K. Les conditions suivantes sont équivalentes :

(i) G est engendré par des pseudo-réflexions;
(ii) S est un R-module libre gradué;
(iii) R est une K-algèbre graduée de polynômes.

L’équivalence de (ii) et (iii) résulte du no 2 et du lemme 5. L’implication (i) $ \Longrightarrow $ (ii) résulte du th. 1.

Montrons que (iii) $ \Longrightarrow $ (i). Soit G’ le sous-groupe de G engendré par les pseudo-réflexions appartenant à G, et soit R’ la sous-algèbre de S formée des éléments invariants par G’. On a R $ \subset $ R’ $ \subset $ S. D’après le lemme 4, on a div(\mathcal{D}_{S/R}) = div(\mathcal{D}_{S/R'}), d’où div(\mathcal{D}_{R'/R}) = 0. Supposons alors que R soit une algèbre graduée de polynômes. Comme c’est aussi le cas pour R’ (puisque G’ est engendré par des pseudo-réflexions), le lemme 5 montre que le R-module R’ admet une base homogène (Q_1, \ldots, Q_m); soit q_i = deg(Q_i). Posons

$$
d = \det(\mathrm{Tr}_{R'/R}(Q_i Q_j)), \quad \text{cf. Alg., chap. IX, § 2.}
$$

Le fait que div(\mathcal{D}_{R'/R}) soit nul montre que div(d) = 0 (Alg. comm.), ce qui signifie que d appartient à K*. Mais d’autre part Tr_{R'/R}(Q_i Q_j) est un élément homogène de degré q_i + q_j, et d est homogène de degré 2 $ \sum_i q_i $. On a donc $ \sum_i q_i = 0 $, i.e. $ q_i = 0 $ pour tout i, ce qui entraîne R’ = R, d’où G’ = G d’après la théorie de Galois. On a donc bien prouvé que G est engendré par des pseudo-réflexions. C.Q.F.D.

#### Remarque 1 {#lie-v-s5-n5-rem-1 .statement}

Sous les hypothèses du th. 4, les degrés caractéristiques de R ont pour produit q (formule (6) et prop. 2 (iii)), donc sont étrangers à l’exposant caractéristique de K. C’est ce qu’on avait annoncé au no 3.
2) Lorsqu’on ne suppose plus que Card (G) est inversible dans K, on a encore (ii) $ \Longleftrightarrow $ (iii) (cf. lemme 5) et (ii) $ \Longrightarrow $ (i) (cf. exerc. 8); l’implication (i) $ \Longrightarrow $ (ii) n’est par contre plus vraie (exerc. 9).

(*) Cela signifie que, pour tout i $ \in \{1, 2, \ldots, s\} $, l’image canonique de $ \alpha_i $ dans l’anneau

$$
S/(S\alpha_1 + \cdots + S\alpha_{i-1})
$$

est non diviseur de zéro dans cet anneau.

#### Proposition 6 {#lie-v-s5-prop-6 .statement}

Les hypothèses et les notations sont celles du th. 4. Soit $ H $ l’ensemble des pseudo-réflexions appartenant à $ G $ et distinctes de 1. On suppose que $ H $ engendre $ G $. Pour tout $ g \in H $, posons $ g(x) = x + f_g(x)e_g $ avec $ e_g \in V $, $ f_g \in V^* $. Posons

$$
D = \prod_{g \in H} e_g \in S.
$$

(i) La différente de $ S $ sur $ R $ est l’idéal principal $ SD $.

(ii) Supposons $ S $ identifiée à l’algèbre $ K[X_1, \ldots, X_l] $ par le choix d’une base $ (X_1, \ldots, X_l) $ de $ V $, et soient $ P_1, \ldots, P_l $ des éléments homogènes algébriquement indépendants engendrant l’algèbre $ R $. Alors le jacobien $ J = \det \left( \frac{\partial P_i}{\partial X_j} \right) $ est de la forme $ \lambda D $ où $ \lambda \in K^* $.

(iii) On a $ \sum_{i=1}^l (\deg(P_i) - 1) = \mathrm{Card}(H) $.

(iv) L’ensemble des éléments anti-invariants de $ S $ est RD.

L’assertion (i) résulte du lemme 4. L’assertion (ii) résulte de ce que $ SJ $ est la différente de $ S $ sur $ R $ (*Alg. comm.*). L’assertion (iii) s’obtient en écrivant que les polynômes homogènes $ D $ et $ J $ ont même degré. La démonstration de (iv) est alors la même qu’au n° 4 (démonstration de la prop. 5, parties $ b $ et $ d $).*

## EXERCICES {#lie-v-s5-exercises}

See the [exercises for § 5](exercises/s5/).
