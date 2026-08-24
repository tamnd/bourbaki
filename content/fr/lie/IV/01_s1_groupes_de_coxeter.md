---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: Groupes de Coxeter et systèmes de Tits
section: 1
section_title: Groupes de Coxeter
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0008-0021, 0036-0044
extraction: ocr
subsections:
    - "no": 1
      title: Longueur et décompositions réduites
      page: 0
      pdf_page: 8
    - "no": 2
      title: Groupes diédraux
      page: 0
      pdf_page: 9
    - "no": 3
      title: Premières propriétés des groupes de Coxeter
      page: 0
      pdf_page: 10
    - "no": 4
      title: Décompositions réduites dans un groupe de Coxeter
      page: 0
      pdf_page: 12
    - "no": 5
      title: La condition d’échange
      page: 0
      pdf_page: 14
    - "no": 6
      title: Caractérisation des groupes de Coxeter
      page: 0
      pdf_page: 16
    - "no": 7
      title: Familles de partitions
      page: 0
      pdf_page: 17
    - "no": 8
      title: Sous-groupes des groupes de Coxeter
      page: 0
      pdf_page: 18
    - "no": 9
      title: Matrices et graphes de Coxeter
      page: 0
      pdf_page: 19
statements: 31
exercises: 12
content_sha256: 62478063b83420b4cdd00b735467dd0009810dd7f46789b3df50f13fe9be97d3
---

## § 1. Groupes de Coxeter

Dans tout ce paragraphe, on désigne par W un groupe, noté multiplicativement, d’élément neutre 1, et par S un sous-ensemble générateur de W tel que S = S^{-1} et 1 \notin S. Tout élément de W est produit d’une suite finie d’éléments de S. À partir du n° 3, on suppose que tout élément de S est d’ordre 2.

### 1. Longueur et décompositions réduites

#### Définition 1 {#lie-iv-s1-def-1 .statement}

Soit w \in W. On appelle longueur de w (par rapport à S), et l’on note l_S(w) ou simplement l(w), le plus petit entier q \geq 0 tel que w soit produit d’une suite de q éléments de S. On appelle décomposition réduite de w (par rapport à S) toute suite s = (s_1, \ldots, s_q) d’éléments de S telle que w = s_1 \ldots s_q et q = l(w).

Ainsi 1 est l’unique élément de longueur 0 et S se compose des éléments de longueur 1.

#### Proposition 1 {#lie-iv-s1-prop-1 .statement}

Soient w et w' dans W. On a les formules:

(1) \quad l(ww') \leq l(w) + l(w')
(2) \quad l(w^{-1}) = l(w)
(3) \quad |l(w) - l(w')| \leq l(ww'^{-1}).

Soient (s_1, \ldots, s_p) et (s'_1, \ldots, s'_q) des décompositions réduites de w et w' respectivement; on a donc l(w) = p et l(w') = q, et comme on a ww' = s_1 \ldots s_p s'_1 \ldots s'_q, on a l(ww') \leq p + q, d’où (1). Comme S = S^{-1} et w^{-1} = s_p^{-1} \ldots s_1^{-1}, on a l(w^{-1}) \leq p = l(w); remplaçant w par w^{-1}, on obtient l’inégalité opposée l(w) \leq l(w^{-1}), d’où (2). Remplaçant w par ww'^{-1} dans (1) et (2), on obtient les relations:

(4) \quad l(w) - l(w') \leq l(ww'^{-1}),
(5) \quad l(ww'^{-1}) = l(w'w^{-1});

en échangeant w et w' dans (4), on obtient l(w') - l(w) \leq l(ww'^{-1}) d’après (5), d’où (3).

#### Corollaire {#lie-iv-s1-n1-cor-1 .statement}

Soient s = (s_1, \ldots, s_p) et s' = (s'_1, \ldots, s'_q) deux suites d’éléments de S telles que w = s_1 \ldots s_p et w' = s'_1 \ldots s'_q. Si la suite (s_1, \ldots, s_p, s'_1, \ldots, s'_q) est une décomposition réduite de $ w w' $, alors $ s $ est une décomposition réduite de $ w $ et $ s' $ en est une de $ w' $.

Par hypothèse, on a $ l(w) \leq p $, $ l(w') \leq q $ et $ l(w w') = p + q $. D’après (1), on a donc $ l(w) = p $ et $ l(w') = q $, d’où le corollaire.

#### Remarque {#lie-iv-s1-n1-rem-1 .statement}

La formule $ d(w, w') = l(w w'^{-1}) $ définit une distance $ d $ sur $ W $, invariante par les translations à droite, en vertu des formules (1) et (2).

### 2. Groupes diédraux

#### Définition 2 {#lie-iv-s1-def-2 .statement}

On appelle groupe diédral tout groupe engendré par deux éléments d’ordre 2, distincts.

#### Exemple {#lie-iv-s1-n2-exa-1 .statement}

Soit $ M $ le groupe multiplicatif $ \{1, -1\} $, et soit $ m $ un entier $ \geq 2 $ (resp. $ m = \infty $). On fait opérer $ M $ sur le groupe $ \mathbf{Z}/m\mathbf{Z} $ (resp. sur $ \mathbf{Z} $) par $ (-1) \cdot x = -x $, et l’on note $ D_m $ le produit semi-direct correspondant de $ M $ par $ \mathbf{Z}/m\mathbf{Z} $ (resp. de $ M $ par $ \mathbf{Z} $). Les éléments de $ D_m $ sont donc les couples $ (\varepsilon, x) $ avec $ \varepsilon = \pm 1 $ et $ x \in \mathbf{Z}/m\mathbf{Z} $ (resp. $ x \in \mathbf{Z} $); la loi de groupe dans $ D_m $ est donnée par la formule:

$$
(\varepsilon, x) \cdot (\varepsilon', x') = (\varepsilon \varepsilon', \varepsilon' x + x').
$$

On note $ t $ la classe de 1 modulo $ m $ (resp. $ t = 1 $) et l’on pose

$$
\rho = (-1, 0), \quad \rho' = (-1, t), \quad \pi = (1, t);
$$

on a alors $ \rho^2 = \rho'^2 = 1 $ et $ \pi = \rho \rho' $. Les formules

$$
\pi^n = (1, n t), \quad \rho \pi^n = (-1, n t)
$$

montrent que $ D_m $ est un groupe diédral engendré par $ \{\rho, \rho'\} $.

#### Proposition 2 {#lie-iv-s1-prop-2 .statement}

On suppose que $ S $ se compose de deux éléments distincts $ s $ et $ s' $ d’ordre 2.

(i) Le sous-groupe $ P $ de $ W $ engendré par $ p = ss' $ est distingué, et $ W $ est produit semi-direct du sous-groupe $ T = \{1, s\} $ et de $ P $. De plus, on a $ (W : P) = 2 $.

(ii) Soit $ m $ l’ordre (fini ou non) de $ p $. On a $ m \geq 2 $ et $ W $ est d’ordre $ 2m $. Il existe un unique isomorphisme $ \varphi $ de $ D_m $ sur $ W $ tel que $ \varphi(\rho) = s $ et $ \varphi(\rho') = s' $.

(i) On a $ sps^{-1} = sss's = s's = p^{-1} $, d’où

$$
sp^n s^{-1} = p^{-n}
$$

pour tout entier $ n $. Comme $ W $ est engendré par $ \{s, s'\} $, donc par $ \{s, p\} $, le sous-groupe $ P $ de $ W $ est distingué. Par suite, TP est un sous-groupe de $ W $; comme TP contient $ s $ et $ s' = sp $, on a donc $ W = TP = P \cup sP $. Pour prouver (i), il suffit donc de montrer que l’on a $ W \neq P $. Si l’on avait $ W = P $, le groupe $ W $ serait commutatif, d’où $ p^2 = s^2 s'^2 = 1 $; les seuls éléments de $ W = P $ seraient 1 n° 1.3.

et $ p $, contrairement à l’hypothèse que $ W $ contient au moins trois éléments, à savoir $ 1, s $ et $ s' $.

(ii) Comme on a $ s \neq s' $, on a $ p \neq 1 $, d’où $ m \geq 2 $. Comme $ P $ est d’ordre $ m $ et que l’on a $ (W : P) = 2 $, l’ordre de $ W $ est $ 2m $. Si $ m $ est fini (resp. infini), il existe un isomorphisme $ \varphi' $ de $ \mathbf{Z}/m\mathbf{Z} $ (resp. $ \mathbf{Z} $) sur $ P $ appliquant $ \pi $ sur $ p $; il existe de plus un isomorphisme $ \varphi'' $ de $ M = \{1, -1\} $ sur $ T $ appliquant — 1 sur $ s $. Le groupe $ W $ est produit semi-direct de $ T $ et $ P $; d’après les formules (9) et $ \rho \pi^n \rho^{-1} = \pi^{-n} $, on déduit de $ \varphi' $ et $ \varphi'' $ un isomorphisme $ \varphi $ de $ D_m $ sur $ W $ tel que $ \varphi(\rho) = s $ et $ \varphi(\pi) = p $, d’où $ \varphi(\rho') = s' $. L’unicité de $ \varphi $ résulte de ce que $ D_m $ est engendré par $ \{\rho, \rho'\} $.

#### Remarque {#lie-iv-s1-n2-rem-1 .statement}

Considérons un groupe diédral $ W $ d’ordre $ 2m $, engendré par deux éléments distincts $ s $ et $ s' $ d’ordre 2. Désignons par $ s_q $ (resp. $ s'_q $) la suite de longueur $ q $ dont les termes de rang impair (resp. pair) sont égaux à $ s $ et les termes de rang pair (resp. impair) à $ s' $ et soit $ w_q $ (resp. $ w'_q $) le produit de la suite $ s_q $ (resp. $ s'_q $). On a:

$$
w_{2k} = (ss')^k, \quad w_{2k+1} = (ss')^k s \\
w'_{2k} = (s's)^k = (ss')^{-k}, \quad w'_{2k+1} = (s's)^k s' = (ss')^{-k-1}s.
$$

Si $ s = (s_1, \ldots, s_q) $ est une décomposition réduite (par rapport à $ \{s, s'\} $) d’un élément $ w $ de $ W $, on a évidemment $ s_i \neq s_{i+1} $ pour $ 1 \leq i \leq q-1 $. Par suite, on a $ s = s_q $ ou $ s = s'_q $.

Si $ m = \infty $, les éléments $ (ss')^n $ et $ (ss')^n s $ pour $ n \in \mathbf{Z} $ sont distincts. Par suite, les éléments $ w_q $ ($ q \geq 0 $) et $ w'_q $ ($ q > 0 $) sont distincts et si $ s $ est une décomposition réduite de $ w_q $ (resp. $ w'_q $), on a nécessairement $ s = s_q $ (resp. $ s = s'_q $). Il en résulte que $ l(w_q) = l(w'_q) = q $ et que l’ensemble des décompositions réduites d’éléments de $ W $ est l’ensemble des $ s_q $ et des $ s'_q $. De plus, tout élément de $ W $ possède une seule décomposition réduite.

Supposons maintenant $ m $ fini. Si $ q \geq 2m $, on a $ w_q = w_{q-2m} $ et $ w'_q = w'_{q-2m} $; si $ m \leq q \leq 2m $, on a $ w_q = w'_{2m-q} $, $ w'_q = w_{2m-q} $. Par suite, ni $ s_q $ ni $ s'_q $ ne sont des décompositions réduites dès que $ q > m $. On en déduit que chacun des $ 2m $ éléments de $ W $ est l’un des $ 2m $ éléments $ w_0 = w'_0, w_q $ et $ w'_q $ pour $ 1 \leq q \leq m-1 $ et $ w_m = w'_m $. Ces $ 2m $ éléments sont donc distincts et il en résulte comme plus haut que $ l(w_q) = l(w'_q) = q $ pour $ q \leq m $ et que l’ensemble des décompositions réduites d’éléments de $ W $ est l’ensemble des $ s_q $ et des $ s'_q $ pour $ 0 \leq q \leq m $. Tout élément de $ W $ distinct de $ w_m $ possède une seule décomposition réduite; $ w_m $ en possède deux.

### 3. Premières propriétés des groupes de Coxeter

Rappelons qu’à partir de maintenant, on suppose que les éléments de $ S $ sont d’ordre 2.

#### Définition 3 {#lie-iv-s1-def-3 .statement}

On dit que $ (W, S) $ est un système de Coxeter s’il satisfait à la condition suivante :

(C) Pour $ s, s' $ dans $ S $, soit $ m(s, s') $ l’ordre de $ ss' $; soit $ I $ l’ensemble des couples $ (s, s') $ tels que $ m(s, s') $ soit fini. L’ensemble générateur $ S $ et les relations $ (ss')^{m(s,s')} = 1 $ pour $ (s, s') $ dans $ I $ forment une présentation (*) du groupe $ W $.

Lorsque $ (W, S) $ est un système de Coxeter, on dit aussi, par abus de langage, que $ W $ est un groupe de Coxeter.

#### Exemple 1 {#lie-iv-s1-n3-exa-1 .statement}

Soit $ m $ un entier $ \geq 2 $ ou $ \infty $ et soit $ W $ un groupe défini par un ensemble générateur $ S = \{s, s'\} $ et les relations $ s^2 = s'^2 = 1 $ lorsque $ m = \infty $, $ s^2 = s'^2 = (ss')^m = 1 $ lorsque $ m $ est fini. Considérons d’autre part le groupe diédral $ D_m $ (n° 2, Exemple) et les éléments $ \rho $ et $ \rho' $ de $ D_m $ définis par (7). Puisque $ \rho^2 = \rho'^2 = 1 $ et que $ (\rho\rho')^m = 1 $ lorsque $ m $ est fini, il existe un homomorphisme $ f $ et un seul de $ W $ sur $ D_m $ tel que $ f(s) = \rho $ et $ f(s') = \rho' $. Comme $ \rho\rho' $ est d’ordre $ m $, il en résulte que $ ss' $ est lui aussi d’ordre $ m $. Par suite, $ (W, S) $ est un système de Coxeter, $ W $ est un groupe diédral d’ordre $ 2m $ et $ f $ est un isomorphisme (prop. 2).

Par transport de structure, on en déduit que tout groupe diédral est un groupe de Coxeter.

#### Exemple 2 {#lie-iv-s1-n3-exa-2 .statement}

Soit $ \mathfrak{S}_n $ le groupe symétrique de degré $ n $, avec $ n \geq 2 $. Soit $ s_i $ la transposition de $ i $ et $ i+1 $ pour $ 1 \leq i < n $, et soit $ S = \{s_1, \ldots, s_{n-1}\} $. On peut montrer (§ 2, n° 4, Exemple et § 1, exerc. 4) que $ (\mathfrak{S}_n, S) $ est un système de Coxeter.

#### Exemple 3 {#lie-iv-s1-n3-exa-3 .statement}

Pour la classification des groupes de Coxeter finis, cf. Chap. VI, § 4.

#### Remarque {#lie-iv-s1-n3-rem-1 .statement}

Supposons que $ (W, S) $ soit un système de Coxeter. Il existe un homomorphisme $ \varepsilon $ de $ W $ dans le groupe $ \{1, -1\} $ caractérisé par $ \varepsilon(s) = -1 $ pour tous $ s \in S $. On dit que $ \varepsilon(w) $ est la signature de $ w $; elle est égale à $ (-1)^{l(w)} $. La formule $ \varepsilon(ww') = \varepsilon(w) \cdot \varepsilon(w') $ se traduit donc par $ l(ww') \equiv l(w) + l(w') $ mod. 2.

#### Proposition 3 {#lie-iv-s1-prop-3 .statement}

Supposons que $ (W, S) $ soit un système de Coxeter. Pour que deux éléments $ s $ et $ s' $ de $ S $ soient conjugués (***) dans $ W $, il faut et il suffit que la condition suivante soit remplie:
(I) Il existe une suite finie $ (s_1, \ldots, s_q) $ d’éléments de $ S $ telle que $ s_1 = s, s_q = s' $ et que $ s_js_{j+1} $ soit d’ordre fini impair pour $ 1 \leq j < q $.

Soient $ s $ et $ s' $ dans $ S $ tels que $ p = ss' $ soit d’ordre fini $ 2n + 1 $. D’après (9), on a $ sp^{-n} = p^n s $, d’où
$$
p^n s p^{-n} = p^n p^n s = p^{-1} s = s' s s = s',
$$
et $ s' $ est conjugué de $ s $.

Pour tout $ s $ dans $ S $, soit $ A_s $ l’ensemble des $ s' \in S $ satisfaisant à (I). Avec les hypothèses de (I), les éléments $ s_j $ et $ s_{j+1} $ sont conjugués pour $ 1 \leq j < q $ d’après ce qui précède, donc tout élément $ s' $ de $ A_s $ est conjugué de $ s $.

(*) Ceci signifie que $ (W, S) $ satisfait à la propriété universelle suivante: étant donnés un groupe $ G $ et une application $ f $ de $ S $ dans $ G $ telle que $ (f(s)f(s'))^{m(s,s')} = 1 $ pour $ (s, s') $ dans $ I $, il existe un homomorphisme $ g $ de $ W $ dans $ G $ prolongeant $ f $. Cet homomorphisme est unique car $ S $ engendre $ W $. Une forme équivalente de cette définition est la suivante : soient $ \overline{W} $ un groupe, $ f $ un homomorphisme de $ \overline{W} $ sur $ W $ et $ h $ une application de $ S $ dans $ \overline{W} $ telle que $ f(h(s)) = s $ et $ (h(s)h(s'))^{m(s,s')} = 1 $ pour $ (s, s') $ dans $ I $ et que les $ h(s) $ (pour $ s \in I $) engendrent $ \overline{W} $; alors $ f $ est injectif (donc un isomorphisme de $ \overline{W} $ sur $ W $).

(**) Rappelons que deux éléments (resp. deux sous-ensembles) d’un groupe $ W $ sont dits conjugués s’il existe un automorphisme intérieur de $ W $ qui transforme l’un en l’autre.

n° 1.4.

Soit $ f $ l’application de $ S $ dans $ M = \{1, -1\} $ égale à 1 dans $ A_s $ et à — 1 dans $ S - A_s $. Soient $ s' $ et $ s'' $ dans $ S $ tels que $ s's'' $ soit d’ordre fini $ m $; on a $ f(s')f(s'') = 1 $ si $ s' $ et $ s'' $ sont tous deux dans $ A_s $ ou dans $ S - A_s $; dans les autres cas, on a $ f(s')f(s'') = -1 $, mais $ m $ est pair; on a donc $ (f(s')f(s''))^m = 1 $ dans tous les cas. Comme $ (W, S) $ est un système de Coxeter, il existe un homomorphisme $ g $ de $ W $ dans $ M $ induisant $ f $ sur $ S $. Soit $ s' $ un conjugué de $ s $; comme $ s $ appartient au noyau de $ g $, il en est de même de $ s' $, d’où $ f(s') = g(s') = 1 $ et finalement $ s' \in A_s $. C.Q.F.D.

### 4. Décompositions réduites dans un groupe de Coxeter

Supposons que $ (W, S) $ soit un système de Coxeter. Soit $ T $ l’ensemble des conjugués des éléments de $ S $ dans $ W $. Pour toute suite finie $ s = (s_1, \ldots, s_q) $ d’éléments de $ S $, on note $ \Phi(s) $ la suite $ (t_1, \ldots, t_q) $ d’éléments de $ T $ définie par :

$$
t_j = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1} \quad \text{pour } 1 \leq j \leq q.
$$

On a $ t_1 = s_1 $ et $ s_1 \ldots s_q = t_q t_{q-1} \ldots t_1 $. Pour tout élément $ t \in T $, on note $ n(s, t) $ le nombre d’entiers $ j $ tels que $ 1 \leq j \leq q $ et $ t_j = t $. Enfin, on pose

$$
R = \{1, -1\} \times T.
$$

#### Lemme 1 {#lie-iv-s1-lem-1 .statement}

(i) *Soient $ w \in W $ et $ t \in T $. Le nombre $ (-1)^{n(s, t)} $ a la même valeur $ \eta(w, t) $ pour toutes les suites $ s = (s_1, \ldots, s_q) $ d’éléments de $ S $ telles que $ w = s_1 \ldots s_q $.*

(ii) *Pour $ w \in W $, soit $ U_w $ l’application de $ R $ dans lui-même définie par :*

$$
U_w(\varepsilon, t) = (\varepsilon \cdot \eta(w^{-1}, t), wt w^{-1}) \quad (\varepsilon = \pm 1, \ t \in T).
$$

*L’application $ w \mapsto U_w $ est un homomorphisme de $ W $ dans le groupe des permutations de $ R $.*

Pour $ s \in S $, définissons une application $ U_s $ de $ R $ dans lui-même par :

$$
U_s(\varepsilon, t) = (\varepsilon \cdot (-1)^{\delta_{s,t}}, st s^{-1}) \quad (\varepsilon = \pm 1, \ t \in T)
$$

où $ \delta_{s,t} $ est le symbole de Kronecker. On vérifie aussitôt que $ U_s^2 = \mathrm{Id}_R $, ce qui montre que $ U_s $ est une permutation de $ R $.

Soit $ s = (s_1, \ldots, s_q) $ une suite d’éléments de $ S $. Posons $ w = s_q \ldots s_1 $ et $ U_s = U_{s_q} \ldots U_{s_1} $. Nous allons montrer, par récurrence sur $ q $, que l’on a :

$$
U_s(\varepsilon, t) = (\varepsilon \cdot (-1)^{n(s, t)}, wt w^{-1}).
$$

C’est évident pour $ q = 0, 1 $. Si $ q > 1 $, posons $ s' = (s_1, \ldots, s_{q-1}) $ et

$$
w' = s_{q-1} \ldots s_1.
$$

En utilisant l’hypothèse de récurrence, on obtient :

$$
U_s(\varepsilon, t) = U_{s_q}(\varepsilon \cdot (-1)^{n(s', t)}, w't w'^{-1})
= (\varepsilon \cdot (-1)^{n(s', t) + \delta_{s_q, w't w'^{-1}}}, wt w^{-1})
$$

Or $ \Phi(s) = (\Phi(s'), w'^{-1}s_qw') $ et $ n(s, t) = n(s', t) + \delta_{w'^{-1}s_qw', t} $ d’où la formule (14).

Soient alors $ s, s' \in S $, tels que $ p = ss' $ soit d’ordre fini $ m $. Soit $ s = (s_1, \ldots, s_{2m}) $ la suite d’éléments de $ S $ définie par $ s_j = s $ pour $ j $ impair et $ s_j = s' $ pour $ j $ pair. On a $ s_{2m} \ldots s_1 = p^{-m} = 1 $ et la formule (11) entraîne :

$$
t_j = p^{j-1}s \quad \text{pour } 1 \leq j \leq 2m.
$$

Comme $ p $ est d’ordre $ m $, les éléments $ t_1, \ldots, t_m $ sont distincts et l’on a $ t_{j+m} = t_j $ pour $ 1 \leq j \leq m $. Pour tout $ t \in T $, l’entier $ n(s, t) $ est donc égal à 0 ou à 2 et (14) montre que $ U_s = \mathrm{Id}_R $. Autrement dit, on a $ (U_s U_{s'})^m = \mathrm{Id}_R $. D’après la définition même des systèmes de Coxeter, il existe donc un homomorphisme $ w \mapsto U_w $ de $ W $ dans le groupe des permutations de $ R $ tel que $ U_s $ soit donné par le second membre de (13). On a alors $ U_w = U_s $ pour toute suite $ s = (s_1, \ldots, s_q) $ telle que $ w = s_q \ldots s_1 $ et le lemme 1 résulte immédiatement de (14).

#### Lemme 2 {#lie-iv-s1-lem-2 .statement}

*Soient $ s = (s_1, \ldots, s_q) $, $ \Phi(s) = (t_1, \ldots, t_q) $ et $ w = s_1 \ldots s_q $. Soit $ T_w $ l’ensemble des éléments $ t \in T $ tels que $ \eta(w, t) = -1 $. Pour que $ s $ soit une décomposition réduite de $ w $, il faut et il suffit que les $ t_i $ soient distincts; on a alors $ T_w = \{t_1, \ldots, t_q\} $ et $ \mathrm{Card}(T_w) = l(w) $.*

On a évidemment $ T_w \subset \{t_1, \ldots, t_q\} $; en prenant $ s $ réduite, on en déduit d’abord que $ \mathrm{Card}(T_w) \leq l(w) $. De plus, si les $ t_i $ sont distincts, $ n(s, t) $ est égal à 1 ou 0 suivant que $ t $ appartient ou non à $ \{t_1, \ldots, t_q\} $. D’où $ T_w = \{t_1, \ldots, t_q\} $ et $ q = \mathrm{Card}(T_w) \leq l(w) $, ce qui entraîne que $ s $ est réduite. Supposons enfin que l’on ait $ t_i = t_j $ avec $ i < j $. On en tire $ s_i = us_ju^{-1} $, avec $ u = s_{i+1} \ldots s_{j-1} $, d’où aussitôt

$$
w = s_1 \ldots s_{i-1} s_{i+1} \ldots s_{j-1} s_{j+1} \ldots s_q,
$$

ce qui montre que $ s $ n’est pas une décomposition réduite de $ w $.

#### Lemme 3 {#lie-iv-s1-lem-3 .statement}

*Soient $ w \in W $ et $ s \in S $ tels que $ l(sw) \leq l(w) $. Pour toute suite $ s = (s_1, \ldots, s_q) $ d’éléments de $ S $ avec $ w = s_1 \ldots s_q $, il existe un entier $ j $ tel que $ 1 \leq j \leq q $ et

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

Soient $ p $ la longueur de $ w $ et $ w' = sw $. D’après la *Remarque* du no 3, on a $ l(w') \equiv l(w) + 1 $ mod. 2; l’hypothèse $ l(w') \leq l(w) $ et la relation

$$
|l(w) - l(w')| \leq l(ww'^{-1}) = l(s) = 1
$$

entraînent $ l(w') = p - 1 $. Choisissons une décomposition réduite

$$
(s'_1, \ldots, s'_{p-1})
$$

n° 1.5.

de $ w' $ et posons $ s' = (s, s'_1, \ldots, s'_{p-1}) $ et $ \Phi(s') = (t'_1, \ldots, t'_p) $. Il est clair que $ s' $ est une décomposition réduite de $ w $ et que l’on a $ t'_1 = s $; les éléments $ t'_1, \ldots, t'_p $ étant distincts par le lemme 2, on a $ n(s', s) = 1 $. Comme $ w $ est le produit de la suite $ s $, on a $ n(s, s) \equiv n(s', s) $ mod. 2 d’après le lemme 1, d’où $ n(s, s) \neq 0 $; par suite, $ s $ est égal à l’un des éléments $ t_j $ de la suite $ \Phi(s) $, d’où le lemme.

#### Remarque {#lie-iv-s1-n4-rem-1 .statement}

L’ensemble $ T_w $ défini au lemme 2 se compose des éléments de la forme $ w''sw''^{-1} $ correspondant aux triplets $ (w', w'', s) \in W \times W \times S $ tels que $ w = w''sw' $ et $ l(w') + l(w'') + 1 = l(w) $.

### 5. La condition d’échange

On désigne sous le nom de « condition d’échange » l’assertion suivante sur $ (W, S) $:

(E). Soient $ w \in W $ et $ s \in S $ tels que $ l(sw) \leq l(w) $. Pour toute décomposition réduite $ (s_1, \ldots, s_q) $ de $ w $, il existe un entier $ j $ tel que $ 1 \leq j \leq q $ et

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1}s_j.
$$

On suppose dans ce numéro que $ (W, S) $ satisfait à (E); d’après le lemme 3, il en est ainsi si $ (W, S) $ est un système de Coxeter. Les résultats de ce numéro s’appliquent donc aux systèmes de Coxeter.

#### Proposition 4 {#lie-iv-s1-prop-4 .statement}

Soient $ s \in S $, $ w \in W $ et $ s = (s_1, \ldots, s_q) $ une décomposition réduite de $ w $. Deux cas seulement sont possibles:

a) $ l(sw) = l(w) + 1 $ et $ (s, s_1, \ldots, s_q) $ est une décomposition réduite de $ sw $.
b) $ l(sw) = l(w) - 1 $ et il existe un entier $ j $ tel que $ 1 \leq j \leq q $, que

$$
(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)
$$

soit une décomposition réduite de $ sw $ et que la suite $ (s, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q) $ soit une décomposition réduite de $ w $.

Posons $ w' = sw $; d’après la formule (3) du n° 1, on a

$$
|l(w) - l(w')| \leq l(s) = 1.
$$

Nous distinguerons deux cas:

a) $ l(w') > l(w) $. On a donc $ l(w') = q + 1 $ et $ w' = ss_1 \ldots s_q $, donc

$$
(s, s_1, \ldots, s_q)
$$

est une décomposition réduite de $ w' $.

b) $ l(w') \leq l(w) $. D’après (E), il existe un entier $ j $ tel que $ 1 \leq j \leq q $, satisfaisant à (16). On a alors $ w = ss_1 \ldots s_{j-1}s_{j+1} \ldots s_q $, d’où

$$
w' = s_1 \ldots s_{j-1}s_{j+1} \ldots s_q;
$$

comme on a $ q - 1 \leq l(w') \leq q $, on a nécessairement $ l(w') = q - 1 $ et $ (s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q) $ est une décomposition réduite de $ w' $.

#### Lemme 4 {#lie-iv-s1-lem-4 .statement}

Soient $ w \in W $ de longueur $ q \geq 1 $, $ D $ l’ensemble des décompositions réduites de $ w $, et $ F $ une application de $ D $ dans un ensemble $ E $. On suppose que l’on a $ F(s) = F(s') $ si les éléments $ s = (s_1, \ldots, s_q) $, $ s' = (s'_1, \ldots, s'_q) $ de $ D $ satisfont à l’une des hypothèses suivantes :

a) On a $ s_1 = s'_1 $ ou $ s_q = s'_q $.

b) Il existe $ s $ et $ s' $ dans $ S $ tels que $ s_j = s'_k = s $ et $ s_k = s'_j = s' $ pour $ j $ impair et $ k $ pair.

Alors $ F $ est constante.

A) Soient $ s, s' \in D $; posons $ t = (s'_1, s_1, \ldots, s_{q-1}) $. Nous allons montrer que si $ F(s) \neq F(s') $, on a $ t \in D $ et $ F(t) \neq F(s) $. On a en effet $ w = s'_1 \ldots s'_q $, donc $ s'_1 w = s'_2 \ldots s'_q $ est de longueur $ < q $. D’après la prop. 4, il existe un entier $ j $ tel que $ 1 \leq j \leq q $ et que la suite $ u = (s'_1, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q) $ appartienne à $ D $. On a $ F(u) = F(s') $ d’après la condition $ a) $; si l’on avait $ j \neq q $, on aurait $ F(s) = F(u) $ pour la même raison, d’où $ F(s) = F(s') $ contrairement à l’hypothèse. On a donc $ j = q $, d’où $ t = u \in D $ et $ F(t) = F(s') \neq F(s) $.

B) Soient $ s $ et $ s' $ dans $ D $. Pour tout entier $ j $ avec $ 0 \leq j \leq q $, définissons une suite $ s_j $ de $ q $ éléments de $ S $ de la manière suivante :

$$
\begin{cases}
s_0 = (s'_1, \ldots, s'_q) \\
s_1 = (s_1, \ldots, s_q) \\
s_{q+1-k} = (s_1, s'_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k) & \text{pour } q - k \text{ pair et } 1 \leq k \leq q \\
s_{q+1-k} = (s'_1, s_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k) & \text{pour } q - k \text{ impair et } 1 \leq k \leq q.
\end{cases}
$$

Notons $ (H_j) $ l’assertion « $ s_j \in D, s_{j+1} \in D $ et $ F(s_j) \neq F(s_{j+1}) $ ». D’après (A), on a $ (H_j) \implies (H_{j+1}) $ pour $ 0 \leq j < q $, et $ (H_q) $ n’est pas satisfaite d’après la condition $ b) $. Par suite, $ (H_0) $ n’est pas satisfaite. Comme $ s_0 = s' $ et $ s_1 = s $, il en résulte que $ F(s) = F(s') $.

#### Proposition 5 {#lie-iv-s1-prop-5 .statement}

Soient $ M $ un monoïde (avec élément unité 1) et $ f $ une application de $ S $ dans $ M $. Pour $ s, s' $ dans $ S $, soit $ m(s, s') $ l’ordre de $ ss' $; on pose

$$
a(s, s') = \begin{cases}
(f(s) f(s'))^l & \text{si } m(s, s') = 2l, \quad l \text{ fini} \\
(f(s) f(s'))^l f(s) & \text{si } m(s, s') = 2l + 1, \quad l \text{ fini} \\
1 & \text{si } m(s, s') = \infty.
\end{cases}
$$

Si l’on a $ a(s, s') = a(s', s) $ quels que soient $ s \neq s' $ dans $ S $, il existe une application $ g $ de $ W $ dans $ M $ telle que

$$
g(w) = f(s_1) \ldots f(s_q)
$$

pour tout $ w \in W $ et toute décomposition réduite $ (s_1, \ldots, s_q) $ de $ w $.

Pour tout $ w \in W $, soient $ D_w $ l’ensemble des décompositions réduites de $ w $ et $ F_w $ l’application de $ D_w $ dans $ M $ définie par

$$
F_w(s_1, \ldots, s_q) = f(s_1) \ldots f(s_q).
$$

n° 1.6.

Nous allons prouver par récurrence sur la longueur de $ w $ que $ F_w $ est constante, ce qui établira la prop. 5. Les cas $ l(w) = 0, 1 $ étant triviaux, nous supposons $ q \geq 2 $ et notre assertion prouvée pour les éléments $ w $ avec $ l(w) < q $. Soient $ w $ de longueur $ q $ et $ s, s' $ dans $ D_w $; d’après le lemme 4, il suffit de prouver que l’on a $ F_w(s) = F_w(s') $ dans les cas $ a) $ et $ b) $ dudit lemme.

$ a) $ La formule

$$
F_w(s_1, \ldots, s_q) = f(s_1) F_{w''}(s_2, \ldots, s_q) = F_{w'}(s_1, \ldots, s_{q-1}) f(s_q)
$$

pour $ w' = s_1 \ldots s_{q-1} $ et $ w'' = s_2 \ldots s_q $ et l’hypothèse de récurrence montrent que l’on a $ F_w(s) = F_w(s') $ si $ s_1 = s'_1 $ ou $ s_q = s'_q $.

$ b) $ Supposons qu’il existe deux éléments $ s $ et $ s' $ de $ S $ tels que $ s_j = s'_k = s $ et $ s_k = s'_j = s' $ pour $ j $ impair et $ k $ pair. Il suffit de traiter le cas $ s \neq s' $. Les suites $ s $ et $ s' $ sont alors deux décompositions réduites distinctes de $ w $ dans le groupe diédral engendré par $ s $ et $ s' $. D’après la Remarque du n° 2, l’ordre $ m $ de $ ss' $ est nécessairement fini et l’on a, avec les notations de cette remarque, $ s = s_m $ et $ s' = s'_m $. Par suite, on a $ F_w(s) = a(s, s') $ et $ F_w(s') = a(s', s) $, d’où

$$
F_w(s) = F_w(s').
$$

### 6. Caractérisation des groupes de Coxeter

#### Théorème 1 {#lie-iv-s1-thm-1 .statement}

Pour que $ (W, S) $ soit un système de Coxeter, il faut et il suffit qu’il satisfasse à la condition d’échange (E) du n° 5.

Le lemme 3 du n° 4 montre que tout système de Coxeter satisfait à (E).

Réciproquement, supposons (E) vérifiée. Soient $ G $ un groupe et $ f $ une application de $ S $ dans $ G $, telle que l’on ait $ |(f(s)f(s'))|^m = 1 $ chaque fois que $ s $ et $ s' $ appartiennent à $ S $ et que $ ss' $ est d’ordre fini $ m $. D’après la prop. 5, il existe alors une application $ g $ de $ W $ dans $ G $ telle que l’on ait:

$$
g(w) = f(s_1) \cdots f(s_q)
$$

chaque fois que $ w = s_1 \ldots s_q $ est de longueur $ q $. Pour prouver que $ (W, S) $ est un système de Coxeter, il suffit de prouver que $ g $ est un homomorphisme, ce qui est conséquence de la formule

$$
g(sw) = f(s)g(w) \quad \text{pour } s \in S, \; w \in W
$$

puisque $ S $ engendre $ W $. D’après la prop. 4 du n° 5, deux cas seulement sont possibles :

$ a) $ $ l(sw) = l(w) + 1 $: si $ (s_1, \ldots, s_q) $ est une décomposition réduite de $ w $, alors $ (s, s_1, \ldots, s_q) $ est une décomposition réduite de $ sw $, d’où (21).

$ b) $ $ l(sw) = l(w) - 1 $: posons $ w' = sw $; on a $ w = sw' $ et $ l(sw') = l(w') + 1 $. D’après $ a) $, on a donc $ g(w) = f(s)g(sw) $, d’où $ f(s)g(w) = g(sw) $ puisque l’on a $ (f(s))^2 = 1 $.

### 7. Familles de partitions

Supposons que (W, S) soit un système de Coxeter. Pour tout s dans S, notons P_s l’ensemble des éléments w de W tels que $ l(sw) > l(w) $. On a les propriétés suivantes :

(A) *On a* $ \bigcap_{s \in S} P_s = \{1\} $.

En effet, soit $ w \neq 1 $ dans W et soit $ (s_1, \ldots, s_q) $ une décomposition réduite de w. On a $ q \geq 1 $, et $ (s_2, \ldots, s_q) $ est une décomposition réduite de $ s_1w $, d’où $ l(w) = q $ et $ l(s_1w) = q - 1 $. On a donc $ w \notin P_{s_1} $.

(B) *Pour tout s dans S, les ensembles* $ P_s $ *et* $ sP_s $ *forment une partition de W*.

Soient $ w \in W $ et $ s \in S $. D’après la prop. 4 du n° 5, on doit distinguer deux cas :
a) $ l(sw) = l(w) + 1 $: on a alors $ w \in P_s $.
b) $ l(sw) = l(w) - 1 $: posons $ w' = sw $ d’où $ w = sw' $; on a alors
$$
l(w') < l(sw')
$$
d’où $ w' \in P_s $, c’est-à-dire $ w \in sP_s $.

(C) *Soient s, s' dans S et w dans W. Si l’on a* $ w \in P_s $ *et* $ ws' \notin P_s $, *on a* $ sw = ws' $.

Soit q la longueur de w. De $ w \in P_s $, on déduit $ l(sw) = q + 1 $; de $ ws' \notin P_s $, on déduit $ l(sws') = l(ws') - 1 \leq q $ et comme on a $ l(sws') = l(sw) \pm 1 $, on a finalement $ l(ws') = q + 1 $ et $ l(sws') = q $.

Soient $ (s_1, \ldots, s_q) $ une décomposition réduite de w et $ s_{q+1} = s' $; alors $ (s_1, \ldots, s_q, s_{q+1}) $ est une décomposition réduite de l’élément $ ws' $ de longueur $ q + 1 $. D’après la condition d’échange, il existe un entier j avec $ 1 \leq j \leq q + 1 $ tel que
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_j.
$$
Si l’on avait $ 1 \leq j \leq q $, on aurait $ sw = s_1 \ldots s_{j-1}s_{j+1} \ldots s_q $ contrairement à la formule $ l(sw) = q + 1 $. On a donc $ j = q + 1 $, et la formule (22) s’écrit alors $ sw = ws' $.

Réciproquement, on a le résultat suivant :

#### Proposition 6 {#lie-iv-s1-prop-6 .statement}

*Soit* $ (P_s)_{s \in S} $ *une famille de parties de* W *satisfaisant à* (C) *et aux conditions suivantes* :

(A') *On a* $ 1 \in P_s $ *pour tout* $ s \in S $.
(B') *Les ensembles* $ P_s $ *et* $ sP_s $ *sont disjoints pour tout* $ s \in S $.
Alors, (W, S) est un système de Coxeter et $ P_s $ se compose des éléments w de W tels que $ l(sw) > l(w) $.

Soient $ s \in S $ et $ w \in W $. De deux choses l’une :
a) $ w \notin P_s $. Soient $ (s_1, \ldots, s_q) $ une décomposition réduite de w et
$$
w_f = s_1 \ldots s_f
$$

n° 1.8.

pour $ 1 \leq j \leq q $; on pose aussi $ w_0 = 1 $. Comme on a $ w_0 \in P_s $ d’après (A’) et que $ w = w_q $ n’est pas dans $ P_s $, il existe un entier $ j $ avec $ 1 \leq j \leq q $ tel que $ w_{j-1} \in P_s $ et que $ w_j = w_{j-1}s_j $ n’appartienne pas à $ P_s $. D’après (C), on a donc

$$
sw_{j-1} = w_{j-1}s_j.
$$

On a donc prouvé la formule

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1}s_j
$$

qui entraîne $ sw = s_1 \ldots s_{j-1}s_{j+1} \ldots s_q $ et $ l(sw) < l(w) $.

$ b) \ w \in P_s : $ posons $ w' = sw $, d’où $ w' \notin P_s $ d’après (B’). D’après $ a) $, on a alors $ l(sw') < l(w') $, c’est-à-dire $ l(w) < l(sw) $.

La comparaison de $ a) $ et $ b) $ prouve que $ P_s $ se compose des $ w \in W $ tels que $ l(sw) > l(w) $. La condition d’échange résulte de ce qui a été vu en $ a) $, donc $ (W, S) $ est un système de Coxeter (th. 1 du n° 6).

### 8. Sous-groupes des groupes de Coxeter

Dans ce numéro, on suppose que $ (W, S) $ est un système de Coxeter. Pour toute partie $ X $ de $ S $, on note $ W_X $ le sous-groupe de $ W $ engendré par $ X $.

#### Proposition 7 {#lie-iv-s1-prop-7 .statement}

*Soit $ w $ dans $ W $. Il existe une partie $ S_w $ de $ S $ telle que l’on ait $ \{s_1, \ldots, s_q\} = S_w $ pour toute décomposition réduite $ (s_1, \ldots, s_q) $ de $ w $.

On note $ M $ le monoïde formé des parties de $ S $ avec la loi de composition $ (A, B) \mapsto A \cup B $; l’élément neutre de $ M $ est $ \varnothing $. On pose $ f(s) = \{s\} $ pour $ s \in S $. Nous allons appliquer la prop. 5 du n° 5 à $ M $ et $ f $; on a $ a(s, s') = \{s, s'\} $ pour $ s, s' $ dans $ S $ si $ m(s, s') $ est fini, et il existe donc une application $ g : w \mapsto S_w $ de $ W $ dans $ M $ telle que $ g(w) = f(s_1) \cup \cdots \cup f(s_q) $, c’est-à-dire $ S_w = \{s_1, \ldots, s_q\} $ pour tout $ w \in W $ et toute décomposition réduite $ (s_1, \ldots, s_q) $ de $ w $.

#### Corollaire 1 {#lie-iv-s1-prop-7-cor-1 .statement}

*Pour toute partie $ X $ de $ S $, le sous-groupe $ W_X $ de $ W $ se compose des éléments $ w $ de $ W $ tels que $ S_w \subset X $.

Si $ w = s_1 \ldots s_q $ avec $ s_1, \ldots, s_q $ dans $ S $, on a $ w^{-1} = s_q \ldots s_1 $; on en déduit

$$
S_{w^{-1}} = S_w.
$$

La prop. 4 du n° 5 montre que l’on a $ S_{sw'} \subset \{s\} \cup S_{w'} $ pour $ s \in S $ et $ w' \in W $, d’où la formule

$$
S_{ww'} \subset S_w \cup S_{w'}
$$

par récurrence sur la longueur de $ w $. D’après (23) et (24), l’ensemble $ U $ des $ w \in W $ tels que $ S_w \subset X $ est un sous-groupe de $ W $; on a $ X \subset U \subset W_X $, d’où $ U = W_X $.

#### Corollaire 2 {#lie-iv-s1-prop-7-cor-2 .statement}

*Pour toute partie $ X $ de $ S $, on a $ W_X \cap S = X $.

Cela résulte du cor. 1 et de la formule $ S_s = \{s\} $ pour $ s $ dans $ S $.

#### Corollaire 3 {#lie-iv-s1-prop-7-cor-3 .statement}

L’ensemble S est un ensemble générateur minimal de W.
Si X ⊂ S engendre W, on a W = W_X, d’où X = S ∩ W_X = S d’après le cor. 2.

#### Corollaire 4 {#lie-iv-s1-prop-7-cor-4 .statement}

Pour toute partie X de S et tout w dans W_X, la longueur de w par rapport à l’ensemble générateur X de W_X est égale à l_S(w).
Soit (s_1, ..., s_q) une décomposition réduite de w considéré comme élément de W; on a w = s_1 ... s_q et s_j ∈ X pour 1 ≤ j ≤ q (cor. 1); par ailleurs, w ne peut être produit de q' < q éléments de X ⊂ S par définition de q = l_S(w).

#### Théorème 2 {#lie-iv-s1-thm-2 .statement}

(i) Pour toute partie X de S, le couple (W_X, X) est un système de Coxeter.
(ii) Soit (X_i)_{i ∈ I} une famille de parties de S. Si X = ⋂_{i ∈ I} X_i, on a W_X = ⋂_{i ∈ I} W_{X_i}.
(iii) Soient X et X' deux parties de S. On a W_X ⊂ W_{X'} (resp. W_X = W_{X'}) si et seulement si l’on a X ⊂ X' (resp. X = X').

Tout élément de X est d’ordre 2 et X engendre W_X. Soient x ∈ X et w ∈ W_X avec l_X(xw) ≤ l_X(w) = q. D’après le cor. 4 de la prop. 7, on a donc
$$
l_S(xw) ≤ l_S(w) = q.
$$
Soient x_1, ..., x_q des éléments de X tels que w = x_1 ... x_q ; comme (W, S) satisfait à la condition d’échange (th. 1 du n° 6), il existe un entier j tel que 1 ≤ j ≤ q et xx_1 ... x_{j-1} = x_1 ... x_{j-1}x_j. Par suite, (W_X, X) satisfait à la condition d’échange, donc c’est un système de Coxeter (th. 1 du n° 6). D’où (i).
Les assertions (ii) et (iii) résultent immédiatement du cor. 1 de la prop. 7.

### 9. Matrices et graphes de Coxeter

#### Définition 4 {#lie-iv-s1-def-4 .statement}

Soit I un ensemble. On appelle matrice de Coxeter de type I toute matrice carrée symétrique M = (m_{ij})_{i,j ∈ I} dont les éléments sont des entiers ou +∞ satisfaisant aux relations:
(25) $ m_{ii} = 1 $ pour tout $ i ∈ I $;
(26) $ m_{ij} ≥ 2 $ pour $ i, j ∈ I $ avec $ i ≠ j $.

On appelle (par abus de langage) graphe de Coxeter de type I un couple formé d’un graphe Γ (*) ayant I comme ensemble de sommets et d’une application f de l’ensemble des arêtes de ce graphe dans l’ensemble formé de +∞ et des entiers ≥ 3. On dit que Γ est le graphe sous-jacent au graphe de Coxeter (Γ, f).

A toute matrice de Coxeter M de type I, on associe un graphe de Coxeter (Γ, f) de la manière suivante:
le graphe Γ a pour ensemble de sommets I et pour ensemble d’arêtes les parties {i, j} de I telles que m_{i,j} ≥ 3, l’application f associe à l’arête {i, j} l’élément correspondant m_{ij} de M.

(*) Voir l’annexe pour la définition et les propriétés des graphes utilisées ici.

Il est clair que l’on obtient ainsi une bijection de l’ensemble des matrices de Coxeter de type I sur l’ensemble des graphes de Coxeter de type I.

Pour faciliter la lecture des raisonnements, on représente souvent un graphe de Coxeter de type I par la figure utilisée pour représenter son graphe sous-jacent, où l’on inscrit en outre à côté ou au-dessus de chaque arête {i, j} le nombre f({i, j}). On omet généralement d’inscrire ceux de ces nombres qui sont égaux à 3.

Si (W, S) est un système de Coxeter, la matrice $ M = (m(s, s'))_{s, s' \in S} $, où $ m(s, s') $ est l’ordre de ss', est une matrice de Coxeter de type S, que l’on appelle la matrice de (W, S) : on a en effet $ m(s, s) = 1 $ puisque $ s^2 = 1 $ pour tout $ s \in S $, et $ m(s, s') = m(s', s) \geq 2 $ si $ s \neq s' $ puisque $ ss' = (s's)^{-1} $ est alors $ \neq 1 $. Le graphe de Coxeter ($ \Gamma, f $) associé à $ M $ s’appelle le graphe de Coxeter de (W, S). Remarquons que deux sommets s et s' de $ \Gamma $ sont liés si et seulement si s et s' ne commutent pas. Par exemple, la matrice de Coxeter d’un groupe diédral d’ordre $ 2m $ est $ \begin{pmatrix} 1 & m \\ m & 1 \end{pmatrix} $ et son graphe de Coxeter est représenté par

lorsque $ m \geq 3 $ (ou

si $ m = 3 $) et par

lorsque $ m = 2 $. *Le graphe de Coxeter du groupe symétrique $ \mathfrak{S}_n $ est représenté par

$$
\circ \cdots \circ \quad (n - 1 \text{ sommets}).
$$

On montrera plus tard (chap. V, § 4) que réciproquement toute matrice de Coxeter est la matrice d’un système de Coxeter.

On dit qu’un système de Coxeter (W, S) est irréductible si le graphe $ \Gamma $ sous-jacent au graphe de Coxeter associé est connexe (Annexe, no 2) et non vide. Il revient au même de dire que S est non vide et qu’il n’existe pas de partition de S en deux ensembles S' et S'' distincts de S tels que tout élément de S' commute avec tout élément de S''. Plus généralement, soit $ (\Gamma_i)_{i \in I} $ la famille des composantes connexes de $ \Gamma $ (Annexe, no 2) et soit $ S_i $ l’ensemble des sommets de $ \Gamma_i $. Soit $ W_i = W_{S_i} $ le sous-groupe de W engendré par $ S_i $ (cf. no 8). Alors les $ (W_i, S_i) $ sont des systèmes de Coxeter irréductibles (no 8, th. 2) qu’on appelle les composantes irréductibles de (W, S). De plus, le groupe W est produit direct restreint (*) des

(*) On dit qu’un groupe G est produit direct restreint d’une famille $ (G_i)_{i \in I} $ de sous-groupes si, pour toute partie finie J de I, le sous-groupe $ G_J $ de G engendré par les $ G_i $ pour $ i \in J $ est produit direct des $ G_i $ pour $ i \in J $, et si G est la réunion des $ G_j $. Il revient au même de dire que tout élément de $ G_i $ commute avec tout élément de $ G_j $ pour $ i \neq j $ et que tout élément de G s’écrit d’une manière et d’une seule comme produit $ \prod_{i \in I} g_i $ avec $ g_i \in G_i $ et $ g_i = 1 $ sauf pour un nombre fini d’indices. Cette dernière condition équivaut à dire que G est engendré par la réunion des $ G_i $ et que $ G_i \cap G_j = \{ 1 \} $ pour tout $ i \in I $ et toute partie finie $ J \subset I $ telle que $ i \notin J $.

sous-groupes $ W_i $ pour $ i \in I $. Cela résulte en effet de la proposition plus générale suivante :

#### Proposition 8 {#lie-iv-s1-prop-8 .statement}

*Soit* $ (S_i)_{i \in I} $ *une partition de S*, *telle que tout élément de S_i commute avec tout élément de S_j pour i \neq j*. *Pour tout i \in I*, *soit* $ W_i $ *le sous-groupe engendré par S_i*. *Alors* W *est produit direct restreint de la famille* $ (W_i)_{i \in I} $.

Il est clair que pour tout $ i \in I $, le sous-groupe $ W'_i $ engendré par la réunion des $ W_j $ pour $ j \neq i $ est aussi engendré par $ S'_i = \bigcup_{j \neq i} S_j $. On a donc

$$
W_i \cap W'_i = W_o = \{1\},
$$

d’après le th. 2 du n° 8. Comme W est engendré par la réunion des $ W_i $, cela démontre la proposition.

## EXERCICES {#lie-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
