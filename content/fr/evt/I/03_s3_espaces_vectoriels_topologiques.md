---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: Espaces vectoriels topologiques sur un corps valué
section: 3
section_title: Espaces vectoriels topologiques métrisables
lang: fr
source: evt-i-v-fr
book_pages: EVT I.28-EVT I.29
pdf_pages: 0022-0028, 0034-0035
extraction: ocr
subsections:
    - "no": 1
      title: Voisinages de 0 dans un espace vectoriel topologique métrisable
      page: 16
      pdf_page: 22
    - "no": 2
      title: Propriétés des espaces vectoriels métrisables
      page: 17
      pdf_page: 23
    - "no": 3
      title: Fonctions linéaires continues dans un espace vectoriel métrisable
      page: 17
      pdf_page: 23
statements: 11
exercises: 9
content_sha256: 40a8dbfebca09c963e47c7e1a135f0060cdcd1578ab3a0a08b49bfaeb9e52620
---

## § 3. ESPACES VECTORIELS TOPOLOGIQUES MÉTRISABLES

### 1. Voisinages de 0 dans un espace vectoriel topologique métrisable

Nous dirons qu’un espace vectoriel topologique E est *métrisable* si sa topologie est métrisable. Muni de sa structure de groupe additif et de sa topologie, E est donc un groupe métrisable (TG, IX, p. 24).

On sait que, pour qu’un groupe topologique soit métrisable, il faut et il suffit que l’élément neutre $ e $ admette un système fondamental dénombrable de voisinages, dont l’intersection soit réduite à $ e $ (TG, IX, p. 23, prop. 1).

On sait qu’on peut définir la structure uniforme d’un espace vectoriel topologique métrisable E par une *distance invariante* $ d(x, y) = |x - y| $, $ x \mapsto |x| $ étant une application continue de E dans $ \mathbf{R}_+ $, qui satisfait aux trois conditions : 1) $ |-x| = |x| $; 2) $ |x + y| \leq |x| + |y| $; 3) la relation $ |x| = 0 $ est équivalente à $ x = 0 $ (TG, IX, p. 24, prop. 3).

On a vu (TG, IX, p. 24, prop. 2) comment une telle distance $ d $ peut être définie à l’aide d’une suite décroissante $ (W_n) $ de voisinages de 0 dans E, formant un système fondamental de voisinages, et telle que $ W_{n+1} + W_{n+1} + W_{n+1} \subset W_n $. Lorsque E est un espace vectoriel métrisable sur un corps valué non discret K, on peut supposer en outre que les $ W_n $ sont équilibrés (I, p. 7, prop. 4); si on remonte au procédé de définition de d (*loc. cit.*), on voit alors que la relation $ |\lambda| \leq 1 $ entraîne $ |\lambda x| \leq |x| $. En outre, les conditions (EVT$_1$) et (EVT$_1'$) de I, p. 3 entraînent que, pour tout $ x_0 \in E $, $ |\lambda x_0| $ tend vers 0 avec $ \lambda \in K $, et que, pour tout $ \lambda_0 \in K $, $ |\lambda_0 x| $ tend vers 0 avec $ |x| $. Inversement, si la fonction $ |x| $ possède toutes les propriétés précédentes, et si $ W_n $ désigne l’ensemble des $ x \in E $ tels que $ |x| \leq 2^{-n} $, on constate aussitôt que les $ W_n $ forment un système fondamental de voisinages équilibrés de 0 pour une topologie métrisable sur E, compatible avec la structure d’espace vectoriel de E.

#### Remarque {#evt-i-s3-n1-rem-1 .statement}

Les espaces normés forment l’une des classes d’espaces vectoriels métrisables les plus importantes (I, p. 3). Mais il faut noter qu’il existe des espaces vectoriels métrisables dont la topologie ne peut être définie par une norme (I, p. 28, exerc. 1); nous en étudierons plus tard d’importants exemples.

### 2. Propriétés des espaces vectoriels métrisables

Tout sous-espace vectoriel d’un espace vectoriel topologique métrisable E est métrisable; il en est de même de tout espace quotient E/M de E par un sous-espace vectoriel fermé M (TG, IX, p. 25, prop. 4). Tout produit d’une famille dénombrable d’espaces vectoriels topologiques métrisables est métrisable (TG, IX, p. 15, cor. 2). Si $ K_0 $ est un corps valué complet, et K un sous-corps partout dense de $ K_0 $, le complété $ \hat{E} $ d’un espace vectoriel métrisable E sur K est un espace vectoriel métrisable sur $ K_0 $ (I, p. 6 et TG, IX, p. 12, prop. 1). Enfin, si E est un espace vectoriel métrisable et complet, pour tout sous-espace vectoriel fermé M de E, E/M est complet (TG, IX, p. 25, prop. 4).

### 3. Fonctions linéaires continues dans un espace vectoriel métrisable

#### Théorème 1 (Banach) {#evt-i-s3-thm-1 .statement}

Soient E et F deux espaces vectoriels métrisables sur un corps valué non discret K, et u une application linéaire continue de E dans F. Supposons que E soit complet. Alors les conditions suivantes sont équivalentes:

(i) u est un morphisme strict surjectif.
(ii) F est complet et u est surjectif.
(iii) L’image de u n’est pas maigre (TG, IX, p. 53) dans F.
(iv) Pour tout voisinage V de 0 dans E, $ u(V) $ est un voisinage de 0 dans F.

Montrons que (i) implique (ii). Supposons que u soit un morphisme strict surjectif, et soit N le noyau de u. Alors u induit un isomorphisme de E/N sur F. De plus, comme E est métrisable et complet, E/N est complet (TG, IX, p. 25, prop. 4), donc F est complet.

Montrons que (ii) implique (iii). Supposons que F soit complet et u surjectif. L’image de u est égale à F, donc n’est pas maigre dans F d’après le théorème de Baire (TG, IX, p. 55).

Le lemme suivant montre que (iii) implique (iv):

#### Lemme 1 {#evt-i-s3-lem-1 .statement}

Soient E et F deux espaces vectoriels topologiques sur un corps valué non discret K, et soit u une application linéaire continue de E dans F dont l’image n’est pas maigre. Pour tout voisinage V de 0 dans E, $ \overline{u(V)} $ est un voisinage de 0 dans F.

Soit W un voisinage équilibré de 0 dans E tel que W + W ⊂ V (I, p. 7, prop. 4). Soit d’autre part α un élément de K tel que $ |\alpha| > 1 $; alors E est la réunion des ensembles $ \alpha^n W $ pour n parcourant N : en effet, pour tout $ x \in E $, il existe $ \beta \in K $ tel que $ x \in \beta W $ (I, p. 7, prop. 4) et il existe un entier $ n \geq 0 $ tel que $ |\beta| < |\alpha|^n $, d’où $ x \in \alpha^n W $ puisque W est équilibré. Par suite, $ u(E) $ est réunion de la suite des ensembles $ u(\alpha^n W) = \alpha^n u(W) $, et comme $ u(E) $ n’est pas maigre dans F, l’un au moins des ensembles $ \alpha^n u(W) $ a un point intérieur (TG, IX, p. 53, déf. 2). Soit $ y_0 $ un point intérieur de $ u(W) $; on a $ -u(W) = u(W) $, d’où $ -u(W) = u(W) $ et par suite $ 0 = y_0 + (-y_0) $ est un point intérieur de $ u(W) + u(W) $. Comme l’addition est une application continue de F × F dans F, l’ensemble $ u(W) + u(W) $ est contenu dans l’adhérence de l’ensemble

$$
u(W) + u(W) = u(W + W) \subset u(V);
$$

par suite, $ \overline{u(V)} $ est un voisinage de 0 dans F.

Dans l’énoncé suivant, on convient que, dans tout espace métrique, $ B_r(x) $ désigne la boule fermée de centre x et de rayon r.

#### Lemme 2 {#evt-i-s3-lem-2 .statement}

Soient E et F deux espaces métriques, E étant en outre supposé complet. Soit u une application continue de E dans F, ayant la propriété suivante : quel que soit le nombre $ r > 0 $, il existe un nombre $ \rho(r) > 0 $ tel que, pour tout $ x \in E $, on ait

$$
B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))}.
$$

Dans ces conditions, pour tout $ a > r $, l’image $ u(B_a(x)) $ contient la boule $ B_{\rho(r)}(u(x)) $.

Soit en effet $ (r_n) $ une suite infinie de nombres $ > 0 $ telle que $ r_1 = r $ et $ a = \sum_{n=1}^\infty r_n $. Pour chaque indice n, il existe un nombre $ \rho_n > 0 $ (avec $ \rho_1 = \rho(r) $) tel que

$$
B_{\rho_n}(u(x)) \subset \overline{u(B_{r_n}(x))}
$$

pour tout $ x \in E $; on peut toujours supposer que $ \lim_{n \to \infty} \rho_n = 0 $.

Soit $ x_0 $ un point de E, et soit $ y $ un point de $ B_{\rho(r)}(u(x_0)) $. Nous allons montrer que $ y $ appartient à $ u(B_a(x_0)) $.

Pour cela, nous allons déterminer par récurrence une suite $ (x_n)_{n>0} $ de points de E telle que, pour tout $ n \geq 1 $, on ait $ x_n \in B_{r_n}(x_{n-1}) $ et $ u(x_n) \in B_{\rho_{n+1}}(y) $. Si les $ x_i $ sont déterminés pour $ 0 \leq i \leq n-1 $ et satisfont à ces relations, on a $ y \in B_{\rho_n}(u(x_{n-1})) $; comme

$$
B_{\rho_n}(u(x_{n-1})) \subset \overline{u(B_{r_n}(x_{n-1}))},
$$

il existe un point $ x_n \in B_{r_n}(x_{n-1}) $ dont l’image $ u(x_n) $ appartient au voisinage $ B_{\rho_{n+1}}(y) $ de $ y $, ce qui démontre l’existence de la suite $ (x_n) $.

La suite $ (x_n) $ est une suite de Cauchy dans E, car la distance de $ x_n $ à $ x_{n+p} $ est majorée par $ r_{n+1} + r_{n+2} + \cdots + r_{n+p} $, qui est arbitrairement petit dès que $ n $ est assez grand. Comme E est complet, la suite $ (x_n) $ converge vers un point $ x \in E $, et la distance de $ x_0 $ à $ x $ est majorée par $ \sum_{n=1}^\infty r_n = a $, donc $ x \in B_a(x_0) $. Mais comme $ u $ est continue, la suite $ (u(x_n)) $ converge vers $ u(x) $; or on a $ u(x_n) \in B_{\rho_{n+1}}(y) $, donc $ y = u(x) $, ce qui achève la démonstration du lemme 2.

Supposons que $ u $ satisfasse à la condition (iv). Munissons chacun des espaces E et F d'une distance invariante par translation et définissant sa topologie (I, p. 16). Par hypothèse, l'ensemble $ \overline{u(B_r(0))} $ est un voisinage de 0 pour tout nombre $ r > 0 $, et il existe donc un nombre $ \rho(r) > 0 $ tel que $ B_{\rho(r)}(0) \subset \overline{u(B_r(0))} $. Par translation, on en conclut que $ B_{\rho(r)}(u(x)) $ est contenue dans $ u(B_r(x)) $ pour tout $ r > 0 $ et tout $ x \in E $. D'après le lemme 2, pour tout couple $ (a, r) $ de nombres réels tel que $ a > r > 0 $, on a $ B_{\rho(r)}(0) \subset u(B_a(0)) $, donc $ u $ est un morphisme strict de E sur F. On a prouvé que (iv) implique (i).

#### Corollaire 1 {#evt-i-s3-lem-2-cor-1 .statement}

Si E et F sont deux espaces vectoriels métrisables et complets sur un corps valué non discret, toute application linéaire continue et bijective $ u $ de E sur F est un isomorphisme.

En particulier, si E et F sont des espaces normés complets, il existe un nombre $ a > 0 $ tel que $ \|u(x)\| \geq a.\|x\| $ pour tout $ x \in E $.

#### Corollaire 2 {#evt-i-s3-lem-2-cor-2 .statement}

Soient E un espace vectoriel sur un corps valué non discret, $ \mathcal{T}_1 $ et $ \mathcal{T}_2 $ deux topologies sur E compatibles avec sa structure d'espace vectoriel et pour chacune desquelles E est métrisable et complet. Si $ \mathcal{T}_1 $ et $ \mathcal{T}_2 $ sont comparables, elles sont identiques.

#### Corollaire 3 {#evt-i-s3-lem-2-cor-3 .statement}

Soient E et F deux espaces vectoriels métrisables et complets sur un corps valué non discret. Pour qu'une application linéaire continue $ u $ de E dans F soit un morphisme strict, il faut et il suffit que $ u(E) $ soit fermé dans F.

La condition est nécessaire, car si $ u $ est un morphisme strict, $ u(E) $, isomorphe au quotient $ E/u^{-1}(0) $, est complet (I, p. 17) donc fermé dans F. La condition est suffisante, car si $ u(E) $ est fermé dans F, c'est un espace vectoriel métrisable et complet, donc $ u $ est un morphisme strict de E sur $ u(E) $ en vertu du th. 1.

#### Corollaire 4 {#evt-i-s3-lem-2-cor-4 .statement}

Soit E un espace vectoriel métrisable et complet sur un corps valué non discret. Si M et N sont deux sous-espaces vectoriels fermés supplémentaires (algébriques) dans E, E est somme directe topologique de M et de N.

En effet, $ M \times N $ est un espace vectoriel métrisable et complet, et l'application $ (y, z) \mapsto y + z $ de $ M \times N $ sur E est continue et bijective, donc un isomorphisme (cor. 1).

#### Corollaire 5 (théorème du graphe fermé) {#evt-i-s3-lem-2-cor-5 .statement}

Soient E et F deux espaces vectoriels métrisables et complets sur un corps valué non discret. Pour qu'une application linéaire u de E dans F soit continue, il faut et il suffit que son graphe dans l’espace produit E × F soit fermé.

La condition est nécessaire, le graphe d’une application continue dans un espace séparé étant toujours fermé (TG, I, p. 53, cor. 2). Pour voir qu’elle est suffisante, remarquons qu’elle entraîne que le graphe G de u, sous-espace vectoriel fermé de l’espace métrisable et complet E × F, est lui-même métrisable et complet. La projection z ↦ pr₁(z) de G sur E est une application linéaire continue et bijective, donc un isomorphisme (cor. 1); comme son application réciproque est x ↦ (x, u(x)), u est continue dans E.

On peut encore exprimer ce corollaire sous la forme suivante : si, pour toute suite (xₙ) de points de E qui converge vers 0 et est telle que la suite (u(xₙ)) ait une limite y, on a nécessairement y = 0, alors u est continue.

#### Exemple {#evt-i-s3-n3-exa-1 .statement}

Soit E un sous-espace vectoriel de l’espace des fonctions numériques définies dans I = {0, 1}; soit \|f\| une norme sur E telle que E, muni de cette norme, soit complet, et que sa topologie soit plus fine que la topologie de la convergence simple. Supposons en outre que E contienne l’ensemble $ C^\infty(I) $ des fonctions indéfiniment dérivables dans I; nous allons montrer qu’il existe alors un entier $ k \geqslant 0 $ tel que E contienne l’ensemble $ C^k(I) $ de toutes les fonctions admettant une dérivée k-ième continue dans I.

Pour tout couple d’entiers $ m > 0, n \geqslant 0 $, soit $ V_{mn} $ l’ensemble des fonctions $ f \in C^\infty(I) $ telles que $ |f^{(h)}(x)| \leqslant 1/m $ pour $ 0 \leqslant h \leqslant n $ et pour tout $ x \in I $; on vérifie aussitôt que les $ V_{mn} $ forment un système fondamental de voisinages de 0 pour une topologie métrisable compatible avec la structure d’espace vectoriel de $ C^\infty(I) $; en outre, $ C^\infty(I) $ est complet pour cette topologie (FVR, II, p. 2, th. 1). Soit u l’application canonique de $ C^\infty(I) $ dans E ; montrons que u est continue. En vertu du cor. 5 de I, p. 19, il suffit de prouver que, si une suite $ (f_n) $ converge vers 0 dans $ C^\infty(I) $ et a une limite f dans E, on a nécessairement $ f = 0 $, ce qui est immédiat, puisque f est par hypothèse limite simple de $ (f_n) $. Il existe donc un entier $ k \geqslant 0 $ et un nombre $ a > 0 $ tels que la relation
$$
p_k(f) = \sup_{\substack{x \in I \\ 0 \leqslant h \leqslant k}} |f^{(h)}(x)| \leqslant a
$$
entraîne $ \|f\| \leqslant 1 $ pour toute fonction $ f \in C^\infty(I) $.

Mais $ p_k $ est une norme sur l’espace $ C^k(I) $, et $ C^\infty(I) $ est un sous-espace partout dense de $ C^k(I) $ pour cette norme (l’ensemble des polynômes étant déjà partout dense dans $ C^k(I) $, comme il résulte aussitôt du th. de Weierstrass-Stone). Comme, en vertu de ce qui précède, l’application identique de $ C^\infty(I) $ (muni de la norme $ p_k $) dans E est continue, elle se prolonge par continuité à l’espace $ C^k(I) $ tout entier (parce que E est complet), ce qui démontre notre assertion.

#### Proposition 1 {#evt-i-s3-prop-1 .statement}

Soient E, F deux espaces vectoriels topologiques sur un corps valué non discret K. On suppose que :

1) E est métrisable et complet.
2) Il existe une suite $ (F_n) $ d’espaces vectoriels métrisables et complets sur K et, pour tout n, une application linéaire injective et continue $ v_n $ de $ F_n $ dans F telles que F soit réunion des sous-espaces $ v_n(F_n) $.

Soit alors u une application linéaire de E dans F. Si le graphe de u est fermé dans E × F, il existe un entier n et une application linéaire continue $ u_n $ de E dans $ F_n $ tels que $ u = v_n \circ u_n $ (ce qui entraîne que u est continue et que $ u(E) \subset v_n(F_n) $).

Soit G le graphe de u dans E × F. Pour tout n, considérons l’application linéaire continue $ w_n : (x, y) \mapsto (x, v_n(y)) $ de $ E \times F_n $ dans $ E \times F $; comme $ G $ est fermé, $ w_n^{-1}(G) = G_n $ est un sous-espace vectoriel fermé de $ E \times F_n $; si $ p_n $ est la restriction à $ G_n $ de la première projection $ pr_1 $, on a $ p_n(G_n) = u^{-1}(v_n(F_n)) $. Comme $ p_n $ est continue et $ G_n $ complet (puisque $ G_n $ est fermé dans l’espace complet $ E \times F_n $), $ p_n(G_n) $ est ou bien maigre dans $ E $, ou bien égal à $ E $ en vertu du th. 1. Mais par hypothèse $ E $ est réunion des $ p_n(G_n) $, et comme $ E $ est complet, les $ p_n(G_n) $ ne peuvent être tous maigres dans $ E $ en vertu du th. de Baire (TG, IX, p. 55, th. 1). Donc il existe un entier $ n $ tel que $ p_n(G_n) = E $, autrement dit $ u(E) \subset v_n(F_n) $. En outre, comme $ v_n $ est injective, $ G_n $ est le graphe d’une application linéaire $ u_n $ de $ E $ dans $ F_n $, et en vertu du th. du graphe fermé (I, p. 19, cor. 5) $ u_n $ est *continue* ; il résulte alors des définitions que $ u = v_n \circ u_n $.

C.Q.F.D.

Exercises

## EXERCICES {#evt-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
