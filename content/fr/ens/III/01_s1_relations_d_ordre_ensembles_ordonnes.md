---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 1
section_title: Relations d’ordre. Ensembles ordonnés
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0105-0119, 0173-0178
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une relation d’ordre
      page: 0
      pdf_page: 105
    - "no": 2
      title: Relations de préordre
      page: 2
      pdf_page: 106
    - "no": 3
      title: Notations et terminologie
      page: 4
      pdf_page: 108
    - "no": 4
      title: Sous-ensembles ordonnés. Produit d'ensembles ordonnés
      page: 5
      pdf_page: 109
    - "no": 5
      title: Applications croissantes
      page: 7
      pdf_page: 111
    - "no": 6
      title: Éléments maximaux et éléments minimaux
      page: 8
      pdf_page: 112
    - "no": 7
      title: Plus grand élément; plus petit élément
      page: 8
      pdf_page: 112
    - "no": 8
      title: Majorants; minorants
      page: 9
      pdf_page: 113
    - "no": 9
      title: Borne supérieure; borne inférieure
      page: 10
      pdf_page: 114
    - "no": 10
      title: Ensembles filtrants
      page: 12
      pdf_page: 116
    - "no": 11
      title: Ensembles réticulés
      page: 13
      pdf_page: 117
    - "no": 12
      title: Ensembles totalement ordonnés
      page: 13
      pdf_page: 117
    - "no": 13
      title: Intervalles
      page: 14
      pdf_page: 118
statements: 50
exercises: 24
content_sha256: 17956b1a02fee70c6291e5281349e67b3533a7e336fa3ffef8ad9c4cfa05fac5
---

## § 1. RELATIONS D’ORDRE.. ENSEMBLES ORDONNÉS

### 1. Définition d’une relation d’ordre

Soit R$x, y$ une relation, $x$ et $y$ étant des lettres distinctes. On dit que R est une *relation d’ordre par rapport aux lettres x et y* (ou *entre x et y*) si les relations

$$
(R(x, y) \text{ et } R(y, z)) \Rightarrow R(x, z)
$$
$$
(R(x, y) \text{ et } R(y, x)) \Rightarrow (x = y)
$$
$$
R(x, y) \Rightarrow (R(x, x) \text{ et } R(y, y))
$$

sont vraies. La première exprime que la relation R est *transitive* par rapport aux lettres $x$ et $y$ (II, p. 40).

*Exemples*

1) La *relation d’égalité* $x = y$ est une relation d’ordre.
2) La relation $X \subset Y$ est une relation d’ordre entre X et Y (II, p. 2, prop. 1 et 2 et axiome A1), que l’on appelle souvent *relation d’inclusion*, ou *relation $\subset$*.
3) Soit R$x, y$ une relation d’ordre entre $x$ et $y$. La relation R$y, x$ est une relation d’ordre *entre x et y*, appelée relation d’ordre *opposée* à R$x, y$.

On appelle *relation d’ordre dans un ensemble* E une relation d’ordre R$x, y$ par rapport à deux lettres distinctes $x, y$ (ne figurant pas dans le terme E de la théorie où l’on s’est placé) telle que la relation R$x, x$ soit *équivalente à* $x \in E$ (autrement dit, telle que R$x, y$ soit *réflexive dans* E (II, p. 40)). Alors la relation R$x, y$ implique « $x \in E$ et $y \in E$ » et la relation (R$x, y$ et R$y, x$) est équivalente à « $x \in E$ et $y \in E$ et $x = y$ ».

#### Exemple 1 {#ens-iii-s1-n1-exa-1 .statement tag=03SH}

La relation d’égalité et la relation d’inclusion ne sont pas des relations d’ordre dans un ensemble, car les relations $x = x$ et $X \subset X$ ne sont pas collectivisantes (II, p. 6).

#### Exemple 2 {#ens-iii-s1-n1-exa-2 .statement tag=03SI}

Soient $R\{x, y\}$ une relation d’ordre entre $x$ et $y$, et $E$ un ensemble tel que $x \in E$ entraîne $R\{x, x\}$ (on notera que l’ensemble vide satisfait à cette condition). La relation « $R\{x, y\}$ et $x \in E$ et $y \in E$ » est alors une relation d’ordre dans $E$, comme on le vérifie aussitôt; on dit que c’est la relation d’ordre *induite* par $R\{x, y\}$ dans $E$ (cf. III, p. 5). Par abus de langage, on dira souvent « la relation $S\{x, y\}$ est une relation d’ordre entre éléments de $E$ » au lieu de dire « la relation ($S\{x, y\}$ et $x \in E$ et $y \in E$) est une relation d’ordre dans $E$ ». Par exemple, étant donné un ensemble $A$, la relation « $X \subset Y$ et $X \subset A$ et $Y \subset A$ » est une relation d’ordre entre parties de $A$.

#### Exemple 3 {#ens-iii-s1-n1-exa-3 .statement tag=03SJ}

Soient $E$ et $F$ des ensembles. La relation « $g$ prolonge $f$ » est une relation d’ordre (entre $f$ et $g$) dans l’ensemble des applications de parties de $E$ dans $F$.

#### Exemple 4 {#ens-iii-s1-n1-exa-4 .statement tag=03V3}

Dans l’ensemble $\mathcal{P}(\mathcal{P}(E))$ des ensembles de parties d’un ensemble $E$, soit $\mathcal{P}$ l’ensemble des *partitions* de $E$ (II, p. 29). Rappelons qu’une partition $\varpi$ est dite *moins fine* qu’une partition $\varpi'$ si, quel que soit $Y \in \varpi'$, il existe $X \in \varpi$ tel que $Y \subset X$ (II, p. 27). Pour toute partition $\varpi \in \mathcal{P}$, soit $\tilde{\varpi}$ le graphe de l’équivalence définie par $\varpi$ dans $E$ (II, p. 42), c’est-à-dire la réunion des ensembles (mutuellement disjoints) $A \times A$, où $A$ parcourt $\varpi$. La relation « $\varpi$ est moins fine que $\varpi'$ » est équivalente à $\tilde{\varpi} \supset \tilde{\varpi}'$, comme on le voit immédiatement; c’est donc une relation d’ordre dans l’ensemble $\mathcal{P}$, entre $\varpi$ et $\varpi'$.

On appelle *ordre* sur un ensemble $E$ une correspondance $\Gamma = (G, E, E)$ ayant $E$ comme ensemble de départ et ensemble d’arrivée et telle que la relation $(x, y) \in G$ soit une relation d’ordre dans $E$. Par abus de langage, on dira parfois que le graphe $G$ de $\Gamma$ est un ordre sur $E$. Si $R\{x, y\}$ est une relation d’ordre dans $E$, elle admet un graphe, qui est un ordre sur $E$.

#### Proposition 1 {#ens-iii-s1-prop-1 .statement tag=03JA}

*Pour qu’une correspondance $\Gamma$ entre $E$ et $E$ soit un ordre sur $E$, il faut et il suffit que son graphe $G$ satisfasse aux conditions suivantes*:

a) *On a* $G \circ G = G$.

b) *L’ensemble* $G \cap \overline{G}^{-1}$ *est la diagonale* $\Delta$ *de* $E \times E$.

En effet, la relation $((x, y) \in G$ et $(y, z) \in G) \Rightarrow ((x, z) \in G)$ s’écrit aussi $G \circ G \subset G$, et la relation

$$
((x, y) \in G \text{ et } (y, x) \in G) \Leftrightarrow (x = y \text{ et } x \in E \text{ et } y \in E)
$$

s’écrit $G \cap \overline{G}^{-1} = \Delta$. De $G \cap \overline{G}^{-1} = \Delta$, on déduit alors $\Delta \subset G$; d’où

$$
G = \Delta \circ G \subset G \circ G,
$$

ce qui, compte tenu de $G \circ G \subset G$, entraîne $G \circ G = G$.

### 2. Relations de préordre

Soit $R\{x, y\}$ une relation, $x$ et $y$ étant des lettres distinctes. Si $R$ est transitive et si l’on a

$$
R\{x, y\} \Rightarrow (R\{x, x\} \text{ et } R\{y, y\}),
$$

$R$ n’est pas nécessairement une relation d’ordre, car la relation $(R\{x, y\}$ et $R\{y, x\})$ n’entraîne pas nécessairement $x = y$. On dit que $R\{x, y\}$ est une *relation de préordre* entre $x$ et $y$; $R \{ y, x \}$ est alors une relation de préordre entre $x$ et $y$, dite *opposée* à $R \{ x, y \}$.

Par exemple, soit $\mathcal{R}$ l’ensemble des parties de $\mathfrak{P}(E)$ qui sont des recouvrements de $E$ (II, p. 27). La relation « $\mathfrak{R}$ est moins fin que $\mathfrak{R}'$ » entre éléments $\mathfrak{R}, \mathfrak{R}'$ de $\mathcal{R}$ (II, p. 27) est transitive et réflexive, mais deux recouvrements distincts peuvent être tels que chacun soit moins fin que l’autre. Il en est par exemple ainsi lorsque $\mathfrak{R}'$ est (dans $\mathfrak{P}(E)$) réunion de $\mathfrak{R}$ et d’une partie de $E$ contenue dans un ensemble de $\mathfrak{R}$, mais n’appartenant pas à $\mathfrak{R}$.

Mais en tout cas la relation $(R \{ x, y \}$ et $R \{ y, x \} )$ est une *relation d’équivalence* $S \{ x, y \}$ par rapport à $x$ et $y$. Soient $x'$ et $y'$ des lettres distinctes de $x, y$ et ne figurant pas dans $R$; alors $R \{ x, y \}$ est *compatible* (par rapport à $x$ et $y$) avec les relations d’équivalence $S \{ x, x' \}$ et $S \{ y, y' \}$; autrement dit (II, p. 42) la relation $(R \{ x, y \}$ et $S \{ x, x' \}$ et $S \{ y, y' \} )$ entraîne $R \{ x', y' \}$.

On appelle *relation de préordre dans un ensemble* $E$ une relation de préordre $R \{ x, y \}$ telle que la relation $R \{ x, x \}$ soit équivalente à $x \in E$ (les lettres $x, y$ ne figurant pas dans le terme $E$); la relation $R \{ x, y \}$ implique alors « $x \in E$ et $y \in E$ ». Si $R \{ x, y \}$ est une relation de préordre dans un ensemble $E$, la relation $S \{ x, y \}$ définie ci-dessus est une relation d’équivalence dans $E$. Soit alors $R' \{ X, Y \}$ la relation

$$
X \in E/S \text{ et } Y \in E/S \text{ et } (\exists x)(\exists y)\,(x \in X \text{ et } y \in Y \text{ et } R \{ x, y \})
$$

c’est-à-dire la relation déduite de $R$ par passage au quotient (par rapport à $x$ et $y$); on a vu (II, p. 43), qu’elle est équivalente à la relation

$$
X \in E/S \text{ et } Y \in E/S \text{ et } (\forall x)(\forall y)\,((x \in X \text{ et } y \in Y) \Rightarrow R \{ x, y \}).
$$

Montrons que $R' \{ X, Y \}$ est une *relation d’ordre* entre éléments de $E/S$. En effet, la relation $(R' \{ X, Y \}$ et $R' \{ Y, Z \} )$ est équivalente à

$X \in E/S$ et $Y \in E/S$ et $Z \in E/S$ et

$$
(\forall x)(\forall y)(\forall z)((x \in X \text{ et } y \in Y \text{ et } z \in Z) \Rightarrow (R \{ x, y \} \text{ et } R \{ y, z \}))
$$

(I, p. 37, critères C40 et C41); comme $R \{ x, y \}$ est transitive et que $Y \in E/S$ entraîne $Y \neq \varnothing$ (II, p. 41), on en déduit aussitôt que $R' \{ X, Y \}$ est transitive. En second lieu, $(R' \{ X, Y \}$ et $R' \{ Y, X \} )$ est équivalente à

$$
X \in E/S \text{ et } Y \in E/S \text{ et } (\forall x)(\forall y)\,((x \in X \text{ et } y \in Y) \Rightarrow (R \{ x, y \} \text{ et } R \{ y, x \}))
$$

c’est-à-dire à

$$
X \in E/S \text{ et } Y \in E/S \text{ et } (\forall x)(\forall y)\,((x \in X \text{ et } y \in Y) \Rightarrow S \{ x, y \})
$$

donc elle entraîne

$$
X \in E/S \text{ et } Y \in E/S \text{ et } X = Y.
$$

Par ailleurs, $R \{ x, y \}$ entraîne $R \{ x, x \}$ et $R \{ y, y \}$, d’où résulte que $R' \{ X, Y \}$ entraîne chacune des relations

$$
X \in E/S \text{ et } (\forall x)((x \in X) \Rightarrow R \{ x, x \})
$$
$$
Y \in E/S \text{ et } (\forall y)((y \in Y) \Rightarrow R \{ y, y \})
$$

donc $R' \{ X, Y \}$ entraîne $(R' \{ X, X \}$ et $R' \{ Y, Y \} )$. Enfin, comme $x \in E$ entraîne $R \{ x, x \}$, $X \in E/S$ entraîne $R' \{ X, X \}$, ce qui achève de démontrer notre assertion. On dit que $R' \{ X, Y \}$ est la relation d’ordre *associée* à $R \{ x, y \}$.

On appelle *préordre* sur un ensemble $E$ une correspondance $\Gamma = (G, E, E)$ ayant $E$ comme ensemble de départ et ensemble d’arrivée, et telle que $(x, y) \in G$ soit une relation de préordre dans $E$; par abus de langage, on dit parfois que le graphe $G$ de $\Gamma$ est un préordre sur $E$. Pour qu’il en soit ainsi, il faut et il suffit que l’on ait $\Delta \subset G$ et $G \circ G \subset G$ (ce qui entraîne $G \circ G = G$). La relation d’équivalence $S$ correspondant à la relation de préordre $(x, y) \in G$ a alors pour graphe $G \cap \overline{G}^1$; la relation d’ordre associée à $(x, y) \in G$ a pour graphe la partie $G'$ de $(E/S) \times (E/S)$ qui correspond (II, p. 47) à l’image de $G$ par l’application canonique de $E \times E$ sur $(E \times E)/(S \times S)$.

#### Exemple {#ens-iii-s1-n2-exa-1 .statement tag=03JB}

*Soit $A$ un anneau ayant un élément unité. La relation $(\exists z)(z \in A \text{ et } y = zx)$ entre deux éléments $x$ et $y$ de $A$ est une relation de préordre dans $A$; elle se lit « $x$ est diviseur à droite de $y$ » ou « $y$ est multiple à gauche de $x$ » (cf. A, I, § 8, no 1 et A, VI, § 1).* \*

### 3. Notations et terminologie

Les définitions qui vont être données dans le reste de ce paragraphe s’appliquent à une relation d’ordre (ou de préordre) quelconque $R \{ x, y \}$ entre $x$ et $y$, mais seront surtout utilisées dans le cas où $R \{ x, y \}$ est notée $x \leq y$* (par analogie avec la relation d’ordre usuelle entre entiers ou nombres réels)* (ou $x \subset y$, ou par un signe analogue); aussi les énoncerons-nous uniquement dans la notation $x \leq y$, laissant au lecteur le soin de les étendre à d’autres cas. Lorsque $R \{ x, y \}$ est notée $x \leq y$, on considère que $y \geq x$ est synonyme de $x \leq y$, et ces relations se lisent « $x$ est *inférieur à* $y$ », ou « $x$ est *plus petit que* $y$ », ou « $y$ est *supérieur à* $x$ », ou « $y$ est *plus grand que* $x$ » (ou parfois « $x$ est *au plus égal à* $y$ », ou « $y$ est *au moins égal à* $x$ »). La relation $x \geq y$ est alors la relation de préordre (*entre* $x$ *et* $y$) *opposée* à $x \leq y$.

Par abus de langage, on parlera souvent de la « relation $\leq$ » au lieu de « la relation $x \leq y$ »; dans ce cas « la relation $\geq$ » sera l’opposée de « la relation $\leq$ ». Observons aussi que, dans une même démonstration, on utilisera souvent le même signe $\leq$ pour noter plusieurs relations d’ordre distinctes, lorsqu’il n’en résulte pas de confusion.

Les conditions pour qu’une relation notée $x \leq y$ soit une relation d’ordre dans un ensemble $E$ s’écrivent:

(RO$_I$) *La relation* « $x \leq y$ et $y \leq z$ » *entraîne* $x \leq z$.
(RO$_{II}$) *La relation* « $x \leq y$ et $y \leq x$ » *entraîne* $x = y$.
(RO$_{III}$) *La relation* $x \leq y$ *entraîne* « $x \leq x$ et $y \leq y$ ».
(RO$_{IV}$) *La relation* $x \leq x$ *est équivalente* à $x \in E$.

Si on omet la condition (RO$_{II}$), on obtient les conditions pour que $x \leq y$ soit une relation de préordre dans $E$.

Lorsqu'une relation d'ordre est notée $x \leq y$, nous écrirons $x < y$ (ou $y > x$) la relation « $x \leq y$ et $x \neq y$ »; ces relations se lisent « $x$ est strictement inférieur à $y$ » ou « $x$ est strictement plus petit que $y$ » ou « $y$ est strictement supérieur à $x$ » ou « $y$ est strictement plus grand que $x$ ».

L'exemple de la relation d'inclusion montre que la négation de $x \leq y$ (qu'on note parfois $x \not\leq y$) n'est pas nécessairement équivalente à $y < x$ (cf. III, p. 14).

C58. Soient $\leq$ une relation d'ordre, $x$ et $y$ deux lettres distinctes. La relation $x \leq y$ est équivalente à « $x < y$ ou $x = y$ ». Chacune des relations « $x \leq y$ et $y < z$ », « $x < y$ et $y \leq z$ » entraîne $x < z$.

La première assertion résulte du critère

$$
A \Rightarrow ((A \text{ et } (\text{non } B)) \text{ ou } B)
$$

(I, p. 31, critère C24). Pour démontrer la seconde, on remarque d'abord que chacune des hypothèses entraîne $x \leq z$, d'après la transitivité; d'autre part, la relation ($x = z$ et $x \leq y$ et $y \leq z$) entraînerait $x = y = z$, ce qui est contraire à l'hypothèse.

Afin de rendre l'exposé plus commode, et de remplacer par des théorèmes mathématiques les critères métamathématiques, nous allons le plus souvent nous placer dans une théorie $\mathcal{T}$, comprenant les axiomes et schémas d'axiomes de la théorie des ensembles, et en outre deux constantes $E$ et $\Gamma$ satisfaisant à l'axiome:

« $\Gamma$ est un ordre sur l'ensemble $E$ » (III, p. 2).

Nous noterons $x \leq y$ la relation $y \in \Gamma \langle x \rangle$, et nous dirons que $E$ est un ensemble ordonné par l'ordre $\Gamma$ (ou par la relation d'ordre $y \in \Gamma \langle x \rangle$) (IV, p. 5).

Lorsque, dans $\mathcal{T}$, $\Gamma$ est un préordre sur $E$, on dit de même que $E$ est un ensemble préordonné par le préordre $\Gamma$.

Dans certains cas (par exemple dans la définition qui suit), les théories dans lesquelles nous nous placerons seront un peu plus compliquées. Nous laisserons au lecteur le soin d'expliciter les constantes et les axiomes de ces théories.

Soient $E, E'$ deux ensembles ordonnés par les ordres $\Gamma$ et $\Gamma'$. On appelle isomorphisme de $E$ sur $E'$ (pour les ordres $\Gamma$ et $\Gamma'$) une application bijective $f$ de $E$ sur $E'$ telle que les relations $x \leq y$ et $f(x) \leq f(y)$ soient équivalentes (IV, p. 6).

### 4. Sous-ensembles ordonnés. Produit d'ensembles ordonnés

Soit $E$ un ensemble ordonné par un ordre $\Gamma$, de graphe $G$. Pour toute partie $A$ de $E$, $G \cap (A \times A)$ est un ordre sur $A$; la relation d'ordre correspondante équivaut à « $x \leq y$ et $x \in A$ et $y \in A$ »; nous la noterons encore $x \leq y$ (par abus de langage). L'ordre et la relation d'ordre ainsi définis sur $A$ sont dits induits par l'ordre et la relation d'ordre donnés sur $E$; on dit aussi que l'ordre et la relation d'ordre sur $E$ sont des prolongements de l'ordre et de la relation d'ordre qu'ils induisent sur A. Quand on considère A comme un ensemble ordonné, c’est de l’ordre induit sur A par celui de E qu’il s’agit, sauf mention expresse du contraire.

#### Exemple {#ens-iii-s1-n4-exa-1 .statement tag=03WB}

Les relations induites par la relation d’inclusion X ⊂ Y sur divers ensembles de parties ont une importance considérable. En voici des exemples:

1) Soient E, F deux ensembles, Φ(E, F) l’ensemble des applications de parties de E dans F; pour toute fonction f ∈ Φ(E, F), soit G_f le graphe de f, qui est une partie de E × F. Si on munit Φ(E, F) de la relation d’ordre « g prolonge f » entre f et g (III, p. 2, Exemple 3), f ↦ G_f est un isomorphisme de l’ensemble ordonné Φ(E, F) sur un sous-ensemble de $\mathfrak{P}(E \times F)$, ordonné par la relation d’inclusion.

2) Pour toute partition ω d’un ensemble E, soit $\tilde{\omega}$ le graphe de l’équivalence définie par ω dans E. L’application ω ↦ $\tilde{\omega}$ est un isomorphisme de l’ensemble $\mathcal{P}$ des partitions de E, ordonné par la relation « ω est plus fine que ω’ » entre ω et ω’ (III, p. 2, Exemple 4) sur un sous-ensemble de $\mathfrak{P}(E \times E)$, ordonné par la relation d’inclusion.

3) Soient E un ensemble, $\Omega \subset \mathfrak{P}(E \times E)$ l’ensemble des graphes des préordres sur E (III, p. 4) (ou, par abus de langage, l’ensemble des préordres sur E). La relation d’ordre s ⊂ t entre s et t, induite sur Ω par la relation d’inclusion dans $\mathfrak{P}(E \times E)$, s’exprime en disant que « le préordre s est plus fin que t » (ou que « t est moins fin que s ») Notons x(s)y et x(t)y respectivement les relations de préordre (x, y) ∈ s et (x, y) ∈ t dans E; dire que s est plus fin que t revient à dire que la relation x(s)y entraîne x(t)y.

Soit $(E_i)_{i \in I}$ une famille d’ensembles, et, pour chaque i ∈ I, soient Γ_i un ordre sur E_i, G_i ⊂ E_i × E_i son graphe; notons $x_i \leq y_i$ la relation d’ordre $(x_i, y_i) \in G_i$ dans E_i. Dans l’ensemble produit $F = \prod_{i \in I} E_i$, la relation

$$
(\forall i)((i \in I) \Rightarrow (x_i \leq y_i))
$$

est une relation d’ordre entre $x = (x_i)$ et $y = (y_i)$, comme on le vérifie aisément. L’ordre et la relation d’ordre ainsi définis sur F sont appelés l’ordre produit des ordres Γ_i, et le produit des relations d’ordre $x_i \leq y_i$; on écrit cette relation $x \leq y$, et on dit que l’ensemble F, ordonné par le produit des ordres Γ_i, est le produit des ensembles ordonnés E_i.

Il est immédiat que le graphe de l’ordre produit sur F est l’image de l’ensemble produit $\prod_{i \in I} G_i$ par l’application canonique de $\prod_{i \in I} (E_i \times E_i)$ sur F × F (II, p. 35).

Un exemple important de produit d’ensembles ordonnés est l’ensemble $F^E$ des graphes des applications d’un ensemble E dans un ensemble ordonné F; on sait qu’il existe une bijection canonique de $F^E$ sur l’ensemble $\mathscr{F}(E; F)$ des applications de E dans F (II, p. 31); cette application est un isomorphisme de l’ensemble ordonné $F^E$ sur $\mathscr{F}(E; F)$ muni de l’ordre défini par la relation « quel que soit $x \in E, f(x) \leq g(x)$ » entre deux applications f, g de E dans F (relation que l’on note $f \leq g$).

On notera que, dans l’ensemble ordonné $\mathscr{F}(E; F)$, la relation $f < g$ signifie
« quel que soit $x \in E, f(x) \leq g(x)$, et il existe $y \in E$ tel que $f(y) < g(y)$ »
et non « quel que soit $x \in E, f(x) < g(x)$ »

Pour ne pas risquer cette confusion, on évitera d’ordinaire de faire usage de la notation $f < g$ dans ce cas.

Les définitions de ce n° s’étendent sans changement aux ensembles préordonnés, en remplaçant partout « ordre » par « préordre ».

### 5. Applications croissantes

#### Définition 1 {#ens-iii-s1-def-1 .statement tag=03JC}

Soient E et F des ensembles préordonnés (par des relations toutes deux notées $\leq$). On dit qu’une application $f$ de E dans F est croissante si la relation $x \leq y$ entraîne $f(x) \leq f(y)$; on dit que $f$ est décroissante si la relation $x \leq y$ entraîne $f(x) \geq f(y)$. Une application de E dans F est dite monotone si elle est croissante ou si elle est décroissante.

Une application croissante de E dans F devient décroissante (et vice versa) quand on remplace l’un des préordres de E ou de F par le préordre opposé. Toute fonction constante est à la fois croissante et décroissante; la réciproque n’est pas vraie en général.

Par exemple, si un ensemble E est ordonné par la relation d’égalité, l’application identique de E sur lui-même est à la fois croissante et décroissante, mais non constante si E a au moins deux éléments (III, p. 71, exerc. 7).

#### Définition 2 {#ens-iii-s1-def-2 .statement tag=03JD}

Soient E et F deux ensembles ordonnés; on dit qu’une application $f$ de E dans F est strictement croissante si la relation $x < y$ entraîne $f(x) < f(y)$; on dit que $f$ est strictement décroissante si la relation $x < y$ entraîne $f(x) > f(y)$. Une application de E dans F est dite strictement monotone si elle est strictement croissante ou si elle est strictement décroissante.

#### Exemple 1 {#ens-iii-s1-n5-exa-1 .statement tag=03SK}

Soit E un ensemble; l’application $X \mapsto E - X$ de $\mathfrak{P}(E)$ (ordonné par inclusion) sur lui-même est strictement décroissante.

#### Exemple 2 {#ens-iii-s1-n5-exa-2 .statement tag=03SL}

Soit E un ensemble ordonné. Pour tout $x \in E$, soit $U_x$ l’ensemble des $y \in E$ tels que $y \geq x$. L’application $x \mapsto U_x$ est une application strictement décroissante de E dans $\mathfrak{P}(E)$ (ordonné par inclusion); on peut même remarquer que la relation $x \leq y$ est équivalente à $U_x \supset U_y$.

Une application monotone et injective d’un ensemble ordonné E dans un ensemble ordonné F est strictement monotone; la réciproque n’est pas vraie en général, puisque l’on peut avoir $f(x) = f(y)$ lorsque aucune des relations $x \leq y$, $x \geq y$ n’est vraie (cf. III, p. 14, prop. 11).

Pour qu’une application bijective $f$ d’un ensemble ordonné E sur un ensemble ordonné E’ soit un isomorphisme de E sur E’ (III, p. 5), il faut et il suffit que $f$ et son application réciproque soient croissantes.

Lorsque I est un ensemble d’indices ordonné, on dit qu’une famille de parties $(X_t)_{t \in I}$ d’un ensemble E est croissante si $t \mapsto X_t$ est un application croissante de I dans $\mathfrak{P}(E)$, ordonné par inclusion (autrement dit, si $i \leq K$ entraîne $X_i \subset X_K$). On définit de même une famille de parties $(X_t)_{t \in I}$ décroissante, strictement croissante ou strictement décroissante.

#### Proposition 2 {#ens-iii-s1-prop-2 .statement tag=03JE}

Soient E, E’ deux ensembles ordonnés, $u : E \to E'$ et $v : E' \to E$ deux applications décroissantes, telles que pour tout $x \in E$ et tout $x' \in E'$, on ait $v(u(x)) \geq x$ et $u(v(x')) \geq x'$. Alors $u \circ v \circ u = u$ et $v \circ u \circ v = v$.

En effet, la relation $v(u(x)) \geq x$ entraîne $u(v(u(x))) \leq u(x)$ puisque $u$ est décroissante; d'autre part, on a aussi $u(v(u(x))) \geq u(x)$ en remplaçant $x'$ par $u(x)$ dans l'inégalité $u(v(x')) \geq x'$. D'où la première égalité; la seconde s'établit de même.

### 6. Éléments maximaux et éléments minimaux

#### Définition 3 {#ens-iii-s1-def-3 .statement tag=03JF}

Soit $E$ un ensemble préordonné. Un élément $a \in E$ est appelé élément minimal (resp. maximal) de $E$ si la relation $x \leq a$ (resp. $x \geq a$) entraîne $x = a$.

Tout élément minimal de $E$ est un élément maximal pour l'ordre opposé, et vice versa.

#### Exemple 1 {#ens-iii-s1-n6-exa-1 .statement tag=03SM}

Soit $A$ un ensemble; dans la partie de $\mathcal{P}(A)$ (ordonnée par inclusion) formée des parties non vides de $A$, les éléments minimaux sont les parties réduites à un élément.

#### Exemple 2 {#ens-iii-s1-n6-exa-2 .statement tag=03SN}

Dans l'ensemble $\Phi(E, F)$ des applications de parties de $E$ dans $F$ ($F$ n'étant pas vide), ordonné par la relation « $v$ prolonge $u$ » entre $u$ et $v$, les éléments maximaux sont les applications de $E$ tout entier dans $F$.

#### Exemple 3 {#ens-iii-s1-n6-exa-3 .statement tag=03SO}

\* Dans l'ensemble des entiers naturels $> 1$, ordonné par la relation « $m$ divise $n$ » entre $m$ et $n$, les éléments minimaux sont les nombres premiers.*

#### Exemple 4 {#ens-iii-s1-n6-exa-4 .statement tag=03SP}

\* L'ensemble des nombres réels n'a pas d'élément maximal ni d'élément minimal.*

### 7. Plus grand élément; plus petit élément

Si, dans un ensemble ordonné $E$, il existe un élément $a$ tel que $a \leq x$ pour tout $x \in E$, c'est le seul élément de $E$ ayant cette propriété; car si on a aussi $b \leq x$ pour tout $x \in E$, on en déduit $a \leq b$ et $b \leq a$, d'où $a = b$.

#### Définition 4 {#ens-iii-s1-def-4 .statement tag=03JG}

Soit $E$ un ensemble ordonné. On dit qu'un élément $a \in E$ est le plus petit (resp. le plus grand) élément de $E$ si, pour tout $x \in E$, on a $a \leq x$ (resp. $x \leq a$).

Un ensemble ordonné n'admet pas nécessairement de plus petit ni de plus grand élément; si $E$ admet un plus petit élément $a$, $a$ est le plus grand élément de $E$ pour l'ordre opposé.

Si $E$ admet un plus petit élément $a$, $a$ est l'unique élément minimal de $E$; en effet, pour tout $x \in E$ distinct de $a$, on a $a < x$.

#### Exemple 1 {#ens-iii-s1-n7-exa-1 .statement tag=03SQ}

Soit $\mathcal{G}$ une partie non vide de l'ensemble $\mathcal{P}(E)$ des parties d'un ensemble $E$. Si $\mathcal{G}$ admet un plus petit (resp. plus grand) élément $A$ pour la relation d'inclusion, $A$ n'est autre que l'intersection (resp. la réunion) des ensembles de $\mathcal{G}$. Réciproquement, si l'intersection (resp. la réunion) des ensembles de $\mathcal{G}$ appartient à $\mathcal{G}$, c'est le plus petit (resp. plus grand) élément de $\mathcal{G}$.

#### Exemple 2 {#ens-iii-s1-n7-exa-2 .statement tag=03SR}

En particulier, $\varnothing$ est le plus petit élément et $E$ le plus grand élément de $\mathcal{P}(E)$. Dans l'ensemble $\Phi(E, F)$ des applications de parties de $E$ dans $F$, ordonné par prolongement (III, p. 2, Exemple 3) l'application vide est le plus petit élément, et il n’y a pas de plus grand élément si F n’est pas réduit à un seul élément. Enfin, la diagonale Δ de E × E est le plus petit élément de l’ensemble des graphes des équivalences sur E (ou des préordres sur E).

#### Proposition 3 {#ens-iii-s1-prop-3 .statement tag=03JH}

Soient E un ensemble ordonné, E’ l’ensemble somme de E et d’un ensemble {a} réduit à un seul élément ; il existe sur E’ un ordre et un seul induisant sur E l’ordre donné et pour lequel a soit le plus grand élément de E’.

En effet, si G est le graphe de l’ordre sur E, le graphe d’un ordre répondant à la question doit être la réunion G’ de G et de l’ensemble des couples (x, a), pour x ∈ E’ ; inversement, il est immédiat que G’ est le graphe d’un ordre sur E’, répondant aux conditions de l’énoncé.

On dit que l’ensemble ordonné E’ est obtenu en adjoignant à E un plus grand élément a (cf. III, p. 70, exerc. 3).

On dit qu’une partie A d’un ensemble préordonné E est cofinale (resp. coinitiale) à E si, pour tout x ∈ E, il existe y ∈ A tel que x ≤ y (resp. y ≤ x). Dire qu’un ensemble ordonné a un plus grand (resp. plus petit) élément signifie donc qu’il existe une partie cofinale (resp. coinitiale) de E réduite à un seul élément.

### 8. Majorants; minorants

#### Définition 5 {#ens-iii-s1-def-5 .statement tag=03JI}

Soient E un ensemble préordonné et X une partie de E. On appelle minorant (resp. majorant) de X dans E tout élément x ∈ E tel que, pour tout y ∈ X, on ait x ≤ y (resp. x ≥ y) ; on dit alors que x minore (resp. majore) X.

Tout majorant de X est un minorant de X pour l’ordre opposé, et vice versa.

Lorsque x minore X, tout élément z ≤ x minore aussi X. Un minorant de X est aussi minorant de toute partie de X. Pour qu’un ensemble ordonné X admette un plus petit élément, il faut et il suffit qu’il existe un minorant de X appartenant à X.

L’ensemble des minorants d’une partie X d’un ensemble préordonné E peut être vide : c’est le cas lorsque X = E et que E est ordonné et n’a pas de plus petit élément.

Une partie X de E dont l’ensemble des minorants (resp. des majorants) est non vide, est dite minorée (resp. majorée) ; une partie à la fois majorée et minorée est dite bornée. Lorsque X est minorée (resp. majorée, bornée), toute partie de X est minorée (resp. majorée, bornée).

Toute partie réduite à un seul élément est bornée. Mais une partie à deux éléments n’est pas nécessairement majorée ni minorée (III, p. 12).

Soient E un ensemble préordonné, et f une application d’un ensemble quelconque A dans E. On dit par abus de langage que l’application f est minorée (resp. majorée, bornée) si l’ensemble f(A) est minoré (resp. majoré, borné) dans E.

### 9. Borne supérieure; borne inférieure

#### Définition 6 {#ens-iii-s1-def-6 .statement tag=03JJ}

Soient E un ensemble ordonné, X une partie de E. On dit qu’un élément de E est la borne inférieure (resp. supérieure) de X dans E si c’est le plus grand (resp. le plus petit) élément de l’ensemble des minorants (resp. majorants) de X dans E.

Étant donnée une partie X d’un ensemble ordonné E, on note sup_E X (resp. inf_E X) ou sup X (resp. inf X) lorsque aucune confusion n’est à craindre, la borne supérieure (resp. inférieure) de X dans E, lorsque cette borne existe. La borne supérieure (resp. inférieure) d’un ensemble à deux éléments {x, y} se note (lorsqu’elle existe) sup (x, y) (resp. inf (x, y)); notations analogues pour les bornes supérieure et inférieure d’un ensemble à trois éléments, etc.

Si une partie X de E admet un plus grand élément a, a est borne supérieure de X dans E.

Si X admet une borne inférieure a dans E, a est borne supérieure de X pour l’ordre opposé sur E; ceci nous permettra, dans ce qui suit, de ne considérer le plus souvent que les propriétés des bornes supérieures.

#### Exemple 1 {#ens-iii-s1-n9-exa-1 .statement tag=03SS}

L’ensemble des majorants de la partie vide $\varnothing$ d’un ensemble ordonné E est évidemment E lui-même; pour que $\varnothing$ admette dans E une borne supérieure, il faut et il suffit donc que E admette un plus petit élément, qui est alors la borne supérieure de $\varnothing$.

#### Exemple 2 {#ens-iii-s1-n9-exa-2 .statement tag=03ST}

Dans l’ensemble $\mathfrak{P}(E)$ des parties d’un ensemble E, ordonné par inclusion, toute partie $\mathcal{G}$ de $\mathfrak{P}(E)$ admet une borne supérieure, qui est la réunion des ensembles de $\mathcal{G}$, et une borne inférieure, qui est l’intersection des ensembles de $\mathcal{G}$.

#### Exemple 3 {#ens-iii-s1-n9-exa-3 .statement tag=03SU}

Soient E et F deux ensembles, et $\Theta$ une partie de l’ensemble $\Phi(E, F)$ des applications de parties de E dans F, ordonné par prolongement (III, p. 2, Exemple 3). Pour tout $u \in \Phi(E, F)$, soit D(u) l’ensemble de définition de u. La condition d’existence d’un prolongement commun pour une famille d’applications appartenant à $\Phi(E, F)$ (II, p. 28, prop. 7) montre que, pour que $\Theta$ admette une borne supérieure dans $\Phi(E, F)$, il faut et il suffit que pour tout couple d’éléments (u, v) de $\Theta$, on ait $u(x) = v(x)$ pour tout $x \in D(u) \cap D(v)$.

Étant donnée une application f d’un ensemble A dans un ensemble ordonné E, on dit que cette fonction admet une borne supérieure si l’image $f(A)$ admet une borne supérieure dans E; cette borne est alors appelée borne supérieure de f et se note $\sup_{x \in A} f(x)$. La borne inférieure de f se définit et se note d’une manière analogue.

En particulier, si une partie A de E admet une borne supérieure dans E, cette borne est la borne supérieure de l’injection canonique de A dans E, et peut donc s’écrire $\sup_{x \in A} x$.

#### Proposition 4 {#ens-iii-s1-prop-4 .statement tag=03JK}

Soient E un ensemble ordonné, et A une partie de E admettant à la fois une borne inférieure et une borne supérieure dans E; on a $\inf A \leq \sup A$ si A n’est pas vide; si $A = \varnothing$, $\sup A$ est le plus petit et $\inf A$ le plus grand élément de E.

Cela résulte aussitôt des définitions.

#### Proposition 5 {#ens-iii-s1-prop-5 .statement tag=03JL}

Soient E un ensemble ordonné, A et B deux parties de E admettant toutes deux une borne supérieure (resp. inférieure) dans E ; si A ⊂ B, on a sup A ≤ sup B (resp. inf A ≥ inf B).

La proposition est évidente.

#### Corollaire {#ens-iii-s1-n9-cor-1 .statement tag=03JM}

Soit $(x_i)_{i \in I}$ une famille d’éléments d’un ensemble ordonné E, admettant une borne supérieure dans E ; si J est une partie de I telle que la famille $(x_i)_{i \in J}$ admette une borne supérieure dans E, on a $\sup_{i \in J} x_i \leq \sup_{i \in I} x_i$.

#### Proposition 6 {#ens-iii-s1-prop-6 .statement tag=03JN}

Soient $(x_i)_{i \in I}, (y_i)_{i \in I}$ deux familles d’éléments d’un ensemble ordonné E, ayant même ensemble d’indices I, et telles que $x_i \leq y_i$ pour tout $i \in I$ ; si elles admettent toutes deux une borne supérieure dans E, on a $\sup_{i \in I} x_i \leq \sup_{i \in I} y_i$.

En effet, $a = \sup_{i \in I} y_i$ est un majorant de l’ensemble des $y_i$, donc $x_i \leq y_i \leq a$ pour tout $i$, ce qui entraîne $\sup_{i \in I} x_i \leq a$.

#### Proposition 7 {#ens-iii-s1-prop-7 .statement tag=03JO}

Soient $(x_i)_{i \in I}$ une famille d’éléments d’un ensemble ordonné E, $(J_\lambda)_{\lambda \in L}$ un recouvrement de l’ensemble d’indices I ; on suppose que chacune des sous-familles $(x_i)_{i \in J_\lambda}$ admette une borne supérieure dans E. Pour que la famille $(x_i)_{i \in I}$ admette une borne supérieure dans E, il faut et il suffit que la famille $(\sup_{i \in J_\lambda} x_i)_{\lambda \in L}$ admette une borne supérieure dans E, et on a alors

(1)
$$
\sup_{i \in I} x_i = \sup_{\lambda \in L} (\sup_{i \in J_\lambda} x_i).
$$

Posons $b_\lambda = \sup_{i \in J_\lambda} x_i$. Supposons que $(x_i)_{i \in I}$ admette une borne supérieure $a$ ; alors $a \geq b_\lambda$ pour tout $\lambda \in L$ (cor. de la prop. 5) ; d’autre part, si $c \geq b_\lambda$ pour tout $\lambda \in L$, on a aussi $c \geq x_i$ pour tout $i \in I$, puisque $(J_\lambda)_{\lambda \in L}$ est un recouvrement de I ; on a donc $c \geq a$, ce qui prouve que $a = \sup_{\lambda \in L} b_\lambda$. Supposons réciproquement que la famille $(b_\lambda)_{\lambda \in L}$ admette une borne supérieure $a'$ ; alors $a' \geq x_i$ pour tout $i \in I$ ; d’autre part, si $c' \geq x_i$ pour tout $i \in I$, on a en particulier $c' \geq \sup_{i \in J_\lambda} x_i = b_\lambda$ pour tout $\lambda \in L$, donc $c' \geq a'$, ce qui prouve que $a' = \sup_{i \in I} x_i$.

#### Corollaire {#ens-iii-s1-n9-cor-2 .statement tag=03JP}

Soit $(x_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$ une famille « double » d’éléments d’un ensemble ordonné E, telle que, pour tout $\mu \in M$, la famille $(x_{\lambda \mu})_{\lambda \in L}$ admette une borne supérieure dans E. Pour que la famille $(x_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$ admette une borne supérieure dans E, il faut et il suffit que la famille $(\sup_{\lambda \in L} x_{\lambda \mu})_{\mu \in M}$ en admette une, et on a alors

(2)
$$
\sup_{(\lambda, \mu) \in L \times M} x_{\lambda \mu} = \sup_{\mu \in M} (\sup_{\lambda \in L} x_{\lambda \mu}).
$$

#### Proposition 8 {#ens-iii-s1-prop-8 .statement tag=03QI}

Soit $(E_i)_{i \in I}$ une famille d’ensembles ordonnés. Soit A une partie de l’ensemble ordonné produit $E = \prod_{i \in I} E_i$, et, pour tout $i \in I$, soit $A_i = \mathrm{pr}_i A$. Pour que A admette une borne supérieure dans E, il faut et il suffit que, pour tout $t \in I$, $A_t$ admette une borne supérieure dans $E_t$, et on a alors

$$
\sup A = (\sup A_t)_{t \in I} = (\sup_{x \in A} \operatorname{pr}_t x)_{t \in I}.
$$

En effet, supposons que, pour tout $t \in I$, $A_t$ admette une borne supérieure $b_t$ dans $E_t$. Dire que $c = (c_t)$ est un majorant de $A$ signifie alors que $c_t \geq b_t$ pour tout $t \in I$, donc $(b_t)_{t \in I}$ est borne supérieure de $A$. Réciproquement, supposons que $A$ admette une borne supérieure $a = (a_t)_{t \in I}$; pour tout $\kappa \in I$, $a_\kappa$ est un majorant de $A_\kappa$, car si $x_\kappa \in A_\kappa$, il existe $x \in A$ tel que $\operatorname{pr}_\kappa x = x_\kappa$, par définition de $A_\kappa$; d'autre part, si $a'_\kappa$ est un majorant de $A_\kappa$ dans $E_\kappa$, l’élément $c' = (c'_t)_{t \in I}$ tel que $c'_t = a_t$ pour $t \neq \kappa$ et $c'_\kappa = a'_\kappa$, est un majorant de $A$, ce qui entraîne $c' \geq a$, et par suite $a'_\kappa \geq a_\kappa$; $a_\kappa$ est donc la borne supérieure de $A_\kappa$ dans $E_\kappa$.

Soit F une partie d’un ensemble ordonné E, et soit A une partie de F. Il peut se faire que l’un des deux éléments $\sup_E A$, $\sup_F A$ existe, et non l’autre, ou qu’il existent tous deux et soient inégaux.

#### Exemple 4 {#ens-iii-s1-n9-exa-4 .statement}

Dans l’ensemble ordonné $E = \mathbf{R}$ des nombres réels, considérons l’ensemble $F = \mathbf{Q}$ des nombres rationnels, et l’ensemble $A \subset F$ des nombres rationnels $< \sqrt{2}$; alors $\sup_E A$ existe, mais non $\sup_F A$.
3) Avec les mêmes notations que dans l’exemple 1), soit G la réunion de A et de l’ensemble {2}; on a $G \subset F$, et $\sup_G A$ existe, mais non $\sup_F A$.
3) Avec les mêmes notations, on a $\sup_E A = \sqrt{2}$, $\sup_G A = 2.*$

On a toutefois le résultat suivant:

#### Proposition 9 {#ens-iii-s1-prop-9 .statement tag=03QJ}

Soient E un ensemble ordonné, F une partie de E et A une partie de F. Si $\sup_E A$ et $\sup_F A$ existent toutes deux, on a $\sup_E A \leq \sup_F A$. Si $\sup_E A$ existe et appartient à F, $\sup_F A$ existe et est égale à $\sup_E A$.

La première assertion résulte de ce que l’ensemble M des majorants de A dans F est contenu dans l’ensemble N des majorants de A dans E, et de la prop. 5 (III, p. 10). D’autre part, si le plus petit élément de N est dans F, il appartient à M, et c’est évidemment le plus petit élément de M; cela démontre la seconde assertion.

### 10. Ensembles filtrants

#### Définition 7 {#ens-iii-s1-def-7 .statement tag=03QK}

On dit qu’un ensemble préordonné E est filtrant à droite (resp. à gauche) si toute partie à deux éléments de E est majorée (resp. minorée).

Au lieu de « filtrant à droite », on dit aussi « filtrant pour la relation $\leq$ »; expressions analogues lorsque la relation de préordre est notée par un autre signe. Par exemple, si $\mathcal{S}$ est un ensemble de parties d’un ensemble A, on dira que $\mathcal{S}$ est filtrant pour la relation $\subset$ (resp. $\supset$) si, pour toute partie à deux éléments {X, Y} de $\mathcal{S}$, il existe $Z \in \mathcal{S}$ tel que $X \subset Z$ et $Y \subset Z$ (resp. $X \supset Z$ et $Y \supset Z$).

Par abus de langage, au lieu d’« ensemble filtrant à droite » (resp. « à gauche »), on dira aussi parfois « ensemble filtrant croissant » (resp. « décroissant »).

#### Exemple 1 {#ens-iii-s1-n10-exa-1 .statement}

Un ensemble ordonné qui admet un plus grand élément est filtrant à droite.

#### Exemple 2 {#ens-iii-s1-n10-exa-2 .statement}

\* Dans un espace topologique, un système fondamental de voisinages d’un point est filtrant pour la relation ⊃ (TG, I, § 1, no. 3).
    3) L’ensemble des sous-modules de type fini d’un module quelconque (A, II, § 1, n° 7) est filtrant pour la relation ⊂.*

#### Proposition 10 {#ens-iii-s1-prop-10 .statement tag=03QL}

Dans un ensemble ordonné filtrant à droite E, un élément maximal a est le plus grand élément de E.
    En effet, pour tout x ∈ E, il existe par hypothèse y ∈ E tel que x ≤ y et a ≤ y, et comme a est maximal, y = a.

Un ensemble préordonné filtrant à droite est filtrant à gauche pour l’ordre opposé. Tout produit d’ensembles filtrants à droite est filtrant à droite. Par contre, une partie d’un ensemble filtrant à droite n’est pas nécessairement filtrante à droite. Toutefois, une partie cofinale F d’un ensemble filtrant à droite E est un ensemble filtrant à droite : en effet, pour tout couple d’éléments x, y de F, il existe z ∈ E tel que x ≤ z et y ≤ z, puis t ∈ F tel que z ≤ t.

### 11. Ensembles réticulés

#### Définition 8 {#ens-iii-s1-def-8 .statement tag=03QM}

On dit qu’un ensemble ordonné E est réticulé (ou que E est un réseau ordonné, ou un lattis) si toute partie à deux éléments de E admet une borne supérieure et une borne inférieure dans E.

Tout produit d’ensembles réticulés est réticulé, comme il résulte de la condition d’existence d’une borne supérieure dans un produit d’ensembles ordonnés (III, p. 11, prop. 8). L’ensemble des parties d’un ensemble A, ordonné par inclusion, est réticulé, puisque la réunion et l’intersection de deux parties de A sont encore des parties de A.

#### Exemple 1 {#ens-iii-s1-n11-exa-1 .statement tag=03SV}

L’ensemble des entiers ≥ 1, ordonné par la relation « m divise n » entre m et n, est réticulé, la borne supérieure (resp. inférieure) de {m, n} n’étant autre que le ppcm (resp. pgcd) de m et n (A, VII, § 1).
    2) L’ensemble des sous-groupes d’un groupe G, ordonné par inclusion, est réticulé (A, I, § 4, n° 3).
    3) L’ensemble des topologies sur un ensemble A, ordonné par la relation « T est moins fine que T’ » entre T et T’, est réticulé (TG, I, § 1, n°s 3 et 4).
    4) L’ensemble $\mathcal{F}(I; \mathbf{R})$ des fonctions numériques définies dans un intervalle I de $\mathbf{R}$ est réticulé pour la relation d’ordre $f \leq g$ (III, p. 6), pour laquelle il est isomorphe au produit $\mathbf{R}^I$ (cf. INT, II).*

#### Remarque {#ens-iii-s1-n11-rem-1 .statement tag=03JQ}

Un ensemble ordonné réticulé est évidemment filtrant à droite et à gauche. Mais un ensemble filtrant à droite et à gauche n’est pas nécessairement réticulé, \* comme le montre l’exemple de l’ensemble des applications $x \mapsto p(x)$ de $\mathbf{R}$ dans lui-même, où $p$ est un polynôme de $\mathbf{R}[X]$, cet ensemble étant ordonné par la relation $p \leq q$ (III, p. 6).*

### 12. Ensembles totalement ordonnés

#### Définition 9 {#ens-iii-s1-def-9 .statement tag=03JR}

On dit que deux éléments x, y d’un ensemble préordonné E sont comparables si la relation « x ≤ y ou y ≤ x » est vraie. On dit qu’un ensemble E est totalement ordonné s'il est ordonné et si deux éléments quelconques de E sont comparables. On dit alors que l'ordre sur E est un ordre total, et la relation d'ordre correspondante une relation d'ordre total.

Lorsque x et y sont des éléments d'un ensemble totalement ordonné E, on a $x = y$, ou $x < y$, ou $x > y$; la négation de $x \leq y$ est alors $x > y$.

Pour qu'un ordre sur E soit un ordre total, il faut et il suffit que son graphe G, en plus des relations $G \circ G = G$ et $G \cap \overline{G}^1 = \Delta$, satisfasse à la relation $G \cup \overline{G}^1 = E \times E$.

#### Exemple 1 {#ens-iii-s1-n12-exa-1 .statement tag=03SW}

Toute partie d'un ensemble totalement ordonné est totalement ordonnée par l'ordre induit.

#### Exemple 2 {#ens-iii-s1-n12-exa-2 .statement tag=03TW}

Soit E un ensemble ordonné quelconque. La partie vide de E est totalement ordonnée, ainsi que toute partie réduite à un élément.

#### Exemple 3 {#ens-iii-s1-n12-exa-3 .statement tag=03TX}

\* L'ensemble $\mathbf{R}$ des nombres réels est totalement ordonné.*

#### Exemple 4 {#ens-iii-s1-n12-exa-4 .statement tag=03TY}

Si A est un ensemble ayant au moins deux éléments distincts, l'ensemble $\mathcal{P}(A)$, ordonné par inclusion, n'est pas totalement ordonné, car si $x \neq y$, les parties $\{x\}$ et $\{y\}$ ne sont pas comparables.

Un ensemble totalement ordonné est aussi totalement ordonné pour l'ordre opposé; il est réticulé et a fortiori filtrant à droite et à gauche.

#### Proposition 11 {#ens-iii-s1-prop-11 .statement tag=03JS}

Toute application strictement monotone f d'un ensemble totalement ordonné E dans un ensemble ordonné F est injective; si f est strictement croissante, f est un isomorphisme de E sur f(E).

En effet, $x \neq y$ entraîne $x < y$ ou $x > y$, donc $f(x) < f(y)$ ou $f(x) > f(y)$, et par suite $f(x) \neq f(y)$ en tous cas. Il reste à montrer que, si f est strictement croissante, $f(x) \leq f(y)$ entraîne $x \leq y$; dans le cas contraire, on aurait $x > y$, d'où $f(x) > f(y)$.

#### Proposition 12 {#ens-iii-s1-prop-12 .statement tag=03JT}

Soient E un ensemble totalement ordonné, X une partie de E. Pour qu'un élément $b \in E$ soit borne supérieure de X dans E, il faut et il suffit que : 1° b soit un majorant de X ; 2° pour tout $c \in E$ tel que $c < b$, il existe $x \in X$ tel que $c < x \leq b$.

En effet, la seconde condition exprime qu'aucun élément $c < b$ n'est un majorant de X, c'est-à-dire que b est un élément minimal de l'ensemble M des majorants de X; mais ceci revient à dire que b est le plus petit élément de M, puisque M est totalement ordonné (III, p. 13, prop. 10).

### 13. Intervalles

Soient E un ensemble ordonné, a et b deux éléments de E tels que $a \leq b$. On appelle intervalle fermé d'origine a et d'extrémité b, et on note $[a, b]$, la partie de E formée des éléments x tels que $a \leq x \leq b$; on appelle intervalle semi-ouvert à droite (resp. à gauche) d'origine a et d'extrémité b et on note $]a, b[$ (resp. $]a, b]$) l'ensemble des $x \in E$ tels que $a \leq x < b$ (resp. $a < x \leq b$); on appelle intervalle ouvert d'origine a et d'extrémité b, et on note $]a, b[$, l'ensemble des $x \in E$ tels que $a < x < b$.

On notera qu’un intervalle fermé n’est jamais vide; l’intervalle $(a, a)$ est l’ensemble réduit à l’élément $a$. Par contre les intervalles $(a, a[, )a, a)$ et $]a, a[$ sont vides; un intervalle ouvert $]a, b[$ peut être vide même si $a < b$.

Soit $a$ un élément de $E$. L’ensemble des $x \in E$ tels que $x \leq a$ (resp. $x < a$) s’appelle l’intervalle fermé (resp. ouvert) illimité à gauche et d’extrémité $a$, et se note $]\leftarrow, a]$ (resp. $]\leftarrow, a[$); l’ensemble des $x \in E$ tels que $x \geq a$ (resp. $x > a$) s’appelle l’intervalle fermé (resp. ouvert) illimité à droite et d’origine $a$, et se note $[a, \rightarrow[$ (resp. $]a, \rightarrow[$). Enfin, $E$ lui-même est appelé l’intervalle ouvert illimité dans les deux sens, et est noté $]\leftarrow, \rightarrow[$.

#### Proposition 13 {#ens-iii-s1-prop-13 .statement tag=03JU}

*Dans un ensemble réticulé, l’intersection de deux intervalles est un intervalle.*

Considérons par exemple l’intersection de deux intervalles fermés $(a, b]$ et $[c, d)$, et posons $\alpha = \sup (a, c)$, $\beta = \inf (b, d)$. Si on a à la fois $a \leq x \leq b$ et $c \leq x \leq d$, on en déduit $\alpha \leq x \leq \beta$ et réciproquement; si on n’a pas $\alpha \leq \beta$, l’intersection de $(a, b]$ et $[c, d)$ est donc vide; si $\alpha \leq \beta$, cette intersection est $[\alpha, \beta]$. Nous laissons au lecteur le soin de faire la démonstration dans les autres cas.

## EXERCICES {#ens-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
