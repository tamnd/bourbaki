---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 1
section_title: Génération d’une structure uniforme par une famille d’écarts. Espaces uniformisables
lang: fr
source: top-v-x-fr
pdf_pages: 0121-0131, 0204-0210
extraction: ocr
subsections:
    - "no": 1
      title: Écarts
      page: 0
      pdf_page: 121
    - "no": 2
      title: Définition d’une structure uniforme par une famille d’écarts
      page: 2
      pdf_page: 122
    - "no": 3
      title: Propriétés des structures uniformes définies par des familles d’écarts
      page: 4
      pdf_page: 124
    - "no": 4
      title: Construction d’une famille d’écarts définissant une structure uniforme
      page: 5
      pdf_page: 125
    - "no": 5
      title: Espaces uniformisables
      page: 7
      pdf_page: 127
    - "no": 6
      title: Compactifié de Stone-Čech
      page: 9
      pdf_page: 129
    - "no": 7
      title: Fonctions semi-continues sur un espace uniformisable
      page: 10
      pdf_page: 130
statements: 26
exercises: 25
content_sha256: 81bdb31fac21d408e69d36d14a256ed55ef672bdffb6df7d5192894226ae729f
---

## § 1. GÉNÉRATION D’UNE STRUCTURE UNIFORME PAR UNE FAMILLE D’ÉCARTS. ESPACES UNIFORMISABLES

### 1. Écarts

#### Définition 1 {#top-ix-s1-def-1 .statement}

Étant donné un ensemble $X$, on appelle écart sur $X$ toute application $f$ de $X \times X$ dans l’intervalle $[0, +\infty)$ de la droite achevée $\overline{\mathbf{R}}$, satisfaisant aux conditions suivantes :

(EC_I) Quel que soit $x \in X$, $f(x, x) = 0$.
(EC_{II}) Quels que soient $x \in X, y \in X$, $f(x, y) = f(y, x)$ (symétrie).
(EC_{III}) Quels que soient $x \in X, y \in X, z \in X$,
$$
f(x, y) \leq f(x, z) + f(z, y)
$$
(inégalité du triangle).

#### Exemple 1 {#top-ix-s1-n1-exa-1 .statement}

Sur l’espace numérique $\mathbf{R}^n$, la distance euclidienne (VI, p. 7) est un écart.

#### Exemple 2 {#top-ix-s1-n1-exa-2 .statement}

Étant donné un ensemble quelconque $X$, la fonction $f$ définie sur $X \times X$ par les conditions : $f(x, x) = 0$ pour tout $x \in X$, $f(x, y) = +\infty$ si $x \neq y$, est un écart sur $X$.

#### Exemple 3 {#top-ix-s1-n1-exa-3 .statement}

Étant donnée une fonction numérique finie $g$ définie dans un ensemble quelconque $X$, la fonction $f$ définie dans $X \times X$ par $f(x, y) = |g(x) - g(y)|$ est un écart sur $X$.

#### Exemple 4 {#top-ix-s1-n1-exa-4 .statement}

Soit $X$ l’ensemble des applications continues de l’intervalle $[0, 1]$ de $\mathbf{R}$ dans $\mathbf{R}$. Si, pour tout couple d’éléments $x, y$ de $X$, on pose $f(x, y) = \int_0^1 |x(t) - y(t)| \, dt$, $f$ est un écart sur $X$.*

#### Remarque 1 {#top-ix-s1-n1-rem-1 .statement}

L’exemple 2 ci-dessus montre qu’un écart peut prendre la valeur $+\infty$ pour certains couples d’éléments de $X$.

#### Remarque 2 {#top-ix-s1-n1-rem-2 .statement}

Si $f$ est un écart sur $X$, on peut en général avoir $f(x, y) = 0$ pour des couples $(x, y)$ tels que $x \neq y$; c’est ce que montre l’exemple 3 ci-dessus (cf. IX, p. 1).

De l’inégalité du triangle, on déduit que, si $f(x, z)$ et $f(y, z)$ sont finis, il en est de même de $f(x, y)$; en outre, dans ce cas, on a

$$
f(x, z) \leq f(y, z) + f(x, y) \quad \text{et} \quad f(y, z) \leq f(x, z) + f(x, y),
$$

et par suite

(1)

$$
|f(x, z) - f(y, z)| \leq f(x, y).
$$

Si $f$ est un écart sur $X$, il en est de même de $\lambda f$, quel que soit le nombre fini $\lambda > 1$. Si $(f_i)_{i \in I}$ est une famille quelconque d’écarts sur $X$, la somme $\sum_{i \in I} f_i(x, y)$ est définie pour tout couple $(x, y) \in X \times X$; si on désigne sa valeur par $f(x, y)$, $f$ est un écart sur $X$. De même, l’enveloppe supérieure $g$ de la famille $(f_i)$ (IV, p. 21) est un écart sur $X$, car des relations $f_i(x, y) \leq f_i(x, z) + f_i(z, y)$, on déduit

$$
\sup_{i \in I} f_i(x, y) \leq \sup_{i \in I} (f_i(x, z) + f_i(z, y)) \leq \sup_{i \in I} f_i(x, z) + \sup_{i \in I} f_i(z, y)
$$

(IV, p. 25, formule (17)).

### 2. Définition d’une structure uniforme par une famille d’écarts

Dans l’espace numérique $\mathbf{R}^n$, on a vu (VI, p. 9) que si, pour tout nombre $a > 0$, on désigne par $U_a$ l’ensemble des couples $(x, y)$ de points de $\mathbf{R}^n$ dont la distance euclidienne est $\leq a$, les $U_a$ forment un système fondamental d’entourages de la structure uniforme de $\mathbf{R}^n$ lorsque $a$ parcourt l’ensemble des nombres $> 0$.

Plus généralement, soit $f$ un écart sur un ensemble $X$; pour tout $a > 0$, posons $U_a = f^{-1}([0, a])$; montrons que, lorsque $a$ parcourt l’ensemble des nombres $> 0$, les $U_a$ forment un système fondamental d’entourages d’une structure uniforme sur $X$. En effet, l’axiome $(U'_I)$ (II, p. 2) est vérifié en vertu de $(EC_I)$ (IX, p. 1); si $a \leq b$, on a $U_a \subset U_b$, donc les $U_a$ forment une base de filtre; d’après $(EC_{II})$, on a $U_a^{-1} = U_a$, donc $(U'_{II})$ est vérifié; enfin, d’après $(EC_{III})$, on a $U_a^2 \subset U_{2a}$, donc $(U'_{III})$ est vérifié. On peut par suite poser la définition suivante:

#### Définition 2 {#top-ix-s1-def-2 .statement}

Étant donné un écart $f$ sur un ensemble $X$, on appelle structure uniforme définie par $f$ la structure uniforme sur $X$ ayant pour système fondamental d’entourages la famille des ensembles $f^{-1}([0, a])$, où $a$ parcourt l’ensemble des nombres $> 0$.

On dit que deux écarts sur $X$ sont équivalents s’ils définissent la même structure uniforme.

#### Remarque 1 {#top-ix-s1-n2-rem-1 .statement}

Pour toute suite $(a_n)$ de nombres $> 0$ tendant vers $0$, les $U_{a_n}$ forment un système fondamental d’entourages de la structure uniforme définie par $f$.

#### Remarque 2 {#top-ix-s1-n2-rem-2 .statement}

La définition d’une structure uniforme par un écart $f$ revient à prendre comme système fondamental d’entourages de cette structure, l’image réciproque par $f$ du filtre des voisinages de 0 dans le sous-espaces $[0, +\infty)$ de $\overline{\mathbf{R}}$. On notera que ce procédé est tout à fait analogue à celui qui nous a permis de définir les structures uniformes d’un groupe topologique (III, p. 19).

Soient $f$ et $g$ deux écarts sur $X$; d’après la déf. 2, pour que la structure uniforme définie par $f$ soit moins fine que la structure uniforme définie par $g$, il faut et il suffit que, pour tout $a > 0$, il existe $b > 0$ tel que la relation $g(x, y) \leq b$ entraîne $f(x, y) \leq a$. Pour que $f$ et $g$ soient deux écarts équivalents, il faut et il suffit que, pour tout $a > 0$, il existe $b > 0$ tel que $g(x, y) \leq b$ entraîne $f(x, y) \leq a$, et que $f(x, y) \leq b$ entraîne $g(x, y) \leq a$.

En particulier, s’il existe une constante $k > 0$ telle que $f \leq kg$, la structure uniforme définie par $f$ est moins fine que celle définie par $g$.

Soit $\varphi$ une application de l’intervalle $[0, +\infty)$ dans lui-même, satisfaisant aux conditions suivantes : $1^\circ \varphi(0) = 0$, et $\varphi$ est continue au point 0 ; $2^\circ \varphi$ est croissante dans $[0, +\infty)$ et strictement croissante dans un voisinage de 0 ; $3^\circ$ quels que soient $u \geq 0$ et $v \geq 0$, $\varphi(u + v) \leq \varphi(u) + \varphi(v)$. D’après les déf. 1 (IX, p. 1) et 2 (IX, p. 1), pour tout écart $f$ sur un ensemble $X$, la fonction composée $g = \varphi \circ f$ est un écart équivalent à $f$.

Le lecteur vérifiera aisément qu’on peut par exemple prendre pour $\varphi$ l’une des fonctions suivantes :

$$
\sqrt{u}, \quad \log(1 + u), \quad \frac{u}{1 + u}, \quad \inf(u, 1).
$$

Les deux derniers exemples prouvent qu’il existe toujours des écarts bornés équivalents à un écart quelconque donné (fini ou non).

#### Définition 3 {#top-ix-s1-def-3 .statement}

Étant donnée une famille $(f_i)_{i \in I}$ d’écarts sur un ensemble $X$, on appelle structure uniforme définie par la famille $(f_i)$ sur l’ensemble $X$, la borne supérieure de l’ensemble des structures uniformes définies sur $X$ par chacun des écarts $f_i$.

On dit que deux familles d’écarts sur $X$ sont équivalentes si elles définissent la même structure uniforme sur $X$.

D’après la définition de la borne supérieure d’un ensemble de structures uniformes (II, p. 10), le filtre d’entourages de la structure uniforme $U$ définie sur $X$ par une famille d’écarts $(f_i)_{i \in I}$ est le filtre engendré (I, p. 37) par la famille des ensembles $f_i^{-1}([0, a])$, où $i$ parcourt $I$ et $a$ l’ensemble des nombres $> 0$. En d’autres termes, on obtient un système fondamental d’entourages de $U$, en procédant de la manière suivante : on prend arbitrairement un nombre fini d’indices $i_1, i_2, \ldots, i_n$ et, pour chacun des $i_k$, un nombre $a_k > 0$, puis on considère l’ensemble des couples $(x, y) \in X \times X$ tels que $f_{i_k}(x, y) \leq a_k$ pour $1 \leq k \leq n$; ces ensembles (pour tous les choix possibles de $n$, des $i_k$ et des $a_k$) forment un système fondamental d’entourages de $U$. On peut d’ailleurs se borner au cas où tous les $a_k$ sont égaux à un même nombre $a > 0$, l’entourage formé des $(x, y)$ tels que

$$
\sup_{1 \leq k \leq n} (f_{i_k}(x, y)) \leq \inf_{1 \leq k \leq n} a_k
$$

étant évidemment contenu dans le précédent.

Pour toute partie finie $H$ de $I$, soit $g_H$ l’enveloppe supérieure de la famille $(f_i)_{i \in H}$; lorsque $H$ parcourt l’ensemble des parties finies de $I$ et $a$ l’ensemble des nombres $> 0$, on voit que les ensembles $g_H^{-1}((0, a])$ forment un *système fondamental d’entourages* de la structure $\mathcal{U}$. Or, les $g_H$ sont des *écarts* sur $X$ (IX, p. 2) et l’enveloppe supérieure d’un nombre fini de fonctions de la famille $(g_H)$ appartient encore par définition à cette famille; on exprimera cette propriété en disant que la famille d’écarts $(g_H)$ est *saturée*. La famille d’écarts $(g_H)$ est donc *équivalente* à la famille $(f_i)$; on dit que c’est la famille d’écarts obtenue en *saturant* $(f_i)$; ce qui précède prouve qu’on peut toujours se borner à considérer les structures uniformes définies par des familles d’écarts *saturées*.

Dans le cas particulier où $I$ est un ensemble *fini*, ce raisonnement montre que la structure uniforme définie par la famille d’écarts $(f_i)_{i \in I}$ est aussi définie par le *seul écart* $g = \sup_{i \in I} f_i$.

Soient $\mathcal{U}$, $\mathcal{U}'$ deux structures uniformes sur $X$, définies respectivement par deux familles d’écarts *saturées* $(f_i)_{i \in I}$, $(g_K)_{K \in K}$; pour que $\mathcal{U}$ soit *moins fine* que $\mathcal{U}'$, il faut et il suffit que, pour tout indice $i \in I$ et tout nombre $a > 0$, il existe un indice $k \in K$ et un nombre $b > 0$ tels que la relation $g_K(x, y) \leq b$ entraîne $f_i(x, y) \leq a$.

*Exemple de structure uniforme définie par une famille d’écarts.* Soit $(f_i)_{i \in I}$ une famille quelconque de *fonctions numériques* (finies) définies dans un ensemble $X$. Soit $\mathcal{U}$ la structure uniforme la moins fine sur $X$ rendant uniformément continues les $f_i$ (II, p. 8); il résulte de la définition des entourages de $\mathcal{U}$ (II, p. 8), que $\mathcal{U}$ est identique à la structure uniforme définie sur $X$ par les écarts
$$
g_i(x, y) = |f_i(x) - f_i(y)|.
$$

### 3. Propriétés des structures uniformes définies par des familles d’écarts

Soit $\mathcal{U}$ une structure uniforme définie sur un ensemble $X$ par une famille d’écarts finis $(f_i)$; si on munit $X \times X$ de la structure uniforme produit de $\mathcal{U}$ par elle-même, chacune des fonctions numériques $f_i$ est *uniformément continue* dans $X \times X$; on a en effet, d’après (1)
$$
|f_i(x, y) - f_i(x', y')| \leq f_i(x, x') + f_i(y, y')
$$
donc les relations $f_i(x, x') \leq \varepsilon/2, f_i(y, y') \leq \varepsilon/2$ entraînent
$$
|f_i(x, y) - f_i(x', y')| \leq \varepsilon.
$$
Pour que $\mathcal{U}$ soit *séparée*, il faut et il suffit, d’après la définition des entourages de $\mathcal{U}$, que pour tout couple de points *distincts* $x, y$ de $X$, il existe un indice $i$ tel que $f_i(x, y) \neq 0$.

En particulier, si $\mathcal{U}$ est définie par *un seul écart* $f$, pour que $\mathcal{U}$ soit séparée, il faut et il suffit que la relation $f(x, y) = 0$ entraîne $x = y$ (cf. IX, p. 11).

Lorsque $\mathcal{U}$ n’est pas séparée, l’intersection de tous les entourages de $\mathcal{U}$ est la partie de $X \times X$ formée des couples $(x, y)$ tels que $f_i(x, y) = 0$ pour tout $i$; cette partie est le graphe d’une relation d’équivalence R sur X, et la structure uniforme séparée associée à $\mathcal{U}$ est définie sur $X/R$ (cf. II, p. 25). On voit alors aisément que les fonctions $f_i$ sont compatibles (en $x$ et en $y$) avec la relation R (E, II, p. 44) et que les fonctions $\tilde{f}_i$ obtenues par passage au quotient (pour $x$ et $y$) à partir des $f_i$, sont des écarts sur $X/R$ définissant la structure uniforme séparée associée à $\mathcal{U}$ (cf. IX, p. 11).

Si Y est une partie non vide de X, la restriction à $Y \times Y$ d’un écart sur X est évidemment un écart sur Y ; il est clair que la structure uniforme induite par $\mathcal{U}$ sur Y est définie par la famille des restrictions à $Y \times Y$ des écarts $f_i$.

Étudions maintenant le complété de l’espace uniforme X, lorsque $\mathcal{U}$ est séparée.

#### Proposition 1 {#top-ix-s1-prop-1 .statement}

*Soit X un espace uniforme séparé, dont la structure uniforme $\mathcal{U}$ est définie par une famille d’écarts finis ($f_i$); soit $\hat{X}$ le complété de X. Les fonctions $f_i$ se prolongent par continuité à $\hat{X} \times \hat{X}$; les fonctions prolongées $\tilde{f}_i$ sont des écarts finis sur $\hat{X}$, et la structure uniforme de $\hat{X}$ est identique à la structure uniforme définie par la famille ($\tilde{f}_i$).*

Tout d’abord, les $f_i$ peuvent être prolongées par continuité à $\hat{X} \times \hat{X}$, puisqu’elles sont uniformément continues dans $X \times X$, et les fonctions prolongées $\tilde{f}_i$ sont uniformément continues dans $\hat{X} \times \hat{X}$ (II, p. 20, th. 2); en outre, ce sont des écarts sur $\hat{X}$, en vertu du principe de prolongement des inégalités (IV, p. 18, th. 1). Désignons par $\mathcal{U}_1$ la structure uniforme sur $\hat{X}$ obtenue par complétion, par $\mathcal{U}_2$ la structure uniforme définie par la famille d’écarts ($\tilde{f}_i$). La structure $\mathcal{U}_2$ est *moins fine* que $\mathcal{U}_1$; en effet chacune des $\tilde{f}_i$ est uniformément continue dans $\hat{X} \times \hat{X}$, quand on munit $\hat{X}$ de la structure $\mathcal{U}_1$; pour tout $a > 0$, il existe donc un entourage V de la structure $\mathcal{U}_1$ tel que, pour tout couple $(x, y) \in V$, on ait

$$
|\tilde{f}_i(x, y) - \tilde{f}_i(x, x)| \leq a,\text{ c’est-à-dire (puisque } \tilde{f}_i(x, x) = 0\text{)}\ V \subset \frac{1}{\tilde{f}_i}((0, a)) ;
$$

tout entourage de la structure $\mathcal{U}_2$ est donc un entourage de la structure $\mathcal{U}_1$. D’autre part, $\mathcal{U}_1$ et $\mathcal{U}_2$ induisent sur X la *même* structure uniforme $\mathcal{U}$. Comme $\hat{X}$ est *complet* pour $\mathcal{U}_1$, il s’ensuit que $\mathcal{U}_1$ et $\mathcal{U}_2$ sont *identiques*, en vertu de II, p. 23, prop. 14.

### 4. Construction d’une famille d’écarts définissant une structure uniforme

L’intérêt du mode de définition d’une structure uniforme par une famille d’écarts réside dans le fait qu’il permet d’obtenir *toutes les structures uniformes*. De façon précise:

#### Théorème 1 {#top-ix-s1-thm-1 .statement}

*Étant donnée une structure uniforme $\mathcal{U}$ sur un ensemble X, il existe une famille d’écarts sur X telle que la structure uniforme définie par cette famille soit identique à $\mathcal{U}$.*

Pour tout entourage V de la structure uniforme $\mathcal{U}$, définissons par récurrence une suite d’entourages symétriques $(\mathbf{U}_n)$ telle que $\mathbf{U}_1 \subset V$, et $\mathbf{U}_{n+1}^2 \subset \mathbf{U}_n$ quel que soit $n \geqslant 1$; la suite $(\mathbf{U}_n)$ est un système fondamental d’entourages d’une structure uniforme $\mathcal{U}_V$ moins fine que $\mathcal{U}$; en outre, il est clair que $\mathcal{U}$ est la *borne supérieure* de toutes les structures $\mathcal{U}_V$, lorsque V parcourt le filtre des entourages de $\mathcal{U}$. Le th. 1 sera donc une conséquence de la proposition suivante:

#### Proposition 2 {#top-ix-s1-prop-2 .statement}

*Si une structure uniforme $\mathcal{U}$ sur $X$ possède un système fondamental dénombrable d’entourages, il existe un écart $f$ sur $X$ tel que $\mathcal{U}$ soit identique à la structure uniforme définie par $f$.*

Soit $(V_n)$ un système fondamental dénombrable d’entourages de $\mathcal{U}$; définissons par récurrence une suite $(\mathbf{U}_n)$ d’entourages symétriques de la structure $\mathcal{U}$ tels que $\mathbf{U}_1 \subset V_1$, et
$$
\mathbf{U}_{n+1}^3 \subset \mathbf{U}_n \cap V_n \quad \text{pour } n \geqslant 1.
$$
Il est clair que $(\mathbf{U}_n)$ est encore un système fondamental d’entourages de $\mathcal{U}$, et on a en particulier $\mathbf{U}_{n+1}^3 \subset \mathbf{U}_n$ pour $n \geqslant 1$. Définissons comme suit une fonction numérique $g$ dans $X \times X$: $g(x, y) = 0$ si $(x, y) \in \mathbf{U}_n$ pour tout $n$; $g(x, y) = 2^{-k}$ si $(x, y) \in \mathbf{U}_n$ pour $1 \leqslant n \leqslant k$, mais $(x, y) \notin \mathbf{U}_{k+1}$; $g(x, y) = 1$ si $(x, y) \notin \mathbf{U}_1$. La fonction $g$ est symétrique, positive, et on a $g(x, x) = 0$ pour tout $x \in X$. Posons
$$
f(x, y) = \inf \sum_{i=0}^{p-1} g(z_i, z_{i+1})
$$
la borne inférieure étant prise sur l’ensemble de toutes les suites finies $(z_i)_{0 \leqslant i \leqslant p}$ ($p$ arbitraire) telles que $z_0 = x$ et $z_p = y$. Nous allons montrer que $f$ est un écart qui satisfait aux inégalités
$$
\frac{1}{2} g(x, y) \leqslant f(x, y) \leqslant g(x, y).
$$
En effet, de la définition de $f$ résulte aussitôt que $f$ satisfait à l’inégalité du triangle, et est symétrique et positive; la seconde inégalité (2) étant évidente, prouve que $f(x, x) = 0$ pour tout $x \in X$, donc que $f$ est un écart. Pour démontrer la première inégalité (2), montrons, par récurrence sur $p$, que pour toute suite finie $(z_i)_{0 \leqslant i \leqslant p}$ de $p + 1$ points de $X$, on a
$$
\sum_{i=0}^{p-1} g(z_i, z_{i+1}) \geqslant \frac{1}{2} g(z_0, z_p).
$$
L’inégalité est évidente si $p = 1$. Posons $a = \sum_{i=0}^{p-1} g(z_i, z_{i+1})$; l’inégalité (3) est vraie si $a \geqslant \frac{1}{2}$, puisque $g(z_0, z_p) \leqslant 1$. Supposons donc $a < \frac{1}{2}$; soit $h$ le plus grand des indices $q$ tels que
$$
\sum_{i<q} g(z_i, z_{i+1}) \leqslant \frac{a}{2};
$$

on a donc

$$
\sum_{i<h} g(z_i, z_{i+1}) \leq \frac{a}{2} \quad \text{et} \quad \sum_{i<h+1} g(z_i, z_{i+1}) > \frac{a}{2},
$$

d’où

$$
\sum_{i>h} g(z_i, z_{i+1}) \leq \frac{a}{2}.
$$

Par l’hypothèse de récurrence, on a $g(z_0, z_h) \leq a, g(z_{h+1}, z_p) \leq a$; d’autre part, on a évidemment $g(z_h, z_{h+1}) \leq a$. Soit $k$ le plus petit entier $> 0$ tel que $2^{-k} \leq a$; on a $k \geq 2$, et $(z_0, z_h) \in U_k, (z_h, z_{h+1}) \in U_k,$ et $(z_{h+1}, z_0) \in U_k$ d’après la définition de $g$; donc $(z_0, z_p) \in U_k \subset U_{k-1}$, ce qui entraîne $g(z_0, z_p) \leq 2^{1-k} \leq 2a$.

Cela étant, les inégalités (2) montrent que, pour tout $a > 0$, l’ensemble $f^{-1}([0, a])$ contient $U_k$ pour tout indice $k$ tel que $2^{-k} < a$, et inversement que tout $U_k$ contient l’ensemble $f^{-1}([0, 2^{-k-1}])$; les ensembles $f^{-1}([0, a])$ forment donc un système fondamental d’entourages de la structure $\mathcal{U}$.

C.Q.F.D.

#### Remarque {#top-ix-s1-n4-rem-1 .statement}

Une structure uniforme $\mathcal{U}$ sur $X$ est définie par la famille $\Phi$ de tous les écarts sur $X$ qui sont uniformément continus dans $X \times X$. En effet, il est clair que la structure uniforme définie par la famille $\Phi$ est moins fine que $\mathcal{U}$; d’autre part, le th. 1 prouve qu’il existe une sous-famille de $\Phi$ qui définit la structure uniforme $\mathcal{U}$, donc la structure uniforme définie par $\Phi$ est plus fine que $\mathcal{U}$, ce qui achève de montrer qu’elle est identique à $\mathcal{U}$.

### 5. Espaces uniformisables

Dans II, p. 27, nous avons posé le problème de la caractérisation des espaces topologiques uniformisables; la solution en est donnée par le th. suivant:

#### Théorème 2 {#top-ix-s1-thm-2 .statement}

Pour qu’un espace topologique $X$ soit uniformisable, il faut et il suffit qu’il vérifie l’axiome suivant:
(OIV) Quels que soient le point $x_0 \in X$ et le voisinage $V$ de $x_0$, il existe une fonction numérique continue dans $X$, prenant ses valeurs dans $[0, 1]$, égale à 0 au point $x_0$ et à 1 dans $CV$.

La condition est nécessaire. En effet, s’il existe une structure uniforme compatible avec la topologie de $X$, cette structure peut, d’après le th. 1 (IX, p. 5), être définie par une famille $(f_i)$ d’écarts sur $X$ et on peut toujours supposer que cette famille est saturée (IX, p. 4). D’après la définition des entourages de la structure uniforme définie par une telle famille d’écarts, il existe un écart $f_\alpha$ de la famille $(f_i)$, et un nombre $a > 0$, tels que $f_\alpha(x_0, x) \geq a$ pour tout $x \in CV$; il en résulte que la fonction $g(x) = \inf(1, (1/a)f_\alpha(x_0, x))$ remplit toutes les conditions énoncées dans (OIV).

La condition est suffisante. En effet, soit $\Phi$ l’ensemble des applications continues de $X$ dans $[0, 1]$. L’axiome (OIV) prouve que la structure uniforme la moins fine rendant uniformément continues les fonctions appartenant à $\Phi$ est compatible avec la topologie de $X$ (II, p. 8, corollaire).

#### Définition 4 {#top-ix-s1-def-4 .statement}

On dit qu’un espace topologique est complètement régulier s’il est uniformisable et séparé.

Il revient au même, d’après le th. 2, de dire qu’un espace est complètement régulier s’il satisfait aux axiomes (H) et (O_{IV}).

#### Remarque {#top-ix-s1-n5-rem-1 .statement}

L’axiome (O_{IV}) entraîne (O_{III}) (cf. I, p. 56, car si V est un voisinage de $x_0$, et $f$ une fonction numérique continue dans $X$, à valeurs dans $(0, 1)$, telle que $f(x_0) = 0, f(x) = 1$ pour tout $x \in \mathcal{V}$, l’ensemble $f^{-1}([0, \frac{1}{2}])$ est un voisinage fermé de $x_0$ contenu dans V. En particulier, tout espace complètement régulier est régulier (ce qui justifie la terminologie). On peut par contre donner des exemples d’espaces réguliers qui ne sont pas complètement réguliers (IX, p. 85, exerc. 8), ce qui montre que (O_{III}) n’entraîne pas (O_{IV}).

On sait (II, p. 27, th. 1) que tout espace compact est complètement régulier, et par suite aussi tout sous-espace d’un espace compact. Nous pouvons maintenant compléter cette proposition en démontrant sa réciproque ; autrement dit :

#### Proposition 3 {#top-ix-s1-prop-3 .statement}

Pour qu’un espace topologique $X$ soit complètement régulier, il faut et il suffit qu’il soit homéomorphe à un sous-espace d’un espace compact.

Reprenons en effet la structure uniforme la moins fine sur $X$ rendant uniformément continues toutes les applications continues de $X$ dans $(0, 1)$; nous avons utilisé cette structure dans la démonstration du th. 2, et vu qu’elle est compatible avec la topologie de $X$ si $X$ est uniformisable. Si en outre $X$ est séparé, cette structure uniforme est une structure d’espace précompact, en vertu de la compacité de l’intervalle $(0, 1)$ et de la prop. 3 de II, p. 31. Le complété de $X$ pour cette structure est donc compact, d’où la proposition.

On peut encore dire qu’un espace complètement régulier peut être plongé dans un espace compact; il est souvent commode de présenter ce résultat de la façon suivante :

Appelons, de façon générale, cube un espace topologique $I^L$, produit d’une famille d’espaces topologiques identiques à un intervalle compact I de $\mathbf{R}$, et ayant pour ensemble d’indices un ensemble L quelconque (si L est fini et a $n$ éléments, on retrouve la notion de cube fermé à $n$ dimensions définie dans VI, p. 1); un cube est un espace compact (I, p. 63, th. 3).

#### Proposition 4 {#top-ix-s1-prop-4 .statement}

Si un espace topologique $X$ est complètement régulier, il est homéomorphe à un sous-espace d’un cube.

Désignons en effet par $(f_\lambda)_{\lambda \in L}$ la famille de toutes les applications continues de $X$ dans $I = (0, 1)$, et considérons l’application $x \mapsto (f_\lambda(x))$ de $X$ dans $I^L$, que nous désignerons par g. D’après les axiomes (H) et (O_{IV}), pour tout couple de points distincts $x, y$ de $X$, il existe un indice $\lambda$ tel que $f_\lambda(x) \neq f_\lambda(y)$, donc g est une application injective de $X$ dans $I^L$. En outre, il est immédiat que g est un isomorphisme de la structure uniforme la moins fine rendant uniformément continues les f_\lambda, sur la structure uniforme induite sur g(X) par la structure uniforme (produit) de I^L; a fortiori, g est un homéomorphisme de X sur g(X).

#### Définition 5 {#top-ix-s1-def-5 .statement}

Étant donné un ensemble X, on dit qu’un ensemble H d’applications de X dans un ensemble Y sépare les éléments d’une partie A de X (ou est un ensemble séparant pour les éléments de A) si, quels que soient les éléments distincts x, y de A, il existe une fonction f \in H telle que f(x) \neq f(y).

#### Proposition 5 {#top-ix-s1-prop-5 .statement}

Soient X un espace compact, H un ensemble de fonctions numériques continues dans X et séparant les points de X. Pour toute partie finie K de H et tout réel $\varepsilon > 0$, soit $U_{K,\varepsilon}$ l’ensemble des couples $(x, y) \in X \times X$ tels que $|f(x) - f(y)| \leq \varepsilon$ pour toute application $f \in K$. Les ensembles $U_{K,\varepsilon}$ forment un système fondamental d’entourages de la structure uniforme de X.

En effet, soit $\varphi : X \to \mathbf{R}^H$ l’application $x \mapsto (f(x))_{f \in H}$; elle est évidemment continue; elle est injective par hypothèse, et comme $\mathbf{R}^H$ est séparé, $\varphi$ est un homéomorphisme de X sur un sous-espace compact de $\mathbf{R}^H$, et par suite aussi un isomorphisme pour les structures uniformes de X et de $\varphi(X)$ (II, p. 27, th. 1). L’assertion résulte alors de la définition des entourages dans l’espace produit $\mathbf{R}^H$ (II, p. 8).

### 6. Compactifié de Stone-Čech

#### Proposition 6 {#top-ix-s1-prop-6 .statement}

Soit X un espace topologique; il existe un espace compact Z et une application continue $f : X \to Z$ ayant la propriété suivante: pour toute application continue g de X dans un espace compact Y, il existe une application continue et une seule $h : Z \to Y$ telle que $g = h \circ f$. En outre, si $Z_1$ est un espace compact et $f_1$ une application continue de X dans $Z_1$ ayant les mêmes propriétés que Z et f, il existe un homéomorphisme unique u de Z sur $Z_1$ tel que $f_1 = u \circ f$.

En d’autres termes, le couple $(Z, f)$ est solution du problème d’application universelle (E, IV, p. 22) où $\Sigma$ est la structure d’espace compact, les morphismes étant les applications continues, ainsi que les $\alpha$-applications.

En effet, considérons la famille $(f_\lambda)_{\lambda \in L}$ de toutes les applications continues de X dans $I = [0, 1]$, et soit $\varphi$ l’application continue $x \mapsto (f_\lambda(x))_{\lambda \in L}$ de X dans $I^L$; alors l’adhérence $Z = \overline{\varphi(X)}$ dans $I^L$ est compacte; notons $f$ l’application continue de X dans Z déduite de $\varphi$, et montrons que Z et f répondent à la question. Il suffit de prouver l’existence de h lorsque $Y = I$; en effet, tout espace compact Y peut être identifié à un sous-espace fermé de $I^A$ pour un ensemble A convenable (IX, p. 8, prop. 4); si, pour tout $\alpha \in A$, il existe une application continue $h_\alpha$ de Z dans I telle que $\mathrm{pr}_\alpha \circ g = h_\alpha \circ f$, on aura donc
$$
(h_\alpha(f(x))) = (\mathrm{pr}_\alpha(g(x))) = g(x) \in Y
$$
pour tout $x \in X$; l’application $h = (h_\alpha)$ de Z dans $I^A$ est donc telle que $h(z) \in Y$ pour tout $z \in \varphi(X)$; comme $h$ est continue et $\varphi(X)$ partout dense dans $Z$, on aura bien $h(Z) \subset Y$ (I, p. 9, th. 1) donc la factorisation $g = f \circ h$ aura la propriété voulue.

Supposons donc $Y = I$; alors par définition, si $g : X \to I$ est continue, il existe un indice $\lambda \in L$ tel que $g = f_\lambda$, et on a donc la factorisation $g = (\mathrm{pr}_\lambda | Z) \circ f$. L’unicité de $h$ résulte de ce que $Y$ est séparé et de ce que $h$ est déterminé de façon unique dans $\varphi(X)$, qui est partout dense dans $Z$. L’unicité du couple $(Z, f)$ à isomorphisme unique près est un résultat général sur les problèmes d’application universelle (E, IV, p. 23).

#### Corollaire {#top-ix-s1-n6-cor-1 .statement}

*Pour que $f$ soit injective, il faut et il suffit que l’ensemble des applications continues de $X$ dans $I = (0, 1)$ sépare les points de $X$. Pour que $f$ soit un homéomorphisme de $X$ sur $f(X)$, il faut et il suffit que $X$ soit complètement régulier.*

La première assertion résulte aussitôt de la façon dont $f$ a été définie dans la démonstration de la prop. 6. La seconde résulte des prop. 3 et 4 (IX, p. 8).

L’espace compact $Z$ défini dans la prop. 6 est appelé *compactifié de Stone-Čech* de $X$ et noté parfois $\beta X$.

### 7. Fonctions semi-continues sur un espace uniformisable

Dans IV, p. 31, corollaire, on a vu que, dans un espace topologique, l’enveloppe supérieure d’une famille de fonctions numériques continues est une fonction semi-continue inférieurement. Dans un espace *uniformisable*, on a en outre une *réciproque* de cette proposition:

#### Proposition 7 {#top-ix-s1-prop-7 .statement}

*Pour que toute fonction numérique $f$ (finie ou non) semi-continue inférieurement dans un espace topologique $X$, soit l’enveloppe supérieure des fonctions numériques (finies ou non) continues dans $X$ et $\leq f$, il faut et il suffit que $X$ soit uniformisable.*

La condition est *nécessaire*: en effet, soient $x_0$ un point quelconque de $X$, et $V$ un voisinage ouvert quelconque de $x_0$; la fonction caractéristique $\varphi_V$ de l’ensemble $V$ est semi-continue inférieurement (IV, p. 29, corollaire); par hypothèse, il existe donc une fonction numérique $g$ continue dans $X$, telle que $g \leq \varphi_V$ et $g(x_0) = a > 0$; la fonction continue $\inf(1, (1/a)g^+)$ prend ses valeurs dans $(0, 1)$, est égale à 0 dans $\mathbf{C}V$ et à 1 au point $x_0$; donc (IX, p. 7, th. 2), $X$ est uniformisable.

La condition est *suffisante*. Considérons d’abord le cas où $f$ prend ses valeurs dans $(-1, +1)$. Il faut montrer que, pour tout $x_0 \in X$ et tout nombre $a < f(x_0)$, il existe une fonction numérique $g$, continue dans $X$, telle que $g \leq f$ et $g(x_0) \geq a$. Si $a \leq -1$, il suffit de prendre pour $g$ la constante $-1$. Si $-1 < a < f(x_0)$, il existe un voisinage $V$ de $x_0$ tel que $f(x) \geq a$ pour tout $x \in V$. Comme $X$ est uniformisable, il existe une fonction numérique $h$, continue dans $X$, à valeurs dans (0, 1), et telle que $h(x_0) = 0$ et $h(x) = 1$ pour $x \in \mathbf{C}V$. Il suffit alors de prendre $g(x) = a - (a + 1)h(x)$ pour avoir une fonction continue répondant aux conditions posées. On notera que cette fonction prend ses valeurs dans $(-1, +1)$.

Le cas général se déduit du cas précédent par transport de structure : il existe en effet un homéomorphisme strictement croissant de $(-1, +1)$ sur $\overline{\mathbf{R}}$ (IV, p. 14, prop. 2).

#### Remarque {#top-ix-s1-n7-rem-1 .statement}

Dans la démonstration précédente, on voit que la fonction $g$ ne prend pas la valeur $+1$. Par transport de structure, on en déduit que toute fonction numérique $f$, semi-continue inférieurement dans l’espace uniformisable E, est enveloppe supérieure des fonctions numériques $g \leq f$, continues dans E et ne prenant pas la valeur $+\infty$.

## EXERCICES {#top-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
