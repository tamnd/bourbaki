---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: Entiers
section: 3
section_title: Algèbres de type fini sur un corps
lang: fr
source: ac-v-vii-fr
pdf_pages: 0054-0065, 0080-0083
extraction: ocr
subsections:
    - "no": 1
      title: Le lemme de normalisation
      page: 0
      pdf_page: 54
    - "no": 2
      title: Fermeture intégrale d’une algèbre de type fini sur un corps
      page: 0
      pdf_page: 59
    - "no": 3
      title: Le théorème des zéros
      page: 0
      pdf_page: 60
    - "no": 4
      title: Anneaux de Jacobson
      page: 0
      pdf_page: 62
statements: 11
exercises: 10
content_sha256: 0c4075dcd7d328f0f7f05fce1be185e129f678a0ccf3e298c0a3427101c4e74f
---

## § 3. Algèbres de type fini sur un corps.

### 1. Le lemme de normalisation

Dans ce numéro et le suivant, $ k $ désigne un corps commutatif.

#### Théorème 1 {#ac-v-s3-thm-1 .statement}

(Lemme de normalisation.) Soit $ A $ une $ k $-algèbre de type fini, et soit $ a_1 \subset a_2 \subset \ldots \subset a_p $ une suite finie croissante d’idéaux de $ A $ telle que $ p \geqslant 1 $ et $ a_p \neq A $. Il existe une suite finie $ (x_i)_{1 \leq i \leq n} $ d’éléments de $ A $, algébriquement indépendants sur $ k $ (chap. III, § 1, no 1) et tels que :

a) $ A $ soit entier sur l’anneau $ B = k[x_1, \ldots, x_n] $.

b) Il existe une suite croissante $ (h(j))_{1 \leq j \leq p} $ d’entiers telle que, pour tout $ j $ l’idéal $ a_j \cap B $ de $ B $ soit engendré par $ x_1, \ldots, x_{h(j)} $.

Remarquons d’abord qu’il suffit de démontrer le théorème lorsque $ A $ est une algèbre de polynômes $ k[Y_1, \ldots, Y_m] $. En effet, dans le cas général, $ A $ est isomorphe au quotient d’une telle algèbre $ A' $ par un idéal $ a'_0 $; notons $ a'_j $ l’image réciproque de $ a_j $ dans $ A' $ et soient $ x'_i (1 \leq i \leq r) $ des éléments de $ A' $ vérifiant les conditions de l’énoncé pour l’anneau $ A' $ et la suite croissante d’idéaux $ a'_0 \subset a'_1 \subset \cdots \subset a'_p $. Alors les images $ x_i $ des $ x'_i $ dans $ A $ pour $ i > h(0) $ vérifient les conditions voulues; c’est évident pour la condition b), et pour la condition a) cela résulte du § 1, no 1, prop. 2; enfin, si les $ x_i (h(0) + 1 \leq i \leq r) $ n’étaient pas algébriquement indépendants sur $ k $, il y aurait un polynôme non nul $ Q \in k[X_{h(0)+1}, \ldots, X_r] $ tel que $ Q(x'_{h(0)+1}, \ldots, x'_r) \in a'_0 \cap B' $, en posant $ B' = k[x'_1, \ldots, x'_r] $; mais par hypothèse, tout élément de $ a'_0 \cap B' $ peut s’écrire d’une seule manière comme polynôme par rapport aux $ x'_j (1 \leq j \leq r) $ à coefficients dans $ k $, et dont chaque monôme contient au moins un des $ x'_j $ pour $ 1 \leq j \leq h(0) $; on aboutit donc à une contradiction, ce qui prouve notre assertion.

Nous supposerons donc dans toute la suite de la démonstration que $ A = k[Y_1, \ldots, Y_m] $, et nous raisonnons par récurrence sur $ p $.

A) $ p = 1 $. Distinguons deux cas :
A 1) L’idéal $ a_1 $ est un idéal principal engendré par un élément $ x_1 \in k $.

On a $ x_1 = P(Y_1, \ldots, Y_m) $, où $ P $ est un polynôme non constant. Nous allons voir que, pour un choix convenable d’entiers $ r_i > 0 $, l’anneau $ \mathbf{A} $ est *entier sur* $ \mathbf{B} = k[x_1, x_2, \ldots, x_m] $, avec
(1)
$$
x_i = Y_i - Y_1^{r_i} \quad (2 \leq i \leq m).
$$
Il suffit pour cela de choisir les $ r_i $ de sorte que $ Y_1 $ soit *entier sur* $ \mathbf{B} $ (\S 1, n° 1, prop. 4). Or, on a la relation
(2)
$$
P(Y_1, x_2 + Y_1^{r_2}, \ldots, x_m + Y_1^{r_m}) - x_1 = 0
$$
Soit $ P = \sum_p a_p Y^p $ où $ p = (p_1, \ldots, p_m) $, les $ p_i $ étant des entiers $ \geq 0 $, $ Y^p = Y_1^{p_1} \cdots Y_m^{p_m} $, les $ a_p $ des éléments $ \neq 0 $ de $ k $, et un des indices $ p $ au moins étant distinct de $ (0, \ldots, 0) $; la relation (2) s’écrit
(3)
$$
\sum_p a_p Y_1^{p_1}(x_2 + Y_1^{r_2})^{p_2} \cdots (x_m + Y_1^{r_m})^{p_m} - x_1 = 0.
$$
Posons $ f(p) = p_1 + r_2 p_2 + \cdots + r_m p_m $, et supposons les $ r_i $ choisis de sorte que tous les $ f(p) $ soient distincts (il suffit par exemple de prendre $ r_i = h^i $, où $ h $ est un entier strictement supérieur à tous les $ p_j $ (*Ens.*, chap. III, § 5, n° 7, prop. 8)). Il y aura alors un système $ p = (p_1, \ldots, p_m) $ et un seul tel que $ f(p) $ soit maximum, et la relation (3) s’écrit
(4)
$$
a_p Y_1^{f(p)} + \sum_{j < f(p)} Q_j(x_1, \ldots, x_m) Y_1^j = 0
$$
où les $ Q_j $ sont des polynômes de $ k[Y_1, \ldots, Y_m] $; comme $ a_p \neq 0 $ est inversible dans $ k $, (4) est bien une équation de dépendance intégrale à coefficients dans $ \mathbf{B} $, d’où notre assertion.

Le corps des fractions $ k(Y_1, \ldots, Y_m) $ de $ \mathbf{A} $ est donc algébrique sur le corps des fractions $ k(x_1, \ldots, x_m) $ de $ \mathbf{B} $, ce qui prouve (*Alg.*, chap. V, § 5, n° 3, th. 4) que les $ x_i $ ($ 1 \leq i \leq m $) sont algébriquement indépendants. De plus, on a $ a_1 \cap \mathbf{B} = B x_1 $; en effet, tout élément $ z \in a_1 \cap \mathbf{B} $ s’écrit $ z = x_1 z' $ avec $ z' \in \mathbf{A} \cap k(x_1, \ldots, x_m) $; mais on a $ \mathbf{A} \cap k(x_1, \ldots, x_m) = k[x_1, \ldots, x_m] = \mathbf{B} $ puisque $ \mathbf{B} $ est intégralement clos (\S 1, n° 3, cor. 2 de la prop. 13); on a par suite $ z' \in \mathbf{B} $, ce qui achève de démontrer les propriétés *a)* et *b)* dans ce cas.

A 2) *Cas général* ($ p = 1 $).

On raisonne par récurrence sur $ m $, le cas $ m = 0 $ étant trivial. On peut évidemment supposer $ a_1 \neq 0 $ (sans quoi on peut prendre $ x_i = Y_i $ pour $ 1 \leq i \leq m $ et $ h(1) = 0 $). Soit $ x_1 $ un élément non nul de $ a_1 $; en vertu de A 1), il existe $ t_2, \ldots, t_m $ tels que $ x_1, t_2, \ldots, t_m $ soient algébriquement indépendants sur $ k $, que $ A $ soit entier sur $ C = k[x_1, t_2, \ldots, t_m] $ et que $ x_1 A \cap C = x_1 C $. En vertu de l’hypothèse de récurrence, il existe des éléments $ x_2, \ldots, x_m $ de $ k[t_2, \ldots, t_m] $ et un entier $ h $ tels que $ k[t_2, \ldots, t_m] $ soit entier sur $ B' = k[x_2, \ldots, x_m] $, que $ x_2, \ldots, x_m $ soient algébriquement indépendants sur $ k $ et que l’idéal $ a_1 \cap B' $ soit engendré par $ x_2, \ldots, x_h $. Alors $ C $ est entier sur $ B = k[x_1, x_2, \ldots, x_m] $ ($ \S 1 $, no 1, cor. de la prop. 5), donc il en est de même de $ A $ ($ \S 1 $, no 1, prop. 6); le même raisonnement que dans le cas A 1) montre que $ x_1, \ldots, x_m $ sont algébriquement indépendants sur $ k $; enfin, comme $ x_1 \in a_1 $ et $ B = B'[x_1] $, on a $ a_1 \cap B = Bx_1 + (a_1 \cap B') $, et comme $ a_1 \cap B' $ est engendré (dans $ B' $) par $ x_2, \ldots, x_h $, $ a_1 \cap B $ est engendré (dans $ B $) par $ x_1, x_2, \ldots, x_h $.

B) Passage de $ p - 1 $ à $ p $.

Soient $ t_1, \ldots, t_m $ des éléments de $ A $ satisfaisant aux conditions du théorème pour la suite croissante d’idéaux $ a_1 \subset \cdots \subset a_{p-1} $, et posons $ r = h(p - 1) $. En vertu de A 2), il existe des éléments $ x_{r+1}, \ldots, x_m $ de $ k[t_{r+1}, \ldots, t_m] $ et un entier $ s $ tels que

$$
C = k[t_{r+1}, \ldots, t_m]
$$

soit entier sur $ B' = k[x_{r+1}, \ldots, x_m] $, que $ x_{r+1}, \ldots, x_m $ soient algébriquement indépendants sur $ k $ et que l’idéal $ a_p \cap B' $ soit engendré par $ x_{r+1}, \ldots, x_s $. En posant $ x_i = t_i $ pour $ i \leq r $, la famille $ (x_i)_{1 \leq i \leq m} $ obtenue répond à la question avec $ h(p) = s $. En effet, $ A $ est entier sur $ C[t_1, \ldots, t_r] = C[x_1, \ldots, x_r] $, donc aussi sur $ B = k[x_1, \ldots, x_m] = B'[x_1, \ldots, x_r] $, puisque $ C $ est entier sur $ B' $ ($ \S 1 $, no 1, cor. de la prop. 5 et prop. 6); on montre comme dans le cas A 1) que les $ x_i $ sont algébriquement indépendants sur $ k $. D’autre part, pour $ j \leq p - 1 $, l’idéal

$$
a_j \cap k[x_1, \ldots, x_r, t_{r+1}, \ldots, t_m]
$$

est par hypothèse l’ensemble des polynômes en $ x_1, \ldots, x_r, t_{r+1}, \ldots, t_m $ dont tous les monômes contiennent un des éléments $ x_1, \ldots, x_{h(j)} $ comme $ x_{r+1}, \ldots, x_m $ sont des polynômes en $ t_{r+1}, \ldots, t_m $ à coefficients dans $ k $, on voit aussitôt qu’un polynôme en $ x_1, \ldots, x_r, x_{r+1}, \ldots, x_m $ (à coefficients dans $ k $) ne peut appartenir à $ a_j $ que si tous ses monômes contiennent un des éléments $ x_1, \ldots, x_{h(j)} $. Enfin, comme $ x_1, \ldots, x_r $ appartiennent à $ a_{p-1} $, donc aussi à $ a_p $, $ a_p \cap B'[x_1, \ldots, x_r] $ est formé des polynômes en $ x_1, \ldots, x_r $ à coefficients dans $ B' $, dont le terme constant appartient à $ a_p \cap B' $; par suite cet idéal est engendré par $ x_1, \ldots, x_r, x_{r+1}, \ldots, x_t $.

C.Q.F.D.

Posons $ S = A - \{0\} $, et soit $ k = S^{-1}A $ le corps des fractions de $ A $; il est clair que $ S^{-1}B $ est une $ k $-algèbre de type fini, et comme elle contient par hypothèse $ k $ (chap. II, § 2, no 4, th. 1) elle n’est pas réduite à 0. En vertu du th. 1 (appliqué pour $ p = 1 $ et $ a_1 = 0 $) il existe donc une suite finie $ (x_i)_{1 \leq i \leq n} $ d’éléments de $ S^{-1}B $ algébriquement indépendants sur $ k $ et tels que $ S^{-1}B $ soit entier sur $ k[x_1, \ldots, x_n] $. Soit $ (z_j)_{1 \leq j \leq m} $ un système de générateurs de la $ A $-algèbre $ B $; dans $ S^{-1}B $, chacun des $ z_j/1 $ vérifie une équation de dépendance intégrale

$$
(z_j/1)^{q_j} + \sum_{h < q_j} P_{hj}(x_1, \ldots, x_n)(z_j/1)^h = 0
$$

où les $ P_{hj} $ sont des polynômes en les $ x_i $ à coefficients dans $ k $. Il existe un élément $ s \neq 0 $ de $ A $ tel que l’on puisse écrire $ x_i = y_i/s $ avec $ y_i \in B $ pour $ 1 \leq i \leq n $, et que tous les coefficients des $ P_{hj} $ soient de la forme $ c/s $ avec $ c \in A $; enfin, remplaçant au besoin $ s $ par un produit d’éléments de $ S $, on peut supposer que l’on ait, dans $ B $

$$
sz_j^{q_j} + \sum_{h < q_j} Q_{hj}z_j^h = 0
$$

où les $ Q_{hj} $ sont des polynômes en $ y_1, \ldots, y_n $, à coefficients dans $ A $; si on pose $ z'_j = sz_j $, on voit, en multipliant (6) par $ s^{q_j-1} $, que $ z'_j $ est entier sur $ B' = A[y_1, \ldots, y_n] $. Montrons que les $ y_i $ sont algébriquement indépendants sur $ A $; en effet, si on a une relation de la forme $ \sum_p a_p y_1^{p_1} \ldots y_n^{p_n} = 0 $ avec $ a_p \in A $ pour tout $ p $, on en déduit $ \sum_p a'_p x_1^{p_1} \ldots x_n^{p_n} = 0 $ dans $ S^{-1}B $, avec $ a'_p = a_p s^{p_1+\cdots+p_n} $ dans $ k $; par hypothèse, on a donc $ a'_p = 0 $ pour tout $ p $, d’où $ a_p = 0 $ pour tout $ p $. En outre, dans l’anneau $ B[s^{-1}] $, chacun des $ z'_j/1 $ est entier sur $ B'[s^{-1}] $ ($ § 1 $, no 1, prop. 2), et comme $ z_j/1 = (z'_j/1)(1/s) $ dans $ B[s^{-1}] $, on voit que les $ z_j/1 $ sont entiers sur $ B'[s^{-1}] $, ce qui achève la démonstration ($ § 1 $, no 1, prop. 4).

COROLLAIRE 2. — Soient $ K $ un corps, $ A $ un sous-anneau de $ K $ et $ L $ le corps des fractions de $ A $. Si $ K $ est une $ A $-algèbre de type fini, $ [K : L] $ est fini et il existe $ a \neq 0 $ dans $ A $ tel que $ L = A[a^{-1}] $.

En effet, il résulte du cor. 1 qu’il existe des éléments $ x_1, \ldots, x_n $ de $ K $ et un élément $ a \neq 0 $ de $ A $ tels que $ x_1, \ldots, x_n $ soient algébriquement indépendants sur $ A $ (et par suite sur $ L $) et que $ K $ soit entier sur le sous-anneau $ A[x_1, \ldots, x_n, a^{-1}] $. Il résulte donc du § 2, no 1, lemme 2 que $ A[x_1, \ldots, x_n, a^{-1}] $ est un corps. Mais les seuls éléments inversibles d’un anneau de polynômes $ C[Y_1, \ldots, Y_n] $ sur un anneau intègre $ C $ sont les éléments inversibles de $ C $; appliquant cette remarque à $ C = A[a^{-1}] $, on voit qu’on a nécessairement $ n = 0 $ et que $ A[a^{-1}] $ est un corps, égal à $ L $ par définition de ce dernier. Comme $ K $ est entier sur $ L $ et est une $ L $-algèbre de type fini, le degré $ [K : L] $ est fini ($ § 1 $, no 1, prop. 4).

COROLLAIRE 3. — Soient $ A $ un anneau intègre, $ B $ une $ A $-algèbre de type fini, $ b $ un élément de $ B $ tel que $ zb^n \neq 0 $ pour tout $ z \neq 0 $ dans $ A $ et tout entier $ n > 0 $. Soit $ \rho : A \to B $ l’homomorphisme canonique; il existe $ a \neq 0 $ dans $ A $ tel que, pour tout homomorphisme $ f $ de $ A $ dans un corps algébriquement clos $ L $, tel que $ f(a) \neq 0 $, il existe un homomorphisme $ g $ de $ B $ dans $ L $ tel que $ g(b) \neq 0 $ et que $ f = g \circ \rho $.

L’hypothèse faite sur $ b $ entraîne que si $ h $ est l’homomorphisme canonique $ x \to x/1 $ de $ B $ dans $ B[b^{-1}] $, l’homomorphisme $ h \circ \rho $ de $ A $ dans $ B[b^{-1}] $ est injectif. En vertu du cor. 1, il existe donc un élément $ a \neq 0 $ de $ A $ et un sous-anneau $ B' $ de $ B[b^{-1}] $ tel que $ B[b^{-1}, a^{-1}] $ soit entier sur $ B'[a^{-1}] $ et que $ B' $ soit isomorphe à une algèbre de polynômes $ A[Y_1, \ldots, Y_n] $. Soit $ f $ un homomorphisme de $ A $ dans un corps algébriquement clos $ L $, tel que $ f(a) \neq 0 $; il existe un homomorphisme de $ A[Y_1, \ldots, Y_n] $ dans $ L $ prolongeant $ f $, donc il existe un homomorphisme $ f' $ de $ B' $ dans $ L $ prolongeant $ f $. Comme $ f'(a) \neq 0 $ dans $ L $, il existe un homomorphisme $ f'' $ de $ B'[a^{-1}] $ dans $ L $ tel que

$$
f''(x/a^n) = f'(x).(f(a))^{-n}
$$

pour tout $ x \in B' $ et tout $ n > 0 $ (chap. II, § 2, no 1, prop. 1). Enfin, comme $ B[b^{-1}, a^{-1}] $ est entier sur $ B'[a^{-1}] $, il existe un homomorphisme $ f''' $ de $ B[b^{-1}, a^{-1}] $ dans $ L $ prolongeant $ f'' $ (§ 2, no 1, cor. 4 du th. 1). Si $ j : x \to x/1 $ est l’homomorphisme canonique de $ B $ dans $ B[b^{-1}, a^{-1}] $, $ g = f''' \circ j $ répond à la question car $ j(b) $ est inversible dans $ B[b^{-1}, a^{-1}] $, donc $ f'''(j(b)) \neq 0 $, dans $ L $.

On notera que si on suppose $ B $ intègre et $ A \subset B $ dans le cor. 3, l’hypothèse faite sur $ b $ équivaut à $ b \neq 0 $.

### 2. Fermeture intégrale d’une algèbre de type fini sur un corps

#### Théorème 2 {#ac-v-s3-thm-2 .statement}

Soient $ A $ une $ k $-algèbre intègre de type fini, $ K $ son corps des fractions, $ A' $ la fermeture intégrale de $ A $ dans un corps $ K' $, extension algébrique de degré fini de $ K $. Alors $ A' $ est un $ A $-module de type fini et une $ k $-algèbre de type fini.

En vertu du th. 1, il existe une sous-algèbre $ C $ de $ A $ isomorphe à une algèbre de polynômes $ k[X_1, \ldots, X_n] $, et telle que $ A $ soit entière sur $ C $; $ A' $ est évidemment la fermeture intégrale de $ C $ dans $ K' $ (\$ 1, no 1, prop. 6); on peut donc se borner au cas où $ A = k[X_1, \ldots, X_n] $. Soit $ N $ l’extension quasi-galoisienne de $ K' $ (dans une clôture algébrique de $ K' $) engendrée par $ K' $, qui est une extension algébrique de degré fini de $ K $ (Alg., chap. V, § 6, no 3, cor. 1 de la prop. 9). Il suffira de prouver que la fermeture intégrale $ B $ de $ A $ dans $ N $ est un $ A $-module de type fini, car $ A' $ est un sous-$ A $-module de $ B $ et $ A $ est un anneau noethérien (chap. III, § 2, no 10, cor. 2 du th. 2). On peut donc se borner au cas où $ K' $ est une extension quasi-galoisienne de $ K $. On sait alors (Alg., chap. V, § 10, no 9, prop. 14) que $ K' $ est une extension galoisienne (de degré fini) d’une extension radicielle $ K'' $ (de degré fini) de $ K $. Si $ A'' $ est la fermeture intégrale de $ A $ dans $ K'' $, $ A' $ est la fermeture intégrale de $ A'' $ dans $ K' $, et il suffira de prouver que $ A'' $ est un $ A $-module de type fini et $ A' $ un $ A'' $-module de type fini. Or, si l’on a prouvé que $ A'' $ est un $ A $-module de type fini, c’est un anneau noethérien, intégralement clos par définition; le fait que $ A' $ est un $ A'' $-module de type fini résultera du § 1, no 6, cor. 1 de la prop. 18.

On voit donc qu’on peut se borner au cas où $ A = k[X_1, \ldots, X_n] $ et où $ K' $ est une extension radicielle de degré fini de $ K = k(X_1, \ldots, X_n) $. Alors $ K' $ est engendré par une famille finie d’éléments $ (y_i)_{1 \leq i \leq m} $, et il existe une puissance $ q $ de l’exposant caractéristique de $ k $ telle que l’on ait $ y_i^q \in k(X_1, \ldots, X_n) $. Soient $ c_j $ ($ 1 \leq j \leq r $) les coefficients des numérateurs et dénominateurs des fractions rationnelles en $ X_1, \ldots, X_n $ égales aux $ y_i^q $ ($ 1 \leq i \leq m $). Alors $ K' $ est contenu dans l’extension $ L = k'(X_1^{q^{-1}}, \ldots X_n^{q^{-1}}) $, où $ k' = k(c_1^{q^{-1}}, \ldots c_r^{q^{-1}}) $, (on se place dans une clôture algébrique de $ K' $), et $ A' $ est contenu dans la fermeture algébrique $ B' $ de $ A $ dans $ L' $. Or, $ k' $ est algébrique sur $ k $, donc $ C' = k'[X_1, \ldots, X_n] $ est entier sur $ A $ ($ \S 1 $, no 1, prop. 5); comme $ k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}] $ est intégralement clos ($ \S 1 $, no 3, cor. 2 de la prop. 13), on voit que cet anneau est la fermeture intégrale de $ C' $ dans $ L' $, donc aussi celle de $ A $ ($ \S 1 $, no 1, prop. 6), autrement dit $ B' = k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}] $. Or il est clair que $ B' $ est un $ C' $-module de type fini ($ \S 1 $, no 1, prop. 4), et comme $ k' $ est une extension de degré fini de $ k $, $ C' $ est un $ A $-module de type fini, donc $ B' $ est un $ A $-module de type fini; puisque $ A $ est noethérien et $ A' \subset B' $, $ A' $ est un $ A $-module de type fini.

C.Q.F.D.

### 3. Le théorème des zéros

#### Proposition 1 {#ac-v-s3-prop-1 .statement}

Soient $ A $ une algèbre de type fini sur un corps $ k $ et $ L $ une clôture algébrique de $ k $.

(i) Si $ A \neq \{0\} $, il existe un $ k $-homomorphisme de $ A $ dans $ L $.

(ii) Soient $ f_1, f_2 $ deux $ k $-homomorphismes de $ A $ dans $ L $. Pour que $ f_1 $ et $ f_2 $ aient même noyau, il faut et il suffit qu’il existe un $ k $-automorphisme $ s $ de $ L $ tel que $ f_2 = s \circ f_1 $.

(iii) Soit $ a $ un idéal de $ A $. Pour que $ a $ soit maximal, il faut et il suffit qu’il soit le noyau d’un $ k $-homomorphisme de $ A $ dans $ L $.

(iv) Pour qu’un élément $ x $ de $ A $ soit tel que $ f(x) = 0 $ pour tout $ k $-homomorphisme $ f $ de $ A $ dans $ L $, il faut et il suffit que $ x $ soit nilpotent.

L’assertion (i) résulte du no 1, cor. 3 du th. 1 appliqué en remplaçant $ A $ par $ k $, $ B $ par $ A $, $ b $ par l’élément unité de $ B $, $ f $ par l’injection canonique de $ k $ dans $ L $.

Si $ f $ est un $ k $-homomorphisme de $ A $ dans $ L $, $ f(A) $ est un sous-anneau de $ L $ contenant $ k $; comme $ L $ est une extension algébrique de $ k $, $ f(A) $ est un corps ($ Alg. $, chap. V, $ \S 3 $, no 2, prop. 3) et si $ a $ est le noyau de $ f $, $ A/a $, isomorphe à $ f(A) $, est donc un corps, ce qui prouve que $ a $ est maximal. Inversement, si $ a $ est un idéal maximal de $ A $, il résulte de (i) qu’il existe un $ k $-homomorphisme de $ A/a $ dans $ L $, donc un $ k $-homomorphisme de $ A $ dans $ L $, dont le noyau $ b $ contient $ a $; mais comme $ a $ est maximal, on a $ b = a $; ceci prouve (iii).

Démontrons (ii). Si $ s $ est un $ k $-automorphisme de $ L $ tel que $ f_2 = s \circ f_1 $, il est clair que $ f_1 $ et $ f_2 $ ont même noyau. Réciproquement, supposons que $ f_1 $ et $ f_2 $ aient même noyau; il existe

Enfin, si $ x \in A $ est tel que $ x^n = 0 $, pour tout $ k $-homomorphisme $ f $ de $ A $ dans $ L $, on a $ (f(x))^n = f(x^n) = 0 $, donc $ f(x) = 0 $ puisque $ L $ est un corps. Inversement, supposons que $ x \in A $ ne soit pas nilpotent; alors $ A[x^{-1}] $ est une $ A $-algèbre de type fini (donc une $ k $-algèbre de type fini) non réduite à 0 (chap. II, § 2, no 1, *Remarque 3*), donc il existe un $ k $-homomorphisme $ g $ de $ A[x^{-1}] $ dans $ L $ en vertu de (i). Si $ j : A \to A[x^{-1}] $ est l’homomorphisme canonique, $ f = g \circ j $ est un $ k $-homomorphisme de $ A $ dans $ L $, et on a $ f(x)g(1/x) = g(x/1)g(1/x) = g(1) = 1 $, d’où $ f(x) \neq 0 $.

C.Q.F.D.

Soient $ k $ un corps et $ L $ un surcorps de $ k $; on dit qu’un élément $ x = (x_1, \ldots, x_n) $ de $ L^n $ est zéro *dans* $ L^n $ *d’un idéal* $ r $ *de l’anneau de polynômes* $ k[X_1, \ldots, X_n] $ si l’on a
$$
P(x) = P(x_1, \ldots, x_n) = 0
$$
pour tout $ P \in r $.

#### Lemme 1 {#ac-v-s3-lem-1 .statement}

*Soient* $ A $ *une algèbre de type fini sur un corps* $ k $, $ (a_i)_{1 \leq i \leq n} $ *un système de générateurs de cette algèbre*, $ r $ *l’idéal des relations algébriques entre les* $ a_i $ *à coefficients dans* $ k $ (*Alg.*, chap. IV, § 2, no 1). *Pour tout surcorps* $ L $ *de* $ k $, *l’application* $ f \to (f(a_i))_{1 \leq i \leq n} $ *est une bijection de l’ensemble des* $ k $*-homomorphismes de* $ A $ *dans* $ L $ *sur l’ensemble des zéros de* $ r $ *dans* $ L^n $.

Il existe un homomorphisme $ h $ de $ k $-algèbres de $ k[X_1, \ldots, X_n] $ sur $ A $ et un seul tel que $ h(X_i) = a_i $ pour $ 1 \leq i \leq n $, et par définition $ r $ est le noyau de $ h $. L’application $ f \to f \circ h $ est une bijection de l’ensemble des $ k $-homomorphismes de $ A $ dans $ L $ sur l’ensemble des $ k $-homomorphismes de $ k[X_1, \ldots, X_n] $ dans $ L $, nuls dans $ r $. Pour tout polynôme $ P \in k[X_1, \ldots, X_n] $ et tout élément $ x = (x_1, \ldots, x_n) \in L^n $, posons $ h_x(P) = P(x) $; alors l’application $ x \to h_x $ est une bijection de $ L^n $ sur l’ensemble des $ k $-homomorphismes de $ k[X_1, \ldots, X_n] $ dans $ L $ (un tel homomorphisme étant déterminé par ses valeurs aux $ X_i (1 \leq i \leq n) $); dire que $ h_x $ est nul dans $ r $ signifie que $ x $ est un zéro de $ r $ dans $ L^n $, d’où le lemme.

Si on applique la prop. 1 à l’algèbre $ A = k[X_1, \ldots, X_n]/r $, où $ r $ est un idéal de $ k[X_1, \ldots, X_n] $ distinct de l’anneau tout entier, on obtient, en vertu du lemme 1, l’énoncé suivant:

PROPOSITION 2 (théorème des zéros de Hilbert). — Soient $ k $ un corps, $ L $ une clôture algébrique de $ k $.

(i) Tout idéal $ r $ de $ k[X_1, \ldots, X_n] $ ne contenant pas 1 admet au moins un zéro dans $ L^n $.

(ii) Soient $ x = (x_1, \ldots, x_n), y = (y_1, \ldots, y_n) $ deux éléments de $ L^n $; pour que l’ensemble des polynômes de $ k[X_1, \ldots, X_n] $ nuls en $ x $ soit identique à l’ensemble des polynômes de $ k[X_1, \ldots, X_n] $ nuls en $ y $, il faut et il suffit qu’il existe un $ k $-automorphisme $ s $ de $ L $ tel que $ y_i = s(x_i) $ pour $ 1 \leq i \leq n $.

(iii) Pour qu’un idéal $ a $ de $ k[X_1, \ldots, X_n] $ soit maximal, il faut et il suffit qu’il existe un $ x $ dans $ L^n $ tel que $ a $ soit l’ensemble des polynômes de $ k[X_1, \ldots, X_n] $ nuls en $ x $.

(iv) Pour qu’un polynôme $ Q $ de $ k[X_1, \ldots, X_n] $ soit nul dans l’ensemble des zéros dans $ L^n $ d’un idéal $ r $ de $ k[X_1, \ldots, X_n] $, il faut et il suffit qu’il existe un entier $ m > 0 $ tel que $ Q^m \in r $.

### 4. Anneaux de Jacobson

#### Définition 1 {#ac-v-s3-def-1 .statement}

On dit qu’un anneau $ A $ est un anneau de Jacobson si tout idéal premier de $ A $ est intersection d’une famille d’idéaux maximaux.

#### Exemple 1 {#ac-v-s3-n4-exa-1 .statement}

Tout corps est un anneau de Jacobson.

#### Exemple 2 {#ac-v-s3-n4-exa-2 .statement}

L’anneau $ \mathbf{Z} $ est un anneau de Jacobson, l’unique idéal premier non maximal (0) étant l’intersection des idéaux maximaux $ (p) $ de $ \mathbf{Z} $, où $ p $ parcourt l’ensemble des nombres premiers (cf. prop. 4).

#### Exemple 3 {#ac-v-s3-n4-exa-3 .statement}

Soit $ A $ un anneau de Jacobson et soit $ a $ un idéal de $ A $. Alors $ A/a $ est un anneau de Jacobson, car les idéaux de $ A/a $ sont de la forme $ b/a $, où $ b $ est un idéal de $ A $ contenant $ a $, et $ b/a $ est premier (resp. maximal) si et seulement si $ b $ l’est.

#### Proposition 3 {#ac-v-s3-prop-3 .statement}

Pour qu’un anneau $ A $ soit un anneau de Jacobson, il faut et il suffit que, pour tout idéal $ a $ de $ A $, le radical de $ A/a $ soit égal à son nilradical (chap. II, § 2, no 6).

Le radical (resp. nilradical) de $ A/a $ est l’intersection des idéaux maximaux (resp. premiers) de $ A/a $ ($ Alg. $, chap. VIII, § 6, no 3, déf. 3 et $ Alg. comm. $, chap. II, § 2, no 6, prop. 13). La condition énoncée signifie donc que pour tout idéal $ a $ de $ A $, l’intersection des idéaux premiers contenant $ a $ est égale à l’intersection des idéaux maximaux contenant $ a $. Cette condition est évidemment vérifiée pour tout idéal $ a $ de $ A $ si $ A $ est un anneau de Jacobson; réciproquement, si elle est vérifiée pour tout idéal premier de $ A $, $ A $ est un anneau de Jacobson par définition.

COROLLAIRE. — *Soit $ A $ un anneau de Jacobson; pour tout idéal $ a $ de $ A $, la racine de $ a $ est l’intersection des idéaux maximaux de $ A $ contenant $ a $.*

Il suffit de remarquer que $ A/a $ est un anneau de Jacobson.

PROPOSITION 4. — *Soient $ A $ un anneau principal, $ (p_\lambda)_{\lambda \in L} $ un système représentatif d’éléments extrémaux de $ A $ (Alg., chap. VII, § 1, no 3, déf. 2). Pour que $ A $ soit un anneau de Jacobson, il faut et il suffit que $ L $ soit infini.*

En effet, les idéaux maximaux de $ A $ sont les $ Ap_\lambda $ (*loc. cit.*, no 2, prop. 2). Si $ L $ est fini, leur intersection est l’idéal $ Ax $, où $ x = \prod_{\lambda \in L} p_\lambda $ (*ibid.*), donc est différente de $ (0) $; au contraire, si $ L $ est infini, l’intersection des $ Ap_\lambda $ est $ (0) $, tout élément $ \neq 0 $ de $ A $ n’étant divisible que par un nombre fini d’éléments extrémaux (*loc. cit.*, no 3, th. 2). La proposition résulte alors de ce que $ (0) $ est le seul idéal premier non maximal de $ A $ (Alg. chap. VI, § 1, no 13, prop. 14 (DIV)).

PROPOSITION 5. — *Soient $ A $ un anneau, $ B $ une $ A $-algèbre entière sur $ A $. Si $ A $ est un anneau de Jacobson, il en est de même de $ B $.*

Remplaçant $ A $ par son image canonique dans $ B $, on peut supposer que $ A \subset B $. Soit $ p' $ un idéal premier de $ B $, et soit $ p = A \cap p' $. Il existe par hypothèse une famille $ (m_\lambda)_{\lambda \in L} $ d’idéaux maximaux de $ A $ dont l’intersection est égale à $ p $. Pour tout $ \lambda \in L $, il existe un idéal maximal $ m'_\lambda $ de $ B $ au-dessus de $ m_\lambda $ et contenant $ p' $ ($ § 2 $, no 1, prop. 1 et cor. 2 du th. 1). Si l’on pose $ q' = \bigcap_{\lambda \in L} m'_\lambda $, on a donc $ q' \cap A = \bigcap_{\lambda \in L} m_\lambda = p $, et $ q' \supset p' $, d’où $ q' = p' $ ($ § 2 $, no 1, cor. 1 de la prop. 1).

THÉORÈME 3. — *Soient $ A $ un anneau de Jacobson, $ B $ une $ A $-algèbre de type fini, $ \rho : A \to B $ l’homomorphisme canonique. Alors :

(i) $ B $ est un anneau de Jacobson.

(ii) *Pour tout idéal maximal $ m' $ de $ B $, $ m = \rho^{-1}(m') $ est un idéal maximal de $ A $ et $ B/m' $ est une extension algébrique de degré fini de $ A/m $.*

Soient $ \mathfrak{p}' $ un idéal premier de $ B $, $ \mathfrak{p} = \rho^{-1}(\mathfrak{p}') $. Soit $ \nu $ un élément $ \neq 0 $ de $ B/\mathfrak{p}' $. Comme $ B/\mathfrak{p}' $ est une $ (A/\mathfrak{p}) $-algèbre intègre de type fini et que l’homomorphisme canonique $ \varphi : A/\mathfrak{p} \to B/\mathfrak{p}' $ est injectif, il existe un élément $ u \neq 0 $ de $ A/\mathfrak{p} $ tel que pour tout homomorphisme $ f $ de $ A/\mathfrak{p} $ dans un corps algébriquement clos $ L $, dont le noyau ne contient pas $ u $, il existe un homomorphisme $ g $ de $ B/\mathfrak{p}' $ dans $ L $, dont le noyau ne contient pas $ \nu $, et pour lequel $ f = g \circ \varphi $ (no 1, cor. 3 du th. 1). Puisque $ A $ est un anneau de Jacobson, il existe un idéal maximal $ m $ de $ A $ contenant $ \mathfrak{p} $ et tel que $ u \notin m/\mathfrak{p} $. Prenons pour $ L $ une clôture algébrique de $ A/m $ et pour $ f $ l’homomorphisme canonique $ A/\mathfrak{p} \to L $; soit

$$
g : B/\mathfrak{p}' \to L
$$

un homomorphisme tel que $ f = g \circ \varphi $ et $ g(\nu) \neq 0 $. On a $ A/m \subset g(B/\mathfrak{p}') \subset L $, donc $ g(B/\mathfrak{p}') $ est un sous-corps de $ L $ ($ Alg. $, chap. V, § 3, no 2, prop. 3), et le noyau de $ g $ est par suite un idéal maximal de $ B/\mathfrak{p}' $ ne contenant pas $ \nu $. On voit ainsi que l’intersection des idéaux maximaux de $ B/\mathfrak{p}' $ est réduite à 0, ce qui prouve que $ B $ est un anneau de Jacobson. En outre, si $ \mathfrak{p}' $ est maximal, $ g $ est nécessairement injectif, donc $ \mathfrak{p} = m $ est maximal; enfin $ B/\mathfrak{p}' $ est alors une algèbre de type fini sur le corps $ A/m $, donc est une extension de degré fini de $ A/m $ (no 1, cor. 2 du th. 1).

#### Corollaire 1 {#ac-v-s3-prop-3-cor-1 .statement}

*Toute algèbre $ A $ de type fini sur $ \mathbf{Z} $ est un anneau de Jacobson; pour qu’un idéal premier $ \mathfrak{p} $ de $ A $ soit maximal, il faut et il suffit que l’anneau $ A/\mathfrak{p} $ soit fini.*

Si l’anneau intègre $ A/\mathfrak{p} $ est fini, c’est un corps, car pour tout $ u \neq 0 $ dans $ A/\mathfrak{p} $, l’application $ \nu \to u\nu $ de $ A/\mathfrak{p} $ dans lui-même est injective, donc bijective puisque $ A/\mathfrak{p} $ est fini. Inversement, pour tout idéal maximal $ m $ de $ A $, l’image réciproque de $ m $ dans $ \mathbf{Z} $ est un idéal maximal ($ p $) et $ A/m $ est de degré fini sur le corps premier $ \mathbf{Z}/(p) = \mathbf{F}_p $, en vertu du th. 3.

#### Corollaire 2 {#ac-v-s3-prop-3-cor-2 .statement}

*Soit $ (P_\lambda)_{\lambda \in L} $ une famille de polynômes de $ \mathbf{Z}[X_1, \ldots, X_n] $, et soit $ Q $ un polynôme de $ \mathbf{Z}[X_1, \ldots, X_n] $ tel que pour tout système d’éléments $ (x_i)_{1 \leq i \leq n} $ appartenant à un corps fini et pour lequel $ P_\lambda(x_1, \ldots, x_n) = 0 $ pour tout $ \lambda $, on ait aussi $ Q(x_1, \ldots, x_n) = 0 $. Alors, si $ a $ est l’idéal de $ \mathbf{Z}[X_1, \ldots, X_n] $ engendré par les $ P_\lambda $, il existe un entier $ m > 0 $ tel que $ Q^m \in a $. En outre, pour tout anneau réduit $ R $ et tout système $ (y_i)_{1 \leq i \leq n} $ d’éléments de $ R $ tel que $ P_\lambda(y_1, \ldots, y_n) = 0 $ pour tout $ \lambda $, on a aussi $ Q(y_1, \ldots, y_n) = 0 $.*

La seconde assertion découle de la première puisque l’idéal de $ \mathbf{Z}[X_1, \ldots, X_n] $ formé des polynômes $ P $ tels que $ P(y_1, \ldots, y_n) = 0 $ contient $ a $. Pour démontrer la première assertion, il suffit de remarquer que pour tout idéal maximal $ m $ de $ A = \mathbf{Z}[X_1, \ldots, X_n] $ contenant $ a $, $ A/m $ est un corps fini (cor. 1), et l’hypothèse entraîne que l’image canonique de $ Q $ dans $ A/m $ est nulle; donc $ Q $ appartient à l’intersection des idéaux maximaux de $ A $ contenant $ a $, qui est la racine de $ a $ (cor. de la prop. 3).

COROLLAIRE 3. — Soit $ A $ un anneau de Jacobson. S’il existe une $ A $-algèbre de type fini $ B $ contenant $ A $, et qui soit un corps, alors $ A $ est un corps et $ B $ est une extension algébrique de $ A $.
En effet, il suffit d’appliquer le th. 3, (ii) avec $ m' = (0) $.

## EXERCICES {#ac-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
