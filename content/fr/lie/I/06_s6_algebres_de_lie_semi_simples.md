---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 6
section_title: Algèbres de Lie semi-simples
lang: fr
source: lie-i-fr
pdf_pages: 0069-0093, 0126-0133
extraction: ocr
subsections:
    - "no": 1
      title: Définition des algèbres de Lie semi-simples
      page: 0
      pdf_page: 69
    - "no": 2
      title: Semi-simplicité des représentations
      page: 0
      pdf_page: 70
    - "no": 3
      title: Éléments semi-simples et éléments nilpotents dans les algèbres de Lie semi-simples
      page: 0
      pdf_page: 74
    - "no": 4
      title: Algèbres de Lie réductives
      page: 0
      pdf_page: 76
    - "no": 5
      title: 'Application : un critère de semi-simplicité pour les représentations'
      page: 0
      pdf_page: 79
    - "no": 6
      title: Sous-algèbres réductives dans une algèbre de Lie
      page: 0
      pdf_page: 81
    - "no": 7
      title: Exemples d’algèbres de Lie semi-simples
      page: 0
      pdf_page: 82
    - "no": 8
      title: Le théorème de Levi-Malcev
      page: 0
      pdf_page: 85
    - "no": 9
      title: Le théorème des invariants
      page: 0
      pdf_page: 90
    - "no": 10
      title: Changement du corps de base
      page: 0
      pdf_page: 92
statements: 53
exercises: 27
content_sha256: 12a8e1e35979b273b24406deeb948dd75e2fd0c51b842d10a7a205ecfe80871d
---

## § 6. Algèbres de Lie semi-simples

On rappelle que K désigne un corps de caractéristique 0 et que toutes les algèbres de Lie sont supposées de dimension finie sur K.

### 1. Définition des algèbres de Lie semi-simples

#### Définition 1 {#lie-i-s6-def-1 .statement}

Soit g une algèbre de Lie. On dit que g est semi-simple si le seul idéal commutatif de g est {0}.

#### Remarque 1 {#lie-i-s6-n1-rem-1 .statement}

L’algèbre {0} est semi-simple. Une algèbre de dimension 1 ou 2 est non semi-simple (cf. § 5, no 1, exemple 1). Il existe des algèbres semi-simples de dimension 3 (cf. n° 7).

#### Remarque 2 {#lie-i-s6-n1-rem-2 .statement}

Une algèbre semi-simple a un centre nul, donc sa représentation adjointe est fidèle.

#### Remarque 3 {#lie-i-s6-n1-rem-3 .statement}

Si g₁, ..., gₙ sont semi-simples, g = g₁ × ... × gₙ est semi-simple ; car, si a est un idéal commutatif de g, les projections de a sur g₁, ..., gₙ sont réduites à {0}.

#### Théorème 1 {#lie-i-s6-thm-1 .statement}

Soit g une algèbre de Lie. Les conditions suivantes sont équivalentes :

a) g est semi-simple.
b) Le radical r de g est nul.
c) La forme de Killing β de g est non dégénérée.

En outre, une algèbre de Lie semi-simple est égale à son idéal dérivé.

a) ⇒ b) : car, si r ≠ {0}, la dernière algèbre dérivée non nulle de r est un idéal commutatif de g.

b) ⇒ c) : ceci résulte de la prop. 5 b) du § 5, n° 5 (qui prouve en même temps la dernière assertion du théorème).

c) ⇒ a) : ceci résulte de la prop. 6 b) du § 4, n° 4.

#### Corollaire {#lie-i-s6-n1-cor-1 .statement}

Soient g une algèbre de Lie semi-simple, ρ une représentation de g dans un espace V de dimension finie. Alors, ρ(g) ⊂ sl(V).

En effet, la forme linéaire x ↦ Tr ρ(x) (x ∈ g) s’annule quand x est de la forme [y, z] (y ∈ g, z ∈ g), donc sur 𝔤 = g.

#### Proposition 1 {#lie-i-s6-prop-1 .statement}

Soient $ g $ une algèbre de Lie semi-simple, $ \rho $ une représentation fidèle de dimension finie de $ g $. Alors la forme bilinéaire sur $ g $ associée à $ \rho $ est non dégénérée.

En effet, l’orthogonal de $ g $ pour cette forme est un idéal résoluble ($ \S 5 $, no 4, th. 2), donc est nul.

#### Corollaire 1 {#lie-i-s6-prop-1-cor-1 .statement}

Soient $ g $ une algèbre de Lie, $ \beta $ sa forme de Killing, $ a $ une sous-algèbre semi-simple de $ g $. L’orthogonal $ h $ de $ a $ par rapport à $ \beta $ est un sous-espace supplémentaire de $ a $ dans $ g $, et on a $[a, h]) \subset h$. Si $ a $ est un idéal de $ g $, il en est de même de $ h $, qui est alors le commutant de $ a $ dans $ g $.

Soit $ \beta' $ la restriction de $ \beta $ à $ a $ : c’est la forme bilinéaire associée à la représentation $ x \to \mathrm{ad}_g x $ de $ a $ dans l’espace $ g $. Cette représentation est fidèle, donc $ \beta' $ est non dégénérée (prop. 1). Donc $ h $ est supplémentaire de $ a $ dans $ g $. Par ailleurs, si $ x, y $ sont dans $ a $ et $ z \in h $, on a $ \beta(x, [y, z]) = \beta([x, y], z) = 0 $, car $[x, y] \in a $, donc $[y, z] \in h $, ce qui prouve que $[a, h]) \subset h $. Si $ a $ est un idéal de $ g $, on sait que $ h $ est un idéal de $ g $ ($ \S 3 $, prop. 7) et $ g $ s’identifie à $ a \times h $. Comme le centre de $ a $ est nul, le commutant de $ a $ dans $ g $ est $ h $.

#### Corollaire 2 {#lie-i-s6-prop-1-cor-2 .statement}

Toute extension d’une algèbre de Lie semi-simple par une algèbre de Lie semi-simple est semi-simple et triviale.

Ceci résulte aussitôt du cor. 1.

#### Corollaire 3 {#lie-i-s6-prop-1-cor-3 .statement}

Si $ g $ est semi-simple, toute dérivation de $ g $ est intérieure.

En effet, $ \mathrm{ad}\, g $ est isomorphe à $ g $, donc semi-simple, et est un idéal de l’algèbre de Lie $ \mathfrak{d} $ des dérivations de $ g $ ($ \S 1 $, prop. 1). Si $ D \in \mathfrak{d} $ commute aux éléments de $ \mathrm{ad}\, g $, on a, pour tout $ x \in g $, $ \mathrm{ad}\, D(x) = [D, \mathrm{ad}\, x] = 0 $, d’où $ D(x) = 0 $; donc $ D = 0 $. Le cor. 3 résulte donc du cor. 1.

### 2. Semi-simplicité des représentations

#### Lemme 1 {#lie-i-s6-lem-1 .statement}

Soit $ g $ une algèbre de Lie semi-simple. La représentation adjointe de $ g $ est semi-simple. Tout idéal et toute algèbre quotient de $ g $ est semi-simple.

En effet, soit $ a $ un idéal de $ g $. L’orthogonal $ b $ de $ a $ dans $ g $ pour la forme de Killing est un idéal de $ g $, et $ a \cap b $ est un idéal commutatif ($ \S 3 $, no 6, prop. 7), donc nul. Donc $ b $ est supplémentaire de $ a $ dans $ g $. En outre, comme la forme de Killing de $ g $ est non dégénérée, il en est de même de ses restrictions à $ a $ et $ b $ (*Alg.*, chap. IX, $ \S 4 $, no 1, cor. de la prop. 1), donc $ a $ et $ b $ sont semi-simples (no 1, th. 1, et $ \S 3 $, no 6, prop. 9).

#### Lemme 2 {#lie-i-s6-lem-2 .statement}

*Soit $ g $ une algèbre de Lie. Alors les deux conditions suivantes sont équivalentes* :

a) *Toutes les représentations linéaires de dimension finie de $ g $ sont semi-simples*.

b) *Etant donnés une représentation linéaire $ \rho $ de $ g $ dans un espace vectoriel $ V $ de dimension finie et un sous-espace vectoriel $ W $ de codimension 1 tel que $ \rho(x)(V) \subset W $ pour tout $ x \in g $, il existe une droite supplémentaire de $ W $ stable pour $ \rho(g) $ (donc annulée par $ \rho(g) $).

Il est clair que $ a) $ entraîne $ b) $. Supposons $ b) $ vraie. Soient $ \sigma $ une représentation de dimension finie de $ g $ dans un espace vectoriel $ M $, et $ N $ un sous-espace vectoriel stable pour $ \sigma(g) $. Soit $ \mu $ la représentation de $ g $ dans $ \mathcal{L}(M) $ canoniquement déduite de $ \sigma $ ($ \S 3 $, no 3) : rappelons que $ \mu(x) = \operatorname{ad}_{\mathcal{L}(M)} \sigma(x) $. Soit $ V $ (resp. $ W $) le sous-espace de $ \mathcal{L}(M) $ formé des applications linéaires de $ M $ dans $ N $ dont la restriction à $ N $ est une homothétie (resp. est nulle) ; alors $ W $ est de codimension 1 dans $ V $, et $ \mu(x)(V) \subset W $ pour tout $ x \in g $. D’après la condition $ b) $, il existe un $ u \in V $ annulé par $ \mu(x) $ pour tout $ x \in g $, et dont la restriction à $ N $ est une homothétie non nulle. En multipliant $ u $ par un scalaire convenable, on peut supposer que $ u $ est un projecteur de $ M $ sur $ N $. Dire que $ \mu(x) \cdot u = 0 $ signifie que $ u $ est permutable à $ \sigma(x) $. Donc le noyau de $ u $ est un supplémentaire de $ N $ dans $ M $ stable pour $ \sigma(x) $, quel que soit $ x \in g $. Donc $ \sigma $ est semi-simple.

#### Lemme 3 {#lie-i-s6-lem-3 .statement}

*Soient $ g $ une algèbre de Lie semi-simple, $ \rho $ une représentation linéaire de $ g $ dans un espace vectoriel $ V $ de dimension finie et $ W $ un sous-espace de $ V $ de codimension 1 tel que $ \rho(x)(V) \subset W $ pour tout $ x \in g $. Alors il existe une droite supplémentaire de $ W $ stable pour $ \rho(g) $*.

Pour tout $ x \in g $, soit $ \sigma(x) $ la restriction de $ \rho(x) $ à $ W $. Supposons d’abord que $ \sigma $ soit simple. Si $ \sigma = 0 $, alors $ \rho(x)\rho(y) = 0 $ quels que

Dans le cas général, on raisonne par récurrence sur la dimension de $ V $. Soit $ T $ un sous-espace stable non nul minimal de $ W $. Soit $ \rho' $ la représentation quotient dans $ V' = V/T $. On a, pour tout $ x \in g $, $ \rho'(x)(V') \subset W' $, où $ W' = W/T $ est de codimension 1 dans $ V' $. Par l’hypothèse de récurrence, il existe une droite $ Z' $ supplémentaire de $ W' $ et stable pour $ \rho'(g) $. Son image réciproque $ Z $ dans $ V $ est stable pour $ \rho(g) $, contient $ T $ comme sous-espace de codimension 1, et on a $ Z \cap W = T $, donc $ \rho(x)(Z) \subset T $ pour tout $ x \in g $. D’après ce qui a été démontré plus haut, il existe une droite supplémentaire de $ T $ dans $ Z $, stable pour $ \rho(g) $ ; cette droite est supplémentaire de $ W $ dans $ V $, ce qui achève la démonstration.

#### Théorème 2 (H. Weyl) {#lie-i-s6-thm-2 .statement}

Toute représentation linéaire de dimension finie d’une algèbre de Lie semi-simple est complètement réductible.

Ceci résulte des lemmes 2 et 3.

#### Définition 2 {#lie-i-s6-def-2 .statement}

Une algèbre de Lie $ g $ est dite simple si les seuls idéaux de $ g $ sont $ \{0\} $ et $ g $ et si en outre $ g $ est non commutative.

Une algèbre de Lie simple est semi-simple. L’algèbre $ \{0\} $ n’est pas simple.

#### Proposition 2 {#lie-i-s6-prop-2 .statement}

Pour qu’une algèbre de Lie $ g $ soit semi-simple, il faut et il suffit qu’elle soit produit d’algèbres simples.

La condition est suffisante (no 1, remarque 3). Réciproquement, supposons $ g $ semi-simple. Puisque la représentation adjointe de $ g $ est semi-simple, $ g $ est somme directe d’idéaux non nuls minimaux $ a_1, \ldots, a_m $. Alors $ g $ s’identifie à l’algèbre produit des $ a_i $ ($ \S 1, \mathrm{n}^{\circ} 1 $). Tout idéal de $ a_i $ est alors un idéal de $ g $, donc nul ou égal à $ a_i $. Par ailleurs, $ a_i $ est non commutatif. Donc les $ a_i $ sont des algèbres de Lie simples.

#### Corollaire 1 {#lie-i-s6-prop-2-cor-1 .statement}

*Une algèbre de Lie semi-simple est le produit de ses idéaux simples $ g_i $. Tout idéal de $ g $ est produit de certains des $ g_i $.*

On a $ g = a_1 \times \cdots \times a_m $, où les $ a_i $ sont simples. Comme le centre de $ a_i $ est nul, le commutant de $ a_i $ dans $ g $ est le produit des $ a_j $ pour $ j \neq i $. Soit alors $ a $ un idéal de $ g $. S’il ne contient pas $ a_i $, on a $ a \cap a_i = \{0\} $, donc $[a, a_i] = \{0\}$, et $ a $ est contenu dans le produit des $ a_j $ pour $ j \neq i $. Il s’ensuit que $ a $ est produit de certains des $ a_i $. Donc les idéaux simples de $ g $ sont exactement les $ a_i $.

Les idéaux simples d’une algèbre de Lie semi-simple sont appelés les *composants simples* de $ g $.

#### Corollaire 2 {#lie-i-s6-prop-2-cor-2 .statement}

*Soient $ g, g' $ deux algèbres de Lie, $ r $ et $ r' $ leurs radicaux, et $ f $ un homomorphisme de $ g $ sur $ g' $. Alors $ r' = f(r) $.*

Comme $ f(r) $ est résoluble, on a $ f(r) \subset r' $. D’autre part, $ g/r $ est semi-simple ($ \S 5, \mathrm{n}^{\circ} 2 $, prop. 3), donc $ g'/f(r) $, qui est isomorphe à un quotient de $ g/r $, est semi-simple (lemme 1), donc $ f(r) \supset r' $ ($ \S 5, \mathrm{n}^{\circ} 2 $, prop. 3).

#### Remarque 1 {#lie-i-s6-n2-rem-1 .statement}

Le th. 2 admet une réciproque : si toute représentation de dimension finie de $ g $ est semi-simple, $ g $ est semi-simple. En effet, puisque la représentation adjointe est semi-simple, tout idéal de $ g $ admet un idéal supplémentaire, donc peut être considéré comme un quotient de $ g $. Si $ g $ n’est pas semi-simple, $ g $ admet donc un quotient commutatif non nul, et par suite un quotient de dimension 1. Or l’algèbre de Lie $ K $ de dimension 1 admet des représentations non semi-simples, par exemple

$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

#### Remarque 2 {#lie-i-s6-n2-rem-2 .statement}

Soient $ g $ une algèbre de Lie sur $ K $, et $ \sigma $ une représentation de $ g $ dans un espace vectoriel $ M $. Soit d’autre part $ f $ une application K-linéaire de g dans M telle que :

(1) $$ f([x, y]) = \sigma(x).f(y) - \sigma(y).f(x) $$

quels que soient x, y dans g. D’après le § 1, n° 8, exemple 2, la donnée de $ \sigma $ et $ f $ équivaut à la donnée d’un homomorphisme $ x \mapsto (f(x), \sigma(x)) $ de g dans $ \mathfrak{af}(M) $. On a vu d’autre part (loc. cit.) que l’élément $ (f(x), \sigma(x)) $ de $ \mathfrak{af}(M) $ s’identifie canoniquement à l’élément $ \rho(x) $ de $ \mathrm{gl}(N) $ (où $ N = M \times K $) qui induit $ \sigma(x) $ sur M et transforme l’élément $ (0, 1) $ de N en $ f(x) $. Et $ \rho $ est alors une représentation de g dans N telle que $ \rho(x)(N) \subset M $ pour tout $ x \in g $.

Ceci posé, si g est semi-simple, il existe (lemme 3) une droite Z supplémentaire de M dans N et annulée par $ \rho(g) $. Autrement dit, *il existe un élément $ m_0 \in M $ tel que $ (-m_0, 1) \in N $ soit annulé par $ \rho(x) $ pour tout $ x \in g $, c’est-à-dire tel que*

(2) $$ f(x) = \sigma(x).m_0 $$

pour tout $ x \in g $.

*Supposons $ K = \mathbf{R} $. Soit G un groupe de Lie connexe d’algèbre de Lie g. Considérons un homomorphisme analytique $ \varphi $ de G dans le groupe affine A de M, correspondant à un homomorphisme $ x \to (f(x), \sigma(x)) $ de g dans $ \mathfrak{af}(M) $. Les résultats précédents peuvent s’interpréter en disant que, si g est semi-simple, $ \varphi(G) $ laisse fixe un point de M. En effet, soit H l’ensemble des éléments de $ \mathbf{GL}(N) $ qui laissent stables toutes les variétés linéaires de N parallèles à M. Il existe (\$ 1, n° 8, exemple 2) un isomorphisme canonique $ \psi $ de A sur H. Soit Z une droite supplémentaire de M dans N. Dire que $ \rho(g) $ annule Z revient à dire que $ (\psi \circ \varphi)(G) $ laisse fixes les points de Z, donc (compte tenu de la définition de $ \psi $) que $ \varphi(G) $ laisse fixe la projection sur M du point d’intersection de Z et de $ M \times \{1\} $. \*

### 3. Éléments semi-simples et éléments nilpotents dans les algèbres de Lie semi-simples

#### Proposition 3 {#lie-i-s6-prop-3 .statement}

Soient M un espace vectoriel de dimension finie sur K, et g une sous-algèbre semi-simple de $ \mathrm{gl}(M) $. Alors g contient les composantes semi-simples et nilpotentes de ses éléments.

Si $ K_1 $ est une extension de $ K $, la forme de Killing de $ g_{(K_1)} $ est l’extension à $ g_{(K_1)} $ de celle de $ g $ (\$ 3, no 8), donc est non dégénérée ; par suite, $ g_{(K_1)} $ est semi-simple. Il suffit donc de démontrer la prop. 3 lorsque le corps de base est algébriquement clos, ce que nous supposons désormais.

Pour tout sous-espace $ N $ de $ M $, soit $ g_N $ la sous-algèbre de $ gl(M) $ formée des éléments qui laissent $ N $ stable, et dont la restriction à $ N $ est de trace nulle. Comme $ g = \mathcal{O}g $, on a $ g \subset g_N $ si $ N $ est stable par $ g $. Soit alors $ g^* $ l’intersection du normalisateur de $ g $ dans $ gl(M) $ et des algèbres $ g_N $ où $ N $ parcourt l’ensemble des sous-espaces de $ M $ stables par $ g $. Comme la composante semi-simple $ s $ (resp. nilpotente $ n $) de $ x \in gl(M) $ est un polynôme sans terme constant en $ x $, et que $ ad\ s $ (resp. $ ad\ n $) est la partie semi-simple (resp. nilpotente) de $ ad\ x $ (\$ 5, no 4, lemme 2), il est clair que $ x \in g^* $ implique $ s \in g^* $ et $ n \in g^* $; il suffit donc de faire voir que $ g^* = g $. Puisque $ g $ et un idéal semi-simple de $ g^* $, on a $ g^* = a \times g $ (no 1, cor. 1 de la prop. 1). Soit $ a \in a $ et soit $ N $ un sous-espace minimal parmi les sous-espaces non nuls de $ M $ stables par $ g $. La restriction de $ a $ à $ N $ est un multiple scalaire de l’identité d’après le th. de Burnside, de trace nulle par construction, donc est nulle puisque $ K $ est de caractéristique 0. Comme $ M $ est somme directe de sous-espaces tels que $ N $, il s’ensuit que $ a = 0 $, donc $ g^* = g $.

#### Corollaire {#lie-i-s6-n3-cor-1 .statement}

*Un élément $ x $ de $ g $ est un endomorphisme semi-simple (resp. nilpotent) de $ M $ si et seulement si $ ad_g\ x $ est un endomorphisme semi-simple (resp. nilpotent) de $ g $*.

Soit $ s $ (resp. $ n $) la composante semi-simple (resp. nilpotente) de $ x \in g $. On a $ s \in g $ et $ n \in g $ (prop. 3). Alors $ ad_g\ s $ (resp. $ ad_g\ n $) est la composante semi-simple (resp. nilpotente) de $ ad_g\ x $, d’après le lemme 2 du \$ 5, no 4. Si $ x $ est semi-simple (resp. nilpotent), il en est donc de même de $ ad_g\ x $. Si maintenant $ ad_g\ x $ est semi-simple (resp. nilpotent), il est égal à $ ad_g\ s $ (resp. $ ad_g\ n $), donc $ x = s $ (resp. $ x = n $) puisque la représentation adjointe de $ g $ est fidèle.

#### Définition 3 {#lie-i-s6-def-3 .statement}

*Soit $ g $ une algèbre de Lie semi-simple. Un élément $ x $ de $ g $ est dit semi-simple (resp. nilpotent) si, pour tout g-module M de dimension finie sur K, $ x_M $ est un endomorphisme semi-simple (resp. nilpotent) de M.

#### Proposition 4 {#lie-i-s6-prop-4 .statement}

Soient g, g' des algèbres de Lie semi-simples, et f un homomorphisme de g dans g'. Si $ x \in g $ est semi-simple (resp. nilpotent), $ f(x) $ l’est aussi. Si f est surjectif, tout élément semi-simple (resp. nilpotent) de g' est image par f d’un élément semi-simple (resp. nilpotent) de g.

Si $ \rho $ est une représentation de g', $ \rho \circ f $ est une représentation de g, d’où la première assertion. Si f est surjectif, il existe un homomorphisme g de g' dans g tel que $ f \circ g $ soit l’homomorphisme identique de g' (n° 1, cor. 2 de la prop. 1), et la deuxième assertion résulte donc de la première.

#### Théorème 3 {#lie-i-s6-thm-3 .statement}

Soit g une algèbre de Lie semi-simple.

a) Soit $ x \in g $. S’il existe une représentation fidèle de $ \rho $ de g telle que $ \rho(x) $ soit un endomorphisme semi-simple (resp. nilpotent), alors x est semi-simple (resp. nilpotent).

b) Tout élément de g s’écrit de manière unique comme somme d’un élément semi-simple et d’un élément nilpotent commutant entre eux.

Supposons satisfaite l’hypothèse de a). Soient $ \sigma $ une représentation de g, b l’idéal supplémentaire du noyau de $ \sigma $, et $ \alpha $ la projection de g sur b. Alors, $ \mathrm{ad}_g x $ est semi-simple (resp. nilpotent) d’après le cor. de la prop. 3, donc $ \mathrm{ad}_b \alpha(x) $ est semi-simple (resp. nilpotent). Comme $ \sigma(x) = \sigma(\alpha(x)) $, la première assertion résulte du cor. de la prop. 3. La deuxième résulte alors de la prop. 3 appliquée à une représentation fidèle.

### 4. Algèbres de Lie réductives

#### Définition 4 {#lie-i-s6-def-4 .statement}

Une algèbre de Lie est dite réductive si sa représentation adjointe est semi-simple.

#### Proposition 5 {#lie-i-s6-prop-5 .statement}

Soient g une algèbre de Lie, r son radical. Les conditions suivantes sont équivalentes :

a) g est réductive.
b) $ \mathcal{O}g $ est semi-simple.

c) $ g $ est produit d’une algèbre semi-simple et d’une algèbre commutative.

d) $ g $ possède une représentation de dimension finie telle que la forme bilinéaire associée soit non dégénérée.

e) $ g $ possède une représentation de dimension finie semi-simple fidèle.

f) *Le radical nilpotent de $ g $ est nul.*

g) $ r $ est le centre de $ g $.

a) $ \Rightarrow b) $ : si la représentation adjointe de $ g $ est semi-simple, $ g $ est somme directe d’idéaux non nuls minimaux $ a_i $, donc $ g $ est isomorphe au produit des $ a_i $; et $ a_i $ ne possède pas d’autre idéaux que $ \{0\} $ et $ a_i $, donc est simple ou commutatif de dimension 1. Par suite, $ \mathcal{O}g $ est égal au produit de ceux des $ a_i $ qui sont simples, donc est semi-simple.

$ b) \Rightarrow c) $ : si $ \mathcal{O}g $ est semi-simple, $ g $ est isomorphe au produit de $ \mathcal{O}g $ par une algèbre de Lie $ h $ (no 1, cor. 1 de la prop. 1); $ h $ est isomorphe à $ g/\mathcal{O}g $, donc commutative.

$ c) \Rightarrow d) $ : soient $ g_1 $ et $ g_2 $ deux algèbres de Lie, $ \rho_i $ une représentation de dimension finie de $ g_i $, $ \beta_i $ la forme bilinéaire sur $ g_i $ associée à $ \rho_i $ ($ i = 1, 2 $); on peut considérer $ \rho_1 $ et $ \rho_2 $ comme des représentations de $ g = g_1 \times g_2 $; soit $ \rho $ leur somme directe. Il est clair que la forme bilinéaire sur $ g $ associée à $ \rho $ est la somme directe de $ \beta_1 $ et $ \beta_2 $, donc est non dégénérée si $ \beta_1 $ et $ \beta_2 $ sont non dégénérées. Ceci posé, pour prouver l’implication $ c) \Rightarrow d) $, il suffit de considérer les 2 cas suivants : 1) $ g $ est semi-simple ; alors la représentation adjointe admet pour forme associée la forme de Killing, qui est non dégénérée ; 2) $ g = K $; alors la représentation identique de $ g $ dans $ K $ a une forme bilinéaire associée qui est non dégénérée.

$ d) \Rightarrow e) $ : soient $ \rho $ une représentation de dimension finie de $ g $ et $ \beta $ la forme bilinéaire associée ; d’après la prop. 4 du § 4, no 3, il existe une représentation semi-simple de dimension finie $ \sigma $ de $ g $ telle que le noyau $ n $ de $ \sigma $ soit orthogonal à $ g $ pour $ \beta $. Si $ \beta $ est non dégénérée, on a $ n = \{0\} $, donc $ \sigma $ est fidèle.

$ e) \Rightarrow f) $ : ceci est évident.

$ f) \Rightarrow g) $ : si le radical nilpotent de $ g $ est nul, $ \mathcal{O}g \cap r $ est nul ($ \S 5, $ no 3, th. 1); comme $[g, r] \subset \mathcal{O}g \cap r$, $ r $ est le centre de $ g $.

#### Remarque {#lie-i-s6-n4-rem-1 .statement}

Si une algèbre de Lie g peut se décomposer en un produit a × b d’une algèbre de Lie commutative a et d’une algèbre de Lie semi-simple b, cette décomposition est unique. Plus précisément, le centre de g est égal au produit des centres de a et de b, donc est égal à a. Et $ \mathcal{O}g = \mathcal{O}a \times \mathcal{O}b = b $.

#### Corollaire {#lie-i-s6-n4-cor-1 .statement}

a) Tout produit fini d’algèbres réductives est une algèbre réductive.

b) Si g est une algèbre de Lie réductive, de centre c, tout idéal de g est facteur direct, produit de ses intersections avec c et $ \mathcal{O}g $, et est une algèbre de Lie réductive.

c) Tout quotient d’une algèbre de Lie réductive est une algèbre de Lie réductive.

L’assertion a) résulte par exemple de la condition c) de la prop. 5.

Supposons g réductive. Soit a un idéal de g. Puisque la représentation adjointe de g est semi-simple, a possède un idéal supplémentaire b, et g s’identifie à a × b. Pour tout $ x \in g $, soit $ \rho(x) $ la restriction de $ \mathrm{ad}_g x $ à a. Alors, $ \rho $ est une représentation semi-simple de g qui s’annule sur b, et définit par passage au quotient la représentation adjointe de a. Donc a est réductive. De même, g/a et b, qui sont isomorphes, sont réductives. Enfin, soient d, d’ les centres de a et b ; on a $ a = d \times \mathcal{O}a, b = d' \times \mathcal{O}b, d \times d' = c, \mathcal{O}a \times \mathcal{O}b = \mathcal{O}g $; donc $ a = (a \cap c) + (a \cap \mathcal{O}g) $.

#### Proposition 6 {#lie-i-s6-prop-6 .statement}

Soient g une algèbre de Lie, r son radical, s son radical nilpotent.

a) $ s = [g, r] = \mathcal{O}g \cap r $.

b) s est l’intersection des orthogonaux de g pour les formes bilinéaires associées aux représentations de dimension finie de g.

Il est clair que $[g, r] \subset \mathcal{O}g \cap r$. On a $\mathcal{O}g \cap r = s$ d’après le th. 1 du § 5, n° 3. Soient $g' = g/[g, r]$, et f l’homomorphisme canonique de g sur $g'$; alors $f(r)$ est le radical $r'$ de $g'$ (cor. 3 de la prop. 2, n° 2), donc $[g', r'] = \{0\}$ et $r'$ est le centre de $g'$; par suite (prop. 5) $g'$ possède une représentation semi-simple fidèle de dimension finie, d’où $s \subset [g, r]$. On a prouvé $a)$.

Soit $t$ l’intersection des orthogonaux de $g$ pour les formes bilinéaires associées aux représentations de dimension finie de $g$. On a $s \subset t$ (\$ 4, n° 3, prop. 4 d)). D'autre part, $g/s$ possède une représentation semi-simple fidèle de dimension finie, donc (prop. 5) une représentation $\rho$ de dimension finie telle que la forme bilinéaire associée soit non dégénérée; considérée comme représentation de $g$, $\rho$ possède une forme bilinéaire associée $\beta$ sur $g$, et l'orthogonal de $g$ pour $\beta$ est $s$, d'où $t \subset s$. Donc $t = s$.

Même si $s \neq \{0\}$, il peut exister des formes bilinéaires invariantes symétriques non dégénérées sur $g$ (exerc. 18 c)). De telles formes, bien entendu, ne sont associées à aucune représentation de $g$.

#### Corollaire {#lie-i-s6-n4-cor-2 .statement}

*Soient g, g' des algèbres de Lie, s* (resp. $s'$) *le radical nilpotent de g* (resp. $g'$), *et f un homomorphisme de g sur g'*.
a) *On a s' = f(s)*.
b) *g' est réductive si et seulement si le noyau de f contient s*.

En effet, si $r, r'$ sont les radicaux de $g, g'$, on a $s' = [g', r'] = [f(g), f(r)] = f([g, r]) = f(s)$. L'assertion $b)$ est conséquence immédiate de $a)$.

### 5. Application : un critère de semi-simplicité pour les représentations

#### Théorème 4 {#lie-i-s6-thm-4 .statement}

*Soient g une algèbre de Lie, r son radical, $\rho$ une représentation de g de dimension finie, $g' = \rho(g)$ et $r' = \rho(r)$. Alors les conditions suivantes sont équivalentes :*
a) $\rho$ est *semi-simple* ;
b) *g' est réductive, et son centre est formé d'endomorphismes semi-simples* ;
c) *r' est formé d'endomorphismes semi-simples* ;
d) *la restriction de $\rho$ à r est semi-simple*.

$ b) \Rightarrow c) $: si $ g' $ est réductive, son centre est égal à son radical, c’est-à-dire à $ r' $, d’où l’implication $ b) \Rightarrow c) $.

$ c) \Rightarrow d) $: supposons $ r' $ formé d’endomorphismes semi-simples. Comme $[g', r']$ est formé d’endomorphismes nilpotents (no 4, prop. 6), on a $[g', r'] = \{0\}$. Ceci posé, l’implication $ c) \Rightarrow d) $ résulte d’*Alg.*, chap. VIII, § 9, no 2, th. 1.

$ d) \Rightarrow a) $: soient $ s $ le radical nilpotent de $ g $, et $ \rho' $ la restriction de $ \rho $ à $ r $. Les éléments de $ \rho(s) $ sont nilpotents, donc $ s $ est contenu dans le plus grand idéal de nilpctence de $ \rho' $. Comme $ \rho' $ est semi-simple, on a $ \rho'(s) = \{0\} $, et $ g' $ est réductive (cor. de la prop. 6), de sorte que $ g' = a' \times r' $ avec $ a' $ semi-simple (prop. 5). Soit $ A' $ (resp. $ R' $) l’algèbre associative engendrée par 1 et $ a' $ (resp. $ r' $). Elle est semi-simple (*Alg.*, chap. VIII, § 5, no 1, prop. 3), donc $ A' \otimes_K R' $ est semi-simple (*loc. cit.*, § 7, no 6, cor. 4 du th. 3), donc l’algèbre associative engendrée par 1 et $ g' $, qui est un quotient de $ A' \otimes_K R' $, est semi-simple, ce qui prouve que $ \rho $ est semi-simple.

#### Corollaire 1 {#lie-i-s6-thm-4-cor-1 .statement}

*Soient g une algèbre de Lie, $ \varphi $ et $ \varphi' $ deux représentations semi-simples de dimension finie de g. Alors, le produit tensoriel de $ \varphi $ et $ \varphi' $ est semi-simple.*

Soit $ r $ le radical de $ g $. Pour $ x \in r $, $ \rho(x) $ et $ \rho'(x) $ sont semi-simples (th. 4), donc $ \rho(x) \otimes 1 + 1 \otimes \rho'(x) $ est semi-simple (*Alg.*, chap. VIII, § 9, cor. du th. 1), donc le produit tensoriel de $ \rho $ et $ \rho' $ est semi-simple (th. 4).

#### Corollaire 2 {#lie-i-s6-thm-4-cor-2 .statement}

*Soient g une algèbre de Lie, $ \varphi $ une représentation semi-simple de g dans un espace vectoriel V de dimension finie, T et S les algèbres tensorielle et symétrique de V, et $ \sigma_T, \sigma_S $ les représentations de g dans T et S canoniquement déduites de $ \varphi $. Alors, $ \sigma_T $ et $ \sigma_S $ sont semi-simples, et, plus précisément, sommes directes de représentations simples de dimension finie.*

Soit $ T^n $ le sous-espace de T formé des tenseurs homogènes d’ordre $ n $. Ce sous-espace est stable pour $ \sigma_T $, et la représentation définie par $ \sigma_T $ dans $ T^n $ est semi-simple (cor. 1). D’où le corollaire pour $ \sigma_T $, et par suite pour $ \sigma_S $, qui est une représentation quotient de $ \sigma_T $.

#### Corollaire 3 {#lie-i-s6-thm-4-cor-3 .statement}

Soient $ g $ une algèbre de Lie, $ \rho $ et $ \rho' $ deux représentations semi-simples de dimension finie de $ g $ dans des espaces $ M $ et $ M' $. Alors, la représentation de $ g $ dans $ \mathcal{L}_k(M, M') $ canoniquement déduite de $ \rho $ et $ \rho' $ est semi-simple.

En effet, le $ g $-module $ \mathcal{L}_k(M, M') $ s’identifie canoniquement au $ g $-module $ M^* \otimes_k M' $ (\$ 3, no 3, prop. 4), de sorte que le cor. 3 résulte du cor. 1.

#### Corollaire 4 {#lie-i-s6-thm-4-cor-4 .statement}

Soient $ g $ une algèbre de Lie, $ a $ un idéal de $ g $, $ \rho $ une représentation semi-simple de $ g $.
a) La restriction $ \rho' $ de $ \rho $ à $ a $ est semi-simple.
b) Si $ \rho $ est simple, $ \rho' $ est somme de représentations simples deux à deux isomorphes.

Passant au quotient par le noyau de $ \rho $, on peut supposer $ \rho $ fidèle. Alors, $ g $ est réductive. Soit $ g = g_1 \times g_2 $, où $ g_1 $ est le centre de $ g $ et où $ g_2 $ est semi-simple. On a $ a = a_1 \times a_2 $, avec $ a_1 \subset g_1 $, $ a_2 \subset g_2 $, et $ a_1 $ est le centre de $ a $. Les éléments de $ \rho(g_1) $, et en particulier ceux de $ \rho(a_1) $, sont semi-simples (th. 4), donc $ \rho' $ est semi-simple (th. 4). D’où $ a $. L’assertion $ b $ résulte de $ a $, compte tenu du \$ 3, no 1, cor. de la prop. 1.

### 6. Sous-algèbres réductives dans une algèbre de Lie

#### Définition 5 {#lie-i-s6-def-5 .statement}

Soient $ g $ une algèbre de Lie, $ h $ une sous-algèbre de Lie de $ g $. On dit que $ h $ est réductive dans $ g $ si la représentation $ x \to \operatorname{ad}_g x $ de $ h $ est semi-simple.

Cette représentation admet comme sous-représentation la représentation adjointe de $ h $. Donc, si $ h $ est réductive dans $ g $, $ h $ est réductive. D’autre part, dire qu’une algèbre de Lie est réductive dans elle-même équivaut à dire qu’elle est réductive.

#### Proposition 7 {#lie-i-s6-prop-7 .statement}

Soient $ g $ une algèbre de Lie, $ h $ une sous-algèbre réductive dans $ g $, $ \rho $ une représentation de $ g $ dans un espace vectoriel $ V $, et $ W $ la somme des sous-espaces de dimension finie de $ V $ qui sont des $ \mathfrak{h} $-modules simples. Alors, $ W $ est stable pour $ \rho(g) $.

Soit $ W_0 $ un sous-$ \mathfrak{h} $-module simple de dimension finie de $ V $. Il s’agit de montrer que $ \rho(x)(W_0) \subset W $ pour tout $ x \in g $. Désignons par $ M $ l’espace vectoriel $ g $ considéré comme $ \mathfrak{h} $-module grâce à la représentation $ x \mapsto \mathrm{ad}_g x $ de $ \mathfrak{h} $ dans $ g $. Alors, $ M \otimes_K W_0 $ est un $ \mathfrak{h} $-module semi-simple (cor. 1 du th. 4). Soit $ \theta $ l’application K-linéaire de $ M \otimes_K W_0 $ dans $ V $ définie par $ \theta(x \otimes w) = \rho(x)w $. C’est un homomorphisme de $ \mathfrak{h} $-modules, car, si $ y \in \mathfrak{h} $, on a :
$$
\begin{align*}
\theta([y, x] \otimes w + x \otimes \rho(y)w) &= \rho([y, x])w + \rho(x)\rho(y)w \\
&= \rho(y)\rho(x)w = \rho(y)\theta(x \otimes w).
\end{align*}
$$
Donc $ \theta(M \otimes_K W_0) $ est un $ \mathfrak{h} $-module semi-simple de dimension finie. Donc $ \theta(M \otimes_K W_0) \subset W $, c’est-à-dire $ \rho(x)(W_0) \subset W $ pour tout $ x \in g $.

#### Corollaire 1 {#lie-i-s6-prop-7-cor-1 .statement}

*Soient $ g $ une algèbre de Lie, $ \mathfrak{h} $ une sous-algèbre réductive dans $ g $, et $ \rho $ une représentation semi-simple de dimension finie de $ g $. Alors la restriction de $ \rho $ à $ \mathfrak{h} $ est semi-simple.*

En effet, il suffit d’étudier le cas où $ \rho $ est simple. Adoptons les notations $ V, W $ de la prop. 4. Soit $ W_1 $ un sous-espace de $ V $ minimal parmi les sous-espaces non nuls et stables pour $ \rho(\mathfrak{h}) $. On a $ W_1 \subset W $, donc $ W \neq \{0\} $, donc $ W = V $.

#### Corollaire 2 {#lie-i-s6-prop-7-cor-2 .statement}

*Soient $ g $ une algèbre de Lie, $ \mathfrak{h} $ une sous-algèbre réductive dans $ g $, et $ \mathfrak{k} $ une sous-algèbre de $ \mathfrak{h} $ réductive dans $ \mathfrak{h} $. Alors, $ \mathfrak{k} $ est réductive dans $ g $.*

En effet, la représentation $ x \mapsto \mathrm{ad}_g x $ de $ \mathfrak{h} $ dans $ g $ est semi-simple, donc sa restriction à $ \mathfrak{k} $ est semi-simple (cor. 1).

### 7. Exemples d’algèbres de Lie semi-simples

#### Proposition 8 {#lie-i-s6-prop-8 .statement}

*Soit $ V $ un espace vectoriel de dimension finie. Alors, $ \mathrm{gl}(V) $ est réductive, son centre est l’ensemble des homothéties de $ V $, son algèbre dérivée est $ \mathfrak{sl}(V) $, et cette dernière est semi-simple.*

La représentation identique de $ \mathrm{gl}(V) $ est simple, donc $ \mathrm{gl}(V) $ est réductive, et par suite $ \mathrm{gl}(V) $ est somme directe de son centre $ c $ et de son algèbre dérivée $ \mathcal{O}(\mathrm{gl}(V)) $. Le centre $ c $ est l’ensemble des homothéties (*Alg.*, chap. II, § 2, n° 5, cor. 1 de la prop. 5). Il est clair que $ \mathcal{O}(gl(V)) \subset sl(V) $. Comme $ sl(V) \cap c = \{0\} $, on a $ \mathcal{O}(gl(V)) = sl(V) $. Donc $ sl(V) $ est semi-simple.

#### Exemple {#lie-i-s6-n7-exa-1 .statement}

Identifions $ sl(K^2) $ à l’algèbre de Lie des matrices d’ordre 2 et de trace nulle. Posons

$$
X = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} \quad Y = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} \quad H = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

Alors, $ X, Y, H $ forment une base de $ sl(K^2) $, et on a

$$
[H, X] = 2X \qquad [H, Y] = -2Y \qquad [X, Y] = H.
$$

Comme une algèbre de dimension 1 ou 2 est non semi-simple (n° 1, remarque 1), $ sl(K^2) $ est simple. En fait, $ sl(V) $ est simple dès que $ \dim V \geq 2 $, comme nous le verrons plus tard (cf. aussi exerc. 21 et 24).

#### Proposition 9 {#lie-i-s6-prop-9 .statement}

*Soient V un espace vectoriel de dimension finie n sur K, $ \beta $ une forme bilinéaire symétrique (resp. alternée) non dégénérée sur V. Soit g l’algèbre de Lie formée des $ x \in gl(V) $ tels que $ \beta(xm, m') + \beta(m, xm') = 0 $ quels que soient $ m, m' $ dans V. Alors, g est réductive ; g est même semi-simple sauf dans le cas où $ \beta $ est symétrique et où $ n = 2 $.*

Pour tout $ u \in gl(V) $, on notera $ u^* $ son adjoint relativement à $ \beta $; on a $ \operatorname{Tr}(u) = \operatorname{Tr}(u^*) $ d’après la prop. 7 d’Alg., chap. IX, § 1, n° 8. La condition $ \beta(um, m') + \beta(m, um') = 0 $ quels que soient $ m, m' $ dans V signifie que $ u + u^* = 0 $. En particulier, si $ v \in gl(V) $, on a $ (v - v^*)^* = v^* - v $, donc $ v - v^* \in g $. Ceci posé, soit $ u $ un élément de g orthogonal à g pour la forme bilinéaire $ \varphi $ associée à la représentation identique de g. Quel que soit $ v \in gl(V) $, on a $ \operatorname{Tr}\, u(v - v^*) = 0 $, donc

$$
\operatorname{Tr}(uv) = \operatorname{Tr}(uv^*) = \operatorname{Tr}(uv^*)^* = \operatorname{Tr}(vu^*) = -\operatorname{Tr}(vu) = -\operatorname{Tr}(uv)
$$

donc $ \operatorname{Tr}(uv) = 0 $. Il en résulte que $ u = 0 $, de sorte que $ \varphi $ est non dégénérée. Donc g est réductive (prop. 5). Il nous reste à montrer que le centre de g est nul (sauf si $ \beta $ est symétrique et que $ n = 2 $). Par extension du corps de base, on peut supposer K algébriquement clos.

b) Lorsque $ \beta $ est alternée et que $ n = 2m $, on peut identifier $ \beta $ à la forme bilinéaire sur $ K^{2m} $ de matrice $ \begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix} $ par rapport à la base canonique ($ Alg. $, chap. IX, § 5, cor. 1 du th. 1). Dans ces conditions $ g $ s’identifie à l’algèbre de Lie des matrices de la forme $ U = \begin{pmatrix} A & B \\ C & D \end{pmatrix} $ avec $ D = -'A $, $ B $ et $ C $ symétriques ($ A, B, C, D $ dans $ \mathbf{M}_m(K) $) ($ § 3 $, no 4, exemple 1). Exprimons d’abord que $ U $ commute à la matrice $ \begin{pmatrix} X & 0 \\ 0 & -'X \end{pmatrix} $, où $ X \in \mathbf{M}_m(K) $. Il vient $ AX = XA $, $ CX = -'XC $, $ XB = -B.'X $; comme ces égalités doivent être vérifiées quel que soit $ X $, on en déduit que $ A $ est une matrice scalaire $ \lambda I_m $. Exprimons maintenant que $ U $ commute à la matrice $ \begin{pmatrix} 0 & Y \\ 0 & 0 \end{pmatrix} $, où $ Y $ est une matrice symétrique de $ \mathbf{M}_m(K) $. Il vient $ \lambda Y = YC = CY = 0 $. Ceci prouve d’abord que $ \lambda = 0 $. En outre, pour tout $ X \in \mathbf{M}_m(K) $, $ X + 'X $ est symétrique, et on doit donc avoir $ XC = -'XC $. Compte tenu de l’égalité $ CX = -'XC $ obtenue plus haut, on voit que $ C $ commute à tout élément de $ \mathbf{M}_m(K) $, donc que $ C $ est une matrice scalaire, nécessairement nulle puisque $ YC = 0 $. On démontre de même que $ B = 0 $.

Pour $ \beta $ symétrique et $ n = 2 $, $ g $ est de dimension 1, donc commutative. Pour les autres cas, cf. exerc. 25 et 26.

### 8. Le théorème de Levi-Malcev

Soient E un espace vectoriel normé complet sur $ \mathbf{R} $, et $ u $ un endomorphisme continu de E. On a vu (Fonct. var. réelle, chap. IV, § 2, n° 6) que la suite $ \frac{u^n}{n!} $ est sommable dans $ \mathcal{L}(E) $, et on a posé
$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$
Soient maintenant E un espace vectoriel sur le corps K et $ u $ un endomorphisme nilpotent de E. La série $ \sum_{n=0}^\infty \frac{u^n}{n!} $ n’a qu’un nombre fini de termes non nuls, et on peut donc poser
$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$
Cette définition concorde avec la précédente si $ K = \mathbf{R} $ et si E est normé complet. Si $ \varphi $ est un autre endomorphisme nilpotent de E permutable à $ u $, on a :
$$
(3) \quad e^u e^\varphi = \left( \sum_{n=0}^\infty \frac{u^n}{n!} \right) \left( \sum_{p=0}^\infty \frac{\varphi^p}{p!} \right) = \sum_{n,p=0}^\infty \frac{u^n \varphi^p}{n! p!}
= \sum_{q=0}^\infty \frac{1}{q!} \left( \sum_{n+p=q} \binom{q}{n} u^n \varphi^p \right) = \sum_{q=0}^\infty \frac{1}{q!} (u + \varphi)^q = e^{u+\varphi}.
$$
En particulier, $ e^u e^{-u} = e^{-u} e^u = e^0 = 1 $, donc $ e^u $ est toujours un automorphisme de E.

Si en outre E est une algèbre (non nécessairement associative), et si $ u $ est une dérivation (nilpotente) de E, alors $ e^u $ est un automorphisme de l’algèbre E. En effet, si $ x, y \in E $, on a
$$
u^p(xy) = \sum_{r+s=p} \binom{p}{r} u^r(x) u^s(y)
$$
pour tout entier $ p \geq 0 $ (formule de Leibniz). Il en résulte que :
$$
e^u(xy) = \sum_{p \geq 0} \frac{1}{p!} u^p(xy) = \sum_{p \geq 0} \sum_{r+s=p} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!}
= \sum_{r,s=0}^\infty \frac{u^r(x)}{r!} \frac{u^s(y)}{s!} = e^u(x) e^u(y)
$$
d’où notre assertion.

Soit maintenant g une algèbre de Lie. Si x appartient au radical nilpotent de g, la dérivation ad_g x de g est nilpotente. On peut donc poser la définition suivante :

#### Définition 6 {#lie-i-s6-def-6 .statement}

On appelle automorphisme spécial de g un automorphisme de g de la forme e^{ad_x}, où x est dans le radical nilpotent de g.

Il est clair qu’un automorphisme spécial laisse stable tout idéal de g.

#### Définition 7 {#lie-i-s6-def-7 .statement}

Soient g une algèbre de Lie, r son radical. On appelle sous-algèbre de Levi de g toute sous-algèbre supplémentaire de r dans g.

Une sous-algèbre de Levi est isomorphe à g/r, donc semi-simple. Comme une sous-algèbre semi-simple n’a que 0 en commun avec r, toute sous-algèbre semi-simple h telle que g = r + h est une sous-algèbre de Levi ; par conséquent, l’image d’une sous-algèbre de Levi par un homomorphisme surjectif est une sous-algèbre de Levi.

#### Théorème 5 (Levi-Malcev) {#lie-i-s6-thm-5 .statement}

Une algèbre de Lie g possède toujours une sous-algèbre de Levi s. Toute sous-algèbre de Levi de g est transformée de s par un automorphisme spécial.

On note r le radical de g. On traitera d’abord deux cas particuliers.

a) [g, r] = {0}.

D’après la prop. 5, g est alors le produit de son centre r par $ \mathcal{O}g $ qui est semi-simple. Donc $ \mathcal{O}g $ est une sous-algèbre de Levi. De plus, si s’ est une sous-algèbre semi-simple, on a s’ = $ \mathcal{O}s' $ (th. 1), donc s’ $ \subset \mathcal{O}g $, et $ \mathcal{O}g $ est l’unique sous-algèbre de Levi de g.

b) [g, r] $ \neq $ {0}, et les seuls idéaux de g contenus dans r sont {0} et r.

Alors, [g, r] = r, [r, r] = {0}, et le centre de g est nul. Soit M (resp. N) le sous-espace de $ \mathfrak{L}(g) $ formé des applications linéaires de g dans r dont la restriction à r est une homothétie (resp. est nulle);

N est donc de codimension 1 dans M. Pour $ m \in M $, on notera $ \lambda(m) $ le rapport de l’homothétie de r définie par m. Soit $ \sigma $ la représentation de g dans $ \mathcal{L}(g) $ canoniquement déduite de la représentation adjointe ; rappelons que $ \sigma(x).u = [\mathrm{ad}_g x, u] $ pour tout $ x \in g $ et tout $ u \in \mathcal{L}(g) $.

$$
\begin{array}{ll}
\mathcal{L}(g) & \text{Il est clair que } \sigma(x)(M) \subset N \text{ pour tout } x \in g. \text{ De plus,} \\
\cup & \text{si } x \in r, y \in g \text{ et } u \in M, \text{ on a} \\
M & (4) \quad (\sigma(x).u)(y) = [x, u(y)] - u([x, y]) = -\lambda(u)[x, y] \\
\cup & \text{puisque } [r, r] = \{0\}; \text{ et (4) peut s’écrire :} \\
N & \\
P & (5) \qquad \sigma(x).u = -\mathrm{ad}\ (\lambda(u).x).
\end{array}
$$

Comme le centre de g est nul, l’application $ x \mapsto \mathrm{ad}_g x $ définit une bijection $ \varphi $ de r sur un sous-espace P de $ \mathcal{L}(g) $. Ce sous-espace est stable pour $ \sigma(g) $ et contenu dans N puisque r est un idéal commutatif, et (5) montre que $ \sigma(x)(M) \subset P $ pour $ x \in r $. La représentation de g dans $ M/P = V $ déduite de $ \sigma $ est donc nulle sur r et définit une représentation $ \sigma' $ de l’algèbre semi-simple $ g/r $ dans V. Pour tout $ y \in g/r $, l’espace $ \sigma'(y)(V) $ est contenu dans $ N/P $, qui est de codimension 1 dans V. Par conséquent (n° 2, lemme 3) il existe un $ u_0 \in M $ tel que $ \lambda(u_0) = -1 $ et tel que $ \sigma(x).u_0 \in P $ pour tout $ x \in g $. L’application $ x \mapsto \overline{\varphi}(\sigma(x).u_0) $ est une application linéaire de g dans r. D’après (5), sa restriction à r est l’application identique de r. Donc son noyau est un sous-espace s de g supplémentaire de r dans g. Comme s est l’ensemble des $ x \in g $ tels que $ \sigma(x).u_0 = 0 $, s est une sous-algèbre de g, et par suite une sous-algèbre de Levi de g.

Soit $ s' $ une deuxième sous-algèbre de Levi. Pour tout $ x \in s' $, soit $ h(x) $ l’unique élément de r tel que $ x + h(x) \in s $. Puisque s est une sous-algèbre et que r est commutatif, on a, pour $ x, y $ dans $ s' $ :

$$
[x + h(x), y + h(y)] = [x, y] + [x, h(y)] + [h(x), y] \in s
$$

donc :

$$
h([x, y]) = (\mathrm{ad}\ x).h(y) - (\mathrm{ad}\ y).h(x).
$$

D’après la remarque 2 du n° 2, il existe un $ a \in r $ tel que $ h(x) = -[x, a] $ pour tout $ x \in s' $. Alors :

(6) $$
x + h(x) = x + [a, x] = (1 + \mathrm{ad}\ a).x.
$$

Comme $ r $ est commutatif, $(\mathrm{ad}\,a)^2 = 0$, donc $ 1 + \mathrm{ad}\,a = e^{\mathrm{ad}\,a} $. Comme $ r = [g, r] $, $ e^{\mathrm{ad}\,a} $ est un automorphisme spécial de $ g $. D’après (6), cet automorphisme spécial transforme $ s' $ en $ s $.

c) Cas général :

On raisonne par récurrence sur la dimension $ n $ du radical. Il n’y a rien à démontrer si $ n = 0 $, et on peut donc supposer le théorème vrai pour les algèbres de Lie dont le radical est de dimension < dim $ r $. D’après $ a $), il suffit de considérer le cas où $[g, r] \neq \{0\}$. Comme $[g, r]$ est nilpotente (n° 4, prop. 6), son centre $ c $ est $ \neq \{0\} $. Soit $ m $ un idéal non nul minimal de $ g $ contenu dans $ c $. Si $ m = r $, on est ramené au cas $ b $). Soit donc $ m \neq r $ et soit $ f $ l’application canonique de $ g $ sur $ g' = g/m $. Le radical de $ g' $ est $ r' = r/m $. D’après l’hypothèse de récurrence, $ g' $ possède une sous-algèbre de Levi $ h' $. Alors $ h = \overline{f(h')}(h') $ est une sous-algèbre de $ g $ contenant $ m $, telle que $ h/m = h' $ soit semi-simple, donc ayant $ m $ pour radical. D’après l’hypothèse de récurrence, $ h = m + s $ où $ s $ est une sous-algèbre semi-simple. Alors l’égalité $ g' = r' + h' $ entraîne $ g = r + h = r + m + s = r + s $, donc $ s $ est une sous-algèbre de Levi de $ g $.

Soit $ s' $ une deuxième sous-algèbre de Levi de $ g $. Alors $ f(s) $ et $ f(s') $ sont deux sous-algèbres de Levi de $ g' $, et il existe, d’après l’hypothèse de récurrence, un $ a' \in [g', r'] $ tel que $ e^{\mathrm{ad}\,a'}(f(s')) = f(s) $. Si $ a \in [g, r] $ est tel que $ f(a) = a' $, il s’ensuit que :

$$
s_1 = e^{\mathrm{ad}\,a}(s') \subset m + s = h.
$$

Alors, $ s_1 $ et $ s $ sont deux sous-algèbres de Levi de $ h $, et il existe, d’après l’hypothèse de récurrence, un $ b \in m $ tel que $ e^{\mathrm{ad}\,b}(s_1) = s $. Donc $ s = e^{\mathrm{ad}\,b}.e^{\mathrm{ad}\,a}(s') $. Enfin, comme $ m $ est dans le centre de $[g, r]$, on a $ e^{\mathrm{ad}\,b}.e^{\mathrm{ad}\,a} = e^{\mathrm{ad}\,(b+a)} $ et $ b + a \in [g, r] $, ce qui achève la démonstration.

#### Corollaire 1 {#lie-i-s6-thm-5-cor-1 .statement}

*Soient s une sous-algèbre de Levi de g, et h une sous-algèbre semi-simple de g.*

a) *Il existe un automorphisme spécial de g transformant h en une sous-algèbre de s.*

b) *h est contenu dans une sous-algèbre de Levi de g.*

Soient $ r $ le radical de $ g $, et $ a = h + r $, qui est une sous-algèbre de $ g $. Alors, $ a/r $ est semi-simple et $ r $ est résoluble, donc $ r $ est le radical de $ a $, et $ h $ est une sous-algèbre de Levi de $ a $. D’autre part, $ a \cap s = h' $ est une sous-algèbre supplémentaire de $ r $ dans $ a $, donc aussi une sous-algèbre de Levi de $ a $. Il existe alors (th. 5) un $ a \in [a, r] $ tel que $ e^{ad_a a} $ transforme $ h $ en $ h' $. On a $ a \in [g, r] $; $ e^{ad_g a} $ transforme $ h $ en une sous-algèbre de $ s $, et $ e^{-ad_g a}(s) $ est une sous-algèbre de Levi de $ g $ contenant $ h $.

#### Corollaire 2 {#lie-i-s6-thm-5-cor-2 .statement}

*Pour qu’une sous-algèbre $ h $ de $ g $ soit une sous-algèbre de Levi de $ g $, il faut et il suffit que $ h $ soit une sous-algèbre semi-simple maximale de $ g $.*

Ceci résulte aussitôt du cor. 1.

#### Corollaire 3 {#lie-i-s6-thm-5-cor-3 .statement}

*Soient $ g $ une algèbre de Lie, $ m $ un idéal de $ g $ tel que $ g/m $ soit semi-simple. Alors $ g $ contient une sous-algèbre supplémentaire de $ m $ dans $ g $. Autrement dit, toute extension d’une algèbre de Lie semi-simple est inessentielle.*

Soit $ s $ une sous-algèbre de Levi de $ g $ (th. 5). Son image canonique dans $ g/m $, étant une sous-algèbre de Levi, est égale à $ g/m $, donc $ g = s + m $. Alors, un idéal de $ s $ supplémentaire dans $ s $ de l’idéal $ m \cap s $ est une sous-algèbre de $ g $ supplémentaire de $ m $ dans $ g $.

#### Corollaire 4 {#lie-i-s6-thm-5-cor-4 .statement}

*Soient $ g $ une algèbre de Lie, $ r $ son radical, $ s $ une sous-algèbre de Levi de $ g $, $ m $ un idéal de $ g $. Alors, $ m $ est somme directe de $ m \cap r $ qui est son radical et de $ m \cap s $ qui est une sous-algèbre de Levi de $ m $.*

On sait que $ m \cap r $ est le radical de $ m $ (\S 5, no 5, cor. 3 de la prop. 5). Soient $ h $ une sous-algèbre de Levi de $ m $, et $ s' $ une sous-algèbre de Levi de $ g $ contenant $ h $ (cor. 1). L’algèbre $ m \cap s' $ est un idéal de $ s' $, donc est semi-simple, et contient $ h $, donc est égale à $ h $. Donc $ m $ est somme directe de $ m \cap r $ et $ m \cap s' $. Il existe un automorphisme spécial transformant $ s' $ en $ s $; cet automorphisme conserve $ r $ et $ m $; donc $ m $ est somme directe de $ m \cap r $ et $ m \cap s $, et $ m \cap s $ est une sous-algèbre de Levi de $ m $.

### 9. Le théorème des invariants

Soient g une algèbre de Lie, ρ une représentation de g dans un espace vectoriel M. Pour toute classe δ de représentation simple de g, soit M_δ le composant isotypique d’espèce δ de M. Le sous-espace M_0 des éléments invariants de M n’est autre que M_{δ_0}, δ_0 désignant la classe de la représentation nulle de g dans un espace de dimension 1.

#### Lemme 4 {#lie-i-s6-lem-4 .statement}

Soient ρ, σ, τ des représentations de g dans des espaces vectoriels M, N, P. Supposons donnée une application K-bilinéaire (m, n) ↦ m.n de M × N dans P, telle que

$$(ρ(x)m).n + m.(σ(x)n) = τ(x)(m.n)$$

quels que soient m ∈ M, n ∈ N, x ∈ g.

a) Si m_0 ∈ M_0, l’application n → m_0.n est un homomorphisme de g-modules.

b) Si n ∈ N_δ, on a m_0.n ∈ P_δ.

c) Si M est une algèbre (non nécessairement associative), et si les ρ(x) sont des dérivations de M, M_0 est une sous-algèbre de M, et chaque M_δ est un M_0-module à droite et à gauche.

On a, pour m_0 ∈ M_0, n ∈ N et x ∈ g,

$$τ(x)(m_0.n) = m_0.(σ(x)n),$$

d’où a). L’assertion b) résulte de a) (Alg., chap. VIII, § 3, no 4, prop. 10). Si on fait N = P = M, σ = τ = ρ, l’assertion b) donne l’assertion c) comme cas particulier.

#### Lemme 5 {#lie-i-s6-lem-5 .statement}

Supposons de plus σ et τ semi-simples, donc N (resp. P) somme directe des N_δ (resp. P_δ). Pour tout n ∈ N (resp. p ∈ P), soit n^h (resp. p^h) sa composante dans N_0 (resp. P_0). Soit m_0 ∈ M_0. Alors, pour tout n ∈ N, on a (m_0.n)^h = m_0.n^h.

Par linéarité, il suffit d’envisager le cas où n ∈ N_δ. Si δ ≠ δ_0, on a n^h = 0, et m_0.n ∈ P_δ (lemme 4), donc (m_0.n)^h = 0 = m_0.n^h. Si δ = δ_0, on a n^h = n, et m_0.n ∈ P_0 (lemme 4), donc (m_0.n)^h = m_0.n = m_0.n^h.

#### Théorème 6 {#lie-i-s6-thm-6 .statement}

Soient g une algèbre de Lie, V un g-module semi-simple de dimension finie sur K, S l’algèbre symétrique de V, et $ x_s $ la dérivation de $ S $ qui prolonge $ x_v $ (de sorte que $ x \to x_s $ est une représentation de $ g $ dans $ S $).

a) L’algèbre $ S_0 $ des invariants de $ S $ est engendrée par un nombre fini d’éléments.

b) Pour toute classe $ \delta $ de représentation simple de $ g $ de dimension finie sur $ K $, soit $ S_\delta $ le composant isotypique d’espèce $ \delta $ de $ S $. Alors, $ S_\delta $ est un $ S_0 $-module de type fini.

Soit $ \overline{S} \subset S $ l’idéal des éléments de $ S $ sans terme constant. Soit $ I $ l’idéal de $ S $ engendré par $ S_0 \cap \overline{S} $, et soit $ (s_1, s_2, \ldots, s_p) $ un système fini de générateurs de l’idéal $ I $ (Alg. comm., chap. III, § 3). On peut supposer que les $ s_i $ appartiennent à $ S_0 \cap \overline{S} $ et sont homogènes (en effet, les $ x_s $ conservent les degrés, donc chaque $ S_\delta $ est un sous-module gradué). Soit $ S_1 $ la sous-algèbre de $ S $ engendrée par 1 et les $ s_i $. On a $ S_1 \subset S_0 $. Montrons que $ S_1 = S_0 $. Pour cela, nous allons montrer que tout élément homogène $ s $ de $ S_0 $ est dans $ S_1 $, en raisonnant par récurrence sur le degré $ n $ de $ s $. Si $ n = 0 $, notre assertion est évidente. Supposons donc $ n > 0 $, et notre assertion démontrée lorsque le degré de $ s $ est $ < n $. Comme $ s \in I $, on a $ s = \sum_{i=1}^p s_i s_i' $, les $ s_i' $ étant des éléments de $ S $ qu’on peut supposer homogènes, avec $ \deg(s_i') = \deg(s) - \deg(s_i) < n $. Le lemme 5 est applicable, car le $ g $-module $ S $ est semi-simple (n° 5, cor. 2 du th. 4); avec les notations de ce lemme, on a

$$
s = s^\sharp = \sum_{i=1}^p (s_i s_i')^\sharp = \sum_{i=1}^p s_i s_i'^\sharp.
$$

Les $ s_i'^\sharp $ sont des éléments de $ S_0 $ homogènes et de degré $ < n $ (parce que chaque $ S_\delta $ est un sous-module gradué). Ils sont donc dans $ S_1 $ d’après l’hypothèse de récurrence. Donc $ s \in S_1 $, ce qui achève la démonstration de $ a $.

Maintenant, considérons une représentation simple de classe $ \delta $ de $ g $ dans un espace $ M $ de dimension finie. Soit $ L = \mathcal{L}_K(M, S) $. Pour tout $ s \in S $ et tout $ f \in L $, soit $ sf $ l’élément de $ L $ défini par $ (sf)(m) = s . f(m) $ ($ m \in M $); on définit ainsi sur $ L $ une structure de $ S $-module ; comme $ M $ est de dimension finie sur $ K $, il est clair que $ L $ est un $ S $-module de type fini, donc un $ S $-module noethérien puisque l’anneau $ S $ est noethérien. Par ailleurs, $ L $ est muni canoniquement d’une structure de $ g $-module. Pour tout entier $ n \geqslant 0 $, soit $ S^n $ l’ensemble des éléments homogènes de degré $ n $ de $ S $; alors, le $ g $-module $ \mathcal{L}_K(M, S^n) $ est semi-simple (n° 5, cor. 3 du th. 4), donc le $ g $-module $ L $ est semi-simple. En outre, on a pour $ s \in S,\ f \in L,\ x \in g $ et $ m \in M $,

$$
\begin{align*}
(x_L(sf))(m) &= x_s((sf)(m)) - (sf)(x_M m) \\
&= x_s(s . f(m)) - s . f(x_M m) \\
&= (x_s s) . f(m) + s . (x_s f(m)) - s . f(x_M m) \\
&= ((x_s s)f)(m) + (s(x_L f))(m)
\end{align*}
$$

donc $ x_L(sf) = (x_s s)f + s(x_L f) $. Nous pourrons donc appliquer le lemme 5.

Le sous-ensemble $ L_0 $ des éléments invariants de $ L $ n’est autre que l’ensemble des homomorphismes du $ g $-module $ M $ dans le $ g $-module $ S $. Donc, si on désigne par $ \varphi $ l’homomorphisme canonique de $ M \otimes_K L $ sur $ S $, on a $ \varphi(M \otimes_K L_0) = S_\delta $. Comme $ \varphi $ est évidemment un homomorphisme de $ S $-modules, il suffit de montrer que $ L_0 $ est un $ S_0 $-module de type fini. Soit $ J $ le sous-$ S $-module de $ L $ engendré par $ L_0 $. Puisque $ L $ est un $ S $-module noethérien, il existe une suite finie $ (f_1, \ldots, f_q) $ d’éléments de $ L_0 $ engendrant le $ S $-module $ J $. Soit $ L_1 $ le $ S_0 $-module engendré par $ f_1, \ldots, f_q $. On a $ L_1 \subset L_0 $. Par ailleurs, si $ f \in L_0 $, on a $ f = \sum_{i=1}^q s_i f_i $ avec $ s_i \in S $ pour tout $ i $, donc compte tenu du lemme 5 dont nous adoptons les notations :

$$
f = f^\sharp = (\sum_{i=1}^q s_i f_i)^\sharp = \sum_{i=1}^q s_i^\sharp f_i \in L_1.
$$

Donc $ L_0 = L_1 $, de sorte que $ L_0 $ est un $ S_0 $-module de type fini.

### 10. Changement du corps de base

Soit $ K_1 $ une extension commutative de $ K $. Pour qu’une algèbre de Lie $ g $ sur $ K $ soit semi-simple, il faut et il suffit que $ g_{(K_1)} $ soit semi-simple ; en effet, la forme de Killing $ \beta_1 $ de $ g_{(K_1)} $ se déduit de la forme de Killing $ \beta $ de $ g $ par extension du corps de base de $ K $ à $ K_1 $; donc $ \beta_1 $ est non dégénérée si et seulement si $ \beta $ est non dégénérée (Alg., chap. IX, § 1, n° 4, cor. de la prop. 3).

Si $ g_{(K_1)} $ est simple, $ g $ est semi-simple d’après ce qui précède, et ne peut être produit de deux idéaux non nuls, donc $ g $ est simple. Par contre, si $ g $ est simple, $ g_{(K_1)} $ (qui est semi-simple) peut être non simple (exerc. 17 et 26 b)).

Soient $ g $ une algèbre de Lie, $ r $ son radical. Alors, $ r_{(K_1)} $ est le radical de $ g_{(K_1)} $ (\S 5, no 6). Par suite, si $ s $ désigne le radical nilpotent de $ g $, le radical nilpotent de $ g_{(K_1)} $ est $[g_{(K_1)}, r_{(K_1)}] = [g, r]_{(K_1)} = s_{(K_1)}$. Il en résulte que $ g $ est réductive si et seulement si $ g_{(K_1)} $ est réductive.

Soient $ g $ une algèbre de Lie, $ h $ une sous-algèbre. Rappelons qu’une représentation de $ h $ est semi-simple si et seulement si la représentation de $ h_{(K_1)} $ qu’on en déduit par extension à $ K_1 $ du corps de base est semi-simple. Donc $ h $ est réductive dans $ g $ si et seulement si $ h_{(K_1)} $ est réductive dans $ g_{(K_1)} $.

Soit maintenant $ K_0 $ un sous-corps de $ K $ tel que $[K : K_0]$ soit fini. Soient $ g $ une algèbre de Lie, et $ g_0 $ l’algèbre de Lie (de dimension finie) déduite de $ g $ par restriction du corps de base de $ K $ à $ K_0 $. Tout idéal commutatif de $ g $ est un idéal commutatif de $ g_0 $; réciproquement, si $ a_0 $ est un idéal commutatif de $ g_0 $, le plus petit sous-espace vectoriel sur $ K $ de $ g $ contenant $ a_0 $ est un idéal commutatif de $ g $; donc $ g $ est semi-simple si et seulement si $ g_0 $ est semi-simple. Si $ g_0 $ est simple, il est clair que $ g $ est simple. Réciproquement, supposons que $ g $ soit simple, et montrons que $ g_0 $ est simple. Soit $ a_0 $ un composant simple de $ g_0 $. Pour tout $ \lambda \in K^* $, $ \lambda a_0 $ est un idéal de $ g_0 $, et $[a_0, \lambda a_0] = \lambda [a_0, a_0] = \lambda a_0 \neq \{0\}$, donc $ \lambda a_0 \supset a_0 $ et par suite $ \lambda a_0 = a_0 $ puisque $ \dim_{K_0}(\lambda a_0) = \dim_{K_0} a_0 $. Or, le sous-espace vectoriel de $ g $ engendré par $ a_0 $ est un idéal non nul de $ g $, donc est $ g $ tout entier. Donc $ g = a_0 $, ce qui prouve notre assertion.

## EXERCICES {#lie-i-s6-exercises}

Les conventions du § 6 restent valables, sauf mention du contraire.

See the [exercises for § 6](exercises/s6/).
