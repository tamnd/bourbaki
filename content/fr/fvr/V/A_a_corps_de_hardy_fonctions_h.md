---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: ÉTUDE LOCALE DES FONCTIONS
section: 0
section_title: Corps de Hardy. Fonctions (H)
appendix: true
lang: fr
source: fvr-i-vii-fr
book_pages: FVR V.51-FVR V.55
pdf_pages: 0241-0253, 0256-0260
extraction: ocr
subsections:
    - "no": 1
      title: Corps de Hardy
      page: 113
      pdf_page: 241
    - "no": 2
      title: Extension d’un corps de Hardy
      page: 37
      pdf_page: 242
    - "no": 3
      title: Comparaison des fonctions d’un corps de Hardy
      page: 39
      pdf_page: 244
    - "no": 4
      title: Fonctions (H)
      page: 41
      pdf_page: 246
    - "no": 5
      title: Exponentielles et logarithmes itérés
      page: 41
      pdf_page: 246
    - "no": 6
      title: Fonction réciproque d’une fonction (H)
      page: 44
      pdf_page: 249
statements: 21
exercises: 1
content_sha256: 8119442795d3361e275b51c13bcd3eeebe54a25fda7fe5a05143ee7ff54ce8e5
---

## APPENDICE

# CORPS DE HARDY. FONCTIONS (H)

### 1. Corps de Hardy

Soit $\mathfrak{F}$ la base de filtre sur $\mathbf{R}$ constituée par les intervalles de la forme $[x_0, +\infty[$. Rappelons que, dans l’ensemble $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ des fonctions numériques définies dans des parties appartenant à $\mathfrak{F}$, nous avons défini la relation d’équivalence $R_\infty$: « il existe un ensemble $M \in \mathfrak{F}$ tel que $f(x) = g(x)$ dans $M$ » (V, p. 2), et que l’ensemble quotient $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$ est muni d’une structure d’anneau ayant un élément unité.

#### Définition 1 {#fvr-v-a0-def-1 .statement}

Étant donné un sous-ensemble $\mathfrak{A}$ de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, on dit que $\mathfrak{A}/R_\infty$ (image canonique de $\mathfrak{A}$ dans $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$) est un corps de Hardy, si $\mathfrak{A}$ satisfait aux conditions suivantes:
1° $\mathfrak{A}/R_\infty$ est un sous-corps de l’anneau $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$.
2° Toute fonction de $\mathfrak{A}$ est continue et dérivable dans un intervalle $[a, +\infty[$ (dépendant de la fonction), et la classe suivant $R_\infty$ de sa dérivée appartient à $\mathfrak{A}/R_\infty$.

L’hypothèse que $\mathfrak{A}/R_\infty$ est un corps équivaut aux conditions suivantes: si $f \in \mathfrak{A}$ et $g \in \mathfrak{A}$, $f + g$ et $fg$ sont égales à des fonctions de $\mathfrak{A}$ dans un ensemble de $\mathfrak{F}$; en outre, si $f$ n’est pas identiquement nulle dans un ensemble de $\mathfrak{F}$, il existe un ensemble $M$ de $\mathfrak{F}$ dans lequel $f$ ne s’annule pas, $1/f$ étant égale à une fonction de $\mathfrak{A}$ dans $M$; d’après la condition 2°, on peut toujours supposer $M$ pris tel que $f$ soit continue dans $M$, et par suite garde un signe constant dans cet intervalle.

Par abus de langage, si $\mathfrak{A}$ est tel que $\mathfrak{A}/R_\infty$ soit un corps de Hardy, nous dirons dans ce qui suit que $\mathfrak{A}$ lui-même est un corps de Hardy.

#### Exemple 1 {#fvr-v-a0-n1-exa-1 .statement}

Tout corps de Hardy contient le corps des constantes rationnelles (plus petit corps de caractéristique 0, cf. A, V, § 1), qu’on peut identifier au corps $\mathbf{Q}$; d’ailleurs, comme deux constantes ne sont congrues modulo $R_{\infty}$ que si elles sont égales, $\mathbf{Q}/R_{\infty}$ est identique à $\mathbf{Q}$. Les *constantes réelles* forment aussi un corps de Hardy, qu’on peut identifier à $\mathbf{R}$.

#### Exemple 2 {#fvr-v-a0-n1-exa-2 .statement}

Un exemple plus important de corps de Hardy est l’*ensemble des fonctions rationnelles à coefficients réels*, que nous noterons $\mathbf{R}(x)$ par abus de langage; si $f(x) = p(x)/q(x)$ est une fonction rationnelle à coefficients réels, non identiquement nulle, elle est continue, dérivable et $\neq 0$ dans l’intervalle $(a, +\infty[$, où $a$ est strictement supérieur à la plus grande des racines réelles des polynômes $p(x)$ et $q(x)$; donc tout élément de $\mathbf{R}(x)/R_{\infty}$ autre que 0 est inversible. On notera encore que deux fonctions rationnelles ne peuvent être congrues modulo $R_{\infty}$ que si elles sont égales, donc $\mathbf{R}(x)/R_{\infty}$ peut encore être identifié à $\mathbf{R}(x)$.

### 2. Extension d’un corps de Hardy

Étant donné un corps de Hardy $\mathfrak{K}$, nous allons voir comment on peut former de nouveaux corps de Hardy $\mathfrak{K}' \supset \mathfrak{K}$ tels que $\mathfrak{K}'/R_{\infty}$ s’obtienne par *adjonction* à $\mathfrak{K}/R_{\infty}$ (au sens algébrique du terme, cf. A, V, § 2) de nouveaux éléments, d’une forme que nous allons préciser.

#### Lemme 1 {#fvr-v-a0-lem-1 .statement}

*Soient $a(x)$, $b(x)$ des fonctions numériques continues et ne changeant pas de signe dans un intervalle $(x_0, +\infty[$. Si, dans cet intervalle, la fonction $y(x)$ est continue et dérivable et vérifie l’identité*

$$
y' = ay + b
$$

*il existe un intervalle $(x_1, +\infty[$ dans lequel $y$ ne change pas de signe.*

En effet, posons $z(x) = y(x) \exp \left( -\int_{x_0}^x a(t)\,dt \right)$ (cf. IV, p. 22); on a, d’après (1), $z'(x) = b(x) \exp \left( -\int_{x_0}^x a(t)\,dt \right)$. Si $b(x) \geqslant 0$ pour $x \geqslant x_0$, $z$ est croissante dans cet intervalle, donc, ou bien est $< 0$ dans tout l’intervalle, ou bien est nulle dans un intervalle $(x_1, +\infty[$, ou bien est $> 0$ dans un intervalle $(x_1, +\infty[$; comme $y$ a le même signe que $z$, la proposition est démontrée dans ce cas. Raisonnement analogue si $b(x) \leqslant 0$ pour $x \geqslant x_0$.

#### Remarque {#fvr-v-a0-n2-rem-1 .statement}

Cette propriété si élémentaire ne s’étend pas aux équations différentielles linéaires d’ordre $> 1$; par exemple, la fonction $y = \sin x$ satisfait à $y'' + y = 0$, mais change de signe dans tout voisinage de $+\infty$.

#### Lemme 2 {#fvr-v-a0-lem-2 .statement}

*Soient $a(x)$ et $b(x)$ deux fonctions appartenant à un même corps de Hardy $\mathfrak{K}$, $y(x)$ une fonction satisfaisant à l’identité (1) dans un intervalle $(x_0, +\infty[$ où $a$ et $b$ sont définies et continues. Si $p(u)$ est un polynôme par rapport à $u$, dont les coefficients sont des fonctions de $x$ appartenant à $\mathfrak{K}$, définies et dérivables dans $(x_0, +\infty[$, il existe un intervalle $(x_1, +\infty[$, dans lequel la fonction $p(y)$ ne change pas de signe.*

La proposition est triviale si $p(u)$ a ses coefficients identiquement nuls dans $(x_0, +\infty[$, ou si $p(u)$ est de degré 0 par rapport à $u$, puisqu’une fonction de $\mathbf{A}$ garde un signe constant dans un intervalle $(x_1, +\infty[$. Supposons que $p(u)$ soit de degré $n > 0$; le coefficient dominant $c$ de $p(u)$ est alors $\neq 0$ dans un intervalle $(\alpha, +\infty[$; on peut donc écrire $p(u) = c(u^n + c_1u^{n-1} + \cdots + c_n)$ où $c, c_1, c_2, \ldots, c_n$ sont des fonctions appartenant à $\mathbf{A}$ et dérivables dans $(\alpha, +\infty[$; il suffit donc de démontrer le lemme pour $c = 1$. Raisonnons alors par récurrence sur $n$; on a

$$
\frac{d}{dx}(p(y)) = (ay + b)(ny^{n-1} + (n-1)c_1y^{n-2} + \cdots + c_{n-1})
$$
$$
+ c'_1y^{n-1} + \cdots + c'_n = na.p(y) + q(y)
$$

où $q(u)$ est un polynôme de degré $\leq n - 1$, à coefficients dans $\mathbf{A}$. Par hypothèse, les fonctions $na(x)$ et $q(y(x))$ ne changent pas de signe dans un intervalle $(\beta, +\infty[$; le lemme est donc une conséquence du lemme 1.

#### Théorème 1 {#fvr-v-a0-thm-1 .statement}

Soient $a(x)$ et $b(x)$ deux fonctions appartenant à un même corps de Hardy $\mathbf{A}$, $y(x)$ une fonction satisfaisant à (1) dans un intervalle $(x_0, +\infty[$. Lorsque $r(u) = p(u)/q(u)$ parcourt l’ensemble des fractions rationnelles en $u$ à coefficients dans $\mathbf{A}$ telles que $q(y)$ ne soit pas identiquement nulle dans un voisinage de $+\infty$, l’ensemble $\mathbf{A}(y)$ des fonctions $r(y)$ forme un corps de Hardy.

En effet, d’après le lemme 2, il existe un intervalle $(x_1, +\infty[$ dans lequel $r(y)$ est définie, continue et ne change pas de signe, d’où résulte aussitôt que $\mathbf{A}(y)/\mathbf{R}_\infty$ est bien un corps; d’autre part, comme

$$
\frac{d}{dx}(r(y)) = r'(y)y' = r'(y)(ay + b)
$$

(où $r'(y) = (p'(y)q(y) - p(y)q'(y))/(q(y))^2$ est définie par hypothèse dans un voisinage de $+\infty$), la dérivée de toute fonction de $\mathbf{A}(y)$ appartient à $\mathbf{A}(y)$, ce qui prouve que $\mathbf{A}(y)$ satisfait aux conditions de la déf. 1 de V, p. 36.

Il est clair que $\mathbf{A}(y)/\mathbf{R}_\infty$ s’obtient par adjonction algébrique à $\mathbf{A}/\mathbf{R}_\infty$ de la classe de $y$ modulo $\mathbf{R}_\infty$. On dit encore que $\mathbf{A}(y)$ s’obtient par adjonction de $y$ à $\mathbf{A}$.

#### Corollaire 1 {#fvr-v-a0-thm-1-cor-1 .statement}

Si $y$ est une fonction de $\mathbf{A}$ non identiquement nulle dans un voisinage de $+\infty$, $\mathbf{A}(\log|y|)$ est un corps de Hardy.

En effet, $(\log|y|)' = y'/y$ est égale à une fonction de $\mathbf{A}$ dans un intervalle $(x_0, +\infty[$.

#### Corollaire 2 {#fvr-v-a0-thm-1-cor-2 .statement}

Si $y$ est une fonction quelconque de $\mathbf{A}$, $\mathbf{A}(e^y)$ est un corps de Hardy.

En effet, $(e^y)' = e^y y'$, et $y'$ est égale à une fonction de $\mathbf{A}$ dans un intervalle $(x_0, +\infty[$.

#### Corollaire 3 {#fvr-v-a0-thm-1-cor-3 .statement}

Si $\mathbf{A}$ contient les constantes réelles, et si $y$ est une fonction de $\mathbf{A}$ non identiquement nulle dans un voisinage de $+\infty$, $g(|y|^{\alpha})$ est un corps de Hardy pour tout nombre réel $\alpha$.

En effet, $\frac{d}{dx}(|y|^{\alpha}) = |y|^{\alpha} (\alpha y'/|y|)$, et $\alpha y'/|y|$ est égale à une fonction de $\mathbf{R}$ dans un intervalle $[x_0, +\infty[$.

Notons enfin que si $y$ est une primitive d’une fonction quelconque de $\mathbf{R}$, $g(y)$ est encore un corps de Hardy.

### 3. Comparaison des fonctions d’un corps de Hardy

#### Proposition 1 {#fvr-v-a0-prop-1 .statement}

Deux fonctions appartenant à un même corps de Hardy sont comparables d’ordre quelconque (V, p. 22).

En effet, si $f$ appartient à un corps de Hardy $\mathbf{R}$, pour tout entier $n > 0$, il existe un intervalle $[x_0, +\infty[$ dans lequel $f$ est $n$ fois dérivable, sa dérivée $n$-ème étant égale à une fonction de $\mathbf{R}$ dans cet intervalle. Il suffit donc de montrer que deux fonctions quelconques $f, g$ de $\mathbf{R}$ sont comparables. C’est évident si l’une d’elles est identiquement nulle dans un voisinage de $+\infty$; on peut donc se borner au cas où elles sont toutes deux strictement positives dans un voisinage de $+\infty$. Mais alors, pour tout nombre réel $t, f - tg$ est égale à une fonction de $\mathbf{R}$ dans un voisinage de $+\infty$, donc garde un signe constant dans un voisinage de $+\infty$, ce qui démontre la proposition (V, p. 8, prop. 9).

On déduit d’abord de cette proposition que, si un corps de Hardy $\mathbf{R}$ contient les constantes réelles (ce que nous supposerons toujours par la suite), et si $f$ et $g$ sont deux fonctions quelconques de $\mathbf{R}$, deux quelconques des fonctions $e^f$, $e^g$, $\log|f|$, $\log|g|$, $|f|^{\alpha}$, $|g|^{\alpha}$ ($\alpha$ réel quelconque), $\int_a f$, $\int_a g$ ($a$ réel quelconque dans un intervalle $[x_0, +\infty[$ où $f$ et $g$ sont réglées) sont comparables (lorsqu’elles sont définies); en effet, deux quelconques de ces fonctions appartiennent à un même corps de Hardy obtenu en les adjoignant successivement à $\mathbf{R}$.

De même, toute fonction $f(x)$ d’un corps de Hardy $\mathbf{R}$ est comparable à $x$, car $x$ et $f(x)$ appartiennent au corps de Hardy $\mathbf{R}(x)$ obtenu en adjoignant $x$ à $\mathbf{R}$. On en conclut donc (en particulier) que $f$ est comparable d’ordre quelconque à toute puissance $x^{\alpha}$, ainsi qu’à $\log x$ et à $e^x$.

On voit aussi que, si $f$ et $g$ appartiennent à un même corps de Hardy $\mathbf{R}$, si $g(x) > 0$ dans un intervalle $[x_0, +\infty[$, et si $g(x)$ tend vers 0 ou vers $+\infty$ lorsque $x$ tend vers $+\infty$, l’ordre de $f$ par rapport à $g$ (V, p. 9) est toujours défini.

La prop. 8 de V, p. 23, est donc applicable à toute fonction $f$ d’un corps de Hardy, et prouve que:

1° si $f$ est d’ordre $+\infty$ par rapport à $x$, $\int_a^x f(t)\,dt \sim (f(x))^2/f'(x).$.

2° si $f$ est d’ordre $\mu > -1$ par rapport à $x$, $\int_a^x f(t)\,dt \sim \frac{1}{\mu + 1}\,x f(x)$.

3° si $f$ est d’ordre $\mu < -1$ par rapport à $x$, $\int_x^{+\infty} f(t)\,dt \sim -\frac{1}{\mu + 1}\,x f(x)$.

4° si $f$ est d’ordre $-\infty$ par rapport à $x$ $\int_x^{+\infty} f(t)\,dt \sim -(f(x))^2/f'(x)$.

On a en outre la proposition suivante:

#### Proposition 2 {#fvr-v-a0-prop-2 .statement}

Soit $f$ une fonction appartenant à un corps de Hardy $\mathfrak{A}$.
1° Si $f$ est d’ordre infini par rapport à $x$, on $a$, pour tout entier $n > 0$,
$$
f^{(n)}(x) \sim \frac{(f'(x))^n}{(f(x))^{n-1}}.
$$
2° Si $f$ est d’ordre fini $\mu$ par rapport à $x$, on $a$, pour tout $n > 0$,
$$
f^{(n)}(x) \sim \mu(\mu-1)\ldots(\mu-n+1)\frac{f(x)}{x^n} \sim \frac{(\mu-1)\ldots(\mu-n+1)}{\mu^{n-1}}\frac{(f'(x))^n}{(f(x))^{n-1}}
$$
sauf si $\mu$ est entier $\geqslant 0$ et $n > \mu$.

1° Si $f$ est d’ordre infini par rapport à $x$, on a $\log |f| \gg \log x$, donc, puisque $\log|f|$ et $\log x$ sont comparables d’ordre quelconque, $f'/f \gg 1/x$. Posons $g = f'/f$; comme $g$ est égale à une fonction de $\mathfrak{A}$ dans un voisinage de $+\infty$, on déduit de $1/g \ll x$, que $g'/g^2 \ll 1$, et par suite $g'/g \ll g = f'/f$, ou encore $fg' \ll gf'$. De la relation $f' = fg$, on déduit en dérivant
$$
f'' = fg' + gf' \sim gf'
$$
ou encore $f''/f' \sim f'/f$. Le même raisonnement, appliqué à $f^{(n)}$ au lieu de $f$, montre, par récurrence sur $n$, que $f^{(n)}/f^{(n-1)} \sim f'/f$; d’où la relation (2).

2° Si $f$ est d’ordre fini $\mu$ par rapport à $x$ et si $\mu \neq 0$, on a $\log |f| \sim \mu \log x$, d’où, en dérivant, $f'(x) \sim \mu \frac{f(x)}{x}$; on en déduit que $f'$ est d’ordre $\mu - 1$ par rapport à $x$, ce qui permet d’appliquer le même raisonnement par récurrence sur $n$ tant que $\mu \neq n$, d’où la formule (3) lorsque $\mu$ n’est pas un entier $\geqslant 0$ et $< n$.

Lorsque $f$ est d’ordre entier $p \geqslant 0$ par rapport à $x$, on peut écrire $f(x) = x^p f_1(x)$, où $f_1$ est d’ordre 0 par rapport à $x$. D’après la prop. 2, on a
$$
f^{(n)} \sim p! f_1.
$$
Pour évaluer les dérivées d’ordre $n > p$, on peut donc se borner au cas où $p = 0$. Alors, on a $\log |f| \ll \log x$, d’où $f'(x)/f(x) \ll 1/x$, autrement dit $x f'(x) \ll f(x)$; si $f$ n’est pas équivalente à une constante $k \neq 0$, on $a$, en dérivant cette relation (V, p. 22, prop. 7), $x f''(x) + f'(x) \ll f'(x)$, ce qui signifie que $x f''(x) \sim -f'(x)$. Tenant compte de cette formule, on voit par récurrence sur $n$ que $f^{(n)}$ est d’ordre $\leqslant -n$ par rapport à $x$, et que
$$
f^{(n)}(x) \sim (-1)^{n+1}(n-1)! \frac{f'(x)}{x^{n-1}}.
$$
Si $f$ est équivalente à une constante $k \neq 0$, on a $f(x) = k + f_2(x)$ avec $f_2 \ll 1$, et on est ramené à étudier les dérivées de $f_2$.

### 4. Fonctions (H)

#### Proposition 3 {#fvr-v-a0-prop-3 .statement}

Si $\mathfrak{R}_0$ est un corps de Hardy, il existe un corps de Hardy $\mathfrak{R}$, contenant $\mathfrak{R}_0$ et tel que, pour toute fonction $z \in \mathfrak{R}$, non identiquement nulle dans un voisinage de $+\infty$, $e^z$ et $\log |z|$ appartiennent à $\mathfrak{R}$.

Désignons par $\mathfrak{R}$ l’ensemble des fonctions $f \in \mathcal{H}(\mathfrak{R}, \mathbf{R})$ ayant les propriétés suivantes: pour chaque fonction $f \in \mathfrak{R}$ il existe un nombre fini de corps de Hardy $\mathfrak{R}_1, \mathfrak{R}_2, \ldots, \mathfrak{R}_n$ (le nombre $n$ et les corps $\mathfrak{R}_i$ dépendant de $f$) tels que $f \in \mathfrak{R}_n$ et que, pour $0 \leq i \leq n - 1$, on ait $\mathfrak{R}_{i+1} = \mathfrak{R}_i(u_{i+1})$, où $u_{i+1}$ est égale, soit à $e^{z_i}$, soit à $\log |z_i|$, $z_i$ appartenant à $\mathfrak{R}_i$ et n’étant pas identiquement nulle au voisinage de $+\infty$. On dit que $u_1, u_2, \ldots, u_n$ forment une suite de définition du corps $\mathfrak{R}_n$ et de la fonction $f$; une même fonction $f \in \mathfrak{R}$ peut naturellement admettre plusieurs suites de définition.

D’après la déf. 1 de V, p. 36, toute fonction $f \in \mathfrak{R}$, non identiquement nulle dans un voisinage de $+\infty$, garde un signe constant et est dérivable dans un intervalle $[x_0, +\infty[$; si $f \in \mathfrak{R}_n$, $1/f$ et $f'$ sont égales à des fonctions de $\mathfrak{R}_n$, donc à des fonctions de $\mathfrak{R}$, dans un voisinage de $+\infty$. Pour voir que $\mathfrak{R}$ est un corps de Hardy, il suffit donc de prouver que si $f$ et $g$ sont deux fonctions de $\mathfrak{R}$, $f - g$ et $fg$ sont égales à des fonctions de $\mathfrak{R}$ dans un voisinage de $+\infty$. Or soit $u_1, u_2, \ldots, u_m$ une suite de définition de $f$, $v_1, v_2, \ldots, v_n$ une suite de définition de $g$. La suite $u_1, u_2, \ldots, u_m, v_1, v_2, \ldots, v_n$ obtenue par juxtaposition des suites $(u_i)$ et $(v_j)$ est encore une suite de définition d’un corps de Hardy $\mathfrak{R}_{m+n}$, et ce corps contient $f$ et $g$, donc $f - g$ et $fg$ sont égales à des fonctions de $\mathfrak{R}_{m+n}$ dans un voisinage de $+\infty$.

On dira que le corps de Hardy $\mathfrak{R}$ défini dans la démonstration de la prop. 3 est l’extension (H) du corps de Hardy $\mathfrak{R}_0$.

Si $\mathfrak{R}'$ est un autre corps de Hardy possédant les propriétés énoncées dans la prop. 3, il résulte de la construction de $\mathfrak{R}$ que $\mathfrak{R}/\mathbf{R}_\infty$ est contenu dans $\mathfrak{R}'/\mathbf{R}_\infty$. Par abus de langage, on peut donc dire que l’extension (H) d’un corps de Hardy $\mathfrak{R}_0$ est le plus petit corps de Hardy $\mathfrak{R}$ ayant les propriétés énoncées dans la prop. 3.

#### Définition 2 {#fvr-v-a0-def-2 .statement}

On appelle corps des fonctions (H) l’extension (H) du corps de Hardy $\mathbf{R}(x)$ des fonctions rationnelles à coefficients réels. Toute fonction appartenant à cette extension est dite fonction (H).

D’après cette définition, si $f$ est une fonction (H) non identiquement nulle dans un voisinage de $+\infty$, $e^f$ et $\log |f|$ sont aussi des fonctions (H). Plus généralement, si $g$ est une seconde fonction (H), $u_1, u_2, \ldots, u_n$ une suite de définition de $g$, et si $f(x)$ tend vers $+\infty$ avec $x$, on voit par récurrence sur $n$ que les fonctions composées $u_1 \circ f, u_2 \circ f, \ldots, u_n \circ f$ et $g \circ f$ sont des fonctions (H).

### 5. Exponentielles et logarithmes itérés

Nous avons déjà (V, p. 19) défini les logarithmes itérés $l_n(x)$ par les conditions $l_0(x) = x$, $l_n(x) = \log(l_{n-1}(x))$ pour $n \geq 1$. On définit de même les exponentielles itérées $e_n(x)$ par les conditions $e_0(x) = x, e_n(x) = \exp(e_{n-1}(x))$ pour $n \geq 1$. Il est immédiat, par récurrence sur $n$, que $l_n(x)$ est la fonction réciproque de $e_n(x)$, définie pour $x > e_{n-1}(0)$, et que $e_m(e_n(x)) = e_{m+n}(x),\ l_m(l_n(x)) = l_{m+n}(x)$. En vertu des relations $\log x \ll x^\mu \ll e^\gamma$ pour tout $\mu > 0$, on a, pour $n \geq 1$

(5)
$$
l_n(x) \ll (l_{n-1}(x))^\mu \quad \text{pour tout } \mu > 0
$$

(6)
$$
e_{n-1}(x^{1+\beta}) \ll e_n(x^{1+\delta}) \ll e_n((1-\gamma)x) \ll (e_n(x))^\mu \ll e_n((1+\alpha)x) \ll e_n(x^{1+\beta})
$$
pour $\mu > 0,\ \alpha > 0,\ \beta > 0,\ 0 < \gamma < 1,\ 0 < \delta < 1$, ces nombres étant par ailleurs quelconques (cf. V, p. 8, prop. 11).

Nous avons déjà vu (V, p. 19) que, pour $n \geq 1$, on a

(7)
$$
\frac{d}{dx}\left(l_n(x)\right) = \prod_{i=0}^{n-1} \frac{1}{l_i(x)}.
$$

On a de même pour $n \geq 1$

(8)
$$
\frac{d}{dx}\left(e_n(x)\right) = \prod_{i=1}^n e_i(x)
$$
d’où, en vertu de la prop. 8 de V, p. 23, pour tout $\mu > 0$

(9)
$$
\int_a^\infty e_n(t^\mu)\ dt \sim \frac{x}{\mu}\ e_n(x^\mu) \prod_{i=0}^{n-1} \frac{1}{e_i(x^\mu)}
$$

(10)
$$
\int_x^{+\infty} \frac{dt}{e_n(t^\mu)} \sim \frac{x}{\mu} \prod_{i=0}^n \frac{1}{e_i(x^\mu)}.
$$

On peut montrer que si $f$ est une fonction (H) quelconque telle que $f \gg 1$, il existe deux entiers $m$ et $n$ tels que
$$
l_m(x) \ll f(x) \ll e_n(x)
$$
(V, p. 51, exerc. 1 et 52, exerc. 5). Par contre, on peut définir des fonctions croissantes $g(x)$ (qui ne sont plus des fonctions (H)) telles que $g(x) \gg e_n(x)$ pour tout $n > 0$, ou $1 \ll g(x) \ll l_m(x)$ pour tout $m > 0$ (V, p. 53, exerc. 8, 9 et 10).

À l’aide des logarithmes itérés, nous allons montrer qu’on peut définir une échelle de comparaison (pour $x$ tendant vers $+\infty$) $\mathscr{E}$ formée de fonctions (H), qui sont $> 0$ dans un voisinage de $+\infty$ et satisfont aux conditions suivantes:
a) le produit de deux fonctions quelconques de $\mathscr{E}$ appartient à $\mathscr{E}$;
b) pour toute fonction $f \in \mathscr{E}$ et tout nombre réel $\mu$, $f^\mu \in \mathscr{E}$;
c) pour toute fonction $f \in \mathscr{E}$, $\log f$ est combinaison linéaire d’un nombre fini de fonctions de $\mathscr{E}$;
d) pour toute fonction $f \in \mathscr{E}$ autre que la constante 1, $e^f$ est équivalente à une fonction de $\mathscr{E}$.

Considérons d’abord l’ensemble $\mathscr{E}_0$ des fonctions de la forme $\prod_{m=0}^\infty (l_m(x))^{\alpha_m}$, où les $\alpha_m$ sont des nombres réels, nuls sauf pour un nombre fini d’indices $m$; il est immédiat, d’après (5) (V, p. 42), que ces fonctions forment une échelle de comparaison quisatisfait aux conditions a), b) et c). Désinissions ensuite par récurrence sur $n$ l’ensemble $\mathscr{E}_n$ (pour $n \geqslant 1$) comme formé de la constante 1 et des fonctions de la forme $\exp \left( \sum_{k=1}^p a_k f_k \right)$, où $p$ est un entier $> 0$ arbitraire, $f_k$ ($1 \leqslant k \leqslant p$) des fonctions de $\mathscr{E}_{n-1}$ telles que $f_1 \gg f_2 \gg \cdots \gg f_p \gg 1$, et les $a_k$ des nombres réels $\neq 0$; montrons par récurrence que $\mathscr{E}_n$ est une échelle de comparaison satisfaisant aux conditions a), b) et c) et contenant $\mathscr{E}_{n-1}$. En premier lieu, la relation $\mathscr{E}_{n-1} \subset \mathscr{E}_n$ est vraie pour $n = 1$, car le logarithme d’une fonction non constante de $\mathscr{E}_0$ est de la forme $\sum_{k=1}^p a_k f_k$, où les $f_k$ sont des logarithmes itérés, donc $\gg 1$; d’autre part, si $\mathscr{E}_{n-2} \subset \mathscr{E}_{n-1}$, on déduit de la définition de $\mathscr{E}_n$ que $\mathscr{E}_{n-1} \subset \mathscr{E}_n$; cette définition montre en outre que $\mathscr{E}_n$ satisfait à a), b) et c). Reste à voir que $\mathscr{E}_n$ est une échelle de comparaison : comme le quotient de deux fonctions de $\mathscr{E}_n$ appartient encore à $\mathscr{E}_n$, il suffit de prouver qu’une fonction $f$ de $\mathscr{E}_n$ autre que la constante 1, ne peut être équivalente à une constante $\neq 0$. Or on a $\log f = \sum_{k=1}^p a_k f_k \sim a_1 f_1$ par construction, et comme $f_1 \gg 1$, $\log f$ tend vers $\pm \infty$, donc $f$ tend vers 0 ou vers $+\infty$ lorsque $x$ tend vers $+\infty$.

Cela étant, si $\mathscr{E}$ est la réunion des $\mathscr{E}_n$ pour $n \geqslant 0$, $\mathscr{E}$ est une échelle de comparaison, car deux fonctions de $\mathscr{E}$ appartiennent à une même échelle $\mathscr{E}_n$; pour la même raison, $\mathscr{E}$ satisfait à a), et il est clair qu’elle satisfait aussi à b) et c). Enfin, si $f \in \mathscr{E}$, il existe $n$ tel que $f \in \mathscr{E}_n$; si $f$ n’est pas la constante 1, $f(x)$ tend vers 0 ou vers $+\infty$ lorsque $x$ tend vers $+\infty$; dans le premier cas, $e^f \sim 1$, et dans le second, $e^f$ appartient à $\mathscr{E}_{n+1}$ par définition, donc à $\mathscr{E}$.

#### Remarque {#fvr-v-a0-n5-rem-1 .statement}

Malgré l’utilité pratique de l’échelle $\mathscr{E}$ que nous venons de définir, il est facile de donner des exemples de fonctions (H) qui n’ont pas de partie principale par rapport à $\mathscr{E}$. En effet, si $f$ est une fonction (H) telle que $f \sim ag$, où $a$ est une constante $> 0$ et $g \in \mathscr{E}$, $\log f - \log g - \log a$ tend vers 0 avec $1/x$, donc $\log f$ admet, relativement à $\mathscr{E}$, un développement asymptotique dont le reste tend vers 0, en vertu de la propriété c). Or, si on considère par exemple la fonction (H)
$$
f(x) = e_2 \left( x + \frac{1}{x} \right),
$$
on a $\log f(x) = \exp \left( x + \frac{1}{x} \right)$, donc les développements asymptotiques de $\log f$ par rapport à $\mathscr{E}$ sont de la forme
$$
\log f(x) = e^x + \frac{e^x}{x} + \frac{1}{2!} \frac{e^x}{x^2} + \cdots + \frac{1}{n!} \frac{e^x}{x^n} + o \left( \frac{e^x}{x^n} \right) \quad (n \text{ entier } > 0).
$$
Il est clair que le reste de ce développement est équivalent à $\frac{1}{(n+1)!} \frac{e^x}{x^{n+1}}$, donc ne tend pas vers 0. Par suite, $f$ n’a pas de partie principale par rapport à $\mathscr{E}$.

### 6. Fonction réciproque d’une fonction (H)

Si $f$ est une fonction (H), $f$ est monotone et continue dans un intervalle $(x_0, +\infty)$, donc la fonction réciproque $\varphi$ de la restriction de $f$ à cet intervalle est monotone et continue au voisinage du point $a = \lim_{x \to +\infty} f(x)$; mais, si $a$ est égal à $+\infty$ (resp. $-\infty$, fini), on peut montrer que $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi\left(a + \frac{1}{y}\right)$ ou $\varphi\left(a - \frac{1}{y}\right)$) n’est pas en général égale à une fonction (H) au voisinage de $+\infty$. Toutefois, nous allons voir que, dans certains cas importants, on peut obtenir une fonction (H) équivalente à $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi\left(a + \frac{1}{y}\right)$, $\varphi\left(a - \frac{1}{y}\right)$) et même parfois un développement asymptotique de cette fonction par rapport à l’échelle $\mathscr{E}$ définie dans V, p. 43.

Nous utiliserons la proposition suivante:

#### Proposition 4 {#fvr-v-a0-prop-4 .statement}

Soient $p$ et $q$ deux fonctions (H) strictement positives dans un intervalle $(x_0, +\infty)$.

1° Si $q \ll p/p'$, on a $p(x + q(x)) \sim p(x)$.

2° Si on a à la fois $q \ll p/p'$ et $q(x) \ll x$, on a $p(x - q(x)) \sim p(x)$.

Les deux parties de la proposition sont évidentes si $p \sim k$ (constante $\neq 0$); on peut donc supposer $p(x) \ll 1$ (sinon on raisonnait sur $1/p$). On en déduit $p'(x) \ll 1$.

1° On peut écrire $p(x + q(x)) = p(x) + q(x)p'(x + \theta q(x))$ avec $0 \leq \theta \leq 1$ (I, p. 22, corollaire). Comme $|p'(x)|$ tend vers 0 lorsque $x$ tend vers $+\infty$, et est égale à une fonction (H) dans un voisinage de $+\infty$, elle est décroissante dans un intervalle $(x_1, +\infty)$, donc, pour $x \geq x_1$, on a $|p'(x + \theta q(x))| \leq |p'(x)|$; comme $qp' \ll p$, on a bien $p(x + q(x)) \sim p(x)$.

2° La condition $q(x) \ll x$ assure que $x - q(x)$ tend vers $+\infty$ avec $x$. On a encore $p(x - q(x)) = p(x) - q(x)p'(x - \theta p(x))$ avec $0 \leq \theta \leq 1$. Le même raisonnement que dans la première partie de la démonstration montre que, pour $x$ assez grand, on a $|p'(x - \theta q(x))| \leq |p'(x - q(x))|$. Tout revient à montrer que $q(x) \frac{p'(x - q(x))}{p(x - q(x))}$ tend vers 0 lorsque $x$ tend vers $+\infty$. La proposition est vraie si $p'/p \gg 1$, car alors $|p'/p|$ est une fonction (H) croissante pour $x$ assez grand, donc $q(x) \frac{|p'(x - q(x))|}{|p(x - q(x))|} \leq q(x) \frac{|p'(x)|}{|p(x)|}$, et on a $qp' \ll p$ par hypothèse. Elle est vraie aussi si $p'/p \sim k$ ($k$ constante $\neq 0$), car alors

$$
\frac{p'(x - q(x))}{p(x - q(x))} \sim \frac{p'(x)}{p(x)}
$$

puisque $x - q(x)$ tend vers $+\infty$. Reste uniquement à examiner le cas où $p'/p \ll 1$. Supposons d’abord que $p(x)$ soit d’ordre fini par rapport à $x$, donc (V, p. 22, prop. 7) que $p'(x)/p(x) \ll 1/x$. On a alors $\frac{p'(x-q(x))}{p(x-q(x))} = \frac{1}{x-q(x)} O_1(1)$, donc $q(x) \frac{p'(x-q(x))}{p(x-q(x))} = \frac{q(x)}{x} \left( 1 - \frac{q(x)}{x} \right)^{-1} O_1(1) = \frac{q(x)}{x} O_2(1)$ et on voit que dans ce cas la proposition est vraie sous la seule hypothèse $q(x) \ll x$. Considérons enfin le cas où $1/x \ll p'(x)/p(x) \ll 1$; la fonction $r = p'/p$ est alors d’ordre fini par rapport à $x$; comme d’après la remarque précédente, la prop. 4 de V, p. 44, est applicable à une telle fonction, on a $p'(x-q(x))/p(x-q(x)) \sim p'(x)/p(x)$, et l’hypothèse $qp' \ll p$ permet alors d’achever la démonstration.

#### Remarque {#fvr-v-a0-n6-rem-3 .statement}

Les conditions imposées à $q(x)$ ne peuvent être améliorées, comme le montrent les exemples suivants:

a) $p(x) = e^x, \quad q(x) = 1 = \frac{p(x)}{p'(x)}, \quad p(x+q(x)) = e.p(x)$

b) $p(x) = \log x, \quad q(x) = x - \log x \ll \frac{p(x)}{p'(x)} = x \log x,$
   $p(x-q(x)) = \log \log x \ll p(x).$

Nous allons d’abord étudier les fonctions réciproques d’un type particulier de fonctions (H):

#### Proposition 5 {#fvr-v-a0-prop-5 .statement}

Soit $g$ une fonction (H) non équivalente à une constante $\neq 0$ et telle que $g(x) \ll x$, et soit $u(x)$ la fonction réciproque de $x - g(x)$, définie dans un voisinage de $+\infty$. Soit $(u_n)$ la suite de fonctions définie, par récurrence sur $n$, par les conditions $u_0(x) = x,$ $u_n(x) = x + g(u_{n-1}(x))$ pour $n \geqslant 1$; on a $u_n \gg 1$, et
$$
u(x) - u_n(x) \sim g(x)(g'(x))^n.
$$
Posons $y = u(x), \ y_n = u_n(x)$; on a donc $x = y - g(y), \ y_0 = x$ et $y_n = x + g(y_{n+1})$. On en tire d’abord $x/y = 1 - \frac{g(y)}{y}$; comme $y$ tend vers $+\infty$ avec $x$, l’hypothèse $g(x) \ll x$ montre que $y = u(x) \sim x = y_0$; en outre,
$$
y - x = g(y) = g(x) + (y - x)g'(z)
$$
où $z$ appartient à l’intervalle d’extrémités $x, y$; quand $x$ tend vers $+\infty$, il en est donc de même de $z$, et comme $g(x) \ll x, \ g' \ll 1$, donc $g'(z)$ tend vers $0$, et on a par suite
$$
y - x = g(x) + o(y - x)
$$
d’où
$$
u(x) - x \sim g(x).
$$

Montrons en second lieu, par récurrence sur $n$, que lorsque $x$ tend vers $+\infty$, on a $u_n \gg 1$, et
$$
u(x) - u_n(x) \ll u(x) - u_{n-1}(x).
$$
En effet, $y - y_n = g(y) - g(y_{n-1}) = (y - y_{n-1})g'(z_{n-1})$, où $z_{n-1}$ appartient à l’intervalle d’extrémités $y$ et $y_{n-1}$; d’après l’hypothèse de récurrence, $z_{n-1}$ tend vers $+\infty$ avec $x$, donc $g'(z_{n-1})$ tend vers 0, ce qui démontre (13). On déduit de cette relation et de (12) que $u(x) - u_n(x) \ll u(x) - x \sim g(x) \ll x \sim u(x)$, d’où $u_n(x) \sim u(x)$ et par suite $u_n \gg 1$. Enfin, la relation $u(x) - u_n(x) \ll u(x) - x$ s’écrit aussi $(u(x) - x) - (u_n(x) - x) \ll u(x) - x$, d’où
$$
u_n(x) - x \sim u(x) - x \sim g(x).
$$
Pour démontrer (11), remarquons d’abord que, si $t(x)$ est une fonction telle que $t(x) - x \sim g(x)$, on a $g'(t(x)) \sim g'(x)$. En effet, quel que soit $\varepsilon > 0$, pour $x$ assez grand, $g'$ est monotone, donc $g'(t(x))$ est comprise entre $g'(x + (1 + \varepsilon)g(x))$ et $g'(x + (1 - \varepsilon)g(x))$. La prop. 4 de V, p. 44, montre donc que $g'(t(x)) \sim g'(x)$, pourvu qu’on établisse la relation $g \ll g'/g''$. Or, si $g$ est d’ordre infini par rapport à $x$, on a (V, p. 40, prop. 2) $g''/g' \sim g'/g$, et comme $g' \ll 1$, $g \ll g/g' \sim g'/g''$; si $g$ est d’ordre fini $\mu$ par rapport à $x$, on a nécessairement $\mu \leqslant 1$; si $\mu < 1$, comme $g$ n’est pas équivalente à une constante $\neq 0$, les formules (3) et (4) (V, p. 40) montrent que $g''/g' \sim k/x$ ($k$ constante $\neq 0$), d’où encore $g \ll g'/g''$; enfin si $\mu = 1$, $g'$ est d’ordre 0 par rapport à $x$, donc $g''/g' \ll 1/x$, et par suite on a encore $g \ll g'/g''$.

Cela étant, comme $z_{n-1}$ est compris entre $y$ et $y_{n-1}$, il résulte de (14) que $z_{n-1} - x \sim g(x)$, d’où $g'(z_{n-1}) \sim g'(x)$ d’après ce qui précède; on a donc
$$
y - y_n \sim (y - y_{n-1})g'(x),
$$
d’où (11) par récurrence sur $n$.

#### Remarque 1 {#fvr-v-a0-n6-rem-1 .statement}

Si $g$ est d’ordre $< 1$ par rapport à $x$, la fonction $u(x) - u_n(x)$ tend vers 0 avec $1/x$ dès que $n$ est assez grand. En effet, dans le cas contraire, on aurait $gg^n \gg 1$ pour tout $n$, donc $g$ serait d’ordre infini par rapport à $1/g'$; autrement dit, on aurait $\log |g| \gg \log |g'|$, d’où en dérivant $g'/g \gg g''/g'$. Mais, si $g$ est d’ordre $\mu < 1$ par rapport à $x$, on a $g'/g \sim g''/g'$ lorsque $\mu = -\infty$, $\frac{g'}{g} \sim \frac{\mu}{\mu - 1} \frac{g''}{g'}$ lorsque $\mu \neq 0$ et enfin $g'/g \ll g''/g'$ lorsque $\mu = 0$ (V, p. 40, no 3).

Par contre, si $g$ est d’ordre 1 par rapport à $x$, on peut avoir $gg^n \gg 1$ pour tout entier $n > 0$, comme le montre l’exemple $g(x) = x/\log x$.

#### Remarque 2 {#fvr-v-a0-n6-rem-2 .statement}

Lorsque $g(x)$ est une fonction (H) équivalente à une constante $k \neq 0$, on a $g(x) = k + g_1(x)$, avec $g_1 \ll 1$; la fonction $u_1(x) = u(x) - k$ est fonction réciproque de $x - g_1(x + k)$, et on est ramené au cas traité dans la prop. 5 de V, p. 45.

Pour avoir un développement asymptotique de la fonction $u$, il suffit donc d’avoir un tel développement pour la fonction $u_n$: si $g$ admet un développement asymptotique par rapport à l’échelle considérée, on est ainsi ramené (en vertu de la définition des fonctions (H)) aux problèmes examinés dans V, p. 14 à 17.

Au cas traité dans la prop. 5 de V, p. 45, se ramène le cas plus général suivant: la fonction $y = u(x)$ est supposée satisfaire à la relation

$$
\varphi(x) = \psi(y) - g(y)
$$

où $\varphi$ est une fonction (H), $\psi$ une fonction (H) telle que $\psi \gg 1$ et que la fonction réciproque $\theta$ de $\psi$ soit aussi une fonction (H), et $g$ une fonction (H) telle que $g \ll \psi$. Soit alors $v(x)$ la fonction réciproque de $x - g(\theta(x))$; on a $u = \theta \circ v \circ \varphi$, et $g(\theta(x)) \ll x$; si on connaît un développement asymptotique de $v$ grâce à la prop. 5 de V, p. 45, on en déduira un développement asymptotique de $u$ par de V, p. 14 à 17.

**Exemples. — 1)** Cherchons un développement asymptotique de la fonction réciproque $v(x)$ de $x^5 + x$ (pour $x$ tendant vers $+\infty$); en posant $x^5 = t$, on est ramené à chercher un développement de la fonction réciproque $u(t)$ de $t + t^{1/5}$ (pour $t$ tendant vers $+\infty$), c’est-à-dire à appliquer la prop. 5 de V, p. 45, au cas où $g(t) = -t^{1/5}$. Calculons par exemple $u_2(t)$; on a

$$
u_2(t) = t - (t - t^{1/5})^{1/5} = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{2}{25} t^{-7/5} + o_1(t^{-7/5}).
$$

D’autre part, d’après (11) (V, p. 45)

$$
u(t) - u_2(t) \sim -\frac{1}{25} t^{-7/5}
$$

d’où

$$
u(t) = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{1}{25} t^{-7/5} + o_2(t^{-7/5})
$$

et on en déduit le développement cherché

$$
v(x) = (u(x))^{1/5} = x^{1/5} - \frac{1}{5} x^{-3/5} - \frac{1}{25} x^{-7/5} + o_3(x^{-7/5}).
$$

2) Cherchons un développement asymptotique de la fonction réciproque $v(x)$ de la fonction $x/\log x$; de l’identité $x = y/\log y$, où $y = v(x)$, on tire $\log x = \log y - \log \log y$; posant $z = \log y$, $t = \log x$, on a $t = z - \log z$, et on est donc ramené à développer la fonction réciproque $u(t)$ de $t - \log t$; on a par exemple

$$
u_2(t) = t + \log (t + \log t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + o_1\left(\frac{\log t}{t^2}\right)
$$

et d’autre part, d’après (11) (V, p. 45)

$$
u(t) \sim u_2(t) \sim \frac{\log t}{t^2}
$$

d’où

$$
u(t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + \frac{\log t}{t^2} + o_2\left(\frac{\log t}{t^2}\right)
$$

et en revenant au problème initial, on obtient le développement asymptotique

$$
v(x) = x \log x + x \log \log x + x \frac{\log \log x}{\log x} + o\left(x \frac{\log \log x}{\log x}\right).
$$

#### Remarque {#fvr-v-a0-n6-rem-4 .statement}

On notera que deux fonctions (H) équivalentes peuvent avoir des fonctions réciproques non équivalentes, comme le montre l’exemple des deux fonctions $\log x$ et $1 + \log x$.

Exercices

## EXERCICES {#fvr-v-a0-exercises}

I) Soit $\mathfrak{R}$ un corps de Hardy tel que, pour toute fonction $f \in \mathfrak{R}$ non identiquement nulle au voisinage de $+\infty$, il existe $\lambda > 0$ tel que
$$
\frac{1}{e_m(x^\lambda)} \ll f(x) \ll e_m(x^\lambda)
$$
(m entier indépendant de $f$).
a) Soient $u_1, u_2, \ldots, u_p$ fonctions de la forme $u_k = \log|z_k|$, où $z_k \in \mathbf{R}$ n’est pas nulle dans un voisinage de $+\infty$. Montrer que pour toute fonction $g$ (non nulle dans un voisinage de $+\infty$) du corps de Hardy $\mathfrak{R}(u_1, \ldots, u_p)$ obtenu par adjonction à $\mathfrak{R}$ des fonctions $u_k$ ($1 \leq k \leq p$), il existe $\mu > 0$ tel que
$$
\frac{1}{e_m(x^\mu)} \ll g(x) \ll e_m(x^\mu)
$$
(se ramener au cas où $g$ est un polynôme par rapport aux $u_k$, à coefficients dans $\mathbf{R}$, et raisonner par récurrence sur $p$, puis, pour $p = 1$, raisonner par récurrence sur le degré du polynôme $g$ en procédant comme dans le lemme 2 de V, p. 37).
b) Soient $u_k$ ($1 \leq k \leq p$) $p$ fonctions de la forme $u_k = \exp(z_k)$ où $z_k \in \mathbf{R}$. Montrer que pour toute fonction g du corps de Hardy $\mathbb{H}(u_1, \ldots, u_p)$, non identiquement nulle au voisinage de $+\infty$, il existe un nombre $\mu > 0$ tel que
$$
\frac{1}{e_{m+1}(x^\mu)} \ll g(x) \ll e_{m+1}(x^\mu)
$$
(méthode analogue).

c) En déduire que si f est une fonction (H) admettant une suite de définition de n termes, et non identiquement nulle dans un voisinage de $+\infty$, il existe un nombre $\lambda > 0$ tel que
$$
\frac{1}{e_n(x^\lambda)} \ll f(x) \ll e_n(x^\lambda).
$$

2) a) Montrer que toute fonction (H) possédant une suite de définition d’un seul terme est équivalente à une fonction de l’une des formes $x^p (\log x)^q$, ou $x^{p e^{g(x)}}$, où $p$ et $q$ sont des entiers rationnels, et $g$ un polynôme en $x$ (méthode de l’exerc.

See the [exercises for Appendix 0](exercises/a0/).
