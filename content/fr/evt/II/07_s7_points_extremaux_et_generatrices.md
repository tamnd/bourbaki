---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 7
section_title: Points extrémaux et génératrices extrémales
lang: fr
source: evt-i-v-fr
book_pages: EVT II.57-EVT II.64, EVT II.92-EVT II.100
pdf_pages: 0092-0099, 0127-0135
extraction: ocr
subsections:
    - "no": 1
      title: Points extrémaux des ensembles convexes compacts
      page: 57
      pdf_page: 92
    - "no": 2
      title: Génératrices extrémales des cônes convexes
      page: 60
      pdf_page: 95
    - "no": 3
      title: Cônes convexes à semelle compacte
      page: 63
      pdf_page: 98
statements: 21
exercises: 5
content_sha256: d5ba8729e49a5c92f5deb98930280d399305ae7aa0e2ba2ff48dc698b66ef057
---

## § 7. POINTS EXTRÉMAUX ET GÉNÉRATRICES EXTRÉMALES

### 1. Points extrémaux des ensembles convexes compacts

#### Définition 1 {#evt-ii-s7-def-1 .statement}

Soit A un ensemble convexe dans un espace affine E. On dit qu’un point $x \in A$ est point extrémal de A s’il n’existe aucun segment ouvert contenu dans A et contenant x.

En d’autres termes, les relations $x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z$ et $0 \leq \lambda \leq 1$ entraînent $\lambda = 0$ ou $\lambda = 1$ (donc $x = y$ ou $x = z$). Cela entraîne que x ne peut être barycentre d’un ensemble de n points $x_i$ de A affectés de masses positives sans être égal à l’un d’eux : en effet, cela n’est autre que la définition pour $n = 2$; pour n quelconque, on raisonne par récurrence sur n, car x est barycentre de $x_1$ et du barycentre $y_1$ des $x_i$ pour $2 \leq i \leq n$, donc est égal à $x_1$ ou à $y_1$, et dans le second cas il suffit d’appliquer l’hypothèse de récurrence.

Dire que x est point extrémal de A signifie aussi que $A - \{x\}$ est convexe.

#### Exemple 1 {#evt-ii-s7-n1-exa-1 .statement}

Dans l’espace $\mathbf{R}^n$, tous les points de la sphère $S_{n-1}$ sont des points extrémaux de la boule fermée $B_n$. En effet, si $\sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1$ et $0 < \lambda < 1$, la relation
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
n’est possible que si
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1 .
$$

Mais cela entraîne $\sum_i (y_i - z_i)^2 = 0$, d’où $y_i = z_i$ pour tout $i$, ce qui prouve notre assertion.

#### Exemple 2 {#evt-ii-s7-n1-exa-2 .statement}

Dans l’espace normé $\mathcal{B}(\mathbf{N})$ des suites bornées de nombres réels (I, p. 4) les points extrémaux de la boule unité sont les points $x = (\xi_n)$ tels que $|\xi_n| = 1$ pour tout $n$. En effet, supposons que l’on ait $|\xi_n| \leq 1$ pour tout $n$ et $|\xi_p| < 1$ pour un indice $p$. On peut alors écrire

$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$

où $y$ (resp. $z$) est le point dont chacune des coordonnées est égale à la coordonnée de même indice de $x$, sauf pour la coordonnée d’indice $p$, égale à 1 (resp. – 1). Cela prouve que dans ce cas $x$ n’est pas extrémal, puisque l’on a $\|y\| \leq 1$ et $\|z\| \leq 1$. Inversement, si $|\xi_n| = 1$ pour tout $n$, $x$ est extrémal, car la relation $\xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n$ avec $|\eta_n| \leq 1$, $|\zeta_n| \leq 1$ et $0 < \lambda < 1$ entraîne $\xi_n = \eta_n = \zeta_n$.

#### Exemple 3 {#evt-ii-s7-n1-exa-3 .statement}

Soit $u : E \to E'$ une application affine d’un espace affine $E$ dans un espace affine $E'$; soient $C \subset E$, $C' \subset E'$ deux ensembles convexes tels que $u(C) \subset C'$. Si $x'$ est un point extrémal de $C'$ et $x$ un point extrémal de $u^{-1}(x') \cap C$, alors $x$ est un point extrémal de $C$, comme il résulte aussitôt de la déf. 1.

#### Proposition 1 {#evt-ii-s7-prop-1 .statement}

*Soient* $E$ *un espace localement convexe séparé*, $A$ *un ensemble convexe compact non vide dans* $E$, $B$ *l’ensemble des points extrémaux de* $A$, $f$ *une fonction convexe définie dans* $A$ *et semi-continue supérieurement*. *Alors* $f$ *atteint sa borne supérieure dans* $A$ *en un point de* $B$ *au moins*.

Nous désignerons par $\mathfrak{F}$ l’ensemble des parties $X$ de $A$ qui sont *fermées non vides*, *et telles que tout segment ouvert contenu dans* $A$ *et rencontrant* $X$ *soit contenu dans* $X$. On a les propriétés suivantes :

(i) $A$ appartient à $\mathfrak{F}$.

(ii) Pour qu’un point $a \in A$ soit tel que $\{a\} \in \mathfrak{F}$, il faut et il suffit que $a$ soit extrémal dans $A$.

(iii) Toute intersection non vide $X$ d’une famille $(X_\alpha)$ d’ensembles de $\mathfrak{F}$ appartient à $\mathfrak{F}$.

Les propriétés (i), (ii) et (iii) découlent aussitôt des définitions.

(iv) Soit $X \in \mathfrak{F}$, et soit $h$ une fonction convexe et semi-continue supérieurement dans $A$; alors l’ensemble $Y$ des points de $X$ où la restriction $h|X$ atteint sa borne supérieure dans $X$ appartient à $\mathfrak{F}$.

En effet, $h|X$ étant semi-continue supérieurement dans $X$ atteint au moins en un point de $X$ sa borne supérieure $\alpha$ dans cet ensemble (TG, IV, p. 30, th. 3); donc $Y$ est non vide et fermé (TG, IV, p. 29, prop. 1). D’autre part, soient $x, y$ deux points distincts de $A$, $z = \lambda x + (1 - \lambda) y$ un point de $Y$ tel que $0 < \lambda < 1$; comme $Y \subset X$ et $X \in \mathfrak{F}$, on a $x \in X$ et $y \in X$; d’autre part, comme $h$ est convexe, on a

$$
h(z) \geq \lambda h(x) + (1 - \lambda) h(y)
$$

mais comme $h(x) \leq \alpha, h(y) \leq \alpha$ et $h(z) = \alpha$, on a nécessairement $h(x) = h(y) = \alpha$, c’est-à-dire $x \in Y$ et $y \in Y$. Donc $Y \in \mathfrak{F}$.

Ces propriétés étant établies, soit $M$ l’ensemble des $x \in A$ où $f$ atteint sa borne supérieure dans $A$; en vertu de (iv), $M \in \mathfrak{F}$. D’autre part, en vertu de (iii) et du fait que les ensembles de $\mathfrak{F}$ sont fermés dans l’espace compact $A$, $\mathfrak{F}$ est *inductif* pour la relation d’ordre $\supset$. En vertu du th. 2 de E, III, p. 20, il existe donc un ensemble $N \subset M$ qui est un élément *minimal* de $\mathfrak{F}$. Montrons que $N$ est réduit à un seul point, ce qui démontrera la proposition. Puisque $E$ est un espace localement convexe séparé, il suffit de voir que pour toute forme linéaire continue $u$ sur $E$, $u$ est constante dans $N$ (II, p. 41, cor. 1). Or il résulte de (iv) que l’ensemble $N'$ des $x \in N$ où $u|N$ atteint sa borne supérieure dans $N$ appartient à $\mathfrak{F}$; puisque $N$ est minimal dans $\mathfrak{F}$, on a nécessairement $N' = N$.

#### Corollaire {#evt-ii-s7-n1-cor-1 .statement}

*Soient* $E$ *un espace localement convexe séparé*, $A$ *un ensemble convexe compact dans* $E$. *Tout hyperplan d’appui fermé* $H$ *de* $A$ *contient au moins un point extrémal de* $A$.

En effet, si $f(x) = \alpha$ est une équation de $H$ telle que $f(x) \leq \alpha$ dans $A$, il suffit d’appliquer la prop. 1 à $f$.

**Théorème 1** (Krein-Milman). — *Dans un espace localement convexe séparé* $E$, *tout ensemble convexe compact* $A$ *est l’enveloppe fermée convexe de l’ensemble de ses points extrémaux*.

En effet, soit $C$ l’enveloppe fermée convexe de l’ensemble des points extrémaux de $A$; il est clair que $C \subset A$. Pour voir que $A \subset C$, il suffit de prouver que, pour toute fonction linéaire affine $u$ continue dans $E$, telle que $u(x) \geq 0$ dans $C$, on a aussi $u(x) \geq 0$ dans $A$ (II, p. 41, cor. 4); mais cela résulte de la prop. 1 appliquée à $-u$.

#### Proposition 2 {#evt-ii-s7-prop-2 .statement}

*Soient* $A$ *un ensemble convexe compact dans un espace localement convexe séparé* $E$, $x$ *un point extrémal de* $A$. *Pour tout voisinage ouvert* $V$ *de* $x$ *dans* $E$, *il existe un demi-espace ouvert* $F$ *dans* $E$ *tel que* $x \in F \cap A \subset V \cap A$ *(en d’autres termes, les traces sur* $A$ *des demi-espaces ouverts contenant* $x$ *forment un système fondamental de voisinages de* $x$ *dans* $A$).

Pour tout demi-espace ouvert $D$ de $E$ contenant $x$, $A \cap \overline{D}$ est un voisinage compact de $x$ dans $A$, et l’intersection de tous ces voisinages est réduite à $x$ (deux points distincts étant séparés strictement par un hyperplan fermé (II, p. 41, prop. 4)). En vertu de TG, I, p. 60, prop. 1, il suffit de prouver que les ensembles $A \cap \overline{D}$ forment une *base de filtre*. Or, si l’on pose $L_D = A \cap (E - D)$, l’ensemble $L_D$ est convexe et compact et contenu dans l’ensemble convexe $A - \{x\}$; si $D_1, D_2$ sont deux demi-espaces ouverts de $E$ contenant $x$, l’enveloppe convexe $B$ de $L_{D_1} \cup L_{D_2}$ est donc contenue dans $A - \{x\}$; mais $B$ est un ensemble compact (II, p. 14, prop. 15) donc il existe un hyperplan fermé $H$ séparant strictement $x$ et $B$ (II, p. 41, prop. 4) et si $D$ est le demi-espace ouvert déterminé par $H$ et contenant $x$, on a $L_{D_1} \cup L_{D_2} \subset L_D$, donc $A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2})$.

#### Corollaire {#evt-ii-s7-n1-cor-2 .statement}

*Dans un espace localement convexe séparé*, *soient* $A$ *un ensemble convexe compact*, $K$ *une partie compacte de* $A$. *Les conditions suivantes sont équivalentes* :

$a)$ *A est l’enveloppe fermée convexe de* $K$.

b) K rencontre l’intersection de A et d’un quelconque de ses hyperplans d’appui.
c) K contient l’ensemble des points extrémaux de A.
a) ⇒ b). Supposons qu’il existe un hyperplan d’appui H de A d’équation $f(x) = \alpha$, tel que $(H \cap A) \cap K = \varnothing$ et supposons par exemple que $f(x) \geq \alpha$ dans A. Comme $f(x) - \alpha > 0$ pour tout $x \in K$ par hypothèse et que K est compact, on aurait
$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$
et K serait donc contenu dans le demi-espace fermé $f(x) \geq \beta$; il en serait donc de même de l’enveloppe fermée convexe A de K, ce qui est absurde.
b) ⇒ c). Supposons qu’un point extrémal $x$ de A n’appartienne pas à K ; il y aurait donc un voisinage V de $x$ dans E tel que $V \cap A \cap K = \varnothing$. Mais en vertu de la prop. 2, on peut supposer que V est un demi-espace ouvert déterminé par un hyperplan H d’équation $f(z) = \alpha$. Si par exemple $f(x) > \alpha$, on aurait $f(y) \leq \alpha$ pour tout $y \in K$, donc K ne rencontrerait pas l’intersection de A et de l’hyperplan d’appui d’équation $f(z) = \gamma > \alpha$ parallèle à H (II, p. 40, prop. 2); ce qui est absurde.
c) ⇒ a). C’est une conséquence évidente du th. de Krein-Milman.

#### Remarque 1 {#evt-ii-s7-n1-rem-1 .statement}

Même dans un espace vectoriel E de dimension finie, l’ensemble des points extrémaux d’un ensemble convexe compact n’est pas nécessairement fermé (II, p. 94, exerc. 11).
2) Dans un espace localement convexe séparé non complet, si K est un ensemble compact dont l’enveloppe fermée convexe A ne soit pas compacte, il peut y avoir des points extrémaux de A qui n’appartiennent pas à K (II, p. 92, exerc. 2).
3) Dans un espace de Banach E de dimension infinie, il peut se faire que la boule fermée de centre 0 et de rayon 1 ne possède aucun point extrémal (II, p. 94, exerc. 14).
4) Si A est un ensemble convexe compact dans un espace localement convexe séparé, il peut se faire qu’un point extrémal de A n’appartienne à aucun hyperplan d’appui de A (II, p. 83, exerc. 11). La démonstration du th. 1 (II, p. 59) montre en tout cas que A est l’enveloppe fermée convexe de l’ensemble des points extrémaux de A appartenant à un hyperplan d’appui.

### 2. Génératrices extrémales des cônes convexes

Dans un espace vectoriel E, soit C un cône convexe de sommet 0 ; il est clair qu’il ne peut exister dans C de point extrémal autre que le sommet ; ce dernier est point extrémal de C si et seulement si C est pointé et saillant.

#### Définition 2 {#evt-ii-s7-def-2 .statement}

Dans un espace vectoriel E, soit C un cône convexe de sommet 0. On dit qu’une demi-droite $D \subset C$ d’origine 0 est une génératrice extrémale de C si tout segment ouvert contenu dans C, ne contenant pas 0 et rencontrant D est contenu dans D.

Il revient au même de dire que pour tout $x \in D$ tel que $x \neq 0$, si $y \neq 0, y' \neq 0$ sont deux points de C tels que $x = y + y'$, on a nécessairement $y \in D$ et $y' \in D$.

#### Remarque 1 {#evt-ii-s7-n2-rem-1 .statement}

Soit C un cône convexe pointé saillant dans E, et considérons sur E la structure d’ordre pour laquelle C est l’ensemble des éléments $\geqslant 0$ (II, p. 13, prop. 13); pour qu’un élément $x > 0$ de E appartienne à une génératrice extrémale de C, *il faut et il suffit que tout élément $y \geqslant 0$ majoré par $x$ soit de la forme $\lambda x$, avec $0 \leqslant \lambda \leqslant 1$* : en effet, dire que $y$ est majoré par $x$ signifie que $x = y + y'$ avec $y' \in C$, d’où la conclusion.

#### Proposition 3 {#evt-ii-s7-prop-3 .statement}

*Dans un espace vectoriel E, soient C un cône convexe de sommet 0, $x_0 \neq 0$ un point de C, D une demi-droite contenue dans C, d’origine 0 et contenant $x_0$, H un hyperplan contenant $x_0$ et ne passant pas par 0. Pour que D soit génératrice extrémale de C, il faut et il suffit que $x_0$ soit point extrémal de $H \cap C$.*

La condition est évidemment nécessaire. Inversement, supposons-la satisfaite ; supposons qu’il existe une droite $D'$ ne contenant pas D, passant par $x_0$ et telle que $D' \cap C$ contienne un segment ouvert auquel appartienne $x_0$. Soit $y \neq 0$ un vecteur directeur de $D'$; les hypothèses entraînent que le point $(1 + \lambda)x_0 + \mu y$ appartient à C pour $|\lambda|$ et $|\mu|$ assez petits. Mais alors, dans le plan P déterminé par D et $D'$ et muni de sa topologie canonique, $x_0$ est point intérieur de $P \cap C$, et par suite la droite $P \cap H$ contient un segment ouvert contenu dans $H \cap C$ et auquel appartient $x_0$, ce qui contredit l’hypothèse.

#### Définition 3 {#evt-ii-s7-def-3 .statement}

*Soit C un ensemble convexe dans un espace vectoriel topologique séparé E. On appelle chapeau de C toute partie convexe compacte non vide A de C telle que le complémentaire $C - A$ de A dans C soit convexe.*

Soient C un cône convexe pointé de sommet 0 dans E, A un chapeau de C et $B = C - A$. Pour toute demi-droite fermée $L \subset C$ d’origine 0, $L \cap A$ et $L \cap B$ sont des parties convexes complémentaires dans L, de réunion L, et $L \cap A$ est compacte. Comme $L \cap A$ est non vide pour au moins une demi-droite L, on voit que $0 \in A$, donc $L \cap A$ est un *segment fermé d’origine 0*.

#### Proposition 4 {#evt-ii-s7-prop-4 .statement}

*Soient E un espace localement convexe séparé, C un cône convexe pointé de sommet 0 dans E.*

a) *Soit A un chapeau de C. Soit p la restriction à C de la jauge de A (II, p. 22). L’ensemble des $x \in C$ tels que $p(x) \leqslant 1$ est égal à A. La fonction p est semi-continue inférieurement et possède les propriétés suivantes :*
(i) *Quels que soient x, y dans C, on a $p(x + y) = p(x) + p(y)$.*
(ii) *Quels que soient $x \in C$ et $\lambda \in \mathbf{R}_+^*$, on a $p(\lambda x) = \lambda p(x)$.*
(iii) *Si $x \in C$, la relation $p(x) = 0$ équivaut à $x = 0$.*

b) *Inversement, soit p une fonction définie dans C, à valeurs dans $[0, + \infty]$, satisfaisant aux conditions (i), (ii) de a). Soit A l’ensemble des $x \in C$ tels que $p(x) \leqslant 1$. Alors A et $C - A$ sont convexes. Pour que A soit un chapeau, il suffit donc que A soit compact et non vide.*

L’assertion b) est évidente. Les propriétés énoncées dans a) sont des conséquences des remarques précédant la prop. 4, et des prop. 22 de II, p. 21 et 23 de II, p. 22, à l’exception de l’inégalité

$$
p(x + y) \geqslant p(x) + p(y) .
$$

Il suffit de démontrer cette dernière lorsque $x \neq 0$ et $y \neq 0$; on a donc $p(x) > 0$, $p(y) > 0$. Soient $\lambda, \mu$ deux nombres $> 0$ tels que $\lambda < p(x), \mu < p(y)$, et notons B le complémentaire de A dans C. On a $x \in \lambda B, y \in \mu B$, donc $x + y \in \lambda B + \mu B$; en vertu de la convexité de B, on a $\lambda B + \mu B \subset (\lambda + \mu) B$, d’où $p(x + y) > \lambda + \mu$, ce qui entraîne l’inégalité annoncée.

#### Corollaire 1 {#evt-ii-s7-prop-4-cor-1 .statement}

Soient E un espace localement convexe séparé, C un cône convexe pointé de sommet 0 dans E, A un chapeau de C, p la jauge de A. Les points extrémaux de A sont alors : le point 0, et les points x situés sur les génératrices extrémales de C et tels que $p(x) = 1$.

Il est clair que 0 est un point extrémal de A. Soit x un point situé sur une génératrice extrémale L de C et tel que $p(x) = 1$. Soient y, z deux points de A tels que $x = \frac{1}{2}(y + z)$. Comme L est extrémale, on a $y = \lambda x$ et $z = \mu x$, où $\lambda$ et $\mu$ sont des nombres $\geq 0$ tels que $\frac{1}{2}(\lambda + \mu) = 1$, $\lambda = \lambda p(x) = p(y) \leq 1$ et $\mu = \mu p(x) = p(z) \leq 1$, d’où $\lambda = \mu = 1$ et par suite $y = z = x$; ainsi, x est point extrémal de A. Réciproquement, soit $x \neq 0$ un point extrémal de A. Il est clair que $p(x) = 1$. Soient y, $y'$ deux points de C tels que $x = y + y'$, et montrons que y, $y'$ sont proportionnels à x. On peut se limiter au cas où les nombres $\lambda = p(y)$ et $\lambda' = p(y')$ sont finis et $> 0$. Alors $\lambda^{-1} y \in A, \lambda'^{-1} y' \in A, \lambda + \lambda' = 1$ en vertu de la prop. 4, (i), et l’égalité $x = \lambda (\lambda^{-1} y) + \lambda' (\lambda'^{-1} y')$ entraîne par hypothèse
$$
x = \lambda^{-1} y = \lambda'^{-1} y'.
$$

#### Corollaire 2 {#evt-ii-s7-prop-4-cor-2 .statement}

Tout point de C qui appartient à un chapeau de C appartient à l’enveloppe fermée convexe de la réunion des génératrices extrémales de C.

Ceci résulte aussitôt du cor. 1, et du th. de Krein-Milman (II, p. 59, th. 1).

\* Exemple. — Soit X un espace localement compact dénombrable à l’infini. Soit C un cône convexe fermé de sommet 0 dans $\mathcal{M}_+(X)$ muni de la topologie vague. Montrons que C est réunion de ses chapeaux. Soit $(X_n)$ une suite croissante de parties ouvertes relativement compactes de X, de réunion X. Soit $\mu$ un élément $\neq 0$ de C. Il existe des $\alpha_n > 0$ tels que $\sum_n \alpha_n \mu(X_n) = 1$. Pour toute mesure $\nu \in C$, posons $p(\nu) = \sum_n \alpha_n \nu(X_n) \in [0, + \infty]$. La fonction p sur C satisfait aux conditions (i) et (ii) de la prop. 4. Elle est semi-continue inférieurement pour la topologie vague (INT, IV, 2e éd., § 1, n° 1, prop. 4). L’ensemble A des $\gamma \in C$ tels que $p(\gamma) \leq 1$ est donc fermé non vide. D’autre part, comme toute partie compacte de X est contenue dans l’un des $X_n$, A est vaguement borné, donc vaguement compact (INT, III, 2e éd., § 1, n° 9, prop. 15). L’ensemble A est donc un chapeau de C contenant $\mu$. \*

#### Proposition 5 {#evt-ii-s7-prop-5 .statement}

Soient E un espace faible séparé, C un cône convexe saillant de sommet 0 dans E ; on suppose que C est complet pour la structure uniforme induite par celle de E, et que 0 admet un système fondamental dénombrable de voisinages dans C. Alors C est réunion de ses chapeaux et est l’enveloppe fermée convexe de la réunion de ses génératrices extrémales.

La seconde assertion est conséquence de la première et du cor. 2 de II, p. 62. Utilisant la prop. 11 de II, p. 56, on est ramené au cas où $E = \mathbf{R}^1$ et $C \subset \mathbf{R}_+^1$. Pour tout $\alpha \in I$, désignons par $f_\alpha$ la projection $pr_\alpha$ dans $E$, qui est une forme linéaire continue. Soit d’autre part $(V_n)_{n \in \mathbf{N}}$ un système fondamental dénombrable de voisinages de 0 dans $C$. Par définition de la topologie de $E$, pour chaque $n \in \mathbf{N}$, il existe une partie finie $J_n$ de $I$ et un nombre $\varepsilon_n > 0$ tels que $V_n$ contienne l’ensemble $W_n$ des $x \in C$ tels que $f_\alpha(x) \leq \varepsilon_n$ pour tout $\alpha \in J_n$; posons $J = \bigcup_{n \in \mathbf{N}} J_n$. Soient $y \neq 0$ un point de $C$, et $p$ la fonction $\sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C)$ où les $\lambda_\alpha > 0$ sont choisis de sorte que $p(y) = 1$; cela est possible, car si l’on avait $f_\alpha(y) = 0$ pour tout $\alpha \in J$, on en conclurait que $y \in V_n$ pour tout $n$, d’où $y = 0$, contrairement à l’hypothèse. Remarquons maintenant que pour tout $\alpha \in I$, $f_\alpha|C$ est continue au point 0, donc il y a un $n \in \mathbf{N}$ tel que $f_\alpha$ soit bornée dans un $W_n$, donc majorée dans $C$ par une combinaison linéaire d’un nombre fini de fonctions $f_\beta|C$, où $\beta \in J$. Il en résulte que si $A$ est l’ensemble des $x \in C$ tels que $p(x) \leq 1$, $f_\alpha$ est bornée dans $A$ pour tout $\alpha \in I$. Comme $p$ est semi-continue inférieurement dans $C$, $A$ est fermé non vide dans $C$, et par suite compact. Comme il est clair que $p$ vérifie les conditions (i) et (ii) de la prop. 4 de II, p. 61, $A$ est un chapeau dans $C$ et contient $y$.

#### Remarque 2 {#evt-ii-s7-n2-rem-2 .statement}

Il existe des cônes convexes saillants faiblement complets qui n’ont aucune génératrice extrémale (II, p. 97, exerc. 31).

### 3. Cônes convexes à semelle compacte

#### Proposition 6 {#evt-ii-s7-prop-6 .statement}

Soient $E$ un espace localement convexe séparé, $K$ un ensemble convexe compact dans $E$, ne contenant pas 0. Alors le plus petit cône pointé $C$ de sommet 0 contenant $K$ est un cône convexe saillant dans $E$ et un sous-espace localement compact et complet de $E$; en outre, il existe dans $E$ un hyperplan fermé $H$ ne contenant pas 0, tel que $H$ rencontre toutes les demi-droites d’origine 0 contenues dans $C$ et que $H \cap C$ soit compact. De plus, pour tout hyperplan fermé $H$ ayant ces propriétés, si $D$ est le demi-espace fermé déterminé par $H$ et contenant 0, $C \cap D$ est un chapeau de $C$ et $C$ est la réunion des $\lambda(C \cap D)$ pour $\lambda > 0$.

En vertu de la prop. 4 de II, p. 41, il existe un hyperplan fermé $H$ qui sépare strictement 0 et $K$. D’autre part, l’enveloppe convexe $A$ de la réunion de $\{0\}$ et de $K$ est compacte (II, p. 14, prop. 15), et c’est la réunion des $\lambda K$ pour $0 \leq \lambda \leq 1$. Comme 0 et $K$ sont strictement de part et d’autre de $H$, pour tout $x \in K$ il existe un $\lambda$ tel que $0 < \lambda < 1$ et $\lambda x \in H$. Comme $C$ est la réunion des $\lambda A$ pour $\lambda \geq 1$, on voit déjà que $H$ rencontre toute demi-droite d’origine 0 contenue dans $C$ et que $H \cap A = H \cap C$ est compact. En outre, $C$ est aussi la réunion des $\lambda(H \cap C)$ pour $\lambda \geq 0$; soit $C_n$ la réunion des $\lambda(H \cap C)$ pour $0 \leq \lambda \leq n$. Il est clair que $C_n$ est l’enveloppe convexe de la réunion de $\{0\}$ et de $n(H \cap C)$, donc est compact. En outre, pour tout $x \in E$, il existe un voisinage fermé $V$ de $x$ dans $E$ et un entier $n$ tels que $V \cap C \subset C_n$ : en effet, si $H$ est défini par l’équation $f(z) = \alpha$, où $\alpha > 0$, il suffit de prendre pour $V$ le demi-espace fermé déterminé par $nH$ et contenant 0, où n est pris assez grand pour que $n\alpha > f(x)$. Ceci montre que C est localement compact (en prenant $x \in C$), et qu’il est fermé dans E. D’ailleurs, on peut aussi considérer K comme une partie du complété $\hat{E}$, donc C est aussi fermé dans $\hat{E}$, et par suite complet.

On appelle *semelle* d’un cône C dans un espace vectoriel topologique séparé E l’intersection de C et d’un hyperplan fermé H ne contenant pas le sommet s de C, tel que C soit le plus petit cône de sommet s contenant H $\cap$ C. La prop. 6 montre que dans un espace localement convexe séparé E, le plus petit cône de sommet 0 contenant un ensemble compact convexe K auquel 0 n’appartient pas, est un *cône à semelle compacte*, et que tout cône convexe ayant une semelle compacte S est localement compact et complet.

#### Exemple 1 {#evt-ii-s7-n3-exa-1 .statement}

Dans un espace vectoriel de dimension finie E, tout cône convexe fermé saillant a une semelle compacte. En effet, en vertu de II, p. 56, prop. 11, on peut se borner au cas où $E = \mathbf{R}^n$ et $C = \mathbf{R}^n_+$. Si $(e_i)_{1 \leq i \leq n}$ est la base canonique de $\mathbf{R}^n$, il est clair que l’ensemble convexe compact, enveloppe convexe des $e_i$ ($1 \leq i \leq n$) est une semelle compacte pour $\mathbf{R}^n_+$.

#### Exemple 2 {#evt-ii-s7-n3-exa-2 .statement}

Si X est un espace compact, le cône $\mathcal{M}_+(X)$ des mesures positives sur X, muni de la topologie vague, est un cône à semelle compacte (INT, III, 2e éd., § 1, no 9, cor. 3 de la prop. 15). \*

## EXERCICES {#evt-ii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
