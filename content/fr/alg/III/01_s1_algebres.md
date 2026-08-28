---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 1
section_title: Algèbres
lang: fr
source: alg-i-iii-fr
pdf_pages: 0389-0399, 0565-0565
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une algèbre
      page: 0
      pdf_page: 389
    - "no": 2
      title: Sous-algèbres. Idéaux. Algèbres quotients
      page: 3
      pdf_page: 390
    - "no": 3
      title: Diagrammes exprimant l’associativité et la commutativité
      page: 5
      pdf_page: 392
    - "no": 4
      title: Produits d’algèbres
      page: 6
      pdf_page: 393
    - "no": 5
      title: Restriction et extension des scalaires
      page: 7
      pdf_page: 394
    - "no": 6
      title: Limites projectives et limites inductives d’algèbres
      page: 8
      pdf_page: 395
    - "no": 7
      title: Bases d’une algèbre. Table de multiplication
      page: 10
      pdf_page: 397
statements: 5
exercises: 1
content_sha256: 2d5e926b08c68d5e7ca5beba37db0cfedb5584bfc190c8df4ab07597ba9427c7
---

## § 1. ALGÈBRES

### 1. Définition d’une algèbre

#### Définition 1 {#alg-iii-s1-def-1 .statement}

Soit A un anneau commutatif. On appelle algèbre sur A (ou A-algèbre, ou simplement algèbre lorsqu’aucune confusion n’est à craindre), un ensemble E muni d’une structure définie par les données suivantes:
  1) une structure de A-module sur E;
  2) une application A-bilinéaire (II, p. 56) de E × E dans E.

L’application A-bilinéaire de E × E dans E qui intervient dans cette définition est appelée la multiplication dans l’algèbre E; on la note d’ordinaire (x, y) ↦ x . y, ou simplement (x, y) ↦ xy.

Soient (α_i)_{i \in I} et (β_j)_{j \in J} deux familles d’éléments de A, à support fini (I, p. 13). Alors, quelles que soient les familles (x_i)_{i \in I} et (y_j)_{j \in J} d’éléments de E, on a la formule générale de distributivité (I, p. 27)

$$
(\sum_{i \in I} α_i x_i)(\sum_{j \in J} β_j y_j) = \sum_{(i, j) \in I \times J} (α_i β_j)(x_i y_j);
$$

en particulier

$$(αx)y = x(αy) = α(xy)$$ pour $α \in A, x \in E$ et $y \in E$.

L’application bilinéaire (x, y) ↦ yx de E × E dans E et la structure de A-module de E définissent sur E une structure de A-algèbre, dite opposée à la structure d’algèbre donnée. L’ensemble E muni de cette nouvelle structure s’appelle l’algèbre opposée à l’algèbre E; on la note souvent E^0. On dit que la A-algèbre E est commutative si elle est identique à son opposée, autrement dit si la multiplication dans E est commutative. Un isomorphisme de E sur E^0 est encore appelé un antiautomorphisme de l’algèbre E.

Lorsque la multiplication dans l’algèbre E est associative, on dit que E est une A-algèbre associative. Lorsque la multiplication dans E admet un élément neutre (nécessairement unique (I, p. 12)), on dit que cet élément est l’élément unité de E et que E est une algèbre unifière.

#### Exemple 1 {#alg-iii-s1-n1-exa-1 .statement}

Tout anneau commutatif A peut être considéré comme une A-algèbre (associative et commutative).
  2) Soit E un pseudo-anneau (I, p. 93). La multiplication dans E et l’unique structure de \mathbf{Z}-module de E définissent sur E une structure de \mathbf{Z}-algèbre associative.
  3) Soient F un ensemble, A un anneau commutatif. L’ensemble A^F de toutes les applications de F dans A, muni de la structure d’anneau produit (I, p. 103) et de la structure de A-module produit (II, p. 11), est une A-algèbre associative et commutative.

4) Soit E une A-algèbre ; les lois internes $(x, y) \mapsto xy + yx$ et $(x, y) \mapsto xy - yx$ définissent (avec la structure de A-module de E) deux structures de A-algèbres sur E, qui ne sont pas en général associatives ; la première loi $(x, y) \mapsto xy + yx$ est toujours commutative.

#### Définition 2 {#alg-iii-s1-def-2 .statement}

*Etant données deux algèbres* E, E′ *sur un anneau commutatif* A, *on appelle homomorphisme de* E *dans* E′ *une application* $f : E \to E'$ *telle que*:
  1) $f$ *soit un homomorphisme de* A-*modules* ;
  2) $f(xy) = f(x)f(y)$ *quels que soient* $x \in E$ *et* $y \in E$.

Il est clair que le composé de deux homomorphismes de A-algèbres est un homomorphisme de A-algèbres. Tout homomorphisme bijectif d’algèbres est un isomorphisme. On peut donc prendre pour *morphismes* de l’espèce de structure de A-algèbre les homomorphismes de A-algèbres (E, IV, p. 11). Nous supposerons toujours par la suite qu’on a fait ce choix de morphismes. Si E, E′ sont deux A-algèbres, on note $\mathrm{Hom}_{\mathrm{A}-\mathrm{alg}}(E, E')$ l’ensemble des homomorphismes de A-algèbres de E dans E′.

Soient E, E′ deux algèbres ayant chacune un élément unité. Un homomorphisme de E dans E′ transformant l’élément unité de E en l’élément unité de E′ est appelé *homomorphisme unifère* (ou *morphisme unifère d’algèbres*).

### 2. Sous-algèbres. Idéaux. Algèbres quotients

Soient A un anneau commutatif, E une A-algèbre. Si F est un sous-A-module de E, stable pour la multiplication dans E, la restriction à F × F de la multiplication dans E définit (avec la structure de A-module de F) une structure de A-algèbre sur F. On dit que F, muni de cette structure, est une *sous-algèbre* de la A-algèbre E. Toute intersection de sous-algèbres de E est une sous-algèbre de E. Pour toute famille $(x_i)_{i \in I}$ d’éléments de E, l’intersection des sous-algèbres de E contenant tous les $x_i$ s’appelle la sous-algèbre de E *engendrée* par la famille $(x_i)_{i \in I}$ et on dit que $(x_i)_{i \in I}$ est un *système générateur* (ou une *famille génératrice*) de cette sous-algèbre. Si $u : E \to E'$ est un homomorphisme de A-algèbres, l’image $u(F)$ de toute sous-algèbre F de E est une sous-algèbre de E′.

Soit E une algèbre *associative*. Pour toute partie M de E, l’ensemble M′ des éléments de M permutables avec tous les éléments de M est une sous-algèbre de E, dite sous-algèbre *commutante* (ou *centralisatrice*) de M dans E (I, p. 8). La commutante M″ de M′ dans E est aussi appelée la *bicommunatante* de M ; il est clair que $M \subset M''$. On en conclut que M′ est contenu dans sa bicommunatante M″, qui n’est autre que la commutante de M″ ; mais la relation $M \subset M''$ entraîne $M'' \subset M'$, de sorte que $M' = M''$ (cf. E, III, p. 7, prop. 2). Si F est une sous-algèbre de E, le *centre* de F est l’intersection F ∩ F′ de F et de sa commutante F′ dans E. On notera que si F est commutative, on a $F \subset F'$, donc $F' \supset F''$; la bi-commutante $F''$ de F est dans ce cas le centre de $F'$.

Pour certaines algèbres non associatives (par exemple les algèbres de Lie), on définit autrement les notions de commutante d’une sous-algèbre et de centre (LIE, I, § 1, n°6).

On dit qu’une partie $a$ d’une A-algèbre E est un idéal à gauche (resp. idéal à droite) de E lorsque $a$ est un sous-A-module de E et que les relations $x \in a, y \in E$ entraînent $yx \in a$ (resp. $xy \in a$). Il revient au même de dire que $a$ est un idéal à gauche de E, ou un idéal à droite de l’algèbre opposée $E^0$. Un idéal bilatère de E est un sous-ensemble $a$ de E qui est à la fois idéal à gauche et idéal à droite. Lorsque E est associative et admet un élément unité $e$, on a, pour $\alpha \in A$ et $x \in E$, $\alpha x = (\alpha e)x = x(\alpha e)$ en vertu de (2) (III, p. 2), donc les idéaux (à droite, à gauche, bilatères) de l’anneau E (I, p. 98) sont identiques aux idéaux (à droite, à gauche, bilatères) de l’algèbre E. Toute somme et toute intersection d’idéaux à gauche (resp. à droite, resp. bilatères) de l’algèbre E est un idéal à gauche (resp. à droite, resp. bilatère). L’intersection des idéaux à gauche (resp. à droite, resp. bilatères) contenant une partie X de E est appelée l’idéal à gauche (resp. à droite, resp. bilatère) de E engendré par X.

Soit $b$ un idéal bilatère d’une A-algèbre E. Si $x \equiv x'$ (mod. $b$) et $y \equiv y'$ (mod. $b$), on a
$$
x(y - y') \in b \quad \text{et} \quad (x - x')y' \in b
$$
donc $xy \equiv x'y'$ (mod. $b$). On peut donc définir sur le A-module quotient $E/b$ une loi de composition quotient de la loi de multiplication $(x, y) \mapsto xy$ de E par la relation d’équivalence $x \equiv x'$ (mod. $b$) (I, p. 10). On vérifie aussitôt que cette loi quotient est une application A-bilinéaire de $(E/b) \times (E/b)$ dans $E/b$; elle définit donc avec la structure de A-module de $E/b$ une structure de A-algèbre sur $E/b$. On dit que $E/b$, muni de cette structure d’algèbre, est l’algèbre quotient de l’algèbre E par l’idéal bilatère $b$. L’application canonique $p : E \to E/b$ est un homomorphisme d’algèbres.

Soient E, E' deux A-algèbres, et $u : E \to E'$ un homomorphisme d’algèbres. L’image $u(E)$ est une sous-algèbre de E' et le noyau $b = \overline{u}^1(0)$ est un idéal bilatère de E; de plus, dans la décomposition canonique de $u$:
$$
E \xrightarrow{p} E/b \xrightarrow{v} u(E) \xrightarrow{j} E'
$$
$v$ est un isomorphisme d’algèbres. Plus généralement, tous les résultats de I, p. 100–102 sont encore valables (ainsi que leurs démonstrations) lorsqu’on remplace partout le mot « anneau » par « algèbre ».

Soient A un anneau commutatif, E une A-algèbre. Sur l’ensemble $\tilde{E} = A \times E$, définissons les lois de composition suivantes:

$$(\lambda, x) + (\mu, y) = (\lambda + \mu, x + y)$$
$$(\lambda, x)(\mu, y) = (\lambda \mu, xy + \mu x + \lambda y)$$
$$\lambda(\mu, x) = (\lambda \mu, \lambda x).$$

On vérifie aussitôt que $\tilde{E}$, muni de ces lois de composition, est une algèbre sur $A$, et que $(1, 0)$ est élément unité de cette algèbre. L’ensemble $\{0\} \times E$ est un idéal bilatère de $\tilde{E}$, et $x \mapsto (0, x)$ est un isomorphisme de l’algèbre $E$ sur la sous-algèbre $\{0\} \times E$, au moyen duquel on identifie $E$ et $\{0\} \times E$. On dit que $\tilde{E}$ est l’algèbre déduite de $E$ par adjonction d’un élément unité; elle est associative (resp. commutative) si et seulement si $E$ l’est.

### 3. Diagrammes exprimant l’associativité et la commutativité

Soient $A$ un anneau commutatif, $E$ un $A$-module; la donnée d’une application bilinéaire de $E \times E$ dans $E$ équivaut à celle d’une application $A$-linéaire:

$$ m : E \otimes_A E \to E $$

(II, p. 56). Une structure de $A$-algèbre sur $E$ est donc définie par la donnée d’une structure de $A$-module sur $E$ et d’une application $A$-linéaire de $E \otimes_A E$ dans $E$.

Soit $E'$ une seconde $A$-algèbre, et soit $m' : E' \otimes_A E' \to E'$ l’application $A$-linéaire définissant la multiplication de $E'$. Une application $f : E \to E'$ est un homomorphisme de $A$-algèbres si et seulement si $f$ est une application $A$-linéaire qui rend commutatif le diagramme

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{f \otimes f} & E' \otimes_A E' \\
m \downarrow & & \downarrow m' \\
E & \xrightarrow{f} & E'
\end{array}
$$

Pour qu’une $A$-algèbre $E$ soit associative, il faut et il suffit (compte tenu de l’associativité du produit tensoriel, cf. II, p. 64) que le diagramme d’applications $A$-linéaires

$$
\begin{array}{ccc}
E \otimes_A E \otimes_A E & \xrightarrow{m \otimes 1_E} & E \otimes_A E \\
1_E \otimes m \downarrow & & \downarrow m \\
E \otimes_A E & \xrightarrow{m} & E
\end{array}
$$

soit commutatif. De même, pour que l’algèbre $E$ soit commutative, il faut et il suffit que le diagramme d’applications $A$-linéaires

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E \\
m \downarrow & & \downarrow m \\
E & & E
\end{array}
$$

soit commutatif, en notant $\sigma$ l’application A-linéaire canonique définie par $\sigma(x \otimes y) = y \otimes x$ pour $x \in E, y \in E$ (II, p. 52, cor. 2).

Pour tout $c \in E$, notons $\eta_c$ l’application A-linéaire de A dans E définie par la condition $\eta_c(1) = c$. Pour que $c$ soit élément unité de E, il faut et il suffit que les deux diagrammes

$$
\begin{array}{ccc}
A \otimes_A E & \xrightarrow{\eta_c \otimes 1_E} & E \otimes_A E \\
i \downarrow & & m \downarrow \\
E & & E
\end{array}
$$
$$
\begin{array}{ccc}
E \otimes_A A & \xrightarrow{1_E \otimes \eta_c} & E \otimes_A E \\
i' \downarrow & & m \downarrow \\
E & & E
\end{array}
$$

soient commutatifs ($i$ et $i'$ désignant les isomorphismes canoniques (II, p. 55, prop. 4)).

Soit E une A-algèbre ayant un élément unité $e$, et posons $\eta = \eta_e$ (qu’on note aussi $\eta_E$); on a $\eta(\alpha \beta) = \eta(\alpha) \eta(\beta) = \alpha \eta(\beta)$ car, d’après (2) (III, p. 2), on a $(\alpha e)(\beta e) = (\alpha \beta)e = \alpha(\beta e)$; donc $\eta$ est un homomorphisme de A-algèbres. On observera que la structure de A-module de E peut se définir à l’aide de $\eta$, car on a
$$
\alpha x = \eta(\alpha) \cdot x \quad \text{pour } \alpha \in A, x \in E
$$
(où, dans le second membre, il s’agit de la multiplication dans E). L’image de l’homomorphisme $\eta$ est une sous-algèbre de E, dont les éléments commutent à tous ceux de E. Le noyau de l’homomorphisme $\eta$ est l’annulateur de l’élément $e$ du A-module E; d’après (3), c’est aussi l’annulateur du A-module E (II, p. 28).

Lorsque l’algèbre E est unifière et est associative, $\eta$ est un homomorphisme d’anneaux. Réciproquement, soit $\rho : A \to B$ un homomorphisme d’anneaux, tel que l’image $\rho(A)$ soit contenue dans le centre de B, l’anneau A étant en outre supposé commutatif; alors on définit sur B une structure de A-algèbre, associative et unifière, en posant (cf. (3))
$$
\lambda x = \rho(\lambda) \cdot x \quad \text{pour } \lambda \in A, x \in E.
$$

### 4. Produits d’algèbres

Soit $(E_i)_{i \in I}$ une famille d’algèbres sur un même anneau commutatif A. On vérifie immédiatement que sur l’ensemble produit $E = \prod_{i \in I} E_i$, la structure de A-module produit (II, p. 10) et la multiplication
$$
((x_i), (y_i)) \mapsto (x_i y_i)
$$
définissent une structure de A-algèbre; muni de cette structure, l’ensemble E est appelé l’algèbre produit de la famille d’algèbres $(E_i)_{i \in I}$.

Lorsque toutes les algèbres $E_i$ sont associatives (resp. commutatives, resp.

unifères) il en est de même de leur produit. En outre, toutes les propriétés énoncées dans I, p. 103–104 s’étendent sans modification aux produits d’algèbres quelconques.

### 5. Restriction et extension des scalaires

Soient $A_0$ et $A$ deux anneaux commutatifs, et $\rho : A_0 \to A$ un homomorphisme d’anneaux. Si $E$ est une $A$-algèbre, on notera (conformément à II, p. 30) $\rho_*(E)$ le $A_0$-module défini par l’addition de $E$ et la loi externe

$$
\lambda . x = \rho(\lambda)x \quad \text{pour tout } \lambda \in A_0 \text{ et tout } x \in E.
$$

La multiplication de $E$ et la structure de $A_0$-module de $\rho_*(E)$ définissent sur $\rho_*(E)$ une structure de $A_0$-algèbre. Lorsque $A_0$ est un sous-anneau de $A$ et que $\rho$ est l’injection canonique, on dit que l’algèbre $\rho_*(E)$ est obtenue à partir de $E$ par restriction à $A_0$ de l’anneau $A$ des scalaires. Par abus de langage, on le dit parfois encore lorsque l’homomorphisme $\rho$ est quelconque.

Soit $F$ une $A_0$-algèbre. On appelle semi-homomorphisme (relatif à $\rho$) ou $\rho$-homomorphisme de $F$ dans la $A$-algèbre $E$, un homomorphisme $F \to \rho_*(E)$ de $A_0$-algèbres; on dit aussi $A_0$-homomorphisme si aucune confusion n’en résulte. Si $E, E'$ sont deux $A$-algèbres, tout homomorphisme de $A$-algèbres $E \to E'$ est aussi un homomorphisme de $A_0$-algèbres $\rho_*(E) \to \rho_*(E')$.

Considérons maintenant deux anneaux commutatifs $A$ et $B$, et un homomorphisme d’anneaux $\rho : A \to B$. Pour tout $A$-module $E$, on a défini (II, p. 82) le $B$-module $\rho^*(E) = E \otimes_A B$ obtenu à partir de $E$ par extension à $B$ de l’anneau $A$ des scalaires. Si $E$ est en outre une $A$-algèbre, on va définir sur $\rho^*(E)$ une structure de $B$-algèbre. Pour cela, on observe que $(E \otimes_A B) \otimes_B (E \otimes_A B)$ est canoniquement isomorphe à $(E \otimes_A E) \otimes_A B$ (II, p. 83, prop. 3). Si $m : E \otimes_A E \to E$ définit la multiplication dans $E$, l’application $m \otimes 1_B : (E \otimes_A E) \otimes_A B \to E \otimes_A B$ s’identifie donc canoniquement à une application $B$-linéaire

$$
m' : \rho^*(E) \otimes_B \rho^*(E) \to \rho^*(E)
$$

qui définit sur $\rho^*(E)$ la structure de $B$-algèbre voulue. On a donc

$$(x \otimes \beta)(x' \otimes \beta') = (xx') \otimes (\beta \beta')$$

pour $x, x'$ dans $E$, $\beta$ et $\beta'$ dans $B$. On dit que la $B$-algèbre $\rho^*(E)$ est déduite de la $A$-algèbre $E$ par extension à $B$ de l’anneau $A$ des scalaires (au moyen de $\rho$). On la note aussi $E_{(B)}$ ou $E \otimes_A B$. Lorsque $E$ est associative (resp. commutative, resp. unifière), il en est de même de l’algèbre $\rho^*(E)$.

#### Proposition 1 {#alg-iii-s1-prop-1 .statement}

Pour toute $A$-algèbre $E$, l’application canonique $\varphi_E : x \mapsto x \otimes 1$ de $E$ dans $E_{(B)}$ est un $A$-homomorphisme d’algèbres. En outre, pour toute $B$-algèbre $F$, et tout $A$-homomorphisme $f : E \to F$, il existe un $B$-homomorphisme $\bar{f} : E_{(B)} \to F$ et un seul tel que $\bar{f}(x \otimes 1) = f(x)$ pour tout $x \in E$.

La première assertion résulte aussitôt de la définition de la multiplication dans $E_{(B)}$, qui donne $(x \otimes 1)(x' \otimes 1) = (xx') \otimes 1$ pour $x \in E$ et $x' \in E$. L’existence et l’unicité de l’application B-linéaire $\bar{f}$ de $E_{(B)}$ dans $F$ vérifiant la relation $\bar{f}(x \otimes 1) = f(x)$ pour tout $x \in E$ résultent de II, p. 82, prop. 1 ; tout revient à voir ici que $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ pour $y$ et $y'$ dans $E_{(B)}$; comme les éléments de la forme $x \otimes 1$ (avec $x \in E$) engendrent le B-module $E_{(B)}$, on peut se limiter au cas où $y = x \otimes 1$, $y' = x' \otimes 1$, avec $x \in E, x' \in E$; comme $yy' = (xx') \otimes 1$, la relation $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ résulte alors de la relation $f(xx') = f(x)f(x')$.

On peut encore dire que $f \mapsto \bar{f}$ est une bijection canonique

$$
\operatorname{Hom}_{A-\mathrm{alg.}}(E, \rho_*(F)) \to \operatorname{Hom}_{B-\mathrm{alg.}}(\rho^*(E), F).
$$

Le couple formé de $E_{(B)}$ et de $\varphi_E$ est donc solution du problème d’application universelle (E, IV, p. 23) où $\Sigma$ est l’espèce de structure de B-algèbre et les $\alpha$-applications les A-homomorphismes de $E$ dans une B-algèbre.

#### Corollaire {#alg-iii-s1-n5-cor-1 .statement}

Soient $E, E'$ deux A-algèbres; pour tout A-homomorphisme d’algèbres $u : E \to E'$, $u \otimes 1_B$ est l’unique B-homomorphisme d’algèbres $v : E \otimes_A B \to E' \otimes_A B$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
E & \xrightarrow{\varphi_E} & E \otimes_A B \\
u \downarrow & & \downarrow v \\
E' & \xrightarrow{\varphi_{E'}} & E' \otimes_A B
\end{array}
$$

Soient C un troisième anneau commutatif, $\sigma : B \to C$ un homomorphisme d’anneaux; il est immédiat que le C-homomorphisme canonique

$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$

transformant $(x \otimes 1) \otimes 1$ en $x \otimes 1$ pour tout $x \in E$ (II, p. 83, prop. 2) est un isomorphisme d’algèbres.

### 6. Limites projectives et limites inductives d’algèbres

Soient I un ensemble préordonné, $(A_i, \varphi_{ij})$ un système projectif d’anneaux commutatifs, ayant I pour ensemble d’indices. Soit $(E_i, f_{ij})$ un système projectif de $A_i$-modules ayant I pour ensemble d’indices (II, p. 89), et supposons en outre que chaque $E_i$ soit muni d’une structure de $A_i$-algèbre, et que, pour $i \leq j$, $f_{ij}$ soit un $A_j$-homomorphisme d’algèbres (relatif à $\varphi_{ij}$) (III, p. 7). Soient $A = \lim \leftarrow A_i$ et $E = \lim \leftarrow E_i$, qui est muni d’une structure de A-module, limite projective des structures des $A_i$-modules $E_i$ (II, p. 89); on vérifie aussitôt que sur $E$, considéré comme limite projective des $E_i$ considérés comme magmas pour la multiplication (I, p. 113), la loi de composition, avec la structure de A-module de $E$, définit sur $E$ une structure de A-algèbre; on dit que $(E_i, f_{ij})$ est un système projectif de $A_i$-algèbres et que la A-algèbre $E$ est sa limite projective. Si $f_i : E \to E_i, \varphi_i : A \to A_i$ sont les applications canoniques, $f_i$ est un $A$-homomorphisme d’algèbres (relatif à $\varphi_i$). Si les $E_i$ sont associatives (rcsp. commutatives), il en est de même de $E$; si chaque $E_i$ admet un élément unité $e_i$, et si $f_{ij}(e_j) = e_i$ pour $i \leq j$, $e = (e_i)$ est élément unité de l’algèbre $E$.

Soit $(E'_i, f'_{ij})$ un second système projectif de $A_i$-algèbres, et pour tout $i$, soit $u_i : E_i \to E'_i$ un homomorphisme de $A_i$-algèbres, ces applications formant un système projectif; alors $u = \lim_{\leftarrow} u_i$ est un homomorphisme de $A$-algèbres.

Supposons maintenant que tous les $A_i$ soient égaux à un même anneau commutatif $A$, et les $\varphi_{ij}$ à $\mathrm{Id}_A$, de sorte que $E = \lim_{\leftarrow} E_i$ est une $A$-algèbre. Soit $F$ une $A$-algèbre, et pour tout $i \in I$, soit $u_i : F \to E_i$ un homomorphisme de $A$-algèbres tel que $(u_i)$ soit un système projectif d’applications; alors $u = \lim_{\leftarrow} u_i$ est un homomorphisme de l’algèbre $F$ dans l’algèbre $E$. Inversement, pour tout homomorphisme de $A$-algèbres $v : F \to E$, la famille des $v_i = f_i \circ v$ est un système projectif d’homomorphismes de $A$-algèbres tel que $v = \lim_{\leftarrow} v_i$. Comme d’ailleurs, en posant $\bar{f}_{ij} = \mathrm{Hom}(1_F, f_{ij})$, il est clair que $(\mathrm{Hom}_{A\text{-alg.}}(F, E_i), \bar{f}_{ij})$ est un système projectif d’ensembles, on voit que les remarques précédentes s’expriment encore en disant que l’application canonique $v \mapsto (f_i \circ v)$ est une bijection

$$
l_F : \mathrm{Hom}_{A\text{-alg.}}(F, \lim_{\leftarrow} E_i) \to \lim_{\leftarrow} \mathrm{Hom}_{A\text{-alg.}}(F, E_i).
$$

En outre, pour tout homomorphisme $w : F \to F'$ de $A$-algèbres, les $\overline{w}_i = \mathrm{Hom}(w, 1_{E_i}) : \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \to \mathrm{Hom}_{A\text{-alg.}}(F, E_i)$ forment un système projectif d’applications, et le diagramme

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(F', \lim_{\leftarrow} E_i) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \\
\downarrow \mathrm{Hom}(w, 1_E) & & \downarrow \lim_{\leftarrow} \overline{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(F, \lim_{\leftarrow} E_i) & \xrightarrow{l_F} & \lim_{\leftarrow} \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
\end{array}
$$

est commutatif.

Supposons maintenant $I$ filtrant croissant. Considérons un système inductif d’anneaux commutatifs $(A_i, \varphi_{ji})$ et un système inductif $(E_i, f_{ji})$ de $A_i$-modules, ayant $I$ pour ensemble d’indices; supposons que chaque $E_i$ soit muni d’une structure de $A_i$-algèbre et que, pour $i \leq j$, $f_{ji}$ soit un $A_i$-homomorphisme d’algèbres (relatif à $\varphi_{ji}$) (III, p. 7). Soient $A = \lim_{\longrightarrow} A_i$, $E = \lim_{\longrightarrow} E_i$; $E$ est muni d’une structure de $A$-module, limite inductive des structures des $A_i$-modules $E_i$ (II, p. 90); en outre, sur $E$, considéré comme limite inductive des $E_i$, considérés comme magmas pour la multiplication (I, p. 115), la loi de composition, avec la structure de $A$-module de $E$, définit sur $E$ une structure de $A$-algèbre; on dit que $(E_i, f_{ji})$ est un système inductif de $A_i$-algèbres et que la $A$-algèbre $E$ est sa limite inductive. Si $f_i : E_i \to E$, $\varphi_i : A_i \to A$ sont les applications canoniques, $f_i$ est un $A_i$-homomorphisme d’algèbres (relatif à $\varphi_i$). Si les $E_i$ sont associatives (resp. commutatives), il en est de même de $E$; si chaque $E_i$ admet un élément unité $e_i$, et si $f_{ji}(e_i) = e_j$ pour $i \leq j$, $E$ admet un élément unité $e$ tel que $f_i(e_i) = e$ pour tout $i \in I$.

Soit $(E'_i, f'_{ij})$ un second système inductif de $A_i$-algèbres, et pour tout $i$, soit $u_i : E_i \to E'_i$ un homomorphisme de $A_i$-algèbres, ces applications formant un système inductif; alors $u = \lim \limits_{\longrightarrow} u_i$ est un homomorphisme de $A$-algèbres.

Supposons maintenant que tous les anneaux $A_i$ soient égaux à un même anneau $A$ et les $\varphi_{ji}$ à $\mathrm{Id}_A$, de sorte que $E = \lim \limits_{\longrightarrow} E_i$ est une $A$-algèbre. Soit $F$ une $A$-algèbre, et, pour tout $i$, soit $u_i : E_i \to F$ un homomorphisme de $A$-algèbres tel que $(u_i)$ soit un système inductif d’applications; alors $u = \lim \limits_{\longrightarrow} u_i$ est un homomorphisme de l’algèbre $E$ dans l’algèbre $F$. Inversement, pour tout homomorphisme de $A$-algèbres $v : E \to F$, la famille des $v_i = v \circ f_i$ est un système inductif d’homomorphismes de $A$-algèbres tel que $v = \lim \limits_{\longrightarrow} v_i$. Comme d’ailleurs, en posant $\bar{f}_{ij} = \mathrm{Hom}(f_{ji}, 1_F)$, il est clair que $(\mathrm{Hom}_{A\text{-alg.}}(E_i, F), \bar{f}_{ij})$ est un système projectif d’ensembles, on voit que les remarques précédentes s’expriment encore en disant que l’application canonique $v \mapsto (v \circ f_i)$ est une bijection

$$
d_F : \mathrm{Hom}_{A\text{-alg.}}(\lim \limits_{\longrightarrow} E_i, F) \to \lim \limits_{\longleftarrow} \mathrm{Hom}_{A\text{-alg.}}(E_i, F).
$$

En outre, pour tout homomorphisme $w : F \to F'$ de $A$-algèbres, les $\overline{w}_i = \mathrm{Hom}(1_{E_i}, w) : \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \to \mathrm{Hom}_{A\text{-alg.}}(E_i, F')$ forment un système projectif d’applications, et le diagramme

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(\lim \limits_{\longrightarrow} E_i, F) & \xrightarrow{d_F} & \lim \limits_{\longleftarrow} \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \\
\downarrow \mathrm{Hom}(1_{E_i}, w) & & \downarrow \lim \overline{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(\lim \limits_{\longrightarrow} E_i, F') & \xrightarrow{d_{F'}} & \lim \limits_{\longleftarrow} \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
\end{array}
$$

est commutatif.

### 7. Bases d’une algèbre. Table de multiplication

Par définition, une base d’une $A$-algèbre $E$ est une base de $E$ pour sa structure de $A$-module. Soit $(a_i)_{i \in I}$ une base de $E$; il existe une famille unique $(\gamma_{ij}^k)_{(i, j, k) \in I \times I \times I}$ d’éléments de l’anneau $A$ telle que pour tout couple $(i, j) \in I \times I$, l’ensemble des $k \in I$ tels que $\gamma_{ij}^k \neq 0$ soit fini, et que

$$
a_i a_j = \sum_{k \in L} \gamma_{ij}^k a_k.
$$

On dit que les $\gamma_{ij}^k$ sont les constantes de structure de l’algèbre $E$ par rapport à la base $(a_i)$, et que les relations (7) constituent la table de multiplication de l’algèbre $E$ (relativement à la base $(a_i)$).

On peut imaginer les relations (7) écrites en disposant les seconds membres de ces relations en un tableau carré

$$
\begin{array}{c|c|c|c}
& \cdots & a_j & \cdots \\
\hline
& & & \\
\vdots & & & \\
a_i & & \sum_k \gamma_{ij}^k a_k & \\
\vdots & & &
\end{array}
$$

étant entendu que l’élément qui figure dans la ligne d’indice $i$ et la colonne d’indice $j$ est égal au produit $a_i a_j$.

Réciproquement, donnons-nous un $A$-module $E$ et une base $(a_i)_{i \in I}$ de $E$, ainsi qu’une famille $(\gamma_{ij}^k)$ d’éléments de $A$ telle que, pour tout couple $(i, j) \in I \times I$, l’ensemble des $k \in I$ tels que $\gamma_{ij}^k \neq 0$ soit fini. Alors il y a sur $E$ une structure de $A$-algèbre et une seule pour laquelle les relations (7) sont satisfaites, puisque le $A$-module $E \otimes_A E$ est libre et admet pour base $(a_i \otimes a_j)_{(i, j) \in I \times I}$ (cf. II, p. 62, cor. 2).

Soient $E$ une $A$-algèbre, $(a_i)_{i \in I}$ un système générateur du $A$-module $E$ (par exemple une base). Pour que $E$ soit *associative*, il faut et il suffit que les $a_i$ vérifient les *relations d’associativité*

$$
(a_i a_j) a_k = a_i (a_j a_k) \quad \text{quels que soient } i, j, k.
$$

En effet l’application $(x, y, z) \mapsto (xy)z - x(yz)$ est une application $A$-trilinéaire $E \times E \times E \to E$, donc définit une application $A$-linéaire $E \otimes_A E \otimes_A E \to E$; si cette dernière application s’annule pour les éléments $a_i \otimes a_j \otimes a_k$, qui forment un système générateur du $A$-module $E \otimes_A E \otimes_A E$, elle est identiquement nulle.

De même, pour que $E$ soit *commutative*, il faut et il suffit que les $a_i$ vérifient les *relations de commutativité*

$$
a_i a_j = a_j a_i \quad \text{quels que soient } i, j.
$$

La démonstration est analogue en considérant cette fois l’application $A$-bilinéaire $(x, y) \mapsto xy - yx$. Enfin, pour qu’un élément $e \in E$ soit élément unité, il faut et il suffit que les $a_i$ vérifient les relations

$$
a_i = ea_i = a_i e \quad \text{quel que soit } i,
$$

comme on le voit cette fois en considérant les applications $A$-linéaires $x \mapsto x - xe$ et $x \mapsto x - ex$.

Lorsque $(a_i)_{i \in I}$ est une base de $E$ et $(\gamma_{ij}^k)$ la famille des constantes de structure correspondante, les relations (8) équivalent aux relations $\sum_r \gamma_{ij}^r \gamma_{rk}^s = \sum_r \gamma_{ir}^s \gamma_{jk}^r$ quels que soient $i, j, k, s$. De même les relations (9) équivalent à $\gamma_{ij}^k = \gamma_{ji}^k$ quels que soient $i, j, k$.

Soit $(a_i)_{i \in I}$ une base de la $A$-algèbre $E$; si $\rho : A \to B$ est un homomorphisme d’anneaux, $(a_i \otimes 1)$ est une base de la B-algèbre $\rho^*(E) = E \otimes_A B$ (II, p. 84, prop. 4). Si $(\gamma_{ij}^k)$ est la famille des constantes de structure de E relativement à la base $(a_i)$, la famille $(\rho(\gamma_{ij}^k))$ est la famille des constantes de structure de $\rho^*(E)$ relativement à la base $(a_i \otimes 1)$.

## EXERCICES {#alg-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
