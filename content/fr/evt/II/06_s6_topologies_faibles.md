---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 6
section_title: Topologies faibles
lang: fr
source: evt-i-v-fr
book_pages: EVT II.43-EVT II.57, EVT II.87-EVT II.92
pdf_pages: 0078-0092, 0122-0127
extraction: ocr
subsections:
    - "no": 1
      title: Espaces vectoriels en dualité
      page: 43
      pdf_page: 78
    - "no": 2
      title: Topologies faibles
      page: 45
      pdf_page: 80
    - "no": 3
      title: Ensembles polaires et sous-espaces orthogonaux
      page: 47
      pdf_page: 82
    - "no": 4
      title: Transposée d’une application linéaire continue
      page: 49
      pdf_page: 84
    - "no": 5
      title: Sous-espaces et espaces quotients d’un espace faible
      page: 51
      pdf_page: 86
    - "no": 6
      title: Produits de topologies faibles
      page: 53
      pdf_page: 88
    - "no": 7
      title: Espaces faiblement complets
      page: 54
      pdf_page: 89
    - "no": 8
      title: Cônes convexes complets dans les espaces faibles
      page: 56
      pdf_page: 91
statements: 45
exercises: 20
content_sha256: ca3f31362016c357e6db7c8065b2dfc7576d34cf3036aeb2c612d049d36f885f
---

## § 6. TOPOLOGIES FAIBLES

### 1. Espaces vectoriels en dualité

Soient F et G deux espaces vectoriels réels, $(x, y) \mapsto B(x, y)$ une forme bilinéaire sur $F \times G$. On dit que la forme bilinéaire B met les espaces vectoriels F et G en dualité, ou que F et G sont en dualité (relativement à B). Rappelons que l’on dit que x ∈ F et y ∈ G sont orthogonaux (pour la dualité définie par B) si B(x, y) = 0 ; on dit qu’une partie M de F et une partie N de G sont orthogonales si tout x ∈ M est orthogonal à tout y ∈ N (A, IX, § 1, n° 2).

On dit que la dualité définie par B est séparante en F (resp. en G) si elle vérifie la condition suivante :

(D₁) Quel que soit x ≠ 0 dans F, il existe un y ∈ G tel que B(x, y) ≠ 0.
(resp.

(D₂) Quel que soit y ≠ 0 dans G, il existe un x ∈ F tel que B(x, y) ≠ 0.)

On dit que la dualité définie par B est séparante si elle est à la fois séparante en F et en G. Pour qu’il en soit ainsi, il faut et il suffit que la forme bilinéaire B soit séparante au sens de A, IX, § 1, n° 1. De manière plus précise, on a le résultat suivant :

#### Proposition 1 {#evt-ii-s6-prop-1 .statement}

Soient F, G deux espaces vectoriels réels, B une forme bilinéaire sur F × G. Soient

$$
d_B : y \mapsto B(., y),
s_B : x \mapsto B(x, .)
$$

les applications linéaires de G dans le dual F* de F, et de F dans le dual G* de G, associées respectivement à droite et à gauche à B (A, IX, § 1, n° 1). Pour que B mette F et G en dualité séparante en G (resp. en F), il faut et il suffit que d_B (resp. s_B) soit injective.

Lorsque F et G sont mis en dualité séparante par B, on identifiera souvent F (resp. G) à un sous-espace de G* (resp. F*) au moyen de s_B (resp. d_B). Lorsqu’on considérera F (resp. G) comme sous-espace de G* (resp. F*) sans spécifier de quelle manière est faite l’identification, il s’agira toujours des identifications précédentes ; la forme bilinéaire B est alors identifiée à la restriction à F × G de la forme bilinéaire canonique

$$(x^*, x) \mapsto \langle x, x^* \rangle \quad (\text{resp. } (x, x^*) \mapsto \langle x, x^* \rangle).$$

#### Exemple 1 {#evt-ii-s6-n1-exa-1 .statement}

Soient E un espace vectoriel, E* son dual. La forme bilinéaire canonique (x, x*) ↦ ⟨x, x*⟩ sur E × E* (A, II, p. 41) met E et E* en dualité séparante : en effet, (D₂) est vérifiée par définition de la relation x* ≠ 0, et on sait d’autre part que pour tout x ≠ 0 dans E, il existe une forme linéaire x* ∈ E* telle que ⟨x, x*⟩ ≠ 0 (A, II, p. 103, th. 6), ce qui prouve (D₁) ; l’identification de E à un sous-espace de E** se fait ici par l’application canonique c_E (loc. cit.).

Lorsque E est de dimension finie, le seul sous-espace G de E* qui soit en dualité séparante avec E pour la restriction à E × G de la forme bilinéaire canonique, est l’espace E* lui-même : en effet, E étant alors canoniquement identifié à E** (loc. cit.), si l’on avait G ≠ E*, il existerait a ≠ 0 dans E tel que ⟨a, x*⟩ = 0 pour tout x* ∈ G (A, II, p. 104, th. 7), contrairement à l’hypothèse.

#### Exemple 2 {#evt-ii-s6-n1-exa-2 .statement}

Lorsque E est un espace vectoriel de dimension infinie, E’ un sous-espace vectoriel de E*, la dualité entre E et E’ définie par la restriction à E × E’ de la forme bilinéaire canonique est toujours séparante en E' ; elle peut être séparante en E même si E' $\neq$ E*. L’exemple le plus important correspond au cas où E est un espace vectoriel topologique :

#### Définition 1 {#evt-ii-s6-def-1 .statement}

On appelle dual d’un espace vectoriel topologique E le sous-espace E' du dual E* de l’espace vectoriel E, constitué par les formes linéaires continues sur E.

Lorsque E est un espace localement convexe séparé, la dualité entre E et son dual E' est séparante ; il résulte en effet du th. de Hahn-Banach (II, p. 26, cor. 1) que pour tout $x \neq 0$ dans E, il existe $x' \in E'$ tel que $\langle x, x' \rangle \neq 0$.

#### Remarque 1 {#evt-ii-s6-n1-rem-1 .statement}

Lorsque E est un espace vectoriel topologique, le dual E* de l’espace vectoriel E sera parfois appelé le dual algébrique de E pour éviter des confusions. On notera d’ailleurs que E* est le dual de l’espace vectoriel topologique obtenu en munissant E de la topologie localement convexe la plus fine (II, p. 27, Exemple 2).

#### Remarque 2 {#evt-ii-s6-n1-rem-2 .statement}

Le dual E' d’un espace vectoriel topologique n’est pas lui-même muni d’une topologie, à moins que cela n’ait été expressément mentionné.

#### Remarque 3 {#evt-ii-s6-n1-rem-3 .statement}

Si F et G $\subset F^*$ sont en dualité séparante pour la forme bilinéaire canonique, il en est de même de F et $G_1$ pour tout sous-espace $G_1$ de $F^*$ tel que $G \subset G_1$.

### 2. Topologies faibles

#### Définition 2 {#evt-ii-s6-def-2 .statement}

Soient F, G deux espaces vectoriels mis en dualité par une forme bilinéaire B. On appelle topologie faible sur F définie par la dualité entre F et G, et l’on note $\sigma(F, G)$, la topologie la moins fine sur F rendant continues toutes les formes linéaires $B(., y) : x \mapsto B(x, y)$ lorsque y parcourt G.

On définit de la même manière la topologie faible $\sigma(G, F)$ sur G, en permutant dans la déf. 1 les rôles de F et de G ; cette possibilité d’échanger F et G s’applique à tous les résultats et définitions qui vont suivre dans ce paragraphe.

On emploiera parfois l’adjectif « faible » et l’adverbe « faiblement » pour désigner des propriétés relatives à une topologie faible $\sigma(F, G)$, lorsqu’il ne pourra en résulter de confusions. On parlera par exemple de « convergence faible », de « fonction faiblement continue », etc.

Lorsque G $\subset F^*$, il est entendu que la notation $\sigma(F, G)$ désignera toujours la topologie faible définie par la dualité correspondant à la restriction à $F \times G$ de la forme bilinéaire canonique $(x, x^*) \mapsto \langle x, x^* \rangle$.

Sans hypothèse supplémentaire sur F et G, on écrit souvent $\langle x, y \rangle$ la valeur $B(x, y)$ de la forme bilinéaire B en $(x, y)$ si aucune confusion n’en résulte ; nous adopterons cette écriture dans le reste de ce paragraphe.

Un espace vectoriel F muni d’une topologie faible $\sigma(F, G)$ sera appelé espace faible.

Une topologie faible $\sigma(F, G)$ est localement convexe (II, p. 29, prop. 4) ; de façon précise, c’est l’image réciproque de la topologie produit de $\mathbf{R}^G$ par l’application linéaire $\varphi : x \mapsto (\langle x, y \rangle)_{y \in G}$ de F dans $\mathbf{R}^G$. Elle est définie par l’ensemble des semi-normes $x \mapsto |\langle x, y \rangle|$ lorsque y parcourt G (II, p. 5). Pour tout $\alpha > 0$ et toute famille finie $(y_i)_{1 \leq i \leq n}$ de points de $G$, soit $W(y_1, ..., y_n; \alpha)$ l’ensemble des $x \in F$ tels que $|\langle x, y_i \rangle| \leq \alpha$ pour $1 \leq i \leq n$; ces ensembles (pour $\alpha, n$ et les $y_i$ arbitraires) forment un *système fondamental de voisinages de $0$* pour $\sigma(F, G)$. On notera que $W(y_1, ..., y_n; \alpha)$ contient le *sous-espace vectoriel* de $F$, de codimension *finie*, défini par les équations $\langle x, y_i \rangle = 0$ pour $1 \leq i \leq n$.

#### Proposition 2 {#evt-ii-s6-prop-2 .statement}

*Pour que la topologie faible $\sigma(F, G)$ soit séparée, il faut et il suffit que la dualité entre $F$ et $G$ soit séparante en $F$.*
C’est un cas particulier de II, p. 4, prop. 2.

#### Proposition 3 {#evt-ii-s6-prop-3 .statement}

*Soient $F, G$ deux espaces vectoriels réels en dualité. Toute forme linéaire sur $F$, continue pour $\sigma(F, G)$, peut s’écrire $x \mapsto \langle x, y \rangle$ pour un $y \in G$. L’élément $y \in G$ est unique lorsque la dualité est séparante en $G$.*
En effet, dire qu’une forme linéaire $f$ sur $F$ est continue pour $\sigma(F, G)$ signifie qu’il existe un nombre fini de points $y_i \in G$ ($1 \leq i \leq n$) tels que l’on ait, pour tout $x$ dans $F$, $|f(x)| \leq \sup_{1 \leq i \leq n} |\langle x, y_i \rangle|$ (II, p. 7, prop. 5). Les $n$ relations $\langle x, y_i \rangle = 0$ ($1 \leq i \leq n$) entraînent donc $f(x) = 0$, et par suite (A, II, p. 104, cor. 1), il existe une combinaison linéaire $y = \sum_{i=1}^n \lambda_i y_i$ telle que $f(x) = \langle x, y \rangle$ pour tout $x \in F$. L’unicité résulte de $(D_{II})$.

En d’autres termes, lorsque la dualité est séparante en $G$ et que $F$ est muni de la topologie $\sigma(F, G)$, on peut *identifier canoniquement* $G$ au *dual de $F$* pour cette topologie (II, p. 45, déf. 1).

#### Corollaire 1 {#evt-ii-s6-prop-3-cor-1 .statement}

*Pour qu’une famille $(a_i)$ de points de $F$ soit totale pour la topologie $\sigma(F, G)$, il faut et il suffit que, pour tout $y \neq 0$ dans $G$, il existe un indice $i$ tel que $\langle a_i, y \rangle \neq 0$.*
Cela exprime en effet, compte tenu de la prop. 3 et de I, p. 13, th. 1, qu’aucun hyperplan fermé pour $\sigma(F, G)$ ne contient tous les $a_i$; le corollaire résulte donc du cor. 3 de II, p. 41.

#### Corollaire 2 {#evt-ii-s6-prop-3-cor-2 .statement}

*Pour qu’une famille $(a_i)$ de points de $F$ soit topologiquement libre pour la topologie $\sigma(F, G)$, il faut et il suffit que, pour tout indice $i$, il existe un élément $b_i \in G$ tel que l’on ait :*
$$
\langle a_i, b_i \rangle \neq 0 \\
\langle a_\kappa, b_i \rangle = 0 \quad \text{pour tout } \kappa \neq i .
$$
Cela exprime en effet que, pour tout $i$, il existe un hyperplan fermé pour $\sigma(F, G)$, contenant les $a_\kappa$ d’indice $\kappa \neq i$ et ne contenant pas $a_i$.

#### Corollaire 3 {#evt-ii-s6-prop-3-cor-3 .statement}

*Soient $G_1, G_2$ deux sous-espaces vectoriels de $F^*$, en dualité avec $F$ (pour la restriction de la forme bilinéaire canonique). *Pour que $\sigma(F, G_2)$ soit plus fine que $\sigma(F, G_1)$, il faut et il suffit que $G_1 \subset G_2$.*

La condition est évidemment suffisante ; d’autre part, si $\sigma(F, G_2)$ est plus fine que $\sigma(F, G_1)$, toute forme linéaire continue pour $\sigma(F, G_1)$ est continue pour $\sigma(F, G_2)$, donc $G_1 \subset G_2$ en vertu de la prop. 3.

#### Corollaire 4 {#evt-ii-s6-prop-3-cor-4 .statement}

*Soient F un espace vectoriel, G un sous-espace vectoriel du dual F*. Pour que F et G soient en dualité séparante (pour la forme bilinéaire canonique), *il faut et il suffit que G soit dense dans F* pour la topologie $\sigma(F^*, F)$.

C’est une conséquence immédiate du cor. 1.

### 3. Ensembles polaires et sous-espaces orthogonaux

#### Définition 2 {#evt-ii-s6-def-2-bis .statement}

*Soient F et G deux espaces vectoriels (réels) en dualité. Pour toute partie M de F, on appelle polaire de M dans G l’ensemble des $y \in G$ tels que l’on ait $\langle x, y \rangle \geq -1$ pour tout $x \in M$. (Pour les espaces vectoriels complexes, *cf. II, p. 68.*)

Si $G_1, G_2$ sont deux sous-espaces de $F^*$ tels que $G_1 \subset G_2$, le polaire de M dans $G_1$ est l’intersection de $G_1$ et du polaire de M dans $G_2$.

Lorsque aucune confusion n’est à craindre, on désigne l’ensemble polaire dans G d’une partie M de F par la notation $M^\circ$. On définit bien entendu de la même manière l’ensemble polaire dans F d’une partie de G.

Il est clair que pour tout scalaire $\lambda \neq 0$ et tout $M \subset F$, on a $(\lambda M)^\circ = \lambda^{-1} M^\circ$. La relation $M \subset N \subset F$ entraîne $N^\circ \subset M^\circ$; si N absorbe M, $M^\circ$ absorbe $N^\circ$; pour toute famille $(M_\alpha)$ de parties de F, l’ensemble polaire de $\bigcup M_\alpha$ est l’intersection des ensembles polaires $M_\alpha^\circ$. Comme, pour $y \in M^\circ$, les demi-espaces fermés définis par les relations $\langle x, y \rangle \geq -1$ contiennent 0 et M, on voit que si $M_1$ est l’enveloppe convexe de $M \cup \{0\}$, on a $M_1^\circ = M^\circ$.

Il est clair que l’on a $M \subset M^{\circ \circ}$. On en conclut que

$$
(M^{\circ \circ})^\circ \subset M^\circ \subset (M^\circ)^{\circ \circ} = (M^{\circ \circ})^\circ
$$

autrement dit $M^{\circ \circ \circ} = M^\circ$ (*cf. E, III, p. 7, prop. 2*).

Si M est une partie symétrique de F, $M^\circ$ est une partie symétrique de G ; $M^\circ$ est aussi dans ce cas l’ensemble des $y \in G$ tels que $|\langle x, y \rangle| \leq 1$ pour tout $x \in M$.

#### Proposition 4 {#evt-ii-s6-prop-4 .statement}

(i) *Pour toute partie M de F, l’ensemble polaire $M^\circ$ contient 0 et c’est un ensemble convexe, fermé dans G pour la topologie $\sigma(G, F)$*.

(ii) *Si M est un cône de sommet 0, $M^\circ$ est un cône de sommet 0, et c’est aussi l’ensemble des $y \in G$ tels que $\langle x, y \rangle \geq 0$ pour tout $x \in M$*.

(iii) *Si M est un sous-espace vectoriel de F, $M^\circ$ est un sous-espace vectoriel de G, et c’est aussi l’ensemble des $y \in G$ tels que $\langle x, y \rangle = 0$ pour tout $x \in M$*.

(i) Comme les formes linéaires $y \mapsto \langle x, y \rangle$ sont continues pour $\sigma(G, F)$, l’assertion résulte aussitôt des définitions et du fait qu’un demi-espace déterminé par un hyperplan est convexe.

(ii) Si M est un cône de sommet 0, et si $x \in M, y \in M^\circ$, on a aussi $\lambda x \in M$ pour tout λ > 0, donc $\langle \lambda x, y \rangle \geq -1$ ou encore $\lambda \langle x, y \rangle \geq -1$ pour tout $\lambda > 0$, et par suite $\langle x, y \rangle \geq 0$, d’où (ii).

(iii) De même, si M est un sous-espace vectoriel de F, les relations $x \in M$, $y \in M^\circ$ entraînent cette fois $\lambda \langle x, y \rangle \geq -1$ pour tout $\lambda$ réel, ce qui n’est possible que si $\langle x, y \rangle = 0$.

Si M est un sous-espace vectoriel de F, on dit que $M^\circ$ est l’orthogonal de M dans G ; si $G \subset F^*$, $M^\circ$ est l’intersection de G et du sous-espace orthogonal à M dans le dual algébrique $F^*$ de F (A, II, p. 42, déf. 4).

Dire qu’un sous-espace vectoriel M de F et un sous-espace vectoriel N de G sont orthogonaux signifie donc que $M \subset N^\circ$ (ou, ce qui est équivalent, que $N \subset M^\circ$).

#### Théorème 1 (Théorème des bipolaires) {#evt-ii-s6-thm-1 .statement}

Soient F, G deux espaces vectoriels réels en dualité. Pour toute partie M de F, l’ensemble polaire $M^{\circ\circ}$ dans F de l’ensemble polaire $M^\circ$ de M dans G est l’enveloppe fermée convexe (pour $\sigma(F, G)$) de $M \cup \{0\}$.

On a vu que l’on peut se borner au cas où M est convexe et $0 \in M$. Soit $\overline{M}$ l’adhérence de M pour $\sigma(F, G)$, qui est donc un ensemble convexe dans F ; la prop. 4 de II, p. 47, montre que l’on a $M^{\circ\circ} \supset \overline{M}$. D’autre part, si $a \in F$ n’appartient pas à $\overline{M}$, il existe un hyperplan fermé H dans F qui sépare strictement a et $\overline{M}$ (II, p. 41, prop. 4) ; comme H ne contient pas 0, il existe un $y \in G$ tel que H ait pour équation $\langle x, y \rangle = -1$ (II, p. 46, prop. 3) ; on a par suite $\langle x, y \rangle > -1$ pour tout $x \in \overline{M}$ et $\langle a, y \rangle < -1$. Cela entraîne que l’on a $y \in M^\circ$ et $a \notin M^{\circ\circ}$, d’où la relation $M^{\circ\circ} = \overline{M}$.

#### Corollaire 1 {#evt-ii-s6-thm-1-cor-1 .statement}

Pour toute famille $(M_\alpha)$ de parties de F, convexes, fermées (pour $\sigma(F, G)$) et contenant 0, l’ensemble polaire de l’intersection $M = \bigcap_\alpha M_\alpha$ est l’enveloppe fermée convexe (pour $\sigma(G, F)$) de la réunion des $M_\alpha^\circ$.

En effet, si N est cette enveloppe fermée convexe, on a

$$
N^\circ = \bigcap_\alpha M_\alpha^{\circ\circ} = \bigcap_\alpha M_\alpha = M
$$

d’où $N = N^{\circ\circ} = M^\circ$.

La conclusion du cor. 1 ne s’étend pas lorsque les $M_\alpha$ ne sont pas nécessairement convexes.

#### Corollaire 2 {#evt-ii-s6-thm-1-cor-2 .statement}

Pour tout sous-espace vectoriel M de F, le sous-espace $M^{\circ\circ}$ est l’adhérence de M pour la topologie $\sigma(F, G)$.

#### Remarque {#evt-ii-s6-n3-rem-1 .statement}

Tout voisinage de 0 dans G pour $\sigma(G, F)$ contient un voisinage V défini par un nombre fini d’inégalités de la forme $|\langle x_i, y \rangle| \leq 1$ ($1 \leq i \leq n$), où les $x_i$ sont des points arbitraires de F. Si A est l’enveloppe convexe symétrique de l’ensemble des $x_i$, V est l’ensemble polaire $A^\circ$ de A dans G. On peut encore dire qu’un système fondamental de voisinages de 0 pour $\sigma(G, F)$ est formé des polaires dans G des ensembles finis symétriques (ou de leurs enveloppes convexes) de F. On notera que si la dualité est séparante en F, ces enveloppes convexes sont compactes pour $\sigma(F, G)$ (II, p. 15, cor. 1 de la prop. 15) et de dimension finie. Inversement, toute partie C *convexe, compacte et de dimension finie* dans F (muni de $\sigma(F, G)$) est alors contenue dans l’enveloppe convexe d’une partie *finie* de F. En effet, soit M un sous-espace vectoriel de dimension finie contenant C. Si $(e_i)_{1 \leq i \leq n}$ est une base de M, on peut supposer que C est contenue dans le parallélétope fermé de centre 0, construit sur les vecteurs de base $e_i$ (TG, VI, p. 3); or, il est immédiat que ce parallélétope est l’enveloppe convexe des points $\sum_{i=1}^n \varepsilon_i e_i$ avec $\varepsilon_i = \pm 1$.

On peut donc dire encore que (si $\sigma(F, G)$ est séparée) *les polaires des ensembles compacts, convexes et de dimension finie dans F* (pour $\sigma(F, G)$, ou pour toute topologie localement convexe séparée plus fine que $\sigma(F, G)$ sur F) forment un système fondamental de voisinages de 0 pour $\sigma(G, F)$.

#### Corollaire 3 {#evt-ii-s6-thm-1-cor-3 .statement}

*Soient E un espace localement convexe, $\mathcal{T}$ sa topologie, E' son dual* (II, p. 45, déf. 1).

(i) *Les ensembles convexes fermés dans E sont les mêmes pour la topologie $\mathcal{T}$ et la topologie faible $\sigma(E, E')$*.

(ii) *Pour toute partie M de E, l’ensemble polaire $M^{oo}$ dans E de l’ensemble polaire $M^o$ de M dans E', est l’enveloppe fermée convexe de $M \cup \{0\}$ pour la topologie $\mathcal{T}$*.

Il est clair que (ii) résulte de (i) et du th. 1. Par définition du dual E', il résulte de II, p. 46, prop. 3 que les formes linéaires continues sur E pour la topologie $\mathcal{T}$ sont les mêmes que les formes linéaires continues pour $\sigma(E, E')$. Les demi-espaces fermés dans E sont donc les mêmes pour $\mathcal{T}$ et pour $\sigma(E, E')$ (II, p. 16, prop. 17), et l’assertion (i) résulte donc de II, p. 41, cor. 1.

### 4. Transposée d’une application linéaire continue

Dans ce no, on suppose que (F, G) et $(F_1, G_1)$ sont deux couples d’espaces vectoriels en dualité.

#### Proposition 5 {#evt-ii-s6-prop-5 .statement}

*Soit u une application linéaire de F dans $F_1$. Les propriétés suivantes sont équivalentes :

a) u est continue pour les topologies faibles $\sigma(F, G)$ et $\sigma(F_1, G_1)$;
b) il existe une application $v : G_1 \to G$ telle que l’on ait :

(1)
$$
\langle u(y), z_1 \rangle = \langle y, v(z_1) \rangle
$$
quels que soient $y \in F$ et $z \in G_1$.

Si ces propriétés sont satisfaites et que la dualité entre F et G est séparante en G, alors il existe une seule application v satisfaisant à (1), et v est linéaire.

Si u est continue pour les topologies faibles, alors, pour tout $z_1 \in G_1$, la forme linéaire $y \mapsto \langle u(y), z_1 \rangle$ sur F est continue pour $\sigma(F, G)$, donc (II, p. 46, prop. 3) s’écrit $y \mapsto \langle y, v(z_1) \rangle$ avec $v(z_1) \in G$, ce qui prouve que a) entraîne b). Inversement, si b) est vérifiée, pour tout $z_1 \in G_1$, la forme linéaire
$$
y \mapsto \langle y, v(z_1) \rangle = \langle u(y), z_1 \rangle
$$

est continue pour $\sigma(F, G)$; il résulte de la définition des topologies faibles que $u$ est continue pour $\sigma(F, G)$ et $\sigma(F_1, G_1)$ (I, p. 10, cor. 1). L’unicité de $v$ résulte de $(D_{II})$ et cette unicité entraîne que $v$ est linéaire.

#### Remarque {#evt-ii-s6-n4-rem-1 .statement}

Supposons la dualité entre F et G séparante en G et la dualité entre $F_1$ et $G_1$ séparante en $G_1$. Si on identifie G et $G_1$ à des sous-espaces de $F^*$ et $F_1^*$ respectivement, les conditions a) et b) équivalent encore à $'u(G_1) \subset G$; $v$ est la restriction de la transposée $'u$ de $u$ (A, II, p. 42) à $G_1$.

Par abus de langage, on dira (lorsqu’il n’en résulte pas de confusion) que $v$ est la transposée de $u$ (relativement aux dualités entre F et G d’une part, $F_1$ et $G_1$ de l’autre), et on la notera encore $'u$.

#### Corollaire {#evt-ii-s6-n4-cor-1 .statement}

*Supposons la dualité entre F et G séparante en G. Si u est une application linéaire de F dans $F_1$, continue pour $\sigma(F, G)$ et $\sigma(F_1, G_1)$, sa transposée est une application linéaire de $G_1$ dans G, continue pour $\sigma(G_1, F_1)$ et $\sigma(G, F)$. On a $'('u) = u$ si de plus la dualité entre $F_1$ et $G_1$ est séparante en $F_1$.

Il suffit, dans la prop. 5, d’échanger les rôles joués par F et $F_1$ d’une part, G et $G_1$ de l’autre.

#### Proposition 6 {#evt-ii-s6-prop-6 .statement}

*On suppose que la dualité entre F et G (resp. $F_1$ et $G_1$) est séparante en G (resp. $F_1$). Soit u une application linéaire de F dans $F_1$, continue pour $\sigma(F, G)$ et $\sigma(F_1, G_1)$. Soient A une partie de F et $A_1$ une partie de $F_1$; alors :

(i) *On a $(u(A))^\circ = 'u^{-1}(A^\circ)$.

(ii) *On a $\overline{'u(A_1^\circ)} \subset (u^{-1}(A_1))^\circ$; en outre, si $A_1$ est convexe, fermée (pour $\sigma(F_1, G_1)$) et contient l’origine, on a $'u(A_1^\circ) = (u^{-1}(A_1))^\circ$.

Soit $z_1 \in G_1$. La relation $z_1 \in (u(A))^\circ$ équivaut à $\langle u(y), z_1 \rangle \geq -1$ pour tout $y \in A$, et la relation $'u(z_1) \in A^\circ$ à $\langle y, 'u(z_1) \rangle \geq -1$ pour tout $y \in A$, d’où l’assertion (i) en vertu de (1). Echangeant alors les rôles de $u$ et de $'u$ et appliquant (i) à la partie $A_1^\circ$ de $G_1$, il vient

$$(2)$$
$$( 'u(A_1^\circ))^\circ = u^{-1}(A_1^{\circ \circ}) \supset u^{-1}(A_1) $$

d’où en prenant les polaires

$$( 'u(A_1^\circ))^{\circ \circ} \subset (u^{-1}(A_1))^\circ .$$

On a $(\overline{'u(A_1^\circ)}) \subset ( 'u(A_1^\circ))^{\circ \circ}$ en vertu du th. des bipolaires (II, p. 48, th. 1); la dernière assertion résulte aussi de (2) et du th. des bipolaires puisque l’on a alors $A_1^{\circ \circ} = A_1$ et que $'u(A_1^\circ)$ est convexe et contient l’origine.

#### Corollaire 1 {#evt-ii-s6-prop-6-cor-1 .statement}

*Avec les notations de la prop. 6, la relation $u(A) \subset A_1$ entraîne $'u(A_1^\circ) \subset A^\circ$; si en outre $A_1$ est convexe, fermée (pour $\sigma(F_1, G_1)$) et contient l’origine, ces deux relations sont équivalentes.

En effet, la relation $u(A) \subset A_1$ équivaut à $A \subset u^{-1}(A_1)$, donc entraîne

$$ 'u(A_1^\circ) \subset \overline{'u(A_1^\circ)} \subset (u^{-1}(A_1))^\circ \subset A^\circ $$

et réciproquement la relation $^t u(A_1^\circ) \subset A^\circ$ entraîne

$$
A^{\circ \circ} \subset (^t u(A_1^0))^\circ = u^{-1}(A_1^{\circ \circ})
$$

d’après (2). Lorsque $A_1 = A_1^{\circ \circ}$, on en déduit $A \subset u^{-1}(A_1)$.

#### Corollaire 2 {#evt-ii-s6-prop-6-cor-2 .statement}

*Soit u une application linéaire de F dans F_1, continue pour σ(F, G) et σ(F_1, G_1). On a alors :*

(3)
$$
\mathrm{Ker}(^t u) = (\mathrm{Im}(u))^\circ ,
$$
(4)
$$
\overline{\mathrm{Im}(^t u)} = (\mathrm{Ker}(u))^\circ .
$$

*Supposons les dualités entre F et G et entre F_1 et G_1 séparantes ; pour que u(F) soit dense dans F_1 (pour σ(F_1, G_1)), il faut et il suffit que ^t u soit injective.*

On applique la prop. 6 avec $A = F$ et $A_1 = \{0\}$, compte tenu de ce que les topologies faibles $\sigma(G, F)$ et $\sigma(F_1, G_1)$ sont séparées. La dernière assertion résulte de (4), où l’on échange $u$ et $^t u$.

### 5. Sous-espaces et espaces quotients d’un espace faible

Soient F, G deux espaces vectoriels réels en dualité. Soit M un sous-espace vectoriel de F, et considérons un sous-espace N de l’orthogonal $M^\circ$ dans G ; si $y_1, y_2$ sont deux points de G congrus mod. N, on a $\langle x, y_1 \rangle = \langle x, y_2 \rangle$ pour tout $x \in M$. Pour toute classe $\dot{y}$ mod. N, désignons par $\langle x, \dot{y} \rangle$ la valeur commune des éléments $\langle x, y \rangle$ lorsque $y$ parcourt $\dot{y}$; il est clair que $(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$ est une forme bilinéaire sur $M \times (G/N)$.

#### Proposition 7 {#evt-ii-s6-prop-7 .statement}

*Soient F, G deux espaces vectoriels en dualité, M un sous-espace vectoriel de F, N un sous-espace vectoriel de G, tels que M et N soient orthogonaux (ce qui équivaut à dire que $N \subset M^\circ$, ou $M \subset N^\circ$). Les espaces vectoriels M et G/N sont alors en dualité par la forme bilinéaire $(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$.*

(i) *La topologie $\sigma(M, G/N)$ pour cette dualité est induite par $\sigma(F, G)$ (et en particulier on a $\sigma(F, G) = \sigma(F, G/F^\circ)$).*

(ii) *La topologie $\sigma(G/N, M)$ pour cette dualité est moins fine que la topologie quotient par N de $\sigma(G, F)$; pour qu’elle lui soit égale, il faut et il suffit que l’on ait $M + G^\circ = N^\circ$.*

(i) Tout élément de G/N est la classe mod. N d’un élément de G ; si $z_i$ ($1 \leq i \leq n$) sont des éléments de G, $\dot{z}_i$ ($1 \leq i \leq n$) la classe de $z_i$ dans G/N, l’ensemble des $y \in M$ tels que $|\langle y, \dot{z}_i \rangle| \leq \alpha$ pour $1 \leq i \leq n$ est la trace sur M de l’ensemble des $x \in F$ tels que $|\langle x, z_i \rangle| \leq \alpha$ pour $1 \leq i \leq n$; la conclusion résulte donc de la définition des voisinages de 0 pour la topologie faible.

(ii) Soit $p : G \to G/N$ la surjection canonique. Montrons que *la topologie quotient $\mathcal{T}$ de $\sigma(G, F)$ par N est identique à $\sigma(G/N, N^\circ)$*. Comme, pour $z \in G, y \in N^\circ$, on a $\langle y, p(z) \rangle = \langle y, z \rangle$, tout voisinage de 0 pour $\sigma(G/N, N^\circ)$ est de la forme p(V), où V est un voisinage de 0 pour $\sigma(G, F)$ saturé pour la relation $z - z' \in N$, donc $\mathcal{T}$ est plus fine que $\sigma(G/N, N^\circ)$. Inversement, soit $U = W(y_1, ..., y_n; \alpha)$ un voisinage de 0 dans G pour $\sigma(G, F)$, où $y_i \in F$ pour $1 \leq i \leq n$ et $\alpha > 0$; nous allons voir que pour $1 \leq i \leq n$, il existe des éléments $t_i \in N^\circ$ tels que si l’on pose $U' = W(t_1, ..., t_n; \alpha)$, on ait $p(U') \subset p(U)$; cela prouvera que $\sigma(G/N, N^\circ)$ est plus fine que $\mathcal{T}$, donc lui est identique. Or, soit L le sous-espace vectoriel de F engendré par $N^\circ$ et les $y_i$, et désignons par P un sous-espace supplémentaire de $N^\circ$ dans L, qui est de dimension finie m. Soit $(x_j)_{1 \leq j \leq m}$ une base de P ; les restrictions à N des formes linéaires $z \mapsto \langle x_j, z \rangle$ sont linéairement indépendantes, sans quoi il existerait $x \neq 0$ dans P tel que $\langle x, z \rangle = 0$ pour tout $z \in N$, c’est-à-dire $x \in N^\circ$, ce qui contredit la définition de P. On en conclut que pour tout $z' \in G$, il existe $s \in N$ tel que $\langle x_j, z' \rangle = \langle x_j, s \rangle$ pour tout $j$; si $z' = z + s$, on a par suite $\langle x, z \rangle = 0$ pour tout $x \in P$. Cela étant, posons $y_i = t_i + w_i$, où $t_i \in N^\circ$ et $w_i \in P$; on a $\langle y_i, z \rangle = \langle t_i, z \rangle = \langle t_i, z' \rangle$ pour $1 \leq i \leq n$; donc, pour tout $z' \in U'$, il existe $z \in U$ tel que $z' - z \in N$, c’est-à-dire que l’on a bien $p(U') \subset p(U)$.

Revenant au cas où M est un sous-espace quelconque de $N^\circ$, notons que l’on a évidemment $\sigma(G/N, M) = \sigma(G/N, M + G^\circ)$; en outre, il résulte de la prop. 3 de II, p. 46, que si $y \in N^\circ$ est tel que la forme linéaire $\dot{z} \mapsto \langle y, \dot{z} \rangle$ soit continue pour $\sigma(G/N, M)$, on a nécessairement $y \in M + G^\circ$. On en conclut que la condition $M + G^\circ = N^\circ$ est nécessaire et suffisante pour que la topologie quotient $\mathcal{T}$ soit égale à $\sigma(G/N, M)$.

#### Remarque {#evt-ii-s6-n5-rem-3 .statement}

Pour que la dualité entre M et G/N (où M et N sont deux sous-espaces orthogonaux) soit séparante en M, il faut et il suffit que $M \cap G^\circ = \{0\}$; pour qu’elle soit séparante en G/N, il faut et il suffit que $N = M^\circ$.

#### Corollaire 1 {#evt-ii-s6-prop-7-cor-1 .statement}

Supposons que la dualité entre F et G soit séparante en F. Pour qu’un sous-espace vectoriel M de F soit tel que $\sigma(G/M^\circ, M)$ soit identique à la topologie quotient par $M^\circ$ de la topologie $\sigma(G, F)$, il faut et il suffit que M soit fermé pour la topologie $\sigma(F, G)$.

Cela résulte de la prop. 7 où l’on fait $N = M^\circ$, en se rappelant que $M^{\circ\circ}$ est l’adhérence de M pour $\sigma(F, G)$ (II, p. 48, cor. 2).

#### Corollaire 2 {#evt-ii-s6-prop-7-cor-2 .statement}

Si M est de dimension finie n et la dualité séparante en F, $M^\circ$ est de codimension n dans G. Si M est fermé pour $\sigma(F, G)$ et de codimension finie n dans F et la dualité séparante en G, alors $M^\circ$ est de dimension n.

En effet, $G/M^\circ$ est en dualité séparante avec M ; si M est de dimension n, il en est donc de même de $G/M^\circ$ (II, p. 44, Exemple 1). Si M est fermé, $F/M = F/M^{\circ\circ}$ est en dualité séparante avec $M^\circ$; si $F/M$ est de dimension n, il en est donc de même de $M^\circ$ (II, p. 44, Exemple 1).

#### Corollaire 3 {#evt-ii-s6-prop-7-cor-3 .statement}

Soient (F, G), $(F_1, G_1)$ deux couples d’espaces en dualité séparante, u une application linéaire de F dans $F_1$, continue pour $\sigma(F, G)$ et $\sigma(F_1, G_1)$. Pour que u soit un morphisme strict de F dans $F_1$, il faut et il suffit que $\operatorname{Im}(^t u)$ soit un sous-espace fermé dans G pour $\sigma(G, F)$.

Soit $N = \operatorname{Im}(t^u) \subset G$; on sait que $N^\circ = \operatorname{Ker}(u)$ dans $F$ (II, p. 51, formule (3)). Soit $p : F \to F/N^\circ$ l’application canonique, de sorte que $u$ se factorise en

$$
u : F \xrightarrow{p} F/N^\circ \xrightarrow{w} F_1,
$$

où $w$ est injective. Les espaces $F/N^\circ$ et $N$ sont en dualité séparante et en vertu de la formule (1) de II, p. 49, on a $\langle w(j), z_1 \rangle = \langle j, t^u(z_1) \rangle$ quels que soient $j \in F/N^\circ$ et $z_1 \in G_1$. Cette relation montre que $w$ est un *isomorphisme* de $F/N^\circ$, muni de la topologie $\sigma(F/N^\circ, N)$, sur $u(F)$, muni de la topologie induite par $\sigma(F_1, G_1)$. La conclusion résulte donc du cor. 1 et de la définition d’un morphisme strict.

#### Corollaire 4 {#evt-ii-s6-prop-7-cor-4 .statement}

*Soient* $(F, G), (F_1, G_1)$ *deux couples d’espaces en dualité séparante, u une application linéaire de F dans F_1, continue pour σ(F, G) et σ(F_1, G_1)*. *Pour que u soit surjective, il faut et il suffit que t^u soit un isomorphisme de G_1 (muni de σ(G_1, F_1)) sur t^u(G_1) muni de la topologie induite par σ(G, F)*.

En effet, dire que $u(F) = F_1$ équivaut à dire que $u(F)$ est fermé et partout dense dans $F_1$ pour $\sigma(F_1, G_1)$; le cor. 4 résulte alors du cor. 3 appliqué à $t^u$, et de II, p. 51, cor. 2.

#### Remarque 1 {#evt-ii-s6-n5-rem-1 .statement}

Soient $(F_1, G_1), (F_2, G_2), (F_3, G_3)$ trois couples d’espaces en dualité séparante et considérons une suite de deux applications linéaires

(5)

$$
F_1 \xrightarrow{u} F_2 \xrightarrow{v} F_3
$$

*continues* pour les topologies faibles correspondant respectivement à $G_1, G_2, G_3$; considérons la suite des transposées

(6)

$$
G_3 \xrightarrow{t^v} G_2 \xrightarrow{t^u} G_1.
$$

Il est clair que $t(v \circ u) = t^u \circ t^v$, donc la relation $v \circ u = 0$ équivaut à $t^u \circ t^v = 0$. Pour que la suite (5) soit *exacte*, il faut et il suffit que les trois conditions suivantes soient satisfaites :
a) $t^u \circ t^v = 0$;
b) $\operatorname{Im}(t^v)$ est *dense* dans $\operatorname{Ker}(t^u)$;
c) $t^u$ est un *morphisme strict* de $G_2$ dans $G_1$.
Cela résulte en effet du cor. 3 de II, p. 52 et des formules (3) et (4) de II, p. 51.

#### Remarque 2 {#evt-ii-s6-n5-rem-2 .statement}

On se gardera de croire que lorsque $u$ est un morphisme strict de $F$ dans $F_1$, $t^u$ soit nécessairement un morphisme strict de $G_1$ dans $G$; autrement dit, $u$ peut être un morphisme strict de $F$ dans $F_1$ sans que $u(F)$ soit fermé dans $F_1$ pour $\sigma(F_1, G_1)$, comme le montre l’exemple où $F$ est un sous-espace non fermé de $F_1$ et $G = G_1/F^\circ$, $u$ étant l’injection canonique. De même, le fait que la suite (5) soit exacte n’entraîne pas nécessairement que la suite (6) le soit ; toutefois, si la suite (5) est exacte et si $v$ est un *morphisme strict*, alors la suite (6) est exacte, en vertu de la remarque 1 et de II, p. 52, cor. 3.

### 6. Produits de topologies faibles

#### Proposition 8 {#evt-ii-s6-prop-8 .statement}

*Soit* $(F_i, G_i)_{i \in I}$ *une famille de couples d’espaces vectoriels en dualité*. *Soient* $F = \prod_{i \in I} F_i$ *l’espace produit des* $F_i$, $G = \bigoplus_{i \in I} G_i$ *l’espace somme directe des* $G_i$.
*Si, pour tout* $x = (x_i) \in F$ *et tout* $y = (y_i) \in G$, *on pose* $\langle x, y \rangle = \sum_{i \in I} \langle x_i, y_i \rangle$ *(somme qui n’a qu’un nombre fini de termes $\neq 0$) la topologie $\sigma(F, G)$ (relative à la forme bilinéaire $(x, y) \mapsto \langle x, y \rangle$) est le produit des topologies $\sigma(F_i, G_i)$.

En effet, soit donnée une topologie $\mathcal{T}$ sur $F$; afin que, pour tout $y \in G$, la forme linéaire $x \mapsto \langle x, y \rangle$ soit continue pour $\mathcal{T}$, il faut et il suffit, par définition de $\langle x, y \rangle$, que chacune des applications $x \mapsto \langle \mathrm{pr}_i x, y_i \rangle$ soit continue pour $\mathcal{T}$, $i$ étant arbitraire dans $I$ et $y_i$ dans $G_i$; mais cela signifie que chacune des applications $\mathrm{pr}_i$ de $F$ dans $F_i$ est continue pour $\mathcal{T}$ et pour $\sigma(F_i, G_i)$ (I, p. 10, cor. 1); cela achève la démonstration.

#### Remarque {#evt-ii-s6-n6-rem-1 .statement}

Pour que la dualité entre $F$ et $G$ soit séparante en $F$ (resp. en $G$), il faut et il suffit que, pour tout $i \in I$, la dualité entre $F_i$ et $G_i$ soit séparante en $F_i$ (resp. $G_i$). Si la dualité entre $F$ et $G$ est séparante en $F$ (resp. $G$), alors, dans $F$ (resp. $G$), le sous-espace orthogonal à un $G_i$ (resp. $F_j$), identifié canoniquement à un sous-espace de $G$ (resp. $F$), est le sous-espace produit des $F_\kappa$ tels que $\kappa \neq i$ (resp. somme directe des $G_\kappa$ tels que $\kappa \neq i$).

#### Corollaire 1 {#evt-ii-s6-prop-8-cor-1 .statement}

Soient $F$ et $G$ deux espaces vectoriels en dualité séparante. Si l’espace $F$ (muni de $\sigma(F, G)$) est somme directe topologique de deux sous-espaces $M$, $N$, l’espace $G$ (muni de $\sigma(G, F)$) est somme directe topologique des sous-espaces $M^\circ$, $N^\circ$ respectivement orthogonaux à $M$ et $N$.

En effet, soient $p : F \to M$, $q : F \to N$ les projecteurs correspondant à la décomposition de $F$ en somme directe de $M$ et $N$; dans ces conditions, l’application $(p, q) : F \to M \times N$ est un isomorphisme topologique. Si $M_1 = G/M^\circ$, $N_1 = G/N^\circ$, les topologies sur $M$ et $N$ (induites par celle de $F$) sont identiques à $\sigma(M, M_1)$, $\sigma(N, N_1)$ respectivement (II, p. 51, prop. 7). L’application $' (p, q) : M_1 \times N_1 \to G$ est un isomorphisme topologique lorsqu’on munit $M_1$, $N_1$ et $G$ de $\sigma(M_1, M)$, $\sigma(N_1, N)$ et $\sigma(G, F)$, en vertu de la prop. 8. Par cette application, $M_1$ (resp. $N_1$) a pour image dans $G$ le sous-espace $N^\circ$ (resp. $M^\circ$), et la topologie $\sigma(M_1, M)$ (resp. $\sigma(N_1, N)$) a pour image la topologie induite sur $N^\circ$ (resp. $M^\circ$) par $\sigma(G, F)$, d’où le corollaire.

#### Corollaire 2 {#evt-ii-s6-prop-8-cor-2 .statement}

Soient $F$ un espace vectoriel, $F^*$ son dual, $(e_i)_{i \in I}$ une base de $F$, $u : \mathbf{R}^{(1)} \to F$ l’isomorphisme (algébrique) défini par cette base. Alors l’application transposée $'u : F^* \to \mathbf{R}^I$ est un isomorphisme topologique lorsqu’on munit $F^*$ de $\sigma(F^*, F)$ et $\mathbf{R}^I$ de la topologie produit.

On sait (A, II, p. 44, prop. 10) que $'u$ est une bijection, et que si, pour un $x^* \in F^*$, on pose $\langle e_i, x^* \rangle = \xi_i^*$ pour tout $i \in I$, l’image $'u(x^*)$ est le vecteur $(\xi_i^*)$ de $\mathbf{R}^I$, de sorte que, pour tout $x = \sum_i \xi_i e_i$ dans $F$, on a $\langle x, x^* \rangle = \sum_{i \in I} \xi_i \xi_i^*$. Le corollaire est alors conséquence de cette formule et de la prop. 8.

### 7. Espaces faiblement complets

#### Proposition 9 {#evt-ii-s6-prop-9 .statement}

Soient $F, G$ deux espaces vectoriels en dualité séparante. Si $\hat{F}$ est le complété de l’espace $F$ pour la topologie $\sigma(F, G)$, et si l’on considère l’injection canonique $j : F \to G^*$, où $G^*$ est muni de $\sigma(G^*, G)$, le prolongement continu $\hat{j} : \hat{F} \to G^*$ de $j$ est un isomorphisme d’espaces vectoriels topologiques.

En effet, on vient de voir que $G^*$, muni de $\sigma(G^*, G)$, est séparé et complet (II, p. 54, cor. 2); si l’on identifie $F$ par $j$ à un sous-espace vectoriel de $G^*$, la topologie induite sur $F$ par $\sigma(G^*, G)$ est $\sigma(F, G)$, et $F$ est dense dans $G^*$ pour $\sigma(G^*, G)$ (II, p. 47, cor. 4); d’où la proposition.

Les espaces vectoriels qui sont complets pour une topologie faible sont donc les duals $G^*$ d’espaces vectoriels $G$ quelconques, munis de $\sigma(G^*, G)$; d’après II, p. 54, cor. 2, ils sont isomorphes (topologiquement) aux produits $\mathbf{R}^l$ de droites réelles. Par abus de langage, nous les appellerons produits de droites (pour une caractérisation intrinsèque de ces espaces, voir II, p. 90, exerc. 13 et II, p. 87, exerc. 1).

On notera que sur $G^*$, la topologie $\sigma(G^*, G)$ est minimale parmi les topologies faibles séparées; en effet, une topologie faible moins fine que $\sigma(G^*, G)$ est nécessairement de la forme $\sigma(G^*, H)$ où $H \subset G$ (II, p. 46, cor. 3); mais si $H \neq G$, il existe une forme linéaire $x^* \in G^*$ non nulle et orthogonale à $H$ (A, II, p. 100, prop. 8), donc $\sigma(G^*, H)$ n’est pas séparée.

On conclut de cette remarque que si $F, G$ sont deux espaces vectoriels, une bijection linéaire $u : G^* \to F^*$, continue pour les topologies $\sigma(G^*, G)$ et $\sigma(F^*, F)$, est nécessairement bicontinue.

#### Proposition 10 {#evt-ii-s6-prop-10 .statement}

Soient $G$ un espace vectoriel réel, $F = G^*$ son dual muni de la topologie $\sigma(G^*, G)$.

(i) L’application $V \mapsto V^\circ$ est une bijection de l’ensemble des sous-espaces vectoriels de $G$ sur l’ensemble des sous-espaces vectoriels fermés de $F$.

(ii) Tout sous-espace vectoriel fermé de $F$ est un produit de droites et admet un supplémentaire topologique.

En vertu du th. des bipolaires (II, p. 48, cor. 2), $V \mapsto V^\circ$ est une bijection de l’ensemble des sous-espaces vectoriels $V$ de $G$, fermés pour $\sigma(G, G^*)$, sur l’ensemble des sous-espaces vectoriels fermés de $F$. Mais par définition, toute forme linéaire sur $G$ est continue pour $\sigma(G, G^*)$, donc tout sous-espace vectoriel dans $G$ est fermé, étant défini par un système d’équations $\langle y, y_\lambda^* \rangle = 0$ (où $y_\lambda^* \in G^*$); ceci prouve (i).

Soit maintenant $W$ un sous-espace fermé de $F$; on a donc $W = V^\circ$ avec $V = W^\circ$ dans $G$. Soit $V'$ un supplémentaire de $V$ dans $G$. On sait que $F = G^*$ s’identifie canoniquement à $V^* \oplus {V'}^*$, ${V'}^*$ s’identifiant à $V^\circ = W$ (A, II, p. 45, corollaire); en outre (II, p. 53, prop. 8) la topologie $\sigma(G^*, G)$ s’identifie au profit des topologies $\sigma(V^*, V)$ et $\sigma({V'}^*, V')$; cela prouve l’assertion (ii).

Bien que, pour la topologie $\sigma(G, G^*)$, tout sous-espace vectoriel de $G$ soit fermé, on notera que si $G$ est de dimension infinie, la topologie $\sigma(G, G^*)$ n’est pas la topologie localement convexe la plus fine sur $G$, tout voisinage de 0 pour $\sigma(G, G^*)$ contenant un sous-espace vectoriel de dimension infinie; c’est toutefois la plus fine des topologies faibles sur $G$ (II, p. 46, cor. 3).

### 8. Cônes convexes complets dans les espaces faibles

#### Lemme 1 {#evt-ii-s6-lem-1 .statement}

Soient E un espace faible séparé, C un cône convexe saillant de sommet 0 dans E, complet pour la structure uniforme induite par celle de E. Toute forme linéaire continue dans E est alors différence de deux formes linéaires continues dans E et positives dans C.

Soient E' le dual de E, F le dual algébrique de E', muni de la topologie σ(F, E'). Soit H = C° − C° le sous-espace vectoriel de E' constitué par les différences de formes linéaires continues dans E et positives dans C (II, p. 47, prop. 4). Il suffit de montrer que l’orthogonal de H dans F est réduit à 0 (II, p. 44, Exemple 1). Soit donc a ∈ F orthogonal à H ; alors a est orthogonal à C°, donc appartient au bipolaire de C dans F. Mais E s’identifie à un sous-espace de F, et comme C est complet, donc fermé dans F, on a a ∈ C (II, p. 48, th. 1). De même, a est orthogonal à − C°, donc a ∈ − C. Comme C est saillant, on a bien a = 0.

#### Proposition 11 {#evt-ii-s6-prop-11 .statement}

Soient E un espace faible séparé, C un cône convexe saillant de sommet 0 dans E, complet pour la structure uniforme induite par celle de E. Il existe un ensemble I et une application linéaire continue u de E dans l’espace produit R^I possédant les propriétés suivantes :
a) u est un isomorphisme de C sur u(C) pour les structures uniformes induites respectivement par celles de E et de R^I ;
b) on a u(C) ⊂ R^I_+.

En outre, si la structure uniforme induite sur C par celle de E est métrisable, on peut prendre I = N.

Soit (f_i)_{i∈I} une famille de formes linéaires continues dans E telle que les sommes finies d’écart de la forme (x, y) ↦ |f_i(x − y)| sur C × C définissent la structure uniforme de C. (Si la structure uniforme de C est métrisable, on peut prendre I = N.) En vertu du lemme 1, on peut supposer en outre que chacune des f_i est positive dans C. Soit u l’application linéaire x ↦ (f_i(x))_{i∈I} de E dans R^I. Il est clair que u est continue et que u(C) ⊂ R^I_+. La restriction u|C est une application uniformément continue et surjective de C sur u(C). De plus, si x, y dans C sont tels que f_i(x) = f_i(y) pour tout i ∈ I, on a x = y puisque la structure uniforme de C est séparée ; donc u|C est bijective. Enfin, si W est un entourage de la structure uniforme de C, il existe une partie finie J de I et un nombre ε > 0 tels que les relations |f_i(x) − f_i(y)| ≤ ε pour i ∈ J entraînent (x, y) ∈ W ; donc u|C est un isomorphisme de C sur u(C) pour les structures uniformes considérées.

#### Corollaire 1 {#evt-ii-s6-prop-11-cor-1 .statement}

Soient E un espace faible séparé, C un cône convexe saillant de sommet 0 dans E, complet pour la structure uniforme induite par celle de E. L’application (x, y) ↦ x + y de C × C dans C est propre.

Grâce à la prop. 11, on peut supposer que E = R^I et que C = R^I_+ (TG, I, p. 74, cor. 1 et 4). Mais alors l’application (x, y) ↦ x + y de C × C dans C s’écrit ((\xi_1), (\eta_1)) \mapsto (\xi_1 + \eta_1), et l’on peut se borner à prouver que l’application continue $f : (\xi, \eta) \mapsto \xi + \eta$ de $\mathbf{R}_+ \times \mathbf{R}_+$ dans $\mathbf{R}_+$ est propre (TG, I, p. 76, cor. 3). Or, pour tout $\zeta \in \mathbf{R}_+$, $f^{-1}(\zeta)$ est l’ensemble des couples $(\xi, \zeta - \xi)$ tels que $0 \leq \xi \leq \zeta$, donc l’image réciproque par $f$ d’un intervalle $[0, \zeta]$ est l’ensemble des $(\xi, \eta) \in \mathbf{R}_+ \times \mathbf{R}_+$ tels que $\xi + \eta \leq \zeta$, qui est compact. On conclut en appliquant TG, I, p. 77, prop. 7.

#### Corollaire 2 {#evt-ii-s6-prop-11-cor-2 .statement}

Soient E un espace faible séparé, C un cône convexe saillant de sommet 0 dans E, complet pour la structure uniforme induite par celle de E.
(i) Pour tout point a de E, l’intersection $C \cap (a - C)$ est compacte.
(ii) Soient A, B deux parties fermées de C. Alors A + B est une partie fermée de C.
(i) L’ensemble des $(x, y) \in C \times C$ tels que $x + y = a$ est compact d’après le cor. 1 et d’après TG, I, p. 75, th. 1, b). Or cet ensemble est aussi l’ensemble des $(x, a - x)$ pour $x \in C \cap (a - C)$, ce qui prouve (i).
(ii) Si A et B sont fermées dans C, $A \times B$ est fermée dans $C \times C$, donc $A + B$ est fermé dans C d’après le cor. 1 et d’après TG, I, p. 72, prop. 1.

## EXERCICES {#evt-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
