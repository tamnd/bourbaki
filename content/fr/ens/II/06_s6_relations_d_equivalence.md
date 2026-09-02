---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 6
section_title: Relations d’équivalence
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E II.51-E II.52
pdf_pages: 0091-0101, 0103-0104
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une relation d’équivalence
      page: 39
      pdf_page: 91
    - "no": 2
      title: Classes d'équivalence; ensemble quotient
      page: 41
      pdf_page: 93
    - "no": 3
      title: Relations compatibles avec une relation d’équivalence
      page: 42
      pdf_page: 94
    - "no": 4
      title: Parties saturées
      page: 43
      pdf_page: 95
    - "no": 5
      title: Applications compatibles avec des relations d'équivalence
      page: 44
      pdf_page: 96
    - "no": 6
      title: Image réciproque d’une relation d’équivalence; relation d’équivalence induite
      page: 45
      pdf_page: 97
    - "no": 7
      title: Quotients de relations d’équivalence
      page: 45
      pdf_page: 97
    - "no": 8
      title: Produit de deux relations d'équivalence
      page: 46
      pdf_page: 98
    - "no": 9
      title: Classes d'objets équivalents
      page: 47
      pdf_page: 99
statements: 5
exercises: 10
content_sha256: 987904398af6d2599bd91eb95321c9683702ab73b500683f239a59359c7532cc
---

## § 6. RELATIONS D’ÉQUIVALENCE

En principe, nous cesserons désormais d’utiliser des lettres italiques grasses pour désigner des assemblages indéterminés; le contexte permettra au lecteur de discerner sans peine les assertions qui s’appliquent à des lettres ou des relations indéterminées.

### 1. Définition d’une relation d’équivalence

Soit $R \{ x, y \}$ une relation, $x$ et $y$ étant des lettres distinctes. On dit que la relation $R$ est symétrique (par rapport aux lettres $x$ et $y$) si l’on a $R \{ x, y \} \Rightarrow R \{ y, x \}$. S’il en est ainsi, en substituant à $x$ et $y$ deux lettres $x', y'$, distinctes entre elles et distinctes de toutes les lettres figurant dans $R$, puis en substituant $y$ et $x$ à $x'$ et $y'$ respectivement, on voit que l’on a $R \{ y, x' \} \Rightarrow R \{ x, y' \}$; donc $R \{ x, y \}$ et $R \{ y, x \}$ sont équivalentes.

Soit $z$ une lettre ne figurant pas dans $R$. On dit que la relation $R$ est transitive (par rapport aux lettres $x$ et $y$) si l’on a $(R \{ x, y \} \text{ et } R \{ y, z \}) \Rightarrow R \{ x, z \}$.

#### Exemple {#ens-ii-s6-n1-exa-1 .statement tag=03IX}

La relation $x = y$ est symétrique et transitive. La relation $X \subset Y$ est transitive, mais non symétrique. La relation $X \cap Y = \varnothing$ est symétrique, mais non transitive.

Si $R\{x, y\}$ est à la fois symétrique et transitive, on dit que $R\{x, y\}$ est une *relation d'équivalence* (par rapport aux lettres $x$ et $y$). Dans ce cas, la notation $x \equiv y$ (mod $R$) est parfois employée comme synonyme de $R\{x, y\}$; elle se lit « *x est équivalent à y modulo R* (ou *suivant R*) ». Si $R$ est une relation d'équivalence, on a
$$
R\{x, y\} \Rightarrow (R\{x, x\} \text{ et } R\{y, y\}),
$$
car $R\{x, y\}$ entraîne $R\{y, x\}$, et $(R\{x, y\} \text{ et } R\{y, x\})$ entraîne $(R\{x, x\} \text{ et } R\{y, y\})$, en vertu des définitions.

Soient $R\{x, y\}$ une relation, $E$ un terme. On dit que la relation $R$ est *réflexive dans* $E$ (par rapport aux lettres $x$ et $y$ ne figurant pas dans $E$) si la relation $R\{x, x\}$ est équivalente à $x \in E$. S'il n'y a pas de confusion possible sur $E$, on dit simplement, par abus de langage, que $R$ est réflexive.

On appelle *relation d'équivalence dans* $E$ une relation d'équivalence réflexive dans $E$. Si $R\{x, y\}$ est une relation d'équivalence dans $E$, on a
$$
R\{x, y\} \Rightarrow ((x, y) \in E \times E),
$$
donc $R$ admet un graphe (par rapport aux lettres $x$ et $y$). Réciproquement, supposons que la relation d'équivalence $R\{x, y\}$ admette un graphe $G$; remarquons que la relation $R\{x, x\}$ est équivalente à la relation $(\exists y)R\{x, y\}$; en effet, elle entraîne cette dernière (I, p. 33, schéma S5), et d'autre part, comme $R\{x, y\}$ entraîne $R\{x, x\}$, $(\exists y)R\{x, y\}$ entraîne $(\exists y)R\{x, x\}$, donc aussi $R\{x, x\}$. On voit donc que $R\{x, x\}$ est équivalente à $x \in \mathrm{pr}_1 G$, de sorte que $R$ est une relation d'équivalence dans $\mathrm{pr}_1 G$.

On appelle *équivalence* dans un ensemble $E$ une correspondance admettant $E$ pour ensemble d'arrivée et pour ensemble de départ, et dont le graphe $F$ est tel que la relation $(x, y) \in F$ soit une relation d'équivalence dans $E$.

*Exemples*
1) La relation $x = y$ est une relation d'équivalence qui n'admet pas de graphe, car la première projection de ce graphe serait l'ensemble de tous les objets.
2) La relation « $x = y$ et $x \in E$ » est une relation d'équivalence dans $E$ dont le graphe est la diagonale de $E \times E$.
3) La relation « il existe une bijection de $X$ sur $Y$ » est une relation d'équivalence qui n'admet pas de graphe (cf. III, p. 30).
4) La relation « $x \in E$ et $y \in E$ » est un relation d'équivalence dans $E$ dont le graphe est $E \times E$.
5) Supposons $A \subset E$. La relation
$$
(x \in E - A \text{ et } y = x) \text{ ou } (x \in A \text{ et } y \in A)
$$
est une relation d'équivalence dans $E$.

6) \* La relation « $x \in \mathbf{Z}$ et $y \in \mathbf{Z}$ et $x - y$ est divisible par 4 » est une relation d'équivalence dans $\mathbf{Z}$.*

#### Proposition 1 {#ens-ii-s6-prop-1 .statement tag=03QH}

Pour qu'une correspondance $\Gamma$ entre $X$ et $X$ soit une équivalence dans $X$, il faut et il suffit que les conditions suivantes soient vérifiées : a) $X$ est l'ensemble de définition de $\Gamma$; b) on a $\Gamma = \overline{\Gamma}^{-1}$; c) on a $\Gamma' \circ \Gamma = \Gamma$.

Soient $\Gamma$ une correspondance entre $X$ et $X$, et $G$ son graphe. Si $\Gamma$ est une équivalence dans $X$, on a $(x, x) \in G$ pour tout $x \in X$, donc $X$ est l'ensemble de définition de $\Gamma$. La relation $(x, y) \in G$ est équivalente à $(y, x) \in G$, donc à $(x, y) \in \overline{G}^{-1}$, de sorte que $G = \overline{G}^{-1}$, donc $\Gamma' = \overline{\Gamma}^{-1}$. Les relations $(x, y) \in G$ et $(y, z) \in G$ entraînent $(x, z) \in G$, ce qui montre que $G \circ G \subset G$; par ailleurs, la relation $(x, y) \in G$ entraîne $(x, x) \in G$, donc $(x, y) \in G \circ G$ de sorte que $G \subset G \circ G$; on a donc $G = G \circ G$, et par suite $\Gamma = \Gamma \circ \Gamma$.

Réciproquement, supposons les conditions $a),\ b),\ c)$ vérifiées. La relation $(x, y) \in G$ est symétrique en vertu de $b)$ en transitive en vertu de $c)$; c'est donc une relation d'équivalence, et il résulte de $a)$ que c'est une relation d'équivalence dans $X$.

### 2. Classes d'équivalence; ensemble quotient

Soient $f$ une fonction, $E$ son ensemble de définition, $F$ son graphe. La relation « $x \in E$ et $y \in E$ et $f(x) = f(y)$ » est une relation d'équivalence dans $E$; nous dirons que cette relation est la relation d'équivalence associée à $f$. Elle est équivalente à la relation $(\exists z)((x, z) \in F \text{ et } (y, z) \in F)$, c'est-à-dire à
$$
(\exists z)((x, z) \in F \text{ et } (z, y) \in \overline{F}^{-1});
$$
son graphe est donc $\overline{F}^{-1} \circ F$.

Nous allons maintenant montrer que toute relation d'équivalence $R$ dans un ensemble $E$ est du type précédent. Soit en effet $G$ le graphe de $R$. Pour tout $x \in E$, l'ensemble (non vide) $G(x) \subset E$ s'appelle la classe d'équivalence de $x$ suivant $R$: c'est donc l'ensemble des $y \in E$ tels que $R \{ x, y \}$; tout ensemble qui peut se mettre sous la forme $G(x)$ pour un $x \in E$ est appelé une classe d'équivalence (suivant $R$). Un élément d'une classe d'équivalence est encore appelé un représentant de cette classe. L'ensemble des classes d'équivalence suivant $R$ (c'est-à-dire l'ensemble des objets de la forme $G(x)$, pour $x \in E$) s'appelle l'ensemble quotient de $E$ par $R$ et se désigne par $E/R$; l'application $x \mapsto G(x)$ ($x \in E$) dont l'ensemble de définition est $E$ et l'ensemble d'arrivée $E/R$, s'appelle l'application canonique de $E$ sur $E/R$. On a alors le critère suivant:

C55. Soient $R$ une relation d'équivalence dans un ensemble $E$, et $p$ l'application canonique de $E$ sur $E/R$. On a
$$
R \{ x, y \} \Leftrightarrow (p(x) = p(y)).
$$

En effet (avec les notations précédentes), soient $x$ et $y$ des éléments de $E$ tels que $(x, y) \in G$. On a d’abord $x \in E$ et $y \in E$; montrons que $G(x) = G(y)$. Puisque $y \in G(x)$, on a (II, p. 41, prop. 1) $G(y) \subset (G \circ G)(x) = G(x)$. Par ailleurs, on a aussi $(y, x) \in G$, d’où $G(x) \subset G(y)$ et par suite $G(x) = G(y)$, c’est-à-dire $p(x) = p(y)$. Réciproquement, si $G(x) = G(y)$, on a $y \in G(y) = G(x)$, d’où $(x, y) \in G$, ce qui démontre le critère.

Une section associée à l’application canonique $p$ de $E$ sur $E/R$ (II, p. 18, déf. 11) s’appelle plus brièvement une section de $E$ (pour la relation $R$).

Exemples

1) Soit $R$ la relation d’équivalence « $x \in E$ et $y \in E$ et $x = y$ » dans un ensemble $E$; la classe d’équivalence de $x \in E$ est alors l’ensemble $\{x\}$, et l’application canonique $x \mapsto \{x\}$ de $E$ sur $E/R$ est bijective.

2) Soient $E$ et $F$ deux ensembles tels que $F \neq \varnothing$, et $R$ la relation d’équivalence dans $E \times F$ associée à l’application $\mathrm{pr}_1$ de $E \times F$ sur $E$. Les classes d’équivalence pour $R$ sont les ensembles de la forme $\{x\} \times F$, où $x \in E$; l’application $x \mapsto \{x\} \times F$ est une bijection de $E$ sur $(E \times F)/R$.

Soit $R$ une relation d’équivalence dans un ensemble $E$. L’ensemble quotient $E/R$ est une partie de $\mathfrak{P}(E)$, et l’application identique de $E/R$ est une partition de $E$ (II, p. 29); en effet, si $G$ est le graphe de $R$, et si deux classes d’équivalences $G(x)$ et $G(y)$ ont un élément commun $z$, on a $R\{x, z\}$ et $R\{z, y\}$, donc $R\{x, y\}$, et par suite $G(x) = G(y)$. En outre la relation

$$
(\exists X)(X \in E/R \text{ et } x \in X \text{ et } y \in X)
$$

est équivalente à $R\{x, y\}$.

Réciproquement, soit $(X_t)_{t \in I}$ une partition d’un ensemble $E$ en ensembles non vides; on vérifie aussitôt que la relation $(\exists t)(t \in I \text{ et } x \in X_t \text{ et } y \in X_t)$ est une relation d’équivalence $R$ dans $E$; les classes d’équivalence suivant $R$ ne sont autres que les ensembles $X_t$ de la partition, et l’application $t \mapsto X_t$ est une bijection de $I$ sur $E/R$. Toute partie $S$ de $E$ telle que, pour tout $t \in I$, l’ensemble $S \cap X_t$ soit réduit à un élément, s’appelle un système de représentants des classes d’équivalence suivant $R$. On désigne aussi sous ce nom toute injection d’un ensemble $K$ dans $E$, telle que l’image de $K$ par cette injection soit un système de représentants des classes d’équivalence suivant $R$; il en est ainsi, en particulier, de toute section de $E$ pour la relation $R$.

### 3. Relations compatibles avec une relation d’équivalence

Soient $R\{x, x'\}$ une relation d’équivalence, et $P\{x\}$ une relation. On dit que $P\{x\}$ est compatible avec la relation d’équivalence $R\{x, x'\}$ (par rapport à $x$) si, $y$ désignant une lettre qui ne figure ni dans $P$, ni dans $R$, on a

$$
(P\{x\} \text{ et } R\{x, y\}) \Rightarrow P\{y\}.
$$

Par exemple, il résulte de C43 (I, p. 39) que n’importe quelle relation P$$x$$ est compatible avec la relation d’équivalence $x = x'$.

C56. Soient R$$x, x'$$ une relation d’équivalence dans un ensemble E, P$$x$$ une relation où ne figure pas la lettre $x'$, compatible (par rapport à x) avec la relation d’équivalence R$$x, x'$$; alors, si t ne figure pas dans P$$x$$, la relation « $t \in E/R$ et $(\exists x)(x \in t \text{ et } P[x])$ » est équivalente à la relation « $t \in E/R$ et $(\forall x)((x \in t) \Rightarrow P[x])$ ».

En effet, soit $t \in E/R$. S’il existe un $a \in t$ tel que P$$a$$, alors, pour tout $x \in t$, on a R$$a, x$$, donc P$$x$$. Donc $(\exists x)(x \in t \text{ et } P[x])$ entraîne $(\forall x)((x \in t) \Rightarrow P[x])$. La réciproque est évidente, puisque $t \in E/R$ implique $t \neq \varnothing$.

On dit que la relation

$$
t \in E/R \text{ et } (\exists x)(x \in t \text{ et } P[x])
$$

est la relation déduite de P$$x$$ par passage au quotient (par rapport à x) pour la relation R. Si on désigne cette relation par P$$t$$, et si f est l’application canonique de E sur E/R, la relation $(y \in E \text{ et } P[f(y)])$ (où y ne figure pas dans P$$x$$) est équivalente à $(y \in E \text{ et } P[y])$ comme on le vérifie aussitôt.

### 4. Parties saturées

Soient R$$x, y$$ une relation d’équivalence dans un ensemble E, et A une partie de E. On dit que A est saturée pour R si la relation $x \in A$ est compatible (par rapport à x) avec R$$x, y$$; il revient au même de dire que, pour tout $x \in A$, la classe d’équivalence de x est contenue dans A. En d’autres termes, pour qu’un ensemble soit saturé pour R, il faut et il suffit qu’il soit réunion d’un ensemble de classes d’équivalence suivant R.

Soit f l’application canonique de E sur E/R; si A est saturé pour R, la classe d’équivalence de tout élément $x \in A$, qui n’est autre que $f^{-1}\langle\{f(x)\}\rangle$, est contenue dans A, donc on a $f^{-1}\langle f\langle A\rangle \rangle \subset A$; comme par ailleurs $A \subset f^{-1}\langle f\langle A\rangle \rangle$, on a $A = f^{-1}\langle f\langle A\rangle \rangle$. Réciproquement, si $A = f^{-1}\langle f\langle A\rangle \rangle$, alors pour tout $x \in A$ la classe d’équivalence K = $f(x)$ de x pour R est un élément de $f\langle A\rangle$, et comme $K = f^{-1}\langle\{K\}\rangle$, on a $K \subset f^{-1}\langle f\langle A\rangle \rangle = A$. On voit donc que les parties de E saturées pour R sont les parties A de E telles que $A = f^{-1}\langle f\langle A\rangle \rangle$. On peut dire aussi que ce sont les parties de E de la forme $f^{-1}\langle B \rangle$, où $B \subset E/R$; en effet, la relation $A = f^{-1}\langle B \rangle$ entraîne $B = f\langle A \rangle$, d’où $A = f^{-1}\langle f\langle A\rangle \rangle$.

Si $(X_i)_{i \in I}$ est une famille de parties saturées de E, les ensembles $\bigcup_{i \in I} X_i$ et $\bigcap_{i \in I} X_i$ sont saturés (II, p. 25, prop. 3 et 4). Si $A = f^{-1}\langle B \rangle$ est une partie saturée de E, il en est de même de $\mathcal{C}_E A = f^{-1}\langle E/R \rangle - f^{-1}\langle B \rangle$ (II, p. 27, prop. 6).

Soit maintenant A une partie quelconque de E. L’ensemble $f^{-1}\langle f\langle A\rangle \rangle$ contient A et est saturé. Réciproquement, si une partie saturée A' de E contient A, on a $f\langle A'\rangle \supset f\langle A\rangle$, d'où $A' = \overline{f}\langle f\langle A'\rangle\rangle \supset \overline{f}\langle f\langle A\rangle\rangle$. On peut donc dire que $\overline{f}\langle f\langle A\rangle\rangle$ est « la plus petite » partie saturée de E contenant A (cf. III, p. 8); cet ensemble est appelé le saturé de A pour la relation R; il est immédiat que c'est la réunion des classes d'équivalence des éléments de A. Si $(X_t)_{t \in I}$ est une famille de parties de E, $A_t$ le saturé de $X_t$ pour R, alors le saturé de $\bigcup_{t \in I} X_t$ est $\bigcup_{t \in I} A_t$ (II, p. 25, prop. 3).

### 5. Applications compatibles avec des relations d'équivalence

Soient R une relation d'équivalence dans un ensemble E, et $f$ une fonction dont l'ensemble de définition est E. On dit que $f$ est compatible avec la relation R si la relation $y = f(x)$ est compatible (par rapport à x) avec la relation $R\{x, x'\}$.

Il revient au même, comme on le voit aussitôt, de dire que la restriction de $f$ à toute classe d'équivalence est une application constante; on dit encore dans ce cas que $f$ est constante sur toute classe d'équivalence suivant R. Si g est l'application canonique de E sur E/R, cela signifie aussi que la relation $g(x) = g(x')$ entraîne $f(x) = f(x')$; par suite (II, p. 20, prop. 9), on a le critère suivant:

C57. Soient R une relation d'équivalence dans un ensemble E, et g l'application canonique de E sur E/R. Pour qu'une application f de E dans F soit compatible avec R, il faut et il suffit que f puisse se mettre sous la forme $h \circ g$, h étant une application de E/R dans F. L'application h est uniquement déterminée par f; si s est une section associée à g, on a $h = f \circ s$.

On dit que h est l'application déduite de f par passage au quotient suivant R.

Soit $f_*$ une application d'un ensemble E dans un ensemble F, et soit $A = f\langle E\rangle \subset F$. Soit R la relation d'équivalence associée à $f$ (II, p. 41); il est clair que $f$ est compatible avec R. En outre, l'application h déduite de $f$ par passage au quotient est une application injective de E/R dans F; en effet, si t et $t'$ sont des classes d'équivalence suivant R, telles que $h(t) = h(t')$, on a $f(x) = f(x')$ pour $x \in t$ et $x' \in t'$, ce qui entraîne $t = t'$ par définition de R. Soit k l'application de E/R sur A déduite de h par passage aux sous-ensembles E/R et A; k est donc bijective. Si j est l'injection canonique de A dans F et g l'application canonique de E sur E/R, on peut écrire $f = j \circ k \circ g$; cette relation est appelée décomposition canonique de f.

Soient $f$ une application d'un ensemble E dans un ensemble F, R une relation d'équivalence dans E, S une relation d'équivalence dans F. Soient u l'application canonique de E sur E/R, v l'application canonique de F sur F/S. On dit que $f$ est compatible avec les relations d'équivalence R et S si $v \circ f$ est compatible avec R; cela signifie que la relation $x \equiv x' \pmod{R}$ entraîne $f(x) \equiv f(x') \pmod{S}$. L'application h de E/R dans F/S déduite de $v \circ f$ par passage au quotient suivant R s’appelle alors l’application déduite de $f$ par passage aux quotients suivant $R$ et $S$; elle est caractérisée par la relation $v \circ f = h \circ u$ (fig. 3).

$$
\begin{array}{ccc}
E & \xrightarrow{f} & F \\
u \downarrow & & v \downarrow \\
E/R & \xrightarrow{h} & F/S
\end{array}
$$

Fig. 3

### 6. Image réciproque d’une relation d’équivalence; relation d’équivalence induite

Soient $\varphi$ une application d’un ensemble $E$ dans un ensemble $F$, et $S$ une relation d’équivalence dans $F$. Si $u$ est l’application canonique de $F$ sur $F/S$, la relation d’équivalence associée à l’application $u \circ \varphi$ de $E$ dans $F/S$ s’appelle l’image réciproque de $S$ par $\varphi$; si $R$ est cette relation, $R \{ x, y \}$ est équivalente à $S \{ \varphi(x), \varphi(y) \}$; les classes d’équivalence suivant $R$ sont les images réciproques par $\varphi$ des classes d’équivalence suivant $S$ qui rencontrent $\varphi(E)$.

En particulier, considérons une relation d’équivalence $R$ dans un ensemble $E$, et soit $A$ une partie de $E$; l’image réciproque de $R$ par l’injection $j$ de $A$ dans $E$ s’appelle la relation d’équivalence induite par $R$-dans $A$, et se note $R_A$.

Les classes d’équivalence suivant $R_A$ sont les traces sur $A$ des classes d’équivalence suivant $R$ qui rencontrent $A$. L’injection $j$ est évidemment compatible avec les relations $R_A$ et $R$; l’application $h$ de $A/R_A$ dans $E/R$ déduite de $j$ par passage aux quotients suivant $R_A$ et $R$ est une application injective de $A/R_A$ dans $E/R$: en effet, si $f$ est l’application canonique de $E$ sur $E/R$, $g$ celle de $A$ sur $A/R_A$, la relation $h(g(x)) = h(g(x'))$, pour $x \in A$ et $x' \in A$, équivaut à $f(x) = f(x')$, donc à $g(x) = g(x')$. L’image $h(A/R_A)$ est égale à $f(A)$; si $k$ est l’application bijective de $A/R_A$ sur $f(A)$ déduite de $h$ par passage aux sous-ensembles $A/R_A$ et $f(A)$, $k$ et son application réciproque sont dites canoniques.

### 7. Quotients de relations d’équivalence

Soient $R$ et $S$ deux relations d’équivalence, par rapport à deux lettres $x, y$. Nous dirons que $S$ est plus fine que $R$ (ou que $R$ est moins fine que $S$) si la relation $S \Rightarrow R$ est vraie. Si $R$ et $S$ sont des relations d’équivalence dans un même ensemble $E$, dire que $S$ est plus fine que $R$ signifie que le graphe de $S$ est contenu dans celui de $R$, ou encore que toute classe d’équivalence suivant $S$ est contenue dans une classe d’équivalence suivant $R$; il revient au même de dire que toute classe d’équivalence suivant $R$ est saturée pour $S$.

#### Exemple 1 {#ens-ii-s6-n7-exa-1 .statement tag=03SF}

La relation « $x \in E$ et $y \in E$ et $x = y$ » est plus fine que toute relation d’équivalence dans $E$; la relation « $x \in E$ et $y \in E$ » est moins fine que toute relation d’équivalence dans $E$.

#### Exemple 2 {#ens-ii-s6-n7-exa-2 .statement tag=03SG}

\* La relation d'équivalence « $x \in \mathbf{Z}$ et $y \in \mathbf{Z}$ et $x - y$ est divisible par 4 » est plus fine que la relation d'équivalence « $x \in \mathbf{Z}$ et $y \in \mathbf{Z}$ et $x - y$ est divisible par 2 ».*

Soient R et S deux relations d'équivalence dans un même ensemble E, telles que S soit plus fine que R. Soient f et g les applications canoniques de E sur E/R et de E sur E/S. La fonction f est compatible avec S; soit h la fonction déduite de f par passage au quotient suivant S; c'est une application de E/S sur E/R. La relation d'équivalence associée à h dans E/S s'appelle le quotient de R par S et se désigne par R/S; la relation $x \equiv y$ (mod. R) est équivalente à $g(x) \equiv g(y)$ (mod. R/S); les classes d'équivalence suivant R/S sont les images par g des classes d'équivalence suivant R. Soit $h = j \circ h_2 \circ h_1$ la décomposition canonique (II, p. 44) de l'application h; $h_1$ est donc l'application canonique de E/S sur (E/S)/(R/S), j est l'application identique de E/R, et $h_2$ est une application bijective de (E/S)/(R/S) sur E/R. L'application $h_2$ et son application réciproque sont dites canoniques.

Considérons inversement une relation d'équivalence quelconque T dans l'ensemble E/S, et soit R la relation d'équivalence dans E, image réciproque par g de la relation T (II, p. 45); comme la relation $x \equiv y$ (mod. R) est équivalente à $g(x) \equiv g(y)$ (mod. T), on voit que T est équivalente à R/S.

### 8. Produit de deux relations d'équivalence

Soient R$\{x, y\}$ et R'$\{x', y'\}$ deux relations d'équivalence. Désignons par S$\{u, v\}$ la relation

$$
(\exists x)(\exists y)(\exists x')(\exists y')(u = (x, x') \text{ et } v = (y, y') \text{ et } R\{x, y\} \text{ et } R'\{x', y'\});
$$

on vérifie aisément que S$\{u, v\}$ est une relation d'équivalence, que l'on appelle produit de R et R' et qu'on désigne par R $\times$ R'. Supposons que R soit une relation d'équivalence dans un ensemble E, et R' une relation d'équivalence dans un ensemble E'. La relation S$\{u, u\}$ est alors équivalente à

$$
(\exists x)(\exists x')(u = (x, x') \text{ et } R\{x, x'\} \text{ et } R'\{x', x'\})
$$

c'est-à-dire à $(\exists x)(\exists x')(u = (x, x') \text{ et } x \in E \text{ et } x' \in E')$, donc à $u \in E \times E'$; il en résulte que R $\times$ R' est une relation d'équivalence dans E $\times$ E'. Si $u = (x, x')$ est un élément de E $\times$ E', la relation S$\{u, v\}$ est équivalente à

$$
(\exists y)(\exists y')(v = (y, y') \text{ et } R\{x, y\} \text{ et } R'\{x', y'\});
$$

si G et G' sont les graphes de R et R', cette relation est encore équivalente à $v \in G(x) \times G'(x')$. Toute classe d'équivalence suivant R $\times$ R' est donc le produit d'une classe d'équivalence suivant R et d'une classe d'équivalence suivant R', et réciproquement.

Soient f et f' les applications canoniques de E sur E/R et de E' sur E'/R', et soit $f \times f'$ l'extension canonique de f et f' aux ensembles produits (II, p. 21); on a donc $(f \times f')(x, x') = (f(x), f'(x'))$ pour $(x, x') \in E \times E'$. L'image réciproque par $f \times f'$ d'une élément $(u, u')$ de $(E/R) \times (E'/R')$ n'est autre que le produit $u \times u'$ de la classe d'équivalence $u$ suivant $R$ et de la classe d'équivalence $u'$ suivant $R'$; il en résulte que la relation d'équivalence associée à $f \times f'$ est équivalente à $R \times R'$. L'application $f \times f'$ peut donc se mettre sous la forme $h \circ g$, où $g$ est l'application canonique de $E \times E'$ sur $(E \times E')/(R \times R')$ et où $h$ est une application bijective de $(E \times E')/(R \times R')$ sur $(E/R) \times (E'/R')$; cette application et son application réciproque sont dites *canoniques*.

#### Remarque {#ens-ii-s6-n8-rem-1 .statement tag=03IY}

Soit $P\{x, x'\}$ une relation où ne figurent pas les lettres $y$ et $y'$; on dit que $P$ est *compatible* avec les relations d'équivalence $R\{x, y\}$ et $R'\{x', y'\}$ (par rapport à $x$ et $x'$) si la relation $(P\{x, x'\}$ et $R\{x, y\}$ et $R'\{x', y'\})$ entraîne $P\{y, y'\}$. Soit $Q\{u\}$ la relation $(\exists x)(\exists x')(u = (x, x'))$ et $P\{x, x'\}$; il revient au même de dire que $Q\{u\}$ est compatible (par rapport à $u$) avec la relation d'équivalence $S\{u, v\}$, produit de $R$ et de $R'$.

### 9. Classes d'objets équivalents

Soit $R\{x, y\}$ une relation d'équivalence ne possédant pas nécessairement de graphe. Il est immédiat que si $x, x', y$ sont trois lettres distinctes, la relation $R\{x, x'\}$ entraîne $R\{x, y\} \Leftrightarrow R\{x', y\}$, donc aussi la relation $(\forall y)(R\{x, y\} \Leftrightarrow R\{x', y\})$. Compte tenu du schéma S7 (I, p. 38) on voit que, si on pose $\theta\{x\} = \tau_y(R\{x, y\})$, la relation $R\{x, x'\}$ implique $\theta\{x\} = \theta\{x'\}$. Notons d'autre part que, par définition, $R\{x, \theta\{x\}\}$ n'est autre que la relation $(\exists y)R\{x, y\}$, donc (II, p. 40) est équivalente à $R\{x, x'\}$. On en conclut que la relation $(R\{x, x\}$ et $R\{x', x'\}$ et $\theta\{x\} = \theta\{x'\})$ est *équivalente* à $R\{x, x'\}$; en effet, elle entraîne, par S6 (I, p. 38) la relation

$$(R\{x, x\} \text{ et } R\{x', x'\} \text{ et } R\{x', \theta\{x\}\} \Leftrightarrow R\{x', \theta\{x'\}\}),$$

donc aussi $(R\{x, \theta\{x\}\}$ et $R\{x', \theta\{x'\}\})$ et finalement $R\{x, x'\}$ par transitivité et symétrie; comme on sait d'autre part que $R\{x, x'\}$ entraîne $(R\{x, x\}$ et $R\{x', x'\})$, notre assertion est démontrée. On dit que le terme $\theta\{x\}$ est *la classe d'objets équivalents* à $x$ (pour la relation $R$).

Supposons maintenant que $T$ soit un terme ne contenant pas $x$, tel que la relation

(1)
$$(\forall y)(R\{y, y\} \Rightarrow (\exists x)(x \in T \text{ et } R\{x, y\}))$$

soit vraie. Alors, la relation $(\exists x)(R\{x, x\}$ et $z = \theta\{x\})$ est *collectivisante en* $z$. On peut en effet supposer que $x \in T$ implique $R\{x, x\}$; il suffit de remplacer $T$ par l'ensemble des $x \in T$ tels que $R\{x, x\}$ (en observant que $R\{x, y\}$ entraîne $R\{x, x\}$). Soit alors $\Theta$ l'ensemble des objets de la forme $\theta\{x\}$ pour $x \in T$ (II, p. 6). Supposons que $R\{y, y\}$ soit vraie; alors il existe $x \in T$ tel que l'on ait $R\{x, y\}$, donc $\theta\{y\} = \theta\{x\} \in \Theta$. On dit que $\Theta$ est *l'ensemble des classes d'objets équivalents* suivant $R$, et pour tout $x$ tel que $R\{x, x\}, \theta\{x\}$ est l'*unique* élément $z \in \Theta$ tel que l'on ait $R\{x, z\}$.

Sous les mêmes hypothèses, soit $A\{x\}$ un terme tel que $R\{x, y\}$ entraîne $A\{x\} = A\{y\}$. Alors la relation $(\exists x)(R\{x, x\}$ et $z = A\{x\})$ est aussi collectivisante en $z$, car $R\{x, x\}$, étant équivalente à $R\{x, \theta\{x\}\}$, entraîne $A\{x\} = A\{\theta\{x\}\}$, et par suite, si $E$ est l'ensemble des objets de la forme $A\{t\}$ pour $t \in \Theta$, $R\{x, x'\}$ entraîne $A\{x'\} \in E$. Si $f$ est la fonction $t \mapsto A\{t\}$ ($t \in \Theta, A\{t\} \in E$), on voit donc que la relation $R\{x, x'\}$ entraîne $A\{x'\} = f(\theta\{x'\})$.

En particulier, si $R$ est une relation d'équivalence *dans un ensemble* $F$, on peut prendre pour $A\{x\}$ la *classe d'équivalence de x suivant R* (II, p. 41), et la fonction $f$ est alors une *bijection* de $\Theta$ sur l'ensemble quotient $F/R$, ce qui justifie la terminologie introduite.

\* Exemple. — Soit $R\{x, y\}$ la relation d'équivalence « $x$ et $y$ sont deux espaces vectoriels de même dimension finie sur $\mathbf{C}$ », qui n'admet pas de graphe. Elle vérifie la condition (1) en prenant pour $T$ l'ensemble des sous-espaces vectoriels de $\mathbf{C}^{(\mathbf{N})}$, ou le sous-ensemble $T'$ de $T$ formé des $\mathbf{C}^n$ ($n \in \mathbf{N}$), où on convient que $\mathbf{C}^0$ est réduit au point 0 de $\mathbf{C}^{(\mathbf{N})}$, et $\mathbf{C}^n$ pour $n > 0$ est la somme des $n$ premiers composants de la somme directe $\mathbf{C}^{(\mathbf{N})}$.*

Exercises

## EXERCICES {#ens-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
