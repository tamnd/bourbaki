---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 3
section_title: Applications universelles
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E IV.31-E IV.32
pdf_pages: 0225-0231, 0234-0235
extraction: ocr
subsections:
    - "no": 1
      title: Ensembles et applications universels
      page: 22
      pdf_page: 225
    - "no": 2
      title: Existence d’applications universelles
      page: 23
      pdf_page: 226
    - "no": 3
      title: Exemples d’applications universelles
      page: 25
      pdf_page: 228
statements: 0
exercises: 3
content_sha256: a2897706a753f536281af7306b30f6322431c9ff55fd294d472b6fb300161861
---

## § 3. APPLICATIONS UNIVERSELLES

### 1. Ensembles et applications universels

Soit $\mathcal{T}$ une théorie plus forte que la théorie des ensembles, et soit $E$ un terme de $\mathcal{T}$. Soit $\Sigma$ une espèce de structure dans $\mathcal{T}$ (que nous supposons toujours, pour simplifier, définie sur un seul ensemble de base (principal)); pour abréger, nous dirons « $\Sigma$-ensemble » pour « ensemble muni d'une structure d'espèce $\Sigma$ ». Nous supposons en outre qu'on ait défini, pour l'espèce $\Sigma$, une notion de $\sigma$-morphisme (IV, p. 11) (comme au § 2, nous dirons « morphisme » au lieu de « $\sigma$-morphisme »). Enfin, l'espèce $\Sigma$ étant définie sur l'ensemble de base $x$, et ayant $s$ comme structure générique (IV, p. 4), supposons défini, dans $\mathcal{T}_\Sigma$, un terme $\alpha \{ x, s \}$ vérifiant les conditions suivantes:

(QM_I) La relation $\alpha \{ x, s \} \subset \mathcal{F}(E; x)$ est vraie dans $\mathcal{T}_\Sigma$.

(QM_{II}) Si, dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, $F, F'$ sont deux ensembles munis de structures $\mathcal{S}, \mathcal{S}'$ d'espèce $\Sigma$, et si $f$ est un morphisme de $F$ dans $F'$, alors la relation $\varphi \in \alpha \{ F, \mathcal{S} \}$ entraîne $f \circ \varphi \in \alpha \{ F', \mathcal{S}' \}$.

Nous exprimerons la relation $\varphi \in \alpha \{ x, s \}$ en disant que $\varphi$ est une $\alpha$-application de $E$ dans $x$ (muni de $s$).

Ceci posé, on dit qu'un $\Sigma$-ensemble $F_E$ et une $\alpha$-application $\varphi_E$ de $E$ dans $F_E$ sont universels si la condition suivante est remplie:

(AU) Pour toute $\alpha$-application $\varphi$ de $E$ dans un $\Sigma$-ensemble $F$, il existe un morphisme et un seul $f$ de $F_E$ dans $F$ tel que $\varphi = f \circ \varphi_E$.

On dit encore dans ce cas que le couple $(F_E, \varphi_E)$ est solution du problème d’application universelle pour $E$ (relativement à la donnée de $\Sigma$, $\sigma$ et $\alpha$).

Soient $(F'_E, \varphi'_E)$ et $(F''_E, \varphi''_E)$ deux solutions du problème d’application universelle pour $E$. La condition (AU) montre qu’il existe alors un morphisme unique $f_1$ de $F'_E$ dans $F''_E$ et un morphisme unique $f_2$ de $F''_E$ dans $F'_E$ tels que $\varphi''_E = f_1 \circ \varphi'_E$ et $\varphi'_E = f_2 \circ \varphi''_E$. On a donc

$$
\varphi'_E = f_2 \circ f_1 \circ \varphi'_E \quad \text{et} \quad \varphi''_E = f_1 \circ f_2 \circ \varphi''_E.
$$

Par application de (AU) au cas où $F = F'_E$ et $\varphi = \varphi'_E$, il en résulte que $f_2 \circ f_1$ est l’application identique de $F'_E$; de même $f_1 \circ f_2$ est l’application identique de $F''_E$. Par suite (IV, p. 12, critère CST8), $f_1$ est un isomorphisme de $F'_E$ sur $F''_E$, et $f_2$ en est l’isomorphisme réciproque. On exprime encore ce résultat en disant qu’une solution du problème d’application universelle pour $E$ est unique à un isomorphisme unique près.

Pour vérifier qu’un couple $(F_E, \varphi_E)$ est solution du problème d’application universelle pour $E$, il est souvent commode de vérifier les deux conditions suivantes:

(AU'_I) Pour tout $\Sigma$-ensemble $F$ et toute $\alpha$-application $\varphi$ de $E$ dans $F$, il existe un morphisme $f$ de $F_E$ dans $F$ tel que $\varphi = f \circ \varphi_E$.

(AU'_II) Pour tout $\Sigma$-ensemble $F$, deux morphismes de $F_E$ dans $F$ qui coïncident dans $\varphi_E(E)$ sont égaux.

En effet, si ces deux conditions sont réalisées, le morphisme $f$ dont l’existence est assurée par (AU'_I) est unique d’après (AU'_II). Réciproquement, il est clair que (AU) entraîne (AU'_I); de plus, si $f$ et $f'$ sont deux morphismes de $F_E$ dans $F$ qui coïncident dans $\varphi_E(E)$, on a $f \circ \varphi_E = f' \circ \varphi_E$, d’où $f = f'$ en appliquant (AU) à la $\alpha$-application $f \circ \varphi_E$.

### 2. Existence d’applications universelles

Un problème d’application universelle n’a pas nécessairement de solution (IV, p. 31, exerc. 1). Nous allons toutefois montrer que les conditions suivantes entraînent l’existence d’une solution:

(CU_I) Sur tout produit d’une famille de $\Sigma$-ensembles, il existe une structure produit d’espèce $\Sigma$ (IV, p. 16).

(CU_{II}) Soit $(F_i)_{i \in I}$ une famille de $\Sigma$-ensembles, et pour tout $i \in I$, soit $\varphi_i$ une $\alpha$-application de $E$ dans $F_i$. Alors l’application $(\varphi_i)_{i \in I}$ de $E$ dans $\prod_{i \in I} F_i$ (muni de la structure produit) est une $\alpha$-application.

Nous dirons qu’une partie $G$ d’un $\Sigma$-ensemble $F$ est $\Sigma$-permise si la structure de $F$ induit une structure d’espèce $\Sigma$ sur $G$ (IV, p. 16).

(CU_{III}) Il existe un cardinal $\alpha$ possédant les propriétés suivantes: pour tout $\Sigma$-ensemble

F et toute $\alpha$-application $\varphi$ de E dans F, il existe une partie $\Sigma$-permise G de F contenant $\varphi(E)$, de cardinal $\leq \alpha$, telle que l’application de E dans G qui a même graphe que $\varphi$ soit une $\alpha$-application, et que deux morphismes de G dans un $\Sigma$-ensemble, qui coïncident dans $\varphi(E)$, soient égaux.

CST22. Si les conditions (CU_I) à (CU_{III}) sont vérifiées, le problème d’application universelle pour E admet une solution.

Montrons d’abord que s’il existe un couple $(F_E, \varphi_E)$ vérifiant (AU'_I), il existe aussi une solution du problème d’application universelle pour E. En effet, il existe, d’après (CU_{III}), une partie $\Sigma$-permise $F'_E$ de $F_E$ contenant $\varphi_E(E)$, telle que l’application $\varphi'_E$ de E dans $F'_E$, qui a même graphe que $\varphi_E$, soit une $\alpha$-application, et que deux morphismes de $F'_E$ dans un $\Sigma$-ensemble, qui coïncident dans $\varphi_E(E)$, soient égaux. Soit $j$ l’injection canonique de $F'_E$ dans $F_E$, de sorte que $\varphi_E = j \circ \varphi'_E$; pour tout morphisme $f$ de $F_E$ dans un $\Sigma$-ensemble F, $f \circ j$ est un morphisme de $F'_E$ dans F, et l’on a $f \circ \varphi_E = (f \circ j) \circ \varphi'_E$. Il est clair alors que $(F'_E, \varphi'_E)$ vérifient (AU'_I) et (AU'_II).

Reste donc à prouver l’existence d’un couple $(F_E, \varphi_E)$ vérifiant (AU'_I). Soit $s \in S(x)$ la caractérisation typique de l’espèce de structure $\Sigma$, et considérons la partie L de l’ensemble produit
$$
\mathfrak{P}(a) \times S(a) \times \mathfrak{P}(E \times a)
$$
formée des triplets $\lambda = (X, V, P)$ ayant la propriété suivante:
« V est une structure d’espèce $\Sigma$ sur $X \subset a$, et P est le graphe d’une $\alpha$-application de E dans X (pour la structure V) »
(on notera que l’on a $S(X) \subset S(a)$, comme on le voit aisément en raisonnant de proche en proche sur la longueur du schéma de construction d’échelon S). Pour tout $\lambda = (X, V, P) \in L$, nous noterons $X_\lambda$ l’ensemble X muni de la structure V, et $\varphi_\lambda$ l’application de E dans $X_\lambda$, de graphe P.

Soit alors $F_E$ le $\Sigma$-ensemble produit des $X_\lambda$ (qui existe d’après (CU_I)), et soit $\varphi_E$ l’application $x \mapsto (\varphi_\lambda(x))$ de E dans $F_E$, qui est une $\alpha$-application en vertu de (CU_{II}). Montrons que $(F_E, \varphi_E)$ vérifie (AU'_I). En effet, étant donnée une $\alpha$-application $\varphi$ de E dans un $\Sigma$-ensemble F, soit G une partie de F vérifiant les conditions énoncées dans (CU_{III}); soient $j$ l’injection canonique de G dans F, et $\psi$ l’application de E dans G qui a même graphe de $\varphi$, de sorte que $\varphi = j \circ \psi$. Il résulte de (CU_{III}) que $\psi$ est une $\alpha$-application de E dans G. Comme Card(G) $\leq \alpha$, il y a une partie $G'$ de $a$ équipotente à G. Soit g une bijection de G sur $G'$; si on transporte par g la structure d’espèce $\Sigma$ de G, il existe par définition un $\lambda \in L$ tel que $G'$ (muni de cette structure transportée) soit égal à $X_\lambda$ et que $g \circ \psi = \varphi_\lambda$. Alors $f = j \circ g^{-1} \circ \mathrm{pr}_\lambda$ est un morphisme de $F_E$ dans F tel que $\varphi = f \circ \varphi_E$, ce qui achève la démonstration.

CST23. Soit $(F_E, \varphi_E)$ une solution du problème d’application universelle pour E. Pour que $\varphi_E$ soit une injection de E dans $F_E$, il faut et il suffit que, pour tout couple d’éléments distincts $x, y$ de $E$, il existe une $\alpha$-application $\varphi$ de $E$ dans un $\Sigma$-ensemble $F$, telle que $\varphi(x) \neq \varphi(y)$.

Comme $\varphi_E$ est une $\alpha$-application, le critère résulte aussitôt des définitions.

On dit encore dans ce cas que les $\alpha$-applications séparent les éléments de $E$. On ne fait alors d’ordinaire aucune distinction, dans le langage, entre les éléments de $E$ et leurs images par $\varphi_E$; avec cette convention, si $(F_E, \varphi_E)$ est une solution du problème d’application universelle, toute $\alpha$-application de $E$ dans un $\Sigma$-ensemble $F$ se prolonge en un morphisme de $F_E$ dans $F$ et un seul.

### 3. Exemples d’applications universelles

*Les exemples qui suivent seront, pour la plupart, traités en détail dans la suite de cet ouvrage.

I. Structures algébriques libres. — Soient $E$ un ensemble, $\Sigma$ une espèce de structure algébrique définie par une ou plusieurs lois de composition; nous prendrons comme morphismes les homomorphismes (pour toutes les lois envisagées), et les $\alpha$-applications seront les applications quelconques de $E$ dans un $\Sigma$-ensemble (autrement dit, $\alpha : x, s \mapsto \mathcal{F}(E; x)$). Toutes les espèces de structure algébrique usuelles vérifient (CU_{III}); à l’exception de la structure de corps, elles vérifient aussi (CU_I), et (CU_{II}) est ici une conséquence triviale de (CU_I).

Comme en général il existe des structures d’espèce $\Sigma$ définies sur des ensembles ayant au moins deux éléments, les $\alpha$-applications séparent les éléments de $E$, et on considère donc $E$ comme plongé dans $F_E$. On dit que $F_E$ est le $\Sigma$-ensemble libre engendré par $E$; c’est ainsi qu’on parle en Algèbre de monoïde libre (A, I, § 7, n° 2), de groupe libre (A, I, § 7, n° 5), de module libre (A, II, § 1, n° 11), d’algèbre libre (A, III, § 2, n° 7).

II. Anneaux et corps de fractions. — Soient $E$ un anneau commutatif, et $S$ une partie multiplicative de $E$, ne contenant pas 0. Nous prendrons pour $\Sigma$ l’espèce de structure d’anneau commutatif, et pour morphismes les homomorphismes (pour la structure d’anneau). Les $\alpha$-applications seront les homomorphismes $\varphi$ de $E$ dans un anneau commutatif $A$ tels que $\varphi(S)$ ne contienne que des éléments inversibles dans $A$. On vérifie immédiatement les conditions (QM_{II}), (CU_I) à (CU_{III}) (avec $\alpha = \mathrm{Card}(E)\mathrm{Card}(\mathbf{N})$); le problème d’application universelle a donc toujours une solution $(F_E, \varphi_E)$, mais en général $\varphi_E$ n’est pas injective. Le cas le plus fréquent est celui où $E$ est un anneau intègre; en ce cas, $\varphi_E$ est injective. Si en outre on prend alors $S = E - \{0\}$, $F_E$ est un corps commutatif, appelé corps des fractions de $E$ (A, I, § 9, n° 2); voir (AC, II, § 2).

III. Produit tensoriel de deux modules. — Soit $E$ le produit $A \times B$ de deux modules sur un anneau commutatif $C$. Prenons pour $\Sigma$ l’espèce de structure de C-module, pour morphismes les applications linéaires, pour $\alpha$-applications les applications bilinéaires de $A \times B$ dans un C-module. La condition (QM_{II}) est évidemment vérifiée, ainsi que les conditions $(\mathrm{CU}_I)$ à $(\mathrm{CU}_{III})$ (avec $\alpha = \mathrm{Card}(E)\mathrm{Card}(C)\mathrm{Card}(N)$). Le C-module universel $F_E$ correspondant au couple $(A, B)$ est appelé le *produit tensoriel* de $A$ par $B$ et noté $A \otimes B$; l’application universelle $\varphi_E$ est notée $(x, y) \mapsto x \otimes y$; elle est bilinéaire, mais n’est pas injective en général (cf. A, II, § 3, no 5).

IV. *Extension de l’anneau d’opérateurs d’un module.* — Soient $A$ un anneau commutatif, $B$ un sous-anneau de $A$, $E$ un $B$-module. L’espèce $\Sigma$ est l’espèce de structure de $A$-module, les morphismes sont les applications $A$-*linéaires*, et les $\alpha$-applications sont les applications $B$-*linéaires* de $E$ dans un $A$-module. On dit que le $A$-module universel $F_E$ correspondant au $B$-module $E$ est obtenu par *extension à* $A$ de l’anneau d’opérateurs $B$ de $E$ (A, II, § 5, no 1).

V. *Complétion d’un espace uniforme.* — Soit $E$ un espace uniforme; prenons pour $\Sigma$ l’espèce de structure d’espace uniforme séparé et complet, pour morphismes les applications uniformément continues, pour $\alpha$-applications les applications uniformément continues de $E$ dans un espace uniforme séparé et complet. Les parties $\Sigma$-permises d’un espace uniforme séparé et complet sont ici les parties *fermées* pour la topologie de l’espace, et les conditions $(\mathrm{QM}_{II})$ et $(\mathrm{CU}_I)$ à $(\mathrm{CU}_{III})$ sont vérifiées en prenant $\alpha = 2^{2^{\mathrm{Card}(E)}}$. L’espace uniforme séparé et complet $F_E$ n’est autre (à un isomorphisme près) que le *séparé complété* de l’espace uniforme $E$ (TG, II, § 3, no 7).

VI. *Compactification de Stone-Čech.* — Soit $E$ un espace complètement régulier; $\Sigma$ est l’espèce de structure d’espace compact, les morphismes étant les applications continues (d’un espace compact dans un espace compact), les $\alpha$-applications les applications continues de $E$ dans un espace compact. Les parties $\Sigma$-permises sont encore ici les ensembles *fermés*, et on vérifie aisément les conditions $(\mathrm{QM}_{II})$, $(\mathrm{CU}_I)$ à $(\mathrm{CU}_{III})$ (avec le même cardinal que dans l’*Exemple V*). L’espace compact $F_E$ est (à un isomorphisme près) le « compactifié de Stone-Čech » obtenu en complétant $E$ pour la structure uniforme la moins fine rendant uniformément continues les applications continues de $E$ dans $\{0, 1\}$ (TG, IX, § 1, no 6); l’application $\varphi_E$ est injective, car deux points distincts de $E$ peuvent être séparés par une application continue de $E$ dans $\{0, 1\}$.

VII. *Groupes topologiques libres.* — Soient $E$ un espace complètement régulier, $\Sigma$ l’espèce de structure de groupe topologique séparé, les morphismes étant les homomorphismes continus; enfin, prenons comme $\alpha$-applications les applications continues de $E$ dans un groupe topologique séparé. On vérifie aisément les conditions $(\mathrm{QM}_{II})$, $(\mathrm{CU}_I)$ à $(\mathrm{CU}_{III})$ avec $\alpha = \mathrm{Card}(E)\mathrm{Card}(N)$. Le groupe topologique séparé $F_E$ solution du problème d’application universelle pour $E$ est appelé le *groupe topologique libre engendré par l’espace* $E$; comme deux points distincts de $E$ peuvent être séparés par une application continue de $E$ dans le groupe topologique séparé $\mathbf{R}$, l’application $\varphi_E$ est injective; on peut montrer que $\varphi_E$ est un homéomorphisme de $E$ sur le sous-espace $\varphi_E(E)$ de $F_E$.\footnote{Voir P. Samuel, On universal mappings and free topological groups, *Bull. Amer. Math. Soc.*, t. LIV (1948), p. 591–598.} Au lieu de prendre pour $\Sigma$ l’espèce de structure de groupe topologique séparé, on pourrait aussi prendre des espèces de structures telles que celles de groupe commutatif topologique séparé, de groupe compact, d’anneau topologique séparé, d’espace vectoriel topologique séparé (sur un corps topologique considéré comme ensemble de base auxiliaire), etc.

VIII. Fonctions presque périodiques sur un groupe topologique. — Soit E un groupe topologique; prenons pour $\Sigma$ l’espèce de structure de groupe compact, les morphismes étant les homomorphismes continus, les $\alpha$-applications étant les homomorphismes continus de E dans un groupe compact. Les conditions (QM$_{\Pi}$), (CU$_{I}$) à (CU$_{III}$) sont vérifiées avec $\alpha = 2^{2^{\text{Card}(E)}}$. On dit que le groupe compact $F_E$, solution du problème d’application universelle pour E, est le groupe compact associé à E; l’application $\varphi_E$ n’est pas nécessairement injective. Toute fonction numérique continue dans E de la forme $g \circ \varphi_E$, où g est une fonction numérique continue dans $F_E$, est appelée fonction presque périodique dans E.

IX. Variété d’Albanese. — Soient E une variété algébrique, $\Sigma$ l’espèce de structure de variété abélienne sur le même corps de base que E (variété algébrique complète, munie d’une loi de groupe algébrique, nécessairement commutative); les morphismes sont les applications rationnelles d’une variété abélienne dans une autre (qui sont nécessairement composées d’un homomorphisme et d’une translation); les $\alpha$-applications sont les applications rationnelles de E dans une variété abélienne. La condition (CU$_{I}$) n’est pas vérifiée, mais le problème d’application universelle admet une solution $F_E$, dite variété d’Albanese de E; en général, l’application rationnelle $\varphi_E$ correspondante n’est pas injective.*

Exercises

## EXERCICES {#ens-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
