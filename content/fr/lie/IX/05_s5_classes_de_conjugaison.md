---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 5
section_title: Classes de conjugaison
lang: fr
source: lie-ix-fr
book_pages: LIE IX.43-LIE IX.51, LIE IX.118-LIE IX.121
pdf_pages: 0046-0054, 0121-0124
extraction: ocr
subsections:
    - "no": 1
      title: Éléments réguliers
      page: 43
      pdf_page: 46
    - "no": 2
      title: Chambres et alcôves
      page: 44
      pdf_page: 47
    - "no": 3
      title: Automorphismes et éléments réguliers
      page: 46
      pdf_page: 49
    - "no": 4
      title: Les applications $ (G/T) \times T \to G $ et $ (G/T) \times A \to G_r $
      page: 49
      pdf_page: 52
statements: 26
exercises: 5
content_sha256: d3c1884d6c875d139b3210957ad4440ffbb101f41be472e1c3137e5f936242e6
---

## § 5. CLASSES DE CONJUGAISON

On conserve les notations du § 4.

### 1. Éléments réguliers

D’après le cor. 4 au th. 2 du § 2, n° 2, les éléments réguliers $ g $ de $ G $ peuvent être caractérisés par l’une ou l’autre des propriétés suivantes :
a) La sous-algèbre de $ g $ fixée par $ \mathrm{Ad}\,g $ est une sous-algèbre de Cartan.
b) $ Z(g)_0 $ est un tore maximal de $ G $.

L’ensemble des éléments réguliers de $ G $ est ouvert et dense dans $ G $.
Dans la suite de ce paragraphe, on note $ G_r $ (resp. $ T_r $) l’ensemble des points de $ G $ (resp. $ T $) qui sont réguliers dans $ G $. Pour qu’un élément $ g $ de $ G $ appartienne à $ T_r $, il faut et il suffit que $ Z(g)_0 $ soit égal à $ T $; tout élément de $ G_r $ est conjugué à un élément de $ T_r $ (§ 2, n° 2, th. 2).
Pour qu’un élément $ t $ de $ T $ appartienne à $ T_r $, il faut et il suffit que, pour toute racine $ \alpha \in R(G, T) $, on ait $ t^\alpha \neq 1 $; par conséquent $ T - T_r $ est réunion des sous-tores $ \mathrm{Ker}\,\alpha $ lorsque $ \alpha $ parcourt $ R(G, T) $.

#### Proposition 1 {#lie-ix-s5-prop-1 .statement tag=01DV}

Posons $ n = \dim G $. Il existe une variété analytique réelle compacte $ V $ de dimension $ n - 3 $ et une application analytique $ \varphi : V \to G $ dont l’image est $ G - G_r $.

Soit $ \alpha \in R(G, T) $; posons $ V_\alpha = (G/Z(\mathrm{Ker}\ \alpha)) \times (\mathrm{Ker}\ \alpha) $, et soit $ \varphi_\alpha $ le morphisme de $ V_\alpha $ dans $ G $ tel que, pour tout $ g \in G $ et tout $ t \in \mathrm{Ker}\ \alpha $, on ait $ \varphi_\alpha(\overline{g}, t) = gtg^{-1} $ (on désigne par $ \overline{g} $ la classe de $ g $ modulo $ Z(\mathrm{Ker}\ \alpha) $). Alors $ V_\alpha $ est une variété analytique réelle compacte de dimension
$$
\dim V_\alpha = \dim G - \dim Z(\mathrm{Ker}\ \alpha) + \dim \mathrm{Ker}\ \alpha = n - (\dim T + 2) + (\dim T - 1) = n - 3
$$
(§ 4, no 5, th. 1); $ \varphi_\alpha $ est un morphisme de variétés analytiques réelles, et l’image de $ \varphi_\alpha $ est formée des éléments de $ G $ conjugués à un élément de $ \mathrm{Ker}\ \alpha $. Il suffit alors de prendre pour $ V $ la somme des variétés $ V_\alpha $, et pour $ \varphi $ le morphisme induisant $ \varphi_\alpha $ sur chaque $ V_\alpha $.

#### Remarque {#lie-ix-s5-n1-rem-1 .statement tag=01DW}

Appelons très réguliers les éléments $ g $ de $ G $ tels que $ Z(g) $ soit un tore maximal de $ G $. Si $ g \in T $, $ g $ est très régulier si et seulement si $ w(g) \neq g $ pour tout élément non neutre $ w $ de $ W_G(T) $ (§ 4, no 7, prop. 14). L’ensemble des éléments très réguliers de $ G $ est donc un ouvert dense de $ G $ (§ 2, no 5, cor. 2 à la prop. 5).

### 2. Chambres et alcôves

Notons $ t_r $ l’ensemble des éléments $ x \in t $ tels que $ \exp x $ soit régulier, c’est-à-dire appartienne à $ T_r $. Pour qu’un élément $ x $ de $ t $ appartienne à $ t - t_r $, il faut et il suffit qu’il existe une racine $ \alpha \in R(G, T) $ telle que $ \delta(\alpha)(x) \in 2\pi i \mathbf{Z} $. Pour chaque racine $ \alpha \in R(G, T) $ et chaque entier $ n $, notons $ H_{\alpha, n} $ l’ensemble des $ x \in t $ tels que $ \delta(\alpha)(x) = 2\pi i n $. Les $ H_{\alpha, n} $ sont appelés les hyperplans singuliers de $ t $, et $ t - t_r $ est réunion des hyperplans singuliers. On appelle alcôves de $ t $ les composantes connexes de $ t_r $, et chambres les composantes connexes du complémentaire dans $ t $ de la réunion de ceux des hyperplans singuliers qui passent par l’origine (c’est-à-dire des $ H_{\alpha, 0} = \mathrm{Ker}\ \delta(\alpha) $, $ \alpha \in R(G, T) $).

On a $ \Gamma(T) \subset t - t_r $; on note $ N(G, T) $ le sous-groupe de $ \Gamma(T) $ engendré par les vecteurs nodaux (§ 4, no 5); d’après la prop. 11 du § 4, no 6, le quotient $ \Gamma(T)/N(G, T) $ s’identifie au groupe fondamental de $ G $.

Enfin, on note $ W $ le groupe de Weyl de $ G $ relativement à $ T $, considéré comme groupe d’automorphismes de $ T $ et de $ t $, et on note $ W_a $ (resp. $ W'_a $) le groupe d’automorphismes de l’espace affine $ t $ engendré par $ W $ et par les translations $ t_\gamma : x \mapsto x + \gamma $ pour $ \gamma \in N(G, T) $ (resp. pour $ \gamma \in \Gamma(T) $).

Soient $ w \in W $, $ \gamma \in \Gamma(T) $, $ \alpha \in R(G, T) $ et $ n \in \mathbf{Z} $. On a :
$$
w(H_{\alpha, n}) = H_{w\alpha, n}, \quad t_\gamma(H_{\alpha, n}) = H_{\alpha, n + <\gamma, \alpha>}.
$$

Il en résulte que pour toute chambre $ C $ et tout $ w \in W $, $ w(C) $ est une chambre et que pour toute alcôve $ A $ et tout $ w \in W'_a $, $ w(A) $ est une alcôve. On notera que lorsqu’on identifie $ X(T) \otimes \mathbf{R} $ à $ t^* $ via l’isomorphisme $ (2\pi i)^{-1} \delta $, les alcôves de $ t $ et le groupe $ W_a $ sont les alcôves et le groupe de Weyl affine associés au système de racines $ R(G, T) $ (VI, § 2, no 1).

#### Proposition 2 {#lie-ix-s5-prop-2 .statement tag=01DX}

a) Le groupe $ W_a $ (resp. $ W'_a $) est produit semi-direct de $ W $ par $ N(G, T) $ (resp. $ \Gamma(T) $); le sous-groupe $ W_a $ de $ W'_a $ est distingué.

b) Le groupe $ W $ (resp. $ W_a $) opère de façon simplement transitive dans l’ensemble des chambres (resp. alcôves).

c) Soient $ C $ une chambre et $ A $ une alcôve. Alors $ \overline{C} $ (resp. $ \overline{A} $, resp. $ A $) est un domaine fondamental pour l’action de $ W $ dans $ t $ (resp. de $ W_a $ dans $ t $, resp. de $ W_a $ dans $ t - t_r $). Si $ x \in t_r $ et $ w \in W_a $ sont tels que $ w(x) = x $, alors $ w = \mathrm{Id} $.

d) Pour toute chambre $ C $, il existe une unique alcôve $ A $ telle que $ A \subset C $ et $ 0 \in \overline{A} $. Pour toute alcôve $ A $, il existe un unique $ \gamma \in N(G, T) $ tel que $ \gamma \in \overline{A} $.

Si $ w \in W $ et $ \gamma \in \Gamma(T) $, on a $ wt_\gamma w^{-1} = t_{w(\gamma)} $ et $ wt_\gamma w^{-1} t_\gamma^{-1} = t_{w(\gamma) - \gamma} $, avec $ w(\gamma) - \gamma \in N(G, T) $; cela implique aussitôt a). Le reste de la proposition résulte de VI, § 1, n° 5 et § 2, n°s 1 et 2.

#### Corollaire 1 {#lie-ix-s5-prop-2-cor-1 .statement tag=01DY}

Soient $ A $ une alcôve de $ t $, $ \overline{A} $ son adhérence, et $ H_A $ le stabilisateur de $ A $ dans $ W'_a $.

a) Le groupe $ W'_a $ est produit semi-direct de $ H_A $ par $ W_a $.

b) L’application exponentielle $ \overline{A} \to T $ et l’injection canonique $ T \to G $ induisent par passage aux quotients et aux sous-ensembles des homéomorphismes

$$
\overline{A}/H_A \to T/W \to G/\mathrm{Int}(G)
$$
$$
A/H_A \to T_r/W \to G_r/\mathrm{Int}(G).
$$

Soit $ w' \in W'_a $; alors $ w'(A) $ est une alcôve de $ t $, et il existe (prop. 2, b)) un unique élément $ w $ de $ W_a $ tel que $ w(A) = w'(A) $, c’est-à-dire $ w^{-1} w' \in H_A $. Puisque $ W_a $ est distingué dans $ W'_a $, ceci démontre a).

L’injection canonique de $ \overline{A} $ dans $ t $ induit une bijection continue $ \theta : \overline{A} \to t/W_a $ (prop. 2, c)), qui est un homéomorphisme puisque $ \overline{A} $ est compact. Comme $ W_a $ est distingué dans $ W'_a $, le groupe $ H_A $ opère de façon canonique dans $ t/W_a $ (A, I, p. 55) et $ t/W'_a $ s’identifie au quotient $ (t/W_a)/H_A $; l’application $ \theta $ est compatible avec les opérations de $ H_A $, donc induit par passage aux quotients un homéomorphisme $ \overline{A}/H_A \to t/W'_a $. Par ailleurs $ \exp_T $ induit un homéomorphisme de $ t/\Gamma(T) $ sur $ T $, donc aussi un homéomorphisme de $ t/W'_a $ sur $ T/W $. L’assertion b) résulte de là et du cor. 1 à la prop. 5 du § 2, n° 4.

#### Remarque 1 {#lie-ix-s5-n2-rem-1 .statement tag=01DZ}

Le groupe $ H_A $ s’identifie naturellement à $ \Gamma(T)/N(G, T) $, donc aussi à $ \pi_1(G) $. Il est donc réduit à l’élément neutre lorsque $ G $ est simplement connexe.

#### Remarque 2 {#lie-ix-s5-n2-rem-2 .statement tag=01E0}

Soit $ x \in A $; on a alors $ \exp x \in T_r $, donc $ Z(\exp x)_0 = T $. Pour que $ \exp x $ soit très régulier (n° 1, remarque), il faut et il suffit qu’on ait $ w(x) \neq x $ pour tout $ w \in W'_a $, distinct de l’identité. D’après le cor. 1, cela signifie aussi que $ h(x) \neq x $ pour tout $ h \in H_A $ distinct de l’identité. En particulier, si $ G $ est simplement connexe, on a $ Z_G(t) = T $ pour tout $ t \in T_r $, et tout élément régulier de $ G $ est très régulier.

#### Remarque 3 {#lie-ix-s5-n2-rem-3 .statement tag=01E1}

Les points spéciaux de $ W_a $ (VI, § 2, n° 2) sont les éléments $ x $ de $ t $ tels que $ \delta(\alpha)(x) \in 2\pi i \mathbf{Z} $ pour tout $ \alpha \in R(G, T) $ (loc. cit., prop. 3), c’est-à-dire tels que exp $ x \in C(G) $ (\S 4, n° 4, prop. 8). Pour un tel élément $ x $ on a $ wx - x \in N(G, T) $ quel que soit $ w \in W $ (VI, \S 1, n° 9, prop. 27), de sorte que les stabilisateurs de $ x $ dans $ W_a $ et dans $ W'_a $ coïncident. Soit $ S $ l’ensemble des points spéciaux de $ A $; il résulte de ce qui précède et du cor. 1 que le groupe $ H_A $ opère librement dans $ S $, et que l’application exponentielle induit une bijection de $ S/H_A $ sur $ C(G) $.

#### Corollaire 2 {#lie-ix-s5-prop-2-cor-2 .statement tag=01E2}

Soient $ C $ une chambre de $ t $ et $ \overline{C} $ son adhérence. Les injections canoniques $ \overline{C} \to t \to g $ induisent par passage aux quotients des homéomorphismes
$$
\overline{C} \to t/W \to g/\mathrm{Ad}(G) .
$$
Les applications canoniques $ \overline{C} \to t $ et $ t \to t/W $ sont propres (TG, III, p. 28, prop. 2, c)). L’application $ \overline{C} \to t/W $ est continue, propre et bijective (prop. 2, c)); c’est donc un homéomorphisme, d’où le corollaire compte tenu du cor. à la prop. 6 du \S 2, n° 5.

#### Remarque 4 {#lie-ix-s5-n2-rem-4 .statement tag=01E3}

Notons $ g_{reg} $ l’ensemble des éléments réguliers de $ g $ (VII, \S 2, n° 2, déf. 2) et posons $ t_{reg} = t \cap g_{reg} $. Pour $ x \in t $, on a
$$
\det(X - \mathrm{ad}_g x) = X^{\dim t} \prod_{\alpha \in R(G, T)} (X - \delta(\alpha)(x)) ,
$$
et par suite $ t_{reg} $ est l’ensemble des éléments $ x $ de $ t $ tels que $ \delta(\alpha)(x) \neq 0 $ pour tout $ \alpha \in R(G, T) $, c’est-à-dire la réunion des chambres de $ t $ (de sorte que $ t_r \subset t_{reg} $). On a par conséquent $ \overline{C} \cap t_{reg} = C $, d’où des homéomorphismes
$$
C \to t_{reg}/W \to g_{reg}/\mathrm{Ad}(G) .
$$

#### Corollaire 3 {#lie-ix-s5-prop-2-cor-3 .statement tag=01E4}

Supposons $ G $ simplement connexe ; soit $ g $ un élément régulier de $ G $. Il existe un tore maximal $ S $ de $ G $ et une alcôve $ A $ de $ L(S) $, uniquement déterminés, tels que $ g \in \exp(A) $ et $ 0 \in \overline{A} $.

On peut supposer que $ g $ appartient à $ T_r $ (\S 2, n° 2, th. 2). Soit $ x $ un élément de $ t_r $ tel que $ \exp x = g $, et soit $ A' $ l’alcôve de $ t $ contenant $ x $. Les alcôves $ A $ de $ t $ telles que $ g \in \exp(A) $ sont les alcôves $ A' - \gamma $ pour $ \gamma \in \Gamma(T) $; l’assertion résulte donc de la prop. 2, d).

### 3. Automorphismes et éléments réguliers

#### Lemme 1 {#lie-ix-s5-lem-1 .statement tag=01E5}

Soient $ u $ un automorphisme de $ G $, et $ H $ l’ensemble de ses points fixes.
a) $ H $ est un sous-groupe fermé de $ G $.
b) Si $ H_0 $ est central dans $ G $, alors $ G $ est commutatif (donc $ G = T $).

L’assertion a) est claire. Pour démontrer b), on peut remplacer $ G $ par $ D(G) $ (\S 1, cor. 1 à la prop. 4), donc supposer $ G $ semi-simple. Alors, si $ H_0 $ est central dans $ G $, on a $ L(H) = \{ 0 \} $, de sorte que l’endomorphisme $ L(u) - \mathrm{Id} $ de $ g $ est bijectif. Soit $ f $ l’endomorphisme de la variété $ G $ défini par $ f(g) = u(g)^{-1}g $ pour $ g \in G $; il est étale, car si $ g \in G $ et $ x \in g $, on a $ T(f)(xg) = u(g)^{-1}(x - L(u)(x))g $, de sorte que l’application tangente à $ f $ en $ g $ est bijective. Il s’ensuit que l’image de $ f $ est ouverte et compacte, donc coïncide avec $ G $ puisque $ G $ est connexe. Soient alors $ E $ un épinglage de $ G $ ($ \S $ 4, n° 10, déf. 3) et $ u(E) $ son image par $ u $. D’après la prop. 19 de loc. cit., il existe un élément $ h $ de $ G $ tel que $ (\mathrm{Int}\ h)\ (E) = u(E) $. Soit $ g \in G $ tel que $ h = f(g) = u(g)^{-1}g $; on a
$$
u \circ \mathrm{Int}\ g = (\mathrm{Int}\ u(g)) \circ u = \mathrm{Int}\ g \circ (\mathrm{Int}\ h)^{-1} \circ u ,
$$
donc l’épinglage $ (\mathrm{Int}\ g)\ (E) $ est stable par $ u $. Si $ (\mathrm{Int}\ g)\ (E) = (T_1, B, (U_\alpha)_{\alpha \in B}) $, on a donc $ \sum U_\alpha \in L(H) $; comme $ L(H) = \{0\} $, cela implique $ B = \varnothing $, donc $ G = T_1 $, et $ G $ est commutatif.

#### Lemme 2 {#lie-ix-s5-lem-2 .statement tag=01E6}

*Soient x un élément de T et S un sous-tore de T. Si la composante neutre de Z(x) ∩ Z(S) est réduite à T, il existe un élément s de S tel que xs soit régulier.*

Pour tout $ \alpha $ dans $ R(G, T) $, soit $ S_\alpha $ la sous-variété de $ S $ formée des éléments $ s $ de $ S $ tels que l’on ait $ (xs)^\alpha = 1 $. S’il n’existe aucun élément $ s $ de $ S $ tel que $ xs $ soit régulier, $ S $ est la réunion des sous-variétés $ S_\alpha $, donc est égale à l’une d’elles. Il existe alors $ \alpha $ dans $ R(G, T) $ tel que $ (xs)^\alpha = 1 $ pour tout $ s \in S $; mais cela implique $ x^\alpha = 1 $ et $ \alpha|S = 1 $, donc $ Z(x) \cap Z(S) \supseteq Z(\mathrm{Ker}\ \alpha) $, d’où le lemme.

#### Lemme 3 {#lie-ix-s5-lem-3 .statement tag=01E7}

*Supposons G simplement connexe. Soient C une chambre de t, et u un automorphisme de G tel que T et C soient stables pour u. Alors l’ensemble des points de T fixés par u est connexe.*

Puisque $ G $ est simplement connexe, $ \Gamma(T) $ est engendré par les vecteurs nodaux $ K_\alpha $ ($ \alpha \in R(G, T) $), donc admet comme base la famille des $ K_\alpha $, lorsque $ \alpha $ parcourt la base $ B(C) $ définie par $ C $ (VI, § 1, n° 10). Il suffit donc de prouver que si $ \varphi $ est un automorphisme du tore $ T $ laissant stable une base de $ \Gamma(T) $, l’ensemble des points fixes de $ \varphi $ est connexe. Décomposant cette base en réunion disjointe d’orbites du groupe engendré par $ \varphi $, on se ramène au cas où $ T = \mathbf{U}^n $ et où $ \varphi $ est l’automorphisme $ (z_1, ..., z_n) \mapsto (z_2, ..., z_n, z_1) $; en ce cas les points fixes de $ \varphi $ sont les points $ (z, z, ..., z) $ pour $ z \in \mathbf{U} $, qui forment un sous-groupe connexe de $ T $.

#### Proposition 3 {#lie-ix-s5-prop-3 .statement tag=01E8}

*Soit u un automorphisme de G, et soit x un point de G fixé par u.*
a) *Il existe un élément a de g, fixé par L(u) et par Ad x, tel que x exp a soit régulier.*
b) *Il existe un élément régulier g de G fixé par u et commutant à x.*

Soient $ H $ le groupe des points fixes de $ u $, $ S $ un tore maximal de $ Z(x) \cap H $, et $ K $ la composante neutre de $ Z(S) \cap Z(x) $. C’est un sous-groupe fermé connexe de $ G $; par ailleurs, d’après le cor. 5 au th. 2 du § 2, n° 2, il existe des tores maximaux de $ G $ contenant $ S $ et $ x $, donc $ K $ est de rang maximum et contient $ S $ et $ x $. D’autre part, $ K $ est stable pour $ u $ puisque $ S $ et $ x $ le sont ; notons $ V $ l’ensemble des points fixes de $ u $ dans $ K $. On a alors
$$
S \subset V_0 \subset K \cap H \subset Z(S) \cap Z(x) \cap H ,
$$
donc $ V_0 $ est contenu dans le centralisateur de $ S $ dans $ (Z(x) \cap H)_0 $; mais ce dernier est réduit à $ S $ (*loc. cit.*, cor. 6), d’où finalement $ V_0 = S $. Le lemme 1 entraîne alors que $ K $ est commutatif, donc est un tore maximal de $ G $ (puisqu’il est connexe et de rang maximum). Il contient S et x, et est égal à la composante neutre de Z(S) ∩ Z(x); l’assertion a) résulte alors du lemme 2. On en déduit b) en prenant g = x exp a.

#### Corollaire {#lie-ix-s5-n3-cor-1 .statement tag=01E9}

Soit s une algèbre de Lie compacte, et soit φ un automorphisme de s. Il existe un élément régulier de s fixé par φ.

Quitte à remplacer s par $ \mathcal{D}s $, on peut supposer s semi-simple. Soit S un groupe de Lie compact simplement connexe d’algèbre de Lie s, et soit u l’automorphisme de S tel que L(u) = φ. La prop. 3 entraîne l’existence d’un élément a de s, fixé par φ, tel que exp a soit régulier dans S ; en particulier a est régulier dans s (n° 2, remarque 4).

#### Théorème 1 {#lie-ix-s5-thm-1 .statement tag=01EA}

Soit u un automorphisme du groupe de Lie compact connexe G.
a) La composante neutre du groupe des points fixes de u contient un élément régulier de G.
b) Il existe un tore maximal K de G et une chambre de L(K) stables par u.
c) Si G est simplement connexe, l’ensemble des points fixes de u est connexe.

L’assertion a) est le cas particulier x = e de la prop. 3. Supposons maintenant G simplement connexe et démontrons b) et c). Soit x un élément de G fixé par u, et soit g un élément régulier de G, fixé par u et commutant à x (prop. 3). Le centralisateur K de g est un tore maximal de G (n° 2, remarque 2), stable par u, contenant x et g. D’après le cor. 3 à la prop. 2 du n° 2, il existe une unique alcôve A de L(K) telle que $ g \in \exp(A) $ et $ 0 \in \overline{A} $; comme g est fixé par u, L(u) laisse stable A, donc aussi la chambre de L(K) qui contient A. Cela démontre b) ; par ailleurs, l’ensemble des points de K fixés par u est connexe (lemme 3) et contient x et e, d’où c) (TG, I, p. 81, prop. 2).

Il nous reste à démontrer b) dans le cas général. Or, si $ \tilde{D}(G) $ est le revêtement universel de D(G), et si $ f : \tilde{D}(G) \to G $ est le morphisme canonique, il existe un automorphisme $ \tilde{u} $ de $ \tilde{D}(G) $ tel que $ f \circ \tilde{u} = u \circ f $. Si $ \tilde{K} $ est un tore maximal de $ \tilde{D}(G) $ et $ \tilde{C} $ une chambre de L($ \tilde{K} $), stables pour $ \tilde{u} $(il en existe d’après ce qui a déjà été démontré), il existe (\S 2, n° 3, remarque 2) un unique tore maximal K de G et une unique chambre C de L(K) tels que $ \tilde{K} = f^{-1}(K) $ et $ \tilde{C} = L(f)^{-1}(C) $, et on voit aussitôt que K et C sont stables pour u, d’où l’assertion b) dans le cas général.

#### Corollaire 1 {#lie-ix-s5-thm-1-cor-1 .statement tag=01EB}

Supposons le $ \mathbf{Z} $-module $ \pi_1(G) $ sans torsion.
a) Le centralisateur de tout élément de G est connexe.
b) Deux éléments de G qui commutent appartiennent à un même tore maximal.

D’après le cor. 3 à la prop. 11 du § 4, n° 6, D(G) est simplement connexe. On a $ G = C(G)_0 . D(G) $; soit $ x \in G $; écrivons $ x = uv $, avec $ u \in C(G)_0 $ et $ v \in D(G) $. Alors $ Z(x) = C(G)_0 . Z_{D(G)}(v) $. D’après le th. 1, c), $ Z_{D(G)}(v) $ est connexe, donc $ Z(x) $ est connexe, d’où a). D’après le cor. 3 au th. 2 du § 2, n° 2, Z(x) est donc la réunion des tores maximaux de G contenant x, d’où b).

#### Corollaire 2 {#lie-ix-s5-thm-1-cor-2 .statement tag=01EC}

Soit $ \Gamma $ un sous-groupe compact de Aut(G) possédant la propriété suivante :
(*) Il existe des éléments $ u_1, ..., u_n $ de $ \Gamma $ tels que, pour tout i, l’adhérence $ \Gamma_i $ du sous-groupe de $ \Gamma $ engendré par $ u_1, ..., u_i $ soit un sous-groupe distingué de $ \Gamma $, et qu’on ait $ \Gamma_n = \Gamma $.

Alors il existe un tore maximal de $ G $ stable pour l’action de $ \Gamma $.

Raisonnons par récurrence sur la dimension de $ G $. On peut évidemment supposer que $ u_1 \neq \mathrm{Id} $; alors le sous-groupe $ H $ des points fixes de $ u_1 $ est distinct de $ G $, et est stable pour l’action de $ \Gamma $. De plus, puisque $ \Gamma $ est compact, l’image de $ \Gamma $ dans $ \mathrm{Aut}(H_0) $ est un quotient de $ \Gamma $, donc satisfait aussi à la condition (*). D’après l’hypothèse de récurrence, il existe un tore maximal $ S $ de $ H $ stable par $ \Gamma $. Le centralisateur $ K $ de $ S $ dans $ G $ est connexe (\S 2, n° 2, cor. 5) et stable par $ \Gamma $; c’est un tore maximal de $ G $, puisque $ H_0 $ contient un élément régulier de $ G $ (th. 1, *a*)) et que celui-ci est conjugué à un élément de $ S $ (*loc. cit.*, cor. 4).

#### Corollaire 3 {#lie-ix-s5-thm-1-cor-3 .statement tag=01ED}

Soient $ H $ un groupe de Lie et $ \Gamma $ un sous-groupe compact de $ H $. On suppose que $ H_0 $ est compact et que $ \Gamma $ satisfait à la condition (*) du cor. 2. Il existe alors un tore maximal $ T $ de $ H_0 $ tel que $ \Gamma \subset N_H(T) $.

#### Corollaire 4 {#lie-ix-s5-thm-1-cor-4 .statement tag=01EE}

Tout sous-groupe nilpotent d’un groupe de Lie compact est contenu dans le normalisateur d’un tore maximal.

Soient $ H $ un groupe de Lie compact, $ N $ un sous-groupe nilpotent de $ H $. Alors l’adhérence $ \Gamma $ de $ N $ est aussi un groupe nilpotent (III, § 9, n° 1, cor. 2 à la prop. 1), et il suffit, vu le cor. 3, de prouver que $ \Gamma $ satisfait à la condition (*). Or $ \Gamma_0 $ est un groupe de Lie compact connexe nilpotent, donc est un tore (\S 1, n° 4, cor. 1 à la prop. 4), et il existe un élément $ u_1 $ de $ \Gamma_0 $ engendrant un sous-groupe dense de $ \Gamma_0 $ (TG, VII, p. 8, texte précédant la prop. 8). Le groupe fini $ \Gamma/\Gamma_0 $ est nilpotent et il existe $ \tilde{u}_2, ..., \tilde{u}_n \in \Gamma/\Gamma_0 $ engendrant $ \Gamma/\Gamma_0 $ et tels que le sous-groupe de $ \Gamma/\Gamma_0 $ engendré par $ (\tilde{u}_2, ..., \tilde{u}_r) $ soit distingué pour $ r = 2, ..., n $ (A, I, p. 73, th. 1 et p. 76, th. 4). Alors, si $ u_2, ..., u_n $ sont des représentants de $ \tilde{u}_2, ..., \tilde{u}_n $ dans $ \Gamma $, la suite $ (u_1, ..., u_n) $ possède la propriété exigée.

#### Exemple {#lie-ix-s5-n3-exa-1 .statement tag=01EF}

Prenons $ G = U(n, \mathbf{C}) $. Nous verrons plus loin que le sous-groupe des matrices diagonales de $ G $ est un tore maximal de $ G $ et que son normalisateur est l’ensemble des matrices monomiales (A, II, p. 151) de $ G $.

On en conclut que si $ \Phi $ est une forme hermitienne positive séparante sur un espace vectoriel complexe de dimension finie $ V $ et $ \Gamma $ un sous-groupe nilpotent de $ U(\Phi) $, il existe une base de $ V $ pour laquelle les matrices des éléments de $ \Gamma $ sont monomiales (« théorème de Blichfeldt »).

### 4. Les applications $ (G/T) \times T \to G $ et $ (G/T) \times A \to G_r $

L’application $ (g, t) \mapsto gtg^{-1} $ de $ G \times T $ dans $ G $ induit par passage au quotient un morphisme de variétés analytiques

$$
f : (G/T) \times T \to G,
$$

qui est surjectif (\S 2, n° 2, th. 2). Par restriction, $ f $ induit un morphisme surjectif

$$
f_r : (G/T) \times T_r \to G_r.
$$

Par composition avec $ \mathrm{Id}_{G/T} \times \exp_T $, on en déduit des morphismes, également surjectifs
$$
\varphi : (G/T) \times t \to G,
$$
$$
\varphi_r : (G/T) \times t_r \to G_r;
$$
enfin, si $ A $ est une alcôve de $ t $, on déduit de $ \varphi_r $ un morphisme surjectif
$$
\varphi_A : (G/T) \times A \to G_r.
$$

On définit une opération à droite de $ W $ dans $ G/T $ comme suit : soient $ w \in W $ et $ u \in G/T $; relevons $ w $ en un élément $ n $ de $ N_G(T) $ et $ u $ en un élément $ g $ de $ G $. Alors l’image de $ gn $ dans $ G/T $ ne dépend pas du choix de $ n $ et $ g $; on la note $ u.w $.

Pour cette opération, $ W $ opère librement dans $ G/T $ : avec les notations précédentes, supposons en effet $ u.w = u $; alors $ gn \in gT $, donc $ n \in T $ et $ w = 1 $.

On définit une opération à droite de $ W $ dans $ (G/T) \times T $ par
$$
(u, t).w = (u.w, w^{-1}(t)) , \quad u \in G/T, \quad t \in T, \quad w \in W
$$
et une opération à droite de $ W'_a $ dans $ (G/T) \times t $ par
$$
(u, x).\omega = (u.\overline{\omega}, \omega^{-1}(x)) , \quad u \in G/T, \quad x \in t, \quad \omega \in W'_a,
$$
où $ \overline{\omega} $ est l’image de $ \omega $ dans le quotient $ W'_a/\Gamma(T) = W $.

Si $ A $ est une alcôve de $ t $, et si $ H_A $ est le sous-groupe de $ W'_a $ qui stabilise $ A $, on obtient par restriction une opération de $ H_A $ sur $ (G/T) \times A $.

Ces différentes opérations sont compatibles avec les morphismes $ f $, $ \varphi $ et $ \varphi_A $ : pour $ u \in G/T, t \in T, x \in t, y \in A, w \in W, \omega \in W'_a, h \in H_A $, on a
$$
f((u, t).w) = f(u, t) , \quad \varphi((u, x).\omega) = \varphi(u, x) , \quad \varphi_A((u, y).h) = \varphi_A(u, y) .
$$

#### Lemme 4 {#lie-ix-s5-lem-4 .statement tag=01EG}

*Soient $ g \in G, t \in T $, et soit $ \overline{g} $ l’image de $ g $ dans $ G/T $. Identifions l’espace tangent à $ G/T $ (resp. $ T $, resp. $ G $) en $ \overline{g} $ (resp. $ t $, resp. $ gtg^{-1} $) à $ g/t $ (resp. $ t $, resp. $ g $) par la translation à gauche $ \gamma(g) $ par $ g $ (resp. $ t $, resp. $ gtg^{-1} $). L’application linéaire tangente à $ f $ en $ (\overline{g}, t) $ s’identifie alors à l’application $ f' : (g/t) \times t \to g $ définie comme suit : si $ z \in g, x \in t $, et si $ \overline{z} $ désigne l’image de $ z $ dans $ g/t $, on a*
$$
f'(\overline{z}, x) = (\mathrm{Ad}\ gt^{-1}) (z - (\mathrm{Ad}\ t)\ z + x) .
$$

Soit $ F $ l’application de $ G \times T $ dans $ T $ telle que $ F(g, t) = gtg^{-1} $. Comme $ F \circ (\gamma(g), \mathrm{Id}_T) = \mathrm{Int}\ g \circ F $, on a $ T_{(g,t)}(F)(gz, tx) = T_t(\mathrm{Int}\ g) \circ T_{(e,t)}(F)(z, tx) $; d’après III, § 3, no 12, prop. 46, on a
$$
T_{(e,t)}(F)(z, tx) = t((\mathrm{Ad}\ t^{-1})\ z - z) + tx = t((\mathrm{Ad}\ t^{-1})\ (z - (\mathrm{Ad}\ t)\ z + x))
$$

et par conséquent

$$
T_{(g,t)}(F)(gz, tx) = gtg^{-1}((\mathrm{Ad}\ gt^{-1})(z - (\mathrm{Ad}\ t)\ z + x)) .
$$

Le lemme résulte aussitôt de cette formule par passage au quotient.

#### Proposition 4 {#lie-ix-s5-prop-4 .statement tag=01EH}

a) Soient $ g \in G $, $ t \in T $, $ x \in t $, et soit $ \overline{g} $ l'image de $ g $ dans $ G/T $. Les conditions suivantes sont équivalentes:
(i) On a $ t \in T_r $ (resp. $ x \in t_r $).
(i bis) L'élément $ f(\overline{g}, t) $ (resp. $ \varphi(\overline{g}, x) $) est régulier dans $ G $.
(ii) L'application $ f $ (resp. $ \varphi $) est une submersion au point $ (\overline{g}, t) $ (resp. $ (\overline{g}, x) $).
(ii bis) L'application $ f $ (resp. $ \varphi $) est étale au point $ (\overline{g}, t) $ (resp. $ (\overline{g}, x) $).
b) L'application $ f_r $ (resp. $ \varphi_r $, resp. $ \varphi_A $) fait de $ (G/T) \times T_r $ (resp. $ (G/T) \times t_r $, resp. $ (G/T) \times A $) un revêtement principal de $ G_r $ de groupe $ W $ (resp. $ W'_a $, resp. $ H_A $).

a) L'équivalence de (i) et (i bis) est claire ; celle de (ii) et (ii bis) résulte des relations $ \dim((G/T) \times T) = \dim((G/T) \times t) = \dim(G) $. D'après le lemme 4, $ f $ est une submersion au point $ (\overline{g}, t) $ si et seulement si $ g = t + \mathrm{Im}(\mathrm{Ad}\ t - \mathrm{Id}) $, ce qui signifie que $ t $ est régulier. Enfin puisque $ \varphi = f \circ (\mathrm{Id}_{G/T} \times \exp_T) $, $ \varphi $ est étale au point $ (\overline{g}, x) $ si et seulement si $ f $ est étale au point $ (\overline{g}, \exp x) $, ce qui signifie d'après ce qui précède que $ x $ appartient à $ t_r $.

b) Les morphismes $ f_r, \varphi_r, \varphi_A $ sont donc étales. D'autre part $ W $ opère librement dans $ G/T $, et a fortiori dans $ (G/T) \times T $. Soient $ g, g' $ dans $ G $ et $ t, t' $ dans $ T_r $ tels que $ f(\overline{g}, t) = f(\overline{g'}, t') $; alors $ \mathrm{Int}\ g^{-1}g' $ applique $ t' $ sur $ t $, donc normalise $ T $, puisque $ T = Z(t)_0 = Z(t')_0 $, et la classe $ w $ de $ g^{-1}g' $ dans $ W $ applique $ (\overline{g}, t) $ sur $ (\overline{g'}, t') $. Il s'ensuit que $ f_r $ est un revêtement principal de groupe $ W $; cela implique aussitôt que $ \varphi_r $ est un revêtement principal de groupe $ W'_a $, donc par restriction à la composante connexe $ (G/T) \times A $ de $ (G/T) \times t_r $, que $ \varphi_A $ est un revêtement principal de groupe $ H_A $.

#### Remarque 1 {#lie-ix-s5-n4-rem-1 .statement tag=01EI}

D'après la prop. 3 du § 2, n° 4, la variété $ (G/T) \times A $ est simplement connexe. Il en résulte que $ \varphi_A $ est un revêtement universel de $ G_r $; comme $ \pi_1(G_r) $ est canoniquement isomorphe à $ \pi_1(G) $ (n° 1, prop. 1 et TG, XI, à paraître), on retrouve ainsi le fait que $ \pi_1(G) $ s'identifie à $ H_A $ (c'est-à-dire à $ \Gamma(T)/N(G, T) $).

#### Remarque 2 {#lie-ix-s5-n4-rem-2 .statement tag=01EJ}

La restriction de $ \varphi_A $ à $ W \times A \subset (G/T) \times A $ fait de $ W \times A $ un revêtement principal de $ T_r $ de groupe $ H_A $. On retrouve ainsi le cor. 1 à la prop. 2 du n° 2.

#### Remarque 3 {#lie-ix-s5-n4-rem-3 .statement tag=01EK}

Notons $ g_r $ l'image réciproque de $ G_r $ par l'application exponentielle et $ \varepsilon : g_r \to G_r $ l'application déduite de $ \exp_G $. L'application $ (g, x) \mapsto (\mathrm{Ad}\ g)(x) $ de $ G \times t_r $ dans $ g_r $ définit par passage au quotient une application $ \psi_r : (G/T) \times t_r \to g_r $. On a $ \varepsilon \circ \psi_r = \varphi_r $. Soient $ w \in W,\ \gamma \in \Gamma(T) $ et $ \omega \in W'_a $ tels que $ \omega(z) = w(z) + \gamma $ pour tout $ z \in t $; on a $ \psi_r((\overline{g}, x)\ \omega) = \psi_r(\overline{g}, x) - (\mathrm{Ad}\ g)(\gamma) $ pour $ g \in G,\ x \in t_r $, de sorte que $ \psi_r((\overline{g}, x)\ \omega) = \psi_r(\overline{g}, x) $ si et seulement si $ \gamma = 0 $. Il en résulte (cf. TG, XI, à paraître) que $ \psi_r $ est un revêtement principal de $ g_r $ de groupe $ W $, et que $ \varepsilon : g_r \to G_r $ est un revêtement associable au revêtement principal $ \varphi_r $, de fibre isomorphe au $ W'_a $-ensemble $ W'_a/W $.

## EXERCICES {#lie-ix-s5-exercises}

See the [exercises for § 5](exercises/s5/).
