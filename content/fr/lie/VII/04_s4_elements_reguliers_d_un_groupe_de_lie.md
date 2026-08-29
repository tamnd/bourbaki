---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 4
section_title: Eléments réguliers d’un groupe de Lie
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0027-0034, 0057-0058
extraction: ocr
subsections:
    - "no": 1
      title: Eléments réguliers pour une représentation linéaire
      page: 0
      pdf_page: 27
    - "no": 2
      title: Eléments réguliers d’un groupe de Lie
      page: 0
      pdf_page: 29
    - "no": 3
      title: Relations avec les éléments réguliers de l’algèbre de Lie
      page: 0
      pdf_page: 30
    - "no": 4
      title: Application aux automorphismes élémentaires
      page: 0
      pdf_page: 33
statements: 18
exercises: 4
content_sha256: 5667ae0fbb8b281fd7472fa139995aa1d1ba9dce33920fdf7a31ab895e4b113d
---

## § 4. Eléments réguliers d’un groupe de Lie

Dans les n°s 1, 2 et 3 de ce paragraphe, on suppose que $k$ est $\mathbf{R}$, ou $\mathbf{C}$, ou un corps ultramétrique complet non discret de caractéristique zéro. On désigne par $G$ un groupe de Lie de dimension finie sur $k$, par $\mathfrak{g}$ son algèbre de Lie, par $e$ son élément neutre. Si $a \in G$, on note $g^1(a)$ le nilespace de $\mathrm{Ad}(a) - 1$, autrement dit l’espace $g^1(\mathrm{Ad}(a))$ (cf. § 1, n° 1).

### 1. Eléments réguliers pour une représentation linéaire

#### Lemme 1 {#lie-vii-s4-lem-1 .statement tag=00VU}

Soient $M$ une variété analytique sur $k$ et $a = (a_0, \ldots, a_{n-1}, a_n = 1)$ une suite de fonctions analytiques sur $M$. Pour tout $x \in M$, soit $r_a(x)$ la borne supérieure des $i \in \{0, n\}$ tels que $a_j(x) = 0$ pour $j < i$ et soit $r_a^0(x)$ la borne supérieure des $i \in \{0, n\}$ tels que $a_j$ soit nulle sur un voisinage de $x$ pour $j < i$.

(i) La fonction $r_a$ est semi-continue supérieurement.
(ii) Pour tout $x \in M$, $r_a^0(x) = \liminf_{y \to x} r_a(y)$.
(iii) La fonction $r_a^0$ est localement constante.
(iv) L’ensemble des points $x \in M$ tels que $r_a^0(x) = r_a(x)$ est l’ensemble des points de $M$ au voisinage desquels la fonction $r_a$ est constante. C’est un ouvert dense dans $M$. Si $k = \mathbf{C}$ et si $M$ est connexe de dimension finie, cet ouvert est connexe.

(i) Si $r_a(x) = i$, alors $a_i(x) \neq 0$ et pour tout $y$ appartenant à un voisinage de $x$, on a $a_i(y) \neq 0$, donc $r_a(y) \leq i$.
(ii) Si $r_a^0(x) = i$, alors les fonctions $a_0, \ldots, a_{i-1}$ sont nulles sur un voisinage de $x$ et, pour tout point $y$ appartenant à ce voisinage, on a $r_a(y) \geq i$. Par conséquent, $\liminf_{y \to x} r_a(y) \geq i$. Tout voisinage de $x$ contient un point $y$ tel que $a_i(y) \neq 0$ et par suite $r_a(y) \leq i$. On a donc $\liminf_{y \to x} r_a(y) = i$.
(iii) Soit $i = r_a^0(x)$ et soit $V$ un voisinage de $x$ tel que $a_j(y) = 0$ pour tout $y \in V$ et tout $j < i$. On a $x \in M - Z$ où $Z$ désigne l’ensemble des points de $M$ au voisinage desquels la fonction $a_i$ est nulle. Puisque $Z$ est fermé dans $M$ (VAR, R, 5.3.5), $V \cap (M - Z)$ est un voisinage de $x$. Pour tout point $y$ appartenant à ce voisinage, on a $r_a^0(y) = i$.
(iv) La fonction $r_a - r_a^0$ est semi-continue supérieurement et sa valeur en tout point est $\geq 0$. Si $r_a(x) = r_a^0(x)$, alors $r_a - r_a^0$ est nulle au voisinage de $x$, ce qui montre que $r_a$ est constante au voisinage de $x$ d’après (iii). Réciproquement, si $r_a$ est constante au voisinage de $x$, on a $r_a^0(x) = r_a(x)$ d’après (ii). L’ensemble des points $x \in M$ tels que $r_a^0(x) = r_a(x)$ est donc un ouvert $\Omega$ de $M$. Si $x \in M$ et si r_a^0(x) < r_a(x), tout voisinage de x contient un point y tel que $r_a(y) < r_a(x)$ et $r_a^0(y) = r_a^0(x)$. Tout voisinage de x contient donc un point y tel que

$$
r_a(y) - r_a^0(y) < r_a(x) - r_a^0(x).
$$

Il en résulte que $\Omega$ est dense dans M.

Si M est connexe et si $p$ est la valeur de $r_a^0$ sur M, les points de $\Omega$ sont les points $x \in M$ tels que $a_p(x) \neq 0$. Si $k = \mathbf{C}$, ceci entraîne que $\Omega$ est connexe d’après le lemme 3 de l’Appendice II.

Soit $\rho$ une représentation linéaire analytique de G dans un espace vectoriel V de dimension finie n sur k. Posons

$$
\det(T - \rho(g) + 1) = a_0(g) + a_1(g)T + \cdots + a_{n-1}(g)T^{n-1} + T^n.
$$

Les fonctions $r_a$ et $r_a^0$ associées à la suite $(a_0, a_1, \ldots, a_{n-1}, 1)$ seront notées respectivement $r_\rho$ et $r_\rho^0$. On a alors, pour tout $g \in G$:

$$
r_\rho(g) = \dim V^1(\rho(g)) \\
r_\rho^0(g) = \liminf_{g' \to g} \dim V^1(\rho(g')).
$$

#### Lemme 2 {#lie-vii-s4-lem-2 .statement tag=00VV}

Soit $0 \to V' \to V \to V'' \to 0$ une suite exacte de G-modules définis respectivement par les représentations linéaires analytiques $\rho', \rho, \rho''$ de G. On a alors:

$$
r_\rho = r_{\rho'} + r_{\rho''} \quad \text{et} \quad r_\rho^0 = r_{\rho'}^0 + r_{\rho''}^0.
$$

En effet, pour tout $g \in G$, on a (§ 1, n° 1, cor. 3 du th. 1) une suite exacte

$$
0 \to (V')^1(\rho'(g)) \to V^1(\rho(g)) \to (V'')^1(\rho''(g)) \to 0,
$$

ce qui prouve la première assertion. La seconde en résulte puisque, d’après le lemme 1 (iv), sur un ouvert dense de G, on a $r_\rho^0 = r_\rho, r_{\rho'}^0 = r_{\rho'},$ et $r_{\rho''}^0 = r_{\rho''}$.

#### Définition 1 {#lie-vii-s4-def-1 .statement tag=00VW}

Un élément $g \in G$ est dit régulier pour la représentation linéaire $\rho$ si $r_\rho(g) = r_\rho^0(g)$.

#### Proposition 1 {#lie-vii-s4-prop-1 .statement tag=00VX}

Les points réguliers pour une représentation linéaire analytique $\rho$ de G sont les points de G au voisinage desquels la fonction $r_\rho$ est constante. Ils forment un ouvert dense dans G. Si $k = \mathbf{C}$ et si G connexe, l’ensemble des points réguliers pour $\rho$ est connexe.

Cela résulte du lemme 1 (iv).

#### Remarque {#lie-vii-s4-n1-rem-1 .statement tag=00VY}

Soit $G^*$ un sous-groupe ouvert de G. Pour qu’un élément $a \in G^*$ soit un élément régulier de G pour la représentation linéaire $\rho$ de G, il faut et il suffit que ce soit un élément régulier de $G^*$ pour la représentation linéaire $\rho|G^*$.

### 2. Eléments réguliers d’un groupe de Lie

#### Définition 2 {#lie-vii-s4-def-2 .statement tag=00VZ}

On dit qu’un élément de G est régulier s’il est régulier pour la représentation adjointe de G.

En d’autres termes (prop. 1), un élément $g \in G$ est régulier si, pour tous les éléments $g'$ d’un voisinage de $g$ dans $G$, la dimension du nilespace de $\mathrm{Ad}(g') - 1$ est égale à la dimension du nilespace de $\mathrm{Ad}(g) - 1$.

#### Proposition 2 {#lie-vii-s4-prop-2 .statement tag=00W0}

Soient $G'$ un groupe de Lie de dimension finie sur $k$ et $f$ un morphisme surjectif de $G$ dans $G'$. L’image par $f$ d’un élément régulier de $G$ est un élément régulier de $G'$. Si le noyau de $f$ est contenu dans le centre de $G$, pour qu’un élément $g \in G$ soit régulier, il faut et il suffit que $f(g)$ soit régulier.

Soient en effet $g'$ l’algèbre de Lie de $G'$ et $\mathfrak{h}$ l’idéal de $g$ noyau de $Tf|_g$. Soit $\rho$ la représentation linéaire de $G$ dans $\mathfrak{h}$, définie par $\rho(g) = \mathrm{Ad}\,g|\mathfrak{h}$ pour tout $g \in G$, et soit $\mathrm{Ad} \circ f$ la représentation linéaire de $G$ dans $g'$ composée de $f$ et de la représentation adjointe de $G'$. Ces représentations linéaires définissent une suite exacte de $G$-modules : $0 \to \mathfrak{h} \to g \to g' \to 0$. D’après le lemme 2, on a $r_{\mathrm{Ad}} = r_\rho + r_{\mathrm{Ad} \circ f}$ et $r_{\mathrm{Ad}}^0 = r_\rho^0 + r_{\mathrm{Ad} \circ f}^0$. Puisque $r_{\mathrm{Ad} \circ f} = r_{\mathrm{Ad}} \circ f$ et que $f$ est une application ouverte, on a $r_{\mathrm{Ad} \circ f}^0 = r_{\mathrm{Ad}}^0 \circ f$. Par conséquent :

$$
r_{\mathrm{Ad}} - r_{\mathrm{Ad}}^0 = r_\rho - r_\rho^0 + (r_{\mathrm{Ad}} - r_{\mathrm{Ad}}^0) \circ f.
$$

Si $g$ est régulier, on a donc $(r_{\mathrm{Ad}} - r_{\mathrm{Ad}}^0)(f(g)) = 0$ ce qui signifie que $f(g)$ est régulier. Si le noyau de $f$ est contenu dans le centre de $G$, alors

$$
r_\rho(g) = r_\rho^0(g) = \dim \mathfrak{h}
$$

pour tout $g \in G$. Par suite, si $f(g)$ est régulier, on a $r_{\mathrm{Ad}}(g) = r_{\mathrm{Ad}}^0(g)$, autrement dit, $g$ est régulier.

#### Proposition 3 {#lie-vii-s4-prop-3 .statement tag=00W1}

Soient $G_1$ et $G_2$ deux groupes de Lie de dimension finie sur $k$. Pour qu’un élément $(g_1, g_2)$ de $G_1 \times G_2$ soit régulier, il faut et il suffit que $g_1$ et $g_2$ soient respectivement des éléments réguliers de $G_1$ et $G_2$.

La condition est nécessaire d’après la prop. 2. Montrons qu’elle est suffisante. Pour tout $g = (g_1, g_2) \in G_1 \times G_2$, on a $r_{\mathrm{Ad}}(g) = r_{\mathrm{Ad}}(g_1) + r_{\mathrm{Ad}}(g_2)$. Compte tenu du lemme 1, (ii), il en résulte que $r_{\mathrm{Ad}}^0(g) = r_{\mathrm{Ad}}^0(g_1) + r_{\mathrm{Ad}}^0(g_2)$. Si $g_1$ et $g_2$ sont réguliers, $r_{\mathrm{Ad}}^0(g_1) = r_{\mathrm{Ad}}(g_1)$ et $r_{\mathrm{Ad}}^0(g_2) = r_{\mathrm{Ad}}(g_2)$, donc $r_{\mathrm{Ad}}^0(g) = r_{\mathrm{Ad}}(g)$, ce qui signifie que $g$ est régulier.

#### Lemme 3 {#lie-vii-s4-lem-3 .statement tag=00W2}

Soient $a \in G$ et $m$ un supplémentaire de $g^1(a)$ dans $g$. Soient $U$ un voisinage de $0$ dans $g$ et exp une application exponentielle de $U$ dans $G$. L’application

$$
f : (x, y) \mapsto (\exp y)a(\exp x)(\exp y)^{-1}
$$

de $(g^1(a) \times m) \cap U$ dans $G$ est étale en $(0, 0)$.

Les applications $x \mapsto a(\exp x)$ et $y \mapsto (\exp y)a(\exp y)^{-1}$ ont respectivement pour applications linéaires tangentes en 0 les applications $x \mapsto ax$ et $y \mapsto ya - ay = a(a^{-1}ya - y)$ de $g$ dans $T_aG = ag$ (III, § 3, n° 12, prop. 46). Par suite, l’application tangente à $f$ en $(0, 0)$ est l’application $(x, y) \mapsto ax + a(a^{-1}ya - y) = a(x + a^{-1}ya - y)$ de $g^1(a) \times m$ dans $ag$. Cette application est injective. En effet, si $x \in g^1(a), y \in m$ et si $x + a^{-1}ya - y = 0$, alors $(\mathrm{Ad}(a) - 1)y = \mathrm{Ad}(a)x \in g^1(a)$ puisque $\mathrm{Ad}(a)g^1(a) \subset g^1(a)$. Ceci entraîne que $y \in g^1(a)$ et par suite que $y = 0$. Puisque $\mathrm{Ad}(a)$ est injectif sur $g^1(a)$, il en résulte que $x = 0$. Puisque $\dim g = \dim g^1(a) + \dim m$, ceci montre que $f$ est étale en $(0, 0)$.

#### Proposition 4 {#lie-vii-s4-prop-4 .statement tag=00W3}

*Soient $a \in G$ et $H$ un sous-groupuscule de Lie de $G$ ayant $g^1(a)$ pour algèbre de Lie. L’application $(b, c) \mapsto cabc^{-1}$ de $H \times G$ dans $G$ est une submersion en $(e, e)$*.

Soient en effet $m$ un supplémentaire de $g^1(a)$ dans $g$ et exp une application exponentielle de $G$ définie sur un voisinage ouvert $U$ de 0 dans $g$. On peut choisir $U$ de sorte que $\exp(U \cap g^1(a)) \subset H$. L’application $f : (x, y) \mapsto (\exp x, \exp y)$ est alors une application analytique d’un voisinage de $(0, 0)$ dans $g^1(a) \times m$ à valeurs dans $H \times G$. D’après le lemme 3, l’application composée de $f$ et de l’application $\varphi : (b, c) \mapsto cabc^{-1}$ est étale en $(0, 0)$. Il en résulte que $\varphi$ est une submersion en $f(0, 0) = (e, e)$.

#### Proposition 5 {#lie-vii-s4-prop-5 .statement tag=00W4}

*Soient $a \in G$ et $W$ un voisinage de $e$ dans $G$. Il existe un voisinage $V$ de $a$ ayant la propriété suivante : pour tout $a' \in V$, il existe un élément $g \in W$ tel que $g^1(a') \subset \mathrm{Ad}(g)g^1(a)$*.

Posons $g^1 = g^1(a)$ et soit $g = g^1 + g^+$ la décomposition de Fitting de $\mathrm{Ad}(a) - 1$ (§ 1, n° 1). Soit $H$ un sous-groupuscule de Lie de $G$ ayant $g^1$ pour algèbre de Lie. Pour tout $h \in H$, on a $\mathrm{Ad}(h)g^1 \subset g^1$. Puisque $[g^1, g^+] \subset g^+$, il existe un voisinage $U$ de $e$ dans $H$ tel que $\mathrm{Ad}(h)g^+ \subset g^+$ pour tout $h \in U$. Puisque la restriction de $\mathrm{Ad}(a) - 1$ à $g^+$ est bijective, on peut choisir $U$ de sorte que, pour tout $h \in U$, la restriction de $\mathrm{Ad}(ah) - 1$ à $g^+$ soit bijective. On a alors $g^1(ah) \subset g^1(a) = g^1$ pour tout $h \in U$. D’après la proposition 4, $\mathrm{Int}(W)(aU)$ est un voisinage de $a$ dans $G$. Si $a' \in \mathrm{Int}(W)(aU)$, alors $a' = g(ah)g^{-1}$ avec $g \in W$ et $h \in U$; il en résulte que $g^1(a') = \mathrm{Ad}(g)g^1(ah) \subset \mathrm{Ad}(g)g^1(a)$.

#### Corollaire {#lie-vii-s4-n2-cor-1 .statement tag=00W5}

*Soit $G^*$ un sous-groupe ouvert de $G$. Si $a \in G$ est régulier, il existe un voisinage $V$ de $a$ tel que, pour tout $a' \in V$, $g^1(a')$ soit conjugué de $g^1(a)$ par $\mathrm{Ad}(G^*)$*

### 3. Relations avec les éléments réguliers de l’algèbre de Lie

#### Proposition 6 {#lie-vii-s4-prop-6 .statement tag=00W6}

*Soient $V$ un sous-groupe ouvert de $g$ et $\exp : V \to G$ une application exponentielle définie sur $V$.*

(i) Il existe un voisinage W de 0 dans V tel que $g^1(\exp x) = g^0(x)$ pour tout $x \in W$.

(ii) Si $k = \mathbf{R}$ ou $\mathbf{C}$, on a $g^1(\exp x) \supseteq g^0(x)$ pour tout $x \in g$.

D'après le cor. 3 à la prop. 8 du chap. III, § 4, n° 4, il existe un voisinage $V'$ de 0 dans V tel que, pour tout $x \in V'$, $\exp(\mathrm{ad}(x)) = \sum_{n=0}^{\infty} \frac{1}{n!} \mathrm{ad}(x)^n$ soit défini et $\mathrm{Ad}(\exp x) = \exp(\mathrm{ad}(x))$. Si $P \in k[X]$ et si $\alpha \in \mathrm{End}(g)$, on vérifie facilement que, pour tout $\lambda \in k$, on a $g^{\lambda}(\alpha) \subset g^{P(\lambda)}(P(\alpha))$. Par suite
$$
g^0(\mathrm{ad}(x)) \subset g^1(\exp(\mathrm{ad}(x))) = g^1(\mathrm{Ad}(\exp x)) = g^1(\exp x)
$$
pour tout $x \in V'$. Si $k = \mathbf{R}$ ou $\mathbf{C}$, on a $V = g$ et on peut choisir $V' = V$ ce qui prouve (ii). Démontrons (i). Soit U un voisinage de 0 dans $\mathrm{End}(g)$ tel que, pour tout $\alpha \in U$, $\mathrm{Log}(1 + \alpha) = \sum_{n > 0} (-1)^{n+1} \frac{1}{n} \alpha^n$ soit défini. On a $\mathrm{Log} \circ \exp = 1$ sur un voisinage de 0 et, pour tout $\alpha \in U$, $g^1(1 + \alpha) \subset g^0(\mathrm{Log}(1 + \alpha))$. Soit W le voisinage de 0 dans g formé par les $x \in V'$ tels que $\exp \mathrm{ad}\, x \in 1 + U$ et
$$
\mathrm{Log}(\exp(\mathrm{ad}(x))) = \mathrm{ad}(x).
$$
Pour tout $x \in W$, on a
$$
g^1(\exp x) = g^1(\mathrm{Ad}(\exp x)) = g^1(\exp(\mathrm{ad}(x)))
$$
$$
\subset g^0(\mathrm{Log}(\exp(\mathrm{ad}(x)))) = g^0(\mathrm{ad}(x)) = g^0(x).
$$
Ceci montre que $g^1(\exp x) = g^0(x)$ pour tout $x \in W$.

#### Lemme 4 {#lie-vii-s4-lem-4 .statement tag=00W7}

Soient U un voisinage de 0 dans g et exp une application exponentielle de U dans G, étale en tout point de U et telle que $g^1(\exp x) = g^0(x)$ quel que soit $x \in U$.

(i) La fonction $r^0_{\mathrm{Ad}}$ est constante et égale au rang de g sur $\exp(U)$.

(ii) Si $x \in U$, pour que $\exp x$ soit régulier, il faut et il suffit que x soit un élément régulier de g.

(iii) Si $a \in \exp(U)$, pour que a soit régulier, il faut et il suffit que $g^1(a)$ soit une sous-algèbre de Cartan de g.

Soit $l = \mathrm{rg}(g)$. Si $x \in U$ est un élément régulier de g, on a
$$
r_{\mathrm{Ad}}(\exp x) = \dim g^1(\exp x) = \dim g^0(x) = l.
$$
Puisque les éléments réguliers de g appartenant à U forment un voisinage de x et que exp est étale en x, ceci montre que $\exp x$ est régulier et que $r^0_{\mathrm{Ad}}(\exp x) = l$. Les éléments réguliers de g appartenant à U étant denses dans U, on a $r^0_{\mathrm{Ad}}(a) = l$ pour tout $a \in \exp(U)$. Soit $a \in \exp(U)$ un élément régulier de G et soit $x \in U$ tel que $a = \exp x$. Puisque $g^0(x) = g^1(a)$, on a $\dim g^0(x) = r^0_{\mathrm{Ad}}(a) = l$. Par suite, x est un élément régulier de g et $g^1(a)$ est une sous-algèbre de Cartan de g. Enfin si $a \in \exp(U)$ et si $g^1(a)$ est une sous-algèbre de Cartan de g, on a
$$
r_{\mathrm{Ad}}(a) = \dim g^1(a) = l = r^0_{\mathrm{Ad}}(a),
$$
donc a est régulier.

#### Proposition 7 {#lie-vii-s4-prop-7 .statement tag=00W8}

Soit V un voisinage de e dans G. Toute sous-algèbre de Cartan de g est de la forme $g^1(a)$ où a est un élément régulier de G appartenant à V.

D’après la prop. 6, il existe un voisinage ouvert U de 0 dans g et une application exponentielle exp : U $\to$ G vérifiant les conditions du lemme 4. Si $\mathfrak{h}$ est une sous-algèbre de Cartan de g, il existe un élément régulier $x \in \mathfrak{h}$ tel que $\mathfrak{h} = g^0(x)$ (§ 3, th. 2). Il existe d’autre part un élément $t \in k^*$ tel que $tx \in U$ et $\exp(tx) \in V$. On a alors $\mathfrak{h} = g^0(x) = g^0(tx) = g^1(\exp(tx))$, et d’après le lemme 4 (ii), $\exp(tx)$ est un élément régulier de G.

#### Proposition 8 {#lie-vii-s4-prop-8 .statement tag=00W9}

Soit l le rang de g. Il existe un sous-groupe ouvert $G^*$ de G tel que :
(i) la fonction $r_{\mathrm{Ad}}^0$ est constante sur $G^*$ et sa valeur est l ;
(ii) pour qu’un élément $a \in G^*$ soit régulier, il faut et il suffit que $g^1(a)$ soit une sous-algèbre de Cartan de g ;
(iii) si $a \in G^*$, toute sous-algèbre de Cartan de $g^1(a)$ est une sous-algèbre de Cartan de g.

(i) D’après la prop. 6, il existe un voisinage ouvert U de 0 dans g et une application exp de U dans G vérifiant les conditions du lemme 4. Dans la suite, on désignera par $G^*$ la composante neutre de G si $k = \mathbf{R}$ ou $\mathbf{C}$ et un sous-groupe ouvert de G contenu dans exp(U) si k est ultramétrique. Puisque $r_{\mathrm{Ad}}^0$ est localement constante et que sa valeur en tout point de exp(U) est l (lemme 4 (i)), on voit que $r_{\mathrm{Ad}}^0$ est constante et égale à l sur $G^*$.

(ii) Soit $R^*$ (resp. $S^*$) l’ensemble des éléments réguliers de $G^*$ (resp. l’ensemble des éléments $a \in G^*$ tels que $g^1(a)$ soit une sous-algèbre de Cartan de g). On a $S^* \subset R^*$. En effet, si $a \in S^*$, alors $r_{\mathrm{Ad}}(a) = l = r_{\mathrm{Ad}}^0(a)$. Montrons que $R^* \subset S^*$. Si k est ultramétrique, cela résulte de l’inclusion $G^* \subset \exp(U)$ et du lemme 4 (iii). Supposons $k = \mathbf{C}$. D’après le cor. à la prop. 5, si $a \in R^*$, alors pour tout $a'$ appartenant à un voisinage de a, $g^1(a')$ est conjugué de $g^1(a)$ par un automorphisme de g. Ceci prouve que $S^*$ et $R^* - S^*$ sont ouverts dans $G^*$. On a vu que $S^*$ contient tous les éléments réguliers d’un voisinage de e (lemme 4 (iii)); par conséquent $S^*$ est non vide. Puisque $G^*$ est connexe, il en est de même de $R^*$ (prop. 1) et par conséquent $S^* = R^*$.

Il reste à étudier le cas $k = \mathbf{R}$. Supposons d’abord que $G^*$ soit un sous-groupe intégral de $\mathbf{GL}(E)$ où E désigne un espace vectoriel réel de dimension finie. Soit $G_c^*$ le sous-groupe intégral de $\mathbf{GL}(E \otimes_{\mathbf{R}} \mathbf{C})$ ayant pour algèbre de Lie $g_c = g \otimes \mathbf{C}$. Il existe une fonction analytique sur $G_c^*$ dont l’ensemble des zéros est le complémentaire de l’ouvert des éléments réguliers de $G_c^*$. D’après VAR, R, 3.2.5, cette fonction ne peut être nulle en tout point de $G^*$. Par conséquent, $G^*$ contient des éléments réguliers de $G_c^*$. Soit $\mathrm{Ad}_c$ la représentation adjointe de $G_c^*$. Pour tout $a \in G^*$, on a $g_c^1(a) = g^1(a) \otimes \mathbf{C}$, donc $r_{\mathrm{Ad}_c}(a) = r_{\mathrm{Ad}}(a)$. Si $a \in G^*$ est un élément régulier de $G_c^*$, alors c’est un élément régulier de $G^*$ et $r_{\mathrm{Ad}_c}^0(a) = r_{\mathrm{Ad}}^0(a)$. Les fonctions $r_{\mathrm{Ad}_c}^0$ et $r_{\mathrm{Ad}}^0$ étant constantes respectivement sur $G_c^*$ et sur $G^*$, il en résulte que les éléments réguliers de $G^*$ sont les éléments réguliers de $G_c^*$ appartenant à

G*. D’après ce qui a été vu plus haut, si $a$ est un élément régulier de $G^*$, alors $g_c^1(a) = g^1(a) \otimes \mathbf{C}$ est une sous-algèbre de Cartan de $g_c$; ceci implique que $g^1(a)$ est une sous-algèbre de Cartan de $g$ (§ 2, prop. 3).

Supposons maintenant $G$ simplement connexe. Il existe un espace vectoriel réel de dimension finie $E$ et un morphisme étale $f$ de $G$ sur un sous-groupe intégral $G'$ de $\mathbf{GL}(E)$ (III, § 6, no 1, cor. au th. 1). D’après la prop. 2, si $a \in G$ est régulier, alors $f(a)$ est régulier. D’après ce qui précède, ${g'}^1(f(a))$ est une sous-algèbre de Cartan de l’algèbre de Lie $g'$ de $G'$. Puisque ${g'}^1(f(a)) = (Tf)g^1(a)$ et que $Tf$ est un isomorphisme de $g$ sur $g'$, ceci prouve que $g^1(a)$ est une sous-algèbre de Cartan de $g$.

Passons-enfin au cas général ($k = \mathbf{R}$). Soient $\tilde{G}$ un revêtement universel de $G^*$, $\tilde{g} = L(\tilde{G})$, et $q$ l’application canonique de $\tilde{G}$ sur $G^*$. Puisque le noyau de $q$ est contenu dans le centre de $\tilde{G}$, si $a \in G^*$ est régulier et si $a' \in q^{-1}(a)$, alors $a'$ est régulier (prop. 2). D’après ce qui précède, $\tilde{g}^1(a')$ est une sous-algèbre de Cartan de $\tilde{g}$. Puisque $g^1(a) = (Tq)\tilde{g}^1(a')$ et que $Tq$ est un isomorphisme de $\tilde{g}$ sur $g$, ceci prouve que $g^1(a)$ est une sous-algèbre de Cartan de $g$.

(iii) D’après la prop. 5, il existe un voisinage $V$ de $a$ tel que, pour tout $a' \in V$, $g^1(a')$ soit conjugué d’une sous-algèbre de $g^1(a)$ par un automorphisme de $g$. Puisque tout voisinage de $a$ contient un élément régulier de $G^*$, il résulte de (ii) que $g^1(a)$ contient une sous-algèbre de Cartan de $g$. D’après la prop. 3 du § 3, toute sous-algèbre de Cartan de $g^1(a)$ est donc une sous-algèbre de Cartan de $g$.

#### Remarque {#lie-vii-s4-n3-rem-1 .statement tag=00WA}

Si $k = \mathbf{C}$, les sous-algèbres $g^1(a)$ pour $a$ régulier appartenant à une composante connexe $M$ de $G$ sont conjuguées par $\mathrm{Int}(g)$. Soit en effet $R$ l’ensemble des éléments réguliers de $G$. Pour tout $a \in R \cap M$, soit $M_a$ l’ensemble des $b \in R \cap M$ tels que $g^1(b)$ soit conjugué de $g^1(a)$ par $\mathrm{Int}(g)$. On a $\mathrm{Int}(g) = \mathrm{Ad}(G^0)$, où $G^0$ est la composante neutre de $G$. D’après le corollaire à la prop. 5, $M_a$ est ouvert dans $R$. Il en résulte que $M_a$ est ouvert et fermé dans $R$. Puisque $k = \mathbf{C}$, $R \cap M$ est connexe (lemme 1) et par conséquent, $M_a = R \cap M$.

### 4. Application aux automorphismes élémentaires

#### Proposition 9 {#lie-vii-s4-prop-9 .statement tag=00WB}

Soient $k$ un corps de caractéristique 0 et $g$ une algèbre de Lie sur $k$. Si $a \in \mathrm{Aut}_e(g)$, la dimension du nilspace de $a - 1$ est au moins égale au rang de $g$.

D’après le « principe de Lefschetz » (A, V, § 14, no 7, prop. 18), $k$ est réunion filtrante croissante d’une famille de sous-corps $(k_i)_{i \in I}$ qui admettent $\mathbf{C}$ pour extension. Soient $(e_\alpha)$ une base de $g$ sur $k$ et $x_1, \ldots, x_m$ des éléments de $g$ tels que $\mathrm{ad}(x_1), \ldots, \mathrm{ad}(x_m)$ soient nilpotents et que $a = e^{\mathrm{ad}(x_1)} \ldots e^{\mathrm{ad}(x_m)}$. Soient $c_{\alpha \beta}^\gamma$ les constantes de structure de $g$ par rapport à la base $(e_\alpha)$ et $(x_r^\alpha)$ les composantes de $x_r$ par rapport à cette base $(1 \leq r \leq m)$. Il existe un indice $j \in I$ tel que les $c_{\alpha \beta}^\gamma$ et les $x_r^\alpha$ appartiennent tous à $k_j$. Soit $g_j = \sum_\alpha k_j e_\alpha$; c'est une algèbre de Lie sur $k_j$ contenant $x_1, \ldots, x_m$, et la restriction $a_j$ de $a$ à $g_j$ est un automorphisme élémentaire de $g_j$. L'extension de $a_j$ à $g_j \otimes_{k_j} \mathbf{C}$ est un automorphisme élémentaire $a_j \otimes 1$ de $g_j \otimes \mathbf{C}$. Soit alors $G_j$ un groupe de Lie complexe connexe d'algèbre de Lie $g_j \otimes \mathbf{C}$, et $s$ un élément de $G_j$ tel que $\mathrm{Ad}(s) = a_j \otimes 1$. La prop. 8, appliquée au couple $(G_j, s)$, montre que le nilespace de $a_j \otimes 1 - 1$ est de dimension $n$, où
$$
n \geqslant \mathrm{rg}(g_j \otimes \mathbf{C}) = \mathrm{rg}(g_j) = \mathrm{rg}(g).
$$
Or ce nilespace a même dimension que celui de $a_j - 1$ et que celui de $a - 1$. D'où la proposition.

## EXERCICES {#lie-vii-s4-exercises}

Les notations et hypothèses sont celles des nos 1, 2, 3 du § 4.

See the [exercises for § 4](exercises/s4/).
