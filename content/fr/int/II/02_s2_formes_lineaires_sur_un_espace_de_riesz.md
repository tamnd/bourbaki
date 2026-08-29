---
book: int
book_title: Integration
chapter: II
chapter_title: Espaces de Riesz
section: 2
section_title: Formes linéaires sur un espace de Riesz
lang: fr
source: int-i-iv-fr
pdf_pages: 0029-0035, 0041-0043
extraction: ocr
subsections:
    - "no": 1
      title: Formes linéaires positives sur un espace de Riesz
      page: 0
      pdf_page: 29
    - "no": 2
      title: Formes linéaires relativement bornées
      page: 0
      pdf_page: 31
statements: 13
exercises: 9
content_sha256: d8983cd1a81982f6dc43554cf1e2755d441bd557cd0e5771e9ba9c357930170d
---

## § 2. Formes linéaires sur un espace de Riesz

### 1. Formes linéaires positives sur un espace de Riesz

Rappelons la définition suivante (Esp. vect. top., chap. II, 2e éd., § 2, n° 5):

#### Définition 1 {#int-ii-s2-def-1 .statement}

Etant donné un espace vectoriel ordonné E, on dit qu’une forme linéaire L sur E est positive si, pour tout x $\geqslant 0$ dans E, on a $L(x) \geqslant 0$.

Comme $L(y) - L(x) = L(y - x)$, il revient au même de dire que la relation $x \leqslant y$ entraîne $L(x) \leqslant L(y)$, ou encore que $L$ est une fonction croissante dans E.

#### Exemple 1 {#int-ii-s2-n1-exa-1 .statement}

Soient A un ensemble quelconque, E un sous-espace de l’espace $\mathbf{R}^A$ de toutes les fonctions numériques définies dans A. Pour tout élément $a \in A$, l’application $x \mapsto x(a)$ est une forme linéaire positive sur E.

#### Exemple 2 {#int-ii-s2-n1-exa-2 .statement}

Soit $I = [a, b]$ un intervalle compact de $\mathbf{R}$, E l’espace de Riesz formé des fonctions numériques réglées dans I (Fonct. var. réelle, chap. II, §1, n° 3); l’application $x \mapsto \int_a^b x(t)\, dt$ est une forme linéaire positive sur E.

#### Exemple 3 {#int-ii-s2-n1-exa-3 .statement}

Soient F un ensemble quelconque, $\mathcal{U}$ un ultrafiltre sur F (Top. gén., chap. I, 3e éd., § 6, n° 4), E l’espace de Riesz $\mathscr{B}(F)$ des fonctions numériques bornées dans F. Pour tout $x \in E$, $\lim_{\mathcal{U}} x(t)$ existe, car $x(\mathcal{U})$ est une base d’ultrafiltre sur l’ensemble relativement compact $x(F)$, et par suite est convergente. En outre, si $x \geqslant 0$, on a $\lim_{\mathcal{U}} x(t) \geqslant 0$ en vertu du principe de prolongement des inégalités; l’application $x \mapsto \lim_{\mathcal{U}} x$ est donc une forme linéaire positive sur E. Si on prend pour $\mathcal{U}$ l’ultrafiltre formé des ensembles contenant un élément $a \in F$, on retrouve la forme linéaire positive $x \mapsto x(a)$ (exemple 1).

#### Proposition 1 {#int-ii-s2-prop-1 .statement}

Soient E un espace vectoriel ordonné, L une application de E dans $\mathbf{R}$ telle que $L(x + y) = L(x) + L(y)$ et que la relation $x \geqslant 0$ entraîne $L(x) \geqslant 0$; alors, pour tout scalaire $\lambda$ et tout $x \geqslant 0$, on a $L(\lambda x) = \lambda L(x)$.

Comme $L(-x) = -L(x)$ (L étant une représentation du groupe additif E dans $\mathbf{R}$), on peut se borner au cas où $\lambda \geqslant 0$. Pour tout entier $n \geqslant 0$, on a $L(nx) = nL(x)$, d’où $L((1/n)x) = (1/n)L(x)$ et par suite $L(rx) = rL(x)$ pour tout nombre rationnel $r \geqslant 0$. D’autre part $L$ est croissante dans E; si $r$ et $r'$ sont deux nombres rationnels tels que $r \leqslant \lambda \leqslant r'$, on a donc $rL(x) \leqslant L(\lambda x) \leqslant r'L(x)$; comme $rL(x)$ et $r'L(x)$ diffèrent d’aussi peu qu’on veut de $\lambda L(x)$, on a $L(\lambda x) = \lambda L(x)$.

#### Proposition 2 {#int-ii-s2-prop-2 .statement}

Soient E un espace vectoriel réel, C un cône convexe de sommet 0 dans E tel que $E = C - C$, $x \mapsto M(x)$ une application de C dans $\mathbf{R}$ telle que, pour $x \in C$, $y \in C$, $\lambda \geqslant 0$, $\mu \geqslant 0$, on ait $M(\lambda x + \mu y) = \lambda M(x) + \mu M(y)$. Alors il existe une forme linéaire et une seule $L$ qui prolonge $M$ à $E$.

En effet, par hypothèse, tout $z \in E$ peut s’écrire $z = y - x$, où $x, y$ appartiennent à $C$; en outre, si $z = y' - x'$ avec $x' \in C, y' \in C$, on a $M(y) - M(x) = M(y') - M(x')$; en effet, de la relation $y - x = y' - x'$, on tire $y + x' = x + y'$, et par suite $M(y) + M(x') = M(x) + M(y')$. Désignons par $L(z)$ la valeur commune de $M(y) - M(x)$ pour toute expression de $z$ comme différence $y - x$ de deux éléments de $C$; on vérifie immédiatement que $L$ est une forme linéaire sur $E$ prolongeant $M$; l’unicité de $L$ résulte de ce que $C$ engendre l’espace $E$.

#### Proposition 3 {#int-ii-s2-prop-3 .statement}

Soient $E$ un espace vectoriel ordonné filtrant, $P$ l’ensemble des éléments $\geqslant 0$ de $E$, $x \mapsto M(x)$ une application de $P$ dans $\mathbf{R}$, à valeurs $\geqslant 0$ et telle que $M(x + y) = M(x) + M(y)$ quels que soient $x, y$ dans $P$. Il existe alors une forme linéaire positive et une seule $L$ qui prolonge $M$ à $E$.

Comme $E = P - P$, le même raisonnement que dans la prop. 2 prouve d’abord l’existence et l’unicité d’une application additive $L$ de $E$ dans $\mathbf{R}$ prolongeant $M$. La prop. 1 montre alors que, pour $\lambda \geqslant 0$ et pour tout $x \in P$, on a $L(\lambda x) = \lambda L(x)$, d’où résulte aussitôt que $L$ est une forme linéaire.

### 2. Formes linéaires relativement bornées

Soit $E$ un espace vectoriel ordonné filtrant. Soit $Q$ l’ensemble des formes linéaires positives sur $E$; c’est une partie du dual algébrique $E^*$ de $E$ (espace de toutes les formes linéaires sur $E$). Il est immédiat que $Q + Q \subset Q$ et $\lambda Q \subset Q$ pour tout scalaire $\lambda > 0$ (en d’autres termes, $Q$ est un cône convexe dans $E^*$). En outre, on a $Q \cap (-Q) = \{0\}$, car si $L$ et $-L$ sont toutes deux des formes linéaires positives, on a $L(x) \geqslant 0$ et $L(x) \leqslant 0$ pour tout $x \geqslant 0$, d’où $L(x) = 0$ pour tout $x \geqslant 0$, et par suite $L = 0$ (n° 1, prop. 3). L’ensemble $Q$ définit donc sur $E^*$ une relation d’ordre $L \leqslant M$, équivalente à « $M - L$ est une forme linéaire positive sur $E$ », ou encore à « pour tout $x \geqslant 0$, $L(x) \leqslant M(x)$ »; les éléments $\geqslant 0$ dans $E^*$ pour cette structure d’ordre sont les formes linéaires positives (ce qui justifie la terminologie introduite). Soit $\Omega$ le sous-espace vectoriel de $E^*$ engendré par $Q$, c’est-à-dire l’ensemble des formes linéaires sur $E$ qui sont différences de deux formes linéaires positives; nous allons donner une autre caractérisation des éléments de $\Omega$ lorsque E est un espace de Riesz.

#### Définition 2 {#int-ii-s2-def-2 .statement}

Etant donné un espace de Riesz E, on dit qu’une forme linéaire L sur E est relativement bornée si, pour tout $x \geqslant 0$ dans E, L est bornée dans l’ensemble des $y \in E$ tels que $|y| \leqslant x$.

#### Théorème 1 {#int-ii-s2-thm-1 .statement}

1° Pour qu’une forme linéaire L sur un espace de Riesz E soit relativement bornée, il faut et il suffit qu’elle soit la différence de deux formes linéaires positives.

2° L’espace vectoriel ordonné $\Omega$ des formes linéaires relativement bornées sur E est un espace de Riesz complètement réticulé.

Si $L = U - V$, où U et V sont deux formes linéaires positives sur E, la relation $-x \leqslant y \leqslant x$ entraîne $-U(x) \leqslant U(y) \leqslant U(x)$ et $-V(x) \leqslant V(y) \leqslant V(x)$ d’où aussitôt $|L(y)| \leqslant U(x) + V(x)$; L est donc relativement bornée. Supposons inversement que L soit relativement bornée; tout revient à prouver qu’il existe une forme linéaire positive N telle que, pour tout $x \geqslant 0$, on ait $N(x) \geqslant L(x)$, car alors $N - L$ sera une forme linéaire positive.

Or, si une forme linéaire positive N a cette propriété, on a, pour tout $x \geqslant 0$ et pour $0 \leqslant y \leqslant x$, $N(x) \geqslant N(y) \geqslant L(y)$, et par suite $N(x) \geqslant \sup_{0 \leqslant y \leqslant x} L(y)$; si nous prouvons que la fonction numérique $x \mapsto M(x) = \sup_{0 \leqslant y \leqslant x} L(y)$, définie dans l’ensemble P des éléments $\geqslant 0$ de E, se prolonge en une forme linéaire positive sur E (qu’on notera encore M), nous aurons démontré la première partie du théorème, et prouvé en outre que M est la borne supérieure de 0 et L dans $\Omega$. Comme $M(x) \geqslant 0$ dans P, tout revient à prouver que, pour deux éléments quelconques $x \geqslant 0$, $x' \geqslant 0$ de E, on a $M(x + x') = M(x) + M(x')$ (n° 1, prop. 3). D’après la définition, on a

$$
M(x) + M(x') = \sup_{0 \leqslant y \leqslant x} L(y) + \sup_{0 \leqslant y' \leqslant x'} L(y')
= \sup_{0 \leqslant y \leqslant x,\ 0 \leqslant y' \leqslant x'} L(y + y') \leqslant M(x + x').
$$

D’autre part, pour tout z tel que $0 \leqslant z \leqslant x + x'$, on a $x + x' = z + u$ avec $u \geqslant 0$; en vertu du lemme de décomposition (§ 1, n° 1), il existe donc deux éléments y, $y'$ tels que $0 \leqslant y \leqslant x$, $0 \leqslant y' \leqslant x'$ et que $z = y + y'$, $u = (x - y) + (x' - y')$; d’où

$$
L(z) = L(y) + L(y') \leqslant M(x) + M(x'),
$$

et par suite $M(x + x') = \sup_{0 \leq z \leq x + x'} L(z) \leq M(x) + M(x')$, ce qui achève de démontrer la première partie du théorème. De plus, nous avons montré ainsi que $\Omega$ est un espace de Riesz, et que, pour toute forme linéaire relativement bornée $L$ sur $E$, et pour tout $x \geq 0$, on a

(1)
$$
L^+(x) = \sup_{0 \leq y \leq x} L(y).
$$

Reste à voir que $\Omega$ est complètement réticulé ; pour cela il suffit de montrer qu’un ensemble $H$ de formes linéaires positives, majoré et filtrant pour la relation $\leq$, a une borne supérieure dans $\Omega$.

Or, on a plus généralement le lemme suivant :

#### Lemme 1 {#int-ii-s2-lem-1 .statement}

Soient $E$ un espace vectoriel ordonné filtrant, $E^*$ son dual, ordonné en prenant pour éléments positifs les formes linéaires positives. Soit $(u_\alpha)$ une famille filtrante croissante d’éléments de $E^*$. Si, pour tout $x \geq 0$ dans $E$, on a $\sup u_\alpha(x) < +\infty$, alors la famille $(u_\alpha)$ admet une borne supérieure $u$ dans $E^*$, et pour tout $x \geq 0$ dans $E$, on a

(2)
$$
u(x) = \sup_\alpha u_\alpha(x).
$$

Dans l’ensemble $P$ des $x \geq 0$ dans $E$, définissons en effet l’application $u$ par la formule (2); il est immédiat que pour $\lambda \geq 0$ et $x \in P$, on a $u(\lambda x) = \lambda u(x)$; pour prouver le lemme, il suffit donc, en vertu de la prop. 2 du n° 1, de montrer que l’on a
$$
u(x + y) = u(x) + u(y)
$$
pour $x, y$ dans $P$. Or cela est immédiat si l’on remarque que l’on a $u(x) = \lim u_\alpha(x)$ suivant l’ensemble filtrant des indices (théorème de la limite monotone).

De la formule (1) on déduit aussitôt que si $L$ et $M$ sont deux formes linéaires relativement bornées sur $E$, on a, pour tout $x \geq 0$

(3)
$$
\begin{cases}
\sup (L, M)(x) = \sup_{y \geq 0, z \geq 0, y + z = x} (L(y) + M(z)) \\
\inf (L, M)(x) = \inf_{y \geq 0, z \geq 0, y + z = x} (L(y) + M(z)).
\end{cases}
$$

En particulier, si dans la première de ces formules, on remplace $M$ par $-L$, il vient

$$
|L|(x) = \sup_{y \geq 0, z \geq 0, y + z = x} L(y - z).
$$

Or, si $x = y + z, y \geq 0$ et $z \geq 0$, on a $-x \leq y - z \leq x$; inversement, la relation $|u| \leq x$ entraîne $L(u) \leq |L|(|u|) \leq |L|(x)$. On en déduit la formule

(4)
$$
|L|(x) = \sup_{|y| \leq x} L(y) \quad \text{pour } x \geq 0,
$$
d’où en particulier
(5)
$$
|L(x)| \leq |L|(|x|)
$$
pour tout $x \in \mathbf{E}$.

#### Proposition 4 {#int-ii-s2-prop-4 .statement}

*Pour que deux formes linéaires positives $L, M$ sur un espace de Riesz $\mathbf{E}$ soient étrangères dans l’espace $\Omega$, il faut et il suffit que, pour tout nombre $\varepsilon > 0$ et pour tout $x \geq 0$ dans $\mathbf{E}$, il existe deux éléments $y \geq 0, z \geq 0$ de $\mathbf{E}$ tels que $x = y + z$ et $L(y) + M(z) \leq \varepsilon$.*

En effet, d’après la seconde formule (3), cette condition exprime que $\inf (L, M) = 0$.

#### Proposition 5 {#int-ii-s2-prop-5 .statement}

*Soit $L$ une forme linéaire positive sur un espace de Riesz $\mathbf{E}$. Pour qu’une forme linéaire positive $M$ sur $\mathbf{E}$ appartienne à la bande engendrée par $L$ dans $\Omega$, il faut et il suffit que, pour tout $x \geq 0$ dans $\mathbf{E}$ et tout nombre $\varepsilon > 0$, il existe un nombre $\delta > 0$ tel que les relations $0 \leq y \leq x$ et $L(y) \leq \delta$ entraînent $M(y) \leq \varepsilon$.*

Montrons d’abord que la condition est nécessaire. Si $M \geq 0$ appartient à la bande engendrée par $L$ dans $\Omega$, on a (§ 1, n° 5, cor. de la prop. 6) $M = \sup_n (\inf (nL, M))$. Si on pose
$$
U_n = M - \inf (nL, M),
$$
$U_n$ est donc une forme linéaire positive sur $\mathbf{E}$ et on a $\inf_n U_n = 0$ dans $\Omega$; par suite (lemme 1) $U_n(x)$ tend vers 0 lorsque $n$ croît indéfiniment, et il existe $n$ tel que $U_n(x) \leq \varepsilon/2$. Le nombre $n$ étant ainsi fixé, on a $U_n(y) \leq \varepsilon/2$ pour tout $y$ tel que $0 \leq y \leq x$, donc la relation $0 \leq y \leq x$ entraîne
$$
M(y) \leq \frac{\varepsilon}{2} + \inf (nL, M)(y) \leq \frac{\varepsilon}{2} + nL(y);
$$

si $y$ est tel que $L(y) \leq \varepsilon/2n$, on a donc $M(y) \leq \varepsilon$, ce qui établit notre assertion.

Montrons maintenant que la condition est suffisante. Pour toute forme linéaire positive $M$ sur $E$, on peut écrire $M = U + V$, où $U$ appartient à la bande engendrée par $L$ dans $\Omega$ et où $V$ est étrangère à $L$, $U$ et $V$ étant positives ($§ 1$, n° 5, th. 1). Si $M$ satisfait à la condition de l’énoncé, il en est de même de $V = M - U$, puisque $0 \leq V \leq M$. Nous allons en déduire que $V = 0$. En effet, pour tout $x \geq 0$ dans $E$ et tout nombre $\eta > 0$, il existe deux éléments $y \geq 0, z \geq 0$ de $E$ tels que $x = y + z$ et $L(y) + V(z) \leq \eta$ (prop. 4); donnons-nous arbitrairement un nombre $\varepsilon > 0$, et choisissons $\eta \leq \varepsilon$ tel que les relations $0 \leq u \leq x$ et $L(u) \leq \eta$ entraînent $V(u) \leq \varepsilon$; $y$ et $z$ étant alors déterminés comme ci-dessus, on a $L(y) \leq \eta$, donc $V(y) \leq \varepsilon$ et par suite

$$
V(x) = V(y) + V(z) \leq \varepsilon + \eta \leq 2\varepsilon;
$$

$\varepsilon$ étant arbitraire, on a $V(x) = 0$ pour tout $x \geq 0$, c’est-à-dire $V = 0$.

#### Exemple {#int-ii-s2-n2-exa-1 .statement}

Soit $E$ un espace de Riesz, muni d’une topologie localement convexe, compatible avec sa structure d’espace vectoriel ordonné (*Esp. vect. top.*, chap. II, 2e éd., § 2, n° 7). Soit $E'$ le dual topologique de $E$, et supposons en outre que le cône $P$ des éléments $\geq 0$ de $E$ soit *complet pour la topologie affaiblie* $\sigma(E, E')$. Alors toute forme linéaire continue $x' \in E'$ est *relativement bornée*, car on sait (*Esp. vect. top.*, chap. II, 2e éd., § 6, n° 8, cor. 2 de la prop. 1) que dans ces conditions, pour tout $x \geq 0$ dans $E$, l’ensemble des $y \in E$ tels que $|y| \leq x$ est *compact* pour $\sigma(E, E')$. On en déduit que $E$ est alors *complètement réticulé*; en effet ($§ 1$, n° 3, prop. 2) il suffit de montrer que pour tout ensemble $H \subset E$ majoré et filtrant pour $\leq$, le filtre des sections $\mathfrak{F}$ de $H$ est *convergent dans E pour la topologie* $\sigma(E, E')$ (cette dernière étant compatible avec la structure d’espace vectoriel ordonné de $E$). Par translation, on peut supposer que $H \subset P$, et il suffit donc de montrer que $\mathfrak{F}$ est un *filtre de Cauchy* pour $\sigma(E, E')$, ou encore que toute forme linéaire continue $x' \in E'$ a une limite suivant $\mathfrak{F}$. Mais cela résulte aussitôt du th. de la limite monotone si $x'$ est une forme linéaire *positive*; et comme toute forme linéaire $x' \in E'$ est différence de deux formes linéaires positives (th. 1), notre assertion est démontrée.

## EXERCICES {#int-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
