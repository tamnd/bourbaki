---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 2
section_title: Bidual. Espaces réflexifs
lang: fr
source: evt-i-v-fr
book_pages: EVT IV.14-EVT IV.20, EVT IV.52-EVT IV.57
pdf_pages: 0200-0206, 0238-0243
extraction: ocr
subsections:
    - "no": 1
      title: Bidual
      page: 14
      pdf_page: 200
    - "no": 2
      title: Espaces semi-réflexifs
      page: 15
      pdf_page: 201
    - "no": 3
      title: Espaces réflexifs
      page: 16
      pdf_page: 202
    - "no": 4
      title: Cas des espaces normés
      page: 16
      pdf_page: 202
    - "no": 5
      title: Espaces de Montel
      page: 18
      pdf_page: 204
statements: 34
exercises: 26
content_sha256: e6722903ebc281254eb64317db1378ab5062b413f45e36d36748bd41a178c207
---

## § 2. BIDUAL. ESPACES RÉFLEXIFS

### 1. Bidual

#### Définition 1 {#evt-iv-s2-def-1 .statement}

*Soient* $E$ *un espace localement convexe et* $E'_b$ *son dual fort*. *On appelle bidual de* $E$, *et l’on note* $E''$, *le dual de l’espace localement convexe* $E'_b$.

Pour tout $x \in E$, notons $\tilde{x}$ la forme linéaire $x' \mapsto \langle x, x' \rangle$ sur $E'$ : elle est continue pour la topologie faible $\sigma(E', E)$, donc *a fortiori* pour la topologie forte sur $E'$; on a donc $\tilde{x} \in E''$ pour tout $x \in E$. L’application $c_E : x \mapsto \tilde{x}$ de $E$ dans $E''$ est une application linéaire, dite *canonique*.

#### Proposition 1 {#evt-iv-s2-prop-1 .statement}

*Le noyau de* $c_E : E \to E''$ *est l’adhérence de* 0 *dans* $E$. *Si* $E$ *est séparé*, $c_E$ *est injective*.

Par construction, le noyau de $c_E$ est l’intersection des noyaux des formes linéaires continues sur $E$, c’est-à-dire l’adhérence de $\{0\}$ dans $E$ (II, p. 26, cor. 1).

Lorsque $E$ est séparé, on identifie $E$ à un sous-espace de $E''$ grâce à $c_E$.

La topologie *forte* sur $E''$ est la $\mathcal{S}$-topologie, où $\mathcal{S}$ est l’ensemble des parties fortement bornées de $E'$. Comme toute partie équicontinue de $E'$ est fortement bornée (III, p. 22, prop. 9), la topologie initiale sur $E$ est *moins fine* que la topologie image réciproque par $c_E$ de la topologie forte de $E''$; elle peut être strictement moins fine (IV, p. 52, exerc. 1). Toutefois :

#### Proposition 2 {#evt-iv-s2-prop-2 .statement}

*Supposons l’espace* $E$ *bornologique ou tonnelé*. *La topologie initiale sur* $E$ *est image réciproque par* $c_E$ *de la topologie forte sur* $E''$.

En effet, toute partie de $E'$ qui est fortement bornée est équicontinue (III, p. 22, prop. 10 et III, p. 24).

#### Proposition 3 {#evt-iv-s2-prop-3 .statement}

Soit E un espace localement convexe séparé. Pour que le dual fort $E'_b$ de E soit tonnelé, il faut et il suffit que toute partie de $E''$ bornée pour $\sigma(E'', E')$ soit contenue dans l’adhérence pour $\sigma(E'', E')$ d’une partie bornée de E.

En effet, les parties équicontinues de $E''$ sont les parties contenues dans le bipolaire (pour la dualité entre $E''$ et $E'$) d’une partie bornée du sous-espace E de $E''$. Il suffit donc d’appliquer le th. des bipolaires (II, p. 49, cor. 3) et la définition d’un espace tonnelé (III, p. 24).

#### Remarque {#evt-iv-s2-n1-rem-1 .statement}

Soient E un espace localement convexe séparé, $E'$ son dual et $E''$ son bidual. On a $E \subset E'' \subset {E'}^*$, où ${E'}^*$ est le dual algébrique de $E'$. Si B est une partie bornée de E, son adhérence $\overline{B}$ dans ${E'}^*$ muni de $\sigma({E'}^*, E')$ est contenue dans $E''$ : en effet, le polaire $U = B^\circ$ de B dans $E'$ est un voisinage de 0 dans $E'_b$, et l’on a
$$
\overline{B} \subset U^\circ \subset E''.
$$

### 2. Espaces semi-réflexifs

#### Définition 2 {#evt-iv-s2-def-2 .statement}

Soit E un espace localement convexe. On dit que E est semi-réflexif si l’application canonique $c_E$ de E dans $E''$ est bijective.

Cela signifie que E est séparé, et que toute forme linéaire sur $E'$, continue pour la topologie forte $\beta(E', E)$, est de la forme $x' \mapsto \langle x, x' \rangle$ avec $x \in E$, c’est-à-dire continue pour la topologie faible $\sigma(E', E)$.

#### Théorème 1 {#evt-iv-s2-thm-1 .statement}

Un espace localement convexe séparé E est semi-réflexif si et seulement si toute partie bornée de E est relativement compacte pour la topologie affaiblie $\sigma(E, E')$. Si E est semi-réflexif, le dual fort $E'_b$ de E est tonnelé.

La deuxième assertion résulte de la prop. 3 (IV, p. 15), et de l’identité entre ensembles bornés pour la topologie initiale et pour la topologie affaiblie de E (III, p. 28, cor. 3).

Dire que E est semi-réflexif signifie que la topologie de $E'_b$ est compatible avec la dualité entre E et $E'$, autrement dit, par le th. de Mackey (IV, p. 2, th. 1) que la topologie de $E'_b$ est moins fine que $\tau(E', E)$ (et en fait lui est identique) ; par définition (IV, p. 2), cela signifie que toute partie convexe fermée et bornée de E est compacte pour $\sigma(E, E')$, et cela équivaut à dire que toute partie bornée de E est relativement compacte pour $\sigma(E, E')$, puisque l’enveloppe convexe fermée d’une partie bornée de E est bornée (III, p. 3, prop. 1).

#### Corollaire {#evt-iv-s2-n2-cor-1 .statement}

Soit E un espace localement convexe semi-réflexif. Tout sous-espace vectoriel fermé M de E est semi-réflexif; de plus, la topologie forte sur $E'/M^\circ$ (considéré comme dual de M) est quotient de la topologie forte de $E'$.

Soit B une partie bornée de M. Comme B est bornée dans E, et que la topologie affaiblie $\sigma(M, M')$ est induite par $\sigma(E, E')$ sur M (IV, p. 10, prop. 11), l’adhérence de B dans M muni de $\sigma(M, M')$ est compacte. Donc M est semi-réflexif d’après le th. 1. La dernière assertion du corollaire résulte de la prop. 10 de IV, p. 9, appliquée à l’ensemble $\mathfrak{S}$ de toutes les parties convexes, fermées et bornées de E.

#### Remarque 1 {#evt-iv-s2-n2-rem-1 .statement}

Supposons E semi-réflexif. Toute partie de E qui est convexe, bornée et fermée pour la topologie initiale est compacte pour la topologie $\sigma(E, E')$ (IV, p. 1, prop. 1). \* Par contre, la sphère unité (d’équation $\|x\| = 1$) d’un espace hilbertien E de dimension infinie est bornée et fermée pour la topologie initiale, mais elle n’est pas fermée pour la topologie affaiblie, bien que E soit semi-réflexif. \*

#### Remarque 2 {#evt-iv-s2-n2-rem-2 .statement}

D’après la remarque 3 de IV, p. 5, on peut reformuler comme suit le th. 1 : l’espace séparé E est semi-réflexif si et seulement s’il est quasi-complet pour sa topologie affaiblie. S’il est semi-réflexif, il est donc quasi-complet pour sa topologie initiale (IV, p. 5, Remarque 2).

#### Remarque 3 {#evt-iv-s2-n2-rem-3 .statement}

Sous les hypothèses du corollaire ci-dessus, l’espace E/M n’est pas nécessairement semi-réflexif (IV, p. 64, exerc. 10).

### 3. Espaces réflexifs

#### Définition 3 {#evt-iv-s2-def-3 .statement}

On dit qu’un espace localement convexe E est réflexif si l’application canonique $c_E$ de E dans $E''$ est un isomorphisme d’espaces vectoriels topologiques de E sur le dual fort de $E'_b$.
En particulier, un espace réflexif est semi-réflexif, donc séparé.

#### Proposition 4 {#evt-iv-s2-prop-4 .statement}

Le dual fort d’un espace réflexif est réflexif.
Cela résulte aussitôt de la déf. 3.

#### Théorème 2 {#evt-iv-s2-thm-2 .statement}

Pour qu’un espace localement convexe séparé E soit réflexif, il faut et il suffit qu’il soit tonnelé et que toute partie bornée de E soit relativement compacte pour la topologie affaiblie $\sigma(E, E')$.
D’après le th. 1 (IV, p. 15), il revient au même de dire que E est réflexif si et seulement s’il est semi-réflexif et tonnelé.
Si E est réflexif, $E'_b$ est réflexif (prop. 4) et par suite E est tonnelé (IV, p. 15, th. 1). Réciproquement, si E est semi-réflexif et tonnelé, $c_E$ est une bijection et est bicontinue en vertu de IV, p. 14, prop. 2, donc E est réflexif.

#### Remarque 1 {#evt-iv-s2-n3-rem-1 .statement}

Soit E un espace hilbertien réel de dimension infinie. Notons F l’espace E muni de la topologie affaiblie. Les espaces E et F ont même dual E', et E est un espace de Banach réflexif (V, p. 16). Par suite, F est semi-réflexif. Cependant sur E, la topologie forte et la topologie affaiblie sont distinctes, donc F n’est pas réflexif. \*

#### Remarque 2 {#evt-iv-s2-n3-rem-2 .statement}

Soient E un espace réflexif et M un sous-espace vectoriel fermé de E. Il se peut que ni M, ni E/M, ne soient des espaces réflexifs (IV, p. 64, exerc. 10). \* Pour le cas des espaces normés, voir la prop. 7 de IV, p. 17. \*

### 4. Cas des espaces normés

Soit E un espace normé. Sur le dual E' de E, la topologie forte est définie par la norme

(1)
$$
\|x'\| = \sup_{x \in E, \|x\| \leq 1} |\langle x, x' \rangle|,
$$

et le dual fort de E est un espace de Banach (III, p. 24, cor. 2). Le bidual E'' de E est donc aussi un espace de Banach, pour la norme définie par

(2) $$
\|x''\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x', x'' \rangle|.
$$

D’après la prop. 8, (i) de IV, p. 7, l’application linéaire canonique $c_E : E \to E''$ est une isométrie. Nous identifierons désormais E à un sous-espace normé de son bidual E''.

#### Proposition 5 {#evt-iv-s2-prop-5 .statement}

Soient E un espace normé, E' son dual et E'' son bidual. La boule unité (fermée) dans E'' est l’adhérence pour la topologie faible $\sigma(E'', E')$ de la boule unité B dans E.

D’après la formules (1) et (2), la boule unité dans E'' est le bipolaire $B^{\circ \circ}$ de B. La prop. 5 résulte alors du th. des bipolaires (II, p. 49, cor. 3).

#### Remarque {#evt-iv-s2-n4-rem-1 .statement}

Un espace de Banach E est fermé dans son bidual E'' pour la topologie forte, mais dense pour la topologie faible (prop. 5).

Pour qu’un espace normé soit réflexif, il faut et il suffit qu’il soit semi-réflexif ; en effet, la topologie initiale de E est toujours induite par la topologie forte de E''. Le th. 1 (IV, p. 15) entraîne donc le résultat suivant :

#### Proposition 6 {#evt-iv-s2-prop-6 .statement}

Pour qu’un espace normé E soit réflexif, il faut et il suffit que la boule unité dans E soit compacte pour la topologie affaiblie $\sigma(E, E')$.

On notera qu’un espace normé réflexif est complet, donc un espace de Banach, et que son dual est un espace de Banach réflexif d’après la prop. 4 de IV, p. 16.

#### Proposition 7 {#evt-iv-s2-prop-7 .statement}

Soient E un espace de Banach réflexif et M un sous-espace vectoriel fermé de E. Alors M et E/M sont des espaces de Banach réflexifs.

Soient E' le dual de E et M° l’orthogonal de M dans E'. On peut identifier comme espace normé E'/M° au dual M' de M (IV, p. 9, prop. 10). Comme M est semi-réflexif (IV, p. 15, corollaire), il est réflexif, donc aussi E'/M° ; de même M° est réflexif, ainsi que son dual $E/M^{\circ \circ} = E/M$.

#### Exemple 1 {#evt-iv-s2-n4-exa-1 .statement}

On note $\ell^\infty(\mathbf{N})$ l’espace de Banach des suites bornées $x = (x_n)_{n \in \mathbf{N}}$ de scalaires, avec la norme

(3) $$
\|x\| = \sup_{n \in \mathbf{N}} |x_n| \quad (\text{I, p. 4}) .
$$

Soit $c_0(\mathbf{N})$ le sous-espace vectoriel fermé de $\ell^\infty(\mathbf{N})$ formé des suites tendant vers 0. Enfin, soit $\ell^1(\mathbf{N})$ l’espace vectoriel des suites sommables, muni de la norme

(4) $$
\|x\|_1 = \sum_{n \in \mathbf{N}} |x_n| .
$$

On peut montrer (IV, p. 47, exerc. 1) que le dual de $c_0(\mathbf{N})$ s’identifie à $\ell^1(\mathbf{N})$ de sorte qu’on ait

(5) $$
\langle x, x' \rangle = \sum_{n \in \mathbf{N}} x_n x'_n
$$

pour $x \in c_0(\mathbf{N})$ et $x' \in \ell^1(\mathbf{N})$. De même, le dual de $\ell^1(\mathbf{N})$ s’identifie à $\ell^\infty(\mathbf{N})$ de sorte que l’on ait la relation (5) pour $x \in \ell^1(\mathbf{N})$ et $x' \in \ell^\infty(\mathbf{N})$. Donc $\ell^\infty(\mathbf{N})$ est le bidual de $c_0(\mathbf{N})$, et ce dernier n’est pas réflexif.

#### Exemple 2 {#evt-iv-s2-n4-exa-2 .statement}

\* Tout espace hilbertien est un espace de Banach réflexif (V, p.16).

#### Exemple 3 {#evt-iv-s2-n4-exa-3 .statement}

\* Soient X un espace topologique séparé et $\mu$ une mesure complexe sur X. Pour tout nombre réel $p > 1$, l’espace de Banach $L^p(X, \mu)$ est réflexif, et son dual s’identifie à $L^q(X, \mu)$ avec $p^{-1} + q^{-1} = 1$ (INT, V, 2e édit., § 5, no 8 et IX, § 1, no 10).

### 5. Espaces de Montel

#### Définition 4 {#evt-iv-s2-def-4 .statement}

On appelle espace de Montel un espace localement convexe, tonnelé et séparé dans lequel toute partie bornée est relativement compacte.

#### Exemple 1 {#evt-iv-s2-n5-exa-1 .statement}

Tout espace séparé de dimension finie est un espace de Montel. Un espace normé qui est un espace de Montel est localement compact, donc de dimension finie (I, p. 15, th. 3).

#### Exemple 2 {#evt-iv-s2-n5-exa-2 .statement}

Reprenons les hypothèses et notations de la prop. 7 de III, p. 6. L’espace E est tonnelé comme limite inductive d’espaces de Banach (III, p. 25); de plus, toute partie bornée de E est relativement compacte (III, p. 6, prop. 7). Autrement dit, E est un espace de Montel.

En particulier, les espaces de Gevrey (III, p. 10) sont des espaces de Montel. \* Il en est de même de l’espace $\mathcal{H}(K)$ des germes de fonctions analytiques au voisinage d’une partie compacte K de $\mathbf{C}^n$ (III, p. 10).

#### Exemple 3 {#evt-iv-s2-n5-exa-3 .statement}

Toute limite inductive stricte E d’une suite $(E_n)$ d’espaces de Montel (II, p. 36) telle que $E_n$ soit fermé dans $E_{n+1}$ pour tout n, est un espace de Montel ; en effet, E est séparé (II, p. 35, prop. 9, (i)), tonnelé (III, p. 25, cor. 3) et toute partie bornée de E est contenue dans un $E_n$ (III, p. 5, prop. 6) donc relativement compacte dans $E_n$, et par suite aussi dans E.

#### Exemple 4 {#evt-iv-s2-n5-exa-4 .statement}

\* Soit U un ouvert de $\mathbf{R}^n$ et soit $\mathcal{C}^\infty(U)$ l’espace de Fréchet des fonctions indéfiniment dérivables sur U (III, p. 9). Démontrons que c’est un espace de Montel. Comme $\mathcal{C}^\infty(U)$ est un espace de Fréchet, il est tonnelé (III, p. 25, corollaire). Soit B une partie bornée de $\mathcal{C}^\infty(U)$, et soit K une partie compacte de U. Pour tout $\alpha \in \mathbf{N}^n$, soit $H_{\alpha, K}$ l’ensemble des restrictions à K des fonctions $\partial^\alpha f$, où $f$ parcourt B. Soit $\alpha \in \mathbf{N}^n$; pour tout $\beta \in \mathbf{N}^n$ tel que $|\beta| = |\alpha| + 1$, l’ensemble $H_{\beta, K}$ est borné dans $\mathcal{C}(K)$ puisque B est borné dans $\mathcal{C}^\infty(U)$; d’après VAR, R., no 2.2.3, l’ensemble $H_{\alpha, K}$ est équicontinu, donc (TG, X, p. 17) relativement compact dans $\mathcal{C}(K)$. Or la topologie de $\mathcal{C}^\infty(U)$ est la moins fine des topologies rendant continues les applications $f \mapsto \partial^\alpha f|K$ de $\mathcal{C}^\infty(U)$ dans $\mathcal{C}(K)$, donc B est relativement compacte dans $\mathcal{C}^\infty(U)$ (TG, I, p. 26, prop. 3 et p. 64, corollaire).

De même, l’espace $\mathcal{C}_0^\infty(U)$ des fonctions indéfiniment dérivables à support compact dans U (III, p. 9) est un espace de Montel. En effet, $\mathcal{C}_0^\infty(U)$ est limite inductive stricte d’une suite d’espaces de Fréchet $\mathcal{C}_{H_n}^\infty(U)$ (III, p. 9), et il suffit de voir que chacun des espaces $\mathcal{C}_{H_n}^\infty(U)$ est un espace de Montel (Exemple 3). Mais une partie bornée et fermée de $\mathcal{C}_{H_n}^\infty(U)$ est bornée et fermée dans $\mathcal{C}^\infty(U)$, donc compacte dans $\mathcal{C}^\infty(U)$, et par suite dans $\mathcal{C}_{H_n}^\infty(U)$. \*

#### Proposition 8 {#evt-iv-s2-prop-8 .statement}

Soit E un espace de Montel et soit $\mathfrak{F}$ un filtre sur E, qui converge vers un point $x_0$ de E pour la topologie affaiblie. Si $\mathfrak{F}$ est à base dénombrable, ou contient un ensemble borné, alors $\mathfrak{F}$ converge aussi vers $x_0$ pour la topologie initiale.

Supposons d’abord qu’il existe dans $\mathfrak{F}$ un ensemble borné B. L’adhérence $\overline{B}$ de B pour la topologie initiale de E est bornée ; de plus, $\overline{B}$ est compacte car E est un espace de Montel. La topologie induite sur $\overline{B}$ par $\sigma(E, E')$ est séparée et moins fine que la topologie induite par la topologie initiale ; elles coïncident donc (TG, I, p. 63). La proposition est démontrée dans ce cas.

Supposons maintenant que $\mathcal{F}$ soit à base dénombrable. Il suffit (TG, I, p. 43, prop. 11) de considérer le cas d’une suite $(x_n)_{n \geq 1}$ tendant vers $x_0$ pour $\sigma(E, E')$. Soit B l’ensemble des $x_n$ pour $n \geq 0$. Il est borné pour $\sigma(E, E')$, donc aussi pour la topologie initiale (III, p. 28, cor. 3). On est donc ramené au premier cas de la démonstration.

*Tout espace de Montel est réflexif* : cela résulte de la déf. 4 et du th. 2 de IV, p. 16. En outre :

#### Proposition 9 {#evt-iv-s2-prop-9 .statement}

*Le dual fort d’un espace de Montel est un espace de Montel.*

Soient E un espace de Montel et $E'_b$ son dual fort. Comme E est réflexif, $E'_b$ est tonnelé (IV, p. 15, th. 1). Comme toute partie bornée de E est relativement compacte, la topologie forte sur $E'$ coïncide avec la topologie de la convergence compacte. Soit B une partie bornée de $E'_b$ ; elle est bornée pour la topologie faible $\sigma(E', E)$, donc équicontinue puisque E est tonnelé. Le th. d’Ascoli (TG, X, p. 17, corollaire, et p. 18, cor. 1) entraîne alors que l’adhérence de B pour $\sigma(E', E)$ est compacte pour la topologie de la convergence compacte, donc B est relativement compact dans $E'_b$.

#### Proposition 10 {#evt-iv-s2-prop-10 .statement}

*Tout espace de Montel métrisable est de type dénombrable.*

Soit E un espace de Montel métrisable. On sait (II, p. 5) que E s’identifie à un sous-espace d’un produit $F = \prod_{n \in \mathbf{N}} F_n$ d’une suite d’espaces normés, et l’on peut même supposer que l’on a $\mathrm{pr}_n(E) = F_n$ pour tout $n \in \mathbf{N}$. Si chacun des espaces métrisables $F_n$ est de type dénombrable, il en est de même de F (TG, IX, p. 19, corollaire), donc de E.

*Raisonnons par l’absurde*, en supposant par exemple que $F_0$ ne soit pas de type dénombrable. Notons $B_0$ la boule unité (fermée) dans $F_0$ ; c’est un espace métrique qui n’est pas de type dénombrable. Nous utiliserons le lemme suivant :

#### Lemme 1 {#evt-iv-s2-lem-1 .statement}

*Supposons que l’espace métrique X ne soit pas de type dénombrable. Il existe alors un nombre réel $\varepsilon > 0$ et une partie non dénombrable A de X tels que l’on ait $d(x, y) \geq \varepsilon$ pour $x, y$ distincts dans A.*

Pour tout entier $n \geq 1$, soit $\mathcal{F}_n$ l’ensemble (ordonné par inclusion) des parties D de X tels que l’on ait $d(x, y) \geq \frac{1}{n}$ pour $x, y$ distincts dans D. L’ensemble $\mathcal{F}_n$ est de caractère fini, donc possède un élément maximal $D_n$ (E, III, p. 35). Pour tout $y \in X$, il existe alors un point $x$ de $D_n$ tel que $d(x, y) < \frac{1}{n}$, vu le caractère maximal de $D_n$. Posons $D = \bigcup_n D_n$ ; l’ensemble D est donc dense dans X, et comme X n’est pas de type dénombrable, D n’est pas dénombrable, et l’un des $D_n$ n’est pas dénombrable.

C.Q.F.D.

D’après le lemme 1 appliqué à $B_0$, il existe une partie non dénombrable $A_0$ de $F_0$ et un nombre $\varepsilon > 0$ tels que l’on ait $\|x\| \leq 1$ et $\|x - y\| \geq \varepsilon$ pour $x, y$ distincts dans $A_0$. On a $\mathrm{pr}_0(E) = F_0$, et il existe donc une partie A de E telle que $\mathrm{pr}_0$ induise une bijection de A sur $A_0$.

#### Lemme 2 {#evt-iv-s2-lem-2 .statement}

Il existe une suite $(x_m)_{m \geq 0}$ bornée dans $E$, et formée d’éléments de $A$ deux à deux distincts.

Nous allons construire par récurrence une suite $(x_m)_{m \geq 0}$ de points de $A$, et une suite décroissante $(C_m)_{m \geq 0}$ de parties de $A$ satisfaisant aux conditions suivantes :
a) Aucun des ensembles $C_m$ n’est dénombrable.
b) Pour tout $m \geq 0$, l’ensemble $\operatorname{pr}_k(C_m)$ est borné dans $F_k$ pour $0 \leq k \leq m$.
c) On a $x_m \in C_m - C_{m+1}$ pour tout $m \geq 0$.

On pose $C_0 = A$. Supposons définis les ensembles $C_m$ pour $0 \leq m \leq n$, satisfaisant à a) et b) pour $0 \leq m \leq n$, et les points $x_m$ de $C_m - C_{m+1}$ pour $0 \leq m < n$.
Pour tout entier $r \geq 1$, soit $C_{n,r}$ l’ensemble des $x \in C_n$ tels que
$$
r - 1 \leq \| \operatorname{pr}_{n+1}(x) \| < r .
$$
Comme $C_n$ n’est pas dénombrable, il existe un entier $r \geq 1$ tel que $C_{n,r}$ ne soit pas dénombrable. Choisissons alors un point $x_n$ de $C_{n,r}$ et posons $C_{n+1} = C_{n,r} - \{ x_n \}$.
On a évidemment $C_{n+1} \subset C_n$ et $x_n \in C_n - C_{n+1}$, l’ensemble $C_{n+1}$ n’est pas dénombrable, et $\operatorname{pr}_k(C_{n+1})$ est borné dans $F_n$ pour $0 \leq k \leq n + 1$.

On a $x_m \in C_m$, d’où $x_m \in C_n$ dès que $m \geq n$. La projection de la suite $(x_m)_{m \geq 0}$ sur $F_n$ est donc bornée pour tout $n \geq 0$; autrement dit, la suite $(x_m)_{m \geq 0}$ est bornée dans $E$, et ceci établit le lemme 2.

C.Q.F.D.

Avec les notations du lemme 2, la suite bornée $(x_m)_{m \geq 0}$ admet une valeur d’adhérence $y$ dans $E$. La suite $(\operatorname{pr}_0(x_m))_{m \geq 0}$ admet donc la valeur d’adhérence $\operatorname{pr}_0(y)$ dans $F_0$, mais ceci contredit la construction de $A_0$.

#### Corollaire {#evt-iv-s2-n5-cor-1 .statement}

Soit $E$ un espace de Montel métrisable. Dans le dual fort de $E$, il existe un ensemble dénombrable dense.

Sur le dual $E'$ de $E$, la topologie forte est identique à celle de la convergence compacte, puisque $E$ est un espace de Montel. Il suffit donc d’appliquer le cor. 1 de la prop. 6 de III, p. 19.

On peut montrer que le dual fort d’un espace de Montel métrisable $E$ n’est pas métrisable si $E$ est de dimension infinie (IV, p. 58, exerc. 1).

## EXERCICES {#evt-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
