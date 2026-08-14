---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 5
section_title: Revêtements principaux
lang: fr
source: ta-i-iv-fr
book_pages: A I.91-A I.119
pdf_pages: 0107-0135
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés principaux
      page: 91
      pdf_page: 107
    - "no": 2
      title: Revêtements principaux
      page: 97
      pdf_page: 113
    - "no": 3
      title: Opérations propres et libres de groupes discrets
      page: 99
      pdf_page: 115
    - "no": 4
      title: Revêtements galoisiens
      page: 101
      pdf_page: 117
    - "no": 5
      title: Espaces fibrés associés
      page: 104
      pdf_page: 120
    - "no": 6
      title: Revêtements associés
      page: 108
      pdf_page: 124
    - "no": 7
      title: Espaces fibrés principaux définis par des cocycles
      page: 114
      pdf_page: 130
statements: 58
exercises: 0
content_sha256: 1c99bc1e39127143367d30f812896f6b739a296bd750efba71a35373cd1a910a
---

## § 5. REVÊTEMENTS PRINCIPAUX

### 1. Espaces fibrés principaux

#### Définition 1 {#ta-i-s5-def-1 .statement tag=01Q5}

Soient G un groupe topologique et B un espace topologique. On appelle espace fibré principal (à droite) de base B et de groupe G un B-espace $(E, p)$ muni d’une opération à droite de G sur E (A, I, p. 50) ayant la propriété suivante :

(FP) Pour tout point $b$ de B, il existe un voisinage U de $b$ et un

U-isomorphisme $f: U\times G\rightarrow^-p^1(U)$ tels que pour tous $u\in U$

et $g,g'\in G$, on ait $f(u, gg') =f(u, g)\cdot g'$.

Au lieu de dire que $(E, p)$ est un espace fibré principal de base B et de groupe G, on dit parfois que le quadruplet $(E,G,B, p)$ est une fibration principale (cf. VAR, R, § 6), ou par abus que l’application $p: E\rightarrow B$ est une fibration principale de base B et de groupe G.

Lorsqu’aucun doute n’est possible quant à la base B, au groupe G et à l’opération de G sur E, on dira simplement que $(E, p)$ est un espace fibré principal.

Soit G un groupe topologique. Soit $(E, p)$ un B-espace muni d’une opération de G à gauche. Si, pour l’opération à droite du groupe $G^{\circ}$, opposée à l’opération donnée (A, I, p. 50), $(E, p)$ est un espace fibré principal à droite de groupe $G^{\circ}$, on dit que $(E, p)$ est un espace fibré principal à gauche de groupe G.

Un espace fibré principal est un espace fibré localement trivial (I, p. 68, déf. 1).

Il résulte de la propriété (FP) que le groupe G opère continûment (TG, III, p. 9) et librement dans E et que les orbites de cette opération sont les fibres du B-espace $(E, p)$. L’application $p': E/G\rightarrow B$ déduite de $p$ est continue et bijective. Toujours d’après la propriété (FP), l’application $p$ est ouverte (TG, I, p. 30, prop. 2 et p. 26, prop. 5) ; par suite, $p'$ est un homéomorphisme (TG, I, p. 32, prop. 3).

Soient $(E, p)$ et $(E', p')$ des espaces fibrés principaux de base B et de groupe G. On dit qu’une application $f: E\rightarrow E'$ est un morphisme d’espaces fibrés principaux (de base B et de groupe G) si $f$ est un B-morphisme et que l’on a $f(x\cdot g) =f(x)\cdot g$ pour tout $x\in E$ et tout $g\in G$. Soit $(E'', p'')$ un espace fibré principal de base B et de groupe G. Si $f: E\rightarrow E'$ et $g: E'\rightarrow E''$ sont des morphismes d’espaces fibrés principaux, l’application $g\circ f: E\rightarrow E''$ est un morphisme d’espaces fibrés principaux. Conformément aux définitions générales (E, IV, p. 11), on peut prendre pour morphismes de la structure d’espace fibré principal de base B et de groupe G ceux définis ci-dessus. On note $\mathscr{C}_B^G(E; E')$ l’ensemble des morphismes d’espaces fibrés principaux de $(E, p)$ dans $(E', p')$.

On appelle espace fibré principal trivial de base B et de groupe G le B-espace $(B\times G$, pr$_1)$ muni de la loi d’opération à droite de G sur $B\times G$ définie par $(b, g)\cdot h= (b, gh)$.

On dit qu’un espace fibré principal $(E, p)$ de base B et de groupe G est trivialisable s’il existe un isomorphisme de $(E, p)$ sur l’espace fibré principal trivial $(B\times G$, pr$_1)$ ; un tel isomorphisme est appelé trivialisation de l’espace fibré principal $(E, p)$. La propriété (FP) exprime qu’il existe un recouvrement ouvert $(U_i)_{i\in I}$ de B tel que, pour tout $i\in I$, le $U_i$-espace $(^-p^1(U_i), p|U_i)$, muni de l’opération à droite de G déduite de celle de G sur E, soit un espace fibré principal trivialisable.

#### Exemple 1 {#ta-i-s5-n1-exa-1 .statement tag=01Q6}

Soit $(E, p)$ un espace fibré principal de base B et de groupe G et soit A un sous-espace de B. Le sous-espace $E_A=^-p^1(A)$ de E est stable pour l’opération de G et l’application $p_A: E_A\rightarrow A$ en fait un espace fibré principal de base A et de groupe G. On dit que $(E_A, p_A)$ est l’espace fibré principal induit par $(E, p)$ au-dessus de A.

#### Exemple 2 {#ta-i-s5-n1-exa-2 .statement tag=01Q7}

Soit $(E, p)$ un espace fibré principal de base B et de groupe G ; soit $(E', p')$ un espace fibré principal de base $B'$ et de groupe $G'$. On définit une loi d’opération à droite du groupe $G\times G'$ sur l’espace $E\times E'$ en posant $(x, x')\cdot (g, g') = (x\cdot g, x'\cdot g')$ pour $x\in E,x'\in E',g\in G$ et $g'\in G'$; cette opération est continue. Soit U une partie ouverte de B et $f: U\times G\rightarrow^-p^1(U)$ une trivialisation du U-espace $(^-p^1(U), p_U)$ ;

soit $U'$ une partie ouverte de $B'$ et $f': U'\times G'\rightarrow (^-{p'}^1)(U')$ une trivialisation du $U'$-espace ($(^-{p'}^1)(U'), p'_U$). L’application $((b, b'),(g, g'))\mapsto$ $(f(b, g), f'(b', g'))$ est un $(U\times U')$-isomorphisme $f''$ de $(U\times U')\times (G\times G')$

sur $^-p^1(U)\times (^-{p'}^1)(U')$ et l’on a

$$
f''((b, b'),(gh, g'h')) = (f(b, gh), f'(b', g'h')) =f''((b, b'),(g, g'))\cdot (h, h')
$$

On en déduit que le $(B\times B')$-espace $E\times E'$, muni de la loi d’opération de $G\times G'$ définie ci-dessus est un espace fibré principal, appelé produit des espaces fibrés principaux E et $E'$.

#### Exemple 3 {#ta-i-s5-n1-exa-3 .statement tag=01Q8}

En particulier, lorsque $B = B'$, le B-espace $E\times_BE'$ s’identifie à l’espace fibré principal de groupe $G\times G'$ induit par $E\times E'$ au-dessus de la diagonale $\Delta_B$ de $B\times B$. Muni de cette structure d’espace fibré principal, le B-espace $E\times_BE'$ est appelé produit fibré des espaces fibrés principaux E et $E'$.

#### Exemple 4 {#ta-i-s5-n1-exa-4 .statement tag=01Q9}

Soit E un espace fibré principal de base B et de groupe G et soit F un espace topologique. Le $(B\times F)$-espace $E\times F$ muni de la loi d’opération $(x, y)\cdot g= (x\cdot g, y)$, pour $x\in E,y\in F$ et $g\in G$, est un espace fibré principal de groupe G. C’est le cas particulier de l’exemple 2, où $p'$ est l’application identique de F et $G'$ est un groupe réduit à l’élément neutre.

#### Exemple 5 {#ta-i-s5-n1-exa-5 .statement tag=01QA}

Soient B un espace topologique et $(E, p)$ un espace fibré principal de base B et de groupe G. Soient $B'$ un espace topologique et $f: B'\rightarrow B$ une application continue. Le groupe G opère à droite dans le produit fibré $B'\times_BE$ par la loi $(b', x)\cdot g= (b', x\cdot g)$, pour $b'\in B',x\in E$ et $g\in G$. Cette opération est continue et libre ; les orbites sont les fibres de l’application pr$_1: B'\times_BE\rightarrow B'$. Il résulte des exemples 1 et 4 ci-dessus et de la remarque 2 de I, p. 16 que le $B'$-espace $B'\times_BE$ est un espace fibré principal de groupe G. On l’appelle l’espace fibré principal déduit de $(E, p)$ par le changement de base $f$, ou encore l’image réciproque de $(E, p)$ par $f$.

#### Proposition 1 {#ta-i-s5-prop-1 .statement tag=01QB}

Tout morphisme d’espaces fibrés principaux est un isomorphisme.

Soit $f: B\times G\rightarrow B\times G$ un morphisme de l’espace fibré principal trivial $(B\times G$, pr$_1)$ dans lui-même et soit $\varphi : B\times G\rightarrow G$ l’application continue pr$_2\circ f$, de sorte que $f(b, g) = (b, \varphi (b, g))$. Pour tout $b\in B$ et tous $g,h\in G$, on a $\varphi (b, gh) =\varphi (b, g)\cdot h$, d’où $\varphi (b, g) =\varphi (b, e)\cdot g$, où $e$ désigne l’élément neutre de G. Le morphisme $f$ est donc un isomorphisme dont le morphisme réciproque $f^{-1}$ est défini par $f^{-1}(b, g) =$ $(b, \varphi (b, e)^{-1}g)$ pour $(b, g)\in B\times G$.

Soient maintenant E et $E'$ des espaces fibrés principaux et soit $f: E\rightarrow E'$ un morphisme d’espaces fibrés principaux. Compte tenu de la propriété (FP), pour tout point $b\in B$, il existe un voisinage ouvert U de $b$ tel que les fibrés principaux $E_U$ et $E'_U$ soient trivialisables. Par passage aux sous-espaces, $f$ induit un morphisme $f_U: E_U\rightarrow E'_U$ d’espaces fibrés principaux ; d’après ce qui précède, ce morphisme $f_U$ est un isomorphisme. En particulier, $f_b: E_b\rightarrow E'_b$ est une bijection. Il existe alors une unique application $g: E'\rightarrow E$ qui induise la bijection $f_b^{-1}$ par passage aux sous-espaces. D’après la proposition 4 de I, p. 19, l’application $g$ est continue, donc $f$ est un isomorphisme d’espaces fibrés principaux.

#### Corollaire {#ta-i-s5-n1-cor-1 .statement tag=01QC}

Soient G un groupe topologique, $(E, p)$ et $(E', p')$ des espaces fibrés principaux de groupe G et de bases B et $B'$ respectivement. Soient $f: B'\rightarrow$ B et $f': E'\rightarrow$ E des applications continues telles que $p\circ f'=f\circ p'$ et telles que, pour tout $x'\in E'$ et tout $g\in G$, $f'(x'\cdot g) =f'(x')\cdot g$. Alors le carré

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

est un carré cartésien.

En effet, l’application $h: E'\rightarrow B'\times_BE$ définie par $h(x') =$ $(p'(x'), f'(x'))$ pour $x'\in E'$, est un $B'$-morphisme de revêtements principaux, donc un isomorphisme ; on a de plus pr$_2\circ h=f'$, d’où le résultat (I, p. 8, prop. 2).

Sous les hypothèses du corollaire précédent, on dit parfois que $f'$ est un $f$-morphisme d’espaces fibrés principaux.

#### Proposition 2 {#ta-i-s5-prop-2 .statement tag=01QD}

Soit $(E, p)$ un espace fibré principal de base B et de groupe G, et soit $\varepsilon$ la section $b\mapsto (b, e)$ de l’espace fibré principal trivial $(B\times G$, pr$_1)$, où $e$ désigne l’élément neutre de G. L’application $h\mapsto h\circ \varepsilon$ est une bijection de $\mathscr{C}_B^G(B\times G; E)$ sur l’ensemble $\mathscr{S}(B; E)$ des sections continues de $p$. La bijection réciproque associe à une section continue $s$ de $p$ le B-morphisme $(b, g)\mapsto s(b)\cdot g$.

#### Corollaire {#ta-i-s5-n1-cor-2 .statement tag=01QE}

Un espace fibré principal est trivialisable si et seulement s’il admet une section continue.

#### Proposition 3 {#ta-i-s5-prop-3 .statement tag=01QF}

Soient E et B des espaces topologiques, $p: E\rightarrow B$ une application continue et G un groupe topologique opérant à droite sur E. Les conditions suivantes sont équivalentes :

(i) Muni de l’application $p$, E est un espace fibré principal de base B et de groupe G;

(ii) Pour tout $x\in E$ et tout $g\in G$, on a $p(x\cdot g) =p(x)$, l’application $\theta : (x, g)\mapsto (x, x\cdot g)$ est un homéomorphisme de $E\times G$ sur $E\times_BE$ et tout point de B possède un voisinage sur lequel existe une section continue de l’application $p$.

(i)$\Rightarrow$(ii) : Supposons que $(E, p)$ soit un espace fibré principal. Le groupe G opère continûment et librement dans E avec pour orbites les fibres de $p$. Par suite, l’application $\theta$ est bijective et continue. Plus précisément, si l’on munit $E\times_BE$ de l’opération de G définie par $(x, y)\cdot g= (x, y\cdot g)$, l’application $\theta$ est un E-morphisme de l’espace fibré principal trivial $E\times G$ dans l’espace fibré principal $(E\times_BE\rightarrow E$, pr$_1)$ (exemple 5), donc un isomorphisme (prop. 1). Les autres assertions de (ii) résultent immédiatement de la définition.

(ii)$\Rightarrow$(i) : Posons $\varphi =$ pr$_2\circ \theta^{-1}$, de sorte que, pour tout $(x, y)\in$ $E\times_BE$, on a

$$
\theta^{-1}(x, y) = (x, \varphi (x, y)) \tag{1}
$$

L’application $\varphi : E\times_BE\rightarrow G$ est continue et, pour $(x, y)\in E\times_BE$, l’élément $\varphi (x, y)$ est l’unique élément $g$ de G tel que $y=x\cdot g$. Soit $b$ un point de B; soit U un voisinage de $b$ et soit $s$ une section continue de $p$ au-dessus de U. Pour $(u, g)\in U\times G$, posons $f(u, g) =s(u)\cdot$ $g$; l’application $f$ est un U-morphisme de $U\times G$ dans $^-p^1(U)$. Pour $y\in^-p^1(U)$, posons $f'(y) = (p(y), \varphi (s(p(y)), y))$. L’application $f'$ est un U-morphisme de $^-p^1(U)$ dans $U\times G$. On a

$$
(f\circ f')(y) =s(p(y))\cdot \varphi (s(p(y)), y) =y
$$

D’autre part, pour $(u, g)\in U\times G$, on a

$$
(f'\circ f)(u, g) =f'(s(u)\cdot g) = (u, \varphi (s(u), s(u)\cdot g)) = (u, g)
$$

Par suite, $f$ est un U-isomorphisme. Il en résulte que $(E, p)$ est un espace fibré principal de base B et de groupe G.

#### Remarque 1 {#ta-i-s5-n1-rem-1 .statement tag=01QG}

Soit $(E, p)$ un espace fibré principal de base B et de groupe G. Avec les notations de la proposition 3, l’application $\theta^{-1}: E\times_BE\rightarrow E\times G$ est une trivialisation de l’espace fibré principal pr$_1: E\times_BE\rightarrow E$. On dit que $\theta^{-1}$ est la trivialisation canonique de cet espace fibré principal.

#### Corollaire 1 {#ta-i-s5-prop-3-cor-1 .statement tag=01QH}

Soit G un groupe topologique opérant continûment à droite dans un espace topologique E. Les conditions suivantes sont équivalentes :

(i) L’espace des orbites $E/G$ est séparé et l’espace E, muni de l’application canonique $p: E\rightarrow E/G$, est un espace fibré principal de groupe G;

(ii) Le groupe G opère proprement (TG, III, p. 27) et librement dans E et tout point de $E/G$ possède un voisinage sur lequel existe une section continue de l’application $p$.

Posons $B = E/G$. Sous chacune des hypothèses (i) et (ii), le groupe G opère continûment et librement dans E, de sorte que l’application $\theta : (x, g)\mapsto (x, x\cdot g)$ est une bijection continue de $E\times G$ sur $E\times_BE$. Plaçons-nous sous cette hypothèse et notons $\varphi : E\times_BE\rightarrow G$ l’application pr$_2\circ \theta^{-1}$. Compte tenu de la formule (1), pour que $\theta$ soit un homéomorphisme, il faut et il suffit que l’application $\varphi$ soit continue. D’autre part, comme la relation d’équivalence définie par G est ouverte (TG, III, p. 10, lemme 2), pour que l’espace $E/G$ soit séparé, il faut et il suffit que le graphe $E\times_BE$ de cette relation d’équivalence soit fermé dans $E\times E$ (TG, I, p. 55, prop. 8). Enfin (TG, III, p. 31, prop. 6), pour que G opère proprement dans E, il faut et il suffit que $E\times_BE$ soit fermé dans $E\times E$ et que l’application $\varphi$ soit continue. L’équivalence des conditions (i) et (ii) résulte alors de la prop. 3.

#### Corollaire 2 {#ta-i-s5-prop-3-cor-2 .statement tag=01QI}

Soit G un groupe topologique, soient H un sous-groupe de G et $p: G\rightarrow G/H$ l’application canonique. Si l’application $p$ possède une section continue au-dessus d’un ensemble ouvert non vide de $G/H$, l’application $p$ fait de G un espace fibré principal de base $G/H$ et de groupe H.

Par translations à gauche, tout point de $G/H$ possède un voisinage au-dessus duquel l’application $p$ possède une section continue. D’autre part, pour $(g, g')$ appartenant à $G\times G$, posons $\varphi (g, g') =$ $g^{-1}g'$. Si $p(g) =p(g'),\varphi (g, g')$ appartient à H. L’application $(g, g')\mapsto$ $(g, \varphi (g, g'))$ de $G\times_{G/H}G$ dans $G\times H$ est continue et c’est la réciproque de l’application continue $\theta : G\times H\rightarrow G\times_{G/H}G$ définie par $\theta (g, h) = (g, gh)$, d’où le corollaire.

#### Remarque 2 {#ta-i-s5-n1-rem-2 .statement tag=01QJ}

Cette situation se présente notamment lorsque G est un groupe de Lie réel, de dimension finie, dénombrable à l’infini, opérant transitivement et analytiquement sur une variété analytique X. Si l’on prend pour H le fixateur d’un point de X, l’application $p$ est une submersion de G sur l’espace homogène de Lie $G/H$, isomorphe à X (LIE, III, p. 109, corollaire). Elle possède donc des sections locales (VAR, p. 50).

### 2. Revêtements principaux

#### Définition 2 {#ta-i-s5-def-2 .statement tag=01QK}

Soit B un espace topologique et soit G un groupe. Munissons G de la topologie discrète. Un espace fibré principal de base B et de groupe G est appelé un revêtement principal de B de groupe G.

Cette terminologie est légitime car un tel B-espace est un revêtement de B.

Un revêtement principal de groupe G d’un espace topologique non vide possède un degré, égal à Card G.

#### Proposition 4 {#ta-i-s5-prop-4 .statement tag=01QL}

Soient B un espace topologique, $(E, p)$ un B-espace et G un groupe topologique discret opérant à droite sur E. Les assertions suivantes sont équivalentes :

(i) Le B-espace E est un revêtement principal de groupe G ;

(ii) Pour tout $g\in G$ et tout $x\in E$, on a $p(x\cdot g) =p(x)$, l’application $p$ induit un homéomorphisme de $E/G$ sur B et l’application $\theta : (x, g)\mapsto (x, x\cdot g)$ est un homéomorphisme de $E\times G$ sur $E\times_BE$ ;

(iii) Le groupe G opère continûment et librement dans E, l’application $p$ est étale et ses fibres sont les orbites de G.

(i)$\Rightarrow$(ii) : Cela résulte de I, p. 91 et de la proposition 3 de I, p. 94.

(ii)$\Rightarrow$(iii) : Sous l’hypothèse (ii), la loi d’action de G est continue, et l’application $p$ est surjective et ouverte (TG, III, p. 10, lemme 2). Soit $x\in E$; l’application $\theta$ induit une bijection de $\{x\} \times G$ sur $\{x\} \times$ $^-p^1(p(x))$, donc le groupe G opère librement et ses orbites sont les fibres de $p$. Si $e$ désigne l’élément neutre de G, la diagonale de $E\times_BE$ est l’image de $E\times  \{e\}$ par l’homéomorphisme $\theta$. Comme le groupe G est discret, l’ensemble $\{e\}$ est ouvert dans G, donc la diagonale $\Delta_E$ est ouverte dans $E\times_BE$. D’après la proposition 7 de I, p. 31, l’application $p$ est étale.

(iii)$\Rightarrow$(i) : Toute fibre de $p$ étant une orbite de l’opération de G dans E, l’application $p$ est surjective. Comme l’application $p$ est étale, pour tout point $b$ de B, il existe un voisinage ouvert U de $b$ et une section continue $s$ de $p$ au-dessus de U. L’ensemble $s(U)$ est ouvert dans E et $s$ induit un homéomorphisme de U sur $s(U)$ (I, p. 30, cor. 3). Pour tout $g\in G$, l’ensemble $s(U)\cdot g$ est ouvert dans E et la réunion des ensembles $s(U)\cdot g$, pour tout $g\in G$, est égale à $^-p^1(U)$. Si $g$ et $g'$ sont deux éléments de G distincts, les ensembles $s(U)\cdot g$ et $s(U)\cdot g'$ sont disjoints, car G opère librement dans E. L’application $f: U\times G\rightarrow$ $^-p^1(U)$ définie par $f(u, g) =s(u)\cdot g$ pour $(u, g)\in U\times G$ est donc un homéomorphisme de $U\times G$ sur $^-p^1(U)$, compatible avec les opérations à droite de G. Par définition, E est donc un revêtement principal de B de groupe G.

#### Exemple 1 {#ta-i-s5-n2-exa-1 .statement tag=01QM}

Soient E un espace topologique, G un groupe topologique discret opérant continûment et librement dans E à droite. Pour que l’application canonique $p: E\rightarrow E/G$ fasse de E un revêtement principal de $E/G$, il faut et il suffit qu’elle soit étale (condition (iii) de la proposition 4). Par exemple, supposons qu’il existe un espace topologique X et une application étale $q: E\rightarrow X$ compatible avec l’opération de G dans E, alors E est un revêtement principal de $E/G$. En effet, notons $q': E/G\rightarrow X$ l’application déduite de $q$; on a $q=q'\circ p$, donc $p$ est étale d’après la proposition 6, d) de I, p. 29.

#### Exemple 2 {#ta-i-s5-n2-exa-2 .statement tag=01QN}

Soit $q: E\rightarrow$ X une application étale et séparée. Le groupe Aut$_X(E)$, muni de la topologie discrète, opère continûment à gauche dans E. Si l’espace E est connexe, cette opération est libre (I, p. 34, corollaire 2). Notons G le groupe Aut$_X(E)^{\circ}$ et munissons E de l’opération à droite opposée à celle de Aut$_X(E)$. D’après l’exemple précédent, l’espace E, muni de l’application canonique $p: E\rightarrow E/G$, est un revêtement principal de groupe G.

### 3. Opérations propres et libres de groupes discrets

#### Théorème 1 {#ta-i-s5-thm-1 .statement tag=01QO}

Soit G un groupe discret opérant continûment à droite dans un espace topologique E. Supposons que tout point de E possède un voisinage U tel que $U\cap (U\cdot g) =\emptyset$ pour tout élément $g$ de G autre que l’élément neutre. Alors, l’application canonique $p: E\rightarrow E/G$ fait de E un revêtement principal de $E/G$ de groupe G.

L’opération de G dans E est libre par hypothèse, donc il suffit de démontrer que l’application $p$ est étale (I, p. 98, exemple 1). Soit $x$ un point de E et soit U un voisinage ouvert de $x$ tel que $U\cap U\cdot g=\emptyset$ pour tout élément $g$ de G distinct de l’élément neutre. L’application $p$ est ouverte (TG, III, p. 10, lemme 2) et induit une application injective, continue et ouverte de U sur $p(U)$, donc un homéomorphisme, ce qui prouve que l’application $p$ est étale.

#### Exemple 1 {#ta-i-s5-n3-exa-1 .statement tag=01QP}

Soit $n$ un entier $\geqslant 0$, soit $\mathbf{P}_n(\mathbf{R})$ l’espace projectif à $n$ dimensions (TG, VI, p. 13) et soit $\mathbf{S}_n$ la sphère unité de $\mathbf{R}^{n+1}$ (TG, VI, p. 9). L’application canonique de $\mathbf{S}_n$ sur $\mathbf{P}_n(\mathbf{R})$ fait de $\mathbf{S}_n$ un revêtement principal de groupe $\{1,-1\}$, ce groupe opérant par homothéties ; les orbites sont les paires de points diamétralement opposés.

#### Exemple 2 {#ta-i-s5-n3-exa-2 .statement tag=01QQ}

Tout revêtement de degré 2 possède une unique structure de revêtement principal de groupe $\mathbf{Z}/2\mathbf{Z}$.

#### Exemple 3 {#ta-i-s5-n3-exa-3 .statement tag=01QR}

Soient X une variété différentielle séparée localement de dimension finie sur $\mathbf{R}$ et $\widetilde{X}$ la variété des orientations du fibré tangent de X (VAR, R, 10.2.4). L’espace $\widetilde{X}$, muni de sa projection canonique sur X, est un revêtement principal de X de groupe $\{1,-1\}$.

#### Corollaire 1 {#ta-i-s5-thm-1-cor-1 .statement tag=01QS}

Soit G un groupe topologique discret opérant continûment à droite dans un espace topologique E. Les conditions suivantes sont équivalentes :

(i) Le groupe G opère proprement et librement dans E ;

(ii) L’espace $E/G$ est séparé et l’espace E est un revêtement principal de base $E/G$ et de groupe G.

En outre, sous ces conditions, l’espace E est séparé.

Supposons la condition (i) satisfaite. Alors les espaces E et $E/G$ sont séparés (TG, III, p. 29, prop. 3) et il existe pour tout $x\in E$ un voisinage ouvert U de $x$ dans E tel que $U\cap (U\cdot g) =\emptyset$ pour tout élément $g$ de G autre que l’élément neutre (TG, III, p. 32, prop. 8). D’après le th. 1, la condition (ii) est alors satisfaite.

L’implication (ii)$\Rightarrow$(i) résulte du corollaire 1 de I, p. 96.

#### Corollaire 2 {#ta-i-s5-thm-1-cor-2 .statement tag=01QT}

Soit G un groupe topologique et soit H un sous-groupe discret de G. Faisons opérer H sur G par translations à droite. Alors, l’application canonique de G dans l’espace $G/H$ des classes à gauche suivant H munit G d’une structure de revêtement principal de $G/H$ de groupe H.

Soit V un voisinage de l’élément neutre $e$ de G tel que $H\cap V =\{e\}$. Il existe un voisinage ouvert U de $e$ dans G tel que $U^{-1}\cdot U\subset V$ (TG, III, p. 3) et, par suite, $U\cap U\cdot h=\emptyset$ pour tout $h\in H,h=\not e$. Le corollaire 2 de I, p. 100 résulte donc du théorème 1.

#### Exemple 4 {#ta-i-s5-n3-exa-4 .statement tag=01QU}

Muni de l’application canonique de $\mathbf{R}$ sur $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. $2),\mathbf{R}$ est un revêtement principal de $\mathbf{R}/\mathbf{Z}$ de groupe $\mathbf{Z}$.

#### Remarque 1 {#ta-i-s5-n3-rem-1 .statement tag=01QV}

Soient G un groupe topologique séparé, K un sous-groupe compact de G et H un sous-groupe discret de G. Le groupe G opère continûment et proprement à droite dans l’espace $K\backslash G$ des classes à droite suivant K (TG, III, p. 30, corollaire). Comme le groupe H est fermé dans G, il opère aussi proprement dans $K\backslash G$ (TG, III, p. 27, exemple 1). Si, de plus, on a $H\cap gKg^{-1}=\{e\}$ pour tout $g\in G$, le groupe H opère librement dans $K\backslash G$. L’espace $K\backslash G$ est alors un revêtement principal de groupe H de $K\backslash G/H$ d’après le corollaire 1.

#### Corollaire 3 {#ta-i-s5-thm-1-cor-3 .statement tag=01QW}

Soient G et $G'$ des groupes topologiques, soit $\varphi : G\rightarrow G'$ un homomorphisme continu, ouvert et surjectif. On suppose que le noyau H de $\varphi$ est discret. Alors, pour l’opération de H dans G par translations à droite, $\varphi$ fait de G un revêtement principal de $G'$ de groupe H.

Si de plus le groupe G est connexe, H est contenu dans le centre de G.

L’homomorphisme $\varphi$ induit un isomorphisme de groupes topologiques de $G/H$ sur $G'$ (TG, III, p. 16, prop. 24), d’où la première assertion d’après le corollaire 2. Supposons le groupe G connexe. Pour tout $h\in H$, l’application continue de G dans H définie par $g\mapsto ghg^{-1}$ est constante, de valeur $h$. Le groupe H est donc contenu dans le centre de G.

#### Remarque 2 {#ta-i-s5-n3-rem-2 .statement tag=01QX}

Soient G et $G'$ des groupes topologiques et soit $\varphi : G\rightarrow G'$ un homomorphisme continu et ouvert. Si le groupe $G'$ est connexe, l’homomorphisme $\varphi$ est surjectif. En effet, $\varphi (G)$ est un sous-groupe ouvert, donc fermé, de $G'$, et par suite, égal à $G'$.

#### Remarque 3 {#ta-i-s5-n3-rem-3 .statement tag=01QY}

Soit G un groupe localement compact dénombrable à l’infini et soit $G'$ un groupe topologique séparé dont l’espace sous-jacent est un espace de Baire. Tout homomorphisme continu et surjectif de G dans $G'$ est ouvert (TG, IX, p. 56, corollaire et TG, III, p. 16, prop. 24).

#### Exemple 5 {#ta-i-s5-n3-exa-5 .statement tag=01QZ}

Pour tout entier $n >$ 0, notons $\mu_n$ le groupe des racines $n$-ièmes de l’unité dans $\mathbf{C}$ (A, V, p. 75). L’application $z\mapsto z^n$ fait de $\mathbf{C}^*$ un revêtement principal de $\mathbf{C}^*$ de groupe $\mu_n$, ce groupe opérant dans $\mathbf{C}^*$ par multiplication.

#### Exemple 6 {#ta-i-s5-n3-exa-6 .statement tag=01R0}

Muni de l’application $z\mapsto e^{2\pi iz}$ (TG, VIII, p. 8, remarque), l’espace $\mathbf{C}$ est un revêtement principal de $\mathbf{C}^*$ de groupe $\mathbf{Z}$. L’application $x\mapsto e^{2\pi ix}=\mathbf{e}(x)$ de $\mathbf{R}$ sur $\mathbf{S}_1$ fait de $\mathbf{R}$ un revêtement principal de $\mathbf{S}_1$ de groupe $\mathbf{Z}$.

### 4. Revêtements galoisiens

#### Définition 3 {#ta-i-s5-def-3 .statement tag=01R1}

Soit B un espace topologique non vide. On dit qu’un revêtement E de B est galoisien s’il est connexe et si, pour tout point $b$ de B, l’opération du groupe Aut$_B(E)$ des B-automorphismes de E sur la fibre $E_b$ est transitive.

Soit E un revêtement galoisien d’un espace topologique B et soit $p$ sa projection. L’application $p$ est surjective (A, I, p. 56, déf. 6) donc l’espace B est connexe. Par suite, le revêtement $(E, p)$ possède un degré, non nul.

#### Proposition 5 {#ta-i-s5-prop-5 .statement tag=01R2}

Soit B un espace topologique non vide et soit E un revêtement galoisien de B. L’application $(h, x)\mapsto h(x)$ de Aut$_B(E)\times E$ dans E est une loi d’opération à droite du groupe Aut$_B(E)^{\circ}$ sur E qui fait de E un revêtement principal de groupe Aut$_B(E)^{\circ}$.

Munissons le groupe Aut$_B(E)^{\circ}$ de la topologie discrète ; la loi d’opération $(h, x)\mapsto h(x)$ est alors continue. Cette opération est libre (I, p. 34, corollaire 2 de la proposition 11). Comme E est un revêtement galoisien de B, ses fibres sont les orbites de cette opération. D’après la proposition 4 de I, p. 97, E est un revêtement principal de groupe Aut$_B(E)^{\circ}$.

#### Théorème 2 {#ta-i-s5-thm-2 .statement tag=01R3}

Soit B un espace topologique connexe, soit E un revêtement de B, connexe et non vide. Les propriétés suivantes sont équivalentes :

(i) Le revêtement E est galoisien ;

(ii) Il existe un groupe topologique discret G et une opération continue à droite de G dans E qui fasse de E un revêtement principal de groupe G ;

(iii) Le revêtement $E\times_BE$ de E défini par la projection pr$_1$ est trivialisable.

Lorsque ces conditions sont réalisées, l’application canonique $G\rightarrow$ Aut$_B(E)^{\circ}$ définie par l’opération de G est un isomorphisme de groupes.

Si, de plus, l’espace B est localement connexe, les propriétés précédentes sont équivalentes à la propriété suivante :

(i$')$ Il existe un point $b$ de B tel que l’opération du groupe Aut$_B(E)$ dans la fibre $E_b$ soit transitive.

L’implication (i)$\Rightarrow$(ii) résulte de la proposition 5 et l’implication (ii)$\Rightarrow$(iii) de la remarque 1 de I, p. 95. Démontrons (iii)$\Rightarrow$(i). Notons $p: E\rightarrow B$ la projection du revêtement E. Comme B est connexe, ce revêtement possède un degré, et ce degré n’est pas nul car E n’est pas vide. Soit $b$ un point de B. Démontrons que l’opération de Aut$_B(E)$ sur la fibre $E_b$ est transitive. D’après ce qui précède, cette fibre n’est pas vide. Soient $x$ et $x'$ des points de $E_b$. Les B-morphismes $h: E\rightarrow E$ tels que $h(x) =x'$ correspondent bijectivement aux sections continues $s$ de l’application pr$_1: E\times_BE\rightarrow E$ telles que $s(x) = (x, x')$ (I, p. 9, prop. 3). Sous l’hypothèse (iii), une telle section existe (I, p. 70, cor. 2) et est unique (I, p. 34, cor. 1 de la prop. 11) car l’espace E est connexe. Ainsi, pour tout couple $(x, x')\in E\times_BE$, il existe un unique B-morphisme $h: E\rightarrow E$ tel que $h(x) =x'$. Si $h': E\rightarrow E$ est l’unique B-morphisme tel que $h'(x') =x$, on a $h'(h(x)) =x$ et $h(h'(x')) =x'$, d’où $h'\circ h=$ Id$_E$ et $h\circ h'=$ Id$_{E'}$. Cela prouve que $h$ est un B-automorphisme de E. Le revêtement E est donc galoisien.

Nous avons démontré que les conditions (i), (ii), (iii) sont équivalentes. Supposons-les satisfaites. Soit $\delta : G\rightarrow$ Aut$_B(E)$ l’application qui à $g\in G$ associe le B-automorphisme $x\mapsto x\cdot g$ de E. L’application $\delta$ est un homomorphisme de groupes de G dans Aut$_B(E)^{\circ}$. Comme G opère librement dans E, l’application $\delta$ est injective. Soit $h\in$ Aut$_B(E)$, soit $x\in$ E et soit $g$ l’unique élément de G tel que $x\cdot g=h(x)$. Les B-morphismes $h$ et $\delta (g)$ coïncident en $x$, donc partout, car l’espace E est connexe (I, p. 34, cor. 1 de la prop. 11), ce qui prouve que $\delta$ est un isomorphisme.

Supposons maintenant l’espace B localement connexe et démontrons, sous l’hypothèse (i$')$, que le revêtement E est galoisien. Soit $E'$ l’espace quotient de E par l’opération à droite de Aut$_B(E)^{\circ}$ et notons $q: E\rightarrow E'$ l’application canonique. Elle fait de E un revêtement surjectif de $E'($I, p. 98, exemple 2) ; l’application $p: E\rightarrow B$ définit par passage au quotient une application continue $p': E'\rightarrow B$ telle que $p'\circ q=p$. Comme l’espace B est localement connexe, le B-espace $(E', p')$ est un revêtement (I, p. 81, prop. 7). Sous l’hypothèse (i$')$, il existe un point $b$ de B tel que la fibre $E'_b$ ait exactement un élément ; comme l’espace B est connexe, il en est alors de même pour tout point $b$ de B (I, p. 74, prop. 4), ce qui démontre que E est un revêtement galoisien de B.

#### Proposition 6 {#ta-i-s5-prop-6 .statement tag=01R4}

Soient B un espace topologique et G un groupe. Soit $(E, p)$ un revêtement de B, principal de groupe G. Supposons l’espace B connexe et localement connexe. Soit $E_0$ une composante connexe de E et soit $G_0$ le sous-groupe de G stabilisateur de $E_0$ (A, I, p. 51). Le B-espace $(E_0, p|E_0)$ est un revêtement principal pour l’opération à droite de $G_0$ dans $E_0$. Ce revêtement est galoisien.

Comme l’espace B est localement connexe, il en est de même de E, de sorte que $E_0$ est un sous-espace ouvert de E (TG, I, p. 85, prop. 11). Comme il est aussi fermé (TG, I, p. 83), l’espace $E_0$ est donc un revêtement de B (I, p. 80, cor. 1). Puisque B est connexe, ce revêtement a un degré ; comme $E_0$ n’est pas vide, toutes les fibres de $p|E_0$ sont donc non vides. Soit $x$ un point de $E_0$, soit $x'\in E_0$ tel que $p(x') =p(x)$ ; il existe un élément $g\in G$ tel que $x\cdot g=x'$. Comme les composantes connexes $E_0$ et $E_0\cdot g$ ont alors un point commun, elles sont égales, ce qui entraîne $g\in G_0$. Ainsi, le groupe $G_0$ opère transitivement dans la fibre du B-espace $E_0$ en $p(x)$. La prop. 6 en résulte.

#### Remarque {#ta-i-s5-n4-rem-1 .statement tag=01R5}

Si, dans la proposition 6, on ne suppose pas l’espace B localement connexe, il peut arriver que l’espace $E_0$ ne soit pas un revêtement de B (I, p. 147, exerc. 1).

### 5. Espaces fibrés associés

Soient E et F des ensembles et soit G un groupe opérant à droite sur E et à gauche sur F. Le groupe G opère à droite sur le produit $E\times F$ par la loi $(x, y)\cdot g= (x\cdot g, g^{-1}\cdot y)$, pour $g\in G$, $(x, y)\in E\times F$. L’ensemble quotient de $E\times F$ par cette opération est noté $E\times^GF$.

Lorsque E et F sont des espaces topologiques, on munit l’ensemble $E\times^GF$ de la topologie quotient de celle de $E\times F$. L’application canonique de $E\times F$ sur $E\times^GF$ est continue. Si le groupe G opère continûment dans E et F, elle est ouverte.

De plus, soit $F'$ un ensemble sur lequel G opère à gauche et soit $h: F\rightarrow F'$ une application compatible avec les opérations de G sur F et $F'$ (A, I, p. 50). L’application Id$_E\times h: E\times F\rightarrow E\times F'$ est compatible avec les opérations de G et définit par passage aux quotients une application notée Id$_E\times^Gh$ de $E\times^GF$ dans $E\times^GF'$.

Si $h: F\rightarrow F'$ est une application continue (compatible avec les opérations de G sur F et $F')$, l’application Id$_E\times^Gh$ est continue (TG, I, p. 21, prop. 6).

#### Exemple 1 {#ta-i-s5-n5-exa-1 .statement tag=01R6}

Soit F un espace topologique et soit G un groupe topologique opérant continûment à gauche dans F. Si l’on munit l’espace topologique G de l’opération de G par translations à droite, l’espace $G\times^GF$ s’identifie canoniquement à F de la façon suivante. Les applications continues $\varphi : F\rightarrow G\times F$ et $\psi : G\times F\rightarrow$ F définies par $\varphi (f) = (e, f)$ (où $e$ désigne l’élément neutre de G) et $\psi (g, f) =g\cdot f$ induisent des applications continues $\varphi : F\rightarrow G\times^GF$ et $\psi : G\times^GF\rightarrow F$ qui sont réciproques l’une de l’autre.

#### Exemple 2 {#ta-i-s5-n5-exa-2 .statement tag=01R7}

L’exemple 1 se généralise comme suit. Soient B et F des espaces topologiques et soit G un groupe topologique opérant continûment à gauche dans F. Par passage aux quotients, l’application de $B\times F$ dans $(B\times G)\times F$ donnée par $(b, f)\mapsto ((b, e), f)$ et l’application de $(B\times G)\times F$ dans $B\times F$ donnée par $((b, g), f)\mapsto (b, gf)$ définissent des B-isomorphismes $B\times F\rightarrow (B\times G)\times^GF$ et $(B\times G)\times^GF\rightarrow B\times F$ réciproques l’un de l’autre.

#### Exemple 3 {#ta-i-s5-n5-exa-3 .statement tag=01R8}

De façon analogue, soit E un espace topologique et soit G un groupe topologique opérant continûment à droite dans E. Si l’on munit l’espace topologique G de l’opération de G par translations à gauche, l’espace $E\times^GG$ s’identifie à E.

Soient E et F des espaces topologiques et soit G un groupe topologique opérant continûment à droite dans E et à gauche dans F. Soient B un espace topologique et $p: E\rightarrow B$ une application continue telle que $p(x\cdot g) =p(x)$ pour $x\in E$ et $g\in G$. L’application $p\circ$ pr$_1: E\times F\rightarrow B$ définit, par passage au quotient, une application continue $p^F: E\times^GF\rightarrow B$ et l’application canonique $\pi : E\times F\rightarrow E\times^GF$ est un B-morphisme.

Soit $B'$ un espace topologique et soit $h: B'\rightarrow B$ une application continue. Le groupe G opère continûment à droite dans $B'\times_BE$ par la loi d’opération $((b', x), g)\mapsto (b', x\cdot g)$. En composant l’isomorphisme canonique $((b', x), y)\mapsto (b',(x, y))$ de $(B'\times_BE)\times F$ sur $B'\times_B(E\times F)$ et l’application Id$_{B'}\times \pi$ de $B'\times_B(E\times F)$ dans $B'\times_B(E\times^GF)$, on obtient une application continue $\lambda_0: (B'\times_BE)\times F\rightarrow B'\times_B(E\times^GF)$. Elle définit par passage au quotient une application continue

$$
\lambda : (B'\times_BE)\times^GF\rightarrow B'\times_B(E\times^GF)
$$

#### Lemme {#ta-i-s5-n5-lem-1 .statement tag=01R9}

L’application $\lambda$ est un homéomorphisme.

L’application $\lambda_0$ est surjective et deux éléments de $(B'\times_BE)\times F$ ont même image par $\lambda_0$ si et seulement s’ils appartiennent à une même orbite pour l’opération de G dans $(B'\times_BE)\times F$. Il en résulte que l’application $\lambda$ est bijective. Comme l’application $\pi$ est ouverte, il en est de même de l’application Id$_{B'}\times_B\pi ($I, p. 17, prop. 8), donc de $\lambda_0$ et de $\lambda$ (TG, I, p. 32, prop. 3), ce qui démontre que $\lambda$ est un homéomorphisme.

#### Proposition 7 {#ta-i-s5-prop-7 .statement tag=01RA}

Soit B un espace topologique, soit G un groupe topologique, soit $(E, p)$ un B-espace fibré principal de groupe G et soit F un espace topologique dans lequel le groupe G opère continûment à gauche.

a) L’espace topologique $E\times^GF$ muni de l’application continue $p^F: E\times^GF\rightarrow B$ déduite de l’application $p\circ$pr$_1: E\times F\rightarrow B$ par passage au quotient est un espace fibré localement trivial de fibre-type F; il est trivialisable si le B-espace fibré E est trivialisable.

b) Soit $\pi : E\times F\rightarrow E\times^GF$ la surjection canonique. L’application $\mu: E\times F\rightarrow E\times_B(E\times^GF)$ qui à $(x, f)$ associe $(x, \pi (x, f))$ est un homéomorphisme dont l’application réciproque est une trivialisation du E-espace fibré localement trivial $(E\times_B(E\times^GF)$, pr$_1)$.

Supposons d’abord que E soit le B-espace fibré principal trivial $B\times G$. D’après l’exemple 2, l’espace $E\times^GF$ s’identifie alors à $B\times F$ et l’application $p^F$ à la première projection pr$_1: B\times F\rightarrow B$, ce qui démontre que $(E\times^GF, p^F)$ est un B-espace fibré trivialisable dans ce cas. Dans le cas général, tout point de B possède un voisinage U tel que l’application $p_U:^-p^1(U)\rightarrow U$ fasse de $^-p^1(U)$ un U-espace fibré principal trivialisable. D’après ce qui précède, $(^-p^1(U)\times^GF\rightarrow U,(p_U)^F)$ est un U-espace fibré trivialisable. D’après le lemme ci-dessus, appliqué au cas où $B'= U$ et $h: U\rightarrow B$ est l’injection canonique, il en est de

même du U-espace ($(p^{-F1})(U),(p^F)_U$) déduit de $(E\times^GF, p^F)$ par restriction au-dessus de U. Ceci démontre que $(E\times^GF, p^F)$ est un B-espace fibré localement trivial et conclut la preuve de l’assertion a).

L’application $\theta : E\times G\rightarrow E\times_BE$ définie par $\theta (x, g) = (x, x\cdot g)$ est un homéomorphisme (I, p. 94, prop. 3) compatible avec les opérations de G sur $E\times G$ et sur $E\times_BE$ données par $((x, g), g')\mapsto (x, gg')$ et $((x, y), g')\mapsto (x, yg')$ respectivement. Par passage aux quotients, $\theta$ induit donc un homéomorphisme $\theta '$ de $(E\times G)\times^GF$ sur $(E\times_B$ $E)\times^GF$. L’application $\mu$ est composée de l’homéomorphisme $E\times F\rightarrow$ $(E\times G)\times^GF$ (exemple 2), de $\theta '$ et de l’homéomorphisme canonique $(E\times_BE)\times^GF\rightarrow E\times_B(E\times^GF)$ (I, p. 105, lemme), d’où b).

Sous les hypothèses de la proposition 7, le B-espace fibré localement trivial ($E\times^GF, p^F$) est appelé espace fibré localement trivial de fibre-type F associé à l’espace fibré principal $(E, p)$. Toutes les fibres du B-espace $E\times^GF$ sont homéomorphes à l’espace F. En particulier, si l’espace F est discret, l’application $p^F$ est un revêtement.

#### Exemple 4 {#ta-i-s5-n5-exa-4 .statement tag=01RB}

Soient B un espace topologique, G un groupe topologique et soit $(E, p)$ un B-espace fibré principal de groupe G. Soit H un sous-groupe de G.

Notons $\varphi : E\rightarrow E\times (G/H)$ et $\psi : E\times (G/H)\rightarrow E/H$ les applications définies par $\varphi (x) = (x,H)$ et $\psi (x, gH) = (x\cdot g)H$. Elles sont compatibles aux projections vers B et aux opérations de G et définissent par passage aux quotients des morphismes de B-espaces $\varphi : E/H\rightarrow E\times^G(G/H)$ et $\psi : E\times^G(G/H)\rightarrow E/H$, réciproques l’un de l’autre. On dit que $\varphi$ est l’homéomorphisme canonique de $E/H$ sur $E\times^G(G/H)$. En particulier, l’espace topologique $E/H$ muni de l’application continue $p_H: E/H\rightarrow B$ est un B-espace fibré localement trivial de fibre-type $G/H$.

Si de plus H est un sous-groupe distingué dans G, l’action de G munit, par passage aux quotients, le B-espace $E/H$ d’une structure d’espace fibré principal de groupe $G/H$.

En particulier, si E est un revêtement principal de B de groupe G, $E/H$ est un revêtement de B ; si H est distingué dans G, c’est un revêtement principal de groupe $G/H$.

#### Exemple 5 {#ta-i-s5-n5-exa-5 .statement tag=01RC}

Soit B un espace topologique, soit G un groupe topologique et soit E un B-espace fibré principal de groupe G. Soit F un espace homogène topologique relativement à G (TG, III, p. 12). Soit $y$ un point de F et soit $G_y$ son fixateur. L’application $\varphi_y:x\mapsto (x, y)$ de E dans $E\times F$ définit par passage aux quotients un homéomorphisme $\varphi_y$ de $E/G_y$ sur $E\times^GF$. Lorsque le groupe G est abélien, le sous-groupe $G_y$ ne dépend pas du point $y$, mais l’homéomorphisme $\varphi_y$, en général, en dépend.

#### Exemple 6 {#ta-i-s5-n5-exa-6 .statement tag=01RD}

Soit B un espace topologique, soit G un groupe topologique, soit $(E, p)$ un B-espace fibré principal de groupe G. Soit H un groupe topologique et soit $f: G\rightarrow H$ un morphisme de groupes topologiques ; munissons H de l’opération à gauche de G donnée par $g\cdot h=f(g)h$.

Soit $q: E\times H\rightarrow E\times^GH$ l’application canonique ; elle est ouverte, donc universellement stricte (I, p. 20, corollaire 11). L’application $m: (x, h, h')\mapsto q(x, hh')$ de $E\times H\times H$ dans $E\times^GH$ est continue. Soient $(x, h)\in E\times H,h'\in H$ et $g\in G$; on a $m(xg, f(g)^{-1}h, h') =$ $q(xg, f(g)^{-1}hh') =q(x, hh') =m(x, h, h')$. Par suite, il existe une unique application

$$
m': (E\times^GH)\times H\rightarrow E\times^GH
$$

telle que $m'(q(x, h), h') =q(x, h, h')$ pour tout $x\in E$ et tous $h, h'\in H$. Puisque $q$ est universellement stricte, l’application $m'$ est continue. C’est une opération à droite du groupe topologique H dans le B-espace $E\times^GH$.

Soit U un ouvert de B tel que $E_U$ soit isomorphe au U-espace fibré principal $U\times G$. Muni de l’opération de H, le U-espace $(E\times^GH)_U$ s’identifie à l’espace fibré principal $U\times H$. Cela prouve que $E\times^GH$ est un B-espace fibré principal de groupe H.

#### Définition 4 {#ta-i-s5-def-4 .statement tag=01RE}

Soit B un espace topologique et soit G un groupe topologique. Un B-espace fibré localement trivial X est dit associable à un B-espace fibré E principal de groupe G s’il existe un espace topologique F sur lequel le groupe G opère continûment à gauche et un B-isomorphisme de $E\times^GF$ sur X.

Soit E un B-espace fibré principal de groupe G et soit X un B-espace fibré localement trivial associable à E. Si l’espace fibré principal E est trivialisable, X est trivialisable (prop. 7). Si $B'$ est un espace topologique et $h: B'\rightarrow B$ une application continue, le $B'$-espace fibré localement trivial $B'\times_BX$ déduit de X par changement de base est associable au $B'$-espace fibré principal $B'\times_BE$ (I, p. 105, lemme).

### 6. Revêtements associés

Soit B un espace topologique, soit G un groupe topologique discret et soit E un revêtement de B principal de groupe G. Soit F un G-ensemble ; si l’on munit F de la topologie discrète, le groupe G opère continûment dans F. Le B-espace $E\times^GF$ est alors un revêtement. On l’appelle le revêtement de B de fibre-type F associé au revêtement principal E.

#### Définition 5 {#ta-i-s5-def-5 .statement tag=01RF}

Soit B un espace topologique, soit G un groupe topologique discret et soit E un revêtement de B principal de groupe G. Un revêtement X de B est dit associable au revêtement principal E s’il existe un G-ensemble F et un B-isomorphisme de $E\times^GF$ sur X.

Soit B un espace topologique, soit G un groupe topologique discret et soit E un revêtement de B, principal de groupe G.

Pour tout revêtement X de B, le groupe G opère à gauche sur $\mathscr{C}_B(E; X)$ par la loi définie par $(g\cdot h)(x) =h(x\cdot g)$ pour $x\in E$, $g\in G,h\in \mathscr{C}_B(E; X)$.

Pour tout G-ensemble F muni de la topologie discrète, définissons une application $\alpha_F: F\rightarrow \mathscr{C}_B(E; E\times^GF)$ par :

(2) $\alpha_F(y)(x) =\pi (x, y)$ pour $y\in F$ et $x\in E$,

où $\pi : E\times F\rightarrow E\times^GF$ est la surjection canonique. L’application $\alpha_F$ est compatible avec les opérations de G sur F et sur $\mathscr{C}_B(E; E\times^GF)$.

Pour tout revêtement X de B, il existe une unique application $\beta_X$ de $E\times^G\mathscr{C}_B(E; X)$ dans X telle que :

(3) $\beta_X(\pi (x, h)) =h(x)$ pour $h\in \mathscr{C}_B(E; X)$ et $x\in E$.

En effet, on a $(g^{-1}\cdot h)(x\cdot g) =h(x)$ pour $x\in E,g\in G$ et $h\in \mathscr{C}_B(E; X)$, par définition de l’opération de G dans $\mathscr{C}_B(E; X)$. Lorsqu’on munit l’ensemble $\mathscr{C}_B(E; X)$ de la topologie discrète, l’application $\beta_X$ est un B-morphisme de revêtements.

Lorsque $X = E\times^GF$, on a

(4) $\beta_X(\pi (x, \alpha_F(y))) =\pi (x, y)$ pour $x\in X$ et $y\in F$.

#### Proposition 8 {#ta-i-s5-prop-8 .statement tag=01RG}

Soit B un espace topologique connexe et non vide. Soit G un groupe discret et soit $(E, p)$ un revêtement de B principal de groupe G. Supposons que E soit connexe. Avec les notations ci-dessus, on a :

a) Pour tout G-ensemble F muni de la topologie discrète, l’application $\alpha_F$ est un isomorphisme du G-ensemble F sur le G-ensemble $\mathscr{C}_B(E; E\times^GF)$.

b) Soit X un revêtement de B. Le B-morphisme $\beta_X$ est un isomorphisme de $E\times^G\mathscr{C}_B(E; X)$ sur X si et seulement si le revêtement $(E\times_BX$, pr$_1)$ de E est trivialisable.

a) Soient $y$ et $y'$ des points de F tels que $\alpha_F(y) =\alpha_F(y')$. L’espace E n’est pas vide ; choisissons-en un point $x$. On a $\pi (x, y) =\pi (x, y')$ dans $E\times^GF$. Par suite, il existe $g\in G$ tel que $x\cdot g=x$ et $g^{-1}\cdot y=y'$. La première égalité implique que $g$ est l’élément neutre $e$ de G, donc $y=y'$. Ainsi, l’application $\alpha_F$ est injective. D’autre part, soit $h\in$ $\mathscr{C}_B(E; E\times^GF)$ et soit $x$ un point de E. Soient $x'\in E,y'\in F$ tels que $h(x) =\pi (x', y')$. En particulier, $p(x) =p(x')$ ; il existe alors un élément $g$ de G tel que $x'=x\cdot g$ et l’on a aussi $h(x) =\pi (x, y)$, où l’on a posé $y=g\cdot y'$. Les B-morphismes $h$ et $\alpha_F(y)$ coïncident au point $x$ de E ; ils sont donc égaux puisque l’espace E est connexe (I, p. 34, cor. 1 de la prop. 11), et ceci prouve que l’application $\alpha_F$ est surjective.

b) D’après la proposition 7, b) de I, p. 105 appliquée à $F =\mathscr{C}_B(E; X)$, le revêtement $p^*(E\times^G\mathscr{C}_B(E; X))$ de E est isomorphe au revêtement trivial $E\times \mathscr{C}_B(E; X)$. Si $\beta_X$ est un isomorphisme, le revêtement $p^*(X)$ de E est donc trivialisable. Inversement, supposons le revêtement $p^*(X)$ trivialisable et démontrons que le B-morphisme $\beta_X$ est bijectif ; il en résultera que $\beta_X$ est un B-isomorphisme (I, p. 30, cor. 2 de la prop. 6).

L’application $\beta_X$ est déduite par passage au quotient de l’application $\gamma : E\times \mathscr{C}_B(E; X)\rightarrow X$ définie par $\gamma (x, h) =h(x)$. Démontrons que l’application $\gamma$ est surjective. Soit $x$ un point de X. La projection du B-espace E est surjective, car c’est un revêtement principal ; il existe donc un point $y$ de E tel que $(y, x)\in E\times_BX$. Il existe alors une section continue $s$ du revêtement trivialisable pr$_1: E\times_BX\rightarrow E$ telle que $s(y) = (y, x)$. L’application $h=$ pr$_2\circ s: E\rightarrow X$ est un B-morphisme et l’on a $h(y) =x$, d’où la surjectivité de l’application $\gamma$ et, par conséquent, celle de l’application $\beta_X$.

Démontrons enfin que $\beta_X$ est injective. Soient $(x, h)$ et $(x', h')$ des éléments de $E\times \mathscr{C}_B(E; X)$ tels que $h(x) =h'(x')$. Remarquons que $x$ et $x'$ ont même projection dans B; il existe donc un élément $g$ de G tel que $x'=x\cdot g$. On a alors $h(x) =h'(x\cdot g) = (g\cdot h')(x)$. Comme l’espace E est connexe, on a $h=g\cdot h'($I, p. 34, cor. 1 de la prop. 11). Ainsi, $(x, h)$ et $(x', h')$ ont même classe dans $E\times^G\mathscr{C}_B(E; X)$, ce qui démontre que l’application $\beta_X$ est injective, et achève la démonstration.

#### Corollaire 1 {#ta-i-s5-prop-8-cor-1 .statement tag=01RH}

Soit $(E, p)$ un revêtement principal de B de groupe G ; supposons que E soit connexe et non vide. Un revêtement X de B est associable à E si et seulement si le revêtement $p^*(X)$ est trivialisable.

Si le revêtement $p^*(X)$ est trivialisable, il découle de la proposition 8, b), que le revêtement X est associable à E. Dans ce cas, l’application $\beta_X$ identifie le revêtement X au revêtement de fibre-type $\mathscr{C}_B(E; X)$ associé à E. Inversement, soit F un G-ensemble muni de la topologie discrète et supposons que l’on ait $X = E\times^GF$. Alors, $\alpha_F$ est un isomorphisme (loc. cit., a)) et la formule (4) entraîne que $\beta_X$ est un isomorphisme. Par suite, le revêtement $p^*(X)$ est trivialisable (prop. 8, b)), d’où le corollaire.

#### Corollaire 2 {#ta-i-s5-prop-8-cor-2 .statement tag=01RI}

Soit B un espace topologique connexe et localement connexe, soit $(E, p)$ un revêtement de B principal de groupe G. Soit $E_0$ une composante connexe de E et soit $G_0$ le sous-groupe de G stabilisateur de $E_0$. Le B-espace $(E_0, p|E_0)$ est un revêtement principal de groupe $G_0($I, p. 103, prop. 6).

Tout revêtement X de B qui est associable au revêtement principal E est associable au revêtement principal $E_0$. En particulier, le revêtement E est associable au revêtement principal $E_0$.

En effet, si le revêtement X est associable à E, le revêtement $p^*(X)$ est trivialisable et le revêtement $p^*_0(X)$ induit par $p^*(X)$ au-dessus de $E_0$ est donc trivialisable.

Plus précisément, notons que l’application $(x, g)\mapsto x\cdot g$ de $E_0\times G$ dans E induit, par passage au quotient, un B-isomorphisme de revêtements principaux de $E_0\times^{G_0}G$ sur E.

#### Proposition 9 {#ta-i-s5-prop-9 .statement tag=01RJ}

Soit B un espace topologique, soit E un revêtement principal de B de groupe G, connexe et non vide. Soit F un G-ensemble non vide muni de la topologie discrète. Pour que l’espace $E\times^GF$ soit connexe, il faut et il suffit que G opère transitivement dans F.

Soit U une partie ouverte et fermée de $E\times^GF$. Si $\pi : E\times F\rightarrow$ $E\times^GF$ désigne la surjection canonique, $^-\pi^1(U)$ est une partie ouverte et fermée de $E\times F$ qui est stable par G. Comme E est connexe, il existe une partie $F'\subset F$, stable par G, telle que $^-\pi^1(U) = E\times F'$, d’où $U =\pi (E\times F')$. Soient $F'$ et $F''$ des parties de F stables par G telles que $\pi (E\times F') =\pi (E\times F'')$ ; comme E n’est pas vide, on a $F'= F''$. L’application $F'\mapsto \pi (E\times F')$ est une bijection de l’ensemble des parties de F stables par G sur l’ensemble des parties ouvertes et fermées de $E\times^GF$. La proposition en résulte.

#### Proposition 10 {#ta-i-s5-prop-10 .statement tag=01RK}

Soit B un espace topologique, soit $(E, p)$ un revêtement de B principal de groupe G et soit X un revêtement de B. Supposons que E et X soient connexes et non vides. Les propriétés suivantes sont équivalentes :

(i) Le revêtement X est associable au revêtement principal E ;

(ii) Il existe un sous-groupe H de G tel que X soit B-isomorphe à $E/H$ ;

(iii) Il existe un B-morphisme surjectif $h: E\rightarrow X$ ;

(iv) Pour tout point $(y, x)$ de $E\times_BX$, il existe un B-morphisme $r: E\rightarrow X$ tel que $r(y) =x$.

Supposons ces conditions satisfaites et soit H un sous-groupe de G tel que X soit B-isomorphe à $E/H$. Le revêtement X est galoisien si et seulement si le sous-groupe H est distingué dans G.

(i)$\Rightarrow$(ii) : Soit F un G-ensemble discret tel que le revêtement $E\times^GF$ soit B-isomorphe à X. L’ensemble F n’est pas vide et l’espace $E\times^GF$ est connexe, donc le groupe G opère transitivement dans F (prop. 9). Alors, l’espace $E\times^GF$ est B-isomorphe à $E/H$, où H est le sous-groupe de G fixateur d’un point de F (I, p. 106, exemple 4).

(ii)$\Rightarrow$(iii) : En effet, la surjection canonique de E sur $E/H$ est un B-morphisme surjectif.

(iii)$\Rightarrow$(iv) : Soit $(y, x)$ un point de $E\times_BX$. Comme l’application $h$ est surjective, il existe un point $y'$ de E tel que $h(y') =x$. Les points $y$ et $y'$ ont même projection dans B. Comme le revêtement E est principal de groupe G, il existe $g\in G$ tel que $y\cdot g=y'$. L’application $r: E\rightarrow X$ définie par $z\mapsto h(z\cdot g)$ est un B-morphisme et l’on a $r(y) =x$.

(iv)$\Rightarrow$(i) : Comme X n’est pas vide et que la projection de E sur B est surjective, l’espace $E\times_BX$ n’est pas vide. Il existe donc un B-morphisme $r$ de E dans X. L’application (Id$_E, r): E\rightarrow E\times_BX$ est une section du revêtement $p^*(X)$ de E. Comme l’espace E est connexe, il résulte du corollaire 2 de la prop. 1 de I, p. 69 que le revêtement $p^*(X)$ est trivialisable, ce qui prouve que le revêtement X est associable au revêtement galoisien $p$ (proposition 8).

Supposons maintenant que ces conditions soient satisfaites. On note X le B-espace $E/H,q$ sa projection et $h: E\rightarrow E/H$ l’application canonique.

Si le groupe H est distingué dans G, alors X est un revêtement principal de groupe $G/H$ (I, p. 106, exemple 4). Comme X et B sont connexes et non vides, X est un revêtement galoisien de B (I, p. 102, th. 2). Inversement, supposons que $E/H$ soit un revêtement galoisien de B et notons K = Aut$_B(E/H)^{\circ}$. On définit une application $\alpha : E\times G\rightarrow K$ en associant à $(t, g)\in E\times G$ l’unique élément $k$ de K tel que $h(t\cdot g) =h(t)\cdot k$. Elle est continue car elle s’obtient en composant l’application continue $(t, g)\mapsto (h(t), h(t\cdot g))$ de $E\times G$ dans $X\times_BX$ avec la trivialisation canonique (I, p. 95, remarque 1) $X\times_BX\rightarrow X\times K$ de $q^*(X)$. Comme E est connexe et K est un groupe discret, l’application continue $t\mapsto \alpha (t, g)$ est constante, pour tout $g\in G$ ; on note $\alpha (g)$ sa valeur. Si $t\in E,g\in G$ et $g'\in H$, on a alors

$$
h(t) =h(t\cdot g^{-1}g) =h(t\cdot g^{-1})\cdot \alpha (g) =h(t\cdot g^{-1}\cdot g')\cdot \alpha (g) =h(t\cdot (g^{-1}g'g))
$$

Il en résulte que $g^{-1}g'g$ appartient à H et donc que H est distingué dans G.

#### Corollaire {#ta-i-s5-n6-cor-1 .statement tag=01RL}

Soit E un revêtement galoisien de B et soit X un revêtement de B, connexe et non vide. Supposons que X soit un revêtement fini ou bien que l’espace B soit localement connexe. S’il existe un B-morphisme $h: E\rightarrow X$, le revêtement X est associable au revêtement principal E.

Dans les deux cas, le B-morphisme $h$ est un revêtement (I, p. 77, cor. 3 du th. 1, et I, p. 78, prop. 5), et un revêtement non vide d’un espace connexe est surjectif (I, p. 68).

#### Théorème 3 {#ta-i-s5-thm-3 .statement tag=01RM}

Soit B un espace topologique non vide, connexe et localement connexe. Tout revêtement de B est associable à un revêtement galoisien ; tout revêtement fini de B est associable à un revêtement fini galoisien.

Soit X un revêtement de B, notons $q$ sa projection. Comme l’espace B est connexe et non vide, le revêtement X possède un degré ; notons F ce degré et munissons l’ensemble F de la topologie discrète. Comme l’espace B est localement connexe, le faisceau $\mathscr{I}$ = $\mathscr{I}$som$_B(B\times F; X)$ est localement constant et en tout point $b$ de B, sa tige $\mathscr{I}_b$ est canoniquement isomorphe à l’ensemble $\mathscr{B}(F; X_b)$ des bijections de F sur la fibre $X_b($I, p. 89, prop. 12). Soit $E = E_{\mathscr{I}}$ le revêtement associé au faisceau localement constant $\mathscr{I}($I, p. 86, corollaire).

Soit G le groupe des permutations de F. Pour tout $g\in G$, on définit comme suit un morphisme $\gamma '(g)$ du faisceau $\mathscr{I}$ dans lui-même : pour tout ouvert U de B, l’application $\gamma '(g)_U$ associe à un U-isomorphisme $\varphi : U\times F\rightarrow^-q^1(U)$ le U-isomorphisme défini par $(b, f)\mapsto \varphi (b, g(f))$ pour $b\in U$ et $f\in F$. On a $\gamma '$(Id$_F) =$ Id$_{\mathscr{I}}$ et $\gamma '(g\circ g') =\gamma '(g')\circ \gamma '(g)$, pour $g,g'\in G$, de sorte que pour tout $g\in G,\gamma '(g)$ est un automorphisme du faisceau $\mathscr{I}$. Le B-morphisme $\gamma (g): E\rightarrow E$ associé à $\gamma '(g)$ est un automorphisme (I, p. 50). Si $x= [U, \varphi , b]$ est un élément de E, où U est un ouvert de B$,b$ un point de U et $\varphi$ un U-isomorphisme de $U\times F$ sur $^-q^1(U)$, on a $\gamma (g)(x) = [U, \psi , b]$, où $\psi$ est défini par $\psi (a, f) =\varphi (a, g(f))$, pour $a\in$ U et $f\in$ F. Si $g$ et $g'$ sont des éléments de G, on a $\gamma (g\circ g') =\gamma (g')\circ \gamma (g)$. On a $\gamma$(Id$_F) =$ Id$_E$. On définit ainsi une loi d’opération à droite continue de G dans E en posant $x\cdot g=\gamma (g)(x)$, pour $x\in E$ et $g\in G$. Le groupe G opère de façon simplement transitive sur toute fibre de E, de sorte que le revêtement E muni de cette opération est un revêtement principal de groupe G (I, p. 97, prop. 4). Soit $h$ l’application de $E\times F$ dans X définie par $h([U, \varphi , b], f) =\varphi (b, f)$ pour tout ouvert U de B, tout point $b$ de U et tout U-isomorphisme $\varphi$ de $U\times F$ sur $^-q^1(U)$. Par définition de la topologie de E, elle est continue ; c’est un B-morphisme. Pour tout élément $g$ de G et tout point $(x, f)$ de $E\times F$, on a $h(x, g(f)) =h(x\cdot g, f)$. L’application $h$ définit donc, par passage au quotient, un B-morphisme $h': E\times^GF\rightarrow X$. Pour tout point $b$ de B, l’application $h_b: E_b\times F\rightarrow X_b$ s’identifie à l’application $(\varphi , f)\mapsto \varphi (f)$ de $\mathscr{B}(F; X_b)\times F$ dans $X_b$, de sorte que l’application $h'_b$ est bijective. Par suite, $h'$ est un B-isomorphisme de $E\times^GF$ sur X (I, p. 30, cor. 2 de la prop. 6).

Comme l’espace B est connexe, localement connexe et non vide, le revêtement X, associable au revêtement principal E, est associable à un revêtement galoisien (I, p. 110, corollaire 2). Si le revêtement X est fini, il en est de même du revêtement E, donc X est associable à un revêtement fini galoisien (loc. cit.).

### 7. Espaces fibrés principaux définis par des cocycles

#### Définition 6 {#ta-i-s5-def-6 .statement tag=01RN}

Soit B un espace topologique, soit G un groupe topologique et soit $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B. On appelle 1-cocycle continu sur B à valeurs dans G, subordonné à $\mathscr{U}$, la donnée, pour tout couple $(i, j)$ d’éléments de I d’une application continue $g_{i,j}$ de $U_i\cap U_j$ dans G, telle que pour tout triplet $(i, j, k)\in I\times I\times I$ et tout point $b$ de $U_i\cap U_j\cap U_k$, on ait

$$
g_{i,k}(b) =g_{i,j}(b)g_{j,k}(b)
$$

On note $Z^1_{cont}(B,\mathscr{U},G)$ l’ensemble des 1-cocycles continus sur B à valeurs dans G, subordonnés au recouvrement $\mathscr{U}$.

Dans ce numéro, nous dirons simplement cocycle au lieu de 1-cocycle continu.

Soit $(E, p)$ un B-espace fibré principal de groupe G et soit $\mathscr{U}$ = $(U_i)_{i\in I}$ un recouvrement de B par des ouverts $U_i$. On dit que E est trivialisable au-dessus de $\mathscr{U}$ si, pour tout $i\in I$, E est trivialisable au-dessus de $U_i$. On appelle alors $\mathscr{U}$ -trivialisation de E une famille $(f_i)_{i\in I}$, où $f_i:^-p^1(U_i)\rightarrow U_i\times G$ est une trivialisation de E au-dessus de $U_i$.

Soit $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement de B par des ouverts et soit $(E, p)$ un B-espace fibré principal de groupe G muni d’une $\mathscr{U}$ -trivialisation $(f_i)_{i\in I}$. Pour tout couple $(i, j)\in I\times I$, notons $g_{ij}$ l’application de $U_i\cap U_j$ dans G définie par

$$
(b, g_{ij}(b)) =f_i\circ f_j^{-1}(b, e)
$$

où $e$ désigne l’élément neutre de G. Elle est continue.

Comme $f_i$ et $f_j$ sont compatibles avec les opérations de G, on a

$$
(f_i\circ f_j^{-1})(b, g) = (b, g_{ij}(b)g)
$$

pour $b\in U_i\cap U_j$ et $g\in G$. Si $b$ est un point de $U_i\cap U_j\cap U_k$ (où $i,j$, $k\in I$), on a

$$
(f_i\circ f_k^{-1})(b, e) = (b, g_{ik}(b))
$$

et

$$
(f_i\circ f_k^{-1})(b, e) = (f_i\circ f_j^{-1})\circ (f_j\circ f_k^{-1})(b, e)
$$

$$
= (f_i\circ f_j^{-1})(b, g_{jk}(b)) = (b, g_{ij}(b)g_{jk}(b))
$$

Il en résulte que

$$
g_{ik}(b) =g_{ij}(b)g_{jk}(b)
$$

de sorte que la famille $(g_{ij})$ est un cocycle sur B à valeurs dans G, subordonné au recouvrement $\mathscr{U}$. On l’appelle le cocycle défini par la famille de trivialisations $(f_i)_{i\in I}$.

Soient B, G et $\mathscr{U}$ comme dans la définition 6 et soit $(g_{ij})\in$ $Z^1_{cont}(B,\mathscr{U},G)$ un cocycle. Pour tout couple $(i, j)\in I\times I$, l’application $\gamma_{ij}: (U_i\cap U_j)\times G\rightarrow (U_i\cap U_j)\times G$ définie par

(5) $\gamma_{ij}(b, g) = (b, g_{ij}(b)g)$ pour $b\in U_i\cap U_j$ et $g\in G$

est un isomorphisme de fibrés principaux de base $U_i\cap U_j$. Pour tout triplet $(i, j, k)\in I\times I\times I$ et tout couple $(b, g)\in (U_i\cap U_j\cap U_k)\times G$, on a :

$$
\gamma_{ik}(b, g) =\gamma_{ij}\circ \gamma_{jk}(b, g)
$$

Soit F l’espace topologique obtenu par recollement des espaces $U_i\times G$ le long des $(U_i\cap U_j)\times G$ au moyen des bijections $\gamma_{ij}$ (TG, I, p. 16). Pour tout $i\in I$, l’image de $U_i\times G$ dans F est un ensemble ouvert de F (TG, I, p. 17, prop. 9). Les projections canoniques $p_i: U_i\times G\rightarrow U_i$ se recollent en une application continue $p$ de F dans B. Les applications $\gamma_{ij}$ étant compatibles avec les opérations de G à droite dans les espaces $U_i\times G$, on en déduit une loi d’opération continue de G dans F à droite qui fait de F un espace fibré principal de base B, de groupe G, muni d’une trivialisation au-dessus de chaque $U_i$. On dit que F est l’espace fibré principal défini par le cocycle $(g_{ij})$.

#### Définition 7 {#ta-i-s5-def-7 .statement tag=01RO}

Soient B un espace topologique, G un groupe topologique et $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B. On dit que deux cocycles $(g_{ij})$ et $(g_{ij}')$ de $Z^1_{cont}(B,\mathscr{U},G)$ sont cohomologues s’il existe une famille $(h_i)_{i\in I}$ d’applications continues $h_i: U_i\rightarrow G$ telle que l’on ait

$$
g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1} \tag{6}
$$

pour tout couple $(i, j)\in I\times I$ et tout $b\in U_i\cap U_j$.

La relation « $(g_{ij})$ est cohomologue à $(g'_{ij})$ » est une relation d’équivalence dans l’ensemble $Z^1_{cont}(B,\mathscr{U},G)$. On note $H^1_{cont}(B,\mathscr{U},G)$ l’ensemble quotient de $Z^1_{cont}(B,\mathscr{U},G)$ pour cette relation d’équivalence.

#### Proposition 11 {#ta-i-s5-prop-11 .statement tag=01RP}

Soient B un espace topologique, G un groupe topologique et $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B.

a) Tout B-espace fibré principal de groupe G qui est trivialisable au-dessus de $\mathscr{U}$ est isomorphe à un espace fibré principal défini par un cocycle de $Z^1_{cont}(B,\mathscr{U},G)$.

b) Soient $(E, p)$ et $(E', p')$ des B-espaces fibrés principaux qui sont trivialisables au-dessus de $\mathscr{U}$. Soit $(f_i)_{i\in I}($ resp. $(f_i')_{i\in I})$ une trivialisation de $(E, p)$ ( resp. de $(E', p')$) adaptée à $\mathscr{U}$ et notons $(g_{ij})_{(i,j)\in I\times I}$ ( resp. $(g_{i,j}')_{(i,j)\in I\times I})$ le cocycle défini par cette trivialisation. Alors, les espaces fibrés principaux $(E, p)$ et $(E', p')$ sont isomorphes si et seulement si ces cocycles sont cohomologues.

Démontrons b). Soit $\varphi : E\rightarrow E'$ un isomorphisme de fibrés principaux de base B et de groupe G. Pour tout $i\in I$, soit $h_i$ l’application continue de $U_i$ dans G définie par

$$
(b, h_i(b)) =f_i'\circ \varphi \circ f_i^{-1}(b, e)
$$

Comme, pour tout $i\in I,f_i$ et $f_i'$ sont compatibles avec les opérations de G, on a pour tout $b\in U_i$ et tout $g\in G$,

$$
(f_i'\circ \varphi \circ f_i^{-1})(b, g) = (b, h_i(b)g)
$$

et

$$
(f_i\circ \varphi^{-1}\circ (f_i')^{-1})(b, g) = (b, h_i(b)^{-1}g)
$$

Par suite, pour tout couple $(i, j)\in I\times I$ et tout point $b$ de $U_i\cap U_j:$ $f_i'\circ (f_j')^{-1}(b, e) = (f_i'\circ \varphi \circ f_i^{-1})\circ (f_i\circ f_j^{-1})\circ (f_j\circ \varphi^{-1}\circ (f_j')^{-1})(b, e)$

$$
= (b, h_i(b)g_{ij}(b)h_j(b)^{-1})
$$

de sorte que l’on a

$$
g_{ij}'(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}
$$

Cela démontre que les cocycles $(g_{ij})$ et $(g'_{ij})$ sont cohomologues.

Inversement, supposons que ces cocycles soient cohomologues et soit $(h_i)_{i\in I}$ une famille d’applications continues $h_i: U_i\rightarrow G$ telle que l’on ait $g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}$ pour $i,j\in I$ et $b\in U_i\cap U_j$. Pour

$i\in I$, soit $\varphi_i:^-p^1(U_i)\rightarrow (^-{p'}^1)(U_i)$ l’application définie par $f_i'\circ \varphi_i\circ$ $f_i^{-1}(b, g) = (b, h_i(b)g)$, pour $b\in U_i$ et $g\in G$. C’est un isomorphisme d’espaces fibrés principaux de base $U_i$ et de groupe G. Pour $(i, j)\in$ $I\times I$, notons $\gamma_{ij}$ et $\gamma_{ij}'$ les homéomorphismes de recollement associés comme ci-dessus aux cocycles $(g_{ij})$ et $(g_{ij}')$ respectivement (I, p. 115, formule (5)), de sorte que $f_i(b, g) =\gamma_{ij}\circ f_j(b, g)$ et $f_i'(b, g) =\gamma_{ij}'\circ f_j'(b, g)$ pour tout $(b, g)\in (U_i\cap U_j)\times G$. Par suite, pour $(i, j)\in I\times I$ et $(b, g)\in (U_i\cap U_j)\times G$, on a les relations

$$
f_i'\circ \varphi_j\circ f_i^{-1}(b, g) =\gamma_{ij}'\circ (f_j'\circ \varphi_j\circ f_j^{-1})(b, g_{ij}(b)^{-1}g)
$$

$$
=\gamma_{ij}'(b, h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, g_{ij}'(b)h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, h_i(b)g) =f_i'\circ \varphi_i\circ f_i^{-1}(b, g)
$$

Cela démontre que $\varphi_i$ et $\varphi_j$ coïncident sur $^-p^1(U_i\cap U_j)$. Les morphismes $\varphi_i$ se recollent donc en un B-morphisme de fibrés principaux de E dans $E'$. L’assertion b) en résulte car tout morphisme de fibrés principaux de base B et de groupe G est un isomorphisme (I, p. 93, prop. 1).

Démontrons maintenant a). Soit $(E, p)$ un espace fibré principal de groupe G muni, pour tout $i\in I$, d’une trivialisation $f_i:^-p^1(U_i)\rightarrow$ $U_i\times G$ au-dessus de $U_i$. Soit $(g_{ij})$ le cocycle défini par cette famille et soit alors F l’espace fibré principal défini par le cocycle $(g_{ij})$. Par construction, l’espace fibré principal F est muni d’une trivialisation au-dessus de $\mathscr{U}$; cette trivialisation définit le cocycle $(g_{ij})$. D’après l’assertion b), l’espace fibré principal $(E, p)$ est isomorphe à F.

Soient B un espace topologique et G un groupe topologique. Soit $(E, p)$ un espace fibré principal de base B et de groupe G. Soit $s$ une section de l’application surjective $p$ (E, II, p. 19, prop. 8). L’application $f: B\times G\rightarrow E$ définie par $f(b, g) =s(b)\cdot g$ est une bijection compatible avec l’action de G. Munissons $B\times G$ de la topologie obtenue par transport de structure ; $(B\times G$, pr$_1)$ est alors un espace fibré principal de base B et de groupe G isomorphe à E. Il existe donc un ensemble T de fibrés principaux de base B et de groupe G tel que tout espace fibré principal de base B et de groupe G soit isomorphe à un élément de T. Notons $P(B,G)$ l’ensemble des classes d’isomorphisme de fibrés principaux de base B et de groupe G (E, II, p. 47).

Soit $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B. Notons $P(B,\mathscr{U},G)$ le sous-ensemble de $P(B,G)$ constitué des classes d’isomorphisme des fibrés principaux qui sont trivialisables au-dessus de $\mathscr{U}$. D’après la proposition 11, il existe une application $r_{\mathscr{U}}$ de $H^1_{cont}(B,\mathscr{U},G)$ dans $P(B,\mathscr{U},G)$ qui à la classe d’un cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ associe la classe d’isomorphisme de l’espace fibré principal défini par ce cocycle ; c’est une bijection (loc. cit.). La bijection réciproque $s_{\mathscr{U}}$ associe à la classe d’isomorphisme dans $H^1_{cont}(B,\mathscr{U},G)$ d’un espace fibré principal E, trivialisable au-dessus de $\mathscr{U}$, la classe du cocycle défini par une famille quelconque de trivialisations de E au-dessus de $\mathscr{U}$. Dans cette correspondance, la classe d’isomorphisme de l’espace fibré principal trivial $B\times G$ correspond à la classe de cohomologie du cocycle constant $g_{ij}=e$, appelé aussi cocycle trivial.

En vertu de la définition d’un espace fibré principal, l’ensemble $P(B,G)$ est la réunion des ensembles de la forme $P(B,\mathscr{U},G)$, où $\mathscr{U}$ est un recouvrement ouvert de B.

Soit $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B et soit $\mathscr{V}= (V_k)_{k\in K}$ un recouvrement ouvert de B plus fin que $\mathscr{U}$. On a $P(B,\mathscr{U},G)\subset$ $P(B,\mathscr{V},G)$ ; on note $i_{\mathscr{V} \mathscr{U}}$ l’injection canonique définie par cette inclusion. Choisissons une application $\varphi : K\rightarrow I$ telle que $V_k\subset U_{\varphi(k)}$ pour tout $k\in K$. Étant donné un cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$, posons, pour tout couple $(k, \ell )\in K\times K,g_{k\ell}=g_{\varphi(k)\varphi(\ell)}|V_k\cap V_{\ell}$.

La famille $(g_{k\ell})$ est un cocycle sur B, à valeurs dans G, subordonné à $\mathscr{V}$. Si $(g_{ij}')\in Z^1_{cont}(B,\mathscr{U},G)$ est un cocycle cohomologue au cocycle $(g_{ij})$, le cocycle $(g'_{k\ell})$ déduit de $(g_{k\ell}'$ ) est cohomologue au cocycle $(g_{k\ell})$. Il en résulte une application

$$
c(\varphi ): H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,\mathscr{V},G)
$$

qui à la classe de $(g_{ij})$ associe la classe de $(g_{k\ell})$.

Soit E un espace fibré principal de base B et de groupe G et, pour tout $i\in$ I, soit $f_i: E_{U_i}\rightarrow U_i\times G$ une trivialisation du $U_i$-espace fibré principal $E_{U_i}$. Pour tout $k\in$ K, soit $f_k': E_{V_k}\rightarrow V_k\times G$ la trivialisation déduite de $f_{\varphi(k)}$ par passage aux sous-ensembles. Soit $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ le cocycle défini par la famille $(f_i)$ ; le cocycle défini par la famille $(f_k')$ est précisément le cocycle $(g_{k\ell})$ défini ci-dessus. Ainsi, le diagramme suivant est commutatif :

$$
H^1_{cont}(B,\mathscr{U},G)^{c(\varphi)}H^1_{cont}(B,\mathscr{V},G)
$$

$r_{\mathscr{U}}r_{\mathscr{V}}$

$$
P(B,\mathscr{U},G)^{i_{\mathscr{V} \mathscr{U}}}P(B,\mathscr{V},G)
$$

Les applications $r_{\mathscr{U}}$ et $r_{\mathscr{V}}$ étant bijectives, l’application $c(\varphi )$, de même que $i_{\mathscr{V} \mathscr{U}}$, est une injection et ne dépend pas du choix de $\varphi$. Nous écrirons désormais $c_{\mathscr{V} \mathscr{U}}$ au lieu de $c(\varphi )$.

Soit $\mathscr{R}$ l’ensemble des éléments de $\mathfrak{P}(\mathfrak{P}(B))$ qui sont des recouvrements ouverts de B. Pour tout recouvrement ouvert $\mathscr{U}$ de B, il existe un recouvrement ouvert $\mathscr{V}$ appartenant à $\mathscr{R}$ tel que $\mathscr{U}$ soit à la fois plus fin et moins fin que $\mathscr{U}$. L’ensemble $\mathscr{R}$ est ordonné et filtrant pour la relation $\leqslant$ définie par $\mathscr{U}\leqslant \mathscr{V}$ si $\mathscr{V}$ est un recouvrement plus fin que $\mathscr{U}$. Il résulte de ce qui précède qu’on a défini un système inductif $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ relatif à l’ensemble ordonné filtrant $\mathscr{R}$ et que la famille $(r_{\mathscr{U}})$ est un système inductif d’applications bijectives de $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ dans $(P(B,\mathscr{U},G), i_{\mathscr{V} \mathscr{U}})$. Si l’on note $H^1_{cont}(B,G)$ la limite inductive du système $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ et $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ la limite inductive de la famille $(r_{\mathscr{U}})$, on a donc :

#### Théorème 4 {#ta-i-s5-thm-4 .statement tag=01RQ}

L’application $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ est bijective.

Soit $\mathscr{U}= (U_i)_{i\in I}$ un recouvrement ouvert de B; notons $c_{\mathscr{U}}$ l’application canonique $H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,G)$. Si $(g_{ij})$ est un cocycle sur B, à valeurs dans G, subordonné au recouvrement ouvert $\mathscr{U}$, l’élément $c_{\mathscr{U}}((g_{ij}))$ de $H^1_{cont}(B,G)$ est appelé classe de cohomologie du cocycle $(g_{ij})$.
