---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 5
section_title: Variétés
lang: fr
source: var-fr
pdf_pages: 0033-0058
extraction: ocr
subsections:
    - "no": 1
      title: Cartes et atlas. Variétés
      page: 0
      pdf_page: 33
    - "no": 2
      title: Exemples de variétés
      page: 0
      pdf_page: 35
    - "no": 3
      title: Fonctions de classe $C^r$ et morphismes de variétés
      page: 0
      pdf_page: 36
    - "no": 4
      title: Caractérisation des variétés par leurs faisceaux de fonctions
      page: 0
      pdf_page: 38
    - "no": 5
      title: Espaces tangents, applications linéaires tangentes
      page: 0
      pdf_page: 39
    - "no": 6
      title: Produits de variétés
      page: 0
      pdf_page: 42
    - "no": 7
      title: Immersions, morphismes étales
      page: 0
      pdf_page: 43
    - "no": 8
      title: Images inverses de structures de variété, sous-variétés
      page: 0
      pdf_page: 45
    - "no": 9
      title: Submersions et variétés quotients
      page: 0
      pdf_page: 48
    - "no": 10
      title: Subimmersions
      page: 0
      pdf_page: 50
    - "no": 11
      title: Produits fibrés et images réciproques
      page: 0
      pdf_page: 51
    - "no": 12
      title: Variétés de groupes
      page: 0
      pdf_page: 54
    - "no": 13
      title: Affaiblissement de structure
      page: 0
      pdf_page: 56
    - "no": 14
      title: Restriction du corps de base
      page: 0
      pdf_page: 56
statements: 0
exercises: 0
content_sha256: dd71956a97de3213da051d44a027f3c8f14a9f8fda6946fb9eaa04f9cbbd04ed
---

## § 5. Variétés

### 5.1. Cartes et atlas. Variétés

5.1.1. Soit X un ensemble. On appelle carte de X un triplet c = (U, φ, E), où U est une partie de X, E un espace de Banach et φ une bijection de U sur un ouvert de E. On dit que U est le domaine de la carte c. Si E est de dimension finie n, on dit que c est de dimension n. Sinon, on pose dim c = +∞.

5.1.2. On dit que deux cartes c = (U, φ, E) et c' = (U', φ', E') de X sont C^r-compatibles (ou simplement compatibles lorsqu’il ne peut y avoir d’ambiguïté sur r) lorsque les conditions suivantes sont réalisées:
(a) φ(U ∩ U') (resp. φ'(U ∩ U')) est ouvert dans E (resp. E');
(b) l’application φ ∘ φ'^{-1} (resp. φ' ∘ φ^{-1}) de φ'(U ∩ U') sur φ(U ∩ U') (resp. de φ(U ∩ U') sur φ'(U ∩ U')) est de classe C^r (cf. 2.3.1, 3.2.1 et 4.2.1).

5.1.3. On appelle C^r-atlas (ou simplement atlas) d’un ensemble X un ensemble de cartes de X deux à deux C^r-compatibles et dont les domaines ont pour réunion X tout entier. Deux atlas A et B de X sont dits C^r-équivalents si A ∪ B est un atlas. La relation de C^r-équivalence entre atlas est une relation d’équivalence.

5.1.4. Soit S un ensemble d’espaces de Banach. On dit qu’un atlas A est de type S si l’on a E ∈ S pour toute carte c = (U, φ, E) de A. D’une manière analogue, on dit qu’un atlas A est de type hilbertien (resp. de type hilbertien de dimension dénombrable) si E est un espace hilbertien (resp. hilbertien de type dénombrable) pour toute carte (U, φ, E) de A.

5.1.5. On appelle K-variété de classe C^r (ou variété de classe C^r sur K, ou simplement variété lorsque il ne peut y avoir d’ambiguïté sur K et r) un ensemble X muni d’une classe d’atlas équivalents (Ens., chap. II, § 6, n° 9) pour la relation de C^r-équivalence. Un atlas de cette classe est appelé un atlas de la variété X. Une carte appartenant à un atlas de X est appelée une carte de la variété X. Une carte de X dont le domaine contient un point a ∈ X est appelée une carte de X en a. Une carte centrée en a est une carte (U, φ, E) de X en a telle que φ(a) = 0.

Si X est un ensemble et A un atlas de X, l’ensemble X muni de la classe d’équivalence de A est appelé la variété définie par A.

Lorsque r ≠ ω (donc K = R), une variété de classe C^r est parfois appelée une variété différentielle. Une variété de classe C^ω est encore appelée une variété analytique sur K (ou encore variété K-analytique).

Lorsque de plus $K = \mathbf{R}$ (resp. $\mathbf{C}$, $\mathbf{Q}_p$), on dit encore variété analytique réelle (resp. analytique complexe, analytique $p$-adique).

5.1.6. Soit $X$ une variété. Les parties de $X$ qui sont réunions de domaines de cartes de $X$ forment l’ensemble des ouverts pour une topologie sur $X$, dite sous-jacente à la structure de variété de $X$. Pour toute carte $c = (U, \varphi, E)$ de $X$, l’application $\varphi$ est un homéomorphisme de l’ouvert $U$ muni de la topologie induite par celle de $X$ sur l’ouvert $\varphi(U)$ de $E$.

L’espace topologique sous-jacent à $X$ est un espace de Baire. Lorsque $K$ est égal à $\mathbf{R}$ ou $\mathbf{C}$, il est localement connexe.

Soit $X$ une variété et soit $\mathcal{A}$ un atlas de $X$. Pour que l’espace topologique $X$ soit séparé, il faut et il suffit que la condition suivante soit satisfaite : quelles que soient les cartes $(U, \varphi, E)$ et $(V, \psi, F)$ appartenant à l’atlas $\mathcal{A}$, le graphe de l’application $\psi \circ \varphi^{-1}$ de $\varphi(U \cap V)$ dans $\psi(U \cap V)$ est fermé dans $\varphi(U) \times \psi(V)$.

Soit $X$ une variété ; supposons que l’espace topologique $X$ soit régulier. Alors pour tout point $a \in X$, il existe une carte $(U, \varphi, E)$ de $X$ en $a$ possédant la propriété suivante : pour qu’une partie $Y$ de $U$ soit fermée dans $X$, il faut et il suffit que son image $\varphi(Y)$ soit fermée dans $E$. Si l’espace $X$ est paracompact, il existe sur $X$ une distance compatible avec la topologie de $X$ et faisant de $X$ un espace métrique complet.

5.1.7. Soit $\mathfrak{S}$ un ensemble d’espaces de Banach. On dit qu’une variété est de type $\mathfrak{S}$ (resp. de type hilbertien, resp. de type hilbertien de dimension dénombrable) si elle possède un atlas de type $\mathfrak{S}$ (resp. de type hilbertien, resp. de type hilbertien de dimension dénombrable). Si $\mathfrak{S}$ est réduit à un seul élément $E$, une variété de type $\mathfrak{S}$ est encore appelée une variété pure de type $E$.

On appelle variété pure de dimension $n$ une variété pure de type $K^n$. On dit qu’une variété est localement de dimension finie si elle est de type $\mathfrak{S}$ avec $\mathfrak{S} = \{ K^n ; n \in \mathbf{N} \}$.

5.1.8. Soit $X$ une variété et soit $x \in X$. La dimension (finie ou $+\infty$) d’une carte de $X$ en $x$ ne dépend que de $x$. On l’appelle dimension de $X$ en $x$ et on la note $\dim_x X$. On appelle dimension de $X$ et on note $\dim X$ la borne supérieure des $\dim_x X$ pour $x \in X$.

La fonction $x \mapsto \dim_x X$ est localement constante. La variété $X$ est localement de dimension finie (resp. pure de dimension $n$) si et seulement si on a $\dim_x X < +\infty$ (resp. $\dim_x X = n$) pour tout $x \in X$.

5.1.9. Supposons $K$ localement compact. Soit $X$ une variété séparée. Alors, pour que $X$ soit localement de dimension finie, il faut et il suffit que $X$ soit localement compacte.

n° 5.2

5.1.10. Soit X une variété et soient $\xi^1, \ldots, \xi^n$ des applications d'une partie U de X dans K. On dit que $\xi = (\xi^1, \ldots, \xi^n)$ est un système de coordonnées de X dans U si le triplet $(U, \xi, K^n)$ est une carte de X ; cette carte se note aussi $(U; \xi)$ ou $(U; \xi^1, \ldots, \xi^n)$. Si $a \in U$, on dit aussi que $\xi$ est un système de coordonnées de X en $a$ ; si de plus $\xi^i(a) = 0$ pour $i = 1, 2, \ldots, n$, on dit que le système de coordonnées $\xi$ est centré en $a$.

### 5.2. Exemples de variétés

5.2.1. Soit X un ensemble ; il existe sur X une structure de variété et une seule pour laquelle l'espace topologique sous-jacent soit discret ; cette structure est une structure de variété pure de dimension 0.

5.2.2. Soit E un espace de Banach. Le triplet $c = (E, \mathrm{Id}_E, E)$ est une carte de E et $\mathcal{A} = \{c\}$ est un atlas de E, donc définit une structure de variété pure de type E sur E ; la topologie sous-jacente est la topologie donnée sur E. Lorsque l'on parlera par la suite de la structure de variété sur E, ce sera toujours à la structure précédente que l'on se référera.

En particulier, ceci s'applique à tout espace vectoriel de dimension finie sur K, muni de l'unique topologie séparée compatible avec sa structure vectorielle (Esp. Vect. Top., chap. I, § 2, n° 3).

5.2.3. Soient X une variété et U une partie ouverte de X. Il existe sur U une structure de variété dont les cartes sont les cartes de la variété X de domaine contenu dans U. Cette structure est dite induite par celle de X (cf. n° 5.3.4); muni de cette structure, U s'appelle une sous-variété ouverte de X.

En particulier, tout ouvert d'un espace de Banach E est muni d'une structure canonique de variété pure de type E. Soit X une variété ; pour qu'un triplet $(U, \varphi, E)$ soit une carte de X, il faut et suffit que U soit ouvert dans X et que $\varphi$ soit un isomorphisme de la sous-variété ouverte U de X sur une sous-variété ouverte de E.

5.2.4. Soient X un ensemble, et $(X_i)_{i \in I}$ un recouvrement de X. On suppose donnée sur chaque $X_i$ une structure de variété telle que la condition suivante soit remplie :

Quels que soient $i$ et $j$ dans I, l'ensemble $X_i \cap X_j$ est ouvert dans $X_i$ et $X_j$ et les structures de variétés induites sur $X_i \cap X_j$ par celles de $X_i$ et $X_j$ coïncident.

Il existe alors sur X une structure de variété et une seule telle que $X_i$ soit une sous-variété ouverte de X pour tout $i$ dans I. On dit que la variété X s'obtient par recollement des variétés $X_i$.

5.2.5. Soit X une variété. L'ensemble $X_n$ des points $x$ de X tels que dim_x X = n (n entier $\geq 0$) est une sous-variété ouverte de X, qui est pure de dimension n.

5.2.6. Soit E un espace de Banach. On peut munir l’ensemble G(E) des sous-espaces vectoriels de E admettant un supplémentaire topologique d’une structure de variété analytique de la façon suivante : pour tout couple (F_0, G_0) $\in G(E) \times G(E)$ tel que E = F_0 $\oplus$ G_0, on note U_{G_0} l’ensemble des F $\in G(E)$ admettant G_0 comme supplémentaire, et on définit une bijection $\varphi_{F_0, G_0}$ de U_{G_0} sur l’espace de Banach $\mathcal{L}(F_0; G_0)$ en associant à tout F $\in U_{G_0}$ l’application de F_0 dans G_0 ayant pour graphe le sous-espace F de E = F_0 $\times$ G_0. Les cartes (U_{G_0}, $\varphi_{F_0, G_0}$, $\mathcal{L}(F_0; G_0)$) forment un atlas de G(E). Muni de la structure de variété définie par cet atlas, G(E) s’appelle la variété grassmannienne de E.

L’espace topologique G(E) est métrisable. Si K est localement compact et E de dimension finie, G(E) est compacte.

Pour tout entier $n \geq 0$, l’ensemble G_n(E) (resp. G^n(E)) des F $\in G(E)$ de dimension (resp. codimension) n est ouvert et fermé dans G(E) et est une sous-variété ouverte pure de G(E). Si K = R ou C, G_n(E) est connexe pour tout n.

L’application qui à F $\in G(E)$, associe son orthogonal dans le dual E’ de E, est un morphisme de G(E) dans G(E’) qui induit un isomorphisme de G^n(E) sur G_n(E’) pour tout entier n.

Si K = R ou C, ou si E est de dimension finie, G_1(E) n’est autre que l’espace projectif déduit de E, qui se trouve ainsi muni d’une structure de variété analytique.

### 5.3. Fonctions de classe $C^r$ et morphismes de variétés

5.3.1. Soient X une variété de classe C', F un espace polynormé séparé et f une application de X dans F. On dit que f est de classe C' si pour toute carte (V, $\varphi$, E) de X, l’application $f \circ \varphi^{-1}$ de $\varphi(V)$ dans F est de classe C'. Pour cela, il suffit que cette condition soit satisfaite pour les cartes d’un atlas de X. L’ensemble des applications de classe C' de X dans F forme un sous-espace vectoriel de l’espace de toutes les applications de X dans F. On le note $\mathcal{C}'(X; F)$.

Lorsque F = K, on pose $\mathcal{C}'(X; K) = \mathcal{C}'(X)$; c’est une sous-K-algèbre de l’algèbre des applications de X dans K. Les éléments de $\mathcal{C}'(X)$ sont encore appelés fonctions morphiques.

Lorsque X est un ouvert d’un espace de Banach, cette terminologie est en accord avec celle des n°s 2.3.1, 3.2.1 et 4.2.1.

5.3.2. Soient X et Y deux variétés de classe C' et soit f une application de X dans Y. On dit que f est de classe C' ou est un morphisme de variétés (de classe C') si elle est continue et si, pour toute carte (V, $\psi$, F) de Y, l’application $\psi \circ f$ de la sous-variété ouverte $f^{-1}(V)$ dans l’espace de Banach F est de classe $C'$. Pour cela, il suffit qu’il existe un atlas $\mathcal{A}$ de Y tel que, pour toute carte $(V, \psi, F) \in \mathcal{A}$, l’ensemble $f^{-1}(V)$ soit ouvert dans X et que l’application $\psi \circ f$ de la sous-variété ouverte $f^{-1}(V)$ de X dans F soit de classe $C'$. L’ensemble des morphismes de X dans Y est noté $\mathcal{C}'(X; Y)$. Lorsque Y est un espace de Banach muni de sa structure canonique de variété, les définitions de 5.3.1. et 5.3.2 sont cohérentes. Une application de classe $C^\omega$ est aussi appelée *application K-analytique* (ou simplement analytique). Lorsque $K = \mathbf{C}$, on dit aussi application holomorphe.

Soient $(U, \varphi, E)$ une carte de X et $(V, \psi, F)$ une carte de Y telles que $f(U) \subset V$. L’application $\psi \circ f \circ \varphi^{-1}$ de l’ouvert $\varphi(U)$ de E dans l’ouvert $\psi(V)$ de F est appelée *l’expression de f* dans les cartes données.

5.3.3. Supposons X et Y de dimension finie; soient $a \in X,\ b \in Y$ et $f$ une application de X dans Y avec $f(a) = b$. Supposons d’abord que $f$ soit de classe $C'$ et considérons des systèmes de coordonnées $(U; \xi^1, \ldots, \xi^m)$ de X en $a$ et $(V; \eta^1, \ldots, \eta^n)$ de Y en $b$ respectivement, avec $f(U) \subset V$. Soit $\xi$ l’application $(\xi^1, \ldots, \xi^m)$ de U dans $K^m$. Il existe alors des fonctions $u^j$ de classe $C'$ sur l’ouvert $\xi(U)$ de $K^m$, à valeurs dans K, telles que les coordonnées d’un point $y = f(x)$ de Y, (pour x dans U), soient données par les formules:

(1)
$$
\eta^j(y) = u^j(\xi^1(x), \ldots, \xi^m(x)) \quad \text{pour } 1 \leq j \leq n
$$
ce qui équivaut à:

(2)
$$
\eta^j \circ f = u^j(\xi^1, \ldots, \xi^m) \quad \text{pour } 1 \leq j \leq n.
$$
On dit que les formules précédentes constituent *l’expression* de $f$ au moyen des systèmes de coordonnées choisis.

Réciproquement, si, pour tout point $a$ de X, on peut trouver *un* système de coordonnées de X en $a$ et *un* système de coordonnées de Y en $b = f(a)$ satisfaisant aux conditions précédentes, alors $f$ est de classe $C'$.

5.3.4. Les morphismes de variétés satisfont aux axiomes d’*Ens.*, chap. IV, § 2:
a) Le composé de deux morphismes est un morphisme.
b) Pour qu’une bijection $f : X \to Y$ soit un isomorphisme, il faut et il suffit que $f$ et $f^{-1}$ soient des morphismes.

5.3.5. Supposons que $r = \omega$. Soient X une variété et $f, g$ deux applications analytiques de X dans un espace polynormé séparé ou dans une variété analytique séparée. L’ensemble des points au voisinage desquels $f$ et $g$ sont égales, est *ouvert et fermé* dans X.

5.3.6. Supposons que $K = \mathbf{R}$ et $r \neq \omega$. On dit qu'une variété $X$ *admet des partitions de l'unité de classe* $C'$ si, pour tout recouvrement ouvert localement fini de $X$, il existe une partition continue de l'unité (*Top. Gén.*, ch. IX, § 4, n° 3) subordonnée à ce recouvrement et formée de fonctions de classe $C'$.

Soit $E$ un espace de Banach ; considérons la propriété suivante :

(PU) *Quels que soient les sous-ensembles fermés disjoints* $A$ *et* $B$ *de* $E$, *il existe une fonction* $f$ *de classe* $C'$ *sur* $E$, *à valeurs dans* $\mathbf{R}$, *telle que* $f(x) = 0$ *pour* $x \in A$, $f(x) = 1$ *pour* $x \in B$ *et* $0 \leq f(x) \leq 1$ *pour tout* $x \in E$.

Si $\mathcal{S}$ est un ensemble d’espaces de Banach possédant la propriété (PU), toute variété paracompacte de type $\mathcal{S}$ admet des partitions de l’unité de classe $C'$.

Tout espace de dimension finie, tout espace hilbertien de type dénombrable possède la propriété (PU).

5.3.7. Supposons $K$ ultramétrique. Soit $X$ une variété paracompacte. Pour tout recouvrement ouvert $U$ de $X$, il existe une partition de $X$ en sous-ensembles ouverts et fermés subordonnée au recouvrement $U$.

5.3.8. Supposons $K$ localement compact. Soient $X$ et $Y$ deux variétés pures de dimension finie, et soit $f$ un morphisme de $X$ dans $Y$. Si $\dim X < \dim Y$ et si la topologie de $X$ admet une base dénombrable d’ouverts, $f(X)$ est *maigre* dans $Y$.

### 5.4. Caractérisation des variétés par leurs faisceaux de fonctions

5.4.1. Soit $X$ un espace topologique, et soit $Y$ un ensemble. Supposons donné, pour tout ouvert $U$ de $X$, un ensemble $\mathcal{L}(U)$ d’applications de $U$ dans $Y$. Nous dirons que la famille $\mathcal{L} = \{\mathcal{L}(U)\}$ est un *faisceau de fonctions à valeurs dans* $Y$ si elle vérifie la condition suivante :

*Soit* $(U_i)_{i \in I}$ *une famille d’ouverts de* $X$, *de réunion* $U$, *et soit* $f$ *une application de* $U$ *dans* $Y$; *pour que* $f$ *appartienne à* $\mathcal{L}(U)$, *il faut et il suffit que* $f|U_i$ *appartienne à* $\mathcal{L}(U_i)$ *pour tout* $i$ *dans* $I$.

5.4.2. Soient $X$ et $Y$ deux variétés ; pour tout ouvert $U \subset X$, soit $\mathcal{L}(U)$ l’ensemble des morphismes de $U$ dans $Y$; alors $\mathcal{L}$ est un faisceau de fonctions à valeurs dans $Y$.

Lorsque $Y = K$, on note $\mathscr{C}_X^{r'}$ le faisceau ainsi défini.

5.4.3. Soit $X$ un espace topologique et soit $\mathcal{S}$ un ensemble d’espaces de Banach. Pour tout $E \in \mathcal{S}$, soit $\mathcal{F}_E$ un faisceau de fonctions sur $X$ à valeurs dans $E$. Supposons que la famille des $\mathcal{F}_E$, pour $E \in \mathcal{S}$, vérifie la condition suivante :

Pour tout $x \in X$, il existe un voisinage ouvert $U$ de $x$, un espace

$E_0 \in \mathcal{S}$, et un homéomorphisme $\varphi$ de U sur un ouvert de E_0, tels que, pour tout ouvert $V \subset U$ et tout $E \in \mathcal{S}$, l’ensemble $\mathcal{F}_E(V)$ se compose des fonctions $g \circ \varphi$, où $g$ parcourt l’espace $\mathcal{C}^r(\varphi(V); E)$.

Il existe alors sur X une structure de variété de classe $C^r$ et de type $\mathcal{S}$ et une seule, compatible avec la topologie donnée sur X et pour laquelle $\mathcal{F}_E$ est le faisceau des fonctions de classe $C^r$ sur X à valeurs dans E.

5.4.4. Soit X un espace topologique et soit $\mathcal{F}$ un faisceau de fonctions à valeurs dans K, vérifiant la condition suivante : pour tout point x de X, il existe un entier n, un voisinage ouvert U de x et un homéomorphisme $\varphi$ de U sur un ouvert de $K^n$, tels que, pour tout ouvert V de U, l’ensemble $\mathcal{F}(V)$ se compose des fonctions $g \circ \varphi$ où $g$ parcourt l’ensemble des fonctions de classe $C^r$ à valeurs dans K sur l’ouvert $\varphi(V)$ de $K^n$.

Il existe alors sur X une structure de variété localement de dimension finie et de classe $C^r$ et une seule telle que $\mathcal{F} = \mathcal{C}^r_X$.

5.4.5. Soient X et X' deux variétés de classe $C^r$, localement de dimension finie, et soit $f$ une application continue de X dans X'. Pour que $f$ soit un morphisme, il faut et il suffit que pour tout ouvert U' de X' et toute fonction $g \in \mathcal{C}^r(U'; K)$, la fonction $g \circ f$ appartienne à $\mathcal{C}^r(U; K)$, avec $U = f^{-1}(U')$.

### 5.5. Espaces tangents, applications linéaires tangentes

5.5.1. Soit X une variété et soit $a \in X$. Considérons les couples $(c, h)$ où $c = (U, \varphi, E)$ est une carte de la variété X en $a$ et où $h$ est un élément de E. Deux tels couples $(c, h)$ et $(c', h')$ sont dits équivalents si la dérivée en $\varphi(a)$ de l’application $\varphi' \circ \varphi^{-1}$ (qui est définie sur un voisinage de $\varphi(a)$) transforme $h$ en $h'$. On obtient ainsi une relation d’équivalence entre couples $(c, h)$ et on appelle vecteur tangent en $a$ à X une classe de couples $(c, h)$ équivalents (Ens., chap. II, § 6, n° 9).

Les vecteurs tangents en $a$ à X forment un ensemble noté $T_a(X)$. Si $c = (U, \varphi, E)$ est une carte de la variété X en $a$, l’application $\theta_c$ de E dans $T_a(X)$ qui associe à un élément $h$ de E le vecteur tangent représenté par le couple $(c, h)$ est une bijection. Si l’on transporte à $T_a(X)$, au moyen de $\theta_c$, la structure de K-espace vectoriel topologique de E, la structure ainsi obtenue ne dépend pas du choix de $c$ et fait de $T_a(X)$ un espace de Banach, appelé espace tangent à X en $a$. La dimension (finie ou $+\infty$) de $T_a(X)$ est égale à la dimension de X en $a$.

5.5.2. Soient X, Y deux variétés, $f$ un morphisme de X dans Y et $a$ un point de X. Considérons une carte $c = (U, \varphi, E)$ de X en $a$ et une carte $c' = (V, \psi, F)$ de Y en $b$ avec $f(U) \subset V$; l’application $\Phi = \psi \circ f \circ \varphi^{-1}$ de $\varphi(U)$ dans F est de classe $C^r$, et sa dérivée $D\Phi(\varphi(a))$ au point $\varphi(a)$ est une application linéaire continue de E dans F. L’application linéaire continue $\theta_{c'} \circ D\Phi(\varphi(a)) \circ \theta_c^{-1}$ de $T_a(X)$ dans $T_b(Y)$ ne dépend pas des cartes $c$ et $c'$ choisies; on la note $T_a(f)$ et on l’appelle l’application linéaire tangente à $f$ en $a$. Si $g$ est un morphisme de $Y$ dans une variété $Z$, on a:

$$
T_a(g \circ f) = T_{f(a)}(g) \circ T_a(f).
$$

5.5.3. Soit $f : X \to Y$ un morphisme de variétés. Si $f$ est localement constant, on a $T_a(f) = 0$ pour tout $a$ dans $X$. Réciproquement, si $T_a(f) = 0$ pour tout $a \in X$ et si le corps $K$ est de caractéristique 0, alors $f$ est localement constant.

5.5.4. Soient $U$ un ouvert d’une variété $X$ et $f$ l’injection canonique de $U$ dans $X$; pour tout point $a$ de $U$, l’application $T_a(f)$ de $T_a(U)$ dans $T_a(X)$ est un isomorphisme d’espaces vectoriels topologiques, par lequel on identifiera désormais ces deux espaces.

5.5.5. Soit $U$ un ouvert d’un espace de Banach $E$; si $\iota$ est l’injection canonique de $U$ dans $E$, le triplet $c = (U, \iota, E)$ est une carte de $U$, et l’atlas $\{c\}$ définit la structure de variété de $U$. Etant donné un point $a$ de $U$, l’application $\theta_c$ est un isomorphisme d’espaces vectoriels topologiques de $E$ sur $T_a(U)$; l’isomorphisme réciproque sera noté $\zeta_E(a)$.

Soit $f$ une application de classe $C^r$ de $U$ dans un ouvert $V$ d’un espace de Banach $F$; pour tout point $a$ de $U$, on a:

$$
Df(a) \circ \zeta_E(a) = \zeta_F(f(a)) \circ T_a(f)
$$

où $Df(a)$ est la dérivée de $f$ en $a$ (1.2.1). Autrement dit, le diagramme :

$$
\begin{array}{ccc}
T_a(U) & \xrightarrow{T_a(f)} & T_{f(a)}(V) \\
\downarrow \zeta_E(a) & & \downarrow \zeta_F(f(a)) \\
E & \xrightarrow{Df(a)} & F
\end{array}
$$

est commutatif.

5.5.6. On appelle vecteur cotangent à $X$ en $a$, ou encore covecteur tangent ou simplement covecteur en $a$, toute forme linéaire continue sur l’espace vectoriel topologique $T_a(X)$; ces covecteurs sont donc les éléments du dual topologique $T_a(X)'$ de l’espace tangent à $X$ en $a$. On munira cet espace de la topologie de la convergence uniforme sur les parties bornées de $T_a(X)$: muni de cette topologie, $T_a(X)'$ est un espace de Banach qu’on appelle espace cotangent à $X$ en $a$. On le note aussi $T'_a(X)$.

Soit $f$ un morphisme de $X$ dans un espace de Banach $E$. On appelle différentielle de $f$ en $a$ et on note $d_a f$ ou $df_a$ l’application linéaire continue $\zeta_E(f(a)) \circ T_a(f)$ de $T_a(X)$ dans $E$. Pour $t \in T_a(X)$, on note parfois t(f) ou t . f la valeur $d_a f(t)$ de l’application linéaire $d_a f$ au point $t$. L’application $f \mapsto d_a f$ est linéaire.

Si $E = K$, la différentielle $d_a f$ de $f$ en $a$ est un covecteur de $X$ en $a$.

Soient $E, F, G$ trois espaces de Banach et soit $(u, v) \mapsto u . v$ une application bilinéaire continue de $F \times G$ dans $E$. Soit $f$ (resp. $g$) un morphisme de $X$ dans $F$ (resp. $G$). Alors l’application $f . g : x \mapsto f(x) . g(x)$ est un morphisme de $X$ dans $E$ et on a, pour tout $t \in T_a(X)$:

$$
d_a(f . g)(t) = f(a) . d_a g(t) + d_a f(t) . g(a).
$$

Prenons en particulier $G = E$ et $F = K$, l’application bilinéaire considérée étant la multiplication. On a alors:

$$
d_a(fg) = f(a)d_ag + g(a)\ d_af.
$$

5.5.7. Soit $X$ une variété localement de dimension finie et soient $\xi^1, \ldots, \xi^m$ des fonctions morphiques définie dans un voisinage ouvert $U$ d’un point $a$ de $X$. Les conditions suivantes sont équivalentes :

(i) il existe un voisinage ouvert $V$ de $a$ contenu dans $U$, tel que les fonctions $\xi^i|V$ (pour $1 \leq i \leq m$) forment un système de coordonnées de $X$ dans $V$;

(ii) les différentielles $d_a \xi^i$ pour $1 \leq i \leq m$ forment une base de $T_a(X)'$;

(iii) l’application $\xi = (\xi^1, \ldots, \xi^m)$ de $U$ dans $K^m$ est étale en $a$ (voir n° 5.7.6).

Pour que les différentielles $d_a \xi^1, \ldots, d_a \xi^m$ soient linéairement indépendantes, il faut et il suffit qu’il existe un voisinage $V$ de $a$, contenu dans $U$, tel que les fonctions $\xi^i|V$ fassent partie d’un système de coordonnées de $X$ dans $V$.

5.5.8. Soit $X$ une variété localement de dimension finie et soit $\xi = (\xi^1, \ldots, \xi^m)$ un système de coordonnées de $X$ dans un ouvert $U$. Soit $a \in U$: on note $(\partial_{1,a}, \ldots, \partial_{m,a})$ la base de l’espace tangent $T_a(X)$ duale de la base $(d_a \xi^1, \ldots, d_a \xi^m)$ de $T_a(X)'$. On a donc:

$$
\partial_{i,a}(\xi^j) = \delta_{i,j} \quad \text{(indice de Kronecker)}.
$$

Le vecteur tangent $\partial_{i,a}$ se note aussi $(\partial/\partial \xi^i)_a$.

Soit $f$ une fonction de classe $C^r$ sur $U$, à valeurs dans un espace de Banach $E$. On note $\partial_i f$ ou $\partial f/\partial \xi^i$ la fonction $a \mapsto \partial_{i,a}(f)$: c’est une fonction de classe $C^{r-1}$ sur $U$ à valeurs dans $E$ (une fonction continue si $r = 1$). Sa valeur en un point $a$ de $U$ est parfois notée $(\partial f/\partial \xi^i)_a$. Pour tout $t \in T_a(X)$, on a:

$$
d_a f(t) = \sum_{i=1}^m d_a \xi^i(t) \frac{\partial f}{\partial \xi^i}(a),
$$

ce qui peut encore s'écrire:

$$
d_a f = \sum_{i=1}^m \frac{\partial f}{\partial \xi^i}(a) d_a \xi^i.
$$

Ces notations sont cohérentes avec celles de 1.6.3.

5.5.9. Soient $X$ et $Y$ deux variétés et $f$ un morphisme de $X$ dans $Y$. On appelle *rang de* $f$ en un point $a$ de $X$, et on note $\mathrm{rg}_a f$, le rang (fini ou égal à $+\infty$) de l’application linéaire $T_a(f)$. L’application $a \mapsto \mathrm{rg}_a f$ est semi-continue inférieurement.

### 5.6. Produits de variétés

5.6.1. Soient $X$ et $X'$ deux ensembles et soit $c = (U, \varphi, E)$ (resp. $c' = (U', \varphi, E')$) une carte de $X$ (resp. $X'$). Le triplet

$$
(U \times U', \varphi \times \varphi', E \times E')
$$

est une carte de l’ensemble produit $X \times X'$, notée $c \times c'$.

5.6.2. Soient $X$ et $X'$ deux variétés de classe $C^r$. Il existe sur l’ensemble produit $X \times X'$ une structure de variété de classe $C^r$ et une seule telle que $c \times c'$ soit une carte de $X \times X'$ pour toute carte $c$ de $X$ et toute carte $c'$ de $X'$. Muni de cette structure, $X \times X'$ s’appelle la *variété produit* des variétés $X$ et $X'$. On définit de même le produit d’un nombre fini quelconque de variétés. La topologie de la variété $X \times X'$ est la topologie produit des topologies de $X$ et de $X'$. Pour $a \in X$ et $b \in X'$, on a:

$$
\dim_{(a,b)}(X \times X') = \dim_a X + \dim_b X'.
$$

5.6.3. Soient $X$ et $X'$ deux variétés, et soit $X \times X'$ leur produit. Soit $a \in X$ et soit $a' \in X'$. Les projections canoniques

$$
\mathrm{pr}_1 : X \times X' \to X \quad \text{et} \quad \mathrm{pr}_2 : X \times X' \to X'
$$

sont des morphismes. Soient $\pi_i \ (i = 1, 2)$ leurs applications linéaires tangentes au point $(a, a')$. L’application

$$
(\pi_1, \pi_2) : T_{(a,a')}(X \times X') \to T_a(X) \times T_{a'}(X')
$$

est un *isomorphisme*, ce qui permet *d’identifier l’espace tangent à* $X \times X'$ *en* $(a, a')$ *au produit* $T_a(X) \times T_{a'}(X')$.

L’injection de $T_a(X)$ dans $T_{(a,a')}(X \times X')$ résultant de cette identification est l’application linéaire tangente en $a$ au morphisme $x \mapsto (x, a')$ de $X$ dans $X \times X'$; on a un résultat analogue pour l’injection de $T_{a'}(X')$ dans $T_{(a,a')}(X \times X')$.

5.6.4. Soient $W, X$ et $X'$ trois variétés, et soient $f : W \to X, f' : W \to X'$ deux applications. Pour que l’application

$$
(f, f') : W \to X \times X'
$$

soit un morphisme, il faut et il suffit que $f$ et $f'$ soient des morphismes (cela justifie l’emploi du terme « produit », cf. Ens., chap. IV, § 2, n° 4). Dans ce cas, si $a$ est un point de $W$, on a:

$$
T_a(f, f') = (T_a(f), T_a(f'))
$$

compte tenu de l’identification faite ci-dessus.

5.6.5. Soient $f : X \to Y$ et $f' : X' \to Y'$ des morphismes de variétés. Alors $f \times f' : X \times X' \to Y \times Y'$ est un morphisme. Si $a \in X$ et $a' \in X'$, on a:

$$
T_{(a, a')}(f \times f') = T_a(f) \times T_{a'}(f')
$$
$$
\mathrm{rg}_{(a, a')}(f \times f') = \mathrm{rg}_a f + \mathrm{rg}_{a'} f'.
$$

5.6.6. Soient $X_1, X_2$ et $Z$ trois variétés et $f$ un morphisme de $X_1 \times X_2$ dans $Z$. Soit $a \in X_1$ et $b \in X_2$. L’application linéaire tangente à l’application partielle $x \mapsto f(x, b)$ (resp. $y \mapsto f(a, y)$) de $X_1$ (resp. $X_2$) dans $Z$ se note $T^1_{(a, b)}(f)$ (resp. $T^2_{(a, b)}(f)$). Si l’on identifie $T_{(a, b)}(X_1 \times X_2)$ à $T_a(X_1) \times T_b(X_2)$, on a:

$$
T_{(a, b)}(f) \cdot (u, v) = T^1_{(a, b)}(f) \cdot u + T^2_{(a, b)}(f) \cdot v
$$

pour tout $u \in T_a(X_1)$ et tout $v \in T_b(X_2)$.

5.6.7. (« Théorème des fonctions implicites »). Les hypothèses et notations étant celles du numéro précédent, supposons de plus que $T^2_{(a, b)}(f)$ soit bijectif. Il existe alors un voisinage ouvert $U$ de $a$ dans $X_1$ et un voisinage ouvert $V$ de $b$ dans $X_2$ possédant la propriété suivante: pour tout $x \in U$, il existe un point $g(x)$ de $V$ et un seul tel que $f(x, g(x)) = f(a, b)$, et l’application $g$ est un morphisme de $U$ dans $V$. Pour tout $x \in U$, on a:

$$
T_x(g) = - (T^2_{(x, g(x))}(f))^{-1} \circ T^1_{(x, g(x))}(f).
$$

### 5.7. Immersions, morphismes étales

5.7.1. Soient $X$ et $Y$ deux variétés, $f$ un morphisme de $X$ dans $Y$ et $a$ un point de $X$. Posons $b = f(a)$. Les conditions suivantes sont équivalentes:
(i) L’application linéaire $T_a(f)$ est injective et son image est un sousespace vectoriel fermé de $T_b(Y)$ admettant un supplémentaire topologique $^1$;

(ii) Il existe un espace de Banach $F$, un sous-espace vectoriel fermé $E$ de $F$ admettant un supplémentaire topologique, et des cartes $(U, \varphi, E)$ de $X$ en $a$ et $(V, \psi, F)$ de $Y$ en $b$ telles que $f(U) \subset V$ et $\varphi = \psi \circ (f|U)$.

(iii) Il existe un voisinage ouvert $U$ de $a$, un voisinage ouvert $V$ de $b$ contenant $f(U)$, une variété $Z$, un point $c$ de $Z$, et un isomorphisme de variétés $g$ de $U \times Z$ sur $V$ tels que $f(x) = g(x, c)$ pour tout $x \in U$.

(iv) Il existe un voisinage ouvert $U$ de $a$, un voisinage ouvert $V$ de $b$ et un morphisme $q$ de $V$ dans $X$ avec $f(U) \subset V$, et $q(f(x)) = x$ pour tout $x \in U$.

Lorsque $X$ et $Y$ sont de dimension finie, les conditions précédentes sont encore équivalentes à la suivante:

(v) Il existe un voisinage ouvert $U$ de $a$, un système de coordonnées $(\eta^1, \ldots, \eta^n)$ de $Y$ dans un voisinage ouvert $V$ de $b$ contenant $f(U)$ et un entier $m \leq n$ tels que $\eta^j \circ f = 0$ pour $m < j \leq n$ et que les fonctions $\eta^1 \circ f, \ldots, \eta^m \circ f$ forment un système de coordonnées de $X$ dans $U$.

Si les propriétés (i) à (iv) sont satisfaites, on dit que $f$ est une immersion en $a$.

L’ensemble des points où $f$ est une immersion est ouvert dans $X$; si cet ouvert est $X$ tout entier, on dit que $f$ est une immersion.

Pour que $f$ soit une immersion, il faut et il suffit que l’on puisse recouvrir $X$ par des ouverts $U_i$ tels que, pour tout $i, f|U_i$ soit un isomorphisme de $U_i$ sur une sous-variété de $Y$ (cf. n° 5.8.3).

5.7.2. Exemples:
(a) Si $X$ est un ouvert d’une variété $Y$, l’injection canonique de $X$ dans $Y$ est une immersion.
(b) Soient $E$ et $F$ deux espaces de Banach et $u$ une application linéaire continue de $E$ dans $F$. Alors $u$ est une immersion si et seulement si $u$ est un isomorphisme de $E$ sur un sous-espace vectoriel fermé de $F$ admettant un supplémentaire topologique.

5.7.3. Soient $f : X \to Y$ et $g : Y \to Z$ deux morphismes. Si $f$ et $g$ sont des immersions, $g \circ f$ est une immersion. Réciproquement, si $g \circ f$ est une immersion, alors $f$ est une immersion. Si $f : X \to Y$ et $f' : X' \to Y'$ sont des immersions, $f \times f'$ est une immersion.

5.7.4 Supposons que $X$ et $Y$ soient des variétés de dimension finie sur un corps $K$ de caractéristique 0. Si $f : X \to Y$ est un morphisme injectif, l’ensemble des points de $X$ où $f$ est une immersion est un ouvert dense

$^1$ Tout sous-espace vectoriel fermé de codimension finie d’un espace de Banach admet un supplémentaire topologique; si $K = \mathbf{R}$ ou $\mathbf{C}$, il en est de même de tout sous-espace vectoriel (nécessairement fermé) de dimension finie.

dans X. Si K = R ou C, ce résultat reste vrai si l’ou suppose seulement que X est de dimension finie.

5.7.5. Soit $f : X \to Y$ une immersion et soit $g$ une application continue d’une variété Z dans X. Pour que $g$ soit un morphisme, il faut et il suffit que $f \circ g$ soit un morphisme.

5.7.6. Soit $f : X \to Y$ un morphisme, et soit $a$ dans X. Les deux propriétés suivantes sont équivalentes:
(i) $T_a(f)$ est bijectif.
(ii) Il existe un voisinage ouvert U de $a$ et un voisinage ouvert V de $f(a)$ tels que $f$ induise un isomorphisme de U sur V.
Lorsque ces propriétés sont vérifiées, on dit que $f$ est un isomorphisme local en $a$, ou que $f$ est étale en $a$. Si cela a lieu pour tout $a \in X$, on dit que $f$ est étale, ou est un étalement, ou que X est étalé dans Y (au moyen de $f$). Pour qu’un morphisme soit étale, il faut et il suffit que ce soit à la fois une immersion (n° 5.7.1) et une submersion (n° 5.9.1.).

5.7.7. Soit $f : X \to Y$ une immersion ; supposons la variété X pure de dimension finie. Alors $f$ est étale dans chacun des deux cas suivants:
(i) $\dim Y = \dim X$;
(ii) $f$ est surjective et la topologie de X admet une base dénombrable d’ouverts.

5.7.8. Pour qu’un morphisme $f$ soit un isomorphisme sur une sous-variété ouverte (resp. un isomorphisme), il faut et il suffit que $f$ soit étale et injectif (resp. étale et bijectif).

### 5.8. Images inverses de structures de variété, sous-variétés

5.8.1. Soient X un espace topologique, Y une variété et $f$ une application de X dans Y. Considérons les conditions suivantes:
(QR) (resp. (R)) Pour tout $a \in X$, il existe un voisinage ouvert U de a dans X et une carte $(V, \varphi, E)$ de la variété Y en $f(a)$ tels que $f(U) \subset V$ et que $\varphi \circ f$ induise un homéomorphisme de U sur l’intersection de $\varphi(V)$ avec un sous-espace vectoriel fermé (resp. fermé et admettant un supplémentaire topologique) F de E.
Si la condition (QR) est réalisée, il existe sur X une structure de variété et une seule pour laquelle les triplets $(U, \varphi \circ f, F)$ (avec les notations de (QR)) sont des cartes de X. On l’appelle la structure image inverse de la structure de variété de Y par $f$. Sa topologie est celle de X.
Pour qu’il existe sur X une structure de variété compatible avec la topologie donnée et pour laquelle $f$ soit une immersion, il faut et il suffit que la condition (R) soit satisfaite. Cette structure est alors unique : c’est l’image inverse par $f$ de la structure de variété de $Y$.

5.8.2. La condition (R) ci-dessus est notamment satisfaite lorsque pour tout $a \in X$ il existe un voisinage ouvert $U$ de $a$ tel que $f|U$ soit un homéomorphisme de $U$ sur un ouvert de $Y$. Dans ce cas, la variété $X$ obtenue est étalée sur $Y$ (5.7.6).

5.8.3. Supposons maintenant que $X$ soit un sous-espace topologique de $Y$, $f$ étant l’injection canonique. Si $f$ satisfait à la condition (R) (resp. (QR)) du n° 5.8.1, on dit que $X$, muni de la structure image inverse de la structure de variété de $Y$ par $f$, est une sous-variété (resp. quasi-sous-variété) de $Y$. Une sous-variété est une quasi-sous-variété.

Toute quasi-sous-variété est localement fermée ; tout ouvert est une sous-variété et sa structure est celle définie au n° 5.2.3.

Lorsque $Y$ est localement de dimension finie, un sous-espace topologique $X$ de $Y$ est une sous-variété de $Y$ si et seulement si, pour tout $a \in X$, il existe un voisinage ouvert $U$ de $a$ dans $Y$, un système de coordonnées $(\xi^1, \ldots, \xi^m)$ de $Y$ dans $U$, et un entier $k \leq m$ tels que $U \cap X$ soit l’ensemble des points de $U$ où s’annulent simultanément les fonctions $\xi^i$ pour $1 \leq i \leq k$.

Soit $f : X \to Y$ un morphisme de variétés. Supposons que $f$ soit une immersion, et que $f$ induise un homéomorphisme de $X$ sur $f(X)$. Alors $f(X)$ est une sous-variété de $Y$, et $f$ induit un isomorphisme de $X$ sur $f(X)$; on dit alors que $f$ est un plongement de $X$ dans $Y$.

5.8.4. Soient $Y$ et $W$ deux variétés, soit $X$ une sous-variété de $Y$ et soit $f$ une application de $X$ dans $W$. Pour que $f$ soit un morphisme, il faut et il suffit que, pour tout $a \in X$, il existe un voisinage $U$ de $a$ dans $Y$ et un morphisme $g : U \to W$ tels que $g$ coïncide avec $f$ sur $U \cap X$.

5.8.5. Soit $X$ une quasi-sous-variété d’une variété $Y$, et soit $g$ une application d’une variété $Z$ dans $X$. Supposons que $K$ soit de caractéristique 0, ou que $X$ soit une sous-variété de $Y$. Pour que $g$ soit un morphisme de $Z$ dans $X$, il faut et il suffit que ce soit un morphisme de $Z$ dans $Y$ : autrement dit, la structure de variété de $X$ est induite par celle de $Y$ (Ens., ch. IV, § 2, n° 4).

5.8.6. Si $X$ est une sous-variété (resp. quasi-sous-variété) de $Y$ et si $Y$ est une sous-variété d’une variété $Z$, alors $X$ est une sous-variété (resp. quasi-sous-variété) de $Z$.

5.8.7. Soit $X_i$ (pour $i = 1, 2$) une variété et soit $Y_i$ une sous-variété (resp. quasi-sous-variété) de $X_i$ (pour $i = 1, 2$). Alors $Y_1 \times Y_2$ est une sous-variété (resp. quasi-sous-variété) de $X_1 \times X_2$.

5.8.8. Soit X une quasi-sous-variété d'une variété Y ; soit x un point de X et notons f l'injection canonique de X dans Y. L'application T_x(f) : T_x(X) → T_x(Y) est injective et elle permet d'identifier l'espace T_x(X) à un sous-espace vectoriel fermé de T_x(Y). L'espace vectoriel topologique quotient T_x(Y)/T_x(X) est un espace de Banach, qu'on appelle espace transversal en x à X (dans Y). Sa dimension (finie ou +∞) s'appelle la codimension de X dans Y au point x.

Si de plus X est une sous-variété de Y, alors l'espace T_x(X) admet un supplémentaire topologique dans T_x(Y).

5.8.9. Soit f une application d'une variété X dans une variété Y, et soit Γ son graphe. Pour que f soit un morphisme, il faut et il suffit que les deux conditions suivantes soient satisfaites :
(i) Γ est une sous-variété de X × Y.
(ii) Pour tout (x, y) ∈ Γ, on a
$$
T_{(x,y)}(X \times Y) = T_{(x,y)}(\Gamma) \oplus T_y(Y).
$$
S'il en est ainsi, l'application $\mathrm{pr}_1$ induit un isomorphisme de $\Gamma$ sur X, et $T_{(x,y)}(\Gamma)$ s'identifie au graphe de $T_x(f)$.

En particulier, la diagonale de X × X est une sous-variété de X × X.

5.8.10. Soit Y une variété, et soit (f_i)_{i∈I} une famille finie de fonctions morphiques sur Y. Soit X l'ensemble des x ∈ Y tels que f_i(x) = 0 pour tout i. Faisons l'hypothèse suivante :
(J) Pour tout x ∈ X, les différentielles d_x f_i sont linéairement indépendantes dans T'_x(Y).

Alors X est une sous-variété fermée de Y, l'espace tangent T'_x(X) est le sous-espace de T_x(Y) formé des α tels que α . f_i = 0 pour tout i dans I. De plus, la codimension de X dans Y est égale à Card (I) en chacun de ses points.

5.8.11. (Points simples d'un idéal). Soit a un idéal de l'algèbre de polynômes K[X_1, ..., X_n]. Un point x = (x_1, ..., x_n) de K^n est appelé un zéro de a si f(x) = 0 pour tout f ∈ a. Si x ∈ K^n, notons S_x la sous-algèbre de K(X_1, ..., X_n) formée des fractions f/g, avec f, g ∈ K[X_1, ..., X_n], et g(x) ≠ 0; notons a_x l'idéal de S_x engendré par a dans S_x. Un point x est appelé un zéro simple de a si c'est un zéro de a et si la condition suivante est satisfaite :
(S) Il existe une suite finie (f_1, ..., f_m) d'éléments de a qui engendrent l'idéal a_x et dont les différentielles en x sont linéairement indépendantes. (Cette condition équivaut à dire que l'anneau local S_x/a_x est régulier (Alg. Comm., à paraître).)
Soit Z (resp. Z_s) l'ensemble des zéros (resp. des zéros simples) de a. L'ensemble Z est fermé dans K^n, Z_s est ouvert dans Z, et Z_s est une sous-variété de $K^n$. Si $x \in Z_s$, l’idéal $K[X_1, \ldots, X_n] \cap a_x$ se compose des polynômes $f$ nuls sur un voisinage de $x$ dans $Z_s$.

Soit $\bar{a}$ l’idéal des polynômes nuls sur $Z$. Si $K$ est algébriquement clos, l’ensemble des zéros simples de $a$ est dense dans $Z$.

5.8.12. Soient $X$ une variété et $L$ l’ensemble des couples $(x, Z)$ où $x$ est un point de $X$ et $Z$ une sous-variété de $X$ contenant $x$. Etant donnés deux couples $\pi = (x, Z)$ et $\pi' = (x', Z')$, nous noterons $R\{\pi, \pi'\}$ la relation :

« On a $x = x'$ et il existe un voisinage $U$ de $x$ tel que $U \cap Z = U \cap Z'$ ». Alors $R$ est une relation d’équivalence dans $L$; on note $\gamma_x(Z)$ la classe d’équivalence du couple $(x, Z) \in L$. Sur l’ensemble $J = L/R$, il existe une structure de variété et une seule qui vérifie la condition suivante :
Pour toute sous-variété $Z$ de $X$, l’application $x \mapsto \gamma_x(Z)$ de $Z$ dans $J$ est un isomorphisme de $Z$ sur une sous-variété ouverte de $J$.
On dit que $J$ est la variété des germes de sous-variétés de $X$ (cf. Top. Gén., chap. I, 4e éd., § 6, n° 10).
L’application $\rho : J \to X$ définie par $\rho(\gamma_x(Z)) = x$ est une immersion ; on l’appelle l’immersion canonique de $J$ dans $X$.
Si $X$ est une variété analytique séparée de dimension finie, il en est de même de $J$.

### 5.9. Submersions et variétés quotients

5.9.1. Soient $f : X \to Y$ un morphisme de variétés, $a$ un point de $X$ et posons $b = f(a)$. Les conditions suivantes sont équivalentes :
(i) L’application linéaire $T_a(f)$ est surjective, et son noyau admet un supplémentaire topologique dans $T_a(X)$.
(ii) Il existe une carte $(U, \varphi, E)$ de $X$ en $a$, une carte $(V, \psi, F)$ de $Y$ en $b$ et une application linéaire continue surjective $u$ de $E$ dans $F$ telles que
$$
f(U) \subset V, \quad \psi \circ f = u \circ \varphi
$$
et que le noyau de $u$ admette un supplémentaire topologique dans $E$.
(iii) Il existe un voisinage ouvert $U$ de $a$, un voisinage ouvert $V$ de $b$ contenant $f(U)$, et un morphisme $g$ de $U$ dans une variété $Z$ tels que l’application $(f, g)$ de $U$ dans $V \times Z$ soit un isomorphisme.
(iv) Il existe un voisinage ouvert $V$ de $b$ et un morphisme $s$ de $V$ dans $X$ tels que $s(b) = a$ et $f(s(y)) = y$ pour tout $y$ dans $V$ (« section locale »).
Lorsque $X$ et $Y$ sont de dimension finie, les conditions précédentes sont équivalentes à la condition suivante :
(v) Il existe un voisinage ouvert $U$ de $a$, un voisinage ouvert $V$ de $b$ contenant $f(U)$, et un système de coordonnées $(\eta^1, \ldots, \eta^n)$ sur $V$ tels que les fonctions $\eta^i \circ f$ sur $U$ fassent partie d’un système de coordonnées sur $U$.
Si les propriétés (i) à (iv) sont satisfaites, on dit que $f$ est une submersion en $a$. L’ensemble des points où $f$ est une submersion est ouvert dans $X$; si cet ouvert est $X$ tout entier, on dit que $f$ est une submersion.

5.9.2. Soient $f : X \to Y$ et $g : Y \to Z$ deux morphismes. Si $f$ et $g$ sont des submersions, il en est de même de $g \circ f$; réciproquement, si $g \circ f$ est une submersion et si $f$ est surjective, alors $g$ est une submersion.

5.9.3. Si $f : X \to Y$ et $f' : X' \to Y'$ sont des submersions, $f \times f'$ est une submersion.

5.9.4. Une submersion $f : X \to Y$ est une application ouverte (cf. Top. gén., chap. I, 4e éd., § 5, n° 1); en particulier, la relation d'équivalence R définie par $f$ est ouverte, $f$ définit par passage au quotient un homéomorphisme de $X/R$ sur $f(X)$, et $f(X)$ est ouvert dans $Y$.

5.9.5. Soit $R$ une relation d'équivalence sur une variété $X$. On dit que $R$ est régulière s'il existe sur l'espace quotient $X/R$ une structure de variété telle que la projection canonique $p : X \to X/R$ soit une submersion; cette structure de variété est alors unique; elle est quotient de celle de $X$ (Ens., ch. IV, § 2, n° 6): autrement dit, pour qu'une application $g$ de $X/R$ dans une variété $Y$ soit un morphisme, il faut et il suffit que $g \circ p$ soit un morphisme de $X$ dans $Y$.

Soit $C \subset X \times X$ le graphe de $R$. Pour que $R$ soit régulière, il faut et il suffit que les deux conditions suivantes soient satisfaites:
(i) $C$ est une sous-variété de $X \times X$.
(ii) L'application $\mathrm{pr}_1$ de $C$ dans $X$ est une submersion.

La condition (ii) signifie aussi que si $a$ et $b$ sont congrus modulo $R$, il existe un voisinage ouvert $U$ de $a$ et un morphisme $s$ de $U$ dans $X$ tel que $s(a) = b$ et que $s(x)$ soit congru à $x$ modulo $R$ pour tout $x \in U$.

Supposons $R$ régulière. Pour que la variété quotient $X/R$ soit séparée, il faut et il suffit que le graphe de $R$ soit fermé dans $X \times X$.

5.9.6. Soient $X$ et $X'$ deux variétés, $R$ et $R'$ des relations d'équivalence régulières sur $X$ et $X'$, et soit $f : X \to X'$ un morphisme compatible avec les relations $R$ et $R'$. L'application $\tilde{f} : X/R \to X'/R'$ déduite de $f$ par passage aux quotients est alors un morphisme.

5.9.7. (« Transitivité des quotients ») Soient $R$ et $S$ deux relations d'équivalence sur une variété $X$ telles que $R$ entraîne $S$, et soit $S/R$ la relation d'équivalence quotient sur $X/R$. Supposons que $R$ soit régulière. Alors, pour que $S$ soit régulière, il faut et il suffit que $S/R$ le soit; s'il en est ainsi, la bijection canonique

$$
(X/R)/(S/R) \to X/S
$$

est un isomorphisme de variétés.

5.9.8. (« Produits de quotients ») Soit $(X_i)_{i \in I}$ une famille finie de variétés, munies chacune d'une relation d'équivalence régulière $R_i$. Soit $X = \prod_{i \in I} X_i$, et soit $R$ la relation d'équivalence sur $X$ produit des $R_i$ (cf. Top. Gén., chap. I, 4e éd., § 5, n° 3, cor. de la prop. 8). Alors $R$ est régulière, et la bijection canonique de $X/R$ sur $\prod_{i \in I} (X_i/R_i)$ est un isomorphisme de variétés.

### 5.10. Subimmersions

5.10.1. Soit $f : X \to Y$ un morphisme de variétés et soit $\Gamma$ le graphe de $f$. L'application $j : x \mapsto (x, f(x))$ est une immersion de $X$ dans $X \times Y$, dont l'image est la sous-variété $\Gamma$, et $f = \mathrm{pr}_2 \circ j$ est composé de l'immersion $j$ suivie de la submersion $\mathrm{pr}_2$.

Soit $a \in X$. On dit que $f$ est une submersion en $a$ s'il existe un voisinage ouvert $U$ de $a$, une variété $Z$, une submersion $s$ de $U$ dans $Z$ et une immersion $i$ de $Z$ dans $Y$ tels que $f|U = i \circ s$. L'ensemble des points de $X$ où $f$ est une submersion est un ouvert de $X$; si cet ouvert est $X$ tout entier, on dit que $f$ est une submersion.

5.10.2. Les immersions et les submersions sont des submersions. Si $f : X \to Y$ est une submersion, $g : Y \to Z$ une immersion et $h : W \to X$ une submersion, alors $g \circ f \circ h$ est une submersion.

Si $f$ et $f'$ sont des submersions, $f \times f'$ est une submersion.

5.10.3. Pour que $f : X \to Y$ soit une submersion en un point $a$ de $X$, il faut et il suffit qu'il existe une carte $(U, \varphi, E)$ de $X$ en $a$, une carte $(V, \psi, F)$ de $Y$ au point $f(a)$ et une application linéaire continue $g$ de $E$ dans $F$ tels que:
(i) $f(U) \subset V,\ g(\varphi(U)) \subset \psi(V)$ et $f|U = \psi^{-1} \circ g \circ \varphi$;
(ii) le noyau (resp. l'image) de $g$ est un sous-espace fermé de $E$ (resp. $F$) admettant un supplémentaire topologique.

5.10.4. Soient $X$ et $Y$ deux variétés de dimension finie. Pour qu'un morphisme $f$ de $X$ dans $Y$ soit une submersion en un point $a$ de $X$, il faut et il suffit qu'il existe un système de coordonnées $(\xi^1, \ldots, \xi^m)$ de $X$ en $a$, un système de coordonnées $(\eta^1, \ldots, \eta^n)$ de $Y$ en $f(a)$ et un entier $k \leq \inf(m, n)$ tels que
$$
\eta^i \circ f = \xi^i \quad \text{pour } 1 \leq i \leq k \\
\eta^i \circ f = 0 \quad \text{pour } k < i \leq n.
$$

5.10.5. Soit $f : X \to Y$ une submersion. Pour tout $b \in Y$, $f^{-1}(b)$ est une sous-variété de $X$; le sous-espace de $T_a(X)$ tangent à la sous-variété $f^{-1}(b)$ au point $a \in f^{-1}(b)$ est le noyau de $T_a(f)$.

5.10.6. (« Théorème du rang constant ») Soit $f : X \to Y$ un morphisme de variétés et soit $a \in X$. Si $f$ est une subimmersion en $a$, on a $\mathrm{rg}_x f = \mathrm{rg}_a f$ pour $x$ voisin de $a$.

Réciproquement, supposons le corps $K$ de caractéristique zéro. Soient $(U, \varphi, E)$ une carte de $X$ en $a$ et soit $(V, \psi, F)$ une carte de $Y$ en $f(a)$, avec $f(U) \subset V$. Posons $g = \psi \circ f \circ \varphi^{-1}$. S’il existe un sous-espace vectoriel fermé $E_1$ de $E$ et un sous-espace vectoriel fermé $F_1$ de $F$ tels que pour tout $x \in U$, le sous-espace $E_1$ (resp. $F_1$) soit un supplémentaire topologique du noyau (resp. de l’image) de la dérivée $Dg(\varphi(x))$ de $g$ au point $\varphi(x)$, alors $f$ est une subimmersion en $a$.

Si $K$ est de caractéristique zéro (resp. $K = \mathbf{R}$ ou $\mathbf{C}$) et si $Y$ est de dimension finie (resp. $\mathrm{rg}_a f < +\infty$), alors $f$ est une subimmersion en $a$ si et seulement si $\mathrm{rg}_x f = \mathrm{rg}_a f$ pour tout $x$ assez voisin de $a$.

Si $K$ est de caractéristique zéro (resp. $K = \mathbf{R}$ ou $\mathbf{C}$) et $Y$ (resp. $X$) de dimension finie, l’ensemble des points $x \in X$ où $f$ est une subimmersion est un ouvert dense dans $X$.

5.10.7. (« Factorisation canonique d’une subimmersion ») Toute subimmersion est composée d’une submersion et d’une immersion. De façon précise, soit $f : X \to Y$ une subimmersion, et soit $J$ la variété des germes de sous-variétés de $Y$ (5.8.12). Soient $x$ dans $X$ et $y = f(x)$; il existe des voisinages ouverts $U$ de $x$ tels que $f|U$ soit une submersion de $U$ sur une sous-variété $Z$ de $Y$; l’élément $\gamma_y(Z)$ de $J$ ne dépend que de $x$ mais non du voisinage $U$ choisi, et, si on le note $\lambda(x)$, l’application $\lambda$ est une submersion de $X$ dans $J$; si l’on note $\rho$ l’immersion canonique de $J$ dans $Y$, on a $f = \rho \circ \lambda$. Si $f$ est une immersion, le morphisme $\lambda$ de $X$ dans $J$ est étale.

Si $g$ est une submersion surjective de $X$ dans une variété $Z$ et $h$ un morphisme de $Z$ dans $Y$ tels que $f = h \circ g$, il existe une submersion $\mu$ et une seule de $Z$ dans $J$ telle que $\lambda = \mu \circ g$.

### 5.11. Produits fibrés et images réciproques

5.11.1. Soient $F$ un espace de Banach, $(E_i)_{i \in I}$ une famille finie d’espaces de Banach et $f = (f_i)_{i \in I}$ une famille d’applications linéaires continues $f_i$ de $E_i$ dans $F$. Soient $E$ le produit des $E_i$ et $f$ l’application linéaire continue de $E$ dans $F^I$ produit des $f_i$. Soit enfin $D$ le sous-espace fermé de $F^I$ formé des $(y_i)_{i \in I}$ tels que $y_i$ soit indépendant de $i$ (« diagonale » de $F^I$). On dit que la famille $f$ est transversale si l’application linéaire continue composée de $f$ et de la projection canonique de $F^I$ sur le quotient $F^I/D$ est surjective et si son noyau $f^{-1}(D)$ admet un supplémentaire topologique.

Si les espaces $E_i$ et $F$ sont tous de dimension finie, la famille $f$ est transversale si et seulement si l’on a:

$$
\operatorname{codim} \left( \bigcap_i \operatorname{Im} f_i \right) = \sum_i \operatorname{codim} (\operatorname{Im} f_i)
$$

Si $I = \{1, 2\}$, le couple $(f_1, f_2)$ est transversal si et seulement si l’application

$$
f_1 + f_2 : E_1 \oplus E_2 \to F
$$

est surjective et si son noyau admet un supplémentaire topologique (si $E_1$ et $E_2$ sont de dimension finie, il revient au même de dire que

$$
\operatorname{Im} f_1 + \operatorname{Im} f_2 = F).
$$

5.11.2. Soient $S$ une variété, $(X_i)_{i \in I}$ une famille finie de variétés et $f = (f_i)_{i \in I}$ une famille de morphismes $f_i$ de $X_i$ dans $S$. Soit $P$ le sous-ensemble du produit $X$ des $X_i$ formé des points $(x_i)_{i \in I}$ tels que $f_i(x_i)$ soit indépendant de $i$. Soit $x \in P$ et soit $y = f_i(x_i) \in F$. On dit que la famille $f$ est *transversale* au point $x$ de $P$ si les applications $T_x(f_i)$ forment une famille transversale d’applications linéaires continues à valeurs dans l’espace de Banach $T_y(S)$. On dit que $f$ est *transversale* si elle est transversale en tout point de $P$.

Si $f$ est transversale, alors $P$ est une *sous-variété* de $X$, que l’on appelle *produit fibré de la famille des $X_i$ au dessus de $S$* (relativement à la famille $f$) et que l’on note $\prod_{i \in I} X_i$ (ou plus simplement $X_1 \times_S X_2$ lorsque $I = \{1, 2\}$ par exemple). Pour tout point $x = (x_i)$ de $P$, l’espace tangent $T_x(\prod_{i \in I} X_i)$ est le sous-espace de $\prod T_{x_i}(X_i)$ formé des vecteurs tangents $t = (t_i)$ tels que $T_{x_i}(f_i) \cdot t_i$ soit indépendant de l’indice $i$.

Si $f_1 : X_1 \to Y$ est une *submersion* et $f_2 : X_2 \to Y$ un morphisme, le couple $(f_1, f_2)$ est transversal.

5.11.3. (*Propriété universelle des produits fibrés*) Soit $f = (f_i)_{i \in I}$ une famille transversale de morphismes $f_i : X_i \to S$ et soit $P$ le produit fibré des $X_i$ au-dessus de $S$; pour tout $i \in I$, on note $\pi_i$ le morphisme de $P$ dans $X_i$ obtenu par restriction à $P$ de la projection de $X$ sur $X_i$; alors $f_i \circ \pi_i$ est un morphisme de $P$ dans $S$ indépendant de $i$. Soient $T$ une variété, et $g_i : T \to X_i$ des morphismes de variétés tels que $f_i \circ g_i$ soit un morphisme de $T$ dans $S$ indépendant de $i \in I$; il existe alors un morphisme $h$ de $T$ dans $P$ et un seul tel que $g_i = \pi_i \circ h$ pour tout $i \in I$.

5.11.4. (*Associativité du produit fibré*) Soit $f = (f_i)_{i \in I}$ une famille finie de morphismes de variétés $f_i : X_i \to S$, et soit $(J_\lambda)_{\lambda \in \Lambda}$ une partition de $I$. On suppose que, pour tout $\lambda$ dans $\Lambda$, la famille $f_\lambda = (f_i)_{i \in J_\lambda}$ est transversale, et l’on note $P_\lambda$ le produit fibré de cette famille; pour tout point $x = (x_i)_{i \in J_\lambda}$ de $P_\lambda$, l’élément $f_i(x_i)$ de $S$ est indépendant de $i \in J_\lambda$ et sera noté $u_\lambda(x)$;

alors $u_\lambda$ est un morphisme de $P_\lambda$ dans $S$. Pour que la famille $u = (u_\lambda)$ soit transversale, il faut et il suffit que la famille $f$ le soit. La bijection canonique de $\prod_{\lambda \in \Lambda} \prod_{i \in J_\lambda} X_i$ sur $\prod_{i \in I} X_i$ donne alors par restriction un isomorphisme du produit fibré $\prod_{\lambda \in \Lambda} \prod_{s} P_\lambda$ sur le produit fibré $\prod_{i \in I} \prod_{s} X_i$.

5.11.5. Soit $S$ une variété. On appelle *variété au dessus de* $S$ une variété $X$ munie d’un morphisme $\lambda : X \to S$. Soient $(X, \lambda)$ une variété au dessus de $S$ et $f : S' \to S$ un morphisme de variétés tel que le couple $(f, \lambda)$ soit transversal. On notera alors $f^*(X)$ la variété $S' \times_S X$, munie du morphisme $f^*(\lambda) : S' \times_S X$ défini par $f^*(\lambda)(s', x) = s'$. On dit que $f^*(X)$ se déduit de $X$ par changement de base de $S$ à $S'$ suivant $f$. Si $\lambda$ est une submersion (resp. une immersion, une subimmersion, un morphisme étale), il en est de même de $f^*(\lambda)$.

5.11.6. Soit $f : X \to Y$ un morphisme de variétés et soit $W$ une sous-variété de $Y$; soit $i$ l’injection canonique de $W$ dans $Y$. On dit que $f$ est *transversal à* $W$ *en un point* $x \in f^{-1}(W)$ si le couple $(f, i)$ est transversal au point $(x, f(x))$ de $X \times W$. Pour cela, il faut et il suffit que les conditions suivantes soient satisfaites :
(i) l’espace tangent $T_{f(x)}(Y)$ est somme de $T_{f(x)}(W)$ et de l’image de $T_x(f)$;
(ii) l’image réciproque $T_x(f)^{-1}(T_{f(x)}(W))$ de l’espace tangent à $W$ en $f(x)$ admet un supplémentaire topologique.
On dit que $f$ est *tranversal à* $W$ s’il est transversal à $W$ en tout point de $f^{-1}(W)$.
Pour qu’un morphisme $f$ de $X$ dans $Y$ soit une submersion, il suffit qu’il soit transversal à tout point de $Y$ et il faut qu’il soit transversal à toute sous-variété de $Y$. Pour qu’une famille finie de morphismes $f_i : X_i \to S$ soit transversale, il faut et suffit que le morphisme $g$ de $\prod_{i \in I} X_i$ dans $S^I$ défini par $g((x_i)_{i \in I}) = (f_i(x_i))_{i \in I}$ soit transversal à la diagonale de $S^I$.

5.11.7. Supposons que le morphisme $f : X \to Y$ soit transversal à la sous-variété $W$ de $Y$. Alors $f^{-1}(W)$ est une sous-variété de $X$, et pour $x$ dans $f^{-1}(W)$ le sous-espace de $T_x(X)$ tangent à $f^{-1}(W)$ est l’image réciproque par $T_x(f)$ du sous-espace $T_{f(x)}(W)$. Par passage au quotient, l’application linéaire $T_x(f)$ définit un isomorphisme d’espaces vectoriels topologiques de l’espace transversal à $f^{-1}(W)$ en $x$ sur l’espace transversal à $W$ en $y = f(x)$. Si $W$ est de codimension $d$ en $y$ dans $Y$, la sous-variété $f^{-1}(W)$ de $X$ est de codimension $d$ en tout point de $f^{-1}(W)$. Enfin, l’application $x \mapsto (x, f(x))$ est un isomorphisme de variétés de $f^{-1}(W)$ sur le produit fibré $X \times_Y W$.

5.11.8. Soient $Y_1$ et $Y_2$ deux sous-variétés d'une variété $X$, et soit $\iota_j$ l'injection de $Y_j$ dans $X$. On dit que $Y_1$ et $Y_2$ sont transversales si le couple $(\iota_1, \iota_2)$ est transversal ; il revient au même de supposer que, pour tout point $x$ de $Y_1 \cap Y_2$, les sous-espaces $T_x(Y_1)$ et $T_x(Y_2)$ de $T_x(X)$ ont $T_x(X)$ pour somme, et que leur intersection admet un supplémentaire topologique dans $T_x(X)$. Sous ces conditions, $Y_1 \cap Y_2$ est une sous-variété de $X$ et pour tout $x$ dans $Y_1 \cap Y_2$, on a :

$$
T_x(Y_1 \cap Y_2) = T_x(Y_1) \cap T_x(Y_2);
$$

si de plus $Y_i$ est de codimension $d_i$ en $x$, alors $Y_1 \cap Y_2$ est de codimension $d_1 + d_2$ en $x$.

5.11.9. Soient $f$ et $g$ deux morphismes d'une variété $X$ dans une variété $Y$. Si le morphisme $(f, g) : X \to Y \times Y$ est transversal à la diagonale de $Y \times Y$, le sous-ensemble $N$ de $X$ formé des points $x$ tels que $f(x) = g(x)$ est une sous-variété de $X$; on l'appelle le *noyau* de la double flèche

$$
f, g : X \twoheadrightarrow Y.
$$

### 5.12. Variétés de groupes

5.12.1. Soit $G$ un groupe. Une structure de variété sur $G$ est dite *compatible* avec la structure de groupe de $G$ si l'application $(x, y) \mapsto xy$ de $G \times G$ dans $G$ est un morphisme. L'application $x \mapsto x^{-1}$ est alors un morphisme de $G$ dans lui-même. L'ensemble $G$, muni de sa structure de groupe et de sa structure de variété, est appelé une *variété de groupe* (« de classe $C^r$ » si l'on veut préciser), ou encore un *groupe de Lie*. Si $r = \omega$, on dit aussi *groupe analytique*. Si $K = \mathbf{R}$ (resp. $\mathbf{C}, \mathbf{Q}_p$), on dit encore *groupe de Lie réel* (resp. *complexe*, *p-adique*). Toute variété de groupe est pure. On appelle *homomorphisme de variétés de groupe* (ou simplement *homomorphisme*) toute application d'une variété de groupe dans une autre qui est à la fois un homomorphisme de groupes et un *morphisme* de variétés.

Si $G$ est une variété de groupe, la structure topologique sous-jacente à la structure de variété de $G$ en fait un *groupe topologique métrisable et complet* ; il est localement compact si $K$ est localement compact et $G$ de dimension finie.

5.12.2. *Exemples* :
(i) Si $V$ est un espace de Banach, la structure canonique de variété de $V$ est compatible avec sa structure de groupe commutatif.
(ii) Soit $A$ une $K$-algèbre normée complète, possédant un élément unité, et soit $A^*$ le groupe des éléments inversibles de $A$. C'est un sous-espace ouvert de $A$ et la structure de variété induite sur cet ouvert par la structure canonique de variété du $K$-espace vectoriel $A$ est compatible avec la structure de groupe dans $A^*$. En particulier, prenons pour $A$ l'algèbre

L(E) des endomorphismes continus d’un espace de Banach E ; le groupe $A^*$ se compose des automorphismes de l’espace vectoriel topologique E ; on note $\mathrm{GL}(E)$ la variété de groupe ainsi définie. Lorsque $A = M_n(K)$, on obtient une structure de variété de groupe sur $\mathrm{GL}(n, K)$.

(iii) Si $G_1, \ldots, G_n$ sont des variétés de groupes, le groupe produit $G = G_1 \times \cdots \times G_n$ est une variété de groupe, lorsqu’on le munit de la structure de variété produit de celles des $G_i$.

5.12.3. Soit $G$ une variété de groupe, soit $H$ un groupe topologique et soit $f : H \to G$ un homomorphisme continu vérifiant la condition (QR) du n° 5.8.1. La structure de variété *image inverse* de celle de $G$ par $f$ fait alors de $H$ une variété de groupe. Ceci s’applique notamment lorsque $H$ est un *sous-groupe de $G$ qui est une sous-variété* (resp. quasi-sous-variété); un tel sous-groupe s’appelle une *sous-variété* (resp. quasi-sous-variété) *de groupe* de $G$; il est nécessairement *fermé* dans $G$.

Si $H_i (i = 1, \ldots, n)$ est une sous variété de groupe de $G_i$, alors $H_1 \times \cdots \times H_n$ est une sous-variété de groupe de $G_1 \times \cdots \times G_n$.

5.12.4. Soit $G$ une variété de groupe et soit $H$ une sous-variété de groupe de $G$. La relation d’équivalence $x^{-1} y \in H$ est régulière, ce qui permet de munir l’espace $G/H$ des classes à gauche $xH$ d’une structure de variété dite *quotient* de celle de $G$. L’application canonique $(g, x) \mapsto g \cdot x$ de $G \times (G/H)$ dans $G/H$ est un morphisme. On a des résultats analogues pour l’espace homogène $H\backslash G$ des classes à droite $Hx$. Si $H$ est distingué, la structure de variété de $G/H$ est compatible avec sa structure de groupe.

5.12.5. Soit $G$ une variété de groupe et soit $X$ une variété. On appelle *loi d’opération à gauche du groupe $G$ dans la variété $X$* tout morphisme $(s, x) \mapsto sx$ de $G \times X$ dans $X$ tel que

$$
s(tx) = (st)x \quad \text{si} \quad s, t \in G, x \in X \\
ex = x \quad \text{si} \quad x \in X \ (\text{$ e $ étant l’élément neutre de } G).
$$

On dit aussi que la variété de groupe $G$ *opère à gauche* sur $X$; on définit de manière analogue les lois d’opération à droite.

Soit $x \in X$ et soit $G_x$ son stabilisateur dans $G$. Supposons que l’application $g \mapsto g \cdot x$ soit une *subimmersion* (hypothèse automatiquement vérifiée si la caractéristique de $K$ est 0 et $X$ de dimension finie). Alors $G_x$ est une sous-variété de groupe de $G$ et l’application de $G/G_x$ dans $X$ obtenue par passage au quotient à partir de $g \mapsto g \cdot x$ est une immersion. Si en outre l’orbite $G \cdot x$ de $x$ est localement fermée et si la topologie de $G$ admet une base dénombrable, $G \cdot x$ est une sous-variété de $X$ et l’application $G/G_x \to G \cdot x$ est un isomorphisme de variétés.

### 5.13. Affaiblissement de structure

Dans tout ce n°, les lettres $r, s, r', s'$ désignent, soit des entiers $\geqslant 1$, soit l’un des symboles $\infty$ et $\omega$. On suppose que $K = \mathbf{R}$.

5.13.1. Soient $r \leqslant s$, et $X$ une variété de classe $C^s$. Il existe sur l’espace topologique $X$ une structure de variété de classe $C^r$ et une seule telle que toute carte de $X$ pour la structure donnée soit une carte de $X$ pour cette nouvelle structure. Soit $X_r$ la variété de classe $C^r$ ainsi définie. On dit qu’elle se déduit de $X$ par affaiblissement de la structure de variété de $X$, ou encore que sa structure de variété est sous-jacente à celle de $X$. La notion d’affaiblissement est transitive : si $r' \leqslant r$, on a $X_{r'} = (X_r)_{r'}$; elle commute aux produits : si $Y$ est de classe $C^s$, on a $(X \times Y)_r = X_r \times Y_r$; on a un résultat analogue pour $X \times_s Y$ sous les hypothèses du n° 5.11.2.

Soit $a \in X$ et soit $c$ une carte de $X$ en $a$; c’est aussi une carte de $X_r$ en $a$. On en déduit (5.5.1) des isomorphismes

$$
\theta_c : E \to T_a(X), \quad \theta'_c : E \to T_a(X_r),
$$

d’où un isomorphisme $\theta'_c \circ \theta_c^{-1} : T_a(X) \to T_a(X_r)$. Cet isomorphisme est indépendant du choix de $c$; il permet d’identifier les espaces tangents à $X$ et à $X_r$ en $a$.

5.13.2. Soit $X$ (resp. $X'$) une variété de classe $C^s$ (resp. $C^{s'}$) et soit $r$ avec $r \leqslant \inf(s, s')$. Une application $f : X \to X'$ est dite de classe $C^r$ si c’est un morphisme de $X_r$ dans $X'_r$; une telle application est de classe $C^{r'}$ pour tout $r' \leqslant r$. De plus, l’application linéaire tangente à $f : X_r \to X'_r$ en un point $a \in X$ coïncide avec l’application linéaire tangente à $f$ considérée comme morphisme de $X_r$ dans $X'_r$.

On désignera le plus souvent par le même symbole les variétés $X$ et $X_r$; ainsi, si $X$ est de classe $C^s$, l’expression « une sous-variété de $X$ de classe $C^r$ » ($r \leqslant s$) signifie « une sous-variété de $X_r$ ».

### 5.14. Restriction du corps de base

Dans ce numéro, on se donne deux corps commutatifs valués complets non discrets $K$ et $L$, ainsi qu’un isomorphisme $\sigma$ du corps valué $K$ sur un sous-corps de $L$. Si $E$ est un espace de Banach sur $L$, on note $\sigma_*(E)$ l’espace vectoriel sur $K$ obtenu par restriction des scalaires (cf. Alg., chap. II, 3e éd., § 8); la topologie donnée sur $E$ est compatible avec la structure de $K$-espace vectoriel, et $\sigma_*(E)$ est un espace de Banach sur $K$.

5.14.1. Soit $X$ une variété analytique sur $L$ et soit $c = (U, \varphi, E)$ une carte de $X$. L’application $\varphi$ est une bijection de $U$ sur un ouvert de $\sigma_*(E)$ et le triplet $c_\sigma = (U, \varphi, \sigma_*(E))$ est une carte de $X$. Il existe sur $X$ une structure de variété analytique sur K et une seule pour laquelle $c_\sigma$ est une carte pour toute carte $c$ de la variété L-analytique X. On note $X_\sigma$ la variété analytique sur K ainsi obtenue et on dit que $X_\sigma$ est obtenue à partir de X par restriction des scalaires (de L à K au moyen de $\sigma$). L’espace topologique sous-jacent à $X_\sigma$ est le même que celui sous-jacent à X.

5.14.2. Exemples:
(a) On prend $K = \mathbf{R},\ L = \mathbf{C},\ \sigma$ étant l’injection canonique de R dans C. Ainsi, toute variété analytique complexe est canoniquement munie d’une structure de variété analytique réelle ; cette structure analytique réelle définit elle-même des structures différentielles de classe $C^r$ pour tout r.
(b) On prend $K = \mathbf{C},\ L = \mathbf{C},\ \sigma$ étant la conjugaison $x \mapsto \bar{x}$. On associe ainsi à toute variété analytique complexe X une variété analytique complexe $\overline{X}$, appelée la conjuguée de X. Si $f$ est une fonction à valeurs complexes, définie sur un ouvert U de X, $f$ est analytique pour la structure de $\overline{X}$ si et seulement si la fonction conjuguée $\bar{f}$ est analytique pour la structure de X. Les variétés X et $\overline{X}$ définissent par restriction des scalaires la même variété analytique réelle.

5.14.3. Soient X une variété analytique sur K, Y une variété analytique sur L. Une application $f : X \to Y$ est dite $\sigma$-analytique si c’est un morphisme de X dans $Y_\sigma$. Si $K \subset L,\ \sigma$ est l’injection de K dans L, et X est une variété analytique sur L, on appelle application K-analytique une application $\sigma$-analytique de $X_\sigma$ dans Y.

5.14.4. Soit V un L-espace de Banach. On a $V_\sigma = \sigma_*(V)$ : la structure canonique de variété analytique sur K de $\sigma_*(V)$ se déduit par restriction des scalaires de la structure canonique de variété analytique sur L de V.

5.14.5. Soit X une variété analytique sur L, et soit $a \in X$. Soit c une carte de X en a ; alors $c_\sigma$ est une carte de $X_\sigma$ en a et l’on en déduit des isomorphismes
$$
\theta_c : E \to T_a(X), \quad \theta_{c_\sigma} : \sigma_*(E) \to T_a(X_\sigma)
$$
d’où un isomorphisme $\theta_{c_\sigma} \circ \sigma_*(\theta_c)^{-1}$ de $\sigma_*(T_a(X))$ sur $T_a(X_\sigma)$; cet isomorphisme ne dépend pas du choix de c ; il permet d’identifier $T_a(X_\sigma)$ à $\sigma_*(T_a(X))$ et même à $T_a(X)$ par abus d’écriture.
Si $f$ est une application analytique sur L de X dans une variété Y, l’application linéaire tangente à $f$ en a ($f$ étant considérée comme un morphisme de $X_\sigma$ dans $Y_\sigma$) est égale à $\sigma_*(T_a(f))$.

5.14.6. Soient X et Y deux variétés analytiques sur L, et soit $f : X_\sigma \to Y$ une application $\sigma$-analytique. Supposons que la caractéristique de K soit 0. Alors, pour que $f$ soit analytique sur L, il faut et il suffit que, pour tout $a \in X$, l’application $T_a(f)$ soit L-linéaire.

Lorsque $K = \mathbf{R},\ L = \mathbf{C}$ (cas (a) du n° 5.14.2), on a un résultat plus précis : si $X$ et $Y$ sont de dimension finie et si $f : X \to Y$ est une application de classe $C^1$ dont l’application tangente en tout point de $x$ est $\mathbf{C}$-linéaire, alors $f$ est analytique complexe.

5.14.7. Soient $X$ une variété *analytique complexe* et $g$ une application de $X$ dans elle-même satisfaisant aux conditions :
(i) On a $g \circ g = \mathrm{Id}_X$.
(ii) L’application $g$ est un isomorphisme de la variété analytique $X$ sur la variété conjuguée $\overline{X}$ (5.14.2).

L’ensemble $X_0$ des points $x$ de $X$ tels que $g(x) = x$ est une sous-variété analytique fermée de la variété analytique réelle sous-jacente à $X$. Pour $x \in X_0$, on a $T_x(X) = T_x(X_0) \oplus i T_x(X_0)$.

Soit $U$ un ouvert *connexe* de $X$ et soient $f$ et $g$ deux applications analytiques complexes de $U$ dans un espace localement convexe séparé complexe ou dans une variété analytique complexe séparée. Si $f$ et $g$ coïncident sur une partie non vide de $U \cap X_0$, ouverte dans $X_0$, alors $f = g$.

Supposons $X_0$ paracompacte. Si $f$ est une application analytique réelle de $X_0$ dans un espace localement convexe séparé ou dans une variété analytique complexe séparée, il existe un voisinage ouvert $U$ de $X_0$ dans $X$ et une application analytique complexe de $U$ dans l’espace des valeurs de $f$, prolongeant $f$. Deux tels prolongements coïncident sur un voisinage de $X_0$ dans $X$.

Supposons $X$ de dimension finie. Pour tout point $a \in X_0$, il existe un système de coordonnées (complexes) $\zeta^1, \ldots, \zeta^n$ dans un voisinage ouvert $U$ de $a$, telles que $\zeta^i \circ g = \bar{\zeta}^i$ pour $1 \leq i \leq n$; la restriction $\zeta^i$ de $\zeta^i$ à $U \cap X_0$ est alors à valeurs réelles et $(\xi^1, \ldots, \xi^n)$ est un système de coordonnées en $a$ de la variété analytique réelle $X_0$.

5.14.8. Pour toute variété analytique réelle $Y$, *paracompacte*, il existe un couple $(X, g)$ formé d’une variété analytique complexe $X$ et d’une application $g$ de $X$ dans elle-même satisfaisant aux conditions (i) et (ii) de 5.14.7, et un isomorphisme $f$ de $Y$ sur $X_0$. On dit que $X$ (munie de $f$ et $g$) est une *complexification* de $Y$.
