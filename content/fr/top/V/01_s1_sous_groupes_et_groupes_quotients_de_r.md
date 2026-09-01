---
book: top
book_title: General Topology
chapter: V
chapter_title: GROUPES À UN PARAMÈTRE
section: 1
section_title: Sous-groupes et groupes quotients de R
lang: fr
source: top-v-x-fr
pdf_pages: 0008-0012, 0022-0023
extraction: ocr
subsections:
    - "no": 1
      title: Sous-groupes fermés de $\mathbf{R}$
      page: 0
      pdf_page: 8
    - "no": 2
      title: Groupes quotients de $\mathbf{R}$
      page: 0
      pdf_page: 8
    - "no": 3
      title: Homomorphismes continus de $\mathbf{R}$ dans lui-même
      page: 2
      pdf_page: 9
    - "no": 4
      title: Définition locale d’un homomorphisme continu de $\mathbf{R}$ dans un groupe topologique
      page: 3
      pdf_page: 10
statements: 13
exercises: 3
content_sha256: aff9b8586066f9061c025ffbfc4d3d79fe587c27f300e1e028b40a65c384d5cf
---

## § 1. SOUS-GROUPES ET GROUPES QUOTIENTS DE $\mathbf{R}$

### 1. Sous-groupes fermés de $\mathbf{R}$

#### Proposition 1 {#top-v-s1-prop-1 .statement}

Tout sous-groupe fermé du groupe additif $\mathbf{R}$, distinct de $\mathbf{R}$ et de $\{0\}$, est un groupe discret de la forme $a.\mathbf{Z}$, où $a > 0$ (autrement dit, est formé des multiples entiers de $a$).

Montrons d’abord que tout sous-groupe non discret de $\mathbf{R}$ est partout dense. Si un sous-groupe $G$ de $\mathbf{R}$ n’est pas discret, pour tout $\varepsilon > 0$, il existe un point $x \neq 0$ de $G$ appartenant à l’intervalle $(-\varepsilon, +\varepsilon)$; comme les multiples entiers de $x$ appartiennent à $G$, tout intervalle de longueur $> \varepsilon$ contient un tel multiple, c’est-à-dire que $G$ est partout dense dans $\mathbf{R}$.

Tout sous-groupe fermé distinct de $\mathbf{R}$ est donc discret. Reste à montrer que tout sous-groupe discret $G$ de $\mathbf{R}$, non réduit à $0$, est de la forme $a.\mathbf{Z}$, où $a > 0$. Or, la relation $-G = G$ montre que l’ensemble $H$ des éléments $> 0$ de $G$ n’est pas vide; si $b \in H$, l’intersection de l’intervalle $[0, b]$ et de $G$ est un ensemble compact et discret, donc fini; soit $a$ le plus petit des éléments de $H$ contenus dans $[0, b]$; pour tout $x \in G$, posons $m = [x/a]$ (partie entière de $x/a$); on a $x - ma \in G$ et $0 \leq x - ma < a$; d’après la définition de $a$, $x - ma = 0$, ce qui prouve que $G = a.\mathbf{Z}$.

### 2. Groupes quotients de $\mathbf{R}$

Tout groupe quotient séparé de $\mathbf{R}$ est de la forme $\mathbf{R}/H$, où $H$ est un sous-groupe fermé de $\mathbf{R}$ (III, p. 13, prop. 18); donc, d’après la prop. 1 de V, p. 1:

#### Proposition 2 {#top-v-s1-prop-2 .statement}

Les groupes quotients séparés de $\mathbf{R}$, non réduits à l’élément neutre, sont les groupes $\mathbf{R}/a\mathbf{Z}$ ($a \geq 0$).

Si $a$ et $b$ sont des nombres $> 0$, l’automorphisme $x \mapsto (b/a)x$ de $\mathbf{R}$ transforme $a\mathbf{Z}$ en $b\mathbf{Z}$; donc (III, p. 17, Remarque 3) les groupes quotients $\mathbf{R}/a\mathbf{Z}$ et $\mathbf{R}/b\mathbf{Z}$ sont isomorphes; en d’autres termes:

#### Proposition 3 {#top-v-s1-prop-3 .statement}

Tout groupe quotient séparé de $\mathbf{R}$, distinct de $\mathbf{R}$ et non réduit à l’élément neutre, est isomorphe au groupe $\mathbf{R}/\mathbf{Z}$.

#### Définition 1 {#top-v-s1-def-1 .statement}

Le groupe topologique $\mathbf{R}/a\mathbf{Z}$ ($a > 0$) est appelé groupe additif des nombres réels modulo $a$. On désigne par $\mathbf{T}$ le groupe topologique $\mathbf{R}/\mathbf{Z}$; en tant qu’espace topologique, $\mathbf{T}$ est appelé tore à une dimension (par abus de langage, on appelle aussi « tore à une dimension » le groupe topologique $\mathbf{T}$).

#### Remarque 1 {#top-v-s1-n2-rem-1 .statement}

La relation $x \equiv y$ (mod. $a\mathbf{Z}$) s’écrit plus souvent $x \equiv y$ (mod. $a$) ou simplement $x \equiv y$ ($a$), et se lit « $x$ et $y$ sont congrus modulo $a$ »; elle signifie donc que $x - y$ est un multiple entier de $a$. Lorsque $a$ est entier, la relation induite sur $\mathbf{Z}$ par cette relation d’équivalence n’est autre que la congruence modulo $a$ (A, I, p. 46), ce qui justifie la notation précédente.

#### Remarque 2 {#top-v-s1-n2-rem-2 .statement}

Comme nous le verrons dans VI, p. 12, l’espace topologique $\mathbf{T}$ est homéomorphe au cercle $x^2 + y^2 = 1$ du plan numérique $\mathbf{R}^2$; le produit $\mathbf{T}^2$ est homéomorphe à un tore de révolution dans $\mathbf{R}^3$ (VII, p. 22, exerc. 15); d’où le nom de « tore à une dimension » employé pour désigner $\mathbf{T}$ (au chap. VII, p. 9, nous appellerons de même $\mathbf{T}^n$ le « tore à $n$ dimensions »).*.

#### Proposition 4 {#top-v-s1-prop-4 .statement}

Le tore $\mathbf{T}$ est un espace homéomorphe à l’espace quotient d’un intervalle fermé quelconque $[a, a + 1]$ de $\mathbf{R}$, obtenu en identifiant les extrémités de cet intervalle; il est compact, connexe et localement connexe.

En effet, tout $x \in \mathbf{R}$ est congru (mod. 1) à un nombre de l’intervalle $[a, a + 1]$, savoir $x - [x - a]$; donc $\mathbf{T}$ est image de cet intervalle par l’application canonique $\varphi$ de $\mathbf{R}$ sur $\mathbf{R}/\mathbf{Z}$, et par suite est compact et connexe (I, p. 62, th. 2 et I, p. 82, prop. 4). D’autre part, deux éléments distincts de l’intervalle $[a, a + 1]$ ne peuvent être congrus (mod. 1) que si ce sont les extrémités; de la compacité de $\mathbf{T}$, on conclut donc que $\mathbf{T}$ est homéomorphe à l’espace quotient de $[a, a + 1]$ obtenu en identifiant ses extrémités (I, p. 63, cor. 4 et I, p. 78, prop. 8). Enfin, comme $\mathbf{Z}$ est un sous-groupe discret de $\mathbf{R}$, $\mathbf{T} = \mathbf{R}/\mathbf{Z}$ est localement isomorphe à $\mathbf{R}$ (III, p. 13, prop. 19), et en particulier localement connexe (ce qui est aussi conséquence de I, p. 85, prop. 12).

#### Remarque {#top-v-s1-n2-rem-3 .statement}

On observera que l’application canonique $\varphi$ de $\mathbf{R}$ sur $\mathbf{T} = \mathbf{R}/\mathbf{Z}$, restreinte à l’intervalle semi-ouvert $[a, a + 1[$, est une application bijective et continue de cet intervalle sur $\mathbf{T}$; son application réciproque est continue en tout point de $\mathbf{T}$ distinct de $\varphi(a)$, discontinue au point $\varphi(a)$. On identifie parfois l’espace $\mathbf{T}$ avec l’intervalle $[a, a + 1[$, muni de la topologie image réciproque par $\varphi$ de celle de $\mathbf{T}$ (I, p. 13); cette topologie est bien entendu distincte de la topologie induite sur $[a, a + 1[$ par celle de $\mathbf{R}$.

### 3. Homomorphismes continus de $\mathbf{R}$ dans lui-même

#### Proposition 5 {#top-v-s1-prop-5 .statement}

Tout homomorphisme continu $f$ du groupe topologique $\mathbf{R}$ dans lui-même est de la forme $x \mapsto ax$, où $a \in \mathbf{R}$; c’est un automorphisme du groupe topologique $\mathbf{R}$ si $a \neq 0$.

En effet, pour tout $x \in \mathbf{R}$ et tout entier $p \in \mathbf{Z}$, on a $f(px) = pf(x)$; en remplaçant $x$ par $(1/p)x$, on en tire $f\left(\frac{1}{p}x\right) = \frac{1}{p}f(x)$, si $p \neq 0$; d’où quels que soient les entiers $p$ et $q \neq 0$, $f\left(\frac{p}{q}x\right) = \frac{p}{q}f(x)$; autrement dit, pour tout nombre rationnel $r$, $f(rx) = rf(x)$. Si maintenant $t$ est un nombre réel quelconque, on a, en vertu de la continuité de $f$ dans $\mathbf{R}$,

$$
f(tx) = \lim_{r \to t,\, r \in \mathbf{Q}} f(rx) = \lim_{r \to t,\, r \in \mathbf{Q}} rf(x) = (\lim_{r \to t,\, r \in \mathbf{Q}} r)f(x) = tf(x).
$$

En particulier, si $a = f(1)$, on a $f(t) = at$, d’où la proposition.

Le groupe des automorphismes du groupe topologique $\mathbf{R}$ est donc isomorphe au groupe multiplicatif $\mathbf{R}^*$ des nombres réels non nuls.

#### Corollaire {#top-v-s1-n3-cor-1 .statement}

Soit $G$ un groupe topologique isomorphe à $\mathbf{R}$; pour tout $a \in G$, il existe un homomorphisme continu et un seul $f_a$ de $\mathbf{R}$ dans $G$, tel que $f_a(1) = a$; cet homomorphisme est un isomorphisme de $\mathbf{R}$ sur $G$ si $a$ est distinct de l’élément neutre de $G$.

### 4. Définition locale d’un homomorphisme continu de $\mathbf{R}$ dans un groupe topologique

Étant donnés un groupe $G$ et une partie $A$ de $G$ engendrant $G$, il est clair que, si deux homomorphismes $f, g$ de $G$ dans un groupe $G'$ prennent la même valeur en tout point de $A$, ils sont égaux. Mais les valeurs dans $A$ d’un homomorphisme $f$ de $G$ dans $G'$ ne peuvent en général être prises arbitrairement; $G$ et $G'$ étant notés multiplicativement, ces valeurs doivent satisfaire à la condition

$$
f(xy) = f(x)f(y)
$$

pour tout couple $(x, y)$ tel que $x \in A, y \in A$ et $xy \in A$; cette condition nécessaire n’est d’ailleurs pas suffisante en général.

En particulier, un isomorphisme local d’un groupe topologique $G$ à un groupe topologique $G'$ ne peut pas toujours se prolonger en un homomorphisme (continu ou non) de $G$ dans $G'$. Par exemple, un isomorphisme local $f$ de $\mathbf{T}$ à $\mathbf{R}$ ne peut se prolonger en un homomorphisme de $\mathbf{T}$ dans $\mathbf{R}$: en effet, si $f$ est défini dans un voisinage $V$ de $0$, il existe un entier $p > 0$ tel que la classe $x$ (mod. $\mathbf{Z}$) de $1/p$ appartienne à $V$; comme $x$ est un élément d’ordre $p$ dans $\mathbf{T}$, son image par tout homomorphisme de $\mathbf{T}$ dans $\mathbf{R}$ est nécessairement $0$, donc distincte de $f(x)$ par hypothèse.

Le groupe topologique $\mathbf{R}$ jouit à cet égard de la propriété suivante:

#### Proposition 6 {#top-v-s1-prop-6 .statement}

Soit $I$ un intervalle de $\mathbf{R}$, contenant $0$ et non réduit à ce point; soit $f$ une application continue de $I$ dans un groupe topologique $G$ (noté multiplicativement), telle que $f(x + y) = f(x)f(y)$ pour tout couple de points $x, y$ tels que $x \in I, y \in I$ et $x + y \in I$. Il existe un homomorphisme continu et un seul de $\mathbf{R}$ dans $G$ qui prolonge $f$.

L’unicité du prolongement de $f$ (s’il existe) résulte des remarques qui précédent, puisque I engendre le groupe $\mathbf{R}$; reste à en démontrer l’existence.

Si $n$ est un entier $> 0$, et si on a $x \in I$ et $nx \in I$, on a $f(nx) = (f(x))^n$, comme on le voit par récurrence sur $n$, en observant que, dans ces conditions, on a $mx \in I$ pour tout entier $m$ tel que $1 \leq m \leq n$. Posons $J = \bigcup_{n \in \mathbf{N}} nI$; $J$ est la droite $\mathbf{R}$, ou bien l’un des intervalles $\{0, +\infty[\text{ ou }]-\infty, 0\}$, suivant que 0 est ou non intérieur à $I$; si $x \in J$, on a $x/n \in I$ dès que $n$ est un entier $> 0$ assez grand. Soit $x \in J$, et soient $m, n$ deux entiers $> 0$ tels que $x/n \in I$ et $x/m \in I$; on a $x/mn \in I$, donc

$$
f\left( \frac{x}{m} \right) = \left( f\left( \frac{x}{mn} \right) \right)^n, \quad \text{et} \quad f\left( \frac{x}{n} \right) = \left( f\left( \frac{x}{mn} \right) \right)^m;
$$

par conséquent, l’élément $(f(x/n))^n$ de G est le même pour tous les entiers $n > 0$ satisfaisant à la condition $x/n \in I$. Désignons cet élément par $f_1(x)$; $f_1$ est une application de $J$ dans G, qui coïncide avec $f$ dans I et est donc continue au point 0 (par rapport à $J$). Soient $x, y$ deux éléments de $J$, $n$ un entier $> 0$ assez grand pour que l’on ait $x/n \in I, y/n \in I, (x+y)/n \in I$; on a

$$
f\left( \frac{x+y}{n} \right) = f\left( \frac{x}{n} \right) f\left( \frac{y}{n} \right) = f\left( \frac{y}{n} \right) f\left( \frac{x}{n} \right),
$$

ce qui prouve que $f(x/n)$ et $f(y/n)$ sont permutables; par définition de $f_1$, on a donc $f_1(x+y) = f_1(x)f_1(y)$. Si $J = \mathbf{R}$, la proposition est démontrée. Sinon, supposons par exemple qu’on ait $J = (0, +\infty[$; pour tout $x < 0$, posons

$$
f_1(x) = (f_1(-x))^{-1}.
$$

La relation $f_1(x+y) = f_1(x)f_1(y)$ reste alors valable quels que soient $x \in \mathbf{R}$, $y \in \mathbf{R}$; c’est immédiat pour $x < 0$ et $y < 0$; pour $x \geq 0, y < 0, x+y \geq 0$, on a $f_1(x) = f_1(x+y)f_1(-y)$, d’où la propriété annoncée; de même pour $x \geq 0, y < 0, x+y < 0$, car on a alors $f_1(-y) = f_1(-x-y)f_1(x)$; démonstrations analogues pour $x < 0$ et $y \geq 0$. On voit donc que $f_1$ est un homomorphisme de $\mathbf{R}$ dans G; on a par suite $f_1(0) = e$ (élément neutre de G), et comme $f_1$ est une fonction continue par rapport à $J$, elle a au point 0 une limite à droite égale à $e$; comme $f_1(-x) = (f_1(x))^{-1}$, $f_1$ a aussi au point 0 une limite à gauche égale à $e$; elle est donc continue en 0, ce qui achève la démonstration.

#### Corollaire {#top-v-s1-n4-cor-1 .statement}

*Soit $f$ un isomorphisme local de $\mathbf{R}$ à un groupe topologique $G$; il existe un morphisme strict et un seul de $\mathbf{R}$ sur un sous-groupe ouvert de $G$, qui coïncide avec $f$ en tous les points d’un voisinage de 0.*

En effet, soit $\bar{f}$ l’homomorphisme continu de $\mathbf{R}$ dans G qui coïncide avec $f$ en tous les points d’un intervalle ouvert I contenant 0 et contenu dans l’ensemble où est défini $f$; $\bar{f}(\mathbf{R})$ contient par hypothèse un voisinage de l’élément neutre de G, donc (III, p. 7, corollaire) est un sous-groupe ouvert de G; en outre, $\bar{f}$ est un morphisme strict de $\mathbf{R}$ sur $\bar{f}(\mathbf{R})$, d’après III, p. 16, prop. 24.

#### Proposition 7 {#top-v-s1-prop-7 .statement}

Tout groupe topologique connexe G, localement isomorphe à $\mathbf{R}$, est isomorphe à $\mathbf{R}$ ou à $\mathbf{T}$.

En effet, un isomorphisme local de $\mathbf{R}$ à G se prolonge en un morphisme strict de $\mathbf{R}$ sur un sous-groupe ouvert de G (cor. de la prop. 6), donc sur G lui-même puisque G est connexe. Il s’ensuit que G est isomorphe à un groupe quotient de $\mathbf{R}$; comme il est séparé et non réduit à l’élément neutre (puisqu’il est localement isomorphe à $\mathbf{R}$), il est isomorphe à $\mathbf{R}$ ou à $\mathbf{T}$ d’après la prop. 3 de V, p. 2.

## EXERCICES {#top-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
