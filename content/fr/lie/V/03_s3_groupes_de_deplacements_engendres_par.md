---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 3
section_title: Groupes de déplacements engendrés par des réflexions
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0071-0088, 0127-0128
extraction: ocr
subsections:
    - "no": 1
      title: Résultats préliminaires
      page: 0
      pdf_page: 71
    - "no": 2
      title: Relation avec les systèmes de Coxeter
      page: 0
      pdf_page: 73
    - "no": 3
      title: Domaine fondamental, stabilisateurs
      page: 0
      pdf_page: 74
    - "no": 4
      title: Matrice et graphe de Coxeter de W
      page: 0
      pdf_page: 75
    - "no": 5
      title: Systèmes de vecteurs à produits scalaires négatifs
      page: 0
      pdf_page: 76
    - "no": 6
      title: Théorèmes de finitude
      page: 0
      pdf_page: 78
    - "no": 7
      title: Décomposition de la représentation linéaire de $ W $ dans $ T $
      page: 0
      pdf_page: 80
    - "no": 8
      title: Décomposition de l’espace affine E en produit
      page: 0
      pdf_page: 82
    - "no": 9
      title: Structure des chambres
      page: 0
      pdf_page: 84
    - "no": 10
      title: Points spéciaux
      page: 0
      pdf_page: 86
statements: 35
exercises: 8
content_sha256: 3d39fd02a70c3420f7b3cb7606b49e05f7564cf554da41d836ed8b673b3f3e84
---

## § 3. Groupes de déplacements engendrés par des réflexions

Dans ce paragraphe, on désigne par $ E $ un espace affine *réel* de dimension finie $ d $, par $ T $ l’espace des translations de $ E $. On suppose $ T $ muni d’un produit scalaire (c’est-à-dire une forme bilinéaire symétrique positive *non dégénérée*) noté $ (t|t') $. Pour $ t \in T $, on pose $ ||t|| = (t|t)^{1/2} $. La fonction $ d(x, y) = ||x - y|| $ est une distance sur $ E $, qui définit la topologie de $ E $ (§ 1).

On désigne par $ \mathfrak{S} $ un ensemble d’hyperplans de $ E $ et par $ W $ le groupe de déplacements de l’espace euclidien $ E $ engendré par les réflexions orthogonales $ s_H $ par rapport aux hyperplans $ H \in \mathfrak{S} $ (§ 2, no 4). On suppose que les conditions suivantes sont satisfaites :

(D 1) *Pour tout* $ w \in W $ *et tout* $ H \in \mathfrak{S} $, *l’hyperplan* $ w(H) $ *appartient à* $ \mathfrak{S} $;
(D 2) *Le groupe* $ W $ *muni de la topologie discrète opère proprement dans* $ E $.

Comme $ E $ est localement compact, il résulte de la *Remarque* du § 4, no 5 de *Top. gén.*, chap. III, 3e éd., que la condition (D 2) équivaut à la condition suivante :

(D' 2) *Quelles que soient les parties compactes* $ K $ *et* $ L $ *de* $ E $, *l’ensemble des* $ w \in W $ *tels que* $ w(K) $ *rencontre* $ L $ *est fini*.

### 1. Résultats préliminaires

#### Lemme 1 {#lie-v-s3-lem-1 .statement}

*L’ensemble d’hyperplans* $ \mathfrak{S} $ *est localement fini*.

Soit en effet $ K $ une partie compacte de $ E $. Si un hyperplan $ H \in \mathfrak{S} $ rencontre $ K $, l’ensemble $ s_H(K) $ rencontre aussi $ K $, puisque tout point de $ K \cap H $ est fixe par $ s_H $. L’ensemble des $ H \in \mathfrak{S} $ rencontrant $ K $ est donc fini d’après (D' 2).

#### Lemme 2 {#lie-v-s3-lem-2 .statement}

*Soit C une chambre.*

(i) *Pour tout $ x \in E $, il existe un élément $ w \in W $ tel que $ w(x) \in \overline{C} $.*
(ii) *Pour toute chambre $ C' $, il existe un élément $ w \in W $ tel que $ w(C') = C $.*
(iii) *Le groupe W est engendré par l’ensemble des réflexions orthogonales par rapport aux murs de C.*

Soit $ \mathfrak{M} $ l’ensemble des murs de C et soit $ W_{\mathfrak{M}} $ le sous-groupe de W engendré par les réflexions par rapport aux murs de C. Démontrons (i) : soit $ x \in E $ et soit J l’orbite de $ x $ par rapport au groupe $ W_{\mathfrak{M}} $. Il suffit de prouver que J rencontre $ \overline{C} $.

Soit $ a $ un point de C ; il existe une boule fermée B de centre $ a $ rencontrant J ; comme B est compacte, la propriété (D’ 2) du n° 1 montre que $ B \cap J $ est fini. Il existe donc un point $ y $ de J tel que

(1)
$$
d(a, y) \leq d(a, y') \quad \text{pour tout } y' \text{ dans } J.
$$

On va prouver que l’on a $ y \in \overline{C} $. Pour cela, il suffit de montrer que si H est un mur de C, on a $ y \in \overline{D_H(C)} $ (cf. § 1, n° 4, prop. 9). Comme on a $ s_H \in W_{\mathfrak{M}} $, on a $ s_H(y) \in J $ d’où (fig. 1)

(2)
$$
d(a, y)^2 \leq d(a, s_H(y))^2
$$
d’après (1). Il existe $ b \in H $ et deux vecteurs $ t $ et $ u $ tels que $ a = b + t $ et $ y = b + u $, le vecteur $ u $ étant orthogonal à H ; on a alors $ s_H(y) = b - u $, et (2) équivaut à $ (t - u|t - u) \leq (t + u|t + u) $, c’est-à-dire à $ (t|u) \geq 0 $. Cette inégalité entraîne $ y \in \overline{D_H(C)} $.

![Figure 1](https://i.imgur.com/3Q5z5QG.png)

Figure 1

(ii) Soient $ C' $ une chambre et $ a' \in C' $. D’après ce qu’on vient de démontrer, il existe $ w \in W_{\mathfrak{M}} $ tel que $ w^{-1}(a') \in \overline{C} $; par suite, la chambre $ C' $ rencontre $ w(C) $; comme $ w(C) $ est réunion de $ w(C) $ et de facettes d’intérieur vide (§ 1, n° 2, prop. 3), on a $ C' = w(C) $.

(iii) On a à prouver $ W = W_{\mathfrak{M}} $ et il suffit de prouver que l’on a $ s_{H'} \in W_{\mathfrak{M}} $ pour tout $ H' \in \mathfrak{S} $. Or $ H' $ est le mur d’au moins une chambre $ C' $ (§ 1, n° 4, prop. 8); on a vu qu’il existe $ w \in W_{\mathfrak{M}} $ tel que $ C' = w(C) $; par suite, il existe un mur H de C tel que $ H' = w(H) $, d’où $ s_{H'} = w.s_H.w^{-1} \in W_{\mathfrak{M}} $.

### 2. Relation avec les systèmes de Coxeter

#### Théorème 1 {#lie-v-s3-thm-1 .statement}

Soient C une chambre et S l’ensemble des réflexions par rapport aux murs de C.

(i) Le couple (W, S) est un système de Coxeter.
(ii) Soient w ∈ W et H un mur de C. La relation l(s_H w) > l(w) signifie que les chambres C et w(C) sont du même côté de H.
(iii) Pour toute chambre C', il existe un unique élément w ∈ W tel que w(C) = C'.
(iv) L’ensemble des hyperplans H tels que s_H ∈ W est égal à 𝔥.

Tout élément de S est d’ordre 2 et le lemme 2 montre que S engendre W. Pour tout mur H de C, notons P_H l’ensemble des w ∈ W tels que les chambres C et w(C) (qui ne rencontrent pas H) soient du même côté de H. Nous allons vérifier les conditions (A'), (B') et (C) du chap. IV, § 1, no 7.

(A') 1 ∈ P_H : Trivial.
(B') P_H est disjoint de s_H . P_H : En effet, w(C) et s_H w(C) sont de part et d’autre de H, donc si w(C) est du même côté de H que C, il n’en est pas de même de s_H w(C).
(C) Soient w ∈ P_H et H' un mur de C tel que ws_{H'} ∉ P_H ; on a ws_{H'} = s_H w :
Par hypothèse w(C) est du même côté de H que C, et ws_{H'}(C) est de l’autre côté de H. Donc ws_{H'}(C) et w(C) sont de part et d’autre de H ; les chambres s_{H'}(C) et C sont de part et d’autre de l’hyperplan w^{-1}(H). Soit a un point de la face de C de support H'. Le point a = s_{H'}(a) est adhérent aux deux chambres C et s_{H'}(C) qui sont respectivement contenues dans les deux demi-espaces ouverts limités par w^{-1}(H) ; on a donc a ∈ w^{-1}(H), d’où H' = w^{-1}(H). De là, on tire s_{H'} = w^{-1} s_H w, d’où ws_{H'} = s_H w.

Ceci étant, les assertions (i) et (ii) résultent de la prop. 6 du chap. IV, § 1, no 7. On a de plus (loc. cit., condition (A))

$$
\bigcap_{H \in \mathcal{M}} P_H = \{1\}.
$$

Le lemme 2 montre que W est transitif sur l’ensemble des chambres. De plus, si w ∈ W est tel que w(C) = C, on a w ∈ P_H pour tout mur H de C, d’où w = 1 par (3). Ceci établit (iii).

Soit enfin H un hyperplan tel que s_H ∈ W. Si l’on avait H ∉ 𝔥, il existerait au moins une chambre C' rencontrant H (§ 1, no 3, prop. 7). Tout point de H ∩ C' est invariant par s_H, donc appartient aux chambres C' et s_H(C') ; on a donc C' = s_H(C') ce qui contredit (iii) puisque s_H ≠ 1.

#### Corollaire {#lie-v-s3-n2-cor-1 .statement}

Soit Σ un ensemble de réflexions engendrant W. Toute réflexion appartenant à W est conjuguée à un élément de Σ.

Soit 𝔥' l’ensemble des hyperplans de la forme w(H) avec w ∈ W et H ∈ 𝔥 tel que s_H ∈ Σ. Comme W est engendré par la famille (s_H)_{H \in 𝔥'} et que 𝔥' est stable par W, on peut appliquer à 𝔥' au lieu de 𝔥 tous les résultats de ce no ; mais le th. 1, (iv) montre que toute réflexion de W est de la forme s_H avec H ∈ 𝔥', d’où le corollaire.

### 3. Domaine fondamental, stabilisateurs

Rappelons (Intégr., chap. VII, § 2, n° 10, déf. 2) qu’une partie D de E est appelée un domaine fondamental pour le groupe W si toute orbite de W dans E rencontre D en un point et un seul. Ceci équivaut à la conjonction des deux conditions :

a) Pour tout $ x \in E $, il existe $ w \in W $ tel que $ w(x) \in D $.

b) Étant donnés $ x, y \in D $ et $ w \in W $ tels que $ y = w(x) $, on a $ y = x $ (mais on peut avoir $ w \neq 1 $).

Nous allons démontrer les trois énoncés suivants :

#### Théorème 2 {#lie-v-s3-thm-2 .statement}

Pour toute chambre C, l’adhérence $ \overline{C} $ de C est un domaine fondamental pour W opérant dans E.

#### Proposition 1 {#lie-v-s3-prop-1 .statement}

Soient F une facette et C une chambre telles que $ F \subset \overline{C} $. Soit $ w \in W $. Les conditions suivantes sont équivalentes :

(i) $ w(F) $ rencontre F;
(ii) $ w(F) = F $;
(iii) $ w(\overline{F}) = \overline{F} $;
(iv) $ w $ laisse fixe au moins un point de F;
(v) $ w $ laisse fixe tout point de F;
(vi) $ w $ laisse fixe tout point de $ \overline{F} $;
(vii) $ w $ appartient au sous-groupe de W engendré par les réflexions par rapport aux murs de C contenant F.

Pour toute partie A de E, notons W(A) le sous-groupe de W formé des éléments laissant fixes tous les points de A.

#### Proposition 2 {#lie-v-s3-prop-2 .statement}

Soit A une partie non vide de E, soit $ \mathfrak{H}_A $ l’ensemble des hyperplans $ H \in \mathfrak{H} $ contenant A, soit $ A' $ l’intersection des $ H \in \mathfrak{H}_A $ et soit F une facette de E, ouverte dans $ A' $ (§ 1, n° 3, prop. 7). On a $ W(A) = W(A') = W(F) $, et $ W(A) $ est engendré par les réflexions par rapport aux hyperplans de $ \mathfrak{H}_A $.

Démontrons tout d’abord l’assertion suivante :

(I) Soient C une chambre, x et y deux points de $ \overline{C} $ et $ w \in W $ tel que $ w(x) = y $. On a alors $ x = y $ et $ w $ appartient au sous-groupe $ W_{\mathfrak{N}} $, où $ \mathfrak{N} $ est l’ensemble des murs de C contenant x.

Nous raisonnons par récurrence sur la longueur q de w (relativement à l’ensemble S des réflexions par rapport aux murs de C), le cas $ q = 0 $ étant évident. Si $ q \geqslant 1 $, il existe un mur H de C et un élément $ w' \in W $ tel que $ w = s_H w' $ et $ l(w') = q - 1 $. Puisque $ l(s_H w) < l(w) $, les chambres C et $ w(C) $ sont de part et d’autre de H d’après le th. 1 du n° 2. On a donc $ \overline{C} \cap w(\overline{C}) \subset H $, d’où $ y \in H $. On a alors $ y = w'(x) $ et l’hypothèse de récurrence entraîne $ x = y $ et $ w' \in W_{\mathfrak{N}} $. De $ y \in H $ on déduit $ H \in \mathfrak{N} $, d’où $ w = s_H w' \in W_{\mathfrak{N}} $, ce qui termine la démonstration de (I).

Démonstration du théorème 2 : il résulte de (I) et du lemme 2.

Démonstration de la proposition 1 : on sait que deux facettes distinctes sont disjointes et ont des adhérences distinctes (\S 1, n° 2, cor. de la prop. 3). L’équivalence de (i), (ii) et (iii) en résulte. D’autre part, il est clair que

(vii) $ \Longrightarrow $ (vi) $ \Longrightarrow $ (v) $ \Longrightarrow $ (iv) $ \Longrightarrow $ (i)

et l’assertion (I) montre que (i) $ \Longrightarrow $ (vii).

Démonstration de la proposition 2 : soit $ A'' $ le sous-espace affine de E engendré par A. On a évidemment $ W(A) = W(A'') $. D’après la prop. 7 du \S 1, n° 3, il existe un point $ x \in A'' $ n’appartenant à aucun hyperplan $ H \in \mathfrak{H} - \mathfrak{H}_A $. Soit $ F_x $ la facette contenant $ x $ : elle est ouverte dans $ A'' $ et la prop. 1 montre que

$$
W(F_x) \subset W(A') \subset W(A) = W(A'') \subset W(\{x\}) = W(F_x)
$$

d’où $ W(A) = W(A') = W(F_x) $. En remplaçant A par F, on a aussi

$$
W(A) = W(F),
$$

d’où la proposition.

#### Remarque 1 {#lie-v-s3-n3-rem-1 .statement}

Il résulte du th. 2 que si C est une chambre et F une facette, *il existe une facette F' et une seule contenue dans $ \overline{C} $ qui soit transformée de F par un élément de W*.

#### Remarque 2 {#lie-v-s3-n3-rem-2 .statement}

Il résulte des prop. 1 et 2 que pour toute partie non vide A de E, il existe un point $ a \in E $ tel que $ W(A) = W(\{a\}) $; de plus, le groupe $ W(A) $ est un *groupe de Coxeter* (th. 1).

#### Remarque 3 {#lie-v-s3-n3-rem-3 .statement}

Soient C une chambre de E et S l’ensemble des réflexions par rapport aux murs de C. Soit $ w \in W $ et soit $ (s_1, \ldots, s_q) $ une décomposition réduite de $ w $ par rapport à S. Si $ x \in \overline{C} $ est fixe par $ w $, on a $ s_j(x) = x $ pour tout $ j $ : cela résulte de la prop. 1 ci-dessus et du cor. 1 de la prop. 7 du chap. IV, § 1.

### 4. Matrice et graphe de Coxeter de W

Soient C une chambre, $ S = S(C) $ l’ensemble des réflexions orthogonales par rapport aux murs de C et $ M = (m(s, s')) $ la matrice de Coxeter du système de Coxeter (W, S) (chap. IV, § 1, n° 9) : rappelons que $ m(s, s') $ est l’ordre (fini ou $ \infty $) de l’élément $ ss' $ de W (pour $ s, s' \in S $). Si $ C' $ est une autre chambre, l’unique élément $ w \in W $ tel que $ w(C) = C' $ définit une bijection

$$
s \mapsto f(s) = ws w^{-1}
$$

de S sur $ S' = S(C') $, et l’on a $ m(f(s), f(s')) = m(s, s') $. Il en résulte que, si l’on fait opérer W sur l’ensemble X des couples (C, s), où C est une chambre et où $ s \in S(C) $, en posant $ w.(C, s) = (w(C), ws w^{-1}) $, chaque orbite i de W dans X rencontre chacun des ensembles $ \{C\} \times S(C) $ en un point et un seul, que l’on note $ (C, s_i(C)) $. Soit alors I l’ensemble de ces orbites ; pour $ i, j \in I $, le nombre $ m_{ij} = m(s_i(C), s_j(C)) $ est indépendant du choix de la chambre C. La matrice

Soit C une chambre. Pour tout i \in I, on désigne par H_i(C) le mur de C tel que s_i(C) soit la réflexion par rapport à H_i(C) et par e_i(C) le vecteur unitaire orthogonal à H_i(C) et situé du même côté de H_i(C) que C. L’application i \mapsto H_i(C) est appelée la famille canoniquement indexée des murs de C.

#### Proposition 3 {#lie-v-s3-prop-3 .statement}

Soit C une chambre, et soient i, j \in I, avec i \neq j. Posons s_i = s_i(C), H_i = H_i(C), e_i = e_i(C) et définissons de même s_j, H_j et e_j.

(i) Si H_i et H_j sont parallèles, on a m_{ij} = \infty et e_i = -e_j.

(ii) Si H_i et H_j ne sont pas parallèles, alors m_{ij} est fini et on a :

$$
(e_i|e_j) = -\cos(\pi/m_{ij}).
$$

(iii) On a (e_i|e_j) \leq 0.

Si H_i et H_j sont parallèles, s_i s_j est une translation (\S 2, no 4, prop. 5), d’où m_{ij} = \infty. De plus, on a ou bien e_i = e_j, ou bien e_i = -e_j. Or il existe un point a (resp. a’) adhérent à C et appartenant à H_i (resp. H_j), mais n’appartenant pas à H_j (resp. H_i). On a alors (a’ - a|e_i) > 0 et (a - a’|e_j) > 0, ce qui exclut le cas e_i = e_j et démontre (i).

Supposons maintenant que H_i et H_j ne soient pas parallèles. Choisissons une origine a \in H_i \cap H_j et identifions T et E par la bijection t \mapsto a + t. Soit V le plan orthogonal à H_i \cap H_j passant par a. Posons \Gamma = V \cap D_{H_i}(C) \cap D_{H_j}(C) (où D_H(C) désigne le demi-espace ouvert limité par H et contenant C (\S 1, no 1)) et soit D (resp. D’) la demi-droite de V portée par H_i \cap V (resp. H_j \cap V) et contenue dans l’adhérence de \Gamma. Pour une orientation convenable de V l’ensemble \Gamma est la réunion des demi-droites ouvertes \Delta de V telles que

$$ 0 < (\overline{D, \Delta}) < (\overline{D, D'}) . $$

Soit W’ le sous-groupe de W engendré par s_i et s_j. Pour tout w \in W’, les hyperplans w(H_i) et w(H_j) appartiennent à \mathcal{S}, contiennent H_i \cap H_j et ne rencontrent pas C. Il en résulte qu’ils ne rencontrent pas \Gamma (\S 1, no 5, prop. 10). Le cor. de la prop. 7 du \S 2, no 5 entraîne alors (ii).

Enfin, l’assertion (iii) résulte immédiatement de (i) et (ii), puisque m_{ij} \geq 2 pour i \neq j.

#### Remarque {#lie-v-s3-n4-rem-1 .statement}

La formule (4) est en fait valable quels que soient i, j \in I : en effet, on a \pi/m_{ij} = 0 si m_{ij} = \infty, et si i = j, on a m_{ij} = 1 et (e_i|e_j) = 1.

### 5. Systèmes de vecteurs à produits scalaires négatifs

#### Lemme 3 {#lie-v-s3-lem-3 .statement}

Soit q une forme quadratique positive sur un espace vectoriel réel V et soit B la forme bilinéaire symétrique associée. Soient a_1, \ldots, a_n des éléments de V tels que B(a_i, a_j) \leq 0 pour i \neq j.

(i) Si $ c_1, \ldots, c_n $ sont des nombres réels tels que $ q\left( \sum_i c_i a_i \right) = 0 $, on a
$$
q\left( \sum_i |c_i| \cdot a_i \right) = 0.
$$
(ii) Si $ q $ est non dégénérée et s’il existe une forme linéaire $ f $ sur $ V $ telle que $ f(a_i) > 0 $ pour tout $ i $, les vecteurs $ a_1, \ldots, a_n $ sont linéairement indépendants.
La relation $ B(a_i, a_j) \leq 0 $ pour $ i \neq j $ entraîne aussitôt
$$
q\left( \sum_i |c_i| \cdot a_i \right) \leq q\left( \sum_i c_i a_i \right),
$$
d’où (i). Si $ q $ est non dégénérée, la relation $ \sum_i c_i a_i = 0 $ entraîne donc
$$
\sum_i |c_i| \cdot a_i = 0;
$$
pour toute forme linéaire $ f $ sur $ V $, on en déduit $ \sum_i |c_i| \cdot f(a_i) = 0 $, d’où $ c_i = 0 $ pour tout $ i $, si de plus $ f(a_i) > 0 $ pour tout $ i $. Cela démontre (ii).

#### Lemme 4 {#lie-v-s3-lem-4 .statement}

Soit $ Q = (q_{ij}) $ une matrice réelle carrée symétrique d’ordre $ n $ telle que :
a) on a $ q_{ij} \leq 0 $ pour $ i \neq j $;
b) il n’existe pas de partition de $ \{1, 2, \ldots, n\} $ en deux ensembles non vides $ I $ et $ J $ tels que $ (i, j) \in I \times J $ entraîne $ q_{ij} = 0 $;
c) la forme quadratique $ q(x_1, \ldots, x_n) = \sum_{i,j} q_{ij} x_i x_j $ sur $ \mathbf{R}^n $ est positive.

Alors :
(i) Le noyau $ N $ de $ q $ est de dimension 0 ou 1. Si $ \dim N = 1 $, $ N $ est engendré par un vecteur dont toutes les coordonnées sont $ > 0 $.
(ii) La plus petite valeur propre de $ Q $ est de multiplicité 1 et un vecteur propre correspondant a toutes ses coordonnées $ > 0 $, ou toutes ses coordonnées $ < 0 $.

Comme $ q $ est une forme quadratique positive, le noyau $ N $ de $ q $ est l’ensemble des vecteurs isotropes pour $ q $ (Alg., chap. IX, § 7, no 1, cor. de la prop. 2). Soit $ a_1, \ldots, a_n $ la base canonique de $ \mathbf{R}^n $. Si $ \sum_i c_i a_i \in N $, le lemme 3 montre que l’on a aussi $ \sum_i |c_i| \cdot a_i \in N $, d’où $ \sum_i q_{ji}|c_i| = 0 $ pour tout $ j $. Soit alors $ I $ l’ensemble des $ i $ tels que $ c_i \neq 0 $. Si $ j \notin I $, on a $ q_{ji}|c_i| \leq 0 $ pour $ i \in I $ et $ q_{ji}|c_i| = 0 $ pour $ i \notin I $, d’où $ q_{ji} = 0 $ pour $ j \notin I $ et $ i \in I $. L’hypothèse b) entraîne donc que ou bien $ I = \varnothing $, ou bien $ I = \{1, \ldots, n\} $. Par suite, tout vecteur non nul de $ N $ a toutes ses coordonnées $ \neq 0 $. Si on avait $ \dim N \geq 2 $, l’intersection de $ N $ et de l’hyperplan d’équation $ x_i = 0 $ serait de dimension $ \geq 1 $, contrairement à ce que l’on vient de voir. En outre, ce qui précède montre que, si $ \dim N = 1 $, alors $ N $ contient un vecteur de coordonnées toutes $ > 0 $. Ceci achève la démonstration de (i).

D’autre part, on sait que les valeurs propres de $ Q $ sont réelles (Alg., chap. IX, § 7, no 3, prop. 5) et positives puisque $ q $ est positive. Soit $ \lambda $ la plus petite d’entre elles. La matrice $ Q' = Q - \lambda I_n $ est alors la matrice d’une forme positive dégénérée $ q' $ et les éléments non diagonaux de $ Q' $ sont les mêmes que ceux de $ Q $. Par suite, $ Q' $ satisfait aux conditions $ a), b) $ et $ c) $ de l’énoncé. Comme le noyau $ N' $ de $ q' $ est le sous-espace propre de $ Q $ correspondant à la valeur propre $ \lambda $, l’assertion (ii) résulte de (i).

#### Lemme 5 {#lie-v-s3-lem-5 .statement}

*Soient $ e_1, \ldots, e_n $ des vecteurs engendrant $ T $ tels que :*
    *a)* $ (e_i|e_j) \leq 0 $ pour $ i \neq j; $
    *b)* *il n’existe pas de partition de $ \{1, \ldots, n\} $ en deux ensembles $ I $ et $ J $ non vides tels que $ (e_i|e_j) = 0 $ pour $ i \in I $ et $ j \in J $.*
    *Alors deux cas sont possibles :*
        1) $ (e_1, \ldots, e_n) $ est une base de $ T; $
        2) $ n = \dim T + 1; $ *il existe une famille $ (c_i)_{1 \leq i \leq n} $ de nombres réels $ > 0 $ tels que $ \sum_i c_i e_i = 0, $ et toute famille $ (c'_i)_{1 \leq i \leq n} $ de nombres réels tels que $ \sum_i c'_i e_i = 0 $ est proportionnelle à $ (c_i)_{1 \leq i \leq n} $.*

    Posons $ q_{ij} = (e_i|e_j) $. La matrice $ Q = (q_{ij}) $ satisfait alors aux hypothèses du lemme 4 : les conditions $ a) $ et $ b) $ du lemme 4 sont les mêmes que les conditions $ a) $ et $ b) $ ci-dessus, et $ c) $ est satisfaite puisque $ \sum_{i,j} q_{ij} x_i x_j = \sum_i ||x_i e_i||^2 $. Le noyau $ N $ de la forme quadratique $ q $ sur $ \mathbf{R}^n $, de matrice $ Q $, est l’ensemble des $ (c_1, \ldots, c_n) \in \mathbf{R}^n $ tels que $ \sum_i c_i e_i = 0 $. Si $ N = \{0\} $, les $ e_i $ sont linéairement indépendants et l’on est dans le cas 1). Si $ \dim N > 0 $, le lemme 4 (i) montre que l’on est dans le cas 2).

#### Lemme 6 {#lie-v-s3-lem-6 .statement}

*Soit $ (e_1, \ldots, e_n) $ une base de $ T $ telle que $ (e_i|e_j) \leq 0 $ pour $ i \neq j $.*
    *(i)* *Si $ x = \sum_i c_i e_i \in T $ est tel que $ (x|e_i) \geq 0 $ pour tout $ i $, on a $ c_i \geq 0 $ pour tout $ i $.*
    *(ii)* *Si $ x $ et $ y $ sont deux éléments de $ T $ tels que $ (x|e_i) \geq 0 $ et $ (y|e_i) \geq 0 $ pour tout $ i $, on a $ (x|y) \geq 0 $. Si $ (x|e_i) > 0 $ et $ (y|e_i) > 0 $ pour tout $ i $, on a $ (x|y) > 0 $.*

Plaçons-nous dans les hypothèses de (i) et supposons qu’il existe un $ i $ tel que $ c_i < 0 $. Soit $ f $ la forme linéaire sur $ T $ définie par $ f(e_i) = 1 $ et
$$
f(e_j) = -c_i / (\sum_{k=1}^n |c_k|)
$$
pour $ j \neq i $.

Les vecteurs — $ x, e_1, \ldots, e_n $ satisfont alors aux hypothèses du lemme 3 (ii) (en prenant pour $ q $ la forme métrique de $ T $). On en conclut qu’ils sont linéairement indépendants, ce qui est absurde. D’où (i). De plus, si $ x = \sum_i c_i e_i \in T $ et si $ y \in T $, on a $ (x|y) = \sum_i c_i (e_i|y) $, de sorte que (ii) résulte immédiatement de (i).

### 6. Théorèmes de finitude

#### Lemme 7 {#lie-v-s3-lem-7 .statement}

*Soit $ A $ un ensemble de vecteurs unitaires de $ T $. S’il existe un nombre réel $ \lambda < 1 $ avec $ (a|a') \leq \lambda $ pour $ a, a' \in A $ et $ a \neq a' $, alors l’ensemble $ A $ est fini.*

Pour $ a, a' \in A $ tels que $ a \neq a' $, on a :

$$
||a - a'||^2 = 2 - 2(a|a') \geq 2 - 2\lambda.
$$

Or, la sphère unité S de T étant compacte, il existe un recouvrement fini de S par des ensembles de diamètre $ < (2 - 2\lambda)^{1/2} $ et chacun de ces ensembles contient au plus un point de A, d’où le lemme.

Notons $ U(w) $ l’automorphisme de T associé à l’application affine $ w \bullet W $ de E dans lui-même. On a

$$
w(x + t) = w(x) + U(w).t \quad \text{pour } t \in T \text{ et } x \in E.
$$

On définit ainsi un homomorphisme $ U $ du groupe W dans le groupe orthogonal de T ; le noyau de $ U $ est l’ensemble des translations appartenant à W.

#### Théorème 3 {#lie-v-s3-thm-3 .statement}

(i) *L’ensemble des murs d’une chambre est fini.*
(ii) *L’ensemble des directions des hyperplans appartenant à $ \mathfrak{H} $ est fini.*
(iii) *Le groupe $ U(W) $ est fini.*

L’assertion (i) résulte aussitôt de la prop. 3, (iii) et du lemme 7. Démontrons (ii). Soient C une chambre et $ \mathfrak{M} $ l’ensemble de ses murs. Les facettes de $ \overline{C} $ (relativement à $ \mathfrak{H} $) sont les mêmes que celles relativement à $ \mathfrak{M} $ ($ \S 1 $, no 4, prop. 9). Puisque $ \mathfrak{M} $ est fini, elles sont en nombre fini. Comme une facette ne rencontre qu’un nombre fini d’hyperplans appartenant à $ \mathfrak{H} $, l’ensemble des hyperplans appartenant à $ \mathfrak{H} $ et rencontrant $ \overline{C} $ est fini, ainsi que l’ensemble $ A(C) $ des vecteurs unitaires de T orthogonaux à un hyperplan appartenant à $ \mathfrak{H} $ et rencontrant $ \overline{C} $. Par suite, il existe un nombre réel $ \lambda < 1 $ tel que $ (a|a') \leq \lambda $ pour $ a, a' \in A(C) $ et $ a \neq a' $.

Soit alors A l’ensemble des vecteurs unitaires de T qui sont orthogonaux à un hyperplan appartenant à $ \mathfrak{H} $. Soient $ a, a' \in A $ avec $ a \neq a' $. Si $ a $ et $ a' $ sont parallèles, on a $ a = -a' $ et $ (a|a') = -1 $. Sinon, soit $ H \in \mathfrak{H} $ (resp. $ H' \in \mathfrak{H} $) tel que $ a $ (resp. $ a' $) soit orthogonal à $ H $ (resp. $ H' $). On a $ H \cap H' \neq \emptyset $, et si $ x \in H \cap H' $, il existe un élément $ w \in W $ tel que $ x \in w(\overline{C}) $. Les vecteurs $ U(w).a $ et $ U(w).a' $ appartiennent alors à $ A(C) $, l’on a :

$$
(a|a') = (U(w).a|U(w).a') \leq \lambda
$$

et l’ensemble A est fini d’après le lemme 7. D’où (ii).

Soit maintenant $ w \in W $ tel que $ U(w).a = a $ pour tout $ a \in A $. On a alors $ U(w).t = t $ pour tout $ t $ appartenant au sous-espace de T engendré par A. D’autre part, si $ t \in T $ est orthogonal à A, on a $ U(s_H).t = t $ pour tout $ H \in \mathfrak{H} $, d’où $ U(w).t = t $ et finalement $ U(w) = 1 $. Comme $ U(w)(A) = A $ pour tout $ w \in W $, on en déduit que $ U(W) $ est isomorphe à un groupe de permutations de l’ensemble fini A, d’où (iii).

#### Proposition 4 {#lie-v-s3-prop-4 .statement}

*Soient C une chambre et $ \mathfrak{N} $ un ensemble de murs de C. Soit $ W_{\mathfrak{N}} $ le sous-groupe de W engendré par les réflexions orthogonales par rapport aux éléments de $ \mathfrak{N} $.*

Pour $ H \in \mathfrak{N} $, notons $ e_H $ le vecteur unitaire orthogonal à $ H $ situé du même côté que $ C $ de $ H $. Les conditions suivantes sont équivalentes :

(i) Le groupe $ W_{\mathfrak{N}} $ est fini.
(ii) Il existe un point de $ E $ invariant par tout élément de $ W_{\mathfrak{N}} $.
(iii) Les hyperplans appartenant à $ \mathfrak{N} $ ont une intersection non vide.
(iv) La famille de vecteurs $ (e_H)_{H \in \mathfrak{N}} $ est libre dans $ T $.

Supposons que $ W_{\mathfrak{N}} $ ait un cardinal fini $ d $. Pour tout point $ a $ de $ E $, le point $ b = \sum_{w \in W_{\mathfrak{N}}} d^{-1} \cdot w(a) $ est invariant par $ W_{\mathfrak{N}} $, donc (i) entraîne (ii).

D’après la propriété (D 2) du début du § 3, le stabilisateur dans $ W $ de tout point de $ E $ est fini, donc (ii) entraîne (i).

Comme le groupe $ W_{\mathfrak{N}} $ est engendré par l’ensemble des réflexions par rapport aux hyperplans appartenant à $ \mathfrak{N} $, les points fixes de $ W_{\mathfrak{N}} $ sont les points de $ E $ appartenant à tout hyperplan $ H \in \mathfrak{N} $, d’où l’équivalence de (ii) et (iii).

Supposons qu’il existe un point $ a $ de $ E $ tel que $ a \in H $ pour tout $ H \in \mathfrak{N} $ et soit $ t \in T $ tel que $ a + t \in C $. Puisque $ (e_H|e_{H'}) \leq 0 $ pour $ H, H' \in \mathfrak{N} $, tels que $ H \neq H' $ (prop. 3), et que $ (t|e_H) > 0 $ pour tout $ H \in \mathfrak{N} $, le lemme 3 (ii) entraîne que les $ e_H $ pour $ H \in \mathfrak{N} $ sont linéairement indépendants. Par suite (iii) entraîne (iv).

Supposons enfin que la famille $ (e_H)_{H \in \mathfrak{N}} $ soit libre. Soit $ a $ un point de $ E $. Pour tout hyperplan $ H \in \mathfrak{N} $, il existe un nombre réel $ c_H $ tel que $ H $ se compose des points $ a + t $ de $ E $ avec $ (t|e_H) = c_H $. Puisque la famille $ (e_H) $ est libre, il existe $ t \in T $ tel que $ (t|e_H) = c_H $ pour tout $ H \in \mathfrak{N} $, et le point $ a + t $ de $ E $ appartient à tous les hyperplans $ H \in \mathfrak{N} $. Donc (iv) entraîne (iii).

#### Remarque 1 {#lie-v-s3-n6-rem-1 .statement}

Comme $ W $ est engendré par les réflexions par rapport aux murs de la chambre $ C $, la proposition précédente donne un critère pour que $ W $ soit fini. Nous reviendrons sur cette question au n° 9.

#### Remarque 2 {#lie-v-s3-n6-rem-2 .statement}

Soient $ F $ un espace affine réel de dimension finie et $ G $ un groupe d’automorphismes de $ F $. Pour tout $ g \in G $, notons $ U(g) $ l’automorphisme de l’espace des translations $ V $ de $ F $ associé à $ g $. Supposons que l’image $ U(G) $ soit un sous-groupe fini de $ \mathbf{GL}(V) $; il existe alors sur $ V $ un produit scalaire invariant par $ U(G) $ (Intégr., chap. VII, § 3, n° 1, prop. 1). Si de plus $ G $ opère proprement sur $ F $ lorsqu’on le munit de la topologie discrète et qu’il soit engendré par des réflexions, on peut donc appliquer à $ G $ tous les résultats du présent paragraphe.

### 7. Décomposition de la représentation linéaire de $ W $ dans $ T $

Soit $ I $ l’ensemble des sommets du graphe de Coxeter de $ W $ (n° 4) et soit $ J $ une partie de $ I $ telle qu’un sommet de $ J $ et un sommet de $ I - J $ ne soient jamais liés. Soient $ C $ une chambre, $ s $ la bijection canonique de $ I $ sur l’ensemble des réflexions par rapport aux murs de $ C $, et soit $ W_{J,C} $ le sous-groupe engendré par l’image $ s(J) $. Il résulte alors du chap. IV, § 1, n° 9, prop. 8, que $ W $ est produit direct des deux sous-groupes $ W_{J,C} $ et $ W_{I-J,C} $. Soient $ C' $ une autre chambre et s' l’injection correspondante de I dans W. Nous avons vu (n° 4) que si $ w \in W $ transforme C en C', on a $ s'(i) = ws(i)w^{-1} $ pour $ i \in I $. Puisque $ W_{J,C} $ est distingué dans W, il en résulte que $ s'(i) \in W_{J,C} $ pour tout $ i \in J $. On en déduit que le sous-groupe $ W_{J,C} $ ne dépend pas de C. Nous le noterons simplement $ W_J $ dans ce qui suit.

La définition de $ W_{J,C} $ s’étend évidemment à une partie J quelconque de I. Mais s’il existe un sommet de J et un sommet de I — J qui soient liés, alors $ W_{J,C} $ n’est pas distingué et dépend du choix de la chambre C.

Soit $ T_J^0 $ le sous-espace de T formé des vecteurs invariants par tout élément de $ U(W_J) $ et soit $ T_J $ le sous-espace orthogonal à $ T_J^0 $. Puisque $ W_J $ est un sous-groupe distingué de W, il est clair que $ T_J^0 $ est invariant par $ U(W) $, donc aussi $ T_J $.

#### Proposition 5 {#lie-v-s3-prop-5 .statement}

Soient $ J_1, \ldots, J_s $ les ensembles de sommets des composantes connexes du graphe de Coxeter de W. Pour $ 1 \leq p \leq s $, posons

$$
W_p = W_{J_p}, \quad T_p = T_{J_p}, \quad T'_p = T_{J_p}^0 \quad \text{et} \quad T_0 = \bigcap_{1 \leq p \leq s} T'_p.
$$

(i) Le groupe W est produit direct des sous-groupes $ W_p $ ($ 1 \leq p \leq s $).

(ii) L’espace T est somme directe orthogonale des sous-espaces $ T_0, T_1, \ldots, T_s $, qui sont stables par $ U(W) $.

(iii) Pour tout q tel que $ 1 \leq q \leq s $, le sous-espace $ T'_q $ de T est formé des vecteurs invariants par $ U(W_q) $; il est somme directe des $ T_p $ pour $ 0 \leq p \leq s $ et $ p \neq q $.

(iv) Soit C une chambre. Le sous-espace $ T_p $ (pour $ 1 \leq p \leq s $) est engendré par les vecteurs $ e_i(C) $ pour $ i \in J_p $ (notations du n° 4).

(v) Les représentations de W dans les sous-espaces $ T_p $ ($ 1 \leq p \leq s $) sont absolument irréductibles, non triviales, et deux à deux non équivalentes.

L’assertion (i) résulte du chap. IV, § 1, n° 9. D’autre part, nous avons déjà vu que les sous-espaces $ T_p $ sont invariants par $ U(W) $, et il en est de même de $ T_0 $. Soit C une chambre; comme $ W_p $ est engendré par les réflexions $ s_i(C) $ pour $ i \in J_p $, il est clair que $ T'_p $ est le sous-espace orthogonal aux $ e_i(C) $ pour $ i \in J_p $, d’où (iv). Par ailleurs, si $ i \in J_p, j \in J_q $ avec $ p \neq q $, on a $ m_{ij} = 2 $ puisque $ \{i, j\} $ n’est pas une arête du graphe de Coxeter de W, d’où $ (e_i|e_j) = 0 $. On en déduit aussitôt (ii). L’assertion (iii) en résulte, puisque $ T'_q $ est l’orthogonal de $ T_q $.

Enfin, soit V un sous-espace de $ T_p $ invariant par $ U(W_p) $. Pour tout $ i \in J_p $, ou bien on a $ e_i \in V $, ou bien $ e_i $ est orthogonal à V ($ \S 2 $, n° 2, prop. 3). Soit A (resp. B) l’ensemble des $ i \in J_p $ tels que $ e_i \in V $ (resp. $ e_i $ orthogonal à V). On a évidemment $ (e_i|e_j) = 0 $ pour $ i \in A $ et $ j \in B $, et puisque $ J_p $ est connexe, on en déduit, ou bien $ A = \emptyset $ et $ V = \{0\} $, ou bien $ A = J_p $ et $ V = T_p $. Par suite, la représentation de $ W_p $ dans $ T_p $ est irréductible, donc absolument irréductible ($ \S 2 $, n° 1, prop. 1). Elle est non triviale par définition même de $ T_p $. Enfin, la dernière assertion de (v) résulte aussitôt de (iii).

On dit que W est essentiel si le sous-espace T_0 des vecteurs de T invariants par U(W) est réduit à {0}; on dit que W est irréductible si la représentation U de W dans T est irréductible.

#### Corollaire {#lie-v-s3-n7-cor-1 .statement}

Supposons W ≠ {1}. Pour que W soit irréductible, il faut et il suffit qu’il soit essentiel et que son graphe de Coxeter soit connexe.

#### Remarque {#lie-v-s3-n7-rem-1 .statement}

Sous les hypothèses de la prop. 5, les sous-espaces T_p pour 0 ≤ p ≤ s sont les composantes isotypiques de la représentation linéaire U de W dans T (Alg., chap. VIII, § 3, no 4). Il en résulte (loc. cit., prop. 11) que tout sous-espace vectoriel V de T stable par W est somme directe des sous-espaces V ∩ T_p pour 0 ≤ p ≤ s; de plus (loc. cit., prop. 10) tout endomorphisme commutant aux opérateurs U(w) pour w ∈ W, laisse stable chacun des T_p pour 0 ≤ p ≤ s et y induit une homothétie pour 1 ≤ p ≤ s. En particulier, les formes bilinéaires Φ sur T invariantes par W sont les formes bilinéaires données par:

$$
\Phi(\sum_k t_k, \sum_k t'_k) = \Phi_0(t_0, t'_0) + \sum_{1 \leq p \leq s} a_p(t_p|t'_p)
$$

où Φ_0 est une forme bilinéaire sur T_0 et a_p (pour 1 ≤ p ≤ s) un nombre réel : en effet, une telle forme Φ s’écrit d’une manière et d’une seule (t, t') ↦ (A(t)|t'), où A est un endomorphisme de T commutant aux U(w) pour w ∈ W.

### 8. Décomposition de l’espace affine E en produit

Conservons les notations de la prop. 5. Pour 0 ≤ p ≤ s, soit E_p l’ensemble des orbites du groupe T'_p dans E, et soit φ_p l’application canonique de E sur E_p. Les opérations de T dans E passent au quotient ; en particulier, T_p opère sur E_p et on vérifie immédiatement (par exemple en prenant une origine dans E) que E_p est un espace affine admettant T_p comme espace des translations. Posons E' = E_0 × ... × E_s : c’est un espace affine ayant T = T_0 ⊕ ... ⊕ T_s comme espace des translations. Soit φ : E → E' l’application produit des φ_p; comme φ commute aux opérations de T, c’est une bijection et même un isomorphisme d’espaces affines. Dans ce qui suit, nous identifierons E et E' au moyen de φ ; l’application φ_p s’identifie alors à la projection canonique de E' sur E_p.

Comme W laisse stable T'_p, les opérations de W dans E passent au quotient et définissent une loi d’opération de W dans E_p (pour 0 ≤ p ≤ s), d’où par restriction une loi d’opération de W_p dans E_p (pour 1 ≤ p ≤ s). D’autre part, soit C une chambre, soit i ∈ I et soit p l’entier tel que i ∈ J_p. Pour tout x ∈ E, on a:

$$
s_i(C)(x) = x - \lambda . e_i(C) \quad \text{avec } \lambda \in \mathbf{R}.
$$

Comme e_i ∈ T'_q pour q ≠ p, on en déduit que

$$
\varphi_q(w(x)) = \varphi_q(x) \quad \text{pour } x \in E, w \in W_p, 0 \leq q \leq s \text{ et } q \neq p.
$$

Par suite, si $ w = w_1 \ldots w_s \in W $ avec $ w_p \in W_p $ pour $ 1 \leq p \leq s $, on a :

$$
w((x_0, \ldots, x_s)) = (x_0, w_1(x_1), \ldots, w_s(x_s))
$$

quels que soient les $ x_p \in E_p $ pour $ 0 \leq p \leq s $. Autrement dit, la loi d’opération de $ W $ dans $ E = E' $ n’est autre que la loi produit des lois d’opérations des $ W_p $ dans les $ E_p $ (en posant $ W_0 = \{1\} $). Il en résulte que $ W_p $ opère fidèlement dans $ E_p $ et qu’on peut identifier $ W_p $ à un groupe de déplacements de l’espace euclidien $ E_p $ (l’espace des translations $ T_p $ de $ E_p $ étant naturellement muni du produit scalaire induit par celui de $ T $).

#### Proposition 6 {#lie-v-s3-prop-6 .statement}

(i) Le groupe $ W_p $ est un groupe de déplacements de l’espace affine euclidien $ E_p $; il est engendré par des réflexions; muni de la topologie discrète, il opère proprement dans $ E_p $; il est irréductible.

(ii) Soit $ \mathfrak{H}_p $ l’ensemble des hyperplans $ H $ de $ E_p $ tels que $ s_H \in W_p $. L’ensemble $ \mathfrak{H} $ se compose des hyperplans de la forme

$$
H = E_0 \times E_1 \times \cdots \times E_{p-1} \times H_p \times E_{p+1} \times \cdots \times E_s
$$

avec $ p = 1, \ldots, s $ et $ H_p \in \mathfrak{H}_p $.

(iii) Toute chambre $ C $ est de la forme $ E_0 \times C_1 \times \cdots \times C_s $, où pour chaque $ p $ l’ensemble $ C_p $ est une chambre définie dans $ E_p $ par l’ensemble d’hyperplans $ \mathfrak{H}_p $; de plus $ C_p $ admet pour murs les hyperplans $ \varphi_p(H_i(C)) $ pour $ i \in J_p $.

Soit $ C $ une chambre. Posons $ H_i = H_i(C) $, $ e_i = e_i(C) $ et $ s_i = s_i(C) $ pour $ i \in I $ (notations du no 4).

(i) Soit $ i $ dans $ J_p $; comme on a $ e_i \in T_p $ et que $ T $ est somme directe des sous-espaces mutuellement orthogonaux $ T_0, T_1, \ldots, T_s $, l’hyperplan de $ T $ orthogonal à $ e_i $ est de la forme $ L_i + T'_p $ où $ L_i $ est l’hyperplan de $ T_p $ orthogonal à $ e_i $. L’hyperplan affine $ H_i $ de $ E $ est de la forme $ L_i + T'_p + x $, avec $ x \in E $, et on a :

$$
H_i = E_0 \times E_1 \times \cdots \times E_{p-1} \times H'_i \times E_{p+1} \times \cdots \times E_s
$$

avec $ H'_i = L_i + \varphi_p(x) = \varphi_p(H_i) $. Il est alors immédiat que $ s_i $ opère dans $ E_p $ par la réflexion associée à l’hyperplan $ H'_i $ de $ E_p $. Donc le groupe $ W_p $ est un groupe de déplacements engendré par des réflexions dans $ E_p $; la vérification du critère (D’ 2) de propreté est immédiate. Enfin, la prop. 5, (v) montre que $ W_p $ est irréductible. On a prouvé (i).

(ii) D’après le cor. du th. 1, l’ensemble $ \mathfrak{H}_p $ se compose des hyperplans de la forme $ w_p(H'_i) $ pour $ i $ dans $ J_p $ et $ w_p $ dans $ W_p $. Par ailleurs, si $ w = w_1 \ldots w_s $ avec $ w_p \in W_p $ pour tout $ p $, les formules (5) et (6) entraînent

$$
w(H_i) = E_0 \times E_1 \times \cdots \times E_{p-1} \times w_p(H'_i) \times E_{p+1} \times \cdots \times E_s
$$

d’où immédiatement (ii).

(iii) Soit $ i $ dans $ J_p $; d’après la formule (6), le demi-espace ouvert $ D_i $ limité par $ H_i $ contenant $ C $ est de la forme
$$
D_i = E_0 \times E_1 \times \cdots \times E_{p-1} \times D'_i \times E_{p+1} \times \cdots \times E_s
$$
où $ D'_i $ est un demi-espace ouvert limité par $ H'_i $ dans $ E_p $. Posons $ C_p = \bigcap_{i \in J_p} D'_i $; puisque l’on a $ C = \bigcap_{i \in I} D_i $, on en déduit immédiatement
$$
C = E_0 \times C_1 \times \cdots \times C_s;
$$
par suite aucun des ensembles $ C_p $ n’est vide, et comme $ C $ ne rencontre aucun hyperplan appartenant à $ \mathfrak{S} $, l’ensemble $ C_p $ ne rencontre aucun hyperplan appartenant à $ \mathfrak{S}_p $. La prop. 5 du § 1, no 3 montre alors que $ C_p $ est l’une des chambres définies par $ \mathfrak{S}_p $ dans $ E_p $. En utilisant la prop. 4 du § 1, no 2, on voit facilement que les murs de $ C_p $ sont les hyperplans $ H'_i = \varphi_p(H_i) $ pour $ i \in J_p $.

### 9. Structure des chambres

Soient $ C $ une chambre, $ \mathcal{M} $ l’ensemble des murs de $ C $ et pour $ H \in \mathcal{M} $, soit $ e_H $ le vecteur unitaire orthogonal à $ H $ situé du même côté que $ C $ de l’hyperplan $ H $.

#### Proposition 7 {#lie-v-s3-prop-7 .statement}

Supposons que le groupe $ W $ soit essentiel et fini. Alors :
(i) Il existe un unique point $ a $ de $ E $ invariant par $ W $.
(ii) La famille $ (e_H)_{H \in \mathcal{M}} $ est une base de $ T $.
(iii) La chambre $ C $ est le cône simplicial ouvert de sommet $ a $ défini par la base $ (e'_H)_{H \in \mathcal{M}} $ de $ T $ telle que $ (e_H|e'_{H'}) = \delta_{HH'} $.

(i) D’après la prop. 4 du no 6, il existe un point $ a \in E $ invariant par $ W $. Soit $ t \in T $ tel que $ t + a $ soit invariant par $ W $. Pour tout $ w \in W $, on a
$$
U(w).t + a = w(t + a) = t + a,
$$
d’où $ U(w).t = t $; comme $ W $ est essentiel, cela entraîne $ t = 0 $, ce qui montre l’unicité de $ a $.

(ii) Comme $ W $ est essentiel, on a $ T = T_1 $ avec les notations du no 7, et la prop. 5, (iv) montre que la famille $ (e_H)_{H \in \mathcal{M}} $ engendre l’espace vectoriel $ T $. L’existence d’un point de $ E $ invariant par $ W $ montre que la famille $ (e_H)_{H \in \mathcal{M}} $ est libre (no 6, prop. 4).

(iii) Soit $ a $ l’unique point de $ E $ invariant par $ W $. Comme $ (e_H)_{H \in \mathcal{M}} $ est une base de $ T $, et que le produit scalaire est une forme bilinéaire non dégénérée sur $ T $, il existe une base $ (e'_H)_{H \in \mathcal{M}} $ de $ T $ et une seule telle que $ (e_H|e'_{H'}) = \delta_{HH'} $ pour $ H, H' $ dans $ \mathcal{M} $. Tout point $ x $ de $ E $ s’écrit de manière unique sous la forme $ x = t + a $ avec $ t = \sum_{H \in \mathcal{M}} \xi_H \cdot e'_H $ et les $ \xi_H $ réels. Pour que $ x $ appartienne à $ C $, il faut et il suffit que, pour tout hyperplan $ H \in \mathcal{M} $, il soit du même côté de $ H $ que $ e_H $, c’est-à-dire que $ (t|e_H) = \xi_H $ soit strictement positif. D’où (iii).

#### Proposition 8 {#lie-v-s3-prop-8 .statement}

Supposons que le groupe W soit essentiel, irréductible et infini. Alors :
(i) Aucun point de E n’est invariant par W.
(ii) On a Card $ \mathfrak{M} = \dim T + 1 $, et il existe des nombres réels $ c_H > 0 $ tels que $ \sum_{H \in \mathfrak{M}} c_H \cdot e_H = 0 $. Si les nombres réels $ c'_H $ sont tels que $ \sum_{H \in \mathfrak{M}} c'_H \cdot e_H = 0 $, il existe $ \xi $ réel avec $ c'_H = \xi c_H $ pour tout H dans $ \mathfrak{M} $.
(iii) La chambre C est un simplexe ouvert.

L’assertion (i) résulte de la prop. 4. D’autre part, puisque W est essentiel, les vecteurs $ (e_H)_{H \in \mathfrak{M}} $ engendrent T. On a $ (e_H|e_{H'}) \leq 0 $ pour $ H, H' \in \mathfrak{M} $ et $ H \neq H' $ (prop. 3) et, puisque W est irréductible, il n’existe pas de partition de $ \mathfrak{M} $ en deux ensembles non vides $ \mathfrak{M}' $ et $ \mathfrak{M}'' $ telle que $ H' \in \mathfrak{M}' $ et $ H'' \in \mathfrak{M}'' $ entraînent $ (e_{H'}|e_{H''}) = 0 $. On peut donc appliquer le lemme 5 du n° 5, et le cas 1) de ce lemme est exclu : en effet, les $ e_H $ ne sont pas linéairement indépendants, puisque W n’a pas de point fixe. L’assertion (ii) en résulte.

Démontrons (iii). Numérotons les murs de C sous la forme $ H_0, H_1, \ldots, H_d $ et posons $ t_m = e_{H_m} $. D’après (ii), les vecteurs $ t_1, \ldots, t_d $ forment une base de T, donc les hyperplans $ H_1, \ldots, H_d $ ont un point $ a_0 $ en commun, et il existe une base $ (t'_1, \ldots, t'_d) $ de T telle que $ (t_m|t'_n) = \delta_{mn} $; de plus, toujours d’après (ii), il existe des nombres réels $ c_1 > 0, \ldots, c_d > 0 $ tels que
$$
t_0 = - (c_1 \cdot t_1 + \cdots + c_d \cdot t_d).
$$
Comme le vecteur $ t_0 $ est orthogonal à l’hyperplan $ H_0 $, il existe un nombre réel $ c $ tel que $ H_0 $ soit l’ensemble des points $ x = t + a_0 $ de E avec $ (t|t_0) = -c $.

Tout point de E s’écrit de manière unique sous la forme $ x = t + a_0 $ avec $ t = \xi_1 \cdot t'_1 + \cdots + \xi_d \cdot t'_d $ et $ \xi_1, \ldots, \xi_d $ réels. Pour que $ x $ appartienne à C, il faut et il suffit qu’il soit du même côté de $ H_m $ que $ t_m $ pour $ 0 \leq m \leq d $; ceci se traduit par les inégalités $ (t|t_1) > 0, \ldots, (t|t_d) > 0 $, et $ (t|t_0) > -c $, ou encore par $ \xi_1 > 0, \ldots, \xi_d > 0, c_1 \xi_1 + \cdots + c_d \xi_d < c $. Comme C est non vide, on a $ c > 0 $. Posons $ a_m = a_0 + \frac{c}{c_m} \cdot t'_m $ pour $ 1 \leq m \leq d $; la chambre C se compose alors des points de E de la forme $ a_0 + \sum_{m=1}^d \lambda_m \cdot (a_m - a_0) $ avec $ \lambda_1 > 0, \ldots, \lambda_d > 0 $ et $ \lambda_1 + \cdots + \lambda_d < 1 $, donc C est le simplexe ouvert de sommets $ a_0, \ldots, a_d $.

#### Remarque 1 {#lie-v-s3-n9-rem-1 .statement}

Identifions E à $ E_0 \times E_1 \times \cdots \times E_s $, et W à $ W_1 \times \cdots \times W_s $ comme au n° 8. D’après la prop. 6, la chambre C s’identifie alors à
$$
E_0 \times C_1 \times \cdots \times C_s
$$
où $ C_p $ est une chambre dans $ E_p $ par rapport à l’ensemble $ \mathfrak{S}_p $ d’hyperplans. D’après les prop. 7 et 8, chacune des chambres $ C_1, \ldots, C_s $ est un cône simplicial ouvert ou un simplexe ouvert.

#### Remarque 2 {#lie-v-s3-n9-rem-2 .statement}

Supposons W irréductible et essentiel. Si H et H’ sont deux murs de C, on a $ m_{HH'} = +\infty $ si et seulement si l’on a $ e_H = -e_{H'} $ (prop. 3). D’après les prop. 7 et 8, ceci ne peut se produire que si $ H $ et $ H' $ sont les seuls murs de $ C $ et $ E $ de dimension 1. Le seul cas où l’un des $ m_{HH'} $ est infini est donc celui où $ E $ est de dimension 1 et où le groupe $ W $ est engendré par les réflexions associées à deux points distincts (cf. § 2, no 4).

Dans le cas général, la matrice de Coxeter associée à $ W $ a ses éléments finis, sauf si l’un au moins des $ E_1, \ldots, E_s $ est du type précédent.

### 10. Points spéciaux

Soient $ L $ l’ensemble des translations appartenant à $ W $ et $ \Lambda $ l’ensemble des $ t \in T $ tels que la translation $ x \mapsto t + x $ appartienne à $ L $. Il est immédiat que $ \Lambda $ est stable par $ U(W) $ et que $ L $ est un sous-groupe distingué de $ W $. Comme $ W $ opère proprement dans $ E $, il en est de même de $ L $, et on en déduit facilement que $ \Lambda $ est un sous-groupe discret de $ T $. Pour tout point $ x $ de $ E $, on notera $ W_x $ le stabilisateur de $ x $ dans $ W $.

#### Proposition 9 {#lie-v-s3-prop-9 .statement}

Soit $ a \in E $. Les conditions suivantes sont équivalentes :

(i) On $ a $ $ W = W_a . L $;
(ii) La restriction de l’homomorphisme $ U $ à $ W_a $ est un isomorphisme de $ W_a $ sur $ U(W) $;
(iii) Pour tout hyperplan $ H \in \mathfrak{S} $, il existe un hyperplan $ H' \in \mathfrak{S} $ parallèle à $ H $ et tel que $ a \in H' $.

Il est clair que (i) $ \iff $ (ii), puisque $ L $ est le noyau de $ U $ et que $ L \cap W_a = \{1\} $.

Admettons (i) et soit $ H \in \mathfrak{S} $; on a $ s_H \in W_a . L $ et il existe donc un vecteur $ t \in \Lambda $ tel que $ a = s_H(a) + t $; le vecteur $ t $ est orthogonal à $ H $, et si $ H' = H + \frac{1}{2} t $ on a $ s_{H'}(x) = s_H(x) + t $ pour tout $ x \in E $ (cf. § 2, no 4, prop. 5). Comme on a $ t \in \Lambda $ et $ s_H \in W $, on a $ s_{H'} \in W $, d’où $ H' \in \mathfrak{S} $; on a aussi $ a = s_{H'}(a) $, d’où $ a \in H' $. Donc (i) implique (iii).

Admettons (iii). Soit $ H \in \mathfrak{S} $; prenons $ H' $ comme dans (iii). Alors $ s_{H'}(a) = a $, d’où $ s_{H'} \in W_a $; comme $ H $ est parallèle à $ H' $, l’élément $ w = s_{H'} s_H $ de $ W $ est une translation (\$ 2, no 4, prop. 5), d’où $ w \in L $; on a alors $ s_H = s_{H'} w \in W_a . L $. Comme $ W $ est engendré par la famille $ (s_H)_{H \in \mathfrak{S}} $, on a donc $ W = W_a . L $ et (iii) implique (i).

#### Définition 1 {#lie-v-s3-def-1 .statement}

On dit qu’un point $ a $ de $ E $ est spécial pour $ W $ s’il satisfait aux conditions équivalentes de la prop. 9.

Il est clair que l’ensemble des points spéciaux de $ E $ est stable par $ W $.

#### Proposition 10 {#lie-v-s3-prop-10 .statement}

Il existe un point spécial pour $ W $.

D’après la prop. 6 du no 8, on peut se limiter au cas où $ W $ est essentiel.

Le groupe $ U(W) $ d’automorphismes de $ T $ est fini (cf. no 6, th. 3) et $ U(s_H) $ est une réflexion orthogonale pour tout hyperplan $ H $; de plus, $ U(W) $ est engendré par la famille $(U(s_H))_{H \in \mathfrak{S}}$. D’après la prop. 7 du n° 9, il existe une base $(e_i)_{i \in I}$ de $T$ telle que le groupe $U(W)$ soit engendré par l’ensemble des réflexions $(s_i)_{i \in I}$ définies par
$$
s_i(t) = t - 2(t|e_i) \cdot e_i.
$$
Le cor. du th. 1 du n° 2 montre que toute réflexion $s \in U(W)$ est de la forme $s = U(s_H)$ avec $H \in \mathfrak{S}$. On peut donc trouver dans $\mathfrak{S}$ une famille d’hyperplans $(H_i)_{i \in I}$ tels que $s_i = U(s_{H_i})$ pour tout $i$. Comme les vecteurs $e_i$ sont linéairement indépendants, il existe $a \in E$ tel que $a \in H_i$ pour tout $i \in I$. On a $s_{H_i} \in W_a$, d’où $U(W) = U(W_a)$, c’est-à-dire $W = W_a$. L puisque $L$ est le noyau de $U$. Donc $a$ est spécial.

Lorsque $W$ est fini essentiel, il n’y a qu’un seul point spécial pour $W$, à savoir l’unique point invariant par $W$. La considération des points spéciaux est donc surtout intéressante quand $W$ est infini.

#### Proposition 11 {#lie-v-s3-prop-11 .statement}

*Supposons $W$ essentiel. Soit $a$ un point spécial pour $W$. Les chambres relatives à $W_a$ sont des cônes simpliciaux ouverts de sommet $a$. Pour toute chambre $C'$ relative à $W_a$ il existe une chambre $C$ et une seule relative à $W$, contenue dans $C'$, et telle que $a \in \overline{C}$. La réunion des $w'(\overline{C})$ pour $w' \in W_a$ est un voisinage fermé de $a$ dans $E$. Tout mur de $C'$ est un mur de $C$. Si $W$ est infini irréductible, les murs de $C$ sont les murs de $C'$ et un hyperplan affine non parallèle aux murs de $C$.

Soit $\mathfrak{S}'$ l’ensemble des $H \in \mathfrak{S}$ qui contiennent $a$. Le groupe $W_a$ est engendré par les $s_H$ pour $H \in \mathfrak{S}'$ (n° 3, prop. 2). Les chambres relatives à $W_a$ sont des cônes simpliciaux ouverts de sommet $a$ (n° 9, prop. 7). Soit $C'$ une telle chambre et soit $U$ une boule ouverte non vide de centre $a$ ne rencontrant aucun élément de $\mathfrak{S} - \mathfrak{S}'$. Comme $a \in \overline{C'}$, il existe $b$ dans $U \cap C'$. On a $b \notin H$ pour tout $H \in \mathfrak{S}$, donc $b$ appartient à une chambre $C$ relative à $\mathfrak{S}$. Comme on a $\mathfrak{S}' \subset \mathfrak{S}$, on a $C \subset C'$. L’ensemble $U \cap C'$ ne rencontre aucun $H \in \mathfrak{S}$ et est convexe, donc $U \cap C' \subset C$; on a donc $a \in \overline{C}$. Inversement, soit $C_1$ une chambre relative à $W$ contenue dans $C'$ et telle que $a \in \overline{C_1}$; alors $C_1$ rencontre $U$, et on a $U \cap C_1 \subset U \cap C' = U \cap C$; les chambres $C$ et $C_1$, ayant un point commun, coïncident. Pour tout $w' \in W_a$, on a $w'(U) = U$, donc
$$
U \cap w'(C) = w'(U \cap C) = w'(U \cap C') = U \cap w'(C');
$$
comme la réunion des $w'(C')$ pour $w' \in W_a$ est dense dans $E$, la réunion des $U \cap w'(C') = U \cap w'(C)$ est dense dans $U$, et la réunion des $w'(\overline{C})$ pour $w' \in W_a$ contient donc $U$. Enfin, si $H$ est un mur de $C'$, il existe un point $c \in U \cap H$ et un voisinage ouvert $V \subset U$ de $c$ tel que $V \cap C'$ soit l’intersection de $V$ et du demi-espace ouvert déterminé par $H$ contenant $C'$; comme $V \cap C' = V \cap U \cap C' = V \cap U \cap C = V \cap C$, on voit que $H$ est un mur de $C$. Si $W$ est infini irréductible, $C$ est un simplexe ouvert (n° 9, prop. 8), donc admet un mur de plus que le cône simplicial ouvert $C'$.

#### Corollaire {#lie-v-s3-n10-cor-1 .statement}

Supposons W essentiel.
    (i) Si $ a \in E $ est spécial, il existe une chambre $ C $ telle que $ a $ soit un point extrémal de $ \overline{C} $.
    (ii) Si $ C $ est une chambre, il existe un point extrémal de $ \overline{C} $ qui est spécial.
La première assertion résulte de la prop. 11. La seconde résulte de la première et du fait que W opère transitivement sur l’ensemble des chambres.

Par contre, un point extrémal de $ \overline{C} $ n’est pas nécessairement un point spécial pour W (cf. chap. VI, planche X, systèmes $ B_2 $ et $ G_2 $).

Remarque 1). — Supposons W essentiel, irréductible et infini et gardons les notations de la prop. 11. Puisque $ U $ est un isomorphisme de $ W_a $ sur $ U(W) $, on voit que le graphe de Coxeter du groupe de déplacements $ U(W) $ (qui est engendré par les réflexions $ U(s_H) $ pour $ H \in \mathfrak{g} $) s’obtient à partir du graphe de Coxeter de W en supprimant le sommet $ i $ correspondant à l’unique mur de $ C $ qui n’est pas un mur de $ C' $.

#### Proposition 12 {#lie-v-s3-prop-12 .statement}

Supposons W essentiel. Soit $ a $ un point spécial, soit $ L(a) $ l’ensemble de ses transformés par le groupe de translations $ L $, et soit $ C $ une chambre. Alors $ \overline{C} $ rencontre $ L(a) $ en un point et un seul; ce point est point extrémal de $ \overline{C} $.

Il existe une chambre $ C_1 $ telle que $ a $ soit point extrémal de $ \overline{C}_1 $ (cor. de la prop. 11). Toute chambre est de la forme $ C = tw'(C_1) $ avec $ w' \in W_a $ et $ t \in L $ puisque $ W = W_a . L $; alors $ \overline{C} $ admet le point extrémal $ tw'(a) = t(a) \in L(a) $. D’autre part, $ \overline{C} $ ne peut contenir deux points distincts de $ L(a) $ puisque $ \overline{C} $ est un domaine fondamental pour W (n° 3, th. 2).

Remarque 2). — L’ensemble $ L(a) $ est contenu dans l’ensemble des points spéciaux. Il en est en général distinct (cf. chap. VI, § 2, n° 2 et planches I à VI).

## EXERCICES {#lie-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
