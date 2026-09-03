---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 2
section_title: Ensembles convexes
lang: fr
source: evt-i-v-fr
book_pages: EVT II.7-EVT II.22
pdf_pages: 0042-0057, 0104-0111
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un ensemble convexe
      page: 7
      pdf_page: 42
    - "no": 2
      title: Intersections d’ensembles convexes. Produits d’ensembles convexes
      page: 9
      pdf_page: 44
    - "no": 3
      title: Enveloppe convexe d’un ensemble
      page: 10
      pdf_page: 45
    - "no": 4
      title: Cônes convexes
      page: 11
      pdf_page: 46
    - "no": 5
      title: Espaces vectoriels ordonnés
      page: 13
      pdf_page: 48
    - "no": 6
      title: Ensembles convexes dans les espaces vectoriels topologiques
      page: 14
      pdf_page: 49
    - "no": 7
      title: Topologies sur les espaces vectoriels ordonnés
      page: 17
      pdf_page: 52
    - "no": 8
      title: Fonctions convexes
      page: 17
      pdf_page: 52
    - "no": 9
      title: Opérations sur les fonctions convexes
      page: 19
      pdf_page: 54
    - "no": 10
      title: Fonctions convexes dans un ensemble convexe ouvert
      page: 20
      pdf_page: 55
    - "no": 11
      title: Semi-normes et ensembles convexes
      page: 21
      pdf_page: 56
statements: 52
exercises: 43
content_sha256: d3793785fdbaa7cc89a387116e47a5d804504a666bbdca5f35b27681d1a80813
---

## § 2. ENSEMBLES CONVEXES

### 1. Définition d’un ensemble convexe

Étant donnés deux points $x, y$ d’un espace affine $E$, l’ensemble des points $\lambda x + \mu y$ où $\lambda \geq 0, \mu \geq 0, \lambda + \mu = 1$ est appelé segment fermé d’extrémités $x$ et $y$; il est réduit à un point lorsque $x = y$. Le complémentaire de $x$ dans ce segment est appelé le segment ouvert en $x$, fermé en $y$, d’extrémités $x, y$; il est vide si $x = y$. Enfin, le complémentaire de $\{x, y\}$ dans le segment fermé d’extrémités $x$ et $y$ est appelé le segment ouvert d’extrémités $x$ et $y$; il est vide si $x = y$.

#### Définition 1 {#evt-ii-s2-def-1 .statement}

Dans un espace affine E, on dit qu’un ensemble A est convexe si, quels que soient les points x, y de A, le segment fermé d’extrémités x et y est contenu dans A.

Comme $(1 - \lambda) a + \lambda x = a + \lambda(x - a)$, cette définition équivaut à la suivante : l’ensemble A est convexe si, pour tout point $a \in A$, le transformé de A par toute homothétie de centre a et de rapport $\lambda$ tel que $0 < \lambda < 1$, est contenu dans A (autrement dit, A est stable pour ces homothéties).

#### Exemple 1 {#evt-ii-s2-n1-exa-1 .statement}

Toute variété linéaire affine de E (et en particulier l’ensemble vide) est convexe.

#### Exemple 2 {#evt-ii-s2-n1-exa-2 .statement}

Les seules parties convexes non vides de $\mathbf{R}$ sont les intervalles (TG, IV, p. 7, prop. 1).

#### Exemple 3 {#evt-ii-s2-n1-exa-3 .statement}

Soient E un espace vectoriel et $\|x\|$ une norme sur E ; la boule unité B, formée des points x tels que $\|x\| \leq 1$, est convexe, car les relations $\|x\| \leq 1, \|y\| \leq 1$ entraînent, pour $0 \leq \lambda \leq 1$
$$
\|\lambda x + (1 - \lambda) y\| \leq \lambda \|x\| + (1 - \lambda) \|y\| \leq \lambda + (1 - \lambda) = 1 .
$$

#### Remarque {#evt-ii-s2-n1-rem-1 .statement}

Soit A un ensemble convexe dans un espace vectoriel E ; quels que soient les scalaires $\alpha > 0$ et $\beta > 0$, on a
$$
\alpha A + \beta A = (\alpha + \beta) A .
$$
En d’autres termes, quels que soient $x \in A$ et $y \in A$, il existe $z \in A$ tel que
$$
(\alpha + \beta) z = \alpha x + \beta y ;
$$
en effet, cette relation s’écrit :
$$
z = \frac{\alpha}{\alpha + \beta} x + \frac{\beta}{\alpha + \beta} y
$$
et on a $\frac{\alpha}{\alpha + \beta} > 0,\ \frac{\beta}{\alpha + \beta} > 0$ et $\frac{\alpha}{\alpha + \beta} + \frac{\beta}{\alpha + \beta} = 1$, d’où l’assertion, en vertu de la déf. 1.

#### Proposition 1 {#evt-ii-s2-prop-1 .statement}

Soit $(x_i)$ une famille de points d’un ensemble convexe A ; tout barycentre $\sum_i \lambda_i x_i$ des $x_i$ affectés de masses positives $\lambda_i$ (telles que $\sum_i \lambda_i = 1$ et $\lambda_i = 0$ sauf pour un nombre fini d’indices, cf. A, II, p. 128) appartient à A.

On peut évidemment se borner au cas où l’ensemble d’indices est un intervalle fini $\{1, p\}$ de $\mathbf{N}$, et où $\lambda_i > 0$ pour tout indice i ; la proposition est triviale pour $p = 1$ ; démontrons-la par récurrence sur $p$. Posons $\mu = \sum_{i=1}^{p-1} \lambda_i > 0$, et $y = \sum_{i=1}^{p-1} \frac{\lambda_i}{\mu} x_i$ ; l’hypothèse de récurrence entraîne la relation $y \in A$. Comme on a $\lambda_p = 1 - \mu$ et $\sum_{i=1}^p \lambda_i x_i = \mu y + (1 - \mu) x_p$, le point $\sum_{i=1}^p \lambda_i x_i$ appartient à A d’après la déf. 1.

#### Proposition 2 {#evt-ii-s2-prop-2 .statement}

Soient E et F deux espaces affines, f une application linéaire affine de E dans F ; l’image par f de toute partie convexe de E et l’image réciproque par f de toute partie convexe de F sont des ensembles convexes.

La première partie résulte de ce que l’image par f du segment fermé d’extrémités x, y est le segment fermé d’extrémités $f(x), f(y)$. On déduit de là que l’image réciproque par $f$ d’un segment fermé de F contient le segment fermé ayant pour extrémités deux quelconques de ses points, d’où la seconde partie de la prop. 2.

En particulier, l’image d’un ensemble convexe par une homothétie ou une translation est convexe.

#### Proposition 3 {#evt-ii-s2-prop-3 .statement}

*Soient E un espace affine, H un hyperplan défini par la relation $g(x) = 0$, où g est une fonction affine non constante sur E. Les demi-espaces définis par l’une des relations $g(x) \geqslant 0$, $g(x) \leqslant 0$, $g(x) > 0$, $g(x) < 0$ sont des ensembles convexes.*

En effet, ce sont les images réciproques par l’application affine $g$ d’intervalles de $\mathbf{R}$, qui sont convexes.

Avec les notations de la prop. 3, les points d’une partie M d’un espace affine sont dits *d’un même côté* (resp. *strictement d’un même côté*) de l’hyperplan H si M est contenue dans un des demi-espaces définis par $\alpha(x) \geqslant 0$ ou $g(x) \leqslant 0$ (resp. $g(x) > 0$ ou $g(x) < 0$.)

#### Proposition 4 {#evt-ii-s2-prop-4 .statement}

*Soit H un hyperplan dans un espace affine E. Pour que les points d’une partie convexe A de E soient strictement d’un même côté de H, il faut et il suffit que A ne rencontre pas H.*

La condition est évidemment nécessaire. Inversement supposons-la remplie, et soit $g(x) = 0$ une équation de H (*g* application linéaire affine de E dans $\mathbf{R}$). L’ensemble $g(A)$ est convexe dans $\mathbf{R}$, donc est un intervalle, et on a $0 \notin g(A)$. Il en résulte que $g(x)$ a un signe constant lorsque $x$ parcourt A.

### 2. Intersections d’ensembles convexes. Produits d’ensembles convexes

#### Proposition 5 {#evt-ii-s2-prop-5 .statement}

*L’intersection d’une famille quelconque de parties convexes d’un espace affine E est convexe.*

La proposition est évidente à partir de la déf. 1 de II, p. 8.

#### Proposition 6 {#evt-ii-s2-prop-6 .statement}

*Soit $(E_i)_{i \in I}$ une famille d’espaces vectoriels, et pour chaque $i \in I$, soit $A_i$ une partie non vide de $E_i$. Pour que l’ensemble $A = \prod_{i \in I} A_i$ soit convexe dans $E = \prod_{i \in I} E_i$, il faut et il suffit que, pour tout $i \in I$, l’ensemble $A_i$ soit convexe dans $E_i$.*

En effet, chacune des projections $\mathrm{pr}_i$ est une application linéaire, et on a $A_i = \mathrm{pr}_i A$ et $A = \bigcap_{i \in I} \mathrm{pr}_i^{-1}(A_i)$; la proposition résulte donc des prop. 2 (II, p. 8) et 5.

#### Corollaire {#evt-ii-s2-n2-cor-1 .statement}

*Dans l’espace $\mathbf{R}^n$, tout parallélétope (TG, VI, p. 3) est un ensemble convexe.*

En effet, c’est l’image d’un pavé par une application linéaire affine, et un pavé de $\mathbf{R}^n$ est convexe en vertu de la prop. 6.

#### Proposition 7 {#evt-ii-s2-prop-7 .statement}

Soient E un espace vectoriel, A et B deux parties convexes de E. Quels que soient les nombres réels α et β, l’ensemble αA + βB (ensemble des αx + βy, où x parcourt A et y parcourt B) est convexe.

En effet, αA + βB est l’image de l’ensemble convexe A × B dans E × E par l’application linéaire (x, y) ↦ αx + βy de E × E dans E.

### 3. Enveloppe convexe d’un ensemble

#### Définition 2 {#evt-ii-s2-def-2 .statement}

Étant donnée une partie quelconque A d’un espace affine E, on appelle enveloppe convexe de A l’intersection des ensembles convexes contenant A, c’est-à-dire (II, p. 9, prop. 5) le plus petit ensemble convexe contenant A.

#### Proposition 8 {#evt-ii-s2-prop-8 .statement}

Soit (A_i)_{i∈I} une famille de parties convexes d’un espace affine E ; l’enveloppe convexe de $\bigcup_{i∈I} A_i$ est identique à l’ensemble des combinaisons linéaires $\sum_{i∈I} λ_i x_i$, où $x_i ∈ A_i$, $λ_i ≥ 0$ pour tout $i ∈ I$ ($λ_i = 0$ sauf pour un nombre fini d’indices) et $\sum_{i∈I} λ_i = 1$.

En effet, l’ensemble C de ces combinaisons linéaires est évidemment contenu dans tout ensemble convexe contenant les A_i (II, p. 8, prop. 1), et d’autre part, on a $A_i ⊂ C$ pour tout i ; tout revient à prouver que C est convexe. Soient $x = \sum_i λ_i x_i$, $y = \sum_i μ_i y_i$ deux points de C, et $α$ un nombre tel que $0 < α < 1$; posons $γ_i = αλ_i + (1 - α) μ_i$ pour tout $i ∈ I$, et soit J la partie (finie) de I formée des indices i tels que $γ_i ≠ 0$; on peut écrire
$$
αx + (1 - α)y = \sum_{i∈J} γ_i z_i,
$$
où $z_i = γ_i^{-1}(αλ_i x_i + (1 - α) μ_i y_i)$ appartient à A_i pour tout $i ∈ J$; comme on a $\sum_{i∈J} γ_i = α \sum_{i∈I} λ_i + (1 - α) \sum_{i∈I} μ_i = 1$, le point $αx + (1 - α)y$ appartient à C.

#### Corollaire 1 {#evt-ii-s2-prop-8-cor-1 .statement}

L’enveloppe convexe d’une partie A de E est identique à l’ensemble des combinaisons linéaires $\sum_i λ_i x_i$, où $(x_i)$ est une famille finie quelconque de points de A, $λ_i > 0$ pour tout i et $\sum_i λ_i = 1$.

La dimension de la variété linéaire affine (A, II, p. 129) engendrée par un ensemble convexe A, est encore appelée la dimension de A.

Soit E un espace vectoriel. L’enveloppe convexe C de l’enveloppe équilibrée d’une partie A de E est encore appelée l’enveloppe convexe équilibrée (ou enveloppe convexe symétrique) de A ; il est immédiat que c’est le plus petit ensemble convexe symétrique contenant A ; c’est aussi l’enveloppe convexe de $A ∪ (-A)$, car tout point de l’enveloppe équilibrée de A appartient à un segment d’extrémités a et −a, où $a ∈ A$. L’ensemble C est égal à l’ensemble des combinaisons linéaires $\sum_i λ_i x_i$ où $x_i ∈ A$ et

$$
\sum_i |\lambda_i| \leq 1 ; \text{ il est clair en effet que l’ensemble de ces points est convexe et contient } A \text{ et } -A ; \text{ il suffit donc de prouver qu’il est contenu dans } C, \text{ et pour cela on peut se borner aux combinaisons linéaires telles que } \mu = \sum_i |\lambda_i| > 0 ; \text{ on peut alors écrire }
$$
$$
\sum_i \lambda_i x_i = \mu \cdot \sum_i \alpha_i y_i \text{ avec } \alpha_i = \lambda_i / \mu \text{ et } y_i = x_i \text{ si } \lambda_i \geq 0, \quad \alpha_i = -\lambda_i / \mu \text{ et } y_i = -x_i \text{ si } \lambda_i < 0 ; \text{ il est clair que } \sum_i \alpha_i = 1, \text{ d’où notre assertion.}
$$

#### Corollaire 2 {#evt-ii-s2-prop-8-cor-2 .statement}

*Soient E et F deux espaces affines, f une application linéaire affine de E dans F ; pour toute partie A de E, l’enveloppe convexe de f(A) est l’image par f de l’enveloppe convexe de A.*

On a un énoncé analogue pour les applications linéaires et les enveloppes convexes équilibrées.

### 4. Cônes convexes

#### Définition 3 {#evt-ii-s2-def-3 .statement}

*On dit qu’une partie C d’un espace affine E est un cône de sommet x_0 si C est stable pour toutes les homothéties de centre x_0 et de rapport > 0.*

Nous supposerons, dans ce n° et le suivant, qu’on a choisi comme origine dans E le sommet du cône que l’on considère ; autrement dit, nous supposerons que E est un espace vectoriel, et quand nous parlerons d’un cône, il sera sous-entendu que c’est un cône de sommet 0. On appelle *demi-droite ouverte* (resp. *fermée*) d’origine 0 l’ensemble des points de la forme $\lambda a$ pour $\lambda > 0$ (resp. $\lambda \geq 0$), où $a$ est un vecteur non nul.

Un cône C de sommet 0 est dit *pointé* si $0 \in C$, *épointé* dans le cas contraire. Un cône pointé est, ou bien réduit à 0, ou bien réunion d’un ensemble de demi-droites fermées d’origine 0. Un cône épointé est réunion d’un ensemble (éventuellement vide) de demi-droites ouvertes d’origine 0. Si C est un cône épointé, $C \cup \{0\}$ est un cône pointé. Si C est un cône pointé, $C - \{0\}$ est un cône épointé.

Si C est un cône *convexe* épointé, $C \cup \{0\}$ est un cône convexe pointé. Par contre, si C est un cône convexe pointé, $C - \{0\}$ n’est pas nécessairement convexe. Disons qu’un cône convexe pointé est *saillant* s’il ne contient aucune droite passant par 0. Alors :

#### Proposition 9 {#evt-ii-s2-prop-9 .statement}

*Pour qu’un cône convexe pointé C soit saillant, il faut et il suffit que le cône épointé C’, complémentaire de 0 par rapport à C, soit convexe.*

Si C contient une droite passant par 0, il est évident que C’ n’est pas convexe. Supposons maintenant C saillant, et soient x et y deux points de C’. Le segment fermé d’extrémités x, y est contenu dans C ; s’il contenait 0, on aurait $\lambda x + (1 - \lambda) y = 0$ pour un $\lambda$ tel que $0 < \lambda < 1$, donc $x = \mu y$ avec $\mu < 0$, de sorte que C contiendrait la droite passant par 0 et x, contrairement à l’hypothèse.

#### Proposition 10 {#evt-ii-s2-prop-10 .statement}

*Pour qu’un ensemble C $\subset E$ soit un cône convexe, il faut et il suffit que l’on ait $C + C \subset C$ et $\lambda C \subset C$ pour tout $\lambda > 0$.*

En effet, la condition $\lambda C \subset C$ pour tout $\lambda > 0$ caractérise les cônes. Si $C$ est convexe, on a $C + C = \frac{1}{2}C + \frac{1}{2}C = C$ (II, p. 8, Remarque). Inversement, si le cône $C$ est tel que $C + C \subset C$, on a, pour $0 < \lambda < 1$, $\lambda C + (1 - \lambda)C = C + C \subset C$, ce qui prouve que $C$ est convexe.

#### Corollaire 1 {#evt-ii-s2-prop-10-cor-1 .statement}

*Si C est un cône convexe non vide, le sous-espace vectoriel engendré par C est l’ensemble* $C - C$ (ensemble des $x - y$, où $x$ et $y$ parcourent $C$).

En effet, si $V = C - C$, $V$ est non vide ; on a $\lambda V = V$ pour tout $\lambda \neq 0$, et $V + V = C + C - (C + C) \subset C - C = V$, ce qui montre que $V$ est un sous-espace vectoriel. Tout sous-espace vectoriel contenant $C$ contient évidemment $V$.

#### Corollaire 2 {#evt-ii-s2-prop-10-cor-2 .statement}

*Si C est un cône convexe pointé, le plus grand sous-espace vectoriel contenu dans C est l’ensemble* $C \cap (-C)$.

En effet, si $W = C \cap (-C)$, $W$ est non vide ; on a $\lambda W = W$ pour tout $\lambda \neq 0$, et
$$
W + W \subset (C + C) \cap (-(C + C)) \subset C \cap (-C) = W,
$$
ce qui montre que $W$ est un sous-espace vectoriel. Tout sous-espace vectoriel contenu dans $C$ est évidemment contenu dans $W$.

Il est clair que, si $f$ est une application linéaire de $E$ dans un espace vectoriel $F$, l’image $f(C)$ de tout cône convexe $C$ dans $E$ est un cône convexe dans $F$. Toute intersection de cônes convexes (de sommet 0) dans $E$ est un cône convexe. Pour tout ensemble $A \subset E$, l’intersection de tous les cônes convexes contenant $A$ (il en existe, ne serait-ce que $E$ lui-même) est donc le plus petit cône convexe contenant $A$; on dit que c’est le cône convexe *engendré* par $A$.

#### Proposition 11 {#evt-ii-s2-prop-11 .statement}

*Soit* $(C_i)_{i \in I}$ *une famille de cônes convexes dans* $E$; *le cône convexe engendré par la réunion des* $C_i$ *est identique à l’ensemble des sommes* $\sum_{i \in J} x_i$, *où* $J$ *est une partie finie non vide quelconque de* $I$, *et où* $x_i \in C_i$ *pour tout* $i \in J$.

En effet, l’ensemble $C$ de ces sommes est évidemment un cône convexe contenant la réunion des $C_i$ et contenu dans tout cône convexe contenant cette réunion.

#### Corollaire {#evt-ii-s2-n4-cor-1 .statement}

*Soit* $A$ *une partie de* $E$; *le cône convexe engendré par* $A$ *est identique à l’ensemble des combinaisons linéaires* $\sum_{i \in J} \lambda_i x_i$, *où* $(x_i)_{i \in J}$ *est une famille finie non vide quelconque de points de* $A$, *et où* $\lambda_i > 0$ *pour tout* $i \in J$.

Il suffit de remarquer que, si un cône convexe contient un point $x \in A$, il contient l’ensemble $C_x$ des $\lambda x$, où $\lambda$ parcourt l’ensemble des nombres $> 0$, et que $C_x$ est un cône convexe.

#### Proposition 12 {#evt-ii-s2-prop-12 .statement}

*Soit* $A$ *une partie convexe de* $E$. *Le cône convexe engendré par* $A$ *est identique à* $C = \bigcup_{\lambda > 0} \lambda A$.

L’ensemble $C$ est évidemment un cône ; il suffit de montrer que $C$ est convexe. Soient $\lambda x$ et $\mu y$ deux points de $C$ ($\lambda > 0, \mu > 0, x \in A, y \in A$). Soient $\alpha > 0, \beta > 0$ tels que $\alpha + \beta = 1$. On a $\alpha \lambda x + \beta \mu y = (\alpha \lambda + \beta \mu) z$, avec $z \in A$, et $\alpha \lambda + \beta \mu > 0$; donc $\alpha \lambda x + \beta \mu y \in C$.

#### Remarque 1 {#evt-ii-s2-n4-rem-1 .statement}

Avec les hypothèses de la prop. 12, si $0 \notin A$, le cône $C$ est épointé, donc $C \cup \{0\}$ est saillant.

#### Remarque 2 {#evt-ii-s2-n4-rem-2 .statement}

Soit $A$ un ensemble convexe quelconque dans $E$; considérons, dans l’espace $F = E \times \mathbf{R}$, l’ensemble convexe $A_1 = A \times \{1\}$ et le cône convexe $C$ de sommet 0 engendré par $A_1$. La prop. 12 prouve que $A_1$ est l’intersection de $C$ et de l’hyperplan $E \times \{1\}$ dans $F$. Tout ensemble convexe dans $E$ peut donc être considéré comme la projection sur $E$ de l’intersection d’un cône convexe de sommet 0 dans $F$, et de l’hyperplan $E \times \{1\}$.

### 5. Espaces vectoriels ordonnés

Soit $E$ un espace vectoriel ; on dit qu’une structure de préordre sur $E$, notée $x \leq y$ ou $y \geq x$, est compatible avec la structure d’espace vectoriel de $E$ si elle satisfait aux deux axiomes suivants :

(EO$_1$) *La relation* $x \leq y$ *entraîne* $x + z \leq y + z$ *quel que soit* $z \in E$.

(EO$_2$) *La relation* $x \geq 0$ *entraîne* $\lambda x \geq 0$ *pour tout scalaire* $\lambda \geq 0$.

L’espace vectoriel $E$, muni de ces deux structures, est appelé *espace vectoriel préordonné* (resp. *espace vectoriel ordonné* lorsque la relation de préordre sur $E$ est une relation d’ordre).

On notera que l’axiome (EO$_1$) signifie que la structure de préordre et la structure de groupe additif de $E$ sont compatibles, autrement dit que $E$, muni de ces deux structures, est un *groupe préordonné* (A, VI, p. 3).

#### Exemple {#evt-ii-s2-n5-exa-1 .statement}

Sur l’espace vectoriel $E = \mathbf{R}^A$ de toutes les fonctions numériques finies définies dans un ensemble $A$, la relation d’ordre « quel que soit $t \in A$, $x(t) \leq y(t)$ » est compatible avec la structure d’espace vectoriel de $E$.

#### Proposition 13 {#evt-ii-s2-prop-13 .statement}

(i) *Si* $E$ *est un espace vectoriel préordonné*, *l’ensemble* $P$ *des éléments* $\geq 0$ *de* $E$ *est un cône convexe pointé*.

(ii) *Inversement, soit* $P$ *un cône convexe pointé dans* $E$; *alors la relation* $y - x \in P$ *est une relation de préordre dans* $E$, *et la structure de préordre qu’elle définit sur* $E$ *est la seule qui soit compatible avec la structure d’espace vectoriel de* $E$, *et pour laquelle* $P$ *soit l’ensemble des éléments* $\geq 0$.

(iii) *Pour que le cône convexe pointé* $P$ *soit tel que* $y - x \in P$ *soit une relation d’ordre sur* $E$, *il faut et il suffit que* $P$ *soit saillant*.

(i) Les axiomes (EO$_1$) et (EO$_2$) entraînent $P + P \subset P$ et $\lambda P \subset P$ pour tout $\lambda > 0$, et comme $0 \in P$, $P$ est un cône convexe pointé (II, p. 11, prop. 10).

(ii) Inversement, si $P$ est un cône convexe pointé, la relation $P + P \subset P$ entraîne que la relation $y - x \in P$ est une relation de préordre compatible avec la structure de groupe additif de $E$ (A, VI, p. 3, prop. 3) ; il est clair que si on l’écrit $x \leq y$, l’ensemble $P$ est identique à l’ensemble des $x \geq 0$; en outre, la relation $\lambda P \subset P$ pour tout $\lambda \geq 0$ signifie que l’axiome (EO$_2$) est vérifié.

(iii) Dire que $P$ est saillant signifie que $P \cap (-P) = \{0\}$ (II, p. 12, cor. 2), donc que $y - x \in P$ est une relation d’ordre.

#### Exemple {#evt-ii-s2-n5-exa-2 .statement}

\* Soit H un espace hilbertien réel ; dans l’espace vectoriel $\mathcal{L}(H)$ des endomorphismes continus de H, les endomorphismes hermitiens positifs forment un cône convexe pointé saillant ; ce cône définit donc une structure d’ordre compatible avec la structure d’espace vectoriel de $\mathcal{L}(H)$ et pour laquelle la relation $A \leq B$ signifie que $B - A$ est un endomorphisme hermitien positif. \*

Si P est un cône convexe pointé quelconque dans un espace vectoriel E, $P \cap (-P)$ est un sous-espace vectoriel H de E (II, p. 12, cor. 2). L’image canonique $P'$ de P dans E/H est un cône convexe, et l’image réciproque de $P'$ dans E est P. On a donc $P' \cap (-P') = \{0\}$, et $P'$ définit sur E/H une structure d’ordre compatible avec sa structure d’espace vectoriel.

On dit qu’une forme linéaire $f$ sur un espace vectoriel préordonné E est positive si, pour tout $x \geq 0$ dans E, on a $f(x) \geq 0$. Il revient au même de dire que le cône convexe P des éléments $\geq 0$ de E est contenu dans le demi-espace des $x$ tels que $f(x) \geq 0$. Il est clair que, dans le dual $E^*$ de E, les formes linéaires positives forment un cône convexe pointé.

### 6. Ensembles convexes dans les espaces vectoriels topologiques

#### Proposition 14 {#evt-ii-s2-prop-14 .statement}

Dans un espace vectoriel topologique E, l’adhérence d’un ensemble convexe (resp. d’un cône convexe) est un ensemble convexe (resp. un cône convexe de même sommet).

En effet, soit A un ensemble convexe ; pour tout $\lambda$ tel que $0 < \lambda < 1$, l’application $(x, y) \mapsto \lambda x + (1 - \lambda) y$ est continue dans $E \times E$ et applique $A \times A$ dans A ; donc (TG, I, p. 9, th. 1) elle applique $\overline{A} \times \overline{A}$ dans $\overline{A}$, ce qui démontre que $\overline{A}$ est convexe. On prouve de même que, si C est un cône convexe de sommet 0, on a $\overline{C} + \overline{C} \subset \overline{C}$ et $\lambda \overline{C} \subset \overline{C}$ pour tout $\lambda > 0$.

#### Définition 4 {#evt-ii-s2-def-4 .statement}

Étant donnée une partie quelconque A d’un espace vectoriel topologique E, on appelle enveloppe fermée convexe de A l’intersection des ensembles fermés convexes contenant A, c’est-à-dire le plus petit ensemble fermé convexe contenant A.

D’après la prop. 14, l’enveloppe fermée convexe de A est l’adhérence de l’enveloppe convexe de A ; elle est évidemment identique à l’enveloppe fermée convexe de $\overline{A}$.

On appelle de même enveloppe fermée convexe symétrique (ou enveloppe fermée convexe équilibrée) de A le plus petit ensemble fermé, convexe et symétrique contenant A ; c’est l’adhérence de l’enveloppe convexe symétrique de A (II, p. 10) ; elle est aussi l’enveloppe fermée convexe symétrique de $\overline{A}$.

#### Proposition 15 {#evt-ii-s2-prop-15 .statement}

Dans un espace vectoriel topologique séparé E, soient $A_i$ ($1 \leq i \leq n$) un nombre fini d’ensembles convexes compacts. Alors l’enveloppe convexe de la réunion des $A_i$ est compacte (donc égale à l’enveloppe fermée convexe de cette réunion).

En effet, soit B la partie compacte de $\mathbf{R}^n$ définie par les relations $\lambda_i \geqslant 0$ ($1 \leqslant i \leqslant n$), $\sum_{i=1}^n \lambda_i = 1$. Définissons une application continue de $B \times \prod_{i=1}^n A_i \subset \mathbf{R}^n \times E^n$ dans E, par la formule :

$$
(\lambda_1, \lambda_2, \ldots, \lambda_n, x_1, x_2, \ldots, x_n) \mapsto \sum_{i=1}^n \lambda_i x_i .
$$

L’enveloppe convexe C de $\bigcup_{i=1}^n A_i$ est l’image de $B \times \prod_{i=1}^n A_i$ par cette application ; comme $B \times \prod_{i=1}^n A_i$ est compact et E est séparé, C est compact.

#### Corollaire 1 {#evt-ii-s2-prop-15-cor-1 .statement}

Dans un espace vectoriel topologique séparé E, l’enveloppe convexe d’un ensemble fini est compacte.

#### Corollaire 2 {#evt-ii-s2-prop-15-cor-2 .statement}

Dans un espace vectoriel topologique E, l’enveloppe convexe d’un ensemble fini A est précompacte.

En effet, soit j l’application linéaire canonique de E dans son séparé complété $\hat{E}$; si C est l’enveloppe convexe de A, $j(C)$ est l’enveloppe convexe de l’ensemble fini $j(A)$ dans $\hat{E}$, donc $j(C)$ est compacte (cor. 1), et par suite C est précompacte (TG, II, p. 29).

#### Proposition 16 {#evt-ii-s2-prop-16 .statement}

Dans un espace vectoriel topologique E, soit A un ensemble convexe ayant au moins un point intérieur $x_0$. Si $x \in \overline{A}$, tout point du segment ouvert d’extrémités $x_0$ et x est point intérieur de A.

En effet, soit y un point de ce segment, et soit f l’homothétie de centre y et de rapport $\lambda < 0$ qui transforme $x_0$ en x ; si V est un voisinage ouvert de $x_0$ contenu dans A, $f(V)$ est un voisinage de x, donc contient un point $f(z) \in A$; on a :

$$
f(z) - y = \lambda (z - y) = \lambda (z - f(z)) + \lambda (f(z) - y),
$$

d’où $y - f(z) = \frac{\lambda}{\lambda - 1} (z - f(z))$, de sorte que y est transformé de z par l’homothétie g de centre $f(z)$ et de rapport $\mu = \lambda / (\lambda - 1)$; comme $0 < \mu < 1$, g transforme V en un voisinage de y contenu dans A, d’où la proposition.

#### Corollaire 1 {#evt-ii-s2-prop-16-cor-1 .statement}

L’intérieur $\overset{\circ}{A}$ d’un ensemble convexe A est un ensemble convexe ; si $\overset{\circ}{A}$ n’est pas vide, il est identique à l’intérieur de $\overline{A}$, et $\overline{A}$ est un ensemble convexe identique à l’adhérence de $\overset{\circ}{A}$.

En effet, si $\overset{\circ}{A}$ n’est pas vide, il résulte de la prop. 16 que c’est un ensemble convexe et que tout point de $\overline{A}$ est adhérent à $\overset{\circ}{A}$. Montrons d’autre part que tout point x intérieur à $\overline{A}$ appartient à $\overset{\circ}{A}$. On peut supposer que $x = 0$. Soit V un voisinage symétrique de 0 contenu dans $\overline{A}$, et soit $y \in \overset{\circ}{A} \cap V$; on a $-y \in \overline{A}$, donc, si $y \neq 0$, la prop. 16 montre que $0 \in \overset{\circ}{A}$; la même conclusion est évidente si $y = 0$.

#### Corollaire 2 {#evt-ii-s2-prop-16-cor-2 .statement}

L’intérieur $\dot{C}$ d’un cône convexe est un cône convexe ; si $\dot{C}$ n’est pas vide, il est identique à l’intérieur de $\overline{C}$, et $\overline{C}$ est un cône convexe pointé identique à l’adhérence de $\dot{C}$.

Comme les homothéties de rapport $> 0$ et de centre 0 transforment C en lui-même, elles transforment $\dot{C}$ en lui-même, ce qui montre que $\dot{C}$ est un cône ; le reste du corollaire découle du cor. 1 et de la remarque évidente que si C n’est pas vide, $\overline{C}$ contient le sommet de C.

Soit H un hyperplan fermé dans un espace vectoriel topologique E sur $\mathbf{R}$ ; il a une équation de la forme $f(x) = \alpha$, où $f$ est une forme linéaire continue non nulle dans E (I, p. 13, th. 1). Les demi-espaces définis respectivement par les relations $f(x) \leqslant \alpha$ et $f(x) \geqslant \alpha$ sont donc des ensembles convexes *fermés* ; leurs complémentaires, définis respectivement par les relations $f(x) > \alpha$ et $f(x) < \alpha$, sont des ensembles convexes *ouverts*. On dit que ces demi-espaces sont les demi-espaces fermés (resp. ouverts) *déterminés* par H.

#### Proposition 17 {#evt-ii-s2-prop-17 .statement}

Dans un espace vectoriel topologique E, soit A un ensemble admettant au moins un point intérieur, et dont tous les points sont situés d’un même côté d’un hyperplan H. Alors H est fermé, les points intérieurs à A sont situés strictement d’un même côté de H, et les points adhérents à A sont situés d’un même côté de H. En particulier, les demi-espaces ouverts (resp. fermés) sont ceux qui sont déterminés par les hyperplans fermés.

En effet, supposons que H contienne l’origine, et soit $f(x) = 0$ une équation de H ; supposons par exemple que $f(x) \geqslant 0$ pour tout point $x \in A$. Le demi-espace formé des points y tels que $f(y) > -1$ contient au moins un point intérieur, et par translation on voit qu’il en est de même du demi-espace des points tels que $f(y) > 0$ ; cela prouve que H est fermé (I, p. 11, corollaire). On sait alors que $f$ est un morphisme strict de E sur $\mathbf{R}$ (I, p. 14, corollaire), donc $f(\overline{A})$ est une partie ouverte de $\mathbf{R}$ ; elle ne peut contenir 0, sans quoi elle contiendrait des nombres $< 0$, contrairement à l’hypothèse ; elle est donc contenue dans l’intervalle ouvert ]0, +∞[. D’autre part, le demi-espace des y tels que $f(y) \geqslant 0$ est fermé et contient A, donc il contient $\overline{A}$.

#### Corollaire {#evt-ii-s2-n6-cor-1 .statement}

Soient E un espace vectoriel topologique, P un cône convexe pointé dans E, avant au moins un point intérieur. Alors toute forme linéaire $f \neq 0$ sur E, positive pour la structure de préordre définie par P (II, p. 14), est continue. En outre, on a $f(x) > 0$ lorsque x est intérieur à P, et $f(x) \geqslant 0$ pour tout x adhérent à P.

Il suffit d’appliquer la prop. 16 au cas où A = P et H est l’hyperplan d’équation $f(x) = 0$.

#### Remarque {#evt-ii-s2-n6-rem-1 .statement}

Dans un espace vectoriel topologique E, tout ensemble convexe C est *connexe*. En effet, si $a \in C$, C est réunion de segments fermés d’extrémité $a$, qui sont connexes ; la conclusion résulte de TG, I, p. 81, prop. 2.

### 7. Topologies sur les espaces vectoriels ordonnés

Soit E un espace vectoriel ordonné. On dit qu’une topologie sur E est compatible avec la structure d’espace vectoriel ordonné de E si d’une part elle est compatible avec la structure d’espace vectoriel de E, et si d’autre part elle satisfait à l’axiome suivant :

(TO) Le cône convexe des $x \geqslant 0$ est fermé dans E.

Un espace vectoriel ordonné sur E, muni d’une topologie compatible avec sa structure d’espace vectoriel ordonné, est appelé espace vectoriel topologique ordonné.

#### Exemple {#evt-ii-s2-n7-exa-1 .statement}

L’espace $\mathbf{R}^n$, muni de sa topologie usuelle et de la structure d’ordre produit des structures d’ordre de ses facteurs, est un espace vectoriel topologique ordonné. Par contre, pour $n \geqslant 2$, lorsqu’on munit $\mathbf{R}^n$ de l’ordre lexicographique (E, III, p. 23), la topologie usuelle n’est pas compatible avec la structure d’espace vectoriel ordonné de $\mathbf{R}^n$.

Soit A un ensemble ; l’espace vectoriel $\mathscr{B}(A ; \mathbf{R})$ des fonctions numériques bornées dans A, muni de la topologie définie par la norme $\|x\| = \sup_{t \in A} |x(t)|$ et de la structure d’ordre induite par la structure d’ordre produit sur $\mathbf{R}^A$, est un espace vectoriel topologique ordonné.

Dans un espace vectoriel topologique ordonné E, l’ensemble des éléments $x \leqslant 0$ est fermé ; les translations étant des homéomorphismes, on en déduit que pour tout $a \in E$, l’ensemble des $x \geqslant a$ (resp. $x \leqslant a$) est fermé. Comme les relations $x \geqslant 0$ et $x \leqslant 0$ entraînent $x = 0$, $\{0\}$ est fermé, donc E est séparé.

#### Proposition 18 {#evt-ii-s2-prop-18 .statement}

Dans un espace vectoriel topologique ordonné E, soit H un ensemble filtrant pour la relation $\leqslant$. Si le filtre des sections de H admet une limite dans E, cette limite est la borne supérieure de H.

En effet, soit $b = \lim_{x \in H} x$; pour tout $y \in H$, l’ensemble des $x \in H$ tels que $x \geqslant y$ est un ensemble du filtre des sections de H, donc $b$ est adhérent à cet ensemble ; mais comme l’ensemble des éléments $x \geqslant y$ est fermé dans E, on a $b \geqslant y$, ce qui montre que $b$ est un majorant de H. D’autre part, si $a$ est un majorant de H, H est contenu dans l’ensemble fermé des $z \leqslant a$; comme $b$ est adhérent à H, on a $b \leqslant a$, ce qui achève la démonstration (II, p. 76, exerc. 42).

### 8. Fonctions convexes

#### Définition 5 {#evt-ii-s2-def-5 .statement}

Soient E un espace affine, X une partie convexe de E. On dit qu’une fonction numérique finie, définie dans X, est convexe (resp. strictement convexe) si, quels que soient $x, y$ distincts dans X et le nombre réel $\lambda$ tel que $0 < \lambda < 1$, on a :

(1) $$ f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) $$

(resp.

(2) $$ f(\lambda x + (1 - \lambda) y) < \lambda f(x) + (1 - \lambda) f(y)) . $$)

Lorsque $E = \mathbf{R}$, cette définition des fonctions convexes n’est autre que celle de FVR, I, p. 32. En outre, pour que $f$ soit convexe (resp. strictement convexe) dans $X$, il faut et il suffit que pour toute droite affine $D \subset E$, la restriction de $f$ à $X \cap D$ soit convexe (resp. strictement convexe) dans $X \cap D$.

#### Exemple {#evt-ii-s2-n8-exa-1 .statement}

Pour toute fonction linéaire affine $f$ sur $E$, $f$ et $f^2$ sont des fonctions convexes dans $E$; c’est évident pour $f$, puisque

$$
f(\lambda x + (1 - \lambda) y) = \lambda f(x) + (1 - \lambda) f(y);
$$

d’autre part, si l’on pose $\alpha = f(x)$, $\beta = f(y)$, on a :

$$
\lambda \alpha^2 + (1 - \lambda) \beta^2 - (\lambda \alpha + (1 - \lambda) \beta)^2 = \lambda(1 - \lambda) (\alpha - \beta)^2 \geqslant 0
$$

pour $0 < \lambda < 1$; on voit ainsi en outre que la restriction de $f^2$ à une droite affine $D \subset E$ est strictement convexe si $f|D$ n’est pas constante.

On dit qu’une fonction numérique finie $f$ définie dans $X$ est concave (resp. strictement concave) si – $f$ est convexe (resp. strictement convexe). Il revient au même de dire que pour tout couple $x, y$ de points distincts dans $X$ et tout nombre $\lambda$ tel que $0 < \lambda < 1$, on a

$$
f(\lambda x + (1 - \lambda) y) \geqslant \lambda f(x) + (1 - \lambda) f(y)
$$

(resp.

$$
f(\lambda x + (1 - \lambda) y) > \lambda f(x) + (1 - \lambda) f(y)).
$$

On dit qu’une application de $X$ dans $\mathbf{R}$ est affine si elle est à la fois convexe et concave (cf. II, p. 83, exerc. 11).

#### Proposition 19 {#evt-ii-s2-prop-19 .statement}

Soient $E$ un espace affine, $X$ une partie convexe de $E$; soient $f$ une fonction numérique finie définie dans $X$, $F$ (resp. $F'$) l’ensemble des points $(x, a) \in E \times \mathbf{R}$ tels que $x \in X$ et $f(x) \leqslant a$ (resp. $x \in X$ et $f(x) < a$). Alors les conditions suivantes sont équivalentes :

a) La fonction $f$ est convexe.
b) L’ensemble $F$ est convexe dans l’espace affine $E \times \mathbf{R}$.
c) L’ensemble $F'$ est convexe dans l’espace affine $E \times \mathbf{R}$.

Montrons que a) implique c). Supposons $f$ convexe ; si $(x, a)$ et $(y, b)$ sont deux points de $F'$ et $0 < \lambda < 1$, on a $f(x) < a, f(y) < b$ et

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) < \lambda a + (1 - \lambda) b
$$

ce qui exprime que le point $\lambda(x, a) + (1 - \lambda)(y, b)$ de $E \times \mathbf{R}$ appartient à $F'$. Donc $F'$ est convexe.

Montrons en second lieu que c) entraîne b). En effet, si $(x, a), (y, b)$ sont deux points de $F$ et $0 < \lambda < 1$, les points $(x, a + \varepsilon)$ et $(y, b + \varepsilon)$ appartiennent à $F'$ pour tout $\varepsilon > 0$, et par suite il en est de même de

$$
(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b + \varepsilon);
$$

par définition de $F$, cela entraîne que $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ appartient à $F$.

Enfin, b) entraîne a), car (avec les mêmes notations), dire que le point $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ appartient à F signifie que l’on a :

$$
f(\lambda x + (1 - \lambda) y) \leq \lambda a + (1 - \lambda) b
$$

quels que soient $a \geq f(x)$ et $b \geq f(y)$; on en conclut que l’on a l’inégalité (1), donc $f$ est convexe.

#### Corollaire {#evt-ii-s2-n8-cor-1 .statement}

*Si $f$ est convexe dans X, alors, pour tout $\alpha \in \mathbf{R}$, l’ensemble des $x \in X$ tels que $f(x) \leq \alpha$ (resp. $f(x) < \alpha$) est convexe.*

En effet, c’est la projection sur E de l’intersection de F (resp. F’) et de l’hyperplan $E \times \{ \alpha \}$ dans $E \times \mathbf{R}$.

#### Proposition 20 {#evt-ii-s2-prop-20 .statement}

*Soit $f$ une fonction convexe dans une partie convexe X d’un espace affine E. Pour toute famille finie $(x_i)_{1 \leq i \leq p}$ de p points de X, et toute famille $(\lambda_i)_{1 \leq i \leq p}$ de p nombres réels $\geq 0$ tels que $\sum_{i=1}^p \lambda_i = 1$, on a :

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i) .
$$

*Si $f$ est strictement convexe et si $\lambda_i > 0$ pour tout i, on a :*

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i) ,
$$

sauf si tous les $x_i$ sont égaux.

L’inégalité (3) résulte de II, p. 18, prop. 19 et p. 8, prop. 1. Supposons que les $x_i$ ne soient pas tous égaux (ce qui implique $p \geq 2$) et que les $\lambda_i$ soient tous $> 0$; alors le point $z = \sum_{i=1}^p \lambda_i x_i$ ne peut être égal à tous les $x_i$. Supposons par exemple $z \neq x_1$, et posons $z = \lambda_1 x_1 + (1 - \lambda_1) y_1$ avec $y_1 = \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} x_i$. On a donc $y_1 \neq x_1$ et comme $0 < \lambda_1 < 1$, on a par hypothèse

$$
f(z) < \lambda_1 f(x_1) + (1 - \lambda_1) f(y_1) .
$$

Mais en vertu de (3) on a $f(y_1) \leq \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} f(x_i)$, d’où l’inégalité (4).

### 9. Opérations sur les fonctions convexes

Soit X une partie convexe d’un espace affine E. Si $f_i$ ($1 \leq i \leq p$) sont des fonctions convexes dans X en nombre fini, et $c_i$ ($1 \leq i \leq p$) des nombres $\geq 0$, la fonction $f = \sum_{i=1}^p c_i f_i$ est convexe dans X.

Si $(f_\alpha)$ est une famille quelconque de fonctions convexes dans $X$, et si l’enveloppe supérieure $g$ de cette famille est finie dans $X$, alors $g$ est convexe.

Enfin, si $H$ est un ensemble de fonctions convexes dans $X$, et $\mathfrak{F}$ un filtre sur $H$ qui converge simplement dans $X$ vers une fonction numérique finie $f_0$, $f_0$ est convexe dans $X$.

### 10. Fonctions convexes dans un ensemble convexe ouvert

#### Proposition 21 {#evt-ii-s2-prop-21 .statement}

*Soient E un espace vectoriel topologique, X une partie convexe ouverte non vide de E, f une fonction convexe définie dans X. Pour que f soit continue, il faut et il suffit qu’il existe une partie ouverte non vide U de X dans laquelle f soit majorée.*

La condition étant évidemment nécessaire, prouvons qu’elle est suffisante. Soit $x_0 \in X$ un point tel que $f$ soit majorée dans un voisinage $V$ de $x_0$; montrons d’abord que $f$ est continue au point $x_0$. Par translation, on peut se borner au cas où $x_0 = 0$ et $f(x_0) = 0$; en outre, on peut supposer le voisinage $V$ équilibré (I, p. 7, prop. 4). Supposons que $f(x) \leq a$ dans $V$; pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, remarquons que, si $x \in \varepsilon V$, on a $x/\varepsilon \in V$ et $-x/\varepsilon \in V$. L’inégalité (1) de II, p. 17 appliquée aux points $x/\varepsilon$ et $0$ et au nombre $\lambda = \varepsilon$, montre que $f(x) \leq \varepsilon f(x/\varepsilon) \leq \varepsilon a$; appliquée aux points $x$ et $-x/\varepsilon$ et au nombre $\lambda = 1/(1 + \varepsilon)$, elle donne l’inégalité $f(x) \geq -\varepsilon f(-x/\varepsilon) \geq -\varepsilon a$, ce qui prouve que $f(x)$ est arbitrairement petit dans $\varepsilon V$ lorsque $\varepsilon$ est assez petit.

Soit maintenant $y$ un point de $X$; il existe un nombre $\rho > 1$ tel que $z = \rho y$ appartienne encore à $X$ puisque $X$ est ouvert. Soit $g$ l’homothétie $x \mapsto \lambda x + (1 - \lambda) z$ de centre $z$ et de rapport $\lambda = 1 - \frac{1}{\rho}$, qui transforme $0$ en $y$; pour tout point $g(x) \in g(V)$, on a, d’après (1), $f(g(x)) \leq \lambda f(x) + (1 - \lambda) f(z) \leq \lambda a + (1 - \lambda) f(z)$. La première partie du raisonnement montre donc que $f$ est continue au point $y$, ce qui achève la démonstration.

#### Corollaire {#evt-ii-s2-n10-cor-1 .statement}

*Toute fonction convexe f définie dans une partie convexe ouverte X de $\mathbf{R}^n$ est continue dans X.*

On peut supposer $X$ non vide. Il existe alors, dans $X$, $n + 1$ points affinement indépendants $a_i$ ($0 \leq i \leq n$), et l’enveloppe convexe $S$ de ces points contient l’ensemble ouvert non vide formé des $\sum_{i=0}^n \lambda_i a_i$ avec $0 < \lambda_i < 1$ pour tout $i$ et $\sum_{i=0}^n \lambda_i = 1$. En vertu de II, p. 19, prop. 20, $f$ est majorée dans $S$, d’où la conclusion du corollaire.

Sur un espace vectoriel topologique de dimension infinie, il existe en général des formes linéaires non continues (II, p. 85, exerc. 25) et par suite des fonctions convexes qui ne sont continues en aucun point.

### 11. Semi-normes et ensembles convexes

Soit E un espace vectoriel sur $\mathbf{R}$; on dit qu’une application $p$ de E dans $\mathbf{R}$ est positivement homogène si, pour tout $\lambda \geqslant 0$, et tout $x \in E$ on a :

$$
p(\lambda x) = \lambda p(x) .
$$

Pour qu’une fonction positivement homogène $p$ dans E soit convexe, il faut et il suffit qu’elle satisfasse à l’axiome (SN_{II}) de II, p. 1 :

$$
p(x + y) \leqslant p(x) + p(y)
$$

quels que soient $x, y$ dans E.
En effet, si $p$ est convexe, on a, pour $x, y$ dans E,

$$
p\left( \frac{1}{2}(x + y) \right) \leqslant \frac{1}{2} p(x) + \frac{1}{2} p(y)
$$

et en vertu de (5), cette relation est équivalente à (6). Inversement, si la relation (6) a lieu, on a aussi, quel que soit $\lambda$ tel que $0 < \lambda < 1$,

$$
p(\lambda x + (1 - \lambda) y) \leqslant p(\lambda x) + p((1 - \lambda) y) = \lambda p(x) + (1 - \lambda) p(y)
$$

en vertu de (5).

On appelle fonction sous-linéaire sur E une fonction convexe et positivement homogène.

Soit $p$ une fonction sous-linéaire dans E ; en vertu de II, p. 19, corollaire, pour tout $a > 0$, l’ensemble $V(p, a)$ (resp. $W(p, a)$) des $x \in E$ tels que $p(x) \leqslant a$ (resp. $p(x) < a$) est un ensemble convexe ; en outre, cet ensemble est absorbant, car pour tout $x \in E$, il existe $\lambda > 0$ tel que $p(\lambda x) = \lambda p(x) < a$.

On a une réciproque partielle de ce résultat :

#### Proposition 22 {#evt-ii-s2-prop-22 .statement}

Soient E un espace vectoriel, A un ensemble convexe dans E, contenant 0. Pour tout $x \in E$, posons

$$
p_A(x) = \inf_{\rho > 0, x \in \rho A} \rho
$$

(élément de $[0, + \infty)$). La fonction $p_A$ vérifie les relations

$$
p_A(x + y) \leqslant p_A(x) + p_A(y) , \quad p_A(\lambda x) = \lambda p_A(x)
$$

quels que soient $x, y$ dans E et $\lambda > 0$. Si $V(p_A, \alpha)$ (resp. $W(p_A, \alpha)$) désigne l’ensemble des $x \in E$ tels que $p_A(x) \leqslant \alpha$ (resp. $p_A(x) < \alpha$), on a

$$
W(p_A, 1) \subset A \subset V(p_A, 1) .
$$

Si A est absorbant, $p_A$ est finie (donc sous-linéaire).

Comme les relations $x \in \rho A$ et $\lambda x \in \lambda \rho A$ sont équivalentes pour $\lambda > 0$, on a $p_A(\lambda x) = \lambda p_A(x)$ pour $\lambda > 0$. Soient $x, y$ deux points de E. Alors l’inégalité $p_A(x + y) \leq p_A(x) + p_A(y)$ est évidente si $x$ (resp. $y$) n’est pas absorbé par A, car alors $p_A(x) = +\infty$ (resp. $p_A(y) = +\infty$). Supposons donc qu’il existe deux nombres $\alpha > 0, \beta > 0$ tels que $x \in \alpha A, y \in \beta A$; on a $x + y \in \alpha A + \beta A = (\alpha + \beta) A$ (II, p. 8, Remarque) ; on a par suite $p_A(x + y) \leq p_A(x) + p_A(y)$. L’inclusion $A \subset V(p_A, 1)$ est évidente. L’inclusion $W(p_A, 1) \subset A$ résulte de ce que A est convexe et contient 0. Enfin, si A est absorbant, il est clair que $p_A$ est finie.

On dit que la fonction $p_A$ définie par (7) est la jauge de l’ensemble convexe A. Si A est absorbant et symétrique, $p_A$ est donc une semi-norme.

#### Proposition 23 {#evt-ii-s2-prop-23 .statement}

*Soit E un espace vectoriel topologique. Si A est un ensemble convexe ouvert contenant 0, $p_A$ est finie et continue et $A = W(p_A, 1)$. Si A est un ensemble convexe fermé contenant 0, $p_A$ est semi-continue inférieurement et l’on a $A = V(p_A, 1)$.

Si A est ouvert et contient 0 (donc est absorbant), pour tout $x \in A$, il existe $\rho < 1$ tel que $x/\rho \in A$, donc $p_A(x) < 1$, ce qui, joint à (9), montre que $A = W(p_A, 1)$. La fonction convexe $p_A$ étant majorée dans l’ensemble ouvert A est continue dans E (II, p. 20, prop. 21).

Si A est fermé et contient 0, pour tout $x \in E$ tel que $p_A(x) \leq 1$, on a $x \in \rho A$ pour tout $\rho > 1$, donc aussi $x \in A$ puisque A est fermé ; tenant compte de (9), cela prouve que $A = V(p_A, 1)$. Pour tout $\mu > 0$, $\mu A$ est donc l’ensemble des $x$ tels que $p_A(x) \leq \mu$ ; comme $p_A(x) \geq 0$ dans E, cela montre que $p_A$ est semi-continue inférieurement dans E (TG, IV, p. 29).

On notera que pour toute fonction sous-linéaire $p$ dans E à valeurs positives, $p$ est la jauge de tout ensemble convexe A tel que $W(p, 1) \subset A \subset V(p, 1)$.

## EXERCICES {#evt-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
