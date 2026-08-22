---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: Diviseurs
section: 2
section_title: Anneaux de Dedekind
lang: fr
source: ac-v-vii-fr
pdf_pages: 0216-0226, 0285-0291
extraction: ocr
subsections:
    - "no": 1
      title: Définition des anneaux de Dedekind
      page: 0
      pdf_page: 216
    - "no": 2
      title: Caractérisations des anneaux de Dedekind
      page: 0
      pdf_page: 217
    - "no": 3
      title: Décomposition des idéaux en produits d’idéaux premiers
      page: 0
      pdf_page: 219
    - "no": 4
      title: Théorème d’approximation dans les anneaux de Dedekind
      page: 0
      pdf_page: 220
    - "no": 5
      title: Le théorème de Krull–Akizuki.
      page: 0
      pdf_page: 223
statements: 7
exercises: 22
content_sha256: ca07e8b1d8b1b676a1563a0874d08ea738fecb16f6c8961570e03eca10533b66
---

## § 2. Anneaux de Dedekind

### 1. Définition des anneaux de Dedekind

Soit $ A $ un anneau intègre. Il est clair que les conditions suivantes sont équivalentes :
a) les idéaux premiers non nuls de $ A $ sont deux à deux non comparables pour la relation d’inclusion ;
b) les idéaux premiers non nuls de $ A $ sont maximaux ;
c) les idéaux premiers non nuls de $ A $ sont de hauteur 1.

#### Définition 1 {#ac-vii-s2-def-1 .statement}

On appelle anneau de Dedekind un anneau de Krull dont tous les idéaux premiers non nuls sont maximaux.

Exemples d’anneaux de Dedekind. — 1) Tout anneau principal est un anneau de Dedekind.

2) Soient K une extension de degré fini de Q, et A la fermeture intégrale de Z dans K. L’anneau A est un anneau de Krull (§ 1, n° 8, prop. 12). Soit p un idéal premier non nul de A. Alors p ∩ Z est non nul (chap. V, § 2, n° 1, cor. de la prop. 1), donc est un idéal maximal de Z ; donc p est un idéal maximal de A (loc. cit., prop 1). Par suite, A est un anneau de Dedekind. En général, A n’est pas principal (Alg., chap. VII, § 1, exerc. 12).

3) *Soient V une variété algébrique affine, et A l’anneau des fonctions régulières sur A. Supposons que A ne soit pas un corps (i.e., que V ne soit pas réduite à un point). Pour que A soit un anneau de Dedekind, il faut et il suffit que V soit une courbe irréductible sans point singulier : en effet, dire que A est intègre revient à dire que V est irréductible ; dire que tout idéal premier non nul de A est maximal revient à dire que A est une courbe ; enfin, comme A est noethérien, dire que c’est un anneau de Krull revient à dire qu’il est intégralement clos, c’est-à-dire que V est une courbe normale, ou encore sans point singulier. \*

4) Un anneau de fractions S^{-1}A d’un anneau de Dedekind A est un anneau de Dedekind si 0 \notin S. En effet, S^{-1}A est un anneau de Krull (§ 1, n° 4, prop. 6), et tout idéal premier non nul de S^{-1}A est maximal d’après le chap. II, § 2, n° 5, prop. 11.

### 2. Caractérisations des anneaux de Dedekind

#### Théorème 1 {#ac-vii-s2-thm-1 .statement}

Soient A un anneau intègre, K son corps des fractions. Les conditions suivantes sont équivalentes :

a) A est un anneau de Dedekind ;
b) A est un anneau de Krull, et toute valuation non impropre de K qui est positive sur A est équivalente à une valuation essentielle de A ;
c) A est un anneau de Krull, et tout idéal fractionnaire $ \mathfrak{J} \neq (0) $ de A est divisoriel ;
d) tout idéal fractionnaire $ \mathfrak{J} \neq (0) $ de A est inversible ;
e) A est noethérien, intégralement clos, et tout idéal premier non nul de A est maximal ;
f) A est noethérien, et, pour tout idéal maximal m de A, $ A_m $ est un corps ou un anneau de valuation discrète ;
g) A est noethérien, et, pour tout idéal maximal m de A, $ A_m $ est principal.

Démontrons d’abord l’équivalence de a) et de b). Le cor. 2

Le reste de la démonstration se fait suivant le schéma logique
$$
a) \Rightarrow c) \Rightarrow d) \Rightarrow e) \Rightarrow f) \Rightarrow g) \Rightarrow a).
$$

Si $A$ est un anneau de Dedekind, et si $b$ est un idéal fractionnaire non nul, on a $bA_p = \tilde{b}A_p$ pour tout idéal maximal $p$ ($§ 1$, n° 4, prop. 7), donc $b = \tilde{b}$ (chap. II, § 3, n° 3, cor. 3 du th. 1); ainsi $a)$ implique $c$).

Montrons que $c)$ implique $d)$. Si $c)$ est vraie, l’application $a \to \operatorname{div} a$ est une bijection de $I(A)$ sur $D(A)$ (cf. § 1, n° 1); comme c’est un homomorphisme ($§ 1$, n° 2) et que $D(A)$ est un groupe, tout élément de $I(A)$ est bien inversible.

Montrons que $d)$ implique $e)$. Si $d)$ est vraie, tout idéal entier $\neq (0)$ de $A$ est de type fini (chap. II, § 5, n° 6, th. 4), donc $A$ est noethérien; comme $I(A)$ est un groupe, $D(A)$ est un groupe, et $A$ est donc complètement intégralement clos ($§ 1$, n° 2, th. 1). Enfin, si $p$ est un idéal premier non nul de $A$, et si $m$ est un idéal maximal de $A$ contenant $p$, l’anneau $A_m$ est principal (chap. II, § 5, n° 6, th. 4); comme $pA_m$ est premier non nul, on a nécessairement $pA_m = mA_m$ (un anneau principal étant un anneau de Dedekind), d’où $p = m$ (chap. II, § 2, n° 5, prop. 11), et $p$ est maximal.

Montrons que $e)$ implique $f)$. En effet, si $m$ est un idéal maximal de $A$, et si $e)$ est vraie, $A_m$ est un anneau noethérien intégralement clos, et son idéal maximal $mA_m$ est, ou bien $(0)$, ou bien le seul idéal premier non nul de $A_m$; donc $A_m$ est un corps ou un anneau de valuation discrète d’après la prop. 11 du § 1, n° 7.

Le fait que $f)$ implique $g)$ est évident.

Montrons enfin que $g)$ implique $a)$. Comme $A$ est l’intersection des $A_m$, où $m$ parcourt l’ensemble des idéaux maximaux (chap. II, § 3, n° 3, cor. 4 du th. 1), $g)$ implique que $A$ est intégralement clos et noethérien, donc que $A$ est un anneau de Krull ($§ 1$, n° 3, cor. du th. 2). D’autre part, on montre que tout idéal premier non nul de $A$ est maximal comme dans la démonstration de $d) \Rightarrow e)$.

C.Q.F.D.

PROPOSITION 1. — *Un anneau de Dedekind semi-local est principal.*

Soient $A$ un anneau de Dedekind semi-local, $K$ son corps des fractions, $ p_1, \ldots, p_n $ ses idéaux maximaux, et $ v_1, \ldots, v_n $ les valuations essentielles correspondantes; ce sont les seules valuations essentielles de A. Soit $ \alpha $ un idéal entier non nul de A. Puisqu’il est divisoriel, il existe ($ \S 1 $, no 4, prop. 5) des entiers $ q_1, \ldots, q_n $ tels que $ \alpha $ soit l’ensemble des $ x \in K $ tels que $ v_i(x) \geq q_i $ pour $ 1 \leq i \leq n $. Soit $ x_0 $ un élément de K tel que $ v_i(x_0) = q_i $ pour $ 1 \leq i \leq n $ (chap. VI, $ \S 7 $, no 2, cor. 1 du th. 1). Alors $ \alpha $ est l’ensemble des $ x \in K $ tels que $ v_i(xx_0^{-1}) \geq 0 $ pour $ 1 \leq i \leq n $. Ainsi $ \alpha = Ax_0 $.

Si A est un anneau de Dedekind, on a vu, dans la démonstration du th. 1, que le groupe D(A) des diviseurs de A s’identifie au groupe I(A) des idéaux fractionnaires $ \alpha \neq (0) $ (comme A est noethérien, tout idéal fractionnaire non nul est de type fini). Le groupe C(A) des classes de diviseurs de A ($ \S 1 $, no 2) s’identifie alors au groupe des classes d’idéaux $ \neq 0 $ de A (défini au chap. II, $ \S 5 $, no 7).

### 3. Décomposition des idéaux en produits d’idéaux premiers

Soient A un anneau de Dedekind, I(A) le groupe multiplicatif ordonné des idéaux fractionnaires non nuls de A, et D(A) le groupe des diviseurs de A. L’isomorphisme $ \alpha \to \operatorname{div} \alpha $ de I(A) sur D(A) fait correspondre les diviseurs extrémaux aux idéaux premiers non nuls de A ($ \S 1 $, no 6, th. 3), donc le groupe multiplicatif I(A) admet pour base l’ensemble des idéaux premiers non nuls de A ($ \S 1 $, no 3, th. 2). Autrement dit, tout idéal fractionnaire non nul $ \alpha $ de A admet une décomposition et une seule de la forme:
$$
\alpha = \prod p^{n(p)}
$$
où le produit est étendu aux idéaux premiers non nuls de A, les exposants $ n(p) $ étant nuls à l’exception d’un nombre fini d’entre eux. De plus $ \alpha $ est entier si et seulement si les $ n(p) $ sont tous positifs. On dit que la relation (1) est la décomposition de $ \alpha $ en facteurs premiers. En particulier, si $ \alpha $ est un idéal principal $ Ax $, on a, pour tout $ p $, $ n(p) = v_p(x) $, où $ v_p $ désigne la valuation essentielle correspondant à $ p $; ceci résulte en effet de la formule (4) du $ \S 1 $, no 3. Soient
$$
\alpha = \prod p^{m(p)}, \quad b = \prod p^{n(p)}
$$
deux idéaux fractionnaires non nuls de A. On a alors:
$$
\alpha b = \prod p^{m(p) + n(p)}
$$

(3) $ a : b = ab^{-1} = \prod p^{m(p)-n(p)} $
(4) $ a + b = \prod p^{\inf(m(p), n(p))} $
(5) $ a \cap b = \prod p^{\sup(m(p), n(p))} $.

En effet, la relation (2) est évidente; la relation (3) en résulte, l’égalité $ a : b = ab^{-1} $ découlant de la formule
$$
\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b
$$
(\S 1, n° 2, cor. du th. 1); les formules (4) et (5) résultent de la prop. 2, \S 1, n° 1.

Ces résultats s’appliquent notamment à la clôture intégrale de $ \mathbf{Z} $ dans une extension de degré fini de $ \mathbf{Q} $.
Lorsque A est principal, les résultats ci-dessus redonnent ceux d’Alg., chap. VII, \S 1, n° 3.

### 4. Théorème d’approximation dans les anneaux de Dedekind

Dans les anneaux de Dedekind, on a un « théorème d’approximation » qui améliore à la fois le th. 1 du chap. VI, \S 7, n° 2 et la prop. 9 du \S 1, n° 5:

#### Proposition 2 {#ac-vii-s2-prop-2 .statement}

*Soient A un anneau de Dedekind, K son corps des fractions, et P l’ensemble des idéaux premiers non nuls de A; pour $ p \in P $, notons $ v_p $ la valuation essentielle correspondante de A. Soient $ p_1, \ldots, p_q $ des éléments deux à deux distincts de P, $ n_1, \ldots, n_q $ des entiers rationnels, et $ x_1, \ldots, x_q $ des éléments de K. Il existe alors $ x \in K $ tel que $ v_{p_i}(x - x_i) \geq n_i $ pour $ 1 \leq i \leq q $, et que $ v_p(x) \geq 0 $ pour tout $ p \in P $ distinct des $ p_i $.*

En remplaçant au besoin les $ n_i $ par des entiers qui leur sont supérieurs, on peut les supposer tous positifs. Examinons d’abord le cas où les $ x_i $ sont dans A; tout revient évidemment à trouver un $ x \in A $ vérifiant les congruences
$$
x \equiv x_i \pmod{p_i^{n_i}}
$$
et l’existence de x résulte alors du chap. II, \S 1, n° 2, prop. 5.

Passons au cas général. On peut écrire $ x_i = s^{-1} y_i $ avec s, $ y_i $ dans A; posant $ x = s^{-1} y $, tout revient à trouver un $ y \in A $ tel que l’on ait, d’une part, $ v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s) $, et, d’autre part, $ v_p(y) \geq v_p(s) $ pour tout $ p \in P $ distinct des $ p_i $; comme $ v_p(s) = 0 $ sauf pour un nombre fini d’indices $ p $, on est ainsi ramené au cas précédent; d’où la proposition.

Pour tout $ x \in K $, soit $ \Delta(x) $ l’élément $ (x_p) \in \prod_{p \in P} \hat{K}_p $ tel que $ x_p = x $ pour tout $ p \in P $; comme $ x_p \in \hat{A}_p $ sauf pour un nombre fini de valeurs de $ p $, on a $ \Delta(x) \in A $; on définit donc ainsi un homomorphisme $ \Delta : K \to A $, qui est injectif si $ P \neq \emptyset $ (c’est-à-dire si $ A $ n’est pas un corps); les éléments de $ \Delta(K) $ sont dits adèles restreints principaux, et il est clair que $ \Delta(A) \subset A_0 $. Dans la suite de ce numéro, nous supposerons que $ A $ n’est pas un corps.

PROPOSITION 3. — L’anneau $ A_0 $ (resp. $ A $) s’identifie au complété de $ A $ (resp. $ K $) pour la topologie d’anneau dont un système fondamental de voisinages de 0 est formé de tous les idéaux entiers $ \neq (0) $ de $ A $.

On pourrait naturellement aussi prouver que $ \Delta(K) $ est dense dans $ A $ en utilisant la prop. 2.

Considérons maintenant le groupe multiplicatif $ SL(n, A) $, formé des matrices $ U \in M_n(A) $ telles que $ \det(U) = 1 $; si on munit $ M_n(A) = A^{n^2} $ de la topologie produit, elle induit sur $ SL(n, A) $ une topologie compatible avec la structure de groupe de $ SL(n, A) $. En effet, il suffit de voir que l’application $ U \to U^{-1} $ est continue dans $ SL(n, A) $; mais comme $ U $ est unimodulaire, on sait (Alg., chap. III, § 6, n° 5, formule (17)) que les éléments de $ U^{-1} $ sont des mineurs de $ U $, donc des polynômes en les éléments de $ U $, ce qui prouve notre assertion. Si on identifie $ K $ à un sous-anneau de $ A $ au moyen de $ \Delta $, le groupe $ SL(n, K) $ est un sous-groupe de $ SL(n, A) $.

PROPOSITION 4. — *Le groupe $ SL(n, K) $ est dense dans $ SL(n, A) $*.

Soit $ G $ l’adhérence de $ SL(n, K) $ dans $ SL(n, A) $; comme $ K $ est dense dans $ A $ (prop. 3), $ G $ contient toutes les matrices de la forme $ I + a . E_{ij} $ pour $ i \neq j $ et $ a \in A $. Pour tout $ p \in P $ et tout $ \lambda \in \hat{K}_p $, soit $ \lambda(p) $ l’adèle restreint $ x = (x_q)_{q \in P} $ tel que $ x_p = \lambda $ et $ x_q = 0 $ pour $ q \neq p $; ce qui précède montre que $ G $ contient les matrices $ I + \lambda(p)E_{ij} $ pour $ i \neq j $. Mais, on sait que les matrices de la forme $ I + \lambda E_{ij} $, pour $ \lambda \in \hat{K}_p $, engendrent le groupe $ SL(n, \hat{K}_p) $ (Alg., chap. III, 3e éd.) Pour toute matrice $ U \in SL(n, A) $, désignons par $ U_p $ l’image canonique de $ U $ dans $ SL(n, \hat{K}_p) $; on voit donc que pour tout $ p \in P $, $ G $ contient les matrices $ U \in SL(n, A) $ telles que $ U_q = I $ pour tout $ q \neq p $. Puisque $ G $ est un groupe, il contient aussi toutes les matrices $ U \in SL(n, A) $ telles que $ U_p = I $ sauf pour un nombre *fini* de $ p \in P $; or, la définition de la topologie de $ A $ montre aussitôt que l’ensemble de ces matrices est dense dans $ SL(n, A) $.

### 5. Le théorème de Krull–Akizuki.

#### Lemme 1 {#ac-vii-s2-lem-1 .statement}

Soient $ A $ un anneau noethérien intègre dans lequel tout idéal premier non nul est maximal, et $ M $ un $ A $-module de torsion de type fini. Alors la longueur $ \operatorname{long}_A(M) $ de $ M $ est finie.

En effet, comme $ M $ est un module de torsion, tout idéal premier associé à $ M $ est $ \neq (0) $, donc maximal. Le lemme résulte alors du chap. IV, § 2, n° 5, prop. 7.

#### Lemme 2 {#ac-vii-s2-lem-2 .statement}

Soient $ A $ un anneau, $ T $ un $ A $-module, $ (T_j) $ une famille filtrante croissante de sous-modules de $ T $, de réunion $ T $. Alors $ \operatorname{long}_A(T) = \sup (\operatorname{long}_A(T_j)) $.

On a $ \operatorname{long}_A(T_j) \leq \operatorname{long}_A(T) $ pour tout $ j $. Le lemme est évident si aucun entier ne majore les $ \operatorname{long}_A(T_j) $, les deux membres étant alors infinis. Sinon, soit $ i_0 $ un indice pour lequel $ \operatorname{long}_A(T_{i_0}) $ prenne sa plus grande valeur; on a $ T_{i_0} = T $ puisque la famille $ (T_j) $ est filtrante; d’où notre assertion dans ce cas.

#### Remarque {#ac-vii-s2-n5-rem-1 .statement}

Cette démonstration ne suppose pas $ A $ commutatif.

#### Lemme 3 {#ac-vii-s2-lem-3 .statement}

Soient $ A $ un anneau intègre noethérien tel que tout idéal premier non nul de $ A $ soit maximal, $ M $ un $ A $-module sans torsion de rang fini $ r $, et $ a $ un élément non nul de $ A $. Alors $ A/Aa $ est un $ A $-module de longueur finie, et on a:

$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$

Le lemme 1 montre que $ \operatorname{long}_A(A/Aa) $ est finie. Démontrons d’abord (6) dans le cas où $ M $ est de type fini. Comme $ M $ est sans torsion et de rang $ r $, il existe un sous-module $ L $ de $ M $ isomorphe à $ A' $ et tel que $ Q = M/L $ soit un $ A $-module de torsion de type fini, donc de longueur finie (lemme 1). Pour tout entier $ n \geq 1 $, le noyau de la surjection canonique $ M/a^nM \to Q/a^nQ $ est égal à $ (L + a^nM)/a^nM $, isomorphe à $ L/(a^nM \cap L) $; comme $ a^nL \subset a^nM \cap L $, on a donc

$$
\operatorname{long}_A(M/a^nM) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ)
$$
$$
\leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$

Or, puisque $ M $ est sans torsion, la multiplication par $ a $ définit un isomorphisme de $ M/aM $ sur $ aM/a^2M $; de même pour $ L $; d’où, par récurrence sur $ n $, les formules :

$$
\text{(8)} \quad \begin{aligned}
& \operatorname{long}_A(M/a^nM) = n \cdot \operatorname{long}_A(M/aM), \\
& \operatorname{long}_A(L/a^nL) = n \cdot \operatorname{long}_A(L/aL).
\end{aligned}
$$

Tenant compte de (7), on en déduit:

$$
\text{(9)} \quad \operatorname{long}_A(M/aM) \leq \operatorname{long}_A(L/aL) + n^{-1} \operatorname{long}_A(Q)
$$
pour tout $ n > 0 $; comme $ L $ est isomorphe à $ A' $, on a $ \operatorname{long}_A(L/aL) = r \operatorname{long}_A(A/Aa) $; d’où (6) en faisant tendre $ n $ vers l’infini dans (9).

Passons maintenant au cas général. Soit $ (M_i) $ la famille des sous-modules de type fini de $ M $. Le module $ T = M/aM $ est réunion des sous-modules $ T_i = (M_i + aM)/aM = M_i/(M_i \cap aM) $. Or, $ T_i $ est isomorphe à un quotient de $ M_i/aM_i $, donc

$$
\operatorname{long}_A(T_i) \leq r \operatorname{long}_A(A/Aa)
$$
en vertu de ce qu’on vient de prouver. D’où

$$
\operatorname{long}_A(T) \leq r \operatorname{long}_A(A/Aa)
$$
d’après le lemme 2.

C.Q.F.D.

PROPOSITION 5 (Krull-Akizuki). — Soient $ A $ un anneau intègre noethérien dont tout idéal premier non nul est maximal, $ K $ son corps des fractions, $ L $ une extension de degré fini de $ K $, et $ B $ un sous-anneau de $ L $ contenant $ A $. Alors $ B $ est noethérien, et tout idéal premier non nul de $ B $ est maximal. En outre, pour tout idéal $ b \neq (0) $ de $ B $, $ B/b $ est un $ A $-module de type fini.

Soit $ b $ un idéal non nul de $ B $. Nous allons montrer que $ B/b $ est un $ A $-module de longueur finie (donc, $ a $ fortiori, un $ B $-module de longueur finie), et que $ b $ est un $ B $-module de type fini.

Un élément non nul $ y $ de $ b $ vérifie une équation de la forme:

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_0 = 0 \quad (a_i \in A, \ a_0 \neq 0).
$$

Cette équation montre que $ a_0 \in By \subset b $. En appliquant le lemme 3 à $ M = B $, on voit que $ B/a_0B $ est un $ A $-module de longueur finie; il en est de même de $ B/b $, qui en est un module quotient. De plus le $ B $-module $ b $ contient, comme sous-module, $ a_0B $ qui est de type fini; comme $ b/a_0B $ est de longueur finie (en tant que sous-module de $ B/a_0B $), donc de type fini, $ b $ est bien un $ B $-module de type fini.

Ce qui précède montre d’abord que $ B $ est noethérien. D’autre part, si $ p $ est un idéal premier non nul de $ B $, l’anneau $ B/p $ est intègre et de longueur finie, donc est un corps ($ Alg. $, chap. VIII, § 6, n° 4; prop. 9), de sorte que $ p $ est maximal.

C.Q.F.D.

COROLLAIRE 1. — Pour tout idéal premier $ p $ de $ A $, l’ensemble des idéaux premiers de $ B $ au-dessus de $ p $ est fini.

Supposons d’abord $ p = (0) $; alors le seul idéal premier $ q $ de $ B $ tel que $ q \cap A = (0) $ est $ (0) $; sinon, en posant $ S = A - \{0\} $, $ S^{-1}q $ serait un idéal premier non nul de $ S^{-1}B $ (chap. II, § 2, no 5, prop. 11), et $ S^{-1}B $ n’est autre que le corps des fractions de $ B $, car c’est un sous-anneau de $ L $ contenant $ K $ (Alg., chap. V, § 3, no 2, prop. 3); d’où une conclusion absurde. Si maintenant $ p \neq (0) $, il résulte de la prop. 5 que $ B/pB $ est un espace vectoriel de dimension finie sur le corps $ A/p $, donc un anneau artinien, et par suite n’a qu’un nombre fini d’idéaux premiers (chap. IV, § 2, no 5, prop. 9), ce qui prouve qu’il n’y a qu’un nombre fini d’idéaux premiers de $ B $ contenant $ p $.

COROLLAIRE 2. — La fermeture intégrale de $ A $ dans $ L $ est un anneau de Dedekind.

Cette fermeture intégrale est, en effet, un anneau noethérien intégralement clos dont les idéaux premiers non nuls sont maximaux ; il suffit donc d’appliquer le th. 1 du no 2.

En particulier :

COROLLAIRE 3. — La fermeture intégrale d’un anneau de Dedekind dans une extension de degré fini de son corps des fractions est un anneau de Dedekind.

PROPOSITION 6. — Soient $ A $ un anneau de Dedekind, $ K $ son corps des fractions, $ L $ une extension de degré fini de $ K $, et $ B $ la fermeture intégrale de $ A $ dans $ L $. Soient $ p $ un idéal premier non nul de $ A $, $ v $ la valuation essentielle de $ K $ correspondante, et

$$
Bp = \prod_i p_i^{e(i)}
$$

la décomposition de l’idéal $ Bp $ en produit d’idéaux premiers. Alors :

a) les idéaux premiers de $ B $ au-dessus de $ p $ sont les $ p_i $ tels que $ e(i) > 0 $;

b) les valuations $ v_i $ de $ L $ correspondant à ces idéaux $ p_i $ sont, à une équivalence près, les valuations de $ L $ prolongeant $ v $;

c) on a $[B/p_i : A/p] = f(v_i/v)$;

d) on a $ e(i) = e(v_i/v) $ (cf. chap. VI, § 8, no 1, déf. 1 et 2).

a) Dire qu’un idéal premier $ q $ de $ B $ est au-dessus de $ p $ revient à dire que $ q \supset p $, donc que $ q \supset Bp $, donc que $ q $ contient l’un des $ p_i $ tels que $ e(i) > 0 $ (chap. II, § 1, no 1, prop. 1).

c) Le corps résiduel de $v$ s’identifie à $A/\mathfrak{p}$, et celui de $v_i$ à $B/\mathfrak{p}_i$ ($§ 1$, n° 4, cor. 1 de la prop. 6).

d) Soit $a$ (resp. $a_i$) une uniformisante pour $v$ (resp. $v_i$). On a
$$
a B_{\mathfrak{p}_i} = a A_p B_{\mathfrak{p}_i} = p A_p B_{\mathfrak{p}_i} = p B . B_{\mathfrak{p}_i} = \left( \prod_j p_j^{e(j)} \right) B_{\mathfrak{p}_i}
$$
$$
= \prod_j (p_j B_{\mathfrak{p}_i})^{e(j)} = (p_i B_{\mathfrak{p}_i})^{e(i)} = a_i^{e(i)} B_{\mathfrak{p}_i}
$$
puisque $p_j B_{\mathfrak{p}_i} = B_{\mathfrak{p}_i}$ pour $j \neq i$; d’où $d$), puisque $e(v_i/v) = v_i(a)$.

## EXERCICES {#ac-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
