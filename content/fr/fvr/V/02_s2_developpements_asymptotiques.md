---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: ÉTUDE LOCALE DES FONCTIONS
section: 2
section_title: Développements asymptotiques
lang: fr
source: fvr-i-vii-fr
book_pages: FVR V.10-FVR V.17
pdf_pages: 0215-0222
extraction: ocr
subsections:
    - "no": 1
      title: Échelles de comparaison
      page: 10
      pdf_page: 215
    - "no": 2
      title: Parties principales et développements asymptotiques
      page: 11
      pdf_page: 216
    - "no": 3
      title: Sommes et produits de développements asymptotiques
      page: 14
      pdf_page: 219
    - "no": 4
      title: Composition des développements asymptotiques
      page: 14
      pdf_page: 219
    - "no": 5
      title: Développements asymptotiques à coefficients variables
      page: 17
      pdf_page: 222
statements: 12
exercises: 0
content_sha256: fba972f80fcf1c93e39dd0acb77f39fca772999181c97e100ff1e3e9ea05c782
---

## § 2. DÉVELOPPEMENTS ASYMPTOTIQUES

### 1. Échelles de comparaison

Soient $E$ un ensemble filtré par un filtre de base $\mathfrak{F}$, et $K$ un corps valué non discret (le plus souvent $K = \mathbf{R}$ ou $K = \mathbf{C}$). Dans l’ensemble des fonctions de $\mathcal{H}(\mathfrak{F}, K)$ non équivalentes à 0 modulo $R_\infty$ (c’est-à-dire telles que dans tout ensemble de $\mathfrak{F}$, il existe un point au moins où la fonction ne s’annule pas), la relation « $f \ll g$ ou $f = g$ » est une relation d’ordre.

#### Définition 1 {#fvr-v-s2-def-1 .statement}

On dit qu’une partie $\mathcal{E}$ de $\mathcal{H}(\mathfrak{F}, K)$ formée de fonctions non équivalentes à 0 modulo $R_\infty$ est une échelle de comparaison lorsque $\mathcal{E}$ est totalement ordonnée par la relation « $f \ll g$ ou $f = g$ ».

En d’autres termes, si $f$ et $g$ sont deux fonctions de $\mathcal{E}$, on a toujours entre $f$ et $g$ une (et une seule) des trois relations $f \ll g$, $g \ll f$, $f = g$. Il s’ensuit que dans $\mathcal{E}$, la relation $f \asymp g$ (et a fortiori $|f| \sim a|g|$, où $a$ est un nombre > 0) entraîne $f = g$.

Toute partie d’une échelle de comparaison est évidemment une échelle de comparaison.

#### Exemple 1 {#fvr-v-s2-n1-exa-1 .statement}

Pour $x$ réel tendant vers $+\infty$, l’ensemble des fonctions $x^\alpha$ ($\alpha$ nombre réel arbitraire) est une échelle de comparaison. Il en est de même des fonctions $(x-a)^\alpha$ lorsque $\mathfrak{F}$ est l’ensemble des intervalles ouverts d’origine $a$.

#### Exemple 2 {#fvr-v-s2-n1-exa-2 .statement}

Pour $z$ complexe tendant vers $\infty$, l’ensemble des fonctions $z^n$ ($n$ entier rationnel) est une échelle de comparaison; il en est de même des fonctions $(z-a)^n$ lorsque $\mathfrak{F}$ est la trace sur le complémentaire du point $a \in \mathbf{C}$ du filtre des voisinages de ce point.

#### Exemple 3 {#fvr-v-s2-n1-exa-3 .statement}

Soit F un espace normé; l’ensemble des fonctions $\|x - a\|^{\alpha}$ ($\alpha$ nombre réel arbitraire) est une échelle de comparaison lorsque $\mathfrak{F}$ est la trace sur le complémentaire de $a$ du filtre des voisinages de ce point. On notera que si $p$ et $q$ sont deux normes distinctes sur $F$, la réunion des deux échelles de comparaison formées des fonctions $(p(x-a))^{\alpha}$ et $(q(x-a))^{\alpha}$ n’est plus en général une échelle de comparaison.

#### Exemple 4 {#fvr-v-s2-n1-exa-4 .statement}

Pour $x$ réel tendant vers $+\infty$, l’ensemble $\mathscr{E}$ des fonctions de la forme $\exp(p(x))$, où $p(x)$ parcourt l’ensemble des polynômes sans terme constant (à coefficients réels), est une échelle de comparaison: il suffit de remarquer que le quotient de deux fonctions de $\mathscr{E}$ appartient encore à $\mathscr{E}$, et qu’une fonction $\exp(p(x))$ tend nécessairement vers 0 ou $+\infty$ si $p \neq 0$; en effet, on a alors $p(x) \sim \alpha x^n$, où $n > 0$ et $\alpha \neq 0$; si $\alpha > 0$, $p(x) > \frac{1}{2} \alpha x^n$ pour $x$ assez grand; si $\alpha < 0$, $p(x) < \frac{1}{2} \alpha x^n$ pour $x$ assez grand; dans le premier cas, $\exp(p(x))$ tend vers $+\infty$, et dans le second cas vers 0.

#### Exemple 5 {#fvr-v-s2-n1-exa-5 .statement}

Pour $x$ réel tendant vers $+\infty$, l’ensemble $\mathscr{E}$ des fonctions de la forme $x^{\alpha}(\log x)^{\beta}$ (définies pour $x > 1$), où $\alpha$ et $\beta$ sont des nombres réels arbitraires, est une échelle de comparaison. En effet, ici encore le quotient de deux fonctions de $\mathscr{E}$ est une fonction de $\mathscr{E}$; il suffit donc de montrer que si $\alpha$ et $\beta$ ne sont pas tous deux nuls, $x^{\alpha}(\log x)^{\beta}$ tend vers 0 ou vers $+\infty$; c’est évident si $\alpha = 0$, $\beta \neq 0$; si $\alpha > 0$, on a $(\log x)^{-\beta} \ll x^{\alpha}$, et si $\alpha < 0$, $(\log x)^{\beta} \ll x^{-\alpha}$ quel que soit $\beta$, d’où la proposition.

On observa que cette dernière échelle de comparaison est un ensemble totalement ordonné (pour la relation «$f \ll g$ ou $f = g$») dont la structure d’ordre est isomorphe à la structure d’ordre lexicographique de $\mathbf{R}^2$ (E, III, p. 23); on rappelle que dans cette structure, la relation $(\alpha, \beta) < (\gamma, \delta)$ signifie $\alpha < \gamma$, ou $\alpha = \gamma$ et $\beta < \delta$.

De même, l’échelle formée des fonctions $\exp(p(x))$, où $p$ parcourt l’ensemble $P_0$ des polynômes sans terme constant, a une structure d’ordre isomorphe à la structure d’ordre de $P_0$, dans laquelle la relation $p < q$ signifie que le terme dominant du polynôme $q - p$ a un coefficient > 0 (cf. A, VI, § 2, no 1, Exemple 2).

Soit $\varphi$ une application d’un ensemble $F$ dans $E$, telle que $\varphi(\mathfrak{F})$ soit une base de filtre sur $F$. Si $\mathscr{E}$ est une échelle de comparaison sur $E$ (pour la base de filtre $\mathfrak{F}$), les fonctions $f \circ \varphi$, où $f$ parcourt $\mathscr{E}$, forment une échelle de comparaison sur $F$ (pour la base de filtre $\varphi^{-1}(\mathfrak{F})$).

### 2. Parties principales et développements asymptotiques

Soit $\mathscr{E}$ une échelle de comparaison formée de fonctions à valeurs dans un corps valué non discret $K$. Soit $V$ un espace normé sur $K$, et soit $f$ une fonction de $\mathscr{H}(\mathfrak{F}, V)$; s’il existe une fonction $g \in \mathscr{E}$, et un élément $a \neq 0$ de $V$ tels que $f \sim a g$, on dit que $a g$ est une partie principale de $f$ relativement à l’échelle $\mathscr{E}$. D’après la déf. 1 de $V$, p. 10, $f$ ne peut avoir qu’une seule partie principale relative à $\mathscr{E}$, car si $g_1$, $g_2$ sont deux fonctions de $\mathscr{E}$, $a_1$, $a_2$ deux éléments $\neq 0$ de $V$, la relation a_1 g_1 \sim a_2 g_2 entraîne |g_1| \asymp |g_2|, et par suite g_1 = g_2, d’où (a_2 - a_1)g_1 \ll g_1, et comme g_1 n’est identiquement nulle dans aucun ensemble de $\mathcal{E}$, cela entraîne $a_2 = a_1$.

Si $f$ admet une partie principale relativement à une échelle de comparaison $\mathcal{E}$, elle admet la même partie principale relativement à toute échelle de comparaison $\mathcal{E}' \supset \mathcal{E}$.

#### Exemple 1 {#fvr-v-s2-n2-exa-1 .statement}

Pour x réel (resp. complexe) tendant vers +∞ (resp. vers ∞), tout polynôme $a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ à coefficients dans V, tels que $a_0 \neq 0$, a pour partie principale $a_0 x^n$ par rapport à l’échelle des $x^n$ (ou de toute échelle contenant les $x^n$). On en déduit que toute fraction rationnelle $\frac{a_0 x^n + \cdots + a_m}{b_0 x^n + \cdots + b_n}$ à coefficients réels ou complexes tels que $a_0 b_0 \neq 0$, a pour partie principale $\frac{a_0}{b_0} x^{m-n}$ par rapport à la même échelle.

#### Exemple 2 {#fvr-v-s2-n2-exa-2 .statement}

Une fonction peut être comparable à toutes les fonctions d’une échelle de comparaison sans admettre de partie principale par rapport à cette échelle. Par exemple, pour x réel tendant vers +∞, $\sqrt{x}$ n’a pas de partie principale par rapport à l’échelle des $x^n$, où n est entier rationnel; log x n’a pas de partie principale par rapport à l’échelle des $x^\alpha$ ($\alpha$ réel quelconque); exp($\sqrt{\log x}$) et $x^x = e^{x \log x}$ n’ont pas de partie principale par rapport à l’échelle des $x^\alpha (\log x)^{\beta}$, ni par rapport à l’échelle des exp ($p(x)$) ($p$ polynôme sans terme constant).

La notion de partie principale est susceptible d’une généralisation étendue. Supposons en effet qu’une fonction $f \in \mathcal{H}(\mathfrak{F}, V)$ ait une partie principale $a_1 g_1$ par rapport à une échelle $\mathcal{E}$; la relation $f \sim a_1 g_1$ équivaut à $f - a_1 g_1 \ll g_1$ (V, p. 6, déf. 4); pour étudier de façon plus précise la fonction $f$, on est donc amené à considérer la fonction $f - a_1 g_1$. Si cette fonction a une partie principale $a_2 g_2$ par rapport à $\mathcal{E}$, on aura nécessairement $g_2 \ll g_1$ et $f - a_1 g_1 - a_2 g_2 \ll g_2$.

D’une façon générale, supposons que l’échelle $\mathcal{E}$ soit écrite paramétriquement sous la forme $(g_\alpha)$, où $\alpha$ parcourt un ensemble d’indices A muni d’une structure d’ensemble totalement ordonné isomorphe à l’opposée de la structure d’ordre de $\mathcal{E}$: la relation $\alpha < \beta$ est donc équivalente à $g_\beta \ll g_\alpha$. Dans ces conditions:

#### Définition 2 {#fvr-v-s2-def-2 .statement}

On dit qu’une fonction $f \in \mathcal{H}(\mathfrak{F}, V)$ admet un développement asymptotique à la précision $g_\alpha$ (relativement à l’échelle $\mathcal{E}$) s’il existe une famille $(a_\lambda)_{\lambda \leq \alpha}$ d’éléments de V, nuls sauf un nombre fini d’entre eux, tels que $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$. On dit que $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ est un développement asymptotique de $f$ à la précision $g_\alpha$, que les $a_\lambda g_\lambda$ ($\lambda \leq \alpha$) sont les termes, les $a_\lambda$ les coefficients et la fonctions $r_\alpha = f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ le reste de ce développement.

Pour exprimer que $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ est un développement asymptotique de $f$ à la précision $g_\alpha$, on se bornera le plus souvent à écrire
$$
f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o(g_\alpha) \quad \text{(ou } f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o_k(g_\alpha)
$$

s’il figure plusieurs fonctions dans la démonstration) conformément aux notations de V, p. 9 et 10.

De deux développements asymptotiques (de deux fonctions distinctes ou non) relativement à la même échelle $\mathscr{E}$, on dit que celui dont la précision a le plus grand indice est le plus précis.

Si $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ est un développement asymptotique de $\mathbf{f}$ à la précision $g_\alpha$, pour tout $\beta < \alpha$, $\sum_{\lambda \leq \beta} a_\lambda g_\lambda$ est un développement asymptotique de $\mathbf{f}$ à la précision $g_\beta$ (V, p. 5, prop. 5): on dit qu’on l’obtient en réduisant à la précision $g_\beta$ le développement donné $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ de $\mathbf{f}$.

Si $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ et $\sum_{\lambda \leq \alpha} b_\lambda g_\lambda$ sont des développements asymptotiques à la même précision $g_\alpha$ de deux fonctions $\mathbf{f}_1, \mathbf{f}_2$, $\sum_{\lambda \leq \alpha} (a_\lambda + b_\lambda) g_\lambda$ est un développement asymptotique de $\mathbf{f}_1 + \mathbf{f}_2$ à la précision $g_\alpha$ (V, p. 7, prop. 5) et pour tout scalaire $c$, $\sum_{\lambda \leq \alpha} a_\lambda c g_\lambda$ est un développement asymptotique de $\mathbf{f}_1 c$ à la précision $g_\alpha$. On en déduit que si une fonction $\mathbf{f}$ admet un développement asymptotique à la précision $g_\alpha$, ce développement est unique: il suffit de voir que la fonction 0 ne peut admettre de développement asymptotique à la précision $g_\alpha$ ayant des coefficients $\neq 0$. Or, si $0 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$, et si $\gamma$ est le plus petit des indices $\lambda \leq \alpha$ tel que $a_\lambda \neq 0$, on aurait $a_\gamma g_\gamma = - \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda - r_\alpha \ll g_\gamma$, ce qui est absurde.

Dire qu’une fonction $\mathbf{f}$ admet un développement asymptotique à la précision $g_\alpha$, dont tous les coefficients sont nuls, équivaut à dire que $\mathbf{f} \ll g_\alpha$. Si $\mathbf{f}$ admet un développement asymptotique $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ à la précision $g_\alpha$, dont les coefficients ne sont pas tous nuls, et si $\gamma$ est le plus petit des indices $\lambda$ tels que $a_\lambda \neq 0$, $a_\gamma g_\gamma$ est la partie principale de $\mathbf{f}$ relativement à l’échelle $\mathscr{E}$, car on a $\mathbf{f} - a_\gamma g_\gamma = \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha \ll g_\gamma$; de même, si $\mu \leq \alpha$ est un indice tel que $a_\mu \neq 0$, $a_\mu g_\mu$ est la partie principale de $\mathbf{f} - \sum_{\lambda < \mu} a_\lambda g_\lambda$.

Les développements asymptotiques les plus importants dans les applications sont les développements relatifs à l’échelle des $x^{-n}$ (resp. des $z^{-n}$), où $n$ est entier positif ou négatif, lorsque $x$ réel tend vers $+\infty$ ou $-\infty$ (resp. lorsque $z$ complexe tend vers $\infty$), ou relatifs à l’échelle des $(x-c)^n$ (resp. $(z-c)^n$) lorsque $x$ réel tend vers $c$ à droite ou à gauche (resp. lorsque $z$ complexe tend vers $c$). On a vu dans I, p. 29 que toute fonction vectorielle d’une variable réelle $x$, $k$ fois dérivable au point $c \in \mathbf{R}$, admet en ce point un développement de Taylor d’ordre $k$, c’est-à-dire un développement asymptotique à la précision $(x-c)^k$ relatif à l’échelle des $(x-c)^n$.

### 3. Sommes et produits de développements asymptotiques

Si $f_1, f_2$ admettent des développements asymptotiques à la précision $g_\alpha$ et $g_\beta$ respectivement, relativement à une échelle de comparaison $\mathscr{E}$, on en déduit des développements à la précision $g_{\min(\alpha,\beta)}$ en *limitant* à cette précision les deux développements; nous avons vu alors dans V, p. 13, comment on obtient un développement asymptotique de $f_1 + f_2$ à la précision $g_{\min(\alpha,\beta)}$.

Soient $V_1, V_2$ et $V$ trois espaces normés sur le corps $K$, et soit $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}, \mathbf{y}]$ une *application bilinéaire continue* de $V_1 \times V_2$ dans $V$; nous supposerons d’autre part dans tout le reste de ce paragraphe, que l’échelle $\mathscr{E}$ soit telle que le *produit* de deux fonctions quelconques de $\mathscr{E}$ appartienne encore à $\mathscr{E}$ (ce qui est le cas pour toutes les échelles de comparaison données en exemples (dans V, p. 10).

Soient alors $f_1, f_2$ des fonctions de $\mathcal{H}(\mathfrak{F}, V_1)$ et $\mathcal{H}(\mathfrak{F}, V_2)$ respectivement, admettant par rapport à l’échelle $\mathscr{E}$ des développements asymptotiques $f_1 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha, \quad f_2 = \sum_{\mu \leq \beta} b_\mu g_\mu + r_\beta$ à la précision $g_\alpha$ et $g_\beta$ respectivement. Supposons en outre que ni les $a_\lambda$ ni les $b_\mu$ ne soient tous nuls, et soient $a_{\gamma, g_\gamma}$ et $b_{\delta, g_\delta}$ les parties principales de $f_1$ et $f_2$. Par hypothèse, on peut écrire $g_\gamma g_\delta = g_\beta$ et $g_\delta g_\alpha = g_\sigma$; montrons que la somme $\sum [a_\lambda, b_\mu] g_\lambda g_\mu$, étendue aux couples $(\lambda, \mu)$ tels que $g_{\min(\alpha, \sigma)} \ll g_\lambda g_\mu$, est un *développement asymptotique de* $[f_1, f_2]$ *à la précision* $g_{\min(\alpha, \sigma)}$. En effet, la différence entre $[f_1, f_2]$ et cette somme est somme d’un nombre fini de termes, qui sont soit de la forme $[a_\lambda, b_\mu] g_\lambda g_\mu$ avec $g_\lambda g_\mu \ll g_{\min(\alpha, \sigma)}$, soit de la forme $[a_\lambda, r_\mu] g_\lambda$, où $\lambda \geq \gamma$, soit de la forme $[r_\alpha, b_\mu] g_\mu$, où $\mu \geq \delta$; mais comme $[\mathbf{x}, \mathbf{y}]$ est continue, on a (V, p. 3, prop. 3 et V, p. 5, prop. 6) $[a_\lambda, r_\mu] g_\lambda \ll r_\beta g_\lambda \ll g_\delta g_\lambda = g_\sigma$ pour $\lambda \geq \gamma$, et de même $[r_\alpha, b_\mu] g_\mu \ll r_\alpha g_\mu \ll g_\alpha g_\delta = g_\sigma$ pour $\mu \geq \delta$, d’où la proposition (V, p. 5, prop. 5).

Si tous les $a_\lambda$ sont nuls, on a $[f_1, f_2] \ll g_\alpha g_\beta$, autrement dit, on a un développement asymptotique de $[f_1, f_2]$ à termes nuls, à la précision $g_\alpha g_\beta$; de même si tous les $a_\lambda$ et tous les $b_\mu$ sont nuls, on a un développement asymptotique de $[f_1, f_2]$ à termes nuls, à la précision $g_\alpha g_\beta$.

On appliquera surtout le résultat précédent au cas où $V$ est une *algèbre normée* sur $K$, et la fonction bilinéaire $[\mathbf{x}, \mathbf{y}]$ le produit $xy$ dans cette algèbre; les cas les plus importants sont ceux où $V$ est égal à $\mathbf{R}$ ou $\mathbf{C}$.

En particulier, si $f_i$ (1 $\leq i \leq n$) sont $n$ fonctions de $\mathcal{H}(\mathfrak{F}, K)$ admettant chacune un développement asymptotique par rapport à $\mathscr{E}$, on pourra obtenir un développement asymptotique par rapport à $\mathscr{E}$ pour tout *polynôme* $\sum_{(v_i)} a_{v_1 v_2 \ldots v_n} f_1^{v_1} \ldots f_n^{v_n}$ par rapport aux $f_i$, à coefficients dans un espace normé $V$; les règles qui précèdent permettent en outre de déterminer la précision du développement obtenu, connaissant celles des développements des fonctions $f_i$.

### 4. Composition des développements asymptotiques

Soit $f$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ (resp. $\mathcal{H}(\mathfrak{F}, \mathbf{C})$) admettant un développement asymptotique à la précision $g_\alpha$ par rapport à une échelle $\mathscr{E}$, et *ayant pour limite* 0 suivant le filtre de base $\mathfrak{F}$. Soit d’autre part $h$ une fonction à valeurs dans l’espace normé $V$ sur $\mathbf{R}$ (resp. $\mathbf{C}$), définie dans un voisinage du point $0$ dans $\mathbf{R}$ (resp. $\mathbf{C}$) et $n$ fois dérivable dans ce voisinage; on a donc dans ce voisinage,

$$
h(t) = c_0 + c_1 t + \cdots + c_n t^n + o(t^n)
$$

(I, p. 29), d’où, dans un ensemble convenable de $\mathfrak{F}$,

$$
h \circ f = c_0 + c_1 f + \cdots + c_n f^n + o(f^n).
$$

Nous avons vu, au no 3, comment on peut former un développement asymptotique de $c_0 + c_1 f + \cdots + c_n f^n$, à une précision $g_\rho$ bien déterminée par la précision du développement de $f$; d’autre part, supposons que les coefficients du développement asymptotique de $f$ ne soient pas tous nuls, et que $a_{\gamma g_\gamma}$ soit la partie principale de $f$, et soit $g_\sigma = g_\gamma^\sigma$; si $\sigma < \rho$, on aura un développement de $h \circ f$ à la précision $g_\sigma$ en limitant le développement de $\sum_{k=0}^n c_k f^k$ à cette précision; si au contraire $\rho \leq \sigma$, le développement de $\sum_{k=0}^n c_k f^k$ est aussi un développement de $h \circ f$ à la précision $g_\rho$.

Si tous les termes de développement asymptotique de $f$ sont nuls et si $g_\alpha \ll 1$, on a $f \ll g_\alpha$, donc $f^k \ll g_\alpha^k \ll g_\alpha$ pour tout entier $k > 0$; si $c_m$ est le premier coefficient d’indice $> 0$ qui ne soit pas nul (en supposant que les $c_k$ d’indice $k > 0$ ne soient pas tous nuls), $c_0$ est un développement asymptotique de $h \circ f$ à la précision $g_\alpha^m$.

Dans le reste de ce no, nous nous bornerons au cas où les fonctions de $\mathcal{E}$ ont des valeurs réelles et strictement positives dans un ensemble de $\mathfrak{F}$, et nous ne considérerons que les développements asymptotiques de fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. Supposons d’abord que pour toute fonction $g \in \mathcal{E}$ et tout nombre réel $v$, $g^v$ appartienne encore à $\mathcal{E}$: cette condition est par exemple remplie par l’échelle des $x^\alpha$, ou celle des $x^\alpha |\log x|^\beta$ ($\alpha$ et $\beta$ réels quelconques) au voisinage de $+\infty$ ou au voisinage de $0$ dans $\mathbf{R}$. Cette propriété entraîne que le quotient de deux fonctions de $\mathcal{E}$ appartient encore à $\mathcal{E}$. Cela étant, d’un développement asymptotique relatif à $\mathcal{E}$ d’une fonction $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$, à la précision $g_\alpha$, on peut déduire un développement de $|f|^v$ pour tout nombre réel $v$. Bornons-nous en effet au cas où les coefficients du développement de $f$ ne sont pas tous nuls, et soit $a_{\gamma g_\gamma}$ la partie principale de $f$; on peut écrire $|f|^v = |a_v|^{g_\gamma}(1 + h)^v$, avec

$$
h = \sum_{\gamma < \lambda < \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} + o\left( \frac{g_\alpha}{g_\gamma} \right).
$$

En vertu des hypothèses faites $\sum_{\gamma < \lambda < \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma}$ est un développement asymptotique de $h$, à la précision $g_\alpha/g_\gamma$; comme $h$ tend vers $0$ suivant $\mathfrak{F}$, la méthode décrite ci-dessus donne un développement asymptotique de $(1 + h)^v$, puis un développement de $|f|^v$ en multipliant par $|a_v|^{g_\gamma}$.

Sous les mêmes hypothèses sur $f$, on peut écrire
$$
\log |f| = \log |a_{\gamma g_\gamma}| + \log (1 + h)
$$
et $\log (1 + h)$ se développe comme il a été dit plus haut, la fonction $\log (1 + t)$ étant indéfiniment dérivable au voisinage de 0 ; si en outre $\log g_\gamma$ admet un développement asymptotique par rapport à $\mathscr{E}$, ou par rapport à une échelle $\mathscr{E}_1 \supset \mathscr{E}$, on obtient un développement asymptotique de $\log |f|$ en faisant la somme de deux développements asymptotiques.

#### Exemple {#fvr-v-s2-n4-exa-1 .statement}

On a $(1 + x)^{1/x} = \exp \left( \frac{1}{x} \log (1 + x) \right)$; lorsque $x$ tend vers $+\infty$, on a $\log (1 + x) = \log x + \log \left( 1 + \frac{1}{x} \right)$, d’où le développement asymptotique de $\frac{1}{x} \log (1 + x)$ par rapport à l’échelle des $x^\alpha (\log x)^\beta$:
$$
\frac{1}{x} \log (1 + x) = \frac{\log x}{x} + \frac{1}{x^2} - \frac{1}{2x^3} + o_1 \left( \frac{1}{x^3} \right).
$$
De ce développement, et du développement de Taylor
$$
e^u = 1 + u + \frac{u^2}{2} + \frac{u^3}{6} + o(u^3)
$$
au voisinage de $u = 0$, on tire par les méthodes exposées ci-dessus, le développement asymptotique
$$
(1 + x)^{1/x} = 1 + \frac{\log x}{x} + \frac{1}{2} \frac{(\log x)^2}{x^2} + \frac{1}{x^2} + \frac{1}{6} \frac{(\log x)^3}{x^3} + \frac{\log x}{x^3} - \frac{1}{2x^3} + o_2 \left( \frac{1}{x^3} \right)
$$
par rapport à l’échelle des $x^\alpha (\log x)^\beta$.

Les hypothèses et les notations restant les mêmes, le développement asymptotique de $e^t$ ne pose de nouveaux problèmes que lorsque $f \gg 1$; il faut alors distinguer deux cas, suivant que $g_\alpha \gg 1$ ou $g_\alpha \ll 1$. Dans le premier cas, la donnée du développement de $f$ ne permet pas d’obtenir une partie principale de $e^t$ relative à $\mathscr{E}$, car on ignore en général si le reste $r_\alpha$ tend vers 0, c’est-à-dire si $e^{r_\alpha}$ tend vers 1. Au contraire, si $g_\alpha \ll 1$, on a $r_\alpha \ll 1$, donc $e^t \sim \exp \left( \sum_{\lambda < \delta} a_{\lambda g_\lambda} \right)$. On peut préciser ce résultat : soit $a_{\gamma g_\gamma}$, la partie principale de $f$, et soit $\delta$ l’indice (tel que $\gamma < \delta \leq \alpha$) pour lequel $g_\delta = 1$; posons $f_1 = \sum_{\lambda < \delta} a_{\lambda g_\lambda}$, $f_2 = \sum_{\delta < \lambda \leq \alpha} a_{\lambda g_\lambda} + r_\alpha$; on a $f = f_1 + f_2$, donc $e^t = e^{f_1} e^{f_2}$, et la méthode générale exposée au début de ce no permet de former un développement asymptotique de $e^{f_2}$ (à partir du développement de Taylor de $e^t$ au point $t = 0$). On aura donc encore un développement asymptotique de $e^t$ si $e^{f_1} = \prod_{\lambda < \delta} \exp(a_{\lambda g_\lambda})$ appartient à $\mathscr{E}$, ou à une échelle $\mathscr{E}_1$ contenant $\mathscr{E}$.

#### Exemple {#fvr-v-s2-n4-exa-2 .statement}

On a $x^{x^{1/x}} = \exp \left( \log x . \exp \left( \frac{1}{x} \log x \right) \right)$; lorsque $x$ tend vers $+\infty$, on a $\log x \ll x$, d’où le développement asymptotique de $\log x . \exp \left( \frac{1}{x} \log x \right)$ par rapport à l’échelle des $x^\alpha (\log x)^\beta$ :
$$
\log x . \exp \left( \frac{1}{x} \log x \right) = \log x + \frac{(\log x)^2}{x} + \frac{1}{2} \frac{(\log x)^3}{x^2} + o \left( \frac{(\log x)^3}{x^2} \right).
$$

Tous les termes de ce développement à partir du second tendent vers 0; à partir de ce développement et du développement de Taylor $e^u = 1 + u + u^2/2 + o(u^2)$ au voisinage de $u = 0$, on tire
$$
x^{x^{1/x}} = x + (\log x)^2 + \frac{1}{2} \frac{(\log x)^4}{x} + \frac{1}{2} \frac{(\log x)^3}{x} + o \left( \frac{(\log x)^3}{x} \right).
$$

### 5. Développements asymptotiques à coefficients variables
On peut généraliser la notion de partie principale et celle de développement asymptotique, de la manière suivante. Soit $\mathscr{E}$ une échelle de comparaison formée de fonctions réelles (resp. complexes) telles que, pour chacune d’elles, il existe un ensemble de $\mathfrak{F}$ où la fonction ne s’annule en aucun point. Soit d’autre part $\mathcal{C}$ un ensemble de fonctions de $\mathscr{H}(\mathfrak{F}, V)$, satisfaisant aux trois conditions suivantes:

(CO_I) Pour toute fonction $a \in \mathcal{C}$, on a $a \ll 1$.

(CO_{II}) La relation $a \ll 1$ pour une fonction $a \in \mathcal{C}$ entraîne $a = 0$.

(CO_{III}) $\mathcal{C}$ est un espace vectoriel sur $\mathbf{R}$ (resp. $\mathbf{C}$).

Soit alors $f$ une fonction quelconque de $\mathscr{H}(\mathfrak{F}, V)$; s’il existe une fonction $g \in \mathscr{E}$ et une fonction non nulle $a \in \mathcal{C}$ telles que $f - a g \ll g$, on dira que $a g$ est une partie principale de $f$, relative à l’échelle de comparaison $\mathscr{E}$ et au domaine de coefficients $\mathcal{C}$. S’il existe une telle partie principale, elle est unique: supposons en effet qu’il existe deux telles parties principales $a_1 g_1$ et $a_2 g_2$; on ne peut avoir $g_1 \ll g_2$, car en vertu de (CO_I) on déduirait de là $a_1 g_1 \ll g_2$, et $f - a_1 g_1 \ll g_1 \ll g_2$, donc $f \ll g_2$; mais alors on aurait aussi $a_2 g_2 \ll g_2$, et par suite $a_2 \ll 1$, contrairement à l’hypothèse $a_2 \neq 0$ et à la condition (CO_{II}). On a donc nécessairement $g_1 = g_2$; des relations $f - a_1 g_1 \ll g_1$, $f - a_2 g_1 \ll g_1$, on tire alors $(a_2 - a_1) g_1 \ll g_1$ d’où $a_2 - a_1 \ll 1$, et par suite $a_2 = a_1$ en vertu de (CO_{II}) et (CO_{III}).

#### Exemple {#fvr-v-s2-n4-exa-3 .statement}

Pour $x$ réel tendant vers $+\infty$, les fonctions périodiques et bornées dans $\mathbf{R}$, ayant une même période $\tau$, satisfont aux conditions (CO_I), (CO_{II}) et (CO_{III}): en effet si $\lim_{x \to +\infty} a(x)_- = 0$, pour tout $\varepsilon > 0$ il existe $x_0$ tel que $x \geq x_0$ entraîne $|a(x)| \leq \varepsilon$; on en déduit qu’on a aussi $|a(x)| \leq \varepsilon$ pour $0 \leq x \leq \tau$, puisqu’il existe un entier $n$ tel que $x + n \tau \geq x_0$, et que $a(x) = a(x + n \tau)$; comme $\varepsilon$ est arbitraire, on a $a(x) = 0$ dans $[0, \tau]$, donc partout.

Avec les notations de V, p. 12, on dira que $\sum_{\lambda < \alpha} a_\lambda g_\lambda$, où les $a_\lambda$ appartiennent à $\mathcal{C}$ et sont nuls sauf un nombre fini d’entre eux, est un développement asymptotique de $f$ à coefficients dans $\mathcal{C}$, à la précision $g_\alpha$, si on a $f - \sum_{\lambda < \alpha} a_\lambda g_\lambda \ll g_\alpha$; pour tout indice $\mu$ tel que $a_\mu \neq 0$, $a_\mu g_\mu$ est alors la partie principale de $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$, relative à $\mathscr{E}$ et à $\mathcal{C}$, ce qui prouve l’unicité de développement asymptotique de $f$ (à la précision $g_\alpha$) lorsqu’il existe.

Les méthodes données au no 3 (V, p. 14) pour former un développement asymptotique de $f_1 + f_2$ ou de $[f_1, f_2]$ à partir de développements asymptotiques donnés de $f_1$ et $f_2$ s’appliquent encore aux développements à coefficients variables, à condition que les $[a_\lambda, b_\mu]$ appartiennent au domaine de coefficients $\mathcal{C}$ correspondant à l’espace normé $V$ ou admettent un développement asymptotique à coefficients dans $\mathcal{C}$.
