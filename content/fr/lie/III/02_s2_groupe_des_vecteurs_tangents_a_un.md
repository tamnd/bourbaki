---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 2
section_title: Groupe des vecteurs tangents à un groupe de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0118-0122
extraction: ocr
subsections:
    - "no": 1
      title: Lois de composition tangentes
      page: 0
      pdf_page: 118
    - "no": 2
      title: Groupe des vecteurs tangents à un groupe de Lie
      page: 0
      pdf_page: 120
    - "no": 3
      title: Cas des groupuscules
      page: 0
      pdf_page: 122
statements: 10
exercises: 0
content_sha256: 9d94aa1466a38057a2b7d2bacbfed1953e7c1bfef258be2bc3963c3719a915a4
---

## § 2. Groupe des vecteurs tangents à un groupe de Lie

### 1. Lois de composition tangentes

Soient X et Y des variétés de classe $ C^r $. On sait (VAR, R, 8.1.4) que $ X \times Y $ est une variété de classe $ C^r $ et que l’application $ (T(\mathrm{pr}_1), T(\mathrm{pr}_2)) $, produit des applications tangentes aux projections canoniques, est un isomorphisme de classe $ C^{r-1} $ de $ T(X \times Y) $ sur $ T(X) \times T(Y) $.\footnote{Pour $ r = 1 $, cela signifie que $ (T(\mathrm{pr}_1), T(\mathrm{pr}_2)) $ est un homéomorphisme de $ T(X \times Y) $ sur $ T(X) \times T(Y) $.} Cet isomorphisme est compatible avec les structures de fibré vectoriel de base $ X \times Y $, et permet d’identifier $ T(X \times Y) $ avec $ T(X) \times T(Y) $. Soient $ a \in X, b \in Y, u \in T_a(X), v \in T_b(Y) $; l’identification précédente permet de considérer $ (u, v) $ comme un élément de $ T_{(a,b)}(X \times Y) $; on a
$$
(u, v) = (u, 0) + (0, v),
$$
et $ (u, 0) $ (resp. $ (0, v) $) est l’image de $ u $ par l’application tangente à l’immersion $ x \mapsto (x, b) $ (resp. $ y \mapsto (a, y) $) de X (resp. Y) dans $ X \times Y $. Quand il sera nécessaire de préciser, on notera $ 0_a $ l’élément nul de $ T_a(X) $.

Soient maintenant X, Y, Z des variétés de classe $ C^r $, et $ f $ une application de classe $ C^r $ de $ X \times Y $ dans Z. L’application tangente est, compte tenu de l’identification précédente, une application de classe $ C^{r-1} $ de $ T(X) \times T(Y) $ dans $ T(Z) $. Pour $ u \in T_a(X) $ et $ v \in T_b(Y) $, on a
$$
\begin{align*}
(1) \quad & T(f)(u, v) = T(f)(u, 0_b) + T(f)(0_a, v), \\
(2) \quad & T(f)(0_a, 0_b) = 0_{f(a,b)}.
\end{align*}
$$
D’autre part, l’application $ y \mapsto f(a, y) $ est composée de l’immersion $ y \mapsto (a, y) $ et de $ f $; on en déduit que
(3) $ T(f)(0, v) $ est l’image de $ v $ par l’application tangente à $ y \mapsto f(a, y) $.
De même
(4) $ T(f)(u, 0) $ est l’image de $ u $ par l’application tangente à $ x \mapsto f(x, b) $.

Si l’application $ f $ de $ X \times Y $ dans Z est notée $ (x, y) \mapsto xy $, on note souvent $ uv $ l’élément $ T(f)(u, v) $ pour $ u \in T(X), v \in T(Y) $.

Soient X une variété de classe $ C^r $, et $ m : X \times X \to X $ une loi de composition de classe $ C^r $ sur X. Alors $ T(m) $ est une loi de composition de classe $ C^{r-1} $ sur $ T(X) $. On l’appelle la *loi de composition tangente à m*. La projection canonique $ p $ de $ T(X) $ sur X est compatible avec les lois $ m $ et $ T(m) $; autrement dit, on a
$$
p \circ T(m) = m \circ (p \times p).
$$

Il résulte de (2) que

$$
T(m)(0_x, 0_y) = 0_{m(x, y)}
$$

quels que soient $ x, y $ dans $ X $; autrement dit, la section nulle $ x \mapsto 0_x $ de $ T(X) $ est compatible avec les lois $ m $ et $ T(m) $.

#### Proposition 1 {#lie-iii-s2-prop-1 .statement}

*Soient $ X $ une variété de classe $ C^r $, et $ m $ une loi de composition de classe $ C^r $ sur $ X $. Si $ m $ est associative (resp. commutative), alors $ T(m) $ est associative (resp. commutative).*

Si $ m $ est associative, on a $ m \circ (m \times \mathrm{Id}_X) = m \circ (\mathrm{Id}_X \times m) $, d’où

$$
T(m) \circ (T(m) \times \mathrm{Id}_{T(X)}) = T(m) \circ (\mathrm{Id}_{T(X)} \times T(m))
$$

donc $ T(m) $ est associative. Soit $ s $ l’application $ (x, y) \mapsto (y, x) $ de $ X \times X $ dans $ X \times X $. Si $ m $ est commutative, on a $ m \circ s = m $, donc

$$
T(m) \circ T(s) = T(m).
$$

Mais $ T(s) $ est l’application $ (u, v) \mapsto (v, u) $ de $ T(X) \times T(X) $ dans $ T(X) \times T(X) $. Donc $ T(m) $ est commutative.

#### Proposition 2 {#lie-iii-s2-prop-2 .statement}

*Soient $ X $ une variété de classe $ C^r $, $ m $ une loi de composition de classe $ C^r $ sur $ X $, $ e $ un élément neutre pour $ m $.
(i) Le vecteur $ 0_e $ est élément neutre pour $ T(m) $.
(ii) $ T_e(X) $ est stable pour $ T(m) $, et la loi de composition induite sur $ T_e(X) $ par $ T(m) $ est l’addition de l’espace vectoriel $ T_e(X) $.
(iii) Soient $ U $ une partie ouverte de $ X $, et $ \alpha $ une application de classe $ C^r $ de $ U $ dans $ X $ telle que, pour tout $ x \in U $, $ \alpha(x) $ soit inverse de $ x $ pour $ m $. Alors, pour tout $ u \in T(U) $, $ T(\alpha)u $ est inverse de $ u $ pour $ T(m) $.*

Les propriétés (3) et (4) montrent que $ T(m)(0_e, u) = T(m)(u, 0_e) = u $ pour tout $ u \in T(X) $, d’où (i). Pour $ u, v $ dans $ T_e(X) $, on a

$$
T(m)(u, v) = T(m)(u, 0_e) + T(m)(0_e, v) = u + v
$$

d’où (ii). Enfin, les relations $ m(x, \alpha(x)) = m(\alpha(x), x) = e $ pour tout $ x \in U $ entraînent

$$
T(m)(u, T(\alpha)(u)) = T(m)(T(\alpha)u, u) = 0_e
$$

pour tout $ u \in T(U) $, d’où (iii).

#### Proposition 3 {#lie-iii-s2-prop-3 .statement}

*Soient $ X_1, X_2, \ldots, X_p, Y $ des variétés de classe $ C^r $, $ i $ un entier de $ [1, p] $, $ m_i $ (resp. $ n $) une loi de composition de classe $ C^r $ sur $ X_i $ (resp. $ Y $), $ u $ une application de classe $ C^r $ de $ X_1 \times X_2 \times \cdots \times X_p $ dans $ Y $. Si $ u $ est distributive relativement à la variable d’indice $ i $, alors $ T(u) $ est distributive relativement à la variable d’indice $ i $.*

La démonstration est analogue à celle de la prop. 1.

### 2. Groupe des vecteurs tangents à un groupe de Lie

#### Proposition 4 {#lie-iii-s2-prop-4 .statement}

Soit $ G $ un groupe de Lie. Alors $ T(G) $, muni de la loi de composition tangente à la multiplication de $ G $, est un groupe de Lie. L’élément neutre de $ T(G) $ est le vecteur $ 0_e $.

Cela résulte des prop. 1 et 2.

#### Proposition 5 {#lie-iii-s2-prop-5 .statement}

Soient $ G $ et $ H $ des groupes de Lie, $ f $ un morphisme de $ G $ dans $ H $. Alors $ T(f) $ est un morphisme du groupe de Lie $ T(G) $ dans le groupe de Lie $ T(H) $.

On sait que $ T(f) $ est analytique. D’autre part, soit $ m $ (resp. $ n $) la multiplication dans $ G $ (resp. $ H $). On a $ f \circ m = n \circ (f \times f) $, d’où

$$
T(f) \circ T(m) = T(n) \circ (T(f) \times T(f)),
$$

ce qui exprime que $ T(f) $ est un homomorphisme de groupes.

#### Corollaire {#lie-iii-s2-n2-cor-1 .statement}

Soient $ G_1, \ldots, G_n $ des groupes de Lie. L’isomorphisme canonique de la variété $ T(G_1 \times \cdots \times G_n) $ sur la variété $ T(G_1) \times \cdots \times T(G_n) $ est un isomorphisme de groupes de Lie.

En effet, $ \mathrm{pr}_i $ est un morphisme de $ G_1 \times \cdots \times G_n $ dans $ G_i $, donc $ T(\mathrm{pr}_i) $ est un morphisme de $ T(G_1 \times \cdots \times G_n) $ dans $ T(G_i) $.

#### Proposition 6 {#lie-iii-s2-prop-6 .statement}

Soit $ G $ un groupe de Lie.

(i) La projection canonique $ p : T(G) \to G $ est un morphisme de groupes de Lie.

(ii) Le noyau de $ p $ est $ T_e(G) $. C’est un sous-groupe de Lie de $ T(G) $. La structure de groupe de Lie induite sur $ T_e(G) $ par celle de $ T(G) $ est la structure de groupe de Lie de l’espace normable complet $ T_e(G) $.

(iii) La section nulle $ s $ est un isomorphisme du groupe de Lie $ G $ sur un sous-groupe de Lie $ s(G) $ de $ T(G) $ (sous-groupe qu’on identifie à $ G $).

(iv) Le groupe de Lie $ T(G) $ est produit semi-direct de $ G $ par $ T_e(G) $.

L’assertion (i) résulte de (5). L’assertion (ii) est évidente compte tenu de la prop. 2 (ii). Les assertions (iii) et (iv) résultent de (6) et du § 1, prop. 8.

C.Q.F.D.

Soient $ u \in T(G) $ et $ g \in G $. D’après (3) et (4), les produits $ ug, gu $ calculés dans le groupe $ T(G) $ sont les images de $ u $ par $ T(\delta(g^{-1})), T(\gamma(g)) $. Il résulte du § 1, cor. 2 de la prop. 17, que l’application $ (g, u) \mapsto gu $ de $ G \times T_e(G) $ dans $ T(G) $ est un isomorphisme du fibré vectoriel trivial $ G \times T_e(G) $ de base $ G $ sur le fibré vectoriel $ T(G) $. L’isomorphisme réciproque s’appelle la trivialisation gauche de $ T(G) $. En considérant l’application $ (g, u) \mapsto ug $, on définit de même la trivialisation droite de $ T(G) $.

#### Proposition 7 {#lie-iii-s2-prop-7 .statement}

Soient G un groupe de Lie, M une variété de classe C^r, f et g des applications de classe C^r de M dans G, de sorte que fg est une application de classe C^r de M dans G. Soient m \in M, x = f(m), y = g(m), u \in T_m(M). On a
$$
T(fg)u = T(f)u.y + x.T(g)u.
$$
Soit m la multiplication de G. On a $ fg = m \circ (f, g) $. Or
$$
T(f, g)(u) = (T(f)u, T(g)u),
$$
donc $ T(fg)u = T(f)u.T(g)u $. Il suffit alors d’appliquer (1) où l’on remplace f par m.

#### Corollaire {#lie-iii-s2-n2-cor-2 .statement}

Soit $ n \in \mathbf{Z} $. L’application tangente en e à l’application $ g \mapsto g^n $ de G dans G est l’application $ x \mapsto nx $ de $ T_e(G) $ dans $ T_e(G) $.

Pour $ n \geqslant 0 $, cela résulte par récurrence sur n de la prop. 7. D’autre part, l’application tangente en e à l’application $ g \mapsto g^{-1} $ est l’application $ x \mapsto -x $ (n° 1, prop. 2).

Soient G un groupe de Lie, X une variété de classe C^r, et $ (g, x) \mapsto gx $ une loi d’opération à gauche de classe C^r de G dans X. Raisonnant comme pour la prop. 1, on en déduit une loi d’opération à gauche de classe C^{r-1} de T(G) dans T(X), que nous noterons encore $ (u, v) \mapsto uv $. Identifiant G (resp. X) à l’image de la section nulle de T(G) (resp. T(X)), on voit, d’après (6), que la loi d’opération à gauche de T(G) dans T(X) prolonge la loi d’opération à gauche de G dans X. Quels que soient $ u \in T_g(G) $ et $ v \in T_x(X) $, on a, d’après (1),
$$
uv = gv + ux.
$$
Si $ g \in G $ et $ v \in T_x(X) $, gv est, d’après (3), l’image de v par l’application tangente en x à l’application $ y \mapsto gy $ de X dans X. Cette application tangente est un isomorphisme de $ T_x(X) $ sur $ T_{gx}(X) $. En particulier,
$$
g(v + v') = gv + gv', \quad g(\lambda v) = \lambda(gv) \quad \text{pour } v, v' \text{ dans } T_x(X), \lambda \in \mathbf{K}.
$$
Si $ x \in X $ et $ u \in T_g(G) $, ux est, d’après (4), l’image de u par l’application tangente en g à l’application $ h \mapsto hx $ de G dans X. Donc
$$
(u + u')x = ux + u'x, \quad (\lambda u)x = \lambda(ux) \quad \text{pour } u, u' \text{ dans } T_g(G), \lambda \in \mathbf{K}.
$$
Ce qui précède s’applique au cas d’un groupe de Lie opérant dans lui-même par translations à gauche (resp. à droite). La loi d’opération correspondante de T(G) dans T(G) est définie par les translations à gauche (resp. à droite) du groupe de Lie T(G). Les formules (7), (8), (9) sont donc valables dans T(G).

#### Proposition 8 {#lie-iii-s2-prop-8 .statement}

Soient $ G_1 $ et $ G_2 $ des groupes de Lie, $ X_1 $ et $ X_2 $ des variétés de classe C^r, $ f_i $ une loi d’opération à gauche de classe C^r de $ G_i $ dans $ X_i $ ($ i = 1, 2 $). Soient $ \varphi $ un morphism de $ G_1 $ dans $ G_2 $, $ \psi $ un $ \varphi $-morphisme de $ X_1 $ dans $ X_2 $. Alors $ T(\psi) $ est un $ T(\varphi) $-morphisme de $ T(X_1) $ dans $ T(X_2) $.

En effet, on a $ f_2 \circ (\varphi \times \psi) = \psi \circ f_1 $, d’où

$$
T(f_2) \circ (T(\varphi) \times T(\psi)) = T(\psi) \circ T(f_1).
$$

Soient $ G $ un groupe de Lie, $ X $ une variété de classe $ C^r $, et $ (g, x) \mapsto gx $ une loi d’opération à gauche de classe $ C^r $ de $ G $ dans $ X $. Soient $ I $ une partie ouverte de $ K $ contenant $ 0 $, et $ \gamma : I \to G $ une application de classe $ C^r $ telle que $ \gamma(0) = e $. Soit $ a = T_0(\gamma)1 \in T_e(G) $. Soit $ x \in X $. Compte tenu de (4), $ ax $ est l’image, par l’application tangente à $ \lambda \mapsto \gamma(\lambda)x $, du vecteur tangent $ 1 $ à $ I $ en $ 0 $. Donc le champ de vecteurs $ x \mapsto ax $ sur $ X $ est le champ de vecteurs défini par l’application $ (\lambda, x) \mapsto \gamma(\lambda)x $ au sens de VAR, R, 8.4.5.

### 3. Cas des groupuscules

Soient $ (G, e, \theta, m) $ un groupuscule de Lie, $ \Omega $ l’ensemble de définition de $ m $. Alors $ T(\Omega) $ s’identifie à une partie ouverte de $ T(G) \times T(G) $, et $ T(m) $ est une application analytique de $ T(\Omega) $ dans $ T(G) $. On vérifie comme au n° 2 que $ (T(G), 0_e, T(\theta), T(m)) $ est un groupuscule de Lie. On note souvent multiplicativement les produits dans $ G $ et $ T(G) $. La projection canonique de $ T(G) $ dans $ G $ est un morphisme de groupuscules de Lie. La restriction de $ T_e(m) $ à $ T_e(G) $ est l’addition de l’espace vectoriel $ T_e(G) $. La section nulle de $ T(G) $ est un isomorphisme du groupuscule de Lie $ G $ sur un sous-groupuscule de Lie de $ T(G) $ qu’on identifie à $ G $. Si $ f $ est un morphisme de $ G $ dans un groupuscule de Lie $ H $, $ T(f) : T(G) \to T(H) $ est un morphisme de groupuscules de Lie.

L’application $ \varphi : (g, u) \mapsto gu $ de $ G \times T_e(G) $ dans $ T(G) $ est un isomorphisme du fibré vectoriel trivial $ G \times T_e(G) $ de base $ G $ sur le fibré vectoriel $ T(G) $; en effet, $ \varphi $ et $ \varphi^{-1} $ sont analytiques, et sont des morphismes de fibration, de sorte qu’il suffit d’appliquer VAR, R, 7.2.1. (On pourrait aussi adapter la démonstration du n° 2.) L’isomorphisme $ \varphi^{-1} $ s’appelle la trivialisation gauche de $ T(G) $. L’isomorphisme réciproque de l’application $ (g, u) \mapsto ug $ s’appelle la trivialisation droite.

Soient $ X $ une variété de classe $ C^r $, $ \psi $ un morceau de loi d’opération à gauche de classe $ C^r $ de $ G $ dans $ X $. Alors $ T(\psi) $ est un morceau de loi d’opération à gauche de classe $ C^{r-1} $ de $ T(G) $ dans $ T(X) $, prolongeant $ \psi $. Les formules (7), (8), (9) restent valables si $ gx $ est défini. Si $ I $ est une partie ouverte de $ K $ contenant $ 0 $, si $ \gamma : I \to G $ est une application de classe $ C^r $ telle que $ \gamma(0) = e $, et si $ a = T_0(\gamma)1 $, le champ de vecteurs $ x \mapsto ax $, défini sur $ X $, est le champ de vecteurs défini par l’application $ (\lambda, x) \mapsto \gamma(\lambda)x $ au sens de VAR, R, 8.4.5.
