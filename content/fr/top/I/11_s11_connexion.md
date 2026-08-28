---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 11
section_title: Connexion
lang: fr
source: top-i-iv-fr
pdf_pages: 0092-0101, 0127-0133
extraction: ocr
subsections:
    - "no": 1
      title: Espaces et ensembles connexes
      page: 80
      pdf_page: 92
    - "no": 2
      title: Image d’un ensemble connexe par une application continue
      page: 82
      pdf_page: 94
    - "no": 3
      title: Espaces quotients d’un espace connexe
      page: 82
      pdf_page: 94
    - "no": 4
      title: Produit d’espaces connexes
      page: 83
      pdf_page: 95
    - "no": 5
      title: Composantes connexes
      page: 83
      pdf_page: 95
    - "no": 6
      title: Espaces localement connexes
      page: 84
      pdf_page: 96
    - "no": 7
      title: 'Application: le théorème de Poincaré-Volterra'
      page: 86
      pdf_page: 98
statements: 28
exercises: 29
content_sha256: e9eff3ed60be295fd962cd027968f4afe1c217f0dc7647c97b8bb23ce797063a
---

## § 11. CONNEXION

### 1. Espaces et ensembles connexes

#### Définition 1 {#top-i-s11-def-1 .statement}

On dit qu’un espace topologique $X$ est connexe s’il n’est pas réunion de deux ensembles ouverts non vides disjoints.

On a une définition équivalente en y remplaçant les mots « ensembles ouverts » par « ensembles fermés »; il revient au même de dire qu’en dehors de l’espace $X$ tout entier et de l’ensemble vide, il n’existe aucun sous-ensemble de $X$ qui soit à la fois ouvert et fermé.

Si $X$ est connexe et si $A$ et $B$ sont deux ensembles ouverts non vides (resp. deux ensembles fermés non vides) tels que $A \cup B = X$, on a $A \cap B \neq \varnothing$.

#### Exemple 1 {#top-i-s11-n1-exa-1 .statement}

On verra dans IV, p. 8 que la droite numérique est connexe, et la droite rationnelle non connexe.*
    2) Un espace discret contenant plus d’un point n’est pas connexe.

On notera que si $(U_\iota)_{\iota \in I}$ est une partition d’un espace topologique $X$ formée d’ensembles ouverts non vides, chacun des $U_\iota$ est à la fois ouvert et fermé, car son complémentaire est ouvert, étant la réunion des $U_\kappa$ pour $\kappa \neq \iota$. Les ensembles ouverts de $X$ sont alors les ensembles $A$ tel que $A \cap U_\iota$ soit ouvert dans $U_\iota$ pour tout $t \in I$, donc $X$ s’identifie à l’espace somme des $U_t$ (I, p. 15, Exemple III), et n’est pas connexe si $I$ a au moins deux éléments.

#### Définition 2 {#top-i-s11-def-2 .statement}

On dit qu’une partie $A$ d’un espace topologique $X$ est un ensemble connexe, si le sous-espace $A$ de $X$ est connexe.

Pour que $A$ soit une partie connexe de $X$, il faut et il suffit que, pour tout recouvrement de $A$ composé de deux ensembles $B, C$, tous deux ouverts (ou tous deux fermés) dans $X$, et tels que $A \cap B$ et $A \cap C$ ne soient pas vides, on ait $A \cap B \cap C \neq \varnothing$.

#### Exemple {#top-i-s11-n1-exa-2 .statement}

Dans un espace topologique, l’ensemble vide et tout ensemble réduit à un point sont connexes; dans un espace séparé, tout ensemble fini comprenant plus d’un point, et plus généralement tout ensemble non réduit à un point et possédant au moins un point isolé est non connexe.

Si un ensemble partout dense $A$ est connexe, l’espace $X$ tout entier est connexe; sinon il existerait deux ensembles ouverts non vides $M, N$ sans point commun tels que $X = M \cup N$; alors $M \cap A$ et $N \cap A$ seraient, dans $A$, deux ensembles ouverts non vides sans point commun, dont la réunion serait $A$, ce qui est contraire à l’hypothèse. D’où:

#### Proposition 1 {#top-i-s11-prop-1 .statement}

Si $A$ est un ensemble connexe, tout ensemble $B$ tel que $A \subset B \subset \overline{A}$ est connexe.

#### Proposition 2 {#top-i-s11-prop-2 .statement}

La réunion d’une famille d’ensembles connexes, dont l’intersection n’est pas vide, est un ensemble connexe.

Soit $(A_t)_{t \in I}$ une famille de parties connexes de $X$, contenant toutes un même point $x$, et montrons que $A = \bigcup_{t \in I} A_t$ est connexe. Sinon, il existerait dans $X$ deux ensembles ouverts $B, C$ tels que $B \cap A$ et $C \cap A$ soient non vides, que $A \subset B \cup C$ et que $A \cap B \cap C = \varnothing$. Le point $x$ appartient à l’un des ensembles $B, C$, soit par exemple $x \in B$; d’autre part il existe un indice $k$ tel que $C \cap A_k \neq \varnothing$; on aurait donc $A_k \subset B \cup C, A_k \cap B \cap C = \varnothing$ et $B \cap A_k$ et $C \cap A_k$ seraient non vides, contrairement à l’hypothèse que les $A_t$ sont connexes.

#### Corollaire {#top-i-s11-n1-cor-1 .statement}

Soit $(A_n)_{n \geq 0}$ une suite infinie d’ensembles connexes tels que $A_{n-1} \cap A_n \neq \varnothing$ pour tout $n \geq 0$; alors la réunion $\bigcup_{n=0}^\infty A_n$ est connexe.

En effet, on voit aussitôt, par récurrence sur $n$, que l’ensemble $B_n = \bigcup_{i=0}^n A_i$ est connexe pour tout $n$, en vertu de la prop. 2; comme les $B_n$ ont une intersection non vide, leur réunion, égale à $\bigcup_{n=0}^\infty A_n$, est connexe en vertu de la prop. 2.

#### Proposition 3 {#top-i-s11-prop-3 .statement}

Soit $A$ une partie d’un espace topologique $X$. Si $B$ est une partie connexe de $X$ qui rencontre à la fois $A$ et $\overline{A}$, $B$ rencontre la frontière de $A$.

En effet, dans le cas contraire, les intersections de B avec l’intérieur et l’extérieur de A seraient deux ensembles non vides ouverts par rapport à B et formant une partition de B, contrairement à l’hypothèse.

#### Corollaire {#top-i-s11-n1-cor-2 .statement}

Dans un espace connexe X, tout ensemble non vide et distinct de X a au moins un point frontière.

### 2. Image d’un ensemble connexe par une application continue

#### Proposition 4 {#top-i-s11-prop-4 .statement}

Soient A une partie connexe d’un espace topologique X, f une application continue de X dans un espace topologique X’ ; alors f(A) est connexe.

En effet, s’il existait deux ensembles M’, N’ non vides ouverts par rapport à f(A) et formant une partition de f(A), $A \cap f^{-1}(M')$ et $A \cap f^{-1}(N')$ seraient non vides, ouverts relativement à A et formeraient une partition de A, contrairement à l’hypothèse.

L’image réciproque d’un ensemble connexe par une application continue n’est pas nécessairement connexe, comme le montre l’exemple d’une application d’un espace discret dans un espace réduit à un seul point.

On déduit de la prop. 4 une nouvelle caractérisation des espaces non connexes :

#### Proposition 5 {#top-i-s11-prop-5 .statement}

Pour qu’un espace topologique X soit non connexe, il faut et il suffit qu’il existe une application continue surjective de X dans un espace discret contenant plus d’un point.

La condition est évidemment suffisante (prop. 4). Elle est nécessaire, car si A, B sont deux ensembles ouverts non vides formant une partition de X, l’application f de X sur un espace discret {a, b} à deux éléments telle que $f(A) = \{a\}$ et $f(B) = \{b\}$, est continue dans X.

### 3. Espaces quotients d’un espace connexe

#### Proposition 6 {#top-i-s11-prop-6 .statement}

Tout espace quotient d’un espace connexe est connexe.

C’est une conséquence immédiate de la prop. 4.

#### Proposition 7 {#top-i-s11-prop-7 .statement}

Soient X un espace topologique, R une relation d’équivalence dans X. Si l’espace quotient X/R est connexe, et si chaque classe d’équivalence suivant R est connexe, alors X est connexe.

Raisonnons par l’absurde, et supposons qu’il existe une partition de X en deux ensembles ouverts non vides A, B. Les ensembles A, B sont saturés pour R : en effet, si $x \in A$, la classe M de x suivant R ne peut rencontrer B, sans quoi les ensembles $A \cap M$ et $B \cap M$ formeraient une partition de M en deux ensembles non vides ouverts par rapport à M, ce qui est contraire à l’hypothèse. Les images canoniques de A et B sont alors des ensembles non vides ouverts dans X/R, formant une partition de X/R, ce qui est absurde.

### 4. Produit d’espaces connexes

#### Proposition 8 {#top-i-s11-prop-8 .statement}

Tout produit d’espaces connexes est connexe. Réciproquement, si un produit d’espaces non vides est connexe, chacun des espaces facteurs est connexe.

Soit $X = \prod_{i \in I} X_i$ un produit d’espaces topologiques. Si les $X_i$ sont non vides, on a $X_i = \operatorname{pr}_i X$ pour tout $i \in I$, donc si $X$ est connexe il en est de même des $X_i$ (I, p. 82, prop. 4). Inversement, supposons tous les $X_i$ connexes, et $X$ non connexe. En vertu de la prop. 5 (I, p. 82), il existerait alors une application surjective continue $f : X \to X'$, où $X'$ est un espace discret comprenant plus d’un point. Soit $a = (a_i)$ un point quelconque de $X$, $\kappa$ un indice quelconque ; l’application partielle $f_\kappa : X_\kappa \to X'$, définie par $f_\kappa(x) = f((y_i))$ avec $y_\kappa = x$ et $y_i = a_i$ pour $i \neq \kappa$, est continue dans $X_\kappa$; comme $X_\kappa$ est connexe, $f_\kappa$ est constante dans $X_\kappa$. Ce résultat prouve aussitôt par récurrence que $f(x) = f(a)$ pour tout point $x = (x_i)$ tel que $x_i = a_i$ sauf pour un nombre fini d’indices. Mais ces points forment une partie partout dense de $X$ (I, p. 28, prop. 8); comme $f$ est continue dans $X$ et constante dans une partie partout dense de $X$, $f$ est constante dans $X$ (I, p. 53, cor. 1), contrairement à l’hypothèse.

### 5. Composantes connexes

Étant donné un point $x$ d’un espace topologique $X$, la réunion des parties connexes de $X$ contenant $x$ est encore un ensemble connexe (I, p. 81, prop. 2); c’est donc la plus grande partie connexe de $X$ contenant $x$.

#### Définition 3 {#top-i-s11-def-3 .statement}

On appelle composante connexe d’un point d’un espace $X$ la plus grande partie connexe de $X$ contenant ce point. On appelle composantes connexes d’une partie $A$ de $X$ les composantes connexes des points de $A$, relativement au sous-espace $A$ de $X$.

Lorsqu’un espace est connexe, il est identique à la composante connexe de chacun de ses points. Si, pour tout couple $(x, y)$ de points d’un espace topologique $X$, il existe un ensemble connexe contenant $x$ et $y$, $X$ est connexe.

On dit qu’un espace $X$ est totalement discontinu lorsque la composante connexe de chacun de ses points est l’ensemble réduit à ce point. On dit qu’une partie $A$ de $X$ est un ensemble totalement discontinu si le sous-espace $A$ de $X$ est totalement discontinu.

Un espace discret est totalement discontinu, mais il faut prendre garde de ne pas confondre ces deux notions : nous verrons par exemple dans IV, p. 8, que la droite rationnelle, qui n’est pas un espace discret, est totalement discontinue.

Remarquons encore qu’un ensemble à la fois ouvert et fermé contient la composante connexe de chacun de ses points : on peut aussi exprimer cela en disant que la composante connexe d’un point est contenue dans l’intersection des ensembles à la fois ouverts et fermés contenant ce point. Elle n’est d’ailleurs pas nécessairement identique à cette intersection (cf. I, p. 115, exerc. 9 et II, p. 32, prop. 6).

#### Proposition 9 {#top-i-s11-prop-9 .statement}

Dans un espace topologique $X$, la composante connexe d’un point quelconque est un ensemble fermé. La relation « $y$ appartient à la composante connexe de $x$ » est une relation d’équivalence $R \{ x, y \}$ dans $X$, dont les classes d’équivalence sont les composantes connexes de $X$; l’espace quotient $X/R$ est totalement discontinu.

La première partie de la proposition est une conséquence immédiate de la déf. 3 et du fait que l’adhérence d’un ensemble connexe est connexe (I, p. 81, prop. 1). Comme la réunion d’ensembles connexes ayant un point commun est connexe (I, p. 81, prop. 2), la relation $R$ est transitive, donc est une relation d’équivalence (puisqu’elle est évidemment réflexive et symétrique) et la classe de $x$ suivant $R$ est la composante connexe de $x$. Reste à voir que $X/R$ est totalement discontinu. Soit $f$ l’application canonique $X \to X/R$, et soit $F$ un ensemble fermé dans $X/R$ contenant deux points distincts au moins; son image réciproque $\overline{f}(F)$ est fermée dans $X$, saturée pour $R$ et contient au moins deux composantes connexes distinctes de $X$, donc est non connexe. Il existe par suite deux ensembles non vides, $B, C$ fermés dans $X$, tels que $B \cap C = \varnothing$ et $B \cup C = \overline{f}(F)$. Comme la composante connexe $\overline{f}(F)$ d’un point quelconque de cet ensemble est identique à la composante connexe de ce point dans $X$ (par définition de $R$), $B$ et $C$, qui sont à la fois ouverts et fermés $\overline{f}(F)$, sont saturés pour $R$; $f(B)$ et $f(C)$ sont donc fermés dans $X/R$ et l’on a $f(B) \cup f(C) = F$ et $f(B) \cap f(C) = \varnothing$, ce qui prouve que $F$ est non connexe, et par suite que $X/R$ est totalement discontinu.

#### Proposition 10 {#top-i-s11-prop-10 .statement}

Dans un espace produit $X = \prod_{t \in I} X_t$, la composante connexe d’un point $x = (x_t)$ est le produit des composantes connexes des points $x_t$ dans les espaces facteurs $X_t$.

En effet, cet ensemble produit est connexe (I, p. 83, prop. 8). D’autre part, si une partie connexe $A$ de $X$ contient $x$, $\mathrm{pr}_t(A)$ est un ensemble connexe (I, p. 82, prop. 4) contenant $x_t$; comme $A \subset \prod_t \mathrm{pr}_t(A)$, $A$ est contenu dans le produit des composantes connexes des $x_t$.

### 6. Espaces localement connexes

#### Définition 4 {#top-i-s11-def-4 .statement}

On dit qu’un espace topologique $X$ est localement connexe si tout point de $X$ possède un système fondamental de voisinages connexes.

*On verra dans IV, p. 8, que la droite numérique est un espace localement connexe.*

L’existence, en tout point $x$ d’un espace $X$, d’un voisinage connexe de $x$, n’entraîne nullement que $X$ soit localement connexe. En particulier, $X$ peut être connexe mais non localement connexe (I, p. 114, exerc. 2 et I, p. 115, exerc. 13). Inversement, un espace peut être localement connexe mais non connexe: un espace discret ayant plus d’un point donne un exemple de ce fait.

#### Proposition 11 {#top-i-s11-prop-11 .statement}

Pour qu’un espace X soit localement connexe, il faut et il suffit que toute composante connexe d’un ensemble ouvert dans X soit un ensemble ouvert dans X.

La condition est évidemment suffisante, car la composante connexe d’un point x relativement à un voisinage ouvert de x dans X est alors un voisinage de x dans X.

La condition est nécessaire : soient en effet A un ensemble ouvert dans un espace localement connexe X, B une composante connexe de A, x un point de B. Soit V un voisinage connexe de x contenu dans A ; par définition des composantes connexes (I, p. 83, déf. 3), V est contenu dans B, ce qui prouve que B est ouvert dans X (I, p. 2, prop. 1).

Les composantes connexes d’un espace localement connexe X constituent donc une partition de X formée d’ensembles ouverts dans X ; X est donc l’espace somme (I, p. 15, Exemple III) de ses composantes connexes (I, p. 81).

#### Corollaire {#top-i-s11-n6-cor-1 .statement}

Soient U un ensemble ouvert dans un espace localement connexe X, V une composante connexe de U ; la frontière de V (relativement à X) est alors contenue dans la frontière de U.

En effet, V est ouvert et fermé dans U en vertu de la remarque précédente ; un point frontière de V relativement à X ne peut donc appartenir à U.

#### Proposition 12 {#top-i-s11-prop-12 .statement}

Tout espace quotient d’un espace localement connexe est localement connexe.

Soient X un espace localement connexe, R une relation d’équivalence dans X, φ l’application canonique X → X/R. Soient A une partie ouverte de X/R, C une composante connexe de A ; montrons que $\overline{\varphi}(C)$ est réunion de composantes connexes de $\overline{\varphi}(A)$. En effet, si $x \in \overline{\varphi}(C)$, et si K est la composante connexe de x par rapport à $\overline{\varphi}(A)$, $\varphi(K)$ est connexe (I, p. 82, prop. 4), contenu dans A, et contient $\varphi(x)$, donc $\varphi(K) \subset C$ par définition, et par suite $K \subset \overline{\varphi}(C)$. Comme X est localement connexe et $\overline{\varphi}(A)$ ouvert dans X, $\overline{\varphi}(C)$ est ouvert dans X (prop. 11) et par suite C est ouvert dans X/R, ce qui démontre la proposition, en vertu de la prop. 11.

#### Proposition 13 {#top-i-s11-prop-13 .statement}

a) Soit $(X_i)_{i \in I}$ une famille d’espaces localement connexes, telle que $X_i$ soit connexe sauf pour un nombre fini d’indices. Alors l’espace produit $X = \prod_{i \in I} X_i$ est localement connexe.

b) Réciproquement, si le produit d’une famille $(X_i)$ d’espaces topologiques non vides est localement connexe, tous les $X_i$ sont localement connexes, et ils sont connexes sauf pour un nombre fini d’indices.

a) Soit J la partie finie de I telle que, pour $i \in J$, $X_i$ ne soit pas connexe. Soit $U = \prod_i U_i$ un ensemble élémentaire contenant un point $x = (x_i)$ de X, et soit K la partie finie de I telle que, pour $i \in K, U_i \neq X_i$. Si on prend $V_i = X_i$ pour $i \notin J \cup K$ et $V_i$ égal à un voisinage connexe de $x_i$ contenu dans $U_i$ pour $i \in J \cup K$, $V = \prod_i V_i$ est, en vertu de I, p. 83, prop. 8, un voisinage connexe de $x$ contenu dans $U$, ce qui prouve a).

b) Soit $a = (a_i)$ un point de $X$ et soit $V$ un voisinage connexe de $a$ dans $X$; comme on a $\mathrm{pr}_i V = X_i$ sauf pour un nombre fini d’indices (I, p. 24), il résulte de I, p. 82, prop. 4 que les $X_i$ sont connexes sauf pour un nombre fini d’indices. D’autre part, pour tout $\kappa \in I$, tout $a_\kappa \in X_\kappa$ et tout voisinage $V_\kappa$ de $a_\kappa$ dans $X_\kappa$, il existe un $x \in X$ tel que $\mathrm{pr}_\kappa x = a_\kappa$ et $V = V_\kappa \times \prod_{i \neq \kappa} X_i$ est un voisinage de $x$; donc $V$ contient un voisinage connexe $W$ de $x$, dont la projection $\mathrm{pr}_\kappa W$ est un voisinage connexe de $a_\kappa$ contenu dans $V_\kappa$ (I, p. 82, prop. 4 et I, p. 26, prop. 5), ce qui montre que $X_\kappa$ est localement connexe.

### 7. Application: le théorème de Poincaré-Volterra

#### Théorème 1 {#top-i-s11-thm-1 .statement}

Soit $X$ un espace topologique satisfaisant à l’axiome $(\mathbf{O}_{III})$ (mais non nécessairement séparé), connexe et localement connexe. Soit $Y$ un espace topologique dont la topologie admet une base dénombrable, et soit $p : X \to Y$ une application continue telle que, pour tout $y \in Y$, $p^{-1}(y)$ soit un sous-espace discret de $X$. Soit enfin $\mathcal{V}$ un ensemble de parties de $X$ dont les intérieurs forment un recouvrement de $X$, et tel en outre que:
1° La restriction de $p$ à toute partie $V \in \mathcal{V}$ est une application fermée de $V$ dans $Y$.
2° Tout ensemble $V \in \mathcal{V}$ contient une partie dénombrable dense dans $V$.
Alors l’espace $X$ est réunion d’une famille dénombrable d’ensembles ouverts dont chacun est contenu dans un ensemble de $\mathcal{V}$.

Soit $\mathcal{B}$ une base dénombrable de la topologie de $Y$. Nous dirons qu’un couple $(W, U)$ est un couple distingué si: 1° $U \in \mathcal{B}$; 2° $W$ est une composante connexe de $p^{-1}(U)$ contenue dans un ensemble de $\mathcal{V}$.

#### Lemme 1 {#top-i-s11-lem-1 .statement}

Pour tout point $x \in X$, il existe un couple distingué $(W, U)$ tel que $x \in W$.

En effet, l’image réciproque $p(p(x))$ étant discrète, il existe dans $X$ un voisinage de $x$ dont tous les points $x' \neq x$ ont une image $p(x') \neq p(x)$; comme $X$ vérifie $(\mathbf{O}_{III})$, il existe un voisinage fermé $V$ de $x$ ayant la même propriété, et on peut évidemment supposer en outre que $V$ est contenu dans un ensemble de $\mathcal{V}$.

Soit $F$ la frontière de $V$ dans $X$; en vertu de la condition 1° de l’énoncé, $p(F)$ est fermé dans $Y$ et comme $p(F)$ ne contient pas $p(x)$, il existe un ensemble $U \in \mathcal{B}$ qui contient $p(x)$ et ne rencontre pas $p(F)$. Soit alors $W$ la composante connexe de $p^{-1}(U)$ qui contient $x$; il suffit de prouver que l’on a $W \subset V$; dans le cas contraire, $W$ rencontrerait $F$ (I, p. 81, prop. 3) et par suite $p(F)$ rencontrerait $U$, contrairement à la définition de $U$.

#### Lemme 2 {#top-i-s11-lem-2 .statement}

Étant donné un couple distingué (W, U), l’ensemble des couples distingués (W', U') tels que W ∩ W' ≠ ∅ est dénombrable.

En effet, $\mathfrak{B}$ étant dénombrable, il suffit de prouver que, pour un $U' \in \mathfrak{B}$ donné, l’ensemble des couples distingués (W', U') tels que W' rencontre W est dénombrable. Or, ces ensembles W' sont ouverts, puisque X est localement connexe (I, p. 85, prop. 11) et deux à deux disjoints, par définition des composantes connexes de $p^{-1}(U')$; il en est de même des ensembles $W' \cap W$; mais comme W contient un ensemble dénombrable dense dans W, l’ensemble des W' tels que $W' \cap W$ soit non vide est nécessairement dénombrable.

Ces lemmes étant établis, considérons dans X la relation suivante R entre deux points x, x':

« il existe une suite finie de couples distingués $(W_i, U_i)$ $(1 \leq i \leq n)$ tels que $x \in W_1,\ x' \in W_n$ et $W_i \cap W_{i+1} \neq \emptyset$ pour $1 \leq i \leq n - 1$. »

La relation R est réflexive en vertu du lemme 1, et on vérifie aussitôt qu’elle est symétrique et transitive; en outre, il résulte de la définition de R et du fait que les $W_i$ sont ouverts, que toute classe d’équivalence suivant R est un ensemble ouvert; comme X est connexe, deux points quelconques de X sont donc équivalents mod. R (I, p. 80). Nous allons en déduire que X est réunion d’une famille dénombrable de premiers éléments de couples distingués, ce qui achèvera de démontrer le th. 1. Or, soit x un point de X; définissons par récurrence sur n une suite $(C_n)$ d’ensembles ouverts dans X, de la façon suivante: en vertu du lemme 1, il existe un couple distingué $(W_1, U_1)$ tel que $x \in W_1$; on prendra $C_1 = W_1$; puis, pour $n > 1$, $C_n$ sera la réunion de tous les premiers éléments W des couples distingués $(W, U)$ tels que W rencontre $C_{n-1}$. On prouve aussitôt, par récurrence sur n, et en appliquant le lemme 2, que $C_n$ est réunion dénombrable de premiers éléments de couples distingués. Montrons enfin que tout point $x' \in X$ appartient à l’un des $C_n$: il existe en effet une suite finie $(W'_i, U'_i)_{1 \leq i \leq m}$ de couples distingués tels que $x \in W'_1,\ x' \in W'_m$ et $W'_i \cap W'_{i+1} \neq \emptyset$ pour $1 \leq i \leq m - 1$; par récurrence sur i, on voit que $W'_i \subset C_{i+1}$ pour tout i, et par suite $x' \in C_{m+1}$.

C.Q.F.D.

#### Corollaire 1 {#top-i-s11-lem-2-cor-1 .statement}

Soit Y un espace régulier dont la topologie possède une base dénombrable.$^1$ Soit X un espace connexe et localement connexe, et soit $p : X \to Y$ une application continue ayant la propriété suivante: pour tout point x de X, il existe un voisinage fermé V de x dans X tel que la restriction de p à V soit un homéomorphisme de V sur un sous-espace fermé de Y. Alors X est un espace régulier dont la topologie possède une base dénombrable.

Les hypothèses entraînent en premier lieu que X est régulier (I, p. 57, prop. 13). Montrons en outre que les hypothèses du th. 1 sont vérifiées en prenant pour $\mathfrak{B}$ l’ensemble des parties fermées V de X, telles que la restriction de $p$ à V soit un

1 *On peut montrer que ces conditions entraînent que la topologie de Y est métrisable (IX, §4, exerc. 29).*

homéomorphisme de $V$ sur un sous-espace fermé de $Y$. Par hypothèse, les intérieurs des ensembles de $\mathfrak{V}$ recouvrent $X$ et, en vertu de l’hypothèse sur $Y$, tout $V \in \mathfrak{V}$ possède une base dénombrable, donc contient une partie dénombrable partout dense (I, p. 8, prop. 6). Reste enfin à voir que pour tout $y \in Y$, le sous-espace $p^{-1}(y)$ de $X$ est discret: or, par hypothèse, pour tout $x \in p^{-1}(y)$, il existe un voisinage $V \in \mathfrak{V}$ de $x$ dans $X$ tel que $V$ ne contienne aucun point de $p(y)$ distinct de $x$, d’où notre assertion. Le th.1 montre donc que $X$ est réunion d’une famille dénombrable $(T_n)_{n \geq 0}$ d’ensembles ouverts, chacun des sous-espaces $T_n$ ayant une base dénombrable $(U_{mn})_{m \geq 0}$. Alors les $U_{mn}$ ($m \geq 0, n \geq 0$) forment une base de la topologie de $X$ (I, p. 19, Remarque).

#### Corollaire 2 {#top-i-s11-lem-2-cor-2 .statement}

*Soit $X$ un espace localement compact, connexe et localement connexe, dont chaque point admet un voisinage ayant une base dénombrable. Soit $Y$ un espace séparé, dont la topologie admet une base dénombrable, et soit $p : X \to Y$ une application continue telle que, pour tout $y \in Y$, $p^{-1}(y)$ soit un sous-espace discret de $X$. Alors la topologie de $X$ admet une base dénombrable.*

Pour tout $x \in X$, soit $V_x$ un voisinage compact de $x$ dans $X$ admettant une base dénombrable; il résulte de I, p. 63, cor. 2, que l’ensemble $\mathfrak{V}$ des $V_x$ vérifie les conditions du th. 1 ; on conclut comme dans le cor. 1.

On notera que, dans ce corollaire, il peut se faire que la restriction de $p$ à un voisinage arbitrairement petit $V$ d’un point de $X$ *ne soit pas un homéomorphisme de $V$ sur $p(V)$*.

#### Corollaire 3 (théorème de Poincaré–Volterra) {#top-i-s11-lem-2-cor-3 .statement}

*Soit $Y$ un espace localement compact, localement connexe et dont la topologie admet une base dénombrable. Soit $X$ un espace séparé et connexe, et soit $p : X \to Y$ une application continue ayant la propriété suivante: pour tout point $x \in X$ il existe un voisinage ouvert $U$ de $x$ dans $X$ tel que la restriction de $p$ à $U$ soit un homéomorphisme de $U$ sur un sous-espace ouvert de $Y$. Alors $X$ est localement compact, localement connexe et sa topologie admet une base dénombrable.*

Il est évident que $X$ est localement connexe; d’autre part, tout point $x \in X$ possède un voisinage ouvert $U$ dans $X$, tel que la restriction de $p$ à $U$ soit un homéomorphisme de $U$ sur un sous-espace ouvert $p(U)$ de $Y$. Comme $p(U)$ est un sous-espace localement compact de $Y$ (I, p. 66, prop. 13), il existe un voisinage compact $W$ de $p(x)$ contenu dans $p(U)$ et $U \cap p^{-1}(W)$ est donc un voisinage compact de $x$ contenu dans $U$. Comme $X$ est séparé, il est donc localement compact; en outre $U \cap p^{-1}(W)$, étant compact, est fermé dans $X$ (I, p. 62, prop. 4) et les hypothèses du cor. 1 sont par suite satisfaites; donc la topologie de $X$ admet une base dénombrable.

Exercices

## EXERCICES {#top-i-s11-exercises}

See the [exercises for § 11](exercises/s11/).
