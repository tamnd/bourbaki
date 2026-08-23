---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 4
section_title: Algèbres de Lie nilpotentes
lang: fr
source: lie-i-fr
pdf_pages: 0053-0059, 0116-0123
extraction: ocr
subsections:
    - "no": 1
      title: Définition des algèbres de Lie nilpotentes
      page: 0
      pdf_page: 53
    - "no": 2
      title: Le théorème d’Engel
      page: 0
      pdf_page: 55
    - "no": 3
      title: Le plus grand idéal de nilpotence d’une représentation
      page: 0
      pdf_page: 56
    - "no": 4
      title: Le plus grand idéal nilpotent d’une algèbre de Lie
      page: 0
      pdf_page: 58
    - "no": 5
      title: Extension du corps de base
      page: 0
      pdf_page: 59
statements: 18
exercises: 27
content_sha256: 944ad1f5841ab1ce2af635628603bbdf5eb7d6d2611c6acac325a3710ca53342
---

## § 4. Algèbres de Lie nilpotentes

On rappelle que K désigne désormais un corps commutatif. Dans toute la fin du chapitre, les algèbres de Lie sont supposées de dimension finie sur K.

### 1. Définition des algèbres de Lie nilpotentes

#### Définition 1 {#lie-i-s4-def-1 .statement}

Une algèbre de Lie g est dite nilpotente s’il existe une suite finie décroissante d’idéaux $(g_i)_{0 \leq i \leq p}$ de g, avec $g_0 = g$, $g_p = \{0\}$, telle que $[g, g_i] \subset g_{i+1}$ pour $0 \leq i < p$.

Une algèbre de Lie commutative est nilpotente.

#### Proposition 1 {#lie-i-s4-prop-1 .statement}

Soit g une algèbre de Lie. Les conditions suivantes sont équivalentes :
a) g est nilpotente ;
b) $C^k g = \{0\}$ pour k assez grand ;
c) $C_k g = g$ pour k assez grand ;
d) il existe un entier k tel que $\operatorname{ad} x_1 \circ \operatorname{ad} x_2 \circ \cdots \circ \operatorname{ad} x_k = 0$ quels que soient les éléments $x_1, x_2, \ldots, x_k$ dans g ;
e) il existe une suite décroissante d’idéaux $(g_i)_{0 \leq i \leq n}$ de g, avec $g_0 = g$, $g_n = \{0\}$, telle que $[g, g_i] \subset g_{i+1}$ et $\dim g_i / g_{i+1} = 1$ pour $0 \leq i < n$.

Si $C^k g = \{0\}$ (resp. $C_k g = g$), il est clair que la suite $C^1 g, \ldots, C^k g$ (resp. $C_k g, C_{k-1} g, \ldots, C_0 g$) possède les propriétés de la définition 1, donc que g est nilpotente. Réciproquement, supposons qu’il existe une suite $(g_i)_{0 \leq i \leq p}$ possédant les propriétés de la définition 1. On voit par récurrence sur i que $g_i \supset C^{i+1} g$ et $g_{p-i} \subset C_i g$. Donc $C^{p+1} g = \{0\}$ et $C_p g = g$. On a ainsi prouvé que les conditions a), b), c) sont équivalentes. D’autre part, $C^i g$ est l’ensemble des combinaisons linéaires d’éléments de la forme
$$
[x_1, [x_2, \ldots, [x_{i-2}, [x_{i-1}, x_i]] \ldots ]]
$$
quand $x_1, x_2, \ldots, x_i$ parcourent g. Donc les conditions b) et d) sont équivalentes. Enfin, s’il existe une suite $(g_i)_{0 \leq i \leq p}$ d’idéaux possédant les propriétés de la déf. 1, il existe une suite décroissante (h_i)_{0 \leq i \leq n} de sous-espaces vectoriels de g de dimension n, n - 1, n - 2, \ldots, 0, et une suite d’indices i_0 < i_1 < \cdots < i_p avec g_0 = h_{i_0}, g_1 = h_{i_1}, \ldots, g_p = h_{i_p}; alors, comme [g, h_{i_k}] \subset h_{i_{k+1}}, les h_i sont des idéaux et [g, h_i] \subset h_{i+1} pour tout i. Donc les conditions a) et e) sont équivalentes.

#### Corollaire 1 {#lie-i-s4-prop-1-cor-1 .statement}

Le centre d’une algèbre de Lie nilpotente non nulle est non nul.

#### Corollaire 2 {#lie-i-s4-prop-1-cor-2 .statement}

La forme de Killing d’une algèbre de Lie nilpotente est nulle.

En effet, quels que soient x et y dans une algèbre de Lie nilpotente, ad x \circ ad y est nilpotent, donc de trace nulle.

#### Proposition 2 {#lie-i-s4-prop-2 .statement}

Une sous-algèbre, une algèbre quotient, une extension centrale d’une algèbre de Lie nilpotente sont nilpotentes. Un produit fini d’algèbres de Lie nilpotentes est une algèbre de Lie nilpotente.

Soient g une algèbre de Lie, g' une sous-algèbre de g, h un idéal de g, \mathfrak{k} = g/h, et \varphi l’application canonique de g sur \mathfrak{k}. Si g est nilpotente, on a C^k g = \{0\} pour un entier k, donc C^k g' \subset C^k g = \{0\} et C^k \mathfrak{k} = \varphi(C^k g) = \{0\}, donc g' et \mathfrak{k} sont nilpotentes. Si \mathfrak{k} est nilpotente et h contenu dans le centre de g, on a C^k \mathfrak{k} = \{0\} pour un entier k, donc C^k g \subset h, et par suite C^{k+1} g \subset [h, g] = \{0\}, de sorte que g est nilpotente. Enfin, l’assertion relative aux produits résulte par exemple de l’assertion a) \Leftrightarrow d) de la prop. 1.

La définition 1 et la proposition 2 montrent que les algèbres de Lie nilpotentes sont exactement les algèbres obtenues à partir des algèbres de Lie commutatives par une suite d’extensions centrales.

#### Proposition 3 {#lie-i-s4-prop-3 .statement}

Soient g une algèbre de Lie nilpotente, h une sous-algèbre de g distincte de g. Le normalisateur de h dans g est distinct de h.

Soit k le plus grand entier tel que C^k g + h \neq h. Alors, [C^k g + h, h] \subset C^{k+1} g + h \subset h, donc le normalisateur de h dans g contient C^k g + h.

### 2. Le théorème d’Engel

#### Lemme 1 {#lie-i-s4-lem-1 .statement}

Soit V un espace vectoriel sur K. Si x est un endomorphisme nilpotent de V, l’application $ y \mapsto [x, y] $ de $ \mathcal{L}(V) $ dans $ \mathcal{L}(V) $ est nilpotente.

En effet, si f désigne cette application, $ f^m(y) $ est une somme de termes de la forme $ \pm x^i y x^j $ avec $ i + j = m $. Si $ x^k = 0 $, on a donc $ f^{2k-1}(y) = 0 $ pour tout $ y $.

#### Théorème 1 (Ergel) {#lie-i-s4-thm-1 .statement}

Soient V un espace vectoriel sur K, et g une sous-algèbre de dimension finie de $ \mathrm{gl}(V) $, dont les éléments sont des endomorphismes nilpotents de V. Si $ V \neq \{0\} $, il existe un $ u \neq 0 $ dans V tel que $ x.u = 0 $ pour tout $ x \in g $.

La démonstration procède par récurrence sur la dimension n de g. Le théorème est évident si $ n = 0 $. Supposons-le vrai pour les algèbres de dimension < n.

Soit $ \mathfrak{h} $ une sous-algèbre de Lie de g de dimension $ m < n $. Si $ x \in \mathfrak{h} $, $ \mathrm{ad}_g x $ applique $ \mathfrak{h} $ dans lui-même et définit par passage au quotient un endomorphisme $ \sigma(x) $ de l’espace $ g/\mathfrak{h} $. D’après le lemme 1, $ \mathrm{ad}_g x $ est nilpotent, donc $ \sigma(x) $ est nilpotent. En vertu de l’hypothèse de récurrence, il existe un élément non nul de $ g/\mathfrak{h} $ qui est annulé par tous les $ \sigma(x), x \in \mathfrak{h} $. Autrement dit, il existe $ y \in g, y \notin \mathfrak{h} $, tel que $ [x, y] \in \mathfrak{h} $ pour tout $ x \in \mathfrak{h} $. Il en résulte que $ \mathfrak{h} $ est un idéal dans une certaine sous-algèbre de dimension $ m + 1 $ de g.

On en conclut (par itération à partir de $ \mathfrak{h} = \{0\} $) que g possède un idéal $ \mathfrak{h} $ de dimension $ n - 1 $. Soit $ a \in g, a \notin \mathfrak{h} $. Faisons usage à nouveau de l’hypothèse de récurrence : les $ u \in V $ tels que $ x.u = 0 $ pour tout $ x \in \mathfrak{h} $ forment un sous-espace vectoriel non nul U de V. Ce sous-espace est stable pour $ a $ (\S 3, no 5, prop. 5). Puisque $ a $ est un endomorphisme nilpotent de V, il existe un élément non nul de U qui est annulé par $ a $, donc par tout élément de g.

#### Corollaire 1 {#lie-i-s4-thm-1-cor-1 .statement}

Pour qu’une algèbre de Lie g soit nilpotente, il faut et il suffit que, pour tout $ x \in g $, $ \mathrm{ad}\, x $ soit nilpotent.

La condition est nécessaire (prop. 1). Supposons démontrée sa suffisance pour les algèbres de Lie de dimension < n ($ n \neq 0 $). Soit g une algèbre de Lie de dimension n telle que, pour tout x \in g, \text{ ad } x \text{ soit nilpotent. Le théorème 1, appliqué à l’ensemble des ad } x\ (x \in g), \text{ prouve que le centre } c \text{ de } g \text{ est non nul. Alors, } g \text{ est extension centrale de l’algèbre de Lie } g/c, \text{ qui est nilpotente d’après notre hypothèse de récurrence. On conclut en appliquant la prop. 2.}

#### Corollaire 2 {#lie-i-s4-thm-1-cor-2 .statement}

*Soient g une algèbre de Lie, h un idéal de g. On suppose que g/h est nilpotente et que, pour tout x \in g, la restriction à h de ad x est nilpotente. Alors g est nilpotente.*

Soit x \in g. Comme g/h est nilpotente, il existe un entier k tel que (ad x)^k(g) \subset h. Par hypothèse, il existe un entier k' tel que (ad x)^{k'}(h) = \{0\}. Donc (ad x)^{k+k'} = \{0\}. Le cor. 2 est donc une conséquence du cor. 1.

#### Corollaire 3 {#lie-i-s4-thm-1-cor-3 .statement}

*Soient V un espace vectoriel, et g une sous-algèbre de dimension finie de gl(V) dont les éléments sont des endomorphismes nilpotents de V. Alors, g est une algèbre de Lie nilpotente.*

Ceci résulte aussitôt du lemme 1 et du cor. 1.

#### Exemple {#lie-i-s4-n2-exa-1 .statement}

L’algèbre n(n, K) (\S 1, no 2, ex. 2, 3°) est nilpotente.

### 3. Le plus grand idéal de nilpotence d’une représentation

#### Lemme 2 {#lie-i-s4-lem-2 .statement}

*Soient g une algèbre de Lie, a un idéal de g, M un g-module simple. Si, pour tout x \in a, x_M est nilpotent, alors x_M = 0 pour tout x \in a.*

En effet, soit N le sous-espace de M formé des m \in M tels que x_M . m = 0 pour tout x \in a. D’après le th. 1, N \neq \{0\}. D’autre part, pour tout y \in g, N est stable pour y_M (\S 3, no 5, prop. 5). Donc N = M, ce qui prouve le lemme.

#### Lemme 3 {#lie-i-s4-lem-3 .statement}

*Soient g une algèbre de Lie, a un idéal de g, M un g-module de dimension finie sur K et (M_i)_{0 \leq i \leq n} une suite de Jordan-Hölder du g-module M. Les conditions suivantes sont équivalentes :

a) pour tout x \in a, x_M est nilpotent ;

b) pour tout $ x \in \mathfrak{a} $, $ x_{\mathbf{M}} $ est dans le radical de l’algèbre associative $ A $ engendrée par 1 et les $ y_{\mathbf{M}} $, où $ y \in \mathfrak{g} $;
c) pour tout $ x \in \mathfrak{a} $, on a
$$
x_{\mathbf{M}}(M_0) \subset M_1,\ x_{\mathbf{M}}(M_1) \subset M_2,\ldots,\ x_{\mathbf{M}}(M_{n-1}) \subset M_n.
$$
Si ces conditions sont remplies, $ \mathfrak{a} $ est orthogonal à $ \mathfrak{g} $ pour la forme bilinéaire associée au $ \mathfrak{g}$-module $ M $.

$ b) \Rightarrow a) $ : comme $ A $ est de dimension finie sur $ K $, le radical de $ A $ est un idéal nilpotent ($ Alg. $, chap. VIII, § 6, n° 4, th. 3), donc tout élément de ce radical est nilpotent.

$ a) \Rightarrow c) $ : chaque $ Q_i = M_i/M_{i+1} $ ($ 0 \leq i < n $) est un $ \mathfrak{g}$-module simple. Pour tout $ x \in \mathfrak{a} $, l’endomorphisme $ x_{Q_i} $ (qui se déduit de $ x_{\mathbf{M}} $ par restriction à $ M_i $ et passage au quotient) est nilpotent si la condition $ a) $ est satisfaite, donc nul d’après le lemme 2 ; autrement dit, $ x_{\mathbf{M}}(M_i) \subset M_{i+1} $.

$ c) \Rightarrow b) $ : supposons satisfaite la condition $ c) $; soient $ x \in \mathfrak{a} $ et $ z \in A $. On a $ z(M_i) \subset M_i $ ($ 0 \leq i < n $), donc $ (zx_{\mathbf{M}})^n(M) = \{0\} $; ainsi $ Ax_{\mathbf{M}} $ est un nilidéal à gauche de $ A $, donc est contenu dans le radical de $ A $ ($ Alg. $, chap. VIII, § 6, n° 3, cor. 3 du th. 1).

Enfin, supposons satisfaites les conditions $ a),\ b),\ c) $. Soient $ x \in \mathfrak{a} $ et $ y \in \mathfrak{g} $. On vient de voir que $ y_{\mathbf{M}}x_{\mathbf{M}} $ est nilpotent, donc $ \operatorname{Tr}(y_{\mathbf{M}}x_{\mathbf{M}}) = 0 $, ce qui prouve la dernière assertion du lemme.

#### Proposition 4 {#lie-i-s4-prop-4 .statement}

Soient $ \mathfrak{g} $ une algèbre de Lie, $ M $ un $ \mathfrak{g}$-module de dimension finie sur $ K $, $ A $ l’algèbre associative engendrée par 1 et l’ensemble des $ x_{\mathbf{M}} $ ($ x \in \mathfrak{g} $).

a) Les idéaux $ \mathfrak{a} $ de $ \mathfrak{g} $, tels que $ x_{\mathbf{M}} $ soit nilpotent pour tout $ x \in \mathfrak{a} $, sont tous contenus dans l’un d’eux, $ \mathfrak{n} $.

b) L’idéal $ \mathfrak{n} $ est l’ensemble des $ x \in \mathfrak{g} $ tels que $ x_{\mathbf{M}} $ appartienne au radical de $ A $.

c) Soit $ (M_i)_{0 \leq i \leq n} $ une suite de Jordan-Hölder du $ \mathfrak{g}$-module $ M $; alors $ \mathfrak{n} $ est aussi l’ensemble des $ x \in \mathfrak{g} $ tels que $ (x)_{M_i/M_{i+1}} = 0 $ pour tout $ i $.

d) $ \mathfrak{n} $ est orthogonal à $ \mathfrak{g} $ pour la forme bilinéaire associée à $ \varphi $.

L’ensemble des $ x \in \mathfrak{g} $ tels que $ x_{\mathbf{M}} $ appartienne au radical de $ A $ est évidemment un idéal de $ \mathfrak{g} $. La proposition résulte alors aussitôt du lemme 3.

#### Définition 2 {#lie-i-s4-def-2 .statement}

L’idéal $ n $ de la prop. 4 s’appelle le plus grand idéal de nilpotence pour le $ g $-module $ M $, ou le plus grand idéal de nilpotence de la représentation correspondante.

Il est clair que $ n $ contient le noyau de cette représentation. Il lui est égal quand $ M $ est semi-simple (prop. 4 c)), mais non en général. On prendra garde qu’un élément $ x $ de $ g $ tel que $ x_M $ soit nilpotent n’appartient pas nécessairement à $ n $.

Notons par ailleurs qu’un cas particulier du lemme 3 fournit aussitôt le résultat suivant :

#### Proposition 5 {#lie-i-s4-prop-5 .statement}

Soient $ V $ un espace vectoriel de dimension finie $ n $ sur $ K $, et $ g $ une sous-algèbre de Lie de $ \mathrm{gl}(V) $ dont les éléments sont des endomorphismes nilpotents de $ V $. Alors, il existe une suite décroissante de sous-espaces vectoriels $ V_0, V_1, \ldots, V_n $ de $ V $, de dimensions $ n, n-1, \ldots, 0 $, tels que $ x(V_i) \subset V_{i+1} $ pour tout $ x \in g $ et tout $ i = 0, 1, \ldots, n-1 $.

### 4. Le plus grand idéal nilpotent d’une algèbre de Lie

Soient $ g $ une algèbre de Lie, $ a $ un idéal de $ g $. Pour que $ a $ soit nilpotent, il faut et il suffit que, pour tout $ x \in a $, $ \mathrm{ad}_g x $ soit nilpotent ; la condition, évidemment suffisante, est nécessaire, car, si $ a $ est nilpotent, et si $ x \in a $, $ \mathrm{ad}_a x $ est nilpotent et $ \mathrm{ad}_g x $ applique $ g $ dans $ a $, donc $ \mathrm{ad}_g x $ est nilpotent. Ceci posé, la prop. 4, appliquée à la représentation adjointe de $ g $, fournit le résultat suivant :

#### Proposition 6 {#lie-i-s4-prop-6 .statement}

Soient $ g $ une algèbre de Lie, $ E $ la sous-algèbre associative de $ \mathcal{L}(g) $ engendrée par 1 et les $ \mathrm{ad}_g x $ ($ x \in g $). Soit $ R $ le radical de $ E $.
a) L’ensemble $ n $ des $ y \in g $ tels que $ \mathrm{ad}_g y \in R $ est le plus grand idéal nilpotent de $ g $.
b) Il est orthogonal à $ g $ pour la forme de Killing.

On prendra garde que $ g/n $ peut avoir des idéaux nilpotents non nuls.

### 5. Extension du corps de base

Soient g une K-algèbre de Lie, K₁ une extension de K, et g' = g_{(K₁)}. Comme C^k g' = (C^k g)_{(K₁)}, g est nilpotente si et seulement si g' est nilpotente.

Soient M un g-module de dimension finie sur K, n le plus grand idéal de nilpotence pour M, et M' = M_{(K₁)}. Soit (M_i)_{0 \leq i \leq n} une suite de Jordan-Hölder du g-module M. On a x_M(M_i) \subset M_{i+1} pour tout i et tout x \in n, donc x'_M'((M_i)_{(K₁)}) \subset (M_{i+1})_{(K₁)} pour tout i et tout x' \in n_{(K₁)} ; donc x'_M' est nilpotent pour x' \in n_{(K₁)}, de sorte que n_{(K₁)} est contenu dans le plus grand idéal de nilpotence n' pour M'. Nous allons voir que, si K₁ est séparable sur K, alors n' = n_{(K₁)}. Soient E la K-algèbre associative engendrée par 1 et les x_M (x \in g), E' la K-algèbre associative engendrée par 1 et les x'_M' (x' \in g'), R et R' les radicaux de E et E'. L’algèbre E' s’identifie canoniquement à E_{(K₁)}. On a R' = R_{(K₁)} (Alg., chap. VIII, § 7, no 2, cor. 2 c) de la prop. 3). Ceci posé, soit y' \in n', et écrivons y' = \sum_{i=1}^n \lambda_i y_i, où les y_i sont dans g et où les \lambda_i \in K₁ sont linéairement indépendants sur K. On a y'_M' = \sum_{i=1}^n \lambda_i (y_i)_M', et y'_M' \in R' = R_{(K₁)}. Donc (y_i)_M \in R, et par suite y_i \in n pour tout i. On en conclut que y' \in n_{(K₁)}, d’où n' \subset n_{(K₁)}.

En particulier, si K₁ est séparable sur K, le plus grand idéal nilpotent de g_{(K₁)} se déduit de celui de g par extension de K à K₁ du corps de base.

## EXERCICES {#lie-i-s4-exercises}

Les conventions du § 4 restent valables, sauf mention contraire.

See the [exercises for § 4](exercises/s4/).
