---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 3
section_title: Produits tensoriels
lang: fr
source: alg-i-iii-fr
book_pages: A II.50-A II.72, A II.189-A II.190
pdf_pages: 0227-0249, 0366-0367
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel de deux modules
      page: 50
      pdf_page: 227
    - "no": 2
      title: Produit tensoriel de deux applications linéaires
      page: 52
      pdf_page: 229
    - "no": 3
      title: Changement d’anneau
      page: 53
      pdf_page: 230
    - "no": 4
      title: Opérateurs sur un produit tensoriel; produits tensoriels comme multimodules
      page: 54
      pdf_page: 231
    - "no": 5
      title: Produit tensoriel de deux modules sur un anneau commutatif
      page: 56
      pdf_page: 233
    - "no": 6
      title: Propriétés de $E \otimes_A F$ relatives aux suites exactes
      page: 58
      pdf_page: 235
    - "no": 7
      title: Produits tensoriels de produits et de sommes directes
      page: 60
      pdf_page: 237
    - "no": 8
      title: Associativité du produit tensoriel.
      page: 64
      pdf_page: 241
    - "no": 9
      title: Produit tensoriel de familles de multimodules
      page: 65
      pdf_page: 242
statements: 30
exercises: 4
content_sha256: b28aa9ba5da82ab13bd8a0b86b506db6372623388c4fd44c594b7ece0775bd9b
---

## § 3. PRODUITS TENSORIELS

### 1. Produit tensoriel de deux modules

Soient $G_1, G_2$ deux $\mathbf{Z}$-modules; on dit qu’une application $u$ de l’ensemble $G = G_1 \times G_2$ dans un $\mathbf{Z}$-module est biadditive (ou $\mathbf{Z}$-bilinéaire) si $u(x_1, x_2)$ est « additive par rapport à $x_1$ et par rapport à $x_2$ »; de façon précise, cela signifie que, pour $x_1, y_1$ dans $G_1$, $x_2, y_2$ dans $G_2$, on a
$$
\begin{align*}
u(x_1 + y_1, x_2) &= u(x_1, x_2) + u(y_1, x_2) \\
u(x_1, x_2 + y_2) &= u(x_1, x_2) + u(x_1, y_2).
\end{align*}
$$
On notera que cela entraîne en particulier $u(0, x_2) = u(x_1, 0) = 0$ quels que soient $x_1 \in G_1, x_2 \in G_2$.

Soient $A$ un anneau, $E$ un $A$-module à droite, $F$ un $A$-module à gauche. Nous allons considérer le problème d’application universelle (E, IV, p. 22) où $\Sigma$ est l’espèce de structure de $\mathbf{Z}$-module (les morphismes étant donc les applications $\mathbf{Z}$-linéaires, autrement dit les homomorphismes de groupes additifs) et où les $\alpha$-applications sont les applications $f$ de $E \times F$ dans un $\mathbf{Z}$-module $G$ qui sont $\mathbf{Z}$-bilinéaires et sont telles en outre que, pour tout $x \in E$, tout $y \in F$ et tout $\lambda \in A$, on ait
$$
f(x \lambda, y) = f(x, \lambda y).
$$
Montrons que ce problème admet une solution. Pour cela, considérons le $\mathbf{Z}$-module $C = \mathbf{Z}^{(E \times F)}$ des combinaisons linéaires formelles des éléments de $E \times F$ à coefficients dans $\mathbf{Z}$ (II, p. 25), dont on peut considérer qu’une base est formée des couples $(x, y)$, où $x \in E$ et $y \in F$. Soit $D$ le sous-$\mathbf{Z}$-module de $C$ engendré par les éléments de l’un des types suivants:
$$
\begin{cases}
(x_1 + x_2, y) - (x_1, y) - (x_2, y) \\
(x, y_1 + y_2) - (x, y_1) - (x, y_2) \\
(x \lambda, y) - (x, \lambda y)
\end{cases}
$$
où $x, x_1, x_2$ sont dans $E$, $y, y_1, y_2$ dans $F$ et $\lambda$ dans $A$.

INITION 1. — On appelle produit tensoriel du A-module à droite E et du A-module à gauche F, et on note $E \otimes_A F$ ou $E \otimes_A F$ (ou simplement $E \otimes F$ si aucune confusion n’est à craindre) le $\mathbf{Z}$-module quotient $C/D$ (quotient du $\mathbf{Z}$-module $C$ des combinaisons linéaires formelles d’éléments de $E \times F$ à coefficients dans $\mathbf{Z}$, par le sous-module $D$ engendré par les éléments de l’un des types (2)). Pour $x \in E$ et $y \in F$, on note $x \otimes y$ et on appelle produit tensoriel de $x$ et de $y$ l’élément de $E \otimes_A F$ image canonique de l’élément $(x, y)$ de $C = \mathbf{Z}^{(E \times F)}$.

L’application $(x, y) \mapsto x \otimes y$ de $E \times F$ dans $E \otimes_A F$ est dite canonique. C’est une application $\mathbf{Z}$-bilinéaire qui vérifie les conditions (1).

Montrons que le produit tensoriel $E \otimes_A F$ et l’application canonique précédente forment une solution du problème d’application universelle posé plus haut. De façon précise:

#### Proposition 1 {#alg-ii-s3-prop-1 .statement}

a) Soit $g$ une application $\mathbf{Z}$-linéaire de $E \otimes_A F$ dans un $\mathbf{Z}$-module $G$. L’application $(x, y) \mapsto f(x, y) = g(x \otimes y)$ de $E \times F$ dans $G$ est $\mathbf{Z}$-bilinéaire et vérifie les conditions (1).

b) Réciproquement, soit $f$ une application $\mathbf{Z}$-bilinéaire de $E \times F$ dans un $\mathbf{Z}$-module $G$, vérifiant les conditions (1). Il existe alors une application $\mathbf{Z}$-linéaire $g$ de $E \otimes_A F$ dans $G$ et une seule telle que $f(x, y) = g(x \otimes y)$ pour $x \in E, y \in F$.

Si $\varphi$ désigne l’application canonique de $E \times F$ dans $E \otimes_A F$, on a $f = g \circ \varphi$; d’où a). Pour démontrer b), remarquons qu’avec les notations de la déf. 1, $f$ se prolonge en une application $\mathbf{Z}$-linéaire $\bar{f}$ de $C$ dans $G$ (II, p. 24, prop. 17). En vertu des relations (1), $\bar{f}$ s’annule pour tous les éléments de $C$ de l’un des types (2), donc dans $D$. Il existe par suite une application $\mathbf{Z}$-linéaire $g$ de $C/D = E \otimes_A F$ dans $G$ telle que $\bar{f} = g \circ \psi$, où $\psi : C \to C/D$ est l’homomorphisme canonique (II, p. 16, Remarque). L’unicité de $g$ est immédiate, puisque $E \otimes_A F$ est engendré, en tant que $\mathbf{Z}$-module, par les éléments de la forme $x \otimes y$.

La prop. 1 définit un isomorphisme canonique du $\mathbf{Z}$-module des applications $\mathbf{Z}$-bilinéaires $f$ de $E \times F$ dans $G$, vérifiant les conditions (1), sur le $\mathbf{Z}$-module $\mathrm{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$.

Lorsque $A = \mathbf{Z}$, les conditions (1) sont automatiquement vérifiées pour toute application $\mathbf{Z}$-bilinéaire $f$, et le sous-module $D$ de $C$ est déjà engendré par les éléments des deux premiers types (2).

Si maintenant on revient au cas général, et si $E'$ et $F'$ désignent les $\mathbf{Z}$-modules sous-jacents à $E$ et $F$ respectivement, la remarque précédente et la déf. 1 montrent aussitôt que le $\mathbf{Z}$-module $E \otimes_A F$ peut s’identifier canoniquement au quotient du $\mathbf{Z}$-module $E' \otimes_{\mathbf{Z}} F'$ par le sous-$\mathbf{Z}$-module engendré par les éléments de la forme $(x \lambda) \otimes y - x \otimes (\lambda y)$, où $x$ parcourt $E$, $y$ parcourt $F$ et $\lambda$ parcourt $A$.

#### Corollaire 1 {#alg-ii-s3-prop-1-cor-1 .statement}

Soient $H$ un $\mathbf{Z}$-module, $h : E \times F \to H$ une application $\mathbf{Z}$-bilinéaire vérifiant les conditions (1) et telle que $H$ soit engendré par $h(E \times F)$. Supposons que pour tout $\mathbf{Z}$-module $G$ et toute application $\mathbf{Z}$-bilinéaire $f$ de $E \times F$ dans $G$ vérifiant (1), il existe une application $\mathbf{Z}$-linéaire $g : H \to G$ telle que $f = g \circ h$. Alors, si $\varphi$ désigne l’application canonique de $E \times F$ dans $E \otimes_A F$, il existe un isomorphisme et un seul $\theta$ de $E \otimes_A F$ sur $H$ tel que $h = \theta \circ \varphi$.

L’hypothèse que $h(E \times F)$ engendre $H$ entraîne en effet l’unicité de $g$; le corollaire n’est autre alors que la propriété générale d’unicité d’une solution d’un problème d’application universelle (E, IV, p. 23).

#### Corollaire 2 {#alg-ii-s3-prop-1-cor-2 .statement}

Désignons par $E^0$ (resp. $F^0$) le module $E$ (resp. $F$) considéré comme module à gauche (resp. à droite) sur l’anneau opposé $A^0$; il existe alors un isomorphisme $\sigma : E \otimes_A F \to F^0 \otimes_{A^0} E^0$ de $\mathbf{Z}$-modules et un seul tel que l’on ait $\sigma(x \otimes y) = y \otimes x$ pour $x \in E$ et $y \in F$ (« commutativité » du produit tensoriel).

En effet, par définition des structures de $A^0$-module sur $E^0$ et $F^0$, l’application $(x, y) \mapsto y \otimes x$ de $E \times F$ dans $F^0 \otimes_{A^0} E^0$ est $\mathbf{Z}$-bilinéaire et vérifie les conditions (1), d’où l’existence et l’unicité de l’application $\mathbf{Z}$-linéaire $\sigma$. On définit de même une application $\mathbf{Z}$-linéaire $\tau : F^0 \otimes_{A^0} E^0 \to E \otimes_A F$ telle que $\tau(y \otimes x) = x \otimes y$, et il est clair que $\sigma$ et $\tau$ sont des isomorphismes réciproques.

#### Remarque {#alg-ii-s3-n1-rem-1 .statement}

Le produit tensoriel de modules non réduits à 0 peut se réduire à 0 : par exemple, si l’on considère les deux $\mathbf{Z}$-modules $E = \mathbf{Z}/2\mathbf{Z}$ et $F = \mathbf{Z}/3\mathbf{Z}$, on a $2x = 0$ et $3y = 0$ quels que soient $x \in E$, $y \in F$; par suite, dans $E \otimes_F F$, on a $x \otimes y = 3(x \otimes y) - 2(x \otimes y) = x \otimes (3y) - (2x) \otimes y = 0$ quels que soient $x$ et $y$ (cf. II, p. 60, cor. 4).

### 2. Produit tensoriel de deux applications linéaires

Soient $A$ un anneau, $E, E'$ deux $A$-modules à droite, $F, F'$ deux $A$-modules à gauche, $u : E \to E'$ et $v : F \to F'$ deux applications $A$-linéaires. On vérifie immédiatement que l’application
$$
(x, y) \mapsto u(x) \otimes v(y)
$$
de $E \times F$ dans $E' \otimes_A F'$ est $\mathbf{Z}$-bilinéaire et satisfait aux conditions (1) de II, p. 50. En vertu de la prop. 1 de II, p. 51, il existe donc une application $\mathbf{Z}$-linéaire et une seule $w : E \otimes_A F \to E' \otimes_A F'$ telle que
$$
w(x \otimes y) = u(x) \otimes v(y)
$$
pour $x \in E, y \in F$. Cette application se note $u \otimes v$ (lorsqu’il n’en résulte pas de confusion) et s’appelle le produit tensoriel des applications linéaires $u$ et $v$.

On déduit aussitôt de (3) que $(u, v) \mapsto u \otimes v$ est une application $\mathbf{Z}$-bilinéaire dite canonique :
$$
\operatorname{Hom}_A(E, E') \times \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F')
$$
Il lui correspond d’après la prop. 1 de II, p. 51 une application $\mathbf{Z}$-linéaire dite canonique :
$$
\operatorname{Hom}_A(E, E') \otimes_{\mathbf{Z}} \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F')
$$
qui, à tout élément $u \otimes v$ du produit tensoriel, fait correspondre l’application linéaire $u \otimes v : E \otimes_A F \to E' \otimes_A F'$. On notera que l’application canonique (4) n’est pas nécessairement injective ni surjective. La notation $u \otimes v$ pourra donc prêter à confusion et il sera nécessaire que le contexte indique s’il s’agit d’un élément d’un produit tensoriel ou d’une application linéaire.

En outre, soient $E''$ un A-module à droite, $F''$ un A-module à gauche, $u': E' \to E''$, $v': F' \to F''$ des applications A-linéaires; il résulte de (3) que l’on a
$$
(u' \circ u) \otimes (v' \circ v) = (u' \otimes v') \circ (u \otimes v).
$$

### 3. Changement d’anneau

#### Proposition 2 {#alg-ii-s3-prop-2 .statement}

Soient $A, B$ deux anneaux, $\rho : B \to A$ un homomorphisme d’anneaux, $E$ (resp. $F$) un A-module à droite (resp. à gauche). Il existe alors une application $\mathbf{Z}$-linéaire et une seule
$$
\varphi : \rho_*(E) \otimes_B \rho_*(F) \to E \otimes_A F
$$
telle que pour tout $x \in E$ et tout $y \in F$, l’image par $\varphi$ de l’élément $x \otimes y$ de $\rho_*(E) \otimes_B \rho_*(F)$ soit l’élément $x \otimes y$ de $E \otimes_A F$; cette application $\mathbf{Z}$-linéaire est surjective.

Considérons en effet l’application $(x, y) \mapsto x \otimes y$ de $\rho_*(E) \times \rho_*(F)$ dans $E \otimes_A F$; elle est $\mathbf{Z}$-bilinéaire et pour tout $\beta \in B$, on a par définition $(x \rho(\beta)) \otimes y = x \otimes (\rho(\beta)y)$, donc les conditions (1) de II, p. 50 sont vérifiées, d’où l’existence et l’unicité de $\varphi$ (II, p. 51, prop. 1). La dernière assertion résulte de ce que les éléments $x \otimes y$ engendrent le $\mathbf{Z}$-module $E \otimes_A F$.

L’application (6) est dite canonique.

#### Corollaire {#alg-ii-s3-n3-cor-1 .statement}

Soient $\mathfrak{J}$ un idéal bilatère de $A$, tel que $\mathfrak{J}$ soit contenu dans l’annulateur de $E$ et dans l’annulateur de $F$, de sorte que $E$ (resp. $F$) est canoniquement muni d’une structure de $(A/\mathfrak{J})$-module à droite (resp. à gauche) (II, p. 28). Alors l’homomorphisme canonique (6)
$$
\varphi : E \otimes_A F \to E \otimes_{A/\mathfrak{J}} F
$$
correspondant à l’homomorphisme canonique $\rho : A \to A/\mathfrak{J}$, est l’identité.

En effet, pour tout $\overline{\alpha} \in A/\mathfrak{J}$, tout $x \in E$ et tout $y \in F$, on a $x \overline{\alpha} = x \alpha$ (resp. $\overline{\alpha} y = \alpha y$) pour tout $\alpha$ tel que $\rho(\alpha) = \overline{\alpha}$. Si $C = \mathbf{Z}^{(E \times F)}$, le sous-module de $C$ engendré par les éléments $(x \alpha, y) - (x, \alpha y)$ est donc égal au sous-module engendré par les éléments $(x \overline{\alpha}, y) - (x, \overline{\alpha} y)$.

Les hypothèses et notations étant celles de la prop. 2, soient $E'$ un B-module à droite, $F'$ un B-module à gauche, et considérons deux applications $u : E' \to E$, $v : F' \to F$ semi-linéaires relativement à l’homomorphisme $\rho : B \to A$; $u$ (resp. $v$) peut être considéré comme une application B-linéaire $E' \to \rho_*(E)$ (resp. $F' \to \rho_*(F)$), d’où une application $\mathbf{Z}$-linéaire $w : E' \otimes_B F' \to \rho_*(E) \otimes_B \rho_*(F)$ telle que $w(x' \otimes y') = u(x') \otimes v(y')$ pour $x' \in E', y' \in F'$; en composant avec cette application l’application canonique (6), on obtient donc une application $\mathbf{Z}$-linéaire $w' : E' \otimes_B F' \to E \otimes_A F$ telle que $w'(x' \otimes y') = u(x') \otimes v(y')$ pour x' \in E', y' \in F'; c'est cette application que l'on notera d'ordinaire $u \otimes v$ s'il n'en résulte pas de confusion. Il est clair que $(u, v) \mapsto u \otimes v$ est une application $\mathbf{Z}$-bilinéaire

$$
\operatorname{Hom}_B(E', \rho_*(E)) \times \operatorname{Hom}_B(F', \rho_*(F)) \to \operatorname{Hom}_\mathbf{Z}(E' \otimes_B F', E \otimes_A F).
$$

En outre, si C est un troisième anneau, $\sigma : C \to B$ un homomorphisme, $E''$ un C-module à droite, $F''$ un C-module à gauche, $u' : E'' \to E'$, $v' : F'' \to F'$ des applications semi-linéaires relatives à $\sigma$, on a

$$(u \circ u') \otimes (v \circ v') = (u \otimes v) \circ (u' \otimes v').$$

### 4. Opérateurs sur un produit tensoriel; produits tensoriels comme multimodules

Les hypothèses et notations étant celles du n° 1, pour tout endomorphisme $u$ (resp. $v$) du A-module E (resp. F), $u \otimes 1_F$ (resp. $1_E \otimes v$) est un endomorphisme du $\mathbf{Z}$-module $E \otimes_A F$; il résulte aussitôt de (5) (II, p. 53) que l’application $u \mapsto u \otimes 1_F$ (resp. $v \mapsto 1_E \otimes v$) est un *homomorphisme d’anneaux* $\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ (resp. $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$); en outre, on a

$$(u \otimes 1_F) \circ (1_E \otimes v) = (1_E \otimes v) \circ (u \otimes 1_F) = u \otimes v$$

et par suite (II, p. 33) $E \otimes_A F$ est canoniquement muni d’une structure de *bimodule à gauche* par rapport aux anneaux $\operatorname{End}_A(E)$ et $\operatorname{End}_A(F)$.

Cela étant, supposons données sur E une structure de $((B'_i); A, (C'_j))-multimodule$, et sur F une structure de $(A, (B''_h); (C''_k))-multimodule$ (II, p. 33); il revient au même de dire que l’on s’est donné des homomorphismes d’anneaux $B'_i \to \operatorname{End}_A(E)$, $C'_j^0 \to \operatorname{End}_A(E)$ d’images deux à deux permutables, et des homomorphismes d’anneaux $B''_h \to \operatorname{End}_A(F)$, $C''_k^0 \to \operatorname{End}_A(F)$ d’images deux à deux permutables. Si l’on compose respectivement avec ces homomorphismes les homomorphismes canoniques $\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ et $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ définis plus haut, on voit (compte tenu de (7)) que l’on définit ainsi des homomorphismes d’anneaux

$$
\begin{align*}
B'_i &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C'_j^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F) \\
B''_h &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C''_k^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
\end{align*}
$$

d’images *deux à deux permutables*; autrement dit, on a défini sur $E \otimes_A F$ une structure de $((B'_i), (B''_h); (C'_j), (C''_k))-multimodule$; c’est ce multimodule qu’on appelle encore *produit tensoriel* (relatif à A) *du* $((B'_i); A, (C'_j))-multimodule* E *et du*$(A, (B''_h); (C''_k))-multimodule* F. Ce multimodule est solution d’un problème d’application universelle analogue à celui considéré au n° 1; de façon précise:

#### Proposition 3 {#alg-ii-s3-prop-3 .statement}

*Soit G un* $((B'_i), (B''_h); (C'_j), (C''_k))-multimodule$.

a) *Soit g une application linéaire du multimodule* $E \otimes_A F$ *dans G*. *L’application* $f : (x, y) \mapsto g(x \otimes y)$ *de* $E \times F$ *dans G est* $\mathbf{Z}$*-bilinéaire*, vérifie les relations (1) de II, p. 50, ainsi que les conditions* (8)
$$
\begin{cases}
f(\mu_i' x, y) = \mu_i' f(x, y), & f(x \nu_j', y) = f(x, y) \nu_j' \\
f(x, \mu_h'' y) = \mu_h'' f(x, y), & f(x, y \nu_k'') = f(x, y) \nu_k''
\end{cases}
$$
pour $x \in E, y \in F, \mu_i' \in B_i', \nu_j' \in C_j', \mu_h'' \in B_h'', \nu_k'' \in C_k'', i, j, h, k$ quelconques.

b) Réciproquement, soit $f$ une application $\mathbf{Z}$-bilinéaire de $E \times F$ dans $G$, vérifiant les conditions (1) (II, p. 50) et (8). Il existe alors une application linéaire et une seule $g$ du multimodule $E \otimes_A F$ dans le multimodule $G$ telle que l’on ait $f(x, y) = g(x \otimes y)$ pour $x \in E, y \in F$.

L’assertion a) résulte aussitôt de la définition de la structure de multimodule de $E \otimes_A F$, car on a par exemple $(x \otimes y) \nu_j' = (x \nu_j') \otimes y$. Pour prouver b), remarquons d’abord que la prop. 1 de II, p. 51 donne l’existence et l’unicité d’une application $\mathbf{Z}$-linéaire $g$ telle que $g(x \otimes y) = f(x, y)$ pour $x \in E, y \in F$; tout revient à voir que $g$ est linéaire pour les structures de *multimodule*. Comme les éléments $x \otimes y$ engendrent le $\mathbf{Z}$-module $E \otimes_A F$, il suffit de vérifier les relations $g(\mu_i'(x \otimes y)) = \mu_i' g(x \otimes y)$ et les analogues; mais cela résulte aussitôt de la formule $g(x \otimes y) = f(x, y)$ et des relations (8).

#### Scholie {#alg-ii-s3-n4-sch-1 .statement}

Un élément de $E \otimes_A F$ s’écrit en général de plusieurs manières sous la forme $\sum_i (x_i \otimes y_i)$, où $x_i \in E$ et $y_i \in F$; mais pour définir une application linéaire $g$ du multimodule $E \otimes_A F$ dans un multimodule $G$, il est *inutile* de vérifier que pour $\sum_i (x_i \otimes y_i) = \sum_j (x_j' \otimes y_j')$, on a $\sum_i g(x_i \otimes y_i) = \sum_j g(x_j' \otimes y_j')$; il suffit de se donner $g(x \otimes y)$ pour $x \in E$ et $y \in F$ et de s’assurer que $(x, y) \mapsto g(x \otimes y)$ est $\mathbf{Z}$-bilinéaire et vérifie les conditions (1) (II, p. 50) et (8).

Soient $E'$ un $((B_i'); A, (C_j'))$-multimodule, $F'$ un $(A, (B_h''); (C_k''))$-multimodule, $u : E \to E'$, $v : F \to F'$ des applications linéaires de *multimodules*; il résulte aussitôt des définitions (II, p. 52) que $u \otimes v$ est une application linéaire du multimodule $E \otimes_A F$ dans le multimodule $E' \otimes_A F'$.

Désignant toujours par $E$ un $A$-module à droite, notons ${}_sA_d$ l’anneau $A$ considéré comme $(A, A)$-bimodule (II, p. 34, *Exemple* 1); d’après ce qui précède, le produit tensoriel $E \otimes_A ({}_sA_d)$ est muni canoniquement d’une structure de *A-module à droite* telle que $(x \otimes \lambda)\mu = x \otimes (\lambda \mu)$ pour $x \in E, \lambda \in A, \mu \in A$. L’application $(x, \lambda) \mapsto x \lambda$ de $E \times ({}_sA_d)$ dans $E$ est $\mathbf{Z}$-bilinéaire et vérifie les conditions (1) (II, p. 50) et (8) (où, dans ces dernières, les $B_i', C_j'$ et $B_h''$ sont absents, la famille $(C_k'')$ réduite à $A$); donc (II, p. 54, prop. 3), il existe une application *A-linéaire* $g$ (dite *canonique*) de $E \otimes_A ({}_sA_d)$ dans $E$ telle que $g(x \otimes \lambda) = x \lambda$ pour $x \in E, \lambda \in A$.

#### Proposition 4 {#alg-ii-s3-prop-4 .statement}

Si $E$ est un $A$-module à droite, l’application $h : x \mapsto x \otimes 1$ de $E$ dans $E \otimes_A ({}_sA_d)$ est un isomorphisme de $A$-modules à droite, dont l’isomorphisme réciproque $g$ est tel que $g(x \otimes \lambda) = x \lambda$ pour $x \in E, \lambda \in A$.

En effet, si $g$ est l’application canonique, $g \circ h$ est l’application identique $1_E$ et $h \circ g$ coïncide avec l’application identique de $E \otimes_A ({}_sA_d)$ sur lui-même pour les éléments de la forme $x \otimes \lambda$, qui engendrent ce dernier $\mathbf{Z}$-module; d’où la conclusion.

On écrira d’ordinaire $E \otimes_A A$ au lieu de $E \otimes_A (sA_d)$ et on identifiera souvent $E \otimes_A A$ et $E$ au moyen des isomorphismes canoniques précédents. On observera que si $E$ est en outre muni d’une structure de B-module (à gauche ou à droite) compatible avec sa structure de A-module à droite, $g$ et $h$ sont aussi des isomorphismes pour les structures de B-module de $E$ et de $E \otimes_A A$ (donc des isomorphismes de multimodules).

Soit maintenant $F$ un A-module à gauche; $(sA_d) \otimes_A F$ (aussi noté $A \otimes_A F$) est alors canoniquement muni d’une structure de A-module à gauche, et on définit comme dans la prop. 4 (II, p. 55) un isomorphisme canonique de $A \otimes_A F$ sur $F$ transformant $\lambda \otimes x$ en $\lambda x$, et son isomorphisme réciproque $x \mapsto 1 \otimes x$.

En particulier il existe un isomorphisme canonique du (A, A)-bimodule $(sA_d) \otimes_A (sA_d)$ sur $sA_d$, qui transforme $\lambda \otimes \mu$ en $\lambda \mu$.

### 5. Produit tensoriel de deux modules sur un anneau commutatif

Soit C un anneau *commutatif*; pour tout C-module E, la structure de module sur E est *compatible avec elle-même* (II, p. 33). Si E et F sont deux C-modules, les considérations de II, p. 54 permettent donc de définir sur le produit tensoriel $E \otimes_C F$ *deux* structures de C-module, respectivement telles que $\gamma(x \otimes y) = (\gamma x) \otimes y$ et $\gamma(x \otimes y) = x \otimes (\gamma y)$; mais comme en vertu de II, p. 51, déf. 1 on a ici $(\gamma x) \otimes y = x \otimes (\gamma y)$, ces deux structures sont *les mêmes*. Quand on parlera désormais de $E \otimes_C F$ comme d’un C-*module*, c’est de la structure ainsi définie qu’il sera question, sauf mention expresse du contraire. L’isomorphisme canonique $\sigma : F \otimes_C E \to E \otimes_C F$ (II, p. 52, cor. 2) est alors un isomorphisme de C-modules.

Il résulte de cette définition que si $(a_\lambda)_{\lambda \in \mathbf{L}}$ (resp. $(b_\mu)_{\mu \in \mathbf{M}}$) est un *système générateur* du C-module E (resp. F), $(a_\lambda \otimes b_\mu)$ est un *système générateur* du C-module $E \otimes_C F$; en particulier, si E et F sont des C-modules *de type fini*, il en est de même de $E \otimes_C F$.

Pour tout C-module G, les applications $\mathbf{Z}$-bilinéaires $f$ de $E \times F$ dans G pour lesquelles on a
$$
f(\gamma x, y) = f(x, \gamma y) = \gamma f(x, y) \quad \text{pour } x \in E, y \in F, \gamma \in C
$$
sont alors appelées C-*bilinéaires*, et forment un C-*module* que l’on note $\mathcal{L}_2(E, F; G)$; la prop. 3 (II, p. 54) définit un *isomorphisme canonique de C-modules* (cf. II, p. 35, *Remarque* 1)
$$
\mathcal{L}_2(E, F; G) \to \mathrm{Hom}_C(E \otimes_C F, G).
$$
Soient $E', F'$ deux C-modules, $u : E \to E'$, $v : F \to F'$ deux applications C-linéaires; alors (II, p. 55) $u \otimes v$ est une application C-*linéaire* de $E \otimes_C F$ dans $E' \otimes_C F'$. En outre, il est immédiat que $(u, v) \mapsto u \otimes v$ est une application C-bilinéaire de $\mathrm{Hom}_C(E, E') \times \mathrm{Hom}_C(F, F')$ dans $\mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')$; il lui correspond donc canoniquement une application C-linéaire, dite canonique:

(11) $$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F') \to \mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')
$$

qui, à tout élément $u \otimes v$ du produit tensoriel

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F')
$$

fait correspondre l’application linéaire $u \otimes v$. On notera que l’application canonique (11) *n’est pas nécessairement injective ni surjective* (II, p. 190, exerc. 2).

#### Remarque 1 {#alg-ii-s3-n5-rem-1 .statement}

Soient A, B deux anneaux *commutatifs*, $\rho : B \to A$ un homomorphisme d’anneaux, E et F deux A-modules; alors l’application canonique (6) de II, p. 53 est une application B-linéaire

(12) $$
\rho_*(E) \otimes_B \rho_*(F) \to \rho_*(E \otimes_A F).
$$

#### Remarque 2 {#alg-ii-s3-n5-rem-2 .statement}

Les considérations de ce n° peuvent se généraliser au cas suivant: soient E un A-module à droite, F un A-module à gauche, C un anneau commutatif, $\rho : C \to A$ un homomorphisme de C dans A tel que $\rho(C)$ soit contenu dans le *centre* de A (cf. III, p. 6). On peut alors considérer les C-modules $\rho_*(E)$ et $\rho_*(F)$ et l’hypothèse sur $\rho$ entraîne que les structures de ces C-modules sont respectivement compatibles avec les structures de A-module de E et F (II, p. 33). Le produit tensoriel $E \otimes_A F$ est donc (en vertu de II, p. 54) muni de deux structures de C-modules telles que $\gamma(x \otimes y) = (x \rho(\gamma)) \otimes y$ et $\gamma(x \otimes y) = x \otimes (\rho(\gamma)y)$ respectivement pour $\gamma \in C, x \in E, y \in F$, et la déf. 1 (II, p. 51) montre encore que ces deux structures sont *identiques*. Si $E'$ (resp. $F'$) est un A-module à droite (resp. à gauche), $u : E \to E', v : F \to F'$ deux applications A-linéaires, alors $u \otimes v : E \otimes_A F \to E' \otimes_A F'$ est C-linéaire pour les structures de C-modules qu’on vient de définir; l’application $(u, v) \mapsto u \otimes v$:

$$
\mathrm{Hom}_A(E, E') \times \mathrm{Hom}_A(F, F') \to \mathrm{Hom}_C(E \otimes_A F, E' \otimes_A F')
$$

est C-*bilinéaire* (pour les structures de C-module sur $\mathrm{Hom}_A(E, E')$ et $\mathrm{Hom}_A(F, F')$ définies dans II, p. 35, *Remarque* 1) d’où l’on déduit encore une application C-linéaire, dite *canonique*

(13) $$
\mathrm{Hom}_A(E, E') \otimes_C \mathrm{Hom}_A(F, F') \to \mathrm{Hom}_C(E \otimes_A F, E' \otimes_A F').
$$

#### Remarque 3 {#alg-ii-s3-n5-rem-3 .statement}

Soient A un anneau intègre, K son corps des fractions. Si E et F sont deux K-espaces vectoriels, l’application canonique

$$
(E_{[A]}) \otimes_A (F_{[A]}) \to E \otimes_K F
$$

(II, p. 53 et p. 30) est *bijective*. Il suffit en effet (II, p. 55) de prouver que si $f$ est une application A-*bilinéaire* de $E \times F$ dans un K-espace vectoriel G, $f$ est aussi K-*bilinéaire*. Or, pour tout $\alpha \neq 0$ dans A, on a alors d’où
$$
\alpha f(\alpha^{-1}x, y) = f(x, y) = \alpha f(x, \alpha^{-1}y),
$$
puisque G est un K-espace vectoriel.

### 6. Propriétés de $E \otimes_A F$ relatives aux suites exactes

#### Proposition 5 {#alg-ii-s3-prop-5 .statement}

Soient $E, E', E''$ des $A$-modules à droite, F un $A$-module à gauche,

(14)
$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
une suite exacte d’applications linéaires. Si l’on pose $\bar{u} = u \otimes 1_F, \bar{v} = v \otimes 1_F$, la suite

(15)
$$
E' \otimes_A F \xrightarrow{\bar{u}} E \otimes_A F \xrightarrow{\bar{v}} E'' \otimes_A F \longrightarrow 0
$$
de $\mathbf{Z}$-homomorphismes est exacte.

En vertu de II, p. 53, formule (5), on a $\bar{v} \circ \bar{u} = (v \circ u) \otimes 1_F = 0$; l’image $H = \bar{u}(E' \otimes F)$ est contenue dans le noyau $L = \mathrm{Ker}(\bar{v})$; par passage au quotient, on déduit donc de $\bar{v}$ une application $\mathbf{Z}$-linéaire $f$ du conoyau $M = (E \otimes F)/H$ de $\bar{u}$ dans $E'' \otimes F$; il s’agit de prouver que $f$ est bijective, et il suffira donc de définir une application $\mathbf{Z}$-linéaire $g : E'' \otimes F \to M$ telle que $g \circ f$ et $f \circ g$ soient les applications identiques.

Soient $x'' \in E'', y \in F$; par hypothèse il existe $x \in E$ tel que $v(x) = x''$. Montrons que si $x_1, x_2$ sont deux éléments de $E$ tels que $v(x_1) = v(x_2) = x''$ et si $\varphi : E \otimes F \to M$ est l’application canonique, on a $\varphi(x_1 \otimes y) = \varphi(x_2 \otimes y)$. Il suffit de prouver que si $v(x) = 0$, on a $\varphi(x \otimes y) = 0$; cela résulte de ce que $x = u(x')$, avec $x' \in E'$, d’où $x \otimes y = u(x') \otimes y = \bar{u}(x' \otimes y) \in H$. Si à $(x'', y)$ on fait correspondre la valeur unique de $\varphi(x \otimes y)$ pour tous les $x \in E$ tels que $v(x) = x''$, on définit une application de $E'' \times F$ dans $M$; cette application est $\mathbf{Z}$-bilinéaire et vérifie les conditions (1) (II, p. 50), puisque $v(x\lambda) = x''\lambda$ et $(x\lambda) \otimes y = x \otimes (\lambda y)$ pour $x \in E$; il existe donc une application $\mathbf{Z}$-linéaire $g$ de $E'' \otimes F$ dans $M$ telle que $g(x'' \otimes y) = \varphi(x \otimes y)$, pour $y \in F, x \in E$ et $x'' = v(x)$. Cette définition prouve en outre que $f \circ g$ coïncide avec l’application identique pour les éléments de $E'' \otimes F$ de la forme $x'' \otimes y$, donc $f \circ g$ est l’application identique de $E'' \otimes F$; d’autre part, pour $x \in E$ et $y \in F$, on a $f(\varphi(x \otimes y)) = v(x) \otimes y$ par définition, donc $g(f(\varphi(x \otimes y))) = \varphi(x \otimes y)$, et comme les éléments de la forme $\varphi(x \otimes y)$ engendrent $M$, $g \circ f$ est l’application identique de $M$.

#### Corollaire {#alg-ii-s3-n6-cor-1 .statement}

Soient $F, F', F''$ des $A$-modules à gauche, $E$ un $A$-module à droite,

(16)
$$
F' \xrightarrow{s} F \xrightarrow{t} F'' \longrightarrow 0
$$
une suite exacte d’applications linéaires. Si on pose $\bar{s} = 1_E \otimes s, \bar{t} = 1_E \otimes t$, la suite de $\mathbf{Z}$-homomorphismes

(17) $E \otimes_A F' \xrightarrow{\bar{s}} E \otimes_A F \xrightarrow{i} E \otimes_A F'' \longrightarrow 0$

est exacte.

En effet, quand on considère $E$ (resp. $F$) comme un $A^0$-module à gauche (resp. à droite), $F \otimes_{A^0} E$ s’identifie à $E \otimes_A F$, et on a des identifications analogues pour $F' \otimes_{A^0} E$ et $F'' \otimes_{A^0} E$ (II, p. 52, cor. 2); le corollaire résulte donc aussitôt de la prop. 5.

#### Remarque {#alg-ii-s3-n6-rem-1 .statement}

On notera qu’en général, si $E'$ est un sous-module d’un $A$-module à droite $E$, $j : E' \to E$ l’injection canonique, l’application $j \otimes 1_F : E' \otimes F \to E \otimes F$ n’est pas nécessairement injective. Autrement dit, d’une suite exacte

(18) $0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0$

on ne peut pas conclure en général que la suite

(19) $0 \longrightarrow E' \otimes F \xrightarrow{\bar{u}} E \otimes F \xrightarrow{\bar{v}} E'' \otimes F \longrightarrow 0$

soit exacte.

Prenons par exemple $A = \mathbf{Z}$, $E = \mathbf{Z}$, $E' = 2\mathbf{Z}$, $F = \mathbf{Z}/2\mathbf{Z}$. Comme $E'$ est isomorphe à $E$, $E' \otimes F$ est isomorphe à $E \otimes F$, lui-même isomorphe à $F$ (II, p. 55, prop. 4). Mais pour tout $x' = 2x \in E'$ (où $x \in E$), et tout $y \in F$, on a $j(x') \otimes y = (2x) \otimes y = x \otimes (2y) = 0$ puisque $2y = 0$, et l’image canonique de $E' \otimes F$ dans $E \otimes F$ est réduite à 0.

En d’autres termes, il faut soigneusement distinguer, pour un sous-module $E'$ de $E$ et un élément $x \in E'$, entre l’élément $x \otimes y$ « calculé dans $E' \otimes F$ » et l’élément $x \otimes y$ « calculé dans $E \otimes F$ » (autrement dit, l’élément $j(x) \otimes y$).

Nous étudierons plus tard, sous le nom de modules plats, les modules $F$ tels que la suite (19) soit exacte pour toute suite exacte (18) (AC, I, § 2).

#### Proposition 6 {#alg-ii-s3-prop-6 .statement}

Si on a les deux suites exactes (14) et (16) (II, p. 58), l’homomorphisme $v \otimes t : E \otimes_A F \to E'' \otimes_A F''$ est surjectif et son noyau est égal à

$$ \operatorname{Im}(u \otimes 1_F) + \operatorname{Im}(1_E \otimes s). $$

En effet, on a $v \otimes t = (v \otimes 1_{F''}) \circ (1_E \otimes t)$ (II, p. 53, formule (5)), et $v \otimes t$ est donc surjectif, étant composé de deux homomorphismes surjectifs en vertu de la prop. 5 (II, p. 58) et de son corollaire (II, p. 58). D’autre part, pour que $z \in E \otimes F$ soit dans le noyau de $v \otimes t$, il faut et il suffit que $(1_E \otimes t)(z)$ appartienne au noyau de $v \otimes 1_{F''}$, c’est-à-dire, en vertu de (15) (II, p. 58), à l’image de $u \otimes 1_{F''} : E' \otimes F'' \to E \otimes F''$. Mais comme l’homomorphisme $t : F \to F''$ est surjectif, il en est de même de $1_{E'} \otimes t : E' \otimes F \to E' \otimes F''$, en vertu de II, p. 58, corollaire, donc la condition pour $z$ se réduit à l’existence d’un $a \in E' \otimes F$ tel que

$$ (1_E \otimes t)(z) = (u \otimes t)(a). $$

Posons $b = z - (u \otimes 1_F)(a)$; on aura alors $(1_E \otimes t)(b) = 0$, et en vertu de (17), $b$ appartient à l’image de $1_E \otimes s$, ce qui démontre la proposition.

Autrement dit:
COROLLAIRE 1. — Soient E' un sous-module d’un A-module à droite E, F' un sous-module d’un A-module à gauche F, Im(E' \otimes_A F) et Im(E \otimes_A F') les sous-\mathbf{Z}-modules de E \otimes_A F, images respectives des applications canoniques E' \otimes_A F \to E \otimes_A F, E \otimes_A F' \to E \otimes_A F. On a alors un isomorphisme canonique de \mathbf{Z}-modules
(20) $\pi : (E/E') \otimes_A (F/F') \to (E \otimes_A F)/(Im(E' \otimes_A F) + Im(E \otimes_A F'))$
tel que pour $\xi \in E/E', \eta \in F/F', \pi(\xi \otimes \eta)$ soit la classe de tout élément $x \otimes y \in E \otimes_A F$ tel que $x \in \xi$ et $y \in \eta$.

On notera que lorsque E est un ((B'_i); A, (C'_j))-multimodule, F un (A, (B''_h); (C''_k))-multimodule, E' et F' des sous-multimodules de E et F respectivement, l’isomorphisme (20) est un isomorphisme pour les structures de ((B'_i), (B''_h); (C'_j), (C''_k))-multimodules des deux membres (II, p. 54).

#### Corollaire 2 {#alg-ii-s3-prop-6-cor-2 .statement}

Soient a un idéal à droite de A, F un A-module à gauche, aF le sous-\mathbf{Z}-module de F engendré par les éléments de la forme $\lambda x$, où $\lambda \in a$ et $x \in F$. On a alors un isomorphisme canonique de \mathbf{Z}-modules
(21) $\pi : (A/a) \otimes_A F \to F/aF$
tel que pour tout $\bar{\lambda} \in A/a$ et tout $x \in F$, $\pi(\bar{\lambda} \otimes x)$ soit la classe mod. aF de $\lambda x$, ou $\lambda \in \bar{\lambda}$.

En particulier, pour A = \mathbf{Z}, on voit que pour tout entier n et tout \mathbf{Z}-module F, (\mathbf{Z}/n\mathbf{Z}) \otimes_{\mathbf{Z}} F s’identifie canoniquement au \mathbf{Z}-module quotient F/nF.

#### Corollaire 3 {#alg-ii-s3-prop-6-cor-3 .statement}

Soient A un anneau commutatif, a un idéal de A, E et F deux A-modules, tels que a soit contenu dans l’annulateur de F. Alors les (A/a)-modules E \otimes_A F et (E/aE) \otimes_{A/a} F sont canoniquement isomorphes.

En effet, F et E \otimes_A F étant annulés par a, sont canoniquement munis de structures de (A/a)-modules (II, p. 28), et si on pose E' = aE, on a Im(E' \otimes_A F) = 0; on a donc un isomorphisme canonique (20) de E \otimes_A F sur (E/aE) \otimes_A F, et ce dernier est lui-même identique à (E/aE) \otimes_{A/a} F (II, p. 35, corollaire).

#### Corollaire 4 {#alg-ii-s3-prop-6-cor-4 .statement}

Soient a, b deux idéaux dans un anneau commutatif C; le C-module (C/a) \otimes_C (C/b) est alors canoniquement isomorphe à C/(a + b).

### 7. Produits tensoriels de produits et de sommes directes

Soient (E_\lambda)_{\lambda \in L} une famille de A-modules à droite, (F_\mu)_{\mu \in M} une famille de A-modules à gauche, et considérons les modules produits C = \prod_{\lambda \in L} E_\lambda, D = \prod_{\mu \in M} F_\mu. L’application ((x_\lambda), (y_\mu)) \mapsto (x_\lambda \otimes y_\mu) de C \times D dans le \mathbf{Z}-module produit \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu) est \mathbf{Z}-bilinéaire et satisfait aux conditions (1) (II, p. 50) de façon évidente. Il existe donc (II, p. 51, prop. 1) une application $\mathbf{Z}$-linéaire, dite *canonique*

$$
f : (\prod_{\lambda \in L} E_\lambda) \otimes_A (\prod_{\mu \in M} F_\mu) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

telle que l’on ait $f((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu)$.

Lorsque $C = R^L, D = S^M, R$ (resp. $S$) étant un $A$-module à droite (resp. à gauche), l’application canonique (22) fait correspondre à tout produit tensoriel $u \otimes v$, où $u$ est une application de $L$ dans $R$ et $v$ une application de $M$ dans $S$, l’application $(\lambda, \mu) \mapsto u(\lambda) \otimes v(\mu)$ de $L \times M$ dans $R \otimes_A S$; même dans ce cas l’application canonique (22) n’est en général *ni injective ni surjective* (II, p. 189, exerc. 3; cf. II, p. 63, cor. 3).

Lorsque les $E_\lambda$ sont des $((B'_i); A, (C'_j))$-multimodules et les $F_\mu$ des $(A, (B''_h); (C''_k))$-multimodules, l’homomorphisme (22) est aussi un homomorphisme pour les structures de $((B'_i), (B''_h); (C'_j), (C''_k))$-multimodules des deux membres.

Considérons maintenant le sous-module $E = \bigoplus_{\lambda \in L} E_\lambda$ (resp. $F = \bigoplus_{\mu \in M} F_\mu$) de $C$ (resp. $D$); les injections canoniques $E \to C, F \to D$ définissent canoniquement une application $\mathbf{Z}$-linéaire $E \otimes_A F \to C \otimes_A D$ qui, composée avec l’application (22), donne une application $\mathbf{Z}$-linéaire $g$ de $E \otimes_A F$ dans $\prod_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)$ telle que $g((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu)$; en outre, comme les familles $(x_\lambda)$ et $(y_\mu)$ ont un support fini, il en est de même de $(x_\lambda \otimes y_\mu)$, donc $g$ est finalement un homomorphisme canonique

$$
g : (\bigoplus_{\lambda \in L} E_\lambda) \otimes_A (\bigoplus_{\mu \in M} F_\mu) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu),
$$

qui est un homomorphisme de multimodules sous les mêmes conditions que (22).

#### Proposition 7 {#alg-ii-s3-prop-7 .statement}

*L’application canonique (23) est bijective.*

Il suffit pour cela de définir une application $\mathbf{Z}$-linéaire $h$ de la somme directe $G = \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)$ dans $E \otimes_A F$ telle que $g \circ h$ et $h \circ g$ soient les applications identiques. Or, pour définir une application $\mathbf{Z}$-linéaire de $G$ dans $E \otimes_A F$, il suffit (II, p. 12, prop. 6), de définir une application $\mathbf{Z}$-linéaire

$$
h_{\lambda \mu} : E_\lambda \otimes_A F_\mu \to E \otimes_A F
$$

pour tout couple $(\lambda, \mu)$, et on prendra $h_{\lambda \mu} = i_\lambda \otimes j_\mu$, où $i_\lambda : E_\lambda \to E$ et $j_\mu : F_\mu \to F$ sont les injections canoniques. Il est clair alors que $h \circ g$ coïncide avec l’application identique pour les éléments de la forme $(\sum x_\lambda) \otimes (\sum y_\mu)$, qui engendrent le $\mathbf{Z}$-module $E \otimes_A F$; de même $g \circ h$ coïncide avec l’application identique pour les éléments de la forme $\sum_{\lambda, \mu} (x_\lambda \otimes y_\mu)$, qui engendrent le $\mathbf{Z}$-module $G$, puisque pour chaque couple $(\lambda, \mu)$ les produits $x_\lambda \otimes y_\mu$ ($x_\lambda \in E_\lambda, y_\mu \in F_\mu$) engendrent le $\mathbf{Z}$-module $E_\lambda \otimes_A F_\mu$. D’où la proposition.

Soient $u_\lambda : E_\lambda \to E'_\lambda, v_\mu : F_\mu \to F'_\mu$ des A-homomorphismes; il est clair que le diagramme

$$
\begin{array}{ccc}
(\bigoplus_\lambda E_\lambda) \otimes_A (\bigoplus_\mu F_\mu) & \longrightarrow & \bigoplus_{\lambda,\mu} (E_\lambda \otimes_A F_\mu) \\
(\bigoplus_\lambda u_\lambda) \otimes (\bigoplus_\mu v_\mu) \downarrow & & \downarrow (\bigoplus_\lambda u_\lambda \otimes v_\mu) \\
(\bigoplus_\lambda E'_\lambda) \otimes_A (\bigoplus_\mu F'_\mu) & \longrightarrow & \bigoplus_{\lambda,\mu} (E'_\lambda \otimes_A F'_\mu)
\end{array}
$$

est commutatif.

#### Corollaire 1 {#alg-ii-s3-prop-7-cor-1 .statement}

*Si le A-module à gauche F admet une base $(b_\mu)_{\mu \in M}$, tout élément de $E \otimes_A F$ s’écrit d’une seule manière sous la forme $\sum_\mu (x_\mu \otimes b_\mu)$, où $x_\mu \in E$ et la famille $(x_\mu)$ a un support fini. Le $\mathbf{Z}$-module $E \otimes_A F$ est isomorphe à $E^{(M)}$ considéré comme $\mathbf{Z}$-module.*

En effet, la base $(b_\mu)$ définit un isomorphisme de F sur $\bigoplus_{\mu \in M} Ab_\mu$, d’où un isomorphisme $E \otimes_A F \to \bigoplus_{\mu \in M} (E \otimes_A Ab_\mu)$ en vertu de la prop. 7; comme $\xi \mapsto \xi b_\mu$ est un isomorphisme de $A_s$ sur $Ab_\mu$, $x \mapsto x \otimes b_\mu$ est un isomorphisme de E sur $E \otimes_A (Ab_\mu)$ en vertu de la prop. 4 de II, p. 55, d’où le corollaire.

Si E est un $((B_i'); A, (C_j'))$-multimodule, l’isomorphisme canonique $E \otimes_A F \to E^{(M)}$ est un isomorphisme de $((B_i'); (C_j'))$-multimodules.

En particulier, si en outre E admet aussi une base $(a_\lambda)_{\lambda \in L}$, tout $z \in E \otimes_A F$ s’écrit d’une manière et d’une seule sous la forme $\sum_{\lambda, \mu} (a_\lambda \xi_{\lambda \mu}) \otimes b_\mu$, où les $\xi_{\lambda \mu}$ appartiennent à A (et forment une famille à support fini); l’application $z \mapsto (\xi_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$ est un isomorphisme de $E \otimes_A F$ sur $A^{(L \times M)}$ pour les structures de $\mathbf{Z}$-module (et même les structures de module sur le *centre* de A). Plus particulièrement:

#### Corollaire 2 {#alg-ii-s3-prop-7-cor-2 .statement}

*Si E et F sont deux modules libres sur un anneau commutatif C, et si $(a_\lambda)$ (resp. $(b_\mu)$) est une base du C-module E (resp. F), alors $(a_\lambda \otimes b_\mu)$ est une base du C-module $E \otimes_C F$.

Par abus de langage, on dit parfois que la base $(a_\lambda \otimes b_\mu)$ est le *produit tensoriel* des bases $(a_\lambda)$ et $(b_\mu)$.

*Remarque 1).* — Soient E un A-module à droite libre, F un A-module à gauche libre, $(a_\lambda)_{\lambda \in L}$ une base de E, $(b_\mu)_{\mu \in M}$ une base de F. Tout élément $z \in E \otimes_A F$ s’écrit d’une seule manière $\sum_\lambda a_\lambda \otimes y_\lambda$, où $y_\lambda \in F$, et aussi d’une seule manière $\sum_\mu x_\mu \otimes b_\mu$, où $x_\mu \in E$. Si on pose $y_\lambda = \sum_\mu \eta_{\lambda \mu} b_\mu$, $x_\mu = \sum_\lambda a_\lambda \xi_{\lambda \mu}$, où les $\xi_{\lambda \mu}$ et $\eta_{\lambda \mu}$ appartiennent à A, on a $\xi_{\lambda \mu} = \eta_{\lambda \mu}$ pour tout $(\lambda, \mu)$, car $\sum_\lambda (a_\lambda \otimes (\sum_\mu \eta_{\lambda \mu} b_\mu)) = \sum_{\lambda, \mu} ((a_\lambda \eta_{\lambda \mu}) \otimes b_\mu) = \sum_\mu ((\sum_\lambda a_\lambda \eta_{\lambda \mu}) \otimes b_\mu)$.

#### Corollaire 3 {#alg-ii-s3-prop-7-cor-3 .statement}

Soient $(E_\lambda)_{\lambda \in L}$ une famille de $A$-modules à droite, $F$ un $A$-module à gauche libre (resp. libre et de type fini). Alors l’application canonique (22)

$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F \to \prod_{\lambda \in L} (E_\lambda \otimes_A F)
$$

est injective (resp. bijective).

En effet, si $(b_\mu)$ est une base de $F$, tout élément de $\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F$ peut s’écrire d’une seule manière $z = \sum_\mu ((x_\lambda^{(\mu)}) \otimes b_\mu)$ (II, p. 62, cor. 1); dire que son image canonique est nulle signifie que pour tout $\lambda \in L$, on a $\sum_\mu (x_\lambda^{(\mu)} \otimes b_\mu) = 0$, donc $x_\lambda^{(\mu)} = 0$ pour tout $\lambda \in L$ et tout $\mu$ (II, p. 62, cor. 1), et par suite $z = 0$.

Pour démontrer que l’application canonique est bijective lorsque $F$ admet une base finie, on est aussitôt ramené, en vertu de la prop. 7, au cas où $F = A_s$; mais alors les deux membres s’identifient canoniquement à $\prod_{\lambda \in L} E_\lambda$ (II, p. 55, prop. 4) et après ces identifications, l’application canonique (22) devient l’identité.

#### Corollaire 4 {#alg-ii-s3-prop-7-cor-4 .statement}

Soient $A$ un anneau sans diviseur de zéro, $E$ un $A$-module à droite libre, $F$ un $A$-module à gauche libre. Alors la relation $x \otimes y = 0$ dans $E \otimes_A F$ entraîne $x = 0$ ou $y = 0$.

En effet, soient $(a_\lambda)$ une base de $E$, $(b_\mu)$ une base de $F$, et soient $x = \sum_\lambda a_\lambda \xi_\lambda$, $y = \sum_\mu \eta_\mu b_\mu$; on a $x \otimes y = \sum_{\lambda, \mu} ((a_\lambda \xi_\lambda \eta_\mu) \otimes b_\mu)$ et la relation $x \otimes y = 0$ entraîne $\xi_\lambda \eta_\mu = 0$ pour tout couple d’indices $(\lambda, \mu)$ (II, p. 62, cor. 1). Donc, si l’on a $x \neq 0$, c’est-à-dire $\xi_\lambda \neq 0$ pour un $\lambda$ au moins, on en conclut $\eta_\mu = 0$ pour tout $\mu$, d’où $y = 0$.

#### Corollaire 5 {#alg-ii-s3-prop-7-cor-5 .statement}

Soient $E$ un $A$-module à droite, $F$ un $A$-module à gauche, $M$ un sous-module de $E$, $N$ un sous-module de $F$. Si $M$ est facteur direct de $E$ et $N$ facteur direct de $F$, l’homomorphisme canonique $M \otimes_A N \to E \otimes_A F$ est injectif, et l’image de $M \otimes_A N$ par cet homomorphisme est facteur direct du $\mathbf{Z}$-module $E \otimes_A F$.

Cela résulte aussitôt de la prop. 7.

On notera que si $E$ est un $((B'_i); A, (C'_j))$-multimodule et $F$ un $(A, (B''_h); (C''_k))$-multimodule, $M$ et $N$ des facteurs directs dans ces multimodules, $M \otimes N$ est facteur direct du $((B'_i), (B''_h); (C'_j), (C''_k))$-multimodule $E \otimes F$.

#### Corollaire 6 {#alg-ii-s3-prop-7-cor-6 .statement}

Soient $P$ un $A$-module à gauche projectif, $E, F$ deux $A$-modules à droite. Pour tout homomorphisme injectif $u : E \to F$, l’homomorphisme

$$
u \otimes 1_P : E \otimes_A P \to F \otimes_A P
$$

est injectif.

En effet, il existe un $A$-module à gauche $Q$ tel que $L = P \oplus Q$ soit libre (II, p. 39, prop. 4), et $u \otimes 1_L$ s’identifie (prop. 7) à $(u \otimes 1_P) \oplus (u \otimes 1_Q)$;

il suffit donc de prouver le corollaire lorsque P est libre (II, p. 14, cor. 1). Le même raisonnement ramène au cas où $P = A_s$, qui découle aussitôt de II, p. 55, prop. 4.

#### Corollaire 7 {#alg-ii-s3-prop-7-cor-7 .statement}

*Soit C un anneau commutatif. Si E et F sont deux C-modules projectifs, $E \otimes_C F$ est un C-module projectif.*

Cela résulte aussitôt de II, p. 63, cor. 5 et du fait que le produit tensoriel de deux C-modules libres est un C-module libre (II, p. 61, cor. 2).

*Remarque 2).* — Sous les hypothèses de la prop. 7 (II, p. 61), soient $E'_\lambda$ un sous-module de $E_\lambda$, $F'_{\mu}$ un sous-module de $F_\mu$, et posons $E' = \bigoplus_{\lambda \in L} E'_\lambda$, $F' = \bigoplus_{\mu \in M} F'_{\mu}$. Désignons par $\operatorname{Im}(E' \otimes_A F')$ (resp. $\operatorname{Im}(E'_\lambda \otimes_A F'_{\mu})$) l’image de $E' \otimes_A F'$ (resp. $E'_\lambda \otimes_A F'_{\mu}$) dans $E \otimes_A F$ (resp. $E_\lambda \otimes_A F_\mu$) par l’application canonique; alors l’isomorphisme (23) identifie les sous-$\mathbf{Z}$-modules

$$
\operatorname{Im}(E' \otimes_A F') \quad \text{et} \quad \bigoplus_{(\lambda, \mu) \in L \times M} \operatorname{Im}(E'_\lambda \otimes_A F'_{\mu});
$$

cela résulte aussitôt de la commutativité du diagramme

$$
\begin{array}{ccc}
(\bigoplus_{\lambda} E'_\lambda) \otimes_A (\bigoplus_{\mu} F'_{\mu}) & \longrightarrow & (\bigoplus_{\lambda} E_\lambda) \otimes_A (\bigoplus_{\mu} F_\mu) \\
\downarrow & & \downarrow \\
\bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_{\mu}) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)
\end{array}
$$

où les flèches verticales sont les isomorphismes canoniques.

### 8. Associativité du produit tensoriel.

#### Proposition 8 {#alg-ii-s3-prop-8 .statement}

*Soient A, B deux anneaux, E un A-module à droite, F un (A, B)-bimodule, G un B-module à gauche. Alors $E \otimes_A F$ est un B-module à droite, $F \otimes_B G$ un A-module à gauche, et il existe une application $\mathbf{Z}$-linéaire et une seule*

$$
\varphi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

*telle que* $\varphi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$ *pour* $x \in E, y \in F, z \in G$; *en outre cette application* $\mathbf{Z}$-*linéaire est bijective* (*« associativité » du produit tensoriel*).

Les structures de B-module à droite sur $E \otimes_A F$ et de A-module à gauche sur $F \otimes_B G$ ont été définies dans II, p. 54. L’unicité de $\varphi$ est évidente puisque les éléments $(x \otimes y) \otimes z$ engendrent le $\mathbf{Z}$-module $(E \otimes_A F) \otimes_B G$. Pour démontrer l’existence de $\varphi$, remarquons que pour tout $z \in G$, $h_z : y \mapsto y \otimes z$ est une application A-linéaire du A-module à gauche F dans le A-module à gauche $F \otimes_B G$. Posons $g_z = 1_E \otimes h_z$, qui est donc une application $\mathbf{Z}$-linéaire de $E \otimes_A F$ dans $E \otimes_A (F \otimes_B G)$, et considérons l’application $(t, z) \mapsto g_z(t)$ de $(E \otimes_A F) \times G$ dans $E \otimes_A (F \otimes_B G)$; comme $h_{z+z'} = h_z + h_{z'}$ pour $z \in G, z' \in G$, il est immédiat que l’application précédente est $\mathbf{Z}$-bilinéaire. En outre, montrons que pour tout $\mu \in B$, on a $g_{\mu z}(t) = g_z(t\mu)$; il suffit évidemment de le faire pour $t = x \otimes y$, où $x \in E$ et $y \in F$; or on a $g_{\mu z}(x \otimes y) = x \otimes (y \otimes \mu z)$ et $g_z((x \otimes y)\mu) = g_z(x \otimes y\mu) = x \otimes (y\mu \otimes z)$. La prop. 1 (II, p. 51) prouve donc l’existence d’une application $\mathbf{Z}$-linéaire

$$
\varphi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

telle que $\varphi(t \otimes z) = g_z(t)$, donc $\varphi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$. On définit de la même façon une application $\mathbf{Z}$-linéaire

$$
\psi : E \otimes_A (F \otimes_B G) \to (E \otimes_A F) \otimes_B G
$$

telle que $\psi(x \otimes (y \otimes z)) = (x \otimes y) \otimes z$, et il est clair que $\psi \circ \varphi$ et $\varphi \circ \psi$ sont les applications identiques de $(E \otimes_A F) \otimes_B G$ et $E \otimes_A (F \otimes_B G)$ respectivement, puisqu’elles se réduisent à l’identité sur des systèmes générateurs de ces $\mathbf{Z}$-modules.

Il est immédiat que si $E$ est un $((C'_i); A, (D'_j))$-multimodule, $F$ un $(A, (C''_h)); B, (D''_k))$-multimodule, $G$ un $(B, (C'''_l)); (D'''_m))$-multimodule, l’isomorphisme canonique défini dans la prop. 8 (II, p. 64) est un isomorphisme de $((C'_i), (C''_h), (C'''_l)); (D'_j), (D''_k), (D'''_m))$-multimodules. En particulier, si $C$ est un anneau *commutatif*, $E, F, G$ trois $C$-modules, on a un isomorphisme canonique de $C$-modules

$$
(E \otimes_C F) \otimes_C G \to E \otimes_C (F \otimes_C G).
$$

Nous allons voir ci-dessous que l’on peut, sous certaines conditions, généraliser la définition du produit tensoriel à une famille de multimodules, ce qui en particulier nous fournira, sous les hypothèses de la prop. 8 (II, p. 64), un $\mathbf{Z}$-module $E \otimes_A F \otimes_B G$, canoniquement isomorphe à chacun des $\mathbf{Z}$-modules $(E \otimes_A F) \otimes_B G$ et $E \otimes_A (F \otimes_B G)$, et auquel on identifiera ces derniers.

### 9. Produit tensoriel de familles de multimodules

Soit $(G_\lambda)_{\lambda \in L}$ une famille de $\mathbf{Z}\text{-modules}$; on dit qu’une application $u$ de l’ensemble $G = \prod_{\lambda \in L} G_\lambda$ dans un $\mathbf{Z}$-module est *multiadditive* (ou $\mathbf{Z}$-*multilinéaire*) si $(x_\lambda) \mapsto u((x_\lambda))$ est additive par rapport à chacune des variables $x_\lambda$: de façon précise, cela signifie que pour tout $\mu \in L$ et tout élément $(a_\lambda) \in \prod_{\lambda \neq \mu} G_\lambda$, on a, en identifiant canoniquement $G$ à $G_\mu \times \prod_{\lambda \neq \mu} G_\lambda$

$$
u(x_\mu + y_\mu, (a_\lambda)) = u(x_\mu, (a_\lambda)) + u(y_\mu, (a_\lambda)) \quad \text{pour } x_\mu, y_\mu \text{ dans } G_\mu.
$$

(24)

Cela entraîne en particulier $u((x_\lambda)) = 0$ si un des $x_\lambda$ est nul.

Considérons encore le *problème d’application universelle* où $\Sigma$ est l’espèce de structure de $\mathbf{Z}$-module, et les $\alpha$-applications les applications multiadditives de $G$ dans un $\mathbf{Z}$-module. On en obtient encore une solution en considérant le $\mathbf{Z}$-module $C = \mathbf{Z}^{(G)}$ des combinaisons linéaires formelles d’éléments de $G$ à coefficients dans $\mathbf{Z}$, et le sous-$\mathbf{Z}$-module $D$ de $C$ engendré par les éléments de la forme

$$
(x_\mu + y_\mu, (z_\lambda)_{\lambda \neq \mu}) - (x_\mu, (z_\lambda)_{\lambda \neq \mu}) - (y_\mu, (z_\lambda)_{\lambda \neq \mu})
$$

où $\mu \in L$, $x_\mu \in G_\mu$, $y_\mu \in G_\mu$ et les $z_\lambda \in G_\lambda$ ($\lambda \neq \mu$) sont arbitraires. On appelle *produit tensoriel (sur $\mathbf{Z}$) de la famille* $(G_\lambda)_{\lambda \in L}$ *de $\mathbf{Z}$-modules* et on note $\bigotimes_{\lambda \in L} G_\lambda$ le $\mathbf{Z}$-module quotient $C/D$; pour tout élément $(x_\lambda)_{\lambda \in L}$ de $G$ qui est un élément de la base canonique de $C$, on note $\bigotimes_{\lambda \in L} x_\lambda$ l’image canonique de cet élément dans $C/D$. Il résulte des définitions précédentes que l’application $\varphi : (x_\lambda) \mapsto \bigotimes_{\lambda \in L} x_\lambda$ de $G$ dans $\bigotimes_{\lambda \in L} G_\lambda$ est $\mathbf{Z}$-multilinéaire, et que pour toute application $\mathbf{Z}$-multilinéaire $f$ de $G$ dans un $\mathbf{Z}$-module $H$, il existe une application $\mathbf{Z}$-linéaire et une seule $g : \bigotimes_{\lambda \in L} G_\lambda \to H$ telle que $f = g \circ \varphi$; le couple $(\bigotimes_{\lambda \in L} G_\lambda, \varphi)$ résout donc le problème d’application universelle considéré.

Soit $(G'_\lambda)_{\lambda \in L}$ une seconde famille de $\mathbf{Z}$-modules, et pour tout $\lambda \in L$, soit $v_\lambda : G_\lambda \to G'_\lambda$ une application $\mathbf{Z}$-linéaire (autrement dit un homomorphisme de groupes commutatifs). Alors l’application

$$
(x_\lambda) \mapsto \bigotimes_{\lambda \in L} v_\lambda(x_\lambda)
$$

de $G$ dans $\bigotimes_{\lambda \in L} G_\lambda$ est *$\mathbf{Z}$-multilinéaire*, et définit donc canoniquement une application *$\mathbf{Z}$-linéaire* de $\bigotimes_{\lambda \in L} G_\lambda$ dans $\bigotimes_{\lambda \in L} G'_\lambda$, qu’on note $\bigotimes_{\lambda \in L} v_\lambda$ et qui est telle que

$$
(\bigotimes_{\lambda \in L} v_\lambda)(\bigotimes_{\lambda \in L} x_\lambda) = \bigotimes_{\lambda \in L} v_\lambda(x_\lambda).
$$

En particulier, considérons, pour un $\mu \in L$, un endomorphisme $\theta$ de $G_\mu$; nous désignerons par $\tilde{\theta}$ l’endomorphisme de $\bigotimes_{\lambda \in L} G_\lambda$ égal à $\bigotimes_{\lambda \in L} v_\lambda$, où l’on prend $v_\mu = \theta$ et $v_\lambda = 1_{G_\lambda}$ pour $\lambda \neq \mu$.

Cela étant, supposons donnés un ensemble $\Omega$, une application

$$
c : \omega \mapsto (\rho(\omega), \sigma(\omega))
$$

de $\Omega$ dans $L \times L$, et pour tout $\omega \in \Omega$, un endomorphisme $p_\omega$ de $G_{\rho(\omega)}$, et un endomorphisme $q_\omega$ de $G_{\sigma(\omega)}$; il leur correspond deux endomorphismes $\tilde{p}_\omega$ et $\tilde{q}_\omega$ de $P = \bigotimes_{\lambda \in L} G_\lambda$. Soit $R$ le sous-$\mathbf{Z}$-module de $P$ *engendré par la réunion des images des endomorphismes* $\tilde{p}_\omega - \tilde{q}_\omega$ lorsque $\omega$ parcourt $\Omega$. Le $\mathbf{Z}$-module quotient $P/R$ s’appelle le produit tensoriel de la famille $(G_\lambda)_{\lambda \in L}$ relativement à $c, p, q$ et se note $\bigotimes_{(c, p, q)} G_\lambda$; en composant l’homomorphisme canonique $P \to P/R$ avec l’application $\varphi : G \to \bigotimes_{\lambda \in L} G_\lambda$ définie ci-dessus, on obtient une application $\mathbf{Z}$-multilinéaire $\varphi_{(c, p, q)} : G \to \bigotimes_{(c, p, q)} G_\lambda$ et on pose $\varphi_{(c, p, q)}((x_\lambda)) = \bigotimes_{(c, p, q)} x_\lambda$ ou simplement $\bigotimes_{(c)} x_\lambda$. Le couple formé de $\bigotimes_{(c, p, q)} G_\lambda$ et de $\varphi_{(c, p, q)}$ résout le problème d’application universelle suivant: désignons par $\bar{p}_\omega$ (resp. $\bar{q}_\omega$) l’application
$$
(x_{\rho(\omega)}, (x_\lambda)_{\lambda \neq \rho(\omega)}) \mapsto (\bar{p}_\omega(x_{\rho(\omega)}), (x_\lambda)_{\lambda \neq \rho(\omega)})
$$
(resp. $(x_{\sigma(\omega)}, (x_\lambda)_{\lambda \neq \sigma(\omega)}) \mapsto (\bar{q}_\omega(x_{\sigma(\omega)}), (x_\lambda)_{\lambda \neq \sigma(\omega)})$)
de $G$ dans lui-même. On prend alors pour $\Sigma$ l’espèce de structure de $\mathbf{Z}$-module, et pour $\alpha$-applications les applications $\mathbf{Z}$-multilinéaires $u$ de $G$ dans un $\mathbf{Z}$-module vérifiant en outre les conditions
$$(26)$$
$$u \circ \bar{p}_\omega = u \circ \bar{q}_\omega$$
pour tout $\omega \in \Omega$. La démonstration est évidente à partir des définitions précédentes.

Cette construction redonne en particulier celle de $E \otimes_A F$ décrite dans II, p. 51: il faut ici prendre $L = \{1, 2\}$, $G_1 = E$, $G_2 = F$, $\Omega = A$; en outre, pour tout $\omega \in A$, on doit poser $\rho(\omega) = 1$, $\sigma(\omega) = 2$, $\bar{p}_\omega$ est l’endomorphisme $x \mapsto x \omega$ du $\mathbf{Z}$-module $E$ et $\bar{q}_\omega$ l’endomorphisme $y \mapsto \omega y$ du $\mathbf{Z}$-module $F$.

Soit $(G'_\lambda)_{\lambda \in L}$ une seconde famille de $\mathbf{Z}$-modules; l’application $c$ restant la même, supposons donnés, pour tout $\omega \in \Omega$, un endomorphisme $p'_\omega$ de $G'_{\rho(\omega)}$ et un endomorphisme $q'_\omega$ de $G'_{\sigma(\omega)}$. Pour tout $\lambda \in L$, soit alors $v_\lambda : G_\lambda \to G'_\lambda$ une application $\mathbf{Z}$-linéaire telle que, pour tout $\omega \in \Omega$, on ait
$$(27)$$
$$v_{\rho(\omega)} \circ p_\omega = p'_\omega \circ v_{\rho(\omega)} \quad \text{et} \quad v_{\sigma(\omega)} \circ q_\omega = q'_\omega \circ v_{\sigma(\omega)}$$
(en d’autres termes, pour tout $\lambda \in L$, $v_\lambda$ est un morphisme pour les lois d’action sur $G_\lambda$ (resp. $G'_\mu$) définies par les $p_\xi$ et $q_\eta$ (resp. $p'_\xi$ et $q'_\eta$), avec $\xi$ et $\eta$ tels que $\rho(\xi) = \lambda$ et $\sigma(\eta) = \lambda$). Alors l’application
$$u : (x_\lambda) \mapsto \bigotimes_{(c, p', q')} v_\lambda(x_\lambda)$$
de $G$ dans $\bigotimes_{(c, p', q')} G'_\lambda$ est $\mathbf{Z}$-multilinéaire et vérifie les conditions (26), donc définit une application $\mathbf{Z}$-linéaire de $\bigotimes_{(c, p', q)} G_\lambda$ dans $\bigotimes_{(c, p', q')} G'_\lambda$, que nous noterons simplement $\bigotimes_{(c)} v_\lambda$ s’il n’en résulte pas de confusion.

Nous allons maintenant donner une propriété d’« associativité » pour les produits tensoriels généraux ainsi définis. Soit $(L_i)_{1 \leq i \leq n}$ une partition finie de $L$; pour tout indice $i$, désignons par $\Omega_i$ la partie de $\Omega$ formée des éléments tels que l’on ait $\rho(\omega) \in L_i$ et $\sigma(\omega) \in L_i$; il est clair que les $\Omega_i$ sont deux à deux disjoints; nous poserons $\Omega' = \Omega - (\bigcup_i \Omega_i)$. Pour chaque indice $i$, nous désignerons par $c^{(i)}$ l’application $\omega \mapsto (\rho(\omega), \sigma(\omega))$ de $\Omega_i$ dans $L_i \times L_i$; pour $\omega \in \Omega_i$, nous écrirons $p_{\omega}^{(i)}$ et $q_{\omega}^{(i)}$ au lieu de $p_\omega$ et $q_\omega$. On a donc pour chaque $i$ un produit tensoriel « partiel »

$$
F_i = \bigotimes_{(c^{(i)}, p^{(i)}, q^{(i)})} G_\lambda.
$$

Nous ferons en outre l’hypothèse de « permutabilité » suivante:

(P) *Si* $\omega \in \Omega'$, $p_\omega$ (resp. $q_\omega$) *permute avec chacun des endomorphismes* $p_\xi$ *et* $q_\eta$ *de* $G_{\rho(\omega)}$ (resp. $G_{\sigma(\omega)}$) *tels que* $\xi \notin \Omega', \eta \notin \Omega'$ *et* $\rho(\omega) = \rho(\xi) = \sigma(\eta)$ (resp. $\sigma(\omega) = \rho(\xi) = \sigma(\eta)$).

Pour chaque $\omega \in \Omega'$, soit $i$ l’indice tel que $\rho(\omega) \in L_i$; considérons alors la famille $(v_\lambda)_{\lambda \in L_i}$ où $v_{\rho(\omega)} = p_\omega$ et $v_\lambda = 1_{G_\lambda}$ pour $\lambda \neq \rho(\omega)$; l’hypothèse (P) entraîne que la famille $(v_\lambda)$ vérifie les conditions (27) de II, p. 67 (où on doit remplacer $p'$ et $p$ par $p^{(i)}$, $q'$ et $q$ par $q^{(i)}$, $\omega$ par un élément $\xi$ parcourant $\Omega_i$); on en déduit donc un endomorphisme $\bigotimes_{(c^{(i)})} v_\lambda = r_\omega$ du $\mathbf{Z}$-module $F_i$. De la même manière, on définit un endomorphisme $s_\omega$ du $\mathbf{Z}$-module $F_j$ à partir de $q_\omega$, $j$ étant l’indice tel que $\sigma(\omega) \in L_j$; posons enfin $d(\omega) = (i, j)$. On peut alors définir le *produit tensoriel* $\bigotimes_{(d, r, s)} F_i$, et l’application canonique correspondante

$$
\varphi_{(d, r, s)} : \prod_{i=1}^n F_i \to \bigotimes_{(d, r, s)} F_i.
$$

On a d’autre part, pour chaque $i$, l’application canonique $\psi_i = \varphi_{(c^{(i)}, p^{(i)}, q^{(i)})} : \prod_{\lambda \in L_i} G_\lambda \to F_i$; utilisant l’associativité du produit d’ensembles, on en déduit une application $\mathbf{Z}$-multilinéaire $\psi = \varphi_{(d, r, s)} \circ (\psi_i)$ de $G$ dans $\bigotimes_{(d, r, s)} F_i$. Nous allons montrer que *le couple* $(\bigotimes_{(d, r, s)} F_i, \psi)$ *est solution du même problème universel que* $(\bigotimes_{(c, p, q)} G_\lambda, \varphi_{(c, p, q)})$, d’où résultera l’existence d’un *unique isomorphisme de* $\mathbf{Z}$*-modules*

$$
\theta : \bigotimes_{(c, p, q)} G_\lambda \to \bigotimes_{(d, r, s)} F_i
$$

tel que $\psi = \theta \circ \varphi_{(c, p, q)}$ (E, IV, p. 23).

Par récurrence sur $n$, on se ramène au cas $n = 2$; nous écrirons pour simplifier $F_1 \otimes_{(d)} F_2$ et $y_1 \otimes_{(d)} y_2$ au lieu de $\bigotimes_{(d, r, s)} F_i$ et $\bigotimes_{(d, r, s)} y_i$. Considérons l’application de $G$ dans $F_1 \otimes_{(d)} F_2$

$$
h : (x_\lambda) \mapsto \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right).
$$

Elle est évidemment $\mathbf{Z}$-multilinéaire; montrons qu’elle satisfait aux conditions (26) de II, p. 67 pour tout $\omega \in \Omega$. C’est évident si $\omega \in \Omega_1$ ou $\omega \in \Omega_2$; dans le cas contraire, en supposant pour fixer les idées que l’on ait $\rho(\omega) \in L_1$ et $\sigma(\omega) \in L_2$, les valeurs de $h \circ \bar{p}_\omega$ et $h \circ \bar{q}_\omega$ pour $(x_\lambda)$ sont respectivement

$$
(r_\omega (\bigotimes_{(c^{(1)})} x_\lambda)) \otimes_{(d)} (\bigotimes_{(c^{(2)})} x_\lambda) \quad \text{et} \quad (\bigotimes_{(c^{(1)})} x_\lambda) \otimes_{(d)} (s_\omega (\bigotimes_{(c^{(2)})} x_\lambda))
$$

qui sont encore égales par définition de $F_1 \otimes_{(d)} F_2$.

Cela étant, soit $u$ une application $\mathbf{Z}$-multilinéaire de $G$ dans un $\mathbf{Z}$-module $H$, vérifiant les conditions (26) de II, p. 67; nous allons définir une application $\mathbf{Z}$-linéaire $v : F_1 \otimes_{(d)} F_2 \to H$ telle que $u = v \circ h$, et cela prouvera notre assertion (en répétant le raisonnement de II, p. 51, cor. 1). Pour tout $z_2 = (x_\lambda)_{\lambda \in L_2}$, considérons l’application « partielle » de $\prod_{\lambda \in L_1} G_\lambda$ dans $H$

$$
u(., z_2) : (x_\lambda)_{\lambda \in L_1} \mapsto u((x_\lambda)_{\lambda \in L_1}, z_2) = u((x_\lambda)_{\lambda \in L}).
$$

Il est clair qu’elle est $\mathbf{Z}$-multilinéaire et vérifie les conditions (26) de II, p. 67 pour $\omega \in \Omega_1$; par définition, il existe donc une application $\mathbf{Z}$-linéaire $y_1 \mapsto w_1(y_1, z_2)$ de $F_1$ dans $H$ telle que

$$
w_1(\bigotimes_{(c^{(1)})} x_\lambda, z_2) = u((x_\lambda)_{\lambda \in L_1}, z_2).
$$

Considérons ensuite l’application

$$
u_2 : (x_\lambda)_{\lambda \in L_2} \mapsto w_1(., (x_\lambda)_{\lambda \in L_2})
$$

de $\prod_{\lambda \in L_2} G_\lambda$ dans $\mathrm{Hom}_\mathbf{Z}(F_1, H)$; elle est évidemment $\mathbf{Z}$-multilinéaire et vérifie les conditions (26) de II, p. 67 pour $\omega \in \Omega_2$, en vertu de l’hypothèse sur $u$ et des relations (28) et (29), et compte tenu de ce que les éléments de la forme $\bigotimes_{(c^{(1)})} x_\lambda$ engendrent le $\mathbf{Z}$-module $F_1$. Il existe donc une application $\mathbf{Z}$-linéaire

$$
w_2 : F_2 \to \mathrm{Hom}_\mathbf{Z}(F_1, H)
$$

telle que

$$
w_2(\bigotimes_{(c^{(2)})} x_\lambda) = u_2((x_\lambda)_{\lambda \in L_2})
$$

ou encore

$$
(w_2(\bigotimes_{(c^{(2)})} x_\lambda))(\bigotimes_{(c^{(1)})} x_\lambda) = u((x_\lambda)_{\lambda \in L}).
$$

Considérons alors, pour $y_1 \in F_1, y_2 \in F_2$, l’élément de $H$

$$
w(y_1, y_2) = (w_2(y_2))(y_1).
$$

Il est clair que $w$ est une application $\mathbf{Z}$-bilinéaire de $F_1 \times F_2$ dans $H$. Montrons en outre que pour tout $\omega \in \Omega'$, on a (en supposant pour fixer les idées, que $\rho(\omega) \in L_1$ et $\sigma(\omega) \in L_2$)

$$
w(r_\omega(y_1), y_2) = w(y_1, s_\omega(y_2)).
$$

Il suffit de vérifier cette relation lorsque $y_1$ (resp. $y_2$) est de la forme $\bigotimes_{(c^{(1)})} x_\lambda$ (resp. $\bigotimes_{(c^{(2)})} x_\lambda$), ces éléments engendrant le $\mathbf{Z}$-module $F_1$ (resp. $F_2$). Mais par définition,
$$
r_\omega \left( \bigotimes_{(c^{(1)})} x_\lambda \right) = \bigotimes_{(c^{(1)})} x'_\lambda, \text{ où } x'_{\rho(\omega)} = p_\omega(x_{\rho(\omega)}) \text{ et } x'_\lambda = x_\lambda \text{ pour } \lambda \neq \rho(\omega) \text{ dans } L_1;
$$
même $s_\omega \left( \bigotimes_{(c^{(2)})} x_\lambda \right) = \bigotimes_{(c^{(2)})} x''_\lambda$, où $x''_{\sigma(\omega)} = q_\omega(x_{\sigma(\omega)})$ et $x''_\lambda = x_\lambda$ pour $\lambda \neq \sigma(\omega)$ dans $L_2$; compte tenu de (30) et (31), la relation (32) se déduit alors de (26) (II, p. 67). Il existe donc une application $\mathbf{Z}\text{-linéaire} \ v$ de $F_1 \otimes_{(a)} F_2$ dans $H$ telle que $v(y_1 \otimes_{(a)} y_2) = w(y_1, y_2)$, et il résulte alors de (30) et (31) (II. p. 69) que l’on a bien $v \circ h = u$.

Le cas particulier le plus important du produit tensoriel général défini ci-dessus est le suivant: on part d’une famille $(A_i)_{1 \leq i \leq n-1}$ d’anneaux, et d’une famille $(E_i)_{1 \leq i \leq n}$, où $E_1$ est un $A_1$-module à droite, $E_n$ un $A_{n-1}$-module à gauche et pour $2 \leq i \leq n-1$, $E_i$ est un $(A_{i-1}, A_i)\text{-bimodule}$. On applique alors la définition ci-dessus comme suit: $L$ est l’ensemble $\{1, n\}$, $G_i = E_i$, $\Omega$ est l’ensemble somme des $A_i$ ($1 \leq i \leq n-1$). Pour $\omega \in A_i$ ($1 \leq i \leq n-1$), on prend $\rho(\omega) = i$, $\sigma(\omega) = i+1$, $p_\omega$ est l’endomorphisme $x \mapsto x \omega$ du $\mathbf{Z}$-module $E_i$ et $q_\omega$ l’endomorphisme $y \mapsto \omega y$ du $\mathbf{Z}$-module $E_{i+1}$; on note le produit tensoriel correspondant
$$
E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n
$$
(notation où l’on se permet parfois de supprimer les $A_i$), et l’élément $\bigotimes_{(c, p, q)} x_i$ de ce produit tensoriel, pour une famille $(x_i)$ telle que $x_i \in E_i$ pour $1 \leq i \leq n$, s’écrit $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ si aucune confusion n’en résulte; on emploie une notation analogue pour une application $\mathbf{Z}\text{-linéaire} \ \bigotimes_{(c)} v_i$. L’hypothèse (P) est vérifiée pour toute partition de $\{1, n\}$, en raison de l’hypothèse que les $E_i$ sont des bimodules pour $2 \leq i \leq n-1$. Lorsque $n = 3$, on a ainsi défini le $\mathbf{Z}$-module $E \otimes_A F \otimes_B G$ auquel il a été fait allusion dans II, p. 65, et retrouvé la prop. 8 (II, p. 64).

Lorsque chacun des $E_i$ est un multimodule (dont, pour $2 \leq i \leq n-1$, $A_{i-1}$ est un des anneaux opérant à gauche et $A_i$ un des anneaux opérant à droite, avec des conditions analogues pour $i = 1$ et $i = n$) on définit comme dans II, p. 54, sur $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ une structure de multimodule par rapport à tous les anneaux autres que les $A_i$ qui opèrent sur les $E_i$ ($1 \leq i \leq n$).

En particulier, soient $C$ un anneau commutatif, $(E_i)_{1 \leq i \leq n}$ une famille de $C\text{-modules}$. En munissant $E_1$ et $E_n$ de deux structures de $C$-module identiques à la structure donnée, $E_i$ pour $2 \leq i \leq n-1$ de trois structures de $C$-modules identiques à la structure donnée, on définit sur le produit tensoriel
$$
E_1 \otimes_C E_2 \otimes_C E_3 \otimes \cdots \otimes_C E_{n-1} \otimes_C E_n
$$
$n$ structures de $C$-module deux à deux compatibles, et qui sont en fait identiques, car pour $\gamma \in \mathbf{C}$ et $(x_i) \in \prod_{i=1}^n E_i$, on a par définition $(\gamma x_1) \otimes x_2 \otimes \cdots \otimes x_n = x_1 \otimes (\gamma x_2) \otimes \cdots \otimes x_n = \cdots = x_1 \otimes x_2 \otimes \cdots \otimes (\gamma x_n)$.

Lorsqu’on parle du produit tensoriel (34) (II, p. 70) comme d’un C-module, c’est toujours de cette structure qu’il est question, sauf mention expresse du contraire, et le produit tensoriel (34) se note aussi $\bigotimes_{1 \leq i \leq n} E_i$ s’il n’en résulte pas de confusion. Pour tout C-module G, les applications $\mathbf{Z}$-multilinéaires de $\prod_{i=1}^n E_i$ dans G qui, pour tout indice $i$, vérifient la relation
$$
f(x_1, \ldots, x_{i-1}, \gamma x_i, x_{i+1}, \ldots, x_n) = \gamma f(x_1, \ldots, x_n)
$$
pour $\gamma \in \mathbf{C}$ et $(x_i) \in \prod_i E_i$ sont alors dites C-multilinéaires et forment un C-module que l’on note $\mathcal{L}_n(E_1, \ldots, E_n; G)$; la propriété universelle du produit tensoriel (34) (II, p.70) permet donc de définir un isomorphisme canonique de C-modules
$$
\mathcal{L}_n(E_1, \ldots, E_n; G) \to \mathrm{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, G)
$$
qui à toute application C-multilinéaire $f$, fait correspondre l’application C-linéaire $g$ telle que
$$
f(x_1, \ldots, x_n) = g(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$
Une application C-multilinéaire de $E_1 \times \cdots \times E_n$ dans $\mathbf{C}$ est encore appelée forme $n$-linéaire.

Soit $(F_i)_{1 \leq i \leq n}$ une seconde famille de C-modules; pour tout système de $n$ applications C-linéaires $u_i : E_i \to F_i$, $u_1 \otimes u_2 \otimes \cdots \otimes u_n$ (aussi notée $\bigotimes_{1 \leq i \leq n} u_i$) est une application C-linéaire de
$$
E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n \text{ dans } F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n.
$$
En outre, $(u_1, \ldots, u_n) \mapsto u_1 \otimes u_2 \otimes \cdots \otimes u_n$ est une application C-multilinéaire de $\prod_i \mathrm{Hom}_\mathbf{C}(E_i, F_i)$ dans
$$
\mathrm{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n).
$$
Il correspond donc canoniquement à cette dernière application une application C-linéaire dite canonique
$$
\mathrm{Hom}_\mathbf{C}(E_1, F_1) \otimes_\mathbf{C} \mathrm{Hom}_\mathbf{C}(E_2, F_2) \otimes \cdots \otimes_\mathbf{C} \mathrm{Hom}_\mathbf{C}(E_n, F_n)
$$
$$
\to \mathrm{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n)
$$
généralisant celle définie dans II, p. 57 pour $n = 2$.

La propriété générale d’associativité vue plus haut se particularise ici comme suit. Étant donnée une partition $(J_k)_{1 \leq k \leq m}$ de l’intervalle $[1, n]$ de $\mathbf{N}$, soit, pour chaque $k$, $F_k$ le produit tensoriel $E_{i_1} \otimes_\mathbf{C} E_{i_2} \otimes \cdots \otimes_\mathbf{C} E_{i_r}$, où $(i_1, \ldots, i_r)$ est la suite strictement croissante des éléments de $J_k$. Alors on a un isomorphisme canonique (dit « isomorphisme d’associativité ») de C-modules

$$
F_1 \otimes_C F_2 \otimes \cdots \otimes_C F_m \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

qui, avec les notations précédentes, fait correspondre le produit tensoriel $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ (où $x_i \in E_i$ pour tout $i$) au produit tensoriel

$$
y_1 \otimes y_2 \otimes \cdots \otimes y_m,\quad \text{où } y_k = x_{i_1} \otimes x_{i_2} \otimes \cdots \otimes x_{i_r}.
$$

En particulier, si $\pi$ est une permutation de $\{1, n\}$, en posant $J_k = \{\pi(k)\}$ pour $1 \leq k \leq n$, on obtient un isomorphisme canonique (dit « de commutativité »)

$$
E_{\pi(1)} \otimes_C E_{\pi(2)} \otimes \cdots \otimes_C E_{\pi(n)} \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

qui fait correspondre $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ à $x_{\pi(1)} \otimes x_{\pi(2)} \otimes \cdots \otimes x_{\pi(n)}$. Nous identifierons souvent les divers produits tensoriels qui se correspondent par ces isomorphismes canoniques.

Pour $1 \leq i \leq n$, supposons que $E_i$ admette une base $(b^{(i)}_{\lambda_i})_{\lambda_i \in L_i}$; par récurrence sur $n$, il résulte de II, p. 62, cor. 2, que la famille $(b^{(1)}_{\lambda_1} \otimes b^{(2)}_{\lambda_2} \otimes \cdots \otimes b^{(n)}_{\lambda_n})$, où $(\lambda_1, ..., \lambda_n)$ parcourt $\prod_{1 \leq i \leq n} L_i$, est une base de $\bigotimes_{1 \leq i \leq n} E_i$, qu’on appelle parfois le *produit tensoriel* des bases $(b^{(i)}_{\lambda_i})$ considérées.

#### Remarque 1 {#alg-ii-s3-n9-rem-1 .statement}

Les considérations précédentes relatives au cas des modules sur un anneau commutatif se généralisent comme dans II, p. 57, *Remarque* 2 lorsqu’il s’agit d’un produit tensoriel $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ où les anneaux $A_i$ ne sont pas nécessairement commutatifs, et où l’on a pour chaque $i$ un homomorphisme $\rho_i : C \to A_i$ d’un même anneau *commutatif* $C$ tel que: 1° $\rho_i(C)$ est contenu dans le *centre* de $A_i$; 2° pour $2 \leq i \leq n - 1$, les structures de $C$-module sur $E_i$ obtenues à l’aide des homomorphismes $\rho_{i-1}$ et $\rho_i$ *coïncident*. On obtient alors sur $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ une structure de $C$*-module*, et des applications canoniques analogues à (13) (II, p. 57), que nous laissons au lecteur le soin d’expliciter.

#### Remarque 2 {#alg-ii-s3-n9-rem-2 .statement}

Soient $A, B$ deux anneaux, $E$ un $A$-module à droite, $E'$ un $A$-module à gauche, $F$ un $B$-module à droite, $F'$ un $B$-module à gauche. Les applications $\mathbf{Z}$-*bilinéaires* de $(E \otimes_A E') \times (F \otimes_B F')$ dans un $\mathbf{Z}$-module $G$ sont alors en *correspondance biunivoque* avec les applications $\mathbf{Z}$-*multilinéaires* $f$ de $E \times E' \times F \times F'$ dans $G$, satisfaisant aux conditions

$$
\begin{cases}
f(x \lambda, x', y, y') = f(x, \lambda x', y, y') \\
f(x, x', y \mu, y') = f(x, x', y, \mu y')
\end{cases}
$$

pour $\lambda \in A, \mu \in B, x \in E, x' \in E', y \in F, y' \in F'$. En effet, les constructions générales données dans ce n° ramènent à définir un isomorphisme canonique de $\mathbf{Z}$-modules entre $(E \otimes_A E') \otimes_{\mathbf{Z}} (F \otimes_B F')$ et $E \otimes_A E' \otimes_{\mathbf{Z}} F \otimes_B F'$, qui résulte de la propriété d’associativité des produits tensoriels de la forme (33).

## EXERCICES {#alg-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
