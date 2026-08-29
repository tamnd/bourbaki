---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 5
section_title: Applications ouvertes et applications fermées
lang: fr
source: top-i-iv-fr
book_pages: TG I.30-TG I.35, TG I.96
pdf_pages: 0042-0047, 0108-0108
extraction: ocr
subsections:
    - "no": 1
      title: Applications ouvertes et applications fermées
      page: 30
      pdf_page: 42
    - "no": 2
      title: Relations d’équivalence ouvertes et relations d’équivalence fermées
      page: 31
      pdf_page: 43
    - "no": 3
      title: Propriétés spéciales aux applications ouvertes
      page: 33
      pdf_page: 45
    - "no": 4
      title: Propriétés spéciales aux applications fermées
      page: 35
      pdf_page: 47
statements: 25
exercises: 7
content_sha256: 4020d4a2dd332ee47e49fa05c38fcf9c87134c29dfa27ba1909ac716e5aa3558
---

## § 5. APPLICATIONS OUVERTES ET APPLICATIONS FERMÉES

### 1. Applications ouvertes et applications fermées

#### Définition 1 {#top-i-s5-def-1 .statement}

Soient $X, X'$ deux espaces topologiques. On dit qu'une application $f : X \to X'$ est ouverte (resp. fermée) si l'image par $f$ de toute partie ouverte (resp. fermée) de $X$ est ouverte (resp. fermée) dans $X'$.

En particulier, $f(X)$ est alors une partie ouverte (resp. fermée) de $X'$.

#### Exemple 1 {#top-i-s5-n1-exa-1 .statement}

Soit $A$ un sous-espace d'un espace topologique $X$; pour que l'injection canonique $j : A \to X$ soit ouverte (resp. fermée), il faut et il suffit que $A$ soit ouvert (resp. fermé) dans $X$ (I, p. 18).

#### Exemple 2 {#top-i-s5-n1-exa-2 .statement}

Pour qu'une bijection $f$ d'un espace topologique $X$ sur un espace topologique $X'$ soit un homéomorphisme, il faut et il suffit que $f$ soit continue et ouverte, ou continue et fermée.

#### Exemple 3 {#top-i-s5-n1-exa-3 .statement}

Soit $f$ une surjection d'un ensemble $X$ dans un espace topologique $X'$; si on munit $X$ de la topologie image réciproque de celle de $X'$ par $f$ (I, p. 13, Exemple I), $f$ est une application continue à la fois ouverte et fermée de $X$ dans $X'$.

#### Exemple 4 {#top-i-s5-n1-exa-4 .statement}

Dans un espace produit $X = \prod_{i \in I} X_i$, toute projection $\mathrm{pr}_i : X \to X_i$ est une application continue ouverte, mais non nécessairement fermée (I, p. 26, prop. 5).

#### Exemple 5 {#top-i-s5-n1-exa-5 .statement}

Une fonction holomorphe non constante $f$, définie dans une partie ouverte connexe $A$ de $\mathbf{C}$, est une application ouverte de $A$ dans $\mathbf{C}$.*

#### Exemple 6 {#top-i-s5-n1-exa-6 .statement}

Soient $X, X'$ deux espaces topologiques, $f$ une bijection continue de $X$ sur $X'$, qui n'est pas bicontinue; alors la bijection réciproque $g : X' \to X$ est une application ouverte et fermée de $X'$ sur $X$, qui n'est pas continue.

#### Proposition 1 {#top-i-s5-prop-1 .statement}

Soient $X, X', X''$ trois espaces topologiques, $f : X \to X', g : X' \to X''$ deux applications. Alors :
a) Si $f$ et $g$ sont ouvertes (resp. fermées), $g \circ f$ est ouverte (resp. fermée).
b) Si $g \circ f$ est ouverte (resp. fermée) et si $f$ est surjective et continue, $g$ est ouverte (resp. fermée).
c) Si $g \circ f$ est ouverte (resp. fermée) et si $g$ est injective et continue, $f$ est ouverte (resp. fermée).

L'assertion a) résulte aussitôt de la déf. 1. Pour démontrer b), il suffit de remarquer que toute partie ouverte (resp. fermée) $A'$ de $X'$ s'écrit $A' = f(A)$, où $A = f^{-1}(A')$ est ouvert (resp. fermé) dans $X$ (I, p. 9, th. 1); donc $g(A') = g(f(A))$ est ouvert (resp. fermé) dans $X''$. Enfin, pour prouver c), on remarque que pour toute partie $A$ de $X$, on a $f(A) = g^{-1}(g(f(A)))$; par hypothèse, si $A$ est ouvert (resp. fermé) dans $X$, $g(f(A))$ est ouvert (resp. fermé) dans $X''$, donc $f(A)$ est ouvert (resp. fermé) dans $X'$ en vertu de I, p. 9, th. 1.

#### Proposition 2 {#top-i-s5-prop-2 .statement}

Soient $X, Y$ deux espaces topologiques, $f$ une application de $X$ dans $Y$.

Pour toute partie T de Y, désignons par $f_T$ l’application de $f^{-1}(T)$ dans T qui coïncide avec $f$ dans $f^{-1}(T)$.

a) Si $f$ est ouverte (resp. fermée), $f_T$ est ouverte (resp. fermée).

b) Soit $(T(\iota))_{\iota \in I}$ une famille de parties de Y dont les intérieurs forment un recouvrement de Y, ou qui est un recouvrement fermé localement fini de Y ; si toutes les $f_{T(\iota)}$ sont ouvertes (resp. fermées), alors $f$ est ouverte (resp. fermée).

a) Si A est une partie ouverte (resp. fermée) de $f^{-1}(T)$, il existe une partie ouverte (resp. fermée) B de X telle que $A = B \cap f^{-1}(T)$; on a alors $f_T(A) = f(B) \cap T$; par hypothèse $f(B)$ est ouvert (resp. fermé) dans Y, donc $f_T(A)$ est ouvert (resp. fermé) dans T.

b) Soit B une partie ouverte (resp. fermée) de X, et soit $B_\iota = B \cap f^{-1}(T(\iota))$; on a $f(B) \cap T(\iota) = f_{T(\iota)}(B_\iota)$; comme $f_{T(\iota)}(B_\iota)$ est ouvert (resp. fermé) dans $T(\iota)$ par hypothèse, $f(B)$ est ouvert (resp. fermé) dans Y en vertu de la prop. 3 de I, p. 18.

#### Corollaire {#top-i-s5-n1-cor-1 .statement}

Soit $(T(\iota))_{\iota \in I}$ une famille de parties de Y dont les intérieurs forment un recouvrement de Y, ou qui est un recouvrement fermé localement fini de Y. Si $f : X \to Y$ est continue et si chacune des $f_{T(\iota)}$ est un homéomorphisme de $f^{-1}(T(\iota))$ sur $T(\iota)$, $f$ est un homéomorphisme de X sur Y.

Il est clair en effet que $f$ est bijective, et elle est ouverte en vertu de la prop. 2.

### 2. Relations d’équivalence ouvertes et relations d’équivalence fermées

#### Définition 2 {#top-i-s5-def-2 .statement}

On dit qu’une relation d’équivalence R dans un espace topologique X est ouverte (resp. fermée) si l’application canonique de X sur $X/R$ est ouverte (resp. fermée).

Il revient au même de dire que le saturé pour R de toute partie ouverte (resp. fermée) de X est un ensemble ouvert (resp. fermé) dans X (I, p. 21).

#### Exemple 1 {#top-i-s5-n2-exa-1 .statement}

Soient X un espace topologique, Γ un groupe d’homéomorphismes de X sur lui-même, R la relation d’équivalence

« il existe $\sigma \in \Gamma$ tel que $y = \sigma(x)$ »

entre x et y (autrement dit, la relation d’équivalence dont les classes sont les orbites de Γ dans X ; cf. A, I, p. 54). Montrons que la relation R est ouverte : en effet, le saturé d’un ensemble $A \subset X$ pour R est la réunion des images $\sigma(A)$, où $\sigma$ parcourt $\Gamma$ ; si A est ouvert, il en est de même des $\sigma(A)$ et par suite de leur réunion.

*Sur la droite numérique $\mathbf{R}$, la relation d’équivalence $x \equiv y$ (mod. 1) est ouverte, car elle est définie de la manière précédente à partir du groupe des translations $x \mapsto x + n \ (n \in \mathbf{Z})$ (voir III, p. 10).*

#### Exemple 2 {#top-i-s5-n2-exa-2 .statement}

Soit X un espace somme d’une famille $(X_\iota)$ de sous-espaces de X, et soit $X/R$ l’espace obtenu par recollement des $X_\iota$ le long d’ensembles ouverts $A_{\iota k}$ au moyen de bijections $h_{k\ell}$ (I, p. 16); nous supposerons que $h_{k\ell}$ soit un homéomorphisme de $A_{t\kappa}$ sur $A_{k\ell}$ pour tout couple d’indices. Dans ces conditions, la relation R est ouverte. En effet, si U est ouvert dans X, le saturé de U est la réunion des $h_{k\ell}(U \cap A_{t\kappa})$; comme $U \cap A_{t\kappa}$ est ouvert dans $A_{t\kappa}$, $h_{k\ell}(U \cap A_{t\kappa})$ est ouvert dans $A_{k\ell}$, donc dans X, d’où notre assertion.

#### Exemple 3 {#top-i-s5-n2-exa-3 .statement}

Avec les notations de l’Exemple 2), supposons maintenant que les $A_{t\kappa}$ soient fermés et que les $h_{k\ell}$ soient des homéomorphismes; en outre, nous supposerons que, pour tout indice $t$, il n’existe qu’un nombre fini d’indices $\kappa$ tels que $A_{t\kappa} \neq \varnothing$ (en termes imagés, chaque $X_t$ n’est « recollé » qu’à un nombre fini de $X_\kappa$). Dans ces conditions, la relation R est fermée. En effet, pour tout ensemble fermé F dans X, le saturé de F est la réunion des $h_{k\ell}(F \cap A_{t\kappa}) \subset A_{k\ell}$; or l’hypothèse entraîne que cette famille est localement finie et d’autre part $h_{k\ell}(F \cap A_{t\kappa})$ est fermé dans $A_{k\ell}$, donc dans X. Notre conclusion résulte alors de la prop. 4 de I, p. 6.

#### Proposition 3 {#top-i-s5-prop-3 .statement}

Soient X, Y deux espaces topologiques, $f : X \to Y$ une application continue, R la relation d’équivalence $f(x) = f(y)$ dans X, $X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y$ la décomposition canonique de f. Les trois propriétés suivantes sont équivalentes:
a) $f$ est une application ouverte.
b) Les trois applications $p, h, i$ sont ouvertes.
c) La relation d’équivalence R est ouverte, h est un homéomorphisme et $f(X)$ est une partie ouverte de Y.

En outre, ce qui précède reste vrai lorsqu’on y remplace partout « ouverte » par « fermée ».
Comme l’injection i est continue, il résulte de la prop. 1 c) de I, p. 30 que si $f$ est ouverte, il en est de même de $h \circ p$; comme $p$ est surjective et continue, la prop. 1 b) de I, p. 30 montre alors que $h$ est ouverte, et comme $h$ est une bijection continue, c’est un homéomorphisme; on en conclut (I, p. 30, prop. 1 a)) que $p^{-1} = h \circ (h \circ p)$ est ouverte. D’autre part (I, p. 30, prop. 1 b)), $i \circ h$ est ouverte, donc (I, p. 30, prop. 1 a)) il en est de même de $i = (i \circ h) \circ h^{-1}$. Ceci prouve que a) entraîne b). Inversement, b) entraîne a) en vertu de la prop. 1 a) de I, p. 30. Enfin, l’équivalence de b) et c) résulte aussitôt des définitions.

La démonstration est analogue, mutatis mutandis, lorsqu’il s’agit d’applications fermées.

#### Proposition 4 {#top-i-s5-prop-4 .statement}

Soient R une relation d’équivalence ouverte (resp. fermée) dans un espace topologique X, f l’application canonique $X \to X/R$, A une partie de X. Supposons que l’une des deux conditions suivantes soit vérifiée:
a) A est ouvert (resp. fermé) dans X.
b) A est saturé pour R.

Dans ces conditions, la relation $R_A$ induite sur A est ouverte (resp. fermée) et l’application canonique de $A/R_A$ sur $f(A)$ est un homéomorphisme.

Considérons le diagramme commutatif (1) de I, p. 23, donnant la décomposition canonique de $f \circ j$. Dans l’hypothèse a), $j$ est ouverte (resp. fermée) et il en est de même de $f$ par hypothèse, donc $f \circ j$ est ouverte (resp. fermée) (I, p. 30, prop. 1 a)), et la conclusion résulte de la prop. 3. Dans l’hypothèse b), on a

A = \overline{f}^{-1}(f(A)), et h \circ \varphi est l’application de A dans f(A) coïncidant avec f dans A; en vertu de la prop. 2 a) de I, p. 31, h \circ \varphi est ouverte (resp. fermée), et la conclusion résulte encore de la prop. 3 appliquée à h \circ \varphi.

### 3. Propriétés spéciales aux applications ouvertes

#### Proposition 5 {#top-i-s5-prop-5 .statement}

Soient X, Y deux espaces topologiques, f une application de X dans Y, $\mathcal{B}$ une base de la topologie de X. Les propriétés suivantes sont équivalentes:
a) f est une application ouverte.
b) Pour tout $U \in \mathcal{B}, f(U)$ est ouvert dans Y.
c) Pour tout $x \in X$ et tout voisinage V de x dans X, $f(V)$ est un voisinage de $f(x)$ dans Y.
L’équivalence de a) et b) résulte aussitôt des définitions et de (O_1); l’équivalence de a) et c) résulte de la prop. 1 de I, p. 2.

#### Proposition 6 {#top-i-s5-prop-6 .statement}

Soit R une relation d’équivalence dans un espace topologique X. Les trois conditions suivantes sont équivalentes:
a) La relation R est ouverte.
b) L’intérieur de tout ensemble saturé pour R est saturé pour R.
c) L’adhérence de tout ensemble saturé pour R est saturé pour R.
Par passage aux complémentaires (I, p. 7, formules (2)), il est évident que b) et c) sont équivalentes. Montrons que b) entraîne a): supposons b) vérifiée et soient U une partie ouverte de X, V son saturé pour R; on a $\dot{V} \supset U$ et comme par hypothèse $\dot{V}$ est saturé, on a $\dot{V} = V$ et le saturé de U est ouvert. Inversement, montrons que a) implique b); supposons a) vérifiée, et soit A un ensemble saturé pour R; si B est le saturé de $\dot{A}$, on a $\dot{A} \subset B \subset A$, et comme B est ouvert par hypothèse, $B = \dot{A}$.

#### Proposition 7 {#top-i-s5-prop-7 .statement}

Soient R une relation d’équivalence dans un espace topologique X, $\varphi$ l’application canonique $X \to X/R$. Si R est ouverte:
(i) Pour tout ensemble $A \subset X$ saturé pour R, l’adhérence (resp. l’intérieur) de $\varphi(A)$ dans $X/R$ est $\varphi(\overline{A})$ (resp. $\varphi(\dot{A})$).
(ii) Pour toute partie C de $X/R$, on a $\overline{\varphi^{-1}(\overline{C})} = \overline{\varphi^{-1}(C)}$.
Inversement, chacune de ces propriétés implique que R est ouverte.
(ii) se déduit de (i), car si $A = \overline{\varphi^{-1}(C)}$, A est saturé pour R, donc aussi $\overline{A}$ (prop. 6), et $\varphi(\overline{A}) = \overline{C}$, d’où $\overline{A} = \overline{\varphi^{-1}(\overline{C})}$. Pour prouver les deux assertions de (i), notons qu’elles se déduisent l’une de l’autre par passage aux complémentaires, en utilisant les formules (2) de I, p. 7, et le fait que si B est une partie saturée de X, on a $\varphi(\mathcal{C}B) = \mathcal{C}\varphi(B)$. En vertu de la prop. 6, $\overline{A}$ est saturé, donc $\varphi(\overline{A})$ est fermé dans $X/R$, et comme $A \subset \overline{A}$, on a $\varphi(A) \subset \varphi(\overline{A})$, d’où $\varphi(A) \subset \varphi(\overline{A})$; mais puisque $\varphi$ est continue, $\varphi(\overline{A}) \subset \varphi(A)$ (I, p. 9, th. 1), d’où la conclusion.

Inversement, supposons que l’on ait $\varphi^{-1}(\overline{C}) = \overline{\varphi^{-1}(C)}$ pour toute partie $C$ de $X/R$, et montrons que pour tout ensemble $U$ ouvert dans $X$, $\varphi(U)$ est ouvert dans $X/R$; dans le cas contraire, il existerait dans $\varphi(U)$ un point $z$ adhérent à $C = \mathcal{C}_{\varphi}(U)$, donc il y aurait dans $U$ un point $x \in \varphi^{-1}(\overline{C}) = \overline{\varphi^{-1}(C)}$; mais cela est absurde puisque $U$ est ouvert et $U \cap \varphi^{-1}(C) = \varnothing$.

#### Corollaire {#top-i-s5-n3-cor-1 .statement}

*Les notations étant celles de la prop. 7, si la relation $R$ est ouverte, alors, pour qu’une partie $Z$ de $X/R$ soit localement fermée, il faut et il suffit que $\varphi^{-1}(Z)$ soit localement fermée dans $X$.

En effet, dire que $Z$ est localement fermée dans $X/R$ signifie que $\overline{Z} - Z$ est fermée dans $X/R$ (I, p. 20, prop. 5); mais cela équivaut à dire que $\varphi^{-1}(\overline{Z} - Z) = \overline{\varphi^{-1}(\overline{Z})} - \varphi^{-1}(Z)$ est une partie fermée de $X$ (I, p. 21); en vertu de la prop. 7, cela signifie aussi que $\varphi^{-1}(Z) - \varphi^{-1}(Z)$ est fermée dans $X$, autrement dit que $\varphi^{-1}(Z)$ est localement fermée dans $X$.

#### Proposition 8 {#top-i-s5-prop-8 .statement}

*Soient $(X_i)_{i \in I}, (Y_i)_{i \in I}$ deux familles d’espaces topologiques ayant même ensemble d’indices. Pour tout $i \in I$, soit $f_i$ une application ouverte de $X_i$ dans $Y_i$, et supposons que $f_i$ soit surjective sauf pour un nombre fini d’indices. Alors l’application produit $f : (x_i) \mapsto (f_i(x_i))$ de $\prod_{i \in I} X_i$ dans $\prod_{i \in I} Y_i$ est ouverte.*

Il suffit en effet (I, p. 33, prop. 5) de prouver que l’image par $f$ de tout ensemble élémentaire $\prod_{i \in I} A_i$ de $\prod_{i \in I} X_i$ est ouverte dans $\prod_{i \in I} Y_i$. Or, cette image est $\prod_{i \in I} f_i(A_i)$ et les hypothèses entraînent que $f_i(A_i)$ est ouvert dans $Y_i$ pour tout $i \in I$ et que $f_i(A_i) = Y_i$ sauf pour un nombre fini d’indices; d’où la conclusion.

#### Corollaire {#top-i-s5-n3-cor-2 .statement}

*Soit $(X_i)_{i \in I}$ une famille d’espaces topologiques, et pour chaque $i \in I$, soient $R_i$ une relation d’équivalence dans $X_i$, $f_i$ l’application canonique $X_i \to X_i/R_i$. Soit $R$ la relation d’équivalence dans $X = \prod_{i \in I} X_i$

« pour tout $i \in I$, $\mathrm{pr}_i x \equiv \mathrm{pr}_i y \ (\mathrm{mod.}\ R_i)$ »

entre $x$ et $y$, et soit $f$ l’application produit $(x_i) \mapsto (f_i(x_i))$ de $X$ dans $\prod_{i \in I} (X_i/R_i)$. Si chacune des relations $R_i$ est ouverte, la relation $R$ est ouverte, et la bijection associée à $f$ est un homéomorphisme de $X/R$ sur $\prod_{i \in I} (X_i/R_i)$.

En effet, $R$ est la relation $f(x) = f(y)$, et comme $f$ est continue et ouverte en vertu de la prop. 8 ci-dessus et de I, p. 25, cor. 1, la conclusion résulte de la prop. 3 de I, p. 32.

En particulier, si R (resp. S) est une relation d’équivalence ouverte dans un espace topologique X (resp. Y), la bijection canonique (E, II, p. 47) de (X × Y)/(R × S) sur (X/R) × (Y/S) est un homéomorphisme; lorsqu’on ne suppose plus R et S ouvertes, cette bijection est encore continue, mais n’est plus nécessairement un homéomorphisme, même lorsque l’une des relations R, S est la relation d’égalité (I, p. 96, exerc. 6).

### 4. Propriétés spéciales aux applications fermées

#### Proposition 9 {#top-i-s5-prop-9 .statement}

Soient X, X' deux espaces topologiques. Pour qu’une application f : X → X' soit continue et fermée, il faut et il suffit que $f(\overline{A}) = \overline{f(A)}$ pour toute partie A de X.

La condition est suffisante, car elle entraîne évidemment que f est fermée, et elle entraîne aussi que f est continue en vertu de I, p. 9, th. 1. Inversement, si f est continue et fermée, on a $f(A) \subset f(\overline{A}) \subset \overline{f(A)}$ en vertu de I, p. 9, th. 1, et en outre $f(\overline{A})$ est fermé dans X' par hypothèse, donc $f(\overline{A}) = \overline{f(A)}$.

#### Proposition 10 {#top-i-s5-prop-10 .statement}

Soit R une relation d’équivalence dans un espace topologique X. Pour que R soit fermée, il faut et il suffit que toute classe d’équivalence M suivant R admette un système fondamental de voisinages saturés pour R.

En effet, supposons que R soit fermée, et soit U un voisinage ouvert quelconque de M; comme F = CU est fermé dans X, l’ensemble S saturé de F pour R est fermé dans X. Comme M est saturé pour R, on a $M \cap S = \varnothing$, donc V = CS est un voisinage ouvert de M, saturé pour R et contenu dans U.

Inversement, supposons que R satisfasse à la condition de l’énoncé, et soit F une partie fermée quelconque de X. Soient T le saturé de F pour R, x un point de CT, M la classe d’équivalence de x; on a $M \cap T = \varnothing$ et a fortiori $M \cap F = \varnothing$, autrement dit, U = CF est un voisinage de M. Il existe donc un voisinage V ⊂ U de M, saturé pour R; comme $V \cap F = \varnothing$, on a aussi $V \cap T = \varnothing$; il en résulte que CT est un voisinage de M, donc de x, ce qui prouve (I, p. 2, prop. 1) que CT est ouvert, donc que T est fermé.

#### Remarque {#top-i-s5-n4-rem-1 .statement}

La prop. 10 entraîne la propriété suivante: Si R est fermée, en désignant par φ l’application canonique X → X/R, pour tout $x \in X$ et tout voisinage U de la classe d’équivalence de x dans X, $\varphi(U)$ est un voisinage de $\varphi(x)$ dans X/R. On aura soin de noter que cela n’entraîne nullement que pour tout voisinage V de x dans X/R, $\varphi(V)$ soit un voisinage de $\varphi(x)$; en d’autres termes (I, p. 33, prop. 5) une relation d’équivalence fermée n’est pas nécessairement ouverte (I, p. 96, exerc. 2). Inversement, une relation d’équivalence ouverte n’est pas nécessairement fermée (I, p. 30, Exemple 4): car si U est un voisinage dans X d’une classe d’équivalence M, pour tout $x \in M$ et tout voisinage $V \subset U$ de x, le saturé de V est bien un voisinage de M dans X, mais ce voisinage n’est pas nécessairement contenu dans U.

Notons enfin qu’il existe des relations d’équivalence distinctes de l’égalité et qui sont à la fois ouvertes et fermées (I, p. 96, exerc. 3) et des relations d’équivalence qui ne sont ni ouvertes ni fermées (I, p. 101, exerc. 10).

## EXERCICES {#top-i-s5-exercises}

See the [exercises for § 5](exercises/s5/).
