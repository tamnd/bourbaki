---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 1
section_title: Dualité
lang: fr
source: evt-i-v-fr
pdf_pages: 0187-0200, 0233-0238
extraction: ocr
subsections:
    - "no": 1
      title: Topologies compatibles avec une dualité
      page: 0
      pdf_page: 187
    - "no": 2
      title: Topologie de Mackey et topologie affaiblie sur un espace localement convexe
      page: 4
      pdf_page: 190
    - "no": 3
      title: Transposée d’une application linéaire continue
      page: 6
      pdf_page: 192
    - "no": 4
      title: Dual d’un espace quotient et d’un sous-espace
      page: 8
      pdf_page: 194
    - "no": 5
      title: Dual d’une somme directe, d’un produit
      page: 11
      pdf_page: 197
statements: 37
exercises: 15
content_sha256: f80dff3a3050a781f0f70f941f94f7ab3a2bbce94e05271d6811d9ceeaf4c457
---

## § 1. DUALITÉ

### 1. Topologies compatibles avec une dualité

Dans ce numéro, on note E et F deux espaces vectoriels mis en dualité par une forme bilinéaire B (II, p. 43). On rappelle (II, p. 44) qu’on a défini deux applications linéaires

$$
d_B : F \to E^*, \quad s_B : E \to F^*
$$

caractérisées par la relation

(1)
$$
B(x, y) = \langle x, d_B(y) \rangle = \langle y, s_B(x) \rangle
$$

pour $x \in E,\ y \in F$.

#### Définition 1 {#evt-iv-s1-def-1 .statement}

On dit qu’une topologie localement convexe $\mathcal{T}$ sur E est compatible avec la dualité entre E et F si $d_B$ est une bijection de F sur le dual de l’espace localement convexe obtenu en munissant E de $\mathcal{T}$.

S’il existe une telle topologie $\mathcal{T}$, l’application $d_B$ est injective, c’est-à-dire que la dualité entre E et F est séparante en F (II, p. 44).

#### Proposition 1 {#evt-iv-s1-prop-1 .statement}

(i) Les parties convexes fermées dans E sont les mêmes pour toutes les topologies localement convexes sur E compatibles avec la dualité entre E et F.

(ii) Les parties bornées de E sont les mêmes pour toutes les topologies localement convexes sur E compatibles avec la dualité entre E et F.

Soit $\mathcal{T}$ une topologie sur E compatible avec la dualité entre E et F, donc plus fine que $\sigma(E, F)$. Si une partie convexe de E est fermée pour $\mathcal{T}$, elle est intersection de demi-espaces réels fermés (II, p. 41, cor. 1), donc fermée pour $\sigma(E, F)$. Ceci prouve (i). L’assertion (ii) a été démontrée au cor. 3 de III, p. 28.

Notons $F_\sigma$ l’espace vectoriel $F$ muni de la topologie faible $\sigma(F, E)$. Alors l’application linéaire $s_B$ applique $E$ sur le dual $(F_\sigma)'$ de $F_\sigma$ (II, p. 46, prop. 3). Soit $\mathcal{S}$ un ensemble de parties bornées de $F_\sigma$. Par abus de langage, on appelle $\mathcal{S}\text{-topologie sur } E$ l’image réciproque par $s_B$ de la $\mathcal{S}\text{-topologie sur } (F_\sigma)'$. Elle est définie par la famille des semi-normes

$$
p_A(x) = \sup_{y \in A} |B(x, y)| ,
$$

où $A$ parcourt $\mathcal{S}$. En particulier, lorsque $\mathcal{S}$ est l’ensemble des parties finies de $F$, la $\mathcal{S}\text{-topologie}$ n’est autre que la topologie faible $\sigma(E, F)$.

#### Définition 2 {#evt-iv-s1-def-2 .statement}

*Soient* $E$ et $F$ *deux espaces en dualité*. *On appelle topologie de Mackey sur* $E$, *et l’on note* $\tau(E, F)$, *la* $\mathcal{S}\text{-topologie sur } E$, *où* $\mathcal{S}$ *est l’ensemble des parties de* $F$ *dont l’image dans* $E^*$ *(par* $d_B$) *est convexe, équilibrée et compacte pour* $\sigma(E^*, E)$.

Lorsque la dualité entre $E$ et $F$ est séparante en $F$, $d_B$ est injective et la topologie $\sigma(F, E)$ sur $F$ est image réciproque par $d_B$ de la topologie $\sigma(E^*, E)$ sur $E^*$. Dans ce cas, $\mathcal{S}$ se compose des parties de $F$ qui sont convexes, équilibrées et compactes pour $\sigma(F, E)$.

En général, si $F_1 = d_B(F) \subset E^*$, et si l’on désigne par $(x, y_1) \mapsto B_1(x, y_1)$ la restriction de la forme bilinéaire canonique $(x, x^*) \mapsto \langle x, x^* \rangle$ à $E \times F_1$, $E$ et $F_1$ sont mis en dualité par $B_1$, et cette dualité est séparante en $F_1$; comme on a par définition $B(x, y) = B_1(x, d_B(y))$, la déf. 2 montre que $\tau(E, F) = \tau(E, F_1)$.

*Remarque* 1. — Soit $A$ une partie convexe compacte d’un espace localement convexe séparé $G$, et soit $\tilde{A}$ l’enveloppe fermée convexe équilibrée de $A$. Lorsque le corps $K$ est égal à $\mathbf{R}$, l’ensemble $\tilde{A}$ est l’enveloppe fermée convexe de $A \cup (-A)$; lorsque $K$ est égal à $\mathbf{C}$, l’ensemble $\tilde{A}$ est contenu dans l’enveloppe fermée convexe de $2A \cup (-2A) \cup (2iA) \cup (-2iA)$. Par suite (II, p. 14, prop. 15), $\tilde{A}$ est compact.

On en déduit en particulier que, lorsque la dualité entre $E$ et $F$ est séparante en $F$,
*la topologie de Mackey* $\tau(E, F)$ *est aussi la* $\mathcal{S}'\text{-topologie}$, *où* $\mathcal{S}'$ *est l’ensemble des parties convexes de* $F$ *qui sont compactes pour* $\sigma(F, E)$.

On définit de manière analogue la topologie de Mackey $\tau(F, E)$ sur $F$.

#### Théorème 1 (Mackey) {#evt-iv-s1-thm-1 .statement}

*Soient* $E$ et $F$ *deux espaces en dualité* ; *on suppose la dualité séparante en* $F$. *Pour qu’une topologie localement convexe* $\mathcal{T}$ *sur* $E$ *soit compatible avec la dualité entre* $E$ *et* $F$, *il faut et il suffit que* $\mathcal{T}$ *soit plus fine que la topologie* $\sigma(E, F)$ *et moins fine que la topologie de Mackey* $\tau(E, F)$.

Identifions $F$ à son image par $d_B$ dans $E^*$. Notons $\mathcal{S}_0$ l’ensemble des parties de $F$ qui sont convexes, équilibrées et compactes pour $\sigma(F, E)$. Par définition, $\tau(E, F)$ est la $\mathcal{S}_0$-topologie sur $E$, donc est plus fine que $\sigma(E, F)$.

*Lemme* 1. — *Le sous-espace* $F$ *de* $E^*$ *se compose des formes linéaires sur* $E$ *continues pour* $\tau(E, F)$.

Tout élément de F est une application continue pour $\sigma(E, F)$, donc pour $\tau(E, F)$.

Réciproquement, soit $f \in E^*$ continue pour $\tau(E, F)$. Il existe un voisinage U de 0 dans E (pour $\tau(E, F)$), tel que $|f| \leq 1$ sur U ; on peut supposer qu’il existe un ensemble $A \in \mathcal{S}_0$ tel que $U = A^\circ$. Autrement dit, $f$ appartient au bipolaire $A^{\circ\circ}$ de A pour la dualité entre $E^*$ et E. Or la topologie $\sigma(F, E)$ sur F est induite par $\sigma(E^*, E)$; par suite, A est convexe, équilibré et compact pour $\sigma(E^*, E)$, et le th. des bipolaires (II, p. 48, th. 1) entraîne l’égalité $A = A^{\circ\circ}$. On a donc $f \in F$, d’où le lemme 1.

#### Lemme 2 {#evt-iv-s1-lem-2 .statement}

Soit $\mathcal{T}$ une topologie localement convexe sur E telle que toute forme linéaire sur E continue pour $\mathcal{T}$ appartienne à F. Alors $\mathcal{T}$ est moins fine que $\tau(E, F)$.

Soit $\mathcal{U}$ l’ensemble des voisinages convexes et équilibrés de 0 pour $\mathcal{T}$. Soit $\mathcal{S}$ l’ensemble des polaires dans F des éléments de $\mathcal{U}$. On a $\mathcal{S} \subset \mathcal{S}_0$ d’après le cor. 2 de III, p. 17, et, d’après le cor. 1 de la prop. 7 de III, p. 19, $\mathcal{T}$ est identique à la $\mathcal{S}'$-topologie, où $\mathcal{S}'$ est l’ensemble des polaires des ensembles de $\mathcal{U}$ dans le dual $E'$ de E. Mais on a par hypothèse $E' \subset F$, donc tout ensemble de $\mathcal{S}'$ est contenu dans un ensemble de $\mathcal{S}$; d’où le lemme 2.

Soit $\mathcal{T}$ une topologie sur E compatible avec la dualité entre E et F. Alors $\mathcal{T}$ est moins fine que $\tau(E, F)$ d’après le lemme 2, et il est évident que $\mathcal{T}$ est plus fine que $\sigma(E, F)$. Réciproquement, F est le dual de E pour la topologie $\tau(E, F)$ (lemme 1) et pour la topologie $\sigma(E, F)$ (II, p. 46, prop. 3), donc aussi pour toute topologie intermédiaire entre $\tau(E, F)$ et $\sigma(E, F)$.

#### Corollaire {#evt-iv-s1-n1-cor-1 .statement}

Soit p une semi-norme sur E. Les conditions suivantes sont équivalentes :

(i) $p$ est continue pour la topologie $\tau(E, F)$;
(ii) toute forme linéaire $f$ sur E, telle que $|f| \leq p$, provient d’un élément de F.

(i) $\Rightarrow$ (ii) : si $p$ est continue pour $\tau(E, F)$, toute forme linéaire $f$ sur E telle que $|f| \leq p$ est continue pour $\tau(E, F)$, donc provient d’un élément de F d’après le lemme 1.

(ii) $\Rightarrow$ (i) : soit $\mathcal{T}$ la topologie sur E définie par la semi-norme $p$. Si la condition (ii) est satisfaite, les formes linéaires sur E continues pour $\mathcal{T}$ appartiennent à F. D’après le lemme 2, $\mathcal{T}$ est moins fine que $\tau(E, F)$, donc $p$ est continue pour $\tau(E, F)$.

#### Remarque 2 {#evt-iv-s1-n1-rem-2 .statement}

\* Soient K une partie convexe de F compacte pour la topologie faible $\sigma(F, E)$ et $\mu$ une mesure positive sur K. Posons

$$
p(x) = \int_K |\mathbf{B}(x, y)|\, d\mu(y)
$$

pour tout $x \in E$. Il est immédiat que $p$ est une semi-norme. De plus, pour tout $x \in E$, la relation « $|\mathbf{B}(x, y)| \leq 1$ pour tout $y \in K$ » entraîne $p(x) \leq \mu(K)$. Ceci prouve que la semi-norme $p$ sur E est continue pour la topologie de Mackey $\tau(E, F)$. \*

#### Exemple {#evt-iv-s1-n1-exa-1 .statement}

Soient G un espace localement convexe et $G'$ son dual. Sur $G'$, la topologie faible $\sigma(G', G)$ et la topologie de la convergence convexe compacte (III, p. 14) sont compatibles avec la dualité entre G' et G. En général, la topologie forte et la topologie de la convergence compacte sur G' ne sont pas compatibles avec la dualité entre G' et G. Rappelons cependant que lorsque G est séparé et quasi-complet, la topologie de la convergence compacte sur G' coïncide avec celle de la convergence convexe compacte (III, p. 8), donc est compatible avec la dualité entre G' et G.

#### Définition 3 {#evt-iv-s1-def-3 .statement}

Soient E et F deux espaces vectoriels en dualité. On note $\beta(E, F)$ la $\mathcal{S}$-topologie, où $\mathcal{S}$ est l’ensemble des parties de F qui sont bornées pour $\sigma(F, E)$.

On définit de manière symétrique la topologie $\beta(F, E)$ sur F. On montre facilement que la topologie $\beta(E, F)$ est identique à $\beta(E, F/E^\circ)$, ce qui permet de se ramener au cas où la dualité entre E et F est séparante en F.

#### Remarque 3 {#evt-iv-s1-n1-rem-3 .statement}

Notons $E_\sigma$ l’espace E muni de la topologie $\sigma(E, F)$. Les tonneaux (III, p. 24) dans $E_\sigma$ sont les parties de E qui sont convexes, équilibrées, fermées pour $\sigma(E, F)$ et absorbantes. Ce ne sont autres que les polaires des parties de F qui sont convexes, équilibrées et bornées pour $\sigma(F, E)$. Par suite, l’ensemble des tonneaux dans $E_\sigma$ est un système fondamental de voisinages de 0 pour la topologie $\beta(E, F)$ dans E. Autrement dit, une semi-norme sur E est continue pour $\beta(E, F)$ si et seulement si elle est semi-continue inférieurement pour $\sigma(E, F)$ (cf. III, p. 24, prop. 1).

#### Remarque 4 {#evt-iv-s1-n1-rem-4 .statement}

Soit $\mathcal{T}$ une topologie sur E compatible avec la dualité entre E et F. D’après la prop. 1, (ii) de IV, p. 1, la topologie $\beta(F, E)$ sur F n’est autre que la topologie forte sur F identifié au dual de E (muni de $\mathcal{T}$).

#### Remarque 5 {#evt-iv-s1-n1-rem-5 .statement}

La topologie $\beta(E, F)$ sur E est plus fine que $\tau(E, F)$. Elle n’est pas en général compatible avec la dualité entre E et F (cf. cependant § 2). En particulier, une partie de E bornée pour $\sigma(E, F)$ n’est pas nécessairement bornée pour $\beta(E, F)$.

### 2. Topologie de Mackey et topologie affaiblie sur un espace localement convexe

Soient E un espace localement convexe, et E' son dual. On met E et E' en dualité au moyen de la forme bilinéaire canonique $(x, x') \mapsto \langle x, x' \rangle$ sur $E \times E'$. Cette dualité est séparante en E'. Sur E, nous disposons de trois topologies compatibles avec la dualité entre E et E' :

a) la topologie donnée sur E, qu’on appellera topologie initiale lorsqu’on voudra éviter les confusions ;
b) la topologie $\sigma(E, E')$, dite topologie affaiblie sur E ;
c) la topologie $\tau(E, E')$, dite topologie de Mackey sur E.
La topologie initiale est plus fine que la topologie affaiblie et moins fine que la topologie de Mackey ; ces trois topologies peuvent d’ailleurs être distinctes (IV, p. 49, exerc. 8).

D’après la prop. 1 de IV, p. 1, ces trois topologies ont les mêmes ensembles convexes fermés, les mêmes tonneaux, les mêmes ensembles bornés et les mêmes bornologies adaptées. En particulier :

#### Proposition 2 {#evt-iv-s1-prop-2 .statement}

Soit E un espace localement convexe, et soit A une partie convexe de E (par exemple, un sous-espace vectoriel de E). L’adhérence de A est la même pour la topologie initiale et pour la topologie affaiblie de E.

#### Remarque 1 {#evt-iv-s1-n2-rem-1 .statement}

Pour qu’une famille $(x_i)_{i\in I}$ d’éléments de $E$ soit totale (resp. topologiquement libre) pour la topologie initiale, il faut et il suffit qu’elle le soit pour la topologie affaiblie ; cela résulte de la prop. 2. On peut donc appliquer les critères de II, p. 46.

#### Remarque 2 {#evt-iv-s1-n2-rem-2 .statement}

Soient $\mathcal{T}_1$ et $\mathcal{T}_2$ deux topologies localement convexes sur $E$, compatibles avec la dualité entre $E$ et $E'$, $\mathcal{T}_1$ étant plus fine que $\mathcal{T}_2$. Alors tout voisinage de 0 pour $\mathcal{T}_1$ qui est convexe et fermé pour $\mathcal{T}_1$ est fermé pour $\mathcal{T}_2$ d’après la prop. 1 de IV, p. 1. Par suite (TG, II, p. 16, corollaire), toute partie de $E$ qui est complète pour $\mathcal{T}_2$ l’est aussi pour $\mathcal{T}_1$.

En particulier, toute partie de $E$ complète pour la topologie affaiblie l’est pour la topologie initiale, toute partie de $E$ complète pour la topologie initiale l’est pour la topologie de Mackey. Si $E$ est quasi-complet pour la topologie affaiblie, il l’est pour toute topologie compatible avec la dualité entre $E$ et $E'$. S’il est quasi-complet pour la topologie initiale, il l’est pour la topologie de Mackey.

#### Remarque 3 {#evt-iv-s1-n2-rem-3 .statement}

Supposons $E$ séparé (pour la topologie initiale). Soit $A$ une partie de $E$, bornée et fermée pour $\sigma(E, E')$, donc aussi pour toute topologie compatible avec la dualité entre $E$ et $E'$. Comme $A$ est précompacte pour $\sigma(E, E')$ (III, p. 3, Remarque 5), il revient au même de supposer que $A$ est complète ou compacte pour $\sigma(E, E')$.

Compte tenu de la remarque 2, on voit donc que :

#### Proposition 3 {#evt-iv-s1-prop-3 .statement}

*Supposons* $E$ séparé, et soit $E'$ son dual. *Toute partie de* $E$ *qui est précompacte pour la topologie initiale, et compacte pour* $\sigma(E, E')$, *est compacte pour la topologie initiale*.

#### Remarque 4 {#evt-iv-s1-n2-rem-4 .statement}

La topologie $\beta(E, E')$ (IV, p. 4, déf. 3) est plus fine que la topologie de Mackey. Si $\beta(E, E')$ est distincte de $\tau(E, E')$, elle n’est pas compatible avec la dualité entre $E$ et $E'$. L’espace $E$ est tonnelé si et seulement si la topologie initiale est égale à $\beta(E, E')$ (III, p. 24).

#### Proposition 4 {#evt-iv-s1-prop-4 .statement}

*Soit* $E$ *un espace localement convexe*. *La topologie de Mackey sur* $E$ *est identique à la topologie initiale dans chacun des cas suivants* :
    a) $E$ *est tonnelé* ;
    b) $E$ *est bornologique* ;
    c) $E$ *est métrisable*.

Remarquons d’abord que la topologie de Mackey de $E$ est identique à la topologie initiale si et seulement si toute partie convexe de $E'$, compacte pour $\sigma(E', E)$, est équicontinue. C’est certainement le cas si $E$ est tonnelé (III, p. 24, corollaire).

Supposons $E$ bornologique, et soit $V$ un voisinage convexe et équilibré de 0 dans $E$ pour la topologie $\tau(E, E')$. Soit $B$ une partie de $E$ bornée pour la topologie initiale. Comme $B$ est bornée pour la topologie de Mackey, $V$ absorbe $B$, et comme $E$ est bornologique, $V$ est un voisinage de 0 pour la topologie initiale.

Dans le cas $c)$, l’espace $E$ est bornologique (III, p. 12, prop. 2).

### 3. Transposée d’une application linéaire continue

Dans ce numéro, on note $E_1$ et $E_2$ deux espaces localement convexes, ayant respectivement pour duals $E'_1$ et $E'_2$.

Soit $u$ une application linéaire de $E_1$ dans $E_2$. Pour que $u$ soit continue lorsqu’on munit $E_1$ et $E_2$ des topologies affaiblies, il faut et il suffit que $f \circ u$ appartienne à $E'_1$ pour toute $f \in E'_2$; c’est le cas si $u$ est continue. On appelle alors transposée de $u$, et l’on note $^t u$, l’application linéaire $f \mapsto f \circ u$ de $E'_2$ dans $E'_1$.

#### Proposition 5 {#evt-iv-s1-prop-5 .statement}

*Soit $u$ une application linéaire continue de $E_1$ dans $E_2$.*

(i) *Si $E_1$ et $E_2$ sont séparés, pour que $u$ soit injective, il faut et il suffit que l’image de $^t u$ soit dense dans $E'_1$ muni de la topologie faible $\sigma(E'_1, E_1)$.*

(ii) *Pour que $^t u$ soit injective, il faut et il suffit que l’image de $u$ soit dense dans $E_2$.*

Un sous-espace vectoriel de $E_2$ est dense pour la topologie initiale si et seulement s’il l’est pour la topologie affaiblie (IV, p. 4, prop. 2). La prop. 5 résulte alors de II, p. 51, cor. 2.

#### Proposition 6 {#evt-iv-s1-prop-6 .statement}

*Soit $u$ une application linéaire de $E_1$ dans $E_2$, continue pour les topologies affaiblies. Pour $i = 1, 2$, soit $\mathcal{S}_i$ un ensemble de parties bornées de $E_i$. Pour que $^t u$ soit une application continue de $(E'_2)_{\mathcal{S}_2}$ dans $(E'_1)_{\mathcal{S}_1}$, il faut et il suffit que, pour tout ensemble $A \in \mathcal{S}_1$, il existe des ensembles $A_1, ..., A_n$ dans $\mathcal{S}_2$ et un nombre réel $\lambda > 0$ tels que $\lambda . u(A)$ soit contenu dans l’enveloppe fermée convexe équilibrée de $A_1 \cup ... \cup A_n$^1.*

C’est une conséquence immédiate de la prop. 2 de III, p. 15.

#### Corollaire {#evt-iv-s1-n3-cor-1 .statement}

*Soit $u$ une application linéaire continue de $E_1$ dans $E_2$. Alors $^t u$ est continue lorsqu’on munit les duals $E'_i$ des topologies suivantes :*
  a) *les topologies faibles $\sigma(E'_i, E_i)$;*
  b) *les topologies fortes $\beta(E'_i, E_i)$;*
  c) *les topologies de Mackey $\tau(E'_i, E_i)$;*
  d) *les topologies de la convergence précompacte.*
*En outre, lorsque $E_2$ est séparé, $^t u$ est continue lorsqu’on munit les duals $E'_i$:*
  e) *des topologies de la convergence compacte* (resp. *compacte convexe*).

Le seul point qui demande une démonstration est le cas c), lorsque les topologies de $E_1$ et $E_2$ ne sont pas nécessairement séparées. Alors pour toute forme linéaire $f \in E'_1*$, $f \circ ^t u$ est une forme linéaire sur $E'_2$; donc il y a une application linéaire $v : E'_1* \to E'_2*$, continue pour les topologies $\sigma(E'_1*, E'_1)$ et $\sigma(E'_2*, E'_2)$ et telle que $d_{B_2} \circ u = v \circ d_{B_1}$, où $d_{B_i}$ est l’application canonique de $E_i$ dans $E'_i*$ ($i = 1, 2$). Par suite, si $A$ est une partie de $E_1$ telle que $d_{B_1}(A)$ soit convexe, équilibrée et compacte pour $\sigma(E'_1*, E'_1)$, $d_{B_2}(u(A)) = v(d_{B_1}(A))$ est convexe, équilibrée et compacte pour $\sigma(E'_2*, E'_2)$, les topologies $\sigma(E'_1*, E'_1)$ et $\sigma(E'_2*, E'_2)$ étant séparées.

^1 Autrement dit, $u(\mathcal{S}_1)$ est contenu dans la plus petite bornologie adaptée contenant $\mathcal{S}_2$ (III, p. 3).

#### Proposition 7 {#evt-iv-s1-prop-7 .statement}

Soit $u : E_1 \to E_2$ une application linéaire. On suppose que $u$ est continue pour les topologies affaiblies de $E_1$ et $E_2$.

(i) L’application $u$ est continue si l’on munit $E_1$ et $E_2$ de leurs topologies de Mackey.

(ii) Si $E_1$ est bornologique ou tonnelé, $u$ est continue pour les topologies initiales de $E_1$ et $E_2$.

(iii) Pour que $u$ soit continue pour les topologies initiales de $E_1$ et $E_2$, il faut et il suffit que l’image par $'u$ de toute partie équicontinue de $E_2'$ soit équicontinue dans $E_1'$.

L’hypothèse entraîne que $'u$ est continue pour les topologies faibles $\sigma(E_2', E_2)$ et $\sigma(E_1', E_1)$ (II, p. 50, corollaire); donc l’image par $'u$ d’une partie convexe, équilibrée et compacte pour $\sigma(E_2', E_2)$ est convexe, équilibrée et compacte pour $\sigma(E_1', E_1)$, les topologies $\sigma(E_2', E_2)$ et $\sigma(E_1', E_1)$ étant séparées. L’assertion (i) résulte alors de TG, X, p. 5, prop. 3, b). L’assertion (ii) est conséquence de (i): en effet, si $E_1$ est bornologique ou tonnelé, sa topologie initiale est celle de Mackey, et la topologie de Mackey de $E_2$ est de toute façon plus fine que la topologie initiale de $E_2$. Enfin, la topologie initiale de $E_i$ est celle de la convergence uniforme dans les parties équicontinues de $E_i'$ (III, p. 19, cor. 1 de la prop. 7), d’où (iii).

#### Corollaire {#evt-iv-s1-n3-cor-2 .statement}

Supposons que $E_1$ soit un espace normé. Soit $u$ une application linéaire de $E_1$ dans $E_2$. Les propriétés suivantes sont équivalentes:

a) $u$ est continue;
b) $u$ est continue pour les topologies affaiblies;
c) l’image par $u$ de la boule unité dans $E_1$ est bornée dans $E_2$;
d) pour toute suite $(x_n)$ de points de $E_1$ tendant vers 0 pour la topologie initiale, la suite $(u(x_n))$ est bornée pour la topologie affaiblie de $E_2$.

Comme $E_1$ est bornologique, l’équivalence de a) et b) résulte de la prop. 7. Celle de a) et c) est immédiate. L’équivalence de a) et d) résulte de la prop. 1 de IV, p. 1 et de la prop. 1 de III, p. 11.

#### Proposition 8 {#evt-iv-s1-prop-8 .statement}

(i) Soit $E$ un espace normé, de dual $E'$. Pour tout $x \in E$, on a
$$
\|x\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x, x' \rangle|.
$$
(ii) Soient $E_1$ et $E_2$ deux espaces normés et $u$ une application linéaire continue de $E_1$ dans $E_2$. On a
$$
\|u'\| = \|u\|.
$$
Soit $x \in E$. Pour tout $x' \in E'$ tel que $\|x'\| \leq 1$, on a
$$
|\langle x, x' \rangle| \leq \|x\| \cdot \|x'\| \leq \|x\|.
$$
D’après le th. de Hahn-Banach (II, p. 24, cor. 2), il existe un élément $x'$ de $E'$ tel que $\|x'\| \leq 1$ et $\langle x, x' \rangle = \|x\|$. Ceci prouve (i).

Prouvons (ii). D’après la formule (3) et la définition de la transposée, on a
$$
\|u'\| = \sup_{\|y'\| \leq 1} \|u'(y')\| = \sup_{\|y'\| \leq 1, \|x\| \leq 1} |\langle x, u'(y') \rangle|
= \sup_{\|x\| \leq 1, \|y'\| \leq 1} |\langle u(x), y' \rangle| = \sup_{\|x\| \leq 1} \|u(x)\| = \|u\|.
$$

#### Remarque 1 {#evt-iv-s1-n3-rem-1 .statement}

La formule (3) est le cas particulier de (4) correspondant à l’application linéaire $\lambda \mapsto \lambda x$ de K dans E.
2) Posons $B(x, y') = \langle u(x), y' \rangle = \langle x, 'u(y') \rangle$ pour $x \in E_1,\ y' \in E'_2$. La démonstration précédente montre que B est une forme bilinéaire continue sur $E_1 \times E'_2$, de norme (TG, X, p. 23) égale à $\|u\|$.

#### Corollaire {#evt-iv-s1-n3-cor-3 .statement}

Soit E un espace normé de type dénombrable. Il existe une partie dénombrable D de $E' - \{0\}$ telle que l’on ait

(5)
$$
\|x\| = \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\|
$$
pour tout $x \in E$.

Soit $B'$ la boule unité du dual $E'$ de E, munie de la topologie faible $\sigma(E', E)$. C’est un espace compact métrisable (III, p. 19, cor. 2); il existe donc une partie dénombrable dense $D'$ de $B'$. Posons $D = D' \cap (E' - \{0\})$. Soit $x \in E$; l’application $x' \mapsto \langle x, x' \rangle$ de $B'$ dans K est continue, d’où
$$
\sup_{x' \in B'} |\langle x, x' \rangle| = \sup_{\xi \in D'} |\langle x, \xi \rangle| \leq \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\| \leq \|x\|.
$$
La formule (5) résulte alors de (3).

### 4. Dual d’un espace quotient et d’un sous-espace

Dans tout ce numéro, on note E un espace localement convexe, M un sous-espace vectoriel de E, et $M^\circ$ l’orthogonal de M dans le dual $E'$ de E. On note $p$ l’application canonique de E sur $E/M$; alors $'p$ est injective, d’image $M^\circ$, donc définit un isomorphisme d’espaces vectoriels (non topologiques)

$$
\pi : (E/M)' \to M^\circ .
$$

De même, soit $i$ l’injection canonique de M dans E. Alors $'i$ est surjective (II, p. 26, prop. 2); son noyau est égal à $M^\circ$, d’où un isomorphisme d’espaces vectoriels (non topologiques)

$$
i : E'/M^\circ \to M'.
$$

#### Proposition 9 {#evt-iv-s1-prop-9 .statement}

(i) Pour qu’une partie A de $(E/M)'$ soit équicontinue, il faut et il suffit que $\pi(A)$ soit une partie équicontinue de $E'$.
(ii) Soient $\mathfrak{S}$ un ensemble de parties bornées de E, et $\mathfrak{S}_1$ l’ensemble des images dans $E/M$ des parties $A \in \mathfrak{S}$. Alors $\pi$ est un isomorphisme de $(E/M)'_{\mathfrak{S}_1}$ sur $M^\circ$ muni de la topologie induite par celle de $E'_{\mathfrak{S}}$.
(iii) Supposons E normé. Alors $\pi$ est une isométrie de l’espace normé $(E/M)'$ sur le sous-espace normé $M^\circ$ de $E'$.

Soient A une partie de $(E/M)'$ et $B = 'p(A) \subset E'$. Posons

$$
q(\xi) = \sup_{\xi' \in A} |\langle \xi, \xi' \rangle|
$$

pour tout $\xi \in E/M$. Pour que A soit équicontinue, il faut et il suffit que l’application q de E/M dans $\overline{\mathbf{R}}_+$ soit une semi-norme continue. Ceci signifie que $q \circ p$ est une semi-norme continue sur E (II, p. 29, prop. 5, (ii)). Comme on a

$$
(q \circ p)(x) = \sup_{x' \in B} |\langle x, x' \rangle|
$$

pour tout $x \in E$, ceci signifie encore que B est équicontinu dans $E'$, d’où (i).

Soient $A \in \mathcal{S}$ et $f$ une forme linéaire continue sur E/M. Pour tout $\lambda \in \mathbf{R}_+$, on a $|f| \leq \lambda$ sur $p(A)$ si et seulement si l’on a $|'p(f)| \leq \lambda$ sur A ; d’où (ii).

Prouvons enfin (iii). Soit $y'$ dans $(E/M)'$. Pour qu’un élément de E/M soit de norme < 1, il faut et il suffit qu’il soit l’image par p d’un élément de norme < 1 dans E. On a donc

$$
\begin{align*}
\|y'\| &= \sup_{y \in E/M, \|y\| < 1} |\langle y, y' \rangle| = \sup_{x \in E, \|x\| < 1} |\langle p(x), y' \rangle| \\
&= \sup_{x \in E, \|x\| < 1} |\langle x, 'p(y') \rangle| = \|'p(y')\|,
\end{align*}
$$

et $'p$ induit une isométrie de $(E/M)'$ sur $M^\circ$.

#### Proposition 10 {#evt-iv-s1-prop-10 .statement}

(i) *Pour qu’une partie A de M’ soit équicontinue, il faut et il suffit qu’elle soit l’image par $'i$ d’une partie équicontinue de E’*.

(ii) *Supposons M fermé dans E. Soit $\mathcal{S}$ un recouvrement de E formé de parties bornées et soit $\mathcal{S}_1$ l’ensemble des parties de M de la forme $M \cap A$ pour A dans $\mathcal{S}$. L’application linéaire bijective $i$ de $E'_\mathcal{S}/M^\circ$ sur $M'_{\mathcal{S}_1}$ est continue. C’est un homéomorphisme si $\mathcal{S}$ est filtrant pour la relation $\subset$ et se compose d’ensembles convexes fermés et compacts pour $\sigma(E, E')$*.

(iii) *Supposons E normé. Alors $i$ est une isométrie de $E'/M^\circ$ sur $M'$*.

L’image par $'i$ d’une partie équicontinue de $E'$ est une partie équicontinue de $M'$ (IV, p. 47, prop. 7). Réciproquement, soit A une partie équicontinue de $M'$. La topologie de M est définie par l’ensemble des restrictions à M des semi-normes continues sur E. Il existe donc une semi-norme continue p sur E telle que $|f(x)| \leq p(x)$ pour $f \in A$ et $x \in M$. Soit B l’ensemble des formes linéaires g sur E, telles que $|g| \leq p$ et dont la restriction à M appartient à A. L’ensemble B est équicontinu dans $E'$; d’après le th. de Hahn-Banach (II, p. 24, cor. 1), on a $'i(B) = A$, d’où (i).

Prouvons (ii). D’après la prop. 6 de IV, p. 6, l’application linéaire $'i$ de $E'_\mathcal{S}$ dans $M'_{\mathcal{S}_1}$ est continue, et définit donc par passage au quotient une application linéaire continue $i$ de $E'_\mathcal{S}/M^\circ$ sur $M'_{\mathcal{S}_1}$. Soit $\mathcal{T}$ la topologie sur $M'$ obtenue en transportant celle de $E'_\mathcal{S}/M^\circ$ par $i$; elle est plus fine que la $\mathcal{S}_1$-topologie.

Supposons maintenant que $\mathcal{S}$ soit filtrant pour $\subset$ et se compose d’ensembles convexes, équilibrés, fermés et compacts pour $\sigma(E, E')$. Pour montrer que $i$ est un homéomorphisme, c’est-à-dire que $\mathcal{T}$ est moins fine que la $\mathcal{S}_1$-topologie sur $M'$, il suffit de prouver que $\mathcal{T}$ est compatible avec la dualité entre $M'$ et M et que tout ensemble équicontinu dans M (considéré comme dual de $M'$ muni de $\mathcal{T}$) est contenu dans l’homothétique d’un ensemble appartenant à $\mathcal{S}_1$. Comme $\mathcal{T}$ est plus fine que la $\mathcal{S}_1$-topologie et que $\mathcal{S}_1$ est un recouvrement de $M$, la forme linéaire $y' \mapsto \langle y, y' \rangle$ sur $M'$ est continue pour $\mathcal{T}$ quel que soit $y \in M$. Soit $f$ une forme linéaire sur $M'$, continue pour $\mathcal{T}$; alors $f \circ 'i$ est une forme linéaire continue sur $E'_\mathcal{S}$. La $\mathcal{S}$-topologie sur $E'$ est moins fine que la topologie de Mackey $\tau(E', E)$; en effet, l’application $d_B : E \to E'^*$ est continue pour les topologies $\sigma(E, E')$ et $\sigma(E'^*, E')$, et comme cette dernière est séparée, l’image par $d_B$ d’un ensemble compact pour $\sigma(E, E')$ est compacte pour $\sigma(E'^*, E')$. D’après le lemme 1 de IV, p. 2, il existe $x_0 \in E$ tel que $f('i(x')) = \langle x_0, x' \rangle$ pour tout $x' \in E'$. En particulier, on a $\langle x_0, x' \rangle = 0$ pour tout $x' \in M^\circ$, et comme $M$ est fermé dans $E$, on a donc $x_0 \in M$ (II, p. 48, cor. 2), et finalement $f(y') = \langle x_0, y' \rangle$ pour tout $y' \in M'$, ce qui prouve que $\mathcal{T}$ est compatible avec la dualité entre $M$ et $M'$.

Soit maintenant $A$ une partie de $M$ équicontinue pour la topologie $\mathcal{T}$ sur $M'$. Par définition de $\mathcal{T}$, et en vertu de l’hypothèse que $\mathcal{S}$ est filtrant, cela signifie qu’il existe un ensemble $B \in \mathcal{S}$ contenant $0$ et tel que la borne supérieure $\lambda$ des nombres $|\langle y, x' \rangle|$, pour $y \in A$ et $x' \in B^\circ$, soit finie (III, p. 19, prop. 7). Comme $B$ est fermé dans $E$, le th. des bipolaires (II, p. 48, th. 1) montre que l’on a $A \subset \lambda(B \cap M)$, ce qui achève de prouver (ii).

Prouvons (iii). Soit $y' \in M'$. Il s’agit d’établir la formule
$$
\|y'\| = \inf_{'i(x') = y'} \|x'\|.
$$
D’après la prop. 8, (ii) de IV, p. 7, on a $\|'i\| = \|i\|$, d’où $\|'i\| \leq 1$, et donc
$$
\|y'\| \leq \inf_{'i(x') = y'} \|x'\|.
$$
D’après le th. de Hahn-Banach (II, p. 25, cor. 3), il existe une forme linéaire $x'_0$ sur $E$, prolongeant $y'$ et de même norme, d’où l’inégalité opposée à (7) puisque $'i(x'_0) = y'$.

#### Remarque {#evt-iv-s1-n4-rem-1 .statement}

On sait (II, p. 51, prop. 7, (ii)) que $i$ est un isomorphisme d’espaces vectoriels topologiques de $E'_s/M^\circ$ sur $M'_s$ (duals faibles). En ce qui concerne la topologie de la convergence convexe compacte, la prop. 10 montre que $i$ est un isomorphisme de $E'_{cc}/M^\circ$ sur $M'_{cc}$ lorsque $E$ est séparé et $M$ fermé dans $E$. Pour les topologies fortes, $i$ est une application continue de $E'_b/M^\circ$ sur $M'_b$; c’est un isomorphisme si $E$ est un espace de Banach \* ou si $E$ est semi-réflexif et $M$ fermé dans $E$ (IV, p. 15) *, mais il n’en est pas toujours ainsi si $E$ est un espace de Fréchet (IV, p. 58, exerc. 5, c)).

#### Proposition 11 {#evt-iv-s1-prop-11 .statement}

(i) La topologie affaiblie sur $E/M$ est quotient de celle de $E$; la topologie affaiblie sur $M$ est induite par celle de $E$.
(ii) La topologie de Mackey sur $E/M$ est quotient de celle de $E$; la topologie de Mackey de $M$ est plus fine que la topologie induite par $\tau(E, E')$.

L’assertion (i) résulte de la prop. 7 de II, p. 51.

L’injection canonique $i : M \to E$ est continue pour les topologies affaiblies, donc pour les topologies de Mackey $\tau(M, M')$ et $\tau(E, E')$ (IV, p. 7, prop. 7). De même, la projection canonique $p : E \to E/M$ est continue pour les topologies de Mackey. On voit aussitôt que la topologie quotient sur $E/M$ de $\tau(E, E')$ est compatible avec la dualité entre $E/M$ et $(E/M)'$, donc est moins fine que la topologie de Mackey de $E/M$ d’après le th. de Mackey (IV, p. 2, th. 1). Ceci prouve (ii).

### 5. Dual d’une somme directe, d’un produit

Pour tout $i \in I$, soit $(E_i, F_i)$ un couple d’espaces vectoriels mis en dualité par une forme bilinéaire $B_i$. On pose $E = \prod_{i \in I} E_i$ et $F = \bigoplus_{i \in I} F_i$, et l’on identifie chaque $F_i$ à un sous-espace de $F$. On met $E$ et $F$ en dualité au moyen de la forme bilinéaire

$$
B(x, y) = \sum_{i \in I} B_i(x_i, y_i) \quad \text{pour} \quad x = (x_i) \quad \text{et} \quad y = (y_i)
$$

(la famille $(B_i(x_i, y_i))_{i \in I}$ est à support fini).

On rappelle (II, p. 53, prop. 8) que la topologie faible $\sigma(E, F)$ est produit des topologies faibles $\sigma(E_i, F_i)$.

#### Lemme 3 {#evt-iv-s1-lem-3 .statement}

(i) Pour tout $i \in I$, soit $\mathcal{S}_i$ un ensemble de parties de $F_i$, bornées pour $\sigma(F_i, E_i)$; posons $\mathcal{S} = \bigcup_{i \in I} \mathcal{S}_i$. Alors la $\mathcal{S}$-topologie sur $E$ est produit des $\mathcal{S}_i$-topologies sur les $E_i$.

(ii) Pour tout $i \in I$, soit $\mathfrak{J}_i$ une bornologie adaptée sur l’espace $E_i$ muni de la topologie faible $\sigma(E_i, F_i)$, non réduite à $\{\emptyset\}$. Soit $\mathfrak{J}$ l’ensemble des parties $A$ de $E = \prod_{i \in I} E_i$ telles que $\operatorname{pr}_i(A) \in \mathfrak{J}_i$ pour tout $i \in I$. Alors la $\mathfrak{J}$-topologie sur $F$ est somme directe des $\mathfrak{J}_i$-topologies sur les $F_i$.

Soit $\mathcal{T}$ le produit des $\mathcal{S}_i$-topologies. Un système fondamental de voisinages de 0 pour $\mathcal{T}$ est formé des ensembles de la forme $A = \prod_{i \in J} A_i^\circ \times \prod_{i \in I - J} E_i$, où $J \subset I$ est fini et $A_i \in \mathcal{S}_i$ pour tout $i \in J$. On a $A = (\bigcup_{i \in J} A_i)^\circ$, donc $\mathcal{T}$ est identique à la $\mathcal{S}$-topologie.

Ceci prouve (i).

Munissons $F$ de la $\mathfrak{J}$-topologie et chaque $F_i$ de la $\mathfrak{J}_i$-topologie. Pour toute partie $A$ de $E$, on a $F_i \cap A^\circ = \operatorname{pr}_i(A)^\circ$, donc l’injection de $F_i$ dans $F$ est continue. Soit $q$ une semi-norme sur $F$; on suppose que la restriction $q_i$ de $q$ à $F_i$ est continue pour tout $i \in I$. On peut donc trouver des parties non vides $A_i \in \mathfrak{J}_i$ telles que l’on ait

$$
q_i(y_i) \leq \sup_{x_i \in A_i} |B_i(x_i, y_i)| \quad (y_i \in F_i) .
$$

Posons $A = \prod_{i \in I} A_i$, d’où $A \in \mathfrak{J}$. Pour $y = (y_i)_{i \in I}$ dans $F$, on a alors

$$
q(y) \leq \sum_{i \in I} q_i(y_i) \leq \sum_{i \in I} \sup_{x_i \in A_i} |B_i(x_i, y_i)| = \sup_{x \in A} |B(x, y)| ,
$$

où la dernière égalité résulte de (8) puisque la famille $(y_i)_{i \in I}$ est à support fini et les $A_i$ sont non vides et peuvent être supposées équilibrées (TG, IV, p. 26, cor. 2). Cette inégalité prouve que $q$ est continue sur $F$, d’où (ii).

#### Proposition 12 {#evt-iv-s1-prop-12 .statement}

La topologie $\beta(F, E)$ est somme directe des topologies $\beta(F_i, E_i)$. La topologie $\beta(E, F)$ est produit des topologies $\beta(E_i, F_i)$.

Nous appliquerons le lemme 3 en prenant pour $\mathcal{S}_i$ l’ensemble de toutes les parties de $F_i$ bornées pour $\sigma(F_i, E_i)$ et pour $\mathfrak{J}_i$ l’ensemble de toutes les parties de $E_i$ bornées pour $\sigma(E_i, F_i)$.

D’après le cor. 2 de III, p. 4, $\mathfrak{J}$ est l’ensemble de toutes les parties de $E$ bornées pour la topologie produit des $\sigma(E_i, F_i)$, identique à $\sigma(E, F)$. D’où l’assertion sur $\beta(F, E)$.

Munissons $F = \bigoplus_{i \in I} F_i$ de la topologie $\mathcal{T}$ somme directe des $\sigma(F_i, E_i)$. Le dual de $F$ se compose alors des formes linéaires $y \mapsto B(x, y)$ pour $x$ parcourant $E$ (II, p. 32, prop. 6). D’après la prop. 1 de IV, p. 1, les topologies $\mathcal{T}$ et $\sigma(F, E)$ ont les mêmes ensembles bornés. Supposons d’abord les topologies $\sigma(F_i, E_i)$ séparées. D’après la prop. 5 de III, p. 5, ces ensembles sont ceux contenus dans une partie de la forme $\sum_{i \in J} B_i$ avec $J \subset I$ fini et $B_i$ borné dans $F_i$ (pour $\sigma(F_i, E_i)$) quel que soit $i \in J$. Comme $\sum_{i \in J} B_i$ est contenue dans l’enveloppe convexe de $\bigcup_{i \in J} nB_i$, où $n = \mathrm{Card}(J)$, on peut appliquer le lemme 3, d’où l’assertion sur $\beta(E, F)$ dans ce cas.

Dans le cas général, soit $N_i$ l’intersection des voisinages de 0 pour $\sigma(F_i, E_i)$, et soit $N = \sum_{i \in I} N_i$, de sorte que $F/N$ est somme directe topologique des $F_i/N_i$ (II, p. 33, prop. 8) ; on en déduit que toute partie bornée de $F$ pour $\mathcal{T}$ est contenue dans un ensemble de la forme $N + \sum_{i \in J} B_i$ avec $J \subset I$ fini et $B_i$ borné dans $F_i$ pour tout $i \in J$ (III, p. 2, Remarque 3) ; comme le polaire de cet ensemble dans $E$ est le même que celui de $\sum_{i \in J} B_i$, on conclut comme ci-dessus.

#### Proposition 13 {#evt-iv-s1-prop-13 .statement}

*La topologie de Mackey* $\tau(F, E)$ *est somme directe des topologies de Mackey* $\tau(F_i, E_i)$. *La topologie* $\tau(E, F)$ *est produit des topologies* $\tau(E_i, F_i)$.

L’assertion sur $\tau(F, E)$ résulte du lemme 3 (ii) et de la propriété suivante : pour qu’une partie convexe, équilibrée, et fermée de $F^* = \prod_{i \in I} F_i^*$ soit compacte pour $\sigma(F^*, F)$, il faut et il suffit que sa projection sur chaque $F_i^*$ soit compacte pour $\sigma(F_i^*, F_i)$.

Pour prouver l’assertion sur $\tau(E, F)$, supposons d’abord les topologies $\sigma(F_i, E_i)$ séparées ; il suffit (lemme 3 (i)) de prouver que toute partie $A$ de $F$ qui est convexe, équilibrée et compacte pour $\sigma(F, E)$ est contenue dans un ensemble de la forme $\sum_{i \in J} A_i$ où $J \subset I$ est fini et où $A_i$ est convexe, équilibrée et compacte pour $\sigma(F_i, E_i)$. Or une telle partie $A$ est bornée pour $\sigma(F, E)$. D’après la démonstration de la prop. 12, il existe donc une partie finie $J$ de $I$ telle que $A \subset \sum_{i \in J} F_i$, et il suffit de prendre pour $A_i$ la projection de $A$ sur $F_i$.

Dans le cas général, en conservant les notations de la preuve de la prop. 12, on a $\tau(E_i, F_i) = \tau(E_i, F_i/N_i)$ et $\tau(E, F) = \tau(E, F/N)$ (IV, p. 2), et comme $F/N$ est somme directe topologique des $F_i/N_i$, on est ramené au cas précédent.

C.Q.F.D.

Dans la fin de ce paragraphe, on suppose que $(E_i)_{i \in I}$ est une famille d’espaces localement convexes. On note S la somme directe topologique des E_i et P leur produit. On définit une application linéaire $\theta : S' \to \prod_{i \in I} E'_i$, dite canonique, par
$$
\theta(x') = (x'|E_i)_{i \in I} \quad (x' \in S')
$$
(on a noté S' le dual de S, et E'_i celui de E_i).

#### Proposition 14 {#evt-iv-s1-prop-14 .statement}

(i) *L’application $\theta$ est un isomorphisme du dual fort (resp. faible) de $S = \bigoplus_{i \in I} E_i$ sur le produit des duals forts (resp. faibles) des $E_i$.*
(ii) *Pour qu’une partie A de S' soit équicontinue, il faut et il suffit que la projection de $\theta(A)$ sur $E'_i$ soit équicontinue pour tout $i \in I$.*
(iii) *La topologie de Mackey $\tau(S, S')$ est somme directe des topologies de Mackey $\tau(E_i, E'_i)$.*
(iv) *La topologie $\beta(S, S')$ est somme directe des topologies $\beta(E_i, E'_i)$.*

Que $\theta$ soit bijectif résulte aussitôt de la définition d’une somme directe topologique (II, p. 32, prop. 6). L’assertion (i) résulte alors de la prop. 12 de IV, p. 11, pour les topologies fortes et de la prop. 8 de II, p. 53, pour les topologies faibles. De même (iii) résulte de la prop. 13 (IV, p. 12) et (iv) de la prop. 12 (IV, p. 11).

Prouvons (ii). Soit A une partie de S'. Posons
$$
q(x) = \sup_{x' \in A} |\langle x, x' \rangle| \quad \text{pour } x \in S;
$$
notons $q_i$ la restriction de $q$ à $E_i$, d’où
$$
q_i(x_i) = \sup_{x'_i \in A_i} |\langle x_i, x'_i \rangle| \quad \text{pour } x_i \in E_i,
$$
en notant $A_i$ la projection de $\theta(A)$ sur $E'_i$. Pour que A soit équicontinue, il faut et il suffit que $q$ soit finie (c’est-à-dire chaque $q_i$ finie) et $q$ continue. Vu la caractérisation des semi-normes continues sur une somme directe topologique (II, p. 29, prop. 5), il revient au même de supposer chaque $q_i$ continue, ou encore que chaque ensemble $A_i$ est équicontinu.

C.Q.F.D.

Soit $\varphi$ l’application linéaire, dite canonique, de $\bigoplus_{i \in I} E'_i$ dans le dual $P'$ de $P = \prod_{i \in I} E_i$ définie par la formule
$$
\langle x, \varphi(x') \rangle = \sum_{i \in I} \langle x_i, x'_i \rangle
$$
pour $x = (x_i)$ dans $P$ et $x' = (x'_i)$ dans $\bigoplus_{i \in I} E'_i$.

#### Proposition 15 {#evt-iv-s1-prop-15 .statement}

(i) *L’application $\varphi$ est un isomorphisme de la somme directe topologique des duals forts des $E_i$ sur le dual fort de $P = \prod_{i \in I} E_i$.*
(ii) *Pour qu’une partie A de $P'$ soit équicontinue, il faut et il suffit qu’elle soit contenue dans une somme finie $\sum_{i \in J} \varphi(A_i)$, où $J \subset I$ est fini et $A_i$ est équicontinu dans $E'_i$ pour tout $i \in J$.*

(iii) *La topologie de Mackey* $\tau(P, P')$ *est produit des topologies* $\tau(E_i, E'_i)$.
(iv) *La topologie* $\beta(P, P')$ *est produit des topologies* $\beta(E_i, E'_i)$.

Il est immédiat que $\varphi$ est injective. Un système fondamental de voisinages de 0 dans $P$ est formé des ensembles de la forme $V = \prod_{i \in J} V_i \times \prod_{i \in I - J} E_i$, où $J \subset I$ est fini et $V_i$ un voisinage de 0 dans $E_i$ pour $i$ dans $J$. Le polaire de $V$ dans $P'$ est égal à $\sum_{i \in J} \varphi(V_i^0)$.

Ceci démontre à la fois la surjectivité de $\varphi$ et l’assertion (ii).

Les assertions (i) et (iv) résultent alors de la prop. 12 (IV, p. 11) et (iii) de la prop. 13 (IV, p. 12).

#### Corollaire {#evt-iv-s1-n5-cor-1 .statement}

*Tout produit d’espaces tonnelés est tonnelé*.

Un espace localement convexe $E$ est tonnelé si et seulement si sa topologie initiale est identique à $\beta(E, E')$ (IV, p. 4, *Remarque* 3). Il suffit alors d’appliquer la prop. 15, (iv).

## EXERCICES {#evt-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
