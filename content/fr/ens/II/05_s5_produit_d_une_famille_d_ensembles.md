---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 5
section_title: Produit d'une famille d'ensembles
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E II.30-E II.39, E II.51
pdf_pages: 0082-0091, 0103-0103
extraction: ocr
subsections:
    - "no": 1
      title: L’axiome de l’ensemble des parties
      page: 30
      pdf_page: 82
    - "no": 2
      title: Ensemble des applications d’un ensemble dans un ensemble
      page: 31
      pdf_page: 83
    - "no": 3
      title: Définition du produit d'une famille d'ensembles
      page: 32
      pdf_page: 84
    - "no": 4
      title: Produits partiels
      page: 33
      pdf_page: 85
    - "no": 5
      title: Associativité des produits d’ensembles
      page: 35
      pdf_page: 87
    - "no": 6
      title: Formules de distributivité
      page: 35
      pdf_page: 87
    - "no": 7
      title: Extension d'applications aux produits
      page: 38
      pdf_page: 90
statements: 24
exercises: 5
content_sha256: db0022e62383130cc1e0ad1d77b9b8d305dc0362a0685af8b0084238db199908
---

## § 5. PRODUIT D’UNE FAMILLE D’ENSEMBLES

### 1. L’axiome de l’ensemble des parties

A3. $$(\forall X) \operatorname{Coll}_Y(Y \subset X).$$

Cet axiome signifie que, pour tout ensemble $X$, il existe un ensemble dont les éléments sont toutes les parties de $X$, savoir l’ensemble $\{Y \mid (Y \subset X)\}$ (II, p. 3); on le désigne par $\mathfrak{P}(X)$, et on l’appelle l’ensemble des parties de $X$. Il est clair que, si $X \subset X'$, on a $\mathfrak{P}(X) \subset \mathfrak{P}(X')$.

Soient $A$ et $B$ deux ensembles, $\Gamma$ une correspondance entre $A$ et $B$. La fonction $X \mapsto \Gamma\langle X \rangle$ ($X \in \mathfrak{P}(A), \Gamma\langle X \rangle \in \mathfrak{P}(B)$) s’appelle l’extension canonique (ou simplement extension) de $\Gamma$ aux ensembles de parties, et se note $\hat{\Gamma}$; c’est une application de $\mathfrak{P}(A)$ dans $\mathfrak{P}(B)$. Si $\Gamma'$ est une correspondance entre $B$ et un ensemble $C$, la formule $(\Gamma' \circ \Gamma)\langle X \rangle = \Gamma'\langle \Gamma\langle X \rangle \rangle$ montre que l’extension de $\Gamma' \circ \Gamma$ aux ensembles de parties est l’application $\hat{\Gamma}' \circ \hat{\Gamma}$.

#### Proposition 1 {#ens-ii-s5-prop-1 .statement tag=03IJ}

1° Si $f$ est une surjection d’un ensemble $E$ sur un ensemble $F$, l’extension canonique $\hat{f}$ est une surjection de $\mathfrak{P}(E)$ sur $\mathfrak{P}(F)$.

2° Si $f$ est une injection de $E$ dans $F$, l’extension canonique $\hat{f}$ est une injection de $\mathfrak{P}(E)$ dans $\mathfrak{P}(F)$.

1° Si $s$ est une section associée à $f$, $f \circ s$ est l’application identique de $F$, donc $\hat{f} \circ \hat{s}$ est l’application identique de $\mathfrak{P}(F)$, ce qui montre que $f$ est une surjection et $\hat{s}$ une section associée (II, p. 18).

2° La proposition est immédiate si $E = \varnothing$, puisqu’alors $\mathfrak{P}(E) = \{\varnothing\}$. Si $E \neq \varnothing$ et si $r$ est une rétraction associée à $f$, $r \circ f$ est l’application identique de $E$, donc $\hat{r} \circ \hat{f}$ est l’application identique de $\mathfrak{P}(E)$, ce qui montre que $\hat{f}$ est une injection et $\hat{r}$ une rétraction associée (II, p. 18).

### 2. Ensemble des applications d’un ensemble dans un ensemble

Soient E et F des ensembles. Le graphe d’une application de E dans F est une partie de $E \times F$. L’ensemble des éléments de $\mathfrak{P}(E \times F)$ qui possèdent la propriété d’être des graphes d’applications de E dans F est donc une partie de $\mathfrak{P}(E \times F)$ que l’on désigne par $F^E$. L’ensemble des triplets $f = (G, E, F)$, pour $G \in F^E$ est donc l’ensemble des applications de E dans F ; on le désigne par $\mathcal{F}(E; F)$. Il est clair que $G \mapsto (G, E, F)$ est une bijection (dite canonique) de $F^E$ sur $\mathcal{F}(E; F)$. L’existence de cette bijection permet de traduire aussitôt toute proposition relative à l’ensemble $F^E$ en une proposition relative à $\mathcal{F}(E; F)$, et vice-versa.

Soient E, E’, F, F’ des ensembles. Soient u une application de E’ dans E, et v une application de F dans F’. La fonction $f \mapsto v \circ f \circ u$ ($f \in \mathcal{F}(E; F)$) est une application de $\mathcal{F}(E; F)$ dans $\mathcal{F}(E'; F')$.

#### Proposition 2 {#ens-ii-s5-prop-2 .statement tag=03Q5}

1° Si u est une surjection de E’ sur E, et v une injection de F dans F’, l’application $f \mapsto v \circ f \circ u$ est injective.

2° Si u est une injection de E’ dans E, et v une surjection de F sur F’, l’application $f \mapsto v \circ f \circ u$ est surjective.

Bornons-nous au cas où les ensembles E’, F sont non vides, la proposition se vérifiant trivialement dans les autres cas.

1° Soient s une section associée à u, r une rétraction associée à v (II, p. 18, déf. 11). On a $r \circ (v \circ f \circ u) \circ s = \mathrm{Id}_F \circ f \circ \mathrm{Id}_E = f$, ce qui montre que $f \mapsto v \circ f \circ u$ est injective.

2° Soient $r'$ une rétraction associée à u, $s'$ une section associée à v. Pour toute application $f': E' \to F'$, on a $v \circ (s' \circ f' \circ r') \circ u = f'$, ce qui montre que $f \mapsto v \circ f \circ u$ est surjective.

#### Corollaire {#ens-ii-s5-n2-cor-1 .statement tag=03Q6}

Si u est une bijection de E’ sur E et v une bijection de F sur F’, $f \mapsto v \circ f \circ u$ est bijective.

Soient A, B, C trois ensembles, et f une application de $B \times C$ dans A. Pour tout $y \in C$, soit $f_y$ l’application partielle $x \mapsto f(x, y)$ de B dans A (II, p. 21); la fonction $y \mapsto f_y$ est une application de C dans $\mathcal{F}(B; A)$. Inversement, pour toute application g de C dans $\mathcal{F}(B; A)$, il existe une application et une seule f de $B \times C$ dans A telle que $g(y) = f_y$ pour tout $y \in C$, savoir l’application $(x, y) \mapsto (g(y))(x)$. Donc:

#### Proposition 3 {#ens-ii-s5-prop-3 .statement tag=03Q7}

Si, pour toute application f de $B \times C$ dans A, on désigne par $\tilde{f}$ l’application $y \mapsto f_y$ de C dans $\mathcal{F}(B; A)$, la fonction $f \mapsto \tilde{f}$ est une bijection (dite canonique) de $\mathcal{F}(B \times C; A)$ sur $\mathcal{F}(C; \mathcal{F}(B; A))$.

On définit de la même manière une bijection (dite canonique) de $\mathcal{F}(B \times C; A)$ sur $\mathcal{F}(B; \mathcal{F}(C; A))$. En raison de la correspondance biunivoque entre applications et graphes fonctionnels, les bijections précédentes fournissent des bijections (dites canoniques) de $A^{B \times C}$ sur $(A^B)^C$ (resp. $(A^C)^B$).

### 3. Définition du produit d'une famille d'ensembles

Soient $(X_i)_{i \in I}$ une famille d'ensembles, F un graphe fonctionnel ayant I pour ensemble de définition, et tel que, pour tout $i \in I$, on ait $F(i) \in X_i$; on en déduit que, pour tout $i \in I$, on a $F(i) \in A = \bigcup_{i \in I} X_i$, et par suite que F est un élément de $\mathfrak{P}(I \times A)$. Les graphes fonctionnels ayant la propriété précédente forment donc une partie de $\mathfrak{P}(I \times A)$.

#### Définition 1 {#ens-ii-s5-def-1 .statement tag=03Q8}

Soit $(X_i)_{i \in I}$ une famille d'ensembles. L'ensemble des graphes fonctionnels F, ayant I pour ensemble de définition, et tels que $F(i) \in X_i$ pour tout $i \in I$, s'appelle le produit de la famille d'ensembles $(X_i)_{i \in I}$ et se désigne par $\prod_{i \in I} X_i$. Pour tout $i \in I$, $X_i$ s'appelle le facteur d'indice $i$ du produit $\prod_{i \in I} X_i$; l'application

$$
F \mapsto F(i) \quad (F \in \prod_{i \in I} X_i, F(i) \in X_i)
$$

s'appelle la fonction coordonnée (ou projection) d'indice $i$, et se note $\mathrm{pr}_i$.

On dit que $F(i)$ est la coordonnée d'indice $i$ (ou projection d'indice $i$) de F ; l'image $\mathrm{pr}_i(A)$ d'une partie A de $\prod_{i \in I} X_i$ par la fonction coordonnée d'indice $i$ s'appelle la projection d'indice $i$ de A ; on vérifie aisément que $A \subset \prod_{i \in I} \mathrm{pr}_i(A)$.

On utilise souvent la notation $(x_i)_{i \in I}$ pour désigner les éléments de $\prod_{i \in I} X_i$ (II, p. 16).

Si $I = \varnothing$, l'ensemble $\prod_{i \in I} X_i$ ne possède qu'un seul élément, savoir l'ensemble vide (II, p. 14, Exemple 1).

Lorsque tous les facteurs $X_i$ du produit $\prod_{i \in I} X_i$ sont égaux à un même ensemble E, on a $\prod_{i \in I} X_i = E^I$, comme il résulte aussitôt des définitions.

Si $(X_i)_{i \in I}$ est une famille d'ensembles quelconque, E un ensemble tel que $\bigcup_{i \in I} X_i \subset E$, la déf. 1 montre que $\prod_{i \in I} X_i \subset E^I$; il y a donc correspondance biunivoque entre $\prod_{i \in I} X_i$ et un ensemble d'applications de I dans E (partie de $\mathcal{F}(I; E)$).

Si $I = \{\alpha\}$ est un ensemble à un seul élément, on a $\prod_{i \in I} X_i = X_{\alpha}^{\{\alpha\}}$; l'application

F ↦ F(α) est alors une application bijective de $\prod_{\iota \in \{\alpha\}} X_\iota$ sur $X_\alpha$ (dite canonique, ainsi que l’application réciproque).

Soient A et B des ensembles, et soient $\alpha, \beta$ deux objets distincts (il en existe, par exemple $\varnothing$ et $\{\varnothing\}$). Considérons le graphe $\{(\alpha, A), (\beta, B)\}$, qui est évidemment fonctionnel, et n’est autre que la famille $(X_\iota)_{\iota \in \{\alpha, \beta\}}$ telle que $X_\alpha = A$, $X_\beta = B$. Pour tout couple $(x, y) \in A \times B$, soit $f_{x, y}$ le graphe fonctionnel $\{(\alpha, x), (\beta, y)\}$. Il est immédiat que la fonction $(x, y) \mapsto f_{x, y}$ est une application bijective de $A \times B$ sur $\prod_{\iota \in \{\alpha, \beta\}} X_\iota$, dont l’application réciproque est $g \mapsto (g(\alpha), g(\beta))$; ces deux applications sont dites canoniques. Nous utiliserons dans la suite cette correspondance biunivoque pour démontrer des propriétés du produit de deux ensembles à partir de propriétés du produit d’une famille d’ensembles.

Soit $(X_\iota)_{\iota \in I}$ une famille d’ensembles dont chacun est un ensemble à un seul élément, soit $X_\iota = \{a_\iota\}$; alors le produit $\prod_{\iota \in I} X_\iota$ est un ensemble réduit au seul élément $(a_\iota)_{\iota \in I}$.

Soit E un ensemble ; les graphes des applications constantes $\iota \mapsto x$ de I dans E forment une partie $\Delta$ du produit $E^I$ appelée diagonale; si $\bar{x}$ désigne le graphe de l’application $\iota \mapsto x$ (pour $x \in E$), l’application $x \mapsto \bar{x}$ est une injection de E dans $E^I$ dite application diagonale.

#### Proposition 4 {#ens-ii-s5-prop-4 .statement tag=03IK}

*Soient* $(X_\iota)_{\iota \in I}$ *une famille d’ensembles, u une bijection d’un ensemble K sur l’ensemble I, U son graphe. L’application* $F \mapsto F \circ U$ *de* $\prod_{\iota \in I} X_\iota$ *dans* $\prod_{\kappa \in K} X_{u(\kappa)}$ *est bijective.*

Soit $A = \bigcup_{\iota \in I} X_\iota = \bigcup_{\kappa \in K} X_{u(\kappa)}$ (II, p. 22, prop. 1). L’application $F \mapsto F \circ U$ ($F \in A^I$) est une application bijective de $A^I$ sur $A^K$ (II, p. 31, prop. 2). Il est évident que la condition « pour tout $\iota \in I$, $F(\iota) \in X_\iota$ » est équivalente à « pour tout $\kappa \in K$, $(F \circ U)(\kappa) \in X_{u(\kappa)}$ », ce qui démontre la proposition.

### 4. Produits partiels

Soient $(X_\iota)_{\iota \in I}$ une famille d’ensembles, et J une partie de I ; on dit que $\prod_{\iota \in J} X_\iota$ est un *produit partiel* de $\prod_{\iota \in I} X_\iota$. Si $f$ est une fonction de graphe $F \in \prod_{\iota \in I} X_\iota$, $F \circ \Delta_J$ (où $\Delta_J$ est la diagonale de $J \times J$) est le graphe de la *restriction* de $f$ à J. On a évidemment $F \circ \Delta_J \in \prod_{\iota \in J} X_\iota$; l’application $F \mapsto F \circ \Delta_J$ de $\prod_{\iota \in I} X_\iota$ dans $\prod_{\iota \in J} X_\iota$ s’appelle la *projection d’indice* J et se note $\mathrm{pr}_J$.

#### Proposition 5 {#ens-ii-s5-prop-5 .statement tag=03Q9}

*Soient* $(X_\iota)_{\iota \in I}$ *une famille d’ensembles, et J une partie de I. Si, pour tout* $\iota \in I$, *on a* $X_\iota \neq \varnothing$, *la projection* $\mathrm{pr}_J$ *est une application de* $\prod_{\iota \in I} X_\iota$ *sur* $\prod_{\iota \in J} X_\iota$.

D’après les remarques faites ci-dessus, il revient au même de démontrer la proposition suivante:

#### Proposition 6 {#ens-ii-s5-prop-6 .statement tag=03QA}

Soit $(X_i)_{i \in I}$ une famille d’ensembles telle que $X_i \neq \varnothing$ pour tout $i \in I$. Etant donnée une application $g$ de $J \subset I$ dans $A = \bigcup_{i \in I} X_i$, telle que $g(i) \in X_i$ pour tout $i \in J$, il existe un prolongement $f$ de $g$ à $I$, tel que $f(i) \in X_i$ pour tout $i \in I$.

En effet, pour tout $i \in I - J$, désignons par $T_i$ le terme $\tau_y(y \in X_i)$. Comme $X_i \neq \varnothing$ par hypothèse, on a $T_i \in X_i$ pour tout $i \in I - J$ (I, p. 32). Si $G$ est le graphe de $g$, le graphe $G \cup (\bigcup_{i \in I - J} \{(i, T_i)\})$ est le graphe d’une fonction $f$ répondant à la question, comme on le vérifie aussitôt.

#### Corollaire 1 {#ens-ii-s5-prop-6-cor-1 .statement tag=03QB}

Soit $(X_i)_{i \in I}$ une famille d’ensembles telle que, pour tout $i \in I$, on ait $X_i \neq \varnothing$. Alors, pour tout $\alpha \in I$, la projection $\mathrm{pr}_\alpha$ est une application de $\prod_{i \in I} X_i$ sur $X_\alpha$.

Il suffit d’appliquer la prop. 5 à la partie $J = \{\alpha\}$ de $I$, et de remarquer que $\mathrm{pr}_\alpha$ est composée de l’application canonique de $X_\alpha^{(\alpha)}$ sur $X_\alpha$ et de l’application $\mathrm{pr}_{\{\alpha\}}$.

#### Corollaire 2 {#ens-ii-s5-prop-6-cor-2 .statement tag=03QC}

Soit $(X_i)_{i \in I}$ une famille d’ensembles. Pour que $\prod_{i \in I} X_i = \varnothing$, il faut et il suffit qu’il existe un $i \in I$ tel que $X_i = \varnothing$.

En effet, si, pour tout $i \in I$, on a $X_i \neq \varnothing$, on a aussi $\prod_{i \in I} X_i \neq \varnothing$ comme il résulte du cor.1; inversement, si $\prod_{i \in I} X_i \neq \varnothing$, la relation $\mathrm{pr}_\alpha(\prod_{i \in I} X_i) \subset X_\alpha$ montre que l’on a $X_\alpha \neq \varnothing$ pour tout $\alpha \in I$.

On voit donc que, si on a une famille $(X_i)_{i \in I}$ d’ensembles non vides, on peut introduire (à titre de constante auxiliaire) une fonction $f$ dont $I$ est l’ensemble de définition, et qui est telle que $f(i) \in X_i$ pour tout $i \in I$. On dira en pratique: « Prenons dans chaque ensemble $X_i$ un élément $x_i$ ». Intuitivement, on a donc « choisi » un élément $x_i$ dans chacun des $X_i$; l’introduction du signe logique $\tau$ et des critères qui en gouvernent l’emploi nous a dispensés d’avoir à formuler ici un « axiome de choix » pour légitimer cette opération (cf. Ens. R, p. 21).

#### Corollaire 3 {#ens-ii-s5-prop-6-cor-3 .statement tag=03QD}

Soient $(X_i)_{i \in I}$ et $(Y_i)_{i \in I}$ deux familles d’ensembles ayant le même ensemble d’indices $I$. Si, pour tout $i \in I$, on a $X_i \subset Y_i$, on a aussi $\prod_{i \in I} X_i \subset \prod_{i \in I} Y_i$.

Réciproquement, si $\prod_{i \in I} X_i \subset \prod_{i \in I} Y_i$ et si, pour tout $i \in I$, on a $X_i \neq \varnothing$, on a $X_i \subset Y_i$ pour tout $i \in I$.

La première assertion est évidente, et la seconde résulte du cor. 1 de la prop. 6, car on a alors, pour tout $\alpha \in I$,

$$
X_\alpha = \mathrm{pr}_\alpha(\prod_{i \in I} X_i) \subset \mathrm{pr}_\alpha(\prod_{i \in I} Y_i) = Y_\alpha.
$$

### 5. Associativité des produits d’ensembles

#### Proposition 7 {#ens-ii-s5-prop-7 .statement tag=03IN}

Soit $(X_i)_{i \in I}$ une famille d’ensembles. Soit $(J_\lambda)_{\lambda \in L}$ une partition de $I$; l’application $f \mapsto (\mathrm{pr}_{J_\lambda} f)_{\lambda \in L}$ de $\prod_{i \in I} X_i$ dans l’ensemble produit $\prod_{\lambda \in L} (\prod_{i \in J_\lambda} X_i)$ est bijective (« associativité » des produits d’ensembles).

D’après l’interprétation de $\mathrm{pr}_{J_\lambda} f$ comme graphe de la restriction d’une fonction de graphe $f$ (II, p. 33), dire que l’application $f \mapsto (\mathrm{pr}_{J_\lambda} f)_{\lambda \in L}$ est bijective signifie que, pour toute famille $(v_\lambda)_{\lambda \in L}$, où $v_\lambda$ est une application de $J_\lambda$ dans $\bigcup_{i \in I} X_i$, il existe une application et une seule $u$ de $I$ dans $\bigcup_{i \in I} X_i$ telle que, pour tout $\lambda \in L$, $v_\lambda$ soit la restriction de $u$ à $J_\lambda$; or, cela résulte de ce que $(J_\lambda)_{\lambda \in L}$ est une partition de $I$ (II, p. 29, prop. 8).

L’application définie dans la prop. 7 et sa réciproque sont dites canoniques.

#### Remarque 1 {#ens-ii-s5-n5-rem-1 .statement tag=03SA}

Soient $\alpha, \beta$ deux objets distincts, et $(J_\lambda)_{\lambda \in \{\alpha, \beta\}}$ une partition de $I$ en deux ensembles $J_\alpha, J_\beta$. On obtient une application bijective (dite encore canonique) du produit $\prod_{i \in I} X_i$ sur $(\prod_{i \in J_\alpha} X_i) \times (\prod_{i \in J_\beta} X_i)$ en composant l’application canonique de $\prod_{\lambda \in \{\alpha, \beta\}} (\prod_{i \in J_\lambda} X_i)$ sur $(\prod_{i \in J_\alpha} X_i) \times (\prod_{i \in J_\beta} X_i)$ et l’application canonique de $\prod_{i \in I} X_i$ sur $\prod_{\lambda \in \{\alpha, \beta\}} (\prod_{i \in J_\lambda} X_i)$. Lorsque, pour tout $i \in J_\beta$, $X_i$ est un ensemble à un seul élément, on en déduit que $\mathrm{pr}_{J_\alpha}$ est une application bijective de $\prod_{i \in I} X_i$ sur $\prod_{i \in J_\alpha} X_i$.

#### Remarque 2 {#ens-ii-s5-n5-rem-2 .statement tag=03SB}

Soient $\alpha, \beta, \gamma$ des objets deux à deux distincts (il en existe, par exemple $\varnothing$, $\{\varnothing\}$ et $\{\{\varnothing\}\}$), et soient $A, B, C$ des ensembles. Considérons le graphe fonctionnel $\{(\alpha, A), (\beta, B), (\gamma, C)\}$, c’est-à-dire la famille d’ensembles $(X_i)_{i \in \{\alpha, \beta, \gamma\}}$ telle que $X_\alpha = A$, $X_\beta = B$, $X_\gamma = C$. A la partition de $\{\alpha, \beta, \gamma\}$ formée des deux ensembles $\{\alpha, \beta\}$ et $\{\gamma\}$ correspond une bijection canonique de $\prod_{i \in \{\alpha, \beta, \gamma\}} X_i$ sur le produit $(\prod_{i \in \{\alpha, \beta\}} X_i) \times X_{\{\gamma\}}$, et par suite une bijection (qu’on appelle encore canonique) de $\prod_{i \in \{\alpha, \beta, \gamma\}} X_i$ sur $A \times B \times C$ (II, p. 9), faisant correspondre à tout graphe $f \in \prod_{i \in \{\alpha, \beta, \gamma\}} X_i$ l’élément $(f(\alpha), f(\beta), f(\gamma))$ de $A \times B \times C$. Tenant compte de la prop. 4 (II, p. 33), on peut ainsi mettre en correspondance biunivoque deux quelconques des ensembles $A \times B \times C, B \times C \times A, C \times A \times B, B \times A \times C, A \times C \times B, C \times B \times A$.

### 6. Formules de distributivité

#### Proposition 8 {#ens-ii-s5-prop-8 .statement tag=03IO}

Soit $((X_{\lambda, i})_{i \in J_\lambda})_{\lambda \in L}$ une famille (admettant $L$ pour ensemble d’indices) de familles d’ensembles. On suppose $L \neq \varnothing$ et $J_\lambda \neq \varnothing$ pour tout $\lambda \in L$. Soit $I = \prod_{\lambda \in L} J_\lambda \neq \varnothing$. On a
$$
\bigcup_{\lambda \in L} (\bigcap_{i \in J_\lambda} X_{\lambda, i}) = \bigcap_{f \in I} (\bigcup_{\lambda \in L} X_{\lambda, f(\lambda)})
$$
et
$$
\bigcap_{\lambda \in L} (\bigcup_{i \in J_\lambda} X_{\lambda, i}) = \bigcup_{f \in I} (\bigcap_{\lambda \in L} X_{\lambda, f(\lambda)})
$$

(« distributivité » de la réunion par rapport à l’intersection et de l’intersection par rapport à la réunion).

Soit $x$ un élément de $\bigcup_{\lambda \in L} (\bigcap_{i \in J_\lambda} X_{\lambda, i})$. Soit $f$ un élément quelconque de $I$. Il existe un indice $\lambda$ tel que $x \in \bigcap_{i \in J_\lambda} X_{\lambda, i}$; on a par suite $x \in X_{\lambda, f(\lambda)}$, d’où $x \in \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$. Ceci étant vrai pour tout $f \in I$, on a $x \in \bigcap_{f \in I} (\bigcup_{\lambda \in L} X_{\lambda, f(\lambda)})$. Soit maintenant $x$ un objet qui n’appartient pas à l’ensemble $\bigcup_{\lambda \in L} (\bigcap_{i \in J_\lambda} X_{\lambda, i})$. Il en résulte que, pour tout $\lambda \in L$, on a $x \notin \bigcap_{i \in J_\lambda} X_{\lambda, i}$, ce qui signifie que, pour tout $\lambda \in L$, l’ensemble $J'_\lambda$ des $i \in J_\lambda$ tels que $x \notin X_{\lambda, i}$ est non vide. D’après le cor. 2 de la prop. 5 (II, p. 34), il existe un graphe fonctionnel $f$ dont l’ensemble de définition est $L$ et qui est tel que, pour tout $\lambda \in L$, $f(\lambda) \in J'_\lambda$. On a donc $f \in I$ et, pour tout $\lambda \in L$, $x \notin X_{\lambda, f(\lambda)}$. On en déduit que $x \notin \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$, et par suite $x \notin \bigcap_{f \in I} (\bigcup_{\lambda \in L} X_{\lambda, f(\lambda)})$.

La première formule est donc démontrée. La seconde s’en déduit, en appliquant la première formule à la famille $((\mathcal{C}_A X_{\lambda, i})_{i \in J_\lambda})_{\lambda \in L}$, où $A$ désigne la réunion $\bigcup_{\lambda \in L} (\bigcup_{i \in J_\lambda} X_{\lambda, i})$.

#### Corollaire {#ens-ii-s5-n6-cor-1 .statement tag=03IP}

*Soient* $(X_i)_{i \in I}$ *et* $(Y_k)_{k \in K}$ *deux familles d’ensembles dont les ensembles d’indices sont non vides.* *On a*

$$
(\bigcap_{i \in I} X_i) \cup (\bigcap_{k \in K} Y_k) = \bigcap_{(i, k) \in I \times K} (X_i \cup Y_k)
$$

et

$$
(\bigcup_{i \in I} X_i) \cap (\bigcup_{k \in K} Y_k) = \bigcup_{(i, k) \in I \times K} (X_i \cap Y_k).
$$

Soient $\alpha$ et $\beta$ deux objets distincts; il suffit d’appliquer les formules de la prop. 8 au cas où $L = \{\alpha, \beta\}$, $J_\alpha = I$, $J_\beta = K$, et à la famille $((Z_{\lambda, \mu})_{\mu \in J_\lambda})_{\lambda \in L}$ telle que $Z_{\alpha, i} = X_i$ pour tout $i \in I$ et $Z_{\beta, k} = Y_k$ pour tout $k \in K$; tenant compte de l’existence de la bijection canonique de $\prod_{\lambda \in L} J_\lambda$ sur $I \times K$ (II, p. 33) et de la prop. 1 de II, p. 30, on obtient les formules énoncées.

#### Proposition 9 {#ens-ii-s5-prop-9 .statement tag=03IQ}

*Soit* $((X_{\lambda, i})_{i \in J_\lambda})_{\lambda \in L}$ *une famille (admettant* $L$ *comme ensemble d’indices)* *de familles d’ensembles.* *Soit* $I = \prod_{\lambda \in L} J_\lambda$. *On a*

$$
\prod_{\lambda \in L} (\bigcup_{i \in J_\lambda} X_{\lambda, i}) = \bigcup_{f \in I} (\prod_{\lambda \in L} X_{\lambda, f(\lambda)})
$$

*et* (*si* $L \neq \varnothing$ *et* $J_\lambda \neq \varnothing$ *pour tout* $\lambda \in L$)

$$
\prod_{\lambda \in L} (\bigcap_{i \in J_\lambda} X_{\lambda, i}) = \bigcap_{f \in I} (\prod_{\lambda \in L} X_{\lambda, f(\lambda)}).
$$

(« distributivité » du produit par rapport à la réunion et à l’intersection).

La première formule est immédiate si $L = \varnothing$ ou si $J_\lambda = \varnothing$ pour un indice λ ∈ L. Sinon, soit g un élément de $\prod_{\lambda \in L} (\bigcup_{i \in J_\lambda} X_{\lambda, i})$; pour tout λ ∈ L, il existe donc un i ∈ J_λ tel que $g(\lambda) \in X_{\lambda, i}$; autrement dit, l’ensemble H_λ des i ∈ J_λ tels que $g(\lambda) \in X_{\lambda, i}$ n’est pas vide. D’après II, p. 34, cor. 2, il existe donc un graphe fonctionnel f dont l’ensemble de définition est L et qui est tel que, pour tout λ ∈ L, $f(\lambda) \in H_\lambda$, ce qui signifie que $g(\lambda) \in X_{\lambda, f(\lambda)}$. On a donc $g \in \prod_{\lambda \in L} X_{\lambda, f(\lambda)}$, et par suite $g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$. Inversement, si $g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$, il existe un graphe fonctionnel $f \in I$ tel que, pour tout $\lambda \in L$, on ait $g(\lambda) \in X_{\lambda, f(\lambda)}$ et *a fortiori* $g(\lambda) \in \bigcup_{i \in J_\lambda} X_{\lambda, i}$, ce qui achève de démontrer la première formule. La seconde se démontre de façon analogue mais plus simple encore, comme nous laissons au lecteur le soin de le vérifier.

#### Corollaire 1 {#ens-ii-s5-prop-9-cor-1 .statement tag=03QE}

*Si, pour chaque indice* $\lambda \in L$, *la famille* $(X_{\lambda, i})_{i \in J_\lambda}$ *est une partition de* $X_\lambda = \bigcup_{i \in J_\lambda} X_{\lambda, i}$, *la famille* $(\prod_{\lambda \in L} X_{\lambda, f(\lambda)})_{f \in I}$ *est une partition de* $\prod_{\lambda \in L} X_\lambda$.

Si on pose $P_f = \prod_{\lambda \in L} X_{\lambda, f(\lambda)}$, il suffit, en vertu de la première des formules de la prop. 9, de démontrer que, si f et g sont des éléments distincts de I, $P_f \cap P_g = \varnothing$. Or, il existe alors un $\lambda \in L$ tel que $f(\lambda) \neq g(\lambda)$, d’où, en vertu de l’hypothèse, $X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \varnothing$. Il en résulte qu’il n’y a aucun graphe appartenant à $P_f \cap P_g$; en effet, pour un tel graphe G, on devrait avoir
$$
G(\lambda) \in X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \varnothing,
$$
ce qui est absurde.

#### Corollaire 2 {#ens-ii-s5-prop-9-cor-2 .statement tag=03QF}

*Soient* $(X_i)_{i \in I}$ *et* $(Y_k)_{k \in K}$ *deux familles d’ensembles*. *On a*
$$
(\bigcup_{i \in I} X_i) \times (\bigcup_{k \in K} Y_k) = \bigcup_{(i, k) \in I \times K} (X_i \times Y_k)
$$
*et (si I et K sont non vides)*
$$
(\bigcap_{i \in I} X_i) \times (\bigcap_{k \in K} Y_k) = \bigcap_{(i, k) \in I \times K} (X_i \times Y_k).
$$

Il suffit de raisonner comme dans la démonstration du corollaire de la prop. 8 (II, p. 36).

#### Proposition 10 {#ens-ii-s5-prop-10 .statement tag=03QG}

*Soit* $(X_{i, k})_{(i, k) \in I \times K}$ *une famille d’ensembles dont l’ensemble d’indices est le produit de deux ensembles* I *et* K. *Si* $K \neq \varnothing$, *on a*
$$
\bigcap_{k \in K} \left( \prod_{i \in I} X_{i, k} \right) = \prod_{i \in I} \left( \bigcap_{k \in K} X_{i, k} \right).
$$

Les deux membres de l’égalité qu’il s’agit de démontrer sont des ensembles de graphes fonctionnels. Pour qu’un tel graphe f appartienne au premier membre, il faut et il suffit que, pour tout $k \in K$, $f \in \prod_{i \in I} X_{i, k}$, c’est-à-dire que, pour tout (ι, κ) ∈ I × K, f(ι) appartienne à X_{ι,κ}. Pour que f appartienne au second membre, il faut et il suffit que, pour tout ι ∈ I, on ait f(ι) ∈ ∩_{κ ∈ K} X_{ι,κ}, c'est-à-dire encore que, pour tout (ι, κ) ∈ I × K, f(ι) appartienne à X_{ι,κ}. La proposition est donc démontrée.

#### Corollaire {#ens-ii-s5-n6-cor-2 .statement tag=03IR}

Soient (X_ι)_{ι ∈ I} et (Y_ι)_{ι ∈ I} deux familles d'ensembles ayant même ensemble d'indices I ≠ ∅. On a

$$(\prod_{ι ∈ I} X_ι) ∩ (\prod_{ι ∈ I} Y_ι) = \prod_{ι ∈ I} (X_ι ∩ Y_ι)$$

et

$$(\cap_{ι ∈ I} X_ι) × (\cap_{ι ∈ I} Y_ι) = \cap_{ι ∈ I} (X_ι × Y_ι).$$

Il suffit d'appliquer la prop. 10 au cas où K (resp. I) est un ensemble à deux éléments distincts.

### 7. Extension d'applications aux produits

#### Définition 2 {#ens-ii-s5-def-2 .statement tag=03IS}

Soient (X_ι^i)_{ι ∈ I}, (Y_ι)_{ι ∈ I} deux familles d'ensembles, et (g_ι)_{ι ∈ I} une famille de fonctions, admettant le même ensemble d'indices, et telles que, pour tout ι ∈ I, g_ι soit une application de X_ι dans Y_ι. Pour tout f ∈ \prod_{ι ∈ I} X_ι, soit u_f le graphe de la fonction ι ↦ g_ι(f(ι)) (ι ∈ I), qui est un élément de \prod_{ι ∈ I} Y_ι. On appelle extension canonique (ou simplement extension) de la famille d'applications (g_ι)_{ι ∈ I} aux produits, l'application f ↦ u_f de \prod_{ι ∈ I} X_ι dans \prod_{ι ∈ I} Y_ι; on dit aussi parfois que c'est le produit de la famille d'applications (g_ι)_{ι ∈ I}.

Quand on utilise la notation indicelle, le produit de la famille (g_ι)_{ι ∈ I} est donc la fonction (x_ι)_{ι ∈ I} ↦ (g_ι(x_ι))_{ι ∈ I}; on la désigne parfois encore par (g_ι)_{ι ∈ I}.

Si I = {α, β}, où α et β sont distincts, l'extension aux produits de la famille d'applications (g_ι)_{ι ∈ I} n'est autre que ψ o (g_α × g_β) o φ, où φ désigne l'application canonique de \prod_{ι ∈ I} X_ι sur X_α × X_β (II, p. 33) et ψ l'application canonique de Y_α × Y_β sur \prod_{ι ∈ I} Y_ι.

#### Proposition 11 {#ens-ii-s5-prop-11 .statement tag=03IT}

Soient (X_ι)_{ι ∈ I}, (Y_ι)_{ι ∈ I}, (Z_ι)_{ι ∈ I} trois familles d'ensembles, (g_ι)_{ι ∈ I}, (g'_ι)_{ι ∈ I} deux familles de fonctions, admettant le même ensemble d'indices, et telles que, pour tout ι ∈ I, g_ι soit une application de X_ι dans Y_ι, et g'_ι une application de Y_ι dans Z_ι. Soient g et g' les extensions des familles (g_ι)_{ι ∈ I} et (g'_ι)_{ι ∈ I} aux produits; alors l'extension aux produits de la famille (g'_ι o g_ι)_{ι ∈ I} est égale à g' o g.

La proposition découle immédiatement de la déf. 2.

#### Corollaire {#ens-ii-s5-n7-cor-1 .statement tag=03IU}

Soient (X_ι)_{ι ∈ I}, (Y_ι)_{ι ∈ I} deux familles d'ensembles, (g_ι)_{ι ∈ I} une famille de fonctions. Si, pour tout $i \in I$, $g_i$ est une injection (resp. surjection) de $X_i$ dans $Y_i$, alors l’extension $g$ de $(g_i)_{i \in I}$ aux ensembles produits est une injection (resp. une surjection) de $\prod_{i \in I} X_i$ dans $\prod_{i \in I} Y_i$.

$1^\circ$ Bornons-nous au cas où $X_i \neq \varnothing$ pour tout $i \in I$, le résultat étant trivial dans le cas contraire. Supposons que, pour tout $i \in I$, $g_i$ soit une injection, et soit $r_i$ une rétraction associée à $g_i$ (II, p. 18, déf. 11), de sorte que $r_i \circ g_i$ est l’application identique de $X_i$. Soit $r$ l’extension aux produits de la famille $(r_i)_{i \in I}$; comme $r \circ g$ est l’extension aux produits de la famille des applications identiques $\mathrm{Id}_{X_i}$, $r \circ g$ est l’application identique de $\prod_{i \in I} X_i$, donc $g$ est une injection (II, p. 18, prop. 8).

$2^\circ$ Supposons que, pour tout $i \in I$, $g_i$ soit une surjection de $X_i$ sur $Y_i$, et soit $s_i$ une section associée à $g_i$ (II, p. 18, déf. 11), de sorte que $g_i \circ s_i$ est l’application identique de $Y_i$. Si $s$ est l’extension aux produits de la famille $(s_i)_{i \in I}$, $g \circ s$ est l’extension aux produits de la famille des applications identiques $\mathrm{Id}_{Y_i}$, donc est l’application identique de $\prod_{i \in I} Y_i$, ce qui prouve que $g$ est une surjection (II, p. 18, prop. 8).

Soit $(X_i)_{i \in I}$ une famille d’ensembles, et soit $E$ un ensemble. Pour toute application $f$ de $E$ dans $\prod_{i \in I} X_i$, $\mathrm{pr}_i \circ f$ est une application de $E$ dans $X_i$; si $\bar{f}$ est l’extension aux produits de cette famille d’applications, et $d$ l’application diagonale (II, p. 33) de $E$ dans $E^I$, on voit aussitôt que l’on a $f = \bar{f} \circ d$. Inversement, soit $(f_i)_{i \in I}$ une famille de fonctions telle que, pour tout $i \in I$, $f_i$ soit une application de $E$ dans $X_i$, et soit $\bar{f}$ l’extension aux produits de cette famille; on a alors, pour tout $i \in I$, $\mathrm{pr}_i \circ (\bar{f} \circ d) = f_i$. Par abus de langage, l’application $\bar{f} \circ d$ se note encore $(f_i)_{i \in I}$. On définit ainsi une application bijective (dite canonique, ainsi que son application réciproque) de l’ensemble $\prod_{i \in I} X_i^E$ sur l’ensemble $(\prod_{i \in I} X_i)^E$.

## EXERCICES {#ens-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
