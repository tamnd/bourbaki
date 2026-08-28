---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 10
section_title: Applications propres
lang: fr
source: top-i-iv-fr
book_pages: TG I.111-TG I.115
pdf_pages: 0084-0092, 0123-0127
extraction: ocr
subsections:
    - "no": 1
      title: Applications propres
      page: 0
      pdf_page: 84
    - "no": 2
      title: Caractérisation des applications propres par des propriétés de compacité
      page: 74
      pdf_page: 86
    - "no": 3
      title: Applications propres dans les espaces localement compacts
      page: 77
      pdf_page: 89
    - "no": 4
      title: Espaces quotients des espaces compacts et des espaces localement compacts
      page: 78
      pdf_page: 90
statements: 30
exercises: 25
content_sha256: b7c0026c11a62e7e8bc121c792ef5e6cf80c8525c8f16f001bedf5104a303325
---

## § 10. APPLICATIONS PROPRES

Dans ce paragraphe, nous noterons $\mathrm{Id}_X$ l’application identique d’un ensemble $X$ sur lui-même.

### 1. Applications propres

Si $f : X \to Y$ et $f' : X' \to Y'$ sont deux applications continues fermées, le produit $f \times f' : X \times X' \to Y \times Y'$ n’est pas nécessairement une application fermée, même si $f$ est de la forme $\mathrm{Id}_X$.

#### Exemple {#top-i-s10-n1-exa-1 .statement}

Toute application constante dans un espace séparé est fermée. Mais si $f$ est l’application constante $\mathbf{Q} \to \{0\}$, $f \times \mathrm{Id}_\mathbf{Q}$ est l’application $(x, y) \mapsto (0, y)$ de $\mathbf{Q}^2$ dans $\mathbf{Q}^2$, qui s’identifie à la deuxième projection et n’est pas fermée (I, p. 26, Remarque 1).

#### Définition 1 {#top-i-s10-def-1 .statement}

Soit $f$ une application d’un espace topologique $X$ dans un espace topologique $Y$. On dit que $f$ est propre si $f$ est continue et si, pour tout espace topologique $Z$, l’application $f \times \mathrm{Id}_Z : X \times Z \to Y \times Z$ est fermée.

On donnera aux nos 2 et 3 d’autres caractérisations des applications propres.

En prenant dans la déf. 1 l’espace $Z$ réduit à un point, on voit que:

#### Proposition 1 {#top-i-s10-prop-1 .statement}

Toute application propre est fermée.

#### Proposition 2 {#top-i-s10-prop-2 .statement}

Soit $f : X \to Y$ une application continue injective. Les trois propriétés suivantes sont équivalentes:
a) $f$ est propre.
b) $f$ est fermée.
c) $f$ est un homéomorphisme de $X$ sur une partie fermée de $Y$.

On vient de voir que a) entraîne b). Comme la relation d’équivalence $f(x) = f(x')$ est la relation d’égalité, l’espace quotient de $X$ par cette relation s’identifie à $X$, donc b) entraîne c) en vertu de I, p. 32, prop. 3. Enfin, si c) est vérifiée, $f \times \mathrm{Id}_Z$ est un homéomorphisme de $X \times Z$ sur un sous-espace fermé de $Y \times Z$, donc est une application fermée, ce qui prouve que c) entraîne a).

#### Proposition 3 {#top-i-s10-prop-3 .statement}

Soit $f : X \to Y$ une application continue; pour toute partie $T$ de $Y$, désignons par $f_T$ l’application de $f^{-1}(T)$ dans $T$ qui coïncide avec $f$ dans $f^{-1}(T)$.
a) Si $f$ est propre, $f_T$ est propre.
b) Soit $(T(t))_{t \in I}$ une famille de parties de $Y$ dont les intérieurs forment un recouvrement de $Y$, ou qui est un recouvrement fermé localement fini de $Y$; si toutes les $f_{T(t)}$ sont propres, alors $f$ est propre.

Soit $Z$ un espace topologique. Pour toute partie $T$ de $Y$, on a $f_T \times \mathrm{Id}_Z = (f \times \mathrm{Id}_Z)_{T \times Z}$; si $f$ est propre, $f \times \mathrm{Id}_Z$ est fermée, donc il en est de même de $(f \times \mathrm{Id}_Z)_{T \times Z}$ (I, p. 31, prop. 2 a)), ce qui démontre a). Si maintenant $(T(t))$ a l’une des propriétés énoncées dans b), le recouvrement $(T(t) \times Z)_{t \in I}$ de

Y × Z a la même propriété; si les $f_{T(i)}$ sont propres, les $(f \times \mathrm{Id}_Z)_{T(i) \times Z}$ sont fermées, donc $f \times \mathrm{Id}_Z$ est fermée (I, p. 31, prop. 2 b)), ce qui achève la démonstration.

#### Proposition 4 {#top-i-s10-prop-4 .statement}

Soit $I$ un ensemble fini, et pour tout $i \in I$, soit $f_i : X_i \to Y_i$ une application continue. Posons $X = \prod_i X_i$, $Y = \prod_i Y_i$, et soit $f : X \to Y$ l’application produit $(x_i) \mapsto (f_i(x_i))$ des $f_i$. Alors:
a) *Si chacune des $f_i$ est propre, $f$ est propre.*
b) *Si $f$ est propre et si les $X_i$ sont non vides, chacune des $f_i$ est propre.*
(Nous verrons dans I, p. 76, cor. 3, que cette proposition s’étend aux produits infinis.)

En raisonnant par récurrence, on voit qu’il suffit de considérer le cas où $I = \{1, 2\}$.
a) Supposons $f_1, f_2$ propres, et soit $Z$ un espace topologique; l’application $f_1 \times f_2 \times \mathrm{Id}_Z$ est la composée des applications $\mathrm{Id}_{Y_1} \times f_2 \times \mathrm{Id}_Z$ et $f_1 \times \mathrm{Id}_{X_2} \times \mathrm{Id}_Z$; ces deux applications sont fermés par hypothèse, donc $f_1 \times f_2 \times \mathrm{Id}_Z$ est fermée (I, p. 30, prop. 1 a)), et $f = f_1 \times f_2$ est propre.
b) Supposons maintenant $f$ propre; soit $F$ une partie fermée de $X_2 \times Z$, et soit $G$ son image dans $Y_2 \times Z$ par $f_2 \times \mathrm{Id}_Z$; l’image de $X_1 \times F$ dans $Y_1 \times Y_2 \times Z$ par $f_1 \times f_2 \times \mathrm{Id}_Z$ est égale à $f_1(X_1) \times G$. Par hypothèse, $f_1(X_1) \times G$ est fermé dans $Y_1 \times Y_2 \times Z$; si $X_1 \neq \varnothing$, $f_1(X_1)$ est non vide, et cela entraîne que $G$ est fermé dans $Y_2 \times Z$ (I, p. 27, corollaire); donc l’application $f_2$ est propre. On montre de même que $f_1$ est propre si $X_2 \neq \varnothing$.

#### Proposition 5 {#top-i-s10-prop-5 .statement}

Soient $f : X \to X'$ et $g : X' \to X''$ deux applications continues. Alors:
a) *Si $f$ et $g$ sont propres, $g \circ f$ est propre.*
b) *Si $g \circ f$ est propre et si $f$ est surjective, $g$ est propre.*
c) *Si $g \circ f$ est propre et si $g$ est injective, $f$ est propre.*
d) *Si $g \circ f$ est propre et si $X'$ est séparé, $f$ est propre.*

Soit $Z$ un espace topologique. On a $(g \circ f) \times \mathrm{Id}_Z = (g \times \mathrm{Id}_Z) \circ (f \times \mathrm{Id}_Z)$; si $f$ et $g$ sont propres, $f \times \mathrm{Id}_Z$ et $g \times \mathrm{Id}_Z$ sont fermées, donc (I, p. 30, prop. 1 a)), $(g \circ f) \times \mathrm{Id}_Z$ est fermée, ce qui démontre a). On démontre de même b) (resp. c)) en appliquant la partie b) (resp. c)) de la prop. 1 de I, p. 30, et en remarquant que si $f$ est surjective (resp. si $g$ est injective), $f \times \mathrm{Id}_Z$ est surjective (resp. $g \times \mathrm{Id}_Z$ est injective). Plaçons-nous maintenant dans les hypothèses de d). Considérons le diagramme commutatif

$$
\begin{array}{ccc}
X & \xrightarrow{\varphi} & X \times X' \\
\downarrow f & & \downarrow (g \circ f) \times \mathrm{Id}_{X'} \\
X' & \xrightarrow{\psi} & X'' \times X'
\end{array}
$$

(1)

où $\varphi(x) = (x, f(x))$ et $\psi(x') = (g(x'), x')$. L’application $\varphi$ (resp. $\psi$) est un homéomorphisme de $X$ (resp. $X'$) sur le graphe de $f$ (resp. le symétrique du graphe de $g$) (I, p. 25, cor. 2); de plus, puisque $X'$ est séparé, le graphe $\varphi(X)$ de $f$ est fermé dans $X \times X'$ (I, p. 53, cor. 2). Donc (I, p. 72, prop. 2) $\varphi$ est propre; d’autre part la prop. 4 de I, p. 73 montre que $(g \circ f) \times \mathrm{Id}_{X'}$ est propre. D’après a) et la commutativité du diagramme (1), $\psi \circ f$ est propre, et puisque $\psi$ est injective, il résulte de c) que $f$ est propre.

#### Remarque {#top-i-s10-n1-rem-1 .statement}

Si $X'$ n’est pas séparé, il peut se faire que $g \circ f$ soit propre sans que $f$ le soit: il suffit de prendre pour $X$ et $X''$ (resp. $X'$) des ensembles à un (resp. deux) éléments et de munir $X'$ de la topologie la moins fine.

#### Corollaire 1 {#top-i-s10-prop-5-cor-1 .statement}

Si $f : X \to Y$ est une application propre, la restriction de $f$ à une partie fermée $F$ de $X$ est une application propre de $F$ dans $Y$.

En effet, cette restriction est la composée $f \circ j$, où $j : F \to X$ est l’injection canonique, qui est propre (I, p. 72, prop. 2).

#### Corollaire 2 {#top-i-s10-prop-5-cor-2 .statement}

Soit $f : X \to Y$ une application propre. Si $X$ est séparé, le sous-espace $f(X)$ de $Y$ est séparé.

En vertu de la prop. 5 c), on peut se borner au cas où $f(X) = Y$. Alors la diagonale de $Y \times Y$ est image par $f \times f$ de la diagonale de $X$, laquelle est fermée (I, p. 52, prop. 1); comme $f \times f$ est propre (I, p. 73, prop. 4) la diagonale de $Y \times Y$ est fermée (I, p. 72, prop. 1), donc $Y$ est séparé (I, p. 52, prop. 1).

#### Corollaire 3 {#top-i-s10-prop-5-cor-3 .statement}

Soit $I$ un ensemble fini, et pour tout $i \in I$, soit $f_i : X \to Y_i$ une application propre. Si $X$ est séparé, l’application $x \mapsto (f_i(x))$ de $X$ dans $\prod_i Y_i$ est propre.

En effet, cette application est composée de l’application produit $(x_i) \mapsto (f_i(x_i))$ de $X^I$ dans $\prod_i Y_i$, et de l’application diagonale de $X$ dans $X^I$; comme cette dernière est propre (I, p. 72, prop. 2 et I, p. 52, prop. 1), la conclusion résulte de la prop. 4 (I, p. 73) et de la prop. 5 a).

#### Corollaire 4 {#top-i-s10-prop-5-cor-4 .statement}

Soient $X, Y$ deux espaces topologiques, $f : X \to Y$ une application continue, $R$ la relation d’équivalence $f(x) = f(y)$ dans $X$, $X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y$ la décomposition canonique de $f$. Pour que $f$ soit propre, il faut et il suffit que $p$ soit propre, que $h$ soit un homéomorphisme et $f(X)$ une partie fermée de $Y$.

Les conditions sont suffisantes en vertu de la prop. 5 a) (I, p. 73) et de la prop. 2 (I, p. 72). Inversement, si $f$ est propre, $f$ est fermée, donc on sait déjà que $f(X)$ est fermé dans $Y$ et que $h$ est un homéomorphisme (I, p. 32, prop. 3); en outre, $h \circ p$ est propre en vertu de la prop. 5 c) (I, p. 73), donc $p = h^{-1} \circ (h \circ p)$ est propre en vertu de la prop. 5 a) (I, p. 73).

### 2. Caractérisation des applications propres par des propriétés de compacité

Dans ce numéro, nous désignerons par $P$ un espace réduit à un point, et muni de son unique topologie.

#### Lemme 1 {#top-i-s10-lem-1 .statement}

Soit $X$ un espace topologique tel que l’application constante $X \to P$ soit propre. Alors $X$ est quasi-compact.

(Nous verrons un peu plus loin (I, p. 76, cor. 1) que cette propriété caractérise les espaces quasi-compacts.)

On peut se borner au cas où $X$ est non vide. Soient $\mathcal{F}$ un filtre sur $X$, $X' = X \cup \{ \omega \}$ l’espace topologique associé à $\mathcal{F}$ (I, p. 40, Exemple). Soient $\Delta$ la partie de $X \times X'$ formée des couples $(x, x)$, où $x$ parcourt $X$, et $F = \overline{\Delta}$ l’adhérence de $\Delta$ dans $X \times X'$. Vu l’hypothèse faite sur $X$, l’image de $F$ par la projection $X \times X' \to X'$ est fermée dans $X'$; comme cette image contient $X$, elle contient nécessairement $\omega$, qui est adhérent à $X$; autrement dit, il existe $x \in X$ tel que $(x, \omega) \in F$. Par définition de la topologie de $X \times X'$, cela signifie que pour tout voisinage $V$ de $x$ dans $X$ et tout ensemble $M \in \mathcal{F}$, on a $(V \times M) \cap \Delta \neq \varnothing$, c’est-à-dire $V \cap M \neq \varnothing$; en d’autres termes, $x$ est adhérent au filtre $\mathcal{F}$.

C.Q.F.D.

#### Théorème 1 {#top-i-s10-thm-1 .statement}

Soit $f : X \to Y$ une application continue. Les quatre propriétés suivantes sont équivalentes:

a) $f$ est propre.

b) $f$ est fermée, et pour tout $y \in Y, f^{-1}(y)$ est quasi-compact.

c) Si $\mathcal{F}$ est un filtre sur $X$ et si $y \in Y$ est adhérent à $f(\mathcal{F})$, il existe un point $x \in X$ adhérent à $\mathcal{F}$ et tel que $f(x) = y$.

d) Si $\mathcal{U}$ est un ultrafiltre sur $X$, et si $y \in Y$ est un point limite de la base d’ultrafiltre $f(\mathcal{U})$, il existe un point limite $x$ de $\mathcal{U}$ tel que $f(x) = y$.

a) entraîne b): En effet, si $f$ est propre, $f$ est fermée (I, p. 72, prop. 1) et pour tout $y \in Y$, l’application $f_{\{y\}} : f(y) \to \{y\}$ est propre (I, p. 72, prop. 3 a)). D’après le lemme 1, cela implique que $f^{-1}(y)$ est quasi-compact.

b) entraîne c): Supposons que $\mathcal{F}$ et $y$ vérifient les hypothèses de c) et soit $\mathcal{B}$ la base de filtre sur $X$ formée des adhérences des ensembles de $\mathcal{F}$. Puisque $f$ est fermée, $f(\overline{M}) = \overline{f(M)}$ pour $M \in \mathcal{F}$ (I, p. 35, prop. 9). Cela prouve que les ensembles $\overline{M} \cap f^{-1}(y)$ sont non vides pour $M \in \mathcal{F}$, et forment par suite une base de filtre sur $f^{-1}(y)$ composée d’ensembles fermés dans $f^{-1}(y)$. Comme $f^{-1}(y)$ est quasi-compact, il existe $x \in f^{-1}(y)$ appartenant à tous les $\overline{M}$ pour $M \in \mathcal{F}$; on a $f(x) = y$ et $x$ est adhérent à $\mathcal{F}$.

c) implique d) trivialement.

d) entraîne que $f$ est fermée. En effet, soit $A$ une partie fermée non vide de $X$, et soit $\mathcal{F}$ le filtre des parties de $X$ contenant $A$; $A$ est alors l’ensemble des points adhérents à $\mathcal{F}$. Soit $B$ l’ensemble des points adhérents au filtre de base $f(\mathcal{F})$ sur $Y$; $B$ est fermé et contient évidemment $f(A)$; nous allons voir que $B = f(A)$, ce qui prouvera notre assertion. Soit $y \in B$ et soit $\mathcal{V}$ le filtre des voisinages de $y$ dans $Y$; par hypothèse, tout ensemble de $\mathcal{W} = f^{-1}(\mathcal{V})$ rencontre tout ensemble de $\mathcal{F}$, donc $\mathfrak{W}$ est une base de filtre sur $X$ et il y a un ultrafiltre $\mathcal{U}$ sur $X$, plus fin que le filtre de base $\mathfrak{W}$ et que $\mathfrak{F}$ (I, p. 37, cor. 2 et I, p. 39, th. 1). L’ultrafiltre de base $f(\mathcal{U})$ est plus fin que $\mathfrak{V}$, donc converge vers $y$. En vertu de d), il existe $x \in X$ tel que $f(x) = y$ et que $\mathcal{U}$ converge vers $x$; comme $\mathcal{U}$ est plus fin que $\mathfrak{F}$, $x$ est adhérent à $\mathfrak{F}$, donc $x \in A$, ce qui prouve que $B = f(A)$.

d) entraîne a) : En effet, il faut montrer que si $f$ vérifie d) l’application $f \times \mathrm{Id}_Z$ est fermée pour tout espace topologique $Z$. D’après ce qui précède, il suffit de prouver que $f \times \mathrm{Id}_Z$ vérifie aussi la condition d). Cela résultera du lemme général suivant:

#### Lemme 2 {#top-i-s10-lem-2 .statement}

Si $(f_i)_{i \in I}$ est une famille d’applications continues $f_i : X_i \to Y_i$ dont chacune vérifie la condition d), alors l’application produit $f : (x_i) \mapsto (f_i(x_i))$ vérifie aussi la condition d).

En effet, soit $\mathcal{U}$ un ultrafiltre sur $X = \prod_i X_i$, et soit $y = (y_i)$ un point de $Y = \prod_i Y_i$ tel que $f(\mathcal{U})$ converge vers $y$. Cela signifie que chacune des bases d’ultrafiltre $\mathrm{pr}_i(f(\mathcal{U})) = f_i(\mathrm{pr}_i(\mathcal{U}))$ converge vers $y_i$ (I, p. 51, cor. 1). En vertu de la condition d), il existe pour chaque $i \in I$, un $x_i \in X_i$ tel que $f_i(x_i) = y_i$ et que $\mathrm{pr}_i(\mathcal{U})$ converge vers $x_i$; mais alors $\mathcal{U}$ converge vers $x = (x_i)$ (loc. cit.) et on a $f(x) = y$, ce qui démontre le lemme et achève la démonstration du th. 1.

#### Corollaire 1 {#top-i-s10-lem-2-cor-1 .statement}

Pour qu’un espace topologique $X$ soit quasi-compact, il faut et il suffit que l’application $X \to P$ soit propre.

On applique l’équivalence de a) et b) à $X \to P$.

#### Corollaire 2 {#top-i-s10-lem-2-cor-2 .statement}

Toute application continue $f$ d’un espace quasi-compact $X$ dans un espace séparé $Y$ est propre.

L’application composée $X \xrightarrow{f} Y \longrightarrow P$ est propre (cor. 1) donc $f$ est propre en vertu de la prop. 5 d) de I, p. 73. On peut aussi appliquer le critère b) du th. 1, en utilisant le cor. 2 de I, p. 63.

#### Corollaire 3 {#top-i-s10-lem-2-cor-3 .statement}

Si $(f_i)$ est une famille d’applications propres, l’application produit $(x_i) \mapsto (f_i(x_i))$ est propre.

Compte tenu du th. 1, ce n’est autre que le lemme 2 ci-dessus.

Si on applique ce corollaire à la famille d’applications $X_i \to P$, on retrouve, compte tenu du cor. 1, le th. de Tychonoff (I, p. 63, th. 3).

#### Corollaire 4 {#top-i-s10-lem-2-cor-4 .statement}

Soit $X$ un espace séparé. Pour toute famille d’applications propres $f_i : X \to Y_i$, l’application $x \mapsto (f_i(x))$ de $X$ dans $\prod_i Y_i$ est propre.

La démonstration est la même que pour le cas d’une famille finie (I, p. 74, cor. 3), en utilisant le cor. 3 ci-dessus, et le fait que la diagonale de $X^I$ est fermée (I, p. 52, prop. 1).

#### Corollaire 5 {#top-i-s10-lem-2-cor-5 .statement}

Pour tout espace quasi-compact $X$ et tout espace topologique $Y$, la projection $\mathrm{pr}_2 : X \times Y \to Y$ est propre.

En effet, on peut identifier $Y$ à $P \times Y$, en identifiant $\mathrm{pr}_2$ au produit des applications propres $X \to P$ (cor. 1) et $\mathrm{Id}_Y$, d’où la conclusion (cor. 3).

#### Exemple {#top-i-s10-n2-exa-1 .statement}

Soient $X$ un ensemble, $f : X \to X'$ une application surjective de $X$ dans un espace topologique $X'$; on munit $X$ de la topologie image réciproque de celle de $X'$ par $f$. Alors $f$ est propre, car elle est fermée (I, p. 30, Exemple 3), et l’image réciproque d’un point de $X'$ est un sous-espace de $X$ dont la topologie est la topologie la moins fine et qui est par suite quasi-compact.

#### Remarque {#top-i-s10-n2-rem-1 .statement}

Lorsque $Y$ est séparé, la condition d) du th. 1 est équivalente à:

d') Si $\mathcal{U}$ est un ultrafiltre sur $X$ tel que $f(\mathcal{U})$ soit une base de filtre convergente, alors $\mathcal{U}$ est convergent.

En effet, si $\mathcal{U}$ converge vers $x$ et $f(\mathcal{U})$ vers $y$, l’unicité de la limite dans $Y$ et la continuité de $f$ montrent que l’on a nécessairement $y = f(x)$. De même, la condition c) du th. 1 est alors équivalente à:

c') Si $\mathcal{F}$ est un filtre sur $X$ tel que $f(\mathcal{F})$ ait un point adhérent, alors $\mathcal{F}$ a un point adhérent.

En effet, c) $\Rightarrow$ c') $\Rightarrow$ d') $\Rightarrow$ d) $\Rightarrow$ c).

Par contre, si $Y$ n’est pas séparé, d') n’entraîne plus d), comme le montre l’exemple où $X$ est réduit à un point, $Y$ formé de deux éléments et muni de la topologie la moins fine.

#### Proposition 6 {#top-i-s10-prop-6 .statement}

Soit $f : X \to Y$ une application propre, et soit $K$ une partie quasi-compacte de $Y$. Alors l’ensemble $f^{-1}(K)$ est quasi-compact.

D’après la prop. 3 de I, p. 72, l’application $f_K : f^{-1}(K) \to K$ est propre; comme $K \to P$ est une application propre (I, p. 76, cor. 1), il résulte de I, p. 73, prop. 5 a), que l’application composée $f^{-1}(K) \xrightarrow{f_K} K \longrightarrow P$ est propre, donc $f^{-1}(K)$ est quasi-compact (I, p. 76, cor. 1).

### 3. Applications propres dans les espaces localement compacts

#### Proposition 7 {#top-i-s10-prop-7 .statement}

Soit $f$ une application continue d’un espace séparé $X$ dans un espace localement compact $Y$. Pour que $f$ soit propre, il faut et il suffit que pour toute partie compacte $K$ de $Y, f^{-1}(K)$ soit un ensemble compact. En outre, si $f$ est propre, $X$ est localement compact.

Si $f$ est propre, $f^{-1}(K)$ est compact pour toute partie compacte $K$ de $Y$, en vertu de la prop. 6. Inversement, supposons cette condition vérifiée, et soit $(\overline{U}_\alpha)$ un recouvrement de $Y$ formé d’ensembles ouverts relativement compacts. L’hypothèse entraîne que les $f^{-1}(\overline{U}_\alpha)$ sont compacts et que leurs intérieurs forment un recouvrement de $X$; comme $X$ est séparé, cela prouve en premier lieu que $X$ est localement compact. En outre, chacune des applications $f_{\overline{U}_\alpha} : f^{-1}(\overline{U}_\alpha) \to \overline{U}_\alpha$ est propre (I, p. 76, cor. 2); donc $f$ est propre (I, p. 72, prop. 3 b)).

#### Corollaire {#top-i-s10-n3-cor-1 .statement}

Soient $X, X'$ deux espaces localement compacts, $Y, Y'$ les espaces compacts obtenus en adjoignant à $X, X'$ respectivement des points à l’infini $\omega, \omega'$ (I, p. 68). Pour qu’une application continue $f : X \to X'$ soit propre, il faut et il suffit que son prolongement $\bar{f} : Y \to Y'$ tel que $\bar{f}(\omega) = \omega'$ soit continu.

En effet, en vertu de la prop. 7, dire que $f$ est propre signifie que pour toute partie compacte $K'$ de $X'$, $\bar{f}(X' - K') = X - \bar{f}(K')$ est le complémentaire d’une partie compacte de $X$; par définition des voisinages de $\omega$ et $\omega'$ dans $Y$ et $Y'$ respectivement (I, p. 67, th. 4), cela équivaut aussi à dire que $\bar{f}$ est continue au point $\omega$, d’où le corollaire.

### 4. Espaces quotients des espaces compacts et des espaces localement compacts

#### Proposition 8 {#top-i-s10-prop-8 .statement}

Soient $X$ un espace compact, $R$ une relation d’équivalence dans $X$, $C$ son graphe dans $X \times X$, $f$ l’application canonique $X \to X/R$. Les conditions suivantes sont équivalentes:
a) $C$ est fermé dans $X \times X$.
b) $R$ est fermée.
c) $f$ est propre.
d) $X/R$ est séparé.
En outre, lorsque ces conditions sont vérifiées, $X/R$ est compact.

Dire que $R$ est fermée équivaut à dire que $f$ est fermée, donc b) entraîne c) en vertu de I, p. 75, th. 1 b). Le fait que c) entraîne d) est un cas particulier de I, p. 74, cor. 2. On sait déjà que d) entraîne a) sans hypothèse sur $X$ (I, p. 55, prop. 8). Prouvons ensuite que a) entraîne b). Or, si $F$ est une partie fermée de $X$, son saturé est $\mathrm{pr}_2(C \cap (F \times X))$; par hypothèse, $C \cap (F \times X)$ est fermé dans l’espace compact $X \times X$, donc est compact (I, p. 61, prop. 2), et notre assertion résulte de la continuité de $\mathrm{pr}_2$ (I, p. 63, cor. 2).

Enfin, il est clair que si $X/R$ est séparé, il est compact en vertu de I, p. 62, th. 2.

#### Proposition 9 {#top-i-s10-prop-9 .statement}

Soient $X$ un espace localement compact, $R$ une relation d’équivalence dans $X$, $C$ son graphe dans $X \times X$, $f$ l’application canonique $X \to X/R$; soit $X'$ l’espace compact obtenu en adjoignant à $X$ un point à l’infini $\omega$ (I, p. 68), et soit $R'$ la relation d’équivalence dans $X'$, de graphe $C' = C \cup \{(\omega, \omega)\}$. Les conditions suivantes sont équivalentes:
a) $f$ est propre.
b) Le saturé pour $R$ de toute partie compacte de $X$ est un ensemble compact.
c) $R'$ est fermée.
d) La restriction à $C$ de $\mathrm{pr}_2$ est propre.
e) $R$ est fermée et les classes suivant $R$ sont compactes.
En outre, lorsque ces conditions sont remplies, $X/R$ est localement compact.
a) $\Rightarrow$ b): En effet, comme $X/R = f(X)$, $X/R$ est séparé (I, p. 74, cor. 2), donc l’image par $f$ de toute partie compacte $K$ de $X$ est compacte (I, p. 63, cor. 1); comme le saturé de $K$ pour $R$ est $f^{-1}(f(K))$, il est compact en vertu de la prop. 6 de I, p. 77.

b) $\Rightarrow$ c): Si $F'$ est fermé dans $X'$ et ne contient pas $\omega$, $F'$ est une partie compacte de $X$, donc son saturé pour $R'$, égal à son saturé pour $R$, est compact et $a fortiori$ fermé dans $X'$. Si $\omega \in F'$ et si $F = F' \cap X = F' - \{ \omega \}$, le saturé de $F'$ pour $R'$ est la réunion de $\{ \omega \}$ et du saturé $H$ de $F$ pour $R$, et il suffit de prouver que $H$ est *fermé dans* $X$ (autrement dit, que $R$ est une relation *fermée*). Pour cela, il suffit de montrer que pour toute partie compacte $K$ de $X$, $H \cap K$ est compact (I, p. 66, prop. 11). Or, le saturé $L$ de $K$ pour $R$ est compact par hypothèse, et la trace de $H$ sur $L$ est le saturé de $F \cap L$, qui est aussi compact; $a fortiori$ $H \cap K = (H \cap L) \cap K$ est compact.

c) $\Rightarrow$ d): En effet, comme $X'$ est régulier (I, p. 61 corollaire), $C'$ est *fermé* dans $X' \times X'$ (I, p. 58, prop. 14), donc compact. On en conclut que $C'$ est le compactifié d’Alexandroff de $C$ (I, p. 67, th. 4); comme la restriction de $\mathrm{pr}_2 : X' \times X' \to X'$ à $C'$ est continue au point $\omega$, la conclusion résulte de I, p. 78, corollaire.

d) $\Rightarrow$ e): Pour toute partie fermée $F$ de $X$, $C \cap (F \times X)$ est fermé dans $C$, donc le saturé de $F$ pour $R$, égal à $\mathrm{pr}_2(C \cap (F \times X))$, est fermé dans $X$ (I, p. 72, prop. 1). En outre, la classe de $x \in X$ suivant $R$ est homéomorphe à l’image réciproque de $\{ x \}$ par la restriction de $\mathrm{pr}_2$ à $C$, donc est compacte (I, p. 75, th. 1 b)).

e) $\Rightarrow$ a): En effet, si $R$ est fermée, $f$ est fermée par définition, et pour tout $z \in X/R, f(z)$ est une classe suivant $R$, donc est compacte; notre assertion résulte de I, p. 75, th. 1 b).

Montrons enfin que $X/R$ est localement compact. En effet, $X'/R'$ est compact en vertu de c) et de la prop. 8; la relation $R$ est induite sur $X$ par $R'$, $X$ est ouvert dans $X'$ et saturé pour $R'$; donc $X/R$ est homéomorphe à l’image $f'(X)$ de $X$ par l’application canonique $f' : X' \to X'/R'$ (I, p. 23, cor. 1). Or $f'(X)$ est ouvert dans $X'/R'$, donc est un sous-espace localement compact.

C.Q.F.D.

#### Corollaire {#top-i-s10-n4-cor-1 .statement}

*Soient $X$ un espace séparé, $Y$ un espace topologique, $f : X \to Y$ une application propre. Pour que $X$ soit compact (resp. localement compact), il faut et il suffit que $f(X)$ soit compact (resp. localement compact), et il suffit que $Y$ soit compact (resp. localement compact)*.

En effet, si $X$ est compact (resp. localement compact), le fait que $f(X)$ est compact (resp. localement compact) résulte de I, p. 74, cor. 4 et des prop. 8 et 9 (I, p. 78) (le cas où $X$ est compact étant d’ailleurs aussi conséquence de I, p. 76, cor. 2 et de I, p. 62, th. 2). Inversement, si $Z = f(X)$ est compact (resp. localement compact), comme $f_z : X \to f(X)$ est propre (I, p. 72, prop. 3 a)), $X$ est compact (resp. localement compact), en vertu des prop. 6 et 7 (I, p. 77).

Enfin, si $Y$ est compact (resp. localement compact), il en est de même de $f(X)$, qui est fermé dans $Y$ (I, p. 72, prop. 1 et I, p. 66, prop. 13).

#### Remarque {#top-i-s10-n4-rem-1 .statement}

Si $X$ est localement compact et non compact, une relation d’équivalence fermée $R$ dans $X$ peut être non séparée (IX, §4, exerc. 8); et même si elle est séparée, $X/R$ n’est pas nécessairement localement compact (I, p. 113, exerc. 17). On a toutefois le critère suivant:

#### Proposition 10 {#top-i-s10-prop-10 .statement}

Soient $X$ un espace localement compact, $R$ une relation d’équivalence ouverte et séparée dans $X$, $f$ l’application canonique $X \to X/R$. Alors $X/R$ est localement compact, et pour toute partie compacte $K'$ de $X/R$, il existe une partie compacte $K$ de $X$ telle que $f(K) = K'$.

La première assertion résulte de ce que tout $x \in X$ a un voisinage compact $V$ et de ce que $f(V)$ est un voisinage compact de $f(x)$ (I, p. 33, prop. 5 et I, p. 63, cor. 1). Pour tout $y \in K'$, soit $V(y)$ un voisinage compact d’un point de $f^{-1}(y)$ dans $X$, de sorte que $f(V(y))$ est un voisinage compact de $y$. Il existe un nombre fini de points $y_i \in K'$ tels que les $f(V(y_i))$ recouvrent $K'$. Soit $K_1$ l’ensemble compact $\bigcup_i V(y_i)$ dans $X$; on a $K' \subset f(K_1)$, donc $K = K_1 \cap f^{-1}(K')$ est compact (puisque fermé dans $K_1$) et $f(K) = K'$.

## EXERCICES {#top-i-s10-exercises}

See the [exercises for § 10](exercises/s10/).
